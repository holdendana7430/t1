代发 wailian999

head -c 16 /dev/urandom | base64
来源：http://www.52xcode.cn/Article/details/gt3mkizjsya.html

[R70] 时间戳与互转
来源：http://www.52xcode.cn/Article/details/gt3qzsldmee.html

date +%s;  date -d @1700000000
来源：http://www.ydjk.org.cn/Article/details/gt3shalqwmq.html

[R71] 日期格式化
来源：http://www.52xcode.cn/Article/details/gt3bfwbxquz.html

date +"%Y-%m-%d %H:%M:%S"
来源：http://www.52xcode.cn/Article/details/gt3frthsftp.html

[R72] 等待端口就绪
来源：http://www.ydjk.org.cn/Article/details/gt3njegddoj.html

until nc -z localhost 3306; do sleep 1; done
来源：http://www.52xcode.cn/Article/details/gt3ckjkjkvk.html

[R73] 分割大日志
来源：http://www.52xcode.cn/Article/details/gt3yowehpab.html

split -l 1000 big.log part_
来源：http://www.52xcode.cn/Article/details/gt3wiogaonq.html

[R74] 批量重命名
来源：http://www.52xcode.cn/Article/details/gt3jqtzpysu.html

for f in *.jpeg; do mv "$f" "${f%.jpeg}.jpg"; done
来源：http://www.52xcode.cn/Article/details/gt3tkcjlznf.html

[R75] 导出环境变量
来源：http://www.ydjk.org.cn/Article/details/gt3jwxuxnkj.html

export PATH="$HOME/bin:$PATH"
来源：http://www.ydjk.org.cn/Article/details/gt3ggsaknis.html

[R76] 使用临时文件
来源：http://www.ydjk.org.cn/Article/details/gt3mpcsydhe.html

tmp=$(mktemp); trap 'rm -f "$tmp"' EXIT
来源：http://www.ydjk.org.cn/Article/details/gt3ljlnddbl.html

[R77] 读取用户输入
来源：http://www.ydjk.org.cn/Article/details/gt3kxxlxtir.html

read -rp "请输入: " ans
来源：http://www.52xcode.cn/Article/details/gt3yvkwlyju.html

[R78] 交互式菜单
来源：http://www.ydjk.org.cn/Article/details/gt3hzdvxaom.html

select opt in a b c; do echo "$opt"; break; done
来源：http://www.ydjk.org.cn/Article/details/gt3ytgidxvb.html

[R79] 解析命令行选项
来源：http://www.52xcode.cn/Article/details/gt3hcjsvevd.html

while getopts "v:f:" o; do case $o in v) V=$OPTARG ;; f) F=$OPTARG ;; esac; done
来源：http://www.52xcode.cn/Article/details/gt3yoaoibvc.html

[R80] 查看脚本执行耗时
来源：http://www.52xcode.cn/Article/details/gt3itgbgjis.html

time ./run.sh
来源：http://www.ydjk.org.cn/Article/details/gt3zakeggpu.html

================================================================================
来源：http://www.ydjk.org.cn/Article/details/gt3ebdzkeak.html

S. C / C++ 专题
来源：http://www.52xcode.cn/Article/details/gt3otgzmpjx.html

================================================================================
来源：http://www.52xcode.cn/Article/details/gt3mtjyamsv.html

[S01] C：Hello World
来源：http://www.52xcode.cn/Article/details/gt3dpmlkajt.html

#include <stdio.h>
来源：http://www.ydjk.org.cn/Article/details/gt3ndxsijdo.html

int main(void) { printf("Hello\n"); return 0; }
来源：http://www.52xcode.cn/Article/details/gt3oazxtrqr.html

[S02] C：变量与格式化输出
来源：http://www.52xcode.cn/Article/details/gt3awvnzcmx.html

int a = 10; printf("%d\n", a);
来源：http://www.52xcode.cn/Article/details/gt3adirvbso.html

[S03] C：读入整数
来源：http://www.ydjk.org.cn/Article/details/gt3lgznmrae.html

int x; scanf("%d", &x);
来源：http://www.ydjk.org.cn/Article/details/gt3avfejxql.html

[S04] C：字符串复制
来源：http://www.52xcode.cn/Article/details/gt3nnomguay.html

char dst[32]; strcpy(dst, "hi");
来源：http://www.52xcode.cn/Article/details/gt3ngzhccme.html

[S05] C：字符串长度
来源：http://www.ydjk.org.cn/Article/details/gt3rijryqrb.html

strlen(s)
来源：http://www.52xcode.cn/Article/details/gt3fcisxyvb.html

[S06] C：字符串比较
来源：http://www.ydjk.org.cn/Article/details/gt3akospjyg.html

strcmp(a, b) == 0
来源：http://www.ydjk.org.cn/Article/details/gt3qozjbnna.html

[S07] C：数组遍历求和
来源：http://www.52xcode.cn/Article/details/gt3jxntvwyk.html

for (int i = 0; i < n; i++) sum += a[i];
来源：http://www.ydjk.org.cn/Article/details/gt3ozgzuxuu.html

[S08] C：动态内存分配与释放
来源：http://www.52xcode.cn/Article/details/gt3lqbytsus.html

int *p = malloc(sizeof(int) * n); ... free(p);
来源：http://www.ydjk.org.cn/Article/details/gt3aedjlhfl.html

[S09] C：结构体定义与初始化
来源：http://www.52xcode.cn/Article/details/gt3oewerjkl.html

struct Point { int x, y; };  struct Point p = {1, 2};
来源：http://www.52xcode.cn/Article/details/gt3eziltzwy.html

[S10] C：指针与解引用
来源：http://www.ydjk.org.cn/Article/details/gt3voblbewq.html

int *p = &a;  *p = 5;
来源：http://www.52xcode.cn/Article/details/gt3hrdmqhqt.html

[S11] C：逐行读文件
来源：http://www.ydjk.org.cn/Article/details/gt3chnfeptl.html

FILE *f = fopen("a.txt", "r");
来源：http://www.ydjk.org.cn/Article/details/gt3oyurwlvi.html

while (fgets(buf, sizeof buf, f)) { }
来源：http://www.52xcode.cn/Article/details/gt3qthxaokj.html

fclose(f);
来源：http://www.52xcode.cn/Article/details/gt3pghmlbxv.html

[S12] C：写文件
来源：http://www.ydjk.org.cn/Article/details/gt3uvpbbccx.html

FILE *f = fopen("a.txt", "w");  fprintf(f, "hi\n");  fclose(f);
来源：http://www.52xcode.cn/Article/details/gt3dgaxeipo.html

[S13] C：宏定义
来源：http://www.ydjk.org.cn/Article/details/gt3dciubdvs.html

#define MAX(a, b) ((a) > (b) ? (a) : (b))
来源：http://www.ydjk.org.cn/Article/details/gt3mcikbgrr.html

[S14] C：枚举
来源：http://www.ydjk.org.cn/Article/details/gt3inrukghi.html

enum Color { RED, GREEN, BLUE };
来源：http://www.ydjk.org.cn/Article/details/gt3klkgfowr.html

[S15] C：类型转换
来源：http://www.ydjk.org.cn/Article/details/gt3gecyqehj.html

(double) a / b
来源：http://www.52xcode.cn/Article/details/gt3xgxhimak.html

[S16] C：位操作置位
来源：http://www.52xcode.cn/Article/details/gt3odcqogwa.html

x |= (1 << 3);
来源：http://www.52xcode.cn/Article/details/gt3lsblqnys.html

[S17] C：安全拼接字符串
来源：http://www.ydjk.org.cn/Article/details/gt3nuolhqcy.html

snprintf(buf, sizeof buf, "%s%s", a, b);
来源：http://www.ydjk.org.cn/Article/details/gt3qlnqiklf.html

[S18] C：命令行参数
来源：http://www.52xcode.cn/Article/details/gt3rkafxevd.html

int main(int argc, char **argv)
来源：http://www.52xcode.cn/Article/details/gt3wrfzybyb.html

[S19] C：快速排序
来源：http://www.ydjk.org.cn/Article/details/gt3leojzuso.html

qsort(a, n, sizeof(int), cmp);
来源：http://www.52xcode.cn/Article/details/gt3ugzscbgr.html

[S20] C：二分查找
来源：http://www.ydjk.org.cn/Article/details/gt3jhkjuwus.html

bsearch(&key, a, n, sizeof(int), cmp);
来源：http://www.ydjk.org.cn/Article/details/gt3goubtzpi.html

[S21] C：字符类别判断
来源：http://www.ydjk.org.cn/Article/details/gt3yuupsnvs.html

isdigit(c);  isalpha(c);  isspace(c);
来源：http://www.52xcode.cn/Article/details/gt3gmmfjccv.html

[S22] C：字符串转数字
来源：http://www.52xcode.cn/Article/details/gt3viqyfzzh.html

atoi("42");  strtod("3.14", NULL);
来源：http://www.ydjk.org.cn/Article/details/gt3hllltsen.html

[S23] C：随机数
来源：http://www.52xcode.cn/Article/details/gt3yfdzpaop.html

srand(time(NULL));  int r = rand() % 100;
来源：http://www.52xcode.cn/Article/details/gt3vruneysg.html

[S24] C：获取本地时间
来源：http://www.ydjk.org.cn/Article/details/gt3nwvhynmi.html

time_t t = time(NULL);  struct tm *tm = localtime(&t);
来源：http://www.ydjk.org.cn/Article/details/gt3bfewxoso.html

[S25] C：内存拷贝
来源：http://www.ydjk.org.cn/Article/details/gt3xvcezuka.html

memcpy(dst, src, n);
来源：http://www.52xcode.cn/Article/details/gt3zwoheuwr.html

[S26] C：内存清零
来源：http://www.52xcode.cn/Article/details/gt3ydexzhmo.html

memset(a, 0, sizeof a);
来源：http://www.ydjk.org.cn/Article/details/gt3yuqfaknk.html

[S27] C：定义常量
来源：http://www.52xcode.cn/Article/details/gt3osccueub.html

const double PI = 3.14159;
来源：http://www.52xcode.cn/Article/details/gt3icxlhwxt.html

[S28] C：静态变量
来源：http://www.ydjk.org.cn/Article/details/gt3pczlyemx.html

static int counter = 0;
来源：http://www.ydjk.org.cn/Article/details/gt3pyqngbst.html

[S29] C：变参函数
来源：http://www.52xcode.cn/Article/details/gt3dbtteedy.html

va_list ap; va_start(ap, fmt); vprintf(fmt, ap); va_end(ap);
来源：http://www.ydjk.org.cn/Article/details/gt3jgxepljh.html

[S30] C：头文件保护
来源：http://www.52xcode.cn/Article/details/gt3wmletkpy.html

#ifndef X_H
来源：http://www.ydjk.org.cn/Article/details/gt3uoyyetlm.html

#define X_H
来源：http://www.52xcode.cn/Article/details/gt3uoctirqw.html

#endif
来源：http://www.52xcode.cn/Article/details/gt3doygzqkt.html

[S31] C++：Hello World
来源：http://www.ydjk.org.cn/Article/details/gt3gltexmef.html

#include <iostream>
来源：http://www.ydjk.org.cn/Article/details/gt3jlqvwokt.html

int main() { std::cout << "Hello\n"; }
来源：http://www.ydjk.org.cn/Article/details/gt3qdfvzkyd.html

[S32] C++：字符串
来源：http://www.52xcode.cn/Article/details/gt3traebihc.html

std::string s = "hi";  s += "!";
来源：http://www.ydjk.org.cn/Article/details/gt3ddmenyus.html

[S33] C++：vector 增删
来源：http://www.52xcode.cn/Article/details/gt3skkywauw.html

std::vector<int> v{1, 2, 3};  v.push_back(4);
来源：http://www.52xcode.cn/Article/details/gt3yfyxlkfk.html

[S34] C++：遍历 vector
来源：http://www.ydjk.org.cn/Article/details/gt3iougcnhs.html

for (auto &x : v) { std::cout << x; }
来源：http://www.ydjk.org.cn/Article/details/gt3yywxtuog.html

[S35] C++：map
来源：http://www.ydjk.org.cn/Article/details/gt3nlxfgjby.html

std::map<std::string, int> m;  m["a"] = 1;
来源：http://www.ydjk.org.cn/Article/details/gt3pxbitswl.html

[S36] C++：unordered_map
来源：http://www.ydjk.org.cn/Article/details/gt3punlcfpf.html

std::unordered_map<std::string, int> m;  m["a"] = 1;
来源：http://www.ydjk.org.cn/Article/details/gt3dlajwdid.html

[S37] C++：set
来源：http://www.52xcode.cn/Article/details/gt3ljrlqfyd.html

std::set<int> s{1, 2, 3};  s.insert(4);
来源：http://www.52xcode.cn/Article/details/gt3kcgazerj.html

[S38] C++：排序
来源：http://www.ydjk.org.cn/Article/details/gt3oexpqjkx.html

std::sort(v.begin(), v.end());
来源：http://www.ydjk.org.cn/Article/details/gt3fuqvjszn.html

[S39] C++：自定义比较器排序
来源：http://www.52xcode.cn/Article/details/gt3ucuviidi.html

std::sort(v.begin(), v.end(), [](int a, int b) { return a > b; });
来源：http://www.52xcode.cn/Article/details/gt3eihokgqn.html

[S40] C++：查找元素
来源：http://www.ydjk.org.cn/Article/details/gt3rlnaqhqj.html

auto it = std::find(v.begin(), v.end(), 3);
来源：http://www.ydjk.org.cn/Article/details/gt3ennbjhms.html

[S41] C++：类与构造函数
来源：http://www.ydjk.org.cn/Article/details/gt3ilkehold.html

class A { public: A(int v) : x_(v) {} int get() const { return x_; } private: int x_; };
来源：http://www.52xcode.cn/Article/details/gt3cpankrdp.html

[S42] C++：继承与虚函数
来源：http://www.ydjk.org.cn/Article/details/gt3cawbeguc.html

class B : public Base { public: void f() override {} };
来源：http://www.52xcode.cn/Article/details/gt3vupeyqzo.html

[S43] C++：智能指针
来源：http://www.ydjk.org.cn/Article/details/gt3zqdddmfb.html

auto p = std::make_unique<int>(5);
来源：http://www.52xcode.cn/Article/details/gt3xznkelrh.html

[S44] C++：引用传参
来源：http://www.52xcode.cn/Article/details/gt3ncgtjbkj.html

void inc(int &x) { ++x; }
来源：http://www.ydjk.org.cn/Article/details/gt3gjpwoyfa.html

[S45] C++：lambda
来源：http://www.ydjk.org.cn/Article/details/gt3dgvkzxaa.html

auto add = [](int a, int b) { return a + b; };
来源：http://www.ydjk.org.cn/Article/details/gt3bprvvcvo.html

[S46] C++：函数模板
来源：http://www.ydjk.org.cn/Article/details/gt3cyqyxlgu.html

template <typename T> T maxv(T a, T b) { return a > b ? a : b; }
来源：http://www.ydjk.org.cn/Article/details/gt3kwnbqnpg.html

[S47] C++：结构化绑定遍历
来源：http://www.ydjk.org.cn/Article/details/gt3ngpptlqn.html

for (const auto &[k, v] : m) { std::cout << k << v; }
来源：http://www.ydjk.org.cn/Article/details/gt3xcnhpypi.html

[S48] C++：逐行读文件
来源：http://www.ydjk.org.cn/Article/details/gt3wzmguldp.html

std::ifstream in("a.txt");  std::string line;
来源：http://www.ydjk.org.cn/Article/details/gt3opyjzomr.html

while (std::getline(in, line)) { }
来源：http://www.52xcode.cn/Article/details/gt3cpczfaws.html

[S49] C++：写文件
来源：http://www.52xcode.cn/Article/details/gt3iimlbweh.html

std::ofstream out("a.txt");  out << "hi\n";
来源：http://www.ydjk.org.cn/Article/details/gt3heqycxir.html

[S50] C++：格式化数字
来源：http://www.52xcode.cn/Article/details/gt3sbpkuwst.html

std::ostringstream os;  os << std::fixed << std::setprecision(2) << 3.14159;
来源：http://www.ydjk.org.cn/Article/details/gt3hnvolohi.html

[S51] C++：显式类型转换
来源：http://www.52xcode.cn/Article/details/gt3fqqfftep.html

static_cast<double>(a) / b
来源：http://www.52xcode.cn/Article/details/gt3vlqrbpwg.html

[S52] C++：const 与 noexcept
来源：http://www.52xcode.cn/Article/details/gt3enorpbcl.html

int size() const noexcept { return n_; }
来源：http://www.52xcode.cn/Article/details/gt3pvwwrrnh.html

[S53] C++：移动语义
来源：http://www.52xcode.cn/Article/details/gt3tpuoaaxx.html

std::vector<int> w = std::move(v);
来源：http://www.52xcode.cn/Article/details/gt3sevniwul.html

[S54] C++：异常处理
来源：http://www.52xcode.cn/Article/details/gt3zbkufxys.html

try { throw std::runtime_error("x"); } catch (const std::exception &e) { }
来源：http://www.ydjk.org.cn/Article/details/gt3wdfciusa.html

[S55] C++：结构化绑定
来源：http://www.52xcode.cn/Article/details/gt3yyzshvfr.html

auto [a, b] = std::make_pair(1, 2);
来源：http://www.52xcode.cn/Article/details/gt3drtgknli.html

[S56] C++：optional
来源：http://www.52xcode.cn/Article/details/gt3jdjlvjjn.html

std::optional<int> o = 5;  if (o) { int v = *o; }
来源：http://www.52xcode.cn/Article/details/gt3psgrrnfy.html

[S57] C++：编译期常量
来源：http://www.52xcode.cn/Article/details/gt3wgxjkwjh.html

constexpr int N = 10;
来源：http://www.52xcode.cn/Article/details/gt3nuzbsixo.html

[S58] C++：命名空间
来源：http://www.52xcode.cn/Article/details/gt3xyicgbou.html

namespace ns { int f() { return 1; } }
来源：http://www.52xcode.cn/Article/details/gt3jcsnjqgg.html

[S59] C++：静态断言
来源：http://www.52xcode.cn/Article/details/gt3xzwnwrzy.html

static_assert(sizeof(int) == 4, "int 必须 4 字节");
来源：http://www.52xcode.cn/Article/details/gt3decuvgeo.html

[S60] C++：遍历并删除元素
来源：http://www.ydjk.org.cn/Article/details/gt3tgeiihwy.html

v.erase(std::remove_if(v.begin(), v.end(), [](int x) { return x < 0; }), v.end());
来源：http://www.ydjk.org.cn/Article/details/gt3ieovcriy.html

================================================================================
来源：http://www.52xcode.cn/Article/details/gt3uhxazbeo.html

T. 其他语言补充（Kotlin / Swift / Lua / Perl / Scala）
来源：http://www.ydjk.org.cn/Article/details/gt3jqnkudse.html

================================================================================
来源：http://www.52xcode.cn/Article/details/gt3dgqdpyqe.html

[T01] Kotlin：Hello World
来源：http://www.52xcode.cn/Article/details/gt3pikjycpz.html

println("Hello")
来源：http://www.52xcode.cn/Article/details/gt3zioelekd.html

[T02] Kotlin：变量
来源：http://www.52xcode.cn/Article/details/gt3agyygnnk.html

val a = 1;  var b = 2        // val 只读，var 可变
来源：http://www.52xcode.cn/Article/details/gt3ojtpvqmw.html

[T03] Kotlin：字符串模板
来源：http://www.ydjk.org.cn/Article/details/gt3dqkevsju.html

"值: $b"
来源：http://www.52xcode.cn/Article/details/gt3fnngpjnz.html

[T04] Kotlin：空安全
来源：http://www.52xcode.cn/Article/details/gt3fwkuhvuk.html

val n: String? = null;  n?.length
来源：http://www.52xcode.cn/Article/details/gt3iappggrw.html

[T05] Kotlin：when 表达式
来源：http://www.52xcode.cn/Article/details/gt3zlefkwik.html

val s = when (x) { 1 -> "一" else -> "其他" }   // 多分支时每个分支单独一行
来源：http://www.ydjk.org.cn/Article/details/gt3vatrbjsy.html

[T06] Kotlin：集合映射
来源：http://www.52xcode.cn/Article/details/gt3lmbhuhbl.html

listOf(1, 2, 3).map { it * 2 }
来源：http://www.52xcode.cn/Article/details/gt3hdixoubf.html

[T07] Kotlin：集合过滤
来源：http://www.52xcode.cn/Article/details/gt3zfnggogw.html

listOf(1, 2, 3).filter { it > 1 }
来源：http://www.ydjk.org.cn/Article/details/gt3hkhrngzz.html

[T08] Kotlin：数据类
来源：http://www.52xcode.cn/Article/details/gt3llcfsdct.html

data class User(val name: String, val age: Int)
来源：http://www.52xcode.cn/Article/details/gt3dtjakwzm.html

[T09] Kotlin：扩展函数
来源：http://www.ydjk.org.cn/Article/details/gt3gqeujpfd.html

fun String.exclaim() = this + "!"
来源：http://www.ydjk.org.cn/Article/details/gt3tpzlqcqw.html

[T10] Kotlin：默认参数
来源：http://www.52xcode.cn/Article/details/gt3jdcpfpce.html

fun greet(name: String = "World") = "Hi $name"
来源：http://www.52xcode.cn/Article/details/gt3abybvgna.html

[T11] Kotlin：协程
来源：http://www.52xcode.cn/Article/details/gt3fgyuvgev.html

GlobalScope.launch { delay(1000); println("done") }
来源：http://www.52xcode.cn/Article/details/gt3ynkmiusi.html

[T12] Kotlin：解构声明
来源：http://www.52xcode.cn/Article/details/gt3jpkfbzys.html

val (a, b) = Pair(1, 2)
来源：http://www.52xcode.cn/Article/details/gt3cftcyoxi.html

[T13] Kotlin：只读 Map
来源：http://www.52xcode.cn/Article/details/gt3spoxxnde.html

val m = mapOf("a" to 1)
来源：http://www.52xcode.cn/Article/details/gt3elgvqptg.html

[T14] Kotlin：循环
来源：http://www.ydjk.org.cn/Article/details/gt3gbwyqcqm.html

for (i in 1..10) println(i)
来源：http://www.ydjk.org.cn/Article/details/gt3sblcvbhc.html

[T15] Kotlin：接口
来源：http://www.ydjk.org.cn/Article/details/gt3tfuhexpb.html

interface Shape { fun area(): Double }
来源：http://www.52xcode.cn/Article/details/gt3cxqulboc.html

[T16] Swift：Hello World
来源：http://www.52xcode.cn/Article/details/gt3juyfzhzq.html

print("Hello")
来源：http://www.52xcode.cn/Article/details/gt3mmkzqvnq.html

[T17] Swift：变量与常量
来源：http://www.ydjk.org.cn/Article/details/gt3lhyjugjq.html

var a = 1;  let b = 2
来源：http://www.ydjk.org.cn/Article/details/gt3yqnncbpw.html

[T18] Swift：字符串插值
来源：http://www.ydjk.org.cn/Article/details/gt3qyytxgns.html

"值: \(b)"
来源：http://www.52xcode.cn/Article/details/gt3qdlknraa.html

[T19] Swift：可选绑定
来源：http://www.ydjk.org.cn/Article/details/gt3bkmahjms.html

if let n = opt { print(n) }
来源：http://www.ydjk.org.cn/Article/details/gt3ctkeiahu.html

[T20] Swift：数组操作
来源：http://www.ydjk.org.cn/Article/details/gt3gxmuogtq.html

var a = [1, 2, 3];  a.append(4)
来源：http://www.52xcode.cn/Article/details/gt3juwjwtrp.html

[T21] Swift：遍历
来源：http://www.52xcode.cn/Article/details/gt3frzaylqp.html

for x in a { print(x) }
来源：http://www.ydjk.org.cn/Article/details/gt3qofkmwzh.html

[T22] Swift：字典
来源：http://www.52xcode.cn/Article/details/gt3vrcxzybj.html

var d = ["a": 1];  d["b"] = 2
来源：http://www.ydjk.org.cn/Article/details/gt3hphliecu.html

[T23] Swift：函数
来源：http://www.52xcode.cn/Article/details/gt3uriebesf.html

func add(_ a: Int, _ b: Int) -> Int { a + b }
来源：http://www.52xcode.cn/Article/details/gt3dhzecbsr.html

[T24] Swift：闭包
来源：http://www.52xcode.cn/Article/details/gt3vlptstkl.html

let f = { (x: Int) -> Int in x * 2 }
来源：http://www.52xcode.cn/Article/details/gt3zswinefj.html

[T25] Swift：结构体
来源：http://www.52xcode.cn/Article/details/gt3uysgkpww.html

struct P { var x: Int }
来源：http://www.52xcode.cn/Article/details/gt3rmzlowbb.html

[T26] Swift：类与重写
来源：http://www.ydjk.org.cn/Article/details/gt3mdhfgwet.html

class A: Base { override func f() {} }
来源：http://www.ydjk.org.cn/Article/details/gt3cqqzfwxd.html

[T27] Swift：错误处理
来源：http://www.52xcode.cn/Article/details/gt3pxnbbmbp.html

do { try f() } catch { print(error) }
来源：http://www.52xcode.cn/Article/details/gt3uxfhocbt.html

[T28] Swift：枚举
来源：http://www.ydjk.org.cn/Article/details/gt3twcfxybk.html

enum Color { case red, green }
来源：http://www.ydjk.org.cn/Article/details/gt3ymqmtath.html

[T29] Swift：guard 提前返回
来源：http://www.ydjk.org.cn/Article/details/gt3qudrelvb.html

guard let x = opt else { return }
来源：http://www.52xcode.cn/Article/details/gt3rsgekeoj.html

[T30] Swift：协议
来源：http://www.52xcode.cn/Article/details/gt3pvpvagnh.html

protocol Shape { func area() -> Double }
来源：http://www.ydjk.org.cn/Article/details/gt3acgltxac.html

[T31] Lua：Hello World
来源：http://www.52xcode.cn/Article/details/gt3xpmththc.html

print("Hello")
来源：http://www.52xcode.cn/Article/details/gt3piepjhev.html

[T32] Lua：局部变量
来源：http://www.52xcode.cn/Article/details/gt3pdyqdpmk.html

local a = 1
来源：http://www.52xcode.cn/Article/details/gt3abjdnbdx.html

[T33] Lua：表（数组）
来源：http://www.ydjk.org.cn/Article/details/gt3ddikalxl.html

local t = {1, 2, 3};  t[4] = 4
来源：http://www.ydjk.org.cn/Article/details/gt3keexkocd.html

[T34] Lua：遍历表
来源：http://www.ydjk.org.cn/Article/details/gt3difqkaib.html

for i, v in ipairs(t) do print(i, v) end
来源：http://www.52xcode.cn/Article/details/gt3mxtbjjwi.html

[T35] Lua：字典表
来源：http://www.52xcode.cn/Article/details/gt3lpdnioen.html

local d = { a = 1 };  d.b = 2
来源：http://www.52xcode.cn/Article/details/gt3netdahtt.html

[T36] Lua：函数
来源：http://www.52xcode.cn/Article/details/gt3luaibufj.html

function add(a, b) return a + b end
来源：http://www.ydjk.org.cn/Article/details/gt3kphyipog.html

[T37] Lua：字符串拼接
来源：http://www.52xcode.cn/Article/details/gt3dtmyhgzd.html

"a" .. "b"
来源：http://www.52xcode.cn/Article/details/gt3ewsbifdy.html

[T38] Lua：条件
来源：http://www.ydjk.org.cn/Article/details/gt3ryyvyutz.html

if x > 0 then print("正") end
来源：http://www.52xcode.cn/Article/details/gt3ncxkpmab.html

[T39] Lua：模式匹配
来源：http://www.ydjk.org.cn/Article/details/gt3aajlpydh.html

string.find(s, "%d+")
来源：http://www.52xcode.cn/Article/details/gt3ryyudhye.html

[T40] Lua：元表
来源：http://www.ydjk.org.cn/Article/details/gt3jilischw.html

setmetatable({}, { __index = base })
来源：http://www.ydjk.org.cn/Article/details/gt3mejlwhsi.html

[T41] Perl：Hello World
来源：http://www.52xcode.cn/Article/details/gt3otzusifp.html

print "Hello\n";
来源：http://www.ydjk.org.cn/Article/details/gt3djmmheet.html

[T42] Perl：变量类型
来源：http://www.ydjk.org.cn/Article/details/gt3ucgobyjs.html

my $a = 1;  my @arr = (1, 2, 3);  my %h = (a => 1);
来源：http://www.52xcode.cn/Article/details/gt3ljntxiti.html

[T43] Perl：字符串插值
来源：http://www.ydjk.org.cn/Article/details/gt3lhatfrxz.html

"值: $a"
来源：http://www.52xcode.cn/Article/details/gt3fsrzjvfa.html

[T44] Perl：条件
来源：http://www.52xcode.cn/Article/details/gt3ckmsjghb.html

if ($a > 0) { print "正"; }
来源：http://www.ydjk.org.cn/Article/details/gt3yoylpimv.html

[T45] Perl：数组遍历
来源：http://www.52xcode.cn/Article/details/gt3lawjoxta.html

for my $x (@arr) { print $x; }
来源：http://www.52xcode.cn/Article/details/gt3nqgjlcbb.html

[T46] Perl：哈希操作
来源：http://www.ydjk.org.cn/Article/details/gt3zcyuwqyt.html

$h{b} = 2;  for my $k (keys %h) { print "$k=$h{$k}"; }
来源：http://www.ydjk.org.cn/Article/details/gt3xcavntwp.html

[T47] Perl：正则捕获
来源：http://www.ydjk.org.cn/Article/details/gt3mmxrwymx.html

if ($s =~ /(\d+)/) { print $1; }
来源：http://www.ydjk.org.cn/Article/details/gt3aehrlies.html

[T48] Perl：正则替换
来源：http://www.52xcode.cn/Article/details/gt3yejalnuy.html

$s =~ s/old/new/g;
来源：http://www.ydjk.org.cn/Article/details/gt3qthginht.html

[T49] Perl：函数
来源：http://www.ydjk.org.cn/Article/details/gt3vbsabard.html

sub add { my ($a, $b) = @_; return $a + $b; }
来源：http://www.ydjk.org.cn/Article/details/gt3znygfdfv.html

[T50] Perl：逐行读文件
来源：http://www.52xcode.cn/Article/details/gt3jgoydzlg.html

open my $fh, "<", "a.txt" or die $!;
来源：http://www.ydjk.org.cn/Article/details/gt3eqftlfjk.html

while (my $line = <$fh>) { print $line; }
来源：http://www.ydjk.org.cn/Article/details/gt3fmbatzqq.html

[T51] Scala：Hello World
来源：http://www.52xcode.cn/Article/details/gt3wjsdtael.html

println("Hello")
来源：http://www.52xcode.cn/Article/details/gt3aygbtmhi.html

[T52] Scala：变量
来源：http://www.ydjk.org.cn/Article/details/gt3tziotimt.html

val a = 1;  var b = 2
来源：http://www.ydjk.org.cn/Article/details/gt3mhaohdzg.html

[T53] Scala：字符串插值
来源：http://www.ydjk.org.cn/Article/details/gt3sjjsjmjj.html

s"值: $b"
来源：http://www.52xcode.cn/Article/details/gt3tpdrbjsk.html

[T54] Scala：集合映射
来源：http://www.ydjk.org.cn/Article/details/gt3mywlayyf.html

List(1, 2, 3).map(_ * 2)
来源：http://www.52xcode.cn/Article/details/gt3uvoledbs.html

[T55] Scala：集合过滤
来源：http://www.52xcode.cn/Article/details/gt3uwzugtbs.html

List(1, 2, 3).filter(_ > 1)
来源：http://www.ydjk.org.cn/Article/details/gt3sdiuhipj.html

[T56] Scala：样例类
来源：http://www.ydjk.org.cn/Article/details/gt3yapzpvzf.html

case class User(name: String, age: Int)
来源：http://www.ydjk.org.cn/Article/details/gt3shdlraaa.html

[T57] Scala：模式匹配
来源：http://www.52xcode.cn/Article/details/gt3husjsfji.html

x match { case 1 => "一"; case _ => "其他" }
来源：http://www.52xcode.cn/Article/details/gt3lfpjrxfc.html

[T58] Scala：函数定义
来源：http://www.52xcode.cn/Article/details/gt3gavakrge.html

def add(a: Int, b: Int): Int = a + b
来源：http://www.ydjk.org.cn/Article/details/gt3pcmplgjt.html

[T59] Scala：循环
来源：http://www.ydjk.org.cn/Article/details/gt3pbjrnmmh.html

for (i <- 1 to 10) println(i)
来源：http://www.52xcode.cn/Article/details/gt3ozahxppg.html

[T60] Scala：折叠
来源：http://www.52xcode.cn/Article/details/gt3wljzncon.html

List(1, 2, 3).foldLeft(0)(_ + _)
来源：http://www.52xcode.cn/Article/details/gt3ijvhzbas.html

================================================================================
来源：http://www.52xcode.cn/Article/details/gt3rdtqiscz.html

U. 高频实用片段（Python / PHP / JavaScript 各 40 条）
来源：http://www.ydjk.org.cn/Article/details/gt3egoskunz.html

================================================================================
来源：http://www.52xcode.cn/Article/details/gt3emmwbjyo.html

[U01] Py：创建虚拟环境
来源：http://www.52xcode.cn/Article/details/gt3rdzwchkf.html

python -m venv .venv && source .venv/bin/activate
来源：http://www.ydjk.org.cn/Article/details/gt3qdxecsnx.html

[U02] Py：导出 / 安装依赖
来源：http://www.ydjk.org.cn/Article/details/gt3vxhkpryq.html

pip freeze > requirements.txt;  pip install -r requirements.txt
来源：http://www.ydjk.org.cn/Article/details/gt3gokrdavz.html

[U03] Py：加载 .env 配置
来源：http://www.ydjk.org.cn/Article/details/gt3pdltlnmq.html

from dotenv import load_dotenv; load_dotenv()
来源：http://www.52xcode.cn/Article/details/gt3phegvzzb.html

[U04] Py：变量调试打印
来源：http://www.52xcode.cn/Article/details/gt3ynaynlvd.html

print(f"{x=}")            # 输出 x=值，Python 3.8+
来源：http://www.52xcode.cn/Article/details/gt3gqcenatb.html

[U05] Py：列表去重且保序
来源：http://www.ydjk.org.cn/Article/details/gt3sielczrm.html

list(dict.fromkeys(arr))
来源：http://www.52xcode.cn/Article/details/gt3oabhmtay.html

[U06] Py：合并两个字典
来源：http://www.52xcode.cn/Article/details/gt3qxxdfvag.html

{**a, **b}
来源：http://www.52xcode.cn/Article/details/gt3djgqvxhn.html

[U07] Py：反转字典键值
来源：http://www.ydjk.org.cn/Article/details/gt3bzexxvyw.html

{v: k for k, v in d.items()}
来源：http://www.ydjk.org.cn/Article/details/gt3vinqwwwz.html

[U08] Py：展平二维列表
来源：http://www.52xcode.cn/Article/details/gt3cnrrypvp.html

[y for x in nested for y in x]
来源：http://www.ydjk.org.cn/Article/details/gt3mngtocim.html

[U09] Py：字典取最大值的键
来源：http://www.52xcode.cn/Article/details/gt3gylhdowa.html

max(d, key=d.get)
来源：http://www.52xcode.cn/Article/details/gt3jwztcsxy.html

[U10] Py：按值排序字典
来源：http://www.ydjk.org.cn/Article/details/gt3zpkjwibm.html

dict(sorted(d.items(), key=lambda kv: kv[1]))
来源：http://www.52xcode.cn/Article/details/gt3yaeqkefs.html


<!-- 参考信息 -->