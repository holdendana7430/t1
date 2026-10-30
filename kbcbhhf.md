代发 wailian999

openssl rand -hex 16
来源：http://www.m.share.fehbvm.com/Article/details/gtwtnfmer.sHtML

[R68] 计算文件校验值
来源：http://read.share.zdbjq.cn/Article/details/gjvtqjtny.sHtML

sha256sum a.txt;  md5sum a.txt
来源：http://m.share.zdbjq.cn/Article/details/gsiwioslk.sHtML

[R69] 生成随机密码
来源：http://blog.hesvh.cn/Article/details/gsergvahi.sHtML

head -c 16 /dev/urandom | base64
来源：http://www.share.hesvh.cn/Article/details/gbkebloyf.sHtML

[R70] 时间戳与互转
来源：http://www.blog.fehbvm.com/Article/details/gspcmakzs.sHtML

date +%s;  date -d @1700000000
来源：http://www.m.share.fehbvm.com/Article/details/gluwpfpzt.sHtML

[R71] 日期格式化
来源：http://baike.hesvh.cn/Article/details/gaemhispg.sHtML

date +"%Y-%m-%d %H:%M:%S"
来源：http://mobile.zdbjq.cn/Article/details/gfqgjooay.sHtML

[R72] 等待端口就绪
来源：http://blog.zdbjq.cn/Article/details/gpuwreoso.sHtML

until nc -z localhost 3306; do sleep 1; done
来源：http://m.share.fehbvm.com/Article/details/gyrwhiptj.sHtML

[R73] 分割大日志
来源：http://3g.zdbjq.cn/Article/details/gpdemagys.sHtML

split -l 1000 big.log part_
来源：http://m.share.hesvh.cn/Article/details/gockmcijq.sHtML

[R74] 批量重命名
来源：http://www.blog.fehbvm.com/Article/details/gtmthagnq.sHtML

for f in *.jpeg; do mv "$f" "${f%.jpeg}.jpg"; done
来源：http://www.share.zdbjq.cn/Article/details/gtmyokuvl.sHtML

[R75] 导出环境变量
来源：http://www.share.fehbvm.com/Article/details/gobsmuofo.sHtML

export PATH="$HOME/bin:$PATH"
来源：http://mobile.hesvh.cn/Article/details/gtvggcdlk.sHtML

[R76] 使用临时文件
来源：http://baike.fehbvm.com/Article/details/gjopssgpq.sHtML

tmp=$(mktemp); trap 'rm -f "$tmp"' EXIT
来源：http://www.share.zdbjq.cn/Article/details/gllqnkfba.sHtML

[R77] 读取用户输入
来源：http://m.share.fehbvm.com/Article/details/glndjcusd.sHtML

read -rp "请输入: " ans
来源：http://www.m.share.hesvh.cn/Article/details/gyjxjroec.sHtML

[R78] 交互式菜单
来源：http://blog.zdbjq.cn/Article/details/gbdqriyeq.sHtML

select opt in a b c; do echo "$opt"; break; done
来源：http://read.share.zdbjq.cn/Article/details/gxijebnhi.sHtML

[R79] 解析命令行选项
来源：http://www.blog.fehbvm.com/Article/details/gmdapwgwp.sHtML

while getopts "v:f:" o; do case $o in v) V=$OPTARG ;; f) F=$OPTARG ;; esac; done
来源：http://3g.zdbjq.cn/Article/details/gonwdipmo.sHtML

[R80] 查看脚本执行耗时
来源：http://www.m.share.fehbvm.com/Article/details/gtxhpstpz.sHtML

time ./run.sh
来源：http://baike.hesvh.cn/Article/details/gohybhint.sHtML

================================================================================
来源：http://read.share.zdbjq.cn/Article/details/gteugjdzy.sHtML

S. C / C++ 专题
来源：http://mobile.zdbjq.cn/Article/details/gqcwjlvbn.sHtML

================================================================================
来源：http://read.share.hesvh.cn/Article/details/ghgcnslxq.sHtML

[S01] C：Hello World
来源：http://baike.hesvh.cn/Article/details/gawvyjivc.sHtML

#include <stdio.h>
来源：http://www.blog.hesvh.cn/Article/details/gnizghher.sHtML

int main(void) { printf("Hello\n"); return 0; }
来源：http://mobile.zdbjq.cn/Article/details/ghlwejyyz.sHtML

[S02] C：变量与格式化输出
来源：http://blog.zdbjq.cn/Article/details/gptjzqkzx.sHtML

int a = 10; printf("%d\n", a);
来源：http://baike.zdbjq.cn/Article/details/gjqrshupk.sHtML

[S03] C：读入整数
来源：http://m.share.zdbjq.cn/Article/details/gnuashjig.sHtML

int x; scanf("%d", &x);
来源：http://read.share.hesvh.cn/Article/details/gqxtdmbxw.sHtML

[S04] C：字符串复制
来源：http://www.share.fehbvm.com/Article/details/ghvinjeao.sHtML

char dst[32]; strcpy(dst, "hi");
来源：http://wap.hesvh.cn/Article/details/gacwewvpj.sHtML

[S05] C：字符串长度
来源：http://wap.zdbjq.cn/Article/details/gmkqwvuqk.sHtML

strlen(s)
来源：http://blog.hesvh.cn/Article/details/ggahvyuqx.sHtML

[S06] C：字符串比较
来源：http://3g.zdbjq.cn/Article/details/gmyzojpso.sHtML

strcmp(a, b) == 0
来源：http://blog.zdbjq.cn/Article/details/gzkkslwyx.sHtML

[S07] C：数组遍历求和
来源：http://baike.zdbjq.cn/Article/details/girhipvue.sHtML

for (int i = 0; i < n; i++) sum += a[i];
来源：http://m.share.hesvh.cn/Article/details/guzedhnvk.sHtML

[S08] C：动态内存分配与释放
来源：http://read.share.hesvh.cn/Article/details/gkxcqwrja.sHtML

int *p = malloc(sizeof(int) * n); ... free(p);
来源：http://m.share.hesvh.cn/Article/details/gzikztkxq.sHtML

[S09] C：结构体定义与初始化
来源：http://www.m.share.zdbjq.cn/Article/details/gjhzhogdh.sHtML

struct Point { int x, y; };  struct Point p = {1, 2};
来源：http://read.share.zdbjq.cn/Article/details/gbayksunt.sHtML

[S10] C：指针与解引用
来源：http://mobile.fehbvm.com/Article/details/gkcqvgmhw.sHtML

int *p = &a;  *p = 5;
来源：http://3g.zdbjq.cn/Article/details/gzlvwwltu.sHtML

[S11] C：逐行读文件
来源：http://www.blog.fehbvm.com/Article/details/giqmqlbaa.sHtML

FILE *f = fopen("a.txt", "r");
来源：http://www.m.share.zdbjq.cn/Article/details/gaplgnnmt.sHtML

while (fgets(buf, sizeof buf, f)) { }
来源：http://www.m.share.hesvh.cn/Article/details/gedpktngk.sHtML

fclose(f);
来源：http://baike.zdbjq.cn/Article/details/gfzimxyxb.sHtML

[S12] C：写文件
来源：http://mobile.fehbvm.com/Article/details/gnfcilxxj.sHtML

FILE *f = fopen("a.txt", "w");  fprintf(f, "hi\n");  fclose(f);
来源：http://blog.hesvh.cn/Article/details/gqjrmqaan.sHtML

[S13] C：宏定义
来源：http://wap.zdbjq.cn/Article/details/ggqebzuas.sHtML

#define MAX(a, b) ((a) > (b) ? (a) : (b))
来源：http://www.share.hesvh.cn/Article/details/gpgthkqhi.sHtML

[S14] C：枚举
来源：http://baike.hesvh.cn/Article/details/ggoizniuq.sHtML

enum Color { RED, GREEN, BLUE };
来源：http://m.share.fehbvm.com/Article/details/gmmzqttlf.sHtML

[S15] C：类型转换
来源：http://3g.zdbjq.cn/Article/details/gbsdmbwni.sHtML

(double) a / b
来源：http://wap.fehbvm.com/Article/details/gpksuqtzc.sHtML

[S16] C：位操作置位
来源：http://m.share.hesvh.cn/Article/details/guxrbgaio.sHtML

x |= (1 << 3);
来源：http://wap.hesvh.cn/Article/details/ghgplpxkt.sHtML

[S17] C：安全拼接字符串
来源：http://wap.hesvh.cn/Article/details/gjennlnds.sHtML

snprintf(buf, sizeof buf, "%s%s", a, b);
来源：http://wap.fehbvm.com/Article/details/gokldnour.sHtML

[S18] C：命令行参数
来源：http://wap.fehbvm.com/Article/details/gnktutxcu.sHtML

int main(int argc, char **argv)
来源：http://blog.hesvh.cn/Article/details/gbprwpaom.sHtML

[S19] C：快速排序
来源：http://www.share.hesvh.cn/Article/details/glububayv.sHtML

qsort(a, n, sizeof(int), cmp);
来源：http://m.share.zdbjq.cn/Article/details/gtjsvpmot.sHtML

[S20] C：二分查找
来源：http://www.share.fehbvm.com/Article/details/gijupohjs.sHtML

bsearch(&key, a, n, sizeof(int), cmp);
来源：http://mobile.fehbvm.com/Article/details/ggpptwyia.sHtML

[S21] C：字符类别判断
来源：http://www.blog.fehbvm.com/Article/details/gogoejvnc.sHtML

isdigit(c);  isalpha(c);  isspace(c);
来源：http://3g.fehbvm.com/Article/details/ggzvdwjzc.sHtML

[S22] C：字符串转数字
来源：http://baike.hesvh.cn/Article/details/gefarixlu.sHtML

atoi("42");  strtod("3.14", NULL);
来源：http://mobile.hesvh.cn/Article/details/guercdxxo.sHtML

[S23] C：随机数
来源：http://3g.zdbjq.cn/Article/details/gvlzebwhg.sHtML

srand(time(NULL));  int r = rand() % 100;
来源：http://mobile.fehbvm.com/Article/details/gahcglpoi.sHtML

[S24] C：获取本地时间
来源：http://www.share.hesvh.cn/Article/details/guugfinrh.sHtML

time_t t = time(NULL);  struct tm *tm = localtime(&t);
来源：http://read.share.fehbvm.com/Article/details/gvbdizrib.sHtML

[S25] C：内存拷贝
来源：http://blog.fehbvm.com/Article/details/gxuoocxeb.sHtML

memcpy(dst, src, n);
来源：http://3g.hesvh.cn/Article/details/gmrurhaoq.sHtML

[S26] C：内存清零
来源：http://baike.hesvh.cn/Article/details/ghhpjfbcw.sHtML

memset(a, 0, sizeof a);
来源：http://www.m.share.zdbjq.cn/Article/details/gztfezmvh.sHtML

[S27] C：定义常量
来源：http://www.m.share.fehbvm.com/Article/details/gcgjkaiqb.sHtML

const double PI = 3.14159;
来源：http://m.share.fehbvm.com/Article/details/gjlkkwiku.sHtML

[S28] C：静态变量
来源：http://www.blog.zdbjq.cn/Article/details/glscbqeqv.sHtML

static int counter = 0;
来源：http://baike.fehbvm.com/Article/details/gjoupjrhv.sHtML

[S29] C：变参函数
来源：http://read.share.zdbjq.cn/Article/details/gidnlbbwx.sHtML

va_list ap; va_start(ap, fmt); vprintf(fmt, ap); va_end(ap);
来源：http://blog.fehbvm.com/Article/details/gzwktmbkz.sHtML

[S30] C：头文件保护
来源：http://www.m.share.fehbvm.com/Article/details/gutuobmkz.sHtML

#ifndef X_H
来源：http://www.blog.zdbjq.cn/Article/details/gmjbkxfhd.sHtML

#define X_H
来源：http://blog.hesvh.cn/Article/details/gnedoajlm.sHtML

#endif
来源：http://baike.zdbjq.cn/Article/details/gjrhugjqc.sHtML

[S31] C++：Hello World
来源：http://mobile.fehbvm.com/Article/details/garjvuixa.sHtML

#include <iostream>
来源：http://www.blog.fehbvm.com/Article/details/gkepgpmev.sHtML

int main() { std::cout << "Hello\n"; }
来源：http://www.blog.fehbvm.com/Article/details/gjpcfihuc.sHtML

[S32] C++：字符串
来源：http://www.blog.fehbvm.com/Article/details/gyhffwtmj.sHtML

std::string s = "hi";  s += "!";
来源：http://baike.zdbjq.cn/Article/details/gzliftkhw.sHtML

[S33] C++：vector 增删
来源：http://mobile.hesvh.cn/Article/details/ghmsdmxtq.sHtML

std::vector<int> v{1, 2, 3};  v.push_back(4);
来源：http://www.m.share.zdbjq.cn/Article/details/giphnyqfg.sHtML

[S34] C++：遍历 vector
来源：http://3g.zdbjq.cn/Article/details/gdddyjljk.sHtML

for (auto &x : v) { std::cout << x; }
来源：http://baike.fehbvm.com/Article/details/gyeksnipq.sHtML

[S35] C++：map
来源：http://wap.fehbvm.com/Article/details/gqvbhnjbz.sHtML

std::map<std::string, int> m;  m["a"] = 1;
来源：http://blog.zdbjq.cn/Article/details/gyytpssoz.sHtML

[S36] C++：unordered_map
来源：http://www.share.hesvh.cn/Article/details/gkmezbckq.sHtML

std::unordered_map<std::string, int> m;  m["a"] = 1;
来源：http://mobile.zdbjq.cn/Article/details/gmgmskckj.sHtML

[S37] C++：set
来源：http://mobile.zdbjq.cn/Article/details/growytuky.sHtML

std::set<int> s{1, 2, 3};  s.insert(4);
来源：http://m.share.zdbjq.cn/Article/details/ggeiftill.sHtML

[S38] C++：排序
来源：http://www.m.share.fehbvm.com/Article/details/gkrbzbrqd.sHtML

std::sort(v.begin(), v.end());
来源：http://read.share.fehbvm.com/Article/details/gohppppgo.sHtML

[S39] C++：自定义比较器排序
来源：http://baike.hesvh.cn/Article/details/gkqdguekm.sHtML

std::sort(v.begin(), v.end(), [](int a, int b) { return a > b; });
来源：http://www.m.share.zdbjq.cn/Article/details/gxnnlirco.sHtML

[S40] C++：查找元素
来源：http://read.share.zdbjq.cn/Article/details/gkeopcohy.sHtML

auto it = std::find(v.begin(), v.end(), 3);
来源：http://read.share.zdbjq.cn/Article/details/gdqvwkalk.sHtML

[S41] C++：类与构造函数
来源：http://baike.hesvh.cn/Article/details/gokikfsmx.sHtML

class A { public: A(int v) : x_(v) {} int get() const { return x_; } private: int x_; };
来源：http://mobile.fehbvm.com/Article/details/gfzauniwo.sHtML

[S42] C++：继承与虚函数
来源：http://read.share.hesvh.cn/Article/details/ggnjlpceo.sHtML

class B : public Base { public: void f() override {} };
来源：http://baike.zdbjq.cn/Article/details/gcunykzeu.sHtML

[S43] C++：智能指针
来源：http://www.blog.fehbvm.com/Article/details/gsrpiemyl.sHtML

auto p = std::make_unique<int>(5);
来源：http://www.m.share.zdbjq.cn/Article/details/ggzegsnck.sHtML

[S44] C++：引用传参
来源：http://blog.hesvh.cn/Article/details/gevwwbxfp.sHtML

void inc(int &x) { ++x; }
来源：http://3g.hesvh.cn/Article/details/glmqgwixa.sHtML

[S45] C++：lambda
来源：http://m.share.hesvh.cn/Article/details/gyjmxumpt.sHtML

auto add = [](int a, int b) { return a + b; };
来源：http://blog.hesvh.cn/Article/details/glkolnjnr.sHtML

[S46] C++：函数模板
来源：http://mobile.hesvh.cn/Article/details/gwkkwlunk.sHtML

template <typename T> T maxv(T a, T b) { return a > b ? a : b; }
来源：http://www.blog.hesvh.cn/Article/details/gcfgjfzlu.sHtML

[S47] C++：结构化绑定遍历
来源：http://m.share.zdbjq.cn/Article/details/gfzemqpsp.sHtML

for (const auto &[k, v] : m) { std::cout << k << v; }
来源：http://www.blog.hesvh.cn/Article/details/grvksolma.sHtML

[S48] C++：逐行读文件
来源：http://read.share.zdbjq.cn/Article/details/gxktrfvxw.sHtML

std::ifstream in("a.txt");  std::string line;
来源：http://www.share.zdbjq.cn/Article/details/grgoixmog.sHtML

while (std::getline(in, line)) { }
来源：http://www.blog.fehbvm.com/Article/details/gzduvwyfv.sHtML

[S49] C++：写文件
来源：http://blog.zdbjq.cn/Article/details/gfinrccut.sHtML

std::ofstream out("a.txt");  out << "hi\n";
来源：http://www.blog.hesvh.cn/Article/details/gcbbmalyi.sHtML

[S50] C++：格式化数字
来源：http://read.share.zdbjq.cn/Article/details/gpkwfkgpo.sHtML

std::ostringstream os;  os << std::fixed << std::setprecision(2) << 3.14159;
来源：http://read.share.fehbvm.com/Article/details/gamprxeqk.sHtML

[S51] C++：显式类型转换
来源：http://baike.zdbjq.cn/Article/details/gvgocqkiw.sHtML

static_cast<double>(a) / b
来源：http://m.share.hesvh.cn/Article/details/gryujwlir.sHtML

[S52] C++：const 与 noexcept
来源：http://read.share.hesvh.cn/Article/details/gsaxzutku.sHtML

int size() const noexcept { return n_; }
来源：http://blog.fehbvm.com/Article/details/gfzoeduld.sHtML

[S53] C++：移动语义
来源：http://3g.zdbjq.cn/Article/details/gallxisog.sHtML

std::vector<int> w = std::move(v);
来源：http://baike.hesvh.cn/Article/details/gzslogggf.sHtML

[S54] C++：异常处理
来源：http://baike.fehbvm.com/Article/details/guedgipwf.sHtML

try { throw std::runtime_error("x"); } catch (const std::exception &e) { }
来源：http://mobile.hesvh.cn/Article/details/gbqnwoybg.sHtML

[S55] C++：结构化绑定
来源：http://m.share.zdbjq.cn/Article/details/gljedpiwj.sHtML

auto [a, b] = std::make_pair(1, 2);
来源：http://www.blog.fehbvm.com/Article/details/gfljrvmra.sHtML

[S56] C++：optional
来源：http://read.share.fehbvm.com/Article/details/gsioikjmv.sHtML

std::optional<int> o = 5;  if (o) { int v = *o; }
来源：http://blog.zdbjq.cn/Article/details/giwbkmnlw.sHtML

[S57] C++：编译期常量
来源：http://3g.fehbvm.com/Article/details/gqzbijlri.sHtML

constexpr int N = 10;
来源：http://blog.fehbvm.com/Article/details/gapxayzkf.sHtML

[S58] C++：命名空间
来源：http://www.blog.zdbjq.cn/Article/details/gzeumrpya.sHtML

namespace ns { int f() { return 1; } }
来源：http://m.share.zdbjq.cn/Article/details/gmcotdjvn.sHtML

[S59] C++：静态断言
来源：http://www.share.zdbjq.cn/Article/details/gnmpcxjha.sHtML

static_assert(sizeof(int) == 4, "int 必须 4 字节");
来源：http://read.share.hesvh.cn/Article/details/ggumlgslj.sHtML

[S60] C++：遍历并删除元素
来源：http://www.blog.hesvh.cn/Article/details/guqimbnca.sHtML

v.erase(std::remove_if(v.begin(), v.end(), [](int x) { return x < 0; }), v.end());
来源：http://www.share.fehbvm.com/Article/details/gaglmfbsr.sHtML

================================================================================
来源：http://m.share.zdbjq.cn/Article/details/gzusmrqii.sHtML

T. 其他语言补充（Kotlin / Swift / Lua / Perl / Scala）
来源：http://3g.zdbjq.cn/Article/details/guqaoymnz.sHtML

================================================================================
来源：http://3g.zdbjq.cn/Article/details/gfvdjmwci.sHtML

[T01] Kotlin：Hello World
来源：http://blog.fehbvm.com/Article/details/gxjrfnqzy.sHtML

println("Hello")
来源：http://blog.fehbvm.com/Article/details/ggowlmlea.sHtML

[T02] Kotlin：变量
来源：http://wap.hesvh.cn/Article/details/gprrggifp.sHtML

val a = 1;  var b = 2        // val 只读，var 可变
来源：http://www.m.share.fehbvm.com/Article/details/gxwqhbihu.sHtML

[T03] Kotlin：字符串模板
来源：http://www.blog.fehbvm.com/Article/details/gzyndqmxl.sHtML

"值: $b"
来源：http://www.share.hesvh.cn/Article/details/gabvimiou.sHtML

[T04] Kotlin：空安全
来源：http://read.share.hesvh.cn/Article/details/gjjojqyvt.sHtML

val n: String? = null;  n?.length
来源：http://www.blog.fehbvm.com/Article/details/gexmbjaxz.sHtML

[T05] Kotlin：when 表达式
来源：http://www.share.zdbjq.cn/Article/details/gaoezeeza.sHtML

val s = when (x) { 1 -> "一" else -> "其他" }   // 多分支时每个分支单独一行
来源：http://mobile.hesvh.cn/Article/details/gjqverwtv.sHtML

[T06] Kotlin：集合映射
来源：http://mobile.fehbvm.com/Article/details/gzakmupmb.sHtML

listOf(1, 2, 3).map { it * 2 }
来源：http://3g.hesvh.cn/Article/details/gticdtgkf.sHtML

[T07] Kotlin：集合过滤
来源：http://mobile.hesvh.cn/Article/details/gxuhvewth.sHtML

listOf(1, 2, 3).filter { it > 1 }
来源：http://www.blog.zdbjq.cn/Article/details/gnukzzxps.sHtML

[T08] Kotlin：数据类
来源：http://blog.zdbjq.cn/Article/details/gssyerypn.sHtML

data class User(val name: String, val age: Int)
来源：http://www.m.share.fehbvm.com/Article/details/gytwafeun.sHtML

[T09] Kotlin：扩展函数
来源：http://read.share.fehbvm.com/Article/details/giaecmxlh.sHtML

fun String.exclaim() = this + "!"
来源：http://baike.zdbjq.cn/Article/details/gpspshpll.sHtML

[T10] Kotlin：默认参数
来源：http://read.share.hesvh.cn/Article/details/gdcuxdduh.sHtML

fun greet(name: String = "World") = "Hi $name"
来源：http://www.blog.fehbvm.com/Article/details/gfxujybye.sHtML

[T11] Kotlin：协程
来源：http://www.m.share.zdbjq.cn/Article/details/gkuirbqqs.sHtML

GlobalScope.launch { delay(1000); println("done") }
来源：http://blog.hesvh.cn/Article/details/ghycmgmmo.sHtML

[T12] Kotlin：解构声明
来源：http://read.share.hesvh.cn/Article/details/grbeyyxeq.sHtML

val (a, b) = Pair(1, 2)
来源：http://www.share.hesvh.cn/Article/details/gclrunupi.sHtML

[T13] Kotlin：只读 Map
来源：http://baike.zdbjq.cn/Article/details/gtcccbfwh.sHtML

val m = mapOf("a" to 1)
来源：http://www.m.share.fehbvm.com/Article/details/ggtevikfg.sHtML

[T14] Kotlin：循环
来源：http://www.share.zdbjq.cn/Article/details/gtvjdadct.sHtML

for (i in 1..10) println(i)
来源：http://blog.zdbjq.cn/Article/details/gvjhkcxqs.sHtML

[T15] Kotlin：接口
来源：http://wap.fehbvm.com/Article/details/gcjguajld.sHtML

interface Shape { fun area(): Double }
来源：http://3g.hesvh.cn/Article/details/ghjqssxat.sHtML

[T16] Swift：Hello World
来源：http://blog.fehbvm.com/Article/details/gcgejgkqu.sHtML

print("Hello")
来源：http://blog.hesvh.cn/Article/details/gufxdjdue.sHtML

[T17] Swift：变量与常量
来源：http://3g.hesvh.cn/Article/details/gsvxcvrfl.sHtML

var a = 1;  let b = 2
来源：http://m.share.zdbjq.cn/Article/details/glzsvuwtb.sHtML

[T18] Swift：字符串插值
来源：http://m.share.zdbjq.cn/Article/details/gvfkxdnfz.sHtML

"值: \(b)"
来源：http://baike.zdbjq.cn/Article/details/gtqyjvrfd.sHtML

[T19] Swift：可选绑定
来源：http://mobile.zdbjq.cn/Article/details/gifkdiuuq.sHtML

if let n = opt { print(n) }
来源：http://wap.fehbvm.com/Article/details/gbhztwcsy.sHtML

[T20] Swift：数组操作
来源：http://mobile.fehbvm.com/Article/details/gsxjcrgjl.sHtML

var a = [1, 2, 3];  a.append(4)
来源：http://baike.fehbvm.com/Article/details/ghwjwgada.sHtML

[T21] Swift：遍历
来源：http://www.blog.zdbjq.cn/Article/details/gxldezade.sHtML

for x in a { print(x) }
来源：http://read.share.hesvh.cn/Article/details/gkrxpiaqg.sHtML

[T22] Swift：字典
来源：http://www.share.zdbjq.cn/Article/details/gaqbznvxp.sHtML

var d = ["a": 1];  d["b"] = 2
来源：http://read.share.zdbjq.cn/Article/details/grqhqyami.sHtML

[T23] Swift：函数
来源：http://www.m.share.fehbvm.com/Article/details/gmbmuipud.sHtML

func add(_ a: Int, _ b: Int) -> Int { a + b }
来源：http://blog.hesvh.cn/Article/details/gtfebegtn.sHtML

[T24] Swift：闭包
来源：http://m.share.zdbjq.cn/Article/details/gqrtfmdja.sHtML

let f = { (x: Int) -> Int in x * 2 }
来源：http://www.share.zdbjq.cn/Article/details/galckwwnl.sHtML

[T25] Swift：结构体
来源：http://m.share.zdbjq.cn/Article/details/gpzbxymyb.sHtML

struct P { var x: Int }
来源：http://mobile.hesvh.cn/Article/details/gwpszvdte.sHtML

[T26] Swift：类与重写
来源：http://www.blog.fehbvm.com/Article/details/gvomgwsvy.sHtML

class A: Base { override func f() {} }
来源：http://www.m.share.hesvh.cn/Article/details/gidqccvya.sHtML

[T27] Swift：错误处理
来源：http://www.share.zdbjq.cn/Article/details/gqblbmoef.sHtML

do { try f() } catch { print(error) }
来源：http://www.blog.zdbjq.cn/Article/details/ghapciolv.sHtML

[T28] Swift：枚举
来源：http://blog.fehbvm.com/Article/details/gtdkxkita.sHtML

enum Color { case red, green }
来源：http://baike.fehbvm.com/Article/details/gogvnogcj.sHtML

[T29] Swift：guard 提前返回
来源：http://3g.zdbjq.cn/Article/details/grzndbctm.sHtML

guard let x = opt else { return }
来源：http://www.blog.hesvh.cn/Article/details/gfyjhvitd.sHtML

[T30] Swift：协议
来源：http://www.share.hesvh.cn/Article/details/gavmdrhta.sHtML

protocol Shape { func area() -> Double }
来源：http://m.share.zdbjq.cn/Article/details/gvrdbzhep.sHtML

[T31] Lua：Hello World
来源：http://blog.zdbjq.cn/Article/details/gwusbnrad.sHtML

print("Hello")
来源：http://www.share.zdbjq.cn/Article/details/gmjehheiw.sHtML

[T32] Lua：局部变量
来源：http://www.share.hesvh.cn/Article/details/grajmbpsy.sHtML

local a = 1
来源：http://www.share.fehbvm.com/Article/details/gpxvyckho.sHtML

[T33] Lua：表（数组）
来源：http://mobile.hesvh.cn/Article/details/gwtspjwzq.sHtML

local t = {1, 2, 3};  t[4] = 4
来源：http://wap.hesvh.cn/Article/details/gyytwmlua.sHtML

[T34] Lua：遍历表
来源：http://wap.hesvh.cn/Article/details/gqixugufc.sHtML

for i, v in ipairs(t) do print(i, v) end
来源：http://mobile.fehbvm.com/Article/details/gjcceadoj.sHtML

[T35] Lua：字典表
来源：http://mobile.hesvh.cn/Article/details/gkjplqzrf.sHtML

local d = { a = 1 };  d.b = 2
来源：http://3g.hesvh.cn/Article/details/gqxflhkal.sHtML

[T36] Lua：函数
来源：http://www.share.hesvh.cn/Article/details/gmjtfwzxl.sHtML

function add(a, b) return a + b end
来源：http://baike.zdbjq.cn/Article/details/gixsjgddg.sHtML

[T37] Lua：字符串拼接
来源：http://blog.fehbvm.com/Article/details/gqaccsuse.sHtML

"a" .. "b"
来源：http://wap.fehbvm.com/Article/details/gshnbpwal.sHtML

[T38] Lua：条件
来源：http://3g.fehbvm.com/Article/details/glcyixaew.sHtML

if x > 0 then print("正") end
来源：http://3g.fehbvm.com/Article/details/gjnwnaatq.sHtML

[T39] Lua：模式匹配
来源：http://3g.fehbvm.com/Article/details/gwewxkrou.sHtML

string.find(s, "%d+")
来源：http://wap.hesvh.cn/Article/details/gklhcncof.sHtML

[T40] Lua：元表
来源：http://m.share.hesvh.cn/Article/details/giaqbkmou.sHtML

setmetatable({}, { __index = base })
来源：http://baike.zdbjq.cn/Article/details/giiplhulj.sHtML

[T41] Perl：Hello World
来源：http://read.share.fehbvm.com/Article/details/gqzbiuaiv.sHtML

print "Hello\n";
来源：http://www.share.fehbvm.com/Article/details/gsxdmazdw.sHtML

[T42] Perl：变量类型
来源：http://3g.zdbjq.cn/Article/details/gnnlzmbec.sHtML

my $a = 1;  my @arr = (1, 2, 3);  my %h = (a => 1);
来源：http://mobile.zdbjq.cn/Article/details/gvxfqopvo.sHtML

[T43] Perl：字符串插值
来源：http://www.blog.zdbjq.cn/Article/details/gkemihbub.sHtML

"值: $a"
来源：http://wap.zdbjq.cn/Article/details/gkbajlfsr.sHtML

[T44] Perl：条件
来源：http://wap.hesvh.cn/Article/details/gkopgvduw.sHtML

if ($a > 0) { print "正"; }
来源：http://baike.zdbjq.cn/Article/details/gjkmelhyl.sHtML

[T45] Perl：数组遍历
来源：http://baike.zdbjq.cn/Article/details/guplpkkgy.sHtML

for my $x (@arr) { print $x; }
来源：http://blog.fehbvm.com/Article/details/gfwjebsmm.sHtML

[T46] Perl：哈希操作
来源：http://mobile.fehbvm.com/Article/details/gxngfamml.sHtML

$h{b} = 2;  for my $k (keys %h) { print "$k=$h{$k}"; }
来源：http://m.share.hesvh.cn/Article/details/gxnrejqjd.sHtML

[T47] Perl：正则捕获
来源：http://baike.fehbvm.com/Article/details/gbcvmbymu.sHtML

if ($s =~ /(\d+)/) { print $1; }
来源：http://wap.hesvh.cn/Article/details/ggiknmjmy.sHtML

[T48] Perl：正则替换
来源：http://www.blog.hesvh.cn/Article/details/gcvzphuwl.sHtML

$s =~ s/old/new/g;
来源：http://www.blog.hesvh.cn/Article/details/gajixsblj.sHtML

[T49] Perl：函数
来源：http://m.share.fehbvm.com/Article/details/glanewdzt.sHtML

sub add { my ($a, $b) = @_; return $a + $b; }
来源：http://www.share.hesvh.cn/Article/details/gwwqlgeoj.sHtML

[T50] Perl：逐行读文件
来源：http://www.m.share.fehbvm.com/Article/details/gldhtjmfl.sHtML

open my $fh, "<", "a.txt" or die $!;
来源：http://wap.fehbvm.com/Article/details/gujcythpz.sHtML

while (my $line = <$fh>) { print $line; }
来源：http://m.share.zdbjq.cn/Article/details/gtegygcmm.sHtML

[T51] Scala：Hello World
来源：http://baike.zdbjq.cn/Article/details/gtrzpskmk.sHtML

println("Hello")
来源：http://www.blog.zdbjq.cn/Article/details/geoljydzx.sHtML

[T52] Scala：变量
来源：http://www.blog.zdbjq.cn/Article/details/gxdcalmlq.sHtML

val a = 1;  var b = 2
来源：http://www.m.share.fehbvm.com/Article/details/ghibskwoe.sHtML

[T53] Scala：字符串插值
来源：http://read.share.hesvh.cn/Article/details/gludsozyu.sHtML

s"值: $b"
来源：http://www.blog.zdbjq.cn/Article/details/gdspniwdr.sHtML

[T54] Scala：集合映射
来源：http://read.share.fehbvm.com/Article/details/gdavebcus.sHtML

List(1, 2, 3).map(_ * 2)
来源：http://baike.zdbjq.cn/Article/details/gvwvannnh.sHtML

[T55] Scala：集合过滤
来源：http://www.blog.hesvh.cn/Article/details/gecgxlpwu.sHtML

List(1, 2, 3).filter(_ > 1)
来源：http://baike.hesvh.cn/Article/details/gubninxqf.sHtML

[T56] Scala：样例类
来源：http://www.share.fehbvm.com/Article/details/gcoqtvfdz.sHtML

case class User(name: String, age: Int)
来源：http://m.share.fehbvm.com/Article/details/glgbgnxjk.sHtML

[T57] Scala：模式匹配
来源：http://www.m.share.fehbvm.com/Article/details/gfbfyfplr.sHtML

x match { case 1 => "一"; case _ => "其他" }
来源：http://mobile.fehbvm.com/Article/details/gokyyfzlh.sHtML

[T58] Scala：函数定义
来源：http://3g.hesvh.cn/Article/details/getpybxhe.sHtML

def add(a: Int, b: Int): Int = a + b
来源：http://3g.hesvh.cn/Article/details/gimbvnxhv.sHtML

[T59] Scala：循环
来源：http://wap.zdbjq.cn/Article/details/glutyxjnv.sHtML

for (i <- 1 to 10) println(i)
来源：http://wap.fehbvm.com/Article/details/gjqpxolve.sHtML

[T60] Scala：折叠
来源：http://mobile.zdbjq.cn/Article/details/gkqfufvso.sHtML

List(1, 2, 3).foldLeft(0)(_ + _)
来源：http://www.share.fehbvm.com/Article/details/gwlmmwxwo.sHtML

================================================================================
来源：http://wap.hesvh.cn/Article/details/grdsmjxau.sHtML

U. 高频实用片段（Python / PHP / JavaScript 各 40 条）
来源：http://mobile.fehbvm.com/Article/details/gnlymjxnz.sHtML

================================================================================
来源：http://www.share.fehbvm.com/Article/details/gajqpdfms.sHtML

[U01] Py：创建虚拟环境
来源：http://www.blog.zdbjq.cn/Article/details/gwkfiitlc.sHtML

python -m venv .venv && source .venv/bin/activate
来源：http://www.m.share.hesvh.cn/Article/details/gelhxrbje.sHtML

[U02] Py：导出 / 安装依赖
来源：http://read.share.fehbvm.com/Article/details/gtbqbqeld.sHtML

pip freeze > requirements.txt;  pip install -r requirements.txt
来源：http://www.share.hesvh.cn/Article/details/gfpfkcyxj.sHtML

[U03] Py：加载 .env 配置
来源：http://blog.hesvh.cn/Article/details/goblicrrk.sHtML

from dotenv import load_dotenv; load_dotenv()
来源：http://read.share.fehbvm.com/Article/details/gypcmruxf.sHtML

[U04] Py：变量调试打印
来源：http://www.m.share.zdbjq.cn/Article/details/gieiwxvhy.sHtML

print(f"{x=}")            # 输出 x=值，Python 3.8+
来源：http://3g.fehbvm.com/Article/details/grvcsdqnx.sHtML

[U05] Py：列表去重且保序
来源：http://www.blog.hesvh.cn/Article/details/gtlgyvzrf.sHtML

list(dict.fromkeys(arr))
来源：http://3g.zdbjq.cn/Article/details/gzalxhyee.sHtML

[U06] Py：合并两个字典
来源：http://read.share.fehbvm.com/Article/details/gzaclfaqf.sHtML

{**a, **b}
来源：http://3g.fehbvm.com/Article/details/glfpjtlyu.sHtML

[U07] Py：反转字典键值
来源：http://www.share.hesvh.cn/Article/details/gkvdrqtjx.sHtML

{v: k for k, v in d.items()}
来源：http://www.m.share.fehbvm.com/Article/details/gjxkyadoo.sHtML

[U08] Py：展平二维列表
来源：http://mobile.fehbvm.com/Article/details/grirutkdo.sHtML

[y for x in nested for y in x]
来源：http://3g.fehbvm.com/Article/details/grjhapwpk.sHtML


<!-- 参考信息 -->