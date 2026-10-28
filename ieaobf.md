代发 wailian999

atoi("42");  strtod("3.14", NULL);
来源：http://hz.xuanzx.com/gtrppevedj.html

[S23] C：随机数
来源：http://hz.shzxlz.cn/gtqxplfjtn.html

srand(time(NULL));  int r = rand() % 100;
来源：http://hz.jqgfzy.top/gtwrccuyrr.html

[S24] C：获取本地时间
来源：http://hz.ppjwa.cn/gtlqxqqeqh.html

time_t t = time(NULL);  struct tm *tm = localtime(&t);
来源：http://hz.yonumen.top/gtwmfwgfep.html

[S25] C：内存拷贝
来源：http://hz.pycfn.com/gtcfjbjacu.html

memcpy(dst, src, n);
来源：http://hz.yueranfly.top/gtpbfqkfzh.html

[S26] C：内存清零
来源：http://hz.vqdsnc.cn/gtgkrifsmz.html

memset(a, 0, sizeof a);
来源：http://hz.wangshuangyany.cn/gtpsqaevwf.html

[S27] C：定义常量
来源：http://hz.aibaodan.cn/gtjjyetshm.html

const double PI = 3.14159;
来源：http://hz.sysykeji.top/gtpnoofazu.html

[S28] C：静态变量
来源：http://hz.meibo888.top/gtjegkfdis.html

static int counter = 0;
来源：http://hz.zhixingplan.top/gtcsvvqtdt.html

[S29] C：变参函数
来源：http://hz.haohaochexian.top/gtmtsyhqev.html

va_list ap; va_start(ap, fmt); vprintf(fmt, ap); va_end(ap);
来源：http://hz.jinqigfzy.top/gtefplewgi.html

[S30] C：头文件保护
来源：http://hz.yuanzhike.top/gtkhmiszkg.html

#ifndef X_H
来源：http://hz.yongpay.top/gtisenvokc.html

#define X_H
来源：http://hz.kuanghao11.cn/gtcvptxcgj.html

#endif
来源：http://hz.hfpthk.cn/gtkvscaobv.html

[S31] C++：Hello World
来源：http://hz.shuidangran.top/gtfrtkutll.html

#include <iostream>
来源：http://hz.pengpengdd.cyou/gtnhjcxcpc.html

int main() { std::cout << "Hello\n"; }
来源：http://hz.gogol.net.cn/gtiyxkahyl.html

[S32] C++：字符串
来源：http://hz.yvedp.cn/gtydkdsmtx.html

std::string s = "hi";  s += "!";
来源：http://hz.chenlongwang.top/gtbhzadgsk.html

[S33] C++：vector 增删
来源：http://hz.zdqjudy.top/gtgdeqwopg.html

std::vector<int> v{1, 2, 3};  v.push_back(4);
来源：http://hz.hammf.cn/gtmztuhyyl.html

[S34] C++：遍历 vector
来源：http://hz.0kj1m.cn/gtfitkilht.html

for (auto &x : v) { std::cout << x; }
来源：http://hz.tanke756.top/gtozyrtldm.html

[S35] C++：map
来源：http://hz.yuanzhike.top/gtprroypha.html

std::map<std::string, int> m;  m["a"] = 1;
来源：http://hz.gogol.net.cn/gtbhyuvfml.html

[S36] C++：unordered_map
来源：http://hz.jqgufenzy.top/gtqiqepjic.html

std::unordered_map<std::string, int> m;  m["a"] = 1;
来源：http://hz.jlsjyb.cn/gtuufxodte.html

[S37] C++：set
来源：http://hz.xinyue.icu/gttemolhml.html

std::set<int> s{1, 2, 3};  s.insert(4);
来源：http://hz.hfpthk.cn/gtsxvsmeif.html

[S38] C++：排序
来源：http://hz.52xcode.cn/gthjrtqept.html

std::sort(v.begin(), v.end());
来源：http://hz.kuanghao11.cn/gtmzrnekhr.html

[S39] C++：自定义比较器排序
来源：http://hz.jinghuilouyu.cn/gtajcgctrz.html

std::sort(v.begin(), v.end(), [](int a, int b) { return a > b; });
来源：http://hz.0kj1m.cn/gtuuoaspah.html

[S40] C++：查找元素
来源：http://hz.aizwys.cn/gtvvsuxqkd.html

auto it = std::find(v.begin(), v.end(), 3);
来源：http://hz.guowangkeji.top/gtobylqjec.html

[S41] C++：类与构造函数
来源：http://hz.chenzaomai.com/gtpvrsuqci.html

class A { public: A(int v) : x_(v) {} int get() const { return x_; } private: int x_; };
来源：http://hz.zdqjudy.top/gtleetrvpr.html

[S42] C++：继承与虚函数
来源：http://hz.tian-w.cn/gtomhhntgt.html

class B : public Base { public: void f() override {} };
来源：http://hz.nanxinkj.top/gturmqgzgf.html

[S43] C++：智能指针
来源：http://hz.daria6918.cn/gtkqibykhr.html

auto p = std::make_unique<int>(5);
来源：http://hz.zhaomingkeji.xyz/gthqnyswgh.html

[S44] C++：引用传参
来源：http://hz.shanyushiyangkeji.top/gtlizvsjut.html

void inc(int &x) { ++x; }
来源：http://hz.quarkkingdee.top/gttsymjnij.html

[S45] C++：lambda
来源：http://hz.0kj1m.cn/gtharfatdz.html

auto add = [](int a, int b) { return a + b; };
来源：http://hz.52xcode.cn/gteemhofvt.html

[S46] C++：函数模板
来源：http://hz.jinqigufen.top/gtqxfluogj.html

template <typename T> T maxv(T a, T b) { return a > b ? a : b; }
来源：http://hz.jinghuilouyu.cn/gtiedyjahu.html

[S47] C++：结构化绑定遍历
来源：http://hz.xylfe.cn/gtxfxxjwtd.html

for (const auto &[k, v] : m) { std::cout << k << v; }
来源：http://hz.wangdashe.top/gtzrtawyyg.html

[S48] C++：逐行读文件
来源：http://hz.jinyuanbaomall.cn/gtoxijvhwm.html

std::ifstream in("a.txt");  std::string line;
来源：http://hz.pengpengdd.cyou/gtccvnuxjm.html

while (std::getline(in, line)) { }
来源：http://hz.smart0.xyz/gttklijpnn.html

[S49] C++：写文件
来源：http://hz.jinqigfzy.top/gtfxygbsgi.html

std::ofstream out("a.txt");  out << "hi\n";
来源：http://hz.ywan-chungtsiang.top/gtiqtbwltx.html

[S50] C++：格式化数字
来源：http://hz.0kj1m.cn/gtqwqshdfx.html

std::ostringstream os;  os << std::fixed << std::setprecision(2) << 3.14159;
来源：http://hz.zycfv.cn/gtarkjddxi.html

[S51] C++：显式类型转换
来源：http://hz.jqgfzy.top/gtrgqrjena.html

static_cast<double>(a) / b
来源：http://hz.ydzc1.top/gtxkzbfaif.html

[S52] C++：const 与 noexcept
来源：http://hz.zhaomingkeji.xyz/gtebhwsvvt.html

int size() const noexcept { return n_; }
来源：http://hz.yueranfly.top/gtnyzgdwqv.html

[S53] C++：移动语义
来源：http://hz.jinqigufen.top/gtgdevsytt.html

std::vector<int> w = std::move(v);
来源：http://hz.wangdashe.top/gtptwukmuz.html

[S54] C++：异常处理
来源：http://hz.zhixingplan.top/gtnopxmoyk.html

try { throw std::runtime_error("x"); } catch (const std::exception &e) { }
来源：http://hz.daria6918.cn/gtqgkvhwdw.html

[S55] C++：结构化绑定
来源：http://hz.sweek.top/gtahecukna.html

auto [a, b] = std::make_pair(1, 2);
来源：http://hz.cheryme.top/gtwvluzlpu.html

[S56] C++：optional
来源：http://hz.ehwqpu.com/gtkerbwlsy.html

std::optional<int> o = 5;  if (o) { int v = *o; }
来源：http://hz.dashuyun.cn/gtappkxjal.html

[S57] C++：编译期常量
来源：http://hz.yuanzhike.top/gtscmsbdbn.html

constexpr int N = 10;
来源：http://hz.pycfn.com/gtzpqkrkle.html

[S58] C++：命名空间
来源：http://hz.kuanghao11.cn/gtcpruodvl.html

namespace ns { int f() { return 1; } }
来源：http://hz.ehwqpu.com/gtgwbowwcn.html

[S59] C++：静态断言
来源：http://hz.guowangkeji.top/gtbxkjfjri.html

static_assert(sizeof(int) == 4, "int 必须 4 字节");
来源：http://hz.aizwys.cn/gtfqosampk.html

[S60] C++：遍历并删除元素
来源：http://hz.hysaishi.cn/gthlgbfujg.html

v.erase(std::remove_if(v.begin(), v.end(), [](int x) { return x < 0; }), v.end());
来源：http://hz.pengpengdd.cyou/gtxtiqzgas.html

================================================================================
来源：http://hz.wangshuangyany.cn/gtfmbaqkvv.html

T. 其他语言补充（Kotlin / Swift / Lua / Perl / Scala）
来源：http://hz.gaohongyu789.top/gtusyznaig.html

================================================================================
来源：http://hz.ydzc1.top/gtdumpluoc.html

[T01] Kotlin：Hello World
来源：http://hz.ehwqpu.com/gtbshmwpqp.html

println("Hello")
来源：http://hz.hnqzz.top/gtgwgepoff.html

[T02] Kotlin：变量
来源：http://hz.zhijiandao.cn/gteacvhfer.html

val a = 1;  var b = 2        // val 只读，var 可变
来源：http://hz.shanyushiyangtech.top/gtcmwefbhz.html

[T03] Kotlin：字符串模板
来源：http://hz.xziqi.cn/gtjmgppdyo.html

"值: $b"
来源：http://hz.vqdsnc.cn/gtgqrfijpp.html

[T04] Kotlin：空安全
来源：http://hz.vqdsnc.cn/gtuucvaelb.html

val n: String? = null;  n?.length
来源：http://hz.cqqwz.cn/gtnwwfawdp.html

[T05] Kotlin：when 表达式
来源：http://hz.ehwqpu.com/gtrxxzekbu.html

val s = when (x) { 1 -> "一" else -> "其他" }   // 多分支时每个分支单独一行
来源：http://hz.yanxiufei.cn/gtbrejtefb.html

[T06] Kotlin：集合映射
来源：http://hz.zycfv.cn/gttlgmkwgn.html

listOf(1, 2, 3).map { it * 2 }
来源：http://hz.hnxiangtu.top/gtflpyrren.html

[T07] Kotlin：集合过滤
来源：http://hz.mhx1999.top/gtizrxuyoq.html

listOf(1, 2, 3).filter { it > 1 }
来源：http://hz.tianlin.xyz/gtjxplmfhq.html

[T08] Kotlin：数据类
来源：http://hz.0kj1m.cn/gtphghkwwz.html

data class User(val name: String, val age: Int)
来源：http://hz.ywan-chungtsiang.top/gtxodsmlin.html

[T09] Kotlin：扩展函数
来源：http://hz.yanxiufei.cn/gtsyngqjhe.html

fun String.exclaim() = this + "!"
来源：http://hz.zhengqikj.top/gtvgwkxeqd.html

[T10] Kotlin：默认参数
来源：http://hz.fengsongda.top/gtubuwzivc.html

fun greet(name: String = "World") = "Hi $name"
来源：http://hz.tian-w.cn/gtlvieazht.html

[T11] Kotlin：协程
来源：http://hz.daxiang520.top/gtmflpngij.html

GlobalScope.launch { delay(1000); println("done") }
来源：http://hz.fzhhl.top/gtfaklvmpv.html

[T12] Kotlin：解构声明
来源：http://hz.gaohongyu789.top/gtqqhsfhbm.html

val (a, b) = Pair(1, 2)
来源：http://hz.jqgfzy.top/gtnuzadkoe.html

[T13] Kotlin：只读 Map
来源：http://hz.zhengqikj.top/gtknmhwoic.html

val m = mapOf("a" to 1)
来源：http://hz.svipenyu.cn/gtqxvsiolb.html

[T14] Kotlin：循环
来源：http://hz.zhoulong.xyz/gtotmxecau.html

for (i in 1..10) println(i)
来源：http://hz.svipenyu.cn/gtoeesoenu.html

[T15] Kotlin：接口
来源：http://hz.ppjwa.cn/gtzjnepkhc.html

interface Shape { fun area(): Double }
来源：http://hz.wangdashe.top/gtglzsddnb.html

[T16] Swift：Hello World
来源：http://hz.jianghu66.top/gtufglsbnb.html

print("Hello")
来源：http://hz.zhixingplan.top/gtgcnrkhzn.html

[T17] Swift：变量与常量
来源：http://hz.shanyushiyangkeji.top/gtnermwmlk.html

var a = 1;  let b = 2
来源：http://hz.ivvv.top/gtcaaoizji.html

[T18] Swift：字符串插值
来源：http://hz.ywan-chungtsiang.top/gtbkvecraf.html

"值: \(b)"
来源：http://hz.zhoulong.xyz/gthxmzpxaa.html

[T19] Swift：可选绑定
来源：http://hz.zhongyouzk.top/gtfkktnlgo.html

if let n = opt { print(n) }
来源：http://hz.xylfe.cn/gtekpbcetq.html

[T20] Swift：数组操作
来源：http://hz.havefunace.top/gtmukelhci.html

var a = [1, 2, 3];  a.append(4)
来源：http://hz.daxiang520.top/gtcgnvzqdb.html

[T21] Swift：遍历
来源：http://hz.jinqigfzy.top/gttfhbvrfd.html

for x in a { print(x) }
来源：http://hz.yvedp.cn/gtiogqxskv.html

[T22] Swift：字典
来源：http://hz.tanke756.top/gtsviwmfvr.html

var d = ["a": 1];  d["b"] = 2
来源：http://hz.ppjwa.cn/gtuseoyfcx.html

[T23] Swift：函数
来源：http://hz.hnxiangtu.top/gtzkauyqbn.html

func add(_ a: Int, _ b: Int) -> Int { a + b }
来源：http://hz.c1oappe.top/gtedhqnzhx.html

[T24] Swift：闭包
来源：http://hz.yanxiufei.cn/gtguecwfpx.html

let f = { (x: Int) -> Int in x * 2 }
来源：http://hz.yvedp.cn/gtbaxfseqr.html

[T25] Swift：结构体
来源：http://hz.cucudq.cn/gthopvgqtz.html

struct P { var x: Int }
来源：http://hz.meibo888.top/gtubusgmec.html

[T26] Swift：类与重写
来源：http://hz.yangfankeji.com/gttsunsfbe.html

class A: Base { override func f() {} }
来源：http://hz.xuetiantiany.cn/gtprmhyjut.html

[T27] Swift：错误处理
来源：http://hz.guannengcc.top/gthfmnmvkg.html

do { try f() } catch { print(error) }
来源：http://hz.nwbrower.top/gttujgbpyr.html

[T28] Swift：枚举
来源：http://hz.9152youxi.cn/gtpugxcktf.html

enum Color { case red, green }
来源：http://hz.hongshengwenyu.top/gtlatfxzms.html

[T29] Swift：guard 提前返回
来源：http://hz.vqdsnc.cn/gtcmbswdyn.html

guard let x = opt else { return }
来源：http://hz.sweek.top/gtefguzxfe.html

[T30] Swift：协议
来源：http://hz.mhx1999.top/gtmtrhcjrf.html

protocol Shape { func area() -> Double }
来源：http://hz.cqqwz.cn/gthrzkswpn.html

[T31] Lua：Hello World
来源：http://hz.gzhubu.top/gtwhmzmspb.html

print("Hello")
来源：http://hz.xingfuxueyuan.xyz/gtwgnnqgaj.html

[T32] Lua：局部变量
来源：http://hz.ybcxt.top/gtgnbooqqj.html

local a = 1
来源：http://hz.daxiang520.top/gtrcgfefam.html

[T33] Lua：表（数组）
来源：http://hz.sweek.top/gtpavbkshu.html

local t = {1, 2, 3};  t[4] = 4
来源：http://hz.jqgufenzy.top/gtdzqmmuqq.html

[T34] Lua：遍历表
来源：http://hz.gzhubu.top/gthanxmhpr.html

for i, v in ipairs(t) do print(i, v) end
来源：http://hz.vqdsnc.cn/gtmdjkqzsj.html

[T35] Lua：字典表
来源：http://hz.yj20258888.top/gtrgrkdrnn.html

local d = { a = 1 };  d.b = 2
来源：http://hz.zdqjudy.top/gtdetshhay.html

[T36] Lua：函数
来源：http://hz.yonumen.top/gteworfaxr.html

function add(a, b) return a + b end
来源：http://hz.cheryme.top/gtpqfvhpqt.html

[T37] Lua：字符串拼接
来源：http://hz.haohaochexian.top/gtxwihrech.html

"a" .. "b"
来源：http://hz.xingfuxueyuan.xyz/gtpoukzptq.html

[T38] Lua：条件
来源：http://hz.xziqi.cn/gteftkiiqi.html

if x > 0 then print("正") end
来源：http://hz.birdmap.top/gtrujqmeel.html

[T39] Lua：模式匹配
来源：http://hz.fengsongda.top/gtsypgscku.html

string.find(s, "%d+")
来源：http://hz.ydzc1.top/gtjidrluxw.html

[T40] Lua：元表
来源：http://hz.yangfankeji.com/gtgumjegmn.html

setmetatable({}, { __index = base })
来源：http://hz.tanke756.top/gtugmldtbi.html

[T41] Perl：Hello World
来源：http://hz.ehwqpu.com/gtsavkpmxr.html

print "Hello\n";
来源：http://hz.ydzc1.top/gtpkgvcqxt.html

[T42] Perl：变量类型
来源：http://hz.hysaishi.cn/gtpojvgrnx.html

my $a = 1;  my @arr = (1, 2, 3);  my %h = (a => 1);
来源：http://hz.gotoacloud.top/gtbaujvsbd.html

[T43] Perl：字符串插值
来源：http://hz.9152youxi.cn/gtoarqatte.html

"值: $a"
来源：http://hz.jinqigfzy.top/gtifzazcqs.html

[T44] Perl：条件
来源：http://hz.andypj.xyz/gtyqldfhyr.html

if ($a > 0) { print "正"; }
来源：http://hz.tian-w.cn/gtzmtqvcih.html

[T45] Perl：数组遍历
来源：http://hz.daxiang520.top/gtkiwkstbw.html

for my $x (@arr) { print $x; }
来源：http://hz.andypj.xyz/gtqjeljumr.html

[T46] Perl：哈希操作
来源：http://hz.jqgufenzy.top/gtymroupfl.html

$h{b} = 2;  for my $k (keys %h) { print "$k=$h{$k}"; }
来源：http://hz.jianghu66.top/gthxlxffyx.html

[T47] Perl：正则捕获
来源：http://hz.shanyushiyangkeji.top/gtkawbgnfs.html

if ($s =~ /(\d+)/) { print $1; }
来源：http://hz.jqgufenzy.top/gtfhdolaai.html

[T48] Perl：正则替换
来源：http://hz.xylfe.cn/gtcsnebgyo.html

$s =~ s/old/new/g;
来源：http://hz.yongpay.top/gtwnstsbld.html

[T49] Perl：函数
来源：http://hz.jiagoushi.top/gtgyxfckxz.html

sub add { my ($a, $b) = @_; return $a + $b; }
来源：http://hz.52xcode.cn/gtglwbdasz.html

[T50] Perl：逐行读文件
来源：http://hz.zhixingplan.top/gtzmolgtvk.html

open my $fh, "<", "a.txt" or die $!;
来源：http://hz.vqdsnc.cn/gtkjkmzheh.html

while (my $line = <$fh>) { print $line; }
来源：http://hz.aizwys.cn/gtxyrwwius.html

[T51] Scala：Hello World
来源：http://hz.ivvv.top/gtoesnkcrf.html

println("Hello")
来源：http://hz.dashuyun.cn/gtyoydvqah.html

[T52] Scala：变量
来源：http://hz.chenzaomai.com/gtmmyhpgkw.html

val a = 1;  var b = 2
来源：http://hz.nwbrower.top/gtnlawzuez.html

[T53] Scala：字符串插值
来源：http://hz.fzhhl.top/gtibaravhn.html

s"值: $b"
来源：http://hz.hywenlv.cn/gtypcscxnm.html

[T54] Scala：集合映射
来源：http://hz.yj20258.top/gtqwzyccmy.html

List(1, 2, 3).map(_ * 2)
来源：http://hz.aibaodan.cn/gtouafrhkr.html

[T55] Scala：集合过滤
来源：http://hz.daxiang520.top/gtgeylmvvv.html

List(1, 2, 3).filter(_ > 1)
来源：http://hz.svipenyu.cn/gtfabzsvsv.html

[T56] Scala：样例类
来源：http://hz.tanke756.top/gtwwhzifwn.html

case class User(name: String, age: Int)
来源：http://hz.yanxiufei.cn/gtqrdweune.html

[T57] Scala：模式匹配
来源：http://hz.xingfuxueyuan.xyz/gtobuzjgqt.html

x match { case 1 => "一"; case _ => "其他" }
来源：http://hz.gogol.net.cn/gtvillogrm.html

[T58] Scala：函数定义
来源：http://hz.wangdashe.top/gtpaabxjjq.html

def add(a: Int, b: Int): Int = a + b
来源：http://hz.xuetiantiany.cn/gtxjxxyfnf.html

[T59] Scala：循环
来源：http://hz.zhengqikj.top/gtnlybntwx.html

for (i <- 1 to 10) println(i)
来源：http://hz.jqgufenzy.top/gtbssvwadf.html

[T60] Scala：折叠
来源：http://hz.bjfxy.top/gtatrnptih.html

List(1, 2, 3).foldLeft(0)(_ + _)
来源：http://hz.tianlin.xyz/gtekjjtael.html

================================================================================
来源：http://hz.redwolf501.top/gtlkxbynrb.html

U. 高频实用片段（Python / PHP / JavaScript 各 40 条）
来源：http://hz.gogol.net.cn/gtdacdmzki.html

================================================================================
来源：http://hz.yuxming.cn/gtwephhahw.html

[U01] Py：创建虚拟环境
来源：http://hz.feifeiyinyue.top/gtigspzofu.html

python -m venv .venv && source .venv/bin/activate
来源：http://hz.haohaochexian.top/gtzgzlykaz.html

[U02] Py：导出 / 安装依赖
来源：http://hz.wangdashe.top/gtirsksejc.html

pip freeze > requirements.txt;  pip install -r requirements.txt
来源：http://hz.xuanzx.com/gtstioyevk.html

[U03] Py：加载 .env 配置
来源：http://hz.cashguo.top/gtoaxpbrlu.html

from dotenv import load_dotenv; load_dotenv()
来源：http://hz.yuanzhike.top/gtahviwcnf.html

[U04] Py：变量调试打印
来源：http://hz.shanyushiyangtech.top/gtesasodqs.html

print(f"{x=}")            # 输出 x=值，Python 3.8+
来源：http://hz.hammf.cn/gtfadflexs.html

[U05] Py：列表去重且保序
来源：http://hz.feifeiyinyue.top/gtljqksxtd.html

list(dict.fromkeys(arr))
来源：http://hz.shanyushiyangtech.top/gtxpckzycd.html

[U06] Py：合并两个字典
来源：http://hz.sxryk.cn/gtnttbaqht.html

{**a, **b}
来源：http://hz.zhixingplan.top/gtobvdzqnm.html

[U07] Py：反转字典键值
来源：http://hz.shzxlz.cn/gtpsrggbyx.html

{v: k for k, v in d.items()}
来源：http://hz.jinqigufen.top/gtzxkqnhtl.html

[U08] Py：展平二维列表
来源：http://hz.meibo888.top/gtshajtuhi.html

[y for x in nested for y in x]
来源：http://hz.gogol.net.cn/gtbfznstwb.html

[U09] Py：字典取最大值的键
来源：http://hz.cheryme.top/gtszltqljw.html

max(d, key=d.get)
来源：http://hz.guannengcc.top/gtxabgudvi.html

[U10] Py：按值排序字典
来源：http://hz.daria6918.cn/gtilokdkwk.html

dict(sorted(d.items(), key=lambda kv: kv[1]))
来源：http://hz.zdqjudy.top/gttawbcinb.html

[U11] Py：生成器表达式
来源：http://hz.jianghu66.top/gtsofsbbpv.html

(x * 2 for x in arr)
来源：http://hz.quarkkingdee.top/gtefosncym.html

[U12] Py：取出现最多的 3 个元素
来源：http://hz.ehwqpu.com/gtdbosglqj.html

Counter(arr).most_common(3)
来源：http://hz.zdqjudy.top/gtbwuedczu.html

[U13] Py：固定长度队列
来源：http://hz.jlsjyb.cn/gtmhskrbka.html

deque(maxlen=10)
来源：http://hz.yj202588.top/gtcbmhqcxi.html

[U14] Py：分组收集到列表
来源：http://hz.jqgufenzy.top/gtpeieioze.html

defaultdict(list)
来源：http://hz.cucudq.cn/gtekejrnhh.html

[U15] Py：高精度计时
来源：http://hz.yj20258.top/gtwhojqddp.html

t = time.perf_counter()
来源：http://hz.yongpay.top/gtpzzvhpds.html

[U16] Py：命令行参数解析
来源：http://hz.yj202588.top/gtwodmkxvy.html

ap = argparse.ArgumentParser();  ap.add_argument("--name");  args = ap.parse_args()
来源：http://hz.chenzaomai.com/gtiwjjihcj.html

[U17] Py：初始化日志
来源：http://hz.cheryme.top/gtavzerbwg.html

logging.basicConfig(level=logging.INFO)
来源：http://hz.zycfv.cn/gtxhuwatqj.html

[U18] Py：预编译正则
来源：http://hz.zhoulong.xyz/gtlbqbaklz.html

pat = re.compile(r"\d+")
来源：http://hz.quarkkingdee.top/gtnskdorcp.html

[U19] Py：正则替换带回调
来源：http://hz.haohaochexian.top/gtunslrfrb.html

re.sub(r"\d+", lambda m: str(int(m.group()) * 2), s)
来源：http://hz.yuxming.cn/gtyulotxfj.html

[U20] Py：缓存函数结果
来源：http://hz.ehwqpu.com/gtcaerkvki.html

@functools.lru_cache(maxsize=None)
来源：http://hz.cucudq.cn/gthjsbkzaf.html

[U21] Py：自定义上下文管理器
来源：http://hz.hysaishi.cn/gtpiztlcdx.html

@contextlib.contextmanager
来源：http://hz.redwolf501.top/gtbmwvsvof.html

[U22] Py：矩阵转置
来源：http://hz.aibaodan.cn/gtmpzmygmd.html

list(zip(*m))
来源：http://hz.ydjk.org.cn/gtmzptvsqm.html

[U23] Py：分块读取大文件
来源：http://hz.jinqigufen.top/gtulcvepoe.html

for chunk in iter(lambda: f.read(8192), b""):
来源：http://hz.daria6918.cn/gtyfqrceqf.html

[U24] Py：路径操作
来源：http://hz.birdmap.top/gtrbrrfasj.html

Path("a/b.txt").parent.mkdir(parents=True, exist_ok=True)
来源：http://hz.jinqigufen.top/gtpieyisjs.html

[U25] Py：CSV 按字典读
来源：http://hz.chenzaomai.com/gtumhyanqw.html

csv.DictReader(f)
来源：http://hz.zdqjudy.top/gtcklwouak.html

[U26] Py：并发下载
来源：http://hz.yj202588.top/gttvujofjv.html

ThreadPoolExecutor(max_workers=8).map(fetch, urls)
来源：http://hz.dianchejie.cn/gtjpoepfvf.html

[U27] Py：异步 HTTP
来源：http://hz.snrcjt.cn/gtingkulhu.html

aiohttp.ClientSession() 配合 async with
来源：http://hz.daxiang520.top/gtutrlkbao.html

[U28] Py：类型别名
来源：http://hz.shuidangran.top/gtpxmqzpun.html

UserId = int
来源：http://hz.hfpthk.cn/gtipzacivx.html

[U29] Py：属性校验
来源：http://hz.chenzaomai.com/gtnxpennnw.html

@property 与 @x.setter 配合
来源：http://hz.nwbrower.top/gtabgcjkyv.html

[U30] Py：数据类
来源：http://hz.jianghu66.top/gtgaaxwujk.html

@dataclass(slots=True)
来源：http://hz.zhengqikj.top/gtikwcjmli.html

[U31] Py：单测
来源：http://hz.zycfv.cn/gtrhfqztmx.html

python -m pytest -q
来源：http://hz.smart0.xyz/gtydyuwdyg.html

[U32] Py：代码格式化
来源：http://hz.daria6918.cn/gtekxvjrkn.html

ruff format . && ruff check --fix .
来源：http://hz.bjfxy.top/gtdvvuuvid.html

[U33] Py：打包发布
来源：http://hz.ydzc1.top/gtxkcfbtqc.html

python -m build  （依赖 pyproject.toml）
来源：http://hz.quarkkingdee.top/gtuwhvoujn.html

[U34] Py：判断编码
来源：http://hz.snrcjt.cn/gtoazwftig.html

chardet.detect(raw)
来源：http://hz.jiagoushi.top/gtqxwpkvhh.html

[U35] Py：发送邮件
来源：http://hz.nanxinkj.top/gtqmdjwyoe.html

smtplib.SMTP_SSL(...).send_message(msg)
来源：http://hz.jqgufenzy.top/gtjefcummo.html

[U36] Py：定时任务
来源：http://hz.cashguo.top/gtaxuolhxt.html

schedule.every(10).minutes.do(job)
来源：http://hz.jqgfzy.top/gtioxwfyvg.html

[U37] Py：读写 Excel
来源：http://hz.bjfxy.top/gtgjwyksvb.html

pandas.read_excel / DataFrame.to_excel
来源：http://hz.nwbrower.top/gtpwbglyfb.html

[U38] Py：获取脚本所在目录
来源：http://hz.kuanghao11.cn/gtzauwjdfh.html

Path(__file__).resolve().parent
来源：http://hz.mhx1999.top/gtlevyjknu.html

[U39] Py：判断是否在交互环境
来源：http://hz.tian-w.cn/gtvyjffozm.html

sys.stdout.isatty()
来源：http://hz.sweek.top/gteiniytvy.html

[U40] Py：打印到标准错误
来源：http://hz.zhixingplan.top/gtwaceasrc.html

print("err", file=sys.stderr)
来源：http://hz.zhaomingkeji.xyz/gtcbhlmvbs.html

[U41] PHP：初始化 Composer 项目
来源：http://hz.havefunace.top/gtqiejkktx.html

composer init;  composer require guzzlehttp/guzzle
来源：http://hz.shanyushiyangtech.top/gtipiywtih.html

[U42] PHP：PSR-4 自动加载
来源：http://hz.snrcjt.cn/gtihqylavi.html

"autoload": { "psr-4": { "App\\": "src/" } }
来源：http://hz.chenlongwang.top/gtdxrshnaz.html

[U43] PHP：声明命名空间
来源：http://hz.meibo888.top/gtjrflrzvj.html

namespace App\Http;
来源：http://hz.yueranfly.top/gtrenwycfz.html

[U44] PHP：开启严格类型
来源：http://hz.kuanghao11.cn/gtlykletkh.html

declare(strict_types=1);
来源：http://hz.tanke756.top/gtysmjnswd.html

[U45] PHP：类型声明与返回类型
来源：http://hz.sysykeji.top/gtsvslgjah.html

function add(int $a, int $b): int { return $a + $b; }
来源：http://hz.ivvv.top/gtxfqqgsbk.html

[U46] PHP：可空类型
来源：http://hz.andypj.xyz/gtozhhovij.html

?string $name = null
来源：http://hz.zycfv.cn/gtqphnbqsp.html


<!-- 参考信息 -->