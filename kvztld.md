代发 wailian999

split -l 1000 big.log part_
来源：http://www.52xcode.cn/Article/details/gt3mgptmebg.html

[R74] 批量重命名
来源：http://www.ydjk.org.cn/Article/details/gt3wytzniww.html

for f in *.jpeg; do mv "$f" "${f%.jpeg}.jpg"; done
来源：http://www.ydjk.org.cn/Article/details/gt3saywozts.html

[R75] 导出环境变量
来源：http://www.ydjk.org.cn/Article/details/gt3arvbooom.html

export PATH="$HOME/bin:$PATH"
来源：http://www.52xcode.cn/Article/details/gt3dotlgbwh.html

[R76] 使用临时文件
来源：http://www.52xcode.cn/Article/details/gt3kagqfqfl.html

tmp=$(mktemp); trap 'rm -f "$tmp"' EXIT
来源：http://www.52xcode.cn/Article/details/gt3ecljooje.html

[R77] 读取用户输入
来源：http://www.52xcode.cn/Article/details/gt3vbfdroxe.html

read -rp "请输入: " ans
来源：http://www.52xcode.cn/Article/details/gt3tgohqvuv.html

[R78] 交互式菜单
来源：http://www.52xcode.cn/Article/details/gt3nmmzuxkf.html

select opt in a b c; do echo "$opt"; break; done
来源：http://www.52xcode.cn/Article/details/gt3csntvbyk.html

[R79] 解析命令行选项
来源：http://www.52xcode.cn/Article/details/gt3kdowoter.html

while getopts "v:f:" o; do case $o in v) V=$OPTARG ;; f) F=$OPTARG ;; esac; done
来源：http://www.ydjk.org.cn/Article/details/gt3cenbfqyd.html

[R80] 查看脚本执行耗时
来源：http://www.ydjk.org.cn/Article/details/gt3aqnsaewh.html

time ./run.sh
来源：http://www.52xcode.cn/Article/details/gt3wbiddygo.html

================================================================================
来源：http://www.52xcode.cn/Article/details/gt3enwcyzoa.html

S. C / C++ 专题
来源：http://www.ydjk.org.cn/Article/details/gt3zghvgton.html

================================================================================
来源：http://www.52xcode.cn/Article/details/gt3dpoqgmqn.html

[S01] C：Hello World
来源：http://www.52xcode.cn/Article/details/gt3jchqyblz.html

#include <stdio.h>
来源：http://www.ydjk.org.cn/Article/details/gt3jyfijraf.html

int main(void) { printf("Hello\n"); return 0; }
来源：http://www.ydjk.org.cn/Article/details/gt3upaqzcrx.html

[S02] C：变量与格式化输出
来源：http://www.ydjk.org.cn/Article/details/gt3clxzkgsw.html

int a = 10; printf("%d\n", a);
来源：http://www.ydjk.org.cn/Article/details/gt3jjimsvvc.html

[S03] C：读入整数
来源：http://www.ydjk.org.cn/Article/details/gt3vllkyvyu.html

int x; scanf("%d", &x);
来源：http://www.52xcode.cn/Article/details/gt3caiwnsqg.html

[S04] C：字符串复制
来源：http://www.ydjk.org.cn/Article/details/gt3vsnrchqe.html

char dst[32]; strcpy(dst, "hi");
来源：http://www.52xcode.cn/Article/details/gt3pbvztqus.html

[S05] C：字符串长度
来源：http://www.ydjk.org.cn/Article/details/gt3siksouho.html

strlen(s)
来源：http://www.ydjk.org.cn/Article/details/gt3gytlijkr.html

[S06] C：字符串比较
来源：http://www.ydjk.org.cn/Article/details/gt3vudaejjs.html

strcmp(a, b) == 0
来源：http://www.52xcode.cn/Article/details/gt3dlugodth.html

[S07] C：数组遍历求和
来源：http://www.52xcode.cn/Article/details/gt3toyksuig.html

for (int i = 0; i < n; i++) sum += a[i];
来源：http://www.ydjk.org.cn/Article/details/gt3pohetjoz.html

[S08] C：动态内存分配与释放
来源：http://www.ydjk.org.cn/Article/details/gt3egxdpstm.html

int *p = malloc(sizeof(int) * n); ... free(p);
来源：http://www.ydjk.org.cn/Article/details/gt3syjyqtsd.html

[S09] C：结构体定义与初始化
来源：http://www.ydjk.org.cn/Article/details/gt3ufozyobb.html

struct Point { int x, y; };  struct Point p = {1, 2};
来源：http://www.52xcode.cn/Article/details/gt3htqhmsay.html

[S10] C：指针与解引用
来源：http://www.52xcode.cn/Article/details/gt3fuvdhhlg.html

int *p = &a;  *p = 5;
来源：http://www.ydjk.org.cn/Article/details/gt3ivutttvd.html

[S11] C：逐行读文件
来源：http://www.ydjk.org.cn/Article/details/gt3pedffoxo.html

FILE *f = fopen("a.txt", "r");
来源：http://www.ydjk.org.cn/Article/details/gt3mwjmsxmq.html

while (fgets(buf, sizeof buf, f)) { }
来源：http://www.52xcode.cn/Article/details/gt3awfyaeej.html

fclose(f);
来源：http://www.52xcode.cn/Article/details/gt3qwtzvhry.html

[S12] C：写文件
来源：http://www.52xcode.cn/Article/details/gt3gqgvabbk.html

FILE *f = fopen("a.txt", "w");  fprintf(f, "hi\n");  fclose(f);
来源：http://www.ydjk.org.cn/Article/details/gt3auhlrlhd.html

[S13] C：宏定义
来源：http://www.52xcode.cn/Article/details/gt3iawrgdxs.html

#define MAX(a, b) ((a) > (b) ? (a) : (b))
来源：http://www.ydjk.org.cn/Article/details/gt3eauhsvlc.html

[S14] C：枚举
来源：http://www.ydjk.org.cn/Article/details/gt3fxlnyujj.html

enum Color { RED, GREEN, BLUE };
来源：http://www.52xcode.cn/Article/details/gt3lhzgnmxs.html

[S15] C：类型转换
来源：http://www.ydjk.org.cn/Article/details/gt3ursibjdn.html

(double) a / b
来源：http://www.ydjk.org.cn/Article/details/gt3rlzeijqc.html

[S16] C：位操作置位
来源：http://www.ydjk.org.cn/Article/details/gt3wlnpaubn.html

x |= (1 << 3);
来源：http://www.52xcode.cn/Article/details/gt3hrmlsrgp.html

[S17] C：安全拼接字符串
来源：http://www.ydjk.org.cn/Article/details/gt3chlgyeis.html

snprintf(buf, sizeof buf, "%s%s", a, b);
来源：http://www.52xcode.cn/Article/details/gt3kijcxesf.html

[S18] C：命令行参数
来源：http://www.52xcode.cn/Article/details/gt3tazftcha.html

int main(int argc, char **argv)
来源：http://www.52xcode.cn/Article/details/gt3lzrtdobn.html

[S19] C：快速排序
来源：http://www.52xcode.cn/Article/details/gt3fxadktby.html

qsort(a, n, sizeof(int), cmp);
来源：http://www.52xcode.cn/Article/details/gt3kztvxeqv.html

[S20] C：二分查找
来源：http://www.ydjk.org.cn/Article/details/gt3risllvha.html

bsearch(&key, a, n, sizeof(int), cmp);
来源：http://www.ydjk.org.cn/Article/details/gt3hdwdfjgi.html

[S21] C：字符类别判断
来源：http://www.52xcode.cn/Article/details/gt3wnzileub.html

isdigit(c);  isalpha(c);  isspace(c);
来源：http://www.ydjk.org.cn/Article/details/gt3ljzajpqk.html

[S22] C：字符串转数字
来源：http://www.ydjk.org.cn/Article/details/gt3yprasrok.html

atoi("42");  strtod("3.14", NULL);
来源：http://www.ydjk.org.cn/Article/details/gt3hiaacuue.html

[S23] C：随机数
来源：http://www.ydjk.org.cn/Article/details/gt3jbwkygdx.html

srand(time(NULL));  int r = rand() % 100;
来源：http://www.52xcode.cn/Article/details/gt3wigdlgsl.html

[S24] C：获取本地时间
来源：http://www.52xcode.cn/Article/details/gt3djfgnrkn.html

time_t t = time(NULL);  struct tm *tm = localtime(&t);
来源：http://www.ydjk.org.cn/Article/details/gt3uspdmddp.html

[S25] C：内存拷贝
来源：http://www.52xcode.cn/Article/details/gt3udqaovea.html

memcpy(dst, src, n);
来源：http://www.52xcode.cn/Article/details/gt3muwfbond.html

[S26] C：内存清零
来源：http://www.ydjk.org.cn/Article/details/gt3pfgjriwa.html

memset(a, 0, sizeof a);
来源：http://www.52xcode.cn/Article/details/gt3kthqdwdw.html

[S27] C：定义常量
来源：http://www.52xcode.cn/Article/details/gt3ufwbdmso.html

const double PI = 3.14159;
来源：http://www.52xcode.cn/Article/details/gt3mzparakj.html

[S28] C：静态变量
来源：http://www.ydjk.org.cn/Article/details/gt3pbqowvvh.html

static int counter = 0;
来源：http://www.ydjk.org.cn/Article/details/gt3shbryvcy.html

[S29] C：变参函数
来源：http://www.ydjk.org.cn/Article/details/gt3ftqdeite.html

va_list ap; va_start(ap, fmt); vprintf(fmt, ap); va_end(ap);
来源：http://www.ydjk.org.cn/Article/details/gt3rpodmqbq.html

[S30] C：头文件保护
来源：http://www.52xcode.cn/Article/details/gt3enzimyfv.html

#ifndef X_H
来源：http://www.ydjk.org.cn/Article/details/gt3oemhwthq.html

#define X_H
来源：http://www.52xcode.cn/Article/details/gt3toiirqyi.html

#endif
来源：http://www.ydjk.org.cn/Article/details/gt3juoxzrgq.html

[S31] C++：Hello World
来源：http://www.ydjk.org.cn/Article/details/gt3ikqcgzsr.html

#include <iostream>
来源：http://www.ydjk.org.cn/Article/details/gt3anmpzsbb.html

int main() { std::cout << "Hello\n"; }
来源：http://www.52xcode.cn/Article/details/gt3bejkuxzz.html

[S32] C++：字符串
来源：http://www.ydjk.org.cn/Article/details/gt3meycsfzc.html

std::string s = "hi";  s += "!";
来源：http://www.ydjk.org.cn/Article/details/gt3szhkjhef.html

[S33] C++：vector 增删
来源：http://www.52xcode.cn/Article/details/gt3zjhhcuhb.html

std::vector<int> v{1, 2, 3};  v.push_back(4);
来源：http://www.52xcode.cn/Article/details/gt3bxxhphkz.html

[S34] C++：遍历 vector
来源：http://www.ydjk.org.cn/Article/details/gt3edovvnvj.html

for (auto &x : v) { std::cout << x; }
来源：http://www.ydjk.org.cn/Article/details/gt3oqqpzued.html

[S35] C++：map
来源：http://www.52xcode.cn/Article/details/gt3atpnjtvr.html

std::map<std::string, int> m;  m["a"] = 1;
来源：http://www.52xcode.cn/Article/details/gt3tkfhfaja.html

[S36] C++：unordered_map
来源：http://www.52xcode.cn/Article/details/gt3kiomkolt.html

std::unordered_map<std::string, int> m;  m["a"] = 1;
来源：http://www.ydjk.org.cn/Article/details/gt3lvmccqru.html

[S37] C++：set
来源：http://www.52xcode.cn/Article/details/gt3xqstvftf.html

std::set<int> s{1, 2, 3};  s.insert(4);
来源：http://www.52xcode.cn/Article/details/gt3crqkyayc.html

[S38] C++：排序
来源：http://www.52xcode.cn/Article/details/gt3pfjazyip.html

std::sort(v.begin(), v.end());
来源：http://www.52xcode.cn/Article/details/gt3jyinjzre.html

[S39] C++：自定义比较器排序
来源：http://www.ydjk.org.cn/Article/details/gt3mqeiwcsa.html

std::sort(v.begin(), v.end(), [](int a, int b) { return a > b; });
来源：http://www.52xcode.cn/Article/details/gt3ialnqnlu.html

[S40] C++：查找元素
来源：http://www.52xcode.cn/Article/details/gt3ibnjwsvk.html

auto it = std::find(v.begin(), v.end(), 3);
来源：http://www.ydjk.org.cn/Article/details/gt3ogwduejt.html

[S41] C++：类与构造函数
来源：http://www.52xcode.cn/Article/details/gt3xkjykmiz.html

class A { public: A(int v) : x_(v) {} int get() const { return x_; } private: int x_; };
来源：http://www.52xcode.cn/Article/details/gt3kzwyryfg.html

[S42] C++：继承与虚函数
来源：http://www.52xcode.cn/Article/details/gt3jpqcpoby.html

class B : public Base { public: void f() override {} };
来源：http://www.52xcode.cn/Article/details/gt3jigmyeil.html

[S43] C++：智能指针
来源：http://www.52xcode.cn/Article/details/gt3cgxlvtmg.html

auto p = std::make_unique<int>(5);
来源：http://www.52xcode.cn/Article/details/gt3qfolmydy.html

[S44] C++：引用传参
来源：http://www.ydjk.org.cn/Article/details/gt3ffulgyvj.html

void inc(int &x) { ++x; }
来源：http://www.52xcode.cn/Article/details/gt3icinfkhr.html

[S45] C++：lambda
来源：http://www.ydjk.org.cn/Article/details/gt3tkbdyfor.html

auto add = [](int a, int b) { return a + b; };
来源：http://www.ydjk.org.cn/Article/details/gt3jvpwohru.html

[S46] C++：函数模板
来源：http://www.52xcode.cn/Article/details/gt3dnqfwucp.html

template <typename T> T maxv(T a, T b) { return a > b ? a : b; }
来源：http://www.52xcode.cn/Article/details/gt3gzioeopv.html

[S47] C++：结构化绑定遍历
来源：http://www.52xcode.cn/Article/details/gt3matlcexe.html

for (const auto &[k, v] : m) { std::cout << k << v; }
来源：http://www.ydjk.org.cn/Article/details/gt3qjlfkfkt.html

[S48] C++：逐行读文件
来源：http://www.ydjk.org.cn/Article/details/gt3nugemzhw.html

std::ifstream in("a.txt");  std::string line;
来源：http://www.ydjk.org.cn/Article/details/gt3caxgiars.html

while (std::getline(in, line)) { }
来源：http://www.ydjk.org.cn/Article/details/gt3cqcziinq.html

[S49] C++：写文件
来源：http://www.ydjk.org.cn/Article/details/gt3khugjyhc.html

std::ofstream out("a.txt");  out << "hi\n";
来源：http://www.52xcode.cn/Article/details/gt3umevgije.html

[S50] C++：格式化数字
来源：http://www.ydjk.org.cn/Article/details/gt3whqmmrft.html

std::ostringstream os;  os << std::fixed << std::setprecision(2) << 3.14159;
来源：http://www.ydjk.org.cn/Article/details/gt3cxuhdjou.html

[S51] C++：显式类型转换
来源：http://www.ydjk.org.cn/Article/details/gt3jleacygu.html

static_cast<double>(a) / b
来源：http://www.ydjk.org.cn/Article/details/gt3fvzqbnda.html

[S52] C++：const 与 noexcept
来源：http://www.52xcode.cn/Article/details/gt3vddxuihv.html

int size() const noexcept { return n_; }
来源：http://www.52xcode.cn/Article/details/gt3lhlkrecm.html

[S53] C++：移动语义
来源：http://www.ydjk.org.cn/Article/details/gt3lgglzdax.html

std::vector<int> w = std::move(v);
来源：http://www.ydjk.org.cn/Article/details/gt3xppcgrdm.html

[S54] C++：异常处理
来源：http://www.ydjk.org.cn/Article/details/gt3gmvmbxgi.html

try { throw std::runtime_error("x"); } catch (const std::exception &e) { }
来源：http://www.52xcode.cn/Article/details/gt3zjynvxrt.html

[S55] C++：结构化绑定
来源：http://www.52xcode.cn/Article/details/gt3xpsahqkw.html

auto [a, b] = std::make_pair(1, 2);
来源：http://www.52xcode.cn/Article/details/gt3uzxtwqqs.html

[S56] C++：optional
来源：http://www.52xcode.cn/Article/details/gt3obbytaip.html

std::optional<int> o = 5;  if (o) { int v = *o; }
来源：http://www.ydjk.org.cn/Article/details/gt3ibzavkvl.html

[S57] C++：编译期常量
来源：http://www.52xcode.cn/Article/details/gt3keqauqou.html

constexpr int N = 10;
来源：http://www.52xcode.cn/Article/details/gt3waoyrhyy.html

[S58] C++：命名空间
来源：http://www.ydjk.org.cn/Article/details/gt3mekxmhvo.html

namespace ns { int f() { return 1; } }
来源：http://www.52xcode.cn/Article/details/gt3moibqikk.html

[S59] C++：静态断言
来源：http://www.ydjk.org.cn/Article/details/gt3vqwtjnij.html

static_assert(sizeof(int) == 4, "int 必须 4 字节");
来源：http://www.52xcode.cn/Article/details/gt3gfipoynp.html

[S60] C++：遍历并删除元素
来源：http://www.52xcode.cn/Article/details/gt3kmhwnrpw.html

v.erase(std::remove_if(v.begin(), v.end(), [](int x) { return x < 0; }), v.end());
来源：http://www.ydjk.org.cn/Article/details/gt3jxisboms.html

================================================================================
来源：http://www.ydjk.org.cn/Article/details/gt3ksrrveqa.html

T. 其他语言补充（Kotlin / Swift / Lua / Perl / Scala）
来源：http://www.52xcode.cn/Article/details/gt3svdxigoc.html

================================================================================
来源：http://www.ydjk.org.cn/Article/details/gt3efuzcesb.html

[T01] Kotlin：Hello World
来源：http://www.ydjk.org.cn/Article/details/gt3sdmwumum.html

println("Hello")
来源：http://www.ydjk.org.cn/Article/details/gt3pawjhjma.html

[T02] Kotlin：变量
来源：http://www.52xcode.cn/Article/details/gt3kqgnnjro.html

val a = 1;  var b = 2        // val 只读，var 可变
来源：http://www.ydjk.org.cn/Article/details/gt3hyswzxio.html

[T03] Kotlin：字符串模板
来源：http://www.52xcode.cn/Article/details/gt3eumsbayu.html

"值: $b"
来源：http://www.52xcode.cn/Article/details/gt3hitgdcdc.html

[T04] Kotlin：空安全
来源：http://www.ydjk.org.cn/Article/details/gt3imcwzmvu.html

val n: String? = null;  n?.length
来源：http://www.ydjk.org.cn/Article/details/gt3jhaqzgof.html

[T05] Kotlin：when 表达式
来源：http://www.52xcode.cn/Article/details/gt3gibtrtqf.html

val s = when (x) { 1 -> "一" else -> "其他" }   // 多分支时每个分支单独一行
来源：http://www.52xcode.cn/Article/details/gt3nnekybph.html

[T06] Kotlin：集合映射
来源：http://www.52xcode.cn/Article/details/gt3ijrfvppu.html

listOf(1, 2, 3).map { it * 2 }
来源：http://www.ydjk.org.cn/Article/details/gt3ysxdvwoz.html

[T07] Kotlin：集合过滤
来源：http://www.ydjk.org.cn/Article/details/gt3cvdhfklc.html

listOf(1, 2, 3).filter { it > 1 }
来源：http://www.ydjk.org.cn/Article/details/gt3uozksbtb.html

[T08] Kotlin：数据类
来源：http://www.ydjk.org.cn/Article/details/gt3amglqqxh.html

data class User(val name: String, val age: Int)
来源：http://www.52xcode.cn/Article/details/gt3cgmxcvgg.html

[T09] Kotlin：扩展函数
来源：http://www.ydjk.org.cn/Article/details/gt3tcxdxufo.html

fun String.exclaim() = this + "!"
来源：http://www.ydjk.org.cn/Article/details/gt3vnoeuvaz.html

[T10] Kotlin：默认参数
来源：http://www.52xcode.cn/Article/details/gt3wfrmawje.html

fun greet(name: String = "World") = "Hi $name"
来源：http://www.52xcode.cn/Article/details/gt3dxvgfvys.html

[T11] Kotlin：协程
来源：http://www.ydjk.org.cn/Article/details/gt3dkwxvimu.html

GlobalScope.launch { delay(1000); println("done") }
来源：http://www.ydjk.org.cn/Article/details/gt3brljytpb.html

[T12] Kotlin：解构声明
来源：http://www.52xcode.cn/Article/details/gt3wcxveomu.html

val (a, b) = Pair(1, 2)
来源：http://www.ydjk.org.cn/Article/details/gt3fmbljtou.html

[T13] Kotlin：只读 Map
来源：http://www.ydjk.org.cn/Article/details/gt3gindyahc.html

val m = mapOf("a" to 1)
来源：http://www.ydjk.org.cn/Article/details/gt3yttatoil.html

[T14] Kotlin：循环
来源：http://www.ydjk.org.cn/Article/details/gt3pjuunkac.html

for (i in 1..10) println(i)
来源：http://www.ydjk.org.cn/Article/details/gt3bkchfkqe.html

[T15] Kotlin：接口
来源：http://www.52xcode.cn/Article/details/gt3ojofpjhp.html

interface Shape { fun area(): Double }
来源：http://www.ydjk.org.cn/Article/details/gt3gyqskkap.html

[T16] Swift：Hello World
来源：http://www.ydjk.org.cn/Article/details/gt3wsleptck.html

print("Hello")
来源：http://www.52xcode.cn/Article/details/gt3hrzjucok.html

[T17] Swift：变量与常量
来源：http://www.ydjk.org.cn/Article/details/gt3pbvurffb.html

var a = 1;  let b = 2
来源：http://www.52xcode.cn/Article/details/gt3unrhcqfx.html

[T18] Swift：字符串插值
来源：http://www.52xcode.cn/Article/details/gt3ofcuncjb.html

"值: \(b)"
来源：http://www.52xcode.cn/Article/details/gt3agjpusmr.html

[T19] Swift：可选绑定
来源：http://www.ydjk.org.cn/Article/details/gt3honwfguq.html

if let n = opt { print(n) }
来源：http://www.52xcode.cn/Article/details/gt3vwcabxyh.html

[T20] Swift：数组操作
来源：http://www.ydjk.org.cn/Article/details/gt3xqjnecbd.html

var a = [1, 2, 3];  a.append(4)
来源：http://www.52xcode.cn/Article/details/gt3dfygfvgn.html

[T21] Swift：遍历
来源：http://www.52xcode.cn/Article/details/gt3exwtyjei.html

for x in a { print(x) }
来源：http://www.ydjk.org.cn/Article/details/gt3vixmzthc.html

[T22] Swift：字典
来源：http://www.52xcode.cn/Article/details/gt3qujrecnd.html

var d = ["a": 1];  d["b"] = 2
来源：http://www.52xcode.cn/Article/details/gt3zaeogevn.html

[T23] Swift：函数
来源：http://www.52xcode.cn/Article/details/gt3teqvrvdz.html

func add(_ a: Int, _ b: Int) -> Int { a + b }
来源：http://www.ydjk.org.cn/Article/details/gt3fckffbfu.html

[T24] Swift：闭包
来源：http://www.52xcode.cn/Article/details/gt3eqznmylw.html

let f = { (x: Int) -> Int in x * 2 }
来源：http://www.ydjk.org.cn/Article/details/gt3fiwxrufz.html

[T25] Swift：结构体
来源：http://www.52xcode.cn/Article/details/gt3npvtpsdp.html

struct P { var x: Int }
来源：http://www.ydjk.org.cn/Article/details/gt3jduvmxei.html

[T26] Swift：类与重写
来源：http://www.ydjk.org.cn/Article/details/gt3twulmird.html

class A: Base { override func f() {} }
来源：http://www.ydjk.org.cn/Article/details/gt3nsmbqlgd.html

[T27] Swift：错误处理
来源：http://www.ydjk.org.cn/Article/details/gt3jfvfxdad.html

do { try f() } catch { print(error) }
来源：http://www.ydjk.org.cn/Article/details/gt3rvbvbdnh.html

[T28] Swift：枚举
来源：http://www.ydjk.org.cn/Article/details/gt3zgffzvns.html

enum Color { case red, green }
来源：http://www.ydjk.org.cn/Article/details/gt3mvbamvjk.html

[T29] Swift：guard 提前返回
来源：http://www.ydjk.org.cn/Article/details/gt3njovomft.html

guard let x = opt else { return }
来源：http://www.52xcode.cn/Article/details/gt3knqbfsaz.html

[T30] Swift：协议
来源：http://www.52xcode.cn/Article/details/gt3chstmqui.html

protocol Shape { func area() -> Double }
来源：http://www.ydjk.org.cn/Article/details/gt3bkjtuigj.html

[T31] Lua：Hello World
来源：http://www.52xcode.cn/Article/details/gt3ldppwyhp.html

print("Hello")
来源：http://www.ydjk.org.cn/Article/details/gt3dosvygxp.html

[T32] Lua：局部变量
来源：http://www.ydjk.org.cn/Article/details/gt3ennxtegr.html

local a = 1
来源：http://www.52xcode.cn/Article/details/gt3hasosldv.html

[T33] Lua：表（数组）
来源：http://www.ydjk.org.cn/Article/details/gt3nqmvjymv.html

local t = {1, 2, 3};  t[4] = 4
来源：http://www.ydjk.org.cn/Article/details/gt3gmlrerte.html

[T34] Lua：遍历表
来源：http://www.ydjk.org.cn/Article/details/gt3rnsnnyxv.html

for i, v in ipairs(t) do print(i, v) end
来源：http://www.52xcode.cn/Article/details/gt3jihbhgrr.html

[T35] Lua：字典表
来源：http://www.ydjk.org.cn/Article/details/gt3mmfkwwnj.html

local d = { a = 1 };  d.b = 2
来源：http://www.52xcode.cn/Article/details/gt3cgmkxzaj.html

[T36] Lua：函数
来源：http://www.ydjk.org.cn/Article/details/gt3zyvemayy.html

function add(a, b) return a + b end
来源：http://www.52xcode.cn/Article/details/gt3mqarlytd.html

[T37] Lua：字符串拼接
来源：http://www.ydjk.org.cn/Article/details/gt3ghdqgrfw.html

"a" .. "b"
来源：http://www.ydjk.org.cn/Article/details/gt3vhlcouko.html

[T38] Lua：条件
来源：http://www.ydjk.org.cn/Article/details/gt3kfiycett.html

if x > 0 then print("正") end
来源：http://www.52xcode.cn/Article/details/gt3lijhifat.html

[T39] Lua：模式匹配
来源：http://www.ydjk.org.cn/Article/details/gt3genfbuaw.html

string.find(s, "%d+")
来源：http://www.ydjk.org.cn/Article/details/gt3eywchpuj.html

[T40] Lua：元表
来源：http://www.52xcode.cn/Article/details/gt3mfkkwnav.html

setmetatable({}, { __index = base })
来源：http://www.52xcode.cn/Article/details/gt3indjibiy.html

[T41] Perl：Hello World
来源：http://www.52xcode.cn/Article/details/gt3uifyjeao.html

print "Hello\n";
来源：http://www.ydjk.org.cn/Article/details/gt3tznchbre.html

[T42] Perl：变量类型
来源：http://www.52xcode.cn/Article/details/gt3krvmawff.html

my $a = 1;  my @arr = (1, 2, 3);  my %h = (a => 1);
来源：http://www.52xcode.cn/Article/details/gt3azhszheb.html

[T43] Perl：字符串插值
来源：http://www.52xcode.cn/Article/details/gt3mudtmkrs.html

"值: $a"
来源：http://www.ydjk.org.cn/Article/details/gt3grkmficd.html

[T44] Perl：条件
来源：http://www.52xcode.cn/Article/details/gt3tofapujj.html

if ($a > 0) { print "正"; }
来源：http://www.52xcode.cn/Article/details/gt3joedwesf.html

[T45] Perl：数组遍历
来源：http://www.52xcode.cn/Article/details/gt3rxxzzhma.html

for my $x (@arr) { print $x; }
来源：http://www.ydjk.org.cn/Article/details/gt3kjmewwvx.html

[T46] Perl：哈希操作
来源：http://www.52xcode.cn/Article/details/gt3wcuscaul.html

$h{b} = 2;  for my $k (keys %h) { print "$k=$h{$k}"; }
来源：http://www.52xcode.cn/Article/details/gt3bbpgnryt.html

[T47] Perl：正则捕获
来源：http://www.52xcode.cn/Article/details/gt3bgsorgly.html

if ($s =~ /(\d+)/) { print $1; }
来源：http://www.52xcode.cn/Article/details/gt3bitojsxc.html

[T48] Perl：正则替换
来源：http://www.52xcode.cn/Article/details/gt3nlfndoma.html

$s =~ s/old/new/g;
来源：http://www.ydjk.org.cn/Article/details/gt3gpmxshvp.html

[T49] Perl：函数
来源：http://www.ydjk.org.cn/Article/details/gt3kfsozhnx.html

sub add { my ($a, $b) = @_; return $a + $b; }
来源：http://www.52xcode.cn/Article/details/gt3gabtypvj.html

[T50] Perl：逐行读文件
来源：http://www.ydjk.org.cn/Article/details/gt3imzjaxda.html

open my $fh, "<", "a.txt" or die $!;
来源：http://www.ydjk.org.cn/Article/details/gt3knczqeky.html

while (my $line = <$fh>) { print $line; }
来源：http://www.52xcode.cn/Article/details/gt3wdjnkcuf.html

[T51] Scala：Hello World
来源：http://www.52xcode.cn/Article/details/gt3nlzkuavb.html

println("Hello")
来源：http://www.ydjk.org.cn/Article/details/gt3qpboxzgl.html

[T52] Scala：变量
来源：http://www.ydjk.org.cn/Article/details/gt3vaebgiug.html

val a = 1;  var b = 2
来源：http://www.52xcode.cn/Article/details/gt3bwskqxnl.html

[T53] Scala：字符串插值
来源：http://www.ydjk.org.cn/Article/details/gt3avyrufdl.html

s"值: $b"
来源：http://www.ydjk.org.cn/Article/details/gt3mlzmsbua.html

[T54] Scala：集合映射
来源：http://www.ydjk.org.cn/Article/details/gt3bqruzzid.html

List(1, 2, 3).map(_ * 2)
来源：http://www.52xcode.cn/Article/details/gt3iorrzdcp.html

[T55] Scala：集合过滤
来源：http://www.52xcode.cn/Article/details/gt3aqnmettb.html

List(1, 2, 3).filter(_ > 1)
来源：http://www.52xcode.cn/Article/details/gt3yduwygvt.html

[T56] Scala：样例类
来源：http://www.52xcode.cn/Article/details/gt3furiiglz.html

case class User(name: String, age: Int)
来源：http://www.52xcode.cn/Article/details/gt3gqszkejy.html

[T57] Scala：模式匹配
来源：http://www.52xcode.cn/Article/details/gt3pzmuflzx.html

x match { case 1 => "一"; case _ => "其他" }
来源：http://www.52xcode.cn/Article/details/gt3snawsjsv.html

[T58] Scala：函数定义
来源：http://www.52xcode.cn/Article/details/gt3qpxtwdyp.html

def add(a: Int, b: Int): Int = a + b
来源：http://www.ydjk.org.cn/Article/details/gt3chzbscwm.html

[T59] Scala：循环
来源：http://www.52xcode.cn/Article/details/gt3hizpffzi.html

for (i <- 1 to 10) println(i)
来源：http://www.ydjk.org.cn/Article/details/gt3eoioamra.html

[T60] Scala：折叠
来源：http://www.ydjk.org.cn/Article/details/gt3zwilghgz.html

List(1, 2, 3).foldLeft(0)(_ + _)
来源：http://www.52xcode.cn/Article/details/gt3xotjkmbp.html

================================================================================
来源：http://www.ydjk.org.cn/Article/details/gt3apcoeofx.html

U. 高频实用片段（Python / PHP / JavaScript 各 40 条）
来源：http://www.52xcode.cn/Article/details/gt3zjemxiyz.html

================================================================================
来源：http://www.52xcode.cn/Article/details/gt3erwykakk.html

[U01] Py：创建虚拟环境
来源：http://www.52xcode.cn/Article/details/gt3bioozoaf.html

python -m venv .venv && source .venv/bin/activate
来源：http://www.52xcode.cn/Article/details/gt3fhxyjils.html

[U02] Py：导出 / 安装依赖
来源：http://www.52xcode.cn/Article/details/gt3mqgpimzw.html

pip freeze > requirements.txt;  pip install -r requirements.txt
来源：http://www.52xcode.cn/Article/details/gt3euatfwvg.html

[U03] Py：加载 .env 配置
来源：http://www.ydjk.org.cn/Article/details/gt3pfounchz.html

from dotenv import load_dotenv; load_dotenv()
来源：http://www.ydjk.org.cn/Article/details/gt3wxlullox.html

[U04] Py：变量调试打印
来源：http://www.52xcode.cn/Article/details/gt3dfzccimi.html

print(f"{x=}")            # 输出 x=值，Python 3.8+
来源：http://www.ydjk.org.cn/Article/details/gt3fjlqwwyp.html

[U05] Py：列表去重且保序
来源：http://www.52xcode.cn/Article/details/gt3hujvgrqc.html

list(dict.fromkeys(arr))
来源：http://www.ydjk.org.cn/Article/details/gt3hxrlfkhf.html

[U06] Py：合并两个字典
来源：http://www.52xcode.cn/Article/details/gt3jgpvozij.html

{**a, **b}
来源：http://www.52xcode.cn/Article/details/gt3noibtvyp.html

[U07] Py：反转字典键值
来源：http://www.52xcode.cn/Article/details/gt3pacbzdsu.html

{v: k for k, v in d.items()}
来源：http://www.ydjk.org.cn/Article/details/gt3nstesvdp.html

[U08] Py：展平二维列表
来源：http://www.52xcode.cn/Article/details/gt3amgeudsi.html

[y for x in nested for y in x]
来源：http://www.ydjk.org.cn/Article/details/gt3cruzedqc.html

[U09] Py：字典取最大值的键
来源：http://www.ydjk.org.cn/Article/details/gt3pflfwsnh.html

max(d, key=d.get)
来源：http://www.ydjk.org.cn/Article/details/gt3vimkqtyb.html

[U10] Py：按值排序字典
来源：http://www.52xcode.cn/Article/details/gt3uwgynfvj.html

dict(sorted(d.items(), key=lambda kv: kv[1]))
来源：http://www.ydjk.org.cn/Article/details/gt3bbqqwhpl.html

[U11] Py：生成器表达式
来源：http://www.52xcode.cn/Article/details/gt3cactfhyg.html

(x * 2 for x in arr)
来源：http://www.52xcode.cn/Article/details/gt3moydxvas.html

[U12] Py：取出现最多的 3 个元素
来源：http://www.52xcode.cn/Article/details/gt3vncqdkvy.html

Counter(arr).most_common(3)
来源：http://www.52xcode.cn/Article/details/gt3tjreuexx.html

[U13] Py：固定长度队列
来源：http://www.ydjk.org.cn/Article/details/gt3hoxtylmu.html

deque(maxlen=10)
来源：http://www.52xcode.cn/Article/details/gt3agthcebp.html

[U14] Py：分组收集到列表
来源：http://www.52xcode.cn/Article/details/gt3qwhdicom.html

defaultdict(list)
来源：http://www.52xcode.cn/Article/details/gt3aabcvbpi.html


<!-- 参考信息 -->