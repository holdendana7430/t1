代发 wailian999

ss -tlnp | grep 8080;  lsof -i:8080
来源：http://www.52xcode.cn/Article/details/gt3nwxuqekg.html

[R66] 定时任务
来源：http://www.ydjk.org.cn/Article/details/gt3pxpaxnji.html

crontab -e;  crontab -l
来源：http://www.52xcode.cn/Article/details/gt3vpnobzhy.html

[R67] 生成随机十六进制串
来源：http://www.ydjk.org.cn/Article/details/gt3mlzwkfqe.html

openssl rand -hex 16
来源：http://www.ydjk.org.cn/Article/details/gt3aehxdzwi.html

[R68] 计算文件校验值
来源：http://www.52xcode.cn/Article/details/gt3ssfiasih.html

sha256sum a.txt;  md5sum a.txt
来源：http://www.52xcode.cn/Article/details/gt3tcintmtx.html

[R69] 生成随机密码
来源：http://www.52xcode.cn/Article/details/gt3kkfcifgh.html

head -c 16 /dev/urandom | base64
来源：http://www.52xcode.cn/Article/details/gt3nbahxfuw.html

[R70] 时间戳与互转
来源：http://www.ydjk.org.cn/Article/details/gt3prfxpqkj.html

date +%s;  date -d @1700000000
来源：http://www.52xcode.cn/Article/details/gt3fivqyjss.html

[R71] 日期格式化
来源：http://www.ydjk.org.cn/Article/details/gt3wdjkkinr.html

date +"%Y-%m-%d %H:%M:%S"
来源：http://www.52xcode.cn/Article/details/gt3kxnntvmh.html

[R72] 等待端口就绪
来源：http://www.52xcode.cn/Article/details/gt3suakesgr.html

until nc -z localhost 3306; do sleep 1; done
来源：http://www.52xcode.cn/Article/details/gt3dsjljitw.html

[R73] 分割大日志
来源：http://www.ydjk.org.cn/Article/details/gt3jfjrrndh.html

split -l 1000 big.log part_
来源：http://www.52xcode.cn/Article/details/gt3kekzbfgs.html

[R74] 批量重命名
来源：http://www.ydjk.org.cn/Article/details/gt3xuzqmrys.html

for f in *.jpeg; do mv "$f" "${f%.jpeg}.jpg"; done
来源：http://www.52xcode.cn/Article/details/gt3qzbpcdux.html

[R75] 导出环境变量
来源：http://www.52xcode.cn/Article/details/gt3esmvgdiu.html

export PATH="$HOME/bin:$PATH"
来源：http://www.ydjk.org.cn/Article/details/gt3tkbyumsk.html

[R76] 使用临时文件
来源：http://www.52xcode.cn/Article/details/gt3wigjgiad.html

tmp=$(mktemp); trap 'rm -f "$tmp"' EXIT
来源：http://www.ydjk.org.cn/Article/details/gt3fcukptxw.html

[R77] 读取用户输入
来源：http://www.52xcode.cn/Article/details/gt3pvsajtin.html

read -rp "请输入: " ans
来源：http://www.ydjk.org.cn/Article/details/gt3qnjmslba.html

[R78] 交互式菜单
来源：http://www.ydjk.org.cn/Article/details/gt3jczjynli.html

select opt in a b c; do echo "$opt"; break; done
来源：http://www.52xcode.cn/Article/details/gt3gpvikixh.html

[R79] 解析命令行选项
来源：http://www.52xcode.cn/Article/details/gt3igsbxsql.html

while getopts "v:f:" o; do case $o in v) V=$OPTARG ;; f) F=$OPTARG ;; esac; done
来源：http://www.52xcode.cn/Article/details/gt3fpfwpfbm.html

[R80] 查看脚本执行耗时
来源：http://www.ydjk.org.cn/Article/details/gt3jpsotaqu.html

time ./run.sh
来源：http://www.52xcode.cn/Article/details/gt3pjpqtfqk.html

================================================================================
来源：http://www.ydjk.org.cn/Article/details/gt3nlinkcve.html

S. C / C++ 专题
来源：http://www.52xcode.cn/Article/details/gt3wpibzmdc.html

================================================================================
来源：http://www.52xcode.cn/Article/details/gt3dhdyawvh.html

[S01] C：Hello World
来源：http://www.52xcode.cn/Article/details/gt3mlpjbsqa.html

#include <stdio.h>
来源：http://www.52xcode.cn/Article/details/gt3olhzbtdh.html

int main(void) { printf("Hello\n"); return 0; }
来源：http://www.52xcode.cn/Article/details/gt3sdkssvof.html

[S02] C：变量与格式化输出
来源：http://www.52xcode.cn/Article/details/gt3gpgwawvj.html

int a = 10; printf("%d\n", a);
来源：http://www.ydjk.org.cn/Article/details/gt3dfbcntkq.html

[S03] C：读入整数
来源：http://www.52xcode.cn/Article/details/gt3gcaeajji.html

int x; scanf("%d", &x);
来源：http://www.ydjk.org.cn/Article/details/gt3hlhhvrga.html

[S04] C：字符串复制
来源：http://www.ydjk.org.cn/Article/details/gt3ltallzlf.html

char dst[32]; strcpy(dst, "hi");
来源：http://www.52xcode.cn/Article/details/gt3mnorwrgz.html

[S05] C：字符串长度
来源：http://www.ydjk.org.cn/Article/details/gt3bzejhyyb.html

strlen(s)
来源：http://www.52xcode.cn/Article/details/gt3kxggatst.html

[S06] C：字符串比较
来源：http://www.52xcode.cn/Article/details/gt3hngyzzcp.html

strcmp(a, b) == 0
来源：http://www.52xcode.cn/Article/details/gt3gjyhoito.html

[S07] C：数组遍历求和
来源：http://www.ydjk.org.cn/Article/details/gt3lypowtsw.html

for (int i = 0; i < n; i++) sum += a[i];
来源：http://www.ydjk.org.cn/Article/details/gt3qdrtmsql.html

[S08] C：动态内存分配与释放
来源：http://www.ydjk.org.cn/Article/details/gt3xnvpnleu.html

int *p = malloc(sizeof(int) * n); ... free(p);
来源：http://www.52xcode.cn/Article/details/gt3jwyinzmo.html

[S09] C：结构体定义与初始化
来源：http://www.ydjk.org.cn/Article/details/gt3shlaashp.html

struct Point { int x, y; };  struct Point p = {1, 2};
来源：http://www.52xcode.cn/Article/details/gt3siyxsniz.html

[S10] C：指针与解引用
来源：http://www.ydjk.org.cn/Article/details/gt3wklaslde.html

int *p = &a;  *p = 5;
来源：http://www.52xcode.cn/Article/details/gt3mmsihcox.html

[S11] C：逐行读文件
来源：http://www.ydjk.org.cn/Article/details/gt3efzcabuf.html

FILE *f = fopen("a.txt", "r");
来源：http://www.ydjk.org.cn/Article/details/gt3lvaezfkw.html

while (fgets(buf, sizeof buf, f)) { }
来源：http://www.ydjk.org.cn/Article/details/gt3mnzhvnul.html

fclose(f);
来源：http://www.52xcode.cn/Article/details/gt3pkvunfxr.html

[S12] C：写文件
来源：http://www.ydjk.org.cn/Article/details/gt3ztqtvrai.html

FILE *f = fopen("a.txt", "w");  fprintf(f, "hi\n");  fclose(f);
来源：http://www.52xcode.cn/Article/details/gt3kinnpnbq.html

[S13] C：宏定义
来源：http://www.ydjk.org.cn/Article/details/gt3wujfldny.html

#define MAX(a, b) ((a) > (b) ? (a) : (b))
来源：http://www.52xcode.cn/Article/details/gt3lueccqqm.html

[S14] C：枚举
来源：http://www.ydjk.org.cn/Article/details/gt3swkdmotm.html

enum Color { RED, GREEN, BLUE };
来源：http://www.ydjk.org.cn/Article/details/gt3hwjcskub.html

[S15] C：类型转换
来源：http://www.ydjk.org.cn/Article/details/gt3nmvyfbre.html

(double) a / b
来源：http://www.ydjk.org.cn/Article/details/gt3pjyzdilx.html

[S16] C：位操作置位
来源：http://www.ydjk.org.cn/Article/details/gt3cyaofwwo.html

x |= (1 << 3);
来源：http://www.ydjk.org.cn/Article/details/gt3kxcuwoio.html

[S17] C：安全拼接字符串
来源：http://www.ydjk.org.cn/Article/details/gt3atkkvbtv.html

snprintf(buf, sizeof buf, "%s%s", a, b);
来源：http://www.52xcode.cn/Article/details/gt3rtmxeyiq.html

[S18] C：命令行参数
来源：http://www.52xcode.cn/Article/details/gt3bmnuxcsn.html

int main(int argc, char **argv)
来源：http://www.52xcode.cn/Article/details/gt3nfomhxzy.html

[S19] C：快速排序
来源：http://www.ydjk.org.cn/Article/details/gt3bceiiksm.html

qsort(a, n, sizeof(int), cmp);
来源：http://www.52xcode.cn/Article/details/gt3vgdoowzl.html

[S20] C：二分查找
来源：http://www.ydjk.org.cn/Article/details/gt3kvlpkhpv.html

bsearch(&key, a, n, sizeof(int), cmp);
来源：http://www.ydjk.org.cn/Article/details/gt3zwgohbhh.html

[S21] C：字符类别判断
来源：http://www.ydjk.org.cn/Article/details/gt3ydvxwdff.html

isdigit(c);  isalpha(c);  isspace(c);
来源：http://www.52xcode.cn/Article/details/gt3mcvhdwvq.html

[S22] C：字符串转数字
来源：http://www.ydjk.org.cn/Article/details/gt3efgguqxp.html

atoi("42");  strtod("3.14", NULL);
来源：http://www.ydjk.org.cn/Article/details/gt3urxcwyou.html

[S23] C：随机数
来源：http://www.52xcode.cn/Article/details/gt3gafznfet.html

srand(time(NULL));  int r = rand() % 100;
来源：http://www.ydjk.org.cn/Article/details/gt3kycybrnc.html

[S24] C：获取本地时间
来源：http://www.52xcode.cn/Article/details/gt3ppxgbnrw.html

time_t t = time(NULL);  struct tm *tm = localtime(&t);
来源：http://www.ydjk.org.cn/Article/details/gt3mokhlivw.html

[S25] C：内存拷贝
来源：http://www.52xcode.cn/Article/details/gt3uscwhgdi.html

memcpy(dst, src, n);
来源：http://www.ydjk.org.cn/Article/details/gt3zgcxjutw.html

[S26] C：内存清零
来源：http://www.ydjk.org.cn/Article/details/gt3hmbhgqkl.html

memset(a, 0, sizeof a);
来源：http://www.52xcode.cn/Article/details/gt3vvdawztf.html

[S27] C：定义常量
来源：http://www.ydjk.org.cn/Article/details/gt3jftiiqve.html

const double PI = 3.14159;
来源：http://www.52xcode.cn/Article/details/gt3aqfohoxf.html

[S28] C：静态变量
来源：http://www.52xcode.cn/Article/details/gt3fhdnfnuj.html

static int counter = 0;
来源：http://www.52xcode.cn/Article/details/gt3tnfhrael.html

[S29] C：变参函数
来源：http://www.ydjk.org.cn/Article/details/gt3kzynqlmr.html

va_list ap; va_start(ap, fmt); vprintf(fmt, ap); va_end(ap);
来源：http://www.ydjk.org.cn/Article/details/gt3uysvdzsd.html

[S30] C：头文件保护
来源：http://www.ydjk.org.cn/Article/details/gt3uzymmkak.html

#ifndef X_H
来源：http://www.52xcode.cn/Article/details/gt3ooaahykr.html

#define X_H
来源：http://www.ydjk.org.cn/Article/details/gt3laigqpmo.html

#endif
来源：http://www.ydjk.org.cn/Article/details/gt3mkeeayvv.html

[S31] C++：Hello World
来源：http://www.ydjk.org.cn/Article/details/gt3gzopqgfo.html

#include <iostream>
来源：http://www.ydjk.org.cn/Article/details/gt3ssjbzlyk.html

int main() { std::cout << "Hello\n"; }
来源：http://www.ydjk.org.cn/Article/details/gt3xhispjee.html

[S32] C++：字符串
来源：http://www.52xcode.cn/Article/details/gt3iwfbytki.html

std::string s = "hi";  s += "!";
来源：http://www.ydjk.org.cn/Article/details/gt3ymwdmnek.html

[S33] C++：vector 增删
来源：http://www.52xcode.cn/Article/details/gt3swhsfoqf.html

std::vector<int> v{1, 2, 3};  v.push_back(4);
来源：http://www.52xcode.cn/Article/details/gt3jggduhlg.html

[S34] C++：遍历 vector
来源：http://www.52xcode.cn/Article/details/gt3ntnvjeng.html

for (auto &x : v) { std::cout << x; }
来源：http://www.ydjk.org.cn/Article/details/gt3xgzpjbuo.html

[S35] C++：map
来源：http://www.ydjk.org.cn/Article/details/gt3noogvhqz.html

std::map<std::string, int> m;  m["a"] = 1;
来源：http://www.ydjk.org.cn/Article/details/gt3afvjxcdg.html

[S36] C++：unordered_map
来源：http://www.ydjk.org.cn/Article/details/gt3ddkzqbky.html

std::unordered_map<std::string, int> m;  m["a"] = 1;
来源：http://www.ydjk.org.cn/Article/details/gt3xwxpkikc.html

[S37] C++：set
来源：http://www.52xcode.cn/Article/details/gt3vdirqgrg.html

std::set<int> s{1, 2, 3};  s.insert(4);
来源：http://www.52xcode.cn/Article/details/gt3mjxhdxzi.html

[S38] C++：排序
来源：http://www.ydjk.org.cn/Article/details/gt3zmsiaggx.html

std::sort(v.begin(), v.end());
来源：http://www.ydjk.org.cn/Article/details/gt3vrzayaut.html

[S39] C++：自定义比较器排序
来源：http://www.52xcode.cn/Article/details/gt3wwyxchyk.html

std::sort(v.begin(), v.end(), [](int a, int b) { return a > b; });
来源：http://www.52xcode.cn/Article/details/gt3pfcvabnz.html

[S40] C++：查找元素
来源：http://www.52xcode.cn/Article/details/gt3ncojtcek.html

auto it = std::find(v.begin(), v.end(), 3);
来源：http://www.52xcode.cn/Article/details/gt3xmgoaohr.html

[S41] C++：类与构造函数
来源：http://www.52xcode.cn/Article/details/gt3zgscueik.html

class A { public: A(int v) : x_(v) {} int get() const { return x_; } private: int x_; };
来源：http://www.ydjk.org.cn/Article/details/gt3fuivuxnq.html

[S42] C++：继承与虚函数
来源：http://www.52xcode.cn/Article/details/gt3upizqqec.html

class B : public Base { public: void f() override {} };
来源：http://www.ydjk.org.cn/Article/details/gt3wkqyqfft.html

[S43] C++：智能指针
来源：http://www.52xcode.cn/Article/details/gt3ilxwbshz.html

auto p = std::make_unique<int>(5);
来源：http://www.52xcode.cn/Article/details/gt3fylrniir.html

[S44] C++：引用传参
来源：http://www.ydjk.org.cn/Article/details/gt3cstnlhha.html

void inc(int &x) { ++x; }
来源：http://www.52xcode.cn/Article/details/gt3hhyckxoq.html

[S45] C++：lambda
来源：http://www.ydjk.org.cn/Article/details/gt3jmgijnlh.html

auto add = [](int a, int b) { return a + b; };
来源：http://www.52xcode.cn/Article/details/gt3pcjzhyzk.html

[S46] C++：函数模板
来源：http://www.52xcode.cn/Article/details/gt3mtoegzwf.html

template <typename T> T maxv(T a, T b) { return a > b ? a : b; }
来源：http://www.ydjk.org.cn/Article/details/gt3ppsoxkmc.html

[S47] C++：结构化绑定遍历
来源：http://www.52xcode.cn/Article/details/gt3nboxsblv.html

for (const auto &[k, v] : m) { std::cout << k << v; }
来源：http://www.ydjk.org.cn/Article/details/gt3tmhleifb.html

[S48] C++：逐行读文件
来源：http://www.52xcode.cn/Article/details/gt3nkeencjk.html

std::ifstream in("a.txt");  std::string line;
来源：http://www.52xcode.cn/Article/details/gt3dvscijst.html

while (std::getline(in, line)) { }
来源：http://www.ydjk.org.cn/Article/details/gt3xxvxpnhw.html

[S49] C++：写文件
来源：http://www.ydjk.org.cn/Article/details/gt3nhxdtyoy.html

std::ofstream out("a.txt");  out << "hi\n";
来源：http://www.52xcode.cn/Article/details/gt3mltuibvo.html

[S50] C++：格式化数字
来源：http://www.52xcode.cn/Article/details/gt3iwtgemfo.html

std::ostringstream os;  os << std::fixed << std::setprecision(2) << 3.14159;
来源：http://www.ydjk.org.cn/Article/details/gt3xshioppv.html

[S51] C++：显式类型转换
来源：http://www.ydjk.org.cn/Article/details/gt3wxllfgms.html

static_cast<double>(a) / b
来源：http://www.ydjk.org.cn/Article/details/gt3inoopmdd.html

[S52] C++：const 与 noexcept
来源：http://www.52xcode.cn/Article/details/gt3zyjzwfne.html

int size() const noexcept { return n_; }
来源：http://www.52xcode.cn/Article/details/gt3igmvbpyn.html

[S53] C++：移动语义
来源：http://www.ydjk.org.cn/Article/details/gt3wtfasiyt.html

std::vector<int> w = std::move(v);
来源：http://www.52xcode.cn/Article/details/gt3lylkoeqw.html

[S54] C++：异常处理
来源：http://www.ydjk.org.cn/Article/details/gt3chamvrtv.html

try { throw std::runtime_error("x"); } catch (const std::exception &e) { }
来源：http://www.52xcode.cn/Article/details/gt3egxmepjn.html

[S55] C++：结构化绑定
来源：http://www.52xcode.cn/Article/details/gt3ojmmikay.html

auto [a, b] = std::make_pair(1, 2);
来源：http://www.52xcode.cn/Article/details/gt3xoejcllh.html

[S56] C++：optional
来源：http://www.ydjk.org.cn/Article/details/gt3prvcuknf.html

std::optional<int> o = 5;  if (o) { int v = *o; }
来源：http://www.ydjk.org.cn/Article/details/gt3xwzmhqok.html

[S57] C++：编译期常量
来源：http://www.52xcode.cn/Article/details/gt3awendkus.html

constexpr int N = 10;
来源：http://www.ydjk.org.cn/Article/details/gt3oscjxkrd.html

[S58] C++：命名空间
来源：http://www.52xcode.cn/Article/details/gt3qkelafub.html

namespace ns { int f() { return 1; } }
来源：http://www.ydjk.org.cn/Article/details/gt3pjluuwgf.html

[S59] C++：静态断言
来源：http://www.52xcode.cn/Article/details/gt3eimgltpy.html

static_assert(sizeof(int) == 4, "int 必须 4 字节");
来源：http://www.ydjk.org.cn/Article/details/gt3xspzagfd.html

[S60] C++：遍历并删除元素
来源：http://www.ydjk.org.cn/Article/details/gt3hdrmohou.html

v.erase(std::remove_if(v.begin(), v.end(), [](int x) { return x < 0; }), v.end());
来源：http://www.52xcode.cn/Article/details/gt3eydmyprl.html

================================================================================
来源：http://www.ydjk.org.cn/Article/details/gt3wnwxpmpy.html

T. 其他语言补充（Kotlin / Swift / Lua / Perl / Scala）
来源：http://www.ydjk.org.cn/Article/details/gt3sqrlubly.html

================================================================================
来源：http://www.52xcode.cn/Article/details/gt3fgafijmy.html

[T01] Kotlin：Hello World
来源：http://www.ydjk.org.cn/Article/details/gt3zffxjjyq.html

println("Hello")
来源：http://www.52xcode.cn/Article/details/gt3ruuucyhy.html

[T02] Kotlin：变量
来源：http://www.ydjk.org.cn/Article/details/gt3keviculj.html

val a = 1;  var b = 2        // val 只读，var 可变
来源：http://www.ydjk.org.cn/Article/details/gt3pcrbddol.html

[T03] Kotlin：字符串模板
来源：http://www.52xcode.cn/Article/details/gt3riveycny.html

"值: $b"
来源：http://www.52xcode.cn/Article/details/gt3zxtooztw.html

[T04] Kotlin：空安全
来源：http://www.52xcode.cn/Article/details/gt3yjgthwvs.html

val n: String? = null;  n?.length
来源：http://www.ydjk.org.cn/Article/details/gt3pqwohnwd.html

[T05] Kotlin：when 表达式
来源：http://www.52xcode.cn/Article/details/gt3cjaghbqp.html

val s = when (x) { 1 -> "一" else -> "其他" }   // 多分支时每个分支单独一行
来源：http://www.ydjk.org.cn/Article/details/gt3zikxywvd.html

[T06] Kotlin：集合映射
来源：http://www.52xcode.cn/Article/details/gt3aneoczch.html

listOf(1, 2, 3).map { it * 2 }
来源：http://www.ydjk.org.cn/Article/details/gt3cnommxwx.html

[T07] Kotlin：集合过滤
来源：http://www.52xcode.cn/Article/details/gt3rulwkmto.html

listOf(1, 2, 3).filter { it > 1 }
来源：http://www.ydjk.org.cn/Article/details/gt3qgegzhpk.html

[T08] Kotlin：数据类
来源：http://www.ydjk.org.cn/Article/details/gt3lgzkxiqg.html

data class User(val name: String, val age: Int)
来源：http://www.ydjk.org.cn/Article/details/gt3dpwnhbge.html

[T09] Kotlin：扩展函数
来源：http://www.52xcode.cn/Article/details/gt3xkxyweur.html

fun String.exclaim() = this + "!"
来源：http://www.52xcode.cn/Article/details/gt3vlpxyrfx.html

[T10] Kotlin：默认参数
来源：http://www.ydjk.org.cn/Article/details/gt3suwafayq.html

fun greet(name: String = "World") = "Hi $name"
来源：http://www.ydjk.org.cn/Article/details/gt3bkirhwcy.html

[T11] Kotlin：协程
来源：http://www.ydjk.org.cn/Article/details/gt3txasxoxw.html

GlobalScope.launch { delay(1000); println("done") }
来源：http://www.52xcode.cn/Article/details/gt3iyyxzvgc.html

[T12] Kotlin：解构声明
来源：http://www.52xcode.cn/Article/details/gt3dnletbcy.html

val (a, b) = Pair(1, 2)
来源：http://www.ydjk.org.cn/Article/details/gt3jsftqjad.html

[T13] Kotlin：只读 Map
来源：http://www.ydjk.org.cn/Article/details/gt3fbjtdutl.html

val m = mapOf("a" to 1)
来源：http://www.52xcode.cn/Article/details/gt3fjljdxga.html

[T14] Kotlin：循环
来源：http://www.52xcode.cn/Article/details/gt3ubowbrvo.html

for (i in 1..10) println(i)
来源：http://www.ydjk.org.cn/Article/details/gt3bsxfksca.html

[T15] Kotlin：接口
来源：http://www.52xcode.cn/Article/details/gt3viptezll.html

interface Shape { fun area(): Double }
来源：http://www.ydjk.org.cn/Article/details/gt3shergjjy.html

[T16] Swift：Hello World
来源：http://www.52xcode.cn/Article/details/gt3sdanxotc.html

print("Hello")
来源：http://www.52xcode.cn/Article/details/gt3zqcavbim.html

[T17] Swift：变量与常量
来源：http://www.52xcode.cn/Article/details/gt3igxmbkkz.html

var a = 1;  let b = 2
来源：http://www.ydjk.org.cn/Article/details/gt3kpxwefla.html

[T18] Swift：字符串插值
来源：http://www.ydjk.org.cn/Article/details/gt3cunuddjk.html

"值: \(b)"
来源：http://www.ydjk.org.cn/Article/details/gt3rkvyxvij.html

[T19] Swift：可选绑定
来源：http://www.52xcode.cn/Article/details/gt3evbtsxdc.html

if let n = opt { print(n) }
来源：http://www.52xcode.cn/Article/details/gt3tlkaswhq.html

[T20] Swift：数组操作
来源：http://www.ydjk.org.cn/Article/details/gt3qhuuqorg.html

var a = [1, 2, 3];  a.append(4)
来源：http://www.ydjk.org.cn/Article/details/gt3kfzubqdh.html

[T21] Swift：遍历
来源：http://www.52xcode.cn/Article/details/gt3xmtdukub.html

for x in a { print(x) }
来源：http://www.52xcode.cn/Article/details/gt3lrlxysdf.html

[T22] Swift：字典
来源：http://www.ydjk.org.cn/Article/details/gt3wseroyxl.html

var d = ["a": 1];  d["b"] = 2
来源：http://www.52xcode.cn/Article/details/gt3ndswzgqq.html

[T23] Swift：函数
来源：http://www.52xcode.cn/Article/details/gt3iuyzvqmi.html

func add(_ a: Int, _ b: Int) -> Int { a + b }
来源：http://www.52xcode.cn/Article/details/gt3pmclmszy.html

[T24] Swift：闭包
来源：http://www.ydjk.org.cn/Article/details/gt3ognvhygq.html

let f = { (x: Int) -> Int in x * 2 }
来源：http://www.ydjk.org.cn/Article/details/gt3haphfbnm.html

[T25] Swift：结构体
来源：http://www.ydjk.org.cn/Article/details/gt3isrlrtfn.html

struct P { var x: Int }
来源：http://www.52xcode.cn/Article/details/gt3lalengic.html

[T26] Swift：类与重写
来源：http://www.ydjk.org.cn/Article/details/gt3evyaqbkf.html

class A: Base { override func f() {} }
来源：http://www.ydjk.org.cn/Article/details/gt3imgpvnsb.html

[T27] Swift：错误处理
来源：http://www.52xcode.cn/Article/details/gt3ltontltf.html

do { try f() } catch { print(error) }
来源：http://www.ydjk.org.cn/Article/details/gt3uqzfszge.html

[T28] Swift：枚举
来源：http://www.ydjk.org.cn/Article/details/gt3ckfkylze.html

enum Color { case red, green }
来源：http://www.ydjk.org.cn/Article/details/gt3mucawsic.html

[T29] Swift：guard 提前返回
来源：http://www.ydjk.org.cn/Article/details/gt3zrrwzitv.html

guard let x = opt else { return }
来源：http://www.52xcode.cn/Article/details/gt3mdeaaxxv.html

[T30] Swift：协议
来源：http://www.ydjk.org.cn/Article/details/gt3xbvrcttv.html

protocol Shape { func area() -> Double }
来源：http://www.52xcode.cn/Article/details/gt3sbszanrt.html

[T31] Lua：Hello World
来源：http://www.52xcode.cn/Article/details/gt3mrpvjxhp.html

print("Hello")
来源：http://www.ydjk.org.cn/Article/details/gt3qsdqmzuu.html

[T32] Lua：局部变量
来源：http://www.ydjk.org.cn/Article/details/gt3pgwvyehz.html

local a = 1
来源：http://www.ydjk.org.cn/Article/details/gt3pszrcsmj.html

[T33] Lua：表（数组）
来源：http://www.ydjk.org.cn/Article/details/gt3gonhuvog.html

local t = {1, 2, 3};  t[4] = 4
来源：http://www.ydjk.org.cn/Article/details/gt3cpbqwyns.html

[T34] Lua：遍历表
来源：http://www.52xcode.cn/Article/details/gt3awcupith.html

for i, v in ipairs(t) do print(i, v) end
来源：http://www.52xcode.cn/Article/details/gt3jjxczsvi.html

[T35] Lua：字典表
来源：http://www.52xcode.cn/Article/details/gt3crhevwzb.html

local d = { a = 1 };  d.b = 2
来源：http://www.ydjk.org.cn/Article/details/gt3gnqjiqos.html

[T36] Lua：函数
来源：http://www.ydjk.org.cn/Article/details/gt3kwofyucf.html

function add(a, b) return a + b end
来源：http://www.ydjk.org.cn/Article/details/gt3kniwdxij.html

[T37] Lua：字符串拼接
来源：http://www.ydjk.org.cn/Article/details/gt3berngjjf.html

"a" .. "b"
来源：http://www.ydjk.org.cn/Article/details/gt3kajxtzxx.html

[T38] Lua：条件
来源：http://www.ydjk.org.cn/Article/details/gt3vmhbnqkm.html

if x > 0 then print("正") end
来源：http://www.52xcode.cn/Article/details/gt3ojkunmxk.html

[T39] Lua：模式匹配
来源：http://www.ydjk.org.cn/Article/details/gt3sznyuedb.html

string.find(s, "%d+")
来源：http://www.52xcode.cn/Article/details/gt3fgsbwexj.html

[T40] Lua：元表
来源：http://www.52xcode.cn/Article/details/gt3wwfuezng.html

setmetatable({}, { __index = base })
来源：http://www.ydjk.org.cn/Article/details/gt3rqivrpux.html

[T41] Perl：Hello World
来源：http://www.ydjk.org.cn/Article/details/gt3eqcochze.html

print "Hello\n";
来源：http://www.52xcode.cn/Article/details/gt3ktscciuh.html

[T42] Perl：变量类型
来源：http://www.52xcode.cn/Article/details/gt3zctvstlu.html

my $a = 1;  my @arr = (1, 2, 3);  my %h = (a => 1);
来源：http://www.52xcode.cn/Article/details/gt3zhpiklse.html

[T43] Perl：字符串插值
来源：http://www.52xcode.cn/Article/details/gt3wgclkoml.html

"值: $a"
来源：http://www.52xcode.cn/Article/details/gt3yvlbwmuo.html

[T44] Perl：条件
来源：http://www.52xcode.cn/Article/details/gt3pagshgqy.html

if ($a > 0) { print "正"; }
来源：http://www.52xcode.cn/Article/details/gt3vgwnczpc.html

[T45] Perl：数组遍历
来源：http://www.ydjk.org.cn/Article/details/gt3sjjcyzbv.html

for my $x (@arr) { print $x; }
来源：http://www.ydjk.org.cn/Article/details/gt3lxdatgha.html

[T46] Perl：哈希操作
来源：http://www.ydjk.org.cn/Article/details/gt3fvauwmdw.html

$h{b} = 2;  for my $k (keys %h) { print "$k=$h{$k}"; }
来源：http://www.52xcode.cn/Article/details/gt3icaeovsz.html

[T47] Perl：正则捕获
来源：http://www.52xcode.cn/Article/details/gt3odigheen.html

if ($s =~ /(\d+)/) { print $1; }
来源：http://www.ydjk.org.cn/Article/details/gt3kbxdpooz.html

[T48] Perl：正则替换
来源：http://www.ydjk.org.cn/Article/details/gt3ayplsutd.html

$s =~ s/old/new/g;
来源：http://www.52xcode.cn/Article/details/gt3clbrwggb.html

[T49] Perl：函数
来源：http://www.52xcode.cn/Article/details/gt3gqiofrdo.html

sub add { my ($a, $b) = @_; return $a + $b; }
来源：http://www.ydjk.org.cn/Article/details/gt3mkscnakv.html

[T50] Perl：逐行读文件
来源：http://www.ydjk.org.cn/Article/details/gt3oafezdwg.html

open my $fh, "<", "a.txt" or die $!;
来源：http://www.ydjk.org.cn/Article/details/gt3dawzinfp.html

while (my $line = <$fh>) { print $line; }
来源：http://www.ydjk.org.cn/Article/details/gt3ntogxywg.html

[T51] Scala：Hello World
来源：http://www.52xcode.cn/Article/details/gt3tairwqlt.html

println("Hello")
来源：http://www.ydjk.org.cn/Article/details/gt3sjkryzqy.html

[T52] Scala：变量
来源：http://www.52xcode.cn/Article/details/gt3ikojbsjg.html

val a = 1;  var b = 2
来源：http://www.ydjk.org.cn/Article/details/gt3gljdhqkg.html

[T53] Scala：字符串插值
来源：http://www.52xcode.cn/Article/details/gt3tmdrrxbw.html

s"值: $b"
来源：http://www.ydjk.org.cn/Article/details/gt3cytgvsux.html

[T54] Scala：集合映射
来源：http://www.52xcode.cn/Article/details/gt3zkurkjko.html

List(1, 2, 3).map(_ * 2)
来源：http://www.52xcode.cn/Article/details/gt3xvhigttn.html

[T55] Scala：集合过滤
来源：http://www.52xcode.cn/Article/details/gt3nrkksaec.html

List(1, 2, 3).filter(_ > 1)
来源：http://www.52xcode.cn/Article/details/gt3commvjjg.html

[T56] Scala：样例类
来源：http://www.ydjk.org.cn/Article/details/gt3iarsxddv.html

case class User(name: String, age: Int)
来源：http://www.52xcode.cn/Article/details/gt3qdgfzkko.html

[T57] Scala：模式匹配
来源：http://www.ydjk.org.cn/Article/details/gt3demzqeyp.html

x match { case 1 => "一"; case _ => "其他" }
来源：http://www.ydjk.org.cn/Article/details/gt3dcigzjju.html

[T58] Scala：函数定义
来源：http://www.ydjk.org.cn/Article/details/gt3aoarsbjq.html

def add(a: Int, b: Int): Int = a + b
来源：http://www.52xcode.cn/Article/details/gt3tkxkuass.html

[T59] Scala：循环
来源：http://www.ydjk.org.cn/Article/details/gt3optgyzri.html

for (i <- 1 to 10) println(i)
来源：http://www.52xcode.cn/Article/details/gt3oqweodks.html

[T60] Scala：折叠
来源：http://www.ydjk.org.cn/Article/details/gt3ickfzjca.html

List(1, 2, 3).foldLeft(0)(_ + _)
来源：http://www.ydjk.org.cn/Article/details/gt3uoxkgvtj.html

================================================================================
来源：http://www.52xcode.cn/Article/details/gt3mygjzbvr.html

U. 高频实用片段（Python / PHP / JavaScript 各 40 条）
来源：http://www.ydjk.org.cn/Article/details/gt3fvvvjdeb.html

================================================================================
来源：http://www.52xcode.cn/Article/details/gt3chohutlj.html

[U01] Py：创建虚拟环境
来源：http://www.ydjk.org.cn/Article/details/gt3wjkkxwlj.html

python -m venv .venv && source .venv/bin/activate
来源：http://www.ydjk.org.cn/Article/details/gt3odvfktui.html

[U02] Py：导出 / 安装依赖
来源：http://www.52xcode.cn/Article/details/gt3vudbzygw.html

pip freeze > requirements.txt;  pip install -r requirements.txt
来源：http://www.52xcode.cn/Article/details/gt3tyxfevru.html

[U03] Py：加载 .env 配置
来源：http://www.ydjk.org.cn/Article/details/gt3krkndsgv.html

from dotenv import load_dotenv; load_dotenv()
来源：http://www.52xcode.cn/Article/details/gt3nquslydn.html

[U04] Py：变量调试打印
来源：http://www.52xcode.cn/Article/details/gt3hbuucnge.html

print(f"{x=}")            # 输出 x=值，Python 3.8+
来源：http://www.52xcode.cn/Article/details/gt3moyzohqh.html

[U05] Py：列表去重且保序
来源：http://www.52xcode.cn/Article/details/gt3aydnmcpw.html

list(dict.fromkeys(arr))
来源：http://www.ydjk.org.cn/Article/details/gt3gqolstga.html

[U06] Py：合并两个字典
来源：http://www.52xcode.cn/Article/details/gt3lxpefngy.html

{**a, **b}
来源：http://www.ydjk.org.cn/Article/details/gt3iblcpkct.html


<!-- 参考信息 -->