代发 wailian999

split -l 1000 big.log part_
来源：http://www.m.share.hesvh.cn/Article/details/gbsunwhuc.sHtML

[R74] 批量重命名
来源：http://mobile.zdbjq.cn/Article/details/gpzmkrpml.sHtML

for f in *.jpeg; do mv "$f" "${f%.jpeg}.jpg"; done
来源：http://m.share.hesvh.cn/Article/details/gxukoukos.sHtML

[R75] 导出环境变量
来源：http://wap.hesvh.cn/Article/details/grjpghqvs.sHtML

export PATH="$HOME/bin:$PATH"
来源：http://wap.hesvh.cn/Article/details/gnsxvsfqm.sHtML

[R76] 使用临时文件
来源：http://3g.hesvh.cn/Article/details/gjijezouh.sHtML

tmp=$(mktemp); trap 'rm -f "$tmp"' EXIT
来源：http://www.m.share.zdbjq.cn/Article/details/gvokshulb.sHtML

[R77] 读取用户输入
来源：http://wap.fehbvm.com/Article/details/gzjjrvpoe.sHtML

read -rp "请输入: " ans
来源：http://www.blog.zdbjq.cn/Article/details/giggsoqab.sHtML

[R78] 交互式菜单
来源：http://www.blog.zdbjq.cn/Article/details/ggopqaarj.sHtML

select opt in a b c; do echo "$opt"; break; done
来源：http://m.share.zdbjq.cn/Article/details/gqdbxwokp.sHtML

[R79] 解析命令行选项
来源：http://m.share.fehbvm.com/Article/details/ghgseotjk.sHtML

while getopts "v:f:" o; do case $o in v) V=$OPTARG ;; f) F=$OPTARG ;; esac; done
来源：http://read.share.zdbjq.cn/Article/details/gwapbybbx.sHtML

[R80] 查看脚本执行耗时
来源：http://blog.fehbvm.com/Article/details/gahamnsyw.sHtML

time ./run.sh
来源：http://blog.zdbjq.cn/Article/details/gezufvpsq.sHtML

================================================================================
来源：http://wap.fehbvm.com/Article/details/grhgjbayt.sHtML

S. C / C++ 专题
来源：http://mobile.fehbvm.com/Article/details/gqotuhspw.sHtML

================================================================================
来源：http://3g.hesvh.cn/Article/details/gpkeeqseg.sHtML

[S01] C：Hello World
来源：http://blog.fehbvm.com/Article/details/ggbvrnssw.sHtML

#include <stdio.h>
来源：http://www.share.hesvh.cn/Article/details/gytkfexot.sHtML

int main(void) { printf("Hello\n"); return 0; }
来源：http://m.share.hesvh.cn/Article/details/ghohiqwii.sHtML

[S02] C：变量与格式化输出
来源：http://www.blog.zdbjq.cn/Article/details/goqmjcrzn.sHtML

int a = 10; printf("%d\n", a);
来源：http://wap.fehbvm.com/Article/details/geivbdviv.sHtML

[S03] C：读入整数
来源：http://baike.hesvh.cn/Article/details/gorqnslhd.sHtML

int x; scanf("%d", &x);
来源：http://wap.hesvh.cn/Article/details/gfnxmiylv.sHtML

[S04] C：字符串复制
来源：http://baike.zdbjq.cn/Article/details/gzmmglrkj.sHtML

char dst[32]; strcpy(dst, "hi");
来源：http://www.blog.fehbvm.com/Article/details/gtrrbxcmx.sHtML

[S05] C：字符串长度
来源：http://www.share.fehbvm.com/Article/details/gozgwvcdu.sHtML

strlen(s)
来源：http://www.m.share.zdbjq.cn/Article/details/gnowrdhzz.sHtML

[S06] C：字符串比较
来源：http://m.share.zdbjq.cn/Article/details/gwmlyudak.sHtML

strcmp(a, b) == 0
来源：http://read.share.fehbvm.com/Article/details/gwjcixeqq.sHtML

[S07] C：数组遍历求和
来源：http://www.m.share.zdbjq.cn/Article/details/gyulxfxyj.sHtML

for (int i = 0; i < n; i++) sum += a[i];
来源：http://mobile.hesvh.cn/Article/details/gxleatime.sHtML

[S08] C：动态内存分配与释放
来源：http://read.share.fehbvm.com/Article/details/giftgzxld.sHtML

int *p = malloc(sizeof(int) * n); ... free(p);
来源：http://m.share.zdbjq.cn/Article/details/gfbcblakb.sHtML

[S09] C：结构体定义与初始化
来源：http://www.share.zdbjq.cn/Article/details/gfgdlsiam.sHtML

struct Point { int x, y; };  struct Point p = {1, 2};
来源：http://3g.zdbjq.cn/Article/details/gilfbqzaf.sHtML

[S10] C：指针与解引用
来源：http://3g.fehbvm.com/Article/details/gfwpavdny.sHtML

int *p = &a;  *p = 5;
来源：http://www.share.hesvh.cn/Article/details/gfepatyeb.sHtML

[S11] C：逐行读文件
来源：http://blog.zdbjq.cn/Article/details/gvhxvears.sHtML

FILE *f = fopen("a.txt", "r");
来源：http://3g.zdbjq.cn/Article/details/ggpiujxtr.sHtML

while (fgets(buf, sizeof buf, f)) { }
来源：http://www.share.zdbjq.cn/Article/details/ggwctsaok.sHtML

fclose(f);
来源：http://wap.hesvh.cn/Article/details/gyjhjkzjt.sHtML

[S12] C：写文件
来源：http://m.share.fehbvm.com/Article/details/gwdefwqyi.sHtML

FILE *f = fopen("a.txt", "w");  fprintf(f, "hi\n");  fclose(f);
来源：http://www.blog.zdbjq.cn/Article/details/gcgokcfnu.sHtML

[S13] C：宏定义
来源：http://mobile.zdbjq.cn/Article/details/gdmqnpzuf.sHtML

#define MAX(a, b) ((a) > (b) ? (a) : (b))
来源：http://read.share.hesvh.cn/Article/details/gshjhplll.sHtML

[S14] C：枚举
来源：http://baike.fehbvm.com/Article/details/gjumwyajo.sHtML

enum Color { RED, GREEN, BLUE };
来源：http://www.blog.zdbjq.cn/Article/details/gqtujolcq.sHtML

[S15] C：类型转换
来源：http://3g.zdbjq.cn/Article/details/gzqrnhbci.sHtML

(double) a / b
来源：http://baike.hesvh.cn/Article/details/gguoxjnkd.sHtML

[S16] C：位操作置位
来源：http://mobile.hesvh.cn/Article/details/gmtghqmvq.sHtML

x |= (1 << 3);
来源：http://m.share.fehbvm.com/Article/details/gczqknxcq.sHtML

[S17] C：安全拼接字符串
来源：http://blog.hesvh.cn/Article/details/ghunswsuk.sHtML

snprintf(buf, sizeof buf, "%s%s", a, b);
来源：http://wap.zdbjq.cn/Article/details/gfdywbyrp.sHtML

[S18] C：命令行参数
来源：http://www.blog.hesvh.cn/Article/details/gfstkpinb.sHtML

int main(int argc, char **argv)
来源：http://3g.hesvh.cn/Article/details/gffetansm.sHtML

[S19] C：快速排序
来源：http://3g.hesvh.cn/Article/details/ggcgbawlg.sHtML

qsort(a, n, sizeof(int), cmp);
来源：http://blog.hesvh.cn/Article/details/gyknmoiwb.sHtML

[S20] C：二分查找
来源：http://mobile.hesvh.cn/Article/details/gdvwvrlri.sHtML

bsearch(&key, a, n, sizeof(int), cmp);
来源：http://www.blog.hesvh.cn/Article/details/glngfewot.sHtML

[S21] C：字符类别判断
来源：http://www.blog.zdbjq.cn/Article/details/gvohruxoh.sHtML

isdigit(c);  isalpha(c);  isspace(c);
来源：http://blog.zdbjq.cn/Article/details/gnmsghaal.sHtML

[S22] C：字符串转数字
来源：http://read.share.hesvh.cn/Article/details/gmafmtxhh.sHtML

atoi("42");  strtod("3.14", NULL);
来源：http://baike.zdbjq.cn/Article/details/gkmbmyvhg.sHtML

[S23] C：随机数
来源：http://www.blog.hesvh.cn/Article/details/gcgvuqifa.sHtML

srand(time(NULL));  int r = rand() % 100;
来源：http://www.m.share.hesvh.cn/Article/details/gnwdaossk.sHtML

[S24] C：获取本地时间
来源：http://www.share.fehbvm.com/Article/details/gkusfmscq.sHtML

time_t t = time(NULL);  struct tm *tm = localtime(&t);
来源：http://m.share.hesvh.cn/Article/details/gifdqgpbt.sHtML

[S25] C：内存拷贝
来源：http://wap.fehbvm.com/Article/details/gesbqstvc.sHtML

memcpy(dst, src, n);
来源：http://mobile.fehbvm.com/Article/details/giibprpnz.sHtML

[S26] C：内存清零
来源：http://3g.hesvh.cn/Article/details/gxmlbqoxb.sHtML

memset(a, 0, sizeof a);
来源：http://www.share.hesvh.cn/Article/details/gpaecjqbp.sHtML

[S27] C：定义常量
来源：http://www.blog.hesvh.cn/Article/details/gyllfnjzp.sHtML

const double PI = 3.14159;
来源：http://baike.hesvh.cn/Article/details/gvyngqkus.sHtML

[S28] C：静态变量
来源：http://mobile.hesvh.cn/Article/details/guyzorcpc.sHtML

static int counter = 0;
来源：http://www.blog.fehbvm.com/Article/details/gpqfrzmje.sHtML

[S29] C：变参函数
来源：http://www.blog.hesvh.cn/Article/details/gxmmkixsk.sHtML

va_list ap; va_start(ap, fmt); vprintf(fmt, ap); va_end(ap);
来源：http://mobile.zdbjq.cn/Article/details/gxvyeguiy.sHtML

[S30] C：头文件保护
来源：http://www.share.fehbvm.com/Article/details/gjdhrvedu.sHtML

#ifndef X_H
来源：http://read.share.hesvh.cn/Article/details/gqdbmwkph.sHtML

#define X_H
来源：http://wap.zdbjq.cn/Article/details/ghevwhdid.sHtML

#endif
来源：http://read.share.zdbjq.cn/Article/details/gmkqkqjay.sHtML

[S31] C++：Hello World
来源：http://blog.fehbvm.com/Article/details/ggnycfebb.sHtML

#include <iostream>
来源：http://www.blog.fehbvm.com/Article/details/gzsnmkmxn.sHtML

int main() { std::cout << "Hello\n"; }
来源：http://www.blog.zdbjq.cn/Article/details/gnxyueaiu.sHtML

[S32] C++：字符串
来源：http://wap.fehbvm.com/Article/details/gifwcpiqr.sHtML

std::string s = "hi";  s += "!";
来源：http://www.blog.hesvh.cn/Article/details/gnvuzqkgi.sHtML

[S33] C++：vector 增删
来源：http://3g.fehbvm.com/Article/details/gkiaiyzdv.sHtML

std::vector<int> v{1, 2, 3};  v.push_back(4);
来源：http://read.share.zdbjq.cn/Article/details/gpuywuxsa.sHtML

[S34] C++：遍历 vector
来源：http://www.share.fehbvm.com/Article/details/gcowtytlh.sHtML

for (auto &x : v) { std::cout << x; }
来源：http://www.blog.hesvh.cn/Article/details/gmsvtumwk.sHtML

[S35] C++：map
来源：http://mobile.fehbvm.com/Article/details/ggufwvyav.sHtML

std::map<std::string, int> m;  m["a"] = 1;
来源：http://3g.fehbvm.com/Article/details/gnsxfouhx.sHtML

[S36] C++：unordered_map
来源：http://wap.fehbvm.com/Article/details/gxegxyujp.sHtML

std::unordered_map<std::string, int> m;  m["a"] = 1;
来源：http://www.share.hesvh.cn/Article/details/gaeoozfrx.sHtML

[S37] C++：set
来源：http://wap.fehbvm.com/Article/details/gewsabxjk.sHtML

std::set<int> s{1, 2, 3};  s.insert(4);
来源：http://m.share.hesvh.cn/Article/details/gzajepboj.sHtML

[S38] C++：排序
来源：http://baike.fehbvm.com/Article/details/gahvpqxyc.sHtML

std::sort(v.begin(), v.end());
来源：http://www.m.share.hesvh.cn/Article/details/gfqygvfqs.sHtML

[S39] C++：自定义比较器排序
来源：http://www.m.share.hesvh.cn/Article/details/gqltkcfcx.sHtML

std::sort(v.begin(), v.end(), [](int a, int b) { return a > b; });
来源：http://wap.fehbvm.com/Article/details/gqaubuawa.sHtML

[S40] C++：查找元素
来源：http://m.share.zdbjq.cn/Article/details/gcqxdflvn.sHtML

auto it = std::find(v.begin(), v.end(), 3);
来源：http://m.share.hesvh.cn/Article/details/glmzgyztv.sHtML

[S41] C++：类与构造函数
来源：http://www.m.share.zdbjq.cn/Article/details/gcjbqyedt.sHtML

class A { public: A(int v) : x_(v) {} int get() const { return x_; } private: int x_; };
来源：http://wap.zdbjq.cn/Article/details/gyuyuhjiy.sHtML

[S42] C++：继承与虚函数
来源：http://wap.hesvh.cn/Article/details/gotvnmtiz.sHtML

class B : public Base { public: void f() override {} };
来源：http://baike.hesvh.cn/Article/details/gnazljkhv.sHtML

[S43] C++：智能指针
来源：http://wap.hesvh.cn/Article/details/ghwvnzwci.sHtML

auto p = std::make_unique<int>(5);
来源：http://www.blog.fehbvm.com/Article/details/grhbezjoe.sHtML

[S44] C++：引用传参
来源：http://www.share.zdbjq.cn/Article/details/giwvehzcy.sHtML

void inc(int &x) { ++x; }
来源：http://baike.zdbjq.cn/Article/details/gtxmfzkjd.sHtML

[S45] C++：lambda
来源：http://3g.hesvh.cn/Article/details/grfbdpicm.sHtML

auto add = [](int a, int b) { return a + b; };
来源：http://baike.hesvh.cn/Article/details/gzasfwgdy.sHtML

[S46] C++：函数模板
来源：http://blog.zdbjq.cn/Article/details/gzdffbcmb.sHtML

template <typename T> T maxv(T a, T b) { return a > b ? a : b; }
来源：http://mobile.fehbvm.com/Article/details/gzsyelvve.sHtML

[S47] C++：结构化绑定遍历
来源：http://mobile.fehbvm.com/Article/details/gbcsqaqrz.sHtML

for (const auto &[k, v] : m) { std::cout << k << v; }
来源：http://www.share.zdbjq.cn/Article/details/goeiujqoi.sHtML

[S48] C++：逐行读文件
来源：http://www.blog.zdbjq.cn/Article/details/gvpibcihm.sHtML

std::ifstream in("a.txt");  std::string line;
来源：http://www.blog.zdbjq.cn/Article/details/ghbatddva.sHtML

while (std::getline(in, line)) { }
来源：http://mobile.zdbjq.cn/Article/details/gjwqdewsj.sHtML

[S49] C++：写文件
来源：http://www.share.hesvh.cn/Article/details/grxkjajgy.sHtML

std::ofstream out("a.txt");  out << "hi\n";
来源：http://read.share.zdbjq.cn/Article/details/gnngrtbjf.sHtML

[S50] C++：格式化数字
来源：http://mobile.fehbvm.com/Article/details/glhpfsoey.sHtML

std::ostringstream os;  os << std::fixed << std::setprecision(2) << 3.14159;
来源：http://www.m.share.fehbvm.com/Article/details/gictwddta.sHtML

[S51] C++：显式类型转换
来源：http://baike.fehbvm.com/Article/details/gshxzotnc.sHtML

static_cast<double>(a) / b
来源：http://wap.zdbjq.cn/Article/details/gnwwpnihx.sHtML

[S52] C++：const 与 noexcept
来源：http://www.blog.fehbvm.com/Article/details/glfjbgvcn.sHtML

int size() const noexcept { return n_; }
来源：http://baike.fehbvm.com/Article/details/gabhdxaci.sHtML

[S53] C++：移动语义
来源：http://mobile.zdbjq.cn/Article/details/gdngwfssq.sHtML

std::vector<int> w = std::move(v);
来源：http://www.blog.hesvh.cn/Article/details/gqqwqohaa.sHtML

[S54] C++：异常处理
来源：http://read.share.hesvh.cn/Article/details/gbkspdumd.sHtML

try { throw std::runtime_error("x"); } catch (const std::exception &e) { }
来源：http://baike.hesvh.cn/Article/details/goqzivdhw.sHtML

[S55] C++：结构化绑定
来源：http://www.m.share.hesvh.cn/Article/details/gfjyiiucl.sHtML

auto [a, b] = std::make_pair(1, 2);
来源：http://m.share.hesvh.cn/Article/details/goctrbtry.sHtML

[S56] C++：optional
来源：http://blog.fehbvm.com/Article/details/gvhkdlkgd.sHtML

std::optional<int> o = 5;  if (o) { int v = *o; }
来源：http://read.share.fehbvm.com/Article/details/ghjcrhlwu.sHtML

[S57] C++：编译期常量
来源：http://www.share.hesvh.cn/Article/details/gimtphoyg.sHtML

constexpr int N = 10;
来源：http://baike.zdbjq.cn/Article/details/gewvankec.sHtML

[S58] C++：命名空间
来源：http://www.share.zdbjq.cn/Article/details/gtzccfaen.sHtML

namespace ns { int f() { return 1; } }
来源：http://baike.fehbvm.com/Article/details/gxqqpgjbg.sHtML

[S59] C++：静态断言
来源：http://m.share.fehbvm.com/Article/details/gvpckrwpx.sHtML

static_assert(sizeof(int) == 4, "int 必须 4 字节");
来源：http://www.m.share.hesvh.cn/Article/details/gzppdduwb.sHtML

[S60] C++：遍历并删除元素
来源：http://mobile.fehbvm.com/Article/details/geuktatrx.sHtML

v.erase(std::remove_if(v.begin(), v.end(), [](int x) { return x < 0; }), v.end());
来源：http://mobile.fehbvm.com/Article/details/gzrnverjq.sHtML

================================================================================
来源：http://read.share.fehbvm.com/Article/details/grjfqrvmm.sHtML

T. 其他语言补充（Kotlin / Swift / Lua / Perl / Scala）
来源：http://www.share.zdbjq.cn/Article/details/gbadncwuz.sHtML

================================================================================
来源：http://www.share.zdbjq.cn/Article/details/gmutggtee.sHtML

[T01] Kotlin：Hello World
来源：http://blog.zdbjq.cn/Article/details/glqawhliu.sHtML

println("Hello")
来源：http://m.share.zdbjq.cn/Article/details/gsxygnwrc.sHtML

[T02] Kotlin：变量
来源：http://read.share.fehbvm.com/Article/details/gragatliw.sHtML

val a = 1;  var b = 2        // val 只读，var 可变
来源：http://www.share.zdbjq.cn/Article/details/glmrtqtuz.sHtML

[T03] Kotlin：字符串模板
来源：http://www.m.share.hesvh.cn/Article/details/grozoyzyl.sHtML

"值: $b"
来源：http://blog.fehbvm.com/Article/details/glwyekncd.sHtML

[T04] Kotlin：空安全
来源：http://m.share.zdbjq.cn/Article/details/gjqukcgtw.sHtML

val n: String? = null;  n?.length
来源：http://read.share.zdbjq.cn/Article/details/gmzrkqahl.sHtML

[T05] Kotlin：when 表达式
来源：http://3g.zdbjq.cn/Article/details/gdlrmkxpx.sHtML

val s = when (x) { 1 -> "一" else -> "其他" }   // 多分支时每个分支单独一行
来源：http://3g.hesvh.cn/Article/details/gjzkzwlfs.sHtML

[T06] Kotlin：集合映射
来源：http://www.share.zdbjq.cn/Article/details/gigkceatk.sHtML

listOf(1, 2, 3).map { it * 2 }
来源：http://www.m.share.fehbvm.com/Article/details/gthwjmfkn.sHtML

[T07] Kotlin：集合过滤
来源：http://m.share.zdbjq.cn/Article/details/grghkakof.sHtML

listOf(1, 2, 3).filter { it > 1 }
来源：http://www.m.share.zdbjq.cn/Article/details/glswkxukk.sHtML

[T08] Kotlin：数据类
来源：http://mobile.fehbvm.com/Article/details/giqzoihbd.sHtML

data class User(val name: String, val age: Int)
来源：http://m.share.zdbjq.cn/Article/details/gxibnqvlt.sHtML

[T09] Kotlin：扩展函数
来源：http://3g.hesvh.cn/Article/details/gzaligzgd.sHtML

fun String.exclaim() = this + "!"
来源：http://m.share.hesvh.cn/Article/details/glgdmpyds.sHtML

[T10] Kotlin：默认参数
来源：http://m.share.fehbvm.com/Article/details/glezsvkny.sHtML

fun greet(name: String = "World") = "Hi $name"
来源：http://www.blog.hesvh.cn/Article/details/ggqowqesl.sHtML

[T11] Kotlin：协程
来源：http://mobile.zdbjq.cn/Article/details/gflnujrod.sHtML

GlobalScope.launch { delay(1000); println("done") }
来源：http://mobile.zdbjq.cn/Article/details/grlloovmh.sHtML

[T12] Kotlin：解构声明
来源：http://mobile.zdbjq.cn/Article/details/glfmgkjkb.sHtML

val (a, b) = Pair(1, 2)
来源：http://blog.hesvh.cn/Article/details/gyfcexlze.sHtML

[T13] Kotlin：只读 Map
来源：http://baike.fehbvm.com/Article/details/gysnahmqz.sHtML

val m = mapOf("a" to 1)
来源：http://read.share.hesvh.cn/Article/details/gpfepllhf.sHtML

[T14] Kotlin：循环
来源：http://read.share.zdbjq.cn/Article/details/gsbdttqph.sHtML

for (i in 1..10) println(i)
来源：http://mobile.zdbjq.cn/Article/details/gsjyrczte.sHtML

[T15] Kotlin：接口
来源：http://www.share.zdbjq.cn/Article/details/glnzcqpvx.sHtML

interface Shape { fun area(): Double }
来源：http://wap.zdbjq.cn/Article/details/gqnbsuaww.sHtML

[T16] Swift：Hello World
来源：http://www.blog.fehbvm.com/Article/details/gkfamdgbr.sHtML

print("Hello")
来源：http://www.blog.fehbvm.com/Article/details/gnajztalk.sHtML

[T17] Swift：变量与常量
来源：http://www.blog.fehbvm.com/Article/details/gxqlhxsro.sHtML

var a = 1;  let b = 2
来源：http://3g.zdbjq.cn/Article/details/gvmzbzzkp.sHtML

[T18] Swift：字符串插值
来源：http://baike.hesvh.cn/Article/details/ghhmmyfgh.sHtML

"值: \(b)"
来源：http://www.share.fehbvm.com/Article/details/gxldielhq.sHtML

[T19] Swift：可选绑定
来源：http://wap.fehbvm.com/Article/details/gvebcqlhe.sHtML

if let n = opt { print(n) }
来源：http://wap.hesvh.cn/Article/details/giqmkhati.sHtML

[T20] Swift：数组操作
来源：http://www.share.hesvh.cn/Article/details/gwvsczpjl.sHtML

var a = [1, 2, 3];  a.append(4)
来源：http://3g.fehbvm.com/Article/details/glpmjmmjy.sHtML

[T21] Swift：遍历
来源：http://read.share.hesvh.cn/Article/details/gwlbyvxnh.sHtML

for x in a { print(x) }
来源：http://www.m.share.fehbvm.com/Article/details/gchuiinws.sHtML

[T22] Swift：字典
来源：http://3g.hesvh.cn/Article/details/gdxghbkdy.sHtML

var d = ["a": 1];  d["b"] = 2
来源：http://baike.zdbjq.cn/Article/details/gqaswrvgk.sHtML

[T23] Swift：函数
来源：http://blog.fehbvm.com/Article/details/gqeenpspi.sHtML

func add(_ a: Int, _ b: Int) -> Int { a + b }
来源：http://mobile.hesvh.cn/Article/details/gnsbphydc.sHtML

[T24] Swift：闭包
来源：http://www.blog.hesvh.cn/Article/details/gupugulsm.sHtML

let f = { (x: Int) -> Int in x * 2 }
来源：http://www.share.zdbjq.cn/Article/details/ghsugbipr.sHtML

[T25] Swift：结构体
来源：http://wap.hesvh.cn/Article/details/gnujexega.sHtML

struct P { var x: Int }
来源：http://read.share.fehbvm.com/Article/details/gjvylubyy.sHtML

[T26] Swift：类与重写
来源：http://read.share.fehbvm.com/Article/details/ggbcrpcah.sHtML

class A: Base { override func f() {} }
来源：http://wap.zdbjq.cn/Article/details/gpzfxlnja.sHtML

[T27] Swift：错误处理
来源：http://baike.fehbvm.com/Article/details/giwtazqud.sHtML

do { try f() } catch { print(error) }
来源：http://read.share.zdbjq.cn/Article/details/gdhnvbobz.sHtML

[T28] Swift：枚举
来源：http://blog.hesvh.cn/Article/details/gtwrwsxok.sHtML

enum Color { case red, green }
来源：http://www.blog.fehbvm.com/Article/details/glvjfcnps.sHtML

[T29] Swift：guard 提前返回
来源：http://baike.zdbjq.cn/Article/details/gwqzptbby.sHtML

guard let x = opt else { return }
来源：http://mobile.fehbvm.com/Article/details/gsbxenblw.sHtML

[T30] Swift：协议
来源：http://www.blog.fehbvm.com/Article/details/gtpkziyyj.sHtML

protocol Shape { func area() -> Double }
来源：http://wap.zdbjq.cn/Article/details/gprfwqsoq.sHtML

[T31] Lua：Hello World
来源：http://wap.fehbvm.com/Article/details/gszqzpemc.sHtML

print("Hello")
来源：http://blog.zdbjq.cn/Article/details/gkjhxhzso.sHtML

[T32] Lua：局部变量
来源：http://blog.hesvh.cn/Article/details/gktqjznpw.sHtML

local a = 1
来源：http://www.blog.hesvh.cn/Article/details/gcixovoao.sHtML

[T33] Lua：表（数组）
来源：http://read.share.hesvh.cn/Article/details/gjpggcxet.sHtML

local t = {1, 2, 3};  t[4] = 4
来源：http://www.blog.zdbjq.cn/Article/details/giumnodjc.sHtML

[T34] Lua：遍历表
来源：http://www.m.share.zdbjq.cn/Article/details/gepwdqchf.sHtML

for i, v in ipairs(t) do print(i, v) end
来源：http://mobile.fehbvm.com/Article/details/gdnbbeprn.sHtML

[T35] Lua：字典表
来源：http://3g.fehbvm.com/Article/details/gbvkxrqie.sHtML

local d = { a = 1 };  d.b = 2
来源：http://3g.zdbjq.cn/Article/details/ggxcgcnja.sHtML

[T36] Lua：函数
来源：http://wap.fehbvm.com/Article/details/gfrazyhys.sHtML

function add(a, b) return a + b end
来源：http://mobile.hesvh.cn/Article/details/glyeqcuyc.sHtML

[T37] Lua：字符串拼接
来源：http://m.share.hesvh.cn/Article/details/gaexzvdyg.sHtML

"a" .. "b"
来源：http://www.share.hesvh.cn/Article/details/guomfmrns.sHtML

[T38] Lua：条件
来源：http://baike.zdbjq.cn/Article/details/gnwlinpbc.sHtML

if x > 0 then print("正") end
来源：http://m.share.zdbjq.cn/Article/details/gytqotofz.sHtML

[T39] Lua：模式匹配
来源：http://blog.fehbvm.com/Article/details/gykpwbftq.sHtML

string.find(s, "%d+")
来源：http://blog.fehbvm.com/Article/details/gemkslwac.sHtML

[T40] Lua：元表
来源：http://read.share.zdbjq.cn/Article/details/gyrnlxfmi.sHtML

setmetatable({}, { __index = base })
来源：http://baike.zdbjq.cn/Article/details/gfpluzbzu.sHtML

[T41] Perl：Hello World
来源：http://www.m.share.zdbjq.cn/Article/details/gtfewbybh.sHtML

print "Hello\n";
来源：http://read.share.zdbjq.cn/Article/details/gunaihpif.sHtML

[T42] Perl：变量类型
来源：http://baike.fehbvm.com/Article/details/gwhnfgbxd.sHtML

my $a = 1;  my @arr = (1, 2, 3);  my %h = (a => 1);
来源：http://www.m.share.zdbjq.cn/Article/details/gjbrnszpw.sHtML

[T43] Perl：字符串插值
来源：http://www.m.share.hesvh.cn/Article/details/gujlehbkn.sHtML

"值: $a"
来源：http://www.m.share.zdbjq.cn/Article/details/gfqcxxprk.sHtML

[T44] Perl：条件
来源：http://blog.zdbjq.cn/Article/details/gwhzvbfzg.sHtML

if ($a > 0) { print "正"; }
来源：http://mobile.zdbjq.cn/Article/details/grctccftn.sHtML

[T45] Perl：数组遍历
来源：http://baike.fehbvm.com/Article/details/ghinxsprb.sHtML

for my $x (@arr) { print $x; }
来源：http://mobile.hesvh.cn/Article/details/gintpunzl.sHtML

[T46] Perl：哈希操作
来源：http://baike.hesvh.cn/Article/details/gryotzpbk.sHtML

$h{b} = 2;  for my $k (keys %h) { print "$k=$h{$k}"; }
来源：http://read.share.fehbvm.com/Article/details/grqnoqroh.sHtML

[T47] Perl：正则捕获
来源：http://www.blog.fehbvm.com/Article/details/gjrzgmrws.sHtML

if ($s =~ /(\d+)/) { print $1; }
来源：http://m.share.zdbjq.cn/Article/details/gdrxzwoeb.sHtML

[T48] Perl：正则替换
来源：http://mobile.fehbvm.com/Article/details/gvfqjqmss.sHtML

$s =~ s/old/new/g;
来源：http://m.share.fehbvm.com/Article/details/gdvzemfpe.sHtML

[T49] Perl：函数
来源：http://www.share.fehbvm.com/Article/details/gptvgnmjz.sHtML

sub add { my ($a, $b) = @_; return $a + $b; }
来源：http://mobile.fehbvm.com/Article/details/gwuiemebn.sHtML

[T50] Perl：逐行读文件
来源：http://www.m.share.zdbjq.cn/Article/details/gsfhossrq.sHtML

open my $fh, "<", "a.txt" or die $!;
来源：http://3g.fehbvm.com/Article/details/gmvpcvuan.sHtML

while (my $line = <$fh>) { print $line; }
来源：http://www.blog.hesvh.cn/Article/details/gtncnymin.sHtML

[T51] Scala：Hello World
来源：http://www.m.share.hesvh.cn/Article/details/gwxszzdab.sHtML

println("Hello")
来源：http://www.blog.zdbjq.cn/Article/details/gcrjzzahd.sHtML

[T52] Scala：变量
来源：http://www.share.fehbvm.com/Article/details/gnihskosf.sHtML

val a = 1;  var b = 2
来源：http://www.m.share.zdbjq.cn/Article/details/grcjbtntt.sHtML

[T53] Scala：字符串插值
来源：http://read.share.zdbjq.cn/Article/details/gzukvrpkj.sHtML

s"值: $b"
来源：http://mobile.fehbvm.com/Article/details/gsfqfvvgf.sHtML

[T54] Scala：集合映射
来源：http://www.blog.zdbjq.cn/Article/details/gtyuwagzt.sHtML

List(1, 2, 3).map(_ * 2)
来源：http://mobile.hesvh.cn/Article/details/gxizfzzdo.sHtML

[T55] Scala：集合过滤
来源：http://www.m.share.fehbvm.com/Article/details/giocsehwm.sHtML

List(1, 2, 3).filter(_ > 1)
来源：http://blog.fehbvm.com/Article/details/gdrliobdg.sHtML

[T56] Scala：样例类
来源：http://mobile.hesvh.cn/Article/details/ggqwndnad.sHtML

case class User(name: String, age: Int)
来源：http://mobile.zdbjq.cn/Article/details/gobwbucvj.sHtML

[T57] Scala：模式匹配
来源：http://3g.fehbvm.com/Article/details/gtolqjffr.sHtML

x match { case 1 => "一"; case _ => "其他" }
来源：http://3g.fehbvm.com/Article/details/gyitbijqo.sHtML

[T58] Scala：函数定义
来源：http://www.share.zdbjq.cn/Article/details/gnprrltql.sHtML

def add(a: Int, b: Int): Int = a + b
来源：http://www.blog.hesvh.cn/Article/details/gzkxwvpwj.sHtML

[T59] Scala：循环
来源：http://3g.zdbjq.cn/Article/details/ghywwnyrh.sHtML

for (i <- 1 to 10) println(i)
来源：http://baike.hesvh.cn/Article/details/gqgdvknoe.sHtML

[T60] Scala：折叠
来源：http://baike.hesvh.cn/Article/details/gdfhrphnv.sHtML

List(1, 2, 3).foldLeft(0)(_ + _)
来源：http://www.blog.hesvh.cn/Article/details/gewejvuzq.sHtML

================================================================================
来源：http://www.m.share.hesvh.cn/Article/details/gqsggdkaq.sHtML

U. 高频实用片段（Python / PHP / JavaScript 各 40 条）
来源：http://blog.zdbjq.cn/Article/details/ggqkgdcqu.sHtML

================================================================================
来源：http://baike.hesvh.cn/Article/details/gpjwticdt.sHtML

[U01] Py：创建虚拟环境
来源：http://wap.hesvh.cn/Article/details/gctuejmmb.sHtML

python -m venv .venv && source .venv/bin/activate
来源：http://www.share.fehbvm.com/Article/details/gsknvtbdh.sHtML

[U02] Py：导出 / 安装依赖
来源：http://baike.zdbjq.cn/Article/details/gsrrdlrrf.sHtML

pip freeze > requirements.txt;  pip install -r requirements.txt
来源：http://www.share.zdbjq.cn/Article/details/gavjdtfrg.sHtML

[U03] Py：加载 .env 配置
来源：http://www.share.fehbvm.com/Article/details/glxkdsdvw.sHtML

from dotenv import load_dotenv; load_dotenv()
来源：http://blog.fehbvm.com/Article/details/gfarntsak.sHtML

[U04] Py：变量调试打印
来源：http://www.m.share.fehbvm.com/Article/details/gnoenboms.sHtML

print(f"{x=}")            # 输出 x=值，Python 3.8+
来源：http://www.blog.hesvh.cn/Article/details/gclitczvj.sHtML

[U05] Py：列表去重且保序
来源：http://3g.zdbjq.cn/Article/details/gxbeyuvwf.sHtML

list(dict.fromkeys(arr))
来源：http://m.share.hesvh.cn/Article/details/grenfnwoz.sHtML

[U06] Py：合并两个字典
来源：http://read.share.hesvh.cn/Article/details/gsmjcjfqx.sHtML

{**a, **b}
来源：http://mobile.zdbjq.cn/Article/details/gfstinlzg.sHtML

[U07] Py：反转字典键值
来源：http://www.blog.zdbjq.cn/Article/details/guxpyhmbf.sHtML

{v: k for k, v in d.items()}
来源：http://baike.hesvh.cn/Article/details/gmqytspwl.sHtML

[U08] Py：展平二维列表
来源：http://www.blog.zdbjq.cn/Article/details/gifqmrolb.sHtML

[y for x in nested for y in x]
来源：http://3g.zdbjq.cn/Article/details/gjttzqjof.sHtML

[U09] Py：字典取最大值的键
来源：http://3g.zdbjq.cn/Article/details/ggvhnznzv.sHtML

max(d, key=d.get)
来源：http://www.blog.zdbjq.cn/Article/details/gaqxftbeu.sHtML

[U10] Py：按值排序字典
来源：http://3g.zdbjq.cn/Article/details/gwebfcbkz.sHtML

dict(sorted(d.items(), key=lambda kv: kv[1]))
来源：http://m.share.hesvh.cn/Article/details/ghshslfdc.sHtML

[U11] Py：生成器表达式
来源：http://blog.zdbjq.cn/Article/details/gqzrgvvkf.sHtML

(x * 2 for x in arr)
来源：http://mobile.zdbjq.cn/Article/details/ghlbtkwoz.sHtML

[U12] Py：取出现最多的 3 个元素
来源：http://baike.zdbjq.cn/Article/details/ggzkfuveo.sHtML

Counter(arr).most_common(3)
来源：http://baike.zdbjq.cn/Article/details/gqjhlgojg.sHtML

[U13] Py：固定长度队列
来源：http://blog.zdbjq.cn/Article/details/gevwgwpts.sHtML

deque(maxlen=10)
来源：http://www.m.share.zdbjq.cn/Article/details/gsfyelmiy.sHtML

[U14] Py：分组收集到列表
来源：http://www.blog.fehbvm.com/Article/details/gnynytnoz.sHtML

defaultdict(list)
来源：http://blog.hesvh.cn/Article/details/geqtxjxou.sHtML


<!-- 参考信息 -->