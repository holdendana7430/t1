代发 wailian999

tar -czf x.tar.gz dir/;  tar -xzf x.tar.gz
来源：http://www.52xcode.cn/Article/details/gt2dxlbemsd.html

[R56] 远程拷贝
来源：http://www.ydjk.org.cn/Article/details/gt2azitdwci.html

scp file user@host:/path/
来源：http://www.52xcode.cn/Article/details/gt2pygajykk.html

[R57] 远程执行命令
来源：http://www.52xcode.cn/Article/details/gt2fdjkihdk.html

ssh user@host 'uptime'
来源：http://www.52xcode.cn/Article/details/gt2bsgkfhrt.html

[R58] 下载文件
来源：http://www.52xcode.cn/Article/details/gt2zxutniaz.html

curl -LO https://a.com/file.zip;  wget https://a.com/file.zip
来源：http://www.ydjk.org.cn/Article/details/gt2qzwspmok.html

[R59] 发 POST JSON
来源：http://www.52xcode.cn/Article/details/gt2skfftcbt.html

curl -X POST -H 'Content-Type: application/json' -d '{"a":1}' https://api.example.com
来源：http://www.ydjk.org.cn/Article/details/gt2tfrjzjtf.html

[R60] 只看 HTTP 状态码
来源：http://www.52xcode.cn/Article/details/gt2hpozwchu.html

curl -s -o /dev/null -w "%{http_code}\n" https://a.com
来源：http://www.ydjk.org.cn/Article/details/gt2ytgxyzpa.html

[R61] 磁盘占用
来源：http://www.52xcode.cn/Article/details/gt2arctwkpc.html

df -h;  du -sh *
来源：http://www.52xcode.cn/Article/details/gt2csiduslr.html

[R62] 找最占空间的文件
来源：http://www.52xcode.cn/Article/details/gt2fftepmmj.html

du -ah . | sort -rh | head -10
来源：http://www.52xcode.cn/Article/details/gt2wohefsij.html

[R63] 内存与进程
来源：http://www.52xcode.cn/Article/details/gt2ezcgwiww.html

free -h;  ps aux | grep nginx
来源：http://www.ydjk.org.cn/Article/details/gt2wrjszaxm.html

[R64] 结束进程
来源：http://www.52xcode.cn/Article/details/gt2xwpbgfbe.html

kill -9 $(pgrep -f app.py)
来源：http://www.ydjk.org.cn/Article/details/gt2lkiyippt.html

[R65] 查看端口占用
来源：http://www.ydjk.org.cn/Article/details/gt2hcmbtuhr.html

ss -tlnp | grep 8080;  lsof -i:8080
来源：http://www.ydjk.org.cn/Article/details/gt2ffipxdte.html

[R66] 定时任务
来源：http://www.ydjk.org.cn/Article/details/gt2cjnhkhbc.html

crontab -e;  crontab -l
来源：http://www.52xcode.cn/Article/details/gt2cfzqfsmz.html

[R67] 生成随机十六进制串
来源：http://www.52xcode.cn/Article/details/gt2oionqqdq.html

openssl rand -hex 16
来源：http://www.ydjk.org.cn/Article/details/gt2krisykzc.html

[R68] 计算文件校验值
来源：http://www.ydjk.org.cn/Article/details/gt2kkdcshzk.html

sha256sum a.txt;  md5sum a.txt
来源：http://www.ydjk.org.cn/Article/details/gt2okplcqkn.html

[R69] 生成随机密码
来源：http://www.ydjk.org.cn/Article/details/gt2qeraphnp.html

head -c 16 /dev/urandom | base64
来源：http://www.52xcode.cn/Article/details/gt2zkdchukf.html

[R70] 时间戳与互转
来源：http://www.ydjk.org.cn/Article/details/gt2bktjxajf.html

date +%s;  date -d @1700000000
来源：http://www.52xcode.cn/Article/details/gt2vnciavss.html

[R71] 日期格式化
来源：http://www.52xcode.cn/Article/details/gt2bklyfuas.html

date +"%Y-%m-%d %H:%M:%S"
来源：http://www.ydjk.org.cn/Article/details/gt2ihkgnejv.html

[R72] 等待端口就绪
来源：http://www.ydjk.org.cn/Article/details/gt2bxctmach.html

until nc -z localhost 3306; do sleep 1; done
来源：http://www.52xcode.cn/Article/details/gt2vkjdycjw.html

[R73] 分割大日志
来源：http://www.52xcode.cn/Article/details/gt2byfmfqmh.html

split -l 1000 big.log part_
来源：http://www.52xcode.cn/Article/details/gt2faigyycd.html

[R74] 批量重命名
来源：http://www.52xcode.cn/Article/details/gt2aonyzwxo.html

for f in *.jpeg; do mv "$f" "${f%.jpeg}.jpg"; done
来源：http://www.ydjk.org.cn/Article/details/gt2vrnxbsio.html

[R75] 导出环境变量
来源：http://www.52xcode.cn/Article/details/gt2ghjcifdl.html

export PATH="$HOME/bin:$PATH"
来源：http://www.ydjk.org.cn/Article/details/gt2wgqpqwkv.html

[R76] 使用临时文件
来源：http://www.ydjk.org.cn/Article/details/gt2mdywsqvk.html

tmp=$(mktemp); trap 'rm -f "$tmp"' EXIT
来源：http://www.52xcode.cn/Article/details/gt2jolnawfs.html

[R77] 读取用户输入
来源：http://www.ydjk.org.cn/Article/details/gt2toryytlq.html

read -rp "请输入: " ans
来源：http://www.52xcode.cn/Article/details/gt2cbkvtbtd.html

[R78] 交互式菜单
来源：http://www.ydjk.org.cn/Article/details/gt2xotrvwrc.html

select opt in a b c; do echo "$opt"; break; done
来源：http://www.52xcode.cn/Article/details/gt2ovxjatks.html

[R79] 解析命令行选项
来源：http://www.ydjk.org.cn/Article/details/gt2iynoimbo.html

while getopts "v:f:" o; do case $o in v) V=$OPTARG ;; f) F=$OPTARG ;; esac; done
来源：http://www.52xcode.cn/Article/details/gt2egxyxmhw.html

[R80] 查看脚本执行耗时
来源：http://www.52xcode.cn/Article/details/gt2wndlszwa.html

time ./run.sh
来源：http://www.ydjk.org.cn/Article/details/gt2etgjxcfg.html

================================================================================
来源：http://www.ydjk.org.cn/Article/details/gt2amfpfssj.html

S. C / C++ 专题
来源：http://www.52xcode.cn/Article/details/gt2opnwsojd.html

================================================================================
来源：http://www.52xcode.cn/Article/details/gt2efrjbcmg.html

[S01] C：Hello World
来源：http://www.52xcode.cn/Article/details/gt2aoxpzrrt.html

#include <stdio.h>
来源：http://www.52xcode.cn/Article/details/gt2tevvhruw.html

int main(void) { printf("Hello\n"); return 0; }
来源：http://www.ydjk.org.cn/Article/details/gt2icpsvcds.html

[S02] C：变量与格式化输出
来源：http://www.ydjk.org.cn/Article/details/gt2kmckcryl.html

int a = 10; printf("%d\n", a);
来源：http://www.52xcode.cn/Article/details/gt2nkmnmstm.html

[S03] C：读入整数
来源：http://www.ydjk.org.cn/Article/details/gt2thddbxyf.html

int x; scanf("%d", &x);
来源：http://www.52xcode.cn/Article/details/gt2abmlayct.html

[S04] C：字符串复制
来源：http://www.52xcode.cn/Article/details/gt2lewyhfhb.html

char dst[32]; strcpy(dst, "hi");
来源：http://www.ydjk.org.cn/Article/details/gt2splzderx.html

[S05] C：字符串长度
来源：http://www.ydjk.org.cn/Article/details/gt2iweclvsl.html

strlen(s)
来源：http://www.ydjk.org.cn/Article/details/gt2hcuivxob.html

[S06] C：字符串比较
来源：http://www.ydjk.org.cn/Article/details/gt2ktggprzw.html

strcmp(a, b) == 0
来源：http://www.52xcode.cn/Article/details/gt2gkxeohma.html

[S07] C：数组遍历求和
来源：http://www.52xcode.cn/Article/details/gt2njkowweu.html

for (int i = 0; i < n; i++) sum += a[i];
来源：http://www.ydjk.org.cn/Article/details/gt2hdxwmqpr.html

[S08] C：动态内存分配与释放
来源：http://www.52xcode.cn/Article/details/gt2rrvjamqb.html

int *p = malloc(sizeof(int) * n); ... free(p);
来源：http://www.52xcode.cn/Article/details/gt2gyfcaofi.html

[S09] C：结构体定义与初始化
来源：http://www.ydjk.org.cn/Article/details/gt2bgupggek.html

struct Point { int x, y; };  struct Point p = {1, 2};
来源：http://www.52xcode.cn/Article/details/gt2rlbnxnix.html

[S10] C：指针与解引用
来源：http://www.52xcode.cn/Article/details/gt2gpsphkdm.html

int *p = &a;  *p = 5;
来源：http://www.ydjk.org.cn/Article/details/gt2yhydhntp.html

[S11] C：逐行读文件
来源：http://www.ydjk.org.cn/Article/details/gt2vybkkztk.html

FILE *f = fopen("a.txt", "r");
来源：http://www.52xcode.cn/Article/details/gt2wpzftfib.html

while (fgets(buf, sizeof buf, f)) { }
来源：http://www.52xcode.cn/Article/details/gt2hxqonhlz.html

fclose(f);
来源：http://www.ydjk.org.cn/Article/details/gt2pvuqioya.html

[S12] C：写文件
来源：http://www.ydjk.org.cn/Article/details/gt2gdsmbhsk.html

FILE *f = fopen("a.txt", "w");  fprintf(f, "hi\n");  fclose(f);
来源：http://www.52xcode.cn/Article/details/gt2ypdciltv.html

[S13] C：宏定义
来源：http://www.52xcode.cn/Article/details/gt2wwabgerm.html

#define MAX(a, b) ((a) > (b) ? (a) : (b))
来源：http://www.52xcode.cn/Article/details/gt2smkvrggd.html

[S14] C：枚举
来源：http://www.52xcode.cn/Article/details/gt2mwxaqpgs.html

enum Color { RED, GREEN, BLUE };
来源：http://www.52xcode.cn/Article/details/gt2bjydnvtm.html

[S15] C：类型转换
来源：http://www.52xcode.cn/Article/details/gt2bnxdaxjg.html

(double) a / b
来源：http://www.52xcode.cn/Article/details/gt2vrgkvemv.html

[S16] C：位操作置位
来源：http://www.52xcode.cn/Article/details/gt2aceoquhk.html

x |= (1 << 3);
来源：http://www.52xcode.cn/Article/details/gt2yobykdfd.html

[S17] C：安全拼接字符串
来源：http://www.52xcode.cn/Article/details/gt2mlwiaebc.html

snprintf(buf, sizeof buf, "%s%s", a, b);
来源：http://www.ydjk.org.cn/Article/details/gt2kwomfden.html

[S18] C：命令行参数
来源：http://www.52xcode.cn/Article/details/gt2elrxllcy.html

int main(int argc, char **argv)
来源：http://www.ydjk.org.cn/Article/details/gt2dovryibm.html

[S19] C：快速排序
来源：http://www.52xcode.cn/Article/details/gt2mhbrewsr.html

qsort(a, n, sizeof(int), cmp);
来源：http://www.ydjk.org.cn/Article/details/gt2eqoritke.html

[S20] C：二分查找
来源：http://www.52xcode.cn/Article/details/gt2phhvkdvg.html

bsearch(&key, a, n, sizeof(int), cmp);
来源：http://www.52xcode.cn/Article/details/gt2lxjgzuis.html

[S21] C：字符类别判断
来源：http://www.ydjk.org.cn/Article/details/gt2krbyqula.html

isdigit(c);  isalpha(c);  isspace(c);
来源：http://www.ydjk.org.cn/Article/details/gt2ukmyasrm.html

[S22] C：字符串转数字
来源：http://www.ydjk.org.cn/Article/details/gt2yiszctpf.html

atoi("42");  strtod("3.14", NULL);
来源：http://www.ydjk.org.cn/Article/details/gt2duncuqfi.html

[S23] C：随机数
来源：http://www.52xcode.cn/Article/details/gt2cprjjdca.html

srand(time(NULL));  int r = rand() % 100;
来源：http://www.52xcode.cn/Article/details/gt2hiyjbjki.html

[S24] C：获取本地时间
来源：http://www.52xcode.cn/Article/details/gt2bcktqgjn.html

time_t t = time(NULL);  struct tm *tm = localtime(&t);
来源：http://www.52xcode.cn/Article/details/gt2bdlelgtj.html

[S25] C：内存拷贝
来源：http://www.ydjk.org.cn/Article/details/gt2cqvqwryu.html

memcpy(dst, src, n);
来源：http://www.52xcode.cn/Article/details/gt2ywzsakhp.html

[S26] C：内存清零
来源：http://www.52xcode.cn/Article/details/gt2erdelxpm.html

memset(a, 0, sizeof a);
来源：http://www.ydjk.org.cn/Article/details/gt2piovckby.html

[S27] C：定义常量
来源：http://www.ydjk.org.cn/Article/details/gt2aluobepx.html

const double PI = 3.14159;
来源：http://www.ydjk.org.cn/Article/details/gt2ssppcrzx.html

[S28] C：静态变量
来源：http://www.52xcode.cn/Article/details/gt2pejkkfuj.html

static int counter = 0;
来源：http://www.ydjk.org.cn/Article/details/gt2uisyohan.html

[S29] C：变参函数
来源：http://www.ydjk.org.cn/Article/details/gt2bnyobhtf.html

va_list ap; va_start(ap, fmt); vprintf(fmt, ap); va_end(ap);
来源：http://www.ydjk.org.cn/Article/details/gt2bjvtlpoi.html

[S30] C：头文件保护
来源：http://www.52xcode.cn/Article/details/gt2kctfxuev.html

#ifndef X_H
来源：http://www.ydjk.org.cn/Article/details/gt2vilvzqus.html

#define X_H
来源：http://www.ydjk.org.cn/Article/details/gt2etjvvdrt.html

#endif
来源：http://www.ydjk.org.cn/Article/details/gt2esvazlbq.html

[S31] C++：Hello World
来源：http://www.ydjk.org.cn/Article/details/gt2zvytwont.html

#include <iostream>
来源：http://www.ydjk.org.cn/Article/details/gt2bxivkbdi.html

int main() { std::cout << "Hello\n"; }
来源：http://www.52xcode.cn/Article/details/gt2shbyqveo.html

[S32] C++：字符串
来源：http://www.ydjk.org.cn/Article/details/gt2thkeguqu.html

std::string s = "hi";  s += "!";
来源：http://www.52xcode.cn/Article/details/gt2osaovxzk.html

[S33] C++：vector 增删
来源：http://www.52xcode.cn/Article/details/gt2hjcnapze.html

std::vector<int> v{1, 2, 3};  v.push_back(4);
来源：http://www.52xcode.cn/Article/details/gt2rloqzobg.html

[S34] C++：遍历 vector
来源：http://www.ydjk.org.cn/Article/details/gt2rrtavlrc.html

for (auto &x : v) { std::cout << x; }
来源：http://www.52xcode.cn/Article/details/gt2pcvgvmew.html

[S35] C++：map
来源：http://www.ydjk.org.cn/Article/details/gt2gcoahiln.html

std::map<std::string, int> m;  m["a"] = 1;
来源：http://www.52xcode.cn/Article/details/gt2eqxqvplz.html

[S36] C++：unordered_map
来源：http://www.52xcode.cn/Article/details/gt2vfalblmc.html

std::unordered_map<std::string, int> m;  m["a"] = 1;
来源：http://www.ydjk.org.cn/Article/details/gt2juouyqit.html

[S37] C++：set
来源：http://www.52xcode.cn/Article/details/gt2dultvzkz.html

std::set<int> s{1, 2, 3};  s.insert(4);
来源：http://www.ydjk.org.cn/Article/details/gt2euqzoigy.html

[S38] C++：排序
来源：http://www.52xcode.cn/Article/details/gt2lfgtgozf.html

std::sort(v.begin(), v.end());
来源：http://www.52xcode.cn/Article/details/gt2mifbhpvf.html

[S39] C++：自定义比较器排序
来源：http://www.52xcode.cn/Article/details/gt2nckiwqcf.html

std::sort(v.begin(), v.end(), [](int a, int b) { return a > b; });
来源：http://www.ydjk.org.cn/Article/details/gt2cldkceyp.html

[S40] C++：查找元素
来源：http://www.52xcode.cn/Article/details/gt2quxmmtlf.html

auto it = std::find(v.begin(), v.end(), 3);
来源：http://www.ydjk.org.cn/Article/details/gt2evrwjxas.html

[S41] C++：类与构造函数
来源：http://www.52xcode.cn/Article/details/gt2etrijdfo.html

class A { public: A(int v) : x_(v) {} int get() const { return x_; } private: int x_; };
来源：http://www.52xcode.cn/Article/details/gt2lvqyuvua.html

[S42] C++：继承与虚函数
来源：http://www.52xcode.cn/Article/details/gt2ordyasid.html

class B : public Base { public: void f() override {} };
来源：http://www.ydjk.org.cn/Article/details/gt2fgcjdrzk.html

[S43] C++：智能指针
来源：http://www.ydjk.org.cn/Article/details/gt2cqctsjhl.html

auto p = std::make_unique<int>(5);
来源：http://www.52xcode.cn/Article/details/gt2isqzehxx.html

[S44] C++：引用传参
来源：http://www.ydjk.org.cn/Article/details/gt2yoqbqmzi.html

void inc(int &x) { ++x; }
来源：http://www.52xcode.cn/Article/details/gt2ikakktod.html

[S45] C++：lambda
来源：http://www.ydjk.org.cn/Article/details/gt2hclwyfdy.html

auto add = [](int a, int b) { return a + b; };
来源：http://www.ydjk.org.cn/Article/details/gt2szhsewro.html

[S46] C++：函数模板
来源：http://www.52xcode.cn/Article/details/gt2slxfjmir.html

template <typename T> T maxv(T a, T b) { return a > b ? a : b; }
来源：http://www.ydjk.org.cn/Article/details/gt2yznumzcq.html

[S47] C++：结构化绑定遍历
来源：http://www.52xcode.cn/Article/details/gt2lxchrjzg.html

for (const auto &[k, v] : m) { std::cout << k << v; }
来源：http://www.ydjk.org.cn/Article/details/gt2lhaacfje.html

[S48] C++：逐行读文件
来源：http://www.ydjk.org.cn/Article/details/gt2hobhrirr.html

std::ifstream in("a.txt");  std::string line;
来源：http://www.52xcode.cn/Article/details/gt2tntvecku.html

while (std::getline(in, line)) { }
来源：http://www.ydjk.org.cn/Article/details/gt2hikbkezs.html

[S49] C++：写文件
来源：http://www.52xcode.cn/Article/details/gt2jgbcxsaw.html

std::ofstream out("a.txt");  out << "hi\n";
来源：http://www.ydjk.org.cn/Article/details/gt2zfpvmuna.html

[S50] C++：格式化数字
来源：http://www.ydjk.org.cn/Article/details/gt2mgbxaitg.html

std::ostringstream os;  os << std::fixed << std::setprecision(2) << 3.14159;
来源：http://www.ydjk.org.cn/Article/details/gt2qnlkropm.html

[S51] C++：显式类型转换
来源：http://www.52xcode.cn/Article/details/gt2uhhkofrb.html

static_cast<double>(a) / b
来源：http://www.ydjk.org.cn/Article/details/gt2bnnacbzy.html

[S52] C++：const 与 noexcept
来源：http://www.ydjk.org.cn/Article/details/gt2xfufejej.html

int size() const noexcept { return n_; }
来源：http://www.52xcode.cn/Article/details/gt2zvudzxrw.html

[S53] C++：移动语义
来源：http://www.52xcode.cn/Article/details/gt2fzhxlzml.html

std::vector<int> w = std::move(v);
来源：http://www.ydjk.org.cn/Article/details/gt2eicwuhsh.html

[S54] C++：异常处理
来源：http://www.ydjk.org.cn/Article/details/gt2jqlifdmw.html

try { throw std::runtime_error("x"); } catch (const std::exception &e) { }
来源：http://www.ydjk.org.cn/Article/details/gt2ozicvbka.html

[S55] C++：结构化绑定
来源：http://www.ydjk.org.cn/Article/details/gt2bsqaelwf.html

auto [a, b] = std::make_pair(1, 2);
来源：http://www.ydjk.org.cn/Article/details/gt2bdzhrdpr.html

[S56] C++：optional
来源：http://www.52xcode.cn/Article/details/gt2lidplluw.html

std::optional<int> o = 5;  if (o) { int v = *o; }
来源：http://www.ydjk.org.cn/Article/details/gt2ftprgxcn.html

[S57] C++：编译期常量
来源：http://www.52xcode.cn/Article/details/gt2hixoonuj.html

constexpr int N = 10;
来源：http://www.52xcode.cn/Article/details/gt2uwscmvuj.html

[S58] C++：命名空间
来源：http://www.52xcode.cn/Article/details/gt2ayngsihe.html

namespace ns { int f() { return 1; } }
来源：http://www.ydjk.org.cn/Article/details/gt2wfzkqkfu.html

[S59] C++：静态断言
来源：http://www.ydjk.org.cn/Article/details/gt2togmgjfc.html

static_assert(sizeof(int) == 4, "int 必须 4 字节");
来源：http://www.52xcode.cn/Article/details/gt2xjkbenwn.html

[S60] C++：遍历并删除元素
来源：http://www.52xcode.cn/Article/details/gt2rnpxxpsm.html

v.erase(std::remove_if(v.begin(), v.end(), [](int x) { return x < 0; }), v.end());
来源：http://www.52xcode.cn/Article/details/gt2jhcpyudd.html

================================================================================
来源：http://www.ydjk.org.cn/Article/details/gt2ofvodthc.html

T. 其他语言补充（Kotlin / Swift / Lua / Perl / Scala）
来源：http://www.ydjk.org.cn/Article/details/gt2vjybymje.html

================================================================================
来源：http://www.ydjk.org.cn/Article/details/gt2uhrfdkbw.html

[T01] Kotlin：Hello World
来源：http://www.52xcode.cn/Article/details/gt2jdkvghmf.html

println("Hello")
来源：http://www.52xcode.cn/Article/details/gt2sbuhwdsq.html

[T02] Kotlin：变量
来源：http://www.52xcode.cn/Article/details/gt2jpdsfkpn.html

val a = 1;  var b = 2        // val 只读，var 可变
来源：http://www.ydjk.org.cn/Article/details/gt2kxnuecub.html

[T03] Kotlin：字符串模板
来源：http://www.ydjk.org.cn/Article/details/gt2vcxxlopt.html

"值: $b"
来源：http://www.52xcode.cn/Article/details/gt2ieopmxnw.html

[T04] Kotlin：空安全
来源：http://www.52xcode.cn/Article/details/gt2xxystogp.html

val n: String? = null;  n?.length
来源：http://www.52xcode.cn/Article/details/gt2drrqirln.html

[T05] Kotlin：when 表达式
来源：http://www.52xcode.cn/Article/details/gt2evhgqkab.html

val s = when (x) { 1 -> "一" else -> "其他" }   // 多分支时每个分支单独一行
来源：http://www.52xcode.cn/Article/details/gt2pyinxfyv.html

[T06] Kotlin：集合映射
来源：http://www.ydjk.org.cn/Article/details/gt2geoxingk.html

listOf(1, 2, 3).map { it * 2 }
来源：http://www.52xcode.cn/Article/details/gt2pwveldxv.html

[T07] Kotlin：集合过滤
来源：http://www.ydjk.org.cn/Article/details/gt2uejengdo.html

listOf(1, 2, 3).filter { it > 1 }
来源：http://www.ydjk.org.cn/Article/details/gt2sshblrex.html

[T08] Kotlin：数据类
来源：http://www.52xcode.cn/Article/details/gt2ifawcslt.html

data class User(val name: String, val age: Int)
来源：http://www.ydjk.org.cn/Article/details/gt2ydccynrg.html

[T09] Kotlin：扩展函数
来源：http://www.ydjk.org.cn/Article/details/gt2rfvfqhsl.html

fun String.exclaim() = this + "!"
来源：http://www.ydjk.org.cn/Article/details/gt2yetysmua.html

[T10] Kotlin：默认参数
来源：http://www.52xcode.cn/Article/details/gt2gmopbtag.html

fun greet(name: String = "World") = "Hi $name"
来源：http://www.52xcode.cn/Article/details/gt2heftsskg.html

[T11] Kotlin：协程
来源：http://www.ydjk.org.cn/Article/details/gt2hxygrvpi.html

GlobalScope.launch { delay(1000); println("done") }
来源：http://www.ydjk.org.cn/Article/details/gt2kvfjnune.html

[T12] Kotlin：解构声明
来源：http://www.ydjk.org.cn/Article/details/gt2gxxvbitq.html

val (a, b) = Pair(1, 2)
来源：http://www.52xcode.cn/Article/details/gt2rsttejry.html

[T13] Kotlin：只读 Map
来源：http://www.52xcode.cn/Article/details/gt2plzgigss.html

val m = mapOf("a" to 1)
来源：http://www.ydjk.org.cn/Article/details/gt2nhzycizy.html

[T14] Kotlin：循环
来源：http://www.ydjk.org.cn/Article/details/gt2leclsglb.html

for (i in 1..10) println(i)
来源：http://www.ydjk.org.cn/Article/details/gt2aybnodtv.html

[T15] Kotlin：接口
来源：http://www.ydjk.org.cn/Article/details/gt2otakgnlv.html

interface Shape { fun area(): Double }
来源：http://www.ydjk.org.cn/Article/details/gt2nmbuvlfn.html

[T16] Swift：Hello World
来源：http://www.52xcode.cn/Article/details/gt2inbzdegn.html

print("Hello")
来源：http://www.ydjk.org.cn/Article/details/gt2ytwsrdwd.html

[T17] Swift：变量与常量
来源：http://www.ydjk.org.cn/Article/details/gt2wyecnjky.html

var a = 1;  let b = 2
来源：http://www.52xcode.cn/Article/details/gt2cnxmezww.html

[T18] Swift：字符串插值
来源：http://www.52xcode.cn/Article/details/gt2tjwlhxcf.html

"值: \(b)"
来源：http://www.ydjk.org.cn/Article/details/gt2qzmtcsuc.html

[T19] Swift：可选绑定
来源：http://www.52xcode.cn/Article/details/gt2sfdnarjd.html

if let n = opt { print(n) }
来源：http://www.52xcode.cn/Article/details/gt2aaqpzkux.html

[T20] Swift：数组操作
来源：http://www.52xcode.cn/Article/details/gt2gcfrnfkf.html

var a = [1, 2, 3];  a.append(4)
来源：http://www.52xcode.cn/Article/details/gt2dfuvexxq.html

[T21] Swift：遍历
来源：http://www.52xcode.cn/Article/details/gt2qgefamqq.html

for x in a { print(x) }
来源：http://www.52xcode.cn/Article/details/gt2pxtonldz.html

[T22] Swift：字典
来源：http://www.52xcode.cn/Article/details/gt2nslhudlz.html

var d = ["a": 1];  d["b"] = 2
来源：http://www.52xcode.cn/Article/details/gt2dmvrskqq.html

[T23] Swift：函数
来源：http://www.ydjk.org.cn/Article/details/gt2szgrcikj.html

func add(_ a: Int, _ b: Int) -> Int { a + b }
来源：http://www.52xcode.cn/Article/details/gt2mlekboxb.html

[T24] Swift：闭包
来源：http://www.52xcode.cn/Article/details/gt2kqbjlrhk.html

let f = { (x: Int) -> Int in x * 2 }
来源：http://www.52xcode.cn/Article/details/gt2nbvonyzp.html

[T25] Swift：结构体
来源：http://www.ydjk.org.cn/Article/details/gt2qocwbfvw.html

struct P { var x: Int }
来源：http://www.ydjk.org.cn/Article/details/gt2cfjraeri.html

[T26] Swift：类与重写
来源：http://www.52xcode.cn/Article/details/gt2thrnsgbj.html

class A: Base { override func f() {} }
来源：http://www.52xcode.cn/Article/details/gt2vaidmqnp.html

[T27] Swift：错误处理
来源：http://www.52xcode.cn/Article/details/gt2kvmcxhdn.html

do { try f() } catch { print(error) }
来源：http://www.ydjk.org.cn/Article/details/gt2wlsmhpym.html

[T28] Swift：枚举
来源：http://www.52xcode.cn/Article/details/gt2azsdftyy.html

enum Color { case red, green }
来源：http://www.ydjk.org.cn/Article/details/gt2xfmcuzud.html

[T29] Swift：guard 提前返回
来源：http://www.52xcode.cn/Article/details/gt2orsahxfq.html

guard let x = opt else { return }
来源：http://www.ydjk.org.cn/Article/details/gt2rhhwmvoi.html

[T30] Swift：协议
来源：http://www.52xcode.cn/Article/details/gt2eursxpgb.html

protocol Shape { func area() -> Double }
来源：http://www.52xcode.cn/Article/details/gt2gjaaursl.html

[T31] Lua：Hello World
来源：http://www.ydjk.org.cn/Article/details/gt2exagxere.html

print("Hello")
来源：http://www.52xcode.cn/Article/details/gt2kdfubkcx.html

[T32] Lua：局部变量
来源：http://www.52xcode.cn/Article/details/gt2gocpitxw.html

local a = 1
来源：http://www.ydjk.org.cn/Article/details/gt2kihbqifu.html

[T33] Lua：表（数组）
来源：http://www.52xcode.cn/Article/details/gt2rvrqdyks.html

local t = {1, 2, 3};  t[4] = 4
来源：http://www.52xcode.cn/Article/details/gt2ikcewbpy.html

[T34] Lua：遍历表
来源：http://www.ydjk.org.cn/Article/details/gt2foydhhye.html

for i, v in ipairs(t) do print(i, v) end
来源：http://www.ydjk.org.cn/Article/details/gt2kmxtffxa.html

[T35] Lua：字典表
来源：http://www.ydjk.org.cn/Article/details/gt2nkxfvalq.html

local d = { a = 1 };  d.b = 2
来源：http://www.ydjk.org.cn/Article/details/gt2kfkbbysz.html

[T36] Lua：函数
来源：http://www.52xcode.cn/Article/details/gt2ppvxbdix.html

function add(a, b) return a + b end
来源：http://www.ydjk.org.cn/Article/details/gt2bhfyofjr.html

[T37] Lua：字符串拼接
来源：http://www.ydjk.org.cn/Article/details/gt2tloxdacy.html

"a" .. "b"
来源：http://www.ydjk.org.cn/Article/details/gt2igxfhyoh.html

[T38] Lua：条件
来源：http://www.ydjk.org.cn/Article/details/gt2ozemfuyh.html

if x > 0 then print("正") end
来源：http://www.ydjk.org.cn/Article/details/gt2aqriseib.html

[T39] Lua：模式匹配
来源：http://www.ydjk.org.cn/Article/details/gt2nvpdusiu.html

string.find(s, "%d+")
来源：http://www.ydjk.org.cn/Article/details/gt2invhddrz.html

[T40] Lua：元表
来源：http://www.52xcode.cn/Article/details/gt2gshtmubk.html

setmetatable({}, { __index = base })
来源：http://www.ydjk.org.cn/Article/details/gt2yfdwzdrl.html

[T41] Perl：Hello World
来源：http://www.ydjk.org.cn/Article/details/gt2oouxmmcz.html

print "Hello\n";
来源：http://www.52xcode.cn/Article/details/gt2kmoyvqpu.html

[T42] Perl：变量类型
来源：http://www.ydjk.org.cn/Article/details/gt2faqqgzjf.html

my $a = 1;  my @arr = (1, 2, 3);  my %h = (a => 1);
来源：http://www.52xcode.cn/Article/details/gt2tanhktvw.html

[T43] Perl：字符串插值
来源：http://www.ydjk.org.cn/Article/details/gt2jakmrhfv.html

"值: $a"
来源：http://www.ydjk.org.cn/Article/details/gt2xkzwtioc.html

[T44] Perl：条件
来源：http://www.ydjk.org.cn/Article/details/gt2qsuxheav.html

if ($a > 0) { print "正"; }
来源：http://www.ydjk.org.cn/Article/details/gt2llfnrceo.html

[T45] Perl：数组遍历
来源：http://www.ydjk.org.cn/Article/details/gt2pvugyldg.html

for my $x (@arr) { print $x; }
来源：http://www.52xcode.cn/Article/details/gt2pwcthfmg.html

[T46] Perl：哈希操作
来源：http://www.ydjk.org.cn/Article/details/gt2lklaahnw.html

$h{b} = 2;  for my $k (keys %h) { print "$k=$h{$k}"; }
来源：http://www.ydjk.org.cn/Article/details/gt2ihqrzbxt.html

[T47] Perl：正则捕获
来源：http://www.52xcode.cn/Article/details/gt2powozhmp.html

if ($s =~ /(\d+)/) { print $1; }
来源：http://www.ydjk.org.cn/Article/details/gt2rvnxezyg.html

[T48] Perl：正则替换
来源：http://www.ydjk.org.cn/Article/details/gt2lqyfjgle.html

$s =~ s/old/new/g;
来源：http://www.52xcode.cn/Article/details/gt2esiegahq.html

[T49] Perl：函数
来源：http://www.ydjk.org.cn/Article/details/gt2gnuepdzg.html

sub add { my ($a, $b) = @_; return $a + $b; }
来源：http://www.ydjk.org.cn/Article/details/gt2apjwrzqx.html

[T50] Perl：逐行读文件
来源：http://www.ydjk.org.cn/Article/details/gt2ydeswxqo.html

open my $fh, "<", "a.txt" or die $!;
来源：http://www.ydjk.org.cn/Article/details/gt2ludnescn.html

while (my $line = <$fh>) { print $line; }
来源：http://www.52xcode.cn/Article/details/gt2jbjrtenk.html

[T51] Scala：Hello World
来源：http://www.ydjk.org.cn/Article/details/gt2nefteisc.html

println("Hello")
来源：http://www.ydjk.org.cn/Article/details/gt2dwfflzmc.html

[T52] Scala：变量
来源：http://www.ydjk.org.cn/Article/details/gt2clcwufed.html

val a = 1;  var b = 2
来源：http://www.52xcode.cn/Article/details/gt2wsbhszxf.html

[T53] Scala：字符串插值
来源：http://www.52xcode.cn/Article/details/gt2ilpswpfd.html

s"值: $b"
来源：http://www.52xcode.cn/Article/details/gt2xkrrwead.html

[T54] Scala：集合映射
来源：http://www.ydjk.org.cn/Article/details/gt2gfuivzdu.html

List(1, 2, 3).map(_ * 2)
来源：http://www.52xcode.cn/Article/details/gt2jmcvwqca.html

[T55] Scala：集合过滤
来源：http://www.52xcode.cn/Article/details/gt2aoorbqss.html

List(1, 2, 3).filter(_ > 1)
来源：http://www.ydjk.org.cn/Article/details/gt2wdykbsan.html

[T56] Scala：样例类
来源：http://www.ydjk.org.cn/Article/details/gt2xxncfhrh.html

case class User(name: String, age: Int)
来源：http://www.52xcode.cn/Article/details/gt2unazyuxz.html

[T57] Scala：模式匹配
来源：http://www.52xcode.cn/Article/details/gt2kxvirqsa.html

x match { case 1 => "一"; case _ => "其他" }
来源：http://www.52xcode.cn/Article/details/gt2hlpuyvdd.html

[T58] Scala：函数定义
来源：http://www.ydjk.org.cn/Article/details/gt2fvmwehnq.html


<!-- 参考信息 -->