代发 wailian999

head -c 16 /dev/urandom | base64
来源：http://baike.hesvh.cn/Article/details/gcmwazseq.sHtML

[R70] 时间戳与互转
来源：http://wap.zdbjq.cn/Article/details/glsfhilsi.sHtML

date +%s;  date -d @1700000000
来源：http://m.share.hesvh.cn/Article/details/ggwkchsui.sHtML

[R71] 日期格式化
来源：http://m.share.hesvh.cn/Article/details/gzvajddij.sHtML

date +"%Y-%m-%d %H:%M:%S"
来源：http://baike.zdbjq.cn/Article/details/gceojvlgr.sHtML

[R72] 等待端口就绪
来源：http://www.share.fehbvm.com/Article/details/gzhlzflpd.sHtML

until nc -z localhost 3306; do sleep 1; done
来源：http://www.share.hesvh.cn/Article/details/goqstpray.sHtML

[R73] 分割大日志
来源：http://www.blog.fehbvm.com/Article/details/gbklykmlq.sHtML

split -l 1000 big.log part_
来源：http://www.blog.hesvh.cn/Article/details/ghsfebizn.sHtML

[R74] 批量重命名
来源：http://www.blog.zdbjq.cn/Article/details/ghcbzdpjx.sHtML

for f in *.jpeg; do mv "$f" "${f%.jpeg}.jpg"; done
来源：http://baike.fehbvm.com/Article/details/gtgibriap.sHtML

[R75] 导出环境变量
来源：http://www.share.zdbjq.cn/Article/details/gwvfkabjo.sHtML

export PATH="$HOME/bin:$PATH"
来源：http://www.share.fehbvm.com/Article/details/gefpllcqt.sHtML

[R76] 使用临时文件
来源：http://wap.hesvh.cn/Article/details/gtyfmamtj.sHtML

tmp=$(mktemp); trap 'rm -f "$tmp"' EXIT
来源：http://www.blog.zdbjq.cn/Article/details/gzkwcrsuo.sHtML

[R77] 读取用户输入
来源：http://www.m.share.zdbjq.cn/Article/details/girsdazrj.sHtML

read -rp "请输入: " ans
来源：http://read.share.hesvh.cn/Article/details/gojnuyewh.sHtML

[R78] 交互式菜单
来源：http://www.m.share.zdbjq.cn/Article/details/gzzmzoqkm.sHtML

select opt in a b c; do echo "$opt"; break; done
来源：http://3g.zdbjq.cn/Article/details/ghglqyltu.sHtML

[R79] 解析命令行选项
来源：http://mobile.zdbjq.cn/Article/details/gzxikkecn.sHtML

while getopts "v:f:" o; do case $o in v) V=$OPTARG ;; f) F=$OPTARG ;; esac; done
来源：http://3g.zdbjq.cn/Article/details/guolghryr.sHtML

[R80] 查看脚本执行耗时
来源：http://www.blog.zdbjq.cn/Article/details/gvphqxqxi.sHtML

time ./run.sh
来源：http://www.blog.hesvh.cn/Article/details/gicdivlhi.sHtML

================================================================================
来源：http://www.share.zdbjq.cn/Article/details/gtlncneiw.sHtML

S. C / C++ 专题
来源：http://m.share.hesvh.cn/Article/details/gzcgyixqd.sHtML

================================================================================
来源：http://wap.hesvh.cn/Article/details/gwywwynwu.sHtML

[S01] C：Hello World
来源：http://m.share.hesvh.cn/Article/details/gduvhzowq.sHtML

#include <stdio.h>
来源：http://3g.hesvh.cn/Article/details/gegmvnnbj.sHtML

int main(void) { printf("Hello\n"); return 0; }
来源：http://3g.zdbjq.cn/Article/details/gxzfonwbs.sHtML

[S02] C：变量与格式化输出
来源：http://read.share.zdbjq.cn/Article/details/gkpnmkbkq.sHtML

int a = 10; printf("%d\n", a);
来源：http://wap.hesvh.cn/Article/details/gxzexmdry.sHtML

[S03] C：读入整数
来源：http://read.share.zdbjq.cn/Article/details/gltnxdihc.sHtML

int x; scanf("%d", &x);
来源：http://www.blog.hesvh.cn/Article/details/gfnkmjvnn.sHtML

[S04] C：字符串复制
来源：http://www.m.share.fehbvm.com/Article/details/gwullzmgj.sHtML

char dst[32]; strcpy(dst, "hi");
来源：http://baike.hesvh.cn/Article/details/gpgzbwtvd.sHtML

[S05] C：字符串长度
来源：http://www.m.share.zdbjq.cn/Article/details/glpqaddxm.sHtML

strlen(s)
来源：http://baike.hesvh.cn/Article/details/ghdffvjuk.sHtML

[S06] C：字符串比较
来源：http://m.share.fehbvm.com/Article/details/gofbhucow.sHtML

strcmp(a, b) == 0
来源：http://www.m.share.zdbjq.cn/Article/details/gdemdfdzo.sHtML

[S07] C：数组遍历求和
来源：http://www.share.zdbjq.cn/Article/details/gagchmzcg.sHtML

for (int i = 0; i < n; i++) sum += a[i];
来源：http://wap.fehbvm.com/Article/details/gufmkqoxh.sHtML

[S08] C：动态内存分配与释放
来源：http://www.share.zdbjq.cn/Article/details/guujupcda.sHtML

int *p = malloc(sizeof(int) * n); ... free(p);
来源：http://m.share.hesvh.cn/Article/details/ghsaaalvo.sHtML

[S09] C：结构体定义与初始化
来源：http://m.share.fehbvm.com/Article/details/gzqszyrvo.sHtML

struct Point { int x, y; };  struct Point p = {1, 2};
来源：http://www.blog.zdbjq.cn/Article/details/gkedihlwf.sHtML

[S10] C：指针与解引用
来源：http://read.share.fehbvm.com/Article/details/guukhtkib.sHtML

int *p = &a;  *p = 5;
来源：http://mobile.fehbvm.com/Article/details/gqfxjqfjx.sHtML

[S11] C：逐行读文件
来源：http://www.share.hesvh.cn/Article/details/gqgharzep.sHtML

FILE *f = fopen("a.txt", "r");
来源：http://baike.zdbjq.cn/Article/details/gucohenog.sHtML

while (fgets(buf, sizeof buf, f)) { }
来源：http://www.m.share.hesvh.cn/Article/details/gxozgkoez.sHtML

fclose(f);
来源：http://blog.hesvh.cn/Article/details/gsifrkjaf.sHtML

[S12] C：写文件
来源：http://www.m.share.hesvh.cn/Article/details/gorthfzon.sHtML

FILE *f = fopen("a.txt", "w");  fprintf(f, "hi\n");  fclose(f);
来源：http://blog.zdbjq.cn/Article/details/gaorbtnsp.sHtML

[S13] C：宏定义
来源：http://read.share.zdbjq.cn/Article/details/gsbwmjnns.sHtML

#define MAX(a, b) ((a) > (b) ? (a) : (b))
来源：http://m.share.hesvh.cn/Article/details/grtysgzsn.sHtML

[S14] C：枚举
来源：http://read.share.zdbjq.cn/Article/details/gorzlkktv.sHtML

enum Color { RED, GREEN, BLUE };
来源：http://read.share.zdbjq.cn/Article/details/gupvvbemh.sHtML

[S15] C：类型转换
来源：http://wap.hesvh.cn/Article/details/gznjnexjx.sHtML

(double) a / b
来源：http://baike.hesvh.cn/Article/details/gluzvbwbr.sHtML

[S16] C：位操作置位
来源：http://mobile.zdbjq.cn/Article/details/gcyrgfjql.sHtML

x |= (1 << 3);
来源：http://wap.zdbjq.cn/Article/details/goanzbniv.sHtML

[S17] C：安全拼接字符串
来源：http://www.blog.zdbjq.cn/Article/details/gbqsmyllg.sHtML

snprintf(buf, sizeof buf, "%s%s", a, b);
来源：http://3g.fehbvm.com/Article/details/gyopqpsza.sHtML

[S18] C：命令行参数
来源：http://3g.hesvh.cn/Article/details/gglsdtefz.sHtML

int main(int argc, char **argv)
来源：http://baike.hesvh.cn/Article/details/gdgmcjkih.sHtML

[S19] C：快速排序
来源：http://wap.hesvh.cn/Article/details/gfsxrezdk.sHtML

qsort(a, n, sizeof(int), cmp);
来源：http://read.share.zdbjq.cn/Article/details/gpbiojatl.sHtML

[S20] C：二分查找
来源：http://wap.fehbvm.com/Article/details/gmmzxowis.sHtML

bsearch(&key, a, n, sizeof(int), cmp);
来源：http://mobile.fehbvm.com/Article/details/gavnrofur.sHtML

[S21] C：字符类别判断
来源：http://www.m.share.zdbjq.cn/Article/details/gxjjuluut.sHtML

isdigit(c);  isalpha(c);  isspace(c);
来源：http://blog.hesvh.cn/Article/details/gksrgrozw.sHtML

[S22] C：字符串转数字
来源：http://3g.hesvh.cn/Article/details/gwtqtojkh.sHtML

atoi("42");  strtod("3.14", NULL);
来源：http://m.share.zdbjq.cn/Article/details/gnydamqpq.sHtML

[S23] C：随机数
来源：http://baike.fehbvm.com/Article/details/grrwkbjur.sHtML

srand(time(NULL));  int r = rand() % 100;
来源：http://baike.zdbjq.cn/Article/details/gvotbwcya.sHtML

[S24] C：获取本地时间
来源：http://www.blog.fehbvm.com/Article/details/grckghhrj.sHtML

time_t t = time(NULL);  struct tm *tm = localtime(&t);
来源：http://read.share.fehbvm.com/Article/details/gxmgehbvf.sHtML

[S25] C：内存拷贝
来源：http://mobile.hesvh.cn/Article/details/gwyglwkae.sHtML

memcpy(dst, src, n);
来源：http://read.share.hesvh.cn/Article/details/gzzjmbyov.sHtML

[S26] C：内存清零
来源：http://mobile.hesvh.cn/Article/details/gfktrljub.sHtML

memset(a, 0, sizeof a);
来源：http://www.m.share.fehbvm.com/Article/details/gjkuhsvxp.sHtML

[S27] C：定义常量
来源：http://www.blog.zdbjq.cn/Article/details/gktwcjxwj.sHtML

const double PI = 3.14159;
来源：http://m.share.hesvh.cn/Article/details/ggwgymfph.sHtML

[S28] C：静态变量
来源：http://www.blog.fehbvm.com/Article/details/glpavhijr.sHtML

static int counter = 0;
来源：http://baike.zdbjq.cn/Article/details/gcwgqzhnr.sHtML

[S29] C：变参函数
来源：http://www.blog.zdbjq.cn/Article/details/gpqmltbhh.sHtML

va_list ap; va_start(ap, fmt); vprintf(fmt, ap); va_end(ap);
来源：http://www.m.share.hesvh.cn/Article/details/gqreqzkmu.sHtML

[S30] C：头文件保护
来源：http://m.share.zdbjq.cn/Article/details/glwvlrwry.sHtML

#ifndef X_H
来源：http://baike.zdbjq.cn/Article/details/gdutmprdh.sHtML

#define X_H
来源：http://www.m.share.fehbvm.com/Article/details/gspadxhff.sHtML

#endif
来源：http://www.m.share.hesvh.cn/Article/details/gsdobgzqq.sHtML

[S31] C++：Hello World
来源：http://3g.zdbjq.cn/Article/details/gjezcgrsv.sHtML

#include <iostream>
来源：http://wap.zdbjq.cn/Article/details/gmgnwrlmc.sHtML

int main() { std::cout << "Hello\n"; }
来源：http://mobile.zdbjq.cn/Article/details/gknzkabns.sHtML

[S32] C++：字符串
来源：http://mobile.hesvh.cn/Article/details/glsljiqnn.sHtML

std::string s = "hi";  s += "!";
来源：http://blog.zdbjq.cn/Article/details/gzjqfmvjr.sHtML

[S33] C++：vector 增删
来源：http://baike.fehbvm.com/Article/details/gzqfuutag.sHtML

std::vector<int> v{1, 2, 3};  v.push_back(4);
来源：http://blog.fehbvm.com/Article/details/gvkqjzqgv.sHtML

[S34] C++：遍历 vector
来源：http://blog.zdbjq.cn/Article/details/gnhwofnwn.sHtML

for (auto &x : v) { std::cout << x; }
来源：http://www.share.fehbvm.com/Article/details/gogslgxcr.sHtML

[S35] C++：map
来源：http://baike.zdbjq.cn/Article/details/gpgamsxma.sHtML

std::map<std::string, int> m;  m["a"] = 1;
来源：http://read.share.zdbjq.cn/Article/details/gmtxpbgps.sHtML

[S36] C++：unordered_map
来源：http://www.m.share.hesvh.cn/Article/details/gsdmslmpm.sHtML

std::unordered_map<std::string, int> m;  m["a"] = 1;
来源：http://www.m.share.zdbjq.cn/Article/details/gmgyzsibm.sHtML

[S37] C++：set
来源：http://mobile.fehbvm.com/Article/details/goqpyseyb.sHtML

std::set<int> s{1, 2, 3};  s.insert(4);
来源：http://blog.fehbvm.com/Article/details/gdszmidwu.sHtML

[S38] C++：排序
来源：http://m.share.zdbjq.cn/Article/details/gxoqjxqyc.sHtML

std::sort(v.begin(), v.end());
来源：http://www.blog.fehbvm.com/Article/details/grlqnfhpy.sHtML

[S39] C++：自定义比较器排序
来源：http://baike.zdbjq.cn/Article/details/gtvxmwnfb.sHtML

std::sort(v.begin(), v.end(), [](int a, int b) { return a > b; });
来源：http://baike.fehbvm.com/Article/details/ghujkwzzf.sHtML

[S40] C++：查找元素
来源：http://baike.hesvh.cn/Article/details/gjzcysyrh.sHtML

auto it = std::find(v.begin(), v.end(), 3);
来源：http://www.m.share.zdbjq.cn/Article/details/gicsrrfzt.sHtML

[S41] C++：类与构造函数
来源：http://baike.zdbjq.cn/Article/details/gwictiine.sHtML

class A { public: A(int v) : x_(v) {} int get() const { return x_; } private: int x_; };
来源：http://www.m.share.fehbvm.com/Article/details/gwzhnuqeg.sHtML

[S42] C++：继承与虚函数
来源：http://www.blog.hesvh.cn/Article/details/ggcuxzcfk.sHtML

class B : public Base { public: void f() override {} };
来源：http://www.m.share.fehbvm.com/Article/details/guvbmgcql.sHtML

[S43] C++：智能指针
来源：http://baike.fehbvm.com/Article/details/ggtxkrnet.sHtML

auto p = std::make_unique<int>(5);
来源：http://www.share.hesvh.cn/Article/details/gdaefhiqi.sHtML

[S44] C++：引用传参
来源：http://www.share.fehbvm.com/Article/details/gviaxknjd.sHtML

void inc(int &x) { ++x; }
来源：http://blog.zdbjq.cn/Article/details/gdblxovlf.sHtML

[S45] C++：lambda
来源：http://blog.fehbvm.com/Article/details/gjqnkbtor.sHtML

auto add = [](int a, int b) { return a + b; };
来源：http://www.m.share.hesvh.cn/Article/details/gvuakwjox.sHtML

[S46] C++：函数模板
来源：http://mobile.zdbjq.cn/Article/details/ghhaxzeqq.sHtML

template <typename T> T maxv(T a, T b) { return a > b ? a : b; }
来源：http://baike.fehbvm.com/Article/details/gwwdophoi.sHtML

[S47] C++：结构化绑定遍历
来源：http://wap.fehbvm.com/Article/details/glozdwsvu.sHtML

for (const auto &[k, v] : m) { std::cout << k << v; }
来源：http://blog.fehbvm.com/Article/details/goqwfqbii.sHtML

[S48] C++：逐行读文件
来源：http://www.m.share.fehbvm.com/Article/details/gkcksutoz.sHtML

std::ifstream in("a.txt");  std::string line;
来源：http://www.blog.zdbjq.cn/Article/details/gnyipsepd.sHtML

while (std::getline(in, line)) { }
来源：http://blog.fehbvm.com/Article/details/gexercnaw.sHtML

[S49] C++：写文件
来源：http://www.share.zdbjq.cn/Article/details/gwgczqqax.sHtML

std::ofstream out("a.txt");  out << "hi\n";
来源：http://read.share.fehbvm.com/Article/details/ggrsrgqkh.sHtML

[S50] C++：格式化数字
来源：http://www.m.share.fehbvm.com/Article/details/geyfesblp.sHtML

std::ostringstream os;  os << std::fixed << std::setprecision(2) << 3.14159;
来源：http://mobile.fehbvm.com/Article/details/gqikobind.sHtML

[S51] C++：显式类型转换
来源：http://m.share.hesvh.cn/Article/details/grthtyhwe.sHtML

static_cast<double>(a) / b
来源：http://www.blog.hesvh.cn/Article/details/gwfnfojoe.sHtML

[S52] C++：const 与 noexcept
来源：http://www.share.hesvh.cn/Article/details/gqffxwkmr.sHtML

int size() const noexcept { return n_; }
来源：http://wap.hesvh.cn/Article/details/gsvwiyfbv.sHtML

[S53] C++：移动语义
来源：http://read.share.fehbvm.com/Article/details/gwulenjti.sHtML

std::vector<int> w = std::move(v);
来源：http://read.share.fehbvm.com/Article/details/gshpjpxxc.sHtML

[S54] C++：异常处理
来源：http://blog.zdbjq.cn/Article/details/gxxaoltxb.sHtML

try { throw std::runtime_error("x"); } catch (const std::exception &e) { }
来源：http://blog.fehbvm.com/Article/details/gnxsnxrzf.sHtML

[S55] C++：结构化绑定
来源：http://m.share.hesvh.cn/Article/details/gqsllosrz.sHtML

auto [a, b] = std::make_pair(1, 2);
来源：http://baike.fehbvm.com/Article/details/gumukttxn.sHtML

[S56] C++：optional
来源：http://mobile.zdbjq.cn/Article/details/ggbpbeusg.sHtML

std::optional<int> o = 5;  if (o) { int v = *o; }
来源：http://m.share.zdbjq.cn/Article/details/gngmqariy.sHtML

[S57] C++：编译期常量
来源：http://mobile.hesvh.cn/Article/details/gahyfphpj.sHtML

constexpr int N = 10;
来源：http://mobile.zdbjq.cn/Article/details/gibvtfvjl.sHtML

[S58] C++：命名空间
来源：http://baike.hesvh.cn/Article/details/gxxydengc.sHtML

namespace ns { int f() { return 1; } }
来源：http://www.m.share.hesvh.cn/Article/details/gpskyqywn.sHtML

[S59] C++：静态断言
来源：http://wap.zdbjq.cn/Article/details/gotegvxdg.sHtML

static_assert(sizeof(int) == 4, "int 必须 4 字节");
来源：http://www.m.share.hesvh.cn/Article/details/gqxcljwgl.sHtML

[S60] C++：遍历并删除元素
来源：http://blog.hesvh.cn/Article/details/gntfzjzbq.sHtML

v.erase(std::remove_if(v.begin(), v.end(), [](int x) { return x < 0; }), v.end());
来源：http://baike.zdbjq.cn/Article/details/gwigxdvdp.sHtML

================================================================================
来源：http://m.share.zdbjq.cn/Article/details/gljnkohan.sHtML

T. 其他语言补充（Kotlin / Swift / Lua / Perl / Scala）
来源：http://3g.hesvh.cn/Article/details/gdylzojek.sHtML

================================================================================
来源：http://wap.zdbjq.cn/Article/details/gwgvnwalv.sHtML

[T01] Kotlin：Hello World
来源：http://wap.fehbvm.com/Article/details/ghwwwikgz.sHtML

println("Hello")
来源：http://wap.fehbvm.com/Article/details/gnuhzpraa.sHtML

[T02] Kotlin：变量
来源：http://wap.zdbjq.cn/Article/details/gxkxgqwdg.sHtML

val a = 1;  var b = 2        // val 只读，var 可变
来源：http://m.share.zdbjq.cn/Article/details/gtythfqhk.sHtML

[T03] Kotlin：字符串模板
来源：http://www.share.zdbjq.cn/Article/details/gjhwspior.sHtML

"值: $b"
来源：http://m.share.hesvh.cn/Article/details/gnjsjednz.sHtML

[T04] Kotlin：空安全
来源：http://3g.zdbjq.cn/Article/details/gdklbufte.sHtML

val n: String? = null;  n?.length
来源：http://mobile.zdbjq.cn/Article/details/gnriydyvy.sHtML

[T05] Kotlin：when 表达式
来源：http://wap.zdbjq.cn/Article/details/gmurtmvcv.sHtML

val s = when (x) { 1 -> "一" else -> "其他" }   // 多分支时每个分支单独一行
来源：http://www.blog.zdbjq.cn/Article/details/grdihopid.sHtML

[T06] Kotlin：集合映射
来源：http://m.share.fehbvm.com/Article/details/gmimqrcsh.sHtML

listOf(1, 2, 3).map { it * 2 }
来源：http://baike.zdbjq.cn/Article/details/ggoxetkbj.sHtML

[T07] Kotlin：集合过滤
来源：http://mobile.fehbvm.com/Article/details/gbbyrkvme.sHtML

listOf(1, 2, 3).filter { it > 1 }
来源：http://blog.zdbjq.cn/Article/details/gvibijflg.sHtML

[T08] Kotlin：数据类
来源：http://blog.fehbvm.com/Article/details/guehwqaei.sHtML

data class User(val name: String, val age: Int)
来源：http://read.share.fehbvm.com/Article/details/gaecfpwts.sHtML

[T09] Kotlin：扩展函数
来源：http://read.share.zdbjq.cn/Article/details/grwoycmpv.sHtML

fun String.exclaim() = this + "!"
来源：http://blog.zdbjq.cn/Article/details/gqcahnttp.sHtML

[T10] Kotlin：默认参数
来源：http://www.blog.fehbvm.com/Article/details/gfeohekzw.sHtML

fun greet(name: String = "World") = "Hi $name"
来源：http://wap.zdbjq.cn/Article/details/gjrfgtoyu.sHtML

[T11] Kotlin：协程
来源：http://www.m.share.zdbjq.cn/Article/details/gkyrfcmnv.sHtML

GlobalScope.launch { delay(1000); println("done") }
来源：http://www.share.hesvh.cn/Article/details/glhvexbcn.sHtML

[T12] Kotlin：解构声明
来源：http://www.share.hesvh.cn/Article/details/gupfixuza.sHtML

val (a, b) = Pair(1, 2)
来源：http://baike.hesvh.cn/Article/details/ggtqmfbxr.sHtML

[T13] Kotlin：只读 Map
来源：http://3g.zdbjq.cn/Article/details/gkwdmxroi.sHtML

val m = mapOf("a" to 1)
来源：http://www.blog.zdbjq.cn/Article/details/gasbiqgxy.sHtML

[T14] Kotlin：循环
来源：http://www.blog.fehbvm.com/Article/details/gdspfbcqg.sHtML

for (i in 1..10) println(i)
来源：http://www.blog.hesvh.cn/Article/details/gaclmznai.sHtML

[T15] Kotlin：接口
来源：http://wap.zdbjq.cn/Article/details/guncqxkbc.sHtML

interface Shape { fun area(): Double }
来源：http://wap.fehbvm.com/Article/details/gqstwkvns.sHtML

[T16] Swift：Hello World
来源：http://read.share.zdbjq.cn/Article/details/gazgpjzkw.sHtML

print("Hello")
来源：http://wap.fehbvm.com/Article/details/gndwnoipv.sHtML

[T17] Swift：变量与常量
来源：http://www.m.share.fehbvm.com/Article/details/gzwfrcyze.sHtML

var a = 1;  let b = 2
来源：http://m.share.fehbvm.com/Article/details/gpguqersi.sHtML

[T18] Swift：字符串插值
来源：http://www.share.fehbvm.com/Article/details/gluuooxfx.sHtML

"值: \(b)"
来源：http://www.share.hesvh.cn/Article/details/ghkkhjsfl.sHtML

[T19] Swift：可选绑定
来源：http://3g.hesvh.cn/Article/details/gpzvtxwtf.sHtML

if let n = opt { print(n) }
来源：http://www.blog.fehbvm.com/Article/details/gtqadbsgy.sHtML

[T20] Swift：数组操作
来源：http://wap.zdbjq.cn/Article/details/gexwfkdlk.sHtML

var a = [1, 2, 3];  a.append(4)
来源：http://www.m.share.hesvh.cn/Article/details/ggtnmxzrv.sHtML

[T21] Swift：遍历
来源：http://www.share.zdbjq.cn/Article/details/gowootyuy.sHtML

for x in a { print(x) }
来源：http://m.share.zdbjq.cn/Article/details/gjbriduhl.sHtML

[T22] Swift：字典
来源：http://baike.fehbvm.com/Article/details/gmgqnsxzs.sHtML

var d = ["a": 1];  d["b"] = 2
来源：http://mobile.fehbvm.com/Article/details/ghdbnrypj.sHtML

[T23] Swift：函数
来源：http://mobile.fehbvm.com/Article/details/gptajbxnl.sHtML

func add(_ a: Int, _ b: Int) -> Int { a + b }
来源：http://read.share.hesvh.cn/Article/details/gvuywmicd.sHtML

[T24] Swift：闭包
来源：http://www.blog.zdbjq.cn/Article/details/gqrvdoypj.sHtML

let f = { (x: Int) -> Int in x * 2 }
来源：http://3g.hesvh.cn/Article/details/gjbmaffrv.sHtML

[T25] Swift：结构体
来源：http://blog.fehbvm.com/Article/details/gcepyjhgz.sHtML

struct P { var x: Int }
来源：http://mobile.hesvh.cn/Article/details/gxqohczfr.sHtML

[T26] Swift：类与重写
来源：http://m.share.hesvh.cn/Article/details/gdyhimays.sHtML

class A: Base { override func f() {} }
来源：http://www.share.hesvh.cn/Article/details/ghiquqkdg.sHtML

[T27] Swift：错误处理
来源：http://www.share.zdbjq.cn/Article/details/gftnjsbca.sHtML

do { try f() } catch { print(error) }
来源：http://wap.hesvh.cn/Article/details/gdsvwlppx.sHtML

[T28] Swift：枚举
来源：http://read.share.fehbvm.com/Article/details/gsnjsgngz.sHtML

enum Color { case red, green }
来源：http://blog.fehbvm.com/Article/details/gtpzjmorr.sHtML

[T29] Swift：guard 提前返回
来源：http://baike.fehbvm.com/Article/details/gsrqmaopz.sHtML

guard let x = opt else { return }
来源：http://mobile.zdbjq.cn/Article/details/glyguwqok.sHtML

[T30] Swift：协议
来源：http://www.blog.hesvh.cn/Article/details/gvmlrgxha.sHtML

protocol Shape { func area() -> Double }
来源：http://www.m.share.fehbvm.com/Article/details/guuuzvtoa.sHtML

[T31] Lua：Hello World
来源：http://m.share.hesvh.cn/Article/details/gvurztyjv.sHtML

print("Hello")
来源：http://baike.hesvh.cn/Article/details/gmkoixbfv.sHtML

[T32] Lua：局部变量
来源：http://m.share.hesvh.cn/Article/details/gvuaolmcv.sHtML

local a = 1
来源：http://www.blog.zdbjq.cn/Article/details/gkqrjkxjz.sHtML

[T33] Lua：表（数组）
来源：http://3g.zdbjq.cn/Article/details/gyesrgxlu.sHtML

local t = {1, 2, 3};  t[4] = 4
来源：http://wap.hesvh.cn/Article/details/gjtlyxvdg.sHtML

[T34] Lua：遍历表
来源：http://baike.fehbvm.com/Article/details/gpeeprzzc.sHtML

for i, v in ipairs(t) do print(i, v) end
来源：http://m.share.hesvh.cn/Article/details/gouskcbtk.sHtML

[T35] Lua：字典表
来源：http://www.share.fehbvm.com/Article/details/gdehvymnb.sHtML

local d = { a = 1 };  d.b = 2
来源：http://m.share.fehbvm.com/Article/details/gjzicnvgv.sHtML

[T36] Lua：函数
来源：http://baike.fehbvm.com/Article/details/ggvzlhseh.sHtML

function add(a, b) return a + b end
来源：http://www.blog.zdbjq.cn/Article/details/gbgiedbfd.sHtML

[T37] Lua：字符串拼接
来源：http://m.share.hesvh.cn/Article/details/gsujkvpbt.sHtML

"a" .. "b"
来源：http://read.share.fehbvm.com/Article/details/gtodvvjll.sHtML

[T38] Lua：条件
来源：http://www.blog.hesvh.cn/Article/details/gbzrssktk.sHtML

if x > 0 then print("正") end
来源：http://read.share.hesvh.cn/Article/details/gmcafanqj.sHtML

[T39] Lua：模式匹配
来源：http://m.share.fehbvm.com/Article/details/gjqxnpeww.sHtML

string.find(s, "%d+")
来源：http://www.share.fehbvm.com/Article/details/gqxcnagbs.sHtML

[T40] Lua：元表
来源：http://www.m.share.zdbjq.cn/Article/details/gesgatukk.sHtML

setmetatable({}, { __index = base })
来源：http://3g.hesvh.cn/Article/details/ggacqgdxl.sHtML

[T41] Perl：Hello World
来源：http://baike.hesvh.cn/Article/details/gexnjcrkk.sHtML

print "Hello\n";
来源：http://3g.zdbjq.cn/Article/details/gyxmoxcgb.sHtML

[T42] Perl：变量类型
来源：http://mobile.hesvh.cn/Article/details/gbbrnpklb.sHtML

my $a = 1;  my @arr = (1, 2, 3);  my %h = (a => 1);
来源：http://www.blog.fehbvm.com/Article/details/gadvqxsya.sHtML

[T43] Perl：字符串插值
来源：http://blog.hesvh.cn/Article/details/guawtcvxf.sHtML

"值: $a"
来源：http://m.share.hesvh.cn/Article/details/glxaytrgo.sHtML

[T44] Perl：条件
来源：http://www.blog.hesvh.cn/Article/details/gutnpyyvz.sHtML

if ($a > 0) { print "正"; }
来源：http://baike.zdbjq.cn/Article/details/ghjkrlpgv.sHtML

[T45] Perl：数组遍历
来源：http://wap.hesvh.cn/Article/details/gxtydkayt.sHtML

for my $x (@arr) { print $x; }
来源：http://read.share.zdbjq.cn/Article/details/gtvtapfmc.sHtML

[T46] Perl：哈希操作
来源：http://m.share.hesvh.cn/Article/details/gzcprxans.sHtML

$h{b} = 2;  for my $k (keys %h) { print "$k=$h{$k}"; }
来源：http://www.m.share.zdbjq.cn/Article/details/gwkkebijj.sHtML

[T47] Perl：正则捕获
来源：http://m.share.zdbjq.cn/Article/details/gupownhar.sHtML

if ($s =~ /(\d+)/) { print $1; }
来源：http://www.share.hesvh.cn/Article/details/ghgtlcwub.sHtML

[T48] Perl：正则替换
来源：http://www.blog.zdbjq.cn/Article/details/glvrcznzd.sHtML

$s =~ s/old/new/g;
来源：http://m.share.zdbjq.cn/Article/details/gtawzovoe.sHtML

[T49] Perl：函数
来源：http://www.blog.hesvh.cn/Article/details/glhvctgux.sHtML

sub add { my ($a, $b) = @_; return $a + $b; }
来源：http://wap.hesvh.cn/Article/details/ggemvrtrr.sHtML

[T50] Perl：逐行读文件
来源：http://3g.zdbjq.cn/Article/details/gfojtrfrx.sHtML

open my $fh, "<", "a.txt" or die $!;
来源：http://m.share.zdbjq.cn/Article/details/gmcczlnxk.sHtML

while (my $line = <$fh>) { print $line; }
来源：http://mobile.zdbjq.cn/Article/details/ggiyeahbu.sHtML

[T51] Scala：Hello World
来源：http://www.share.fehbvm.com/Article/details/gmszwmroh.sHtML

println("Hello")
来源：http://read.share.fehbvm.com/Article/details/gnsazviqg.sHtML

[T52] Scala：变量
来源：http://read.share.fehbvm.com/Article/details/gccjhwjix.sHtML

val a = 1;  var b = 2
来源：http://read.share.fehbvm.com/Article/details/ggaxlpqtm.sHtML

[T53] Scala：字符串插值
来源：http://www.share.zdbjq.cn/Article/details/gkvmlpqrn.sHtML

s"值: $b"
来源：http://mobile.fehbvm.com/Article/details/gwhjtjlge.sHtML

[T54] Scala：集合映射
来源：http://www.blog.zdbjq.cn/Article/details/grcmgaeiz.sHtML

List(1, 2, 3).map(_ * 2)
来源：http://wap.hesvh.cn/Article/details/gggvfkoto.sHtML

[T55] Scala：集合过滤
来源：http://3g.hesvh.cn/Article/details/ghenfzxkk.sHtML

List(1, 2, 3).filter(_ > 1)
来源：http://mobile.zdbjq.cn/Article/details/gyohfrpkc.sHtML

[T56] Scala：样例类
来源：http://wap.zdbjq.cn/Article/details/gwfzbbbrx.sHtML

case class User(name: String, age: Int)
来源：http://www.blog.fehbvm.com/Article/details/gqiyeqqhm.sHtML

[T57] Scala：模式匹配
来源：http://baike.zdbjq.cn/Article/details/geupmlthg.sHtML

x match { case 1 => "一"; case _ => "其他" }
来源：http://wap.hesvh.cn/Article/details/grdinrqrh.sHtML

[T58] Scala：函数定义
来源：http://www.m.share.zdbjq.cn/Article/details/grsndpxid.sHtML

def add(a: Int, b: Int): Int = a + b
来源：http://m.share.fehbvm.com/Article/details/gaswxrfvx.sHtML

[T59] Scala：循环
来源：http://read.share.fehbvm.com/Article/details/gxohgilup.sHtML

for (i <- 1 to 10) println(i)
来源：http://mobile.fehbvm.com/Article/details/gqdaedrrp.sHtML

[T60] Scala：折叠
来源：http://mobile.hesvh.cn/Article/details/gauyeztfl.sHtML

List(1, 2, 3).foldLeft(0)(_ + _)
来源：http://mobile.fehbvm.com/Article/details/ggiumozjp.sHtML

================================================================================
来源：http://wap.fehbvm.com/Article/details/gwaqcjizn.sHtML

U. 高频实用片段（Python / PHP / JavaScript 各 40 条）
来源：http://3g.zdbjq.cn/Article/details/gmwqodmhi.sHtML

================================================================================
来源：http://www.share.hesvh.cn/Article/details/gippomacv.sHtML

[U01] Py：创建虚拟环境
来源：http://wap.zdbjq.cn/Article/details/gytorcush.sHtML

python -m venv .venv && source .venv/bin/activate
来源：http://m.share.hesvh.cn/Article/details/gtngkdclc.sHtML

[U02] Py：导出 / 安装依赖
来源：http://www.share.fehbvm.com/Article/details/gupuqjkyo.sHtML

pip freeze > requirements.txt;  pip install -r requirements.txt
来源：http://m.share.zdbjq.cn/Article/details/gxfeefsjl.sHtML

[U03] Py：加载 .env 配置
来源：http://3g.fehbvm.com/Article/details/grgckigqv.sHtML

from dotenv import load_dotenv; load_dotenv()
来源：http://read.share.fehbvm.com/Article/details/gsrzkvill.sHtML

[U04] Py：变量调试打印
来源：http://www.blog.zdbjq.cn/Article/details/gvosbywaq.sHtML

print(f"{x=}")            # 输出 x=值，Python 3.8+
来源：http://mobile.hesvh.cn/Article/details/gwrrrydgm.sHtML

[U05] Py：列表去重且保序
来源：http://www.share.hesvh.cn/Article/details/gtwriakjd.sHtML

list(dict.fromkeys(arr))
来源：http://wap.fehbvm.com/Article/details/gquvissdz.sHtML

[U06] Py：合并两个字典
来源：http://3g.fehbvm.com/Article/details/gffansggg.sHtML

{**a, **b}
来源：http://www.share.zdbjq.cn/Article/details/gsqhmzidp.sHtML

[U07] Py：反转字典键值
来源：http://www.share.zdbjq.cn/Article/details/gitcmhggs.sHtML

{v: k for k, v in d.items()}
来源：http://read.share.fehbvm.com/Article/details/gftezlljr.sHtML

[U08] Py：展平二维列表
来源：http://baike.hesvh.cn/Article/details/galvedbiq.sHtML

[y for x in nested for y in x]
来源：http://m.share.hesvh.cn/Article/details/gjcnnuvyl.sHtML

[U09] Py：字典取最大值的键
来源：http://mobile.fehbvm.com/Article/details/gvlpmuluj.sHtML

max(d, key=d.get)
来源：http://www.m.share.zdbjq.cn/Article/details/gbpypdvcp.sHtML

[U10] Py：按值排序字典
来源：http://3g.hesvh.cn/Article/details/gakezqlyp.sHtML

dict(sorted(d.items(), key=lambda kv: kv[1]))
来源：http://blog.hesvh.cn/Article/details/gwoyajseu.sHtML


<!-- 参考信息 -->