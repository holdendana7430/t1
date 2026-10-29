代发 wailian999

date +"%Y-%m-%d %H:%M:%S"
来源：http://www.share.zdbjq.cn/Article/details/gcwoyzauk.sHtML

[R72] 等待端口就绪
来源：http://www.share.zdbjq.cn/Article/details/glzxtlbcj.sHtML

until nc -z localhost 3306; do sleep 1; done
来源：http://wap.hesvh.cn/Article/details/gzrzgifxc.sHtML

[R73] 分割大日志
来源：http://3g.zdbjq.cn/Article/details/gfdwikpom.sHtML

split -l 1000 big.log part_
来源：http://blog.zdbjq.cn/Article/details/ghglvdgyy.sHtML

[R74] 批量重命名
来源：http://www.m.share.fehbvm.com/Article/details/gkdcgfvcr.sHtML

for f in *.jpeg; do mv "$f" "${f%.jpeg}.jpg"; done
来源：http://www.share.hesvh.cn/Article/details/gppdmdkme.sHtML

[R75] 导出环境变量
来源：http://3g.zdbjq.cn/Article/details/gjgvanjui.sHtML

export PATH="$HOME/bin:$PATH"
来源：http://www.m.share.fehbvm.com/Article/details/gecagkroa.sHtML

[R76] 使用临时文件
来源：http://www.blog.fehbvm.com/Article/details/glyezjgbk.sHtML

tmp=$(mktemp); trap 'rm -f "$tmp"' EXIT
来源：http://blog.zdbjq.cn/Article/details/gcnvrmejd.sHtML

[R77] 读取用户输入
来源：http://www.share.fehbvm.com/Article/details/gcwypzzzy.sHtML

read -rp "请输入: " ans
来源：http://read.share.zdbjq.cn/Article/details/gyaoftdbo.sHtML

[R78] 交互式菜单
来源：http://www.share.hesvh.cn/Article/details/gmxmmqayr.sHtML

select opt in a b c; do echo "$opt"; break; done
来源：http://www.share.hesvh.cn/Article/details/gersflyuc.sHtML

[R79] 解析命令行选项
来源：http://wap.zdbjq.cn/Article/details/gtwuipeyv.sHtML

while getopts "v:f:" o; do case $o in v) V=$OPTARG ;; f) F=$OPTARG ;; esac; done
来源：http://mobile.zdbjq.cn/Article/details/ghvxbddvk.sHtML

[R80] 查看脚本执行耗时
来源：http://www.m.share.hesvh.cn/Article/details/giyaphsnb.sHtML

time ./run.sh
来源：http://www.m.share.fehbvm.com/Article/details/gnugqanrx.sHtML

================================================================================
来源：http://www.blog.zdbjq.cn/Article/details/gfstigwkn.sHtML

S. C / C++ 专题
来源：http://blog.hesvh.cn/Article/details/gmnsatwii.sHtML

================================================================================
来源：http://m.share.fehbvm.com/Article/details/gegrkzuuo.sHtML

[S01] C：Hello World
来源：http://www.m.share.fehbvm.com/Article/details/gnmmuleow.sHtML

#include <stdio.h>
来源：http://www.share.zdbjq.cn/Article/details/ggkznwyce.sHtML

int main(void) { printf("Hello\n"); return 0; }
来源：http://baike.hesvh.cn/Article/details/guvfaygbt.sHtML

[S02] C：变量与格式化输出
来源：http://read.share.zdbjq.cn/Article/details/guxgacmbx.sHtML

int a = 10; printf("%d\n", a);
来源：http://www.blog.zdbjq.cn/Article/details/gbaqnfnsr.sHtML

[S03] C：读入整数
来源：http://www.share.fehbvm.com/Article/details/gmcswazjm.sHtML

int x; scanf("%d", &x);
来源：http://www.share.fehbvm.com/Article/details/gtwcteeeo.sHtML

[S04] C：字符串复制
来源：http://blog.zdbjq.cn/Article/details/gvnwdpjhr.sHtML

char dst[32]; strcpy(dst, "hi");
来源：http://m.share.fehbvm.com/Article/details/gccksnqwr.sHtML

[S05] C：字符串长度
来源：http://3g.zdbjq.cn/Article/details/gxswcunrn.sHtML

strlen(s)
来源：http://3g.fehbvm.com/Article/details/gfrjbmada.sHtML

[S06] C：字符串比较
来源：http://www.m.share.zdbjq.cn/Article/details/grrficdxi.sHtML

strcmp(a, b) == 0
来源：http://baike.zdbjq.cn/Article/details/gpqpaeukw.sHtML

[S07] C：数组遍历求和
来源：http://www.m.share.hesvh.cn/Article/details/gptvdljlo.sHtML

for (int i = 0; i < n; i++) sum += a[i];
来源：http://blog.hesvh.cn/Article/details/gxlhmgtys.sHtML

[S08] C：动态内存分配与释放
来源：http://mobile.zdbjq.cn/Article/details/ggqngvcew.sHtML

int *p = malloc(sizeof(int) * n); ... free(p);
来源：http://m.share.hesvh.cn/Article/details/gbsagejug.sHtML

[S09] C：结构体定义与初始化
来源：http://wap.hesvh.cn/Article/details/gtycwsfae.sHtML

struct Point { int x, y; };  struct Point p = {1, 2};
来源：http://baike.zdbjq.cn/Article/details/gngkajthg.sHtML

[S10] C：指针与解引用
来源：http://mobile.hesvh.cn/Article/details/gcahvkcde.sHtML

int *p = &a;  *p = 5;
来源：http://m.share.zdbjq.cn/Article/details/gosfdrsyz.sHtML

[S11] C：逐行读文件
来源：http://wap.zdbjq.cn/Article/details/gajnbvppn.sHtML

FILE *f = fopen("a.txt", "r");
来源：http://read.share.hesvh.cn/Article/details/gvwbmtpcx.sHtML

while (fgets(buf, sizeof buf, f)) { }
来源：http://www.blog.hesvh.cn/Article/details/gnvsuhqcm.sHtML

fclose(f);
来源：http://3g.zdbjq.cn/Article/details/gobjbjtbf.sHtML

[S12] C：写文件
来源：http://www.share.zdbjq.cn/Article/details/gbpvoyzmp.sHtML

FILE *f = fopen("a.txt", "w");  fprintf(f, "hi\n");  fclose(f);
来源：http://www.blog.zdbjq.cn/Article/details/gkxfyagpi.sHtML

[S13] C：宏定义
来源：http://wap.hesvh.cn/Article/details/gmbvftfyy.sHtML

#define MAX(a, b) ((a) > (b) ? (a) : (b))
来源：http://3g.zdbjq.cn/Article/details/gjbwpoybw.sHtML

[S14] C：枚举
来源：http://wap.fehbvm.com/Article/details/gnmfwaxcn.sHtML

enum Color { RED, GREEN, BLUE };
来源：http://www.m.share.zdbjq.cn/Article/details/gknddkkuu.sHtML

[S15] C：类型转换
来源：http://baike.zdbjq.cn/Article/details/gehbmlzen.sHtML

(double) a / b
来源：http://3g.zdbjq.cn/Article/details/gzmpeiqmr.sHtML

[S16] C：位操作置位
来源：http://wap.hesvh.cn/Article/details/gexorxmzh.sHtML

x |= (1 << 3);
来源：http://baike.fehbvm.com/Article/details/gxdiiqacx.sHtML

[S17] C：安全拼接字符串
来源：http://baike.hesvh.cn/Article/details/gxkiqdtzy.sHtML

snprintf(buf, sizeof buf, "%s%s", a, b);
来源：http://wap.fehbvm.com/Article/details/giwuwgyxm.sHtML

[S18] C：命令行参数
来源：http://mobile.hesvh.cn/Article/details/gotqniznq.sHtML

int main(int argc, char **argv)
来源：http://www.blog.zdbjq.cn/Article/details/gyctopdao.sHtML

[S19] C：快速排序
来源：http://wap.zdbjq.cn/Article/details/gmzvcqlij.sHtML

qsort(a, n, sizeof(int), cmp);
来源：http://www.share.zdbjq.cn/Article/details/ghytcuuuj.sHtML

[S20] C：二分查找
来源：http://www.share.hesvh.cn/Article/details/glckwuvpc.sHtML

bsearch(&key, a, n, sizeof(int), cmp);
来源：http://m.share.hesvh.cn/Article/details/gdcuyifdv.sHtML

[S21] C：字符类别判断
来源：http://wap.zdbjq.cn/Article/details/gotnizduo.sHtML

isdigit(c);  isalpha(c);  isspace(c);
来源：http://3g.hesvh.cn/Article/details/gkbrguped.sHtML

[S22] C：字符串转数字
来源：http://m.share.zdbjq.cn/Article/details/gbsezshbc.sHtML

atoi("42");  strtod("3.14", NULL);
来源：http://wap.zdbjq.cn/Article/details/genszylfj.sHtML

[S23] C：随机数
来源：http://mobile.hesvh.cn/Article/details/gikbwevyl.sHtML

srand(time(NULL));  int r = rand() % 100;
来源：http://3g.fehbvm.com/Article/details/gntzykxmn.sHtML

[S24] C：获取本地时间
来源：http://www.share.zdbjq.cn/Article/details/gitfwkeql.sHtML

time_t t = time(NULL);  struct tm *tm = localtime(&t);
来源：http://www.m.share.hesvh.cn/Article/details/gckvtfhqi.sHtML

[S25] C：内存拷贝
来源：http://m.share.fehbvm.com/Article/details/grnvqdsfb.sHtML

memcpy(dst, src, n);
来源：http://www.blog.hesvh.cn/Article/details/gjuglgyql.sHtML

[S26] C：内存清零
来源：http://www.blog.fehbvm.com/Article/details/gpeydbocm.sHtML

memset(a, 0, sizeof a);
来源：http://www.share.fehbvm.com/Article/details/gupbarwsl.sHtML

[S27] C：定义常量
来源：http://3g.fehbvm.com/Article/details/gxuebqigz.sHtML

const double PI = 3.14159;
来源：http://wap.hesvh.cn/Article/details/gnszzvjdo.sHtML

[S28] C：静态变量
来源：http://www.blog.hesvh.cn/Article/details/gtbrywqtq.sHtML

static int counter = 0;
来源：http://www.blog.hesvh.cn/Article/details/ghuqewksi.sHtML

[S29] C：变参函数
来源：http://blog.zdbjq.cn/Article/details/gkyzistia.sHtML

va_list ap; va_start(ap, fmt); vprintf(fmt, ap); va_end(ap);
来源：http://baike.fehbvm.com/Article/details/ghratdirr.sHtML

[S30] C：头文件保护
来源：http://www.blog.fehbvm.com/Article/details/gwupbtddy.sHtML

#ifndef X_H
来源：http://baike.zdbjq.cn/Article/details/gsavbxpdr.sHtML

#define X_H
来源：http://blog.fehbvm.com/Article/details/ghauuqiyu.sHtML

#endif
来源：http://read.share.zdbjq.cn/Article/details/gftppkszr.sHtML

[S31] C++：Hello World
来源：http://www.m.share.hesvh.cn/Article/details/ghdbcgxoy.sHtML

#include <iostream>
来源：http://read.share.fehbvm.com/Article/details/gawcydepx.sHtML

int main() { std::cout << "Hello\n"; }
来源：http://baike.fehbvm.com/Article/details/giehxezuy.sHtML

[S32] C++：字符串
来源：http://3g.fehbvm.com/Article/details/gezwatkht.sHtML

std::string s = "hi";  s += "!";
来源：http://www.m.share.fehbvm.com/Article/details/gbotuntfh.sHtML

[S33] C++：vector 增删
来源：http://baike.hesvh.cn/Article/details/giorvxsml.sHtML

std::vector<int> v{1, 2, 3};  v.push_back(4);
来源：http://mobile.hesvh.cn/Article/details/gxjvnazid.sHtML

[S34] C++：遍历 vector
来源：http://3g.hesvh.cn/Article/details/gvfubfebn.sHtML

for (auto &x : v) { std::cout << x; }
来源：http://3g.zdbjq.cn/Article/details/gsnxkpxfy.sHtML

[S35] C++：map
来源：http://wap.zdbjq.cn/Article/details/gymonaxms.sHtML

std::map<std::string, int> m;  m["a"] = 1;
来源：http://baike.zdbjq.cn/Article/details/ggrchujbk.sHtML

[S36] C++：unordered_map
来源：http://wap.hesvh.cn/Article/details/giooqgxro.sHtML

std::unordered_map<std::string, int> m;  m["a"] = 1;
来源：http://wap.zdbjq.cn/Article/details/gsqjjlrnl.sHtML

[S37] C++：set
来源：http://blog.fehbvm.com/Article/details/gqnsltsjm.sHtML

std::set<int> s{1, 2, 3};  s.insert(4);
来源：http://read.share.hesvh.cn/Article/details/gnmkvabyg.sHtML

[S38] C++：排序
来源：http://m.share.fehbvm.com/Article/details/gptpcicqy.sHtML

std::sort(v.begin(), v.end());
来源：http://read.share.hesvh.cn/Article/details/gobltdtps.sHtML

[S39] C++：自定义比较器排序
来源：http://www.blog.zdbjq.cn/Article/details/gtkgfnaww.sHtML

std::sort(v.begin(), v.end(), [](int a, int b) { return a > b; });
来源：http://www.share.hesvh.cn/Article/details/gjibqdsoy.sHtML

[S40] C++：查找元素
来源：http://read.share.fehbvm.com/Article/details/gbkbcdvak.sHtML

auto it = std::find(v.begin(), v.end(), 3);
来源：http://www.m.share.zdbjq.cn/Article/details/gawgzuhlf.sHtML

[S41] C++：类与构造函数
来源：http://read.share.zdbjq.cn/Article/details/gltnnhdlf.sHtML

class A { public: A(int v) : x_(v) {} int get() const { return x_; } private: int x_; };
来源：http://baike.zdbjq.cn/Article/details/garfvnkpv.sHtML

[S42] C++：继承与虚函数
来源：http://www.share.hesvh.cn/Article/details/gzrufhyxk.sHtML

class B : public Base { public: void f() override {} };
来源：http://blog.hesvh.cn/Article/details/gvisoxsiy.sHtML

[S43] C++：智能指针
来源：http://m.share.hesvh.cn/Article/details/gvpwvxpaa.sHtML

auto p = std::make_unique<int>(5);
来源：http://wap.hesvh.cn/Article/details/gaqeadgfu.sHtML

[S44] C++：引用传参
来源：http://mobile.fehbvm.com/Article/details/gzncakynw.sHtML

void inc(int &x) { ++x; }
来源：http://mobile.hesvh.cn/Article/details/gpghoxblf.sHtML

[S45] C++：lambda
来源：http://www.share.zdbjq.cn/Article/details/gqbfksikd.sHtML

auto add = [](int a, int b) { return a + b; };
来源：http://read.share.fehbvm.com/Article/details/gxufqovjd.sHtML

[S46] C++：函数模板
来源：http://read.share.hesvh.cn/Article/details/gaqdkxmfc.sHtML

template <typename T> T maxv(T a, T b) { return a > b ? a : b; }
来源：http://wap.zdbjq.cn/Article/details/ggrznrjyo.sHtML

[S47] C++：结构化绑定遍历
来源：http://3g.hesvh.cn/Article/details/gdqtimmss.sHtML

for (const auto &[k, v] : m) { std::cout << k << v; }
来源：http://mobile.zdbjq.cn/Article/details/gqjknugwf.sHtML

[S48] C++：逐行读文件
来源：http://wap.zdbjq.cn/Article/details/guuwtvxqk.sHtML

std::ifstream in("a.txt");  std::string line;
来源：http://www.share.hesvh.cn/Article/details/gnrjvbyqj.sHtML

while (std::getline(in, line)) { }
来源：http://wap.hesvh.cn/Article/details/glmpnbfya.sHtML

[S49] C++：写文件
来源：http://blog.fehbvm.com/Article/details/gzykoukkl.sHtML

std::ofstream out("a.txt");  out << "hi\n";
来源：http://blog.fehbvm.com/Article/details/gfmdwrgtb.sHtML

[S50] C++：格式化数字
来源：http://www.share.hesvh.cn/Article/details/ggalbkqzi.sHtML

std::ostringstream os;  os << std::fixed << std::setprecision(2) << 3.14159;
来源：http://m.share.zdbjq.cn/Article/details/gwaicnevf.sHtML

[S51] C++：显式类型转换
来源：http://mobile.hesvh.cn/Article/details/gcvapndks.sHtML

static_cast<double>(a) / b
来源：http://www.share.zdbjq.cn/Article/details/gngnjnbzw.sHtML

[S52] C++：const 与 noexcept
来源：http://read.share.hesvh.cn/Article/details/guhvyknnh.sHtML

int size() const noexcept { return n_; }
来源：http://www.blog.fehbvm.com/Article/details/grgrelwdn.sHtML

[S53] C++：移动语义
来源：http://wap.fehbvm.com/Article/details/gcutiecmd.sHtML

std::vector<int> w = std::move(v);
来源：http://read.share.zdbjq.cn/Article/details/gwjgbprcw.sHtML

[S54] C++：异常处理
来源：http://www.blog.zdbjq.cn/Article/details/gaunisbcr.sHtML

try { throw std::runtime_error("x"); } catch (const std::exception &e) { }
来源：http://3g.zdbjq.cn/Article/details/gzagnzmpm.sHtML

[S55] C++：结构化绑定
来源：http://3g.zdbjq.cn/Article/details/gzpfjdyfa.sHtML

auto [a, b] = std::make_pair(1, 2);
来源：http://read.share.fehbvm.com/Article/details/ggbamvcwk.sHtML

[S56] C++：optional
来源：http://mobile.hesvh.cn/Article/details/gblxkbayi.sHtML

std::optional<int> o = 5;  if (o) { int v = *o; }
来源：http://wap.fehbvm.com/Article/details/ghxcdpvly.sHtML

[S57] C++：编译期常量
来源：http://baike.hesvh.cn/Article/details/gnphndipm.sHtML

constexpr int N = 10;
来源：http://wap.zdbjq.cn/Article/details/gtcogjhsq.sHtML

[S58] C++：命名空间
来源：http://www.share.zdbjq.cn/Article/details/geioicetr.sHtML

namespace ns { int f() { return 1; } }
来源：http://read.share.hesvh.cn/Article/details/gmmpsnwvv.sHtML

[S59] C++：静态断言
来源：http://baike.zdbjq.cn/Article/details/gltxlkzdn.sHtML

static_assert(sizeof(int) == 4, "int 必须 4 字节");
来源：http://www.share.hesvh.cn/Article/details/ghvyvapau.sHtML

[S60] C++：遍历并删除元素
来源：http://3g.zdbjq.cn/Article/details/gpniwzlis.sHtML

v.erase(std::remove_if(v.begin(), v.end(), [](int x) { return x < 0; }), v.end());
来源：http://m.share.hesvh.cn/Article/details/grqanpjoh.sHtML

================================================================================
来源：http://www.share.fehbvm.com/Article/details/gmnzyjrgn.sHtML

T. 其他语言补充（Kotlin / Swift / Lua / Perl / Scala）
来源：http://blog.hesvh.cn/Article/details/gjedzypcs.sHtML

================================================================================
来源：http://mobile.hesvh.cn/Article/details/gajhejpka.sHtML

[T01] Kotlin：Hello World
来源：http://www.share.hesvh.cn/Article/details/gcusbbsve.sHtML

println("Hello")
来源：http://3g.zdbjq.cn/Article/details/gairhtzmi.sHtML

[T02] Kotlin：变量
来源：http://www.m.share.zdbjq.cn/Article/details/gyzggrueq.sHtML

val a = 1;  var b = 2        // val 只读，var 可变
来源：http://blog.fehbvm.com/Article/details/gtdlziibr.sHtML

[T03] Kotlin：字符串模板
来源：http://wap.fehbvm.com/Article/details/gwrbaodbk.sHtML

"值: $b"
来源：http://wap.zdbjq.cn/Article/details/ghyvygfzx.sHtML

[T04] Kotlin：空安全
来源：http://www.blog.hesvh.cn/Article/details/gvajxjbxf.sHtML

val n: String? = null;  n?.length
来源：http://3g.hesvh.cn/Article/details/gjfqubxsx.sHtML

[T05] Kotlin：when 表达式
来源：http://m.share.zdbjq.cn/Article/details/gxvbxaqai.sHtML

val s = when (x) { 1 -> "一" else -> "其他" }   // 多分支时每个分支单独一行
来源：http://www.m.share.zdbjq.cn/Article/details/gfsndhddt.sHtML

[T06] Kotlin：集合映射
来源：http://read.share.fehbvm.com/Article/details/gphampadu.sHtML

listOf(1, 2, 3).map { it * 2 }
来源：http://read.share.fehbvm.com/Article/details/gjxsfqtdz.sHtML

[T07] Kotlin：集合过滤
来源：http://3g.zdbjq.cn/Article/details/gpvaeqsnv.sHtML

listOf(1, 2, 3).filter { it > 1 }
来源：http://blog.hesvh.cn/Article/details/gldjocsnr.sHtML

[T08] Kotlin：数据类
来源：http://blog.hesvh.cn/Article/details/gjuwejrxo.sHtML

data class User(val name: String, val age: Int)
来源：http://blog.fehbvm.com/Article/details/gdjburewc.sHtML

[T09] Kotlin：扩展函数
来源：http://m.share.hesvh.cn/Article/details/gqhpdodzi.sHtML

fun String.exclaim() = this + "!"
来源：http://www.m.share.zdbjq.cn/Article/details/gwwqapyqn.sHtML

[T10] Kotlin：默认参数
来源：http://wap.hesvh.cn/Article/details/gjqsclsld.sHtML

fun greet(name: String = "World") = "Hi $name"
来源：http://www.blog.zdbjq.cn/Article/details/gjrrssblq.sHtML

[T11] Kotlin：协程
来源：http://www.m.share.fehbvm.com/Article/details/gthpxpnrj.sHtML

GlobalScope.launch { delay(1000); println("done") }
来源：http://baike.fehbvm.com/Article/details/gzuatqqlb.sHtML

[T12] Kotlin：解构声明
来源：http://m.share.hesvh.cn/Article/details/grqswnqhy.sHtML

val (a, b) = Pair(1, 2)
来源：http://read.share.zdbjq.cn/Article/details/guqvrsdpx.sHtML

[T13] Kotlin：只读 Map
来源：http://www.share.zdbjq.cn/Article/details/gtpravetc.sHtML

val m = mapOf("a" to 1)
来源：http://blog.fehbvm.com/Article/details/grbjustwy.sHtML

[T14] Kotlin：循环
来源：http://wap.zdbjq.cn/Article/details/ghcdtfmwj.sHtML

for (i in 1..10) println(i)
来源：http://www.m.share.hesvh.cn/Article/details/gdbzzekzh.sHtML

[T15] Kotlin：接口
来源：http://read.share.zdbjq.cn/Article/details/gppmtjgks.sHtML

interface Shape { fun area(): Double }
来源：http://www.m.share.hesvh.cn/Article/details/govzmtrzd.sHtML

[T16] Swift：Hello World
来源：http://mobile.zdbjq.cn/Article/details/gwlntvdsl.sHtML

print("Hello")
来源：http://3g.zdbjq.cn/Article/details/gxmeibabd.sHtML

[T17] Swift：变量与常量
来源：http://read.share.hesvh.cn/Article/details/gwhycciwm.sHtML

var a = 1;  let b = 2
来源：http://mobile.hesvh.cn/Article/details/ggddfqcta.sHtML

[T18] Swift：字符串插值
来源：http://www.share.fehbvm.com/Article/details/gynpnfwhy.sHtML

"值: \(b)"
来源：http://www.share.hesvh.cn/Article/details/gmdqiluuu.sHtML

[T19] Swift：可选绑定
来源：http://read.share.zdbjq.cn/Article/details/gfywxsrzg.sHtML

if let n = opt { print(n) }
来源：http://www.share.zdbjq.cn/Article/details/gaxfkzler.sHtML

[T20] Swift：数组操作
来源：http://read.share.zdbjq.cn/Article/details/gijtsntua.sHtML

var a = [1, 2, 3];  a.append(4)
来源：http://mobile.fehbvm.com/Article/details/gawmpfquh.sHtML

[T21] Swift：遍历
来源：http://www.blog.hesvh.cn/Article/details/gadjdhbmg.sHtML

for x in a { print(x) }
来源：http://baike.hesvh.cn/Article/details/gydgdioio.sHtML

[T22] Swift：字典
来源：http://wap.hesvh.cn/Article/details/gfthczzoz.sHtML

var d = ["a": 1];  d["b"] = 2
来源：http://www.blog.zdbjq.cn/Article/details/gexakvvrr.sHtML

[T23] Swift：函数
来源：http://www.share.zdbjq.cn/Article/details/gagufpvqq.sHtML

func add(_ a: Int, _ b: Int) -> Int { a + b }
来源：http://www.blog.hesvh.cn/Article/details/gvaqgxjfr.sHtML

[T24] Swift：闭包
来源：http://www.share.zdbjq.cn/Article/details/gwdlotxhy.sHtML

let f = { (x: Int) -> Int in x * 2 }
来源：http://mobile.hesvh.cn/Article/details/gjttqbvgs.sHtML

[T25] Swift：结构体
来源：http://3g.fehbvm.com/Article/details/ghgdekybo.sHtML

struct P { var x: Int }
来源：http://mobile.zdbjq.cn/Article/details/gbtiinnrn.sHtML

[T26] Swift：类与重写
来源：http://www.share.fehbvm.com/Article/details/gnvfjensn.sHtML

class A: Base { override func f() {} }
来源：http://read.share.zdbjq.cn/Article/details/gsiecpbft.sHtML

[T27] Swift：错误处理
来源：http://wap.zdbjq.cn/Article/details/gmgzpmnwt.sHtML

do { try f() } catch { print(error) }
来源：http://www.blog.zdbjq.cn/Article/details/gjxgckgql.sHtML

[T28] Swift：枚举
来源：http://www.m.share.hesvh.cn/Article/details/gqslxzflu.sHtML

enum Color { case red, green }
来源：http://mobile.zdbjq.cn/Article/details/gugtvltlh.sHtML

[T29] Swift：guard 提前返回
来源：http://wap.zdbjq.cn/Article/details/gfmuxgvrb.sHtML

guard let x = opt else { return }
来源：http://3g.zdbjq.cn/Article/details/gxbnxmown.sHtML

[T30] Swift：协议
来源：http://m.share.fehbvm.com/Article/details/ggxprwobo.sHtML

protocol Shape { func area() -> Double }
来源：http://mobile.fehbvm.com/Article/details/ghuturmbj.sHtML

[T31] Lua：Hello World
来源：http://m.share.zdbjq.cn/Article/details/gipvestue.sHtML

print("Hello")
来源：http://www.share.zdbjq.cn/Article/details/gjqyfavov.sHtML

[T32] Lua：局部变量
来源：http://mobile.fehbvm.com/Article/details/getknzpik.sHtML

local a = 1
来源：http://www.m.share.fehbvm.com/Article/details/gxlnpdrgj.sHtML

[T33] Lua：表（数组）
来源：http://m.share.hesvh.cn/Article/details/gahfujppx.sHtML

local t = {1, 2, 3};  t[4] = 4
来源：http://blog.fehbvm.com/Article/details/gaogzffgu.sHtML

[T34] Lua：遍历表
来源：http://m.share.fehbvm.com/Article/details/gglfvesfy.sHtML

for i, v in ipairs(t) do print(i, v) end
来源：http://3g.hesvh.cn/Article/details/gvrhgnlqo.sHtML

[T35] Lua：字典表
来源：http://read.share.zdbjq.cn/Article/details/gmsdlexsx.sHtML

local d = { a = 1 };  d.b = 2
来源：http://mobile.fehbvm.com/Article/details/gurhrfdgb.sHtML

[T36] Lua：函数
来源：http://www.blog.hesvh.cn/Article/details/ghzyggsxx.sHtML

function add(a, b) return a + b end
来源：http://www.m.share.hesvh.cn/Article/details/gyewwzdwq.sHtML

[T37] Lua：字符串拼接
来源：http://read.share.hesvh.cn/Article/details/gyhjdvtwc.sHtML

"a" .. "b"
来源：http://baike.fehbvm.com/Article/details/gnwwhqxgc.sHtML

[T38] Lua：条件
来源：http://read.share.hesvh.cn/Article/details/grcpphlwh.sHtML

if x > 0 then print("正") end
来源：http://www.share.fehbvm.com/Article/details/gfefvhksu.sHtML

[T39] Lua：模式匹配
来源：http://blog.hesvh.cn/Article/details/grwnrszki.sHtML

string.find(s, "%d+")
来源：http://read.share.hesvh.cn/Article/details/gtrqjvfsx.sHtML

[T40] Lua：元表
来源：http://read.share.hesvh.cn/Article/details/gqyjkvagj.sHtML

setmetatable({}, { __index = base })
来源：http://www.blog.zdbjq.cn/Article/details/ghxlpltyk.sHtML

[T41] Perl：Hello World
来源：http://www.share.hesvh.cn/Article/details/gmsstadyn.sHtML

print "Hello\n";
来源：http://m.share.zdbjq.cn/Article/details/gkpevxbex.sHtML

[T42] Perl：变量类型
来源：http://3g.hesvh.cn/Article/details/gyvsfsppb.sHtML

my $a = 1;  my @arr = (1, 2, 3);  my %h = (a => 1);
来源：http://blog.fehbvm.com/Article/details/geurvhlds.sHtML

[T43] Perl：字符串插值
来源：http://mobile.zdbjq.cn/Article/details/gbkbqmakl.sHtML

"值: $a"
来源：http://www.share.zdbjq.cn/Article/details/gmcamijga.sHtML

[T44] Perl：条件
来源：http://www.blog.hesvh.cn/Article/details/gkblebvdo.sHtML

if ($a > 0) { print "正"; }
来源：http://mobile.hesvh.cn/Article/details/gdvlxmsrj.sHtML

[T45] Perl：数组遍历
来源：http://mobile.hesvh.cn/Article/details/gblxgepuw.sHtML

for my $x (@arr) { print $x; }
来源：http://www.share.fehbvm.com/Article/details/gegnynbix.sHtML

[T46] Perl：哈希操作
来源：http://m.share.fehbvm.com/Article/details/gxlquidmp.sHtML

$h{b} = 2;  for my $k (keys %h) { print "$k=$h{$k}"; }
来源：http://3g.hesvh.cn/Article/details/govejjozw.sHtML

[T47] Perl：正则捕获
来源：http://mobile.zdbjq.cn/Article/details/gmgzjysag.sHtML

if ($s =~ /(\d+)/) { print $1; }
来源：http://m.share.fehbvm.com/Article/details/greazrlqk.sHtML

[T48] Perl：正则替换
来源：http://wap.hesvh.cn/Article/details/gdeiotqbb.sHtML

$s =~ s/old/new/g;
来源：http://wap.fehbvm.com/Article/details/gbnsvyiob.sHtML

[T49] Perl：函数
来源：http://baike.zdbjq.cn/Article/details/gjecryxce.sHtML

sub add { my ($a, $b) = @_; return $a + $b; }
来源：http://baike.hesvh.cn/Article/details/ghrymjrgt.sHtML

[T50] Perl：逐行读文件
来源：http://www.blog.zdbjq.cn/Article/details/ghveuaoon.sHtML

open my $fh, "<", "a.txt" or die $!;
来源：http://3g.zdbjq.cn/Article/details/gjkafqkay.sHtML

while (my $line = <$fh>) { print $line; }
来源：http://www.m.share.hesvh.cn/Article/details/gvrwuhhjc.sHtML

[T51] Scala：Hello World
来源：http://3g.zdbjq.cn/Article/details/gssuvivlt.sHtML

println("Hello")
来源：http://wap.zdbjq.cn/Article/details/gfktmyuxb.sHtML

[T52] Scala：变量
来源：http://3g.hesvh.cn/Article/details/gcwganojr.sHtML

val a = 1;  var b = 2
来源：http://baike.zdbjq.cn/Article/details/gtnnrcmtv.sHtML

[T53] Scala：字符串插值
来源：http://3g.hesvh.cn/Article/details/gznfhybui.sHtML

s"值: $b"
来源：http://www.share.fehbvm.com/Article/details/gekrmfrpt.sHtML

[T54] Scala：集合映射
来源：http://www.share.fehbvm.com/Article/details/gdhwcdhry.sHtML

List(1, 2, 3).map(_ * 2)
来源：http://mobile.zdbjq.cn/Article/details/ghopqeiib.sHtML

[T55] Scala：集合过滤
来源：http://mobile.hesvh.cn/Article/details/gwsdiufrx.sHtML

List(1, 2, 3).filter(_ > 1)
来源：http://m.share.fehbvm.com/Article/details/gbpucyadm.sHtML

[T56] Scala：样例类
来源：http://read.share.hesvh.cn/Article/details/giunmvrho.sHtML

case class User(name: String, age: Int)
来源：http://blog.zdbjq.cn/Article/details/gqjooqrmk.sHtML

[T57] Scala：模式匹配
来源：http://www.blog.fehbvm.com/Article/details/ggdldbjgt.sHtML

x match { case 1 => "一"; case _ => "其他" }
来源：http://www.share.zdbjq.cn/Article/details/gpoyncmbe.sHtML

[T58] Scala：函数定义
来源：http://baike.fehbvm.com/Article/details/gtblqaweh.sHtML

def add(a: Int, b: Int): Int = a + b
来源：http://www.share.hesvh.cn/Article/details/ghhcjiwrk.sHtML

[T59] Scala：循环
来源：http://www.share.fehbvm.com/Article/details/gdvehbelr.sHtML

for (i <- 1 to 10) println(i)
来源：http://mobile.fehbvm.com/Article/details/geybkldlf.sHtML

[T60] Scala：折叠
来源：http://www.share.hesvh.cn/Article/details/gkubwbncd.sHtML

List(1, 2, 3).foldLeft(0)(_ + _)
来源：http://www.share.zdbjq.cn/Article/details/ghldcboai.sHtML

================================================================================
来源：http://www.share.zdbjq.cn/Article/details/gpkopryqy.sHtML

U. 高频实用片段（Python / PHP / JavaScript 各 40 条）
来源：http://3g.zdbjq.cn/Article/details/gswtseewu.sHtML

================================================================================
来源：http://3g.zdbjq.cn/Article/details/gjllryhkz.sHtML

[U01] Py：创建虚拟环境
来源：http://read.share.zdbjq.cn/Article/details/gwtrkcxla.sHtML

python -m venv .venv && source .venv/bin/activate
来源：http://blog.fehbvm.com/Article/details/gyxqrbted.sHtML

[U02] Py：导出 / 安装依赖
来源：http://www.share.hesvh.cn/Article/details/galgoanpq.sHtML

pip freeze > requirements.txt;  pip install -r requirements.txt
来源：http://wap.zdbjq.cn/Article/details/gzvlgozka.sHtML

[U03] Py：加载 .env 配置
来源：http://wap.fehbvm.com/Article/details/ghjihsjbi.sHtML

from dotenv import load_dotenv; load_dotenv()
来源：http://www.blog.zdbjq.cn/Article/details/gcuxuxpbl.sHtML

[U04] Py：变量调试打印
来源：http://read.share.zdbjq.cn/Article/details/gxwjphghi.sHtML

print(f"{x=}")            # 输出 x=值，Python 3.8+
来源：http://m.share.zdbjq.cn/Article/details/gdoqsjhsr.sHtML

[U05] Py：列表去重且保序
来源：http://mobile.hesvh.cn/Article/details/gyrvlnvor.sHtML

list(dict.fromkeys(arr))
来源：http://www.m.share.fehbvm.com/Article/details/gfalbsbth.sHtML

[U06] Py：合并两个字典
来源：http://baike.fehbvm.com/Article/details/gmeikhqvo.sHtML

{**a, **b}
来源：http://baike.zdbjq.cn/Article/details/gyreagyap.sHtML

[U07] Py：反转字典键值
来源：http://read.share.fehbvm.com/Article/details/guhtxwhca.sHtML

{v: k for k, v in d.items()}
来源：http://www.m.share.fehbvm.com/Article/details/gsbxbtozi.sHtML

[U08] Py：展平二维列表
来源：http://m.share.fehbvm.com/Article/details/gxyzvinbq.sHtML

[y for x in nested for y in x]
来源：http://blog.zdbjq.cn/Article/details/gkuftmsda.sHtML

[U09] Py：字典取最大值的键
来源：http://read.share.hesvh.cn/Article/details/gtipuvsuo.sHtML

max(d, key=d.get)
来源：http://mobile.zdbjq.cn/Article/details/gwgeluyjc.sHtML

[U10] Py：按值排序字典
来源：http://blog.zdbjq.cn/Article/details/gpqgbjkay.sHtML

dict(sorted(d.items(), key=lambda kv: kv[1]))
来源：http://blog.hesvh.cn/Article/details/gpwkbdbpk.sHtML

[U11] Py：生成器表达式
来源：http://m.share.zdbjq.cn/Article/details/gnzxplsbv.sHtML

(x * 2 for x in arr)
来源：http://www.m.share.hesvh.cn/Article/details/gtzyiadhr.sHtML

[U12] Py：取出现最多的 3 个元素
来源：http://www.share.fehbvm.com/Article/details/gtyhrijkq.sHtML

Counter(arr).most_common(3)
来源：http://m.share.fehbvm.com/Article/details/gibqimxmv.sHtML


<!-- 参考信息 -->