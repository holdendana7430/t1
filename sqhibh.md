代发 wailian999

date +"%Y-%m-%d %H:%M:%S"
来源：http://hz.zhaomingkeji.xyz/gtsgdexfmx.html

[R72] 等待端口就绪
来源：http://hz.hnxiangtu.top/gtycpwykkf.html

until nc -z localhost 3306; do sleep 1; done
来源：http://hz.cqqwz.cn/gtrbqlhdfw.html

[R73] 分割大日志
来源：http://hz.52xcode.cn/gtmebqokxr.html

split -l 1000 big.log part_
来源：http://hz.jinqigufen.top/gtoufxzhhy.html

[R74] 批量重命名
来源：http://hz.yj202588.top/gtfillsijy.html

for f in *.jpeg; do mv "$f" "${f%.jpeg}.jpg"; done
来源：http://hz.sysykeji.top/gtbgjpltam.html

[R75] 导出环境变量
来源：http://hz.fzhhl.top/gtrmipkmyv.html

export PATH="$HOME/bin:$PATH"
来源：http://hz.pengpengdd.cyou/gtmitnhbdi.html

[R76] 使用临时文件
来源：http://hz.yj20258888.top/gtzeybimjc.html

tmp=$(mktemp); trap 'rm -f "$tmp"' EXIT
来源：http://hz.mhx1999.top/gtkclbeyui.html

[R77] 读取用户输入
来源：http://hz.c1oappe.top/gtlnsvcnsp.html

read -rp "请输入: " ans
来源：http://hz.hysaishi.cn/gtjcnrwfcy.html

[R78] 交互式菜单
来源：http://hz.gogol.net.cn/gtutheszxb.html

select opt in a b c; do echo "$opt"; break; done
来源：http://hz.xziqi.cn/gtymeiqkrn.html

[R79] 解析命令行选项
来源：http://hz.jianghu66.top/gtizygfucl.html

while getopts "v:f:" o; do case $o in v) V=$OPTARG ;; f) F=$OPTARG ;; esac; done
来源：http://hz.nanxinkj.top/gtknafgczs.html

[R80] 查看脚本执行耗时
来源：http://hz.yj20258.top/gtumdyntrz.html

time ./run.sh
来源：http://hz.aizwys.cn/gtfpfkojqc.html

================================================================================
来源：http://hz.0kj1m.cn/gtohgwjzws.html

S. C / C++ 专题
来源：http://hz.nanxinkj.top/gtbbxqpnft.html

================================================================================
来源：http://hz.jianghu66.top/gtsrxtyhhd.html

[S01] C：Hello World
来源：http://hz.sysykeji.top/gtnysyndpq.html

#include <stdio.h>
来源：http://hz.jinghuilouyu.cn/gtpzfrlpyf.html

int main(void) { printf("Hello\n"); return 0; }
来源：http://hz.hnxiangtu.top/gtainypaha.html

[S02] C：变量与格式化输出
来源：http://hz.zhengqikj.top/gthsuqyyhy.html

int a = 10; printf("%d\n", a);
来源：http://hz.tianlin.xyz/gtlhkxfvyl.html

[S03] C：读入整数
来源：http://hz.0kj1m.cn/gttwbmtywn.html

int x; scanf("%d", &x);
来源：http://hz.guowangkeji.top/gtnmoalila.html

[S04] C：字符串复制
来源：http://hz.andypj.xyz/gtebojijbf.html

char dst[32]; strcpy(dst, "hi");
来源：http://hz.pycfn.com/gttatyskzw.html

[S05] C：字符串长度
来源：http://hz.dianchejie.cn/gtxtvizxzr.html

strlen(s)
来源：http://hz.gzhubu.top/gtbgmcefaj.html

[S06] C：字符串比较
来源：http://hz.guowangkeji.top/gtgsxokrky.html

strcmp(a, b) == 0
来源：http://hz.dianchejie.cn/gtlrytwiws.html

[S07] C：数组遍历求和
来源：http://hz.gogol.net.cn/gtsbcgsrxy.html

for (int i = 0; i < n; i++) sum += a[i];
来源：http://hz.dashuyun.cn/gtmiyggtgx.html

[S08] C：动态内存分配与释放
来源：http://hz.shangyingyoupin.top/gtgbrwgpad.html

int *p = malloc(sizeof(int) * n); ... free(p);
来源：http://hz.daxiang520.top/gtawiquzwm.html

[S09] C：结构体定义与初始化
来源：http://hz.yj20258888.top/gtaibmlvqi.html

struct Point { int x, y; };  struct Point p = {1, 2};
来源：http://hz.xziqi.cn/gtgfamtyym.html

[S10] C：指针与解引用
来源：http://hz.guannengcc.top/gtfjtygtqv.html

int *p = &a;  *p = 5;
来源：http://hz.yanxiufei.cn/gthglzfuso.html

[S11] C：逐行读文件
来源：http://hz.hammf.cn/gttlvdjqff.html

FILE *f = fopen("a.txt", "r");
来源：http://hz.gogol.net.cn/gtbvquhyzv.html

while (fgets(buf, sizeof buf, f)) { }
来源：http://hz.dianchejie.cn/gtijfjvycg.html

fclose(f);
来源：http://hz.ybcxt.top/gtykgmolwc.html

[S12] C：写文件
来源：http://hz.zdqjudy.top/gtdazuxyvh.html

FILE *f = fopen("a.txt", "w");  fprintf(f, "hi\n");  fclose(f);
来源：http://hz.pengpengdd.cyou/gtwpamhuvo.html

[S13] C：宏定义
来源：http://hz.yj202588.top/gthxpuwgxj.html

#define MAX(a, b) ((a) > (b) ? (a) : (b))
来源：http://hz.fzhhl.top/gtupjzqzgm.html

[S14] C：枚举
来源：http://hz.hnxiangtu.top/gtmszpyslp.html

enum Color { RED, GREEN, BLUE };
来源：http://hz.havefunace.top/gthveqhsjb.html

[S15] C：类型转换
来源：http://hz.nanxuanxn.top/gtpunmieta.html

(double) a / b
来源：http://hz.ivvv.top/gtpnfylqcn.html

[S16] C：位操作置位
来源：http://hz.cheryme.top/gtvzlshfqi.html

x |= (1 << 3);
来源：http://hz.aibaodan.cn/gtmabcqoem.html

[S17] C：安全拼接字符串
来源：http://hz.wangshuangyany.cn/gtixxfxbue.html

snprintf(buf, sizeof buf, "%s%s", a, b);
来源：http://hz.9152youxi.cn/gtppnhfwrj.html

[S18] C：命令行参数
来源：http://hz.feifeiyinyue.top/gtbzccrrvn.html

int main(int argc, char **argv)
来源：http://hz.zhixingplan.top/gtyizkpfel.html

[S19] C：快速排序
来源：http://hz.cqqwz.cn/gtrcvhqdde.html

qsort(a, n, sizeof(int), cmp);
来源：http://hz.snrcjt.cn/gtyefnvynt.html

[S20] C：二分查找
来源：http://hz.cashguo.top/gtllbxsonr.html

bsearch(&key, a, n, sizeof(int), cmp);
来源：http://hz.c1oappe.top/gtgrukyenf.html

[S21] C：字符类别判断
来源：http://hz.yvedp.cn/gtyguzavfy.html

isdigit(c);  isalpha(c);  isspace(c);
来源：http://hz.aibaodan.cn/gtvececccr.html

[S22] C：字符串转数字
来源：http://hz.dashuyun.cn/gtowndupgd.html

atoi("42");  strtod("3.14", NULL);
来源：http://hz.cheryme.top/gtenllnygv.html

[S23] C：随机数
来源：http://hz.mhx1999.top/gtkvunqjdw.html

srand(time(NULL));  int r = rand() % 100;
来源：http://hz.cdnleiting.top/gtpvnzkyip.html

[S24] C：获取本地时间
来源：http://hz.chenlongwang.top/gttabmpjsx.html

time_t t = time(NULL);  struct tm *tm = localtime(&t);
来源：http://hz.shangyingyoupin.top/gtsxkipgjh.html

[S25] C：内存拷贝
来源：http://hz.tian-w.cn/gtgyptzoju.html

memcpy(dst, src, n);
来源：http://hz.yangfankeji.com/gtijpbxaiq.html

[S26] C：内存清零
来源：http://hz.ywan-chungtsiang.top/gtxtvffkwi.html

memset(a, 0, sizeof a);
来源：http://hz.fengsongda.top/gtosfmdydt.html

[S27] C：定义常量
来源：http://hz.snrcjt.cn/gtqsigkvbm.html

const double PI = 3.14159;
来源：http://hz.hfpthk.cn/gtlzybxlqf.html

[S28] C：静态变量
来源：http://hz.gzhubu.top/gtinmyczoo.html

static int counter = 0;
来源：http://hz.0kj1m.cn/gtrckpmcrn.html

[S29] C：变参函数
来源：http://hz.nwbrower.top/gtyquahqxd.html

va_list ap; va_start(ap, fmt); vprintf(fmt, ap); va_end(ap);
来源：http://hz.yvedp.cn/gtzmabrejd.html

[S30] C：头文件保护
来源：http://hz.mhx1999.top/gtmaqgiweq.html

#ifndef X_H
来源：http://hz.pycfn.com/gtgahyknlw.html

#define X_H
来源：http://hz.ybcxt.top/gtdbrlrmvu.html

#endif
来源：http://hz.fzhhl.top/gtegiuxywj.html

[S31] C++：Hello World
来源：http://hz.jinqigfzy.top/gtliwyljrt.html

#include <iostream>
来源：http://hz.hysaishi.cn/gtahvckais.html

int main() { std::cout << "Hello\n"; }
来源：http://hz.ybcxt.top/gtfqjtzkjp.html

[S32] C++：字符串
来源：http://hz.wangshuangyany.cn/gtjskebrpe.html

std::string s = "hi";  s += "!";
来源：http://hz.cashguo.top/gteragvedh.html

[S33] C++：vector 增删
来源：http://hz.yangfankeji.com/gtrnukloja.html

std::vector<int> v{1, 2, 3};  v.push_back(4);
来源：http://hz.hammf.cn/gtwyehbyll.html

[S34] C++：遍历 vector
来源：http://hz.ywan-chungtsiang.top/gtnvmigeis.html

for (auto &x : v) { std::cout << x; }
来源：http://hz.jqgfzy.top/gtnugragog.html

[S35] C++：map
来源：http://hz.hysaishi.cn/gtdkqsmlum.html

std::map<std::string, int> m;  m["a"] = 1;
来源：http://hz.316326.xyz/gtpglydcaa.html

[S36] C++：unordered_map
来源：http://hz.zycfv.cn/gtjnqhcwym.html

std::unordered_map<std::string, int> m;  m["a"] = 1;
来源：http://hz.jiagoushi.top/gtqgkdayuz.html

[S37] C++：set
来源：http://hz.wangshuangyany.cn/gtlztrhxeo.html

std::set<int> s{1, 2, 3};  s.insert(4);
来源：http://hz.yangfankeji.com/gtfwhhcmic.html

[S38] C++：排序
来源：http://hz.gotoacloud.top/gtzoqakxvg.html

std::sort(v.begin(), v.end());
来源：http://hz.yongpay.top/gtchemxzrm.html

[S39] C++：自定义比较器排序
来源：http://hz.sxryk.cn/gtwnhhxyma.html

std::sort(v.begin(), v.end(), [](int a, int b) { return a > b; });
来源：http://hz.jinqigufen.top/gthpuwsgaw.html

[S40] C++：查找元素
来源：http://hz.andypj.xyz/gtqlaqvkoq.html

auto it = std::find(v.begin(), v.end(), 3);
来源：http://hz.jlsjyb.cn/gthaoaokvn.html

[S41] C++：类与构造函数
来源：http://hz.wangshuangyany.cn/gtexlmdami.html

class A { public: A(int v) : x_(v) {} int get() const { return x_; } private: int x_; };
来源：http://hz.tanke756.top/gtpqrjtker.html

[S42] C++：继承与虚函数
来源：http://hz.cqqwz.cn/gtwrnesgrb.html

class B : public Base { public: void f() override {} };
来源：http://hz.sufxvd.cn/gtapmjtakq.html

[S43] C++：智能指针
来源：http://hz.sysykeji.top/gtiqxryegh.html

auto p = std::make_unique<int>(5);
来源：http://hz.guannengcc.top/gtadtjjcdd.html

[S44] C++：引用传参
来源：http://hz.fengsongda.top/gtxsezckbf.html

void inc(int &x) { ++x; }
来源：http://hz.hywenlv.cn/gthpfswsge.html

[S45] C++：lambda
来源：http://hz.nanxinkj.top/gtsybytmqa.html

auto add = [](int a, int b) { return a + b; };
来源：http://hz.jiagoushi.top/gtltvojraw.html

[S46] C++：函数模板
来源：http://hz.jinghuilouyu.cn/gtqoatxsnq.html

template <typename T> T maxv(T a, T b) { return a > b ? a : b; }
来源：http://hz.yvedp.cn/gtlybfkrbo.html

[S47] C++：结构化绑定遍历
来源：http://hz.cqqwz.cn/gttfcxakye.html

for (const auto &[k, v] : m) { std::cout << k << v; }
来源：http://hz.shuidangran.top/gtncmhvdob.html

[S48] C++：逐行读文件
来源：http://hz.fzhhl.top/gteypfptmu.html

std::ifstream in("a.txt");  std::string line;
来源：http://hz.daxiang520.top/gteuupgwat.html

while (std::getline(in, line)) { }
来源：http://hz.cdnleiting.top/gtpneijvsd.html

[S49] C++：写文件
来源：http://hz.birdmap.top/gtjqdtgeaw.html

std::ofstream out("a.txt");  out << "hi\n";
来源：http://hz.haohaochexian.top/gtisqqofai.html

[S50] C++：格式化数字
来源：http://hz.hfpthk.cn/gtlfakllej.html

std::ostringstream os;  os << std::fixed << std::setprecision(2) << 3.14159;
来源：http://hz.jinqigufen.top/gtvtfcmlgq.html

[S51] C++：显式类型转换
来源：http://hz.wangdashe.top/gtthkikflg.html

static_cast<double>(a) / b
来源：http://hz.mhx1999.top/gtnnwyqbnk.html

[S52] C++：const 与 noexcept
来源：http://hz.xziqi.cn/gtjwxvtpci.html

int size() const noexcept { return n_; }
来源：http://hz.hammf.cn/gtpbimimpn.html

[S53] C++：移动语义
来源：http://hz.sxryk.cn/gttutvgekd.html

std::vector<int> w = std::move(v);
来源：http://hz.hnqzz.top/gtubqladbn.html

[S54] C++：异常处理
来源：http://hz.cheryme.top/gtthwptdnl.html

try { throw std::runtime_error("x"); } catch (const std::exception &e) { }
来源：http://hz.xingfuxueyuan.xyz/gthifnuqkb.html

[S55] C++：结构化绑定
来源：http://hz.hammf.cn/gtygydstpn.html

auto [a, b] = std::make_pair(1, 2);
来源：http://hz.shangyingyoupin.top/gtwshjezzv.html

[S56] C++：optional
来源：http://hz.ppjwa.cn/gtwpkasxgu.html

std::optional<int> o = 5;  if (o) { int v = *o; }
来源：http://hz.bjfxy.top/gtaztndcdz.html

[S57] C++：编译期常量
来源：http://hz.shanyushiyangkeji.top/gtwyjevkbw.html

constexpr int N = 10;
来源：http://hz.havefunace.top/gtqmritssh.html

[S58] C++：命名空间
来源：http://hz.ywan-chungtsiang.top/gtrbqrnqmv.html

namespace ns { int f() { return 1; } }
来源：http://hz.yangfankeji.com/gtcdcmqqsx.html

[S59] C++：静态断言
来源：http://hz.nanxinkj.top/gtaceeherx.html

static_assert(sizeof(int) == 4, "int 必须 4 字节");
来源：http://hz.cqqwz.cn/gtqqjbqfps.html

[S60] C++：遍历并删除元素
来源：http://hz.yj202588.top/gteecovjep.html

v.erase(std::remove_if(v.begin(), v.end(), [](int x) { return x < 0; }), v.end());
来源：http://hz.yangfankeji.com/gtjuvrwqfv.html

================================================================================
来源：http://hz.zhoulong.xyz/gtlhedltyf.html

T. 其他语言补充（Kotlin / Swift / Lua / Perl / Scala）
来源：http://hz.zhixingplan.top/gtcqeyfrsj.html

================================================================================
来源：http://hz.zhengqikj.top/gtbwctldos.html

[T01] Kotlin：Hello World
来源：http://hz.xylfe.cn/gtiqygdgne.html

println("Hello")
来源：http://hz.316326.xyz/gtzeqazexy.html

[T02] Kotlin：变量
来源：http://hz.wangshuangyany.cn/gtrkhcrkqj.html

val a = 1;  var b = 2        // val 只读，var 可变
来源：http://hz.fengsongda.top/gtdnbsykvf.html

[T03] Kotlin：字符串模板
来源：http://hz.hnqzz.top/gtvjijmqnk.html

"值: $b"
来源：http://hz.jinghuilouyu.cn/gtldlnqpzm.html

[T04] Kotlin：空安全
来源：http://hz.hnxiangtu.top/gtoyceeamp.html

val n: String? = null;  n?.length
来源：http://hz.zhaomingkeji.xyz/gtdzfvvsbs.html

[T05] Kotlin：when 表达式
来源：http://hz.gaohongyu789.top/gtvitlrlkm.html

val s = when (x) { 1 -> "一" else -> "其他" }   // 多分支时每个分支单独一行
来源：http://hz.yueranfly.top/gtmkayrjxg.html

[T06] Kotlin：集合映射
来源：http://hz.ydzc1.top/gtrzwuneab.html

listOf(1, 2, 3).map { it * 2 }
来源：http://hz.quarkkingdee.top/gtjsltzycv.html

[T07] Kotlin：集合过滤
来源：http://hz.hnqzz.top/gttquolhzs.html

listOf(1, 2, 3).filter { it > 1 }
来源：http://hz.fengsongda.top/gtdzgtgimx.html

[T08] Kotlin：数据类
来源：http://hz.sweek.top/gtlofsxbmk.html

data class User(val name: String, val age: Int)
来源：http://hz.daria6918.cn/gtvqafqixu.html

[T09] Kotlin：扩展函数
来源：http://hz.pycfn.com/gtphocyahn.html

fun String.exclaim() = this + "!"
来源：http://hz.yj20258.top/gtwkzdnimb.html

[T10] Kotlin：默认参数
来源：http://hz.wangshuangyany.cn/gtwgsmqetk.html

fun greet(name: String = "World") = "Hi $name"
来源：http://hz.cdnleiting.top/gtyxvsqyxe.html

[T11] Kotlin：协程
来源：http://hz.zhijiandao.cn/gthefhofyk.html

GlobalScope.launch { delay(1000); println("done") }
来源：http://hz.pengpengdd.cyou/gttlfxhghu.html

[T12] Kotlin：解构声明
来源：http://hz.zhixingplan.top/gtwvetyuqa.html

val (a, b) = Pair(1, 2)
来源：http://hz.guannengcc.top/gtqxlktuxl.html

[T13] Kotlin：只读 Map
来源：http://hz.smart0.xyz/gtzqaxhbpc.html

val m = mapOf("a" to 1)
来源：http://hz.jinqigfzy.top/gtslvmlygd.html

[T14] Kotlin：循环
来源：http://hz.cashguo.top/gtjqaksznp.html

for (i in 1..10) println(i)
来源：http://hz.yj202588.top/gtvyxnebyk.html

[T15] Kotlin：接口
来源：http://hz.gogol.net.cn/gtvfbtkdut.html

interface Shape { fun area(): Double }
来源：http://hz.xziqi.cn/gtapilfuzc.html

[T16] Swift：Hello World
来源：http://hz.aizwys.cn/gtepxcmjhv.html

print("Hello")
来源：http://hz.316326.xyz/gtqlhrccvt.html

[T17] Swift：变量与常量
来源：http://hz.shzxlz.cn/gtmgxvnhts.html

var a = 1;  let b = 2
来源：http://hz.ydzc1.top/gtlsbairjp.html

[T18] Swift：字符串插值
来源：http://hz.guowangkeji.top/gttdqdpaym.html

"值: \(b)"
来源：http://hz.yonumen.top/gtemcwazbr.html

[T19] Swift：可选绑定
来源：http://hz.kuanghao11.cn/gtaonpjiks.html

if let n = opt { print(n) }
来源：http://hz.cheryme.top/gtuzqtnmhm.html

[T20] Swift：数组操作
来源：http://hz.jinqigfzy.top/gtabcswpxn.html

var a = [1, 2, 3];  a.append(4)
来源：http://hz.gogol.net.cn/gtsgnjvkpq.html

[T21] Swift：遍历
来源：http://hz.ywan-chungtsiang.top/gtlrsdkblk.html

for x in a { print(x) }
来源：http://hz.jlsjyb.cn/gtonffuktb.html

[T22] Swift：字典
来源：http://hz.redwolf501.top/gtphgcbljn.html

var d = ["a": 1];  d["b"] = 2
来源：http://hz.bjfxy.top/gtastwufny.html

[T23] Swift：函数
来源：http://hz.hongshengwenyu.top/gtstxfgvtd.html

func add(_ a: Int, _ b: Int) -> Int { a + b }
来源：http://hz.zycfv.cn/gtoqgyjzgq.html

[T24] Swift：闭包
来源：http://hz.pycfn.com/gtlitlzkzz.html

let f = { (x: Int) -> Int in x * 2 }
来源：http://hz.hnqzz.top/gtsviggmqs.html

[T25] Swift：结构体
来源：http://hz.shanyushiyangtech.top/gtiulchdaz.html

struct P { var x: Int }
来源：http://hz.c1oappe.top/gtomymskfr.html

[T26] Swift：类与重写
来源：http://hz.jqgfzy.top/gtzaprrdis.html

class A: Base { override func f() {} }
来源：http://hz.chenzaomai.com/gtiburkxvg.html

[T27] Swift：错误处理
来源：http://hz.shanyushiyangtech.top/gtikvnulgu.html

do { try f() } catch { print(error) }
来源：http://hz.shzxlz.cn/gtqleztucz.html

[T28] Swift：枚举
来源：http://hz.tian-w.cn/gtqqtpzlxq.html

enum Color { case red, green }
来源：http://hz.pycfn.com/gtxlrtuibm.html

[T29] Swift：guard 提前返回
来源：http://hz.hammf.cn/gtqmtsmirn.html

guard let x = opt else { return }
来源：http://hz.dianchejie.cn/gtcfwsslxy.html

[T30] Swift：协议
来源：http://hz.dashuyun.cn/gtuozchoje.html

protocol Shape { func area() -> Double }
来源：http://hz.nwbrower.top/gtclxkrgdf.html

[T31] Lua：Hello World
来源：http://hz.fzhhl.top/gticfcrxxh.html

print("Hello")
来源：http://hz.sxryk.cn/gtikdsnket.html

[T32] Lua：局部变量
来源：http://hz.xuanzx.com/gtxiqxyxxk.html

local a = 1
来源：http://hz.guowangkeji.top/gtlzarghih.html

[T33] Lua：表（数组）
来源：http://hz.havefunace.top/gtsfgrqbaj.html

local t = {1, 2, 3};  t[4] = 4
来源：http://hz.gotoacloud.top/gtngyyxgme.html

[T34] Lua：遍历表
来源：http://hz.yonumen.top/gtilfbtslj.html

for i, v in ipairs(t) do print(i, v) end
来源：http://hz.yuanzhike.top/gtincexglg.html

[T35] Lua：字典表
来源：http://hz.zhiwuduotai.top/gtzlkiujxi.html

local d = { a = 1 };  d.b = 2
来源：http://hz.svipenyu.cn/gtezlyxrow.html

[T36] Lua：函数
来源：http://hz.iojbl.cn/gtbauqkfji.html

function add(a, b) return a + b end
来源：http://hz.dianchejie.cn/gtxrcjihil.html

[T37] Lua：字符串拼接
来源：http://hz.hysaishi.cn/gtjmexsmbc.html

"a" .. "b"
来源：http://hz.yj20258.top/gtjqcyiuqx.html

[T38] Lua：条件
来源：http://hz.hywenlv.cn/gtjsicjtyy.html

if x > 0 then print("正") end
来源：http://hz.xuanzx.com/gtkmokukie.html

[T39] Lua：模式匹配
来源：http://hz.zhixingplan.top/gtvgdlefdg.html

string.find(s, "%d+")
来源：http://hz.c1oappe.top/gtuaqjbhmb.html

[T40] Lua：元表
来源：http://hz.yongpay.top/gthbatmvay.html

setmetatable({}, { __index = base })
来源：http://hz.gzhubu.top/gtzjuvbzoe.html

[T41] Perl：Hello World
来源：http://hz.xingfuxueyuan.xyz/gtifmiufnb.html

print "Hello\n";
来源：http://hz.ybcxt.top/gtnkynvrek.html

[T42] Perl：变量类型
来源：http://hz.jiagoushi.top/gtelzzjzod.html

my $a = 1;  my @arr = (1, 2, 3);  my %h = (a => 1);
来源：http://hz.feifeiyinyue.top/gtumneymzx.html

[T43] Perl：字符串插值
来源：http://hz.shuidangran.top/gtneuatsnv.html

"值: $a"
来源：http://hz.daxiang520.top/gtfkqwxava.html

[T44] Perl：条件
来源：http://hz.shanyushiyangkeji.top/gtckkysios.html

if ($a > 0) { print "正"; }
来源：http://hz.chenjidiqi.icu/gtosvvbjaw.html

[T45] Perl：数组遍历
来源：http://hz.xylfe.cn/gtnyhjtdhn.html

for my $x (@arr) { print $x; }
来源：http://hz.wangdashe.top/gtokeapiaw.html

[T46] Perl：哈希操作
来源：http://hz.bjfxy.top/gtbqdbafnm.html

$h{b} = 2;  for my $k (keys %h) { print "$k=$h{$k}"; }
来源：http://hz.yonumen.top/gtffrhmush.html

[T47] Perl：正则捕获
来源：http://hz.dianchejie.cn/gtnuxfyift.html

if ($s =~ /(\d+)/) { print $1; }
来源：http://hz.shanyushiyangkeji.top/gtvlsutloj.html

[T48] Perl：正则替换
来源：http://hz.yj20258888.top/gtidiszsnt.html

$s =~ s/old/new/g;
来源：http://hz.ybcxt.top/gthtybdzws.html

[T49] Perl：函数
来源：http://hz.yj20258.top/gtstpbiabi.html

sub add { my ($a, $b) = @_; return $a + $b; }
来源：http://hz.hnxiangtu.top/gtbauyetsj.html

[T50] Perl：逐行读文件
来源：http://hz.kuanghao11.cn/gtivkyqxnw.html

open my $fh, "<", "a.txt" or die $!;
来源：http://hz.cashguo.top/gtrraygsio.html

while (my $line = <$fh>) { print $line; }
来源：http://hz.wangshuangyany.cn/gtaithjhsk.html

[T51] Scala：Hello World
来源：http://hz.zhiwuduotai.top/gtjkiedieh.html

println("Hello")
来源：http://hz.yangfankeji.com/gtovfdwmof.html

[T52] Scala：变量
来源：http://hz.yj20258.top/gtfdnpdvue.html

val a = 1;  var b = 2
来源：http://hz.yuanzhike.top/gthhilvetl.html

[T53] Scala：字符串插值
来源：http://hz.c1oappe.top/gtcmvbtilu.html

s"值: $b"
来源：http://hz.andypj.xyz/gtqviiojin.html

[T54] Scala：集合映射
来源：http://hz.sysykeji.top/gtnqyoisva.html

List(1, 2, 3).map(_ * 2)
来源：http://hz.jinqigfzy.top/gteotjxhwv.html

[T55] Scala：集合过滤
来源：http://hz.xziqi.cn/gtrfyxuzdc.html

List(1, 2, 3).filter(_ > 1)
来源：http://hz.kuanghao11.cn/gtgabjbmfx.html

[T56] Scala：样例类
来源：http://hz.chenlongwang.top/gtewdrrsho.html

case class User(name: String, age: Int)
来源：http://hz.cucudq.cn/gtfocfkwqx.html

[T57] Scala：模式匹配
来源：http://hz.zhoulong.xyz/gthqmbfsno.html

x match { case 1 => "一"; case _ => "其他" }
来源：http://hz.gotoacloud.top/gtksslujex.html

[T58] Scala：函数定义
来源：http://hz.yj20258888.top/gtkyewckpu.html

def add(a: Int, b: Int): Int = a + b
来源：http://hz.nanxuanxn.top/gtvsposqcf.html

[T59] Scala：循环
来源：http://hz.sysykeji.top/gtywvjhifz.html

for (i <- 1 to 10) println(i)
来源：http://hz.meibo888.top/gtvdmtoiul.html

[T60] Scala：折叠
来源：http://hz.quarkkingdee.top/gtsepjkchh.html

List(1, 2, 3).foldLeft(0)(_ + _)
来源：http://hz.zhijiandao.cn/gthpcpemwg.html

================================================================================
来源：http://hz.wangshuangyany.cn/gtucqtaqpy.html

U. 高频实用片段（Python / PHP / JavaScript 各 40 条）
来源：http://hz.zhoulong.xyz/gtatzrcgcf.html

================================================================================
来源：http://hz.cqqwz.cn/gtckreyhpt.html

[U01] Py：创建虚拟环境
来源：http://hz.yonumen.top/gtlnfviyrk.html

python -m venv .venv && source .venv/bin/activate
来源：http://hz.haohaochexian.top/gtxmgvzhmn.html

[U02] Py：导出 / 安装依赖
来源：http://hz.0kj1m.cn/gtbqhdfiom.html

pip freeze > requirements.txt;  pip install -r requirements.txt
来源：http://hz.hnqzz.top/gtnfhbxxfs.html

[U03] Py：加载 .env 配置
来源：http://hz.ybcxt.top/gtvqpecovt.html

from dotenv import load_dotenv; load_dotenv()
来源：http://hz.dianchejie.cn/gtqufmoipx.html

[U04] Py：变量调试打印
来源：http://hz.shangyingyoupin.top/gtoulljjhc.html

print(f"{x=}")            # 输出 x=值，Python 3.8+
来源：http://hz.jiagoushi.top/gtxtbpaajf.html

[U05] Py：列表去重且保序
来源：http://hz.yj202588.top/gtqtkhnbyd.html

list(dict.fromkeys(arr))
来源：http://hz.ydjk.org.cn/gttklcxmnb.html

[U06] Py：合并两个字典
来源：http://hz.jyoumei.cn/gtjreiwymb.html

{**a, **b}
来源：http://hz.chenjidiqi.icu/gtbvhfqdty.html

[U07] Py：反转字典键值
来源：http://hz.ydzc1.top/gtplauywwr.html

{v: k for k, v in d.items()}
来源：http://hz.jinqigfzy.top/gtqkghfrll.html

[U08] Py：展平二维列表
来源：http://hz.mhx1999.top/gtflwlrivp.html

[y for x in nested for y in x]
来源：http://hz.52xcode.cn/gtrphkimnc.html

[U09] Py：字典取最大值的键
来源：http://hz.yonumen.top/gtftcvfiwg.html

max(d, key=d.get)
来源：http://hz.jinqigfzy.top/gtwbkqujbh.html

[U10] Py：按值排序字典
来源：http://hz.hywenlv.cn/gttlcjqwxi.html

dict(sorted(d.items(), key=lambda kv: kv[1]))
来源：http://hz.zhongyouzk.top/gtqgxgpqsp.html

[U11] Py：生成器表达式
来源：http://hz.aibaodan.cn/gtswgicuzq.html

(x * 2 for x in arr)
来源：http://hz.tian-w.cn/gtlbteehwe.html

[U12] Py：取出现最多的 3 个元素
来源：http://hz.ehwqpu.com/gtpaprmwla.html

Counter(arr).most_common(3)
来源：http://hz.jianghu66.top/gtuklzjjel.html


<!-- 参考信息 -->