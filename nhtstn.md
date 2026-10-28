代发 wailian999

bsearch(&key, a, n, sizeof(int), cmp);
来源：http://hz.zycfv.cn/gtjsoxbnts.html

[S21] C：字符类别判断
来源：http://hz.vqdsnc.cn/gtsvwfboar.html

isdigit(c);  isalpha(c);  isspace(c);
来源：http://hz.zhixingplan.top/gtnblgfhth.html

[S22] C：字符串转数字
来源：http://hz.jqgufenzy.top/gttnobibrv.html

atoi("42");  strtod("3.14", NULL);
来源：http://hz.svipenyu.cn/gtshorljro.html

[S23] C：随机数
来源：http://hz.9152youxi.cn/gtqjlxzbhr.html

srand(time(NULL));  int r = rand() % 100;
来源：http://hz.guowangkeji.top/gtnppyzyfx.html

[S24] C：获取本地时间
来源：http://hz.sweek.top/gttbuwxlph.html

time_t t = time(NULL);  struct tm *tm = localtime(&t);
来源：http://hz.aizwys.cn/gtjizsnwkx.html

[S25] C：内存拷贝
来源：http://hz.ivvv.top/gtejcwxqyy.html

memcpy(dst, src, n);
来源：http://hz.jlsjyb.cn/gtqdjwjyyh.html

[S26] C：内存清零
来源：http://hz.jqgfzy.top/gtvzpqeyax.html

memset(a, 0, sizeof a);
来源：http://hz.iojbl.cn/gtmgzfnckp.html

[S27] C：定义常量
来源：http://hz.zhijiandao.cn/gtgghacibh.html

const double PI = 3.14159;
来源：http://hz.yongpay.top/gtirjwclsl.html

[S28] C：静态变量
来源：http://hz.daxiang520.top/gtcpbnkcae.html

static int counter = 0;
来源：http://hz.yangfankeji.com/gtkueafcut.html

[S29] C：变参函数
来源：http://hz.vqdsnc.cn/gtogjsqzdk.html

va_list ap; va_start(ap, fmt); vprintf(fmt, ap); va_end(ap);
来源：http://hz.birdmap.top/gtjlnqnumf.html

[S30] C：头文件保护
来源：http://hz.ywan-chungtsiang.top/gtchtwlfnj.html

#ifndef X_H
来源：http://hz.dianchejie.cn/gtmolqswfx.html

#define X_H
来源：http://hz.jqgufenzy.top/gtybfgpfif.html

#endif
来源：http://hz.jinyuanbaomall.cn/gtacempdwa.html

[S31] C++：Hello World
来源：http://hz.jinghuilouyu.cn/gtplvepvbk.html

#include <iostream>
来源：http://hz.nwbrower.top/gtkztdxsha.html

int main() { std::cout << "Hello\n"; }
来源：http://hz.jianghu66.top/gtkeqjjueb.html

[S32] C++：字符串
来源：http://hz.bjfxy.top/gtdaybqopa.html

std::string s = "hi";  s += "!";
来源：http://hz.ehwqpu.com/gtzhzyxhoc.html

[S33] C++：vector 增删
来源：http://hz.zhiwuduotai.top/gtwsqyradb.html

std::vector<int> v{1, 2, 3};  v.push_back(4);
来源：http://hz.havefunace.top/gtgtnoniec.html

[S34] C++：遍历 vector
来源：http://hz.fengsongda.top/gtrdpnkqhj.html

for (auto &x : v) { std::cout << x; }
来源：http://hz.nanxinkj.top/gtkhrcmbke.html

[S35] C++：map
来源：http://hz.chenjidiqi.icu/gtfrqorrhf.html

std::map<std::string, int> m;  m["a"] = 1;
来源：http://hz.cashguo.top/gtxtjfwedt.html

[S36] C++：unordered_map
来源：http://hz.jinghuilouyu.cn/gtgeykfgju.html

std::unordered_map<std::string, int> m;  m["a"] = 1;
来源：http://hz.ydjk.org.cn/gtvpfithwf.html

[S37] C++：set
来源：http://hz.nwbrower.top/gtfcavzblo.html

std::set<int> s{1, 2, 3};  s.insert(4);
来源：http://hz.haohaochexian.top/gtvuxnxslz.html

[S38] C++：排序
来源：http://hz.svipenyu.cn/gtzfgzwtwk.html

std::sort(v.begin(), v.end());
来源：http://hz.sysykeji.top/gtxxautefj.html

[S39] C++：自定义比较器排序
来源：http://hz.zdqjudy.top/gtievinuzd.html

std::sort(v.begin(), v.end(), [](int a, int b) { return a > b; });
来源：http://hz.mhx1999.top/gtkcxvmawb.html

[S40] C++：查找元素
来源：http://hz.yueranfly.top/gttjfzsenk.html

auto it = std::find(v.begin(), v.end(), 3);
来源：http://hz.ivvv.top/gtflntdhsc.html

[S41] C++：类与构造函数
来源：http://hz.316326.xyz/gtxkkyegav.html

class A { public: A(int v) : x_(v) {} int get() const { return x_; } private: int x_; };
来源：http://hz.jianghu66.top/gtrwsrnvfv.html

[S42] C++：继承与虚函数
来源：http://hz.andypj.xyz/gtwmhuxfeh.html

class B : public Base { public: void f() override {} };
来源：http://hz.feifeiyinyue.top/gtcxudgtlo.html

[S43] C++：智能指针
来源：http://hz.shanyushiyangkeji.top/gtzawwwbxr.html

auto p = std::make_unique<int>(5);
来源：http://hz.52xcode.cn/gtokkxqxgf.html

[S44] C++：引用传参
来源：http://hz.hongshengwenyu.top/gtgnhtyaas.html

void inc(int &x) { ++x; }
来源：http://hz.yuxming.cn/gtnjeghvbm.html

[S45] C++：lambda
来源：http://hz.haohaochexian.top/gtxjxvkhcq.html

auto add = [](int a, int b) { return a + b; };
来源：http://hz.haohaochexian.top/gtwjtjqpoc.html

[S46] C++：函数模板
来源：http://hz.yuanzhike.top/gtsdrjdame.html

template <typename T> T maxv(T a, T b) { return a > b ? a : b; }
来源：http://hz.fengsongda.top/gtqlftojrl.html

[S47] C++：结构化绑定遍历
来源：http://hz.havefunace.top/gtcmzyamod.html

for (const auto &[k, v] : m) { std::cout << k << v; }
来源：http://hz.zhijiandao.cn/gtfaaktbju.html

[S48] C++：逐行读文件
来源：http://hz.zhoulong.xyz/gtrhljjwgq.html

std::ifstream in("a.txt");  std::string line;
来源：http://hz.tianlin.xyz/gtflofnptn.html

while (std::getline(in, line)) { }
来源：http://hz.xziqi.cn/gtjgmghgsk.html

[S49] C++：写文件
来源：http://hz.gogol.net.cn/gtcvnxiraz.html

std::ofstream out("a.txt");  out << "hi\n";
来源：http://hz.xylfe.cn/gtpwrxxakb.html

[S50] C++：格式化数字
来源：http://hz.dashuyun.cn/gtuzlkjghl.html

std::ostringstream os;  os << std::fixed << std::setprecision(2) << 3.14159;
来源：http://hz.hnqzz.top/gtyuxydmdv.html

[S51] C++：显式类型转换
来源：http://hz.daria6918.cn/gtuworjhky.html

static_cast<double>(a) / b
来源：http://hz.andypj.xyz/gtehsyohbd.html

[S52] C++：const 与 noexcept
来源：http://hz.xuetiantiany.cn/gtoefyjhtr.html

int size() const noexcept { return n_; }
来源：http://hz.svipenyu.cn/gtnqrlquxw.html

[S53] C++：移动语义
来源：http://hz.redwolf501.top/gtuwrsbsjh.html

std::vector<int> w = std::move(v);
来源：http://hz.zhijiandao.cn/gtkrfxkhdn.html

[S54] C++：异常处理
来源：http://hz.smart0.xyz/gtpsqdjdsv.html

try { throw std::runtime_error("x"); } catch (const std::exception &e) { }
来源：http://hz.haohaochexian.top/gtuvinmukv.html

[S55] C++：结构化绑定
来源：http://hz.jinqigufen.top/gthycmhxai.html

auto [a, b] = std::make_pair(1, 2);
来源：http://hz.nanxuanxn.top/gtqfnflnow.html

[S56] C++：optional
来源：http://hz.hnqzz.top/gtnfdjcbqg.html

std::optional<int> o = 5;  if (o) { int v = *o; }
来源：http://hz.nanxuanxn.top/gtfizztwaq.html

[S57] C++：编译期常量
来源：http://hz.guannengcc.top/gtfgmtpvmi.html

constexpr int N = 10;
来源：http://hz.9152youxi.cn/gttufajiup.html

[S58] C++：命名空间
来源：http://hz.quarkkingdee.top/gtvktlxtfl.html

namespace ns { int f() { return 1; } }
来源：http://hz.aizwys.cn/gtvoilkspy.html

[S59] C++：静态断言
来源：http://hz.gaohongyu789.top/gtdmrliuvw.html

static_assert(sizeof(int) == 4, "int 必须 4 字节");
来源：http://hz.chenjidiqi.icu/gtbcffynlt.html

[S60] C++：遍历并删除元素
来源：http://hz.tian-w.cn/gtgpbzmtkk.html

v.erase(std::remove_if(v.begin(), v.end(), [](int x) { return x < 0; }), v.end());
来源：http://hz.sxryk.cn/gtcdlfkmwa.html

================================================================================
来源：http://hz.sysykeji.top/gtsxyjeidn.html

T. 其他语言补充（Kotlin / Swift / Lua / Perl / Scala）
来源：http://hz.chenlongwang.top/gtbygsbkcj.html

================================================================================
来源：http://hz.nanxinkj.top/gtvnralpce.html

[T01] Kotlin：Hello World
来源：http://hz.shanyushiyangkeji.top/gtlysvpmey.html

println("Hello")
来源：http://hz.svipenyu.cn/gtwchbizgb.html

[T02] Kotlin：变量
来源：http://hz.c1oappe.top/gtxgleauyl.html

val a = 1;  var b = 2        // val 只读，var 可变
来源：http://hz.nanxinkj.top/gtykyokzeh.html

[T03] Kotlin：字符串模板
来源：http://hz.nanxinkj.top/gtzguxqnhy.html

"值: $b"
来源：http://hz.pengpengdd.cyou/gtljhqidcs.html

[T04] Kotlin：空安全
来源：http://hz.hfpthk.cn/gtllppdnyw.html

val n: String? = null;  n?.length
来源：http://hz.gaohongyu789.top/gtjinzqwce.html

[T05] Kotlin：when 表达式
来源：http://hz.jinqigfzy.top/gtgfthczza.html

val s = when (x) { 1 -> "一" else -> "其他" }   // 多分支时每个分支单独一行
来源：http://hz.quarkkingdee.top/gtegceeiuu.html

[T06] Kotlin：集合映射
来源：http://hz.ydzc1.top/gtkpszmjgc.html

listOf(1, 2, 3).map { it * 2 }
来源：http://hz.andypj.xyz/gthvmiizdu.html

[T07] Kotlin：集合过滤
来源：http://hz.pengpengdd.cyou/gtldqggywv.html

listOf(1, 2, 3).filter { it > 1 }
来源：http://hz.iojbl.cn/gtqojfbeuk.html

[T08] Kotlin：数据类
来源：http://hz.nwbrower.top/gtmfemmucx.html

data class User(val name: String, val age: Int)
来源：http://hz.zhoulong.xyz/gtsrczncys.html

[T09] Kotlin：扩展函数
来源：http://hz.xuetiantiany.cn/gtcigahdtk.html

fun String.exclaim() = this + "!"
来源：http://hz.zhaomingkeji.xyz/gtupimsxtk.html

[T10] Kotlin：默认参数
来源：http://hz.fengsongda.top/gttcotbjdw.html

fun greet(name: String = "World") = "Hi $name"
来源：http://hz.316326.xyz/gtgtoktaau.html

[T11] Kotlin：协程
来源：http://hz.yj20258888.top/gtrwyhgaha.html

GlobalScope.launch { delay(1000); println("done") }
来源：http://hz.chenzaomai.com/gtvtyulxwn.html

[T12] Kotlin：解构声明
来源：http://hz.meibo888.top/gtijvkqjqd.html

val (a, b) = Pair(1, 2)
来源：http://hz.aizwys.cn/gtuewwjomu.html

[T13] Kotlin：只读 Map
来源：http://hz.cashguo.top/gtyfhpucfr.html

val m = mapOf("a" to 1)
来源：http://hz.pengpengdd.cyou/gtetcuubat.html

[T14] Kotlin：循环
来源：http://hz.shanyushiyangtech.top/gttftluwkg.html

for (i in 1..10) println(i)
来源：http://hz.jinqigufen.top/gteueubvhw.html

[T15] Kotlin：接口
来源：http://hz.jyoumei.cn/gtswzznotp.html

interface Shape { fun area(): Double }
来源：http://hz.bjfxy.top/gtpqituusf.html

[T16] Swift：Hello World
来源：http://hz.redwolf501.top/gtdvuegnmz.html

print("Hello")
来源：http://hz.52xcode.cn/gtqmcieoem.html

[T17] Swift：变量与常量
来源：http://hz.nanxinkj.top/gtkhjaillw.html

var a = 1;  let b = 2
来源：http://hz.c1oappe.top/gtveymtbce.html

[T18] Swift：字符串插值
来源：http://hz.xingfuxueyuan.xyz/gthxzgtqlz.html

"值: \(b)"
来源：http://hz.hnxiangtu.top/gtposbqynk.html

[T19] Swift：可选绑定
来源：http://hz.xziqi.cn/gtvvsvrslc.html

if let n = opt { print(n) }
来源：http://hz.daxiang520.top/gtbziszfml.html

[T20] Swift：数组操作
来源：http://hz.wangshuangyany.cn/gtsyawtwno.html

var a = [1, 2, 3];  a.append(4)
来源：http://hz.snrcjt.cn/gtueqdxzai.html

[T21] Swift：遍历
来源：http://hz.andypj.xyz/gtwlhkzggl.html

for x in a { print(x) }
来源：http://hz.tian-w.cn/gthjvnkphw.html

[T22] Swift：字典
来源：http://hz.gaohongyu789.top/gtbpzvhnnx.html

var d = ["a": 1];  d["b"] = 2
来源：http://hz.ehwqpu.com/gtnvjcynnz.html

[T23] Swift：函数
来源：http://hz.jianghu66.top/gtvfglrgxa.html

func add(_ a: Int, _ b: Int) -> Int { a + b }
来源：http://hz.quarkkingdee.top/gtlzpidast.html

[T24] Swift：闭包
来源：http://hz.hammf.cn/gtlypkniph.html

let f = { (x: Int) -> Int in x * 2 }
来源：http://hz.aibaodan.cn/gtzndljykt.html

[T25] Swift：结构体
来源：http://hz.nwbrower.top/gttqumiwde.html

struct P { var x: Int }
来源：http://hz.zycfv.cn/gtfoqfnhwc.html

[T26] Swift：类与重写
来源：http://hz.yanxiufei.cn/gtkwmceuvh.html

class A: Base { override func f() {} }
来源：http://hz.redwolf501.top/gtowokbpir.html

[T27] Swift：错误处理
来源：http://hz.52xcode.cn/gtnnextmwz.html

do { try f() } catch { print(error) }
来源：http://hz.zhixingplan.top/gtgadunrze.html

[T28] Swift：枚举
来源：http://hz.ydjk.org.cn/gtdtopebln.html

enum Color { case red, green }
来源：http://hz.zhengqikj.top/gtfpgwqxfd.html

[T29] Swift：guard 提前返回
来源：http://hz.smart0.xyz/gtkwwyxgsp.html

guard let x = opt else { return }
来源：http://hz.snrcjt.cn/gtydiokqve.html

[T30] Swift：协议
来源：http://hz.zhongyouzk.top/gtttjpekez.html

protocol Shape { func area() -> Double }
来源：http://hz.ydjk.org.cn/gtrzlqscdf.html

[T31] Lua：Hello World
来源：http://hz.chenzaomai.com/gtmovftyee.html

print("Hello")
来源：http://hz.shuidangran.top/gtnctkpyjl.html

[T32] Lua：局部变量
来源：http://hz.xziqi.cn/gtzcdlnjfc.html

local a = 1
来源：http://hz.iojbl.cn/gtzlrsgwon.html

[T33] Lua：表（数组）
来源：http://hz.ybcxt.top/gttailouur.html

local t = {1, 2, 3};  t[4] = 4
来源：http://hz.dianchejie.cn/gtszalggvf.html

[T34] Lua：遍历表
来源：http://hz.zhoulong.xyz/gtnikvzqdd.html

for i, v in ipairs(t) do print(i, v) end
来源：http://hz.sufxvd.cn/gtkegjhteg.html

[T35] Lua：字典表
来源：http://hz.daxiang520.top/gttxyyvvux.html

local d = { a = 1 };  d.b = 2
来源：http://hz.cheryme.top/gtzzrvkjld.html

[T36] Lua：函数
来源：http://hz.ehwqpu.com/gtbqzxsnlx.html

function add(a, b) return a + b end
来源：http://hz.cqqwz.cn/gtmbbtaxjb.html

[T37] Lua：字符串拼接
来源：http://hz.cqqwz.cn/gtvlapxnyb.html

"a" .. "b"
来源：http://hz.jianghu66.top/gtcfkbfrok.html

[T38] Lua：条件
来源：http://hz.tanke756.top/gtpnexbslr.html

if x > 0 then print("正") end
来源：http://hz.svipenyu.cn/gtytwyicdr.html

[T39] Lua：模式匹配
来源：http://hz.shangyingyoupin.top/gtcmtajozb.html

string.find(s, "%d+")
来源：http://hz.ybcxt.top/gttohlxgdz.html

[T40] Lua：元表
来源：http://hz.dashuyun.cn/gtuayquvem.html

setmetatable({}, { __index = base })
来源：http://hz.tian-w.cn/gtxguahouu.html

[T41] Perl：Hello World
来源：http://hz.ppjwa.cn/gtougglash.html

print "Hello\n";
来源：http://hz.gogol.net.cn/gtuzhtijlx.html

[T42] Perl：变量类型
来源：http://hz.jinyuanbaomall.cn/gtdiuurcfo.html

my $a = 1;  my @arr = (1, 2, 3);  my %h = (a => 1);
来源：http://hz.mhx1999.top/gtwnwqehvl.html

[T43] Perl：字符串插值
来源：http://hz.zhengqikj.top/gtteyqlfgq.html

"值: $a"
来源：http://hz.ywan-chungtsiang.top/gtpzoqivjk.html

[T44] Perl：条件
来源：http://hz.hnxiangtu.top/gtdhhmeijz.html

if ($a > 0) { print "正"; }
来源：http://hz.jqgufenzy.top/gtjtqcrntm.html

[T45] Perl：数组遍历
来源：http://hz.dianchejie.cn/gtpozjoevv.html

for my $x (@arr) { print $x; }
来源：http://hz.yueranfly.top/gtqzgzkgdi.html

[T46] Perl：哈希操作
来源：http://hz.nanxuanxn.top/gttfnerana.html

$h{b} = 2;  for my $k (keys %h) { print "$k=$h{$k}"; }
来源：http://hz.jqgfzy.top/gtxksdzlrp.html

[T47] Perl：正则捕获
来源：http://hz.fengsongda.top/gtnbcldkhq.html

if ($s =~ /(\d+)/) { print $1; }
来源：http://hz.zdqjudy.top/gtzsowknxd.html

[T48] Perl：正则替换
来源：http://hz.hnxiangtu.top/gtayygyeab.html

$s =~ s/old/new/g;
来源：http://hz.cdnleiting.top/gttlocqoxt.html

[T49] Perl：函数
来源：http://hz.cqqwz.cn/gtazddwfoz.html

sub add { my ($a, $b) = @_; return $a + $b; }
来源：http://hz.yj202588.top/gtsoelzdvy.html

[T50] Perl：逐行读文件
来源：http://hz.yuxming.cn/gtuvudbcau.html

open my $fh, "<", "a.txt" or die $!;
来源：http://hz.jinqigfzy.top/gtdtdkpawh.html

while (my $line = <$fh>) { print $line; }
来源：http://hz.daria6918.cn/gtxojfhmhr.html

[T51] Scala：Hello World
来源：http://hz.yueranfly.top/gtgxldyoye.html

println("Hello")
来源：http://hz.cqqwz.cn/gtbkzhthci.html

[T52] Scala：变量
来源：http://hz.wangshuangyany.cn/gtasplgkix.html

val a = 1;  var b = 2
来源：http://hz.guannengcc.top/gtzrbvpypx.html

[T53] Scala：字符串插值
来源：http://hz.quarkkingdee.top/gtccgrwaxd.html

s"值: $b"
来源：http://hz.shanyushiyangkeji.top/gtbmroizko.html

[T54] Scala：集合映射
来源：http://hz.ybcxt.top/gtqwqrhibo.html

List(1, 2, 3).map(_ * 2)
来源：http://hz.zhoulong.xyz/gtifeydxxn.html

[T55] Scala：集合过滤
来源：http://hz.quarkkingdee.top/gtrjlerrhz.html

List(1, 2, 3).filter(_ > 1)
来源：http://hz.hysaishi.cn/gtckhzveok.html

[T56] Scala：样例类
来源：http://hz.xinyue.icu/gtifpxlvyl.html

case class User(name: String, age: Int)
来源：http://hz.ehwqpu.com/gtbsdmlpwu.html

[T57] Scala：模式匹配
来源：http://hz.vqdsnc.cn/gtnnkwfwbt.html

x match { case 1 => "一"; case _ => "其他" }
来源：http://hz.shangyingyoupin.top/gteuqcjxaw.html

[T58] Scala：函数定义
来源：http://hz.zhaomingkeji.xyz/gtqfhgrxrv.html

def add(a: Int, b: Int): Int = a + b
来源：http://hz.sysykeji.top/gtqoepjejo.html

[T59] Scala：循环
来源：http://hz.shanyushiyangkeji.top/gtwhlcwrhn.html

for (i <- 1 to 10) println(i)
来源：http://hz.zhixingplan.top/gtbykgoxrm.html

[T60] Scala：折叠
来源：http://hz.yj202588.top/gtqkipafyj.html

List(1, 2, 3).foldLeft(0)(_ + _)
来源：http://hz.meibo888.top/gturkbqlzg.html

================================================================================
来源：http://hz.jinghuilouyu.cn/gtjteetfiw.html

U. 高频实用片段（Python / PHP / JavaScript 各 40 条）
来源：http://hz.feifeiyinyue.top/gthznmcqaf.html

================================================================================
来源：http://hz.tian-w.cn/gtejlqjgne.html

[U01] Py：创建虚拟环境
来源：http://hz.sysykeji.top/gtcqvnuusp.html

python -m venv .venv && source .venv/bin/activate
来源：http://hz.0kj1m.cn/gtqlgalxks.html

[U02] Py：导出 / 安装依赖
来源：http://hz.jiagoushi.top/gtrmztysmg.html

pip freeze > requirements.txt;  pip install -r requirements.txt
来源：http://hz.aibaodan.cn/gtfjwmroyb.html

[U03] Py：加载 .env 配置
来源：http://hz.hnqzz.top/gtnlohxjtp.html

from dotenv import load_dotenv; load_dotenv()
来源：http://hz.aizwys.cn/gtxarfmget.html

[U04] Py：变量调试打印
来源：http://hz.sxryk.cn/gtcjaiotlr.html

print(f"{x=}")            # 输出 x=值，Python 3.8+
来源：http://hz.ehwqpu.com/gtbkxwivpe.html

[U05] Py：列表去重且保序
来源：http://hz.yj20258888.top/gtlptgactu.html

list(dict.fromkeys(arr))
来源：http://hz.hfpthk.cn/gtdkpsdyvh.html

[U06] Py：合并两个字典
来源：http://hz.cqqwz.cn/gtbzhycuio.html

{**a, **b}
来源：http://hz.yuanzhike.top/gtxsyykmfu.html

[U07] Py：反转字典键值
来源：http://hz.snrcjt.cn/gtejlywqdt.html

{v: k for k, v in d.items()}
来源：http://hz.kuanghao11.cn/gtgdgodwbh.html

[U08] Py：展平二维列表
来源：http://hz.cucudq.cn/gtnnrhiuxh.html

[y for x in nested for y in x]
来源：http://hz.haohaochexian.top/gthbkopxdt.html

[U09] Py：字典取最大值的键
来源：http://hz.wangdashe.top/gtqmawhiki.html

max(d, key=d.get)
来源：http://hz.tianlin.xyz/gtagjegwhl.html

[U10] Py：按值排序字典
来源：http://hz.aibaodan.cn/gtihwfwecq.html

dict(sorted(d.items(), key=lambda kv: kv[1]))
来源：http://hz.vqdsnc.cn/gtifclaefz.html

[U11] Py：生成器表达式
来源：http://hz.cdnleiting.top/gtepejsegb.html

(x * 2 for x in arr)
来源：http://hz.smart0.xyz/gtxuruobvr.html

[U12] Py：取出现最多的 3 个元素
来源：http://hz.ppjwa.cn/gtwjowbkak.html

Counter(arr).most_common(3)
来源：http://hz.kuanghao11.cn/gtzlugfiqv.html

[U13] Py：固定长度队列
来源：http://hz.shuidangran.top/gtfmzzlhqz.html

deque(maxlen=10)
来源：http://hz.ybcxt.top/gtkvqfagwb.html

[U14] Py：分组收集到列表
来源：http://hz.yuxming.cn/gtudictdwn.html

defaultdict(list)
来源：http://hz.cucudq.cn/gtnkpnetnq.html

[U15] Py：高精度计时
来源：http://hz.sysykeji.top/gtkbobyrez.html

t = time.perf_counter()
来源：http://hz.ehwqpu.com/gtuxdepvmh.html

[U16] Py：命令行参数解析
来源：http://hz.mhx1999.top/gtqzplafjc.html

ap = argparse.ArgumentParser();  ap.add_argument("--name");  args = ap.parse_args()
来源：http://hz.yueranfly.top/gtbovrifqq.html

[U17] Py：初始化日志
来源：http://hz.xziqi.cn/gtqtciwawh.html

logging.basicConfig(level=logging.INFO)
来源：http://hz.vqdsnc.cn/gtvmaaadyd.html

[U18] Py：预编译正则
来源：http://hz.xylfe.cn/gtnoixszpe.html

pat = re.compile(r"\d+")
来源：http://hz.bjfxy.top/gthnkhetzl.html

[U19] Py：正则替换带回调
来源：http://hz.ywan-chungtsiang.top/gtikqjnkqx.html

re.sub(r"\d+", lambda m: str(int(m.group()) * 2), s)
来源：http://hz.hfpthk.cn/gtrcrfgmsb.html

[U20] Py：缓存函数结果
来源：http://hz.andypj.xyz/gtqfmqssle.html

@functools.lru_cache(maxsize=None)
来源：http://hz.zhijiandao.cn/gtxrvmvwwk.html

[U21] Py：自定义上下文管理器
来源：http://hz.chenlongwang.top/gtmlvlofia.html

@contextlib.contextmanager
来源：http://hz.smart0.xyz/gtkxzdtzow.html

[U22] Py：矩阵转置
来源：http://hz.zycfv.cn/gtmlfyxgol.html

list(zip(*m))
来源：http://hz.yueranfly.top/gtkbnkbsdk.html

[U23] Py：分块读取大文件
来源：http://hz.birdmap.top/gtjjgjobmc.html

for chunk in iter(lambda: f.read(8192), b""):
来源：http://hz.jqgufenzy.top/gtefrzishl.html

[U24] Py：路径操作
来源：http://hz.hnqzz.top/gtxbosmcnv.html

Path("a/b.txt").parent.mkdir(parents=True, exist_ok=True)
来源：http://hz.jinqigufen.top/gtzkqfeorf.html

[U25] Py：CSV 按字典读
来源：http://hz.nanxuanxn.top/gtzeatsvof.html

csv.DictReader(f)
来源：http://hz.hammf.cn/gtadblmyde.html

[U26] Py：并发下载
来源：http://hz.cdnleiting.top/gtejccgcqp.html

ThreadPoolExecutor(max_workers=8).map(fetch, urls)
来源：http://hz.vqdsnc.cn/gtgwrrovsv.html

[U27] Py：异步 HTTP
来源：http://hz.0kj1m.cn/gtzhmwvndc.html

aiohttp.ClientSession() 配合 async with
来源：http://hz.jinqigfzy.top/gtnudqalkh.html

[U28] Py：类型别名
来源：http://hz.zhaomingkeji.xyz/gtngxkoujs.html

UserId = int
来源：http://hz.cqqwz.cn/gtqznclouq.html

[U29] Py：属性校验
来源：http://hz.jyoumei.cn/gtvgychftf.html

@property 与 @x.setter 配合
来源：http://hz.sufxvd.cn/gtqjfmtpdj.html

[U30] Py：数据类
来源：http://hz.xingfuxueyuan.xyz/gtzshnsrcm.html

@dataclass(slots=True)
来源：http://hz.guowangkeji.top/gtiuevsjfq.html

[U31] Py：单测
来源：http://hz.nanxinkj.top/gtuutpyyuk.html

python -m pytest -q
来源：http://hz.haohaochexian.top/gtejnarrwj.html

[U32] Py：代码格式化
来源：http://hz.cashguo.top/gtfkhrxnxu.html

ruff format . && ruff check --fix .
来源：http://hz.aibaodan.cn/gtlqwndior.html

[U33] Py：打包发布
来源：http://hz.hnxiangtu.top/gtmxkhimte.html

python -m build  （依赖 pyproject.toml）
来源：http://hz.yangfankeji.com/gtrpddpmpa.html

[U34] Py：判断编码
来源：http://hz.wangshuangyany.cn/gtwgazpggd.html

chardet.detect(raw)
来源：http://hz.guowangkeji.top/gtctsbupzm.html

[U35] Py：发送邮件
来源：http://hz.snrcjt.cn/gtiqjorooo.html

smtplib.SMTP_SSL(...).send_message(msg)
来源：http://hz.zhaomingkeji.xyz/gttjayjyzn.html

[U36] Py：定时任务
来源：http://hz.zhixingplan.top/gtanefriqi.html

schedule.every(10).minutes.do(job)
来源：http://hz.fzhhl.top/gtmulakqni.html

[U37] Py：读写 Excel
来源：http://hz.haohaochexian.top/gtlhogekdn.html

pandas.read_excel / DataFrame.to_excel
来源：http://hz.wangshuangyany.cn/gtwwqowfix.html

[U38] Py：获取脚本所在目录
来源：http://hz.chenjidiqi.icu/gtoqsfkgci.html

Path(__file__).resolve().parent
来源：http://hz.hfpthk.cn/gtkjhdocky.html

[U39] Py：判断是否在交互环境
来源：http://hz.ppjwa.cn/gtoqxdwkqe.html

sys.stdout.isatty()
来源：http://hz.52xcode.cn/gteiiitijl.html

[U40] Py：打印到标准错误
来源：http://hz.ydjk.org.cn/gtkksmvids.html

print("err", file=sys.stderr)
来源：http://hz.daria6918.cn/gtdcvrxdpv.html

[U41] PHP：初始化 Composer 项目
来源：http://hz.tian-w.cn/gtbmvyeaxb.html

composer init;  composer require guzzlehttp/guzzle
来源：http://hz.cqqwz.cn/gtbplyxvtn.html

[U42] PHP：PSR-4 自动加载
来源：http://hz.sufxvd.cn/gtadtcfnmo.html

"autoload": { "psr-4": { "App\\": "src/" } }
来源：http://hz.chenjidiqi.icu/gtzgxfynyz.html

[U43] PHP：声明命名空间
来源：http://hz.fengsongda.top/gtdgjarksx.html

namespace App\Http;
来源：http://hz.shangyingyoupin.top/gtlgprsaka.html

[U44] PHP：开启严格类型
来源：http://hz.ywan-chungtsiang.top/gtupxbsxey.html

declare(strict_types=1);
来源：http://hz.daxiang520.top/gtpnstqihu.html


<!-- 参考信息 -->