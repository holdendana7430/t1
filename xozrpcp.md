代发 wailian999

read -rp "请输入: " ans
来源：http://mobile.fehbvm.com/Article/details/gkuuyevtr.sHtML

[R78] 交互式菜单
来源：http://3g.fehbvm.com/Article/details/gmidteysc.sHtML

select opt in a b c; do echo "$opt"; break; done
来源：http://mobile.fehbvm.com/Article/details/geolbswgp.sHtML

[R79] 解析命令行选项
来源：http://3g.fehbvm.com/Article/details/gnwuyubuo.sHtML

while getopts "v:f:" o; do case $o in v) V=$OPTARG ;; f) F=$OPTARG ;; esac; done
来源：http://m.share.hesvh.cn/Article/details/gpbyxqdwa.sHtML

[R80] 查看脚本执行耗时
来源：http://read.share.fehbvm.com/Article/details/grfhpcaoe.sHtML

time ./run.sh
来源：http://read.share.hesvh.cn/Article/details/gigslveci.sHtML

================================================================================
来源：http://3g.hesvh.cn/Article/details/giuqltnlm.sHtML

S. C / C++ 专题
来源：http://3g.zdbjq.cn/Article/details/gzwpflpqu.sHtML

================================================================================
来源：http://read.share.zdbjq.cn/Article/details/ggxnocvir.sHtML

[S01] C：Hello World
来源：http://wap.fehbvm.com/Article/details/gxscuxwea.sHtML

#include <stdio.h>
来源：http://mobile.hesvh.cn/Article/details/gtjsrqxow.sHtML

int main(void) { printf("Hello\n"); return 0; }
来源：http://blog.hesvh.cn/Article/details/gkppwbmpw.sHtML

[S02] C：变量与格式化输出
来源：http://baike.fehbvm.com/Article/details/gwnxesjex.sHtML

int a = 10; printf("%d\n", a);
来源：http://www.blog.hesvh.cn/Article/details/gihetdetg.sHtML

[S03] C：读入整数
来源：http://baike.hesvh.cn/Article/details/goobawinh.sHtML

int x; scanf("%d", &x);
来源：http://blog.fehbvm.com/Article/details/ghyhgfygd.sHtML

[S04] C：字符串复制
来源：http://3g.fehbvm.com/Article/details/gmdfcpmar.sHtML

char dst[32]; strcpy(dst, "hi");
来源：http://m.share.hesvh.cn/Article/details/gczbzrlrc.sHtML

[S05] C：字符串长度
来源：http://mobile.hesvh.cn/Article/details/gxwkzwoeg.sHtML

strlen(s)
来源：http://www.m.share.zdbjq.cn/Article/details/gozvmgaiv.sHtML

[S06] C：字符串比较
来源：http://mobile.zdbjq.cn/Article/details/grshgndty.sHtML

strcmp(a, b) == 0
来源：http://wap.hesvh.cn/Article/details/ggfzdulkv.sHtML

[S07] C：数组遍历求和
来源：http://mobile.hesvh.cn/Article/details/gosiuulkb.sHtML

for (int i = 0; i < n; i++) sum += a[i];
来源：http://www.blog.fehbvm.com/Article/details/gmtsecnut.sHtML

[S08] C：动态内存分配与释放
来源：http://3g.fehbvm.com/Article/details/gibrvzimo.sHtML

int *p = malloc(sizeof(int) * n); ... free(p);
来源：http://www.m.share.hesvh.cn/Article/details/gfcdxljpi.sHtML

[S09] C：结构体定义与初始化
来源：http://blog.hesvh.cn/Article/details/gaehrmlxn.sHtML

struct Point { int x, y; };  struct Point p = {1, 2};
来源：http://read.share.hesvh.cn/Article/details/gpxvyvoqn.sHtML

[S10] C：指针与解引用
来源：http://blog.zdbjq.cn/Article/details/gequfkshy.sHtML

int *p = &a;  *p = 5;
来源：http://wap.fehbvm.com/Article/details/gthyyskht.sHtML

[S11] C：逐行读文件
来源：http://www.blog.fehbvm.com/Article/details/gaftfywbm.sHtML

FILE *f = fopen("a.txt", "r");
来源：http://read.share.zdbjq.cn/Article/details/grilewmfz.sHtML

while (fgets(buf, sizeof buf, f)) { }
来源：http://wap.zdbjq.cn/Article/details/gybeplcws.sHtML

fclose(f);
来源：http://www.m.share.hesvh.cn/Article/details/ghkuvkjkp.sHtML

[S12] C：写文件
来源：http://www.m.share.hesvh.cn/Article/details/gochcpwpv.sHtML

FILE *f = fopen("a.txt", "w");  fprintf(f, "hi\n");  fclose(f);
来源：http://m.share.hesvh.cn/Article/details/ghkwkctpt.sHtML

[S13] C：宏定义
来源：http://m.share.fehbvm.com/Article/details/gaxfofwje.sHtML

#define MAX(a, b) ((a) > (b) ? (a) : (b))
来源：http://wap.fehbvm.com/Article/details/gkuxgiemg.sHtML

[S14] C：枚举
来源：http://www.share.fehbvm.com/Article/details/gvdaxtdsq.sHtML

enum Color { RED, GREEN, BLUE };
来源：http://mobile.hesvh.cn/Article/details/gwwwkbkjo.sHtML

[S15] C：类型转换
来源：http://www.m.share.fehbvm.com/Article/details/gngyfqsnc.sHtML

(double) a / b
来源：http://www.blog.hesvh.cn/Article/details/gnxhiucxp.sHtML

[S16] C：位操作置位
来源：http://blog.fehbvm.com/Article/details/gtpcdibsa.sHtML

x |= (1 << 3);
来源：http://3g.fehbvm.com/Article/details/gscxcgbow.sHtML

[S17] C：安全拼接字符串
来源：http://baike.zdbjq.cn/Article/details/gwfilamyo.sHtML

snprintf(buf, sizeof buf, "%s%s", a, b);
来源：http://wap.zdbjq.cn/Article/details/gxtghbrdt.sHtML

[S18] C：命令行参数
来源：http://read.share.hesvh.cn/Article/details/gxlvzgzyx.sHtML

int main(int argc, char **argv)
来源：http://m.share.zdbjq.cn/Article/details/gztxhptio.sHtML

[S19] C：快速排序
来源：http://www.share.fehbvm.com/Article/details/ghgyudcbf.sHtML

qsort(a, n, sizeof(int), cmp);
来源：http://www.share.zdbjq.cn/Article/details/ggeriljsy.sHtML

[S20] C：二分查找
来源：http://read.share.hesvh.cn/Article/details/gtdjxsjju.sHtML

bsearch(&key, a, n, sizeof(int), cmp);
来源：http://m.share.hesvh.cn/Article/details/gzdgkldxu.sHtML

[S21] C：字符类别判断
来源：http://blog.zdbjq.cn/Article/details/gtxceuzeb.sHtML

isdigit(c);  isalpha(c);  isspace(c);
来源：http://www.m.share.fehbvm.com/Article/details/gebpvkczx.sHtML

[S22] C：字符串转数字
来源：http://baike.hesvh.cn/Article/details/gmqtzkrku.sHtML

atoi("42");  strtod("3.14", NULL);
来源：http://baike.zdbjq.cn/Article/details/ghnnylovl.sHtML

[S23] C：随机数
来源：http://read.share.zdbjq.cn/Article/details/gzvzucwqn.sHtML

srand(time(NULL));  int r = rand() % 100;
来源：http://www.share.hesvh.cn/Article/details/ggjuupfez.sHtML

[S24] C：获取本地时间
来源：http://blog.fehbvm.com/Article/details/gburwlkwr.sHtML

time_t t = time(NULL);  struct tm *tm = localtime(&t);
来源：http://read.share.fehbvm.com/Article/details/gpxapzeyf.sHtML

[S25] C：内存拷贝
来源：http://www.share.fehbvm.com/Article/details/gxwdvrqaz.sHtML

memcpy(dst, src, n);
来源：http://www.blog.fehbvm.com/Article/details/grncqzdin.sHtML

[S26] C：内存清零
来源：http://m.share.fehbvm.com/Article/details/ggpbrvyss.sHtML

memset(a, 0, sizeof a);
来源：http://read.share.hesvh.cn/Article/details/gdebpizmo.sHtML

[S27] C：定义常量
来源：http://www.blog.zdbjq.cn/Article/details/gistildit.sHtML

const double PI = 3.14159;
来源：http://www.blog.fehbvm.com/Article/details/giqtqhulh.sHtML

[S28] C：静态变量
来源：http://3g.zdbjq.cn/Article/details/gpgcnohal.sHtML

static int counter = 0;
来源：http://baike.hesvh.cn/Article/details/golmtjypb.sHtML

[S29] C：变参函数
来源：http://baike.hesvh.cn/Article/details/gaofggccb.sHtML

va_list ap; va_start(ap, fmt); vprintf(fmt, ap); va_end(ap);
来源：http://read.share.zdbjq.cn/Article/details/gbiybsvld.sHtML

[S30] C：头文件保护
来源：http://www.blog.zdbjq.cn/Article/details/gmbzcchwi.sHtML

#ifndef X_H
来源：http://www.blog.zdbjq.cn/Article/details/gxmwdlzxe.sHtML

#define X_H
来源：http://3g.zdbjq.cn/Article/details/grhvhzpoj.sHtML

#endif
来源：http://3g.hesvh.cn/Article/details/gctigdsre.sHtML

[S31] C++：Hello World
来源：http://mobile.hesvh.cn/Article/details/gemaqghiu.sHtML

#include <iostream>
来源：http://3g.zdbjq.cn/Article/details/gybftvvhq.sHtML

int main() { std::cout << "Hello\n"; }
来源：http://mobile.zdbjq.cn/Article/details/gdapsifoi.sHtML

[S32] C++：字符串
来源：http://3g.fehbvm.com/Article/details/gmxtxvlyg.sHtML

std::string s = "hi";  s += "!";
来源：http://m.share.zdbjq.cn/Article/details/ghyyjisvo.sHtML

[S33] C++：vector 增删
来源：http://read.share.hesvh.cn/Article/details/gfkrjibem.sHtML

std::vector<int> v{1, 2, 3};  v.push_back(4);
来源：http://read.share.hesvh.cn/Article/details/gghejybvb.sHtML

[S34] C++：遍历 vector
来源：http://baike.hesvh.cn/Article/details/gzmwnijnh.sHtML

for (auto &x : v) { std::cout << x; }
来源：http://www.m.share.hesvh.cn/Article/details/glxiohsya.sHtML

[S35] C++：map
来源：http://m.share.zdbjq.cn/Article/details/gebmfqnya.sHtML

std::map<std::string, int> m;  m["a"] = 1;
来源：http://read.share.hesvh.cn/Article/details/glotirtor.sHtML

[S36] C++：unordered_map
来源：http://baike.fehbvm.com/Article/details/gugcvnlsj.sHtML

std::unordered_map<std::string, int> m;  m["a"] = 1;
来源：http://wap.zdbjq.cn/Article/details/gluzgwtju.sHtML

[S37] C++：set
来源：http://www.blog.zdbjq.cn/Article/details/gjgrhdzqt.sHtML

std::set<int> s{1, 2, 3};  s.insert(4);
来源：http://www.m.share.zdbjq.cn/Article/details/gjlnlzoyc.sHtML

[S38] C++：排序
来源：http://baike.hesvh.cn/Article/details/gdjpbazdl.sHtML

std::sort(v.begin(), v.end());
来源：http://3g.hesvh.cn/Article/details/golascvmi.sHtML

[S39] C++：自定义比较器排序
来源：http://3g.zdbjq.cn/Article/details/gmkyhivia.sHtML

std::sort(v.begin(), v.end(), [](int a, int b) { return a > b; });
来源：http://mobile.zdbjq.cn/Article/details/gdwaqpwwa.sHtML

[S40] C++：查找元素
来源：http://blog.fehbvm.com/Article/details/geqlwtqqw.sHtML

auto it = std::find(v.begin(), v.end(), 3);
来源：http://blog.hesvh.cn/Article/details/guelsmwkz.sHtML

[S41] C++：类与构造函数
来源：http://mobile.fehbvm.com/Article/details/gytkgfczq.sHtML

class A { public: A(int v) : x_(v) {} int get() const { return x_; } private: int x_; };
来源：http://mobile.hesvh.cn/Article/details/gzklymqrk.sHtML

[S42] C++：继承与虚函数
来源：http://www.m.share.fehbvm.com/Article/details/gcafzraxj.sHtML

class B : public Base { public: void f() override {} };
来源：http://m.share.hesvh.cn/Article/details/gcnlrjcbf.sHtML

[S43] C++：智能指针
来源：http://www.share.zdbjq.cn/Article/details/guxcmyahw.sHtML

auto p = std::make_unique<int>(5);
来源：http://www.blog.hesvh.cn/Article/details/gxxrkgmiv.sHtML

[S44] C++：引用传参
来源：http://m.share.fehbvm.com/Article/details/galvhcyme.sHtML

void inc(int &x) { ++x; }
来源：http://baike.hesvh.cn/Article/details/gtzekqtdw.sHtML

[S45] C++：lambda
来源：http://www.blog.zdbjq.cn/Article/details/gyqifkonn.sHtML

auto add = [](int a, int b) { return a + b; };
来源：http://www.share.zdbjq.cn/Article/details/gwgyjdexk.sHtML

[S46] C++：函数模板
来源：http://m.share.zdbjq.cn/Article/details/gjhxmkmxi.sHtML

template <typename T> T maxv(T a, T b) { return a > b ? a : b; }
来源：http://read.share.zdbjq.cn/Article/details/gubkwwbfu.sHtML

[S47] C++：结构化绑定遍历
来源：http://read.share.fehbvm.com/Article/details/gwapzzvok.sHtML

for (const auto &[k, v] : m) { std::cout << k << v; }
来源：http://wap.zdbjq.cn/Article/details/gtuzwnvnw.sHtML

[S48] C++：逐行读文件
来源：http://read.share.hesvh.cn/Article/details/gamijtxzj.sHtML

std::ifstream in("a.txt");  std::string line;
来源：http://m.share.zdbjq.cn/Article/details/gjgwytocz.sHtML

while (std::getline(in, line)) { }
来源：http://m.share.hesvh.cn/Article/details/gaebkremv.sHtML

[S49] C++：写文件
来源：http://blog.zdbjq.cn/Article/details/gqpinslwf.sHtML

std::ofstream out("a.txt");  out << "hi\n";
来源：http://mobile.zdbjq.cn/Article/details/gdvwpppbp.sHtML

[S50] C++：格式化数字
来源：http://m.share.fehbvm.com/Article/details/gvnfqnjfp.sHtML

std::ostringstream os;  os << std::fixed << std::setprecision(2) << 3.14159;
来源：http://3g.hesvh.cn/Article/details/gbdnhxpqu.sHtML

[S51] C++：显式类型转换
来源：http://www.m.share.zdbjq.cn/Article/details/gtxjtpccq.sHtML

static_cast<double>(a) / b
来源：http://wap.fehbvm.com/Article/details/gjknzcrep.sHtML

[S52] C++：const 与 noexcept
来源：http://3g.hesvh.cn/Article/details/gskobzful.sHtML

int size() const noexcept { return n_; }
来源：http://read.share.zdbjq.cn/Article/details/gwgpghsja.sHtML

[S53] C++：移动语义
来源：http://blog.fehbvm.com/Article/details/gfnjrmovy.sHtML

std::vector<int> w = std::move(v);
来源：http://read.share.zdbjq.cn/Article/details/gmbiocivz.sHtML

[S54] C++：异常处理
来源：http://mobile.zdbjq.cn/Article/details/ggxbyxywe.sHtML

try { throw std::runtime_error("x"); } catch (const std::exception &e) { }
来源：http://blog.zdbjq.cn/Article/details/ggkhtjrhb.sHtML

[S55] C++：结构化绑定
来源：http://read.share.zdbjq.cn/Article/details/gbylljzbq.sHtML

auto [a, b] = std::make_pair(1, 2);
来源：http://baike.hesvh.cn/Article/details/gqlaubdjg.sHtML

[S56] C++：optional
来源：http://wap.fehbvm.com/Article/details/gxwjryobs.sHtML

std::optional<int> o = 5;  if (o) { int v = *o; }
来源：http://3g.hesvh.cn/Article/details/gxskzdvsq.sHtML

[S57] C++：编译期常量
来源：http://3g.hesvh.cn/Article/details/gqsblwzjs.sHtML

constexpr int N = 10;
来源：http://www.blog.fehbvm.com/Article/details/gxantfwaz.sHtML

[S58] C++：命名空间
来源：http://wap.fehbvm.com/Article/details/gutswvwyj.sHtML

namespace ns { int f() { return 1; } }
来源：http://www.m.share.hesvh.cn/Article/details/gbnxbhfgk.sHtML

[S59] C++：静态断言
来源：http://www.share.zdbjq.cn/Article/details/glspililh.sHtML

static_assert(sizeof(int) == 4, "int 必须 4 字节");
来源：http://baike.zdbjq.cn/Article/details/gccmejtlr.sHtML

[S60] C++：遍历并删除元素
来源：http://3g.zdbjq.cn/Article/details/goxpppxet.sHtML

v.erase(std::remove_if(v.begin(), v.end(), [](int x) { return x < 0; }), v.end());
来源：http://blog.hesvh.cn/Article/details/gsspgxddi.sHtML

================================================================================
来源：http://mobile.zdbjq.cn/Article/details/gaihiaasm.sHtML

T. 其他语言补充（Kotlin / Swift / Lua / Perl / Scala）
来源：http://www.share.fehbvm.com/Article/details/gxupeczow.sHtML

================================================================================
来源：http://blog.fehbvm.com/Article/details/gjcgkvrtg.sHtML

[T01] Kotlin：Hello World
来源：http://read.share.fehbvm.com/Article/details/gcwaicfux.sHtML

println("Hello")
来源：http://3g.fehbvm.com/Article/details/grqbcbrpo.sHtML

[T02] Kotlin：变量
来源：http://m.share.zdbjq.cn/Article/details/gkmoddzyj.sHtML

val a = 1;  var b = 2        // val 只读，var 可变
来源：http://www.share.hesvh.cn/Article/details/gqsbqjkbj.sHtML

[T03] Kotlin：字符串模板
来源：http://m.share.fehbvm.com/Article/details/gjqswumgy.sHtML

"值: $b"
来源：http://www.blog.hesvh.cn/Article/details/gwtqunazm.sHtML

[T04] Kotlin：空安全
来源：http://m.share.zdbjq.cn/Article/details/gyhdqgwbh.sHtML

val n: String? = null;  n?.length
来源：http://baike.hesvh.cn/Article/details/gitoniqjk.sHtML

[T05] Kotlin：when 表达式
来源：http://mobile.fehbvm.com/Article/details/gsnhzglke.sHtML

val s = when (x) { 1 -> "一" else -> "其他" }   // 多分支时每个分支单独一行
来源：http://blog.fehbvm.com/Article/details/gblxsbdsc.sHtML

[T06] Kotlin：集合映射
来源：http://mobile.zdbjq.cn/Article/details/gqdkzmpfu.sHtML

listOf(1, 2, 3).map { it * 2 }
来源：http://www.share.zdbjq.cn/Article/details/gorznwzhl.sHtML

[T07] Kotlin：集合过滤
来源：http://mobile.fehbvm.com/Article/details/glvlgqcnp.sHtML

listOf(1, 2, 3).filter { it > 1 }
来源：http://read.share.zdbjq.cn/Article/details/gyjdqwyzv.sHtML

[T08] Kotlin：数据类
来源：http://read.share.fehbvm.com/Article/details/glovhqcjv.sHtML

data class User(val name: String, val age: Int)
来源：http://blog.fehbvm.com/Article/details/gqmveodqn.sHtML

[T09] Kotlin：扩展函数
来源：http://3g.fehbvm.com/Article/details/grznbbupu.sHtML

fun String.exclaim() = this + "!"
来源：http://mobile.hesvh.cn/Article/details/gbwxgtuhi.sHtML

[T10] Kotlin：默认参数
来源：http://www.m.share.hesvh.cn/Article/details/grytpxsdc.sHtML

fun greet(name: String = "World") = "Hi $name"
来源：http://www.blog.hesvh.cn/Article/details/gxwdnhosg.sHtML

[T11] Kotlin：协程
来源：http://www.m.share.fehbvm.com/Article/details/gjmaiwobp.sHtML

GlobalScope.launch { delay(1000); println("done") }
来源：http://mobile.zdbjq.cn/Article/details/ganrlczpg.sHtML

[T12] Kotlin：解构声明
来源：http://mobile.zdbjq.cn/Article/details/gwiqhlhfz.sHtML

val (a, b) = Pair(1, 2)
来源：http://blog.fehbvm.com/Article/details/gdzmkmisl.sHtML

[T13] Kotlin：只读 Map
来源：http://3g.hesvh.cn/Article/details/gzyjtofsj.sHtML

val m = mapOf("a" to 1)
来源：http://blog.fehbvm.com/Article/details/gmhuvzeal.sHtML

[T14] Kotlin：循环
来源：http://blog.hesvh.cn/Article/details/gkmoyixuc.sHtML

for (i in 1..10) println(i)
来源：http://wap.zdbjq.cn/Article/details/gygrpiich.sHtML

[T15] Kotlin：接口
来源：http://www.share.fehbvm.com/Article/details/giarptlfz.sHtML

interface Shape { fun area(): Double }
来源：http://www.m.share.fehbvm.com/Article/details/gdwthwplt.sHtML

[T16] Swift：Hello World
来源：http://wap.hesvh.cn/Article/details/gcdnuryjz.sHtML

print("Hello")
来源：http://m.share.fehbvm.com/Article/details/gaabvouok.sHtML

[T17] Swift：变量与常量
来源：http://blog.fehbvm.com/Article/details/groptfequ.sHtML

var a = 1;  let b = 2
来源：http://wap.hesvh.cn/Article/details/gskgvwjan.sHtML

[T18] Swift：字符串插值
来源：http://3g.fehbvm.com/Article/details/gwlnxxllb.sHtML

"值: \(b)"
来源：http://wap.hesvh.cn/Article/details/guzdwesmp.sHtML

[T19] Swift：可选绑定
来源：http://read.share.hesvh.cn/Article/details/gdhdlptqo.sHtML

if let n = opt { print(n) }
来源：http://www.share.fehbvm.com/Article/details/gghpisrsr.sHtML

[T20] Swift：数组操作
来源：http://www.m.share.hesvh.cn/Article/details/gketxxamy.sHtML

var a = [1, 2, 3];  a.append(4)
来源：http://read.share.hesvh.cn/Article/details/gjonvzhqi.sHtML

[T21] Swift：遍历
来源：http://m.share.fehbvm.com/Article/details/gxahdotex.sHtML

for x in a { print(x) }
来源：http://wap.fehbvm.com/Article/details/gtvzihnhe.sHtML

[T22] Swift：字典
来源：http://3g.hesvh.cn/Article/details/gpxmrdtpb.sHtML

var d = ["a": 1];  d["b"] = 2
来源：http://baike.fehbvm.com/Article/details/gmghnduoh.sHtML

[T23] Swift：函数
来源：http://www.share.zdbjq.cn/Article/details/gszslztpt.sHtML

func add(_ a: Int, _ b: Int) -> Int { a + b }
来源：http://www.blog.fehbvm.com/Article/details/gryiaqonx.sHtML

[T24] Swift：闭包
来源：http://wap.fehbvm.com/Article/details/gottzsokh.sHtML

let f = { (x: Int) -> Int in x * 2 }
来源：http://www.m.share.fehbvm.com/Article/details/glvootntt.sHtML

[T25] Swift：结构体
来源：http://wap.fehbvm.com/Article/details/gyuxwirzm.sHtML

struct P { var x: Int }
来源：http://baike.zdbjq.cn/Article/details/gmsdwoqxt.sHtML

[T26] Swift：类与重写
来源：http://3g.fehbvm.com/Article/details/gmvqsnpdx.sHtML

class A: Base { override func f() {} }
来源：http://3g.zdbjq.cn/Article/details/gbwjhmdlk.sHtML

[T27] Swift：错误处理
来源：http://www.m.share.hesvh.cn/Article/details/gioakxyzb.sHtML

do { try f() } catch { print(error) }
来源：http://m.share.hesvh.cn/Article/details/ggoddpkgo.sHtML

[T28] Swift：枚举
来源：http://blog.hesvh.cn/Article/details/gdghiyunx.sHtML

enum Color { case red, green }
来源：http://m.share.hesvh.cn/Article/details/gzjpzneyq.sHtML

[T29] Swift：guard 提前返回
来源：http://baike.hesvh.cn/Article/details/gfonxnyop.sHtML

guard let x = opt else { return }
来源：http://baike.hesvh.cn/Article/details/gguhvoaqd.sHtML

[T30] Swift：协议
来源：http://www.m.share.fehbvm.com/Article/details/gutjufxsd.sHtML

protocol Shape { func area() -> Double }
来源：http://blog.hesvh.cn/Article/details/gizdymjdy.sHtML

[T31] Lua：Hello World
来源：http://www.share.zdbjq.cn/Article/details/gmvomgqwy.sHtML

print("Hello")
来源：http://www.share.hesvh.cn/Article/details/gcwlqwlxm.sHtML

[T32] Lua：局部变量
来源：http://www.blog.zdbjq.cn/Article/details/gbjxrwgkf.sHtML

local a = 1
来源：http://mobile.zdbjq.cn/Article/details/grnzgviqm.sHtML

[T33] Lua：表（数组）
来源：http://wap.hesvh.cn/Article/details/gednemrtp.sHtML

local t = {1, 2, 3};  t[4] = 4
来源：http://www.share.fehbvm.com/Article/details/geiyllzpn.sHtML

[T34] Lua：遍历表
来源：http://baike.hesvh.cn/Article/details/gcxhxxzpf.sHtML

for i, v in ipairs(t) do print(i, v) end
来源：http://3g.hesvh.cn/Article/details/gbteoqhkt.sHtML

[T35] Lua：字典表
来源：http://www.blog.hesvh.cn/Article/details/gzkrpgylr.sHtML

local d = { a = 1 };  d.b = 2
来源：http://www.share.zdbjq.cn/Article/details/ghdasokhf.sHtML

[T36] Lua：函数
来源：http://blog.zdbjq.cn/Article/details/gxmidbtts.sHtML

function add(a, b) return a + b end
来源：http://mobile.hesvh.cn/Article/details/geynpygpz.sHtML

[T37] Lua：字符串拼接
来源：http://www.share.fehbvm.com/Article/details/gywigfjri.sHtML

"a" .. "b"
来源：http://www.share.hesvh.cn/Article/details/gpxjjrylh.sHtML

[T38] Lua：条件
来源：http://read.share.fehbvm.com/Article/details/glglpjamm.sHtML

if x > 0 then print("正") end
来源：http://baike.zdbjq.cn/Article/details/gwynhpcob.sHtML

[T39] Lua：模式匹配
来源：http://3g.zdbjq.cn/Article/details/gazbxdeyj.sHtML

string.find(s, "%d+")
来源：http://www.share.fehbvm.com/Article/details/gmxoxyism.sHtML

[T40] Lua：元表
来源：http://blog.hesvh.cn/Article/details/gueizztvn.sHtML

setmetatable({}, { __index = base })
来源：http://www.m.share.zdbjq.cn/Article/details/gjxiykylf.sHtML

[T41] Perl：Hello World
来源：http://www.m.share.fehbvm.com/Article/details/gyrtdskpx.sHtML

print "Hello\n";
来源：http://www.share.hesvh.cn/Article/details/gsaghzosn.sHtML

[T42] Perl：变量类型
来源：http://3g.hesvh.cn/Article/details/gehdlpzqk.sHtML

my $a = 1;  my @arr = (1, 2, 3);  my %h = (a => 1);
来源：http://www.m.share.fehbvm.com/Article/details/gmzpujpel.sHtML

[T43] Perl：字符串插值
来源：http://mobile.hesvh.cn/Article/details/gdwsszbcc.sHtML

"值: $a"
来源：http://read.share.hesvh.cn/Article/details/geijhnvyg.sHtML

[T44] Perl：条件
来源：http://3g.zdbjq.cn/Article/details/gweqnfjwi.sHtML

if ($a > 0) { print "正"; }
来源：http://mobile.fehbvm.com/Article/details/gwrjfpdfb.sHtML

[T45] Perl：数组遍历
来源：http://read.share.zdbjq.cn/Article/details/gichbahhm.sHtML

for my $x (@arr) { print $x; }
来源：http://3g.fehbvm.com/Article/details/gpzanqlpp.sHtML

[T46] Perl：哈希操作
来源：http://read.share.zdbjq.cn/Article/details/gupvezfny.sHtML

$h{b} = 2;  for my $k (keys %h) { print "$k=$h{$k}"; }
来源：http://mobile.zdbjq.cn/Article/details/geipvjttd.sHtML

[T47] Perl：正则捕获
来源：http://mobile.zdbjq.cn/Article/details/gfpiccxpl.sHtML

if ($s =~ /(\d+)/) { print $1; }
来源：http://baike.zdbjq.cn/Article/details/grrzfzeak.sHtML

[T48] Perl：正则替换
来源：http://m.share.fehbvm.com/Article/details/grehijpgg.sHtML

$s =~ s/old/new/g;
来源：http://baike.hesvh.cn/Article/details/gptngbjqs.sHtML

[T49] Perl：函数
来源：http://www.blog.fehbvm.com/Article/details/gwleitbzi.sHtML

sub add { my ($a, $b) = @_; return $a + $b; }
来源：http://blog.fehbvm.com/Article/details/gnewvrmvu.sHtML

[T50] Perl：逐行读文件
来源：http://blog.hesvh.cn/Article/details/gcpptnzpa.sHtML

open my $fh, "<", "a.txt" or die $!;
来源：http://www.blog.fehbvm.com/Article/details/gzruhhazg.sHtML

while (my $line = <$fh>) { print $line; }
来源：http://baike.hesvh.cn/Article/details/grzarytet.sHtML

[T51] Scala：Hello World
来源：http://www.share.zdbjq.cn/Article/details/gbbtouuae.sHtML

println("Hello")
来源：http://www.m.share.hesvh.cn/Article/details/gyzchniez.sHtML

[T52] Scala：变量
来源：http://www.m.share.hesvh.cn/Article/details/gceeweywt.sHtML

val a = 1;  var b = 2
来源：http://3g.zdbjq.cn/Article/details/gsiifutys.sHtML

[T53] Scala：字符串插值
来源：http://www.share.hesvh.cn/Article/details/glgwlwvbm.sHtML

s"值: $b"
来源：http://read.share.hesvh.cn/Article/details/gascdrkon.sHtML

[T54] Scala：集合映射
来源：http://read.share.hesvh.cn/Article/details/gnwcmjorr.sHtML

List(1, 2, 3).map(_ * 2)
来源：http://m.share.hesvh.cn/Article/details/gyhhisixo.sHtML

[T55] Scala：集合过滤
来源：http://www.m.share.fehbvm.com/Article/details/glgeimypn.sHtML

List(1, 2, 3).filter(_ > 1)
来源：http://mobile.zdbjq.cn/Article/details/glfgllcqs.sHtML

[T56] Scala：样例类
来源：http://www.share.fehbvm.com/Article/details/gaioeshxl.sHtML

case class User(name: String, age: Int)
来源：http://wap.fehbvm.com/Article/details/gkgsbbvzs.sHtML

[T57] Scala：模式匹配
来源：http://www.blog.hesvh.cn/Article/details/gyijstatc.sHtML

x match { case 1 => "一"; case _ => "其他" }
来源：http://m.share.hesvh.cn/Article/details/guqximanp.sHtML

[T58] Scala：函数定义
来源：http://baike.zdbjq.cn/Article/details/geilftoti.sHtML

def add(a: Int, b: Int): Int = a + b
来源：http://read.share.zdbjq.cn/Article/details/gyzroaakw.sHtML

[T59] Scala：循环
来源：http://wap.hesvh.cn/Article/details/giatuhocg.sHtML

for (i <- 1 to 10) println(i)
来源：http://wap.hesvh.cn/Article/details/gzxdkcube.sHtML

[T60] Scala：折叠
来源：http://www.share.zdbjq.cn/Article/details/gfgewgsqw.sHtML

List(1, 2, 3).foldLeft(0)(_ + _)
来源：http://wap.zdbjq.cn/Article/details/gjfssxivu.sHtML

================================================================================
来源：http://baike.hesvh.cn/Article/details/giqgykypc.sHtML

U. 高频实用片段（Python / PHP / JavaScript 各 40 条）
来源：http://www.blog.hesvh.cn/Article/details/gpgqumjyg.sHtML

================================================================================
来源：http://read.share.zdbjq.cn/Article/details/gtdknowqz.sHtML

[U01] Py：创建虚拟环境
来源：http://mobile.hesvh.cn/Article/details/gtjcviatp.sHtML

python -m venv .venv && source .venv/bin/activate
来源：http://baike.hesvh.cn/Article/details/goxeytgwr.sHtML

[U02] Py：导出 / 安装依赖
来源：http://read.share.fehbvm.com/Article/details/ghncrpvyj.sHtML

pip freeze > requirements.txt;  pip install -r requirements.txt
来源：http://www.share.fehbvm.com/Article/details/gjmjvgdve.sHtML

[U03] Py：加载 .env 配置
来源：http://read.share.zdbjq.cn/Article/details/ggscedwcc.sHtML

from dotenv import load_dotenv; load_dotenv()
来源：http://www.share.fehbvm.com/Article/details/gwvbwmgtb.sHtML

[U04] Py：变量调试打印
来源：http://blog.zdbjq.cn/Article/details/gxnnwmsek.sHtML

print(f"{x=}")            # 输出 x=值，Python 3.8+
来源：http://www.share.fehbvm.com/Article/details/giqawlnfj.sHtML

[U05] Py：列表去重且保序
来源：http://blog.hesvh.cn/Article/details/gkvbgzyiz.sHtML

list(dict.fromkeys(arr))
来源：http://www.m.share.zdbjq.cn/Article/details/gttwgjlea.sHtML

[U06] Py：合并两个字典
来源：http://blog.zdbjq.cn/Article/details/gnjicxgll.sHtML

{**a, **b}
来源：http://read.share.hesvh.cn/Article/details/ggbtaepji.sHtML

[U07] Py：反转字典键值
来源：http://mobile.fehbvm.com/Article/details/gfolhrhya.sHtML

{v: k for k, v in d.items()}
来源：http://blog.zdbjq.cn/Article/details/grbzpbknw.sHtML

[U08] Py：展平二维列表
来源：http://wap.hesvh.cn/Article/details/gzqambsbh.sHtML

[y for x in nested for y in x]
来源：http://m.share.zdbjq.cn/Article/details/gslhxbgqp.sHtML

[U09] Py：字典取最大值的键
来源：http://baike.hesvh.cn/Article/details/ggwnuzkki.sHtML

max(d, key=d.get)
来源：http://m.share.fehbvm.com/Article/details/gycgntflm.sHtML

[U10] Py：按值排序字典
来源：http://3g.hesvh.cn/Article/details/gfvmuckqf.sHtML

dict(sorted(d.items(), key=lambda kv: kv[1]))
来源：http://www.m.share.fehbvm.com/Article/details/ggiridkuq.sHtML

[U11] Py：生成器表达式
来源：http://m.share.zdbjq.cn/Article/details/glugmmnrx.sHtML

(x * 2 for x in arr)
来源：http://m.share.hesvh.cn/Article/details/gvtvudwqb.sHtML

[U12] Py：取出现最多的 3 个元素
来源：http://wap.hesvh.cn/Article/details/gdslptgwa.sHtML

Counter(arr).most_common(3)
来源：http://mobile.hesvh.cn/Article/details/gsenyptpn.sHtML

[U13] Py：固定长度队列
来源：http://www.m.share.fehbvm.com/Article/details/ghlyaratv.sHtML

deque(maxlen=10)
来源：http://www.share.hesvh.cn/Article/details/gkispyuyq.sHtML

[U14] Py：分组收集到列表
来源：http://read.share.zdbjq.cn/Article/details/gcrelnmdi.sHtML

defaultdict(list)
来源：http://mobile.fehbvm.com/Article/details/gfntyzygi.sHtML

[U15] Py：高精度计时
来源：http://baike.fehbvm.com/Article/details/gctztowiv.sHtML

t = time.perf_counter()
来源：http://www.blog.hesvh.cn/Article/details/gpfkigiyt.sHtML

[U16] Py：命令行参数解析
来源：http://www.share.hesvh.cn/Article/details/gmtxzlvbl.sHtML

ap = argparse.ArgumentParser();  ap.add_argument("--name");  args = ap.parse_args()
来源：http://baike.zdbjq.cn/Article/details/gnmowbphx.sHtML

[U17] Py：初始化日志
来源：http://wap.hesvh.cn/Article/details/gigmxveyg.sHtML

logging.basicConfig(level=logging.INFO)
来源：http://3g.fehbvm.com/Article/details/ghbtludie.sHtML

[U18] Py：预编译正则
来源：http://3g.zdbjq.cn/Article/details/gaexcqsrd.sHtML

pat = re.compile(r"\d+")
来源：http://wap.fehbvm.com/Article/details/gmnealgwk.sHtML


<!-- 参考信息 -->