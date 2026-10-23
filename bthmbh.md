代发 wailian999

awk -F, '$3 > 100 {print $1}' a.csv
来源：http://www.52xcode.cn/Article/details/gt3nqxcjspy.html

[R50] awk 求和
来源：http://www.52xcode.cn/Article/details/gt3rpknicgr.html

awk '{s += $2} END {print s}' a.txt
来源：http://www.ydjk.org.cn/Article/details/gt3osavlnup.html

[R51] 排序去重取前几
来源：http://www.ydjk.org.cn/Article/details/gt3bnaegrag.html

sort a.txt | uniq -c | sort -rn | head
来源：http://www.ydjk.org.cn/Article/details/gt3trvlfwaw.html

[R52] 统计行数
来源：http://www.ydjk.org.cn/Article/details/gt3tybzrzkm.html

wc -l a.txt
来源：http://www.52xcode.cn/Article/details/gt3ejvghsds.html

[R53] 查看文件头与实时尾
来源：http://www.ydjk.org.cn/Article/details/gt3fzexgbur.html

head -n 20 a.txt;  tail -f -n 100 app.log
来源：http://www.52xcode.cn/Article/details/gt3wckwvpqj.html

[R54] 比较两个文件
来源：http://www.52xcode.cn/Article/details/gt3abialwwd.html

diff a.txt b.txt
来源：http://www.52xcode.cn/Article/details/gt3miqujiio.html

[R55] 压缩与解压
来源：http://www.52xcode.cn/Article/details/gt3paghfljd.html

tar -czf x.tar.gz dir/;  tar -xzf x.tar.gz
来源：http://www.ydjk.org.cn/Article/details/gt3kdweqasy.html

[R56] 远程拷贝
来源：http://www.ydjk.org.cn/Article/details/gt3qdkrukxy.html

scp file user@host:/path/
来源：http://www.52xcode.cn/Article/details/gt3fmnfgqcc.html

[R57] 远程执行命令
来源：http://www.52xcode.cn/Article/details/gt3udjfymwy.html

ssh user@host 'uptime'
来源：http://www.ydjk.org.cn/Article/details/gt3qqjbbklt.html

[R58] 下载文件
来源：http://www.ydjk.org.cn/Article/details/gt3sqpqakby.html

curl -LO https://a.com/file.zip;  wget https://a.com/file.zip
来源：http://www.52xcode.cn/Article/details/gt3rkjtugrf.html

[R59] 发 POST JSON
来源：http://www.ydjk.org.cn/Article/details/gt3wfcrnlpl.html

curl -X POST -H 'Content-Type: application/json' -d '{"a":1}' https://api.example.com
来源：http://www.52xcode.cn/Article/details/gt3ceufyvxi.html

[R60] 只看 HTTP 状态码
来源：http://www.52xcode.cn/Article/details/gt3prwvbqdt.html

curl -s -o /dev/null -w "%{http_code}\n" https://a.com
来源：http://www.ydjk.org.cn/Article/details/gt3onbgvunw.html

[R61] 磁盘占用
来源：http://www.52xcode.cn/Article/details/gt3ltbeqqtg.html

df -h;  du -sh *
来源：http://www.52xcode.cn/Article/details/gt3dewqeywm.html

[R62] 找最占空间的文件
来源：http://www.52xcode.cn/Article/details/gt3dldhpnzl.html

du -ah . | sort -rh | head -10
来源：http://www.ydjk.org.cn/Article/details/gt3zkdwonrj.html

[R63] 内存与进程
来源：http://www.ydjk.org.cn/Article/details/gt3jlonryux.html

free -h;  ps aux | grep nginx
来源：http://www.52xcode.cn/Article/details/gt3jcrbhdci.html

[R64] 结束进程
来源：http://www.ydjk.org.cn/Article/details/gt3mqlovbrk.html

kill -9 $(pgrep -f app.py)
来源：http://www.52xcode.cn/Article/details/gt3crorwius.html

[R65] 查看端口占用
来源：http://www.52xcode.cn/Article/details/gt3souvvrom.html

ss -tlnp | grep 8080;  lsof -i:8080
来源：http://www.52xcode.cn/Article/details/gt3wuigkxte.html

[R66] 定时任务
来源：http://www.52xcode.cn/Article/details/gt3nkgymxqq.html

crontab -e;  crontab -l
来源：http://www.52xcode.cn/Article/details/gt3sfmpfovi.html

[R67] 生成随机十六进制串
来源：http://www.52xcode.cn/Article/details/gt3cdqvezfq.html

openssl rand -hex 16
来源：http://www.ydjk.org.cn/Article/details/gt3vqnpjmnx.html

[R68] 计算文件校验值
来源：http://www.52xcode.cn/Article/details/gt3mypnqslj.html

sha256sum a.txt;  md5sum a.txt
来源：http://www.ydjk.org.cn/Article/details/gt3mermhbvc.html

[R69] 生成随机密码
来源：http://www.ydjk.org.cn/Article/details/gt3ifztajpk.html

head -c 16 /dev/urandom | base64
来源：http://www.52xcode.cn/Article/details/gt3bmqpjxdx.html

[R70] 时间戳与互转
来源：http://www.52xcode.cn/Article/details/gt3npixwkxc.html

date +%s;  date -d @1700000000
来源：http://www.ydjk.org.cn/Article/details/gt3durkwuad.html

[R71] 日期格式化
来源：http://www.ydjk.org.cn/Article/details/gt3nubmukab.html

date +"%Y-%m-%d %H:%M:%S"
来源：http://www.ydjk.org.cn/Article/details/gt3xyjsguxd.html

[R72] 等待端口就绪
来源：http://www.52xcode.cn/Article/details/gt3ttbjuxku.html

until nc -z localhost 3306; do sleep 1; done
来源：http://www.ydjk.org.cn/Article/details/gt3sqyynmqq.html

[R73] 分割大日志
来源：http://www.ydjk.org.cn/Article/details/gt3gwclwouo.html

split -l 1000 big.log part_
来源：http://www.52xcode.cn/Article/details/gt3wnoclrjf.html

[R74] 批量重命名
来源：http://www.52xcode.cn/Article/details/gt3vuigqrbt.html

for f in *.jpeg; do mv "$f" "${f%.jpeg}.jpg"; done
来源：http://www.52xcode.cn/Article/details/gt3erckiruv.html

[R75] 导出环境变量
来源：http://www.ydjk.org.cn/Article/details/gt3qaebniuo.html

export PATH="$HOME/bin:$PATH"
来源：http://www.ydjk.org.cn/Article/details/gt3unftqzzn.html

[R76] 使用临时文件
来源：http://www.ydjk.org.cn/Article/details/gt3kqruugwj.html

tmp=$(mktemp); trap 'rm -f "$tmp"' EXIT
来源：http://www.52xcode.cn/Article/details/gt3xmdvwbea.html

[R77] 读取用户输入
来源：http://www.52xcode.cn/Article/details/gt3ihtdklpi.html

read -rp "请输入: " ans
来源：http://www.ydjk.org.cn/Article/details/gt3bzrbynct.html

[R78] 交互式菜单
来源：http://www.ydjk.org.cn/Article/details/gt3pouuqejm.html

select opt in a b c; do echo "$opt"; break; done
来源：http://www.ydjk.org.cn/Article/details/gt3gdyvsfad.html

[R79] 解析命令行选项
来源：http://www.52xcode.cn/Article/details/gt3rohrilky.html

while getopts "v:f:" o; do case $o in v) V=$OPTARG ;; f) F=$OPTARG ;; esac; done
来源：http://www.ydjk.org.cn/Article/details/gt3ncozvsqy.html

[R80] 查看脚本执行耗时
来源：http://www.52xcode.cn/Article/details/gt3xdessucl.html

time ./run.sh
来源：http://www.ydjk.org.cn/Article/details/gt3hchanwkk.html

================================================================================
来源：http://www.52xcode.cn/Article/details/gt3phlgmwij.html

S. C / C++ 专题
来源：http://www.ydjk.org.cn/Article/details/gt3pntzdhkh.html

================================================================================
来源：http://www.52xcode.cn/Article/details/gt3qlexdstk.html

[S01] C：Hello World
来源：http://www.ydjk.org.cn/Article/details/gt3kvbdoazm.html

#include <stdio.h>
来源：http://www.ydjk.org.cn/Article/details/gt3lowwatxe.html

int main(void) { printf("Hello\n"); return 0; }
来源：http://www.ydjk.org.cn/Article/details/gt3wbzgbfqo.html

[S02] C：变量与格式化输出
来源：http://www.ydjk.org.cn/Article/details/gt3fhfrnqlr.html

int a = 10; printf("%d\n", a);
来源：http://www.ydjk.org.cn/Article/details/gt3kdlsyrvq.html

[S03] C：读入整数
来源：http://www.52xcode.cn/Article/details/gt3rtyofkyg.html

int x; scanf("%d", &x);
来源：http://www.52xcode.cn/Article/details/gt3tagbdsvp.html

[S04] C：字符串复制
来源：http://www.ydjk.org.cn/Article/details/gt3mgoymyzw.html

char dst[32]; strcpy(dst, "hi");
来源：http://www.ydjk.org.cn/Article/details/gt3zlsehulp.html

[S05] C：字符串长度
来源：http://www.52xcode.cn/Article/details/gt3ahebvsbu.html

strlen(s)
来源：http://www.ydjk.org.cn/Article/details/gt3ruivbaqv.html

[S06] C：字符串比较
来源：http://www.52xcode.cn/Article/details/gt3kjtbkyvw.html

strcmp(a, b) == 0
来源：http://www.52xcode.cn/Article/details/gt3qsofxdld.html

[S07] C：数组遍历求和
来源：http://www.52xcode.cn/Article/details/gt3hrsuzjty.html

for (int i = 0; i < n; i++) sum += a[i];
来源：http://www.ydjk.org.cn/Article/details/gt3aoqpwxrl.html

[S08] C：动态内存分配与释放
来源：http://www.52xcode.cn/Article/details/gt3baadqtpq.html

int *p = malloc(sizeof(int) * n); ... free(p);
来源：http://www.ydjk.org.cn/Article/details/gt3reeuyanu.html

[S09] C：结构体定义与初始化
来源：http://www.52xcode.cn/Article/details/gt3trrpsuwa.html

struct Point { int x, y; };  struct Point p = {1, 2};
来源：http://www.52xcode.cn/Article/details/gt3szuzlfjo.html

[S10] C：指针与解引用
来源：http://www.52xcode.cn/Article/details/gt3mqdsxyqr.html

int *p = &a;  *p = 5;
来源：http://www.ydjk.org.cn/Article/details/gt3qbfpmuwj.html

[S11] C：逐行读文件
来源：http://www.ydjk.org.cn/Article/details/gt3mohdukdo.html

FILE *f = fopen("a.txt", "r");
来源：http://www.ydjk.org.cn/Article/details/gt3ksojfewm.html

while (fgets(buf, sizeof buf, f)) { }
来源：http://www.ydjk.org.cn/Article/details/gt3miwvvceg.html

fclose(f);
来源：http://www.ydjk.org.cn/Article/details/gt3nscpxami.html

[S12] C：写文件
来源：http://www.ydjk.org.cn/Article/details/gt3ywfablvg.html

FILE *f = fopen("a.txt", "w");  fprintf(f, "hi\n");  fclose(f);
来源：http://www.52xcode.cn/Article/details/gt3czjhfocy.html

[S13] C：宏定义
来源：http://www.ydjk.org.cn/Article/details/gt3luhhdtbc.html

#define MAX(a, b) ((a) > (b) ? (a) : (b))
来源：http://www.ydjk.org.cn/Article/details/gt3etelghjv.html

[S14] C：枚举
来源：http://www.ydjk.org.cn/Article/details/gt3ziysoqty.html

enum Color { RED, GREEN, BLUE };
来源：http://www.52xcode.cn/Article/details/gt3ybvukcud.html

[S15] C：类型转换
来源：http://www.52xcode.cn/Article/details/gt3xitijodx.html

(double) a / b
来源：http://www.52xcode.cn/Article/details/gt3zekcrnuq.html

[S16] C：位操作置位
来源：http://www.ydjk.org.cn/Article/details/gt3pwkpugsy.html

x |= (1 << 3);
来源：http://www.ydjk.org.cn/Article/details/gt3myzizzbt.html

[S17] C：安全拼接字符串
来源：http://www.52xcode.cn/Article/details/gt3pcoqqoox.html

snprintf(buf, sizeof buf, "%s%s", a, b);
来源：http://www.52xcode.cn/Article/details/gt3gkxcexog.html

[S18] C：命令行参数
来源：http://www.ydjk.org.cn/Article/details/gt3slevgrgw.html

int main(int argc, char **argv)
来源：http://www.52xcode.cn/Article/details/gt3mveskobc.html

[S19] C：快速排序
来源：http://www.52xcode.cn/Article/details/gt3ndelhnpr.html

qsort(a, n, sizeof(int), cmp);
来源：http://www.ydjk.org.cn/Article/details/gt3qrsahmgj.html

[S20] C：二分查找
来源：http://www.ydjk.org.cn/Article/details/gt3dcgqpflt.html

bsearch(&key, a, n, sizeof(int), cmp);
来源：http://www.52xcode.cn/Article/details/gt3mjdgomur.html

[S21] C：字符类别判断
来源：http://www.52xcode.cn/Article/details/gt3afpojeoc.html

isdigit(c);  isalpha(c);  isspace(c);
来源：http://www.52xcode.cn/Article/details/gt3oojlyiwe.html

[S22] C：字符串转数字
来源：http://www.52xcode.cn/Article/details/gt3mtkzjmec.html

atoi("42");  strtod("3.14", NULL);
来源：http://www.52xcode.cn/Article/details/gt3zdtgnfrb.html

[S23] C：随机数
来源：http://www.ydjk.org.cn/Article/details/gt3mbczsowy.html

srand(time(NULL));  int r = rand() % 100;
来源：http://www.52xcode.cn/Article/details/gt3zyghnrrr.html

[S24] C：获取本地时间
来源：http://www.52xcode.cn/Article/details/gt3tffopahs.html

time_t t = time(NULL);  struct tm *tm = localtime(&t);
来源：http://www.52xcode.cn/Article/details/gt3qxkxvzmw.html

[S25] C：内存拷贝
来源：http://www.ydjk.org.cn/Article/details/gt3bcruhtqw.html

memcpy(dst, src, n);
来源：http://www.52xcode.cn/Article/details/gt3puetpmil.html

[S26] C：内存清零
来源：http://www.ydjk.org.cn/Article/details/gt3ohuawcgm.html

memset(a, 0, sizeof a);
来源：http://www.52xcode.cn/Article/details/gt3sdacivgh.html

[S27] C：定义常量
来源：http://www.ydjk.org.cn/Article/details/gt3eshszasg.html

const double PI = 3.14159;
来源：http://www.ydjk.org.cn/Article/details/gt3jqdedknw.html

[S28] C：静态变量
来源：http://www.ydjk.org.cn/Article/details/gt3pkjgcnnp.html

static int counter = 0;
来源：http://www.ydjk.org.cn/Article/details/gt3gtgsglxn.html

[S29] C：变参函数
来源：http://www.52xcode.cn/Article/details/gt3xxneeodv.html

va_list ap; va_start(ap, fmt); vprintf(fmt, ap); va_end(ap);
来源：http://www.52xcode.cn/Article/details/gt3aeribcgw.html

[S30] C：头文件保护
来源：http://www.52xcode.cn/Article/details/gt3uzrtidll.html

#ifndef X_H
来源：http://www.52xcode.cn/Article/details/gt3ywmgcyid.html

#define X_H
来源：http://www.ydjk.org.cn/Article/details/gt3hdigvyeo.html

#endif
来源：http://www.ydjk.org.cn/Article/details/gt3puskxytb.html

[S31] C++：Hello World
来源：http://www.ydjk.org.cn/Article/details/gt3gvasdxer.html

#include <iostream>
来源：http://www.ydjk.org.cn/Article/details/gt3gjhhyizk.html

int main() { std::cout << "Hello\n"; }
来源：http://www.ydjk.org.cn/Article/details/gt3npmiakog.html

[S32] C++：字符串
来源：http://www.52xcode.cn/Article/details/gt3uzncufvk.html

std::string s = "hi";  s += "!";
来源：http://www.52xcode.cn/Article/details/gt3mtququkh.html

[S33] C++：vector 增删
来源：http://www.52xcode.cn/Article/details/gt3ejrbrqky.html

std::vector<int> v{1, 2, 3};  v.push_back(4);
来源：http://www.ydjk.org.cn/Article/details/gt3mdpydcsh.html

[S34] C++：遍历 vector
来源：http://www.52xcode.cn/Article/details/gt3hqieduak.html

for (auto &x : v) { std::cout << x; }
来源：http://www.ydjk.org.cn/Article/details/gt3vnqsnghs.html

[S35] C++：map
来源：http://www.ydjk.org.cn/Article/details/gt3ibsppaey.html

std::map<std::string, int> m;  m["a"] = 1;
来源：http://www.ydjk.org.cn/Article/details/gt3eammpsvt.html

[S36] C++：unordered_map
来源：http://www.52xcode.cn/Article/details/gt3vxnedtbc.html

std::unordered_map<std::string, int> m;  m["a"] = 1;
来源：http://www.ydjk.org.cn/Article/details/gt3pqyneeca.html

[S37] C++：set
来源：http://www.ydjk.org.cn/Article/details/gt3krieoefe.html

std::set<int> s{1, 2, 3};  s.insert(4);
来源：http://www.ydjk.org.cn/Article/details/gt3wytlwuvc.html

[S38] C++：排序
来源：http://www.52xcode.cn/Article/details/gt3hfgqoeqq.html

std::sort(v.begin(), v.end());
来源：http://www.52xcode.cn/Article/details/gt3uvbbmimg.html

[S39] C++：自定义比较器排序
来源：http://www.ydjk.org.cn/Article/details/gt3ypcotmsj.html

std::sort(v.begin(), v.end(), [](int a, int b) { return a > b; });
来源：http://www.52xcode.cn/Article/details/gt3avqwqrvx.html

[S40] C++：查找元素
来源：http://www.ydjk.org.cn/Article/details/gt3hktkmmyg.html

auto it = std::find(v.begin(), v.end(), 3);
来源：http://www.52xcode.cn/Article/details/gt3onvkddcc.html

[S41] C++：类与构造函数
来源：http://www.ydjk.org.cn/Article/details/gt3erjpmlwo.html

class A { public: A(int v) : x_(v) {} int get() const { return x_; } private: int x_; };
来源：http://www.ydjk.org.cn/Article/details/gt3vuyvzqvn.html

[S42] C++：继承与虚函数
来源：http://www.52xcode.cn/Article/details/gt3aantnejm.html

class B : public Base { public: void f() override {} };
来源：http://www.ydjk.org.cn/Article/details/gt3xbitshti.html

[S43] C++：智能指针
来源：http://www.ydjk.org.cn/Article/details/gt3zlzgnhhv.html

auto p = std::make_unique<int>(5);
来源：http://www.52xcode.cn/Article/details/gt3keypqwzx.html

[S44] C++：引用传参
来源：http://www.ydjk.org.cn/Article/details/gt3npzctaro.html

void inc(int &x) { ++x; }
来源：http://www.52xcode.cn/Article/details/gt3ngmspcmw.html

[S45] C++：lambda
来源：http://www.ydjk.org.cn/Article/details/gt3mkcbgogy.html

auto add = [](int a, int b) { return a + b; };
来源：http://www.52xcode.cn/Article/details/gt3ewqwcqfx.html

[S46] C++：函数模板
来源：http://www.ydjk.org.cn/Article/details/gt3zpqvoxbq.html

template <typename T> T maxv(T a, T b) { return a > b ? a : b; }
来源：http://www.ydjk.org.cn/Article/details/gt3qllxhqhz.html

[S47] C++：结构化绑定遍历
来源：http://www.52xcode.cn/Article/details/gt3vwobfwta.html

for (const auto &[k, v] : m) { std::cout << k << v; }
来源：http://www.ydjk.org.cn/Article/details/gt3mfnlytzy.html

[S48] C++：逐行读文件
来源：http://www.52xcode.cn/Article/details/gt3jihuffpe.html

std::ifstream in("a.txt");  std::string line;
来源：http://www.ydjk.org.cn/Article/details/gt3giswbnqh.html

while (std::getline(in, line)) { }
来源：http://www.ydjk.org.cn/Article/details/gt3yhsstilk.html

[S49] C++：写文件
来源：http://www.ydjk.org.cn/Article/details/gt3bkpmznho.html

std::ofstream out("a.txt");  out << "hi\n";
来源：http://www.ydjk.org.cn/Article/details/gt3yatxvjha.html

[S50] C++：格式化数字
来源：http://www.ydjk.org.cn/Article/details/gt3mcfmfiif.html

std::ostringstream os;  os << std::fixed << std::setprecision(2) << 3.14159;
来源：http://www.52xcode.cn/Article/details/gt3tvrehhgn.html

[S51] C++：显式类型转换
来源：http://www.52xcode.cn/Article/details/gt3wzdszczb.html

static_cast<double>(a) / b
来源：http://www.ydjk.org.cn/Article/details/gt3fxgjpjsm.html

[S52] C++：const 与 noexcept
来源：http://www.52xcode.cn/Article/details/gt3pbegetgj.html

int size() const noexcept { return n_; }
来源：http://www.52xcode.cn/Article/details/gt3wkznjxfw.html

[S53] C++：移动语义
来源：http://www.ydjk.org.cn/Article/details/gt3ziensoeo.html

std::vector<int> w = std::move(v);
来源：http://www.52xcode.cn/Article/details/gt3cvhefkiy.html

[S54] C++：异常处理
来源：http://www.52xcode.cn/Article/details/gt3ykaryohb.html

try { throw std::runtime_error("x"); } catch (const std::exception &e) { }
来源：http://www.52xcode.cn/Article/details/gt3irhojybz.html

[S55] C++：结构化绑定
来源：http://www.ydjk.org.cn/Article/details/gt3mnviogll.html

auto [a, b] = std::make_pair(1, 2);
来源：http://www.52xcode.cn/Article/details/gt3tlvpcclx.html

[S56] C++：optional
来源：http://www.52xcode.cn/Article/details/gt3lujhwief.html

std::optional<int> o = 5;  if (o) { int v = *o; }
来源：http://www.52xcode.cn/Article/details/gt3pcwrtlwk.html

[S57] C++：编译期常量
来源：http://www.ydjk.org.cn/Article/details/gt3kxobgjzc.html

constexpr int N = 10;
来源：http://www.ydjk.org.cn/Article/details/gt3ljvjhpmn.html

[S58] C++：命名空间
来源：http://www.52xcode.cn/Article/details/gt3jepdkcux.html

namespace ns { int f() { return 1; } }
来源：http://www.52xcode.cn/Article/details/gt3jtyxgszc.html

[S59] C++：静态断言
来源：http://www.ydjk.org.cn/Article/details/gt3ssghjbbj.html

static_assert(sizeof(int) == 4, "int 必须 4 字节");
来源：http://www.ydjk.org.cn/Article/details/gt3suvtjalm.html

[S60] C++：遍历并删除元素
来源：http://www.52xcode.cn/Article/details/gt3dxdobrer.html

v.erase(std::remove_if(v.begin(), v.end(), [](int x) { return x < 0; }), v.end());
来源：http://www.52xcode.cn/Article/details/gt3eygyiofd.html

================================================================================
来源：http://www.ydjk.org.cn/Article/details/gt3yeghvrbp.html

T. 其他语言补充（Kotlin / Swift / Lua / Perl / Scala）
来源：http://www.52xcode.cn/Article/details/gt3qcvbiluz.html

================================================================================
来源：http://www.ydjk.org.cn/Article/details/gt3henjzert.html

[T01] Kotlin：Hello World
来源：http://www.ydjk.org.cn/Article/details/gt3efzvghzt.html

println("Hello")
来源：http://www.52xcode.cn/Article/details/gt3qvpvohvt.html

[T02] Kotlin：变量
来源：http://www.52xcode.cn/Article/details/gt3vfymfmfe.html

val a = 1;  var b = 2        // val 只读，var 可变
来源：http://www.52xcode.cn/Article/details/gt3wfmfljhb.html

[T03] Kotlin：字符串模板
来源：http://www.ydjk.org.cn/Article/details/gt3nttxagpx.html

"值: $b"
来源：http://www.52xcode.cn/Article/details/gt3ktykgvji.html

[T04] Kotlin：空安全
来源：http://www.52xcode.cn/Article/details/gt3kpwllkei.html

val n: String? = null;  n?.length
来源：http://www.52xcode.cn/Article/details/gt3dcvgdxnu.html

[T05] Kotlin：when 表达式
来源：http://www.ydjk.org.cn/Article/details/gt3dhlkqwpq.html

val s = when (x) { 1 -> "一" else -> "其他" }   // 多分支时每个分支单独一行
来源：http://www.52xcode.cn/Article/details/gt3uavwgsfq.html

[T06] Kotlin：集合映射
来源：http://www.ydjk.org.cn/Article/details/gt3dtmrtxpb.html

listOf(1, 2, 3).map { it * 2 }
来源：http://www.ydjk.org.cn/Article/details/gt3olbscoso.html

[T07] Kotlin：集合过滤
来源：http://www.ydjk.org.cn/Article/details/gt3eqrkzeiw.html

listOf(1, 2, 3).filter { it > 1 }
来源：http://www.52xcode.cn/Article/details/gt3fubrhsat.html

[T08] Kotlin：数据类
来源：http://www.52xcode.cn/Article/details/gt3naidfbjg.html

data class User(val name: String, val age: Int)
来源：http://www.ydjk.org.cn/Article/details/gt3pfpqlnlc.html

[T09] Kotlin：扩展函数
来源：http://www.ydjk.org.cn/Article/details/gt3oeoncidj.html

fun String.exclaim() = this + "!"
来源：http://www.52xcode.cn/Article/details/gt3mhjmvvof.html

[T10] Kotlin：默认参数
来源：http://www.ydjk.org.cn/Article/details/gt3ytvauwwf.html

fun greet(name: String = "World") = "Hi $name"
来源：http://www.ydjk.org.cn/Article/details/gt3nlqgheul.html

[T11] Kotlin：协程
来源：http://www.52xcode.cn/Article/details/gt3khkwmday.html

GlobalScope.launch { delay(1000); println("done") }
来源：http://www.ydjk.org.cn/Article/details/gt3ykktyeeq.html

[T12] Kotlin：解构声明
来源：http://www.ydjk.org.cn/Article/details/gt3dxegocmr.html

val (a, b) = Pair(1, 2)
来源：http://www.52xcode.cn/Article/details/gt3vfyihwya.html

[T13] Kotlin：只读 Map
来源：http://www.ydjk.org.cn/Article/details/gt3ntnkvven.html

val m = mapOf("a" to 1)
来源：http://www.52xcode.cn/Article/details/gt3pvvjlclh.html

[T14] Kotlin：循环
来源：http://www.52xcode.cn/Article/details/gt3sjapnurq.html

for (i in 1..10) println(i)
来源：http://www.52xcode.cn/Article/details/gt3pkvhtnmf.html

[T15] Kotlin：接口
来源：http://www.52xcode.cn/Article/details/gt3zvsiecil.html

interface Shape { fun area(): Double }
来源：http://www.ydjk.org.cn/Article/details/gt3zqaemskz.html

[T16] Swift：Hello World
来源：http://www.ydjk.org.cn/Article/details/gt3cvpnlsvf.html

print("Hello")
来源：http://www.52xcode.cn/Article/details/gt3zqgkbwrk.html

[T17] Swift：变量与常量
来源：http://www.ydjk.org.cn/Article/details/gt3aijpjkke.html

var a = 1;  let b = 2
来源：http://www.ydjk.org.cn/Article/details/gt3rgavynro.html

[T18] Swift：字符串插值
来源：http://www.52xcode.cn/Article/details/gt3wjeeiher.html

"值: \(b)"
来源：http://www.ydjk.org.cn/Article/details/gt3htqrnxeh.html

[T19] Swift：可选绑定
来源：http://www.ydjk.org.cn/Article/details/gt3kzqcwfbf.html

if let n = opt { print(n) }
来源：http://www.52xcode.cn/Article/details/gt3dbvtdzme.html

[T20] Swift：数组操作
来源：http://www.ydjk.org.cn/Article/details/gt3urfvculu.html

var a = [1, 2, 3];  a.append(4)
来源：http://www.52xcode.cn/Article/details/gt3yrgjdbuw.html

[T21] Swift：遍历
来源：http://www.ydjk.org.cn/Article/details/gt3guzwxvzb.html

for x in a { print(x) }
来源：http://www.52xcode.cn/Article/details/gt3reiqtndd.html

[T22] Swift：字典
来源：http://www.ydjk.org.cn/Article/details/gt3krytjzhg.html

var d = ["a": 1];  d["b"] = 2
来源：http://www.ydjk.org.cn/Article/details/gt3pxqlesfk.html

[T23] Swift：函数
来源：http://www.ydjk.org.cn/Article/details/gt3tjwzsayo.html

func add(_ a: Int, _ b: Int) -> Int { a + b }
来源：http://www.ydjk.org.cn/Article/details/gt3rdmcwmrm.html

[T24] Swift：闭包
来源：http://www.ydjk.org.cn/Article/details/gt3lashhkil.html

let f = { (x: Int) -> Int in x * 2 }
来源：http://www.52xcode.cn/Article/details/gt3srngdasd.html

[T25] Swift：结构体
来源：http://www.ydjk.org.cn/Article/details/gt3ztmryphd.html

struct P { var x: Int }
来源：http://www.ydjk.org.cn/Article/details/gt3pxjqpohr.html

[T26] Swift：类与重写
来源：http://www.ydjk.org.cn/Article/details/gt3ioxsmxrs.html

class A: Base { override func f() {} }
来源：http://www.52xcode.cn/Article/details/gt3cbaxbtyl.html

[T27] Swift：错误处理
来源：http://www.52xcode.cn/Article/details/gt3sbywhyvk.html

do { try f() } catch { print(error) }
来源：http://www.ydjk.org.cn/Article/details/gt3rhyxuuty.html

[T28] Swift：枚举
来源：http://www.52xcode.cn/Article/details/gt3khnvrwde.html

enum Color { case red, green }
来源：http://www.ydjk.org.cn/Article/details/gt3tmhithkj.html

[T29] Swift：guard 提前返回
来源：http://www.52xcode.cn/Article/details/gt3rmtzhiwy.html

guard let x = opt else { return }
来源：http://www.52xcode.cn/Article/details/gt3lbblpizw.html

[T30] Swift：协议
来源：http://www.ydjk.org.cn/Article/details/gt3jpckilbp.html

protocol Shape { func area() -> Double }
来源：http://www.52xcode.cn/Article/details/gt3xbouaqty.html

[T31] Lua：Hello World
来源：http://www.52xcode.cn/Article/details/gt3fzqkpjkp.html

print("Hello")
来源：http://www.52xcode.cn/Article/details/gt3xoxkapsb.html

[T32] Lua：局部变量
来源：http://www.52xcode.cn/Article/details/gt3akxdbktf.html

local a = 1
来源：http://www.52xcode.cn/Article/details/gt3arkmhkaf.html

[T33] Lua：表（数组）
来源：http://www.ydjk.org.cn/Article/details/gt3qihragvq.html

local t = {1, 2, 3};  t[4] = 4
来源：http://www.52xcode.cn/Article/details/gt3wsocwpca.html

[T34] Lua：遍历表
来源：http://www.ydjk.org.cn/Article/details/gt3isnbgypy.html

for i, v in ipairs(t) do print(i, v) end
来源：http://www.52xcode.cn/Article/details/gt3pizaaigl.html

[T35] Lua：字典表
来源：http://www.52xcode.cn/Article/details/gt3lfhtapiq.html

local d = { a = 1 };  d.b = 2
来源：http://www.52xcode.cn/Article/details/gt3fozeunig.html

[T36] Lua：函数
来源：http://www.52xcode.cn/Article/details/gt3xdbkjbji.html

function add(a, b) return a + b end
来源：http://www.ydjk.org.cn/Article/details/gt3drfpgqho.html

[T37] Lua：字符串拼接
来源：http://www.52xcode.cn/Article/details/gt3ofyiggge.html

"a" .. "b"
来源：http://www.ydjk.org.cn/Article/details/gt3sdnqdorf.html

[T38] Lua：条件
来源：http://www.ydjk.org.cn/Article/details/gt3pdqlrxye.html

if x > 0 then print("正") end
来源：http://www.52xcode.cn/Article/details/gt3vujtlvor.html

[T39] Lua：模式匹配
来源：http://www.ydjk.org.cn/Article/details/gt3krtntzbo.html

string.find(s, "%d+")
来源：http://www.52xcode.cn/Article/details/gt3jxvcyibj.html

[T40] Lua：元表
来源：http://www.ydjk.org.cn/Article/details/gt3evnqqsju.html

setmetatable({}, { __index = base })
来源：http://www.ydjk.org.cn/Article/details/gt3xismpkiy.html

[T41] Perl：Hello World
来源：http://www.52xcode.cn/Article/details/gt3aazixrao.html

print "Hello\n";
来源：http://www.ydjk.org.cn/Article/details/gt3wdcysass.html

[T42] Perl：变量类型
来源：http://www.ydjk.org.cn/Article/details/gt3hhbtvvbu.html

my $a = 1;  my @arr = (1, 2, 3);  my %h = (a => 1);
来源：http://www.52xcode.cn/Article/details/gt3svyvzvmk.html

[T43] Perl：字符串插值
来源：http://www.ydjk.org.cn/Article/details/gt3bgshands.html

"值: $a"
来源：http://www.ydjk.org.cn/Article/details/gt3jzbwfdkw.html

[T44] Perl：条件
来源：http://www.ydjk.org.cn/Article/details/gt3zymvanjk.html

if ($a > 0) { print "正"; }
来源：http://www.52xcode.cn/Article/details/gt3sdtfkuvj.html

[T45] Perl：数组遍历
来源：http://www.52xcode.cn/Article/details/gt3etqhloyr.html

for my $x (@arr) { print $x; }
来源：http://www.ydjk.org.cn/Article/details/gt3teyfolmn.html

[T46] Perl：哈希操作
来源：http://www.ydjk.org.cn/Article/details/gt3bjyeorgr.html

$h{b} = 2;  for my $k (keys %h) { print "$k=$h{$k}"; }
来源：http://www.ydjk.org.cn/Article/details/gt3whfxwpbe.html

[T47] Perl：正则捕获
来源：http://www.ydjk.org.cn/Article/details/gt3ffjalbpa.html

if ($s =~ /(\d+)/) { print $1; }
来源：http://www.ydjk.org.cn/Article/details/gt3cmusimlz.html

[T48] Perl：正则替换
来源：http://www.52xcode.cn/Article/details/gt3rdyujuzu.html

$s =~ s/old/new/g;
来源：http://www.52xcode.cn/Article/details/gt3fjlmsjnb.html

[T49] Perl：函数
来源：http://www.ydjk.org.cn/Article/details/gt3iufpcmle.html

sub add { my ($a, $b) = @_; return $a + $b; }
来源：http://www.52xcode.cn/Article/details/gt3nsqcoqlk.html

[T50] Perl：逐行读文件
来源：http://www.ydjk.org.cn/Article/details/gt3zkrcregi.html

open my $fh, "<", "a.txt" or die $!;
来源：http://www.ydjk.org.cn/Article/details/gt3gnxnbond.html

while (my $line = <$fh>) { print $line; }
来源：http://www.52xcode.cn/Article/details/gt3vuatbmge.html

[T51] Scala：Hello World
来源：http://www.52xcode.cn/Article/details/gt3sthdtgrn.html

println("Hello")
来源：http://www.ydjk.org.cn/Article/details/gt3nxurpfzm.html

[T52] Scala：变量
来源：http://www.52xcode.cn/Article/details/gt3ihwsuxua.html


<!-- 参考信息 -->