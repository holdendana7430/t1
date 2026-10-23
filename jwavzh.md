代发 wailian999

head -n 20 a.txt;  tail -f -n 100 app.log
来源：http://www.52xcode.cn/Article/details/gt3irdgrgey.html

[R54] 比较两个文件
来源：http://www.52xcode.cn/Article/details/gt3hzrhipfr.html

diff a.txt b.txt
来源：http://www.ydjk.org.cn/Article/details/gt3rnudhzwy.html

[R55] 压缩与解压
来源：http://www.ydjk.org.cn/Article/details/gt3velcsqty.html

tar -czf x.tar.gz dir/;  tar -xzf x.tar.gz
来源：http://www.52xcode.cn/Article/details/gt3isrinyuk.html

[R56] 远程拷贝
来源：http://www.52xcode.cn/Article/details/gt3ofmtaprl.html

scp file user@host:/path/
来源：http://www.ydjk.org.cn/Article/details/gt3xilalqki.html

[R57] 远程执行命令
来源：http://www.52xcode.cn/Article/details/gt3cqekrfdy.html

ssh user@host 'uptime'
来源：http://www.52xcode.cn/Article/details/gt3iewpoank.html

[R58] 下载文件
来源：http://www.52xcode.cn/Article/details/gt3spbsydln.html

curl -LO https://a.com/file.zip;  wget https://a.com/file.zip
来源：http://www.ydjk.org.cn/Article/details/gt3ljbhgpbw.html

[R59] 发 POST JSON
来源：http://www.52xcode.cn/Article/details/gt3ilwjpsdy.html

curl -X POST -H 'Content-Type: application/json' -d '{"a":1}' https://api.example.com
来源：http://www.52xcode.cn/Article/details/gt3wetdmktv.html

[R60] 只看 HTTP 状态码
来源：http://www.ydjk.org.cn/Article/details/gt3grpsnlam.html

curl -s -o /dev/null -w "%{http_code}\n" https://a.com
来源：http://www.52xcode.cn/Article/details/gt3xppottny.html

[R61] 磁盘占用
来源：http://www.ydjk.org.cn/Article/details/gt3kwhkrbwo.html

df -h;  du -sh *
来源：http://www.ydjk.org.cn/Article/details/gt3zabohfxh.html

[R62] 找最占空间的文件
来源：http://www.52xcode.cn/Article/details/gt3rzaovqtg.html

du -ah . | sort -rh | head -10
来源：http://www.ydjk.org.cn/Article/details/gt3qekaltce.html

[R63] 内存与进程
来源：http://www.ydjk.org.cn/Article/details/gt3yxqhphvb.html

free -h;  ps aux | grep nginx
来源：http://www.ydjk.org.cn/Article/details/gt3msprdrxi.html

[R64] 结束进程
来源：http://www.ydjk.org.cn/Article/details/gt3phvufwby.html

kill -9 $(pgrep -f app.py)
来源：http://www.52xcode.cn/Article/details/gt3xaqtbsyh.html

[R65] 查看端口占用
来源：http://www.ydjk.org.cn/Article/details/gt3hqbmdnau.html

ss -tlnp | grep 8080;  lsof -i:8080
来源：http://www.52xcode.cn/Article/details/gt3rtghiqup.html

[R66] 定时任务
来源：http://www.ydjk.org.cn/Article/details/gt3uqcorhvp.html

crontab -e;  crontab -l
来源：http://www.ydjk.org.cn/Article/details/gt3ruuqxzrn.html

[R67] 生成随机十六进制串
来源：http://www.52xcode.cn/Article/details/gt3rzzcegco.html

openssl rand -hex 16
来源：http://www.ydjk.org.cn/Article/details/gt3wgqkjezf.html

[R68] 计算文件校验值
来源：http://www.ydjk.org.cn/Article/details/gt3qlrdaaqs.html

sha256sum a.txt;  md5sum a.txt
来源：http://www.52xcode.cn/Article/details/gt3xnbzmkxv.html

[R69] 生成随机密码
来源：http://www.ydjk.org.cn/Article/details/gt3occlvezh.html

head -c 16 /dev/urandom | base64
来源：http://www.ydjk.org.cn/Article/details/gt3nksueetz.html

[R70] 时间戳与互转
来源：http://www.52xcode.cn/Article/details/gt3fufodkee.html

date +%s;  date -d @1700000000
来源：http://www.ydjk.org.cn/Article/details/gt3gtlfufpb.html

[R71] 日期格式化
来源：http://www.ydjk.org.cn/Article/details/gt3jeqoawjo.html

date +"%Y-%m-%d %H:%M:%S"
来源：http://www.ydjk.org.cn/Article/details/gt3dlceaxjw.html

[R72] 等待端口就绪
来源：http://www.ydjk.org.cn/Article/details/gt3iydpiqjh.html

until nc -z localhost 3306; do sleep 1; done
来源：http://www.52xcode.cn/Article/details/gt3fyyyrjsz.html

[R73] 分割大日志
来源：http://www.52xcode.cn/Article/details/gt3exhsruoe.html

split -l 1000 big.log part_
来源：http://www.ydjk.org.cn/Article/details/gt3hapuwdci.html

[R74] 批量重命名
来源：http://www.52xcode.cn/Article/details/gt3dxccqvkn.html

for f in *.jpeg; do mv "$f" "${f%.jpeg}.jpg"; done
来源：http://www.ydjk.org.cn/Article/details/gt3xakrdlit.html

[R75] 导出环境变量
来源：http://www.52xcode.cn/Article/details/gt3tslejmwx.html

export PATH="$HOME/bin:$PATH"
来源：http://www.ydjk.org.cn/Article/details/gt3bibftkjv.html

[R76] 使用临时文件
来源：http://www.52xcode.cn/Article/details/gt3cfvfkxak.html

tmp=$(mktemp); trap 'rm -f "$tmp"' EXIT
来源：http://www.ydjk.org.cn/Article/details/gt3gwbtazch.html

[R77] 读取用户输入
来源：http://www.52xcode.cn/Article/details/gt3boqcblef.html

read -rp "请输入: " ans
来源：http://www.52xcode.cn/Article/details/gt3dlwvxuzg.html

[R78] 交互式菜单
来源：http://www.ydjk.org.cn/Article/details/gt3jhmqmtho.html

select opt in a b c; do echo "$opt"; break; done
来源：http://www.ydjk.org.cn/Article/details/gt3slqjwose.html

[R79] 解析命令行选项
来源：http://www.52xcode.cn/Article/details/gt3xygyqyhy.html

while getopts "v:f:" o; do case $o in v) V=$OPTARG ;; f) F=$OPTARG ;; esac; done
来源：http://www.ydjk.org.cn/Article/details/gt3lrteembq.html

[R80] 查看脚本执行耗时
来源：http://www.52xcode.cn/Article/details/gt3fyigflil.html

time ./run.sh
来源：http://www.52xcode.cn/Article/details/gt3ngqlqpqd.html

================================================================================
来源：http://www.ydjk.org.cn/Article/details/gt3kmeoemrw.html

S. C / C++ 专题
来源：http://www.ydjk.org.cn/Article/details/gt3lngmkesb.html

================================================================================
来源：http://www.52xcode.cn/Article/details/gt3oxuubcky.html

[S01] C：Hello World
来源：http://www.ydjk.org.cn/Article/details/gt3gmziwuax.html

#include <stdio.h>
来源：http://www.52xcode.cn/Article/details/gt3stsajsfy.html

int main(void) { printf("Hello\n"); return 0; }
来源：http://www.52xcode.cn/Article/details/gt3cyzozwxl.html

[S02] C：变量与格式化输出
来源：http://www.52xcode.cn/Article/details/gt3ogjawmpy.html

int a = 10; printf("%d\n", a);
来源：http://www.ydjk.org.cn/Article/details/gt3fplwdbzh.html

[S03] C：读入整数
来源：http://www.ydjk.org.cn/Article/details/gt3utsikldc.html

int x; scanf("%d", &x);
来源：http://www.52xcode.cn/Article/details/gt3swznafkt.html

[S04] C：字符串复制
来源：http://www.ydjk.org.cn/Article/details/gt3swhresmd.html

char dst[32]; strcpy(dst, "hi");
来源：http://www.ydjk.org.cn/Article/details/gt3kctzwnia.html

[S05] C：字符串长度
来源：http://www.52xcode.cn/Article/details/gt3aqfxpoej.html

strlen(s)
来源：http://www.ydjk.org.cn/Article/details/gt3gklufkkv.html

[S06] C：字符串比较
来源：http://www.ydjk.org.cn/Article/details/gt3tkwdmioq.html

strcmp(a, b) == 0
来源：http://www.ydjk.org.cn/Article/details/gt3kkdpwtic.html

[S07] C：数组遍历求和
来源：http://www.ydjk.org.cn/Article/details/gt3bwmeujyk.html

for (int i = 0; i < n; i++) sum += a[i];
来源：http://www.52xcode.cn/Article/details/gt3ylrofheb.html

[S08] C：动态内存分配与释放
来源：http://www.52xcode.cn/Article/details/gt3wxlqgjql.html

int *p = malloc(sizeof(int) * n); ... free(p);
来源：http://www.ydjk.org.cn/Article/details/gt3ejpsjnbh.html

[S09] C：结构体定义与初始化
来源：http://www.52xcode.cn/Article/details/gt3ullqcefo.html

struct Point { int x, y; };  struct Point p = {1, 2};
来源：http://www.52xcode.cn/Article/details/gt3dhdruroa.html

[S10] C：指针与解引用
来源：http://www.52xcode.cn/Article/details/gt3soxeahnh.html

int *p = &a;  *p = 5;
来源：http://www.ydjk.org.cn/Article/details/gt3equzzwlx.html

[S11] C：逐行读文件
来源：http://www.52xcode.cn/Article/details/gt3penjlhlh.html

FILE *f = fopen("a.txt", "r");
来源：http://www.ydjk.org.cn/Article/details/gt3uhilblby.html

while (fgets(buf, sizeof buf, f)) { }
来源：http://www.ydjk.org.cn/Article/details/gt3ntvjqhff.html

fclose(f);
来源：http://www.ydjk.org.cn/Article/details/gt3tqxqdrcu.html

[S12] C：写文件
来源：http://www.52xcode.cn/Article/details/gt3azdhzzol.html

FILE *f = fopen("a.txt", "w");  fprintf(f, "hi\n");  fclose(f);
来源：http://www.52xcode.cn/Article/details/gt3mktfkgey.html

[S13] C：宏定义
来源：http://www.52xcode.cn/Article/details/gt3tqeymcso.html

#define MAX(a, b) ((a) > (b) ? (a) : (b))
来源：http://www.ydjk.org.cn/Article/details/gt3qvfhepkh.html

[S14] C：枚举
来源：http://www.ydjk.org.cn/Article/details/gt3dfaneobx.html

enum Color { RED, GREEN, BLUE };
来源：http://www.ydjk.org.cn/Article/details/gt3logfnnvq.html

[S15] C：类型转换
来源：http://www.ydjk.org.cn/Article/details/gt3hmwmbrav.html

(double) a / b
来源：http://www.ydjk.org.cn/Article/details/gt3tqrknpfs.html

[S16] C：位操作置位
来源：http://www.52xcode.cn/Article/details/gt3mejjsmkz.html

x |= (1 << 3);
来源：http://www.ydjk.org.cn/Article/details/gt3fuhvyduo.html

[S17] C：安全拼接字符串
来源：http://www.ydjk.org.cn/Article/details/gt3onawzcef.html

snprintf(buf, sizeof buf, "%s%s", a, b);
来源：http://www.52xcode.cn/Article/details/gt3vqkwirsu.html

[S18] C：命令行参数
来源：http://www.52xcode.cn/Article/details/gt3cxgpapky.html

int main(int argc, char **argv)
来源：http://www.ydjk.org.cn/Article/details/gt3injoalwz.html

[S19] C：快速排序
来源：http://www.52xcode.cn/Article/details/gt3dtdabers.html

qsort(a, n, sizeof(int), cmp);
来源：http://www.52xcode.cn/Article/details/gt3xpgygpvq.html

[S20] C：二分查找
来源：http://www.ydjk.org.cn/Article/details/gt3viwlxsck.html

bsearch(&key, a, n, sizeof(int), cmp);
来源：http://www.52xcode.cn/Article/details/gt3vzyfjlzy.html

[S21] C：字符类别判断
来源：http://www.52xcode.cn/Article/details/gt3ksopmgqm.html

isdigit(c);  isalpha(c);  isspace(c);
来源：http://www.ydjk.org.cn/Article/details/gt3ikrwdnxx.html

[S22] C：字符串转数字
来源：http://www.ydjk.org.cn/Article/details/gt3gexjshrl.html

atoi("42");  strtod("3.14", NULL);
来源：http://www.52xcode.cn/Article/details/gt3wrejshkh.html

[S23] C：随机数
来源：http://www.ydjk.org.cn/Article/details/gt3fkowrfqf.html

srand(time(NULL));  int r = rand() % 100;
来源：http://www.52xcode.cn/Article/details/gt3uvwfvpyo.html

[S24] C：获取本地时间
来源：http://www.ydjk.org.cn/Article/details/gt3yqwfcaky.html

time_t t = time(NULL);  struct tm *tm = localtime(&t);
来源：http://www.52xcode.cn/Article/details/gt3fzjevjmu.html

[S25] C：内存拷贝
来源：http://www.52xcode.cn/Article/details/gt3nqujmmng.html

memcpy(dst, src, n);
来源：http://www.52xcode.cn/Article/details/gt3rttjfxmi.html

[S26] C：内存清零
来源：http://www.ydjk.org.cn/Article/details/gt3yoqausfw.html

memset(a, 0, sizeof a);
来源：http://www.52xcode.cn/Article/details/gt3mlqkrgqk.html

[S27] C：定义常量
来源：http://www.52xcode.cn/Article/details/gt3lngrtrii.html

const double PI = 3.14159;
来源：http://www.ydjk.org.cn/Article/details/gt3skzzxkus.html

[S28] C：静态变量
来源：http://www.52xcode.cn/Article/details/gt3peadzxnu.html

static int counter = 0;
来源：http://www.52xcode.cn/Article/details/gt3agkbcvde.html

[S29] C：变参函数
来源：http://www.ydjk.org.cn/Article/details/gt3zrbtgaax.html

va_list ap; va_start(ap, fmt); vprintf(fmt, ap); va_end(ap);
来源：http://www.ydjk.org.cn/Article/details/gt3fsghgiqh.html

[S30] C：头文件保护
来源：http://www.ydjk.org.cn/Article/details/gt3njxlqtxf.html

#ifndef X_H
来源：http://www.52xcode.cn/Article/details/gt3oanswjea.html

#define X_H
来源：http://www.ydjk.org.cn/Article/details/gt3xlgxsryr.html

#endif
来源：http://www.ydjk.org.cn/Article/details/gt3etgbhqic.html

[S31] C++：Hello World
来源：http://www.ydjk.org.cn/Article/details/gt3wgtdjhuo.html

#include <iostream>
来源：http://www.52xcode.cn/Article/details/gt3cemyhfur.html

int main() { std::cout << "Hello\n"; }
来源：http://www.52xcode.cn/Article/details/gt3esyaovnl.html

[S32] C++：字符串
来源：http://www.ydjk.org.cn/Article/details/gt3krzxldjq.html

std::string s = "hi";  s += "!";
来源：http://www.52xcode.cn/Article/details/gt3gnryiywe.html

[S33] C++：vector 增删
来源：http://www.ydjk.org.cn/Article/details/gt3zetevngz.html

std::vector<int> v{1, 2, 3};  v.push_back(4);
来源：http://www.ydjk.org.cn/Article/details/gt3elmsisuc.html

[S34] C++：遍历 vector
来源：http://www.52xcode.cn/Article/details/gt3qdggervw.html

for (auto &x : v) { std::cout << x; }
来源：http://www.52xcode.cn/Article/details/gt3bodtugtx.html

[S35] C++：map
来源：http://www.52xcode.cn/Article/details/gt3etpfncim.html

std::map<std::string, int> m;  m["a"] = 1;
来源：http://www.ydjk.org.cn/Article/details/gt3wpjxugbj.html

[S36] C++：unordered_map
来源：http://www.52xcode.cn/Article/details/gt3hdwyaqvt.html

std::unordered_map<std::string, int> m;  m["a"] = 1;
来源：http://www.52xcode.cn/Article/details/gt3cvhfygxr.html

[S37] C++：set
来源：http://www.ydjk.org.cn/Article/details/gt3qswsrley.html

std::set<int> s{1, 2, 3};  s.insert(4);
来源：http://www.52xcode.cn/Article/details/gt3epnxesho.html

[S38] C++：排序
来源：http://www.52xcode.cn/Article/details/gt3dtzhjjsh.html

std::sort(v.begin(), v.end());
来源：http://www.52xcode.cn/Article/details/gt3yqavxrhf.html

[S39] C++：自定义比较器排序
来源：http://www.ydjk.org.cn/Article/details/gt3qtenfvpq.html

std::sort(v.begin(), v.end(), [](int a, int b) { return a > b; });
来源：http://www.ydjk.org.cn/Article/details/gt3umsojwpw.html

[S40] C++：查找元素
来源：http://www.52xcode.cn/Article/details/gt3rkwmcguq.html

auto it = std::find(v.begin(), v.end(), 3);
来源：http://www.52xcode.cn/Article/details/gt3tuyxwruz.html

[S41] C++：类与构造函数
来源：http://www.52xcode.cn/Article/details/gt3bhcbovhl.html

class A { public: A(int v) : x_(v) {} int get() const { return x_; } private: int x_; };
来源：http://www.ydjk.org.cn/Article/details/gt3zywhozpd.html

[S42] C++：继承与虚函数
来源：http://www.ydjk.org.cn/Article/details/gt3toaqkmjg.html

class B : public Base { public: void f() override {} };
来源：http://www.ydjk.org.cn/Article/details/gt3gkvszpqh.html

[S43] C++：智能指针
来源：http://www.ydjk.org.cn/Article/details/gt3ruftvjoa.html

auto p = std::make_unique<int>(5);
来源：http://www.ydjk.org.cn/Article/details/gt3unlbudwf.html

[S44] C++：引用传参
来源：http://www.52xcode.cn/Article/details/gt3xfxzhncf.html

void inc(int &x) { ++x; }
来源：http://www.ydjk.org.cn/Article/details/gt3dhrcslsm.html

[S45] C++：lambda
来源：http://www.52xcode.cn/Article/details/gt3roiyzvvw.html

auto add = [](int a, int b) { return a + b; };
来源：http://www.ydjk.org.cn/Article/details/gt3eehkhiew.html

[S46] C++：函数模板
来源：http://www.ydjk.org.cn/Article/details/gt3tnmsphwn.html

template <typename T> T maxv(T a, T b) { return a > b ? a : b; }
来源：http://www.52xcode.cn/Article/details/gt3ruzbeidi.html

[S47] C++：结构化绑定遍历
来源：http://www.ydjk.org.cn/Article/details/gt3kpxclqdo.html

for (const auto &[k, v] : m) { std::cout << k << v; }
来源：http://www.ydjk.org.cn/Article/details/gt3akrbgszy.html

[S48] C++：逐行读文件
来源：http://www.ydjk.org.cn/Article/details/gt3cyidpsey.html

std::ifstream in("a.txt");  std::string line;
来源：http://www.52xcode.cn/Article/details/gt3kmndbbzt.html

while (std::getline(in, line)) { }
来源：http://www.52xcode.cn/Article/details/gt3qajanysz.html

[S49] C++：写文件
来源：http://www.52xcode.cn/Article/details/gt3vpmpnucs.html

std::ofstream out("a.txt");  out << "hi\n";
来源：http://www.ydjk.org.cn/Article/details/gt3imjsclob.html

[S50] C++：格式化数字
来源：http://www.52xcode.cn/Article/details/gt3xshvgvij.html

std::ostringstream os;  os << std::fixed << std::setprecision(2) << 3.14159;
来源：http://www.52xcode.cn/Article/details/gt3stapebvs.html

[S51] C++：显式类型转换
来源：http://www.ydjk.org.cn/Article/details/gt3lnqbqgvn.html

static_cast<double>(a) / b
来源：http://www.ydjk.org.cn/Article/details/gt3kfshjdkn.html

[S52] C++：const 与 noexcept
来源：http://www.52xcode.cn/Article/details/gt3aoiwjdjt.html

int size() const noexcept { return n_; }
来源：http://www.52xcode.cn/Article/details/gt3ivdvzybq.html

[S53] C++：移动语义
来源：http://www.52xcode.cn/Article/details/gt3ccmgvrpg.html

std::vector<int> w = std::move(v);
来源：http://www.ydjk.org.cn/Article/details/gt3slknkfrn.html

[S54] C++：异常处理
来源：http://www.52xcode.cn/Article/details/gt3togcqoqz.html

try { throw std::runtime_error("x"); } catch (const std::exception &e) { }
来源：http://www.ydjk.org.cn/Article/details/gt3meztdloj.html

[S55] C++：结构化绑定
来源：http://www.ydjk.org.cn/Article/details/gt3uyxqpgir.html

auto [a, b] = std::make_pair(1, 2);
来源：http://www.ydjk.org.cn/Article/details/gt3tsxjqzbp.html

[S56] C++：optional
来源：http://www.52xcode.cn/Article/details/gt3lazpltdx.html

std::optional<int> o = 5;  if (o) { int v = *o; }
来源：http://www.ydjk.org.cn/Article/details/gt3nczvhegd.html

[S57] C++：编译期常量
来源：http://www.52xcode.cn/Article/details/gt3gxzfggcf.html

constexpr int N = 10;
来源：http://www.52xcode.cn/Article/details/gt3obraquiq.html

[S58] C++：命名空间
来源：http://www.ydjk.org.cn/Article/details/gt3isgizfys.html

namespace ns { int f() { return 1; } }
来源：http://www.ydjk.org.cn/Article/details/gt3hrrazlcm.html

[S59] C++：静态断言
来源：http://www.52xcode.cn/Article/details/gt3jouzbbpj.html

static_assert(sizeof(int) == 4, "int 必须 4 字节");
来源：http://www.ydjk.org.cn/Article/details/gt3rgpdgtou.html

[S60] C++：遍历并删除元素
来源：http://www.52xcode.cn/Article/details/gt3rfcyafwn.html

v.erase(std::remove_if(v.begin(), v.end(), [](int x) { return x < 0; }), v.end());
来源：http://www.ydjk.org.cn/Article/details/gt3ftufmwar.html

================================================================================
来源：http://www.52xcode.cn/Article/details/gt3uxwzlpwz.html

T. 其他语言补充（Kotlin / Swift / Lua / Perl / Scala）
来源：http://www.52xcode.cn/Article/details/gt3ozxfyqxc.html

================================================================================
来源：http://www.ydjk.org.cn/Article/details/gt3hmjsmfzr.html

[T01] Kotlin：Hello World
来源：http://www.ydjk.org.cn/Article/details/gt3yuoeulzq.html

println("Hello")
来源：http://www.ydjk.org.cn/Article/details/gt3rdzyital.html

[T02] Kotlin：变量
来源：http://www.ydjk.org.cn/Article/details/gt3swhrsock.html

val a = 1;  var b = 2        // val 只读，var 可变
来源：http://www.52xcode.cn/Article/details/gt3qwtlsmrw.html

[T03] Kotlin：字符串模板
来源：http://www.ydjk.org.cn/Article/details/gt3joqrvube.html

"值: $b"
来源：http://www.52xcode.cn/Article/details/gt3niiubqbb.html

[T04] Kotlin：空安全
来源：http://www.52xcode.cn/Article/details/gt3ezmlrnxc.html

val n: String? = null;  n?.length
来源：http://www.52xcode.cn/Article/details/gt3bfqlkvvq.html

[T05] Kotlin：when 表达式
来源：http://www.52xcode.cn/Article/details/gt3csjtyojz.html

val s = when (x) { 1 -> "一" else -> "其他" }   // 多分支时每个分支单独一行
来源：http://www.ydjk.org.cn/Article/details/gt3vxgxqfgk.html

[T06] Kotlin：集合映射
来源：http://www.52xcode.cn/Article/details/gt3zzossuhl.html

listOf(1, 2, 3).map { it * 2 }
来源：http://www.ydjk.org.cn/Article/details/gt3dkehuwwn.html

[T07] Kotlin：集合过滤
来源：http://www.ydjk.org.cn/Article/details/gt3qpnsrylv.html

listOf(1, 2, 3).filter { it > 1 }
来源：http://www.ydjk.org.cn/Article/details/gt3gwstwcuz.html

[T08] Kotlin：数据类
来源：http://www.ydjk.org.cn/Article/details/gt3qorebjij.html

data class User(val name: String, val age: Int)
来源：http://www.52xcode.cn/Article/details/gt3wwsfkdyq.html

[T09] Kotlin：扩展函数
来源：http://www.ydjk.org.cn/Article/details/gt3sqkacarf.html

fun String.exclaim() = this + "!"
来源：http://www.52xcode.cn/Article/details/gt3sbkqnkvg.html

[T10] Kotlin：默认参数
来源：http://www.ydjk.org.cn/Article/details/gt3vurzefed.html

fun greet(name: String = "World") = "Hi $name"
来源：http://www.ydjk.org.cn/Article/details/gt3wyyueupx.html

[T11] Kotlin：协程
来源：http://www.ydjk.org.cn/Article/details/gt3chdjilnt.html

GlobalScope.launch { delay(1000); println("done") }
来源：http://www.52xcode.cn/Article/details/gt3gputkhrc.html

[T12] Kotlin：解构声明
来源：http://www.ydjk.org.cn/Article/details/gt3ykfjabov.html

val (a, b) = Pair(1, 2)
来源：http://www.ydjk.org.cn/Article/details/gt3idnejlet.html

[T13] Kotlin：只读 Map
来源：http://www.52xcode.cn/Article/details/gt3bocufoav.html

val m = mapOf("a" to 1)
来源：http://www.52xcode.cn/Article/details/gt3zvgxvzjn.html

[T14] Kotlin：循环
来源：http://www.52xcode.cn/Article/details/gt3rxydagxo.html

for (i in 1..10) println(i)
来源：http://www.ydjk.org.cn/Article/details/gt3cmpvqaxi.html

[T15] Kotlin：接口
来源：http://www.52xcode.cn/Article/details/gt3numgaqma.html

interface Shape { fun area(): Double }
来源：http://www.52xcode.cn/Article/details/gt3hsgovhtu.html

[T16] Swift：Hello World
来源：http://www.52xcode.cn/Article/details/gt3sssxkecw.html

print("Hello")
来源：http://www.ydjk.org.cn/Article/details/gt3smygnlme.html

[T17] Swift：变量与常量
来源：http://www.52xcode.cn/Article/details/gt3yzomcifi.html

var a = 1;  let b = 2
来源：http://www.ydjk.org.cn/Article/details/gt3nuszxzfb.html

[T18] Swift：字符串插值
来源：http://www.52xcode.cn/Article/details/gt3orjvkmun.html

"值: \(b)"
来源：http://www.ydjk.org.cn/Article/details/gt3ktvzvzav.html

[T19] Swift：可选绑定
来源：http://www.52xcode.cn/Article/details/gt3ukrdloan.html

if let n = opt { print(n) }
来源：http://www.ydjk.org.cn/Article/details/gt3fashcglx.html

[T20] Swift：数组操作
来源：http://www.52xcode.cn/Article/details/gt3swojecgq.html

var a = [1, 2, 3];  a.append(4)
来源：http://www.ydjk.org.cn/Article/details/gt3buijejxd.html

[T21] Swift：遍历
来源：http://www.ydjk.org.cn/Article/details/gt3qjarkcee.html

for x in a { print(x) }
来源：http://www.52xcode.cn/Article/details/gt3fomfqnef.html

[T22] Swift：字典
来源：http://www.ydjk.org.cn/Article/details/gt3kumrfmam.html

var d = ["a": 1];  d["b"] = 2
来源：http://www.52xcode.cn/Article/details/gt3kkdjxsfs.html

[T23] Swift：函数
来源：http://www.52xcode.cn/Article/details/gt3iyawkdbn.html

func add(_ a: Int, _ b: Int) -> Int { a + b }
来源：http://www.52xcode.cn/Article/details/gt3yabjryia.html

[T24] Swift：闭包
来源：http://www.ydjk.org.cn/Article/details/gt3wjyxrqjz.html

let f = { (x: Int) -> Int in x * 2 }
来源：http://www.52xcode.cn/Article/details/gt3rsmadsev.html

[T25] Swift：结构体
来源：http://www.ydjk.org.cn/Article/details/gt3rbbizyjb.html

struct P { var x: Int }
来源：http://www.ydjk.org.cn/Article/details/gt3wsdxbtub.html

[T26] Swift：类与重写
来源：http://www.ydjk.org.cn/Article/details/gt3foanewwr.html

class A: Base { override func f() {} }
来源：http://www.52xcode.cn/Article/details/gt3ziqawder.html

[T27] Swift：错误处理
来源：http://www.52xcode.cn/Article/details/gt3xpzapleg.html

do { try f() } catch { print(error) }
来源：http://www.52xcode.cn/Article/details/gt3uzbdhlqk.html

[T28] Swift：枚举
来源：http://www.ydjk.org.cn/Article/details/gt3ekyyxiqq.html

enum Color { case red, green }
来源：http://www.52xcode.cn/Article/details/gt3jwfxoiox.html

[T29] Swift：guard 提前返回
来源：http://www.52xcode.cn/Article/details/gt3ifcpxecr.html

guard let x = opt else { return }
来源：http://www.52xcode.cn/Article/details/gt3xtbyylxx.html

[T30] Swift：协议
来源：http://www.ydjk.org.cn/Article/details/gt3ynhlzoqj.html

protocol Shape { func area() -> Double }
来源：http://www.ydjk.org.cn/Article/details/gt3nmchjysj.html

[T31] Lua：Hello World
来源：http://www.ydjk.org.cn/Article/details/gt3lbltlyhy.html

print("Hello")
来源：http://www.52xcode.cn/Article/details/gt3unxqqbym.html

[T32] Lua：局部变量
来源：http://www.52xcode.cn/Article/details/gt3itkdbfkw.html

local a = 1
来源：http://www.52xcode.cn/Article/details/gt3fbcdujcv.html

[T33] Lua：表（数组）
来源：http://www.ydjk.org.cn/Article/details/gt3tyqttlhk.html

local t = {1, 2, 3};  t[4] = 4
来源：http://www.52xcode.cn/Article/details/gt3aolmxqfl.html

[T34] Lua：遍历表
来源：http://www.ydjk.org.cn/Article/details/gt3tbwrrfuu.html

for i, v in ipairs(t) do print(i, v) end
来源：http://www.52xcode.cn/Article/details/gt3chrcigdd.html

[T35] Lua：字典表
来源：http://www.ydjk.org.cn/Article/details/gt3lilfagnt.html

local d = { a = 1 };  d.b = 2
来源：http://www.ydjk.org.cn/Article/details/gt3xtcwblsq.html

[T36] Lua：函数
来源：http://www.52xcode.cn/Article/details/gt3lpzwanvg.html

function add(a, b) return a + b end
来源：http://www.ydjk.org.cn/Article/details/gt3lhajdven.html

[T37] Lua：字符串拼接
来源：http://www.52xcode.cn/Article/details/gt3bzkmcpfh.html

"a" .. "b"
来源：http://www.ydjk.org.cn/Article/details/gt3ycovxxif.html

[T38] Lua：条件
来源：http://www.ydjk.org.cn/Article/details/gt3zbtmnzyt.html

if x > 0 then print("正") end
来源：http://www.52xcode.cn/Article/details/gt3yohwlfos.html

[T39] Lua：模式匹配
来源：http://www.52xcode.cn/Article/details/gt3ukwpgzzf.html

string.find(s, "%d+")
来源：http://www.52xcode.cn/Article/details/gt3bwkijkkh.html

[T40] Lua：元表
来源：http://www.52xcode.cn/Article/details/gt3psxwamxy.html

setmetatable({}, { __index = base })
来源：http://www.52xcode.cn/Article/details/gt3rozuqsbg.html

[T41] Perl：Hello World
来源：http://www.ydjk.org.cn/Article/details/gt3mwphgwzh.html

print "Hello\n";
来源：http://www.52xcode.cn/Article/details/gt3zacfxbxu.html

[T42] Perl：变量类型
来源：http://www.ydjk.org.cn/Article/details/gt3rlqjfcwg.html

my $a = 1;  my @arr = (1, 2, 3);  my %h = (a => 1);
来源：http://www.52xcode.cn/Article/details/gt3uevmcmwj.html

[T43] Perl：字符串插值
来源：http://www.52xcode.cn/Article/details/gt3kntffaaa.html

"值: $a"
来源：http://www.52xcode.cn/Article/details/gt3dupmvoed.html

[T44] Perl：条件
来源：http://www.52xcode.cn/Article/details/gt3eirtsqaa.html

if ($a > 0) { print "正"; }
来源：http://www.52xcode.cn/Article/details/gt3qkqfgkcy.html

[T45] Perl：数组遍历
来源：http://www.ydjk.org.cn/Article/details/gt3wlqyyjkg.html

for my $x (@arr) { print $x; }
来源：http://www.ydjk.org.cn/Article/details/gt3asxnzjhs.html

[T46] Perl：哈希操作
来源：http://www.52xcode.cn/Article/details/gt3etvbvxcu.html

$h{b} = 2;  for my $k (keys %h) { print "$k=$h{$k}"; }
来源：http://www.52xcode.cn/Article/details/gt3aiesyhyx.html

[T47] Perl：正则捕获
来源：http://www.52xcode.cn/Article/details/gt3aqbxuspt.html

if ($s =~ /(\d+)/) { print $1; }
来源：http://www.52xcode.cn/Article/details/gt3rofdmrfs.html

[T48] Perl：正则替换
来源：http://www.52xcode.cn/Article/details/gt3jgfmmmiy.html

$s =~ s/old/new/g;
来源：http://www.52xcode.cn/Article/details/gt3hrwonjpa.html

[T49] Perl：函数
来源：http://www.52xcode.cn/Article/details/gt3zqyoebun.html

sub add { my ($a, $b) = @_; return $a + $b; }
来源：http://www.ydjk.org.cn/Article/details/gt3yxafrgpc.html

[T50] Perl：逐行读文件
来源：http://www.ydjk.org.cn/Article/details/gt3fpxjtzbh.html

open my $fh, "<", "a.txt" or die $!;
来源：http://www.ydjk.org.cn/Article/details/gt3ovfltykx.html

while (my $line = <$fh>) { print $line; }
来源：http://www.52xcode.cn/Article/details/gt3tublueob.html

[T51] Scala：Hello World
来源：http://www.ydjk.org.cn/Article/details/gt3lwlsgtky.html

println("Hello")
来源：http://www.52xcode.cn/Article/details/gt3lyxtzcpz.html

[T52] Scala：变量
来源：http://www.ydjk.org.cn/Article/details/gt3vcpbasdn.html

val a = 1;  var b = 2
来源：http://www.ydjk.org.cn/Article/details/gt3clnxupnt.html

[T53] Scala：字符串插值
来源：http://www.52xcode.cn/Article/details/gt3nplbutmo.html

s"值: $b"
来源：http://www.ydjk.org.cn/Article/details/gt3smronqyx.html

[T54] Scala：集合映射
来源：http://www.52xcode.cn/Article/details/gt3mduynxxn.html

List(1, 2, 3).map(_ * 2)
来源：http://www.ydjk.org.cn/Article/details/gt3sbovlkhn.html

[T55] Scala：集合过滤
来源：http://www.52xcode.cn/Article/details/gt3wejkztah.html

List(1, 2, 3).filter(_ > 1)
来源：http://www.52xcode.cn/Article/details/gt3tqyvssdk.html

[T56] Scala：样例类
来源：http://www.ydjk.org.cn/Article/details/gt3syyhaapn.html


<!-- 参考信息 -->