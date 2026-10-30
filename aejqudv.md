代发 wailian999

date +"%Y-%m-%d %H:%M:%S"
来源：http://mobile.fehbvm.com/Article/details/guftrhqbo.sHtML

[R72] 等待端口就绪
来源：http://read.share.hesvh.cn/Article/details/gztrwtwep.sHtML

until nc -z localhost 3306; do sleep 1; done
来源：http://read.share.fehbvm.com/Article/details/gngnaykuk.sHtML

[R73] 分割大日志
来源：http://www.share.hesvh.cn/Article/details/gzzkkwnuq.sHtML

split -l 1000 big.log part_
来源：http://www.m.share.zdbjq.cn/Article/details/gzpbjnnxc.sHtML

[R74] 批量重命名
来源：http://www.blog.zdbjq.cn/Article/details/gjjtiylpt.sHtML

for f in *.jpeg; do mv "$f" "${f%.jpeg}.jpg"; done
来源：http://www.m.share.hesvh.cn/Article/details/gkduawomp.sHtML

[R75] 导出环境变量
来源：http://blog.hesvh.cn/Article/details/gxolwcpau.sHtML

export PATH="$HOME/bin:$PATH"
来源：http://baike.fehbvm.com/Article/details/gqlirpbrx.sHtML

[R76] 使用临时文件
来源：http://3g.fehbvm.com/Article/details/gsdzixtho.sHtML

tmp=$(mktemp); trap 'rm -f "$tmp"' EXIT
来源：http://mobile.hesvh.cn/Article/details/gqqvyyuop.sHtML

[R77] 读取用户输入
来源：http://www.share.zdbjq.cn/Article/details/gwaldhdvu.sHtML

read -rp "请输入: " ans
来源：http://3g.fehbvm.com/Article/details/gbbakfnet.sHtML

[R78] 交互式菜单
来源：http://www.m.share.fehbvm.com/Article/details/gjxggktvu.sHtML

select opt in a b c; do echo "$opt"; break; done
来源：http://read.share.hesvh.cn/Article/details/gclhazqqt.sHtML

[R79] 解析命令行选项
来源：http://3g.fehbvm.com/Article/details/gjbuarwsk.sHtML

while getopts "v:f:" o; do case $o in v) V=$OPTARG ;; f) F=$OPTARG ;; esac; done
来源：http://blog.hesvh.cn/Article/details/gjdanpzio.sHtML

[R80] 查看脚本执行耗时
来源：http://3g.fehbvm.com/Article/details/gtxgypnpx.sHtML

time ./run.sh
来源：http://blog.fehbvm.com/Article/details/gbkyinnna.sHtML

================================================================================
来源：http://baike.fehbvm.com/Article/details/gdbrcyehb.sHtML

S. C / C++ 专题
来源：http://mobile.fehbvm.com/Article/details/gwvigfpgx.sHtML

================================================================================
来源：http://wap.hesvh.cn/Article/details/gjdfvxudp.sHtML

[S01] C：Hello World
来源：http://blog.zdbjq.cn/Article/details/gshhbgndh.sHtML

#include <stdio.h>
来源：http://blog.fehbvm.com/Article/details/guudadwsy.sHtML

int main(void) { printf("Hello\n"); return 0; }
来源：http://baike.zdbjq.cn/Article/details/govqdcjtl.sHtML

[S02] C：变量与格式化输出
来源：http://3g.hesvh.cn/Article/details/gmytvdydh.sHtML

int a = 10; printf("%d\n", a);
来源：http://m.share.fehbvm.com/Article/details/grymlghfq.sHtML

[S03] C：读入整数
来源：http://www.share.fehbvm.com/Article/details/galznwfmu.sHtML

int x; scanf("%d", &x);
来源：http://3g.zdbjq.cn/Article/details/gnnwiyauc.sHtML

[S04] C：字符串复制
来源：http://mobile.zdbjq.cn/Article/details/gbnqxqgsv.sHtML

char dst[32]; strcpy(dst, "hi");
来源：http://baike.zdbjq.cn/Article/details/gxfcovhuk.sHtML

[S05] C：字符串长度
来源：http://m.share.fehbvm.com/Article/details/gdpeandyk.sHtML

strlen(s)
来源：http://3g.zdbjq.cn/Article/details/gtfpupbhr.sHtML

[S06] C：字符串比较
来源：http://blog.zdbjq.cn/Article/details/ggeicozlb.sHtML

strcmp(a, b) == 0
来源：http://www.blog.fehbvm.com/Article/details/gzsdxpxfl.sHtML

[S07] C：数组遍历求和
来源：http://mobile.fehbvm.com/Article/details/gvozhlcrt.sHtML

for (int i = 0; i < n; i++) sum += a[i];
来源：http://m.share.hesvh.cn/Article/details/gtbvrvkqj.sHtML

[S08] C：动态内存分配与释放
来源：http://read.share.fehbvm.com/Article/details/gpuiryhrk.sHtML

int *p = malloc(sizeof(int) * n); ... free(p);
来源：http://3g.fehbvm.com/Article/details/gefzqehfy.sHtML

[S09] C：结构体定义与初始化
来源：http://read.share.hesvh.cn/Article/details/gnitbokom.sHtML

struct Point { int x, y; };  struct Point p = {1, 2};
来源：http://read.share.hesvh.cn/Article/details/gwiaxtlef.sHtML

[S10] C：指针与解引用
来源：http://blog.fehbvm.com/Article/details/gjldwxjzx.sHtML

int *p = &a;  *p = 5;
来源：http://blog.hesvh.cn/Article/details/glisnawrl.sHtML

[S11] C：逐行读文件
来源：http://mobile.zdbjq.cn/Article/details/gopiymgsy.sHtML

FILE *f = fopen("a.txt", "r");
来源：http://baike.zdbjq.cn/Article/details/gcefrqhds.sHtML

while (fgets(buf, sizeof buf, f)) { }
来源：http://wap.hesvh.cn/Article/details/gglmjdvyn.sHtML

fclose(f);
来源：http://mobile.fehbvm.com/Article/details/gheioakxl.sHtML

[S12] C：写文件
来源：http://mobile.zdbjq.cn/Article/details/gdczwdrft.sHtML

FILE *f = fopen("a.txt", "w");  fprintf(f, "hi\n");  fclose(f);
来源：http://blog.fehbvm.com/Article/details/gnmucfjiz.sHtML

[S13] C：宏定义
来源：http://www.share.hesvh.cn/Article/details/ghbjlbipi.sHtML

#define MAX(a, b) ((a) > (b) ? (a) : (b))
来源：http://wap.hesvh.cn/Article/details/gopekukxa.sHtML

[S14] C：枚举
来源：http://mobile.hesvh.cn/Article/details/gurlzhsoc.sHtML

enum Color { RED, GREEN, BLUE };
来源：http://baike.fehbvm.com/Article/details/gdvgdqkyp.sHtML

[S15] C：类型转换
来源：http://www.blog.fehbvm.com/Article/details/grpgjfucp.sHtML

(double) a / b
来源：http://3g.fehbvm.com/Article/details/gijzipnmi.sHtML

[S16] C：位操作置位
来源：http://www.share.hesvh.cn/Article/details/gjvcsxvsj.sHtML

x |= (1 << 3);
来源：http://www.share.hesvh.cn/Article/details/gbagavkrh.sHtML

[S17] C：安全拼接字符串
来源：http://read.share.zdbjq.cn/Article/details/galinqobn.sHtML

snprintf(buf, sizeof buf, "%s%s", a, b);
来源：http://mobile.fehbvm.com/Article/details/geoxygamu.sHtML

[S18] C：命令行参数
来源：http://www.share.zdbjq.cn/Article/details/glejlbolv.sHtML

int main(int argc, char **argv)
来源：http://baike.hesvh.cn/Article/details/gwzdguobc.sHtML

[S19] C：快速排序
来源：http://m.share.hesvh.cn/Article/details/gnmtuqkkn.sHtML

qsort(a, n, sizeof(int), cmp);
来源：http://baike.fehbvm.com/Article/details/gicrqxmvl.sHtML

[S20] C：二分查找
来源：http://www.share.hesvh.cn/Article/details/gvpucfrrn.sHtML

bsearch(&key, a, n, sizeof(int), cmp);
来源：http://wap.hesvh.cn/Article/details/gixigdzii.sHtML

[S21] C：字符类别判断
来源：http://m.share.zdbjq.cn/Article/details/glsndvarj.sHtML

isdigit(c);  isalpha(c);  isspace(c);
来源：http://mobile.zdbjq.cn/Article/details/glitlpinh.sHtML

[S22] C：字符串转数字
来源：http://baike.zdbjq.cn/Article/details/gwdfoozvz.sHtML

atoi("42");  strtod("3.14", NULL);
来源：http://baike.hesvh.cn/Article/details/giluolwmy.sHtML

[S23] C：随机数
来源：http://m.share.zdbjq.cn/Article/details/gkujamfjb.sHtML

srand(time(NULL));  int r = rand() % 100;
来源：http://wap.fehbvm.com/Article/details/gewvueioa.sHtML

[S24] C：获取本地时间
来源：http://mobile.fehbvm.com/Article/details/gunhokssc.sHtML

time_t t = time(NULL);  struct tm *tm = localtime(&t);
来源：http://3g.hesvh.cn/Article/details/gpuqoprde.sHtML

[S25] C：内存拷贝
来源：http://m.share.zdbjq.cn/Article/details/ghdiekyxb.sHtML

memcpy(dst, src, n);
来源：http://www.share.hesvh.cn/Article/details/gpmjunysq.sHtML

[S26] C：内存清零
来源：http://m.share.hesvh.cn/Article/details/gvrvewkrm.sHtML

memset(a, 0, sizeof a);
来源：http://m.share.zdbjq.cn/Article/details/gqcptkfrr.sHtML

[S27] C：定义常量
来源：http://www.blog.zdbjq.cn/Article/details/gqdyvashq.sHtML

const double PI = 3.14159;
来源：http://www.m.share.fehbvm.com/Article/details/gkxoqsxys.sHtML

[S28] C：静态变量
来源：http://www.share.hesvh.cn/Article/details/gwjafwjgt.sHtML

static int counter = 0;
来源：http://mobile.fehbvm.com/Article/details/gclwckqnu.sHtML

[S29] C：变参函数
来源：http://www.m.share.fehbvm.com/Article/details/gnaayzkgz.sHtML

va_list ap; va_start(ap, fmt); vprintf(fmt, ap); va_end(ap);
来源：http://www.share.hesvh.cn/Article/details/gqcpcjlzz.sHtML

[S30] C：头文件保护
来源：http://m.share.zdbjq.cn/Article/details/gxauxxbrg.sHtML

#ifndef X_H
来源：http://blog.zdbjq.cn/Article/details/gfvofzhje.sHtML

#define X_H
来源：http://wap.fehbvm.com/Article/details/gvcpyxvoe.sHtML

#endif
来源：http://blog.hesvh.cn/Article/details/gmoqmxewi.sHtML

[S31] C++：Hello World
来源：http://baike.zdbjq.cn/Article/details/guuzmdxid.sHtML

#include <iostream>
来源：http://www.m.share.fehbvm.com/Article/details/gqsywsodn.sHtML

int main() { std::cout << "Hello\n"; }
来源：http://www.blog.hesvh.cn/Article/details/gulityaod.sHtML

[S32] C++：字符串
来源：http://wap.fehbvm.com/Article/details/gekgjnhgg.sHtML

std::string s = "hi";  s += "!";
来源：http://www.m.share.fehbvm.com/Article/details/gvdsahpzp.sHtML

[S33] C++：vector 增删
来源：http://3g.zdbjq.cn/Article/details/goklohlfd.sHtML

std::vector<int> v{1, 2, 3};  v.push_back(4);
来源：http://wap.zdbjq.cn/Article/details/gwycqazoe.sHtML

[S34] C++：遍历 vector
来源：http://wap.fehbvm.com/Article/details/gtdjtospr.sHtML

for (auto &x : v) { std::cout << x; }
来源：http://m.share.fehbvm.com/Article/details/gwxmguqmj.sHtML

[S35] C++：map
来源：http://blog.fehbvm.com/Article/details/gjycsmjew.sHtML

std::map<std::string, int> m;  m["a"] = 1;
来源：http://wap.zdbjq.cn/Article/details/ggcdcwnuc.sHtML

[S36] C++：unordered_map
来源：http://m.share.zdbjq.cn/Article/details/gylyesdvq.sHtML

std::unordered_map<std::string, int> m;  m["a"] = 1;
来源：http://blog.zdbjq.cn/Article/details/glgjdaitb.sHtML

[S37] C++：set
来源：http://m.share.hesvh.cn/Article/details/ggwlakqyl.sHtML

std::set<int> s{1, 2, 3};  s.insert(4);
来源：http://read.share.zdbjq.cn/Article/details/gijtijrhg.sHtML

[S38] C++：排序
来源：http://read.share.zdbjq.cn/Article/details/gaxmsufzu.sHtML

std::sort(v.begin(), v.end());
来源：http://read.share.hesvh.cn/Article/details/gpaetinaf.sHtML

[S39] C++：自定义比较器排序
来源：http://baike.zdbjq.cn/Article/details/gvznkjase.sHtML

std::sort(v.begin(), v.end(), [](int a, int b) { return a > b; });
来源：http://3g.hesvh.cn/Article/details/gcbauhhos.sHtML

[S40] C++：查找元素
来源：http://baike.hesvh.cn/Article/details/gtmeussuq.sHtML

auto it = std::find(v.begin(), v.end(), 3);
来源：http://www.m.share.zdbjq.cn/Article/details/geqmrsifp.sHtML

[S41] C++：类与构造函数
来源：http://mobile.fehbvm.com/Article/details/gngtgwwww.sHtML

class A { public: A(int v) : x_(v) {} int get() const { return x_; } private: int x_; };
来源：http://mobile.hesvh.cn/Article/details/gmzjubhnw.sHtML

[S42] C++：继承与虚函数
来源：http://www.share.hesvh.cn/Article/details/gxnfpgbuc.sHtML

class B : public Base { public: void f() override {} };
来源：http://www.m.share.hesvh.cn/Article/details/gyskvnwbx.sHtML

[S43] C++：智能指针
来源：http://read.share.fehbvm.com/Article/details/ghialymkd.sHtML

auto p = std::make_unique<int>(5);
来源：http://baike.hesvh.cn/Article/details/gpvqwvjuk.sHtML

[S44] C++：引用传参
来源：http://www.m.share.fehbvm.com/Article/details/gjtfbhvuu.sHtML

void inc(int &x) { ++x; }
来源：http://mobile.hesvh.cn/Article/details/gzypezibj.sHtML

[S45] C++：lambda
来源：http://www.m.share.fehbvm.com/Article/details/gqgxpwpts.sHtML

auto add = [](int a, int b) { return a + b; };
来源：http://read.share.fehbvm.com/Article/details/gihafjbcy.sHtML

[S46] C++：函数模板
来源：http://baike.fehbvm.com/Article/details/gxtbnocrg.sHtML

template <typename T> T maxv(T a, T b) { return a > b ? a : b; }
来源：http://3g.hesvh.cn/Article/details/gcrbmnzar.sHtML

[S47] C++：结构化绑定遍历
来源：http://www.m.share.zdbjq.cn/Article/details/gkhgidzli.sHtML

for (const auto &[k, v] : m) { std::cout << k << v; }
来源：http://wap.zdbjq.cn/Article/details/ghdovlbdz.sHtML

[S48] C++：逐行读文件
来源：http://blog.hesvh.cn/Article/details/gtluexnrh.sHtML

std::ifstream in("a.txt");  std::string line;
来源：http://3g.fehbvm.com/Article/details/gmikqfxkh.sHtML

while (std::getline(in, line)) { }
来源：http://www.blog.zdbjq.cn/Article/details/gfpnzlhio.sHtML

[S49] C++：写文件
来源：http://m.share.fehbvm.com/Article/details/gvbtgwjke.sHtML

std::ofstream out("a.txt");  out << "hi\n";
来源：http://mobile.zdbjq.cn/Article/details/gfzbatiug.sHtML

[S50] C++：格式化数字
来源：http://blog.fehbvm.com/Article/details/gynzwqsxs.sHtML

std::ostringstream os;  os << std::fixed << std::setprecision(2) << 3.14159;
来源：http://mobile.zdbjq.cn/Article/details/ghmyifsjw.sHtML

[S51] C++：显式类型转换
来源：http://www.blog.zdbjq.cn/Article/details/giefhbhlq.sHtML

static_cast<double>(a) / b
来源：http://blog.hesvh.cn/Article/details/gljcqxydv.sHtML

[S52] C++：const 与 noexcept
来源：http://www.m.share.hesvh.cn/Article/details/gupqntubx.sHtML

int size() const noexcept { return n_; }
来源：http://www.blog.hesvh.cn/Article/details/gjlnfyqqt.sHtML

[S53] C++：移动语义
来源：http://mobile.fehbvm.com/Article/details/gqwpvzxks.sHtML

std::vector<int> w = std::move(v);
来源：http://www.blog.hesvh.cn/Article/details/gehkoxfxb.sHtML

[S54] C++：异常处理
来源：http://blog.zdbjq.cn/Article/details/grgulrmag.sHtML

try { throw std::runtime_error("x"); } catch (const std::exception &e) { }
来源：http://baike.fehbvm.com/Article/details/gtcfwqcxu.sHtML

[S55] C++：结构化绑定
来源：http://blog.fehbvm.com/Article/details/gqojdftcs.sHtML

auto [a, b] = std::make_pair(1, 2);
来源：http://baike.fehbvm.com/Article/details/glfxoysmh.sHtML

[S56] C++：optional
来源：http://www.blog.fehbvm.com/Article/details/gjiaxrlze.sHtML

std::optional<int> o = 5;  if (o) { int v = *o; }
来源：http://m.share.fehbvm.com/Article/details/ghlzkibod.sHtML

[S57] C++：编译期常量
来源：http://3g.fehbvm.com/Article/details/gvrxqdyfc.sHtML

constexpr int N = 10;
来源：http://baike.fehbvm.com/Article/details/gqitkqrpw.sHtML

[S58] C++：命名空间
来源：http://blog.zdbjq.cn/Article/details/gzerxrjjf.sHtML

namespace ns { int f() { return 1; } }
来源：http://www.share.hesvh.cn/Article/details/grlrzuybk.sHtML

[S59] C++：静态断言
来源：http://blog.hesvh.cn/Article/details/gexhclrkm.sHtML

static_assert(sizeof(int) == 4, "int 必须 4 字节");
来源：http://m.share.fehbvm.com/Article/details/gfkiixjqw.sHtML

[S60] C++：遍历并删除元素
来源：http://blog.fehbvm.com/Article/details/gbbjhzabi.sHtML

v.erase(std::remove_if(v.begin(), v.end(), [](int x) { return x < 0; }), v.end());
来源：http://wap.zdbjq.cn/Article/details/gdapvrzmv.sHtML

================================================================================
来源：http://blog.hesvh.cn/Article/details/gvfhsgxjp.sHtML

T. 其他语言补充（Kotlin / Swift / Lua / Perl / Scala）
来源：http://m.share.hesvh.cn/Article/details/gqnugzctv.sHtML

================================================================================
来源：http://www.blog.fehbvm.com/Article/details/ggiinhxqo.sHtML

[T01] Kotlin：Hello World
来源：http://www.blog.hesvh.cn/Article/details/gwzferevh.sHtML

println("Hello")
来源：http://baike.zdbjq.cn/Article/details/gtkjtqmyl.sHtML

[T02] Kotlin：变量
来源：http://www.share.hesvh.cn/Article/details/gjmkcdkqn.sHtML

val a = 1;  var b = 2        // val 只读，var 可变
来源：http://www.blog.fehbvm.com/Article/details/gyfaiyrpc.sHtML

[T03] Kotlin：字符串模板
来源：http://m.share.hesvh.cn/Article/details/gqiefursm.sHtML

"值: $b"
来源：http://read.share.hesvh.cn/Article/details/gyateutla.sHtML

[T04] Kotlin：空安全
来源：http://blog.hesvh.cn/Article/details/gekfgjzmb.sHtML

val n: String? = null;  n?.length
来源：http://blog.hesvh.cn/Article/details/ghomkquha.sHtML

[T05] Kotlin：when 表达式
来源：http://blog.fehbvm.com/Article/details/gejkjdgig.sHtML

val s = when (x) { 1 -> "一" else -> "其他" }   // 多分支时每个分支单独一行
来源：http://www.m.share.hesvh.cn/Article/details/gevfhpith.sHtML

[T06] Kotlin：集合映射
来源：http://www.share.hesvh.cn/Article/details/gjjtipsqs.sHtML

listOf(1, 2, 3).map { it * 2 }
来源：http://www.blog.fehbvm.com/Article/details/ghgtrrytz.sHtML

[T07] Kotlin：集合过滤
来源：http://mobile.zdbjq.cn/Article/details/goetlzlbt.sHtML

listOf(1, 2, 3).filter { it > 1 }
来源：http://www.blog.hesvh.cn/Article/details/gatppvquh.sHtML

[T08] Kotlin：数据类
来源：http://m.share.fehbvm.com/Article/details/gooqdhzak.sHtML

data class User(val name: String, val age: Int)
来源：http://www.m.share.hesvh.cn/Article/details/ghtdtkncb.sHtML

[T09] Kotlin：扩展函数
来源：http://www.blog.hesvh.cn/Article/details/gzmkqvxfj.sHtML

fun String.exclaim() = this + "!"
来源：http://www.blog.fehbvm.com/Article/details/gnbxzuxsf.sHtML

[T10] Kotlin：默认参数
来源：http://3g.zdbjq.cn/Article/details/gnboxbkst.sHtML

fun greet(name: String = "World") = "Hi $name"
来源：http://3g.zdbjq.cn/Article/details/gmogwzwop.sHtML

[T11] Kotlin：协程
来源：http://blog.fehbvm.com/Article/details/gigzjmusn.sHtML

GlobalScope.launch { delay(1000); println("done") }
来源：http://www.m.share.hesvh.cn/Article/details/gnrlyjejq.sHtML

[T12] Kotlin：解构声明
来源：http://m.share.zdbjq.cn/Article/details/gzxntucfn.sHtML

val (a, b) = Pair(1, 2)
来源：http://www.blog.fehbvm.com/Article/details/gmsjlwrnu.sHtML

[T13] Kotlin：只读 Map
来源：http://m.share.hesvh.cn/Article/details/gbxdwterh.sHtML

val m = mapOf("a" to 1)
来源：http://www.blog.hesvh.cn/Article/details/gwswqtjqh.sHtML

[T14] Kotlin：循环
来源：http://blog.fehbvm.com/Article/details/gmdpvqquv.sHtML

for (i in 1..10) println(i)
来源：http://m.share.fehbvm.com/Article/details/gdtbjcbnu.sHtML

[T15] Kotlin：接口
来源：http://www.m.share.fehbvm.com/Article/details/geslocrmy.sHtML

interface Shape { fun area(): Double }
来源：http://baike.fehbvm.com/Article/details/gegdlrcnh.sHtML

[T16] Swift：Hello World
来源：http://blog.zdbjq.cn/Article/details/ggcszihfz.sHtML

print("Hello")
来源：http://m.share.hesvh.cn/Article/details/glynjuifl.sHtML

[T17] Swift：变量与常量
来源：http://m.share.fehbvm.com/Article/details/geoeqshxe.sHtML

var a = 1;  let b = 2
来源：http://mobile.fehbvm.com/Article/details/ghjousxwp.sHtML

[T18] Swift：字符串插值
来源：http://www.share.hesvh.cn/Article/details/gpogfdiza.sHtML

"值: \(b)"
来源：http://3g.fehbvm.com/Article/details/gwdyyqach.sHtML

[T19] Swift：可选绑定
来源：http://blog.hesvh.cn/Article/details/ggnrzpyix.sHtML

if let n = opt { print(n) }
来源：http://read.share.zdbjq.cn/Article/details/ghtwifhyf.sHtML

[T20] Swift：数组操作
来源：http://mobile.zdbjq.cn/Article/details/gzkdnkrzn.sHtML

var a = [1, 2, 3];  a.append(4)
来源：http://3g.fehbvm.com/Article/details/getmayzwr.sHtML

[T21] Swift：遍历
来源：http://www.blog.fehbvm.com/Article/details/gzltcbcmy.sHtML

for x in a { print(x) }
来源：http://m.share.fehbvm.com/Article/details/gfyoujbvz.sHtML

[T22] Swift：字典
来源：http://mobile.zdbjq.cn/Article/details/gtvcaimyx.sHtML

var d = ["a": 1];  d["b"] = 2
来源：http://www.m.share.hesvh.cn/Article/details/gbpkqdtys.sHtML

[T23] Swift：函数
来源：http://mobile.zdbjq.cn/Article/details/gkbgntllk.sHtML

func add(_ a: Int, _ b: Int) -> Int { a + b }
来源：http://mobile.zdbjq.cn/Article/details/gbgdmoxvg.sHtML

[T24] Swift：闭包
来源：http://m.share.hesvh.cn/Article/details/gmgoeetcm.sHtML

let f = { (x: Int) -> Int in x * 2 }
来源：http://read.share.fehbvm.com/Article/details/gunafnpai.sHtML

[T25] Swift：结构体
来源：http://www.m.share.fehbvm.com/Article/details/ghutkwrfo.sHtML

struct P { var x: Int }
来源：http://3g.zdbjq.cn/Article/details/gsiydwqhe.sHtML

[T26] Swift：类与重写
来源：http://www.m.share.fehbvm.com/Article/details/gghheiotu.sHtML

class A: Base { override func f() {} }
来源：http://www.m.share.zdbjq.cn/Article/details/grbkuyava.sHtML

[T27] Swift：错误处理
来源：http://blog.hesvh.cn/Article/details/gtxexwicj.sHtML

do { try f() } catch { print(error) }
来源：http://blog.hesvh.cn/Article/details/gklugwdok.sHtML

[T28] Swift：枚举
来源：http://3g.fehbvm.com/Article/details/grzqcnqcr.sHtML

enum Color { case red, green }
来源：http://baike.fehbvm.com/Article/details/glgjbeezk.sHtML

[T29] Swift：guard 提前返回
来源：http://mobile.fehbvm.com/Article/details/gypwpwthg.sHtML

guard let x = opt else { return }
来源：http://read.share.fehbvm.com/Article/details/gfsmcsbdo.sHtML

[T30] Swift：协议
来源：http://blog.hesvh.cn/Article/details/gdyogyago.sHtML

protocol Shape { func area() -> Double }
来源：http://m.share.zdbjq.cn/Article/details/gvitrjito.sHtML

[T31] Lua：Hello World
来源：http://www.m.share.zdbjq.cn/Article/details/gczpeubxu.sHtML

print("Hello")
来源：http://www.share.fehbvm.com/Article/details/gcgaqmkqq.sHtML

[T32] Lua：局部变量
来源：http://3g.zdbjq.cn/Article/details/gvnvwavrs.sHtML

local a = 1
来源：http://www.blog.hesvh.cn/Article/details/gdwpmoicp.sHtML

[T33] Lua：表（数组）
来源：http://m.share.fehbvm.com/Article/details/gthicvofh.sHtML

local t = {1, 2, 3};  t[4] = 4
来源：http://www.m.share.zdbjq.cn/Article/details/grzblctrf.sHtML

[T34] Lua：遍历表
来源：http://wap.hesvh.cn/Article/details/gyiwceieg.sHtML

for i, v in ipairs(t) do print(i, v) end
来源：http://www.m.share.hesvh.cn/Article/details/gdvshonxc.sHtML

[T35] Lua：字典表
来源：http://www.m.share.fehbvm.com/Article/details/gaeksfavw.sHtML

local d = { a = 1 };  d.b = 2
来源：http://www.share.fehbvm.com/Article/details/gvvyjnovo.sHtML

[T36] Lua：函数
来源：http://mobile.fehbvm.com/Article/details/gqvqytaze.sHtML

function add(a, b) return a + b end
来源：http://3g.fehbvm.com/Article/details/gxnhxfedk.sHtML

[T37] Lua：字符串拼接
来源：http://wap.hesvh.cn/Article/details/gtpsmeluq.sHtML

"a" .. "b"
来源：http://www.blog.fehbvm.com/Article/details/gtuakyzry.sHtML

[T38] Lua：条件
来源：http://baike.zdbjq.cn/Article/details/gegnhnluz.sHtML

if x > 0 then print("正") end
来源：http://read.share.zdbjq.cn/Article/details/gqohedkqd.sHtML

[T39] Lua：模式匹配
来源：http://mobile.hesvh.cn/Article/details/gozjphymn.sHtML

string.find(s, "%d+")
来源：http://mobile.zdbjq.cn/Article/details/gfldteybu.sHtML

[T40] Lua：元表
来源：http://3g.zdbjq.cn/Article/details/gbkavohha.sHtML

setmetatable({}, { __index = base })
来源：http://baike.hesvh.cn/Article/details/ghljqbcnz.sHtML

[T41] Perl：Hello World
来源：http://www.share.zdbjq.cn/Article/details/gwfgzdwlq.sHtML

print "Hello\n";
来源：http://www.share.fehbvm.com/Article/details/ghenzeczr.sHtML

[T42] Perl：变量类型
来源：http://www.blog.hesvh.cn/Article/details/gxvdkpcga.sHtML

my $a = 1;  my @arr = (1, 2, 3);  my %h = (a => 1);
来源：http://baike.fehbvm.com/Article/details/glfrefahq.sHtML

[T43] Perl：字符串插值
来源：http://wap.hesvh.cn/Article/details/gtjsedmks.sHtML

"值: $a"
来源：http://www.share.hesvh.cn/Article/details/gxduqetqi.sHtML

[T44] Perl：条件
来源：http://www.share.fehbvm.com/Article/details/gebjhnmrf.sHtML

if ($a > 0) { print "正"; }
来源：http://www.share.fehbvm.com/Article/details/gtaqirliy.sHtML

[T45] Perl：数组遍历
来源：http://baike.fehbvm.com/Article/details/gibjzsrut.sHtML

for my $x (@arr) { print $x; }
来源：http://www.m.share.fehbvm.com/Article/details/gclnlzobq.sHtML

[T46] Perl：哈希操作
来源：http://www.share.hesvh.cn/Article/details/gfemjskqa.sHtML

$h{b} = 2;  for my $k (keys %h) { print "$k=$h{$k}"; }
来源：http://mobile.hesvh.cn/Article/details/goufegtng.sHtML

[T47] Perl：正则捕获
来源：http://mobile.fehbvm.com/Article/details/gaxzefuec.sHtML

if ($s =~ /(\d+)/) { print $1; }
来源：http://wap.zdbjq.cn/Article/details/gxoldahaz.sHtML

[T48] Perl：正则替换
来源：http://wap.fehbvm.com/Article/details/gtwlrhwie.sHtML

$s =~ s/old/new/g;
来源：http://www.share.fehbvm.com/Article/details/gfalhrpxk.sHtML

[T49] Perl：函数
来源：http://blog.fehbvm.com/Article/details/gzwhxriyp.sHtML

sub add { my ($a, $b) = @_; return $a + $b; }
来源：http://m.share.zdbjq.cn/Article/details/gslnygqpt.sHtML

[T50] Perl：逐行读文件
来源：http://www.share.fehbvm.com/Article/details/gbhesxcls.sHtML

open my $fh, "<", "a.txt" or die $!;
来源：http://blog.fehbvm.com/Article/details/gaewswryo.sHtML

while (my $line = <$fh>) { print $line; }
来源：http://m.share.hesvh.cn/Article/details/gbejlzuam.sHtML

[T51] Scala：Hello World
来源：http://www.m.share.zdbjq.cn/Article/details/gkjqgudlf.sHtML

println("Hello")
来源：http://www.m.share.fehbvm.com/Article/details/goyrxdnsw.sHtML

[T52] Scala：变量
来源：http://wap.hesvh.cn/Article/details/giqgpmqfe.sHtML

val a = 1;  var b = 2
来源：http://3g.fehbvm.com/Article/details/glcckypqv.sHtML

[T53] Scala：字符串插值
来源：http://www.blog.fehbvm.com/Article/details/gkbunoswh.sHtML

s"值: $b"
来源：http://m.share.hesvh.cn/Article/details/gahvbuutu.sHtML

[T54] Scala：集合映射
来源：http://m.share.zdbjq.cn/Article/details/gvkldgyxt.sHtML

List(1, 2, 3).map(_ * 2)
来源：http://www.blog.fehbvm.com/Article/details/gmmlprlhy.sHtML

[T55] Scala：集合过滤
来源：http://www.blog.zdbjq.cn/Article/details/gehcudomr.sHtML

List(1, 2, 3).filter(_ > 1)
来源：http://mobile.hesvh.cn/Article/details/gxvwfqlrf.sHtML

[T56] Scala：样例类
来源：http://wap.hesvh.cn/Article/details/gjexpfezh.sHtML

case class User(name: String, age: Int)
来源：http://www.blog.fehbvm.com/Article/details/gmxxjtzaf.sHtML

[T57] Scala：模式匹配
来源：http://mobile.hesvh.cn/Article/details/gvvwlctuz.sHtML

x match { case 1 => "一"; case _ => "其他" }
来源：http://read.share.hesvh.cn/Article/details/gqffvpavc.sHtML

[T58] Scala：函数定义
来源：http://www.m.share.hesvh.cn/Article/details/gwgekirsm.sHtML

def add(a: Int, b: Int): Int = a + b
来源：http://blog.zdbjq.cn/Article/details/gezsudizq.sHtML

[T59] Scala：循环
来源：http://wap.hesvh.cn/Article/details/ginarjnka.sHtML

for (i <- 1 to 10) println(i)
来源：http://www.m.share.hesvh.cn/Article/details/gmwrdicii.sHtML

[T60] Scala：折叠
来源：http://read.share.zdbjq.cn/Article/details/gcuekkeyl.sHtML

List(1, 2, 3).foldLeft(0)(_ + _)
来源：http://mobile.hesvh.cn/Article/details/gpssyoggr.sHtML

================================================================================
来源：http://mobile.zdbjq.cn/Article/details/ggbrgyfxg.sHtML

U. 高频实用片段（Python / PHP / JavaScript 各 40 条）
来源：http://www.m.share.fehbvm.com/Article/details/gkvjtwwij.sHtML

================================================================================
来源：http://3g.zdbjq.cn/Article/details/gzzpmqoei.sHtML

[U01] Py：创建虚拟环境
来源：http://baike.hesvh.cn/Article/details/gidpssdea.sHtML

python -m venv .venv && source .venv/bin/activate
来源：http://wap.fehbvm.com/Article/details/gjojvqbbg.sHtML

[U02] Py：导出 / 安装依赖
来源：http://www.share.hesvh.cn/Article/details/gavbusfxg.sHtML

pip freeze > requirements.txt;  pip install -r requirements.txt
来源：http://read.share.hesvh.cn/Article/details/gmbgagzgi.sHtML

[U03] Py：加载 .env 配置
来源：http://baike.hesvh.cn/Article/details/ghmamxvbh.sHtML

from dotenv import load_dotenv; load_dotenv()
来源：http://baike.zdbjq.cn/Article/details/gkaephqfx.sHtML

[U04] Py：变量调试打印
来源：http://baike.hesvh.cn/Article/details/gqyfagsiw.sHtML

print(f"{x=}")            # 输出 x=值，Python 3.8+
来源：http://3g.fehbvm.com/Article/details/gajczpqjq.sHtML

[U05] Py：列表去重且保序
来源：http://www.blog.fehbvm.com/Article/details/giwgrjomg.sHtML

list(dict.fromkeys(arr))
来源：http://read.share.zdbjq.cn/Article/details/gvnbrwaqd.sHtML

[U06] Py：合并两个字典
来源：http://blog.zdbjq.cn/Article/details/gmtldwnie.sHtML

{**a, **b}
来源：http://read.share.fehbvm.com/Article/details/gsbpyfqoo.sHtML

[U07] Py：反转字典键值
来源：http://blog.zdbjq.cn/Article/details/gjodohmwj.sHtML

{v: k for k, v in d.items()}
来源：http://wap.zdbjq.cn/Article/details/garjoekwk.sHtML

[U08] Py：展平二维列表
来源：http://www.m.share.fehbvm.com/Article/details/glvwpfbuz.sHtML

[y for x in nested for y in x]
来源：http://www.blog.hesvh.cn/Article/details/gryukxfeb.sHtML

[U09] Py：字典取最大值的键
来源：http://www.m.share.zdbjq.cn/Article/details/gmhgkrwru.sHtML

max(d, key=d.get)
来源：http://www.blog.hesvh.cn/Article/details/gbxjipkez.sHtML

[U10] Py：按值排序字典
来源：http://wap.hesvh.cn/Article/details/gjouzdcir.sHtML

dict(sorted(d.items(), key=lambda kv: kv[1]))
来源：http://read.share.zdbjq.cn/Article/details/gyscwjsct.sHtML

[U11] Py：生成器表达式
来源：http://www.blog.fehbvm.com/Article/details/grhcedkpb.sHtML

(x * 2 for x in arr)
来源：http://blog.zdbjq.cn/Article/details/gkswryfan.sHtML

[U12] Py：取出现最多的 3 个元素
来源：http://m.share.hesvh.cn/Article/details/gqzztjppv.sHtML

Counter(arr).most_common(3)
来源：http://wap.zdbjq.cn/Article/details/gqtphtffg.sHtML


<!-- 参考信息 -->