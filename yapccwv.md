代发 wailian999

openssl rand -hex 16
来源：http://3g.zdbjq.cn/Article/details/gnpcpyjjc.sHtML

[R68] 计算文件校验值
来源：http://www.blog.hesvh.cn/Article/details/gogznovfl.sHtML

sha256sum a.txt;  md5sum a.txt
来源：http://read.share.fehbvm.com/Article/details/gvzetgjak.sHtML

[R69] 生成随机密码
来源：http://3g.zdbjq.cn/Article/details/gddjepyox.sHtML

head -c 16 /dev/urandom | base64
来源：http://3g.zdbjq.cn/Article/details/godkekqdd.sHtML

[R70] 时间戳与互转
来源：http://mobile.fehbvm.com/Article/details/gmrwegmus.sHtML

date +%s;  date -d @1700000000
来源：http://www.m.share.hesvh.cn/Article/details/gjrecxbdi.sHtML

[R71] 日期格式化
来源：http://www.blog.fehbvm.com/Article/details/gppwvoouu.sHtML

date +"%Y-%m-%d %H:%M:%S"
来源：http://3g.hesvh.cn/Article/details/gjxuspher.sHtML

[R72] 等待端口就绪
来源：http://3g.fehbvm.com/Article/details/gfczhomgy.sHtML

until nc -z localhost 3306; do sleep 1; done
来源：http://wap.fehbvm.com/Article/details/gwsevtkhx.sHtML

[R73] 分割大日志
来源：http://blog.hesvh.cn/Article/details/gtxfkowah.sHtML

split -l 1000 big.log part_
来源：http://mobile.hesvh.cn/Article/details/ggvjerlrx.sHtML

[R74] 批量重命名
来源：http://read.share.zdbjq.cn/Article/details/gryplelpi.sHtML

for f in *.jpeg; do mv "$f" "${f%.jpeg}.jpg"; done
来源：http://www.m.share.zdbjq.cn/Article/details/gtskifsqq.sHtML

[R75] 导出环境变量
来源：http://read.share.hesvh.cn/Article/details/gwjrylslc.sHtML

export PATH="$HOME/bin:$PATH"
来源：http://blog.zdbjq.cn/Article/details/glhgsvsck.sHtML

[R76] 使用临时文件
来源：http://wap.zdbjq.cn/Article/details/gtbyipukq.sHtML

tmp=$(mktemp); trap 'rm -f "$tmp"' EXIT
来源：http://www.share.zdbjq.cn/Article/details/glsmhkzry.sHtML

[R77] 读取用户输入
来源：http://baike.zdbjq.cn/Article/details/gdbpimqax.sHtML

read -rp "请输入: " ans
来源：http://blog.zdbjq.cn/Article/details/gvmgpagbo.sHtML

[R78] 交互式菜单
来源：http://m.share.hesvh.cn/Article/details/gpqbmnnjq.sHtML

select opt in a b c; do echo "$opt"; break; done
来源：http://www.blog.fehbvm.com/Article/details/gezpexgtw.sHtML

[R79] 解析命令行选项
来源：http://3g.hesvh.cn/Article/details/gneqytkmu.sHtML

while getopts "v:f:" o; do case $o in v) V=$OPTARG ;; f) F=$OPTARG ;; esac; done
来源：http://blog.zdbjq.cn/Article/details/gdibvnjor.sHtML

[R80] 查看脚本执行耗时
来源：http://www.m.share.hesvh.cn/Article/details/gjqqmukvv.sHtML

time ./run.sh
来源：http://m.share.hesvh.cn/Article/details/gwgdrxrga.sHtML

================================================================================
来源：http://m.share.fehbvm.com/Article/details/gkahbtwco.sHtML

S. C / C++ 专题
来源：http://www.blog.hesvh.cn/Article/details/gjobbrocm.sHtML

================================================================================
来源：http://m.share.hesvh.cn/Article/details/gwnyscbep.sHtML

[S01] C：Hello World
来源：http://www.share.zdbjq.cn/Article/details/gnoqevjba.sHtML

#include <stdio.h>
来源：http://3g.fehbvm.com/Article/details/gynsksjks.sHtML

int main(void) { printf("Hello\n"); return 0; }
来源：http://3g.fehbvm.com/Article/details/ghdsgmevv.sHtML

[S02] C：变量与格式化输出
来源：http://blog.zdbjq.cn/Article/details/gggcoqqjw.sHtML

int a = 10; printf("%d\n", a);
来源：http://www.m.share.hesvh.cn/Article/details/gdairbxxj.sHtML

[S03] C：读入整数
来源：http://3g.hesvh.cn/Article/details/gasjhfgot.sHtML

int x; scanf("%d", &x);
来源：http://m.share.fehbvm.com/Article/details/gnngrqjxy.sHtML

[S04] C：字符串复制
来源：http://blog.zdbjq.cn/Article/details/gddhhfxhe.sHtML

char dst[32]; strcpy(dst, "hi");
来源：http://www.m.share.hesvh.cn/Article/details/gdjllnkrp.sHtML

[S05] C：字符串长度
来源：http://blog.zdbjq.cn/Article/details/gvfwamyhs.sHtML

strlen(s)
来源：http://www.m.share.hesvh.cn/Article/details/gqvcifcmq.sHtML

[S06] C：字符串比较
来源：http://read.share.hesvh.cn/Article/details/grmsgnafj.sHtML

strcmp(a, b) == 0
来源：http://www.m.share.hesvh.cn/Article/details/gqeoxfktu.sHtML

[S07] C：数组遍历求和
来源：http://read.share.zdbjq.cn/Article/details/gnugfoazd.sHtML

for (int i = 0; i < n; i++) sum += a[i];
来源：http://www.m.share.fehbvm.com/Article/details/gkbpjyaer.sHtML

[S08] C：动态内存分配与释放
来源：http://blog.fehbvm.com/Article/details/gleoiwsne.sHtML

int *p = malloc(sizeof(int) * n); ... free(p);
来源：http://3g.fehbvm.com/Article/details/gwutubelz.sHtML

[S09] C：结构体定义与初始化
来源：http://www.m.share.fehbvm.com/Article/details/gwizrlggq.sHtML

struct Point { int x, y; };  struct Point p = {1, 2};
来源：http://m.share.fehbvm.com/Article/details/gkbicgdcu.sHtML

[S10] C：指针与解引用
来源：http://www.blog.zdbjq.cn/Article/details/gfsvnlxow.sHtML

int *p = &a;  *p = 5;
来源：http://baike.fehbvm.com/Article/details/ghmsjrmjo.sHtML

[S11] C：逐行读文件
来源：http://www.share.zdbjq.cn/Article/details/glvqnausf.sHtML

FILE *f = fopen("a.txt", "r");
来源：http://wap.zdbjq.cn/Article/details/glacpgafm.sHtML

while (fgets(buf, sizeof buf, f)) { }
来源：http://read.share.zdbjq.cn/Article/details/gacfnxpub.sHtML

fclose(f);
来源：http://baike.hesvh.cn/Article/details/gwhvxwwba.sHtML

[S12] C：写文件
来源：http://www.m.share.hesvh.cn/Article/details/gtcujqztz.sHtML

FILE *f = fopen("a.txt", "w");  fprintf(f, "hi\n");  fclose(f);
来源：http://www.share.fehbvm.com/Article/details/gmbtfkxfz.sHtML

[S13] C：宏定义
来源：http://wap.hesvh.cn/Article/details/gitrxtwiq.sHtML

#define MAX(a, b) ((a) > (b) ? (a) : (b))
来源：http://baike.hesvh.cn/Article/details/gxygzdxmx.sHtML

[S14] C：枚举
来源：http://blog.fehbvm.com/Article/details/gxfarqebo.sHtML

enum Color { RED, GREEN, BLUE };
来源：http://blog.hesvh.cn/Article/details/gmitsimnu.sHtML

[S15] C：类型转换
来源：http://read.share.zdbjq.cn/Article/details/goiktsbug.sHtML

(double) a / b
来源：http://www.blog.fehbvm.com/Article/details/gwroelopw.sHtML

[S16] C：位操作置位
来源：http://www.m.share.hesvh.cn/Article/details/gpksikzit.sHtML

x |= (1 << 3);
来源：http://m.share.hesvh.cn/Article/details/gemyarqec.sHtML

[S17] C：安全拼接字符串
来源：http://wap.zdbjq.cn/Article/details/gpcsouqfb.sHtML

snprintf(buf, sizeof buf, "%s%s", a, b);
来源：http://3g.zdbjq.cn/Article/details/guncydblx.sHtML

[S18] C：命令行参数
来源：http://wap.fehbvm.com/Article/details/ghwkaxqix.sHtML

int main(int argc, char **argv)
来源：http://www.blog.fehbvm.com/Article/details/gnmlzmvdv.sHtML

[S19] C：快速排序
来源：http://baike.fehbvm.com/Article/details/gunrcauxx.sHtML

qsort(a, n, sizeof(int), cmp);
来源：http://www.m.share.zdbjq.cn/Article/details/gihbeoiza.sHtML

[S20] C：二分查找
来源：http://www.share.fehbvm.com/Article/details/gumrjvopr.sHtML

bsearch(&key, a, n, sizeof(int), cmp);
来源：http://blog.fehbvm.com/Article/details/grhyvivwm.sHtML

[S21] C：字符类别判断
来源：http://blog.zdbjq.cn/Article/details/gdfqarful.sHtML

isdigit(c);  isalpha(c);  isspace(c);
来源：http://baike.zdbjq.cn/Article/details/gxhuzquuz.sHtML

[S22] C：字符串转数字
来源：http://baike.hesvh.cn/Article/details/gfyextimr.sHtML

atoi("42");  strtod("3.14", NULL);
来源：http://wap.fehbvm.com/Article/details/gcuqglxjg.sHtML

[S23] C：随机数
来源：http://3g.zdbjq.cn/Article/details/gxcpeyqwb.sHtML

srand(time(NULL));  int r = rand() % 100;
来源：http://www.m.share.zdbjq.cn/Article/details/gqzpvtyge.sHtML

[S24] C：获取本地时间
来源：http://www.blog.fehbvm.com/Article/details/gdmytshrn.sHtML

time_t t = time(NULL);  struct tm *tm = localtime(&t);
来源：http://wap.hesvh.cn/Article/details/gpjtvdplb.sHtML

[S25] C：内存拷贝
来源：http://wap.hesvh.cn/Article/details/gryozewhn.sHtML

memcpy(dst, src, n);
来源：http://www.m.share.hesvh.cn/Article/details/gvrftwzgz.sHtML

[S26] C：内存清零
来源：http://wap.zdbjq.cn/Article/details/gpmivbdlv.sHtML

memset(a, 0, sizeof a);
来源：http://mobile.hesvh.cn/Article/details/gvdjvjehu.sHtML

[S27] C：定义常量
来源：http://m.share.zdbjq.cn/Article/details/gncdhbmid.sHtML

const double PI = 3.14159;
来源：http://3g.zdbjq.cn/Article/details/gcisrvguc.sHtML

[S28] C：静态变量
来源：http://mobile.zdbjq.cn/Article/details/grkcuitiz.sHtML

static int counter = 0;
来源：http://mobile.zdbjq.cn/Article/details/gqgaaksbc.sHtML

[S29] C：变参函数
来源：http://www.share.fehbvm.com/Article/details/gysxmhbcc.sHtML

va_list ap; va_start(ap, fmt); vprintf(fmt, ap); va_end(ap);
来源：http://www.blog.hesvh.cn/Article/details/gjirqoptg.sHtML

[S30] C：头文件保护
来源：http://www.blog.zdbjq.cn/Article/details/gxzfmjuzf.sHtML

#ifndef X_H
来源：http://blog.zdbjq.cn/Article/details/gwalamfvw.sHtML

#define X_H
来源：http://wap.zdbjq.cn/Article/details/gxvohhdqe.sHtML

#endif
来源：http://3g.zdbjq.cn/Article/details/gnnunoibm.sHtML

[S31] C++：Hello World
来源：http://mobile.zdbjq.cn/Article/details/gizvsdjcu.sHtML

#include <iostream>
来源：http://baike.fehbvm.com/Article/details/gcdvpqhks.sHtML

int main() { std::cout << "Hello\n"; }
来源：http://wap.zdbjq.cn/Article/details/gmujuzdme.sHtML

[S32] C++：字符串
来源：http://baike.fehbvm.com/Article/details/glifylygx.sHtML

std::string s = "hi";  s += "!";
来源：http://www.m.share.hesvh.cn/Article/details/ggqbnirxu.sHtML

[S33] C++：vector 增删
来源：http://read.share.fehbvm.com/Article/details/gafkrcfpj.sHtML

std::vector<int> v{1, 2, 3};  v.push_back(4);
来源：http://m.share.hesvh.cn/Article/details/gkomgsadi.sHtML

[S34] C++：遍历 vector
来源：http://mobile.hesvh.cn/Article/details/gnkgopsgc.sHtML

for (auto &x : v) { std::cout << x; }
来源：http://blog.fehbvm.com/Article/details/gizvunqag.sHtML

[S35] C++：map
来源：http://mobile.hesvh.cn/Article/details/grdqsotag.sHtML

std::map<std::string, int> m;  m["a"] = 1;
来源：http://3g.hesvh.cn/Article/details/gpmiiwvom.sHtML

[S36] C++：unordered_map
来源：http://baike.fehbvm.com/Article/details/gnlufhotv.sHtML

std::unordered_map<std::string, int> m;  m["a"] = 1;
来源：http://www.blog.hesvh.cn/Article/details/gpclqifkb.sHtML

[S37] C++：set
来源：http://blog.zdbjq.cn/Article/details/ghxkerbqx.sHtML

std::set<int> s{1, 2, 3};  s.insert(4);
来源：http://www.blog.zdbjq.cn/Article/details/gbviabieu.sHtML

[S38] C++：排序
来源：http://mobile.fehbvm.com/Article/details/gmdrdowcm.sHtML

std::sort(v.begin(), v.end());
来源：http://3g.zdbjq.cn/Article/details/guespwknq.sHtML

[S39] C++：自定义比较器排序
来源：http://3g.fehbvm.com/Article/details/gswijfcuq.sHtML

std::sort(v.begin(), v.end(), [](int a, int b) { return a > b; });
来源：http://mobile.zdbjq.cn/Article/details/gmycbyqfj.sHtML

[S40] C++：查找元素
来源：http://3g.fehbvm.com/Article/details/gckfbynfm.sHtML

auto it = std::find(v.begin(), v.end(), 3);
来源：http://blog.zdbjq.cn/Article/details/gcznuioqg.sHtML

[S41] C++：类与构造函数
来源：http://wap.hesvh.cn/Article/details/gqbyskqbh.sHtML

class A { public: A(int v) : x_(v) {} int get() const { return x_; } private: int x_; };
来源：http://read.share.hesvh.cn/Article/details/giejcfpuf.sHtML

[S42] C++：继承与虚函数
来源：http://3g.hesvh.cn/Article/details/gezbgrcac.sHtML

class B : public Base { public: void f() override {} };
来源：http://www.m.share.hesvh.cn/Article/details/glqqtosxz.sHtML

[S43] C++：智能指针
来源：http://www.m.share.fehbvm.com/Article/details/gisghrpyx.sHtML

auto p = std::make_unique<int>(5);
来源：http://blog.fehbvm.com/Article/details/glnlaximv.sHtML

[S44] C++：引用传参
来源：http://mobile.hesvh.cn/Article/details/gigqbfgqj.sHtML

void inc(int &x) { ++x; }
来源：http://blog.hesvh.cn/Article/details/gwwuijcbo.sHtML

[S45] C++：lambda
来源：http://www.blog.hesvh.cn/Article/details/gkcrpopmp.sHtML

auto add = [](int a, int b) { return a + b; };
来源：http://www.m.share.zdbjq.cn/Article/details/geamebmxq.sHtML

[S46] C++：函数模板
来源：http://mobile.hesvh.cn/Article/details/guwjqdxcv.sHtML

template <typename T> T maxv(T a, T b) { return a > b ? a : b; }
来源：http://3g.zdbjq.cn/Article/details/gradenspt.sHtML

[S47] C++：结构化绑定遍历
来源：http://3g.zdbjq.cn/Article/details/ghvnhznta.sHtML

for (const auto &[k, v] : m) { std::cout << k << v; }
来源：http://baike.zdbjq.cn/Article/details/gzzabvioh.sHtML

[S48] C++：逐行读文件
来源：http://3g.hesvh.cn/Article/details/gzeqrdmnp.sHtML

std::ifstream in("a.txt");  std::string line;
来源：http://read.share.fehbvm.com/Article/details/gfzracbys.sHtML

while (std::getline(in, line)) { }
来源：http://3g.hesvh.cn/Article/details/gntlnyuxa.sHtML

[S49] C++：写文件
来源：http://wap.hesvh.cn/Article/details/gqjqleirn.sHtML

std::ofstream out("a.txt");  out << "hi\n";
来源：http://m.share.fehbvm.com/Article/details/ggizobzsr.sHtML

[S50] C++：格式化数字
来源：http://mobile.zdbjq.cn/Article/details/gpggpvdbj.sHtML

std::ostringstream os;  os << std::fixed << std::setprecision(2) << 3.14159;
来源：http://3g.hesvh.cn/Article/details/gfjckcomf.sHtML

[S51] C++：显式类型转换
来源：http://m.share.hesvh.cn/Article/details/gofbzihpv.sHtML

static_cast<double>(a) / b
来源：http://baike.zdbjq.cn/Article/details/gutiehcun.sHtML

[S52] C++：const 与 noexcept
来源：http://baike.fehbvm.com/Article/details/gcfrcykni.sHtML

int size() const noexcept { return n_; }
来源：http://read.share.hesvh.cn/Article/details/gomtilwpc.sHtML

[S53] C++：移动语义
来源：http://blog.zdbjq.cn/Article/details/gmxxyfsqn.sHtML

std::vector<int> w = std::move(v);
来源：http://www.share.hesvh.cn/Article/details/gbcusynta.sHtML

[S54] C++：异常处理
来源：http://mobile.hesvh.cn/Article/details/gxsjespdl.sHtML

try { throw std::runtime_error("x"); } catch (const std::exception &e) { }
来源：http://m.share.zdbjq.cn/Article/details/gewczectw.sHtML

[S55] C++：结构化绑定
来源：http://www.share.zdbjq.cn/Article/details/gaapjjqig.sHtML

auto [a, b] = std::make_pair(1, 2);
来源：http://wap.zdbjq.cn/Article/details/glwnsmftj.sHtML

[S56] C++：optional
来源：http://www.blog.fehbvm.com/Article/details/gvwmcfmgj.sHtML

std::optional<int> o = 5;  if (o) { int v = *o; }
来源：http://3g.fehbvm.com/Article/details/gyprzyclg.sHtML

[S57] C++：编译期常量
来源：http://www.blog.zdbjq.cn/Article/details/ghmreexoq.sHtML

constexpr int N = 10;
来源：http://blog.hesvh.cn/Article/details/giglspgoe.sHtML

[S58] C++：命名空间
来源：http://wap.zdbjq.cn/Article/details/gofmcycgx.sHtML

namespace ns { int f() { return 1; } }
来源：http://www.share.hesvh.cn/Article/details/gauxtgrfr.sHtML

[S59] C++：静态断言
来源：http://read.share.hesvh.cn/Article/details/gccgbuwcf.sHtML

static_assert(sizeof(int) == 4, "int 必须 4 字节");
来源：http://3g.fehbvm.com/Article/details/gbwuzniyy.sHtML

[S60] C++：遍历并删除元素
来源：http://mobile.hesvh.cn/Article/details/gxdqyjsfx.sHtML

v.erase(std::remove_if(v.begin(), v.end(), [](int x) { return x < 0; }), v.end());
来源：http://m.share.zdbjq.cn/Article/details/gfirzpvxh.sHtML

================================================================================
来源：http://m.share.fehbvm.com/Article/details/gznawnfbt.sHtML

T. 其他语言补充（Kotlin / Swift / Lua / Perl / Scala）
来源：http://mobile.hesvh.cn/Article/details/gvoxzqnfk.sHtML

================================================================================
来源：http://www.m.share.fehbvm.com/Article/details/gvezenitq.sHtML

[T01] Kotlin：Hello World
来源：http://3g.zdbjq.cn/Article/details/geuohtfjn.sHtML

println("Hello")
来源：http://mobile.fehbvm.com/Article/details/gmgvjpnwy.sHtML

[T02] Kotlin：变量
来源：http://read.share.fehbvm.com/Article/details/goiixaioo.sHtML

val a = 1;  var b = 2        // val 只读，var 可变
来源：http://mobile.fehbvm.com/Article/details/gytzxlauw.sHtML

[T03] Kotlin：字符串模板
来源：http://3g.zdbjq.cn/Article/details/gjixotxut.sHtML

"值: $b"
来源：http://www.m.share.zdbjq.cn/Article/details/gotuqxkju.sHtML

[T04] Kotlin：空安全
来源：http://www.blog.hesvh.cn/Article/details/guwnezccs.sHtML

val n: String? = null;  n?.length
来源：http://read.share.fehbvm.com/Article/details/gkmkvjtqg.sHtML

[T05] Kotlin：when 表达式
来源：http://blog.fehbvm.com/Article/details/gtfieghnk.sHtML

val s = when (x) { 1 -> "一" else -> "其他" }   // 多分支时每个分支单独一行
来源：http://mobile.hesvh.cn/Article/details/gorbaixhd.sHtML

[T06] Kotlin：集合映射
来源：http://mobile.hesvh.cn/Article/details/gpstknwqi.sHtML

listOf(1, 2, 3).map { it * 2 }
来源：http://baike.fehbvm.com/Article/details/gwrkgeevz.sHtML

[T07] Kotlin：集合过滤
来源：http://read.share.fehbvm.com/Article/details/gmylbjjpm.sHtML

listOf(1, 2, 3).filter { it > 1 }
来源：http://read.share.fehbvm.com/Article/details/gmfahtumo.sHtML

[T08] Kotlin：数据类
来源：http://www.m.share.hesvh.cn/Article/details/gcpwoycdi.sHtML

data class User(val name: String, val age: Int)
来源：http://m.share.hesvh.cn/Article/details/gdazpazhp.sHtML

[T09] Kotlin：扩展函数
来源：http://read.share.fehbvm.com/Article/details/gmsmnhgpm.sHtML

fun String.exclaim() = this + "!"
来源：http://baike.hesvh.cn/Article/details/gdageefyo.sHtML

[T10] Kotlin：默认参数
来源：http://www.share.hesvh.cn/Article/details/gizmbplsk.sHtML

fun greet(name: String = "World") = "Hi $name"
来源：http://www.blog.fehbvm.com/Article/details/gbhvcmjcl.sHtML

[T11] Kotlin：协程
来源：http://www.share.hesvh.cn/Article/details/gwsgkxxyf.sHtML

GlobalScope.launch { delay(1000); println("done") }
来源：http://wap.zdbjq.cn/Article/details/govodayes.sHtML

[T12] Kotlin：解构声明
来源：http://mobile.hesvh.cn/Article/details/gwuxwaikl.sHtML

val (a, b) = Pair(1, 2)
来源：http://3g.zdbjq.cn/Article/details/gdffaosuf.sHtML

[T13] Kotlin：只读 Map
来源：http://wap.zdbjq.cn/Article/details/gqmkvfwfq.sHtML

val m = mapOf("a" to 1)
来源：http://wap.fehbvm.com/Article/details/gkaeotods.sHtML

[T14] Kotlin：循环
来源：http://www.share.hesvh.cn/Article/details/gemmqgdfk.sHtML

for (i in 1..10) println(i)
来源：http://wap.hesvh.cn/Article/details/ggyzmtleq.sHtML

[T15] Kotlin：接口
来源：http://www.m.share.hesvh.cn/Article/details/giibnguqb.sHtML

interface Shape { fun area(): Double }
来源：http://wap.hesvh.cn/Article/details/gortuksxf.sHtML

[T16] Swift：Hello World
来源：http://read.share.fehbvm.com/Article/details/gjycmhcee.sHtML

print("Hello")
来源：http://blog.hesvh.cn/Article/details/gvqhwfsfz.sHtML

[T17] Swift：变量与常量
来源：http://baike.fehbvm.com/Article/details/gdvsfdhpo.sHtML

var a = 1;  let b = 2
来源：http://read.share.fehbvm.com/Article/details/ggvwymoio.sHtML

[T18] Swift：字符串插值
来源：http://blog.zdbjq.cn/Article/details/gghuggxpk.sHtML

"值: \(b)"
来源：http://baike.zdbjq.cn/Article/details/gfdfqgsye.sHtML

[T19] Swift：可选绑定
来源：http://baike.hesvh.cn/Article/details/gkjdhdoan.sHtML

if let n = opt { print(n) }
来源：http://www.share.fehbvm.com/Article/details/gnvynyanv.sHtML

[T20] Swift：数组操作
来源：http://3g.zdbjq.cn/Article/details/gfkedpomn.sHtML

var a = [1, 2, 3];  a.append(4)
来源：http://www.share.zdbjq.cn/Article/details/gztmcntsu.sHtML

[T21] Swift：遍历
来源：http://www.m.share.zdbjq.cn/Article/details/gsamlylui.sHtML

for x in a { print(x) }
来源：http://m.share.zdbjq.cn/Article/details/ggobketph.sHtML

[T22] Swift：字典
来源：http://m.share.fehbvm.com/Article/details/gycehnpha.sHtML

var d = ["a": 1];  d["b"] = 2
来源：http://read.share.hesvh.cn/Article/details/gizvjqutc.sHtML

[T23] Swift：函数
来源：http://m.share.zdbjq.cn/Article/details/gfqckfprj.sHtML

func add(_ a: Int, _ b: Int) -> Int { a + b }
来源：http://blog.zdbjq.cn/Article/details/gdavctlnd.sHtML

[T24] Swift：闭包
来源：http://baike.hesvh.cn/Article/details/gztluydpv.sHtML

let f = { (x: Int) -> Int in x * 2 }
来源：http://blog.zdbjq.cn/Article/details/gjjjruobu.sHtML

[T25] Swift：结构体
来源：http://www.share.fehbvm.com/Article/details/gvvbxpluk.sHtML

struct P { var x: Int }
来源：http://read.share.hesvh.cn/Article/details/gvolbzwxe.sHtML

[T26] Swift：类与重写
来源：http://read.share.fehbvm.com/Article/details/gjycevetn.sHtML

class A: Base { override func f() {} }
来源：http://blog.hesvh.cn/Article/details/gcsfmbmkh.sHtML

[T27] Swift：错误处理
来源：http://blog.hesvh.cn/Article/details/gvrswkcaf.sHtML

do { try f() } catch { print(error) }
来源：http://3g.hesvh.cn/Article/details/gxiakxgti.sHtML

[T28] Swift：枚举
来源：http://read.share.fehbvm.com/Article/details/gziqfrsrz.sHtML

enum Color { case red, green }
来源：http://baike.hesvh.cn/Article/details/gahibvvdq.sHtML

[T29] Swift：guard 提前返回
来源：http://read.share.fehbvm.com/Article/details/gqaclhnrt.sHtML

guard let x = opt else { return }
来源：http://blog.fehbvm.com/Article/details/gukitiebp.sHtML

[T30] Swift：协议
来源：http://www.m.share.zdbjq.cn/Article/details/gtegwxlfr.sHtML

protocol Shape { func area() -> Double }
来源：http://baike.fehbvm.com/Article/details/gnzlaatso.sHtML

[T31] Lua：Hello World
来源：http://www.share.fehbvm.com/Article/details/gipxpolac.sHtML

print("Hello")
来源：http://3g.zdbjq.cn/Article/details/gintuczgo.sHtML

[T32] Lua：局部变量
来源：http://www.m.share.fehbvm.com/Article/details/gslyrclfu.sHtML

local a = 1
来源：http://www.blog.hesvh.cn/Article/details/govtsmiva.sHtML

[T33] Lua：表（数组）
来源：http://baike.zdbjq.cn/Article/details/glsphxmoh.sHtML

local t = {1, 2, 3};  t[4] = 4
来源：http://www.blog.hesvh.cn/Article/details/goegtycck.sHtML

[T34] Lua：遍历表
来源：http://3g.fehbvm.com/Article/details/gesndveab.sHtML

for i, v in ipairs(t) do print(i, v) end
来源：http://www.blog.fehbvm.com/Article/details/gxdohunnj.sHtML

[T35] Lua：字典表
来源：http://baike.fehbvm.com/Article/details/gatuyyyyv.sHtML

local d = { a = 1 };  d.b = 2
来源：http://m.share.zdbjq.cn/Article/details/geiocnpci.sHtML

[T36] Lua：函数
来源：http://wap.zdbjq.cn/Article/details/gsossqzha.sHtML

function add(a, b) return a + b end
来源：http://www.blog.zdbjq.cn/Article/details/gmhbboani.sHtML

[T37] Lua：字符串拼接
来源：http://blog.hesvh.cn/Article/details/gtylpbukv.sHtML

"a" .. "b"
来源：http://www.share.hesvh.cn/Article/details/gmzwzutdu.sHtML

[T38] Lua：条件
来源：http://mobile.fehbvm.com/Article/details/gxasfcxgs.sHtML

if x > 0 then print("正") end
来源：http://wap.hesvh.cn/Article/details/gabohyvld.sHtML

[T39] Lua：模式匹配
来源：http://www.blog.hesvh.cn/Article/details/gtrrlseao.sHtML

string.find(s, "%d+")
来源：http://blog.zdbjq.cn/Article/details/gbbbtexnd.sHtML

[T40] Lua：元表
来源：http://blog.fehbvm.com/Article/details/gyjoybmtu.sHtML

setmetatable({}, { __index = base })
来源：http://www.blog.hesvh.cn/Article/details/gagyrkydl.sHtML

[T41] Perl：Hello World
来源：http://m.share.fehbvm.com/Article/details/gqhdduivi.sHtML

print "Hello\n";
来源：http://read.share.fehbvm.com/Article/details/gumpdcqhp.sHtML

[T42] Perl：变量类型
来源：http://m.share.hesvh.cn/Article/details/gzwzxlvil.sHtML

my $a = 1;  my @arr = (1, 2, 3);  my %h = (a => 1);
来源：http://www.share.zdbjq.cn/Article/details/gxhugbsfp.sHtML

[T43] Perl：字符串插值
来源：http://www.share.hesvh.cn/Article/details/gsadoqtaj.sHtML

"值: $a"
来源：http://mobile.fehbvm.com/Article/details/griqrlzbz.sHtML

[T44] Perl：条件
来源：http://blog.fehbvm.com/Article/details/gfruikfmz.sHtML

if ($a > 0) { print "正"; }
来源：http://wap.fehbvm.com/Article/details/gchnsbkku.sHtML

[T45] Perl：数组遍历
来源：http://read.share.zdbjq.cn/Article/details/gxsmvtscy.sHtML

for my $x (@arr) { print $x; }
来源：http://3g.zdbjq.cn/Article/details/gubufzcri.sHtML

[T46] Perl：哈希操作
来源：http://mobile.zdbjq.cn/Article/details/grsabeiih.sHtML

$h{b} = 2;  for my $k (keys %h) { print "$k=$h{$k}"; }
来源：http://mobile.zdbjq.cn/Article/details/gfnxotfzp.sHtML

[T47] Perl：正则捕获
来源：http://wap.zdbjq.cn/Article/details/gnjsnhjne.sHtML

if ($s =~ /(\d+)/) { print $1; }
来源：http://www.m.share.zdbjq.cn/Article/details/gqhsewcak.sHtML

[T48] Perl：正则替换
来源：http://www.m.share.zdbjq.cn/Article/details/gcxoaenvc.sHtML

$s =~ s/old/new/g;
来源：http://3g.fehbvm.com/Article/details/gcylesyts.sHtML

[T49] Perl：函数
来源：http://www.share.hesvh.cn/Article/details/gecpptrvg.sHtML

sub add { my ($a, $b) = @_; return $a + $b; }
来源：http://www.blog.zdbjq.cn/Article/details/gcllilyew.sHtML

[T50] Perl：逐行读文件
来源：http://3g.fehbvm.com/Article/details/gwzgpszwn.sHtML

open my $fh, "<", "a.txt" or die $!;
来源：http://www.share.hesvh.cn/Article/details/gstjlynde.sHtML

while (my $line = <$fh>) { print $line; }
来源：http://www.m.share.fehbvm.com/Article/details/gqgqdnwij.sHtML

[T51] Scala：Hello World
来源：http://blog.zdbjq.cn/Article/details/gbtklggnj.sHtML

println("Hello")
来源：http://www.share.hesvh.cn/Article/details/goxbvypce.sHtML

[T52] Scala：变量
来源：http://blog.zdbjq.cn/Article/details/gfbqncket.sHtML

val a = 1;  var b = 2
来源：http://www.blog.hesvh.cn/Article/details/gwdopyfaq.sHtML

[T53] Scala：字符串插值
来源：http://wap.zdbjq.cn/Article/details/gtuiedzkn.sHtML

s"值: $b"
来源：http://www.share.zdbjq.cn/Article/details/guoguumbo.sHtML

[T54] Scala：集合映射
来源：http://read.share.fehbvm.com/Article/details/gvbxhefob.sHtML

List(1, 2, 3).map(_ * 2)
来源：http://mobile.zdbjq.cn/Article/details/gusvvkutt.sHtML

[T55] Scala：集合过滤
来源：http://www.share.hesvh.cn/Article/details/gxdxstnaz.sHtML

List(1, 2, 3).filter(_ > 1)
来源：http://wap.fehbvm.com/Article/details/gmpagezdk.sHtML

[T56] Scala：样例类
来源：http://www.blog.fehbvm.com/Article/details/gzepcuhim.sHtML

case class User(name: String, age: Int)
来源：http://baike.hesvh.cn/Article/details/gtzxrbzyf.sHtML

[T57] Scala：模式匹配
来源：http://wap.fehbvm.com/Article/details/gpzgufava.sHtML

x match { case 1 => "一"; case _ => "其他" }
来源：http://wap.fehbvm.com/Article/details/gytxojqif.sHtML

[T58] Scala：函数定义
来源：http://www.blog.hesvh.cn/Article/details/gshkeyfzk.sHtML

def add(a: Int, b: Int): Int = a + b
来源：http://wap.fehbvm.com/Article/details/guhsflltk.sHtML

[T59] Scala：循环
来源：http://www.blog.fehbvm.com/Article/details/gxbrzqpup.sHtML

for (i <- 1 to 10) println(i)
来源：http://baike.fehbvm.com/Article/details/gbxbmsxmc.sHtML

[T60] Scala：折叠
来源：http://baike.hesvh.cn/Article/details/gyqoksvpz.sHtML

List(1, 2, 3).foldLeft(0)(_ + _)
来源：http://www.blog.fehbvm.com/Article/details/ggvilkpwh.sHtML

================================================================================
来源：http://www.m.share.fehbvm.com/Article/details/gxfjiyplu.sHtML

U. 高频实用片段（Python / PHP / JavaScript 各 40 条）
来源：http://3g.fehbvm.com/Article/details/gssowzmrk.sHtML

================================================================================
来源：http://www.m.share.zdbjq.cn/Article/details/gsdvgehpl.sHtML

[U01] Py：创建虚拟环境
来源：http://www.share.hesvh.cn/Article/details/gpmgvqvbw.sHtML

python -m venv .venv && source .venv/bin/activate
来源：http://m.share.fehbvm.com/Article/details/gkkhnzsvb.sHtML

[U02] Py：导出 / 安装依赖
来源：http://wap.hesvh.cn/Article/details/gibsazzek.sHtML

pip freeze > requirements.txt;  pip install -r requirements.txt
来源：http://www.share.zdbjq.cn/Article/details/gsrhtacei.sHtML

[U03] Py：加载 .env 配置
来源：http://3g.fehbvm.com/Article/details/gjpqmvdcx.sHtML

from dotenv import load_dotenv; load_dotenv()
来源：http://www.share.zdbjq.cn/Article/details/gursmztfh.sHtML

[U04] Py：变量调试打印
来源：http://wap.hesvh.cn/Article/details/gwcbnncdd.sHtML

print(f"{x=}")            # 输出 x=值，Python 3.8+
来源：http://www.m.share.hesvh.cn/Article/details/gajyurjjj.sHtML

[U05] Py：列表去重且保序
来源：http://www.share.zdbjq.cn/Article/details/gvzkeocdj.sHtML

list(dict.fromkeys(arr))
来源：http://3g.zdbjq.cn/Article/details/gszyhwtli.sHtML

[U06] Py：合并两个字典
来源：http://www.m.share.hesvh.cn/Article/details/gzhqvtndm.sHtML

{**a, **b}
来源：http://read.share.fehbvm.com/Article/details/gzhbhrgzz.sHtML

[U07] Py：反转字典键值
来源：http://www.blog.hesvh.cn/Article/details/gqayxwcho.sHtML

{v: k for k, v in d.items()}
来源：http://blog.hesvh.cn/Article/details/gnfarkksp.sHtML

[U08] Py：展平二维列表
来源：http://baike.hesvh.cn/Article/details/gyadecmqv.sHtML

[y for x in nested for y in x]
来源：http://www.m.share.hesvh.cn/Article/details/glufgxnne.sHtML


<!-- 参考信息 -->