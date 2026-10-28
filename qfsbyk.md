代发 wailian999

#include <iostream>
来源：http://hz.jlsjyb.cn/gtmijddmiw.html

int main() { std::cout << "Hello\n"; }
来源：http://hz.sysykeji.top/gtbavyettf.html

[S32] C++：字符串
来源：http://hz.yj202588.top/gtgtlsfjxg.html

std::string s = "hi";  s += "!";
来源：http://hz.birdmap.top/gtxqyntldw.html

[S33] C++：vector 增删
来源：http://hz.chenzaomai.com/gtqievoaxx.html

std::vector<int> v{1, 2, 3};  v.push_back(4);
来源：http://hz.cashguo.top/gtbrbhmujm.html

[S34] C++：遍历 vector
来源：http://hz.yanxiufei.cn/gtfffxwzhy.html

for (auto &x : v) { std::cout << x; }
来源：http://hz.cucudq.cn/gtzygvtpnb.html

[S35] C++：map
来源：http://hz.zdqjudy.top/gtuqwuxeco.html

std::map<std::string, int> m;  m["a"] = 1;
来源：http://hz.jinqigfzy.top/gtibnijcbc.html

[S36] C++：unordered_map
来源：http://hz.nwbrower.top/gteaoqeawr.html

std::unordered_map<std::string, int> m;  m["a"] = 1;
来源：http://hz.ivvv.top/gtjpfkdyas.html

[S37] C++：set
来源：http://hz.tanke756.top/gtuuekbphi.html

std::set<int> s{1, 2, 3};  s.insert(4);
来源：http://hz.gotoacloud.top/gtlixwrtpx.html

[S38] C++：排序
来源：http://hz.pycfn.com/gthrqdxgks.html

std::sort(v.begin(), v.end());
来源：http://hz.9152youxi.cn/gtbnwkcbqf.html

[S39] C++：自定义比较器排序
来源：http://hz.jqgufenzy.top/gtjbgbsvrr.html

std::sort(v.begin(), v.end(), [](int a, int b) { return a > b; });
来源：http://hz.jiagoushi.top/gtidcqdrjz.html

[S40] C++：查找元素
来源：http://hz.ybcxt.top/gtehsfczrc.html

auto it = std::find(v.begin(), v.end(), 3);
来源：http://hz.9152youxi.cn/gtfbxsbszw.html

[S41] C++：类与构造函数
来源：http://hz.nanxinkj.top/gtkbrrwswm.html

class A { public: A(int v) : x_(v) {} int get() const { return x_; } private: int x_; };
来源：http://hz.sweek.top/gtcedkmwbw.html

[S42] C++：继承与虚函数
来源：http://hz.tian-w.cn/gtehwvntwm.html

class B : public Base { public: void f() override {} };
来源：http://hz.shzxlz.cn/gtlgyyoudl.html

[S43] C++：智能指针
来源：http://hz.shzxlz.cn/gtxyktjhgi.html

auto p = std::make_unique<int>(5);
来源：http://hz.gzhubu.top/gtpmqawbkn.html

[S44] C++：引用传参
来源：http://hz.dianchejie.cn/gttpllqtpf.html

void inc(int &x) { ++x; }
来源：http://hz.guowangkeji.top/gtqzhfvqhy.html

[S45] C++：lambda
来源：http://hz.yongpay.top/gtfhnpozho.html

auto add = [](int a, int b) { return a + b; };
来源：http://hz.yonumen.top/gtxhvkbwyf.html

[S46] C++：函数模板
来源：http://hz.daxiang520.top/gtvpotptjg.html

template <typename T> T maxv(T a, T b) { return a > b ? a : b; }
来源：http://hz.jqgfzy.top/gtufijkkmo.html

[S47] C++：结构化绑定遍历
来源：http://hz.zhiwuduotai.top/gtdtchpjlw.html

for (const auto &[k, v] : m) { std::cout << k << v; }
来源：http://hz.jinghuilouyu.cn/gtadfzsltt.html

[S48] C++：逐行读文件
来源：http://hz.guowangkeji.top/gtqanyzxwe.html

std::ifstream in("a.txt");  std::string line;
来源：http://hz.cashguo.top/gtnhjdomig.html

while (std::getline(in, line)) { }
来源：http://hz.vqdsnc.cn/gtupgvwfcj.html

[S49] C++：写文件
来源：http://hz.yvedp.cn/gtfzfinqsh.html

std::ofstream out("a.txt");  out << "hi\n";
来源：http://hz.tianlin.xyz/gtzcabpnzo.html

[S50] C++：格式化数字
来源：http://hz.redwolf501.top/gtdpnxubao.html

std::ostringstream os;  os << std::fixed << std::setprecision(2) << 3.14159;
来源：http://hz.xinyue.icu/gtverqlnrz.html

[S51] C++：显式类型转换
来源：http://hz.shanyushiyangtech.top/gtnfgklnpi.html

static_cast<double>(a) / b
来源：http://hz.zdqjudy.top/gtjjkmditu.html

[S52] C++：const 与 noexcept
来源：http://hz.ivvv.top/gtateoelrn.html

int size() const noexcept { return n_; }
来源：http://hz.nanxuanxn.top/gtqhvjbsjo.html

[S53] C++：移动语义
来源：http://hz.svipenyu.cn/gtbxbfcrtv.html

std::vector<int> w = std::move(v);
来源：http://hz.yonumen.top/gtwrzwihaw.html

[S54] C++：异常处理
来源：http://hz.yj20258888.top/gtzkxmfnir.html

try { throw std::runtime_error("x"); } catch (const std::exception &e) { }
来源：http://hz.shangyingyoupin.top/gtecmegsjg.html

[S55] C++：结构化绑定
来源：http://hz.cheryme.top/gthowopstc.html

auto [a, b] = std::make_pair(1, 2);
来源：http://hz.ehwqpu.com/gtjnviiyjh.html

[S56] C++：optional
来源：http://hz.mhx1999.top/gtndfqqddc.html

std::optional<int> o = 5;  if (o) { int v = *o; }
来源：http://hz.havefunace.top/gtogdujvby.html

[S57] C++：编译期常量
来源：http://hz.bjfxy.top/gtrpwxsftg.html

constexpr int N = 10;
来源：http://hz.yj20258.top/gtribuwzif.html

[S58] C++：命名空间
来源：http://hz.gaohongyu789.top/gtapgthdss.html

namespace ns { int f() { return 1; } }
来源：http://hz.316326.xyz/gtodpobqke.html

[S59] C++：静态断言
来源：http://hz.ydzc1.top/gtslhlqlni.html

static_assert(sizeof(int) == 4, "int 必须 4 字节");
来源：http://hz.zhaomingkeji.xyz/gtiqbfbnax.html

[S60] C++：遍历并删除元素
来源：http://hz.shanyushiyangtech.top/gtctonrffr.html

v.erase(std::remove_if(v.begin(), v.end(), [](int x) { return x < 0; }), v.end());
来源：http://hz.smart0.xyz/gtjhiizehz.html

================================================================================
来源：http://hz.xinyue.icu/gttbaweyki.html

T. 其他语言补充（Kotlin / Swift / Lua / Perl / Scala）
来源：http://hz.quarkkingdee.top/gtvbdhlnmw.html

================================================================================
来源：http://hz.shuidangran.top/gtyuxovpsy.html

[T01] Kotlin：Hello World
来源：http://hz.gotoacloud.top/gticnfiivc.html

println("Hello")
来源：http://hz.zhoulong.xyz/gtcbmacprq.html

[T02] Kotlin：变量
来源：http://hz.tianlin.xyz/gtekobonmo.html

val a = 1;  var b = 2        // val 只读，var 可变
来源：http://hz.shanyushiyangkeji.top/gtcdjlbphx.html

[T03] Kotlin：字符串模板
来源：http://hz.yangfankeji.com/gtywzfhxqd.html

"值: $b"
来源：http://hz.svipenyu.cn/gtbmfesrrz.html

[T04] Kotlin：空安全
来源：http://hz.sufxvd.cn/gtdktgoiqy.html

val n: String? = null;  n?.length
来源：http://hz.shanyushiyangkeji.top/gtdispiusj.html

[T05] Kotlin：when 表达式
来源：http://hz.meibo888.top/gtnteqqvdm.html

val s = when (x) { 1 -> "一" else -> "其他" }   // 多分支时每个分支单独一行
来源：http://hz.zhijiandao.cn/gterzfzamh.html

[T06] Kotlin：集合映射
来源：http://hz.zhongyouzk.top/gtvvnyiheb.html

listOf(1, 2, 3).map { it * 2 }
来源：http://hz.nanxuanxn.top/gtuzkvtlce.html

[T07] Kotlin：集合过滤
来源：http://hz.nanxuanxn.top/gtyfteslld.html

listOf(1, 2, 3).filter { it > 1 }
来源：http://hz.yuanzhike.top/gtrztdtpol.html

[T08] Kotlin：数据类
来源：http://hz.gaohongyu789.top/gtndsfihju.html

data class User(val name: String, val age: Int)
来源：http://hz.dianchejie.cn/gtsacrsnnk.html

[T09] Kotlin：扩展函数
来源：http://hz.wangshuangyany.cn/gtmppuqhes.html

fun String.exclaim() = this + "!"
来源：http://hz.wangdashe.top/gtnakpomar.html

[T10] Kotlin：默认参数
来源：http://hz.yanxiufei.cn/gtuoiurnyx.html

fun greet(name: String = "World") = "Hi $name"
来源：http://hz.zhoulong.xyz/gtpqhlppuy.html

[T11] Kotlin：协程
来源：http://hz.xuetiantiany.cn/gtpvxtuhmg.html

GlobalScope.launch { delay(1000); println("done") }
来源：http://hz.316326.xyz/gtjvrjtjvc.html

[T12] Kotlin：解构声明
来源：http://hz.hnxiangtu.top/gtveddplry.html

val (a, b) = Pair(1, 2)
来源：http://hz.yanxiufei.cn/gtxeklcobo.html

[T13] Kotlin：只读 Map
来源：http://hz.sysykeji.top/gtpznqivsf.html

val m = mapOf("a" to 1)
来源：http://hz.gzhubu.top/gtmwryxkyp.html

[T14] Kotlin：循环
来源：http://hz.xylfe.cn/gtnbsozehr.html

for (i in 1..10) println(i)
来源：http://hz.ywan-chungtsiang.top/gtglwhimsw.html

[T15] Kotlin：接口
来源：http://hz.xylfe.cn/gtbicuzggl.html

interface Shape { fun area(): Double }
来源：http://hz.yueranfly.top/gttwwhxdia.html

[T16] Swift：Hello World
来源：http://hz.52xcode.cn/gtlzryghxk.html

print("Hello")
来源：http://hz.hnxiangtu.top/gtuzdlimty.html

[T17] Swift：变量与常量
来源：http://hz.yj20258.top/gtcswkyrcu.html

var a = 1;  let b = 2
来源：http://hz.sweek.top/gthoudycef.html

[T18] Swift：字符串插值
来源：http://hz.xziqi.cn/gtozfasrfz.html

"值: \(b)"
来源：http://hz.sysykeji.top/gtrbhhdwyb.html

[T19] Swift：可选绑定
来源：http://hz.pycfn.com/gtcyoqqwak.html

if let n = opt { print(n) }
来源：http://hz.havefunace.top/gtzfseiocr.html

[T20] Swift：数组操作
来源：http://hz.snrcjt.cn/gtbhxellda.html

var a = [1, 2, 3];  a.append(4)
来源：http://hz.sysykeji.top/gtbnigrwvt.html

[T21] Swift：遍历
来源：http://hz.jinyuanbaomall.cn/gthjfcyfoo.html

for x in a { print(x) }
来源：http://hz.wangshuangyany.cn/gtqvejxuyw.html

[T22] Swift：字典
来源：http://hz.cashguo.top/gtpktcoyic.html

var d = ["a": 1];  d["b"] = 2
来源：http://hz.dashuyun.cn/gtoxrjopvc.html

[T23] Swift：函数
来源：http://hz.yj20258888.top/gtctauhmtc.html

func add(_ a: Int, _ b: Int) -> Int { a + b }
来源：http://hz.aizwys.cn/gtlfdhvnqw.html

[T24] Swift：闭包
来源：http://hz.zycfv.cn/gtxaqulena.html

let f = { (x: Int) -> Int in x * 2 }
来源：http://hz.fengsongda.top/gtdxtbobfd.html

[T25] Swift：结构体
来源：http://hz.cqqwz.cn/gttskvdlrf.html

struct P { var x: Int }
来源：http://hz.xylfe.cn/gtvcmimusa.html

[T26] Swift：类与重写
来源：http://hz.shanyushiyangtech.top/gtjmfhjsde.html

class A: Base { override func f() {} }
来源：http://hz.aizwys.cn/gtcmyrejrq.html

[T27] Swift：错误处理
来源：http://hz.vqdsnc.cn/gtjkssgbzx.html

do { try f() } catch { print(error) }
来源：http://hz.redwolf501.top/gtawurbatz.html

[T28] Swift：枚举
来源：http://hz.ehwqpu.com/gtjvderarw.html

enum Color { case red, green }
来源：http://hz.hysaishi.cn/gtpyahcamw.html

[T29] Swift：guard 提前返回
来源：http://hz.svipenyu.cn/gtgybtjmei.html

guard let x = opt else { return }
来源：http://hz.ppjwa.cn/gtuokqfewv.html

[T30] Swift：协议
来源：http://hz.fengsongda.top/gtejksgikq.html

protocol Shape { func area() -> Double }
来源：http://hz.yj202588.top/gtbvlgvrlm.html

[T31] Lua：Hello World
来源：http://hz.cdnleiting.top/gtzqhqszlt.html

print("Hello")
来源：http://hz.hfpthk.cn/gtnpeeetkv.html

[T32] Lua：局部变量
来源：http://hz.zycfv.cn/gtiahqllct.html

local a = 1
来源：http://hz.bjfxy.top/gtxisccvty.html

[T33] Lua：表（数组）
来源：http://hz.yuxming.cn/gtrryeqrjm.html

local t = {1, 2, 3};  t[4] = 4
来源：http://hz.kuanghao11.cn/gtyunmcgul.html

[T34] Lua：遍历表
来源：http://hz.zycfv.cn/gtcolmqfek.html

for i, v in ipairs(t) do print(i, v) end
来源：http://hz.sweek.top/gtnzihkvex.html

[T35] Lua：字典表
来源：http://hz.gogol.net.cn/gtjsvczxdu.html

local d = { a = 1 };  d.b = 2
来源：http://hz.cheryme.top/gtyxqsqetn.html

[T36] Lua：函数
来源：http://hz.jqgfzy.top/gtnrlvlgew.html

function add(a, b) return a + b end
来源：http://hz.sweek.top/gteccygidn.html

[T37] Lua：字符串拼接
来源：http://hz.jqgfzy.top/gtnapdmpoi.html

"a" .. "b"
来源：http://hz.0kj1m.cn/gtuynpserz.html

[T38] Lua：条件
来源：http://hz.jinqigufen.top/gtquqqbhdu.html

if x > 0 then print("正") end
来源：http://hz.nwbrower.top/gtnkuskxdh.html

[T39] Lua：模式匹配
来源：http://hz.52xcode.cn/gtakiqccik.html

string.find(s, "%d+")
来源：http://hz.cdnleiting.top/gtuxzysptt.html

[T40] Lua：元表
来源：http://hz.jyoumei.cn/gtvxuircfj.html

setmetatable({}, { __index = base })
来源：http://hz.yuanzhike.top/gtmakrmuue.html

[T41] Perl：Hello World
来源：http://hz.cqqwz.cn/gtqntvlppe.html

print "Hello\n";
来源：http://hz.shanyushiyangtech.top/gtyxwhlsvm.html

[T42] Perl：变量类型
来源：http://hz.feifeiyinyue.top/gtwntydyjf.html

my $a = 1;  my @arr = (1, 2, 3);  my %h = (a => 1);
来源：http://hz.nanxinkj.top/gtkwpumxcm.html

[T43] Perl：字符串插值
来源：http://hz.birdmap.top/gtvaknbrwe.html

"值: $a"
来源：http://hz.redwolf501.top/gtypfmslna.html

[T44] Perl：条件
来源：http://hz.gotoacloud.top/gtcikrtnus.html

if ($a > 0) { print "正"; }
来源：http://hz.tanke756.top/gtlrrguzkq.html

[T45] Perl：数组遍历
来源：http://hz.snrcjt.cn/gtncmvasns.html

for my $x (@arr) { print $x; }
来源：http://hz.andypj.xyz/gtlobossom.html

[T46] Perl：哈希操作
来源：http://hz.shzxlz.cn/gtowuzgixc.html

$h{b} = 2;  for my $k (keys %h) { print "$k=$h{$k}"; }
来源：http://hz.dianchejie.cn/gtwpqvhphj.html

[T47] Perl：正则捕获
来源：http://hz.ybcxt.top/gtmfwzfayw.html

if ($s =~ /(\d+)/) { print $1; }
来源：http://hz.shanyushiyangkeji.top/gttposjzyf.html

[T48] Perl：正则替换
来源：http://hz.hnxiangtu.top/gtqqfcvtqm.html

$s =~ s/old/new/g;
来源：http://hz.wangshuangyany.cn/gtuqjloecf.html

[T49] Perl：函数
来源：http://hz.mhx1999.top/gthycadlet.html

sub add { my ($a, $b) = @_; return $a + $b; }
来源：http://hz.zhixingplan.top/gtaoixztiz.html

[T50] Perl：逐行读文件
来源：http://hz.hywenlv.cn/gtcyejzehx.html

open my $fh, "<", "a.txt" or die $!;
来源：http://hz.tanke756.top/gtafxicesm.html

while (my $line = <$fh>) { print $line; }
来源：http://hz.hfpthk.cn/gtolpmxeid.html

[T51] Scala：Hello World
来源：http://hz.316326.xyz/gtduorzkdt.html

println("Hello")
来源：http://hz.xuanzx.com/gttdkjzeak.html

[T52] Scala：变量
来源：http://hz.haohaochexian.top/gtecbqiywj.html

val a = 1;  var b = 2
来源：http://hz.52xcode.cn/gtlfwodrso.html

[T53] Scala：字符串插值
来源：http://hz.andypj.xyz/gtupqccpdy.html

s"值: $b"
来源：http://hz.daria6918.cn/gthqszqbby.html

[T54] Scala：集合映射
来源：http://hz.zhongyouzk.top/gtkceomamz.html

List(1, 2, 3).map(_ * 2)
来源：http://hz.jyoumei.cn/gtrdttliea.html

[T55] Scala：集合过滤
来源：http://hz.svipenyu.cn/gtyvhlbsyq.html

List(1, 2, 3).filter(_ > 1)
来源：http://hz.shzxlz.cn/gtdelkrykb.html

[T56] Scala：样例类
来源：http://hz.vqdsnc.cn/gtlnskadcu.html

case class User(name: String, age: Int)
来源：http://hz.yongpay.top/gtvsodnwgu.html

[T57] Scala：模式匹配
来源：http://hz.sweek.top/gtkyvywxxa.html

x match { case 1 => "一"; case _ => "其他" }
来源：http://hz.pengpengdd.cyou/gtovjasozy.html

[T58] Scala：函数定义
来源：http://hz.jinyuanbaomall.cn/gtakgwrgmk.html

def add(a: Int, b: Int): Int = a + b
来源：http://hz.nwbrower.top/gtelvrmyjt.html

[T59] Scala：循环
来源：http://hz.jinghuilouyu.cn/gttbrkortx.html

for (i <- 1 to 10) println(i)
来源：http://hz.chenjidiqi.icu/gthoyjacra.html

[T60] Scala：折叠
来源：http://hz.ydjk.org.cn/gtcauwvamz.html

List(1, 2, 3).foldLeft(0)(_ + _)
来源：http://hz.yj20258888.top/gtvcusvmwj.html

================================================================================
来源：http://hz.zhixingplan.top/gtidssifne.html

U. 高频实用片段（Python / PHP / JavaScript 各 40 条）
来源：http://hz.shanyushiyangtech.top/gtseyilowc.html

================================================================================
来源：http://hz.havefunace.top/gtdxnpvwac.html

[U01] Py：创建虚拟环境
来源：http://hz.haohaochexian.top/gtskrghmed.html

python -m venv .venv && source .venv/bin/activate
来源：http://hz.hammf.cn/gtnlhirqgp.html

[U02] Py：导出 / 安装依赖
来源：http://hz.quarkkingdee.top/gtemfpuysw.html

pip freeze > requirements.txt;  pip install -r requirements.txt
来源：http://hz.gzhubu.top/gtqcpjzlzz.html

[U03] Py：加载 .env 配置
来源：http://hz.zhijiandao.cn/gtaesawpzi.html

from dotenv import load_dotenv; load_dotenv()
来源：http://hz.ivvv.top/gtgdsjghoq.html

[U04] Py：变量调试打印
来源：http://hz.hammf.cn/gtveqpiazv.html

print(f"{x=}")            # 输出 x=值，Python 3.8+
来源：http://hz.zhixingplan.top/gthytuzmyt.html

[U05] Py：列表去重且保序
来源：http://hz.jiagoushi.top/gtauztasbn.html

list(dict.fromkeys(arr))
来源：http://hz.jianghu66.top/gtoojpqtug.html

[U06] Py：合并两个字典
来源：http://hz.jqgufenzy.top/gtrcfqfrio.html

{**a, **b}
来源：http://hz.jyoumei.cn/gtzmahdjfe.html

[U07] Py：反转字典键值
来源：http://hz.sufxvd.cn/gtppobdulg.html

{v: k for k, v in d.items()}
来源：http://hz.yueranfly.top/gtcuaahucc.html

[U08] Py：展平二维列表
来源：http://hz.gotoacloud.top/gtfnidfgii.html

[y for x in nested for y in x]
来源：http://hz.sweek.top/gtucywymcu.html

[U09] Py：字典取最大值的键
来源：http://hz.fengsongda.top/gtpxifgvvn.html

max(d, key=d.get)
来源：http://hz.snrcjt.cn/gtoynewjqe.html

[U10] Py：按值排序字典
来源：http://hz.sysykeji.top/gtpyasesjo.html

dict(sorted(d.items(), key=lambda kv: kv[1]))
来源：http://hz.yangfankeji.com/gtfhjcslvk.html

[U11] Py：生成器表达式
来源：http://hz.fengsongda.top/gtyljgbxal.html

(x * 2 for x in arr)
来源：http://hz.zhoulong.xyz/gtkjynxtlw.html

[U12] Py：取出现最多的 3 个元素
来源：http://hz.ywan-chungtsiang.top/gtzuylrcqj.html

Counter(arr).most_common(3)
来源：http://hz.chenlongwang.top/gtskoxhdav.html

[U13] Py：固定长度队列
来源：http://hz.hnxiangtu.top/gtihrtruhr.html

deque(maxlen=10)
来源：http://hz.guannengcc.top/gtzgplpiqd.html

[U14] Py：分组收集到列表
来源：http://hz.jinqigfzy.top/gtknzetkqy.html

defaultdict(list)
来源：http://hz.xuetiantiany.cn/gteealnnjh.html

[U15] Py：高精度计时
来源：http://hz.hnxiangtu.top/gtpuplssfe.html

t = time.perf_counter()
来源：http://hz.haohaochexian.top/gtrfzbgcxh.html

[U16] Py：命令行参数解析
来源：http://hz.yonumen.top/gtzhuklcwt.html

ap = argparse.ArgumentParser();  ap.add_argument("--name");  args = ap.parse_args()
来源：http://hz.yongpay.top/gtnljymqvs.html

[U17] Py：初始化日志
来源：http://hz.wangdashe.top/gtbqhkyeke.html

logging.basicConfig(level=logging.INFO)
来源：http://hz.gzhubu.top/gtnfjwuyst.html

[U18] Py：预编译正则
来源：http://hz.hnxiangtu.top/gtabtuzhcz.html

pat = re.compile(r"\d+")
来源：http://hz.gogol.net.cn/gtggpaojvc.html

[U19] Py：正则替换带回调
来源：http://hz.52xcode.cn/gtyaztodci.html

re.sub(r"\d+", lambda m: str(int(m.group()) * 2), s)
来源：http://hz.mhx1999.top/gtqedslsux.html

[U20] Py：缓存函数结果
来源：http://hz.zhongyouzk.top/gtcvlzxwlv.html

@functools.lru_cache(maxsize=None)
来源：http://hz.svipenyu.cn/gtjpgmtwmr.html

[U21] Py：自定义上下文管理器
来源：http://hz.yonumen.top/gtwqcwxqao.html

@contextlib.contextmanager
来源：http://hz.xziqi.cn/gtgllcrhyk.html

[U22] Py：矩阵转置
来源：http://hz.cashguo.top/gtxmwmxdzx.html

list(zip(*m))
来源：http://hz.zhaomingkeji.xyz/gtrhnqshog.html

[U23] Py：分块读取大文件
来源：http://hz.gotoacloud.top/gtehcaameq.html

for chunk in iter(lambda: f.read(8192), b""):
来源：http://hz.sufxvd.cn/gtzeekmtld.html

[U24] Py：路径操作
来源：http://hz.quarkkingdee.top/gtvbxjpyxq.html

Path("a/b.txt").parent.mkdir(parents=True, exist_ok=True)
来源：http://hz.jlsjyb.cn/gtpmwebbzn.html

[U25] Py：CSV 按字典读
来源：http://hz.c1oappe.top/gtzxwcnuzx.html

csv.DictReader(f)
来源：http://hz.ivvv.top/gttgxgtrbl.html

[U26] Py：并发下载
来源：http://hz.cheryme.top/gtxlowvdkt.html

ThreadPoolExecutor(max_workers=8).map(fetch, urls)
来源：http://hz.guowangkeji.top/gtsqmkjprd.html

[U27] Py：异步 HTTP
来源：http://hz.wangdashe.top/gtumoyxjqg.html

aiohttp.ClientSession() 配合 async with
来源：http://hz.tian-w.cn/gtcupgjhdr.html

[U28] Py：类型别名
来源：http://hz.andypj.xyz/gtakexpslr.html

UserId = int
来源：http://hz.zycfv.cn/gtealzsfrq.html

[U29] Py：属性校验
来源：http://hz.daxiang520.top/gtragnlxng.html

@property 与 @x.setter 配合
来源：http://hz.316326.xyz/gtuqvayedg.html

[U30] Py：数据类
来源：http://hz.sysykeji.top/gtyosijqot.html

@dataclass(slots=True)
来源：http://hz.zycfv.cn/gtqdvmfjkf.html

[U31] Py：单测
来源：http://hz.hnqzz.top/gtuwnxxcvt.html

python -m pytest -q
来源：http://hz.bjfxy.top/gtgnadudbm.html

[U32] Py：代码格式化
来源：http://hz.sxryk.cn/gtwlafhlkj.html

ruff format . && ruff check --fix .
来源：http://hz.jlsjyb.cn/gtrmbkmwme.html

[U33] Py：打包发布
来源：http://hz.cheryme.top/gtlixnfhaz.html

python -m build  （依赖 pyproject.toml）
来源：http://hz.jinyuanbaomall.cn/gtogkblzgl.html

[U34] Py：判断编码
来源：http://hz.ywan-chungtsiang.top/gtefisrskt.html

chardet.detect(raw)
来源：http://hz.zhengqikj.top/gtbwlsptgc.html

[U35] Py：发送邮件
来源：http://hz.zdqjudy.top/gthsylpizx.html

smtplib.SMTP_SSL(...).send_message(msg)
来源：http://hz.shanyushiyangtech.top/gtwtmicebe.html

[U36] Py：定时任务
来源：http://hz.zdqjudy.top/gtsxambeci.html

schedule.every(10).minutes.do(job)
来源：http://hz.ivvv.top/gtsumnptqa.html

[U37] Py：读写 Excel
来源：http://hz.0kj1m.cn/gtpuxvwxzm.html

pandas.read_excel / DataFrame.to_excel
来源：http://hz.wangshuangyany.cn/gtixcwtoiw.html

[U38] Py：获取脚本所在目录
来源：http://hz.sweek.top/gtutkvzkel.html

Path(__file__).resolve().parent
来源：http://hz.9152youxi.cn/gtiinvnllf.html

[U39] Py：判断是否在交互环境
来源：http://hz.mhx1999.top/gtzdwekjwa.html

sys.stdout.isatty()
来源：http://hz.xziqi.cn/gtvxtyshdc.html

[U40] Py：打印到标准错误
来源：http://hz.0kj1m.cn/gtjqtjuefe.html

print("err", file=sys.stderr)
来源：http://hz.ybcxt.top/gtkuhdvkni.html

[U41] PHP：初始化 Composer 项目
来源：http://hz.shzxlz.cn/gtlqayklps.html

composer init;  composer require guzzlehttp/guzzle
来源：http://hz.xuanzx.com/gtgwlfnvhr.html

[U42] PHP：PSR-4 自动加载
来源：http://hz.zhijiandao.cn/gthobkebpw.html

"autoload": { "psr-4": { "App\\": "src/" } }
来源：http://hz.xuanzx.com/gtnppdrvcz.html

[U43] PHP：声明命名空间
来源：http://hz.cqqwz.cn/gtjfmhweff.html

namespace App\Http;
来源：http://hz.hysaishi.cn/gtlpnnnxgd.html

[U44] PHP：开启严格类型
来源：http://hz.sysykeji.top/gtjtipgzir.html

declare(strict_types=1);
来源：http://hz.pengpengdd.cyou/gtmqlygdqn.html

[U45] PHP：类型声明与返回类型
来源：http://hz.hfpthk.cn/gtcrnldbxq.html

function add(int $a, int $b): int { return $a + $b; }
来源：http://hz.nanxuanxn.top/gthksixgdw.html

[U46] PHP：可空类型
来源：http://hz.0kj1m.cn/gtcpwomfeh.html

?string $name = null
来源：http://hz.tian-w.cn/gtisdaouxt.html

[U47] PHP：联合类型
来源：http://hz.iojbl.cn/gtkeqejmpb.html

int|string $id
来源：http://hz.guowangkeji.top/gtydxqzytj.html

[U48] PHP：纯枚举
来源：http://hz.nanxinkj.top/gtxxajduqh.html

enum Status: string { case Active = "active"; case Off = "off"; }
来源：http://hz.jinyuanbaomall.cn/gtivmboasv.html

[U49] PHP：只读属性
来源：http://hz.smart0.xyz/gtxrfqwlbj.html

public readonly string $name
来源：http://hz.zhaomingkeji.xyz/gtpmaibtbi.html

[U50] PHP：构造器属性提升
来源：http://hz.hfpthk.cn/gtgxxkzzai.html

public function __construct(private int $id) {}
来源：http://hz.shanyushiyangtech.top/gtzdbdjazu.html

[U51] PHP：数组解构
来源：http://hz.gotoacloud.top/gtgwixzlof.html

[$a, $b] = $arr;
来源：http://hz.smart0.xyz/gtedmgurxs.html

[U52] PHP：箭头函数
来源：http://hz.gzhubu.top/gtdnxlvjwr.html

$double = fn($x) => $x * 2;
来源：http://hz.shanyushiyangtech.top/gtpsizimhb.html

[U53] PHP：空合并运算符
来源：http://hz.zycfv.cn/gtbpnfiaya.html

$v = $a ?? $b ?? "default";
来源：http://hz.daria6918.cn/gtraljryte.html

[U54] PHP：空安全调用
来源：http://hz.meibo888.top/gtrcenokgq.html

$obj?->method()
来源：http://hz.0kj1m.cn/gtjfpiytde.html

[U55] PHP：match 表达式
来源：http://hz.shzxlz.cn/gtsyxkxnpo.html

$s = match($x) { 1 => "一", default => "其他" };
来源：http://hz.yj20258888.top/gttawjfsip.html

[U56] PHP：命名参数
来源：http://hz.yj20258888.top/gtymruepvc.html

f(a: 1, b: 2)
来源：http://hz.guannengcc.top/gtxogpwcyy.html


<!-- 参考信息 -->