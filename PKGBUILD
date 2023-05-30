pkgname=msm-modem
pkgver=1.0
pkgrel=1
pkgdesc="Script and service files for Qualcomm QMI modem"
arch=('any')
depends=('rmtfs')
url="https://example.com"
license=('MIT')
source=('setup-modem.sh'
'setup-msm-modem.conf'
'setup-msm-modem.service')

package() {
    # Install the script
    install -Dm755 "${srcdir}/setup-modem.sh" "${pkgdir}/usr/bin/setup-modem.sh"

    # Install the service file
    install -Dm644 "${srcdir}/setup-msm-modem.service" "${pkgdir}/usr/lib/systemd/system/setup-msm-modem.service"

    # Install the configuration file
    install -Dm644 "${srcdir}/setup-msm-modem.conf" "${pkgdir}/etc//etc/systemd/system/setup-msm-modem.d/setup-msm-modem.conf"
}

sha256sums=('4d0c292cc877f4dc4c4d8d64d0883637c1375ca33234b757a0140a2f29d1a6e2'
            'a77ba16ddf5b0afafc115ae2746a1691d510112e0be9520d7086adaa88958173'
            '9cd44c173253fa10fdd77adebc829488e04383927db3d7917a675be9d2f0c3c0')

