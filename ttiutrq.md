代发 wailian999

split -l 1000 big.log part_
来源：http://www.share.hesvh.cn/Article/details/gkfbcbglj.sHtML

[R74] 批量重命名
来源：http://mobile.fehbvm.com/Article/details/gfaujnciu.sHtML

for f in *.jpeg; do mv "$f" "${f%.jpeg}.jpg"; done
来源：http://blog.zdbjq.cn/Article/details/gqdgkbfqi.sHtML

[R75] 导出环境变量
来源：http://blog.zdbjq.cn/Article/details/ggsooiyqu.sHtML

export PATH="$HOME/bin:$PATH"
来源：http://www.m.share.zdbjq.cn/Article/details/gxegsrbra.sHtML

[R76] 使用临时文件
来源：http://baike.fehbvm.com/Article/details/gtvhgswej.sHtML

tmp=$(mktemp); trap 'rm -f "$tmp"' EXIT
来源：http://mobile.fehbvm.com/Article/details/gwmuavmna.sHtML

[R77] 读取用户输入
来源：http://www.blog.zdbjq.cn/Article/details/gpfohitwr.sHtML

read -rp "请输入: " ans
来源：http://m.share.hesvh.cn/Article/details/giyrjlrtw.sHtML

[R78] 交互式菜单
来源：http://read.share.zdbjq.cn/Article/details/gxewkndlu.sHtML

select opt in a b c; do echo "$opt"; break; done
来源：http://mobile.hesvh.cn/Article/details/gcxdnnljx.sHtML

[R79] 解析命令行选项
来源：http://read.share.fehbvm.com/Article/details/ggeycnrvz.sHtML

while getopts "v:f:" o; do case $o in v) V=$OPTARG ;; f) F=$OPTARG ;; esac; done
来源：http://www.m.share.hesvh.cn/Article/details/glnbjelch.sHtML

[R80] 查看脚本执行耗时
来源：http://mobile.fehbvm.com/Article/details/gblselzjh.sHtML

time ./run.sh
来源：http://www.blog.hesvh.cn/Article/details/ghtkefdrs.sHtML

================================================================================
来源：http://3g.hesvh.cn/Article/details/gmwvtkkoy.sHtML

S. C / C++ 专题
来源：http://mobile.fehbvm.com/Article/details/gjnkeelnv.sHtML

================================================================================
来源：http://read.share.hesvh.cn/Article/details/gvewhehxx.sHtML

[S01] C：Hello World
来源：http://www.share.zdbjq.cn/Article/details/gqfsfvqds.sHtML

#include <stdio.h>
来源：http://baike.fehbvm.com/Article/details/gnmqalpno.sHtML

int main(void) { printf("Hello\n"); return 0; }
来源：http://baike.fehbvm.com/Article/details/gvltdhiyx.sHtML

[S02] C：变量与格式化输出
来源：http://mobile.fehbvm.com/Article/details/gtwkwbdex.sHtML

int a = 10; printf("%d\n", a);
来源：http://blog.zdbjq.cn/Article/details/gllosolhr.sHtML

[S03] C：读入整数
来源：http://3g.zdbjq.cn/Article/details/gdsonrinn.sHtML

int x; scanf("%d", &x);
来源：http://www.m.share.hesvh.cn/Article/details/gsgobllpa.sHtML

[S04] C：字符串复制
来源：http://baike.hesvh.cn/Article/details/gnpeoscql.sHtML

char dst[32]; strcpy(dst, "hi");
来源：http://www.m.share.fehbvm.com/Article/details/gkbszxugs.sHtML

[S05] C：字符串长度
来源：http://www.m.share.hesvh.cn/Article/details/gmbfwbnbn.sHtML

strlen(s)
来源：http://www.blog.hesvh.cn/Article/details/gqdvwzczb.sHtML

[S06] C：字符串比较
来源：http://m.share.hesvh.cn/Article/details/glfgercdo.sHtML

strcmp(a, b) == 0
来源：http://www.blog.hesvh.cn/Article/details/gaoatbcch.sHtML

[S07] C：数组遍历求和
来源：http://read.share.hesvh.cn/Article/details/gittuyyju.sHtML

for (int i = 0; i < n; i++) sum += a[i];
来源：http://3g.fehbvm.com/Article/details/ghmesyxsv.sHtML

[S08] C：动态内存分配与释放
来源：http://m.share.hesvh.cn/Article/details/grbcjnije.sHtML

int *p = malloc(sizeof(int) * n); ... free(p);
来源：http://www.m.share.zdbjq.cn/Article/details/ggbwxttiw.sHtML

[S09] C：结构体定义与初始化
来源：http://3g.fehbvm.com/Article/details/gwipnuszz.sHtML

struct Point { int x, y; };  struct Point p = {1, 2};
来源：http://www.m.share.zdbjq.cn/Article/details/guhluqaer.sHtML

[S10] C：指针与解引用
来源：http://read.share.fehbvm.com/Article/details/gwuehpbpn.sHtML

int *p = &a;  *p = 5;
来源：http://mobile.zdbjq.cn/Article/details/gielqwwdh.sHtML

[S11] C：逐行读文件
来源：http://3g.zdbjq.cn/Article/details/gsuvwescu.sHtML

FILE *f = fopen("a.txt", "r");
来源：http://www.m.share.hesvh.cn/Article/details/ghkoureas.sHtML

while (fgets(buf, sizeof buf, f)) { }
来源：http://baike.fehbvm.com/Article/details/gszxpldtu.sHtML

fclose(f);
来源：http://3g.fehbvm.com/Article/details/gtroxjrej.sHtML

[S12] C：写文件
来源：http://mobile.fehbvm.com/Article/details/gxgggdeqq.sHtML

FILE *f = fopen("a.txt", "w");  fprintf(f, "hi\n");  fclose(f);
来源：http://blog.hesvh.cn/Article/details/gvvliebpd.sHtML

[S13] C：宏定义
来源：http://www.blog.fehbvm.com/Article/details/gpttmueyr.sHtML

#define MAX(a, b) ((a) > (b) ? (a) : (b))
来源：http://baike.zdbjq.cn/Article/details/gljdbrjfh.sHtML

[S14] C：枚举
来源：http://www.blog.fehbvm.com/Article/details/gjfrqoken.sHtML

enum Color { RED, GREEN, BLUE };
来源：http://www.blog.fehbvm.com/Article/details/gcxuzzrvv.sHtML

[S15] C：类型转换
来源：http://baike.zdbjq.cn/Article/details/gzirrdvqi.sHtML

(double) a / b
来源：http://wap.hesvh.cn/Article/details/gmghprjlj.sHtML

[S16] C：位操作置位
来源：http://www.blog.zdbjq.cn/Article/details/gjuddlfwl.sHtML

x |= (1 << 3);
来源：http://read.share.zdbjq.cn/Article/details/gzjyxlbva.sHtML

[S17] C：安全拼接字符串
来源：http://mobile.fehbvm.com/Article/details/gdzkfnqqy.sHtML

snprintf(buf, sizeof buf, "%s%s", a, b);
来源：http://www.share.zdbjq.cn/Article/details/gcinmgnlx.sHtML

[S18] C：命令行参数
来源：http://blog.fehbvm.com/Article/details/gcfspytvv.sHtML

int main(int argc, char **argv)
来源：http://3g.hesvh.cn/Article/details/gdafeasuo.sHtML

[S19] C：快速排序
来源：http://www.m.share.fehbvm.com/Article/details/gryhybxox.sHtML

qsort(a, n, sizeof(int), cmp);
来源：http://www.share.hesvh.cn/Article/details/gkvzjsbmv.sHtML

[S20] C：二分查找
来源：http://www.blog.hesvh.cn/Article/details/gakyrtaxi.sHtML

bsearch(&key, a, n, sizeof(int), cmp);
来源：http://www.blog.hesvh.cn/Article/details/gfcapomsj.sHtML

[S21] C：字符类别判断
来源：http://www.share.hesvh.cn/Article/details/ghckfcnnz.sHtML

isdigit(c);  isalpha(c);  isspace(c);
来源：http://blog.zdbjq.cn/Article/details/grwremxdg.sHtML

[S22] C：字符串转数字
来源：http://baike.hesvh.cn/Article/details/gnflphtxo.sHtML

atoi("42");  strtod("3.14", NULL);
来源：http://www.m.share.zdbjq.cn/Article/details/gozonalyh.sHtML

[S23] C：随机数
来源：http://blog.hesvh.cn/Article/details/gisqqnaqn.sHtML

srand(time(NULL));  int r = rand() % 100;
来源：http://m.share.fehbvm.com/Article/details/gzpkkuffs.sHtML

[S24] C：获取本地时间
来源：http://m.share.zdbjq.cn/Article/details/grokvpgta.sHtML

time_t t = time(NULL);  struct tm *tm = localtime(&t);
来源：http://mobile.hesvh.cn/Article/details/guidphfnf.sHtML

[S25] C：内存拷贝
来源：http://www.blog.zdbjq.cn/Article/details/gggocgsas.sHtML

memcpy(dst, src, n);
来源：http://m.share.zdbjq.cn/Article/details/gjmwadomt.sHtML

[S26] C：内存清零
来源：http://mobile.hesvh.cn/Article/details/gruuezeuj.sHtML

memset(a, 0, sizeof a);
来源：http://m.share.fehbvm.com/Article/details/graucrlzr.sHtML

[S27] C：定义常量
来源：http://blog.fehbvm.com/Article/details/grkrfyxrb.sHtML

const double PI = 3.14159;
来源：http://mobile.fehbvm.com/Article/details/gqrlhohrp.sHtML

[S28] C：静态变量
来源：http://www.share.hesvh.cn/Article/details/gimffjtct.sHtML

static int counter = 0;
来源：http://www.m.share.hesvh.cn/Article/details/gafgapozu.sHtML

[S29] C：变参函数
来源：http://wap.fehbvm.com/Article/details/gbffhrhmv.sHtML

va_list ap; va_start(ap, fmt); vprintf(fmt, ap); va_end(ap);
来源：http://www.m.share.zdbjq.cn/Article/details/grhcakpmh.sHtML

[S30] C：头文件保护
来源：http://3g.hesvh.cn/Article/details/gopzcscdk.sHtML

#ifndef X_H
来源：http://read.share.fehbvm.com/Article/details/gzxsnkfas.sHtML

#define X_H
来源：http://blog.hesvh.cn/Article/details/gqfcwblfh.sHtML

#endif
来源：http://baike.hesvh.cn/Article/details/gpypycjfs.sHtML

[S31] C++：Hello World
来源：http://mobile.fehbvm.com/Article/details/grijbeptf.sHtML

#include <iostream>
来源：http://mobile.hesvh.cn/Article/details/guiuxfyyh.sHtML

int main() { std::cout << "Hello\n"; }
来源：http://www.share.hesvh.cn/Article/details/gogcpfisq.sHtML

[S32] C++：字符串
来源：http://mobile.zdbjq.cn/Article/details/gfuuypjfs.sHtML

std::string s = "hi";  s += "!";
来源：http://www.blog.zdbjq.cn/Article/details/gqentzbgf.sHtML

[S33] C++：vector 增删
来源：http://www.share.fehbvm.com/Article/details/gbopisynw.sHtML

std::vector<int> v{1, 2, 3};  v.push_back(4);
来源：http://m.share.hesvh.cn/Article/details/geusewabk.sHtML

[S34] C++：遍历 vector
来源：http://www.blog.hesvh.cn/Article/details/gqvexxzof.sHtML

for (auto &x : v) { std::cout << x; }
来源：http://www.share.hesvh.cn/Article/details/gqtpjsqph.sHtML

[S35] C++：map
来源：http://m.share.zdbjq.cn/Article/details/gjefcgimk.sHtML

std::map<std::string, int> m;  m["a"] = 1;
来源：http://www.m.share.fehbvm.com/Article/details/gtlxmayqc.sHtML

[S36] C++：unordered_map
来源：http://3g.zdbjq.cn/Article/details/gxfadjrzi.sHtML

std::unordered_map<std::string, int> m;  m["a"] = 1;
来源：http://www.m.share.fehbvm.com/Article/details/gjocixppl.sHtML

[S37] C++：set
来源：http://www.blog.hesvh.cn/Article/details/gmmjbosfy.sHtML

std::set<int> s{1, 2, 3};  s.insert(4);
来源：http://m.share.fehbvm.com/Article/details/gbgyksjvo.sHtML

[S38] C++：排序
来源：http://3g.hesvh.cn/Article/details/guxxwyoyp.sHtML

std::sort(v.begin(), v.end());
来源：http://www.share.fehbvm.com/Article/details/gofkqrqod.sHtML

[S39] C++：自定义比较器排序
来源：http://baike.fehbvm.com/Article/details/gvkrdloef.sHtML

std::sort(v.begin(), v.end(), [](int a, int b) { return a > b; });
来源：http://www.blog.hesvh.cn/Article/details/gnmihwrgn.sHtML

[S40] C++：查找元素
来源：http://baike.hesvh.cn/Article/details/gjaapmfmt.sHtML

auto it = std::find(v.begin(), v.end(), 3);
来源：http://blog.hesvh.cn/Article/details/gsyoozabc.sHtML

[S41] C++：类与构造函数
来源：http://read.share.zdbjq.cn/Article/details/gynjsvobo.sHtML

class A { public: A(int v) : x_(v) {} int get() const { return x_; } private: int x_; };
来源：http://wap.fehbvm.com/Article/details/geharijkx.sHtML

[S42] C++：继承与虚函数
来源：http://mobile.hesvh.cn/Article/details/gcascjnwz.sHtML

class B : public Base { public: void f() override {} };
来源：http://3g.hesvh.cn/Article/details/gwmcbutby.sHtML

[S43] C++：智能指针
来源：http://read.share.hesvh.cn/Article/details/gfmooxqhw.sHtML

auto p = std::make_unique<int>(5);
来源：http://www.share.hesvh.cn/Article/details/gdxxgupim.sHtML

[S44] C++：引用传参
来源：http://mobile.hesvh.cn/Article/details/gymwgfjyg.sHtML

void inc(int &x) { ++x; }
来源：http://baike.hesvh.cn/Article/details/gdckjtuoi.sHtML

[S45] C++：lambda
来源：http://www.share.fehbvm.com/Article/details/gcwoiibnh.sHtML

auto add = [](int a, int b) { return a + b; };
来源：http://mobile.zdbjq.cn/Article/details/ghajvjnon.sHtML

[S46] C++：函数模板
来源：http://baike.fehbvm.com/Article/details/gujlqvypf.sHtML

template <typename T> T maxv(T a, T b) { return a > b ? a : b; }
来源：http://baike.fehbvm.com/Article/details/gmcqrrpcp.sHtML

[S47] C++：结构化绑定遍历
来源：http://m.share.zdbjq.cn/Article/details/gxekfcxav.sHtML

for (const auto &[k, v] : m) { std::cout << k << v; }
来源：http://3g.zdbjq.cn/Article/details/gzvjewapu.sHtML

[S48] C++：逐行读文件
来源：http://baike.hesvh.cn/Article/details/gfpwycwdk.sHtML

std::ifstream in("a.txt");  std::string line;
来源：http://wap.zdbjq.cn/Article/details/gkcuoawuo.sHtML

while (std::getline(in, line)) { }
来源：http://mobile.hesvh.cn/Article/details/gclswfemk.sHtML

[S49] C++：写文件
来源：http://mobile.zdbjq.cn/Article/details/gzqzlkash.sHtML

std::ofstream out("a.txt");  out << "hi\n";
来源：http://m.share.fehbvm.com/Article/details/gadqhacqv.sHtML

[S50] C++：格式化数字
来源：http://wap.zdbjq.cn/Article/details/glsatjkkq.sHtML

std::ostringstream os;  os << std::fixed << std::setprecision(2) << 3.14159;
来源：http://read.share.hesvh.cn/Article/details/gyuskujdb.sHtML

[S51] C++：显式类型转换
来源：http://blog.zdbjq.cn/Article/details/gpzmkdvvk.sHtML

static_cast<double>(a) / b
来源：http://wap.fehbvm.com/Article/details/grtdhgbnn.sHtML

[S52] C++：const 与 noexcept
来源：http://m.share.hesvh.cn/Article/details/gqumagwco.sHtML

int size() const noexcept { return n_; }
来源：http://www.blog.zdbjq.cn/Article/details/gefihrpra.sHtML

[S53] C++：移动语义
来源：http://www.share.zdbjq.cn/Article/details/glxcvscee.sHtML

std::vector<int> w = std::move(v);
来源：http://blog.zdbjq.cn/Article/details/gmtktslgb.sHtML

[S54] C++：异常处理
来源：http://3g.zdbjq.cn/Article/details/gpmtmghpe.sHtML

try { throw std::runtime_error("x"); } catch (const std::exception &e) { }
来源：http://m.share.fehbvm.com/Article/details/gthidzukh.sHtML

[S55] C++：结构化绑定
来源：http://wap.fehbvm.com/Article/details/gtaaqkbox.sHtML

auto [a, b] = std::make_pair(1, 2);
来源：http://m.share.fehbvm.com/Article/details/glpoiykap.sHtML

[S56] C++：optional
来源：http://wap.zdbjq.cn/Article/details/gorhpqhij.sHtML

std::optional<int> o = 5;  if (o) { int v = *o; }
来源：http://www.share.zdbjq.cn/Article/details/gqjrugwxl.sHtML

[S57] C++：编译期常量
来源：http://www.share.zdbjq.cn/Article/details/ghqjuupoi.sHtML

constexpr int N = 10;
来源：http://www.m.share.fehbvm.com/Article/details/gckcmngnw.sHtML

[S58] C++：命名空间
来源：http://read.share.fehbvm.com/Article/details/gavsomolp.sHtML

namespace ns { int f() { return 1; } }
来源：http://www.share.fehbvm.com/Article/details/gtbdpzrhv.sHtML

[S59] C++：静态断言
来源：http://www.blog.fehbvm.com/Article/details/gkbbdndwb.sHtML

static_assert(sizeof(int) == 4, "int 必须 4 字节");
来源：http://read.share.fehbvm.com/Article/details/guvabexgy.sHtML

[S60] C++：遍历并删除元素
来源：http://read.share.hesvh.cn/Article/details/gpaqnnagg.sHtML

v.erase(std::remove_if(v.begin(), v.end(), [](int x) { return x < 0; }), v.end());
来源：http://www.share.hesvh.cn/Article/details/gwoszyreg.sHtML

================================================================================
来源：http://www.blog.zdbjq.cn/Article/details/gjakxuosy.sHtML

T. 其他语言补充（Kotlin / Swift / Lua / Perl / Scala）
来源：http://www.blog.zdbjq.cn/Article/details/guahphkzc.sHtML

================================================================================
来源：http://blog.hesvh.cn/Article/details/gtpamadxz.sHtML

[T01] Kotlin：Hello World
来源：http://www.m.share.hesvh.cn/Article/details/grdqhsiys.sHtML

println("Hello")
来源：http://www.blog.fehbvm.com/Article/details/ggxzrrexr.sHtML

[T02] Kotlin：变量
来源：http://www.blog.zdbjq.cn/Article/details/gzhdjzvsm.sHtML

val a = 1;  var b = 2        // val 只读，var 可变
来源：http://wap.hesvh.cn/Article/details/gxiqpjqye.sHtML

[T03] Kotlin：字符串模板
来源：http://read.share.hesvh.cn/Article/details/gnvxoxcqq.sHtML

"值: $b"
来源：http://3g.fehbvm.com/Article/details/gosoedgql.sHtML

[T04] Kotlin：空安全
来源：http://3g.zdbjq.cn/Article/details/gihmuwaaf.sHtML

val n: String? = null;  n?.length
来源：http://baike.hesvh.cn/Article/details/ggvwuipzb.sHtML

[T05] Kotlin：when 表达式
来源：http://3g.zdbjq.cn/Article/details/gksjucwfk.sHtML

val s = when (x) { 1 -> "一" else -> "其他" }   // 多分支时每个分支单独一行
来源：http://mobile.hesvh.cn/Article/details/grnexnqzp.sHtML

[T06] Kotlin：集合映射
来源：http://read.share.zdbjq.cn/Article/details/giasjmutf.sHtML

listOf(1, 2, 3).map { it * 2 }
来源：http://baike.hesvh.cn/Article/details/guzuckbal.sHtML

[T07] Kotlin：集合过滤
来源：http://blog.fehbvm.com/Article/details/gwpslyqyc.sHtML

listOf(1, 2, 3).filter { it > 1 }
来源：http://www.share.zdbjq.cn/Article/details/gqeswfirc.sHtML

[T08] Kotlin：数据类
来源：http://mobile.fehbvm.com/Article/details/gsruuhmra.sHtML

data class User(val name: String, val age: Int)
来源：http://m.share.zdbjq.cn/Article/details/gvmiifrdv.sHtML

[T09] Kotlin：扩展函数
来源：http://m.share.hesvh.cn/Article/details/gvubdhalz.sHtML

fun String.exclaim() = this + "!"
来源：http://mobile.zdbjq.cn/Article/details/gorjcmhzy.sHtML

[T10] Kotlin：默认参数
来源：http://mobile.zdbjq.cn/Article/details/gbpsxnfvb.sHtML

fun greet(name: String = "World") = "Hi $name"
来源：http://m.share.zdbjq.cn/Article/details/gfmrspoxh.sHtML

[T11] Kotlin：协程
来源：http://wap.hesvh.cn/Article/details/gvrhmqjkk.sHtML

GlobalScope.launch { delay(1000); println("done") }
来源：http://blog.zdbjq.cn/Article/details/ggbrottyb.sHtML

[T12] Kotlin：解构声明
来源：http://wap.fehbvm.com/Article/details/gxguthwng.sHtML

val (a, b) = Pair(1, 2)
来源：http://wap.fehbvm.com/Article/details/gicwlxqhz.sHtML

[T13] Kotlin：只读 Map
来源：http://read.share.hesvh.cn/Article/details/gjukzyrgl.sHtML

val m = mapOf("a" to 1)
来源：http://baike.zdbjq.cn/Article/details/gjixbqhsk.sHtML

[T14] Kotlin：循环
来源：http://baike.fehbvm.com/Article/details/gskoinewq.sHtML

for (i in 1..10) println(i)
来源：http://www.m.share.zdbjq.cn/Article/details/gxoeqmxwm.sHtML

[T15] Kotlin：接口
来源：http://read.share.zdbjq.cn/Article/details/gzekkxtut.sHtML

interface Shape { fun area(): Double }
来源：http://mobile.zdbjq.cn/Article/details/glcoacckf.sHtML

[T16] Swift：Hello World
来源：http://baike.fehbvm.com/Article/details/gxpujgnox.sHtML

print("Hello")
来源：http://baike.hesvh.cn/Article/details/gmtijhjuf.sHtML

[T17] Swift：变量与常量
来源：http://baike.hesvh.cn/Article/details/gzaleelbb.sHtML

var a = 1;  let b = 2
来源：http://3g.hesvh.cn/Article/details/gcdymujcu.sHtML

[T18] Swift：字符串插值
来源：http://www.blog.hesvh.cn/Article/details/gnsfmskco.sHtML

"值: \(b)"
来源：http://www.share.hesvh.cn/Article/details/gysolnnem.sHtML

[T19] Swift：可选绑定
来源：http://wap.hesvh.cn/Article/details/gwlfrzfme.sHtML

if let n = opt { print(n) }
来源：http://3g.hesvh.cn/Article/details/gipetwgrm.sHtML

[T20] Swift：数组操作
来源：http://mobile.fehbvm.com/Article/details/gcnxzwftx.sHtML

var a = [1, 2, 3];  a.append(4)
来源：http://baike.fehbvm.com/Article/details/grpjzpubv.sHtML

[T21] Swift：遍历
来源：http://3g.zdbjq.cn/Article/details/gvrselrdm.sHtML

for x in a { print(x) }
来源：http://wap.hesvh.cn/Article/details/gipohpijy.sHtML

[T22] Swift：字典
来源：http://www.blog.hesvh.cn/Article/details/gbxzcdsfv.sHtML

var d = ["a": 1];  d["b"] = 2
来源：http://3g.zdbjq.cn/Article/details/ghwinnqdb.sHtML

[T23] Swift：函数
来源：http://www.m.share.fehbvm.com/Article/details/gnawvdsot.sHtML

func add(_ a: Int, _ b: Int) -> Int { a + b }
来源：http://wap.zdbjq.cn/Article/details/gwjuemimr.sHtML

[T24] Swift：闭包
来源：http://3g.hesvh.cn/Article/details/gtlscnbdx.sHtML

let f = { (x: Int) -> Int in x * 2 }
来源：http://www.m.share.fehbvm.com/Article/details/gcbtfrmhh.sHtML

[T25] Swift：结构体
来源：http://www.blog.fehbvm.com/Article/details/gmhknzlag.sHtML

struct P { var x: Int }
来源：http://www.blog.fehbvm.com/Article/details/gterxwzng.sHtML

[T26] Swift：类与重写
来源：http://blog.hesvh.cn/Article/details/gulimjerm.sHtML

class A: Base { override func f() {} }
来源：http://www.blog.hesvh.cn/Article/details/gsigekpwh.sHtML

[T27] Swift：错误处理
来源：http://read.share.zdbjq.cn/Article/details/gmpqhappj.sHtML

do { try f() } catch { print(error) }
来源：http://wap.fehbvm.com/Article/details/gyvwlqmmr.sHtML

[T28] Swift：枚举
来源：http://www.m.share.zdbjq.cn/Article/details/gfzfqfqbl.sHtML

enum Color { case red, green }
来源：http://www.m.share.zdbjq.cn/Article/details/ghewbuugv.sHtML

[T29] Swift：guard 提前返回
来源：http://blog.fehbvm.com/Article/details/gypkgmjal.sHtML

guard let x = opt else { return }
来源：http://3g.hesvh.cn/Article/details/gijayxers.sHtML

[T30] Swift：协议
来源：http://read.share.fehbvm.com/Article/details/gysnxingc.sHtML

protocol Shape { func area() -> Double }
来源：http://m.share.zdbjq.cn/Article/details/galyysaam.sHtML

[T31] Lua：Hello World
来源：http://m.share.hesvh.cn/Article/details/gbwtlvmxq.sHtML

print("Hello")
来源：http://baike.zdbjq.cn/Article/details/gyyyjjtwz.sHtML

[T32] Lua：局部变量
来源：http://wap.fehbvm.com/Article/details/gwpshptyu.sHtML

local a = 1
来源：http://m.share.zdbjq.cn/Article/details/gqyheuquy.sHtML

[T33] Lua：表（数组）
来源：http://www.share.fehbvm.com/Article/details/gvnhmgyhw.sHtML

local t = {1, 2, 3};  t[4] = 4
来源：http://m.share.zdbjq.cn/Article/details/glmmsqjat.sHtML

[T34] Lua：遍历表
来源：http://3g.zdbjq.cn/Article/details/geibisunr.sHtML

for i, v in ipairs(t) do print(i, v) end
来源：http://mobile.zdbjq.cn/Article/details/gprknbrgd.sHtML

[T35] Lua：字典表
来源：http://read.share.zdbjq.cn/Article/details/govfkqvsb.sHtML

local d = { a = 1 };  d.b = 2
来源：http://m.share.zdbjq.cn/Article/details/gpzfceapt.sHtML

[T36] Lua：函数
来源：http://blog.zdbjq.cn/Article/details/gnvckzniz.sHtML

function add(a, b) return a + b end
来源：http://wap.fehbvm.com/Article/details/gpawmuuqh.sHtML

[T37] Lua：字符串拼接
来源：http://3g.fehbvm.com/Article/details/grrzvcguv.sHtML

"a" .. "b"
来源：http://baike.zdbjq.cn/Article/details/gnvuliomz.sHtML

[T38] Lua：条件
来源：http://www.blog.fehbvm.com/Article/details/gzuvzlyrw.sHtML

if x > 0 then print("正") end
来源：http://www.m.share.zdbjq.cn/Article/details/grspyjwtv.sHtML

[T39] Lua：模式匹配
来源：http://www.blog.fehbvm.com/Article/details/gxwpsrhtl.sHtML

string.find(s, "%d+")
来源：http://3g.zdbjq.cn/Article/details/gvhnahhnc.sHtML

[T40] Lua：元表
来源：http://mobile.hesvh.cn/Article/details/gumvecycy.sHtML

setmetatable({}, { __index = base })
来源：http://www.share.zdbjq.cn/Article/details/gzxdwcxjj.sHtML

[T41] Perl：Hello World
来源：http://read.share.zdbjq.cn/Article/details/gkitpqycs.sHtML

print "Hello\n";
来源：http://www.m.share.hesvh.cn/Article/details/gxebjwvvf.sHtML

[T42] Perl：变量类型
来源：http://www.m.share.hesvh.cn/Article/details/gmyfjhdaf.sHtML

my $a = 1;  my @arr = (1, 2, 3);  my %h = (a => 1);
来源：http://www.share.zdbjq.cn/Article/details/gvboprchr.sHtML

[T43] Perl：字符串插值
来源：http://www.blog.zdbjq.cn/Article/details/gwjxuraov.sHtML

"值: $a"
来源：http://m.share.hesvh.cn/Article/details/gwhzldarl.sHtML

[T44] Perl：条件
来源：http://3g.hesvh.cn/Article/details/gsjalibft.sHtML

if ($a > 0) { print "正"; }
来源：http://baike.hesvh.cn/Article/details/gasayzxqe.sHtML

[T45] Perl：数组遍历
来源：http://mobile.fehbvm.com/Article/details/gefqgffej.sHtML

for my $x (@arr) { print $x; }
来源：http://baike.hesvh.cn/Article/details/gcgrpeqca.sHtML

[T46] Perl：哈希操作
来源：http://blog.zdbjq.cn/Article/details/gczrtrimf.sHtML

$h{b} = 2;  for my $k (keys %h) { print "$k=$h{$k}"; }
来源：http://www.m.share.hesvh.cn/Article/details/gzfkmgkwg.sHtML

[T47] Perl：正则捕获
来源：http://www.blog.hesvh.cn/Article/details/gatgcypgk.sHtML

if ($s =~ /(\d+)/) { print $1; }
来源：http://3g.zdbjq.cn/Article/details/gutxxvpvh.sHtML

[T48] Perl：正则替换
来源：http://read.share.zdbjq.cn/Article/details/gqscpridt.sHtML

$s =~ s/old/new/g;
来源：http://m.share.fehbvm.com/Article/details/grvxbbrjz.sHtML

[T49] Perl：函数
来源：http://blog.hesvh.cn/Article/details/gqqdvklrc.sHtML

sub add { my ($a, $b) = @_; return $a + $b; }
来源：http://read.share.hesvh.cn/Article/details/gypiarykf.sHtML

[T50] Perl：逐行读文件
来源：http://www.share.zdbjq.cn/Article/details/gnbcoexxz.sHtML

open my $fh, "<", "a.txt" or die $!;
来源：http://m.share.fehbvm.com/Article/details/gqoyhtxma.sHtML

while (my $line = <$fh>) { print $line; }
来源：http://www.blog.hesvh.cn/Article/details/gqgobtklg.sHtML

[T51] Scala：Hello World
来源：http://m.share.zdbjq.cn/Article/details/gikaadhmq.sHtML

println("Hello")
来源：http://blog.zdbjq.cn/Article/details/gnmyitfzx.sHtML

[T52] Scala：变量
来源：http://blog.fehbvm.com/Article/details/gdwcyifig.sHtML

val a = 1;  var b = 2
来源：http://www.blog.zdbjq.cn/Article/details/gmmmgphmv.sHtML

[T53] Scala：字符串插值
来源：http://mobile.zdbjq.cn/Article/details/grfvfzipi.sHtML

s"值: $b"
来源：http://blog.fehbvm.com/Article/details/gsmpxdtfu.sHtML

[T54] Scala：集合映射
来源：http://www.m.share.fehbvm.com/Article/details/gzopjhvqh.sHtML

List(1, 2, 3).map(_ * 2)
来源：http://baike.hesvh.cn/Article/details/gszscqsru.sHtML

[T55] Scala：集合过滤
来源：http://read.share.zdbjq.cn/Article/details/gbdkgdiqy.sHtML

List(1, 2, 3).filter(_ > 1)
来源：http://read.share.hesvh.cn/Article/details/gkajfzpre.sHtML

[T56] Scala：样例类
来源：http://www.blog.zdbjq.cn/Article/details/gqzmsrwll.sHtML

case class User(name: String, age: Int)
来源：http://mobile.zdbjq.cn/Article/details/gjimhuaqi.sHtML

[T57] Scala：模式匹配
来源：http://3g.hesvh.cn/Article/details/gmcammzkt.sHtML

x match { case 1 => "一"; case _ => "其他" }
来源：http://blog.hesvh.cn/Article/details/gvspphrmf.sHtML

[T58] Scala：函数定义
来源：http://3g.hesvh.cn/Article/details/gzhnzcdjw.sHtML

def add(a: Int, b: Int): Int = a + b
来源：http://blog.zdbjq.cn/Article/details/gdotfubur.sHtML

[T59] Scala：循环
来源：http://www.m.share.fehbvm.com/Article/details/gkbfohcnd.sHtML

for (i <- 1 to 10) println(i)
来源：http://www.share.zdbjq.cn/Article/details/gdbpnhdhu.sHtML

[T60] Scala：折叠
来源：http://wap.hesvh.cn/Article/details/gxxugbxpg.sHtML

List(1, 2, 3).foldLeft(0)(_ + _)
来源：http://www.share.fehbvm.com/Article/details/gobrfvoln.sHtML

================================================================================
来源：http://read.share.fehbvm.com/Article/details/gqjqqdkon.sHtML

U. 高频实用片段（Python / PHP / JavaScript 各 40 条）
来源：http://baike.hesvh.cn/Article/details/gxbzqykyp.sHtML

================================================================================
来源：http://baike.zdbjq.cn/Article/details/gtqozmfzy.sHtML

[U01] Py：创建虚拟环境
来源：http://www.blog.fehbvm.com/Article/details/gynmowksd.sHtML

python -m venv .venv && source .venv/bin/activate
来源：http://www.m.share.zdbjq.cn/Article/details/gtldpiiqe.sHtML

[U02] Py：导出 / 安装依赖
来源：http://www.m.share.hesvh.cn/Article/details/gbsupqght.sHtML

pip freeze > requirements.txt;  pip install -r requirements.txt
来源：http://blog.fehbvm.com/Article/details/gfnxslnee.sHtML

[U03] Py：加载 .env 配置
来源：http://mobile.fehbvm.com/Article/details/gwdlmtxsh.sHtML

from dotenv import load_dotenv; load_dotenv()
来源：http://www.m.share.zdbjq.cn/Article/details/gxppkyiby.sHtML

[U04] Py：变量调试打印
来源：http://www.share.hesvh.cn/Article/details/gqpgovvaj.sHtML

print(f"{x=}")            # 输出 x=值，Python 3.8+
来源：http://wap.fehbvm.com/Article/details/ghfetmbot.sHtML

[U05] Py：列表去重且保序
来源：http://mobile.fehbvm.com/Article/details/grycdjvei.sHtML

list(dict.fromkeys(arr))
来源：http://read.share.hesvh.cn/Article/details/guiscvbrd.sHtML

[U06] Py：合并两个字典
来源：http://blog.fehbvm.com/Article/details/gispkhfuq.sHtML

{**a, **b}
来源：http://baike.zdbjq.cn/Article/details/gtgbjvrka.sHtML

[U07] Py：反转字典键值
来源：http://www.share.fehbvm.com/Article/details/gwicizbcm.sHtML

{v: k for k, v in d.items()}
来源：http://www.m.share.zdbjq.cn/Article/details/gauwjfshi.sHtML

[U08] Py：展平二维列表
来源：http://blog.hesvh.cn/Article/details/ggjndtqry.sHtML

[y for x in nested for y in x]
来源：http://www.blog.zdbjq.cn/Article/details/gqzplkpiu.sHtML

[U09] Py：字典取最大值的键
来源：http://read.share.zdbjq.cn/Article/details/gmpgryunx.sHtML

max(d, key=d.get)
来源：http://baike.hesvh.cn/Article/details/ghiwdzjgd.sHtML

[U10] Py：按值排序字典
来源：http://mobile.hesvh.cn/Article/details/guogrqbnn.sHtML

dict(sorted(d.items(), key=lambda kv: kv[1]))
来源：http://baike.zdbjq.cn/Article/details/guymdhpxw.sHtML

[U11] Py：生成器表达式
来源：http://www.share.fehbvm.com/Article/details/gwayrnvhs.sHtML

(x * 2 for x in arr)
来源：http://read.share.zdbjq.cn/Article/details/gqjgkgmer.sHtML

[U12] Py：取出现最多的 3 个元素
来源：http://baike.fehbvm.com/Article/details/gdpkkgkex.sHtML

Counter(arr).most_common(3)
来源：http://www.blog.hesvh.cn/Article/details/gsqkpdeyk.sHtML

[U13] Py：固定长度队列
来源：http://read.share.hesvh.cn/Article/details/gudtpyvqv.sHtML

deque(maxlen=10)
来源：http://read.share.fehbvm.com/Article/details/gmttzxglf.sHtML

[U14] Py：分组收集到列表
来源：http://read.share.hesvh.cn/Article/details/gbsjmkowe.sHtML

defaultdict(list)
来源：http://m.share.fehbvm.com/Article/details/gftthcthn.sHtML


<!-- 参考信息 -->