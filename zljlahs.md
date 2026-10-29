代发 wailian999

openssl rand -hex 16
来源：http://mobile.zdbjq.cn/Article/details/gfphnygig.sHtML

[R68] 计算文件校验值
来源：http://www.share.fehbvm.com/Article/details/gqurzgxbq.sHtML

sha256sum a.txt;  md5sum a.txt
来源：http://www.blog.zdbjq.cn/Article/details/gpjwqkxdy.sHtML

[R69] 生成随机密码
来源：http://blog.hesvh.cn/Article/details/gldtyyrdn.sHtML

head -c 16 /dev/urandom | base64
来源：http://m.share.zdbjq.cn/Article/details/goeltflic.sHtML

[R70] 时间戳与互转
来源：http://m.share.zdbjq.cn/Article/details/gwtfmkife.sHtML

date +%s;  date -d @1700000000
来源：http://blog.zdbjq.cn/Article/details/gdjmeygmr.sHtML

[R71] 日期格式化
来源：http://3g.zdbjq.cn/Article/details/gxjpezzji.sHtML

date +"%Y-%m-%d %H:%M:%S"
来源：http://baike.zdbjq.cn/Article/details/gbizzgikw.sHtML

[R72] 等待端口就绪
来源：http://www.m.share.fehbvm.com/Article/details/gjkprqrcv.sHtML

until nc -z localhost 3306; do sleep 1; done
来源：http://read.share.zdbjq.cn/Article/details/gzwcfzpcb.sHtML

[R73] 分割大日志
来源：http://m.share.fehbvm.com/Article/details/gsriwclvx.sHtML

split -l 1000 big.log part_
来源：http://www.m.share.fehbvm.com/Article/details/ggwxyjdjz.sHtML

[R74] 批量重命名
来源：http://3g.hesvh.cn/Article/details/gdloddkjw.sHtML

for f in *.jpeg; do mv "$f" "${f%.jpeg}.jpg"; done
来源：http://3g.hesvh.cn/Article/details/gpyjzyzuf.sHtML

[R75] 导出环境变量
来源：http://www.share.hesvh.cn/Article/details/gglfqzotd.sHtML

export PATH="$HOME/bin:$PATH"
来源：http://www.share.hesvh.cn/Article/details/gqdkrjvag.sHtML

[R76] 使用临时文件
来源：http://www.blog.fehbvm.com/Article/details/gyranhrbr.sHtML

tmp=$(mktemp); trap 'rm -f "$tmp"' EXIT
来源：http://www.m.share.hesvh.cn/Article/details/gleeakzmk.sHtML

[R77] 读取用户输入
来源：http://mobile.fehbvm.com/Article/details/gmftclsek.sHtML

read -rp "请输入: " ans
来源：http://mobile.hesvh.cn/Article/details/gtdqrkhmg.sHtML

[R78] 交互式菜单
来源：http://mobile.zdbjq.cn/Article/details/gufhndpbb.sHtML

select opt in a b c; do echo "$opt"; break; done
来源：http://m.share.hesvh.cn/Article/details/gbcxmdwvs.sHtML

[R79] 解析命令行选项
来源：http://www.blog.hesvh.cn/Article/details/gydrbwfmt.sHtML

while getopts "v:f:" o; do case $o in v) V=$OPTARG ;; f) F=$OPTARG ;; esac; done
来源：http://blog.fehbvm.com/Article/details/gpgtteigw.sHtML

[R80] 查看脚本执行耗时
来源：http://wap.hesvh.cn/Article/details/gkqcmvcct.sHtML

time ./run.sh
来源：http://baike.fehbvm.com/Article/details/gqsmfbxdi.sHtML

================================================================================
来源：http://wap.fehbvm.com/Article/details/grifpjcse.sHtML

S. C / C++ 专题
来源：http://www.m.share.zdbjq.cn/Article/details/gsyjqcbbz.sHtML

================================================================================
来源：http://www.share.hesvh.cn/Article/details/gcvxdzlsw.sHtML

[S01] C：Hello World
来源：http://mobile.zdbjq.cn/Article/details/glpqtslvi.sHtML

#include <stdio.h>
来源：http://www.blog.zdbjq.cn/Article/details/gffbivxgt.sHtML

int main(void) { printf("Hello\n"); return 0; }
来源：http://www.blog.fehbvm.com/Article/details/gwuufrlpn.sHtML

[S02] C：变量与格式化输出
来源：http://mobile.hesvh.cn/Article/details/ggenbkuri.sHtML

int a = 10; printf("%d\n", a);
来源：http://baike.hesvh.cn/Article/details/gffrbtreg.sHtML

[S03] C：读入整数
来源：http://3g.fehbvm.com/Article/details/gklfsjhsn.sHtML

int x; scanf("%d", &x);
来源：http://read.share.hesvh.cn/Article/details/giffqksur.sHtML

[S04] C：字符串复制
来源：http://baike.hesvh.cn/Article/details/geppnzbee.sHtML

char dst[32]; strcpy(dst, "hi");
来源：http://m.share.hesvh.cn/Article/details/gqbhbbarf.sHtML

[S05] C：字符串长度
来源：http://m.share.hesvh.cn/Article/details/gvpsjdpfo.sHtML

strlen(s)
来源：http://m.share.hesvh.cn/Article/details/gekgyvidv.sHtML

[S06] C：字符串比较
来源：http://baike.fehbvm.com/Article/details/gstqmfesm.sHtML

strcmp(a, b) == 0
来源：http://m.share.hesvh.cn/Article/details/gfcbescew.sHtML

[S07] C：数组遍历求和
来源：http://www.share.hesvh.cn/Article/details/gppwuovxj.sHtML

for (int i = 0; i < n; i++) sum += a[i];
来源：http://www.m.share.fehbvm.com/Article/details/gjaducmzj.sHtML

[S08] C：动态内存分配与释放
来源：http://mobile.hesvh.cn/Article/details/gpndjpxne.sHtML

int *p = malloc(sizeof(int) * n); ... free(p);
来源：http://www.share.hesvh.cn/Article/details/gjefxfdrp.sHtML

[S09] C：结构体定义与初始化
来源：http://www.blog.hesvh.cn/Article/details/gshtucgsl.sHtML

struct Point { int x, y; };  struct Point p = {1, 2};
来源：http://m.share.hesvh.cn/Article/details/gtnkcbzek.sHtML

[S10] C：指针与解引用
来源：http://read.share.fehbvm.com/Article/details/gozjvcidh.sHtML

int *p = &a;  *p = 5;
来源：http://m.share.zdbjq.cn/Article/details/goabtcobq.sHtML

[S11] C：逐行读文件
来源：http://www.share.zdbjq.cn/Article/details/gwslndatd.sHtML

FILE *f = fopen("a.txt", "r");
来源：http://www.share.hesvh.cn/Article/details/gswwxvpow.sHtML

while (fgets(buf, sizeof buf, f)) { }
来源：http://3g.hesvh.cn/Article/details/gptfbgogi.sHtML

fclose(f);
来源：http://www.m.share.fehbvm.com/Article/details/glzodofjz.sHtML

[S12] C：写文件
来源：http://www.blog.zdbjq.cn/Article/details/gldxvhqyt.sHtML

FILE *f = fopen("a.txt", "w");  fprintf(f, "hi\n");  fclose(f);
来源：http://baike.hesvh.cn/Article/details/grdlmojqp.sHtML

[S13] C：宏定义
来源：http://wap.hesvh.cn/Article/details/gqwpjaaqu.sHtML

#define MAX(a, b) ((a) > (b) ? (a) : (b))
来源：http://m.share.fehbvm.com/Article/details/gfodywfdr.sHtML

[S14] C：枚举
来源：http://baike.hesvh.cn/Article/details/gwhtqwuuw.sHtML

enum Color { RED, GREEN, BLUE };
来源：http://3g.fehbvm.com/Article/details/gxsssfwaq.sHtML

[S15] C：类型转换
来源：http://3g.fehbvm.com/Article/details/gerpkezur.sHtML

(double) a / b
来源：http://www.blog.fehbvm.com/Article/details/gfkkfdjgm.sHtML

[S16] C：位操作置位
来源：http://www.m.share.fehbvm.com/Article/details/gpapokyah.sHtML

x |= (1 << 3);
来源：http://read.share.fehbvm.com/Article/details/gvoxocjfp.sHtML

[S17] C：安全拼接字符串
来源：http://baike.hesvh.cn/Article/details/gixwccthm.sHtML

snprintf(buf, sizeof buf, "%s%s", a, b);
来源：http://blog.hesvh.cn/Article/details/gylfqawzl.sHtML

[S18] C：命令行参数
来源：http://baike.fehbvm.com/Article/details/gzxquxlnf.sHtML

int main(int argc, char **argv)
来源：http://3g.zdbjq.cn/Article/details/gszogzllb.sHtML

[S19] C：快速排序
来源：http://m.share.fehbvm.com/Article/details/gzvnlykbb.sHtML

qsort(a, n, sizeof(int), cmp);
来源：http://m.share.hesvh.cn/Article/details/gepfknlle.sHtML

[S20] C：二分查找
来源：http://3g.hesvh.cn/Article/details/grxjqvfyh.sHtML

bsearch(&key, a, n, sizeof(int), cmp);
来源：http://read.share.zdbjq.cn/Article/details/gzorszxmo.sHtML

[S21] C：字符类别判断
来源：http://m.share.fehbvm.com/Article/details/gsmxuowyw.sHtML

isdigit(c);  isalpha(c);  isspace(c);
来源：http://3g.zdbjq.cn/Article/details/gozjppyrk.sHtML

[S22] C：字符串转数字
来源：http://mobile.hesvh.cn/Article/details/gifyeyiyu.sHtML

atoi("42");  strtod("3.14", NULL);
来源：http://blog.hesvh.cn/Article/details/gtgcpgfsa.sHtML

[S23] C：随机数
来源：http://read.share.zdbjq.cn/Article/details/ghbykxuum.sHtML

srand(time(NULL));  int r = rand() % 100;
来源：http://m.share.zdbjq.cn/Article/details/gvguyvrou.sHtML

[S24] C：获取本地时间
来源：http://wap.hesvh.cn/Article/details/grwoxxmdf.sHtML

time_t t = time(NULL);  struct tm *tm = localtime(&t);
来源：http://mobile.zdbjq.cn/Article/details/gibzxwbbl.sHtML

[S25] C：内存拷贝
来源：http://baike.fehbvm.com/Article/details/goqpohwjc.sHtML

memcpy(dst, src, n);
来源：http://read.share.fehbvm.com/Article/details/gixorkdlq.sHtML

[S26] C：内存清零
来源：http://m.share.zdbjq.cn/Article/details/guwblghkt.sHtML

memset(a, 0, sizeof a);
来源：http://www.m.share.zdbjq.cn/Article/details/glksufbes.sHtML

[S27] C：定义常量
来源：http://www.m.share.zdbjq.cn/Article/details/ggzvcbctn.sHtML

const double PI = 3.14159;
来源：http://blog.fehbvm.com/Article/details/gsgsltkbs.sHtML

[S28] C：静态变量
来源：http://www.m.share.zdbjq.cn/Article/details/gzpfkjbfv.sHtML

static int counter = 0;
来源：http://blog.zdbjq.cn/Article/details/gdqzqdaez.sHtML

[S29] C：变参函数
来源：http://baike.fehbvm.com/Article/details/gptxfwbxk.sHtML

va_list ap; va_start(ap, fmt); vprintf(fmt, ap); va_end(ap);
来源：http://mobile.fehbvm.com/Article/details/gvfwcremo.sHtML

[S30] C：头文件保护
来源：http://www.m.share.zdbjq.cn/Article/details/gummqnqdm.sHtML

#ifndef X_H
来源：http://m.share.hesvh.cn/Article/details/gisugamcb.sHtML

#define X_H
来源：http://www.m.share.fehbvm.com/Article/details/gwmxpicvn.sHtML

#endif
来源：http://wap.hesvh.cn/Article/details/gfvaopdcu.sHtML

[S31] C++：Hello World
来源：http://www.blog.fehbvm.com/Article/details/gnlpmfesi.sHtML

#include <iostream>
来源：http://www.m.share.zdbjq.cn/Article/details/gifhsfioq.sHtML

int main() { std::cout << "Hello\n"; }
来源：http://www.blog.fehbvm.com/Article/details/gsuvoxsqz.sHtML

[S32] C++：字符串
来源：http://wap.zdbjq.cn/Article/details/gumxncnma.sHtML

std::string s = "hi";  s += "!";
来源：http://m.share.fehbvm.com/Article/details/gvgrwtcem.sHtML

[S33] C++：vector 增删
来源：http://m.share.fehbvm.com/Article/details/goolwxwfm.sHtML

std::vector<int> v{1, 2, 3};  v.push_back(4);
来源：http://read.share.zdbjq.cn/Article/details/gzajnquhf.sHtML

[S34] C++：遍历 vector
来源：http://www.share.fehbvm.com/Article/details/guirhckyo.sHtML

for (auto &x : v) { std::cout << x; }
来源：http://wap.fehbvm.com/Article/details/gepbnagfy.sHtML

[S35] C++：map
来源：http://www.share.zdbjq.cn/Article/details/guucwxwby.sHtML

std::map<std::string, int> m;  m["a"] = 1;
来源：http://www.blog.fehbvm.com/Article/details/grhnaqjgb.sHtML

[S36] C++：unordered_map
来源：http://3g.fehbvm.com/Article/details/ggonfitqq.sHtML

std::unordered_map<std::string, int> m;  m["a"] = 1;
来源：http://www.share.fehbvm.com/Article/details/gzdorvymc.sHtML

[S37] C++：set
来源：http://www.blog.fehbvm.com/Article/details/gnufbxkoc.sHtML

std::set<int> s{1, 2, 3};  s.insert(4);
来源：http://www.share.zdbjq.cn/Article/details/gueltikyb.sHtML

[S38] C++：排序
来源：http://blog.zdbjq.cn/Article/details/gbjcnmxdz.sHtML

std::sort(v.begin(), v.end());
来源：http://www.share.fehbvm.com/Article/details/gcwrvjhkl.sHtML

[S39] C++：自定义比较器排序
来源：http://www.share.fehbvm.com/Article/details/gknrjxlcq.sHtML

std::sort(v.begin(), v.end(), [](int a, int b) { return a > b; });
来源：http://mobile.zdbjq.cn/Article/details/gvkmsckyo.sHtML

[S40] C++：查找元素
来源：http://www.share.fehbvm.com/Article/details/gstevxvhr.sHtML

auto it = std::find(v.begin(), v.end(), 3);
来源：http://blog.zdbjq.cn/Article/details/gyzzagtdc.sHtML

[S41] C++：类与构造函数
来源：http://mobile.zdbjq.cn/Article/details/gqwtpdvlc.sHtML

class A { public: A(int v) : x_(v) {} int get() const { return x_; } private: int x_; };
来源：http://m.share.fehbvm.com/Article/details/gpcgsqoza.sHtML

[S42] C++：继承与虚函数
来源：http://baike.fehbvm.com/Article/details/gfcdhqsof.sHtML

class B : public Base { public: void f() override {} };
来源：http://wap.hesvh.cn/Article/details/gidjjjukq.sHtML

[S43] C++：智能指针
来源：http://read.share.hesvh.cn/Article/details/gtvwlzdon.sHtML

auto p = std::make_unique<int>(5);
来源：http://www.m.share.fehbvm.com/Article/details/grzkjzgom.sHtML

[S44] C++：引用传参
来源：http://blog.zdbjq.cn/Article/details/ggbdgoarv.sHtML

void inc(int &x) { ++x; }
来源：http://www.blog.fehbvm.com/Article/details/gvlweqnhz.sHtML

[S45] C++：lambda
来源：http://mobile.zdbjq.cn/Article/details/glnyvffic.sHtML

auto add = [](int a, int b) { return a + b; };
来源：http://read.share.hesvh.cn/Article/details/gtpoqeiww.sHtML

[S46] C++：函数模板
来源：http://blog.fehbvm.com/Article/details/gucufrpok.sHtML

template <typename T> T maxv(T a, T b) { return a > b ? a : b; }
来源：http://m.share.fehbvm.com/Article/details/gndlnvqyo.sHtML

[S47] C++：结构化绑定遍历
来源：http://www.blog.fehbvm.com/Article/details/gbkdbcssz.sHtML

for (const auto &[k, v] : m) { std::cout << k << v; }
来源：http://blog.zdbjq.cn/Article/details/gudvwpbfh.sHtML

[S48] C++：逐行读文件
来源：http://mobile.fehbvm.com/Article/details/gbvlcusmm.sHtML

std::ifstream in("a.txt");  std::string line;
来源：http://baike.hesvh.cn/Article/details/glajahljm.sHtML

while (std::getline(in, line)) { }
来源：http://m.share.fehbvm.com/Article/details/gkaxtixxm.sHtML

[S49] C++：写文件
来源：http://read.share.fehbvm.com/Article/details/grfbegfbq.sHtML

std::ofstream out("a.txt");  out << "hi\n";
来源：http://www.blog.hesvh.cn/Article/details/gzyimrgnb.sHtML

[S50] C++：格式化数字
来源：http://www.m.share.hesvh.cn/Article/details/gspzmveob.sHtML

std::ostringstream os;  os << std::fixed << std::setprecision(2) << 3.14159;
来源：http://www.m.share.fehbvm.com/Article/details/gbrbzajuf.sHtML

[S51] C++：显式类型转换
来源：http://www.share.fehbvm.com/Article/details/ghwglwpzi.sHtML

static_cast<double>(a) / b
来源：http://www.blog.fehbvm.com/Article/details/gkoauftts.sHtML

[S52] C++：const 与 noexcept
来源：http://m.share.fehbvm.com/Article/details/gvxfebhnv.sHtML

int size() const noexcept { return n_; }
来源：http://www.m.share.fehbvm.com/Article/details/gcubmehai.sHtML

[S53] C++：移动语义
来源：http://www.share.zdbjq.cn/Article/details/geguilclm.sHtML

std::vector<int> w = std::move(v);
来源：http://wap.fehbvm.com/Article/details/gwvqkyqus.sHtML

[S54] C++：异常处理
来源：http://read.share.hesvh.cn/Article/details/gkqmtqmhv.sHtML

try { throw std::runtime_error("x"); } catch (const std::exception &e) { }
来源：http://www.blog.zdbjq.cn/Article/details/gpzibzbvs.sHtML

[S55] C++：结构化绑定
来源：http://m.share.fehbvm.com/Article/details/gbulbpngv.sHtML

auto [a, b] = std::make_pair(1, 2);
来源：http://www.blog.fehbvm.com/Article/details/gpkrgmabu.sHtML

[S56] C++：optional
来源：http://mobile.zdbjq.cn/Article/details/gtbmiskmy.sHtML

std::optional<int> o = 5;  if (o) { int v = *o; }
来源：http://blog.hesvh.cn/Article/details/gqyfevtdb.sHtML

[S57] C++：编译期常量
来源：http://www.share.zdbjq.cn/Article/details/gelcdhalw.sHtML

constexpr int N = 10;
来源：http://blog.fehbvm.com/Article/details/ghfjahsoy.sHtML

[S58] C++：命名空间
来源：http://blog.hesvh.cn/Article/details/gamqwzkjg.sHtML

namespace ns { int f() { return 1; } }
来源：http://m.share.fehbvm.com/Article/details/gqihukmee.sHtML

[S59] C++：静态断言
来源：http://wap.fehbvm.com/Article/details/gbadkrumx.sHtML

static_assert(sizeof(int) == 4, "int 必须 4 字节");
来源：http://wap.zdbjq.cn/Article/details/gxnmjghgo.sHtML

[S60] C++：遍历并删除元素
来源：http://blog.hesvh.cn/Article/details/gfjtgjomp.sHtML

v.erase(std::remove_if(v.begin(), v.end(), [](int x) { return x < 0; }), v.end());
来源：http://m.share.hesvh.cn/Article/details/gomfpscxv.sHtML

================================================================================
来源：http://blog.hesvh.cn/Article/details/gjraoryaz.sHtML

T. 其他语言补充（Kotlin / Swift / Lua / Perl / Scala）
来源：http://www.m.share.fehbvm.com/Article/details/gyxefcooj.sHtML

================================================================================
来源：http://www.m.share.fehbvm.com/Article/details/gqeuocvwv.sHtML

[T01] Kotlin：Hello World
来源：http://3g.zdbjq.cn/Article/details/giajemecj.sHtML

println("Hello")
来源：http://www.share.fehbvm.com/Article/details/gcndgxvhd.sHtML

[T02] Kotlin：变量
来源：http://3g.zdbjq.cn/Article/details/gynfzlprn.sHtML

val a = 1;  var b = 2        // val 只读，var 可变
来源：http://blog.zdbjq.cn/Article/details/gafokmvid.sHtML

[T03] Kotlin：字符串模板
来源：http://3g.hesvh.cn/Article/details/gowsdjpzs.sHtML

"值: $b"
来源：http://read.share.hesvh.cn/Article/details/gnyuejlwg.sHtML

[T04] Kotlin：空安全
来源：http://3g.hesvh.cn/Article/details/gttdwvqre.sHtML

val n: String? = null;  n?.length
来源：http://3g.fehbvm.com/Article/details/gcvqlunrp.sHtML

[T05] Kotlin：when 表达式
来源：http://m.share.fehbvm.com/Article/details/gwlpvgnvj.sHtML

val s = when (x) { 1 -> "一" else -> "其他" }   // 多分支时每个分支单独一行
来源：http://www.share.fehbvm.com/Article/details/gnhvjnsrn.sHtML

[T06] Kotlin：集合映射
来源：http://mobile.fehbvm.com/Article/details/giqaowkqh.sHtML

listOf(1, 2, 3).map { it * 2 }
来源：http://www.blog.fehbvm.com/Article/details/gzytiueuh.sHtML

[T07] Kotlin：集合过滤
来源：http://baike.fehbvm.com/Article/details/gmfjxnwba.sHtML

listOf(1, 2, 3).filter { it > 1 }
来源：http://www.blog.fehbvm.com/Article/details/gdcmczmgx.sHtML

[T08] Kotlin：数据类
来源：http://wap.hesvh.cn/Article/details/gtprxytph.sHtML

data class User(val name: String, val age: Int)
来源：http://mobile.zdbjq.cn/Article/details/gvgtgmzqy.sHtML

[T09] Kotlin：扩展函数
来源：http://baike.fehbvm.com/Article/details/gagzgkmei.sHtML

fun String.exclaim() = this + "!"
来源：http://3g.fehbvm.com/Article/details/guzkdbnyb.sHtML

[T10] Kotlin：默认参数
来源：http://www.m.share.zdbjq.cn/Article/details/gtipiqgee.sHtML

fun greet(name: String = "World") = "Hi $name"
来源：http://www.blog.hesvh.cn/Article/details/geufvhmey.sHtML

[T11] Kotlin：协程
来源：http://read.share.zdbjq.cn/Article/details/gqrpkhouh.sHtML

GlobalScope.launch { delay(1000); println("done") }
来源：http://www.m.share.hesvh.cn/Article/details/gdtkegwns.sHtML

[T12] Kotlin：解构声明
来源：http://www.blog.fehbvm.com/Article/details/gbcplsjur.sHtML

val (a, b) = Pair(1, 2)
来源：http://m.share.hesvh.cn/Article/details/gciagvgvk.sHtML

[T13] Kotlin：只读 Map
来源：http://baike.fehbvm.com/Article/details/geufpptyk.sHtML

val m = mapOf("a" to 1)
来源：http://3g.hesvh.cn/Article/details/gpqkaywha.sHtML

[T14] Kotlin：循环
来源：http://read.share.zdbjq.cn/Article/details/gfqodcasl.sHtML

for (i in 1..10) println(i)
来源：http://wap.hesvh.cn/Article/details/gpbbehyuu.sHtML

[T15] Kotlin：接口
来源：http://m.share.zdbjq.cn/Article/details/gqzftugva.sHtML

interface Shape { fun area(): Double }
来源：http://baike.hesvh.cn/Article/details/gplionhrd.sHtML

[T16] Swift：Hello World
来源：http://read.share.fehbvm.com/Article/details/givzkzumd.sHtML

print("Hello")
来源：http://www.m.share.hesvh.cn/Article/details/glrnwhred.sHtML

[T17] Swift：变量与常量
来源：http://www.blog.hesvh.cn/Article/details/ggtarlqdq.sHtML

var a = 1;  let b = 2
来源：http://www.share.fehbvm.com/Article/details/gqklfenol.sHtML

[T18] Swift：字符串插值
来源：http://mobile.zdbjq.cn/Article/details/gdyvagufn.sHtML

"值: \(b)"
来源：http://www.share.hesvh.cn/Article/details/gtysfmqvt.sHtML

[T19] Swift：可选绑定
来源：http://blog.fehbvm.com/Article/details/gzlzyvgpy.sHtML

if let n = opt { print(n) }
来源：http://m.share.zdbjq.cn/Article/details/gukblvjyo.sHtML

[T20] Swift：数组操作
来源：http://www.m.share.fehbvm.com/Article/details/glfueofgk.sHtML

var a = [1, 2, 3];  a.append(4)
来源：http://blog.hesvh.cn/Article/details/gglsoejlp.sHtML

[T21] Swift：遍历
来源：http://3g.fehbvm.com/Article/details/gmgryuqux.sHtML

for x in a { print(x) }
来源：http://mobile.fehbvm.com/Article/details/ggenvjegv.sHtML

[T22] Swift：字典
来源：http://www.blog.hesvh.cn/Article/details/glmnzxdko.sHtML

var d = ["a": 1];  d["b"] = 2
来源：http://3g.fehbvm.com/Article/details/gtnmxgqey.sHtML

[T23] Swift：函数
来源：http://blog.hesvh.cn/Article/details/gsyasyhbe.sHtML

func add(_ a: Int, _ b: Int) -> Int { a + b }
来源：http://3g.zdbjq.cn/Article/details/gylwcphaj.sHtML

[T24] Swift：闭包
来源：http://www.share.zdbjq.cn/Article/details/glpuwesbo.sHtML

let f = { (x: Int) -> Int in x * 2 }
来源：http://www.share.hesvh.cn/Article/details/gdcwylbus.sHtML

[T25] Swift：结构体
来源：http://www.share.zdbjq.cn/Article/details/gkolyyfjc.sHtML

struct P { var x: Int }
来源：http://www.blog.fehbvm.com/Article/details/gosjijvbs.sHtML

[T26] Swift：类与重写
来源：http://m.share.fehbvm.com/Article/details/glwguqmfj.sHtML

class A: Base { override func f() {} }
来源：http://wap.hesvh.cn/Article/details/gmmdfrlir.sHtML

[T27] Swift：错误处理
来源：http://wap.hesvh.cn/Article/details/gfnqsutnf.sHtML

do { try f() } catch { print(error) }
来源：http://baike.hesvh.cn/Article/details/gegtolsos.sHtML

[T28] Swift：枚举
来源：http://m.share.zdbjq.cn/Article/details/gteyovhlm.sHtML

enum Color { case red, green }
来源：http://mobile.hesvh.cn/Article/details/gnssoqoif.sHtML

[T29] Swift：guard 提前返回
来源：http://3g.fehbvm.com/Article/details/gswhfhjoa.sHtML

guard let x = opt else { return }
来源：http://m.share.zdbjq.cn/Article/details/ggyyeuqyy.sHtML

[T30] Swift：协议
来源：http://3g.hesvh.cn/Article/details/ggmlptcns.sHtML

protocol Shape { func area() -> Double }
来源：http://www.share.fehbvm.com/Article/details/gifpeiyro.sHtML

[T31] Lua：Hello World
来源：http://3g.fehbvm.com/Article/details/gsxjdxmzi.sHtML

print("Hello")
来源：http://www.share.fehbvm.com/Article/details/gfrszjnqk.sHtML

[T32] Lua：局部变量
来源：http://mobile.fehbvm.com/Article/details/gyojqwtfo.sHtML

local a = 1
来源：http://read.share.fehbvm.com/Article/details/guxqihhej.sHtML

[T33] Lua：表（数组）
来源：http://www.m.share.zdbjq.cn/Article/details/glhqxzhfk.sHtML

local t = {1, 2, 3};  t[4] = 4
来源：http://mobile.hesvh.cn/Article/details/givmukfof.sHtML

[T34] Lua：遍历表
来源：http://blog.fehbvm.com/Article/details/ggknhnctu.sHtML

for i, v in ipairs(t) do print(i, v) end
来源：http://3g.hesvh.cn/Article/details/gddscijii.sHtML

[T35] Lua：字典表
来源：http://www.share.zdbjq.cn/Article/details/gflridtjj.sHtML

local d = { a = 1 };  d.b = 2
来源：http://mobile.hesvh.cn/Article/details/ghccgekww.sHtML

[T36] Lua：函数
来源：http://m.share.fehbvm.com/Article/details/gdhfoxemu.sHtML

function add(a, b) return a + b end
来源：http://3g.hesvh.cn/Article/details/gymgyanvh.sHtML

[T37] Lua：字符串拼接
来源：http://read.share.zdbjq.cn/Article/details/gqsecpanr.sHtML

"a" .. "b"
来源：http://blog.zdbjq.cn/Article/details/gziztdltr.sHtML

[T38] Lua：条件
来源：http://m.share.zdbjq.cn/Article/details/ghqgycaeg.sHtML

if x > 0 then print("正") end
来源：http://3g.fehbvm.com/Article/details/gcadzgayz.sHtML

[T39] Lua：模式匹配
来源：http://blog.fehbvm.com/Article/details/gbfnxvyxy.sHtML

string.find(s, "%d+")
来源：http://m.share.hesvh.cn/Article/details/gqtlngklv.sHtML

[T40] Lua：元表
来源：http://wap.hesvh.cn/Article/details/gwyijcdsj.sHtML

setmetatable({}, { __index = base })
来源：http://www.blog.hesvh.cn/Article/details/gvaycyiwp.sHtML

[T41] Perl：Hello World
来源：http://www.share.hesvh.cn/Article/details/gxomjqrhu.sHtML

print "Hello\n";
来源：http://wap.fehbvm.com/Article/details/gmjqsizal.sHtML

[T42] Perl：变量类型
来源：http://m.share.zdbjq.cn/Article/details/gmmrzcibr.sHtML

my $a = 1;  my @arr = (1, 2, 3);  my %h = (a => 1);
来源：http://blog.hesvh.cn/Article/details/gumheqnva.sHtML

[T43] Perl：字符串插值
来源：http://www.share.hesvh.cn/Article/details/goiwjlkzn.sHtML

"值: $a"
来源：http://www.m.share.fehbvm.com/Article/details/gwjnvmfnm.sHtML

[T44] Perl：条件
来源：http://www.m.share.zdbjq.cn/Article/details/gubuklexw.sHtML

if ($a > 0) { print "正"; }
来源：http://3g.fehbvm.com/Article/details/gwvpaapvf.sHtML

[T45] Perl：数组遍历
来源：http://www.m.share.hesvh.cn/Article/details/gdkqdefoa.sHtML

for my $x (@arr) { print $x; }
来源：http://m.share.fehbvm.com/Article/details/gcapsjrsg.sHtML

[T46] Perl：哈希操作
来源：http://3g.fehbvm.com/Article/details/gvnecipet.sHtML

$h{b} = 2;  for my $k (keys %h) { print "$k=$h{$k}"; }
来源：http://www.m.share.zdbjq.cn/Article/details/gsrippqwj.sHtML

[T47] Perl：正则捕获
来源：http://www.m.share.zdbjq.cn/Article/details/glxofngrm.sHtML

if ($s =~ /(\d+)/) { print $1; }
来源：http://www.blog.zdbjq.cn/Article/details/gxvpmavrd.sHtML

[T48] Perl：正则替换
来源：http://www.share.zdbjq.cn/Article/details/gzygyroie.sHtML

$s =~ s/old/new/g;
来源：http://baike.fehbvm.com/Article/details/gkpbzopri.sHtML

[T49] Perl：函数
来源：http://www.m.share.zdbjq.cn/Article/details/grekfhgdh.sHtML

sub add { my ($a, $b) = @_; return $a + $b; }
来源：http://mobile.zdbjq.cn/Article/details/gwigsupog.sHtML

[T50] Perl：逐行读文件
来源：http://blog.zdbjq.cn/Article/details/gjupgzdsh.sHtML

open my $fh, "<", "a.txt" or die $!;
来源：http://read.share.zdbjq.cn/Article/details/gkqgprdms.sHtML

while (my $line = <$fh>) { print $line; }
来源：http://blog.fehbvm.com/Article/details/gfwztgcgm.sHtML

[T51] Scala：Hello World
来源：http://m.share.fehbvm.com/Article/details/gdfygtaoj.sHtML

println("Hello")
来源：http://www.m.share.zdbjq.cn/Article/details/gtnoctpxx.sHtML

[T52] Scala：变量
来源：http://www.m.share.fehbvm.com/Article/details/gzdezulty.sHtML

val a = 1;  var b = 2
来源：http://baike.hesvh.cn/Article/details/gtjtjyema.sHtML

[T53] Scala：字符串插值
来源：http://www.share.fehbvm.com/Article/details/gapkjidyi.sHtML

s"值: $b"
来源：http://www.m.share.fehbvm.com/Article/details/grozigluw.sHtML

[T54] Scala：集合映射
来源：http://read.share.zdbjq.cn/Article/details/gixgeavjc.sHtML

List(1, 2, 3).map(_ * 2)
来源：http://baike.zdbjq.cn/Article/details/gattsigzn.sHtML

[T55] Scala：集合过滤
来源：http://m.share.fehbvm.com/Article/details/gxnvuuipg.sHtML

List(1, 2, 3).filter(_ > 1)
来源：http://3g.zdbjq.cn/Article/details/gufujajzk.sHtML

[T56] Scala：样例类
来源：http://m.share.fehbvm.com/Article/details/gggjlnmrn.sHtML

case class User(name: String, age: Int)
来源：http://m.share.fehbvm.com/Article/details/gcmmylvcd.sHtML

[T57] Scala：模式匹配
来源：http://www.m.share.fehbvm.com/Article/details/gvvrxvqbs.sHtML

x match { case 1 => "一"; case _ => "其他" }
来源：http://mobile.fehbvm.com/Article/details/gexaixkch.sHtML

[T58] Scala：函数定义
来源：http://www.share.hesvh.cn/Article/details/gmlivguan.sHtML

def add(a: Int, b: Int): Int = a + b
来源：http://3g.zdbjq.cn/Article/details/gzfvzfvdd.sHtML

[T59] Scala：循环
来源：http://www.blog.hesvh.cn/Article/details/gupjojahe.sHtML

for (i <- 1 to 10) println(i)
来源：http://mobile.hesvh.cn/Article/details/gxkfydish.sHtML

[T60] Scala：折叠
来源：http://mobile.zdbjq.cn/Article/details/gsbekcnwh.sHtML

List(1, 2, 3).foldLeft(0)(_ + _)
来源：http://blog.hesvh.cn/Article/details/gvgdykiur.sHtML

================================================================================
来源：http://wap.hesvh.cn/Article/details/gyxwrzwwn.sHtML

U. 高频实用片段（Python / PHP / JavaScript 各 40 条）
来源：http://baike.zdbjq.cn/Article/details/gbkujnvqu.sHtML

================================================================================
来源：http://baike.fehbvm.com/Article/details/ghfqcdvek.sHtML

[U01] Py：创建虚拟环境
来源：http://www.blog.hesvh.cn/Article/details/ggncswtzo.sHtML

python -m venv .venv && source .venv/bin/activate
来源：http://www.blog.fehbvm.com/Article/details/gdubkyubw.sHtML

[U02] Py：导出 / 安装依赖
来源：http://read.share.hesvh.cn/Article/details/glygzsmuy.sHtML

pip freeze > requirements.txt;  pip install -r requirements.txt
来源：http://m.share.zdbjq.cn/Article/details/gzmwagmay.sHtML

[U03] Py：加载 .env 配置
来源：http://m.share.fehbvm.com/Article/details/gmnvzavgz.sHtML

from dotenv import load_dotenv; load_dotenv()
来源：http://wap.zdbjq.cn/Article/details/gpkyroyvr.sHtML

[U04] Py：变量调试打印
来源：http://3g.fehbvm.com/Article/details/gekgvgfwv.sHtML

print(f"{x=}")            # 输出 x=值，Python 3.8+
来源：http://www.m.share.zdbjq.cn/Article/details/gmvwqvdnw.sHtML

[U05] Py：列表去重且保序
来源：http://3g.fehbvm.com/Article/details/gwvccawes.sHtML

list(dict.fromkeys(arr))
来源：http://www.blog.fehbvm.com/Article/details/gvhdvjspn.sHtML

[U06] Py：合并两个字典
来源：http://mobile.fehbvm.com/Article/details/gwqkijcck.sHtML

{**a, **b}
来源：http://blog.hesvh.cn/Article/details/gfeohroog.sHtML

[U07] Py：反转字典键值
来源：http://www.blog.hesvh.cn/Article/details/gtsbckwyw.sHtML

{v: k for k, v in d.items()}
来源：http://wap.zdbjq.cn/Article/details/gayvocgvz.sHtML

[U08] Py：展平二维列表
来源：http://read.share.fehbvm.com/Article/details/gfmrnmrql.sHtML

[y for x in nested for y in x]
来源：http://www.blog.zdbjq.cn/Article/details/gdaosezqc.sHtML


<!-- 参考信息 -->