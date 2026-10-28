代发 wailian999

#include <iostream>
来源：http://hz.hammf.cn/gtdsqhgktp.html

int main() { std::cout << "Hello\n"; }
来源：http://hz.yanxiufei.cn/gthggjztir.html

[S32] C++：字符串
来源：http://hz.meibo888.top/gtwunpmhqu.html

std::string s = "hi";  s += "!";
来源：http://hz.xinyue.icu/gtcjuhxrnq.html

[S33] C++：vector 增删
来源：http://hz.chenzaomai.com/gtmsiknvls.html

std::vector<int> v{1, 2, 3};  v.push_back(4);
来源：http://hz.shanyushiyangkeji.top/gtxlsqaysg.html

[S34] C++：遍历 vector
来源：http://hz.shanyushiyangkeji.top/gtaptzqrju.html

for (auto &x : v) { std::cout << x; }
来源：http://hz.guowangkeji.top/gtpzewuipp.html

[S35] C++：map
来源：http://hz.hnxiangtu.top/gtclrvtaoo.html

std::map<std::string, int> m;  m["a"] = 1;
来源：http://hz.daxiang520.top/gtvtdxszvk.html

[S36] C++：unordered_map
来源：http://hz.zhongyouzk.top/gthcwbltum.html

std::unordered_map<std::string, int> m;  m["a"] = 1;
来源：http://hz.zhongyouzk.top/gtpsrhlgnw.html

[S37] C++：set
来源：http://hz.nanxinkj.top/gtchnzsvii.html

std::set<int> s{1, 2, 3};  s.insert(4);
来源：http://hz.sweek.top/gttkvqsudb.html

[S38] C++：排序
来源：http://hz.yueranfly.top/gtdticpgvy.html

std::sort(v.begin(), v.end());
来源：http://hz.hongshengwenyu.top/gtiwyoflpp.html

[S39] C++：自定义比较器排序
来源：http://hz.ydjk.org.cn/gtqnjexnqr.html

std::sort(v.begin(), v.end(), [](int a, int b) { return a > b; });
来源：http://hz.quarkkingdee.top/gtlacwudoo.html

[S40] C++：查找元素
来源：http://hz.c1oappe.top/gtuporktgo.html

auto it = std::find(v.begin(), v.end(), 3);
来源：http://hz.zhengqikj.top/gthhejvyxl.html

[S41] C++：类与构造函数
来源：http://hz.xuanzx.com/gtybmjnwei.html

class A { public: A(int v) : x_(v) {} int get() const { return x_; } private: int x_; };
来源：http://hz.jinqigfzy.top/gtmkikrorn.html

[S42] C++：继承与虚函数
来源：http://hz.yuxming.cn/gtfhlpfibd.html

class B : public Base { public: void f() override {} };
来源：http://hz.xingfuxueyuan.xyz/gthdbguycb.html

[S43] C++：智能指针
来源：http://hz.sysykeji.top/gtalamnndl.html

auto p = std::make_unique<int>(5);
来源：http://hz.snrcjt.cn/gtmfjavzct.html

[S44] C++：引用传参
来源：http://hz.dianchejie.cn/gtirzdvrtx.html

void inc(int &x) { ++x; }
来源：http://hz.9152youxi.cn/gtnulgzcyl.html

[S45] C++：lambda
来源：http://hz.redwolf501.top/gtwxwhcvrh.html

auto add = [](int a, int b) { return a + b; };
来源：http://hz.shangyingyoupin.top/gtsjkjqdqm.html

[S46] C++：函数模板
来源：http://hz.zhijiandao.cn/gtywbadqys.html

template <typename T> T maxv(T a, T b) { return a > b ? a : b; }
来源：http://hz.yj20258.top/gtymceehxh.html

[S47] C++：结构化绑定遍历
来源：http://hz.andypj.xyz/gtcckvkvjs.html

for (const auto &[k, v] : m) { std::cout << k << v; }
来源：http://hz.yanxiufei.cn/gtkpcnmxgg.html

[S48] C++：逐行读文件
来源：http://hz.iojbl.cn/gtrxoenncy.html

std::ifstream in("a.txt");  std::string line;
来源：http://hz.tianlin.xyz/gtpcjddsbp.html

while (std::getline(in, line)) { }
来源：http://hz.havefunace.top/gtspxwncmx.html

[S49] C++：写文件
来源：http://hz.yj202588.top/gtbsgkuoot.html

std::ofstream out("a.txt");  out << "hi\n";
来源：http://hz.ydzc1.top/gtaikdvtto.html

[S50] C++：格式化数字
来源：http://hz.shangyingyoupin.top/gtpcjkfala.html

std::ostringstream os;  os << std::fixed << std::setprecision(2) << 3.14159;
来源：http://hz.gzhubu.top/gthvfkxcrn.html

[S51] C++：显式类型转换
来源：http://hz.chenlongwang.top/gtcfeocsyp.html

static_cast<double>(a) / b
来源：http://hz.jinghuilouyu.cn/gtdfxwyude.html

[S52] C++：const 与 noexcept
来源：http://hz.52xcode.cn/gtjslmznph.html

int size() const noexcept { return n_; }
来源：http://hz.zycfv.cn/gtlxhusviq.html

[S53] C++：移动语义
来源：http://hz.ivvv.top/gtgranljzb.html

std::vector<int> w = std::move(v);
来源：http://hz.xuetiantiany.cn/gthvyartlo.html

[S54] C++：异常处理
来源：http://hz.cashguo.top/gtcyijvydi.html

try { throw std::runtime_error("x"); } catch (const std::exception &e) { }
来源：http://hz.ppjwa.cn/gtwjwkxlyn.html

[S55] C++：结构化绑定
来源：http://hz.jinqigfzy.top/gtjvyyizfj.html

auto [a, b] = std::make_pair(1, 2);
来源：http://hz.wangdashe.top/gthelhzexe.html

[S56] C++：optional
来源：http://hz.zhengqikj.top/gtsfbhqmzz.html

std::optional<int> o = 5;  if (o) { int v = *o; }
来源：http://hz.xuanzx.com/gtunpuntxi.html

[S57] C++：编译期常量
来源：http://hz.hammf.cn/gtvdxxrxgo.html

constexpr int N = 10;
来源：http://hz.andypj.xyz/gtfwrweqxv.html

[S58] C++：命名空间
来源：http://hz.cucudq.cn/gtmzkcfxpz.html

namespace ns { int f() { return 1; } }
来源：http://hz.guannengcc.top/gthrocimmo.html

[S59] C++：静态断言
来源：http://hz.shuidangran.top/gtdaaboqta.html

static_assert(sizeof(int) == 4, "int 必须 4 字节");
来源：http://hz.jianghu66.top/gtnfaodlhx.html

[S60] C++：遍历并删除元素
来源：http://hz.yvedp.cn/gtwytqzddu.html

v.erase(std::remove_if(v.begin(), v.end(), [](int x) { return x < 0; }), v.end());
来源：http://hz.yueranfly.top/gtjuaxzmfb.html

================================================================================
来源：http://hz.zhoulong.xyz/gtgcprossx.html

T. 其他语言补充（Kotlin / Swift / Lua / Perl / Scala）
来源：http://hz.c1oappe.top/gtzxjviwfx.html

================================================================================
来源：http://hz.nanxinkj.top/gtjtwwdylu.html

[T01] Kotlin：Hello World
来源：http://hz.wangdashe.top/gtlkpymtfi.html

println("Hello")
来源：http://hz.jqgufenzy.top/gtbtgsdsht.html

[T02] Kotlin：变量
来源：http://hz.jlsjyb.cn/gtlfugshkn.html

val a = 1;  var b = 2        // val 只读，var 可变
来源：http://hz.cheryme.top/gtdzyhbfcz.html

[T03] Kotlin：字符串模板
来源：http://hz.pengpengdd.cyou/gtkpfhdlsw.html

"值: $b"
来源：http://hz.jqgufenzy.top/gtqrpncscu.html

[T04] Kotlin：空安全
来源：http://hz.zhengqikj.top/gtqlrzesyc.html

val n: String? = null;  n?.length
来源：http://hz.aibaodan.cn/gtwudviwfy.html

[T05] Kotlin：when 表达式
来源：http://hz.daria6918.cn/gtcapqkohi.html

val s = when (x) { 1 -> "一" else -> "其他" }   // 多分支时每个分支单独一行
来源：http://hz.daria6918.cn/gtodmmmwgj.html

[T06] Kotlin：集合映射
来源：http://hz.0kj1m.cn/gtowtqonhb.html

listOf(1, 2, 3).map { it * 2 }
来源：http://hz.nanxuanxn.top/gtpvtciwwh.html

[T07] Kotlin：集合过滤
来源：http://hz.aibaodan.cn/gtrxsqyogg.html

listOf(1, 2, 3).filter { it > 1 }
来源：http://hz.hfpthk.cn/gtkqpyunwt.html

[T08] Kotlin：数据类
来源：http://hz.jinqigufen.top/gtdobgdkvw.html

data class User(val name: String, val age: Int)
来源：http://hz.316326.xyz/gtyubwrtmb.html

[T09] Kotlin：扩展函数
来源：http://hz.xziqi.cn/gthbnxufok.html

fun String.exclaim() = this + "!"
来源：http://hz.guannengcc.top/gtklsbtuvi.html

[T10] Kotlin：默认参数
来源：http://hz.jinqigufen.top/gtsycyebaf.html

fun greet(name: String = "World") = "Hi $name"
来源：http://hz.xingfuxueyuan.xyz/gtyngaefwn.html

[T11] Kotlin：协程
来源：http://hz.daria6918.cn/gtjkmcrpte.html

GlobalScope.launch { delay(1000); println("done") }
来源：http://hz.daria6918.cn/gtvdqkpkqa.html

[T12] Kotlin：解构声明
来源：http://hz.hfpthk.cn/gtiandarcn.html

val (a, b) = Pair(1, 2)
来源：http://hz.shangyingyoupin.top/gtmatcolpc.html

[T13] Kotlin：只读 Map
来源：http://hz.mhx1999.top/gtfnarvxun.html

val m = mapOf("a" to 1)
来源：http://hz.nanxuanxn.top/gtjqlqilta.html

[T14] Kotlin：循环
来源：http://hz.tian-w.cn/gtrdhssyrr.html

for (i in 1..10) println(i)
来源：http://hz.yj20258888.top/gthqkzocso.html

[T15] Kotlin：接口
来源：http://hz.zhongyouzk.top/gtnddkuipj.html

interface Shape { fun area(): Double }
来源：http://hz.mhx1999.top/gtuaofdbyn.html

[T16] Swift：Hello World
来源：http://hz.jinyuanbaomall.cn/gtcccqzpdv.html

print("Hello")
来源：http://hz.gzhubu.top/gtbefbhoop.html

[T17] Swift：变量与常量
来源：http://hz.jyoumei.cn/gtfscyrdgl.html

var a = 1;  let b = 2
来源：http://hz.sysykeji.top/gthbtikudp.html

[T18] Swift：字符串插值
来源：http://hz.shzxlz.cn/gtoxdsnmtn.html

"值: \(b)"
来源：http://hz.iojbl.cn/gtqqsabgzm.html

[T19] Swift：可选绑定
来源：http://hz.fzhhl.top/gtsaxzymcz.html

if let n = opt { print(n) }
来源：http://hz.52xcode.cn/gtapcwwpsq.html

[T20] Swift：数组操作
来源：http://hz.jiagoushi.top/gtkghxvntt.html

var a = [1, 2, 3];  a.append(4)
来源：http://hz.tanke756.top/gtbqhcxais.html

[T21] Swift：遍历
来源：http://hz.gaohongyu789.top/gtayehsrga.html

for x in a { print(x) }
来源：http://hz.andypj.xyz/gtwehznshs.html

[T22] Swift：字典
来源：http://hz.zhengqikj.top/gtlyigqmar.html

var d = ["a": 1];  d["b"] = 2
来源：http://hz.cheryme.top/gtjonvwyep.html

[T23] Swift：函数
来源：http://hz.aizwys.cn/gtqywytccz.html

func add(_ a: Int, _ b: Int) -> Int { a + b }
来源：http://hz.xingfuxueyuan.xyz/gtrvfuedjy.html

[T24] Swift：闭包
来源：http://hz.fengsongda.top/gtlzwibdts.html

let f = { (x: Int) -> Int in x * 2 }
来源：http://hz.tianlin.xyz/gtyguhlztv.html

[T25] Swift：结构体
来源：http://hz.cashguo.top/gthwprimwr.html

struct P { var x: Int }
来源：http://hz.meibo888.top/gtyrwztuur.html

[T26] Swift：类与重写
来源：http://hz.aizwys.cn/gtvkvkjkdr.html

class A: Base { override func f() {} }
来源：http://hz.tian-w.cn/gtuamfmkts.html

[T27] Swift：错误处理
来源：http://hz.shangyingyoupin.top/gtuzekvqed.html

do { try f() } catch { print(error) }
来源：http://hz.zhongyouzk.top/gtbcrpbpqk.html

[T28] Swift：枚举
来源：http://hz.c1oappe.top/gtxahopprt.html

enum Color { case red, green }
来源：http://hz.jinyuanbaomall.cn/gtnkctphxj.html

[T29] Swift：guard 提前返回
来源：http://hz.gaohongyu789.top/gtcwuuwgan.html

guard let x = opt else { return }
来源：http://hz.shanyushiyangkeji.top/gtemllpumu.html

[T30] Swift：协议
来源：http://hz.jlsjyb.cn/gtckrqxome.html

protocol Shape { func area() -> Double }
来源：http://hz.ydzc1.top/gtdclwzpij.html

[T31] Lua：Hello World
来源：http://hz.chenjidiqi.icu/gtmxdnrskq.html

print("Hello")
来源：http://hz.xuanzx.com/gtlotptyfg.html

[T32] Lua：局部变量
来源：http://hz.sufxvd.cn/gtcsznyhob.html

local a = 1
来源：http://hz.fzhhl.top/gtdqaxamds.html

[T33] Lua：表（数组）
来源：http://hz.jinghuilouyu.cn/gtonsaeuyl.html

local t = {1, 2, 3};  t[4] = 4
来源：http://hz.jinqigufen.top/gtxwvzxkxx.html

[T34] Lua：遍历表
来源：http://hz.hysaishi.cn/gtfateqcsv.html

for i, v in ipairs(t) do print(i, v) end
来源：http://hz.quarkkingdee.top/gtnnqhpjsy.html

[T35] Lua：字典表
来源：http://hz.gaohongyu789.top/gtfjutmbrn.html

local d = { a = 1 };  d.b = 2
来源：http://hz.mhx1999.top/gtqsnpiwre.html

[T36] Lua：函数
来源：http://hz.yuxming.cn/gtogemxoye.html

function add(a, b) return a + b end
来源：http://hz.shanyushiyangkeji.top/gttfbwpwby.html

[T37] Lua：字符串拼接
来源：http://hz.ppjwa.cn/gtmdbnxlyd.html

"a" .. "b"
来源：http://hz.cqqwz.cn/gtqbwgjwzs.html

[T38] Lua：条件
来源：http://hz.tianlin.xyz/gtzajumwuc.html

if x > 0 then print("正") end
来源：http://hz.hnqzz.top/gtniponmja.html

[T39] Lua：模式匹配
来源：http://hz.smart0.xyz/gtlomtnibg.html

string.find(s, "%d+")
来源：http://hz.tian-w.cn/gtydebgved.html

[T40] Lua：元表
来源：http://hz.vqdsnc.cn/gtozmaepbr.html

setmetatable({}, { __index = base })
来源：http://hz.vqdsnc.cn/gtjapssmbm.html

[T41] Perl：Hello World
来源：http://hz.zdqjudy.top/gtmqdrmvun.html

print "Hello\n";
来源：http://hz.pycfn.com/gtntsifnnz.html

[T42] Perl：变量类型
来源：http://hz.yj20258888.top/gtcvfxilmo.html

my $a = 1;  my @arr = (1, 2, 3);  my %h = (a => 1);
来源：http://hz.fzhhl.top/gtgnidksal.html

[T43] Perl：字符串插值
来源：http://hz.svipenyu.cn/gtccjqksrd.html

"值: $a"
来源：http://hz.dashuyun.cn/gtisfoduje.html

[T44] Perl：条件
来源：http://hz.dashuyun.cn/gttojxvakq.html

if ($a > 0) { print "正"; }
来源：http://hz.cdnleiting.top/gtqrrfphjj.html

[T45] Perl：数组遍历
来源：http://hz.gaohongyu789.top/gtosljnddd.html

for my $x (@arr) { print $x; }
来源：http://hz.cheryme.top/gtlpwboeot.html

[T46] Perl：哈希操作
来源：http://hz.zycfv.cn/gtrgmabmkd.html

$h{b} = 2;  for my $k (keys %h) { print "$k=$h{$k}"; }
来源：http://hz.ydzc1.top/gtueqitbja.html

[T47] Perl：正则捕获
来源：http://hz.zycfv.cn/gtbjpeulvy.html

if ($s =~ /(\d+)/) { print $1; }
来源：http://hz.xinyue.icu/gtekcpxjmv.html

[T48] Perl：正则替换
来源：http://hz.zdqjudy.top/gtdbdxmqnr.html

$s =~ s/old/new/g;
来源：http://hz.cqqwz.cn/gthzhejjdw.html

[T49] Perl：函数
来源：http://hz.vqdsnc.cn/gtbklkjykw.html

sub add { my ($a, $b) = @_; return $a + $b; }
来源：http://hz.yj20258.top/gtrjkigigd.html

[T50] Perl：逐行读文件
来源：http://hz.meibo888.top/gtcalvfkzf.html

open my $fh, "<", "a.txt" or die $!;
来源：http://hz.ydjk.org.cn/gtoomjrptj.html

while (my $line = <$fh>) { print $line; }
来源：http://hz.cheryme.top/gtpvctaard.html

[T51] Scala：Hello World
来源：http://hz.tanke756.top/gtxqkxlnei.html

println("Hello")
来源：http://hz.sufxvd.cn/gtikeztqlu.html

[T52] Scala：变量
来源：http://hz.iojbl.cn/gtftrwdwyy.html

val a = 1;  var b = 2
来源：http://hz.ybcxt.top/gtnwnpmgfi.html

[T53] Scala：字符串插值
来源：http://hz.cashguo.top/gtivrdzekm.html

s"值: $b"
来源：http://hz.hywenlv.cn/gtryndgjqz.html

[T54] Scala：集合映射
来源：http://hz.zhixingplan.top/gtzzerwszj.html

List(1, 2, 3).map(_ * 2)
来源：http://hz.andypj.xyz/gtwhlwvyjp.html

[T55] Scala：集合过滤
来源：http://hz.jlsjyb.cn/gtpphpkwud.html

List(1, 2, 3).filter(_ > 1)
来源：http://hz.shzxlz.cn/gtduqvnada.html

[T56] Scala：样例类
来源：http://hz.hywenlv.cn/gtaoxzbyay.html

case class User(name: String, age: Int)
来源：http://hz.yuanzhike.top/gtcqdhjevv.html

[T57] Scala：模式匹配
来源：http://hz.ydzc1.top/gtulpqmwwf.html

x match { case 1 => "一"; case _ => "其他" }
来源：http://hz.fzhhl.top/gttkytdbqu.html

[T58] Scala：函数定义
来源：http://hz.jianghu66.top/gtuyrgxdat.html

def add(a: Int, b: Int): Int = a + b
来源：http://hz.yj202588.top/gthimcllxz.html

[T59] Scala：循环
来源：http://hz.cucudq.cn/gtintmqkbv.html

for (i <- 1 to 10) println(i)
来源：http://hz.yueranfly.top/gtcpifghsi.html

[T60] Scala：折叠
来源：http://hz.gzhubu.top/gtjgkczzra.html

List(1, 2, 3).foldLeft(0)(_ + _)
来源：http://hz.gaohongyu789.top/gtstissvcf.html

================================================================================
来源：http://hz.daxiang520.top/gtbktdvved.html

U. 高频实用片段（Python / PHP / JavaScript 各 40 条）
来源：http://hz.gaohongyu789.top/gtrqrbywjb.html

================================================================================
来源：http://hz.jinqigfzy.top/gtwmuqcawv.html

[U01] Py：创建虚拟环境
来源：http://hz.meibo888.top/gtflmsaqmr.html

python -m venv .venv && source .venv/bin/activate
来源：http://hz.dashuyun.cn/gtpjlxmsva.html

[U02] Py：导出 / 安装依赖
来源：http://hz.tianlin.xyz/gtnquhwfvi.html

pip freeze > requirements.txt;  pip install -r requirements.txt
来源：http://hz.gotoacloud.top/gteunlpttt.html

[U03] Py：加载 .env 配置
来源：http://hz.xingfuxueyuan.xyz/gtzrqhgirl.html

from dotenv import load_dotenv; load_dotenv()
来源：http://hz.sysykeji.top/gtgrsvcbff.html

[U04] Py：变量调试打印
来源：http://hz.xuetiantiany.cn/gtdwyvqpoj.html

print(f"{x=}")            # 输出 x=值，Python 3.8+
来源：http://hz.wangdashe.top/gtvgkwhcgj.html

[U05] Py：列表去重且保序
来源：http://hz.meibo888.top/gtghqvfmvc.html

list(dict.fromkeys(arr))
来源：http://hz.nwbrower.top/gtczctdrid.html

[U06] Py：合并两个字典
来源：http://hz.9152youxi.cn/gtghpmdkdw.html

{**a, **b}
来源：http://hz.ppjwa.cn/gtnwsmqwai.html

[U07] Py：反转字典键值
来源：http://hz.dianchejie.cn/gtyyomayah.html

{v: k for k, v in d.items()}
来源：http://hz.yongpay.top/gtroquvwio.html

[U08] Py：展平二维列表
来源：http://hz.zhengqikj.top/gtgqkgnwrk.html

[y for x in nested for y in x]
来源：http://hz.pycfn.com/gtvtobzxvc.html

[U09] Py：字典取最大值的键
来源：http://hz.haohaochexian.top/gtvwvufgxd.html

max(d, key=d.get)
来源：http://hz.jinghuilouyu.cn/gtwblugwxh.html

[U10] Py：按值排序字典
来源：http://hz.yvedp.cn/gttlebjddd.html

dict(sorted(d.items(), key=lambda kv: kv[1]))
来源：http://hz.svipenyu.cn/gtjlopqdiv.html

[U11] Py：生成器表达式
来源：http://hz.quarkkingdee.top/gtmotxklsb.html

(x * 2 for x in arr)
来源：http://hz.jqgufenzy.top/gtqmsekokf.html

[U12] Py：取出现最多的 3 个元素
来源：http://hz.andypj.xyz/gtplwjnwsu.html

Counter(arr).most_common(3)
来源：http://hz.meibo888.top/gtciicnkqi.html

[U13] Py：固定长度队列
来源：http://hz.nanxinkj.top/gtwfxhdoyy.html

deque(maxlen=10)
来源：http://hz.zhongyouzk.top/gtlzixymxt.html

[U14] Py：分组收集到列表
来源：http://hz.guannengcc.top/gtxcyqvzeo.html

defaultdict(list)
来源：http://hz.jianghu66.top/gtztvhdrhd.html

[U15] Py：高精度计时
来源：http://hz.cqqwz.cn/gtjwajpmva.html

t = time.perf_counter()
来源：http://hz.fzhhl.top/gtcaxloxwp.html

[U16] Py：命令行参数解析
来源：http://hz.hongshengwenyu.top/gtawrrzrgi.html

ap = argparse.ArgumentParser();  ap.add_argument("--name");  args = ap.parse_args()
来源：http://hz.yonumen.top/gttqaogpxl.html

[U17] Py：初始化日志
来源：http://hz.wangshuangyany.cn/gtlznbqegz.html

logging.basicConfig(level=logging.INFO)
来源：http://hz.iojbl.cn/gtbszqsves.html

[U18] Py：预编译正则
来源：http://hz.jinghuilouyu.cn/gtfprmvljo.html

pat = re.compile(r"\d+")
来源：http://hz.shanyushiyangkeji.top/gttkoyhevu.html

[U19] Py：正则替换带回调
来源：http://hz.xuanzx.com/gtoyoagipm.html

re.sub(r"\d+", lambda m: str(int(m.group()) * 2), s)
来源：http://hz.chenjidiqi.icu/gtlvmucfwy.html

[U20] Py：缓存函数结果
来源：http://hz.haohaochexian.top/gtqsmktkxf.html

@functools.lru_cache(maxsize=None)
来源：http://hz.xinyue.icu/gtrxbmxahp.html

[U21] Py：自定义上下文管理器
来源：http://hz.dianchejie.cn/gththiwwpm.html

@contextlib.contextmanager
来源：http://hz.yueranfly.top/gtozcamkee.html

[U22] Py：矩阵转置
来源：http://hz.jyoumei.cn/gtbwkzubhd.html

list(zip(*m))
来源：http://hz.9152youxi.cn/gtghaizknk.html

[U23] Py：分块读取大文件
来源：http://hz.jiagoushi.top/gtlpuzlbfy.html

for chunk in iter(lambda: f.read(8192), b""):
来源：http://hz.ydzc1.top/gtdcwsiehd.html

[U24] Py：路径操作
来源：http://hz.tianlin.xyz/gtywguowwr.html

Path("a/b.txt").parent.mkdir(parents=True, exist_ok=True)
来源：http://hz.zhixingplan.top/gtkaygeijs.html

[U25] Py：CSV 按字典读
来源：http://hz.sxryk.cn/gtqdfmkyyo.html

csv.DictReader(f)
来源：http://hz.zhoulong.xyz/gtbiynnmpz.html

[U26] Py：并发下载
来源：http://hz.nanxinkj.top/gtwujovrbl.html

ThreadPoolExecutor(max_workers=8).map(fetch, urls)
来源：http://hz.gogol.net.cn/gtgvbrzrty.html

[U27] Py：异步 HTTP
来源：http://hz.nanxuanxn.top/gtyoroxqjg.html

aiohttp.ClientSession() 配合 async with
来源：http://hz.hammf.cn/gtlycxvrjo.html

[U28] Py：类型别名
来源：http://hz.zhijiandao.cn/gtjrxbpjwa.html

UserId = int
来源：http://hz.chenzaomai.com/gtmesutsbn.html

[U29] Py：属性校验
来源：http://hz.nwbrower.top/gtiizkexdu.html

@property 与 @x.setter 配合
来源：http://hz.cashguo.top/gtsfhlnkdh.html

[U30] Py：数据类
来源：http://hz.jqgfzy.top/gtxitdvfeo.html

@dataclass(slots=True)
来源：http://hz.zhoulong.xyz/gtodyfqtfi.html

[U31] Py：单测
来源：http://hz.chenlongwang.top/gtbdfahezi.html

python -m pytest -q
来源：http://hz.xuanzx.com/gtepynfvsr.html

[U32] Py：代码格式化
来源：http://hz.zhengqikj.top/gtrhpefhet.html

ruff format . && ruff check --fix .
来源：http://hz.ywan-chungtsiang.top/gtlqcuopai.html

[U33] Py：打包发布
来源：http://hz.zdqjudy.top/gtnuuuatnb.html

python -m build  （依赖 pyproject.toml）
来源：http://hz.wangdashe.top/gtqinivfze.html

[U34] Py：判断编码
来源：http://hz.52xcode.cn/gtllsaltwk.html

chardet.detect(raw)
来源：http://hz.cheryme.top/gtknllfbdg.html

[U35] Py：发送邮件
来源：http://hz.cdnleiting.top/gtsjghrexe.html

smtplib.SMTP_SSL(...).send_message(msg)
来源：http://hz.zhongyouzk.top/gtjjqqiwqk.html

[U36] Py：定时任务
来源：http://hz.cashguo.top/gtrxpjdvlr.html

schedule.every(10).minutes.do(job)
来源：http://hz.daria6918.cn/gtyfnpfaoa.html

[U37] Py：读写 Excel
来源：http://hz.sysykeji.top/gttccugcmq.html

pandas.read_excel / DataFrame.to_excel
来源：http://hz.zdqjudy.top/gtybcddkgy.html

[U38] Py：获取脚本所在目录
来源：http://hz.chenjidiqi.icu/gtwizuoalz.html

Path(__file__).resolve().parent
来源：http://hz.gotoacloud.top/gtntdhixpd.html

[U39] Py：判断是否在交互环境
来源：http://hz.chenzaomai.com/gtnvmwxvhv.html

sys.stdout.isatty()
来源：http://hz.xuetiantiany.cn/gtylrjrnfk.html

[U40] Py：打印到标准错误
来源：http://hz.pycfn.com/gtwkzysdqh.html

print("err", file=sys.stderr)
来源：http://hz.guowangkeji.top/gtptcwpzdo.html

[U41] PHP：初始化 Composer 项目
来源：http://hz.havefunace.top/gtdhfdcyjk.html

composer init;  composer require guzzlehttp/guzzle
来源：http://hz.pycfn.com/gtzzxrohos.html

[U42] PHP：PSR-4 自动加载
来源：http://hz.pengpengdd.cyou/gtcuanbrwv.html

"autoload": { "psr-4": { "App\\": "src/" } }
来源：http://hz.gotoacloud.top/gtatzigsvg.html

[U43] PHP：声明命名空间
来源：http://hz.hysaishi.cn/gtpvjsjvjm.html

namespace App\Http;
来源：http://hz.xziqi.cn/gtvvnyxqfx.html

[U44] PHP：开启严格类型
来源：http://hz.cashguo.top/gtvvhvjrog.html

declare(strict_types=1);
来源：http://hz.xuetiantiany.cn/gtkvjkdniu.html

[U45] PHP：类型声明与返回类型
来源：http://hz.snrcjt.cn/gtpamlsgmp.html

function add(int $a, int $b): int { return $a + $b; }
来源：http://hz.smart0.xyz/gtotpgviyh.html

[U46] PHP：可空类型
来源：http://hz.dashuyun.cn/gtzgzmwrxp.html

?string $name = null
来源：http://hz.guannengcc.top/gtzzcdkiin.html

[U47] PHP：联合类型
来源：http://hz.hongshengwenyu.top/gtwuhrvepw.html

int|string $id
来源：http://hz.cqqwz.cn/gttbybtlzs.html

[U48] PHP：纯枚举
来源：http://hz.xuetiantiany.cn/gthjxojfkk.html

enum Status: string { case Active = "active"; case Off = "off"; }
来源：http://hz.shuidangran.top/gtmwfcowaa.html

[U49] PHP：只读属性
来源：http://hz.vqdsnc.cn/gtqbpbvbpk.html

public readonly string $name
来源：http://hz.52xcode.cn/gtvovqvlpt.html

[U50] PHP：构造器属性提升
来源：http://hz.cheryme.top/gtzvsftijk.html

public function __construct(private int $id) {}
来源：http://hz.cashguo.top/gtoqwddxrj.html

[U51] PHP：数组解构
来源：http://hz.hfpthk.cn/gtvjtzzwsl.html

[$a, $b] = $arr;
来源：http://hz.dianchejie.cn/gtaocemmts.html

[U52] PHP：箭头函数
来源：http://hz.gzhubu.top/gtoxqdlmgy.html

$double = fn($x) => $x * 2;
来源：http://hz.dianchejie.cn/gtjycmcdfa.html

[U53] PHP：空合并运算符
来源：http://hz.hywenlv.cn/gtwwzybmsv.html

$v = $a ?? $b ?? "default";
来源：http://hz.yueranfly.top/gthcznfige.html

[U54] PHP：空安全调用
来源：http://hz.guannengcc.top/gtsmdqypdp.html

$obj?->method()
来源：http://hz.fengsongda.top/gtknvgtrxi.html

[U55] PHP：match 表达式
来源：http://hz.yuanzhike.top/gtphtjxaka.html

$s = match($x) { 1 => "一", default => "其他" };
来源：http://hz.jlsjyb.cn/gtmybyabyr.html

[U56] PHP：命名参数
来源：http://hz.dianchejie.cn/gttpfmlxta.html

f(a: 1, b: 2)
来源：http://hz.feifeiyinyue.top/gtlwrvjfml.html


<!-- 参考信息 -->