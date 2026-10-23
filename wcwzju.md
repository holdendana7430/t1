代发 wailian999

read -rp "请输入: " ans
来源：http://www.52xcode.cn/Article/details/gt3bjxxmtkb.html

[R78] 交互式菜单
来源：http://www.ydjk.org.cn/Article/details/gt3gbthjoec.html

select opt in a b c; do echo "$opt"; break; done
来源：http://www.52xcode.cn/Article/details/gt3sjttiagy.html

[R79] 解析命令行选项
来源：http://www.52xcode.cn/Article/details/gt3yvqqdohy.html

while getopts "v:f:" o; do case $o in v) V=$OPTARG ;; f) F=$OPTARG ;; esac; done
来源：http://www.52xcode.cn/Article/details/gt3ekbpdrvb.html

[R80] 查看脚本执行耗时
来源：http://www.52xcode.cn/Article/details/gt3kaeeeydg.html

time ./run.sh
来源：http://www.52xcode.cn/Article/details/gt3ugtvvdkc.html

================================================================================
来源：http://www.52xcode.cn/Article/details/gt3dweyffxi.html

S. C / C++ 专题
来源：http://www.ydjk.org.cn/Article/details/gt3qizjtfes.html

================================================================================
来源：http://www.ydjk.org.cn/Article/details/gt3wgmmuawr.html

[S01] C：Hello World
来源：http://www.52xcode.cn/Article/details/gt3zqpdeqet.html

#include <stdio.h>
来源：http://www.ydjk.org.cn/Article/details/gt3xtqlxafk.html

int main(void) { printf("Hello\n"); return 0; }
来源：http://www.52xcode.cn/Article/details/gt3wekrdmus.html

[S02] C：变量与格式化输出
来源：http://www.52xcode.cn/Article/details/gt3iaqcbqsz.html

int a = 10; printf("%d\n", a);
来源：http://www.ydjk.org.cn/Article/details/gt3xneimyyi.html

[S03] C：读入整数
来源：http://www.ydjk.org.cn/Article/details/gt3onalvsqi.html

int x; scanf("%d", &x);
来源：http://www.52xcode.cn/Article/details/gt3yvjcevpg.html

[S04] C：字符串复制
来源：http://www.52xcode.cn/Article/details/gt3wcpvdrvu.html

char dst[32]; strcpy(dst, "hi");
来源：http://www.52xcode.cn/Article/details/gt3gutzjvna.html

[S05] C：字符串长度
来源：http://www.ydjk.org.cn/Article/details/gt3cjvcatxf.html

strlen(s)
来源：http://www.52xcode.cn/Article/details/gt3cbsfnumn.html

[S06] C：字符串比较
来源：http://www.ydjk.org.cn/Article/details/gt3jcqykkvk.html

strcmp(a, b) == 0
来源：http://www.ydjk.org.cn/Article/details/gt3pdqccccf.html

[S07] C：数组遍历求和
来源：http://www.ydjk.org.cn/Article/details/gt3gdlpdoxw.html

for (int i = 0; i < n; i++) sum += a[i];
来源：http://www.52xcode.cn/Article/details/gt3xieegahn.html

[S08] C：动态内存分配与释放
来源：http://www.ydjk.org.cn/Article/details/gt3pwbmcehq.html

int *p = malloc(sizeof(int) * n); ... free(p);
来源：http://www.ydjk.org.cn/Article/details/gt3eapoundp.html

[S09] C：结构体定义与初始化
来源：http://www.52xcode.cn/Article/details/gt3unujmrbo.html

struct Point { int x, y; };  struct Point p = {1, 2};
来源：http://www.52xcode.cn/Article/details/gt3ribrnrve.html

[S10] C：指针与解引用
来源：http://www.52xcode.cn/Article/details/gt3ariakkkk.html

int *p = &a;  *p = 5;
来源：http://www.ydjk.org.cn/Article/details/gt3xsskzijp.html

[S11] C：逐行读文件
来源：http://www.52xcode.cn/Article/details/gt3psktnjah.html

FILE *f = fopen("a.txt", "r");
来源：http://www.ydjk.org.cn/Article/details/gt3yfueytmi.html

while (fgets(buf, sizeof buf, f)) { }
来源：http://www.ydjk.org.cn/Article/details/gt3yhvxkszp.html

fclose(f);
来源：http://www.ydjk.org.cn/Article/details/gt3sisgccyy.html

[S12] C：写文件
来源：http://www.52xcode.cn/Article/details/gt3pydmfell.html

FILE *f = fopen("a.txt", "w");  fprintf(f, "hi\n");  fclose(f);
来源：http://www.ydjk.org.cn/Article/details/gt3jadiknrx.html

[S13] C：宏定义
来源：http://www.ydjk.org.cn/Article/details/gt3ejytuiwo.html

#define MAX(a, b) ((a) > (b) ? (a) : (b))
来源：http://www.52xcode.cn/Article/details/gt3cvyvehep.html

[S14] C：枚举
来源：http://www.52xcode.cn/Article/details/gt3fzyspncp.html

enum Color { RED, GREEN, BLUE };
来源：http://www.ydjk.org.cn/Article/details/gt3owmghezf.html

[S15] C：类型转换
来源：http://www.ydjk.org.cn/Article/details/gt3yttuvgmn.html

(double) a / b
来源：http://www.ydjk.org.cn/Article/details/gt3tbglpqnx.html

[S16] C：位操作置位
来源：http://www.ydjk.org.cn/Article/details/gt3wrpymfjw.html

x |= (1 << 3);
来源：http://www.52xcode.cn/Article/details/gt3ufavcrzo.html

[S17] C：安全拼接字符串
来源：http://www.52xcode.cn/Article/details/gt3ccsuffdh.html

snprintf(buf, sizeof buf, "%s%s", a, b);
来源：http://www.ydjk.org.cn/Article/details/gt3emiaovlz.html

[S18] C：命令行参数
来源：http://www.ydjk.org.cn/Article/details/gt3zmxnsuuz.html

int main(int argc, char **argv)
来源：http://www.52xcode.cn/Article/details/gt3scgvcfue.html

[S19] C：快速排序
来源：http://www.ydjk.org.cn/Article/details/gt3sucuyiae.html

qsort(a, n, sizeof(int), cmp);
来源：http://www.ydjk.org.cn/Article/details/gt3nionetva.html

[S20] C：二分查找
来源：http://www.52xcode.cn/Article/details/gt3vsdszzdi.html

bsearch(&key, a, n, sizeof(int), cmp);
来源：http://www.ydjk.org.cn/Article/details/gt3oyktyxzg.html

[S21] C：字符类别判断
来源：http://www.ydjk.org.cn/Article/details/gt3itrsgecm.html

isdigit(c);  isalpha(c);  isspace(c);
来源：http://www.52xcode.cn/Article/details/gt3brvrtggr.html

[S22] C：字符串转数字
来源：http://www.ydjk.org.cn/Article/details/gt3txrrxifc.html

atoi("42");  strtod("3.14", NULL);
来源：http://www.52xcode.cn/Article/details/gt3bivroree.html

[S23] C：随机数
来源：http://www.52xcode.cn/Article/details/gt3ljwhdzdn.html

srand(time(NULL));  int r = rand() % 100;
来源：http://www.ydjk.org.cn/Article/details/gt3yibpfkzo.html

[S24] C：获取本地时间
来源：http://www.ydjk.org.cn/Article/details/gt3mevumxpf.html

time_t t = time(NULL);  struct tm *tm = localtime(&t);
来源：http://www.52xcode.cn/Article/details/gt3iqxwetwr.html

[S25] C：内存拷贝
来源：http://www.ydjk.org.cn/Article/details/gt3gzyoguuc.html

memcpy(dst, src, n);
来源：http://www.52xcode.cn/Article/details/gt3fjnanigk.html

[S26] C：内存清零
来源：http://www.52xcode.cn/Article/details/gt3rjslqyoa.html

memset(a, 0, sizeof a);
来源：http://www.ydjk.org.cn/Article/details/gt3ornoeykd.html

[S27] C：定义常量
来源：http://www.52xcode.cn/Article/details/gt3ijlyafjw.html

const double PI = 3.14159;
来源：http://www.52xcode.cn/Article/details/gt3yylnilvy.html

[S28] C：静态变量
来源：http://www.52xcode.cn/Article/details/gt3iiuanyzf.html

static int counter = 0;
来源：http://www.52xcode.cn/Article/details/gt3kjwzxojv.html

[S29] C：变参函数
来源：http://www.52xcode.cn/Article/details/gt3vbtatusq.html

va_list ap; va_start(ap, fmt); vprintf(fmt, ap); va_end(ap);
来源：http://www.ydjk.org.cn/Article/details/gt3vnqpqwdw.html

[S30] C：头文件保护
来源：http://www.52xcode.cn/Article/details/gt3nponkszy.html

#ifndef X_H
来源：http://www.52xcode.cn/Article/details/gt3epegubga.html

#define X_H
来源：http://www.ydjk.org.cn/Article/details/gt3ilcdoqrz.html

#endif
来源：http://www.52xcode.cn/Article/details/gt3wyazjjva.html

[S31] C++：Hello World
来源：http://www.ydjk.org.cn/Article/details/gt3vpckyrfe.html

#include <iostream>
来源：http://www.52xcode.cn/Article/details/gt3ikwzhfcu.html

int main() { std::cout << "Hello\n"; }
来源：http://www.ydjk.org.cn/Article/details/gt3fqtnlcuc.html

[S32] C++：字符串
来源：http://www.ydjk.org.cn/Article/details/gt3zljabbbf.html

std::string s = "hi";  s += "!";
来源：http://www.52xcode.cn/Article/details/gt3zqarxhny.html

[S33] C++：vector 增删
来源：http://www.ydjk.org.cn/Article/details/gt3bnxfqurd.html

std::vector<int> v{1, 2, 3};  v.push_back(4);
来源：http://www.52xcode.cn/Article/details/gt3lhroakip.html

[S34] C++：遍历 vector
来源：http://www.52xcode.cn/Article/details/gt3jqcezlqu.html

for (auto &x : v) { std::cout << x; }
来源：http://www.ydjk.org.cn/Article/details/gt3kuhocgrr.html

[S35] C++：map
来源：http://www.ydjk.org.cn/Article/details/gt3rtredqxx.html

std::map<std::string, int> m;  m["a"] = 1;
来源：http://www.ydjk.org.cn/Article/details/gt3baimzzqq.html

[S36] C++：unordered_map
来源：http://www.ydjk.org.cn/Article/details/gt3utkfbfxv.html

std::unordered_map<std::string, int> m;  m["a"] = 1;
来源：http://www.ydjk.org.cn/Article/details/gt3gjbczgga.html

[S37] C++：set
来源：http://www.ydjk.org.cn/Article/details/gt3yafaqpjs.html

std::set<int> s{1, 2, 3};  s.insert(4);
来源：http://www.52xcode.cn/Article/details/gt3mmzkmsci.html

[S38] C++：排序
来源：http://www.52xcode.cn/Article/details/gt3pcbxqqid.html

std::sort(v.begin(), v.end());
来源：http://www.ydjk.org.cn/Article/details/gt3lmdxptkq.html

[S39] C++：自定义比较器排序
来源：http://www.52xcode.cn/Article/details/gt3zzmcefqc.html

std::sort(v.begin(), v.end(), [](int a, int b) { return a > b; });
来源：http://www.52xcode.cn/Article/details/gt3zywvbqnq.html

[S40] C++：查找元素
来源：http://www.52xcode.cn/Article/details/gt3xypsjzua.html

auto it = std::find(v.begin(), v.end(), 3);
来源：http://www.ydjk.org.cn/Article/details/gt3nxmxkggl.html

[S41] C++：类与构造函数
来源：http://www.52xcode.cn/Article/details/gt3ebkdazzf.html

class A { public: A(int v) : x_(v) {} int get() const { return x_; } private: int x_; };
来源：http://www.52xcode.cn/Article/details/gt3tpwgqsoh.html

[S42] C++：继承与虚函数
来源：http://www.ydjk.org.cn/Article/details/gt3wjkzzfuj.html

class B : public Base { public: void f() override {} };
来源：http://www.52xcode.cn/Article/details/gt3ohlutntt.html

[S43] C++：智能指针
来源：http://www.ydjk.org.cn/Article/details/gt3bkhabwet.html

auto p = std::make_unique<int>(5);
来源：http://www.52xcode.cn/Article/details/gt3ovcidfab.html

[S44] C++：引用传参
来源：http://www.ydjk.org.cn/Article/details/gt3uutdtalk.html

void inc(int &x) { ++x; }
来源：http://www.ydjk.org.cn/Article/details/gt3uqcghmxi.html

[S45] C++：lambda
来源：http://www.ydjk.org.cn/Article/details/gt3rvpmhblu.html

auto add = [](int a, int b) { return a + b; };
来源：http://www.ydjk.org.cn/Article/details/gt3kfcmthwe.html

[S46] C++：函数模板
来源：http://www.ydjk.org.cn/Article/details/gt3ukfndpfy.html

template <typename T> T maxv(T a, T b) { return a > b ? a : b; }
来源：http://www.ydjk.org.cn/Article/details/gt3mrbxfdii.html

[S47] C++：结构化绑定遍历
来源：http://www.ydjk.org.cn/Article/details/gt3zubykifo.html

for (const auto &[k, v] : m) { std::cout << k << v; }
来源：http://www.ydjk.org.cn/Article/details/gt3cachaxsf.html

[S48] C++：逐行读文件
来源：http://www.52xcode.cn/Article/details/gt3wmhliucv.html

std::ifstream in("a.txt");  std::string line;
来源：http://www.ydjk.org.cn/Article/details/gt3rrwcqqnt.html

while (std::getline(in, line)) { }
来源：http://www.ydjk.org.cn/Article/details/gt3larjqccy.html

[S49] C++：写文件
来源：http://www.52xcode.cn/Article/details/gt3hyooggyf.html

std::ofstream out("a.txt");  out << "hi\n";
来源：http://www.52xcode.cn/Article/details/gt3lxdqocob.html

[S50] C++：格式化数字
来源：http://www.ydjk.org.cn/Article/details/gt3gammolqc.html

std::ostringstream os;  os << std::fixed << std::setprecision(2) << 3.14159;
来源：http://www.52xcode.cn/Article/details/gt3gzqnbbar.html

[S51] C++：显式类型转换
来源：http://www.52xcode.cn/Article/details/gt3duiqyjci.html

static_cast<double>(a) / b
来源：http://www.52xcode.cn/Article/details/gt3husyakxk.html

[S52] C++：const 与 noexcept
来源：http://www.52xcode.cn/Article/details/gt3aeyuegsw.html

int size() const noexcept { return n_; }
来源：http://www.ydjk.org.cn/Article/details/gt3ejvpgshf.html

[S53] C++：移动语义
来源：http://www.52xcode.cn/Article/details/gt3qjoivpwe.html

std::vector<int> w = std::move(v);
来源：http://www.52xcode.cn/Article/details/gt3acxsbmtj.html

[S54] C++：异常处理
来源：http://www.52xcode.cn/Article/details/gt3pchrgrsx.html

try { throw std::runtime_error("x"); } catch (const std::exception &e) { }
来源：http://www.52xcode.cn/Article/details/gt3trgfbrlz.html

[S55] C++：结构化绑定
来源：http://www.52xcode.cn/Article/details/gt3nrutosoa.html

auto [a, b] = std::make_pair(1, 2);
来源：http://www.ydjk.org.cn/Article/details/gt3qzykkwxh.html

[S56] C++：optional
来源：http://www.ydjk.org.cn/Article/details/gt3uqaihutc.html

std::optional<int> o = 5;  if (o) { int v = *o; }
来源：http://www.52xcode.cn/Article/details/gt3heiffztk.html

[S57] C++：编译期常量
来源：http://www.52xcode.cn/Article/details/gt3diaufwqz.html

constexpr int N = 10;
来源：http://www.ydjk.org.cn/Article/details/gt3uoamniaq.html

[S58] C++：命名空间
来源：http://www.52xcode.cn/Article/details/gt3lbgyjote.html

namespace ns { int f() { return 1; } }
来源：http://www.ydjk.org.cn/Article/details/gt3cairsyqn.html

[S59] C++：静态断言
来源：http://www.ydjk.org.cn/Article/details/gt3efuvwnla.html

static_assert(sizeof(int) == 4, "int 必须 4 字节");
来源：http://www.52xcode.cn/Article/details/gt3pfbuhwog.html

[S60] C++：遍历并删除元素
来源：http://www.ydjk.org.cn/Article/details/gt3mxnshvoh.html

v.erase(std::remove_if(v.begin(), v.end(), [](int x) { return x < 0; }), v.end());
来源：http://www.52xcode.cn/Article/details/gt3vhbmmtcu.html

================================================================================
来源：http://www.ydjk.org.cn/Article/details/gt3yaiutipi.html

T. 其他语言补充（Kotlin / Swift / Lua / Perl / Scala）
来源：http://www.52xcode.cn/Article/details/gt3wyxmnszr.html

================================================================================
来源：http://www.ydjk.org.cn/Article/details/gt3glqdswsg.html

[T01] Kotlin：Hello World
来源：http://www.ydjk.org.cn/Article/details/gt3phzdwpdi.html

println("Hello")
来源：http://www.ydjk.org.cn/Article/details/gt3vnlgdamt.html

[T02] Kotlin：变量
来源：http://www.52xcode.cn/Article/details/gt3xbubghsx.html

val a = 1;  var b = 2        // val 只读，var 可变
来源：http://www.ydjk.org.cn/Article/details/gt3kybissjk.html

[T03] Kotlin：字符串模板
来源：http://www.ydjk.org.cn/Article/details/gt3pastswds.html

"值: $b"
来源：http://www.ydjk.org.cn/Article/details/gt3htjzyups.html

[T04] Kotlin：空安全
来源：http://www.52xcode.cn/Article/details/gt3uzbgvefc.html

val n: String? = null;  n?.length
来源：http://www.52xcode.cn/Article/details/gt3lawijhzk.html

[T05] Kotlin：when 表达式
来源：http://www.52xcode.cn/Article/details/gt3aamensor.html

val s = when (x) { 1 -> "一" else -> "其他" }   // 多分支时每个分支单独一行
来源：http://www.ydjk.org.cn/Article/details/gt3myrjetug.html

[T06] Kotlin：集合映射
来源：http://www.52xcode.cn/Article/details/gt3hoshamnz.html

listOf(1, 2, 3).map { it * 2 }
来源：http://www.52xcode.cn/Article/details/gt3ocxzjscs.html

[T07] Kotlin：集合过滤
来源：http://www.52xcode.cn/Article/details/gt3jzhhngun.html

listOf(1, 2, 3).filter { it > 1 }
来源：http://www.ydjk.org.cn/Article/details/gt3jgjdpcpp.html

[T08] Kotlin：数据类
来源：http://www.ydjk.org.cn/Article/details/gt3nywlvzom.html

data class User(val name: String, val age: Int)
来源：http://www.ydjk.org.cn/Article/details/gt3ihbvbdsh.html

[T09] Kotlin：扩展函数
来源：http://www.52xcode.cn/Article/details/gt3bvgsbrgo.html

fun String.exclaim() = this + "!"
来源：http://www.52xcode.cn/Article/details/gt3qcndxmyn.html

[T10] Kotlin：默认参数
来源：http://www.ydjk.org.cn/Article/details/gt3wldeldmg.html

fun greet(name: String = "World") = "Hi $name"
来源：http://www.ydjk.org.cn/Article/details/gt3lqrngtxz.html

[T11] Kotlin：协程
来源：http://www.ydjk.org.cn/Article/details/gt3swedxude.html

GlobalScope.launch { delay(1000); println("done") }
来源：http://www.52xcode.cn/Article/details/gt3xyjfahkb.html

[T12] Kotlin：解构声明
来源：http://www.ydjk.org.cn/Article/details/gt3angdhvvp.html

val (a, b) = Pair(1, 2)
来源：http://www.ydjk.org.cn/Article/details/gt3vuwcfxln.html

[T13] Kotlin：只读 Map
来源：http://www.ydjk.org.cn/Article/details/gt3pthudros.html

val m = mapOf("a" to 1)
来源：http://www.ydjk.org.cn/Article/details/gt3cliezzfs.html

[T14] Kotlin：循环
来源：http://www.52xcode.cn/Article/details/gt3oxlvnunj.html

for (i in 1..10) println(i)
来源：http://www.ydjk.org.cn/Article/details/gt3btlpxwwg.html

[T15] Kotlin：接口
来源：http://www.52xcode.cn/Article/details/gt3ejipszjc.html

interface Shape { fun area(): Double }
来源：http://www.52xcode.cn/Article/details/gt3uytdxync.html

[T16] Swift：Hello World
来源：http://www.ydjk.org.cn/Article/details/gt3tiegewyp.html

print("Hello")
来源：http://www.ydjk.org.cn/Article/details/gt3rwhoaery.html

[T17] Swift：变量与常量
来源：http://www.ydjk.org.cn/Article/details/gt3uauvcqux.html

var a = 1;  let b = 2
来源：http://www.52xcode.cn/Article/details/gt3phwlsici.html

[T18] Swift：字符串插值
来源：http://www.ydjk.org.cn/Article/details/gt3ukyrmbub.html

"值: \(b)"
来源：http://www.52xcode.cn/Article/details/gt3rtawjnfh.html

[T19] Swift：可选绑定
来源：http://www.ydjk.org.cn/Article/details/gt3nwhjhtap.html

if let n = opt { print(n) }
来源：http://www.52xcode.cn/Article/details/gt3zypjldio.html

[T20] Swift：数组操作
来源：http://www.52xcode.cn/Article/details/gt3hfjtnahp.html

var a = [1, 2, 3];  a.append(4)
来源：http://www.52xcode.cn/Article/details/gt3ibpzidex.html

[T21] Swift：遍历
来源：http://www.ydjk.org.cn/Article/details/gt3eqyyhdhz.html

for x in a { print(x) }
来源：http://www.52xcode.cn/Article/details/gt3ovchnsdb.html

[T22] Swift：字典
来源：http://www.ydjk.org.cn/Article/details/gt3parwlqpt.html

var d = ["a": 1];  d["b"] = 2
来源：http://www.52xcode.cn/Article/details/gt3ethladxi.html

[T23] Swift：函数
来源：http://www.52xcode.cn/Article/details/gt3jivlxlpz.html

func add(_ a: Int, _ b: Int) -> Int { a + b }
来源：http://www.ydjk.org.cn/Article/details/gt3bpptazzb.html

[T24] Swift：闭包
来源：http://www.ydjk.org.cn/Article/details/gt3kcvxpjnx.html

let f = { (x: Int) -> Int in x * 2 }
来源：http://www.ydjk.org.cn/Article/details/gt3gnekehha.html

[T25] Swift：结构体
来源：http://www.ydjk.org.cn/Article/details/gt3ywuvubgg.html

struct P { var x: Int }
来源：http://www.ydjk.org.cn/Article/details/gt3ampanrmq.html

[T26] Swift：类与重写
来源：http://www.52xcode.cn/Article/details/gt3ysbngvxc.html

class A: Base { override func f() {} }
来源：http://www.ydjk.org.cn/Article/details/gt3dujqdzya.html

[T27] Swift：错误处理
来源：http://www.52xcode.cn/Article/details/gt3tbnznbje.html

do { try f() } catch { print(error) }
来源：http://www.ydjk.org.cn/Article/details/gt3afulgfhs.html

[T28] Swift：枚举
来源：http://www.ydjk.org.cn/Article/details/gt3qepgwkvf.html

enum Color { case red, green }
来源：http://www.ydjk.org.cn/Article/details/gt3uhhnbzph.html

[T29] Swift：guard 提前返回
来源：http://www.52xcode.cn/Article/details/gt3lzbybhoy.html

guard let x = opt else { return }
来源：http://www.52xcode.cn/Article/details/gt3yjnwvhxc.html

[T30] Swift：协议
来源：http://www.52xcode.cn/Article/details/gt3ufpgaxdf.html

protocol Shape { func area() -> Double }
来源：http://www.52xcode.cn/Article/details/gt3bhwuprsz.html

[T31] Lua：Hello World
来源：http://www.52xcode.cn/Article/details/gt3rszaurrg.html

print("Hello")
来源：http://www.ydjk.org.cn/Article/details/gt3wgtgghys.html

[T32] Lua：局部变量
来源：http://www.52xcode.cn/Article/details/gt3btjdknap.html

local a = 1
来源：http://www.52xcode.cn/Article/details/gt3qmgvpnld.html

[T33] Lua：表（数组）
来源：http://www.52xcode.cn/Article/details/gt3hpfsviad.html

local t = {1, 2, 3};  t[4] = 4
来源：http://www.ydjk.org.cn/Article/details/gt3ogqwrbpu.html

[T34] Lua：遍历表
来源：http://www.ydjk.org.cn/Article/details/gt3qmbplsix.html

for i, v in ipairs(t) do print(i, v) end
来源：http://www.52xcode.cn/Article/details/gt3dryasurp.html

[T35] Lua：字典表
来源：http://www.52xcode.cn/Article/details/gt3kcxxssvu.html

local d = { a = 1 };  d.b = 2
来源：http://www.ydjk.org.cn/Article/details/gt3tfmiesyl.html

[T36] Lua：函数
来源：http://www.52xcode.cn/Article/details/gt3zrodhide.html

function add(a, b) return a + b end
来源：http://www.ydjk.org.cn/Article/details/gt3aviwifjr.html

[T37] Lua：字符串拼接
来源：http://www.52xcode.cn/Article/details/gt3hxuswyfa.html

"a" .. "b"
来源：http://www.ydjk.org.cn/Article/details/gt3pqfyoqvy.html

[T38] Lua：条件
来源：http://www.ydjk.org.cn/Article/details/gt3ufszbfsj.html

if x > 0 then print("正") end
来源：http://www.ydjk.org.cn/Article/details/gt3seapgxoz.html

[T39] Lua：模式匹配
来源：http://www.52xcode.cn/Article/details/gt3cesnhngb.html

string.find(s, "%d+")
来源：http://www.ydjk.org.cn/Article/details/gt3lwuzfgxz.html

[T40] Lua：元表
来源：http://www.ydjk.org.cn/Article/details/gt3iuprglfe.html

setmetatable({}, { __index = base })
来源：http://www.52xcode.cn/Article/details/gt3zyjpwceh.html

[T41] Perl：Hello World
来源：http://www.52xcode.cn/Article/details/gt3hpyojyhq.html

print "Hello\n";
来源：http://www.52xcode.cn/Article/details/gt3xhzldhko.html

[T42] Perl：变量类型
来源：http://www.52xcode.cn/Article/details/gt3zkfrjbta.html

my $a = 1;  my @arr = (1, 2, 3);  my %h = (a => 1);
来源：http://www.52xcode.cn/Article/details/gt3zvoxsedf.html

[T43] Perl：字符串插值
来源：http://www.52xcode.cn/Article/details/gt3jwufvvkf.html

"值: $a"
来源：http://www.52xcode.cn/Article/details/gt3szixfroz.html

[T44] Perl：条件
来源：http://www.52xcode.cn/Article/details/gt3rpdpzxqg.html

if ($a > 0) { print "正"; }
来源：http://www.52xcode.cn/Article/details/gt3gfzmaksf.html

[T45] Perl：数组遍历
来源：http://www.52xcode.cn/Article/details/gt3fgeosjkh.html

for my $x (@arr) { print $x; }
来源：http://www.ydjk.org.cn/Article/details/gt3fxamuzqn.html

[T46] Perl：哈希操作
来源：http://www.52xcode.cn/Article/details/gt3poxyrdya.html

$h{b} = 2;  for my $k (keys %h) { print "$k=$h{$k}"; }
来源：http://www.52xcode.cn/Article/details/gt3hzybzgat.html

[T47] Perl：正则捕获
来源：http://www.ydjk.org.cn/Article/details/gt3raiclqew.html

if ($s =~ /(\d+)/) { print $1; }
来源：http://www.ydjk.org.cn/Article/details/gt3ufknzehx.html

[T48] Perl：正则替换
来源：http://www.ydjk.org.cn/Article/details/gt3pxismqzm.html

$s =~ s/old/new/g;
来源：http://www.52xcode.cn/Article/details/gt3psqxfnkr.html

[T49] Perl：函数
来源：http://www.52xcode.cn/Article/details/gt3onejqnke.html

sub add { my ($a, $b) = @_; return $a + $b; }
来源：http://www.52xcode.cn/Article/details/gt3nbactoam.html

[T50] Perl：逐行读文件
来源：http://www.52xcode.cn/Article/details/gt3qhsnkukv.html

open my $fh, "<", "a.txt" or die $!;
来源：http://www.ydjk.org.cn/Article/details/gt3qvpqyxjk.html

while (my $line = <$fh>) { print $line; }
来源：http://www.52xcode.cn/Article/details/gt3zcuyibqg.html

[T51] Scala：Hello World
来源：http://www.ydjk.org.cn/Article/details/gt3kashdycc.html

println("Hello")
来源：http://www.52xcode.cn/Article/details/gt3sxojvsce.html

[T52] Scala：变量
来源：http://www.ydjk.org.cn/Article/details/gt3gtwavyzv.html

val a = 1;  var b = 2
来源：http://www.ydjk.org.cn/Article/details/gt3kksstucq.html

[T53] Scala：字符串插值
来源：http://www.ydjk.org.cn/Article/details/gt3xbixgeki.html

s"值: $b"
来源：http://www.52xcode.cn/Article/details/gt3bkzuivdq.html

[T54] Scala：集合映射
来源：http://www.ydjk.org.cn/Article/details/gt3rjpiidch.html

List(1, 2, 3).map(_ * 2)
来源：http://www.52xcode.cn/Article/details/gt3ptnuoqeh.html

[T55] Scala：集合过滤
来源：http://www.52xcode.cn/Article/details/gt3fpuadnsc.html

List(1, 2, 3).filter(_ > 1)
来源：http://www.52xcode.cn/Article/details/gt3uklqbsww.html

[T56] Scala：样例类
来源：http://www.52xcode.cn/Article/details/gt3gcjzoues.html

case class User(name: String, age: Int)
来源：http://www.ydjk.org.cn/Article/details/gt3rekqjpei.html

[T57] Scala：模式匹配
来源：http://www.ydjk.org.cn/Article/details/gt3lgexixhl.html

x match { case 1 => "一"; case _ => "其他" }
来源：http://www.ydjk.org.cn/Article/details/gt3kjurmizn.html

[T58] Scala：函数定义
来源：http://www.52xcode.cn/Article/details/gt3qfjqscfz.html

def add(a: Int, b: Int): Int = a + b
来源：http://www.ydjk.org.cn/Article/details/gt3wdybryys.html

[T59] Scala：循环
来源：http://www.ydjk.org.cn/Article/details/gt3jjdqegxa.html

for (i <- 1 to 10) println(i)
来源：http://www.ydjk.org.cn/Article/details/gt3glvrzypf.html

[T60] Scala：折叠
来源：http://www.ydjk.org.cn/Article/details/gt3phppdvww.html

List(1, 2, 3).foldLeft(0)(_ + _)
来源：http://www.ydjk.org.cn/Article/details/gt3dnebnjfn.html

================================================================================
来源：http://www.ydjk.org.cn/Article/details/gt3grtbphde.html

U. 高频实用片段（Python / PHP / JavaScript 各 40 条）
来源：http://www.ydjk.org.cn/Article/details/gt3cxoopmly.html

================================================================================
来源：http://www.52xcode.cn/Article/details/gt3mfqbmtki.html

[U01] Py：创建虚拟环境
来源：http://www.52xcode.cn/Article/details/gt3wjotbidy.html

python -m venv .venv && source .venv/bin/activate
来源：http://www.ydjk.org.cn/Article/details/gt3btfulkbv.html

[U02] Py：导出 / 安装依赖
来源：http://www.ydjk.org.cn/Article/details/gt3udemraio.html

pip freeze > requirements.txt;  pip install -r requirements.txt
来源：http://www.ydjk.org.cn/Article/details/gt3woxuddtc.html

[U03] Py：加载 .env 配置
来源：http://www.ydjk.org.cn/Article/details/gt3gwurburh.html

from dotenv import load_dotenv; load_dotenv()
来源：http://www.ydjk.org.cn/Article/details/gt3pihtkvrc.html

[U04] Py：变量调试打印
来源：http://www.ydjk.org.cn/Article/details/gt3fbfynkoz.html

print(f"{x=}")            # 输出 x=值，Python 3.8+
来源：http://www.ydjk.org.cn/Article/details/gt3ghjaqzft.html

[U05] Py：列表去重且保序
来源：http://www.52xcode.cn/Article/details/gt3waxstnfl.html

list(dict.fromkeys(arr))
来源：http://www.ydjk.org.cn/Article/details/gt3lpnsyqqy.html

[U06] Py：合并两个字典
来源：http://www.ydjk.org.cn/Article/details/gt3wvvtwegz.html

{**a, **b}
来源：http://www.52xcode.cn/Article/details/gt3mkvvpkta.html

[U07] Py：反转字典键值
来源：http://www.52xcode.cn/Article/details/gt3mfbuiave.html

{v: k for k, v in d.items()}
来源：http://www.ydjk.org.cn/Article/details/gt3gbrgbcfa.html

[U08] Py：展平二维列表
来源：http://www.52xcode.cn/Article/details/gt3etsuybyt.html

[y for x in nested for y in x]
来源：http://www.ydjk.org.cn/Article/details/gt3sbgzykda.html

[U09] Py：字典取最大值的键
来源：http://www.ydjk.org.cn/Article/details/gt3qgkqoflv.html

max(d, key=d.get)
来源：http://www.52xcode.cn/Article/details/gt3xnixgbou.html

[U10] Py：按值排序字典
来源：http://www.ydjk.org.cn/Article/details/gt3hbpnmzzx.html

dict(sorted(d.items(), key=lambda kv: kv[1]))
来源：http://www.52xcode.cn/Article/details/gt3mzwzzxoz.html

[U11] Py：生成器表达式
来源：http://www.52xcode.cn/Article/details/gt3vllwbfcs.html

(x * 2 for x in arr)
来源：http://www.52xcode.cn/Article/details/gt3hzcodhap.html

[U12] Py：取出现最多的 3 个元素
来源：http://www.ydjk.org.cn/Article/details/gt3nrezdpwp.html

Counter(arr).most_common(3)
来源：http://www.52xcode.cn/Article/details/gt3xklbfumr.html

[U13] Py：固定长度队列
来源：http://www.ydjk.org.cn/Article/details/gt3yzcpkzjg.html

deque(maxlen=10)
来源：http://www.ydjk.org.cn/Article/details/gt3zoumzjil.html

[U14] Py：分组收集到列表
来源：http://www.52xcode.cn/Article/details/gt3aaxbplbl.html

defaultdict(list)
来源：http://www.52xcode.cn/Article/details/gt3qccurgcc.html

[U15] Py：高精度计时
来源：http://www.ydjk.org.cn/Article/details/gt3xopxzjbk.html

t = time.perf_counter()
来源：http://www.ydjk.org.cn/Article/details/gt3vsvgasuj.html

[U16] Py：命令行参数解析
来源：http://www.ydjk.org.cn/Article/details/gt3mcdflhbv.html

ap = argparse.ArgumentParser();  ap.add_argument("--name");  args = ap.parse_args()
来源：http://www.ydjk.org.cn/Article/details/gt3gjxehtga.html

[U17] Py：初始化日志
来源：http://www.52xcode.cn/Article/details/gt3jwjrvngd.html

logging.basicConfig(level=logging.INFO)
来源：http://www.52xcode.cn/Article/details/gt3bdrpxqzd.html

[U18] Py：预编译正则
来源：http://www.52xcode.cn/Article/details/gt3mltvoywa.html

pat = re.compile(r"\d+")
来源：http://www.ydjk.org.cn/Article/details/gt3moevwfhg.html


<!-- 参考信息 -->