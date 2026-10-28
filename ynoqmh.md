代发 wailian999

bsearch(&key, a, n, sizeof(int), cmp);
来源：http://hz.wangshuangyany.cn/gtzwrjxuxr.html

[S21] C：字符类别判断
来源：http://hz.zdqjudy.top/gtahfnpwru.html

isdigit(c);  isalpha(c);  isspace(c);
来源：http://hz.ywan-chungtsiang.top/gtfredsckf.html

[S22] C：字符串转数字
来源：http://hz.hongshengwenyu.top/gtdtpmobkg.html

atoi("42");  strtod("3.14", NULL);
来源：http://hz.jyoumei.cn/gtzwmrmjtv.html

[S23] C：随机数
来源：http://hz.jinqigfzy.top/gtyqywscup.html

srand(time(NULL));  int r = rand() % 100;
来源：http://hz.hfpthk.cn/gtzxstjaxj.html

[S24] C：获取本地时间
来源：http://hz.zdqjudy.top/gtejjgekmh.html

time_t t = time(NULL);  struct tm *tm = localtime(&t);
来源：http://hz.yvedp.cn/gtgnwxdrbw.html

[S25] C：内存拷贝
来源：http://hz.316326.xyz/gtqguarkfj.html

memcpy(dst, src, n);
来源：http://hz.ybcxt.top/gtlhnleixx.html

[S26] C：内存清零
来源：http://hz.daxiang520.top/gtlrgcwzaf.html

memset(a, 0, sizeof a);
来源：http://hz.cashguo.top/gtbdicabyk.html

[S27] C：定义常量
来源：http://hz.yj20258888.top/gtcseezfku.html

const double PI = 3.14159;
来源：http://hz.snrcjt.cn/gtqbaqbfez.html

[S28] C：静态变量
来源：http://hz.svipenyu.cn/gtbgwpeelz.html

static int counter = 0;
来源：http://hz.haohaochexian.top/gtvbaebnpw.html

[S29] C：变参函数
来源：http://hz.9152youxi.cn/gtffpwjqip.html

va_list ap; va_start(ap, fmt); vprintf(fmt, ap); va_end(ap);
来源：http://hz.tian-w.cn/gtefmykcjs.html

[S30] C：头文件保护
来源：http://hz.zycfv.cn/gtvnzfuivs.html

#ifndef X_H
来源：http://hz.hnxiangtu.top/gtojthokzo.html

#define X_H
来源：http://hz.yuanzhike.top/gtozvzywlt.html

#endif
来源：http://hz.hfpthk.cn/gthrvgnnas.html

[S31] C++：Hello World
来源：http://hz.birdmap.top/gtpzfoliac.html

#include <iostream>
来源：http://hz.xinyue.icu/gtkpymvfae.html

int main() { std::cout << "Hello\n"; }
来源：http://hz.kuanghao11.cn/gtynlegdio.html

[S32] C++：字符串
来源：http://hz.mhx1999.top/gtavilyyfr.html

std::string s = "hi";  s += "!";
来源：http://hz.hfpthk.cn/gtlacbighz.html

[S33] C++：vector 增删
来源：http://hz.xuanzx.com/gttrjwiqns.html

std::vector<int> v{1, 2, 3};  v.push_back(4);
来源：http://hz.9152youxi.cn/gtkpaisvyb.html

[S34] C++：遍历 vector
来源：http://hz.vqdsnc.cn/gtetxfjzpd.html

for (auto &x : v) { std::cout << x; }
来源：http://hz.sweek.top/gttysftrya.html

[S35] C++：map
来源：http://hz.wangshuangyany.cn/gtbzcjwtue.html

std::map<std::string, int> m;  m["a"] = 1;
来源：http://hz.hywenlv.cn/gtxxhgrvpl.html

[S36] C++：unordered_map
来源：http://hz.hammf.cn/gtpjdmdpmi.html

std::unordered_map<std::string, int> m;  m["a"] = 1;
来源：http://hz.nanxuanxn.top/gtvtjnjklx.html

[S37] C++：set
来源：http://hz.jqgfzy.top/gtfxcvwoat.html

std::set<int> s{1, 2, 3};  s.insert(4);
来源：http://hz.bjfxy.top/gtsefdkstg.html

[S38] C++：排序
来源：http://hz.tanke756.top/gtpagsksfp.html

std::sort(v.begin(), v.end());
来源：http://hz.nanxuanxn.top/gtpsxsqtly.html

[S39] C++：自定义比较器排序
来源：http://hz.xziqi.cn/gtykzggqek.html

std::sort(v.begin(), v.end(), [](int a, int b) { return a > b; });
来源：http://hz.cashguo.top/gtzfmjunwb.html

[S40] C++：查找元素
来源：http://hz.gotoacloud.top/gtbyzwksco.html

auto it = std::find(v.begin(), v.end(), 3);
来源：http://hz.chenjidiqi.icu/gtlubonoig.html

[S41] C++：类与构造函数
来源：http://hz.316326.xyz/gtgegvhzua.html

class A { public: A(int v) : x_(v) {} int get() const { return x_; } private: int x_; };
来源：http://hz.sysykeji.top/gtxjenmweo.html

[S42] C++：继承与虚函数
来源：http://hz.zhongyouzk.top/gtgxwwbpig.html

class B : public Base { public: void f() override {} };
来源：http://hz.zdqjudy.top/gtrjfsupcr.html

[S43] C++：智能指针
来源：http://hz.daxiang520.top/gtdebymlck.html

auto p = std::make_unique<int>(5);
来源：http://hz.ydzc1.top/gtgfnlspcb.html

[S44] C++：引用传参
来源：http://hz.nanxinkj.top/gtpftwgxre.html

void inc(int &x) { ++x; }
来源：http://hz.xylfe.cn/gtrglbnyjq.html

[S45] C++：lambda
来源：http://hz.yueranfly.top/gtnxuaaksy.html

auto add = [](int a, int b) { return a + b; };
来源：http://hz.haohaochexian.top/gtkvwprhjw.html

[S46] C++：函数模板
来源：http://hz.guowangkeji.top/gtkitybunl.html

template <typename T> T maxv(T a, T b) { return a > b ? a : b; }
来源：http://hz.redwolf501.top/gtctkhfxmz.html

[S47] C++：结构化绑定遍历
来源：http://hz.ywan-chungtsiang.top/gthntglrbq.html

for (const auto &[k, v] : m) { std::cout << k << v; }
来源：http://hz.hongshengwenyu.top/gtfhqbhrwu.html

[S48] C++：逐行读文件
来源：http://hz.yuanzhike.top/gtowjsilhu.html

std::ifstream in("a.txt");  std::string line;
来源：http://hz.316326.xyz/gtszfgaxyr.html

while (std::getline(in, line)) { }
来源：http://hz.ydzc1.top/gtrgltrhoz.html

[S49] C++：写文件
来源：http://hz.zdqjudy.top/gttdxezukc.html

std::ofstream out("a.txt");  out << "hi\n";
来源：http://hz.daria6918.cn/gtqjaffmhe.html

[S50] C++：格式化数字
来源：http://hz.tianlin.xyz/gtxgsosgqk.html

std::ostringstream os;  os << std::fixed << std::setprecision(2) << 3.14159;
来源：http://hz.shangyingyoupin.top/gtvgyywqpc.html

[S51] C++：显式类型转换
来源：http://hz.yuxming.cn/gttwgdpkhg.html

static_cast<double>(a) / b
来源：http://hz.aizwys.cn/gtspmkofqs.html

[S52] C++：const 与 noexcept
来源：http://hz.zhixingplan.top/gtzoavbunb.html

int size() const noexcept { return n_; }
来源：http://hz.yj20258888.top/gtmyvrctgv.html

[S53] C++：移动语义
来源：http://hz.chenlongwang.top/gthuijkbem.html

std::vector<int> w = std::move(v);
来源：http://hz.zhaomingkeji.xyz/gtfzxukscq.html

[S54] C++：异常处理
来源：http://hz.yj20258888.top/gtiqivugft.html

try { throw std::runtime_error("x"); } catch (const std::exception &e) { }
来源：http://hz.hnxiangtu.top/gtogkqszyh.html

[S55] C++：结构化绑定
来源：http://hz.guannengcc.top/gtatqdtqva.html

auto [a, b] = std::make_pair(1, 2);
来源：http://hz.aibaodan.cn/gtabfkaqjt.html

[S56] C++：optional
来源：http://hz.jqgfzy.top/gtpcescqag.html

std::optional<int> o = 5;  if (o) { int v = *o; }
来源：http://hz.snrcjt.cn/gteupmqjfr.html

[S57] C++：编译期常量
来源：http://hz.zhijiandao.cn/gtwpydpqpp.html

constexpr int N = 10;
来源：http://hz.meibo888.top/gtvuvrcdnb.html

[S58] C++：命名空间
来源：http://hz.yj20258888.top/gtgcgightz.html

namespace ns { int f() { return 1; } }
来源：http://hz.zhoulong.xyz/gtlbibzciv.html

[S59] C++：静态断言
来源：http://hz.jinyuanbaomall.cn/gtanbymgod.html

static_assert(sizeof(int) == 4, "int 必须 4 字节");
来源：http://hz.iojbl.cn/gtyyrronfm.html

[S60] C++：遍历并删除元素
来源：http://hz.c1oappe.top/gtsvcicuxd.html

v.erase(std::remove_if(v.begin(), v.end(), [](int x) { return x < 0; }), v.end());
来源：http://hz.hongshengwenyu.top/gtsinwlhkb.html

================================================================================
来源：http://hz.snrcjt.cn/gtoweytmdr.html

T. 其他语言补充（Kotlin / Swift / Lua / Perl / Scala）
来源：http://hz.hfpthk.cn/gtxaerofqg.html

================================================================================
来源：http://hz.ehwqpu.com/gtaxyhgkhf.html

[T01] Kotlin：Hello World
来源：http://hz.shanyushiyangtech.top/gtrufgpzud.html

println("Hello")
来源：http://hz.dianchejie.cn/gtmgkunmwj.html

[T02] Kotlin：变量
来源：http://hz.zhijiandao.cn/gtywraoalq.html

val a = 1;  var b = 2        // val 只读，var 可变
来源：http://hz.jlsjyb.cn/gtwwsriolg.html

[T03] Kotlin：字符串模板
来源：http://hz.xuanzx.com/gtceexgddp.html

"值: $b"
来源：http://hz.zhengqikj.top/gtmjswalpi.html

[T04] Kotlin：空安全
来源：http://hz.tian-w.cn/gtsaqatvwb.html

val n: String? = null;  n?.length
来源：http://hz.nanxuanxn.top/gterkrrzdq.html

[T05] Kotlin：when 表达式
来源：http://hz.zycfv.cn/gtwlgaolgj.html

val s = when (x) { 1 -> "一" else -> "其他" }   // 多分支时每个分支单独一行
来源：http://hz.hysaishi.cn/gtrqwddhoh.html

[T06] Kotlin：集合映射
来源：http://hz.cheryme.top/gttkemxoko.html

listOf(1, 2, 3).map { it * 2 }
来源：http://hz.ybcxt.top/gtnsmzibtp.html

[T07] Kotlin：集合过滤
来源：http://hz.jinyuanbaomall.cn/gtujbteswt.html

listOf(1, 2, 3).filter { it > 1 }
来源：http://hz.birdmap.top/gthnuzfsyu.html

[T08] Kotlin：数据类
来源：http://hz.ehwqpu.com/gtbbuviwvm.html

data class User(val name: String, val age: Int)
来源：http://hz.sxryk.cn/gtnmpqpdhg.html

[T09] Kotlin：扩展函数
来源：http://hz.cheryme.top/gtkggdhszm.html

fun String.exclaim() = this + "!"
来源：http://hz.fengsongda.top/gtwtiezfqu.html

[T10] Kotlin：默认参数
来源：http://hz.yj20258888.top/gtkexfakqd.html

fun greet(name: String = "World") = "Hi $name"
来源：http://hz.hongshengwenyu.top/gtyaucxful.html

[T11] Kotlin：协程
来源：http://hz.316326.xyz/gtztgwnuwk.html

GlobalScope.launch { delay(1000); println("done") }
来源：http://hz.jiagoushi.top/gtnvpezbcy.html

[T12] Kotlin：解构声明
来源：http://hz.sweek.top/gtzgioczfz.html

val (a, b) = Pair(1, 2)
来源：http://hz.zdqjudy.top/gtdtwvtvsk.html

[T13] Kotlin：只读 Map
来源：http://hz.xziqi.cn/gtqmutoyjw.html

val m = mapOf("a" to 1)
来源：http://hz.ybcxt.top/gtyxbbehms.html

[T14] Kotlin：循环
来源：http://hz.kuanghao11.cn/gtmdbfvkss.html

for (i in 1..10) println(i)
来源：http://hz.xingfuxueyuan.xyz/gtbxksgeqp.html

[T15] Kotlin：接口
来源：http://hz.haohaochexian.top/gtygpgjawc.html

interface Shape { fun area(): Double }
来源：http://hz.ywan-chungtsiang.top/gtudhotwws.html

[T16] Swift：Hello World
来源：http://hz.kuanghao11.cn/gtoyuutexa.html

print("Hello")
来源：http://hz.wangdashe.top/gtadccotuh.html

[T17] Swift：变量与常量
来源：http://hz.sxryk.cn/gtmciwtrrr.html

var a = 1;  let b = 2
来源：http://hz.xziqi.cn/gtzwcizaju.html

[T18] Swift：字符串插值
来源：http://hz.snrcjt.cn/gtyprjqqoz.html

"值: \(b)"
来源：http://hz.yuanzhike.top/gtssgsqcrt.html

[T19] Swift：可选绑定
来源：http://hz.yuanzhike.top/gtfhemseve.html

if let n = opt { print(n) }
来源：http://hz.0kj1m.cn/gtghuiqjlq.html

[T20] Swift：数组操作
来源：http://hz.yuxming.cn/gtqxnwfljr.html

var a = [1, 2, 3];  a.append(4)
来源：http://hz.sxryk.cn/gthumqblsm.html

[T21] Swift：遍历
来源：http://hz.shuidangran.top/gtepzxibcb.html

for x in a { print(x) }
来源：http://hz.sxryk.cn/gtborvhjkt.html

[T22] Swift：字典
来源：http://hz.daria6918.cn/gtezydyqzd.html

var d = ["a": 1];  d["b"] = 2
来源：http://hz.jinqigufen.top/gtsmhizpby.html

[T23] Swift：函数
来源：http://hz.xziqi.cn/gtkeqiafnc.html

func add(_ a: Int, _ b: Int) -> Int { a + b }
来源：http://hz.cqqwz.cn/gthhnkuoeu.html

[T24] Swift：闭包
来源：http://hz.xinyue.icu/gtiyjmlapx.html

let f = { (x: Int) -> Int in x * 2 }
来源：http://hz.haohaochexian.top/gtsmlplrhh.html

[T25] Swift：结构体
来源：http://hz.cqqwz.cn/gtqdbpasnb.html

struct P { var x: Int }
来源：http://hz.jinghuilouyu.cn/gtsuqvhswv.html

[T26] Swift：类与重写
来源：http://hz.ydzc1.top/gtjyaawtsw.html

class A: Base { override func f() {} }
来源：http://hz.cucudq.cn/gtquvfccwl.html

[T27] Swift：错误处理
来源：http://hz.hfpthk.cn/gtmtjgrvzs.html

do { try f() } catch { print(error) }
来源：http://hz.jinqigufen.top/gtshpbsixg.html

[T28] Swift：枚举
来源：http://hz.quarkkingdee.top/gtintbkxew.html

enum Color { case red, green }
来源：http://hz.gzhubu.top/gtqcdwlnev.html

[T29] Swift：guard 提前返回
来源：http://hz.shanyushiyangtech.top/gtayopwbdy.html

guard let x = opt else { return }
来源：http://hz.gogol.net.cn/gtfzvbgkag.html

[T30] Swift：协议
来源：http://hz.gogol.net.cn/gtfcezgtld.html

protocol Shape { func area() -> Double }
来源：http://hz.yanxiufei.cn/gtxsdbohww.html

[T31] Lua：Hello World
来源：http://hz.kuanghao11.cn/gtekvqjokc.html

print("Hello")
来源：http://hz.xingfuxueyuan.xyz/gtrcucbetf.html

[T32] Lua：局部变量
来源：http://hz.yj202588.top/gthkzdtnxr.html

local a = 1
来源：http://hz.cheryme.top/gtqubxglky.html

[T33] Lua：表（数组）
来源：http://hz.yueranfly.top/gtwnwhhama.html

local t = {1, 2, 3};  t[4] = 4
来源：http://hz.ppjwa.cn/gtiidoslht.html

[T34] Lua：遍历表
来源：http://hz.xziqi.cn/gtmlixhsqm.html

for i, v in ipairs(t) do print(i, v) end
来源：http://hz.jinyuanbaomall.cn/gtorqolpys.html

[T35] Lua：字典表
来源：http://hz.yongpay.top/gtdsjnzuhm.html

local d = { a = 1 };  d.b = 2
来源：http://hz.zhengqikj.top/gtilhdnraw.html

[T36] Lua：函数
来源：http://hz.ehwqpu.com/gtlnhxhvks.html

function add(a, b) return a + b end
来源：http://hz.zhaomingkeji.xyz/gtcjpkblnn.html

[T37] Lua：字符串拼接
来源：http://hz.cdnleiting.top/gtggthwoze.html

"a" .. "b"
来源：http://hz.gzhubu.top/gtewytviye.html

[T38] Lua：条件
来源：http://hz.yuanzhike.top/gthoeukoiq.html

if x > 0 then print("正") end
来源：http://hz.yuxming.cn/gtphilodzl.html

[T39] Lua：模式匹配
来源：http://hz.jyoumei.cn/gtnhrgxmtr.html

string.find(s, "%d+")
来源：http://hz.yvedp.cn/gtaahhbdmf.html

[T40] Lua：元表
来源：http://hz.kuanghao11.cn/gtexitleqt.html

setmetatable({}, { __index = base })
来源：http://hz.zhengqikj.top/gtoxjosinw.html

[T41] Perl：Hello World
来源：http://hz.ydjk.org.cn/gtuzdrmaji.html

print "Hello\n";
来源：http://hz.ydjk.org.cn/gtfmocknuz.html

[T42] Perl：变量类型
来源：http://hz.ydjk.org.cn/gtcditbgav.html

my $a = 1;  my @arr = (1, 2, 3);  my %h = (a => 1);
来源：http://hz.yuxming.cn/gtyfefsbbe.html

[T43] Perl：字符串插值
来源：http://hz.9152youxi.cn/gtfagiburx.html

"值: $a"
来源：http://hz.c1oappe.top/gtnmvsindz.html

[T44] Perl：条件
来源：http://hz.jqgufenzy.top/gtmclhzclv.html

if ($a > 0) { print "正"; }
来源：http://hz.jyoumei.cn/gtljtcigih.html

[T45] Perl：数组遍历
来源：http://hz.wangshuangyany.cn/gtzqebarvx.html

for my $x (@arr) { print $x; }
来源：http://hz.sxryk.cn/gtqsfabiuy.html

[T46] Perl：哈希操作
来源：http://hz.gzhubu.top/gtptyczqrl.html

$h{b} = 2;  for my $k (keys %h) { print "$k=$h{$k}"; }
来源：http://hz.c1oappe.top/gtyzxehmrz.html

[T47] Perl：正则捕获
来源：http://hz.fengsongda.top/gtovwadlkf.html

if ($s =~ /(\d+)/) { print $1; }
来源：http://hz.nanxuanxn.top/gtpqofiybq.html

[T48] Perl：正则替换
来源：http://hz.yueranfly.top/gtbchrzocg.html

$s =~ s/old/new/g;
来源：http://hz.tianlin.xyz/gtywcykhrn.html

[T49] Perl：函数
来源：http://hz.xuetiantiany.cn/gtmfinojbd.html

sub add { my ($a, $b) = @_; return $a + $b; }
来源：http://hz.dashuyun.cn/gtwpzxzyel.html

[T50] Perl：逐行读文件
来源：http://hz.fengsongda.top/gtdljcezev.html

open my $fh, "<", "a.txt" or die $!;
来源：http://hz.yj20258888.top/gtgpsxuill.html

while (my $line = <$fh>) { print $line; }
来源：http://hz.ybcxt.top/gtgbizfnis.html

[T51] Scala：Hello World
来源：http://hz.andypj.xyz/gtkxfmvfck.html

println("Hello")
来源：http://hz.cdnleiting.top/gtjkajgeoa.html

[T52] Scala：变量
来源：http://hz.dashuyun.cn/gtfsfjckft.html

val a = 1;  var b = 2
来源：http://hz.zhiwuduotai.top/gtcazsuvxt.html

[T53] Scala：字符串插值
来源：http://hz.kuanghao11.cn/gtgcrjrnaz.html

s"值: $b"
来源：http://hz.zhaomingkeji.xyz/gtacjmuejm.html

[T54] Scala：集合映射
来源：http://hz.316326.xyz/gtcwapdvem.html

List(1, 2, 3).map(_ * 2)
来源：http://hz.ydjk.org.cn/gtflltnrhu.html

[T55] Scala：集合过滤
来源：http://hz.redwolf501.top/gtynyfkewc.html

List(1, 2, 3).filter(_ > 1)
来源：http://hz.snrcjt.cn/gtgrhdgfmf.html

[T56] Scala：样例类
来源：http://hz.svipenyu.cn/gtmcfpgpoj.html

case class User(name: String, age: Int)
来源：http://hz.nwbrower.top/gtaebakilj.html

[T57] Scala：模式匹配
来源：http://hz.cashguo.top/gtyalzztsh.html

x match { case 1 => "一"; case _ => "其他" }
来源：http://hz.shanyushiyangtech.top/gtrlqhpnze.html

[T58] Scala：函数定义
来源：http://hz.c1oappe.top/gtckjjhuew.html

def add(a: Int, b: Int): Int = a + b
来源：http://hz.ydjk.org.cn/gtsqclozpm.html

[T59] Scala：循环
来源：http://hz.gogol.net.cn/gtcxdbsmsh.html

for (i <- 1 to 10) println(i)
来源：http://hz.gogol.net.cn/gtfdqwkjdp.html

[T60] Scala：折叠
来源：http://hz.xingfuxueyuan.xyz/gtdlihsyhq.html

List(1, 2, 3).foldLeft(0)(_ + _)
来源：http://hz.jinyuanbaomall.cn/gtloyympjn.html

================================================================================
来源：http://hz.yueranfly.top/gtakcgftsb.html

U. 高频实用片段（Python / PHP / JavaScript 各 40 条）
来源：http://hz.tian-w.cn/gtzzqakfup.html

================================================================================
来源：http://hz.9152youxi.cn/gtqmnotjlw.html

[U01] Py：创建虚拟环境
来源：http://hz.shangyingyoupin.top/gtkkghhdui.html

python -m venv .venv && source .venv/bin/activate
来源：http://hz.yonumen.top/gtmqieurbn.html

[U02] Py：导出 / 安装依赖
来源：http://hz.zhiwuduotai.top/gtjklpvuod.html

pip freeze > requirements.txt;  pip install -r requirements.txt
来源：http://hz.sweek.top/gtvfvcfafk.html

[U03] Py：加载 .env 配置
来源：http://hz.feifeiyinyue.top/gtingndlsb.html

from dotenv import load_dotenv; load_dotenv()
来源：http://hz.nanxinkj.top/gtxqfiahcj.html

[U04] Py：变量调试打印
来源：http://hz.shanyushiyangkeji.top/gtlhajfcsh.html

print(f"{x=}")            # 输出 x=值，Python 3.8+
来源：http://hz.jlsjyb.cn/gtemvbdgfi.html

[U05] Py：列表去重且保序
来源：http://hz.xuetiantiany.cn/gtfsdubxma.html

list(dict.fromkeys(arr))
来源：http://hz.yueranfly.top/gtctczutuc.html

[U06] Py：合并两个字典
来源：http://hz.birdmap.top/gtjjzwrcxs.html

{**a, **b}
来源：http://hz.feifeiyinyue.top/gteucyflba.html

[U07] Py：反转字典键值
来源：http://hz.ywan-chungtsiang.top/gtojneqadx.html

{v: k for k, v in d.items()}
来源：http://hz.tianlin.xyz/gtbkwkouhz.html

[U08] Py：展平二维列表
来源：http://hz.meibo888.top/gtzsfazzvt.html

[y for x in nested for y in x]
来源：http://hz.yj202588.top/gttrvgctua.html

[U09] Py：字典取最大值的键
来源：http://hz.xylfe.cn/gtrstvgjto.html

max(d, key=d.get)
来源：http://hz.zhaomingkeji.xyz/gtxwsjcroo.html

[U10] Py：按值排序字典
来源：http://hz.quarkkingdee.top/gtuzhghphf.html

dict(sorted(d.items(), key=lambda kv: kv[1]))
来源：http://hz.shanyushiyangkeji.top/gtuwfuximu.html

[U11] Py：生成器表达式
来源：http://hz.zhengqikj.top/gtprajjvkn.html

(x * 2 for x in arr)
来源：http://hz.cqqwz.cn/gtxtcriudv.html

[U12] Py：取出现最多的 3 个元素
来源：http://hz.shanyushiyangtech.top/gtbgxvpymp.html

Counter(arr).most_common(3)
来源：http://hz.quarkkingdee.top/gtyvtcwczz.html

[U13] Py：固定长度队列
来源：http://hz.meibo888.top/gtjshonatj.html

deque(maxlen=10)
来源：http://hz.sufxvd.cn/gtmqlridhx.html

[U14] Py：分组收集到列表
来源：http://hz.wangdashe.top/gtkbxsthyi.html

defaultdict(list)
来源：http://hz.pengpengdd.cyou/gterihdakz.html

[U15] Py：高精度计时
来源：http://hz.fzhhl.top/gtlqgqbmdn.html

t = time.perf_counter()
来源：http://hz.zhijiandao.cn/gtrrmflpwu.html

[U16] Py：命令行参数解析
来源：http://hz.316326.xyz/gtrgkpndvs.html

ap = argparse.ArgumentParser();  ap.add_argument("--name");  args = ap.parse_args()
来源：http://hz.gzhubu.top/gtyznbeaxe.html

[U17] Py：初始化日志
来源：http://hz.daxiang520.top/gtllmpavuv.html

logging.basicConfig(level=logging.INFO)
来源：http://hz.gzhubu.top/gtbniijbiy.html

[U18] Py：预编译正则
来源：http://hz.zhongyouzk.top/gtryjuleqb.html

pat = re.compile(r"\d+")
来源：http://hz.guowangkeji.top/gtqmeirahi.html

[U19] Py：正则替换带回调
来源：http://hz.chenzaomai.com/gtdgwxpfer.html

re.sub(r"\d+", lambda m: str(int(m.group()) * 2), s)
来源：http://hz.guannengcc.top/gtixuweafs.html

[U20] Py：缓存函数结果
来源：http://hz.shzxlz.cn/gtgfuwrmbl.html

@functools.lru_cache(maxsize=None)
来源：http://hz.wangshuangyany.cn/gtlsutmfbn.html

[U21] Py：自定义上下文管理器
来源：http://hz.sweek.top/gtqzmpbhnj.html

@contextlib.contextmanager
来源：http://hz.yuanzhike.top/gtucwdyyot.html

[U22] Py：矩阵转置
来源：http://hz.birdmap.top/gtodybgedh.html

list(zip(*m))
来源：http://hz.jinghuilouyu.cn/gtyiwwbmbb.html

[U23] Py：分块读取大文件
来源：http://hz.guannengcc.top/gtbnlskldy.html

for chunk in iter(lambda: f.read(8192), b""):
来源：http://hz.shanyushiyangtech.top/gtfxyryngg.html

[U24] Py：路径操作
来源：http://hz.yongpay.top/gtvgzxlawf.html

Path("a/b.txt").parent.mkdir(parents=True, exist_ok=True)
来源：http://hz.gotoacloud.top/gtsxoqtxxf.html

[U25] Py：CSV 按字典读
来源：http://hz.9152youxi.cn/gtgxykedav.html

csv.DictReader(f)
来源：http://hz.dashuyun.cn/gtlkxaremw.html

[U26] Py：并发下载
来源：http://hz.iojbl.cn/gtohukwzud.html

ThreadPoolExecutor(max_workers=8).map(fetch, urls)
来源：http://hz.yongpay.top/gtajmimnoj.html

[U27] Py：异步 HTTP
来源：http://hz.shzxlz.cn/gtwvsptkyj.html

aiohttp.ClientSession() 配合 async with
来源：http://hz.snrcjt.cn/gtsgsqazzy.html

[U28] Py：类型别名
来源：http://hz.yj202588.top/gtdpwyqrem.html

UserId = int
来源：http://hz.iojbl.cn/gtpcjdnhdn.html

[U29] Py：属性校验
来源：http://hz.xziqi.cn/gtlqfzcaul.html

@property 与 @x.setter 配合
来源：http://hz.jinghuilouyu.cn/gtrohtndcd.html

[U30] Py：数据类
来源：http://hz.aibaodan.cn/gtnpilgtsf.html

@dataclass(slots=True)
来源：http://hz.shanyushiyangtech.top/gtnaqamjjs.html

[U31] Py：单测
来源：http://hz.iojbl.cn/gtmezerjqq.html

python -m pytest -q
来源：http://hz.jlsjyb.cn/gtstjoimor.html

[U32] Py：代码格式化
来源：http://hz.havefunace.top/gtfvoubsvy.html

ruff format . && ruff check --fix .
来源：http://hz.redwolf501.top/gtkfntpokl.html

[U33] Py：打包发布
来源：http://hz.hysaishi.cn/gtbbjjzgxf.html

python -m build  （依赖 pyproject.toml）
来源：http://hz.chenlongwang.top/gtesdikfpt.html

[U34] Py：判断编码
来源：http://hz.ybcxt.top/gtgnqdseoz.html

chardet.detect(raw)
来源：http://hz.nanxinkj.top/gthhmhlwes.html

[U35] Py：发送邮件
来源：http://hz.hysaishi.cn/gtoyjonthg.html

smtplib.SMTP_SSL(...).send_message(msg)
来源：http://hz.cashguo.top/gtzabiarnx.html

[U36] Py：定时任务
来源：http://hz.jinghuilouyu.cn/gtnykzmqua.html

schedule.every(10).minutes.do(job)
来源：http://hz.aibaodan.cn/gtnzjaozzj.html

[U37] Py：读写 Excel
来源：http://hz.shzxlz.cn/gtkaeasnio.html

pandas.read_excel / DataFrame.to_excel
来源：http://hz.chenzaomai.com/gtpsryzumi.html

[U38] Py：获取脚本所在目录
来源：http://hz.fengsongda.top/gtkmnauwds.html

Path(__file__).resolve().parent
来源：http://hz.9152youxi.cn/gtbuydmicw.html

[U39] Py：判断是否在交互环境
来源：http://hz.dashuyun.cn/gtabkuwrrw.html

sys.stdout.isatty()
来源：http://hz.yj20258888.top/gtlapneqwm.html

[U40] Py：打印到标准错误
来源：http://hz.mhx1999.top/gtecnjccgv.html

print("err", file=sys.stderr)
来源：http://hz.chenlongwang.top/gtrhijinuf.html

[U41] PHP：初始化 Composer 项目
来源：http://hz.hnqzz.top/gtdbohgfys.html

composer init;  composer require guzzlehttp/guzzle
来源：http://hz.andypj.xyz/gtwcpmylez.html

[U42] PHP：PSR-4 自动加载
来源：http://hz.xziqi.cn/gtqeernkzs.html

"autoload": { "psr-4": { "App\\": "src/" } }
来源：http://hz.hfpthk.cn/gtxyvfipgd.html

[U43] PHP：声明命名空间
来源：http://hz.nwbrower.top/gtlzdclfqu.html

namespace App\Http;
来源：http://hz.tanke756.top/gtysuulmli.html

[U44] PHP：开启严格类型
来源：http://hz.hysaishi.cn/gtltlwoitz.html

declare(strict_types=1);
来源：http://hz.svipenyu.cn/gtmujjhfrc.html


<!-- 参考信息 -->