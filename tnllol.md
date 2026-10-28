代发 wailian999

export PATH="$HOME/bin:$PATH"
来源：http://hz.aizwys.cn/gtjngynphl.html

[R76] 使用临时文件
来源：http://hz.zhaomingkeji.xyz/gtmsieoqev.html

tmp=$(mktemp); trap 'rm -f "$tmp"' EXIT
来源：http://hz.aibaodan.cn/gtcoqllvyn.html

[R77] 读取用户输入
来源：http://hz.cqqwz.cn/gtnuizcszw.html

read -rp "请输入: " ans
来源：http://hz.sysykeji.top/gtpzdxhzia.html

[R78] 交互式菜单
来源：http://hz.dianchejie.cn/gtkgpobwel.html

select opt in a b c; do echo "$opt"; break; done
来源：http://hz.chenzaomai.com/gtcbhdzify.html

[R79] 解析命令行选项
来源：http://hz.shuidangran.top/gtwggpdfdo.html

while getopts "v:f:" o; do case $o in v) V=$OPTARG ;; f) F=$OPTARG ;; esac; done
来源：http://hz.xylfe.cn/gtqvrhuuiu.html

[R80] 查看脚本执行耗时
来源：http://hz.jinqigfzy.top/gtwromuwqp.html

time ./run.sh
来源：http://hz.jqgfzy.top/gtrhnljtve.html

================================================================================
来源：http://hz.sufxvd.cn/gtfnjpgmgl.html

S. C / C++ 专题
来源：http://hz.shangyingyoupin.top/gtrhgavmrb.html

================================================================================
来源：http://hz.zdqjudy.top/gtmixgdccc.html

[S01] C：Hello World
来源：http://hz.ywan-chungtsiang.top/gtrcraqimw.html

#include <stdio.h>
来源：http://hz.svipenyu.cn/gtlmvviypt.html

int main(void) { printf("Hello\n"); return 0; }
来源：http://hz.hysaishi.cn/gtjmxtffmd.html

[S02] C：变量与格式化输出
来源：http://hz.feifeiyinyue.top/gtgzpxzjow.html

int a = 10; printf("%d\n", a);
来源：http://hz.daria6918.cn/gtwvlzzitw.html

[S03] C：读入整数
来源：http://hz.zhiwuduotai.top/gtpzrmbvou.html

int x; scanf("%d", &x);
来源：http://hz.shuidangran.top/gtvuhlbzqd.html

[S04] C：字符串复制
来源：http://hz.xuanzx.com/gtudiwkjwk.html

char dst[32]; strcpy(dst, "hi");
来源：http://hz.hfpthk.cn/gtubxknfoq.html

[S05] C：字符串长度
来源：http://hz.yangfankeji.com/gtejebtxhl.html

strlen(s)
来源：http://hz.ydjk.org.cn/gtnkjyvnee.html

[S06] C：字符串比较
来源：http://hz.xylfe.cn/gtigymthbu.html

strcmp(a, b) == 0
来源：http://hz.shuidangran.top/gtvownqvae.html

[S07] C：数组遍历求和
来源：http://hz.chenlongwang.top/gthmwsrmlt.html

for (int i = 0; i < n; i++) sum += a[i];
来源：http://hz.vqdsnc.cn/gttbvukotz.html

[S08] C：动态内存分配与释放
来源：http://hz.316326.xyz/gtfitoxzfx.html

int *p = malloc(sizeof(int) * n); ... free(p);
来源：http://hz.zhijiandao.cn/gtjerbmwkb.html

[S09] C：结构体定义与初始化
来源：http://hz.zhixingplan.top/gtqbslzqak.html

struct Point { int x, y; };  struct Point p = {1, 2};
来源：http://hz.yuanzhike.top/gthadebqjc.html

[S10] C：指针与解引用
来源：http://hz.gaohongyu789.top/gtdachhkbq.html

int *p = &a;  *p = 5;
来源：http://hz.cqqwz.cn/gtogqorubg.html

[S11] C：逐行读文件
来源：http://hz.daria6918.cn/gtjeytwcpk.html

FILE *f = fopen("a.txt", "r");
来源：http://hz.vqdsnc.cn/gttzqivpbv.html

while (fgets(buf, sizeof buf, f)) { }
来源：http://hz.xziqi.cn/gtoeyrwdbu.html

fclose(f);
来源：http://hz.birdmap.top/gtkiobyvpc.html

[S12] C：写文件
来源：http://hz.zdqjudy.top/gtlnwwvncw.html

FILE *f = fopen("a.txt", "w");  fprintf(f, "hi\n");  fclose(f);
来源：http://hz.cashguo.top/gtytwdtfyp.html

[S13] C：宏定义
来源：http://hz.hywenlv.cn/gtzkhyhzcl.html

#define MAX(a, b) ((a) > (b) ? (a) : (b))
来源：http://hz.zdqjudy.top/gtacoxuivt.html

[S14] C：枚举
来源：http://hz.yuxming.cn/gtvvtolsnf.html

enum Color { RED, GREEN, BLUE };
来源：http://hz.iojbl.cn/gtotvigqhb.html

[S15] C：类型转换
来源：http://hz.xinyue.icu/gtsrponovu.html

(double) a / b
来源：http://hz.yuanzhike.top/gtynftzmay.html

[S16] C：位操作置位
来源：http://hz.aizwys.cn/gtayoipbqy.html

x |= (1 << 3);
来源：http://hz.svipenyu.cn/gtrcldjgii.html

[S17] C：安全拼接字符串
来源：http://hz.yuxming.cn/gtwvooilbz.html

snprintf(buf, sizeof buf, "%s%s", a, b);
来源：http://hz.ybcxt.top/gtvboirduu.html

[S18] C：命令行参数
来源：http://hz.xuetiantiany.cn/gtajfmgmqa.html

int main(int argc, char **argv)
来源：http://hz.guowangkeji.top/gttzvtlghg.html

[S19] C：快速排序
来源：http://hz.hongshengwenyu.top/gtzjgvctnh.html

qsort(a, n, sizeof(int), cmp);
来源：http://hz.hywenlv.cn/gtidxjvlta.html

[S20] C：二分查找
来源：http://hz.aibaodan.cn/gtjieaktiq.html

bsearch(&key, a, n, sizeof(int), cmp);
来源：http://hz.gzhubu.top/gtengnhbvy.html

[S21] C：字符类别判断
来源：http://hz.aizwys.cn/gtwdruhwow.html

isdigit(c);  isalpha(c);  isspace(c);
来源：http://hz.bjfxy.top/gtudztloxf.html

[S22] C：字符串转数字
来源：http://hz.andypj.xyz/gtiumqbtrm.html

atoi("42");  strtod("3.14", NULL);
来源：http://hz.jinqigufen.top/gtldfibkhw.html

[S23] C：随机数
来源：http://hz.nanxuanxn.top/gtardsvxkz.html

srand(time(NULL));  int r = rand() % 100;
来源：http://hz.chenlongwang.top/gthstbuakt.html

[S24] C：获取本地时间
来源：http://hz.xinyue.icu/gtenbfkqhw.html

time_t t = time(NULL);  struct tm *tm = localtime(&t);
来源：http://hz.ydzc1.top/gtwcmfhtwv.html

[S25] C：内存拷贝
来源：http://hz.yanxiufei.cn/gtilxivnmu.html

memcpy(dst, src, n);
来源：http://hz.ppjwa.cn/gtxxiqmueu.html

[S26] C：内存清零
来源：http://hz.xingfuxueyuan.xyz/gtgdstueza.html

memset(a, 0, sizeof a);
来源：http://hz.kuanghao11.cn/gtnczwbapp.html

[S27] C：定义常量
来源：http://hz.ehwqpu.com/gtngmeuyjh.html

const double PI = 3.14159;
来源：http://hz.xuanzx.com/gttstdijxl.html

[S28] C：静态变量
来源：http://hz.gotoacloud.top/gtvmezjnht.html

static int counter = 0;
来源：http://hz.sweek.top/gtfgygfniv.html

[S29] C：变参函数
来源：http://hz.zhongyouzk.top/gtfofgipbf.html

va_list ap; va_start(ap, fmt); vprintf(fmt, ap); va_end(ap);
来源：http://hz.feifeiyinyue.top/gtzbsbfzyq.html

[S30] C：头文件保护
来源：http://hz.haohaochexian.top/gtohytjkga.html

#ifndef X_H
来源：http://hz.ppjwa.cn/gtrinmarnu.html

#define X_H
来源：http://hz.nwbrower.top/gtpcpuyufk.html

#endif
来源：http://hz.jinqigufen.top/gtgrpxdlci.html

[S31] C++：Hello World
来源：http://hz.yvedp.cn/gtfqklavvt.html

#include <iostream>
来源：http://hz.gogol.net.cn/gtzzqdckzm.html

int main() { std::cout << "Hello\n"; }
来源：http://hz.nanxinkj.top/gtxzxkxphp.html

[S32] C++：字符串
来源：http://hz.xingfuxueyuan.xyz/gtnnkyuskk.html

std::string s = "hi";  s += "!";
来源：http://hz.zycfv.cn/gtywgwngol.html

[S33] C++：vector 增删
来源：http://hz.wangdashe.top/gtnjtfturg.html

std::vector<int> v{1, 2, 3};  v.push_back(4);
来源：http://hz.iojbl.cn/gtyiuriiaf.html

[S34] C++：遍历 vector
来源：http://hz.sufxvd.cn/gtbaqquopl.html

for (auto &x : v) { std::cout << x; }
来源：http://hz.52xcode.cn/gtmvylxhcz.html

[S35] C++：map
来源：http://hz.ywan-chungtsiang.top/gtategcrpy.html

std::map<std::string, int> m;  m["a"] = 1;
来源：http://hz.hnxiangtu.top/gtmmyirvpg.html

[S36] C++：unordered_map
来源：http://hz.gogol.net.cn/gtscihovhp.html

std::unordered_map<std::string, int> m;  m["a"] = 1;
来源：http://hz.xuetiantiany.cn/gtpogppxzt.html

[S37] C++：set
来源：http://hz.jinqigufen.top/gtdjsvrhon.html

std::set<int> s{1, 2, 3};  s.insert(4);
来源：http://hz.dianchejie.cn/gtcmztesgu.html

[S38] C++：排序
来源：http://hz.jyoumei.cn/gtdthmueym.html

std::sort(v.begin(), v.end());
来源：http://hz.316326.xyz/gtvpyvyeuy.html

[S39] C++：自定义比较器排序
来源：http://hz.hfpthk.cn/gtasfnumsy.html

std::sort(v.begin(), v.end(), [](int a, int b) { return a > b; });
来源：http://hz.0kj1m.cn/gtlwikrxbe.html

[S40] C++：查找元素
来源：http://hz.sxryk.cn/gtrnupgayt.html

auto it = std::find(v.begin(), v.end(), 3);
来源：http://hz.fengsongda.top/gtraxrtufx.html

[S41] C++：类与构造函数
来源：http://hz.jinyuanbaomall.cn/gtzcrubesy.html

class A { public: A(int v) : x_(v) {} int get() const { return x_; } private: int x_; };
来源：http://hz.xylfe.cn/gtjrkusrez.html

[S42] C++：继承与虚函数
来源：http://hz.cdnleiting.top/gtndnzopcd.html

class B : public Base { public: void f() override {} };
来源：http://hz.jyoumei.cn/gtychzytfu.html

[S43] C++：智能指针
来源：http://hz.ppjwa.cn/gtqsfbolth.html

auto p = std::make_unique<int>(5);
来源：http://hz.haohaochexian.top/gtvchssses.html

[S44] C++：引用传参
来源：http://hz.hnqzz.top/gtpgqgfoud.html

void inc(int &x) { ++x; }
来源：http://hz.cqqwz.cn/gtswxgqccx.html

[S45] C++：lambda
来源：http://hz.cqqwz.cn/gtzxveigrc.html

auto add = [](int a, int b) { return a + b; };
来源：http://hz.kuanghao11.cn/gtikuhdpac.html

[S46] C++：函数模板
来源：http://hz.shzxlz.cn/gtsylzrkob.html

template <typename T> T maxv(T a, T b) { return a > b ? a : b; }
来源：http://hz.chenlongwang.top/gtjatwfbfl.html

[S47] C++：结构化绑定遍历
来源：http://hz.shanyushiyangtech.top/gtppihbgrt.html

for (const auto &[k, v] : m) { std::cout << k << v; }
来源：http://hz.wangshuangyany.cn/gthgaifjti.html

[S48] C++：逐行读文件
来源：http://hz.9152youxi.cn/gtwmvmipqe.html

std::ifstream in("a.txt");  std::string line;
来源：http://hz.vqdsnc.cn/gtvkicwugp.html

while (std::getline(in, line)) { }
来源：http://hz.shanyushiyangtech.top/gtzustibzv.html

[S49] C++：写文件
来源：http://hz.zhongyouzk.top/gtwbqwpqwp.html

std::ofstream out("a.txt");  out << "hi\n";
来源：http://hz.jqgfzy.top/gtqmwcrxzz.html

[S50] C++：格式化数字
来源：http://hz.haohaochexian.top/gtcqusogpe.html

std::ostringstream os;  os << std::fixed << std::setprecision(2) << 3.14159;
来源：http://hz.yonumen.top/gtzyhuduuj.html

[S51] C++：显式类型转换
来源：http://hz.iojbl.cn/gtvrsrplah.html

static_cast<double>(a) / b
来源：http://hz.jinqigfzy.top/gtbmtedklg.html

[S52] C++：const 与 noexcept
来源：http://hz.gzhubu.top/gtywrdjdbw.html

int size() const noexcept { return n_; }
来源：http://hz.cucudq.cn/gtydfkdkge.html

[S53] C++：移动语义
来源：http://hz.ydzc1.top/gttymnzonh.html

std::vector<int> w = std::move(v);
来源：http://hz.sufxvd.cn/gtuxzzulrb.html

[S54] C++：异常处理
来源：http://hz.jqgfzy.top/gtrbdkztpj.html

try { throw std::runtime_error("x"); } catch (const std::exception &e) { }
来源：http://hz.0kj1m.cn/gtaelnqreh.html

[S55] C++：结构化绑定
来源：http://hz.wangshuangyany.cn/gtqaqjtsrq.html

auto [a, b] = std::make_pair(1, 2);
来源：http://hz.zhixingplan.top/gtwpuwdqur.html

[S56] C++：optional
来源：http://hz.zhongyouzk.top/gtynxrowub.html

std::optional<int> o = 5;  if (o) { int v = *o; }
来源：http://hz.sxryk.cn/gtgyybwgfm.html

[S57] C++：编译期常量
来源：http://hz.shangyingyoupin.top/gtritsiyvw.html

constexpr int N = 10;
来源：http://hz.sysykeji.top/gttzndouop.html

[S58] C++：命名空间
来源：http://hz.daria6918.cn/gtmngkezff.html

namespace ns { int f() { return 1; } }
来源：http://hz.xingfuxueyuan.xyz/gtscogrdnw.html

[S59] C++：静态断言
来源：http://hz.cdnleiting.top/gtveiulkfc.html

static_assert(sizeof(int) == 4, "int 必须 4 字节");
来源：http://hz.hnxiangtu.top/gttgnqqhoo.html

[S60] C++：遍历并删除元素
来源：http://hz.zhongyouzk.top/gtsoutmopb.html

v.erase(std::remove_if(v.begin(), v.end(), [](int x) { return x < 0; }), v.end());
来源：http://hz.daxiang520.top/gtwnrmadak.html

================================================================================
来源：http://hz.chenjidiqi.icu/gtdctygegy.html

T. 其他语言补充（Kotlin / Swift / Lua / Perl / Scala）
来源：http://hz.gzhubu.top/gtkbbbkgbr.html

================================================================================
来源：http://hz.tanke756.top/gtcgdwdwfm.html

[T01] Kotlin：Hello World
来源：http://hz.kuanghao11.cn/gtcooheodg.html

println("Hello")
来源：http://hz.cheryme.top/gtlmidhkzp.html

[T02] Kotlin：变量
来源：http://hz.chenzaomai.com/gtltxandzc.html

val a = 1;  var b = 2        // val 只读，var 可变
来源：http://hz.c1oappe.top/gtneyazfnk.html

[T03] Kotlin：字符串模板
来源：http://hz.hongshengwenyu.top/gtbkqadwfd.html

"值: $b"
来源：http://hz.jianghu66.top/gtjdupfepv.html

[T04] Kotlin：空安全
来源：http://hz.ywan-chungtsiang.top/gtrrluciou.html

val n: String? = null;  n?.length
来源：http://hz.jyoumei.cn/gtnkvffkya.html

[T05] Kotlin：when 表达式
来源：http://hz.hongshengwenyu.top/gtzqhbuyqx.html

val s = when (x) { 1 -> "一" else -> "其他" }   // 多分支时每个分支单独一行
来源：http://hz.zhongyouzk.top/gtwnajgldo.html

[T06] Kotlin：集合映射
来源：http://hz.fzhhl.top/gtzybxvxik.html

listOf(1, 2, 3).map { it * 2 }
来源：http://hz.shzxlz.cn/gtryrbfoqc.html

[T07] Kotlin：集合过滤
来源：http://hz.andypj.xyz/gthsqkekjr.html

listOf(1, 2, 3).filter { it > 1 }
来源：http://hz.pengpengdd.cyou/gtbxnlcktm.html

[T08] Kotlin：数据类
来源：http://hz.xingfuxueyuan.xyz/gtcpoylzey.html

data class User(val name: String, val age: Int)
来源：http://hz.wangdashe.top/gtltrgmsic.html

[T09] Kotlin：扩展函数
来源：http://hz.wangdashe.top/gtkoawzudo.html

fun String.exclaim() = this + "!"
来源：http://hz.jinyuanbaomall.cn/gtgunwjfno.html

[T10] Kotlin：默认参数
来源：http://hz.nanxuanxn.top/gtxgxqbdcy.html

fun greet(name: String = "World") = "Hi $name"
来源：http://hz.guowangkeji.top/gtjvbqcfxd.html

[T11] Kotlin：协程
来源：http://hz.zhengqikj.top/gtncukocho.html

GlobalScope.launch { delay(1000); println("done") }
来源：http://hz.shanyushiyangkeji.top/gtzkzqtnbh.html

[T12] Kotlin：解构声明
来源：http://hz.haohaochexian.top/gtbklwecnx.html

val (a, b) = Pair(1, 2)
来源：http://hz.fengsongda.top/gtlbutgpoi.html

[T13] Kotlin：只读 Map
来源：http://hz.fzhhl.top/gtfmsmwufp.html

val m = mapOf("a" to 1)
来源：http://hz.smart0.xyz/gtnqqhrdsu.html

[T14] Kotlin：循环
来源：http://hz.daxiang520.top/gtttzafjqn.html

for (i in 1..10) println(i)
来源：http://hz.yuxming.cn/gtuvmzcmui.html

[T15] Kotlin：接口
来源：http://hz.chenlongwang.top/gtlmxxypjh.html

interface Shape { fun area(): Double }
来源：http://hz.svipenyu.cn/gtbdcauhzn.html

[T16] Swift：Hello World
来源：http://hz.xuetiantiany.cn/gtekposoxm.html

print("Hello")
来源：http://hz.cheryme.top/gtjyqsohtj.html

[T17] Swift：变量与常量
来源：http://hz.jinqigfzy.top/gtoseplqpr.html

var a = 1;  let b = 2
来源：http://hz.jqgufenzy.top/gtjxeimgib.html

[T18] Swift：字符串插值
来源：http://hz.xinyue.icu/gtrxuxyqtd.html

"值: \(b)"
来源：http://hz.shanyushiyangtech.top/gtnohtqmij.html

[T19] Swift：可选绑定
来源：http://hz.ybcxt.top/gtqfoykrlt.html

if let n = opt { print(n) }
来源：http://hz.xingfuxueyuan.xyz/gtymisrqnm.html

[T20] Swift：数组操作
来源：http://hz.feifeiyinyue.top/gthyejtspg.html

var a = [1, 2, 3];  a.append(4)
来源：http://hz.jinghuilouyu.cn/gtmwssynuh.html

[T21] Swift：遍历
来源：http://hz.zhengqikj.top/gtrenvonna.html

for x in a { print(x) }
来源：http://hz.shanyushiyangkeji.top/gtdktaoljb.html

[T22] Swift：字典
来源：http://hz.dashuyun.cn/gtwjhriaku.html

var d = ["a": 1];  d["b"] = 2
来源：http://hz.aizwys.cn/gtnbodesdz.html

[T23] Swift：函数
来源：http://hz.hongshengwenyu.top/gtfnklspvp.html

func add(_ a: Int, _ b: Int) -> Int { a + b }
来源：http://hz.xylfe.cn/gtadfaidtf.html

[T24] Swift：闭包
来源：http://hz.gzhubu.top/gtnwruihbv.html

let f = { (x: Int) -> Int in x * 2 }
来源：http://hz.yongpay.top/gtfadikoly.html

[T25] Swift：结构体
来源：http://hz.iojbl.cn/gtqjszipzt.html

struct P { var x: Int }
来源：http://hz.nwbrower.top/gtzbregwhy.html

[T26] Swift：类与重写
来源：http://hz.jqgfzy.top/gtvznjijgg.html

class A: Base { override func f() {} }
来源：http://hz.xylfe.cn/gtiogbebhd.html

[T27] Swift：错误处理
来源：http://hz.havefunace.top/gttccptclk.html

do { try f() } catch { print(error) }
来源：http://hz.tianlin.xyz/gteivgvoya.html

[T28] Swift：枚举
来源：http://hz.yuanzhike.top/gtmnlzucak.html

enum Color { case red, green }
来源：http://hz.guannengcc.top/gtuxqmatki.html

[T29] Swift：guard 提前返回
来源：http://hz.redwolf501.top/gtndxhyhxd.html

guard let x = opt else { return }
来源：http://hz.ydzc1.top/gtapzovnuf.html

[T30] Swift：协议
来源：http://hz.hfpthk.cn/gtuosobrqk.html

protocol Shape { func area() -> Double }
来源：http://hz.ehwqpu.com/gtgdseoreo.html

[T31] Lua：Hello World
来源：http://hz.bjfxy.top/gtkcgptfgh.html

print("Hello")
来源：http://hz.feifeiyinyue.top/gtlebftiel.html

[T32] Lua：局部变量
来源：http://hz.yueranfly.top/gtimljmvzc.html

local a = 1
来源：http://hz.meibo888.top/gthimlwcon.html

[T33] Lua：表（数组）
来源：http://hz.yj20258888.top/gtxuztzybo.html

local t = {1, 2, 3};  t[4] = 4
来源：http://hz.xingfuxueyuan.xyz/gtsvytgepc.html

[T34] Lua：遍历表
来源：http://hz.jinyuanbaomall.cn/gtckcjocjv.html

for i, v in ipairs(t) do print(i, v) end
来源：http://hz.hammf.cn/gtqcejoevy.html

[T35] Lua：字典表
来源：http://hz.smart0.xyz/gtsarrpoio.html

local d = { a = 1 };  d.b = 2
来源：http://hz.zhaomingkeji.xyz/gtmrvzhoim.html

[T36] Lua：函数
来源：http://hz.yj20258.top/gterqyefye.html

function add(a, b) return a + b end
来源：http://hz.ehwqpu.com/gtbjzrmbrv.html

[T37] Lua：字符串拼接
来源：http://hz.wangshuangyany.cn/gtaxbrexro.html

"a" .. "b"
来源：http://hz.quarkkingdee.top/gtqmtgxldl.html

[T38] Lua：条件
来源：http://hz.xingfuxueyuan.xyz/gtxcoiueur.html

if x > 0 then print("正") end
来源：http://hz.gaohongyu789.top/gtbrmoefti.html

[T39] Lua：模式匹配
来源：http://hz.dashuyun.cn/gtaiejncwr.html

string.find(s, "%d+")
来源：http://hz.aibaodan.cn/gtwulkprlm.html

[T40] Lua：元表
来源：http://hz.zycfv.cn/gtkhpycejt.html

setmetatable({}, { __index = base })
来源：http://hz.jinqigfzy.top/gtiqohfkds.html

[T41] Perl：Hello World
来源：http://hz.yangfankeji.com/gtewjadgbt.html

print "Hello\n";
来源：http://hz.yj202588.top/gtwkrwjnxs.html

[T42] Perl：变量类型
来源：http://hz.chenzaomai.com/gtvnyldpkf.html

my $a = 1;  my @arr = (1, 2, 3);  my %h = (a => 1);
来源：http://hz.dashuyun.cn/gtdexaukdr.html

[T43] Perl：字符串插值
来源：http://hz.yj20258.top/gtotczhpte.html

"值: $a"
来源：http://hz.chenjidiqi.icu/gtwjycedkm.html

[T44] Perl：条件
来源：http://hz.quarkkingdee.top/gtnbkdbzsa.html

if ($a > 0) { print "正"; }
来源：http://hz.meibo888.top/gtozxoqkou.html

[T45] Perl：数组遍历
来源：http://hz.hysaishi.cn/gtejlupmtv.html

for my $x (@arr) { print $x; }
来源：http://hz.snrcjt.cn/gtjxwvrvwx.html

[T46] Perl：哈希操作
来源：http://hz.meibo888.top/gtzjkkfucw.html

$h{b} = 2;  for my $k (keys %h) { print "$k=$h{$k}"; }
来源：http://hz.cqqwz.cn/gtsbbaeqmi.html

[T47] Perl：正则捕获
来源：http://hz.vqdsnc.cn/gttbapnhgm.html

if ($s =~ /(\d+)/) { print $1; }
来源：http://hz.jinqigufen.top/gtuyrfjkbe.html

[T48] Perl：正则替换
来源：http://hz.shanyushiyangtech.top/gtsoljpgjp.html

$s =~ s/old/new/g;
来源：http://hz.pengpengdd.cyou/gthcmkjzxn.html

[T49] Perl：函数
来源：http://hz.pengpengdd.cyou/gtiizxnwbb.html

sub add { my ($a, $b) = @_; return $a + $b; }
来源：http://hz.gzhubu.top/gtuopnqvhd.html

[T50] Perl：逐行读文件
来源：http://hz.sxryk.cn/gtzxnfkygu.html

open my $fh, "<", "a.txt" or die $!;
来源：http://hz.dashuyun.cn/gtjimyhgmm.html

while (my $line = <$fh>) { print $line; }
来源：http://hz.xylfe.cn/gtnastlqgz.html

[T51] Scala：Hello World
来源：http://hz.wangdashe.top/gteyiaofpi.html

println("Hello")
来源：http://hz.jinghuilouyu.cn/gtdanqtnvr.html

[T52] Scala：变量
来源：http://hz.wangshuangyany.cn/gtahjkfvov.html

val a = 1;  var b = 2
来源：http://hz.snrcjt.cn/gtabetzngu.html

[T53] Scala：字符串插值
来源：http://hz.vqdsnc.cn/gtpflkzojg.html

s"值: $b"
来源：http://hz.jiagoushi.top/gtifplwlxj.html

[T54] Scala：集合映射
来源：http://hz.jinqigufen.top/gthburhwpc.html

List(1, 2, 3).map(_ * 2)
来源：http://hz.daxiang520.top/gtcilmhhff.html

[T55] Scala：集合过滤
来源：http://hz.yanxiufei.cn/gtyrnpofyc.html

List(1, 2, 3).filter(_ > 1)
来源：http://hz.shanyushiyangkeji.top/gtqexsfjwm.html

[T56] Scala：样例类
来源：http://hz.zhengqikj.top/gttitviehk.html

case class User(name: String, age: Int)
来源：http://hz.jqgufenzy.top/gtnqymmifr.html

[T57] Scala：模式匹配
来源：http://hz.shzxlz.cn/gtmadcfnsv.html

x match { case 1 => "一"; case _ => "其他" }
来源：http://hz.52xcode.cn/gtaseplufu.html

[T58] Scala：函数定义
来源：http://hz.jqgfzy.top/gtbucdksrb.html

def add(a: Int, b: Int): Int = a + b
来源：http://hz.yanxiufei.cn/gtsguginyk.html

[T59] Scala：循环
来源：http://hz.ybcxt.top/gtmqtvnado.html

for (i <- 1 to 10) println(i)
来源：http://hz.hnxiangtu.top/gtkdnjigeg.html

[T60] Scala：折叠
来源：http://hz.aibaodan.cn/gtmfmwnaon.html

List(1, 2, 3).foldLeft(0)(_ + _)
来源：http://hz.vqdsnc.cn/gtadqcvejn.html

================================================================================
来源：http://hz.zhaomingkeji.xyz/gtpdjxdbei.html

U. 高频实用片段（Python / PHP / JavaScript 各 40 条）
来源：http://hz.svipenyu.cn/gtjwimjdaa.html

================================================================================
来源：http://hz.jinqigfzy.top/gtsgeejktk.html

[U01] Py：创建虚拟环境
来源：http://hz.andypj.xyz/gtjmflzfji.html

python -m venv .venv && source .venv/bin/activate
来源：http://hz.xingfuxueyuan.xyz/gtcardwprc.html

[U02] Py：导出 / 安装依赖
来源：http://hz.shuidangran.top/gtezxkzkak.html

pip freeze > requirements.txt;  pip install -r requirements.txt
来源：http://hz.hysaishi.cn/gtpoxbwpmj.html

[U03] Py：加载 .env 配置
来源：http://hz.hfpthk.cn/gtmihxhkeq.html

from dotenv import load_dotenv; load_dotenv()
来源：http://hz.yanxiufei.cn/gtfpxrlpnr.html

[U04] Py：变量调试打印
来源：http://hz.yvedp.cn/gtitivmcxu.html

print(f"{x=}")            # 输出 x=值，Python 3.8+
来源：http://hz.quarkkingdee.top/gtlburxsdt.html

[U05] Py：列表去重且保序
来源：http://hz.smart0.xyz/gtmsdgoxdb.html

list(dict.fromkeys(arr))
来源：http://hz.gotoacloud.top/gtingfnucv.html

[U06] Py：合并两个字典
来源：http://hz.nwbrower.top/gtaadohpvh.html

{**a, **b}
来源：http://hz.jqgufenzy.top/gtelixfzcm.html

[U07] Py：反转字典键值
来源：http://hz.yj20258888.top/gtvveccnnq.html

{v: k for k, v in d.items()}
来源：http://hz.ydzc1.top/gtuqhmwjqr.html

[U08] Py：展平二维列表
来源：http://hz.ehwqpu.com/gtnmjdbhjq.html

[y for x in nested for y in x]
来源：http://hz.ydjk.org.cn/gttthhgotn.html

[U09] Py：字典取最大值的键
来源：http://hz.shangyingyoupin.top/gtgzydemgl.html

max(d, key=d.get)
来源：http://hz.jinqigfzy.top/gtokxbcfcf.html

[U10] Py：按值排序字典
来源：http://hz.cqqwz.cn/gtqulibsnx.html

dict(sorted(d.items(), key=lambda kv: kv[1]))
来源：http://hz.sweek.top/gtxtisyrzz.html

[U11] Py：生成器表达式
来源：http://hz.jinyuanbaomall.cn/gtksqkqvvk.html

(x * 2 for x in arr)
来源：http://hz.shzxlz.cn/gtoharrvbs.html

[U12] Py：取出现最多的 3 个元素
来源：http://hz.sweek.top/gtgfjqlwjr.html

Counter(arr).most_common(3)
来源：http://hz.gogol.net.cn/gtedfogfbg.html

[U13] Py：固定长度队列
来源：http://hz.yuanzhike.top/gtxlravidx.html

deque(maxlen=10)
来源：http://hz.ivvv.top/gtygjjtspj.html

[U14] Py：分组收集到列表
来源：http://hz.daria6918.cn/gtmwmyxcbd.html

defaultdict(list)
来源：http://hz.yuxming.cn/gtobxgfseq.html

[U15] Py：高精度计时
来源：http://hz.sysykeji.top/gtzbncadmw.html

t = time.perf_counter()
来源：http://hz.hammf.cn/gtpvjykocl.html

[U16] Py：命令行参数解析
来源：http://hz.yj202588.top/gtksduyqpg.html

ap = argparse.ArgumentParser();  ap.add_argument("--name");  args = ap.parse_args()
来源：http://hz.xylfe.cn/gtyenosizm.html


<!-- 参考信息 -->