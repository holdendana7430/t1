代发 wailian999

head -n 20 a.txt;  tail -f -n 100 app.log
来源：http://www.ydjk.org.cn/Article/details/gt3yfxitmzj.html

[R54] 比较两个文件
来源：http://www.52xcode.cn/Article/details/gt3mmqtvwlw.html

diff a.txt b.txt
来源：http://www.ydjk.org.cn/Article/details/gt3jaawyodq.html

[R55] 压缩与解压
来源：http://www.52xcode.cn/Article/details/gt3ypnqskme.html

tar -czf x.tar.gz dir/;  tar -xzf x.tar.gz
来源：http://www.ydjk.org.cn/Article/details/gt3iqquhpci.html

[R56] 远程拷贝
来源：http://www.ydjk.org.cn/Article/details/gt3swftogrg.html

scp file user@host:/path/
来源：http://www.52xcode.cn/Article/details/gt3lnpxzlfk.html

[R57] 远程执行命令
来源：http://www.ydjk.org.cn/Article/details/gt3hbdkussa.html

ssh user@host 'uptime'
来源：http://www.52xcode.cn/Article/details/gt3fazlnxmv.html

[R58] 下载文件
来源：http://www.ydjk.org.cn/Article/details/gt3bdefgfwk.html

curl -LO https://a.com/file.zip;  wget https://a.com/file.zip
来源：http://www.52xcode.cn/Article/details/gt3owdfwppj.html

[R59] 发 POST JSON
来源：http://www.ydjk.org.cn/Article/details/gt3bgkrfzcf.html

curl -X POST -H 'Content-Type: application/json' -d '{"a":1}' https://api.example.com
来源：http://www.ydjk.org.cn/Article/details/gt3omeyzsfi.html

[R60] 只看 HTTP 状态码
来源：http://www.ydjk.org.cn/Article/details/gt3wxeawqfb.html

curl -s -o /dev/null -w "%{http_code}\n" https://a.com
来源：http://www.52xcode.cn/Article/details/gt3znaalhvm.html

[R61] 磁盘占用
来源：http://www.52xcode.cn/Article/details/gt3olwrqftw.html

df -h;  du -sh *
来源：http://www.ydjk.org.cn/Article/details/gt3gqhoprgu.html

[R62] 找最占空间的文件
来源：http://www.ydjk.org.cn/Article/details/gt3phhgxfnp.html

du -ah . | sort -rh | head -10
来源：http://www.ydjk.org.cn/Article/details/gt3twsoejwz.html

[R63] 内存与进程
来源：http://www.52xcode.cn/Article/details/gt3vcyfhjey.html

free -h;  ps aux | grep nginx
来源：http://www.ydjk.org.cn/Article/details/gt3qpwaazgo.html

[R64] 结束进程
来源：http://www.ydjk.org.cn/Article/details/gt3wbmqfrpa.html

kill -9 $(pgrep -f app.py)
来源：http://www.ydjk.org.cn/Article/details/gt3wrihkfah.html

[R65] 查看端口占用
来源：http://www.ydjk.org.cn/Article/details/gt3rjjwnsnv.html

ss -tlnp | grep 8080;  lsof -i:8080
来源：http://www.ydjk.org.cn/Article/details/gt3stmpwcqu.html

[R66] 定时任务
来源：http://www.52xcode.cn/Article/details/gt3zpboqbuj.html

crontab -e;  crontab -l
来源：http://www.ydjk.org.cn/Article/details/gt3zslcqego.html

[R67] 生成随机十六进制串
来源：http://www.ydjk.org.cn/Article/details/gt3ecuzkfoc.html

openssl rand -hex 16
来源：http://www.ydjk.org.cn/Article/details/gt3nfujlnhg.html

[R68] 计算文件校验值
来源：http://www.ydjk.org.cn/Article/details/gt3jmuwgxtj.html

sha256sum a.txt;  md5sum a.txt
来源：http://www.ydjk.org.cn/Article/details/gt3vorstqxe.html

[R69] 生成随机密码
来源：http://www.ydjk.org.cn/Article/details/gt3yvexkbsy.html

head -c 16 /dev/urandom | base64
来源：http://www.ydjk.org.cn/Article/details/gt3fiwoqqyr.html

[R70] 时间戳与互转
来源：http://www.52xcode.cn/Article/details/gt3qisbepnv.html

date +%s;  date -d @1700000000
来源：http://www.ydjk.org.cn/Article/details/gt3qwjalnsk.html

[R71] 日期格式化
来源：http://www.ydjk.org.cn/Article/details/gt3ekhsgvkx.html

date +"%Y-%m-%d %H:%M:%S"
来源：http://www.ydjk.org.cn/Article/details/gt3tprfwels.html

[R72] 等待端口就绪
来源：http://www.ydjk.org.cn/Article/details/gt3flrnoxsx.html

until nc -z localhost 3306; do sleep 1; done
来源：http://www.ydjk.org.cn/Article/details/gt3fmwhtolg.html

[R73] 分割大日志
来源：http://www.52xcode.cn/Article/details/gt3qexbtrkz.html

split -l 1000 big.log part_
来源：http://www.ydjk.org.cn/Article/details/gt3wxwboxzy.html

[R74] 批量重命名
来源：http://www.52xcode.cn/Article/details/gt3nhxmxfor.html

for f in *.jpeg; do mv "$f" "${f%.jpeg}.jpg"; done
来源：http://www.52xcode.cn/Article/details/gt3oglpsgbe.html

[R75] 导出环境变量
来源：http://www.52xcode.cn/Article/details/gt3yjalzlcc.html

export PATH="$HOME/bin:$PATH"
来源：http://www.52xcode.cn/Article/details/gt3dpolvbqy.html

[R76] 使用临时文件
来源：http://www.52xcode.cn/Article/details/gt3githcfpl.html

tmp=$(mktemp); trap 'rm -f "$tmp"' EXIT
来源：http://www.52xcode.cn/Article/details/gt3hkqenryj.html

[R77] 读取用户输入
来源：http://www.ydjk.org.cn/Article/details/gt3atrcfnol.html

read -rp "请输入: " ans
来源：http://www.ydjk.org.cn/Article/details/gt3uuvfskea.html

[R78] 交互式菜单
来源：http://www.ydjk.org.cn/Article/details/gt3ndhjwria.html

select opt in a b c; do echo "$opt"; break; done
来源：http://www.52xcode.cn/Article/details/gt3bqunepsr.html

[R79] 解析命令行选项
来源：http://www.52xcode.cn/Article/details/gt3fcumztpz.html

while getopts "v:f:" o; do case $o in v) V=$OPTARG ;; f) F=$OPTARG ;; esac; done
来源：http://www.ydjk.org.cn/Article/details/gt3wbpoairq.html

[R80] 查看脚本执行耗时
来源：http://www.52xcode.cn/Article/details/gt3kbglvnny.html

time ./run.sh
来源：http://www.ydjk.org.cn/Article/details/gt3caivfpth.html

================================================================================
来源：http://www.ydjk.org.cn/Article/details/gt3vhmrxqvj.html

S. C / C++ 专题
来源：http://www.52xcode.cn/Article/details/gt3fjnjwfia.html

================================================================================
来源：http://www.ydjk.org.cn/Article/details/gt3wpmupkdx.html

[S01] C：Hello World
来源：http://www.ydjk.org.cn/Article/details/gt3eyxvehtd.html

#include <stdio.h>
来源：http://www.52xcode.cn/Article/details/gt3ejysyrop.html

int main(void) { printf("Hello\n"); return 0; }
来源：http://www.52xcode.cn/Article/details/gt3rfgmpqzv.html

[S02] C：变量与格式化输出
来源：http://www.52xcode.cn/Article/details/gt3swncdshh.html

int a = 10; printf("%d\n", a);
来源：http://www.52xcode.cn/Article/details/gt3wbnkprvb.html

[S03] C：读入整数
来源：http://www.52xcode.cn/Article/details/gt3aulxsndi.html

int x; scanf("%d", &x);
来源：http://www.52xcode.cn/Article/details/gt3coyhsxpo.html

[S04] C：字符串复制
来源：http://www.52xcode.cn/Article/details/gt3pjneireo.html

char dst[32]; strcpy(dst, "hi");
来源：http://www.ydjk.org.cn/Article/details/gt3xcuuuoel.html

[S05] C：字符串长度
来源：http://www.ydjk.org.cn/Article/details/gt3nnvkpzfa.html

strlen(s)
来源：http://www.52xcode.cn/Article/details/gt3hlzuznpx.html

[S06] C：字符串比较
来源：http://www.ydjk.org.cn/Article/details/gt3yhblrxac.html

strcmp(a, b) == 0
来源：http://www.52xcode.cn/Article/details/gt3bbhqnzlj.html

[S07] C：数组遍历求和
来源：http://www.52xcode.cn/Article/details/gt3qsdlisie.html

for (int i = 0; i < n; i++) sum += a[i];
来源：http://www.52xcode.cn/Article/details/gt3pawqefdf.html

[S08] C：动态内存分配与释放
来源：http://www.ydjk.org.cn/Article/details/gt3vyccjrfj.html

int *p = malloc(sizeof(int) * n); ... free(p);
来源：http://www.ydjk.org.cn/Article/details/gt3mdwykqcg.html

[S09] C：结构体定义与初始化
来源：http://www.52xcode.cn/Article/details/gt3urfkrtsw.html

struct Point { int x, y; };  struct Point p = {1, 2};
来源：http://www.52xcode.cn/Article/details/gt3ngndubam.html

[S10] C：指针与解引用
来源：http://www.ydjk.org.cn/Article/details/gt3yaabuhwh.html

int *p = &a;  *p = 5;
来源：http://www.ydjk.org.cn/Article/details/gt3rfjqgzsv.html

[S11] C：逐行读文件
来源：http://www.52xcode.cn/Article/details/gt3tzwivzgm.html

FILE *f = fopen("a.txt", "r");
来源：http://www.52xcode.cn/Article/details/gt3trpwmydw.html

while (fgets(buf, sizeof buf, f)) { }
来源：http://www.52xcode.cn/Article/details/gt3ixlfkcft.html

fclose(f);
来源：http://www.ydjk.org.cn/Article/details/gt3fbdqavyu.html

[S12] C：写文件
来源：http://www.52xcode.cn/Article/details/gt3fddhbief.html

FILE *f = fopen("a.txt", "w");  fprintf(f, "hi\n");  fclose(f);
来源：http://www.ydjk.org.cn/Article/details/gt3limgulai.html

[S13] C：宏定义
来源：http://www.ydjk.org.cn/Article/details/gt3woazxscu.html

#define MAX(a, b) ((a) > (b) ? (a) : (b))
来源：http://www.52xcode.cn/Article/details/gt3upapumzk.html

[S14] C：枚举
来源：http://www.ydjk.org.cn/Article/details/gt3uhdwmohl.html

enum Color { RED, GREEN, BLUE };
来源：http://www.ydjk.org.cn/Article/details/gt3clckavft.html

[S15] C：类型转换
来源：http://www.52xcode.cn/Article/details/gt3ajebydec.html

(double) a / b
来源：http://www.52xcode.cn/Article/details/gt3ziqpjapi.html

[S16] C：位操作置位
来源：http://www.ydjk.org.cn/Article/details/gt3fwqkzznd.html

x |= (1 << 3);
来源：http://www.52xcode.cn/Article/details/gt3bovrdphq.html

[S17] C：安全拼接字符串
来源：http://www.52xcode.cn/Article/details/gt3kljiptxk.html

snprintf(buf, sizeof buf, "%s%s", a, b);
来源：http://www.52xcode.cn/Article/details/gt3yaycbcbw.html

[S18] C：命令行参数
来源：http://www.ydjk.org.cn/Article/details/gt3gfijdlsd.html

int main(int argc, char **argv)
来源：http://www.52xcode.cn/Article/details/gt3nyntgxfh.html

[S19] C：快速排序
来源：http://www.ydjk.org.cn/Article/details/gt3ziptqbgu.html

qsort(a, n, sizeof(int), cmp);
来源：http://www.52xcode.cn/Article/details/gt3hzqjjjgp.html

[S20] C：二分查找
来源：http://www.52xcode.cn/Article/details/gt3khgmyvws.html

bsearch(&key, a, n, sizeof(int), cmp);
来源：http://www.52xcode.cn/Article/details/gt3dmxlzlzk.html

[S21] C：字符类别判断
来源：http://www.ydjk.org.cn/Article/details/gt3nngpgjhe.html

isdigit(c);  isalpha(c);  isspace(c);
来源：http://www.ydjk.org.cn/Article/details/gt3ibhpmatm.html

[S22] C：字符串转数字
来源：http://www.ydjk.org.cn/Article/details/gt3apefdjpe.html

atoi("42");  strtod("3.14", NULL);
来源：http://www.52xcode.cn/Article/details/gt3ytxeqjdq.html

[S23] C：随机数
来源：http://www.ydjk.org.cn/Article/details/gt3rbmwpbfc.html

srand(time(NULL));  int r = rand() % 100;
来源：http://www.ydjk.org.cn/Article/details/gt3vvofedia.html

[S24] C：获取本地时间
来源：http://www.52xcode.cn/Article/details/gt3yjmrpcei.html

time_t t = time(NULL);  struct tm *tm = localtime(&t);
来源：http://www.52xcode.cn/Article/details/gt3xrngazpq.html

[S25] C：内存拷贝
来源：http://www.52xcode.cn/Article/details/gt3auzjuxyu.html

memcpy(dst, src, n);
来源：http://www.52xcode.cn/Article/details/gt3zkxrgfok.html

[S26] C：内存清零
来源：http://www.ydjk.org.cn/Article/details/gt3chdbetpx.html

memset(a, 0, sizeof a);
来源：http://www.52xcode.cn/Article/details/gt3xaiumaml.html

[S27] C：定义常量
来源：http://www.ydjk.org.cn/Article/details/gt3nbocwtgv.html

const double PI = 3.14159;
来源：http://www.52xcode.cn/Article/details/gt3clmpsfvl.html

[S28] C：静态变量
来源：http://www.52xcode.cn/Article/details/gt3hwpooiei.html

static int counter = 0;
来源：http://www.ydjk.org.cn/Article/details/gt3hhywwihi.html

[S29] C：变参函数
来源：http://www.ydjk.org.cn/Article/details/gt3kkkbfchy.html

va_list ap; va_start(ap, fmt); vprintf(fmt, ap); va_end(ap);
来源：http://www.52xcode.cn/Article/details/gt3odclelhp.html

[S30] C：头文件保护
来源：http://www.ydjk.org.cn/Article/details/gt3fftivdqo.html

#ifndef X_H
来源：http://www.52xcode.cn/Article/details/gt3mpmlcrpd.html

#define X_H
来源：http://www.52xcode.cn/Article/details/gt3frynyvei.html

#endif
来源：http://www.52xcode.cn/Article/details/gt3lzhtdkks.html

[S31] C++：Hello World
来源：http://www.52xcode.cn/Article/details/gt3dlzhgira.html

#include <iostream>
来源：http://www.ydjk.org.cn/Article/details/gt3liyswulm.html

int main() { std::cout << "Hello\n"; }
来源：http://www.52xcode.cn/Article/details/gt3ratjzhkc.html

[S32] C++：字符串
来源：http://www.ydjk.org.cn/Article/details/gt3kuypwffp.html

std::string s = "hi";  s += "!";
来源：http://www.ydjk.org.cn/Article/details/gt3sdgtbhxf.html

[S33] C++：vector 增删
来源：http://www.52xcode.cn/Article/details/gt3anzamewp.html

std::vector<int> v{1, 2, 3};  v.push_back(4);
来源：http://www.ydjk.org.cn/Article/details/gt3loiwlpsh.html

[S34] C++：遍历 vector
来源：http://www.52xcode.cn/Article/details/gt3gtocgyww.html

for (auto &x : v) { std::cout << x; }
来源：http://www.52xcode.cn/Article/details/gt3hcenriab.html

[S35] C++：map
来源：http://www.ydjk.org.cn/Article/details/gt3xpfrefki.html

std::map<std::string, int> m;  m["a"] = 1;
来源：http://www.52xcode.cn/Article/details/gt3xhccppch.html

[S36] C++：unordered_map
来源：http://www.52xcode.cn/Article/details/gt3ftpisjbz.html

std::unordered_map<std::string, int> m;  m["a"] = 1;
来源：http://www.52xcode.cn/Article/details/gt3fiphujby.html

[S37] C++：set
来源：http://www.52xcode.cn/Article/details/gt3epyuwqke.html

std::set<int> s{1, 2, 3};  s.insert(4);
来源：http://www.52xcode.cn/Article/details/gt3xbgmzvvx.html

[S38] C++：排序
来源：http://www.ydjk.org.cn/Article/details/gt3mhbiyrdk.html

std::sort(v.begin(), v.end());
来源：http://www.52xcode.cn/Article/details/gt3chydasil.html

[S39] C++：自定义比较器排序
来源：http://www.ydjk.org.cn/Article/details/gt3bpfxacfx.html

std::sort(v.begin(), v.end(), [](int a, int b) { return a > b; });
来源：http://www.52xcode.cn/Article/details/gt3vdcpbafc.html

[S40] C++：查找元素
来源：http://www.ydjk.org.cn/Article/details/gt3cfsgjzqz.html

auto it = std::find(v.begin(), v.end(), 3);
来源：http://www.ydjk.org.cn/Article/details/gt3fjrlfijw.html

[S41] C++：类与构造函数
来源：http://www.ydjk.org.cn/Article/details/gt3haygnkgr.html

class A { public: A(int v) : x_(v) {} int get() const { return x_; } private: int x_; };
来源：http://www.ydjk.org.cn/Article/details/gt3dskfuikr.html

[S42] C++：继承与虚函数
来源：http://www.ydjk.org.cn/Article/details/gt3flstqdwa.html

class B : public Base { public: void f() override {} };
来源：http://www.ydjk.org.cn/Article/details/gt3wyozrlop.html

[S43] C++：智能指针
来源：http://www.ydjk.org.cn/Article/details/gt3ilesstkx.html

auto p = std::make_unique<int>(5);
来源：http://www.ydjk.org.cn/Article/details/gt3qdttibwv.html

[S44] C++：引用传参
来源：http://www.ydjk.org.cn/Article/details/gt3umqfcgsb.html

void inc(int &x) { ++x; }
来源：http://www.ydjk.org.cn/Article/details/gt3guiyymkg.html

[S45] C++：lambda
来源：http://www.52xcode.cn/Article/details/gt3eailoajj.html

auto add = [](int a, int b) { return a + b; };
来源：http://www.ydjk.org.cn/Article/details/gt3njvkhkdx.html

[S46] C++：函数模板
来源：http://www.52xcode.cn/Article/details/gt3rrzufgbo.html

template <typename T> T maxv(T a, T b) { return a > b ? a : b; }
来源：http://www.ydjk.org.cn/Article/details/gt3pwieuzbi.html

[S47] C++：结构化绑定遍历
来源：http://www.52xcode.cn/Article/details/gt3uppqocfp.html

for (const auto &[k, v] : m) { std::cout << k << v; }
来源：http://www.52xcode.cn/Article/details/gt3aiovbrrz.html

[S48] C++：逐行读文件
来源：http://www.52xcode.cn/Article/details/gt3qruxzkit.html

std::ifstream in("a.txt");  std::string line;
来源：http://www.ydjk.org.cn/Article/details/gt3jzkzeuqw.html

while (std::getline(in, line)) { }
来源：http://www.52xcode.cn/Article/details/gt3wzcznpyv.html

[S49] C++：写文件
来源：http://www.52xcode.cn/Article/details/gt3snpqxfjy.html

std::ofstream out("a.txt");  out << "hi\n";
来源：http://www.52xcode.cn/Article/details/gt3yvwowfqo.html

[S50] C++：格式化数字
来源：http://www.ydjk.org.cn/Article/details/gt3qenkapau.html

std::ostringstream os;  os << std::fixed << std::setprecision(2) << 3.14159;
来源：http://www.ydjk.org.cn/Article/details/gt3imypnejj.html

[S51] C++：显式类型转换
来源：http://www.52xcode.cn/Article/details/gt3cmpcppcf.html

static_cast<double>(a) / b
来源：http://www.52xcode.cn/Article/details/gt3vvdaxutq.html

[S52] C++：const 与 noexcept
来源：http://www.52xcode.cn/Article/details/gt3rahvqozf.html

int size() const noexcept { return n_; }
来源：http://www.52xcode.cn/Article/details/gt3lbniwhzk.html

[S53] C++：移动语义
来源：http://www.52xcode.cn/Article/details/gt3ybdycqrw.html

std::vector<int> w = std::move(v);
来源：http://www.ydjk.org.cn/Article/details/gt3cfjjjwkf.html

[S54] C++：异常处理
来源：http://www.ydjk.org.cn/Article/details/gt3fyrcqshm.html

try { throw std::runtime_error("x"); } catch (const std::exception &e) { }
来源：http://www.ydjk.org.cn/Article/details/gt3kgeynopb.html

[S55] C++：结构化绑定
来源：http://www.ydjk.org.cn/Article/details/gt3uzzzmygy.html

auto [a, b] = std::make_pair(1, 2);
来源：http://www.ydjk.org.cn/Article/details/gt3qcgkraqp.html

[S56] C++：optional
来源：http://www.ydjk.org.cn/Article/details/gt3hzdqlixa.html

std::optional<int> o = 5;  if (o) { int v = *o; }
来源：http://www.52xcode.cn/Article/details/gt3fmuagkpw.html

[S57] C++：编译期常量
来源：http://www.ydjk.org.cn/Article/details/gt3juwiheqy.html

constexpr int N = 10;
来源：http://www.52xcode.cn/Article/details/gt3vittrgfx.html

[S58] C++：命名空间
来源：http://www.52xcode.cn/Article/details/gt3qsqiwqrv.html

namespace ns { int f() { return 1; } }
来源：http://www.ydjk.org.cn/Article/details/gt3lqnymhio.html

[S59] C++：静态断言
来源：http://www.52xcode.cn/Article/details/gt3rkgeikmr.html

static_assert(sizeof(int) == 4, "int 必须 4 字节");
来源：http://www.ydjk.org.cn/Article/details/gt3uyzftnzi.html

[S60] C++：遍历并删除元素
来源：http://www.ydjk.org.cn/Article/details/gt3oyuhcfcq.html

v.erase(std::remove_if(v.begin(), v.end(), [](int x) { return x < 0; }), v.end());
来源：http://www.ydjk.org.cn/Article/details/gt3bitlppsv.html

================================================================================
来源：http://www.52xcode.cn/Article/details/gt3nifpgywl.html

T. 其他语言补充（Kotlin / Swift / Lua / Perl / Scala）
来源：http://www.52xcode.cn/Article/details/gt3urzhnbuc.html

================================================================================
来源：http://www.ydjk.org.cn/Article/details/gt3uzgnafxz.html

[T01] Kotlin：Hello World
来源：http://www.52xcode.cn/Article/details/gt3gztgpatu.html

println("Hello")
来源：http://www.52xcode.cn/Article/details/gt3xubbifyk.html

[T02] Kotlin：变量
来源：http://www.ydjk.org.cn/Article/details/gt3wimjzqmg.html

val a = 1;  var b = 2        // val 只读，var 可变
来源：http://www.ydjk.org.cn/Article/details/gt3kzaspzau.html

[T03] Kotlin：字符串模板
来源：http://www.ydjk.org.cn/Article/details/gt3dtkmfnpt.html

"值: $b"
来源：http://www.52xcode.cn/Article/details/gt3rxbcwkxk.html

[T04] Kotlin：空安全
来源：http://www.ydjk.org.cn/Article/details/gt3zenvfemv.html

val n: String? = null;  n?.length
来源：http://www.ydjk.org.cn/Article/details/gt3ecejdutr.html

[T05] Kotlin：when 表达式
来源：http://www.52xcode.cn/Article/details/gt3konicxyw.html

val s = when (x) { 1 -> "一" else -> "其他" }   // 多分支时每个分支单独一行
来源：http://www.52xcode.cn/Article/details/gt3erwkawbu.html

[T06] Kotlin：集合映射
来源：http://www.ydjk.org.cn/Article/details/gt3ocajucuw.html

listOf(1, 2, 3).map { it * 2 }
来源：http://www.52xcode.cn/Article/details/gt3mnhsprhw.html

[T07] Kotlin：集合过滤
来源：http://www.ydjk.org.cn/Article/details/gt3ivptspey.html

listOf(1, 2, 3).filter { it > 1 }
来源：http://www.52xcode.cn/Article/details/gt3ajvibykk.html

[T08] Kotlin：数据类
来源：http://www.ydjk.org.cn/Article/details/gt3trhpnxvz.html

data class User(val name: String, val age: Int)
来源：http://www.52xcode.cn/Article/details/gt3xdbwzhct.html

[T09] Kotlin：扩展函数
来源：http://www.52xcode.cn/Article/details/gt3xjgmnmia.html

fun String.exclaim() = this + "!"
来源：http://www.52xcode.cn/Article/details/gt3xbnypcsm.html

[T10] Kotlin：默认参数
来源：http://www.ydjk.org.cn/Article/details/gt3rwhzpntc.html

fun greet(name: String = "World") = "Hi $name"
来源：http://www.52xcode.cn/Article/details/gt3vxjrdvwg.html

[T11] Kotlin：协程
来源：http://www.52xcode.cn/Article/details/gt3qfylbdar.html

GlobalScope.launch { delay(1000); println("done") }
来源：http://www.52xcode.cn/Article/details/gt3rttimdgb.html

[T12] Kotlin：解构声明
来源：http://www.52xcode.cn/Article/details/gt3pjcpthdw.html

val (a, b) = Pair(1, 2)
来源：http://www.52xcode.cn/Article/details/gt3wrbkuchg.html

[T13] Kotlin：只读 Map
来源：http://www.ydjk.org.cn/Article/details/gt3ywwhuydn.html

val m = mapOf("a" to 1)
来源：http://www.52xcode.cn/Article/details/gt3zhuuwwfy.html

[T14] Kotlin：循环
来源：http://www.52xcode.cn/Article/details/gt3gtxurior.html

for (i in 1..10) println(i)
来源：http://www.ydjk.org.cn/Article/details/gt3lxdczhvw.html

[T15] Kotlin：接口
来源：http://www.52xcode.cn/Article/details/gt3heobmxmi.html

interface Shape { fun area(): Double }
来源：http://www.52xcode.cn/Article/details/gt3ylfrlmnx.html

[T16] Swift：Hello World
来源：http://www.52xcode.cn/Article/details/gt3nqvdyyts.html

print("Hello")
来源：http://www.52xcode.cn/Article/details/gt3ludsvkic.html

[T17] Swift：变量与常量
来源：http://www.ydjk.org.cn/Article/details/gt3azfwhzgq.html

var a = 1;  let b = 2
来源：http://www.52xcode.cn/Article/details/gt3yfcmroob.html

[T18] Swift：字符串插值
来源：http://www.52xcode.cn/Article/details/gt3fmbsgcgx.html

"值: \(b)"
来源：http://www.ydjk.org.cn/Article/details/gt3pkpjqqdh.html

[T19] Swift：可选绑定
来源：http://www.52xcode.cn/Article/details/gt3pjuzfwci.html

if let n = opt { print(n) }
来源：http://www.ydjk.org.cn/Article/details/gt3nvmcmbvu.html

[T20] Swift：数组操作
来源：http://www.52xcode.cn/Article/details/gt3tuoitgrj.html

var a = [1, 2, 3];  a.append(4)
来源：http://www.ydjk.org.cn/Article/details/gt3awherhue.html

[T21] Swift：遍历
来源：http://www.52xcode.cn/Article/details/gt3qqqcqtva.html

for x in a { print(x) }
来源：http://www.ydjk.org.cn/Article/details/gt3poeqewzg.html

[T22] Swift：字典
来源：http://www.ydjk.org.cn/Article/details/gt3hrptqeun.html

var d = ["a": 1];  d["b"] = 2
来源：http://www.52xcode.cn/Article/details/gt3raeaeifr.html

[T23] Swift：函数
来源：http://www.ydjk.org.cn/Article/details/gt3infgkpek.html

func add(_ a: Int, _ b: Int) -> Int { a + b }
来源：http://www.52xcode.cn/Article/details/gt3poqbtorj.html

[T24] Swift：闭包
来源：http://www.52xcode.cn/Article/details/gt3vraaqddn.html

let f = { (x: Int) -> Int in x * 2 }
来源：http://www.ydjk.org.cn/Article/details/gt3tqbitrmi.html

[T25] Swift：结构体
来源：http://www.52xcode.cn/Article/details/gt3mymwcnxt.html

struct P { var x: Int }
来源：http://www.52xcode.cn/Article/details/gt3vqjjcrio.html

[T26] Swift：类与重写
来源：http://www.ydjk.org.cn/Article/details/gt3xsxtrcmg.html

class A: Base { override func f() {} }
来源：http://www.ydjk.org.cn/Article/details/gt3tkhqkstj.html

[T27] Swift：错误处理
来源：http://www.ydjk.org.cn/Article/details/gt3oddqyxqd.html

do { try f() } catch { print(error) }
来源：http://www.52xcode.cn/Article/details/gt3frcvievx.html

[T28] Swift：枚举
来源：http://www.52xcode.cn/Article/details/gt3zddyxtxb.html

enum Color { case red, green }
来源：http://www.52xcode.cn/Article/details/gt3jeivyffd.html

[T29] Swift：guard 提前返回
来源：http://www.ydjk.org.cn/Article/details/gt3dlkzrykp.html

guard let x = opt else { return }
来源：http://www.52xcode.cn/Article/details/gt3pkrhqmua.html

[T30] Swift：协议
来源：http://www.52xcode.cn/Article/details/gt3ujgcgagd.html

protocol Shape { func area() -> Double }
来源：http://www.52xcode.cn/Article/details/gt3ttsruids.html

[T31] Lua：Hello World
来源：http://www.52xcode.cn/Article/details/gt3xwvggusj.html

print("Hello")
来源：http://www.ydjk.org.cn/Article/details/gt3wkakhxeo.html

[T32] Lua：局部变量
来源：http://www.52xcode.cn/Article/details/gt3kagsrppi.html

local a = 1
来源：http://www.52xcode.cn/Article/details/gt3mwcwqgdy.html

[T33] Lua：表（数组）
来源：http://www.52xcode.cn/Article/details/gt3vxwlkgio.html

local t = {1, 2, 3};  t[4] = 4
来源：http://www.ydjk.org.cn/Article/details/gt3gafajvgr.html

[T34] Lua：遍历表
来源：http://www.52xcode.cn/Article/details/gt3kofesseb.html

for i, v in ipairs(t) do print(i, v) end
来源：http://www.52xcode.cn/Article/details/gt3luxpnxmv.html

[T35] Lua：字典表
来源：http://www.ydjk.org.cn/Article/details/gt3pbewedvf.html

local d = { a = 1 };  d.b = 2
来源：http://www.ydjk.org.cn/Article/details/gt3wuacdozj.html

[T36] Lua：函数
来源：http://www.ydjk.org.cn/Article/details/gt3niylxjbt.html

function add(a, b) return a + b end
来源：http://www.52xcode.cn/Article/details/gt3ecjnagcq.html

[T37] Lua：字符串拼接
来源：http://www.52xcode.cn/Article/details/gt3yielzlfq.html

"a" .. "b"
来源：http://www.52xcode.cn/Article/details/gt3tuoarmmh.html

[T38] Lua：条件
来源：http://www.ydjk.org.cn/Article/details/gt3sgnyakqi.html

if x > 0 then print("正") end
来源：http://www.52xcode.cn/Article/details/gt3czgwiaot.html

[T39] Lua：模式匹配
来源：http://www.52xcode.cn/Article/details/gt3kqprtywt.html

string.find(s, "%d+")
来源：http://www.52xcode.cn/Article/details/gt3sxspisvb.html

[T40] Lua：元表
来源：http://www.52xcode.cn/Article/details/gt3dveizboe.html

setmetatable({}, { __index = base })
来源：http://www.52xcode.cn/Article/details/gt3qtqajojf.html

[T41] Perl：Hello World
来源：http://www.ydjk.org.cn/Article/details/gt3jvgxctxe.html

print "Hello\n";
来源：http://www.52xcode.cn/Article/details/gt3rhlvrwbe.html

[T42] Perl：变量类型
来源：http://www.52xcode.cn/Article/details/gt3rapaaisv.html

my $a = 1;  my @arr = (1, 2, 3);  my %h = (a => 1);
来源：http://www.ydjk.org.cn/Article/details/gt3gmvmpana.html

[T43] Perl：字符串插值
来源：http://www.52xcode.cn/Article/details/gt3sdlabdzu.html

"值: $a"
来源：http://www.ydjk.org.cn/Article/details/gt3zpcgzpiz.html

[T44] Perl：条件
来源：http://www.52xcode.cn/Article/details/gt3komyesll.html

if ($a > 0) { print "正"; }
来源：http://www.ydjk.org.cn/Article/details/gt3evcooxyd.html

[T45] Perl：数组遍历
来源：http://www.ydjk.org.cn/Article/details/gt3yklghnly.html

for my $x (@arr) { print $x; }
来源：http://www.ydjk.org.cn/Article/details/gt3gizmvenq.html

[T46] Perl：哈希操作
来源：http://www.52xcode.cn/Article/details/gt3ndooxbfs.html

$h{b} = 2;  for my $k (keys %h) { print "$k=$h{$k}"; }
来源：http://www.ydjk.org.cn/Article/details/gt3oodzodel.html

[T47] Perl：正则捕获
来源：http://www.ydjk.org.cn/Article/details/gt3lmlsbril.html

if ($s =~ /(\d+)/) { print $1; }
来源：http://www.ydjk.org.cn/Article/details/gt3zymltwqo.html

[T48] Perl：正则替换
来源：http://www.ydjk.org.cn/Article/details/gt3lvjglrna.html

$s =~ s/old/new/g;
来源：http://www.ydjk.org.cn/Article/details/gt3eawzammt.html

[T49] Perl：函数
来源：http://www.52xcode.cn/Article/details/gt3qbdgiefz.html

sub add { my ($a, $b) = @_; return $a + $b; }
来源：http://www.ydjk.org.cn/Article/details/gt3zqcqtrns.html

[T50] Perl：逐行读文件
来源：http://www.ydjk.org.cn/Article/details/gt3hybhkxkp.html

open my $fh, "<", "a.txt" or die $!;
来源：http://www.ydjk.org.cn/Article/details/gt3xubacbcf.html

while (my $line = <$fh>) { print $line; }
来源：http://www.52xcode.cn/Article/details/gt3sfognuhm.html

[T51] Scala：Hello World
来源：http://www.ydjk.org.cn/Article/details/gt3qiebbahr.html

println("Hello")
来源：http://www.ydjk.org.cn/Article/details/gt3owfzucae.html

[T52] Scala：变量
来源：http://www.52xcode.cn/Article/details/gt3gvudqtzr.html

val a = 1;  var b = 2
来源：http://www.ydjk.org.cn/Article/details/gt3gzwsdeib.html

[T53] Scala：字符串插值
来源：http://www.52xcode.cn/Article/details/gt3pmexfeiv.html

s"值: $b"
来源：http://www.ydjk.org.cn/Article/details/gt3hsuznemd.html

[T54] Scala：集合映射
来源：http://www.52xcode.cn/Article/details/gt3sqxrizqd.html

List(1, 2, 3).map(_ * 2)
来源：http://www.52xcode.cn/Article/details/gt3eourzkpo.html

[T55] Scala：集合过滤
来源：http://www.52xcode.cn/Article/details/gt3crcqlqch.html

List(1, 2, 3).filter(_ > 1)
来源：http://www.ydjk.org.cn/Article/details/gt3iibiprft.html

[T56] Scala：样例类
来源：http://www.52xcode.cn/Article/details/gt3tosrtqbf.html


<!-- 参考信息 -->