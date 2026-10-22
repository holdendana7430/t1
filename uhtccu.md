代发 wailian999

openssl rand -hex 16
来源：http://www.ydjk.org.cn/Article/details/gt2iqkczkmn.html

[R68] 计算文件校验值
来源：http://www.ydjk.org.cn/Article/details/gt2uodqwmbv.html

sha256sum a.txt;  md5sum a.txt
来源：http://www.ydjk.org.cn/Article/details/gt2iaslibvj.html

[R69] 生成随机密码
来源：http://www.ydjk.org.cn/Article/details/gt2guwlwljh.html

head -c 16 /dev/urandom | base64
来源：http://www.52xcode.cn/Article/details/gt2ydyljzno.html

[R70] 时间戳与互转
来源：http://www.ydjk.org.cn/Article/details/gt2niuljgnb.html

date +%s;  date -d @1700000000
来源：http://www.52xcode.cn/Article/details/gt2gdjzwbkg.html

[R71] 日期格式化
来源：http://www.ydjk.org.cn/Article/details/gt2kuwpojbf.html

date +"%Y-%m-%d %H:%M:%S"
来源：http://www.52xcode.cn/Article/details/gt2oitxbvdc.html

[R72] 等待端口就绪
来源：http://www.52xcode.cn/Article/details/gt2egjqobpb.html

until nc -z localhost 3306; do sleep 1; done
来源：http://www.ydjk.org.cn/Article/details/gt2rshfswqw.html

[R73] 分割大日志
来源：http://www.52xcode.cn/Article/details/gt2jtcypcql.html

split -l 1000 big.log part_
来源：http://www.ydjk.org.cn/Article/details/gt2wmhkbodh.html

[R74] 批量重命名
来源：http://www.ydjk.org.cn/Article/details/gt2ejwtwuie.html

for f in *.jpeg; do mv "$f" "${f%.jpeg}.jpg"; done
来源：http://www.ydjk.org.cn/Article/details/gt2vmlusxic.html

[R75] 导出环境变量
来源：http://www.ydjk.org.cn/Article/details/gt2mtcbvkyc.html

export PATH="$HOME/bin:$PATH"
来源：http://www.ydjk.org.cn/Article/details/gt2aeumkkbo.html

[R76] 使用临时文件
来源：http://www.ydjk.org.cn/Article/details/gt2ulekoszm.html

tmp=$(mktemp); trap 'rm -f "$tmp"' EXIT
来源：http://www.ydjk.org.cn/Article/details/gt2iamgtphh.html

[R77] 读取用户输入
来源：http://www.ydjk.org.cn/Article/details/gt2zfpjjlbm.html

read -rp "请输入: " ans
来源：http://www.ydjk.org.cn/Article/details/gt2fodrvyly.html

[R78] 交互式菜单
来源：http://www.ydjk.org.cn/Article/details/gt2srrsqsfk.html

select opt in a b c; do echo "$opt"; break; done
来源：http://www.52xcode.cn/Article/details/gt2cmwirciy.html

[R79] 解析命令行选项
来源：http://www.ydjk.org.cn/Article/details/gt2pbgmzmbw.html

while getopts "v:f:" o; do case $o in v) V=$OPTARG ;; f) F=$OPTARG ;; esac; done
来源：http://www.52xcode.cn/Article/details/gt2umhgoofw.html

[R80] 查看脚本执行耗时
来源：http://www.52xcode.cn/Article/details/gt2efgbxgju.html

time ./run.sh
来源：http://www.ydjk.org.cn/Article/details/gt2ryvjmkbk.html

================================================================================
来源：http://www.ydjk.org.cn/Article/details/gt2tiommedx.html

S. C / C++ 专题
来源：http://www.ydjk.org.cn/Article/details/gt2hzwovupm.html

================================================================================
来源：http://www.ydjk.org.cn/Article/details/gt2euxjyzve.html

[S01] C：Hello World
来源：http://www.ydjk.org.cn/Article/details/gt2qsjekkxx.html

#include <stdio.h>
来源：http://www.ydjk.org.cn/Article/details/gt2sierddfu.html

int main(void) { printf("Hello\n"); return 0; }
来源：http://www.52xcode.cn/Article/details/gt2flwoiexz.html

[S02] C：变量与格式化输出
来源：http://www.52xcode.cn/Article/details/gt2qwqvywmq.html

int a = 10; printf("%d\n", a);
来源：http://www.52xcode.cn/Article/details/gt2vhhtjdfl.html

[S03] C：读入整数
来源：http://www.ydjk.org.cn/Article/details/gt2gtsklbfz.html

int x; scanf("%d", &x);
来源：http://www.52xcode.cn/Article/details/gt2tztytbyg.html

[S04] C：字符串复制
来源：http://www.52xcode.cn/Article/details/gt2wnpctopc.html

char dst[32]; strcpy(dst, "hi");
来源：http://www.ydjk.org.cn/Article/details/gt2hyfufoet.html

[S05] C：字符串长度
来源：http://www.ydjk.org.cn/Article/details/gt2ekowonjx.html

strlen(s)
来源：http://www.ydjk.org.cn/Article/details/gt2ydqilhrk.html

[S06] C：字符串比较
来源：http://www.52xcode.cn/Article/details/gt2yugjgvhh.html

strcmp(a, b) == 0
来源：http://www.ydjk.org.cn/Article/details/gt2qanpmzaj.html

[S07] C：数组遍历求和
来源：http://www.52xcode.cn/Article/details/gt2coloqazn.html

for (int i = 0; i < n; i++) sum += a[i];
来源：http://www.ydjk.org.cn/Article/details/gt2wyhoajyx.html

[S08] C：动态内存分配与释放
来源：http://www.ydjk.org.cn/Article/details/gt2afztygfk.html

int *p = malloc(sizeof(int) * n); ... free(p);
来源：http://www.ydjk.org.cn/Article/details/gt2stvimdaz.html

[S09] C：结构体定义与初始化
来源：http://www.52xcode.cn/Article/details/gt2mkzpqykc.html

struct Point { int x, y; };  struct Point p = {1, 2};
来源：http://www.ydjk.org.cn/Article/details/gt2zlndmxbu.html

[S10] C：指针与解引用
来源：http://www.ydjk.org.cn/Article/details/gt2yiweflkf.html

int *p = &a;  *p = 5;
来源：http://www.ydjk.org.cn/Article/details/gt2quemqkje.html

[S11] C：逐行读文件
来源：http://www.ydjk.org.cn/Article/details/gt2oqxgdywe.html

FILE *f = fopen("a.txt", "r");
来源：http://www.ydjk.org.cn/Article/details/gt2kblxttgj.html

while (fgets(buf, sizeof buf, f)) { }
来源：http://www.52xcode.cn/Article/details/gt2tjvbnrfn.html

fclose(f);
来源：http://www.ydjk.org.cn/Article/details/gt2quaqehjl.html

[S12] C：写文件
来源：http://www.ydjk.org.cn/Article/details/gt2tpnjrxgm.html

FILE *f = fopen("a.txt", "w");  fprintf(f, "hi\n");  fclose(f);
来源：http://www.ydjk.org.cn/Article/details/gt2vsgupjxv.html

[S13] C：宏定义
来源：http://www.52xcode.cn/Article/details/gt2bhbwclnc.html

#define MAX(a, b) ((a) > (b) ? (a) : (b))
来源：http://www.ydjk.org.cn/Article/details/gt2brcnaiey.html

[S14] C：枚举
来源：http://www.52xcode.cn/Article/details/gt2bguduukf.html

enum Color { RED, GREEN, BLUE };
来源：http://www.52xcode.cn/Article/details/gt2lcqyfbjg.html

[S15] C：类型转换
来源：http://www.ydjk.org.cn/Article/details/gt2ojnjnpwb.html

(double) a / b
来源：http://www.ydjk.org.cn/Article/details/gt2qkaiopui.html

[S16] C：位操作置位
来源：http://www.52xcode.cn/Article/details/gt2lmfrrwys.html

x |= (1 << 3);
来源：http://www.52xcode.cn/Article/details/gt2ylhnsgrd.html

[S17] C：安全拼接字符串
来源：http://www.ydjk.org.cn/Article/details/gt2fthdydby.html

snprintf(buf, sizeof buf, "%s%s", a, b);
来源：http://www.ydjk.org.cn/Article/details/gt2yycqonhn.html

[S18] C：命令行参数
来源：http://www.ydjk.org.cn/Article/details/gt2hkwrlpzt.html

int main(int argc, char **argv)
来源：http://www.52xcode.cn/Article/details/gt2xqriguuu.html

[S19] C：快速排序
来源：http://www.52xcode.cn/Article/details/gt2jjxhicct.html

qsort(a, n, sizeof(int), cmp);
来源：http://www.ydjk.org.cn/Article/details/gt2lztcvtsu.html

[S20] C：二分查找
来源：http://www.52xcode.cn/Article/details/gt2rggnixrt.html

bsearch(&key, a, n, sizeof(int), cmp);
来源：http://www.52xcode.cn/Article/details/gt2ymhvmisq.html

[S21] C：字符类别判断
来源：http://www.ydjk.org.cn/Article/details/gt2nrladagq.html

isdigit(c);  isalpha(c);  isspace(c);
来源：http://www.52xcode.cn/Article/details/gt2nuifuitj.html

[S22] C：字符串转数字
来源：http://www.52xcode.cn/Article/details/gt2cdkdrhun.html

atoi("42");  strtod("3.14", NULL);
来源：http://www.52xcode.cn/Article/details/gt2uweqhjfa.html

[S23] C：随机数
来源：http://www.52xcode.cn/Article/details/gt2chwtrmqy.html

srand(time(NULL));  int r = rand() % 100;
来源：http://www.ydjk.org.cn/Article/details/gt2xmvlshtv.html

[S24] C：获取本地时间
来源：http://www.ydjk.org.cn/Article/details/gt2pyjotuqw.html

time_t t = time(NULL);  struct tm *tm = localtime(&t);
来源：http://www.ydjk.org.cn/Article/details/gt2ndrytnys.html

[S25] C：内存拷贝
来源：http://www.52xcode.cn/Article/details/gt2anysnpyg.html

memcpy(dst, src, n);
来源：http://www.52xcode.cn/Article/details/gt2dwksopny.html

[S26] C：内存清零
来源：http://www.ydjk.org.cn/Article/details/gt2mrtgacgn.html

memset(a, 0, sizeof a);
来源：http://www.52xcode.cn/Article/details/gt2evkvafsq.html

[S27] C：定义常量
来源：http://www.52xcode.cn/Article/details/gt2mrbapgoq.html

const double PI = 3.14159;
来源：http://www.ydjk.org.cn/Article/details/gt2abscpogk.html

[S28] C：静态变量
来源：http://www.ydjk.org.cn/Article/details/gt2kpbtzxay.html

static int counter = 0;
来源：http://www.52xcode.cn/Article/details/gt2uwxuhaqp.html

[S29] C：变参函数
来源：http://www.ydjk.org.cn/Article/details/gt2flzwwfrg.html

va_list ap; va_start(ap, fmt); vprintf(fmt, ap); va_end(ap);
来源：http://www.52xcode.cn/Article/details/gt2aplyeezc.html

[S30] C：头文件保护
来源：http://www.ydjk.org.cn/Article/details/gt2svzgodlt.html

#ifndef X_H
来源：http://www.52xcode.cn/Article/details/gt2gdvtcqyu.html

#define X_H
来源：http://www.52xcode.cn/Article/details/gt2nksvbfdz.html

#endif
来源：http://www.52xcode.cn/Article/details/gt2nryxsfgi.html

[S31] C++：Hello World
来源：http://www.ydjk.org.cn/Article/details/gt2oeweszkq.html

#include <iostream>
来源：http://www.ydjk.org.cn/Article/details/gt2xwjazlwk.html

int main() { std::cout << "Hello\n"; }
来源：http://www.52xcode.cn/Article/details/gt2glizkyjr.html

[S32] C++：字符串
来源：http://www.ydjk.org.cn/Article/details/gt2tbfrtjbq.html

std::string s = "hi";  s += "!";
来源：http://www.ydjk.org.cn/Article/details/gt2qtnavvfi.html

[S33] C++：vector 增删
来源：http://www.52xcode.cn/Article/details/gt2jsnujnkr.html

std::vector<int> v{1, 2, 3};  v.push_back(4);
来源：http://www.52xcode.cn/Article/details/gt2kozfezwa.html

[S34] C++：遍历 vector
来源：http://www.ydjk.org.cn/Article/details/gt2ctvpjrfr.html

for (auto &x : v) { std::cout << x; }
来源：http://www.52xcode.cn/Article/details/gt2vohvchpm.html

[S35] C++：map
来源：http://www.ydjk.org.cn/Article/details/gt2stkmalxn.html

std::map<std::string, int> m;  m["a"] = 1;
来源：http://www.ydjk.org.cn/Article/details/gt2otivdljj.html

[S36] C++：unordered_map
来源：http://www.ydjk.org.cn/Article/details/gt2rfapizmm.html

std::unordered_map<std::string, int> m;  m["a"] = 1;
来源：http://www.52xcode.cn/Article/details/gt2ylfctbqe.html

[S37] C++：set
来源：http://www.ydjk.org.cn/Article/details/gt2ofajhgpi.html

std::set<int> s{1, 2, 3};  s.insert(4);
来源：http://www.ydjk.org.cn/Article/details/gt2kwhcglue.html

[S38] C++：排序
来源：http://www.52xcode.cn/Article/details/gt2gaiausgf.html

std::sort(v.begin(), v.end());
来源：http://www.ydjk.org.cn/Article/details/gt2zoevtnny.html

[S39] C++：自定义比较器排序
来源：http://www.52xcode.cn/Article/details/gt2ggxnmrdy.html

std::sort(v.begin(), v.end(), [](int a, int b) { return a > b; });
来源：http://www.52xcode.cn/Article/details/gt2iuoikgah.html

[S40] C++：查找元素
来源：http://www.52xcode.cn/Article/details/gt2yutaryog.html

auto it = std::find(v.begin(), v.end(), 3);
来源：http://www.ydjk.org.cn/Article/details/gt2zkxgmrbj.html

[S41] C++：类与构造函数
来源：http://www.52xcode.cn/Article/details/gt2qtwzlkhc.html

class A { public: A(int v) : x_(v) {} int get() const { return x_; } private: int x_; };
来源：http://www.52xcode.cn/Article/details/gt2ktkanyly.html

[S42] C++：继承与虚函数
来源：http://www.52xcode.cn/Article/details/gt2hysecfws.html

class B : public Base { public: void f() override {} };
来源：http://www.52xcode.cn/Article/details/gt2wmjzbwvu.html

[S43] C++：智能指针
来源：http://www.52xcode.cn/Article/details/gt2nhhegxvq.html

auto p = std::make_unique<int>(5);
来源：http://www.52xcode.cn/Article/details/gt2twcfgjof.html

[S44] C++：引用传参
来源：http://www.ydjk.org.cn/Article/details/gt2vsfwnihi.html

void inc(int &x) { ++x; }
来源：http://www.52xcode.cn/Article/details/gt2wsnymetr.html

[S45] C++：lambda
来源：http://www.ydjk.org.cn/Article/details/gt2mpzxinfv.html

auto add = [](int a, int b) { return a + b; };
来源：http://www.ydjk.org.cn/Article/details/gt2fpgajlem.html

[S46] C++：函数模板
来源：http://www.ydjk.org.cn/Article/details/gt2otspjczn.html

template <typename T> T maxv(T a, T b) { return a > b ? a : b; }
来源：http://www.ydjk.org.cn/Article/details/gt2ggmuaphq.html

[S47] C++：结构化绑定遍历
来源：http://www.52xcode.cn/Article/details/gt2zxobzbhj.html

for (const auto &[k, v] : m) { std::cout << k << v; }
来源：http://www.52xcode.cn/Article/details/gt2qgsniegl.html

[S48] C++：逐行读文件
来源：http://www.52xcode.cn/Article/details/gt2aqwwzuio.html

std::ifstream in("a.txt");  std::string line;
来源：http://www.ydjk.org.cn/Article/details/gt2kqextbfh.html

while (std::getline(in, line)) { }
来源：http://www.52xcode.cn/Article/details/gt2duuifmby.html

[S49] C++：写文件
来源：http://www.52xcode.cn/Article/details/gt2vxuvspdk.html

std::ofstream out("a.txt");  out << "hi\n";
来源：http://www.52xcode.cn/Article/details/gt2lsegzzrp.html

[S50] C++：格式化数字
来源：http://www.ydjk.org.cn/Article/details/gt2dqevfqgg.html

std::ostringstream os;  os << std::fixed << std::setprecision(2) << 3.14159;
来源：http://www.52xcode.cn/Article/details/gt2abxvlrcs.html

[S51] C++：显式类型转换
来源：http://www.52xcode.cn/Article/details/gt2xpvveqco.html

static_cast<double>(a) / b
来源：http://www.ydjk.org.cn/Article/details/gt2sjtwjtow.html

[S52] C++：const 与 noexcept
来源：http://www.52xcode.cn/Article/details/gt2qsgbbwso.html

int size() const noexcept { return n_; }
来源：http://www.52xcode.cn/Article/details/gt2dywmbziz.html

[S53] C++：移动语义
来源：http://www.ydjk.org.cn/Article/details/gt2pcesppet.html

std::vector<int> w = std::move(v);
来源：http://www.52xcode.cn/Article/details/gt2ajxbmbfu.html

[S54] C++：异常处理
来源：http://www.ydjk.org.cn/Article/details/gt2xuxbgrgc.html

try { throw std::runtime_error("x"); } catch (const std::exception &e) { }
来源：http://www.ydjk.org.cn/Article/details/gt2ivaobyxr.html

[S55] C++：结构化绑定
来源：http://www.ydjk.org.cn/Article/details/gt2ytddnmfw.html

auto [a, b] = std::make_pair(1, 2);
来源：http://www.ydjk.org.cn/Article/details/gt2hphpvbob.html

[S56] C++：optional
来源：http://www.ydjk.org.cn/Article/details/gt2wlkcuzbs.html

std::optional<int> o = 5;  if (o) { int v = *o; }
来源：http://www.52xcode.cn/Article/details/gt2tpmegsna.html

[S57] C++：编译期常量
来源：http://www.ydjk.org.cn/Article/details/gt2ofjffufx.html

constexpr int N = 10;
来源：http://www.ydjk.org.cn/Article/details/gt2yfrmorgg.html

[S58] C++：命名空间
来源：http://www.52xcode.cn/Article/details/gt2mjwiqowd.html

namespace ns { int f() { return 1; } }
来源：http://www.52xcode.cn/Article/details/gt2xqhxcpsi.html

[S59] C++：静态断言
来源：http://www.52xcode.cn/Article/details/gt2wpyxlmny.html

static_assert(sizeof(int) == 4, "int 必须 4 字节");
来源：http://www.52xcode.cn/Article/details/gt2twgrqnuv.html

[S60] C++：遍历并删除元素
来源：http://www.ydjk.org.cn/Article/details/gt2ghwkomsp.html

v.erase(std::remove_if(v.begin(), v.end(), [](int x) { return x < 0; }), v.end());
来源：http://www.52xcode.cn/Article/details/gt2svhqkxtn.html

================================================================================
来源：http://www.52xcode.cn/Article/details/gt2ankmlswr.html

T. 其他语言补充（Kotlin / Swift / Lua / Perl / Scala）
来源：http://www.ydjk.org.cn/Article/details/gt2mrfcdoju.html

================================================================================
来源：http://www.ydjk.org.cn/Article/details/gt2byirdyun.html

[T01] Kotlin：Hello World
来源：http://www.52xcode.cn/Article/details/gt2osmdgpcw.html

println("Hello")
来源：http://www.52xcode.cn/Article/details/gt2tvjwneee.html

[T02] Kotlin：变量
来源：http://www.ydjk.org.cn/Article/details/gt2nbqtnpaw.html

val a = 1;  var b = 2        // val 只读，var 可变
来源：http://www.52xcode.cn/Article/details/gt2wbnbwlrl.html

[T03] Kotlin：字符串模板
来源：http://www.ydjk.org.cn/Article/details/gt2pabokelr.html

"值: $b"
来源：http://www.52xcode.cn/Article/details/gt2iawlifcj.html

[T04] Kotlin：空安全
来源：http://www.52xcode.cn/Article/details/gt2pseewfvm.html

val n: String? = null;  n?.length
来源：http://www.ydjk.org.cn/Article/details/gt2ofdlxmba.html

[T05] Kotlin：when 表达式
来源：http://www.ydjk.org.cn/Article/details/gt2vhqutpwa.html

val s = when (x) { 1 -> "一" else -> "其他" }   // 多分支时每个分支单独一行
来源：http://www.52xcode.cn/Article/details/gt2raicwiem.html

[T06] Kotlin：集合映射
来源：http://www.ydjk.org.cn/Article/details/gt2xhucydft.html

listOf(1, 2, 3).map { it * 2 }
来源：http://www.ydjk.org.cn/Article/details/gt2mamyynmp.html

[T07] Kotlin：集合过滤
来源：http://www.ydjk.org.cn/Article/details/gt2bhadzcjq.html

listOf(1, 2, 3).filter { it > 1 }
来源：http://www.52xcode.cn/Article/details/gt2jocwgsxk.html

[T08] Kotlin：数据类
来源：http://www.ydjk.org.cn/Article/details/gt2jvxgmluz.html

data class User(val name: String, val age: Int)
来源：http://www.52xcode.cn/Article/details/gt2ravnsojb.html

[T09] Kotlin：扩展函数
来源：http://www.ydjk.org.cn/Article/details/gt2lqwyilji.html

fun String.exclaim() = this + "!"
来源：http://www.52xcode.cn/Article/details/gt2tmpheckt.html

[T10] Kotlin：默认参数
来源：http://www.52xcode.cn/Article/details/gt2gexnpmbv.html

fun greet(name: String = "World") = "Hi $name"
来源：http://www.52xcode.cn/Article/details/gt2ukeiymte.html

[T11] Kotlin：协程
来源：http://www.52xcode.cn/Article/details/gt2kovyqcmm.html

GlobalScope.launch { delay(1000); println("done") }
来源：http://www.52xcode.cn/Article/details/gt2euynmjrb.html

[T12] Kotlin：解构声明
来源：http://www.52xcode.cn/Article/details/gt2lolsopsv.html

val (a, b) = Pair(1, 2)
来源：http://www.52xcode.cn/Article/details/gt2yrkzoaht.html

[T13] Kotlin：只读 Map
来源：http://www.52xcode.cn/Article/details/gt2dwhvytin.html

val m = mapOf("a" to 1)
来源：http://www.ydjk.org.cn/Article/details/gt2qdaponpi.html

[T14] Kotlin：循环
来源：http://www.ydjk.org.cn/Article/details/gt2zrwjjzmc.html

for (i in 1..10) println(i)
来源：http://www.52xcode.cn/Article/details/gt2pnahsrzq.html

[T15] Kotlin：接口
来源：http://www.52xcode.cn/Article/details/gt2tulcpyqi.html

interface Shape { fun area(): Double }
来源：http://www.52xcode.cn/Article/details/gt2folwvgms.html

[T16] Swift：Hello World
来源：http://www.52xcode.cn/Article/details/gt2wdiejmko.html

print("Hello")
来源：http://www.52xcode.cn/Article/details/gt2psbdfdlt.html

[T17] Swift：变量与常量
来源：http://www.52xcode.cn/Article/details/gt2pdvepfux.html

var a = 1;  let b = 2
来源：http://www.52xcode.cn/Article/details/gt2xfghsego.html

[T18] Swift：字符串插值
来源：http://www.52xcode.cn/Article/details/gt2bpfsxlzb.html

"值: \(b)"
来源：http://www.ydjk.org.cn/Article/details/gt2hurkhsxw.html

[T19] Swift：可选绑定
来源：http://www.52xcode.cn/Article/details/gt2catzwdca.html

if let n = opt { print(n) }
来源：http://www.52xcode.cn/Article/details/gt2exypwgfz.html

[T20] Swift：数组操作
来源：http://www.52xcode.cn/Article/details/gt2bxalskop.html

var a = [1, 2, 3];  a.append(4)
来源：http://www.52xcode.cn/Article/details/gt2lhennaiw.html

[T21] Swift：遍历
来源：http://www.52xcode.cn/Article/details/gt2psddwybj.html

for x in a { print(x) }
来源：http://www.ydjk.org.cn/Article/details/gt2mjyfdtqe.html

[T22] Swift：字典
来源：http://www.ydjk.org.cn/Article/details/gt2yyurjhir.html

var d = ["a": 1];  d["b"] = 2
来源：http://www.ydjk.org.cn/Article/details/gt2lepxongq.html

[T23] Swift：函数
来源：http://www.52xcode.cn/Article/details/gt2cbepskvl.html

func add(_ a: Int, _ b: Int) -> Int { a + b }
来源：http://www.52xcode.cn/Article/details/gt2ocqgfhhr.html

[T24] Swift：闭包
来源：http://www.52xcode.cn/Article/details/gt2reqbmwzn.html

let f = { (x: Int) -> Int in x * 2 }
来源：http://www.ydjk.org.cn/Article/details/gt2chzndjal.html

[T25] Swift：结构体
来源：http://www.ydjk.org.cn/Article/details/gt2cjkjhkbb.html

struct P { var x: Int }
来源：http://www.ydjk.org.cn/Article/details/gt2sjicdfoz.html

[T26] Swift：类与重写
来源：http://www.52xcode.cn/Article/details/gt2mzyvoatz.html

class A: Base { override func f() {} }
来源：http://www.ydjk.org.cn/Article/details/gt2kmnxlvbs.html

[T27] Swift：错误处理
来源：http://www.52xcode.cn/Article/details/gt2sfotfdoa.html

do { try f() } catch { print(error) }
来源：http://www.52xcode.cn/Article/details/gt2nxiihxoi.html

[T28] Swift：枚举
来源：http://www.52xcode.cn/Article/details/gt2gahixfaa.html

enum Color { case red, green }
来源：http://www.ydjk.org.cn/Article/details/gt2pbafipig.html

[T29] Swift：guard 提前返回
来源：http://www.ydjk.org.cn/Article/details/gt2bqolnipc.html

guard let x = opt else { return }
来源：http://www.ydjk.org.cn/Article/details/gt2qnygnfff.html

[T30] Swift：协议
来源：http://www.52xcode.cn/Article/details/gt2zyjewixa.html

protocol Shape { func area() -> Double }
来源：http://www.52xcode.cn/Article/details/gt2ekrsxdxa.html

[T31] Lua：Hello World
来源：http://www.ydjk.org.cn/Article/details/gt2fktqbffm.html

print("Hello")
来源：http://www.52xcode.cn/Article/details/gt2mwuyezur.html

[T32] Lua：局部变量
来源：http://www.52xcode.cn/Article/details/gt2matedsfp.html

local a = 1
来源：http://www.52xcode.cn/Article/details/gt2zqpaabsd.html

[T33] Lua：表（数组）
来源：http://www.ydjk.org.cn/Article/details/gt2wddafewo.html

local t = {1, 2, 3};  t[4] = 4
来源：http://www.52xcode.cn/Article/details/gt2tynxteyg.html

[T34] Lua：遍历表
来源：http://www.ydjk.org.cn/Article/details/gt2sqkjknlg.html

for i, v in ipairs(t) do print(i, v) end
来源：http://www.ydjk.org.cn/Article/details/gt2jhrpshoa.html

[T35] Lua：字典表
来源：http://www.52xcode.cn/Article/details/gt2okzfoveu.html

local d = { a = 1 };  d.b = 2
来源：http://www.52xcode.cn/Article/details/gt2fpnalkyu.html

[T36] Lua：函数
来源：http://www.52xcode.cn/Article/details/gt2ouovugof.html

function add(a, b) return a + b end
来源：http://www.52xcode.cn/Article/details/gt2xywatxsw.html

[T37] Lua：字符串拼接
来源：http://www.ydjk.org.cn/Article/details/gt2fwlflyib.html

"a" .. "b"
来源：http://www.52xcode.cn/Article/details/gt2axpphpmo.html

[T38] Lua：条件
来源：http://www.ydjk.org.cn/Article/details/gt2nebhqbco.html

if x > 0 then print("正") end
来源：http://www.ydjk.org.cn/Article/details/gt2wruyktdi.html

[T39] Lua：模式匹配
来源：http://www.ydjk.org.cn/Article/details/gt2mzkabaak.html

string.find(s, "%d+")
来源：http://www.ydjk.org.cn/Article/details/gt2qtcnsllm.html

[T40] Lua：元表
来源：http://www.52xcode.cn/Article/details/gt2nseuxeoy.html

setmetatable({}, { __index = base })
来源：http://www.ydjk.org.cn/Article/details/gt2orlfbwea.html

[T41] Perl：Hello World
来源：http://www.ydjk.org.cn/Article/details/gt2qonngmpk.html

print "Hello\n";
来源：http://www.ydjk.org.cn/Article/details/gt2dqzrowgp.html

[T42] Perl：变量类型
来源：http://www.ydjk.org.cn/Article/details/gt2lmqyuqir.html

my $a = 1;  my @arr = (1, 2, 3);  my %h = (a => 1);
来源：http://www.52xcode.cn/Article/details/gt2tzqywdar.html

[T43] Perl：字符串插值
来源：http://www.52xcode.cn/Article/details/gt2pzshfqov.html

"值: $a"
来源：http://www.52xcode.cn/Article/details/gt2xovtfvze.html

[T44] Perl：条件
来源：http://www.ydjk.org.cn/Article/details/gt2swbkbxrl.html

if ($a > 0) { print "正"; }
来源：http://www.52xcode.cn/Article/details/gt2eiamoela.html

[T45] Perl：数组遍历
来源：http://www.ydjk.org.cn/Article/details/gt2awkamjro.html

for my $x (@arr) { print $x; }
来源：http://www.52xcode.cn/Article/details/gt2xyskycys.html

[T46] Perl：哈希操作
来源：http://www.ydjk.org.cn/Article/details/gt2aomrptua.html

$h{b} = 2;  for my $k (keys %h) { print "$k=$h{$k}"; }
来源：http://www.ydjk.org.cn/Article/details/gt2vnkfvrxc.html

[T47] Perl：正则捕获
来源：http://www.52xcode.cn/Article/details/gt2cwufjhmw.html

if ($s =~ /(\d+)/) { print $1; }
来源：http://www.ydjk.org.cn/Article/details/gt2smlsqwqy.html

[T48] Perl：正则替换
来源：http://www.52xcode.cn/Article/details/gt2biupmmcn.html

$s =~ s/old/new/g;
来源：http://www.ydjk.org.cn/Article/details/gt2wxqlazwp.html

[T49] Perl：函数
来源：http://www.52xcode.cn/Article/details/gt2fphhysnm.html

sub add { my ($a, $b) = @_; return $a + $b; }
来源：http://www.52xcode.cn/Article/details/gt2urkscdae.html

[T50] Perl：逐行读文件
来源：http://www.52xcode.cn/Article/details/gt2dwbzoaak.html

open my $fh, "<", "a.txt" or die $!;
来源：http://www.ydjk.org.cn/Article/details/gt2jsxtdwmp.html

while (my $line = <$fh>) { print $line; }
来源：http://www.52xcode.cn/Article/details/gt2pptvqjmy.html

[T51] Scala：Hello World
来源：http://www.ydjk.org.cn/Article/details/gt2epvyoupz.html

println("Hello")
来源：http://www.ydjk.org.cn/Article/details/gt2cxblghbb.html

[T52] Scala：变量
来源：http://www.52xcode.cn/Article/details/gt2dsgcmhje.html

val a = 1;  var b = 2
来源：http://www.ydjk.org.cn/Article/details/gt2mlwgdrtp.html

[T53] Scala：字符串插值
来源：http://www.52xcode.cn/Article/details/gt2mngiawaz.html

s"值: $b"
来源：http://www.52xcode.cn/Article/details/gt2eggdfetj.html

[T54] Scala：集合映射
来源：http://www.ydjk.org.cn/Article/details/gt2bpzdmpwg.html

List(1, 2, 3).map(_ * 2)
来源：http://www.ydjk.org.cn/Article/details/gt2slyksrvd.html

[T55] Scala：集合过滤
来源：http://www.ydjk.org.cn/Article/details/gt2ropapsoq.html

List(1, 2, 3).filter(_ > 1)
来源：http://www.52xcode.cn/Article/details/gt2ynrvygzc.html

[T56] Scala：样例类
来源：http://www.52xcode.cn/Article/details/gt2zsnhtdet.html

case class User(name: String, age: Int)
来源：http://www.52xcode.cn/Article/details/gt2rlrtzpuj.html

[T57] Scala：模式匹配
来源：http://www.52xcode.cn/Article/details/gt2lwtzrvjl.html

x match { case 1 => "一"; case _ => "其他" }
来源：http://www.52xcode.cn/Article/details/gt2rpnuilsr.html

[T58] Scala：函数定义
来源：http://www.ydjk.org.cn/Article/details/gt2cjvkgvjz.html

def add(a: Int, b: Int): Int = a + b
来源：http://www.ydjk.org.cn/Article/details/gt2ttblujmj.html

[T59] Scala：循环
来源：http://www.52xcode.cn/Article/details/gt2fwkdioqe.html

for (i <- 1 to 10) println(i)
来源：http://www.ydjk.org.cn/Article/details/gt2kzwgykgw.html

[T60] Scala：折叠
来源：http://www.ydjk.org.cn/Article/details/gt2ykwyjquy.html

List(1, 2, 3).foldLeft(0)(_ + _)
来源：http://www.52xcode.cn/Article/details/gt2pqzarkyf.html

================================================================================
来源：http://www.52xcode.cn/Article/details/gt2xumiaktf.html

U. 高频实用片段（Python / PHP / JavaScript 各 40 条）
来源：http://www.52xcode.cn/Article/details/gt2ssodbmwf.html

================================================================================
来源：http://www.ydjk.org.cn/Article/details/gt2mrnzzjug.html

[U01] Py：创建虚拟环境
来源：http://www.52xcode.cn/Article/details/gt2dpkovotx.html

python -m venv .venv && source .venv/bin/activate
来源：http://www.52xcode.cn/Article/details/gt2yjwnkhkg.html

[U02] Py：导出 / 安装依赖
来源：http://www.ydjk.org.cn/Article/details/gt2hhwypnhi.html

pip freeze > requirements.txt;  pip install -r requirements.txt
来源：http://www.52xcode.cn/Article/details/gt2vofxjwbi.html

[U03] Py：加载 .env 配置
来源：http://www.ydjk.org.cn/Article/details/gt2alkqtwvh.html

from dotenv import load_dotenv; load_dotenv()
来源：http://www.52xcode.cn/Article/details/gt2taxtdbbi.html

[U04] Py：变量调试打印
来源：http://www.52xcode.cn/Article/details/gt2lyqalztv.html

print(f"{x=}")            # 输出 x=值，Python 3.8+
来源：http://www.52xcode.cn/Article/details/gt2xpojogbb.html

[U05] Py：列表去重且保序
来源：http://www.ydjk.org.cn/Article/details/gt2wkhkhxug.html

list(dict.fromkeys(arr))
来源：http://www.52xcode.cn/Article/details/gt2tdxdljnv.html

[U06] Py：合并两个字典
来源：http://www.52xcode.cn/Article/details/gt2xulxkkom.html

{**a, **b}
来源：http://www.52xcode.cn/Article/details/gt2xdlfiuii.html

[U07] Py：反转字典键值
来源：http://www.ydjk.org.cn/Article/details/gt2kwwguabb.html

{v: k for k, v in d.items()}
来源：http://www.52xcode.cn/Article/details/gt2kvydbont.html

[U08] Py：展平二维列表
来源：http://www.52xcode.cn/Article/details/gt2jaxdzmpu.html

[y for x in nested for y in x]
来源：http://www.ydjk.org.cn/Article/details/gt2jtxowauc.html


<!-- 参考信息 -->