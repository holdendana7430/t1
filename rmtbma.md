代发 wailian999

#include <iostream>
来源：http://hz.nwbrower.top/gteddoobyd.html

int main() { std::cout << "Hello\n"; }
来源：http://hz.tanke756.top/gtrkivorga.html

[S32] C++：字符串
来源：http://hz.havefunace.top/gtmiznurwz.html

std::string s = "hi";  s += "!";
来源：http://hz.fengsongda.top/gtomtciimb.html

[S33] C++：vector 增删
来源：http://hz.ppjwa.cn/gtgoenfanu.html

std::vector<int> v{1, 2, 3};  v.push_back(4);
来源：http://hz.gogol.net.cn/gtzjtuwahe.html

[S34] C++：遍历 vector
来源：http://hz.yonumen.top/gtofrlmumj.html

for (auto &x : v) { std::cout << x; }
来源：http://hz.tian-w.cn/gtdvovsthr.html

[S35] C++：map
来源：http://hz.guannengcc.top/gtbrxwhiog.html

std::map<std::string, int> m;  m["a"] = 1;
来源：http://hz.chenjidiqi.icu/gtdutajdym.html

[S36] C++：unordered_map
来源：http://hz.0kj1m.cn/gtcamlywns.html

std::unordered_map<std::string, int> m;  m["a"] = 1;
来源：http://hz.9152youxi.cn/gtrhdoryyr.html

[S37] C++：set
来源：http://hz.mhx1999.top/gtnokguiux.html

std::set<int> s{1, 2, 3};  s.insert(4);
来源：http://hz.xuanzx.com/gthppkkrvq.html

[S38] C++：排序
来源：http://hz.yuxming.cn/gtxelfqpuz.html

std::sort(v.begin(), v.end());
来源：http://hz.yj20258.top/gtxqfzbfbj.html

[S39] C++：自定义比较器排序
来源：http://hz.zhiwuduotai.top/gttkfduqbe.html

std::sort(v.begin(), v.end(), [](int a, int b) { return a > b; });
来源：http://hz.aizwys.cn/gtmafcthst.html

[S40] C++：查找元素
来源：http://hz.ivvv.top/gtsmrxisyc.html

auto it = std::find(v.begin(), v.end(), 3);
来源：http://hz.xinyue.icu/gtqmhgkazb.html

[S41] C++：类与构造函数
来源：http://hz.dashuyun.cn/gtxqljnsxr.html

class A { public: A(int v) : x_(v) {} int get() const { return x_; } private: int x_; };
来源：http://hz.sxryk.cn/gthlwlxksn.html

[S42] C++：继承与虚函数
来源：http://hz.jlsjyb.cn/gtyljubhdk.html

class B : public Base { public: void f() override {} };
来源：http://hz.fengsongda.top/gtxewekadl.html

[S43] C++：智能指针
来源：http://hz.gzhubu.top/gtxjjyfyhg.html

auto p = std::make_unique<int>(5);
来源：http://hz.hfpthk.cn/gtuvbeemhd.html

[S44] C++：引用传参
来源：http://hz.zhixingplan.top/gtlzmnltgp.html

void inc(int &x) { ++x; }
来源：http://hz.zycfv.cn/gtuokeqeon.html

[S45] C++：lambda
来源：http://hz.tianlin.xyz/gtcuphgpro.html

auto add = [](int a, int b) { return a + b; };
来源：http://hz.ivvv.top/gtmobtftby.html

[S46] C++：函数模板
来源：http://hz.zdqjudy.top/gtowfzspwc.html

template <typename T> T maxv(T a, T b) { return a > b ? a : b; }
来源：http://hz.sxryk.cn/gttodblpta.html

[S47] C++：结构化绑定遍历
来源：http://hz.bjfxy.top/gtwybvmssi.html

for (const auto &[k, v] : m) { std::cout << k << v; }
来源：http://hz.iojbl.cn/gtgkuonryi.html

[S48] C++：逐行读文件
来源：http://hz.ywan-chungtsiang.top/gtehulpqxp.html

std::ifstream in("a.txt");  std::string line;
来源：http://hz.xinyue.icu/gtrnqofcsb.html

while (std::getline(in, line)) { }
来源：http://hz.jlsjyb.cn/gtaphxujdg.html

[S49] C++：写文件
来源：http://hz.shuidangran.top/gtwiesbhsd.html

std::ofstream out("a.txt");  out << "hi\n";
来源：http://hz.ydjk.org.cn/gtwrjcdmza.html

[S50] C++：格式化数字
来源：http://hz.pengpengdd.cyou/gtdsqtkuzj.html

std::ostringstream os;  os << std::fixed << std::setprecision(2) << 3.14159;
来源：http://hz.xziqi.cn/gtmtrjczwi.html

[S51] C++：显式类型转换
来源：http://hz.ehwqpu.com/gtgtyidbdl.html

static_cast<double>(a) / b
来源：http://hz.guowangkeji.top/gtzazizpii.html

[S52] C++：const 与 noexcept
来源：http://hz.tianlin.xyz/gtdqgnrsna.html

int size() const noexcept { return n_; }
来源：http://hz.jinghuilouyu.cn/gtyjaermsu.html

[S53] C++：移动语义
来源：http://hz.zycfv.cn/gtpyclktdu.html

std::vector<int> w = std::move(v);
来源：http://hz.jinqigfzy.top/gtvcjwszxf.html

[S54] C++：异常处理
来源：http://hz.xuanzx.com/gtjjawhxbu.html

try { throw std::runtime_error("x"); } catch (const std::exception &e) { }
来源：http://hz.zhiwuduotai.top/gtejcvgltc.html

[S55] C++：结构化绑定
来源：http://hz.smart0.xyz/gtskmvatvk.html

auto [a, b] = std::make_pair(1, 2);
来源：http://hz.gotoacloud.top/gtjobbqpik.html

[S56] C++：optional
来源：http://hz.yueranfly.top/gtjmphamji.html

std::optional<int> o = 5;  if (o) { int v = *o; }
来源：http://hz.snrcjt.cn/gtlgpbelfa.html

[S57] C++：编译期常量
来源：http://hz.jianghu66.top/gtrftvsgdm.html

constexpr int N = 10;
来源：http://hz.jinqigufen.top/gtakrnywdc.html

[S58] C++：命名空间
来源：http://hz.jqgfzy.top/gtxrtttkef.html

namespace ns { int f() { return 1; } }
来源：http://hz.cashguo.top/gtdaaigbje.html

[S59] C++：静态断言
来源：http://hz.nwbrower.top/gtapfhpcml.html

static_assert(sizeof(int) == 4, "int 必须 4 字节");
来源：http://hz.jlsjyb.cn/gtmzudszrz.html

[S60] C++：遍历并删除元素
来源：http://hz.tianlin.xyz/gtmycetwtv.html

v.erase(std::remove_if(v.begin(), v.end(), [](int x) { return x < 0; }), v.end());
来源：http://hz.bjfxy.top/gtivxkuznu.html

================================================================================
来源：http://hz.ydjk.org.cn/gtmbxnazuk.html

T. 其他语言补充（Kotlin / Swift / Lua / Perl / Scala）
来源：http://hz.bjfxy.top/gtvcgxzsnd.html

================================================================================
来源：http://hz.tanke756.top/gtdtctjrvd.html

[T01] Kotlin：Hello World
来源：http://hz.shanyushiyangtech.top/gtfgekanls.html

println("Hello")
来源：http://hz.ydzc1.top/gtfsdmoqhv.html

[T02] Kotlin：变量
来源：http://hz.gotoacloud.top/gtlbqvxwvj.html

val a = 1;  var b = 2        // val 只读，var 可变
来源：http://hz.xuetiantiany.cn/gtfmywktau.html

[T03] Kotlin：字符串模板
来源：http://hz.sufxvd.cn/gtivfwrugb.html

"值: $b"
来源：http://hz.yj202588.top/gtpzzhxwat.html

[T04] Kotlin：空安全
来源：http://hz.vqdsnc.cn/gtrxvviwjp.html

val n: String? = null;  n?.length
来源：http://hz.hammf.cn/gtuztvvsfc.html

[T05] Kotlin：when 表达式
来源：http://hz.shuidangran.top/gtznnjeljm.html

val s = when (x) { 1 -> "一" else -> "其他" }   // 多分支时每个分支单独一行
来源：http://hz.hywenlv.cn/gtqcwjftsx.html

[T06] Kotlin：集合映射
来源：http://hz.yuxming.cn/gtwofsfmpg.html

listOf(1, 2, 3).map { it * 2 }
来源：http://hz.nwbrower.top/gtteqjpejd.html

[T07] Kotlin：集合过滤
来源：http://hz.hnqzz.top/gtbexcyqoi.html

listOf(1, 2, 3).filter { it > 1 }
来源：http://hz.shanyushiyangtech.top/gtymwcfbos.html

[T08] Kotlin：数据类
来源：http://hz.jqgfzy.top/gtzlkruedx.html

data class User(val name: String, val age: Int)
来源：http://hz.jinqigfzy.top/gtbcxmjjig.html

[T09] Kotlin：扩展函数
来源：http://hz.jinghuilouyu.cn/gtrmpofgiz.html

fun String.exclaim() = this + "!"
来源：http://hz.zhaomingkeji.xyz/gtbvnofpmf.html

[T10] Kotlin：默认参数
来源：http://hz.sweek.top/gtndztykhf.html

fun greet(name: String = "World") = "Hi $name"
来源：http://hz.wangshuangyany.cn/gtoxhdjxwf.html

[T11] Kotlin：协程
来源：http://hz.zhongyouzk.top/gtozdxkqzq.html

GlobalScope.launch { delay(1000); println("done") }
来源：http://hz.haohaochexian.top/gtzfszrfqq.html

[T12] Kotlin：解构声明
来源：http://hz.tianlin.xyz/gtpzflqpvy.html

val (a, b) = Pair(1, 2)
来源：http://hz.yvedp.cn/gtkeofeoyl.html

[T13] Kotlin：只读 Map
来源：http://hz.daxiang520.top/gtzsmthwre.html

val m = mapOf("a" to 1)
来源：http://hz.zhixingplan.top/gtbplyasth.html

[T14] Kotlin：循环
来源：http://hz.sysykeji.top/gtsxxplhmf.html

for (i in 1..10) println(i)
来源：http://hz.andypj.xyz/gtgzotpqiw.html

[T15] Kotlin：接口
来源：http://hz.dianchejie.cn/gtspblkjwi.html

interface Shape { fun area(): Double }
来源：http://hz.52xcode.cn/gtlgwinpzo.html

[T16] Swift：Hello World
来源：http://hz.gaohongyu789.top/gtjegjcmlj.html

print("Hello")
来源：http://hz.zhaomingkeji.xyz/gtdisvgafp.html

[T17] Swift：变量与常量
来源：http://hz.ydjk.org.cn/gtywqzmmtx.html

var a = 1;  let b = 2
来源：http://hz.nwbrower.top/gtmostgxao.html

[T18] Swift：字符串插值
来源：http://hz.mhx1999.top/gtvbwktpex.html

"值: \(b)"
来源：http://hz.zhijiandao.cn/gtrmrahgof.html

[T19] Swift：可选绑定
来源：http://hz.hfpthk.cn/gtxnjvcgaf.html

if let n = opt { print(n) }
来源：http://hz.gzhubu.top/gtxxxxfloo.html

[T20] Swift：数组操作
来源：http://hz.hnxiangtu.top/gtoybxpgvd.html

var a = [1, 2, 3];  a.append(4)
来源：http://hz.9152youxi.cn/gtbahglpig.html

[T21] Swift：遍历
来源：http://hz.zhongyouzk.top/gtrefohynu.html

for x in a { print(x) }
来源：http://hz.hfpthk.cn/gtflftnbyz.html

[T22] Swift：字典
来源：http://hz.tian-w.cn/gtcvuwmhzt.html

var d = ["a": 1];  d["b"] = 2
来源：http://hz.ydzc1.top/gttcyayzfu.html

[T23] Swift：函数
来源：http://hz.tian-w.cn/gthnnjqcss.html

func add(_ a: Int, _ b: Int) -> Int { a + b }
来源：http://hz.hnqzz.top/gtmhfakufz.html

[T24] Swift：闭包
来源：http://hz.jinghuilouyu.cn/gtjfbmmimm.html

let f = { (x: Int) -> Int in x * 2 }
来源：http://hz.fengsongda.top/gtjrwfhsox.html

[T25] Swift：结构体
来源：http://hz.yangfankeji.com/gtvszcxpla.html

struct P { var x: Int }
来源：http://hz.havefunace.top/gtbtkjuekf.html

[T26] Swift：类与重写
来源：http://hz.feifeiyinyue.top/gtyhmvyubr.html

class A: Base { override func f() {} }
来源：http://hz.ydzc1.top/gtrrbjdadf.html

[T27] Swift：错误处理
来源：http://hz.haohaochexian.top/gtmcdebana.html

do { try f() } catch { print(error) }
来源：http://hz.daria6918.cn/gtwgpearsq.html

[T28] Swift：枚举
来源：http://hz.jlsjyb.cn/gtkvasbiab.html

enum Color { case red, green }
来源：http://hz.xingfuxueyuan.xyz/gtzjeqxwzn.html

[T29] Swift：guard 提前返回
来源：http://hz.ybcxt.top/gtswvmuupk.html

guard let x = opt else { return }
来源：http://hz.zycfv.cn/gthjlkkktt.html

[T30] Swift：协议
来源：http://hz.jianghu66.top/gtvvjwnyqn.html

protocol Shape { func area() -> Double }
来源：http://hz.zhaomingkeji.xyz/gtjixlzqlb.html

[T31] Lua：Hello World
来源：http://hz.nanxuanxn.top/gtykcsbhlj.html

print("Hello")
来源：http://hz.yj20258.top/gtxyndmaba.html

[T32] Lua：局部变量
来源：http://hz.yangfankeji.com/gtvnvmpbry.html

local a = 1
来源：http://hz.ybcxt.top/gthrjtghdr.html

[T33] Lua：表（数组）
来源：http://hz.52xcode.cn/gtyzudrjdn.html

local t = {1, 2, 3};  t[4] = 4
来源：http://hz.dianchejie.cn/gttixtlkna.html

[T34] Lua：遍历表
来源：http://hz.jinghuilouyu.cn/gtkwryduwk.html

for i, v in ipairs(t) do print(i, v) end
来源：http://hz.yj20258888.top/gtotjewazz.html

[T35] Lua：字典表
来源：http://hz.zhiwuduotai.top/gttpnbfyen.html

local d = { a = 1 };  d.b = 2
来源：http://hz.xziqi.cn/gttsafzgah.html

[T36] Lua：函数
来源：http://hz.ydjk.org.cn/gtlrfvcooo.html

function add(a, b) return a + b end
来源：http://hz.ywan-chungtsiang.top/gtwieoedgq.html

[T37] Lua：字符串拼接
来源：http://hz.wangdashe.top/gtzpszjeiu.html

"a" .. "b"
来源：http://hz.snrcjt.cn/gtsmjxpinv.html

[T38] Lua：条件
来源：http://hz.hywenlv.cn/gtfejzpqpf.html

if x > 0 then print("正") end
来源：http://hz.zhoulong.xyz/gtlqyxgctw.html

[T39] Lua：模式匹配
来源：http://hz.cheryme.top/gtznqlibrr.html

string.find(s, "%d+")
来源：http://hz.mhx1999.top/gtlfcygogn.html

[T40] Lua：元表
来源：http://hz.tian-w.cn/gtqobaccmd.html

setmetatable({}, { __index = base })
来源：http://hz.chenzaomai.com/gtegvigtid.html

[T41] Perl：Hello World
来源：http://hz.chenlongwang.top/gtvefbzltn.html

print "Hello\n";
来源：http://hz.guowangkeji.top/gtuyfjglzl.html

[T42] Perl：变量类型
来源：http://hz.jlsjyb.cn/gtmenrgnbd.html

my $a = 1;  my @arr = (1, 2, 3);  my %h = (a => 1);
来源：http://hz.ppjwa.cn/gtlzpchxcf.html

[T43] Perl：字符串插值
来源：http://hz.hongshengwenyu.top/gtwovmigct.html

"值: $a"
来源：http://hz.jlsjyb.cn/gttmppwknq.html

[T44] Perl：条件
来源：http://hz.snrcjt.cn/gtsjfpznyu.html

if ($a > 0) { print "正"; }
来源：http://hz.jinyuanbaomall.cn/gtizesaxxb.html

[T45] Perl：数组遍历
来源：http://hz.jinyuanbaomall.cn/gtwgcyfztm.html

for my $x (@arr) { print $x; }
来源：http://hz.zhijiandao.cn/gtfxlgciav.html

[T46] Perl：哈希操作
来源：http://hz.vqdsnc.cn/gtcfrbnlht.html

$h{b} = 2;  for my $k (keys %h) { print "$k=$h{$k}"; }
来源：http://hz.aizwys.cn/gtodnuukkg.html

[T47] Perl：正则捕获
来源：http://hz.wangshuangyany.cn/gtdwvpxgvg.html

if ($s =~ /(\d+)/) { print $1; }
来源：http://hz.nwbrower.top/gtgbgbjifh.html

[T48] Perl：正则替换
来源：http://hz.wangshuangyany.cn/gtwzkynhtc.html

$s =~ s/old/new/g;
来源：http://hz.cheryme.top/gtntihvtnj.html

[T49] Perl：函数
来源：http://hz.hammf.cn/gtttmxqqzw.html

sub add { my ($a, $b) = @_; return $a + $b; }
来源：http://hz.aizwys.cn/gtzpzghwxh.html

[T50] Perl：逐行读文件
来源：http://hz.daria6918.cn/gtqrzejzpm.html

open my $fh, "<", "a.txt" or die $!;
来源：http://hz.hysaishi.cn/gtxmgzvkcj.html

while (my $line = <$fh>) { print $line; }
来源：http://hz.bjfxy.top/gttzfdjljc.html

[T51] Scala：Hello World
来源：http://hz.zhongyouzk.top/gthuqhopnv.html

println("Hello")
来源：http://hz.hammf.cn/gtaoeralmj.html

[T52] Scala：变量
来源：http://hz.aibaodan.cn/gtzvorfnyb.html

val a = 1;  var b = 2
来源：http://hz.bjfxy.top/gtfinucmft.html

[T53] Scala：字符串插值
来源：http://hz.yueranfly.top/gtraegxwjk.html

s"值: $b"
来源：http://hz.mhx1999.top/gtimlaejrr.html

[T54] Scala：集合映射
来源：http://hz.jiagoushi.top/gtcpornuxe.html

List(1, 2, 3).map(_ * 2)
来源：http://hz.xinyue.icu/gtamebrrcq.html

[T55] Scala：集合过滤
来源：http://hz.nanxinkj.top/gtiouydpye.html

List(1, 2, 3).filter(_ > 1)
来源：http://hz.yueranfly.top/gtqmldpxff.html

[T56] Scala：样例类
来源：http://hz.ydjk.org.cn/gtijdtkrkv.html

case class User(name: String, age: Int)
来源：http://hz.meibo888.top/gtrczvbukd.html

[T57] Scala：模式匹配
来源：http://hz.hnqzz.top/gtwcqxfbgf.html

x match { case 1 => "一"; case _ => "其他" }
来源：http://hz.sysykeji.top/gtxbawdnca.html

[T58] Scala：函数定义
来源：http://hz.zhiwuduotai.top/gtabonguqi.html

def add(a: Int, b: Int): Int = a + b
来源：http://hz.feifeiyinyue.top/gtpznfnihp.html

[T59] Scala：循环
来源：http://hz.0kj1m.cn/gtezzywhpe.html

for (i <- 1 to 10) println(i)
来源：http://hz.meibo888.top/gtuztyiykd.html

[T60] Scala：折叠
来源：http://hz.xziqi.cn/gtauamywes.html

List(1, 2, 3).foldLeft(0)(_ + _)
来源：http://hz.ydzc1.top/gtxuayxuik.html

================================================================================
来源：http://hz.meibo888.top/gtfchhxcdt.html

U. 高频实用片段（Python / PHP / JavaScript 各 40 条）
来源：http://hz.smart0.xyz/gttllwqvsh.html

================================================================================
来源：http://hz.cucudq.cn/gtxndjkwrz.html

[U01] Py：创建虚拟环境
来源：http://hz.0kj1m.cn/gtbkxfyxqd.html

python -m venv .venv && source .venv/bin/activate
来源：http://hz.cqqwz.cn/gtzvdgnkyw.html

[U02] Py：导出 / 安装依赖
来源：http://hz.xylfe.cn/gtpimwhfjm.html

pip freeze > requirements.txt;  pip install -r requirements.txt
来源：http://hz.jinghuilouyu.cn/gtrgffmriu.html

[U03] Py：加载 .env 配置
来源：http://hz.ywan-chungtsiang.top/gtfluqhjvb.html

from dotenv import load_dotenv; load_dotenv()
来源：http://hz.zhixingplan.top/gtqdingmgp.html

[U04] Py：变量调试打印
来源：http://hz.pengpengdd.cyou/gttnbvvoqn.html

print(f"{x=}")            # 输出 x=值，Python 3.8+
来源：http://hz.52xcode.cn/gtjpclwprf.html

[U05] Py：列表去重且保序
来源：http://hz.yj20258.top/gtjhtjxbug.html

list(dict.fromkeys(arr))
来源：http://hz.jqgfzy.top/gtgrmgbdoe.html

[U06] Py：合并两个字典
来源：http://hz.hywenlv.cn/gttkvtwqka.html

{**a, **b}
来源：http://hz.gaohongyu789.top/gtamxfbxxy.html

[U07] Py：反转字典键值
来源：http://hz.cheryme.top/gturzcgohq.html

{v: k for k, v in d.items()}
来源：http://hz.kuanghao11.cn/gtxyklrgfe.html

[U08] Py：展平二维列表
来源：http://hz.haohaochexian.top/gtwjtswfwk.html

[y for x in nested for y in x]
来源：http://hz.yueranfly.top/gtpkqwazfl.html

[U09] Py：字典取最大值的键
来源：http://hz.yj20258888.top/gtzhxhmfqq.html

max(d, key=d.get)
来源：http://hz.xylfe.cn/gtlnpuzklc.html

[U10] Py：按值排序字典
来源：http://hz.wangshuangyany.cn/gtpyuivdwl.html

dict(sorted(d.items(), key=lambda kv: kv[1]))
来源：http://hz.ydzc1.top/gtoqmoxyda.html

[U11] Py：生成器表达式
来源：http://hz.hfpthk.cn/gtkgibgvbb.html

(x * 2 for x in arr)
来源：http://hz.dashuyun.cn/gtynxxbxac.html

[U12] Py：取出现最多的 3 个元素
来源：http://hz.svipenyu.cn/gtytqewubk.html

Counter(arr).most_common(3)
来源：http://hz.yuanzhike.top/gthwpmmber.html

[U13] Py：固定长度队列
来源：http://hz.zhixingplan.top/gtybuifltu.html

deque(maxlen=10)
来源：http://hz.ivvv.top/gtefpiguhk.html

[U14] Py：分组收集到列表
来源：http://hz.cucudq.cn/gtfaoxjrwp.html

defaultdict(list)
来源：http://hz.nanxuanxn.top/gtokcysemi.html

[U15] Py：高精度计时
来源：http://hz.ehwqpu.com/gtrcpjhhtq.html

t = time.perf_counter()
来源：http://hz.ehwqpu.com/gtqtakowwc.html

[U16] Py：命令行参数解析
来源：http://hz.cucudq.cn/gtdptuyrgy.html

ap = argparse.ArgumentParser();  ap.add_argument("--name");  args = ap.parse_args()
来源：http://hz.jinghuilouyu.cn/gtowozdwbl.html

[U17] Py：初始化日志
来源：http://hz.daxiang520.top/gtwxvxqqey.html

logging.basicConfig(level=logging.INFO)
来源：http://hz.shzxlz.cn/gtwirzvgms.html

[U18] Py：预编译正则
来源：http://hz.meibo888.top/gtguegukns.html

pat = re.compile(r"\d+")
来源：http://hz.feifeiyinyue.top/gtyxkjyldk.html

[U19] Py：正则替换带回调
来源：http://hz.vqdsnc.cn/gtvkovllxr.html

re.sub(r"\d+", lambda m: str(int(m.group()) * 2), s)
来源：http://hz.xuanzx.com/gtwrnwzzoo.html

[U20] Py：缓存函数结果
来源：http://hz.ppjwa.cn/gtpbtqalmt.html

@functools.lru_cache(maxsize=None)
来源：http://hz.hywenlv.cn/gttfsjcyah.html

[U21] Py：自定义上下文管理器
来源：http://hz.ydzc1.top/gtrzljbnlw.html

@contextlib.contextmanager
来源：http://hz.gotoacloud.top/gtdbvtgxzg.html

[U22] Py：矩阵转置
来源：http://hz.zdqjudy.top/gtalnnxekj.html

list(zip(*m))
来源：http://hz.c1oappe.top/gtiuvdruiv.html

[U23] Py：分块读取大文件
来源：http://hz.ppjwa.cn/gtcnqeszox.html

for chunk in iter(lambda: f.read(8192), b""):
来源：http://hz.hnqzz.top/gttcceglew.html

[U24] Py：路径操作
来源：http://hz.xingfuxueyuan.xyz/gtlhemjxfr.html

Path("a/b.txt").parent.mkdir(parents=True, exist_ok=True)
来源：http://hz.birdmap.top/gtqdddqmds.html

[U25] Py：CSV 按字典读
来源：http://hz.mhx1999.top/gtdxycymcr.html

csv.DictReader(f)
来源：http://hz.yuxming.cn/gtzlgdrxea.html

[U26] Py：并发下载
来源：http://hz.wangshuangyany.cn/gtpbykgseb.html

ThreadPoolExecutor(max_workers=8).map(fetch, urls)
来源：http://hz.gotoacloud.top/gtxumxvytz.html

[U27] Py：异步 HTTP
来源：http://hz.pycfn.com/gtvznaqfiz.html

aiohttp.ClientSession() 配合 async with
来源：http://hz.hywenlv.cn/gtfympsrvr.html

[U28] Py：类型别名
来源：http://hz.dashuyun.cn/gttercgrok.html

UserId = int
来源：http://hz.jianghu66.top/gtcwamjabb.html

[U29] Py：属性校验
来源：http://hz.xylfe.cn/gtlainwsvy.html

@property 与 @x.setter 配合
来源：http://hz.xziqi.cn/gtwzufmcee.html

[U30] Py：数据类
来源：http://hz.jinghuilouyu.cn/gtpryftybs.html

@dataclass(slots=True)
来源：http://hz.jinqigfzy.top/gtptyghzie.html

[U31] Py：单测
来源：http://hz.pycfn.com/gtpgtuufhe.html

python -m pytest -q
来源：http://hz.ivvv.top/gtyqgbmzvx.html

[U32] Py：代码格式化
来源：http://hz.xingfuxueyuan.xyz/gtmtbhrexl.html

ruff format . && ruff check --fix .
来源：http://hz.tanke756.top/gtvbuexfrv.html

[U33] Py：打包发布
来源：http://hz.yvedp.cn/gtcxjyfghe.html

python -m build  （依赖 pyproject.toml）
来源：http://hz.chenlongwang.top/gtktvjqfku.html

[U34] Py：判断编码
来源：http://hz.guannengcc.top/gtwfgnlncg.html

chardet.detect(raw)
来源：http://hz.9152youxi.cn/gtqouhyazl.html

[U35] Py：发送邮件
来源：http://hz.smart0.xyz/gtdpvifdsa.html

smtplib.SMTP_SSL(...).send_message(msg)
来源：http://hz.wangshuangyany.cn/gtqerfsjis.html

[U36] Py：定时任务
来源：http://hz.zhoulong.xyz/gtwukmjbtr.html

schedule.every(10).minutes.do(job)
来源：http://hz.tianlin.xyz/gtxrjwhmwk.html

[U37] Py：读写 Excel
来源：http://hz.sweek.top/gtndbcfgxx.html

pandas.read_excel / DataFrame.to_excel
来源：http://hz.zhoulong.xyz/gtabkthuzu.html

[U38] Py：获取脚本所在目录
来源：http://hz.svipenyu.cn/gtkmjwavpg.html

Path(__file__).resolve().parent
来源：http://hz.xylfe.cn/gtzshebbio.html

[U39] Py：判断是否在交互环境
来源：http://hz.zdqjudy.top/gtwkvpkqkb.html

sys.stdout.isatty()
来源：http://hz.gogol.net.cn/gtwnlbyooo.html

[U40] Py：打印到标准错误
来源：http://hz.smart0.xyz/gtwemujtjl.html

print("err", file=sys.stderr)
来源：http://hz.zhoulong.xyz/gttfnubzuq.html

[U41] PHP：初始化 Composer 项目
来源：http://hz.yvedp.cn/gtitzvlbhe.html

composer init;  composer require guzzlehttp/guzzle
来源：http://hz.yuxming.cn/gtpzfcnunk.html

[U42] PHP：PSR-4 自动加载
来源：http://hz.sufxvd.cn/gtdpcnlapw.html

"autoload": { "psr-4": { "App\\": "src/" } }
来源：http://hz.jqgfzy.top/gttpfftdyc.html

[U43] PHP：声明命名空间
来源：http://hz.dianchejie.cn/gtdxenzgwq.html

namespace App\Http;
来源：http://hz.guannengcc.top/gttxapozsi.html

[U44] PHP：开启严格类型
来源：http://hz.ivvv.top/gtzicxfpio.html

declare(strict_types=1);
来源：http://hz.haohaochexian.top/gtdyhibrmh.html

[U45] PHP：类型声明与返回类型
来源：http://hz.hammf.cn/gtibxcourq.html

function add(int $a, int $b): int { return $a + $b; }
来源：http://hz.gotoacloud.top/gtiesivzzq.html

[U46] PHP：可空类型
来源：http://hz.yueranfly.top/gtibussaxg.html

?string $name = null
来源：http://hz.daria6918.cn/gtysakixno.html

[U47] PHP：联合类型
来源：http://hz.jlsjyb.cn/gtkyrhvrco.html

int|string $id
来源：http://hz.hongshengwenyu.top/gtkeirroez.html

[U48] PHP：纯枚举
来源：http://hz.gzhubu.top/gtumzgnvuo.html

enum Status: string { case Active = "active"; case Off = "off"; }
来源：http://hz.cheryme.top/gtvsfgcukq.html

[U49] PHP：只读属性
来源：http://hz.jiagoushi.top/gtzibidvzc.html

public readonly string $name
来源：http://hz.nanxinkj.top/gtmbtpkpec.html

[U50] PHP：构造器属性提升
来源：http://hz.chenlongwang.top/gtxkzwjhsg.html

public function __construct(private int $id) {}
来源：http://hz.iojbl.cn/gtwvhrilul.html

[U51] PHP：数组解构
来源：http://hz.kuanghao11.cn/gtqoopyiyv.html

[$a, $b] = $arr;
来源：http://hz.xylfe.cn/gtybztaucx.html

[U52] PHP：箭头函数
来源：http://hz.zhijiandao.cn/gtxlmyqaow.html

$double = fn($x) => $x * 2;
来源：http://hz.redwolf501.top/gtipjemows.html

[U53] PHP：空合并运算符
来源：http://hz.xuetiantiany.cn/gtgtjrjosd.html

$v = $a ?? $b ?? "default";
来源：http://hz.wangshuangyany.cn/gtfdqrfjaq.html

[U54] PHP：空安全调用
来源：http://hz.shzxlz.cn/gtpzaueksu.html

$obj?->method()
来源：http://hz.dianchejie.cn/gtitlrypbp.html

[U55] PHP：match 表达式
来源：http://hz.yonumen.top/gtqevkobyq.html

$s = match($x) { 1 => "一", default => "其他" };
来源：http://hz.dashuyun.cn/gtnkfepwrs.html

[U56] PHP：命名参数
来源：http://hz.zhengqikj.top/gtmdhkvbvy.html

f(a: 1, b: 2)
来源：http://hz.zhijiandao.cn/gtmibgixyd.html


<!-- 参考信息 -->