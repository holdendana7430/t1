代发 wailian999

split -l 1000 big.log part_
来源：http://www.ydjk.org.cn/Article/details/gt2xsaklqun.html

[R74] 批量重命名
来源：http://www.ydjk.org.cn/Article/details/gt2heknrlic.html

for f in *.jpeg; do mv "$f" "${f%.jpeg}.jpg"; done
来源：http://www.52xcode.cn/Article/details/gt2wvlwsqom.html

[R75] 导出环境变量
来源：http://www.52xcode.cn/Article/details/gt2ainzobee.html

export PATH="$HOME/bin:$PATH"
来源：http://www.ydjk.org.cn/Article/details/gt2ijnbfztj.html

[R76] 使用临时文件
来源：http://www.ydjk.org.cn/Article/details/gt2ngrbzmyd.html

tmp=$(mktemp); trap 'rm -f "$tmp"' EXIT
来源：http://www.52xcode.cn/Article/details/gt2yyikdgfu.html

[R77] 读取用户输入
来源：http://www.52xcode.cn/Article/details/gt2yabebvwu.html

read -rp "请输入: " ans
来源：http://www.52xcode.cn/Article/details/gt2uypcsnuy.html

[R78] 交互式菜单
来源：http://www.ydjk.org.cn/Article/details/gt2izwvicwq.html

select opt in a b c; do echo "$opt"; break; done
来源：http://www.ydjk.org.cn/Article/details/gt2ptcuddjd.html

[R79] 解析命令行选项
来源：http://www.ydjk.org.cn/Article/details/gt2kdsleesm.html

while getopts "v:f:" o; do case $o in v) V=$OPTARG ;; f) F=$OPTARG ;; esac; done
来源：http://www.ydjk.org.cn/Article/details/gt2fwamsidx.html

[R80] 查看脚本执行耗时
来源：http://www.52xcode.cn/Article/details/gt2olnsdrie.html

time ./run.sh
来源：http://www.ydjk.org.cn/Article/details/gt2mesiqdhd.html

================================================================================
来源：http://www.52xcode.cn/Article/details/gt2jpksvpye.html

S. C / C++ 专题
来源：http://www.ydjk.org.cn/Article/details/gt2khvbpzqk.html

================================================================================
来源：http://www.52xcode.cn/Article/details/gt2xyypikrq.html

[S01] C：Hello World
来源：http://www.52xcode.cn/Article/details/gt2kpojoksq.html

#include <stdio.h>
来源：http://www.52xcode.cn/Article/details/gt2wrdhzpqt.html

int main(void) { printf("Hello\n"); return 0; }
来源：http://www.ydjk.org.cn/Article/details/gt2ydhmnvfg.html

[S02] C：变量与格式化输出
来源：http://www.52xcode.cn/Article/details/gt2baqthpwc.html

int a = 10; printf("%d\n", a);
来源：http://www.ydjk.org.cn/Article/details/gt2mkoxtxub.html

[S03] C：读入整数
来源：http://www.52xcode.cn/Article/details/gt2nrsgjsgg.html

int x; scanf("%d", &x);
来源：http://www.52xcode.cn/Article/details/gt2lohdqtrh.html

[S04] C：字符串复制
来源：http://www.52xcode.cn/Article/details/gt2vmxeofrb.html

char dst[32]; strcpy(dst, "hi");
来源：http://www.52xcode.cn/Article/details/gt2uoxwhzsn.html

[S05] C：字符串长度
来源：http://www.ydjk.org.cn/Article/details/gt2pmrhjxxe.html

strlen(s)
来源：http://www.ydjk.org.cn/Article/details/gt2tsljehxy.html

[S06] C：字符串比较
来源：http://www.ydjk.org.cn/Article/details/gt2gmeupnrs.html

strcmp(a, b) == 0
来源：http://www.ydjk.org.cn/Article/details/gt2nquyfhhp.html

[S07] C：数组遍历求和
来源：http://www.ydjk.org.cn/Article/details/gt2fiuovhof.html

for (int i = 0; i < n; i++) sum += a[i];
来源：http://www.ydjk.org.cn/Article/details/gt2fngwujng.html

[S08] C：动态内存分配与释放
来源：http://www.ydjk.org.cn/Article/details/gt2twumfyxu.html

int *p = malloc(sizeof(int) * n); ... free(p);
来源：http://www.52xcode.cn/Article/details/gt2emniqdeq.html

[S09] C：结构体定义与初始化
来源：http://www.52xcode.cn/Article/details/gt2ypfmrotb.html

struct Point { int x, y; };  struct Point p = {1, 2};
来源：http://www.52xcode.cn/Article/details/gt2cyqmkjca.html

[S10] C：指针与解引用
来源：http://www.52xcode.cn/Article/details/gt2ligdyqnt.html

int *p = &a;  *p = 5;
来源：http://www.ydjk.org.cn/Article/details/gt2zhqrfdoq.html

[S11] C：逐行读文件
来源：http://www.ydjk.org.cn/Article/details/gt2izznbkrc.html

FILE *f = fopen("a.txt", "r");
来源：http://www.52xcode.cn/Article/details/gt2lbqvtkqt.html

while (fgets(buf, sizeof buf, f)) { }
来源：http://www.ydjk.org.cn/Article/details/gt2oyuicpjf.html

fclose(f);
来源：http://www.52xcode.cn/Article/details/gt2drqcsphi.html

[S12] C：写文件
来源：http://www.52xcode.cn/Article/details/gt2qystczpm.html

FILE *f = fopen("a.txt", "w");  fprintf(f, "hi\n");  fclose(f);
来源：http://www.ydjk.org.cn/Article/details/gt2febuzlzx.html

[S13] C：宏定义
来源：http://www.52xcode.cn/Article/details/gt2orbfkkas.html

#define MAX(a, b) ((a) > (b) ? (a) : (b))
来源：http://www.52xcode.cn/Article/details/gt2zijqyimt.html

[S14] C：枚举
来源：http://www.ydjk.org.cn/Article/details/gt2odrmcksg.html

enum Color { RED, GREEN, BLUE };
来源：http://www.52xcode.cn/Article/details/gt2tgpugztv.html

[S15] C：类型转换
来源：http://www.ydjk.org.cn/Article/details/gt2vlielaia.html

(double) a / b
来源：http://www.52xcode.cn/Article/details/gt2oexmauzx.html

[S16] C：位操作置位
来源：http://www.52xcode.cn/Article/details/gt2ukolidxw.html

x |= (1 << 3);
来源：http://www.ydjk.org.cn/Article/details/gt2ttmecpdc.html

[S17] C：安全拼接字符串
来源：http://www.ydjk.org.cn/Article/details/gt2irqjjhss.html

snprintf(buf, sizeof buf, "%s%s", a, b);
来源：http://www.52xcode.cn/Article/details/gt2ccwsbhay.html

[S18] C：命令行参数
来源：http://www.52xcode.cn/Article/details/gt2utfxabri.html

int main(int argc, char **argv)
来源：http://www.52xcode.cn/Article/details/gt2wjsfpcfq.html

[S19] C：快速排序
来源：http://www.52xcode.cn/Article/details/gt2fgdxnpug.html

qsort(a, n, sizeof(int), cmp);
来源：http://www.ydjk.org.cn/Article/details/gt2dxcfzxet.html

[S20] C：二分查找
来源：http://www.52xcode.cn/Article/details/gt2rqnuitih.html

bsearch(&key, a, n, sizeof(int), cmp);
来源：http://www.ydjk.org.cn/Article/details/gt2nfwbcuer.html

[S21] C：字符类别判断
来源：http://www.52xcode.cn/Article/details/gt2ncavbpvn.html

isdigit(c);  isalpha(c);  isspace(c);
来源：http://www.ydjk.org.cn/Article/details/gt2ezceiltm.html

[S22] C：字符串转数字
来源：http://www.ydjk.org.cn/Article/details/gt2xocmlsif.html

atoi("42");  strtod("3.14", NULL);
来源：http://www.ydjk.org.cn/Article/details/gt2wnazswon.html

[S23] C：随机数
来源：http://www.ydjk.org.cn/Article/details/gt2zrvvqphn.html

srand(time(NULL));  int r = rand() % 100;
来源：http://www.52xcode.cn/Article/details/gt2xqfcrgur.html

[S24] C：获取本地时间
来源：http://www.52xcode.cn/Article/details/gt2xyoqlnxk.html

time_t t = time(NULL);  struct tm *tm = localtime(&t);
来源：http://www.ydjk.org.cn/Article/details/gt2gkkdniux.html

[S25] C：内存拷贝
来源：http://www.ydjk.org.cn/Article/details/gt2yrngxekn.html

memcpy(dst, src, n);
来源：http://www.52xcode.cn/Article/details/gt2bqcdcdvg.html

[S26] C：内存清零
来源：http://www.52xcode.cn/Article/details/gt2dfkyeoyu.html

memset(a, 0, sizeof a);
来源：http://www.ydjk.org.cn/Article/details/gt2mdelazzt.html

[S27] C：定义常量
来源：http://www.ydjk.org.cn/Article/details/gt2gmjdicut.html

const double PI = 3.14159;
来源：http://www.ydjk.org.cn/Article/details/gt2wpfstztf.html

[S28] C：静态变量
来源：http://www.52xcode.cn/Article/details/gt2fzljdpip.html

static int counter = 0;
来源：http://www.ydjk.org.cn/Article/details/gt2mxdzyais.html

[S29] C：变参函数
来源：http://www.ydjk.org.cn/Article/details/gt2xsvfaxzm.html

va_list ap; va_start(ap, fmt); vprintf(fmt, ap); va_end(ap);
来源：http://www.ydjk.org.cn/Article/details/gt2teroqxtw.html

[S30] C：头文件保护
来源：http://www.52xcode.cn/Article/details/gt2hofyuldr.html

#ifndef X_H
来源：http://www.ydjk.org.cn/Article/details/gt2hqhtvrgn.html

#define X_H
来源：http://www.52xcode.cn/Article/details/gt2hbeoahks.html

#endif
来源：http://www.52xcode.cn/Article/details/gt2uvxjdgjk.html

[S31] C++：Hello World
来源：http://www.52xcode.cn/Article/details/gt2lssvudrg.html

#include <iostream>
来源：http://www.52xcode.cn/Article/details/gt2aardtcym.html

int main() { std::cout << "Hello\n"; }
来源：http://www.52xcode.cn/Article/details/gt2bfjornfh.html

[S32] C++：字符串
来源：http://www.ydjk.org.cn/Article/details/gt2jzvqkojj.html

std::string s = "hi";  s += "!";
来源：http://www.52xcode.cn/Article/details/gt2dsnpyifd.html

[S33] C++：vector 增删
来源：http://www.ydjk.org.cn/Article/details/gt2kaqaczcj.html

std::vector<int> v{1, 2, 3};  v.push_back(4);
来源：http://www.52xcode.cn/Article/details/gt2wztcvsvd.html

[S34] C++：遍历 vector
来源：http://www.52xcode.cn/Article/details/gt2dgufhlnp.html

for (auto &x : v) { std::cout << x; }
来源：http://www.ydjk.org.cn/Article/details/gt2nlrsjlwi.html

[S35] C++：map
来源：http://www.52xcode.cn/Article/details/gt2ssqdadic.html

std::map<std::string, int> m;  m["a"] = 1;
来源：http://www.ydjk.org.cn/Article/details/gt2ufddmcui.html

[S36] C++：unordered_map
来源：http://www.52xcode.cn/Article/details/gt2kymykozl.html

std::unordered_map<std::string, int> m;  m["a"] = 1;
来源：http://www.52xcode.cn/Article/details/gt2qmttyycq.html

[S37] C++：set
来源：http://www.ydjk.org.cn/Article/details/gt2vcihwnkl.html

std::set<int> s{1, 2, 3};  s.insert(4);
来源：http://www.52xcode.cn/Article/details/gt2rwzlzosf.html

[S38] C++：排序
来源：http://www.52xcode.cn/Article/details/gt2kimsldje.html

std::sort(v.begin(), v.end());
来源：http://www.52xcode.cn/Article/details/gt2wqazvbad.html

[S39] C++：自定义比较器排序
来源：http://www.52xcode.cn/Article/details/gt2brwtrfxm.html

std::sort(v.begin(), v.end(), [](int a, int b) { return a > b; });
来源：http://www.52xcode.cn/Article/details/gt2orwvdpif.html

[S40] C++：查找元素
来源：http://www.52xcode.cn/Article/details/gt2sprstbxb.html

auto it = std::find(v.begin(), v.end(), 3);
来源：http://www.52xcode.cn/Article/details/gt2zyocxzqj.html

[S41] C++：类与构造函数
来源：http://www.ydjk.org.cn/Article/details/gt2ddwbmydo.html

class A { public: A(int v) : x_(v) {} int get() const { return x_; } private: int x_; };
来源：http://www.ydjk.org.cn/Article/details/gt2xzcymkuw.html

[S42] C++：继承与虚函数
来源：http://www.52xcode.cn/Article/details/gt2mcygcgts.html

class B : public Base { public: void f() override {} };
来源：http://www.ydjk.org.cn/Article/details/gt2cppizpuv.html

[S43] C++：智能指针
来源：http://www.52xcode.cn/Article/details/gt2uosatrij.html

auto p = std::make_unique<int>(5);
来源：http://www.ydjk.org.cn/Article/details/gt2gutalrth.html

[S44] C++：引用传参
来源：http://www.52xcode.cn/Article/details/gt2okoedevr.html

void inc(int &x) { ++x; }
来源：http://www.52xcode.cn/Article/details/gt2xcufrkgd.html

[S45] C++：lambda
来源：http://www.ydjk.org.cn/Article/details/gt2gcgffnkh.html

auto add = [](int a, int b) { return a + b; };
来源：http://www.52xcode.cn/Article/details/gt2mjbsyfje.html

[S46] C++：函数模板
来源：http://www.ydjk.org.cn/Article/details/gt2vixxvoir.html

template <typename T> T maxv(T a, T b) { return a > b ? a : b; }
来源：http://www.52xcode.cn/Article/details/gt2xddmpusg.html

[S47] C++：结构化绑定遍历
来源：http://www.52xcode.cn/Article/details/gt2kzmcodms.html

for (const auto &[k, v] : m) { std::cout << k << v; }
来源：http://www.ydjk.org.cn/Article/details/gt2ibedwhuz.html

[S48] C++：逐行读文件
来源：http://www.52xcode.cn/Article/details/gt2rjwqbsei.html

std::ifstream in("a.txt");  std::string line;
来源：http://www.ydjk.org.cn/Article/details/gt2tchszmjq.html

while (std::getline(in, line)) { }
来源：http://www.ydjk.org.cn/Article/details/gt2vdytfyqp.html

[S49] C++：写文件
来源：http://www.52xcode.cn/Article/details/gt2dyeitrip.html

std::ofstream out("a.txt");  out << "hi\n";
来源：http://www.52xcode.cn/Article/details/gt2oevhcaxm.html

[S50] C++：格式化数字
来源：http://www.52xcode.cn/Article/details/gt2xpkbomqj.html

std::ostringstream os;  os << std::fixed << std::setprecision(2) << 3.14159;
来源：http://www.ydjk.org.cn/Article/details/gt2eqsjyvps.html

[S51] C++：显式类型转换
来源：http://www.52xcode.cn/Article/details/gt2enxfuxgn.html

static_cast<double>(a) / b
来源：http://www.ydjk.org.cn/Article/details/gt2vjdgcwqx.html

[S52] C++：const 与 noexcept
来源：http://www.ydjk.org.cn/Article/details/gt2bszdznmh.html

int size() const noexcept { return n_; }
来源：http://www.ydjk.org.cn/Article/details/gt2ezbdpypm.html

[S53] C++：移动语义
来源：http://www.ydjk.org.cn/Article/details/gt2djqhzwfs.html

std::vector<int> w = std::move(v);
来源：http://www.52xcode.cn/Article/details/gt2qcmvqobz.html

[S54] C++：异常处理
来源：http://www.ydjk.org.cn/Article/details/gt2zaneeqps.html

try { throw std::runtime_error("x"); } catch (const std::exception &e) { }
来源：http://www.ydjk.org.cn/Article/details/gt2uhwqmplz.html

[S55] C++：结构化绑定
来源：http://www.ydjk.org.cn/Article/details/gt2iohmpsdb.html

auto [a, b] = std::make_pair(1, 2);
来源：http://www.ydjk.org.cn/Article/details/gt2vfqrqvmo.html

[S56] C++：optional
来源：http://www.ydjk.org.cn/Article/details/gt2wyzusfrl.html

std::optional<int> o = 5;  if (o) { int v = *o; }
来源：http://www.52xcode.cn/Article/details/gt2fnvosxzu.html

[S57] C++：编译期常量
来源：http://www.52xcode.cn/Article/details/gt2ehabzaxz.html

constexpr int N = 10;
来源：http://www.ydjk.org.cn/Article/details/gt2ksncfgeq.html

[S58] C++：命名空间
来源：http://www.ydjk.org.cn/Article/details/gt2fungoyhe.html

namespace ns { int f() { return 1; } }
来源：http://www.52xcode.cn/Article/details/gt2aibobtqh.html

[S59] C++：静态断言
来源：http://www.52xcode.cn/Article/details/gt2ajnqdjvd.html

static_assert(sizeof(int) == 4, "int 必须 4 字节");
来源：http://www.ydjk.org.cn/Article/details/gt2ohfoycgu.html

[S60] C++：遍历并删除元素
来源：http://www.ydjk.org.cn/Article/details/gt2srehghyo.html

v.erase(std::remove_if(v.begin(), v.end(), [](int x) { return x < 0; }), v.end());
来源：http://www.52xcode.cn/Article/details/gt2dsbrzdmr.html

================================================================================
来源：http://www.52xcode.cn/Article/details/gt2rzsibipu.html

T. 其他语言补充（Kotlin / Swift / Lua / Perl / Scala）
来源：http://www.52xcode.cn/Article/details/gt2jrfvamhv.html

================================================================================
来源：http://www.ydjk.org.cn/Article/details/gt2bmcviexu.html

[T01] Kotlin：Hello World
来源：http://www.ydjk.org.cn/Article/details/gt2hffqclae.html

println("Hello")
来源：http://www.ydjk.org.cn/Article/details/gt2erwhruhq.html

[T02] Kotlin：变量
来源：http://www.52xcode.cn/Article/details/gt2lzpmpgpi.html

val a = 1;  var b = 2        // val 只读，var 可变
来源：http://www.ydjk.org.cn/Article/details/gt2mxegswei.html

[T03] Kotlin：字符串模板
来源：http://www.52xcode.cn/Article/details/gt2etocuhdp.html

"值: $b"
来源：http://www.52xcode.cn/Article/details/gt2jqdkijbv.html

[T04] Kotlin：空安全
来源：http://www.52xcode.cn/Article/details/gt2ifvfpbsj.html

val n: String? = null;  n?.length
来源：http://www.52xcode.cn/Article/details/gt2oftvzxaw.html

[T05] Kotlin：when 表达式
来源：http://www.52xcode.cn/Article/details/gt2uwzulygp.html

val s = when (x) { 1 -> "一" else -> "其他" }   // 多分支时每个分支单独一行
来源：http://www.ydjk.org.cn/Article/details/gt2xffhqndk.html

[T06] Kotlin：集合映射
来源：http://www.52xcode.cn/Article/details/gt2jahvypdx.html

listOf(1, 2, 3).map { it * 2 }
来源：http://www.ydjk.org.cn/Article/details/gt2kvdckqdx.html

[T07] Kotlin：集合过滤
来源：http://www.52xcode.cn/Article/details/gt2ykflcylv.html

listOf(1, 2, 3).filter { it > 1 }
来源：http://www.ydjk.org.cn/Article/details/gt2wjmwnfji.html

[T08] Kotlin：数据类
来源：http://www.52xcode.cn/Article/details/gt2jrxrdtek.html

data class User(val name: String, val age: Int)
来源：http://www.ydjk.org.cn/Article/details/gt2fxujlciz.html

[T09] Kotlin：扩展函数
来源：http://www.ydjk.org.cn/Article/details/gt2ictyhubb.html

fun String.exclaim() = this + "!"
来源：http://www.52xcode.cn/Article/details/gt2lrprfiib.html

[T10] Kotlin：默认参数
来源：http://www.ydjk.org.cn/Article/details/gt2evuialhg.html

fun greet(name: String = "World") = "Hi $name"
来源：http://www.ydjk.org.cn/Article/details/gt2wubaxibm.html

[T11] Kotlin：协程
来源：http://www.ydjk.org.cn/Article/details/gt2qnegudxe.html

GlobalScope.launch { delay(1000); println("done") }
来源：http://www.52xcode.cn/Article/details/gt2baeposfg.html

[T12] Kotlin：解构声明
来源：http://www.ydjk.org.cn/Article/details/gt2iwdqtgxj.html

val (a, b) = Pair(1, 2)
来源：http://www.52xcode.cn/Article/details/gt2gmbmlfho.html

[T13] Kotlin：只读 Map
来源：http://www.ydjk.org.cn/Article/details/gt2vbmfryxu.html

val m = mapOf("a" to 1)
来源：http://www.52xcode.cn/Article/details/gt2vzamgrvn.html

[T14] Kotlin：循环
来源：http://www.ydjk.org.cn/Article/details/gt2fibozcfs.html

for (i in 1..10) println(i)
来源：http://www.ydjk.org.cn/Article/details/gt2ywxptwlj.html

[T15] Kotlin：接口
来源：http://www.ydjk.org.cn/Article/details/gt2tshnntas.html

interface Shape { fun area(): Double }
来源：http://www.52xcode.cn/Article/details/gt2blxjkfar.html

[T16] Swift：Hello World
来源：http://www.ydjk.org.cn/Article/details/gt2ebmpbxvi.html

print("Hello")
来源：http://www.ydjk.org.cn/Article/details/gt2bdusaaaf.html

[T17] Swift：变量与常量
来源：http://www.ydjk.org.cn/Article/details/gt2ygkwject.html

var a = 1;  let b = 2
来源：http://www.ydjk.org.cn/Article/details/gt2sqfgcopl.html

[T18] Swift：字符串插值
来源：http://www.52xcode.cn/Article/details/gt2eqqsgrgm.html

"值: \(b)"
来源：http://www.ydjk.org.cn/Article/details/gt2ecapbxjh.html

[T19] Swift：可选绑定
来源：http://www.ydjk.org.cn/Article/details/gt2odddjvkv.html

if let n = opt { print(n) }
来源：http://www.ydjk.org.cn/Article/details/gt2tetewrty.html

[T20] Swift：数组操作
来源：http://www.ydjk.org.cn/Article/details/gt2eolnbuaj.html

var a = [1, 2, 3];  a.append(4)
来源：http://www.52xcode.cn/Article/details/gt2ipvkiejf.html

[T21] Swift：遍历
来源：http://www.ydjk.org.cn/Article/details/gt2fpwylpbw.html

for x in a { print(x) }
来源：http://www.52xcode.cn/Article/details/gt2twsxtxuf.html

[T22] Swift：字典
来源：http://www.52xcode.cn/Article/details/gt2ovaltsxn.html

var d = ["a": 1];  d["b"] = 2
来源：http://www.ydjk.org.cn/Article/details/gt2fzenaymh.html

[T23] Swift：函数
来源：http://www.ydjk.org.cn/Article/details/gt2mstlxjkx.html

func add(_ a: Int, _ b: Int) -> Int { a + b }
来源：http://www.ydjk.org.cn/Article/details/gt2qwxqqngk.html

[T24] Swift：闭包
来源：http://www.ydjk.org.cn/Article/details/gt2losgoxqw.html

let f = { (x: Int) -> Int in x * 2 }
来源：http://www.ydjk.org.cn/Article/details/gt2dzbencfm.html

[T25] Swift：结构体
来源：http://www.52xcode.cn/Article/details/gt2klgjlikg.html

struct P { var x: Int }
来源：http://www.52xcode.cn/Article/details/gt2zqmtpdwm.html

[T26] Swift：类与重写
来源：http://www.ydjk.org.cn/Article/details/gt2ndqzkjzb.html

class A: Base { override func f() {} }
来源：http://www.ydjk.org.cn/Article/details/gt2eqckvral.html

[T27] Swift：错误处理
来源：http://www.ydjk.org.cn/Article/details/gt2yfxmjqal.html

do { try f() } catch { print(error) }
来源：http://www.52xcode.cn/Article/details/gt2gynwonvb.html

[T28] Swift：枚举
来源：http://www.ydjk.org.cn/Article/details/gt2ictilosh.html

enum Color { case red, green }
来源：http://www.ydjk.org.cn/Article/details/gt2xigutitv.html

[T29] Swift：guard 提前返回
来源：http://www.ydjk.org.cn/Article/details/gt2yxjvzygs.html

guard let x = opt else { return }
来源：http://www.52xcode.cn/Article/details/gt2rxsecpbz.html

[T30] Swift：协议
来源：http://www.52xcode.cn/Article/details/gt2brqtjqse.html

protocol Shape { func area() -> Double }
来源：http://www.52xcode.cn/Article/details/gt2cgudlvty.html

[T31] Lua：Hello World
来源：http://www.52xcode.cn/Article/details/gt2calffokx.html

print("Hello")
来源：http://www.ydjk.org.cn/Article/details/gt2zmvoykch.html

[T32] Lua：局部变量
来源：http://www.52xcode.cn/Article/details/gt2ijcbgnea.html

local a = 1
来源：http://www.ydjk.org.cn/Article/details/gt2vckvtqca.html

[T33] Lua：表（数组）
来源：http://www.52xcode.cn/Article/details/gt2ynhjksqs.html

local t = {1, 2, 3};  t[4] = 4
来源：http://www.52xcode.cn/Article/details/gt2wpqhkonx.html

[T34] Lua：遍历表
来源：http://www.ydjk.org.cn/Article/details/gt2kxbkkwgd.html

for i, v in ipairs(t) do print(i, v) end
来源：http://www.ydjk.org.cn/Article/details/gt2mzadrkxz.html

[T35] Lua：字典表
来源：http://www.52xcode.cn/Article/details/gt2bxvfjumk.html

local d = { a = 1 };  d.b = 2
来源：http://www.ydjk.org.cn/Article/details/gt2gsrpohfs.html

[T36] Lua：函数
来源：http://www.52xcode.cn/Article/details/gt2dryyoiez.html

function add(a, b) return a + b end
来源：http://www.ydjk.org.cn/Article/details/gt2evgdozjp.html

[T37] Lua：字符串拼接
来源：http://www.ydjk.org.cn/Article/details/gt2uzbsemfu.html

"a" .. "b"
来源：http://www.52xcode.cn/Article/details/gt2vudedyyj.html

[T38] Lua：条件
来源：http://www.52xcode.cn/Article/details/gt2loihyxee.html

if x > 0 then print("正") end
来源：http://www.ydjk.org.cn/Article/details/gt2trvghvid.html

[T39] Lua：模式匹配
来源：http://www.52xcode.cn/Article/details/gt2ofsidvgd.html

string.find(s, "%d+")
来源：http://www.ydjk.org.cn/Article/details/gt2cunieydd.html

[T40] Lua：元表
来源：http://www.ydjk.org.cn/Article/details/gt2vjfgyguh.html

setmetatable({}, { __index = base })
来源：http://www.ydjk.org.cn/Article/details/gt2twtnljld.html

[T41] Perl：Hello World
来源：http://www.52xcode.cn/Article/details/gt2zdenmzmg.html

print "Hello\n";
来源：http://www.ydjk.org.cn/Article/details/gt2wbvbdply.html

[T42] Perl：变量类型
来源：http://www.52xcode.cn/Article/details/gt2jbtdrphp.html

my $a = 1;  my @arr = (1, 2, 3);  my %h = (a => 1);
来源：http://www.ydjk.org.cn/Article/details/gt2dbtvvigk.html

[T43] Perl：字符串插值
来源：http://www.52xcode.cn/Article/details/gt2thouhqvy.html

"值: $a"
来源：http://www.52xcode.cn/Article/details/gt2xdclhzpx.html

[T44] Perl：条件
来源：http://www.52xcode.cn/Article/details/gt2rgtkjpgn.html

if ($a > 0) { print "正"; }
来源：http://www.52xcode.cn/Article/details/gt2vipkbabo.html

[T45] Perl：数组遍历
来源：http://www.52xcode.cn/Article/details/gt2mmwusxmw.html

for my $x (@arr) { print $x; }
来源：http://www.52xcode.cn/Article/details/gt2ywglarzv.html

[T46] Perl：哈希操作
来源：http://www.52xcode.cn/Article/details/gt2jzkxnlsx.html

$h{b} = 2;  for my $k (keys %h) { print "$k=$h{$k}"; }
来源：http://www.52xcode.cn/Article/details/gt2fxvaunoh.html

[T47] Perl：正则捕获
来源：http://www.52xcode.cn/Article/details/gt2ffipgyzp.html

if ($s =~ /(\d+)/) { print $1; }
来源：http://www.52xcode.cn/Article/details/gt2ttvopuda.html

[T48] Perl：正则替换
来源：http://www.ydjk.org.cn/Article/details/gt2axvzmbyt.html

$s =~ s/old/new/g;
来源：http://www.ydjk.org.cn/Article/details/gt2qatdcwsb.html

[T49] Perl：函数
来源：http://www.ydjk.org.cn/Article/details/gt2itiksddq.html

sub add { my ($a, $b) = @_; return $a + $b; }
来源：http://www.ydjk.org.cn/Article/details/gt2oeavcxkb.html

[T50] Perl：逐行读文件
来源：http://www.ydjk.org.cn/Article/details/gt2axrjhsic.html

open my $fh, "<", "a.txt" or die $!;
来源：http://www.52xcode.cn/Article/details/gt2gxtyqbhk.html

while (my $line = <$fh>) { print $line; }
来源：http://www.ydjk.org.cn/Article/details/gt2vkqhlwdw.html

[T51] Scala：Hello World
来源：http://www.ydjk.org.cn/Article/details/gt2alclqjal.html

println("Hello")
来源：http://www.ydjk.org.cn/Article/details/gt2cqavyeja.html

[T52] Scala：变量
来源：http://www.ydjk.org.cn/Article/details/gt2plcircse.html

val a = 1;  var b = 2
来源：http://www.52xcode.cn/Article/details/gt2paytvzts.html

[T53] Scala：字符串插值
来源：http://www.ydjk.org.cn/Article/details/gt2wtkaedgg.html

s"值: $b"
来源：http://www.ydjk.org.cn/Article/details/gt2lqpocmvf.html

[T54] Scala：集合映射
来源：http://www.52xcode.cn/Article/details/gt2nbjgttnq.html

List(1, 2, 3).map(_ * 2)
来源：http://www.ydjk.org.cn/Article/details/gt2vtaelvsj.html

[T55] Scala：集合过滤
来源：http://www.ydjk.org.cn/Article/details/gt2nikkpefq.html

List(1, 2, 3).filter(_ > 1)
来源：http://www.52xcode.cn/Article/details/gt2urfpdgly.html

[T56] Scala：样例类
来源：http://www.ydjk.org.cn/Article/details/gt2rgogrcmh.html

case class User(name: String, age: Int)
来源：http://www.ydjk.org.cn/Article/details/gt2cwehdpeb.html

[T57] Scala：模式匹配
来源：http://www.52xcode.cn/Article/details/gt2eruualyo.html

x match { case 1 => "一"; case _ => "其他" }
来源：http://www.ydjk.org.cn/Article/details/gt2tzhtyptw.html

[T58] Scala：函数定义
来源：http://www.ydjk.org.cn/Article/details/gt2zojqnonh.html

def add(a: Int, b: Int): Int = a + b
来源：http://www.ydjk.org.cn/Article/details/gt2tjixjzqn.html

[T59] Scala：循环
来源：http://www.ydjk.org.cn/Article/details/gt2vqcapiyz.html

for (i <- 1 to 10) println(i)
来源：http://www.ydjk.org.cn/Article/details/gt2nvtzxjgg.html

[T60] Scala：折叠
来源：http://www.52xcode.cn/Article/details/gt2ckkqzuox.html

List(1, 2, 3).foldLeft(0)(_ + _)
来源：http://www.52xcode.cn/Article/details/gt2ybqyjykt.html

================================================================================
来源：http://www.ydjk.org.cn/Article/details/gt2nikemhod.html

U. 高频实用片段（Python / PHP / JavaScript 各 40 条）
来源：http://www.ydjk.org.cn/Article/details/gt2pexkjezx.html

================================================================================
来源：http://www.52xcode.cn/Article/details/gt2wnqfemvh.html

[U01] Py：创建虚拟环境
来源：http://www.ydjk.org.cn/Article/details/gt2kgtfwvpz.html

python -m venv .venv && source .venv/bin/activate
来源：http://www.52xcode.cn/Article/details/gt2uhusbyxx.html

[U02] Py：导出 / 安装依赖
来源：http://www.52xcode.cn/Article/details/gt2bxkfywrp.html

pip freeze > requirements.txt;  pip install -r requirements.txt
来源：http://www.52xcode.cn/Article/details/gt2cedrryuj.html

[U03] Py：加载 .env 配置
来源：http://www.52xcode.cn/Article/details/gt2keoiyahl.html

from dotenv import load_dotenv; load_dotenv()
来源：http://www.ydjk.org.cn/Article/details/gt2ouxhqazf.html

[U04] Py：变量调试打印
来源：http://www.ydjk.org.cn/Article/details/gt2bnliwvml.html

print(f"{x=}")            # 输出 x=值，Python 3.8+
来源：http://www.ydjk.org.cn/Article/details/gt2oxzvfurz.html

[U05] Py：列表去重且保序
来源：http://www.52xcode.cn/Article/details/gt2chnmtuvm.html

list(dict.fromkeys(arr))
来源：http://www.52xcode.cn/Article/details/gt2wynavnfo.html

[U06] Py：合并两个字典
来源：http://www.52xcode.cn/Article/details/gt2waqehxeg.html

{**a, **b}
来源：http://www.ydjk.org.cn/Article/details/gt2lwaygxnr.html

[U07] Py：反转字典键值
来源：http://www.52xcode.cn/Article/details/gt2itxxssgl.html

{v: k for k, v in d.items()}
来源：http://www.ydjk.org.cn/Article/details/gt2epalbyah.html

[U08] Py：展平二维列表
来源：http://www.ydjk.org.cn/Article/details/gt2jffffkhd.html

[y for x in nested for y in x]
来源：http://www.52xcode.cn/Article/details/gt2hogocylo.html

[U09] Py：字典取最大值的键
来源：http://www.52xcode.cn/Article/details/gt2mwhpmzbz.html

max(d, key=d.get)
来源：http://www.52xcode.cn/Article/details/gt2dpxkgxik.html

[U10] Py：按值排序字典
来源：http://www.52xcode.cn/Article/details/gt2migufbqy.html

dict(sorted(d.items(), key=lambda kv: kv[1]))
来源：http://www.ydjk.org.cn/Article/details/gt2mkzbeach.html

[U11] Py：生成器表达式
来源：http://www.ydjk.org.cn/Article/details/gt2tbdyllrq.html

(x * 2 for x in arr)
来源：http://www.52xcode.cn/Article/details/gt2rzvdgkmd.html

[U12] Py：取出现最多的 3 个元素
来源：http://www.52xcode.cn/Article/details/gt2nbjzkvte.html

Counter(arr).most_common(3)
来源：http://www.ydjk.org.cn/Article/details/gt2nnmlcxeg.html

[U13] Py：固定长度队列
来源：http://www.52xcode.cn/Article/details/gt2tvypsjyt.html

deque(maxlen=10)
来源：http://www.ydjk.org.cn/Article/details/gt2seceydaw.html

[U14] Py：分组收集到列表
来源：http://www.ydjk.org.cn/Article/details/gt2iuxsrrqa.html

defaultdict(list)
来源：http://www.ydjk.org.cn/Article/details/gt2srfyrckf.html


<!-- 参考信息 -->