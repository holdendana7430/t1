代发 wailian999

time_t t = time(NULL);  struct tm *tm = localtime(&t);
来源：http://hz.guannengcc.top/gtdbjtckfs.html

[S25] C：内存拷贝
来源：http://hz.chenzaomai.com/gtjykbdjdx.html

memcpy(dst, src, n);
来源：http://hz.cdnleiting.top/gtaiozqpty.html

[S26] C：内存清零
来源：http://hz.c1oappe.top/gtndhifgzo.html

memset(a, 0, sizeof a);
来源：http://hz.sweek.top/gtvxkkwlye.html

[S27] C：定义常量
来源：http://hz.mhx1999.top/gtnhkpjsay.html

const double PI = 3.14159;
来源：http://hz.hongshengwenyu.top/gtlybarwrx.html

[S28] C：静态变量
来源：http://hz.tian-w.cn/gtdumygxgi.html

static int counter = 0;
来源：http://hz.wangdashe.top/gtrukhdfkf.html

[S29] C：变参函数
来源：http://hz.sxryk.cn/gtkqmfjlus.html

va_list ap; va_start(ap, fmt); vprintf(fmt, ap); va_end(ap);
来源：http://hz.aizwys.cn/gthyhuiwyf.html

[S30] C：头文件保护
来源：http://hz.redwolf501.top/gtfjkruifa.html

#ifndef X_H
来源：http://hz.mhx1999.top/gtciqxduot.html

#define X_H
来源：http://hz.tianlin.xyz/gtnwfpjwui.html

#endif
来源：http://hz.hysaishi.cn/gtxultaalz.html

[S31] C++：Hello World
来源：http://hz.zdqjudy.top/gtnlpizljf.html

#include <iostream>
来源：http://hz.wangdashe.top/gtestahgis.html

int main() { std::cout << "Hello\n"; }
来源：http://hz.yuxming.cn/gtenonytal.html

[S32] C++：字符串
来源：http://hz.jinqigufen.top/gttujvbrov.html

std::string s = "hi";  s += "!";
来源：http://hz.aibaodan.cn/gthrtjsggw.html

[S33] C++：vector 增删
来源：http://hz.c1oappe.top/gtlgxzokzy.html

std::vector<int> v{1, 2, 3};  v.push_back(4);
来源：http://hz.52xcode.cn/gtoptyrytl.html

[S34] C++：遍历 vector
来源：http://hz.ydjk.org.cn/gtgepsbpmr.html

for (auto &x : v) { std::cout << x; }
来源：http://hz.svipenyu.cn/gtunzabuqt.html

[S35] C++：map
来源：http://hz.zhengqikj.top/gtaxduclcd.html

std::map<std::string, int> m;  m["a"] = 1;
来源：http://hz.ydzc1.top/gtqjpjzvfk.html

[S36] C++：unordered_map
来源：http://hz.nwbrower.top/gtoqbnfjij.html

std::unordered_map<std::string, int> m;  m["a"] = 1;
来源：http://hz.ybcxt.top/gtvxnwsofm.html

[S37] C++：set
来源：http://hz.guowangkeji.top/gtxphkbgaw.html

std::set<int> s{1, 2, 3};  s.insert(4);
来源：http://hz.snrcjt.cn/gtbcdhwczz.html

[S38] C++：排序
来源：http://hz.aizwys.cn/gtdnveqkfb.html

std::sort(v.begin(), v.end());
来源：http://hz.aizwys.cn/gtocneddsh.html

[S39] C++：自定义比较器排序
来源：http://hz.cdnleiting.top/gtzcbibrgo.html

std::sort(v.begin(), v.end(), [](int a, int b) { return a > b; });
来源：http://hz.316326.xyz/gtfphiahsw.html

[S40] C++：查找元素
来源：http://hz.cucudq.cn/gtkpxkdazg.html

auto it = std::find(v.begin(), v.end(), 3);
来源：http://hz.hongshengwenyu.top/gtzvqifale.html

[S41] C++：类与构造函数
来源：http://hz.yueranfly.top/gtuuasiqwr.html

class A { public: A(int v) : x_(v) {} int get() const { return x_; } private: int x_; };
来源：http://hz.hongshengwenyu.top/gtddpfqmqv.html

[S42] C++：继承与虚函数
来源：http://hz.andypj.xyz/gtwqvttqxa.html

class B : public Base { public: void f() override {} };
来源：http://hz.jinyuanbaomall.cn/gtjxmbvzuh.html

[S43] C++：智能指针
来源：http://hz.fzhhl.top/gtmkokgvqi.html

auto p = std::make_unique<int>(5);
来源：http://hz.andypj.xyz/gtisvdxpwd.html

[S44] C++：引用传参
来源：http://hz.hfpthk.cn/gtemjdxlow.html

void inc(int &x) { ++x; }
来源：http://hz.quarkkingdee.top/gtpkptiwxh.html

[S45] C++：lambda
来源：http://hz.sxryk.cn/gtjhfhtthe.html

auto add = [](int a, int b) { return a + b; };
来源：http://hz.hfpthk.cn/gtqxorosvn.html

[S46] C++：函数模板
来源：http://hz.jyoumei.cn/gtgyprhibu.html

template <typename T> T maxv(T a, T b) { return a > b ? a : b; }
来源：http://hz.52xcode.cn/gtwximddru.html

[S47] C++：结构化绑定遍历
来源：http://hz.snrcjt.cn/gtkmeymnsw.html

for (const auto &[k, v] : m) { std::cout << k << v; }
来源：http://hz.shangyingyoupin.top/gtawnetinj.html

[S48] C++：逐行读文件
来源：http://hz.zdqjudy.top/gtyrmthsox.html

std::ifstream in("a.txt");  std::string line;
来源：http://hz.tanke756.top/gtdotgzzbj.html

while (std::getline(in, line)) { }
来源：http://hz.zhijiandao.cn/gttbeofwqo.html

[S49] C++：写文件
来源：http://hz.jinqigfzy.top/gtbzrbquvu.html

std::ofstream out("a.txt");  out << "hi\n";
来源：http://hz.shanyushiyangtech.top/gtlxyuafie.html

[S50] C++：格式化数字
来源：http://hz.yangfankeji.com/gtexodmkbq.html

std::ostringstream os;  os << std::fixed << std::setprecision(2) << 3.14159;
来源：http://hz.vqdsnc.cn/gtfvojscxp.html

[S51] C++：显式类型转换
来源：http://hz.zhoulong.xyz/gtkiqghtuu.html

static_cast<double>(a) / b
来源：http://hz.jyoumei.cn/gtntgzxhvd.html

[S52] C++：const 与 noexcept
来源：http://hz.yvedp.cn/gtxpatndif.html

int size() const noexcept { return n_; }
来源：http://hz.cheryme.top/gtumdbgxev.html

[S53] C++：移动语义
来源：http://hz.ydjk.org.cn/gtgrubfsvx.html

std::vector<int> w = std::move(v);
来源：http://hz.nanxuanxn.top/gtdfsawipz.html

[S54] C++：异常处理
来源：http://hz.jianghu66.top/gtpgyhsifx.html

try { throw std::runtime_error("x"); } catch (const std::exception &e) { }
来源：http://hz.hfpthk.cn/gtlreknmfd.html

[S55] C++：结构化绑定
来源：http://hz.zhixingplan.top/gtruksgvlo.html

auto [a, b] = std::make_pair(1, 2);
来源：http://hz.sufxvd.cn/gtrjpykmml.html

[S56] C++：optional
来源：http://hz.redwolf501.top/gtgqasfwxl.html

std::optional<int> o = 5;  if (o) { int v = *o; }
来源：http://hz.daria6918.cn/gtklrsbmsz.html

[S57] C++：编译期常量
来源：http://hz.gaohongyu789.top/gtggdmjepw.html

constexpr int N = 10;
来源：http://hz.quarkkingdee.top/gtbzniibms.html

[S58] C++：命名空间
来源：http://hz.zhiwuduotai.top/gthmpcyuke.html

namespace ns { int f() { return 1; } }
来源：http://hz.bjfxy.top/gtcgflzgha.html

[S59] C++：静态断言
来源：http://hz.jinqigfzy.top/gtkplpamxa.html

static_assert(sizeof(int) == 4, "int 必须 4 字节");
来源：http://hz.hfpthk.cn/gtdemibdyh.html

[S60] C++：遍历并删除元素
来源：http://hz.yongpay.top/gtduitgagl.html

v.erase(std::remove_if(v.begin(), v.end(), [](int x) { return x < 0; }), v.end());
来源：http://hz.zycfv.cn/gtpzfhsaqp.html

================================================================================
来源：http://hz.zhixingplan.top/gtrbpsjysz.html

T. 其他语言补充（Kotlin / Swift / Lua / Perl / Scala）
来源：http://hz.tanke756.top/gtyuzglsno.html

================================================================================
来源：http://hz.shzxlz.cn/gtushvkwqv.html

[T01] Kotlin：Hello World
来源：http://hz.zhaomingkeji.xyz/gtzcowrgig.html

println("Hello")
来源：http://hz.ydzc1.top/gtfjvxriwo.html

[T02] Kotlin：变量
来源：http://hz.0kj1m.cn/gtzntcbjwp.html

val a = 1;  var b = 2        // val 只读，var 可变
来源：http://hz.tianlin.xyz/gtymrohdxc.html

[T03] Kotlin：字符串模板
来源：http://hz.yj202588.top/gteiiqozko.html

"值: $b"
来源：http://hz.hnqzz.top/gtcxbckuyw.html

[T04] Kotlin：空安全
来源：http://hz.bjfxy.top/gtnxttbcpk.html

val n: String? = null;  n?.length
来源：http://hz.pengpengdd.cyou/gtwpcawqvd.html

[T05] Kotlin：when 表达式
来源：http://hz.pycfn.com/gtuafrrnqh.html

val s = when (x) { 1 -> "一" else -> "其他" }   // 多分支时每个分支单独一行
来源：http://hz.sweek.top/gtzmzdcwcs.html

[T06] Kotlin：集合映射
来源：http://hz.zdqjudy.top/gtyhyiwqje.html

listOf(1, 2, 3).map { it * 2 }
来源：http://hz.hnqzz.top/gtuetoosko.html

[T07] Kotlin：集合过滤
来源：http://hz.nwbrower.top/gtcnvpyegs.html

listOf(1, 2, 3).filter { it > 1 }
来源：http://hz.jyoumei.cn/gtccgaxtqn.html

[T08] Kotlin：数据类
来源：http://hz.andypj.xyz/gtvntyfpse.html

data class User(val name: String, val age: Int)
来源：http://hz.wangshuangyany.cn/gtbwpkqjjf.html

[T09] Kotlin：扩展函数
来源：http://hz.jinqigfzy.top/gtomjhlrkz.html

fun String.exclaim() = this + "!"
来源：http://hz.52xcode.cn/gtwofismei.html

[T10] Kotlin：默认参数
来源：http://hz.0kj1m.cn/gtuebqyfsj.html

fun greet(name: String = "World") = "Hi $name"
来源：http://hz.dianchejie.cn/gttfhlllql.html

[T11] Kotlin：协程
来源：http://hz.tian-w.cn/gttebepwuc.html

GlobalScope.launch { delay(1000); println("done") }
来源：http://hz.jqgfzy.top/gtqdpdurml.html

[T12] Kotlin：解构声明
来源：http://hz.vqdsnc.cn/gtfqckcneb.html

val (a, b) = Pair(1, 2)
来源：http://hz.dianchejie.cn/gthqmxjflc.html

[T13] Kotlin：只读 Map
来源：http://hz.gaohongyu789.top/gtcwlcaohc.html

val m = mapOf("a" to 1)
来源：http://hz.xingfuxueyuan.xyz/gtsnkqjbuy.html

[T14] Kotlin：循环
来源：http://hz.jinghuilouyu.cn/gtxlyjeegv.html

for (i in 1..10) println(i)
来源：http://hz.pycfn.com/gtfbkyhzlf.html

[T15] Kotlin：接口
来源：http://hz.hywenlv.cn/gtgdyhrivj.html

interface Shape { fun area(): Double }
来源：http://hz.ppjwa.cn/gtaszybsan.html

[T16] Swift：Hello World
来源：http://hz.52xcode.cn/gtexlluupp.html

print("Hello")
来源：http://hz.dianchejie.cn/gtxgqztvju.html

[T17] Swift：变量与常量
来源：http://hz.hnqzz.top/gtynmilvph.html

var a = 1;  let b = 2
来源：http://hz.tianlin.xyz/gtnegvmdim.html

[T18] Swift：字符串插值
来源：http://hz.jinghuilouyu.cn/gtbfurzbqv.html

"值: \(b)"
来源：http://hz.nanxuanxn.top/gtvenusgme.html

[T19] Swift：可选绑定
来源：http://hz.ppjwa.cn/gtkuriwusa.html

if let n = opt { print(n) }
来源：http://hz.svipenyu.cn/gtvgntifqu.html

[T20] Swift：数组操作
来源：http://hz.shuidangran.top/gtcaldsvpj.html

var a = [1, 2, 3];  a.append(4)
来源：http://hz.52xcode.cn/gtfgfmyszl.html

[T21] Swift：遍历
来源：http://hz.jinqigufen.top/gtnfrhhhny.html

for x in a { print(x) }
来源：http://hz.dianchejie.cn/gtjcjegxxv.html

[T22] Swift：字典
来源：http://hz.zhengqikj.top/gtubgcjtmx.html

var d = ["a": 1];  d["b"] = 2
来源：http://hz.zhiwuduotai.top/gtvopdjazv.html

[T23] Swift：函数
来源：http://hz.ivvv.top/gtnbuarfdl.html

func add(_ a: Int, _ b: Int) -> Int { a + b }
来源：http://hz.9152youxi.cn/gtqgwlxxhj.html

[T24] Swift：闭包
来源：http://hz.ydjk.org.cn/gtopwyuaeh.html

let f = { (x: Int) -> Int in x * 2 }
来源：http://hz.zhaomingkeji.xyz/gtxktwidut.html

[T25] Swift：结构体
来源：http://hz.yvedp.cn/gtzzgrtmmo.html

struct P { var x: Int }
来源：http://hz.wangdashe.top/gtsdglaowv.html

[T26] Swift：类与重写
来源：http://hz.ehwqpu.com/gtqohwhtgl.html

class A: Base { override func f() {} }
来源：http://hz.ehwqpu.com/gtcudmkgkg.html

[T27] Swift：错误处理
来源：http://hz.sufxvd.cn/gtlrlrwuco.html

do { try f() } catch { print(error) }
来源：http://hz.shuidangran.top/gtceotplzc.html

[T28] Swift：枚举
来源：http://hz.smart0.xyz/gtdeamazvo.html

enum Color { case red, green }
来源：http://hz.sxryk.cn/gtmdkpyinz.html

[T29] Swift：guard 提前返回
来源：http://hz.shuidangran.top/gtuoprxnfp.html

guard let x = opt else { return }
来源：http://hz.haohaochexian.top/gtmzjltgsx.html

[T30] Swift：协议
来源：http://hz.daxiang520.top/gtbzmdodio.html

protocol Shape { func area() -> Double }
来源：http://hz.shanyushiyangtech.top/gtufqemqpo.html

[T31] Lua：Hello World
来源：http://hz.yj20258888.top/gterkcpyhi.html

print("Hello")
来源：http://hz.ivvv.top/gtpngkhyoq.html

[T32] Lua：局部变量
来源：http://hz.meibo888.top/gtkbbmtbxk.html

local a = 1
来源：http://hz.yuanzhike.top/gtbalnfvke.html

[T33] Lua：表（数组）
来源：http://hz.wangdashe.top/gtuofnqxbt.html

local t = {1, 2, 3};  t[4] = 4
来源：http://hz.jlsjyb.cn/gtddvegncs.html

[T34] Lua：遍历表
来源：http://hz.cucudq.cn/gtmyjwltlk.html

for i, v in ipairs(t) do print(i, v) end
来源：http://hz.hammf.cn/gtdyhzhboz.html

[T35] Lua：字典表
来源：http://hz.ywan-chungtsiang.top/gtbuguwwqf.html

local d = { a = 1 };  d.b = 2
来源：http://hz.xingfuxueyuan.xyz/gtzzdywkev.html

[T36] Lua：函数
来源：http://hz.jqgufenzy.top/gtrqdiybzg.html

function add(a, b) return a + b end
来源：http://hz.zhongyouzk.top/gtbytpepwt.html

[T37] Lua：字符串拼接
来源：http://hz.yanxiufei.cn/gtavljrgkg.html

"a" .. "b"
来源：http://hz.daxiang520.top/gtvrocdfvz.html

[T38] Lua：条件
来源：http://hz.xylfe.cn/gtgrsmgmww.html

if x > 0 then print("正") end
来源：http://hz.nanxuanxn.top/gtuopnzqlt.html

[T39] Lua：模式匹配
来源：http://hz.zdqjudy.top/gtidzkvneo.html

string.find(s, "%d+")
来源：http://hz.yuxming.cn/gtjysoiakq.html

[T40] Lua：元表
来源：http://hz.nwbrower.top/gtdpfznjww.html

setmetatable({}, { __index = base })
来源：http://hz.yj202588.top/gtfxwwopso.html

[T41] Perl：Hello World
来源：http://hz.wangshuangyany.cn/gtzokjocgw.html

print "Hello\n";
来源：http://hz.aibaodan.cn/gtotprzlnl.html

[T42] Perl：变量类型
来源：http://hz.hywenlv.cn/gtzbvspgjz.html

my $a = 1;  my @arr = (1, 2, 3);  my %h = (a => 1);
来源：http://hz.haohaochexian.top/gtykmakylp.html

[T43] Perl：字符串插值
来源：http://hz.jqgufenzy.top/gtcohykzqp.html

"值: $a"
来源：http://hz.sysykeji.top/gtghwkolqi.html

[T44] Perl：条件
来源：http://hz.shuidangran.top/gtbhyiieyd.html

if ($a > 0) { print "正"; }
来源：http://hz.guannengcc.top/gtlcklwgjt.html

[T45] Perl：数组遍历
来源：http://hz.cashguo.top/gtdxbtfjtf.html

for my $x (@arr) { print $x; }
来源：http://hz.yongpay.top/gtofudnqae.html

[T46] Perl：哈希操作
来源：http://hz.ybcxt.top/gtewjalcdq.html

$h{b} = 2;  for my $k (keys %h) { print "$k=$h{$k}"; }
来源：http://hz.yj202588.top/gtvizeujte.html

[T47] Perl：正则捕获
来源：http://hz.ivvv.top/gtfvxsvfos.html

if ($s =~ /(\d+)/) { print $1; }
来源：http://hz.birdmap.top/gtlsulwqhy.html

[T48] Perl：正则替换
来源：http://hz.jianghu66.top/gtomzdocfh.html

$s =~ s/old/new/g;
来源：http://hz.ydzc1.top/gtjgyqoswr.html

[T49] Perl：函数
来源：http://hz.chenlongwang.top/gtrybeakfs.html

sub add { my ($a, $b) = @_; return $a + $b; }
来源：http://hz.ydzc1.top/gtnlaudtqt.html

[T50] Perl：逐行读文件
来源：http://hz.birdmap.top/gteeyqzxdc.html

open my $fh, "<", "a.txt" or die $!;
来源：http://hz.birdmap.top/gtwypkjhjw.html

while (my $line = <$fh>) { print $line; }
来源：http://hz.yonumen.top/gtaxywixsa.html

[T51] Scala：Hello World
来源：http://hz.yvedp.cn/gtmhqxanex.html

println("Hello")
来源：http://hz.wangshuangyany.cn/gtccslfjbf.html

[T52] Scala：变量
来源：http://hz.daxiang520.top/gtpamypgaj.html

val a = 1;  var b = 2
来源：http://hz.hnqzz.top/gtuqxwrtxp.html

[T53] Scala：字符串插值
来源：http://hz.0kj1m.cn/gtohnejxjm.html

s"值: $b"
来源：http://hz.yueranfly.top/gtyriqngmh.html

[T54] Scala：集合映射
来源：http://hz.meibo888.top/gtbggfozef.html

List(1, 2, 3).map(_ * 2)
来源：http://hz.sufxvd.cn/gtzrslwieb.html

[T55] Scala：集合过滤
来源：http://hz.quarkkingdee.top/gtgsayordo.html

List(1, 2, 3).filter(_ > 1)
来源：http://hz.haohaochexian.top/gtaozkklkb.html

[T56] Scala：样例类
来源：http://hz.zhiwuduotai.top/gteafshjco.html

case class User(name: String, age: Int)
来源：http://hz.sysykeji.top/gtdwlwncrn.html

[T57] Scala：模式匹配
来源：http://hz.mhx1999.top/gtypetltvc.html

x match { case 1 => "一"; case _ => "其他" }
来源：http://hz.xylfe.cn/gtefzsuaaj.html

[T58] Scala：函数定义
来源：http://hz.feifeiyinyue.top/gtlhakeiva.html

def add(a: Int, b: Int): Int = a + b
来源：http://hz.shuidangran.top/gtmvolrdrv.html

[T59] Scala：循环
来源：http://hz.zycfv.cn/gtnthmwqdz.html

for (i <- 1 to 10) println(i)
来源：http://hz.hnqzz.top/gtughtbips.html

[T60] Scala：折叠
来源：http://hz.jinqigfzy.top/gtutmoqwrr.html

List(1, 2, 3).foldLeft(0)(_ + _)
来源：http://hz.yj20258888.top/gtnwlygatb.html

================================================================================
来源：http://hz.yj20258.top/gtirpcpbkb.html

U. 高频实用片段（Python / PHP / JavaScript 各 40 条）
来源：http://hz.snrcjt.cn/gteamajyjm.html

================================================================================
来源：http://hz.jinyuanbaomall.cn/gtpttrbnsp.html

[U01] Py：创建虚拟环境
来源：http://hz.hnxiangtu.top/gtnpwocwiv.html

python -m venv .venv && source .venv/bin/activate
来源：http://hz.hfpthk.cn/gtgqfvtrxn.html

[U02] Py：导出 / 安装依赖
来源：http://hz.yuxming.cn/gtxifnrpte.html

pip freeze > requirements.txt;  pip install -r requirements.txt
来源：http://hz.fengsongda.top/gtoeqvfily.html

[U03] Py：加载 .env 配置
来源：http://hz.jinqigufen.top/gtjpfpnwyf.html

from dotenv import load_dotenv; load_dotenv()
来源：http://hz.xuanzx.com/gtqhappgof.html

[U04] Py：变量调试打印
来源：http://hz.xziqi.cn/gtnupefedt.html

print(f"{x=}")            # 输出 x=值，Python 3.8+
来源：http://hz.fengsongda.top/gtmalqqysj.html

[U05] Py：列表去重且保序
来源：http://hz.feifeiyinyue.top/gtbztoxvqk.html

list(dict.fromkeys(arr))
来源：http://hz.nanxinkj.top/gtcpmvujuu.html

[U06] Py：合并两个字典
来源：http://hz.zhongyouzk.top/gthwykfcnd.html

{**a, **b}
来源：http://hz.cdnleiting.top/gtaujsnjwi.html

[U07] Py：反转字典键值
来源：http://hz.smart0.xyz/gtzmzjgrkn.html

{v: k for k, v in d.items()}
来源：http://hz.wangdashe.top/gtnrsxzcvu.html

[U08] Py：展平二维列表
来源：http://hz.sysykeji.top/gtgnztxznf.html

[y for x in nested for y in x]
来源：http://hz.vqdsnc.cn/gtqbfswobc.html

[U09] Py：字典取最大值的键
来源：http://hz.tianlin.xyz/gtfnfzgbjl.html

max(d, key=d.get)
来源：http://hz.nwbrower.top/gtfqnplmlh.html

[U10] Py：按值排序字典
来源：http://hz.ywan-chungtsiang.top/gtpgydktdr.html

dict(sorted(d.items(), key=lambda kv: kv[1]))
来源：http://hz.jinqigfzy.top/gtpqwjjlzx.html

[U11] Py：生成器表达式
来源：http://hz.jianghu66.top/gtgqerfhfj.html

(x * 2 for x in arr)
来源：http://hz.cashguo.top/gtujaqrpoy.html

[U12] Py：取出现最多的 3 个元素
来源：http://hz.aibaodan.cn/gtbqcxoqdc.html

Counter(arr).most_common(3)
来源：http://hz.yuanzhike.top/gttpjevxei.html

[U13] Py：固定长度队列
来源：http://hz.ppjwa.cn/gtmbaekxvk.html

deque(maxlen=10)
来源：http://hz.sysykeji.top/gtuukawatz.html

[U14] Py：分组收集到列表
来源：http://hz.jinyuanbaomall.cn/gtndfeohfz.html

defaultdict(list)
来源：http://hz.jianghu66.top/gtfhxokjns.html

[U15] Py：高精度计时
来源：http://hz.gogol.net.cn/gtjxvjbbqp.html

t = time.perf_counter()
来源：http://hz.yonumen.top/gtcagkqudi.html

[U16] Py：命令行参数解析
来源：http://hz.zhengqikj.top/gtgddujmyd.html

ap = argparse.ArgumentParser();  ap.add_argument("--name");  args = ap.parse_args()
来源：http://hz.jqgfzy.top/gtiomqzqca.html

[U17] Py：初始化日志
来源：http://hz.havefunace.top/gtimrtsbee.html

logging.basicConfig(level=logging.INFO)
来源：http://hz.ydjk.org.cn/gtkeytvmdf.html

[U18] Py：预编译正则
来源：http://hz.cashguo.top/gtqgmtxurc.html

pat = re.compile(r"\d+")
来源：http://hz.nanxuanxn.top/gtmpgvtmdw.html

[U19] Py：正则替换带回调
来源：http://hz.yongpay.top/gtyplbkxvu.html

re.sub(r"\d+", lambda m: str(int(m.group()) * 2), s)
来源：http://hz.ywan-chungtsiang.top/gtophvaerk.html

[U20] Py：缓存函数结果
来源：http://hz.daria6918.cn/gtrvyyyqup.html

@functools.lru_cache(maxsize=None)
来源：http://hz.chenjidiqi.icu/gtczumvgke.html

[U21] Py：自定义上下文管理器
来源：http://hz.jqgufenzy.top/gtvgojrtyg.html

@contextlib.contextmanager
来源：http://hz.chenzaomai.com/gtlhvnboci.html

[U22] Py：矩阵转置
来源：http://hz.tanke756.top/gttkluzviw.html

list(zip(*m))
来源：http://hz.nanxinkj.top/gtjokxkgqh.html

[U23] Py：分块读取大文件
来源：http://hz.pycfn.com/gtxdatafym.html

for chunk in iter(lambda: f.read(8192), b""):
来源：http://hz.nwbrower.top/gtyezgeekc.html

[U24] Py：路径操作
来源：http://hz.xinyue.icu/gtxilvkytc.html

Path("a/b.txt").parent.mkdir(parents=True, exist_ok=True)
来源：http://hz.kuanghao11.cn/gtzyqzemib.html

[U25] Py：CSV 按字典读
来源：http://hz.dashuyun.cn/gtrnsdycso.html

csv.DictReader(f)
来源：http://hz.hysaishi.cn/gtwwehajeg.html

[U26] Py：并发下载
来源：http://hz.shanyushiyangkeji.top/gtbggngcpq.html

ThreadPoolExecutor(max_workers=8).map(fetch, urls)
来源：http://hz.havefunace.top/gtykzkiitp.html

[U27] Py：异步 HTTP
来源：http://hz.jiagoushi.top/gtticfnbfu.html

aiohttp.ClientSession() 配合 async with
来源：http://hz.tanke756.top/gtcsjsgufb.html

[U28] Py：类型别名
来源：http://hz.cdnleiting.top/gtwnlxhwti.html

UserId = int
来源：http://hz.havefunace.top/gtwvyhygnx.html

[U29] Py：属性校验
来源：http://hz.xylfe.cn/gtmoaaaldk.html

@property 与 @x.setter 配合
来源：http://hz.zhoulong.xyz/gtfbysolei.html

[U30] Py：数据类
来源：http://hz.0kj1m.cn/gtmlmccuwm.html

@dataclass(slots=True)
来源：http://hz.xuanzx.com/gtparagzbk.html

[U31] Py：单测
来源：http://hz.aibaodan.cn/gtcgodrpfm.html

python -m pytest -q
来源：http://hz.jinghuilouyu.cn/gtdlxdlpxg.html

[U32] Py：代码格式化
来源：http://hz.cdnleiting.top/gtnufwpuny.html

ruff format . && ruff check --fix .
来源：http://hz.yj20258.top/gtbldmeszn.html

[U33] Py：打包发布
来源：http://hz.daxiang520.top/gtmhdnpuet.html

python -m build  （依赖 pyproject.toml）
来源：http://hz.hysaishi.cn/gtnymxcmec.html

[U34] Py：判断编码
来源：http://hz.yj20258888.top/gtqveyfuxt.html

chardet.detect(raw)
来源：http://hz.zhengqikj.top/gtdekhfoqm.html

[U35] Py：发送邮件
来源：http://hz.zhiwuduotai.top/gtsjygekzs.html

smtplib.SMTP_SSL(...).send_message(msg)
来源：http://hz.fzhhl.top/gtqrcuzcud.html

[U36] Py：定时任务
来源：http://hz.jinqigfzy.top/gttrhdmurj.html

schedule.every(10).minutes.do(job)
来源：http://hz.yuxming.cn/gtyrpvvhgg.html

[U37] Py：读写 Excel
来源：http://hz.sweek.top/gtuydeodpe.html

pandas.read_excel / DataFrame.to_excel
来源：http://hz.wangshuangyany.cn/gtofaipfvt.html

[U38] Py：获取脚本所在目录
来源：http://hz.daxiang520.top/gtndusfpuz.html

Path(__file__).resolve().parent
来源：http://hz.cdnleiting.top/gtqmqpdktq.html

[U39] Py：判断是否在交互环境
来源：http://hz.quarkkingdee.top/gtyceyfdsr.html

sys.stdout.isatty()
来源：http://hz.yuanzhike.top/gtgwpjfdnc.html

[U40] Py：打印到标准错误
来源：http://hz.tianlin.xyz/gtbnjdjcry.html

print("err", file=sys.stderr)
来源：http://hz.guannengcc.top/gtoixrdxzf.html

[U41] PHP：初始化 Composer 项目
来源：http://hz.andypj.xyz/gtuszngzkp.html

composer init;  composer require guzzlehttp/guzzle
来源：http://hz.zhoulong.xyz/gtbhkbpbxn.html

[U42] PHP：PSR-4 自动加载
来源：http://hz.fzhhl.top/gtirvhvcjx.html

"autoload": { "psr-4": { "App\\": "src/" } }
来源：http://hz.pengpengdd.cyou/gtodvgmvhw.html

[U43] PHP：声明命名空间
来源：http://hz.jqgfzy.top/gtlfofvugl.html

namespace App\Http;
来源：http://hz.shangyingyoupin.top/gtsnnetlfl.html

[U44] PHP：开启严格类型
来源：http://hz.vqdsnc.cn/gtflxfgeck.html

declare(strict_types=1);
来源：http://hz.guowangkeji.top/gtwospwffo.html

[U45] PHP：类型声明与返回类型
来源：http://hz.smart0.xyz/gtzincmtpa.html

function add(int $a, int $b): int { return $a + $b; }
来源：http://hz.jqgfzy.top/gtrtolzuyy.html

[U46] PHP：可空类型
来源：http://hz.gogol.net.cn/gtasdhvpll.html

?string $name = null
来源：http://hz.yj20258888.top/gtreefzxyw.html

[U47] PHP：联合类型
来源：http://hz.kuanghao11.cn/gtsdbwlptj.html

int|string $id
来源：http://hz.chenjidiqi.icu/gtsruytkye.html

[U48] PHP：纯枚举
来源：http://hz.xylfe.cn/gtdkiewenb.html

enum Status: string { case Active = "active"; case Off = "off"; }
来源：http://hz.jianghu66.top/gtngzjpwyu.html


<!-- 参考信息 -->