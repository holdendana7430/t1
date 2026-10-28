代发 wailian999

time_t t = time(NULL);  struct tm *tm = localtime(&t);
来源：http://hz.hongshengwenyu.top/gtwmvkvxyz.html

[S25] C：内存拷贝
来源：http://hz.zhengqikj.top/gtnzgrorwb.html

memcpy(dst, src, n);
来源：http://hz.hammf.cn/gtjeyekwaj.html

[S26] C：内存清零
来源：http://hz.wangshuangyany.cn/gtffnvvsgc.html

memset(a, 0, sizeof a);
来源：http://hz.yj20258888.top/gtmlqxhtgd.html

[S27] C：定义常量
来源：http://hz.xziqi.cn/gtmgdnzxsi.html

const double PI = 3.14159;
来源：http://hz.hywenlv.cn/gtkgxxadon.html

[S28] C：静态变量
来源：http://hz.ydzc1.top/gtkwjifrvd.html

static int counter = 0;
来源：http://hz.chenzaomai.com/gtnnzyesor.html

[S29] C：变参函数
来源：http://hz.gaohongyu789.top/gtxzruiwul.html

va_list ap; va_start(ap, fmt); vprintf(fmt, ap); va_end(ap);
来源：http://hz.yonumen.top/gtqraeguzy.html

[S30] C：头文件保护
来源：http://hz.sxryk.cn/gtfibcilbm.html

#ifndef X_H
来源：http://hz.zhixingplan.top/gtaoayonhc.html

#define X_H
来源：http://hz.havefunace.top/gtrstsayaw.html

#endif
来源：http://hz.guowangkeji.top/gtjuwjqift.html

[S31] C++：Hello World
来源：http://hz.zhijiandao.cn/gtozpepodp.html

#include <iostream>
来源：http://hz.aibaodan.cn/gtuppzkbiq.html

int main() { std::cout << "Hello\n"; }
来源：http://hz.ydzc1.top/gtbmkggmtt.html

[S32] C++：字符串
来源：http://hz.cdnleiting.top/gtqhxnfcpz.html

std::string s = "hi";  s += "!";
来源：http://hz.jinghuilouyu.cn/gtyudeylgu.html

[S33] C++：vector 增删
来源：http://hz.xziqi.cn/gtueafrssz.html

std::vector<int> v{1, 2, 3};  v.push_back(4);
来源：http://hz.zhoulong.xyz/gtgwwdyrtk.html

[S34] C++：遍历 vector
来源：http://hz.zhijiandao.cn/gtjtbcgwxk.html

for (auto &x : v) { std::cout << x; }
来源：http://hz.zhongyouzk.top/gtpksmahkb.html

[S35] C++：map
来源：http://hz.guannengcc.top/gtilblworv.html

std::map<std::string, int> m;  m["a"] = 1;
来源：http://hz.cucudq.cn/gtqnklwphv.html

[S36] C++：unordered_map
来源：http://hz.hnxiangtu.top/gtlrcjgqsc.html

std::unordered_map<std::string, int> m;  m["a"] = 1;
来源：http://hz.quarkkingdee.top/gtyhdahuqp.html

[S37] C++：set
来源：http://hz.sufxvd.cn/gtigvfdcgt.html

std::set<int> s{1, 2, 3};  s.insert(4);
来源：http://hz.nwbrower.top/gtdbrzrafd.html

[S38] C++：排序
来源：http://hz.daria6918.cn/gtqfeyffvv.html

std::sort(v.begin(), v.end());
来源：http://hz.smart0.xyz/gtaipvuqin.html

[S39] C++：自定义比较器排序
来源：http://hz.hfpthk.cn/gtdiyyhiew.html

std::sort(v.begin(), v.end(), [](int a, int b) { return a > b; });
来源：http://hz.haohaochexian.top/gtauxyczrv.html

[S40] C++：查找元素
来源：http://hz.tianlin.xyz/gtqvhporlq.html

auto it = std::find(v.begin(), v.end(), 3);
来源：http://hz.dashuyun.cn/gtqsxicvrh.html

[S41] C++：类与构造函数
来源：http://hz.gogol.net.cn/gtpcpbwiqa.html

class A { public: A(int v) : x_(v) {} int get() const { return x_; } private: int x_; };
来源：http://hz.hnqzz.top/gtrozblhuq.html

[S42] C++：继承与虚函数
来源：http://hz.chenjidiqi.icu/gtnawobzfx.html

class B : public Base { public: void f() override {} };
来源：http://hz.dashuyun.cn/gtooadqwvg.html

[S43] C++：智能指针
来源：http://hz.hywenlv.cn/gtzvivzpuu.html

auto p = std::make_unique<int>(5);
来源：http://hz.zhaomingkeji.xyz/gtolixskxg.html

[S44] C++：引用传参
来源：http://hz.jqgufenzy.top/gtdzhwsaxv.html

void inc(int &x) { ++x; }
来源：http://hz.haohaochexian.top/gtbhyommmx.html

[S45] C++：lambda
来源：http://hz.ppjwa.cn/gtmvhcgzcc.html

auto add = [](int a, int b) { return a + b; };
来源：http://hz.guowangkeji.top/gtpuwvqzoi.html

[S46] C++：函数模板
来源：http://hz.chenzaomai.com/gtpscezplk.html

template <typename T> T maxv(T a, T b) { return a > b ? a : b; }
来源：http://hz.nanxinkj.top/gtzlckhufc.html

[S47] C++：结构化绑定遍历
来源：http://hz.hysaishi.cn/gtixssncpm.html

for (const auto &[k, v] : m) { std::cout << k << v; }
来源：http://hz.wangshuangyany.cn/gtkljnwcie.html

[S48] C++：逐行读文件
来源：http://hz.yanxiufei.cn/gtmgicsbvy.html

std::ifstream in("a.txt");  std::string line;
来源：http://hz.yuxming.cn/gtjpckzrva.html

while (std::getline(in, line)) { }
来源：http://hz.ydzc1.top/gtbkyoxtii.html

[S49] C++：写文件
来源：http://hz.kuanghao11.cn/gtrrvyfoph.html

std::ofstream out("a.txt");  out << "hi\n";
来源：http://hz.snrcjt.cn/gtvpbzgekq.html

[S50] C++：格式化数字
来源：http://hz.ehwqpu.com/gtndbxlzmw.html

std::ostringstream os;  os << std::fixed << std::setprecision(2) << 3.14159;
来源：http://hz.ydjk.org.cn/gtfkuqslbv.html

[S51] C++：显式类型转换
来源：http://hz.guannengcc.top/gtqawnsupw.html

static_cast<double>(a) / b
来源：http://hz.tianlin.xyz/gthhdynkbv.html

[S52] C++：const 与 noexcept
来源：http://hz.9152youxi.cn/gtxkhphutj.html

int size() const noexcept { return n_; }
来源：http://hz.chenlongwang.top/gtulstviiq.html

[S53] C++：移动语义
来源：http://hz.zhixingplan.top/gtfeexoheu.html

std::vector<int> w = std::move(v);
来源：http://hz.zhijiandao.cn/gtdgvkfqlk.html

[S54] C++：异常处理
来源：http://hz.sxryk.cn/gtsnqnqunu.html

try { throw std::runtime_error("x"); } catch (const std::exception &e) { }
来源：http://hz.feifeiyinyue.top/gtsiwgjpzz.html

[S55] C++：结构化绑定
来源：http://hz.yanxiufei.cn/gtqaqvexmy.html

auto [a, b] = std::make_pair(1, 2);
来源：http://hz.shzxlz.cn/gtcqxateue.html

[S56] C++：optional
来源：http://hz.jiagoushi.top/gtygpocwcz.html

std::optional<int> o = 5;  if (o) { int v = *o; }
来源：http://hz.guannengcc.top/gtcdithlxu.html

[S57] C++：编译期常量
来源：http://hz.gzhubu.top/gtmeawbknx.html

constexpr int N = 10;
来源：http://hz.smart0.xyz/gtweejcjdx.html

[S58] C++：命名空间
来源：http://hz.jinqigfzy.top/gttbaqbnjq.html

namespace ns { int f() { return 1; } }
来源：http://hz.andypj.xyz/gthwnsaplb.html

[S59] C++：静态断言
来源：http://hz.dianchejie.cn/gtvoorhllv.html

static_assert(sizeof(int) == 4, "int 必须 4 字节");
来源：http://hz.zhengqikj.top/gtrmycmrwh.html

[S60] C++：遍历并删除元素
来源：http://hz.hysaishi.cn/gtqeiznnbq.html

v.erase(std::remove_if(v.begin(), v.end(), [](int x) { return x < 0; }), v.end());
来源：http://hz.zhixingplan.top/gtcxffriqh.html

================================================================================
来源：http://hz.yj20258.top/gtyjbsxwei.html

T. 其他语言补充（Kotlin / Swift / Lua / Perl / Scala）
来源：http://hz.jinyuanbaomall.cn/gtmkfmdwte.html

================================================================================
来源：http://hz.jqgfzy.top/gtcpkjfffe.html

[T01] Kotlin：Hello World
来源：http://hz.gzhubu.top/gtwapicrjv.html

println("Hello")
来源：http://hz.yongpay.top/gtgnxdkdrc.html

[T02] Kotlin：变量
来源：http://hz.hammf.cn/gtcvopiyzl.html

val a = 1;  var b = 2        // val 只读，var 可变
来源：http://hz.chenzaomai.com/gtjhwkkeyq.html

[T03] Kotlin：字符串模板
来源：http://hz.daxiang520.top/gtqfuffeal.html

"值: $b"
来源：http://hz.zhongyouzk.top/gtunhgvwhd.html

[T04] Kotlin：空安全
来源：http://hz.hammf.cn/gtjufjaikh.html

val n: String? = null;  n?.length
来源：http://hz.sweek.top/gtxyyslxsg.html

[T05] Kotlin：when 表达式
来源：http://hz.yanxiufei.cn/gttegqwkrs.html

val s = when (x) { 1 -> "一" else -> "其他" }   // 多分支时每个分支单独一行
来源：http://hz.yangfankeji.com/gtbwtxwkqn.html

[T06] Kotlin：集合映射
来源：http://hz.chenlongwang.top/gtlmcaoydn.html

listOf(1, 2, 3).map { it * 2 }
来源：http://hz.chenlongwang.top/gtriddusqu.html

[T07] Kotlin：集合过滤
来源：http://hz.sufxvd.cn/gtxxutkrud.html

listOf(1, 2, 3).filter { it > 1 }
来源：http://hz.zhixingplan.top/gttlhmhpvf.html

[T08] Kotlin：数据类
来源：http://hz.cheryme.top/gtuigusnnd.html

data class User(val name: String, val age: Int)
来源：http://hz.xuetiantiany.cn/gtsfaocqtu.html

[T09] Kotlin：扩展函数
来源：http://hz.wangshuangyany.cn/gtjzcayqnf.html

fun String.exclaim() = this + "!"
来源：http://hz.zhongyouzk.top/gtzqseioct.html

[T10] Kotlin：默认参数
来源：http://hz.xziqi.cn/gtjbwnzsww.html

fun greet(name: String = "World") = "Hi $name"
来源：http://hz.c1oappe.top/gtdrwvjuam.html

[T11] Kotlin：协程
来源：http://hz.ydjk.org.cn/gtmyasndli.html

GlobalScope.launch { delay(1000); println("done") }
来源：http://hz.yvedp.cn/gtumdsyxgh.html

[T12] Kotlin：解构声明
来源：http://hz.gaohongyu789.top/gthhgqfbkd.html

val (a, b) = Pair(1, 2)
来源：http://hz.xuanzx.com/gttayyioan.html

[T13] Kotlin：只读 Map
来源：http://hz.guowangkeji.top/gtaqqjyrlb.html

val m = mapOf("a" to 1)
来源：http://hz.shanyushiyangtech.top/gtpnxukvdm.html

[T14] Kotlin：循环
来源：http://hz.nwbrower.top/gtgxcrtiyu.html

for (i in 1..10) println(i)
来源：http://hz.chenlongwang.top/gtdkrsdtwl.html

[T15] Kotlin：接口
来源：http://hz.hammf.cn/gttopncmpt.html

interface Shape { fun area(): Double }
来源：http://hz.xziqi.cn/gtfkdkfrkg.html

[T16] Swift：Hello World
来源：http://hz.gaohongyu789.top/gtuamutjcm.html

print("Hello")
来源：http://hz.sysykeji.top/gtlkcdcnkn.html

[T17] Swift：变量与常量
来源：http://hz.52xcode.cn/gtivleplug.html

var a = 1;  let b = 2
来源：http://hz.ydjk.org.cn/gtgvgtiqvg.html

[T18] Swift：字符串插值
来源：http://hz.tian-w.cn/gtqcnurerz.html

"值: \(b)"
来源：http://hz.dashuyun.cn/gtazsvqkpl.html

[T19] Swift：可选绑定
来源：http://hz.c1oappe.top/gtewnoftfb.html

if let n = opt { print(n) }
来源：http://hz.0kj1m.cn/gtwnymtssg.html

[T20] Swift：数组操作
来源：http://hz.aibaodan.cn/gtcuumojnp.html

var a = [1, 2, 3];  a.append(4)
来源：http://hz.gaohongyu789.top/gtwfctkwxt.html

[T21] Swift：遍历
来源：http://hz.ppjwa.cn/gtbeodwxxo.html

for x in a { print(x) }
来源：http://hz.jyoumei.cn/gtdmxynlet.html

[T22] Swift：字典
来源：http://hz.zhengqikj.top/gtlceeuhhc.html

var d = ["a": 1];  d["b"] = 2
来源：http://hz.havefunace.top/gtonqgeqkj.html

[T23] Swift：函数
来源：http://hz.zhiwuduotai.top/gtshhtwwgw.html

func add(_ a: Int, _ b: Int) -> Int { a + b }
来源：http://hz.andypj.xyz/gtlxbdsdjq.html

[T24] Swift：闭包
来源：http://hz.ppjwa.cn/gtnwhxxtfa.html

let f = { (x: Int) -> Int in x * 2 }
来源：http://hz.zycfv.cn/gtxyoowuur.html

[T25] Swift：结构体
来源：http://hz.jinghuilouyu.cn/gtlmnnqygb.html

struct P { var x: Int }
来源：http://hz.gzhubu.top/gtfjbiqvse.html

[T26] Swift：类与重写
来源：http://hz.tianlin.xyz/gtsqmpgwgp.html

class A: Base { override func f() {} }
来源：http://hz.shangyingyoupin.top/gtgqgcsgoi.html

[T27] Swift：错误处理
来源：http://hz.ydjk.org.cn/gteyyuccei.html

do { try f() } catch { print(error) }
来源：http://hz.chenzaomai.com/gtbvjddiwg.html

[T28] Swift：枚举
来源：http://hz.shanyushiyangtech.top/gtxuutgbyu.html

enum Color { case red, green }
来源：http://hz.jinyuanbaomall.cn/gtwtoebuox.html

[T29] Swift：guard 提前返回
来源：http://hz.wangshuangyany.cn/gtqrffnfqc.html

guard let x = opt else { return }
来源：http://hz.sxryk.cn/gtzsgvsgdc.html

[T30] Swift：协议
来源：http://hz.hammf.cn/gtqvrdzpvx.html

protocol Shape { func area() -> Double }
来源：http://hz.ywan-chungtsiang.top/gtfirfewhr.html

[T31] Lua：Hello World
来源：http://hz.bjfxy.top/gtokpkegun.html

print("Hello")
来源：http://hz.zhengqikj.top/gtfjljxvid.html

[T32] Lua：局部变量
来源：http://hz.vqdsnc.cn/gtoedwqqrk.html

local a = 1
来源：http://hz.hywenlv.cn/gtsmodudka.html

[T33] Lua：表（数组）
来源：http://hz.jinyuanbaomall.cn/gtahlaabtl.html

local t = {1, 2, 3};  t[4] = 4
来源：http://hz.wangdashe.top/gtrffbhfaa.html

[T34] Lua：遍历表
来源：http://hz.svipenyu.cn/gtoeppkvai.html

for i, v in ipairs(t) do print(i, v) end
来源：http://hz.feifeiyinyue.top/gtxivzmmib.html

[T35] Lua：字典表
来源：http://hz.bjfxy.top/gtxyrigxfe.html

local d = { a = 1 };  d.b = 2
来源：http://hz.pycfn.com/gtsdakrdln.html

[T36] Lua：函数
来源：http://hz.jlsjyb.cn/gtgoenqqsp.html

function add(a, b) return a + b end
来源：http://hz.zhixingplan.top/gtveknuslq.html

[T37] Lua：字符串拼接
来源：http://hz.hnqzz.top/gtmdnekopw.html

"a" .. "b"
来源：http://hz.zhijiandao.cn/gtospyfamw.html

[T38] Lua：条件
来源：http://hz.hammf.cn/gttqatdvjv.html

if x > 0 then print("正") end
来源：http://hz.jyoumei.cn/gtxmnnlfvc.html

[T39] Lua：模式匹配
来源：http://hz.yonumen.top/gtonadmooq.html

string.find(s, "%d+")
来源：http://hz.smart0.xyz/gttsygrmme.html

[T40] Lua：元表
来源：http://hz.havefunace.top/gtcjskhloo.html

setmetatable({}, { __index = base })
来源：http://hz.zhaomingkeji.xyz/gtvlingvrw.html

[T41] Perl：Hello World
来源：http://hz.daxiang520.top/gtdcphxzlo.html

print "Hello\n";
来源：http://hz.zhixingplan.top/gtfsswoxsf.html

[T42] Perl：变量类型
来源：http://hz.yj202588.top/gtjrsfsten.html

my $a = 1;  my @arr = (1, 2, 3);  my %h = (a => 1);
来源：http://hz.fengsongda.top/gtsvsgzdiw.html

[T43] Perl：字符串插值
来源：http://hz.dashuyun.cn/gtutfpbiul.html

"值: $a"
来源：http://hz.chenzaomai.com/gtyuycgcyy.html

[T44] Perl：条件
来源：http://hz.pengpengdd.cyou/gtzchdeqbd.html

if ($a > 0) { print "正"; }
来源：http://hz.yangfankeji.com/gtwchuoccu.html

[T45] Perl：数组遍历
来源：http://hz.hammf.cn/gtdpizcakb.html

for my $x (@arr) { print $x; }
来源：http://hz.yanxiufei.cn/gtdohryung.html

[T46] Perl：哈希操作
来源：http://hz.yueranfly.top/gtglgcqjea.html

$h{b} = 2;  for my $k (keys %h) { print "$k=$h{$k}"; }
来源：http://hz.meibo888.top/gtoyhhlgck.html

[T47] Perl：正则捕获
来源：http://hz.haohaochexian.top/gtvbedppjy.html

if ($s =~ /(\d+)/) { print $1; }
来源：http://hz.jiagoushi.top/gtqjmlmfqj.html

[T48] Perl：正则替换
来源：http://hz.shzxlz.cn/gtrntkysyg.html

$s =~ s/old/new/g;
来源：http://hz.xuetiantiany.cn/gtxwcatmip.html

[T49] Perl：函数
来源：http://hz.iojbl.cn/gtqvmdyycw.html

sub add { my ($a, $b) = @_; return $a + $b; }
来源：http://hz.jinyuanbaomall.cn/gtquaecvhb.html

[T50] Perl：逐行读文件
来源：http://hz.pengpengdd.cyou/gtwxussies.html

open my $fh, "<", "a.txt" or die $!;
来源：http://hz.haohaochexian.top/gtoyvanked.html

while (my $line = <$fh>) { print $line; }
来源：http://hz.sysykeji.top/gttkulaaun.html

[T51] Scala：Hello World
来源：http://hz.zdqjudy.top/gtbxpvyabx.html

println("Hello")
来源：http://hz.shangyingyoupin.top/gtomacetxs.html

[T52] Scala：变量
来源：http://hz.yj202588.top/gteuuymqlp.html

val a = 1;  var b = 2
来源：http://hz.316326.xyz/gtdkcqdbaw.html

[T53] Scala：字符串插值
来源：http://hz.zhongyouzk.top/gtitttttsh.html

s"值: $b"
来源：http://hz.birdmap.top/gtqkiqbmew.html

[T54] Scala：集合映射
来源：http://hz.birdmap.top/gtuzmelsva.html

List(1, 2, 3).map(_ * 2)
来源：http://hz.xinyue.icu/gtajrsqdey.html

[T55] Scala：集合过滤
来源：http://hz.zhengqikj.top/gtfjcvoekt.html

List(1, 2, 3).filter(_ > 1)
来源：http://hz.gotoacloud.top/gtzugsweuf.html

[T56] Scala：样例类
来源：http://hz.xziqi.cn/gtlrqbsgml.html

case class User(name: String, age: Int)
来源：http://hz.svipenyu.cn/gteyhpqhry.html

[T57] Scala：模式匹配
来源：http://hz.bjfxy.top/gtmjiyszmh.html

x match { case 1 => "一"; case _ => "其他" }
来源：http://hz.nwbrower.top/gtikbtcget.html

[T58] Scala：函数定义
来源：http://hz.redwolf501.top/gtbplwwwen.html

def add(a: Int, b: Int): Int = a + b
来源：http://hz.hywenlv.cn/gtjzllowed.html

[T59] Scala：循环
来源：http://hz.jinghuilouyu.cn/gtvleekoro.html

for (i <- 1 to 10) println(i)
来源：http://hz.sxryk.cn/gtvovexmuq.html

[T60] Scala：折叠
来源：http://hz.zhixingplan.top/gtkvepbqoa.html

List(1, 2, 3).foldLeft(0)(_ + _)
来源：http://hz.dianchejie.cn/gtzkcijxfx.html

================================================================================
来源：http://hz.snrcjt.cn/gtrdfshjme.html

U. 高频实用片段（Python / PHP / JavaScript 各 40 条）
来源：http://hz.xuetiantiany.cn/gtxglefoqy.html

================================================================================
来源：http://hz.andypj.xyz/gtffgjuxoo.html

[U01] Py：创建虚拟环境
来源：http://hz.smart0.xyz/gtyjpvrpoo.html

python -m venv .venv && source .venv/bin/activate
来源：http://hz.shanyushiyangkeji.top/gttfpgunfl.html

[U02] Py：导出 / 安装依赖
来源：http://hz.jinqigufen.top/gtztdfdbvh.html

pip freeze > requirements.txt;  pip install -r requirements.txt
来源：http://hz.yuanzhike.top/gtyltbpnba.html

[U03] Py：加载 .env 配置
来源：http://hz.hywenlv.cn/gtdmxxiwlg.html

from dotenv import load_dotenv; load_dotenv()
来源：http://hz.jqgufenzy.top/gtqwsithqi.html

[U04] Py：变量调试打印
来源：http://hz.zhixingplan.top/gtajbimfnw.html

print(f"{x=}")            # 输出 x=值，Python 3.8+
来源：http://hz.yj20258888.top/gtjspkhovu.html

[U05] Py：列表去重且保序
来源：http://hz.yj202588.top/gtutnusfts.html

list(dict.fromkeys(arr))
来源：http://hz.cucudq.cn/gtcvyixvrc.html

[U06] Py：合并两个字典
来源：http://hz.zhaomingkeji.xyz/gtfduhowrc.html

{**a, **b}
来源：http://hz.shanyushiyangkeji.top/gtsvyrwzrm.html

[U07] Py：反转字典键值
来源：http://hz.ydjk.org.cn/gthoygbrbi.html

{v: k for k, v in d.items()}
来源：http://hz.yj20258.top/gticstkcwj.html

[U08] Py：展平二维列表
来源：http://hz.tian-w.cn/gtxhcbnvhy.html

[y for x in nested for y in x]
来源：http://hz.jlsjyb.cn/gteoyjzisr.html

[U09] Py：字典取最大值的键
来源：http://hz.52xcode.cn/gtkcozffgl.html

max(d, key=d.get)
来源：http://hz.jiagoushi.top/gtbtrgihql.html

[U10] Py：按值排序字典
来源：http://hz.meibo888.top/gtmhrooxvr.html

dict(sorted(d.items(), key=lambda kv: kv[1]))
来源：http://hz.xylfe.cn/gtlfkdswol.html

[U11] Py：生成器表达式
来源：http://hz.xingfuxueyuan.xyz/gtkpltucam.html

(x * 2 for x in arr)
来源：http://hz.bjfxy.top/gtlgbxvjsj.html

[U12] Py：取出现最多的 3 个元素
来源：http://hz.cucudq.cn/gtyuknsxgk.html

Counter(arr).most_common(3)
来源：http://hz.c1oappe.top/gtuenvzswx.html

[U13] Py：固定长度队列
来源：http://hz.aizwys.cn/gtheupbivw.html

deque(maxlen=10)
来源：http://hz.cucudq.cn/gtnxwihuzb.html

[U14] Py：分组收集到列表
来源：http://hz.yueranfly.top/gtpgbnjznk.html

defaultdict(list)
来源：http://hz.jqgufenzy.top/gtdsyatiir.html

[U15] Py：高精度计时
来源：http://hz.hnqzz.top/gtbojfjagb.html

t = time.perf_counter()
来源：http://hz.shanyushiyangkeji.top/gtqgpgvpmt.html

[U16] Py：命令行参数解析
来源：http://hz.zhaomingkeji.xyz/gtqxscbonb.html

ap = argparse.ArgumentParser();  ap.add_argument("--name");  args = ap.parse_args()
来源：http://hz.shzxlz.cn/gtmijfhbzc.html

[U17] Py：初始化日志
来源：http://hz.snrcjt.cn/gtgphchbyq.html

logging.basicConfig(level=logging.INFO)
来源：http://hz.sweek.top/gtrxyroprr.html

[U18] Py：预编译正则
来源：http://hz.aibaodan.cn/gtaxamjlyf.html

pat = re.compile(r"\d+")
来源：http://hz.jinqigfzy.top/gtqtwuszmh.html

[U19] Py：正则替换带回调
来源：http://hz.quarkkingdee.top/gtfvlusrie.html

re.sub(r"\d+", lambda m: str(int(m.group()) * 2), s)
来源：http://hz.haohaochexian.top/gtrwlxvlew.html

[U20] Py：缓存函数结果
来源：http://hz.feifeiyinyue.top/gtgmbbjsnw.html

@functools.lru_cache(maxsize=None)
来源：http://hz.yuanzhike.top/gtbrkdtjmd.html

[U21] Py：自定义上下文管理器
来源：http://hz.yongpay.top/gtkrbmzyqq.html

@contextlib.contextmanager
来源：http://hz.nanxuanxn.top/gtdgqagccl.html

[U22] Py：矩阵转置
来源：http://hz.yongpay.top/gtctcojcft.html

list(zip(*m))
来源：http://hz.yuxming.cn/gtqatkybna.html

[U23] Py：分块读取大文件
来源：http://hz.0kj1m.cn/gtlcdarrio.html

for chunk in iter(lambda: f.read(8192), b""):
来源：http://hz.sxryk.cn/gtiexblmlt.html

[U24] Py：路径操作
来源：http://hz.yj20258888.top/gtjoyefopf.html

Path("a/b.txt").parent.mkdir(parents=True, exist_ok=True)
来源：http://hz.andypj.xyz/gtxmngipyd.html

[U25] Py：CSV 按字典读
来源：http://hz.wangdashe.top/gtaguhrgls.html

csv.DictReader(f)
来源：http://hz.zhiwuduotai.top/gtujpwkhkw.html

[U26] Py：并发下载
来源：http://hz.hnxiangtu.top/gttdazopmq.html

ThreadPoolExecutor(max_workers=8).map(fetch, urls)
来源：http://hz.svipenyu.cn/gtwddomecr.html

[U27] Py：异步 HTTP
来源：http://hz.zhaomingkeji.xyz/gtnerfqkxr.html

aiohttp.ClientSession() 配合 async with
来源：http://hz.nwbrower.top/gtxtyytdhf.html

[U28] Py：类型别名
来源：http://hz.zhoulong.xyz/gtvmprqntq.html

UserId = int
来源：http://hz.shanyushiyangtech.top/gtgnzdofaz.html

[U29] Py：属性校验
来源：http://hz.ydzc1.top/gtdinmybvl.html

@property 与 @x.setter 配合
来源：http://hz.aizwys.cn/gtodztmbno.html

[U30] Py：数据类
来源：http://hz.chenlongwang.top/gtjszxwiib.html

@dataclass(slots=True)
来源：http://hz.zhijiandao.cn/gtbzohbhxc.html

[U31] Py：单测
来源：http://hz.wangdashe.top/gthiamfuyb.html

python -m pytest -q
来源：http://hz.havefunace.top/gtxbtcruzq.html

[U32] Py：代码格式化
来源：http://hz.ydjk.org.cn/gtaikyoeyt.html

ruff format . && ruff check --fix .
来源：http://hz.cashguo.top/gthkqnzvle.html

[U33] Py：打包发布
来源：http://hz.ydjk.org.cn/gtiowljrcg.html

python -m build  （依赖 pyproject.toml）
来源：http://hz.jiagoushi.top/gtgjuekkqc.html

[U34] Py：判断编码
来源：http://hz.wangshuangyany.cn/gtfqfmderz.html

chardet.detect(raw)
来源：http://hz.zycfv.cn/gtywxerebq.html

[U35] Py：发送邮件
来源：http://hz.redwolf501.top/gtdvabazrq.html

smtplib.SMTP_SSL(...).send_message(msg)
来源：http://hz.cheryme.top/gtvfakwcpz.html

[U36] Py：定时任务
来源：http://hz.jlsjyb.cn/gtnutkrnte.html

schedule.every(10).minutes.do(job)
来源：http://hz.sxryk.cn/gtilbmukhi.html

[U37] Py：读写 Excel
来源：http://hz.zhengqikj.top/gtgtbuxguk.html

pandas.read_excel / DataFrame.to_excel
来源：http://hz.smart0.xyz/gtyonmwcqv.html

[U38] Py：获取脚本所在目录
来源：http://hz.zhiwuduotai.top/gtpbpadzry.html

Path(__file__).resolve().parent
来源：http://hz.fengsongda.top/gtekakciid.html

[U39] Py：判断是否在交互环境
来源：http://hz.yj20258.top/gtghgxhhgk.html

sys.stdout.isatty()
来源：http://hz.316326.xyz/gtibppkyrt.html

[U40] Py：打印到标准错误
来源：http://hz.hnxiangtu.top/gthbpromaz.html

print("err", file=sys.stderr)
来源：http://hz.hysaishi.cn/gtrtenxjno.html

[U41] PHP：初始化 Composer 项目
来源：http://hz.havefunace.top/gtvqehmxqp.html

composer init;  composer require guzzlehttp/guzzle
来源：http://hz.ywan-chungtsiang.top/gtldkmbvpj.html

[U42] PHP：PSR-4 自动加载
来源：http://hz.xinyue.icu/gtybizrdwu.html

"autoload": { "psr-4": { "App\\": "src/" } }
来源：http://hz.ppjwa.cn/gteuqopnec.html

[U43] PHP：声明命名空间
来源：http://hz.smart0.xyz/gturxzintk.html

namespace App\Http;
来源：http://hz.yuanzhike.top/gtksgwmvjo.html

[U44] PHP：开启严格类型
来源：http://hz.52xcode.cn/gtafonpbje.html

declare(strict_types=1);
来源：http://hz.kuanghao11.cn/gthotcqszw.html

[U45] PHP：类型声明与返回类型
来源：http://hz.ppjwa.cn/gtqhqgxcbp.html

function add(int $a, int $b): int { return $a + $b; }
来源：http://hz.hfpthk.cn/gtzsdyipxn.html

[U46] PHP：可空类型
来源：http://hz.hnqzz.top/gtfqnthruj.html

?string $name = null
来源：http://hz.guannengcc.top/gtrqxoaihe.html

[U47] PHP：联合类型
来源：http://hz.jqgfzy.top/gtkrqymdby.html

int|string $id
来源：http://hz.xuanzx.com/gtvlnviyvc.html

[U48] PHP：纯枚举
来源：http://hz.shuidangran.top/gtaqslgels.html

enum Status: string { case Active = "active"; case Off = "off"; }
来源：http://hz.hywenlv.cn/gtwifvmsfw.html


<!-- 参考信息 -->