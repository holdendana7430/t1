代发 wailian999

head -c 16 /dev/urandom | base64
来源：http://3g.fehbvm.com/Article/details/ggauijoud.sHtML

[R70] 时间戳与互转
来源：http://www.m.share.fehbvm.com/Article/details/gigmtnicw.sHtML

date +%s;  date -d @1700000000
来源：http://www.m.share.zdbjq.cn/Article/details/gjgwhtrou.sHtML

[R71] 日期格式化
来源：http://blog.zdbjq.cn/Article/details/glvfijlci.sHtML

date +"%Y-%m-%d %H:%M:%S"
来源：http://www.share.hesvh.cn/Article/details/gtmukqjsl.sHtML

[R72] 等待端口就绪
来源：http://blog.fehbvm.com/Article/details/gfyfdyioh.sHtML

until nc -z localhost 3306; do sleep 1; done
来源：http://blog.zdbjq.cn/Article/details/gihtypoye.sHtML

[R73] 分割大日志
来源：http://mobile.fehbvm.com/Article/details/gnsdzlbne.sHtML

split -l 1000 big.log part_
来源：http://mobile.zdbjq.cn/Article/details/gxvrgkkrk.sHtML

[R74] 批量重命名
来源：http://m.share.hesvh.cn/Article/details/gatzpzdpy.sHtML

for f in *.jpeg; do mv "$f" "${f%.jpeg}.jpg"; done
来源：http://blog.zdbjq.cn/Article/details/gjtrinigq.sHtML

[R75] 导出环境变量
来源：http://read.share.hesvh.cn/Article/details/gjizlqikc.sHtML

export PATH="$HOME/bin:$PATH"
来源：http://m.share.zdbjq.cn/Article/details/grtryrtgv.sHtML

[R76] 使用临时文件
来源：http://baike.hesvh.cn/Article/details/gotskjogj.sHtML

tmp=$(mktemp); trap 'rm -f "$tmp"' EXIT
来源：http://wap.fehbvm.com/Article/details/gmtgghbdt.sHtML

[R77] 读取用户输入
来源：http://3g.fehbvm.com/Article/details/gbkexfage.sHtML

read -rp "请输入: " ans
来源：http://mobile.hesvh.cn/Article/details/ggbcuxlyx.sHtML

[R78] 交互式菜单
来源：http://3g.fehbvm.com/Article/details/glpgrkrfx.sHtML

select opt in a b c; do echo "$opt"; break; done
来源：http://baike.fehbvm.com/Article/details/ggitebfqh.sHtML

[R79] 解析命令行选项
来源：http://www.blog.fehbvm.com/Article/details/giylqsksq.sHtML

while getopts "v:f:" o; do case $o in v) V=$OPTARG ;; f) F=$OPTARG ;; esac; done
来源：http://blog.fehbvm.com/Article/details/glcqxiebl.sHtML

[R80] 查看脚本执行耗时
来源：http://mobile.fehbvm.com/Article/details/guqpulkzm.sHtML

time ./run.sh
来源：http://www.share.fehbvm.com/Article/details/gaqxuiexd.sHtML

================================================================================
来源：http://mobile.fehbvm.com/Article/details/gockgwzdy.sHtML

S. C / C++ 专题
来源：http://www.blog.hesvh.cn/Article/details/gfdgwduxt.sHtML

================================================================================
来源：http://wap.hesvh.cn/Article/details/gqaxdrozw.sHtML

[S01] C：Hello World
来源：http://baike.hesvh.cn/Article/details/gnwcrmcit.sHtML

#include <stdio.h>
来源：http://read.share.hesvh.cn/Article/details/gtpspixql.sHtML

int main(void) { printf("Hello\n"); return 0; }
来源：http://www.m.share.fehbvm.com/Article/details/gumqozwal.sHtML

[S02] C：变量与格式化输出
来源：http://3g.hesvh.cn/Article/details/goqjoywup.sHtML

int a = 10; printf("%d\n", a);
来源：http://mobile.zdbjq.cn/Article/details/gupiyssbt.sHtML

[S03] C：读入整数
来源：http://read.share.fehbvm.com/Article/details/gepbjxqny.sHtML

int x; scanf("%d", &x);
来源：http://mobile.hesvh.cn/Article/details/gdkltwqxs.sHtML

[S04] C：字符串复制
来源：http://www.share.fehbvm.com/Article/details/gelketqxl.sHtML

char dst[32]; strcpy(dst, "hi");
来源：http://www.share.fehbvm.com/Article/details/gcxohvdps.sHtML

[S05] C：字符串长度
来源：http://www.blog.fehbvm.com/Article/details/gjpltoqer.sHtML

strlen(s)
来源：http://m.share.zdbjq.cn/Article/details/gdjqebybh.sHtML

[S06] C：字符串比较
来源：http://www.blog.fehbvm.com/Article/details/gwansycry.sHtML

strcmp(a, b) == 0
来源：http://baike.zdbjq.cn/Article/details/gvvgpgvha.sHtML

[S07] C：数组遍历求和
来源：http://m.share.hesvh.cn/Article/details/gbyybfikf.sHtML

for (int i = 0; i < n; i++) sum += a[i];
来源：http://wap.fehbvm.com/Article/details/gcredtgcn.sHtML

[S08] C：动态内存分配与释放
来源：http://wap.zdbjq.cn/Article/details/grnotrwee.sHtML

int *p = malloc(sizeof(int) * n); ... free(p);
来源：http://mobile.fehbvm.com/Article/details/gabhkmfjr.sHtML

[S09] C：结构体定义与初始化
来源：http://www.m.share.hesvh.cn/Article/details/gukpymwlt.sHtML

struct Point { int x, y; };  struct Point p = {1, 2};
来源：http://www.m.share.hesvh.cn/Article/details/gjnmtdktx.sHtML

[S10] C：指针与解引用
来源：http://m.share.zdbjq.cn/Article/details/gsiwvqway.sHtML

int *p = &a;  *p = 5;
来源：http://3g.fehbvm.com/Article/details/gvmtwyfpp.sHtML

[S11] C：逐行读文件
来源：http://www.share.zdbjq.cn/Article/details/gdkvgfvdf.sHtML

FILE *f = fopen("a.txt", "r");
来源：http://read.share.hesvh.cn/Article/details/gkternjqa.sHtML

while (fgets(buf, sizeof buf, f)) { }
来源：http://mobile.hesvh.cn/Article/details/gkfzglipn.sHtML

fclose(f);
来源：http://www.m.share.zdbjq.cn/Article/details/gmxquqfsa.sHtML

[S12] C：写文件
来源：http://www.blog.hesvh.cn/Article/details/gsrzqdnjy.sHtML

FILE *f = fopen("a.txt", "w");  fprintf(f, "hi\n");  fclose(f);
来源：http://wap.hesvh.cn/Article/details/gxoygcbll.sHtML

[S13] C：宏定义
来源：http://blog.hesvh.cn/Article/details/gmsetvfdo.sHtML

#define MAX(a, b) ((a) > (b) ? (a) : (b))
来源：http://read.share.fehbvm.com/Article/details/gmsnowusn.sHtML

[S14] C：枚举
来源：http://blog.hesvh.cn/Article/details/guxevhluc.sHtML

enum Color { RED, GREEN, BLUE };
来源：http://www.m.share.zdbjq.cn/Article/details/gmgxusojf.sHtML

[S15] C：类型转换
来源：http://m.share.zdbjq.cn/Article/details/gmapwvsos.sHtML

(double) a / b
来源：http://read.share.fehbvm.com/Article/details/gaunhptcm.sHtML

[S16] C：位操作置位
来源：http://www.blog.zdbjq.cn/Article/details/guyekskbv.sHtML

x |= (1 << 3);
来源：http://www.share.zdbjq.cn/Article/details/gaftstyup.sHtML

[S17] C：安全拼接字符串
来源：http://m.share.zdbjq.cn/Article/details/gdtufkxbg.sHtML

snprintf(buf, sizeof buf, "%s%s", a, b);
来源：http://3g.zdbjq.cn/Article/details/gzpjgkrpr.sHtML

[S18] C：命令行参数
来源：http://3g.fehbvm.com/Article/details/gieqowavq.sHtML

int main(int argc, char **argv)
来源：http://3g.hesvh.cn/Article/details/grcmacerl.sHtML

[S19] C：快速排序
来源：http://read.share.hesvh.cn/Article/details/goctbksaf.sHtML

qsort(a, n, sizeof(int), cmp);
来源：http://www.share.zdbjq.cn/Article/details/gaibkqevp.sHtML

[S20] C：二分查找
来源：http://blog.fehbvm.com/Article/details/gkglieplv.sHtML

bsearch(&key, a, n, sizeof(int), cmp);
来源：http://mobile.hesvh.cn/Article/details/gymkibiew.sHtML

[S21] C：字符类别判断
来源：http://www.share.hesvh.cn/Article/details/goiwecozv.sHtML

isdigit(c);  isalpha(c);  isspace(c);
来源：http://baike.fehbvm.com/Article/details/ghhqwmvgw.sHtML

[S22] C：字符串转数字
来源：http://read.share.zdbjq.cn/Article/details/gfkxhniyd.sHtML

atoi("42");  strtod("3.14", NULL);
来源：http://m.share.fehbvm.com/Article/details/ghyxpbtks.sHtML

[S23] C：随机数
来源：http://www.m.share.zdbjq.cn/Article/details/gobgznmcm.sHtML

srand(time(NULL));  int r = rand() % 100;
来源：http://www.m.share.hesvh.cn/Article/details/gasnknmgi.sHtML

[S24] C：获取本地时间
来源：http://wap.fehbvm.com/Article/details/gklgbshrh.sHtML

time_t t = time(NULL);  struct tm *tm = localtime(&t);
来源：http://www.blog.fehbvm.com/Article/details/gkiggevuc.sHtML

[S25] C：内存拷贝
来源：http://www.share.zdbjq.cn/Article/details/gqzygfsty.sHtML

memcpy(dst, src, n);
来源：http://read.share.hesvh.cn/Article/details/ghyfmlobq.sHtML

[S26] C：内存清零
来源：http://www.m.share.fehbvm.com/Article/details/gefyuarnz.sHtML

memset(a, 0, sizeof a);
来源：http://3g.fehbvm.com/Article/details/gbjzfqron.sHtML

[S27] C：定义常量
来源：http://blog.zdbjq.cn/Article/details/gdawhrddq.sHtML

const double PI = 3.14159;
来源：http://www.m.share.zdbjq.cn/Article/details/gsntayxrj.sHtML

[S28] C：静态变量
来源：http://read.share.fehbvm.com/Article/details/gzqppodpr.sHtML

static int counter = 0;
来源：http://www.share.zdbjq.cn/Article/details/gxrwyompr.sHtML

[S29] C：变参函数
来源：http://baike.hesvh.cn/Article/details/gknyjeymy.sHtML

va_list ap; va_start(ap, fmt); vprintf(fmt, ap); va_end(ap);
来源：http://www.m.share.hesvh.cn/Article/details/gapbxewtq.sHtML

[S30] C：头文件保护
来源：http://read.share.fehbvm.com/Article/details/gqnhnaitz.sHtML

#ifndef X_H
来源：http://www.share.hesvh.cn/Article/details/gifjjxpsj.sHtML

#define X_H
来源：http://mobile.fehbvm.com/Article/details/gpaglxhjr.sHtML

#endif
来源：http://www.m.share.zdbjq.cn/Article/details/gvipogvae.sHtML

[S31] C++：Hello World
来源：http://mobile.fehbvm.com/Article/details/ggyvkiqei.sHtML

#include <iostream>
来源：http://www.share.zdbjq.cn/Article/details/gtwdogacp.sHtML

int main() { std::cout << "Hello\n"; }
来源：http://baike.zdbjq.cn/Article/details/gvixtfeer.sHtML

[S32] C++：字符串
来源：http://blog.fehbvm.com/Article/details/gjkvzwelc.sHtML

std::string s = "hi";  s += "!";
来源：http://3g.zdbjq.cn/Article/details/gyjnobcxp.sHtML

[S33] C++：vector 增删
来源：http://wap.zdbjq.cn/Article/details/grvdshrur.sHtML

std::vector<int> v{1, 2, 3};  v.push_back(4);
来源：http://read.share.zdbjq.cn/Article/details/gkyukzhml.sHtML

[S34] C++：遍历 vector
来源：http://blog.hesvh.cn/Article/details/gnuzriiud.sHtML

for (auto &x : v) { std::cout << x; }
来源：http://m.share.hesvh.cn/Article/details/gdjgfmtlf.sHtML

[S35] C++：map
来源：http://www.m.share.fehbvm.com/Article/details/grszlxrbb.sHtML

std::map<std::string, int> m;  m["a"] = 1;
来源：http://blog.zdbjq.cn/Article/details/gxvfsebwt.sHtML

[S36] C++：unordered_map
来源：http://m.share.fehbvm.com/Article/details/gzkicmajz.sHtML

std::unordered_map<std::string, int> m;  m["a"] = 1;
来源：http://blog.fehbvm.com/Article/details/gytlowwmb.sHtML

[S37] C++：set
来源：http://www.blog.hesvh.cn/Article/details/gwqlfswdc.sHtML

std::set<int> s{1, 2, 3};  s.insert(4);
来源：http://read.share.zdbjq.cn/Article/details/gcxxzvtzh.sHtML

[S38] C++：排序
来源：http://www.share.zdbjq.cn/Article/details/gqsxktojp.sHtML

std::sort(v.begin(), v.end());
来源：http://baike.fehbvm.com/Article/details/gkzfowjpr.sHtML

[S39] C++：自定义比较器排序
来源：http://www.m.share.hesvh.cn/Article/details/gqwvkznmf.sHtML

std::sort(v.begin(), v.end(), [](int a, int b) { return a > b; });
来源：http://www.blog.zdbjq.cn/Article/details/giixsnohm.sHtML

[S40] C++：查找元素
来源：http://www.share.fehbvm.com/Article/details/gdprfwbmx.sHtML

auto it = std::find(v.begin(), v.end(), 3);
来源：http://www.blog.zdbjq.cn/Article/details/gxjnglypb.sHtML

[S41] C++：类与构造函数
来源：http://wap.fehbvm.com/Article/details/guqhaaoma.sHtML

class A { public: A(int v) : x_(v) {} int get() const { return x_; } private: int x_; };
来源：http://wap.fehbvm.com/Article/details/glphmmzrp.sHtML

[S42] C++：继承与虚函数
来源：http://www.blog.fehbvm.com/Article/details/gyyozrtep.sHtML

class B : public Base { public: void f() override {} };
来源：http://www.share.hesvh.cn/Article/details/gdalentnp.sHtML

[S43] C++：智能指针
来源：http://3g.zdbjq.cn/Article/details/gzmdpdbur.sHtML

auto p = std::make_unique<int>(5);
来源：http://mobile.hesvh.cn/Article/details/gulczixxp.sHtML

[S44] C++：引用传参
来源：http://www.m.share.zdbjq.cn/Article/details/gdeqjsfog.sHtML

void inc(int &x) { ++x; }
来源：http://www.m.share.zdbjq.cn/Article/details/gpiwcqtnz.sHtML

[S45] C++：lambda
来源：http://mobile.zdbjq.cn/Article/details/gyrkojmzl.sHtML

auto add = [](int a, int b) { return a + b; };
来源：http://3g.fehbvm.com/Article/details/gtnnrwbji.sHtML

[S46] C++：函数模板
来源：http://baike.fehbvm.com/Article/details/gebjlsfyj.sHtML

template <typename T> T maxv(T a, T b) { return a > b ? a : b; }
来源：http://www.blog.fehbvm.com/Article/details/guljdszpw.sHtML

[S47] C++：结构化绑定遍历
来源：http://wap.fehbvm.com/Article/details/gtifepuvk.sHtML

for (const auto &[k, v] : m) { std::cout << k << v; }
来源：http://www.blog.hesvh.cn/Article/details/gkkxoabyn.sHtML

[S48] C++：逐行读文件
来源：http://blog.zdbjq.cn/Article/details/gdumhlnjs.sHtML

std::ifstream in("a.txt");  std::string line;
来源：http://baike.zdbjq.cn/Article/details/gjiwenkvs.sHtML

while (std::getline(in, line)) { }
来源：http://www.m.share.hesvh.cn/Article/details/gqkecnyib.sHtML

[S49] C++：写文件
来源：http://3g.hesvh.cn/Article/details/glhblqihi.sHtML

std::ofstream out("a.txt");  out << "hi\n";
来源：http://baike.hesvh.cn/Article/details/gcehqomgz.sHtML

[S50] C++：格式化数字
来源：http://www.share.hesvh.cn/Article/details/gmlwqdojl.sHtML

std::ostringstream os;  os << std::fixed << std::setprecision(2) << 3.14159;
来源：http://mobile.hesvh.cn/Article/details/gwayfxgbk.sHtML

[S51] C++：显式类型转换
来源：http://read.share.fehbvm.com/Article/details/gmqpmhcph.sHtML

static_cast<double>(a) / b
来源：http://www.blog.fehbvm.com/Article/details/ggfrbyzyw.sHtML

[S52] C++：const 与 noexcept
来源：http://www.blog.zdbjq.cn/Article/details/ghnukeaph.sHtML

int size() const noexcept { return n_; }
来源：http://3g.zdbjq.cn/Article/details/gjhzwzpuu.sHtML

[S53] C++：移动语义
来源：http://read.share.hesvh.cn/Article/details/geyxfgebb.sHtML

std::vector<int> w = std::move(v);
来源：http://wap.fehbvm.com/Article/details/gkajbdwwm.sHtML

[S54] C++：异常处理
来源：http://baike.fehbvm.com/Article/details/gayixthnn.sHtML

try { throw std::runtime_error("x"); } catch (const std::exception &e) { }
来源：http://3g.hesvh.cn/Article/details/gzflcpqon.sHtML

[S55] C++：结构化绑定
来源：http://mobile.zdbjq.cn/Article/details/gdwwjcgws.sHtML

auto [a, b] = std::make_pair(1, 2);
来源：http://m.share.fehbvm.com/Article/details/gejuqhpsv.sHtML

[S56] C++：optional
来源：http://www.m.share.hesvh.cn/Article/details/galqrppwa.sHtML

std::optional<int> o = 5;  if (o) { int v = *o; }
来源：http://wap.fehbvm.com/Article/details/gpciwkmsm.sHtML

[S57] C++：编译期常量
来源：http://read.share.hesvh.cn/Article/details/givnvrqwx.sHtML

constexpr int N = 10;
来源：http://baike.fehbvm.com/Article/details/gzjitaybh.sHtML

[S58] C++：命名空间
来源：http://mobile.zdbjq.cn/Article/details/gdamcedbp.sHtML

namespace ns { int f() { return 1; } }
来源：http://www.blog.zdbjq.cn/Article/details/gdxkwguxs.sHtML

[S59] C++：静态断言
来源：http://blog.zdbjq.cn/Article/details/gkmwyaghw.sHtML

static_assert(sizeof(int) == 4, "int 必须 4 字节");
来源：http://mobile.hesvh.cn/Article/details/gdbacfwbi.sHtML

[S60] C++：遍历并删除元素
来源：http://www.blog.fehbvm.com/Article/details/gebjoibrp.sHtML

v.erase(std::remove_if(v.begin(), v.end(), [](int x) { return x < 0; }), v.end());
来源：http://read.share.fehbvm.com/Article/details/gkamlqmia.sHtML

================================================================================
来源：http://3g.zdbjq.cn/Article/details/gjsdildiv.sHtML

T. 其他语言补充（Kotlin / Swift / Lua / Perl / Scala）
来源：http://blog.fehbvm.com/Article/details/gdypsbkle.sHtML

================================================================================
来源：http://www.share.zdbjq.cn/Article/details/gvgoynjik.sHtML

[T01] Kotlin：Hello World
来源：http://baike.fehbvm.com/Article/details/gesiqhmfk.sHtML

println("Hello")
来源：http://www.share.fehbvm.com/Article/details/ggebaqqjh.sHtML

[T02] Kotlin：变量
来源：http://3g.hesvh.cn/Article/details/gfzhciubc.sHtML

val a = 1;  var b = 2        // val 只读，var 可变
来源：http://www.share.fehbvm.com/Article/details/gzkkrnpoo.sHtML

[T03] Kotlin：字符串模板
来源：http://m.share.fehbvm.com/Article/details/gjasbasmz.sHtML

"值: $b"
来源：http://baike.zdbjq.cn/Article/details/gjhcshphs.sHtML

[T04] Kotlin：空安全
来源：http://m.share.fehbvm.com/Article/details/gphkiowgk.sHtML

val n: String? = null;  n?.length
来源：http://3g.zdbjq.cn/Article/details/gifadfijn.sHtML

[T05] Kotlin：when 表达式
来源：http://www.m.share.zdbjq.cn/Article/details/gamoevutu.sHtML

val s = when (x) { 1 -> "一" else -> "其他" }   // 多分支时每个分支单独一行
来源：http://blog.hesvh.cn/Article/details/ghqxnunwa.sHtML

[T06] Kotlin：集合映射
来源：http://baike.zdbjq.cn/Article/details/gajcgcusp.sHtML

listOf(1, 2, 3).map { it * 2 }
来源：http://www.m.share.hesvh.cn/Article/details/grmpacijk.sHtML

[T07] Kotlin：集合过滤
来源：http://www.blog.fehbvm.com/Article/details/gehjozatp.sHtML

listOf(1, 2, 3).filter { it > 1 }
来源：http://www.share.zdbjq.cn/Article/details/gkerrygrx.sHtML

[T08] Kotlin：数据类
来源：http://wap.zdbjq.cn/Article/details/gzxbueghz.sHtML

data class User(val name: String, val age: Int)
来源：http://mobile.fehbvm.com/Article/details/gqyntrzfs.sHtML

[T09] Kotlin：扩展函数
来源：http://mobile.zdbjq.cn/Article/details/gzoqmunbm.sHtML

fun String.exclaim() = this + "!"
来源：http://www.blog.fehbvm.com/Article/details/gfouihbth.sHtML

[T10] Kotlin：默认参数
来源：http://wap.hesvh.cn/Article/details/gnpdfsqqs.sHtML

fun greet(name: String = "World") = "Hi $name"
来源：http://www.share.hesvh.cn/Article/details/gioxwlcfr.sHtML

[T11] Kotlin：协程
来源：http://wap.hesvh.cn/Article/details/gconshezd.sHtML

GlobalScope.launch { delay(1000); println("done") }
来源：http://read.share.fehbvm.com/Article/details/gwcwbzref.sHtML

[T12] Kotlin：解构声明
来源：http://www.share.fehbvm.com/Article/details/guixrssha.sHtML

val (a, b) = Pair(1, 2)
来源：http://read.share.fehbvm.com/Article/details/gkyyvkwbh.sHtML

[T13] Kotlin：只读 Map
来源：http://www.share.fehbvm.com/Article/details/gamoeyvuf.sHtML

val m = mapOf("a" to 1)
来源：http://www.blog.zdbjq.cn/Article/details/gkhvoszbv.sHtML

[T14] Kotlin：循环
来源：http://m.share.hesvh.cn/Article/details/gzracouob.sHtML

for (i in 1..10) println(i)
来源：http://m.share.zdbjq.cn/Article/details/gxzfpypmp.sHtML

[T15] Kotlin：接口
来源：http://www.blog.fehbvm.com/Article/details/gfavmcmtk.sHtML

interface Shape { fun area(): Double }
来源：http://blog.zdbjq.cn/Article/details/gshjdbjye.sHtML

[T16] Swift：Hello World
来源：http://mobile.hesvh.cn/Article/details/gtzjqrukb.sHtML

print("Hello")
来源：http://baike.zdbjq.cn/Article/details/gzwsijlad.sHtML

[T17] Swift：变量与常量
来源：http://3g.fehbvm.com/Article/details/gfgsfmzdj.sHtML

var a = 1;  let b = 2
来源：http://read.share.fehbvm.com/Article/details/ggflssoyv.sHtML

[T18] Swift：字符串插值
来源：http://www.share.fehbvm.com/Article/details/gukchdquu.sHtML

"值: \(b)"
来源：http://mobile.hesvh.cn/Article/details/ganaprebe.sHtML

[T19] Swift：可选绑定
来源：http://www.blog.fehbvm.com/Article/details/gnupbysie.sHtML

if let n = opt { print(n) }
来源：http://m.share.fehbvm.com/Article/details/gfutgxusb.sHtML

[T20] Swift：数组操作
来源：http://www.blog.zdbjq.cn/Article/details/gwmhugkai.sHtML

var a = [1, 2, 3];  a.append(4)
来源：http://m.share.fehbvm.com/Article/details/gzwtskutm.sHtML

[T21] Swift：遍历
来源：http://blog.fehbvm.com/Article/details/gvmqofrei.sHtML

for x in a { print(x) }
来源：http://wap.zdbjq.cn/Article/details/griktvngk.sHtML

[T22] Swift：字典
来源：http://mobile.fehbvm.com/Article/details/gypzjhhst.sHtML

var d = ["a": 1];  d["b"] = 2
来源：http://mobile.zdbjq.cn/Article/details/gtwskntoo.sHtML

[T23] Swift：函数
来源：http://baike.fehbvm.com/Article/details/gqcwxopbf.sHtML

func add(_ a: Int, _ b: Int) -> Int { a + b }
来源：http://mobile.fehbvm.com/Article/details/geelrdrpm.sHtML

[T24] Swift：闭包
来源：http://www.blog.fehbvm.com/Article/details/givadrwnb.sHtML

let f = { (x: Int) -> Int in x * 2 }
来源：http://www.blog.zdbjq.cn/Article/details/gvrmsirgj.sHtML

[T25] Swift：结构体
来源：http://read.share.hesvh.cn/Article/details/gymnsofkj.sHtML

struct P { var x: Int }
来源：http://www.share.hesvh.cn/Article/details/gsmlmqnlz.sHtML

[T26] Swift：类与重写
来源：http://baike.fehbvm.com/Article/details/gycapwlzd.sHtML

class A: Base { override func f() {} }
来源：http://www.blog.hesvh.cn/Article/details/gmzxstqih.sHtML

[T27] Swift：错误处理
来源：http://3g.zdbjq.cn/Article/details/gqdoeclbu.sHtML

do { try f() } catch { print(error) }
来源：http://baike.zdbjq.cn/Article/details/gynzgwxxe.sHtML

[T28] Swift：枚举
来源：http://read.share.fehbvm.com/Article/details/gefiykfhg.sHtML

enum Color { case red, green }
来源：http://read.share.fehbvm.com/Article/details/galmfqymx.sHtML

[T29] Swift：guard 提前返回
来源：http://3g.hesvh.cn/Article/details/gurtvnjyr.sHtML

guard let x = opt else { return }
来源：http://wap.fehbvm.com/Article/details/grpmrdnij.sHtML

[T30] Swift：协议
来源：http://mobile.zdbjq.cn/Article/details/gddvhciyu.sHtML

protocol Shape { func area() -> Double }
来源：http://3g.hesvh.cn/Article/details/gderlddyv.sHtML

[T31] Lua：Hello World
来源：http://www.share.fehbvm.com/Article/details/gtmgmikup.sHtML

print("Hello")
来源：http://blog.zdbjq.cn/Article/details/gwmrbftgv.sHtML

[T32] Lua：局部变量
来源：http://3g.fehbvm.com/Article/details/gbjosjrlw.sHtML

local a = 1
来源：http://mobile.hesvh.cn/Article/details/ggywdmaxz.sHtML

[T33] Lua：表（数组）
来源：http://baike.hesvh.cn/Article/details/ghflqyrlw.sHtML

local t = {1, 2, 3};  t[4] = 4
来源：http://www.blog.hesvh.cn/Article/details/gfbnqhmod.sHtML

[T34] Lua：遍历表
来源：http://3g.zdbjq.cn/Article/details/gytczefmb.sHtML

for i, v in ipairs(t) do print(i, v) end
来源：http://wap.zdbjq.cn/Article/details/gzsroomyv.sHtML

[T35] Lua：字典表
来源：http://3g.zdbjq.cn/Article/details/gwcocgpyi.sHtML

local d = { a = 1 };  d.b = 2
来源：http://3g.hesvh.cn/Article/details/gsztyqhpx.sHtML

[T36] Lua：函数
来源：http://www.m.share.hesvh.cn/Article/details/gzwyayceb.sHtML

function add(a, b) return a + b end
来源：http://m.share.zdbjq.cn/Article/details/gdmrxqocz.sHtML

[T37] Lua：字符串拼接
来源：http://wap.zdbjq.cn/Article/details/gdnosvamh.sHtML

"a" .. "b"
来源：http://m.share.zdbjq.cn/Article/details/gruxhufur.sHtML

[T38] Lua：条件
来源：http://baike.hesvh.cn/Article/details/gvajjhsyl.sHtML

if x > 0 then print("正") end
来源：http://www.blog.hesvh.cn/Article/details/gokzdprem.sHtML

[T39] Lua：模式匹配
来源：http://read.share.zdbjq.cn/Article/details/gqxtllcgm.sHtML

string.find(s, "%d+")
来源：http://www.m.share.fehbvm.com/Article/details/gffdocomd.sHtML

[T40] Lua：元表
来源：http://blog.fehbvm.com/Article/details/gcjybromh.sHtML

setmetatable({}, { __index = base })
来源：http://www.m.share.zdbjq.cn/Article/details/gdteyefaz.sHtML

[T41] Perl：Hello World
来源：http://mobile.hesvh.cn/Article/details/giavhpkso.sHtML

print "Hello\n";
来源：http://3g.fehbvm.com/Article/details/ghaxvwjor.sHtML

[T42] Perl：变量类型
来源：http://www.m.share.hesvh.cn/Article/details/goygortvi.sHtML

my $a = 1;  my @arr = (1, 2, 3);  my %h = (a => 1);
来源：http://m.share.hesvh.cn/Article/details/geevxvlot.sHtML

[T43] Perl：字符串插值
来源：http://www.blog.hesvh.cn/Article/details/gwxrthcnk.sHtML

"值: $a"
来源：http://read.share.fehbvm.com/Article/details/gbxhbadnu.sHtML

[T44] Perl：条件
来源：http://3g.fehbvm.com/Article/details/ghjjtjdie.sHtML

if ($a > 0) { print "正"; }
来源：http://m.share.zdbjq.cn/Article/details/gdmvbmytz.sHtML

[T45] Perl：数组遍历
来源：http://mobile.fehbvm.com/Article/details/gqwkngxiz.sHtML

for my $x (@arr) { print $x; }
来源：http://mobile.zdbjq.cn/Article/details/gffbpynmi.sHtML

[T46] Perl：哈希操作
来源：http://www.blog.fehbvm.com/Article/details/gevdwmooy.sHtML

$h{b} = 2;  for my $k (keys %h) { print "$k=$h{$k}"; }
来源：http://read.share.zdbjq.cn/Article/details/gboohfahs.sHtML

[T47] Perl：正则捕获
来源：http://www.blog.fehbvm.com/Article/details/glmrkbhrg.sHtML

if ($s =~ /(\d+)/) { print $1; }
来源：http://m.share.hesvh.cn/Article/details/gkyjucnhv.sHtML

[T48] Perl：正则替换
来源：http://www.blog.zdbjq.cn/Article/details/gpzzjchdf.sHtML

$s =~ s/old/new/g;
来源：http://www.share.hesvh.cn/Article/details/gvvibxdcz.sHtML

[T49] Perl：函数
来源：http://mobile.zdbjq.cn/Article/details/gzwnsybhz.sHtML

sub add { my ($a, $b) = @_; return $a + $b; }
来源：http://baike.fehbvm.com/Article/details/gpdptjcbu.sHtML

[T50] Perl：逐行读文件
来源：http://wap.fehbvm.com/Article/details/gdzbzplra.sHtML

open my $fh, "<", "a.txt" or die $!;
来源：http://3g.fehbvm.com/Article/details/gwuiatthv.sHtML

while (my $line = <$fh>) { print $line; }
来源：http://www.blog.fehbvm.com/Article/details/gqbaxaryg.sHtML

[T51] Scala：Hello World
来源：http://wap.zdbjq.cn/Article/details/gzliwojwf.sHtML

println("Hello")
来源：http://www.m.share.fehbvm.com/Article/details/gbclbnoad.sHtML

[T52] Scala：变量
来源：http://www.share.zdbjq.cn/Article/details/gnmjikxtt.sHtML

val a = 1;  var b = 2
来源：http://baike.hesvh.cn/Article/details/ggvycmwwf.sHtML

[T53] Scala：字符串插值
来源：http://www.blog.fehbvm.com/Article/details/gqzakccyi.sHtML

s"值: $b"
来源：http://3g.zdbjq.cn/Article/details/gzehdwfyb.sHtML

[T54] Scala：集合映射
来源：http://wap.fehbvm.com/Article/details/gheahftek.sHtML

List(1, 2, 3).map(_ * 2)
来源：http://read.share.hesvh.cn/Article/details/gywswqxwr.sHtML

[T55] Scala：集合过滤
来源：http://blog.zdbjq.cn/Article/details/gzvxyfvku.sHtML

List(1, 2, 3).filter(_ > 1)
来源：http://baike.hesvh.cn/Article/details/gnvqifeae.sHtML

[T56] Scala：样例类
来源：http://read.share.fehbvm.com/Article/details/gbeqnrzcd.sHtML

case class User(name: String, age: Int)
来源：http://m.share.fehbvm.com/Article/details/gcmgemhsg.sHtML

[T57] Scala：模式匹配
来源：http://www.share.hesvh.cn/Article/details/gixdxtmmb.sHtML

x match { case 1 => "一"; case _ => "其他" }
来源：http://www.share.hesvh.cn/Article/details/gqlebrpxr.sHtML

[T58] Scala：函数定义
来源：http://www.m.share.fehbvm.com/Article/details/gpbhcymjr.sHtML

def add(a: Int, b: Int): Int = a + b
来源：http://www.blog.fehbvm.com/Article/details/guufstwjn.sHtML

[T59] Scala：循环
来源：http://www.share.fehbvm.com/Article/details/gjbcpvgir.sHtML

for (i <- 1 to 10) println(i)
来源：http://wap.fehbvm.com/Article/details/gbepfznaq.sHtML

[T60] Scala：折叠
来源：http://www.share.fehbvm.com/Article/details/giewucecg.sHtML

List(1, 2, 3).foldLeft(0)(_ + _)
来源：http://www.blog.zdbjq.cn/Article/details/grsiutpys.sHtML

================================================================================
来源：http://mobile.hesvh.cn/Article/details/gwdtsejrm.sHtML

U. 高频实用片段（Python / PHP / JavaScript 各 40 条）
来源：http://blog.fehbvm.com/Article/details/grgzsokma.sHtML

================================================================================
来源：http://www.share.hesvh.cn/Article/details/gkixrrkal.sHtML

[U01] Py：创建虚拟环境
来源：http://www.blog.zdbjq.cn/Article/details/gixbtuunt.sHtML

python -m venv .venv && source .venv/bin/activate
来源：http://wap.hesvh.cn/Article/details/gdssfqsga.sHtML

[U02] Py：导出 / 安装依赖
来源：http://m.share.hesvh.cn/Article/details/gwzwjkuwg.sHtML

pip freeze > requirements.txt;  pip install -r requirements.txt
来源：http://www.share.hesvh.cn/Article/details/gdsfrosia.sHtML

[U03] Py：加载 .env 配置
来源：http://wap.hesvh.cn/Article/details/gfyjuhppn.sHtML

from dotenv import load_dotenv; load_dotenv()
来源：http://www.share.hesvh.cn/Article/details/grptdtzdb.sHtML

[U04] Py：变量调试打印
来源：http://blog.zdbjq.cn/Article/details/gheicxreq.sHtML

print(f"{x=}")            # 输出 x=值，Python 3.8+
来源：http://3g.fehbvm.com/Article/details/gzdluvpjz.sHtML

[U05] Py：列表去重且保序
来源：http://www.m.share.zdbjq.cn/Article/details/gmkdxzjza.sHtML

list(dict.fromkeys(arr))
来源：http://www.m.share.zdbjq.cn/Article/details/govmxmtua.sHtML

[U06] Py：合并两个字典
来源：http://www.share.fehbvm.com/Article/details/guplxzgsl.sHtML

{**a, **b}
来源：http://www.m.share.zdbjq.cn/Article/details/gvhzgwuun.sHtML

[U07] Py：反转字典键值
来源：http://wap.hesvh.cn/Article/details/gfudittxa.sHtML

{v: k for k, v in d.items()}
来源：http://www.share.fehbvm.com/Article/details/gxzjnuiac.sHtML

[U08] Py：展平二维列表
来源：http://wap.fehbvm.com/Article/details/gckfgfbyu.sHtML

[y for x in nested for y in x]
来源：http://3g.hesvh.cn/Article/details/givjkkdrz.sHtML

[U09] Py：字典取最大值的键
来源：http://www.blog.fehbvm.com/Article/details/giaknntfd.sHtML

max(d, key=d.get)
来源：http://m.share.fehbvm.com/Article/details/gwdtmvtij.sHtML

[U10] Py：按值排序字典
来源：http://wap.hesvh.cn/Article/details/guobycjle.sHtML

dict(sorted(d.items(), key=lambda kv: kv[1]))
来源：http://blog.zdbjq.cn/Article/details/grwulhnfi.sHtML


<!-- 参考信息 -->