代发 wailian999

head -c 16 /dev/urandom | base64
来源：http://www.ydjk.org.cn/Article/details/gt3btqbjyhp.html

[R70] 时间戳与互转
来源：http://www.ydjk.org.cn/Article/details/gt3ecleoetn.html

date +%s;  date -d @1700000000
来源：http://www.ydjk.org.cn/Article/details/gt3fyysrhll.html

[R71] 日期格式化
来源：http://www.ydjk.org.cn/Article/details/gt3jbocilhu.html

date +"%Y-%m-%d %H:%M:%S"
来源：http://www.ydjk.org.cn/Article/details/gt3dwflwozv.html

[R72] 等待端口就绪
来源：http://www.52xcode.cn/Article/details/gt3jzvwczsl.html

until nc -z localhost 3306; do sleep 1; done
来源：http://www.ydjk.org.cn/Article/details/gt3cjtwzeid.html

[R73] 分割大日志
来源：http://www.52xcode.cn/Article/details/gt3ydxzaidb.html

split -l 1000 big.log part_
来源：http://www.52xcode.cn/Article/details/gt3ixqnltqt.html

[R74] 批量重命名
来源：http://www.52xcode.cn/Article/details/gt3zkdctadb.html

for f in *.jpeg; do mv "$f" "${f%.jpeg}.jpg"; done
来源：http://www.ydjk.org.cn/Article/details/gt3bflciosv.html

[R75] 导出环境变量
来源：http://www.ydjk.org.cn/Article/details/gt3mtmksnry.html

export PATH="$HOME/bin:$PATH"
来源：http://www.ydjk.org.cn/Article/details/gt3ajdkytqw.html

[R76] 使用临时文件
来源：http://www.52xcode.cn/Article/details/gt3snxfmivg.html

tmp=$(mktemp); trap 'rm -f "$tmp"' EXIT
来源：http://www.52xcode.cn/Article/details/gt3fxazgsbj.html

[R77] 读取用户输入
来源：http://www.52xcode.cn/Article/details/gt3zepfpaxo.html

read -rp "请输入: " ans
来源：http://www.ydjk.org.cn/Article/details/gt3qlxsjzqh.html

[R78] 交互式菜单
来源：http://www.52xcode.cn/Article/details/gt3ghpeakya.html

select opt in a b c; do echo "$opt"; break; done
来源：http://www.52xcode.cn/Article/details/gt3ivkfyloe.html

[R79] 解析命令行选项
来源：http://www.52xcode.cn/Article/details/gt3kbquenpj.html

while getopts "v:f:" o; do case $o in v) V=$OPTARG ;; f) F=$OPTARG ;; esac; done
来源：http://www.ydjk.org.cn/Article/details/gt3zwqokdyu.html

[R80] 查看脚本执行耗时
来源：http://www.ydjk.org.cn/Article/details/gt3ajdrdumf.html

time ./run.sh
来源：http://www.ydjk.org.cn/Article/details/gt3dbhauahc.html

================================================================================
来源：http://www.52xcode.cn/Article/details/gt3vwrjvwvl.html

S. C / C++ 专题
来源：http://www.ydjk.org.cn/Article/details/gt3nwkhtlis.html

================================================================================
来源：http://www.ydjk.org.cn/Article/details/gt3bwomgdfd.html

[S01] C：Hello World
来源：http://www.ydjk.org.cn/Article/details/gt3zfkahoxv.html

#include <stdio.h>
来源：http://www.ydjk.org.cn/Article/details/gt3eembeuqo.html

int main(void) { printf("Hello\n"); return 0; }
来源：http://www.ydjk.org.cn/Article/details/gt3bzsfooia.html

[S02] C：变量与格式化输出
来源：http://www.52xcode.cn/Article/details/gt3kfhlaloc.html

int a = 10; printf("%d\n", a);
来源：http://www.ydjk.org.cn/Article/details/gt3xufahyjc.html

[S03] C：读入整数
来源：http://www.ydjk.org.cn/Article/details/gt3pqbdifxl.html

int x; scanf("%d", &x);
来源：http://www.ydjk.org.cn/Article/details/gt3ojrbduvi.html

[S04] C：字符串复制
来源：http://www.52xcode.cn/Article/details/gt3ixajeiic.html

char dst[32]; strcpy(dst, "hi");
来源：http://www.ydjk.org.cn/Article/details/gt3jazafhfj.html

[S05] C：字符串长度
来源：http://www.52xcode.cn/Article/details/gt3kvgukpxk.html

strlen(s)
来源：http://www.52xcode.cn/Article/details/gt3mldmlyys.html

[S06] C：字符串比较
来源：http://www.52xcode.cn/Article/details/gt3uljgklce.html

strcmp(a, b) == 0
来源：http://www.52xcode.cn/Article/details/gt3ngmtxzhd.html

[S07] C：数组遍历求和
来源：http://www.52xcode.cn/Article/details/gt3kcjsjqpg.html

for (int i = 0; i < n; i++) sum += a[i];
来源：http://www.ydjk.org.cn/Article/details/gt3bzceawsh.html

[S08] C：动态内存分配与释放
来源：http://www.52xcode.cn/Article/details/gt3luwnkque.html

int *p = malloc(sizeof(int) * n); ... free(p);
来源：http://www.ydjk.org.cn/Article/details/gt3lxbnbtjv.html

[S09] C：结构体定义与初始化
来源：http://www.52xcode.cn/Article/details/gt3hzqfcliw.html

struct Point { int x, y; };  struct Point p = {1, 2};
来源：http://www.ydjk.org.cn/Article/details/gt3nvvzygcd.html

[S10] C：指针与解引用
来源：http://www.52xcode.cn/Article/details/gt3wcevaxgp.html

int *p = &a;  *p = 5;
来源：http://www.52xcode.cn/Article/details/gt3wbyiogxf.html

[S11] C：逐行读文件
来源：http://www.52xcode.cn/Article/details/gt3qmixkfma.html

FILE *f = fopen("a.txt", "r");
来源：http://www.ydjk.org.cn/Article/details/gt3mnjfhvqm.html

while (fgets(buf, sizeof buf, f)) { }
来源：http://www.52xcode.cn/Article/details/gt3rkbyuwfw.html

fclose(f);
来源：http://www.52xcode.cn/Article/details/gt3gthjqyoa.html

[S12] C：写文件
来源：http://www.ydjk.org.cn/Article/details/gt3edwwrdor.html

FILE *f = fopen("a.txt", "w");  fprintf(f, "hi\n");  fclose(f);
来源：http://www.52xcode.cn/Article/details/gt3aweuhtua.html

[S13] C：宏定义
来源：http://www.ydjk.org.cn/Article/details/gt3uqijxnqv.html

#define MAX(a, b) ((a) > (b) ? (a) : (b))
来源：http://www.52xcode.cn/Article/details/gt3jhmuckgd.html

[S14] C：枚举
来源：http://www.ydjk.org.cn/Article/details/gt3jtkjmgpw.html

enum Color { RED, GREEN, BLUE };
来源：http://www.ydjk.org.cn/Article/details/gt3rejlkhiv.html

[S15] C：类型转换
来源：http://www.ydjk.org.cn/Article/details/gt3ezdsudru.html

(double) a / b
来源：http://www.52xcode.cn/Article/details/gt3cckkowjs.html

[S16] C：位操作置位
来源：http://www.52xcode.cn/Article/details/gt3aaadczqf.html

x |= (1 << 3);
来源：http://www.52xcode.cn/Article/details/gt3qyfmbxqc.html

[S17] C：安全拼接字符串
来源：http://www.ydjk.org.cn/Article/details/gt3cckcjjxg.html

snprintf(buf, sizeof buf, "%s%s", a, b);
来源：http://www.52xcode.cn/Article/details/gt3qjrcbgxw.html

[S18] C：命令行参数
来源：http://www.ydjk.org.cn/Article/details/gt3euzzgasy.html

int main(int argc, char **argv)
来源：http://www.ydjk.org.cn/Article/details/gt3gyoaflyt.html

[S19] C：快速排序
来源：http://www.ydjk.org.cn/Article/details/gt3omtoscxf.html

qsort(a, n, sizeof(int), cmp);
来源：http://www.ydjk.org.cn/Article/details/gt3hmjgrbly.html

[S20] C：二分查找
来源：http://www.52xcode.cn/Article/details/gt3bjvgcpin.html

bsearch(&key, a, n, sizeof(int), cmp);
来源：http://www.52xcode.cn/Article/details/gt3umsnsaac.html

[S21] C：字符类别判断
来源：http://www.52xcode.cn/Article/details/gt3whvkgtyx.html

isdigit(c);  isalpha(c);  isspace(c);
来源：http://www.52xcode.cn/Article/details/gt3diudmker.html

[S22] C：字符串转数字
来源：http://www.ydjk.org.cn/Article/details/gt3expskwlu.html

atoi("42");  strtod("3.14", NULL);
来源：http://www.ydjk.org.cn/Article/details/gt3pvyjavbw.html

[S23] C：随机数
来源：http://www.ydjk.org.cn/Article/details/gt3ualuhslr.html

srand(time(NULL));  int r = rand() % 100;
来源：http://www.52xcode.cn/Article/details/gt3erwetkbr.html

[S24] C：获取本地时间
来源：http://www.52xcode.cn/Article/details/gt3yjtzhkeb.html

time_t t = time(NULL);  struct tm *tm = localtime(&t);
来源：http://www.ydjk.org.cn/Article/details/gt3urqgcqjh.html

[S25] C：内存拷贝
来源：http://www.52xcode.cn/Article/details/gt3aexrnhou.html

memcpy(dst, src, n);
来源：http://www.ydjk.org.cn/Article/details/gt3sxwiejji.html

[S26] C：内存清零
来源：http://www.52xcode.cn/Article/details/gt3xgeqmwkx.html

memset(a, 0, sizeof a);
来源：http://www.52xcode.cn/Article/details/gt3hngodxzl.html

[S27] C：定义常量
来源：http://www.ydjk.org.cn/Article/details/gt3hhlxmvxw.html

const double PI = 3.14159;
来源：http://www.ydjk.org.cn/Article/details/gt3gtzhdgih.html

[S28] C：静态变量
来源：http://www.52xcode.cn/Article/details/gt3qotarrzs.html

static int counter = 0;
来源：http://www.52xcode.cn/Article/details/gt3dkhngpbv.html

[S29] C：变参函数
来源：http://www.ydjk.org.cn/Article/details/gt3wejgvfbj.html

va_list ap; va_start(ap, fmt); vprintf(fmt, ap); va_end(ap);
来源：http://www.52xcode.cn/Article/details/gt3urledqcn.html

[S30] C：头文件保护
来源：http://www.ydjk.org.cn/Article/details/gt3cadmqlrw.html

#ifndef X_H
来源：http://www.52xcode.cn/Article/details/gt3txtjuats.html

#define X_H
来源：http://www.52xcode.cn/Article/details/gt3ljrajbdj.html

#endif
来源：http://www.52xcode.cn/Article/details/gt3nbzvskkm.html

[S31] C++：Hello World
来源：http://www.ydjk.org.cn/Article/details/gt3qjupghfq.html

#include <iostream>
来源：http://www.52xcode.cn/Article/details/gt3vtulmcxv.html

int main() { std::cout << "Hello\n"; }
来源：http://www.ydjk.org.cn/Article/details/gt3xaxctqwy.html

[S32] C++：字符串
来源：http://www.ydjk.org.cn/Article/details/gt3rupetlvj.html

std::string s = "hi";  s += "!";
来源：http://www.ydjk.org.cn/Article/details/gt3ehxrfslt.html

[S33] C++：vector 增删
来源：http://www.ydjk.org.cn/Article/details/gt3igbnwgse.html

std::vector<int> v{1, 2, 3};  v.push_back(4);
来源：http://www.ydjk.org.cn/Article/details/gt3rpwvvvwq.html

[S34] C++：遍历 vector
来源：http://www.52xcode.cn/Article/details/gt3zxvrbrgn.html

for (auto &x : v) { std::cout << x; }
来源：http://www.ydjk.org.cn/Article/details/gt3jtveohvx.html

[S35] C++：map
来源：http://www.ydjk.org.cn/Article/details/gt3jzgewjnc.html

std::map<std::string, int> m;  m["a"] = 1;
来源：http://www.52xcode.cn/Article/details/gt3nacdvebs.html

[S36] C++：unordered_map
来源：http://www.52xcode.cn/Article/details/gt3xbmjzigw.html

std::unordered_map<std::string, int> m;  m["a"] = 1;
来源：http://www.52xcode.cn/Article/details/gt3ftapkyle.html

[S37] C++：set
来源：http://www.ydjk.org.cn/Article/details/gt3yplzcrja.html

std::set<int> s{1, 2, 3};  s.insert(4);
来源：http://www.52xcode.cn/Article/details/gt3rmsznyge.html

[S38] C++：排序
来源：http://www.52xcode.cn/Article/details/gt3xqpcxiuh.html

std::sort(v.begin(), v.end());
来源：http://www.ydjk.org.cn/Article/details/gt3qndhjspl.html

[S39] C++：自定义比较器排序
来源：http://www.52xcode.cn/Article/details/gt3sepbepcj.html

std::sort(v.begin(), v.end(), [](int a, int b) { return a > b; });
来源：http://www.52xcode.cn/Article/details/gt3albmajah.html

[S40] C++：查找元素
来源：http://www.ydjk.org.cn/Article/details/gt3odyhztcx.html

auto it = std::find(v.begin(), v.end(), 3);
来源：http://www.52xcode.cn/Article/details/gt3phwmizok.html

[S41] C++：类与构造函数
来源：http://www.ydjk.org.cn/Article/details/gt3yisdrktz.html

class A { public: A(int v) : x_(v) {} int get() const { return x_; } private: int x_; };
来源：http://www.52xcode.cn/Article/details/gt3lsdpzsxg.html

[S42] C++：继承与虚函数
来源：http://www.52xcode.cn/Article/details/gt3cwwunnkz.html

class B : public Base { public: void f() override {} };
来源：http://www.52xcode.cn/Article/details/gt3gpisuchr.html

[S43] C++：智能指针
来源：http://www.52xcode.cn/Article/details/gt3nkvtjpkr.html

auto p = std::make_unique<int>(5);
来源：http://www.52xcode.cn/Article/details/gt3fwqzwskr.html

[S44] C++：引用传参
来源：http://www.ydjk.org.cn/Article/details/gt3glszvvmr.html

void inc(int &x) { ++x; }
来源：http://www.52xcode.cn/Article/details/gt3aizmdvir.html

[S45] C++：lambda
来源：http://www.52xcode.cn/Article/details/gt3dctwzfja.html

auto add = [](int a, int b) { return a + b; };
来源：http://www.52xcode.cn/Article/details/gt3przbsagc.html

[S46] C++：函数模板
来源：http://www.ydjk.org.cn/Article/details/gt3yekbdsuh.html

template <typename T> T maxv(T a, T b) { return a > b ? a : b; }
来源：http://www.52xcode.cn/Article/details/gt3mybaiocw.html

[S47] C++：结构化绑定遍历
来源：http://www.52xcode.cn/Article/details/gt3nsuyvtyq.html

for (const auto &[k, v] : m) { std::cout << k << v; }
来源：http://www.ydjk.org.cn/Article/details/gt3opmmkpiu.html

[S48] C++：逐行读文件
来源：http://www.ydjk.org.cn/Article/details/gt3ubdqjukl.html

std::ifstream in("a.txt");  std::string line;
来源：http://www.52xcode.cn/Article/details/gt3cxwplein.html

while (std::getline(in, line)) { }
来源：http://www.52xcode.cn/Article/details/gt3gohnphra.html

[S49] C++：写文件
来源：http://www.52xcode.cn/Article/details/gt3lwszgtvm.html

std::ofstream out("a.txt");  out << "hi\n";
来源：http://www.ydjk.org.cn/Article/details/gt3eckkjnzh.html

[S50] C++：格式化数字
来源：http://www.52xcode.cn/Article/details/gt3wptcgiaq.html

std::ostringstream os;  os << std::fixed << std::setprecision(2) << 3.14159;
来源：http://www.52xcode.cn/Article/details/gt3weenkncq.html

[S51] C++：显式类型转换
来源：http://www.52xcode.cn/Article/details/gt3qapgsefl.html

static_cast<double>(a) / b
来源：http://www.ydjk.org.cn/Article/details/gt3jbcjgxtg.html

[S52] C++：const 与 noexcept
来源：http://www.ydjk.org.cn/Article/details/gt3bspvjylv.html

int size() const noexcept { return n_; }
来源：http://www.ydjk.org.cn/Article/details/gt3bqrhmhai.html

[S53] C++：移动语义
来源：http://www.52xcode.cn/Article/details/gt3qazikeyh.html

std::vector<int> w = std::move(v);
来源：http://www.52xcode.cn/Article/details/gt3pquacnok.html

[S54] C++：异常处理
来源：http://www.52xcode.cn/Article/details/gt3ekywgzbi.html

try { throw std::runtime_error("x"); } catch (const std::exception &e) { }
来源：http://www.ydjk.org.cn/Article/details/gt3iqkhtbld.html

[S55] C++：结构化绑定
来源：http://www.ydjk.org.cn/Article/details/gt3nlhyjhlg.html

auto [a, b] = std::make_pair(1, 2);
来源：http://www.52xcode.cn/Article/details/gt3fvnbzwvg.html

[S56] C++：optional
来源：http://www.ydjk.org.cn/Article/details/gt3bnwmungz.html

std::optional<int> o = 5;  if (o) { int v = *o; }
来源：http://www.ydjk.org.cn/Article/details/gt3ostoojvg.html

[S57] C++：编译期常量
来源：http://www.ydjk.org.cn/Article/details/gt3bkqsopou.html

constexpr int N = 10;
来源：http://www.ydjk.org.cn/Article/details/gt3dykakdnd.html

[S58] C++：命名空间
来源：http://www.ydjk.org.cn/Article/details/gt3znapfdcc.html

namespace ns { int f() { return 1; } }
来源：http://www.52xcode.cn/Article/details/gt3stygwuga.html

[S59] C++：静态断言
来源：http://www.52xcode.cn/Article/details/gt3vfjqfoon.html

static_assert(sizeof(int) == 4, "int 必须 4 字节");
来源：http://www.52xcode.cn/Article/details/gt3nwytzfil.html

[S60] C++：遍历并删除元素
来源：http://www.ydjk.org.cn/Article/details/gt3jsfhkrdd.html

v.erase(std::remove_if(v.begin(), v.end(), [](int x) { return x < 0; }), v.end());
来源：http://www.52xcode.cn/Article/details/gt3obwqqhrz.html

================================================================================
来源：http://www.ydjk.org.cn/Article/details/gt3hauowdog.html

T. 其他语言补充（Kotlin / Swift / Lua / Perl / Scala）
来源：http://www.ydjk.org.cn/Article/details/gt3wzevnmvc.html

================================================================================
来源：http://www.ydjk.org.cn/Article/details/gt3wnqlkppj.html

[T01] Kotlin：Hello World
来源：http://www.52xcode.cn/Article/details/gt3gmlpnkdg.html

println("Hello")
来源：http://www.ydjk.org.cn/Article/details/gt3yznkvvwt.html

[T02] Kotlin：变量
来源：http://www.ydjk.org.cn/Article/details/gt3dhmdbyhb.html

val a = 1;  var b = 2        // val 只读，var 可变
来源：http://www.ydjk.org.cn/Article/details/gt3pdbrhyii.html

[T03] Kotlin：字符串模板
来源：http://www.ydjk.org.cn/Article/details/gt3zksjhxct.html

"值: $b"
来源：http://www.52xcode.cn/Article/details/gt3dftjoylz.html

[T04] Kotlin：空安全
来源：http://www.ydjk.org.cn/Article/details/gt3evjarjbk.html

val n: String? = null;  n?.length
来源：http://www.52xcode.cn/Article/details/gt3odnpbnml.html

[T05] Kotlin：when 表达式
来源：http://www.ydjk.org.cn/Article/details/gt3ioerwzie.html

val s = when (x) { 1 -> "一" else -> "其他" }   // 多分支时每个分支单独一行
来源：http://www.52xcode.cn/Article/details/gt3ahyykzcv.html

[T06] Kotlin：集合映射
来源：http://www.ydjk.org.cn/Article/details/gt3klxqvmlp.html

listOf(1, 2, 3).map { it * 2 }
来源：http://www.52xcode.cn/Article/details/gt3kyradxdh.html

[T07] Kotlin：集合过滤
来源：http://www.ydjk.org.cn/Article/details/gt3lrhmvnlt.html

listOf(1, 2, 3).filter { it > 1 }
来源：http://www.52xcode.cn/Article/details/gt3vrrnpgkj.html

[T08] Kotlin：数据类
来源：http://www.52xcode.cn/Article/details/gt3kfjlubpx.html

data class User(val name: String, val age: Int)
来源：http://www.ydjk.org.cn/Article/details/gt3erbnsqmw.html

[T09] Kotlin：扩展函数
来源：http://www.ydjk.org.cn/Article/details/gt3hphsaxxa.html

fun String.exclaim() = this + "!"
来源：http://www.ydjk.org.cn/Article/details/gt3fiibueyp.html

[T10] Kotlin：默认参数
来源：http://www.ydjk.org.cn/Article/details/gt3degbgdag.html

fun greet(name: String = "World") = "Hi $name"
来源：http://www.ydjk.org.cn/Article/details/gt3htnayiex.html

[T11] Kotlin：协程
来源：http://www.ydjk.org.cn/Article/details/gt3gbkkbgaa.html

GlobalScope.launch { delay(1000); println("done") }
来源：http://www.ydjk.org.cn/Article/details/gt3qhrtqzbg.html

[T12] Kotlin：解构声明
来源：http://www.ydjk.org.cn/Article/details/gt3eyhccoiu.html

val (a, b) = Pair(1, 2)
来源：http://www.52xcode.cn/Article/details/gt3hiuyamwo.html

[T13] Kotlin：只读 Map
来源：http://www.ydjk.org.cn/Article/details/gt3umvvotdw.html

val m = mapOf("a" to 1)
来源：http://www.52xcode.cn/Article/details/gt3ybbbvwjg.html

[T14] Kotlin：循环
来源：http://www.52xcode.cn/Article/details/gt3wfrwogmv.html

for (i in 1..10) println(i)
来源：http://www.52xcode.cn/Article/details/gt3gyfvujvf.html

[T15] Kotlin：接口
来源：http://www.52xcode.cn/Article/details/gt3tydvhawl.html

interface Shape { fun area(): Double }
来源：http://www.52xcode.cn/Article/details/gt3mizpgwsm.html

[T16] Swift：Hello World
来源：http://www.ydjk.org.cn/Article/details/gt3ldoccvff.html

print("Hello")
来源：http://www.ydjk.org.cn/Article/details/gt3mmabktse.html

[T17] Swift：变量与常量
来源：http://www.52xcode.cn/Article/details/gt3jqymoers.html

var a = 1;  let b = 2
来源：http://www.52xcode.cn/Article/details/gt3mfxaprmn.html

[T18] Swift：字符串插值
来源：http://www.52xcode.cn/Article/details/gt3bivpzmmc.html

"值: \(b)"
来源：http://www.52xcode.cn/Article/details/gt3yvkbbzii.html

[T19] Swift：可选绑定
来源：http://www.52xcode.cn/Article/details/gt3lrukehrh.html

if let n = opt { print(n) }
来源：http://www.ydjk.org.cn/Article/details/gt3jqqvlljr.html

[T20] Swift：数组操作
来源：http://www.52xcode.cn/Article/details/gt3zoqfrfxa.html

var a = [1, 2, 3];  a.append(4)
来源：http://www.52xcode.cn/Article/details/gt3zhbvadrp.html

[T21] Swift：遍历
来源：http://www.52xcode.cn/Article/details/gt3ryybmlnw.html

for x in a { print(x) }
来源：http://www.ydjk.org.cn/Article/details/gt3slssbyoc.html

[T22] Swift：字典
来源：http://www.ydjk.org.cn/Article/details/gt3ufbxzusc.html

var d = ["a": 1];  d["b"] = 2
来源：http://www.ydjk.org.cn/Article/details/gt3gkbbxkvl.html

[T23] Swift：函数
来源：http://www.52xcode.cn/Article/details/gt3egveuwnh.html

func add(_ a: Int, _ b: Int) -> Int { a + b }
来源：http://www.52xcode.cn/Article/details/gt3kmuxnjme.html

[T24] Swift：闭包
来源：http://www.52xcode.cn/Article/details/gt3zetjsmxl.html

let f = { (x: Int) -> Int in x * 2 }
来源：http://www.ydjk.org.cn/Article/details/gt3jczvgjtn.html

[T25] Swift：结构体
来源：http://www.52xcode.cn/Article/details/gt3dqvwbpmp.html

struct P { var x: Int }
来源：http://www.ydjk.org.cn/Article/details/gt3vuydjwvp.html

[T26] Swift：类与重写
来源：http://www.ydjk.org.cn/Article/details/gt3rliyyamf.html

class A: Base { override func f() {} }
来源：http://www.52xcode.cn/Article/details/gt3maltqupz.html

[T27] Swift：错误处理
来源：http://www.52xcode.cn/Article/details/gt3nohwqkkp.html

do { try f() } catch { print(error) }
来源：http://www.52xcode.cn/Article/details/gt3aooyltnm.html

[T28] Swift：枚举
来源：http://www.ydjk.org.cn/Article/details/gt3uevicmpb.html

enum Color { case red, green }
来源：http://www.ydjk.org.cn/Article/details/gt3ubvnrhgj.html

[T29] Swift：guard 提前返回
来源：http://www.52xcode.cn/Article/details/gt3meoxjqhs.html

guard let x = opt else { return }
来源：http://www.ydjk.org.cn/Article/details/gt3imgnspyl.html

[T30] Swift：协议
来源：http://www.ydjk.org.cn/Article/details/gt3jttyjrgd.html

protocol Shape { func area() -> Double }
来源：http://www.ydjk.org.cn/Article/details/gt3riynlzhy.html

[T31] Lua：Hello World
来源：http://www.ydjk.org.cn/Article/details/gt3oazbkbjg.html

print("Hello")
来源：http://www.ydjk.org.cn/Article/details/gt3hrpkrnnt.html

[T32] Lua：局部变量
来源：http://www.ydjk.org.cn/Article/details/gt3ezbdsaki.html

local a = 1
来源：http://www.ydjk.org.cn/Article/details/gt3bkigsgec.html

[T33] Lua：表（数组）
来源：http://www.52xcode.cn/Article/details/gt3rjdaczjq.html

local t = {1, 2, 3};  t[4] = 4
来源：http://www.52xcode.cn/Article/details/gt3bxejxufp.html

[T34] Lua：遍历表
来源：http://www.52xcode.cn/Article/details/gt3jqvzrfbp.html

for i, v in ipairs(t) do print(i, v) end
来源：http://www.ydjk.org.cn/Article/details/gt3kvsnaple.html

[T35] Lua：字典表
来源：http://www.52xcode.cn/Article/details/gt3rrrwbpen.html

local d = { a = 1 };  d.b = 2
来源：http://www.52xcode.cn/Article/details/gt3rijfgajv.html

[T36] Lua：函数
来源：http://www.ydjk.org.cn/Article/details/gt3klnwvqyr.html

function add(a, b) return a + b end
来源：http://www.ydjk.org.cn/Article/details/gt3eeufttze.html

[T37] Lua：字符串拼接
来源：http://www.52xcode.cn/Article/details/gt3qoirfaec.html

"a" .. "b"
来源：http://www.52xcode.cn/Article/details/gt3khpjkpwy.html

[T38] Lua：条件
来源：http://www.52xcode.cn/Article/details/gt3bzsvpzww.html

if x > 0 then print("正") end
来源：http://www.52xcode.cn/Article/details/gt3nkzkpuwm.html

[T39] Lua：模式匹配
来源：http://www.52xcode.cn/Article/details/gt3tbcoagee.html

string.find(s, "%d+")
来源：http://www.ydjk.org.cn/Article/details/gt3tmpvumlc.html

[T40] Lua：元表
来源：http://www.ydjk.org.cn/Article/details/gt3mykmqqvg.html

setmetatable({}, { __index = base })
来源：http://www.ydjk.org.cn/Article/details/gt3nrceqjoc.html

[T41] Perl：Hello World
来源：http://www.52xcode.cn/Article/details/gt3bsuzvgrw.html

print "Hello\n";
来源：http://www.ydjk.org.cn/Article/details/gt3qjomixer.html

[T42] Perl：变量类型
来源：http://www.52xcode.cn/Article/details/gt3thpquscv.html

my $a = 1;  my @arr = (1, 2, 3);  my %h = (a => 1);
来源：http://www.ydjk.org.cn/Article/details/gt3ftasoiuu.html

[T43] Perl：字符串插值
来源：http://www.ydjk.org.cn/Article/details/gt3twjtebhd.html

"值: $a"
来源：http://www.ydjk.org.cn/Article/details/gt3gwwbpyfm.html

[T44] Perl：条件
来源：http://www.ydjk.org.cn/Article/details/gt3wjmtrsos.html

if ($a > 0) { print "正"; }
来源：http://www.52xcode.cn/Article/details/gt3sqxltpoi.html

[T45] Perl：数组遍历
来源：http://www.ydjk.org.cn/Article/details/gt3khavbyox.html

for my $x (@arr) { print $x; }
来源：http://www.ydjk.org.cn/Article/details/gt3sssaycai.html

[T46] Perl：哈希操作
来源：http://www.ydjk.org.cn/Article/details/gt3uhpefihp.html

$h{b} = 2;  for my $k (keys %h) { print "$k=$h{$k}"; }
来源：http://www.ydjk.org.cn/Article/details/gt3gpliljtu.html

[T47] Perl：正则捕获
来源：http://www.52xcode.cn/Article/details/gt3ospbulfd.html

if ($s =~ /(\d+)/) { print $1; }
来源：http://www.52xcode.cn/Article/details/gt3ipuzdmxs.html

[T48] Perl：正则替换
来源：http://www.ydjk.org.cn/Article/details/gt3wijcnqqm.html

$s =~ s/old/new/g;
来源：http://www.ydjk.org.cn/Article/details/gt3mlbaqcve.html

[T49] Perl：函数
来源：http://www.ydjk.org.cn/Article/details/gt3djlmapmp.html

sub add { my ($a, $b) = @_; return $a + $b; }
来源：http://www.52xcode.cn/Article/details/gt3fmohswqs.html

[T50] Perl：逐行读文件
来源：http://www.ydjk.org.cn/Article/details/gt3csjuocvf.html

open my $fh, "<", "a.txt" or die $!;
来源：http://www.ydjk.org.cn/Article/details/gt3lwbvyltz.html

while (my $line = <$fh>) { print $line; }
来源：http://www.ydjk.org.cn/Article/details/gt3uqzlcldh.html

[T51] Scala：Hello World
来源：http://www.ydjk.org.cn/Article/details/gt3otxhzlby.html

println("Hello")
来源：http://www.52xcode.cn/Article/details/gt3qitxotgj.html

[T52] Scala：变量
来源：http://www.ydjk.org.cn/Article/details/gt3ptlkedxu.html

val a = 1;  var b = 2
来源：http://www.52xcode.cn/Article/details/gt3tdlkfsru.html

[T53] Scala：字符串插值
来源：http://www.52xcode.cn/Article/details/gt3faouzvxc.html

s"值: $b"
来源：http://www.ydjk.org.cn/Article/details/gt3jnpjvoll.html

[T54] Scala：集合映射
来源：http://www.52xcode.cn/Article/details/gt3mkedxyzc.html

List(1, 2, 3).map(_ * 2)
来源：http://www.ydjk.org.cn/Article/details/gt3afsvtglr.html

[T55] Scala：集合过滤
来源：http://www.52xcode.cn/Article/details/gt3jxdhbshq.html

List(1, 2, 3).filter(_ > 1)
来源：http://www.52xcode.cn/Article/details/gt3nzraitnt.html

[T56] Scala：样例类
来源：http://www.ydjk.org.cn/Article/details/gt3valfefou.html

case class User(name: String, age: Int)
来源：http://www.52xcode.cn/Article/details/gt3lqzqogfy.html

[T57] Scala：模式匹配
来源：http://www.52xcode.cn/Article/details/gt3uytqfjra.html

x match { case 1 => "一"; case _ => "其他" }
来源：http://www.ydjk.org.cn/Article/details/gt3jptkubwy.html

[T58] Scala：函数定义
来源：http://www.ydjk.org.cn/Article/details/gt3tewhtmfe.html

def add(a: Int, b: Int): Int = a + b
来源：http://www.52xcode.cn/Article/details/gt3uzzqeaiq.html

[T59] Scala：循环
来源：http://www.52xcode.cn/Article/details/gt3idgecztz.html

for (i <- 1 to 10) println(i)
来源：http://www.52xcode.cn/Article/details/gt3cwbcnmqi.html

[T60] Scala：折叠
来源：http://www.52xcode.cn/Article/details/gt3sbfpkivi.html

List(1, 2, 3).foldLeft(0)(_ + _)
来源：http://www.52xcode.cn/Article/details/gt3lmhhveuv.html

================================================================================
来源：http://www.ydjk.org.cn/Article/details/gt3upldpodg.html

U. 高频实用片段（Python / PHP / JavaScript 各 40 条）
来源：http://www.52xcode.cn/Article/details/gt3lcxedkpn.html

================================================================================
来源：http://www.52xcode.cn/Article/details/gt3jaoxkosc.html

[U01] Py：创建虚拟环境
来源：http://www.ydjk.org.cn/Article/details/gt3gaudfejs.html

python -m venv .venv && source .venv/bin/activate
来源：http://www.52xcode.cn/Article/details/gt3wtfpjjfi.html

[U02] Py：导出 / 安装依赖
来源：http://www.ydjk.org.cn/Article/details/gt3ldlgbinb.html

pip freeze > requirements.txt;  pip install -r requirements.txt
来源：http://www.52xcode.cn/Article/details/gt3nnfgfwxx.html

[U03] Py：加载 .env 配置
来源：http://www.52xcode.cn/Article/details/gt3sofglyom.html

from dotenv import load_dotenv; load_dotenv()
来源：http://www.52xcode.cn/Article/details/gt3goxszrzu.html

[U04] Py：变量调试打印
来源：http://www.ydjk.org.cn/Article/details/gt3mlkubrbn.html

print(f"{x=}")            # 输出 x=值，Python 3.8+
来源：http://www.ydjk.org.cn/Article/details/gt3dticzfjo.html

[U05] Py：列表去重且保序
来源：http://www.ydjk.org.cn/Article/details/gt3skujvxin.html

list(dict.fromkeys(arr))
来源：http://www.52xcode.cn/Article/details/gt3wqlbnghp.html

[U06] Py：合并两个字典
来源：http://www.ydjk.org.cn/Article/details/gt3grmqtjrp.html

{**a, **b}
来源：http://www.ydjk.org.cn/Article/details/gt3ecufxpur.html

[U07] Py：反转字典键值
来源：http://www.52xcode.cn/Article/details/gt3cymqbjyf.html

{v: k for k, v in d.items()}
来源：http://www.52xcode.cn/Article/details/gt3wdjbpwur.html

[U08] Py：展平二维列表
来源：http://www.ydjk.org.cn/Article/details/gt3sgvhqmuq.html

[y for x in nested for y in x]
来源：http://www.ydjk.org.cn/Article/details/gt3qkdujvdb.html

[U09] Py：字典取最大值的键
来源：http://www.52xcode.cn/Article/details/gt3gehgaqxg.html

max(d, key=d.get)
来源：http://www.ydjk.org.cn/Article/details/gt3pcciahnp.html

[U10] Py：按值排序字典
来源：http://www.52xcode.cn/Article/details/gt3toisyjun.html

dict(sorted(d.items(), key=lambda kv: kv[1]))
来源：http://www.ydjk.org.cn/Article/details/gt3ycoftdan.html


<!-- 参考信息 -->