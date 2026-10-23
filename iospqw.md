代发 wailian999

head -c 16 /dev/urandom | base64
来源：http://www.ydjk.org.cn/Article/details/gt3dnggvzam.html

[R70] 时间戳与互转
来源：http://www.ydjk.org.cn/Article/details/gt3mrdcyhza.html

date +%s;  date -d @1700000000
来源：http://www.52xcode.cn/Article/details/gt3bdoaftdc.html

[R71] 日期格式化
来源：http://www.ydjk.org.cn/Article/details/gt3yumaggut.html

date +"%Y-%m-%d %H:%M:%S"
来源：http://www.ydjk.org.cn/Article/details/gt3stxijaum.html

[R72] 等待端口就绪
来源：http://www.ydjk.org.cn/Article/details/gt3lluacnow.html

until nc -z localhost 3306; do sleep 1; done
来源：http://www.ydjk.org.cn/Article/details/gt3nxwqsuwu.html

[R73] 分割大日志
来源：http://www.ydjk.org.cn/Article/details/gt3kwcfbjou.html

split -l 1000 big.log part_
来源：http://www.ydjk.org.cn/Article/details/gt3zltktwsl.html

[R74] 批量重命名
来源：http://www.ydjk.org.cn/Article/details/gt3jibcsvay.html

for f in *.jpeg; do mv "$f" "${f%.jpeg}.jpg"; done
来源：http://www.ydjk.org.cn/Article/details/gt3liagcgjn.html

[R75] 导出环境变量
来源：http://www.52xcode.cn/Article/details/gt3zgtudpkb.html

export PATH="$HOME/bin:$PATH"
来源：http://www.52xcode.cn/Article/details/gt3zehwpbhl.html

[R76] 使用临时文件
来源：http://www.ydjk.org.cn/Article/details/gt3yqlmjivy.html

tmp=$(mktemp); trap 'rm -f "$tmp"' EXIT
来源：http://www.52xcode.cn/Article/details/gt3erhoozzi.html

[R77] 读取用户输入
来源：http://www.52xcode.cn/Article/details/gt3jdgydrby.html

read -rp "请输入: " ans
来源：http://www.ydjk.org.cn/Article/details/gt3hxafivpm.html

[R78] 交互式菜单
来源：http://www.ydjk.org.cn/Article/details/gt3fwaopytp.html

select opt in a b c; do echo "$opt"; break; done
来源：http://www.52xcode.cn/Article/details/gt3qthjeuni.html

[R79] 解析命令行选项
来源：http://www.52xcode.cn/Article/details/gt3ycmwakbm.html

while getopts "v:f:" o; do case $o in v) V=$OPTARG ;; f) F=$OPTARG ;; esac; done
来源：http://www.ydjk.org.cn/Article/details/gt3gjcjhjtv.html

[R80] 查看脚本执行耗时
来源：http://www.ydjk.org.cn/Article/details/gt3rzenbnok.html

time ./run.sh
来源：http://www.52xcode.cn/Article/details/gt3jjnkjxxu.html

================================================================================
来源：http://www.ydjk.org.cn/Article/details/gt3grskrupv.html

S. C / C++ 专题
来源：http://www.ydjk.org.cn/Article/details/gt3ohhmhtrk.html

================================================================================
来源：http://www.ydjk.org.cn/Article/details/gt3xgepsmgz.html

[S01] C：Hello World
来源：http://www.52xcode.cn/Article/details/gt3lzhyafkx.html

#include <stdio.h>
来源：http://www.52xcode.cn/Article/details/gt3vtwlzmoe.html

int main(void) { printf("Hello\n"); return 0; }
来源：http://www.ydjk.org.cn/Article/details/gt3yalsysnr.html

[S02] C：变量与格式化输出
来源：http://www.ydjk.org.cn/Article/details/gt3vazfjpvk.html

int a = 10; printf("%d\n", a);
来源：http://www.ydjk.org.cn/Article/details/gt3wtjwgmra.html

[S03] C：读入整数
来源：http://www.ydjk.org.cn/Article/details/gt3wghibzaw.html

int x; scanf("%d", &x);
来源：http://www.52xcode.cn/Article/details/gt3usfcbeei.html

[S04] C：字符串复制
来源：http://www.52xcode.cn/Article/details/gt3iypnverz.html

char dst[32]; strcpy(dst, "hi");
来源：http://www.52xcode.cn/Article/details/gt3qtujpycb.html

[S05] C：字符串长度
来源：http://www.52xcode.cn/Article/details/gt3fmlpzjyh.html

strlen(s)
来源：http://www.ydjk.org.cn/Article/details/gt3rsrflwnj.html

[S06] C：字符串比较
来源：http://www.52xcode.cn/Article/details/gt3bwrluqme.html

strcmp(a, b) == 0
来源：http://www.ydjk.org.cn/Article/details/gt3aexalqqw.html

[S07] C：数组遍历求和
来源：http://www.ydjk.org.cn/Article/details/gt3ujmivesh.html

for (int i = 0; i < n; i++) sum += a[i];
来源：http://www.ydjk.org.cn/Article/details/gt3zloaxihw.html

[S08] C：动态内存分配与释放
来源：http://www.ydjk.org.cn/Article/details/gt3twcfyook.html

int *p = malloc(sizeof(int) * n); ... free(p);
来源：http://www.52xcode.cn/Article/details/gt3kyxcskcb.html

[S09] C：结构体定义与初始化
来源：http://www.ydjk.org.cn/Article/details/gt3leqtxwwz.html

struct Point { int x, y; };  struct Point p = {1, 2};
来源：http://www.52xcode.cn/Article/details/gt3bvmewsml.html

[S10] C：指针与解引用
来源：http://www.52xcode.cn/Article/details/gt3sidbasuo.html

int *p = &a;  *p = 5;
来源：http://www.52xcode.cn/Article/details/gt3hzgxdojk.html

[S11] C：逐行读文件
来源：http://www.52xcode.cn/Article/details/gt3frhmlwsb.html

FILE *f = fopen("a.txt", "r");
来源：http://www.ydjk.org.cn/Article/details/gt3aiabhace.html

while (fgets(buf, sizeof buf, f)) { }
来源：http://www.ydjk.org.cn/Article/details/gt3fthnvycg.html

fclose(f);
来源：http://www.ydjk.org.cn/Article/details/gt3grpmtxvc.html

[S12] C：写文件
来源：http://www.ydjk.org.cn/Article/details/gt3gxehcsbn.html

FILE *f = fopen("a.txt", "w");  fprintf(f, "hi\n");  fclose(f);
来源：http://www.52xcode.cn/Article/details/gt3qdeddxbj.html

[S13] C：宏定义
来源：http://www.52xcode.cn/Article/details/gt3adkumjkk.html

#define MAX(a, b) ((a) > (b) ? (a) : (b))
来源：http://www.52xcode.cn/Article/details/gt3hljeyxsf.html

[S14] C：枚举
来源：http://www.52xcode.cn/Article/details/gt3rshshovb.html

enum Color { RED, GREEN, BLUE };
来源：http://www.ydjk.org.cn/Article/details/gt3yzreeuvx.html

[S15] C：类型转换
来源：http://www.52xcode.cn/Article/details/gt3mklbfjug.html

(double) a / b
来源：http://www.ydjk.org.cn/Article/details/gt3hqtwafex.html

[S16] C：位操作置位
来源：http://www.52xcode.cn/Article/details/gt3cfjnymng.html

x |= (1 << 3);
来源：http://www.ydjk.org.cn/Article/details/gt3huzcjeku.html

[S17] C：安全拼接字符串
来源：http://www.52xcode.cn/Article/details/gt3xvsmbktc.html

snprintf(buf, sizeof buf, "%s%s", a, b);
来源：http://www.ydjk.org.cn/Article/details/gt3timfnhyj.html

[S18] C：命令行参数
来源：http://www.52xcode.cn/Article/details/gt3zuiptxoy.html

int main(int argc, char **argv)
来源：http://www.ydjk.org.cn/Article/details/gt3ervgbsip.html

[S19] C：快速排序
来源：http://www.ydjk.org.cn/Article/details/gt3tihcyoqd.html

qsort(a, n, sizeof(int), cmp);
来源：http://www.52xcode.cn/Article/details/gt3mtnollsb.html

[S20] C：二分查找
来源：http://www.52xcode.cn/Article/details/gt3cvrpskrf.html

bsearch(&key, a, n, sizeof(int), cmp);
来源：http://www.ydjk.org.cn/Article/details/gt3wbprgjre.html

[S21] C：字符类别判断
来源：http://www.52xcode.cn/Article/details/gt3ciajrmdp.html

isdigit(c);  isalpha(c);  isspace(c);
来源：http://www.ydjk.org.cn/Article/details/gt3senooris.html

[S22] C：字符串转数字
来源：http://www.52xcode.cn/Article/details/gt3cspublpm.html

atoi("42");  strtod("3.14", NULL);
来源：http://www.52xcode.cn/Article/details/gt3lbhotwae.html

[S23] C：随机数
来源：http://www.52xcode.cn/Article/details/gt3innmzeeq.html

srand(time(NULL));  int r = rand() % 100;
来源：http://www.52xcode.cn/Article/details/gt3nqfbjwcb.html

[S24] C：获取本地时间
来源：http://www.52xcode.cn/Article/details/gt3pzwtgqvy.html

time_t t = time(NULL);  struct tm *tm = localtime(&t);
来源：http://www.52xcode.cn/Article/details/gt3ulsawnyb.html

[S25] C：内存拷贝
来源：http://www.ydjk.org.cn/Article/details/gt3gdvajxvv.html

memcpy(dst, src, n);
来源：http://www.52xcode.cn/Article/details/gt3wmykijti.html

[S26] C：内存清零
来源：http://www.ydjk.org.cn/Article/details/gt3ckyenovm.html

memset(a, 0, sizeof a);
来源：http://www.ydjk.org.cn/Article/details/gt3nhyozfrf.html

[S27] C：定义常量
来源：http://www.52xcode.cn/Article/details/gt3wjipqgpp.html

const double PI = 3.14159;
来源：http://www.ydjk.org.cn/Article/details/gt3ketgimdo.html

[S28] C：静态变量
来源：http://www.ydjk.org.cn/Article/details/gt3qbyxwidu.html

static int counter = 0;
来源：http://www.52xcode.cn/Article/details/gt3tigqdhya.html

[S29] C：变参函数
来源：http://www.ydjk.org.cn/Article/details/gt3ifcyokrc.html

va_list ap; va_start(ap, fmt); vprintf(fmt, ap); va_end(ap);
来源：http://www.ydjk.org.cn/Article/details/gt3fmayxlbf.html

[S30] C：头文件保护
来源：http://www.52xcode.cn/Article/details/gt3doxwagym.html

#ifndef X_H
来源：http://www.ydjk.org.cn/Article/details/gt3izmvwlpj.html

#define X_H
来源：http://www.ydjk.org.cn/Article/details/gt3htnnbfmj.html

#endif
来源：http://www.ydjk.org.cn/Article/details/gt3wewwxfqx.html

[S31] C++：Hello World
来源：http://www.52xcode.cn/Article/details/gt3xiqmgrsb.html

#include <iostream>
来源：http://www.ydjk.org.cn/Article/details/gt3efrbfdoa.html

int main() { std::cout << "Hello\n"; }
来源：http://www.52xcode.cn/Article/details/gt3zxjwczxh.html

[S32] C++：字符串
来源：http://www.52xcode.cn/Article/details/gt3namwygab.html

std::string s = "hi";  s += "!";
来源：http://www.52xcode.cn/Article/details/gt3rntlzbwg.html

[S33] C++：vector 增删
来源：http://www.ydjk.org.cn/Article/details/gt3djixoqkb.html

std::vector<int> v{1, 2, 3};  v.push_back(4);
来源：http://www.52xcode.cn/Article/details/gt3nwrsbzba.html

[S34] C++：遍历 vector
来源：http://www.ydjk.org.cn/Article/details/gt3mshjrefa.html

for (auto &x : v) { std::cout << x; }
来源：http://www.ydjk.org.cn/Article/details/gt3fnhmevgz.html

[S35] C++：map
来源：http://www.52xcode.cn/Article/details/gt3anggaewr.html

std::map<std::string, int> m;  m["a"] = 1;
来源：http://www.ydjk.org.cn/Article/details/gt3ordbvqfw.html

[S36] C++：unordered_map
来源：http://www.ydjk.org.cn/Article/details/gt3jznbkcaa.html

std::unordered_map<std::string, int> m;  m["a"] = 1;
来源：http://www.ydjk.org.cn/Article/details/gt3nlccahdf.html

[S37] C++：set
来源：http://www.52xcode.cn/Article/details/gt3uxznmnnq.html

std::set<int> s{1, 2, 3};  s.insert(4);
来源：http://www.52xcode.cn/Article/details/gt3mnsbydru.html

[S38] C++：排序
来源：http://www.ydjk.org.cn/Article/details/gt3lhhuaksf.html

std::sort(v.begin(), v.end());
来源：http://www.52xcode.cn/Article/details/gt3bbqfjsdc.html

[S39] C++：自定义比较器排序
来源：http://www.ydjk.org.cn/Article/details/gt3utnpyiya.html

std::sort(v.begin(), v.end(), [](int a, int b) { return a > b; });
来源：http://www.52xcode.cn/Article/details/gt3whzrpcgk.html

[S40] C++：查找元素
来源：http://www.52xcode.cn/Article/details/gt3easzptek.html

auto it = std::find(v.begin(), v.end(), 3);
来源：http://www.ydjk.org.cn/Article/details/gt3xkxlxyjl.html

[S41] C++：类与构造函数
来源：http://www.ydjk.org.cn/Article/details/gt3gkkybldz.html

class A { public: A(int v) : x_(v) {} int get() const { return x_; } private: int x_; };
来源：http://www.ydjk.org.cn/Article/details/gt3tktuqcna.html

[S42] C++：继承与虚函数
来源：http://www.52xcode.cn/Article/details/gt3xwpmwwho.html

class B : public Base { public: void f() override {} };
来源：http://www.52xcode.cn/Article/details/gt3ruevwpbi.html

[S43] C++：智能指针
来源：http://www.52xcode.cn/Article/details/gt3gexbhabb.html

auto p = std::make_unique<int>(5);
来源：http://www.ydjk.org.cn/Article/details/gt3fkrqruyy.html

[S44] C++：引用传参
来源：http://www.ydjk.org.cn/Article/details/gt3bdhoqnum.html

void inc(int &x) { ++x; }
来源：http://www.52xcode.cn/Article/details/gt3phxpmvok.html

[S45] C++：lambda
来源：http://www.52xcode.cn/Article/details/gt3ckynyque.html

auto add = [](int a, int b) { return a + b; };
来源：http://www.52xcode.cn/Article/details/gt3uhtomxft.html

[S46] C++：函数模板
来源：http://www.52xcode.cn/Article/details/gt3tltxgaml.html

template <typename T> T maxv(T a, T b) { return a > b ? a : b; }
来源：http://www.ydjk.org.cn/Article/details/gt3cfjgrajb.html

[S47] C++：结构化绑定遍历
来源：http://www.52xcode.cn/Article/details/gt3yulevvmw.html

for (const auto &[k, v] : m) { std::cout << k << v; }
来源：http://www.ydjk.org.cn/Article/details/gt3iankwwnc.html

[S48] C++：逐行读文件
来源：http://www.ydjk.org.cn/Article/details/gt3ypnafadi.html

std::ifstream in("a.txt");  std::string line;
来源：http://www.ydjk.org.cn/Article/details/gt3dohntdqf.html

while (std::getline(in, line)) { }
来源：http://www.ydjk.org.cn/Article/details/gt3fsubdkep.html

[S49] C++：写文件
来源：http://www.52xcode.cn/Article/details/gt3hngbqaje.html

std::ofstream out("a.txt");  out << "hi\n";
来源：http://www.ydjk.org.cn/Article/details/gt3coewhcxn.html

[S50] C++：格式化数字
来源：http://www.ydjk.org.cn/Article/details/gt3fcsaquyg.html

std::ostringstream os;  os << std::fixed << std::setprecision(2) << 3.14159;
来源：http://www.52xcode.cn/Article/details/gt3xbsnwxub.html

[S51] C++：显式类型转换
来源：http://www.ydjk.org.cn/Article/details/gt3ohtzpmsq.html

static_cast<double>(a) / b
来源：http://www.52xcode.cn/Article/details/gt3gjcxsymt.html

[S52] C++：const 与 noexcept
来源：http://www.ydjk.org.cn/Article/details/gt3ohyvkbft.html

int size() const noexcept { return n_; }
来源：http://www.52xcode.cn/Article/details/gt3afcirqrh.html

[S53] C++：移动语义
来源：http://www.52xcode.cn/Article/details/gt3oawtnnnl.html

std::vector<int> w = std::move(v);
来源：http://www.52xcode.cn/Article/details/gt3aeyopyjg.html

[S54] C++：异常处理
来源：http://www.ydjk.org.cn/Article/details/gt3skycjdrp.html

try { throw std::runtime_error("x"); } catch (const std::exception &e) { }
来源：http://www.52xcode.cn/Article/details/gt3zrhzkimu.html

[S55] C++：结构化绑定
来源：http://www.52xcode.cn/Article/details/gt3apkyuykd.html

auto [a, b] = std::make_pair(1, 2);
来源：http://www.ydjk.org.cn/Article/details/gt3luvpycji.html

[S56] C++：optional
来源：http://www.ydjk.org.cn/Article/details/gt3ocdhzyjk.html

std::optional<int> o = 5;  if (o) { int v = *o; }
来源：http://www.ydjk.org.cn/Article/details/gt3lhcicvll.html

[S57] C++：编译期常量
来源：http://www.ydjk.org.cn/Article/details/gt3sjxmkgcd.html

constexpr int N = 10;
来源：http://www.ydjk.org.cn/Article/details/gt3avvcagfm.html

[S58] C++：命名空间
来源：http://www.52xcode.cn/Article/details/gt3owttsola.html

namespace ns { int f() { return 1; } }
来源：http://www.52xcode.cn/Article/details/gt3yctnsepx.html

[S59] C++：静态断言
来源：http://www.52xcode.cn/Article/details/gt3tsveeazh.html

static_assert(sizeof(int) == 4, "int 必须 4 字节");
来源：http://www.52xcode.cn/Article/details/gt3qjoidfki.html

[S60] C++：遍历并删除元素
来源：http://www.ydjk.org.cn/Article/details/gt3iunmnbqr.html

v.erase(std::remove_if(v.begin(), v.end(), [](int x) { return x < 0; }), v.end());
来源：http://www.ydjk.org.cn/Article/details/gt3dhtpxvbu.html

================================================================================
来源：http://www.ydjk.org.cn/Article/details/gt3jzsqlkpq.html

T. 其他语言补充（Kotlin / Swift / Lua / Perl / Scala）
来源：http://www.52xcode.cn/Article/details/gt3gxqlqusf.html

================================================================================
来源：http://www.52xcode.cn/Article/details/gt3dzqwzjwy.html

[T01] Kotlin：Hello World
来源：http://www.ydjk.org.cn/Article/details/gt3byjlbyzi.html

println("Hello")
来源：http://www.52xcode.cn/Article/details/gt3aijzbfrv.html

[T02] Kotlin：变量
来源：http://www.ydjk.org.cn/Article/details/gt3sbqbxmqt.html

val a = 1;  var b = 2        // val 只读，var 可变
来源：http://www.ydjk.org.cn/Article/details/gt3ppjecdzb.html

[T03] Kotlin：字符串模板
来源：http://www.52xcode.cn/Article/details/gt3cqwsbjct.html

"值: $b"
来源：http://www.52xcode.cn/Article/details/gt3uqchoier.html

[T04] Kotlin：空安全
来源：http://www.52xcode.cn/Article/details/gt3vxzmiwep.html

val n: String? = null;  n?.length
来源：http://www.52xcode.cn/Article/details/gt3jqqudrlf.html

[T05] Kotlin：when 表达式
来源：http://www.ydjk.org.cn/Article/details/gt3dgvlmdtr.html

val s = when (x) { 1 -> "一" else -> "其他" }   // 多分支时每个分支单独一行
来源：http://www.ydjk.org.cn/Article/details/gt3xnnjdazv.html

[T06] Kotlin：集合映射
来源：http://www.52xcode.cn/Article/details/gt3vriwmrhn.html

listOf(1, 2, 3).map { it * 2 }
来源：http://www.52xcode.cn/Article/details/gt3orwilvzd.html

[T07] Kotlin：集合过滤
来源：http://www.ydjk.org.cn/Article/details/gt3iydcubki.html

listOf(1, 2, 3).filter { it > 1 }
来源：http://www.52xcode.cn/Article/details/gt3minenygj.html

[T08] Kotlin：数据类
来源：http://www.ydjk.org.cn/Article/details/gt3sqsjgezx.html

data class User(val name: String, val age: Int)
来源：http://www.ydjk.org.cn/Article/details/gt3yjxigahn.html

[T09] Kotlin：扩展函数
来源：http://www.ydjk.org.cn/Article/details/gt3zevpmszv.html

fun String.exclaim() = this + "!"
来源：http://www.52xcode.cn/Article/details/gt3dpwypdpu.html

[T10] Kotlin：默认参数
来源：http://www.ydjk.org.cn/Article/details/gt3vihhpldp.html

fun greet(name: String = "World") = "Hi $name"
来源：http://www.52xcode.cn/Article/details/gt3rvgfdswh.html

[T11] Kotlin：协程
来源：http://www.52xcode.cn/Article/details/gt3yogmpetg.html

GlobalScope.launch { delay(1000); println("done") }
来源：http://www.ydjk.org.cn/Article/details/gt3tfhmkjlh.html

[T12] Kotlin：解构声明
来源：http://www.52xcode.cn/Article/details/gt3nopkcuke.html

val (a, b) = Pair(1, 2)
来源：http://www.52xcode.cn/Article/details/gt3qvntogio.html

[T13] Kotlin：只读 Map
来源：http://www.52xcode.cn/Article/details/gt3xavzyeho.html

val m = mapOf("a" to 1)
来源：http://www.ydjk.org.cn/Article/details/gt3vfveyfzb.html

[T14] Kotlin：循环
来源：http://www.ydjk.org.cn/Article/details/gt3bjjdbpzc.html

for (i in 1..10) println(i)
来源：http://www.ydjk.org.cn/Article/details/gt3oanunfix.html

[T15] Kotlin：接口
来源：http://www.52xcode.cn/Article/details/gt3avxcwtve.html

interface Shape { fun area(): Double }
来源：http://www.ydjk.org.cn/Article/details/gt3kgppovek.html

[T16] Swift：Hello World
来源：http://www.52xcode.cn/Article/details/gt3nzedlgbf.html

print("Hello")
来源：http://www.ydjk.org.cn/Article/details/gt3dejigiic.html

[T17] Swift：变量与常量
来源：http://www.52xcode.cn/Article/details/gt3wmcinadh.html

var a = 1;  let b = 2
来源：http://www.52xcode.cn/Article/details/gt3vsfywklf.html

[T18] Swift：字符串插值
来源：http://www.ydjk.org.cn/Article/details/gt3yakfjghp.html

"值: \(b)"
来源：http://www.ydjk.org.cn/Article/details/gt3garqvhou.html

[T19] Swift：可选绑定
来源：http://www.ydjk.org.cn/Article/details/gt3pmrlfgaz.html

if let n = opt { print(n) }
来源：http://www.ydjk.org.cn/Article/details/gt3tptpgvke.html

[T20] Swift：数组操作
来源：http://www.52xcode.cn/Article/details/gt3akxdzwuq.html

var a = [1, 2, 3];  a.append(4)
来源：http://www.52xcode.cn/Article/details/gt3pjadllyy.html

[T21] Swift：遍历
来源：http://www.52xcode.cn/Article/details/gt3qcrhqrpu.html

for x in a { print(x) }
来源：http://www.52xcode.cn/Article/details/gt3ptjktoft.html

[T22] Swift：字典
来源：http://www.52xcode.cn/Article/details/gt3eoizotjn.html

var d = ["a": 1];  d["b"] = 2
来源：http://www.52xcode.cn/Article/details/gt3fmqmuymd.html

[T23] Swift：函数
来源：http://www.ydjk.org.cn/Article/details/gt3aaeptltk.html

func add(_ a: Int, _ b: Int) -> Int { a + b }
来源：http://www.52xcode.cn/Article/details/gt3rierrztu.html

[T24] Swift：闭包
来源：http://www.52xcode.cn/Article/details/gt3lviyqyjp.html

let f = { (x: Int) -> Int in x * 2 }
来源：http://www.ydjk.org.cn/Article/details/gt3hlvjpoqj.html

[T25] Swift：结构体
来源：http://www.52xcode.cn/Article/details/gt3wjgwnebo.html

struct P { var x: Int }
来源：http://www.52xcode.cn/Article/details/gt3abkzrweu.html

[T26] Swift：类与重写
来源：http://www.52xcode.cn/Article/details/gt3gqqvbsxh.html

class A: Base { override func f() {} }
来源：http://www.ydjk.org.cn/Article/details/gt3plyxcgyf.html

[T27] Swift：错误处理
来源：http://www.ydjk.org.cn/Article/details/gt3okvaqmrh.html

do { try f() } catch { print(error) }
来源：http://www.52xcode.cn/Article/details/gt3puklorrp.html

[T28] Swift：枚举
来源：http://www.ydjk.org.cn/Article/details/gt3ncqocsyl.html

enum Color { case red, green }
来源：http://www.ydjk.org.cn/Article/details/gt3tfrifdtu.html

[T29] Swift：guard 提前返回
来源：http://www.ydjk.org.cn/Article/details/gt3tegjthpf.html

guard let x = opt else { return }
来源：http://www.ydjk.org.cn/Article/details/gt3iyavysci.html

[T30] Swift：协议
来源：http://www.52xcode.cn/Article/details/gt3xxwokdxo.html

protocol Shape { func area() -> Double }
来源：http://www.52xcode.cn/Article/details/gt3orczetal.html

[T31] Lua：Hello World
来源：http://www.52xcode.cn/Article/details/gt3muuqvsbg.html

print("Hello")
来源：http://www.ydjk.org.cn/Article/details/gt3zjgvbqvx.html

[T32] Lua：局部变量
来源：http://www.ydjk.org.cn/Article/details/gt3iyfdavgw.html

local a = 1
来源：http://www.ydjk.org.cn/Article/details/gt3mtmcibyb.html

[T33] Lua：表（数组）
来源：http://www.52xcode.cn/Article/details/gt3vwyckkvr.html

local t = {1, 2, 3};  t[4] = 4
来源：http://www.ydjk.org.cn/Article/details/gt3wmltuynx.html

[T34] Lua：遍历表
来源：http://www.52xcode.cn/Article/details/gt3yomsqnjd.html

for i, v in ipairs(t) do print(i, v) end
来源：http://www.ydjk.org.cn/Article/details/gt3vqavtitt.html

[T35] Lua：字典表
来源：http://www.ydjk.org.cn/Article/details/gt3funcqhti.html

local d = { a = 1 };  d.b = 2
来源：http://www.ydjk.org.cn/Article/details/gt3llhrikgs.html

[T36] Lua：函数
来源：http://www.ydjk.org.cn/Article/details/gt3cnuavham.html

function add(a, b) return a + b end
来源：http://www.52xcode.cn/Article/details/gt3pjetmdyh.html

[T37] Lua：字符串拼接
来源：http://www.52xcode.cn/Article/details/gt3tvirzdbi.html

"a" .. "b"
来源：http://www.52xcode.cn/Article/details/gt3iofkxdcq.html

[T38] Lua：条件
来源：http://www.52xcode.cn/Article/details/gt3bqxeyojd.html

if x > 0 then print("正") end
来源：http://www.ydjk.org.cn/Article/details/gt3gnbdwqjq.html

[T39] Lua：模式匹配
来源：http://www.ydjk.org.cn/Article/details/gt3ouxdttkt.html

string.find(s, "%d+")
来源：http://www.ydjk.org.cn/Article/details/gt3pyzrgwwr.html

[T40] Lua：元表
来源：http://www.52xcode.cn/Article/details/gt3oolxdnnv.html

setmetatable({}, { __index = base })
来源：http://www.52xcode.cn/Article/details/gt3icxtssee.html

[T41] Perl：Hello World
来源：http://www.ydjk.org.cn/Article/details/gt3qixnczhu.html

print "Hello\n";
来源：http://www.52xcode.cn/Article/details/gt3xtgwmxtw.html

[T42] Perl：变量类型
来源：http://www.ydjk.org.cn/Article/details/gt3uvbgydtt.html

my $a = 1;  my @arr = (1, 2, 3);  my %h = (a => 1);
来源：http://www.52xcode.cn/Article/details/gt3dcjrjpja.html

[T43] Perl：字符串插值
来源：http://www.ydjk.org.cn/Article/details/gt3vksovxao.html

"值: $a"
来源：http://www.52xcode.cn/Article/details/gt3elbdafsg.html

[T44] Perl：条件
来源：http://www.52xcode.cn/Article/details/gt3zjtgdqjt.html

if ($a > 0) { print "正"; }
来源：http://www.ydjk.org.cn/Article/details/gt3zcbfxpxb.html

[T45] Perl：数组遍历
来源：http://www.52xcode.cn/Article/details/gt3iydhaaxq.html

for my $x (@arr) { print $x; }
来源：http://www.52xcode.cn/Article/details/gt3zqxxvakh.html

[T46] Perl：哈希操作
来源：http://www.ydjk.org.cn/Article/details/gt3ffdmpqct.html

$h{b} = 2;  for my $k (keys %h) { print "$k=$h{$k}"; }
来源：http://www.52xcode.cn/Article/details/gt3aclfltxs.html

[T47] Perl：正则捕获
来源：http://www.ydjk.org.cn/Article/details/gt3sxrkuenl.html

if ($s =~ /(\d+)/) { print $1; }
来源：http://www.52xcode.cn/Article/details/gt3gkabwjcm.html

[T48] Perl：正则替换
来源：http://www.52xcode.cn/Article/details/gt3vmvomijh.html

$s =~ s/old/new/g;
来源：http://www.52xcode.cn/Article/details/gt3ssdypezc.html

[T49] Perl：函数
来源：http://www.ydjk.org.cn/Article/details/gt3cdabrwnz.html

sub add { my ($a, $b) = @_; return $a + $b; }
来源：http://www.ydjk.org.cn/Article/details/gt3sryqasqn.html

[T50] Perl：逐行读文件
来源：http://www.ydjk.org.cn/Article/details/gt3vfbpzsju.html

open my $fh, "<", "a.txt" or die $!;
来源：http://www.52xcode.cn/Article/details/gt3iupauonp.html

while (my $line = <$fh>) { print $line; }
来源：http://www.ydjk.org.cn/Article/details/gt3wmnigmmn.html

[T51] Scala：Hello World
来源：http://www.52xcode.cn/Article/details/gt3omkkhpve.html

println("Hello")
来源：http://www.52xcode.cn/Article/details/gt3ujgmcrur.html

[T52] Scala：变量
来源：http://www.52xcode.cn/Article/details/gt3elolffgq.html

val a = 1;  var b = 2
来源：http://www.52xcode.cn/Article/details/gt3dmrksxha.html

[T53] Scala：字符串插值
来源：http://www.ydjk.org.cn/Article/details/gt3yvbqghng.html

s"值: $b"
来源：http://www.ydjk.org.cn/Article/details/gt3blqclrbp.html

[T54] Scala：集合映射
来源：http://www.52xcode.cn/Article/details/gt3dqpnnzmh.html

List(1, 2, 3).map(_ * 2)
来源：http://www.52xcode.cn/Article/details/gt3ekqexgtz.html

[T55] Scala：集合过滤
来源：http://www.52xcode.cn/Article/details/gt3helohnwd.html

List(1, 2, 3).filter(_ > 1)
来源：http://www.ydjk.org.cn/Article/details/gt3dzqvutmy.html

[T56] Scala：样例类
来源：http://www.52xcode.cn/Article/details/gt3azravtls.html

case class User(name: String, age: Int)
来源：http://www.52xcode.cn/Article/details/gt3ayehkwhf.html

[T57] Scala：模式匹配
来源：http://www.52xcode.cn/Article/details/gt3pqvwugbz.html

x match { case 1 => "一"; case _ => "其他" }
来源：http://www.ydjk.org.cn/Article/details/gt3avrutwrs.html

[T58] Scala：函数定义
来源：http://www.ydjk.org.cn/Article/details/gt3wlowtfud.html

def add(a: Int, b: Int): Int = a + b
来源：http://www.52xcode.cn/Article/details/gt3ycsgcpqc.html

[T59] Scala：循环
来源：http://www.52xcode.cn/Article/details/gt3fyemruwz.html

for (i <- 1 to 10) println(i)
来源：http://www.ydjk.org.cn/Article/details/gt3ewtqlhwf.html

[T60] Scala：折叠
来源：http://www.ydjk.org.cn/Article/details/gt3vtkqjuse.html

List(1, 2, 3).foldLeft(0)(_ + _)
来源：http://www.52xcode.cn/Article/details/gt3fphbubjg.html

================================================================================
来源：http://www.52xcode.cn/Article/details/gt3wvlfeojv.html

U. 高频实用片段（Python / PHP / JavaScript 各 40 条）
来源：http://www.52xcode.cn/Article/details/gt3hsnnxuel.html

================================================================================
来源：http://www.ydjk.org.cn/Article/details/gt3ayrmtvxq.html

[U01] Py：创建虚拟环境
来源：http://www.ydjk.org.cn/Article/details/gt3ujozqley.html

python -m venv .venv && source .venv/bin/activate
来源：http://www.ydjk.org.cn/Article/details/gt3fwojvedc.html

[U02] Py：导出 / 安装依赖
来源：http://www.ydjk.org.cn/Article/details/gt3katwskcc.html

pip freeze > requirements.txt;  pip install -r requirements.txt
来源：http://www.ydjk.org.cn/Article/details/gt3zgiyztsh.html

[U03] Py：加载 .env 配置
来源：http://www.52xcode.cn/Article/details/gt3ufoqfdha.html

from dotenv import load_dotenv; load_dotenv()
来源：http://www.52xcode.cn/Article/details/gt3buqaeknl.html

[U04] Py：变量调试打印
来源：http://www.52xcode.cn/Article/details/gt3tnmynmli.html

print(f"{x=}")            # 输出 x=值，Python 3.8+
来源：http://www.ydjk.org.cn/Article/details/gt3ebewefwk.html

[U05] Py：列表去重且保序
来源：http://www.52xcode.cn/Article/details/gt3bkbtbgob.html

list(dict.fromkeys(arr))
来源：http://www.52xcode.cn/Article/details/gt3pdynrcuy.html

[U06] Py：合并两个字典
来源：http://www.52xcode.cn/Article/details/gt3xkhrujpz.html

{**a, **b}
来源：http://www.ydjk.org.cn/Article/details/gt3isopgnft.html

[U07] Py：反转字典键值
来源：http://www.ydjk.org.cn/Article/details/gt3xblidqpa.html

{v: k for k, v in d.items()}
来源：http://www.52xcode.cn/Article/details/gt3rsuzqnyq.html

[U08] Py：展平二维列表
来源：http://www.ydjk.org.cn/Article/details/gt3zlhgemrm.html

[y for x in nested for y in x]
来源：http://www.ydjk.org.cn/Article/details/gt3bpaleqwf.html

[U09] Py：字典取最大值的键
来源：http://www.52xcode.cn/Article/details/gt3tuytigcz.html

max(d, key=d.get)
来源：http://www.52xcode.cn/Article/details/gt3jkhomdvl.html

[U10] Py：按值排序字典
来源：http://www.ydjk.org.cn/Article/details/gt3tdyixdaj.html

dict(sorted(d.items(), key=lambda kv: kv[1]))
来源：http://www.52xcode.cn/Article/details/gt3mkvvsaqj.html


<!-- 参考信息 -->