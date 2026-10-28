代发 wailian999

static int counter = 0;
来源：http://hz.chenzaomai.com/gtxigqvxtx.html

[S29] C：变参函数
来源：http://hz.pengpengdd.cyou/gtrczrrvjl.html

va_list ap; va_start(ap, fmt); vprintf(fmt, ap); va_end(ap);
来源：http://hz.xziqi.cn/gtkrqhwgfd.html

[S30] C：头文件保护
来源：http://hz.xuanzx.com/gtwlqhjvim.html

#ifndef X_H
来源：http://hz.wangdashe.top/gtmprmbpwl.html

#define X_H
来源：http://hz.sysykeji.top/gtcrsriael.html

#endif
来源：http://hz.jqgfzy.top/gtnsawnadl.html

[S31] C++：Hello World
来源：http://hz.yanxiufei.cn/gtifzrxfps.html

#include <iostream>
来源：http://hz.daria6918.cn/gtgjrddtru.html

int main() { std::cout << "Hello\n"; }
来源：http://hz.shzxlz.cn/gtuvengazn.html

[S32] C++：字符串
来源：http://hz.dashuyun.cn/gtgdckqgas.html

std::string s = "hi";  s += "!";
来源：http://hz.yj202588.top/gtasestlpk.html

[S33] C++：vector 增删
来源：http://hz.zdqjudy.top/gtygwnueqa.html

std::vector<int> v{1, 2, 3};  v.push_back(4);
来源：http://hz.fzhhl.top/gtgltjilcj.html

[S34] C++：遍历 vector
来源：http://hz.xziqi.cn/gtcyuhzxnf.html

for (auto &x : v) { std::cout << x; }
来源：http://hz.xuetiantiany.cn/gtlusmdlgz.html

[S35] C++：map
来源：http://hz.shanyushiyangtech.top/gtnqavqjgi.html

std::map<std::string, int> m;  m["a"] = 1;
来源：http://hz.mhx1999.top/gtnfqwmiba.html

[S36] C++：unordered_map
来源：http://hz.tanke756.top/gtktbhbkqq.html

std::unordered_map<std::string, int> m;  m["a"] = 1;
来源：http://hz.andypj.xyz/gtfgoqiuxy.html

[S37] C++：set
来源：http://hz.snrcjt.cn/gtqexoeeon.html

std::set<int> s{1, 2, 3};  s.insert(4);
来源：http://hz.xuanzx.com/gtyxgdzfoy.html

[S38] C++：排序
来源：http://hz.cqqwz.cn/gtlcukdksr.html

std::sort(v.begin(), v.end());
来源：http://hz.jianghu66.top/gttgztquju.html

[S39] C++：自定义比较器排序
来源：http://hz.iojbl.cn/gtvzqimwcp.html

std::sort(v.begin(), v.end(), [](int a, int b) { return a > b; });
来源：http://hz.kuanghao11.cn/gttkqvtfep.html

[S40] C++：查找元素
来源：http://hz.jinqigufen.top/gtjdyxhalt.html

auto it = std::find(v.begin(), v.end(), 3);
来源：http://hz.chenzaomai.com/gtbznvzxnm.html

[S41] C++：类与构造函数
来源：http://hz.ivvv.top/gtwldpvtwc.html

class A { public: A(int v) : x_(v) {} int get() const { return x_; } private: int x_; };
来源：http://hz.yonumen.top/gtjhbtpnhw.html

[S42] C++：继承与虚函数
来源：http://hz.dianchejie.cn/gthrmfreix.html

class B : public Base { public: void f() override {} };
来源：http://hz.hfpthk.cn/gtxtgrejeg.html

[S43] C++：智能指针
来源：http://hz.pycfn.com/gtmkmqqsnc.html

auto p = std::make_unique<int>(5);
来源：http://hz.aizwys.cn/gtxjnelveq.html

[S44] C++：引用传参
来源：http://hz.yj20258888.top/gtizrnkmmz.html

void inc(int &x) { ++x; }
来源：http://hz.zhoulong.xyz/gtcwsbvwky.html

[S45] C++：lambda
来源：http://hz.shuidangran.top/gthuuhuzub.html

auto add = [](int a, int b) { return a + b; };
来源：http://hz.yj20258888.top/gtlqkdrpbv.html

[S46] C++：函数模板
来源：http://hz.hammf.cn/gtqnhbtgwj.html

template <typename T> T maxv(T a, T b) { return a > b ? a : b; }
来源：http://hz.cheryme.top/gttqqckflq.html

[S47] C++：结构化绑定遍历
来源：http://hz.ivvv.top/gtkgwxseke.html

for (const auto &[k, v] : m) { std::cout << k << v; }
来源：http://hz.gogol.net.cn/gtoqxttnkg.html

[S48] C++：逐行读文件
来源：http://hz.jlsjyb.cn/gtqxupuvkq.html

std::ifstream in("a.txt");  std::string line;
来源：http://hz.gaohongyu789.top/gtbedxrsza.html

while (std::getline(in, line)) { }
来源：http://hz.jqgfzy.top/gtlvltforb.html

[S49] C++：写文件
来源：http://hz.svipenyu.cn/gtzjtuiugm.html

std::ofstream out("a.txt");  out << "hi\n";
来源：http://hz.meibo888.top/gtxtwdgchk.html

[S50] C++：格式化数字
来源：http://hz.sxryk.cn/gtedhsgafq.html

std::ostringstream os;  os << std::fixed << std::setprecision(2) << 3.14159;
来源：http://hz.yj202588.top/gtiawszxoo.html

[S51] C++：显式类型转换
来源：http://hz.zhengqikj.top/gttdyprcut.html

static_cast<double>(a) / b
来源：http://hz.xziqi.cn/gtkzpbmija.html

[S52] C++：const 与 noexcept
来源：http://hz.bjfxy.top/gthyriwoaf.html

int size() const noexcept { return n_; }
来源：http://hz.jinqigfzy.top/gtvijeygcl.html

[S53] C++：移动语义
来源：http://hz.sweek.top/gtsnhhysdx.html

std::vector<int> w = std::move(v);
来源：http://hz.wangdashe.top/gttehtumvv.html

[S54] C++：异常处理
来源：http://hz.aizwys.cn/gtynlkwzfi.html

try { throw std::runtime_error("x"); } catch (const std::exception &e) { }
来源：http://hz.gogol.net.cn/gtldluajje.html

[S55] C++：结构化绑定
来源：http://hz.cqqwz.cn/gtcdynhgny.html

auto [a, b] = std::make_pair(1, 2);
来源：http://hz.birdmap.top/gtlkmwtfze.html

[S56] C++：optional
来源：http://hz.hnxiangtu.top/gtsjqaeict.html

std::optional<int> o = 5;  if (o) { int v = *o; }
来源：http://hz.cucudq.cn/gtnkgxjipj.html

[S57] C++：编译期常量
来源：http://hz.daxiang520.top/gttxqjdtfw.html

constexpr int N = 10;
来源：http://hz.pengpengdd.cyou/gtyvrpfwvd.html

[S58] C++：命名空间
来源：http://hz.nanxinkj.top/gtzhcvrzvs.html

namespace ns { int f() { return 1; } }
来源：http://hz.52xcode.cn/gtrthiwqct.html

[S59] C++：静态断言
来源：http://hz.ppjwa.cn/gtvxjouskt.html

static_assert(sizeof(int) == 4, "int 必须 4 字节");
来源：http://hz.mhx1999.top/gtcvwbwxwt.html

[S60] C++：遍历并删除元素
来源：http://hz.pycfn.com/gtnlvjapca.html

v.erase(std::remove_if(v.begin(), v.end(), [](int x) { return x < 0; }), v.end());
来源：http://hz.zhijiandao.cn/gtaopmcmig.html

================================================================================
来源：http://hz.mhx1999.top/gtsbbttmyv.html

T. 其他语言补充（Kotlin / Swift / Lua / Perl / Scala）
来源：http://hz.tanke756.top/gtcprxlrzr.html

================================================================================
来源：http://hz.zhixingplan.top/gtknckpylb.html

[T01] Kotlin：Hello World
来源：http://hz.andypj.xyz/gtzbxfgvbw.html

println("Hello")
来源：http://hz.gotoacloud.top/gthhxhbuua.html

[T02] Kotlin：变量
来源：http://hz.zhongyouzk.top/gtafvgqoaf.html

val a = 1;  var b = 2        // val 只读，var 可变
来源：http://hz.ydzc1.top/gtjmxxsrsx.html

[T03] Kotlin：字符串模板
来源：http://hz.snrcjt.cn/gtjqpnmlif.html

"值: $b"
来源：http://hz.mhx1999.top/gtjdiuiesd.html

[T04] Kotlin：空安全
来源：http://hz.tanke756.top/gtvuwcoiet.html

val n: String? = null;  n?.length
来源：http://hz.zhijiandao.cn/gtgrneukzr.html

[T05] Kotlin：when 表达式
来源：http://hz.meibo888.top/gtttygaetn.html

val s = when (x) { 1 -> "一" else -> "其他" }   // 多分支时每个分支单独一行
来源：http://hz.jianghu66.top/gtksiocika.html

[T06] Kotlin：集合映射
来源：http://hz.dashuyun.cn/gtqvmytznq.html

listOf(1, 2, 3).map { it * 2 }
来源：http://hz.jianghu66.top/gtuhykeaxe.html

[T07] Kotlin：集合过滤
来源：http://hz.cheryme.top/gthrmrpxin.html

listOf(1, 2, 3).filter { it > 1 }
来源：http://hz.yongpay.top/gttierroif.html

[T08] Kotlin：数据类
来源：http://hz.ywan-chungtsiang.top/gtpdazxiwu.html

data class User(val name: String, val age: Int)
来源：http://hz.chenlongwang.top/gtqhgannjq.html

[T09] Kotlin：扩展函数
来源：http://hz.chenjidiqi.icu/gttucxrrfu.html

fun String.exclaim() = this + "!"
来源：http://hz.tanke756.top/gthwfveunm.html

[T10] Kotlin：默认参数
来源：http://hz.jianghu66.top/gtrtdscheg.html

fun greet(name: String = "World") = "Hi $name"
来源：http://hz.nwbrower.top/gtwxkgjzqv.html

[T11] Kotlin：协程
来源：http://hz.ppjwa.cn/gtdthralof.html

GlobalScope.launch { delay(1000); println("done") }
来源：http://hz.yvedp.cn/gtjorkgbaf.html

[T12] Kotlin：解构声明
来源：http://hz.shangyingyoupin.top/gtglhmfbqm.html

val (a, b) = Pair(1, 2)
来源：http://hz.fzhhl.top/gtimzayfhq.html

[T13] Kotlin：只读 Map
来源：http://hz.jinqigufen.top/gtystfvivu.html

val m = mapOf("a" to 1)
来源：http://hz.andypj.xyz/gtrlgyrfli.html

[T14] Kotlin：循环
来源：http://hz.9152youxi.cn/gthobqrjrs.html

for (i in 1..10) println(i)
来源：http://hz.sxryk.cn/gtimeqyxur.html

[T15] Kotlin：接口
来源：http://hz.316326.xyz/gtdfecmxef.html

interface Shape { fun area(): Double }
来源：http://hz.hnqzz.top/gtbbbikyoq.html

[T16] Swift：Hello World
来源：http://hz.yj202588.top/gtwquakpau.html

print("Hello")
来源：http://hz.dianchejie.cn/gtpgzbgits.html

[T17] Swift：变量与常量
来源：http://hz.tanke756.top/gtwcaffzpd.html

var a = 1;  let b = 2
来源：http://hz.9152youxi.cn/gtdutkodsv.html

[T18] Swift：字符串插值
来源：http://hz.zhengqikj.top/gtfyurtpgc.html

"值: \(b)"
来源：http://hz.gotoacloud.top/gtxewnrwtc.html

[T19] Swift：可选绑定
来源：http://hz.bjfxy.top/gtzsypdbdd.html

if let n = opt { print(n) }
来源：http://hz.quarkkingdee.top/gtfmhjjkcf.html

[T20] Swift：数组操作
来源：http://hz.zhaomingkeji.xyz/gtrlspmdrc.html

var a = [1, 2, 3];  a.append(4)
来源：http://hz.zhongyouzk.top/gtgjxvqujl.html

[T21] Swift：遍历
来源：http://hz.zhixingplan.top/gthjmcdeyk.html

for x in a { print(x) }
来源：http://hz.yj202588.top/gtaugtuvzb.html

[T22] Swift：字典
来源：http://hz.cdnleiting.top/gtslpdazfr.html

var d = ["a": 1];  d["b"] = 2
来源：http://hz.hnqzz.top/gtlrldlvpj.html

[T23] Swift：函数
来源：http://hz.cucudq.cn/gthmuweroz.html

func add(_ a: Int, _ b: Int) -> Int { a + b }
来源：http://hz.shangyingyoupin.top/gthrosvlyk.html

[T24] Swift：闭包
来源：http://hz.yangfankeji.com/gtfnyitnrm.html

let f = { (x: Int) -> Int in x * 2 }
来源：http://hz.tianlin.xyz/gtcvyvzitv.html

[T25] Swift：结构体
来源：http://hz.ehwqpu.com/gtaiyljfrs.html

struct P { var x: Int }
来源：http://hz.jinyuanbaomall.cn/gtktkzyfnj.html

[T26] Swift：类与重写
来源：http://hz.chenzaomai.com/gtjfasntas.html

class A: Base { override func f() {} }
来源：http://hz.pycfn.com/gtmjyfqnwf.html

[T27] Swift：错误处理
来源：http://hz.jqgufenzy.top/gtuspsojgu.html

do { try f() } catch { print(error) }
来源：http://hz.meibo888.top/gtigdgyzbq.html

[T28] Swift：枚举
来源：http://hz.andypj.xyz/gtfdnypbjv.html

enum Color { case red, green }
来源：http://hz.0kj1m.cn/gtinchbivt.html

[T29] Swift：guard 提前返回
来源：http://hz.cqqwz.cn/gtrbanxbjn.html

guard let x = opt else { return }
来源：http://hz.wangshuangyany.cn/gthdwfdgue.html

[T30] Swift：协议
来源：http://hz.316326.xyz/gtyhnqehwi.html

protocol Shape { func area() -> Double }
来源：http://hz.smart0.xyz/gthharjiwr.html

[T31] Lua：Hello World
来源：http://hz.kuanghao11.cn/gthuqrqsmi.html

print("Hello")
来源：http://hz.vqdsnc.cn/gtvtrknkoc.html

[T32] Lua：局部变量
来源：http://hz.wangdashe.top/gtlqfumuep.html

local a = 1
来源：http://hz.jinqigufen.top/gtowmcniig.html

[T33] Lua：表（数组）
来源：http://hz.hfpthk.cn/gtclthtsbg.html

local t = {1, 2, 3};  t[4] = 4
来源：http://hz.yj202588.top/gtgwhguzdj.html

[T34] Lua：遍历表
来源：http://hz.zdqjudy.top/gtuadsggmf.html

for i, v in ipairs(t) do print(i, v) end
来源：http://hz.yongpay.top/gtllwkfhmw.html

[T35] Lua：字典表
来源：http://hz.hongshengwenyu.top/gtfwgwfcqa.html

local d = { a = 1 };  d.b = 2
来源：http://hz.chenlongwang.top/gtwagsiahj.html

[T36] Lua：函数
来源：http://hz.jqgfzy.top/gtfzcjapis.html

function add(a, b) return a + b end
来源：http://hz.quarkkingdee.top/gtgxmabpci.html

[T37] Lua：字符串拼接
来源：http://hz.iojbl.cn/gtudqkhgcj.html

"a" .. "b"
来源：http://hz.hywenlv.cn/gtfkhpbcic.html

[T38] Lua：条件
来源：http://hz.xuanzx.com/gtnrutqack.html

if x > 0 then print("正") end
来源：http://hz.jlsjyb.cn/gthjwtydit.html

[T39] Lua：模式匹配
来源：http://hz.vqdsnc.cn/gttseizsxv.html

string.find(s, "%d+")
来源：http://hz.havefunace.top/gtterfcgvd.html

[T40] Lua：元表
来源：http://hz.aizwys.cn/gtgfjomzfb.html

setmetatable({}, { __index = base })
来源：http://hz.cqqwz.cn/gtapfuqwbx.html

[T41] Perl：Hello World
来源：http://hz.ywan-chungtsiang.top/gtjtrwmhoz.html

print "Hello\n";
来源：http://hz.yj20258.top/gtdzhqmwrq.html

[T42] Perl：变量类型
来源：http://hz.jlsjyb.cn/gtxpjwmayk.html

my $a = 1;  my @arr = (1, 2, 3);  my %h = (a => 1);
来源：http://hz.shuidangran.top/gtwcakfcst.html

[T43] Perl：字符串插值
来源：http://hz.ydzc1.top/gttlddbcpb.html

"值: $a"
来源：http://hz.vqdsnc.cn/gtppxzfhkh.html

[T44] Perl：条件
来源：http://hz.316326.xyz/gtkivfrysj.html

if ($a > 0) { print "正"; }
来源：http://hz.mhx1999.top/gtakrajtgi.html

[T45] Perl：数组遍历
来源：http://hz.cqqwz.cn/gtlhbhlaic.html

for my $x (@arr) { print $x; }
来源：http://hz.52xcode.cn/gtfftaqddb.html

[T46] Perl：哈希操作
来源：http://hz.cucudq.cn/gtgjwvuyxr.html

$h{b} = 2;  for my $k (keys %h) { print "$k=$h{$k}"; }
来源：http://hz.fzhhl.top/gtgkabmlfu.html

[T47] Perl：正则捕获
来源：http://hz.guowangkeji.top/gtvngexfnx.html

if ($s =~ /(\d+)/) { print $1; }
来源：http://hz.fengsongda.top/gtysifvpep.html

[T48] Perl：正则替换
来源：http://hz.yuxming.cn/gtthwiamen.html

$s =~ s/old/new/g;
来源：http://hz.jianghu66.top/gtajpjielr.html

[T49] Perl：函数
来源：http://hz.snrcjt.cn/gtspjdivuy.html

sub add { my ($a, $b) = @_; return $a + $b; }
来源：http://hz.jianghu66.top/gthebmyjps.html

[T50] Perl：逐行读文件
来源：http://hz.mhx1999.top/gtlirgxxdf.html

open my $fh, "<", "a.txt" or die $!;
来源：http://hz.xuetiantiany.cn/gtzogfcont.html

while (my $line = <$fh>) { print $line; }
来源：http://hz.haohaochexian.top/gtkeauwfzt.html

[T51] Scala：Hello World
来源：http://hz.vqdsnc.cn/gtzkwawpuh.html

println("Hello")
来源：http://hz.sweek.top/gtblpgwzcv.html

[T52] Scala：变量
来源：http://hz.yvedp.cn/gtuukwfvga.html

val a = 1;  var b = 2
来源：http://hz.zhengqikj.top/gtkzjskjdf.html

[T53] Scala：字符串插值
来源：http://hz.cdnleiting.top/gtbcuaogrf.html

s"值: $b"
来源：http://hz.zdqjudy.top/gtocramaay.html

[T54] Scala：集合映射
来源：http://hz.jlsjyb.cn/gtubqhxizy.html

List(1, 2, 3).map(_ * 2)
来源：http://hz.gaohongyu789.top/gtdvjqhonp.html

[T55] Scala：集合过滤
来源：http://hz.yj202588.top/gtnbjfqvoc.html

List(1, 2, 3).filter(_ > 1)
来源：http://hz.9152youxi.cn/gtrulvxxyz.html

[T56] Scala：样例类
来源：http://hz.yongpay.top/gteaikxkyz.html

case class User(name: String, age: Int)
来源：http://hz.gotoacloud.top/gtjusaspng.html

[T57] Scala：模式匹配
来源：http://hz.tianlin.xyz/gtgapjzyqw.html

x match { case 1 => "一"; case _ => "其他" }
来源：http://hz.havefunace.top/gtgdlywnwn.html

[T58] Scala：函数定义
来源：http://hz.jinqigfzy.top/gtmezwbnay.html

def add(a: Int, b: Int): Int = a + b
来源：http://hz.gotoacloud.top/gtpxzxufaf.html

[T59] Scala：循环
来源：http://hz.cdnleiting.top/gtfcxmetan.html

for (i <- 1 to 10) println(i)
来源：http://hz.shuidangran.top/gtfjxbrvsk.html

[T60] Scala：折叠
来源：http://hz.yangfankeji.com/gtlcdxszwx.html

List(1, 2, 3).foldLeft(0)(_ + _)
来源：http://hz.gzhubu.top/gtcnmgzifb.html

================================================================================
来源：http://hz.9152youxi.cn/gtkknzkeux.html

U. 高频实用片段（Python / PHP / JavaScript 各 40 条）
来源：http://hz.iojbl.cn/gttltqjgxr.html

================================================================================
来源：http://hz.c1oappe.top/gtvstvjqwl.html

[U01] Py：创建虚拟环境
来源：http://hz.zhoulong.xyz/gtnufmscba.html

python -m venv .venv && source .venv/bin/activate
来源：http://hz.snrcjt.cn/gtirzrilpk.html

[U02] Py：导出 / 安装依赖
来源：http://hz.fengsongda.top/gtaqkfapnv.html

pip freeze > requirements.txt;  pip install -r requirements.txt
来源：http://hz.aizwys.cn/gtzqdfdctb.html

[U03] Py：加载 .env 配置
来源：http://hz.dianchejie.cn/gtaojlgcjr.html

from dotenv import load_dotenv; load_dotenv()
来源：http://hz.nanxinkj.top/gtasvzuvpx.html

[U04] Py：变量调试打印
来源：http://hz.hammf.cn/gtoihnxeet.html

print(f"{x=}")            # 输出 x=值，Python 3.8+
来源：http://hz.zhiwuduotai.top/gtkarqlfhc.html

[U05] Py：列表去重且保序
来源：http://hz.aibaodan.cn/gtyfqygtfw.html

list(dict.fromkeys(arr))
来源：http://hz.smart0.xyz/gtwtqoyxpf.html

[U06] Py：合并两个字典
来源：http://hz.dianchejie.cn/gtufcfhepl.html

{**a, **b}
来源：http://hz.zycfv.cn/gtrnuzqyui.html

[U07] Py：反转字典键值
来源：http://hz.snrcjt.cn/gtamlnkshc.html

{v: k for k, v in d.items()}
来源：http://hz.zhoulong.xyz/gtnzmoxjld.html

[U08] Py：展平二维列表
来源：http://hz.zhongyouzk.top/gttnciowfj.html

[y for x in nested for y in x]
来源：http://hz.yongpay.top/gtrzbxpeau.html

[U09] Py：字典取最大值的键
来源：http://hz.sweek.top/gtmxgbwqui.html

max(d, key=d.get)
来源：http://hz.jlsjyb.cn/gtauluughx.html

[U10] Py：按值排序字典
来源：http://hz.tanke756.top/gtxjlwfcif.html

dict(sorted(d.items(), key=lambda kv: kv[1]))
来源：http://hz.zycfv.cn/gtqwdkusmn.html

[U11] Py：生成器表达式
来源：http://hz.xuetiantiany.cn/gtaifwazao.html

(x * 2 for x in arr)
来源：http://hz.ppjwa.cn/gtaennhwzb.html

[U12] Py：取出现最多的 3 个元素
来源：http://hz.nanxuanxn.top/gtxrpviycl.html

Counter(arr).most_common(3)
来源：http://hz.mhx1999.top/gtrvagitzc.html

[U13] Py：固定长度队列
来源：http://hz.fzhhl.top/gtnvpbyala.html

deque(maxlen=10)
来源：http://hz.wangshuangyany.cn/gtcsbjtizo.html

[U14] Py：分组收集到列表
来源：http://hz.jqgfzy.top/gtrfvvinfd.html

defaultdict(list)
来源：http://hz.yuxming.cn/gtzvqxzlwx.html

[U15] Py：高精度计时
来源：http://hz.shzxlz.cn/gtohgcowzx.html

t = time.perf_counter()
来源：http://hz.jianghu66.top/gtnsolqgse.html

[U16] Py：命令行参数解析
来源：http://hz.cashguo.top/gtdozxbzih.html

ap = argparse.ArgumentParser();  ap.add_argument("--name");  args = ap.parse_args()
来源：http://hz.wangshuangyany.cn/gtvzrwyodm.html

[U17] Py：初始化日志
来源：http://hz.redwolf501.top/gtkfaxbyas.html

logging.basicConfig(level=logging.INFO)
来源：http://hz.yongpay.top/gtxbcumhbt.html

[U18] Py：预编译正则
来源：http://hz.aizwys.cn/gtlyzdlpae.html

pat = re.compile(r"\d+")
来源：http://hz.jinqigufen.top/gtcbsquoiu.html

[U19] Py：正则替换带回调
来源：http://hz.hongshengwenyu.top/gtsglynerk.html

re.sub(r"\d+", lambda m: str(int(m.group()) * 2), s)
来源：http://hz.fengsongda.top/gtlfruufcl.html

[U20] Py：缓存函数结果
来源：http://hz.snrcjt.cn/gtoxrteoqo.html

@functools.lru_cache(maxsize=None)
来源：http://hz.jqgufenzy.top/gtgryhvzve.html

[U21] Py：自定义上下文管理器
来源：http://hz.0kj1m.cn/gtgrnenvql.html

@contextlib.contextmanager
来源：http://hz.zhiwuduotai.top/gtxtizhgwg.html

[U22] Py：矩阵转置
来源：http://hz.jqgfzy.top/gtybrrryis.html

list(zip(*m))
来源：http://hz.jqgufenzy.top/gtblnycmca.html

[U23] Py：分块读取大文件
来源：http://hz.xingfuxueyuan.xyz/gtibqzzutn.html

for chunk in iter(lambda: f.read(8192), b""):
来源：http://hz.pycfn.com/gtdjnkwhef.html

[U24] Py：路径操作
来源：http://hz.chenzaomai.com/gtnxyfoiih.html

Path("a/b.txt").parent.mkdir(parents=True, exist_ok=True)
来源：http://hz.chenzaomai.com/gtamrkruqf.html

[U25] Py：CSV 按字典读
来源：http://hz.jianghu66.top/gtremzasdh.html

csv.DictReader(f)
来源：http://hz.jinqigufen.top/gtikmmdwax.html

[U26] Py：并发下载
来源：http://hz.jinghuilouyu.cn/gtcidomyga.html

ThreadPoolExecutor(max_workers=8).map(fetch, urls)
来源：http://hz.wangshuangyany.cn/gtuxvbhqik.html

[U27] Py：异步 HTTP
来源：http://hz.9152youxi.cn/gtmumycbey.html

aiohttp.ClientSession() 配合 async with
来源：http://hz.cheryme.top/gtpstkurjj.html

[U28] Py：类型别名
来源：http://hz.havefunace.top/gtsitnudpd.html

UserId = int
来源：http://hz.guowangkeji.top/gtryqmwkkr.html

[U29] Py：属性校验
来源：http://hz.hongshengwenyu.top/gtsfldacwl.html

@property 与 @x.setter 配合
来源：http://hz.zhixingplan.top/gtmdcgwkmf.html

[U30] Py：数据类
来源：http://hz.vqdsnc.cn/gtekdpodqs.html

@dataclass(slots=True)
来源：http://hz.birdmap.top/gtjgksmcdc.html

[U31] Py：单测
来源：http://hz.0kj1m.cn/gtukzdyhdz.html

python -m pytest -q
来源：http://hz.dashuyun.cn/gtegkhesmx.html

[U32] Py：代码格式化
来源：http://hz.9152youxi.cn/gtbwnxemhh.html

ruff format . && ruff check --fix .
来源：http://hz.cdnleiting.top/gtirwvwviu.html

[U33] Py：打包发布
来源：http://hz.yanxiufei.cn/gtaozxiyfo.html

python -m build  （依赖 pyproject.toml）
来源：http://hz.nanxuanxn.top/gteronlfya.html

[U34] Py：判断编码
来源：http://hz.jinqigfzy.top/gtwownzryj.html

chardet.detect(raw)
来源：http://hz.kuanghao11.cn/gtkfsxpaak.html

[U35] Py：发送邮件
来源：http://hz.hnqzz.top/gtxjlfzgke.html

smtplib.SMTP_SSL(...).send_message(msg)
来源：http://hz.chenzaomai.com/gtdsdocuww.html

[U36] Py：定时任务
来源：http://hz.9152youxi.cn/gtzclmwdbi.html

schedule.every(10).minutes.do(job)
来源：http://hz.xylfe.cn/gtapcjupeh.html

[U37] Py：读写 Excel
来源：http://hz.vqdsnc.cn/gtymemutig.html

pandas.read_excel / DataFrame.to_excel
来源：http://hz.ydjk.org.cn/gtrpcyvfxn.html

[U38] Py：获取脚本所在目录
来源：http://hz.sysykeji.top/gtoeyqnzdb.html

Path(__file__).resolve().parent
来源：http://hz.nwbrower.top/gttqtbysdv.html

[U39] Py：判断是否在交互环境
来源：http://hz.dianchejie.cn/gtyrrkcmcp.html

sys.stdout.isatty()
来源：http://hz.ehwqpu.com/gtjvvlmvpm.html

[U40] Py：打印到标准错误
来源：http://hz.hysaishi.cn/gtcinzpsiz.html

print("err", file=sys.stderr)
来源：http://hz.dashuyun.cn/gtzviukdod.html

[U41] PHP：初始化 Composer 项目
来源：http://hz.xylfe.cn/gtcgpudecx.html

composer init;  composer require guzzlehttp/guzzle
来源：http://hz.hongshengwenyu.top/gtxikyfegm.html

[U42] PHP：PSR-4 自动加载
来源：http://hz.chenlongwang.top/gtdsxnphmx.html

"autoload": { "psr-4": { "App\\": "src/" } }
来源：http://hz.daria6918.cn/gttbcnnigq.html

[U43] PHP：声明命名空间
来源：http://hz.tianlin.xyz/gtjlgzfazo.html

namespace App\Http;
来源：http://hz.zhijiandao.cn/gtkzcyncyg.html

[U44] PHP：开启严格类型
来源：http://hz.pengpengdd.cyou/gtpyfqjnfa.html

declare(strict_types=1);
来源：http://hz.nwbrower.top/gtipohtizb.html

[U45] PHP：类型声明与返回类型
来源：http://hz.tanke756.top/gtnqhcqfof.html

function add(int $a, int $b): int { return $a + $b; }
来源：http://hz.guowangkeji.top/gtfjcbrkma.html

[U46] PHP：可空类型
来源：http://hz.jiagoushi.top/gtnxdokaxn.html

?string $name = null
来源：http://hz.dianchejie.cn/gtqfybirhn.html

[U47] PHP：联合类型
来源：http://hz.tianlin.xyz/gtdgnaudpq.html

int|string $id
来源：http://hz.hnqzz.top/gtjfjmggfl.html

[U48] PHP：纯枚举
来源：http://hz.xuetiantiany.cn/gtiwidknzu.html

enum Status: string { case Active = "active"; case Off = "off"; }
来源：http://hz.xingfuxueyuan.xyz/gtyisxowsp.html

[U49] PHP：只读属性
来源：http://hz.wangdashe.top/gtrfpnqesi.html

public readonly string $name
来源：http://hz.jinqigufen.top/gtzbyxsjcr.html

[U50] PHP：构造器属性提升
来源：http://hz.daxiang520.top/gtqfrzjobd.html

public function __construct(private int $id) {}
来源：http://hz.smart0.xyz/gtlprkhavt.html

[U51] PHP：数组解构
来源：http://hz.yuanzhike.top/gtwmtdevnn.html

[$a, $b] = $arr;
来源：http://hz.xingfuxueyuan.xyz/gtqerjkvcq.html

[U52] PHP：箭头函数
来源：http://hz.tanke756.top/gteuhhwnnp.html

$double = fn($x) => $x * 2;
来源：http://hz.ywan-chungtsiang.top/gtdkyjbrth.html


<!-- 参考信息 -->