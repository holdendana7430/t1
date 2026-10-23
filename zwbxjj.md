代发 wailian999

free -h;  ps aux | grep nginx
来源：http://www.ydjk.org.cn/Article/details/gt3apkexxqz.html

[R64] 结束进程
来源：http://www.ydjk.org.cn/Article/details/gt3aalpkfaf.html

kill -9 $(pgrep -f app.py)
来源：http://www.52xcode.cn/Article/details/gt3agoahbnp.html

[R65] 查看端口占用
来源：http://www.ydjk.org.cn/Article/details/gt3rddjoipg.html

ss -tlnp | grep 8080;  lsof -i:8080
来源：http://www.52xcode.cn/Article/details/gt3drqfjfli.html

[R66] 定时任务
来源：http://www.ydjk.org.cn/Article/details/gt3qvkuhzad.html

crontab -e;  crontab -l
来源：http://www.ydjk.org.cn/Article/details/gt3rwqdbyef.html

[R67] 生成随机十六进制串
来源：http://www.ydjk.org.cn/Article/details/gt3nucajdpq.html

openssl rand -hex 16
来源：http://www.52xcode.cn/Article/details/gt3pjxclipr.html

[R68] 计算文件校验值
来源：http://www.52xcode.cn/Article/details/gt3nchiwtpf.html

sha256sum a.txt;  md5sum a.txt
来源：http://www.ydjk.org.cn/Article/details/gt3dnuinwxd.html

[R69] 生成随机密码
来源：http://www.52xcode.cn/Article/details/gt3umtyawst.html

head -c 16 /dev/urandom | base64
来源：http://www.ydjk.org.cn/Article/details/gt3uuyquzcz.html

[R70] 时间戳与互转
来源：http://www.ydjk.org.cn/Article/details/gt3pjikqjsx.html

date +%s;  date -d @1700000000
来源：http://www.ydjk.org.cn/Article/details/gt3bqetvmuq.html

[R71] 日期格式化
来源：http://www.52xcode.cn/Article/details/gt3qqjvhdzj.html

date +"%Y-%m-%d %H:%M:%S"
来源：http://www.52xcode.cn/Article/details/gt3fdjyblwv.html

[R72] 等待端口就绪
来源：http://www.ydjk.org.cn/Article/details/gt3osidyvbo.html

until nc -z localhost 3306; do sleep 1; done
来源：http://www.52xcode.cn/Article/details/gt3rlytgtfr.html

[R73] 分割大日志
来源：http://www.52xcode.cn/Article/details/gt3plzvccst.html

split -l 1000 big.log part_
来源：http://www.52xcode.cn/Article/details/gt3cquekazc.html

[R74] 批量重命名
来源：http://www.52xcode.cn/Article/details/gt3qoxaimai.html

for f in *.jpeg; do mv "$f" "${f%.jpeg}.jpg"; done
来源：http://www.52xcode.cn/Article/details/gt3hygqvbuz.html

[R75] 导出环境变量
来源：http://www.ydjk.org.cn/Article/details/gt3ezjkqirq.html

export PATH="$HOME/bin:$PATH"
来源：http://www.ydjk.org.cn/Article/details/gt3jugfugdt.html

[R76] 使用临时文件
来源：http://www.ydjk.org.cn/Article/details/gt3kofhmfqe.html

tmp=$(mktemp); trap 'rm -f "$tmp"' EXIT
来源：http://www.ydjk.org.cn/Article/details/gt3ndiaxtxn.html

[R77] 读取用户输入
来源：http://www.ydjk.org.cn/Article/details/gt3iixdvabl.html

read -rp "请输入: " ans
来源：http://www.52xcode.cn/Article/details/gt3uowwiwud.html

[R78] 交互式菜单
来源：http://www.ydjk.org.cn/Article/details/gt3qgqpqqng.html

select opt in a b c; do echo "$opt"; break; done
来源：http://www.52xcode.cn/Article/details/gt3dbsnkfeb.html

[R79] 解析命令行选项
来源：http://www.52xcode.cn/Article/details/gt3hcaknafw.html

while getopts "v:f:" o; do case $o in v) V=$OPTARG ;; f) F=$OPTARG ;; esac; done
来源：http://www.52xcode.cn/Article/details/gt3ptkikzbk.html

[R80] 查看脚本执行耗时
来源：http://www.ydjk.org.cn/Article/details/gt3lmzkgqxr.html

time ./run.sh
来源：http://www.ydjk.org.cn/Article/details/gt3kkvpjadw.html

================================================================================
来源：http://www.52xcode.cn/Article/details/gt3rasspwkc.html

S. C / C++ 专题
来源：http://www.ydjk.org.cn/Article/details/gt3bwqrxbbs.html

================================================================================
来源：http://www.52xcode.cn/Article/details/gt3dszuevlx.html

[S01] C：Hello World
来源：http://www.52xcode.cn/Article/details/gt3gxdwznsd.html

#include <stdio.h>
来源：http://www.52xcode.cn/Article/details/gt3mabobcck.html

int main(void) { printf("Hello\n"); return 0; }
来源：http://www.ydjk.org.cn/Article/details/gt3vnidxlwy.html

[S02] C：变量与格式化输出
来源：http://www.ydjk.org.cn/Article/details/gt3pjgccxdv.html

int a = 10; printf("%d\n", a);
来源：http://www.ydjk.org.cn/Article/details/gt3kjylahzq.html

[S03] C：读入整数
来源：http://www.ydjk.org.cn/Article/details/gt3kgrnzgac.html

int x; scanf("%d", &x);
来源：http://www.52xcode.cn/Article/details/gt3behoerxr.html

[S04] C：字符串复制
来源：http://www.52xcode.cn/Article/details/gt3oawxzxly.html

char dst[32]; strcpy(dst, "hi");
来源：http://www.52xcode.cn/Article/details/gt3renjkjtb.html

[S05] C：字符串长度
来源：http://www.ydjk.org.cn/Article/details/gt3rlcjqxqa.html

strlen(s)
来源：http://www.52xcode.cn/Article/details/gt3gkzwmtvn.html

[S06] C：字符串比较
来源：http://www.ydjk.org.cn/Article/details/gt3vrgrwsjz.html

strcmp(a, b) == 0
来源：http://www.52xcode.cn/Article/details/gt3qgpbcrei.html

[S07] C：数组遍历求和
来源：http://www.52xcode.cn/Article/details/gt3ghrgqiyc.html

for (int i = 0; i < n; i++) sum += a[i];
来源：http://www.ydjk.org.cn/Article/details/gt3gefmjqhs.html

[S08] C：动态内存分配与释放
来源：http://www.ydjk.org.cn/Article/details/gt3vzafalon.html

int *p = malloc(sizeof(int) * n); ... free(p);
来源：http://www.ydjk.org.cn/Article/details/gt3yotxxemy.html

[S09] C：结构体定义与初始化
来源：http://www.ydjk.org.cn/Article/details/gt3vxnrdejk.html

struct Point { int x, y; };  struct Point p = {1, 2};
来源：http://www.52xcode.cn/Article/details/gt3wrfiboph.html

[S10] C：指针与解引用
来源：http://www.ydjk.org.cn/Article/details/gt3vrdbgdnb.html

int *p = &a;  *p = 5;
来源：http://www.52xcode.cn/Article/details/gt3axbwnicx.html

[S11] C：逐行读文件
来源：http://www.ydjk.org.cn/Article/details/gt3nunaxajz.html

FILE *f = fopen("a.txt", "r");
来源：http://www.52xcode.cn/Article/details/gt3wmtlslab.html

while (fgets(buf, sizeof buf, f)) { }
来源：http://www.52xcode.cn/Article/details/gt3hoqdpddw.html

fclose(f);
来源：http://www.ydjk.org.cn/Article/details/gt3naznwlfn.html

[S12] C：写文件
来源：http://www.ydjk.org.cn/Article/details/gt3toybbxxz.html

FILE *f = fopen("a.txt", "w");  fprintf(f, "hi\n");  fclose(f);
来源：http://www.52xcode.cn/Article/details/gt3wygykesj.html

[S13] C：宏定义
来源：http://www.52xcode.cn/Article/details/gt3tmobsyzp.html

#define MAX(a, b) ((a) > (b) ? (a) : (b))
来源：http://www.52xcode.cn/Article/details/gt3fndzpwre.html

[S14] C：枚举
来源：http://www.52xcode.cn/Article/details/gt3asntylwt.html

enum Color { RED, GREEN, BLUE };
来源：http://www.52xcode.cn/Article/details/gt3hdlywfqn.html

[S15] C：类型转换
来源：http://www.52xcode.cn/Article/details/gt3cykgusdp.html

(double) a / b
来源：http://www.ydjk.org.cn/Article/details/gt3bjsltkrt.html

[S16] C：位操作置位
来源：http://www.52xcode.cn/Article/details/gt3hyadiomv.html

x |= (1 << 3);
来源：http://www.52xcode.cn/Article/details/gt3ryvxbote.html

[S17] C：安全拼接字符串
来源：http://www.52xcode.cn/Article/details/gt3uphazixj.html

snprintf(buf, sizeof buf, "%s%s", a, b);
来源：http://www.ydjk.org.cn/Article/details/gt3qxkewwvt.html

[S18] C：命令行参数
来源：http://www.ydjk.org.cn/Article/details/gt3nclvjrni.html

int main(int argc, char **argv)
来源：http://www.ydjk.org.cn/Article/details/gt3kxklxxad.html

[S19] C：快速排序
来源：http://www.52xcode.cn/Article/details/gt3fwtcxhqj.html

qsort(a, n, sizeof(int), cmp);
来源：http://www.ydjk.org.cn/Article/details/gt3swbbgraq.html

[S20] C：二分查找
来源：http://www.ydjk.org.cn/Article/details/gt3fypubdqs.html

bsearch(&key, a, n, sizeof(int), cmp);
来源：http://www.52xcode.cn/Article/details/gt3xvqjtbcq.html

[S21] C：字符类别判断
来源：http://www.ydjk.org.cn/Article/details/gt3znmgrfpk.html

isdigit(c);  isalpha(c);  isspace(c);
来源：http://www.ydjk.org.cn/Article/details/gt3yviklopi.html

[S22] C：字符串转数字
来源：http://www.ydjk.org.cn/Article/details/gt3oejawlgc.html

atoi("42");  strtod("3.14", NULL);
来源：http://www.52xcode.cn/Article/details/gt3bfwnxnuu.html

[S23] C：随机数
来源：http://www.52xcode.cn/Article/details/gt3ybnopgvh.html

srand(time(NULL));  int r = rand() % 100;
来源：http://www.52xcode.cn/Article/details/gt3fuvptmbs.html

[S24] C：获取本地时间
来源：http://www.ydjk.org.cn/Article/details/gt3qjttieri.html

time_t t = time(NULL);  struct tm *tm = localtime(&t);
来源：http://www.ydjk.org.cn/Article/details/gt3cagleweo.html

[S25] C：内存拷贝
来源：http://www.52xcode.cn/Article/details/gt3ewehfekp.html

memcpy(dst, src, n);
来源：http://www.ydjk.org.cn/Article/details/gt3wrckwwtz.html

[S26] C：内存清零
来源：http://www.ydjk.org.cn/Article/details/gt3dmebyybu.html

memset(a, 0, sizeof a);
来源：http://www.ydjk.org.cn/Article/details/gt3ugihnatw.html

[S27] C：定义常量
来源：http://www.ydjk.org.cn/Article/details/gt3bmlhooiq.html

const double PI = 3.14159;
来源：http://www.ydjk.org.cn/Article/details/gt3pkhnarks.html

[S28] C：静态变量
来源：http://www.ydjk.org.cn/Article/details/gt3hfbyrxqp.html

static int counter = 0;
来源：http://www.ydjk.org.cn/Article/details/gt3ymyffjnt.html

[S29] C：变参函数
来源：http://www.ydjk.org.cn/Article/details/gt3gkyrmjfe.html

va_list ap; va_start(ap, fmt); vprintf(fmt, ap); va_end(ap);
来源：http://www.52xcode.cn/Article/details/gt3rhtqsktl.html

[S30] C：头文件保护
来源：http://www.ydjk.org.cn/Article/details/gt3nzjfhnle.html

#ifndef X_H
来源：http://www.ydjk.org.cn/Article/details/gt3asxrealp.html

#define X_H
来源：http://www.ydjk.org.cn/Article/details/gt3hohvqqbw.html

#endif
来源：http://www.52xcode.cn/Article/details/gt3hwrpxhsb.html

[S31] C++：Hello World
来源：http://www.ydjk.org.cn/Article/details/gt3pmskgpfg.html

#include <iostream>
来源：http://www.ydjk.org.cn/Article/details/gt3audgmffb.html

int main() { std::cout << "Hello\n"; }
来源：http://www.52xcode.cn/Article/details/gt3skfiinpa.html

[S32] C++：字符串
来源：http://www.ydjk.org.cn/Article/details/gt3zwgfkgff.html

std::string s = "hi";  s += "!";
来源：http://www.52xcode.cn/Article/details/gt3kuiyknfc.html

[S33] C++：vector 增删
来源：http://www.ydjk.org.cn/Article/details/gt3qoegoypu.html

std::vector<int> v{1, 2, 3};  v.push_back(4);
来源：http://www.ydjk.org.cn/Article/details/gt3xhaadgbp.html

[S34] C++：遍历 vector
来源：http://www.52xcode.cn/Article/details/gt3mxaapkss.html

for (auto &x : v) { std::cout << x; }
来源：http://www.ydjk.org.cn/Article/details/gt3dqxidedu.html

[S35] C++：map
来源：http://www.52xcode.cn/Article/details/gt3cyrhjzlu.html

std::map<std::string, int> m;  m["a"] = 1;
来源：http://www.ydjk.org.cn/Article/details/gt3ivthoqrr.html

[S36] C++：unordered_map
来源：http://www.52xcode.cn/Article/details/gt3vzrxlszh.html

std::unordered_map<std::string, int> m;  m["a"] = 1;
来源：http://www.52xcode.cn/Article/details/gt3uzhijjue.html

[S37] C++：set
来源：http://www.ydjk.org.cn/Article/details/gt3muuphwqt.html

std::set<int> s{1, 2, 3};  s.insert(4);
来源：http://www.52xcode.cn/Article/details/gt3ksqgnroa.html

[S38] C++：排序
来源：http://www.ydjk.org.cn/Article/details/gt3flnjrrbu.html

std::sort(v.begin(), v.end());
来源：http://www.ydjk.org.cn/Article/details/gt3nbrdcrnj.html

[S39] C++：自定义比较器排序
来源：http://www.ydjk.org.cn/Article/details/gt3ypdmbgeo.html

std::sort(v.begin(), v.end(), [](int a, int b) { return a > b; });
来源：http://www.52xcode.cn/Article/details/gt3iguespff.html

[S40] C++：查找元素
来源：http://www.52xcode.cn/Article/details/gt3blkvlooi.html

auto it = std::find(v.begin(), v.end(), 3);
来源：http://www.52xcode.cn/Article/details/gt3zyqmujdm.html

[S41] C++：类与构造函数
来源：http://www.52xcode.cn/Article/details/gt3dbcppzbw.html

class A { public: A(int v) : x_(v) {} int get() const { return x_; } private: int x_; };
来源：http://www.ydjk.org.cn/Article/details/gt3jylfwazc.html

[S42] C++：继承与虚函数
来源：http://www.ydjk.org.cn/Article/details/gt3reqjavib.html

class B : public Base { public: void f() override {} };
来源：http://www.52xcode.cn/Article/details/gt3klhomkkv.html

[S43] C++：智能指针
来源：http://www.52xcode.cn/Article/details/gt3qmkhajju.html

auto p = std::make_unique<int>(5);
来源：http://www.ydjk.org.cn/Article/details/gt3eylqqsja.html

[S44] C++：引用传参
来源：http://www.ydjk.org.cn/Article/details/gt3titplmxo.html

void inc(int &x) { ++x; }
来源：http://www.52xcode.cn/Article/details/gt3dgtqmrha.html

[S45] C++：lambda
来源：http://www.ydjk.org.cn/Article/details/gt3dynnkioa.html

auto add = [](int a, int b) { return a + b; };
来源：http://www.52xcode.cn/Article/details/gt3yyoerlqh.html

[S46] C++：函数模板
来源：http://www.ydjk.org.cn/Article/details/gt3eprebcpi.html

template <typename T> T maxv(T a, T b) { return a > b ? a : b; }
来源：http://www.52xcode.cn/Article/details/gt3vvbdxdxe.html

[S47] C++：结构化绑定遍历
来源：http://www.ydjk.org.cn/Article/details/gt3bnygfgbv.html

for (const auto &[k, v] : m) { std::cout << k << v; }
来源：http://www.52xcode.cn/Article/details/gt3pdvdzezr.html

[S48] C++：逐行读文件
来源：http://www.52xcode.cn/Article/details/gt3ajlmtrxq.html

std::ifstream in("a.txt");  std::string line;
来源：http://www.ydjk.org.cn/Article/details/gt3tguajmjc.html

while (std::getline(in, line)) { }
来源：http://www.52xcode.cn/Article/details/gt3gkvvierz.html

[S49] C++：写文件
来源：http://www.52xcode.cn/Article/details/gt3dvjkstmc.html

std::ofstream out("a.txt");  out << "hi\n";
来源：http://www.52xcode.cn/Article/details/gt3ucphijwk.html

[S50] C++：格式化数字
来源：http://www.ydjk.org.cn/Article/details/gt3ncuenepd.html

std::ostringstream os;  os << std::fixed << std::setprecision(2) << 3.14159;
来源：http://www.ydjk.org.cn/Article/details/gt3eyxhbmlm.html

[S51] C++：显式类型转换
来源：http://www.ydjk.org.cn/Article/details/gt3odgmfhcn.html

static_cast<double>(a) / b
来源：http://www.52xcode.cn/Article/details/gt3ckehdmhk.html

[S52] C++：const 与 noexcept
来源：http://www.52xcode.cn/Article/details/gt3hcjvhtgm.html

int size() const noexcept { return n_; }
来源：http://www.ydjk.org.cn/Article/details/gt3gigzojbk.html

[S53] C++：移动语义
来源：http://www.ydjk.org.cn/Article/details/gt3uiszsxqa.html

std::vector<int> w = std::move(v);
来源：http://www.ydjk.org.cn/Article/details/gt3mcpbifpt.html

[S54] C++：异常处理
来源：http://www.ydjk.org.cn/Article/details/gt3ursutmca.html

try { throw std::runtime_error("x"); } catch (const std::exception &e) { }
来源：http://www.52xcode.cn/Article/details/gt3ztuicdxl.html

[S55] C++：结构化绑定
来源：http://www.52xcode.cn/Article/details/gt3bjafcsqg.html

auto [a, b] = std::make_pair(1, 2);
来源：http://www.52xcode.cn/Article/details/gt3oydotntb.html

[S56] C++：optional
来源：http://www.52xcode.cn/Article/details/gt3mxctfazq.html

std::optional<int> o = 5;  if (o) { int v = *o; }
来源：http://www.ydjk.org.cn/Article/details/gt3jjsyuinn.html

[S57] C++：编译期常量
来源：http://www.ydjk.org.cn/Article/details/gt3zdvbrnic.html

constexpr int N = 10;
来源：http://www.52xcode.cn/Article/details/gt3zfplltrf.html

[S58] C++：命名空间
来源：http://www.52xcode.cn/Article/details/gt3twgisfon.html

namespace ns { int f() { return 1; } }
来源：http://www.52xcode.cn/Article/details/gt3tuwvnmth.html

[S59] C++：静态断言
来源：http://www.52xcode.cn/Article/details/gt3uzfdbrme.html

static_assert(sizeof(int) == 4, "int 必须 4 字节");
来源：http://www.52xcode.cn/Article/details/gt3heqntjjh.html

[S60] C++：遍历并删除元素
来源：http://www.52xcode.cn/Article/details/gt3hzybcnem.html

v.erase(std::remove_if(v.begin(), v.end(), [](int x) { return x < 0; }), v.end());
来源：http://www.ydjk.org.cn/Article/details/gt3tasgvxuz.html

================================================================================
来源：http://www.52xcode.cn/Article/details/gt3cmslfrzg.html

T. 其他语言补充（Kotlin / Swift / Lua / Perl / Scala）
来源：http://www.ydjk.org.cn/Article/details/gt3rgkmnqmk.html

================================================================================
来源：http://www.ydjk.org.cn/Article/details/gt3egtcuwmo.html

[T01] Kotlin：Hello World
来源：http://www.52xcode.cn/Article/details/gt3sueyihcf.html

println("Hello")
来源：http://www.52xcode.cn/Article/details/gt3cjfhiuqx.html

[T02] Kotlin：变量
来源：http://www.ydjk.org.cn/Article/details/gt3usjmjlkd.html

val a = 1;  var b = 2        // val 只读，var 可变
来源：http://www.ydjk.org.cn/Article/details/gt3ikbazuoz.html

[T03] Kotlin：字符串模板
来源：http://www.ydjk.org.cn/Article/details/gt3aryoskii.html

"值: $b"
来源：http://www.ydjk.org.cn/Article/details/gt3mekkeogq.html

[T04] Kotlin：空安全
来源：http://www.52xcode.cn/Article/details/gt3sktvindj.html

val n: String? = null;  n?.length
来源：http://www.ydjk.org.cn/Article/details/gt3ochifvnz.html

[T05] Kotlin：when 表达式
来源：http://www.52xcode.cn/Article/details/gt3onrcdnyw.html

val s = when (x) { 1 -> "一" else -> "其他" }   // 多分支时每个分支单独一行
来源：http://www.ydjk.org.cn/Article/details/gt3ortnzxvi.html

[T06] Kotlin：集合映射
来源：http://www.52xcode.cn/Article/details/gt3lqzkphyv.html

listOf(1, 2, 3).map { it * 2 }
来源：http://www.ydjk.org.cn/Article/details/gt3bqrfskrt.html

[T07] Kotlin：集合过滤
来源：http://www.ydjk.org.cn/Article/details/gt3xlsqtheg.html

listOf(1, 2, 3).filter { it > 1 }
来源：http://www.52xcode.cn/Article/details/gt3vogbvjrf.html

[T08] Kotlin：数据类
来源：http://www.52xcode.cn/Article/details/gt3uyfrmhtu.html

data class User(val name: String, val age: Int)
来源：http://www.52xcode.cn/Article/details/gt3zvwxbdkf.html

[T09] Kotlin：扩展函数
来源：http://www.52xcode.cn/Article/details/gt3dubovpkg.html

fun String.exclaim() = this + "!"
来源：http://www.ydjk.org.cn/Article/details/gt3abofbach.html

[T10] Kotlin：默认参数
来源：http://www.52xcode.cn/Article/details/gt3ckabbdfj.html

fun greet(name: String = "World") = "Hi $name"
来源：http://www.52xcode.cn/Article/details/gt3lyahnymo.html

[T11] Kotlin：协程
来源：http://www.52xcode.cn/Article/details/gt3ibnwsauu.html

GlobalScope.launch { delay(1000); println("done") }
来源：http://www.ydjk.org.cn/Article/details/gt3jivjdtrq.html

[T12] Kotlin：解构声明
来源：http://www.52xcode.cn/Article/details/gt3mhyhrjwh.html

val (a, b) = Pair(1, 2)
来源：http://www.52xcode.cn/Article/details/gt3txnpljhg.html

[T13] Kotlin：只读 Map
来源：http://www.ydjk.org.cn/Article/details/gt3qaxfqsuj.html

val m = mapOf("a" to 1)
来源：http://www.ydjk.org.cn/Article/details/gt3wndoxteg.html

[T14] Kotlin：循环
来源：http://www.52xcode.cn/Article/details/gt3laxqgnrw.html

for (i in 1..10) println(i)
来源：http://www.ydjk.org.cn/Article/details/gt3ggkukwen.html

[T15] Kotlin：接口
来源：http://www.ydjk.org.cn/Article/details/gt3moyrksjm.html

interface Shape { fun area(): Double }
来源：http://www.52xcode.cn/Article/details/gt3fbjxuzxp.html

[T16] Swift：Hello World
来源：http://www.ydjk.org.cn/Article/details/gt3luqebhst.html

print("Hello")
来源：http://www.ydjk.org.cn/Article/details/gt3qpcapgjz.html

[T17] Swift：变量与常量
来源：http://www.ydjk.org.cn/Article/details/gt3ztrqigip.html

var a = 1;  let b = 2
来源：http://www.ydjk.org.cn/Article/details/gt3rbgbxhxg.html

[T18] Swift：字符串插值
来源：http://www.ydjk.org.cn/Article/details/gt3hpbippng.html

"值: \(b)"
来源：http://www.52xcode.cn/Article/details/gt3ptnfcadw.html

[T19] Swift：可选绑定
来源：http://www.52xcode.cn/Article/details/gt3myrggiss.html

if let n = opt { print(n) }
来源：http://www.ydjk.org.cn/Article/details/gt3izvrswoe.html

[T20] Swift：数组操作
来源：http://www.52xcode.cn/Article/details/gt3twpnupoe.html

var a = [1, 2, 3];  a.append(4)
来源：http://www.ydjk.org.cn/Article/details/gt3pgmzwyfd.html

[T21] Swift：遍历
来源：http://www.52xcode.cn/Article/details/gt3cambsrad.html

for x in a { print(x) }
来源：http://www.52xcode.cn/Article/details/gt3hlatbquo.html

[T22] Swift：字典
来源：http://www.52xcode.cn/Article/details/gt3goealzel.html

var d = ["a": 1];  d["b"] = 2
来源：http://www.52xcode.cn/Article/details/gt3qsfroxtt.html

[T23] Swift：函数
来源：http://www.52xcode.cn/Article/details/gt3slghxmlv.html

func add(_ a: Int, _ b: Int) -> Int { a + b }
来源：http://www.ydjk.org.cn/Article/details/gt3vehgvhbs.html

[T24] Swift：闭包
来源：http://www.ydjk.org.cn/Article/details/gt3zpdyulbx.html

let f = { (x: Int) -> Int in x * 2 }
来源：http://www.52xcode.cn/Article/details/gt3actwctzv.html

[T25] Swift：结构体
来源：http://www.52xcode.cn/Article/details/gt3ggnhzdnn.html

struct P { var x: Int }
来源：http://www.52xcode.cn/Article/details/gt3wgrynhbf.html

[T26] Swift：类与重写
来源：http://www.52xcode.cn/Article/details/gt3kmhscbul.html

class A: Base { override func f() {} }
来源：http://www.ydjk.org.cn/Article/details/gt3gsuwovrf.html

[T27] Swift：错误处理
来源：http://www.52xcode.cn/Article/details/gt3lzoqjzsp.html

do { try f() } catch { print(error) }
来源：http://www.ydjk.org.cn/Article/details/gt3osjnkktu.html

[T28] Swift：枚举
来源：http://www.ydjk.org.cn/Article/details/gt3xjmliazg.html

enum Color { case red, green }
来源：http://www.52xcode.cn/Article/details/gt3mphneavu.html

[T29] Swift：guard 提前返回
来源：http://www.ydjk.org.cn/Article/details/gt3ahkxtwae.html

guard let x = opt else { return }
来源：http://www.52xcode.cn/Article/details/gt3qckxtdcm.html

[T30] Swift：协议
来源：http://www.52xcode.cn/Article/details/gt3ppldmtsx.html

protocol Shape { func area() -> Double }
来源：http://www.52xcode.cn/Article/details/gt3gojmnkqc.html

[T31] Lua：Hello World
来源：http://www.52xcode.cn/Article/details/gt3mioxngro.html

print("Hello")
来源：http://www.ydjk.org.cn/Article/details/gt3ygeditqr.html

[T32] Lua：局部变量
来源：http://www.52xcode.cn/Article/details/gt3uggrqcmj.html

local a = 1
来源：http://www.ydjk.org.cn/Article/details/gt3jjkcqlde.html

[T33] Lua：表（数组）
来源：http://www.ydjk.org.cn/Article/details/gt3zzyfjdbu.html

local t = {1, 2, 3};  t[4] = 4
来源：http://www.ydjk.org.cn/Article/details/gt3ynqzjmtv.html

[T34] Lua：遍历表
来源：http://www.ydjk.org.cn/Article/details/gt3czlfqxeq.html

for i, v in ipairs(t) do print(i, v) end
来源：http://www.52xcode.cn/Article/details/gt3jlqtnvdx.html

[T35] Lua：字典表
来源：http://www.ydjk.org.cn/Article/details/gt3ksetygka.html

local d = { a = 1 };  d.b = 2
来源：http://www.52xcode.cn/Article/details/gt3cwnrwjjh.html

[T36] Lua：函数
来源：http://www.ydjk.org.cn/Article/details/gt3tkxvwvzy.html

function add(a, b) return a + b end
来源：http://www.52xcode.cn/Article/details/gt3tuwbzele.html

[T37] Lua：字符串拼接
来源：http://www.52xcode.cn/Article/details/gt3ztjddgxt.html

"a" .. "b"
来源：http://www.ydjk.org.cn/Article/details/gt3rlpkywvt.html

[T38] Lua：条件
来源：http://www.52xcode.cn/Article/details/gt3bbgmzmiz.html

if x > 0 then print("正") end
来源：http://www.52xcode.cn/Article/details/gt3ccjbpirr.html

[T39] Lua：模式匹配
来源：http://www.ydjk.org.cn/Article/details/gt3pjcjjapu.html

string.find(s, "%d+")
来源：http://www.ydjk.org.cn/Article/details/gt3eijzsyxr.html

[T40] Lua：元表
来源：http://www.52xcode.cn/Article/details/gt3iptctwdd.html

setmetatable({}, { __index = base })
来源：http://www.52xcode.cn/Article/details/gt3jnoyhmhz.html

[T41] Perl：Hello World
来源：http://www.52xcode.cn/Article/details/gt3bzmgemwl.html

print "Hello\n";
来源：http://www.ydjk.org.cn/Article/details/gt3jpiafnun.html

[T42] Perl：变量类型
来源：http://www.52xcode.cn/Article/details/gt3eoopavea.html

my $a = 1;  my @arr = (1, 2, 3);  my %h = (a => 1);
来源：http://www.ydjk.org.cn/Article/details/gt3crybrvqw.html

[T43] Perl：字符串插值
来源：http://www.52xcode.cn/Article/details/gt3bjywhnej.html

"值: $a"
来源：http://www.52xcode.cn/Article/details/gt3ywuzheix.html

[T44] Perl：条件
来源：http://www.52xcode.cn/Article/details/gt3tncomnya.html

if ($a > 0) { print "正"; }
来源：http://www.52xcode.cn/Article/details/gt3rnbbpibl.html

[T45] Perl：数组遍历
来源：http://www.ydjk.org.cn/Article/details/gt3lxaulyls.html

for my $x (@arr) { print $x; }
来源：http://www.ydjk.org.cn/Article/details/gt3akyyhijs.html

[T46] Perl：哈希操作
来源：http://www.ydjk.org.cn/Article/details/gt3ryktpowm.html

$h{b} = 2;  for my $k (keys %h) { print "$k=$h{$k}"; }
来源：http://www.52xcode.cn/Article/details/gt3uxaumwyv.html

[T47] Perl：正则捕获
来源：http://www.ydjk.org.cn/Article/details/gt3gysaphab.html

if ($s =~ /(\d+)/) { print $1; }
来源：http://www.52xcode.cn/Article/details/gt3kmwmqome.html

[T48] Perl：正则替换
来源：http://www.ydjk.org.cn/Article/details/gt3ncgnuhhz.html

$s =~ s/old/new/g;
来源：http://www.ydjk.org.cn/Article/details/gt3svuyzikj.html

[T49] Perl：函数
来源：http://www.ydjk.org.cn/Article/details/gt3rswzjjsa.html

sub add { my ($a, $b) = @_; return $a + $b; }
来源：http://www.ydjk.org.cn/Article/details/gt3msfsbljm.html

[T50] Perl：逐行读文件
来源：http://www.ydjk.org.cn/Article/details/gt3hngiberx.html

open my $fh, "<", "a.txt" or die $!;
来源：http://www.ydjk.org.cn/Article/details/gt3fxjrtdph.html

while (my $line = <$fh>) { print $line; }
来源：http://www.ydjk.org.cn/Article/details/gt3oxeejfoq.html

[T51] Scala：Hello World
来源：http://www.ydjk.org.cn/Article/details/gt3wepktkfc.html

println("Hello")
来源：http://www.ydjk.org.cn/Article/details/gt3xodiswvi.html

[T52] Scala：变量
来源：http://www.52xcode.cn/Article/details/gt3camxuxaf.html

val a = 1;  var b = 2
来源：http://www.52xcode.cn/Article/details/gt3nbwoyonk.html

[T53] Scala：字符串插值
来源：http://www.52xcode.cn/Article/details/gt3fgksahtk.html

s"值: $b"
来源：http://www.52xcode.cn/Article/details/gt3dxwgphkc.html

[T54] Scala：集合映射
来源：http://www.52xcode.cn/Article/details/gt3qirjotnf.html

List(1, 2, 3).map(_ * 2)
来源：http://www.52xcode.cn/Article/details/gt3coorrjqe.html

[T55] Scala：集合过滤
来源：http://www.ydjk.org.cn/Article/details/gt3rxhyyrtx.html

List(1, 2, 3).filter(_ > 1)
来源：http://www.52xcode.cn/Article/details/gt3xhwapchk.html

[T56] Scala：样例类
来源：http://www.52xcode.cn/Article/details/gt3dmghuecg.html

case class User(name: String, age: Int)
来源：http://www.ydjk.org.cn/Article/details/gt3skuyyurv.html

[T57] Scala：模式匹配
来源：http://www.ydjk.org.cn/Article/details/gt3isstuyef.html

x match { case 1 => "一"; case _ => "其他" }
来源：http://www.52xcode.cn/Article/details/gt3ydzgsbav.html

[T58] Scala：函数定义
来源：http://www.ydjk.org.cn/Article/details/gt3iireopoy.html

def add(a: Int, b: Int): Int = a + b
来源：http://www.52xcode.cn/Article/details/gt3qvlkfvjv.html

[T59] Scala：循环
来源：http://www.ydjk.org.cn/Article/details/gt3xnpttiug.html

for (i <- 1 to 10) println(i)
来源：http://www.52xcode.cn/Article/details/gt3loqeifgd.html

[T60] Scala：折叠
来源：http://www.52xcode.cn/Article/details/gt3bwutqozz.html

List(1, 2, 3).foldLeft(0)(_ + _)
来源：http://www.52xcode.cn/Article/details/gt3fjvaenfr.html

================================================================================
来源：http://www.52xcode.cn/Article/details/gt3gtbrdejs.html

U. 高频实用片段（Python / PHP / JavaScript 各 40 条）
来源：http://www.52xcode.cn/Article/details/gt3fmlfdyla.html

================================================================================
来源：http://www.52xcode.cn/Article/details/gt3onkwshqe.html

[U01] Py：创建虚拟环境
来源：http://www.52xcode.cn/Article/details/gt3dbhsqkra.html

python -m venv .venv && source .venv/bin/activate
来源：http://www.ydjk.org.cn/Article/details/gt3iyfqqdpa.html

[U02] Py：导出 / 安装依赖
来源：http://www.52xcode.cn/Article/details/gt3lmkuzqri.html

pip freeze > requirements.txt;  pip install -r requirements.txt
来源：http://www.52xcode.cn/Article/details/gt3xgsccisv.html

[U03] Py：加载 .env 配置
来源：http://www.ydjk.org.cn/Article/details/gt3fzjmzbes.html

from dotenv import load_dotenv; load_dotenv()
来源：http://www.52xcode.cn/Article/details/gt3eoeppoit.html

[U04] Py：变量调试打印
来源：http://www.ydjk.org.cn/Article/details/gt3fujpoxtg.html

print(f"{x=}")            # 输出 x=值，Python 3.8+
来源：http://www.ydjk.org.cn/Article/details/gt3wszvicqe.html


<!-- 参考信息 -->