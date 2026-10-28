代发 wailian999

#ifndef X_H
来源：http://hz.cheryme.top/gtktpeyvpg.html

#define X_H
来源：http://hz.jinghuilouyu.cn/gtqdodxpub.html

#endif
来源：http://hz.shanyushiyangtech.top/gtfflkfznn.html

[S31] C++：Hello World
来源：http://hz.cdnleiting.top/gtvziryrfd.html

#include <iostream>
来源：http://hz.fengsongda.top/gtacyodynk.html

int main() { std::cout << "Hello\n"; }
来源：http://hz.dashuyun.cn/gthzspmchs.html

[S32] C++：字符串
来源：http://hz.jianghu66.top/gtwmubzkue.html

std::string s = "hi";  s += "!";
来源：http://hz.zhaomingkeji.xyz/gtrfydmadf.html

[S33] C++：vector 增删
来源：http://hz.zhengqikj.top/gtjwjvsyns.html

std::vector<int> v{1, 2, 3};  v.push_back(4);
来源：http://hz.shanyushiyangkeji.top/gtgydxxqym.html

[S34] C++：遍历 vector
来源：http://hz.shanyushiyangtech.top/gthochfrwm.html

for (auto &x : v) { std::cout << x; }
来源：http://hz.zhoulong.xyz/gtahiojozl.html

[S35] C++：map
来源：http://hz.yuanzhike.top/gtmarahhvk.html

std::map<std::string, int> m;  m["a"] = 1;
来源：http://hz.cashguo.top/gtlnffecle.html

[S36] C++：unordered_map
来源：http://hz.kuanghao11.cn/gtgabcuerw.html

std::unordered_map<std::string, int> m;  m["a"] = 1;
来源：http://hz.hnxiangtu.top/gtnjwdfwfp.html

[S37] C++：set
来源：http://hz.yanxiufei.cn/gtxoakhbda.html

std::set<int> s{1, 2, 3};  s.insert(4);
来源：http://hz.fengsongda.top/gtkagzwyfu.html

[S38] C++：排序
来源：http://hz.sxryk.cn/gtdchiimjv.html

std::sort(v.begin(), v.end());
来源：http://hz.xingfuxueyuan.xyz/gtmazdvdbi.html

[S39] C++：自定义比较器排序
来源：http://hz.cdnleiting.top/gtnjmejqqg.html

std::sort(v.begin(), v.end(), [](int a, int b) { return a > b; });
来源：http://hz.yueranfly.top/gthpyvcrxo.html

[S40] C++：查找元素
来源：http://hz.gaohongyu789.top/gtdxipzspx.html

auto it = std::find(v.begin(), v.end(), 3);
来源：http://hz.gogol.net.cn/gtkdpqaaxj.html

[S41] C++：类与构造函数
来源：http://hz.cheryme.top/gtpslawenh.html

class A { public: A(int v) : x_(v) {} int get() const { return x_; } private: int x_; };
来源：http://hz.cqqwz.cn/gtppurmiae.html

[S42] C++：继承与虚函数
来源：http://hz.havefunace.top/gtmrpzmzxb.html

class B : public Base { public: void f() override {} };
来源：http://hz.yj20258.top/gtmbrphfzq.html

[S43] C++：智能指针
来源：http://hz.zhengqikj.top/gtahinkyus.html

auto p = std::make_unique<int>(5);
来源：http://hz.feifeiyinyue.top/gtarytpukc.html

[S44] C++：引用传参
来源：http://hz.yonumen.top/gtwpmelzhz.html

void inc(int &x) { ++x; }
来源：http://hz.316326.xyz/gtpdudhgvq.html

[S45] C++：lambda
来源：http://hz.ppjwa.cn/gtjqrtbgsx.html

auto add = [](int a, int b) { return a + b; };
来源：http://hz.zycfv.cn/gtkrpowghy.html

[S46] C++：函数模板
来源：http://hz.zhijiandao.cn/gtxvrhbkqu.html

template <typename T> T maxv(T a, T b) { return a > b ? a : b; }
来源：http://hz.kuanghao11.cn/gtssajuzqy.html

[S47] C++：结构化绑定遍历
来源：http://hz.sufxvd.cn/gtncqtjnce.html

for (const auto &[k, v] : m) { std::cout << k << v; }
来源：http://hz.smart0.xyz/gtbzkewwzn.html

[S48] C++：逐行读文件
来源：http://hz.kuanghao11.cn/gtximbwmdh.html

std::ifstream in("a.txt");  std::string line;
来源：http://hz.jqgfzy.top/gtcgazijyb.html

while (std::getline(in, line)) { }
来源：http://hz.ydzc1.top/gtgzyswzjh.html

[S49] C++：写文件
来源：http://hz.shangyingyoupin.top/gtekmizvep.html

std::ofstream out("a.txt");  out << "hi\n";
来源：http://hz.9152youxi.cn/gtoxeihjlp.html

[S50] C++：格式化数字
来源：http://hz.fengsongda.top/gtwuueoetq.html

std::ostringstream os;  os << std::fixed << std::setprecision(2) << 3.14159;
来源：http://hz.smart0.xyz/gtrtaxcndd.html

[S51] C++：显式类型转换
来源：http://hz.jinyuanbaomall.cn/gttqakawkw.html

static_cast<double>(a) / b
来源：http://hz.vqdsnc.cn/gtwfybbffa.html

[S52] C++：const 与 noexcept
来源：http://hz.cashguo.top/gtvgxcpzbc.html

int size() const noexcept { return n_; }
来源：http://hz.fengsongda.top/gtqnombrjs.html

[S53] C++：移动语义
来源：http://hz.zhengqikj.top/gtjlkvprcs.html

std::vector<int> w = std::move(v);
来源：http://hz.chenjidiqi.icu/gtnbszaxqq.html

[S54] C++：异常处理
来源：http://hz.pycfn.com/gtdbcaiusr.html

try { throw std::runtime_error("x"); } catch (const std::exception &e) { }
来源：http://hz.yuanzhike.top/gtovxfntny.html

[S55] C++：结构化绑定
来源：http://hz.aizwys.cn/gtiyspjnje.html

auto [a, b] = std::make_pair(1, 2);
来源：http://hz.vqdsnc.cn/gtfhabifis.html

[S56] C++：optional
来源：http://hz.zhiwuduotai.top/gtqlcvsbyc.html

std::optional<int> o = 5;  if (o) { int v = *o; }
来源：http://hz.tanke756.top/gtiszcjpzp.html

[S57] C++：编译期常量
来源：http://hz.ydjk.org.cn/gtnahnrcye.html

constexpr int N = 10;
来源：http://hz.cdnleiting.top/gtyqmjoejg.html

[S58] C++：命名空间
来源：http://hz.jinghuilouyu.cn/gtslfhfvol.html

namespace ns { int f() { return 1; } }
来源：http://hz.mhx1999.top/gtvhnjdgul.html

[S59] C++：静态断言
来源：http://hz.nwbrower.top/gtjulddccc.html

static_assert(sizeof(int) == 4, "int 必须 4 字节");
来源：http://hz.jqgfzy.top/gtqqgsuzoc.html

[S60] C++：遍历并删除元素
来源：http://hz.guowangkeji.top/gtfekelxai.html

v.erase(std::remove_if(v.begin(), v.end(), [](int x) { return x < 0; }), v.end());
来源：http://hz.xuetiantiany.cn/gtsvtvmhec.html

================================================================================
来源：http://hz.sufxvd.cn/gtckxcheby.html

T. 其他语言补充（Kotlin / Swift / Lua / Perl / Scala）
来源：http://hz.gaohongyu789.top/gtxzkbwrtf.html

================================================================================
来源：http://hz.yongpay.top/gtqijrjvhv.html

[T01] Kotlin：Hello World
来源：http://hz.xuanzx.com/gtzstuilns.html

println("Hello")
来源：http://hz.gogol.net.cn/gtuxdesdni.html

[T02] Kotlin：变量
来源：http://hz.svipenyu.cn/gtnilrrahf.html

val a = 1;  var b = 2        // val 只读，var 可变
来源：http://hz.ppjwa.cn/gtcgdmhjzx.html

[T03] Kotlin：字符串模板
来源：http://hz.nanxuanxn.top/gtttrqygxe.html

"值: $b"
来源：http://hz.feifeiyinyue.top/gthhvxabfi.html

[T04] Kotlin：空安全
来源：http://hz.ybcxt.top/gtqjtraojx.html

val n: String? = null;  n?.length
来源：http://hz.ehwqpu.com/gtajylszsi.html

[T05] Kotlin：when 表达式
来源：http://hz.ydzc1.top/gtfndmkmbc.html

val s = when (x) { 1 -> "一" else -> "其他" }   // 多分支时每个分支单独一行
来源：http://hz.cashguo.top/gtxwddqodn.html

[T06] Kotlin：集合映射
来源：http://hz.ppjwa.cn/gttiivngls.html

listOf(1, 2, 3).map { it * 2 }
来源：http://hz.jlsjyb.cn/gtooriqggv.html

[T07] Kotlin：集合过滤
来源：http://hz.havefunace.top/gtcykeinlo.html

listOf(1, 2, 3).filter { it > 1 }
来源：http://hz.gzhubu.top/gtziqhzotq.html

[T08] Kotlin：数据类
来源：http://hz.xuetiantiany.cn/gtazpoljjr.html

data class User(val name: String, val age: Int)
来源：http://hz.cheryme.top/gtvzndqvcc.html

[T09] Kotlin：扩展函数
来源：http://hz.svipenyu.cn/gtrwriwtvg.html

fun String.exclaim() = this + "!"
来源：http://hz.jianghu66.top/gtblpwafjp.html

[T10] Kotlin：默认参数
来源：http://hz.gzhubu.top/gtfmionwva.html

fun greet(name: String = "World") = "Hi $name"
来源：http://hz.hysaishi.cn/gtxyoemmxz.html

[T11] Kotlin：协程
来源：http://hz.iojbl.cn/gtbewinvrr.html

GlobalScope.launch { delay(1000); println("done") }
来源：http://hz.tianlin.xyz/gttymnblwf.html

[T12] Kotlin：解构声明
来源：http://hz.wangdashe.top/gttfpkjuid.html

val (a, b) = Pair(1, 2)
来源：http://hz.nwbrower.top/gtitsddhlt.html

[T13] Kotlin：只读 Map
来源：http://hz.haohaochexian.top/gtxdwhfikc.html

val m = mapOf("a" to 1)
来源：http://hz.cqqwz.cn/gtucomgods.html

[T14] Kotlin：循环
来源：http://hz.jinqigufen.top/gtbjynychu.html

for (i in 1..10) println(i)
来源：http://hz.316326.xyz/gtxnboqehe.html

[T15] Kotlin：接口
来源：http://hz.yuxming.cn/gtgzdxdzpm.html

interface Shape { fun area(): Double }
来源：http://hz.ppjwa.cn/gtbfwfgkbb.html

[T16] Swift：Hello World
来源：http://hz.ywan-chungtsiang.top/gtcjkhoijh.html

print("Hello")
来源：http://hz.yj202588.top/gtcewetwjr.html

[T17] Swift：变量与常量
来源：http://hz.wangshuangyany.cn/gtcldysmsd.html

var a = 1;  let b = 2
来源：http://hz.aibaodan.cn/gtxqakolvr.html

[T18] Swift：字符串插值
来源：http://hz.gotoacloud.top/gtypseafgr.html

"值: \(b)"
来源：http://hz.tianlin.xyz/gtmxllhiau.html

[T19] Swift：可选绑定
来源：http://hz.52xcode.cn/gtglodwbeg.html

if let n = opt { print(n) }
来源：http://hz.snrcjt.cn/gtafrcwqwp.html

[T20] Swift：数组操作
来源：http://hz.shzxlz.cn/gtmayzrqsc.html

var a = [1, 2, 3];  a.append(4)
来源：http://hz.zhijiandao.cn/gtjjraottl.html

[T21] Swift：遍历
来源：http://hz.zycfv.cn/gtzhhnnuqc.html

for x in a { print(x) }
来源：http://hz.shzxlz.cn/gtwzvejncv.html

[T22] Swift：字典
来源：http://hz.shuidangran.top/gtqdivygpi.html

var d = ["a": 1];  d["b"] = 2
来源：http://hz.jyoumei.cn/gtawealjwe.html

[T23] Swift：函数
来源：http://hz.nanxuanxn.top/gtbqmanpcl.html

func add(_ a: Int, _ b: Int) -> Int { a + b }
来源：http://hz.wangdashe.top/gtsiiqoepc.html

[T24] Swift：闭包
来源：http://hz.quarkkingdee.top/gttjolgztj.html

let f = { (x: Int) -> Int in x * 2 }
来源：http://hz.jinghuilouyu.cn/gtdubsgvse.html

[T25] Swift：结构体
来源：http://hz.gzhubu.top/gtyleljozy.html

struct P { var x: Int }
来源：http://hz.0kj1m.cn/gtewjlfwvh.html

[T26] Swift：类与重写
来源：http://hz.cdnleiting.top/gtqkvbufbd.html

class A: Base { override func f() {} }
来源：http://hz.iojbl.cn/gthqnlxkrt.html

[T27] Swift：错误处理
来源：http://hz.zhijiandao.cn/gtpofujdoy.html

do { try f() } catch { print(error) }
来源：http://hz.aizwys.cn/gtckegcsgl.html

[T28] Swift：枚举
来源：http://hz.shuidangran.top/gtscibqdzz.html

enum Color { case red, green }
来源：http://hz.yuxming.cn/gtlztkejot.html

[T29] Swift：guard 提前返回
来源：http://hz.ppjwa.cn/gtznnsnusd.html

guard let x = opt else { return }
来源：http://hz.shuidangran.top/gtsvlyruwr.html

[T30] Swift：协议
来源：http://hz.hongshengwenyu.top/gtttzgivbv.html

protocol Shape { func area() -> Double }
来源：http://hz.tanke756.top/gtjneuekpe.html

[T31] Lua：Hello World
来源：http://hz.ydzc1.top/gtminhvtiv.html

print("Hello")
来源：http://hz.bjfxy.top/gthjkjmjsw.html

[T32] Lua：局部变量
来源：http://hz.daria6918.cn/gtqjwueddv.html

local a = 1
来源：http://hz.zycfv.cn/gtlctnpchh.html

[T33] Lua：表（数组）
来源：http://hz.shangyingyoupin.top/gtfhnskfan.html

local t = {1, 2, 3};  t[4] = 4
来源：http://hz.birdmap.top/gtivqjifwz.html

[T34] Lua：遍历表
来源：http://hz.cashguo.top/gtqbnoqusu.html

for i, v in ipairs(t) do print(i, v) end
来源：http://hz.feifeiyinyue.top/gtlxolyxsz.html

[T35] Lua：字典表
来源：http://hz.wangdashe.top/gtewgjjzrf.html

local d = { a = 1 };  d.b = 2
来源：http://hz.shanyushiyangtech.top/gtytoylsgw.html

[T36] Lua：函数
来源：http://hz.pycfn.com/gtoijnsend.html

function add(a, b) return a + b end
来源：http://hz.jqgfzy.top/gtsvuzaflk.html

[T37] Lua：字符串拼接
来源：http://hz.jinghuilouyu.cn/gtolztpgpg.html

"a" .. "b"
来源：http://hz.sweek.top/gtgdnvzzun.html

[T38] Lua：条件
来源：http://hz.jqgufenzy.top/gtxvddmkrl.html

if x > 0 then print("正") end
来源：http://hz.zhoulong.xyz/gtpnjteuzf.html

[T39] Lua：模式匹配
来源：http://hz.smart0.xyz/gtuvqnxeao.html

string.find(s, "%d+")
来源：http://hz.yongpay.top/gtbvtoxsre.html

[T40] Lua：元表
来源：http://hz.pengpengdd.cyou/gtrjenvlil.html

setmetatable({}, { __index = base })
来源：http://hz.hnxiangtu.top/gtomorfgpc.html

[T41] Perl：Hello World
来源：http://hz.yj202588.top/gttptyxavp.html

print "Hello\n";
来源：http://hz.zhoulong.xyz/gtjivxboap.html

[T42] Perl：变量类型
来源：http://hz.ywan-chungtsiang.top/gtezxfrkef.html

my $a = 1;  my @arr = (1, 2, 3);  my %h = (a => 1);
来源：http://hz.cqqwz.cn/gthlhblwha.html

[T43] Perl：字符串插值
来源：http://hz.zhiwuduotai.top/gtfeaoahub.html

"值: $a"
来源：http://hz.xinyue.icu/gtmabzwvqf.html

[T44] Perl：条件
来源：http://hz.wangdashe.top/gtitoegzmw.html

if ($a > 0) { print "正"; }
来源：http://hz.birdmap.top/gtvqelhqun.html

[T45] Perl：数组遍历
来源：http://hz.vqdsnc.cn/gtndyuahnh.html

for my $x (@arr) { print $x; }
来源：http://hz.yuxming.cn/gtwlacfyuh.html

[T46] Perl：哈希操作
来源：http://hz.yj202588.top/gtlnixoeah.html

$h{b} = 2;  for my $k (keys %h) { print "$k=$h{$k}"; }
来源：http://hz.xziqi.cn/gtgliocecf.html

[T47] Perl：正则捕获
来源：http://hz.xziqi.cn/gtkgujzmme.html

if ($s =~ /(\d+)/) { print $1; }
来源：http://hz.fengsongda.top/gtniwtdhda.html

[T48] Perl：正则替换
来源：http://hz.vqdsnc.cn/gtrsaggkvq.html

$s =~ s/old/new/g;
来源：http://hz.mhx1999.top/gtcejdfqln.html

[T49] Perl：函数
来源：http://hz.feifeiyinyue.top/gtjvhsfrvw.html

sub add { my ($a, $b) = @_; return $a + $b; }
来源：http://hz.316326.xyz/gtkplneval.html

[T50] Perl：逐行读文件
来源：http://hz.chenzaomai.com/gtbkbekpwe.html

open my $fh, "<", "a.txt" or die $!;
来源：http://hz.yvedp.cn/gtpipmgspa.html

while (my $line = <$fh>) { print $line; }
来源：http://hz.tianlin.xyz/gtlmpdzqoe.html

[T51] Scala：Hello World
来源：http://hz.pycfn.com/gtfvrgkfmv.html

println("Hello")
来源：http://hz.daxiang520.top/gtrruimnjb.html

[T52] Scala：变量
来源：http://hz.yj20258888.top/gtwzkiryno.html

val a = 1;  var b = 2
来源：http://hz.svipenyu.cn/gtnuxlvdto.html

[T53] Scala：字符串插值
来源：http://hz.feifeiyinyue.top/gthevstaxe.html

s"值: $b"
来源：http://hz.quarkkingdee.top/gtypagacyi.html

[T54] Scala：集合映射
来源：http://hz.ydzc1.top/gterrzabtv.html

List(1, 2, 3).map(_ * 2)
来源：http://hz.9152youxi.cn/gtdenfbtaz.html

[T55] Scala：集合过滤
来源：http://hz.yj202588.top/gthyfseehg.html

List(1, 2, 3).filter(_ > 1)
来源：http://hz.svipenyu.cn/gtbgpspmfj.html

[T56] Scala：样例类
来源：http://hz.yanxiufei.cn/gtmxjnolxi.html

case class User(name: String, age: Int)
来源：http://hz.sweek.top/gtyinvwcka.html

[T57] Scala：模式匹配
来源：http://hz.c1oappe.top/gtwaqyswpe.html

x match { case 1 => "一"; case _ => "其他" }
来源：http://hz.chenjidiqi.icu/gtqcinrzsy.html

[T58] Scala：函数定义
来源：http://hz.meibo888.top/gtbyvdnqck.html

def add(a: Int, b: Int): Int = a + b
来源：http://hz.birdmap.top/gtucjkzkyc.html

[T59] Scala：循环
来源：http://hz.zycfv.cn/gtwnafsqzr.html

for (i <- 1 to 10) println(i)
来源：http://hz.fzhhl.top/gtpkwbsjqk.html

[T60] Scala：折叠
来源：http://hz.andypj.xyz/gtqbdvpisn.html

List(1, 2, 3).foldLeft(0)(_ + _)
来源：http://hz.redwolf501.top/gtvgivkppj.html

================================================================================
来源：http://hz.haohaochexian.top/gthyfmotfb.html

U. 高频实用片段（Python / PHP / JavaScript 各 40 条）
来源：http://hz.daxiang520.top/gtydzggfpn.html

================================================================================
来源：http://hz.andypj.xyz/gtcbfeyqjs.html

[U01] Py：创建虚拟环境
来源：http://hz.hfpthk.cn/gthdnhncly.html

python -m venv .venv && source .venv/bin/activate
来源：http://hz.jianghu66.top/gtjgkgiuer.html

[U02] Py：导出 / 安装依赖
来源：http://hz.daria6918.cn/gtgzsuktsx.html

pip freeze > requirements.txt;  pip install -r requirements.txt
来源：http://hz.yanxiufei.cn/gtdgliqgyc.html

[U03] Py：加载 .env 配置
来源：http://hz.sysykeji.top/gtcraawqwu.html

from dotenv import load_dotenv; load_dotenv()
来源：http://hz.nanxinkj.top/gtdymsaobj.html

[U04] Py：变量调试打印
来源：http://hz.cqqwz.cn/gteedwgtkt.html

print(f"{x=}")            # 输出 x=值，Python 3.8+
来源：http://hz.svipenyu.cn/gtkqbsczgl.html

[U05] Py：列表去重且保序
来源：http://hz.snrcjt.cn/gtmlospadm.html

list(dict.fromkeys(arr))
来源：http://hz.dashuyun.cn/gtqnvpqmhu.html

[U06] Py：合并两个字典
来源：http://hz.fzhhl.top/gtiihbblsd.html

{**a, **b}
来源：http://hz.bjfxy.top/gthgxbaurv.html

[U07] Py：反转字典键值
来源：http://hz.havefunace.top/gtropjmwas.html

{v: k for k, v in d.items()}
来源：http://hz.jianghu66.top/gtacvuagku.html

[U08] Py：展平二维列表
来源：http://hz.hfpthk.cn/gtylffqvvj.html

[y for x in nested for y in x]
来源：http://hz.sufxvd.cn/gttqferhjz.html

[U09] Py：字典取最大值的键
来源：http://hz.jinyuanbaomall.cn/gtrgqxyjbs.html

max(d, key=d.get)
来源：http://hz.zdqjudy.top/gtmagffnkn.html

[U10] Py：按值排序字典
来源：http://hz.tianlin.xyz/gtxyuswkpz.html

dict(sorted(d.items(), key=lambda kv: kv[1]))
来源：http://hz.cheryme.top/gtqvjfvudt.html

[U11] Py：生成器表达式
来源：http://hz.jinqigufen.top/gtmifwqfca.html

(x * 2 for x in arr)
来源：http://hz.shuidangran.top/gtdesrxmee.html

[U12] Py：取出现最多的 3 个元素
来源：http://hz.ywan-chungtsiang.top/gtndjbihig.html

Counter(arr).most_common(3)
来源：http://hz.sufxvd.cn/gtrvoamgsy.html

[U13] Py：固定长度队列
来源：http://hz.hysaishi.cn/gtftbyicro.html

deque(maxlen=10)
来源：http://hz.chenlongwang.top/gtnjvqpksn.html

[U14] Py：分组收集到列表
来源：http://hz.yj202588.top/gtivyrczwv.html

defaultdict(list)
来源：http://hz.ppjwa.cn/gtwjttwecc.html

[U15] Py：高精度计时
来源：http://hz.yvedp.cn/gtrghwgfte.html

t = time.perf_counter()
来源：http://hz.gzhubu.top/gtmknbfhsj.html

[U16] Py：命令行参数解析
来源：http://hz.xuetiantiany.cn/gticdnqoph.html

ap = argparse.ArgumentParser();  ap.add_argument("--name");  args = ap.parse_args()
来源：http://hz.yvedp.cn/gthvctlcel.html

[U17] Py：初始化日志
来源：http://hz.ivvv.top/gtbkxhwmar.html

logging.basicConfig(level=logging.INFO)
来源：http://hz.yuanzhike.top/gttrhhohhd.html

[U18] Py：预编译正则
来源：http://hz.shanyushiyangtech.top/gtzqtkpbri.html

pat = re.compile(r"\d+")
来源：http://hz.sysykeji.top/gtimnqnhbq.html

[U19] Py：正则替换带回调
来源：http://hz.aibaodan.cn/gtxsebovmr.html

re.sub(r"\d+", lambda m: str(int(m.group()) * 2), s)
来源：http://hz.gotoacloud.top/gtcwbirsof.html

[U20] Py：缓存函数结果
来源：http://hz.smart0.xyz/gtyjcuahos.html

@functools.lru_cache(maxsize=None)
来源：http://hz.shuidangran.top/gtyuikwlqc.html

[U21] Py：自定义上下文管理器
来源：http://hz.fengsongda.top/gtnotqvcse.html

@contextlib.contextmanager
来源：http://hz.ivvv.top/gtzzdpjppb.html

[U22] Py：矩阵转置
来源：http://hz.316326.xyz/gtxqgsovft.html

list(zip(*m))
来源：http://hz.hnxiangtu.top/gtezjgjtea.html

[U23] Py：分块读取大文件
来源：http://hz.xuetiantiany.cn/gtqnqeokzp.html

for chunk in iter(lambda: f.read(8192), b""):
来源：http://hz.birdmap.top/gttbrykkhv.html

[U24] Py：路径操作
来源：http://hz.pycfn.com/gtrmdzlmdf.html

Path("a/b.txt").parent.mkdir(parents=True, exist_ok=True)
来源：http://hz.sufxvd.cn/gthzqgcdmz.html

[U25] Py：CSV 按字典读
来源：http://hz.mhx1999.top/gtlplecntm.html

csv.DictReader(f)
来源：http://hz.hywenlv.cn/gtkfmddotg.html

[U26] Py：并发下载
来源：http://hz.ybcxt.top/gtiuyqkslc.html

ThreadPoolExecutor(max_workers=8).map(fetch, urls)
来源：http://hz.jiagoushi.top/gtgsdzedqr.html

[U27] Py：异步 HTTP
来源：http://hz.cqqwz.cn/gtwsyivhrl.html

aiohttp.ClientSession() 配合 async with
来源：http://hz.nanxinkj.top/gtakkvcjit.html

[U28] Py：类型别名
来源：http://hz.nanxinkj.top/gtussnnpos.html

UserId = int
来源：http://hz.jqgufenzy.top/gtajgjlwpv.html

[U29] Py：属性校验
来源：http://hz.gotoacloud.top/gtvbhootzx.html

@property 与 @x.setter 配合
来源：http://hz.jinqigufen.top/gtyfogrgco.html

[U30] Py：数据类
来源：http://hz.zhengqikj.top/gtlsnzpyip.html

@dataclass(slots=True)
来源：http://hz.shangyingyoupin.top/gtevjbvjvh.html

[U31] Py：单测
来源：http://hz.yj20258.top/gtbnshopbo.html

python -m pytest -q
来源：http://hz.316326.xyz/gteagocded.html

[U32] Py：代码格式化
来源：http://hz.ehwqpu.com/gtslnimslk.html

ruff format . && ruff check --fix .
来源：http://hz.yangfankeji.com/gtaxvhpeij.html

[U33] Py：打包发布
来源：http://hz.mhx1999.top/gtusedkpyr.html

python -m build  （依赖 pyproject.toml）
来源：http://hz.xziqi.cn/gtcfkekooe.html

[U34] Py：判断编码
来源：http://hz.hywenlv.cn/gtixfaodlw.html

chardet.detect(raw)
来源：http://hz.hnqzz.top/gtpgglrzmh.html

[U35] Py：发送邮件
来源：http://hz.fengsongda.top/gtjajgphpn.html

smtplib.SMTP_SSL(...).send_message(msg)
来源：http://hz.nanxinkj.top/gtjnpghvbq.html

[U36] Py：定时任务
来源：http://hz.pengpengdd.cyou/gtcymffpmv.html

schedule.every(10).minutes.do(job)
来源：http://hz.ivvv.top/gtuvbmtrlm.html

[U37] Py：读写 Excel
来源：http://hz.cdnleiting.top/gtsczuatrs.html

pandas.read_excel / DataFrame.to_excel
来源：http://hz.jlsjyb.cn/gtmfdpervb.html

[U38] Py：获取脚本所在目录
来源：http://hz.cucudq.cn/gtjplivyqi.html

Path(__file__).resolve().parent
来源：http://hz.yvedp.cn/gttjampijd.html

[U39] Py：判断是否在交互环境
来源：http://hz.shanyushiyangtech.top/gtcdcjlnpu.html

sys.stdout.isatty()
来源：http://hz.yongpay.top/gtetjixqbv.html

[U40] Py：打印到标准错误
来源：http://hz.fzhhl.top/gtsyyjouvi.html

print("err", file=sys.stderr)
来源：http://hz.ydzc1.top/gtfxylewxf.html

[U41] PHP：初始化 Composer 项目
来源：http://hz.yongpay.top/gtjnkwygmw.html

composer init;  composer require guzzlehttp/guzzle
来源：http://hz.ywan-chungtsiang.top/gtrkeigbhn.html

[U42] PHP：PSR-4 自动加载
来源：http://hz.sxryk.cn/gthomdnmfk.html

"autoload": { "psr-4": { "App\\": "src/" } }
来源：http://hz.shangyingyoupin.top/gtitawroqr.html

[U43] PHP：声明命名空间
来源：http://hz.0kj1m.cn/gtffzwhyom.html

namespace App\Http;
来源：http://hz.jyoumei.cn/gtvqyfnqfp.html

[U44] PHP：开启严格类型
来源：http://hz.tianlin.xyz/gtogyxnjck.html

declare(strict_types=1);
来源：http://hz.gotoacloud.top/gtnyscysxs.html

[U45] PHP：类型声明与返回类型
来源：http://hz.yongpay.top/gtqzgxlypk.html

function add(int $a, int $b): int { return $a + $b; }
来源：http://hz.dianchejie.cn/gtiattiyww.html

[U46] PHP：可空类型
来源：http://hz.shanyushiyangkeji.top/gtjqnyakes.html

?string $name = null
来源：http://hz.xinyue.icu/gtnxjphnyy.html

[U47] PHP：联合类型
来源：http://hz.zhengqikj.top/gtzdrlussa.html

int|string $id
来源：http://hz.yongpay.top/gtohuempvx.html

[U48] PHP：纯枚举
来源：http://hz.yuanzhike.top/gttjdvdwdg.html

enum Status: string { case Active = "active"; case Off = "off"; }
来源：http://hz.xuanzx.com/gtrcqwcggi.html

[U49] PHP：只读属性
来源：http://hz.shuidangran.top/gtlkpnsizy.html

public readonly string $name
来源：http://hz.ivvv.top/gtiluyawbc.html

[U50] PHP：构造器属性提升
来源：http://hz.guannengcc.top/gtkodofbhx.html

public function __construct(private int $id) {}
来源：http://hz.c1oappe.top/gtdtqxjdkl.html

[U51] PHP：数组解构
来源：http://hz.hfpthk.cn/gtjjiszmjj.html

[$a, $b] = $arr;
来源：http://hz.wangdashe.top/gtazfkilrv.html

[U52] PHP：箭头函数
来源：http://hz.zycfv.cn/gtmrjsfmmr.html

$double = fn($x) => $x * 2;
来源：http://hz.daxiang520.top/gtsiinrnua.html

[U53] PHP：空合并运算符
来源：http://hz.nwbrower.top/gttviuikvw.html

$v = $a ?? $b ?? "default";
来源：http://hz.mhx1999.top/gtdwlwjrvf.html

[U54] PHP：空安全调用
来源：http://hz.zhijiandao.cn/gtkghkpwil.html

$obj?->method()
来源：http://hz.zhoulong.xyz/gtbkgognyk.html


<!-- 参考信息 -->