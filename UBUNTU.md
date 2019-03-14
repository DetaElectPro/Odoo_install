# Odoo install
شرح التثبيت علي نظام اوبنتو لينكس

## الخطوة الـ1
```
    sudo apt-get update
    sudo apt-get -y upgrade
    sudo apt-get install python3-pip
```
### الخطوة الـ2
 تثبيت الاعتمادات الخاصة بـ
  pip3
```
pip3 install Babel decorator docutils ebaysdk feedparser gevent greenlet html2text Jinja2 lxml Mako MarkupSafe mock num2words ofxparse passlib Pillow psutil psycogreen psycopg2 pydot pyparsing PyPDF2 pyserial python-dateutil python-openid pytz pyusb PyYAML qrcode reportlab requests six suds-jurko vatnumber vobject Werkzeug XlsxWriter xlwt xlrd
```
#### الخطوة الـ3
*يفضل استخدام 
nvm node js
```
sudo apt-get install -y npm

sudo ln -s /usr/bin/nodejs /usr/bin/node

sudo npm install -g less less-plugin-clean-css

sudo apt-get install node-less
```

###الخطوة الـ4.
اعداد قاعدة البيانات
"postgresql".

```
sudo apt-get install python-software-properties

sudo vim /etc/apt/sources.list.d/pgdg.list


add a line for the repository



deb http://apt.postgresql.org/pub/repos/apt/ xenial-pgdg main



wget --quiet -O - https://www.postgresql.org/media/keys/ACCC4CF8.asc | sudo apt-key add -



sudo apt-get update


sudo apt-get install postgresql-9.6
```

### الخطوة الـ5
اضافة اسم المستخدم للاودو و قاعدة البيانات لستخدامهم في ما بعدن دون الحاجة الي صلاحيات الجزر.
```
sudo su postgres


cd


createuser -s odoo

createuser -s ubuntu_user_name

exit

sudo adduser --system --home=/opt/odoo --group odoo
```
## الخطوة الـ6
تنزيل و تثبيت الاودو 11.
```
cd /opt/odoo

sudo apt-get install git


sudo su - odoo -s /bin/bash


git clone https://www.github.com/odoo/odoo --depth 1 --branch 11.0 –single-branch

exit
```