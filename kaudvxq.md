代发 wailian999

split -l 1000 big.log part_
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gwlyabvvb.sHtML

[R74] 批量重命名
来源：http://m.share.fanxiaobao.xyz/Article/details/gcubcespc.sHtML

for f in *.jpeg; do mv "$f" "${f%.jpeg}.jpg"; done
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gfdnfikls.sHtML

[R75] 导出环境变量
来源：http://m.share.fanxiaobao.xyz/Article/details/gdejopsew.sHtML

export PATH="$HOME/bin:$PATH"
来源：http://www.blog.fanxiaobao.xyz/Article/details/gqkbqfwyu.sHtML

[R76] 使用临时文件
来源：http://3g.fanxiaobao.xyz/Article/details/gispcwkgt.sHtML

tmp=$(mktemp); trap 'rm -f "$tmp"' EXIT
来源：http://www.blog.fanxiaobao.xyz/Article/details/gfebltntg.sHtML

[R77] 读取用户输入
来源：http://www.share.fanxiaobao.xyz/Article/details/gtlxvfzxf.sHtML

read -rp "请输入: " ans
来源：http://mobile.fanxiaobao.xyz/Article/details/ggrimpjdd.sHtML

[R78] 交互式菜单
来源：http://3g.fanxiaobao.xyz/Article/details/glboozgdm.sHtML

select opt in a b c; do echo "$opt"; break; done
来源：http://www.share.fanxiaobao.xyz/Article/details/ghqtrbgyv.sHtML

[R79] 解析命令行选项
来源：http://wap.fanxiaobao.xyz/Article/details/gkdjxjhhj.sHtML

while getopts "v:f:" o; do case $o in v) V=$OPTARG ;; f) F=$OPTARG ;; esac; done
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gdxdyvusb.sHtML

[R80] 查看脚本执行耗时
来源：http://wap.fanxiaobao.xyz/Article/details/geapuckiv.sHtML

time ./run.sh
来源：http://www.blog.fanxiaobao.xyz/Article/details/gurhuskrb.sHtML

================================================================================
来源：http://blog.fanxiaobao.xyz/Article/details/gczefqsdq.sHtML

S. C / C++ 专题
来源：http://www.blog.fanxiaobao.xyz/Article/details/gocyqwejg.sHtML

================================================================================
来源：http://blog.fanxiaobao.xyz/Article/details/gdpbtvowg.sHtML

[S01] C：Hello World
来源：http://wap.fanxiaobao.xyz/Article/details/gsxyacgrx.sHtML

#include <stdio.h>
来源：http://wap.fanxiaobao.xyz/Article/details/gfqmxykeo.sHtML

int main(void) { printf("Hello\n"); return 0; }
来源：http://baike.fanxiaobao.xyz/Article/details/gjxdqxsnf.sHtML

[S02] C：变量与格式化输出
来源：http://mobile.fanxiaobao.xyz/Article/details/gdedubvzu.sHtML

int a = 10; printf("%d\n", a);
来源：http://mobile.fanxiaobao.xyz/Article/details/gqxqpvkyf.sHtML

[S03] C：读入整数
来源：http://www.blog.fanxiaobao.xyz/Article/details/ghnzzhkij.sHtML

int x; scanf("%d", &x);
来源：http://read.share.fanxiaobao.xyz/Article/details/gjchetviw.sHtML

[S04] C：字符串复制
来源：http://wap.fanxiaobao.xyz/Article/details/ghhhuksbs.sHtML

char dst[32]; strcpy(dst, "hi");
来源：http://www.share.fanxiaobao.xyz/Article/details/ggfzofxvz.sHtML

[S05] C：字符串长度
来源：http://3g.fanxiaobao.xyz/Article/details/gacywbbxk.sHtML

strlen(s)
来源：http://blog.fanxiaobao.xyz/Article/details/gtpdgqkwv.sHtML

[S06] C：字符串比较
来源：http://m.share.fanxiaobao.xyz/Article/details/ggjudpycz.sHtML

strcmp(a, b) == 0
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gwalmkxgr.sHtML

[S07] C：数组遍历求和
来源：http://www.share.fanxiaobao.xyz/Article/details/glchngtoq.sHtML

for (int i = 0; i < n; i++) sum += a[i];
来源：http://m.share.fanxiaobao.xyz/Article/details/gnrcvhftm.sHtML

[S08] C：动态内存分配与释放
来源：http://blog.fanxiaobao.xyz/Article/details/gikiaphfk.sHtML

int *p = malloc(sizeof(int) * n); ... free(p);
来源：http://mobile.fanxiaobao.xyz/Article/details/gsyekvkhs.sHtML

[S09] C：结构体定义与初始化
来源：http://blog.fanxiaobao.xyz/Article/details/grwlfftmc.sHtML

struct Point { int x, y; };  struct Point p = {1, 2};
来源：http://blog.fanxiaobao.xyz/Article/details/gafjdesvj.sHtML

[S10] C：指针与解引用
来源：http://wap.fanxiaobao.xyz/Article/details/gpxamoqda.sHtML

int *p = &a;  *p = 5;
来源：http://baike.fanxiaobao.xyz/Article/details/gcoaxnypl.sHtML

[S11] C：逐行读文件
来源：http://www.share.fanxiaobao.xyz/Article/details/gnvbsyqeo.sHtML

FILE *f = fopen("a.txt", "r");
来源：http://m.share.fanxiaobao.xyz/Article/details/gyvsbglbd.sHtML

while (fgets(buf, sizeof buf, f)) { }
来源：http://m.share.fanxiaobao.xyz/Article/details/gbngllclk.sHtML

fclose(f);
来源：http://mobile.fanxiaobao.xyz/Article/details/gbyvtezok.sHtML

[S12] C：写文件
来源：http://mobile.fanxiaobao.xyz/Article/details/geilvmggs.sHtML

FILE *f = fopen("a.txt", "w");  fprintf(f, "hi\n");  fclose(f);
来源：http://m.share.fanxiaobao.xyz/Article/details/gfikmacbg.sHtML

[S13] C：宏定义
来源：http://baike.fanxiaobao.xyz/Article/details/gfuqrpxbp.sHtML

#define MAX(a, b) ((a) > (b) ? (a) : (b))
来源：http://www.blog.fanxiaobao.xyz/Article/details/giktlbtdv.sHtML

[S14] C：枚举
来源：http://m.share.fanxiaobao.xyz/Article/details/gvwkyaxvm.sHtML

enum Color { RED, GREEN, BLUE };
来源：http://wap.fanxiaobao.xyz/Article/details/ghzlaesuq.sHtML

[S15] C：类型转换
来源：http://wap.fanxiaobao.xyz/Article/details/ghaxzzsjo.sHtML

(double) a / b
来源：http://baike.fanxiaobao.xyz/Article/details/gaswzgsgz.sHtML

[S16] C：位操作置位
来源：http://www.share.fanxiaobao.xyz/Article/details/gasdbgcmk.sHtML

x |= (1 << 3);
来源：http://3g.fanxiaobao.xyz/Article/details/gnkhzpydp.sHtML

[S17] C：安全拼接字符串
来源：http://read.share.fanxiaobao.xyz/Article/details/glczultey.sHtML

snprintf(buf, sizeof buf, "%s%s", a, b);
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gnqhicloq.sHtML

[S18] C：命令行参数
来源：http://www.share.fanxiaobao.xyz/Article/details/gnfvncumb.sHtML

int main(int argc, char **argv)
来源：http://mobile.fanxiaobao.xyz/Article/details/glkgssect.sHtML

[S19] C：快速排序
来源：http://read.share.fanxiaobao.xyz/Article/details/grqgwqxct.sHtML

qsort(a, n, sizeof(int), cmp);
来源：http://baike.fanxiaobao.xyz/Article/details/geofevptq.sHtML

[S20] C：二分查找
来源：http://wap.fanxiaobao.xyz/Article/details/gnkzggnxe.sHtML

bsearch(&key, a, n, sizeof(int), cmp);
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gaigtbgtg.sHtML

[S21] C：字符类别判断
来源：http://baike.fanxiaobao.xyz/Article/details/gdxdqojrm.sHtML

isdigit(c);  isalpha(c);  isspace(c);
来源：http://mobile.fanxiaobao.xyz/Article/details/gnmgqdnyz.sHtML

[S22] C：字符串转数字
来源：http://m.share.fanxiaobao.xyz/Article/details/gmqijwdsr.sHtML

atoi("42");  strtod("3.14", NULL);
来源：http://m.share.fanxiaobao.xyz/Article/details/gazjqqnnc.sHtML

[S23] C：随机数
来源：http://www.share.fanxiaobao.xyz/Article/details/gyqviwfsu.sHtML

srand(time(NULL));  int r = rand() % 100;
来源：http://read.share.fanxiaobao.xyz/Article/details/gphdfoqbj.sHtML

[S24] C：获取本地时间
来源：http://blog.fanxiaobao.xyz/Article/details/gfrtvpopw.sHtML

time_t t = time(NULL);  struct tm *tm = localtime(&t);
来源：http://m.share.fanxiaobao.xyz/Article/details/gzewudvwr.sHtML

[S25] C：内存拷贝
来源：http://mobile.fanxiaobao.xyz/Article/details/gpqdcoyhe.sHtML

memcpy(dst, src, n);
来源：http://blog.fanxiaobao.xyz/Article/details/gvcvcasjo.sHtML

[S26] C：内存清零
来源：http://mobile.fanxiaobao.xyz/Article/details/gtizgjcmg.sHtML

memset(a, 0, sizeof a);
来源：http://read.share.fanxiaobao.xyz/Article/details/gagzagnps.sHtML

[S27] C：定义常量
来源：http://blog.fanxiaobao.xyz/Article/details/glomisjnr.sHtML

const double PI = 3.14159;
来源：http://www.blog.fanxiaobao.xyz/Article/details/gsutkucwq.sHtML

[S28] C：静态变量
来源：http://blog.fanxiaobao.xyz/Article/details/gyuuwajfu.sHtML

static int counter = 0;
来源：http://m.share.fanxiaobao.xyz/Article/details/gvzmatuht.sHtML

[S29] C：变参函数
来源：http://www.share.fanxiaobao.xyz/Article/details/gdxyqlysj.sHtML

va_list ap; va_start(ap, fmt); vprintf(fmt, ap); va_end(ap);
来源：http://3g.fanxiaobao.xyz/Article/details/gbhizfkao.sHtML

[S30] C：头文件保护
来源：http://read.share.fanxiaobao.xyz/Article/details/gnterfcyx.sHtML

#ifndef X_H
来源：http://read.share.fanxiaobao.xyz/Article/details/gepgvmowk.sHtML

#define X_H
来源：http://www.blog.fanxiaobao.xyz/Article/details/gkpqwsflu.sHtML

#endif
来源：http://wap.fanxiaobao.xyz/Article/details/gsobzirmd.sHtML

[S31] C++：Hello World
来源：http://mobile.fanxiaobao.xyz/Article/details/gmkvchjoe.sHtML

#include <iostream>
来源：http://wap.fanxiaobao.xyz/Article/details/gfripfbxw.sHtML

int main() { std::cout << "Hello\n"; }
来源：http://mobile.fanxiaobao.xyz/Article/details/gbgvefocy.sHtML

[S32] C++：字符串
来源：http://baike.fanxiaobao.xyz/Article/details/gncaqrfng.sHtML

std::string s = "hi";  s += "!";
来源：http://3g.fanxiaobao.xyz/Article/details/gyucayntl.sHtML

[S33] C++：vector 增删
来源：http://baike.fanxiaobao.xyz/Article/details/grmdclnhi.sHtML

std::vector<int> v{1, 2, 3};  v.push_back(4);
来源：http://www.share.fanxiaobao.xyz/Article/details/ggdfwzxxv.sHtML

[S34] C++：遍历 vector
来源：http://wap.fanxiaobao.xyz/Article/details/gktsxfvzf.sHtML

for (auto &x : v) { std::cout << x; }
来源：http://3g.fanxiaobao.xyz/Article/details/gurliilaj.sHtML

[S35] C++：map
来源：http://blog.fanxiaobao.xyz/Article/details/gyhwcqejp.sHtML

std::map<std::string, int> m;  m["a"] = 1;
来源：http://www.share.fanxiaobao.xyz/Article/details/gkfcxbbov.sHtML

[S36] C++：unordered_map
来源：http://mobile.fanxiaobao.xyz/Article/details/gukodtdhj.sHtML

std::unordered_map<std::string, int> m;  m["a"] = 1;
来源：http://wap.fanxiaobao.xyz/Article/details/gtrzlydmi.sHtML

[S37] C++：set
来源：http://www.blog.fanxiaobao.xyz/Article/details/gxqstrhpv.sHtML

std::set<int> s{1, 2, 3};  s.insert(4);
来源：http://baike.fanxiaobao.xyz/Article/details/gwuhlpvca.sHtML

[S38] C++：排序
来源：http://mobile.fanxiaobao.xyz/Article/details/gmjuooxzx.sHtML

std::sort(v.begin(), v.end());
来源：http://blog.fanxiaobao.xyz/Article/details/gytqckurd.sHtML

[S39] C++：自定义比较器排序
来源：http://3g.fanxiaobao.xyz/Article/details/gkhgqsqjj.sHtML

std::sort(v.begin(), v.end(), [](int a, int b) { return a > b; });
来源：http://read.share.fanxiaobao.xyz/Article/details/gforbklhj.sHtML

[S40] C++：查找元素
来源：http://3g.fanxiaobao.xyz/Article/details/gqrtsczoz.sHtML

auto it = std::find(v.begin(), v.end(), 3);
来源：http://3g.fanxiaobao.xyz/Article/details/gkorpktxh.sHtML

[S41] C++：类与构造函数
来源：http://www.share.fanxiaobao.xyz/Article/details/glluayziw.sHtML

class A { public: A(int v) : x_(v) {} int get() const { return x_; } private: int x_; };
来源：http://read.share.fanxiaobao.xyz/Article/details/ggjkigmmo.sHtML

[S42] C++：继承与虚函数
来源：http://blog.fanxiaobao.xyz/Article/details/gzvdeeqvt.sHtML

class B : public Base { public: void f() override {} };
来源：http://m.share.fanxiaobao.xyz/Article/details/gndajhied.sHtML

[S43] C++：智能指针
来源：http://wap.fanxiaobao.xyz/Article/details/gqrsbbzez.sHtML

auto p = std::make_unique<int>(5);
来源：http://www.blog.fanxiaobao.xyz/Article/details/ghhanrewe.sHtML

[S44] C++：引用传参
来源：http://m.share.fanxiaobao.xyz/Article/details/grpicvdqp.sHtML

void inc(int &x) { ++x; }
来源：http://blog.fanxiaobao.xyz/Article/details/gsdlpisns.sHtML

[S45] C++：lambda
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gsibktrnf.sHtML

auto add = [](int a, int b) { return a + b; };
来源：http://www.m.share.fanxiaobao.xyz/Article/details/ghtupmhaj.sHtML

[S46] C++：函数模板
来源：http://blog.fanxiaobao.xyz/Article/details/gmwmjsubw.sHtML

template <typename T> T maxv(T a, T b) { return a > b ? a : b; }
来源：http://www.blog.fanxiaobao.xyz/Article/details/giwitrtfo.sHtML

[S47] C++：结构化绑定遍历
来源：http://read.share.fanxiaobao.xyz/Article/details/gudxiffna.sHtML

for (const auto &[k, v] : m) { std::cout << k << v; }
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gyxdlvzmu.sHtML

[S48] C++：逐行读文件
来源：http://3g.fanxiaobao.xyz/Article/details/gyfkacztj.sHtML

std::ifstream in("a.txt");  std::string line;
来源：http://www.blog.fanxiaobao.xyz/Article/details/giaiwqvuf.sHtML

while (std::getline(in, line)) { }
来源：http://read.share.fanxiaobao.xyz/Article/details/gmlweenfs.sHtML

[S49] C++：写文件
来源：http://wap.fanxiaobao.xyz/Article/details/genszlcdx.sHtML

std::ofstream out("a.txt");  out << "hi\n";
来源：http://m.share.fanxiaobao.xyz/Article/details/gujyevxaa.sHtML

[S50] C++：格式化数字
来源：http://read.share.fanxiaobao.xyz/Article/details/gqefwgjpa.sHtML

std::ostringstream os;  os << std::fixed << std::setprecision(2) << 3.14159;
来源：http://wap.fanxiaobao.xyz/Article/details/gehfrdzqh.sHtML

[S51] C++：显式类型转换
来源：http://www.share.fanxiaobao.xyz/Article/details/gcojfprhg.sHtML

static_cast<double>(a) / b
来源：http://m.share.fanxiaobao.xyz/Article/details/gwrtndwzc.sHtML

[S52] C++：const 与 noexcept
来源：http://read.share.fanxiaobao.xyz/Article/details/gqqsyyjtm.sHtML

int size() const noexcept { return n_; }
来源：http://mobile.fanxiaobao.xyz/Article/details/gyvdynsqh.sHtML

[S53] C++：移动语义
来源：http://www.blog.fanxiaobao.xyz/Article/details/guhbrtvjy.sHtML

std::vector<int> w = std::move(v);
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gntsrqtcl.sHtML

[S54] C++：异常处理
来源：http://www.share.fanxiaobao.xyz/Article/details/glhmpufxv.sHtML

try { throw std::runtime_error("x"); } catch (const std::exception &e) { }
来源：http://baike.fanxiaobao.xyz/Article/details/gdywakuzw.sHtML

[S55] C++：结构化绑定
来源：http://www.blog.fanxiaobao.xyz/Article/details/gfyrznydz.sHtML

auto [a, b] = std::make_pair(1, 2);
来源：http://mobile.fanxiaobao.xyz/Article/details/gshhtfmbe.sHtML

[S56] C++：optional
来源：http://3g.fanxiaobao.xyz/Article/details/garjhvbce.sHtML

std::optional<int> o = 5;  if (o) { int v = *o; }
来源：http://baike.fanxiaobao.xyz/Article/details/gmtbadgtk.sHtML

[S57] C++：编译期常量
来源：http://3g.fanxiaobao.xyz/Article/details/ggfqizqqt.sHtML

constexpr int N = 10;
来源：http://read.share.fanxiaobao.xyz/Article/details/gwouotynn.sHtML

[S58] C++：命名空间
来源：http://baike.fanxiaobao.xyz/Article/details/gggradevt.sHtML

namespace ns { int f() { return 1; } }
来源：http://mobile.fanxiaobao.xyz/Article/details/gajjrtphi.sHtML

[S59] C++：静态断言
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gtpqdvbdi.sHtML

static_assert(sizeof(int) == 4, "int 必须 4 字节");
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gdmwrnpsa.sHtML

[S60] C++：遍历并删除元素
来源：http://mobile.fanxiaobao.xyz/Article/details/gbsatmvcg.sHtML

v.erase(std::remove_if(v.begin(), v.end(), [](int x) { return x < 0; }), v.end());
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gtwqvgmwa.sHtML

================================================================================
来源：http://baike.fanxiaobao.xyz/Article/details/gltzufwzk.sHtML

T. 其他语言补充（Kotlin / Swift / Lua / Perl / Scala）
来源：http://blog.fanxiaobao.xyz/Article/details/guipkcblr.sHtML

================================================================================
来源：http://www.blog.fanxiaobao.xyz/Article/details/gaenfagge.sHtML

[T01] Kotlin：Hello World
来源：http://m.share.fanxiaobao.xyz/Article/details/gejezbpal.sHtML

println("Hello")
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gmbhukgdl.sHtML

[T02] Kotlin：变量
来源：http://blog.fanxiaobao.xyz/Article/details/gyojfitdf.sHtML

val a = 1;  var b = 2        // val 只读，var 可变
来源：http://m.share.fanxiaobao.xyz/Article/details/grlthxdqb.sHtML

[T03] Kotlin：字符串模板
来源：http://blog.fanxiaobao.xyz/Article/details/gjmiaqxts.sHtML

"值: $b"
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gordtqbsl.sHtML

[T04] Kotlin：空安全
来源：http://wap.fanxiaobao.xyz/Article/details/guoawwnny.sHtML

val n: String? = null;  n?.length
来源：http://mobile.fanxiaobao.xyz/Article/details/goetpqapc.sHtML

[T05] Kotlin：when 表达式
来源：http://www.blog.fanxiaobao.xyz/Article/details/gebpjkswf.sHtML

val s = when (x) { 1 -> "一" else -> "其他" }   // 多分支时每个分支单独一行
来源：http://3g.fanxiaobao.xyz/Article/details/garpbgxqp.sHtML

[T06] Kotlin：集合映射
来源：http://read.share.fanxiaobao.xyz/Article/details/gyuwejxwk.sHtML

listOf(1, 2, 3).map { it * 2 }
来源：http://blog.fanxiaobao.xyz/Article/details/ghmgebags.sHtML

[T07] Kotlin：集合过滤
来源：http://www.m.share.fanxiaobao.xyz/Article/details/ggizneaxn.sHtML

listOf(1, 2, 3).filter { it > 1 }
来源：http://read.share.fanxiaobao.xyz/Article/details/glvygmkql.sHtML

[T08] Kotlin：数据类
来源：http://mobile.fanxiaobao.xyz/Article/details/gbxocromy.sHtML

data class User(val name: String, val age: Int)
来源：http://www.blog.fanxiaobao.xyz/Article/details/gdlazjowu.sHtML

[T09] Kotlin：扩展函数
来源：http://blog.fanxiaobao.xyz/Article/details/gzcxskukw.sHtML

fun String.exclaim() = this + "!"
来源：http://baike.fanxiaobao.xyz/Article/details/gjhwigszn.sHtML

[T10] Kotlin：默认参数
来源：http://baike.fanxiaobao.xyz/Article/details/gkqzabbyz.sHtML

fun greet(name: String = "World") = "Hi $name"
来源：http://www.share.fanxiaobao.xyz/Article/details/gkzzlnhjc.sHtML

[T11] Kotlin：协程
来源：http://3g.fanxiaobao.xyz/Article/details/gjgqgixsi.sHtML

GlobalScope.launch { delay(1000); println("done") }
来源：http://www.blog.fanxiaobao.xyz/Article/details/gdemkzxev.sHtML

[T12] Kotlin：解构声明
来源：http://mobile.fanxiaobao.xyz/Article/details/grmxlieyy.sHtML

val (a, b) = Pair(1, 2)
来源：http://read.share.fanxiaobao.xyz/Article/details/gdfagngji.sHtML

[T13] Kotlin：只读 Map
来源：http://baike.fanxiaobao.xyz/Article/details/gqphrcqum.sHtML

val m = mapOf("a" to 1)
来源：http://m.share.fanxiaobao.xyz/Article/details/gvsajthmx.sHtML

[T14] Kotlin：循环
来源：http://baike.fanxiaobao.xyz/Article/details/gvyimvrni.sHtML

for (i in 1..10) println(i)
来源：http://www.blog.fanxiaobao.xyz/Article/details/gjpcflyfa.sHtML

[T15] Kotlin：接口
来源：http://www.blog.fanxiaobao.xyz/Article/details/gcynvhizz.sHtML

interface Shape { fun area(): Double }
来源：http://www.share.fanxiaobao.xyz/Article/details/gmynmiasq.sHtML

[T16] Swift：Hello World
来源：http://blog.fanxiaobao.xyz/Article/details/gpvawxoqu.sHtML

print("Hello")
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gwrtrjqbn.sHtML

[T17] Swift：变量与常量
来源：http://wap.fanxiaobao.xyz/Article/details/guiauuiaz.sHtML

var a = 1;  let b = 2
来源：http://3g.fanxiaobao.xyz/Article/details/gkbsxcjqk.sHtML

[T18] Swift：字符串插值
来源：http://www.blog.fanxiaobao.xyz/Article/details/gxfzhuwcv.sHtML

"值: \(b)"
来源：http://baike.fanxiaobao.xyz/Article/details/goiqbjwop.sHtML

[T19] Swift：可选绑定
来源：http://read.share.fanxiaobao.xyz/Article/details/garysfduu.sHtML

if let n = opt { print(n) }
来源：http://read.share.fanxiaobao.xyz/Article/details/gdnkavstn.sHtML

[T20] Swift：数组操作
来源：http://www.m.share.fanxiaobao.xyz/Article/details/ggjhhwpay.sHtML

var a = [1, 2, 3];  a.append(4)
来源：http://www.share.fanxiaobao.xyz/Article/details/gvspmbvdy.sHtML

[T21] Swift：遍历
来源：http://read.share.fanxiaobao.xyz/Article/details/gafroqico.sHtML

for x in a { print(x) }
来源：http://m.share.fanxiaobao.xyz/Article/details/gnkhoxryk.sHtML

[T22] Swift：字典
来源：http://blog.fanxiaobao.xyz/Article/details/goteopkrv.sHtML

var d = ["a": 1];  d["b"] = 2
来源：http://mobile.fanxiaobao.xyz/Article/details/gfbqbnuot.sHtML

[T23] Swift：函数
来源：http://read.share.fanxiaobao.xyz/Article/details/gdncyvanb.sHtML

func add(_ a: Int, _ b: Int) -> Int { a + b }
来源：http://m.share.fanxiaobao.xyz/Article/details/gbccjltdq.sHtML

[T24] Swift：闭包
来源：http://www.share.fanxiaobao.xyz/Article/details/gfyoyszhv.sHtML

let f = { (x: Int) -> Int in x * 2 }
来源：http://www.share.fanxiaobao.xyz/Article/details/gredqpoll.sHtML

[T25] Swift：结构体
来源：http://read.share.fanxiaobao.xyz/Article/details/gduresxsl.sHtML

struct P { var x: Int }
来源：http://read.share.fanxiaobao.xyz/Article/details/gtbjzmqmm.sHtML

[T26] Swift：类与重写
来源：http://baike.fanxiaobao.xyz/Article/details/glgukkapb.sHtML

class A: Base { override func f() {} }
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gutajfbcp.sHtML

[T27] Swift：错误处理
来源：http://www.share.fanxiaobao.xyz/Article/details/gihrqkjto.sHtML

do { try f() } catch { print(error) }
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gtgwsoxng.sHtML

[T28] Swift：枚举
来源：http://www.m.share.fanxiaobao.xyz/Article/details/geqcxwxji.sHtML

enum Color { case red, green }
来源：http://baike.fanxiaobao.xyz/Article/details/gkmlufbzn.sHtML

[T29] Swift：guard 提前返回
来源：http://read.share.fanxiaobao.xyz/Article/details/glrfzoiry.sHtML

guard let x = opt else { return }
来源：http://blog.fanxiaobao.xyz/Article/details/gzqudntjr.sHtML

[T30] Swift：协议
来源：http://blog.fanxiaobao.xyz/Article/details/gxxzztdch.sHtML

protocol Shape { func area() -> Double }
来源：http://read.share.fanxiaobao.xyz/Article/details/gfmdieexl.sHtML

[T31] Lua：Hello World
来源：http://3g.fanxiaobao.xyz/Article/details/gdjgwqwhk.sHtML

print("Hello")
来源：http://blog.fanxiaobao.xyz/Article/details/gzfjozggf.sHtML

[T32] Lua：局部变量
来源：http://read.share.fanxiaobao.xyz/Article/details/gkuxsoysg.sHtML

local a = 1
来源：http://wap.fanxiaobao.xyz/Article/details/gdpxkkdzk.sHtML

[T33] Lua：表（数组）
来源：http://mobile.fanxiaobao.xyz/Article/details/gcesruqez.sHtML

local t = {1, 2, 3};  t[4] = 4
来源：http://blog.fanxiaobao.xyz/Article/details/glvonbxrp.sHtML

[T34] Lua：遍历表
来源：http://wap.fanxiaobao.xyz/Article/details/gjpcugtgv.sHtML

for i, v in ipairs(t) do print(i, v) end
来源：http://www.share.fanxiaobao.xyz/Article/details/gyiroqfbe.sHtML

[T35] Lua：字典表
来源：http://baike.fanxiaobao.xyz/Article/details/ghgxuhish.sHtML

local d = { a = 1 };  d.b = 2
来源：http://www.share.fanxiaobao.xyz/Article/details/giohysyoo.sHtML

[T36] Lua：函数
来源：http://m.share.fanxiaobao.xyz/Article/details/gmixmopfn.sHtML

function add(a, b) return a + b end
来源：http://www.share.fanxiaobao.xyz/Article/details/gxhttdobe.sHtML

[T37] Lua：字符串拼接
来源：http://baike.fanxiaobao.xyz/Article/details/gzierxvrk.sHtML

"a" .. "b"
来源：http://3g.fanxiaobao.xyz/Article/details/gibnmpxxu.sHtML

[T38] Lua：条件
来源：http://www.share.fanxiaobao.xyz/Article/details/gzvhrsnrm.sHtML

if x > 0 then print("正") end
来源：http://baike.fanxiaobao.xyz/Article/details/gcdooebev.sHtML

[T39] Lua：模式匹配
来源：http://read.share.fanxiaobao.xyz/Article/details/gnttqkvov.sHtML

string.find(s, "%d+")
来源：http://wap.fanxiaobao.xyz/Article/details/ggzivqixz.sHtML

[T40] Lua：元表
来源：http://wap.fanxiaobao.xyz/Article/details/gklrwqmnk.sHtML

setmetatable({}, { __index = base })
来源：http://blog.fanxiaobao.xyz/Article/details/gfvfcglnz.sHtML

[T41] Perl：Hello World
来源：http://baike.fanxiaobao.xyz/Article/details/gsqtdaube.sHtML

print "Hello\n";
来源：http://baike.fanxiaobao.xyz/Article/details/gmhqppqwo.sHtML

[T42] Perl：变量类型
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gdlbtzadw.sHtML

my $a = 1;  my @arr = (1, 2, 3);  my %h = (a => 1);
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gazmdkpua.sHtML

[T43] Perl：字符串插值
来源：http://www.share.fanxiaobao.xyz/Article/details/gjqrflwhv.sHtML

"值: $a"
来源：http://read.share.fanxiaobao.xyz/Article/details/gsmxslkst.sHtML

[T44] Perl：条件
来源：http://wap.fanxiaobao.xyz/Article/details/gwlnxxzdp.sHtML

if ($a > 0) { print "正"; }
来源：http://m.share.fanxiaobao.xyz/Article/details/gapombybi.sHtML

[T45] Perl：数组遍历
来源：http://baike.fanxiaobao.xyz/Article/details/guqfnmgha.sHtML

for my $x (@arr) { print $x; }
来源：http://blog.fanxiaobao.xyz/Article/details/gxbsfddkd.sHtML

[T46] Perl：哈希操作
来源：http://www.blog.fanxiaobao.xyz/Article/details/gywxjqazz.sHtML

$h{b} = 2;  for my $k (keys %h) { print "$k=$h{$k}"; }
来源：http://read.share.fanxiaobao.xyz/Article/details/gqzayitvq.sHtML

[T47] Perl：正则捕获
来源：http://baike.fanxiaobao.xyz/Article/details/ghfjugnvj.sHtML

if ($s =~ /(\d+)/) { print $1; }
来源：http://www.m.share.fanxiaobao.xyz/Article/details/guqmnpmwy.sHtML

[T48] Perl：正则替换
来源：http://wap.fanxiaobao.xyz/Article/details/gjwezfpxf.sHtML

$s =~ s/old/new/g;
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gehpyvraz.sHtML

[T49] Perl：函数
来源：http://www.blog.fanxiaobao.xyz/Article/details/gmxlzgsiu.sHtML

sub add { my ($a, $b) = @_; return $a + $b; }
来源：http://mobile.fanxiaobao.xyz/Article/details/gitbjfsfm.sHtML

[T50] Perl：逐行读文件
来源：http://www.share.fanxiaobao.xyz/Article/details/gcmikrifn.sHtML

open my $fh, "<", "a.txt" or die $!;
来源：http://wap.fanxiaobao.xyz/Article/details/grhhtjikk.sHtML

while (my $line = <$fh>) { print $line; }
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gzhjuuttn.sHtML

[T51] Scala：Hello World
来源：http://3g.fanxiaobao.xyz/Article/details/grbjlhafq.sHtML

println("Hello")
来源：http://m.share.fanxiaobao.xyz/Article/details/gmoesvkhk.sHtML

[T52] Scala：变量
来源：http://blog.fanxiaobao.xyz/Article/details/gnyjavfal.sHtML

val a = 1;  var b = 2
来源：http://mobile.fanxiaobao.xyz/Article/details/gklngibda.sHtML

[T53] Scala：字符串插值
来源：http://m.share.fanxiaobao.xyz/Article/details/gybtjlyjm.sHtML

s"值: $b"
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gjbbrktyw.sHtML

[T54] Scala：集合映射
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gtljzivbs.sHtML

List(1, 2, 3).map(_ * 2)
来源：http://blog.fanxiaobao.xyz/Article/details/gibakvves.sHtML

[T55] Scala：集合过滤
来源：http://read.share.fanxiaobao.xyz/Article/details/gkzyzfbfd.sHtML

List(1, 2, 3).filter(_ > 1)
来源：http://wap.fanxiaobao.xyz/Article/details/gvomiuncj.sHtML

[T56] Scala：样例类
来源：http://3g.fanxiaobao.xyz/Article/details/gftlnwfhn.sHtML

case class User(name: String, age: Int)
来源：http://blog.fanxiaobao.xyz/Article/details/gxnjpkfvj.sHtML

[T57] Scala：模式匹配
来源：http://baike.fanxiaobao.xyz/Article/details/gzxtqgmza.sHtML

x match { case 1 => "一"; case _ => "其他" }
来源：http://blog.fanxiaobao.xyz/Article/details/gzrazdigm.sHtML

[T58] Scala：函数定义
来源：http://www.blog.fanxiaobao.xyz/Article/details/gpzqanxgg.sHtML

def add(a: Int, b: Int): Int = a + b
来源：http://www.share.fanxiaobao.xyz/Article/details/gmpebfzlz.sHtML

[T59] Scala：循环
来源：http://baike.fanxiaobao.xyz/Article/details/gotuxojgf.sHtML

for (i <- 1 to 10) println(i)
来源：http://wap.fanxiaobao.xyz/Article/details/ggsdypbzs.sHtML

[T60] Scala：折叠
来源：http://mobile.fanxiaobao.xyz/Article/details/gzomdtmyh.sHtML

List(1, 2, 3).foldLeft(0)(_ + _)
来源：http://www.share.fanxiaobao.xyz/Article/details/gznrgngvp.sHtML

================================================================================
来源：http://m.share.fanxiaobao.xyz/Article/details/gfaahjxhq.sHtML

U. 高频实用片段（Python / PHP / JavaScript 各 40 条）
来源：http://mobile.fanxiaobao.xyz/Article/details/grudqtyew.sHtML

================================================================================
来源：http://3g.fanxiaobao.xyz/Article/details/grakbuyqu.sHtML

[U01] Py：创建虚拟环境
来源：http://blog.fanxiaobao.xyz/Article/details/galmddxhl.sHtML

python -m venv .venv && source .venv/bin/activate
来源：http://www.share.fanxiaobao.xyz/Article/details/gkthpxkxb.sHtML

[U02] Py：导出 / 安装依赖
来源：http://wap.fanxiaobao.xyz/Article/details/gehbgjdgq.sHtML

pip freeze > requirements.txt;  pip install -r requirements.txt
来源：http://mobile.fanxiaobao.xyz/Article/details/gburekkoi.sHtML

[U03] Py：加载 .env 配置
来源：http://3g.fanxiaobao.xyz/Article/details/grqtgivib.sHtML

from dotenv import load_dotenv; load_dotenv()
来源：http://www.blog.fanxiaobao.xyz/Article/details/gsbyqqkwr.sHtML

[U04] Py：变量调试打印
来源：http://www.blog.fanxiaobao.xyz/Article/details/ggqmgtvzw.sHtML

print(f"{x=}")            # 输出 x=值，Python 3.8+
来源：http://baike.fanxiaobao.xyz/Article/details/gsvpwpqrj.sHtML

[U05] Py：列表去重且保序
来源：http://read.share.fanxiaobao.xyz/Article/details/gfdbbadls.sHtML

list(dict.fromkeys(arr))
来源：http://mobile.fanxiaobao.xyz/Article/details/ghhdrcgbh.sHtML

[U06] Py：合并两个字典
来源：http://blog.fanxiaobao.xyz/Article/details/gweoddpyx.sHtML

{**a, **b}
来源：http://www.share.fanxiaobao.xyz/Article/details/giwthkakl.sHtML

[U07] Py：反转字典键值
来源：http://baike.fanxiaobao.xyz/Article/details/gtuurlzee.sHtML

{v: k for k, v in d.items()}
来源：http://www.share.fanxiaobao.xyz/Article/details/gwdabnlng.sHtML

[U08] Py：展平二维列表
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gtsutrqed.sHtML

[y for x in nested for y in x]
来源：http://blog.fanxiaobao.xyz/Article/details/gazomxupi.sHtML

[U09] Py：字典取最大值的键
来源：http://www.share.fanxiaobao.xyz/Article/details/gentfygci.sHtML

max(d, key=d.get)
来源：http://blog.fanxiaobao.xyz/Article/details/gbytxxtsm.sHtML

[U10] Py：按值排序字典
来源：http://mobile.fanxiaobao.xyz/Article/details/gsrcvlplz.sHtML

dict(sorted(d.items(), key=lambda kv: kv[1]))
来源：http://baike.fanxiaobao.xyz/Article/details/gjaqjjblr.sHtML

[U11] Py：生成器表达式
来源：http://3g.fanxiaobao.xyz/Article/details/gqlkfimsx.sHtML

(x * 2 for x in arr)
来源：http://www.blog.fanxiaobao.xyz/Article/details/gnuijlkzo.sHtML

[U12] Py：取出现最多的 3 个元素
来源：http://baike.fanxiaobao.xyz/Article/details/gtjgkupnh.sHtML

Counter(arr).most_common(3)
来源：http://blog.fanxiaobao.xyz/Article/details/gzzqncxfm.sHtML

[U13] Py：固定长度队列
来源：http://www.share.fanxiaobao.xyz/Article/details/gfpvtmlcc.sHtML

deque(maxlen=10)
来源：http://3g.fanxiaobao.xyz/Article/details/gtsypzbiq.sHtML

[U14] Py：分组收集到列表
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gtgeywgkl.sHtML

defaultdict(list)
来源：http://m.share.fanxiaobao.xyz/Article/details/gavdfnrly.sHtML


<!-- 参考信息 -->