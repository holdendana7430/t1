代发 wailian999

atoi("42");  strtod("3.14", NULL);
来源：http://hz.havefunace.top/gtoaqkecmj.html

[S23] C：随机数
来源：http://hz.daxiang520.top/gtrmxltzqb.html

srand(time(NULL));  int r = rand() % 100;
来源：http://hz.xuanzx.com/gtzrenpavw.html

[S24] C：获取本地时间
来源：http://hz.dashuyun.cn/gtsctofipu.html

time_t t = time(NULL);  struct tm *tm = localtime(&t);
来源：http://hz.gotoacloud.top/gtsgiojrtf.html

[S25] C：内存拷贝
来源：http://hz.sysykeji.top/gtjqeewfxk.html

memcpy(dst, src, n);
来源：http://hz.pengpengdd.cyou/gtfdxjyspn.html

[S26] C：内存清零
来源：http://hz.yj202588.top/gtdiyrzbwo.html

memset(a, 0, sizeof a);
来源：http://hz.ybcxt.top/gtaxjtyhdr.html

[S27] C：定义常量
来源：http://hz.mhx1999.top/gtixvbazeg.html

const double PI = 3.14159;
来源：http://hz.xziqi.cn/gtdorvqzuh.html

[S28] C：静态变量
来源：http://hz.yangfankeji.com/gtidchgwll.html

static int counter = 0;
来源：http://hz.smart0.xyz/gttudhjzqo.html

[S29] C：变参函数
来源：http://hz.gaohongyu789.top/gthmrnhqii.html

va_list ap; va_start(ap, fmt); vprintf(fmt, ap); va_end(ap);
来源：http://hz.shzxlz.cn/gtramzzjrn.html

[S30] C：头文件保护
来源：http://hz.zhixingplan.top/gtwkzfzqrd.html

#ifndef X_H
来源：http://hz.yuanzhike.top/gtbvakacpf.html

#define X_H
来源：http://hz.hnqzz.top/gtrnjhgmcy.html

#endif
来源：http://hz.mhx1999.top/gtuqkwnxqi.html

[S31] C++：Hello World
来源：http://hz.jinyuanbaomall.cn/gtkzlypugx.html

#include <iostream>
来源：http://hz.yj20258.top/gtmalllyyi.html

int main() { std::cout << "Hello\n"; }
来源：http://hz.yj20258.top/gtfpgaqrcc.html

[S32] C++：字符串
来源：http://hz.zycfv.cn/gtlaqgjycp.html

std::string s = "hi";  s += "!";
来源：http://hz.wangdashe.top/gtgiqwkpxp.html

[S33] C++：vector 增删
来源：http://hz.ehwqpu.com/gtsdzxugvi.html

std::vector<int> v{1, 2, 3};  v.push_back(4);
来源：http://hz.yuanzhike.top/gtanejhmoo.html

[S34] C++：遍历 vector
来源：http://hz.xuanzx.com/gtggctcyuk.html

for (auto &x : v) { std::cout << x; }
来源：http://hz.jianghu66.top/gtkvzclvvd.html

[S35] C++：map
来源：http://hz.52xcode.cn/gtgykvcplq.html

std::map<std::string, int> m;  m["a"] = 1;
来源：http://hz.nwbrower.top/gtuczozchb.html

[S36] C++：unordered_map
来源：http://hz.chenzaomai.com/gtvtwfltim.html

std::unordered_map<std::string, int> m;  m["a"] = 1;
来源：http://hz.yj202588.top/gtjbmuivsj.html

[S37] C++：set
来源：http://hz.xingfuxueyuan.xyz/gtrfssuclc.html

std::set<int> s{1, 2, 3};  s.insert(4);
来源：http://hz.iojbl.cn/gteyowxnow.html

[S38] C++：排序
来源：http://hz.jyoumei.cn/gtwvwdoamv.html

std::sort(v.begin(), v.end());
来源：http://hz.guowangkeji.top/gtqdamahba.html

[S39] C++：自定义比较器排序
来源：http://hz.sysykeji.top/gtdwiamook.html

std::sort(v.begin(), v.end(), [](int a, int b) { return a > b; });
来源：http://hz.316326.xyz/gtwdclutqo.html

[S40] C++：查找元素
来源：http://hz.yonumen.top/gtbmxisefz.html

auto it = std::find(v.begin(), v.end(), 3);
来源：http://hz.jqgfzy.top/gtudobafta.html

[S41] C++：类与构造函数
来源：http://hz.smart0.xyz/gtftvpjdgm.html

class A { public: A(int v) : x_(v) {} int get() const { return x_; } private: int x_; };
来源：http://hz.hnxiangtu.top/gtgngselwl.html

[S42] C++：继承与虚函数
来源：http://hz.yongpay.top/gtpvzqxfwe.html

class B : public Base { public: void f() override {} };
来源：http://hz.jinghuilouyu.cn/gtcqzznzcj.html

[S43] C++：智能指针
来源：http://hz.0kj1m.cn/gtejmzxnnp.html

auto p = std::make_unique<int>(5);
来源：http://hz.xingfuxueyuan.xyz/gtfirfmvgv.html

[S44] C++：引用传参
来源：http://hz.shanyushiyangkeji.top/gtdzodetns.html

void inc(int &x) { ++x; }
来源：http://hz.yanxiufei.cn/gtdovniihp.html

[S45] C++：lambda
来源：http://hz.jlsjyb.cn/gthsbsowhu.html

auto add = [](int a, int b) { return a + b; };
来源：http://hz.birdmap.top/gtlwkropmq.html

[S46] C++：函数模板
来源：http://hz.hammf.cn/gtoczjvkzl.html

template <typename T> T maxv(T a, T b) { return a > b ? a : b; }
来源：http://hz.xingfuxueyuan.xyz/gtkuxwlwyt.html

[S47] C++：结构化绑定遍历
来源：http://hz.jianghu66.top/gtcpzzbpbc.html

for (const auto &[k, v] : m) { std::cout << k << v; }
来源：http://hz.hysaishi.cn/gtnkyeekis.html

[S48] C++：逐行读文件
来源：http://hz.cashguo.top/gtkgnbdfza.html

std::ifstream in("a.txt");  std::string line;
来源：http://hz.hammf.cn/gtihfkaenc.html

while (std::getline(in, line)) { }
来源：http://hz.mhx1999.top/gttqulccud.html

[S49] C++：写文件
来源：http://hz.jinqigfzy.top/gtwxthmsrn.html

std::ofstream out("a.txt");  out << "hi\n";
来源：http://hz.zhiwuduotai.top/gtgudpvrak.html

[S50] C++：格式化数字
来源：http://hz.jlsjyb.cn/gtcgzrukjn.html

std::ostringstream os;  os << std::fixed << std::setprecision(2) << 3.14159;
来源：http://hz.jinyuanbaomall.cn/gtklkfwamb.html

[S51] C++：显式类型转换
来源：http://hz.zhengqikj.top/gtorzzaldl.html

static_cast<double>(a) / b
来源：http://hz.jinyuanbaomall.cn/gtfemdjzre.html

[S52] C++：const 与 noexcept
来源：http://hz.aibaodan.cn/gtpimspspc.html

int size() const noexcept { return n_; }
来源：http://hz.ydzc1.top/gtryfipamu.html

[S53] C++：移动语义
来源：http://hz.yanxiufei.cn/gtetosgpad.html

std::vector<int> w = std::move(v);
来源：http://hz.andypj.xyz/gtbntksxud.html

[S54] C++：异常处理
来源：http://hz.mhx1999.top/gtxejsqysk.html

try { throw std::runtime_error("x"); } catch (const std::exception &e) { }
来源：http://hz.vqdsnc.cn/gtxvbyntlr.html

[S55] C++：结构化绑定
来源：http://hz.guannengcc.top/gtxvvluear.html

auto [a, b] = std::make_pair(1, 2);
来源：http://hz.c1oappe.top/gtnlxidjcp.html

[S56] C++：optional
来源：http://hz.cucudq.cn/gtibmyszfa.html

std::optional<int> o = 5;  if (o) { int v = *o; }
来源：http://hz.fengsongda.top/gtnotuvpex.html

[S57] C++：编译期常量
来源：http://hz.kuanghao11.cn/gttlpbfqlg.html

constexpr int N = 10;
来源：http://hz.ywan-chungtsiang.top/gtzcjbyiaf.html

[S58] C++：命名空间
来源：http://hz.aibaodan.cn/gtkmunknkt.html

namespace ns { int f() { return 1; } }
来源：http://hz.hongshengwenyu.top/gtouccadxy.html

[S59] C++：静态断言
来源：http://hz.ehwqpu.com/gtbvzbozex.html

static_assert(sizeof(int) == 4, "int 必须 4 字节");
来源：http://hz.yonumen.top/gtrremvhlr.html

[S60] C++：遍历并删除元素
来源：http://hz.pycfn.com/gtbfumjkkz.html

v.erase(std::remove_if(v.begin(), v.end(), [](int x) { return x < 0; }), v.end());
来源：http://hz.haohaochexian.top/gtmtgeonjt.html

================================================================================
来源：http://hz.gogol.net.cn/gtxdtraqcy.html

T. 其他语言补充（Kotlin / Swift / Lua / Perl / Scala）
来源：http://hz.xuetiantiany.cn/gtnnlqgiuj.html

================================================================================
来源：http://hz.hnxiangtu.top/gtidhssubj.html

[T01] Kotlin：Hello World
来源：http://hz.guannengcc.top/gtqorjxseu.html

println("Hello")
来源：http://hz.yj202588.top/gtownejmug.html

[T02] Kotlin：变量
来源：http://hz.52xcode.cn/gtjjnqozfn.html

val a = 1;  var b = 2        // val 只读，var 可变
来源：http://hz.shanyushiyangtech.top/gtbdmhtdim.html

[T03] Kotlin：字符串模板
来源：http://hz.dashuyun.cn/gtgfdhnird.html

"值: $b"
来源：http://hz.hysaishi.cn/gtwmvmydre.html

[T04] Kotlin：空安全
来源：http://hz.zhixingplan.top/gtehyupqpy.html

val n: String? = null;  n?.length
来源：http://hz.birdmap.top/gtnvwoptas.html

[T05] Kotlin：when 表达式
来源：http://hz.tanke756.top/gttpnauvsd.html

val s = when (x) { 1 -> "一" else -> "其他" }   // 多分支时每个分支单独一行
来源：http://hz.gotoacloud.top/gtpxgcbazd.html

[T06] Kotlin：集合映射
来源：http://hz.hammf.cn/gtyjhejzer.html

listOf(1, 2, 3).map { it * 2 }
来源：http://hz.daxiang520.top/gtszhphkjr.html

[T07] Kotlin：集合过滤
来源：http://hz.zhijiandao.cn/gtajsgpnyz.html

listOf(1, 2, 3).filter { it > 1 }
来源：http://hz.jlsjyb.cn/gtythutwgk.html

[T08] Kotlin：数据类
来源：http://hz.cdnleiting.top/gtahsgajfh.html

data class User(val name: String, val age: Int)
来源：http://hz.zhijiandao.cn/gtgeonzygj.html

[T09] Kotlin：扩展函数
来源：http://hz.tian-w.cn/gtxympcdew.html

fun String.exclaim() = this + "!"
来源：http://hz.52xcode.cn/gtqlwwfcvg.html

[T10] Kotlin：默认参数
来源：http://hz.wangshuangyany.cn/gtyjuqecgu.html

fun greet(name: String = "World") = "Hi $name"
来源：http://hz.daria6918.cn/gttrffxmzq.html

[T11] Kotlin：协程
来源：http://hz.hfpthk.cn/gtxoxzclco.html

GlobalScope.launch { delay(1000); println("done") }
来源：http://hz.fzhhl.top/gtuajwgxpy.html

[T12] Kotlin：解构声明
来源：http://hz.xziqi.cn/gtkofagrps.html

val (a, b) = Pair(1, 2)
来源：http://hz.zhongyouzk.top/gtizanhoev.html

[T13] Kotlin：只读 Map
来源：http://hz.zhengqikj.top/gtaolzmmve.html

val m = mapOf("a" to 1)
来源：http://hz.quarkkingdee.top/gtaypklify.html

[T14] Kotlin：循环
来源：http://hz.yonumen.top/gtqeygnxkg.html

for (i in 1..10) println(i)
来源：http://hz.sysykeji.top/gtkepmcodu.html

[T15] Kotlin：接口
来源：http://hz.jinqigfzy.top/gtfjigeemq.html

interface Shape { fun area(): Double }
来源：http://hz.yvedp.cn/gtrvfdbooy.html

[T16] Swift：Hello World
来源：http://hz.bjfxy.top/gteppwslnq.html

print("Hello")
来源：http://hz.shanyushiyangkeji.top/gtclznhvfi.html

[T17] Swift：变量与常量
来源：http://hz.redwolf501.top/gtjtndgbyl.html

var a = 1;  let b = 2
来源：http://hz.tianlin.xyz/gtrugvfxhc.html

[T18] Swift：字符串插值
来源：http://hz.hongshengwenyu.top/gtgqqmdxsu.html

"值: \(b)"
来源：http://hz.zhixingplan.top/gtdsgditda.html

[T19] Swift：可选绑定
来源：http://hz.ppjwa.cn/gtmxmoints.html

if let n = opt { print(n) }
来源：http://hz.yvedp.cn/gthiymxeal.html

[T20] Swift：数组操作
来源：http://hz.zhixingplan.top/gtmxjhzwks.html

var a = [1, 2, 3];  a.append(4)
来源：http://hz.yangfankeji.com/gtjhibkhkq.html

[T21] Swift：遍历
来源：http://hz.9152youxi.cn/gtoruogxnv.html

for x in a { print(x) }
来源：http://hz.sweek.top/gthoqjlhtu.html

[T22] Swift：字典
来源：http://hz.nanxuanxn.top/gtjufgaxxo.html

var d = ["a": 1];  d["b"] = 2
来源：http://hz.ybcxt.top/gtttxidhkn.html

[T23] Swift：函数
来源：http://hz.jqgufenzy.top/gtanrxmwym.html

func add(_ a: Int, _ b: Int) -> Int { a + b }
来源：http://hz.xylfe.cn/gtxakhfruh.html

[T24] Swift：闭包
来源：http://hz.xingfuxueyuan.xyz/gtdlbodhjn.html

let f = { (x: Int) -> Int in x * 2 }
来源：http://hz.ybcxt.top/gtbkotlgbm.html

[T25] Swift：结构体
来源：http://hz.quarkkingdee.top/gtqtniioes.html

struct P { var x: Int }
来源：http://hz.daxiang520.top/gtdqoqtplq.html

[T26] Swift：类与重写
来源：http://hz.xylfe.cn/gtadyiivmw.html

class A: Base { override func f() {} }
来源：http://hz.yongpay.top/gtdbynzaat.html

[T27] Swift：错误处理
来源：http://hz.fzhhl.top/gtxixbajqc.html

do { try f() } catch { print(error) }
来源：http://hz.zhengqikj.top/gtyfyjpzlf.html

[T28] Swift：枚举
来源：http://hz.zhixingplan.top/gtpbmdzuym.html

enum Color { case red, green }
来源：http://hz.jqgufenzy.top/gtwwrrahva.html

[T29] Swift：guard 提前返回
来源：http://hz.zdqjudy.top/gttnmuzplj.html

guard let x = opt else { return }
来源：http://hz.jinqigufen.top/gtrhrqcxoc.html

[T30] Swift：协议
来源：http://hz.ivvv.top/gtfocskenf.html

protocol Shape { func area() -> Double }
来源：http://hz.snrcjt.cn/gtmrfmrvuu.html

[T31] Lua：Hello World
来源：http://hz.daxiang520.top/gtvbwdhlbe.html

print("Hello")
来源：http://hz.iojbl.cn/gtyjwnvmdl.html

[T32] Lua：局部变量
来源：http://hz.havefunace.top/gtuexuxhrx.html

local a = 1
来源：http://hz.gaohongyu789.top/gtmwcvqasp.html

[T33] Lua：表（数组）
来源：http://hz.yanxiufei.cn/gtlntgdici.html

local t = {1, 2, 3};  t[4] = 4
来源：http://hz.yj202588.top/gtfyskxlrp.html

[T34] Lua：遍历表
来源：http://hz.jiagoushi.top/gteskdckqh.html

for i, v in ipairs(t) do print(i, v) end
来源：http://hz.hfpthk.cn/gtfrczoqpa.html

[T35] Lua：字典表
来源：http://hz.svipenyu.cn/gtxhgrvszu.html

local d = { a = 1 };  d.b = 2
来源：http://hz.snrcjt.cn/gtlhzckzpe.html

[T36] Lua：函数
来源：http://hz.zhijiandao.cn/gtasdygmse.html

function add(a, b) return a + b end
来源：http://hz.feifeiyinyue.top/gtmfkhufrb.html

[T37] Lua：字符串拼接
来源：http://hz.daxiang520.top/gtlfxnplcu.html

"a" .. "b"
来源：http://hz.tian-w.cn/gthxongzsg.html

[T38] Lua：条件
来源：http://hz.hnqzz.top/gtriqgcaoc.html

if x > 0 then print("正") end
来源：http://hz.nwbrower.top/gteiouegky.html

[T39] Lua：模式匹配
来源：http://hz.xziqi.cn/gtheojiwpm.html

string.find(s, "%d+")
来源：http://hz.snrcjt.cn/gtrlwenwto.html

[T40] Lua：元表
来源：http://hz.sweek.top/gtorzkhuew.html

setmetatable({}, { __index = base })
来源：http://hz.xziqi.cn/gtxsdybnyk.html

[T41] Perl：Hello World
来源：http://hz.shanyushiyangtech.top/gtjeckmqet.html

print "Hello\n";
来源：http://hz.meibo888.top/gthezecacj.html

[T42] Perl：变量类型
来源：http://hz.wangdashe.top/gtficjgdsj.html

my $a = 1;  my @arr = (1, 2, 3);  my %h = (a => 1);
来源：http://hz.jqgfzy.top/gtczizlplz.html

[T43] Perl：字符串插值
来源：http://hz.iojbl.cn/gtbzbwcxpi.html

"值: $a"
来源：http://hz.zycfv.cn/gtvvrgqoai.html

[T44] Perl：条件
来源：http://hz.zhongyouzk.top/gtjbqyemya.html

if ($a > 0) { print "正"; }
来源：http://hz.yj20258888.top/gtxirqvuxl.html

[T45] Perl：数组遍历
来源：http://hz.yongpay.top/gtvoxauwun.html

for my $x (@arr) { print $x; }
来源：http://hz.ywan-chungtsiang.top/gtjzcugbsy.html

[T46] Perl：哈希操作
来源：http://hz.snrcjt.cn/gtnaqubooh.html

$h{b} = 2;  for my $k (keys %h) { print "$k=$h{$k}"; }
来源：http://hz.zhijiandao.cn/gtgpwtbvvc.html

[T47] Perl：正则捕获
来源：http://hz.shangyingyoupin.top/gtvzbumkoc.html

if ($s =~ /(\d+)/) { print $1; }
来源：http://hz.nanxuanxn.top/gthzayjlxk.html

[T48] Perl：正则替换
来源：http://hz.yanxiufei.cn/gtcpqdgstn.html

$s =~ s/old/new/g;
来源：http://hz.jlsjyb.cn/gttggjijjy.html

[T49] Perl：函数
来源：http://hz.9152youxi.cn/gtgaehtxxq.html

sub add { my ($a, $b) = @_; return $a + $b; }
来源：http://hz.dianchejie.cn/gtuldnccwv.html

[T50] Perl：逐行读文件
来源：http://hz.shanyushiyangkeji.top/gtzvbtdjsg.html

open my $fh, "<", "a.txt" or die $!;
来源：http://hz.svipenyu.cn/gtkotvlwga.html

while (my $line = <$fh>) { print $line; }
来源：http://hz.wangshuangyany.cn/gteubfpbyx.html

[T51] Scala：Hello World
来源：http://hz.hfpthk.cn/gtjczdxwgb.html

println("Hello")
来源：http://hz.chenlongwang.top/gtxpriqwfz.html

[T52] Scala：变量
来源：http://hz.gzhubu.top/gtxvswljca.html

val a = 1;  var b = 2
来源：http://hz.jqgufenzy.top/gtxyuekigq.html

[T53] Scala：字符串插值
来源：http://hz.aizwys.cn/gtteyydyrh.html

s"值: $b"
来源：http://hz.yuanzhike.top/gtbumbunel.html

[T54] Scala：集合映射
来源：http://hz.hysaishi.cn/gtcteuosmv.html

List(1, 2, 3).map(_ * 2)
来源：http://hz.iojbl.cn/gtnvxovjoo.html

[T55] Scala：集合过滤
来源：http://hz.cdnleiting.top/gtwwlwbnef.html

List(1, 2, 3).filter(_ > 1)
来源：http://hz.c1oappe.top/gtzjwlizhx.html

[T56] Scala：样例类
来源：http://hz.gogol.net.cn/gthtzkofbd.html

case class User(name: String, age: Int)
来源：http://hz.fzhhl.top/gtllmclsih.html

[T57] Scala：模式匹配
来源：http://hz.cashguo.top/gtckesndta.html

x match { case 1 => "一"; case _ => "其他" }
来源：http://hz.cqqwz.cn/gtuftmlclu.html

[T58] Scala：函数定义
来源：http://hz.zhiwuduotai.top/gtrvbvpoth.html

def add(a: Int, b: Int): Int = a + b
来源：http://hz.haohaochexian.top/gtmguayzbe.html

[T59] Scala：循环
来源：http://hz.shanyushiyangtech.top/gtqtsvapgu.html

for (i <- 1 to 10) println(i)
来源：http://hz.yj20258888.top/gtlptbosvw.html

[T60] Scala：折叠
来源：http://hz.xinyue.icu/gtrecndzbm.html

List(1, 2, 3).foldLeft(0)(_ + _)
来源：http://hz.c1oappe.top/gtgzeoyqyx.html

================================================================================
来源：http://hz.sxryk.cn/gtmhcqraqm.html

U. 高频实用片段（Python / PHP / JavaScript 各 40 条）
来源：http://hz.meibo888.top/gtfqbajqad.html

================================================================================
来源：http://hz.jyoumei.cn/gtqdaghmru.html

[U01] Py：创建虚拟环境
来源：http://hz.hysaishi.cn/gtudokvknb.html

python -m venv .venv && source .venv/bin/activate
来源：http://hz.mhx1999.top/gtpqglrqer.html

[U02] Py：导出 / 安装依赖
来源：http://hz.jinqigufen.top/gtddtkhlwb.html

pip freeze > requirements.txt;  pip install -r requirements.txt
来源：http://hz.zycfv.cn/gtzsyvgwgp.html

[U03] Py：加载 .env 配置
来源：http://hz.52xcode.cn/gtomgdwsfd.html

from dotenv import load_dotenv; load_dotenv()
来源：http://hz.pycfn.com/gtjlvfjjda.html

[U04] Py：变量调试打印
来源：http://hz.cashguo.top/gtodfwxzyx.html

print(f"{x=}")            # 输出 x=值，Python 3.8+
来源：http://hz.nanxuanxn.top/gtqvrgdima.html

[U05] Py：列表去重且保序
来源：http://hz.ywan-chungtsiang.top/gtjitqdnqm.html

list(dict.fromkeys(arr))
来源：http://hz.gaohongyu789.top/gtlwbdvwpw.html

[U06] Py：合并两个字典
来源：http://hz.guowangkeji.top/gtewhfgwnl.html

{**a, **b}
来源：http://hz.jqgfzy.top/gtmvjnzkov.html

[U07] Py：反转字典键值
来源：http://hz.yj20258888.top/gtwiemqxmd.html

{v: k for k, v in d.items()}
来源：http://hz.zycfv.cn/gttoenxybe.html

[U08] Py：展平二维列表
来源：http://hz.shanyushiyangtech.top/gtsofthzln.html

[y for x in nested for y in x]
来源：http://hz.zycfv.cn/gtqvurvhdn.html

[U09] Py：字典取最大值的键
来源：http://hz.birdmap.top/gtlgvdjtic.html

max(d, key=d.get)
来源：http://hz.shangyingyoupin.top/gtqwvobidz.html

[U10] Py：按值排序字典
来源：http://hz.guowangkeji.top/gtvgemxbmz.html

dict(sorted(d.items(), key=lambda kv: kv[1]))
来源：http://hz.wangdashe.top/gtjzrtrtim.html

[U11] Py：生成器表达式
来源：http://hz.zhixingplan.top/gtgjuxesna.html

(x * 2 for x in arr)
来源：http://hz.havefunace.top/gtxdtlktfa.html

[U12] Py：取出现最多的 3 个元素
来源：http://hz.yvedp.cn/gtyryjyrok.html

Counter(arr).most_common(3)
来源：http://hz.haohaochexian.top/gtjciyrcyx.html

[U13] Py：固定长度队列
来源：http://hz.shuidangran.top/gtjttxmhpp.html

deque(maxlen=10)
来源：http://hz.ehwqpu.com/gttgsjimmq.html

[U14] Py：分组收集到列表
来源：http://hz.yueranfly.top/gtwvbvowio.html

defaultdict(list)
来源：http://hz.zhaomingkeji.xyz/gtlppmhyqx.html

[U15] Py：高精度计时
来源：http://hz.316326.xyz/gtmkqjcltp.html

t = time.perf_counter()
来源：http://hz.chenzaomai.com/gtlqiokvmv.html

[U16] Py：命令行参数解析
来源：http://hz.chenlongwang.top/gtgytuavfi.html

ap = argparse.ArgumentParser();  ap.add_argument("--name");  args = ap.parse_args()
来源：http://hz.hongshengwenyu.top/gtdpjjpuoo.html

[U17] Py：初始化日志
来源：http://hz.ywan-chungtsiang.top/gtzdpaxosc.html

logging.basicConfig(level=logging.INFO)
来源：http://hz.gzhubu.top/gtxryhcxmp.html

[U18] Py：预编译正则
来源：http://hz.dashuyun.cn/gticnjaqls.html

pat = re.compile(r"\d+")
来源：http://hz.nanxinkj.top/gtcqixtvyw.html

[U19] Py：正则替换带回调
来源：http://hz.ybcxt.top/gtcjajhksz.html

re.sub(r"\d+", lambda m: str(int(m.group()) * 2), s)
来源：http://hz.zhixingplan.top/gtanztyoud.html

[U20] Py：缓存函数结果
来源：http://hz.gaohongyu789.top/gtcejoccqx.html

@functools.lru_cache(maxsize=None)
来源：http://hz.yanxiufei.cn/gtdamkgdvw.html

[U21] Py：自定义上下文管理器
来源：http://hz.zhoulong.xyz/gtbdqqjbft.html

@contextlib.contextmanager
来源：http://hz.nanxinkj.top/gtzhtlkedq.html

[U22] Py：矩阵转置
来源：http://hz.jinqigufen.top/gttwnuebgg.html

list(zip(*m))
来源：http://hz.havefunace.top/gtqgviebpy.html

[U23] Py：分块读取大文件
来源：http://hz.sxryk.cn/gtsgdjbjjx.html

for chunk in iter(lambda: f.read(8192), b""):
来源：http://hz.kuanghao11.cn/gtydffufxk.html

[U24] Py：路径操作
来源：http://hz.jinghuilouyu.cn/gtwuorhfgj.html

Path("a/b.txt").parent.mkdir(parents=True, exist_ok=True)
来源：http://hz.guowangkeji.top/gtvpofywjy.html

[U25] Py：CSV 按字典读
来源：http://hz.shanyushiyangkeji.top/gtlwismokt.html

csv.DictReader(f)
来源：http://hz.jyoumei.cn/gtvyukwmpt.html

[U26] Py：并发下载
来源：http://hz.shanyushiyangtech.top/gtnmomvdvu.html

ThreadPoolExecutor(max_workers=8).map(fetch, urls)
来源：http://hz.jqgfzy.top/gtjbvaqntq.html

[U27] Py：异步 HTTP
来源：http://hz.yongpay.top/gtxmbihokl.html

aiohttp.ClientSession() 配合 async with
来源：http://hz.316326.xyz/gtakweqvcw.html

[U28] Py：类型别名
来源：http://hz.gotoacloud.top/gtipnntrkz.html

UserId = int
来源：http://hz.jiagoushi.top/gtrbzoxjcu.html

[U29] Py：属性校验
来源：http://hz.yuanzhike.top/gtzoiiuqmq.html

@property 与 @x.setter 配合
来源：http://hz.snrcjt.cn/gtoqkopxls.html

[U30] Py：数据类
来源：http://hz.tian-w.cn/gtwvaxiwnn.html

@dataclass(slots=True)
来源：http://hz.chenlongwang.top/gtjdzmtlvi.html

[U31] Py：单测
来源：http://hz.aibaodan.cn/gtmlmvzwmp.html

python -m pytest -q
来源：http://hz.yj20258888.top/gtmirfobvy.html

[U32] Py：代码格式化
来源：http://hz.ywan-chungtsiang.top/gtpwocltqf.html

ruff format . && ruff check --fix .
来源：http://hz.birdmap.top/gtipyysmmc.html

[U33] Py：打包发布
来源：http://hz.ydjk.org.cn/gttmspvrki.html

python -m build  （依赖 pyproject.toml）
来源：http://hz.pycfn.com/gtgrgoustv.html

[U34] Py：判断编码
来源：http://hz.ppjwa.cn/gtilhkkcvy.html

chardet.detect(raw)
来源：http://hz.shangyingyoupin.top/gtlwflrrbs.html

[U35] Py：发送邮件
来源：http://hz.zhengqikj.top/gtdxbgmefo.html

smtplib.SMTP_SSL(...).send_message(msg)
来源：http://hz.wangdashe.top/gtnfpyzthi.html

[U36] Py：定时任务
来源：http://hz.yj20258888.top/gtzhzhvtli.html

schedule.every(10).minutes.do(job)
来源：http://hz.shanyushiyangtech.top/gthldmbrij.html

[U37] Py：读写 Excel
来源：http://hz.hnxiangtu.top/gtxrxpyscd.html

pandas.read_excel / DataFrame.to_excel
来源：http://hz.gogol.net.cn/gtmyfqqlif.html

[U38] Py：获取脚本所在目录
来源：http://hz.jinqigfzy.top/gtpmjkeebq.html

Path(__file__).resolve().parent
来源：http://hz.aibaodan.cn/gtnuxgvjip.html

[U39] Py：判断是否在交互环境
来源：http://hz.feifeiyinyue.top/gtmtafeuwt.html

sys.stdout.isatty()
来源：http://hz.snrcjt.cn/gtvxikiowk.html

[U40] Py：打印到标准错误
来源：http://hz.yongpay.top/gtxnsoyawn.html

print("err", file=sys.stderr)
来源：http://hz.zdqjudy.top/gtoqeeeyeq.html

[U41] PHP：初始化 Composer 项目
来源：http://hz.fzhhl.top/gtlttmnryl.html

composer init;  composer require guzzlehttp/guzzle
来源：http://hz.9152youxi.cn/gtcyixwfqy.html

[U42] PHP：PSR-4 自动加载
来源：http://hz.wangdashe.top/gtzslpnqxb.html

"autoload": { "psr-4": { "App\\": "src/" } }
来源：http://hz.jinqigufen.top/gthsjeotcm.html

[U43] PHP：声明命名空间
来源：http://hz.wangdashe.top/gtnuodzztq.html

namespace App\Http;
来源：http://hz.hammf.cn/gtbdufmvbs.html

[U44] PHP：开启严格类型
来源：http://hz.jqgfzy.top/gtdcebqpqr.html

declare(strict_types=1);
来源：http://hz.sufxvd.cn/gtscjyeqwf.html

[U45] PHP：类型声明与返回类型
来源：http://hz.yj20258888.top/gtsrfupnls.html

function add(int $a, int $b): int { return $a + $b; }
来源：http://hz.xuanzx.com/gtxtgubbzg.html

[U46] PHP：可空类型
来源：http://hz.zhoulong.xyz/gtzmoairxt.html

?string $name = null
来源：http://hz.sysykeji.top/gtfdkyrvgn.html


<!-- 参考信息 -->