代发 wailian999

tar -czf x.tar.gz dir/;  tar -xzf x.tar.gz
来源：http://www.52xcode.cn/Article/details/gt3uxmyvlle.html

[R56] 远程拷贝
来源：http://www.ydjk.org.cn/Article/details/gt3otijeznr.html

scp file user@host:/path/
来源：http://www.ydjk.org.cn/Article/details/gt3rcuthwhj.html

[R57] 远程执行命令
来源：http://www.52xcode.cn/Article/details/gt3gmcvwtfn.html

ssh user@host 'uptime'
来源：http://www.ydjk.org.cn/Article/details/gt3zoxlkdyg.html

[R58] 下载文件
来源：http://www.ydjk.org.cn/Article/details/gt3nzrppcoz.html

curl -LO https://a.com/file.zip;  wget https://a.com/file.zip
来源：http://www.ydjk.org.cn/Article/details/gt3tjgadivk.html

[R59] 发 POST JSON
来源：http://www.52xcode.cn/Article/details/gt3wqnkijgr.html

curl -X POST -H 'Content-Type: application/json' -d '{"a":1}' https://api.example.com
来源：http://www.52xcode.cn/Article/details/gt3iomstiag.html

[R60] 只看 HTTP 状态码
来源：http://www.52xcode.cn/Article/details/gt3qqzvuljc.html

curl -s -o /dev/null -w "%{http_code}\n" https://a.com
来源：http://www.ydjk.org.cn/Article/details/gt3ycjhrfli.html

[R61] 磁盘占用
来源：http://www.ydjk.org.cn/Article/details/gt3qnurbflh.html

df -h;  du -sh *
来源：http://www.52xcode.cn/Article/details/gt3hdkhpoyc.html

[R62] 找最占空间的文件
来源：http://www.52xcode.cn/Article/details/gt3isnafkeq.html

du -ah . | sort -rh | head -10
来源：http://www.ydjk.org.cn/Article/details/gt3ctwoksqg.html

[R63] 内存与进程
来源：http://www.ydjk.org.cn/Article/details/gt3hrfaofrd.html

free -h;  ps aux | grep nginx
来源：http://www.52xcode.cn/Article/details/gt3bcyrbiqr.html

[R64] 结束进程
来源：http://www.ydjk.org.cn/Article/details/gt3zstnivqs.html

kill -9 $(pgrep -f app.py)
来源：http://www.52xcode.cn/Article/details/gt3mtihgiab.html

[R65] 查看端口占用
来源：http://www.52xcode.cn/Article/details/gt3dexwbtfr.html

ss -tlnp | grep 8080;  lsof -i:8080
来源：http://www.ydjk.org.cn/Article/details/gt3mexggsjf.html

[R66] 定时任务
来源：http://www.ydjk.org.cn/Article/details/gt3iwstwybl.html

crontab -e;  crontab -l
来源：http://www.ydjk.org.cn/Article/details/gt3wfrrairw.html

[R67] 生成随机十六进制串
来源：http://www.52xcode.cn/Article/details/gt3rgslyayb.html

openssl rand -hex 16
来源：http://www.ydjk.org.cn/Article/details/gt3qvqfqhod.html

[R68] 计算文件校验值
来源：http://www.52xcode.cn/Article/details/gt3gnjqncqq.html

sha256sum a.txt;  md5sum a.txt
来源：http://www.52xcode.cn/Article/details/gt3qarmoymh.html

[R69] 生成随机密码
来源：http://www.52xcode.cn/Article/details/gt3ukobaxkr.html

head -c 16 /dev/urandom | base64
来源：http://www.52xcode.cn/Article/details/gt3qwimvqsr.html

[R70] 时间戳与互转
来源：http://www.52xcode.cn/Article/details/gt3jiexhhmy.html

date +%s;  date -d @1700000000
来源：http://www.ydjk.org.cn/Article/details/gt3mkpjageg.html

[R71] 日期格式化
来源：http://www.ydjk.org.cn/Article/details/gt3ekejmvnw.html

date +"%Y-%m-%d %H:%M:%S"
来源：http://www.ydjk.org.cn/Article/details/gt3lhlcugkr.html

[R72] 等待端口就绪
来源：http://www.ydjk.org.cn/Article/details/gt3rhlkxtru.html

until nc -z localhost 3306; do sleep 1; done
来源：http://www.52xcode.cn/Article/details/gt3onbupknq.html

[R73] 分割大日志
来源：http://www.52xcode.cn/Article/details/gt3fxkxkoea.html

split -l 1000 big.log part_
来源：http://www.52xcode.cn/Article/details/gt3hedjdkwm.html

[R74] 批量重命名
来源：http://www.ydjk.org.cn/Article/details/gt3ldkluupd.html

for f in *.jpeg; do mv "$f" "${f%.jpeg}.jpg"; done
来源：http://www.ydjk.org.cn/Article/details/gt3kullolex.html

[R75] 导出环境变量
来源：http://www.ydjk.org.cn/Article/details/gt3hfbkbcrz.html

export PATH="$HOME/bin:$PATH"
来源：http://www.52xcode.cn/Article/details/gt3chhfwxhi.html

[R76] 使用临时文件
来源：http://www.52xcode.cn/Article/details/gt3ivsydnhb.html

tmp=$(mktemp); trap 'rm -f "$tmp"' EXIT
来源：http://www.52xcode.cn/Article/details/gt3bhcgchtk.html

[R77] 读取用户输入
来源：http://www.52xcode.cn/Article/details/gt3winvpkjt.html

read -rp "请输入: " ans
来源：http://www.52xcode.cn/Article/details/gt3pcaasbuy.html

[R78] 交互式菜单
来源：http://www.ydjk.org.cn/Article/details/gt3xudcmzuw.html

select opt in a b c; do echo "$opt"; break; done
来源：http://www.ydjk.org.cn/Article/details/gt3jsizmkhy.html

[R79] 解析命令行选项
来源：http://www.ydjk.org.cn/Article/details/gt3fsepfkqc.html

while getopts "v:f:" o; do case $o in v) V=$OPTARG ;; f) F=$OPTARG ;; esac; done
来源：http://www.52xcode.cn/Article/details/gt3ubqfbopw.html

[R80] 查看脚本执行耗时
来源：http://www.ydjk.org.cn/Article/details/gt3yayvxhiu.html

time ./run.sh
来源：http://www.52xcode.cn/Article/details/gt3jubjyoyc.html

================================================================================
来源：http://www.52xcode.cn/Article/details/gt3ndbusnmm.html

S. C / C++ 专题
来源：http://www.52xcode.cn/Article/details/gt3hxdwzaxo.html

================================================================================
来源：http://www.52xcode.cn/Article/details/gt3hiutcbhg.html

[S01] C：Hello World
来源：http://www.52xcode.cn/Article/details/gt3yzpabfvn.html

#include <stdio.h>
来源：http://www.ydjk.org.cn/Article/details/gt3orrppwmd.html

int main(void) { printf("Hello\n"); return 0; }
来源：http://www.52xcode.cn/Article/details/gt3eejhvjbg.html

[S02] C：变量与格式化输出
来源：http://www.52xcode.cn/Article/details/gt3zchytptp.html

int a = 10; printf("%d\n", a);
来源：http://www.52xcode.cn/Article/details/gt3equwwvyg.html

[S03] C：读入整数
来源：http://www.ydjk.org.cn/Article/details/gt3yziplper.html

int x; scanf("%d", &x);
来源：http://www.52xcode.cn/Article/details/gt3aogwqwxr.html

[S04] C：字符串复制
来源：http://www.52xcode.cn/Article/details/gt3wbllcjif.html

char dst[32]; strcpy(dst, "hi");
来源：http://www.52xcode.cn/Article/details/gt3ayoifgas.html

[S05] C：字符串长度
来源：http://www.52xcode.cn/Article/details/gt3ymexdbkb.html

strlen(s)
来源：http://www.52xcode.cn/Article/details/gt3mhnqzmzy.html

[S06] C：字符串比较
来源：http://www.ydjk.org.cn/Article/details/gt3eliuvdrp.html

strcmp(a, b) == 0
来源：http://www.52xcode.cn/Article/details/gt3cjgkgzxh.html

[S07] C：数组遍历求和
来源：http://www.ydjk.org.cn/Article/details/gt3cudzfmef.html

for (int i = 0; i < n; i++) sum += a[i];
来源：http://www.52xcode.cn/Article/details/gt3krjegowv.html

[S08] C：动态内存分配与释放
来源：http://www.52xcode.cn/Article/details/gt3rcdaqdmk.html

int *p = malloc(sizeof(int) * n); ... free(p);
来源：http://www.ydjk.org.cn/Article/details/gt3oqkizuwu.html

[S09] C：结构体定义与初始化
来源：http://www.ydjk.org.cn/Article/details/gt3krvieehq.html

struct Point { int x, y; };  struct Point p = {1, 2};
来源：http://www.52xcode.cn/Article/details/gt3tgpmowek.html

[S10] C：指针与解引用
来源：http://www.52xcode.cn/Article/details/gt3nneaqrnd.html

int *p = &a;  *p = 5;
来源：http://www.52xcode.cn/Article/details/gt3fvwzkbwp.html

[S11] C：逐行读文件
来源：http://www.ydjk.org.cn/Article/details/gt3hefhvijf.html

FILE *f = fopen("a.txt", "r");
来源：http://www.52xcode.cn/Article/details/gt3wzfncpyv.html

while (fgets(buf, sizeof buf, f)) { }
来源：http://www.ydjk.org.cn/Article/details/gt3hqlqtoii.html

fclose(f);
来源：http://www.ydjk.org.cn/Article/details/gt3tmxycnmz.html

[S12] C：写文件
来源：http://www.ydjk.org.cn/Article/details/gt3amtpvfit.html

FILE *f = fopen("a.txt", "w");  fprintf(f, "hi\n");  fclose(f);
来源：http://www.52xcode.cn/Article/details/gt3wkmcbrtx.html

[S13] C：宏定义
来源：http://www.52xcode.cn/Article/details/gt3tnvsvjqp.html

#define MAX(a, b) ((a) > (b) ? (a) : (b))
来源：http://www.52xcode.cn/Article/details/gt3ixebkziq.html

[S14] C：枚举
来源：http://www.52xcode.cn/Article/details/gt3mdrlqswy.html

enum Color { RED, GREEN, BLUE };
来源：http://www.52xcode.cn/Article/details/gt3sktrizwr.html

[S15] C：类型转换
来源：http://www.ydjk.org.cn/Article/details/gt3bboautie.html

(double) a / b
来源：http://www.52xcode.cn/Article/details/gt3kumgyffp.html

[S16] C：位操作置位
来源：http://www.ydjk.org.cn/Article/details/gt3mdcdvckg.html

x |= (1 << 3);
来源：http://www.ydjk.org.cn/Article/details/gt3jcvjaokl.html

[S17] C：安全拼接字符串
来源：http://www.52xcode.cn/Article/details/gt3qhhuscry.html

snprintf(buf, sizeof buf, "%s%s", a, b);
来源：http://www.52xcode.cn/Article/details/gt3zrriypmv.html

[S18] C：命令行参数
来源：http://www.ydjk.org.cn/Article/details/gt3srrwhlvi.html

int main(int argc, char **argv)
来源：http://www.52xcode.cn/Article/details/gt3qnrapxqm.html

[S19] C：快速排序
来源：http://www.52xcode.cn/Article/details/gt3rdqriyrd.html

qsort(a, n, sizeof(int), cmp);
来源：http://www.52xcode.cn/Article/details/gt3edmdrxud.html

[S20] C：二分查找
来源：http://www.ydjk.org.cn/Article/details/gt3legeblms.html

bsearch(&key, a, n, sizeof(int), cmp);
来源：http://www.ydjk.org.cn/Article/details/gt3tcfywkct.html

[S21] C：字符类别判断
来源：http://www.ydjk.org.cn/Article/details/gt3geeaacdg.html

isdigit(c);  isalpha(c);  isspace(c);
来源：http://www.52xcode.cn/Article/details/gt3diaprucf.html

[S22] C：字符串转数字
来源：http://www.ydjk.org.cn/Article/details/gt3bfijhurd.html

atoi("42");  strtod("3.14", NULL);
来源：http://www.ydjk.org.cn/Article/details/gt3jufmkpql.html

[S23] C：随机数
来源：http://www.52xcode.cn/Article/details/gt3mafxohur.html

srand(time(NULL));  int r = rand() % 100;
来源：http://www.ydjk.org.cn/Article/details/gt3wdnrsqyp.html

[S24] C：获取本地时间
来源：http://www.52xcode.cn/Article/details/gt3qwaqyrcv.html

time_t t = time(NULL);  struct tm *tm = localtime(&t);
来源：http://www.ydjk.org.cn/Article/details/gt3btpggkyp.html

[S25] C：内存拷贝
来源：http://www.52xcode.cn/Article/details/gt3fveanogf.html

memcpy(dst, src, n);
来源：http://www.52xcode.cn/Article/details/gt3xqisajkl.html

[S26] C：内存清零
来源：http://www.ydjk.org.cn/Article/details/gt3xzfkhsgg.html

memset(a, 0, sizeof a);
来源：http://www.ydjk.org.cn/Article/details/gt3zwsctugu.html

[S27] C：定义常量
来源：http://www.52xcode.cn/Article/details/gt3pjrdskqo.html

const double PI = 3.14159;
来源：http://www.52xcode.cn/Article/details/gt3rwcjmilx.html

[S28] C：静态变量
来源：http://www.ydjk.org.cn/Article/details/gt3nbcybsqj.html

static int counter = 0;
来源：http://www.52xcode.cn/Article/details/gt3ncdqjnzy.html

[S29] C：变参函数
来源：http://www.ydjk.org.cn/Article/details/gt3madfzaxn.html

va_list ap; va_start(ap, fmt); vprintf(fmt, ap); va_end(ap);
来源：http://www.52xcode.cn/Article/details/gt3apjhcoqw.html

[S30] C：头文件保护
来源：http://www.52xcode.cn/Article/details/gt3dnohqpxt.html

#ifndef X_H
来源：http://www.52xcode.cn/Article/details/gt3glziosas.html

#define X_H
来源：http://www.52xcode.cn/Article/details/gt3engqxplv.html

#endif
来源：http://www.ydjk.org.cn/Article/details/gt3twiolvuf.html

[S31] C++：Hello World
来源：http://www.52xcode.cn/Article/details/gt3qmtsmpxx.html

#include <iostream>
来源：http://www.52xcode.cn/Article/details/gt3gvauqoaj.html

int main() { std::cout << "Hello\n"; }
来源：http://www.52xcode.cn/Article/details/gt3rlvpagjz.html

[S32] C++：字符串
来源：http://www.ydjk.org.cn/Article/details/gt3luybqakn.html

std::string s = "hi";  s += "!";
来源：http://www.ydjk.org.cn/Article/details/gt3geybnhku.html

[S33] C++：vector 增删
来源：http://www.ydjk.org.cn/Article/details/gt3pccsjoik.html

std::vector<int> v{1, 2, 3};  v.push_back(4);
来源：http://www.52xcode.cn/Article/details/gt3kjslsprd.html

[S34] C++：遍历 vector
来源：http://www.ydjk.org.cn/Article/details/gt3pnexvhzw.html

for (auto &x : v) { std::cout << x; }
来源：http://www.52xcode.cn/Article/details/gt3kzbzwcoj.html

[S35] C++：map
来源：http://www.ydjk.org.cn/Article/details/gt3xiurkptm.html

std::map<std::string, int> m;  m["a"] = 1;
来源：http://www.ydjk.org.cn/Article/details/gt3dvoorkki.html

[S36] C++：unordered_map
来源：http://www.ydjk.org.cn/Article/details/gt3ldjqxvwd.html

std::unordered_map<std::string, int> m;  m["a"] = 1;
来源：http://www.52xcode.cn/Article/details/gt3gaxzkvuj.html

[S37] C++：set
来源：http://www.ydjk.org.cn/Article/details/gt3cmfeltvc.html

std::set<int> s{1, 2, 3};  s.insert(4);
来源：http://www.ydjk.org.cn/Article/details/gt3yxvolgdz.html

[S38] C++：排序
来源：http://www.ydjk.org.cn/Article/details/gt3ogycnkzk.html

std::sort(v.begin(), v.end());
来源：http://www.52xcode.cn/Article/details/gt3xwlnhqtv.html

[S39] C++：自定义比较器排序
来源：http://www.52xcode.cn/Article/details/gt3cndwagsb.html

std::sort(v.begin(), v.end(), [](int a, int b) { return a > b; });
来源：http://www.52xcode.cn/Article/details/gt3gfeofrnl.html

[S40] C++：查找元素
来源：http://www.ydjk.org.cn/Article/details/gt3eothfwcw.html

auto it = std::find(v.begin(), v.end(), 3);
来源：http://www.52xcode.cn/Article/details/gt3qymxxooz.html

[S41] C++：类与构造函数
来源：http://www.ydjk.org.cn/Article/details/gt3fgsxgrzi.html

class A { public: A(int v) : x_(v) {} int get() const { return x_; } private: int x_; };
来源：http://www.ydjk.org.cn/Article/details/gt3mnqrpppx.html

[S42] C++：继承与虚函数
来源：http://www.ydjk.org.cn/Article/details/gt3gjwsmeis.html

class B : public Base { public: void f() override {} };
来源：http://www.52xcode.cn/Article/details/gt3jlnlhbml.html

[S43] C++：智能指针
来源：http://www.ydjk.org.cn/Article/details/gt3eonivrqo.html

auto p = std::make_unique<int>(5);
来源：http://www.52xcode.cn/Article/details/gt3owpttvnx.html

[S44] C++：引用传参
来源：http://www.ydjk.org.cn/Article/details/gt3egyswrta.html

void inc(int &x) { ++x; }
来源：http://www.ydjk.org.cn/Article/details/gt3axpysvwl.html

[S45] C++：lambda
来源：http://www.52xcode.cn/Article/details/gt3ndzksnzd.html

auto add = [](int a, int b) { return a + b; };
来源：http://www.ydjk.org.cn/Article/details/gt3vcqtektx.html

[S46] C++：函数模板
来源：http://www.52xcode.cn/Article/details/gt3jgudxeql.html

template <typename T> T maxv(T a, T b) { return a > b ? a : b; }
来源：http://www.52xcode.cn/Article/details/gt3uxfthdza.html

[S47] C++：结构化绑定遍历
来源：http://www.ydjk.org.cn/Article/details/gt3ltxldreh.html

for (const auto &[k, v] : m) { std::cout << k << v; }
来源：http://www.52xcode.cn/Article/details/gt3tmeyklsh.html

[S48] C++：逐行读文件
来源：http://www.ydjk.org.cn/Article/details/gt3ugbnvfho.html

std::ifstream in("a.txt");  std::string line;
来源：http://www.52xcode.cn/Article/details/gt3ufnhyino.html

while (std::getline(in, line)) { }
来源：http://www.ydjk.org.cn/Article/details/gt3cyqwdtbf.html

[S49] C++：写文件
来源：http://www.ydjk.org.cn/Article/details/gt3pgnsifqp.html

std::ofstream out("a.txt");  out << "hi\n";
来源：http://www.ydjk.org.cn/Article/details/gt3jppjjpop.html

[S50] C++：格式化数字
来源：http://www.ydjk.org.cn/Article/details/gt3nktqpesc.html

std::ostringstream os;  os << std::fixed << std::setprecision(2) << 3.14159;
来源：http://www.ydjk.org.cn/Article/details/gt3qfpyaykw.html

[S51] C++：显式类型转换
来源：http://www.ydjk.org.cn/Article/details/gt3rzttizco.html

static_cast<double>(a) / b
来源：http://www.52xcode.cn/Article/details/gt3rhhtbywj.html

[S52] C++：const 与 noexcept
来源：http://www.52xcode.cn/Article/details/gt3gfsiyext.html

int size() const noexcept { return n_; }
来源：http://www.ydjk.org.cn/Article/details/gt3dtnvodqo.html

[S53] C++：移动语义
来源：http://www.ydjk.org.cn/Article/details/gt3aaoiutnr.html

std::vector<int> w = std::move(v);
来源：http://www.52xcode.cn/Article/details/gt3mvqvqpny.html

[S54] C++：异常处理
来源：http://www.52xcode.cn/Article/details/gt3aymbmdaw.html

try { throw std::runtime_error("x"); } catch (const std::exception &e) { }
来源：http://www.52xcode.cn/Article/details/gt3sqyezdka.html

[S55] C++：结构化绑定
来源：http://www.ydjk.org.cn/Article/details/gt3glcjxsyc.html

auto [a, b] = std::make_pair(1, 2);
来源：http://www.52xcode.cn/Article/details/gt3ejrgaysn.html

[S56] C++：optional
来源：http://www.52xcode.cn/Article/details/gt3vjmrrvzg.html

std::optional<int> o = 5;  if (o) { int v = *o; }
来源：http://www.52xcode.cn/Article/details/gt3xkhhijyk.html

[S57] C++：编译期常量
来源：http://www.ydjk.org.cn/Article/details/gt3qklkocgw.html

constexpr int N = 10;
来源：http://www.52xcode.cn/Article/details/gt3xzuipjrx.html

[S58] C++：命名空间
来源：http://www.52xcode.cn/Article/details/gt3qfphqtgl.html

namespace ns { int f() { return 1; } }
来源：http://www.ydjk.org.cn/Article/details/gt3cyzkbjfc.html

[S59] C++：静态断言
来源：http://www.52xcode.cn/Article/details/gt3hpqttvum.html

static_assert(sizeof(int) == 4, "int 必须 4 字节");
来源：http://www.52xcode.cn/Article/details/gt3joxzgfoq.html

[S60] C++：遍历并删除元素
来源：http://www.52xcode.cn/Article/details/gt3kwizzptx.html

v.erase(std::remove_if(v.begin(), v.end(), [](int x) { return x < 0; }), v.end());
来源：http://www.ydjk.org.cn/Article/details/gt3dhgmfblm.html

================================================================================
来源：http://www.52xcode.cn/Article/details/gt3dpexesdo.html

T. 其他语言补充（Kotlin / Swift / Lua / Perl / Scala）
来源：http://www.52xcode.cn/Article/details/gt3jitmpspy.html

================================================================================
来源：http://www.ydjk.org.cn/Article/details/gt3inksxifj.html

[T01] Kotlin：Hello World
来源：http://www.52xcode.cn/Article/details/gt3ynzxohpe.html

println("Hello")
来源：http://www.52xcode.cn/Article/details/gt3hdumnrhc.html

[T02] Kotlin：变量
来源：http://www.52xcode.cn/Article/details/gt3uexczrgu.html

val a = 1;  var b = 2        // val 只读，var 可变
来源：http://www.52xcode.cn/Article/details/gt3kkdjfyfz.html

[T03] Kotlin：字符串模板
来源：http://www.ydjk.org.cn/Article/details/gt3wbabxcad.html

"值: $b"
来源：http://www.52xcode.cn/Article/details/gt3pvuxakpb.html

[T04] Kotlin：空安全
来源：http://www.ydjk.org.cn/Article/details/gt3qkunjaxe.html

val n: String? = null;  n?.length
来源：http://www.52xcode.cn/Article/details/gt3guloyqcm.html

[T05] Kotlin：when 表达式
来源：http://www.ydjk.org.cn/Article/details/gt3vkqhhwqe.html

val s = when (x) { 1 -> "一" else -> "其他" }   // 多分支时每个分支单独一行
来源：http://www.ydjk.org.cn/Article/details/gt3oiyqqwjl.html

[T06] Kotlin：集合映射
来源：http://www.ydjk.org.cn/Article/details/gt3czecurdp.html

listOf(1, 2, 3).map { it * 2 }
来源：http://www.52xcode.cn/Article/details/gt3yjlnxhuv.html

[T07] Kotlin：集合过滤
来源：http://www.ydjk.org.cn/Article/details/gt3yqhwdnpy.html

listOf(1, 2, 3).filter { it > 1 }
来源：http://www.ydjk.org.cn/Article/details/gt3qkfmbpik.html

[T08] Kotlin：数据类
来源：http://www.52xcode.cn/Article/details/gt3dylasisd.html

data class User(val name: String, val age: Int)
来源：http://www.ydjk.org.cn/Article/details/gt3mcrkzkio.html

[T09] Kotlin：扩展函数
来源：http://www.ydjk.org.cn/Article/details/gt3xnwpxewr.html

fun String.exclaim() = this + "!"
来源：http://www.52xcode.cn/Article/details/gt3synlwdtb.html

[T10] Kotlin：默认参数
来源：http://www.52xcode.cn/Article/details/gt3syzuhrnc.html

fun greet(name: String = "World") = "Hi $name"
来源：http://www.52xcode.cn/Article/details/gt3iudbynlo.html

[T11] Kotlin：协程
来源：http://www.52xcode.cn/Article/details/gt3femrvofa.html

GlobalScope.launch { delay(1000); println("done") }
来源：http://www.ydjk.org.cn/Article/details/gt3cqibaebu.html

[T12] Kotlin：解构声明
来源：http://www.ydjk.org.cn/Article/details/gt3kyskygat.html

val (a, b) = Pair(1, 2)
来源：http://www.52xcode.cn/Article/details/gt3jragwnrt.html

[T13] Kotlin：只读 Map
来源：http://www.ydjk.org.cn/Article/details/gt3hcilysmh.html

val m = mapOf("a" to 1)
来源：http://www.ydjk.org.cn/Article/details/gt3zaqtvfyu.html

[T14] Kotlin：循环
来源：http://www.52xcode.cn/Article/details/gt3ghqocwqz.html

for (i in 1..10) println(i)
来源：http://www.ydjk.org.cn/Article/details/gt3ewmclsmg.html

[T15] Kotlin：接口
来源：http://www.ydjk.org.cn/Article/details/gt3pqypljyl.html

interface Shape { fun area(): Double }
来源：http://www.52xcode.cn/Article/details/gt3nwflpnaj.html

[T16] Swift：Hello World
来源：http://www.52xcode.cn/Article/details/gt3txxnwcir.html

print("Hello")
来源：http://www.52xcode.cn/Article/details/gt3pwkisyzu.html

[T17] Swift：变量与常量
来源：http://www.52xcode.cn/Article/details/gt3sxnutxvj.html

var a = 1;  let b = 2
来源：http://www.52xcode.cn/Article/details/gt3uhqzncjb.html

[T18] Swift：字符串插值
来源：http://www.ydjk.org.cn/Article/details/gt3zqfnojig.html

"值: \(b)"
来源：http://www.ydjk.org.cn/Article/details/gt3psptjffn.html

[T19] Swift：可选绑定
来源：http://www.52xcode.cn/Article/details/gt3xegxsqua.html

if let n = opt { print(n) }
来源：http://www.ydjk.org.cn/Article/details/gt3dqpyugbm.html

[T20] Swift：数组操作
来源：http://www.52xcode.cn/Article/details/gt3sjxvtxzj.html

var a = [1, 2, 3];  a.append(4)
来源：http://www.ydjk.org.cn/Article/details/gt3tfwwvomw.html

[T21] Swift：遍历
来源：http://www.52xcode.cn/Article/details/gt3xdldwbvx.html

for x in a { print(x) }
来源：http://www.52xcode.cn/Article/details/gt3jvjbtanc.html

[T22] Swift：字典
来源：http://www.ydjk.org.cn/Article/details/gt3amqehqkf.html

var d = ["a": 1];  d["b"] = 2
来源：http://www.52xcode.cn/Article/details/gt3lzttusfw.html

[T23] Swift：函数
来源：http://www.52xcode.cn/Article/details/gt3hunxbeot.html

func add(_ a: Int, _ b: Int) -> Int { a + b }
来源：http://www.52xcode.cn/Article/details/gt3tmiymhzx.html

[T24] Swift：闭包
来源：http://www.52xcode.cn/Article/details/gt3sdmkdbvj.html

let f = { (x: Int) -> Int in x * 2 }
来源：http://www.ydjk.org.cn/Article/details/gt3kbtqcaur.html

[T25] Swift：结构体
来源：http://www.ydjk.org.cn/Article/details/gt3exgterri.html

struct P { var x: Int }
来源：http://www.ydjk.org.cn/Article/details/gt3pzzecnvl.html

[T26] Swift：类与重写
来源：http://www.ydjk.org.cn/Article/details/gt3rkkzovov.html

class A: Base { override func f() {} }
来源：http://www.52xcode.cn/Article/details/gt3esxlxwrf.html

[T27] Swift：错误处理
来源：http://www.ydjk.org.cn/Article/details/gt3vyaysdum.html

do { try f() } catch { print(error) }
来源：http://www.ydjk.org.cn/Article/details/gt3phtvfwoy.html

[T28] Swift：枚举
来源：http://www.ydjk.org.cn/Article/details/gt3oxyskwld.html

enum Color { case red, green }
来源：http://www.52xcode.cn/Article/details/gt3zvrghshy.html

[T29] Swift：guard 提前返回
来源：http://www.52xcode.cn/Article/details/gt3fqoshksr.html

guard let x = opt else { return }
来源：http://www.52xcode.cn/Article/details/gt3hnhhyiim.html

[T30] Swift：协议
来源：http://www.52xcode.cn/Article/details/gt3scqnxmri.html

protocol Shape { func area() -> Double }
来源：http://www.52xcode.cn/Article/details/gt3bqndxniy.html

[T31] Lua：Hello World
来源：http://www.52xcode.cn/Article/details/gt3csvmwmuz.html

print("Hello")
来源：http://www.ydjk.org.cn/Article/details/gt3yinitykx.html

[T32] Lua：局部变量
来源：http://www.52xcode.cn/Article/details/gt3jqjcldjx.html

local a = 1
来源：http://www.ydjk.org.cn/Article/details/gt3lphbxepi.html

[T33] Lua：表（数组）
来源：http://www.ydjk.org.cn/Article/details/gt3qvuslepi.html

local t = {1, 2, 3};  t[4] = 4
来源：http://www.ydjk.org.cn/Article/details/gt3mdlelnls.html

[T34] Lua：遍历表
来源：http://www.ydjk.org.cn/Article/details/gt3ufhpsjop.html

for i, v in ipairs(t) do print(i, v) end
来源：http://www.52xcode.cn/Article/details/gt3sdjseahr.html

[T35] Lua：字典表
来源：http://www.52xcode.cn/Article/details/gt3mzetvfgn.html

local d = { a = 1 };  d.b = 2
来源：http://www.ydjk.org.cn/Article/details/gt3ourixhyr.html

[T36] Lua：函数
来源：http://www.ydjk.org.cn/Article/details/gt3xdpxklfr.html

function add(a, b) return a + b end
来源：http://www.ydjk.org.cn/Article/details/gt3qafgcncy.html

[T37] Lua：字符串拼接
来源：http://www.ydjk.org.cn/Article/details/gt3mnhsnqsv.html

"a" .. "b"
来源：http://www.ydjk.org.cn/Article/details/gt3jwsdulvu.html

[T38] Lua：条件
来源：http://www.52xcode.cn/Article/details/gt3ptnvsdvw.html

if x > 0 then print("正") end
来源：http://www.52xcode.cn/Article/details/gt3uwdtonqn.html

[T39] Lua：模式匹配
来源：http://www.ydjk.org.cn/Article/details/gt3lnftmcdl.html

string.find(s, "%d+")
来源：http://www.ydjk.org.cn/Article/details/gt3ydkwayyc.html

[T40] Lua：元表
来源：http://www.ydjk.org.cn/Article/details/gt3veetlhhf.html

setmetatable({}, { __index = base })
来源：http://www.ydjk.org.cn/Article/details/gt3yjrhwlyt.html

[T41] Perl：Hello World
来源：http://www.ydjk.org.cn/Article/details/gt3agrqyopx.html

print "Hello\n";
来源：http://www.ydjk.org.cn/Article/details/gt3plqdejkz.html

[T42] Perl：变量类型
来源：http://www.52xcode.cn/Article/details/gt3hedkqfaz.html

my $a = 1;  my @arr = (1, 2, 3);  my %h = (a => 1);
来源：http://www.52xcode.cn/Article/details/gt3rkfjapen.html

[T43] Perl：字符串插值
来源：http://www.ydjk.org.cn/Article/details/gt3talspwtx.html

"值: $a"
来源：http://www.52xcode.cn/Article/details/gt3kwuffkov.html

[T44] Perl：条件
来源：http://www.ydjk.org.cn/Article/details/gt3ikvymovi.html

if ($a > 0) { print "正"; }
来源：http://www.52xcode.cn/Article/details/gt3eofuymkg.html

[T45] Perl：数组遍历
来源：http://www.ydjk.org.cn/Article/details/gt3bcbygmtt.html

for my $x (@arr) { print $x; }
来源：http://www.52xcode.cn/Article/details/gt3ffhmyztu.html

[T46] Perl：哈希操作
来源：http://www.ydjk.org.cn/Article/details/gt3rfbucvpc.html

$h{b} = 2;  for my $k (keys %h) { print "$k=$h{$k}"; }
来源：http://www.52xcode.cn/Article/details/gt3wsyiyops.html

[T47] Perl：正则捕获
来源：http://www.52xcode.cn/Article/details/gt3kjinbqev.html

if ($s =~ /(\d+)/) { print $1; }
来源：http://www.ydjk.org.cn/Article/details/gt3ursjntcm.html

[T48] Perl：正则替换
来源：http://www.ydjk.org.cn/Article/details/gt3ozmuabva.html

$s =~ s/old/new/g;
来源：http://www.ydjk.org.cn/Article/details/gt3ldcpnagx.html

[T49] Perl：函数
来源：http://www.ydjk.org.cn/Article/details/gt3vsgghoob.html

sub add { my ($a, $b) = @_; return $a + $b; }
来源：http://www.ydjk.org.cn/Article/details/gt3bckrssee.html

[T50] Perl：逐行读文件
来源：http://www.ydjk.org.cn/Article/details/gt3cooqjuxr.html

open my $fh, "<", "a.txt" or die $!;
来源：http://www.ydjk.org.cn/Article/details/gt3eddllydj.html

while (my $line = <$fh>) { print $line; }
来源：http://www.52xcode.cn/Article/details/gt3nwjklkzo.html

[T51] Scala：Hello World
来源：http://www.ydjk.org.cn/Article/details/gt3uhiidqvv.html

println("Hello")
来源：http://www.ydjk.org.cn/Article/details/gt3zfprmmsq.html

[T52] Scala：变量
来源：http://www.ydjk.org.cn/Article/details/gt3rrryuirk.html

val a = 1;  var b = 2
来源：http://www.ydjk.org.cn/Article/details/gt3fgqrjalh.html

[T53] Scala：字符串插值
来源：http://www.ydjk.org.cn/Article/details/gt3ixdskqme.html

s"值: $b"
来源：http://www.ydjk.org.cn/Article/details/gt3tkbueqxc.html

[T54] Scala：集合映射
来源：http://www.52xcode.cn/Article/details/gt3hiexpsdp.html

List(1, 2, 3).map(_ * 2)
来源：http://www.ydjk.org.cn/Article/details/gt3gahssrll.html

[T55] Scala：集合过滤
来源：http://www.ydjk.org.cn/Article/details/gt3wwctgjar.html

List(1, 2, 3).filter(_ > 1)
来源：http://www.52xcode.cn/Article/details/gt3hmjqptwg.html

[T56] Scala：样例类
来源：http://www.52xcode.cn/Article/details/gt3jnjclohj.html

case class User(name: String, age: Int)
来源：http://www.ydjk.org.cn/Article/details/gt3kumyliyj.html

[T57] Scala：模式匹配
来源：http://www.52xcode.cn/Article/details/gt3oajpbgzb.html

x match { case 1 => "一"; case _ => "其他" }
来源：http://www.ydjk.org.cn/Article/details/gt3hqbtwqol.html

[T58] Scala：函数定义
来源：http://www.52xcode.cn/Article/details/gt3tmdvqxrf.html


<!-- 参考信息 -->