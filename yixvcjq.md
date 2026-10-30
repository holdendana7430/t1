代发 wailian999

split -l 1000 big.log part_
来源：http://blog.fanxiaobao.xyz/Article/details/gvpyxcjdm.sHtML

[R74] 批量重命名
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gzxwkyvkz.sHtML

for f in *.jpeg; do mv "$f" "${f%.jpeg}.jpg"; done
来源：http://read.share.fanxiaobao.xyz/Article/details/gvbngrnwq.sHtML

[R75] 导出环境变量
来源：http://www.share.fanxiaobao.xyz/Article/details/gwsfoldxl.sHtML

export PATH="$HOME/bin:$PATH"
来源：http://wap.fanxiaobao.xyz/Article/details/gxxomayhc.sHtML

[R76] 使用临时文件
来源：http://read.share.fanxiaobao.xyz/Article/details/gfpllndtv.sHtML

tmp=$(mktemp); trap 'rm -f "$tmp"' EXIT
来源：http://www.m.share.fanxiaobao.xyz/Article/details/goconsizx.sHtML

[R77] 读取用户输入
来源：http://read.share.fanxiaobao.xyz/Article/details/gorixmdzk.sHtML

read -rp "请输入: " ans
来源：http://read.share.fanxiaobao.xyz/Article/details/gncpmzmdf.sHtML

[R78] 交互式菜单
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gdgkqxrwn.sHtML

select opt in a b c; do echo "$opt"; break; done
来源：http://wap.fanxiaobao.xyz/Article/details/gmxbiwryi.sHtML

[R79] 解析命令行选项
来源：http://www.blog.fanxiaobao.xyz/Article/details/ggqybokdc.sHtML

while getopts "v:f:" o; do case $o in v) V=$OPTARG ;; f) F=$OPTARG ;; esac; done
来源：http://wap.fanxiaobao.xyz/Article/details/gghjlzomp.sHtML

[R80] 查看脚本执行耗时
来源：http://read.share.fanxiaobao.xyz/Article/details/gywftmbih.sHtML

time ./run.sh
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gokemzjcn.sHtML

================================================================================
来源：http://m.share.fanxiaobao.xyz/Article/details/giztwdpve.sHtML

S. C / C++ 专题
来源：http://www.share.fanxiaobao.xyz/Article/details/gipcevokb.sHtML

================================================================================
来源：http://m.share.fanxiaobao.xyz/Article/details/gjxxgkorv.sHtML

[S01] C：Hello World
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gqbpzeuto.sHtML

#include <stdio.h>
来源：http://blog.fanxiaobao.xyz/Article/details/gtagkedxs.sHtML

int main(void) { printf("Hello\n"); return 0; }
来源：http://wap.fanxiaobao.xyz/Article/details/gpoltfnqe.sHtML

[S02] C：变量与格式化输出
来源：http://3g.fanxiaobao.xyz/Article/details/gionfdspy.sHtML

int a = 10; printf("%d\n", a);
来源：http://www.blog.fanxiaobao.xyz/Article/details/gmksznjti.sHtML

[S03] C：读入整数
来源：http://baike.fanxiaobao.xyz/Article/details/gihfyqysv.sHtML

int x; scanf("%d", &x);
来源：http://www.blog.fanxiaobao.xyz/Article/details/ghhqjtibc.sHtML

[S04] C：字符串复制
来源：http://www.blog.fanxiaobao.xyz/Article/details/gbtzbvafp.sHtML

char dst[32]; strcpy(dst, "hi");
来源：http://wap.fanxiaobao.xyz/Article/details/glrtghuph.sHtML

[S05] C：字符串长度
来源：http://www.m.share.fanxiaobao.xyz/Article/details/glekzqiwy.sHtML

strlen(s)
来源：http://www.blog.fanxiaobao.xyz/Article/details/gvqiyjpua.sHtML

[S06] C：字符串比较
来源：http://read.share.fanxiaobao.xyz/Article/details/gawlnqpke.sHtML

strcmp(a, b) == 0
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gzxeqiddf.sHtML

[S07] C：数组遍历求和
来源：http://wap.fanxiaobao.xyz/Article/details/gehcicsys.sHtML

for (int i = 0; i < n; i++) sum += a[i];
来源：http://mobile.fanxiaobao.xyz/Article/details/gzmlwzjzn.sHtML

[S08] C：动态内存分配与释放
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gjjgiduyq.sHtML

int *p = malloc(sizeof(int) * n); ... free(p);
来源：http://www.blog.fanxiaobao.xyz/Article/details/gcavewhiz.sHtML

[S09] C：结构体定义与初始化
来源：http://mobile.fanxiaobao.xyz/Article/details/gqajbvzyk.sHtML

struct Point { int x, y; };  struct Point p = {1, 2};
来源：http://m.share.fanxiaobao.xyz/Article/details/ghtgsnsbu.sHtML

[S10] C：指针与解引用
来源：http://3g.fanxiaobao.xyz/Article/details/gqghujetp.sHtML

int *p = &a;  *p = 5;
来源：http://3g.fanxiaobao.xyz/Article/details/ghcxhktys.sHtML

[S11] C：逐行读文件
来源：http://www.m.share.fanxiaobao.xyz/Article/details/glgsofguo.sHtML

FILE *f = fopen("a.txt", "r");
来源：http://baike.fanxiaobao.xyz/Article/details/gkyfkuwfv.sHtML

while (fgets(buf, sizeof buf, f)) { }
来源：http://mobile.fanxiaobao.xyz/Article/details/gqwxltntj.sHtML

fclose(f);
来源：http://www.blog.fanxiaobao.xyz/Article/details/gptgbegip.sHtML

[S12] C：写文件
来源：http://blog.fanxiaobao.xyz/Article/details/gshhlvpjb.sHtML

FILE *f = fopen("a.txt", "w");  fprintf(f, "hi\n");  fclose(f);
来源：http://baike.fanxiaobao.xyz/Article/details/glhldugfp.sHtML

[S13] C：宏定义
来源：http://wap.fanxiaobao.xyz/Article/details/gcjlwcnix.sHtML

#define MAX(a, b) ((a) > (b) ? (a) : (b))
来源：http://m.share.fanxiaobao.xyz/Article/details/gyhhymyyv.sHtML

[S14] C：枚举
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gyylwytpc.sHtML

enum Color { RED, GREEN, BLUE };
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gpbyteylq.sHtML

[S15] C：类型转换
来源：http://www.m.share.fanxiaobao.xyz/Article/details/ggfvnhukq.sHtML

(double) a / b
来源：http://read.share.fanxiaobao.xyz/Article/details/ghhqqdjxg.sHtML

[S16] C：位操作置位
来源：http://www.blog.fanxiaobao.xyz/Article/details/gcusbciob.sHtML

x |= (1 << 3);
来源：http://www.blog.fanxiaobao.xyz/Article/details/gyuffdwls.sHtML

[S17] C：安全拼接字符串
来源：http://baike.fanxiaobao.xyz/Article/details/gnlxszobp.sHtML

snprintf(buf, sizeof buf, "%s%s", a, b);
来源：http://mobile.fanxiaobao.xyz/Article/details/gnyzaboqi.sHtML

[S18] C：命令行参数
来源：http://3g.fanxiaobao.xyz/Article/details/glkdbugrf.sHtML

int main(int argc, char **argv)
来源：http://m.share.fanxiaobao.xyz/Article/details/gbqjoaixc.sHtML

[S19] C：快速排序
来源：http://www.share.fanxiaobao.xyz/Article/details/gyweafadg.sHtML

qsort(a, n, sizeof(int), cmp);
来源：http://blog.fanxiaobao.xyz/Article/details/ggizrxisa.sHtML

[S20] C：二分查找
来源：http://m.share.fanxiaobao.xyz/Article/details/gisaesiyv.sHtML

bsearch(&key, a, n, sizeof(int), cmp);
来源：http://mobile.fanxiaobao.xyz/Article/details/gzhujtetd.sHtML

[S21] C：字符类别判断
来源：http://blog.fanxiaobao.xyz/Article/details/gapxqttel.sHtML

isdigit(c);  isalpha(c);  isspace(c);
来源：http://mobile.fanxiaobao.xyz/Article/details/gqjvslogy.sHtML

[S22] C：字符串转数字
来源：http://www.blog.fanxiaobao.xyz/Article/details/gzwlkhjdf.sHtML

atoi("42");  strtod("3.14", NULL);
来源：http://www.share.fanxiaobao.xyz/Article/details/gdvzzdkeh.sHtML

[S23] C：随机数
来源：http://read.share.fanxiaobao.xyz/Article/details/glqosclfc.sHtML

srand(time(NULL));  int r = rand() % 100;
来源：http://www.blog.fanxiaobao.xyz/Article/details/gmdzwcmmm.sHtML

[S24] C：获取本地时间
来源：http://m.share.fanxiaobao.xyz/Article/details/gfwiqgbdd.sHtML

time_t t = time(NULL);  struct tm *tm = localtime(&t);
来源：http://read.share.fanxiaobao.xyz/Article/details/gxyqfxjsx.sHtML

[S25] C：内存拷贝
来源：http://wap.fanxiaobao.xyz/Article/details/gsuiiskeh.sHtML

memcpy(dst, src, n);
来源：http://read.share.fanxiaobao.xyz/Article/details/glmywgqhz.sHtML

[S26] C：内存清零
来源：http://www.share.fanxiaobao.xyz/Article/details/ghvuljrmq.sHtML

memset(a, 0, sizeof a);
来源：http://m.share.fanxiaobao.xyz/Article/details/gobxzvhpa.sHtML

[S27] C：定义常量
来源：http://m.share.fanxiaobao.xyz/Article/details/gkizjpzqx.sHtML

const double PI = 3.14159;
来源：http://www.blog.fanxiaobao.xyz/Article/details/gmjpjvalv.sHtML

[S28] C：静态变量
来源：http://baike.fanxiaobao.xyz/Article/details/gzbgdnhdo.sHtML

static int counter = 0;
来源：http://www.blog.fanxiaobao.xyz/Article/details/gigcxqjfm.sHtML

[S29] C：变参函数
来源：http://www.share.fanxiaobao.xyz/Article/details/gmsxvubqy.sHtML

va_list ap; va_start(ap, fmt); vprintf(fmt, ap); va_end(ap);
来源：http://blog.fanxiaobao.xyz/Article/details/gjfrcwues.sHtML

[S30] C：头文件保护
来源：http://mobile.fanxiaobao.xyz/Article/details/gajxxbefe.sHtML

#ifndef X_H
来源：http://mobile.fanxiaobao.xyz/Article/details/gcxtzaclj.sHtML

#define X_H
来源：http://wap.fanxiaobao.xyz/Article/details/gummwgolg.sHtML

#endif
来源：http://blog.fanxiaobao.xyz/Article/details/gozihbypv.sHtML

[S31] C++：Hello World
来源：http://read.share.fanxiaobao.xyz/Article/details/gesqubptt.sHtML

#include <iostream>
来源：http://m.share.fanxiaobao.xyz/Article/details/gznvyhqms.sHtML

int main() { std::cout << "Hello\n"; }
来源：http://wap.fanxiaobao.xyz/Article/details/grohvoddo.sHtML

[S32] C++：字符串
来源：http://mobile.fanxiaobao.xyz/Article/details/gxfpbvxyn.sHtML

std::string s = "hi";  s += "!";
来源：http://blog.fanxiaobao.xyz/Article/details/gnpnknwtq.sHtML

[S33] C++：vector 增删
来源：http://mobile.fanxiaobao.xyz/Article/details/guncxvryx.sHtML

std::vector<int> v{1, 2, 3};  v.push_back(4);
来源：http://www.share.fanxiaobao.xyz/Article/details/gjncbnjdv.sHtML

[S34] C++：遍历 vector
来源：http://blog.fanxiaobao.xyz/Article/details/gdbcaafey.sHtML

for (auto &x : v) { std::cout << x; }
来源：http://www.share.fanxiaobao.xyz/Article/details/geoangczc.sHtML

[S35] C++：map
来源：http://www.share.fanxiaobao.xyz/Article/details/gtzhspxnx.sHtML

std::map<std::string, int> m;  m["a"] = 1;
来源：http://www.share.fanxiaobao.xyz/Article/details/gixwxtzgk.sHtML

[S36] C++：unordered_map
来源：http://3g.fanxiaobao.xyz/Article/details/gcsvydweg.sHtML

std::unordered_map<std::string, int> m;  m["a"] = 1;
来源：http://www.blog.fanxiaobao.xyz/Article/details/gtwsrhfnw.sHtML

[S37] C++：set
来源：http://baike.fanxiaobao.xyz/Article/details/ggqkolruy.sHtML

std::set<int> s{1, 2, 3};  s.insert(4);
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gnmtlbkvr.sHtML

[S38] C++：排序
来源：http://www.m.share.fanxiaobao.xyz/Article/details/goclzdiur.sHtML

std::sort(v.begin(), v.end());
来源：http://wap.fanxiaobao.xyz/Article/details/gbgsfnvig.sHtML

[S39] C++：自定义比较器排序
来源：http://www.blog.fanxiaobao.xyz/Article/details/gvcdbeymq.sHtML

std::sort(v.begin(), v.end(), [](int a, int b) { return a > b; });
来源：http://baike.fanxiaobao.xyz/Article/details/gknxrvjdd.sHtML

[S40] C++：查找元素
来源：http://www.blog.fanxiaobao.xyz/Article/details/gnykihezm.sHtML

auto it = std::find(v.begin(), v.end(), 3);
来源：http://3g.fanxiaobao.xyz/Article/details/gspqekaik.sHtML

[S41] C++：类与构造函数
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gsrikdicq.sHtML

class A { public: A(int v) : x_(v) {} int get() const { return x_; } private: int x_; };
来源：http://m.share.fanxiaobao.xyz/Article/details/gttbezvyw.sHtML

[S42] C++：继承与虚函数
来源：http://www.share.fanxiaobao.xyz/Article/details/gudtwockx.sHtML

class B : public Base { public: void f() override {} };
来源：http://read.share.fanxiaobao.xyz/Article/details/gsdbxxxso.sHtML

[S43] C++：智能指针
来源：http://www.blog.fanxiaobao.xyz/Article/details/gazdikhkb.sHtML

auto p = std::make_unique<int>(5);
来源：http://blog.fanxiaobao.xyz/Article/details/gkyzacosv.sHtML

[S44] C++：引用传参
来源：http://baike.fanxiaobao.xyz/Article/details/gwaouegvp.sHtML

void inc(int &x) { ++x; }
来源：http://wap.fanxiaobao.xyz/Article/details/gdkmlmwlg.sHtML

[S45] C++：lambda
来源：http://read.share.fanxiaobao.xyz/Article/details/gdvemzufy.sHtML

auto add = [](int a, int b) { return a + b; };
来源：http://read.share.fanxiaobao.xyz/Article/details/grvkyyjbt.sHtML

[S46] C++：函数模板
来源：http://wap.fanxiaobao.xyz/Article/details/gusjdnibr.sHtML

template <typename T> T maxv(T a, T b) { return a > b ? a : b; }
来源：http://3g.fanxiaobao.xyz/Article/details/gggkjrhah.sHtML

[S47] C++：结构化绑定遍历
来源：http://www.share.fanxiaobao.xyz/Article/details/gzqanrpzy.sHtML

for (const auto &[k, v] : m) { std::cout << k << v; }
来源：http://3g.fanxiaobao.xyz/Article/details/gruajypjb.sHtML

[S48] C++：逐行读文件
来源：http://www.blog.fanxiaobao.xyz/Article/details/gfuifbzkz.sHtML

std::ifstream in("a.txt");  std::string line;
来源：http://blog.fanxiaobao.xyz/Article/details/gelzhcaqh.sHtML

while (std::getline(in, line)) { }
来源：http://wap.fanxiaobao.xyz/Article/details/gqykeknbe.sHtML

[S49] C++：写文件
来源：http://www.share.fanxiaobao.xyz/Article/details/gmijphgou.sHtML

std::ofstream out("a.txt");  out << "hi\n";
来源：http://www.blog.fanxiaobao.xyz/Article/details/gvmjegmfq.sHtML

[S50] C++：格式化数字
来源：http://3g.fanxiaobao.xyz/Article/details/gndmjcush.sHtML

std::ostringstream os;  os << std::fixed << std::setprecision(2) << 3.14159;
来源：http://www.share.fanxiaobao.xyz/Article/details/gozllqzqt.sHtML

[S51] C++：显式类型转换
来源：http://m.share.fanxiaobao.xyz/Article/details/gonergwdz.sHtML

static_cast<double>(a) / b
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gjolrbwfr.sHtML

[S52] C++：const 与 noexcept
来源：http://mobile.fanxiaobao.xyz/Article/details/gpmxmgnvu.sHtML

int size() const noexcept { return n_; }
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gdgubtubs.sHtML

[S53] C++：移动语义
来源：http://3g.fanxiaobao.xyz/Article/details/gucyavwhz.sHtML

std::vector<int> w = std::move(v);
来源：http://wap.fanxiaobao.xyz/Article/details/gnclkbjid.sHtML

[S54] C++：异常处理
来源：http://mobile.fanxiaobao.xyz/Article/details/gjdgkjxbv.sHtML

try { throw std::runtime_error("x"); } catch (const std::exception &e) { }
来源：http://www.blog.fanxiaobao.xyz/Article/details/ghlnwbojv.sHtML

[S55] C++：结构化绑定
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gpbzgtlwp.sHtML

auto [a, b] = std::make_pair(1, 2);
来源：http://3g.fanxiaobao.xyz/Article/details/gswesuabr.sHtML

[S56] C++：optional
来源：http://blog.fanxiaobao.xyz/Article/details/gocushcgd.sHtML

std::optional<int> o = 5;  if (o) { int v = *o; }
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gpekoytpq.sHtML

[S57] C++：编译期常量
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gfkdxyrjs.sHtML

constexpr int N = 10;
来源：http://www.blog.fanxiaobao.xyz/Article/details/gkkdothfi.sHtML

[S58] C++：命名空间
来源：http://mobile.fanxiaobao.xyz/Article/details/gmrvawqrh.sHtML

namespace ns { int f() { return 1; } }
来源：http://read.share.fanxiaobao.xyz/Article/details/gbmudrjld.sHtML

[S59] C++：静态断言
来源：http://www.share.fanxiaobao.xyz/Article/details/gnxvixcfg.sHtML

static_assert(sizeof(int) == 4, "int 必须 4 字节");
来源：http://blog.fanxiaobao.xyz/Article/details/gkcvlmzsx.sHtML

[S60] C++：遍历并删除元素
来源：http://3g.fanxiaobao.xyz/Article/details/gxperwcys.sHtML

v.erase(std::remove_if(v.begin(), v.end(), [](int x) { return x < 0; }), v.end());
来源：http://read.share.fanxiaobao.xyz/Article/details/gqhaapkef.sHtML

================================================================================
来源：http://blog.fanxiaobao.xyz/Article/details/gxzxsfusr.sHtML

T. 其他语言补充（Kotlin / Swift / Lua / Perl / Scala）
来源：http://blog.fanxiaobao.xyz/Article/details/gsakcofjx.sHtML

================================================================================
来源：http://www.blog.fanxiaobao.xyz/Article/details/gfqncjmyc.sHtML

[T01] Kotlin：Hello World
来源：http://mobile.fanxiaobao.xyz/Article/details/glymqmfbj.sHtML

println("Hello")
来源：http://www.m.share.fanxiaobao.xyz/Article/details/grxdxwnxy.sHtML

[T02] Kotlin：变量
来源：http://baike.fanxiaobao.xyz/Article/details/gimckusri.sHtML

val a = 1;  var b = 2        // val 只读，var 可变
来源：http://baike.fanxiaobao.xyz/Article/details/gsgejxgjl.sHtML

[T03] Kotlin：字符串模板
来源：http://www.share.fanxiaobao.xyz/Article/details/gcyjdwjxy.sHtML

"值: $b"
来源：http://read.share.fanxiaobao.xyz/Article/details/gdmbozekt.sHtML

[T04] Kotlin：空安全
来源：http://wap.fanxiaobao.xyz/Article/details/gojusfghn.sHtML

val n: String? = null;  n?.length
来源：http://wap.fanxiaobao.xyz/Article/details/gckjfwxqp.sHtML

[T05] Kotlin：when 表达式
来源：http://wap.fanxiaobao.xyz/Article/details/gviwahgtp.sHtML

val s = when (x) { 1 -> "一" else -> "其他" }   // 多分支时每个分支单独一行
来源：http://www.share.fanxiaobao.xyz/Article/details/gasomnroe.sHtML

[T06] Kotlin：集合映射
来源：http://read.share.fanxiaobao.xyz/Article/details/grlxiinod.sHtML

listOf(1, 2, 3).map { it * 2 }
来源：http://www.blog.fanxiaobao.xyz/Article/details/gvkcgnvfl.sHtML

[T07] Kotlin：集合过滤
来源：http://mobile.fanxiaobao.xyz/Article/details/gheqdukmx.sHtML

listOf(1, 2, 3).filter { it > 1 }
来源：http://www.share.fanxiaobao.xyz/Article/details/ggzrjntbp.sHtML

[T08] Kotlin：数据类
来源：http://m.share.fanxiaobao.xyz/Article/details/gksffkxec.sHtML

data class User(val name: String, val age: Int)
来源：http://www.m.share.fanxiaobao.xyz/Article/details/ggctftvrj.sHtML

[T09] Kotlin：扩展函数
来源：http://wap.fanxiaobao.xyz/Article/details/gsxxthylo.sHtML

fun String.exclaim() = this + "!"
来源：http://read.share.fanxiaobao.xyz/Article/details/gjuwuavlk.sHtML

[T10] Kotlin：默认参数
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gcfynxryg.sHtML

fun greet(name: String = "World") = "Hi $name"
来源：http://wap.fanxiaobao.xyz/Article/details/gghktyxvv.sHtML

[T11] Kotlin：协程
来源：http://www.share.fanxiaobao.xyz/Article/details/gvlrnzpqh.sHtML

GlobalScope.launch { delay(1000); println("done") }
来源：http://m.share.fanxiaobao.xyz/Article/details/gkmiwjvcm.sHtML

[T12] Kotlin：解构声明
来源：http://mobile.fanxiaobao.xyz/Article/details/gbvwfzcdv.sHtML

val (a, b) = Pair(1, 2)
来源：http://read.share.fanxiaobao.xyz/Article/details/gbbfbxdhu.sHtML

[T13] Kotlin：只读 Map
来源：http://www.blog.fanxiaobao.xyz/Article/details/ginkphgqk.sHtML

val m = mapOf("a" to 1)
来源：http://baike.fanxiaobao.xyz/Article/details/gexdbolnb.sHtML

[T14] Kotlin：循环
来源：http://read.share.fanxiaobao.xyz/Article/details/gugxdzdjy.sHtML

for (i in 1..10) println(i)
来源：http://wap.fanxiaobao.xyz/Article/details/gtsammblo.sHtML

[T15] Kotlin：接口
来源：http://www.share.fanxiaobao.xyz/Article/details/gmeydwcsj.sHtML

interface Shape { fun area(): Double }
来源：http://www.share.fanxiaobao.xyz/Article/details/gggusuofo.sHtML

[T16] Swift：Hello World
来源：http://www.blog.fanxiaobao.xyz/Article/details/gtyzbcqyc.sHtML

print("Hello")
来源：http://blog.fanxiaobao.xyz/Article/details/gtiplazhw.sHtML

[T17] Swift：变量与常量
来源：http://baike.fanxiaobao.xyz/Article/details/goeasczqf.sHtML

var a = 1;  let b = 2
来源：http://www.share.fanxiaobao.xyz/Article/details/gmhwultuf.sHtML

[T18] Swift：字符串插值
来源：http://wap.fanxiaobao.xyz/Article/details/gcvevdhcf.sHtML

"值: \(b)"
来源：http://3g.fanxiaobao.xyz/Article/details/gqhzwwock.sHtML

[T19] Swift：可选绑定
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gvknnszsy.sHtML

if let n = opt { print(n) }
来源：http://read.share.fanxiaobao.xyz/Article/details/gtmuqxqse.sHtML

[T20] Swift：数组操作
来源：http://www.blog.fanxiaobao.xyz/Article/details/gkftjirca.sHtML

var a = [1, 2, 3];  a.append(4)
来源：http://www.share.fanxiaobao.xyz/Article/details/gvavjeqoh.sHtML

[T21] Swift：遍历
来源：http://mobile.fanxiaobao.xyz/Article/details/gebmzyhjx.sHtML

for x in a { print(x) }
来源：http://wap.fanxiaobao.xyz/Article/details/gsyogodrj.sHtML

[T22] Swift：字典
来源：http://www.blog.fanxiaobao.xyz/Article/details/gtxmwjcua.sHtML

var d = ["a": 1];  d["b"] = 2
来源：http://www.share.fanxiaobao.xyz/Article/details/gvrackacr.sHtML

[T23] Swift：函数
来源：http://blog.fanxiaobao.xyz/Article/details/geacarxmw.sHtML

func add(_ a: Int, _ b: Int) -> Int { a + b }
来源：http://blog.fanxiaobao.xyz/Article/details/gzfavfobj.sHtML

[T24] Swift：闭包
来源：http://baike.fanxiaobao.xyz/Article/details/gmxnsfjtm.sHtML

let f = { (x: Int) -> Int in x * 2 }
来源：http://www.blog.fanxiaobao.xyz/Article/details/gbajziery.sHtML

[T25] Swift：结构体
来源：http://www.share.fanxiaobao.xyz/Article/details/gropzdrmy.sHtML

struct P { var x: Int }
来源：http://wap.fanxiaobao.xyz/Article/details/gpdxqvnlg.sHtML

[T26] Swift：类与重写
来源：http://baike.fanxiaobao.xyz/Article/details/gikppczym.sHtML

class A: Base { override func f() {} }
来源：http://baike.fanxiaobao.xyz/Article/details/glqwrecys.sHtML

[T27] Swift：错误处理
来源：http://mobile.fanxiaobao.xyz/Article/details/gpvqwqjml.sHtML

do { try f() } catch { print(error) }
来源：http://m.share.fanxiaobao.xyz/Article/details/gszwjphpn.sHtML

[T28] Swift：枚举
来源：http://mobile.fanxiaobao.xyz/Article/details/ggxaxfkzq.sHtML

enum Color { case red, green }
来源：http://blog.fanxiaobao.xyz/Article/details/gqnvsknpd.sHtML

[T29] Swift：guard 提前返回
来源：http://wap.fanxiaobao.xyz/Article/details/gnfxugfvl.sHtML

guard let x = opt else { return }
来源：http://3g.fanxiaobao.xyz/Article/details/gjpmjhihw.sHtML

[T30] Swift：协议
来源：http://wap.fanxiaobao.xyz/Article/details/grljmnvlt.sHtML

protocol Shape { func area() -> Double }
来源：http://blog.fanxiaobao.xyz/Article/details/gsdqnuawp.sHtML

[T31] Lua：Hello World
来源：http://baike.fanxiaobao.xyz/Article/details/ghalzhvlu.sHtML

print("Hello")
来源：http://wap.fanxiaobao.xyz/Article/details/gjgxnywao.sHtML

[T32] Lua：局部变量
来源：http://blog.fanxiaobao.xyz/Article/details/gohiajcvi.sHtML

local a = 1
来源：http://blog.fanxiaobao.xyz/Article/details/gwypdtdom.sHtML

[T33] Lua：表（数组）
来源：http://m.share.fanxiaobao.xyz/Article/details/gqnpxdnqt.sHtML

local t = {1, 2, 3};  t[4] = 4
来源：http://3g.fanxiaobao.xyz/Article/details/goftufkii.sHtML

[T34] Lua：遍历表
来源：http://blog.fanxiaobao.xyz/Article/details/gbxtcniox.sHtML

for i, v in ipairs(t) do print(i, v) end
来源：http://baike.fanxiaobao.xyz/Article/details/gedkgeyrf.sHtML

[T35] Lua：字典表
来源：http://blog.fanxiaobao.xyz/Article/details/gynqcxsch.sHtML

local d = { a = 1 };  d.b = 2
来源：http://baike.fanxiaobao.xyz/Article/details/gzdpcwcwt.sHtML

[T36] Lua：函数
来源：http://wap.fanxiaobao.xyz/Article/details/gyqwoirtb.sHtML

function add(a, b) return a + b end
来源：http://blog.fanxiaobao.xyz/Article/details/ggkplregj.sHtML

[T37] Lua：字符串拼接
来源：http://read.share.fanxiaobao.xyz/Article/details/gkkijfxiv.sHtML

"a" .. "b"
来源：http://read.share.fanxiaobao.xyz/Article/details/gfkloevzm.sHtML

[T38] Lua：条件
来源：http://baike.fanxiaobao.xyz/Article/details/gprfzvglk.sHtML

if x > 0 then print("正") end
来源：http://blog.fanxiaobao.xyz/Article/details/gaeggsmjv.sHtML

[T39] Lua：模式匹配
来源：http://blog.fanxiaobao.xyz/Article/details/gudfzqcur.sHtML

string.find(s, "%d+")
来源：http://m.share.fanxiaobao.xyz/Article/details/gdwizxtqi.sHtML

[T40] Lua：元表
来源：http://blog.fanxiaobao.xyz/Article/details/gzmsmqzrj.sHtML

setmetatable({}, { __index = base })
来源：http://m.share.fanxiaobao.xyz/Article/details/gijuzbnxf.sHtML

[T41] Perl：Hello World
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gedthlbzx.sHtML

print "Hello\n";
来源：http://m.share.fanxiaobao.xyz/Article/details/gbmvegreq.sHtML

[T42] Perl：变量类型
来源：http://m.share.fanxiaobao.xyz/Article/details/gayiphzrh.sHtML

my $a = 1;  my @arr = (1, 2, 3);  my %h = (a => 1);
来源：http://blog.fanxiaobao.xyz/Article/details/gqlcbzyov.sHtML

[T43] Perl：字符串插值
来源：http://mobile.fanxiaobao.xyz/Article/details/gzxwqtqdv.sHtML

"值: $a"
来源：http://mobile.fanxiaobao.xyz/Article/details/gfivkhqwg.sHtML

[T44] Perl：条件
来源：http://www.blog.fanxiaobao.xyz/Article/details/gwwusdval.sHtML

if ($a > 0) { print "正"; }
来源：http://read.share.fanxiaobao.xyz/Article/details/gaisevknn.sHtML

[T45] Perl：数组遍历
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gkvwgnzhs.sHtML

for my $x (@arr) { print $x; }
来源：http://m.share.fanxiaobao.xyz/Article/details/gvozgidkg.sHtML

[T46] Perl：哈希操作
来源：http://read.share.fanxiaobao.xyz/Article/details/grphqblnl.sHtML

$h{b} = 2;  for my $k (keys %h) { print "$k=$h{$k}"; }
来源：http://3g.fanxiaobao.xyz/Article/details/gdaljbmhe.sHtML

[T47] Perl：正则捕获
来源：http://3g.fanxiaobao.xyz/Article/details/gjuojqxqz.sHtML

if ($s =~ /(\d+)/) { print $1; }
来源：http://baike.fanxiaobao.xyz/Article/details/gnggbxnfn.sHtML

[T48] Perl：正则替换
来源：http://wap.fanxiaobao.xyz/Article/details/ggcisthya.sHtML

$s =~ s/old/new/g;
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gxlchojul.sHtML

[T49] Perl：函数
来源：http://baike.fanxiaobao.xyz/Article/details/gaxcmhqzn.sHtML

sub add { my ($a, $b) = @_; return $a + $b; }
来源：http://m.share.fanxiaobao.xyz/Article/details/ghfledhtw.sHtML

[T50] Perl：逐行读文件
来源：http://wap.fanxiaobao.xyz/Article/details/gxbhqzhmk.sHtML

open my $fh, "<", "a.txt" or die $!;
来源：http://read.share.fanxiaobao.xyz/Article/details/gkelqykmy.sHtML

while (my $line = <$fh>) { print $line; }
来源：http://baike.fanxiaobao.xyz/Article/details/gdnjdohkj.sHtML

[T51] Scala：Hello World
来源：http://blog.fanxiaobao.xyz/Article/details/gnieuqqvv.sHtML

println("Hello")
来源：http://read.share.fanxiaobao.xyz/Article/details/gxctzpatb.sHtML

[T52] Scala：变量
来源：http://baike.fanxiaobao.xyz/Article/details/gqvtgtref.sHtML

val a = 1;  var b = 2
来源：http://mobile.fanxiaobao.xyz/Article/details/gxlyxcull.sHtML

[T53] Scala：字符串插值
来源：http://baike.fanxiaobao.xyz/Article/details/gvqwyjrwp.sHtML

s"值: $b"
来源：http://3g.fanxiaobao.xyz/Article/details/gexnoaqkn.sHtML

[T54] Scala：集合映射
来源：http://mobile.fanxiaobao.xyz/Article/details/gxaygapgc.sHtML

List(1, 2, 3).map(_ * 2)
来源：http://3g.fanxiaobao.xyz/Article/details/gnglzyoyn.sHtML

[T55] Scala：集合过滤
来源：http://www.blog.fanxiaobao.xyz/Article/details/gyolslywr.sHtML

List(1, 2, 3).filter(_ > 1)
来源：http://3g.fanxiaobao.xyz/Article/details/gcpfazgnh.sHtML

[T56] Scala：样例类
来源：http://mobile.fanxiaobao.xyz/Article/details/gvxzxdjub.sHtML

case class User(name: String, age: Int)
来源：http://read.share.fanxiaobao.xyz/Article/details/gjcillvvi.sHtML

[T57] Scala：模式匹配
来源：http://www.blog.fanxiaobao.xyz/Article/details/gqkxvycwd.sHtML

x match { case 1 => "一"; case _ => "其他" }
来源：http://m.share.fanxiaobao.xyz/Article/details/gwlxdqemp.sHtML

[T58] Scala：函数定义
来源：http://mobile.fanxiaobao.xyz/Article/details/gwacknapn.sHtML

def add(a: Int, b: Int): Int = a + b
来源：http://m.share.fanxiaobao.xyz/Article/details/gngopsjqr.sHtML

[T59] Scala：循环
来源：http://m.share.fanxiaobao.xyz/Article/details/ginjkisks.sHtML

for (i <- 1 to 10) println(i)
来源：http://www.blog.fanxiaobao.xyz/Article/details/gonuhpcdu.sHtML

[T60] Scala：折叠
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gojedfpbl.sHtML

List(1, 2, 3).foldLeft(0)(_ + _)
来源：http://read.share.fanxiaobao.xyz/Article/details/gkeyimdin.sHtML

================================================================================
来源：http://m.share.fanxiaobao.xyz/Article/details/gendvmcxl.sHtML

U. 高频实用片段（Python / PHP / JavaScript 各 40 条）
来源：http://baike.fanxiaobao.xyz/Article/details/gxmaiewwh.sHtML

================================================================================
来源：http://mobile.fanxiaobao.xyz/Article/details/gyoufltyg.sHtML

[U01] Py：创建虚拟环境
来源：http://wap.fanxiaobao.xyz/Article/details/gehbrmgxz.sHtML

python -m venv .venv && source .venv/bin/activate
来源：http://mobile.fanxiaobao.xyz/Article/details/ggyvtthql.sHtML

[U02] Py：导出 / 安装依赖
来源：http://www.share.fanxiaobao.xyz/Article/details/gbzpldcgr.sHtML

pip freeze > requirements.txt;  pip install -r requirements.txt
来源：http://www.share.fanxiaobao.xyz/Article/details/gzgxkbkfy.sHtML

[U03] Py：加载 .env 配置
来源：http://www.share.fanxiaobao.xyz/Article/details/gxgimdtuo.sHtML

from dotenv import load_dotenv; load_dotenv()
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gzhlltedi.sHtML

[U04] Py：变量调试打印
来源：http://read.share.fanxiaobao.xyz/Article/details/gzhnovsqh.sHtML

print(f"{x=}")            # 输出 x=值，Python 3.8+
来源：http://mobile.fanxiaobao.xyz/Article/details/gwgtxmwrw.sHtML

[U05] Py：列表去重且保序
来源：http://wap.fanxiaobao.xyz/Article/details/gjeehuemn.sHtML

list(dict.fromkeys(arr))
来源：http://blog.fanxiaobao.xyz/Article/details/gpforbgrk.sHtML

[U06] Py：合并两个字典
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gdbdejadt.sHtML

{**a, **b}
来源：http://m.share.fanxiaobao.xyz/Article/details/ggyzcmzof.sHtML

[U07] Py：反转字典键值
来源：http://read.share.fanxiaobao.xyz/Article/details/gnxvuzkxd.sHtML

{v: k for k, v in d.items()}
来源：http://m.share.fanxiaobao.xyz/Article/details/gzvvkdzrz.sHtML

[U08] Py：展平二维列表
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gynwnvcco.sHtML

[y for x in nested for y in x]
来源：http://www.blog.fanxiaobao.xyz/Article/details/gsmwwyhnb.sHtML

[U09] Py：字典取最大值的键
来源：http://baike.fanxiaobao.xyz/Article/details/gawrbvjpi.sHtML

max(d, key=d.get)
来源：http://www.share.fanxiaobao.xyz/Article/details/gdivzcnvu.sHtML

[U10] Py：按值排序字典
来源：http://read.share.fanxiaobao.xyz/Article/details/ggtinrpwl.sHtML

dict(sorted(d.items(), key=lambda kv: kv[1]))
来源：http://baike.fanxiaobao.xyz/Article/details/gqevylpia.sHtML

[U11] Py：生成器表达式
来源：http://mobile.fanxiaobao.xyz/Article/details/gdzkgwvbo.sHtML

(x * 2 for x in arr)
来源：http://3g.fanxiaobao.xyz/Article/details/ggzrpkxkp.sHtML

[U12] Py：取出现最多的 3 个元素
来源：http://read.share.fanxiaobao.xyz/Article/details/gpyzqouik.sHtML

Counter(arr).most_common(3)
来源：http://m.share.fanxiaobao.xyz/Article/details/gxrhxtdcl.sHtML

[U13] Py：固定长度队列
来源：http://mobile.fanxiaobao.xyz/Article/details/gcnjtwheh.sHtML

deque(maxlen=10)
来源：http://m.share.fanxiaobao.xyz/Article/details/ghtpvukmt.sHtML

[U14] Py：分组收集到列表
来源：http://m.share.fanxiaobao.xyz/Article/details/gtoueeavd.sHtML

defaultdict(list)
来源：http://blog.fanxiaobao.xyz/Article/details/gnmdeanyt.sHtML


<!-- 参考信息 -->