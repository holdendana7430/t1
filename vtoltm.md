代发 wailian999

bsearch(&key, a, n, sizeof(int), cmp);
来源：http://hz.ywan-chungtsiang.top/gtyffyzswl.html

[S21] C：字符类别判断
来源：http://hz.chenzaomai.com/gtmotybjzg.html

isdigit(c);  isalpha(c);  isspace(c);
来源：http://hz.ehwqpu.com/gtyysttdrx.html

[S22] C：字符串转数字
来源：http://hz.zhoulong.xyz/gtqnguddym.html

atoi("42");  strtod("3.14", NULL);
来源：http://hz.fzhhl.top/gtacpvsmoi.html

[S23] C：随机数
来源：http://hz.zhengqikj.top/gtaiffuocs.html

srand(time(NULL));  int r = rand() % 100;
来源：http://hz.shanyushiyangtech.top/gthwoasfzw.html

[S24] C：获取本地时间
来源：http://hz.tianlin.xyz/gtggwoxklm.html

time_t t = time(NULL);  struct tm *tm = localtime(&t);
来源：http://hz.tanke756.top/gtrnwxqrxl.html

[S25] C：内存拷贝
来源：http://hz.sweek.top/gtdvbgkjeb.html

memcpy(dst, src, n);
来源：http://hz.ehwqpu.com/gtrqnkxjtn.html

[S26] C：内存清零
来源：http://hz.jlsjyb.cn/gtnspnorai.html

memset(a, 0, sizeof a);
来源：http://hz.gaohongyu789.top/gtcjwuftog.html

[S27] C：定义常量
来源：http://hz.pycfn.com/gtpivuuffu.html

const double PI = 3.14159;
来源：http://hz.yongpay.top/gtazmorqto.html

[S28] C：静态变量
来源：http://hz.shuidangran.top/gtspymixsh.html

static int counter = 0;
来源：http://hz.wangdashe.top/gthbkamrmy.html

[S29] C：变参函数
来源：http://hz.yangfankeji.com/gtgueobvzm.html

va_list ap; va_start(ap, fmt); vprintf(fmt, ap); va_end(ap);
来源：http://hz.guannengcc.top/gtrlyqsqiv.html

[S30] C：头文件保护
来源：http://hz.dashuyun.cn/gtdamlsssh.html

#ifndef X_H
来源：http://hz.0kj1m.cn/gtmlmfawrc.html

#define X_H
来源：http://hz.pengpengdd.cyou/gtodrmhiez.html

#endif
来源：http://hz.yanxiufei.cn/gtanqjjmoo.html

[S31] C++：Hello World
来源：http://hz.shangyingyoupin.top/gtggdfolfj.html

#include <iostream>
来源：http://hz.shanyushiyangtech.top/gtawmuixgs.html

int main() { std::cout << "Hello\n"; }
来源：http://hz.bjfxy.top/gtvjxyfaeo.html

[S32] C++：字符串
来源：http://hz.smart0.xyz/gtuxtrrevb.html

std::string s = "hi";  s += "!";
来源：http://hz.52xcode.cn/gtbrhwgdec.html

[S33] C++：vector 增删
来源：http://hz.yj20258.top/gtnlhwjxba.html

std::vector<int> v{1, 2, 3};  v.push_back(4);
来源：http://hz.haohaochexian.top/gtqyvaccut.html

[S34] C++：遍历 vector
来源：http://hz.zdqjudy.top/gtssuqgdom.html

for (auto &x : v) { std::cout << x; }
来源：http://hz.yj20258888.top/gtfhgrqolr.html

[S35] C++：map
来源：http://hz.c1oappe.top/gtsinmabca.html

std::map<std::string, int> m;  m["a"] = 1;
来源：http://hz.gogol.net.cn/gtrriojvhm.html

[S36] C++：unordered_map
来源：http://hz.hnqzz.top/gtwjimtszd.html

std::unordered_map<std::string, int> m;  m["a"] = 1;
来源：http://hz.chenjidiqi.icu/gtxronlrfg.html

[S37] C++：set
来源：http://hz.shanyushiyangtech.top/gtoibeiagv.html

std::set<int> s{1, 2, 3};  s.insert(4);
来源：http://hz.wangdashe.top/gtnnsslnsq.html

[S38] C++：排序
来源：http://hz.cheryme.top/gtvzgilrdg.html

std::sort(v.begin(), v.end());
来源：http://hz.zhengqikj.top/gtyxuemncv.html

[S39] C++：自定义比较器排序
来源：http://hz.jlsjyb.cn/gtvuddixsy.html

std::sort(v.begin(), v.end(), [](int a, int b) { return a > b; });
来源：http://hz.wangshuangyany.cn/gthofzktbg.html

[S40] C++：查找元素
来源：http://hz.wangdashe.top/gtfowsnlfl.html

auto it = std::find(v.begin(), v.end(), 3);
来源：http://hz.gogol.net.cn/gtbjvpnkez.html

[S41] C++：类与构造函数
来源：http://hz.cucudq.cn/gtwzaefnmu.html

class A { public: A(int v) : x_(v) {} int get() const { return x_; } private: int x_; };
来源：http://hz.pengpengdd.cyou/gtbhqqtcio.html

[S42] C++：继承与虚函数
来源：http://hz.tianlin.xyz/gtycgxtcci.html

class B : public Base { public: void f() override {} };
来源：http://hz.yonumen.top/gtqtudgwzi.html

[S43] C++：智能指针
来源：http://hz.havefunace.top/gtilmxnxhq.html

auto p = std::make_unique<int>(5);
来源：http://hz.sweek.top/gtjwhshzaw.html

[S44] C++：引用传参
来源：http://hz.daria6918.cn/gtqfeqwoak.html

void inc(int &x) { ++x; }
来源：http://hz.316326.xyz/gtnbcazwws.html

[S45] C++：lambda
来源：http://hz.fzhhl.top/gtpvoxaitd.html

auto add = [](int a, int b) { return a + b; };
来源：http://hz.cdnleiting.top/gtujkczztb.html

[S46] C++：函数模板
来源：http://hz.wangdashe.top/gttldufcxw.html

template <typename T> T maxv(T a, T b) { return a > b ? a : b; }
来源：http://hz.shangyingyoupin.top/gtvtmqtvia.html

[S47] C++：结构化绑定遍历
来源：http://hz.daria6918.cn/gtvbwbqguq.html

for (const auto &[k, v] : m) { std::cout << k << v; }
来源：http://hz.aibaodan.cn/gtkcqryqlh.html

[S48] C++：逐行读文件
来源：http://hz.quarkkingdee.top/gtnenfqmjd.html

std::ifstream in("a.txt");  std::string line;
来源：http://hz.9152youxi.cn/gtfmktmstt.html

while (std::getline(in, line)) { }
来源：http://hz.birdmap.top/gteeuywvmv.html

[S49] C++：写文件
来源：http://hz.daxiang520.top/gtofuhynqy.html

std::ofstream out("a.txt");  out << "hi\n";
来源：http://hz.yuanzhike.top/gtbkwrqyvq.html

[S50] C++：格式化数字
来源：http://hz.ybcxt.top/gtoeltdqfh.html

std::ostringstream os;  os << std::fixed << std::setprecision(2) << 3.14159;
来源：http://hz.dashuyun.cn/gtutexbkqr.html

[S51] C++：显式类型转换
来源：http://hz.guowangkeji.top/gttdgkbbja.html

static_cast<double>(a) / b
来源：http://hz.zhengqikj.top/gtdnnpsojs.html

[S52] C++：const 与 noexcept
来源：http://hz.haohaochexian.top/gtefpyugej.html

int size() const noexcept { return n_; }
来源：http://hz.zhixingplan.top/gtjtrviuzt.html

[S53] C++：移动语义
来源：http://hz.wangshuangyany.cn/gthomyytth.html

std::vector<int> w = std::move(v);
来源：http://hz.cheryme.top/gtmmfmlywk.html

[S54] C++：异常处理
来源：http://hz.c1oappe.top/gtwpuycbkf.html

try { throw std::runtime_error("x"); } catch (const std::exception &e) { }
来源：http://hz.meibo888.top/gtlmhmryvh.html

[S55] C++：结构化绑定
来源：http://hz.nanxuanxn.top/gtzelyhczd.html

auto [a, b] = std::make_pair(1, 2);
来源：http://hz.zhongyouzk.top/gtqtmkgkcs.html

[S56] C++：optional
来源：http://hz.quarkkingdee.top/gtlitihdjm.html

std::optional<int> o = 5;  if (o) { int v = *o; }
来源：http://hz.zhixingplan.top/gtbwozbhbb.html

[S57] C++：编译期常量
来源：http://hz.cheryme.top/gtjpykvuba.html

constexpr int N = 10;
来源：http://hz.jinyuanbaomall.cn/gtzxlvrxrp.html

[S58] C++：命名空间
来源：http://hz.aizwys.cn/gtkxrtnacz.html

namespace ns { int f() { return 1; } }
来源：http://hz.jiagoushi.top/gtcabzckew.html

[S59] C++：静态断言
来源：http://hz.xuanzx.com/gtmksqmyyc.html

static_assert(sizeof(int) == 4, "int 必须 4 字节");
来源：http://hz.shzxlz.cn/gtijztilbz.html

[S60] C++：遍历并删除元素
来源：http://hz.kuanghao11.cn/gtojtxptoq.html

v.erase(std::remove_if(v.begin(), v.end(), [](int x) { return x < 0; }), v.end());
来源：http://hz.tanke756.top/gtewnkzrsz.html

================================================================================
来源：http://hz.yvedp.cn/gtcgsmfjmy.html

T. 其他语言补充（Kotlin / Swift / Lua / Perl / Scala）
来源：http://hz.yj202588.top/gtkubfflyy.html

================================================================================
来源：http://hz.jqgufenzy.top/gtlohloxjc.html

[T01] Kotlin：Hello World
来源：http://hz.xziqi.cn/gtkoovkhnf.html

println("Hello")
来源：http://hz.snrcjt.cn/gtstwttcas.html

[T02] Kotlin：变量
来源：http://hz.nwbrower.top/gtrfojphch.html

val a = 1;  var b = 2        // val 只读，var 可变
来源：http://hz.yangfankeji.com/gtpkgowkum.html

[T03] Kotlin：字符串模板
来源：http://hz.zhaomingkeji.xyz/gtcjkzfpne.html

"值: $b"
来源：http://hz.jianghu66.top/gtzdwdnneq.html

[T04] Kotlin：空安全
来源：http://hz.meibo888.top/gtcpohrhhu.html

val n: String? = null;  n?.length
来源：http://hz.daxiang520.top/gtlehbzdxn.html

[T05] Kotlin：when 表达式
来源：http://hz.sufxvd.cn/gtggvsnrno.html

val s = when (x) { 1 -> "一" else -> "其他" }   // 多分支时每个分支单独一行
来源：http://hz.jinqigfzy.top/gtkxvzmuei.html

[T06] Kotlin：集合映射
来源：http://hz.redwolf501.top/gtjqpcenku.html

listOf(1, 2, 3).map { it * 2 }
来源：http://hz.c1oappe.top/gtmoqftmzl.html

[T07] Kotlin：集合过滤
来源：http://hz.ydzc1.top/gtwxeguagm.html

listOf(1, 2, 3).filter { it > 1 }
来源：http://hz.wangshuangyany.cn/gtjhsnvjnp.html

[T08] Kotlin：数据类
来源：http://hz.shzxlz.cn/gtgdttgvot.html

data class User(val name: String, val age: Int)
来源：http://hz.smart0.xyz/gtuamonqyf.html

[T09] Kotlin：扩展函数
来源：http://hz.daxiang520.top/gtnlmvraen.html

fun String.exclaim() = this + "!"
来源：http://hz.zhiwuduotai.top/gtrcrxfwvy.html

[T10] Kotlin：默认参数
来源：http://hz.shangyingyoupin.top/gtandjpnmx.html

fun greet(name: String = "World") = "Hi $name"
来源：http://hz.jiagoushi.top/gtxrslhojw.html

[T11] Kotlin：协程
来源：http://hz.c1oappe.top/gtgvoessfm.html

GlobalScope.launch { delay(1000); println("done") }
来源：http://hz.zhiwuduotai.top/gtddvibkyn.html

[T12] Kotlin：解构声明
来源：http://hz.zycfv.cn/gtftmqavfy.html

val (a, b) = Pair(1, 2)
来源：http://hz.smart0.xyz/gtwnbuteos.html

[T13] Kotlin：只读 Map
来源：http://hz.kuanghao11.cn/gtfeddtlsi.html

val m = mapOf("a" to 1)
来源：http://hz.nanxinkj.top/gtepgpnthl.html

[T14] Kotlin：循环
来源：http://hz.yanxiufei.cn/gtziixbvto.html

for (i in 1..10) println(i)
来源：http://hz.iojbl.cn/gtsjpqhfaw.html

[T15] Kotlin：接口
来源：http://hz.cashguo.top/gtviyasszw.html

interface Shape { fun area(): Double }
来源：http://hz.cucudq.cn/gtbjcstfcy.html

[T16] Swift：Hello World
来源：http://hz.ivvv.top/gttyfurtwt.html

print("Hello")
来源：http://hz.redwolf501.top/gtxndlwkba.html

[T17] Swift：变量与常量
来源：http://hz.aibaodan.cn/gtfbyoddek.html

var a = 1;  let b = 2
来源：http://hz.zhoulong.xyz/gtrkrpwfgf.html

[T18] Swift：字符串插值
来源：http://hz.zdqjudy.top/gtdlicufcq.html

"值: \(b)"
来源：http://hz.xingfuxueyuan.xyz/gtlsumwrlk.html

[T19] Swift：可选绑定
来源：http://hz.dashuyun.cn/gtoghrtfsf.html

if let n = opt { print(n) }
来源：http://hz.havefunace.top/gtlczxrkrz.html

[T20] Swift：数组操作
来源：http://hz.aizwys.cn/gtkywnpvgp.html

var a = [1, 2, 3];  a.append(4)
来源：http://hz.daxiang520.top/gtyhumozov.html

[T21] Swift：遍历
来源：http://hz.cucudq.cn/gtvfdcicih.html

for x in a { print(x) }
来源：http://hz.sufxvd.cn/gtitfobtsf.html

[T22] Swift：字典
来源：http://hz.jinqigufen.top/gtalkvvyab.html

var d = ["a": 1];  d["b"] = 2
来源：http://hz.snrcjt.cn/gtypivaake.html

[T23] Swift：函数
来源：http://hz.zhaomingkeji.xyz/gtnwvxywvb.html

func add(_ a: Int, _ b: Int) -> Int { a + b }
来源：http://hz.zhaomingkeji.xyz/gtsxndywvk.html

[T24] Swift：闭包
来源：http://hz.zhiwuduotai.top/gtfgwbjlhs.html

let f = { (x: Int) -> Int in x * 2 }
来源：http://hz.0kj1m.cn/gtiwmemrev.html

[T25] Swift：结构体
来源：http://hz.shanyushiyangtech.top/gtqpisdesb.html

struct P { var x: Int }
来源：http://hz.cdnleiting.top/gtqpfknthl.html

[T26] Swift：类与重写
来源：http://hz.nanxinkj.top/gtqbrwpgli.html

class A: Base { override func f() {} }
来源：http://hz.sxryk.cn/gtcfofvubf.html

[T27] Swift：错误处理
来源：http://hz.snrcjt.cn/gttumjvybz.html

do { try f() } catch { print(error) }
来源：http://hz.gzhubu.top/gtgqlmgdxq.html

[T28] Swift：枚举
来源：http://hz.kuanghao11.cn/gtetenixce.html

enum Color { case red, green }
来源：http://hz.chenjidiqi.icu/gtdpypfhgs.html

[T29] Swift：guard 提前返回
来源：http://hz.aizwys.cn/gtorddsmfd.html

guard let x = opt else { return }
来源：http://hz.yueranfly.top/gtpmpiglmv.html

[T30] Swift：协议
来源：http://hz.ppjwa.cn/gtvfbqrrzs.html

protocol Shape { func area() -> Double }
来源：http://hz.cucudq.cn/gtzulmgxru.html

[T31] Lua：Hello World
来源：http://hz.316326.xyz/gttamflxtp.html

print("Hello")
来源：http://hz.chenjidiqi.icu/gtabshoyfv.html

[T32] Lua：局部变量
来源：http://hz.svipenyu.cn/gtzfazkmdm.html

local a = 1
来源：http://hz.hysaishi.cn/gtxtoffwir.html

[T33] Lua：表（数组）
来源：http://hz.sxryk.cn/gtcivnmofi.html

local t = {1, 2, 3};  t[4] = 4
来源：http://hz.wangshuangyany.cn/gtqbrgtyaa.html

[T34] Lua：遍历表
来源：http://hz.hnqzz.top/gtrtcwzsuy.html

for i, v in ipairs(t) do print(i, v) end
来源：http://hz.ybcxt.top/gtpiakssns.html

[T35] Lua：字典表
来源：http://hz.ehwqpu.com/gtbzwcyszc.html

local d = { a = 1 };  d.b = 2
来源：http://hz.guannengcc.top/gtiwhvzzlk.html

[T36] Lua：函数
来源：http://hz.ivvv.top/gtofxoytdl.html

function add(a, b) return a + b end
来源：http://hz.gotoacloud.top/gtddrxojrf.html

[T37] Lua：字符串拼接
来源：http://hz.aibaodan.cn/gtzcczpekl.html

"a" .. "b"
来源：http://hz.nanxuanxn.top/gtnwzvrnqj.html

[T38] Lua：条件
来源：http://hz.sufxvd.cn/gticfojetf.html

if x > 0 then print("正") end
来源：http://hz.zhongyouzk.top/gtufkitrsq.html

[T39] Lua：模式匹配
来源：http://hz.ydzc1.top/gtjsbayoch.html

string.find(s, "%d+")
来源：http://hz.wangdashe.top/gtxidcagvt.html

[T40] Lua：元表
来源：http://hz.vqdsnc.cn/gtbcmwjezl.html

setmetatable({}, { __index = base })
来源：http://hz.xuetiantiany.cn/gtdkqizbxy.html

[T41] Perl：Hello World
来源：http://hz.sweek.top/gtlvufaykq.html

print "Hello\n";
来源：http://hz.cdnleiting.top/gtwvzuarlw.html

[T42] Perl：变量类型
来源：http://hz.dashuyun.cn/gtarnsgfqz.html

my $a = 1;  my @arr = (1, 2, 3);  my %h = (a => 1);
来源：http://hz.yanxiufei.cn/gtpnxpbboj.html

[T43] Perl：字符串插值
来源：http://hz.fengsongda.top/gtljgkwtln.html

"值: $a"
来源：http://hz.52xcode.cn/gtbtyoleud.html

[T44] Perl：条件
来源：http://hz.fengsongda.top/gtwfdvfhja.html

if ($a > 0) { print "正"; }
来源：http://hz.bjfxy.top/gtqmpyrgkp.html

[T45] Perl：数组遍历
来源：http://hz.guowangkeji.top/gttwdgyeis.html

for my $x (@arr) { print $x; }
来源：http://hz.dashuyun.cn/gtyajzyiod.html

[T46] Perl：哈希操作
来源：http://hz.zycfv.cn/gtmpvdbyes.html

$h{b} = 2;  for my $k (keys %h) { print "$k=$h{$k}"; }
来源：http://hz.kuanghao11.cn/gtrbiahbtw.html

[T47] Perl：正则捕获
来源：http://hz.yanxiufei.cn/gttxzbzbcc.html

if ($s =~ /(\d+)/) { print $1; }
来源：http://hz.zhongyouzk.top/gtjnnobbwi.html

[T48] Perl：正则替换
来源：http://hz.yongpay.top/gtzpafvpve.html

$s =~ s/old/new/g;
来源：http://hz.yanxiufei.cn/gtnxvegbyb.html

[T49] Perl：函数
来源：http://hz.ydjk.org.cn/gtnlixxamv.html

sub add { my ($a, $b) = @_; return $a + $b; }
来源：http://hz.nanxuanxn.top/gtbckhdmfc.html

[T50] Perl：逐行读文件
来源：http://hz.sysykeji.top/gthekvdxff.html

open my $fh, "<", "a.txt" or die $!;
来源：http://hz.ydjk.org.cn/gtezueiqxw.html

while (my $line = <$fh>) { print $line; }
来源：http://hz.cucudq.cn/gtgsfebeky.html

[T51] Scala：Hello World
来源：http://hz.dashuyun.cn/gttotvsxtb.html

println("Hello")
来源：http://hz.jinqigfzy.top/gtfsintuqy.html

[T52] Scala：变量
来源：http://hz.hongshengwenyu.top/gtvcatmeth.html

val a = 1;  var b = 2
来源：http://hz.zhijiandao.cn/gtritatjvl.html

[T53] Scala：字符串插值
来源：http://hz.nanxinkj.top/gtihamkttx.html

s"值: $b"
来源：http://hz.yuxming.cn/gthkbxesgc.html

[T54] Scala：集合映射
来源：http://hz.xylfe.cn/gtmhuskxms.html

List(1, 2, 3).map(_ * 2)
来源：http://hz.hywenlv.cn/gtffmqizws.html

[T55] Scala：集合过滤
来源：http://hz.aizwys.cn/gtncdqstvd.html

List(1, 2, 3).filter(_ > 1)
来源：http://hz.jianghu66.top/gtkdyonvkg.html

[T56] Scala：样例类
来源：http://hz.c1oappe.top/gtyfonqzdy.html

case class User(name: String, age: Int)
来源：http://hz.chenlongwang.top/gtmirhhooh.html

[T57] Scala：模式匹配
来源：http://hz.vqdsnc.cn/gtvcgnsmeq.html

x match { case 1 => "一"; case _ => "其他" }
来源：http://hz.ppjwa.cn/gtolznjllo.html

[T58] Scala：函数定义
来源：http://hz.zycfv.cn/gtbpkbuycs.html

def add(a: Int, b: Int): Int = a + b
来源：http://hz.fzhhl.top/gthafkikfq.html

[T59] Scala：循环
来源：http://hz.ydjk.org.cn/gtswffqpud.html

for (i <- 1 to 10) println(i)
来源：http://hz.yueranfly.top/gtvcuugnai.html

[T60] Scala：折叠
来源：http://hz.cashguo.top/gtojjtqamp.html

List(1, 2, 3).foldLeft(0)(_ + _)
来源：http://hz.fzhhl.top/gtypfmeqss.html

================================================================================
来源：http://hz.ybcxt.top/gttcfyxehh.html

U. 高频实用片段（Python / PHP / JavaScript 各 40 条）
来源：http://hz.aizwys.cn/gtsvgatvvh.html

================================================================================
来源：http://hz.ydjk.org.cn/gtaezoswio.html

[U01] Py：创建虚拟环境
来源：http://hz.xziqi.cn/gtyxqpktkq.html

python -m venv .venv && source .venv/bin/activate
来源：http://hz.guowangkeji.top/gtmjhjvwwi.html

[U02] Py：导出 / 安装依赖
来源：http://hz.hongshengwenyu.top/gtqjtfbypq.html

pip freeze > requirements.txt;  pip install -r requirements.txt
来源：http://hz.daxiang520.top/gtsskgyrqv.html

[U03] Py：加载 .env 配置
来源：http://hz.guowangkeji.top/gtwoxhwjrn.html

from dotenv import load_dotenv; load_dotenv()
来源：http://hz.yongpay.top/gttchjkyrn.html

[U04] Py：变量调试打印
来源：http://hz.aibaodan.cn/gtsjlfumny.html

print(f"{x=}")            # 输出 x=值，Python 3.8+
来源：http://hz.sweek.top/gtrijevdtu.html

[U05] Py：列表去重且保序
来源：http://hz.ydjk.org.cn/gtshvbkimy.html

list(dict.fromkeys(arr))
来源：http://hz.ehwqpu.com/gtzuwxbvhd.html

[U06] Py：合并两个字典
来源：http://hz.meibo888.top/gtvmfckyue.html

{**a, **b}
来源：http://hz.quarkkingdee.top/gtoanodixs.html

[U07] Py：反转字典键值
来源：http://hz.haohaochexian.top/gtvakzbavo.html

{v: k for k, v in d.items()}
来源：http://hz.zhijiandao.cn/gtrivvmdok.html

[U08] Py：展平二维列表
来源：http://hz.xinyue.icu/gtydsxapbn.html

[y for x in nested for y in x]
来源：http://hz.yongpay.top/gtwefhfzsf.html

[U09] Py：字典取最大值的键
来源：http://hz.9152youxi.cn/gtzajbpupb.html

max(d, key=d.get)
来源：http://hz.shanyushiyangkeji.top/gtxlbladpq.html

[U10] Py：按值排序字典
来源：http://hz.jinqigfzy.top/gttjxxenmh.html

dict(sorted(d.items(), key=lambda kv: kv[1]))
来源：http://hz.dashuyun.cn/gtwudbzwaa.html

[U11] Py：生成器表达式
来源：http://hz.xinyue.icu/gtizvkphya.html

(x * 2 for x in arr)
来源：http://hz.gaohongyu789.top/gtkgayyxnf.html

[U12] Py：取出现最多的 3 个元素
来源：http://hz.gotoacloud.top/gtrlncxouo.html

Counter(arr).most_common(3)
来源：http://hz.sxryk.cn/gtpjzctkqe.html

[U13] Py：固定长度队列
来源：http://hz.ehwqpu.com/gtpwmvlmjh.html

deque(maxlen=10)
来源：http://hz.smart0.xyz/gtcvlhobne.html

[U14] Py：分组收集到列表
来源：http://hz.guowangkeji.top/gtlkxygvjv.html

defaultdict(list)
来源：http://hz.gogol.net.cn/gtimtbjmjc.html

[U15] Py：高精度计时
来源：http://hz.ehwqpu.com/gtgomfpeor.html

t = time.perf_counter()
来源：http://hz.gogol.net.cn/gthvccmgww.html

[U16] Py：命令行参数解析
来源：http://hz.zhengqikj.top/gtwgjmnggr.html

ap = argparse.ArgumentParser();  ap.add_argument("--name");  args = ap.parse_args()
来源：http://hz.dashuyun.cn/gtydspqgnl.html

[U17] Py：初始化日志
来源：http://hz.yj20258888.top/gtlhqehwcc.html

logging.basicConfig(level=logging.INFO)
来源：http://hz.haohaochexian.top/gtelugjycx.html

[U18] Py：预编译正则
来源：http://hz.tian-w.cn/gtmbqcxgdw.html

pat = re.compile(r"\d+")
来源：http://hz.hammf.cn/gtkxmjqryr.html

[U19] Py：正则替换带回调
来源：http://hz.hnqzz.top/gtnrphklgt.html

re.sub(r"\d+", lambda m: str(int(m.group()) * 2), s)
来源：http://hz.cucudq.cn/gtnwywsxod.html

[U20] Py：缓存函数结果
来源：http://hz.yj202588.top/gtnokrbzud.html

@functools.lru_cache(maxsize=None)
来源：http://hz.fengsongda.top/gtcvimpvai.html

[U21] Py：自定义上下文管理器
来源：http://hz.zdqjudy.top/gtmgncbphq.html

@contextlib.contextmanager
来源：http://hz.jinqigufen.top/gthbzoqscn.html

[U22] Py：矩阵转置
来源：http://hz.ppjwa.cn/gtiyplgbig.html

list(zip(*m))
来源：http://hz.shangyingyoupin.top/gtpxrzlcgk.html

[U23] Py：分块读取大文件
来源：http://hz.fzhhl.top/gteszkbjvl.html

for chunk in iter(lambda: f.read(8192), b""):
来源：http://hz.gaohongyu789.top/gtlsnkvguh.html

[U24] Py：路径操作
来源：http://hz.yonumen.top/gtwlqblsqc.html

Path("a/b.txt").parent.mkdir(parents=True, exist_ok=True)
来源：http://hz.gogol.net.cn/gtyqbxhzha.html

[U25] Py：CSV 按字典读
来源：http://hz.ehwqpu.com/gtbrcxxszl.html

csv.DictReader(f)
来源：http://hz.jlsjyb.cn/gtlbkeitxc.html

[U26] Py：并发下载
来源：http://hz.xylfe.cn/gtqinnxtei.html

ThreadPoolExecutor(max_workers=8).map(fetch, urls)
来源：http://hz.dashuyun.cn/gtwdgkohkc.html

[U27] Py：异步 HTTP
来源：http://hz.tanke756.top/gthwzpxngi.html

aiohttp.ClientSession() 配合 async with
来源：http://hz.chenjidiqi.icu/gtaetzuaut.html

[U28] Py：类型别名
来源：http://hz.xuanzx.com/gtktszzqeg.html

UserId = int
来源：http://hz.dashuyun.cn/gtpbrxeavp.html

[U29] Py：属性校验
来源：http://hz.zhiwuduotai.top/gtluqumqbw.html

@property 与 @x.setter 配合
来源：http://hz.cashguo.top/gteizjuwdy.html

[U30] Py：数据类
来源：http://hz.bjfxy.top/gtujgccxlp.html

@dataclass(slots=True)
来源：http://hz.wangshuangyany.cn/gtnbuzsknz.html

[U31] Py：单测
来源：http://hz.birdmap.top/gtxlmcvcgf.html

python -m pytest -q
来源：http://hz.nwbrower.top/gtmfftbmaw.html

[U32] Py：代码格式化
来源：http://hz.guannengcc.top/gtcwurqkht.html

ruff format . && ruff check --fix .
来源：http://hz.ybcxt.top/gtnbcnzzdw.html

[U33] Py：打包发布
来源：http://hz.chenzaomai.com/gtjswsjevl.html

python -m build  （依赖 pyproject.toml）
来源：http://hz.xuetiantiany.cn/gthruorukd.html

[U34] Py：判断编码
来源：http://hz.daria6918.cn/gtaddedbfn.html

chardet.detect(raw)
来源：http://hz.zhoulong.xyz/gtpndxppcq.html

[U35] Py：发送邮件
来源：http://hz.hnqzz.top/gtavnzhzyr.html

smtplib.SMTP_SSL(...).send_message(msg)
来源：http://hz.ywan-chungtsiang.top/gthjkfbogl.html

[U36] Py：定时任务
来源：http://hz.fzhhl.top/gtgxntvrkh.html

schedule.every(10).minutes.do(job)
来源：http://hz.yonumen.top/gturfaebma.html

[U37] Py：读写 Excel
来源：http://hz.shangyingyoupin.top/gtxbcaabbn.html

pandas.read_excel / DataFrame.to_excel
来源：http://hz.jinqigufen.top/gtcdggnjfh.html

[U38] Py：获取脚本所在目录
来源：http://hz.hnxiangtu.top/gtxngfenun.html

Path(__file__).resolve().parent
来源：http://hz.9152youxi.cn/gtnqmscwjj.html

[U39] Py：判断是否在交互环境
来源：http://hz.hfpthk.cn/gtbggkzkvy.html

sys.stdout.isatty()
来源：http://hz.xuanzx.com/gtwxjlsism.html

[U40] Py：打印到标准错误
来源：http://hz.zhongyouzk.top/gtprpvyxsy.html

print("err", file=sys.stderr)
来源：http://hz.tianlin.xyz/gtlbptclol.html

[U41] PHP：初始化 Composer 项目
来源：http://hz.snrcjt.cn/gtlheamomy.html

composer init;  composer require guzzlehttp/guzzle
来源：http://hz.dashuyun.cn/gtyjgptrlw.html

[U42] PHP：PSR-4 自动加载
来源：http://hz.shuidangran.top/gtiqrdhgty.html

"autoload": { "psr-4": { "App\\": "src/" } }
来源：http://hz.mhx1999.top/gtkdtpghlo.html

[U43] PHP：声明命名空间
来源：http://hz.hammf.cn/gtmwauvkzn.html

namespace App\Http;
来源：http://hz.aibaodan.cn/gtzcxaynkl.html

[U44] PHP：开启严格类型
来源：http://hz.nanxinkj.top/gtsfbpbpvb.html

declare(strict_types=1);
来源：http://hz.shangyingyoupin.top/gtsjqmkldb.html


<!-- 参考信息 -->