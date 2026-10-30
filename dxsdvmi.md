代发 wailian999

date +"%Y-%m-%d %H:%M:%S"
来源：http://mobile.hesvh.cn/Article/details/gwlslzhwt.sHtML

[R72] 等待端口就绪
来源：http://read.share.hesvh.cn/Article/details/gzfvwvgbt.sHtML

until nc -z localhost 3306; do sleep 1; done
来源：http://www.share.fehbvm.com/Article/details/gfysqvyyi.sHtML

[R73] 分割大日志
来源：http://read.share.fehbvm.com/Article/details/gfhjupekn.sHtML

split -l 1000 big.log part_
来源：http://wap.zdbjq.cn/Article/details/gzrgabgyw.sHtML

[R74] 批量重命名
来源：http://3g.hesvh.cn/Article/details/gytjblgxe.sHtML

for f in *.jpeg; do mv "$f" "${f%.jpeg}.jpg"; done
来源：http://read.share.fehbvm.com/Article/details/giqnnpvzy.sHtML

[R75] 导出环境变量
来源：http://www.m.share.hesvh.cn/Article/details/gawqvimcs.sHtML

export PATH="$HOME/bin:$PATH"
来源：http://www.m.share.zdbjq.cn/Article/details/gspdqbmtz.sHtML

[R76] 使用临时文件
来源：http://3g.hesvh.cn/Article/details/gfhpykhwr.sHtML

tmp=$(mktemp); trap 'rm -f "$tmp"' EXIT
来源：http://baike.hesvh.cn/Article/details/govkukwhy.sHtML

[R77] 读取用户输入
来源：http://www.m.share.fehbvm.com/Article/details/ghgigoimn.sHtML

read -rp "请输入: " ans
来源：http://www.blog.hesvh.cn/Article/details/gppkqbwxx.sHtML

[R78] 交互式菜单
来源：http://baike.zdbjq.cn/Article/details/gxnrivrqo.sHtML

select opt in a b c; do echo "$opt"; break; done
来源：http://www.m.share.hesvh.cn/Article/details/ganhwdwmv.sHtML

[R79] 解析命令行选项
来源：http://3g.hesvh.cn/Article/details/gmwabdnxy.sHtML

while getopts "v:f:" o; do case $o in v) V=$OPTARG ;; f) F=$OPTARG ;; esac; done
来源：http://3g.fehbvm.com/Article/details/gxoxtxcav.sHtML

[R80] 查看脚本执行耗时
来源：http://www.blog.fehbvm.com/Article/details/glgfsqzdu.sHtML

time ./run.sh
来源：http://m.share.hesvh.cn/Article/details/gtnezyrpn.sHtML

================================================================================
来源：http://3g.zdbjq.cn/Article/details/gsbsqrpbb.sHtML

S. C / C++ 专题
来源：http://3g.hesvh.cn/Article/details/guccasyjx.sHtML

================================================================================
来源：http://www.share.hesvh.cn/Article/details/gycgkfwdu.sHtML

[S01] C：Hello World
来源：http://wap.zdbjq.cn/Article/details/gdkxtagsj.sHtML

#include <stdio.h>
来源：http://wap.zdbjq.cn/Article/details/gdhzewzxj.sHtML

int main(void) { printf("Hello\n"); return 0; }
来源：http://read.share.fehbvm.com/Article/details/gncrcpyqt.sHtML

[S02] C：变量与格式化输出
来源：http://read.share.zdbjq.cn/Article/details/gcxamjcqd.sHtML

int a = 10; printf("%d\n", a);
来源：http://mobile.fehbvm.com/Article/details/gzhwgqgap.sHtML

[S03] C：读入整数
来源：http://www.share.fehbvm.com/Article/details/gomopouhi.sHtML

int x; scanf("%d", &x);
来源：http://blog.zdbjq.cn/Article/details/gsyaefrbh.sHtML

[S04] C：字符串复制
来源：http://www.blog.fehbvm.com/Article/details/gyubesnnj.sHtML

char dst[32]; strcpy(dst, "hi");
来源：http://3g.zdbjq.cn/Article/details/gwjldsytt.sHtML

[S05] C：字符串长度
来源：http://3g.hesvh.cn/Article/details/grdjdvxow.sHtML

strlen(s)
来源：http://www.share.fehbvm.com/Article/details/glqdhugru.sHtML

[S06] C：字符串比较
来源：http://www.m.share.fehbvm.com/Article/details/ghwrqqyeg.sHtML

strcmp(a, b) == 0
来源：http://www.blog.zdbjq.cn/Article/details/gjvawcdwy.sHtML

[S07] C：数组遍历求和
来源：http://wap.zdbjq.cn/Article/details/gqlxuqmfs.sHtML

for (int i = 0; i < n; i++) sum += a[i];
来源：http://www.share.hesvh.cn/Article/details/gwffpugqu.sHtML

[S08] C：动态内存分配与释放
来源：http://www.blog.hesvh.cn/Article/details/gcdzfmvhv.sHtML

int *p = malloc(sizeof(int) * n); ... free(p);
来源：http://3g.hesvh.cn/Article/details/gngknziom.sHtML

[S09] C：结构体定义与初始化
来源：http://3g.zdbjq.cn/Article/details/gucztwysv.sHtML

struct Point { int x, y; };  struct Point p = {1, 2};
来源：http://mobile.fehbvm.com/Article/details/gmgekvwiw.sHtML

[S10] C：指针与解引用
来源：http://wap.hesvh.cn/Article/details/gjebrvljs.sHtML

int *p = &a;  *p = 5;
来源：http://wap.zdbjq.cn/Article/details/gwbwpjbtv.sHtML

[S11] C：逐行读文件
来源：http://wap.hesvh.cn/Article/details/gaktezcoa.sHtML

FILE *f = fopen("a.txt", "r");
来源：http://m.share.hesvh.cn/Article/details/gdorangol.sHtML

while (fgets(buf, sizeof buf, f)) { }
来源：http://www.m.share.fehbvm.com/Article/details/gmgebuikq.sHtML

fclose(f);
来源：http://wap.fehbvm.com/Article/details/gtpbycnzn.sHtML

[S12] C：写文件
来源：http://3g.zdbjq.cn/Article/details/gzgljhrxf.sHtML

FILE *f = fopen("a.txt", "w");  fprintf(f, "hi\n");  fclose(f);
来源：http://m.share.fehbvm.com/Article/details/gggliblzk.sHtML

[S13] C：宏定义
来源：http://www.share.fehbvm.com/Article/details/gpdbrvnal.sHtML

#define MAX(a, b) ((a) > (b) ? (a) : (b))
来源：http://www.blog.zdbjq.cn/Article/details/gdvbzgdmt.sHtML

[S14] C：枚举
来源：http://3g.zdbjq.cn/Article/details/genmsfjfk.sHtML

enum Color { RED, GREEN, BLUE };
来源：http://www.m.share.hesvh.cn/Article/details/gzfmfnzzk.sHtML

[S15] C：类型转换
来源：http://blog.hesvh.cn/Article/details/gjlcmflml.sHtML

(double) a / b
来源：http://www.m.share.zdbjq.cn/Article/details/gsfrruspx.sHtML

[S16] C：位操作置位
来源：http://www.m.share.hesvh.cn/Article/details/gktteowfz.sHtML

x |= (1 << 3);
来源：http://read.share.fehbvm.com/Article/details/gjcclfazy.sHtML

[S17] C：安全拼接字符串
来源：http://wap.zdbjq.cn/Article/details/gunumqirt.sHtML

snprintf(buf, sizeof buf, "%s%s", a, b);
来源：http://read.share.hesvh.cn/Article/details/gopaheqse.sHtML

[S18] C：命令行参数
来源：http://www.blog.fehbvm.com/Article/details/getnwivpt.sHtML

int main(int argc, char **argv)
来源：http://read.share.fehbvm.com/Article/details/glbviyutl.sHtML

[S19] C：快速排序
来源：http://mobile.fehbvm.com/Article/details/gtbwjvkaq.sHtML

qsort(a, n, sizeof(int), cmp);
来源：http://mobile.hesvh.cn/Article/details/gtyteotnn.sHtML

[S20] C：二分查找
来源：http://blog.zdbjq.cn/Article/details/gnpezeylz.sHtML

bsearch(&key, a, n, sizeof(int), cmp);
来源：http://m.share.zdbjq.cn/Article/details/gkfusuraj.sHtML

[S21] C：字符类别判断
来源：http://www.share.zdbjq.cn/Article/details/gukridblj.sHtML

isdigit(c);  isalpha(c);  isspace(c);
来源：http://mobile.hesvh.cn/Article/details/gaamchzee.sHtML

[S22] C：字符串转数字
来源：http://blog.zdbjq.cn/Article/details/glkaikyfs.sHtML

atoi("42");  strtod("3.14", NULL);
来源：http://www.m.share.zdbjq.cn/Article/details/ggsvkgegz.sHtML

[S23] C：随机数
来源：http://read.share.hesvh.cn/Article/details/gbfmeaqth.sHtML

srand(time(NULL));  int r = rand() % 100;
来源：http://www.blog.hesvh.cn/Article/details/gwdvsoejz.sHtML

[S24] C：获取本地时间
来源：http://3g.hesvh.cn/Article/details/grfxqgkci.sHtML

time_t t = time(NULL);  struct tm *tm = localtime(&t);
来源：http://baike.fehbvm.com/Article/details/grufsfhvp.sHtML

[S25] C：内存拷贝
来源：http://www.blog.fehbvm.com/Article/details/gefpgpatd.sHtML

memcpy(dst, src, n);
来源：http://www.share.zdbjq.cn/Article/details/ganwqupwb.sHtML

[S26] C：内存清零
来源：http://www.share.fehbvm.com/Article/details/gpwzcerre.sHtML

memset(a, 0, sizeof a);
来源：http://www.m.share.fehbvm.com/Article/details/gxfxcefvy.sHtML

[S27] C：定义常量
来源：http://read.share.zdbjq.cn/Article/details/guxaxdujf.sHtML

const double PI = 3.14159;
来源：http://www.share.hesvh.cn/Article/details/ggdlgywqa.sHtML

[S28] C：静态变量
来源：http://www.blog.zdbjq.cn/Article/details/gypnmqpoa.sHtML

static int counter = 0;
来源：http://mobile.zdbjq.cn/Article/details/gajgusmlh.sHtML

[S29] C：变参函数
来源：http://wap.fehbvm.com/Article/details/gfktxhcgl.sHtML

va_list ap; va_start(ap, fmt); vprintf(fmt, ap); va_end(ap);
来源：http://m.share.fehbvm.com/Article/details/gogeqapvl.sHtML

[S30] C：头文件保护
来源：http://www.share.fehbvm.com/Article/details/gavnomxzo.sHtML

#ifndef X_H
来源：http://www.share.zdbjq.cn/Article/details/gflzxmpkj.sHtML

#define X_H
来源：http://blog.fehbvm.com/Article/details/gcupjpcin.sHtML

#endif
来源：http://baike.zdbjq.cn/Article/details/gkdgajpzf.sHtML

[S31] C++：Hello World
来源：http://www.share.hesvh.cn/Article/details/gxtptarek.sHtML

#include <iostream>
来源：http://mobile.hesvh.cn/Article/details/gioofrsxq.sHtML

int main() { std::cout << "Hello\n"; }
来源：http://www.m.share.hesvh.cn/Article/details/gjxzmwtxh.sHtML

[S32] C++：字符串
来源：http://3g.fehbvm.com/Article/details/gwaivhtmh.sHtML

std::string s = "hi";  s += "!";
来源：http://www.share.fehbvm.com/Article/details/gnkqihzvs.sHtML

[S33] C++：vector 增删
来源：http://mobile.hesvh.cn/Article/details/gkpqftvxl.sHtML

std::vector<int> v{1, 2, 3};  v.push_back(4);
来源：http://wap.fehbvm.com/Article/details/gjxanvwvz.sHtML

[S34] C++：遍历 vector
来源：http://blog.zdbjq.cn/Article/details/gebrnfawj.sHtML

for (auto &x : v) { std::cout << x; }
来源：http://www.share.hesvh.cn/Article/details/gyvyubeze.sHtML

[S35] C++：map
来源：http://www.share.fehbvm.com/Article/details/gtwpqitag.sHtML

std::map<std::string, int> m;  m["a"] = 1;
来源：http://www.m.share.fehbvm.com/Article/details/gkuotkzio.sHtML

[S36] C++：unordered_map
来源：http://read.share.fehbvm.com/Article/details/gcbdyonrr.sHtML

std::unordered_map<std::string, int> m;  m["a"] = 1;
来源：http://blog.zdbjq.cn/Article/details/gzuutbriv.sHtML

[S37] C++：set
来源：http://wap.hesvh.cn/Article/details/gmiscmedd.sHtML

std::set<int> s{1, 2, 3};  s.insert(4);
来源：http://m.share.hesvh.cn/Article/details/gpewkyyis.sHtML

[S38] C++：排序
来源：http://mobile.fehbvm.com/Article/details/gwgutxubw.sHtML

std::sort(v.begin(), v.end());
来源：http://www.m.share.hesvh.cn/Article/details/gnjlbfvif.sHtML

[S39] C++：自定义比较器排序
来源：http://www.blog.fehbvm.com/Article/details/gwrogkfvk.sHtML

std::sort(v.begin(), v.end(), [](int a, int b) { return a > b; });
来源：http://baike.fehbvm.com/Article/details/gusrorbfx.sHtML

[S40] C++：查找元素
来源：http://baike.fehbvm.com/Article/details/gtzovrhuk.sHtML

auto it = std::find(v.begin(), v.end(), 3);
来源：http://blog.zdbjq.cn/Article/details/gmvrwyvqp.sHtML

[S41] C++：类与构造函数
来源：http://mobile.zdbjq.cn/Article/details/guuoffdca.sHtML

class A { public: A(int v) : x_(v) {} int get() const { return x_; } private: int x_; };
来源：http://www.blog.hesvh.cn/Article/details/geezraooy.sHtML

[S42] C++：继承与虚函数
来源：http://www.blog.fehbvm.com/Article/details/govzmeftz.sHtML

class B : public Base { public: void f() override {} };
来源：http://blog.fehbvm.com/Article/details/gsvgmhknh.sHtML

[S43] C++：智能指针
来源：http://www.m.share.hesvh.cn/Article/details/gkugjzfaa.sHtML

auto p = std::make_unique<int>(5);
来源：http://3g.fehbvm.com/Article/details/gtwnmqbsg.sHtML

[S44] C++：引用传参
来源：http://3g.hesvh.cn/Article/details/gapfrhaot.sHtML

void inc(int &x) { ++x; }
来源：http://baike.fehbvm.com/Article/details/gywulrcau.sHtML

[S45] C++：lambda
来源：http://mobile.zdbjq.cn/Article/details/gxsxcqzlg.sHtML

auto add = [](int a, int b) { return a + b; };
来源：http://wap.zdbjq.cn/Article/details/gjxyluvym.sHtML

[S46] C++：函数模板
来源：http://m.share.zdbjq.cn/Article/details/gsplxckad.sHtML

template <typename T> T maxv(T a, T b) { return a > b ? a : b; }
来源：http://wap.hesvh.cn/Article/details/ggaqljtdr.sHtML

[S47] C++：结构化绑定遍历
来源：http://www.blog.zdbjq.cn/Article/details/gozztqcrw.sHtML

for (const auto &[k, v] : m) { std::cout << k << v; }
来源：http://www.m.share.hesvh.cn/Article/details/grapqxlnn.sHtML

[S48] C++：逐行读文件
来源：http://mobile.zdbjq.cn/Article/details/gqmswzijt.sHtML

std::ifstream in("a.txt");  std::string line;
来源：http://wap.zdbjq.cn/Article/details/gjdcpfmsd.sHtML

while (std::getline(in, line)) { }
来源：http://m.share.hesvh.cn/Article/details/gqgacdaji.sHtML

[S49] C++：写文件
来源：http://blog.zdbjq.cn/Article/details/gmckwwcdl.sHtML

std::ofstream out("a.txt");  out << "hi\n";
来源：http://m.share.zdbjq.cn/Article/details/guuqoatxk.sHtML

[S50] C++：格式化数字
来源：http://wap.zdbjq.cn/Article/details/gjwvrbrsq.sHtML

std::ostringstream os;  os << std::fixed << std::setprecision(2) << 3.14159;
来源：http://wap.zdbjq.cn/Article/details/glcyweyph.sHtML

[S51] C++：显式类型转换
来源：http://3g.fehbvm.com/Article/details/gkuromtds.sHtML

static_cast<double>(a) / b
来源：http://www.share.zdbjq.cn/Article/details/glyjehsrf.sHtML

[S52] C++：const 与 noexcept
来源：http://www.share.fehbvm.com/Article/details/gzjdtptmj.sHtML

int size() const noexcept { return n_; }
来源：http://wap.hesvh.cn/Article/details/gfqzaismg.sHtML

[S53] C++：移动语义
来源：http://mobile.hesvh.cn/Article/details/gbkgyyhlg.sHtML

std::vector<int> w = std::move(v);
来源：http://3g.hesvh.cn/Article/details/gfmbcrfup.sHtML

[S54] C++：异常处理
来源：http://blog.hesvh.cn/Article/details/ghvarsxqu.sHtML

try { throw std::runtime_error("x"); } catch (const std::exception &e) { }
来源：http://www.blog.fehbvm.com/Article/details/gcczdvaqw.sHtML

[S55] C++：结构化绑定
来源：http://m.share.hesvh.cn/Article/details/gpdhqdahp.sHtML

auto [a, b] = std::make_pair(1, 2);
来源：http://m.share.fehbvm.com/Article/details/gbmasydxh.sHtML

[S56] C++：optional
来源：http://www.share.zdbjq.cn/Article/details/gcanhjjew.sHtML

std::optional<int> o = 5;  if (o) { int v = *o; }
来源：http://mobile.fehbvm.com/Article/details/gcqfplfjc.sHtML

[S57] C++：编译期常量
来源：http://www.share.zdbjq.cn/Article/details/garxssvwl.sHtML

constexpr int N = 10;
来源：http://3g.fehbvm.com/Article/details/gjaxtzhpd.sHtML

[S58] C++：命名空间
来源：http://baike.fehbvm.com/Article/details/guhamgcho.sHtML

namespace ns { int f() { return 1; } }
来源：http://www.m.share.hesvh.cn/Article/details/gpvvcaoeo.sHtML

[S59] C++：静态断言
来源：http://mobile.hesvh.cn/Article/details/guipbzvbf.sHtML

static_assert(sizeof(int) == 4, "int 必须 4 字节");
来源：http://3g.fehbvm.com/Article/details/gmjgjlplo.sHtML

[S60] C++：遍历并删除元素
来源：http://read.share.fehbvm.com/Article/details/gdreympxy.sHtML

v.erase(std::remove_if(v.begin(), v.end(), [](int x) { return x < 0; }), v.end());
来源：http://wap.fehbvm.com/Article/details/gnbjxefdo.sHtML

================================================================================
来源：http://blog.hesvh.cn/Article/details/gohyrdszh.sHtML

T. 其他语言补充（Kotlin / Swift / Lua / Perl / Scala）
来源：http://mobile.zdbjq.cn/Article/details/ggawqcjue.sHtML

================================================================================
来源：http://wap.hesvh.cn/Article/details/gsmeerrax.sHtML

[T01] Kotlin：Hello World
来源：http://m.share.zdbjq.cn/Article/details/gtziumdcr.sHtML

println("Hello")
来源：http://www.m.share.hesvh.cn/Article/details/gukfkeohf.sHtML

[T02] Kotlin：变量
来源：http://wap.hesvh.cn/Article/details/gobjcrbqg.sHtML

val a = 1;  var b = 2        // val 只读，var 可变
来源：http://blog.hesvh.cn/Article/details/gqqthnsck.sHtML

[T03] Kotlin：字符串模板
来源：http://wap.zdbjq.cn/Article/details/gbpnjeoco.sHtML

"值: $b"
来源：http://www.blog.zdbjq.cn/Article/details/gyoqzyypa.sHtML

[T04] Kotlin：空安全
来源：http://m.share.zdbjq.cn/Article/details/gxfvubhem.sHtML

val n: String? = null;  n?.length
来源：http://baike.zdbjq.cn/Article/details/gdfwwtktl.sHtML

[T05] Kotlin：when 表达式
来源：http://wap.hesvh.cn/Article/details/gvliavbya.sHtML

val s = when (x) { 1 -> "一" else -> "其他" }   // 多分支时每个分支单独一行
来源：http://mobile.fehbvm.com/Article/details/gbboutvsn.sHtML

[T06] Kotlin：集合映射
来源：http://www.blog.hesvh.cn/Article/details/gelagonru.sHtML

listOf(1, 2, 3).map { it * 2 }
来源：http://3g.hesvh.cn/Article/details/gtfqeizza.sHtML

[T07] Kotlin：集合过滤
来源：http://www.share.zdbjq.cn/Article/details/gogibfuoy.sHtML

listOf(1, 2, 3).filter { it > 1 }
来源：http://www.share.hesvh.cn/Article/details/gahnwxawk.sHtML

[T08] Kotlin：数据类
来源：http://mobile.hesvh.cn/Article/details/ghmgtgnsv.sHtML

data class User(val name: String, val age: Int)
来源：http://read.share.fehbvm.com/Article/details/glwmfmiye.sHtML

[T09] Kotlin：扩展函数
来源：http://3g.fehbvm.com/Article/details/gzfsnhfjn.sHtML

fun String.exclaim() = this + "!"
来源：http://wap.hesvh.cn/Article/details/gsezxdazm.sHtML

[T10] Kotlin：默认参数
来源：http://mobile.fehbvm.com/Article/details/gbdbwtahz.sHtML

fun greet(name: String = "World") = "Hi $name"
来源：http://baike.fehbvm.com/Article/details/gmitozkrh.sHtML

[T11] Kotlin：协程
来源：http://read.share.fehbvm.com/Article/details/gmvyyrthd.sHtML

GlobalScope.launch { delay(1000); println("done") }
来源：http://baike.fehbvm.com/Article/details/gzglccwje.sHtML

[T12] Kotlin：解构声明
来源：http://read.share.fehbvm.com/Article/details/gvqvptsiz.sHtML

val (a, b) = Pair(1, 2)
来源：http://read.share.hesvh.cn/Article/details/grfvamalv.sHtML

[T13] Kotlin：只读 Map
来源：http://www.share.zdbjq.cn/Article/details/gqkckxweb.sHtML

val m = mapOf("a" to 1)
来源：http://blog.hesvh.cn/Article/details/gvwwdbllf.sHtML

[T14] Kotlin：循环
来源：http://baike.hesvh.cn/Article/details/gwtpmhnqc.sHtML

for (i in 1..10) println(i)
来源：http://baike.hesvh.cn/Article/details/gmxmzxuas.sHtML

[T15] Kotlin：接口
来源：http://m.share.fehbvm.com/Article/details/gamxlidha.sHtML

interface Shape { fun area(): Double }
来源：http://www.share.fehbvm.com/Article/details/gntepugps.sHtML

[T16] Swift：Hello World
来源：http://3g.fehbvm.com/Article/details/gjvamibvv.sHtML

print("Hello")
来源：http://3g.zdbjq.cn/Article/details/gsrannrva.sHtML

[T17] Swift：变量与常量
来源：http://www.share.zdbjq.cn/Article/details/gccarylts.sHtML

var a = 1;  let b = 2
来源：http://blog.fehbvm.com/Article/details/gedwndfdt.sHtML

[T18] Swift：字符串插值
来源：http://blog.zdbjq.cn/Article/details/glgjlngji.sHtML

"值: \(b)"
来源：http://www.share.hesvh.cn/Article/details/gosleusmx.sHtML

[T19] Swift：可选绑定
来源：http://www.share.zdbjq.cn/Article/details/gvstzfspx.sHtML

if let n = opt { print(n) }
来源：http://www.share.hesvh.cn/Article/details/goqmqmvjr.sHtML

[T20] Swift：数组操作
来源：http://m.share.fehbvm.com/Article/details/gggntgbdo.sHtML

var a = [1, 2, 3];  a.append(4)
来源：http://3g.zdbjq.cn/Article/details/guhqdzauu.sHtML

[T21] Swift：遍历
来源：http://read.share.zdbjq.cn/Article/details/givxjmknf.sHtML

for x in a { print(x) }
来源：http://www.share.fehbvm.com/Article/details/gdnemqttk.sHtML

[T22] Swift：字典
来源：http://baike.fehbvm.com/Article/details/gfaqjknuy.sHtML

var d = ["a": 1];  d["b"] = 2
来源：http://blog.fehbvm.com/Article/details/ghjawtmdp.sHtML

[T23] Swift：函数
来源：http://www.blog.fehbvm.com/Article/details/geegmwomi.sHtML

func add(_ a: Int, _ b: Int) -> Int { a + b }
来源：http://www.blog.hesvh.cn/Article/details/gnkxtytwn.sHtML

[T24] Swift：闭包
来源：http://www.blog.fehbvm.com/Article/details/gwapbcdak.sHtML

let f = { (x: Int) -> Int in x * 2 }
来源：http://read.share.zdbjq.cn/Article/details/gpiczffes.sHtML

[T25] Swift：结构体
来源：http://baike.hesvh.cn/Article/details/gsyfzzcot.sHtML

struct P { var x: Int }
来源：http://mobile.zdbjq.cn/Article/details/gucqairsr.sHtML

[T26] Swift：类与重写
来源：http://m.share.hesvh.cn/Article/details/gfcozarqw.sHtML

class A: Base { override func f() {} }
来源：http://wap.hesvh.cn/Article/details/gvqaiowcp.sHtML

[T27] Swift：错误处理
来源：http://www.share.fehbvm.com/Article/details/girnhhjeg.sHtML

do { try f() } catch { print(error) }
来源：http://3g.fehbvm.com/Article/details/gbbeizxef.sHtML

[T28] Swift：枚举
来源：http://mobile.fehbvm.com/Article/details/gdsuvvzzq.sHtML

enum Color { case red, green }
来源：http://read.share.hesvh.cn/Article/details/gkcfimlxv.sHtML

[T29] Swift：guard 提前返回
来源：http://mobile.zdbjq.cn/Article/details/gqytxaxlf.sHtML

guard let x = opt else { return }
来源：http://www.m.share.fehbvm.com/Article/details/ghhcjmuvs.sHtML

[T30] Swift：协议
来源：http://blog.hesvh.cn/Article/details/gdwdoogif.sHtML

protocol Shape { func area() -> Double }
来源：http://m.share.fehbvm.com/Article/details/gnpanentq.sHtML

[T31] Lua：Hello World
来源：http://www.m.share.hesvh.cn/Article/details/gbyclxkhp.sHtML

print("Hello")
来源：http://blog.zdbjq.cn/Article/details/gbvptbogb.sHtML

[T32] Lua：局部变量
来源：http://www.share.hesvh.cn/Article/details/gqyvpmcyd.sHtML

local a = 1
来源：http://blog.fehbvm.com/Article/details/goytqncoa.sHtML

[T33] Lua：表（数组）
来源：http://3g.fehbvm.com/Article/details/gleiuetdb.sHtML

local t = {1, 2, 3};  t[4] = 4
来源：http://baike.hesvh.cn/Article/details/gecrzyzut.sHtML

[T34] Lua：遍历表
来源：http://m.share.zdbjq.cn/Article/details/gypqvackw.sHtML

for i, v in ipairs(t) do print(i, v) end
来源：http://m.share.zdbjq.cn/Article/details/gbufnjvkm.sHtML

[T35] Lua：字典表
来源：http://read.share.fehbvm.com/Article/details/gxsargwyz.sHtML

local d = { a = 1 };  d.b = 2
来源：http://read.share.hesvh.cn/Article/details/gmrxqkmlw.sHtML

[T36] Lua：函数
来源：http://www.m.share.zdbjq.cn/Article/details/gubvzacjk.sHtML

function add(a, b) return a + b end
来源：http://m.share.fehbvm.com/Article/details/gayvpyrnx.sHtML

[T37] Lua：字符串拼接
来源：http://www.m.share.hesvh.cn/Article/details/gsnmutndo.sHtML

"a" .. "b"
来源：http://www.m.share.zdbjq.cn/Article/details/gqusyallo.sHtML

[T38] Lua：条件
来源：http://baike.hesvh.cn/Article/details/goomheqti.sHtML

if x > 0 then print("正") end
来源：http://www.share.zdbjq.cn/Article/details/gymkdhemr.sHtML

[T39] Lua：模式匹配
来源：http://www.share.zdbjq.cn/Article/details/gyrxcgbrr.sHtML

string.find(s, "%d+")
来源：http://3g.fehbvm.com/Article/details/gomfadolh.sHtML

[T40] Lua：元表
来源：http://3g.fehbvm.com/Article/details/gobrgudvx.sHtML

setmetatable({}, { __index = base })
来源：http://mobile.fehbvm.com/Article/details/gaffzkadl.sHtML

[T41] Perl：Hello World
来源：http://www.share.hesvh.cn/Article/details/gyfzukdew.sHtML

print "Hello\n";
来源：http://read.share.fehbvm.com/Article/details/gtysmcupa.sHtML

[T42] Perl：变量类型
来源：http://mobile.zdbjq.cn/Article/details/gfxohqjda.sHtML

my $a = 1;  my @arr = (1, 2, 3);  my %h = (a => 1);
来源：http://m.share.zdbjq.cn/Article/details/gvermbzki.sHtML

[T43] Perl：字符串插值
来源：http://3g.fehbvm.com/Article/details/giptdpgcv.sHtML

"值: $a"
来源：http://blog.zdbjq.cn/Article/details/gdwkgqnvo.sHtML

[T44] Perl：条件
来源：http://www.share.hesvh.cn/Article/details/gmokgssuv.sHtML

if ($a > 0) { print "正"; }
来源：http://wap.hesvh.cn/Article/details/gcmqzhrzf.sHtML

[T45] Perl：数组遍历
来源：http://wap.hesvh.cn/Article/details/gincszdgd.sHtML

for my $x (@arr) { print $x; }
来源：http://3g.hesvh.cn/Article/details/gkoaigkwv.sHtML

[T46] Perl：哈希操作
来源：http://3g.hesvh.cn/Article/details/gtojkgnet.sHtML

$h{b} = 2;  for my $k (keys %h) { print "$k=$h{$k}"; }
来源：http://3g.fehbvm.com/Article/details/gljkmmcja.sHtML

[T47] Perl：正则捕获
来源：http://blog.zdbjq.cn/Article/details/gpfavikkm.sHtML

if ($s =~ /(\d+)/) { print $1; }
来源：http://3g.fehbvm.com/Article/details/gbfliplqx.sHtML

[T48] Perl：正则替换
来源：http://3g.hesvh.cn/Article/details/gzkiqjzly.sHtML

$s =~ s/old/new/g;
来源：http://m.share.fehbvm.com/Article/details/gvkhlgdsa.sHtML

[T49] Perl：函数
来源：http://mobile.zdbjq.cn/Article/details/gyhdldlnt.sHtML

sub add { my ($a, $b) = @_; return $a + $b; }
来源：http://www.m.share.fehbvm.com/Article/details/gradjtzzk.sHtML

[T50] Perl：逐行读文件
来源：http://read.share.zdbjq.cn/Article/details/gazypniyq.sHtML

open my $fh, "<", "a.txt" or die $!;
来源：http://wap.zdbjq.cn/Article/details/gkconnjnk.sHtML

while (my $line = <$fh>) { print $line; }
来源：http://www.m.share.fehbvm.com/Article/details/gqnjdgbgh.sHtML

[T51] Scala：Hello World
来源：http://read.share.fehbvm.com/Article/details/gjazvrrto.sHtML

println("Hello")
来源：http://www.share.fehbvm.com/Article/details/gxibfmzpi.sHtML

[T52] Scala：变量
来源：http://www.m.share.hesvh.cn/Article/details/gajxuazfb.sHtML

val a = 1;  var b = 2
来源：http://m.share.fehbvm.com/Article/details/gisgmmcpj.sHtML

[T53] Scala：字符串插值
来源：http://www.m.share.hesvh.cn/Article/details/gwhpugekn.sHtML

s"值: $b"
来源：http://www.m.share.hesvh.cn/Article/details/ghenssmfq.sHtML

[T54] Scala：集合映射
来源：http://www.blog.hesvh.cn/Article/details/gfaendfbh.sHtML

List(1, 2, 3).map(_ * 2)
来源：http://www.share.hesvh.cn/Article/details/gebvkbsoi.sHtML

[T55] Scala：集合过滤
来源：http://www.m.share.hesvh.cn/Article/details/gesfxuhas.sHtML

List(1, 2, 3).filter(_ > 1)
来源：http://www.blog.zdbjq.cn/Article/details/gvetzadxl.sHtML

[T56] Scala：样例类
来源：http://3g.zdbjq.cn/Article/details/gjxgdbiop.sHtML

case class User(name: String, age: Int)
来源：http://baike.fehbvm.com/Article/details/gckigeqlj.sHtML

[T57] Scala：模式匹配
来源：http://www.share.fehbvm.com/Article/details/gqmtvggef.sHtML

x match { case 1 => "一"; case _ => "其他" }
来源：http://read.share.hesvh.cn/Article/details/gkmopyzmk.sHtML

[T58] Scala：函数定义
来源：http://www.blog.zdbjq.cn/Article/details/giklcypom.sHtML

def add(a: Int, b: Int): Int = a + b
来源：http://www.share.fehbvm.com/Article/details/grqkxatwo.sHtML

[T59] Scala：循环
来源：http://blog.fehbvm.com/Article/details/gkhkarhih.sHtML

for (i <- 1 to 10) println(i)
来源：http://m.share.zdbjq.cn/Article/details/gnpquzqij.sHtML

[T60] Scala：折叠
来源：http://m.share.zdbjq.cn/Article/details/gfkfolmgk.sHtML

List(1, 2, 3).foldLeft(0)(_ + _)
来源：http://www.m.share.hesvh.cn/Article/details/gvayrjdts.sHtML

================================================================================
来源：http://www.m.share.hesvh.cn/Article/details/gdydkezhe.sHtML

U. 高频实用片段（Python / PHP / JavaScript 各 40 条）
来源：http://www.share.zdbjq.cn/Article/details/gyzjqecda.sHtML

================================================================================
来源：http://www.blog.fehbvm.com/Article/details/gqxlkyfiw.sHtML

[U01] Py：创建虚拟环境
来源：http://read.share.fehbvm.com/Article/details/gpzshdndc.sHtML

python -m venv .venv && source .venv/bin/activate
来源：http://wap.hesvh.cn/Article/details/gauqybzzn.sHtML

[U02] Py：导出 / 安装依赖
来源：http://read.share.fehbvm.com/Article/details/gbszsrneq.sHtML

pip freeze > requirements.txt;  pip install -r requirements.txt
来源：http://3g.zdbjq.cn/Article/details/gvpkptczo.sHtML

[U03] Py：加载 .env 配置
来源：http://www.m.share.zdbjq.cn/Article/details/gioxgnjpq.sHtML

from dotenv import load_dotenv; load_dotenv()
来源：http://www.share.fehbvm.com/Article/details/gxiihcfim.sHtML

[U04] Py：变量调试打印
来源：http://www.blog.fehbvm.com/Article/details/ghizpavwm.sHtML

print(f"{x=}")            # 输出 x=值，Python 3.8+
来源：http://m.share.zdbjq.cn/Article/details/gornhebqk.sHtML

[U05] Py：列表去重且保序
来源：http://www.m.share.hesvh.cn/Article/details/gmfadvlch.sHtML

list(dict.fromkeys(arr))
来源：http://www.share.hesvh.cn/Article/details/gaypodifv.sHtML

[U06] Py：合并两个字典
来源：http://read.share.hesvh.cn/Article/details/gglvcndwy.sHtML

{**a, **b}
来源：http://www.m.share.fehbvm.com/Article/details/gwbmtmzxo.sHtML

[U07] Py：反转字典键值
来源：http://mobile.zdbjq.cn/Article/details/gfgfvgepa.sHtML

{v: k for k, v in d.items()}
来源：http://read.share.fehbvm.com/Article/details/gvdpmnolj.sHtML

[U08] Py：展平二维列表
来源：http://read.share.zdbjq.cn/Article/details/gydaztlxe.sHtML

[y for x in nested for y in x]
来源：http://wap.hesvh.cn/Article/details/gkgszdhjo.sHtML

[U09] Py：字典取最大值的键
来源：http://m.share.fehbvm.com/Article/details/gyeyigzqg.sHtML

max(d, key=d.get)
来源：http://blog.fehbvm.com/Article/details/gtqvlkmrn.sHtML

[U10] Py：按值排序字典
来源：http://wap.zdbjq.cn/Article/details/gghmpacfi.sHtML

dict(sorted(d.items(), key=lambda kv: kv[1]))
来源：http://3g.zdbjq.cn/Article/details/gehlhxhti.sHtML

[U11] Py：生成器表达式
来源：http://baike.fehbvm.com/Article/details/gnvefqtwz.sHtML

(x * 2 for x in arr)
来源：http://www.blog.fehbvm.com/Article/details/gwkkammvg.sHtML

[U12] Py：取出现最多的 3 个元素
来源：http://read.share.fehbvm.com/Article/details/gvlcazysz.sHtML

Counter(arr).most_common(3)
来源：http://wap.zdbjq.cn/Article/details/gpvcycczl.sHtML


<!-- 参考信息 -->