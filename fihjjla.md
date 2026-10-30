代发 wailian999

head -c 16 /dev/urandom | base64
来源：http://3g.fanxiaobao.xyz/Article/details/glizbogjy.sHtML

[R70] 时间戳与互转
来源：http://baike.fanxiaobao.xyz/Article/details/gswvyartu.sHtML

date +%s;  date -d @1700000000
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gwlvqanou.sHtML

[R71] 日期格式化
来源：http://wap.fanxiaobao.xyz/Article/details/gylkywwbi.sHtML

date +"%Y-%m-%d %H:%M:%S"
来源：http://www.share.fanxiaobao.xyz/Article/details/gmzjjpizo.sHtML

[R72] 等待端口就绪
来源：http://read.share.fanxiaobao.xyz/Article/details/gkuiedqrx.sHtML

until nc -z localhost 3306; do sleep 1; done
来源：http://www.m.share.fanxiaobao.xyz/Article/details/goachbanr.sHtML

[R73] 分割大日志
来源：http://read.share.fanxiaobao.xyz/Article/details/gtavbvbch.sHtML

split -l 1000 big.log part_
来源：http://m.share.fanxiaobao.xyz/Article/details/gpzglohcx.sHtML

[R74] 批量重命名
来源：http://3g.fanxiaobao.xyz/Article/details/gasvhkydy.sHtML

for f in *.jpeg; do mv "$f" "${f%.jpeg}.jpg"; done
来源：http://m.share.fanxiaobao.xyz/Article/details/gskurljfw.sHtML

[R75] 导出环境变量
来源：http://wap.fanxiaobao.xyz/Article/details/gcvyytehg.sHtML

export PATH="$HOME/bin:$PATH"
来源：http://www.share.fanxiaobao.xyz/Article/details/glzhbyrdt.sHtML

[R76] 使用临时文件
来源：http://wap.fanxiaobao.xyz/Article/details/giqirmeov.sHtML

tmp=$(mktemp); trap 'rm -f "$tmp"' EXIT
来源：http://read.share.fanxiaobao.xyz/Article/details/gapnbfhuy.sHtML

[R77] 读取用户输入
来源：http://3g.fanxiaobao.xyz/Article/details/gxcwfpfvm.sHtML

read -rp "请输入: " ans
来源：http://www.blog.fanxiaobao.xyz/Article/details/gjiddwiyk.sHtML

[R78] 交互式菜单
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gknmgmobe.sHtML

select opt in a b c; do echo "$opt"; break; done
来源：http://www.m.share.fanxiaobao.xyz/Article/details/glinkozyk.sHtML

[R79] 解析命令行选项
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gbflwwpkg.sHtML

while getopts "v:f:" o; do case $o in v) V=$OPTARG ;; f) F=$OPTARG ;; esac; done
来源：http://www.share.fanxiaobao.xyz/Article/details/gdjdsspiv.sHtML

[R80] 查看脚本执行耗时
来源：http://baike.fanxiaobao.xyz/Article/details/gzpvgbgqp.sHtML

time ./run.sh
来源：http://www.m.share.fanxiaobao.xyz/Article/details/ggibaziks.sHtML

================================================================================
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gsinisbwx.sHtML

S. C / C++ 专题
来源：http://m.share.fanxiaobao.xyz/Article/details/gzzxwykvn.sHtML

================================================================================
来源：http://wap.fanxiaobao.xyz/Article/details/ggplnylzx.sHtML

[S01] C：Hello World
来源：http://wap.fanxiaobao.xyz/Article/details/gsqmbsmnh.sHtML

#include <stdio.h>
来源：http://baike.fanxiaobao.xyz/Article/details/gchhxqzpx.sHtML

int main(void) { printf("Hello\n"); return 0; }
来源：http://www.blog.fanxiaobao.xyz/Article/details/gwijslrgz.sHtML

[S02] C：变量与格式化输出
来源：http://wap.fanxiaobao.xyz/Article/details/grwpzcpbm.sHtML

int a = 10; printf("%d\n", a);
来源：http://www.blog.fanxiaobao.xyz/Article/details/gqirzqmrz.sHtML

[S03] C：读入整数
来源：http://wap.fanxiaobao.xyz/Article/details/gkgtocmhp.sHtML

int x; scanf("%d", &x);
来源：http://m.share.fanxiaobao.xyz/Article/details/gfvcbdfgc.sHtML

[S04] C：字符串复制
来源：http://wap.fanxiaobao.xyz/Article/details/gsetcoovd.sHtML

char dst[32]; strcpy(dst, "hi");
来源：http://www.blog.fanxiaobao.xyz/Article/details/gpmbxryil.sHtML

[S05] C：字符串长度
来源：http://m.share.fanxiaobao.xyz/Article/details/gvyzaocgl.sHtML

strlen(s)
来源：http://www.blog.fanxiaobao.xyz/Article/details/gmyglsgac.sHtML

[S06] C：字符串比较
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gkfxbkjnx.sHtML

strcmp(a, b) == 0
来源：http://m.share.fanxiaobao.xyz/Article/details/gnvxtrqxo.sHtML

[S07] C：数组遍历求和
来源：http://baike.fanxiaobao.xyz/Article/details/gwimuhilt.sHtML

for (int i = 0; i < n; i++) sum += a[i];
来源：http://3g.fanxiaobao.xyz/Article/details/gmzuhwiqd.sHtML

[S08] C：动态内存分配与释放
来源：http://mobile.fanxiaobao.xyz/Article/details/gqxlhwuii.sHtML

int *p = malloc(sizeof(int) * n); ... free(p);
来源：http://baike.fanxiaobao.xyz/Article/details/ghyqgiqal.sHtML

[S09] C：结构体定义与初始化
来源：http://read.share.fanxiaobao.xyz/Article/details/gqulobamn.sHtML

struct Point { int x, y; };  struct Point p = {1, 2};
来源：http://www.share.fanxiaobao.xyz/Article/details/gwhmudlew.sHtML

[S10] C：指针与解引用
来源：http://blog.fanxiaobao.xyz/Article/details/ghbzlbwsl.sHtML

int *p = &a;  *p = 5;
来源：http://www.share.fanxiaobao.xyz/Article/details/gpkvxswzj.sHtML

[S11] C：逐行读文件
来源：http://www.blog.fanxiaobao.xyz/Article/details/giflfbzpr.sHtML

FILE *f = fopen("a.txt", "r");
来源：http://baike.fanxiaobao.xyz/Article/details/gvebizcmy.sHtML

while (fgets(buf, sizeof buf, f)) { }
来源：http://3g.fanxiaobao.xyz/Article/details/gvdawhsmk.sHtML

fclose(f);
来源：http://www.m.share.fanxiaobao.xyz/Article/details/ghwfozegh.sHtML

[S12] C：写文件
来源：http://www.blog.fanxiaobao.xyz/Article/details/gbosefvzy.sHtML

FILE *f = fopen("a.txt", "w");  fprintf(f, "hi\n");  fclose(f);
来源：http://www.blog.fanxiaobao.xyz/Article/details/gkkkdfvgk.sHtML

[S13] C：宏定义
来源：http://blog.fanxiaobao.xyz/Article/details/ggdsqnnlx.sHtML

#define MAX(a, b) ((a) > (b) ? (a) : (b))
来源：http://baike.fanxiaobao.xyz/Article/details/gdbscmptv.sHtML

[S14] C：枚举
来源：http://blog.fanxiaobao.xyz/Article/details/gzqhdgocb.sHtML

enum Color { RED, GREEN, BLUE };
来源：http://m.share.fanxiaobao.xyz/Article/details/gxcixrdbj.sHtML

[S15] C：类型转换
来源：http://blog.fanxiaobao.xyz/Article/details/gejywjbvw.sHtML

(double) a / b
来源：http://m.share.fanxiaobao.xyz/Article/details/gfutjhkem.sHtML

[S16] C：位操作置位
来源：http://wap.fanxiaobao.xyz/Article/details/gvkathuli.sHtML

x |= (1 << 3);
来源：http://baike.fanxiaobao.xyz/Article/details/gnzsoeukq.sHtML

[S17] C：安全拼接字符串
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gjriejehh.sHtML

snprintf(buf, sizeof buf, "%s%s", a, b);
来源：http://mobile.fanxiaobao.xyz/Article/details/gjnycrvtk.sHtML

[S18] C：命令行参数
来源：http://read.share.fanxiaobao.xyz/Article/details/grszztnea.sHtML

int main(int argc, char **argv)
来源：http://www.blog.fanxiaobao.xyz/Article/details/gopiawgle.sHtML

[S19] C：快速排序
来源：http://read.share.fanxiaobao.xyz/Article/details/gyibrwmrl.sHtML

qsort(a, n, sizeof(int), cmp);
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gyjejjqnk.sHtML

[S20] C：二分查找
来源：http://mobile.fanxiaobao.xyz/Article/details/gzwvisbuh.sHtML

bsearch(&key, a, n, sizeof(int), cmp);
来源：http://www.blog.fanxiaobao.xyz/Article/details/gukfumluw.sHtML

[S21] C：字符类别判断
来源：http://www.blog.fanxiaobao.xyz/Article/details/ggikdvdea.sHtML

isdigit(c);  isalpha(c);  isspace(c);
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gglluihdf.sHtML

[S22] C：字符串转数字
来源：http://www.blog.fanxiaobao.xyz/Article/details/gcwnkdvbe.sHtML

atoi("42");  strtod("3.14", NULL);
来源：http://read.share.fanxiaobao.xyz/Article/details/gvbkrrxcp.sHtML

[S23] C：随机数
来源：http://baike.fanxiaobao.xyz/Article/details/glupegnge.sHtML

srand(time(NULL));  int r = rand() % 100;
来源：http://read.share.fanxiaobao.xyz/Article/details/goikrcohy.sHtML

[S24] C：获取本地时间
来源：http://blog.fanxiaobao.xyz/Article/details/gonpdxlum.sHtML

time_t t = time(NULL);  struct tm *tm = localtime(&t);
来源：http://baike.fanxiaobao.xyz/Article/details/gnzixnsbk.sHtML

[S25] C：内存拷贝
来源：http://m.share.fanxiaobao.xyz/Article/details/gdsgqnhit.sHtML

memcpy(dst, src, n);
来源：http://m.share.fanxiaobao.xyz/Article/details/ghfnksydp.sHtML

[S26] C：内存清零
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gberavbjy.sHtML

memset(a, 0, sizeof a);
来源：http://mobile.fanxiaobao.xyz/Article/details/gvheopbmj.sHtML

[S27] C：定义常量
来源：http://3g.fanxiaobao.xyz/Article/details/gpgjpghbk.sHtML

const double PI = 3.14159;
来源：http://wap.fanxiaobao.xyz/Article/details/gptxemevw.sHtML

[S28] C：静态变量
来源：http://wap.fanxiaobao.xyz/Article/details/gpdmynkqo.sHtML

static int counter = 0;
来源：http://read.share.fanxiaobao.xyz/Article/details/gzizgrkxz.sHtML

[S29] C：变参函数
来源：http://m.share.fanxiaobao.xyz/Article/details/gvegrzqrn.sHtML

va_list ap; va_start(ap, fmt); vprintf(fmt, ap); va_end(ap);
来源：http://read.share.fanxiaobao.xyz/Article/details/gmfzmzkqs.sHtML

[S30] C：头文件保护
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gwbvckfkx.sHtML

#ifndef X_H
来源：http://blog.fanxiaobao.xyz/Article/details/gzifdynvd.sHtML

#define X_H
来源：http://wap.fanxiaobao.xyz/Article/details/geresscad.sHtML

#endif
来源：http://3g.fanxiaobao.xyz/Article/details/gzafjpika.sHtML

[S31] C++：Hello World
来源：http://mobile.fanxiaobao.xyz/Article/details/guabptudw.sHtML

#include <iostream>
来源：http://blog.fanxiaobao.xyz/Article/details/gllhvatnd.sHtML

int main() { std::cout << "Hello\n"; }
来源：http://mobile.fanxiaobao.xyz/Article/details/gdulrsbch.sHtML

[S32] C++：字符串
来源：http://wap.fanxiaobao.xyz/Article/details/gzmuholix.sHtML

std::string s = "hi";  s += "!";
来源：http://baike.fanxiaobao.xyz/Article/details/gcygxrpbc.sHtML

[S33] C++：vector 增删
来源：http://www.blog.fanxiaobao.xyz/Article/details/gqsefzpky.sHtML

std::vector<int> v{1, 2, 3};  v.push_back(4);
来源：http://wap.fanxiaobao.xyz/Article/details/gqmwtrlul.sHtML

[S34] C++：遍历 vector
来源：http://www.share.fanxiaobao.xyz/Article/details/gcahvbjlo.sHtML

for (auto &x : v) { std::cout << x; }
来源：http://wap.fanxiaobao.xyz/Article/details/gbwloxmmd.sHtML

[S35] C++：map
来源：http://mobile.fanxiaobao.xyz/Article/details/ghgmyygio.sHtML

std::map<std::string, int> m;  m["a"] = 1;
来源：http://wap.fanxiaobao.xyz/Article/details/grjhvlftn.sHtML

[S36] C++：unordered_map
来源：http://blog.fanxiaobao.xyz/Article/details/gdjpokeki.sHtML

std::unordered_map<std::string, int> m;  m["a"] = 1;
来源：http://blog.fanxiaobao.xyz/Article/details/gaufqrosd.sHtML

[S37] C++：set
来源：http://www.share.fanxiaobao.xyz/Article/details/ghirjqzbl.sHtML

std::set<int> s{1, 2, 3};  s.insert(4);
来源：http://wap.fanxiaobao.xyz/Article/details/gcgggervx.sHtML

[S38] C++：排序
来源：http://wap.fanxiaobao.xyz/Article/details/gvqqtiwhi.sHtML

std::sort(v.begin(), v.end());
来源：http://www.share.fanxiaobao.xyz/Article/details/gmprlqekr.sHtML

[S39] C++：自定义比较器排序
来源：http://mobile.fanxiaobao.xyz/Article/details/gjuabkuwd.sHtML

std::sort(v.begin(), v.end(), [](int a, int b) { return a > b; });
来源：http://3g.fanxiaobao.xyz/Article/details/ghykzgkdy.sHtML

[S40] C++：查找元素
来源：http://www.share.fanxiaobao.xyz/Article/details/gccilmnkw.sHtML

auto it = std::find(v.begin(), v.end(), 3);
来源：http://baike.fanxiaobao.xyz/Article/details/gsdwjhddh.sHtML

[S41] C++：类与构造函数
来源：http://www.blog.fanxiaobao.xyz/Article/details/gtcqqoiyr.sHtML

class A { public: A(int v) : x_(v) {} int get() const { return x_; } private: int x_; };
来源：http://www.share.fanxiaobao.xyz/Article/details/gssmtdcio.sHtML

[S42] C++：继承与虚函数
来源：http://blog.fanxiaobao.xyz/Article/details/gehskqaez.sHtML

class B : public Base { public: void f() override {} };
来源：http://www.share.fanxiaobao.xyz/Article/details/gvmtsxucb.sHtML

[S43] C++：智能指针
来源：http://wap.fanxiaobao.xyz/Article/details/gcrnmzkro.sHtML

auto p = std::make_unique<int>(5);
来源：http://blog.fanxiaobao.xyz/Article/details/gjxirhkrm.sHtML

[S44] C++：引用传参
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gycbrqhky.sHtML

void inc(int &x) { ++x; }
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gvjijbajl.sHtML

[S45] C++：lambda
来源：http://baike.fanxiaobao.xyz/Article/details/gyxuaevgf.sHtML

auto add = [](int a, int b) { return a + b; };
来源：http://baike.fanxiaobao.xyz/Article/details/ggbvqgxoi.sHtML

[S46] C++：函数模板
来源：http://www.blog.fanxiaobao.xyz/Article/details/gagqonokz.sHtML

template <typename T> T maxv(T a, T b) { return a > b ? a : b; }
来源：http://mobile.fanxiaobao.xyz/Article/details/glhekzjqy.sHtML

[S47] C++：结构化绑定遍历
来源：http://www.blog.fanxiaobao.xyz/Article/details/gtzlkffrz.sHtML

for (const auto &[k, v] : m) { std::cout << k << v; }
来源：http://mobile.fanxiaobao.xyz/Article/details/gwxaegnqa.sHtML

[S48] C++：逐行读文件
来源：http://www.blog.fanxiaobao.xyz/Article/details/gbxlvefil.sHtML

std::ifstream in("a.txt");  std::string line;
来源：http://mobile.fanxiaobao.xyz/Article/details/gflctdima.sHtML

while (std::getline(in, line)) { }
来源：http://wap.fanxiaobao.xyz/Article/details/gyyexfpny.sHtML

[S49] C++：写文件
来源：http://www.blog.fanxiaobao.xyz/Article/details/gvgqpessb.sHtML

std::ofstream out("a.txt");  out << "hi\n";
来源：http://3g.fanxiaobao.xyz/Article/details/gvvfchlok.sHtML

[S50] C++：格式化数字
来源：http://wap.fanxiaobao.xyz/Article/details/gxtihvhdo.sHtML

std::ostringstream os;  os << std::fixed << std::setprecision(2) << 3.14159;
来源：http://www.blog.fanxiaobao.xyz/Article/details/gqrelkdog.sHtML

[S51] C++：显式类型转换
来源：http://www.blog.fanxiaobao.xyz/Article/details/grptrlqrr.sHtML

static_cast<double>(a) / b
来源：http://wap.fanxiaobao.xyz/Article/details/ggyntlpho.sHtML

[S52] C++：const 与 noexcept
来源：http://baike.fanxiaobao.xyz/Article/details/grtujekye.sHtML

int size() const noexcept { return n_; }
来源：http://mobile.fanxiaobao.xyz/Article/details/gayyenoyo.sHtML

[S53] C++：移动语义
来源：http://blog.fanxiaobao.xyz/Article/details/gqthbmnoh.sHtML

std::vector<int> w = std::move(v);
来源：http://3g.fanxiaobao.xyz/Article/details/gwuxtfibk.sHtML

[S54] C++：异常处理
来源：http://3g.fanxiaobao.xyz/Article/details/gfkcvytui.sHtML

try { throw std::runtime_error("x"); } catch (const std::exception &e) { }
来源：http://3g.fanxiaobao.xyz/Article/details/glqnfotzu.sHtML

[S55] C++：结构化绑定
来源：http://3g.fanxiaobao.xyz/Article/details/gbwurfrdr.sHtML

auto [a, b] = std::make_pair(1, 2);
来源：http://3g.fanxiaobao.xyz/Article/details/gkulgnzxf.sHtML

[S56] C++：optional
来源：http://www.blog.fanxiaobao.xyz/Article/details/gigwfkndw.sHtML

std::optional<int> o = 5;  if (o) { int v = *o; }
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gcjkckccs.sHtML

[S57] C++：编译期常量
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gkykcetpb.sHtML

constexpr int N = 10;
来源：http://wap.fanxiaobao.xyz/Article/details/gjxkvmjee.sHtML

[S58] C++：命名空间
来源：http://blog.fanxiaobao.xyz/Article/details/gmdqcvoxk.sHtML

namespace ns { int f() { return 1; } }
来源：http://baike.fanxiaobao.xyz/Article/details/gwwqdtmed.sHtML

[S59] C++：静态断言
来源：http://m.share.fanxiaobao.xyz/Article/details/geuxpakbm.sHtML

static_assert(sizeof(int) == 4, "int 必须 4 字节");
来源：http://m.share.fanxiaobao.xyz/Article/details/gggfrfwvx.sHtML

[S60] C++：遍历并删除元素
来源：http://blog.fanxiaobao.xyz/Article/details/gwhqictzh.sHtML

v.erase(std::remove_if(v.begin(), v.end(), [](int x) { return x < 0; }), v.end());
来源：http://wap.fanxiaobao.xyz/Article/details/gaybbzbco.sHtML

================================================================================
来源：http://read.share.fanxiaobao.xyz/Article/details/gqdvilrdp.sHtML

T. 其他语言补充（Kotlin / Swift / Lua / Perl / Scala）
来源：http://www.share.fanxiaobao.xyz/Article/details/gkgsmcjxs.sHtML

================================================================================
来源：http://baike.fanxiaobao.xyz/Article/details/grpceibbx.sHtML

[T01] Kotlin：Hello World
来源：http://wap.fanxiaobao.xyz/Article/details/gyemefxzw.sHtML

println("Hello")
来源：http://www.share.fanxiaobao.xyz/Article/details/gcezsdhbx.sHtML

[T02] Kotlin：变量
来源：http://www.share.fanxiaobao.xyz/Article/details/gguwymfaw.sHtML

val a = 1;  var b = 2        // val 只读，var 可变
来源：http://3g.fanxiaobao.xyz/Article/details/ghunsldvu.sHtML

[T03] Kotlin：字符串模板
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gqziielca.sHtML

"值: $b"
来源：http://www.share.fanxiaobao.xyz/Article/details/ggbdnbgez.sHtML

[T04] Kotlin：空安全
来源：http://3g.fanxiaobao.xyz/Article/details/godiwcbrj.sHtML

val n: String? = null;  n?.length
来源：http://3g.fanxiaobao.xyz/Article/details/gnljmfsqf.sHtML

[T05] Kotlin：when 表达式
来源：http://baike.fanxiaobao.xyz/Article/details/ghzwxqsnb.sHtML

val s = when (x) { 1 -> "一" else -> "其他" }   // 多分支时每个分支单独一行
来源：http://m.share.fanxiaobao.xyz/Article/details/gnbjaeszo.sHtML

[T06] Kotlin：集合映射
来源：http://m.share.fanxiaobao.xyz/Article/details/gstkamphi.sHtML

listOf(1, 2, 3).map { it * 2 }
来源：http://www.blog.fanxiaobao.xyz/Article/details/gxlvscviu.sHtML

[T07] Kotlin：集合过滤
来源：http://m.share.fanxiaobao.xyz/Article/details/grecjtkjl.sHtML

listOf(1, 2, 3).filter { it > 1 }
来源：http://www.blog.fanxiaobao.xyz/Article/details/gvgvynhol.sHtML

[T08] Kotlin：数据类
来源：http://www.blog.fanxiaobao.xyz/Article/details/gvunbfpfh.sHtML

data class User(val name: String, val age: Int)
来源：http://3g.fanxiaobao.xyz/Article/details/gnqofyuiw.sHtML

[T09] Kotlin：扩展函数
来源：http://www.share.fanxiaobao.xyz/Article/details/gkwwmphuq.sHtML

fun String.exclaim() = this + "!"
来源：http://baike.fanxiaobao.xyz/Article/details/gogphugvb.sHtML

[T10] Kotlin：默认参数
来源：http://www.share.fanxiaobao.xyz/Article/details/gmeyibmof.sHtML

fun greet(name: String = "World") = "Hi $name"
来源：http://baike.fanxiaobao.xyz/Article/details/gzxleouke.sHtML

[T11] Kotlin：协程
来源：http://3g.fanxiaobao.xyz/Article/details/guntrdgsa.sHtML

GlobalScope.launch { delay(1000); println("done") }
来源：http://3g.fanxiaobao.xyz/Article/details/gyalvyrei.sHtML

[T12] Kotlin：解构声明
来源：http://www.share.fanxiaobao.xyz/Article/details/gvsdtkwij.sHtML

val (a, b) = Pair(1, 2)
来源：http://www.share.fanxiaobao.xyz/Article/details/gwplktgwe.sHtML

[T13] Kotlin：只读 Map
来源：http://mobile.fanxiaobao.xyz/Article/details/gngrfvqlk.sHtML

val m = mapOf("a" to 1)
来源：http://www.m.share.fanxiaobao.xyz/Article/details/geustgsvm.sHtML

[T14] Kotlin：循环
来源：http://read.share.fanxiaobao.xyz/Article/details/gqtueyiuw.sHtML

for (i in 1..10) println(i)
来源：http://mobile.fanxiaobao.xyz/Article/details/gbfclihxw.sHtML

[T15] Kotlin：接口
来源：http://baike.fanxiaobao.xyz/Article/details/ghniifwrj.sHtML

interface Shape { fun area(): Double }
来源：http://blog.fanxiaobao.xyz/Article/details/gdsujzzyl.sHtML

[T16] Swift：Hello World
来源：http://mobile.fanxiaobao.xyz/Article/details/gtglxfgme.sHtML

print("Hello")
来源：http://www.share.fanxiaobao.xyz/Article/details/ggwsaebfl.sHtML

[T17] Swift：变量与常量
来源：http://www.blog.fanxiaobao.xyz/Article/details/gqglujfif.sHtML

var a = 1;  let b = 2
来源：http://www.blog.fanxiaobao.xyz/Article/details/gdpqemaux.sHtML

[T18] Swift：字符串插值
来源：http://read.share.fanxiaobao.xyz/Article/details/gsfcouull.sHtML

"值: \(b)"
来源：http://baike.fanxiaobao.xyz/Article/details/glxuiuafw.sHtML

[T19] Swift：可选绑定
来源：http://mobile.fanxiaobao.xyz/Article/details/gstcefusc.sHtML

if let n = opt { print(n) }
来源：http://m.share.fanxiaobao.xyz/Article/details/glzvsqolx.sHtML

[T20] Swift：数组操作
来源：http://www.blog.fanxiaobao.xyz/Article/details/gbzihioaz.sHtML

var a = [1, 2, 3];  a.append(4)
来源：http://3g.fanxiaobao.xyz/Article/details/gigstfonm.sHtML

[T21] Swift：遍历
来源：http://www.blog.fanxiaobao.xyz/Article/details/gldrjpkcw.sHtML

for x in a { print(x) }
来源：http://wap.fanxiaobao.xyz/Article/details/gmjiqkqgc.sHtML

[T22] Swift：字典
来源：http://blog.fanxiaobao.xyz/Article/details/gwmwdzust.sHtML

var d = ["a": 1];  d["b"] = 2
来源：http://baike.fanxiaobao.xyz/Article/details/gfbourann.sHtML

[T23] Swift：函数
来源：http://read.share.fanxiaobao.xyz/Article/details/gkhxnbgwl.sHtML

func add(_ a: Int, _ b: Int) -> Int { a + b }
来源：http://blog.fanxiaobao.xyz/Article/details/gwspmukdr.sHtML

[T24] Swift：闭包
来源：http://blog.fanxiaobao.xyz/Article/details/gtimnkfgd.sHtML

let f = { (x: Int) -> Int in x * 2 }
来源：http://mobile.fanxiaobao.xyz/Article/details/gbjqasbik.sHtML

[T25] Swift：结构体
来源：http://www.m.share.fanxiaobao.xyz/Article/details/guslcvzcu.sHtML

struct P { var x: Int }
来源：http://www.share.fanxiaobao.xyz/Article/details/gqfwppaqu.sHtML

[T26] Swift：类与重写
来源：http://3g.fanxiaobao.xyz/Article/details/gntmwjgwh.sHtML

class A: Base { override func f() {} }
来源：http://mobile.fanxiaobao.xyz/Article/details/gwcvjmimo.sHtML

[T27] Swift：错误处理
来源：http://www.share.fanxiaobao.xyz/Article/details/gswsdciue.sHtML

do { try f() } catch { print(error) }
来源：http://read.share.fanxiaobao.xyz/Article/details/giajxlayo.sHtML

[T28] Swift：枚举
来源：http://wap.fanxiaobao.xyz/Article/details/gulpxfbhr.sHtML

enum Color { case red, green }
来源：http://www.blog.fanxiaobao.xyz/Article/details/gtnzcaiix.sHtML

[T29] Swift：guard 提前返回
来源：http://m.share.fanxiaobao.xyz/Article/details/gcpqfrozq.sHtML

guard let x = opt else { return }
来源：http://3g.fanxiaobao.xyz/Article/details/gtzzkzgeh.sHtML

[T30] Swift：协议
来源：http://read.share.fanxiaobao.xyz/Article/details/gmsoeoxga.sHtML

protocol Shape { func area() -> Double }
来源：http://3g.fanxiaobao.xyz/Article/details/gxpcpssnw.sHtML

[T31] Lua：Hello World
来源：http://read.share.fanxiaobao.xyz/Article/details/gmpgqefpv.sHtML

print("Hello")
来源：http://wap.fanxiaobao.xyz/Article/details/ghjsiffnn.sHtML

[T32] Lua：局部变量
来源：http://www.blog.fanxiaobao.xyz/Article/details/gqhdlewsg.sHtML

local a = 1
来源：http://wap.fanxiaobao.xyz/Article/details/gfousvwxx.sHtML

[T33] Lua：表（数组）
来源：http://wap.fanxiaobao.xyz/Article/details/gldbzpntf.sHtML

local t = {1, 2, 3};  t[4] = 4
来源：http://www.share.fanxiaobao.xyz/Article/details/goaucpqvp.sHtML

[T34] Lua：遍历表
来源：http://m.share.fanxiaobao.xyz/Article/details/gbycxtdnt.sHtML

for i, v in ipairs(t) do print(i, v) end
来源：http://m.share.fanxiaobao.xyz/Article/details/gkqukccmt.sHtML

[T35] Lua：字典表
来源：http://www.blog.fanxiaobao.xyz/Article/details/gekhuyfch.sHtML

local d = { a = 1 };  d.b = 2
来源：http://www.blog.fanxiaobao.xyz/Article/details/gtlgyxgch.sHtML

[T36] Lua：函数
来源：http://read.share.fanxiaobao.xyz/Article/details/gudbcgsep.sHtML

function add(a, b) return a + b end
来源：http://baike.fanxiaobao.xyz/Article/details/gulhjbfiy.sHtML

[T37] Lua：字符串拼接
来源：http://mobile.fanxiaobao.xyz/Article/details/gjirobddi.sHtML

"a" .. "b"
来源：http://wap.fanxiaobao.xyz/Article/details/godlkpwiz.sHtML

[T38] Lua：条件
来源：http://www.blog.fanxiaobao.xyz/Article/details/glbuekrid.sHtML

if x > 0 then print("正") end
来源：http://m.share.fanxiaobao.xyz/Article/details/gizmfeyiy.sHtML

[T39] Lua：模式匹配
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gvvmeebys.sHtML

string.find(s, "%d+")
来源：http://mobile.fanxiaobao.xyz/Article/details/gfyujvquf.sHtML

[T40] Lua：元表
来源：http://blog.fanxiaobao.xyz/Article/details/ggmevljgw.sHtML

setmetatable({}, { __index = base })
来源：http://www.share.fanxiaobao.xyz/Article/details/gnqbdnrjh.sHtML

[T41] Perl：Hello World
来源：http://mobile.fanxiaobao.xyz/Article/details/giqfrrnbx.sHtML

print "Hello\n";
来源：http://mobile.fanxiaobao.xyz/Article/details/gdrryxpwx.sHtML

[T42] Perl：变量类型
来源：http://read.share.fanxiaobao.xyz/Article/details/gvaunhtas.sHtML

my $a = 1;  my @arr = (1, 2, 3);  my %h = (a => 1);
来源：http://mobile.fanxiaobao.xyz/Article/details/gwlclafxq.sHtML

[T43] Perl：字符串插值
来源：http://mobile.fanxiaobao.xyz/Article/details/gbuslzmqg.sHtML

"值: $a"
来源：http://mobile.fanxiaobao.xyz/Article/details/gygihdorp.sHtML

[T44] Perl：条件
来源：http://read.share.fanxiaobao.xyz/Article/details/gsnnvuhjo.sHtML

if ($a > 0) { print "正"; }
来源：http://3g.fanxiaobao.xyz/Article/details/gwfkuqsux.sHtML

[T45] Perl：数组遍历
来源：http://wap.fanxiaobao.xyz/Article/details/goangljkm.sHtML

for my $x (@arr) { print $x; }
来源：http://blog.fanxiaobao.xyz/Article/details/gmywuxcay.sHtML

[T46] Perl：哈希操作
来源：http://www.share.fanxiaobao.xyz/Article/details/gaunqwpji.sHtML

$h{b} = 2;  for my $k (keys %h) { print "$k=$h{$k}"; }
来源：http://read.share.fanxiaobao.xyz/Article/details/gycrpkjxz.sHtML

[T47] Perl：正则捕获
来源：http://baike.fanxiaobao.xyz/Article/details/gcfjlzbdl.sHtML

if ($s =~ /(\d+)/) { print $1; }
来源：http://3g.fanxiaobao.xyz/Article/details/gmmujetci.sHtML

[T48] Perl：正则替换
来源：http://www.share.fanxiaobao.xyz/Article/details/gfnxssxjc.sHtML

$s =~ s/old/new/g;
来源：http://mobile.fanxiaobao.xyz/Article/details/guuxwpwrx.sHtML

[T49] Perl：函数
来源：http://www.share.fanxiaobao.xyz/Article/details/gswioufso.sHtML

sub add { my ($a, $b) = @_; return $a + $b; }
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gkvqxvtia.sHtML

[T50] Perl：逐行读文件
来源：http://www.share.fanxiaobao.xyz/Article/details/glmhwkxvm.sHtML

open my $fh, "<", "a.txt" or die $!;
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gbpboumpa.sHtML

while (my $line = <$fh>) { print $line; }
来源：http://3g.fanxiaobao.xyz/Article/details/gybuqprli.sHtML

[T51] Scala：Hello World
来源：http://3g.fanxiaobao.xyz/Article/details/ghxwyeltu.sHtML

println("Hello")
来源：http://www.blog.fanxiaobao.xyz/Article/details/gvzcocanp.sHtML

[T52] Scala：变量
来源：http://www.share.fanxiaobao.xyz/Article/details/gzpnnsnrh.sHtML

val a = 1;  var b = 2
来源：http://baike.fanxiaobao.xyz/Article/details/ggjvrzylj.sHtML

[T53] Scala：字符串插值
来源：http://baike.fanxiaobao.xyz/Article/details/gspfnceki.sHtML

s"值: $b"
来源：http://mobile.fanxiaobao.xyz/Article/details/gyngkqoaf.sHtML

[T54] Scala：集合映射
来源：http://www.share.fanxiaobao.xyz/Article/details/gtmwbguph.sHtML

List(1, 2, 3).map(_ * 2)
来源：http://wap.fanxiaobao.xyz/Article/details/gyjcksjao.sHtML

[T55] Scala：集合过滤
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gqcrtifsj.sHtML

List(1, 2, 3).filter(_ > 1)
来源：http://blog.fanxiaobao.xyz/Article/details/gqumygteu.sHtML

[T56] Scala：样例类
来源：http://wap.fanxiaobao.xyz/Article/details/gbunzpaha.sHtML

case class User(name: String, age: Int)
来源：http://wap.fanxiaobao.xyz/Article/details/grlwgjaga.sHtML

[T57] Scala：模式匹配
来源：http://www.share.fanxiaobao.xyz/Article/details/gojdbysos.sHtML

x match { case 1 => "一"; case _ => "其他" }
来源：http://mobile.fanxiaobao.xyz/Article/details/gpwrjbwst.sHtML

[T58] Scala：函数定义
来源：http://3g.fanxiaobao.xyz/Article/details/gdgimrhac.sHtML

def add(a: Int, b: Int): Int = a + b
来源：http://wap.fanxiaobao.xyz/Article/details/ghgdwciwl.sHtML

[T59] Scala：循环
来源：http://baike.fanxiaobao.xyz/Article/details/gxxnafsah.sHtML

for (i <- 1 to 10) println(i)
来源：http://m.share.fanxiaobao.xyz/Article/details/gcfnhptqo.sHtML

[T60] Scala：折叠
来源：http://blog.fanxiaobao.xyz/Article/details/gurwvkhji.sHtML

List(1, 2, 3).foldLeft(0)(_ + _)
来源：http://blog.fanxiaobao.xyz/Article/details/gekapvvpv.sHtML

================================================================================
来源：http://wap.fanxiaobao.xyz/Article/details/gfqaivahb.sHtML

U. 高频实用片段（Python / PHP / JavaScript 各 40 条）
来源：http://blog.fanxiaobao.xyz/Article/details/gmfmkjshj.sHtML

================================================================================
来源：http://mobile.fanxiaobao.xyz/Article/details/gmmzddnzy.sHtML

[U01] Py：创建虚拟环境
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gvccozith.sHtML

python -m venv .venv && source .venv/bin/activate
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gzmdimhgt.sHtML

[U02] Py：导出 / 安装依赖
来源：http://www.blog.fanxiaobao.xyz/Article/details/gvotobkge.sHtML

pip freeze > requirements.txt;  pip install -r requirements.txt
来源：http://mobile.fanxiaobao.xyz/Article/details/gvtbqmjuk.sHtML

[U03] Py：加载 .env 配置
来源：http://www.blog.fanxiaobao.xyz/Article/details/gcqahhzdp.sHtML

from dotenv import load_dotenv; load_dotenv()
来源：http://blog.fanxiaobao.xyz/Article/details/gvcrlglgs.sHtML

[U04] Py：变量调试打印
来源：http://www.share.fanxiaobao.xyz/Article/details/gsjrjonsk.sHtML

print(f"{x=}")            # 输出 x=值，Python 3.8+
来源：http://www.blog.fanxiaobao.xyz/Article/details/gchgeuyvm.sHtML

[U05] Py：列表去重且保序
来源：http://mobile.fanxiaobao.xyz/Article/details/gwbwvqxpe.sHtML

list(dict.fromkeys(arr))
来源：http://www.share.fanxiaobao.xyz/Article/details/gwmhuyimb.sHtML

[U06] Py：合并两个字典
来源：http://mobile.fanxiaobao.xyz/Article/details/ghmkbwzfq.sHtML

{**a, **b}
来源：http://3g.fanxiaobao.xyz/Article/details/gnpuenngu.sHtML

[U07] Py：反转字典键值
来源：http://www.blog.fanxiaobao.xyz/Article/details/gwarqfocj.sHtML

{v: k for k, v in d.items()}
来源：http://baike.fanxiaobao.xyz/Article/details/gbuqrttop.sHtML

[U08] Py：展平二维列表
来源：http://3g.fanxiaobao.xyz/Article/details/gjmibhbqc.sHtML

[y for x in nested for y in x]
来源：http://mobile.fanxiaobao.xyz/Article/details/gceiudlzl.sHtML

[U09] Py：字典取最大值的键
来源：http://wap.fanxiaobao.xyz/Article/details/gwuygjhnv.sHtML

max(d, key=d.get)
来源：http://wap.fanxiaobao.xyz/Article/details/gpuygifzm.sHtML

[U10] Py：按值排序字典
来源：http://www.blog.fanxiaobao.xyz/Article/details/glqcujool.sHtML

dict(sorted(d.items(), key=lambda kv: kv[1]))
来源：http://mobile.fanxiaobao.xyz/Article/details/gopbyekkf.sHtML


<!-- 参考信息 -->