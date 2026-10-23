代发 wailian999

split -l 1000 big.log part_
来源：http://www.52xcode.cn/Article/details/gt3lsmvtqug.html

[R74] 批量重命名
来源：http://www.52xcode.cn/Article/details/gt3sqcomohq.html

for f in *.jpeg; do mv "$f" "${f%.jpeg}.jpg"; done
来源：http://www.ydjk.org.cn/Article/details/gt3xazczhnq.html

[R75] 导出环境变量
来源：http://www.ydjk.org.cn/Article/details/gt3hdvlobpa.html

export PATH="$HOME/bin:$PATH"
来源：http://www.52xcode.cn/Article/details/gt3ksfcukho.html

[R76] 使用临时文件
来源：http://www.ydjk.org.cn/Article/details/gt3dtqkympk.html

tmp=$(mktemp); trap 'rm -f "$tmp"' EXIT
来源：http://www.ydjk.org.cn/Article/details/gt3biwchtdx.html

[R77] 读取用户输入
来源：http://www.ydjk.org.cn/Article/details/gt3pxoelmoy.html

read -rp "请输入: " ans
来源：http://www.52xcode.cn/Article/details/gt3cjzhmetm.html

[R78] 交互式菜单
来源：http://www.52xcode.cn/Article/details/gt3chiidbsf.html

select opt in a b c; do echo "$opt"; break; done
来源：http://www.ydjk.org.cn/Article/details/gt3ydxbkfjw.html

[R79] 解析命令行选项
来源：http://www.ydjk.org.cn/Article/details/gt3pltnxnnk.html

while getopts "v:f:" o; do case $o in v) V=$OPTARG ;; f) F=$OPTARG ;; esac; done
来源：http://www.ydjk.org.cn/Article/details/gt3rsyghbko.html

[R80] 查看脚本执行耗时
来源：http://www.52xcode.cn/Article/details/gt3khtslixn.html

time ./run.sh
来源：http://www.52xcode.cn/Article/details/gt3diqxjcxt.html

================================================================================
来源：http://www.ydjk.org.cn/Article/details/gt3jotjnmgf.html

S. C / C++ 专题
来源：http://www.ydjk.org.cn/Article/details/gt3kicsslfu.html

================================================================================
来源：http://www.ydjk.org.cn/Article/details/gt3zwyyrnmz.html

[S01] C：Hello World
来源：http://www.52xcode.cn/Article/details/gt3boydluco.html

#include <stdio.h>
来源：http://www.ydjk.org.cn/Article/details/gt3qafsyrcf.html

int main(void) { printf("Hello\n"); return 0; }
来源：http://www.52xcode.cn/Article/details/gt3vzaanrqb.html

[S02] C：变量与格式化输出
来源：http://www.52xcode.cn/Article/details/gt3fvqdliaq.html

int a = 10; printf("%d\n", a);
来源：http://www.52xcode.cn/Article/details/gt3zsiulpdf.html

[S03] C：读入整数
来源：http://www.ydjk.org.cn/Article/details/gt3eorsqwyf.html

int x; scanf("%d", &x);
来源：http://www.ydjk.org.cn/Article/details/gt3wccxjurg.html

[S04] C：字符串复制
来源：http://www.52xcode.cn/Article/details/gt3ltrsqilv.html

char dst[32]; strcpy(dst, "hi");
来源：http://www.52xcode.cn/Article/details/gt3yoiixrsk.html

[S05] C：字符串长度
来源：http://www.ydjk.org.cn/Article/details/gt3mjrfgutm.html

strlen(s)
来源：http://www.52xcode.cn/Article/details/gt3krnpvotw.html

[S06] C：字符串比较
来源：http://www.ydjk.org.cn/Article/details/gt3cuctewjv.html

strcmp(a, b) == 0
来源：http://www.52xcode.cn/Article/details/gt3dnuwvnzv.html

[S07] C：数组遍历求和
来源：http://www.ydjk.org.cn/Article/details/gt3ltulsklu.html

for (int i = 0; i < n; i++) sum += a[i];
来源：http://www.ydjk.org.cn/Article/details/gt3jktpwsns.html

[S08] C：动态内存分配与释放
来源：http://www.52xcode.cn/Article/details/gt3sxiumqny.html

int *p = malloc(sizeof(int) * n); ... free(p);
来源：http://www.52xcode.cn/Article/details/gt3cgpabwhq.html

[S09] C：结构体定义与初始化
来源：http://www.52xcode.cn/Article/details/gt3vyabheuu.html

struct Point { int x, y; };  struct Point p = {1, 2};
来源：http://www.ydjk.org.cn/Article/details/gt3mfdhmiqk.html

[S10] C：指针与解引用
来源：http://www.52xcode.cn/Article/details/gt3foxvevgw.html

int *p = &a;  *p = 5;
来源：http://www.ydjk.org.cn/Article/details/gt3oktpqvok.html

[S11] C：逐行读文件
来源：http://www.52xcode.cn/Article/details/gt3jkxudomp.html

FILE *f = fopen("a.txt", "r");
来源：http://www.52xcode.cn/Article/details/gt3iyxhtcit.html

while (fgets(buf, sizeof buf, f)) { }
来源：http://www.52xcode.cn/Article/details/gt3cdievprn.html

fclose(f);
来源：http://www.52xcode.cn/Article/details/gt3fruupcnb.html

[S12] C：写文件
来源：http://www.52xcode.cn/Article/details/gt3ndrvmzeb.html

FILE *f = fopen("a.txt", "w");  fprintf(f, "hi\n");  fclose(f);
来源：http://www.ydjk.org.cn/Article/details/gt3oimphtqx.html

[S13] C：宏定义
来源：http://www.52xcode.cn/Article/details/gt3hqscpgeu.html

#define MAX(a, b) ((a) > (b) ? (a) : (b))
来源：http://www.ydjk.org.cn/Article/details/gt3itaelvqj.html

[S14] C：枚举
来源：http://www.52xcode.cn/Article/details/gt3qaokwfoz.html

enum Color { RED, GREEN, BLUE };
来源：http://www.ydjk.org.cn/Article/details/gt3lzhridih.html

[S15] C：类型转换
来源：http://www.52xcode.cn/Article/details/gt3euqdfetz.html

(double) a / b
来源：http://www.ydjk.org.cn/Article/details/gt3xgicqfcj.html

[S16] C：位操作置位
来源：http://www.ydjk.org.cn/Article/details/gt3fbmxneqc.html

x |= (1 << 3);
来源：http://www.ydjk.org.cn/Article/details/gt3wqmdxkoo.html

[S17] C：安全拼接字符串
来源：http://www.52xcode.cn/Article/details/gt3qtooyvfj.html

snprintf(buf, sizeof buf, "%s%s", a, b);
来源：http://www.ydjk.org.cn/Article/details/gt3zvocghui.html

[S18] C：命令行参数
来源：http://www.52xcode.cn/Article/details/gt3yvmxwbtl.html

int main(int argc, char **argv)
来源：http://www.52xcode.cn/Article/details/gt3xnwygyzk.html

[S19] C：快速排序
来源：http://www.52xcode.cn/Article/details/gt3lolvzmmz.html

qsort(a, n, sizeof(int), cmp);
来源：http://www.ydjk.org.cn/Article/details/gt3yooffrer.html

[S20] C：二分查找
来源：http://www.ydjk.org.cn/Article/details/gt3antnokxa.html

bsearch(&key, a, n, sizeof(int), cmp);
来源：http://www.52xcode.cn/Article/details/gt3gjbevcqf.html

[S21] C：字符类别判断
来源：http://www.ydjk.org.cn/Article/details/gt3xgqjyuvk.html

isdigit(c);  isalpha(c);  isspace(c);
来源：http://www.52xcode.cn/Article/details/gt3fahjpomw.html

[S22] C：字符串转数字
来源：http://www.52xcode.cn/Article/details/gt3mdbyrsmy.html

atoi("42");  strtod("3.14", NULL);
来源：http://www.ydjk.org.cn/Article/details/gt3awedabpt.html

[S23] C：随机数
来源：http://www.ydjk.org.cn/Article/details/gt3zqzdyzzx.html

srand(time(NULL));  int r = rand() % 100;
来源：http://www.52xcode.cn/Article/details/gt3siuwmqdl.html

[S24] C：获取本地时间
来源：http://www.52xcode.cn/Article/details/gt3dzswhapr.html

time_t t = time(NULL);  struct tm *tm = localtime(&t);
来源：http://www.52xcode.cn/Article/details/gt3eaexqfcw.html

[S25] C：内存拷贝
来源：http://www.ydjk.org.cn/Article/details/gt3ywnlkhjt.html

memcpy(dst, src, n);
来源：http://www.52xcode.cn/Article/details/gt3bldvsqyq.html

[S26] C：内存清零
来源：http://www.ydjk.org.cn/Article/details/gt3nxujeuai.html

memset(a, 0, sizeof a);
来源：http://www.ydjk.org.cn/Article/details/gt3lktulxzf.html

[S27] C：定义常量
来源：http://www.ydjk.org.cn/Article/details/gt3lxbslyjd.html

const double PI = 3.14159;
来源：http://www.52xcode.cn/Article/details/gt3dyliedyz.html

[S28] C：静态变量
来源：http://www.ydjk.org.cn/Article/details/gt3ivvajdkr.html

static int counter = 0;
来源：http://www.52xcode.cn/Article/details/gt3zadewdtm.html

[S29] C：变参函数
来源：http://www.ydjk.org.cn/Article/details/gt3gjvizlho.html

va_list ap; va_start(ap, fmt); vprintf(fmt, ap); va_end(ap);
来源：http://www.52xcode.cn/Article/details/gt3rptvgejf.html

[S30] C：头文件保护
来源：http://www.52xcode.cn/Article/details/gt3tfcsdymi.html

#ifndef X_H
来源：http://www.52xcode.cn/Article/details/gt3ectnyovr.html

#define X_H
来源：http://www.52xcode.cn/Article/details/gt3qsqfoqfn.html

#endif
来源：http://www.ydjk.org.cn/Article/details/gt3qvyuedsn.html

[S31] C++：Hello World
来源：http://www.52xcode.cn/Article/details/gt3swudjajz.html

#include <iostream>
来源：http://www.52xcode.cn/Article/details/gt3okjgiifj.html

int main() { std::cout << "Hello\n"; }
来源：http://www.ydjk.org.cn/Article/details/gt3gtlvbish.html

[S32] C++：字符串
来源：http://www.ydjk.org.cn/Article/details/gt3pyqgspcj.html

std::string s = "hi";  s += "!";
来源：http://www.ydjk.org.cn/Article/details/gt3njmuvrus.html

[S33] C++：vector 增删
来源：http://www.ydjk.org.cn/Article/details/gt3yfgxuxnj.html

std::vector<int> v{1, 2, 3};  v.push_back(4);
来源：http://www.52xcode.cn/Article/details/gt3endtxmbe.html

[S34] C++：遍历 vector
来源：http://www.ydjk.org.cn/Article/details/gt3qfweypjd.html

for (auto &x : v) { std::cout << x; }
来源：http://www.52xcode.cn/Article/details/gt3ytbyuhtc.html

[S35] C++：map
来源：http://www.ydjk.org.cn/Article/details/gt3pzuwdgyv.html

std::map<std::string, int> m;  m["a"] = 1;
来源：http://www.52xcode.cn/Article/details/gt3cqezbbsk.html

[S36] C++：unordered_map
来源：http://www.52xcode.cn/Article/details/gt3vfahtsut.html

std::unordered_map<std::string, int> m;  m["a"] = 1;
来源：http://www.ydjk.org.cn/Article/details/gt3ohznlirx.html

[S37] C++：set
来源：http://www.52xcode.cn/Article/details/gt3tdstozqt.html

std::set<int> s{1, 2, 3};  s.insert(4);
来源：http://www.ydjk.org.cn/Article/details/gt3putoxgpx.html

[S38] C++：排序
来源：http://www.52xcode.cn/Article/details/gt3whbqenmz.html

std::sort(v.begin(), v.end());
来源：http://www.ydjk.org.cn/Article/details/gt3lncxztek.html

[S39] C++：自定义比较器排序
来源：http://www.52xcode.cn/Article/details/gt3jyoqnvdh.html

std::sort(v.begin(), v.end(), [](int a, int b) { return a > b; });
来源：http://www.ydjk.org.cn/Article/details/gt3dmeomshy.html

[S40] C++：查找元素
来源：http://www.ydjk.org.cn/Article/details/gt3roeyvyrh.html

auto it = std::find(v.begin(), v.end(), 3);
来源：http://www.ydjk.org.cn/Article/details/gt3sccobmkb.html

[S41] C++：类与构造函数
来源：http://www.52xcode.cn/Article/details/gt3rpvsxtge.html

class A { public: A(int v) : x_(v) {} int get() const { return x_; } private: int x_; };
来源：http://www.52xcode.cn/Article/details/gt3ofckuzob.html

[S42] C++：继承与虚函数
来源：http://www.ydjk.org.cn/Article/details/gt3wgmlswfg.html

class B : public Base { public: void f() override {} };
来源：http://www.ydjk.org.cn/Article/details/gt3aevsdktk.html

[S43] C++：智能指针
来源：http://www.52xcode.cn/Article/details/gt3kjaeaysm.html

auto p = std::make_unique<int>(5);
来源：http://www.52xcode.cn/Article/details/gt3dacpdkfn.html

[S44] C++：引用传参
来源：http://www.ydjk.org.cn/Article/details/gt3jniphrjx.html

void inc(int &x) { ++x; }
来源：http://www.ydjk.org.cn/Article/details/gt3iaybycef.html

[S45] C++：lambda
来源：http://www.ydjk.org.cn/Article/details/gt3kfisrnev.html

auto add = [](int a, int b) { return a + b; };
来源：http://www.52xcode.cn/Article/details/gt3tywpptmg.html

[S46] C++：函数模板
来源：http://www.52xcode.cn/Article/details/gt3jpncuywg.html

template <typename T> T maxv(T a, T b) { return a > b ? a : b; }
来源：http://www.52xcode.cn/Article/details/gt3ruyoqvqw.html

[S47] C++：结构化绑定遍历
来源：http://www.ydjk.org.cn/Article/details/gt3abrzjtrm.html

for (const auto &[k, v] : m) { std::cout << k << v; }
来源：http://www.52xcode.cn/Article/details/gt3dfdoerwq.html

[S48] C++：逐行读文件
来源：http://www.ydjk.org.cn/Article/details/gt3dovhdnoq.html

std::ifstream in("a.txt");  std::string line;
来源：http://www.ydjk.org.cn/Article/details/gt3pzssjlge.html

while (std::getline(in, line)) { }
来源：http://www.52xcode.cn/Article/details/gt3ucuytwpa.html

[S49] C++：写文件
来源：http://www.ydjk.org.cn/Article/details/gt3tnnheute.html

std::ofstream out("a.txt");  out << "hi\n";
来源：http://www.52xcode.cn/Article/details/gt3ejqwxbik.html

[S50] C++：格式化数字
来源：http://www.ydjk.org.cn/Article/details/gt3ddzadepv.html

std::ostringstream os;  os << std::fixed << std::setprecision(2) << 3.14159;
来源：http://www.52xcode.cn/Article/details/gt3jriowqbd.html

[S51] C++：显式类型转换
来源：http://www.52xcode.cn/Article/details/gt3hyqnpmdd.html

static_cast<double>(a) / b
来源：http://www.ydjk.org.cn/Article/details/gt3pgofaiie.html

[S52] C++：const 与 noexcept
来源：http://www.ydjk.org.cn/Article/details/gt3cmzdelxo.html

int size() const noexcept { return n_; }
来源：http://www.52xcode.cn/Article/details/gt3ngcqkpkf.html

[S53] C++：移动语义
来源：http://www.ydjk.org.cn/Article/details/gt3xlpxvmia.html

std::vector<int> w = std::move(v);
来源：http://www.ydjk.org.cn/Article/details/gt3pqmbidvo.html

[S54] C++：异常处理
来源：http://www.52xcode.cn/Article/details/gt3wrpqddlw.html

try { throw std::runtime_error("x"); } catch (const std::exception &e) { }
来源：http://www.ydjk.org.cn/Article/details/gt3caavkxjw.html

[S55] C++：结构化绑定
来源：http://www.52xcode.cn/Article/details/gt3shyywvab.html

auto [a, b] = std::make_pair(1, 2);
来源：http://www.ydjk.org.cn/Article/details/gt3wmaatdtd.html

[S56] C++：optional
来源：http://www.52xcode.cn/Article/details/gt3nyjhmbax.html

std::optional<int> o = 5;  if (o) { int v = *o; }
来源：http://www.ydjk.org.cn/Article/details/gt3rnsahwon.html

[S57] C++：编译期常量
来源：http://www.ydjk.org.cn/Article/details/gt3fpllrpgp.html

constexpr int N = 10;
来源：http://www.ydjk.org.cn/Article/details/gt3uobjwlgt.html

[S58] C++：命名空间
来源：http://www.52xcode.cn/Article/details/gt3siwabaqh.html

namespace ns { int f() { return 1; } }
来源：http://www.ydjk.org.cn/Article/details/gt3rfeiykbx.html

[S59] C++：静态断言
来源：http://www.ydjk.org.cn/Article/details/gt3zlzxdgrz.html

static_assert(sizeof(int) == 4, "int 必须 4 字节");
来源：http://www.52xcode.cn/Article/details/gt3otseatze.html

[S60] C++：遍历并删除元素
来源：http://www.ydjk.org.cn/Article/details/gt3mtclkqtc.html

v.erase(std::remove_if(v.begin(), v.end(), [](int x) { return x < 0; }), v.end());
来源：http://www.52xcode.cn/Article/details/gt3urcpvkba.html

================================================================================
来源：http://www.ydjk.org.cn/Article/details/gt3jeryygiq.html

T. 其他语言补充（Kotlin / Swift / Lua / Perl / Scala）
来源：http://www.ydjk.org.cn/Article/details/gt3ygdbfuem.html

================================================================================
来源：http://www.52xcode.cn/Article/details/gt3yrlflgbs.html

[T01] Kotlin：Hello World
来源：http://www.ydjk.org.cn/Article/details/gt3ckpwffow.html

println("Hello")
来源：http://www.ydjk.org.cn/Article/details/gt3kmiaakib.html

[T02] Kotlin：变量
来源：http://www.52xcode.cn/Article/details/gt3chmaejzb.html

val a = 1;  var b = 2        // val 只读，var 可变
来源：http://www.52xcode.cn/Article/details/gt3dykjezqn.html

[T03] Kotlin：字符串模板
来源：http://www.ydjk.org.cn/Article/details/gt3odhqeyik.html

"值: $b"
来源：http://www.ydjk.org.cn/Article/details/gt3jzgsmacf.html

[T04] Kotlin：空安全
来源：http://www.ydjk.org.cn/Article/details/gt3sqcuctfe.html

val n: String? = null;  n?.length
来源：http://www.52xcode.cn/Article/details/gt3vxkjfhfm.html

[T05] Kotlin：when 表达式
来源：http://www.ydjk.org.cn/Article/details/gt3qtdpwvqj.html

val s = when (x) { 1 -> "一" else -> "其他" }   // 多分支时每个分支单独一行
来源：http://www.ydjk.org.cn/Article/details/gt3zvucaghc.html

[T06] Kotlin：集合映射
来源：http://www.52xcode.cn/Article/details/gt3kofvgvyy.html

listOf(1, 2, 3).map { it * 2 }
来源：http://www.ydjk.org.cn/Article/details/gt3ayjnttjj.html

[T07] Kotlin：集合过滤
来源：http://www.52xcode.cn/Article/details/gt3upihwxth.html

listOf(1, 2, 3).filter { it > 1 }
来源：http://www.ydjk.org.cn/Article/details/gt3rlczhurj.html

[T08] Kotlin：数据类
来源：http://www.ydjk.org.cn/Article/details/gt3swbjwyff.html

data class User(val name: String, val age: Int)
来源：http://www.52xcode.cn/Article/details/gt3nwgrylbe.html

[T09] Kotlin：扩展函数
来源：http://www.52xcode.cn/Article/details/gt3bpbjbtly.html

fun String.exclaim() = this + "!"
来源：http://www.52xcode.cn/Article/details/gt3qahsiceu.html

[T10] Kotlin：默认参数
来源：http://www.ydjk.org.cn/Article/details/gt3jpyeiftf.html

fun greet(name: String = "World") = "Hi $name"
来源：http://www.52xcode.cn/Article/details/gt3tioufmic.html

[T11] Kotlin：协程
来源：http://www.52xcode.cn/Article/details/gt3agqrpbyp.html

GlobalScope.launch { delay(1000); println("done") }
来源：http://www.52xcode.cn/Article/details/gt3naxgqrzv.html

[T12] Kotlin：解构声明
来源：http://www.ydjk.org.cn/Article/details/gt3dpulsxix.html

val (a, b) = Pair(1, 2)
来源：http://www.52xcode.cn/Article/details/gt3xlvbvmue.html

[T13] Kotlin：只读 Map
来源：http://www.ydjk.org.cn/Article/details/gt3jbwzfklf.html

val m = mapOf("a" to 1)
来源：http://www.ydjk.org.cn/Article/details/gt3kegnxudc.html

[T14] Kotlin：循环
来源：http://www.ydjk.org.cn/Article/details/gt3iswimqjh.html

for (i in 1..10) println(i)
来源：http://www.ydjk.org.cn/Article/details/gt3bczzvdsa.html

[T15] Kotlin：接口
来源：http://www.52xcode.cn/Article/details/gt3pqtfruap.html

interface Shape { fun area(): Double }
来源：http://www.ydjk.org.cn/Article/details/gt3eerzfgpv.html

[T16] Swift：Hello World
来源：http://www.52xcode.cn/Article/details/gt3zgkhlesb.html

print("Hello")
来源：http://www.ydjk.org.cn/Article/details/gt3dsnuzrfd.html

[T17] Swift：变量与常量
来源：http://www.52xcode.cn/Article/details/gt3uzffhwic.html

var a = 1;  let b = 2
来源：http://www.52xcode.cn/Article/details/gt3kotdfwbo.html

[T18] Swift：字符串插值
来源：http://www.52xcode.cn/Article/details/gt3hwlfpgge.html

"值: \(b)"
来源：http://www.ydjk.org.cn/Article/details/gt3xeajzsli.html

[T19] Swift：可选绑定
来源：http://www.ydjk.org.cn/Article/details/gt3zsnpgdus.html

if let n = opt { print(n) }
来源：http://www.52xcode.cn/Article/details/gt3dlcamdmg.html

[T20] Swift：数组操作
来源：http://www.ydjk.org.cn/Article/details/gt3inoybfwj.html

var a = [1, 2, 3];  a.append(4)
来源：http://www.52xcode.cn/Article/details/gt3wqoyfckd.html

[T21] Swift：遍历
来源：http://www.ydjk.org.cn/Article/details/gt3ckqlvezi.html

for x in a { print(x) }
来源：http://www.52xcode.cn/Article/details/gt3fzcghwte.html

[T22] Swift：字典
来源：http://www.52xcode.cn/Article/details/gt3knxarecc.html

var d = ["a": 1];  d["b"] = 2
来源：http://www.52xcode.cn/Article/details/gt3fsycsppb.html

[T23] Swift：函数
来源：http://www.ydjk.org.cn/Article/details/gt3drdmjyhz.html

func add(_ a: Int, _ b: Int) -> Int { a + b }
来源：http://www.52xcode.cn/Article/details/gt3izopjsfl.html

[T24] Swift：闭包
来源：http://www.52xcode.cn/Article/details/gt3ommlczmn.html

let f = { (x: Int) -> Int in x * 2 }
来源：http://www.ydjk.org.cn/Article/details/gt3qjpxnyqt.html

[T25] Swift：结构体
来源：http://www.52xcode.cn/Article/details/gt3tmhiilpt.html

struct P { var x: Int }
来源：http://www.ydjk.org.cn/Article/details/gt3xqezsfyc.html

[T26] Swift：类与重写
来源：http://www.ydjk.org.cn/Article/details/gt3cokcksbr.html

class A: Base { override func f() {} }
来源：http://www.ydjk.org.cn/Article/details/gt3ibgjptfc.html

[T27] Swift：错误处理
来源：http://www.ydjk.org.cn/Article/details/gt3rclegcwd.html

do { try f() } catch { print(error) }
来源：http://www.52xcode.cn/Article/details/gt3pyzdrcgq.html

[T28] Swift：枚举
来源：http://www.52xcode.cn/Article/details/gt3pyolxlkl.html

enum Color { case red, green }
来源：http://www.ydjk.org.cn/Article/details/gt3qggfivtb.html

[T29] Swift：guard 提前返回
来源：http://www.52xcode.cn/Article/details/gt3azzooyrp.html

guard let x = opt else { return }
来源：http://www.52xcode.cn/Article/details/gt3dovrlcfz.html

[T30] Swift：协议
来源：http://www.52xcode.cn/Article/details/gt3hundsfzq.html

protocol Shape { func area() -> Double }
来源：http://www.ydjk.org.cn/Article/details/gt3akhnrrmo.html

[T31] Lua：Hello World
来源：http://www.52xcode.cn/Article/details/gt3boqjlurj.html

print("Hello")
来源：http://www.52xcode.cn/Article/details/gt3sbdjjrfu.html

[T32] Lua：局部变量
来源：http://www.52xcode.cn/Article/details/gt3buvjhnnl.html

local a = 1
来源：http://www.ydjk.org.cn/Article/details/gt3gjcysecd.html

[T33] Lua：表（数组）
来源：http://www.ydjk.org.cn/Article/details/gt3cjmaiwky.html

local t = {1, 2, 3};  t[4] = 4
来源：http://www.52xcode.cn/Article/details/gt3ahiutzzx.html

[T34] Lua：遍历表
来源：http://www.ydjk.org.cn/Article/details/gt3avgrnryb.html

for i, v in ipairs(t) do print(i, v) end
来源：http://www.52xcode.cn/Article/details/gt3kdurdclf.html

[T35] Lua：字典表
来源：http://www.ydjk.org.cn/Article/details/gt3vsxhrujc.html

local d = { a = 1 };  d.b = 2
来源：http://www.52xcode.cn/Article/details/gt3rhypbksi.html

[T36] Lua：函数
来源：http://www.52xcode.cn/Article/details/gt3zyilmoht.html

function add(a, b) return a + b end
来源：http://www.52xcode.cn/Article/details/gt3wlilyglc.html

[T37] Lua：字符串拼接
来源：http://www.ydjk.org.cn/Article/details/gt3xpcvsjia.html

"a" .. "b"
来源：http://www.ydjk.org.cn/Article/details/gt3wvsulyiv.html

[T38] Lua：条件
来源：http://www.52xcode.cn/Article/details/gt3tacbpgvo.html

if x > 0 then print("正") end
来源：http://www.ydjk.org.cn/Article/details/gt3ukpmxuwu.html

[T39] Lua：模式匹配
来源：http://www.52xcode.cn/Article/details/gt3sgskdzon.html

string.find(s, "%d+")
来源：http://www.52xcode.cn/Article/details/gt3issyykek.html

[T40] Lua：元表
来源：http://www.ydjk.org.cn/Article/details/gt3ocedkmod.html

setmetatable({}, { __index = base })
来源：http://www.ydjk.org.cn/Article/details/gt3xtptfygp.html

[T41] Perl：Hello World
来源：http://www.ydjk.org.cn/Article/details/gt3zblixtzv.html

print "Hello\n";
来源：http://www.ydjk.org.cn/Article/details/gt3gzybimto.html

[T42] Perl：变量类型
来源：http://www.ydjk.org.cn/Article/details/gt3vwvdfuqv.html

my $a = 1;  my @arr = (1, 2, 3);  my %h = (a => 1);
来源：http://www.52xcode.cn/Article/details/gt3thazynvr.html

[T43] Perl：字符串插值
来源：http://www.52xcode.cn/Article/details/gt3ticfktlr.html

"值: $a"
来源：http://www.52xcode.cn/Article/details/gt3mghdzhaq.html

[T44] Perl：条件
来源：http://www.52xcode.cn/Article/details/gt3vocqrexd.html

if ($a > 0) { print "正"; }
来源：http://www.ydjk.org.cn/Article/details/gt3ewkzmziz.html

[T45] Perl：数组遍历
来源：http://www.ydjk.org.cn/Article/details/gt3pyxqdvgc.html

for my $x (@arr) { print $x; }
来源：http://www.ydjk.org.cn/Article/details/gt3xkjkpsoo.html

[T46] Perl：哈希操作
来源：http://www.ydjk.org.cn/Article/details/gt3qxxoizxr.html

$h{b} = 2;  for my $k (keys %h) { print "$k=$h{$k}"; }
来源：http://www.ydjk.org.cn/Article/details/gt3pyvtwlbe.html

[T47] Perl：正则捕获
来源：http://www.ydjk.org.cn/Article/details/gt3worgmybl.html

if ($s =~ /(\d+)/) { print $1; }
来源：http://www.52xcode.cn/Article/details/gt3hpmdczup.html

[T48] Perl：正则替换
来源：http://www.52xcode.cn/Article/details/gt3lypwaawo.html

$s =~ s/old/new/g;
来源：http://www.ydjk.org.cn/Article/details/gt3qdrezqef.html

[T49] Perl：函数
来源：http://www.ydjk.org.cn/Article/details/gt3ivcrkgig.html

sub add { my ($a, $b) = @_; return $a + $b; }
来源：http://www.52xcode.cn/Article/details/gt3mcpytsvk.html

[T50] Perl：逐行读文件
来源：http://www.52xcode.cn/Article/details/gt3dtjhrtrg.html

open my $fh, "<", "a.txt" or die $!;
来源：http://www.ydjk.org.cn/Article/details/gt3ypseqcbl.html

while (my $line = <$fh>) { print $line; }
来源：http://www.52xcode.cn/Article/details/gt3dsokjcmk.html

[T51] Scala：Hello World
来源：http://www.ydjk.org.cn/Article/details/gt3lcgfmefe.html

println("Hello")
来源：http://www.ydjk.org.cn/Article/details/gt3yyzawvxf.html

[T52] Scala：变量
来源：http://www.52xcode.cn/Article/details/gt3rjvwjigu.html

val a = 1;  var b = 2
来源：http://www.52xcode.cn/Article/details/gt3lkkwzjhj.html

[T53] Scala：字符串插值
来源：http://www.ydjk.org.cn/Article/details/gt3usubidfp.html

s"值: $b"
来源：http://www.52xcode.cn/Article/details/gt3shxnjnag.html

[T54] Scala：集合映射
来源：http://www.ydjk.org.cn/Article/details/gt3rcmaknpm.html

List(1, 2, 3).map(_ * 2)
来源：http://www.52xcode.cn/Article/details/gt3uzqqnvuc.html

[T55] Scala：集合过滤
来源：http://www.ydjk.org.cn/Article/details/gt3paqbubgd.html

List(1, 2, 3).filter(_ > 1)
来源：http://www.52xcode.cn/Article/details/gt3dkhshiqv.html

[T56] Scala：样例类
来源：http://www.ydjk.org.cn/Article/details/gt3mvelfawc.html

case class User(name: String, age: Int)
来源：http://www.ydjk.org.cn/Article/details/gt3mdazxrig.html

[T57] Scala：模式匹配
来源：http://www.52xcode.cn/Article/details/gt3ghaxoodn.html

x match { case 1 => "一"; case _ => "其他" }
来源：http://www.52xcode.cn/Article/details/gt3rfrlfeyh.html

[T58] Scala：函数定义
来源：http://www.ydjk.org.cn/Article/details/gt3tlfnohgx.html

def add(a: Int, b: Int): Int = a + b
来源：http://www.52xcode.cn/Article/details/gt3padbmsrn.html

[T59] Scala：循环
来源：http://www.ydjk.org.cn/Article/details/gt3jgtrewxp.html

for (i <- 1 to 10) println(i)
来源：http://www.ydjk.org.cn/Article/details/gt3vbiubguk.html

[T60] Scala：折叠
来源：http://www.ydjk.org.cn/Article/details/gt3hqnamman.html

List(1, 2, 3).foldLeft(0)(_ + _)
来源：http://www.ydjk.org.cn/Article/details/gt3aufownrs.html

================================================================================
来源：http://www.ydjk.org.cn/Article/details/gt3klrxwhgv.html

U. 高频实用片段（Python / PHP / JavaScript 各 40 条）
来源：http://www.ydjk.org.cn/Article/details/gt3ntftdxom.html

================================================================================
来源：http://www.ydjk.org.cn/Article/details/gt3fowtynno.html

[U01] Py：创建虚拟环境
来源：http://www.ydjk.org.cn/Article/details/gt3ghpnmbrv.html

python -m venv .venv && source .venv/bin/activate
来源：http://www.52xcode.cn/Article/details/gt3czkgusfa.html

[U02] Py：导出 / 安装依赖
来源：http://www.ydjk.org.cn/Article/details/gt3ulbdodfw.html

pip freeze > requirements.txt;  pip install -r requirements.txt
来源：http://www.52xcode.cn/Article/details/gt3ofsziozy.html

[U03] Py：加载 .env 配置
来源：http://www.52xcode.cn/Article/details/gt3pfuvxntx.html

from dotenv import load_dotenv; load_dotenv()
来源：http://www.52xcode.cn/Article/details/gt3vgavsgxq.html

[U04] Py：变量调试打印
来源：http://www.ydjk.org.cn/Article/details/gt3psvkouvq.html

print(f"{x=}")            # 输出 x=值，Python 3.8+
来源：http://www.ydjk.org.cn/Article/details/gt3huyjtawy.html

[U05] Py：列表去重且保序
来源：http://www.ydjk.org.cn/Article/details/gt3vsxrjhnu.html

list(dict.fromkeys(arr))
来源：http://www.ydjk.org.cn/Article/details/gt3qoyphcmf.html

[U06] Py：合并两个字典
来源：http://www.ydjk.org.cn/Article/details/gt3cvpeslpr.html

{**a, **b}
来源：http://www.ydjk.org.cn/Article/details/gt3fsaaxdxp.html

[U07] Py：反转字典键值
来源：http://www.52xcode.cn/Article/details/gt3fsapcmza.html

{v: k for k, v in d.items()}
来源：http://www.ydjk.org.cn/Article/details/gt3pbexehjv.html

[U08] Py：展平二维列表
来源：http://www.52xcode.cn/Article/details/gt3bzyzohig.html

[y for x in nested for y in x]
来源：http://www.52xcode.cn/Article/details/gt3psqazqqb.html

[U09] Py：字典取最大值的键
来源：http://www.ydjk.org.cn/Article/details/gt3holcnntk.html

max(d, key=d.get)
来源：http://www.ydjk.org.cn/Article/details/gt3yfmoprij.html

[U10] Py：按值排序字典
来源：http://www.ydjk.org.cn/Article/details/gt3pwhurzlk.html

dict(sorted(d.items(), key=lambda kv: kv[1]))
来源：http://www.ydjk.org.cn/Article/details/gt3vzfczkmj.html

[U11] Py：生成器表达式
来源：http://www.52xcode.cn/Article/details/gt3pmgoihld.html

(x * 2 for x in arr)
来源：http://www.ydjk.org.cn/Article/details/gt3nuxamzum.html

[U12] Py：取出现最多的 3 个元素
来源：http://www.52xcode.cn/Article/details/gt3notisgfr.html

Counter(arr).most_common(3)
来源：http://www.52xcode.cn/Article/details/gt3ipxcmhuh.html

[U13] Py：固定长度队列
来源：http://www.52xcode.cn/Article/details/gt3butnrzao.html

deque(maxlen=10)
来源：http://www.52xcode.cn/Article/details/gt3jwwfvmnl.html

[U14] Py：分组收集到列表
来源：http://www.ydjk.org.cn/Article/details/gt3qltoayqa.html

defaultdict(list)
来源：http://www.ydjk.org.cn/Article/details/gt3gjkwaokb.html


<!-- 参考信息 -->