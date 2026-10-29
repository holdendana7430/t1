代发 wailian999

openssl rand -hex 16
来源：http://www.share.hesvh.cn/Article/details/gkprwlboo.sHtML

[R68] 计算文件校验值
来源：http://baike.fehbvm.com/Article/details/giaucodze.sHtML

sha256sum a.txt;  md5sum a.txt
来源：http://baike.fehbvm.com/Article/details/grmkvbate.sHtML

[R69] 生成随机密码
来源：http://www.blog.zdbjq.cn/Article/details/gcvlohuea.sHtML

head -c 16 /dev/urandom | base64
来源：http://blog.hesvh.cn/Article/details/gckecudvb.sHtML

[R70] 时间戳与互转
来源：http://3g.zdbjq.cn/Article/details/gciylvswz.sHtML

date +%s;  date -d @1700000000
来源：http://www.m.share.zdbjq.cn/Article/details/gbvmzrayn.sHtML

[R71] 日期格式化
来源：http://www.blog.fehbvm.com/Article/details/gsxdpnkrs.sHtML

date +"%Y-%m-%d %H:%M:%S"
来源：http://blog.fehbvm.com/Article/details/gapqiigrx.sHtML

[R72] 等待端口就绪
来源：http://mobile.zdbjq.cn/Article/details/gbmloethi.sHtML

until nc -z localhost 3306; do sleep 1; done
来源：http://www.m.share.fehbvm.com/Article/details/ghujeqxys.sHtML

[R73] 分割大日志
来源：http://blog.fehbvm.com/Article/details/gfqdyudwr.sHtML

split -l 1000 big.log part_
来源：http://read.share.zdbjq.cn/Article/details/gjkgsfzcr.sHtML

[R74] 批量重命名
来源：http://baike.zdbjq.cn/Article/details/gvbozhfal.sHtML

for f in *.jpeg; do mv "$f" "${f%.jpeg}.jpg"; done
来源：http://mobile.zdbjq.cn/Article/details/gyutlljlj.sHtML

[R75] 导出环境变量
来源：http://www.blog.fehbvm.com/Article/details/ggokirmpd.sHtML

export PATH="$HOME/bin:$PATH"
来源：http://www.blog.zdbjq.cn/Article/details/gtzifevoh.sHtML

[R76] 使用临时文件
来源：http://blog.fehbvm.com/Article/details/gzxpaemop.sHtML

tmp=$(mktemp); trap 'rm -f "$tmp"' EXIT
来源：http://3g.hesvh.cn/Article/details/gacawxrvx.sHtML

[R77] 读取用户输入
来源：http://m.share.hesvh.cn/Article/details/gulrgtcww.sHtML

read -rp "请输入: " ans
来源：http://www.share.zdbjq.cn/Article/details/gkqozzfdd.sHtML

[R78] 交互式菜单
来源：http://baike.fehbvm.com/Article/details/gwekidchx.sHtML

select opt in a b c; do echo "$opt"; break; done
来源：http://mobile.zdbjq.cn/Article/details/ghddpyngn.sHtML

[R79] 解析命令行选项
来源：http://mobile.hesvh.cn/Article/details/gkozceojc.sHtML

while getopts "v:f:" o; do case $o in v) V=$OPTARG ;; f) F=$OPTARG ;; esac; done
来源：http://m.share.zdbjq.cn/Article/details/gcisawuzv.sHtML

[R80] 查看脚本执行耗时
来源：http://read.share.fehbvm.com/Article/details/gxmcaahhh.sHtML

time ./run.sh
来源：http://www.blog.zdbjq.cn/Article/details/gohflijjq.sHtML

================================================================================
来源：http://wap.hesvh.cn/Article/details/gjivshfit.sHtML

S. C / C++ 专题
来源：http://m.share.fehbvm.com/Article/details/gbfpbqmqb.sHtML

================================================================================
来源：http://www.share.fehbvm.com/Article/details/gptdlztoe.sHtML

[S01] C：Hello World
来源：http://www.share.hesvh.cn/Article/details/gxikbucqw.sHtML

#include <stdio.h>
来源：http://www.m.share.zdbjq.cn/Article/details/gujmncfha.sHtML

int main(void) { printf("Hello\n"); return 0; }
来源：http://read.share.hesvh.cn/Article/details/gcxgzrhhd.sHtML

[S02] C：变量与格式化输出
来源：http://read.share.hesvh.cn/Article/details/gbnvtjiob.sHtML

int a = 10; printf("%d\n", a);
来源：http://wap.zdbjq.cn/Article/details/gpmedxcak.sHtML

[S03] C：读入整数
来源：http://3g.zdbjq.cn/Article/details/gsrwbtqdr.sHtML

int x; scanf("%d", &x);
来源：http://3g.hesvh.cn/Article/details/gisfrhynw.sHtML

[S04] C：字符串复制
来源：http://www.share.fehbvm.com/Article/details/gnxsdoivo.sHtML

char dst[32]; strcpy(dst, "hi");
来源：http://www.blog.hesvh.cn/Article/details/geghegpcj.sHtML

[S05] C：字符串长度
来源：http://mobile.zdbjq.cn/Article/details/grklgznwy.sHtML

strlen(s)
来源：http://3g.fehbvm.com/Article/details/gnqtbczxc.sHtML

[S06] C：字符串比较
来源：http://baike.zdbjq.cn/Article/details/griyivamr.sHtML

strcmp(a, b) == 0
来源：http://www.share.zdbjq.cn/Article/details/ghpyiftfw.sHtML

[S07] C：数组遍历求和
来源：http://baike.zdbjq.cn/Article/details/gktaapefc.sHtML

for (int i = 0; i < n; i++) sum += a[i];
来源：http://wap.fehbvm.com/Article/details/glwejyvuw.sHtML

[S08] C：动态内存分配与释放
来源：http://www.share.zdbjq.cn/Article/details/gingcxswv.sHtML

int *p = malloc(sizeof(int) * n); ... free(p);
来源：http://www.m.share.zdbjq.cn/Article/details/gtjnshjhb.sHtML

[S09] C：结构体定义与初始化
来源：http://mobile.hesvh.cn/Article/details/gbxastvqd.sHtML

struct Point { int x, y; };  struct Point p = {1, 2};
来源：http://read.share.hesvh.cn/Article/details/gojthgvyj.sHtML

[S10] C：指针与解引用
来源：http://blog.fehbvm.com/Article/details/gjqxlabrh.sHtML

int *p = &a;  *p = 5;
来源：http://www.m.share.zdbjq.cn/Article/details/gmijbdhbx.sHtML

[S11] C：逐行读文件
来源：http://mobile.zdbjq.cn/Article/details/gjadecxky.sHtML

FILE *f = fopen("a.txt", "r");
来源：http://mobile.fehbvm.com/Article/details/geyznbrgr.sHtML

while (fgets(buf, sizeof buf, f)) { }
来源：http://wap.hesvh.cn/Article/details/gbvwgqzmv.sHtML

fclose(f);
来源：http://blog.zdbjq.cn/Article/details/gqwtxcuhl.sHtML

[S12] C：写文件
来源：http://baike.zdbjq.cn/Article/details/gcjgtgtjh.sHtML

FILE *f = fopen("a.txt", "w");  fprintf(f, "hi\n");  fclose(f);
来源：http://wap.zdbjq.cn/Article/details/ghgfdiiqv.sHtML

[S13] C：宏定义
来源：http://read.share.hesvh.cn/Article/details/gqyllifgz.sHtML

#define MAX(a, b) ((a) > (b) ? (a) : (b))
来源：http://blog.hesvh.cn/Article/details/gzaswfrwd.sHtML

[S14] C：枚举
来源：http://blog.zdbjq.cn/Article/details/ghsuecviu.sHtML

enum Color { RED, GREEN, BLUE };
来源：http://www.share.fehbvm.com/Article/details/gqmyrspjo.sHtML

[S15] C：类型转换
来源：http://m.share.zdbjq.cn/Article/details/gfuggxsbg.sHtML

(double) a / b
来源：http://read.share.hesvh.cn/Article/details/gqcugsioe.sHtML

[S16] C：位操作置位
来源：http://www.m.share.zdbjq.cn/Article/details/gikhrcdvd.sHtML

x |= (1 << 3);
来源：http://mobile.hesvh.cn/Article/details/gqwduqnzm.sHtML

[S17] C：安全拼接字符串
来源：http://baike.fehbvm.com/Article/details/gxqsddmjn.sHtML

snprintf(buf, sizeof buf, "%s%s", a, b);
来源：http://read.share.fehbvm.com/Article/details/gdmpqjxtj.sHtML

[S18] C：命令行参数
来源：http://blog.zdbjq.cn/Article/details/gfszathwe.sHtML

int main(int argc, char **argv)
来源：http://www.share.zdbjq.cn/Article/details/gwslfafzr.sHtML

[S19] C：快速排序
来源：http://m.share.hesvh.cn/Article/details/gnqcvyina.sHtML

qsort(a, n, sizeof(int), cmp);
来源：http://mobile.hesvh.cn/Article/details/gisbabkch.sHtML

[S20] C：二分查找
来源：http://mobile.hesvh.cn/Article/details/gknohybkz.sHtML

bsearch(&key, a, n, sizeof(int), cmp);
来源：http://blog.hesvh.cn/Article/details/gtykaolkz.sHtML

[S21] C：字符类别判断
来源：http://3g.fehbvm.com/Article/details/gqhfrqhvc.sHtML

isdigit(c);  isalpha(c);  isspace(c);
来源：http://blog.zdbjq.cn/Article/details/gfbepfoab.sHtML

[S22] C：字符串转数字
来源：http://read.share.zdbjq.cn/Article/details/guszitsyn.sHtML

atoi("42");  strtod("3.14", NULL);
来源：http://blog.zdbjq.cn/Article/details/gdioaxade.sHtML

[S23] C：随机数
来源：http://mobile.fehbvm.com/Article/details/gkxzoicdl.sHtML

srand(time(NULL));  int r = rand() % 100;
来源：http://read.share.zdbjq.cn/Article/details/gnyogbviv.sHtML

[S24] C：获取本地时间
来源：http://3g.hesvh.cn/Article/details/gqoypzybz.sHtML

time_t t = time(NULL);  struct tm *tm = localtime(&t);
来源：http://3g.zdbjq.cn/Article/details/gwmjosfwu.sHtML

[S25] C：内存拷贝
来源：http://mobile.zdbjq.cn/Article/details/ggeiayavo.sHtML

memcpy(dst, src, n);
来源：http://m.share.fehbvm.com/Article/details/gngejhlyz.sHtML

[S26] C：内存清零
来源：http://mobile.fehbvm.com/Article/details/gbfrcomlf.sHtML

memset(a, 0, sizeof a);
来源：http://3g.hesvh.cn/Article/details/glvmnizdh.sHtML

[S27] C：定义常量
来源：http://www.m.share.zdbjq.cn/Article/details/gtroabspm.sHtML

const double PI = 3.14159;
来源：http://www.blog.fehbvm.com/Article/details/glozspbvb.sHtML

[S28] C：静态变量
来源：http://blog.fehbvm.com/Article/details/gwiwqedog.sHtML

static int counter = 0;
来源：http://blog.zdbjq.cn/Article/details/glcygbwri.sHtML

[S29] C：变参函数
来源：http://3g.fehbvm.com/Article/details/gdwygdqtr.sHtML

va_list ap; va_start(ap, fmt); vprintf(fmt, ap); va_end(ap);
来源：http://3g.fehbvm.com/Article/details/gbcrgyuzo.sHtML

[S30] C：头文件保护
来源：http://www.m.share.fehbvm.com/Article/details/gtrhvyeon.sHtML

#ifndef X_H
来源：http://blog.zdbjq.cn/Article/details/ghfjumzpn.sHtML

#define X_H
来源：http://m.share.hesvh.cn/Article/details/gkeiplfxs.sHtML

#endif
来源：http://www.blog.fehbvm.com/Article/details/gdeyezyut.sHtML

[S31] C++：Hello World
来源：http://read.share.hesvh.cn/Article/details/grkbbxhij.sHtML

#include <iostream>
来源：http://baike.hesvh.cn/Article/details/gytbhggnb.sHtML

int main() { std::cout << "Hello\n"; }
来源：http://wap.fehbvm.com/Article/details/gpxyynjgi.sHtML

[S32] C++：字符串
来源：http://read.share.zdbjq.cn/Article/details/ghskvvwru.sHtML

std::string s = "hi";  s += "!";
来源：http://www.m.share.fehbvm.com/Article/details/ghajgtfvo.sHtML

[S33] C++：vector 增删
来源：http://www.blog.hesvh.cn/Article/details/gwmexlzpd.sHtML

std::vector<int> v{1, 2, 3};  v.push_back(4);
来源：http://m.share.zdbjq.cn/Article/details/gqzejtlfn.sHtML

[S34] C++：遍历 vector
来源：http://3g.hesvh.cn/Article/details/gmqkflppe.sHtML

for (auto &x : v) { std::cout << x; }
来源：http://3g.fehbvm.com/Article/details/gmohbxiuj.sHtML

[S35] C++：map
来源：http://www.blog.hesvh.cn/Article/details/gdioomdrv.sHtML

std::map<std::string, int> m;  m["a"] = 1;
来源：http://blog.fehbvm.com/Article/details/gglhpbmht.sHtML

[S36] C++：unordered_map
来源：http://www.m.share.fehbvm.com/Article/details/gxvesqlon.sHtML

std::unordered_map<std::string, int> m;  m["a"] = 1;
来源：http://read.share.hesvh.cn/Article/details/gsmehniuo.sHtML

[S37] C++：set
来源：http://wap.zdbjq.cn/Article/details/gyisldeyw.sHtML

std::set<int> s{1, 2, 3};  s.insert(4);
来源：http://wap.hesvh.cn/Article/details/gwglbtqym.sHtML

[S38] C++：排序
来源：http://baike.fehbvm.com/Article/details/gbcnbvuhf.sHtML

std::sort(v.begin(), v.end());
来源：http://baike.zdbjq.cn/Article/details/gdnkhttkt.sHtML

[S39] C++：自定义比较器排序
来源：http://m.share.fehbvm.com/Article/details/gtschzplw.sHtML

std::sort(v.begin(), v.end(), [](int a, int b) { return a > b; });
来源：http://read.share.hesvh.cn/Article/details/gsyeaosvt.sHtML

[S40] C++：查找元素
来源：http://3g.zdbjq.cn/Article/details/gqlxheavt.sHtML

auto it = std::find(v.begin(), v.end(), 3);
来源：http://3g.hesvh.cn/Article/details/gugwhdgir.sHtML

[S41] C++：类与构造函数
来源：http://mobile.fehbvm.com/Article/details/gkcsfxhof.sHtML

class A { public: A(int v) : x_(v) {} int get() const { return x_; } private: int x_; };
来源：http://read.share.fehbvm.com/Article/details/gybispuxc.sHtML

[S42] C++：继承与虚函数
来源：http://blog.hesvh.cn/Article/details/gexhobcvx.sHtML

class B : public Base { public: void f() override {} };
来源：http://baike.hesvh.cn/Article/details/guzbtkqrz.sHtML

[S43] C++：智能指针
来源：http://www.m.share.zdbjq.cn/Article/details/gqptervmc.sHtML

auto p = std::make_unique<int>(5);
来源：http://www.blog.hesvh.cn/Article/details/gmwsnlhxt.sHtML

[S44] C++：引用传参
来源：http://baike.hesvh.cn/Article/details/giphovujf.sHtML

void inc(int &x) { ++x; }
来源：http://www.share.fehbvm.com/Article/details/gzjehhszp.sHtML

[S45] C++：lambda
来源：http://www.blog.zdbjq.cn/Article/details/guzwvwmkd.sHtML

auto add = [](int a, int b) { return a + b; };
来源：http://mobile.zdbjq.cn/Article/details/gykinkeol.sHtML

[S46] C++：函数模板
来源：http://www.blog.zdbjq.cn/Article/details/gtoxytltp.sHtML

template <typename T> T maxv(T a, T b) { return a > b ? a : b; }
来源：http://baike.hesvh.cn/Article/details/gsvgjsmgd.sHtML

[S47] C++：结构化绑定遍历
来源：http://baike.hesvh.cn/Article/details/gqfsajmew.sHtML

for (const auto &[k, v] : m) { std::cout << k << v; }
来源：http://mobile.zdbjq.cn/Article/details/gnymilgwo.sHtML

[S48] C++：逐行读文件
来源：http://read.share.hesvh.cn/Article/details/gkbwqbeyp.sHtML

std::ifstream in("a.txt");  std::string line;
来源：http://www.m.share.fehbvm.com/Article/details/gbzcktbzq.sHtML

while (std::getline(in, line)) { }
来源：http://blog.fehbvm.com/Article/details/gmzrhzaum.sHtML

[S49] C++：写文件
来源：http://www.blog.zdbjq.cn/Article/details/gqzpogbtv.sHtML

std::ofstream out("a.txt");  out << "hi\n";
来源：http://baike.hesvh.cn/Article/details/ginyiupyh.sHtML

[S50] C++：格式化数字
来源：http://baike.fehbvm.com/Article/details/gxghlnfgt.sHtML

std::ostringstream os;  os << std::fixed << std::setprecision(2) << 3.14159;
来源：http://www.share.zdbjq.cn/Article/details/giqnhpeka.sHtML

[S51] C++：显式类型转换
来源：http://mobile.fehbvm.com/Article/details/gyawtlrnq.sHtML

static_cast<double>(a) / b
来源：http://www.share.hesvh.cn/Article/details/glqhoceoh.sHtML

[S52] C++：const 与 noexcept
来源：http://read.share.hesvh.cn/Article/details/gryhynnef.sHtML

int size() const noexcept { return n_; }
来源：http://www.blog.fehbvm.com/Article/details/gdxrispti.sHtML

[S53] C++：移动语义
来源：http://m.share.fehbvm.com/Article/details/gwjseqskk.sHtML

std::vector<int> w = std::move(v);
来源：http://blog.hesvh.cn/Article/details/gixbbylou.sHtML

[S54] C++：异常处理
来源：http://baike.zdbjq.cn/Article/details/gnjyeafpt.sHtML

try { throw std::runtime_error("x"); } catch (const std::exception &e) { }
来源：http://read.share.fehbvm.com/Article/details/grngzvidy.sHtML

[S55] C++：结构化绑定
来源：http://baike.zdbjq.cn/Article/details/gojbjjxdk.sHtML

auto [a, b] = std::make_pair(1, 2);
来源：http://www.share.fehbvm.com/Article/details/gfhsqembf.sHtML

[S56] C++：optional
来源：http://www.m.share.zdbjq.cn/Article/details/gaboumywj.sHtML

std::optional<int> o = 5;  if (o) { int v = *o; }
来源：http://www.share.fehbvm.com/Article/details/gexsolkzl.sHtML

[S57] C++：编译期常量
来源：http://blog.zdbjq.cn/Article/details/gfvlptdpr.sHtML

constexpr int N = 10;
来源：http://m.share.zdbjq.cn/Article/details/gndbxfhuz.sHtML

[S58] C++：命名空间
来源：http://blog.hesvh.cn/Article/details/gqydrhhnm.sHtML

namespace ns { int f() { return 1; } }
来源：http://www.blog.hesvh.cn/Article/details/gdxlxcixt.sHtML

[S59] C++：静态断言
来源：http://www.blog.zdbjq.cn/Article/details/gefmhewax.sHtML

static_assert(sizeof(int) == 4, "int 必须 4 字节");
来源：http://www.m.share.fehbvm.com/Article/details/grawbsemc.sHtML

[S60] C++：遍历并删除元素
来源：http://www.share.zdbjq.cn/Article/details/gcnviyauk.sHtML

v.erase(std::remove_if(v.begin(), v.end(), [](int x) { return x < 0; }), v.end());
来源：http://baike.fehbvm.com/Article/details/gfbwghweo.sHtML

================================================================================
来源：http://blog.hesvh.cn/Article/details/gorxlcaqy.sHtML

T. 其他语言补充（Kotlin / Swift / Lua / Perl / Scala）
来源：http://baike.zdbjq.cn/Article/details/ggvwbpcqs.sHtML

================================================================================
来源：http://www.m.share.zdbjq.cn/Article/details/glpsyztqk.sHtML

[T01] Kotlin：Hello World
来源：http://wap.fehbvm.com/Article/details/gepgryqxm.sHtML

println("Hello")
来源：http://mobile.fehbvm.com/Article/details/govxzmddo.sHtML

[T02] Kotlin：变量
来源：http://mobile.zdbjq.cn/Article/details/gfwmuskjy.sHtML

val a = 1;  var b = 2        // val 只读，var 可变
来源：http://3g.fehbvm.com/Article/details/gwtgotiyq.sHtML

[T03] Kotlin：字符串模板
来源：http://mobile.fehbvm.com/Article/details/giezmqbch.sHtML

"值: $b"
来源：http://www.m.share.fehbvm.com/Article/details/gjyebxkfl.sHtML

[T04] Kotlin：空安全
来源：http://mobile.zdbjq.cn/Article/details/gfdxbivcj.sHtML

val n: String? = null;  n?.length
来源：http://mobile.fehbvm.com/Article/details/gvtsehhwv.sHtML

[T05] Kotlin：when 表达式
来源：http://www.blog.zdbjq.cn/Article/details/gszdzqgja.sHtML

val s = when (x) { 1 -> "一" else -> "其他" }   // 多分支时每个分支单独一行
来源：http://mobile.zdbjq.cn/Article/details/gtxxmevns.sHtML

[T06] Kotlin：集合映射
来源：http://3g.zdbjq.cn/Article/details/grwvfvavw.sHtML

listOf(1, 2, 3).map { it * 2 }
来源：http://www.blog.hesvh.cn/Article/details/gcbvxyfpw.sHtML

[T07] Kotlin：集合过滤
来源：http://www.blog.fehbvm.com/Article/details/ghczsrtun.sHtML

listOf(1, 2, 3).filter { it > 1 }
来源：http://blog.hesvh.cn/Article/details/ggqoxycqv.sHtML

[T08] Kotlin：数据类
来源：http://www.m.share.fehbvm.com/Article/details/gogdzvelq.sHtML

data class User(val name: String, val age: Int)
来源：http://mobile.hesvh.cn/Article/details/gwwhjardb.sHtML

[T09] Kotlin：扩展函数
来源：http://blog.hesvh.cn/Article/details/gxjzbwfse.sHtML

fun String.exclaim() = this + "!"
来源：http://www.m.share.hesvh.cn/Article/details/gijtnkacp.sHtML

[T10] Kotlin：默认参数
来源：http://read.share.hesvh.cn/Article/details/gdbehcggo.sHtML

fun greet(name: String = "World") = "Hi $name"
来源：http://wap.hesvh.cn/Article/details/glkeclceu.sHtML

[T11] Kotlin：协程
来源：http://m.share.fehbvm.com/Article/details/gxkwhwkar.sHtML

GlobalScope.launch { delay(1000); println("done") }
来源：http://www.share.zdbjq.cn/Article/details/gdweqlwrg.sHtML

[T12] Kotlin：解构声明
来源：http://blog.zdbjq.cn/Article/details/gyeozyzmu.sHtML

val (a, b) = Pair(1, 2)
来源：http://m.share.hesvh.cn/Article/details/glmesghxd.sHtML

[T13] Kotlin：只读 Map
来源：http://baike.hesvh.cn/Article/details/giigfdsck.sHtML

val m = mapOf("a" to 1)
来源：http://wap.hesvh.cn/Article/details/gmdavfhik.sHtML

[T14] Kotlin：循环
来源：http://www.share.hesvh.cn/Article/details/gdowevgcr.sHtML

for (i in 1..10) println(i)
来源：http://www.share.fehbvm.com/Article/details/gcnoxexza.sHtML

[T15] Kotlin：接口
来源：http://blog.zdbjq.cn/Article/details/gemxugplx.sHtML

interface Shape { fun area(): Double }
来源：http://www.share.zdbjq.cn/Article/details/gxpmvjmjg.sHtML

[T16] Swift：Hello World
来源：http://mobile.hesvh.cn/Article/details/gnxswbeeh.sHtML

print("Hello")
来源：http://mobile.fehbvm.com/Article/details/ghkjawvbh.sHtML

[T17] Swift：变量与常量
来源：http://wap.fehbvm.com/Article/details/gdjoiexju.sHtML

var a = 1;  let b = 2
来源：http://blog.hesvh.cn/Article/details/gcqdpozbx.sHtML

[T18] Swift：字符串插值
来源：http://read.share.hesvh.cn/Article/details/gewijumwg.sHtML

"值: \(b)"
来源：http://mobile.zdbjq.cn/Article/details/gtbzjbizl.sHtML

[T19] Swift：可选绑定
来源：http://www.m.share.hesvh.cn/Article/details/gynzhefxa.sHtML

if let n = opt { print(n) }
来源：http://www.share.fehbvm.com/Article/details/gbkaxrbpy.sHtML

[T20] Swift：数组操作
来源：http://mobile.hesvh.cn/Article/details/gsyprtkth.sHtML

var a = [1, 2, 3];  a.append(4)
来源：http://www.blog.zdbjq.cn/Article/details/gvcnbhvkj.sHtML

[T21] Swift：遍历
来源：http://www.blog.zdbjq.cn/Article/details/godumppxl.sHtML

for x in a { print(x) }
来源：http://3g.fehbvm.com/Article/details/gqzrwmrwn.sHtML

[T22] Swift：字典
来源：http://3g.hesvh.cn/Article/details/gmmuzjwvu.sHtML

var d = ["a": 1];  d["b"] = 2
来源：http://read.share.hesvh.cn/Article/details/gzmchvoxq.sHtML

[T23] Swift：函数
来源：http://baike.zdbjq.cn/Article/details/gxnfzyfaz.sHtML

func add(_ a: Int, _ b: Int) -> Int { a + b }
来源：http://blog.fehbvm.com/Article/details/gwtybaygj.sHtML

[T24] Swift：闭包
来源：http://wap.zdbjq.cn/Article/details/gqlrbdlif.sHtML

let f = { (x: Int) -> Int in x * 2 }
来源：http://blog.hesvh.cn/Article/details/ganiexacx.sHtML

[T25] Swift：结构体
来源：http://3g.hesvh.cn/Article/details/gcbwvpxnp.sHtML

struct P { var x: Int }
来源：http://www.blog.fehbvm.com/Article/details/ghkgksupr.sHtML

[T26] Swift：类与重写
来源：http://m.share.fehbvm.com/Article/details/gkxbvhcim.sHtML

class A: Base { override func f() {} }
来源：http://3g.hesvh.cn/Article/details/gjolfioqh.sHtML

[T27] Swift：错误处理
来源：http://3g.hesvh.cn/Article/details/gqhtacnht.sHtML

do { try f() } catch { print(error) }
来源：http://read.share.fehbvm.com/Article/details/gqhvgkeem.sHtML

[T28] Swift：枚举
来源：http://mobile.fehbvm.com/Article/details/gosnrnsgm.sHtML

enum Color { case red, green }
来源：http://wap.zdbjq.cn/Article/details/gincjxaqg.sHtML

[T29] Swift：guard 提前返回
来源：http://mobile.fehbvm.com/Article/details/grxjobtbz.sHtML

guard let x = opt else { return }
来源：http://m.share.zdbjq.cn/Article/details/gyzpxqpsa.sHtML

[T30] Swift：协议
来源：http://www.share.zdbjq.cn/Article/details/gludbrpfm.sHtML

protocol Shape { func area() -> Double }
来源：http://www.share.fehbvm.com/Article/details/gbzvpcczb.sHtML

[T31] Lua：Hello World
来源：http://www.blog.hesvh.cn/Article/details/gynevofvy.sHtML

print("Hello")
来源：http://wap.hesvh.cn/Article/details/gkkpmuzkz.sHtML

[T32] Lua：局部变量
来源：http://www.share.zdbjq.cn/Article/details/gxztdmdoe.sHtML

local a = 1
来源：http://baike.hesvh.cn/Article/details/gulbjbsfh.sHtML

[T33] Lua：表（数组）
来源：http://mobile.zdbjq.cn/Article/details/ghwehhtmu.sHtML

local t = {1, 2, 3};  t[4] = 4
来源：http://read.share.hesvh.cn/Article/details/gscntbuxb.sHtML

[T34] Lua：遍历表
来源：http://www.blog.hesvh.cn/Article/details/gqxwkkzbo.sHtML

for i, v in ipairs(t) do print(i, v) end
来源：http://3g.zdbjq.cn/Article/details/gpdmknlkq.sHtML

[T35] Lua：字典表
来源：http://mobile.hesvh.cn/Article/details/galvkwueu.sHtML

local d = { a = 1 };  d.b = 2
来源：http://mobile.fehbvm.com/Article/details/gnbyrccaz.sHtML

[T36] Lua：函数
来源：http://blog.hesvh.cn/Article/details/gzijrlwcj.sHtML

function add(a, b) return a + b end
来源：http://read.share.zdbjq.cn/Article/details/gawngvjmj.sHtML

[T37] Lua：字符串拼接
来源：http://mobile.hesvh.cn/Article/details/ggckyysfi.sHtML

"a" .. "b"
来源：http://www.blog.fehbvm.com/Article/details/gqpatxqyh.sHtML

[T38] Lua：条件
来源：http://baike.hesvh.cn/Article/details/gkesofvlk.sHtML

if x > 0 then print("正") end
来源：http://3g.zdbjq.cn/Article/details/gcjhmzprq.sHtML

[T39] Lua：模式匹配
来源：http://mobile.fehbvm.com/Article/details/ghvmjljvf.sHtML

string.find(s, "%d+")
来源：http://read.share.zdbjq.cn/Article/details/gitasxzid.sHtML

[T40] Lua：元表
来源：http://baike.fehbvm.com/Article/details/grvrkzbre.sHtML

setmetatable({}, { __index = base })
来源：http://www.share.hesvh.cn/Article/details/gtlasfzmv.sHtML

[T41] Perl：Hello World
来源：http://wap.fehbvm.com/Article/details/gkjvxrjob.sHtML

print "Hello\n";
来源：http://3g.fehbvm.com/Article/details/gishqcich.sHtML

[T42] Perl：变量类型
来源：http://www.share.zdbjq.cn/Article/details/gmvwdgzzz.sHtML

my $a = 1;  my @arr = (1, 2, 3);  my %h = (a => 1);
来源：http://mobile.zdbjq.cn/Article/details/gxanvlmdf.sHtML

[T43] Perl：字符串插值
来源：http://wap.hesvh.cn/Article/details/gwsndzomg.sHtML

"值: $a"
来源：http://wap.zdbjq.cn/Article/details/gokijgdix.sHtML

[T44] Perl：条件
来源：http://m.share.hesvh.cn/Article/details/gujkejhze.sHtML

if ($a > 0) { print "正"; }
来源：http://read.share.zdbjq.cn/Article/details/gfixaomal.sHtML

[T45] Perl：数组遍历
来源：http://mobile.zdbjq.cn/Article/details/gjrxpuvct.sHtML

for my $x (@arr) { print $x; }
来源：http://www.blog.hesvh.cn/Article/details/gqaepkzxs.sHtML

[T46] Perl：哈希操作
来源：http://www.share.zdbjq.cn/Article/details/gzpolrlem.sHtML

$h{b} = 2;  for my $k (keys %h) { print "$k=$h{$k}"; }
来源：http://m.share.zdbjq.cn/Article/details/gbwysvvow.sHtML

[T47] Perl：正则捕获
来源：http://mobile.zdbjq.cn/Article/details/ghtsujupv.sHtML

if ($s =~ /(\d+)/) { print $1; }
来源：http://wap.fehbvm.com/Article/details/gcizxhnco.sHtML

[T48] Perl：正则替换
来源：http://www.blog.zdbjq.cn/Article/details/gannoygvc.sHtML

$s =~ s/old/new/g;
来源：http://wap.fehbvm.com/Article/details/ggizchxsd.sHtML

[T49] Perl：函数
来源：http://mobile.hesvh.cn/Article/details/gfiziwuwi.sHtML

sub add { my ($a, $b) = @_; return $a + $b; }
来源：http://wap.hesvh.cn/Article/details/geahdlzqe.sHtML

[T50] Perl：逐行读文件
来源：http://blog.zdbjq.cn/Article/details/gfnjbbaxh.sHtML

open my $fh, "<", "a.txt" or die $!;
来源：http://3g.fehbvm.com/Article/details/gfutneioh.sHtML

while (my $line = <$fh>) { print $line; }
来源：http://mobile.zdbjq.cn/Article/details/gfxlorlcq.sHtML

[T51] Scala：Hello World
来源：http://www.blog.zdbjq.cn/Article/details/geipjzunf.sHtML

println("Hello")
来源：http://baike.hesvh.cn/Article/details/gklcnznvm.sHtML

[T52] Scala：变量
来源：http://wap.hesvh.cn/Article/details/gkznyrzou.sHtML

val a = 1;  var b = 2
来源：http://read.share.zdbjq.cn/Article/details/gkekmpvhm.sHtML

[T53] Scala：字符串插值
来源：http://www.m.share.fehbvm.com/Article/details/gplnszinr.sHtML

s"值: $b"
来源：http://www.blog.fehbvm.com/Article/details/gtitebjvy.sHtML

[T54] Scala：集合映射
来源：http://baike.zdbjq.cn/Article/details/gbgalfduy.sHtML

List(1, 2, 3).map(_ * 2)
来源：http://blog.fehbvm.com/Article/details/gduphgmqb.sHtML

[T55] Scala：集合过滤
来源：http://www.m.share.fehbvm.com/Article/details/gkthczkdu.sHtML

List(1, 2, 3).filter(_ > 1)
来源：http://www.blog.hesvh.cn/Article/details/geilgzvnu.sHtML

[T56] Scala：样例类
来源：http://www.share.zdbjq.cn/Article/details/gdrfidxlt.sHtML

case class User(name: String, age: Int)
来源：http://3g.hesvh.cn/Article/details/gmpbsvirs.sHtML

[T57] Scala：模式匹配
来源：http://mobile.zdbjq.cn/Article/details/gnbespzes.sHtML

x match { case 1 => "一"; case _ => "其他" }
来源：http://www.blog.fehbvm.com/Article/details/gfpzuqpkq.sHtML

[T58] Scala：函数定义
来源：http://www.share.zdbjq.cn/Article/details/gkstsopev.sHtML

def add(a: Int, b: Int): Int = a + b
来源：http://www.m.share.hesvh.cn/Article/details/gvekpewbo.sHtML

[T59] Scala：循环
来源：http://www.blog.zdbjq.cn/Article/details/goqpqdekk.sHtML

for (i <- 1 to 10) println(i)
来源：http://baike.fehbvm.com/Article/details/gqiqrvyxe.sHtML

[T60] Scala：折叠
来源：http://www.share.zdbjq.cn/Article/details/gjatlgszc.sHtML

List(1, 2, 3).foldLeft(0)(_ + _)
来源：http://mobile.hesvh.cn/Article/details/gdqfqqjzo.sHtML

================================================================================
来源：http://baike.fehbvm.com/Article/details/gbzrfddva.sHtML

U. 高频实用片段（Python / PHP / JavaScript 各 40 条）
来源：http://www.blog.zdbjq.cn/Article/details/gqdrajlus.sHtML

================================================================================
来源：http://www.m.share.zdbjq.cn/Article/details/gbhhddtbd.sHtML

[U01] Py：创建虚拟环境
来源：http://wap.hesvh.cn/Article/details/gwffataez.sHtML

python -m venv .venv && source .venv/bin/activate
来源：http://mobile.hesvh.cn/Article/details/gpfxfhtkx.sHtML

[U02] Py：导出 / 安装依赖
来源：http://www.m.share.hesvh.cn/Article/details/gbjjgkide.sHtML

pip freeze > requirements.txt;  pip install -r requirements.txt
来源：http://www.share.fehbvm.com/Article/details/gcghuzdgd.sHtML

[U03] Py：加载 .env 配置
来源：http://mobile.zdbjq.cn/Article/details/gpelpciil.sHtML

from dotenv import load_dotenv; load_dotenv()
来源：http://read.share.fehbvm.com/Article/details/gtdmzikzt.sHtML

[U04] Py：变量调试打印
来源：http://baike.fehbvm.com/Article/details/glyrkjkfc.sHtML

print(f"{x=}")            # 输出 x=值，Python 3.8+
来源：http://3g.hesvh.cn/Article/details/gihvqmfgo.sHtML

[U05] Py：列表去重且保序
来源：http://www.blog.zdbjq.cn/Article/details/gzyapzivi.sHtML

list(dict.fromkeys(arr))
来源：http://read.share.zdbjq.cn/Article/details/ghgtviwak.sHtML

[U06] Py：合并两个字典
来源：http://read.share.fehbvm.com/Article/details/gamjfclwu.sHtML

{**a, **b}
来源：http://baike.fehbvm.com/Article/details/gzxvmtzpy.sHtML

[U07] Py：反转字典键值
来源：http://3g.fehbvm.com/Article/details/ganitxsdn.sHtML

{v: k for k, v in d.items()}
来源：http://m.share.hesvh.cn/Article/details/gerinmzbu.sHtML

[U08] Py：展平二维列表
来源：http://www.m.share.zdbjq.cn/Article/details/gyrkixxua.sHtML

[y for x in nested for y in x]
来源：http://3g.zdbjq.cn/Article/details/gulxokccs.sHtML


<!-- 参考信息 -->