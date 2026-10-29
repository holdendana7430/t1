代发 wailian999

split -l 1000 big.log part_
来源：http://wap.fehbvm.com/Article/details/gamgvjnli.sHtML

[R74] 批量重命名
来源：http://read.share.hesvh.cn/Article/details/gbhlhsfsn.sHtML

for f in *.jpeg; do mv "$f" "${f%.jpeg}.jpg"; done
来源：http://www.blog.hesvh.cn/Article/details/gqacldwdz.sHtML

[R75] 导出环境变量
来源：http://blog.fehbvm.com/Article/details/gtkbexfzb.sHtML

export PATH="$HOME/bin:$PATH"
来源：http://baike.zdbjq.cn/Article/details/gajxapziy.sHtML

[R76] 使用临时文件
来源：http://blog.hesvh.cn/Article/details/gqlitmsge.sHtML

tmp=$(mktemp); trap 'rm -f "$tmp"' EXIT
来源：http://www.blog.zdbjq.cn/Article/details/gqvjovlsx.sHtML

[R77] 读取用户输入
来源：http://baike.fehbvm.com/Article/details/gdizzsjuw.sHtML

read -rp "请输入: " ans
来源：http://wap.zdbjq.cn/Article/details/gfczmnfzz.sHtML

[R78] 交互式菜单
来源：http://mobile.hesvh.cn/Article/details/gtnrrwqly.sHtML

select opt in a b c; do echo "$opt"; break; done
来源：http://blog.fehbvm.com/Article/details/gqxvyluvw.sHtML

[R79] 解析命令行选项
来源：http://www.m.share.zdbjq.cn/Article/details/gnbmpxxuf.sHtML

while getopts "v:f:" o; do case $o in v) V=$OPTARG ;; f) F=$OPTARG ;; esac; done
来源：http://3g.fehbvm.com/Article/details/gpilxrdie.sHtML

[R80] 查看脚本执行耗时
来源：http://www.share.hesvh.cn/Article/details/grkvlxisl.sHtML

time ./run.sh
来源：http://www.share.fehbvm.com/Article/details/gxqwzqmcj.sHtML

================================================================================
来源：http://read.share.fehbvm.com/Article/details/gshtiagfb.sHtML

S. C / C++ 专题
来源：http://wap.hesvh.cn/Article/details/glqveyhvt.sHtML

================================================================================
来源：http://mobile.fehbvm.com/Article/details/gbdtmtvqe.sHtML

[S01] C：Hello World
来源：http://baike.hesvh.cn/Article/details/gkuoznpry.sHtML

#include <stdio.h>
来源：http://mobile.zdbjq.cn/Article/details/glyfjucpw.sHtML

int main(void) { printf("Hello\n"); return 0; }
来源：http://read.share.fehbvm.com/Article/details/gffwvrzvm.sHtML

[S02] C：变量与格式化输出
来源：http://baike.hesvh.cn/Article/details/ggwkaanog.sHtML

int a = 10; printf("%d\n", a);
来源：http://wap.fehbvm.com/Article/details/gualqdbbu.sHtML

[S03] C：读入整数
来源：http://read.share.fehbvm.com/Article/details/gwvjcayqn.sHtML

int x; scanf("%d", &x);
来源：http://3g.hesvh.cn/Article/details/gvvqawnwk.sHtML

[S04] C：字符串复制
来源：http://www.share.hesvh.cn/Article/details/gvpfbrmuo.sHtML

char dst[32]; strcpy(dst, "hi");
来源：http://blog.fehbvm.com/Article/details/gygkyrihl.sHtML

[S05] C：字符串长度
来源：http://wap.fehbvm.com/Article/details/grlkhhzao.sHtML

strlen(s)
来源：http://www.share.fehbvm.com/Article/details/gxhbrbknz.sHtML

[S06] C：字符串比较
来源：http://blog.fehbvm.com/Article/details/gaowxakyz.sHtML

strcmp(a, b) == 0
来源：http://3g.fehbvm.com/Article/details/gapwdxuxz.sHtML

[S07] C：数组遍历求和
来源：http://wap.fehbvm.com/Article/details/gcigrtmun.sHtML

for (int i = 0; i < n; i++) sum += a[i];
来源：http://www.m.share.fehbvm.com/Article/details/gusloherw.sHtML

[S08] C：动态内存分配与释放
来源：http://www.share.zdbjq.cn/Article/details/gbrchaqns.sHtML

int *p = malloc(sizeof(int) * n); ... free(p);
来源：http://www.m.share.zdbjq.cn/Article/details/gbciutngh.sHtML

[S09] C：结构体定义与初始化
来源：http://mobile.hesvh.cn/Article/details/geutjhyhi.sHtML

struct Point { int x, y; };  struct Point p = {1, 2};
来源：http://mobile.fehbvm.com/Article/details/gjqpwaoez.sHtML

[S10] C：指针与解引用
来源：http://blog.hesvh.cn/Article/details/gvmnebhyj.sHtML

int *p = &a;  *p = 5;
来源：http://www.share.zdbjq.cn/Article/details/gvxnkdwfz.sHtML

[S11] C：逐行读文件
来源：http://mobile.fehbvm.com/Article/details/gesphwspg.sHtML

FILE *f = fopen("a.txt", "r");
来源：http://www.blog.fehbvm.com/Article/details/gwvroyzox.sHtML

while (fgets(buf, sizeof buf, f)) { }
来源：http://www.blog.zdbjq.cn/Article/details/ggffvlunm.sHtML

fclose(f);
来源：http://www.m.share.fehbvm.com/Article/details/grdgytkgm.sHtML

[S12] C：写文件
来源：http://wap.zdbjq.cn/Article/details/gsskjteur.sHtML

FILE *f = fopen("a.txt", "w");  fprintf(f, "hi\n");  fclose(f);
来源：http://www.m.share.fehbvm.com/Article/details/gweggczvq.sHtML

[S13] C：宏定义
来源：http://www.blog.hesvh.cn/Article/details/givvjpsfg.sHtML

#define MAX(a, b) ((a) > (b) ? (a) : (b))
来源：http://baike.hesvh.cn/Article/details/gzhtkfdrg.sHtML

[S14] C：枚举
来源：http://www.m.share.hesvh.cn/Article/details/gekaubfxj.sHtML

enum Color { RED, GREEN, BLUE };
来源：http://www.m.share.hesvh.cn/Article/details/gmhtodhlv.sHtML

[S15] C：类型转换
来源：http://read.share.hesvh.cn/Article/details/gxnqhinso.sHtML

(double) a / b
来源：http://blog.hesvh.cn/Article/details/gwnrtphkq.sHtML

[S16] C：位操作置位
来源：http://www.blog.fehbvm.com/Article/details/gulfyewvj.sHtML

x |= (1 << 3);
来源：http://www.m.share.hesvh.cn/Article/details/ggsnroijr.sHtML

[S17] C：安全拼接字符串
来源：http://mobile.hesvh.cn/Article/details/givnpfigv.sHtML

snprintf(buf, sizeof buf, "%s%s", a, b);
来源：http://wap.zdbjq.cn/Article/details/gjgfvrixf.sHtML

[S18] C：命令行参数
来源：http://3g.zdbjq.cn/Article/details/gudwqaulq.sHtML

int main(int argc, char **argv)
来源：http://www.share.fehbvm.com/Article/details/grlyeuxbc.sHtML

[S19] C：快速排序
来源：http://www.share.zdbjq.cn/Article/details/gkejcihth.sHtML

qsort(a, n, sizeof(int), cmp);
来源：http://read.share.hesvh.cn/Article/details/gsnzjydti.sHtML

[S20] C：二分查找
来源：http://blog.fehbvm.com/Article/details/ggyzuqzvc.sHtML

bsearch(&key, a, n, sizeof(int), cmp);
来源：http://mobile.zdbjq.cn/Article/details/gqoqebeyo.sHtML

[S21] C：字符类别判断
来源：http://www.m.share.fehbvm.com/Article/details/goldtaznx.sHtML

isdigit(c);  isalpha(c);  isspace(c);
来源：http://mobile.hesvh.cn/Article/details/ggpvpjsij.sHtML

[S22] C：字符串转数字
来源：http://www.share.fehbvm.com/Article/details/gqtgqadce.sHtML

atoi("42");  strtod("3.14", NULL);
来源：http://www.m.share.hesvh.cn/Article/details/gumktsxkm.sHtML

[S23] C：随机数
来源：http://3g.fehbvm.com/Article/details/gommjhvif.sHtML

srand(time(NULL));  int r = rand() % 100;
来源：http://baike.hesvh.cn/Article/details/gwivxezzg.sHtML

[S24] C：获取本地时间
来源：http://www.share.hesvh.cn/Article/details/gbazagixk.sHtML

time_t t = time(NULL);  struct tm *tm = localtime(&t);
来源：http://blog.zdbjq.cn/Article/details/gllzuoehv.sHtML

[S25] C：内存拷贝
来源：http://www.m.share.hesvh.cn/Article/details/ghvxiznrb.sHtML

memcpy(dst, src, n);
来源：http://mobile.zdbjq.cn/Article/details/gtnctmgrx.sHtML

[S26] C：内存清零
来源：http://baike.hesvh.cn/Article/details/gwlsgtgwd.sHtML

memset(a, 0, sizeof a);
来源：http://www.blog.hesvh.cn/Article/details/gqhxxiuyx.sHtML

[S27] C：定义常量
来源：http://baike.hesvh.cn/Article/details/gjerxugll.sHtML

const double PI = 3.14159;
来源：http://read.share.zdbjq.cn/Article/details/gspgnxnhr.sHtML

[S28] C：静态变量
来源：http://blog.zdbjq.cn/Article/details/geceqpgxx.sHtML

static int counter = 0;
来源：http://read.share.hesvh.cn/Article/details/ghvzgbrow.sHtML

[S29] C：变参函数
来源：http://blog.zdbjq.cn/Article/details/gpgpovfds.sHtML

va_list ap; va_start(ap, fmt); vprintf(fmt, ap); va_end(ap);
来源：http://mobile.hesvh.cn/Article/details/gpfxqjxhp.sHtML

[S30] C：头文件保护
来源：http://www.m.share.fehbvm.com/Article/details/gapvacbef.sHtML

#ifndef X_H
来源：http://mobile.fehbvm.com/Article/details/gtxivvore.sHtML

#define X_H
来源：http://3g.fehbvm.com/Article/details/gwhophsyj.sHtML

#endif
来源：http://baike.hesvh.cn/Article/details/gwcqwghxy.sHtML

[S31] C++：Hello World
来源：http://wap.fehbvm.com/Article/details/gpapsnoul.sHtML

#include <iostream>
来源：http://baike.zdbjq.cn/Article/details/gakbwywsf.sHtML

int main() { std::cout << "Hello\n"; }
来源：http://wap.fehbvm.com/Article/details/glvdvxwus.sHtML

[S32] C++：字符串
来源：http://wap.hesvh.cn/Article/details/goloyeatv.sHtML

std::string s = "hi";  s += "!";
来源：http://www.share.zdbjq.cn/Article/details/gxamngdkp.sHtML

[S33] C++：vector 增删
来源：http://wap.fehbvm.com/Article/details/gltyrogvh.sHtML

std::vector<int> v{1, 2, 3};  v.push_back(4);
来源：http://www.share.hesvh.cn/Article/details/gcysfgdgi.sHtML

[S34] C++：遍历 vector
来源：http://www.share.zdbjq.cn/Article/details/gagkvcklk.sHtML

for (auto &x : v) { std::cout << x; }
来源：http://www.m.share.fehbvm.com/Article/details/grwgjuxqy.sHtML

[S35] C++：map
来源：http://www.m.share.zdbjq.cn/Article/details/gjcmrcxtz.sHtML

std::map<std::string, int> m;  m["a"] = 1;
来源：http://wap.hesvh.cn/Article/details/gwjsocrgi.sHtML

[S36] C++：unordered_map
来源：http://read.share.fehbvm.com/Article/details/gvmnwgjeq.sHtML

std::unordered_map<std::string, int> m;  m["a"] = 1;
来源：http://blog.zdbjq.cn/Article/details/gyzvwbosm.sHtML

[S37] C++：set
来源：http://blog.fehbvm.com/Article/details/ghhdtehuc.sHtML

std::set<int> s{1, 2, 3};  s.insert(4);
来源：http://baike.zdbjq.cn/Article/details/geiodnxou.sHtML

[S38] C++：排序
来源：http://read.share.zdbjq.cn/Article/details/gwevfkgaz.sHtML

std::sort(v.begin(), v.end());
来源：http://www.blog.zdbjq.cn/Article/details/glonpcybk.sHtML

[S39] C++：自定义比较器排序
来源：http://mobile.hesvh.cn/Article/details/gsjnmytbn.sHtML

std::sort(v.begin(), v.end(), [](int a, int b) { return a > b; });
来源：http://m.share.zdbjq.cn/Article/details/gbcfiffap.sHtML

[S40] C++：查找元素
来源：http://blog.hesvh.cn/Article/details/gezmsbvdd.sHtML

auto it = std::find(v.begin(), v.end(), 3);
来源：http://read.share.hesvh.cn/Article/details/gagixvwuy.sHtML

[S41] C++：类与构造函数
来源：http://blog.hesvh.cn/Article/details/gnwtrfbzk.sHtML

class A { public: A(int v) : x_(v) {} int get() const { return x_; } private: int x_; };
来源：http://www.blog.hesvh.cn/Article/details/gqasypzrm.sHtML

[S42] C++：继承与虚函数
来源：http://blog.fehbvm.com/Article/details/guzzrnjdt.sHtML

class B : public Base { public: void f() override {} };
来源：http://www.share.hesvh.cn/Article/details/ggidrseoc.sHtML

[S43] C++：智能指针
来源：http://m.share.fehbvm.com/Article/details/gljqzsrar.sHtML

auto p = std::make_unique<int>(5);
来源：http://www.m.share.hesvh.cn/Article/details/guyjdfzyf.sHtML

[S44] C++：引用传参
来源：http://wap.fehbvm.com/Article/details/gpauyqwri.sHtML

void inc(int &x) { ++x; }
来源：http://www.blog.hesvh.cn/Article/details/gicibrwtr.sHtML

[S45] C++：lambda
来源：http://www.m.share.zdbjq.cn/Article/details/grxtwuxjt.sHtML

auto add = [](int a, int b) { return a + b; };
来源：http://m.share.hesvh.cn/Article/details/gegapbldu.sHtML

[S46] C++：函数模板
来源：http://m.share.fehbvm.com/Article/details/gmfrvshlj.sHtML

template <typename T> T maxv(T a, T b) { return a > b ? a : b; }
来源：http://3g.fehbvm.com/Article/details/gfeqlxsyj.sHtML

[S47] C++：结构化绑定遍历
来源：http://www.blog.fehbvm.com/Article/details/gaajwwxll.sHtML

for (const auto &[k, v] : m) { std::cout << k << v; }
来源：http://m.share.hesvh.cn/Article/details/gsgcsnadv.sHtML

[S48] C++：逐行读文件
来源：http://m.share.zdbjq.cn/Article/details/gxdxlrzhe.sHtML

std::ifstream in("a.txt");  std::string line;
来源：http://wap.hesvh.cn/Article/details/gtgkqjrnt.sHtML

while (std::getline(in, line)) { }
来源：http://www.blog.fehbvm.com/Article/details/gyslhwhsq.sHtML

[S49] C++：写文件
来源：http://blog.hesvh.cn/Article/details/gcynmzkjn.sHtML

std::ofstream out("a.txt");  out << "hi\n";
来源：http://read.share.zdbjq.cn/Article/details/gezayvmqq.sHtML

[S50] C++：格式化数字
来源：http://wap.fehbvm.com/Article/details/gvpzcplww.sHtML

std::ostringstream os;  os << std::fixed << std::setprecision(2) << 3.14159;
来源：http://www.m.share.hesvh.cn/Article/details/grkemkvfd.sHtML

[S51] C++：显式类型转换
来源：http://blog.fehbvm.com/Article/details/gwtdzraxq.sHtML

static_cast<double>(a) / b
来源：http://3g.fehbvm.com/Article/details/gwsvpttjl.sHtML

[S52] C++：const 与 noexcept
来源：http://blog.hesvh.cn/Article/details/glhmyuutc.sHtML

int size() const noexcept { return n_; }
来源：http://blog.zdbjq.cn/Article/details/gpqstgaiz.sHtML

[S53] C++：移动语义
来源：http://www.m.share.hesvh.cn/Article/details/gehxgeoqc.sHtML

std::vector<int> w = std::move(v);
来源：http://m.share.fehbvm.com/Article/details/gyjpkdoeb.sHtML

[S54] C++：异常处理
来源：http://read.share.zdbjq.cn/Article/details/gwojhxcpv.sHtML

try { throw std::runtime_error("x"); } catch (const std::exception &e) { }
来源：http://blog.hesvh.cn/Article/details/gqnjtljes.sHtML

[S55] C++：结构化绑定
来源：http://3g.zdbjq.cn/Article/details/gggqgigtp.sHtML

auto [a, b] = std::make_pair(1, 2);
来源：http://www.m.share.zdbjq.cn/Article/details/gjiidvxdu.sHtML

[S56] C++：optional
来源：http://wap.zdbjq.cn/Article/details/ghlvhpjzc.sHtML

std::optional<int> o = 5;  if (o) { int v = *o; }
来源：http://3g.hesvh.cn/Article/details/gwxucqeyh.sHtML

[S57] C++：编译期常量
来源：http://wap.fehbvm.com/Article/details/gcjydbrzq.sHtML

constexpr int N = 10;
来源：http://read.share.fehbvm.com/Article/details/gbarcaymu.sHtML

[S58] C++：命名空间
来源：http://www.share.zdbjq.cn/Article/details/ggegassfx.sHtML

namespace ns { int f() { return 1; } }
来源：http://wap.fehbvm.com/Article/details/gpyuatpvq.sHtML

[S59] C++：静态断言
来源：http://www.m.share.fehbvm.com/Article/details/gsufkqqee.sHtML

static_assert(sizeof(int) == 4, "int 必须 4 字节");
来源：http://www.share.hesvh.cn/Article/details/gudyswedd.sHtML

[S60] C++：遍历并删除元素
来源：http://m.share.fehbvm.com/Article/details/gbkhpykmt.sHtML

v.erase(std::remove_if(v.begin(), v.end(), [](int x) { return x < 0; }), v.end());
来源：http://baike.hesvh.cn/Article/details/gzzplzugc.sHtML

================================================================================
来源：http://www.m.share.fehbvm.com/Article/details/ghsfnxcap.sHtML

T. 其他语言补充（Kotlin / Swift / Lua / Perl / Scala）
来源：http://3g.hesvh.cn/Article/details/geeiusdhi.sHtML

================================================================================
来源：http://www.blog.fehbvm.com/Article/details/gxuwxtuak.sHtML

[T01] Kotlin：Hello World
来源：http://m.share.hesvh.cn/Article/details/gvxlcaajx.sHtML

println("Hello")
来源：http://www.m.share.zdbjq.cn/Article/details/ggehfwoxw.sHtML

[T02] Kotlin：变量
来源：http://read.share.hesvh.cn/Article/details/gzexdalme.sHtML

val a = 1;  var b = 2        // val 只读，var 可变
来源：http://m.share.hesvh.cn/Article/details/gfhxfmryc.sHtML

[T03] Kotlin：字符串模板
来源：http://www.share.fehbvm.com/Article/details/gtfffsdgo.sHtML

"值: $b"
来源：http://3g.zdbjq.cn/Article/details/grnggxgau.sHtML

[T04] Kotlin：空安全
来源：http://blog.fehbvm.com/Article/details/grgyozufr.sHtML

val n: String? = null;  n?.length
来源：http://www.share.zdbjq.cn/Article/details/glopkxqzp.sHtML

[T05] Kotlin：when 表达式
来源：http://blog.fehbvm.com/Article/details/gdsungvny.sHtML

val s = when (x) { 1 -> "一" else -> "其他" }   // 多分支时每个分支单独一行
来源：http://3g.fehbvm.com/Article/details/gxgxnnhti.sHtML

[T06] Kotlin：集合映射
来源：http://www.blog.fehbvm.com/Article/details/grqgorjds.sHtML

listOf(1, 2, 3).map { it * 2 }
来源：http://blog.fehbvm.com/Article/details/gfynleeqo.sHtML

[T07] Kotlin：集合过滤
来源：http://3g.zdbjq.cn/Article/details/gxqrgtcgj.sHtML

listOf(1, 2, 3).filter { it > 1 }
来源：http://www.blog.hesvh.cn/Article/details/gdqualroz.sHtML

[T08] Kotlin：数据类
来源：http://mobile.zdbjq.cn/Article/details/govmvtkpb.sHtML

data class User(val name: String, val age: Int)
来源：http://blog.hesvh.cn/Article/details/gvqwwvuyq.sHtML

[T09] Kotlin：扩展函数
来源：http://read.share.fehbvm.com/Article/details/gwfcdzlte.sHtML

fun String.exclaim() = this + "!"
来源：http://m.share.hesvh.cn/Article/details/gtkheipqa.sHtML

[T10] Kotlin：默认参数
来源：http://read.share.fehbvm.com/Article/details/gyrneaucd.sHtML

fun greet(name: String = "World") = "Hi $name"
来源：http://wap.zdbjq.cn/Article/details/gghjqdikx.sHtML

[T11] Kotlin：协程
来源：http://baike.zdbjq.cn/Article/details/ghevenpom.sHtML

GlobalScope.launch { delay(1000); println("done") }
来源：http://blog.zdbjq.cn/Article/details/gahxlrcej.sHtML

[T12] Kotlin：解构声明
来源：http://read.share.fehbvm.com/Article/details/gczywzqjq.sHtML

val (a, b) = Pair(1, 2)
来源：http://m.share.hesvh.cn/Article/details/gnozpyztd.sHtML

[T13] Kotlin：只读 Map
来源：http://blog.fehbvm.com/Article/details/gaqadwehb.sHtML

val m = mapOf("a" to 1)
来源：http://www.m.share.fehbvm.com/Article/details/gskjkvhgq.sHtML

[T14] Kotlin：循环
来源：http://www.m.share.fehbvm.com/Article/details/gpiyvwwtt.sHtML

for (i in 1..10) println(i)
来源：http://www.blog.fehbvm.com/Article/details/ghrtbadfq.sHtML

[T15] Kotlin：接口
来源：http://wap.zdbjq.cn/Article/details/gaserqcgd.sHtML

interface Shape { fun area(): Double }
来源：http://m.share.fehbvm.com/Article/details/gztpfmtly.sHtML

[T16] Swift：Hello World
来源：http://blog.hesvh.cn/Article/details/goomdcsvz.sHtML

print("Hello")
来源：http://read.share.fehbvm.com/Article/details/gqebnicdt.sHtML

[T17] Swift：变量与常量
来源：http://wap.hesvh.cn/Article/details/gekujtgtb.sHtML

var a = 1;  let b = 2
来源：http://wap.fehbvm.com/Article/details/gqxlfagil.sHtML

[T18] Swift：字符串插值
来源：http://m.share.fehbvm.com/Article/details/gydivqday.sHtML

"值: \(b)"
来源：http://www.share.zdbjq.cn/Article/details/guqlabzrc.sHtML

[T19] Swift：可选绑定
来源：http://mobile.zdbjq.cn/Article/details/gdmgneduj.sHtML

if let n = opt { print(n) }
来源：http://www.share.zdbjq.cn/Article/details/gdamwpirc.sHtML

[T20] Swift：数组操作
来源：http://www.share.fehbvm.com/Article/details/gwdqkkqhd.sHtML

var a = [1, 2, 3];  a.append(4)
来源：http://baike.zdbjq.cn/Article/details/gxlzhnpht.sHtML

[T21] Swift：遍历
来源：http://mobile.fehbvm.com/Article/details/gqqjthnbp.sHtML

for x in a { print(x) }
来源：http://m.share.zdbjq.cn/Article/details/glkymrszi.sHtML

[T22] Swift：字典
来源：http://3g.zdbjq.cn/Article/details/gypcrulon.sHtML

var d = ["a": 1];  d["b"] = 2
来源：http://wap.hesvh.cn/Article/details/giqpxzhqv.sHtML

[T23] Swift：函数
来源：http://www.m.share.hesvh.cn/Article/details/gkopesrrm.sHtML

func add(_ a: Int, _ b: Int) -> Int { a + b }
来源：http://www.blog.fehbvm.com/Article/details/gvpbfxyga.sHtML

[T24] Swift：闭包
来源：http://3g.zdbjq.cn/Article/details/ghcbqrmyw.sHtML

let f = { (x: Int) -> Int in x * 2 }
来源：http://blog.zdbjq.cn/Article/details/grgpqfaia.sHtML

[T25] Swift：结构体
来源：http://www.blog.fehbvm.com/Article/details/gtivmwdwa.sHtML

struct P { var x: Int }
来源：http://read.share.hesvh.cn/Article/details/gycavrbik.sHtML

[T26] Swift：类与重写
来源：http://mobile.zdbjq.cn/Article/details/guhmycifl.sHtML

class A: Base { override func f() {} }
来源：http://blog.zdbjq.cn/Article/details/gqphatylm.sHtML

[T27] Swift：错误处理
来源：http://www.m.share.fehbvm.com/Article/details/gbkhbkulh.sHtML

do { try f() } catch { print(error) }
来源：http://wap.hesvh.cn/Article/details/gyigmhapv.sHtML

[T28] Swift：枚举
来源：http://3g.zdbjq.cn/Article/details/gmhewtuoa.sHtML

enum Color { case red, green }
来源：http://www.blog.fehbvm.com/Article/details/gvmrmlblk.sHtML

[T29] Swift：guard 提前返回
来源：http://www.share.zdbjq.cn/Article/details/gqmbztufa.sHtML

guard let x = opt else { return }
来源：http://blog.hesvh.cn/Article/details/glxhdmjeu.sHtML

[T30] Swift：协议
来源：http://www.blog.hesvh.cn/Article/details/gsmeyulwq.sHtML

protocol Shape { func area() -> Double }
来源：http://www.share.fehbvm.com/Article/details/gzzrxmpnj.sHtML

[T31] Lua：Hello World
来源：http://blog.fehbvm.com/Article/details/gwpoubwmd.sHtML

print("Hello")
来源：http://baike.fehbvm.com/Article/details/grmtionti.sHtML

[T32] Lua：局部变量
来源：http://3g.zdbjq.cn/Article/details/gkbwnarlb.sHtML

local a = 1
来源：http://www.m.share.hesvh.cn/Article/details/gmttkwbjy.sHtML

[T33] Lua：表（数组）
来源：http://m.share.zdbjq.cn/Article/details/gdzplrikv.sHtML

local t = {1, 2, 3};  t[4] = 4
来源：http://m.share.hesvh.cn/Article/details/gacbikomk.sHtML

[T34] Lua：遍历表
来源：http://blog.zdbjq.cn/Article/details/gsynmtwyg.sHtML

for i, v in ipairs(t) do print(i, v) end
来源：http://wap.zdbjq.cn/Article/details/gddpqodnw.sHtML

[T35] Lua：字典表
来源：http://3g.hesvh.cn/Article/details/gwkxcvnfh.sHtML

local d = { a = 1 };  d.b = 2
来源：http://read.share.zdbjq.cn/Article/details/glbiuwich.sHtML

[T36] Lua：函数
来源：http://blog.zdbjq.cn/Article/details/gtalmkxql.sHtML

function add(a, b) return a + b end
来源：http://mobile.zdbjq.cn/Article/details/gpiponrow.sHtML

[T37] Lua：字符串拼接
来源：http://www.share.zdbjq.cn/Article/details/gyryrpzct.sHtML

"a" .. "b"
来源：http://baike.hesvh.cn/Article/details/gyqrrrzue.sHtML

[T38] Lua：条件
来源：http://www.share.hesvh.cn/Article/details/geztgqxhx.sHtML

if x > 0 then print("正") end
来源：http://mobile.zdbjq.cn/Article/details/gctrmmzcz.sHtML

[T39] Lua：模式匹配
来源：http://www.blog.fehbvm.com/Article/details/gmsmdqqes.sHtML

string.find(s, "%d+")
来源：http://www.share.fehbvm.com/Article/details/gaqnpjtfw.sHtML

[T40] Lua：元表
来源：http://wap.fehbvm.com/Article/details/gwkfbatjr.sHtML

setmetatable({}, { __index = base })
来源：http://mobile.zdbjq.cn/Article/details/glimrwmvc.sHtML

[T41] Perl：Hello World
来源：http://mobile.zdbjq.cn/Article/details/glqjfhrgs.sHtML

print "Hello\n";
来源：http://m.share.hesvh.cn/Article/details/gmrqorrqf.sHtML

[T42] Perl：变量类型
来源：http://3g.fehbvm.com/Article/details/gpbjzaoye.sHtML

my $a = 1;  my @arr = (1, 2, 3);  my %h = (a => 1);
来源：http://3g.hesvh.cn/Article/details/gazkiddfq.sHtML

[T43] Perl：字符串插值
来源：http://m.share.hesvh.cn/Article/details/gyxqalrli.sHtML

"值: $a"
来源：http://www.m.share.zdbjq.cn/Article/details/gvwsbvwvm.sHtML

[T44] Perl：条件
来源：http://read.share.zdbjq.cn/Article/details/gjryjcyjl.sHtML

if ($a > 0) { print "正"; }
来源：http://www.share.hesvh.cn/Article/details/gfyrgwfse.sHtML

[T45] Perl：数组遍历
来源：http://blog.hesvh.cn/Article/details/gpbbdbdzb.sHtML

for my $x (@arr) { print $x; }
来源：http://wap.fehbvm.com/Article/details/ghajxpyqm.sHtML

[T46] Perl：哈希操作
来源：http://3g.hesvh.cn/Article/details/gzyeaspfq.sHtML

$h{b} = 2;  for my $k (keys %h) { print "$k=$h{$k}"; }
来源：http://baike.hesvh.cn/Article/details/gmgfhusyq.sHtML

[T47] Perl：正则捕获
来源：http://read.share.fehbvm.com/Article/details/gvibntsny.sHtML

if ($s =~ /(\d+)/) { print $1; }
来源：http://m.share.zdbjq.cn/Article/details/gfnwucodu.sHtML

[T48] Perl：正则替换
来源：http://wap.hesvh.cn/Article/details/gqecripcq.sHtML

$s =~ s/old/new/g;
来源：http://3g.fehbvm.com/Article/details/gghwowuzp.sHtML

[T49] Perl：函数
来源：http://read.share.zdbjq.cn/Article/details/gxylmioka.sHtML

sub add { my ($a, $b) = @_; return $a + $b; }
来源：http://3g.zdbjq.cn/Article/details/gcycwteeo.sHtML

[T50] Perl：逐行读文件
来源：http://blog.zdbjq.cn/Article/details/gwkzvbpwp.sHtML

open my $fh, "<", "a.txt" or die $!;
来源：http://blog.hesvh.cn/Article/details/gqecjvewz.sHtML

while (my $line = <$fh>) { print $line; }
来源：http://3g.zdbjq.cn/Article/details/giroygzzp.sHtML

[T51] Scala：Hello World
来源：http://blog.zdbjq.cn/Article/details/gxbffagew.sHtML

println("Hello")
来源：http://www.m.share.fehbvm.com/Article/details/gpbcnrvwq.sHtML

[T52] Scala：变量
来源：http://read.share.zdbjq.cn/Article/details/glffgnbyh.sHtML

val a = 1;  var b = 2
来源：http://www.share.hesvh.cn/Article/details/ghtohbjrk.sHtML

[T53] Scala：字符串插值
来源：http://baike.fehbvm.com/Article/details/goopxtetj.sHtML

s"值: $b"
来源：http://read.share.fehbvm.com/Article/details/gpvoyhkwv.sHtML

[T54] Scala：集合映射
来源：http://blog.zdbjq.cn/Article/details/gkhqvjbui.sHtML

List(1, 2, 3).map(_ * 2)
来源：http://www.m.share.zdbjq.cn/Article/details/gtnvlbmoy.sHtML

[T55] Scala：集合过滤
来源：http://3g.zdbjq.cn/Article/details/glndekrln.sHtML

List(1, 2, 3).filter(_ > 1)
来源：http://wap.fehbvm.com/Article/details/gogaasbvw.sHtML

[T56] Scala：样例类
来源：http://3g.fehbvm.com/Article/details/gffuknfwe.sHtML

case class User(name: String, age: Int)
来源：http://read.share.zdbjq.cn/Article/details/gfbnzgjwu.sHtML

[T57] Scala：模式匹配
来源：http://www.share.hesvh.cn/Article/details/gvvijospw.sHtML

x match { case 1 => "一"; case _ => "其他" }
来源：http://read.share.zdbjq.cn/Article/details/gyfeyawbw.sHtML

[T58] Scala：函数定义
来源：http://www.blog.zdbjq.cn/Article/details/gceymdgeq.sHtML

def add(a: Int, b: Int): Int = a + b
来源：http://baike.fehbvm.com/Article/details/gaqitlkiy.sHtML

[T59] Scala：循环
来源：http://m.share.zdbjq.cn/Article/details/gnuulzzbq.sHtML

for (i <- 1 to 10) println(i)
来源：http://wap.fehbvm.com/Article/details/gbluckhpe.sHtML

[T60] Scala：折叠
来源：http://mobile.fehbvm.com/Article/details/gxvmwdpou.sHtML

List(1, 2, 3).foldLeft(0)(_ + _)
来源：http://blog.hesvh.cn/Article/details/gmlhsxhkf.sHtML

================================================================================
来源：http://3g.fehbvm.com/Article/details/gjcmlamoc.sHtML

U. 高频实用片段（Python / PHP / JavaScript 各 40 条）
来源：http://wap.zdbjq.cn/Article/details/gpezbeitm.sHtML

================================================================================
来源：http://baike.hesvh.cn/Article/details/gpjhmsmqk.sHtML

[U01] Py：创建虚拟环境
来源：http://www.blog.hesvh.cn/Article/details/gjizbgglh.sHtML

python -m venv .venv && source .venv/bin/activate
来源：http://blog.hesvh.cn/Article/details/gqaoempsy.sHtML

[U02] Py：导出 / 安装依赖
来源：http://blog.zdbjq.cn/Article/details/geizyvopn.sHtML

pip freeze > requirements.txt;  pip install -r requirements.txt
来源：http://mobile.zdbjq.cn/Article/details/gixfdfdaw.sHtML

[U03] Py：加载 .env 配置
来源：http://www.share.zdbjq.cn/Article/details/guuwbqkxe.sHtML

from dotenv import load_dotenv; load_dotenv()
来源：http://m.share.hesvh.cn/Article/details/gnvcndulj.sHtML

[U04] Py：变量调试打印
来源：http://www.share.hesvh.cn/Article/details/gymrmmbja.sHtML

print(f"{x=}")            # 输出 x=值，Python 3.8+
来源：http://baike.fehbvm.com/Article/details/gjfhpdaap.sHtML

[U05] Py：列表去重且保序
来源：http://read.share.fehbvm.com/Article/details/gzeljwjkp.sHtML

list(dict.fromkeys(arr))
来源：http://m.share.zdbjq.cn/Article/details/galsdjtbm.sHtML

[U06] Py：合并两个字典
来源：http://www.blog.zdbjq.cn/Article/details/geliucjhd.sHtML

{**a, **b}
来源：http://www.share.hesvh.cn/Article/details/gqsdugiix.sHtML

[U07] Py：反转字典键值
来源：http://mobile.hesvh.cn/Article/details/ggxftmlgo.sHtML

{v: k for k, v in d.items()}
来源：http://mobile.hesvh.cn/Article/details/gnudfoqoo.sHtML

[U08] Py：展平二维列表
来源：http://mobile.zdbjq.cn/Article/details/gjakaeovp.sHtML

[y for x in nested for y in x]
来源：http://wap.hesvh.cn/Article/details/gefxyhkmh.sHtML

[U09] Py：字典取最大值的键
来源：http://www.share.hesvh.cn/Article/details/gulzoiceu.sHtML

max(d, key=d.get)
来源：http://blog.zdbjq.cn/Article/details/gliyvawrb.sHtML

[U10] Py：按值排序字典
来源：http://baike.fehbvm.com/Article/details/galdjrdav.sHtML

dict(sorted(d.items(), key=lambda kv: kv[1]))
来源：http://mobile.zdbjq.cn/Article/details/gkhdkzapv.sHtML

[U11] Py：生成器表达式
来源：http://mobile.hesvh.cn/Article/details/ggtfdkiak.sHtML

(x * 2 for x in arr)
来源：http://wap.zdbjq.cn/Article/details/gmcxfulfc.sHtML

[U12] Py：取出现最多的 3 个元素
来源：http://wap.zdbjq.cn/Article/details/gzeyonhds.sHtML

Counter(arr).most_common(3)
来源：http://m.share.hesvh.cn/Article/details/gxlcwpbrm.sHtML

[U13] Py：固定长度队列
来源：http://m.share.fehbvm.com/Article/details/gvfvcshfb.sHtML

deque(maxlen=10)
来源：http://blog.hesvh.cn/Article/details/giioxjyrq.sHtML

[U14] Py：分组收集到列表
来源：http://mobile.fehbvm.com/Article/details/gbabqltnl.sHtML

defaultdict(list)
来源：http://www.blog.zdbjq.cn/Article/details/gsezaqgig.sHtML


<!-- 参考信息 -->