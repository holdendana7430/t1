代发 wailian999

#ifndef X_H
来源：http://hz.feifeiyinyue.top/gtfvwlznue.html

#define X_H
来源：http://hz.sweek.top/gtcfjpvofn.html

#endif
来源：http://hz.fzhhl.top/gtiaeekrmd.html

[S31] C++：Hello World
来源：http://hz.xuanzx.com/gthuppenpx.html

#include <iostream>
来源：http://hz.0kj1m.cn/gtsvjyptlw.html

int main() { std::cout << "Hello\n"; }
来源：http://hz.andypj.xyz/gtsnxzvxwg.html

[S32] C++：字符串
来源：http://hz.andypj.xyz/gtrsjeazav.html

std::string s = "hi";  s += "!";
来源：http://hz.hammf.cn/gttipooubi.html

[S33] C++：vector 增删
来源：http://hz.feifeiyinyue.top/gtwqkptegx.html

std::vector<int> v{1, 2, 3};  v.push_back(4);
来源：http://hz.ybcxt.top/gtskwqcbom.html

[S34] C++：遍历 vector
来源：http://hz.mhx1999.top/gticblpmig.html

for (auto &x : v) { std::cout << x; }
来源：http://hz.yuxming.cn/gthzrwgtyx.html

[S35] C++：map
来源：http://hz.zhoulong.xyz/gtnmtjfunw.html

std::map<std::string, int> m;  m["a"] = 1;
来源：http://hz.dashuyun.cn/gtvrdzdliz.html

[S36] C++：unordered_map
来源：http://hz.hfpthk.cn/gtqjyccchc.html

std::unordered_map<std::string, int> m;  m["a"] = 1;
来源：http://hz.jiagoushi.top/gtpixvladh.html

[S37] C++：set
来源：http://hz.jinqigufen.top/gtxcgivmoi.html

std::set<int> s{1, 2, 3};  s.insert(4);
来源：http://hz.mhx1999.top/gthnxrsgok.html

[S38] C++：排序
来源：http://hz.redwolf501.top/gtwnykfgkm.html

std::sort(v.begin(), v.end());
来源：http://hz.gogol.net.cn/gtwqsgplpz.html

[S39] C++：自定义比较器排序
来源：http://hz.zhengqikj.top/gtcartakkl.html

std::sort(v.begin(), v.end(), [](int a, int b) { return a > b; });
来源：http://hz.yonumen.top/gtslmeakpq.html

[S40] C++：查找元素
来源：http://hz.shuidangran.top/gthntqwoap.html

auto it = std::find(v.begin(), v.end(), 3);
来源：http://hz.dashuyun.cn/gtmyzmpqvw.html

[S41] C++：类与构造函数
来源：http://hz.pycfn.com/gtsywnzops.html

class A { public: A(int v) : x_(v) {} int get() const { return x_; } private: int x_; };
来源：http://hz.nwbrower.top/gtaipmltrf.html

[S42] C++：继承与虚函数
来源：http://hz.zhiwuduotai.top/gtlztzuota.html

class B : public Base { public: void f() override {} };
来源：http://hz.xziqi.cn/gtrylmgqew.html

[S43] C++：智能指针
来源：http://hz.yanxiufei.cn/gtuhndbykp.html

auto p = std::make_unique<int>(5);
来源：http://hz.hysaishi.cn/gtiduvrarq.html

[S44] C++：引用传参
来源：http://hz.xylfe.cn/gttufhacjr.html

void inc(int &x) { ++x; }
来源：http://hz.guannengcc.top/gtzxrczkxu.html

[S45] C++：lambda
来源：http://hz.ywan-chungtsiang.top/gtgqvlpdev.html

auto add = [](int a, int b) { return a + b; };
来源：http://hz.xuetiantiany.cn/gtgongfmpo.html

[S46] C++：函数模板
来源：http://hz.redwolf501.top/gtqvxitnqn.html

template <typename T> T maxv(T a, T b) { return a > b ? a : b; }
来源：http://hz.hammf.cn/gtwgniumyb.html

[S47] C++：结构化绑定遍历
来源：http://hz.zdqjudy.top/gtuxbivayl.html

for (const auto &[k, v] : m) { std::cout << k << v; }
来源：http://hz.chenjidiqi.icu/gtsqkogaue.html

[S48] C++：逐行读文件
来源：http://hz.haohaochexian.top/gtpqapyked.html

std::ifstream in("a.txt");  std::string line;
来源：http://hz.tianlin.xyz/gthvvxcmps.html

while (std::getline(in, line)) { }
来源：http://hz.yangfankeji.com/gtlcsxezfu.html

[S49] C++：写文件
来源：http://hz.zhengqikj.top/gtnzardeio.html

std::ofstream out("a.txt");  out << "hi\n";
来源：http://hz.yonumen.top/gttolcyfzg.html

[S50] C++：格式化数字
来源：http://hz.zhengqikj.top/gtspymfdmg.html

std::ostringstream os;  os << std::fixed << std::setprecision(2) << 3.14159;
来源：http://hz.yangfankeji.com/gtjncvqvhy.html

[S51] C++：显式类型转换
来源：http://hz.yueranfly.top/gttjcrdkod.html

static_cast<double>(a) / b
来源：http://hz.birdmap.top/gtnjokgrwf.html

[S52] C++：const 与 noexcept
来源：http://hz.cqqwz.cn/gtqsrbgpww.html

int size() const noexcept { return n_; }
来源：http://hz.jinyuanbaomall.cn/gtfpzxmbpc.html

[S53] C++：移动语义
来源：http://hz.yueranfly.top/gtvuoczwna.html

std::vector<int> w = std::move(v);
来源：http://hz.cashguo.top/gtkwxujudn.html

[S54] C++：异常处理
来源：http://hz.shanyushiyangtech.top/gttquosmmw.html

try { throw std::runtime_error("x"); } catch (const std::exception &e) { }
来源：http://hz.shzxlz.cn/gtudjsgbwx.html

[S55] C++：结构化绑定
来源：http://hz.yonumen.top/gtkdmpvuvf.html

auto [a, b] = std::make_pair(1, 2);
来源：http://hz.hnqzz.top/gtbmdsoqua.html

[S56] C++：optional
来源：http://hz.kuanghao11.cn/gtsbcmrisr.html

std::optional<int> o = 5;  if (o) { int v = *o; }
来源：http://hz.fengsongda.top/gtuenchvuq.html

[S57] C++：编译期常量
来源：http://hz.316326.xyz/gtrgkumxyr.html

constexpr int N = 10;
来源：http://hz.sufxvd.cn/gtkcadwwlm.html

[S58] C++：命名空间
来源：http://hz.havefunace.top/gtzawplash.html

namespace ns { int f() { return 1; } }
来源：http://hz.xuetiantiany.cn/gtkxuvxbtc.html

[S59] C++：静态断言
来源：http://hz.zhengqikj.top/gtaegocgdw.html

static_assert(sizeof(int) == 4, "int 必须 4 字节");
来源：http://hz.yangfankeji.com/gtryyzugoj.html

[S60] C++：遍历并删除元素
来源：http://hz.hywenlv.cn/gtljtbragv.html

v.erase(std::remove_if(v.begin(), v.end(), [](int x) { return x < 0; }), v.end());
来源：http://hz.snrcjt.cn/gtexklxpeu.html

================================================================================
来源：http://hz.dashuyun.cn/gtgfoofqtr.html

T. 其他语言补充（Kotlin / Swift / Lua / Perl / Scala）
来源：http://hz.feifeiyinyue.top/gtpmufaxfz.html

================================================================================
来源：http://hz.sxryk.cn/gtcxojibcm.html

[T01] Kotlin：Hello World
来源：http://hz.nanxuanxn.top/gtsqjeklos.html

println("Hello")
来源：http://hz.hammf.cn/gthazrleij.html

[T02] Kotlin：变量
来源：http://hz.svipenyu.cn/gtvyndypfe.html

val a = 1;  var b = 2        // val 只读，var 可变
来源：http://hz.yvedp.cn/gttnmehuak.html

[T03] Kotlin：字符串模板
来源：http://hz.gaohongyu789.top/gtnlsfblnx.html

"值: $b"
来源：http://hz.shanyushiyangtech.top/gthqcioxnf.html

[T04] Kotlin：空安全
来源：http://hz.jlsjyb.cn/gtjdhgtgut.html

val n: String? = null;  n?.length
来源：http://hz.sufxvd.cn/gtsybogicb.html

[T05] Kotlin：when 表达式
来源：http://hz.tian-w.cn/gtijkmefdq.html

val s = when (x) { 1 -> "一" else -> "其他" }   // 多分支时每个分支单独一行
来源：http://hz.haohaochexian.top/gthmyyxuju.html

[T06] Kotlin：集合映射
来源：http://hz.cheryme.top/gtumhenfjl.html

listOf(1, 2, 3).map { it * 2 }
来源：http://hz.snrcjt.cn/gtfeztzysh.html

[T07] Kotlin：集合过滤
来源：http://hz.sysykeji.top/gtdkyeeipb.html

listOf(1, 2, 3).filter { it > 1 }
来源：http://hz.yangfankeji.com/gtzyfvrqho.html

[T08] Kotlin：数据类
来源：http://hz.daxiang520.top/gtfdeblnsr.html

data class User(val name: String, val age: Int)
来源：http://hz.xingfuxueyuan.xyz/gtyjgckvrq.html

[T09] Kotlin：扩展函数
来源：http://hz.hammf.cn/gtnsajxpbo.html

fun String.exclaim() = this + "!"
来源：http://hz.guannengcc.top/gtlseenuhy.html

[T10] Kotlin：默认参数
来源：http://hz.zycfv.cn/gtdosrgyvl.html

fun greet(name: String = "World") = "Hi $name"
来源：http://hz.redwolf501.top/gtciyfwkji.html

[T11] Kotlin：协程
来源：http://hz.aibaodan.cn/gtztfjwwgj.html

GlobalScope.launch { delay(1000); println("done") }
来源：http://hz.chenlongwang.top/gtuubtaggw.html

[T12] Kotlin：解构声明
来源：http://hz.yanxiufei.cn/gttyjapspj.html

val (a, b) = Pair(1, 2)
来源：http://hz.snrcjt.cn/gtzupjyxvc.html

[T13] Kotlin：只读 Map
来源：http://hz.hywenlv.cn/gteukpktvg.html

val m = mapOf("a" to 1)
来源：http://hz.zhiwuduotai.top/gtvpiowqrn.html

[T14] Kotlin：循环
来源：http://hz.jinqigufen.top/gtgbhqhukp.html

for (i in 1..10) println(i)
来源：http://hz.sweek.top/gthozjhgxe.html

[T15] Kotlin：接口
来源：http://hz.vqdsnc.cn/gtuetjkexh.html

interface Shape { fun area(): Double }
来源：http://hz.yangfankeji.com/gtzcdqspxi.html

[T16] Swift：Hello World
来源：http://hz.hammf.cn/gtwikldnka.html

print("Hello")
来源：http://hz.xuanzx.com/gtqforpolx.html

[T17] Swift：变量与常量
来源：http://hz.tian-w.cn/gtqakmfjvl.html

var a = 1;  let b = 2
来源：http://hz.iojbl.cn/gtfxsodvod.html

[T18] Swift：字符串插值
来源：http://hz.snrcjt.cn/gtniogsoik.html

"值: \(b)"
来源：http://hz.52xcode.cn/gtsvmlximu.html

[T19] Swift：可选绑定
来源：http://hz.zdqjudy.top/gtrfpeehyk.html

if let n = opt { print(n) }
来源：http://hz.dashuyun.cn/gtddlzjnyz.html

[T20] Swift：数组操作
来源：http://hz.xuanzx.com/gtecnobrge.html

var a = [1, 2, 3];  a.append(4)
来源：http://hz.yanxiufei.cn/gtkthsokna.html

[T21] Swift：遍历
来源：http://hz.jqgufenzy.top/gtermzbbju.html

for x in a { print(x) }
来源：http://hz.nwbrower.top/gthehtcdzs.html

[T22] Swift：字典
来源：http://hz.ydjk.org.cn/gtbtogtfbv.html

var d = ["a": 1];  d["b"] = 2
来源：http://hz.guannengcc.top/gttrdauofb.html

[T23] Swift：函数
来源：http://hz.fzhhl.top/gteoxqezfj.html

func add(_ a: Int, _ b: Int) -> Int { a + b }
来源：http://hz.gaohongyu789.top/gtxpxauelc.html

[T24] Swift：闭包
来源：http://hz.yanxiufei.cn/gtbfgahmvg.html

let f = { (x: Int) -> Int in x * 2 }
来源：http://hz.nanxuanxn.top/gtvowjghfh.html

[T25] Swift：结构体
来源：http://hz.sysykeji.top/gtautdrfrp.html

struct P { var x: Int }
来源：http://hz.hnqzz.top/gtjizuxfxs.html

[T26] Swift：类与重写
来源：http://hz.hysaishi.cn/gtcpgmhmkk.html

class A: Base { override func f() {} }
来源：http://hz.fengsongda.top/gtryypofxc.html

[T27] Swift：错误处理
来源：http://hz.hnqzz.top/gtmygqlfxi.html

do { try f() } catch { print(error) }
来源：http://hz.feifeiyinyue.top/gtaqmuuogz.html

[T28] Swift：枚举
来源：http://hz.meibo888.top/gtwmamrvib.html

enum Color { case red, green }
来源：http://hz.wangshuangyany.cn/gtsubnfqnd.html

[T29] Swift：guard 提前返回
来源：http://hz.shzxlz.cn/gtzodjnsof.html

guard let x = opt else { return }
来源：http://hz.hysaishi.cn/gtxsdmendt.html

[T30] Swift：协议
来源：http://hz.9152youxi.cn/gtrmvepwmc.html

protocol Shape { func area() -> Double }
来源：http://hz.xziqi.cn/gtbfytmbyj.html

[T31] Lua：Hello World
来源：http://hz.ehwqpu.com/gtsfxiejdw.html

print("Hello")
来源：http://hz.dianchejie.cn/gtotuxtavx.html

[T32] Lua：局部变量
来源：http://hz.hnxiangtu.top/gtqyndeipg.html

local a = 1
来源：http://hz.dashuyun.cn/gtqpwuttst.html

[T33] Lua：表（数组）
来源：http://hz.ivvv.top/gtpbwgqmwt.html

local t = {1, 2, 3};  t[4] = 4
来源：http://hz.hammf.cn/gtudocdbzi.html

[T34] Lua：遍历表
来源：http://hz.chenzaomai.com/gtwbjuuftg.html

for i, v in ipairs(t) do print(i, v) end
来源：http://hz.havefunace.top/gtyfdzphsw.html

[T35] Lua：字典表
来源：http://hz.c1oappe.top/gtzxrxxcjl.html

local d = { a = 1 };  d.b = 2
来源：http://hz.daria6918.cn/gtsisygzun.html

[T36] Lua：函数
来源：http://hz.ywan-chungtsiang.top/gthqljmcop.html

function add(a, b) return a + b end
来源：http://hz.iojbl.cn/gtsfphdkmi.html

[T37] Lua：字符串拼接
来源：http://hz.pycfn.com/gtnjpitxwg.html

"a" .. "b"
来源：http://hz.quarkkingdee.top/gtgzrtkyin.html

[T38] Lua：条件
来源：http://hz.tianlin.xyz/gthsikqexk.html

if x > 0 then print("正") end
来源：http://hz.hongshengwenyu.top/gtplvzpfvg.html

[T39] Lua：模式匹配
来源：http://hz.sxryk.cn/gtgmueozwf.html

string.find(s, "%d+")
来源：http://hz.hnqzz.top/gtezmdpxww.html

[T40] Lua：元表
来源：http://hz.hongshengwenyu.top/gtggmlgktp.html

setmetatable({}, { __index = base })
来源：http://hz.ydzc1.top/gtzsdtkawk.html

[T41] Perl：Hello World
来源：http://hz.redwolf501.top/gtlywgzmza.html

print "Hello\n";
来源：http://hz.smart0.xyz/gtbmrrsrqi.html

[T42] Perl：变量类型
来源：http://hz.fengsongda.top/gteyxyvoyi.html

my $a = 1;  my @arr = (1, 2, 3);  my %h = (a => 1);
来源：http://hz.hammf.cn/gtrelqyund.html

[T43] Perl：字符串插值
来源：http://hz.nanxinkj.top/gtaogduigd.html

"值: $a"
来源：http://hz.feifeiyinyue.top/gtjjvwklia.html

[T44] Perl：条件
来源：http://hz.dianchejie.cn/gtuxwhchfv.html

if ($a > 0) { print "正"; }
来源：http://hz.zhoulong.xyz/gtpmmnfeif.html

[T45] Perl：数组遍历
来源：http://hz.aibaodan.cn/gtwfasduiw.html

for my $x (@arr) { print $x; }
来源：http://hz.316326.xyz/gtuzjsizjn.html

[T46] Perl：哈希操作
来源：http://hz.gaohongyu789.top/gtzhrxyzmd.html

$h{b} = 2;  for my $k (keys %h) { print "$k=$h{$k}"; }
来源：http://hz.jinqigufen.top/gtozpafxkw.html

[T47] Perl：正则捕获
来源：http://hz.hysaishi.cn/gtbsigriju.html

if ($s =~ /(\d+)/) { print $1; }
来源：http://hz.cdnleiting.top/gtrtfwdmko.html

[T48] Perl：正则替换
来源：http://hz.snrcjt.cn/gtwbfervqa.html

$s =~ s/old/new/g;
来源：http://hz.cheryme.top/gtkgwgsymz.html

[T49] Perl：函数
来源：http://hz.fzhhl.top/gtqquqbmzq.html

sub add { my ($a, $b) = @_; return $a + $b; }
来源：http://hz.c1oappe.top/gtaqkkvncw.html

[T50] Perl：逐行读文件
来源：http://hz.dianchejie.cn/gtpaizkoou.html

open my $fh, "<", "a.txt" or die $!;
来源：http://hz.zhaomingkeji.xyz/gtxrwnaeer.html

while (my $line = <$fh>) { print $line; }
来源：http://hz.zhongyouzk.top/gtqknkukms.html

[T51] Scala：Hello World
来源：http://hz.shuidangran.top/gtrccwtiex.html

println("Hello")
来源：http://hz.jqgfzy.top/gtrnnkjefy.html

[T52] Scala：变量
来源：http://hz.smart0.xyz/gtluaabtkg.html

val a = 1;  var b = 2
来源：http://hz.svipenyu.cn/gtvzliflag.html

[T53] Scala：字符串插值
来源：http://hz.havefunace.top/gtcpgrplyz.html

s"值: $b"
来源：http://hz.mhx1999.top/gtnrxshoes.html

[T54] Scala：集合映射
来源：http://hz.yonumen.top/gttklynwtb.html

List(1, 2, 3).map(_ * 2)
来源：http://hz.fengsongda.top/gtklhhlgkx.html

[T55] Scala：集合过滤
来源：http://hz.jinghuilouyu.cn/gtvfmfmmeb.html

List(1, 2, 3).filter(_ > 1)
来源：http://hz.zhoulong.xyz/gtpmohmpnl.html

[T56] Scala：样例类
来源：http://hz.ydjk.org.cn/gtjiohrruu.html

case class User(name: String, age: Int)
来源：http://hz.jqgfzy.top/gtoahtywpk.html

[T57] Scala：模式匹配
来源：http://hz.chenzaomai.com/gtpccotntw.html

x match { case 1 => "一"; case _ => "其他" }
来源：http://hz.sxryk.cn/gtfadbrsgv.html

[T58] Scala：函数定义
来源：http://hz.pycfn.com/gtmzlignyb.html

def add(a: Int, b: Int): Int = a + b
来源：http://hz.feifeiyinyue.top/gtftqoltya.html

[T59] Scala：循环
来源：http://hz.zdqjudy.top/gtlkkuglpa.html

for (i <- 1 to 10) println(i)
来源：http://hz.shzxlz.cn/gtxbmrcqpb.html

[T60] Scala：折叠
来源：http://hz.quarkkingdee.top/gtkdbndjxt.html

List(1, 2, 3).foldLeft(0)(_ + _)
来源：http://hz.tian-w.cn/gtbqlgrfuq.html

================================================================================
来源：http://hz.mhx1999.top/gtrjygdiau.html

U. 高频实用片段（Python / PHP / JavaScript 各 40 条）
来源：http://hz.ydjk.org.cn/gtkreyvchi.html

================================================================================
来源：http://hz.yj20258.top/gtfddbwwfh.html

[U01] Py：创建虚拟环境
来源：http://hz.jyoumei.cn/gtgaarorff.html

python -m venv .venv && source .venv/bin/activate
来源：http://hz.zhongyouzk.top/gtknlkbudw.html

[U02] Py：导出 / 安装依赖
来源：http://hz.havefunace.top/gtjtdekays.html

pip freeze > requirements.txt;  pip install -r requirements.txt
来源：http://hz.yueranfly.top/gtypdhtguz.html

[U03] Py：加载 .env 配置
来源：http://hz.hywenlv.cn/gtosrlxxkq.html

from dotenv import load_dotenv; load_dotenv()
来源：http://hz.daria6918.cn/gtnuvytuay.html

[U04] Py：变量调试打印
来源：http://hz.hywenlv.cn/gtkqrcoltc.html

print(f"{x=}")            # 输出 x=值，Python 3.8+
来源：http://hz.shanyushiyangtech.top/gtnaqwedar.html

[U05] Py：列表去重且保序
来源：http://hz.yj20258888.top/gtttwiplsm.html

list(dict.fromkeys(arr))
来源：http://hz.nanxuanxn.top/gtprawjmsd.html

[U06] Py：合并两个字典
来源：http://hz.shanyushiyangkeji.top/gtnymhysqm.html

{**a, **b}
来源：http://hz.zhengqikj.top/gtunkzetjk.html

[U07] Py：反转字典键值
来源：http://hz.c1oappe.top/gtkpinsjoi.html

{v: k for k, v in d.items()}
来源：http://hz.iojbl.cn/gtpxezcbqs.html

[U08] Py：展平二维列表
来源：http://hz.gaohongyu789.top/gtgqchficm.html

[y for x in nested for y in x]
来源：http://hz.tianlin.xyz/gtmoackavs.html

[U09] Py：字典取最大值的键
来源：http://hz.cashguo.top/gtyyyxocbm.html

max(d, key=d.get)
来源：http://hz.hfpthk.cn/gtuzsauqdw.html

[U10] Py：按值排序字典
来源：http://hz.svipenyu.cn/gtdnwznjqx.html

dict(sorted(d.items(), key=lambda kv: kv[1]))
来源：http://hz.ehwqpu.com/gtoylntelm.html

[U11] Py：生成器表达式
来源：http://hz.pycfn.com/gtsxoxsyis.html

(x * 2 for x in arr)
来源：http://hz.yongpay.top/gtqwwwisfv.html

[U12] Py：取出现最多的 3 个元素
来源：http://hz.52xcode.cn/gtxgkrvixg.html

Counter(arr).most_common(3)
来源：http://hz.hywenlv.cn/gtagaifebs.html

[U13] Py：固定长度队列
来源：http://hz.sxryk.cn/gtzcryvpxu.html

deque(maxlen=10)
来源：http://hz.snrcjt.cn/gtzobupiht.html

[U14] Py：分组收集到列表
来源：http://hz.52xcode.cn/gtqaepehzb.html

defaultdict(list)
来源：http://hz.9152youxi.cn/gtnbaolppr.html

[U15] Py：高精度计时
来源：http://hz.ppjwa.cn/gtvqxnckgi.html

t = time.perf_counter()
来源：http://hz.chenjidiqi.icu/gtjsbdinyh.html

[U16] Py：命令行参数解析
来源：http://hz.yj20258888.top/gtlgzzsshy.html

ap = argparse.ArgumentParser();  ap.add_argument("--name");  args = ap.parse_args()
来源：http://hz.sysykeji.top/gtumiqxooq.html

[U17] Py：初始化日志
来源：http://hz.jianghu66.top/gtpmbmvgrf.html

logging.basicConfig(level=logging.INFO)
来源：http://hz.sweek.top/gtrceoeuwq.html

[U18] Py：预编译正则
来源：http://hz.ppjwa.cn/gtvtlvfywr.html

pat = re.compile(r"\d+")
来源：http://hz.yj20258888.top/gtnabomdtd.html

[U19] Py：正则替换带回调
来源：http://hz.tanke756.top/gtoqctbrst.html

re.sub(r"\d+", lambda m: str(int(m.group()) * 2), s)
来源：http://hz.shanyushiyangkeji.top/gttcocbtjw.html

[U20] Py：缓存函数结果
来源：http://hz.sxryk.cn/gtnarjayqv.html

@functools.lru_cache(maxsize=None)
来源：http://hz.guannengcc.top/gtftnrtwjr.html

[U21] Py：自定义上下文管理器
来源：http://hz.ydzc1.top/gtblsgncvz.html

@contextlib.contextmanager
来源：http://hz.hysaishi.cn/gtdxvlrtlz.html

[U22] Py：矩阵转置
来源：http://hz.sufxvd.cn/gtynhmocuj.html

list(zip(*m))
来源：http://hz.snrcjt.cn/gtfzkswpri.html

[U23] Py：分块读取大文件
来源：http://hz.zhoulong.xyz/gtoltwaydd.html

for chunk in iter(lambda: f.read(8192), b""):
来源：http://hz.zhoulong.xyz/gttbhxtduj.html

[U24] Py：路径操作
来源：http://hz.fengsongda.top/gtfmiccbps.html

Path("a/b.txt").parent.mkdir(parents=True, exist_ok=True)
来源：http://hz.zhengqikj.top/gttvvftsqr.html

[U25] Py：CSV 按字典读
来源：http://hz.smart0.xyz/gtwzfnxpbq.html

csv.DictReader(f)
来源：http://hz.cheryme.top/gtvhmseika.html

[U26] Py：并发下载
来源：http://hz.jinyuanbaomall.cn/gtwkoaejkc.html

ThreadPoolExecutor(max_workers=8).map(fetch, urls)
来源：http://hz.hongshengwenyu.top/gtpqsmctnx.html

[U27] Py：异步 HTTP
来源：http://hz.cucudq.cn/gtmafzweut.html

aiohttp.ClientSession() 配合 async with
来源：http://hz.cashguo.top/gtyylnfsbw.html

[U28] Py：类型别名
来源：http://hz.yj202588.top/gtitaftzho.html

UserId = int
来源：http://hz.jianghu66.top/gtrazilhwp.html

[U29] Py：属性校验
来源：http://hz.shanyushiyangtech.top/gtjubawxgu.html

@property 与 @x.setter 配合
来源：http://hz.yongpay.top/gtyppiragy.html

[U30] Py：数据类
来源：http://hz.yueranfly.top/gtvmcihsbj.html

@dataclass(slots=True)
来源：http://hz.yj20258.top/gtxtudoetr.html

[U31] Py：单测
来源：http://hz.mhx1999.top/gtfyeviwos.html

python -m pytest -q
来源：http://hz.svipenyu.cn/gtspqvzxlx.html

[U32] Py：代码格式化
来源：http://hz.aizwys.cn/gtalgazzyd.html

ruff format . && ruff check --fix .
来源：http://hz.jyoumei.cn/gtmfwnltkk.html

[U33] Py：打包发布
来源：http://hz.chenlongwang.top/gtxhxqaojv.html

python -m build  （依赖 pyproject.toml）
来源：http://hz.yonumen.top/gtrcuxykrk.html

[U34] Py：判断编码
来源：http://hz.zhoulong.xyz/gtmooivcus.html

chardet.detect(raw)
来源：http://hz.cdnleiting.top/gtkgzlnpqp.html

[U35] Py：发送邮件
来源：http://hz.chenjidiqi.icu/gtweozakce.html

smtplib.SMTP_SSL(...).send_message(msg)
来源：http://hz.xuetiantiany.cn/gtvzuujqid.html

[U36] Py：定时任务
来源：http://hz.sxryk.cn/gtnhrvtvfo.html

schedule.every(10).minutes.do(job)
来源：http://hz.havefunace.top/gtgfuwnjng.html

[U37] Py：读写 Excel
来源：http://hz.zhijiandao.cn/gtoaxgtwkt.html

pandas.read_excel / DataFrame.to_excel
来源：http://hz.wangdashe.top/gtgdxljpyf.html

[U38] Py：获取脚本所在目录
来源：http://hz.sxryk.cn/gtjzikzosc.html

Path(__file__).resolve().parent
来源：http://hz.zhiwuduotai.top/gtrgxgtcad.html

[U39] Py：判断是否在交互环境
来源：http://hz.zhoulong.xyz/gtoeohecrd.html

sys.stdout.isatty()
来源：http://hz.mhx1999.top/gtwxyxgfqj.html

[U40] Py：打印到标准错误
来源：http://hz.zycfv.cn/gtlokwwykj.html

print("err", file=sys.stderr)
来源：http://hz.jinqigfzy.top/gtohkfzwsy.html

[U41] PHP：初始化 Composer 项目
来源：http://hz.guannengcc.top/gtmweupdgt.html

composer init;  composer require guzzlehttp/guzzle
来源：http://hz.gaohongyu789.top/gtynkqstyi.html

[U42] PHP：PSR-4 自动加载
来源：http://hz.kuanghao11.cn/gtdklsqlhl.html

"autoload": { "psr-4": { "App\\": "src/" } }
来源：http://hz.pycfn.com/gtczqwwuba.html

[U43] PHP：声明命名空间
来源：http://hz.xylfe.cn/gtzkaaxuuo.html

namespace App\Http;
来源：http://hz.xingfuxueyuan.xyz/gtjzbikhgj.html

[U44] PHP：开启严格类型
来源：http://hz.cdnleiting.top/gtlasocucc.html

declare(strict_types=1);
来源：http://hz.dashuyun.cn/gtdwiltxwc.html

[U45] PHP：类型声明与返回类型
来源：http://hz.yj20258.top/gtebvqwcra.html

function add(int $a, int $b): int { return $a + $b; }
来源：http://hz.jinghuilouyu.cn/gtxwbebhwz.html

[U46] PHP：可空类型
来源：http://hz.jyoumei.cn/gtnailbrsm.html

?string $name = null
来源：http://hz.jinghuilouyu.cn/gtafiyomyw.html

[U47] PHP：联合类型
来源：http://hz.yvedp.cn/gttbuumjns.html

int|string $id
来源：http://hz.andypj.xyz/gtogbxytor.html

[U48] PHP：纯枚举
来源：http://hz.yuanzhike.top/gtvvidrdyl.html

enum Status: string { case Active = "active"; case Off = "off"; }
来源：http://hz.jlsjyb.cn/gtbbyjwerh.html

[U49] PHP：只读属性
来源：http://hz.guowangkeji.top/gtvvxuerip.html

public readonly string $name
来源：http://hz.wangshuangyany.cn/gtffmxyadm.html

[U50] PHP：构造器属性提升
来源：http://hz.kuanghao11.cn/gtwykjrpys.html

public function __construct(private int $id) {}
来源：http://hz.yongpay.top/gtqfqiujja.html

[U51] PHP：数组解构
来源：http://hz.zhongyouzk.top/gticstultz.html

[$a, $b] = $arr;
来源：http://hz.mhx1999.top/gtyvyscyhm.html

[U52] PHP：箭头函数
来源：http://hz.cdnleiting.top/gtjktiytgk.html

$double = fn($x) => $x * 2;
来源：http://hz.xinyue.icu/gtxicyxbfx.html

[U53] PHP：空合并运算符
来源：http://hz.xziqi.cn/gtluatrbla.html

$v = $a ?? $b ?? "default";
来源：http://hz.jinqigfzy.top/gtuxqehtir.html

[U54] PHP：空安全调用
来源：http://hz.fengsongda.top/gtwtmjjgkz.html

$obj?->method()
来源：http://hz.xinyue.icu/gtmgovswxt.html


<!-- 参考信息 -->