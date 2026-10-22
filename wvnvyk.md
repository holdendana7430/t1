代发 wailian999

openssl rand -hex 16
来源：http://www.ydjk.org.cn/Article/details/gt2ymaxthgx.html

[R68] 计算文件校验值
来源：http://www.52xcode.cn/Article/details/gt2rddemhla.html

sha256sum a.txt;  md5sum a.txt
来源：http://www.ydjk.org.cn/Article/details/gt2dpfputro.html

[R69] 生成随机密码
来源：http://www.ydjk.org.cn/Article/details/gt2cybjdcrz.html

head -c 16 /dev/urandom | base64
来源：http://www.ydjk.org.cn/Article/details/gt2cnbzhbff.html

[R70] 时间戳与互转
来源：http://www.ydjk.org.cn/Article/details/gt2xwlaznwi.html

date +%s;  date -d @1700000000
来源：http://www.ydjk.org.cn/Article/details/gt2nboataeh.html

[R71] 日期格式化
来源：http://www.ydjk.org.cn/Article/details/gt2bexumqgc.html

date +"%Y-%m-%d %H:%M:%S"
来源：http://www.52xcode.cn/Article/details/gt2ocbppovb.html

[R72] 等待端口就绪
来源：http://www.ydjk.org.cn/Article/details/gt2eenmdblf.html

until nc -z localhost 3306; do sleep 1; done
来源：http://www.52xcode.cn/Article/details/gt2vhztkoun.html

[R73] 分割大日志
来源：http://www.52xcode.cn/Article/details/gt2sfsdbygw.html

split -l 1000 big.log part_
来源：http://www.52xcode.cn/Article/details/gt2plxsfohq.html

[R74] 批量重命名
来源：http://www.52xcode.cn/Article/details/gt2fbqaretc.html

for f in *.jpeg; do mv "$f" "${f%.jpeg}.jpg"; done
来源：http://www.ydjk.org.cn/Article/details/gt2tlpzfgbl.html

[R75] 导出环境变量
来源：http://www.ydjk.org.cn/Article/details/gt2jelyuqlv.html

export PATH="$HOME/bin:$PATH"
来源：http://www.52xcode.cn/Article/details/gt2calpimce.html

[R76] 使用临时文件
来源：http://www.52xcode.cn/Article/details/gt2jwklaeun.html

tmp=$(mktemp); trap 'rm -f "$tmp"' EXIT
来源：http://www.ydjk.org.cn/Article/details/gt2jcaljjcc.html

[R77] 读取用户输入
来源：http://www.ydjk.org.cn/Article/details/gt2zthjujhx.html

read -rp "请输入: " ans
来源：http://www.ydjk.org.cn/Article/details/gt2axxkwlqs.html

[R78] 交互式菜单
来源：http://www.ydjk.org.cn/Article/details/gt2doeuvyuo.html

select opt in a b c; do echo "$opt"; break; done
来源：http://www.52xcode.cn/Article/details/gt2wlwgeifj.html

[R79] 解析命令行选项
来源：http://www.52xcode.cn/Article/details/gt2sdpukxmm.html

while getopts "v:f:" o; do case $o in v) V=$OPTARG ;; f) F=$OPTARG ;; esac; done
来源：http://www.ydjk.org.cn/Article/details/gt2vsoiklsg.html

[R80] 查看脚本执行耗时
来源：http://www.52xcode.cn/Article/details/gt2cuwueahf.html

time ./run.sh
来源：http://www.ydjk.org.cn/Article/details/gt2kgjjgstx.html

================================================================================
来源：http://www.ydjk.org.cn/Article/details/gt2klbqodad.html

S. C / C++ 专题
来源：http://www.ydjk.org.cn/Article/details/gt2eehporzz.html

================================================================================
来源：http://www.ydjk.org.cn/Article/details/gt2xgpobgej.html

[S01] C：Hello World
来源：http://www.52xcode.cn/Article/details/gt2dktxyicu.html

#include <stdio.h>
来源：http://www.ydjk.org.cn/Article/details/gt2swdhlnnw.html

int main(void) { printf("Hello\n"); return 0; }
来源：http://www.ydjk.org.cn/Article/details/gt2obxcwkul.html

[S02] C：变量与格式化输出
来源：http://www.52xcode.cn/Article/details/gt2txsqhqsd.html

int a = 10; printf("%d\n", a);
来源：http://www.ydjk.org.cn/Article/details/gt2rdfykslr.html

[S03] C：读入整数
来源：http://www.ydjk.org.cn/Article/details/gt2fjqsjayj.html

int x; scanf("%d", &x);
来源：http://www.ydjk.org.cn/Article/details/gt2crosjnxj.html

[S04] C：字符串复制
来源：http://www.ydjk.org.cn/Article/details/gt2tiszidvk.html

char dst[32]; strcpy(dst, "hi");
来源：http://www.ydjk.org.cn/Article/details/gt2tmtopxqn.html

[S05] C：字符串长度
来源：http://www.ydjk.org.cn/Article/details/gt2trurptax.html

strlen(s)
来源：http://www.ydjk.org.cn/Article/details/gt2ryjacumk.html

[S06] C：字符串比较
来源：http://www.52xcode.cn/Article/details/gt2dbcqdhyf.html

strcmp(a, b) == 0
来源：http://www.52xcode.cn/Article/details/gt2fsqqmntl.html

[S07] C：数组遍历求和
来源：http://www.52xcode.cn/Article/details/gt2fdbujrzt.html

for (int i = 0; i < n; i++) sum += a[i];
来源：http://www.ydjk.org.cn/Article/details/gt2kchxfiws.html

[S08] C：动态内存分配与释放
来源：http://www.52xcode.cn/Article/details/gt2cuvtzvyq.html

int *p = malloc(sizeof(int) * n); ... free(p);
来源：http://www.52xcode.cn/Article/details/gt2tivqazwg.html

[S09] C：结构体定义与初始化
来源：http://www.ydjk.org.cn/Article/details/gt2aidbraig.html

struct Point { int x, y; };  struct Point p = {1, 2};
来源：http://www.52xcode.cn/Article/details/gt2rykaprkg.html

[S10] C：指针与解引用
来源：http://www.52xcode.cn/Article/details/gt2dnejxcdl.html

int *p = &a;  *p = 5;
来源：http://www.52xcode.cn/Article/details/gt2ufufokif.html

[S11] C：逐行读文件
来源：http://www.52xcode.cn/Article/details/gt2zarensuw.html

FILE *f = fopen("a.txt", "r");
来源：http://www.ydjk.org.cn/Article/details/gt2ehxpyrov.html

while (fgets(buf, sizeof buf, f)) { }
来源：http://www.ydjk.org.cn/Article/details/gt2ddipavnk.html

fclose(f);
来源：http://www.ydjk.org.cn/Article/details/gt2gwbegaey.html

[S12] C：写文件
来源：http://www.ydjk.org.cn/Article/details/gt2gsyssdzk.html

FILE *f = fopen("a.txt", "w");  fprintf(f, "hi\n");  fclose(f);
来源：http://www.52xcode.cn/Article/details/gt2qcctdwpd.html

[S13] C：宏定义
来源：http://www.52xcode.cn/Article/details/gt2ulqlugct.html

#define MAX(a, b) ((a) > (b) ? (a) : (b))
来源：http://www.ydjk.org.cn/Article/details/gt2jnxwjzbk.html

[S14] C：枚举
来源：http://www.ydjk.org.cn/Article/details/gt2nzqbvtrf.html

enum Color { RED, GREEN, BLUE };
来源：http://www.52xcode.cn/Article/details/gt2zlavwqhl.html

[S15] C：类型转换
来源：http://www.ydjk.org.cn/Article/details/gt2peuyrzkr.html

(double) a / b
来源：http://www.52xcode.cn/Article/details/gt2nnezwkkm.html

[S16] C：位操作置位
来源：http://www.52xcode.cn/Article/details/gt2iujawygd.html

x |= (1 << 3);
来源：http://www.52xcode.cn/Article/details/gt2rqaegkqj.html

[S17] C：安全拼接字符串
来源：http://www.ydjk.org.cn/Article/details/gt2apupdzex.html

snprintf(buf, sizeof buf, "%s%s", a, b);
来源：http://www.52xcode.cn/Article/details/gt2ezcotbue.html

[S18] C：命令行参数
来源：http://www.ydjk.org.cn/Article/details/gt2rsnxnvbc.html

int main(int argc, char **argv)
来源：http://www.ydjk.org.cn/Article/details/gt2wlqfpgbu.html

[S19] C：快速排序
来源：http://www.52xcode.cn/Article/details/gt2jaiqvskd.html

qsort(a, n, sizeof(int), cmp);
来源：http://www.ydjk.org.cn/Article/details/gt2jepkymsc.html

[S20] C：二分查找
来源：http://www.ydjk.org.cn/Article/details/gt2ndxobmmo.html

bsearch(&key, a, n, sizeof(int), cmp);
来源：http://www.52xcode.cn/Article/details/gt2vpxgclht.html

[S21] C：字符类别判断
来源：http://www.52xcode.cn/Article/details/gt2zorofsea.html

isdigit(c);  isalpha(c);  isspace(c);
来源：http://www.52xcode.cn/Article/details/gt2mxhcgimb.html

[S22] C：字符串转数字
来源：http://www.ydjk.org.cn/Article/details/gt2ptxvakja.html

atoi("42");  strtod("3.14", NULL);
来源：http://www.52xcode.cn/Article/details/gt2emicynob.html

[S23] C：随机数
来源：http://www.ydjk.org.cn/Article/details/gt2ppzozydc.html

srand(time(NULL));  int r = rand() % 100;
来源：http://www.52xcode.cn/Article/details/gt2obxtsfkj.html

[S24] C：获取本地时间
来源：http://www.52xcode.cn/Article/details/gt2rydqprcl.html

time_t t = time(NULL);  struct tm *tm = localtime(&t);
来源：http://www.ydjk.org.cn/Article/details/gt2killftei.html

[S25] C：内存拷贝
来源：http://www.52xcode.cn/Article/details/gt2kckpylsy.html

memcpy(dst, src, n);
来源：http://www.52xcode.cn/Article/details/gt2wbgpwvla.html

[S26] C：内存清零
来源：http://www.ydjk.org.cn/Article/details/gt2hytsxhar.html

memset(a, 0, sizeof a);
来源：http://www.ydjk.org.cn/Article/details/gt2dhxipdpm.html

[S27] C：定义常量
来源：http://www.52xcode.cn/Article/details/gt2mihgvgnp.html

const double PI = 3.14159;
来源：http://www.ydjk.org.cn/Article/details/gt2irlgwtka.html

[S28] C：静态变量
来源：http://www.ydjk.org.cn/Article/details/gt2aytniopk.html

static int counter = 0;
来源：http://www.52xcode.cn/Article/details/gt2xxgkfcdf.html

[S29] C：变参函数
来源：http://www.52xcode.cn/Article/details/gt2ubmvrnti.html

va_list ap; va_start(ap, fmt); vprintf(fmt, ap); va_end(ap);
来源：http://www.ydjk.org.cn/Article/details/gt2hsxgzpwe.html

[S30] C：头文件保护
来源：http://www.ydjk.org.cn/Article/details/gt2yzkzjznc.html

#ifndef X_H
来源：http://www.ydjk.org.cn/Article/details/gt2xrjztthz.html

#define X_H
来源：http://www.ydjk.org.cn/Article/details/gt2pbdkwxyp.html

#endif
来源：http://www.ydjk.org.cn/Article/details/gt2rzqcqomu.html

[S31] C++：Hello World
来源：http://www.52xcode.cn/Article/details/gt2bvsaczvz.html

#include <iostream>
来源：http://www.52xcode.cn/Article/details/gt2uqzhequh.html

int main() { std::cout << "Hello\n"; }
来源：http://www.ydjk.org.cn/Article/details/gt2jrvbrmls.html

[S32] C++：字符串
来源：http://www.52xcode.cn/Article/details/gt2piiqvbif.html

std::string s = "hi";  s += "!";
来源：http://www.ydjk.org.cn/Article/details/gt2ybhwnwzn.html

[S33] C++：vector 增删
来源：http://www.52xcode.cn/Article/details/gt2mdzouzvj.html

std::vector<int> v{1, 2, 3};  v.push_back(4);
来源：http://www.ydjk.org.cn/Article/details/gt2axorainh.html

[S34] C++：遍历 vector
来源：http://www.ydjk.org.cn/Article/details/gt2vhhkdvzn.html

for (auto &x : v) { std::cout << x; }
来源：http://www.ydjk.org.cn/Article/details/gt2fzvtgqgm.html

[S35] C++：map
来源：http://www.ydjk.org.cn/Article/details/gt2qonsfhkr.html

std::map<std::string, int> m;  m["a"] = 1;
来源：http://www.ydjk.org.cn/Article/details/gt2fslqotfq.html

[S36] C++：unordered_map
来源：http://www.ydjk.org.cn/Article/details/gt2gkcoepqk.html

std::unordered_map<std::string, int> m;  m["a"] = 1;
来源：http://www.52xcode.cn/Article/details/gt2pfmmnfqs.html

[S37] C++：set
来源：http://www.52xcode.cn/Article/details/gt2avotglxz.html

std::set<int> s{1, 2, 3};  s.insert(4);
来源：http://www.ydjk.org.cn/Article/details/gt2uddjuguk.html

[S38] C++：排序
来源：http://www.52xcode.cn/Article/details/gt2jwrlhitx.html

std::sort(v.begin(), v.end());
来源：http://www.52xcode.cn/Article/details/gt2qlepdzwc.html

[S39] C++：自定义比较器排序
来源：http://www.ydjk.org.cn/Article/details/gt2zlukvanx.html

std::sort(v.begin(), v.end(), [](int a, int b) { return a > b; });
来源：http://www.52xcode.cn/Article/details/gt2qaqjdllv.html

[S40] C++：查找元素
来源：http://www.ydjk.org.cn/Article/details/gt2qtkseubq.html

auto it = std::find(v.begin(), v.end(), 3);
来源：http://www.52xcode.cn/Article/details/gt2opeykqkd.html

[S41] C++：类与构造函数
来源：http://www.52xcode.cn/Article/details/gt2sxcbotwx.html

class A { public: A(int v) : x_(v) {} int get() const { return x_; } private: int x_; };
来源：http://www.ydjk.org.cn/Article/details/gt2kiumbmxy.html

[S42] C++：继承与虚函数
来源：http://www.ydjk.org.cn/Article/details/gt2fszykfua.html

class B : public Base { public: void f() override {} };
来源：http://www.52xcode.cn/Article/details/gt2ceuixehz.html

[S43] C++：智能指针
来源：http://www.52xcode.cn/Article/details/gt2klouckii.html

auto p = std::make_unique<int>(5);
来源：http://www.52xcode.cn/Article/details/gt2drafnddk.html

[S44] C++：引用传参
来源：http://www.52xcode.cn/Article/details/gt2ckwmudip.html

void inc(int &x) { ++x; }
来源：http://www.52xcode.cn/Article/details/gt2umddrcjk.html

[S45] C++：lambda
来源：http://www.ydjk.org.cn/Article/details/gt2vbnailoa.html

auto add = [](int a, int b) { return a + b; };
来源：http://www.52xcode.cn/Article/details/gt2yjwsqpvd.html

[S46] C++：函数模板
来源：http://www.ydjk.org.cn/Article/details/gt2jhkduzcm.html

template <typename T> T maxv(T a, T b) { return a > b ? a : b; }
来源：http://www.52xcode.cn/Article/details/gt2hccmocri.html

[S47] C++：结构化绑定遍历
来源：http://www.52xcode.cn/Article/details/gt2vavjczjf.html

for (const auto &[k, v] : m) { std::cout << k << v; }
来源：http://www.ydjk.org.cn/Article/details/gt2qmlwijcs.html

[S48] C++：逐行读文件
来源：http://www.ydjk.org.cn/Article/details/gt2nrnqxtvl.html

std::ifstream in("a.txt");  std::string line;
来源：http://www.ydjk.org.cn/Article/details/gt2cxxzanvv.html

while (std::getline(in, line)) { }
来源：http://www.52xcode.cn/Article/details/gt2aqzqisth.html

[S49] C++：写文件
来源：http://www.ydjk.org.cn/Article/details/gt2dzqdqqws.html

std::ofstream out("a.txt");  out << "hi\n";
来源：http://www.ydjk.org.cn/Article/details/gt2yguqdyjp.html

[S50] C++：格式化数字
来源：http://www.52xcode.cn/Article/details/gt2vhqfeapc.html

std::ostringstream os;  os << std::fixed << std::setprecision(2) << 3.14159;
来源：http://www.52xcode.cn/Article/details/gt2nxrvwhny.html

[S51] C++：显式类型转换
来源：http://www.52xcode.cn/Article/details/gt2fgrjmcjq.html

static_cast<double>(a) / b
来源：http://www.ydjk.org.cn/Article/details/gt2oazsvyfi.html

[S52] C++：const 与 noexcept
来源：http://www.ydjk.org.cn/Article/details/gt2bdwlrspm.html

int size() const noexcept { return n_; }
来源：http://www.ydjk.org.cn/Article/details/gt2wutnmybf.html

[S53] C++：移动语义
来源：http://www.52xcode.cn/Article/details/gt2kearugdz.html

std::vector<int> w = std::move(v);
来源：http://www.52xcode.cn/Article/details/gt2nwxngxyq.html

[S54] C++：异常处理
来源：http://www.52xcode.cn/Article/details/gt2tstvcezf.html

try { throw std::runtime_error("x"); } catch (const std::exception &e) { }
来源：http://www.ydjk.org.cn/Article/details/gt2nxrbbxmb.html

[S55] C++：结构化绑定
来源：http://www.52xcode.cn/Article/details/gt2ahxqrwpp.html

auto [a, b] = std::make_pair(1, 2);
来源：http://www.ydjk.org.cn/Article/details/gt2zbqwpuay.html

[S56] C++：optional
来源：http://www.52xcode.cn/Article/details/gt2gxuaextj.html

std::optional<int> o = 5;  if (o) { int v = *o; }
来源：http://www.52xcode.cn/Article/details/gt2mxfeccfg.html

[S57] C++：编译期常量
来源：http://www.ydjk.org.cn/Article/details/gt2gguimowd.html

constexpr int N = 10;
来源：http://www.52xcode.cn/Article/details/gt2kubcwvuf.html

[S58] C++：命名空间
来源：http://www.52xcode.cn/Article/details/gt2ufdwmmna.html

namespace ns { int f() { return 1; } }
来源：http://www.ydjk.org.cn/Article/details/gt2nbkvaxsa.html

[S59] C++：静态断言
来源：http://www.ydjk.org.cn/Article/details/gt2jccuchbv.html

static_assert(sizeof(int) == 4, "int 必须 4 字节");
来源：http://www.52xcode.cn/Article/details/gt2dagtevok.html

[S60] C++：遍历并删除元素
来源：http://www.ydjk.org.cn/Article/details/gt2gbdqrnep.html

v.erase(std::remove_if(v.begin(), v.end(), [](int x) { return x < 0; }), v.end());
来源：http://www.ydjk.org.cn/Article/details/gt2yojljgdu.html

================================================================================
来源：http://www.ydjk.org.cn/Article/details/gt2pykmupiq.html

T. 其他语言补充（Kotlin / Swift / Lua / Perl / Scala）
来源：http://www.52xcode.cn/Article/details/gt2usvsbcvv.html

================================================================================
来源：http://www.ydjk.org.cn/Article/details/gt2kyulkivi.html

[T01] Kotlin：Hello World
来源：http://www.ydjk.org.cn/Article/details/gt2ynwsxjwz.html

println("Hello")
来源：http://www.52xcode.cn/Article/details/gt2ilijhwlo.html

[T02] Kotlin：变量
来源：http://www.52xcode.cn/Article/details/gt2zqlcblol.html

val a = 1;  var b = 2        // val 只读，var 可变
来源：http://www.52xcode.cn/Article/details/gt2xorbdwng.html

[T03] Kotlin：字符串模板
来源：http://www.ydjk.org.cn/Article/details/gt2daiybptg.html

"值: $b"
来源：http://www.ydjk.org.cn/Article/details/gt2flewokkb.html

[T04] Kotlin：空安全
来源：http://www.ydjk.org.cn/Article/details/gt2jagfmsmg.html

val n: String? = null;  n?.length
来源：http://www.ydjk.org.cn/Article/details/gt2zdfjpalg.html

[T05] Kotlin：when 表达式
来源：http://www.52xcode.cn/Article/details/gt2kxitsost.html

val s = when (x) { 1 -> "一" else -> "其他" }   // 多分支时每个分支单独一行
来源：http://www.52xcode.cn/Article/details/gt2kvmposce.html

[T06] Kotlin：集合映射
来源：http://www.ydjk.org.cn/Article/details/gt2uiijxeoj.html

listOf(1, 2, 3).map { it * 2 }
来源：http://www.52xcode.cn/Article/details/gt2urxpzmin.html

[T07] Kotlin：集合过滤
来源：http://www.ydjk.org.cn/Article/details/gt2dheovrco.html

listOf(1, 2, 3).filter { it > 1 }
来源：http://www.52xcode.cn/Article/details/gt2dkizavds.html

[T08] Kotlin：数据类
来源：http://www.ydjk.org.cn/Article/details/gt2rnoapcbm.html

data class User(val name: String, val age: Int)
来源：http://www.ydjk.org.cn/Article/details/gt2jwkgdugy.html

[T09] Kotlin：扩展函数
来源：http://www.52xcode.cn/Article/details/gt2oojhhggl.html

fun String.exclaim() = this + "!"
来源：http://www.52xcode.cn/Article/details/gt2ppcoeefw.html

[T10] Kotlin：默认参数
来源：http://www.52xcode.cn/Article/details/gt2melugsji.html

fun greet(name: String = "World") = "Hi $name"
来源：http://www.52xcode.cn/Article/details/gt2yxryvkgp.html

[T11] Kotlin：协程
来源：http://www.52xcode.cn/Article/details/gt2ryqqcfuw.html

GlobalScope.launch { delay(1000); println("done") }
来源：http://www.52xcode.cn/Article/details/gt2urgtbcjn.html

[T12] Kotlin：解构声明
来源：http://www.52xcode.cn/Article/details/gt2pnsrakps.html

val (a, b) = Pair(1, 2)
来源：http://www.ydjk.org.cn/Article/details/gt2xavagpxa.html

[T13] Kotlin：只读 Map
来源：http://www.ydjk.org.cn/Article/details/gt2ijspcebg.html

val m = mapOf("a" to 1)
来源：http://www.52xcode.cn/Article/details/gt2sogbsbqr.html

[T14] Kotlin：循环
来源：http://www.ydjk.org.cn/Article/details/gt2tyxwmqzm.html

for (i in 1..10) println(i)
来源：http://www.ydjk.org.cn/Article/details/gt2gdeavsrv.html

[T15] Kotlin：接口
来源：http://www.52xcode.cn/Article/details/gt2qyzztxsa.html

interface Shape { fun area(): Double }
来源：http://www.52xcode.cn/Article/details/gt2kykjyjwb.html

[T16] Swift：Hello World
来源：http://www.ydjk.org.cn/Article/details/gt2jmsfqotg.html

print("Hello")
来源：http://www.ydjk.org.cn/Article/details/gt2vallblxw.html

[T17] Swift：变量与常量
来源：http://www.52xcode.cn/Article/details/gt2kspxdauh.html

var a = 1;  let b = 2
来源：http://www.ydjk.org.cn/Article/details/gt2nswpukch.html

[T18] Swift：字符串插值
来源：http://www.ydjk.org.cn/Article/details/gt2elwioplc.html

"值: \(b)"
来源：http://www.ydjk.org.cn/Article/details/gt2rvhseqcf.html

[T19] Swift：可选绑定
来源：http://www.52xcode.cn/Article/details/gt2ziobxgrf.html

if let n = opt { print(n) }
来源：http://www.ydjk.org.cn/Article/details/gt2sqeihdod.html

[T20] Swift：数组操作
来源：http://www.ydjk.org.cn/Article/details/gt2zyvldcyr.html

var a = [1, 2, 3];  a.append(4)
来源：http://www.52xcode.cn/Article/details/gt2sjtneyff.html

[T21] Swift：遍历
来源：http://www.52xcode.cn/Article/details/gt2vspnyfgs.html

for x in a { print(x) }
来源：http://www.52xcode.cn/Article/details/gt2qnpvnlbi.html

[T22] Swift：字典
来源：http://www.52xcode.cn/Article/details/gt2jqpsbuqg.html

var d = ["a": 1];  d["b"] = 2
来源：http://www.ydjk.org.cn/Article/details/gt2gdqmpasq.html

[T23] Swift：函数
来源：http://www.ydjk.org.cn/Article/details/gt2bqwoopsy.html

func add(_ a: Int, _ b: Int) -> Int { a + b }
来源：http://www.ydjk.org.cn/Article/details/gt2uueqilgv.html

[T24] Swift：闭包
来源：http://www.ydjk.org.cn/Article/details/gt2kcgauehb.html

let f = { (x: Int) -> Int in x * 2 }
来源：http://www.ydjk.org.cn/Article/details/gt2usqfbkar.html

[T25] Swift：结构体
来源：http://www.52xcode.cn/Article/details/gt2vkxzbauv.html

struct P { var x: Int }
来源：http://www.ydjk.org.cn/Article/details/gt2dykvwbvg.html

[T26] Swift：类与重写
来源：http://www.ydjk.org.cn/Article/details/gt2qwujflfb.html

class A: Base { override func f() {} }
来源：http://www.ydjk.org.cn/Article/details/gt2inypeoyw.html

[T27] Swift：错误处理
来源：http://www.52xcode.cn/Article/details/gt2oegbjpof.html

do { try f() } catch { print(error) }
来源：http://www.52xcode.cn/Article/details/gt2xhjkyiix.html

[T28] Swift：枚举
来源：http://www.52xcode.cn/Article/details/gt2qtditplk.html

enum Color { case red, green }
来源：http://www.52xcode.cn/Article/details/gt2ezajtcxc.html

[T29] Swift：guard 提前返回
来源：http://www.52xcode.cn/Article/details/gt2vnagvexa.html

guard let x = opt else { return }
来源：http://www.52xcode.cn/Article/details/gt2zglbgvgs.html

[T30] Swift：协议
来源：http://www.ydjk.org.cn/Article/details/gt2pkwazwyl.html

protocol Shape { func area() -> Double }
来源：http://www.52xcode.cn/Article/details/gt2cmkyohiu.html

[T31] Lua：Hello World
来源：http://www.ydjk.org.cn/Article/details/gt2wgxrobbr.html

print("Hello")
来源：http://www.ydjk.org.cn/Article/details/gt2kbeqoewh.html

[T32] Lua：局部变量
来源：http://www.52xcode.cn/Article/details/gt2nqrjcvaa.html

local a = 1
来源：http://www.ydjk.org.cn/Article/details/gt2myhtvirf.html

[T33] Lua：表（数组）
来源：http://www.ydjk.org.cn/Article/details/gt2qkgqxxpc.html

local t = {1, 2, 3};  t[4] = 4
来源：http://www.ydjk.org.cn/Article/details/gt2djmziwdi.html

[T34] Lua：遍历表
来源：http://www.ydjk.org.cn/Article/details/gt2ihcumizk.html

for i, v in ipairs(t) do print(i, v) end
来源：http://www.ydjk.org.cn/Article/details/gt2jktnvmrh.html

[T35] Lua：字典表
来源：http://www.52xcode.cn/Article/details/gt2dixffvcg.html

local d = { a = 1 };  d.b = 2
来源：http://www.52xcode.cn/Article/details/gt2ypmxamqp.html

[T36] Lua：函数
来源：http://www.52xcode.cn/Article/details/gt2bfedxala.html

function add(a, b) return a + b end
来源：http://www.ydjk.org.cn/Article/details/gt2oykxphlp.html

[T37] Lua：字符串拼接
来源：http://www.ydjk.org.cn/Article/details/gt2oggbnkyk.html

"a" .. "b"
来源：http://www.ydjk.org.cn/Article/details/gt2fvihqclu.html

[T38] Lua：条件
来源：http://www.52xcode.cn/Article/details/gt2gpdeadnn.html

if x > 0 then print("正") end
来源：http://www.52xcode.cn/Article/details/gt2puddihvc.html

[T39] Lua：模式匹配
来源：http://www.ydjk.org.cn/Article/details/gt2jjkvegij.html

string.find(s, "%d+")
来源：http://www.52xcode.cn/Article/details/gt2zdudzaze.html

[T40] Lua：元表
来源：http://www.ydjk.org.cn/Article/details/gt2wuvatsbl.html

setmetatable({}, { __index = base })
来源：http://www.52xcode.cn/Article/details/gt2tiserffg.html

[T41] Perl：Hello World
来源：http://www.ydjk.org.cn/Article/details/gt2hqicaqzz.html

print "Hello\n";
来源：http://www.52xcode.cn/Article/details/gt2nywikfbt.html

[T42] Perl：变量类型
来源：http://www.52xcode.cn/Article/details/gt2lzmdxuxr.html

my $a = 1;  my @arr = (1, 2, 3);  my %h = (a => 1);
来源：http://www.ydjk.org.cn/Article/details/gt2orkdkssa.html

[T43] Perl：字符串插值
来源：http://www.52xcode.cn/Article/details/gt2ptoyrcyr.html

"值: $a"
来源：http://www.52xcode.cn/Article/details/gt2nyngjheg.html

[T44] Perl：条件
来源：http://www.52xcode.cn/Article/details/gt2ukoigaqz.html

if ($a > 0) { print "正"; }
来源：http://www.52xcode.cn/Article/details/gt2bsdicfvh.html

[T45] Perl：数组遍历
来源：http://www.ydjk.org.cn/Article/details/gt2fhuafnmg.html

for my $x (@arr) { print $x; }
来源：http://www.ydjk.org.cn/Article/details/gt2feyjusmj.html

[T46] Perl：哈希操作
来源：http://www.ydjk.org.cn/Article/details/gt2llbkitmw.html

$h{b} = 2;  for my $k (keys %h) { print "$k=$h{$k}"; }
来源：http://www.52xcode.cn/Article/details/gt2jvksdbhu.html

[T47] Perl：正则捕获
来源：http://www.ydjk.org.cn/Article/details/gt2uyprlone.html

if ($s =~ /(\d+)/) { print $1; }
来源：http://www.52xcode.cn/Article/details/gt2chjjzzxv.html

[T48] Perl：正则替换
来源：http://www.52xcode.cn/Article/details/gt2pbqszfgt.html

$s =~ s/old/new/g;
来源：http://www.ydjk.org.cn/Article/details/gt2qgicksow.html

[T49] Perl：函数
来源：http://www.ydjk.org.cn/Article/details/gt2miuzloen.html

sub add { my ($a, $b) = @_; return $a + $b; }
来源：http://www.52xcode.cn/Article/details/gt2ppqgpckj.html

[T50] Perl：逐行读文件
来源：http://www.ydjk.org.cn/Article/details/gt2pfqzlsem.html

open my $fh, "<", "a.txt" or die $!;
来源：http://www.ydjk.org.cn/Article/details/gt2tgadiegr.html

while (my $line = <$fh>) { print $line; }
来源：http://www.52xcode.cn/Article/details/gt2guwhuyvc.html

[T51] Scala：Hello World
来源：http://www.ydjk.org.cn/Article/details/gt2qwtjssmx.html

println("Hello")
来源：http://www.52xcode.cn/Article/details/gt2ycohinlx.html

[T52] Scala：变量
来源：http://www.52xcode.cn/Article/details/gt2tadgtwvb.html

val a = 1;  var b = 2
来源：http://www.52xcode.cn/Article/details/gt2xubypqye.html

[T53] Scala：字符串插值
来源：http://www.ydjk.org.cn/Article/details/gt2wawjfogb.html

s"值: $b"
来源：http://www.ydjk.org.cn/Article/details/gt2cjyuedau.html

[T54] Scala：集合映射
来源：http://www.52xcode.cn/Article/details/gt2irmgqwmj.html

List(1, 2, 3).map(_ * 2)
来源：http://www.ydjk.org.cn/Article/details/gt2lbddgyzm.html

[T55] Scala：集合过滤
来源：http://www.52xcode.cn/Article/details/gt2btmposyi.html

List(1, 2, 3).filter(_ > 1)
来源：http://www.ydjk.org.cn/Article/details/gt2jbvapvsh.html

[T56] Scala：样例类
来源：http://www.52xcode.cn/Article/details/gt2ptwwpuiv.html

case class User(name: String, age: Int)
来源：http://www.52xcode.cn/Article/details/gt2kbholgxq.html

[T57] Scala：模式匹配
来源：http://www.ydjk.org.cn/Article/details/gt2wgpwmwns.html

x match { case 1 => "一"; case _ => "其他" }
来源：http://www.52xcode.cn/Article/details/gt2jrbetgci.html

[T58] Scala：函数定义
来源：http://www.ydjk.org.cn/Article/details/gt2hggqmxoh.html

def add(a: Int, b: Int): Int = a + b
来源：http://www.52xcode.cn/Article/details/gt2poirfykf.html

[T59] Scala：循环
来源：http://www.ydjk.org.cn/Article/details/gt2iabbmoao.html

for (i <- 1 to 10) println(i)
来源：http://www.ydjk.org.cn/Article/details/gt2bvkcgrrw.html

[T60] Scala：折叠
来源：http://www.52xcode.cn/Article/details/gt2jzbpukao.html

List(1, 2, 3).foldLeft(0)(_ + _)
来源：http://www.52xcode.cn/Article/details/gt2cjjrhayw.html

================================================================================
来源：http://www.ydjk.org.cn/Article/details/gt2wwhecfxw.html

U. 高频实用片段（Python / PHP / JavaScript 各 40 条）
来源：http://www.ydjk.org.cn/Article/details/gt2eujkufga.html

================================================================================
来源：http://www.ydjk.org.cn/Article/details/gt2fhygskqp.html

[U01] Py：创建虚拟环境
来源：http://www.ydjk.org.cn/Article/details/gt2swirbgps.html

python -m venv .venv && source .venv/bin/activate
来源：http://www.52xcode.cn/Article/details/gt2dtpxqgty.html

[U02] Py：导出 / 安装依赖
来源：http://www.ydjk.org.cn/Article/details/gt2bilzpavw.html

pip freeze > requirements.txt;  pip install -r requirements.txt
来源：http://www.52xcode.cn/Article/details/gt2mzswuhli.html

[U03] Py：加载 .env 配置
来源：http://www.ydjk.org.cn/Article/details/gt2rnnpssvz.html

from dotenv import load_dotenv; load_dotenv()
来源：http://www.ydjk.org.cn/Article/details/gt2dpjkdnxd.html

[U04] Py：变量调试打印
来源：http://www.52xcode.cn/Article/details/gt2zsdpixut.html

print(f"{x=}")            # 输出 x=值，Python 3.8+
来源：http://www.ydjk.org.cn/Article/details/gt2widvkhrq.html

[U05] Py：列表去重且保序
来源：http://www.52xcode.cn/Article/details/gt2lyfzqswa.html

list(dict.fromkeys(arr))
来源：http://www.52xcode.cn/Article/details/gt2pxjprmcd.html

[U06] Py：合并两个字典
来源：http://www.52xcode.cn/Article/details/gt2gogaqibp.html

{**a, **b}
来源：http://www.ydjk.org.cn/Article/details/gt2dhqllyqz.html

[U07] Py：反转字典键值
来源：http://www.ydjk.org.cn/Article/details/gt2ncepwmpw.html

{v: k for k, v in d.items()}
来源：http://www.52xcode.cn/Article/details/gt2pfqbbcso.html

[U08] Py：展平二维列表
来源：http://www.ydjk.org.cn/Article/details/gt2ylabbdvt.html

[y for x in nested for y in x]
来源：http://www.ydjk.org.cn/Article/details/gt2itemexjj.html


<!-- 参考信息 -->