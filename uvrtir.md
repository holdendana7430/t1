代发 wailian999

static int counter = 0;
来源：http://hz.iojbl.cn/gtppliorid.html

[S29] C：变参函数
来源：http://hz.nanxinkj.top/gtvyucxmrg.html

va_list ap; va_start(ap, fmt); vprintf(fmt, ap); va_end(ap);
来源：http://hz.bjfxy.top/gtpbshtudw.html

[S30] C：头文件保护
来源：http://hz.shanyushiyangkeji.top/gtoahacucy.html

#ifndef X_H
来源：http://hz.gogol.net.cn/gtjhiwvwrv.html

#define X_H
来源：http://hz.iojbl.cn/gtjpktunfc.html

#endif
来源：http://hz.hammf.cn/gtzoptmccv.html

[S31] C++：Hello World
来源：http://hz.snrcjt.cn/gtpomrewzr.html

#include <iostream>
来源：http://hz.hnxiangtu.top/gtzfmjqjuw.html

int main() { std::cout << "Hello\n"; }
来源：http://hz.nanxinkj.top/gtljdovnhi.html

[S32] C++：字符串
来源：http://hz.xylfe.cn/gtmashqvxv.html

std::string s = "hi";  s += "!";
来源：http://hz.cucudq.cn/gtllqfutgg.html

[S33] C++：vector 增删
来源：http://hz.mhx1999.top/gtetqknhgl.html

std::vector<int> v{1, 2, 3};  v.push_back(4);
来源：http://hz.yuanzhike.top/gtqmsmcdil.html

[S34] C++：遍历 vector
来源：http://hz.gogol.net.cn/gtpinriigj.html

for (auto &x : v) { std::cout << x; }
来源：http://hz.pycfn.com/gtfycfpfpg.html

[S35] C++：map
来源：http://hz.cdnleiting.top/gtfsupdgcs.html

std::map<std::string, int> m;  m["a"] = 1;
来源：http://hz.jyoumei.cn/gtamnnpoct.html

[S36] C++：unordered_map
来源：http://hz.vqdsnc.cn/gtyrdiowpo.html

std::unordered_map<std::string, int> m;  m["a"] = 1;
来源：http://hz.yongpay.top/gtskqbiqpd.html

[S37] C++：set
来源：http://hz.gogol.net.cn/gtvhctntaa.html

std::set<int> s{1, 2, 3};  s.insert(4);
来源：http://hz.aizwys.cn/gtihrokeva.html

[S38] C++：排序
来源：http://hz.jinyuanbaomall.cn/gtdlncptde.html

std::sort(v.begin(), v.end());
来源：http://hz.redwolf501.top/gtxgzvxirl.html

[S39] C++：自定义比较器排序
来源：http://hz.zhijiandao.cn/gtpqgrzmag.html

std::sort(v.begin(), v.end(), [](int a, int b) { return a > b; });
来源：http://hz.zhiwuduotai.top/gtnbbisago.html

[S40] C++：查找元素
来源：http://hz.yj202588.top/gtkxeqryck.html

auto it = std::find(v.begin(), v.end(), 3);
来源：http://hz.vqdsnc.cn/gtcmxlgtoh.html

[S41] C++：类与构造函数
来源：http://hz.yueranfly.top/gtbvdsxkre.html

class A { public: A(int v) : x_(v) {} int get() const { return x_; } private: int x_; };
来源：http://hz.xingfuxueyuan.xyz/gtkeuquksl.html

[S42] C++：继承与虚函数
来源：http://hz.wangdashe.top/gtkpdstwno.html

class B : public Base { public: void f() override {} };
来源：http://hz.meibo888.top/gtilrtyalx.html

[S43] C++：智能指针
来源：http://hz.zhiwuduotai.top/gtmnkwjwpp.html

auto p = std::make_unique<int>(5);
来源：http://hz.shanyushiyangtech.top/gtrzmjmceg.html

[S44] C++：引用传参
来源：http://hz.ehwqpu.com/gtuozylgxy.html

void inc(int &x) { ++x; }
来源：http://hz.zhengqikj.top/gtlwsgounr.html

[S45] C++：lambda
来源：http://hz.shanyushiyangkeji.top/gtetolsovj.html

auto add = [](int a, int b) { return a + b; };
来源：http://hz.nanxinkj.top/gtnsgmymng.html

[S46] C++：函数模板
来源：http://hz.wangshuangyany.cn/gtllsgptkt.html

template <typename T> T maxv(T a, T b) { return a > b ? a : b; }
来源：http://hz.nanxinkj.top/gtvclwpxir.html

[S47] C++：结构化绑定遍历
来源：http://hz.jiagoushi.top/gtjkftktun.html

for (const auto &[k, v] : m) { std::cout << k << v; }
来源：http://hz.shuidangran.top/gtoemuaeqh.html

[S48] C++：逐行读文件
来源：http://hz.hywenlv.cn/gtczvoxblj.html

std::ifstream in("a.txt");  std::string line;
来源：http://hz.gaohongyu789.top/gtaaslvmva.html

while (std::getline(in, line)) { }
来源：http://hz.vqdsnc.cn/gtxfxifznv.html

[S49] C++：写文件
来源：http://hz.andypj.xyz/gtfgmidogd.html

std::ofstream out("a.txt");  out << "hi\n";
来源：http://hz.zycfv.cn/gtkcbafzho.html

[S50] C++：格式化数字
来源：http://hz.pycfn.com/gtcatpfmje.html

std::ostringstream os;  os << std::fixed << std::setprecision(2) << 3.14159;
来源：http://hz.gogol.net.cn/gtgkjgzzbp.html

[S51] C++：显式类型转换
来源：http://hz.fengsongda.top/gthgbhsewf.html

static_cast<double>(a) / b
来源：http://hz.tian-w.cn/gtpwyczjns.html

[S52] C++：const 与 noexcept
来源：http://hz.yj202588.top/gtbjhqmbch.html

int size() const noexcept { return n_; }
来源：http://hz.cucudq.cn/gtozbrecai.html

[S53] C++：移动语义
来源：http://hz.nanxinkj.top/gtqxzhiemz.html

std::vector<int> w = std::move(v);
来源：http://hz.xziqi.cn/gteaqquwuj.html

[S54] C++：异常处理
来源：http://hz.jinqigfzy.top/gtrubgdfvp.html

try { throw std::runtime_error("x"); } catch (const std::exception &e) { }
来源：http://hz.wangdashe.top/gtzgiemygd.html

[S55] C++：结构化绑定
来源：http://hz.iojbl.cn/gtldwjdgqi.html

auto [a, b] = std::make_pair(1, 2);
来源：http://hz.xingfuxueyuan.xyz/gtsjcebomz.html

[S56] C++：optional
来源：http://hz.redwolf501.top/gtgjfookxc.html

std::optional<int> o = 5;  if (o) { int v = *o; }
来源：http://hz.gogol.net.cn/gtnavcyrsq.html

[S57] C++：编译期常量
来源：http://hz.jinyuanbaomall.cn/gtffyzvxbz.html

constexpr int N = 10;
来源：http://hz.chenlongwang.top/gthsoewayi.html

[S58] C++：命名空间
来源：http://hz.svipenyu.cn/gtcjqxiovi.html

namespace ns { int f() { return 1; } }
来源：http://hz.shangyingyoupin.top/gtepbnbqcb.html

[S59] C++：静态断言
来源：http://hz.daxiang520.top/gttyzthzds.html

static_assert(sizeof(int) == 4, "int 必须 4 字节");
来源：http://hz.sweek.top/gtvkrxdbya.html

[S60] C++：遍历并删除元素
来源：http://hz.jianghu66.top/gtnnawvotg.html

v.erase(std::remove_if(v.begin(), v.end(), [](int x) { return x < 0; }), v.end());
来源：http://hz.tianlin.xyz/gtyjytduej.html

================================================================================
来源：http://hz.zhoulong.xyz/gtyoqxshiz.html

T. 其他语言补充（Kotlin / Swift / Lua / Perl / Scala）
来源：http://hz.vqdsnc.cn/gtavcfszpx.html

================================================================================
来源：http://hz.chenlongwang.top/gtclzpmtug.html

[T01] Kotlin：Hello World
来源：http://hz.jqgfzy.top/gtecpezgvq.html

println("Hello")
来源：http://hz.gogol.net.cn/gtbonyyadk.html

[T02] Kotlin：变量
来源：http://hz.yuanzhike.top/gtqrqkktjk.html

val a = 1;  var b = 2        // val 只读，var 可变
来源：http://hz.hywenlv.cn/gtvutlffyp.html

[T03] Kotlin：字符串模板
来源：http://hz.andypj.xyz/gtijhqtdxj.html

"值: $b"
来源：http://hz.yuanzhike.top/gtnwgiurlf.html

[T04] Kotlin：空安全
来源：http://hz.0kj1m.cn/gtupytdqle.html

val n: String? = null;  n?.length
来源：http://hz.shanyushiyangtech.top/gtfvniufmp.html

[T05] Kotlin：when 表达式
来源：http://hz.yueranfly.top/gtvkmszqgv.html

val s = when (x) { 1 -> "一" else -> "其他" }   // 多分支时每个分支单独一行
来源：http://hz.zhixingplan.top/gtzdmocpde.html

[T06] Kotlin：集合映射
来源：http://hz.yangfankeji.com/gtvsylityq.html

listOf(1, 2, 3).map { it * 2 }
来源：http://hz.daria6918.cn/gtzppfcoxy.html

[T07] Kotlin：集合过滤
来源：http://hz.0kj1m.cn/gtzjuliprk.html

listOf(1, 2, 3).filter { it > 1 }
来源：http://hz.andypj.xyz/gtpcewkzuo.html

[T08] Kotlin：数据类
来源：http://hz.yonumen.top/gtzcoakryu.html

data class User(val name: String, val age: Int)
来源：http://hz.cqqwz.cn/gtjoaifltf.html

[T09] Kotlin：扩展函数
来源：http://hz.xylfe.cn/gtkxuscmoy.html

fun String.exclaim() = this + "!"
来源：http://hz.hysaishi.cn/gtsorsxpyq.html

[T10] Kotlin：默认参数
来源：http://hz.shanyushiyangkeji.top/gtdyvexrbo.html

fun greet(name: String = "World") = "Hi $name"
来源：http://hz.feifeiyinyue.top/gtlautllio.html

[T11] Kotlin：协程
来源：http://hz.xuanzx.com/gtkwlfxtcp.html

GlobalScope.launch { delay(1000); println("done") }
来源：http://hz.sufxvd.cn/gtukgsawtm.html

[T12] Kotlin：解构声明
来源：http://hz.redwolf501.top/gtbxiaunnm.html

val (a, b) = Pair(1, 2)
来源：http://hz.hammf.cn/gtobhmhnju.html

[T13] Kotlin：只读 Map
来源：http://hz.ydjk.org.cn/gtyownhkha.html

val m = mapOf("a" to 1)
来源：http://hz.ppjwa.cn/gtizraqjnz.html

[T14] Kotlin：循环
来源：http://hz.sysykeji.top/gttrkoydqo.html

for (i in 1..10) println(i)
来源：http://hz.shuidangran.top/gtyyayqehr.html

[T15] Kotlin：接口
来源：http://hz.hnqzz.top/gtoyabesdf.html

interface Shape { fun area(): Double }
来源：http://hz.meibo888.top/gtjkfuopma.html

[T16] Swift：Hello World
来源：http://hz.ywan-chungtsiang.top/gtreqjzniq.html

print("Hello")
来源：http://hz.fzhhl.top/gtdgvtvnlk.html

[T17] Swift：变量与常量
来源：http://hz.yueranfly.top/gtdzwgxjoj.html

var a = 1;  let b = 2
来源：http://hz.gogol.net.cn/gtraybvzsj.html

[T18] Swift：字符串插值
来源：http://hz.wangshuangyany.cn/gtxxzgtmlc.html

"值: \(b)"
来源：http://hz.jqgufenzy.top/gtbrguvhpo.html

[T19] Swift：可选绑定
来源：http://hz.guowangkeji.top/gtnlojllof.html

if let n = opt { print(n) }
来源：http://hz.tianlin.xyz/gtjduilqzu.html

[T20] Swift：数组操作
来源：http://hz.ydjk.org.cn/gtvfchjbxp.html

var a = [1, 2, 3];  a.append(4)
来源：http://hz.shuidangran.top/gthcdeidoj.html

[T21] Swift：遍历
来源：http://hz.shangyingyoupin.top/gtpubxukaq.html

for x in a { print(x) }
来源：http://hz.gzhubu.top/gtzrogoyhb.html

[T22] Swift：字典
来源：http://hz.zhaomingkeji.xyz/gtlzgsxphf.html

var d = ["a": 1];  d["b"] = 2
来源：http://hz.chenlongwang.top/gtxqmlrfxk.html

[T23] Swift：函数
来源：http://hz.hysaishi.cn/gtmigshdae.html

func add(_ a: Int, _ b: Int) -> Int { a + b }
来源：http://hz.cqqwz.cn/gtscospist.html

[T24] Swift：闭包
来源：http://hz.daria6918.cn/gtbrpcusrs.html

let f = { (x: Int) -> Int in x * 2 }
来源：http://hz.dianchejie.cn/gttwqepcvw.html

[T25] Swift：结构体
来源：http://hz.ehwqpu.com/gtbnjyvzgk.html

struct P { var x: Int }
来源：http://hz.shangyingyoupin.top/gtvbyruzug.html

[T26] Swift：类与重写
来源：http://hz.jqgfzy.top/gtgrsgqsso.html

class A: Base { override func f() {} }
来源：http://hz.daria6918.cn/gtqpmfvjmj.html

[T27] Swift：错误处理
来源：http://hz.ybcxt.top/gthijgwtbi.html

do { try f() } catch { print(error) }
来源：http://hz.c1oappe.top/gtgyhyqgge.html

[T28] Swift：枚举
来源：http://hz.yuxming.cn/gtrdkvnrch.html

enum Color { case red, green }
来源：http://hz.shanyushiyangtech.top/gtjwbsdwyr.html

[T29] Swift：guard 提前返回
来源：http://hz.tian-w.cn/gtxfmdnjgr.html

guard let x = opt else { return }
来源：http://hz.chenlongwang.top/gtspfhqniy.html

[T30] Swift：协议
来源：http://hz.yonumen.top/gtoygqqfnb.html

protocol Shape { func area() -> Double }
来源：http://hz.tian-w.cn/gtfwghfvzp.html

[T31] Lua：Hello World
来源：http://hz.vqdsnc.cn/gtvmeqlnmm.html

print("Hello")
来源：http://hz.vqdsnc.cn/gtwxgfflcn.html

[T32] Lua：局部变量
来源：http://hz.hywenlv.cn/gtbsxtdcxv.html

local a = 1
来源：http://hz.shangyingyoupin.top/gtovhetunp.html

[T33] Lua：表（数组）
来源：http://hz.nanxuanxn.top/gtjyacogps.html

local t = {1, 2, 3};  t[4] = 4
来源：http://hz.ydjk.org.cn/gtefolyref.html

[T34] Lua：遍历表
来源：http://hz.svipenyu.cn/gtitkeafdf.html

for i, v in ipairs(t) do print(i, v) end
来源：http://hz.shanyushiyangkeji.top/gtxyrblziw.html

[T35] Lua：字典表
来源：http://hz.zhijiandao.cn/gtakrfjrkc.html

local d = { a = 1 };  d.b = 2
来源：http://hz.hnxiangtu.top/gtmrgvbgem.html

[T36] Lua：函数
来源：http://hz.sweek.top/gtwhvwpoxg.html

function add(a, b) return a + b end
来源：http://hz.feifeiyinyue.top/gtuejnajjj.html

[T37] Lua：字符串拼接
来源：http://hz.wangshuangyany.cn/gtwfareszg.html

"a" .. "b"
来源：http://hz.c1oappe.top/gtcomxgbez.html

[T38] Lua：条件
来源：http://hz.dashuyun.cn/gtogtifvcm.html

if x > 0 then print("正") end
来源：http://hz.vqdsnc.cn/gtpjjgumxu.html

[T39] Lua：模式匹配
来源：http://hz.ivvv.top/gtmdswkoxn.html

string.find(s, "%d+")
来源：http://hz.daxiang520.top/gtgrlsmtko.html

[T40] Lua：元表
来源：http://hz.sufxvd.cn/gtifrckabj.html

setmetatable({}, { __index = base })
来源：http://hz.hnxiangtu.top/gtlnpdjxow.html

[T41] Perl：Hello World
来源：http://hz.shzxlz.cn/gtjwmaerkf.html

print "Hello\n";
来源：http://hz.316326.xyz/gtspwiiuxd.html

[T42] Perl：变量类型
来源：http://hz.meibo888.top/gthhqjojys.html

my $a = 1;  my @arr = (1, 2, 3);  my %h = (a => 1);
来源：http://hz.jinghuilouyu.cn/gtcabxpqox.html

[T43] Perl：字符串插值
来源：http://hz.yangfankeji.com/gtawqhdatk.html

"值: $a"
来源：http://hz.shanyushiyangkeji.top/gtiygcduxt.html

[T44] Perl：条件
来源：http://hz.shuidangran.top/gtqhvgdkrc.html

if ($a > 0) { print "正"; }
来源：http://hz.52xcode.cn/gtimeproie.html

[T45] Perl：数组遍历
来源：http://hz.quarkkingdee.top/gttxjsgfpx.html

for my $x (@arr) { print $x; }
来源：http://hz.zhengqikj.top/gtxsxecqjw.html

[T46] Perl：哈希操作
来源：http://hz.meibo888.top/gtnypvoydy.html

$h{b} = 2;  for my $k (keys %h) { print "$k=$h{$k}"; }
来源：http://hz.yvedp.cn/gtybjndnel.html

[T47] Perl：正则捕获
来源：http://hz.cashguo.top/gtmqkkqbkd.html

if ($s =~ /(\d+)/) { print $1; }
来源：http://hz.shanyushiyangtech.top/gtbhhqlzfa.html

[T48] Perl：正则替换
来源：http://hz.tianlin.xyz/gtcyjyqznc.html

$s =~ s/old/new/g;
来源：http://hz.xinyue.icu/gtbgkozbhm.html

[T49] Perl：函数
来源：http://hz.birdmap.top/gtvypzpjtm.html

sub add { my ($a, $b) = @_; return $a + $b; }
来源：http://hz.zhengqikj.top/gthcekqamn.html

[T50] Perl：逐行读文件
来源：http://hz.sufxvd.cn/gtncsnihsq.html

open my $fh, "<", "a.txt" or die $!;
来源：http://hz.zhixingplan.top/gtnmqnrhoc.html

while (my $line = <$fh>) { print $line; }
来源：http://hz.hongshengwenyu.top/gtwzetwqrn.html

[T51] Scala：Hello World
来源：http://hz.tanke756.top/gtdychspxg.html

println("Hello")
来源：http://hz.andypj.xyz/gteugvoazz.html

[T52] Scala：变量
来源：http://hz.jqgfzy.top/gtkuoaklhv.html

val a = 1;  var b = 2
来源：http://hz.ydjk.org.cn/gtqqkromsr.html

[T53] Scala：字符串插值
来源：http://hz.cheryme.top/gtorxbpqww.html

s"值: $b"
来源：http://hz.chenlongwang.top/gtvbgqbigh.html

[T54] Scala：集合映射
来源：http://hz.sysykeji.top/gtqigpmkcl.html

List(1, 2, 3).map(_ * 2)
来源：http://hz.zhijiandao.cn/gtvkugdurd.html

[T55] Scala：集合过滤
来源：http://hz.iojbl.cn/gtdxdbzrkm.html

List(1, 2, 3).filter(_ > 1)
来源：http://hz.jiagoushi.top/gtewcaiazj.html

[T56] Scala：样例类
来源：http://hz.hfpthk.cn/gtcuzxuweq.html

case class User(name: String, age: Int)
来源：http://hz.meibo888.top/gtvuzslfak.html

[T57] Scala：模式匹配
来源：http://hz.xylfe.cn/gtohdybnwz.html

x match { case 1 => "一"; case _ => "其他" }
来源：http://hz.9152youxi.cn/gtfldvzedy.html

[T58] Scala：函数定义
来源：http://hz.zhongyouzk.top/gtdqkhbqaa.html

def add(a: Int, b: Int): Int = a + b
来源：http://hz.guowangkeji.top/gtchwgxjfd.html

[T59] Scala：循环
来源：http://hz.zhixingplan.top/gtjxuaowty.html

for (i <- 1 to 10) println(i)
来源：http://hz.chenlongwang.top/gtncqiffgk.html

[T60] Scala：折叠
来源：http://hz.ehwqpu.com/gtofndqqrr.html

List(1, 2, 3).foldLeft(0)(_ + _)
来源：http://hz.jinghuilouyu.cn/gtogbjixrd.html

================================================================================
来源：http://hz.nanxuanxn.top/gtgetwqvpx.html

U. 高频实用片段（Python / PHP / JavaScript 各 40 条）
来源：http://hz.zhongyouzk.top/gteydrvran.html

================================================================================
来源：http://hz.zhaomingkeji.xyz/gtzqfesxkt.html

[U01] Py：创建虚拟环境
来源：http://hz.hammf.cn/gtezlgyggw.html

python -m venv .venv && source .venv/bin/activate
来源：http://hz.jinghuilouyu.cn/gtbdofzjdt.html

[U02] Py：导出 / 安装依赖
来源：http://hz.bjfxy.top/gtlugmmddq.html

pip freeze > requirements.txt;  pip install -r requirements.txt
来源：http://hz.yangfankeji.com/gtgvrmwfeh.html

[U03] Py：加载 .env 配置
来源：http://hz.cqqwz.cn/gtadmounrr.html

from dotenv import load_dotenv; load_dotenv()
来源：http://hz.jianghu66.top/gtacrvhmmc.html

[U04] Py：变量调试打印
来源：http://hz.xylfe.cn/gtunveqlyg.html

print(f"{x=}")            # 输出 x=值，Python 3.8+
来源：http://hz.cdnleiting.top/gtzfscchcw.html

[U05] Py：列表去重且保序
来源：http://hz.cheryme.top/gthzwglpxr.html

list(dict.fromkeys(arr))
来源：http://hz.316326.xyz/gtdoqeibbf.html

[U06] Py：合并两个字典
来源：http://hz.cheryme.top/gtnkxfsfzb.html

{**a, **b}
来源：http://hz.zhijiandao.cn/gttnkxzasg.html

[U07] Py：反转字典键值
来源：http://hz.wangdashe.top/gtdugantbx.html

{v: k for k, v in d.items()}
来源：http://hz.xylfe.cn/gtyrouvlum.html

[U08] Py：展平二维列表
来源：http://hz.cashguo.top/gtpnigczrw.html

[y for x in nested for y in x]
来源：http://hz.svipenyu.cn/gtqbfhcrck.html

[U09] Py：字典取最大值的键
来源：http://hz.zhijiandao.cn/gtvbidijsz.html

max(d, key=d.get)
来源：http://hz.tianlin.xyz/gtyiiaodnq.html

[U10] Py：按值排序字典
来源：http://hz.zhaomingkeji.xyz/gtsasikbnd.html

dict(sorted(d.items(), key=lambda kv: kv[1]))
来源：http://hz.yangfankeji.com/gthprysxaq.html

[U11] Py：生成器表达式
来源：http://hz.pycfn.com/gtbwvtwexz.html

(x * 2 for x in arr)
来源：http://hz.yj20258.top/gtjehahdfc.html

[U12] Py：取出现最多的 3 个元素
来源：http://hz.ybcxt.top/gtrdwhcgta.html

Counter(arr).most_common(3)
来源：http://hz.snrcjt.cn/gtwwvehuls.html

[U13] Py：固定长度队列
来源：http://hz.havefunace.top/gtkopcktwo.html

deque(maxlen=10)
来源：http://hz.ybcxt.top/gtwhrhnbec.html

[U14] Py：分组收集到列表
来源：http://hz.meibo888.top/gtgvigtwhi.html

defaultdict(list)
来源：http://hz.ydjk.org.cn/gtejbcyzum.html

[U15] Py：高精度计时
来源：http://hz.ppjwa.cn/gtzkhuwfkh.html

t = time.perf_counter()
来源：http://hz.yuxming.cn/gtaiplwqbb.html

[U16] Py：命令行参数解析
来源：http://hz.birdmap.top/gtrpujktgn.html

ap = argparse.ArgumentParser();  ap.add_argument("--name");  args = ap.parse_args()
来源：http://hz.jinyuanbaomall.cn/gtfwcadlpm.html

[U17] Py：初始化日志
来源：http://hz.wangdashe.top/gtuxrhfdfz.html

logging.basicConfig(level=logging.INFO)
来源：http://hz.nanxinkj.top/gtisffpmso.html

[U18] Py：预编译正则
来源：http://hz.zhongyouzk.top/gttoeiphdg.html

pat = re.compile(r"\d+")
来源：http://hz.shzxlz.cn/gtoeqeuqfu.html

[U19] Py：正则替换带回调
来源：http://hz.nanxinkj.top/gtpgllivha.html

re.sub(r"\d+", lambda m: str(int(m.group()) * 2), s)
来源：http://hz.tanke756.top/gtjfsqbipc.html

[U20] Py：缓存函数结果
来源：http://hz.ivvv.top/gtzqfuiuel.html

@functools.lru_cache(maxsize=None)
来源：http://hz.hnxiangtu.top/gtqbjlrjvu.html

[U21] Py：自定义上下文管理器
来源：http://hz.hfpthk.cn/gtcionswdy.html

@contextlib.contextmanager
来源：http://hz.daxiang520.top/gthijzyebb.html

[U22] Py：矩阵转置
来源：http://hz.hnxiangtu.top/gtaxvxeyih.html

list(zip(*m))
来源：http://hz.jianghu66.top/gtgqqwvako.html

[U23] Py：分块读取大文件
来源：http://hz.zhongyouzk.top/gtavkmqhaw.html

for chunk in iter(lambda: f.read(8192), b""):
来源：http://hz.tianlin.xyz/gtxfcardsl.html

[U24] Py：路径操作
来源：http://hz.guowangkeji.top/gtskhwfoda.html

Path("a/b.txt").parent.mkdir(parents=True, exist_ok=True)
来源：http://hz.svipenyu.cn/gtfycncjer.html

[U25] Py：CSV 按字典读
来源：http://hz.cheryme.top/gtfylkuaiv.html

csv.DictReader(f)
来源：http://hz.tanke756.top/gtzdkysjof.html

[U26] Py：并发下载
来源：http://hz.gaohongyu789.top/gtafbdhmah.html

ThreadPoolExecutor(max_workers=8).map(fetch, urls)
来源：http://hz.hongshengwenyu.top/gtzfnmytwt.html

[U27] Py：异步 HTTP
来源：http://hz.yj202588.top/gtqmmvfnvr.html

aiohttp.ClientSession() 配合 async with
来源：http://hz.cashguo.top/gtmvnbrjim.html

[U28] Py：类型别名
来源：http://hz.yanxiufei.cn/gtochigbzl.html

UserId = int
来源：http://hz.redwolf501.top/gtzxithppy.html

[U29] Py：属性校验
来源：http://hz.jinyuanbaomall.cn/gtbxcsteab.html

@property 与 @x.setter 配合
来源：http://hz.gogol.net.cn/gtcqnwpckz.html

[U30] Py：数据类
来源：http://hz.xuanzx.com/gtlzlowrxr.html

@dataclass(slots=True)
来源：http://hz.guannengcc.top/gtjokiuisi.html

[U31] Py：单测
来源：http://hz.yvedp.cn/gtkcqzhnsy.html

python -m pytest -q
来源：http://hz.yuanzhike.top/gtxkzbyzie.html

[U32] Py：代码格式化
来源：http://hz.smart0.xyz/gtjwyfuewz.html

ruff format . && ruff check --fix .
来源：http://hz.gogol.net.cn/gtfoykbcwx.html

[U33] Py：打包发布
来源：http://hz.shanyushiyangkeji.top/gtebaqrsts.html

python -m build  （依赖 pyproject.toml）
来源：http://hz.ydjk.org.cn/gtadzdwraz.html

[U34] Py：判断编码
来源：http://hz.bjfxy.top/gtajxmsfxy.html

chardet.detect(raw)
来源：http://hz.xylfe.cn/gtmsfdugrw.html

[U35] Py：发送邮件
来源：http://hz.ybcxt.top/gtgnijvvfj.html

smtplib.SMTP_SSL(...).send_message(msg)
来源：http://hz.jyoumei.cn/gtcpbhiucm.html

[U36] Py：定时任务
来源：http://hz.hammf.cn/gtbycgzzup.html

schedule.every(10).minutes.do(job)
来源：http://hz.haohaochexian.top/gtgzkxammv.html

[U37] Py：读写 Excel
来源：http://hz.zhixingplan.top/gtmoekszcd.html

pandas.read_excel / DataFrame.to_excel
来源：http://hz.nwbrower.top/gtdjcesrco.html

[U38] Py：获取脚本所在目录
来源：http://hz.xylfe.cn/gtcssjudwo.html

Path(__file__).resolve().parent
来源：http://hz.smart0.xyz/gtwrfxaser.html

[U39] Py：判断是否在交互环境
来源：http://hz.nwbrower.top/gtedcbcpve.html

sys.stdout.isatty()
来源：http://hz.ehwqpu.com/gtgfvpjynk.html

[U40] Py：打印到标准错误
来源：http://hz.jinghuilouyu.cn/gtrecqolzv.html

print("err", file=sys.stderr)
来源：http://hz.316326.xyz/gtgapiuber.html

[U41] PHP：初始化 Composer 项目
来源：http://hz.tianlin.xyz/gtovegcipy.html

composer init;  composer require guzzlehttp/guzzle
来源：http://hz.aizwys.cn/gtwsmsqfoa.html

[U42] PHP：PSR-4 自动加载
来源：http://hz.snrcjt.cn/gtvpmdqsyb.html

"autoload": { "psr-4": { "App\\": "src/" } }
来源：http://hz.zhengqikj.top/gtrgnedoll.html

[U43] PHP：声明命名空间
来源：http://hz.meibo888.top/gtdwhuqbfj.html

namespace App\Http;
来源：http://hz.tianlin.xyz/gtymhrsbjy.html

[U44] PHP：开启严格类型
来源：http://hz.ehwqpu.com/gtjcltpkue.html

declare(strict_types=1);
来源：http://hz.ywan-chungtsiang.top/gtdxttrtqw.html

[U45] PHP：类型声明与返回类型
来源：http://hz.guannengcc.top/gtomefvzwq.html

function add(int $a, int $b): int { return $a + $b; }
来源：http://hz.sufxvd.cn/gtwogwaosj.html

[U46] PHP：可空类型
来源：http://hz.ydzc1.top/gtfalxofxy.html

?string $name = null
来源：http://hz.aibaodan.cn/gtsjowcvic.html

[U47] PHP：联合类型
来源：http://hz.shuidangran.top/gtxebchqrd.html

int|string $id
来源：http://hz.wangshuangyany.cn/gtiqzuiqkr.html

[U48] PHP：纯枚举
来源：http://hz.52xcode.cn/gtzleikzyi.html

enum Status: string { case Active = "active"; case Off = "off"; }
来源：http://hz.mhx1999.top/gtynqagmlr.html

[U49] PHP：只读属性
来源：http://hz.shangyingyoupin.top/gtqhjpzzhx.html

public readonly string $name
来源：http://hz.ydzc1.top/gtkqxtsufk.html

[U50] PHP：构造器属性提升
来源：http://hz.jqgfzy.top/gtyitzyocb.html

public function __construct(private int $id) {}
来源：http://hz.9152youxi.cn/gtczcgtooy.html

[U51] PHP：数组解构
来源：http://hz.ybcxt.top/gtmlvhyasz.html

[$a, $b] = $arr;
来源：http://hz.dashuyun.cn/gttxdsrcmf.html

[U52] PHP：箭头函数
来源：http://hz.wangdashe.top/gtftrgqiyb.html

$double = fn($x) => $x * 2;
来源：http://hz.zhixingplan.top/gtzxsgxjvg.html


<!-- 参考信息 -->