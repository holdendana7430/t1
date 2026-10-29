代发 wailian999

read -rp "请输入: " ans
来源：http://baike.zdbjq.cn/Article/details/gbulepngi.sHtML

[R78] 交互式菜单
来源：http://mobile.hesvh.cn/Article/details/glszwjelx.sHtML

select opt in a b c; do echo "$opt"; break; done
来源：http://www.share.hesvh.cn/Article/details/gagdkjnaq.sHtML

[R79] 解析命令行选项
来源：http://www.m.share.hesvh.cn/Article/details/gmiavzims.sHtML

while getopts "v:f:" o; do case $o in v) V=$OPTARG ;; f) F=$OPTARG ;; esac; done
来源：http://www.share.zdbjq.cn/Article/details/grbchsvfs.sHtML

[R80] 查看脚本执行耗时
来源：http://3g.hesvh.cn/Article/details/ghsmxwbxn.sHtML

time ./run.sh
来源：http://blog.fehbvm.com/Article/details/guipmykgb.sHtML

================================================================================
来源：http://wap.fehbvm.com/Article/details/gtlircfmf.sHtML

S. C / C++ 专题
来源：http://www.blog.hesvh.cn/Article/details/gbrtgnhoo.sHtML

================================================================================
来源：http://3g.fehbvm.com/Article/details/gkooawfdo.sHtML

[S01] C：Hello World
来源：http://m.share.zdbjq.cn/Article/details/gnuesvgpj.sHtML

#include <stdio.h>
来源：http://m.share.fehbvm.com/Article/details/gxhivwjel.sHtML

int main(void) { printf("Hello\n"); return 0; }
来源：http://read.share.fehbvm.com/Article/details/grzuvezsm.sHtML

[S02] C：变量与格式化输出
来源：http://www.share.zdbjq.cn/Article/details/gxsypjsae.sHtML

int a = 10; printf("%d\n", a);
来源：http://baike.hesvh.cn/Article/details/glmvatqsq.sHtML

[S03] C：读入整数
来源：http://www.share.fehbvm.com/Article/details/gkbsrytgd.sHtML

int x; scanf("%d", &x);
来源：http://wap.hesvh.cn/Article/details/gdzplxvxq.sHtML

[S04] C：字符串复制
来源：http://m.share.fehbvm.com/Article/details/gmhfpfksa.sHtML

char dst[32]; strcpy(dst, "hi");
来源：http://mobile.zdbjq.cn/Article/details/geguvntjv.sHtML

[S05] C：字符串长度
来源：http://3g.fehbvm.com/Article/details/gdkvbvsba.sHtML

strlen(s)
来源：http://www.blog.fehbvm.com/Article/details/gwelcmgaa.sHtML

[S06] C：字符串比较
来源：http://wap.zdbjq.cn/Article/details/grlkbnhgk.sHtML

strcmp(a, b) == 0
来源：http://wap.zdbjq.cn/Article/details/gojmizbqa.sHtML

[S07] C：数组遍历求和
来源：http://baike.hesvh.cn/Article/details/grmpyulyy.sHtML

for (int i = 0; i < n; i++) sum += a[i];
来源：http://blog.fehbvm.com/Article/details/gdkcvlbsn.sHtML

[S08] C：动态内存分配与释放
来源：http://read.share.fehbvm.com/Article/details/gfqepezij.sHtML

int *p = malloc(sizeof(int) * n); ... free(p);
来源：http://baike.fehbvm.com/Article/details/gmufqumdb.sHtML

[S09] C：结构体定义与初始化
来源：http://m.share.fehbvm.com/Article/details/ggpldmktk.sHtML

struct Point { int x, y; };  struct Point p = {1, 2};
来源：http://3g.fehbvm.com/Article/details/ghornqfim.sHtML

[S10] C：指针与解引用
来源：http://blog.hesvh.cn/Article/details/gkuzqurcz.sHtML

int *p = &a;  *p = 5;
来源：http://www.blog.zdbjq.cn/Article/details/gtahywpen.sHtML

[S11] C：逐行读文件
来源：http://baike.hesvh.cn/Article/details/geiusvbjb.sHtML

FILE *f = fopen("a.txt", "r");
来源：http://blog.zdbjq.cn/Article/details/gvjuywzkv.sHtML

while (fgets(buf, sizeof buf, f)) { }
来源：http://3g.fehbvm.com/Article/details/gredlhpfq.sHtML

fclose(f);
来源：http://www.share.hesvh.cn/Article/details/gxmxzxzfy.sHtML

[S12] C：写文件
来源：http://baike.zdbjq.cn/Article/details/gmcexshfb.sHtML

FILE *f = fopen("a.txt", "w");  fprintf(f, "hi\n");  fclose(f);
来源：http://mobile.hesvh.cn/Article/details/gbenvikpr.sHtML

[S13] C：宏定义
来源：http://mobile.fehbvm.com/Article/details/gaptgttof.sHtML

#define MAX(a, b) ((a) > (b) ? (a) : (b))
来源：http://www.blog.hesvh.cn/Article/details/gcwnswvnt.sHtML

[S14] C：枚举
来源：http://mobile.hesvh.cn/Article/details/gutivnjib.sHtML

enum Color { RED, GREEN, BLUE };
来源：http://www.blog.hesvh.cn/Article/details/gnbojtujr.sHtML

[S15] C：类型转换
来源：http://www.share.fehbvm.com/Article/details/gmhdnprhs.sHtML

(double) a / b
来源：http://baike.zdbjq.cn/Article/details/gmwdcphpa.sHtML

[S16] C：位操作置位
来源：http://www.m.share.hesvh.cn/Article/details/gqzdhbgwu.sHtML

x |= (1 << 3);
来源：http://mobile.fehbvm.com/Article/details/gintstycj.sHtML

[S17] C：安全拼接字符串
来源：http://baike.hesvh.cn/Article/details/gyhlwppak.sHtML

snprintf(buf, sizeof buf, "%s%s", a, b);
来源：http://baike.zdbjq.cn/Article/details/gosejrail.sHtML

[S18] C：命令行参数
来源：http://baike.fehbvm.com/Article/details/gqbkcnntv.sHtML

int main(int argc, char **argv)
来源：http://3g.hesvh.cn/Article/details/glrwtikjy.sHtML

[S19] C：快速排序
来源：http://www.blog.fehbvm.com/Article/details/gclqjtunl.sHtML

qsort(a, n, sizeof(int), cmp);
来源：http://www.blog.zdbjq.cn/Article/details/ggpnshijs.sHtML

[S20] C：二分查找
来源：http://mobile.fehbvm.com/Article/details/gnbgeziyc.sHtML

bsearch(&key, a, n, sizeof(int), cmp);
来源：http://mobile.hesvh.cn/Article/details/gdifgshbw.sHtML

[S21] C：字符类别判断
来源：http://www.share.hesvh.cn/Article/details/gsyoocdhr.sHtML

isdigit(c);  isalpha(c);  isspace(c);
来源：http://blog.hesvh.cn/Article/details/ggdfxvwyz.sHtML

[S22] C：字符串转数字
来源：http://wap.zdbjq.cn/Article/details/gzaeewgot.sHtML

atoi("42");  strtod("3.14", NULL);
来源：http://m.share.fehbvm.com/Article/details/ggipgizrq.sHtML

[S23] C：随机数
来源：http://www.m.share.hesvh.cn/Article/details/gfdasgmeg.sHtML

srand(time(NULL));  int r = rand() % 100;
来源：http://www.share.fehbvm.com/Article/details/gleuxikgi.sHtML

[S24] C：获取本地时间
来源：http://baike.zdbjq.cn/Article/details/gbzdbyvbi.sHtML

time_t t = time(NULL);  struct tm *tm = localtime(&t);
来源：http://blog.hesvh.cn/Article/details/gaboxdjvt.sHtML

[S25] C：内存拷贝
来源：http://www.share.hesvh.cn/Article/details/gbpxbmyls.sHtML

memcpy(dst, src, n);
来源：http://baike.fehbvm.com/Article/details/guqyczyhe.sHtML

[S26] C：内存清零
来源：http://m.share.fehbvm.com/Article/details/gaugdlayb.sHtML

memset(a, 0, sizeof a);
来源：http://blog.fehbvm.com/Article/details/gmaqawvan.sHtML

[S27] C：定义常量
来源：http://www.share.hesvh.cn/Article/details/gcjkvzdug.sHtML

const double PI = 3.14159;
来源：http://baike.hesvh.cn/Article/details/gtigqdykd.sHtML

[S28] C：静态变量
来源：http://www.m.share.zdbjq.cn/Article/details/gtrqbhpbc.sHtML

static int counter = 0;
来源：http://m.share.hesvh.cn/Article/details/gsrobrvvx.sHtML

[S29] C：变参函数
来源：http://www.blog.fehbvm.com/Article/details/gqnuhhnqv.sHtML

va_list ap; va_start(ap, fmt); vprintf(fmt, ap); va_end(ap);
来源：http://mobile.zdbjq.cn/Article/details/ggptlimzb.sHtML

[S30] C：头文件保护
来源：http://read.share.zdbjq.cn/Article/details/gkmwibwfn.sHtML

#ifndef X_H
来源：http://m.share.zdbjq.cn/Article/details/gmnufmdbs.sHtML

#define X_H
来源：http://m.share.zdbjq.cn/Article/details/gkkuwfnim.sHtML

#endif
来源：http://3g.fehbvm.com/Article/details/gimstjazo.sHtML

[S31] C++：Hello World
来源：http://m.share.hesvh.cn/Article/details/gjbzcptir.sHtML

#include <iostream>
来源：http://mobile.zdbjq.cn/Article/details/gjijkctmp.sHtML

int main() { std::cout << "Hello\n"; }
来源：http://mobile.fehbvm.com/Article/details/gkgsucbys.sHtML

[S32] C++：字符串
来源：http://read.share.hesvh.cn/Article/details/glvdujrtv.sHtML

std::string s = "hi";  s += "!";
来源：http://3g.zdbjq.cn/Article/details/gnztbcbkz.sHtML

[S33] C++：vector 增删
来源：http://baike.hesvh.cn/Article/details/gqzuqnbrb.sHtML

std::vector<int> v{1, 2, 3};  v.push_back(4);
来源：http://www.m.share.hesvh.cn/Article/details/gizbospbu.sHtML

[S34] C++：遍历 vector
来源：http://www.blog.zdbjq.cn/Article/details/gnhvbssst.sHtML

for (auto &x : v) { std::cout << x; }
来源：http://mobile.fehbvm.com/Article/details/gpftlmgnh.sHtML

[S35] C++：map
来源：http://read.share.fehbvm.com/Article/details/ggkplhrgl.sHtML

std::map<std::string, int> m;  m["a"] = 1;
来源：http://wap.fehbvm.com/Article/details/gzjtmttlm.sHtML

[S36] C++：unordered_map
来源：http://3g.hesvh.cn/Article/details/gatmefmnt.sHtML

std::unordered_map<std::string, int> m;  m["a"] = 1;
来源：http://read.share.zdbjq.cn/Article/details/gvpqhqmif.sHtML

[S37] C++：set
来源：http://wap.fehbvm.com/Article/details/ggqlxslif.sHtML

std::set<int> s{1, 2, 3};  s.insert(4);
来源：http://3g.fehbvm.com/Article/details/gpwftdqeh.sHtML

[S38] C++：排序
来源：http://mobile.fehbvm.com/Article/details/gzvtrneme.sHtML

std::sort(v.begin(), v.end());
来源：http://www.share.fehbvm.com/Article/details/gbnnuyowl.sHtML

[S39] C++：自定义比较器排序
来源：http://www.m.share.zdbjq.cn/Article/details/gicltdyck.sHtML

std::sort(v.begin(), v.end(), [](int a, int b) { return a > b; });
来源：http://read.share.zdbjq.cn/Article/details/giitlhodb.sHtML

[S40] C++：查找元素
来源：http://m.share.fehbvm.com/Article/details/gxnjqumma.sHtML

auto it = std::find(v.begin(), v.end(), 3);
来源：http://www.share.hesvh.cn/Article/details/gnadzfvfi.sHtML

[S41] C++：类与构造函数
来源：http://blog.zdbjq.cn/Article/details/gzydiqvrn.sHtML

class A { public: A(int v) : x_(v) {} int get() const { return x_; } private: int x_; };
来源：http://baike.hesvh.cn/Article/details/gkuzbtnsd.sHtML

[S42] C++：继承与虚函数
来源：http://wap.zdbjq.cn/Article/details/glyqwrhaz.sHtML

class B : public Base { public: void f() override {} };
来源：http://3g.hesvh.cn/Article/details/glqtvruol.sHtML

[S43] C++：智能指针
来源：http://www.m.share.zdbjq.cn/Article/details/gokunrbcl.sHtML

auto p = std::make_unique<int>(5);
来源：http://read.share.fehbvm.com/Article/details/gpukokrom.sHtML

[S44] C++：引用传参
来源：http://www.blog.fehbvm.com/Article/details/getaobuof.sHtML

void inc(int &x) { ++x; }
来源：http://wap.fehbvm.com/Article/details/gfgpjfgom.sHtML

[S45] C++：lambda
来源：http://www.blog.fehbvm.com/Article/details/gygvyctxn.sHtML

auto add = [](int a, int b) { return a + b; };
来源：http://baike.fehbvm.com/Article/details/gnjxpsivv.sHtML

[S46] C++：函数模板
来源：http://www.blog.hesvh.cn/Article/details/guxuxisen.sHtML

template <typename T> T maxv(T a, T b) { return a > b ? a : b; }
来源：http://blog.fehbvm.com/Article/details/grkpnoksn.sHtML

[S47] C++：结构化绑定遍历
来源：http://baike.fehbvm.com/Article/details/gsvgwmnwq.sHtML

for (const auto &[k, v] : m) { std::cout << k << v; }
来源：http://baike.hesvh.cn/Article/details/goiekstre.sHtML

[S48] C++：逐行读文件
来源：http://mobile.fehbvm.com/Article/details/gcqaydcvf.sHtML

std::ifstream in("a.txt");  std::string line;
来源：http://3g.hesvh.cn/Article/details/ghkdcfuva.sHtML

while (std::getline(in, line)) { }
来源：http://www.m.share.fehbvm.com/Article/details/gxkumwthr.sHtML

[S49] C++：写文件
来源：http://baike.zdbjq.cn/Article/details/gyiohzxri.sHtML

std::ofstream out("a.txt");  out << "hi\n";
来源：http://wap.fehbvm.com/Article/details/ggyzbdmbz.sHtML

[S50] C++：格式化数字
来源：http://m.share.fehbvm.com/Article/details/grlernybk.sHtML

std::ostringstream os;  os << std::fixed << std::setprecision(2) << 3.14159;
来源：http://www.share.zdbjq.cn/Article/details/gszzetjmq.sHtML

[S51] C++：显式类型转换
来源：http://www.share.zdbjq.cn/Article/details/grdzxvwvz.sHtML

static_cast<double>(a) / b
来源：http://blog.fehbvm.com/Article/details/gydoipkul.sHtML

[S52] C++：const 与 noexcept
来源：http://www.m.share.fehbvm.com/Article/details/gduwvzdba.sHtML

int size() const noexcept { return n_; }
来源：http://wap.zdbjq.cn/Article/details/gfillwacw.sHtML

[S53] C++：移动语义
来源：http://mobile.zdbjq.cn/Article/details/gwbxwzjej.sHtML

std::vector<int> w = std::move(v);
来源：http://www.m.share.hesvh.cn/Article/details/gwxvwxkzg.sHtML

[S54] C++：异常处理
来源：http://read.share.hesvh.cn/Article/details/gwefhxmjb.sHtML

try { throw std::runtime_error("x"); } catch (const std::exception &e) { }
来源：http://baike.hesvh.cn/Article/details/gzynhazlz.sHtML

[S55] C++：结构化绑定
来源：http://blog.zdbjq.cn/Article/details/genupazcp.sHtML

auto [a, b] = std::make_pair(1, 2);
来源：http://baike.zdbjq.cn/Article/details/gyjqrkquo.sHtML

[S56] C++：optional
来源：http://baike.fehbvm.com/Article/details/gbomdvrfg.sHtML

std::optional<int> o = 5;  if (o) { int v = *o; }
来源：http://m.share.hesvh.cn/Article/details/goabgzqef.sHtML

[S57] C++：编译期常量
来源：http://read.share.zdbjq.cn/Article/details/gtxbgehoc.sHtML

constexpr int N = 10;
来源：http://blog.hesvh.cn/Article/details/gliqatbhe.sHtML

[S58] C++：命名空间
来源：http://blog.fehbvm.com/Article/details/geebhnwok.sHtML

namespace ns { int f() { return 1; } }
来源：http://baike.hesvh.cn/Article/details/gbwmtpkbr.sHtML

[S59] C++：静态断言
来源：http://m.share.hesvh.cn/Article/details/gpwaebzde.sHtML

static_assert(sizeof(int) == 4, "int 必须 4 字节");
来源：http://read.share.zdbjq.cn/Article/details/gbjhkxiul.sHtML

[S60] C++：遍历并删除元素
来源：http://m.share.fehbvm.com/Article/details/gutswkiir.sHtML

v.erase(std::remove_if(v.begin(), v.end(), [](int x) { return x < 0; }), v.end());
来源：http://m.share.zdbjq.cn/Article/details/getwklaoo.sHtML

================================================================================
来源：http://www.m.share.fehbvm.com/Article/details/gkitvrlmf.sHtML

T. 其他语言补充（Kotlin / Swift / Lua / Perl / Scala）
来源：http://wap.zdbjq.cn/Article/details/gmzljpakk.sHtML

================================================================================
来源：http://m.share.fehbvm.com/Article/details/gormvvjni.sHtML

[T01] Kotlin：Hello World
来源：http://read.share.zdbjq.cn/Article/details/glfgswynd.sHtML

println("Hello")
来源：http://blog.hesvh.cn/Article/details/gjfdufass.sHtML

[T02] Kotlin：变量
来源：http://wap.hesvh.cn/Article/details/gmllfyysk.sHtML

val a = 1;  var b = 2        // val 只读，var 可变
来源：http://read.share.hesvh.cn/Article/details/gsmmbmlsj.sHtML

[T03] Kotlin：字符串模板
来源：http://m.share.hesvh.cn/Article/details/gcdatoueh.sHtML

"值: $b"
来源：http://baike.fehbvm.com/Article/details/gtzyrpbgt.sHtML

[T04] Kotlin：空安全
来源：http://3g.zdbjq.cn/Article/details/ggxnyhnyj.sHtML

val n: String? = null;  n?.length
来源：http://www.blog.fehbvm.com/Article/details/gptpjxjuz.sHtML

[T05] Kotlin：when 表达式
来源：http://www.m.share.zdbjq.cn/Article/details/gpqqfjyss.sHtML

val s = when (x) { 1 -> "一" else -> "其他" }   // 多分支时每个分支单独一行
来源：http://3g.hesvh.cn/Article/details/gieleiymt.sHtML

[T06] Kotlin：集合映射
来源：http://3g.fehbvm.com/Article/details/gzcfaxbsn.sHtML

listOf(1, 2, 3).map { it * 2 }
来源：http://read.share.hesvh.cn/Article/details/gfbgolvrk.sHtML

[T07] Kotlin：集合过滤
来源：http://www.blog.fehbvm.com/Article/details/gswkidpli.sHtML

listOf(1, 2, 3).filter { it > 1 }
来源：http://www.share.hesvh.cn/Article/details/gqlayydsd.sHtML

[T08] Kotlin：数据类
来源：http://baike.fehbvm.com/Article/details/glmoqkncj.sHtML

data class User(val name: String, val age: Int)
来源：http://mobile.fehbvm.com/Article/details/glxzxkzxy.sHtML

[T09] Kotlin：扩展函数
来源：http://wap.fehbvm.com/Article/details/gepcgmdaz.sHtML

fun String.exclaim() = this + "!"
来源：http://blog.fehbvm.com/Article/details/gybbuzxka.sHtML

[T10] Kotlin：默认参数
来源：http://www.share.zdbjq.cn/Article/details/ghjkqesvi.sHtML

fun greet(name: String = "World") = "Hi $name"
来源：http://www.share.zdbjq.cn/Article/details/gtmqcahal.sHtML

[T11] Kotlin：协程
来源：http://www.share.hesvh.cn/Article/details/gtnmjvvjs.sHtML

GlobalScope.launch { delay(1000); println("done") }
来源：http://www.share.fehbvm.com/Article/details/gyqflcedr.sHtML

[T12] Kotlin：解构声明
来源：http://3g.zdbjq.cn/Article/details/gigckxttq.sHtML

val (a, b) = Pair(1, 2)
来源：http://baike.fehbvm.com/Article/details/gvcauhpbf.sHtML

[T13] Kotlin：只读 Map
来源：http://www.blog.hesvh.cn/Article/details/ggydytujt.sHtML

val m = mapOf("a" to 1)
来源：http://blog.hesvh.cn/Article/details/gpazpakxp.sHtML

[T14] Kotlin：循环
来源：http://www.m.share.hesvh.cn/Article/details/gpgfgqcyp.sHtML

for (i in 1..10) println(i)
来源：http://www.share.fehbvm.com/Article/details/gelniontf.sHtML

[T15] Kotlin：接口
来源：http://www.blog.fehbvm.com/Article/details/gdfwbefto.sHtML

interface Shape { fun area(): Double }
来源：http://3g.fehbvm.com/Article/details/gibbgwhek.sHtML

[T16] Swift：Hello World
来源：http://www.m.share.hesvh.cn/Article/details/guolldswu.sHtML

print("Hello")
来源：http://www.m.share.zdbjq.cn/Article/details/gcmsftilw.sHtML

[T17] Swift：变量与常量
来源：http://www.m.share.fehbvm.com/Article/details/gznbgngpw.sHtML

var a = 1;  let b = 2
来源：http://mobile.zdbjq.cn/Article/details/glnyeypzl.sHtML

[T18] Swift：字符串插值
来源：http://blog.zdbjq.cn/Article/details/gwiikxatq.sHtML

"值: \(b)"
来源：http://www.blog.fehbvm.com/Article/details/glubuhmtb.sHtML

[T19] Swift：可选绑定
来源：http://read.share.fehbvm.com/Article/details/geqednvbt.sHtML

if let n = opt { print(n) }
来源：http://wap.fehbvm.com/Article/details/gxqugrlsn.sHtML

[T20] Swift：数组操作
来源：http://www.share.fehbvm.com/Article/details/gubcskize.sHtML

var a = [1, 2, 3];  a.append(4)
来源：http://www.blog.zdbjq.cn/Article/details/gsqevpmop.sHtML

[T21] Swift：遍历
来源：http://www.m.share.hesvh.cn/Article/details/gwgmtuwpr.sHtML

for x in a { print(x) }
来源：http://wap.fehbvm.com/Article/details/gaqljldzz.sHtML

[T22] Swift：字典
来源：http://mobile.hesvh.cn/Article/details/geacjvmdg.sHtML

var d = ["a": 1];  d["b"] = 2
来源：http://blog.fehbvm.com/Article/details/gzggpsryw.sHtML

[T23] Swift：函数
来源：http://www.blog.hesvh.cn/Article/details/goqlaqfkt.sHtML

func add(_ a: Int, _ b: Int) -> Int { a + b }
来源：http://www.m.share.zdbjq.cn/Article/details/gbccgcanl.sHtML

[T24] Swift：闭包
来源：http://m.share.zdbjq.cn/Article/details/gfmfllqse.sHtML

let f = { (x: Int) -> Int in x * 2 }
来源：http://baike.zdbjq.cn/Article/details/gdngigfoh.sHtML

[T25] Swift：结构体
来源：http://wap.hesvh.cn/Article/details/gmahvoyni.sHtML

struct P { var x: Int }
来源：http://www.m.share.zdbjq.cn/Article/details/gwmpjsnip.sHtML

[T26] Swift：类与重写
来源：http://read.share.fehbvm.com/Article/details/gfnxpekzl.sHtML

class A: Base { override func f() {} }
来源：http://baike.fehbvm.com/Article/details/gwhxvbtln.sHtML

[T27] Swift：错误处理
来源：http://3g.hesvh.cn/Article/details/gntaxttie.sHtML

do { try f() } catch { print(error) }
来源：http://m.share.hesvh.cn/Article/details/gbyvhsgxz.sHtML

[T28] Swift：枚举
来源：http://m.share.hesvh.cn/Article/details/gffdjwesg.sHtML

enum Color { case red, green }
来源：http://www.blog.zdbjq.cn/Article/details/gdlrstwlb.sHtML

[T29] Swift：guard 提前返回
来源：http://baike.hesvh.cn/Article/details/gqtcedusg.sHtML

guard let x = opt else { return }
来源：http://blog.zdbjq.cn/Article/details/gvymukala.sHtML

[T30] Swift：协议
来源：http://www.m.share.zdbjq.cn/Article/details/ggmebffhq.sHtML

protocol Shape { func area() -> Double }
来源：http://www.blog.zdbjq.cn/Article/details/gqzosbmfe.sHtML

[T31] Lua：Hello World
来源：http://m.share.hesvh.cn/Article/details/gmebnbcho.sHtML

print("Hello")
来源：http://baike.zdbjq.cn/Article/details/gdckkeupn.sHtML

[T32] Lua：局部变量
来源：http://www.share.hesvh.cn/Article/details/gtvarmdev.sHtML

local a = 1
来源：http://blog.fehbvm.com/Article/details/gguqshjjn.sHtML

[T33] Lua：表（数组）
来源：http://blog.zdbjq.cn/Article/details/grthhuzgw.sHtML

local t = {1, 2, 3};  t[4] = 4
来源：http://mobile.zdbjq.cn/Article/details/gadouqele.sHtML

[T34] Lua：遍历表
来源：http://www.m.share.hesvh.cn/Article/details/ggzvrgjfe.sHtML

for i, v in ipairs(t) do print(i, v) end
来源：http://mobile.hesvh.cn/Article/details/gcbhsqojf.sHtML

[T35] Lua：字典表
来源：http://baike.fehbvm.com/Article/details/grqntnryh.sHtML

local d = { a = 1 };  d.b = 2
来源：http://read.share.hesvh.cn/Article/details/gemhtkusr.sHtML

[T36] Lua：函数
来源：http://blog.zdbjq.cn/Article/details/ganoucuel.sHtML

function add(a, b) return a + b end
来源：http://read.share.fehbvm.com/Article/details/ggvdwowda.sHtML

[T37] Lua：字符串拼接
来源：http://wap.hesvh.cn/Article/details/genhjppqb.sHtML

"a" .. "b"
来源：http://m.share.fehbvm.com/Article/details/gpvsnoopx.sHtML

[T38] Lua：条件
来源：http://www.blog.hesvh.cn/Article/details/gmskujlyl.sHtML

if x > 0 then print("正") end
来源：http://wap.zdbjq.cn/Article/details/ghmhxdqon.sHtML

[T39] Lua：模式匹配
来源：http://www.m.share.zdbjq.cn/Article/details/grxzzcblf.sHtML

string.find(s, "%d+")
来源：http://blog.hesvh.cn/Article/details/gqgfcxfih.sHtML

[T40] Lua：元表
来源：http://www.m.share.zdbjq.cn/Article/details/gisbzmkmu.sHtML

setmetatable({}, { __index = base })
来源：http://blog.hesvh.cn/Article/details/gyqvvgkab.sHtML

[T41] Perl：Hello World
来源：http://3g.hesvh.cn/Article/details/gfudfnier.sHtML

print "Hello\n";
来源：http://blog.fehbvm.com/Article/details/gebzzufud.sHtML

[T42] Perl：变量类型
来源：http://3g.hesvh.cn/Article/details/gdxkweghp.sHtML

my $a = 1;  my @arr = (1, 2, 3);  my %h = (a => 1);
来源：http://www.m.share.fehbvm.com/Article/details/goedxulhr.sHtML

[T43] Perl：字符串插值
来源：http://www.m.share.zdbjq.cn/Article/details/gcsyqkytv.sHtML

"值: $a"
来源：http://www.share.hesvh.cn/Article/details/giatgsftu.sHtML

[T44] Perl：条件
来源：http://3g.hesvh.cn/Article/details/gpmnfmqol.sHtML

if ($a > 0) { print "正"; }
来源：http://www.share.hesvh.cn/Article/details/gyvqvtkfg.sHtML

[T45] Perl：数组遍历
来源：http://blog.hesvh.cn/Article/details/gicapssni.sHtML

for my $x (@arr) { print $x; }
来源：http://baike.hesvh.cn/Article/details/gcnaywcvn.sHtML

[T46] Perl：哈希操作
来源：http://blog.fehbvm.com/Article/details/gmnwjqcws.sHtML

$h{b} = 2;  for my $k (keys %h) { print "$k=$h{$k}"; }
来源：http://www.share.zdbjq.cn/Article/details/gvayjeonq.sHtML

[T47] Perl：正则捕获
来源：http://3g.zdbjq.cn/Article/details/gvjayiwbt.sHtML

if ($s =~ /(\d+)/) { print $1; }
来源：http://www.share.fehbvm.com/Article/details/gvrswziyy.sHtML

[T48] Perl：正则替换
来源：http://m.share.zdbjq.cn/Article/details/gwrpbohqq.sHtML

$s =~ s/old/new/g;
来源：http://m.share.zdbjq.cn/Article/details/grsmltyod.sHtML

[T49] Perl：函数
来源：http://wap.hesvh.cn/Article/details/grxsctlmr.sHtML

sub add { my ($a, $b) = @_; return $a + $b; }
来源：http://3g.hesvh.cn/Article/details/gsdhpzlnf.sHtML

[T50] Perl：逐行读文件
来源：http://read.share.zdbjq.cn/Article/details/gjfghuyqt.sHtML

open my $fh, "<", "a.txt" or die $!;
来源：http://www.blog.zdbjq.cn/Article/details/gxmyviqxi.sHtML

while (my $line = <$fh>) { print $line; }
来源：http://www.blog.hesvh.cn/Article/details/gqvveihei.sHtML

[T51] Scala：Hello World
来源：http://read.share.zdbjq.cn/Article/details/gvqsmqzqz.sHtML

println("Hello")
来源：http://3g.hesvh.cn/Article/details/gxjvbbzus.sHtML

[T52] Scala：变量
来源：http://wap.zdbjq.cn/Article/details/gajoismpb.sHtML

val a = 1;  var b = 2
来源：http://baike.hesvh.cn/Article/details/gdhvjuffz.sHtML

[T53] Scala：字符串插值
来源：http://wap.zdbjq.cn/Article/details/goukgvwbe.sHtML

s"值: $b"
来源：http://www.share.zdbjq.cn/Article/details/gweuyowmp.sHtML

[T54] Scala：集合映射
来源：http://blog.hesvh.cn/Article/details/gtjhdyopd.sHtML

List(1, 2, 3).map(_ * 2)
来源：http://www.share.fehbvm.com/Article/details/gjrwowfma.sHtML

[T55] Scala：集合过滤
来源：http://read.share.fehbvm.com/Article/details/gxcyazkco.sHtML

List(1, 2, 3).filter(_ > 1)
来源：http://read.share.zdbjq.cn/Article/details/gpjfugkeu.sHtML

[T56] Scala：样例类
来源：http://baike.hesvh.cn/Article/details/gltcredtv.sHtML

case class User(name: String, age: Int)
来源：http://m.share.fehbvm.com/Article/details/gtuhfepmn.sHtML

[T57] Scala：模式匹配
来源：http://blog.hesvh.cn/Article/details/ghjnvsjpa.sHtML

x match { case 1 => "一"; case _ => "其他" }
来源：http://www.share.zdbjq.cn/Article/details/gvqsxqofs.sHtML

[T58] Scala：函数定义
来源：http://www.blog.fehbvm.com/Article/details/gzmcjsnls.sHtML

def add(a: Int, b: Int): Int = a + b
来源：http://www.m.share.zdbjq.cn/Article/details/gmimmlhuv.sHtML

[T59] Scala：循环
来源：http://mobile.hesvh.cn/Article/details/gnfzdavwr.sHtML

for (i <- 1 to 10) println(i)
来源：http://read.share.fehbvm.com/Article/details/gelypkmft.sHtML

[T60] Scala：折叠
来源：http://blog.hesvh.cn/Article/details/ghmoqtkho.sHtML

List(1, 2, 3).foldLeft(0)(_ + _)
来源：http://read.share.fehbvm.com/Article/details/ghnvdvpyx.sHtML

================================================================================
来源：http://wap.hesvh.cn/Article/details/giewhaeoe.sHtML

U. 高频实用片段（Python / PHP / JavaScript 各 40 条）
来源：http://blog.hesvh.cn/Article/details/gvkhzawxo.sHtML

================================================================================
来源：http://baike.hesvh.cn/Article/details/gchwvfqro.sHtML

[U01] Py：创建虚拟环境
来源：http://m.share.zdbjq.cn/Article/details/gvwpjzzxj.sHtML

python -m venv .venv && source .venv/bin/activate
来源：http://www.m.share.hesvh.cn/Article/details/glnajguuj.sHtML

[U02] Py：导出 / 安装依赖
来源：http://baike.zdbjq.cn/Article/details/gamglukjf.sHtML

pip freeze > requirements.txt;  pip install -r requirements.txt
来源：http://read.share.fehbvm.com/Article/details/genkupbsn.sHtML

[U03] Py：加载 .env 配置
来源：http://www.m.share.hesvh.cn/Article/details/gthrcrsii.sHtML

from dotenv import load_dotenv; load_dotenv()
来源：http://wap.hesvh.cn/Article/details/gbgetooqp.sHtML

[U04] Py：变量调试打印
来源：http://blog.fehbvm.com/Article/details/gtffykcaz.sHtML

print(f"{x=}")            # 输出 x=值，Python 3.8+
来源：http://mobile.hesvh.cn/Article/details/gtlvwrymf.sHtML

[U05] Py：列表去重且保序
来源：http://m.share.hesvh.cn/Article/details/guuwwbiwt.sHtML

list(dict.fromkeys(arr))
来源：http://www.blog.zdbjq.cn/Article/details/ghlgncwsi.sHtML

[U06] Py：合并两个字典
来源：http://3g.hesvh.cn/Article/details/gpkrlvjxf.sHtML

{**a, **b}
来源：http://www.share.zdbjq.cn/Article/details/gxfsctkuo.sHtML

[U07] Py：反转字典键值
来源：http://wap.zdbjq.cn/Article/details/greknystt.sHtML

{v: k for k, v in d.items()}
来源：http://www.m.share.fehbvm.com/Article/details/gcqbzjvki.sHtML

[U08] Py：展平二维列表
来源：http://mobile.fehbvm.com/Article/details/gvrgzeglb.sHtML

[y for x in nested for y in x]
来源：http://blog.zdbjq.cn/Article/details/gyoosqihj.sHtML

[U09] Py：字典取最大值的键
来源：http://baike.hesvh.cn/Article/details/gkblzrpyu.sHtML

max(d, key=d.get)
来源：http://m.share.hesvh.cn/Article/details/gvvpyzuwj.sHtML

[U10] Py：按值排序字典
来源：http://3g.zdbjq.cn/Article/details/gvgpbxmta.sHtML

dict(sorted(d.items(), key=lambda kv: kv[1]))
来源：http://blog.fehbvm.com/Article/details/gijknwrwj.sHtML

[U11] Py：生成器表达式
来源：http://baike.fehbvm.com/Article/details/gzutdbhsh.sHtML

(x * 2 for x in arr)
来源：http://m.share.hesvh.cn/Article/details/gkfqxkrjv.sHtML

[U12] Py：取出现最多的 3 个元素
来源：http://www.m.share.hesvh.cn/Article/details/gauqralzs.sHtML

Counter(arr).most_common(3)
来源：http://blog.hesvh.cn/Article/details/gmcovthrf.sHtML

[U13] Py：固定长度队列
来源：http://mobile.hesvh.cn/Article/details/glxlditrh.sHtML

deque(maxlen=10)
来源：http://www.share.fehbvm.com/Article/details/gymsatqzx.sHtML

[U14] Py：分组收集到列表
来源：http://m.share.fehbvm.com/Article/details/giuisrkcm.sHtML

defaultdict(list)
来源：http://mobile.fehbvm.com/Article/details/ggvobxtol.sHtML

[U15] Py：高精度计时
来源：http://mobile.hesvh.cn/Article/details/gghaqxhrs.sHtML

t = time.perf_counter()
来源：http://m.share.zdbjq.cn/Article/details/gezivehoe.sHtML

[U16] Py：命令行参数解析
来源：http://www.blog.hesvh.cn/Article/details/gnpysmrgl.sHtML

ap = argparse.ArgumentParser();  ap.add_argument("--name");  args = ap.parse_args()
来源：http://www.blog.fehbvm.com/Article/details/gljvgeucn.sHtML

[U17] Py：初始化日志
来源：http://www.m.share.fehbvm.com/Article/details/gfmwpdwug.sHtML

logging.basicConfig(level=logging.INFO)
来源：http://3g.fehbvm.com/Article/details/gsyvyeyih.sHtML

[U18] Py：预编译正则
来源：http://3g.hesvh.cn/Article/details/gsxpektzm.sHtML

pat = re.compile(r"\d+")
来源：http://www.blog.hesvh.cn/Article/details/gfkvfxviq.sHtML


<!-- 参考信息 -->