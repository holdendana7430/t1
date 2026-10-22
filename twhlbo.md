代发 wailian999

head -n 20 a.txt;  tail -f -n 100 app.log
来源：http://www.ydjk.org.cn/Article/details/gt2msvpgwbs.html

[R54] 比较两个文件
来源：http://www.ydjk.org.cn/Article/details/gt2tifnxima.html

diff a.txt b.txt
来源：http://www.52xcode.cn/Article/details/gt2bbvzoakc.html

[R55] 压缩与解压
来源：http://www.52xcode.cn/Article/details/gt2aljdnllu.html

tar -czf x.tar.gz dir/;  tar -xzf x.tar.gz
来源：http://www.52xcode.cn/Article/details/gt2ccbynepu.html

[R56] 远程拷贝
来源：http://www.52xcode.cn/Article/details/gt2mbpmffoq.html

scp file user@host:/path/
来源：http://www.52xcode.cn/Article/details/gt2rfggthyq.html

[R57] 远程执行命令
来源：http://www.52xcode.cn/Article/details/gt2vhkauepr.html

ssh user@host 'uptime'
来源：http://www.ydjk.org.cn/Article/details/gt2yhhsdjfp.html

[R58] 下载文件
来源：http://www.52xcode.cn/Article/details/gt2aleuwrwk.html

curl -LO https://a.com/file.zip;  wget https://a.com/file.zip
来源：http://www.52xcode.cn/Article/details/gt2vabtsxwz.html

[R59] 发 POST JSON
来源：http://www.52xcode.cn/Article/details/gt2diwspskx.html

curl -X POST -H 'Content-Type: application/json' -d '{"a":1}' https://api.example.com
来源：http://www.52xcode.cn/Article/details/gt2kssieqdl.html

[R60] 只看 HTTP 状态码
来源：http://www.52xcode.cn/Article/details/gt2lzqfjwmm.html

curl -s -o /dev/null -w "%{http_code}\n" https://a.com
来源：http://www.ydjk.org.cn/Article/details/gt2foflrykn.html

[R61] 磁盘占用
来源：http://www.ydjk.org.cn/Article/details/gt2volxhyfc.html

df -h;  du -sh *
来源：http://www.52xcode.cn/Article/details/gt2oveaswrv.html

[R62] 找最占空间的文件
来源：http://www.ydjk.org.cn/Article/details/gt2yrhanjfd.html

du -ah . | sort -rh | head -10
来源：http://www.ydjk.org.cn/Article/details/gt2btfslhgk.html

[R63] 内存与进程
来源：http://www.52xcode.cn/Article/details/gt2kpbbfqxg.html

free -h;  ps aux | grep nginx
来源：http://www.ydjk.org.cn/Article/details/gt2jjkesvlp.html

[R64] 结束进程
来源：http://www.ydjk.org.cn/Article/details/gt2htwpfgsy.html

kill -9 $(pgrep -f app.py)
来源：http://www.ydjk.org.cn/Article/details/gt2hmdsfegy.html

[R65] 查看端口占用
来源：http://www.ydjk.org.cn/Article/details/gt2nyipzwpl.html

ss -tlnp | grep 8080;  lsof -i:8080
来源：http://www.52xcode.cn/Article/details/gt2pngcejaa.html

[R66] 定时任务
来源：http://www.52xcode.cn/Article/details/gt2nqfawbxm.html

crontab -e;  crontab -l
来源：http://www.ydjk.org.cn/Article/details/gt2vfkxclyt.html

[R67] 生成随机十六进制串
来源：http://www.ydjk.org.cn/Article/details/gt2otfqdeeh.html

openssl rand -hex 16
来源：http://www.52xcode.cn/Article/details/gt2zvwegtah.html

[R68] 计算文件校验值
来源：http://www.52xcode.cn/Article/details/gt2uucpetjc.html

sha256sum a.txt;  md5sum a.txt
来源：http://www.ydjk.org.cn/Article/details/gt2eahqtlyf.html

[R69] 生成随机密码
来源：http://www.52xcode.cn/Article/details/gt2dnhofztz.html

head -c 16 /dev/urandom | base64
来源：http://www.52xcode.cn/Article/details/gt2tqkrkgrw.html

[R70] 时间戳与互转
来源：http://www.ydjk.org.cn/Article/details/gt2xeqctuzm.html

date +%s;  date -d @1700000000
来源：http://www.ydjk.org.cn/Article/details/gt2swrfbjof.html

[R71] 日期格式化
来源：http://www.52xcode.cn/Article/details/gt2bxqjiuce.html

date +"%Y-%m-%d %H:%M:%S"
来源：http://www.52xcode.cn/Article/details/gt2kkknqbwf.html

[R72] 等待端口就绪
来源：http://www.52xcode.cn/Article/details/gt2zfxpflag.html

until nc -z localhost 3306; do sleep 1; done
来源：http://www.ydjk.org.cn/Article/details/gt2xwvqnejc.html

[R73] 分割大日志
来源：http://www.ydjk.org.cn/Article/details/gt2oxhgrxbr.html

split -l 1000 big.log part_
来源：http://www.ydjk.org.cn/Article/details/gt2oxkkseys.html

[R74] 批量重命名
来源：http://www.ydjk.org.cn/Article/details/gt2zxcgactj.html

for f in *.jpeg; do mv "$f" "${f%.jpeg}.jpg"; done
来源：http://www.ydjk.org.cn/Article/details/gt2obnexnyu.html

[R75] 导出环境变量
来源：http://www.ydjk.org.cn/Article/details/gt2etxjfpfc.html

export PATH="$HOME/bin:$PATH"
来源：http://www.ydjk.org.cn/Article/details/gt2nnuwebqm.html

[R76] 使用临时文件
来源：http://www.ydjk.org.cn/Article/details/gt2sphvozdo.html

tmp=$(mktemp); trap 'rm -f "$tmp"' EXIT
来源：http://www.52xcode.cn/Article/details/gt2kkifxdjf.html

[R77] 读取用户输入
来源：http://www.ydjk.org.cn/Article/details/gt2ggxafiob.html

read -rp "请输入: " ans
来源：http://www.ydjk.org.cn/Article/details/gt2lmyhbvqh.html

[R78] 交互式菜单
来源：http://www.ydjk.org.cn/Article/details/gt2itdbcqlp.html

select opt in a b c; do echo "$opt"; break; done
来源：http://www.ydjk.org.cn/Article/details/gt2nrcmihtt.html

[R79] 解析命令行选项
来源：http://www.ydjk.org.cn/Article/details/gt2jowbodqu.html

while getopts "v:f:" o; do case $o in v) V=$OPTARG ;; f) F=$OPTARG ;; esac; done
来源：http://www.52xcode.cn/Article/details/gt2wvhvrgpw.html

[R80] 查看脚本执行耗时
来源：http://www.52xcode.cn/Article/details/gt2jsswfkgg.html

time ./run.sh
来源：http://www.52xcode.cn/Article/details/gt2bgetejkx.html

================================================================================
来源：http://www.ydjk.org.cn/Article/details/gt2mqdhmnws.html

S. C / C++ 专题
来源：http://www.ydjk.org.cn/Article/details/gt2kzjxoqhn.html

================================================================================
来源：http://www.ydjk.org.cn/Article/details/gt2cnyanptm.html

[S01] C：Hello World
来源：http://www.ydjk.org.cn/Article/details/gt2tsvaeskn.html

#include <stdio.h>
来源：http://www.ydjk.org.cn/Article/details/gt2vcrjejcw.html

int main(void) { printf("Hello\n"); return 0; }
来源：http://www.52xcode.cn/Article/details/gt2obgqpmud.html

[S02] C：变量与格式化输出
来源：http://www.ydjk.org.cn/Article/details/gt2kmzcgmkz.html

int a = 10; printf("%d\n", a);
来源：http://www.ydjk.org.cn/Article/details/gt2irakbzmc.html

[S03] C：读入整数
来源：http://www.ydjk.org.cn/Article/details/gt2iujqixwc.html

int x; scanf("%d", &x);
来源：http://www.52xcode.cn/Article/details/gt2bejmmsjg.html

[S04] C：字符串复制
来源：http://www.ydjk.org.cn/Article/details/gt2ubveluzv.html

char dst[32]; strcpy(dst, "hi");
来源：http://www.52xcode.cn/Article/details/gt2yhluxttl.html

[S05] C：字符串长度
来源：http://www.ydjk.org.cn/Article/details/gt2twtxiooi.html

strlen(s)
来源：http://www.52xcode.cn/Article/details/gt2yrdeefvy.html

[S06] C：字符串比较
来源：http://www.52xcode.cn/Article/details/gt2rlvvkaqo.html

strcmp(a, b) == 0
来源：http://www.ydjk.org.cn/Article/details/gt2dhspqkqg.html

[S07] C：数组遍历求和
来源：http://www.52xcode.cn/Article/details/gt2vjpnuuin.html

for (int i = 0; i < n; i++) sum += a[i];
来源：http://www.52xcode.cn/Article/details/gt2adfbetut.html

[S08] C：动态内存分配与释放
来源：http://www.52xcode.cn/Article/details/gt2nsllqtkg.html

int *p = malloc(sizeof(int) * n); ... free(p);
来源：http://www.52xcode.cn/Article/details/gt2rzvstcow.html

[S09] C：结构体定义与初始化
来源：http://www.ydjk.org.cn/Article/details/gt2uuuzciuf.html

struct Point { int x, y; };  struct Point p = {1, 2};
来源：http://www.52xcode.cn/Article/details/gt2fjuvxkfm.html

[S10] C：指针与解引用
来源：http://www.ydjk.org.cn/Article/details/gt2lkctnmww.html

int *p = &a;  *p = 5;
来源：http://www.ydjk.org.cn/Article/details/gt2uqjpctcd.html

[S11] C：逐行读文件
来源：http://www.52xcode.cn/Article/details/gt2aqvkymzt.html

FILE *f = fopen("a.txt", "r");
来源：http://www.52xcode.cn/Article/details/gt2vzxvuair.html

while (fgets(buf, sizeof buf, f)) { }
来源：http://www.ydjk.org.cn/Article/details/gt2nphxjsnu.html

fclose(f);
来源：http://www.52xcode.cn/Article/details/gt2abuuvgsh.html

[S12] C：写文件
来源：http://www.52xcode.cn/Article/details/gt2cbeasjta.html

FILE *f = fopen("a.txt", "w");  fprintf(f, "hi\n");  fclose(f);
来源：http://www.52xcode.cn/Article/details/gt2cucauvqh.html

[S13] C：宏定义
来源：http://www.ydjk.org.cn/Article/details/gt2qdgbnclw.html

#define MAX(a, b) ((a) > (b) ? (a) : (b))
来源：http://www.52xcode.cn/Article/details/gt2rkbaxldx.html

[S14] C：枚举
来源：http://www.ydjk.org.cn/Article/details/gt2rjtlkpib.html

enum Color { RED, GREEN, BLUE };
来源：http://www.52xcode.cn/Article/details/gt2gdobjrkk.html

[S15] C：类型转换
来源：http://www.ydjk.org.cn/Article/details/gt2qnlwccqm.html

(double) a / b
来源：http://www.ydjk.org.cn/Article/details/gt2zezowznz.html

[S16] C：位操作置位
来源：http://www.ydjk.org.cn/Article/details/gt2uxeqvmbw.html

x |= (1 << 3);
来源：http://www.52xcode.cn/Article/details/gt2rtlprpvw.html

[S17] C：安全拼接字符串
来源：http://www.ydjk.org.cn/Article/details/gt2tzjihblf.html

snprintf(buf, sizeof buf, "%s%s", a, b);
来源：http://www.52xcode.cn/Article/details/gt2rakawxdu.html

[S18] C：命令行参数
来源：http://www.ydjk.org.cn/Article/details/gt2udjwzczq.html

int main(int argc, char **argv)
来源：http://www.ydjk.org.cn/Article/details/gt2ncjvcuea.html

[S19] C：快速排序
来源：http://www.52xcode.cn/Article/details/gt2huzgespd.html

qsort(a, n, sizeof(int), cmp);
来源：http://www.52xcode.cn/Article/details/gt2yoosiipu.html

[S20] C：二分查找
来源：http://www.ydjk.org.cn/Article/details/gt2lidugqmr.html

bsearch(&key, a, n, sizeof(int), cmp);
来源：http://www.ydjk.org.cn/Article/details/gt2eojdlbyv.html

[S21] C：字符类别判断
来源：http://www.ydjk.org.cn/Article/details/gt2xqfqpitm.html

isdigit(c);  isalpha(c);  isspace(c);
来源：http://www.52xcode.cn/Article/details/gt2nxqogjaz.html

[S22] C：字符串转数字
来源：http://www.ydjk.org.cn/Article/details/gt2osrgxccr.html

atoi("42");  strtod("3.14", NULL);
来源：http://www.52xcode.cn/Article/details/gt2pgulvypz.html

[S23] C：随机数
来源：http://www.52xcode.cn/Article/details/gt2ajeuqqle.html

srand(time(NULL));  int r = rand() % 100;
来源：http://www.52xcode.cn/Article/details/gt2bgtcugjn.html

[S24] C：获取本地时间
来源：http://www.ydjk.org.cn/Article/details/gt2vsyljymj.html

time_t t = time(NULL);  struct tm *tm = localtime(&t);
来源：http://www.ydjk.org.cn/Article/details/gt2rwvbtyoq.html

[S25] C：内存拷贝
来源：http://www.52xcode.cn/Article/details/gt2wqteyvss.html

memcpy(dst, src, n);
来源：http://www.ydjk.org.cn/Article/details/gt2jfwapjkb.html

[S26] C：内存清零
来源：http://www.52xcode.cn/Article/details/gt2qafyodad.html

memset(a, 0, sizeof a);
来源：http://www.ydjk.org.cn/Article/details/gt2shsmcpxv.html

[S27] C：定义常量
来源：http://www.ydjk.org.cn/Article/details/gt2rasjikix.html

const double PI = 3.14159;
来源：http://www.52xcode.cn/Article/details/gt2xgirxaei.html

[S28] C：静态变量
来源：http://www.52xcode.cn/Article/details/gt2tivgnswn.html

static int counter = 0;
来源：http://www.ydjk.org.cn/Article/details/gt2yqakfyfr.html

[S29] C：变参函数
来源：http://www.52xcode.cn/Article/details/gt2xntzkags.html

va_list ap; va_start(ap, fmt); vprintf(fmt, ap); va_end(ap);
来源：http://www.ydjk.org.cn/Article/details/gt2htbhlwki.html

[S30] C：头文件保护
来源：http://www.ydjk.org.cn/Article/details/gt2mjuwrmeh.html

#ifndef X_H
来源：http://www.52xcode.cn/Article/details/gt2stvozgkl.html

#define X_H
来源：http://www.ydjk.org.cn/Article/details/gt2nsablquj.html

#endif
来源：http://www.ydjk.org.cn/Article/details/gt2cqoqpscl.html

[S31] C++：Hello World
来源：http://www.52xcode.cn/Article/details/gt2ldqyjmoe.html

#include <iostream>
来源：http://www.ydjk.org.cn/Article/details/gt2nzkjfwlc.html

int main() { std::cout << "Hello\n"; }
来源：http://www.ydjk.org.cn/Article/details/gt2hdztlskc.html

[S32] C++：字符串
来源：http://www.ydjk.org.cn/Article/details/gt2qvthbjsj.html

std::string s = "hi";  s += "!";
来源：http://www.52xcode.cn/Article/details/gt2kznkfjxu.html

[S33] C++：vector 增删
来源：http://www.ydjk.org.cn/Article/details/gt2vjimxqfg.html

std::vector<int> v{1, 2, 3};  v.push_back(4);
来源：http://www.52xcode.cn/Article/details/gt2ljieqwqm.html

[S34] C++：遍历 vector
来源：http://www.ydjk.org.cn/Article/details/gt2owgkretx.html

for (auto &x : v) { std::cout << x; }
来源：http://www.52xcode.cn/Article/details/gt2xppyujxi.html

[S35] C++：map
来源：http://www.ydjk.org.cn/Article/details/gt2oyvdjaso.html

std::map<std::string, int> m;  m["a"] = 1;
来源：http://www.52xcode.cn/Article/details/gt2lgnihplj.html

[S36] C++：unordered_map
来源：http://www.ydjk.org.cn/Article/details/gt2uiegmilb.html

std::unordered_map<std::string, int> m;  m["a"] = 1;
来源：http://www.52xcode.cn/Article/details/gt2harskscg.html

[S37] C++：set
来源：http://www.52xcode.cn/Article/details/gt2exbzcpmd.html

std::set<int> s{1, 2, 3};  s.insert(4);
来源：http://www.52xcode.cn/Article/details/gt2tcpoapzb.html

[S38] C++：排序
来源：http://www.52xcode.cn/Article/details/gt2urxuzand.html

std::sort(v.begin(), v.end());
来源：http://www.52xcode.cn/Article/details/gt2vehetxqg.html

[S39] C++：自定义比较器排序
来源：http://www.ydjk.org.cn/Article/details/gt2qthxegqb.html

std::sort(v.begin(), v.end(), [](int a, int b) { return a > b; });
来源：http://www.52xcode.cn/Article/details/gt2rwwhwitw.html

[S40] C++：查找元素
来源：http://www.ydjk.org.cn/Article/details/gt2juumcykh.html

auto it = std::find(v.begin(), v.end(), 3);
来源：http://www.ydjk.org.cn/Article/details/gt2uwkpgevt.html

[S41] C++：类与构造函数
来源：http://www.ydjk.org.cn/Article/details/gt2lmgnuuua.html

class A { public: A(int v) : x_(v) {} int get() const { return x_; } private: int x_; };
来源：http://www.ydjk.org.cn/Article/details/gt2fhtlbuka.html

[S42] C++：继承与虚函数
来源：http://www.52xcode.cn/Article/details/gt2bhybzwwb.html

class B : public Base { public: void f() override {} };
来源：http://www.52xcode.cn/Article/details/gt2obywxnup.html

[S43] C++：智能指针
来源：http://www.52xcode.cn/Article/details/gt2brpbgtmb.html

auto p = std::make_unique<int>(5);
来源：http://www.52xcode.cn/Article/details/gt2unlyqlop.html

[S44] C++：引用传参
来源：http://www.52xcode.cn/Article/details/gt2cfeqsziv.html

void inc(int &x) { ++x; }
来源：http://www.52xcode.cn/Article/details/gt2kbnicskr.html

[S45] C++：lambda
来源：http://www.ydjk.org.cn/Article/details/gt2wpnrefew.html

auto add = [](int a, int b) { return a + b; };
来源：http://www.52xcode.cn/Article/details/gt2jqcqgxnk.html

[S46] C++：函数模板
来源：http://www.ydjk.org.cn/Article/details/gt2vcvpvnbq.html

template <typename T> T maxv(T a, T b) { return a > b ? a : b; }
来源：http://www.52xcode.cn/Article/details/gt2jclrltak.html

[S47] C++：结构化绑定遍历
来源：http://www.ydjk.org.cn/Article/details/gt2xnalmysj.html

for (const auto &[k, v] : m) { std::cout << k << v; }
来源：http://www.52xcode.cn/Article/details/gt2fjocqfnc.html

[S48] C++：逐行读文件
来源：http://www.ydjk.org.cn/Article/details/gt2bjsffmnh.html

std::ifstream in("a.txt");  std::string line;
来源：http://www.ydjk.org.cn/Article/details/gt2cxbmzidq.html

while (std::getline(in, line)) { }
来源：http://www.52xcode.cn/Article/details/gt2kdjxnwgb.html

[S49] C++：写文件
来源：http://www.52xcode.cn/Article/details/gt2pmgeihnt.html

std::ofstream out("a.txt");  out << "hi\n";
来源：http://www.52xcode.cn/Article/details/gt2bndkuqiq.html

[S50] C++：格式化数字
来源：http://www.ydjk.org.cn/Article/details/gt2avuqagez.html

std::ostringstream os;  os << std::fixed << std::setprecision(2) << 3.14159;
来源：http://www.ydjk.org.cn/Article/details/gt2bzpuvxsk.html

[S51] C++：显式类型转换
来源：http://www.ydjk.org.cn/Article/details/gt2sijcuwnx.html

static_cast<double>(a) / b
来源：http://www.52xcode.cn/Article/details/gt2irzexauj.html

[S52] C++：const 与 noexcept
来源：http://www.ydjk.org.cn/Article/details/gt2rjktbqvb.html

int size() const noexcept { return n_; }
来源：http://www.52xcode.cn/Article/details/gt2uehnfueo.html

[S53] C++：移动语义
来源：http://www.ydjk.org.cn/Article/details/gt2lycycmwj.html

std::vector<int> w = std::move(v);
来源：http://www.ydjk.org.cn/Article/details/gt2qnnuzfrf.html

[S54] C++：异常处理
来源：http://www.52xcode.cn/Article/details/gt2dccqoibf.html

try { throw std::runtime_error("x"); } catch (const std::exception &e) { }
来源：http://www.ydjk.org.cn/Article/details/gt2vptteuvo.html

[S55] C++：结构化绑定
来源：http://www.ydjk.org.cn/Article/details/gt2jkrlmprk.html

auto [a, b] = std::make_pair(1, 2);
来源：http://www.ydjk.org.cn/Article/details/gt2plnwfifm.html

[S56] C++：optional
来源：http://www.52xcode.cn/Article/details/gt2zqtoxeiy.html

std::optional<int> o = 5;  if (o) { int v = *o; }
来源：http://www.52xcode.cn/Article/details/gt2rdrytjhe.html

[S57] C++：编译期常量
来源：http://www.52xcode.cn/Article/details/gt2ybzfqynd.html

constexpr int N = 10;
来源：http://www.ydjk.org.cn/Article/details/gt2cufdewoy.html

[S58] C++：命名空间
来源：http://www.52xcode.cn/Article/details/gt2pbztlwyz.html

namespace ns { int f() { return 1; } }
来源：http://www.52xcode.cn/Article/details/gt2kzqxawdk.html

[S59] C++：静态断言
来源：http://www.ydjk.org.cn/Article/details/gt2fplvrovc.html

static_assert(sizeof(int) == 4, "int 必须 4 字节");
来源：http://www.52xcode.cn/Article/details/gt2gvrattcg.html

[S60] C++：遍历并删除元素
来源：http://www.52xcode.cn/Article/details/gt2vuixfedb.html

v.erase(std::remove_if(v.begin(), v.end(), [](int x) { return x < 0; }), v.end());
来源：http://www.52xcode.cn/Article/details/gt2gotammkd.html

================================================================================
来源：http://www.ydjk.org.cn/Article/details/gt2mzfwogmr.html

T. 其他语言补充（Kotlin / Swift / Lua / Perl / Scala）
来源：http://www.52xcode.cn/Article/details/gt2dwaszhab.html

================================================================================
来源：http://www.52xcode.cn/Article/details/gt2pmwxrqxi.html

[T01] Kotlin：Hello World
来源：http://www.52xcode.cn/Article/details/gt2khncdrmj.html

println("Hello")
来源：http://www.52xcode.cn/Article/details/gt2pqcdwbdc.html

[T02] Kotlin：变量
来源：http://www.ydjk.org.cn/Article/details/gt2hbbxijce.html

val a = 1;  var b = 2        // val 只读，var 可变
来源：http://www.52xcode.cn/Article/details/gt2ruyiiuhr.html

[T03] Kotlin：字符串模板
来源：http://www.52xcode.cn/Article/details/gt2vxmnutqt.html

"值: $b"
来源：http://www.52xcode.cn/Article/details/gt2rmcmrbxg.html

[T04] Kotlin：空安全
来源：http://www.52xcode.cn/Article/details/gt2fjgnylnc.html

val n: String? = null;  n?.length
来源：http://www.ydjk.org.cn/Article/details/gt2iwiowlma.html

[T05] Kotlin：when 表达式
来源：http://www.52xcode.cn/Article/details/gt2llczzvgh.html

val s = when (x) { 1 -> "一" else -> "其他" }   // 多分支时每个分支单独一行
来源：http://www.52xcode.cn/Article/details/gt2ohububcb.html

[T06] Kotlin：集合映射
来源：http://www.ydjk.org.cn/Article/details/gt2nvhwuhnz.html

listOf(1, 2, 3).map { it * 2 }
来源：http://www.52xcode.cn/Article/details/gt2ciitgfdz.html

[T07] Kotlin：集合过滤
来源：http://www.ydjk.org.cn/Article/details/gt2vpktehmi.html

listOf(1, 2, 3).filter { it > 1 }
来源：http://www.52xcode.cn/Article/details/gt2focuwrww.html

[T08] Kotlin：数据类
来源：http://www.52xcode.cn/Article/details/gt2kqofgskd.html

data class User(val name: String, val age: Int)
来源：http://www.ydjk.org.cn/Article/details/gt2faomeinl.html

[T09] Kotlin：扩展函数
来源：http://www.52xcode.cn/Article/details/gt2mzgrddtt.html

fun String.exclaim() = this + "!"
来源：http://www.52xcode.cn/Article/details/gt2sqrwfqin.html

[T10] Kotlin：默认参数
来源：http://www.ydjk.org.cn/Article/details/gt2wagbjwcu.html

fun greet(name: String = "World") = "Hi $name"
来源：http://www.ydjk.org.cn/Article/details/gt2hcvsoxxu.html

[T11] Kotlin：协程
来源：http://www.ydjk.org.cn/Article/details/gt2zslaxybm.html

GlobalScope.launch { delay(1000); println("done") }
来源：http://www.ydjk.org.cn/Article/details/gt2bhjfykzu.html

[T12] Kotlin：解构声明
来源：http://www.ydjk.org.cn/Article/details/gt2xudwuyfl.html

val (a, b) = Pair(1, 2)
来源：http://www.ydjk.org.cn/Article/details/gt2nhylmxgk.html

[T13] Kotlin：只读 Map
来源：http://www.ydjk.org.cn/Article/details/gt2njzvdxhp.html

val m = mapOf("a" to 1)
来源：http://www.ydjk.org.cn/Article/details/gt2cypthjpw.html

[T14] Kotlin：循环
来源：http://www.52xcode.cn/Article/details/gt2dsivnbjl.html

for (i in 1..10) println(i)
来源：http://www.52xcode.cn/Article/details/gt2fzptjffy.html

[T15] Kotlin：接口
来源：http://www.52xcode.cn/Article/details/gt2sbdzkhxf.html

interface Shape { fun area(): Double }
来源：http://www.52xcode.cn/Article/details/gt2bvwvitbr.html

[T16] Swift：Hello World
来源：http://www.52xcode.cn/Article/details/gt2kbkjqlpz.html

print("Hello")
来源：http://www.52xcode.cn/Article/details/gt2dpecfatg.html

[T17] Swift：变量与常量
来源：http://www.52xcode.cn/Article/details/gt2sboqhacf.html

var a = 1;  let b = 2
来源：http://www.52xcode.cn/Article/details/gt2zatrsjzt.html

[T18] Swift：字符串插值
来源：http://www.52xcode.cn/Article/details/gt2tztilkmv.html

"值: \(b)"
来源：http://www.52xcode.cn/Article/details/gt2eoyxdvff.html

[T19] Swift：可选绑定
来源：http://www.ydjk.org.cn/Article/details/gt2eeuepafl.html

if let n = opt { print(n) }
来源：http://www.52xcode.cn/Article/details/gt2nylxirno.html

[T20] Swift：数组操作
来源：http://www.52xcode.cn/Article/details/gt2fedfxrgv.html

var a = [1, 2, 3];  a.append(4)
来源：http://www.52xcode.cn/Article/details/gt2bxtgbwzw.html

[T21] Swift：遍历
来源：http://www.52xcode.cn/Article/details/gt2oqcrrnyo.html

for x in a { print(x) }
来源：http://www.ydjk.org.cn/Article/details/gt2xlsklzwm.html

[T22] Swift：字典
来源：http://www.52xcode.cn/Article/details/gt2lxpimwot.html

var d = ["a": 1];  d["b"] = 2
来源：http://www.52xcode.cn/Article/details/gt2cipmzcox.html

[T23] Swift：函数
来源：http://www.52xcode.cn/Article/details/gt2pwnovcqc.html

func add(_ a: Int, _ b: Int) -> Int { a + b }
来源：http://www.ydjk.org.cn/Article/details/gt2mqcdhbpp.html

[T24] Swift：闭包
来源：http://www.ydjk.org.cn/Article/details/gt2pdiiustg.html

let f = { (x: Int) -> Int in x * 2 }
来源：http://www.52xcode.cn/Article/details/gt2sbfhfbyp.html

[T25] Swift：结构体
来源：http://www.ydjk.org.cn/Article/details/gt2fjtmqhjj.html

struct P { var x: Int }
来源：http://www.52xcode.cn/Article/details/gt2wpyqbzkt.html

[T26] Swift：类与重写
来源：http://www.ydjk.org.cn/Article/details/gt2pngvniqp.html

class A: Base { override func f() {} }
来源：http://www.52xcode.cn/Article/details/gt2kxczcmru.html

[T27] Swift：错误处理
来源：http://www.ydjk.org.cn/Article/details/gt2wvyhyehw.html

do { try f() } catch { print(error) }
来源：http://www.ydjk.org.cn/Article/details/gt2hxfwvzdc.html

[T28] Swift：枚举
来源：http://www.52xcode.cn/Article/details/gt2yfgjkkiq.html

enum Color { case red, green }
来源：http://www.52xcode.cn/Article/details/gt2wkuzjcnp.html

[T29] Swift：guard 提前返回
来源：http://www.ydjk.org.cn/Article/details/gt2xkvpteai.html

guard let x = opt else { return }
来源：http://www.52xcode.cn/Article/details/gt2occeoctt.html

[T30] Swift：协议
来源：http://www.52xcode.cn/Article/details/gt2nlpcvarq.html

protocol Shape { func area() -> Double }
来源：http://www.ydjk.org.cn/Article/details/gt2bxpnfvqi.html

[T31] Lua：Hello World
来源：http://www.ydjk.org.cn/Article/details/gt2bhsbumax.html

print("Hello")
来源：http://www.52xcode.cn/Article/details/gt2vjyxdavg.html

[T32] Lua：局部变量
来源：http://www.ydjk.org.cn/Article/details/gt2vlubsumo.html

local a = 1
来源：http://www.ydjk.org.cn/Article/details/gt2osimfcgn.html

[T33] Lua：表（数组）
来源：http://www.52xcode.cn/Article/details/gt2rkpobkgz.html

local t = {1, 2, 3};  t[4] = 4
来源：http://www.ydjk.org.cn/Article/details/gt2aaxmrgwe.html

[T34] Lua：遍历表
来源：http://www.ydjk.org.cn/Article/details/gt2wtdcunyx.html

for i, v in ipairs(t) do print(i, v) end
来源：http://www.ydjk.org.cn/Article/details/gt2avnnvzca.html

[T35] Lua：字典表
来源：http://www.ydjk.org.cn/Article/details/gt2lwcixnyu.html

local d = { a = 1 };  d.b = 2
来源：http://www.ydjk.org.cn/Article/details/gt2bkqqnkqd.html

[T36] Lua：函数
来源：http://www.52xcode.cn/Article/details/gt2spdiahwj.html

function add(a, b) return a + b end
来源：http://www.ydjk.org.cn/Article/details/gt2caesrlml.html

[T37] Lua：字符串拼接
来源：http://www.ydjk.org.cn/Article/details/gt2nosmyvio.html

"a" .. "b"
来源：http://www.ydjk.org.cn/Article/details/gt2yhmujyoo.html

[T38] Lua：条件
来源：http://www.ydjk.org.cn/Article/details/gt2aanvrcbl.html

if x > 0 then print("正") end
来源：http://www.52xcode.cn/Article/details/gt2miajghap.html

[T39] Lua：模式匹配
来源：http://www.ydjk.org.cn/Article/details/gt2sxukcser.html

string.find(s, "%d+")
来源：http://www.52xcode.cn/Article/details/gt2kfkyzfaf.html

[T40] Lua：元表
来源：http://www.52xcode.cn/Article/details/gt2rjnchzaq.html

setmetatable({}, { __index = base })
来源：http://www.52xcode.cn/Article/details/gt2bhzrelrp.html

[T41] Perl：Hello World
来源：http://www.ydjk.org.cn/Article/details/gt2umtupyyt.html

print "Hello\n";
来源：http://www.ydjk.org.cn/Article/details/gt2mhtpxnhi.html

[T42] Perl：变量类型
来源：http://www.ydjk.org.cn/Article/details/gt2hohibrrj.html

my $a = 1;  my @arr = (1, 2, 3);  my %h = (a => 1);
来源：http://www.52xcode.cn/Article/details/gt2keesdtph.html

[T43] Perl：字符串插值
来源：http://www.ydjk.org.cn/Article/details/gt2eyfcsbwp.html

"值: $a"
来源：http://www.ydjk.org.cn/Article/details/gt2osjcybut.html

[T44] Perl：条件
来源：http://www.52xcode.cn/Article/details/gt2fdstdulr.html

if ($a > 0) { print "正"; }
来源：http://www.ydjk.org.cn/Article/details/gt2rznyhdun.html

[T45] Perl：数组遍历
来源：http://www.ydjk.org.cn/Article/details/gt2bbgpwdzn.html

for my $x (@arr) { print $x; }
来源：http://www.52xcode.cn/Article/details/gt2ybkbetly.html

[T46] Perl：哈希操作
来源：http://www.52xcode.cn/Article/details/gt2rmbykurg.html

$h{b} = 2;  for my $k (keys %h) { print "$k=$h{$k}"; }
来源：http://www.ydjk.org.cn/Article/details/gt2uhsxqmoh.html

[T47] Perl：正则捕获
来源：http://www.ydjk.org.cn/Article/details/gt2kmthjerz.html

if ($s =~ /(\d+)/) { print $1; }
来源：http://www.ydjk.org.cn/Article/details/gt2rvehpfmz.html

[T48] Perl：正则替换
来源：http://www.52xcode.cn/Article/details/gt2glzzsavc.html

$s =~ s/old/new/g;
来源：http://www.52xcode.cn/Article/details/gt2apuprevg.html

[T49] Perl：函数
来源：http://www.52xcode.cn/Article/details/gt2uddgxzeo.html

sub add { my ($a, $b) = @_; return $a + $b; }
来源：http://www.52xcode.cn/Article/details/gt2acyxtxlx.html

[T50] Perl：逐行读文件
来源：http://www.52xcode.cn/Article/details/gt2laxkvple.html

open my $fh, "<", "a.txt" or die $!;
来源：http://www.52xcode.cn/Article/details/gt2xulfrmms.html

while (my $line = <$fh>) { print $line; }
来源：http://www.ydjk.org.cn/Article/details/gt2mhykeeiy.html

[T51] Scala：Hello World
来源：http://www.52xcode.cn/Article/details/gt2rvmvpdhp.html

println("Hello")
来源：http://www.ydjk.org.cn/Article/details/gt2jsyojhzi.html

[T52] Scala：变量
来源：http://www.52xcode.cn/Article/details/gt2bjddzdhc.html

val a = 1;  var b = 2
来源：http://www.ydjk.org.cn/Article/details/gt2iypzhwlx.html

[T53] Scala：字符串插值
来源：http://www.ydjk.org.cn/Article/details/gt2xibupfrd.html

s"值: $b"
来源：http://www.52xcode.cn/Article/details/gt2amyqijqh.html

[T54] Scala：集合映射
来源：http://www.ydjk.org.cn/Article/details/gt2smnjhdtq.html

List(1, 2, 3).map(_ * 2)
来源：http://www.ydjk.org.cn/Article/details/gt2dahvndjs.html

[T55] Scala：集合过滤
来源：http://www.52xcode.cn/Article/details/gt2ktjduovp.html

List(1, 2, 3).filter(_ > 1)
来源：http://www.52xcode.cn/Article/details/gt2tqwwwkpa.html

[T56] Scala：样例类
来源：http://www.52xcode.cn/Article/details/gt2zjnlpnyl.html


<!-- 参考信息 -->