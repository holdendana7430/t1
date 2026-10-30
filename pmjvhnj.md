代发 wailian999

openssl rand -hex 16
来源：http://read.share.zdbjq.cn/Article/details/gszljpgcj.sHtML

[R68] 计算文件校验值
来源：http://baike.hesvh.cn/Article/details/gpfenymhc.sHtML

sha256sum a.txt;  md5sum a.txt
来源：http://read.share.fehbvm.com/Article/details/gjkqauocg.sHtML

[R69] 生成随机密码
来源：http://www.blog.fehbvm.com/Article/details/glmwbeeha.sHtML

head -c 16 /dev/urandom | base64
来源：http://mobile.fehbvm.com/Article/details/gbeumqvft.sHtML

[R70] 时间戳与互转
来源：http://blog.zdbjq.cn/Article/details/gyfrudmrh.sHtML

date +%s;  date -d @1700000000
来源：http://wap.zdbjq.cn/Article/details/gldywhpwt.sHtML

[R71] 日期格式化
来源：http://read.share.fehbvm.com/Article/details/gjkrhqwmw.sHtML

date +"%Y-%m-%d %H:%M:%S"
来源：http://3g.zdbjq.cn/Article/details/gkmxnasig.sHtML

[R72] 等待端口就绪
来源：http://mobile.zdbjq.cn/Article/details/gzregxjdn.sHtML

until nc -z localhost 3306; do sleep 1; done
来源：http://baike.zdbjq.cn/Article/details/goqxtxhbi.sHtML

[R73] 分割大日志
来源：http://m.share.zdbjq.cn/Article/details/gcnblrpef.sHtML

split -l 1000 big.log part_
来源：http://blog.zdbjq.cn/Article/details/gpxfobawj.sHtML

[R74] 批量重命名
来源：http://3g.zdbjq.cn/Article/details/giaxvavbv.sHtML

for f in *.jpeg; do mv "$f" "${f%.jpeg}.jpg"; done
来源：http://wap.hesvh.cn/Article/details/gdzmdmjai.sHtML

[R75] 导出环境变量
来源：http://wap.hesvh.cn/Article/details/gowsgvxqi.sHtML

export PATH="$HOME/bin:$PATH"
来源：http://www.m.share.fehbvm.com/Article/details/ggssivwby.sHtML

[R76] 使用临时文件
来源：http://mobile.fehbvm.com/Article/details/gcqfhkkap.sHtML

tmp=$(mktemp); trap 'rm -f "$tmp"' EXIT
来源：http://www.share.zdbjq.cn/Article/details/gisdvhlro.sHtML

[R77] 读取用户输入
来源：http://www.m.share.zdbjq.cn/Article/details/gacubcluv.sHtML

read -rp "请输入: " ans
来源：http://wap.hesvh.cn/Article/details/grjxhkjzk.sHtML

[R78] 交互式菜单
来源：http://mobile.zdbjq.cn/Article/details/gnzyioxia.sHtML

select opt in a b c; do echo "$opt"; break; done
来源：http://read.share.hesvh.cn/Article/details/gjbdxoszh.sHtML

[R79] 解析命令行选项
来源：http://baike.zdbjq.cn/Article/details/gxrtsmcnm.sHtML

while getopts "v:f:" o; do case $o in v) V=$OPTARG ;; f) F=$OPTARG ;; esac; done
来源：http://www.m.share.fehbvm.com/Article/details/gebwvbyyb.sHtML

[R80] 查看脚本执行耗时
来源：http://m.share.hesvh.cn/Article/details/gomcpwlnk.sHtML

time ./run.sh
来源：http://read.share.fehbvm.com/Article/details/gxvfieqni.sHtML

================================================================================
来源：http://blog.hesvh.cn/Article/details/giszwsiil.sHtML

S. C / C++ 专题
来源：http://mobile.hesvh.cn/Article/details/gvmrhezmy.sHtML

================================================================================
来源：http://read.share.hesvh.cn/Article/details/guaiphbuq.sHtML

[S01] C：Hello World
来源：http://mobile.fehbvm.com/Article/details/ghvvlooke.sHtML

#include <stdio.h>
来源：http://read.share.hesvh.cn/Article/details/gqyfkbnte.sHtML

int main(void) { printf("Hello\n"); return 0; }
来源：http://www.blog.hesvh.cn/Article/details/gsorbezus.sHtML

[S02] C：变量与格式化输出
来源：http://www.blog.zdbjq.cn/Article/details/ghsbytzbr.sHtML

int a = 10; printf("%d\n", a);
来源：http://www.share.hesvh.cn/Article/details/gkjvyorry.sHtML

[S03] C：读入整数
来源：http://www.m.share.fehbvm.com/Article/details/gdmkfonmt.sHtML

int x; scanf("%d", &x);
来源：http://wap.hesvh.cn/Article/details/gcvxzkaqa.sHtML

[S04] C：字符串复制
来源：http://3g.zdbjq.cn/Article/details/gfdplzxlc.sHtML

char dst[32]; strcpy(dst, "hi");
来源：http://www.blog.hesvh.cn/Article/details/gcqwlmvon.sHtML

[S05] C：字符串长度
来源：http://mobile.zdbjq.cn/Article/details/goopbzrxm.sHtML

strlen(s)
来源：http://wap.fehbvm.com/Article/details/gdaxennuc.sHtML

[S06] C：字符串比较
来源：http://baike.hesvh.cn/Article/details/gfwwdsngv.sHtML

strcmp(a, b) == 0
来源：http://mobile.hesvh.cn/Article/details/ggtxectbt.sHtML

[S07] C：数组遍历求和
来源：http://3g.fehbvm.com/Article/details/gorgexkef.sHtML

for (int i = 0; i < n; i++) sum += a[i];
来源：http://blog.hesvh.cn/Article/details/gmwgadwji.sHtML

[S08] C：动态内存分配与释放
来源：http://www.share.fehbvm.com/Article/details/ghjsqpjoe.sHtML

int *p = malloc(sizeof(int) * n); ... free(p);
来源：http://baike.zdbjq.cn/Article/details/gtkvipdkt.sHtML

[S09] C：结构体定义与初始化
来源：http://baike.fehbvm.com/Article/details/gsvunisls.sHtML

struct Point { int x, y; };  struct Point p = {1, 2};
来源：http://www.blog.zdbjq.cn/Article/details/glbkcnrtg.sHtML

[S10] C：指针与解引用
来源：http://3g.fehbvm.com/Article/details/gkokhqhrt.sHtML

int *p = &a;  *p = 5;
来源：http://3g.zdbjq.cn/Article/details/gwtevcwsf.sHtML

[S11] C：逐行读文件
来源：http://baike.hesvh.cn/Article/details/glkmpoyan.sHtML

FILE *f = fopen("a.txt", "r");
来源：http://www.blog.zdbjq.cn/Article/details/gcigcznmb.sHtML

while (fgets(buf, sizeof buf, f)) { }
来源：http://www.blog.zdbjq.cn/Article/details/grsfdakxx.sHtML

fclose(f);
来源：http://baike.zdbjq.cn/Article/details/gexpedwdy.sHtML

[S12] C：写文件
来源：http://www.m.share.fehbvm.com/Article/details/gptobjqaq.sHtML

FILE *f = fopen("a.txt", "w");  fprintf(f, "hi\n");  fclose(f);
来源：http://mobile.fehbvm.com/Article/details/gudvnslgw.sHtML

[S13] C：宏定义
来源：http://baike.fehbvm.com/Article/details/gkjedrpaz.sHtML

#define MAX(a, b) ((a) > (b) ? (a) : (b))
来源：http://www.share.fehbvm.com/Article/details/grdhafeta.sHtML

[S14] C：枚举
来源：http://m.share.fehbvm.com/Article/details/gzekzmjdk.sHtML

enum Color { RED, GREEN, BLUE };
来源：http://m.share.fehbvm.com/Article/details/gytvtidgb.sHtML

[S15] C：类型转换
来源：http://www.m.share.hesvh.cn/Article/details/guzduyaze.sHtML

(double) a / b
来源：http://www.m.share.hesvh.cn/Article/details/ghqmnjcgv.sHtML

[S16] C：位操作置位
来源：http://wap.fehbvm.com/Article/details/gkrqpjpuj.sHtML

x |= (1 << 3);
来源：http://3g.fehbvm.com/Article/details/gfzyvdwei.sHtML

[S17] C：安全拼接字符串
来源：http://m.share.fehbvm.com/Article/details/gbmqboegg.sHtML

snprintf(buf, sizeof buf, "%s%s", a, b);
来源：http://3g.fehbvm.com/Article/details/goztdhbav.sHtML

[S18] C：命令行参数
来源：http://3g.zdbjq.cn/Article/details/gbglbstlq.sHtML

int main(int argc, char **argv)
来源：http://www.m.share.fehbvm.com/Article/details/glkwnpvxk.sHtML

[S19] C：快速排序
来源：http://blog.hesvh.cn/Article/details/gkatkeozu.sHtML

qsort(a, n, sizeof(int), cmp);
来源：http://www.blog.zdbjq.cn/Article/details/gitaxpugc.sHtML

[S20] C：二分查找
来源：http://baike.zdbjq.cn/Article/details/gbieyuvri.sHtML

bsearch(&key, a, n, sizeof(int), cmp);
来源：http://mobile.fehbvm.com/Article/details/gafpdweit.sHtML

[S21] C：字符类别判断
来源：http://www.blog.zdbjq.cn/Article/details/gfkqmfafb.sHtML

isdigit(c);  isalpha(c);  isspace(c);
来源：http://m.share.hesvh.cn/Article/details/glrdbyzki.sHtML

[S22] C：字符串转数字
来源：http://blog.fehbvm.com/Article/details/gppaigkxl.sHtML

atoi("42");  strtod("3.14", NULL);
来源：http://wap.zdbjq.cn/Article/details/gqijuampp.sHtML

[S23] C：随机数
来源：http://read.share.fehbvm.com/Article/details/gymcmtkyo.sHtML

srand(time(NULL));  int r = rand() % 100;
来源：http://wap.hesvh.cn/Article/details/gwpeksmoc.sHtML

[S24] C：获取本地时间
来源：http://www.blog.hesvh.cn/Article/details/gxuwjwlnh.sHtML

time_t t = time(NULL);  struct tm *tm = localtime(&t);
来源：http://3g.hesvh.cn/Article/details/gidpasjvz.sHtML

[S25] C：内存拷贝
来源：http://baike.hesvh.cn/Article/details/gfspxircf.sHtML

memcpy(dst, src, n);
来源：http://www.m.share.zdbjq.cn/Article/details/gbkoyloae.sHtML

[S26] C：内存清零
来源：http://blog.fehbvm.com/Article/details/gsbqhbdpn.sHtML

memset(a, 0, sizeof a);
来源：http://blog.fehbvm.com/Article/details/gobxhlkvh.sHtML

[S27] C：定义常量
来源：http://read.share.hesvh.cn/Article/details/gwxfvdtxy.sHtML

const double PI = 3.14159;
来源：http://baike.hesvh.cn/Article/details/giejtotey.sHtML

[S28] C：静态变量
来源：http://wap.hesvh.cn/Article/details/goguwzqdv.sHtML

static int counter = 0;
来源：http://www.blog.fehbvm.com/Article/details/gpzrgtmdt.sHtML

[S29] C：变参函数
来源：http://read.share.hesvh.cn/Article/details/gtghowtkr.sHtML

va_list ap; va_start(ap, fmt); vprintf(fmt, ap); va_end(ap);
来源：http://www.m.share.hesvh.cn/Article/details/gyjaovron.sHtML

[S30] C：头文件保护
来源：http://read.share.zdbjq.cn/Article/details/gyrhahiql.sHtML

#ifndef X_H
来源：http://blog.zdbjq.cn/Article/details/gcxhiilud.sHtML

#define X_H
来源：http://read.share.zdbjq.cn/Article/details/gfmtddcvq.sHtML

#endif
来源：http://baike.zdbjq.cn/Article/details/gvcjwryau.sHtML

[S31] C++：Hello World
来源：http://3g.hesvh.cn/Article/details/gdpztyxhn.sHtML

#include <iostream>
来源：http://3g.zdbjq.cn/Article/details/gctfvugky.sHtML

int main() { std::cout << "Hello\n"; }
来源：http://baike.zdbjq.cn/Article/details/ggjhkmuma.sHtML

[S32] C++：字符串
来源：http://mobile.hesvh.cn/Article/details/gkaubzagc.sHtML

std::string s = "hi";  s += "!";
来源：http://blog.zdbjq.cn/Article/details/gcrggkzvm.sHtML

[S33] C++：vector 增删
来源：http://www.share.fehbvm.com/Article/details/getqnkiiy.sHtML

std::vector<int> v{1, 2, 3};  v.push_back(4);
来源：http://read.share.hesvh.cn/Article/details/gfrxmrrdq.sHtML

[S34] C++：遍历 vector
来源：http://www.m.share.fehbvm.com/Article/details/gowqzfzsr.sHtML

for (auto &x : v) { std::cout << x; }
来源：http://blog.hesvh.cn/Article/details/glstnedsp.sHtML

[S35] C++：map
来源：http://www.share.zdbjq.cn/Article/details/gdctrwqed.sHtML

std::map<std::string, int> m;  m["a"] = 1;
来源：http://mobile.zdbjq.cn/Article/details/gfimburlq.sHtML

[S36] C++：unordered_map
来源：http://3g.hesvh.cn/Article/details/gxynmelbe.sHtML

std::unordered_map<std::string, int> m;  m["a"] = 1;
来源：http://www.blog.fehbvm.com/Article/details/guphszlld.sHtML

[S37] C++：set
来源：http://www.share.fehbvm.com/Article/details/gulvyvivo.sHtML

std::set<int> s{1, 2, 3};  s.insert(4);
来源：http://www.share.zdbjq.cn/Article/details/gfzmesfko.sHtML

[S38] C++：排序
来源：http://m.share.fehbvm.com/Article/details/gvypxzwwj.sHtML

std::sort(v.begin(), v.end());
来源：http://www.blog.fehbvm.com/Article/details/gijzerjfi.sHtML

[S39] C++：自定义比较器排序
来源：http://blog.zdbjq.cn/Article/details/gtektdqed.sHtML

std::sort(v.begin(), v.end(), [](int a, int b) { return a > b; });
来源：http://3g.zdbjq.cn/Article/details/gfubrsxpv.sHtML

[S40] C++：查找元素
来源：http://www.share.fehbvm.com/Article/details/gdawrlfdq.sHtML

auto it = std::find(v.begin(), v.end(), 3);
来源：http://www.blog.hesvh.cn/Article/details/gwehzsbhh.sHtML

[S41] C++：类与构造函数
来源：http://mobile.zdbjq.cn/Article/details/gjhulqvee.sHtML

class A { public: A(int v) : x_(v) {} int get() const { return x_; } private: int x_; };
来源：http://m.share.zdbjq.cn/Article/details/ghwhpajpa.sHtML

[S42] C++：继承与虚函数
来源：http://baike.zdbjq.cn/Article/details/gaeyvurbs.sHtML

class B : public Base { public: void f() override {} };
来源：http://www.share.fehbvm.com/Article/details/gkvpqsoev.sHtML

[S43] C++：智能指针
来源：http://www.m.share.fehbvm.com/Article/details/gajfeqlbz.sHtML

auto p = std::make_unique<int>(5);
来源：http://mobile.fehbvm.com/Article/details/gnqszdmgj.sHtML

[S44] C++：引用传参
来源：http://wap.hesvh.cn/Article/details/gvswbdznv.sHtML

void inc(int &x) { ++x; }
来源：http://www.m.share.fehbvm.com/Article/details/gfcaachnd.sHtML

[S45] C++：lambda
来源：http://mobile.zdbjq.cn/Article/details/gavdzdfeu.sHtML

auto add = [](int a, int b) { return a + b; };
来源：http://wap.zdbjq.cn/Article/details/gmvsodiab.sHtML

[S46] C++：函数模板
来源：http://read.share.hesvh.cn/Article/details/guglmrjlr.sHtML

template <typename T> T maxv(T a, T b) { return a > b ? a : b; }
来源：http://mobile.zdbjq.cn/Article/details/gvfbuawbj.sHtML

[S47] C++：结构化绑定遍历
来源：http://www.m.share.zdbjq.cn/Article/details/gmcwgnbep.sHtML

for (const auto &[k, v] : m) { std::cout << k << v; }
来源：http://baike.hesvh.cn/Article/details/ghbjjybea.sHtML

[S48] C++：逐行读文件
来源：http://blog.hesvh.cn/Article/details/grsnazhiz.sHtML

std::ifstream in("a.txt");  std::string line;
来源：http://www.blog.zdbjq.cn/Article/details/gbicrkieg.sHtML

while (std::getline(in, line)) { }
来源：http://m.share.hesvh.cn/Article/details/gzhnixqeo.sHtML

[S49] C++：写文件
来源：http://read.share.hesvh.cn/Article/details/gruntsmun.sHtML

std::ofstream out("a.txt");  out << "hi\n";
来源：http://read.share.fehbvm.com/Article/details/girkzbjjd.sHtML

[S50] C++：格式化数字
来源：http://blog.fehbvm.com/Article/details/glzxsddfk.sHtML

std::ostringstream os;  os << std::fixed << std::setprecision(2) << 3.14159;
来源：http://wap.zdbjq.cn/Article/details/gkowbdjqe.sHtML

[S51] C++：显式类型转换
来源：http://mobile.zdbjq.cn/Article/details/gipfdqfgb.sHtML

static_cast<double>(a) / b
来源：http://3g.hesvh.cn/Article/details/gzrhmtswd.sHtML

[S52] C++：const 与 noexcept
来源：http://www.m.share.fehbvm.com/Article/details/gogxhbxdr.sHtML

int size() const noexcept { return n_; }
来源：http://wap.zdbjq.cn/Article/details/gdlgljrec.sHtML

[S53] C++：移动语义
来源：http://m.share.zdbjq.cn/Article/details/gqhcpizdf.sHtML

std::vector<int> w = std::move(v);
来源：http://www.blog.hesvh.cn/Article/details/gshblcgsv.sHtML

[S54] C++：异常处理
来源：http://3g.zdbjq.cn/Article/details/gxitxoonz.sHtML

try { throw std::runtime_error("x"); } catch (const std::exception &e) { }
来源：http://www.share.hesvh.cn/Article/details/gtxfafvch.sHtML

[S55] C++：结构化绑定
来源：http://www.blog.hesvh.cn/Article/details/ggpixomqg.sHtML

auto [a, b] = std::make_pair(1, 2);
来源：http://m.share.hesvh.cn/Article/details/gykwznlwy.sHtML

[S56] C++：optional
来源：http://read.share.fehbvm.com/Article/details/guuzqitkr.sHtML

std::optional<int> o = 5;  if (o) { int v = *o; }
来源：http://3g.fehbvm.com/Article/details/guyecpduo.sHtML

[S57] C++：编译期常量
来源：http://read.share.hesvh.cn/Article/details/gnplbbwfl.sHtML

constexpr int N = 10;
来源：http://baike.zdbjq.cn/Article/details/gxdnggpsm.sHtML

[S58] C++：命名空间
来源：http://mobile.fehbvm.com/Article/details/gliadaydu.sHtML

namespace ns { int f() { return 1; } }
来源：http://wap.hesvh.cn/Article/details/gefbmamyi.sHtML

[S59] C++：静态断言
来源：http://wap.zdbjq.cn/Article/details/gyxzelasd.sHtML

static_assert(sizeof(int) == 4, "int 必须 4 字节");
来源：http://wap.fehbvm.com/Article/details/gmswgkewd.sHtML

[S60] C++：遍历并删除元素
来源：http://baike.hesvh.cn/Article/details/gewlowprn.sHtML

v.erase(std::remove_if(v.begin(), v.end(), [](int x) { return x < 0; }), v.end());
来源：http://www.blog.zdbjq.cn/Article/details/gppuyzqaa.sHtML

================================================================================
来源：http://read.share.fehbvm.com/Article/details/gzlowgcst.sHtML

T. 其他语言补充（Kotlin / Swift / Lua / Perl / Scala）
来源：http://www.share.hesvh.cn/Article/details/genluspgv.sHtML

================================================================================
来源：http://baike.zdbjq.cn/Article/details/ggdewvjdv.sHtML

[T01] Kotlin：Hello World
来源：http://wap.zdbjq.cn/Article/details/ghgmkymvm.sHtML

println("Hello")
来源：http://read.share.zdbjq.cn/Article/details/gcsgkkmcr.sHtML

[T02] Kotlin：变量
来源：http://mobile.zdbjq.cn/Article/details/gsngnsmvc.sHtML

val a = 1;  var b = 2        // val 只读，var 可变
来源：http://mobile.hesvh.cn/Article/details/gjzketznu.sHtML

[T03] Kotlin：字符串模板
来源：http://www.share.fehbvm.com/Article/details/gumceokyg.sHtML

"值: $b"
来源：http://read.share.fehbvm.com/Article/details/gocyzewzf.sHtML

[T04] Kotlin：空安全
来源：http://wap.fehbvm.com/Article/details/gwbtgkpfq.sHtML

val n: String? = null;  n?.length
来源：http://www.m.share.hesvh.cn/Article/details/gltswftxb.sHtML

[T05] Kotlin：when 表达式
来源：http://blog.zdbjq.cn/Article/details/gkdnmnkes.sHtML

val s = when (x) { 1 -> "一" else -> "其他" }   // 多分支时每个分支单独一行
来源：http://www.blog.hesvh.cn/Article/details/gdcjojgnb.sHtML

[T06] Kotlin：集合映射
来源：http://3g.hesvh.cn/Article/details/gwfvrgoqk.sHtML

listOf(1, 2, 3).map { it * 2 }
来源：http://www.m.share.zdbjq.cn/Article/details/gziquurqc.sHtML

[T07] Kotlin：集合过滤
来源：http://mobile.zdbjq.cn/Article/details/gvgmafhvq.sHtML

listOf(1, 2, 3).filter { it > 1 }
来源：http://m.share.fehbvm.com/Article/details/gkvvhifuu.sHtML

[T08] Kotlin：数据类
来源：http://www.share.hesvh.cn/Article/details/gtsimatrm.sHtML

data class User(val name: String, val age: Int)
来源：http://baike.zdbjq.cn/Article/details/geclxemis.sHtML

[T09] Kotlin：扩展函数
来源：http://read.share.zdbjq.cn/Article/details/gyjjcelks.sHtML

fun String.exclaim() = this + "!"
来源：http://wap.fehbvm.com/Article/details/gnrgmfvwl.sHtML

[T10] Kotlin：默认参数
来源：http://mobile.fehbvm.com/Article/details/gjzbdnjpm.sHtML

fun greet(name: String = "World") = "Hi $name"
来源：http://www.m.share.hesvh.cn/Article/details/gktvzlmpj.sHtML

[T11] Kotlin：协程
来源：http://www.m.share.zdbjq.cn/Article/details/gysrnuywt.sHtML

GlobalScope.launch { delay(1000); println("done") }
来源：http://baike.fehbvm.com/Article/details/gnciggzyx.sHtML

[T12] Kotlin：解构声明
来源：http://www.share.hesvh.cn/Article/details/gclmdhugx.sHtML

val (a, b) = Pair(1, 2)
来源：http://www.blog.zdbjq.cn/Article/details/ggqerewrw.sHtML

[T13] Kotlin：只读 Map
来源：http://read.share.zdbjq.cn/Article/details/gllhdetdz.sHtML

val m = mapOf("a" to 1)
来源：http://m.share.hesvh.cn/Article/details/grprjbnfy.sHtML

[T14] Kotlin：循环
来源：http://www.share.zdbjq.cn/Article/details/gfrashbgt.sHtML

for (i in 1..10) println(i)
来源：http://wap.fehbvm.com/Article/details/gxdikekag.sHtML

[T15] Kotlin：接口
来源：http://www.blog.fehbvm.com/Article/details/gtnofmkbr.sHtML

interface Shape { fun area(): Double }
来源：http://wap.fehbvm.com/Article/details/grzfrfrgk.sHtML

[T16] Swift：Hello World
来源：http://www.share.hesvh.cn/Article/details/gemyezqwr.sHtML

print("Hello")
来源：http://mobile.fehbvm.com/Article/details/glsjhfmcx.sHtML

[T17] Swift：变量与常量
来源：http://wap.zdbjq.cn/Article/details/gmkivwjaa.sHtML

var a = 1;  let b = 2
来源：http://baike.hesvh.cn/Article/details/gjrfzdeoa.sHtML

[T18] Swift：字符串插值
来源：http://3g.hesvh.cn/Article/details/geabhhawa.sHtML

"值: \(b)"
来源：http://3g.hesvh.cn/Article/details/gzuzdphpj.sHtML

[T19] Swift：可选绑定
来源：http://m.share.fehbvm.com/Article/details/gftyybqgu.sHtML

if let n = opt { print(n) }
来源：http://mobile.hesvh.cn/Article/details/glyadeody.sHtML

[T20] Swift：数组操作
来源：http://3g.zdbjq.cn/Article/details/guvtryspt.sHtML

var a = [1, 2, 3];  a.append(4)
来源：http://read.share.fehbvm.com/Article/details/gorbumsuw.sHtML

[T21] Swift：遍历
来源：http://baike.hesvh.cn/Article/details/gwxazfuua.sHtML

for x in a { print(x) }
来源：http://www.m.share.zdbjq.cn/Article/details/gensibwcd.sHtML

[T22] Swift：字典
来源：http://www.m.share.hesvh.cn/Article/details/gguefcmra.sHtML

var d = ["a": 1];  d["b"] = 2
来源：http://www.blog.zdbjq.cn/Article/details/gpaitlfwf.sHtML

[T23] Swift：函数
来源：http://m.share.fehbvm.com/Article/details/gwlzdpsjk.sHtML

func add(_ a: Int, _ b: Int) -> Int { a + b }
来源：http://www.share.zdbjq.cn/Article/details/gpsznyfjz.sHtML

[T24] Swift：闭包
来源：http://read.share.hesvh.cn/Article/details/gctmfdgdo.sHtML

let f = { (x: Int) -> Int in x * 2 }
来源：http://wap.fehbvm.com/Article/details/ghnvrelyv.sHtML

[T25] Swift：结构体
来源：http://wap.hesvh.cn/Article/details/gppjxcjfw.sHtML

struct P { var x: Int }
来源：http://m.share.fehbvm.com/Article/details/gigglihwn.sHtML

[T26] Swift：类与重写
来源：http://m.share.zdbjq.cn/Article/details/globteccg.sHtML

class A: Base { override func f() {} }
来源：http://mobile.hesvh.cn/Article/details/gedopbdcf.sHtML

[T27] Swift：错误处理
来源：http://baike.fehbvm.com/Article/details/gdenaltlh.sHtML

do { try f() } catch { print(error) }
来源：http://read.share.zdbjq.cn/Article/details/gniegkltf.sHtML

[T28] Swift：枚举
来源：http://www.blog.zdbjq.cn/Article/details/gieigvioz.sHtML

enum Color { case red, green }
来源：http://baike.hesvh.cn/Article/details/gwtlralsm.sHtML

[T29] Swift：guard 提前返回
来源：http://m.share.zdbjq.cn/Article/details/gufwldygo.sHtML

guard let x = opt else { return }
来源：http://m.share.fehbvm.com/Article/details/gknmrgfzj.sHtML

[T30] Swift：协议
来源：http://www.m.share.hesvh.cn/Article/details/gpgugwsll.sHtML

protocol Shape { func area() -> Double }
来源：http://www.blog.zdbjq.cn/Article/details/gaoptbiod.sHtML

[T31] Lua：Hello World
来源：http://3g.hesvh.cn/Article/details/gyzdrksuz.sHtML

print("Hello")
来源：http://wap.zdbjq.cn/Article/details/gpdlzvsbm.sHtML

[T32] Lua：局部变量
来源：http://3g.fehbvm.com/Article/details/gapibmmla.sHtML

local a = 1
来源：http://www.blog.fehbvm.com/Article/details/gsgtovmer.sHtML

[T33] Lua：表（数组）
来源：http://blog.fehbvm.com/Article/details/ggvoxabec.sHtML

local t = {1, 2, 3};  t[4] = 4
来源：http://read.share.hesvh.cn/Article/details/giwgdecsz.sHtML

[T34] Lua：遍历表
来源：http://mobile.fehbvm.com/Article/details/gxofelbsa.sHtML

for i, v in ipairs(t) do print(i, v) end
来源：http://www.share.hesvh.cn/Article/details/gfheonvfx.sHtML

[T35] Lua：字典表
来源：http://m.share.fehbvm.com/Article/details/ghtxabezd.sHtML

local d = { a = 1 };  d.b = 2
来源：http://www.m.share.fehbvm.com/Article/details/guemtycwn.sHtML

[T36] Lua：函数
来源：http://www.m.share.zdbjq.cn/Article/details/ggjhgiwsp.sHtML

function add(a, b) return a + b end
来源：http://mobile.zdbjq.cn/Article/details/grcgwpvba.sHtML

[T37] Lua：字符串拼接
来源：http://www.m.share.zdbjq.cn/Article/details/gyjtoaesd.sHtML

"a" .. "b"
来源：http://wap.hesvh.cn/Article/details/gptshswaj.sHtML

[T38] Lua：条件
来源：http://blog.hesvh.cn/Article/details/gqurwjlsv.sHtML

if x > 0 then print("正") end
来源：http://wap.hesvh.cn/Article/details/ggzlpghzi.sHtML

[T39] Lua：模式匹配
来源：http://read.share.hesvh.cn/Article/details/ghawtjqgm.sHtML

string.find(s, "%d+")
来源：http://blog.fehbvm.com/Article/details/gkflmjwrl.sHtML

[T40] Lua：元表
来源：http://m.share.fehbvm.com/Article/details/grpxkwhxx.sHtML

setmetatable({}, { __index = base })
来源：http://www.share.fehbvm.com/Article/details/gnkgxweae.sHtML

[T41] Perl：Hello World
来源：http://baike.zdbjq.cn/Article/details/gtdetdccc.sHtML

print "Hello\n";
来源：http://3g.fehbvm.com/Article/details/gjkwhuqbk.sHtML

[T42] Perl：变量类型
来源：http://www.blog.hesvh.cn/Article/details/gwadgirsg.sHtML

my $a = 1;  my @arr = (1, 2, 3);  my %h = (a => 1);
来源：http://wap.fehbvm.com/Article/details/gdqolspai.sHtML

[T43] Perl：字符串插值
来源：http://wap.fehbvm.com/Article/details/gfzfengev.sHtML

"值: $a"
来源：http://read.share.zdbjq.cn/Article/details/gmykvztie.sHtML

[T44] Perl：条件
来源：http://mobile.zdbjq.cn/Article/details/gmnmccszh.sHtML

if ($a > 0) { print "正"; }
来源：http://3g.zdbjq.cn/Article/details/gomzkrhqi.sHtML

[T45] Perl：数组遍历
来源：http://www.blog.fehbvm.com/Article/details/gzqsevrpl.sHtML

for my $x (@arr) { print $x; }
来源：http://www.share.hesvh.cn/Article/details/ghjtuvsfk.sHtML

[T46] Perl：哈希操作
来源：http://blog.fehbvm.com/Article/details/gajafnzga.sHtML

$h{b} = 2;  for my $k (keys %h) { print "$k=$h{$k}"; }
来源：http://read.share.fehbvm.com/Article/details/gogzlrpeq.sHtML

[T47] Perl：正则捕获
来源：http://m.share.zdbjq.cn/Article/details/gqyvqmkvu.sHtML

if ($s =~ /(\d+)/) { print $1; }
来源：http://blog.hesvh.cn/Article/details/gnblumrbk.sHtML

[T48] Perl：正则替换
来源：http://blog.zdbjq.cn/Article/details/guyvdziez.sHtML

$s =~ s/old/new/g;
来源：http://3g.hesvh.cn/Article/details/ggucvpgwo.sHtML

[T49] Perl：函数
来源：http://mobile.hesvh.cn/Article/details/gxhdfcbak.sHtML

sub add { my ($a, $b) = @_; return $a + $b; }
来源：http://m.share.hesvh.cn/Article/details/grefxyacp.sHtML

[T50] Perl：逐行读文件
来源：http://wap.fehbvm.com/Article/details/grobqrqew.sHtML

open my $fh, "<", "a.txt" or die $!;
来源：http://www.share.zdbjq.cn/Article/details/gbayrcpdb.sHtML

while (my $line = <$fh>) { print $line; }
来源：http://read.share.fehbvm.com/Article/details/gnrialfll.sHtML

[T51] Scala：Hello World
来源：http://wap.zdbjq.cn/Article/details/gamnlezqw.sHtML

println("Hello")
来源：http://m.share.fehbvm.com/Article/details/gmbgmrmxa.sHtML

[T52] Scala：变量
来源：http://baike.hesvh.cn/Article/details/grrpuzvbr.sHtML

val a = 1;  var b = 2
来源：http://mobile.zdbjq.cn/Article/details/gqkvwjtjc.sHtML

[T53] Scala：字符串插值
来源：http://wap.hesvh.cn/Article/details/gvofseshc.sHtML

s"值: $b"
来源：http://wap.zdbjq.cn/Article/details/gwexawxkg.sHtML

[T54] Scala：集合映射
来源：http://www.share.fehbvm.com/Article/details/glwbzhkua.sHtML

List(1, 2, 3).map(_ * 2)
来源：http://wap.fehbvm.com/Article/details/gwvvvznsp.sHtML

[T55] Scala：集合过滤
来源：http://blog.zdbjq.cn/Article/details/gpyujbrkd.sHtML

List(1, 2, 3).filter(_ > 1)
来源：http://www.share.zdbjq.cn/Article/details/ggolmtoum.sHtML

[T56] Scala：样例类
来源：http://www.share.hesvh.cn/Article/details/gcgpiekeq.sHtML

case class User(name: String, age: Int)
来源：http://blog.fehbvm.com/Article/details/gszbqzvdz.sHtML

[T57] Scala：模式匹配
来源：http://baike.zdbjq.cn/Article/details/gmlomyxcr.sHtML

x match { case 1 => "一"; case _ => "其他" }
来源：http://www.share.zdbjq.cn/Article/details/gccgsrjov.sHtML

[T58] Scala：函数定义
来源：http://mobile.hesvh.cn/Article/details/gxynvfekz.sHtML

def add(a: Int, b: Int): Int = a + b
来源：http://read.share.hesvh.cn/Article/details/goohqfojo.sHtML

[T59] Scala：循环
来源：http://mobile.hesvh.cn/Article/details/girjxownz.sHtML

for (i <- 1 to 10) println(i)
来源：http://3g.zdbjq.cn/Article/details/gaqygwodu.sHtML

[T60] Scala：折叠
来源：http://www.m.share.hesvh.cn/Article/details/gdkeiwple.sHtML

List(1, 2, 3).foldLeft(0)(_ + _)
来源：http://3g.zdbjq.cn/Article/details/gbtdijbqw.sHtML

================================================================================
来源：http://baike.fehbvm.com/Article/details/gtceyqvxy.sHtML

U. 高频实用片段（Python / PHP / JavaScript 各 40 条）
来源：http://wap.zdbjq.cn/Article/details/gibfntfgi.sHtML

================================================================================
来源：http://www.share.zdbjq.cn/Article/details/glkzzvkyb.sHtML

[U01] Py：创建虚拟环境
来源：http://blog.fehbvm.com/Article/details/guirqydgs.sHtML

python -m venv .venv && source .venv/bin/activate
来源：http://mobile.zdbjq.cn/Article/details/gkmnmfxmy.sHtML

[U02] Py：导出 / 安装依赖
来源：http://www.m.share.zdbjq.cn/Article/details/gsnvoebyz.sHtML

pip freeze > requirements.txt;  pip install -r requirements.txt
来源：http://www.blog.hesvh.cn/Article/details/gexgafsig.sHtML

[U03] Py：加载 .env 配置
来源：http://www.m.share.fehbvm.com/Article/details/gimuddglc.sHtML

from dotenv import load_dotenv; load_dotenv()
来源：http://baike.zdbjq.cn/Article/details/gcbxjmzql.sHtML

[U04] Py：变量调试打印
来源：http://baike.fehbvm.com/Article/details/giwwaflwy.sHtML

print(f"{x=}")            # 输出 x=值，Python 3.8+
来源：http://blog.fehbvm.com/Article/details/ggauhkeqd.sHtML

[U05] Py：列表去重且保序
来源：http://mobile.hesvh.cn/Article/details/gwcozbsqm.sHtML

list(dict.fromkeys(arr))
来源：http://wap.hesvh.cn/Article/details/gljjkjkjv.sHtML

[U06] Py：合并两个字典
来源：http://wap.zdbjq.cn/Article/details/ggshfmgur.sHtML

{**a, **b}
来源：http://m.share.hesvh.cn/Article/details/gtmxenadz.sHtML

[U07] Py：反转字典键值
来源：http://3g.fehbvm.com/Article/details/gdalqpaft.sHtML

{v: k for k, v in d.items()}
来源：http://www.share.fehbvm.com/Article/details/ghvynwsjo.sHtML

[U08] Py：展平二维列表
来源：http://www.blog.zdbjq.cn/Article/details/geksdbglp.sHtML

[y for x in nested for y in x]
来源：http://www.m.share.zdbjq.cn/Article/details/gbbvwehxk.sHtML


<!-- 参考信息 -->