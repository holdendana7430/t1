代发 wailian999

free -h;  ps aux | grep nginx
来源：http://www.ydjk.org.cn/Article/details/gt3mnyfsqma.html

[R64] 结束进程
来源：http://www.52xcode.cn/Article/details/gt3mqvpoxcy.html

kill -9 $(pgrep -f app.py)
来源：http://www.52xcode.cn/Article/details/gt3srkmdmtu.html

[R65] 查看端口占用
来源：http://www.ydjk.org.cn/Article/details/gt3zbqzjiop.html

ss -tlnp | grep 8080;  lsof -i:8080
来源：http://www.ydjk.org.cn/Article/details/gt3vmfhmami.html

[R66] 定时任务
来源：http://www.52xcode.cn/Article/details/gt3ronldfou.html

crontab -e;  crontab -l
来源：http://www.ydjk.org.cn/Article/details/gt3qitdgwco.html

[R67] 生成随机十六进制串
来源：http://www.ydjk.org.cn/Article/details/gt3fxoftlrb.html

openssl rand -hex 16
来源：http://www.52xcode.cn/Article/details/gt3iapsxtqc.html

[R68] 计算文件校验值
来源：http://www.52xcode.cn/Article/details/gt3qaolangd.html

sha256sum a.txt;  md5sum a.txt
来源：http://www.52xcode.cn/Article/details/gt3scqidjxc.html

[R69] 生成随机密码
来源：http://www.ydjk.org.cn/Article/details/gt3udvncdom.html

head -c 16 /dev/urandom | base64
来源：http://www.52xcode.cn/Article/details/gt3bilyshok.html

[R70] 时间戳与互转
来源：http://www.52xcode.cn/Article/details/gt3igsaaljk.html

date +%s;  date -d @1700000000
来源：http://www.ydjk.org.cn/Article/details/gt3ubndxwnp.html

[R71] 日期格式化
来源：http://www.ydjk.org.cn/Article/details/gt3ofbfahqn.html

date +"%Y-%m-%d %H:%M:%S"
来源：http://www.52xcode.cn/Article/details/gt3ouhkgtfa.html

[R72] 等待端口就绪
来源：http://www.52xcode.cn/Article/details/gt3lrubqznf.html

until nc -z localhost 3306; do sleep 1; done
来源：http://www.ydjk.org.cn/Article/details/gt3yylvhzba.html

[R73] 分割大日志
来源：http://www.ydjk.org.cn/Article/details/gt3ygsddtny.html

split -l 1000 big.log part_
来源：http://www.ydjk.org.cn/Article/details/gt3ptkwbifd.html

[R74] 批量重命名
来源：http://www.ydjk.org.cn/Article/details/gt3cbffkrry.html

for f in *.jpeg; do mv "$f" "${f%.jpeg}.jpg"; done
来源：http://www.ydjk.org.cn/Article/details/gt3qrsjjxjm.html

[R75] 导出环境变量
来源：http://www.ydjk.org.cn/Article/details/gt3hgbevcil.html

export PATH="$HOME/bin:$PATH"
来源：http://www.ydjk.org.cn/Article/details/gt3utnpjzjt.html

[R76] 使用临时文件
来源：http://www.ydjk.org.cn/Article/details/gt3snjbirkk.html

tmp=$(mktemp); trap 'rm -f "$tmp"' EXIT
来源：http://www.ydjk.org.cn/Article/details/gt3kzzmfgyy.html

[R77] 读取用户输入
来源：http://www.ydjk.org.cn/Article/details/gt3bvmvcfsv.html

read -rp "请输入: " ans
来源：http://www.52xcode.cn/Article/details/gt3qpsbfveu.html

[R78] 交互式菜单
来源：http://www.ydjk.org.cn/Article/details/gt3besjhtku.html

select opt in a b c; do echo "$opt"; break; done
来源：http://www.ydjk.org.cn/Article/details/gt3nvalogwv.html

[R79] 解析命令行选项
来源：http://www.52xcode.cn/Article/details/gt3aacycviy.html

while getopts "v:f:" o; do case $o in v) V=$OPTARG ;; f) F=$OPTARG ;; esac; done
来源：http://www.ydjk.org.cn/Article/details/gt3qasmdzpo.html

[R80] 查看脚本执行耗时
来源：http://www.ydjk.org.cn/Article/details/gt3gyetavdw.html

time ./run.sh
来源：http://www.ydjk.org.cn/Article/details/gt3frwvrtox.html

================================================================================
来源：http://www.ydjk.org.cn/Article/details/gt3zlncxdop.html

S. C / C++ 专题
来源：http://www.52xcode.cn/Article/details/gt3obziojwi.html

================================================================================
来源：http://www.ydjk.org.cn/Article/details/gt3yiedfvqs.html

[S01] C：Hello World
来源：http://www.52xcode.cn/Article/details/gt3jnmniswf.html

#include <stdio.h>
来源：http://www.ydjk.org.cn/Article/details/gt3raoofofv.html

int main(void) { printf("Hello\n"); return 0; }
来源：http://www.52xcode.cn/Article/details/gt3dczxggeg.html

[S02] C：变量与格式化输出
来源：http://www.52xcode.cn/Article/details/gt3kudbrtmh.html

int a = 10; printf("%d\n", a);
来源：http://www.52xcode.cn/Article/details/gt3echhuhey.html

[S03] C：读入整数
来源：http://www.52xcode.cn/Article/details/gt3siyrgjus.html

int x; scanf("%d", &x);
来源：http://www.ydjk.org.cn/Article/details/gt3nctyfggd.html

[S04] C：字符串复制
来源：http://www.ydjk.org.cn/Article/details/gt3gzpfeslb.html

char dst[32]; strcpy(dst, "hi");
来源：http://www.ydjk.org.cn/Article/details/gt3ysmjsdrn.html

[S05] C：字符串长度
来源：http://www.52xcode.cn/Article/details/gt3hlzmaavz.html

strlen(s)
来源：http://www.ydjk.org.cn/Article/details/gt3opuimwfp.html

[S06] C：字符串比较
来源：http://www.ydjk.org.cn/Article/details/gt3kxndfdec.html

strcmp(a, b) == 0
来源：http://www.ydjk.org.cn/Article/details/gt3ucbkajtf.html

[S07] C：数组遍历求和
来源：http://www.52xcode.cn/Article/details/gt3rzxbckod.html

for (int i = 0; i < n; i++) sum += a[i];
来源：http://www.52xcode.cn/Article/details/gt3vfzfjtzd.html

[S08] C：动态内存分配与释放
来源：http://www.52xcode.cn/Article/details/gt3xydvavls.html

int *p = malloc(sizeof(int) * n); ... free(p);
来源：http://www.ydjk.org.cn/Article/details/gt3wxiagktw.html

[S09] C：结构体定义与初始化
来源：http://www.52xcode.cn/Article/details/gt3aigcuvuv.html

struct Point { int x, y; };  struct Point p = {1, 2};
来源：http://www.52xcode.cn/Article/details/gt3ipdahmay.html

[S10] C：指针与解引用
来源：http://www.ydjk.org.cn/Article/details/gt3qvfvbtgh.html

int *p = &a;  *p = 5;
来源：http://www.52xcode.cn/Article/details/gt3qxvomkxk.html

[S11] C：逐行读文件
来源：http://www.52xcode.cn/Article/details/gt3xovgtjfg.html

FILE *f = fopen("a.txt", "r");
来源：http://www.ydjk.org.cn/Article/details/gt3smpuakiq.html

while (fgets(buf, sizeof buf, f)) { }
来源：http://www.ydjk.org.cn/Article/details/gt3fcsjnext.html

fclose(f);
来源：http://www.52xcode.cn/Article/details/gt3jxgozynz.html

[S12] C：写文件
来源：http://www.ydjk.org.cn/Article/details/gt3odjysaop.html

FILE *f = fopen("a.txt", "w");  fprintf(f, "hi\n");  fclose(f);
来源：http://www.ydjk.org.cn/Article/details/gt3pyeseygc.html

[S13] C：宏定义
来源：http://www.ydjk.org.cn/Article/details/gt3ukhqarsq.html

#define MAX(a, b) ((a) > (b) ? (a) : (b))
来源：http://www.52xcode.cn/Article/details/gt3tsrkuuvq.html

[S14] C：枚举
来源：http://www.52xcode.cn/Article/details/gt3iofaxfex.html

enum Color { RED, GREEN, BLUE };
来源：http://www.52xcode.cn/Article/details/gt3ksggzdxv.html

[S15] C：类型转换
来源：http://www.ydjk.org.cn/Article/details/gt3vxhiwchc.html

(double) a / b
来源：http://www.ydjk.org.cn/Article/details/gt3hqbrmkjz.html

[S16] C：位操作置位
来源：http://www.ydjk.org.cn/Article/details/gt3qrjxgstu.html

x |= (1 << 3);
来源：http://www.ydjk.org.cn/Article/details/gt3vjvwekll.html

[S17] C：安全拼接字符串
来源：http://www.52xcode.cn/Article/details/gt3mziwqorn.html

snprintf(buf, sizeof buf, "%s%s", a, b);
来源：http://www.ydjk.org.cn/Article/details/gt3ohkvyjkz.html

[S18] C：命令行参数
来源：http://www.52xcode.cn/Article/details/gt3fjkylkcx.html

int main(int argc, char **argv)
来源：http://www.ydjk.org.cn/Article/details/gt3epwdkoyl.html

[S19] C：快速排序
来源：http://www.52xcode.cn/Article/details/gt3yfatnbuj.html

qsort(a, n, sizeof(int), cmp);
来源：http://www.52xcode.cn/Article/details/gt3gjpqrsgi.html

[S20] C：二分查找
来源：http://www.ydjk.org.cn/Article/details/gt3apnchwlg.html

bsearch(&key, a, n, sizeof(int), cmp);
来源：http://www.ydjk.org.cn/Article/details/gt3jisdtbyd.html

[S21] C：字符类别判断
来源：http://www.52xcode.cn/Article/details/gt3bogzsxfr.html

isdigit(c);  isalpha(c);  isspace(c);
来源：http://www.52xcode.cn/Article/details/gt3isihmcra.html

[S22] C：字符串转数字
来源：http://www.52xcode.cn/Article/details/gt3ppjhhfth.html

atoi("42");  strtod("3.14", NULL);
来源：http://www.ydjk.org.cn/Article/details/gt3sjeudbay.html

[S23] C：随机数
来源：http://www.52xcode.cn/Article/details/gt3fsdjyniw.html

srand(time(NULL));  int r = rand() % 100;
来源：http://www.ydjk.org.cn/Article/details/gt3fbibaait.html

[S24] C：获取本地时间
来源：http://www.ydjk.org.cn/Article/details/gt3zoufhgcv.html

time_t t = time(NULL);  struct tm *tm = localtime(&t);
来源：http://www.52xcode.cn/Article/details/gt3xqrglsek.html

[S25] C：内存拷贝
来源：http://www.ydjk.org.cn/Article/details/gt3hpetyerk.html

memcpy(dst, src, n);
来源：http://www.52xcode.cn/Article/details/gt3edmntdgr.html

[S26] C：内存清零
来源：http://www.52xcode.cn/Article/details/gt3avrttaag.html

memset(a, 0, sizeof a);
来源：http://www.52xcode.cn/Article/details/gt3uzkuwaxa.html

[S27] C：定义常量
来源：http://www.ydjk.org.cn/Article/details/gt3tdagpmws.html

const double PI = 3.14159;
来源：http://www.ydjk.org.cn/Article/details/gt3xlgftykc.html

[S28] C：静态变量
来源：http://www.ydjk.org.cn/Article/details/gt3ntzyuzgv.html

static int counter = 0;
来源：http://www.52xcode.cn/Article/details/gt3eiwuykar.html

[S29] C：变参函数
来源：http://www.52xcode.cn/Article/details/gt3txgbmutb.html

va_list ap; va_start(ap, fmt); vprintf(fmt, ap); va_end(ap);
来源：http://www.52xcode.cn/Article/details/gt3boorkibz.html

[S30] C：头文件保护
来源：http://www.52xcode.cn/Article/details/gt3lkbtfqms.html

#ifndef X_H
来源：http://www.ydjk.org.cn/Article/details/gt3qqjuqvkt.html

#define X_H
来源：http://www.52xcode.cn/Article/details/gt3loywvygo.html

#endif
来源：http://www.ydjk.org.cn/Article/details/gt3wkgyjzxt.html

[S31] C++：Hello World
来源：http://www.ydjk.org.cn/Article/details/gt3cxjvsdyk.html

#include <iostream>
来源：http://www.52xcode.cn/Article/details/gt3cwvgnlne.html

int main() { std::cout << "Hello\n"; }
来源：http://www.ydjk.org.cn/Article/details/gt3irwdaahg.html

[S32] C++：字符串
来源：http://www.52xcode.cn/Article/details/gt3yeyvmwsc.html

std::string s = "hi";  s += "!";
来源：http://www.ydjk.org.cn/Article/details/gt3oizxetlb.html

[S33] C++：vector 增删
来源：http://www.52xcode.cn/Article/details/gt3nzqjqemi.html

std::vector<int> v{1, 2, 3};  v.push_back(4);
来源：http://www.ydjk.org.cn/Article/details/gt3wqifczdi.html

[S34] C++：遍历 vector
来源：http://www.52xcode.cn/Article/details/gt3fxdczpwr.html

for (auto &x : v) { std::cout << x; }
来源：http://www.ydjk.org.cn/Article/details/gt3klycownz.html

[S35] C++：map
来源：http://www.ydjk.org.cn/Article/details/gt3gbuyqjjk.html

std::map<std::string, int> m;  m["a"] = 1;
来源：http://www.ydjk.org.cn/Article/details/gt3rehxrmbr.html

[S36] C++：unordered_map
来源：http://www.52xcode.cn/Article/details/gt3dxsbgxtt.html

std::unordered_map<std::string, int> m;  m["a"] = 1;
来源：http://www.52xcode.cn/Article/details/gt3eyryricl.html

[S37] C++：set
来源：http://www.52xcode.cn/Article/details/gt3oiuipkpq.html

std::set<int> s{1, 2, 3};  s.insert(4);
来源：http://www.52xcode.cn/Article/details/gt3tykyedhn.html

[S38] C++：排序
来源：http://www.52xcode.cn/Article/details/gt3tagiunek.html

std::sort(v.begin(), v.end());
来源：http://www.52xcode.cn/Article/details/gt3sdmhyscp.html

[S39] C++：自定义比较器排序
来源：http://www.ydjk.org.cn/Article/details/gt3ycfofdzg.html

std::sort(v.begin(), v.end(), [](int a, int b) { return a > b; });
来源：http://www.ydjk.org.cn/Article/details/gt3yenixrae.html

[S40] C++：查找元素
来源：http://www.52xcode.cn/Article/details/gt3qxdxwzfr.html

auto it = std::find(v.begin(), v.end(), 3);
来源：http://www.52xcode.cn/Article/details/gt3raqpjqun.html

[S41] C++：类与构造函数
来源：http://www.ydjk.org.cn/Article/details/gt3bockmhtg.html

class A { public: A(int v) : x_(v) {} int get() const { return x_; } private: int x_; };
来源：http://www.ydjk.org.cn/Article/details/gt3acljapkm.html

[S42] C++：继承与虚函数
来源：http://www.52xcode.cn/Article/details/gt3ylslqdme.html

class B : public Base { public: void f() override {} };
来源：http://www.52xcode.cn/Article/details/gt3rquwudql.html

[S43] C++：智能指针
来源：http://www.ydjk.org.cn/Article/details/gt3mfwltaji.html

auto p = std::make_unique<int>(5);
来源：http://www.52xcode.cn/Article/details/gt3mvhpqoyn.html

[S44] C++：引用传参
来源：http://www.ydjk.org.cn/Article/details/gt3bggaxfon.html

void inc(int &x) { ++x; }
来源：http://www.ydjk.org.cn/Article/details/gt3wtgcfzik.html

[S45] C++：lambda
来源：http://www.52xcode.cn/Article/details/gt3myndzekj.html

auto add = [](int a, int b) { return a + b; };
来源：http://www.ydjk.org.cn/Article/details/gt3fqklusfb.html

[S46] C++：函数模板
来源：http://www.ydjk.org.cn/Article/details/gt3izjtuxhg.html

template <typename T> T maxv(T a, T b) { return a > b ? a : b; }
来源：http://www.52xcode.cn/Article/details/gt3bsniqkub.html

[S47] C++：结构化绑定遍历
来源：http://www.52xcode.cn/Article/details/gt3sptyruyp.html

for (const auto &[k, v] : m) { std::cout << k << v; }
来源：http://www.52xcode.cn/Article/details/gt3izvvauqp.html

[S48] C++：逐行读文件
来源：http://www.ydjk.org.cn/Article/details/gt3vzrufodd.html

std::ifstream in("a.txt");  std::string line;
来源：http://www.ydjk.org.cn/Article/details/gt3sryybyvq.html

while (std::getline(in, line)) { }
来源：http://www.52xcode.cn/Article/details/gt3nbfcxhmy.html

[S49] C++：写文件
来源：http://www.52xcode.cn/Article/details/gt3vlfbxtdw.html

std::ofstream out("a.txt");  out << "hi\n";
来源：http://www.52xcode.cn/Article/details/gt3xullaorm.html

[S50] C++：格式化数字
来源：http://www.ydjk.org.cn/Article/details/gt3uvkyehdm.html

std::ostringstream os;  os << std::fixed << std::setprecision(2) << 3.14159;
来源：http://www.52xcode.cn/Article/details/gt3cyanaieu.html

[S51] C++：显式类型转换
来源：http://www.52xcode.cn/Article/details/gt3rlxozomw.html

static_cast<double>(a) / b
来源：http://www.52xcode.cn/Article/details/gt3qgjachfo.html

[S52] C++：const 与 noexcept
来源：http://www.52xcode.cn/Article/details/gt3mfwxawtr.html

int size() const noexcept { return n_; }
来源：http://www.52xcode.cn/Article/details/gt3bcmvkhxc.html

[S53] C++：移动语义
来源：http://www.52xcode.cn/Article/details/gt3ppeexdvc.html

std::vector<int> w = std::move(v);
来源：http://www.ydjk.org.cn/Article/details/gt3mobulfck.html

[S54] C++：异常处理
来源：http://www.52xcode.cn/Article/details/gt3ftrppnkp.html

try { throw std::runtime_error("x"); } catch (const std::exception &e) { }
来源：http://www.52xcode.cn/Article/details/gt3ugbimvnl.html

[S55] C++：结构化绑定
来源：http://www.ydjk.org.cn/Article/details/gt3paoaqjns.html

auto [a, b] = std::make_pair(1, 2);
来源：http://www.52xcode.cn/Article/details/gt3zwbinnwa.html

[S56] C++：optional
来源：http://www.52xcode.cn/Article/details/gt3lvzaqhvu.html

std::optional<int> o = 5;  if (o) { int v = *o; }
来源：http://www.ydjk.org.cn/Article/details/gt3jhaypcpd.html

[S57] C++：编译期常量
来源：http://www.ydjk.org.cn/Article/details/gt3speikcbw.html

constexpr int N = 10;
来源：http://www.ydjk.org.cn/Article/details/gt3swczlnys.html

[S58] C++：命名空间
来源：http://www.ydjk.org.cn/Article/details/gt3oukmhljc.html

namespace ns { int f() { return 1; } }
来源：http://www.52xcode.cn/Article/details/gt3bqkhkwms.html

[S59] C++：静态断言
来源：http://www.52xcode.cn/Article/details/gt3utzqovrl.html

static_assert(sizeof(int) == 4, "int 必须 4 字节");
来源：http://www.52xcode.cn/Article/details/gt3mcmkbymh.html

[S60] C++：遍历并删除元素
来源：http://www.ydjk.org.cn/Article/details/gt3tjdfrjzr.html

v.erase(std::remove_if(v.begin(), v.end(), [](int x) { return x < 0; }), v.end());
来源：http://www.ydjk.org.cn/Article/details/gt3hjetkvso.html

================================================================================
来源：http://www.ydjk.org.cn/Article/details/gt3uncqzxyr.html

T. 其他语言补充（Kotlin / Swift / Lua / Perl / Scala）
来源：http://www.52xcode.cn/Article/details/gt3nuetjxro.html

================================================================================
来源：http://www.ydjk.org.cn/Article/details/gt3invguqeo.html

[T01] Kotlin：Hello World
来源：http://www.52xcode.cn/Article/details/gt3lskgcpxc.html

println("Hello")
来源：http://www.52xcode.cn/Article/details/gt3mslgtzmm.html

[T02] Kotlin：变量
来源：http://www.52xcode.cn/Article/details/gt3ckntplce.html

val a = 1;  var b = 2        // val 只读，var 可变
来源：http://www.ydjk.org.cn/Article/details/gt3hecwniyd.html

[T03] Kotlin：字符串模板
来源：http://www.52xcode.cn/Article/details/gt3alflwlnf.html

"值: $b"
来源：http://www.ydjk.org.cn/Article/details/gt3tndfrzkc.html

[T04] Kotlin：空安全
来源：http://www.52xcode.cn/Article/details/gt3islevjle.html

val n: String? = null;  n?.length
来源：http://www.ydjk.org.cn/Article/details/gt3wuwcqroi.html

[T05] Kotlin：when 表达式
来源：http://www.52xcode.cn/Article/details/gt3pjrczeaf.html

val s = when (x) { 1 -> "一" else -> "其他" }   // 多分支时每个分支单独一行
来源：http://www.ydjk.org.cn/Article/details/gt3wazfnnsx.html

[T06] Kotlin：集合映射
来源：http://www.ydjk.org.cn/Article/details/gt3xiaghivs.html

listOf(1, 2, 3).map { it * 2 }
来源：http://www.ydjk.org.cn/Article/details/gt3rvoavzks.html

[T07] Kotlin：集合过滤
来源：http://www.ydjk.org.cn/Article/details/gt3pnpdexdg.html

listOf(1, 2, 3).filter { it > 1 }
来源：http://www.52xcode.cn/Article/details/gt3fzviuncx.html

[T08] Kotlin：数据类
来源：http://www.52xcode.cn/Article/details/gt3sjwffhou.html

data class User(val name: String, val age: Int)
来源：http://www.ydjk.org.cn/Article/details/gt3dxmxcmyq.html

[T09] Kotlin：扩展函数
来源：http://www.ydjk.org.cn/Article/details/gt3pbjbnqjt.html

fun String.exclaim() = this + "!"
来源：http://www.52xcode.cn/Article/details/gt3olegyapp.html

[T10] Kotlin：默认参数
来源：http://www.52xcode.cn/Article/details/gt3gknjkncx.html

fun greet(name: String = "World") = "Hi $name"
来源：http://www.52xcode.cn/Article/details/gt3jigvojzk.html

[T11] Kotlin：协程
来源：http://www.52xcode.cn/Article/details/gt3lawerfcc.html

GlobalScope.launch { delay(1000); println("done") }
来源：http://www.ydjk.org.cn/Article/details/gt3myspztby.html

[T12] Kotlin：解构声明
来源：http://www.52xcode.cn/Article/details/gt3kkcfqxum.html

val (a, b) = Pair(1, 2)
来源：http://www.52xcode.cn/Article/details/gt3phmctbff.html

[T13] Kotlin：只读 Map
来源：http://www.ydjk.org.cn/Article/details/gt3twnowkso.html

val m = mapOf("a" to 1)
来源：http://www.52xcode.cn/Article/details/gt3mhbtwdlq.html

[T14] Kotlin：循环
来源：http://www.52xcode.cn/Article/details/gt3jhdniwtl.html

for (i in 1..10) println(i)
来源：http://www.ydjk.org.cn/Article/details/gt3nciwrmcg.html

[T15] Kotlin：接口
来源：http://www.52xcode.cn/Article/details/gt3nyciywjx.html

interface Shape { fun area(): Double }
来源：http://www.ydjk.org.cn/Article/details/gt3aneemnnp.html

[T16] Swift：Hello World
来源：http://www.ydjk.org.cn/Article/details/gt3irnofuln.html

print("Hello")
来源：http://www.52xcode.cn/Article/details/gt3ekofvjru.html

[T17] Swift：变量与常量
来源：http://www.ydjk.org.cn/Article/details/gt3oaxndtyf.html

var a = 1;  let b = 2
来源：http://www.52xcode.cn/Article/details/gt3covbmauw.html

[T18] Swift：字符串插值
来源：http://www.52xcode.cn/Article/details/gt3ktwltfho.html

"值: \(b)"
来源：http://www.52xcode.cn/Article/details/gt3uhywvtij.html

[T19] Swift：可选绑定
来源：http://www.52xcode.cn/Article/details/gt3kwcoeojv.html

if let n = opt { print(n) }
来源：http://www.ydjk.org.cn/Article/details/gt3bqzjeqwo.html

[T20] Swift：数组操作
来源：http://www.ydjk.org.cn/Article/details/gt3arzslcbm.html

var a = [1, 2, 3];  a.append(4)
来源：http://www.ydjk.org.cn/Article/details/gt3dvkskkpy.html

[T21] Swift：遍历
来源：http://www.52xcode.cn/Article/details/gt3xmfwjpvp.html

for x in a { print(x) }
来源：http://www.52xcode.cn/Article/details/gt3gzigmcko.html

[T22] Swift：字典
来源：http://www.ydjk.org.cn/Article/details/gt3ywnvsuxp.html

var d = ["a": 1];  d["b"] = 2
来源：http://www.52xcode.cn/Article/details/gt3suuzktlj.html

[T23] Swift：函数
来源：http://www.ydjk.org.cn/Article/details/gt3ebjmhowa.html

func add(_ a: Int, _ b: Int) -> Int { a + b }
来源：http://www.52xcode.cn/Article/details/gt3xlpvjyva.html

[T24] Swift：闭包
来源：http://www.52xcode.cn/Article/details/gt3joaaecma.html

let f = { (x: Int) -> Int in x * 2 }
来源：http://www.52xcode.cn/Article/details/gt3ssxxwugt.html

[T25] Swift：结构体
来源：http://www.52xcode.cn/Article/details/gt3kuzphjar.html

struct P { var x: Int }
来源：http://www.52xcode.cn/Article/details/gt3kjoxaabr.html

[T26] Swift：类与重写
来源：http://www.ydjk.org.cn/Article/details/gt3nejmluae.html

class A: Base { override func f() {} }
来源：http://www.52xcode.cn/Article/details/gt3baurtgfl.html

[T27] Swift：错误处理
来源：http://www.ydjk.org.cn/Article/details/gt3macvmzda.html

do { try f() } catch { print(error) }
来源：http://www.ydjk.org.cn/Article/details/gt3ijzhfliv.html

[T28] Swift：枚举
来源：http://www.ydjk.org.cn/Article/details/gt3dsdnomye.html

enum Color { case red, green }
来源：http://www.52xcode.cn/Article/details/gt3tbxsaaic.html

[T29] Swift：guard 提前返回
来源：http://www.52xcode.cn/Article/details/gt3hwbxyftw.html

guard let x = opt else { return }
来源：http://www.52xcode.cn/Article/details/gt3mbnfiepj.html

[T30] Swift：协议
来源：http://www.ydjk.org.cn/Article/details/gt3qmogmjbw.html

protocol Shape { func area() -> Double }
来源：http://www.52xcode.cn/Article/details/gt3evpcttfj.html

[T31] Lua：Hello World
来源：http://www.ydjk.org.cn/Article/details/gt3bnxdijpb.html

print("Hello")
来源：http://www.52xcode.cn/Article/details/gt3tltktbkz.html

[T32] Lua：局部变量
来源：http://www.52xcode.cn/Article/details/gt3iomoueze.html

local a = 1
来源：http://www.52xcode.cn/Article/details/gt3iaiwhrgl.html

[T33] Lua：表（数组）
来源：http://www.ydjk.org.cn/Article/details/gt3iqmzqgsq.html

local t = {1, 2, 3};  t[4] = 4
来源：http://www.ydjk.org.cn/Article/details/gt3jbimnjsf.html

[T34] Lua：遍历表
来源：http://www.ydjk.org.cn/Article/details/gt3lzilckaw.html

for i, v in ipairs(t) do print(i, v) end
来源：http://www.ydjk.org.cn/Article/details/gt3zzbnuddq.html

[T35] Lua：字典表
来源：http://www.52xcode.cn/Article/details/gt3unoeyntg.html

local d = { a = 1 };  d.b = 2
来源：http://www.52xcode.cn/Article/details/gt3kvgcxljf.html

[T36] Lua：函数
来源：http://www.ydjk.org.cn/Article/details/gt3inwxzybg.html

function add(a, b) return a + b end
来源：http://www.52xcode.cn/Article/details/gt3bqqmhsyd.html

[T37] Lua：字符串拼接
来源：http://www.ydjk.org.cn/Article/details/gt3iihushjd.html

"a" .. "b"
来源：http://www.ydjk.org.cn/Article/details/gt3srvuwryl.html

[T38] Lua：条件
来源：http://www.ydjk.org.cn/Article/details/gt3swvfitfw.html

if x > 0 then print("正") end
来源：http://www.ydjk.org.cn/Article/details/gt3zsbariuc.html

[T39] Lua：模式匹配
来源：http://www.ydjk.org.cn/Article/details/gt3xbxzjcgc.html

string.find(s, "%d+")
来源：http://www.52xcode.cn/Article/details/gt3gnlqamtg.html

[T40] Lua：元表
来源：http://www.52xcode.cn/Article/details/gt3dhgbqdjr.html

setmetatable({}, { __index = base })
来源：http://www.ydjk.org.cn/Article/details/gt3azwiwaza.html

[T41] Perl：Hello World
来源：http://www.ydjk.org.cn/Article/details/gt3pbbibgph.html

print "Hello\n";
来源：http://www.52xcode.cn/Article/details/gt3cwpkhcul.html

[T42] Perl：变量类型
来源：http://www.52xcode.cn/Article/details/gt3gvvbkkqw.html

my $a = 1;  my @arr = (1, 2, 3);  my %h = (a => 1);
来源：http://www.ydjk.org.cn/Article/details/gt3vekjzyol.html

[T43] Perl：字符串插值
来源：http://www.ydjk.org.cn/Article/details/gt3avoqrrri.html

"值: $a"
来源：http://www.ydjk.org.cn/Article/details/gt3exuxxhyd.html

[T44] Perl：条件
来源：http://www.52xcode.cn/Article/details/gt3aybmbboc.html

if ($a > 0) { print "正"; }
来源：http://www.52xcode.cn/Article/details/gt3mobolbmp.html

[T45] Perl：数组遍历
来源：http://www.ydjk.org.cn/Article/details/gt3yqazxgat.html

for my $x (@arr) { print $x; }
来源：http://www.52xcode.cn/Article/details/gt3ecsoaxvk.html

[T46] Perl：哈希操作
来源：http://www.ydjk.org.cn/Article/details/gt3xlmcsloy.html

$h{b} = 2;  for my $k (keys %h) { print "$k=$h{$k}"; }
来源：http://www.52xcode.cn/Article/details/gt3erjxbydg.html

[T47] Perl：正则捕获
来源：http://www.52xcode.cn/Article/details/gt3yymxncgx.html

if ($s =~ /(\d+)/) { print $1; }
来源：http://www.52xcode.cn/Article/details/gt3svggqkjl.html

[T48] Perl：正则替换
来源：http://www.52xcode.cn/Article/details/gt3lqlvhlqw.html

$s =~ s/old/new/g;
来源：http://www.ydjk.org.cn/Article/details/gt3wwrbpygc.html

[T49] Perl：函数
来源：http://www.52xcode.cn/Article/details/gt3mawpemgl.html

sub add { my ($a, $b) = @_; return $a + $b; }
来源：http://www.52xcode.cn/Article/details/gt3rkcayvjs.html

[T50] Perl：逐行读文件
来源：http://www.52xcode.cn/Article/details/gt3souermhd.html

open my $fh, "<", "a.txt" or die $!;
来源：http://www.ydjk.org.cn/Article/details/gt3ugcqwrjb.html

while (my $line = <$fh>) { print $line; }
来源：http://www.52xcode.cn/Article/details/gt3hntghpmx.html

[T51] Scala：Hello World
来源：http://www.52xcode.cn/Article/details/gt3njrriitw.html

println("Hello")
来源：http://www.ydjk.org.cn/Article/details/gt3gzjbpwto.html

[T52] Scala：变量
来源：http://www.ydjk.org.cn/Article/details/gt3waroqhgp.html

val a = 1;  var b = 2
来源：http://www.52xcode.cn/Article/details/gt3nkxkpmti.html

[T53] Scala：字符串插值
来源：http://www.ydjk.org.cn/Article/details/gt3ezpmhxop.html

s"值: $b"
来源：http://www.52xcode.cn/Article/details/gt3qgewukom.html

[T54] Scala：集合映射
来源：http://www.52xcode.cn/Article/details/gt3tjbibnyh.html

List(1, 2, 3).map(_ * 2)
来源：http://www.ydjk.org.cn/Article/details/gt3lxwtgctr.html

[T55] Scala：集合过滤
来源：http://www.52xcode.cn/Article/details/gt3fvnakvbf.html

List(1, 2, 3).filter(_ > 1)
来源：http://www.52xcode.cn/Article/details/gt3bflisnay.html

[T56] Scala：样例类
来源：http://www.ydjk.org.cn/Article/details/gt3usatsudl.html

case class User(name: String, age: Int)
来源：http://www.ydjk.org.cn/Article/details/gt3xnygzoqp.html

[T57] Scala：模式匹配
来源：http://www.52xcode.cn/Article/details/gt3rquyvuyc.html

x match { case 1 => "一"; case _ => "其他" }
来源：http://www.52xcode.cn/Article/details/gt3qnfsazxr.html

[T58] Scala：函数定义
来源：http://www.ydjk.org.cn/Article/details/gt3vgqliiwf.html

def add(a: Int, b: Int): Int = a + b
来源：http://www.52xcode.cn/Article/details/gt3kamoxbad.html

[T59] Scala：循环
来源：http://www.52xcode.cn/Article/details/gt3lpwuuhxa.html

for (i <- 1 to 10) println(i)
来源：http://www.ydjk.org.cn/Article/details/gt3rvyiegtc.html

[T60] Scala：折叠
来源：http://www.ydjk.org.cn/Article/details/gt3cojxzmow.html

List(1, 2, 3).foldLeft(0)(_ + _)
来源：http://www.ydjk.org.cn/Article/details/gt3gqiqxkym.html

================================================================================
来源：http://www.ydjk.org.cn/Article/details/gt3pjszrugb.html

U. 高频实用片段（Python / PHP / JavaScript 各 40 条）
来源：http://www.ydjk.org.cn/Article/details/gt3kwdqoora.html

================================================================================
来源：http://www.52xcode.cn/Article/details/gt3dsfkrahg.html

[U01] Py：创建虚拟环境
来源：http://www.ydjk.org.cn/Article/details/gt3tduauosq.html

python -m venv .venv && source .venv/bin/activate
来源：http://www.52xcode.cn/Article/details/gt3ptltnyzi.html

[U02] Py：导出 / 安装依赖
来源：http://www.ydjk.org.cn/Article/details/gt3ekxziycd.html

pip freeze > requirements.txt;  pip install -r requirements.txt
来源：http://www.52xcode.cn/Article/details/gt3hnxrryxl.html

[U03] Py：加载 .env 配置
来源：http://www.52xcode.cn/Article/details/gt3jrvcnvyb.html

from dotenv import load_dotenv; load_dotenv()
来源：http://www.ydjk.org.cn/Article/details/gt3zpxfnogy.html

[U04] Py：变量调试打印
来源：http://www.ydjk.org.cn/Article/details/gt3zbdvrkvv.html

print(f"{x=}")            # 输出 x=值，Python 3.8+
来源：http://www.ydjk.org.cn/Article/details/gt3kvplpnvs.html


<!-- 参考信息 -->