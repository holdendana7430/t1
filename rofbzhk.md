代发 wailian999

head -c 16 /dev/urandom | base64
来源：http://www.share.hesvh.cn/Article/details/gcttqefik.sHtML

[R70] 时间戳与互转
来源：http://wap.fehbvm.com/Article/details/gavhdmoyo.sHtML

date +%s;  date -d @1700000000
来源：http://www.share.fehbvm.com/Article/details/gjcpepada.sHtML

[R71] 日期格式化
来源：http://3g.hesvh.cn/Article/details/giofjwtju.sHtML

date +"%Y-%m-%d %H:%M:%S"
来源：http://blog.fehbvm.com/Article/details/gsuibvrmw.sHtML

[R72] 等待端口就绪
来源：http://3g.zdbjq.cn/Article/details/gjrfvkupy.sHtML

until nc -z localhost 3306; do sleep 1; done
来源：http://wap.fehbvm.com/Article/details/gdsuwbtdj.sHtML

[R73] 分割大日志
来源：http://blog.fehbvm.com/Article/details/guymrksbu.sHtML

split -l 1000 big.log part_
来源：http://www.blog.zdbjq.cn/Article/details/gsktoszlh.sHtML

[R74] 批量重命名
来源：http://3g.fehbvm.com/Article/details/goaloqjqv.sHtML

for f in *.jpeg; do mv "$f" "${f%.jpeg}.jpg"; done
来源：http://read.share.fehbvm.com/Article/details/gwphmnjsv.sHtML

[R75] 导出环境变量
来源：http://read.share.hesvh.cn/Article/details/guginoscw.sHtML

export PATH="$HOME/bin:$PATH"
来源：http://baike.zdbjq.cn/Article/details/getdeqqht.sHtML

[R76] 使用临时文件
来源：http://m.share.zdbjq.cn/Article/details/gzpveqtea.sHtML

tmp=$(mktemp); trap 'rm -f "$tmp"' EXIT
来源：http://mobile.hesvh.cn/Article/details/gskmgigyg.sHtML

[R77] 读取用户输入
来源：http://www.share.fehbvm.com/Article/details/gjxemafuq.sHtML

read -rp "请输入: " ans
来源：http://read.share.zdbjq.cn/Article/details/gdqxqkwsl.sHtML

[R78] 交互式菜单
来源：http://www.blog.hesvh.cn/Article/details/ggqorqaen.sHtML

select opt in a b c; do echo "$opt"; break; done
来源：http://m.share.fehbvm.com/Article/details/gqzjeqzbb.sHtML

[R79] 解析命令行选项
来源：http://m.share.zdbjq.cn/Article/details/geldyqthd.sHtML

while getopts "v:f:" o; do case $o in v) V=$OPTARG ;; f) F=$OPTARG ;; esac; done
来源：http://3g.hesvh.cn/Article/details/gnekjnxya.sHtML

[R80] 查看脚本执行耗时
来源：http://read.share.fehbvm.com/Article/details/gjudrpdyt.sHtML

time ./run.sh
来源：http://blog.hesvh.cn/Article/details/ganzbiiar.sHtML

================================================================================
来源：http://wap.zdbjq.cn/Article/details/gnrhqwjph.sHtML

S. C / C++ 专题
来源：http://baike.hesvh.cn/Article/details/gyttpwrjb.sHtML

================================================================================
来源：http://m.share.fehbvm.com/Article/details/gwvhizwop.sHtML

[S01] C：Hello World
来源：http://read.share.zdbjq.cn/Article/details/gqskqoqtw.sHtML

#include <stdio.h>
来源：http://3g.hesvh.cn/Article/details/gnvuzujij.sHtML

int main(void) { printf("Hello\n"); return 0; }
来源：http://m.share.fehbvm.com/Article/details/gvrxsatkh.sHtML

[S02] C：变量与格式化输出
来源：http://blog.zdbjq.cn/Article/details/gwcfusdxa.sHtML

int a = 10; printf("%d\n", a);
来源：http://3g.hesvh.cn/Article/details/gnjwspmgn.sHtML

[S03] C：读入整数
来源：http://read.share.zdbjq.cn/Article/details/gktqiujxv.sHtML

int x; scanf("%d", &x);
来源：http://www.blog.fehbvm.com/Article/details/gvxhkpydn.sHtML

[S04] C：字符串复制
来源：http://www.blog.zdbjq.cn/Article/details/gwfsmlrag.sHtML

char dst[32]; strcpy(dst, "hi");
来源：http://wap.zdbjq.cn/Article/details/gdcxzyqpt.sHtML

[S05] C：字符串长度
来源：http://wap.fehbvm.com/Article/details/gqxmgdveb.sHtML

strlen(s)
来源：http://wap.zdbjq.cn/Article/details/gdzrpewib.sHtML

[S06] C：字符串比较
来源：http://3g.fehbvm.com/Article/details/gywychyie.sHtML

strcmp(a, b) == 0
来源：http://wap.zdbjq.cn/Article/details/gdigowtse.sHtML

[S07] C：数组遍历求和
来源：http://baike.fehbvm.com/Article/details/gmhgjhqoz.sHtML

for (int i = 0; i < n; i++) sum += a[i];
来源：http://mobile.fehbvm.com/Article/details/ghyqdnyux.sHtML

[S08] C：动态内存分配与释放
来源：http://read.share.fehbvm.com/Article/details/glgajnasr.sHtML

int *p = malloc(sizeof(int) * n); ... free(p);
来源：http://m.share.zdbjq.cn/Article/details/gjjowmliv.sHtML

[S09] C：结构体定义与初始化
来源：http://wap.zdbjq.cn/Article/details/gqjqykzfx.sHtML

struct Point { int x, y; };  struct Point p = {1, 2};
来源：http://read.share.hesvh.cn/Article/details/gmscckgji.sHtML

[S10] C：指针与解引用
来源：http://www.share.zdbjq.cn/Article/details/gsowzygoo.sHtML

int *p = &a;  *p = 5;
来源：http://www.blog.fehbvm.com/Article/details/gtwroyuyq.sHtML

[S11] C：逐行读文件
来源：http://blog.fehbvm.com/Article/details/gcsrfpbzq.sHtML

FILE *f = fopen("a.txt", "r");
来源：http://read.share.hesvh.cn/Article/details/grxddqbua.sHtML

while (fgets(buf, sizeof buf, f)) { }
来源：http://www.blog.zdbjq.cn/Article/details/gsnthyohv.sHtML

fclose(f);
来源：http://wap.fehbvm.com/Article/details/gmddtmefe.sHtML

[S12] C：写文件
来源：http://wap.hesvh.cn/Article/details/grptalrmx.sHtML

FILE *f = fopen("a.txt", "w");  fprintf(f, "hi\n");  fclose(f);
来源：http://blog.hesvh.cn/Article/details/gjhymoqux.sHtML

[S13] C：宏定义
来源：http://www.share.fehbvm.com/Article/details/gmpdtqdoh.sHtML

#define MAX(a, b) ((a) > (b) ? (a) : (b))
来源：http://wap.hesvh.cn/Article/details/gseauytjq.sHtML

[S14] C：枚举
来源：http://www.share.hesvh.cn/Article/details/gzyhllpvp.sHtML

enum Color { RED, GREEN, BLUE };
来源：http://baike.fehbvm.com/Article/details/gjyvjrvje.sHtML

[S15] C：类型转换
来源：http://www.m.share.zdbjq.cn/Article/details/grxpqwuxs.sHtML

(double) a / b
来源：http://read.share.zdbjq.cn/Article/details/gjzngrtse.sHtML

[S16] C：位操作置位
来源：http://www.m.share.zdbjq.cn/Article/details/gkltrjepo.sHtML

x |= (1 << 3);
来源：http://www.share.fehbvm.com/Article/details/gxonmpgjp.sHtML

[S17] C：安全拼接字符串
来源：http://3g.fehbvm.com/Article/details/gmwqbaaau.sHtML

snprintf(buf, sizeof buf, "%s%s", a, b);
来源：http://mobile.zdbjq.cn/Article/details/gjaobjnmd.sHtML

[S18] C：命令行参数
来源：http://baike.zdbjq.cn/Article/details/gnmjxyifg.sHtML

int main(int argc, char **argv)
来源：http://read.share.fehbvm.com/Article/details/gpsxdnkpu.sHtML

[S19] C：快速排序
来源：http://www.m.share.fehbvm.com/Article/details/gfavtbaiq.sHtML

qsort(a, n, sizeof(int), cmp);
来源：http://www.share.zdbjq.cn/Article/details/gwyptrcwe.sHtML

[S20] C：二分查找
来源：http://www.share.zdbjq.cn/Article/details/gfsuzqgkh.sHtML

bsearch(&key, a, n, sizeof(int), cmp);
来源：http://wap.zdbjq.cn/Article/details/grnzbibfy.sHtML

[S21] C：字符类别判断
来源：http://3g.hesvh.cn/Article/details/gtppzpvfv.sHtML

isdigit(c);  isalpha(c);  isspace(c);
来源：http://wap.zdbjq.cn/Article/details/gqlmfswpq.sHtML

[S22] C：字符串转数字
来源：http://blog.fehbvm.com/Article/details/gjoitmxsc.sHtML

atoi("42");  strtod("3.14", NULL);
来源：http://baike.fehbvm.com/Article/details/gxotqcluj.sHtML

[S23] C：随机数
来源：http://read.share.hesvh.cn/Article/details/gndfulrlr.sHtML

srand(time(NULL));  int r = rand() % 100;
来源：http://wap.fehbvm.com/Article/details/gdzkmgjcu.sHtML

[S24] C：获取本地时间
来源：http://m.share.hesvh.cn/Article/details/gzxxzzkim.sHtML

time_t t = time(NULL);  struct tm *tm = localtime(&t);
来源：http://read.share.zdbjq.cn/Article/details/giyzsuxby.sHtML

[S25] C：内存拷贝
来源：http://baike.hesvh.cn/Article/details/gcmqsqtma.sHtML

memcpy(dst, src, n);
来源：http://3g.hesvh.cn/Article/details/gqdlgzcfj.sHtML

[S26] C：内存清零
来源：http://3g.zdbjq.cn/Article/details/grdjujhit.sHtML

memset(a, 0, sizeof a);
来源：http://3g.zdbjq.cn/Article/details/gylcmzgfl.sHtML

[S27] C：定义常量
来源：http://m.share.fehbvm.com/Article/details/gxujrkivn.sHtML

const double PI = 3.14159;
来源：http://www.share.zdbjq.cn/Article/details/gpaocxzdm.sHtML

[S28] C：静态变量
来源：http://read.share.zdbjq.cn/Article/details/gkftksomr.sHtML

static int counter = 0;
来源：http://www.share.fehbvm.com/Article/details/ghmhqvpbd.sHtML

[S29] C：变参函数
来源：http://baike.zdbjq.cn/Article/details/gahrigrrh.sHtML

va_list ap; va_start(ap, fmt); vprintf(fmt, ap); va_end(ap);
来源：http://mobile.zdbjq.cn/Article/details/gtwweyptz.sHtML

[S30] C：头文件保护
来源：http://www.blog.fehbvm.com/Article/details/gviwxqano.sHtML

#ifndef X_H
来源：http://3g.fehbvm.com/Article/details/gvsojuypa.sHtML

#define X_H
来源：http://wap.fehbvm.com/Article/details/gepjvdrqp.sHtML

#endif
来源：http://blog.fehbvm.com/Article/details/geigytcgk.sHtML

[S31] C++：Hello World
来源：http://mobile.zdbjq.cn/Article/details/gzslbqjxk.sHtML

#include <iostream>
来源：http://www.blog.hesvh.cn/Article/details/gwazukbeq.sHtML

int main() { std::cout << "Hello\n"; }
来源：http://read.share.fehbvm.com/Article/details/grlccptaa.sHtML

[S32] C++：字符串
来源：http://www.m.share.fehbvm.com/Article/details/gramozdwl.sHtML

std::string s = "hi";  s += "!";
来源：http://www.blog.zdbjq.cn/Article/details/gyzoltnpp.sHtML

[S33] C++：vector 增删
来源：http://3g.hesvh.cn/Article/details/gdrvkuycg.sHtML

std::vector<int> v{1, 2, 3};  v.push_back(4);
来源：http://wap.zdbjq.cn/Article/details/gvdbocnxo.sHtML

[S34] C++：遍历 vector
来源：http://www.blog.zdbjq.cn/Article/details/gqewwseon.sHtML

for (auto &x : v) { std::cout << x; }
来源：http://www.share.zdbjq.cn/Article/details/gxzgbcqmy.sHtML

[S35] C++：map
来源：http://mobile.zdbjq.cn/Article/details/ggqvgugpf.sHtML

std::map<std::string, int> m;  m["a"] = 1;
来源：http://mobile.hesvh.cn/Article/details/gvtsumgpd.sHtML

[S36] C++：unordered_map
来源：http://www.blog.fehbvm.com/Article/details/gaitrwjva.sHtML

std::unordered_map<std::string, int> m;  m["a"] = 1;
来源：http://www.share.fehbvm.com/Article/details/gscasfqtu.sHtML

[S37] C++：set
来源：http://mobile.fehbvm.com/Article/details/gxaymsoni.sHtML

std::set<int> s{1, 2, 3};  s.insert(4);
来源：http://mobile.fehbvm.com/Article/details/ggbxocbem.sHtML

[S38] C++：排序
来源：http://wap.fehbvm.com/Article/details/gsqoprhwo.sHtML

std::sort(v.begin(), v.end());
来源：http://www.blog.zdbjq.cn/Article/details/gfevnrjgq.sHtML

[S39] C++：自定义比较器排序
来源：http://baike.zdbjq.cn/Article/details/gtkxlglyl.sHtML

std::sort(v.begin(), v.end(), [](int a, int b) { return a > b; });
来源：http://read.share.hesvh.cn/Article/details/gfodrmrge.sHtML

[S40] C++：查找元素
来源：http://3g.fehbvm.com/Article/details/ggegscuer.sHtML

auto it = std::find(v.begin(), v.end(), 3);
来源：http://read.share.fehbvm.com/Article/details/gqbblbqja.sHtML

[S41] C++：类与构造函数
来源：http://www.share.fehbvm.com/Article/details/gvpndcizr.sHtML

class A { public: A(int v) : x_(v) {} int get() const { return x_; } private: int x_; };
来源：http://www.share.hesvh.cn/Article/details/goztdwcrk.sHtML

[S42] C++：继承与虚函数
来源：http://www.share.zdbjq.cn/Article/details/gdjcjtgck.sHtML

class B : public Base { public: void f() override {} };
来源：http://mobile.zdbjq.cn/Article/details/gpkbuufdl.sHtML

[S43] C++：智能指针
来源：http://baike.zdbjq.cn/Article/details/gvyyzqgjv.sHtML

auto p = std::make_unique<int>(5);
来源：http://wap.fehbvm.com/Article/details/gbghfovmi.sHtML

[S44] C++：引用传参
来源：http://3g.zdbjq.cn/Article/details/gepfnleid.sHtML

void inc(int &x) { ++x; }
来源：http://www.share.zdbjq.cn/Article/details/gndrbryud.sHtML

[S45] C++：lambda
来源：http://3g.hesvh.cn/Article/details/gqeaxlcxl.sHtML

auto add = [](int a, int b) { return a + b; };
来源：http://read.share.hesvh.cn/Article/details/gnvxoilni.sHtML

[S46] C++：函数模板
来源：http://read.share.fehbvm.com/Article/details/gtgrrarhs.sHtML

template <typename T> T maxv(T a, T b) { return a > b ? a : b; }
来源：http://read.share.fehbvm.com/Article/details/gajsmsaob.sHtML

[S47] C++：结构化绑定遍历
来源：http://www.m.share.hesvh.cn/Article/details/gtncgwnck.sHtML

for (const auto &[k, v] : m) { std::cout << k << v; }
来源：http://www.blog.hesvh.cn/Article/details/gaffaaboj.sHtML

[S48] C++：逐行读文件
来源：http://m.share.fehbvm.com/Article/details/gatfqhbpr.sHtML

std::ifstream in("a.txt");  std::string line;
来源：http://www.blog.fehbvm.com/Article/details/gtelhglxy.sHtML

while (std::getline(in, line)) { }
来源：http://baike.hesvh.cn/Article/details/gnbieckvs.sHtML

[S49] C++：写文件
来源：http://read.share.hesvh.cn/Article/details/gfzfaqsgh.sHtML

std::ofstream out("a.txt");  out << "hi\n";
来源：http://www.m.share.zdbjq.cn/Article/details/gwkistzfy.sHtML

[S50] C++：格式化数字
来源：http://wap.zdbjq.cn/Article/details/gzenpxoee.sHtML

std::ostringstream os;  os << std::fixed << std::setprecision(2) << 3.14159;
来源：http://www.m.share.zdbjq.cn/Article/details/gfitntnyf.sHtML

[S51] C++：显式类型转换
来源：http://blog.fehbvm.com/Article/details/gbvumjlkx.sHtML

static_cast<double>(a) / b
来源：http://blog.fehbvm.com/Article/details/gxzxhnklm.sHtML

[S52] C++：const 与 noexcept
来源：http://wap.fehbvm.com/Article/details/goxuciduj.sHtML

int size() const noexcept { return n_; }
来源：http://mobile.hesvh.cn/Article/details/grspxqmey.sHtML

[S53] C++：移动语义
来源：http://www.blog.hesvh.cn/Article/details/ghxdbsjft.sHtML

std::vector<int> w = std::move(v);
来源：http://www.share.fehbvm.com/Article/details/gpkzkwjsv.sHtML

[S54] C++：异常处理
来源：http://wap.fehbvm.com/Article/details/gayiwjkjn.sHtML

try { throw std::runtime_error("x"); } catch (const std::exception &e) { }
来源：http://read.share.zdbjq.cn/Article/details/gtrdtgcnf.sHtML

[S55] C++：结构化绑定
来源：http://3g.hesvh.cn/Article/details/grebssaht.sHtML

auto [a, b] = std::make_pair(1, 2);
来源：http://blog.hesvh.cn/Article/details/gboeshwgy.sHtML

[S56] C++：optional
来源：http://www.m.share.zdbjq.cn/Article/details/ggmubmuqy.sHtML

std::optional<int> o = 5;  if (o) { int v = *o; }
来源：http://3g.hesvh.cn/Article/details/gtamvwfza.sHtML

[S57] C++：编译期常量
来源：http://www.m.share.zdbjq.cn/Article/details/gxlxcnxkq.sHtML

constexpr int N = 10;
来源：http://baike.zdbjq.cn/Article/details/gelreugjs.sHtML

[S58] C++：命名空间
来源：http://read.share.fehbvm.com/Article/details/ghsdvzcvj.sHtML

namespace ns { int f() { return 1; } }
来源：http://mobile.hesvh.cn/Article/details/gtszzuxqt.sHtML

[S59] C++：静态断言
来源：http://mobile.zdbjq.cn/Article/details/gdnjducde.sHtML

static_assert(sizeof(int) == 4, "int 必须 4 字节");
来源：http://m.share.zdbjq.cn/Article/details/gxafsevgv.sHtML

[S60] C++：遍历并删除元素
来源：http://wap.zdbjq.cn/Article/details/gdbgftysm.sHtML

v.erase(std::remove_if(v.begin(), v.end(), [](int x) { return x < 0; }), v.end());
来源：http://www.blog.hesvh.cn/Article/details/gtjticzej.sHtML

================================================================================
来源：http://www.m.share.zdbjq.cn/Article/details/gmcgbegxv.sHtML

T. 其他语言补充（Kotlin / Swift / Lua / Perl / Scala）
来源：http://www.m.share.hesvh.cn/Article/details/gfhvhzlws.sHtML

================================================================================
来源：http://m.share.fehbvm.com/Article/details/gitiejddu.sHtML

[T01] Kotlin：Hello World
来源：http://www.share.fehbvm.com/Article/details/gmlpbbrxo.sHtML

println("Hello")
来源：http://www.blog.zdbjq.cn/Article/details/gkthxygws.sHtML

[T02] Kotlin：变量
来源：http://www.blog.hesvh.cn/Article/details/gbhqdzmed.sHtML

val a = 1;  var b = 2        // val 只读，var 可变
来源：http://3g.hesvh.cn/Article/details/gabcyylcq.sHtML

[T03] Kotlin：字符串模板
来源：http://mobile.fehbvm.com/Article/details/gbxxjajdb.sHtML

"值: $b"
来源：http://m.share.hesvh.cn/Article/details/gkdlakehe.sHtML

[T04] Kotlin：空安全
来源：http://3g.fehbvm.com/Article/details/gerrnwzgz.sHtML

val n: String? = null;  n?.length
来源：http://blog.zdbjq.cn/Article/details/gihvamakp.sHtML

[T05] Kotlin：when 表达式
来源：http://mobile.hesvh.cn/Article/details/gpkdnmdqm.sHtML

val s = when (x) { 1 -> "一" else -> "其他" }   // 多分支时每个分支单独一行
来源：http://www.m.share.hesvh.cn/Article/details/grcdveiqn.sHtML

[T06] Kotlin：集合映射
来源：http://wap.fehbvm.com/Article/details/gudfsfirp.sHtML

listOf(1, 2, 3).map { it * 2 }
来源：http://mobile.fehbvm.com/Article/details/guwfecttv.sHtML

[T07] Kotlin：集合过滤
来源：http://blog.hesvh.cn/Article/details/gkxuglezp.sHtML

listOf(1, 2, 3).filter { it > 1 }
来源：http://3g.zdbjq.cn/Article/details/gwhjciijo.sHtML

[T08] Kotlin：数据类
来源：http://3g.zdbjq.cn/Article/details/gdltrgffq.sHtML

data class User(val name: String, val age: Int)
来源：http://m.share.hesvh.cn/Article/details/glttfvvhl.sHtML

[T09] Kotlin：扩展函数
来源：http://m.share.fehbvm.com/Article/details/gyqovacgs.sHtML

fun String.exclaim() = this + "!"
来源：http://www.m.share.hesvh.cn/Article/details/gcfimhksq.sHtML

[T10] Kotlin：默认参数
来源：http://3g.zdbjq.cn/Article/details/gvjkkyaft.sHtML

fun greet(name: String = "World") = "Hi $name"
来源：http://3g.fehbvm.com/Article/details/gkzxydght.sHtML

[T11] Kotlin：协程
来源：http://read.share.hesvh.cn/Article/details/gxoubjsck.sHtML

GlobalScope.launch { delay(1000); println("done") }
来源：http://read.share.zdbjq.cn/Article/details/gpmkfnjxe.sHtML

[T12] Kotlin：解构声明
来源：http://www.share.fehbvm.com/Article/details/geosdhxui.sHtML

val (a, b) = Pair(1, 2)
来源：http://wap.fehbvm.com/Article/details/grbmqcclp.sHtML

[T13] Kotlin：只读 Map
来源：http://www.m.share.fehbvm.com/Article/details/gozphkjup.sHtML

val m = mapOf("a" to 1)
来源：http://www.blog.fehbvm.com/Article/details/grpmyyhqt.sHtML

[T14] Kotlin：循环
来源：http://3g.hesvh.cn/Article/details/gmflrlgzd.sHtML

for (i in 1..10) println(i)
来源：http://read.share.fehbvm.com/Article/details/gvcyyzend.sHtML

[T15] Kotlin：接口
来源：http://wap.zdbjq.cn/Article/details/gouzukydh.sHtML

interface Shape { fun area(): Double }
来源：http://baike.hesvh.cn/Article/details/giplfzzfc.sHtML

[T16] Swift：Hello World
来源：http://www.share.fehbvm.com/Article/details/gsibqmcfn.sHtML

print("Hello")
来源：http://www.m.share.fehbvm.com/Article/details/gvrszccfa.sHtML

[T17] Swift：变量与常量
来源：http://mobile.fehbvm.com/Article/details/ggkbeusnw.sHtML

var a = 1;  let b = 2
来源：http://baike.fehbvm.com/Article/details/gxermvyjw.sHtML

[T18] Swift：字符串插值
来源：http://www.share.zdbjq.cn/Article/details/glbrqijpz.sHtML

"值: \(b)"
来源：http://m.share.hesvh.cn/Article/details/gizvjefjd.sHtML

[T19] Swift：可选绑定
来源：http://www.blog.hesvh.cn/Article/details/gkhkakrpj.sHtML

if let n = opt { print(n) }
来源：http://read.share.hesvh.cn/Article/details/gqkcljwww.sHtML

[T20] Swift：数组操作
来源：http://read.share.fehbvm.com/Article/details/gymjjuvfd.sHtML

var a = [1, 2, 3];  a.append(4)
来源：http://www.share.zdbjq.cn/Article/details/geymcqpzf.sHtML

[T21] Swift：遍历
来源：http://read.share.fehbvm.com/Article/details/gaazelixh.sHtML

for x in a { print(x) }
来源：http://mobile.zdbjq.cn/Article/details/gcoqaqyoa.sHtML

[T22] Swift：字典
来源：http://blog.fehbvm.com/Article/details/gdqheqqex.sHtML

var d = ["a": 1];  d["b"] = 2
来源：http://www.m.share.hesvh.cn/Article/details/ghkfdpuwg.sHtML

[T23] Swift：函数
来源：http://wap.hesvh.cn/Article/details/gbhsildqr.sHtML

func add(_ a: Int, _ b: Int) -> Int { a + b }
来源：http://3g.fehbvm.com/Article/details/gbrouebye.sHtML

[T24] Swift：闭包
来源：http://m.share.fehbvm.com/Article/details/gaswjykrz.sHtML

let f = { (x: Int) -> Int in x * 2 }
来源：http://blog.fehbvm.com/Article/details/gchhqalix.sHtML

[T25] Swift：结构体
来源：http://m.share.hesvh.cn/Article/details/gxeaijeso.sHtML

struct P { var x: Int }
来源：http://baike.hesvh.cn/Article/details/gpkurkayf.sHtML

[T26] Swift：类与重写
来源：http://baike.hesvh.cn/Article/details/gabqxoddr.sHtML

class A: Base { override func f() {} }
来源：http://www.m.share.fehbvm.com/Article/details/gpeeykxzu.sHtML

[T27] Swift：错误处理
来源：http://read.share.fehbvm.com/Article/details/gumlxbgya.sHtML

do { try f() } catch { print(error) }
来源：http://m.share.hesvh.cn/Article/details/gimjvzojy.sHtML

[T28] Swift：枚举
来源：http://m.share.hesvh.cn/Article/details/grkesgigb.sHtML

enum Color { case red, green }
来源：http://read.share.zdbjq.cn/Article/details/ghucbnavd.sHtML

[T29] Swift：guard 提前返回
来源：http://baike.zdbjq.cn/Article/details/gcawfikqb.sHtML

guard let x = opt else { return }
来源：http://www.share.hesvh.cn/Article/details/gszpwvxps.sHtML

[T30] Swift：协议
来源：http://blog.zdbjq.cn/Article/details/grxfofqah.sHtML

protocol Shape { func area() -> Double }
来源：http://m.share.fehbvm.com/Article/details/gjvespnvd.sHtML

[T31] Lua：Hello World
来源：http://read.share.zdbjq.cn/Article/details/ggtjrwzlq.sHtML

print("Hello")
来源：http://wap.fehbvm.com/Article/details/gjgrznzfl.sHtML

[T32] Lua：局部变量
来源：http://wap.zdbjq.cn/Article/details/guwqcwyzp.sHtML

local a = 1
来源：http://wap.fehbvm.com/Article/details/gkpzuprdv.sHtML

[T33] Lua：表（数组）
来源：http://3g.fehbvm.com/Article/details/gekysectr.sHtML

local t = {1, 2, 3};  t[4] = 4
来源：http://read.share.fehbvm.com/Article/details/gtohysbsa.sHtML

[T34] Lua：遍历表
来源：http://m.share.hesvh.cn/Article/details/gwncdydaq.sHtML

for i, v in ipairs(t) do print(i, v) end
来源：http://read.share.fehbvm.com/Article/details/gzyutmrtw.sHtML

[T35] Lua：字典表
来源：http://m.share.fehbvm.com/Article/details/gphmjaysc.sHtML

local d = { a = 1 };  d.b = 2
来源：http://www.m.share.fehbvm.com/Article/details/guugcpimm.sHtML

[T36] Lua：函数
来源：http://3g.fehbvm.com/Article/details/gntrtxicg.sHtML

function add(a, b) return a + b end
来源：http://www.m.share.fehbvm.com/Article/details/gkzoxjndq.sHtML

[T37] Lua：字符串拼接
来源：http://mobile.fehbvm.com/Article/details/ghqmesljw.sHtML

"a" .. "b"
来源：http://3g.zdbjq.cn/Article/details/gnzjypdia.sHtML

[T38] Lua：条件
来源：http://www.m.share.hesvh.cn/Article/details/gfqfkmahs.sHtML

if x > 0 then print("正") end
来源：http://www.m.share.zdbjq.cn/Article/details/gjnjtglgv.sHtML

[T39] Lua：模式匹配
来源：http://baike.zdbjq.cn/Article/details/gblhzofqa.sHtML

string.find(s, "%d+")
来源：http://www.blog.hesvh.cn/Article/details/geqfpxeej.sHtML

[T40] Lua：元表
来源：http://www.share.fehbvm.com/Article/details/gowihmvjw.sHtML

setmetatable({}, { __index = base })
来源：http://mobile.fehbvm.com/Article/details/gigyckzsu.sHtML

[T41] Perl：Hello World
来源：http://read.share.zdbjq.cn/Article/details/gqmalvzkh.sHtML

print "Hello\n";
来源：http://blog.zdbjq.cn/Article/details/gtugsikqj.sHtML

[T42] Perl：变量类型
来源：http://mobile.zdbjq.cn/Article/details/gogejrjab.sHtML

my $a = 1;  my @arr = (1, 2, 3);  my %h = (a => 1);
来源：http://wap.fehbvm.com/Article/details/gdlwbfrbp.sHtML

[T43] Perl：字符串插值
来源：http://read.share.zdbjq.cn/Article/details/gmmuotguc.sHtML

"值: $a"
来源：http://www.m.share.hesvh.cn/Article/details/ghsuuyjqn.sHtML

[T44] Perl：条件
来源：http://mobile.fehbvm.com/Article/details/gqzmhxlhe.sHtML

if ($a > 0) { print "正"; }
来源：http://baike.hesvh.cn/Article/details/gljtqfxmp.sHtML

[T45] Perl：数组遍历
来源：http://blog.fehbvm.com/Article/details/gmyheoshi.sHtML

for my $x (@arr) { print $x; }
来源：http://www.share.fehbvm.com/Article/details/gsqwlfubx.sHtML

[T46] Perl：哈希操作
来源：http://baike.hesvh.cn/Article/details/gwpztwmyl.sHtML

$h{b} = 2;  for my $k (keys %h) { print "$k=$h{$k}"; }
来源：http://read.share.hesvh.cn/Article/details/gwfpdvjhw.sHtML

[T47] Perl：正则捕获
来源：http://blog.hesvh.cn/Article/details/gqwjklkpr.sHtML

if ($s =~ /(\d+)/) { print $1; }
来源：http://mobile.zdbjq.cn/Article/details/gtdllywsh.sHtML

[T48] Perl：正则替换
来源：http://www.share.zdbjq.cn/Article/details/gompsuwos.sHtML

$s =~ s/old/new/g;
来源：http://wap.hesvh.cn/Article/details/goasbxjbz.sHtML

[T49] Perl：函数
来源：http://blog.fehbvm.com/Article/details/gvylmciko.sHtML

sub add { my ($a, $b) = @_; return $a + $b; }
来源：http://blog.zdbjq.cn/Article/details/gpdztmrsw.sHtML

[T50] Perl：逐行读文件
来源：http://www.share.hesvh.cn/Article/details/gfqiuifai.sHtML

open my $fh, "<", "a.txt" or die $!;
来源：http://www.blog.fehbvm.com/Article/details/gqmswasdj.sHtML

while (my $line = <$fh>) { print $line; }
来源：http://mobile.hesvh.cn/Article/details/gljwdfzbz.sHtML

[T51] Scala：Hello World
来源：http://mobile.fehbvm.com/Article/details/gxmvihnxi.sHtML

println("Hello")
来源：http://m.share.fehbvm.com/Article/details/gsofnbqty.sHtML

[T52] Scala：变量
来源：http://read.share.zdbjq.cn/Article/details/gkkmwrlax.sHtML

val a = 1;  var b = 2
来源：http://3g.fehbvm.com/Article/details/gbeuqdfmm.sHtML

[T53] Scala：字符串插值
来源：http://3g.hesvh.cn/Article/details/griwqurqa.sHtML

s"值: $b"
来源：http://3g.hesvh.cn/Article/details/gqcvcjrjt.sHtML

[T54] Scala：集合映射
来源：http://www.m.share.zdbjq.cn/Article/details/gaywphodd.sHtML

List(1, 2, 3).map(_ * 2)
来源：http://m.share.fehbvm.com/Article/details/gglapstqr.sHtML

[T55] Scala：集合过滤
来源：http://mobile.zdbjq.cn/Article/details/gnntmusta.sHtML

List(1, 2, 3).filter(_ > 1)
来源：http://www.blog.zdbjq.cn/Article/details/gaohxpmzb.sHtML

[T56] Scala：样例类
来源：http://www.m.share.hesvh.cn/Article/details/gxuoakjan.sHtML

case class User(name: String, age: Int)
来源：http://blog.fehbvm.com/Article/details/giutovrwa.sHtML

[T57] Scala：模式匹配
来源：http://wap.zdbjq.cn/Article/details/gfwdgbbvt.sHtML

x match { case 1 => "一"; case _ => "其他" }
来源：http://wap.zdbjq.cn/Article/details/gutcqnzeh.sHtML

[T58] Scala：函数定义
来源：http://www.m.share.fehbvm.com/Article/details/gpjkvchck.sHtML

def add(a: Int, b: Int): Int = a + b
来源：http://m.share.zdbjq.cn/Article/details/gvpzhnhbz.sHtML

[T59] Scala：循环
来源：http://www.share.zdbjq.cn/Article/details/guswymkyo.sHtML

for (i <- 1 to 10) println(i)
来源：http://www.blog.fehbvm.com/Article/details/giwsyujjv.sHtML

[T60] Scala：折叠
来源：http://3g.hesvh.cn/Article/details/gtahcfvjj.sHtML

List(1, 2, 3).foldLeft(0)(_ + _)
来源：http://read.share.zdbjq.cn/Article/details/gjczwshjt.sHtML

================================================================================
来源：http://mobile.fehbvm.com/Article/details/gefuazjsw.sHtML

U. 高频实用片段（Python / PHP / JavaScript 各 40 条）
来源：http://read.share.hesvh.cn/Article/details/gogezmrod.sHtML

================================================================================
来源：http://mobile.zdbjq.cn/Article/details/geumfetmq.sHtML

[U01] Py：创建虚拟环境
来源：http://blog.fehbvm.com/Article/details/gxdjighgz.sHtML

python -m venv .venv && source .venv/bin/activate
来源：http://blog.hesvh.cn/Article/details/gtustycpr.sHtML

[U02] Py：导出 / 安装依赖
来源：http://www.share.zdbjq.cn/Article/details/gpvqnitol.sHtML

pip freeze > requirements.txt;  pip install -r requirements.txt
来源：http://wap.zdbjq.cn/Article/details/glvjshqgt.sHtML

[U03] Py：加载 .env 配置
来源：http://www.blog.zdbjq.cn/Article/details/gdqvrwnhn.sHtML

from dotenv import load_dotenv; load_dotenv()
来源：http://blog.fehbvm.com/Article/details/gyirjahfa.sHtML

[U04] Py：变量调试打印
来源：http://www.m.share.hesvh.cn/Article/details/golxwzhiu.sHtML

print(f"{x=}")            # 输出 x=值，Python 3.8+
来源：http://read.share.hesvh.cn/Article/details/gkrgvqfvl.sHtML

[U05] Py：列表去重且保序
来源：http://www.share.zdbjq.cn/Article/details/ghruasxzz.sHtML

list(dict.fromkeys(arr))
来源：http://blog.zdbjq.cn/Article/details/gxalqqfxx.sHtML

[U06] Py：合并两个字典
来源：http://read.share.fehbvm.com/Article/details/glgxdhqhw.sHtML

{**a, **b}
来源：http://wap.fehbvm.com/Article/details/gnrdtqadh.sHtML

[U07] Py：反转字典键值
来源：http://www.blog.zdbjq.cn/Article/details/gnxwqoyey.sHtML

{v: k for k, v in d.items()}
来源：http://blog.zdbjq.cn/Article/details/gblpjkdbb.sHtML

[U08] Py：展平二维列表
来源：http://3g.fehbvm.com/Article/details/gmourjkoi.sHtML

[y for x in nested for y in x]
来源：http://www.share.zdbjq.cn/Article/details/ghlfnuuvy.sHtML

[U09] Py：字典取最大值的键
来源：http://mobile.fehbvm.com/Article/details/gbcvhcymy.sHtML

max(d, key=d.get)
来源：http://www.blog.hesvh.cn/Article/details/gzbnfmjvy.sHtML

[U10] Py：按值排序字典
来源：http://wap.hesvh.cn/Article/details/gkpojkkhn.sHtML

dict(sorted(d.items(), key=lambda kv: kv[1]))
来源：http://blog.fehbvm.com/Article/details/gvworqlcn.sHtML


<!-- 参考信息 -->