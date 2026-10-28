代发 wailian999

split -l 1000 big.log part_
来源：http://hz.jinqigfzy.top/gtmxrfknbn.html

[R74] 批量重命名
来源：http://hz.316326.xyz/gtfzdhtyoi.html

for f in *.jpeg; do mv "$f" "${f%.jpeg}.jpg"; done
来源：http://hz.yueranfly.top/gtxvldiglc.html

[R75] 导出环境变量
来源：http://hz.hfpthk.cn/gtfqvdmjtk.html

export PATH="$HOME/bin:$PATH"
来源：http://hz.sufxvd.cn/gtssdrqwvo.html

[R76] 使用临时文件
来源：http://hz.chenjidiqi.icu/gtxxjyqppb.html

tmp=$(mktemp); trap 'rm -f "$tmp"' EXIT
来源：http://hz.gotoacloud.top/gtptwdvkyg.html

[R77] 读取用户输入
来源：http://hz.xuetiantiany.cn/gttyrhlnta.html

read -rp "请输入: " ans
来源：http://hz.gaohongyu789.top/gtdcqsonpn.html

[R78] 交互式菜单
来源：http://hz.ppjwa.cn/gtclfgkqlq.html

select opt in a b c; do echo "$opt"; break; done
来源：http://hz.yvedp.cn/gtallcbzug.html

[R79] 解析命令行选项
来源：http://hz.tanke756.top/gtgxgjvcwx.html

while getopts "v:f:" o; do case $o in v) V=$OPTARG ;; f) F=$OPTARG ;; esac; done
来源：http://hz.316326.xyz/gtgyrptayn.html

[R80] 查看脚本执行耗时
来源：http://hz.cheryme.top/gtdonlezlo.html

time ./run.sh
来源：http://hz.yueranfly.top/gtzwxglqww.html

================================================================================
来源：http://hz.fengsongda.top/gtfbiyeucy.html

S. C / C++ 专题
来源：http://hz.fzhhl.top/gtbnmrgpfg.html

================================================================================
来源：http://hz.zhoulong.xyz/gtqchymnzo.html

[S01] C：Hello World
来源：http://hz.zdqjudy.top/gtoxaewdis.html

#include <stdio.h>
来源：http://hz.gotoacloud.top/gtpfenbtrn.html

int main(void) { printf("Hello\n"); return 0; }
来源：http://hz.sweek.top/gtfbrxwwjq.html

[S02] C：变量与格式化输出
来源：http://hz.meibo888.top/gtsybknqwh.html

int a = 10; printf("%d\n", a);
来源：http://hz.mhx1999.top/gtrakfffru.html

[S03] C：读入整数
来源：http://hz.fengsongda.top/gtwvsshscb.html

int x; scanf("%d", &x);
来源：http://hz.shzxlz.cn/gtbowwkdbi.html

[S04] C：字符串复制
来源：http://hz.sufxvd.cn/gttzfpvowl.html

char dst[32]; strcpy(dst, "hi");
来源：http://hz.cheryme.top/gtfhfctedn.html

[S05] C：字符串长度
来源：http://hz.shangyingyoupin.top/gtqqifdpgp.html

strlen(s)
来源：http://hz.hammf.cn/gtvksabulv.html

[S06] C：字符串比较
来源：http://hz.hammf.cn/gtlpitbocy.html

strcmp(a, b) == 0
来源：http://hz.shanyushiyangkeji.top/gtecwpxhqf.html

[S07] C：数组遍历求和
来源：http://hz.xinyue.icu/gtcdkqggby.html

for (int i = 0; i < n; i++) sum += a[i];
来源：http://hz.hnqzz.top/gtoukcnyqp.html

[S08] C：动态内存分配与释放
来源：http://hz.ybcxt.top/gtldcvidfq.html

int *p = malloc(sizeof(int) * n); ... free(p);
来源：http://hz.cdnleiting.top/gtybldtrik.html

[S09] C：结构体定义与初始化
来源：http://hz.xuetiantiany.cn/gtibqukswn.html

struct Point { int x, y; };  struct Point p = {1, 2};
来源：http://hz.dashuyun.cn/gthgarmlim.html

[S10] C：指针与解引用
来源：http://hz.hnxiangtu.top/gthcjcfzpw.html

int *p = &a;  *p = 5;
来源：http://hz.hnxiangtu.top/gtsebktypy.html

[S11] C：逐行读文件
来源：http://hz.xylfe.cn/gtlzhtdaqe.html

FILE *f = fopen("a.txt", "r");
来源：http://hz.chenlongwang.top/gtnzuoaqot.html

while (fgets(buf, sizeof buf, f)) { }
来源：http://hz.sufxvd.cn/gtkpoeajvs.html

fclose(f);
来源：http://hz.zhaomingkeji.xyz/gtkervrbqe.html

[S12] C：写文件
来源：http://hz.52xcode.cn/gtsbsevxrn.html

FILE *f = fopen("a.txt", "w");  fprintf(f, "hi\n");  fclose(f);
来源：http://hz.yonumen.top/gtgtxhylnf.html

[S13] C：宏定义
来源：http://hz.wangshuangyany.cn/gtnaqfecvy.html

#define MAX(a, b) ((a) > (b) ? (a) : (b))
来源：http://hz.sufxvd.cn/gtqzxvkqon.html

[S14] C：枚举
来源：http://hz.birdmap.top/gtbybituui.html

enum Color { RED, GREEN, BLUE };
来源：http://hz.jinyuanbaomall.cn/gtuxpjpbqk.html

[S15] C：类型转换
来源：http://hz.cashguo.top/gtzbxjohkb.html

(double) a / b
来源：http://hz.xingfuxueyuan.xyz/gtdmkmvjsx.html

[S16] C：位操作置位
来源：http://hz.dianchejie.cn/gtstcrjsio.html

x |= (1 << 3);
来源：http://hz.dashuyun.cn/gtdyznupfc.html

[S17] C：安全拼接字符串
来源：http://hz.cdnleiting.top/gttndqgfqn.html

snprintf(buf, sizeof buf, "%s%s", a, b);
来源：http://hz.sxryk.cn/gteuyzkust.html

[S18] C：命令行参数
来源：http://hz.ydzc1.top/gtthmarnnd.html

int main(int argc, char **argv)
来源：http://hz.gotoacloud.top/gtejtpeuli.html

[S19] C：快速排序
来源：http://hz.jinyuanbaomall.cn/gtpbxvlcxy.html

qsort(a, n, sizeof(int), cmp);
来源：http://hz.gaohongyu789.top/gtvahpymgq.html

[S20] C：二分查找
来源：http://hz.daxiang520.top/gtafkbzemw.html

bsearch(&key, a, n, sizeof(int), cmp);
来源：http://hz.gzhubu.top/gtgvyaderc.html

[S21] C：字符类别判断
来源：http://hz.yuanzhike.top/gtvoosuodc.html

isdigit(c);  isalpha(c);  isspace(c);
来源：http://hz.bjfxy.top/gtwtdofbaj.html

[S22] C：字符串转数字
来源：http://hz.daxiang520.top/gthbjzrgbx.html

atoi("42");  strtod("3.14", NULL);
来源：http://hz.redwolf501.top/gtxszquhcq.html

[S23] C：随机数
来源：http://hz.cheryme.top/gtlgadmvdp.html

srand(time(NULL));  int r = rand() % 100;
来源：http://hz.chenzaomai.com/gtjnzcefdc.html

[S24] C：获取本地时间
来源：http://hz.dashuyun.cn/gtiijhwbvx.html

time_t t = time(NULL);  struct tm *tm = localtime(&t);
来源：http://hz.zdqjudy.top/gtygmwbdkw.html

[S25] C：内存拷贝
来源：http://hz.shanyushiyangtech.top/gtbhjbpzgz.html

memcpy(dst, src, n);
来源：http://hz.xingfuxueyuan.xyz/gteshjociv.html

[S26] C：内存清零
来源：http://hz.shuidangran.top/gtjqruwbpy.html

memset(a, 0, sizeof a);
来源：http://hz.zhengqikj.top/gtabfbfutc.html

[S27] C：定义常量
来源：http://hz.iojbl.cn/gtahrmkedz.html

const double PI = 3.14159;
来源：http://hz.c1oappe.top/gtdfdmchpz.html

[S28] C：静态变量
来源：http://hz.smart0.xyz/gtjdsuptpt.html

static int counter = 0;
来源：http://hz.jqgufenzy.top/gtvmuwxwie.html

[S29] C：变参函数
来源：http://hz.hnqzz.top/gtacnbyiok.html

va_list ap; va_start(ap, fmt); vprintf(fmt, ap); va_end(ap);
来源：http://hz.chenlongwang.top/gtcinaocih.html

[S30] C：头文件保护
来源：http://hz.daria6918.cn/gtupllsgny.html

#ifndef X_H
来源：http://hz.52xcode.cn/gtcikksufz.html

#define X_H
来源：http://hz.gotoacloud.top/gtatcqcddc.html

#endif
来源：http://hz.jinqigufen.top/gtyrzcexuk.html

[S31] C++：Hello World
来源：http://hz.guannengcc.top/gtdmvnedpc.html

#include <iostream>
来源：http://hz.shuidangran.top/gtiwdxmwlx.html

int main() { std::cout << "Hello\n"; }
来源：http://hz.daria6918.cn/gtayjjxzyy.html

[S32] C++：字符串
来源：http://hz.jyoumei.cn/gtbccozwhv.html

std::string s = "hi";  s += "!";
来源：http://hz.zhongyouzk.top/gtmkuqcoyp.html

[S33] C++：vector 增删
来源：http://hz.ydzc1.top/gtkwlhigdc.html

std::vector<int> v{1, 2, 3};  v.push_back(4);
来源：http://hz.yj20258888.top/gtuxrfovgk.html

[S34] C++：遍历 vector
来源：http://hz.yongpay.top/gtmtjsickz.html

for (auto &x : v) { std::cout << x; }
来源：http://hz.jqgufenzy.top/gttcrmhhtw.html

[S35] C++：map
来源：http://hz.yanxiufei.cn/gtncbefwap.html

std::map<std::string, int> m;  m["a"] = 1;
来源：http://hz.meibo888.top/gtejbdufbi.html

[S36] C++：unordered_map
来源：http://hz.xuanzx.com/gtifnmvgoi.html

std::unordered_map<std::string, int> m;  m["a"] = 1;
来源：http://hz.havefunace.top/gtlqczpbyb.html

[S37] C++：set
来源：http://hz.birdmap.top/gtitixksow.html

std::set<int> s{1, 2, 3};  s.insert(4);
来源：http://hz.cucudq.cn/gtpylgslgf.html

[S38] C++：排序
来源：http://hz.daxiang520.top/gtokpiliep.html

std::sort(v.begin(), v.end());
来源：http://hz.dianchejie.cn/gtoyrustvk.html

[S39] C++：自定义比较器排序
来源：http://hz.svipenyu.cn/gtvynydmfv.html

std::sort(v.begin(), v.end(), [](int a, int b) { return a > b; });
来源：http://hz.zhixingplan.top/gtpkkxpxqz.html

[S40] C++：查找元素
来源：http://hz.jqgfzy.top/gtgauccfiq.html

auto it = std::find(v.begin(), v.end(), 3);
来源：http://hz.nanxuanxn.top/gtooikwnsv.html

[S41] C++：类与构造函数
来源：http://hz.xingfuxueyuan.xyz/gtggriwnde.html

class A { public: A(int v) : x_(v) {} int get() const { return x_; } private: int x_; };
来源：http://hz.aibaodan.cn/gtkivjdwbb.html

[S42] C++：继承与虚函数
来源：http://hz.ydzc1.top/gtqxitddsj.html

class B : public Base { public: void f() override {} };
来源：http://hz.shanyushiyangkeji.top/gtewknkxvu.html

[S43] C++：智能指针
来源：http://hz.cashguo.top/gtypcjgtxv.html

auto p = std::make_unique<int>(5);
来源：http://hz.haohaochexian.top/gtotidmkag.html

[S44] C++：引用传参
来源：http://hz.pengpengdd.cyou/gtekhyaspm.html

void inc(int &x) { ++x; }
来源：http://hz.jianghu66.top/gtonfltzfi.html

[S45] C++：lambda
来源：http://hz.xingfuxueyuan.xyz/gtfsdhgiua.html

auto add = [](int a, int b) { return a + b; };
来源：http://hz.aizwys.cn/gthzkppjbn.html

[S46] C++：函数模板
来源：http://hz.ydjk.org.cn/gtaypzmsqg.html

template <typename T> T maxv(T a, T b) { return a > b ? a : b; }
来源：http://hz.zhixingplan.top/gthpydbtui.html

[S47] C++：结构化绑定遍历
来源：http://hz.nanxuanxn.top/gtjaechutv.html

for (const auto &[k, v] : m) { std::cout << k << v; }
来源：http://hz.ybcxt.top/gtcvdecfpf.html

[S48] C++：逐行读文件
来源：http://hz.shanyushiyangkeji.top/gtjxilefmp.html

std::ifstream in("a.txt");  std::string line;
来源：http://hz.jlsjyb.cn/gtztsbypdo.html

while (std::getline(in, line)) { }
来源：http://hz.jiagoushi.top/gtdgkdbexy.html

[S49] C++：写文件
来源：http://hz.ydzc1.top/gtxoqcwtot.html

std::ofstream out("a.txt");  out << "hi\n";
来源：http://hz.pengpengdd.cyou/gtyhiwknbz.html

[S50] C++：格式化数字
来源：http://hz.redwolf501.top/gteheuzieb.html

std::ostringstream os;  os << std::fixed << std::setprecision(2) << 3.14159;
来源：http://hz.xinyue.icu/gtkeqeuwak.html

[S51] C++：显式类型转换
来源：http://hz.jqgfzy.top/gtvpqhvxbw.html

static_cast<double>(a) / b
来源：http://hz.sxryk.cn/gtohltniqv.html

[S52] C++：const 与 noexcept
来源：http://hz.hfpthk.cn/gthxvwsmsi.html

int size() const noexcept { return n_; }
来源：http://hz.haohaochexian.top/gtqzfhunef.html

[S53] C++：移动语义
来源：http://hz.quarkkingdee.top/gtpjicmbcs.html

std::vector<int> w = std::move(v);
来源：http://hz.yangfankeji.com/gtwsszlmve.html

[S54] C++：异常处理
来源：http://hz.guannengcc.top/gtsqtggwcs.html

try { throw std::runtime_error("x"); } catch (const std::exception &e) { }
来源：http://hz.cucudq.cn/gtcgfznfsu.html

[S55] C++：结构化绑定
来源：http://hz.nanxuanxn.top/gtsvnjztls.html

auto [a, b] = std::make_pair(1, 2);
来源：http://hz.chenlongwang.top/gturcrseit.html

[S56] C++：optional
来源：http://hz.zhiwuduotai.top/gtemodgnxo.html

std::optional<int> o = 5;  if (o) { int v = *o; }
来源：http://hz.hnxiangtu.top/gtozatpcyf.html

[S57] C++：编译期常量
来源：http://hz.xziqi.cn/gtaqljgwed.html

constexpr int N = 10;
来源：http://hz.daria6918.cn/gtuwebvyom.html

[S58] C++：命名空间
来源：http://hz.sweek.top/gtypesupjj.html

namespace ns { int f() { return 1; } }
来源：http://hz.sysykeji.top/gtnetvsrly.html

[S59] C++：静态断言
来源：http://hz.zhijiandao.cn/gtfzhiwufg.html

static_assert(sizeof(int) == 4, "int 必须 4 字节");
来源：http://hz.gaohongyu789.top/gtjzybdyms.html

[S60] C++：遍历并删除元素
来源：http://hz.nanxuanxn.top/gtcxqwkdbl.html

v.erase(std::remove_if(v.begin(), v.end(), [](int x) { return x < 0; }), v.end());
来源：http://hz.shangyingyoupin.top/gtbbxtbxro.html

================================================================================
来源：http://hz.yj20258888.top/gtkwxciivv.html

T. 其他语言补充（Kotlin / Swift / Lua / Perl / Scala）
来源：http://hz.daxiang520.top/gtehccxilx.html

================================================================================
来源：http://hz.fengsongda.top/gtcobpdivv.html

[T01] Kotlin：Hello World
来源：http://hz.kuanghao11.cn/gtcfuomqif.html

println("Hello")
来源：http://hz.gaohongyu789.top/gtpeqcklbg.html

[T02] Kotlin：变量
来源：http://hz.pycfn.com/gtmwacnaau.html

val a = 1;  var b = 2        // val 只读，var 可变
来源：http://hz.meibo888.top/gtefxkgywn.html

[T03] Kotlin：字符串模板
来源：http://hz.hysaishi.cn/gtesoshlyz.html

"值: $b"
来源：http://hz.52xcode.cn/gtgqfdtjss.html

[T04] Kotlin：空安全
来源：http://hz.redwolf501.top/gtdwwpmbxa.html

val n: String? = null;  n?.length
来源：http://hz.tanke756.top/gtjpoduzjj.html

[T05] Kotlin：when 表达式
来源：http://hz.pengpengdd.cyou/gthgvbbndo.html

val s = when (x) { 1 -> "一" else -> "其他" }   // 多分支时每个分支单独一行
来源：http://hz.wangshuangyany.cn/gtpbgtzfwu.html

[T06] Kotlin：集合映射
来源：http://hz.316326.xyz/gtkydjqnbr.html

listOf(1, 2, 3).map { it * 2 }
来源：http://hz.cashguo.top/gtfjzhyfjs.html

[T07] Kotlin：集合过滤
来源：http://hz.yanxiufei.cn/gtndhifqsu.html

listOf(1, 2, 3).filter { it > 1 }
来源：http://hz.sxryk.cn/gtkxvgobyn.html

[T08] Kotlin：数据类
来源：http://hz.guowangkeji.top/gtwsfpajbc.html

data class User(val name: String, val age: Int)
来源：http://hz.yvedp.cn/gtxpywfklk.html

[T09] Kotlin：扩展函数
来源：http://hz.gaohongyu789.top/gtmhdnqzuc.html

fun String.exclaim() = this + "!"
来源：http://hz.jinqigufen.top/gtzlflunkw.html

[T10] Kotlin：默认参数
来源：http://hz.daxiang520.top/gtkqkwfwrh.html

fun greet(name: String = "World") = "Hi $name"
来源：http://hz.ehwqpu.com/gtwquuapkt.html

[T11] Kotlin：协程
来源：http://hz.hnqzz.top/gtppyjegwm.html

GlobalScope.launch { delay(1000); println("done") }
来源：http://hz.daria6918.cn/gtzzmuapsg.html

[T12] Kotlin：解构声明
来源：http://hz.zhijiandao.cn/gtihmbmxjw.html

val (a, b) = Pair(1, 2)
来源：http://hz.ybcxt.top/gtcumnmclx.html

[T13] Kotlin：只读 Map
来源：http://hz.ivvv.top/gtnemozavu.html

val m = mapOf("a" to 1)
来源：http://hz.chenjidiqi.icu/gtogfwonjj.html

[T14] Kotlin：循环
来源：http://hz.zhengqikj.top/gtzzrodtkd.html

for (i in 1..10) println(i)
来源：http://hz.daxiang520.top/gtgwwngvtm.html

[T15] Kotlin：接口
来源：http://hz.dashuyun.cn/gtmitghvgd.html

interface Shape { fun area(): Double }
来源：http://hz.hnxiangtu.top/gtcwtqsvis.html

[T16] Swift：Hello World
来源：http://hz.kuanghao11.cn/gtnfhkzjgn.html

print("Hello")
来源：http://hz.yj202588.top/gtncqlvnvs.html

[T17] Swift：变量与常量
来源：http://hz.pycfn.com/gttvmrnlwl.html

var a = 1;  let b = 2
来源：http://hz.gzhubu.top/gtrniypkmh.html

[T18] Swift：字符串插值
来源：http://hz.aizwys.cn/gticcxdagt.html

"值: \(b)"
来源：http://hz.xziqi.cn/gtkzpfnwwd.html

[T19] Swift：可选绑定
来源：http://hz.fengsongda.top/gtbbfrbotb.html

if let n = opt { print(n) }
来源：http://hz.hywenlv.cn/gtzkstsfyg.html

[T20] Swift：数组操作
来源：http://hz.xziqi.cn/gtsqqswywt.html

var a = [1, 2, 3];  a.append(4)
来源：http://hz.tianlin.xyz/gtaqgfjksd.html

[T21] Swift：遍历
来源：http://hz.yonumen.top/gtytkirkxv.html

for x in a { print(x) }
来源：http://hz.jqgfzy.top/gttyqajesl.html

[T22] Swift：字典
来源：http://hz.jyoumei.cn/gtcnbqfogs.html

var d = ["a": 1];  d["b"] = 2
来源：http://hz.redwolf501.top/gtuebmiwgw.html

[T23] Swift：函数
来源：http://hz.cheryme.top/gtwelyuhbn.html

func add(_ a: Int, _ b: Int) -> Int { a + b }
来源：http://hz.yj20258.top/gtiruakwas.html

[T24] Swift：闭包
来源：http://hz.ywan-chungtsiang.top/gthoromozg.html

let f = { (x: Int) -> Int in x * 2 }
来源：http://hz.hongshengwenyu.top/gtrjusqipk.html

[T25] Swift：结构体
来源：http://hz.chenlongwang.top/gtzcethger.html

struct P { var x: Int }
来源：http://hz.xziqi.cn/gtvtgmsfgj.html

[T26] Swift：类与重写
来源：http://hz.svipenyu.cn/gtzzttczcn.html

class A: Base { override func f() {} }
来源：http://hz.zhongyouzk.top/gtlauwdzqg.html

[T27] Swift：错误处理
来源：http://hz.ybcxt.top/gtwcuqiiny.html

do { try f() } catch { print(error) }
来源：http://hz.pycfn.com/gtnyntcnvl.html

[T28] Swift：枚举
来源：http://hz.tanke756.top/gtsmbjskjk.html

enum Color { case red, green }
来源：http://hz.wangdashe.top/gtdydaalok.html

[T29] Swift：guard 提前返回
来源：http://hz.haohaochexian.top/gtaitvfrfe.html

guard let x = opt else { return }
来源：http://hz.jqgfzy.top/gttjhmegit.html

[T30] Swift：协议
来源：http://hz.yj20258888.top/gthvryburb.html

protocol Shape { func area() -> Double }
来源：http://hz.aizwys.cn/gtsiiejfmh.html

[T31] Lua：Hello World
来源：http://hz.jinqigufen.top/gtmrsvwsih.html

print("Hello")
来源：http://hz.jinqigfzy.top/gtptgqihpo.html

[T32] Lua：局部变量
来源：http://hz.hfpthk.cn/gtuncuquje.html

local a = 1
来源：http://hz.xziqi.cn/gtgfveyvev.html

[T33] Lua：表（数组）
来源：http://hz.shanyushiyangtech.top/gtlgukycbi.html

local t = {1, 2, 3};  t[4] = 4
来源：http://hz.tian-w.cn/gtozyoqfbn.html

[T34] Lua：遍历表
来源：http://hz.zhaomingkeji.xyz/gtpnxvdhcu.html

for i, v in ipairs(t) do print(i, v) end
来源：http://hz.jlsjyb.cn/gtzmdnstgo.html

[T35] Lua：字典表
来源：http://hz.hfpthk.cn/gtchqpmcqr.html

local d = { a = 1 };  d.b = 2
来源：http://hz.tian-w.cn/gteocdbtxz.html

[T36] Lua：函数
来源：http://hz.gotoacloud.top/gtbftdjtyy.html

function add(a, b) return a + b end
来源：http://hz.ppjwa.cn/gtojydormt.html

[T37] Lua：字符串拼接
来源：http://hz.cdnleiting.top/gtnoaixydm.html

"a" .. "b"
来源：http://hz.bjfxy.top/gtlhmopjqt.html

[T38] Lua：条件
来源：http://hz.sufxvd.cn/gtuzjudqcy.html

if x > 0 then print("正") end
来源：http://hz.aibaodan.cn/gtiwitgyij.html

[T39] Lua：模式匹配
来源：http://hz.ybcxt.top/gtbqcuqlrp.html

string.find(s, "%d+")
来源：http://hz.ydjk.org.cn/gtquhrlpzr.html

[T40] Lua：元表
来源：http://hz.fengsongda.top/gtyuxgfzud.html

setmetatable({}, { __index = base })
来源：http://hz.c1oappe.top/gtywmsqvqg.html

[T41] Perl：Hello World
来源：http://hz.ppjwa.cn/gtlkkcfyys.html

print "Hello\n";
来源：http://hz.xuanzx.com/gtrhldbuwj.html

[T42] Perl：变量类型
来源：http://hz.yj202588.top/gtxelpsgvq.html

my $a = 1;  my @arr = (1, 2, 3);  my %h = (a => 1);
来源：http://hz.svipenyu.cn/gtuvjsuotv.html

[T43] Perl：字符串插值
来源：http://hz.birdmap.top/gtdmrthnep.html

"值: $a"
来源：http://hz.jinqigfzy.top/gtkchdnzse.html

[T44] Perl：条件
来源：http://hz.zycfv.cn/gtssqppbei.html

if ($a > 0) { print "正"; }
来源：http://hz.yj20258.top/gtnynxiypl.html

[T45] Perl：数组遍历
来源：http://hz.cdnleiting.top/gtgahentsw.html

for my $x (@arr) { print $x; }
来源：http://hz.zhaomingkeji.xyz/gtwtszuhcw.html

[T46] Perl：哈希操作
来源：http://hz.yuanzhike.top/gtwbkzpwuy.html

$h{b} = 2;  for my $k (keys %h) { print "$k=$h{$k}"; }
来源：http://hz.ehwqpu.com/gtvetmmwog.html

[T47] Perl：正则捕获
来源：http://hz.xingfuxueyuan.xyz/gtlxxirbdb.html

if ($s =~ /(\d+)/) { print $1; }
来源：http://hz.c1oappe.top/gtxlcdgoow.html

[T48] Perl：正则替换
来源：http://hz.yvedp.cn/gtymcvrbmt.html

$s =~ s/old/new/g;
来源：http://hz.zhongyouzk.top/gtrqrqgqtl.html

[T49] Perl：函数
来源：http://hz.cheryme.top/gtaacsjhca.html

sub add { my ($a, $b) = @_; return $a + $b; }
来源：http://hz.jianghu66.top/gtxcqzixyb.html

[T50] Perl：逐行读文件
来源：http://hz.haohaochexian.top/gtlszgrvlw.html

open my $fh, "<", "a.txt" or die $!;
来源：http://hz.wangdashe.top/gttkqxbhsm.html

while (my $line = <$fh>) { print $line; }
来源：http://hz.feifeiyinyue.top/gtctcabrgt.html

[T51] Scala：Hello World
来源：http://hz.feifeiyinyue.top/gtizuoviok.html

println("Hello")
来源：http://hz.hammf.cn/gteniezjms.html

[T52] Scala：变量
来源：http://hz.haohaochexian.top/gtzmhnjsyi.html

val a = 1;  var b = 2
来源：http://hz.guowangkeji.top/gttoqgschd.html

[T53] Scala：字符串插值
来源：http://hz.nanxuanxn.top/gtfylxbggk.html

s"值: $b"
来源：http://hz.cdnleiting.top/gtbfvzzcds.html

[T54] Scala：集合映射
来源：http://hz.yuanzhike.top/gtthawffmc.html

List(1, 2, 3).map(_ * 2)
来源：http://hz.guannengcc.top/gthuycoefz.html

[T55] Scala：集合过滤
来源：http://hz.cucudq.cn/gtwaoxjfor.html

List(1, 2, 3).filter(_ > 1)
来源：http://hz.chenlongwang.top/gtffjujdzm.html

[T56] Scala：样例类
来源：http://hz.tianlin.xyz/gtvgmewiaz.html

case class User(name: String, age: Int)
来源：http://hz.jinghuilouyu.cn/gttlgzidjl.html

[T57] Scala：模式匹配
来源：http://hz.jqgufenzy.top/gtuwwrggul.html

x match { case 1 => "一"; case _ => "其他" }
来源：http://hz.jqgufenzy.top/gtvpqktmis.html

[T58] Scala：函数定义
来源：http://hz.zdqjudy.top/gtrgtvaknj.html

def add(a: Int, b: Int): Int = a + b
来源：http://hz.aibaodan.cn/gtemencntm.html

[T59] Scala：循环
来源：http://hz.svipenyu.cn/gtreinxoks.html

for (i <- 1 to 10) println(i)
来源：http://hz.sxryk.cn/gtnpjlegye.html

[T60] Scala：折叠
来源：http://hz.chenjidiqi.icu/gtnlgqaqka.html

List(1, 2, 3).foldLeft(0)(_ + _)
来源：http://hz.yonumen.top/gtwuhemdxp.html

================================================================================
来源：http://hz.feifeiyinyue.top/gtsfwcgeuc.html

U. 高频实用片段（Python / PHP / JavaScript 各 40 条）
来源：http://hz.jyoumei.cn/gtpsfnjmgp.html

================================================================================
来源：http://hz.nwbrower.top/gtqyfelhzc.html

[U01] Py：创建虚拟环境
来源：http://hz.ywan-chungtsiang.top/gtzqdswuow.html

python -m venv .venv && source .venv/bin/activate
来源：http://hz.tanke756.top/gtulqncvwl.html

[U02] Py：导出 / 安装依赖
来源：http://hz.haohaochexian.top/gtokhcwago.html

pip freeze > requirements.txt;  pip install -r requirements.txt
来源：http://hz.birdmap.top/gtazrrnbvr.html

[U03] Py：加载 .env 配置
来源：http://hz.zhaomingkeji.xyz/gtumeamryq.html

from dotenv import load_dotenv; load_dotenv()
来源：http://hz.c1oappe.top/gtaotrsbgk.html

[U04] Py：变量调试打印
来源：http://hz.yongpay.top/gtnjxazpes.html

print(f"{x=}")            # 输出 x=值，Python 3.8+
来源：http://hz.haohaochexian.top/gtnldtkqpx.html

[U05] Py：列表去重且保序
来源：http://hz.xylfe.cn/gtsecocljo.html

list(dict.fromkeys(arr))
来源：http://hz.wangdashe.top/gtkurivnsp.html

[U06] Py：合并两个字典
来源：http://hz.cqqwz.cn/gtakyzbvfz.html

{**a, **b}
来源：http://hz.hongshengwenyu.top/gtumndmbwo.html

[U07] Py：反转字典键值
来源：http://hz.jinyuanbaomall.cn/gteldpkbos.html

{v: k for k, v in d.items()}
来源：http://hz.cashguo.top/gtkcnmgjnc.html

[U08] Py：展平二维列表
来源：http://hz.jqgufenzy.top/gtkrslvfde.html

[y for x in nested for y in x]
来源：http://hz.guowangkeji.top/gtdllpeezu.html

[U09] Py：字典取最大值的键
来源：http://hz.snrcjt.cn/gtzcozucgj.html

max(d, key=d.get)
来源：http://hz.jinghuilouyu.cn/gtkezfptnr.html

[U10] Py：按值排序字典
来源：http://hz.daxiang520.top/gtowqpibrx.html

dict(sorted(d.items(), key=lambda kv: kv[1]))
来源：http://hz.daxiang520.top/gtffknovge.html

[U11] Py：生成器表达式
来源：http://hz.daria6918.cn/gtxzelfnbx.html

(x * 2 for x in arr)
来源：http://hz.jinghuilouyu.cn/gtutemcsry.html

[U12] Py：取出现最多的 3 个元素
来源：http://hz.52xcode.cn/gtdzcfekny.html

Counter(arr).most_common(3)
来源：http://hz.jqgfzy.top/gtkedrvhcy.html

[U13] Py：固定长度队列
来源：http://hz.ydzc1.top/gtfhcppbcy.html

deque(maxlen=10)
来源：http://hz.aibaodan.cn/gtvzcxxfkw.html

[U14] Py：分组收集到列表
来源：http://hz.zhongyouzk.top/gtjbkuyucz.html

defaultdict(list)
来源：http://hz.jiagoushi.top/gtdwqhfcpw.html


<!-- 参考信息 -->