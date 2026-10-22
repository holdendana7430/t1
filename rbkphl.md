代发 wailian999

split -l 1000 big.log part_
来源：http://www.52xcode.cn/Article/details/gt2uzdxyjmq.html

[R74] 批量重命名
来源：http://www.52xcode.cn/Article/details/gt2asuatijn.html

for f in *.jpeg; do mv "$f" "${f%.jpeg}.jpg"; done
来源：http://www.ydjk.org.cn/Article/details/gt2cxkzwuef.html

[R75] 导出环境变量
来源：http://www.ydjk.org.cn/Article/details/gt2yqgbooqo.html

export PATH="$HOME/bin:$PATH"
来源：http://www.ydjk.org.cn/Article/details/gt2lormehdt.html

[R76] 使用临时文件
来源：http://www.52xcode.cn/Article/details/gt2rakuapbk.html

tmp=$(mktemp); trap 'rm -f "$tmp"' EXIT
来源：http://www.ydjk.org.cn/Article/details/gt2eierpdto.html

[R77] 读取用户输入
来源：http://www.ydjk.org.cn/Article/details/gt2iwhadnqz.html

read -rp "请输入: " ans
来源：http://www.ydjk.org.cn/Article/details/gt2okknyvnz.html

[R78] 交互式菜单
来源：http://www.52xcode.cn/Article/details/gt2npujkqsj.html

select opt in a b c; do echo "$opt"; break; done
来源：http://www.52xcode.cn/Article/details/gt2rpngykkm.html

[R79] 解析命令行选项
来源：http://www.52xcode.cn/Article/details/gt2dokglzos.html

while getopts "v:f:" o; do case $o in v) V=$OPTARG ;; f) F=$OPTARG ;; esac; done
来源：http://www.52xcode.cn/Article/details/gt2irjzpxtd.html

[R80] 查看脚本执行耗时
来源：http://www.52xcode.cn/Article/details/gt2zsscxsro.html

time ./run.sh
来源：http://www.ydjk.org.cn/Article/details/gt2xdoiybzl.html

================================================================================
来源：http://www.52xcode.cn/Article/details/gt2mgmlvawd.html

S. C / C++ 专题
来源：http://www.ydjk.org.cn/Article/details/gt2kfhhnkkr.html

================================================================================
来源：http://www.ydjk.org.cn/Article/details/gt2mdxsvajk.html

[S01] C：Hello World
来源：http://www.52xcode.cn/Article/details/gt2zepojjdd.html

#include <stdio.h>
来源：http://www.52xcode.cn/Article/details/gt2qufslpbe.html

int main(void) { printf("Hello\n"); return 0; }
来源：http://www.52xcode.cn/Article/details/gt2wjtugugi.html

[S02] C：变量与格式化输出
来源：http://www.ydjk.org.cn/Article/details/gt2tmucmnpt.html

int a = 10; printf("%d\n", a);
来源：http://www.52xcode.cn/Article/details/gt2ooztdhqk.html

[S03] C：读入整数
来源：http://www.52xcode.cn/Article/details/gt2inwielig.html

int x; scanf("%d", &x);
来源：http://www.ydjk.org.cn/Article/details/gt2pqsvjcuf.html

[S04] C：字符串复制
来源：http://www.52xcode.cn/Article/details/gt2reuuckzm.html

char dst[32]; strcpy(dst, "hi");
来源：http://www.52xcode.cn/Article/details/gt2hlnbivzy.html

[S05] C：字符串长度
来源：http://www.ydjk.org.cn/Article/details/gt2ruhtzcsy.html

strlen(s)
来源：http://www.52xcode.cn/Article/details/gt2vppjfmrf.html

[S06] C：字符串比较
来源：http://www.52xcode.cn/Article/details/gt2ahymdmzc.html

strcmp(a, b) == 0
来源：http://www.ydjk.org.cn/Article/details/gt2kdapcvqm.html

[S07] C：数组遍历求和
来源：http://www.52xcode.cn/Article/details/gt2tkucyqar.html

for (int i = 0; i < n; i++) sum += a[i];
来源：http://www.ydjk.org.cn/Article/details/gt2vafndhyh.html

[S08] C：动态内存分配与释放
来源：http://www.52xcode.cn/Article/details/gt2irfsfxpz.html

int *p = malloc(sizeof(int) * n); ... free(p);
来源：http://www.52xcode.cn/Article/details/gt2jpwgbdsd.html

[S09] C：结构体定义与初始化
来源：http://www.ydjk.org.cn/Article/details/gt2kzxynoao.html

struct Point { int x, y; };  struct Point p = {1, 2};
来源：http://www.52xcode.cn/Article/details/gt2hruzxcnf.html

[S10] C：指针与解引用
来源：http://www.ydjk.org.cn/Article/details/gt2ihcjkbxd.html

int *p = &a;  *p = 5;
来源：http://www.ydjk.org.cn/Article/details/gt2rvdttwiq.html

[S11] C：逐行读文件
来源：http://www.52xcode.cn/Article/details/gt2cdywspqx.html

FILE *f = fopen("a.txt", "r");
来源：http://www.52xcode.cn/Article/details/gt2setwizjn.html

while (fgets(buf, sizeof buf, f)) { }
来源：http://www.52xcode.cn/Article/details/gt2qxwubuln.html

fclose(f);
来源：http://www.ydjk.org.cn/Article/details/gt2ikqiwmcd.html

[S12] C：写文件
来源：http://www.52xcode.cn/Article/details/gt2aeasczjq.html

FILE *f = fopen("a.txt", "w");  fprintf(f, "hi\n");  fclose(f);
来源：http://www.ydjk.org.cn/Article/details/gt2kwcorpek.html

[S13] C：宏定义
来源：http://www.ydjk.org.cn/Article/details/gt2kxocytkb.html

#define MAX(a, b) ((a) > (b) ? (a) : (b))
来源：http://www.52xcode.cn/Article/details/gt2nlvtumla.html

[S14] C：枚举
来源：http://www.52xcode.cn/Article/details/gt2ksrfkmil.html

enum Color { RED, GREEN, BLUE };
来源：http://www.ydjk.org.cn/Article/details/gt2lllrjvyv.html

[S15] C：类型转换
来源：http://www.52xcode.cn/Article/details/gt2lcnnmhaa.html

(double) a / b
来源：http://www.ydjk.org.cn/Article/details/gt2znbcpnrg.html

[S16] C：位操作置位
来源：http://www.ydjk.org.cn/Article/details/gt2yodbosij.html

x |= (1 << 3);
来源：http://www.52xcode.cn/Article/details/gt2jsbgrlle.html

[S17] C：安全拼接字符串
来源：http://www.52xcode.cn/Article/details/gt2cewjozrm.html

snprintf(buf, sizeof buf, "%s%s", a, b);
来源：http://www.52xcode.cn/Article/details/gt2wtbaafiu.html

[S18] C：命令行参数
来源：http://www.52xcode.cn/Article/details/gt2zsipejjn.html

int main(int argc, char **argv)
来源：http://www.52xcode.cn/Article/details/gt2auxmphen.html

[S19] C：快速排序
来源：http://www.52xcode.cn/Article/details/gt2ajchutin.html

qsort(a, n, sizeof(int), cmp);
来源：http://www.52xcode.cn/Article/details/gt2donlcivf.html

[S20] C：二分查找
来源：http://www.52xcode.cn/Article/details/gt2bwihefgp.html

bsearch(&key, a, n, sizeof(int), cmp);
来源：http://www.ydjk.org.cn/Article/details/gt2pmzhdtzt.html

[S21] C：字符类别判断
来源：http://www.ydjk.org.cn/Article/details/gt2igsejsno.html

isdigit(c);  isalpha(c);  isspace(c);
来源：http://www.ydjk.org.cn/Article/details/gt2dftwfvsd.html

[S22] C：字符串转数字
来源：http://www.52xcode.cn/Article/details/gt2nusbvjhu.html

atoi("42");  strtod("3.14", NULL);
来源：http://www.ydjk.org.cn/Article/details/gt2qsvhlotb.html

[S23] C：随机数
来源：http://www.52xcode.cn/Article/details/gt2irlnhwcc.html

srand(time(NULL));  int r = rand() % 100;
来源：http://www.52xcode.cn/Article/details/gt2arxxlhdv.html

[S24] C：获取本地时间
来源：http://www.ydjk.org.cn/Article/details/gt2xcvwnaar.html

time_t t = time(NULL);  struct tm *tm = localtime(&t);
来源：http://www.ydjk.org.cn/Article/details/gt2utsrgmwe.html

[S25] C：内存拷贝
来源：http://www.52xcode.cn/Article/details/gt2zjnsqfui.html

memcpy(dst, src, n);
来源：http://www.ydjk.org.cn/Article/details/gt2owsihyqc.html

[S26] C：内存清零
来源：http://www.ydjk.org.cn/Article/details/gt2cwdlxfel.html

memset(a, 0, sizeof a);
来源：http://www.ydjk.org.cn/Article/details/gt2fuxhopjl.html

[S27] C：定义常量
来源：http://www.52xcode.cn/Article/details/gt2kfyosmfc.html

const double PI = 3.14159;
来源：http://www.ydjk.org.cn/Article/details/gt2kotaheky.html

[S28] C：静态变量
来源：http://www.ydjk.org.cn/Article/details/gt2swxmljdv.html

static int counter = 0;
来源：http://www.ydjk.org.cn/Article/details/gt2zxuwerut.html

[S29] C：变参函数
来源：http://www.52xcode.cn/Article/details/gt2gtxyvdgy.html

va_list ap; va_start(ap, fmt); vprintf(fmt, ap); va_end(ap);
来源：http://www.52xcode.cn/Article/details/gt2pueevlyj.html

[S30] C：头文件保护
来源：http://www.ydjk.org.cn/Article/details/gt2uepzccep.html

#ifndef X_H
来源：http://www.ydjk.org.cn/Article/details/gt2vpvjrgem.html

#define X_H
来源：http://www.52xcode.cn/Article/details/gt2myocihpk.html

#endif
来源：http://www.52xcode.cn/Article/details/gt2vvkayokf.html

[S31] C++：Hello World
来源：http://www.52xcode.cn/Article/details/gt2vyilguco.html

#include <iostream>
来源：http://www.52xcode.cn/Article/details/gt2atvkxwgq.html

int main() { std::cout << "Hello\n"; }
来源：http://www.ydjk.org.cn/Article/details/gt2xhammzus.html

[S32] C++：字符串
来源：http://www.52xcode.cn/Article/details/gt2oiyaidlz.html

std::string s = "hi";  s += "!";
来源：http://www.52xcode.cn/Article/details/gt2uwqxldte.html

[S33] C++：vector 增删
来源：http://www.ydjk.org.cn/Article/details/gt2crlcqjqv.html

std::vector<int> v{1, 2, 3};  v.push_back(4);
来源：http://www.ydjk.org.cn/Article/details/gt2ykosjxom.html

[S34] C++：遍历 vector
来源：http://www.52xcode.cn/Article/details/gt2cffkaafj.html

for (auto &x : v) { std::cout << x; }
来源：http://www.ydjk.org.cn/Article/details/gt2vfiasmof.html

[S35] C++：map
来源：http://www.52xcode.cn/Article/details/gt2kpeonbxy.html

std::map<std::string, int> m;  m["a"] = 1;
来源：http://www.ydjk.org.cn/Article/details/gt2dxcijjnc.html

[S36] C++：unordered_map
来源：http://www.ydjk.org.cn/Article/details/gt2immbziyt.html

std::unordered_map<std::string, int> m;  m["a"] = 1;
来源：http://www.ydjk.org.cn/Article/details/gt2cvbclkdk.html

[S37] C++：set
来源：http://www.52xcode.cn/Article/details/gt2medahabr.html

std::set<int> s{1, 2, 3};  s.insert(4);
来源：http://www.ydjk.org.cn/Article/details/gt2oussiymn.html

[S38] C++：排序
来源：http://www.ydjk.org.cn/Article/details/gt2syrdzkwt.html

std::sort(v.begin(), v.end());
来源：http://www.ydjk.org.cn/Article/details/gt2ertsrwjo.html

[S39] C++：自定义比较器排序
来源：http://www.ydjk.org.cn/Article/details/gt2jlqrlvop.html

std::sort(v.begin(), v.end(), [](int a, int b) { return a > b; });
来源：http://www.52xcode.cn/Article/details/gt2kpavrczn.html

[S40] C++：查找元素
来源：http://www.52xcode.cn/Article/details/gt2knksiwnc.html

auto it = std::find(v.begin(), v.end(), 3);
来源：http://www.ydjk.org.cn/Article/details/gt2hlzzyvtr.html

[S41] C++：类与构造函数
来源：http://www.52xcode.cn/Article/details/gt2djcflkwh.html

class A { public: A(int v) : x_(v) {} int get() const { return x_; } private: int x_; };
来源：http://www.ydjk.org.cn/Article/details/gt2eesnbtxq.html

[S42] C++：继承与虚函数
来源：http://www.52xcode.cn/Article/details/gt2oyaaaibi.html

class B : public Base { public: void f() override {} };
来源：http://www.ydjk.org.cn/Article/details/gt2edeepymw.html

[S43] C++：智能指针
来源：http://www.ydjk.org.cn/Article/details/gt2atdpxfhr.html

auto p = std::make_unique<int>(5);
来源：http://www.ydjk.org.cn/Article/details/gt2gywnzxwm.html

[S44] C++：引用传参
来源：http://www.52xcode.cn/Article/details/gt2xrjksxum.html

void inc(int &x) { ++x; }
来源：http://www.52xcode.cn/Article/details/gt2kvfhbqbu.html

[S45] C++：lambda
来源：http://www.52xcode.cn/Article/details/gt2mdjqhxzb.html

auto add = [](int a, int b) { return a + b; };
来源：http://www.ydjk.org.cn/Article/details/gt2awxkrxce.html

[S46] C++：函数模板
来源：http://www.52xcode.cn/Article/details/gt2ctekagfb.html

template <typename T> T maxv(T a, T b) { return a > b ? a : b; }
来源：http://www.52xcode.cn/Article/details/gt2aonplevv.html

[S47] C++：结构化绑定遍历
来源：http://www.ydjk.org.cn/Article/details/gt2whuhdftd.html

for (const auto &[k, v] : m) { std::cout << k << v; }
来源：http://www.ydjk.org.cn/Article/details/gt2hxuogpxj.html

[S48] C++：逐行读文件
来源：http://www.52xcode.cn/Article/details/gt2dliiilak.html

std::ifstream in("a.txt");  std::string line;
来源：http://www.ydjk.org.cn/Article/details/gt2onwsbmxg.html

while (std::getline(in, line)) { }
来源：http://www.ydjk.org.cn/Article/details/gt2ijxcrfla.html

[S49] C++：写文件
来源：http://www.52xcode.cn/Article/details/gt2iiqbupkq.html

std::ofstream out("a.txt");  out << "hi\n";
来源：http://www.52xcode.cn/Article/details/gt2klujfczz.html

[S50] C++：格式化数字
来源：http://www.ydjk.org.cn/Article/details/gt2vyysdwuk.html

std::ostringstream os;  os << std::fixed << std::setprecision(2) << 3.14159;
来源：http://www.52xcode.cn/Article/details/gt2xigrtqfc.html

[S51] C++：显式类型转换
来源：http://www.52xcode.cn/Article/details/gt2dbarnnln.html

static_cast<double>(a) / b
来源：http://www.52xcode.cn/Article/details/gt2ynktines.html

[S52] C++：const 与 noexcept
来源：http://www.ydjk.org.cn/Article/details/gt2exrudksa.html

int size() const noexcept { return n_; }
来源：http://www.ydjk.org.cn/Article/details/gt2homubcep.html

[S53] C++：移动语义
来源：http://www.52xcode.cn/Article/details/gt2fwllhzne.html

std::vector<int> w = std::move(v);
来源：http://www.52xcode.cn/Article/details/gt2qoqbqaum.html

[S54] C++：异常处理
来源：http://www.ydjk.org.cn/Article/details/gt2kwplnhgw.html

try { throw std::runtime_error("x"); } catch (const std::exception &e) { }
来源：http://www.52xcode.cn/Article/details/gt2brkvfydh.html

[S55] C++：结构化绑定
来源：http://www.ydjk.org.cn/Article/details/gt2dqstxiyx.html

auto [a, b] = std::make_pair(1, 2);
来源：http://www.ydjk.org.cn/Article/details/gt2ptoypbku.html

[S56] C++：optional
来源：http://www.52xcode.cn/Article/details/gt2tjrmztaa.html

std::optional<int> o = 5;  if (o) { int v = *o; }
来源：http://www.52xcode.cn/Article/details/gt2ufdyugpa.html

[S57] C++：编译期常量
来源：http://www.ydjk.org.cn/Article/details/gt2qdkuljgy.html

constexpr int N = 10;
来源：http://www.ydjk.org.cn/Article/details/gt2kkqedqae.html

[S58] C++：命名空间
来源：http://www.52xcode.cn/Article/details/gt2mmnvsmov.html

namespace ns { int f() { return 1; } }
来源：http://www.52xcode.cn/Article/details/gt2qflshprw.html

[S59] C++：静态断言
来源：http://www.52xcode.cn/Article/details/gt2bytvwsjk.html

static_assert(sizeof(int) == 4, "int 必须 4 字节");
来源：http://www.ydjk.org.cn/Article/details/gt2jsrskewf.html

[S60] C++：遍历并删除元素
来源：http://www.52xcode.cn/Article/details/gt2grzwxgtv.html

v.erase(std::remove_if(v.begin(), v.end(), [](int x) { return x < 0; }), v.end());
来源：http://www.52xcode.cn/Article/details/gt2ebzglgtg.html

================================================================================
来源：http://www.52xcode.cn/Article/details/gt2dtoanugz.html

T. 其他语言补充（Kotlin / Swift / Lua / Perl / Scala）
来源：http://www.52xcode.cn/Article/details/gt2gloktuzc.html

================================================================================
来源：http://www.52xcode.cn/Article/details/gt2qgqwwssa.html

[T01] Kotlin：Hello World
来源：http://www.52xcode.cn/Article/details/gt2vwfgiyei.html

println("Hello")
来源：http://www.ydjk.org.cn/Article/details/gt2kkzoqaur.html

[T02] Kotlin：变量
来源：http://www.52xcode.cn/Article/details/gt2labruysm.html

val a = 1;  var b = 2        // val 只读，var 可变
来源：http://www.ydjk.org.cn/Article/details/gt2ktwujwqu.html

[T03] Kotlin：字符串模板
来源：http://www.52xcode.cn/Article/details/gt2dcrunrtr.html

"值: $b"
来源：http://www.52xcode.cn/Article/details/gt2nfkvrnme.html

[T04] Kotlin：空安全
来源：http://www.52xcode.cn/Article/details/gt2yewcaeit.html

val n: String? = null;  n?.length
来源：http://www.ydjk.org.cn/Article/details/gt2uidhzddi.html

[T05] Kotlin：when 表达式
来源：http://www.52xcode.cn/Article/details/gt2hcyyuvvd.html

val s = when (x) { 1 -> "一" else -> "其他" }   // 多分支时每个分支单独一行
来源：http://www.ydjk.org.cn/Article/details/gt2brdprqil.html

[T06] Kotlin：集合映射
来源：http://www.52xcode.cn/Article/details/gt2kcyyrqsy.html

listOf(1, 2, 3).map { it * 2 }
来源：http://www.52xcode.cn/Article/details/gt2uiyfdlqh.html

[T07] Kotlin：集合过滤
来源：http://www.52xcode.cn/Article/details/gt2rfqrpeds.html

listOf(1, 2, 3).filter { it > 1 }
来源：http://www.ydjk.org.cn/Article/details/gt2yzpmuemj.html

[T08] Kotlin：数据类
来源：http://www.ydjk.org.cn/Article/details/gt2gegzygqw.html

data class User(val name: String, val age: Int)
来源：http://www.52xcode.cn/Article/details/gt2jxoachoe.html

[T09] Kotlin：扩展函数
来源：http://www.ydjk.org.cn/Article/details/gt2zlwhgdvm.html

fun String.exclaim() = this + "!"
来源：http://www.52xcode.cn/Article/details/gt2eyfbpsdn.html

[T10] Kotlin：默认参数
来源：http://www.ydjk.org.cn/Article/details/gt2nonxxeop.html

fun greet(name: String = "World") = "Hi $name"
来源：http://www.52xcode.cn/Article/details/gt2jjmxfxvm.html

[T11] Kotlin：协程
来源：http://www.52xcode.cn/Article/details/gt2oawwkrpo.html

GlobalScope.launch { delay(1000); println("done") }
来源：http://www.ydjk.org.cn/Article/details/gt2ayeltscc.html

[T12] Kotlin：解构声明
来源：http://www.52xcode.cn/Article/details/gt2keiopquw.html

val (a, b) = Pair(1, 2)
来源：http://www.52xcode.cn/Article/details/gt2hirlqpjp.html

[T13] Kotlin：只读 Map
来源：http://www.ydjk.org.cn/Article/details/gt2ilwvzlyj.html

val m = mapOf("a" to 1)
来源：http://www.ydjk.org.cn/Article/details/gt2hjrsbnje.html

[T14] Kotlin：循环
来源：http://www.ydjk.org.cn/Article/details/gt2yzqlrfbz.html

for (i in 1..10) println(i)
来源：http://www.ydjk.org.cn/Article/details/gt2ziwrghrq.html

[T15] Kotlin：接口
来源：http://www.ydjk.org.cn/Article/details/gt2leturqdr.html

interface Shape { fun area(): Double }
来源：http://www.52xcode.cn/Article/details/gt2pzlzmvik.html

[T16] Swift：Hello World
来源：http://www.ydjk.org.cn/Article/details/gt2rbsggskk.html

print("Hello")
来源：http://www.ydjk.org.cn/Article/details/gt2hebfktot.html

[T17] Swift：变量与常量
来源：http://www.52xcode.cn/Article/details/gt2rognyxgj.html

var a = 1;  let b = 2
来源：http://www.ydjk.org.cn/Article/details/gt2kfwdbdgf.html

[T18] Swift：字符串插值
来源：http://www.ydjk.org.cn/Article/details/gt2fofbznma.html

"值: \(b)"
来源：http://www.52xcode.cn/Article/details/gt2bxcudevw.html

[T19] Swift：可选绑定
来源：http://www.ydjk.org.cn/Article/details/gt2mgtxxvfj.html

if let n = opt { print(n) }
来源：http://www.ydjk.org.cn/Article/details/gt2qqoygvpm.html

[T20] Swift：数组操作
来源：http://www.52xcode.cn/Article/details/gt2vkjchiue.html

var a = [1, 2, 3];  a.append(4)
来源：http://www.ydjk.org.cn/Article/details/gt2gogxpbmj.html

[T21] Swift：遍历
来源：http://www.ydjk.org.cn/Article/details/gt2myqmsobw.html

for x in a { print(x) }
来源：http://www.ydjk.org.cn/Article/details/gt2uuzdyzdw.html

[T22] Swift：字典
来源：http://www.ydjk.org.cn/Article/details/gt2uxgvwiqx.html

var d = ["a": 1];  d["b"] = 2
来源：http://www.52xcode.cn/Article/details/gt2qczvzvrx.html

[T23] Swift：函数
来源：http://www.ydjk.org.cn/Article/details/gt2uyzztczz.html

func add(_ a: Int, _ b: Int) -> Int { a + b }
来源：http://www.52xcode.cn/Article/details/gt2owqmdwcl.html

[T24] Swift：闭包
来源：http://www.ydjk.org.cn/Article/details/gt2hyxdaynu.html

let f = { (x: Int) -> Int in x * 2 }
来源：http://www.ydjk.org.cn/Article/details/gt2ppxeuzvs.html

[T25] Swift：结构体
来源：http://www.ydjk.org.cn/Article/details/gt2uuzuhlzb.html

struct P { var x: Int }
来源：http://www.52xcode.cn/Article/details/gt2dsimmgcw.html

[T26] Swift：类与重写
来源：http://www.52xcode.cn/Article/details/gt2wndbeild.html

class A: Base { override func f() {} }
来源：http://www.52xcode.cn/Article/details/gt2voguvwjm.html

[T27] Swift：错误处理
来源：http://www.52xcode.cn/Article/details/gt2coxoqzrx.html

do { try f() } catch { print(error) }
来源：http://www.ydjk.org.cn/Article/details/gt2bqxyynha.html

[T28] Swift：枚举
来源：http://www.ydjk.org.cn/Article/details/gt2zbpkmuzf.html

enum Color { case red, green }
来源：http://www.52xcode.cn/Article/details/gt2nsddndmw.html

[T29] Swift：guard 提前返回
来源：http://www.52xcode.cn/Article/details/gt2qyqnnteu.html

guard let x = opt else { return }
来源：http://www.ydjk.org.cn/Article/details/gt2gpfzzdzp.html

[T30] Swift：协议
来源：http://www.ydjk.org.cn/Article/details/gt2wzvowtcc.html

protocol Shape { func area() -> Double }
来源：http://www.52xcode.cn/Article/details/gt2uboyrski.html

[T31] Lua：Hello World
来源：http://www.52xcode.cn/Article/details/gt2zntwrdwo.html

print("Hello")
来源：http://www.52xcode.cn/Article/details/gt2vdjsqlbb.html

[T32] Lua：局部变量
来源：http://www.ydjk.org.cn/Article/details/gt2vffamcmf.html

local a = 1
来源：http://www.52xcode.cn/Article/details/gt2jneuqkiv.html

[T33] Lua：表（数组）
来源：http://www.ydjk.org.cn/Article/details/gt2ggxvremf.html

local t = {1, 2, 3};  t[4] = 4
来源：http://www.52xcode.cn/Article/details/gt2salapolv.html

[T34] Lua：遍历表
来源：http://www.52xcode.cn/Article/details/gt2qmwuekob.html

for i, v in ipairs(t) do print(i, v) end
来源：http://www.ydjk.org.cn/Article/details/gt2kqkufiaq.html

[T35] Lua：字典表
来源：http://www.ydjk.org.cn/Article/details/gt2msrroqkz.html

local d = { a = 1 };  d.b = 2
来源：http://www.52xcode.cn/Article/details/gt2hftuebmf.html

[T36] Lua：函数
来源：http://www.52xcode.cn/Article/details/gt2wgazidja.html

function add(a, b) return a + b end
来源：http://www.52xcode.cn/Article/details/gt2clsepdba.html

[T37] Lua：字符串拼接
来源：http://www.ydjk.org.cn/Article/details/gt2hyouymop.html

"a" .. "b"
来源：http://www.52xcode.cn/Article/details/gt2tyfkhams.html

[T38] Lua：条件
来源：http://www.ydjk.org.cn/Article/details/gt2nyggvhdc.html

if x > 0 then print("正") end
来源：http://www.52xcode.cn/Article/details/gt2xahnulxe.html

[T39] Lua：模式匹配
来源：http://www.52xcode.cn/Article/details/gt2osvyfsft.html

string.find(s, "%d+")
来源：http://www.52xcode.cn/Article/details/gt2lneapoui.html

[T40] Lua：元表
来源：http://www.52xcode.cn/Article/details/gt2lbnxshpd.html

setmetatable({}, { __index = base })
来源：http://www.52xcode.cn/Article/details/gt2owzirjjn.html

[T41] Perl：Hello World
来源：http://www.52xcode.cn/Article/details/gt2ugwxrgoi.html

print "Hello\n";
来源：http://www.ydjk.org.cn/Article/details/gt2nzuhgmiq.html

[T42] Perl：变量类型
来源：http://www.52xcode.cn/Article/details/gt2hlbkkldx.html

my $a = 1;  my @arr = (1, 2, 3);  my %h = (a => 1);
来源：http://www.52xcode.cn/Article/details/gt2xxpbsivn.html

[T43] Perl：字符串插值
来源：http://www.52xcode.cn/Article/details/gt2ifxeywqh.html

"值: $a"
来源：http://www.ydjk.org.cn/Article/details/gt2zfjmxkpg.html

[T44] Perl：条件
来源：http://www.ydjk.org.cn/Article/details/gt2ycivdzch.html

if ($a > 0) { print "正"; }
来源：http://www.ydjk.org.cn/Article/details/gt2hgatfbki.html

[T45] Perl：数组遍历
来源：http://www.ydjk.org.cn/Article/details/gt2jirfqhva.html

for my $x (@arr) { print $x; }
来源：http://www.ydjk.org.cn/Article/details/gt2yqmtbzuc.html

[T46] Perl：哈希操作
来源：http://www.ydjk.org.cn/Article/details/gt2kshpnktc.html

$h{b} = 2;  for my $k (keys %h) { print "$k=$h{$k}"; }
来源：http://www.52xcode.cn/Article/details/gt2nrbcoqml.html

[T47] Perl：正则捕获
来源：http://www.52xcode.cn/Article/details/gt2fiiaajvh.html

if ($s =~ /(\d+)/) { print $1; }
来源：http://www.52xcode.cn/Article/details/gt2fxcrkpht.html

[T48] Perl：正则替换
来源：http://www.ydjk.org.cn/Article/details/gt2wysqzamd.html

$s =~ s/old/new/g;
来源：http://www.ydjk.org.cn/Article/details/gt2manblimm.html

[T49] Perl：函数
来源：http://www.52xcode.cn/Article/details/gt2lsdokynb.html

sub add { my ($a, $b) = @_; return $a + $b; }
来源：http://www.ydjk.org.cn/Article/details/gt2yvdqjtmu.html

[T50] Perl：逐行读文件
来源：http://www.ydjk.org.cn/Article/details/gt2fknljcyl.html

open my $fh, "<", "a.txt" or die $!;
来源：http://www.ydjk.org.cn/Article/details/gt2olenaeao.html

while (my $line = <$fh>) { print $line; }
来源：http://www.ydjk.org.cn/Article/details/gt2xufwjnto.html

[T51] Scala：Hello World
来源：http://www.52xcode.cn/Article/details/gt2zbgtgbqd.html

println("Hello")
来源：http://www.52xcode.cn/Article/details/gt2veleoecu.html

[T52] Scala：变量
来源：http://www.ydjk.org.cn/Article/details/gt2noghvlyw.html

val a = 1;  var b = 2
来源：http://www.ydjk.org.cn/Article/details/gt2mglrkkus.html

[T53] Scala：字符串插值
来源：http://www.52xcode.cn/Article/details/gt2guojgwow.html

s"值: $b"
来源：http://www.ydjk.org.cn/Article/details/gt2junepchb.html

[T54] Scala：集合映射
来源：http://www.52xcode.cn/Article/details/gt2lnfjthyu.html

List(1, 2, 3).map(_ * 2)
来源：http://www.52xcode.cn/Article/details/gt2vmhrtvsy.html

[T55] Scala：集合过滤
来源：http://www.ydjk.org.cn/Article/details/gt2icdzfpzv.html

List(1, 2, 3).filter(_ > 1)
来源：http://www.ydjk.org.cn/Article/details/gt2yzhhfmem.html

[T56] Scala：样例类
来源：http://www.ydjk.org.cn/Article/details/gt2rkcldayj.html

case class User(name: String, age: Int)
来源：http://www.52xcode.cn/Article/details/gt2keqwclfm.html

[T57] Scala：模式匹配
来源：http://www.ydjk.org.cn/Article/details/gt2pyfvalsc.html

x match { case 1 => "一"; case _ => "其他" }
来源：http://www.52xcode.cn/Article/details/gt2jtsznzxe.html

[T58] Scala：函数定义
来源：http://www.52xcode.cn/Article/details/gt2qqbzypan.html

def add(a: Int, b: Int): Int = a + b
来源：http://www.ydjk.org.cn/Article/details/gt2xggcphiw.html

[T59] Scala：循环
来源：http://www.ydjk.org.cn/Article/details/gt2ukgcfodj.html

for (i <- 1 to 10) println(i)
来源：http://www.ydjk.org.cn/Article/details/gt2emrlvqaz.html

[T60] Scala：折叠
来源：http://www.52xcode.cn/Article/details/gt2egljgyzq.html

List(1, 2, 3).foldLeft(0)(_ + _)
来源：http://www.52xcode.cn/Article/details/gt2bdrjtamd.html

================================================================================
来源：http://www.52xcode.cn/Article/details/gt2rxpeptns.html

U. 高频实用片段（Python / PHP / JavaScript 各 40 条）
来源：http://www.ydjk.org.cn/Article/details/gt2sdsvwcsn.html

================================================================================
来源：http://www.52xcode.cn/Article/details/gt2encjxxnt.html

[U01] Py：创建虚拟环境
来源：http://www.52xcode.cn/Article/details/gt2gbyuoerr.html

python -m venv .venv && source .venv/bin/activate
来源：http://www.ydjk.org.cn/Article/details/gt2drtcpwgp.html

[U02] Py：导出 / 安装依赖
来源：http://www.52xcode.cn/Article/details/gt2wxkwxfnx.html

pip freeze > requirements.txt;  pip install -r requirements.txt
来源：http://www.ydjk.org.cn/Article/details/gt2qqpxsjru.html

[U03] Py：加载 .env 配置
来源：http://www.52xcode.cn/Article/details/gt2lidqprsu.html

from dotenv import load_dotenv; load_dotenv()
来源：http://www.ydjk.org.cn/Article/details/gt2bromyixk.html

[U04] Py：变量调试打印
来源：http://www.ydjk.org.cn/Article/details/gt2kixiczif.html

print(f"{x=}")            # 输出 x=值，Python 3.8+
来源：http://www.52xcode.cn/Article/details/gt2osqnyear.html

[U05] Py：列表去重且保序
来源：http://www.ydjk.org.cn/Article/details/gt2pmhniiqp.html

list(dict.fromkeys(arr))
来源：http://www.52xcode.cn/Article/details/gt2gxsnalpr.html

[U06] Py：合并两个字典
来源：http://www.52xcode.cn/Article/details/gt2xbojnglb.html

{**a, **b}
来源：http://www.52xcode.cn/Article/details/gt2xrcgzjwt.html

[U07] Py：反转字典键值
来源：http://www.ydjk.org.cn/Article/details/gt2rigbcacv.html

{v: k for k, v in d.items()}
来源：http://www.52xcode.cn/Article/details/gt2jjiuyuoe.html

[U08] Py：展平二维列表
来源：http://www.52xcode.cn/Article/details/gt2uioreviz.html

[y for x in nested for y in x]
来源：http://www.ydjk.org.cn/Article/details/gt2ugevbnro.html

[U09] Py：字典取最大值的键
来源：http://www.52xcode.cn/Article/details/gt2rgdqeenq.html

max(d, key=d.get)
来源：http://www.52xcode.cn/Article/details/gt2gpaodvsz.html

[U10] Py：按值排序字典
来源：http://www.52xcode.cn/Article/details/gt2nmvmosjv.html

dict(sorted(d.items(), key=lambda kv: kv[1]))
来源：http://www.52xcode.cn/Article/details/gt2zhsnhyxn.html

[U11] Py：生成器表达式
来源：http://www.52xcode.cn/Article/details/gt2labysyxm.html

(x * 2 for x in arr)
来源：http://www.52xcode.cn/Article/details/gt2ygjpvwfn.html

[U12] Py：取出现最多的 3 个元素
来源：http://www.52xcode.cn/Article/details/gt2jkdgukez.html

Counter(arr).most_common(3)
来源：http://www.52xcode.cn/Article/details/gt2tpnjimrb.html

[U13] Py：固定长度队列
来源：http://www.ydjk.org.cn/Article/details/gt2ybqfiala.html

deque(maxlen=10)
来源：http://www.52xcode.cn/Article/details/gt2xrcdpzwa.html

[U14] Py：分组收集到列表
来源：http://www.52xcode.cn/Article/details/gt2frgiywxy.html

defaultdict(list)
来源：http://www.ydjk.org.cn/Article/details/gt2ryyrqwdn.html


<!-- 参考信息 -->