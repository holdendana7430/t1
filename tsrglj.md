代发 wailian999

date +"%Y-%m-%d %H:%M:%S"
来源：http://www.ydjk.org.cn/Article/details/gt2mmolcgma.html

[R72] 等待端口就绪
来源：http://www.ydjk.org.cn/Article/details/gt2hddlbyyu.html

until nc -z localhost 3306; do sleep 1; done
来源：http://www.ydjk.org.cn/Article/details/gt2sspfjeqh.html

[R73] 分割大日志
来源：http://www.ydjk.org.cn/Article/details/gt2fnskcfvd.html

split -l 1000 big.log part_
来源：http://www.ydjk.org.cn/Article/details/gt2zbhmcxsg.html

[R74] 批量重命名
来源：http://www.ydjk.org.cn/Article/details/gt2ipvkfunc.html

for f in *.jpeg; do mv "$f" "${f%.jpeg}.jpg"; done
来源：http://www.52xcode.cn/Article/details/gt2ijnwmqlm.html

[R75] 导出环境变量
来源：http://www.ydjk.org.cn/Article/details/gt2psikbtej.html

export PATH="$HOME/bin:$PATH"
来源：http://www.ydjk.org.cn/Article/details/gt2czcbmldn.html

[R76] 使用临时文件
来源：http://www.52xcode.cn/Article/details/gt2zvjzgjrc.html

tmp=$(mktemp); trap 'rm -f "$tmp"' EXIT
来源：http://www.ydjk.org.cn/Article/details/gt2finwirnl.html

[R77] 读取用户输入
来源：http://www.ydjk.org.cn/Article/details/gt2agrxqtnc.html

read -rp "请输入: " ans
来源：http://www.ydjk.org.cn/Article/details/gt2xzzqsjmg.html

[R78] 交互式菜单
来源：http://www.52xcode.cn/Article/details/gt2jqbxialy.html

select opt in a b c; do echo "$opt"; break; done
来源：http://www.ydjk.org.cn/Article/details/gt2enjclbkb.html

[R79] 解析命令行选项
来源：http://www.52xcode.cn/Article/details/gt2tqhzmzdv.html

while getopts "v:f:" o; do case $o in v) V=$OPTARG ;; f) F=$OPTARG ;; esac; done
来源：http://www.52xcode.cn/Article/details/gt2bxhkreqh.html

[R80] 查看脚本执行耗时
来源：http://www.ydjk.org.cn/Article/details/gt2pazvwjqn.html

time ./run.sh
来源：http://www.52xcode.cn/Article/details/gt2dfcryogz.html

================================================================================
来源：http://www.ydjk.org.cn/Article/details/gt2jyyamnxu.html

S. C / C++ 专题
来源：http://www.ydjk.org.cn/Article/details/gt2rohffaki.html

================================================================================
来源：http://www.ydjk.org.cn/Article/details/gt2gtzjjcjg.html

[S01] C：Hello World
来源：http://www.52xcode.cn/Article/details/gt2tfievtwa.html

#include <stdio.h>
来源：http://www.52xcode.cn/Article/details/gt2ljvyaqrc.html

int main(void) { printf("Hello\n"); return 0; }
来源：http://www.52xcode.cn/Article/details/gt2oixlsvpz.html

[S02] C：变量与格式化输出
来源：http://www.ydjk.org.cn/Article/details/gt2ujfipgid.html

int a = 10; printf("%d\n", a);
来源：http://www.52xcode.cn/Article/details/gt2yzronwwn.html

[S03] C：读入整数
来源：http://www.52xcode.cn/Article/details/gt2kpzxhgdg.html

int x; scanf("%d", &x);
来源：http://www.ydjk.org.cn/Article/details/gt2zsoxyzux.html

[S04] C：字符串复制
来源：http://www.ydjk.org.cn/Article/details/gt2vpirninr.html

char dst[32]; strcpy(dst, "hi");
来源：http://www.52xcode.cn/Article/details/gt2dguotcdk.html

[S05] C：字符串长度
来源：http://www.ydjk.org.cn/Article/details/gt2upknmmub.html

strlen(s)
来源：http://www.ydjk.org.cn/Article/details/gt2dhjexiyj.html

[S06] C：字符串比较
来源：http://www.ydjk.org.cn/Article/details/gt2tnogssvk.html

strcmp(a, b) == 0
来源：http://www.52xcode.cn/Article/details/gt2kdcpceec.html

[S07] C：数组遍历求和
来源：http://www.ydjk.org.cn/Article/details/gt2ffvgvxyr.html

for (int i = 0; i < n; i++) sum += a[i];
来源：http://www.ydjk.org.cn/Article/details/gt2qbbiarjr.html

[S08] C：动态内存分配与释放
来源：http://www.52xcode.cn/Article/details/gt2mfizlfoi.html

int *p = malloc(sizeof(int) * n); ... free(p);
来源：http://www.ydjk.org.cn/Article/details/gt2pythrgwg.html

[S09] C：结构体定义与初始化
来源：http://www.52xcode.cn/Article/details/gt2kqnqqfie.html

struct Point { int x, y; };  struct Point p = {1, 2};
来源：http://www.ydjk.org.cn/Article/details/gt2esvasazi.html

[S10] C：指针与解引用
来源：http://www.52xcode.cn/Article/details/gt2sbeynycl.html

int *p = &a;  *p = 5;
来源：http://www.ydjk.org.cn/Article/details/gt2pdmgmekg.html

[S11] C：逐行读文件
来源：http://www.52xcode.cn/Article/details/gt2edabveam.html

FILE *f = fopen("a.txt", "r");
来源：http://www.ydjk.org.cn/Article/details/gt2paqhywfx.html

while (fgets(buf, sizeof buf, f)) { }
来源：http://www.ydjk.org.cn/Article/details/gt2bwxwinng.html

fclose(f);
来源：http://www.52xcode.cn/Article/details/gt2ilkjhkmx.html

[S12] C：写文件
来源：http://www.52xcode.cn/Article/details/gt2hyodiebr.html

FILE *f = fopen("a.txt", "w");  fprintf(f, "hi\n");  fclose(f);
来源：http://www.ydjk.org.cn/Article/details/gt2lcjkkzkq.html

[S13] C：宏定义
来源：http://www.ydjk.org.cn/Article/details/gt2ueyosumq.html

#define MAX(a, b) ((a) > (b) ? (a) : (b))
来源：http://www.52xcode.cn/Article/details/gt2ceojzxio.html

[S14] C：枚举
来源：http://www.ydjk.org.cn/Article/details/gt2qazhcayv.html

enum Color { RED, GREEN, BLUE };
来源：http://www.ydjk.org.cn/Article/details/gt2vmfgeqoe.html

[S15] C：类型转换
来源：http://www.ydjk.org.cn/Article/details/gt2tzgfavkx.html

(double) a / b
来源：http://www.ydjk.org.cn/Article/details/gt2vxbxvcwd.html

[S16] C：位操作置位
来源：http://www.ydjk.org.cn/Article/details/gt2lggzrink.html

x |= (1 << 3);
来源：http://www.52xcode.cn/Article/details/gt2vhxsufae.html

[S17] C：安全拼接字符串
来源：http://www.52xcode.cn/Article/details/gt2rszbqvns.html

snprintf(buf, sizeof buf, "%s%s", a, b);
来源：http://www.52xcode.cn/Article/details/gt2veggifmg.html

[S18] C：命令行参数
来源：http://www.52xcode.cn/Article/details/gt2wiuytpof.html

int main(int argc, char **argv)
来源：http://www.52xcode.cn/Article/details/gt2ovyhxsdd.html

[S19] C：快速排序
来源：http://www.52xcode.cn/Article/details/gt2dfirhdtx.html

qsort(a, n, sizeof(int), cmp);
来源：http://www.52xcode.cn/Article/details/gt2skjjditp.html

[S20] C：二分查找
来源：http://www.ydjk.org.cn/Article/details/gt2agpoxxps.html

bsearch(&key, a, n, sizeof(int), cmp);
来源：http://www.ydjk.org.cn/Article/details/gt2gflmkixv.html

[S21] C：字符类别判断
来源：http://www.52xcode.cn/Article/details/gt2swscywxd.html

isdigit(c);  isalpha(c);  isspace(c);
来源：http://www.52xcode.cn/Article/details/gt2lyheqlan.html

[S22] C：字符串转数字
来源：http://www.52xcode.cn/Article/details/gt2ywwvevzp.html

atoi("42");  strtod("3.14", NULL);
来源：http://www.ydjk.org.cn/Article/details/gt2ftpvdzod.html

[S23] C：随机数
来源：http://www.52xcode.cn/Article/details/gt2tlowbkhv.html

srand(time(NULL));  int r = rand() % 100;
来源：http://www.52xcode.cn/Article/details/gt2xyvlkiux.html

[S24] C：获取本地时间
来源：http://www.ydjk.org.cn/Article/details/gt2budlcwif.html

time_t t = time(NULL);  struct tm *tm = localtime(&t);
来源：http://www.ydjk.org.cn/Article/details/gt2fkvwsrhc.html

[S25] C：内存拷贝
来源：http://www.ydjk.org.cn/Article/details/gt2hralvjkh.html

memcpy(dst, src, n);
来源：http://www.ydjk.org.cn/Article/details/gt2wheouejw.html

[S26] C：内存清零
来源：http://www.ydjk.org.cn/Article/details/gt2suszklal.html

memset(a, 0, sizeof a);
来源：http://www.ydjk.org.cn/Article/details/gt2bgldrzec.html

[S27] C：定义常量
来源：http://www.ydjk.org.cn/Article/details/gt2whfhdkko.html

const double PI = 3.14159;
来源：http://www.52xcode.cn/Article/details/gt2nkyxbagd.html

[S28] C：静态变量
来源：http://www.ydjk.org.cn/Article/details/gt2opmfudfv.html

static int counter = 0;
来源：http://www.ydjk.org.cn/Article/details/gt2mthpmkbg.html

[S29] C：变参函数
来源：http://www.ydjk.org.cn/Article/details/gt2zhqerpob.html

va_list ap; va_start(ap, fmt); vprintf(fmt, ap); va_end(ap);
来源：http://www.52xcode.cn/Article/details/gt2dnlyhyaj.html

[S30] C：头文件保护
来源：http://www.52xcode.cn/Article/details/gt2phmodpbh.html

#ifndef X_H
来源：http://www.ydjk.org.cn/Article/details/gt2oyntaoap.html

#define X_H
来源：http://www.ydjk.org.cn/Article/details/gt2lbgfqgan.html

#endif
来源：http://www.ydjk.org.cn/Article/details/gt2atzmbiee.html

[S31] C++：Hello World
来源：http://www.52xcode.cn/Article/details/gt2ywiwdspy.html

#include <iostream>
来源：http://www.52xcode.cn/Article/details/gt2wmbahlpg.html

int main() { std::cout << "Hello\n"; }
来源：http://www.ydjk.org.cn/Article/details/gt2vqxyeely.html

[S32] C++：字符串
来源：http://www.ydjk.org.cn/Article/details/gt2rdktzprq.html

std::string s = "hi";  s += "!";
来源：http://www.52xcode.cn/Article/details/gt2sohftlqd.html

[S33] C++：vector 增删
来源：http://www.52xcode.cn/Article/details/gt2niqftsmk.html

std::vector<int> v{1, 2, 3};  v.push_back(4);
来源：http://www.ydjk.org.cn/Article/details/gt2esaxfduf.html

[S34] C++：遍历 vector
来源：http://www.52xcode.cn/Article/details/gt2kdfneaij.html

for (auto &x : v) { std::cout << x; }
来源：http://www.ydjk.org.cn/Article/details/gt2xhwkargu.html

[S35] C++：map
来源：http://www.ydjk.org.cn/Article/details/gt2arveebyp.html

std::map<std::string, int> m;  m["a"] = 1;
来源：http://www.52xcode.cn/Article/details/gt2llfwunfs.html

[S36] C++：unordered_map
来源：http://www.ydjk.org.cn/Article/details/gt2cbxpdvhi.html

std::unordered_map<std::string, int> m;  m["a"] = 1;
来源：http://www.52xcode.cn/Article/details/gt2deeuyzfo.html

[S37] C++：set
来源：http://www.52xcode.cn/Article/details/gt2okpdampt.html

std::set<int> s{1, 2, 3};  s.insert(4);
来源：http://www.ydjk.org.cn/Article/details/gt2garbybbf.html

[S38] C++：排序
来源：http://www.52xcode.cn/Article/details/gt2wrxzznhc.html

std::sort(v.begin(), v.end());
来源：http://www.52xcode.cn/Article/details/gt2onchvbmz.html

[S39] C++：自定义比较器排序
来源：http://www.ydjk.org.cn/Article/details/gt2xhzemwie.html

std::sort(v.begin(), v.end(), [](int a, int b) { return a > b; });
来源：http://www.52xcode.cn/Article/details/gt2neppemgf.html

[S40] C++：查找元素
来源：http://www.52xcode.cn/Article/details/gt2czernbtq.html

auto it = std::find(v.begin(), v.end(), 3);
来源：http://www.52xcode.cn/Article/details/gt2wyhmzddg.html

[S41] C++：类与构造函数
来源：http://www.52xcode.cn/Article/details/gt2hzkvlomn.html

class A { public: A(int v) : x_(v) {} int get() const { return x_; } private: int x_; };
来源：http://www.ydjk.org.cn/Article/details/gt2olvmpceq.html

[S42] C++：继承与虚函数
来源：http://www.ydjk.org.cn/Article/details/gt2hweyjses.html

class B : public Base { public: void f() override {} };
来源：http://www.ydjk.org.cn/Article/details/gt2nrttmrgl.html

[S43] C++：智能指针
来源：http://www.52xcode.cn/Article/details/gt2jzknvkvd.html

auto p = std::make_unique<int>(5);
来源：http://www.ydjk.org.cn/Article/details/gt2wriwptec.html

[S44] C++：引用传参
来源：http://www.ydjk.org.cn/Article/details/gt2iypihmdg.html

void inc(int &x) { ++x; }
来源：http://www.52xcode.cn/Article/details/gt2hvsaqgic.html

[S45] C++：lambda
来源：http://www.52xcode.cn/Article/details/gt2fwzjnoqb.html

auto add = [](int a, int b) { return a + b; };
来源：http://www.52xcode.cn/Article/details/gt2lkcacblv.html

[S46] C++：函数模板
来源：http://www.52xcode.cn/Article/details/gt2idoqtrrm.html

template <typename T> T maxv(T a, T b) { return a > b ? a : b; }
来源：http://www.ydjk.org.cn/Article/details/gt2eftlzkbr.html

[S47] C++：结构化绑定遍历
来源：http://www.ydjk.org.cn/Article/details/gt2ypkxwflm.html

for (const auto &[k, v] : m) { std::cout << k << v; }
来源：http://www.ydjk.org.cn/Article/details/gt2cbocsloe.html

[S48] C++：逐行读文件
来源：http://www.ydjk.org.cn/Article/details/gt2qnaxvzlp.html

std::ifstream in("a.txt");  std::string line;
来源：http://www.52xcode.cn/Article/details/gt2jsgetnzr.html

while (std::getline(in, line)) { }
来源：http://www.52xcode.cn/Article/details/gt2rbgzzdzf.html

[S49] C++：写文件
来源：http://www.ydjk.org.cn/Article/details/gt2vdyecest.html

std::ofstream out("a.txt");  out << "hi\n";
来源：http://www.52xcode.cn/Article/details/gt2jxqpsyhk.html

[S50] C++：格式化数字
来源：http://www.ydjk.org.cn/Article/details/gt2cjvccqgn.html

std::ostringstream os;  os << std::fixed << std::setprecision(2) << 3.14159;
来源：http://www.ydjk.org.cn/Article/details/gt2onrpqqzr.html

[S51] C++：显式类型转换
来源：http://www.ydjk.org.cn/Article/details/gt2hdasexjh.html

static_cast<double>(a) / b
来源：http://www.ydjk.org.cn/Article/details/gt2iblwaijd.html

[S52] C++：const 与 noexcept
来源：http://www.52xcode.cn/Article/details/gt2mluljqyd.html

int size() const noexcept { return n_; }
来源：http://www.52xcode.cn/Article/details/gt2krzovjcf.html

[S53] C++：移动语义
来源：http://www.ydjk.org.cn/Article/details/gt2dzdrllic.html

std::vector<int> w = std::move(v);
来源：http://www.ydjk.org.cn/Article/details/gt2akajgqcr.html

[S54] C++：异常处理
来源：http://www.52xcode.cn/Article/details/gt2klptryvw.html

try { throw std::runtime_error("x"); } catch (const std::exception &e) { }
来源：http://www.52xcode.cn/Article/details/gt2oujmkful.html

[S55] C++：结构化绑定
来源：http://www.52xcode.cn/Article/details/gt2hlhawfdn.html

auto [a, b] = std::make_pair(1, 2);
来源：http://www.ydjk.org.cn/Article/details/gt2pyqkwyva.html

[S56] C++：optional
来源：http://www.ydjk.org.cn/Article/details/gt2uhitiseq.html

std::optional<int> o = 5;  if (o) { int v = *o; }
来源：http://www.52xcode.cn/Article/details/gt2xnvtoehm.html

[S57] C++：编译期常量
来源：http://www.52xcode.cn/Article/details/gt2fcrwuled.html

constexpr int N = 10;
来源：http://www.ydjk.org.cn/Article/details/gt2pdfzfnkp.html

[S58] C++：命名空间
来源：http://www.52xcode.cn/Article/details/gt2fyhuscxt.html

namespace ns { int f() { return 1; } }
来源：http://www.52xcode.cn/Article/details/gt2ojhsjutx.html

[S59] C++：静态断言
来源：http://www.ydjk.org.cn/Article/details/gt2swftgzxb.html

static_assert(sizeof(int) == 4, "int 必须 4 字节");
来源：http://www.ydjk.org.cn/Article/details/gt2rjqngfqq.html

[S60] C++：遍历并删除元素
来源：http://www.ydjk.org.cn/Article/details/gt2mjgjepyw.html

v.erase(std::remove_if(v.begin(), v.end(), [](int x) { return x < 0; }), v.end());
来源：http://www.ydjk.org.cn/Article/details/gt2gbwzyhqp.html

================================================================================
来源：http://www.52xcode.cn/Article/details/gt2nrvflsfl.html

T. 其他语言补充（Kotlin / Swift / Lua / Perl / Scala）
来源：http://www.52xcode.cn/Article/details/gt2beraesli.html

================================================================================
来源：http://www.ydjk.org.cn/Article/details/gt2beggssnv.html

[T01] Kotlin：Hello World
来源：http://www.ydjk.org.cn/Article/details/gt2jpzoyuwe.html

println("Hello")
来源：http://www.52xcode.cn/Article/details/gt2hqgvrraj.html

[T02] Kotlin：变量
来源：http://www.ydjk.org.cn/Article/details/gt2gofhlqcj.html

val a = 1;  var b = 2        // val 只读，var 可变
来源：http://www.ydjk.org.cn/Article/details/gt2bomwwwzp.html

[T03] Kotlin：字符串模板
来源：http://www.52xcode.cn/Article/details/gt2ppectbmt.html

"值: $b"
来源：http://www.ydjk.org.cn/Article/details/gt2aaybonow.html

[T04] Kotlin：空安全
来源：http://www.ydjk.org.cn/Article/details/gt2jvgpxbcc.html

val n: String? = null;  n?.length
来源：http://www.52xcode.cn/Article/details/gt2rdfonily.html

[T05] Kotlin：when 表达式
来源：http://www.ydjk.org.cn/Article/details/gt2ydjqzrxm.html

val s = when (x) { 1 -> "一" else -> "其他" }   // 多分支时每个分支单独一行
来源：http://www.52xcode.cn/Article/details/gt2kkepaaoz.html

[T06] Kotlin：集合映射
来源：http://www.52xcode.cn/Article/details/gt2gqjfxjai.html

listOf(1, 2, 3).map { it * 2 }
来源：http://www.52xcode.cn/Article/details/gt2xwcscctm.html

[T07] Kotlin：集合过滤
来源：http://www.52xcode.cn/Article/details/gt2bxrtquih.html

listOf(1, 2, 3).filter { it > 1 }
来源：http://www.52xcode.cn/Article/details/gt2kzydgqxp.html

[T08] Kotlin：数据类
来源：http://www.ydjk.org.cn/Article/details/gt2ycugpemd.html

data class User(val name: String, val age: Int)
来源：http://www.52xcode.cn/Article/details/gt2mwqhqgdy.html

[T09] Kotlin：扩展函数
来源：http://www.52xcode.cn/Article/details/gt2caczhiea.html

fun String.exclaim() = this + "!"
来源：http://www.ydjk.org.cn/Article/details/gt2vtzabsaz.html

[T10] Kotlin：默认参数
来源：http://www.ydjk.org.cn/Article/details/gt2fmrsduzv.html

fun greet(name: String = "World") = "Hi $name"
来源：http://www.52xcode.cn/Article/details/gt2sabghkpy.html

[T11] Kotlin：协程
来源：http://www.ydjk.org.cn/Article/details/gt2ysjkmcyq.html

GlobalScope.launch { delay(1000); println("done") }
来源：http://www.ydjk.org.cn/Article/details/gt2riwdhqhk.html

[T12] Kotlin：解构声明
来源：http://www.ydjk.org.cn/Article/details/gt2khwmcopv.html

val (a, b) = Pair(1, 2)
来源：http://www.ydjk.org.cn/Article/details/gt2irjjoxqu.html

[T13] Kotlin：只读 Map
来源：http://www.ydjk.org.cn/Article/details/gt2nxeprvvi.html

val m = mapOf("a" to 1)
来源：http://www.52xcode.cn/Article/details/gt2ilivajeh.html

[T14] Kotlin：循环
来源：http://www.ydjk.org.cn/Article/details/gt2fvxmwwut.html

for (i in 1..10) println(i)
来源：http://www.52xcode.cn/Article/details/gt2jiaaaeer.html

[T15] Kotlin：接口
来源：http://www.ydjk.org.cn/Article/details/gt2qxivvbah.html

interface Shape { fun area(): Double }
来源：http://www.ydjk.org.cn/Article/details/gt2zrvydxqf.html

[T16] Swift：Hello World
来源：http://www.52xcode.cn/Article/details/gt2hrpgmufn.html

print("Hello")
来源：http://www.ydjk.org.cn/Article/details/gt2urjrntrk.html

[T17] Swift：变量与常量
来源：http://www.52xcode.cn/Article/details/gt2coayycol.html

var a = 1;  let b = 2
来源：http://www.52xcode.cn/Article/details/gt2irmfotkb.html

[T18] Swift：字符串插值
来源：http://www.52xcode.cn/Article/details/gt2zongqwvc.html

"值: \(b)"
来源：http://www.ydjk.org.cn/Article/details/gt2frdgrwfh.html

[T19] Swift：可选绑定
来源：http://www.52xcode.cn/Article/details/gt2fayxzzbq.html

if let n = opt { print(n) }
来源：http://www.ydjk.org.cn/Article/details/gt2ptjwouhb.html

[T20] Swift：数组操作
来源：http://www.ydjk.org.cn/Article/details/gt2ojgizgsf.html

var a = [1, 2, 3];  a.append(4)
来源：http://www.52xcode.cn/Article/details/gt2gncvlagu.html

[T21] Swift：遍历
来源：http://www.52xcode.cn/Article/details/gt2yzclbihy.html

for x in a { print(x) }
来源：http://www.ydjk.org.cn/Article/details/gt2fcuseksj.html

[T22] Swift：字典
来源：http://www.ydjk.org.cn/Article/details/gt2ylnvnclv.html

var d = ["a": 1];  d["b"] = 2
来源：http://www.ydjk.org.cn/Article/details/gt2mphjixdx.html

[T23] Swift：函数
来源：http://www.52xcode.cn/Article/details/gt2ykzslsbl.html

func add(_ a: Int, _ b: Int) -> Int { a + b }
来源：http://www.ydjk.org.cn/Article/details/gt2iojpkgrv.html

[T24] Swift：闭包
来源：http://www.ydjk.org.cn/Article/details/gt2gdoizysz.html

let f = { (x: Int) -> Int in x * 2 }
来源：http://www.52xcode.cn/Article/details/gt2nsjqonee.html

[T25] Swift：结构体
来源：http://www.ydjk.org.cn/Article/details/gt2xquazrgn.html

struct P { var x: Int }
来源：http://www.ydjk.org.cn/Article/details/gt2rnvtajdg.html

[T26] Swift：类与重写
来源：http://www.ydjk.org.cn/Article/details/gt2pbmjkoce.html

class A: Base { override func f() {} }
来源：http://www.ydjk.org.cn/Article/details/gt2xhhrasrq.html

[T27] Swift：错误处理
来源：http://www.ydjk.org.cn/Article/details/gt2sustvnoc.html

do { try f() } catch { print(error) }
来源：http://www.52xcode.cn/Article/details/gt2waaqvwrb.html

[T28] Swift：枚举
来源：http://www.52xcode.cn/Article/details/gt2jqfwtiov.html

enum Color { case red, green }
来源：http://www.52xcode.cn/Article/details/gt2esilpcnf.html

[T29] Swift：guard 提前返回
来源：http://www.ydjk.org.cn/Article/details/gt2xbljdvfa.html

guard let x = opt else { return }
来源：http://www.ydjk.org.cn/Article/details/gt2caflnrcu.html

[T30] Swift：协议
来源：http://www.ydjk.org.cn/Article/details/gt2ajgxrzle.html

protocol Shape { func area() -> Double }
来源：http://www.52xcode.cn/Article/details/gt2lwuzwfdl.html

[T31] Lua：Hello World
来源：http://www.ydjk.org.cn/Article/details/gt2eickcefi.html

print("Hello")
来源：http://www.52xcode.cn/Article/details/gt2mxiushet.html

[T32] Lua：局部变量
来源：http://www.ydjk.org.cn/Article/details/gt2yoxldqnx.html

local a = 1
来源：http://www.52xcode.cn/Article/details/gt2ndesrtyy.html

[T33] Lua：表（数组）
来源：http://www.ydjk.org.cn/Article/details/gt2ydyfhokj.html

local t = {1, 2, 3};  t[4] = 4
来源：http://www.52xcode.cn/Article/details/gt2nymqezts.html

[T34] Lua：遍历表
来源：http://www.52xcode.cn/Article/details/gt2ycpgitzr.html

for i, v in ipairs(t) do print(i, v) end
来源：http://www.ydjk.org.cn/Article/details/gt2pztwpdwt.html

[T35] Lua：字典表
来源：http://www.ydjk.org.cn/Article/details/gt2fjeqihbr.html

local d = { a = 1 };  d.b = 2
来源：http://www.52xcode.cn/Article/details/gt2fubqdkpb.html

[T36] Lua：函数
来源：http://www.ydjk.org.cn/Article/details/gt2whurzuml.html

function add(a, b) return a + b end
来源：http://www.ydjk.org.cn/Article/details/gt2hlewgady.html

[T37] Lua：字符串拼接
来源：http://www.ydjk.org.cn/Article/details/gt2sfazjcom.html

"a" .. "b"
来源：http://www.52xcode.cn/Article/details/gt2kgikkotr.html

[T38] Lua：条件
来源：http://www.52xcode.cn/Article/details/gt2rmjgbomy.html

if x > 0 then print("正") end
来源：http://www.ydjk.org.cn/Article/details/gt2gcxyglvh.html

[T39] Lua：模式匹配
来源：http://www.52xcode.cn/Article/details/gt2fjcskjwd.html

string.find(s, "%d+")
来源：http://www.ydjk.org.cn/Article/details/gt2kqibztqk.html

[T40] Lua：元表
来源：http://www.ydjk.org.cn/Article/details/gt2sobjkaor.html

setmetatable({}, { __index = base })
来源：http://www.52xcode.cn/Article/details/gt2jznknhak.html

[T41] Perl：Hello World
来源：http://www.52xcode.cn/Article/details/gt2hgrqkscm.html

print "Hello\n";
来源：http://www.52xcode.cn/Article/details/gt2ibthorqx.html

[T42] Perl：变量类型
来源：http://www.52xcode.cn/Article/details/gt2iliyjnig.html

my $a = 1;  my @arr = (1, 2, 3);  my %h = (a => 1);
来源：http://www.52xcode.cn/Article/details/gt2syiyyijt.html

[T43] Perl：字符串插值
来源：http://www.ydjk.org.cn/Article/details/gt2mgvujdig.html

"值: $a"
来源：http://www.ydjk.org.cn/Article/details/gt2gvmyfkjv.html

[T44] Perl：条件
来源：http://www.52xcode.cn/Article/details/gt2pyacnyrv.html

if ($a > 0) { print "正"; }
来源：http://www.ydjk.org.cn/Article/details/gt2cmptmojs.html

[T45] Perl：数组遍历
来源：http://www.52xcode.cn/Article/details/gt2burgdrhs.html

for my $x (@arr) { print $x; }
来源：http://www.ydjk.org.cn/Article/details/gt2jpozqbyk.html

[T46] Perl：哈希操作
来源：http://www.ydjk.org.cn/Article/details/gt2dwsutpzw.html

$h{b} = 2;  for my $k (keys %h) { print "$k=$h{$k}"; }
来源：http://www.52xcode.cn/Article/details/gt2glakrucm.html

[T47] Perl：正则捕获
来源：http://www.52xcode.cn/Article/details/gt2jpxfwhrb.html

if ($s =~ /(\d+)/) { print $1; }
来源：http://www.52xcode.cn/Article/details/gt2ggwrdorc.html

[T48] Perl：正则替换
来源：http://www.52xcode.cn/Article/details/gt2ihuljwbc.html

$s =~ s/old/new/g;
来源：http://www.ydjk.org.cn/Article/details/gt2olrfximr.html

[T49] Perl：函数
来源：http://www.ydjk.org.cn/Article/details/gt2rwlawimj.html

sub add { my ($a, $b) = @_; return $a + $b; }
来源：http://www.ydjk.org.cn/Article/details/gt2zdhhmuth.html

[T50] Perl：逐行读文件
来源：http://www.52xcode.cn/Article/details/gt2ksxwkkxl.html

open my $fh, "<", "a.txt" or die $!;
来源：http://www.52xcode.cn/Article/details/gt2vuqpqrkf.html

while (my $line = <$fh>) { print $line; }
来源：http://www.52xcode.cn/Article/details/gt2tcbnpdbr.html

[T51] Scala：Hello World
来源：http://www.52xcode.cn/Article/details/gt2srhkdqyd.html

println("Hello")
来源：http://www.52xcode.cn/Article/details/gt2deagnxao.html

[T52] Scala：变量
来源：http://www.52xcode.cn/Article/details/gt2nvjacxls.html

val a = 1;  var b = 2
来源：http://www.52xcode.cn/Article/details/gt2zlceodgv.html

[T53] Scala：字符串插值
来源：http://www.52xcode.cn/Article/details/gt2mnbjqxov.html

s"值: $b"
来源：http://www.ydjk.org.cn/Article/details/gt2glhkutsw.html

[T54] Scala：集合映射
来源：http://www.52xcode.cn/Article/details/gt2mztxayfu.html

List(1, 2, 3).map(_ * 2)
来源：http://www.52xcode.cn/Article/details/gt2vuvgqzir.html

[T55] Scala：集合过滤
来源：http://www.ydjk.org.cn/Article/details/gt2zgmhzynh.html

List(1, 2, 3).filter(_ > 1)
来源：http://www.ydjk.org.cn/Article/details/gt2bwwoypeo.html

[T56] Scala：样例类
来源：http://www.52xcode.cn/Article/details/gt2aqfwnvgj.html

case class User(name: String, age: Int)
来源：http://www.52xcode.cn/Article/details/gt2wlpeassq.html

[T57] Scala：模式匹配
来源：http://www.52xcode.cn/Article/details/gt2yyiwukyj.html

x match { case 1 => "一"; case _ => "其他" }
来源：http://www.52xcode.cn/Article/details/gt2uieoszup.html

[T58] Scala：函数定义
来源：http://www.ydjk.org.cn/Article/details/gt2pcwzlbkm.html

def add(a: Int, b: Int): Int = a + b
来源：http://www.52xcode.cn/Article/details/gt2dyfwrumg.html

[T59] Scala：循环
来源：http://www.52xcode.cn/Article/details/gt2ywezoxxp.html

for (i <- 1 to 10) println(i)
来源：http://www.ydjk.org.cn/Article/details/gt2dwjvedne.html

[T60] Scala：折叠
来源：http://www.ydjk.org.cn/Article/details/gt2boqdzhrb.html

List(1, 2, 3).foldLeft(0)(_ + _)
来源：http://www.ydjk.org.cn/Article/details/gt2ydhmfrod.html

================================================================================
来源：http://www.ydjk.org.cn/Article/details/gt2fevdtvij.html

U. 高频实用片段（Python / PHP / JavaScript 各 40 条）
来源：http://www.52xcode.cn/Article/details/gt2lwkgskiq.html

================================================================================
来源：http://www.ydjk.org.cn/Article/details/gt2fawasbgt.html

[U01] Py：创建虚拟环境
来源：http://www.52xcode.cn/Article/details/gt2vjdytbka.html

python -m venv .venv && source .venv/bin/activate
来源：http://www.ydjk.org.cn/Article/details/gt2whhzccui.html

[U02] Py：导出 / 安装依赖
来源：http://www.52xcode.cn/Article/details/gt2lnzigozz.html

pip freeze > requirements.txt;  pip install -r requirements.txt
来源：http://www.ydjk.org.cn/Article/details/gt2sowsbpzf.html

[U03] Py：加载 .env 配置
来源：http://www.ydjk.org.cn/Article/details/gt2ilnloeih.html

from dotenv import load_dotenv; load_dotenv()
来源：http://www.ydjk.org.cn/Article/details/gt2qijuzjnj.html

[U04] Py：变量调试打印
来源：http://www.ydjk.org.cn/Article/details/gt2uavfftdk.html

print(f"{x=}")            # 输出 x=值，Python 3.8+
来源：http://www.ydjk.org.cn/Article/details/gt2dscferfa.html

[U05] Py：列表去重且保序
来源：http://www.52xcode.cn/Article/details/gt2qvikysmt.html

list(dict.fromkeys(arr))
来源：http://www.ydjk.org.cn/Article/details/gt2nzhogizp.html

[U06] Py：合并两个字典
来源：http://www.52xcode.cn/Article/details/gt2nlkawpoy.html

{**a, **b}
来源：http://www.52xcode.cn/Article/details/gt2qtkqvfpi.html

[U07] Py：反转字典键值
来源：http://www.ydjk.org.cn/Article/details/gt2wdkzrxyk.html

{v: k for k, v in d.items()}
来源：http://www.52xcode.cn/Article/details/gt2tnmpeadn.html

[U08] Py：展平二维列表
来源：http://www.ydjk.org.cn/Article/details/gt2lspnjnoe.html

[y for x in nested for y in x]
来源：http://www.ydjk.org.cn/Article/details/gt2ahgaesug.html

[U09] Py：字典取最大值的键
来源：http://www.ydjk.org.cn/Article/details/gt2yecqxlmm.html

max(d, key=d.get)
来源：http://www.52xcode.cn/Article/details/gt2giaqbwwv.html

[U10] Py：按值排序字典
来源：http://www.52xcode.cn/Article/details/gt2cplzidpn.html

dict(sorted(d.items(), key=lambda kv: kv[1]))
来源：http://www.ydjk.org.cn/Article/details/gt2qrocgniv.html

[U11] Py：生成器表达式
来源：http://www.52xcode.cn/Article/details/gt2czgsiqwi.html

(x * 2 for x in arr)
来源：http://www.ydjk.org.cn/Article/details/gt2rtdqxkuk.html

[U12] Py：取出现最多的 3 个元素
来源：http://www.52xcode.cn/Article/details/gt2xdgxfzjh.html

Counter(arr).most_common(3)
来源：http://www.52xcode.cn/Article/details/gt2ywtxgluj.html


<!-- 参考信息 -->