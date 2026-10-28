代发 wailian999

int main(void) { printf("Hello\n"); return 0; }
来源：http://hz.sxryk.cn/gtcqpyfrea.html

[S02] C：变量与格式化输出
来源：http://hz.jinqigfzy.top/gthtgfpnaz.html

int a = 10; printf("%d\n", a);
来源：http://hz.0kj1m.cn/gtclpaodtv.html

[S03] C：读入整数
来源：http://hz.xylfe.cn/gtctvsvpfb.html

int x; scanf("%d", &x);
来源：http://hz.zhixingplan.top/gtlgjqeltl.html

[S04] C：字符串复制
来源：http://hz.andypj.xyz/gtsgfsbcwg.html

char dst[32]; strcpy(dst, "hi");
来源：http://hz.xziqi.cn/gteffrkvgd.html

[S05] C：字符串长度
来源：http://hz.bjfxy.top/gthpqjqzsy.html

strlen(s)
来源：http://hz.zhixingplan.top/gtuwoesqtr.html

[S06] C：字符串比较
来源：http://hz.jqgfzy.top/gtxqbuvpcs.html

strcmp(a, b) == 0
来源：http://hz.daxiang520.top/gtfykqbnad.html

[S07] C：数组遍历求和
来源：http://hz.sysykeji.top/gtomknyflj.html

for (int i = 0; i < n; i++) sum += a[i];
来源：http://hz.wangdashe.top/gtdqyasnoe.html

[S08] C：动态内存分配与释放
来源：http://hz.feifeiyinyue.top/gtbeevwpdm.html

int *p = malloc(sizeof(int) * n); ... free(p);
来源：http://hz.birdmap.top/gtbcxuwyub.html

[S09] C：结构体定义与初始化
来源：http://hz.cucudq.cn/gtcymjxpyx.html

struct Point { int x, y; };  struct Point p = {1, 2};
来源：http://hz.bjfxy.top/gtajpjjmic.html

[S10] C：指针与解引用
来源：http://hz.yanxiufei.cn/gtycwowiqs.html

int *p = &a;  *p = 5;
来源：http://hz.iojbl.cn/gtmtijeqwe.html

[S11] C：逐行读文件
来源：http://hz.jqgfzy.top/gtbysozfjg.html

FILE *f = fopen("a.txt", "r");
来源：http://hz.tanke756.top/gtbymbeeuk.html

while (fgets(buf, sizeof buf, f)) { }
来源：http://hz.jinyuanbaomall.cn/gtskhzgejw.html

fclose(f);
来源：http://hz.andypj.xyz/gthyugvwha.html

[S12] C：写文件
来源：http://hz.cucudq.cn/gtxengjkkl.html

FILE *f = fopen("a.txt", "w");  fprintf(f, "hi\n");  fclose(f);
来源：http://hz.jqgufenzy.top/gtidrvduqf.html

[S13] C：宏定义
来源：http://hz.316326.xyz/gtutxizfto.html

#define MAX(a, b) ((a) > (b) ? (a) : (b))
来源：http://hz.cqqwz.cn/gtyoljtbyc.html

[S14] C：枚举
来源：http://hz.sxryk.cn/gtwqhprmjf.html

enum Color { RED, GREEN, BLUE };
来源：http://hz.birdmap.top/gtflnydedc.html

[S15] C：类型转换
来源：http://hz.yuxming.cn/gtwowtwoqv.html

(double) a / b
来源：http://hz.yongpay.top/gtyhskvcok.html

[S16] C：位操作置位
来源：http://hz.sweek.top/gtznjjgilv.html

x |= (1 << 3);
来源：http://hz.ppjwa.cn/gtapwqwfme.html

[S17] C：安全拼接字符串
来源：http://hz.shanyushiyangkeji.top/gtkfwngpei.html

snprintf(buf, sizeof buf, "%s%s", a, b);
来源：http://hz.haohaochexian.top/gtgvusbwvz.html

[S18] C：命令行参数
来源：http://hz.vqdsnc.cn/gtmbeuvwhv.html

int main(int argc, char **argv)
来源：http://hz.jinyuanbaomall.cn/gtooghptkk.html

[S19] C：快速排序
来源：http://hz.hammf.cn/gtiursewhw.html

qsort(a, n, sizeof(int), cmp);
来源：http://hz.havefunace.top/gtzuqxiups.html

[S20] C：二分查找
来源：http://hz.hnqzz.top/gtqxrgermx.html

bsearch(&key, a, n, sizeof(int), cmp);
来源：http://hz.zhoulong.xyz/gtivlgbkzm.html

[S21] C：字符类别判断
来源：http://hz.wangdashe.top/gtigsldtvo.html

isdigit(c);  isalpha(c);  isspace(c);
来源：http://hz.jqgufenzy.top/gtbzbwgonw.html

[S22] C：字符串转数字
来源：http://hz.tianlin.xyz/gtxtywstrd.html

atoi("42");  strtod("3.14", NULL);
来源：http://hz.ydzc1.top/gtmlpmbrpl.html

[S23] C：随机数
来源：http://hz.xziqi.cn/gtifcbdvhr.html

srand(time(NULL));  int r = rand() % 100;
来源：http://hz.hywenlv.cn/gtdnixhiui.html

[S24] C：获取本地时间
来源：http://hz.yangfankeji.com/gtfesxlpng.html

time_t t = time(NULL);  struct tm *tm = localtime(&t);
来源：http://hz.sysykeji.top/gtoyxycqkc.html

[S25] C：内存拷贝
来源：http://hz.iojbl.cn/gtekehxwpm.html

memcpy(dst, src, n);
来源：http://hz.bjfxy.top/gtzjazuccc.html

[S26] C：内存清零
来源：http://hz.ybcxt.top/gtqewqdbzj.html

memset(a, 0, sizeof a);
来源：http://hz.havefunace.top/gtxelsfhzr.html

[S27] C：定义常量
来源：http://hz.pycfn.com/gttqiqarsb.html

const double PI = 3.14159;
来源：http://hz.sxryk.cn/gthxqunhja.html

[S28] C：静态变量
来源：http://hz.guowangkeji.top/gtpeyiekrb.html

static int counter = 0;
来源：http://hz.gaohongyu789.top/gtpkxgkwty.html

[S29] C：变参函数
来源：http://hz.ydjk.org.cn/gtripryuxu.html

va_list ap; va_start(ap, fmt); vprintf(fmt, ap); va_end(ap);
来源：http://hz.jinghuilouyu.cn/gthwljtwkk.html

[S30] C：头文件保护
来源：http://hz.vqdsnc.cn/gtfktzvrml.html

#ifndef X_H
来源：http://hz.jinqigfzy.top/gtraqheege.html

#define X_H
来源：http://hz.gaohongyu789.top/gtvkwjovxw.html

#endif
来源：http://hz.xingfuxueyuan.xyz/gtloiwelhi.html

[S31] C++：Hello World
来源：http://hz.gaohongyu789.top/gtenzckgvh.html

#include <iostream>
来源：http://hz.ppjwa.cn/gtlraffrcj.html

int main() { std::cout << "Hello\n"; }
来源：http://hz.jinqigufen.top/gtpowvlkkm.html

[S32] C++：字符串
来源：http://hz.xingfuxueyuan.xyz/gtybyvilfp.html

std::string s = "hi";  s += "!";
来源：http://hz.yongpay.top/gtpjlmddzy.html

[S33] C++：vector 增删
来源：http://hz.fengsongda.top/gtqgtegtqg.html

std::vector<int> v{1, 2, 3};  v.push_back(4);
来源：http://hz.gaohongyu789.top/gtngyfzovd.html

[S34] C++：遍历 vector
来源：http://hz.hnqzz.top/gtlntwzski.html

for (auto &x : v) { std::cout << x; }
来源：http://hz.aibaodan.cn/gtbyrafsjd.html

[S35] C++：map
来源：http://hz.zycfv.cn/gtbdufvwim.html

std::map<std::string, int> m;  m["a"] = 1;
来源：http://hz.xuanzx.com/gtymxlfhby.html

[S36] C++：unordered_map
来源：http://hz.ydzc1.top/gtmwdheygd.html

std::unordered_map<std::string, int> m;  m["a"] = 1;
来源：http://hz.yj20258888.top/gtgfmjcuse.html

[S37] C++：set
来源：http://hz.zhaomingkeji.xyz/gtxrzdsivw.html

std::set<int> s{1, 2, 3};  s.insert(4);
来源：http://hz.cqqwz.cn/gtaxojwxmj.html

[S38] C++：排序
来源：http://hz.xuanzx.com/gtirederhd.html

std::sort(v.begin(), v.end());
来源：http://hz.sufxvd.cn/gtnowdpsrv.html

[S39] C++：自定义比较器排序
来源：http://hz.yuanzhike.top/gtcwpfilvt.html

std::sort(v.begin(), v.end(), [](int a, int b) { return a > b; });
来源：http://hz.yongpay.top/gtijvezlis.html

[S40] C++：查找元素
来源：http://hz.ydjk.org.cn/gtspyjhoqd.html

auto it = std::find(v.begin(), v.end(), 3);
来源：http://hz.zhijiandao.cn/gtpipukwqt.html

[S41] C++：类与构造函数
来源：http://hz.iojbl.cn/gtqsubxfqg.html

class A { public: A(int v) : x_(v) {} int get() const { return x_; } private: int x_; };
来源：http://hz.c1oappe.top/gtgcjfleco.html

[S42] C++：继承与虚函数
来源：http://hz.shzxlz.cn/gtepljjmul.html

class B : public Base { public: void f() override {} };
来源：http://hz.yanxiufei.cn/gteyoqbukq.html

[S43] C++：智能指针
来源：http://hz.jinyuanbaomall.cn/gtpthhafsc.html

auto p = std::make_unique<int>(5);
来源：http://hz.chenjidiqi.icu/gtztnklihe.html

[S44] C++：引用传参
来源：http://hz.nwbrower.top/gtopyclnne.html

void inc(int &x) { ++x; }
来源：http://hz.iojbl.cn/gtsjgltksl.html

[S45] C++：lambda
来源：http://hz.zhengqikj.top/gtdyghqvnu.html

auto add = [](int a, int b) { return a + b; };
来源：http://hz.ehwqpu.com/gtdvurhuer.html

[S46] C++：函数模板
来源：http://hz.hysaishi.cn/gtixbqadja.html

template <typename T> T maxv(T a, T b) { return a > b ? a : b; }
来源：http://hz.zhoulong.xyz/gtneiyongb.html

[S47] C++：结构化绑定遍历
来源：http://hz.0kj1m.cn/gtlsbdtbli.html

for (const auto &[k, v] : m) { std::cout << k << v; }
来源：http://hz.jqgufenzy.top/gtrdqrhvif.html

[S48] C++：逐行读文件
来源：http://hz.quarkkingdee.top/gtcbobufno.html

std::ifstream in("a.txt");  std::string line;
来源：http://hz.9152youxi.cn/gtphfaeyqn.html

while (std::getline(in, line)) { }
来源：http://hz.yonumen.top/gtyajvnomc.html

[S49] C++：写文件
来源：http://hz.yangfankeji.com/gtajnwfcfz.html

std::ofstream out("a.txt");  out << "hi\n";
来源：http://hz.316326.xyz/gtojrotmjz.html

[S50] C++：格式化数字
来源：http://hz.wangdashe.top/gtklomewxp.html

std::ostringstream os;  os << std::fixed << std::setprecision(2) << 3.14159;
来源：http://hz.c1oappe.top/gttdkgvudf.html

[S51] C++：显式类型转换
来源：http://hz.havefunace.top/gtyfrceijn.html

static_cast<double>(a) / b
来源：http://hz.xuanzx.com/gtboraxjck.html

[S52] C++：const 与 noexcept
来源：http://hz.aibaodan.cn/gtovwqhhzg.html

int size() const noexcept { return n_; }
来源：http://hz.zhongyouzk.top/gtjobcvhpd.html

[S53] C++：移动语义
来源：http://hz.jlsjyb.cn/gtqqqvvxuz.html

std::vector<int> w = std::move(v);
来源：http://hz.shuidangran.top/gtzngrcsiv.html

[S54] C++：异常处理
来源：http://hz.havefunace.top/gtnzirddgg.html

try { throw std::runtime_error("x"); } catch (const std::exception &e) { }
来源：http://hz.hammf.cn/gtzetyajey.html

[S55] C++：结构化绑定
来源：http://hz.daria6918.cn/gtfltobjce.html

auto [a, b] = std::make_pair(1, 2);
来源：http://hz.feifeiyinyue.top/gthjjbbjih.html

[S56] C++：optional
来源：http://hz.andypj.xyz/gtlgnhegod.html

std::optional<int> o = 5;  if (o) { int v = *o; }
来源：http://hz.ppjwa.cn/gtiwesoili.html

[S57] C++：编译期常量
来源：http://hz.tanke756.top/gtetgkjult.html

constexpr int N = 10;
来源：http://hz.pycfn.com/gtdoajacwu.html

[S58] C++：命名空间
来源：http://hz.tian-w.cn/gtpxqnpued.html

namespace ns { int f() { return 1; } }
来源：http://hz.jinqigfzy.top/gtfascjwnh.html

[S59] C++：静态断言
来源：http://hz.dianchejie.cn/gtbwjundnr.html

static_assert(sizeof(int) == 4, "int 必须 4 字节");
来源：http://hz.nwbrower.top/gtboclgzrn.html

[S60] C++：遍历并删除元素
来源：http://hz.yuanzhike.top/gtpfsqysve.html

v.erase(std::remove_if(v.begin(), v.end(), [](int x) { return x < 0; }), v.end());
来源：http://hz.haohaochexian.top/gtoycmaivr.html

================================================================================
来源：http://hz.0kj1m.cn/gtnljoivro.html

T. 其他语言补充（Kotlin / Swift / Lua / Perl / Scala）
来源：http://hz.sxryk.cn/gtwzhhzttg.html

================================================================================
来源：http://hz.xylfe.cn/gtdihusrpd.html

[T01] Kotlin：Hello World
来源：http://hz.sysykeji.top/gtvtgqsnge.html

println("Hello")
来源：http://hz.0kj1m.cn/gtysbztjqi.html

[T02] Kotlin：变量
来源：http://hz.kuanghao11.cn/gtkygknxqe.html

val a = 1;  var b = 2        // val 只读，var 可变
来源：http://hz.shanyushiyangtech.top/gtaytfjqsj.html

[T03] Kotlin：字符串模板
来源：http://hz.chenzaomai.com/gtoovckrhs.html

"值: $b"
来源：http://hz.nanxuanxn.top/gtzsohcvlo.html

[T04] Kotlin：空安全
来源：http://hz.zhijiandao.cn/gtximktfhx.html

val n: String? = null;  n?.length
来源：http://hz.xingfuxueyuan.xyz/gtobbznpha.html

[T05] Kotlin：when 表达式
来源：http://hz.guowangkeji.top/gtudlunijk.html

val s = when (x) { 1 -> "一" else -> "其他" }   // 多分支时每个分支单独一行
来源：http://hz.hnqzz.top/gtvifsgqrw.html

[T06] Kotlin：集合映射
来源：http://hz.mhx1999.top/gtnkffymas.html

listOf(1, 2, 3).map { it * 2 }
来源：http://hz.jiagoushi.top/gtmizqdmld.html

[T07] Kotlin：集合过滤
来源：http://hz.nanxuanxn.top/gtcziydboe.html

listOf(1, 2, 3).filter { it > 1 }
来源：http://hz.ydjk.org.cn/gttgtobnaq.html

[T08] Kotlin：数据类
来源：http://hz.quarkkingdee.top/gtixgibjgh.html

data class User(val name: String, val age: Int)
来源：http://hz.wangdashe.top/gtoesqmmbw.html

[T09] Kotlin：扩展函数
来源：http://hz.ybcxt.top/gtlilafxke.html

fun String.exclaim() = this + "!"
来源：http://hz.tanke756.top/gtdpbtabhu.html

[T10] Kotlin：默认参数
来源：http://hz.ywan-chungtsiang.top/gtgditqdyx.html

fun greet(name: String = "World") = "Hi $name"
来源：http://hz.wangshuangyany.cn/gtimzwzgkj.html

[T11] Kotlin：协程
来源：http://hz.jlsjyb.cn/gtzcggwbwz.html

GlobalScope.launch { delay(1000); println("done") }
来源：http://hz.jinqigufen.top/gtllwsmsaj.html

[T12] Kotlin：解构声明
来源：http://hz.zhaomingkeji.xyz/gtiktshaet.html

val (a, b) = Pair(1, 2)
来源：http://hz.yonumen.top/gtfgdvwqfl.html

[T13] Kotlin：只读 Map
来源：http://hz.guannengcc.top/gtjzeojmgt.html

val m = mapOf("a" to 1)
来源：http://hz.bjfxy.top/gtxttnvqme.html

[T14] Kotlin：循环
来源：http://hz.andypj.xyz/gtllhwhnai.html

for (i in 1..10) println(i)
来源：http://hz.aizwys.cn/gtmnslfvog.html

[T15] Kotlin：接口
来源：http://hz.ywan-chungtsiang.top/gteewhauzy.html

interface Shape { fun area(): Double }
来源：http://hz.52xcode.cn/gtkwkgycou.html

[T16] Swift：Hello World
来源：http://hz.cheryme.top/gtldotqvdm.html

print("Hello")
来源：http://hz.hysaishi.cn/gtcizjshfb.html

[T17] Swift：变量与常量
来源：http://hz.ehwqpu.com/gtyaaiejam.html

var a = 1;  let b = 2
来源：http://hz.wangdashe.top/gtfppkrkot.html

[T18] Swift：字符串插值
来源：http://hz.hywenlv.cn/gtpfqlvzjj.html

"值: \(b)"
来源：http://hz.c1oappe.top/gtzlfcjqqn.html

[T19] Swift：可选绑定
来源：http://hz.jinghuilouyu.cn/gttupkjsef.html

if let n = opt { print(n) }
来源：http://hz.xinyue.icu/gtmfesvksz.html

[T20] Swift：数组操作
来源：http://hz.cheryme.top/gtinribyng.html

var a = [1, 2, 3];  a.append(4)
来源：http://hz.jqgufenzy.top/gtuxxybytt.html

[T21] Swift：遍历
来源：http://hz.guannengcc.top/gthyywbmux.html

for x in a { print(x) }
来源：http://hz.hongshengwenyu.top/gtqvewchvs.html

[T22] Swift：字典
来源：http://hz.52xcode.cn/gtyybuwnqo.html

var d = ["a": 1];  d["b"] = 2
来源：http://hz.chenlongwang.top/gtdmsxyivn.html

[T23] Swift：函数
来源：http://hz.yj20258888.top/gtceulccvn.html

func add(_ a: Int, _ b: Int) -> Int { a + b }
来源：http://hz.zhixingplan.top/gtdgrtljvs.html

[T24] Swift：闭包
来源：http://hz.nanxuanxn.top/gtddlplczo.html

let f = { (x: Int) -> Int in x * 2 }
来源：http://hz.feifeiyinyue.top/gtdikhpccx.html

[T25] Swift：结构体
来源：http://hz.ehwqpu.com/gtvfugypvk.html

struct P { var x: Int }
来源：http://hz.cashguo.top/gtiqwarruq.html

[T26] Swift：类与重写
来源：http://hz.xingfuxueyuan.xyz/gtjiqjvpck.html

class A: Base { override func f() {} }
来源：http://hz.yueranfly.top/gtlnglrmlo.html

[T27] Swift：错误处理
来源：http://hz.ydjk.org.cn/gtllipatuv.html

do { try f() } catch { print(error) }
来源：http://hz.meibo888.top/gtmatjbbtf.html

[T28] Swift：枚举
来源：http://hz.birdmap.top/gtgpkzvfod.html

enum Color { case red, green }
来源：http://hz.daxiang520.top/gtznmrkjga.html

[T29] Swift：guard 提前返回
来源：http://hz.wangshuangyany.cn/gtzcocyfle.html

guard let x = opt else { return }
来源：http://hz.fengsongda.top/gtahsyjnxx.html

[T30] Swift：协议
来源：http://hz.zhaomingkeji.xyz/gtgludyehw.html

protocol Shape { func area() -> Double }
来源：http://hz.snrcjt.cn/gtbykgftse.html

[T31] Lua：Hello World
来源：http://hz.jqgufenzy.top/gtpmplhsqk.html

print("Hello")
来源：http://hz.yvedp.cn/gtnfvnlnfz.html

[T32] Lua：局部变量
来源：http://hz.wangdashe.top/gtxqmbikno.html

local a = 1
来源：http://hz.mhx1999.top/gtcnpezlwy.html

[T33] Lua：表（数组）
来源：http://hz.yuxming.cn/gtbhoiabcl.html

local t = {1, 2, 3};  t[4] = 4
来源：http://hz.zhixingplan.top/gttonlxahn.html

[T34] Lua：遍历表
来源：http://hz.quarkkingdee.top/gterfsotln.html

for i, v in ipairs(t) do print(i, v) end
来源：http://hz.ydjk.org.cn/gtyphfkggq.html

[T35] Lua：字典表
来源：http://hz.birdmap.top/gtuxulmyfs.html

local d = { a = 1 };  d.b = 2
来源：http://hz.mhx1999.top/gttekzybbu.html

[T36] Lua：函数
来源：http://hz.andypj.xyz/gtfniitcrp.html

function add(a, b) return a + b end
来源：http://hz.quarkkingdee.top/gtjuarelxz.html

[T37] Lua：字符串拼接
来源：http://hz.hnqzz.top/gtrecrinry.html

"a" .. "b"
来源：http://hz.jinqigfzy.top/gtnghebwmg.html

[T38] Lua：条件
来源：http://hz.daxiang520.top/gtkfvbvxpa.html

if x > 0 then print("正") end
来源：http://hz.0kj1m.cn/gtmjnryqxx.html

[T39] Lua：模式匹配
来源：http://hz.sysykeji.top/gtiesyminm.html

string.find(s, "%d+")
来源：http://hz.nanxinkj.top/gthpyapdjx.html

[T40] Lua：元表
来源：http://hz.jiagoushi.top/gtzcnjrgkp.html

setmetatable({}, { __index = base })
来源：http://hz.bjfxy.top/gtybxwugiq.html

[T41] Perl：Hello World
来源：http://hz.vqdsnc.cn/gtvdlbnqww.html

print "Hello\n";
来源：http://hz.cqqwz.cn/gtqpmnhgsi.html

[T42] Perl：变量类型
来源：http://hz.tianlin.xyz/gtmwpnjwsy.html

my $a = 1;  my @arr = (1, 2, 3);  my %h = (a => 1);
来源：http://hz.birdmap.top/gtnrfuphbg.html

[T43] Perl：字符串插值
来源：http://hz.aibaodan.cn/gtibkaommf.html

"值: $a"
来源：http://hz.wangdashe.top/gtuiqfflis.html

[T44] Perl：条件
来源：http://hz.sxryk.cn/gtjksjchqn.html

if ($a > 0) { print "正"; }
来源：http://hz.jlsjyb.cn/gteeqsodsb.html

[T45] Perl：数组遍历
来源：http://hz.dashuyun.cn/gtkepvrcyv.html

for my $x (@arr) { print $x; }
来源：http://hz.wangdashe.top/gtirpvciew.html

[T46] Perl：哈希操作
来源：http://hz.guannengcc.top/gtmgecogcp.html

$h{b} = 2;  for my $k (keys %h) { print "$k=$h{$k}"; }
来源：http://hz.birdmap.top/gtbmmlghjc.html

[T47] Perl：正则捕获
来源：http://hz.fengsongda.top/gttextjcok.html

if ($s =~ /(\d+)/) { print $1; }
来源：http://hz.hfpthk.cn/gtmfydhmbh.html

[T48] Perl：正则替换
来源：http://hz.zhoulong.xyz/gtdpxmnyry.html

$s =~ s/old/new/g;
来源：http://hz.zhaomingkeji.xyz/gtmealmtpy.html

[T49] Perl：函数
来源：http://hz.yj202588.top/gtwnzzzagz.html

sub add { my ($a, $b) = @_; return $a + $b; }
来源：http://hz.aizwys.cn/gtwondyzeh.html

[T50] Perl：逐行读文件
来源：http://hz.fengsongda.top/gtqetpiufz.html

open my $fh, "<", "a.txt" or die $!;
来源：http://hz.sweek.top/gtoviiifst.html

while (my $line = <$fh>) { print $line; }
来源：http://hz.hnqzz.top/gtlejutnck.html

[T51] Scala：Hello World
来源：http://hz.aizwys.cn/gtwmfpxdrf.html

println("Hello")
来源：http://hz.birdmap.top/gtxjwonowi.html

[T52] Scala：变量
来源：http://hz.jqgfzy.top/gtefcovevx.html

val a = 1;  var b = 2
来源：http://hz.jianghu66.top/gtnhhrmqgu.html

[T53] Scala：字符串插值
来源：http://hz.quarkkingdee.top/gtvklwdmlc.html

s"值: $b"
来源：http://hz.xziqi.cn/gtswsxeiyb.html

[T54] Scala：集合映射
来源：http://hz.chenzaomai.com/gtjarawvsl.html

List(1, 2, 3).map(_ * 2)
来源：http://hz.daria6918.cn/gterhujfmc.html

[T55] Scala：集合过滤
来源：http://hz.mhx1999.top/gtacikbpga.html

List(1, 2, 3).filter(_ > 1)
来源：http://hz.wangdashe.top/gtljkwqrmm.html

[T56] Scala：样例类
来源：http://hz.zhongyouzk.top/gtuclfohwp.html

case class User(name: String, age: Int)
来源：http://hz.cqqwz.cn/gtvlkmzfeq.html

[T57] Scala：模式匹配
来源：http://hz.aibaodan.cn/gtgsardpqk.html

x match { case 1 => "一"; case _ => "其他" }
来源：http://hz.c1oappe.top/gtzjbxzyto.html

[T58] Scala：函数定义
来源：http://hz.ybcxt.top/gtnzlhupjy.html

def add(a: Int, b: Int): Int = a + b
来源：http://hz.jinghuilouyu.cn/gtffeaobax.html

[T59] Scala：循环
来源：http://hz.shanyushiyangtech.top/gttiusmnsy.html

for (i <- 1 to 10) println(i)
来源：http://hz.pycfn.com/gtfyhpibqy.html

[T60] Scala：折叠
来源：http://hz.dashuyun.cn/gtjerwtjcb.html

List(1, 2, 3).foldLeft(0)(_ + _)
来源：http://hz.jinyuanbaomall.cn/gtmdjosjkb.html

================================================================================
来源：http://hz.jinqigufen.top/gtagzlxwrn.html

U. 高频实用片段（Python / PHP / JavaScript 各 40 条）
来源：http://hz.guowangkeji.top/gtiyyirjio.html

================================================================================
来源：http://hz.zhiwuduotai.top/gtxsxmxxdv.html

[U01] Py：创建虚拟环境
来源：http://hz.c1oappe.top/gtpdszxeiu.html

python -m venv .venv && source .venv/bin/activate
来源：http://hz.tanke756.top/gtiucpjbsg.html

[U02] Py：导出 / 安装依赖
来源：http://hz.yonumen.top/gtxggrzjnm.html

pip freeze > requirements.txt;  pip install -r requirements.txt
来源：http://hz.shanyushiyangkeji.top/gtimszwqsp.html

[U03] Py：加载 .env 配置
来源：http://hz.sysykeji.top/gtonzaidjs.html

from dotenv import load_dotenv; load_dotenv()
来源：http://hz.svipenyu.cn/gtzojtlrwr.html

[U04] Py：变量调试打印
来源：http://hz.xylfe.cn/gtnaujbkuq.html

print(f"{x=}")            # 输出 x=值，Python 3.8+
来源：http://hz.hammf.cn/gttwcxxteg.html

[U05] Py：列表去重且保序
来源：http://hz.redwolf501.top/gtxksmbdrn.html

list(dict.fromkeys(arr))
来源：http://hz.wangshuangyany.cn/gtkzlkrhjp.html

[U06] Py：合并两个字典
来源：http://hz.jiagoushi.top/gtybmzznhk.html

{**a, **b}
来源：http://hz.haohaochexian.top/gtzfjlrjon.html

[U07] Py：反转字典键值
来源：http://hz.nwbrower.top/gtowaqowdz.html

{v: k for k, v in d.items()}
来源：http://hz.jyoumei.cn/gtmzbdndlz.html

[U08] Py：展平二维列表
来源：http://hz.hnqzz.top/gtwcacdlmx.html

[y for x in nested for y in x]
来源：http://hz.cashguo.top/gthilicvxw.html

[U09] Py：字典取最大值的键
来源：http://hz.iojbl.cn/gtjhkefazx.html

max(d, key=d.get)
来源：http://hz.tanke756.top/gtglajosdp.html

[U10] Py：按值排序字典
来源：http://hz.yuxming.cn/gtckmevgkl.html

dict(sorted(d.items(), key=lambda kv: kv[1]))
来源：http://hz.hywenlv.cn/gtghsomtzc.html

[U11] Py：生成器表达式
来源：http://hz.0kj1m.cn/gtgzxrreju.html

(x * 2 for x in arr)
来源：http://hz.dashuyun.cn/gticfmvhse.html

[U12] Py：取出现最多的 3 个元素
来源：http://hz.ivvv.top/gtxfntbttw.html

Counter(arr).most_common(3)
来源：http://hz.hfpthk.cn/gtobllkaox.html

[U13] Py：固定长度队列
来源：http://hz.yj20258888.top/gtvedsdsyh.html

deque(maxlen=10)
来源：http://hz.cqqwz.cn/gtzvlzvygo.html

[U14] Py：分组收集到列表
来源：http://hz.xziqi.cn/gtcsfmtxac.html

defaultdict(list)
来源：http://hz.wangshuangyany.cn/gthofkwfva.html

[U15] Py：高精度计时
来源：http://hz.zhijiandao.cn/gtmldmeodc.html

t = time.perf_counter()
来源：http://hz.nanxinkj.top/gtwxumitie.html

[U16] Py：命令行参数解析
来源：http://hz.gotoacloud.top/gtoaapzwpf.html

ap = argparse.ArgumentParser();  ap.add_argument("--name");  args = ap.parse_args()
来源：http://hz.jiagoushi.top/gttetuwqls.html

[U17] Py：初始化日志
来源：http://hz.tian-w.cn/gtvtivcggh.html

logging.basicConfig(level=logging.INFO)
来源：http://hz.zdqjudy.top/gtljlfqwuo.html

[U18] Py：预编译正则
来源：http://hz.guowangkeji.top/gttonajhbe.html

pat = re.compile(r"\d+")
来源：http://hz.daria6918.cn/gtcncdmaik.html

[U19] Py：正则替换带回调
来源：http://hz.nanxuanxn.top/gttptryjdi.html

re.sub(r"\d+", lambda m: str(int(m.group()) * 2), s)
来源：http://hz.tianlin.xyz/gtesadpiwy.html

[U20] Py：缓存函数结果
来源：http://hz.quarkkingdee.top/gtceviqohd.html

@functools.lru_cache(maxsize=None)
来源：http://hz.smart0.xyz/gtdcvbqdgg.html

[U21] Py：自定义上下文管理器
来源：http://hz.yueranfly.top/gtgnefwgku.html

@contextlib.contextmanager
来源：http://hz.iojbl.cn/gtkxovazap.html

[U22] Py：矩阵转置
来源：http://hz.jianghu66.top/gtinwoovck.html

list(zip(*m))
来源：http://hz.xuetiantiany.cn/gtewicfkni.html

[U23] Py：分块读取大文件
来源：http://hz.yvedp.cn/gtkjdpnyob.html

for chunk in iter(lambda: f.read(8192), b""):
来源：http://hz.gzhubu.top/gtvauvcpnm.html

[U24] Py：路径操作
来源：http://hz.yongpay.top/gtpuizdfcm.html

Path("a/b.txt").parent.mkdir(parents=True, exist_ok=True)
来源：http://hz.wangdashe.top/gtzzavcbof.html


<!-- 参考信息 -->