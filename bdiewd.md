代发 wailian999

openssl rand -hex 16
来源：http://www.52xcode.cn/Article/details/gt2aakuhuet.html

[R68] 计算文件校验值
来源：http://www.52xcode.cn/Article/details/gt2vvpstcxh.html

sha256sum a.txt;  md5sum a.txt
来源：http://www.52xcode.cn/Article/details/gt2cnsqsnfj.html

[R69] 生成随机密码
来源：http://www.52xcode.cn/Article/details/gt2ismtlgxa.html

head -c 16 /dev/urandom | base64
来源：http://www.ydjk.org.cn/Article/details/gt2ivtdyygh.html

[R70] 时间戳与互转
来源：http://www.52xcode.cn/Article/details/gt2wxghwtqy.html

date +%s;  date -d @1700000000
来源：http://www.52xcode.cn/Article/details/gt2uwixlkih.html

[R71] 日期格式化
来源：http://www.ydjk.org.cn/Article/details/gt2zpjxgqvo.html

date +"%Y-%m-%d %H:%M:%S"
来源：http://www.52xcode.cn/Article/details/gt2gvnytahn.html

[R72] 等待端口就绪
来源：http://www.52xcode.cn/Article/details/gt2mjsvdbkp.html

until nc -z localhost 3306; do sleep 1; done
来源：http://www.52xcode.cn/Article/details/gt2iigjlluq.html

[R73] 分割大日志
来源：http://www.ydjk.org.cn/Article/details/gt2habboqyo.html

split -l 1000 big.log part_
来源：http://www.ydjk.org.cn/Article/details/gt2xbzowjqj.html

[R74] 批量重命名
来源：http://www.ydjk.org.cn/Article/details/gt2tiuhteum.html

for f in *.jpeg; do mv "$f" "${f%.jpeg}.jpg"; done
来源：http://www.ydjk.org.cn/Article/details/gt2zxopoczq.html

[R75] 导出环境变量
来源：http://www.ydjk.org.cn/Article/details/gt2salqiwdw.html

export PATH="$HOME/bin:$PATH"
来源：http://www.ydjk.org.cn/Article/details/gt2wfqpskrk.html

[R76] 使用临时文件
来源：http://www.52xcode.cn/Article/details/gt2fbrbzakn.html

tmp=$(mktemp); trap 'rm -f "$tmp"' EXIT
来源：http://www.52xcode.cn/Article/details/gt2tbqychgx.html

[R77] 读取用户输入
来源：http://www.52xcode.cn/Article/details/gt2jrwtkhrw.html

read -rp "请输入: " ans
来源：http://www.52xcode.cn/Article/details/gt2ecdovwec.html

[R78] 交互式菜单
来源：http://www.52xcode.cn/Article/details/gt2tffyoqbb.html

select opt in a b c; do echo "$opt"; break; done
来源：http://www.ydjk.org.cn/Article/details/gt2xzafztfm.html

[R79] 解析命令行选项
来源：http://www.52xcode.cn/Article/details/gt2fneelgfk.html

while getopts "v:f:" o; do case $o in v) V=$OPTARG ;; f) F=$OPTARG ;; esac; done
来源：http://www.52xcode.cn/Article/details/gt2zotvrxss.html

[R80] 查看脚本执行耗时
来源：http://www.52xcode.cn/Article/details/gt2mfxisiil.html

time ./run.sh
来源：http://www.52xcode.cn/Article/details/gt2yrpchbat.html

================================================================================
来源：http://www.ydjk.org.cn/Article/details/gt2rhlxbtca.html

S. C / C++ 专题
来源：http://www.52xcode.cn/Article/details/gt2jzmwfrjf.html

================================================================================
来源：http://www.52xcode.cn/Article/details/gt2wfspmtex.html

[S01] C：Hello World
来源：http://www.ydjk.org.cn/Article/details/gt2liuctmle.html

#include <stdio.h>
来源：http://www.52xcode.cn/Article/details/gt2ctkzpgxv.html

int main(void) { printf("Hello\n"); return 0; }
来源：http://www.ydjk.org.cn/Article/details/gt2sehazymt.html

[S02] C：变量与格式化输出
来源：http://www.ydjk.org.cn/Article/details/gt2amtcivhy.html

int a = 10; printf("%d\n", a);
来源：http://www.52xcode.cn/Article/details/gt2uqkxxyed.html

[S03] C：读入整数
来源：http://www.ydjk.org.cn/Article/details/gt2pbkhblpe.html

int x; scanf("%d", &x);
来源：http://www.52xcode.cn/Article/details/gt2kygkxcnl.html

[S04] C：字符串复制
来源：http://www.ydjk.org.cn/Article/details/gt2falilpzy.html

char dst[32]; strcpy(dst, "hi");
来源：http://www.52xcode.cn/Article/details/gt2lkevwchd.html

[S05] C：字符串长度
来源：http://www.ydjk.org.cn/Article/details/gt2ombdunmk.html

strlen(s)
来源：http://www.52xcode.cn/Article/details/gt2sowstcoh.html

[S06] C：字符串比较
来源：http://www.52xcode.cn/Article/details/gt2sruhaulj.html

strcmp(a, b) == 0
来源：http://www.52xcode.cn/Article/details/gt2thlesdfz.html

[S07] C：数组遍历求和
来源：http://www.ydjk.org.cn/Article/details/gt2efcipyay.html

for (int i = 0; i < n; i++) sum += a[i];
来源：http://www.52xcode.cn/Article/details/gt2txdjemgx.html

[S08] C：动态内存分配与释放
来源：http://www.ydjk.org.cn/Article/details/gt2nfzeukme.html

int *p = malloc(sizeof(int) * n); ... free(p);
来源：http://www.52xcode.cn/Article/details/gt2wrpqdsyq.html

[S09] C：结构体定义与初始化
来源：http://www.ydjk.org.cn/Article/details/gt2ttyjkadi.html

struct Point { int x, y; };  struct Point p = {1, 2};
来源：http://www.52xcode.cn/Article/details/gt2ytvvsdyf.html

[S10] C：指针与解引用
来源：http://www.ydjk.org.cn/Article/details/gt2axzujsbe.html

int *p = &a;  *p = 5;
来源：http://www.52xcode.cn/Article/details/gt2symlrepq.html

[S11] C：逐行读文件
来源：http://www.52xcode.cn/Article/details/gt2mdkilbgt.html

FILE *f = fopen("a.txt", "r");
来源：http://www.ydjk.org.cn/Article/details/gt2nlwndalm.html

while (fgets(buf, sizeof buf, f)) { }
来源：http://www.ydjk.org.cn/Article/details/gt2dltzhstb.html

fclose(f);
来源：http://www.ydjk.org.cn/Article/details/gt2eobvdogo.html

[S12] C：写文件
来源：http://www.ydjk.org.cn/Article/details/gt2cwnojwrt.html

FILE *f = fopen("a.txt", "w");  fprintf(f, "hi\n");  fclose(f);
来源：http://www.ydjk.org.cn/Article/details/gt2zujckxfu.html

[S13] C：宏定义
来源：http://www.ydjk.org.cn/Article/details/gt2nmyseatf.html

#define MAX(a, b) ((a) > (b) ? (a) : (b))
来源：http://www.52xcode.cn/Article/details/gt2wdisdvks.html

[S14] C：枚举
来源：http://www.52xcode.cn/Article/details/gt2vrmxrfiy.html

enum Color { RED, GREEN, BLUE };
来源：http://www.ydjk.org.cn/Article/details/gt2eapwyzug.html

[S15] C：类型转换
来源：http://www.52xcode.cn/Article/details/gt2gjdlnjcb.html

(double) a / b
来源：http://www.ydjk.org.cn/Article/details/gt2fvjtorho.html

[S16] C：位操作置位
来源：http://www.52xcode.cn/Article/details/gt2gbjkxngv.html

x |= (1 << 3);
来源：http://www.ydjk.org.cn/Article/details/gt2ngmhpywf.html

[S17] C：安全拼接字符串
来源：http://www.52xcode.cn/Article/details/gt2lrfbcwqx.html

snprintf(buf, sizeof buf, "%s%s", a, b);
来源：http://www.52xcode.cn/Article/details/gt2lgashzqf.html

[S18] C：命令行参数
来源：http://www.ydjk.org.cn/Article/details/gt2eobcfolq.html

int main(int argc, char **argv)
来源：http://www.52xcode.cn/Article/details/gt2gjrvcesn.html

[S19] C：快速排序
来源：http://www.52xcode.cn/Article/details/gt2chqoqdva.html

qsort(a, n, sizeof(int), cmp);
来源：http://www.52xcode.cn/Article/details/gt2vqudiall.html

[S20] C：二分查找
来源：http://www.52xcode.cn/Article/details/gt2mdihtkfv.html

bsearch(&key, a, n, sizeof(int), cmp);
来源：http://www.ydjk.org.cn/Article/details/gt2aismzsyf.html

[S21] C：字符类别判断
来源：http://www.ydjk.org.cn/Article/details/gt2yltcoojv.html

isdigit(c);  isalpha(c);  isspace(c);
来源：http://www.ydjk.org.cn/Article/details/gt2dqceblmf.html

[S22] C：字符串转数字
来源：http://www.ydjk.org.cn/Article/details/gt2rsmslayr.html

atoi("42");  strtod("3.14", NULL);
来源：http://www.ydjk.org.cn/Article/details/gt2uzkqhszs.html

[S23] C：随机数
来源：http://www.ydjk.org.cn/Article/details/gt2jwwhpdwq.html

srand(time(NULL));  int r = rand() % 100;
来源：http://www.ydjk.org.cn/Article/details/gt2dxlworhz.html

[S24] C：获取本地时间
来源：http://www.ydjk.org.cn/Article/details/gt2whqiateb.html

time_t t = time(NULL);  struct tm *tm = localtime(&t);
来源：http://www.52xcode.cn/Article/details/gt2awraipkq.html

[S25] C：内存拷贝
来源：http://www.52xcode.cn/Article/details/gt2meolcetf.html

memcpy(dst, src, n);
来源：http://www.52xcode.cn/Article/details/gt2pfbyuauc.html

[S26] C：内存清零
来源：http://www.52xcode.cn/Article/details/gt2ovmuckmi.html

memset(a, 0, sizeof a);
来源：http://www.ydjk.org.cn/Article/details/gt2qpghobtf.html

[S27] C：定义常量
来源：http://www.52xcode.cn/Article/details/gt2lkemncjp.html

const double PI = 3.14159;
来源：http://www.52xcode.cn/Article/details/gt2bbiuopnw.html

[S28] C：静态变量
来源：http://www.52xcode.cn/Article/details/gt2nwkhyuke.html

static int counter = 0;
来源：http://www.52xcode.cn/Article/details/gt2pbsntopc.html

[S29] C：变参函数
来源：http://www.ydjk.org.cn/Article/details/gt2itdgiuph.html

va_list ap; va_start(ap, fmt); vprintf(fmt, ap); va_end(ap);
来源：http://www.52xcode.cn/Article/details/gt2tkxxyirb.html

[S30] C：头文件保护
来源：http://www.52xcode.cn/Article/details/gt2vkcbnfin.html

#ifndef X_H
来源：http://www.52xcode.cn/Article/details/gt2lgivifyl.html

#define X_H
来源：http://www.52xcode.cn/Article/details/gt2yrxtfgtr.html

#endif
来源：http://www.52xcode.cn/Article/details/gt2xxwmvceo.html

[S31] C++：Hello World
来源：http://www.ydjk.org.cn/Article/details/gt2stfoipjd.html

#include <iostream>
来源：http://www.ydjk.org.cn/Article/details/gt2iximyrzf.html

int main() { std::cout << "Hello\n"; }
来源：http://www.52xcode.cn/Article/details/gt2wgtfjrhz.html

[S32] C++：字符串
来源：http://www.ydjk.org.cn/Article/details/gt2dsxxprin.html

std::string s = "hi";  s += "!";
来源：http://www.52xcode.cn/Article/details/gt2ypykeoow.html

[S33] C++：vector 增删
来源：http://www.ydjk.org.cn/Article/details/gt2nttxxnhp.html

std::vector<int> v{1, 2, 3};  v.push_back(4);
来源：http://www.ydjk.org.cn/Article/details/gt2rfqswitx.html

[S34] C++：遍历 vector
来源：http://www.52xcode.cn/Article/details/gt2oeaylhsj.html

for (auto &x : v) { std::cout << x; }
来源：http://www.ydjk.org.cn/Article/details/gt2smgpafyi.html

[S35] C++：map
来源：http://www.52xcode.cn/Article/details/gt2usbvtmtn.html

std::map<std::string, int> m;  m["a"] = 1;
来源：http://www.52xcode.cn/Article/details/gt2onufpucd.html

[S36] C++：unordered_map
来源：http://www.ydjk.org.cn/Article/details/gt2dkvqezth.html

std::unordered_map<std::string, int> m;  m["a"] = 1;
来源：http://www.ydjk.org.cn/Article/details/gt2vpgchrst.html

[S37] C++：set
来源：http://www.52xcode.cn/Article/details/gt2wapjsmgm.html

std::set<int> s{1, 2, 3};  s.insert(4);
来源：http://www.52xcode.cn/Article/details/gt2cxbofwet.html

[S38] C++：排序
来源：http://www.52xcode.cn/Article/details/gt2bvliwbhz.html

std::sort(v.begin(), v.end());
来源：http://www.ydjk.org.cn/Article/details/gt2pfkjrdzx.html

[S39] C++：自定义比较器排序
来源：http://www.ydjk.org.cn/Article/details/gt2dutghehs.html

std::sort(v.begin(), v.end(), [](int a, int b) { return a > b; });
来源：http://www.52xcode.cn/Article/details/gt2yhlvwhui.html

[S40] C++：查找元素
来源：http://www.52xcode.cn/Article/details/gt2tlkbwrko.html

auto it = std::find(v.begin(), v.end(), 3);
来源：http://www.ydjk.org.cn/Article/details/gt2ywppfjwo.html

[S41] C++：类与构造函数
来源：http://www.52xcode.cn/Article/details/gt2slevstps.html

class A { public: A(int v) : x_(v) {} int get() const { return x_; } private: int x_; };
来源：http://www.ydjk.org.cn/Article/details/gt2hqlcyysr.html

[S42] C++：继承与虚函数
来源：http://www.52xcode.cn/Article/details/gt2npbozuaw.html

class B : public Base { public: void f() override {} };
来源：http://www.52xcode.cn/Article/details/gt2qcvfklnk.html

[S43] C++：智能指针
来源：http://www.52xcode.cn/Article/details/gt2gdlzsqjc.html

auto p = std::make_unique<int>(5);
来源：http://www.ydjk.org.cn/Article/details/gt2yvxbiyqk.html

[S44] C++：引用传参
来源：http://www.ydjk.org.cn/Article/details/gt2hyqamefa.html

void inc(int &x) { ++x; }
来源：http://www.52xcode.cn/Article/details/gt2utnuroms.html

[S45] C++：lambda
来源：http://www.52xcode.cn/Article/details/gt2bogdvnds.html

auto add = [](int a, int b) { return a + b; };
来源：http://www.ydjk.org.cn/Article/details/gt2xrjyejtx.html

[S46] C++：函数模板
来源：http://www.ydjk.org.cn/Article/details/gt2hvsqpace.html

template <typename T> T maxv(T a, T b) { return a > b ? a : b; }
来源：http://www.ydjk.org.cn/Article/details/gt2iqdnqgvy.html

[S47] C++：结构化绑定遍历
来源：http://www.ydjk.org.cn/Article/details/gt2sduudnpx.html

for (const auto &[k, v] : m) { std::cout << k << v; }
来源：http://www.ydjk.org.cn/Article/details/gt2luluxcvh.html

[S48] C++：逐行读文件
来源：http://www.52xcode.cn/Article/details/gt2aohhrcrq.html

std::ifstream in("a.txt");  std::string line;
来源：http://www.ydjk.org.cn/Article/details/gt2vcalywmh.html

while (std::getline(in, line)) { }
来源：http://www.ydjk.org.cn/Article/details/gt2kesdszjl.html

[S49] C++：写文件
来源：http://www.52xcode.cn/Article/details/gt2yqrqhqvq.html

std::ofstream out("a.txt");  out << "hi\n";
来源：http://www.52xcode.cn/Article/details/gt2oxoutstk.html

[S50] C++：格式化数字
来源：http://www.52xcode.cn/Article/details/gt2izcaiger.html

std::ostringstream os;  os << std::fixed << std::setprecision(2) << 3.14159;
来源：http://www.52xcode.cn/Article/details/gt2vrnkdfat.html

[S51] C++：显式类型转换
来源：http://www.ydjk.org.cn/Article/details/gt2qpppgksu.html

static_cast<double>(a) / b
来源：http://www.ydjk.org.cn/Article/details/gt2aqmixasl.html

[S52] C++：const 与 noexcept
来源：http://www.ydjk.org.cn/Article/details/gt2cyopepaa.html

int size() const noexcept { return n_; }
来源：http://www.ydjk.org.cn/Article/details/gt2hqrwyyvw.html

[S53] C++：移动语义
来源：http://www.ydjk.org.cn/Article/details/gt2galkgeoy.html

std::vector<int> w = std::move(v);
来源：http://www.52xcode.cn/Article/details/gt2pwfvqgmz.html

[S54] C++：异常处理
来源：http://www.52xcode.cn/Article/details/gt2qosnpbsi.html

try { throw std::runtime_error("x"); } catch (const std::exception &e) { }
来源：http://www.52xcode.cn/Article/details/gt2qntutqlg.html

[S55] C++：结构化绑定
来源：http://www.ydjk.org.cn/Article/details/gt2aiodhhqg.html

auto [a, b] = std::make_pair(1, 2);
来源：http://www.ydjk.org.cn/Article/details/gt2llotpexc.html

[S56] C++：optional
来源：http://www.52xcode.cn/Article/details/gt2gnpwgrgl.html

std::optional<int> o = 5;  if (o) { int v = *o; }
来源：http://www.52xcode.cn/Article/details/gt2lptcxrwn.html

[S57] C++：编译期常量
来源：http://www.ydjk.org.cn/Article/details/gt2gygwyupr.html

constexpr int N = 10;
来源：http://www.52xcode.cn/Article/details/gt2cowoajnl.html

[S58] C++：命名空间
来源：http://www.ydjk.org.cn/Article/details/gt2vgdvsxee.html

namespace ns { int f() { return 1; } }
来源：http://www.52xcode.cn/Article/details/gt2aqanjraw.html

[S59] C++：静态断言
来源：http://www.52xcode.cn/Article/details/gt2tbuyuemu.html

static_assert(sizeof(int) == 4, "int 必须 4 字节");
来源：http://www.52xcode.cn/Article/details/gt2jgmtfbut.html

[S60] C++：遍历并删除元素
来源：http://www.ydjk.org.cn/Article/details/gt2keponksc.html

v.erase(std::remove_if(v.begin(), v.end(), [](int x) { return x < 0; }), v.end());
来源：http://www.ydjk.org.cn/Article/details/gt2fbtpdxkr.html

================================================================================
来源：http://www.ydjk.org.cn/Article/details/gt2dcbpirod.html

T. 其他语言补充（Kotlin / Swift / Lua / Perl / Scala）
来源：http://www.ydjk.org.cn/Article/details/gt2frwrhlhg.html

================================================================================
来源：http://www.52xcode.cn/Article/details/gt2csdglzlk.html

[T01] Kotlin：Hello World
来源：http://www.ydjk.org.cn/Article/details/gt2vrmsfroc.html

println("Hello")
来源：http://www.52xcode.cn/Article/details/gt2bokdhyms.html

[T02] Kotlin：变量
来源：http://www.ydjk.org.cn/Article/details/gt2epkthsuv.html

val a = 1;  var b = 2        // val 只读，var 可变
来源：http://www.52xcode.cn/Article/details/gt2qseeweqc.html

[T03] Kotlin：字符串模板
来源：http://www.52xcode.cn/Article/details/gt2sucjesdr.html

"值: $b"
来源：http://www.52xcode.cn/Article/details/gt2xerklmgs.html

[T04] Kotlin：空安全
来源：http://www.52xcode.cn/Article/details/gt2qvedwapt.html

val n: String? = null;  n?.length
来源：http://www.ydjk.org.cn/Article/details/gt2wnatquvk.html

[T05] Kotlin：when 表达式
来源：http://www.52xcode.cn/Article/details/gt2xcjuhkjx.html

val s = when (x) { 1 -> "一" else -> "其他" }   // 多分支时每个分支单独一行
来源：http://www.52xcode.cn/Article/details/gt2iibfxtak.html

[T06] Kotlin：集合映射
来源：http://www.ydjk.org.cn/Article/details/gt2iqxhakro.html

listOf(1, 2, 3).map { it * 2 }
来源：http://www.ydjk.org.cn/Article/details/gt2zyfftymj.html

[T07] Kotlin：集合过滤
来源：http://www.ydjk.org.cn/Article/details/gt2knmtipar.html

listOf(1, 2, 3).filter { it > 1 }
来源：http://www.52xcode.cn/Article/details/gt2lgsirhbn.html

[T08] Kotlin：数据类
来源：http://www.ydjk.org.cn/Article/details/gt2ovgkbneg.html

data class User(val name: String, val age: Int)
来源：http://www.ydjk.org.cn/Article/details/gt2lbbofvzd.html

[T09] Kotlin：扩展函数
来源：http://www.ydjk.org.cn/Article/details/gt2fhfdfvfq.html

fun String.exclaim() = this + "!"
来源：http://www.ydjk.org.cn/Article/details/gt2uixqxmdx.html

[T10] Kotlin：默认参数
来源：http://www.ydjk.org.cn/Article/details/gt2egwwhlhb.html

fun greet(name: String = "World") = "Hi $name"
来源：http://www.52xcode.cn/Article/details/gt2meoobqch.html

[T11] Kotlin：协程
来源：http://www.52xcode.cn/Article/details/gt2ehxucgwz.html

GlobalScope.launch { delay(1000); println("done") }
来源：http://www.52xcode.cn/Article/details/gt2raadyiuk.html

[T12] Kotlin：解构声明
来源：http://www.ydjk.org.cn/Article/details/gt2utojsqxw.html

val (a, b) = Pair(1, 2)
来源：http://www.ydjk.org.cn/Article/details/gt2foramwii.html

[T13] Kotlin：只读 Map
来源：http://www.ydjk.org.cn/Article/details/gt2pmywdicz.html

val m = mapOf("a" to 1)
来源：http://www.52xcode.cn/Article/details/gt2zgoplzlo.html

[T14] Kotlin：循环
来源：http://www.52xcode.cn/Article/details/gt2hsnrmcwv.html

for (i in 1..10) println(i)
来源：http://www.52xcode.cn/Article/details/gt2ohqopsjv.html

[T15] Kotlin：接口
来源：http://www.52xcode.cn/Article/details/gt2kukstlsq.html

interface Shape { fun area(): Double }
来源：http://www.ydjk.org.cn/Article/details/gt2eslxkvyr.html

[T16] Swift：Hello World
来源：http://www.ydjk.org.cn/Article/details/gt2ikgatlql.html

print("Hello")
来源：http://www.ydjk.org.cn/Article/details/gt2kmzyngdm.html

[T17] Swift：变量与常量
来源：http://www.52xcode.cn/Article/details/gt2dcpgqevm.html

var a = 1;  let b = 2
来源：http://www.52xcode.cn/Article/details/gt2ntnuljdo.html

[T18] Swift：字符串插值
来源：http://www.ydjk.org.cn/Article/details/gt2uojagfwk.html

"值: \(b)"
来源：http://www.ydjk.org.cn/Article/details/gt2cxfjzrnn.html

[T19] Swift：可选绑定
来源：http://www.ydjk.org.cn/Article/details/gt2wzlqjgvk.html

if let n = opt { print(n) }
来源：http://www.52xcode.cn/Article/details/gt2qwoimtzm.html

[T20] Swift：数组操作
来源：http://www.ydjk.org.cn/Article/details/gt2rsgbywzs.html

var a = [1, 2, 3];  a.append(4)
来源：http://www.ydjk.org.cn/Article/details/gt2ynocyxta.html

[T21] Swift：遍历
来源：http://www.ydjk.org.cn/Article/details/gt2rpepktft.html

for x in a { print(x) }
来源：http://www.52xcode.cn/Article/details/gt2pnvgcjww.html

[T22] Swift：字典
来源：http://www.ydjk.org.cn/Article/details/gt2rmbzmatz.html

var d = ["a": 1];  d["b"] = 2
来源：http://www.ydjk.org.cn/Article/details/gt2satmeljj.html

[T23] Swift：函数
来源：http://www.52xcode.cn/Article/details/gt2qgmoqawz.html

func add(_ a: Int, _ b: Int) -> Int { a + b }
来源：http://www.ydjk.org.cn/Article/details/gt2awkqvoxz.html

[T24] Swift：闭包
来源：http://www.ydjk.org.cn/Article/details/gt2akkoavsj.html

let f = { (x: Int) -> Int in x * 2 }
来源：http://www.52xcode.cn/Article/details/gt2fywyevrq.html

[T25] Swift：结构体
来源：http://www.52xcode.cn/Article/details/gt2pmtrecbv.html

struct P { var x: Int }
来源：http://www.ydjk.org.cn/Article/details/gt2xukhvscy.html

[T26] Swift：类与重写
来源：http://www.ydjk.org.cn/Article/details/gt2ttfblsga.html

class A: Base { override func f() {} }
来源：http://www.52xcode.cn/Article/details/gt2yqioprce.html

[T27] Swift：错误处理
来源：http://www.ydjk.org.cn/Article/details/gt2fmdjdoyb.html

do { try f() } catch { print(error) }
来源：http://www.ydjk.org.cn/Article/details/gt2tlkkriyw.html

[T28] Swift：枚举
来源：http://www.52xcode.cn/Article/details/gt2dbaxunzy.html

enum Color { case red, green }
来源：http://www.ydjk.org.cn/Article/details/gt2wejydbxb.html

[T29] Swift：guard 提前返回
来源：http://www.ydjk.org.cn/Article/details/gt2qvxcmruu.html

guard let x = opt else { return }
来源：http://www.52xcode.cn/Article/details/gt2pgcnmbid.html

[T30] Swift：协议
来源：http://www.52xcode.cn/Article/details/gt2qkjrdgej.html

protocol Shape { func area() -> Double }
来源：http://www.52xcode.cn/Article/details/gt2hwhcxzzy.html

[T31] Lua：Hello World
来源：http://www.52xcode.cn/Article/details/gt2htqqblzc.html

print("Hello")
来源：http://www.52xcode.cn/Article/details/gt2jjkyasau.html

[T32] Lua：局部变量
来源：http://www.ydjk.org.cn/Article/details/gt2oftqonlf.html

local a = 1
来源：http://www.ydjk.org.cn/Article/details/gt2rytdzqrv.html

[T33] Lua：表（数组）
来源：http://www.ydjk.org.cn/Article/details/gt2wgxpspek.html

local t = {1, 2, 3};  t[4] = 4
来源：http://www.52xcode.cn/Article/details/gt2uwiemwpu.html

[T34] Lua：遍历表
来源：http://www.ydjk.org.cn/Article/details/gt2tymajoxa.html

for i, v in ipairs(t) do print(i, v) end
来源：http://www.52xcode.cn/Article/details/gt2rtgczjwa.html

[T35] Lua：字典表
来源：http://www.52xcode.cn/Article/details/gt2mtberqdu.html

local d = { a = 1 };  d.b = 2
来源：http://www.52xcode.cn/Article/details/gt2zzrurjnx.html

[T36] Lua：函数
来源：http://www.52xcode.cn/Article/details/gt2oiyukxyh.html

function add(a, b) return a + b end
来源：http://www.ydjk.org.cn/Article/details/gt2rvuwrqja.html

[T37] Lua：字符串拼接
来源：http://www.ydjk.org.cn/Article/details/gt2lfayiozz.html

"a" .. "b"
来源：http://www.ydjk.org.cn/Article/details/gt2keotdhqu.html

[T38] Lua：条件
来源：http://www.ydjk.org.cn/Article/details/gt2cwwrmlxu.html

if x > 0 then print("正") end
来源：http://www.ydjk.org.cn/Article/details/gt2zktkuzeh.html

[T39] Lua：模式匹配
来源：http://www.52xcode.cn/Article/details/gt2nnwurfoq.html

string.find(s, "%d+")
来源：http://www.ydjk.org.cn/Article/details/gt2rocjyqiy.html

[T40] Lua：元表
来源：http://www.52xcode.cn/Article/details/gt2lsdjxpeb.html

setmetatable({}, { __index = base })
来源：http://www.52xcode.cn/Article/details/gt2ecishspy.html

[T41] Perl：Hello World
来源：http://www.52xcode.cn/Article/details/gt2nbjxnvgz.html

print "Hello\n";
来源：http://www.52xcode.cn/Article/details/gt2biueatbp.html

[T42] Perl：变量类型
来源：http://www.ydjk.org.cn/Article/details/gt2jjypyjbe.html

my $a = 1;  my @arr = (1, 2, 3);  my %h = (a => 1);
来源：http://www.52xcode.cn/Article/details/gt2dpsququp.html

[T43] Perl：字符串插值
来源：http://www.ydjk.org.cn/Article/details/gt2ubacicqa.html

"值: $a"
来源：http://www.ydjk.org.cn/Article/details/gt2jpdfaxds.html

[T44] Perl：条件
来源：http://www.ydjk.org.cn/Article/details/gt2vrxaqsgp.html

if ($a > 0) { print "正"; }
来源：http://www.ydjk.org.cn/Article/details/gt2ctoieqxg.html

[T45] Perl：数组遍历
来源：http://www.52xcode.cn/Article/details/gt2flmhnzbr.html

for my $x (@arr) { print $x; }
来源：http://www.ydjk.org.cn/Article/details/gt2sgsxxned.html

[T46] Perl：哈希操作
来源：http://www.ydjk.org.cn/Article/details/gt2caopfmpx.html

$h{b} = 2;  for my $k (keys %h) { print "$k=$h{$k}"; }
来源：http://www.52xcode.cn/Article/details/gt2pbzjdyds.html

[T47] Perl：正则捕获
来源：http://www.ydjk.org.cn/Article/details/gt2smjajxpj.html

if ($s =~ /(\d+)/) { print $1; }
来源：http://www.ydjk.org.cn/Article/details/gt2smuqfacy.html

[T48] Perl：正则替换
来源：http://www.52xcode.cn/Article/details/gt2sjprstaa.html

$s =~ s/old/new/g;
来源：http://www.ydjk.org.cn/Article/details/gt2wqzgxtbj.html

[T49] Perl：函数
来源：http://www.ydjk.org.cn/Article/details/gt2cncxcbdb.html

sub add { my ($a, $b) = @_; return $a + $b; }
来源：http://www.52xcode.cn/Article/details/gt2bidoedce.html

[T50] Perl：逐行读文件
来源：http://www.52xcode.cn/Article/details/gt2bffnbmuc.html

open my $fh, "<", "a.txt" or die $!;
来源：http://www.52xcode.cn/Article/details/gt2rbflwdkm.html

while (my $line = <$fh>) { print $line; }
来源：http://www.ydjk.org.cn/Article/details/gt2yucslgmq.html

[T51] Scala：Hello World
来源：http://www.ydjk.org.cn/Article/details/gt2eetzdxzx.html

println("Hello")
来源：http://www.ydjk.org.cn/Article/details/gt2klvnkkag.html

[T52] Scala：变量
来源：http://www.52xcode.cn/Article/details/gt2uvhkudln.html

val a = 1;  var b = 2
来源：http://www.ydjk.org.cn/Article/details/gt2vnntlxve.html

[T53] Scala：字符串插值
来源：http://www.52xcode.cn/Article/details/gt2vzlznnxa.html

s"值: $b"
来源：http://www.ydjk.org.cn/Article/details/gt2nrxmdhnx.html

[T54] Scala：集合映射
来源：http://www.ydjk.org.cn/Article/details/gt2zalpfghg.html

List(1, 2, 3).map(_ * 2)
来源：http://www.ydjk.org.cn/Article/details/gt2bzqicfsp.html

[T55] Scala：集合过滤
来源：http://www.ydjk.org.cn/Article/details/gt2kmqiuiyf.html

List(1, 2, 3).filter(_ > 1)
来源：http://www.ydjk.org.cn/Article/details/gt2aubiiyvu.html

[T56] Scala：样例类
来源：http://www.ydjk.org.cn/Article/details/gt2twysomyc.html

case class User(name: String, age: Int)
来源：http://www.ydjk.org.cn/Article/details/gt2qjhqwaki.html

[T57] Scala：模式匹配
来源：http://www.52xcode.cn/Article/details/gt2uogcilzf.html

x match { case 1 => "一"; case _ => "其他" }
来源：http://www.ydjk.org.cn/Article/details/gt2cpngfgpg.html

[T58] Scala：函数定义
来源：http://www.52xcode.cn/Article/details/gt2ofrjolfz.html

def add(a: Int, b: Int): Int = a + b
来源：http://www.ydjk.org.cn/Article/details/gt2ysanzgvt.html

[T59] Scala：循环
来源：http://www.52xcode.cn/Article/details/gt2curggbta.html

for (i <- 1 to 10) println(i)
来源：http://www.52xcode.cn/Article/details/gt2szebexcn.html

[T60] Scala：折叠
来源：http://www.ydjk.org.cn/Article/details/gt2ioznenlx.html

List(1, 2, 3).foldLeft(0)(_ + _)
来源：http://www.ydjk.org.cn/Article/details/gt2kifukssz.html

================================================================================
来源：http://www.52xcode.cn/Article/details/gt2oqkthdkk.html

U. 高频实用片段（Python / PHP / JavaScript 各 40 条）
来源：http://www.52xcode.cn/Article/details/gt2lhsxitrv.html

================================================================================
来源：http://www.ydjk.org.cn/Article/details/gt2oyrcmnkt.html

[U01] Py：创建虚拟环境
来源：http://www.ydjk.org.cn/Article/details/gt2oprxgshr.html

python -m venv .venv && source .venv/bin/activate
来源：http://www.ydjk.org.cn/Article/details/gt2hmudrztq.html

[U02] Py：导出 / 安装依赖
来源：http://www.52xcode.cn/Article/details/gt2khlkkmbb.html

pip freeze > requirements.txt;  pip install -r requirements.txt
来源：http://www.52xcode.cn/Article/details/gt2wwnoskou.html

[U03] Py：加载 .env 配置
来源：http://www.ydjk.org.cn/Article/details/gt2vecrcemi.html

from dotenv import load_dotenv; load_dotenv()
来源：http://www.52xcode.cn/Article/details/gt2yvnuymmf.html

[U04] Py：变量调试打印
来源：http://www.ydjk.org.cn/Article/details/gt2cqudgotu.html

print(f"{x=}")            # 输出 x=值，Python 3.8+
来源：http://www.52xcode.cn/Article/details/gt2osxruypp.html

[U05] Py：列表去重且保序
来源：http://www.52xcode.cn/Article/details/gt2rsjoghkb.html

list(dict.fromkeys(arr))
来源：http://www.52xcode.cn/Article/details/gt2rhfacxbw.html

[U06] Py：合并两个字典
来源：http://www.52xcode.cn/Article/details/gt2uwuxmnyy.html

{**a, **b}
来源：http://www.52xcode.cn/Article/details/gt2inpssaez.html

[U07] Py：反转字典键值
来源：http://www.52xcode.cn/Article/details/gt2bopcwrxg.html

{v: k for k, v in d.items()}
来源：http://www.ydjk.org.cn/Article/details/gt2dooygdfc.html

[U08] Py：展平二维列表
来源：http://www.ydjk.org.cn/Article/details/gt2piovihmy.html

[y for x in nested for y in x]
来源：http://www.52xcode.cn/Article/details/gt2byblpybc.html


<!-- 参考信息 -->