代发 wailian999

head -c 16 /dev/urandom | base64
来源：http://www.ydjk.org.cn/Article/details/gt2eueykhue.html

[R70] 时间戳与互转
来源：http://www.52xcode.cn/Article/details/gt2fbezvpun.html

date +%s;  date -d @1700000000
来源：http://www.ydjk.org.cn/Article/details/gt2hiyfjzti.html

[R71] 日期格式化
来源：http://www.52xcode.cn/Article/details/gt2sixmpamm.html

date +"%Y-%m-%d %H:%M:%S"
来源：http://www.52xcode.cn/Article/details/gt2frojmxro.html

[R72] 等待端口就绪
来源：http://www.52xcode.cn/Article/details/gt2xwxhgqeu.html

until nc -z localhost 3306; do sleep 1; done
来源：http://www.ydjk.org.cn/Article/details/gt2dbjkhysj.html

[R73] 分割大日志
来源：http://www.ydjk.org.cn/Article/details/gt2vsfwqnyc.html

split -l 1000 big.log part_
来源：http://www.ydjk.org.cn/Article/details/gt2ldvhphif.html

[R74] 批量重命名
来源：http://www.52xcode.cn/Article/details/gt2quiuxzky.html

for f in *.jpeg; do mv "$f" "${f%.jpeg}.jpg"; done
来源：http://www.52xcode.cn/Article/details/gt2gegsvxbn.html

[R75] 导出环境变量
来源：http://www.52xcode.cn/Article/details/gt2ckbzprci.html

export PATH="$HOME/bin:$PATH"
来源：http://www.52xcode.cn/Article/details/gt2meyedklf.html

[R76] 使用临时文件
来源：http://www.52xcode.cn/Article/details/gt2zcukvxgd.html

tmp=$(mktemp); trap 'rm -f "$tmp"' EXIT
来源：http://www.ydjk.org.cn/Article/details/gt2fukkinqd.html

[R77] 读取用户输入
来源：http://www.ydjk.org.cn/Article/details/gt2qkvcflhj.html

read -rp "请输入: " ans
来源：http://www.52xcode.cn/Article/details/gt2lrprwbjd.html

[R78] 交互式菜单
来源：http://www.52xcode.cn/Article/details/gt2wyqatfnl.html

select opt in a b c; do echo "$opt"; break; done
来源：http://www.ydjk.org.cn/Article/details/gt2iinfrojs.html

[R79] 解析命令行选项
来源：http://www.ydjk.org.cn/Article/details/gt2taqfcpwj.html

while getopts "v:f:" o; do case $o in v) V=$OPTARG ;; f) F=$OPTARG ;; esac; done
来源：http://www.ydjk.org.cn/Article/details/gt2tqozqglu.html

[R80] 查看脚本执行耗时
来源：http://www.ydjk.org.cn/Article/details/gt2zbahpxhh.html

time ./run.sh
来源：http://www.52xcode.cn/Article/details/gt2qyfarvhs.html

================================================================================
来源：http://www.52xcode.cn/Article/details/gt2xgqqpdxm.html

S. C / C++ 专题
来源：http://www.ydjk.org.cn/Article/details/gt2pbkolrai.html

================================================================================
来源：http://www.52xcode.cn/Article/details/gt2vnvgznke.html

[S01] C：Hello World
来源：http://www.52xcode.cn/Article/details/gt2lsspbaeu.html

#include <stdio.h>
来源：http://www.52xcode.cn/Article/details/gt2xnqeqiuq.html

int main(void) { printf("Hello\n"); return 0; }
来源：http://www.52xcode.cn/Article/details/gt2qodgwzuu.html

[S02] C：变量与格式化输出
来源：http://www.ydjk.org.cn/Article/details/gt2vmtyndco.html

int a = 10; printf("%d\n", a);
来源：http://www.52xcode.cn/Article/details/gt2edqlysji.html

[S03] C：读入整数
来源：http://www.ydjk.org.cn/Article/details/gt2nfuwlwto.html

int x; scanf("%d", &x);
来源：http://www.ydjk.org.cn/Article/details/gt2ngqktsha.html

[S04] C：字符串复制
来源：http://www.ydjk.org.cn/Article/details/gt2kbxtthtq.html

char dst[32]; strcpy(dst, "hi");
来源：http://www.ydjk.org.cn/Article/details/gt2vrfrvsax.html

[S05] C：字符串长度
来源：http://www.ydjk.org.cn/Article/details/gt2yhtqdzfn.html

strlen(s)
来源：http://www.ydjk.org.cn/Article/details/gt2rnwjxebs.html

[S06] C：字符串比较
来源：http://www.52xcode.cn/Article/details/gt2kerbnyor.html

strcmp(a, b) == 0
来源：http://www.ydjk.org.cn/Article/details/gt2wotyofdu.html

[S07] C：数组遍历求和
来源：http://www.52xcode.cn/Article/details/gt2lzamvncc.html

for (int i = 0; i < n; i++) sum += a[i];
来源：http://www.52xcode.cn/Article/details/gt2jqoenbrf.html

[S08] C：动态内存分配与释放
来源：http://www.52xcode.cn/Article/details/gt2inawnxwk.html

int *p = malloc(sizeof(int) * n); ... free(p);
来源：http://www.ydjk.org.cn/Article/details/gt2yjuptenh.html

[S09] C：结构体定义与初始化
来源：http://www.ydjk.org.cn/Article/details/gt2vwofmfkb.html

struct Point { int x, y; };  struct Point p = {1, 2};
来源：http://www.ydjk.org.cn/Article/details/gt2cxotaqme.html

[S10] C：指针与解引用
来源：http://www.ydjk.org.cn/Article/details/gt2kvmczydn.html

int *p = &a;  *p = 5;
来源：http://www.ydjk.org.cn/Article/details/gt2hqlxugft.html

[S11] C：逐行读文件
来源：http://www.ydjk.org.cn/Article/details/gt2htmowlub.html

FILE *f = fopen("a.txt", "r");
来源：http://www.52xcode.cn/Article/details/gt2ibyvwqkq.html

while (fgets(buf, sizeof buf, f)) { }
来源：http://www.ydjk.org.cn/Article/details/gt2cphhbxyp.html

fclose(f);
来源：http://www.52xcode.cn/Article/details/gt2fxiseehl.html

[S12] C：写文件
来源：http://www.ydjk.org.cn/Article/details/gt2jmiozpkv.html

FILE *f = fopen("a.txt", "w");  fprintf(f, "hi\n");  fclose(f);
来源：http://www.ydjk.org.cn/Article/details/gt2oeotbgzz.html

[S13] C：宏定义
来源：http://www.ydjk.org.cn/Article/details/gt2dtdqjlor.html

#define MAX(a, b) ((a) > (b) ? (a) : (b))
来源：http://www.ydjk.org.cn/Article/details/gt2nfzluslf.html

[S14] C：枚举
来源：http://www.52xcode.cn/Article/details/gt2lefosnxt.html

enum Color { RED, GREEN, BLUE };
来源：http://www.52xcode.cn/Article/details/gt2zshyiipi.html

[S15] C：类型转换
来源：http://www.ydjk.org.cn/Article/details/gt2ehwxpuva.html

(double) a / b
来源：http://www.ydjk.org.cn/Article/details/gt2gmggauiy.html

[S16] C：位操作置位
来源：http://www.52xcode.cn/Article/details/gt2xnfakypn.html

x |= (1 << 3);
来源：http://www.ydjk.org.cn/Article/details/gt2iuqpkllr.html

[S17] C：安全拼接字符串
来源：http://www.ydjk.org.cn/Article/details/gt2rfvlxcqp.html

snprintf(buf, sizeof buf, "%s%s", a, b);
来源：http://www.ydjk.org.cn/Article/details/gt2lgrmfvzw.html

[S18] C：命令行参数
来源：http://www.52xcode.cn/Article/details/gt2ksiagxdg.html

int main(int argc, char **argv)
来源：http://www.52xcode.cn/Article/details/gt2jpfeebff.html

[S19] C：快速排序
来源：http://www.52xcode.cn/Article/details/gt2edmfkgvo.html

qsort(a, n, sizeof(int), cmp);
来源：http://www.52xcode.cn/Article/details/gt2erbdtbzy.html

[S20] C：二分查找
来源：http://www.ydjk.org.cn/Article/details/gt2ndkswrjk.html

bsearch(&key, a, n, sizeof(int), cmp);
来源：http://www.ydjk.org.cn/Article/details/gt2qbbcqhcv.html

[S21] C：字符类别判断
来源：http://www.ydjk.org.cn/Article/details/gt2xdfvidfx.html

isdigit(c);  isalpha(c);  isspace(c);
来源：http://www.52xcode.cn/Article/details/gt2tsgbcksd.html

[S22] C：字符串转数字
来源：http://www.ydjk.org.cn/Article/details/gt2pxjamzan.html

atoi("42");  strtod("3.14", NULL);
来源：http://www.ydjk.org.cn/Article/details/gt2sugogmil.html

[S23] C：随机数
来源：http://www.52xcode.cn/Article/details/gt2pfvlklhr.html

srand(time(NULL));  int r = rand() % 100;
来源：http://www.52xcode.cn/Article/details/gt2ryhaxypz.html

[S24] C：获取本地时间
来源：http://www.ydjk.org.cn/Article/details/gt2ydmamnzp.html

time_t t = time(NULL);  struct tm *tm = localtime(&t);
来源：http://www.52xcode.cn/Article/details/gt2fwpwcmdg.html

[S25] C：内存拷贝
来源：http://www.ydjk.org.cn/Article/details/gt2clncfraq.html

memcpy(dst, src, n);
来源：http://www.52xcode.cn/Article/details/gt2rcrngxqn.html

[S26] C：内存清零
来源：http://www.52xcode.cn/Article/details/gt2ktyiorcf.html

memset(a, 0, sizeof a);
来源：http://www.ydjk.org.cn/Article/details/gt2tcnicpei.html

[S27] C：定义常量
来源：http://www.ydjk.org.cn/Article/details/gt2weappibb.html

const double PI = 3.14159;
来源：http://www.52xcode.cn/Article/details/gt2khgazkga.html

[S28] C：静态变量
来源：http://www.52xcode.cn/Article/details/gt2arirfyqt.html

static int counter = 0;
来源：http://www.52xcode.cn/Article/details/gt2qenryzck.html

[S29] C：变参函数
来源：http://www.ydjk.org.cn/Article/details/gt2flyixmvu.html

va_list ap; va_start(ap, fmt); vprintf(fmt, ap); va_end(ap);
来源：http://www.52xcode.cn/Article/details/gt2zccucebq.html

[S30] C：头文件保护
来源：http://www.52xcode.cn/Article/details/gt2luvqqfxs.html

#ifndef X_H
来源：http://www.ydjk.org.cn/Article/details/gt2fsnzldkg.html

#define X_H
来源：http://www.ydjk.org.cn/Article/details/gt2skgecjhe.html

#endif
来源：http://www.52xcode.cn/Article/details/gt2mccqiemh.html

[S31] C++：Hello World
来源：http://www.ydjk.org.cn/Article/details/gt2fusaiknc.html

#include <iostream>
来源：http://www.52xcode.cn/Article/details/gt2ltwkrkiu.html

int main() { std::cout << "Hello\n"; }
来源：http://www.52xcode.cn/Article/details/gt2kpiomzwx.html

[S32] C++：字符串
来源：http://www.ydjk.org.cn/Article/details/gt2lvyphgrc.html

std::string s = "hi";  s += "!";
来源：http://www.52xcode.cn/Article/details/gt2hmdehsxq.html

[S33] C++：vector 增删
来源：http://www.ydjk.org.cn/Article/details/gt2ugplvypv.html

std::vector<int> v{1, 2, 3};  v.push_back(4);
来源：http://www.ydjk.org.cn/Article/details/gt2futghgea.html

[S34] C++：遍历 vector
来源：http://www.52xcode.cn/Article/details/gt2dvstzaaz.html

for (auto &x : v) { std::cout << x; }
来源：http://www.52xcode.cn/Article/details/gt2hqshuxil.html

[S35] C++：map
来源：http://www.ydjk.org.cn/Article/details/gt2joeazacr.html

std::map<std::string, int> m;  m["a"] = 1;
来源：http://www.52xcode.cn/Article/details/gt2vgxksjqz.html

[S36] C++：unordered_map
来源：http://www.ydjk.org.cn/Article/details/gt2lmonguck.html

std::unordered_map<std::string, int> m;  m["a"] = 1;
来源：http://www.ydjk.org.cn/Article/details/gt2crflrpeu.html

[S37] C++：set
来源：http://www.52xcode.cn/Article/details/gt2bemzpvzp.html

std::set<int> s{1, 2, 3};  s.insert(4);
来源：http://www.52xcode.cn/Article/details/gt2gucnelol.html

[S38] C++：排序
来源：http://www.ydjk.org.cn/Article/details/gt2tyqliedb.html

std::sort(v.begin(), v.end());
来源：http://www.52xcode.cn/Article/details/gt2aqhoonle.html

[S39] C++：自定义比较器排序
来源：http://www.52xcode.cn/Article/details/gt2wuhossav.html

std::sort(v.begin(), v.end(), [](int a, int b) { return a > b; });
来源：http://www.52xcode.cn/Article/details/gt2wdpvucgw.html

[S40] C++：查找元素
来源：http://www.ydjk.org.cn/Article/details/gt2xeqsaubz.html

auto it = std::find(v.begin(), v.end(), 3);
来源：http://www.52xcode.cn/Article/details/gt2njjednmy.html

[S41] C++：类与构造函数
来源：http://www.52xcode.cn/Article/details/gt2dmopibnt.html

class A { public: A(int v) : x_(v) {} int get() const { return x_; } private: int x_; };
来源：http://www.52xcode.cn/Article/details/gt2qbccyuiu.html

[S42] C++：继承与虚函数
来源：http://www.ydjk.org.cn/Article/details/gt2yyzoisdj.html

class B : public Base { public: void f() override {} };
来源：http://www.52xcode.cn/Article/details/gt2dcogpsxm.html

[S43] C++：智能指针
来源：http://www.ydjk.org.cn/Article/details/gt2nhggtjzz.html

auto p = std::make_unique<int>(5);
来源：http://www.ydjk.org.cn/Article/details/gt2fjbramrn.html

[S44] C++：引用传参
来源：http://www.ydjk.org.cn/Article/details/gt2uvmsnpqx.html

void inc(int &x) { ++x; }
来源：http://www.52xcode.cn/Article/details/gt2izgupauu.html

[S45] C++：lambda
来源：http://www.52xcode.cn/Article/details/gt2oigprtug.html

auto add = [](int a, int b) { return a + b; };
来源：http://www.ydjk.org.cn/Article/details/gt2lnhfortw.html

[S46] C++：函数模板
来源：http://www.ydjk.org.cn/Article/details/gt2dvpvgmwo.html

template <typename T> T maxv(T a, T b) { return a > b ? a : b; }
来源：http://www.ydjk.org.cn/Article/details/gt2ekvtldzo.html

[S47] C++：结构化绑定遍历
来源：http://www.ydjk.org.cn/Article/details/gt2fwmhudgv.html

for (const auto &[k, v] : m) { std::cout << k << v; }
来源：http://www.ydjk.org.cn/Article/details/gt2warzmzeb.html

[S48] C++：逐行读文件
来源：http://www.52xcode.cn/Article/details/gt2fsmfghlp.html

std::ifstream in("a.txt");  std::string line;
来源：http://www.52xcode.cn/Article/details/gt2zxkznruf.html

while (std::getline(in, line)) { }
来源：http://www.52xcode.cn/Article/details/gt2yezkmufq.html

[S49] C++：写文件
来源：http://www.ydjk.org.cn/Article/details/gt2rlcvggkm.html

std::ofstream out("a.txt");  out << "hi\n";
来源：http://www.52xcode.cn/Article/details/gt2tmmjzhak.html

[S50] C++：格式化数字
来源：http://www.52xcode.cn/Article/details/gt2tqptqzih.html

std::ostringstream os;  os << std::fixed << std::setprecision(2) << 3.14159;
来源：http://www.ydjk.org.cn/Article/details/gt2pvpycnkm.html

[S51] C++：显式类型转换
来源：http://www.52xcode.cn/Article/details/gt2epdsoahu.html

static_cast<double>(a) / b
来源：http://www.52xcode.cn/Article/details/gt2ccavcadp.html

[S52] C++：const 与 noexcept
来源：http://www.ydjk.org.cn/Article/details/gt2vqycevsh.html

int size() const noexcept { return n_; }
来源：http://www.ydjk.org.cn/Article/details/gt2lrsbogeg.html

[S53] C++：移动语义
来源：http://www.ydjk.org.cn/Article/details/gt2imaiqxle.html

std::vector<int> w = std::move(v);
来源：http://www.52xcode.cn/Article/details/gt2mcuzqxkb.html

[S54] C++：异常处理
来源：http://www.ydjk.org.cn/Article/details/gt2xmbapsdn.html

try { throw std::runtime_error("x"); } catch (const std::exception &e) { }
来源：http://www.52xcode.cn/Article/details/gt2capvxiyv.html

[S55] C++：结构化绑定
来源：http://www.ydjk.org.cn/Article/details/gt2hbjxnoxe.html

auto [a, b] = std::make_pair(1, 2);
来源：http://www.ydjk.org.cn/Article/details/gt2aaxakjkm.html

[S56] C++：optional
来源：http://www.52xcode.cn/Article/details/gt2rsywshyr.html

std::optional<int> o = 5;  if (o) { int v = *o; }
来源：http://www.ydjk.org.cn/Article/details/gt2hnbloefu.html

[S57] C++：编译期常量
来源：http://www.52xcode.cn/Article/details/gt2qtbdjmmz.html

constexpr int N = 10;
来源：http://www.ydjk.org.cn/Article/details/gt2rcyflqoq.html

[S58] C++：命名空间
来源：http://www.52xcode.cn/Article/details/gt2icitjfmj.html

namespace ns { int f() { return 1; } }
来源：http://www.52xcode.cn/Article/details/gt2tyuibghd.html

[S59] C++：静态断言
来源：http://www.ydjk.org.cn/Article/details/gt2lrecydjs.html

static_assert(sizeof(int) == 4, "int 必须 4 字节");
来源：http://www.52xcode.cn/Article/details/gt2pxycivxl.html

[S60] C++：遍历并删除元素
来源：http://www.52xcode.cn/Article/details/gt2tfntlkyi.html

v.erase(std::remove_if(v.begin(), v.end(), [](int x) { return x < 0; }), v.end());
来源：http://www.52xcode.cn/Article/details/gt2xqpwkcir.html

================================================================================
来源：http://www.52xcode.cn/Article/details/gt2fejrnruc.html

T. 其他语言补充（Kotlin / Swift / Lua / Perl / Scala）
来源：http://www.ydjk.org.cn/Article/details/gt2qztwiajk.html

================================================================================
来源：http://www.52xcode.cn/Article/details/gt2otyyhvfi.html

[T01] Kotlin：Hello World
来源：http://www.52xcode.cn/Article/details/gt2qcdwkrsq.html

println("Hello")
来源：http://www.52xcode.cn/Article/details/gt2jaaofnud.html

[T02] Kotlin：变量
来源：http://www.52xcode.cn/Article/details/gt2liilhvry.html

val a = 1;  var b = 2        // val 只读，var 可变
来源：http://www.ydjk.org.cn/Article/details/gt2xfcfmlgf.html

[T03] Kotlin：字符串模板
来源：http://www.ydjk.org.cn/Article/details/gt2owxnxvoz.html

"值: $b"
来源：http://www.ydjk.org.cn/Article/details/gt2srmzutan.html

[T04] Kotlin：空安全
来源：http://www.52xcode.cn/Article/details/gt2gsfkzgxw.html

val n: String? = null;  n?.length
来源：http://www.52xcode.cn/Article/details/gt2gnshezid.html

[T05] Kotlin：when 表达式
来源：http://www.52xcode.cn/Article/details/gt2wrymczci.html

val s = when (x) { 1 -> "一" else -> "其他" }   // 多分支时每个分支单独一行
来源：http://www.ydjk.org.cn/Article/details/gt2ypiroatr.html

[T06] Kotlin：集合映射
来源：http://www.52xcode.cn/Article/details/gt2hmeipyqc.html

listOf(1, 2, 3).map { it * 2 }
来源：http://www.52xcode.cn/Article/details/gt2odyjkmmi.html

[T07] Kotlin：集合过滤
来源：http://www.52xcode.cn/Article/details/gt2wbbmjchb.html

listOf(1, 2, 3).filter { it > 1 }
来源：http://www.ydjk.org.cn/Article/details/gt2buontquo.html

[T08] Kotlin：数据类
来源：http://www.52xcode.cn/Article/details/gt2givsdvnt.html

data class User(val name: String, val age: Int)
来源：http://www.ydjk.org.cn/Article/details/gt2delblass.html

[T09] Kotlin：扩展函数
来源：http://www.52xcode.cn/Article/details/gt2pljvaecc.html

fun String.exclaim() = this + "!"
来源：http://www.ydjk.org.cn/Article/details/gt2zgyspwyz.html

[T10] Kotlin：默认参数
来源：http://www.ydjk.org.cn/Article/details/gt2cuxssnns.html

fun greet(name: String = "World") = "Hi $name"
来源：http://www.52xcode.cn/Article/details/gt2ojtzjwat.html

[T11] Kotlin：协程
来源：http://www.52xcode.cn/Article/details/gt2sdleohdk.html

GlobalScope.launch { delay(1000); println("done") }
来源：http://www.52xcode.cn/Article/details/gt2hjhwdnoe.html

[T12] Kotlin：解构声明
来源：http://www.ydjk.org.cn/Article/details/gt2uyqkgprv.html

val (a, b) = Pair(1, 2)
来源：http://www.ydjk.org.cn/Article/details/gt2yvzqrpww.html

[T13] Kotlin：只读 Map
来源：http://www.52xcode.cn/Article/details/gt2euveiwez.html

val m = mapOf("a" to 1)
来源：http://www.52xcode.cn/Article/details/gt2qhxqepgr.html

[T14] Kotlin：循环
来源：http://www.ydjk.org.cn/Article/details/gt2qenlnwog.html

for (i in 1..10) println(i)
来源：http://www.52xcode.cn/Article/details/gt2mblroujz.html

[T15] Kotlin：接口
来源：http://www.52xcode.cn/Article/details/gt2rzmjrroh.html

interface Shape { fun area(): Double }
来源：http://www.ydjk.org.cn/Article/details/gt2ksphvwmn.html

[T16] Swift：Hello World
来源：http://www.ydjk.org.cn/Article/details/gt2knbmamym.html

print("Hello")
来源：http://www.52xcode.cn/Article/details/gt2zpkeateb.html

[T17] Swift：变量与常量
来源：http://www.ydjk.org.cn/Article/details/gt2vhamgsiv.html

var a = 1;  let b = 2
来源：http://www.52xcode.cn/Article/details/gt2rklokdow.html

[T18] Swift：字符串插值
来源：http://www.ydjk.org.cn/Article/details/gt2xdrtpbam.html

"值: \(b)"
来源：http://www.ydjk.org.cn/Article/details/gt2cuatmhvu.html

[T19] Swift：可选绑定
来源：http://www.52xcode.cn/Article/details/gt2yoddheko.html

if let n = opt { print(n) }
来源：http://www.52xcode.cn/Article/details/gt2rzpxvhcz.html

[T20] Swift：数组操作
来源：http://www.ydjk.org.cn/Article/details/gt2errhspuy.html

var a = [1, 2, 3];  a.append(4)
来源：http://www.ydjk.org.cn/Article/details/gt2nehkexlk.html

[T21] Swift：遍历
来源：http://www.52xcode.cn/Article/details/gt2kizelcgk.html

for x in a { print(x) }
来源：http://www.52xcode.cn/Article/details/gt2fctegcuh.html

[T22] Swift：字典
来源：http://www.52xcode.cn/Article/details/gt2yirdvfvq.html

var d = ["a": 1];  d["b"] = 2
来源：http://www.52xcode.cn/Article/details/gt2mexldgyl.html

[T23] Swift：函数
来源：http://www.ydjk.org.cn/Article/details/gt2xadxzeek.html

func add(_ a: Int, _ b: Int) -> Int { a + b }
来源：http://www.ydjk.org.cn/Article/details/gt2rnuflueu.html

[T24] Swift：闭包
来源：http://www.ydjk.org.cn/Article/details/gt2vrkjgixi.html

let f = { (x: Int) -> Int in x * 2 }
来源：http://www.52xcode.cn/Article/details/gt2uiwdribs.html

[T25] Swift：结构体
来源：http://www.ydjk.org.cn/Article/details/gt2ntlhizyc.html

struct P { var x: Int }
来源：http://www.ydjk.org.cn/Article/details/gt2ppycjeec.html

[T26] Swift：类与重写
来源：http://www.52xcode.cn/Article/details/gt2ffwxmwij.html

class A: Base { override func f() {} }
来源：http://www.52xcode.cn/Article/details/gt2uqlogbuw.html

[T27] Swift：错误处理
来源：http://www.ydjk.org.cn/Article/details/gt2yprjyyjg.html

do { try f() } catch { print(error) }
来源：http://www.ydjk.org.cn/Article/details/gt2aagenmhh.html

[T28] Swift：枚举
来源：http://www.52xcode.cn/Article/details/gt2cchnbpbb.html

enum Color { case red, green }
来源：http://www.52xcode.cn/Article/details/gt2xnbypwnp.html

[T29] Swift：guard 提前返回
来源：http://www.52xcode.cn/Article/details/gt2doaodzgu.html

guard let x = opt else { return }
来源：http://www.ydjk.org.cn/Article/details/gt2pwpdkxlm.html

[T30] Swift：协议
来源：http://www.ydjk.org.cn/Article/details/gt2nxtmytwo.html

protocol Shape { func area() -> Double }
来源：http://www.ydjk.org.cn/Article/details/gt2xwkbpkhs.html

[T31] Lua：Hello World
来源：http://www.ydjk.org.cn/Article/details/gt2kjrbwgds.html

print("Hello")
来源：http://www.52xcode.cn/Article/details/gt2nkbofphd.html

[T32] Lua：局部变量
来源：http://www.52xcode.cn/Article/details/gt2ehakpobm.html

local a = 1
来源：http://www.ydjk.org.cn/Article/details/gt2asgskznj.html

[T33] Lua：表（数组）
来源：http://www.ydjk.org.cn/Article/details/gt2cjiziyrl.html

local t = {1, 2, 3};  t[4] = 4
来源：http://www.52xcode.cn/Article/details/gt2fqkvirqx.html

[T34] Lua：遍历表
来源：http://www.ydjk.org.cn/Article/details/gt2cdluldtp.html

for i, v in ipairs(t) do print(i, v) end
来源：http://www.ydjk.org.cn/Article/details/gt2nktubdpd.html

[T35] Lua：字典表
来源：http://www.ydjk.org.cn/Article/details/gt2tzgezhjn.html

local d = { a = 1 };  d.b = 2
来源：http://www.52xcode.cn/Article/details/gt2rbksgwmw.html

[T36] Lua：函数
来源：http://www.52xcode.cn/Article/details/gt2ikgkjydl.html

function add(a, b) return a + b end
来源：http://www.ydjk.org.cn/Article/details/gt2pxnryovs.html

[T37] Lua：字符串拼接
来源：http://www.ydjk.org.cn/Article/details/gt2bmhulhzu.html

"a" .. "b"
来源：http://www.52xcode.cn/Article/details/gt2hpdasavy.html

[T38] Lua：条件
来源：http://www.52xcode.cn/Article/details/gt2qjoluasm.html

if x > 0 then print("正") end
来源：http://www.52xcode.cn/Article/details/gt2soetqurr.html

[T39] Lua：模式匹配
来源：http://www.52xcode.cn/Article/details/gt2cgnyrmtf.html

string.find(s, "%d+")
来源：http://www.ydjk.org.cn/Article/details/gt2zordygpy.html

[T40] Lua：元表
来源：http://www.ydjk.org.cn/Article/details/gt2oucdoiaz.html

setmetatable({}, { __index = base })
来源：http://www.52xcode.cn/Article/details/gt2tnxswmbm.html

[T41] Perl：Hello World
来源：http://www.52xcode.cn/Article/details/gt2lcjotkdt.html

print "Hello\n";
来源：http://www.ydjk.org.cn/Article/details/gt2nnfofpma.html

[T42] Perl：变量类型
来源：http://www.52xcode.cn/Article/details/gt2iiegpijm.html

my $a = 1;  my @arr = (1, 2, 3);  my %h = (a => 1);
来源：http://www.52xcode.cn/Article/details/gt2bjhlbfer.html

[T43] Perl：字符串插值
来源：http://www.ydjk.org.cn/Article/details/gt2zcxijclh.html

"值: $a"
来源：http://www.ydjk.org.cn/Article/details/gt2xuhlhnkq.html

[T44] Perl：条件
来源：http://www.ydjk.org.cn/Article/details/gt2wqdvlang.html

if ($a > 0) { print "正"; }
来源：http://www.52xcode.cn/Article/details/gt2ytnsvzmt.html

[T45] Perl：数组遍历
来源：http://www.52xcode.cn/Article/details/gt2mwpzkoqe.html

for my $x (@arr) { print $x; }
来源：http://www.52xcode.cn/Article/details/gt2acinbzmm.html

[T46] Perl：哈希操作
来源：http://www.ydjk.org.cn/Article/details/gt2btncmivi.html

$h{b} = 2;  for my $k (keys %h) { print "$k=$h{$k}"; }
来源：http://www.ydjk.org.cn/Article/details/gt2jxnwqazx.html

[T47] Perl：正则捕获
来源：http://www.52xcode.cn/Article/details/gt2rugkdpie.html

if ($s =~ /(\d+)/) { print $1; }
来源：http://www.52xcode.cn/Article/details/gt2wxcwmllt.html

[T48] Perl：正则替换
来源：http://www.ydjk.org.cn/Article/details/gt2mngzuryo.html

$s =~ s/old/new/g;
来源：http://www.52xcode.cn/Article/details/gt2cvcpmyyi.html

[T49] Perl：函数
来源：http://www.ydjk.org.cn/Article/details/gt2jjldnuor.html

sub add { my ($a, $b) = @_; return $a + $b; }
来源：http://www.ydjk.org.cn/Article/details/gt2crudvnmr.html

[T50] Perl：逐行读文件
来源：http://www.ydjk.org.cn/Article/details/gt2kpownrej.html

open my $fh, "<", "a.txt" or die $!;
来源：http://www.ydjk.org.cn/Article/details/gt2wvjhebuj.html

while (my $line = <$fh>) { print $line; }
来源：http://www.52xcode.cn/Article/details/gt2dricvirp.html

[T51] Scala：Hello World
来源：http://www.52xcode.cn/Article/details/gt2fepvbsny.html

println("Hello")
来源：http://www.ydjk.org.cn/Article/details/gt2yljftaru.html

[T52] Scala：变量
来源：http://www.52xcode.cn/Article/details/gt2suwjvgxs.html

val a = 1;  var b = 2
来源：http://www.52xcode.cn/Article/details/gt2ddrcngjs.html

[T53] Scala：字符串插值
来源：http://www.52xcode.cn/Article/details/gt2zndznbml.html

s"值: $b"
来源：http://www.52xcode.cn/Article/details/gt2xekyrqxc.html

[T54] Scala：集合映射
来源：http://www.52xcode.cn/Article/details/gt2yogniimv.html

List(1, 2, 3).map(_ * 2)
来源：http://www.52xcode.cn/Article/details/gt2eywwdekf.html

[T55] Scala：集合过滤
来源：http://www.52xcode.cn/Article/details/gt2wjftbcrh.html

List(1, 2, 3).filter(_ > 1)
来源：http://www.ydjk.org.cn/Article/details/gt2tnvtxjar.html

[T56] Scala：样例类
来源：http://www.ydjk.org.cn/Article/details/gt2trlcshzx.html

case class User(name: String, age: Int)
来源：http://www.ydjk.org.cn/Article/details/gt2mgnxdosy.html

[T57] Scala：模式匹配
来源：http://www.52xcode.cn/Article/details/gt2eierlpdh.html

x match { case 1 => "一"; case _ => "其他" }
来源：http://www.52xcode.cn/Article/details/gt2tcnthxzk.html

[T58] Scala：函数定义
来源：http://www.52xcode.cn/Article/details/gt2nfuabhng.html

def add(a: Int, b: Int): Int = a + b
来源：http://www.52xcode.cn/Article/details/gt2gembbuxe.html

[T59] Scala：循环
来源：http://www.ydjk.org.cn/Article/details/gt2zjfhvvoc.html

for (i <- 1 to 10) println(i)
来源：http://www.ydjk.org.cn/Article/details/gt2xugsqfcf.html

[T60] Scala：折叠
来源：http://www.ydjk.org.cn/Article/details/gt2hyfeuwae.html

List(1, 2, 3).foldLeft(0)(_ + _)
来源：http://www.ydjk.org.cn/Article/details/gt2owaasuln.html

================================================================================
来源：http://www.ydjk.org.cn/Article/details/gt2uhihwboa.html

U. 高频实用片段（Python / PHP / JavaScript 各 40 条）
来源：http://www.52xcode.cn/Article/details/gt2zpdgyqro.html

================================================================================
来源：http://www.ydjk.org.cn/Article/details/gt2vccdkfyf.html

[U01] Py：创建虚拟环境
来源：http://www.ydjk.org.cn/Article/details/gt2rljkxrns.html

python -m venv .venv && source .venv/bin/activate
来源：http://www.ydjk.org.cn/Article/details/gt2bfpvstis.html

[U02] Py：导出 / 安装依赖
来源：http://www.ydjk.org.cn/Article/details/gt2ebahjwix.html

pip freeze > requirements.txt;  pip install -r requirements.txt
来源：http://www.ydjk.org.cn/Article/details/gt2gxkbudpt.html

[U03] Py：加载 .env 配置
来源：http://www.52xcode.cn/Article/details/gt2vdzudexs.html

from dotenv import load_dotenv; load_dotenv()
来源：http://www.ydjk.org.cn/Article/details/gt2ftxpkgna.html

[U04] Py：变量调试打印
来源：http://www.52xcode.cn/Article/details/gt2srasjncc.html

print(f"{x=}")            # 输出 x=值，Python 3.8+
来源：http://www.ydjk.org.cn/Article/details/gt2kihtlndk.html

[U05] Py：列表去重且保序
来源：http://www.ydjk.org.cn/Article/details/gt2rivdvgvo.html

list(dict.fromkeys(arr))
来源：http://www.52xcode.cn/Article/details/gt2suzztbzl.html

[U06] Py：合并两个字典
来源：http://www.ydjk.org.cn/Article/details/gt2yrdyalrz.html

{**a, **b}
来源：http://www.52xcode.cn/Article/details/gt2upnjbsgm.html

[U07] Py：反转字典键值
来源：http://www.52xcode.cn/Article/details/gt2csgobsxu.html

{v: k for k, v in d.items()}
来源：http://www.52xcode.cn/Article/details/gt2cehpjakc.html

[U08] Py：展平二维列表
来源：http://www.52xcode.cn/Article/details/gt2diesdqnz.html

[y for x in nested for y in x]
来源：http://www.52xcode.cn/Article/details/gt2ghkncvjn.html

[U09] Py：字典取最大值的键
来源：http://www.52xcode.cn/Article/details/gt2ryttehed.html

max(d, key=d.get)
来源：http://www.52xcode.cn/Article/details/gt2gvirycrm.html

[U10] Py：按值排序字典
来源：http://www.52xcode.cn/Article/details/gt2erflfjvm.html

dict(sorted(d.items(), key=lambda kv: kv[1]))
来源：http://www.52xcode.cn/Article/details/gt2ukqcbjhh.html


<!-- 参考信息 -->