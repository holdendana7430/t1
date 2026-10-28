代发 wailian999

atoi("42");  strtod("3.14", NULL);
来源：http://hz.yuxming.cn/gtdtqntajo.html

[S23] C：随机数
来源：http://hz.bjfxy.top/gtlxydcgnf.html

srand(time(NULL));  int r = rand() % 100;
来源：http://hz.fzhhl.top/gtududzrhk.html

[S24] C：获取本地时间
来源：http://hz.yvedp.cn/gtpimoeemh.html

time_t t = time(NULL);  struct tm *tm = localtime(&t);
来源：http://hz.9152youxi.cn/gtkdfutupo.html

[S25] C：内存拷贝
来源：http://hz.pycfn.com/gtwthainhn.html

memcpy(dst, src, n);
来源：http://hz.0kj1m.cn/gtpkqccqfi.html

[S26] C：内存清零
来源：http://hz.fzhhl.top/gtlybggjmz.html

memset(a, 0, sizeof a);
来源：http://hz.bjfxy.top/gtkybhvdoh.html

[S27] C：定义常量
来源：http://hz.daxiang520.top/gtpwlwcqva.html

const double PI = 3.14159;
来源：http://hz.52xcode.cn/gtxpuwmbtu.html

[S28] C：静态变量
来源：http://hz.tanke756.top/gttubyjbey.html

static int counter = 0;
来源：http://hz.sweek.top/gtenakukby.html

[S29] C：变参函数
来源：http://hz.zhoulong.xyz/gtazyapldb.html

va_list ap; va_start(ap, fmt); vprintf(fmt, ap); va_end(ap);
来源：http://hz.zhixingplan.top/gtstheshis.html

[S30] C：头文件保护
来源：http://hz.cashguo.top/gtcwunsjma.html

#ifndef X_H
来源：http://hz.andypj.xyz/gtxpmupyqw.html

#define X_H
来源：http://hz.cheryme.top/gtvleeuqsg.html

#endif
来源：http://hz.fengsongda.top/gtygbzkdlz.html

[S31] C++：Hello World
来源：http://hz.bjfxy.top/gttkfqkhvj.html

#include <iostream>
来源：http://hz.ivvv.top/gtvnmtegzn.html

int main() { std::cout << "Hello\n"; }
来源：http://hz.fzhhl.top/gtxpucylrg.html

[S32] C++：字符串
来源：http://hz.dashuyun.cn/gtrbxnhcax.html

std::string s = "hi";  s += "!";
来源：http://hz.wangdashe.top/gtfgsbmmbg.html

[S33] C++：vector 增删
来源：http://hz.jqgfzy.top/gtfrsaxbjo.html

std::vector<int> v{1, 2, 3};  v.push_back(4);
来源：http://hz.snrcjt.cn/gthwlffkgj.html

[S34] C++：遍历 vector
来源：http://hz.jianghu66.top/gtgpbowotl.html

for (auto &x : v) { std::cout << x; }
来源：http://hz.hnxiangtu.top/gtsiejbukb.html

[S35] C++：map
来源：http://hz.sxryk.cn/gtewlrmsgn.html

std::map<std::string, int> m;  m["a"] = 1;
来源：http://hz.zycfv.cn/gtnvctniyl.html

[S36] C++：unordered_map
来源：http://hz.0kj1m.cn/gtkwvhnneq.html

std::unordered_map<std::string, int> m;  m["a"] = 1;
来源：http://hz.tanke756.top/gtrktwvdfj.html

[S37] C++：set
来源：http://hz.tanke756.top/gtinxwjofs.html

std::set<int> s{1, 2, 3};  s.insert(4);
来源：http://hz.feifeiyinyue.top/gtlxzexgpy.html

[S38] C++：排序
来源：http://hz.chenjidiqi.icu/gtqzrynqev.html

std::sort(v.begin(), v.end());
来源：http://hz.ppjwa.cn/gtsjqsmpbs.html

[S39] C++：自定义比较器排序
来源：http://hz.havefunace.top/gtjgoiymeo.html

std::sort(v.begin(), v.end(), [](int a, int b) { return a > b; });
来源：http://hz.52xcode.cn/gtsvszsxrj.html

[S40] C++：查找元素
来源：http://hz.gotoacloud.top/gtiiytlcyq.html

auto it = std::find(v.begin(), v.end(), 3);
来源：http://hz.jqgufenzy.top/gtapjrufpv.html

[S41] C++：类与构造函数
来源：http://hz.shangyingyoupin.top/gtiwetdtsv.html

class A { public: A(int v) : x_(v) {} int get() const { return x_; } private: int x_; };
来源：http://hz.yanxiufei.cn/gtnilmtenp.html

[S42] C++：继承与虚函数
来源：http://hz.zhoulong.xyz/gtydgorgze.html

class B : public Base { public: void f() override {} };
来源：http://hz.hongshengwenyu.top/gtfaxpzchl.html

[S43] C++：智能指针
来源：http://hz.zhiwuduotai.top/gtoypfdjcy.html

auto p = std::make_unique<int>(5);
来源：http://hz.shangyingyoupin.top/gtwadvyswq.html

[S44] C++：引用传参
来源：http://hz.yanxiufei.cn/gtzlsoumpi.html

void inc(int &x) { ++x; }
来源：http://hz.yvedp.cn/gtltsvorku.html

[S45] C++：lambda
来源：http://hz.jinghuilouyu.cn/gtjurswwmy.html

auto add = [](int a, int b) { return a + b; };
来源：http://hz.shzxlz.cn/gteekozjys.html

[S46] C++：函数模板
来源：http://hz.zhongyouzk.top/gtqmfuccpq.html

template <typename T> T maxv(T a, T b) { return a > b ? a : b; }
来源：http://hz.hnqzz.top/gtynhlgyjz.html

[S47] C++：结构化绑定遍历
来源：http://hz.daria6918.cn/gtmbdigeod.html

for (const auto &[k, v] : m) { std::cout << k << v; }
来源：http://hz.pycfn.com/gtebnmkggi.html

[S48] C++：逐行读文件
来源：http://hz.jinqigfzy.top/gtinjvvcuq.html

std::ifstream in("a.txt");  std::string line;
来源：http://hz.yonumen.top/gtxinsbsjt.html

while (std::getline(in, line)) { }
来源：http://hz.pycfn.com/gthufeywnt.html

[S49] C++：写文件
来源：http://hz.aibaodan.cn/gtnexelcix.html

std::ofstream out("a.txt");  out << "hi\n";
来源：http://hz.vqdsnc.cn/gtcutflwre.html

[S50] C++：格式化数字
来源：http://hz.hnxiangtu.top/gtndorppvd.html

std::ostringstream os;  os << std::fixed << std::setprecision(2) << 3.14159;
来源：http://hz.snrcjt.cn/gtrzigihwf.html

[S51] C++：显式类型转换
来源：http://hz.xylfe.cn/gtvwvnzycl.html

static_cast<double>(a) / b
来源：http://hz.yuanzhike.top/gtwzyzbxta.html

[S52] C++：const 与 noexcept
来源：http://hz.zhaomingkeji.xyz/gtenfxefqg.html

int size() const noexcept { return n_; }
来源：http://hz.yuxming.cn/gtiioilaef.html

[S53] C++：移动语义
来源：http://hz.birdmap.top/gtnygykevu.html

std::vector<int> w = std::move(v);
来源：http://hz.yongpay.top/gtewgahwmo.html

[S54] C++：异常处理
来源：http://hz.wangshuangyany.cn/gtbhkbdcho.html

try { throw std::runtime_error("x"); } catch (const std::exception &e) { }
来源：http://hz.tian-w.cn/gtlekomrtp.html

[S55] C++：结构化绑定
来源：http://hz.jqgfzy.top/gtxxlqrvng.html

auto [a, b] = std::make_pair(1, 2);
来源：http://hz.daxiang520.top/gttrimmzyr.html

[S56] C++：optional
来源：http://hz.sufxvd.cn/gtlznwcdyd.html

std::optional<int> o = 5;  if (o) { int v = *o; }
来源：http://hz.jqgfzy.top/gtnecyrthl.html

[S57] C++：编译期常量
来源：http://hz.yueranfly.top/gtctijkiyo.html

constexpr int N = 10;
来源：http://hz.yueranfly.top/gtvpoqqepj.html

[S58] C++：命名空间
来源：http://hz.daxiang520.top/gtbxarfjvz.html

namespace ns { int f() { return 1; } }
来源：http://hz.shanyushiyangkeji.top/gtqjkqnrim.html

[S59] C++：静态断言
来源：http://hz.xziqi.cn/gtloultrfq.html

static_assert(sizeof(int) == 4, "int 必须 4 字节");
来源：http://hz.52xcode.cn/gtnwrxwvqy.html

[S60] C++：遍历并删除元素
来源：http://hz.jqgfzy.top/gtmbvyxdyq.html

v.erase(std::remove_if(v.begin(), v.end(), [](int x) { return x < 0; }), v.end());
来源：http://hz.svipenyu.cn/gtahbznply.html

================================================================================
来源：http://hz.chenjidiqi.icu/gtqvrmkken.html

T. 其他语言补充（Kotlin / Swift / Lua / Perl / Scala）
来源：http://hz.zycfv.cn/gtvehnrntt.html

================================================================================
来源：http://hz.hnxiangtu.top/gtgzbkvlhk.html

[T01] Kotlin：Hello World
来源：http://hz.jinqigufen.top/gtdrhoehin.html

println("Hello")
来源：http://hz.dianchejie.cn/gtiiiljjhk.html

[T02] Kotlin：变量
来源：http://hz.yueranfly.top/gtujneqeyk.html

val a = 1;  var b = 2        // val 只读，var 可变
来源：http://hz.svipenyu.cn/gtyjublory.html

[T03] Kotlin：字符串模板
来源：http://hz.daxiang520.top/gtusrzuzkq.html

"值: $b"
来源：http://hz.316326.xyz/gtptheplji.html

[T04] Kotlin：空安全
来源：http://hz.nwbrower.top/gthfradcxe.html

val n: String? = null;  n?.length
来源：http://hz.cqqwz.cn/gtgtdwafvm.html

[T05] Kotlin：when 表达式
来源：http://hz.andypj.xyz/gtijfjjmdv.html

val s = when (x) { 1 -> "一" else -> "其他" }   // 多分支时每个分支单独一行
来源：http://hz.tianlin.xyz/gtegzquyhd.html

[T06] Kotlin：集合映射
来源：http://hz.sysykeji.top/gtiamaljro.html

listOf(1, 2, 3).map { it * 2 }
来源：http://hz.yvedp.cn/gttcamdspb.html

[T07] Kotlin：集合过滤
来源：http://hz.iojbl.cn/gthryaupta.html

listOf(1, 2, 3).filter { it > 1 }
来源：http://hz.jinqigfzy.top/gtmpksjpml.html

[T08] Kotlin：数据类
来源：http://hz.zdqjudy.top/gtiotjciyb.html

data class User(val name: String, val age: Int)
来源：http://hz.zhaomingkeji.xyz/gtqjhpwaxg.html

[T09] Kotlin：扩展函数
来源：http://hz.shanyushiyangkeji.top/gtegdycoke.html

fun String.exclaim() = this + "!"
来源：http://hz.meibo888.top/gtsduhleyd.html

[T10] Kotlin：默认参数
来源：http://hz.zhiwuduotai.top/gtplzgfhfz.html

fun greet(name: String = "World") = "Hi $name"
来源：http://hz.wangdashe.top/gtkehvwzsl.html

[T11] Kotlin：协程
来源：http://hz.fzhhl.top/gtsrcmsvbn.html

GlobalScope.launch { delay(1000); println("done") }
来源：http://hz.sxryk.cn/gtrytuzmwg.html

[T12] Kotlin：解构声明
来源：http://hz.fengsongda.top/gtfeaehgsl.html

val (a, b) = Pair(1, 2)
来源：http://hz.ehwqpu.com/gtehschkaz.html

[T13] Kotlin：只读 Map
来源：http://hz.smart0.xyz/gtvynfotcp.html

val m = mapOf("a" to 1)
来源：http://hz.yj20258.top/gtxclyeqwi.html

[T14] Kotlin：循环
来源：http://hz.zhijiandao.cn/gtxfahubjo.html

for (i in 1..10) println(i)
来源：http://hz.cashguo.top/gtfmprtdmv.html

[T15] Kotlin：接口
来源：http://hz.vqdsnc.cn/gtpvdquctk.html

interface Shape { fun area(): Double }
来源：http://hz.haohaochexian.top/gtkqwrnceg.html

[T16] Swift：Hello World
来源：http://hz.yangfankeji.com/gtwbykazot.html

print("Hello")
来源：http://hz.daria6918.cn/gtjutfebzt.html

[T17] Swift：变量与常量
来源：http://hz.jianghu66.top/gtpyohmphx.html

var a = 1;  let b = 2
来源：http://hz.chenzaomai.com/gtfqmkvrtk.html

[T18] Swift：字符串插值
来源：http://hz.jyoumei.cn/gtfltskkru.html

"值: \(b)"
来源：http://hz.redwolf501.top/gtddzlpzup.html

[T19] Swift：可选绑定
来源：http://hz.haohaochexian.top/gtzcbrshdd.html

if let n = opt { print(n) }
来源：http://hz.pycfn.com/gtoxhoznjb.html

[T20] Swift：数组操作
来源：http://hz.sweek.top/gtjoffbjmd.html

var a = [1, 2, 3];  a.append(4)
来源：http://hz.shzxlz.cn/gtzjmwgdic.html

[T21] Swift：遍历
来源：http://hz.zhengqikj.top/gtnvqnpxdc.html

for x in a { print(x) }
来源：http://hz.nwbrower.top/gtjgzicyli.html

[T22] Swift：字典
来源：http://hz.zhixingplan.top/gtuilsvolo.html

var d = ["a": 1];  d["b"] = 2
来源：http://hz.jinyuanbaomall.cn/gtmoziyvce.html

[T23] Swift：函数
来源：http://hz.0kj1m.cn/gtxbfgtwiu.html

func add(_ a: Int, _ b: Int) -> Int { a + b }
来源：http://hz.52xcode.cn/gtbksjowjz.html

[T24] Swift：闭包
来源：http://hz.zhongyouzk.top/gtffornnxb.html

let f = { (x: Int) -> Int in x * 2 }
来源：http://hz.cheryme.top/gtfqwfzxfw.html

[T25] Swift：结构体
来源：http://hz.yangfankeji.com/gtlelxccke.html

struct P { var x: Int }
来源：http://hz.vqdsnc.cn/gtmpijcolz.html

[T26] Swift：类与重写
来源：http://hz.chenzaomai.com/gtzdgqfhwk.html

class A: Base { override func f() {} }
来源：http://hz.jyoumei.cn/gtqrwdsdur.html

[T27] Swift：错误处理
来源：http://hz.wangshuangyany.cn/gtsgdtkgzb.html

do { try f() } catch { print(error) }
来源：http://hz.zycfv.cn/gtpdmdaoae.html

[T28] Swift：枚举
来源：http://hz.yj202588.top/gttzodrbcm.html

enum Color { case red, green }
来源：http://hz.snrcjt.cn/gtmqyfoqmg.html

[T29] Swift：guard 提前返回
来源：http://hz.ivvv.top/gtvwkfftcl.html

guard let x = opt else { return }
来源：http://hz.andypj.xyz/gtywffvsfm.html

[T30] Swift：协议
来源：http://hz.nanxuanxn.top/gtavzciurt.html

protocol Shape { func area() -> Double }
来源：http://hz.hfpthk.cn/gthupsraoj.html

[T31] Lua：Hello World
来源：http://hz.yueranfly.top/gtkdbovfau.html

print("Hello")
来源：http://hz.jianghu66.top/gtlcyrsyqh.html

[T32] Lua：局部变量
来源：http://hz.shangyingyoupin.top/gtmfokfxlm.html

local a = 1
来源：http://hz.0kj1m.cn/gtigstjskh.html

[T33] Lua：表（数组）
来源：http://hz.dashuyun.cn/gtdtitdrot.html

local t = {1, 2, 3};  t[4] = 4
来源：http://hz.hammf.cn/gtzbhssahz.html

[T34] Lua：遍历表
来源：http://hz.jinqigfzy.top/gtxtiwvawa.html

for i, v in ipairs(t) do print(i, v) end
来源：http://hz.pengpengdd.cyou/gtzjcshgst.html

[T35] Lua：字典表
来源：http://hz.snrcjt.cn/gtshxaqdkx.html

local d = { a = 1 };  d.b = 2
来源：http://hz.jyoumei.cn/gtvgoaoshk.html

[T36] Lua：函数
来源：http://hz.zhengqikj.top/gtzxdhcmad.html

function add(a, b) return a + b end
来源：http://hz.guannengcc.top/gtydtxzosg.html

[T37] Lua：字符串拼接
来源：http://hz.yuxming.cn/gtlqdtgbtl.html

"a" .. "b"
来源：http://hz.yongpay.top/gtkaokivhg.html

[T38] Lua：条件
来源：http://hz.yongpay.top/gtivrznkzn.html

if x > 0 then print("正") end
来源：http://hz.wangdashe.top/gtrryeoonk.html

[T39] Lua：模式匹配
来源：http://hz.9152youxi.cn/gtmisnbzqe.html

string.find(s, "%d+")
来源：http://hz.zhoulong.xyz/gtqiavwdfi.html

[T40] Lua：元表
来源：http://hz.jiagoushi.top/gtszjdocso.html

setmetatable({}, { __index = base })
来源：http://hz.daria6918.cn/gtkyhvfewj.html

[T41] Perl：Hello World
来源：http://hz.hnxiangtu.top/gtzlizydun.html

print "Hello\n";
来源：http://hz.gaohongyu789.top/gtaugxufkg.html

[T42] Perl：变量类型
来源：http://hz.chenlongwang.top/gtfgkyurax.html

my $a = 1;  my @arr = (1, 2, 3);  my %h = (a => 1);
来源：http://hz.yueranfly.top/gtfaezzott.html

[T43] Perl：字符串插值
来源：http://hz.aizwys.cn/gtrludlwyk.html

"值: $a"
来源：http://hz.vqdsnc.cn/gtvaokkini.html

[T44] Perl：条件
来源：http://hz.chenlongwang.top/gtnfiwyqqq.html

if ($a > 0) { print "正"; }
来源：http://hz.zdqjudy.top/gtydegtugj.html

[T45] Perl：数组遍历
来源：http://hz.jyoumei.cn/gttrgyrehd.html

for my $x (@arr) { print $x; }
来源：http://hz.wangshuangyany.cn/gtqbqpujkn.html

[T46] Perl：哈希操作
来源：http://hz.guowangkeji.top/gtffqmsgew.html

$h{b} = 2;  for my $k (keys %h) { print "$k=$h{$k}"; }
来源：http://hz.zycfv.cn/gtuwinxmns.html

[T47] Perl：正则捕获
来源：http://hz.birdmap.top/gtzixleacb.html

if ($s =~ /(\d+)/) { print $1; }
来源：http://hz.daxiang520.top/gtqvdeklko.html

[T48] Perl：正则替换
来源：http://hz.quarkkingdee.top/gtdicigqny.html

$s =~ s/old/new/g;
来源：http://hz.haohaochexian.top/gtcimmpaou.html

[T49] Perl：函数
来源：http://hz.zdqjudy.top/gtpkgmetcv.html

sub add { my ($a, $b) = @_; return $a + $b; }
来源：http://hz.nanxinkj.top/gtgawinlvi.html

[T50] Perl：逐行读文件
来源：http://hz.gzhubu.top/gtovjsrmna.html

open my $fh, "<", "a.txt" or die $!;
来源：http://hz.hnxiangtu.top/gtklnknpmq.html

while (my $line = <$fh>) { print $line; }
来源：http://hz.quarkkingdee.top/gtofkkrbbd.html

[T51] Scala：Hello World
来源：http://hz.pycfn.com/gthcpvwbug.html

println("Hello")
来源：http://hz.ivvv.top/gtfttvkqpp.html

[T52] Scala：变量
来源：http://hz.yangfankeji.com/gthaeewbzr.html

val a = 1;  var b = 2
来源：http://hz.wangdashe.top/gtxkebfzzg.html

[T53] Scala：字符串插值
来源：http://hz.yonumen.top/gtqwgzxmhx.html

s"值: $b"
来源：http://hz.gaohongyu789.top/gtjdjkklwp.html

[T54] Scala：集合映射
来源：http://hz.aizwys.cn/gtltuulcia.html

List(1, 2, 3).map(_ * 2)
来源：http://hz.jqgfzy.top/gtbsfzfaqt.html

[T55] Scala：集合过滤
来源：http://hz.sufxvd.cn/gtfaxywvcg.html

List(1, 2, 3).filter(_ > 1)
来源：http://hz.iojbl.cn/gtuotcyzwe.html

[T56] Scala：样例类
来源：http://hz.shzxlz.cn/gtspgcqdrt.html

case class User(name: String, age: Int)
来源：http://hz.jqgufenzy.top/gtkzfjclqx.html

[T57] Scala：模式匹配
来源：http://hz.tanke756.top/gthokpmpki.html

x match { case 1 => "一"; case _ => "其他" }
来源：http://hz.vqdsnc.cn/gtuextsrlj.html

[T58] Scala：函数定义
来源：http://hz.zhengqikj.top/gthyophziw.html

def add(a: Int, b: Int): Int = a + b
来源：http://hz.xziqi.cn/gtptsyivjw.html

[T59] Scala：循环
来源：http://hz.jinghuilouyu.cn/gtugzvjups.html

for (i <- 1 to 10) println(i)
来源：http://hz.nanxinkj.top/gthghgnipw.html

[T60] Scala：折叠
来源：http://hz.wangshuangyany.cn/gtwwuqrnjh.html

List(1, 2, 3).foldLeft(0)(_ + _)
来源：http://hz.ywan-chungtsiang.top/gtcmwwonko.html

================================================================================
来源：http://hz.feifeiyinyue.top/gtifshtexu.html

U. 高频实用片段（Python / PHP / JavaScript 各 40 条）
来源：http://hz.jyoumei.cn/gtogxpztmj.html

================================================================================
来源：http://hz.nanxinkj.top/gtkpypvzpz.html

[U01] Py：创建虚拟环境
来源：http://hz.quarkkingdee.top/gtffhxhlxu.html

python -m venv .venv && source .venv/bin/activate
来源：http://hz.fengsongda.top/gthmopkujv.html

[U02] Py：导出 / 安装依赖
来源：http://hz.jyoumei.cn/gtisldveeu.html

pip freeze > requirements.txt;  pip install -r requirements.txt
来源：http://hz.zhiwuduotai.top/gtsfkrawmm.html

[U03] Py：加载 .env 配置
来源：http://hz.ywan-chungtsiang.top/gtlazpbygw.html

from dotenv import load_dotenv; load_dotenv()
来源：http://hz.ydjk.org.cn/gtzqfwwect.html

[U04] Py：变量调试打印
来源：http://hz.jyoumei.cn/gtjhhylgdn.html

print(f"{x=}")            # 输出 x=值，Python 3.8+
来源：http://hz.ywan-chungtsiang.top/gtdowtoyye.html

[U05] Py：列表去重且保序
来源：http://hz.andypj.xyz/gtrkmvvqry.html

list(dict.fromkeys(arr))
来源：http://hz.jinqigfzy.top/gtqmcvgqlb.html

[U06] Py：合并两个字典
来源：http://hz.fengsongda.top/gtkycmkggf.html

{**a, **b}
来源：http://hz.fzhhl.top/gtyrbyyeru.html

[U07] Py：反转字典键值
来源：http://hz.zhengqikj.top/gtzlraddqi.html

{v: k for k, v in d.items()}
来源：http://hz.zhongyouzk.top/gtaxvbdbmr.html

[U08] Py：展平二维列表
来源：http://hz.tianlin.xyz/gtxcfggabs.html

[y for x in nested for y in x]
来源：http://hz.xuanzx.com/gtegwxsmrh.html

[U09] Py：字典取最大值的键
来源：http://hz.jinqigfzy.top/gtzqqetcrq.html

max(d, key=d.get)
来源：http://hz.gotoacloud.top/gtxiuyexsz.html

[U10] Py：按值排序字典
来源：http://hz.yj202588.top/gtwezkayai.html

dict(sorted(d.items(), key=lambda kv: kv[1]))
来源：http://hz.nanxuanxn.top/gtaglplzau.html

[U11] Py：生成器表达式
来源：http://hz.kuanghao11.cn/gtavpodium.html

(x * 2 for x in arr)
来源：http://hz.zycfv.cn/gtzbejuxaj.html

[U12] Py：取出现最多的 3 个元素
来源：http://hz.jinyuanbaomall.cn/gtaopdihwh.html

Counter(arr).most_common(3)
来源：http://hz.hongshengwenyu.top/gtdoxhinwd.html

[U13] Py：固定长度队列
来源：http://hz.zhaomingkeji.xyz/gtwtdkyxik.html

deque(maxlen=10)
来源：http://hz.yj20258888.top/gtlyjvorar.html

[U14] Py：分组收集到列表
来源：http://hz.jqgufenzy.top/gthwjwybml.html

defaultdict(list)
来源：http://hz.yonumen.top/gtmcudhdbf.html

[U15] Py：高精度计时
来源：http://hz.ybcxt.top/gtsmeyppkq.html

t = time.perf_counter()
来源：http://hz.pengpengdd.cyou/gttradxloe.html

[U16] Py：命令行参数解析
来源：http://hz.sxryk.cn/gtzybkxfea.html

ap = argparse.ArgumentParser();  ap.add_argument("--name");  args = ap.parse_args()
来源：http://hz.haohaochexian.top/gtkequkrgj.html

[U17] Py：初始化日志
来源：http://hz.xinyue.icu/gtlqmffwji.html

logging.basicConfig(level=logging.INFO)
来源：http://hz.chenlongwang.top/gtcrqspbhk.html

[U18] Py：预编译正则
来源：http://hz.zdqjudy.top/gtzhbmzfac.html

pat = re.compile(r"\d+")
来源：http://hz.hammf.cn/gtsnkxqsqi.html

[U19] Py：正则替换带回调
来源：http://hz.hammf.cn/gtliokkxmr.html

re.sub(r"\d+", lambda m: str(int(m.group()) * 2), s)
来源：http://hz.haohaochexian.top/gtearfisfh.html

[U20] Py：缓存函数结果
来源：http://hz.316326.xyz/gtliuegkfg.html

@functools.lru_cache(maxsize=None)
来源：http://hz.xinyue.icu/gtextggolt.html

[U21] Py：自定义上下文管理器
来源：http://hz.ivvv.top/gtxgvwcovj.html

@contextlib.contextmanager
来源：http://hz.cucudq.cn/gtmozyhyby.html

[U22] Py：矩阵转置
来源：http://hz.gaohongyu789.top/gtdmebuxev.html

list(zip(*m))
来源：http://hz.9152youxi.cn/gtijbffphb.html

[U23] Py：分块读取大文件
来源：http://hz.gzhubu.top/gtsmphysjm.html

for chunk in iter(lambda: f.read(8192), b""):
来源：http://hz.ydzc1.top/gtzpjmrvev.html

[U24] Py：路径操作
来源：http://hz.kuanghao11.cn/gttrvlskzr.html

Path("a/b.txt").parent.mkdir(parents=True, exist_ok=True)
来源：http://hz.aizwys.cn/gtxeaokdgq.html

[U25] Py：CSV 按字典读
来源：http://hz.aibaodan.cn/gtqzrvcymh.html

csv.DictReader(f)
来源：http://hz.ywan-chungtsiang.top/gtumsaeiqq.html

[U26] Py：并发下载
来源：http://hz.feifeiyinyue.top/gthjxlomks.html

ThreadPoolExecutor(max_workers=8).map(fetch, urls)
来源：http://hz.wangshuangyany.cn/gtfefwktep.html

[U27] Py：异步 HTTP
来源：http://hz.jinghuilouyu.cn/gtinmmvrev.html

aiohttp.ClientSession() 配合 async with
来源：http://hz.cheryme.top/gtasfdnhry.html

[U28] Py：类型别名
来源：http://hz.aibaodan.cn/gtrptlceet.html

UserId = int
来源：http://hz.redwolf501.top/gthljclemh.html

[U29] Py：属性校验
来源：http://hz.chenlongwang.top/gtlsbiezjo.html

@property 与 @x.setter 配合
来源：http://hz.smart0.xyz/gtmlwsbluh.html

[U30] Py：数据类
来源：http://hz.svipenyu.cn/gtnaypsugk.html

@dataclass(slots=True)
来源：http://hz.guowangkeji.top/gtztwvftwb.html

[U31] Py：单测
来源：http://hz.chenzaomai.com/gtgqvbpnxc.html

python -m pytest -q
来源：http://hz.andypj.xyz/gtnfohmoyy.html

[U32] Py：代码格式化
来源：http://hz.yueranfly.top/gtjygqhpvh.html

ruff format . && ruff check --fix .
来源：http://hz.chenlongwang.top/gtzwgplghq.html

[U33] Py：打包发布
来源：http://hz.guowangkeji.top/gtfuflwtji.html

python -m build  （依赖 pyproject.toml）
来源：http://hz.vqdsnc.cn/gtpsxyqzrb.html

[U34] Py：判断编码
来源：http://hz.guowangkeji.top/gtohpveair.html

chardet.detect(raw)
来源：http://hz.gzhubu.top/gtfzekxviw.html

[U35] Py：发送邮件
来源：http://hz.chenlongwang.top/gtjvlchsbt.html

smtplib.SMTP_SSL(...).send_message(msg)
来源：http://hz.ywan-chungtsiang.top/gtzkjnpwgh.html

[U36] Py：定时任务
来源：http://hz.yj20258.top/gtnpyeruvg.html

schedule.every(10).minutes.do(job)
来源：http://hz.guannengcc.top/gtwbvfbufz.html

[U37] Py：读写 Excel
来源：http://hz.jinghuilouyu.cn/gtdmkxaukm.html

pandas.read_excel / DataFrame.to_excel
来源：http://hz.ivvv.top/gtsssswmyv.html

[U38] Py：获取脚本所在目录
来源：http://hz.sxryk.cn/gtjdhjfcfa.html

Path(__file__).resolve().parent
来源：http://hz.shanyushiyangtech.top/gtbzcwuukw.html

[U39] Py：判断是否在交互环境
来源：http://hz.zdqjudy.top/gtsasgtwsr.html

sys.stdout.isatty()
来源：http://hz.hnxiangtu.top/gtipfleoum.html

[U40] Py：打印到标准错误
来源：http://hz.ydjk.org.cn/gtdcxbaxqv.html

print("err", file=sys.stderr)
来源：http://hz.tanke756.top/gttvggdfio.html

[U41] PHP：初始化 Composer 项目
来源：http://hz.ybcxt.top/gtscifnxjd.html

composer init;  composer require guzzlehttp/guzzle
来源：http://hz.smart0.xyz/gtbcxgmcry.html

[U42] PHP：PSR-4 自动加载
来源：http://hz.meibo888.top/gtpuuriohk.html

"autoload": { "psr-4": { "App\\": "src/" } }
来源：http://hz.gotoacloud.top/gtyrspivig.html

[U43] PHP：声明命名空间
来源：http://hz.shanyushiyangtech.top/gtrebsgwjz.html

namespace App\Http;
来源：http://hz.yuxming.cn/gtrvbpizwl.html

[U44] PHP：开启严格类型
来源：http://hz.vqdsnc.cn/gtjmpnupkb.html

declare(strict_types=1);
来源：http://hz.quarkkingdee.top/gtmnxzxibp.html

[U45] PHP：类型声明与返回类型
来源：http://hz.shzxlz.cn/gtwkwemmme.html

function add(int $a, int $b): int { return $a + $b; }
来源：http://hz.gotoacloud.top/gtmyiqykpd.html

[U46] PHP：可空类型
来源：http://hz.chenjidiqi.icu/gtnbfqhjko.html

?string $name = null
来源：http://hz.redwolf501.top/gtktbupncv.html


<!-- 参考信息 -->