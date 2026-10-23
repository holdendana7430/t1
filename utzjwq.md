代发 wailian999

openssl rand -hex 16
来源：http://www.52xcode.cn/Article/details/gt3agnuzieq.html

[R68] 计算文件校验值
来源：http://www.52xcode.cn/Article/details/gt3rwonwoin.html

sha256sum a.txt;  md5sum a.txt
来源：http://www.ydjk.org.cn/Article/details/gt3qwrazfzf.html

[R69] 生成随机密码
来源：http://www.ydjk.org.cn/Article/details/gt3vrxpmucm.html

head -c 16 /dev/urandom | base64
来源：http://www.52xcode.cn/Article/details/gt3fonqmlfj.html

[R70] 时间戳与互转
来源：http://www.52xcode.cn/Article/details/gt3bfmzdkri.html

date +%s;  date -d @1700000000
来源：http://www.52xcode.cn/Article/details/gt3wkzcqweo.html

[R71] 日期格式化
来源：http://www.ydjk.org.cn/Article/details/gt3gjgpzcxf.html

date +"%Y-%m-%d %H:%M:%S"
来源：http://www.ydjk.org.cn/Article/details/gt3abgqlezj.html

[R72] 等待端口就绪
来源：http://www.ydjk.org.cn/Article/details/gt3fdrdzcte.html

until nc -z localhost 3306; do sleep 1; done
来源：http://www.ydjk.org.cn/Article/details/gt3jtfzicoq.html

[R73] 分割大日志
来源：http://www.ydjk.org.cn/Article/details/gt3xmtgtqgn.html

split -l 1000 big.log part_
来源：http://www.52xcode.cn/Article/details/gt3yppepbex.html

[R74] 批量重命名
来源：http://www.ydjk.org.cn/Article/details/gt3emmkpcvy.html

for f in *.jpeg; do mv "$f" "${f%.jpeg}.jpg"; done
来源：http://www.52xcode.cn/Article/details/gt3whqsryua.html

[R75] 导出环境变量
来源：http://www.52xcode.cn/Article/details/gt3vengmhbd.html

export PATH="$HOME/bin:$PATH"
来源：http://www.52xcode.cn/Article/details/gt3iqviffah.html

[R76] 使用临时文件
来源：http://www.52xcode.cn/Article/details/gt3xidiqwxh.html

tmp=$(mktemp); trap 'rm -f "$tmp"' EXIT
来源：http://www.ydjk.org.cn/Article/details/gt3ieszoxuy.html

[R77] 读取用户输入
来源：http://www.52xcode.cn/Article/details/gt3tbizabio.html

read -rp "请输入: " ans
来源：http://www.ydjk.org.cn/Article/details/gt3tcmthyuv.html

[R78] 交互式菜单
来源：http://www.52xcode.cn/Article/details/gt3rqrvwojh.html

select opt in a b c; do echo "$opt"; break; done
来源：http://www.ydjk.org.cn/Article/details/gt3vhvjxkqt.html

[R79] 解析命令行选项
来源：http://www.52xcode.cn/Article/details/gt3xpjwbvge.html

while getopts "v:f:" o; do case $o in v) V=$OPTARG ;; f) F=$OPTARG ;; esac; done
来源：http://www.52xcode.cn/Article/details/gt3xgibmfqf.html

[R80] 查看脚本执行耗时
来源：http://www.52xcode.cn/Article/details/gt3yrpzfofi.html

time ./run.sh
来源：http://www.52xcode.cn/Article/details/gt3urtnhesr.html

================================================================================
来源：http://www.ydjk.org.cn/Article/details/gt3vpuhynmo.html

S. C / C++ 专题
来源：http://www.52xcode.cn/Article/details/gt3ucrwdhzc.html

================================================================================
来源：http://www.52xcode.cn/Article/details/gt3uzbvaeno.html

[S01] C：Hello World
来源：http://www.52xcode.cn/Article/details/gt3sleojxwr.html

#include <stdio.h>
来源：http://www.52xcode.cn/Article/details/gt3jiyofkgr.html

int main(void) { printf("Hello\n"); return 0; }
来源：http://www.52xcode.cn/Article/details/gt3kvghowwt.html

[S02] C：变量与格式化输出
来源：http://www.52xcode.cn/Article/details/gt3bhopamfl.html

int a = 10; printf("%d\n", a);
来源：http://www.ydjk.org.cn/Article/details/gt3abkntdlh.html

[S03] C：读入整数
来源：http://www.52xcode.cn/Article/details/gt3hhitavqs.html

int x; scanf("%d", &x);
来源：http://www.52xcode.cn/Article/details/gt3zosvlauz.html

[S04] C：字符串复制
来源：http://www.52xcode.cn/Article/details/gt3whurznre.html

char dst[32]; strcpy(dst, "hi");
来源：http://www.ydjk.org.cn/Article/details/gt3vdxlblen.html

[S05] C：字符串长度
来源：http://www.ydjk.org.cn/Article/details/gt3rulhigjo.html

strlen(s)
来源：http://www.52xcode.cn/Article/details/gt3zjhhkobw.html

[S06] C：字符串比较
来源：http://www.52xcode.cn/Article/details/gt3irovwsix.html

strcmp(a, b) == 0
来源：http://www.ydjk.org.cn/Article/details/gt3impqaokz.html

[S07] C：数组遍历求和
来源：http://www.52xcode.cn/Article/details/gt3htdmwwmr.html

for (int i = 0; i < n; i++) sum += a[i];
来源：http://www.ydjk.org.cn/Article/details/gt3gkkojzny.html

[S08] C：动态内存分配与释放
来源：http://www.ydjk.org.cn/Article/details/gt3ilscdwbu.html

int *p = malloc(sizeof(int) * n); ... free(p);
来源：http://www.ydjk.org.cn/Article/details/gt3milgvyim.html

[S09] C：结构体定义与初始化
来源：http://www.52xcode.cn/Article/details/gt3gbonegng.html

struct Point { int x, y; };  struct Point p = {1, 2};
来源：http://www.52xcode.cn/Article/details/gt3qenxkryo.html

[S10] C：指针与解引用
来源：http://www.52xcode.cn/Article/details/gt3gqewgkqo.html

int *p = &a;  *p = 5;
来源：http://www.ydjk.org.cn/Article/details/gt3smzduhmz.html

[S11] C：逐行读文件
来源：http://www.52xcode.cn/Article/details/gt3ytfwqyks.html

FILE *f = fopen("a.txt", "r");
来源：http://www.52xcode.cn/Article/details/gt3eoknieps.html

while (fgets(buf, sizeof buf, f)) { }
来源：http://www.52xcode.cn/Article/details/gt3wxyyvjrm.html

fclose(f);
来源：http://www.ydjk.org.cn/Article/details/gt3uaoycsvh.html

[S12] C：写文件
来源：http://www.ydjk.org.cn/Article/details/gt3zsettvvk.html

FILE *f = fopen("a.txt", "w");  fprintf(f, "hi\n");  fclose(f);
来源：http://www.ydjk.org.cn/Article/details/gt3kxbnfqre.html

[S13] C：宏定义
来源：http://www.52xcode.cn/Article/details/gt3zksntjpj.html

#define MAX(a, b) ((a) > (b) ? (a) : (b))
来源：http://www.ydjk.org.cn/Article/details/gt3hqxhujez.html

[S14] C：枚举
来源：http://www.ydjk.org.cn/Article/details/gt3bmiyxgzp.html

enum Color { RED, GREEN, BLUE };
来源：http://www.ydjk.org.cn/Article/details/gt3mttkhezm.html

[S15] C：类型转换
来源：http://www.52xcode.cn/Article/details/gt3fkazuhbw.html

(double) a / b
来源：http://www.52xcode.cn/Article/details/gt3kvqdqjyz.html

[S16] C：位操作置位
来源：http://www.52xcode.cn/Article/details/gt3cyctfqgf.html

x |= (1 << 3);
来源：http://www.ydjk.org.cn/Article/details/gt3casolmth.html

[S17] C：安全拼接字符串
来源：http://www.ydjk.org.cn/Article/details/gt3kncluycg.html

snprintf(buf, sizeof buf, "%s%s", a, b);
来源：http://www.ydjk.org.cn/Article/details/gt3ololbuan.html

[S18] C：命令行参数
来源：http://www.52xcode.cn/Article/details/gt3wrwkzvfa.html

int main(int argc, char **argv)
来源：http://www.52xcode.cn/Article/details/gt3raskoxjg.html

[S19] C：快速排序
来源：http://www.ydjk.org.cn/Article/details/gt3rgnvajua.html

qsort(a, n, sizeof(int), cmp);
来源：http://www.ydjk.org.cn/Article/details/gt3nfuelexf.html

[S20] C：二分查找
来源：http://www.52xcode.cn/Article/details/gt3luydbeov.html

bsearch(&key, a, n, sizeof(int), cmp);
来源：http://www.52xcode.cn/Article/details/gt3lvziyvgn.html

[S21] C：字符类别判断
来源：http://www.52xcode.cn/Article/details/gt3pyrbmiep.html

isdigit(c);  isalpha(c);  isspace(c);
来源：http://www.ydjk.org.cn/Article/details/gt3mcofwnqn.html

[S22] C：字符串转数字
来源：http://www.ydjk.org.cn/Article/details/gt3lbsidslk.html

atoi("42");  strtod("3.14", NULL);
来源：http://www.ydjk.org.cn/Article/details/gt3xelttelo.html

[S23] C：随机数
来源：http://www.52xcode.cn/Article/details/gt3pzusedjx.html

srand(time(NULL));  int r = rand() % 100;
来源：http://www.ydjk.org.cn/Article/details/gt3uvgnsbje.html

[S24] C：获取本地时间
来源：http://www.52xcode.cn/Article/details/gt3pnnfmxii.html

time_t t = time(NULL);  struct tm *tm = localtime(&t);
来源：http://www.52xcode.cn/Article/details/gt3kyjvrhyp.html

[S25] C：内存拷贝
来源：http://www.ydjk.org.cn/Article/details/gt3hxggcsan.html

memcpy(dst, src, n);
来源：http://www.52xcode.cn/Article/details/gt3dhgsqdsk.html

[S26] C：内存清零
来源：http://www.ydjk.org.cn/Article/details/gt3yranhefv.html

memset(a, 0, sizeof a);
来源：http://www.52xcode.cn/Article/details/gt3tefrqgju.html

[S27] C：定义常量
来源：http://www.ydjk.org.cn/Article/details/gt3sooyqndp.html

const double PI = 3.14159;
来源：http://www.52xcode.cn/Article/details/gt3lfxzspxw.html

[S28] C：静态变量
来源：http://www.52xcode.cn/Article/details/gt3rwzdzzll.html

static int counter = 0;
来源：http://www.52xcode.cn/Article/details/gt3kvxbgqgg.html

[S29] C：变参函数
来源：http://www.ydjk.org.cn/Article/details/gt3khdrwkbk.html

va_list ap; va_start(ap, fmt); vprintf(fmt, ap); va_end(ap);
来源：http://www.ydjk.org.cn/Article/details/gt3ncqnhhsw.html

[S30] C：头文件保护
来源：http://www.ydjk.org.cn/Article/details/gt3vvtpayet.html

#ifndef X_H
来源：http://www.ydjk.org.cn/Article/details/gt3vpcijrtr.html

#define X_H
来源：http://www.ydjk.org.cn/Article/details/gt3csifpmxj.html

#endif
来源：http://www.52xcode.cn/Article/details/gt3fxoxwjlo.html

[S31] C++：Hello World
来源：http://www.52xcode.cn/Article/details/gt3mqmgpyhx.html

#include <iostream>
来源：http://www.ydjk.org.cn/Article/details/gt3unhrkijh.html

int main() { std::cout << "Hello\n"; }
来源：http://www.ydjk.org.cn/Article/details/gt3xkrqsctk.html

[S32] C++：字符串
来源：http://www.ydjk.org.cn/Article/details/gt3ugrzylok.html

std::string s = "hi";  s += "!";
来源：http://www.52xcode.cn/Article/details/gt3duvseolu.html

[S33] C++：vector 增删
来源：http://www.ydjk.org.cn/Article/details/gt3hjyltfgx.html

std::vector<int> v{1, 2, 3};  v.push_back(4);
来源：http://www.52xcode.cn/Article/details/gt3eorrealt.html

[S34] C++：遍历 vector
来源：http://www.ydjk.org.cn/Article/details/gt3mqeskqiy.html

for (auto &x : v) { std::cout << x; }
来源：http://www.ydjk.org.cn/Article/details/gt3mdnvzvym.html

[S35] C++：map
来源：http://www.52xcode.cn/Article/details/gt3mlcejjph.html

std::map<std::string, int> m;  m["a"] = 1;
来源：http://www.52xcode.cn/Article/details/gt3cydbctoj.html

[S36] C++：unordered_map
来源：http://www.ydjk.org.cn/Article/details/gt3wwszdkex.html

std::unordered_map<std::string, int> m;  m["a"] = 1;
来源：http://www.ydjk.org.cn/Article/details/gt3nagvksvb.html

[S37] C++：set
来源：http://www.52xcode.cn/Article/details/gt3dzroxnke.html

std::set<int> s{1, 2, 3};  s.insert(4);
来源：http://www.52xcode.cn/Article/details/gt3awazimfu.html

[S38] C++：排序
来源：http://www.ydjk.org.cn/Article/details/gt3asxzndxr.html

std::sort(v.begin(), v.end());
来源：http://www.52xcode.cn/Article/details/gt3mqqhtccx.html

[S39] C++：自定义比较器排序
来源：http://www.ydjk.org.cn/Article/details/gt3dkzpbnxv.html

std::sort(v.begin(), v.end(), [](int a, int b) { return a > b; });
来源：http://www.52xcode.cn/Article/details/gt3ngspdtyj.html

[S40] C++：查找元素
来源：http://www.ydjk.org.cn/Article/details/gt3lofrwxju.html

auto it = std::find(v.begin(), v.end(), 3);
来源：http://www.52xcode.cn/Article/details/gt3oxneaemt.html

[S41] C++：类与构造函数
来源：http://www.52xcode.cn/Article/details/gt3buelguzw.html

class A { public: A(int v) : x_(v) {} int get() const { return x_; } private: int x_; };
来源：http://www.ydjk.org.cn/Article/details/gt3uuuoysoo.html

[S42] C++：继承与虚函数
来源：http://www.52xcode.cn/Article/details/gt3lzdfvzxj.html

class B : public Base { public: void f() override {} };
来源：http://www.ydjk.org.cn/Article/details/gt3salcskwp.html

[S43] C++：智能指针
来源：http://www.52xcode.cn/Article/details/gt3ctlngtbz.html

auto p = std::make_unique<int>(5);
来源：http://www.52xcode.cn/Article/details/gt3mzckmaqp.html

[S44] C++：引用传参
来源：http://www.52xcode.cn/Article/details/gt3qkqtbaoc.html

void inc(int &x) { ++x; }
来源：http://www.52xcode.cn/Article/details/gt3hjovdxyx.html

[S45] C++：lambda
来源：http://www.ydjk.org.cn/Article/details/gt3ewsyxdpb.html

auto add = [](int a, int b) { return a + b; };
来源：http://www.ydjk.org.cn/Article/details/gt3tftchurb.html

[S46] C++：函数模板
来源：http://www.52xcode.cn/Article/details/gt3xhsweewa.html

template <typename T> T maxv(T a, T b) { return a > b ? a : b; }
来源：http://www.ydjk.org.cn/Article/details/gt3uiwhpjtk.html

[S47] C++：结构化绑定遍历
来源：http://www.ydjk.org.cn/Article/details/gt3sefbnnlr.html

for (const auto &[k, v] : m) { std::cout << k << v; }
来源：http://www.ydjk.org.cn/Article/details/gt3dbvtwvul.html

[S48] C++：逐行读文件
来源：http://www.52xcode.cn/Article/details/gt3ysbiedqp.html

std::ifstream in("a.txt");  std::string line;
来源：http://www.52xcode.cn/Article/details/gt3ycuoibym.html

while (std::getline(in, line)) { }
来源：http://www.52xcode.cn/Article/details/gt3bzfkvxin.html

[S49] C++：写文件
来源：http://www.ydjk.org.cn/Article/details/gt3aizkdlov.html

std::ofstream out("a.txt");  out << "hi\n";
来源：http://www.52xcode.cn/Article/details/gt3dnkcmtep.html

[S50] C++：格式化数字
来源：http://www.ydjk.org.cn/Article/details/gt3qtcdvtvp.html

std::ostringstream os;  os << std::fixed << std::setprecision(2) << 3.14159;
来源：http://www.52xcode.cn/Article/details/gt3ptzlpsdt.html

[S51] C++：显式类型转换
来源：http://www.ydjk.org.cn/Article/details/gt3ddskygju.html

static_cast<double>(a) / b
来源：http://www.52xcode.cn/Article/details/gt3csgivipg.html

[S52] C++：const 与 noexcept
来源：http://www.52xcode.cn/Article/details/gt3ajsuhqoa.html

int size() const noexcept { return n_; }
来源：http://www.ydjk.org.cn/Article/details/gt3dmjkgfos.html

[S53] C++：移动语义
来源：http://www.ydjk.org.cn/Article/details/gt3xtsvhrek.html

std::vector<int> w = std::move(v);
来源：http://www.52xcode.cn/Article/details/gt3numdnegh.html

[S54] C++：异常处理
来源：http://www.ydjk.org.cn/Article/details/gt3uodxoajt.html

try { throw std::runtime_error("x"); } catch (const std::exception &e) { }
来源：http://www.52xcode.cn/Article/details/gt3eplujyyi.html

[S55] C++：结构化绑定
来源：http://www.52xcode.cn/Article/details/gt3cqzunyot.html

auto [a, b] = std::make_pair(1, 2);
来源：http://www.52xcode.cn/Article/details/gt3kvqliryf.html

[S56] C++：optional
来源：http://www.ydjk.org.cn/Article/details/gt3euugkrbs.html

std::optional<int> o = 5;  if (o) { int v = *o; }
来源：http://www.ydjk.org.cn/Article/details/gt3ovwtvpuz.html

[S57] C++：编译期常量
来源：http://www.ydjk.org.cn/Article/details/gt3sryksepp.html

constexpr int N = 10;
来源：http://www.ydjk.org.cn/Article/details/gt3qyreyjzq.html

[S58] C++：命名空间
来源：http://www.52xcode.cn/Article/details/gt3ioafzgzl.html

namespace ns { int f() { return 1; } }
来源：http://www.ydjk.org.cn/Article/details/gt3gieeqopv.html

[S59] C++：静态断言
来源：http://www.52xcode.cn/Article/details/gt3pfeoxexr.html

static_assert(sizeof(int) == 4, "int 必须 4 字节");
来源：http://www.ydjk.org.cn/Article/details/gt3olctyawk.html

[S60] C++：遍历并删除元素
来源：http://www.ydjk.org.cn/Article/details/gt3wrxsdfrp.html

v.erase(std::remove_if(v.begin(), v.end(), [](int x) { return x < 0; }), v.end());
来源：http://www.ydjk.org.cn/Article/details/gt3tvfykcvh.html

================================================================================
来源：http://www.52xcode.cn/Article/details/gt3lufayljp.html

T. 其他语言补充（Kotlin / Swift / Lua / Perl / Scala）
来源：http://www.ydjk.org.cn/Article/details/gt3rfqhdqyw.html

================================================================================
来源：http://www.ydjk.org.cn/Article/details/gt3jppulxdg.html

[T01] Kotlin：Hello World
来源：http://www.52xcode.cn/Article/details/gt3kolrzvac.html

println("Hello")
来源：http://www.ydjk.org.cn/Article/details/gt3oadaewpp.html

[T02] Kotlin：变量
来源：http://www.52xcode.cn/Article/details/gt3msnwtiyo.html

val a = 1;  var b = 2        // val 只读，var 可变
来源：http://www.52xcode.cn/Article/details/gt3inebktqg.html

[T03] Kotlin：字符串模板
来源：http://www.ydjk.org.cn/Article/details/gt3lsxhihva.html

"值: $b"
来源：http://www.ydjk.org.cn/Article/details/gt3qfpovffy.html

[T04] Kotlin：空安全
来源：http://www.ydjk.org.cn/Article/details/gt3ubftcdfu.html

val n: String? = null;  n?.length
来源：http://www.52xcode.cn/Article/details/gt3uicdmcfs.html

[T05] Kotlin：when 表达式
来源：http://www.ydjk.org.cn/Article/details/gt3fzmbkzbp.html

val s = when (x) { 1 -> "一" else -> "其他" }   // 多分支时每个分支单独一行
来源：http://www.52xcode.cn/Article/details/gt3hawpojbc.html

[T06] Kotlin：集合映射
来源：http://www.52xcode.cn/Article/details/gt3tscxzwnh.html

listOf(1, 2, 3).map { it * 2 }
来源：http://www.ydjk.org.cn/Article/details/gt3oislspcq.html

[T07] Kotlin：集合过滤
来源：http://www.ydjk.org.cn/Article/details/gt3uzdbkskr.html

listOf(1, 2, 3).filter { it > 1 }
来源：http://www.52xcode.cn/Article/details/gt3obafqmfs.html

[T08] Kotlin：数据类
来源：http://www.52xcode.cn/Article/details/gt3jxmydbku.html

data class User(val name: String, val age: Int)
来源：http://www.ydjk.org.cn/Article/details/gt3ymnpbire.html

[T09] Kotlin：扩展函数
来源：http://www.52xcode.cn/Article/details/gt3fetnhilk.html

fun String.exclaim() = this + "!"
来源：http://www.ydjk.org.cn/Article/details/gt3yxmklbic.html

[T10] Kotlin：默认参数
来源：http://www.ydjk.org.cn/Article/details/gt3dyovaxdi.html

fun greet(name: String = "World") = "Hi $name"
来源：http://www.ydjk.org.cn/Article/details/gt3pjuhyimp.html

[T11] Kotlin：协程
来源：http://www.ydjk.org.cn/Article/details/gt3wzttrpdg.html

GlobalScope.launch { delay(1000); println("done") }
来源：http://www.ydjk.org.cn/Article/details/gt3nhpecdxe.html

[T12] Kotlin：解构声明
来源：http://www.52xcode.cn/Article/details/gt3vnclnxmb.html

val (a, b) = Pair(1, 2)
来源：http://www.52xcode.cn/Article/details/gt3fivlweio.html

[T13] Kotlin：只读 Map
来源：http://www.52xcode.cn/Article/details/gt3zpdtvywz.html

val m = mapOf("a" to 1)
来源：http://www.52xcode.cn/Article/details/gt3spinxnhh.html

[T14] Kotlin：循环
来源：http://www.52xcode.cn/Article/details/gt3mfpqqndy.html

for (i in 1..10) println(i)
来源：http://www.ydjk.org.cn/Article/details/gt3qgpmyadh.html

[T15] Kotlin：接口
来源：http://www.52xcode.cn/Article/details/gt3mjpnnvgh.html

interface Shape { fun area(): Double }
来源：http://www.52xcode.cn/Article/details/gt3wbejgjbf.html

[T16] Swift：Hello World
来源：http://www.ydjk.org.cn/Article/details/gt3zldepzwo.html

print("Hello")
来源：http://www.ydjk.org.cn/Article/details/gt3pkistarr.html

[T17] Swift：变量与常量
来源：http://www.ydjk.org.cn/Article/details/gt3bybcqiaf.html

var a = 1;  let b = 2
来源：http://www.52xcode.cn/Article/details/gt3fqlgaull.html

[T18] Swift：字符串插值
来源：http://www.ydjk.org.cn/Article/details/gt3xalgeqke.html

"值: \(b)"
来源：http://www.ydjk.org.cn/Article/details/gt3xexhnhxi.html

[T19] Swift：可选绑定
来源：http://www.ydjk.org.cn/Article/details/gt3eupcmcay.html

if let n = opt { print(n) }
来源：http://www.52xcode.cn/Article/details/gt3kawovasz.html

[T20] Swift：数组操作
来源：http://www.52xcode.cn/Article/details/gt3gwfnprbf.html

var a = [1, 2, 3];  a.append(4)
来源：http://www.52xcode.cn/Article/details/gt3woxbmnec.html

[T21] Swift：遍历
来源：http://www.52xcode.cn/Article/details/gt3pyvxeccv.html

for x in a { print(x) }
来源：http://www.52xcode.cn/Article/details/gt3mjhunfnf.html

[T22] Swift：字典
来源：http://www.ydjk.org.cn/Article/details/gt3rxkajqlb.html

var d = ["a": 1];  d["b"] = 2
来源：http://www.52xcode.cn/Article/details/gt3cwhlfjfa.html

[T23] Swift：函数
来源：http://www.52xcode.cn/Article/details/gt3yhtnszjh.html

func add(_ a: Int, _ b: Int) -> Int { a + b }
来源：http://www.ydjk.org.cn/Article/details/gt3uepinpyc.html

[T24] Swift：闭包
来源：http://www.ydjk.org.cn/Article/details/gt3gaiavtvc.html

let f = { (x: Int) -> Int in x * 2 }
来源：http://www.ydjk.org.cn/Article/details/gt3vzkkjpww.html

[T25] Swift：结构体
来源：http://www.ydjk.org.cn/Article/details/gt3ssulityc.html

struct P { var x: Int }
来源：http://www.ydjk.org.cn/Article/details/gt3hlxglumb.html

[T26] Swift：类与重写
来源：http://www.ydjk.org.cn/Article/details/gt3eadrmrkz.html

class A: Base { override func f() {} }
来源：http://www.ydjk.org.cn/Article/details/gt3qwnjrkmo.html

[T27] Swift：错误处理
来源：http://www.ydjk.org.cn/Article/details/gt3cxhhmtmj.html

do { try f() } catch { print(error) }
来源：http://www.ydjk.org.cn/Article/details/gt3isheolfx.html

[T28] Swift：枚举
来源：http://www.ydjk.org.cn/Article/details/gt3orpmqifz.html

enum Color { case red, green }
来源：http://www.ydjk.org.cn/Article/details/gt3osxpxjly.html

[T29] Swift：guard 提前返回
来源：http://www.52xcode.cn/Article/details/gt3sxwzhtmf.html

guard let x = opt else { return }
来源：http://www.52xcode.cn/Article/details/gt3jrpctbwy.html

[T30] Swift：协议
来源：http://www.52xcode.cn/Article/details/gt3nnhdzjdm.html

protocol Shape { func area() -> Double }
来源：http://www.52xcode.cn/Article/details/gt3apkoslnq.html

[T31] Lua：Hello World
来源：http://www.ydjk.org.cn/Article/details/gt3tfoakdnd.html

print("Hello")
来源：http://www.52xcode.cn/Article/details/gt3pvqsaooj.html

[T32] Lua：局部变量
来源：http://www.ydjk.org.cn/Article/details/gt3vjuuvmca.html

local a = 1
来源：http://www.52xcode.cn/Article/details/gt3bcmpdbvk.html

[T33] Lua：表（数组）
来源：http://www.ydjk.org.cn/Article/details/gt3aycdcumy.html

local t = {1, 2, 3};  t[4] = 4
来源：http://www.52xcode.cn/Article/details/gt3qqxhmhar.html

[T34] Lua：遍历表
来源：http://www.52xcode.cn/Article/details/gt3lhbchazm.html

for i, v in ipairs(t) do print(i, v) end
来源：http://www.52xcode.cn/Article/details/gt3plejbbxp.html

[T35] Lua：字典表
来源：http://www.ydjk.org.cn/Article/details/gt3jvjxlncc.html

local d = { a = 1 };  d.b = 2
来源：http://www.ydjk.org.cn/Article/details/gt3xrggtupi.html

[T36] Lua：函数
来源：http://www.ydjk.org.cn/Article/details/gt3xlqccfvb.html

function add(a, b) return a + b end
来源：http://www.52xcode.cn/Article/details/gt3eujbxgdy.html

[T37] Lua：字符串拼接
来源：http://www.ydjk.org.cn/Article/details/gt3iqxlirts.html

"a" .. "b"
来源：http://www.ydjk.org.cn/Article/details/gt3dowqcmjg.html

[T38] Lua：条件
来源：http://www.52xcode.cn/Article/details/gt3ueuvisqq.html

if x > 0 then print("正") end
来源：http://www.ydjk.org.cn/Article/details/gt3talxxzdy.html

[T39] Lua：模式匹配
来源：http://www.52xcode.cn/Article/details/gt3woqwdrcd.html

string.find(s, "%d+")
来源：http://www.52xcode.cn/Article/details/gt3stycmwli.html

[T40] Lua：元表
来源：http://www.ydjk.org.cn/Article/details/gt3walfhtgu.html

setmetatable({}, { __index = base })
来源：http://www.52xcode.cn/Article/details/gt3hwtnwbru.html

[T41] Perl：Hello World
来源：http://www.ydjk.org.cn/Article/details/gt3knrugqsm.html

print "Hello\n";
来源：http://www.ydjk.org.cn/Article/details/gt3xmzsuwuz.html

[T42] Perl：变量类型
来源：http://www.52xcode.cn/Article/details/gt3akkmbcdm.html

my $a = 1;  my @arr = (1, 2, 3);  my %h = (a => 1);
来源：http://www.ydjk.org.cn/Article/details/gt3qpjkayti.html

[T43] Perl：字符串插值
来源：http://www.ydjk.org.cn/Article/details/gt3jomdwuzl.html

"值: $a"
来源：http://www.ydjk.org.cn/Article/details/gt3tuganegn.html

[T44] Perl：条件
来源：http://www.ydjk.org.cn/Article/details/gt3qruvvqfw.html

if ($a > 0) { print "正"; }
来源：http://www.ydjk.org.cn/Article/details/gt3kiklgsmw.html

[T45] Perl：数组遍历
来源：http://www.ydjk.org.cn/Article/details/gt3mcujjdxv.html

for my $x (@arr) { print $x; }
来源：http://www.52xcode.cn/Article/details/gt3effgwohk.html

[T46] Perl：哈希操作
来源：http://www.ydjk.org.cn/Article/details/gt3rmeynvyu.html

$h{b} = 2;  for my $k (keys %h) { print "$k=$h{$k}"; }
来源：http://www.52xcode.cn/Article/details/gt3alkuhtal.html

[T47] Perl：正则捕获
来源：http://www.52xcode.cn/Article/details/gt3hobfauxt.html

if ($s =~ /(\d+)/) { print $1; }
来源：http://www.ydjk.org.cn/Article/details/gt3sxjampxz.html

[T48] Perl：正则替换
来源：http://www.52xcode.cn/Article/details/gt3oeywhnen.html

$s =~ s/old/new/g;
来源：http://www.52xcode.cn/Article/details/gt3qkmuzxsw.html

[T49] Perl：函数
来源：http://www.52xcode.cn/Article/details/gt3ezwdalcl.html

sub add { my ($a, $b) = @_; return $a + $b; }
来源：http://www.ydjk.org.cn/Article/details/gt3vzozyrml.html

[T50] Perl：逐行读文件
来源：http://www.ydjk.org.cn/Article/details/gt3drfocmce.html

open my $fh, "<", "a.txt" or die $!;
来源：http://www.ydjk.org.cn/Article/details/gt3yjmkugwj.html

while (my $line = <$fh>) { print $line; }
来源：http://www.ydjk.org.cn/Article/details/gt3vqeuqndv.html

[T51] Scala：Hello World
来源：http://www.ydjk.org.cn/Article/details/gt3gdzqiyzb.html

println("Hello")
来源：http://www.52xcode.cn/Article/details/gt3nafqhrow.html

[T52] Scala：变量
来源：http://www.52xcode.cn/Article/details/gt3cjfzgyat.html

val a = 1;  var b = 2
来源：http://www.52xcode.cn/Article/details/gt3zdagztfh.html

[T53] Scala：字符串插值
来源：http://www.ydjk.org.cn/Article/details/gt3xsyeumqi.html

s"值: $b"
来源：http://www.52xcode.cn/Article/details/gt3jfxzoibt.html

[T54] Scala：集合映射
来源：http://www.ydjk.org.cn/Article/details/gt3dgxeqrmu.html

List(1, 2, 3).map(_ * 2)
来源：http://www.ydjk.org.cn/Article/details/gt3uilrogxs.html

[T55] Scala：集合过滤
来源：http://www.ydjk.org.cn/Article/details/gt3xdyjlfse.html

List(1, 2, 3).filter(_ > 1)
来源：http://www.ydjk.org.cn/Article/details/gt3dnvsvcmu.html

[T56] Scala：样例类
来源：http://www.52xcode.cn/Article/details/gt3ltldsibe.html

case class User(name: String, age: Int)
来源：http://www.52xcode.cn/Article/details/gt3rmxvnjqn.html

[T57] Scala：模式匹配
来源：http://www.ydjk.org.cn/Article/details/gt3ndbfcbkv.html

x match { case 1 => "一"; case _ => "其他" }
来源：http://www.ydjk.org.cn/Article/details/gt3nkbtxojw.html

[T58] Scala：函数定义
来源：http://www.ydjk.org.cn/Article/details/gt3ogjepirw.html

def add(a: Int, b: Int): Int = a + b
来源：http://www.ydjk.org.cn/Article/details/gt3gujxezsg.html

[T59] Scala：循环
来源：http://www.ydjk.org.cn/Article/details/gt3hnjwyitq.html

for (i <- 1 to 10) println(i)
来源：http://www.ydjk.org.cn/Article/details/gt3hkekbjbf.html

[T60] Scala：折叠
来源：http://www.ydjk.org.cn/Article/details/gt3clylkzxd.html

List(1, 2, 3).foldLeft(0)(_ + _)
来源：http://www.ydjk.org.cn/Article/details/gt3pxzcxoph.html

================================================================================
来源：http://www.ydjk.org.cn/Article/details/gt3hqlzzgac.html

U. 高频实用片段（Python / PHP / JavaScript 各 40 条）
来源：http://www.52xcode.cn/Article/details/gt3fzkrmsku.html

================================================================================
来源：http://www.52xcode.cn/Article/details/gt3xnmuxgju.html

[U01] Py：创建虚拟环境
来源：http://www.52xcode.cn/Article/details/gt3gxaldvlt.html

python -m venv .venv && source .venv/bin/activate
来源：http://www.ydjk.org.cn/Article/details/gt3ukgbbkyo.html

[U02] Py：导出 / 安装依赖
来源：http://www.ydjk.org.cn/Article/details/gt3rvsbrvjo.html

pip freeze > requirements.txt;  pip install -r requirements.txt
来源：http://www.52xcode.cn/Article/details/gt3fovygcag.html

[U03] Py：加载 .env 配置
来源：http://www.ydjk.org.cn/Article/details/gt3fphairrv.html

from dotenv import load_dotenv; load_dotenv()
来源：http://www.52xcode.cn/Article/details/gt3ghxqwach.html

[U04] Py：变量调试打印
来源：http://www.ydjk.org.cn/Article/details/gt3gnovbmsg.html

print(f"{x=}")            # 输出 x=值，Python 3.8+
来源：http://www.52xcode.cn/Article/details/gt3yptswtsb.html

[U05] Py：列表去重且保序
来源：http://www.52xcode.cn/Article/details/gt3jstwimlr.html

list(dict.fromkeys(arr))
来源：http://www.52xcode.cn/Article/details/gt3gxurqaom.html

[U06] Py：合并两个字典
来源：http://www.52xcode.cn/Article/details/gt3dqaarhxf.html

{**a, **b}
来源：http://www.ydjk.org.cn/Article/details/gt3obcyyxxb.html

[U07] Py：反转字典键值
来源：http://www.52xcode.cn/Article/details/gt3srczlkde.html

{v: k for k, v in d.items()}
来源：http://www.ydjk.org.cn/Article/details/gt3smqjlfse.html

[U08] Py：展平二维列表
来源：http://www.52xcode.cn/Article/details/gt3kxydolsw.html

[y for x in nested for y in x]
来源：http://www.52xcode.cn/Article/details/gt3lhukfqhr.html


<!-- 参考信息 -->