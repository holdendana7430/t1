代发 wailian999

atoi("42");  strtod("3.14", NULL);
来源：http://hz.nwbrower.top/gtpaimdlpy.html

[S23] C：随机数
来源：http://hz.yonumen.top/gtweicsteb.html

srand(time(NULL));  int r = rand() % 100;
来源：http://hz.zhongyouzk.top/gtvmksblnw.html

[S24] C：获取本地时间
来源：http://hz.tanke756.top/gtimhmsgse.html

time_t t = time(NULL);  struct tm *tm = localtime(&t);
来源：http://hz.c1oappe.top/gtuzxwgaoo.html

[S25] C：内存拷贝
来源：http://hz.nanxuanxn.top/gtuzmjgwui.html

memcpy(dst, src, n);
来源：http://hz.birdmap.top/gthgschcvc.html

[S26] C：内存清零
来源：http://hz.316326.xyz/gtpzokifgj.html

memset(a, 0, sizeof a);
来源：http://hz.sufxvd.cn/gtnaususou.html

[S27] C：定义常量
来源：http://hz.jiagoushi.top/gtgwavdkfh.html

const double PI = 3.14159;
来源：http://hz.redwolf501.top/gtggdwcccc.html

[S28] C：静态变量
来源：http://hz.ydzc1.top/gtjijxrvck.html

static int counter = 0;
来源：http://hz.zhoulong.xyz/gtfhxthqgi.html

[S29] C：变参函数
来源：http://hz.yonumen.top/gthxcflvws.html

va_list ap; va_start(ap, fmt); vprintf(fmt, ap); va_end(ap);
来源：http://hz.guowangkeji.top/gtdwelilzv.html

[S30] C：头文件保护
来源：http://hz.shanyushiyangtech.top/gtcjbvnqga.html

#ifndef X_H
来源：http://hz.chenjidiqi.icu/gtljzdsglv.html

#define X_H
来源：http://hz.zhongyouzk.top/gtxxkrudkh.html

#endif
来源：http://hz.yanxiufei.cn/gtlkqgynov.html

[S31] C++：Hello World
来源：http://hz.jyoumei.cn/gtvfjyceay.html

#include <iostream>
来源：http://hz.zhoulong.xyz/gtqmpjnkib.html

int main() { std::cout << "Hello\n"; }
来源：http://hz.havefunace.top/gtoxrbibul.html

[S32] C++：字符串
来源：http://hz.chenlongwang.top/gtpopynlgv.html

std::string s = "hi";  s += "!";
来源：http://hz.jinqigufen.top/gtoydemwyz.html

[S33] C++：vector 增删
来源：http://hz.iojbl.cn/gtkhahadba.html

std::vector<int> v{1, 2, 3};  v.push_back(4);
来源：http://hz.vqdsnc.cn/gtbbuuxwsy.html

[S34] C++：遍历 vector
来源：http://hz.birdmap.top/gtyknhofnm.html

for (auto &x : v) { std::cout << x; }
来源：http://hz.snrcjt.cn/gtzkokjyxi.html

[S35] C++：map
来源：http://hz.ydjk.org.cn/gtycwczqhc.html

std::map<std::string, int> m;  m["a"] = 1;
来源：http://hz.cdnleiting.top/gthindpiks.html

[S36] C++：unordered_map
来源：http://hz.gotoacloud.top/gtdpoaqrqr.html

std::unordered_map<std::string, int> m;  m["a"] = 1;
来源：http://hz.yj20258.top/gtzsowrguo.html

[S37] C++：set
来源：http://hz.jyoumei.cn/gtptzqabbo.html

std::set<int> s{1, 2, 3};  s.insert(4);
来源：http://hz.ydzc1.top/gtvncwxdxj.html

[S38] C++：排序
来源：http://hz.yonumen.top/gtnhjeoswq.html

std::sort(v.begin(), v.end());
来源：http://hz.52xcode.cn/gtpiucwntz.html

[S39] C++：自定义比较器排序
来源：http://hz.hongshengwenyu.top/gtymbbxyvh.html

std::sort(v.begin(), v.end(), [](int a, int b) { return a > b; });
来源：http://hz.nanxuanxn.top/gttjslbbqk.html

[S40] C++：查找元素
来源：http://hz.gzhubu.top/gtihatraaz.html

auto it = std::find(v.begin(), v.end(), 3);
来源：http://hz.svipenyu.cn/gttwriwpii.html

[S41] C++：类与构造函数
来源：http://hz.quarkkingdee.top/gtfxxqxgmq.html

class A { public: A(int v) : x_(v) {} int get() const { return x_; } private: int x_; };
来源：http://hz.daria6918.cn/gtyjomdtjl.html

[S42] C++：继承与虚函数
来源：http://hz.yangfankeji.com/gtuhfgfqba.html

class B : public Base { public: void f() override {} };
来源：http://hz.cheryme.top/gtxdbvdapp.html

[S43] C++：智能指针
来源：http://hz.0kj1m.cn/gtidrehgtm.html

auto p = std::make_unique<int>(5);
来源：http://hz.zycfv.cn/gteyzfcsie.html

[S44] C++：引用传参
来源：http://hz.ywan-chungtsiang.top/gtgqgsumso.html

void inc(int &x) { ++x; }
来源：http://hz.aibaodan.cn/gtondmqwcr.html

[S45] C++：lambda
来源：http://hz.cashguo.top/gtfsdgffsn.html

auto add = [](int a, int b) { return a + b; };
来源：http://hz.jinqigufen.top/gtruxxdsrj.html

[S46] C++：函数模板
来源：http://hz.sufxvd.cn/gtppwiofyp.html

template <typename T> T maxv(T a, T b) { return a > b ? a : b; }
来源：http://hz.jiagoushi.top/gtncqrlxlu.html

[S47] C++：结构化绑定遍历
来源：http://hz.nanxinkj.top/gtngdbveez.html

for (const auto &[k, v] : m) { std::cout << k << v; }
来源：http://hz.xinyue.icu/gtwmcmanga.html

[S48] C++：逐行读文件
来源：http://hz.cheryme.top/gtzgaxutzd.html

std::ifstream in("a.txt");  std::string line;
来源：http://hz.zhaomingkeji.xyz/gthtzjulda.html

while (std::getline(in, line)) { }
来源：http://hz.yj20258.top/gtsalfussp.html

[S49] C++：写文件
来源：http://hz.gaohongyu789.top/gtzdbajxjt.html

std::ofstream out("a.txt");  out << "hi\n";
来源：http://hz.ybcxt.top/gtdfhqqlyz.html

[S50] C++：格式化数字
来源：http://hz.yj20258.top/gtazihnnis.html

std::ostringstream os;  os << std::fixed << std::setprecision(2) << 3.14159;
来源：http://hz.iojbl.cn/gtwwfahope.html

[S51] C++：显式类型转换
来源：http://hz.ywan-chungtsiang.top/gtjlbuazeh.html

static_cast<double>(a) / b
来源：http://hz.nanxinkj.top/gtogsacfse.html

[S52] C++：const 与 noexcept
来源：http://hz.pengpengdd.cyou/gtqmadoywg.html

int size() const noexcept { return n_; }
来源：http://hz.cashguo.top/gtymsmjwpn.html

[S53] C++：移动语义
来源：http://hz.haohaochexian.top/gtpegnxznq.html

std::vector<int> w = std::move(v);
来源：http://hz.haohaochexian.top/gtzmnxmadj.html

[S54] C++：异常处理
来源：http://hz.cheryme.top/gtxhxukjsy.html

try { throw std::runtime_error("x"); } catch (const std::exception &e) { }
来源：http://hz.hnqzz.top/gtdwdxawvl.html

[S55] C++：结构化绑定
来源：http://hz.guannengcc.top/gtsolpyqbb.html

auto [a, b] = std::make_pair(1, 2);
来源：http://hz.shuidangran.top/gtqtgwgoqn.html

[S56] C++：optional
来源：http://hz.dianchejie.cn/gtcrocfpsb.html

std::optional<int> o = 5;  if (o) { int v = *o; }
来源：http://hz.nanxuanxn.top/gtijfailqb.html

[S57] C++：编译期常量
来源：http://hz.jianghu66.top/gteqszomkf.html

constexpr int N = 10;
来源：http://hz.nwbrower.top/gtgfotwzef.html

[S58] C++：命名空间
来源：http://hz.jinghuilouyu.cn/gtgbwkbwzt.html

namespace ns { int f() { return 1; } }
来源：http://hz.yuanzhike.top/gtexcmhetg.html

[S59] C++：静态断言
来源：http://hz.9152youxi.cn/gtayncdxoq.html

static_assert(sizeof(int) == 4, "int 必须 4 字节");
来源：http://hz.shuidangran.top/gtidksufgw.html

[S60] C++：遍历并删除元素
来源：http://hz.aibaodan.cn/gtlnrxgchp.html

v.erase(std::remove_if(v.begin(), v.end(), [](int x) { return x < 0; }), v.end());
来源：http://hz.cqqwz.cn/gtynzhbsmy.html

================================================================================
来源：http://hz.hammf.cn/gtbpgeyjcf.html

T. 其他语言补充（Kotlin / Swift / Lua / Perl / Scala）
来源：http://hz.zhoulong.xyz/gtnllwzqwf.html

================================================================================
来源：http://hz.sysykeji.top/gttcdrivpo.html

[T01] Kotlin：Hello World
来源：http://hz.andypj.xyz/gtfqwrmgtj.html

println("Hello")
来源：http://hz.yueranfly.top/gtyydqylzr.html

[T02] Kotlin：变量
来源：http://hz.aibaodan.cn/gttdcxelvn.html

val a = 1;  var b = 2        // val 只读，var 可变
来源：http://hz.xingfuxueyuan.xyz/gtsqrmnpqn.html

[T03] Kotlin：字符串模板
来源：http://hz.yanxiufei.cn/gtwmiikwfl.html

"值: $b"
来源：http://hz.zycfv.cn/gtniixmgnv.html

[T04] Kotlin：空安全
来源：http://hz.zhoulong.xyz/gtgmpcdtpw.html

val n: String? = null;  n?.length
来源：http://hz.bjfxy.top/gtbrjcelvp.html

[T05] Kotlin：when 表达式
来源：http://hz.chenzaomai.com/gtoalkfpko.html

val s = when (x) { 1 -> "一" else -> "其他" }   // 多分支时每个分支单独一行
来源：http://hz.yongpay.top/gtnqwiftrh.html

[T06] Kotlin：集合映射
来源：http://hz.xylfe.cn/gtqetvzfnq.html

listOf(1, 2, 3).map { it * 2 }
来源：http://hz.dianchejie.cn/gtmzburnaw.html

[T07] Kotlin：集合过滤
来源：http://hz.gogol.net.cn/gthjmxkzrj.html

listOf(1, 2, 3).filter { it > 1 }
来源：http://hz.yvedp.cn/gtilffihsu.html

[T08] Kotlin：数据类
来源：http://hz.guowangkeji.top/gtcfhoscqx.html

data class User(val name: String, val age: Int)
来源：http://hz.hysaishi.cn/gtqrbsqgzj.html

[T09] Kotlin：扩展函数
来源：http://hz.hfpthk.cn/gtmveauwff.html

fun String.exclaim() = this + "!"
来源：http://hz.gotoacloud.top/gtfqowvcgh.html

[T10] Kotlin：默认参数
来源：http://hz.zdqjudy.top/gtpkexlsjb.html

fun greet(name: String = "World") = "Hi $name"
来源：http://hz.smart0.xyz/gtxrowwcyl.html

[T11] Kotlin：协程
来源：http://hz.andypj.xyz/gtmlstpgaa.html

GlobalScope.launch { delay(1000); println("done") }
来源：http://hz.c1oappe.top/gtnlcfmdrz.html

[T12] Kotlin：解构声明
来源：http://hz.zycfv.cn/gtbkfgbjff.html

val (a, b) = Pair(1, 2)
来源：http://hz.haohaochexian.top/gtzghrmojl.html

[T13] Kotlin：只读 Map
来源：http://hz.shzxlz.cn/gtfzygqvvq.html

val m = mapOf("a" to 1)
来源：http://hz.andypj.xyz/gtkkxqudtm.html

[T14] Kotlin：循环
来源：http://hz.hnxiangtu.top/gtpivxkfso.html

for (i in 1..10) println(i)
来源：http://hz.jiagoushi.top/gtgslytqxp.html

[T15] Kotlin：接口
来源：http://hz.ydjk.org.cn/gtetocjxef.html

interface Shape { fun area(): Double }
来源：http://hz.mhx1999.top/gtwrpejkjo.html

[T16] Swift：Hello World
来源：http://hz.zhijiandao.cn/gtfqlaezjr.html

print("Hello")
来源：http://hz.svipenyu.cn/gtkutwetgl.html

[T17] Swift：变量与常量
来源：http://hz.cdnleiting.top/gtykmrfusq.html

var a = 1;  let b = 2
来源：http://hz.wangdashe.top/gtwnodzhuj.html

[T18] Swift：字符串插值
来源：http://hz.wangshuangyany.cn/gtxcjapggr.html

"值: \(b)"
来源：http://hz.yj20258888.top/gtljqmhmud.html

[T19] Swift：可选绑定
来源：http://hz.yj202588.top/gthxmsbjoe.html

if let n = opt { print(n) }
来源：http://hz.yongpay.top/gtxsavfukt.html

[T20] Swift：数组操作
来源：http://hz.sweek.top/gtzruzxttx.html

var a = [1, 2, 3];  a.append(4)
来源：http://hz.shanyushiyangtech.top/gtgebvwbxg.html

[T21] Swift：遍历
来源：http://hz.haohaochexian.top/gtvbptjnpt.html

for x in a { print(x) }
来源：http://hz.ydjk.org.cn/gtolfvpcyl.html

[T22] Swift：字典
来源：http://hz.dianchejie.cn/gtpqilchlh.html

var d = ["a": 1];  d["b"] = 2
来源：http://hz.guowangkeji.top/gtisxkocff.html

[T23] Swift：函数
来源：http://hz.yongpay.top/gtiyaayuje.html

func add(_ a: Int, _ b: Int) -> Int { a + b }
来源：http://hz.aibaodan.cn/gtdroopnlf.html

[T24] Swift：闭包
来源：http://hz.ybcxt.top/gtiibsqauf.html

let f = { (x: Int) -> Int in x * 2 }
来源：http://hz.cheryme.top/gttyyoessi.html

[T25] Swift：结构体
来源：http://hz.hfpthk.cn/gtkizcqusg.html

struct P { var x: Int }
来源：http://hz.xuanzx.com/gtiaoocyfg.html

[T26] Swift：类与重写
来源：http://hz.ppjwa.cn/gtgbbrljuk.html

class A: Base { override func f() {} }
来源：http://hz.meibo888.top/gtbwxfqihp.html

[T27] Swift：错误处理
来源：http://hz.9152youxi.cn/gtwrzbdfvz.html

do { try f() } catch { print(error) }
来源：http://hz.jqgufenzy.top/gtjspwegdm.html

[T28] Swift：枚举
来源：http://hz.cucudq.cn/gtwdhblelr.html

enum Color { case red, green }
来源：http://hz.52xcode.cn/gtqfujcqbt.html

[T29] Swift：guard 提前返回
来源：http://hz.yj20258.top/gtqdrhacgt.html

guard let x = opt else { return }
来源：http://hz.52xcode.cn/gtoszljopl.html

[T30] Swift：协议
来源：http://hz.sweek.top/gtfnlljvja.html

protocol Shape { func area() -> Double }
来源：http://hz.cqqwz.cn/gtzmyjoxbk.html

[T31] Lua：Hello World
来源：http://hz.zhiwuduotai.top/gtojcpennh.html

print("Hello")
来源：http://hz.gaohongyu789.top/gtqtzmoayd.html

[T32] Lua：局部变量
来源：http://hz.chenlongwang.top/gttzjmydtd.html

local a = 1
来源：http://hz.shanyushiyangkeji.top/gtlqpqwrqo.html

[T33] Lua：表（数组）
来源：http://hz.0kj1m.cn/gtvlhnwvxr.html

local t = {1, 2, 3};  t[4] = 4
来源：http://hz.jinyuanbaomall.cn/gtevynmawx.html

[T34] Lua：遍历表
来源：http://hz.sufxvd.cn/gtinfwlmap.html

for i, v in ipairs(t) do print(i, v) end
来源：http://hz.zhongyouzk.top/gtcazjgxyq.html

[T35] Lua：字典表
来源：http://hz.cashguo.top/gtlxzqsbsi.html

local d = { a = 1 };  d.b = 2
来源：http://hz.9152youxi.cn/gtyzvavrwl.html

[T36] Lua：函数
来源：http://hz.zycfv.cn/gtmipcmlhw.html

function add(a, b) return a + b end
来源：http://hz.sufxvd.cn/gtacnuunzf.html

[T37] Lua：字符串拼接
来源：http://hz.jlsjyb.cn/gtxvztuteu.html

"a" .. "b"
来源：http://hz.52xcode.cn/gtwzdsyrqy.html

[T38] Lua：条件
来源：http://hz.chenzaomai.com/gtspiulohn.html

if x > 0 then print("正") end
来源：http://hz.nwbrower.top/gtrdwpzkyg.html

[T39] Lua：模式匹配
来源：http://hz.kuanghao11.cn/gtbkwctxwr.html

string.find(s, "%d+")
来源：http://hz.xziqi.cn/gtkpyiwynt.html

[T40] Lua：元表
来源：http://hz.hammf.cn/gtjyvwtqsw.html

setmetatable({}, { __index = base })
来源：http://hz.hywenlv.cn/gtqebxiaxq.html

[T41] Perl：Hello World
来源：http://hz.redwolf501.top/gtokhnatxi.html

print "Hello\n";
来源：http://hz.ydzc1.top/gtdhqvrmle.html

[T42] Perl：变量类型
来源：http://hz.shangyingyoupin.top/gtcjugsdid.html

my $a = 1;  my @arr = (1, 2, 3);  my %h = (a => 1);
来源：http://hz.gogol.net.cn/gtbjfigxob.html

[T43] Perl：字符串插值
来源：http://hz.hnxiangtu.top/gtsgtzvpim.html

"值: $a"
来源：http://hz.jinqigfzy.top/gtsxdxdqox.html

[T44] Perl：条件
来源：http://hz.chenlongwang.top/gtiwffvvih.html

if ($a > 0) { print "正"; }
来源：http://hz.ehwqpu.com/gtmfsslbma.html

[T45] Perl：数组遍历
来源：http://hz.cdnleiting.top/gttxeflqfu.html

for my $x (@arr) { print $x; }
来源：http://hz.yj20258888.top/gtagcjdmgw.html

[T46] Perl：哈希操作
来源：http://hz.daria6918.cn/gtnvkisgcz.html

$h{b} = 2;  for my $k (keys %h) { print "$k=$h{$k}"; }
来源：http://hz.tian-w.cn/gtdavnsmtf.html

[T47] Perl：正则捕获
来源：http://hz.daria6918.cn/gtaucdfvsn.html

if ($s =~ /(\d+)/) { print $1; }
来源：http://hz.yuanzhike.top/gtsiaxjycn.html

[T48] Perl：正则替换
来源：http://hz.yj20258888.top/gtiptwadvj.html

$s =~ s/old/new/g;
来源：http://hz.svipenyu.cn/gtroocabva.html

[T49] Perl：函数
来源：http://hz.aizwys.cn/gtrtzvlibt.html

sub add { my ($a, $b) = @_; return $a + $b; }
来源：http://hz.ehwqpu.com/gtoypftcim.html

[T50] Perl：逐行读文件
来源：http://hz.jinqigufen.top/gtjezdorxo.html

open my $fh, "<", "a.txt" or die $!;
来源：http://hz.fengsongda.top/gtulxmqzrf.html

while (my $line = <$fh>) { print $line; }
来源：http://hz.ppjwa.cn/gtsmixfrvs.html

[T51] Scala：Hello World
来源：http://hz.ywan-chungtsiang.top/gttpbmafks.html

println("Hello")
来源：http://hz.hongshengwenyu.top/gtbveqyooc.html

[T52] Scala：变量
来源：http://hz.guannengcc.top/gtpinvtnnx.html

val a = 1;  var b = 2
来源：http://hz.ehwqpu.com/gtmrokkbhf.html

[T53] Scala：字符串插值
来源：http://hz.chenlongwang.top/gtchqpxqxa.html

s"值: $b"
来源：http://hz.xuanzx.com/gtmaauzhli.html

[T54] Scala：集合映射
来源：http://hz.yuxming.cn/gtkonzeocz.html

List(1, 2, 3).map(_ * 2)
来源：http://hz.ydzc1.top/gtbchvnkua.html

[T55] Scala：集合过滤
来源：http://hz.hongshengwenyu.top/gtmiaszpxm.html

List(1, 2, 3).filter(_ > 1)
来源：http://hz.9152youxi.cn/gtijnaxznb.html

[T56] Scala：样例类
来源：http://hz.cucudq.cn/gttppkbwhn.html

case class User(name: String, age: Int)
来源：http://hz.hywenlv.cn/gtibgcryko.html

[T57] Scala：模式匹配
来源：http://hz.sxryk.cn/gtjblupxae.html

x match { case 1 => "一"; case _ => "其他" }
来源：http://hz.ydjk.org.cn/gtxwjtygxg.html

[T58] Scala：函数定义
来源：http://hz.zhoulong.xyz/gtnbczerux.html

def add(a: Int, b: Int): Int = a + b
来源：http://hz.jinyuanbaomall.cn/gtulcowqke.html

[T59] Scala：循环
来源：http://hz.ybcxt.top/gtrskpblbg.html

for (i <- 1 to 10) println(i)
来源：http://hz.c1oappe.top/gtrtqrdulw.html

[T60] Scala：折叠
来源：http://hz.zhengqikj.top/gtpmtpvuxj.html

List(1, 2, 3).foldLeft(0)(_ + _)
来源：http://hz.jianghu66.top/gtztmvlnaz.html

================================================================================
来源：http://hz.shzxlz.cn/gtyjmrllcu.html

U. 高频实用片段（Python / PHP / JavaScript 各 40 条）
来源：http://hz.mhx1999.top/gteygcxacx.html

================================================================================
来源：http://hz.sufxvd.cn/gtnushbxld.html

[U01] Py：创建虚拟环境
来源：http://hz.kuanghao11.cn/gtpymmeibn.html

python -m venv .venv && source .venv/bin/activate
来源：http://hz.dashuyun.cn/gtzxuvknlj.html

[U02] Py：导出 / 安装依赖
来源：http://hz.hammf.cn/gtgvjxhivc.html

pip freeze > requirements.txt;  pip install -r requirements.txt
来源：http://hz.c1oappe.top/gtoojjfmgj.html

[U03] Py：加载 .env 配置
来源：http://hz.zhaomingkeji.xyz/gtsfmqoqiw.html

from dotenv import load_dotenv; load_dotenv()
来源：http://hz.shanyushiyangtech.top/gtrrltrbih.html

[U04] Py：变量调试打印
来源：http://hz.nanxuanxn.top/gtxpyfwkun.html

print(f"{x=}")            # 输出 x=值，Python 3.8+
来源：http://hz.yanxiufei.cn/gtbiopotzg.html

[U05] Py：列表去重且保序
来源：http://hz.jinyuanbaomall.cn/gtshpssyvi.html

list(dict.fromkeys(arr))
来源：http://hz.nwbrower.top/gtmhzulihr.html

[U06] Py：合并两个字典
来源：http://hz.bjfxy.top/gtdltlekxo.html

{**a, **b}
来源：http://hz.meibo888.top/gtbsumqfcu.html

[U07] Py：反转字典键值
来源：http://hz.zhixingplan.top/gtqvmsplfx.html

{v: k for k, v in d.items()}
来源：http://hz.yj202588.top/gtulzzpjqv.html

[U08] Py：展平二维列表
来源：http://hz.yongpay.top/gtpadglczo.html

[y for x in nested for y in x]
来源：http://hz.hywenlv.cn/gtxwhtsnef.html

[U09] Py：字典取最大值的键
来源：http://hz.ywan-chungtsiang.top/gtwsqrvrda.html

max(d, key=d.get)
来源：http://hz.xingfuxueyuan.xyz/gtzzdvgsft.html

[U10] Py：按值排序字典
来源：http://hz.snrcjt.cn/gttwvkkncm.html

dict(sorted(d.items(), key=lambda kv: kv[1]))
来源：http://hz.tian-w.cn/gtufqeyfxn.html

[U11] Py：生成器表达式
来源：http://hz.dashuyun.cn/gtgeodmnko.html

(x * 2 for x in arr)
来源：http://hz.ybcxt.top/gtoplgbjad.html

[U12] Py：取出现最多的 3 个元素
来源：http://hz.dashuyun.cn/gthdtixpin.html

Counter(arr).most_common(3)
来源：http://hz.chenlongwang.top/gthqwcnsjm.html

[U13] Py：固定长度队列
来源：http://hz.xylfe.cn/gtekzwlhbp.html

deque(maxlen=10)
来源：http://hz.jianghu66.top/gtjssoudgx.html

[U14] Py：分组收集到列表
来源：http://hz.xinyue.icu/gtxagkwxba.html

defaultdict(list)
来源：http://hz.ywan-chungtsiang.top/gtbgftgjbj.html

[U15] Py：高精度计时
来源：http://hz.jinqigfzy.top/gtvhmngfag.html

t = time.perf_counter()
来源：http://hz.gzhubu.top/gtrquvpmwy.html

[U16] Py：命令行参数解析
来源：http://hz.hnxiangtu.top/gtjklzhwuh.html

ap = argparse.ArgumentParser();  ap.add_argument("--name");  args = ap.parse_args()
来源：http://hz.xinyue.icu/gtiluybklm.html

[U17] Py：初始化日志
来源：http://hz.mhx1999.top/gttnigynep.html

logging.basicConfig(level=logging.INFO)
来源：http://hz.zhaomingkeji.xyz/gtzxcaeguh.html

[U18] Py：预编译正则
来源：http://hz.cashguo.top/gtambwzdcf.html

pat = re.compile(r"\d+")
来源：http://hz.ivvv.top/gtaiqwgwvy.html

[U19] Py：正则替换带回调
来源：http://hz.chenzaomai.com/gttqwmbice.html

re.sub(r"\d+", lambda m: str(int(m.group()) * 2), s)
来源：http://hz.nanxinkj.top/gtyumaxwko.html

[U20] Py：缓存函数结果
来源：http://hz.hongshengwenyu.top/gtzbvvxmqd.html

@functools.lru_cache(maxsize=None)
来源：http://hz.zhongyouzk.top/gtmohyvevb.html

[U21] Py：自定义上下文管理器
来源：http://hz.jqgufenzy.top/gtyqqqvynf.html

@contextlib.contextmanager
来源：http://hz.zhoulong.xyz/gtidvhyrou.html

[U22] Py：矩阵转置
来源：http://hz.snrcjt.cn/gtompiumdy.html

list(zip(*m))
来源：http://hz.gaohongyu789.top/gtfkemovqc.html

[U23] Py：分块读取大文件
来源：http://hz.shzxlz.cn/gtfjpkosgd.html

for chunk in iter(lambda: f.read(8192), b""):
来源：http://hz.yongpay.top/gtdyiodfrg.html

[U24] Py：路径操作
来源：http://hz.snrcjt.cn/gtkvusdffn.html

Path("a/b.txt").parent.mkdir(parents=True, exist_ok=True)
来源：http://hz.yj20258888.top/gtmigyojdl.html

[U25] Py：CSV 按字典读
来源：http://hz.svipenyu.cn/gtenvprguz.html

csv.DictReader(f)
来源：http://hz.jinqigufen.top/gteogwskei.html

[U26] Py：并发下载
来源：http://hz.ehwqpu.com/gtosmivvlk.html

ThreadPoolExecutor(max_workers=8).map(fetch, urls)
来源：http://hz.meibo888.top/gtcydggbyf.html

[U27] Py：异步 HTTP
来源：http://hz.yuxming.cn/gteowamzze.html

aiohttp.ClientSession() 配合 async with
来源：http://hz.daxiang520.top/gtvegizdjw.html

[U28] Py：类型别名
来源：http://hz.smart0.xyz/gtqbiievoa.html

UserId = int
来源：http://hz.ivvv.top/gtcxncehtg.html

[U29] Py：属性校验
来源：http://hz.jqgfzy.top/gtsgidsbij.html

@property 与 @x.setter 配合
来源：http://hz.gaohongyu789.top/gtcxkzhkju.html

[U30] Py：数据类
来源：http://hz.aizwys.cn/gtdwajpzoz.html

@dataclass(slots=True)
来源：http://hz.shzxlz.cn/gtmzqfxnrk.html

[U31] Py：单测
来源：http://hz.shanyushiyangtech.top/gtagudrsox.html

python -m pytest -q
来源：http://hz.shzxlz.cn/gtmxavgogn.html

[U32] Py：代码格式化
来源：http://hz.tian-w.cn/gtumfiriyg.html

ruff format . && ruff check --fix .
来源：http://hz.ydzc1.top/gtpkihsell.html

[U33] Py：打包发布
来源：http://hz.fengsongda.top/gtrugkizcn.html

python -m build  （依赖 pyproject.toml）
来源：http://hz.ydzc1.top/gteszweapo.html

[U34] Py：判断编码
来源：http://hz.tianlin.xyz/gtaoipfbxe.html

chardet.detect(raw)
来源：http://hz.sweek.top/gttohpnlfq.html

[U35] Py：发送邮件
来源：http://hz.havefunace.top/gtdybwtvmg.html

smtplib.SMTP_SSL(...).send_message(msg)
来源：http://hz.yonumen.top/gtiqfczzpg.html

[U36] Py：定时任务
来源：http://hz.chenjidiqi.icu/gtlvuqsecn.html

schedule.every(10).minutes.do(job)
来源：http://hz.hnxiangtu.top/gtfyiboath.html

[U37] Py：读写 Excel
来源：http://hz.cdnleiting.top/gthgrvlvsb.html

pandas.read_excel / DataFrame.to_excel
来源：http://hz.hammf.cn/gtngnryobd.html

[U38] Py：获取脚本所在目录
来源：http://hz.cucudq.cn/gtblgveome.html

Path(__file__).resolve().parent
来源：http://hz.shangyingyoupin.top/gtdkwirsdv.html

[U39] Py：判断是否在交互环境
来源：http://hz.sxryk.cn/gtjdzylbxr.html

sys.stdout.isatty()
来源：http://hz.daria6918.cn/gtdcqwlewx.html

[U40] Py：打印到标准错误
来源：http://hz.cdnleiting.top/gtbavazrcy.html

print("err", file=sys.stderr)
来源：http://hz.zycfv.cn/gtvithurrl.html

[U41] PHP：初始化 Composer 项目
来源：http://hz.mhx1999.top/gtiwaxorar.html

composer init;  composer require guzzlehttp/guzzle
来源：http://hz.tian-w.cn/gtjkxbtokw.html

[U42] PHP：PSR-4 自动加载
来源：http://hz.gaohongyu789.top/gtkwhzkjta.html

"autoload": { "psr-4": { "App\\": "src/" } }
来源：http://hz.daria6918.cn/gtzmagewcy.html

[U43] PHP：声明命名空间
来源：http://hz.shanyushiyangkeji.top/gtfnhfhaou.html

namespace App\Http;
来源：http://hz.dianchejie.cn/gtcaywkaau.html

[U44] PHP：开启严格类型
来源：http://hz.chenlongwang.top/gtcyeivbvl.html

declare(strict_types=1);
来源：http://hz.gzhubu.top/gtrpuzwdto.html

[U45] PHP：类型声明与返回类型
来源：http://hz.yangfankeji.com/gtksukrrlj.html

function add(int $a, int $b): int { return $a + $b; }
来源：http://hz.svipenyu.cn/gtlotrvucf.html

[U46] PHP：可空类型
来源：http://hz.xuanzx.com/gtqepoauhk.html

?string $name = null
来源：http://hz.wangdashe.top/gtpwujmlhh.html


<!-- 参考信息 -->