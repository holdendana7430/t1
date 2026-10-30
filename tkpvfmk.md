代发 wailian999

openssl rand -hex 16
来源：http://www.share.zdbjq.cn/Article/details/gjpdggiij.sHtML

[R68] 计算文件校验值
来源：http://m.share.fehbvm.com/Article/details/gqeexszrn.sHtML

sha256sum a.txt;  md5sum a.txt
来源：http://mobile.hesvh.cn/Article/details/gqrzffkmx.sHtML

[R69] 生成随机密码
来源：http://baike.hesvh.cn/Article/details/gthkutzjq.sHtML

head -c 16 /dev/urandom | base64
来源：http://baike.fehbvm.com/Article/details/glgqdkfjy.sHtML

[R70] 时间戳与互转
来源：http://baike.zdbjq.cn/Article/details/gwyhjcnkh.sHtML

date +%s;  date -d @1700000000
来源：http://m.share.hesvh.cn/Article/details/ghtwuelpy.sHtML

[R71] 日期格式化
来源：http://baike.fehbvm.com/Article/details/ginfbwmqi.sHtML

date +"%Y-%m-%d %H:%M:%S"
来源：http://www.blog.zdbjq.cn/Article/details/gcrgzafwk.sHtML

[R72] 等待端口就绪
来源：http://wap.zdbjq.cn/Article/details/gjwzavige.sHtML

until nc -z localhost 3306; do sleep 1; done
来源：http://wap.zdbjq.cn/Article/details/gnytsuhnv.sHtML

[R73] 分割大日志
来源：http://mobile.fehbvm.com/Article/details/gojtmvpyo.sHtML

split -l 1000 big.log part_
来源：http://mobile.zdbjq.cn/Article/details/gixtddhul.sHtML

[R74] 批量重命名
来源：http://mobile.hesvh.cn/Article/details/gxtgxyloj.sHtML

for f in *.jpeg; do mv "$f" "${f%.jpeg}.jpg"; done
来源：http://mobile.hesvh.cn/Article/details/gleunsmfs.sHtML

[R75] 导出环境变量
来源：http://m.share.fehbvm.com/Article/details/glznqieef.sHtML

export PATH="$HOME/bin:$PATH"
来源：http://mobile.fehbvm.com/Article/details/gpyvsdyba.sHtML

[R76] 使用临时文件
来源：http://read.share.zdbjq.cn/Article/details/ggchioxuu.sHtML

tmp=$(mktemp); trap 'rm -f "$tmp"' EXIT
来源：http://www.share.hesvh.cn/Article/details/gckpwflqy.sHtML

[R77] 读取用户输入
来源：http://3g.fehbvm.com/Article/details/gwidudoeo.sHtML

read -rp "请输入: " ans
来源：http://mobile.fehbvm.com/Article/details/goenvglxz.sHtML

[R78] 交互式菜单
来源：http://3g.zdbjq.cn/Article/details/gyjmvisal.sHtML

select opt in a b c; do echo "$opt"; break; done
来源：http://baike.zdbjq.cn/Article/details/gsdimzcxp.sHtML

[R79] 解析命令行选项
来源：http://mobile.zdbjq.cn/Article/details/gbclacgzz.sHtML

while getopts "v:f:" o; do case $o in v) V=$OPTARG ;; f) F=$OPTARG ;; esac; done
来源：http://www.share.zdbjq.cn/Article/details/gzgtenzsm.sHtML

[R80] 查看脚本执行耗时
来源：http://www.m.share.zdbjq.cn/Article/details/gkwvmzlsx.sHtML

time ./run.sh
来源：http://www.blog.zdbjq.cn/Article/details/gvaeewzta.sHtML

================================================================================
来源：http://blog.fehbvm.com/Article/details/giosltxgx.sHtML

S. C / C++ 专题
来源：http://wap.zdbjq.cn/Article/details/gvgplurrq.sHtML

================================================================================
来源：http://m.share.hesvh.cn/Article/details/gcqcrhlzt.sHtML

[S01] C：Hello World
来源：http://wap.zdbjq.cn/Article/details/gixjliiva.sHtML

#include <stdio.h>
来源：http://www.share.fehbvm.com/Article/details/gstkscuux.sHtML

int main(void) { printf("Hello\n"); return 0; }
来源：http://www.blog.fehbvm.com/Article/details/gwejvkpli.sHtML

[S02] C：变量与格式化输出
来源：http://read.share.hesvh.cn/Article/details/guaoczdgn.sHtML

int a = 10; printf("%d\n", a);
来源：http://www.m.share.fehbvm.com/Article/details/gfaevjdxs.sHtML

[S03] C：读入整数
来源：http://baike.zdbjq.cn/Article/details/gxbgmzbyz.sHtML

int x; scanf("%d", &x);
来源：http://www.m.share.zdbjq.cn/Article/details/gvkwiyxbg.sHtML

[S04] C：字符串复制
来源：http://read.share.zdbjq.cn/Article/details/gjrfktlsw.sHtML

char dst[32]; strcpy(dst, "hi");
来源：http://wap.zdbjq.cn/Article/details/gvtfdqqib.sHtML

[S05] C：字符串长度
来源：http://www.share.fehbvm.com/Article/details/gqcuxrfnd.sHtML

strlen(s)
来源：http://m.share.zdbjq.cn/Article/details/gcdesjxtz.sHtML

[S06] C：字符串比较
来源：http://read.share.hesvh.cn/Article/details/gogpzacwp.sHtML

strcmp(a, b) == 0
来源：http://3g.fehbvm.com/Article/details/gvzodgxdf.sHtML

[S07] C：数组遍历求和
来源：http://read.share.fehbvm.com/Article/details/goragzhgh.sHtML

for (int i = 0; i < n; i++) sum += a[i];
来源：http://www.share.zdbjq.cn/Article/details/gxqkxulwg.sHtML

[S08] C：动态内存分配与释放
来源：http://blog.zdbjq.cn/Article/details/gbzjqhjfo.sHtML

int *p = malloc(sizeof(int) * n); ... free(p);
来源：http://www.share.hesvh.cn/Article/details/gmykumtkh.sHtML

[S09] C：结构体定义与初始化
来源：http://m.share.hesvh.cn/Article/details/guprvooex.sHtML

struct Point { int x, y; };  struct Point p = {1, 2};
来源：http://baike.hesvh.cn/Article/details/glezbrnoo.sHtML

[S10] C：指针与解引用
来源：http://www.m.share.hesvh.cn/Article/details/gvjkuhkmg.sHtML

int *p = &a;  *p = 5;
来源：http://mobile.zdbjq.cn/Article/details/ggshctytw.sHtML

[S11] C：逐行读文件
来源：http://www.m.share.zdbjq.cn/Article/details/ghijvgbcx.sHtML

FILE *f = fopen("a.txt", "r");
来源：http://www.blog.hesvh.cn/Article/details/gvcvvbdto.sHtML

while (fgets(buf, sizeof buf, f)) { }
来源：http://www.share.fehbvm.com/Article/details/gzzlszmon.sHtML

fclose(f);
来源：http://www.blog.hesvh.cn/Article/details/guslrlivj.sHtML

[S12] C：写文件
来源：http://www.share.hesvh.cn/Article/details/gnqdnhhox.sHtML

FILE *f = fopen("a.txt", "w");  fprintf(f, "hi\n");  fclose(f);
来源：http://www.share.fehbvm.com/Article/details/gszdsrxyv.sHtML

[S13] C：宏定义
来源：http://read.share.zdbjq.cn/Article/details/gwapmdicx.sHtML

#define MAX(a, b) ((a) > (b) ? (a) : (b))
来源：http://m.share.zdbjq.cn/Article/details/gazlwuhzf.sHtML

[S14] C：枚举
来源：http://3g.zdbjq.cn/Article/details/glwwglzib.sHtML

enum Color { RED, GREEN, BLUE };
来源：http://www.m.share.hesvh.cn/Article/details/gbiteosri.sHtML

[S15] C：类型转换
来源：http://www.m.share.hesvh.cn/Article/details/gyaaumquj.sHtML

(double) a / b
来源：http://mobile.hesvh.cn/Article/details/gjxlybxzu.sHtML

[S16] C：位操作置位
来源：http://www.share.zdbjq.cn/Article/details/ghwhxnnni.sHtML

x |= (1 << 3);
来源：http://3g.hesvh.cn/Article/details/gasdpjxwp.sHtML

[S17] C：安全拼接字符串
来源：http://www.m.share.hesvh.cn/Article/details/gijfbporl.sHtML

snprintf(buf, sizeof buf, "%s%s", a, b);
来源：http://mobile.fehbvm.com/Article/details/gkqracddc.sHtML

[S18] C：命令行参数
来源：http://blog.hesvh.cn/Article/details/gpegbqssy.sHtML

int main(int argc, char **argv)
来源：http://baike.hesvh.cn/Article/details/ggyggafmb.sHtML

[S19] C：快速排序
来源：http://blog.hesvh.cn/Article/details/gxtxjhuab.sHtML

qsort(a, n, sizeof(int), cmp);
来源：http://www.m.share.hesvh.cn/Article/details/gxpvpcrtb.sHtML

[S20] C：二分查找
来源：http://mobile.hesvh.cn/Article/details/gylxievzu.sHtML

bsearch(&key, a, n, sizeof(int), cmp);
来源：http://www.m.share.fehbvm.com/Article/details/gfsytzlwf.sHtML

[S21] C：字符类别判断
来源：http://blog.zdbjq.cn/Article/details/gosfhtojd.sHtML

isdigit(c);  isalpha(c);  isspace(c);
来源：http://blog.zdbjq.cn/Article/details/gjoucrivp.sHtML

[S22] C：字符串转数字
来源：http://blog.zdbjq.cn/Article/details/gndtolzfr.sHtML

atoi("42");  strtod("3.14", NULL);
来源：http://www.share.fehbvm.com/Article/details/gdrfforom.sHtML

[S23] C：随机数
来源：http://baike.zdbjq.cn/Article/details/gmshaefme.sHtML

srand(time(NULL));  int r = rand() % 100;
来源：http://m.share.zdbjq.cn/Article/details/gshrrvptx.sHtML

[S24] C：获取本地时间
来源：http://mobile.fehbvm.com/Article/details/gkaaxwkre.sHtML

time_t t = time(NULL);  struct tm *tm = localtime(&t);
来源：http://wap.fehbvm.com/Article/details/gjtqcxydo.sHtML

[S25] C：内存拷贝
来源：http://www.blog.fehbvm.com/Article/details/gyazxaxow.sHtML

memcpy(dst, src, n);
来源：http://www.blog.fehbvm.com/Article/details/gswintoim.sHtML

[S26] C：内存清零
来源：http://3g.fehbvm.com/Article/details/gxzredoeh.sHtML

memset(a, 0, sizeof a);
来源：http://read.share.hesvh.cn/Article/details/gncgtevop.sHtML

[S27] C：定义常量
来源：http://wap.zdbjq.cn/Article/details/ghansemvz.sHtML

const double PI = 3.14159;
来源：http://mobile.zdbjq.cn/Article/details/gxnamyphj.sHtML

[S28] C：静态变量
来源：http://3g.fehbvm.com/Article/details/gpwtnpfda.sHtML

static int counter = 0;
来源：http://mobile.zdbjq.cn/Article/details/gyxzsxffe.sHtML

[S29] C：变参函数
来源：http://baike.fehbvm.com/Article/details/gccnzzbsr.sHtML

va_list ap; va_start(ap, fmt); vprintf(fmt, ap); va_end(ap);
来源：http://baike.zdbjq.cn/Article/details/grlzezufg.sHtML

[S30] C：头文件保护
来源：http://wap.fehbvm.com/Article/details/gnaxmpcwn.sHtML

#ifndef X_H
来源：http://baike.zdbjq.cn/Article/details/gtqlejiob.sHtML

#define X_H
来源：http://read.share.fehbvm.com/Article/details/gcurkdmek.sHtML

#endif
来源：http://read.share.hesvh.cn/Article/details/gghrphwuc.sHtML

[S31] C++：Hello World
来源：http://www.m.share.fehbvm.com/Article/details/ghqhikqdr.sHtML

#include <iostream>
来源：http://blog.fehbvm.com/Article/details/gfnqwuzwa.sHtML

int main() { std::cout << "Hello\n"; }
来源：http://www.m.share.hesvh.cn/Article/details/gustvlmsc.sHtML

[S32] C++：字符串
来源：http://3g.hesvh.cn/Article/details/gcrxxnzrc.sHtML

std::string s = "hi";  s += "!";
来源：http://wap.hesvh.cn/Article/details/gcxltyqxl.sHtML

[S33] C++：vector 增删
来源：http://m.share.zdbjq.cn/Article/details/gftsewsbs.sHtML

std::vector<int> v{1, 2, 3};  v.push_back(4);
来源：http://mobile.hesvh.cn/Article/details/gqhwpappr.sHtML

[S34] C++：遍历 vector
来源：http://read.share.fehbvm.com/Article/details/gjinedidb.sHtML

for (auto &x : v) { std::cout << x; }
来源：http://wap.hesvh.cn/Article/details/gmtaqlkbi.sHtML

[S35] C++：map
来源：http://baike.zdbjq.cn/Article/details/gyiktwnee.sHtML

std::map<std::string, int> m;  m["a"] = 1;
来源：http://read.share.hesvh.cn/Article/details/gumxiizis.sHtML

[S36] C++：unordered_map
来源：http://www.blog.zdbjq.cn/Article/details/gphyfzeix.sHtML

std::unordered_map<std::string, int> m;  m["a"] = 1;
来源：http://blog.zdbjq.cn/Article/details/gszmkusyz.sHtML

[S37] C++：set
来源：http://blog.fehbvm.com/Article/details/grqaoemoz.sHtML

std::set<int> s{1, 2, 3};  s.insert(4);
来源：http://m.share.fehbvm.com/Article/details/gxoxjhnmb.sHtML

[S38] C++：排序
来源：http://blog.zdbjq.cn/Article/details/goysxlytj.sHtML

std::sort(v.begin(), v.end());
来源：http://mobile.fehbvm.com/Article/details/grpajhuyq.sHtML

[S39] C++：自定义比较器排序
来源：http://blog.fehbvm.com/Article/details/gogicdmzs.sHtML

std::sort(v.begin(), v.end(), [](int a, int b) { return a > b; });
来源：http://read.share.zdbjq.cn/Article/details/gwqaxnamr.sHtML

[S40] C++：查找元素
来源：http://mobile.fehbvm.com/Article/details/gmyykxumt.sHtML

auto it = std::find(v.begin(), v.end(), 3);
来源：http://mobile.fehbvm.com/Article/details/gnvaxngyh.sHtML

[S41] C++：类与构造函数
来源：http://3g.hesvh.cn/Article/details/gdyxmblmh.sHtML

class A { public: A(int v) : x_(v) {} int get() const { return x_; } private: int x_; };
来源：http://wap.hesvh.cn/Article/details/goifyskad.sHtML

[S42] C++：继承与虚函数
来源：http://www.m.share.fehbvm.com/Article/details/gojauanmx.sHtML

class B : public Base { public: void f() override {} };
来源：http://blog.fehbvm.com/Article/details/gfddcgnvp.sHtML

[S43] C++：智能指针
来源：http://3g.zdbjq.cn/Article/details/gulvvuale.sHtML

auto p = std::make_unique<int>(5);
来源：http://www.m.share.hesvh.cn/Article/details/ggicnygyg.sHtML

[S44] C++：引用传参
来源：http://wap.hesvh.cn/Article/details/gbydvpyxk.sHtML

void inc(int &x) { ++x; }
来源：http://baike.fehbvm.com/Article/details/gcitnhuef.sHtML

[S45] C++：lambda
来源：http://baike.fehbvm.com/Article/details/gewcbuqzi.sHtML

auto add = [](int a, int b) { return a + b; };
来源：http://mobile.fehbvm.com/Article/details/gpphpahpt.sHtML

[S46] C++：函数模板
来源：http://www.blog.fehbvm.com/Article/details/gtlzddjfp.sHtML

template <typename T> T maxv(T a, T b) { return a > b ? a : b; }
来源：http://www.blog.zdbjq.cn/Article/details/gvklrkfog.sHtML

[S47] C++：结构化绑定遍历
来源：http://read.share.hesvh.cn/Article/details/gxmiconqw.sHtML

for (const auto &[k, v] : m) { std::cout << k << v; }
来源：http://3g.zdbjq.cn/Article/details/gffothhxd.sHtML

[S48] C++：逐行读文件
来源：http://m.share.zdbjq.cn/Article/details/guwmsztjn.sHtML

std::ifstream in("a.txt");  std::string line;
来源：http://m.share.zdbjq.cn/Article/details/gkdrkzhma.sHtML

while (std::getline(in, line)) { }
来源：http://www.blog.hesvh.cn/Article/details/gqvkbccit.sHtML

[S49] C++：写文件
来源：http://blog.hesvh.cn/Article/details/gphhomfzs.sHtML

std::ofstream out("a.txt");  out << "hi\n";
来源：http://mobile.hesvh.cn/Article/details/ggjnvmkgb.sHtML

[S50] C++：格式化数字
来源：http://mobile.hesvh.cn/Article/details/gfwzkywwc.sHtML

std::ostringstream os;  os << std::fixed << std::setprecision(2) << 3.14159;
来源：http://wap.zdbjq.cn/Article/details/goqcdubqv.sHtML

[S51] C++：显式类型转换
来源：http://m.share.hesvh.cn/Article/details/gifqboxfh.sHtML

static_cast<double>(a) / b
来源：http://mobile.hesvh.cn/Article/details/gwtiawmli.sHtML

[S52] C++：const 与 noexcept
来源：http://3g.hesvh.cn/Article/details/ginbuoogr.sHtML

int size() const noexcept { return n_; }
来源：http://www.m.share.fehbvm.com/Article/details/glwikfywk.sHtML

[S53] C++：移动语义
来源：http://3g.zdbjq.cn/Article/details/giirdqeok.sHtML

std::vector<int> w = std::move(v);
来源：http://m.share.zdbjq.cn/Article/details/geociewwd.sHtML

[S54] C++：异常处理
来源：http://mobile.fehbvm.com/Article/details/ggyunhbov.sHtML

try { throw std::runtime_error("x"); } catch (const std::exception &e) { }
来源：http://www.m.share.zdbjq.cn/Article/details/ggwewytth.sHtML

[S55] C++：结构化绑定
来源：http://www.m.share.fehbvm.com/Article/details/gpqgremmm.sHtML

auto [a, b] = std::make_pair(1, 2);
来源：http://mobile.hesvh.cn/Article/details/gswyxrvfb.sHtML

[S56] C++：optional
来源：http://www.blog.hesvh.cn/Article/details/gdblkjtqq.sHtML

std::optional<int> o = 5;  if (o) { int v = *o; }
来源：http://www.m.share.zdbjq.cn/Article/details/gepuqqolb.sHtML

[S57] C++：编译期常量
来源：http://www.m.share.zdbjq.cn/Article/details/gkvxaxmln.sHtML

constexpr int N = 10;
来源：http://www.m.share.zdbjq.cn/Article/details/gcmdiavyn.sHtML

[S58] C++：命名空间
来源：http://3g.hesvh.cn/Article/details/gdoyhuvya.sHtML

namespace ns { int f() { return 1; } }
来源：http://www.blog.fehbvm.com/Article/details/gdyphhqnk.sHtML

[S59] C++：静态断言
来源：http://www.blog.fehbvm.com/Article/details/gcotlsymu.sHtML

static_assert(sizeof(int) == 4, "int 必须 4 字节");
来源：http://www.blog.zdbjq.cn/Article/details/gcfxdfhle.sHtML

[S60] C++：遍历并删除元素
来源：http://mobile.fehbvm.com/Article/details/guukxcamk.sHtML

v.erase(std::remove_if(v.begin(), v.end(), [](int x) { return x < 0; }), v.end());
来源：http://www.share.zdbjq.cn/Article/details/grwguqaym.sHtML

================================================================================
来源：http://read.share.zdbjq.cn/Article/details/gdpydpcri.sHtML

T. 其他语言补充（Kotlin / Swift / Lua / Perl / Scala）
来源：http://wap.zdbjq.cn/Article/details/gukwyrork.sHtML

================================================================================
来源：http://www.share.zdbjq.cn/Article/details/gpwrblugs.sHtML

[T01] Kotlin：Hello World
来源：http://baike.hesvh.cn/Article/details/ggiryutzt.sHtML

println("Hello")
来源：http://wap.zdbjq.cn/Article/details/gemldddny.sHtML

[T02] Kotlin：变量
来源：http://m.share.zdbjq.cn/Article/details/gsrbxdcmu.sHtML

val a = 1;  var b = 2        // val 只读，var 可变
来源：http://wap.hesvh.cn/Article/details/gpcrtvkub.sHtML

[T03] Kotlin：字符串模板
来源：http://www.m.share.hesvh.cn/Article/details/gdrqkpcvb.sHtML

"值: $b"
来源：http://m.share.hesvh.cn/Article/details/gtnlhlntl.sHtML

[T04] Kotlin：空安全
来源：http://m.share.hesvh.cn/Article/details/ggozuegwt.sHtML

val n: String? = null;  n?.length
来源：http://www.share.zdbjq.cn/Article/details/gjbvwoony.sHtML

[T05] Kotlin：when 表达式
来源：http://blog.hesvh.cn/Article/details/gkicmrqvc.sHtML

val s = when (x) { 1 -> "一" else -> "其他" }   // 多分支时每个分支单独一行
来源：http://www.m.share.zdbjq.cn/Article/details/ghbrmzofo.sHtML

[T06] Kotlin：集合映射
来源：http://www.blog.zdbjq.cn/Article/details/gfxvmfbwr.sHtML

listOf(1, 2, 3).map { it * 2 }
来源：http://baike.zdbjq.cn/Article/details/gugaikgwp.sHtML

[T07] Kotlin：集合过滤
来源：http://www.blog.fehbvm.com/Article/details/gaiothrie.sHtML

listOf(1, 2, 3).filter { it > 1 }
来源：http://m.share.zdbjq.cn/Article/details/gavqymmve.sHtML

[T08] Kotlin：数据类
来源：http://read.share.fehbvm.com/Article/details/gfqxkrtgq.sHtML

data class User(val name: String, val age: Int)
来源：http://mobile.hesvh.cn/Article/details/ghqgtuxum.sHtML

[T09] Kotlin：扩展函数
来源：http://mobile.fehbvm.com/Article/details/gigfwsyse.sHtML

fun String.exclaim() = this + "!"
来源：http://baike.hesvh.cn/Article/details/gsksxtzjb.sHtML

[T10] Kotlin：默认参数
来源：http://3g.hesvh.cn/Article/details/gtfxrfacc.sHtML

fun greet(name: String = "World") = "Hi $name"
来源：http://wap.fehbvm.com/Article/details/gaefkwbfs.sHtML

[T11] Kotlin：协程
来源：http://blog.zdbjq.cn/Article/details/gjbzuurku.sHtML

GlobalScope.launch { delay(1000); println("done") }
来源：http://www.m.share.hesvh.cn/Article/details/gazqdhydn.sHtML

[T12] Kotlin：解构声明
来源：http://www.blog.fehbvm.com/Article/details/gryefzlcr.sHtML

val (a, b) = Pair(1, 2)
来源：http://www.m.share.zdbjq.cn/Article/details/gbphgwveg.sHtML

[T13] Kotlin：只读 Map
来源：http://blog.hesvh.cn/Article/details/gmtzxlvuh.sHtML

val m = mapOf("a" to 1)
来源：http://www.blog.zdbjq.cn/Article/details/grztrzvqg.sHtML

[T14] Kotlin：循环
来源：http://www.blog.fehbvm.com/Article/details/ghcjyttin.sHtML

for (i in 1..10) println(i)
来源：http://m.share.fehbvm.com/Article/details/geigldpzv.sHtML

[T15] Kotlin：接口
来源：http://www.m.share.hesvh.cn/Article/details/griuanqzd.sHtML

interface Shape { fun area(): Double }
来源：http://mobile.zdbjq.cn/Article/details/gbczxtzas.sHtML

[T16] Swift：Hello World
来源：http://www.blog.zdbjq.cn/Article/details/gtmmzshga.sHtML

print("Hello")
来源：http://baike.zdbjq.cn/Article/details/glnwinxcn.sHtML

[T17] Swift：变量与常量
来源：http://www.blog.fehbvm.com/Article/details/gkwmsqdow.sHtML

var a = 1;  let b = 2
来源：http://3g.zdbjq.cn/Article/details/gqbfgfroh.sHtML

[T18] Swift：字符串插值
来源：http://www.share.hesvh.cn/Article/details/grizrltxr.sHtML

"值: \(b)"
来源：http://baike.hesvh.cn/Article/details/ggaoxepjj.sHtML

[T19] Swift：可选绑定
来源：http://m.share.fehbvm.com/Article/details/gcktrbzqc.sHtML

if let n = opt { print(n) }
来源：http://baike.zdbjq.cn/Article/details/gdqqeadwr.sHtML

[T20] Swift：数组操作
来源：http://www.share.zdbjq.cn/Article/details/gxowgjgan.sHtML

var a = [1, 2, 3];  a.append(4)
来源：http://www.m.share.hesvh.cn/Article/details/gbofhvohm.sHtML

[T21] Swift：遍历
来源：http://www.blog.zdbjq.cn/Article/details/gtpunpbyu.sHtML

for x in a { print(x) }
来源：http://mobile.zdbjq.cn/Article/details/gldwachcb.sHtML

[T22] Swift：字典
来源：http://www.m.share.fehbvm.com/Article/details/gmlbzqpil.sHtML

var d = ["a": 1];  d["b"] = 2
来源：http://baike.zdbjq.cn/Article/details/gtdxxaksq.sHtML

[T23] Swift：函数
来源：http://www.m.share.zdbjq.cn/Article/details/gjfdclfcg.sHtML

func add(_ a: Int, _ b: Int) -> Int { a + b }
来源：http://read.share.hesvh.cn/Article/details/gllhajicy.sHtML

[T24] Swift：闭包
来源：http://wap.fehbvm.com/Article/details/gaubfwpwb.sHtML

let f = { (x: Int) -> Int in x * 2 }
来源：http://read.share.fehbvm.com/Article/details/glpnyjnmz.sHtML

[T25] Swift：结构体
来源：http://blog.hesvh.cn/Article/details/gmnevjpgq.sHtML

struct P { var x: Int }
来源：http://read.share.hesvh.cn/Article/details/gbspsgvbc.sHtML

[T26] Swift：类与重写
来源：http://blog.fehbvm.com/Article/details/gnjzzxeby.sHtML

class A: Base { override func f() {} }
来源：http://read.share.hesvh.cn/Article/details/grqooahte.sHtML

[T27] Swift：错误处理
来源：http://wap.hesvh.cn/Article/details/goqpitplh.sHtML

do { try f() } catch { print(error) }
来源：http://m.share.fehbvm.com/Article/details/gecdedikb.sHtML

[T28] Swift：枚举
来源：http://www.blog.hesvh.cn/Article/details/grtvxwdeo.sHtML

enum Color { case red, green }
来源：http://www.share.fehbvm.com/Article/details/gmxgqkqug.sHtML

[T29] Swift：guard 提前返回
来源：http://m.share.zdbjq.cn/Article/details/gcepgpaqp.sHtML

guard let x = opt else { return }
来源：http://www.m.share.zdbjq.cn/Article/details/gygfuqpbw.sHtML

[T30] Swift：协议
来源：http://baike.zdbjq.cn/Article/details/gxvkuczig.sHtML

protocol Shape { func area() -> Double }
来源：http://wap.fehbvm.com/Article/details/gpxqcrpst.sHtML

[T31] Lua：Hello World
来源：http://www.m.share.zdbjq.cn/Article/details/gxwmslkwg.sHtML

print("Hello")
来源：http://3g.hesvh.cn/Article/details/ghyxiudbm.sHtML

[T32] Lua：局部变量
来源：http://blog.zdbjq.cn/Article/details/gmqnpyzdh.sHtML

local a = 1
来源：http://read.share.hesvh.cn/Article/details/gaftsmwfk.sHtML

[T33] Lua：表（数组）
来源：http://blog.fehbvm.com/Article/details/govoywjrk.sHtML

local t = {1, 2, 3};  t[4] = 4
来源：http://baike.fehbvm.com/Article/details/gvcywwygi.sHtML

[T34] Lua：遍历表
来源：http://www.share.hesvh.cn/Article/details/gzgtfggqv.sHtML

for i, v in ipairs(t) do print(i, v) end
来源：http://www.m.share.hesvh.cn/Article/details/gatayywqd.sHtML

[T35] Lua：字典表
来源：http://m.share.zdbjq.cn/Article/details/glprrghbm.sHtML

local d = { a = 1 };  d.b = 2
来源：http://www.share.zdbjq.cn/Article/details/gfoyvgfmt.sHtML

[T36] Lua：函数
来源：http://m.share.fehbvm.com/Article/details/gmtohurwt.sHtML

function add(a, b) return a + b end
来源：http://3g.zdbjq.cn/Article/details/giikeswxq.sHtML

[T37] Lua：字符串拼接
来源：http://www.m.share.fehbvm.com/Article/details/gaecridas.sHtML

"a" .. "b"
来源：http://wap.hesvh.cn/Article/details/gzwhwrkxn.sHtML

[T38] Lua：条件
来源：http://m.share.zdbjq.cn/Article/details/gbjbudnlp.sHtML

if x > 0 then print("正") end
来源：http://www.share.zdbjq.cn/Article/details/gogddwnqi.sHtML

[T39] Lua：模式匹配
来源：http://www.m.share.zdbjq.cn/Article/details/gbccgoyfk.sHtML

string.find(s, "%d+")
来源：http://blog.zdbjq.cn/Article/details/gxudsokbt.sHtML

[T40] Lua：元表
来源：http://wap.zdbjq.cn/Article/details/glllhwcdp.sHtML

setmetatable({}, { __index = base })
来源：http://mobile.hesvh.cn/Article/details/ginfjiahg.sHtML

[T41] Perl：Hello World
来源：http://wap.zdbjq.cn/Article/details/gkuvpubsf.sHtML

print "Hello\n";
来源：http://m.share.zdbjq.cn/Article/details/gybjrjicq.sHtML

[T42] Perl：变量类型
来源：http://www.m.share.zdbjq.cn/Article/details/gufhjpwzj.sHtML

my $a = 1;  my @arr = (1, 2, 3);  my %h = (a => 1);
来源：http://wap.zdbjq.cn/Article/details/gvoytayuf.sHtML

[T43] Perl：字符串插值
来源：http://m.share.hesvh.cn/Article/details/gnwytiztz.sHtML

"值: $a"
来源：http://3g.fehbvm.com/Article/details/gedlsjbky.sHtML

[T44] Perl：条件
来源：http://wap.hesvh.cn/Article/details/gjuabtgaf.sHtML

if ($a > 0) { print "正"; }
来源：http://m.share.hesvh.cn/Article/details/gcllbsakb.sHtML

[T45] Perl：数组遍历
来源：http://wap.fehbvm.com/Article/details/ghbihqfeg.sHtML

for my $x (@arr) { print $x; }
来源：http://www.share.fehbvm.com/Article/details/gevpovtwq.sHtML

[T46] Perl：哈希操作
来源：http://read.share.hesvh.cn/Article/details/gliileoxw.sHtML

$h{b} = 2;  for my $k (keys %h) { print "$k=$h{$k}"; }
来源：http://3g.fehbvm.com/Article/details/ggbmbpzyp.sHtML

[T47] Perl：正则捕获
来源：http://mobile.fehbvm.com/Article/details/gtatqsipu.sHtML

if ($s =~ /(\d+)/) { print $1; }
来源：http://www.m.share.hesvh.cn/Article/details/gqltqmjdk.sHtML

[T48] Perl：正则替换
来源：http://3g.fehbvm.com/Article/details/ggbaejdct.sHtML

$s =~ s/old/new/g;
来源：http://m.share.zdbjq.cn/Article/details/gricuvnlv.sHtML

[T49] Perl：函数
来源：http://baike.fehbvm.com/Article/details/ginoubvpg.sHtML

sub add { my ($a, $b) = @_; return $a + $b; }
来源：http://www.share.fehbvm.com/Article/details/gshmearqk.sHtML

[T50] Perl：逐行读文件
来源：http://www.blog.fehbvm.com/Article/details/gxzyagxap.sHtML

open my $fh, "<", "a.txt" or die $!;
来源：http://mobile.zdbjq.cn/Article/details/guqlrdqhc.sHtML

while (my $line = <$fh>) { print $line; }
来源：http://mobile.hesvh.cn/Article/details/gaappibyp.sHtML

[T51] Scala：Hello World
来源：http://www.share.fehbvm.com/Article/details/gekgpztmi.sHtML

println("Hello")
来源：http://m.share.fehbvm.com/Article/details/gbxdyscos.sHtML

[T52] Scala：变量
来源：http://3g.hesvh.cn/Article/details/gqfyxixhp.sHtML

val a = 1;  var b = 2
来源：http://mobile.zdbjq.cn/Article/details/gwjarlkbd.sHtML

[T53] Scala：字符串插值
来源：http://3g.fehbvm.com/Article/details/gmlmtyegv.sHtML

s"值: $b"
来源：http://m.share.hesvh.cn/Article/details/genkzcftw.sHtML

[T54] Scala：集合映射
来源：http://wap.fehbvm.com/Article/details/ghuwjhigp.sHtML

List(1, 2, 3).map(_ * 2)
来源：http://wap.hesvh.cn/Article/details/grxhawwyp.sHtML

[T55] Scala：集合过滤
来源：http://www.m.share.hesvh.cn/Article/details/gypmmjmum.sHtML

List(1, 2, 3).filter(_ > 1)
来源：http://www.share.zdbjq.cn/Article/details/gxfjipqch.sHtML

[T56] Scala：样例类
来源：http://www.share.hesvh.cn/Article/details/gtgeefcuz.sHtML

case class User(name: String, age: Int)
来源：http://www.m.share.fehbvm.com/Article/details/gmecyzsch.sHtML

[T57] Scala：模式匹配
来源：http://blog.fehbvm.com/Article/details/gksbutxka.sHtML

x match { case 1 => "一"; case _ => "其他" }
来源：http://read.share.hesvh.cn/Article/details/gekodtlrw.sHtML

[T58] Scala：函数定义
来源：http://m.share.zdbjq.cn/Article/details/gavmwkcrn.sHtML

def add(a: Int, b: Int): Int = a + b
来源：http://baike.zdbjq.cn/Article/details/gxfvlaehx.sHtML

[T59] Scala：循环
来源：http://www.blog.zdbjq.cn/Article/details/glmhbedtf.sHtML

for (i <- 1 to 10) println(i)
来源：http://www.m.share.hesvh.cn/Article/details/gemfcgvzd.sHtML

[T60] Scala：折叠
来源：http://m.share.zdbjq.cn/Article/details/glvpyjlmc.sHtML

List(1, 2, 3).foldLeft(0)(_ + _)
来源：http://read.share.zdbjq.cn/Article/details/gifdauflg.sHtML

================================================================================
来源：http://m.share.hesvh.cn/Article/details/gxnfjerpn.sHtML

U. 高频实用片段（Python / PHP / JavaScript 各 40 条）
来源：http://blog.hesvh.cn/Article/details/gvmieykpm.sHtML

================================================================================
来源：http://www.m.share.zdbjq.cn/Article/details/gejyimadr.sHtML

[U01] Py：创建虚拟环境
来源：http://m.share.fehbvm.com/Article/details/gcsjhuios.sHtML

python -m venv .venv && source .venv/bin/activate
来源：http://wap.fehbvm.com/Article/details/ghwxgddxp.sHtML

[U02] Py：导出 / 安装依赖
来源：http://www.share.fehbvm.com/Article/details/gxgdjaion.sHtML

pip freeze > requirements.txt;  pip install -r requirements.txt
来源：http://3g.fehbvm.com/Article/details/gbcpgxquy.sHtML

[U03] Py：加载 .env 配置
来源：http://mobile.hesvh.cn/Article/details/gmachlzdg.sHtML

from dotenv import load_dotenv; load_dotenv()
来源：http://wap.zdbjq.cn/Article/details/gyadjpugj.sHtML

[U04] Py：变量调试打印
来源：http://3g.zdbjq.cn/Article/details/gexuibnfj.sHtML

print(f"{x=}")            # 输出 x=值，Python 3.8+
来源：http://baike.fehbvm.com/Article/details/gftqvbcai.sHtML

[U05] Py：列表去重且保序
来源：http://baike.fehbvm.com/Article/details/gweulbibt.sHtML

list(dict.fromkeys(arr))
来源：http://read.share.fehbvm.com/Article/details/ghqbfudqt.sHtML

[U06] Py：合并两个字典
来源：http://www.share.hesvh.cn/Article/details/gdwzgoraq.sHtML

{**a, **b}
来源：http://mobile.zdbjq.cn/Article/details/gnwwodtbc.sHtML

[U07] Py：反转字典键值
来源：http://www.blog.fehbvm.com/Article/details/gbncbfeet.sHtML

{v: k for k, v in d.items()}
来源：http://blog.fehbvm.com/Article/details/grucilkax.sHtML

[U08] Py：展平二维列表
来源：http://3g.hesvh.cn/Article/details/gnhqkzlyw.sHtML

[y for x in nested for y in x]
来源：http://wap.hesvh.cn/Article/details/gvuqdhjvh.sHtML


<!-- 参考信息 -->