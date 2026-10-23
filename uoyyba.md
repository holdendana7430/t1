代发 wailian999

split -l 1000 big.log part_
来源：http://www.52xcode.cn/Article/details/gt3juvrofqp.html

[R74] 批量重命名
来源：http://www.ydjk.org.cn/Article/details/gt3rifuunfm.html

for f in *.jpeg; do mv "$f" "${f%.jpeg}.jpg"; done
来源：http://www.ydjk.org.cn/Article/details/gt3njdyuvym.html

[R75] 导出环境变量
来源：http://www.ydjk.org.cn/Article/details/gt3wkoslmeg.html

export PATH="$HOME/bin:$PATH"
来源：http://www.ydjk.org.cn/Article/details/gt3pqyhfhad.html

[R76] 使用临时文件
来源：http://www.ydjk.org.cn/Article/details/gt3zemwmdca.html

tmp=$(mktemp); trap 'rm -f "$tmp"' EXIT
来源：http://www.52xcode.cn/Article/details/gt3hzdbgkeu.html

[R77] 读取用户输入
来源：http://www.52xcode.cn/Article/details/gt3rhjbfybl.html

read -rp "请输入: " ans
来源：http://www.ydjk.org.cn/Article/details/gt3oyrhgefk.html

[R78] 交互式菜单
来源：http://www.52xcode.cn/Article/details/gt3otyccmja.html

select opt in a b c; do echo "$opt"; break; done
来源：http://www.52xcode.cn/Article/details/gt3giwebcco.html

[R79] 解析命令行选项
来源：http://www.52xcode.cn/Article/details/gt3jwvuteer.html

while getopts "v:f:" o; do case $o in v) V=$OPTARG ;; f) F=$OPTARG ;; esac; done
来源：http://www.ydjk.org.cn/Article/details/gt3gybtvavw.html

[R80] 查看脚本执行耗时
来源：http://www.52xcode.cn/Article/details/gt3kbjpzziw.html

time ./run.sh
来源：http://www.52xcode.cn/Article/details/gt3hrienwwq.html

================================================================================
来源：http://www.52xcode.cn/Article/details/gt3tzxsvwto.html

S. C / C++ 专题
来源：http://www.ydjk.org.cn/Article/details/gt3ixnwivat.html

================================================================================
来源：http://www.52xcode.cn/Article/details/gt3zfzmmozm.html

[S01] C：Hello World
来源：http://www.ydjk.org.cn/Article/details/gt3mvhntcql.html

#include <stdio.h>
来源：http://www.52xcode.cn/Article/details/gt3iuujeyfr.html

int main(void) { printf("Hello\n"); return 0; }
来源：http://www.ydjk.org.cn/Article/details/gt3rkmkykib.html

[S02] C：变量与格式化输出
来源：http://www.ydjk.org.cn/Article/details/gt3qqhmysll.html

int a = 10; printf("%d\n", a);
来源：http://www.ydjk.org.cn/Article/details/gt3imbpakmf.html

[S03] C：读入整数
来源：http://www.ydjk.org.cn/Article/details/gt3oycwzvfj.html

int x; scanf("%d", &x);
来源：http://www.52xcode.cn/Article/details/gt3rtysyspg.html

[S04] C：字符串复制
来源：http://www.52xcode.cn/Article/details/gt3qpzhwvpj.html

char dst[32]; strcpy(dst, "hi");
来源：http://www.ydjk.org.cn/Article/details/gt3xgjvafet.html

[S05] C：字符串长度
来源：http://www.ydjk.org.cn/Article/details/gt3sjynvrad.html

strlen(s)
来源：http://www.52xcode.cn/Article/details/gt3ynpysmpn.html

[S06] C：字符串比较
来源：http://www.ydjk.org.cn/Article/details/gt3yrcihyxm.html

strcmp(a, b) == 0
来源：http://www.ydjk.org.cn/Article/details/gt3zcgyctae.html

[S07] C：数组遍历求和
来源：http://www.ydjk.org.cn/Article/details/gt3ptysgkgs.html

for (int i = 0; i < n; i++) sum += a[i];
来源：http://www.ydjk.org.cn/Article/details/gt3bcsmcumh.html

[S08] C：动态内存分配与释放
来源：http://www.52xcode.cn/Article/details/gt3apucwbmf.html

int *p = malloc(sizeof(int) * n); ... free(p);
来源：http://www.ydjk.org.cn/Article/details/gt3vfzngilo.html

[S09] C：结构体定义与初始化
来源：http://www.52xcode.cn/Article/details/gt3qmdxbuqi.html

struct Point { int x, y; };  struct Point p = {1, 2};
来源：http://www.ydjk.org.cn/Article/details/gt3fqiwvnoo.html

[S10] C：指针与解引用
来源：http://www.52xcode.cn/Article/details/gt3wnaqudod.html

int *p = &a;  *p = 5;
来源：http://www.52xcode.cn/Article/details/gt3yccdppse.html

[S11] C：逐行读文件
来源：http://www.52xcode.cn/Article/details/gt3jgcdhfof.html

FILE *f = fopen("a.txt", "r");
来源：http://www.52xcode.cn/Article/details/gt3eloyurug.html

while (fgets(buf, sizeof buf, f)) { }
来源：http://www.52xcode.cn/Article/details/gt3xbcyimng.html

fclose(f);
来源：http://www.ydjk.org.cn/Article/details/gt3uywysorb.html

[S12] C：写文件
来源：http://www.ydjk.org.cn/Article/details/gt3bqqjhojk.html

FILE *f = fopen("a.txt", "w");  fprintf(f, "hi\n");  fclose(f);
来源：http://www.ydjk.org.cn/Article/details/gt3vlqvqgrx.html

[S13] C：宏定义
来源：http://www.52xcode.cn/Article/details/gt3xycveztl.html

#define MAX(a, b) ((a) > (b) ? (a) : (b))
来源：http://www.52xcode.cn/Article/details/gt3fihajnkn.html

[S14] C：枚举
来源：http://www.ydjk.org.cn/Article/details/gt3fgcahjdd.html

enum Color { RED, GREEN, BLUE };
来源：http://www.ydjk.org.cn/Article/details/gt3ovcjgfjr.html

[S15] C：类型转换
来源：http://www.ydjk.org.cn/Article/details/gt3hzipedra.html

(double) a / b
来源：http://www.ydjk.org.cn/Article/details/gt3hlmgzgie.html

[S16] C：位操作置位
来源：http://www.52xcode.cn/Article/details/gt3dhpsazyy.html

x |= (1 << 3);
来源：http://www.ydjk.org.cn/Article/details/gt3mvwtyknl.html

[S17] C：安全拼接字符串
来源：http://www.ydjk.org.cn/Article/details/gt3uvdkdtyf.html

snprintf(buf, sizeof buf, "%s%s", a, b);
来源：http://www.ydjk.org.cn/Article/details/gt3jobguvey.html

[S18] C：命令行参数
来源：http://www.ydjk.org.cn/Article/details/gt3lxnezwmt.html

int main(int argc, char **argv)
来源：http://www.52xcode.cn/Article/details/gt3qxacidll.html

[S19] C：快速排序
来源：http://www.ydjk.org.cn/Article/details/gt3djtgfjbt.html

qsort(a, n, sizeof(int), cmp);
来源：http://www.52xcode.cn/Article/details/gt3ayfqhizv.html

[S20] C：二分查找
来源：http://www.52xcode.cn/Article/details/gt3owguhxjw.html

bsearch(&key, a, n, sizeof(int), cmp);
来源：http://www.ydjk.org.cn/Article/details/gt3cjczhigk.html

[S21] C：字符类别判断
来源：http://www.52xcode.cn/Article/details/gt3sfhjqdph.html

isdigit(c);  isalpha(c);  isspace(c);
来源：http://www.52xcode.cn/Article/details/gt3szbijsnb.html

[S22] C：字符串转数字
来源：http://www.52xcode.cn/Article/details/gt3hdmdttbu.html

atoi("42");  strtod("3.14", NULL);
来源：http://www.52xcode.cn/Article/details/gt3rysdxshs.html

[S23] C：随机数
来源：http://www.52xcode.cn/Article/details/gt3hvgtbfvq.html

srand(time(NULL));  int r = rand() % 100;
来源：http://www.ydjk.org.cn/Article/details/gt3mtenftwj.html

[S24] C：获取本地时间
来源：http://www.52xcode.cn/Article/details/gt3afqqvnaa.html

time_t t = time(NULL);  struct tm *tm = localtime(&t);
来源：http://www.ydjk.org.cn/Article/details/gt3cqgoibwu.html

[S25] C：内存拷贝
来源：http://www.ydjk.org.cn/Article/details/gt3txjpkwdh.html

memcpy(dst, src, n);
来源：http://www.52xcode.cn/Article/details/gt3kyonvjyd.html

[S26] C：内存清零
来源：http://www.ydjk.org.cn/Article/details/gt3thvyzphl.html

memset(a, 0, sizeof a);
来源：http://www.52xcode.cn/Article/details/gt3rawmecpe.html

[S27] C：定义常量
来源：http://www.ydjk.org.cn/Article/details/gt3rvhywpjj.html

const double PI = 3.14159;
来源：http://www.52xcode.cn/Article/details/gt3kdqsoguz.html

[S28] C：静态变量
来源：http://www.ydjk.org.cn/Article/details/gt3kgyoipji.html

static int counter = 0;
来源：http://www.52xcode.cn/Article/details/gt3mmxwwtcv.html

[S29] C：变参函数
来源：http://www.52xcode.cn/Article/details/gt3wspwbrhl.html

va_list ap; va_start(ap, fmt); vprintf(fmt, ap); va_end(ap);
来源：http://www.52xcode.cn/Article/details/gt3jqhbawwh.html

[S30] C：头文件保护
来源：http://www.ydjk.org.cn/Article/details/gt3pdhsgdys.html

#ifndef X_H
来源：http://www.52xcode.cn/Article/details/gt3nrxljbfw.html

#define X_H
来源：http://www.ydjk.org.cn/Article/details/gt3zoryxqeo.html

#endif
来源：http://www.52xcode.cn/Article/details/gt3ilhnzbek.html

[S31] C++：Hello World
来源：http://www.52xcode.cn/Article/details/gt3blvrymyr.html

#include <iostream>
来源：http://www.52xcode.cn/Article/details/gt3piqmjsxb.html

int main() { std::cout << "Hello\n"; }
来源：http://www.ydjk.org.cn/Article/details/gt3tjdpavum.html

[S32] C++：字符串
来源：http://www.ydjk.org.cn/Article/details/gt3opxexlrh.html

std::string s = "hi";  s += "!";
来源：http://www.52xcode.cn/Article/details/gt3dwhhoarj.html

[S33] C++：vector 增删
来源：http://www.ydjk.org.cn/Article/details/gt3mkjifkkh.html

std::vector<int> v{1, 2, 3};  v.push_back(4);
来源：http://www.ydjk.org.cn/Article/details/gt3koqejqil.html

[S34] C++：遍历 vector
来源：http://www.ydjk.org.cn/Article/details/gt3rvhreocg.html

for (auto &x : v) { std::cout << x; }
来源：http://www.ydjk.org.cn/Article/details/gt3nskebnuq.html

[S35] C++：map
来源：http://www.52xcode.cn/Article/details/gt3bxcwyjfl.html

std::map<std::string, int> m;  m["a"] = 1;
来源：http://www.52xcode.cn/Article/details/gt3lhjbkegv.html

[S36] C++：unordered_map
来源：http://www.52xcode.cn/Article/details/gt3ajmabhkz.html

std::unordered_map<std::string, int> m;  m["a"] = 1;
来源：http://www.ydjk.org.cn/Article/details/gt3nfbrpiah.html

[S37] C++：set
来源：http://www.52xcode.cn/Article/details/gt3pvccpxib.html

std::set<int> s{1, 2, 3};  s.insert(4);
来源：http://www.ydjk.org.cn/Article/details/gt3bkkfhilc.html

[S38] C++：排序
来源：http://www.ydjk.org.cn/Article/details/gt3pjahuitz.html

std::sort(v.begin(), v.end());
来源：http://www.52xcode.cn/Article/details/gt3nyubqgag.html

[S39] C++：自定义比较器排序
来源：http://www.ydjk.org.cn/Article/details/gt3azinjrew.html

std::sort(v.begin(), v.end(), [](int a, int b) { return a > b; });
来源：http://www.ydjk.org.cn/Article/details/gt3wzjkyehl.html

[S40] C++：查找元素
来源：http://www.ydjk.org.cn/Article/details/gt3yucdcyrd.html

auto it = std::find(v.begin(), v.end(), 3);
来源：http://www.ydjk.org.cn/Article/details/gt3vlqtouxf.html

[S41] C++：类与构造函数
来源：http://www.52xcode.cn/Article/details/gt3wefeglmc.html

class A { public: A(int v) : x_(v) {} int get() const { return x_; } private: int x_; };
来源：http://www.ydjk.org.cn/Article/details/gt3fonrgpqn.html

[S42] C++：继承与虚函数
来源：http://www.ydjk.org.cn/Article/details/gt3myvjohoa.html

class B : public Base { public: void f() override {} };
来源：http://www.ydjk.org.cn/Article/details/gt3arrwqlvb.html

[S43] C++：智能指针
来源：http://www.52xcode.cn/Article/details/gt3vcyptvji.html

auto p = std::make_unique<int>(5);
来源：http://www.52xcode.cn/Article/details/gt3oltcarri.html

[S44] C++：引用传参
来源：http://www.52xcode.cn/Article/details/gt3pynntzqq.html

void inc(int &x) { ++x; }
来源：http://www.52xcode.cn/Article/details/gt3ohqcsgtv.html

[S45] C++：lambda
来源：http://www.ydjk.org.cn/Article/details/gt3qrhigyyw.html

auto add = [](int a, int b) { return a + b; };
来源：http://www.ydjk.org.cn/Article/details/gt3aiwzlhju.html

[S46] C++：函数模板
来源：http://www.52xcode.cn/Article/details/gt3buftvdbh.html

template <typename T> T maxv(T a, T b) { return a > b ? a : b; }
来源：http://www.ydjk.org.cn/Article/details/gt3nrdqxhdq.html

[S47] C++：结构化绑定遍历
来源：http://www.52xcode.cn/Article/details/gt3gqtunxhx.html

for (const auto &[k, v] : m) { std::cout << k << v; }
来源：http://www.52xcode.cn/Article/details/gt3nkidqcip.html

[S48] C++：逐行读文件
来源：http://www.52xcode.cn/Article/details/gt3ynplvgml.html

std::ifstream in("a.txt");  std::string line;
来源：http://www.ydjk.org.cn/Article/details/gt3rarinqlj.html

while (std::getline(in, line)) { }
来源：http://www.ydjk.org.cn/Article/details/gt3nphxkeza.html

[S49] C++：写文件
来源：http://www.ydjk.org.cn/Article/details/gt3lpldbtrm.html

std::ofstream out("a.txt");  out << "hi\n";
来源：http://www.ydjk.org.cn/Article/details/gt3pwucmkin.html

[S50] C++：格式化数字
来源：http://www.ydjk.org.cn/Article/details/gt3qzaocmmm.html

std::ostringstream os;  os << std::fixed << std::setprecision(2) << 3.14159;
来源：http://www.52xcode.cn/Article/details/gt3clwgfxgu.html

[S51] C++：显式类型转换
来源：http://www.52xcode.cn/Article/details/gt3sqdkmhxl.html

static_cast<double>(a) / b
来源：http://www.ydjk.org.cn/Article/details/gt3omcsbdwx.html

[S52] C++：const 与 noexcept
来源：http://www.ydjk.org.cn/Article/details/gt3iyfahdxg.html

int size() const noexcept { return n_; }
来源：http://www.52xcode.cn/Article/details/gt3cenjxcfd.html

[S53] C++：移动语义
来源：http://www.52xcode.cn/Article/details/gt3wryxwqfu.html

std::vector<int> w = std::move(v);
来源：http://www.52xcode.cn/Article/details/gt3vvlxzqtu.html

[S54] C++：异常处理
来源：http://www.52xcode.cn/Article/details/gt3afamizqy.html

try { throw std::runtime_error("x"); } catch (const std::exception &e) { }
来源：http://www.ydjk.org.cn/Article/details/gt3flevwlud.html

[S55] C++：结构化绑定
来源：http://www.ydjk.org.cn/Article/details/gt3jadsmaql.html

auto [a, b] = std::make_pair(1, 2);
来源：http://www.52xcode.cn/Article/details/gt3pjuuvoxx.html

[S56] C++：optional
来源：http://www.ydjk.org.cn/Article/details/gt3kfhnxzme.html

std::optional<int> o = 5;  if (o) { int v = *o; }
来源：http://www.ydjk.org.cn/Article/details/gt3tgcsawhc.html

[S57] C++：编译期常量
来源：http://www.ydjk.org.cn/Article/details/gt3dzisanid.html

constexpr int N = 10;
来源：http://www.ydjk.org.cn/Article/details/gt3ssoihlwi.html

[S58] C++：命名空间
来源：http://www.52xcode.cn/Article/details/gt3aglslvxe.html

namespace ns { int f() { return 1; } }
来源：http://www.ydjk.org.cn/Article/details/gt3jffunaht.html

[S59] C++：静态断言
来源：http://www.ydjk.org.cn/Article/details/gt3saievysw.html

static_assert(sizeof(int) == 4, "int 必须 4 字节");
来源：http://www.52xcode.cn/Article/details/gt3lnjhfirp.html

[S60] C++：遍历并删除元素
来源：http://www.ydjk.org.cn/Article/details/gt3anvguujf.html

v.erase(std::remove_if(v.begin(), v.end(), [](int x) { return x < 0; }), v.end());
来源：http://www.52xcode.cn/Article/details/gt3uezpudyr.html

================================================================================
来源：http://www.ydjk.org.cn/Article/details/gt3zfmyvdnb.html

T. 其他语言补充（Kotlin / Swift / Lua / Perl / Scala）
来源：http://www.ydjk.org.cn/Article/details/gt3nmesccmc.html

================================================================================
来源：http://www.52xcode.cn/Article/details/gt3hsnpzqnb.html

[T01] Kotlin：Hello World
来源：http://www.52xcode.cn/Article/details/gt3obmpxtht.html

println("Hello")
来源：http://www.52xcode.cn/Article/details/gt3hzdevrhn.html

[T02] Kotlin：变量
来源：http://www.ydjk.org.cn/Article/details/gt3lefsgmfj.html

val a = 1;  var b = 2        // val 只读，var 可变
来源：http://www.52xcode.cn/Article/details/gt3bbfvatlq.html

[T03] Kotlin：字符串模板
来源：http://www.52xcode.cn/Article/details/gt3eymuidkj.html

"值: $b"
来源：http://www.ydjk.org.cn/Article/details/gt3cponqcwl.html

[T04] Kotlin：空安全
来源：http://www.52xcode.cn/Article/details/gt3icwjpdtn.html

val n: String? = null;  n?.length
来源：http://www.ydjk.org.cn/Article/details/gt3sichtipu.html

[T05] Kotlin：when 表达式
来源：http://www.52xcode.cn/Article/details/gt3gcxcfisc.html

val s = when (x) { 1 -> "一" else -> "其他" }   // 多分支时每个分支单独一行
来源：http://www.52xcode.cn/Article/details/gt3wklucaky.html

[T06] Kotlin：集合映射
来源：http://www.52xcode.cn/Article/details/gt3vlvnethq.html

listOf(1, 2, 3).map { it * 2 }
来源：http://www.52xcode.cn/Article/details/gt3fmubmrzm.html

[T07] Kotlin：集合过滤
来源：http://www.52xcode.cn/Article/details/gt3btolvlqn.html

listOf(1, 2, 3).filter { it > 1 }
来源：http://www.ydjk.org.cn/Article/details/gt3imvzffuu.html

[T08] Kotlin：数据类
来源：http://www.52xcode.cn/Article/details/gt3jchxnytk.html

data class User(val name: String, val age: Int)
来源：http://www.52xcode.cn/Article/details/gt3efckxnkn.html

[T09] Kotlin：扩展函数
来源：http://www.52xcode.cn/Article/details/gt3yankcccm.html

fun String.exclaim() = this + "!"
来源：http://www.ydjk.org.cn/Article/details/gt3byvipkzf.html

[T10] Kotlin：默认参数
来源：http://www.52xcode.cn/Article/details/gt3rtcpcily.html

fun greet(name: String = "World") = "Hi $name"
来源：http://www.ydjk.org.cn/Article/details/gt3bysscble.html

[T11] Kotlin：协程
来源：http://www.52xcode.cn/Article/details/gt3wnfgshhi.html

GlobalScope.launch { delay(1000); println("done") }
来源：http://www.ydjk.org.cn/Article/details/gt3orwaezwl.html

[T12] Kotlin：解构声明
来源：http://www.ydjk.org.cn/Article/details/gt3amqwzewa.html

val (a, b) = Pair(1, 2)
来源：http://www.52xcode.cn/Article/details/gt3kqlulowj.html

[T13] Kotlin：只读 Map
来源：http://www.52xcode.cn/Article/details/gt3dwkoynui.html

val m = mapOf("a" to 1)
来源：http://www.52xcode.cn/Article/details/gt3rrljtcyf.html

[T14] Kotlin：循环
来源：http://www.ydjk.org.cn/Article/details/gt3ntprehza.html

for (i in 1..10) println(i)
来源：http://www.52xcode.cn/Article/details/gt3xawgjlxc.html

[T15] Kotlin：接口
来源：http://www.ydjk.org.cn/Article/details/gt3yjwhiekz.html

interface Shape { fun area(): Double }
来源：http://www.ydjk.org.cn/Article/details/gt3ukzspzgn.html

[T16] Swift：Hello World
来源：http://www.ydjk.org.cn/Article/details/gt3cbhtlypg.html

print("Hello")
来源：http://www.ydjk.org.cn/Article/details/gt3biurjehg.html

[T17] Swift：变量与常量
来源：http://www.52xcode.cn/Article/details/gt3ynsmolya.html

var a = 1;  let b = 2
来源：http://www.ydjk.org.cn/Article/details/gt3yphhehzy.html

[T18] Swift：字符串插值
来源：http://www.52xcode.cn/Article/details/gt3iilfemfs.html

"值: \(b)"
来源：http://www.52xcode.cn/Article/details/gt3jstwjnxx.html

[T19] Swift：可选绑定
来源：http://www.ydjk.org.cn/Article/details/gt3owpssxwv.html

if let n = opt { print(n) }
来源：http://www.52xcode.cn/Article/details/gt3ldeulsgp.html

[T20] Swift：数组操作
来源：http://www.52xcode.cn/Article/details/gt3qehsbzga.html

var a = [1, 2, 3];  a.append(4)
来源：http://www.ydjk.org.cn/Article/details/gt3mpedtdcd.html

[T21] Swift：遍历
来源：http://www.52xcode.cn/Article/details/gt3optwodex.html

for x in a { print(x) }
来源：http://www.52xcode.cn/Article/details/gt3owtjqtma.html

[T22] Swift：字典
来源：http://www.52xcode.cn/Article/details/gt3htnrlvhh.html

var d = ["a": 1];  d["b"] = 2
来源：http://www.ydjk.org.cn/Article/details/gt3llpqhxdv.html

[T23] Swift：函数
来源：http://www.ydjk.org.cn/Article/details/gt3xiusfsyq.html

func add(_ a: Int, _ b: Int) -> Int { a + b }
来源：http://www.52xcode.cn/Article/details/gt3jjhvaojh.html

[T24] Swift：闭包
来源：http://www.52xcode.cn/Article/details/gt3efazsxzn.html

let f = { (x: Int) -> Int in x * 2 }
来源：http://www.ydjk.org.cn/Article/details/gt3hykhsezr.html

[T25] Swift：结构体
来源：http://www.ydjk.org.cn/Article/details/gt3syehbwma.html

struct P { var x: Int }
来源：http://www.52xcode.cn/Article/details/gt3glzlphuz.html

[T26] Swift：类与重写
来源：http://www.52xcode.cn/Article/details/gt3jmmztndm.html

class A: Base { override func f() {} }
来源：http://www.52xcode.cn/Article/details/gt3hjojobid.html

[T27] Swift：错误处理
来源：http://www.52xcode.cn/Article/details/gt3vilewwjg.html

do { try f() } catch { print(error) }
来源：http://www.ydjk.org.cn/Article/details/gt3rpzdcnca.html

[T28] Swift：枚举
来源：http://www.ydjk.org.cn/Article/details/gt3gvpqbhnp.html

enum Color { case red, green }
来源：http://www.52xcode.cn/Article/details/gt3elgmmaaa.html

[T29] Swift：guard 提前返回
来源：http://www.52xcode.cn/Article/details/gt3rmrbcqho.html

guard let x = opt else { return }
来源：http://www.ydjk.org.cn/Article/details/gt3uupbnfwd.html

[T30] Swift：协议
来源：http://www.ydjk.org.cn/Article/details/gt3mcvhqazt.html

protocol Shape { func area() -> Double }
来源：http://www.52xcode.cn/Article/details/gt3zvxosild.html

[T31] Lua：Hello World
来源：http://www.ydjk.org.cn/Article/details/gt3hvpmvanc.html

print("Hello")
来源：http://www.52xcode.cn/Article/details/gt3ffehtrgw.html

[T32] Lua：局部变量
来源：http://www.ydjk.org.cn/Article/details/gt3cbexxxgm.html

local a = 1
来源：http://www.52xcode.cn/Article/details/gt3wzbvqodq.html

[T33] Lua：表（数组）
来源：http://www.52xcode.cn/Article/details/gt3vnfqmfzh.html

local t = {1, 2, 3};  t[4] = 4
来源：http://www.52xcode.cn/Article/details/gt3amlvzhho.html

[T34] Lua：遍历表
来源：http://www.ydjk.org.cn/Article/details/gt3tqvkbnmv.html

for i, v in ipairs(t) do print(i, v) end
来源：http://www.ydjk.org.cn/Article/details/gt3iynzqwhc.html

[T35] Lua：字典表
来源：http://www.52xcode.cn/Article/details/gt3zajkpnxw.html

local d = { a = 1 };  d.b = 2
来源：http://www.52xcode.cn/Article/details/gt3jgwntrse.html

[T36] Lua：函数
来源：http://www.ydjk.org.cn/Article/details/gt3doxxgwul.html

function add(a, b) return a + b end
来源：http://www.52xcode.cn/Article/details/gt3enxcqfcj.html

[T37] Lua：字符串拼接
来源：http://www.52xcode.cn/Article/details/gt3wfwbaxps.html

"a" .. "b"
来源：http://www.ydjk.org.cn/Article/details/gt3soiysock.html

[T38] Lua：条件
来源：http://www.52xcode.cn/Article/details/gt3sddvlmrj.html

if x > 0 then print("正") end
来源：http://www.ydjk.org.cn/Article/details/gt3rmkouugu.html

[T39] Lua：模式匹配
来源：http://www.ydjk.org.cn/Article/details/gt3uqphdqtd.html

string.find(s, "%d+")
来源：http://www.52xcode.cn/Article/details/gt3funnusgk.html

[T40] Lua：元表
来源：http://www.52xcode.cn/Article/details/gt3bixmxuho.html

setmetatable({}, { __index = base })
来源：http://www.ydjk.org.cn/Article/details/gt3jrarycly.html

[T41] Perl：Hello World
来源：http://www.52xcode.cn/Article/details/gt3xntohezq.html

print "Hello\n";
来源：http://www.ydjk.org.cn/Article/details/gt3wbfbctjt.html

[T42] Perl：变量类型
来源：http://www.52xcode.cn/Article/details/gt3uguhscyk.html

my $a = 1;  my @arr = (1, 2, 3);  my %h = (a => 1);
来源：http://www.ydjk.org.cn/Article/details/gt3zdufjuju.html

[T43] Perl：字符串插值
来源：http://www.ydjk.org.cn/Article/details/gt3ahsjumsq.html

"值: $a"
来源：http://www.ydjk.org.cn/Article/details/gt3evnbvavp.html

[T44] Perl：条件
来源：http://www.52xcode.cn/Article/details/gt3tooyfxit.html

if ($a > 0) { print "正"; }
来源：http://www.52xcode.cn/Article/details/gt3pzipuljo.html

[T45] Perl：数组遍历
来源：http://www.52xcode.cn/Article/details/gt3bhlmzpll.html

for my $x (@arr) { print $x; }
来源：http://www.ydjk.org.cn/Article/details/gt3goyeyeal.html

[T46] Perl：哈希操作
来源：http://www.ydjk.org.cn/Article/details/gt3tpinenhz.html

$h{b} = 2;  for my $k (keys %h) { print "$k=$h{$k}"; }
来源：http://www.ydjk.org.cn/Article/details/gt3tpzhyxkg.html

[T47] Perl：正则捕获
来源：http://www.52xcode.cn/Article/details/gt3ckstkuac.html

if ($s =~ /(\d+)/) { print $1; }
来源：http://www.ydjk.org.cn/Article/details/gt3qspvrdqh.html

[T48] Perl：正则替换
来源：http://www.52xcode.cn/Article/details/gt3aukhhapm.html

$s =~ s/old/new/g;
来源：http://www.ydjk.org.cn/Article/details/gt3ixsnurwj.html

[T49] Perl：函数
来源：http://www.52xcode.cn/Article/details/gt3bndbtrbh.html

sub add { my ($a, $b) = @_; return $a + $b; }
来源：http://www.ydjk.org.cn/Article/details/gt3vvghuepb.html

[T50] Perl：逐行读文件
来源：http://www.ydjk.org.cn/Article/details/gt3fmnyvily.html

open my $fh, "<", "a.txt" or die $!;
来源：http://www.52xcode.cn/Article/details/gt3fgvshbwv.html

while (my $line = <$fh>) { print $line; }
来源：http://www.ydjk.org.cn/Article/details/gt3pfgwuywk.html

[T51] Scala：Hello World
来源：http://www.52xcode.cn/Article/details/gt3dbalxqjl.html

println("Hello")
来源：http://www.ydjk.org.cn/Article/details/gt3vilkfpyy.html

[T52] Scala：变量
来源：http://www.ydjk.org.cn/Article/details/gt3vnkosrrj.html

val a = 1;  var b = 2
来源：http://www.52xcode.cn/Article/details/gt3vsmkatsg.html

[T53] Scala：字符串插值
来源：http://www.ydjk.org.cn/Article/details/gt3dnotlioc.html

s"值: $b"
来源：http://www.ydjk.org.cn/Article/details/gt3rtgexynq.html

[T54] Scala：集合映射
来源：http://www.52xcode.cn/Article/details/gt3kuiawoza.html

List(1, 2, 3).map(_ * 2)
来源：http://www.ydjk.org.cn/Article/details/gt3qgilxlcs.html

[T55] Scala：集合过滤
来源：http://www.ydjk.org.cn/Article/details/gt3asgmiczj.html

List(1, 2, 3).filter(_ > 1)
来源：http://www.ydjk.org.cn/Article/details/gt3jlssxrwi.html

[T56] Scala：样例类
来源：http://www.ydjk.org.cn/Article/details/gt3yqzmkmin.html

case class User(name: String, age: Int)
来源：http://www.52xcode.cn/Article/details/gt3ujbcruls.html

[T57] Scala：模式匹配
来源：http://www.ydjk.org.cn/Article/details/gt3pebovjwo.html

x match { case 1 => "一"; case _ => "其他" }
来源：http://www.52xcode.cn/Article/details/gt3ieghnsko.html

[T58] Scala：函数定义
来源：http://www.52xcode.cn/Article/details/gt3unzwyocd.html

def add(a: Int, b: Int): Int = a + b
来源：http://www.ydjk.org.cn/Article/details/gt3pwnljxvp.html

[T59] Scala：循环
来源：http://www.ydjk.org.cn/Article/details/gt3kvlkeive.html

for (i <- 1 to 10) println(i)
来源：http://www.ydjk.org.cn/Article/details/gt3gthjfzyt.html

[T60] Scala：折叠
来源：http://www.ydjk.org.cn/Article/details/gt3vphsrfly.html

List(1, 2, 3).foldLeft(0)(_ + _)
来源：http://www.ydjk.org.cn/Article/details/gt3atwywuiu.html

================================================================================
来源：http://www.52xcode.cn/Article/details/gt3xqkannzx.html

U. 高频实用片段（Python / PHP / JavaScript 各 40 条）
来源：http://www.52xcode.cn/Article/details/gt3qarnilbd.html

================================================================================
来源：http://www.ydjk.org.cn/Article/details/gt3lhiaadro.html

[U01] Py：创建虚拟环境
来源：http://www.52xcode.cn/Article/details/gt3hqsuntrc.html

python -m venv .venv && source .venv/bin/activate
来源：http://www.52xcode.cn/Article/details/gt3icluzeat.html

[U02] Py：导出 / 安装依赖
来源：http://www.ydjk.org.cn/Article/details/gt3wgaeqbdo.html

pip freeze > requirements.txt;  pip install -r requirements.txt
来源：http://www.ydjk.org.cn/Article/details/gt3yzlipkob.html

[U03] Py：加载 .env 配置
来源：http://www.ydjk.org.cn/Article/details/gt3dmacramg.html

from dotenv import load_dotenv; load_dotenv()
来源：http://www.52xcode.cn/Article/details/gt3jxxhyebk.html

[U04] Py：变量调试打印
来源：http://www.ydjk.org.cn/Article/details/gt3pwungdjq.html

print(f"{x=}")            # 输出 x=值，Python 3.8+
来源：http://www.52xcode.cn/Article/details/gt3zmtsyenm.html

[U05] Py：列表去重且保序
来源：http://www.ydjk.org.cn/Article/details/gt3yrrdtrpx.html

list(dict.fromkeys(arr))
来源：http://www.ydjk.org.cn/Article/details/gt3qeotazfi.html

[U06] Py：合并两个字典
来源：http://www.ydjk.org.cn/Article/details/gt3qcqqjodi.html

{**a, **b}
来源：http://www.52xcode.cn/Article/details/gt3rylghbnh.html

[U07] Py：反转字典键值
来源：http://www.52xcode.cn/Article/details/gt3lnzcfxvf.html

{v: k for k, v in d.items()}
来源：http://www.ydjk.org.cn/Article/details/gt3hkorljje.html

[U08] Py：展平二维列表
来源：http://www.52xcode.cn/Article/details/gt3hrsapyfi.html

[y for x in nested for y in x]
来源：http://www.52xcode.cn/Article/details/gt3xfjeaqmg.html

[U09] Py：字典取最大值的键
来源：http://www.ydjk.org.cn/Article/details/gt3kxensiem.html

max(d, key=d.get)
来源：http://www.ydjk.org.cn/Article/details/gt3zgtvjrhh.html

[U10] Py：按值排序字典
来源：http://www.52xcode.cn/Article/details/gt3wghbcvrq.html

dict(sorted(d.items(), key=lambda kv: kv[1]))
来源：http://www.52xcode.cn/Article/details/gt3vxqasnhe.html

[U11] Py：生成器表达式
来源：http://www.52xcode.cn/Article/details/gt3zrrmjaeh.html

(x * 2 for x in arr)
来源：http://www.ydjk.org.cn/Article/details/gt3epdtzabc.html

[U12] Py：取出现最多的 3 个元素
来源：http://www.52xcode.cn/Article/details/gt3rualusia.html

Counter(arr).most_common(3)
来源：http://www.ydjk.org.cn/Article/details/gt3llgncejb.html

[U13] Py：固定长度队列
来源：http://www.52xcode.cn/Article/details/gt3eddqyffy.html

deque(maxlen=10)
来源：http://www.52xcode.cn/Article/details/gt3lbdhuwaq.html

[U14] Py：分组收集到列表
来源：http://www.ydjk.org.cn/Article/details/gt3cpkyeltw.html

defaultdict(list)
来源：http://www.ydjk.org.cn/Article/details/gt3ybaizncr.html


<!-- 参考信息 -->