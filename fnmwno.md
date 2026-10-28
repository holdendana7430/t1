代发 wailian999

bsearch(&key, a, n, sizeof(int), cmp);
来源：http://hz.quarkkingdee.top/gthbjqojws.html

[S21] C：字符类别判断
来源：http://hz.cqqwz.cn/gtmxghfinh.html

isdigit(c);  isalpha(c);  isspace(c);
来源：http://hz.jinyuanbaomall.cn/gthnjomqiy.html

[S22] C：字符串转数字
来源：http://hz.cucudq.cn/gtwsgmswta.html

atoi("42");  strtod("3.14", NULL);
来源：http://hz.nwbrower.top/gtwjohlbsh.html

[S23] C：随机数
来源：http://hz.mhx1999.top/gtjizmkdmm.html

srand(time(NULL));  int r = rand() % 100;
来源：http://hz.fengsongda.top/gtsiggnkkp.html

[S24] C：获取本地时间
来源：http://hz.bjfxy.top/gtglkooley.html

time_t t = time(NULL);  struct tm *tm = localtime(&t);
来源：http://hz.fengsongda.top/gtldoykuud.html

[S25] C：内存拷贝
来源：http://hz.chenzaomai.com/gtohtipvlo.html

memcpy(dst, src, n);
来源：http://hz.zycfv.cn/gtubpbjiyi.html

[S26] C：内存清零
来源：http://hz.yj20258.top/gtzxnikxce.html

memset(a, 0, sizeof a);
来源：http://hz.xingfuxueyuan.xyz/gthodxigoo.html

[S27] C：定义常量
来源：http://hz.yueranfly.top/gtpusiqygt.html

const double PI = 3.14159;
来源：http://hz.svipenyu.cn/gthdpejxqy.html

[S28] C：静态变量
来源：http://hz.316326.xyz/gtwglhiicm.html

static int counter = 0;
来源：http://hz.c1oappe.top/gtljntkajy.html

[S29] C：变参函数
来源：http://hz.xinyue.icu/gtijmydbrg.html

va_list ap; va_start(ap, fmt); vprintf(fmt, ap); va_end(ap);
来源：http://hz.yj20258.top/gtbuynhdri.html

[S30] C：头文件保护
来源：http://hz.chenzaomai.com/gtdvkpjjzm.html

#ifndef X_H
来源：http://hz.bjfxy.top/gttukhkrpe.html

#define X_H
来源：http://hz.jianghu66.top/gtarxqivol.html

#endif
来源：http://hz.shuidangran.top/gttntrtlhf.html

[S31] C++：Hello World
来源：http://hz.jyoumei.cn/gtpgaiyqiu.html

#include <iostream>
来源：http://hz.chenlongwang.top/gteegwmswx.html

int main() { std::cout << "Hello\n"; }
来源：http://hz.gzhubu.top/gtsfamccjc.html

[S32] C++：字符串
来源：http://hz.ydjk.org.cn/gtislrmkgd.html

std::string s = "hi";  s += "!";
来源：http://hz.meibo888.top/gtqicahgmn.html

[S33] C++：vector 增删
来源：http://hz.daxiang520.top/gtzvbukdos.html

std::vector<int> v{1, 2, 3};  v.push_back(4);
来源：http://hz.meibo888.top/gtvwtvvtuk.html

[S34] C++：遍历 vector
来源：http://hz.c1oappe.top/gtqyjqafmw.html

for (auto &x : v) { std::cout << x; }
来源：http://hz.gaohongyu789.top/gtpjnlaums.html

[S35] C++：map
来源：http://hz.cheryme.top/gtaceddcpo.html

std::map<std::string, int> m;  m["a"] = 1;
来源：http://hz.gaohongyu789.top/gtdtxmeryh.html

[S36] C++：unordered_map
来源：http://hz.cucudq.cn/gtckqpxlof.html

std::unordered_map<std::string, int> m;  m["a"] = 1;
来源：http://hz.jyoumei.cn/gtszexyfsy.html

[S37] C++：set
来源：http://hz.cdnleiting.top/gtkmaicgom.html

std::set<int> s{1, 2, 3};  s.insert(4);
来源：http://hz.ybcxt.top/gtrnejfgwg.html

[S38] C++：排序
来源：http://hz.havefunace.top/gthoowkhiy.html

std::sort(v.begin(), v.end());
来源：http://hz.cucudq.cn/gtqecqsgbh.html

[S39] C++：自定义比较器排序
来源：http://hz.xylfe.cn/gtaiftnxak.html

std::sort(v.begin(), v.end(), [](int a, int b) { return a > b; });
来源：http://hz.cashguo.top/gtmhfruuoo.html

[S40] C++：查找元素
来源：http://hz.mhx1999.top/gtmersfteh.html

auto it = std::find(v.begin(), v.end(), 3);
来源：http://hz.xingfuxueyuan.xyz/gtdnhbuvnj.html

[S41] C++：类与构造函数
来源：http://hz.jinqigufen.top/gttysaamye.html

class A { public: A(int v) : x_(v) {} int get() const { return x_; } private: int x_; };
来源：http://hz.feifeiyinyue.top/gtqomkrknv.html

[S42] C++：继承与虚函数
来源：http://hz.gotoacloud.top/gtkphowzls.html

class B : public Base { public: void f() override {} };
来源：http://hz.jinqigfzy.top/gtrrcvjnnd.html

[S43] C++：智能指针
来源：http://hz.cqqwz.cn/gtccgpqaml.html

auto p = std::make_unique<int>(5);
来源：http://hz.yj202588.top/gttnxbdbdj.html

[S44] C++：引用传参
来源：http://hz.52xcode.cn/gtoyxwnsns.html

void inc(int &x) { ++x; }
来源：http://hz.c1oappe.top/gtxiyhljem.html

[S45] C++：lambda
来源：http://hz.wangshuangyany.cn/gtnjazsaxq.html

auto add = [](int a, int b) { return a + b; };
来源：http://hz.ydzc1.top/gtasvuqpod.html

[S46] C++：函数模板
来源：http://hz.guannengcc.top/gtgxrqzkms.html

template <typename T> T maxv(T a, T b) { return a > b ? a : b; }
来源：http://hz.ivvv.top/gtnwoeuafb.html

[S47] C++：结构化绑定遍历
来源：http://hz.redwolf501.top/gtyxxqynok.html

for (const auto &[k, v] : m) { std::cout << k << v; }
来源：http://hz.shangyingyoupin.top/gtieolfpmn.html

[S48] C++：逐行读文件
来源：http://hz.ywan-chungtsiang.top/gtszisukle.html

std::ifstream in("a.txt");  std::string line;
来源：http://hz.xziqi.cn/gttrdyzsmr.html

while (std::getline(in, line)) { }
来源：http://hz.shangyingyoupin.top/gtmbricqsy.html

[S49] C++：写文件
来源：http://hz.0kj1m.cn/gthwpsfykl.html

std::ofstream out("a.txt");  out << "hi\n";
来源：http://hz.svipenyu.cn/gtnjsxgnxm.html

[S50] C++：格式化数字
来源：http://hz.shanyushiyangtech.top/gtnqmebjaj.html

std::ostringstream os;  os << std::fixed << std::setprecision(2) << 3.14159;
来源：http://hz.guowangkeji.top/gtjdqtcynp.html

[S51] C++：显式类型转换
来源：http://hz.xingfuxueyuan.xyz/gtfwodjrkx.html

static_cast<double>(a) / b
来源：http://hz.nanxuanxn.top/gtmnuvlmmd.html

[S52] C++：const 与 noexcept
来源：http://hz.zhaomingkeji.xyz/gttkorpvex.html

int size() const noexcept { return n_; }
来源：http://hz.wangshuangyany.cn/gtuqjasirx.html

[S53] C++：移动语义
来源：http://hz.yongpay.top/gtabkbifhx.html

std::vector<int> w = std::move(v);
来源：http://hz.wangdashe.top/gtjiuqmpxh.html

[S54] C++：异常处理
来源：http://hz.zdqjudy.top/gtsgoxawds.html

try { throw std::runtime_error("x"); } catch (const std::exception &e) { }
来源：http://hz.ivvv.top/gtiwdkciks.html

[S55] C++：结构化绑定
来源：http://hz.9152youxi.cn/gtngmmjexe.html

auto [a, b] = std::make_pair(1, 2);
来源：http://hz.hongshengwenyu.top/gtzcksafqn.html

[S56] C++：optional
来源：http://hz.gaohongyu789.top/gtmqgyflqi.html

std::optional<int> o = 5;  if (o) { int v = *o; }
来源：http://hz.jinghuilouyu.cn/gtgnllpbqp.html

[S57] C++：编译期常量
来源：http://hz.zhixingplan.top/gtmaylmpsn.html

constexpr int N = 10;
来源：http://hz.xylfe.cn/gtzfabzmtl.html

[S58] C++：命名空间
来源：http://hz.havefunace.top/gtiwzqnxej.html

namespace ns { int f() { return 1; } }
来源：http://hz.fengsongda.top/gtjzptziga.html

[S59] C++：静态断言
来源：http://hz.sxryk.cn/gtgoxmhqds.html

static_assert(sizeof(int) == 4, "int 必须 4 字节");
来源：http://hz.zhoulong.xyz/gtrxykvenl.html

[S60] C++：遍历并删除元素
来源：http://hz.zhixingplan.top/gtqrzhkvhl.html

v.erase(std::remove_if(v.begin(), v.end(), [](int x) { return x < 0; }), v.end());
来源：http://hz.zhijiandao.cn/gtrdqgafmi.html

================================================================================
来源：http://hz.shangyingyoupin.top/gtdakvtfgs.html

T. 其他语言补充（Kotlin / Swift / Lua / Perl / Scala）
来源：http://hz.zhiwuduotai.top/gtemyxaxka.html

================================================================================
来源：http://hz.havefunace.top/gtugnqhcnz.html

[T01] Kotlin：Hello World
来源：http://hz.fzhhl.top/gtxrskrlzl.html

println("Hello")
来源：http://hz.tian-w.cn/gtonftaduz.html

[T02] Kotlin：变量
来源：http://hz.xylfe.cn/gtuxmvinvv.html

val a = 1;  var b = 2        // val 只读，var 可变
来源：http://hz.haohaochexian.top/gteiqliqyh.html

[T03] Kotlin：字符串模板
来源：http://hz.ehwqpu.com/gtqmeiadjq.html

"值: $b"
来源：http://hz.xingfuxueyuan.xyz/gtsdlrioag.html

[T04] Kotlin：空安全
来源：http://hz.xziqi.cn/gtazyhgafw.html

val n: String? = null;  n?.length
来源：http://hz.cdnleiting.top/gtdplyovwl.html

[T05] Kotlin：when 表达式
来源：http://hz.yueranfly.top/gtjnxrmejy.html

val s = when (x) { 1 -> "一" else -> "其他" }   // 多分支时每个分支单独一行
来源：http://hz.shanyushiyangtech.top/gtsguqezvl.html

[T06] Kotlin：集合映射
来源：http://hz.aizwys.cn/gtscnryfty.html

listOf(1, 2, 3).map { it * 2 }
来源：http://hz.wangshuangyany.cn/gtirckelkx.html

[T07] Kotlin：集合过滤
来源：http://hz.iojbl.cn/gtncgqeadw.html

listOf(1, 2, 3).filter { it > 1 }
来源：http://hz.yangfankeji.com/gtnqphswxh.html

[T08] Kotlin：数据类
来源：http://hz.cashguo.top/gtjakcqryo.html

data class User(val name: String, val age: Int)
来源：http://hz.zhaomingkeji.xyz/gtuyfclneh.html

[T09] Kotlin：扩展函数
来源：http://hz.daria6918.cn/gtyzlavtsx.html

fun String.exclaim() = this + "!"
来源：http://hz.c1oappe.top/gtgcuaakan.html

[T10] Kotlin：默认参数
来源：http://hz.hfpthk.cn/gthfqocsln.html

fun greet(name: String = "World") = "Hi $name"
来源：http://hz.yongpay.top/gtstocuugi.html

[T11] Kotlin：协程
来源：http://hz.316326.xyz/gtwpdzasem.html

GlobalScope.launch { delay(1000); println("done") }
来源：http://hz.hywenlv.cn/gtcdtyxdgo.html

[T12] Kotlin：解构声明
来源：http://hz.dashuyun.cn/gtqztakgsa.html

val (a, b) = Pair(1, 2)
来源：http://hz.nanxinkj.top/gtmsxcvoyz.html

[T13] Kotlin：只读 Map
来源：http://hz.hywenlv.cn/gtkgbsumtw.html

val m = mapOf("a" to 1)
来源：http://hz.nwbrower.top/gtiorwteto.html

[T14] Kotlin：循环
来源：http://hz.sweek.top/gtafyorpnc.html

for (i in 1..10) println(i)
来源：http://hz.sufxvd.cn/gthhzxuuzm.html

[T15] Kotlin：接口
来源：http://hz.jianghu66.top/gtnvlftyau.html

interface Shape { fun area(): Double }
来源：http://hz.ivvv.top/gtmzxkjtya.html

[T16] Swift：Hello World
来源：http://hz.shzxlz.cn/gtymmpndie.html

print("Hello")
来源：http://hz.shanyushiyangkeji.top/gtyhtfhqqe.html

[T17] Swift：变量与常量
来源：http://hz.guannengcc.top/gtipdvfbgx.html

var a = 1;  let b = 2
来源：http://hz.yuanzhike.top/gtghmxwnwk.html

[T18] Swift：字符串插值
来源：http://hz.ydzc1.top/gtlcfuymkf.html

"值: \(b)"
来源：http://hz.xylfe.cn/gttppcinqb.html

[T19] Swift：可选绑定
来源：http://hz.jinghuilouyu.cn/gtgczemxgd.html

if let n = opt { print(n) }
来源：http://hz.sysykeji.top/gtvjxoqkty.html

[T20] Swift：数组操作
来源：http://hz.zhijiandao.cn/gtikafeexs.html

var a = [1, 2, 3];  a.append(4)
来源：http://hz.chenjidiqi.icu/gtvucfwfqt.html

[T21] Swift：遍历
来源：http://hz.xuanzx.com/gtaowfqvuk.html

for x in a { print(x) }
来源：http://hz.dianchejie.cn/gtniwwdpar.html

[T22] Swift：字典
来源：http://hz.jqgufenzy.top/gtsklatfcf.html

var d = ["a": 1];  d["b"] = 2
来源：http://hz.jinqigufen.top/gtfdblldyr.html

[T23] Swift：函数
来源：http://hz.jqgfzy.top/gtegdxrumt.html

func add(_ a: Int, _ b: Int) -> Int { a + b }
来源：http://hz.redwolf501.top/gtpgkxylfg.html

[T24] Swift：闭包
来源：http://hz.ywan-chungtsiang.top/gtqnvivgti.html

let f = { (x: Int) -> Int in x * 2 }
来源：http://hz.xuanzx.com/gtgonhpycp.html

[T25] Swift：结构体
来源：http://hz.ehwqpu.com/gtmwxulost.html

struct P { var x: Int }
来源：http://hz.yuxming.cn/gtamiapuce.html

[T26] Swift：类与重写
来源：http://hz.hfpthk.cn/gtkyzriaqs.html

class A: Base { override func f() {} }
来源：http://hz.shanyushiyangtech.top/gtmuejkozo.html

[T27] Swift：错误处理
来源：http://hz.ivvv.top/gtlgnpbzyq.html

do { try f() } catch { print(error) }
来源：http://hz.hnxiangtu.top/gtcfezptra.html

[T28] Swift：枚举
来源：http://hz.c1oappe.top/gtcdhoabzb.html

enum Color { case red, green }
来源：http://hz.yj20258.top/gtmvkzekoj.html

[T29] Swift：guard 提前返回
来源：http://hz.yj20258.top/gtarffpejy.html

guard let x = opt else { return }
来源：http://hz.xuetiantiany.cn/gtoguigqoz.html

[T30] Swift：协议
来源：http://hz.tian-w.cn/gtxcimyvaj.html

protocol Shape { func area() -> Double }
来源：http://hz.hysaishi.cn/gtzpcqozuz.html

[T31] Lua：Hello World
来源：http://hz.ybcxt.top/gtgaddeecv.html

print("Hello")
来源：http://hz.xylfe.cn/gtefjfxmcp.html

[T32] Lua：局部变量
来源：http://hz.gogol.net.cn/gtbmyuzxor.html

local a = 1
来源：http://hz.shangyingyoupin.top/gtbkmteuwe.html

[T33] Lua：表（数组）
来源：http://hz.jinghuilouyu.cn/gtxsfstyhs.html

local t = {1, 2, 3};  t[4] = 4
来源：http://hz.wangshuangyany.cn/gtduxrqsws.html

[T34] Lua：遍历表
来源：http://hz.guowangkeji.top/gtpztukeda.html

for i, v in ipairs(t) do print(i, v) end
来源：http://hz.tanke756.top/gtdklmdzxe.html

[T35] Lua：字典表
来源：http://hz.chenzaomai.com/gtxlyeblok.html

local d = { a = 1 };  d.b = 2
来源：http://hz.yuanzhike.top/gtnqaquzvh.html

[T36] Lua：函数
来源：http://hz.fzhhl.top/gtevfvhllm.html

function add(a, b) return a + b end
来源：http://hz.zhengqikj.top/gtjvxbyawr.html

[T37] Lua：字符串拼接
来源：http://hz.yuanzhike.top/gtgowgoboh.html

"a" .. "b"
来源：http://hz.meibo888.top/gtnyqaorgp.html

[T38] Lua：条件
来源：http://hz.yvedp.cn/gtnovppnem.html

if x > 0 then print("正") end
来源：http://hz.shanyushiyangtech.top/gtuypyhdpb.html

[T39] Lua：模式匹配
来源：http://hz.shuidangran.top/gtgojnrnln.html

string.find(s, "%d+")
来源：http://hz.jinqigfzy.top/gtyxvicamv.html

[T40] Lua：元表
来源：http://hz.zhiwuduotai.top/gtkllpqlld.html

setmetatable({}, { __index = base })
来源：http://hz.chenjidiqi.icu/gtwnnjdpxb.html

[T41] Perl：Hello World
来源：http://hz.yuanzhike.top/gttkhckdco.html

print "Hello\n";
来源：http://hz.fengsongda.top/gtzmnvupmp.html

[T42] Perl：变量类型
来源：http://hz.zycfv.cn/gtvkyeupud.html

my $a = 1;  my @arr = (1, 2, 3);  my %h = (a => 1);
来源：http://hz.yueranfly.top/gthxdhhxwl.html

[T43] Perl：字符串插值
来源：http://hz.chenjidiqi.icu/gtewhmykzn.html

"值: $a"
来源：http://hz.c1oappe.top/gtnojijale.html

[T44] Perl：条件
来源：http://hz.cqqwz.cn/gtfrsgtrds.html

if ($a > 0) { print "正"; }
来源：http://hz.aibaodan.cn/gtelxissay.html

[T45] Perl：数组遍历
来源：http://hz.hammf.cn/gtdecgstjy.html

for my $x (@arr) { print $x; }
来源：http://hz.yonumen.top/gtztpehrdm.html

[T46] Perl：哈希操作
来源：http://hz.jqgufenzy.top/gtalgwzgxs.html

$h{b} = 2;  for my $k (keys %h) { print "$k=$h{$k}"; }
来源：http://hz.tianlin.xyz/gtjtcpeqqr.html

[T47] Perl：正则捕获
来源：http://hz.nanxuanxn.top/gtdztjzjzw.html

if ($s =~ /(\d+)/) { print $1; }
来源：http://hz.xingfuxueyuan.xyz/gtokserrus.html

[T48] Perl：正则替换
来源：http://hz.bjfxy.top/gtjddsxfca.html

$s =~ s/old/new/g;
来源：http://hz.wangshuangyany.cn/gtoqjbfedr.html

[T49] Perl：函数
来源：http://hz.zhixingplan.top/gtwodbbonq.html

sub add { my ($a, $b) = @_; return $a + $b; }
来源：http://hz.feifeiyinyue.top/gtjbuybsis.html

[T50] Perl：逐行读文件
来源：http://hz.meibo888.top/gtpfhdcmst.html

open my $fh, "<", "a.txt" or die $!;
来源：http://hz.jinghuilouyu.cn/gtskrlbstr.html

while (my $line = <$fh>) { print $line; }
来源：http://hz.tian-w.cn/gtypsedlis.html

[T51] Scala：Hello World
来源：http://hz.jqgufenzy.top/gtsmwlzeve.html

println("Hello")
来源：http://hz.vqdsnc.cn/gtzxfnpddz.html

[T52] Scala：变量
来源：http://hz.ydzc1.top/gtropzdfbm.html

val a = 1;  var b = 2
来源：http://hz.0kj1m.cn/gtavsuxpyy.html

[T53] Scala：字符串插值
来源：http://hz.yongpay.top/gtaulkoghu.html

s"值: $b"
来源：http://hz.316326.xyz/gtwtahqwxr.html

[T54] Scala：集合映射
来源：http://hz.ydzc1.top/gtqmxngdzw.html

List(1, 2, 3).map(_ * 2)
来源：http://hz.yj20258888.top/gtgitexfet.html

[T55] Scala：集合过滤
来源：http://hz.gogol.net.cn/gtrdvfirbj.html

List(1, 2, 3).filter(_ > 1)
来源：http://hz.gogol.net.cn/gthlcairud.html

[T56] Scala：样例类
来源：http://hz.yuanzhike.top/gtcsofaexv.html

case class User(name: String, age: Int)
来源：http://hz.cheryme.top/gtslfxjmaj.html

[T57] Scala：模式匹配
来源：http://hz.hfpthk.cn/gtpqhainbe.html

x match { case 1 => "一"; case _ => "其他" }
来源：http://hz.pengpengdd.cyou/gtxfntzvvt.html

[T58] Scala：函数定义
来源：http://hz.meibo888.top/gtxcgfdvso.html

def add(a: Int, b: Int): Int = a + b
来源：http://hz.xuanzx.com/gtrukbqlza.html

[T59] Scala：循环
来源：http://hz.smart0.xyz/gtxbfvhjbs.html

for (i <- 1 to 10) println(i)
来源：http://hz.hammf.cn/gtfgrtqkqq.html

[T60] Scala：折叠
来源：http://hz.yonumen.top/gtdcvlejqm.html

List(1, 2, 3).foldLeft(0)(_ + _)
来源：http://hz.feifeiyinyue.top/gtwvpuzyhb.html

================================================================================
来源：http://hz.iojbl.cn/gttmhuoxgm.html

U. 高频实用片段（Python / PHP / JavaScript 各 40 条）
来源：http://hz.birdmap.top/gtcdwmnteq.html

================================================================================
来源：http://hz.jinqigfzy.top/gtniucmmes.html

[U01] Py：创建虚拟环境
来源：http://hz.ivvv.top/gtgjskaaoa.html

python -m venv .venv && source .venv/bin/activate
来源：http://hz.zdqjudy.top/gtxncjzsro.html

[U02] Py：导出 / 安装依赖
来源：http://hz.hnqzz.top/gtskdfdihv.html

pip freeze > requirements.txt;  pip install -r requirements.txt
来源：http://hz.zhoulong.xyz/gtflkcxmbg.html

[U03] Py：加载 .env 配置
来源：http://hz.zhongyouzk.top/gtduemrmcs.html

from dotenv import load_dotenv; load_dotenv()
来源：http://hz.hnqzz.top/gtdxnaohfq.html

[U04] Py：变量调试打印
来源：http://hz.c1oappe.top/gtoglheqmo.html

print(f"{x=}")            # 输出 x=值，Python 3.8+
来源：http://hz.ivvv.top/gtkkjutagr.html

[U05] Py：列表去重且保序
来源：http://hz.jlsjyb.cn/gtzcbnxylt.html

list(dict.fromkeys(arr))
来源：http://hz.pengpengdd.cyou/gtxbxpnzie.html

[U06] Py：合并两个字典
来源：http://hz.gotoacloud.top/gtmydpmxns.html

{**a, **b}
来源：http://hz.jqgfzy.top/gtemypnjmm.html

[U07] Py：反转字典键值
来源：http://hz.shanyushiyangkeji.top/gtotmfbaig.html

{v: k for k, v in d.items()}
来源：http://hz.zhoulong.xyz/gtxcoauyzz.html

[U08] Py：展平二维列表
来源：http://hz.shangyingyoupin.top/gtltdmxlhu.html

[y for x in nested for y in x]
来源：http://hz.xziqi.cn/gtvegroqvx.html

[U09] Py：字典取最大值的键
来源：http://hz.zhaomingkeji.xyz/gtfpsvntto.html

max(d, key=d.get)
来源：http://hz.cqqwz.cn/gtegzfxrfq.html

[U10] Py：按值排序字典
来源：http://hz.9152youxi.cn/gtsyfofywy.html

dict(sorted(d.items(), key=lambda kv: kv[1]))
来源：http://hz.xuetiantiany.cn/gtctatqpib.html

[U11] Py：生成器表达式
来源：http://hz.gogol.net.cn/gtppsqdseb.html

(x * 2 for x in arr)
来源：http://hz.kuanghao11.cn/gtnmachoka.html

[U12] Py：取出现最多的 3 个元素
来源：http://hz.smart0.xyz/gtipsmbygw.html

Counter(arr).most_common(3)
来源：http://hz.jinqigufen.top/gtfpyuqzxk.html

[U13] Py：固定长度队列
来源：http://hz.hongshengwenyu.top/gtjmgvfvwj.html

deque(maxlen=10)
来源：http://hz.yongpay.top/gtwsmaxgcn.html

[U14] Py：分组收集到列表
来源：http://hz.havefunace.top/gtpzkgagwc.html

defaultdict(list)
来源：http://hz.guowangkeji.top/gthwhtknnl.html

[U15] Py：高精度计时
来源：http://hz.tianlin.xyz/gtdgqfdcag.html

t = time.perf_counter()
来源：http://hz.0kj1m.cn/gtirsanghy.html

[U16] Py：命令行参数解析
来源：http://hz.xuanzx.com/gtwikzqzzp.html

ap = argparse.ArgumentParser();  ap.add_argument("--name");  args = ap.parse_args()
来源：http://hz.zycfv.cn/gtvdldaxvc.html

[U17] Py：初始化日志
来源：http://hz.yj20258.top/gtdqtxkeor.html

logging.basicConfig(level=logging.INFO)
来源：http://hz.52xcode.cn/gtheatfoqk.html

[U18] Py：预编译正则
来源：http://hz.zhongyouzk.top/gtvrpkxpwz.html

pat = re.compile(r"\d+")
来源：http://hz.yvedp.cn/gtsuvsvlwt.html

[U19] Py：正则替换带回调
来源：http://hz.hnxiangtu.top/gtuwjveffd.html

re.sub(r"\d+", lambda m: str(int(m.group()) * 2), s)
来源：http://hz.shanyushiyangkeji.top/gtyxjshusp.html

[U20] Py：缓存函数结果
来源：http://hz.cheryme.top/gtowltmjoa.html

@functools.lru_cache(maxsize=None)
来源：http://hz.zhiwuduotai.top/gtoflgqdwr.html

[U21] Py：自定义上下文管理器
来源：http://hz.cdnleiting.top/gtslemroeo.html

@contextlib.contextmanager
来源：http://hz.yj20258888.top/gtykgifemv.html

[U22] Py：矩阵转置
来源：http://hz.tian-w.cn/gtikmtcsku.html

list(zip(*m))
来源：http://hz.ppjwa.cn/gthgurdqex.html

[U23] Py：分块读取大文件
来源：http://hz.jinyuanbaomall.cn/gtygyhpteg.html

for chunk in iter(lambda: f.read(8192), b""):
来源：http://hz.jiagoushi.top/gtpomecnnr.html

[U24] Py：路径操作
来源：http://hz.zhiwuduotai.top/gtfuusjenq.html

Path("a/b.txt").parent.mkdir(parents=True, exist_ok=True)
来源：http://hz.jinqigfzy.top/gtksoyhetq.html

[U25] Py：CSV 按字典读
来源：http://hz.zhijiandao.cn/gtzdumwasc.html

csv.DictReader(f)
来源：http://hz.shanyushiyangtech.top/gtcqweesft.html

[U26] Py：并发下载
来源：http://hz.redwolf501.top/gtcdbqwrej.html

ThreadPoolExecutor(max_workers=8).map(fetch, urls)
来源：http://hz.quarkkingdee.top/gtcluywxuh.html

[U27] Py：异步 HTTP
来源：http://hz.zhiwuduotai.top/gtlxrtzrea.html

aiohttp.ClientSession() 配合 async with
来源：http://hz.316326.xyz/gtvrdvbodo.html

[U28] Py：类型别名
来源：http://hz.yuanzhike.top/gtmrlmjgkd.html

UserId = int
来源：http://hz.zhixingplan.top/gtlogldocz.html

[U29] Py：属性校验
来源：http://hz.fengsongda.top/gttbszdccj.html

@property 与 @x.setter 配合
来源：http://hz.cdnleiting.top/gtpbmcnjge.html

[U30] Py：数据类
来源：http://hz.zycfv.cn/gtktharjbm.html

@dataclass(slots=True)
来源：http://hz.316326.xyz/gthmtbqxqi.html

[U31] Py：单测
来源：http://hz.daria6918.cn/gtoubuahlm.html

python -m pytest -q
来源：http://hz.cheryme.top/gtbutrpdtc.html

[U32] Py：代码格式化
来源：http://hz.xziqi.cn/gtfvcwnehf.html

ruff format . && ruff check --fix .
来源：http://hz.jinqigfzy.top/gtxwegkhor.html

[U33] Py：打包发布
来源：http://hz.pengpengdd.cyou/gtyjpqtjrd.html

python -m build  （依赖 pyproject.toml）
来源：http://hz.hfpthk.cn/gtrgyswppw.html

[U34] Py：判断编码
来源：http://hz.haohaochexian.top/gtonofvbzd.html

chardet.detect(raw)
来源：http://hz.yj20258.top/gtaawgibhc.html

[U35] Py：发送邮件
来源：http://hz.nanxinkj.top/gttgnjfiau.html

smtplib.SMTP_SSL(...).send_message(msg)
来源：http://hz.dianchejie.cn/gtbfhidvet.html

[U36] Py：定时任务
来源：http://hz.ivvv.top/gtsnsgvieq.html

schedule.every(10).minutes.do(job)
来源：http://hz.feifeiyinyue.top/gtfwhoqwoj.html

[U37] Py：读写 Excel
来源：http://hz.redwolf501.top/gtskzkwgzn.html

pandas.read_excel / DataFrame.to_excel
来源：http://hz.yvedp.cn/gtychovjzl.html

[U38] Py：获取脚本所在目录
来源：http://hz.zhoulong.xyz/gtqbjajgoy.html

Path(__file__).resolve().parent
来源：http://hz.zhiwuduotai.top/gtzdjvkddb.html

[U39] Py：判断是否在交互环境
来源：http://hz.yanxiufei.cn/gtrhtxofbm.html

sys.stdout.isatty()
来源：http://hz.gzhubu.top/gtaoxsvaws.html

[U40] Py：打印到标准错误
来源：http://hz.tianlin.xyz/gtazghhzka.html

print("err", file=sys.stderr)
来源：http://hz.zhijiandao.cn/gtuwctexei.html

[U41] PHP：初始化 Composer 项目
来源：http://hz.tianlin.xyz/gtfbteqjdq.html

composer init;  composer require guzzlehttp/guzzle
来源：http://hz.yangfankeji.com/gtbboeoicc.html

[U42] PHP：PSR-4 自动加载
来源：http://hz.cheryme.top/gtxyceqeqa.html

"autoload": { "psr-4": { "App\\": "src/" } }
来源：http://hz.tian-w.cn/gtoorjnhpb.html

[U43] PHP：声明命名空间
来源：http://hz.gogol.net.cn/gtyugenfft.html

namespace App\Http;
来源：http://hz.tanke756.top/gtysvcanhg.html

[U44] PHP：开启严格类型
来源：http://hz.svipenyu.cn/gtekyzcnkx.html

declare(strict_types=1);
来源：http://hz.yj20258888.top/gtzsgioccx.html


<!-- 参考信息 -->