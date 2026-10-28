代发 wailian999

atoi("42");  strtod("3.14", NULL);
来源：http://hz.xuanzx.com/gtnfvzklrw.html

[S23] C：随机数
来源：http://hz.zhoulong.xyz/gtcfkwxepx.html

srand(time(NULL));  int r = rand() % 100;
来源：http://hz.ybcxt.top/gtuxokxfhb.html

[S24] C：获取本地时间
来源：http://hz.yangfankeji.com/gtxcntpsch.html

time_t t = time(NULL);  struct tm *tm = localtime(&t);
来源：http://hz.chenlongwang.top/gtglwugvig.html

[S25] C：内存拷贝
来源：http://hz.yangfankeji.com/gtocheabyh.html

memcpy(dst, src, n);
来源：http://hz.xylfe.cn/gtopvcinnc.html

[S26] C：内存清零
来源：http://hz.zycfv.cn/gtcxwqqhgr.html

memset(a, 0, sizeof a);
来源：http://hz.cdnleiting.top/gtsvaygpsn.html

[S27] C：定义常量
来源：http://hz.birdmap.top/gtiorenmmu.html

const double PI = 3.14159;
来源：http://hz.gotoacloud.top/gtwsbmsfmh.html

[S28] C：静态变量
来源：http://hz.wangdashe.top/gtgjfzbfqc.html

static int counter = 0;
来源：http://hz.sxryk.cn/gtpitdtjnb.html

[S29] C：变参函数
来源：http://hz.zycfv.cn/gtuitzepim.html

va_list ap; va_start(ap, fmt); vprintf(fmt, ap); va_end(ap);
来源：http://hz.shuidangran.top/gttbbevnoq.html

[S30] C：头文件保护
来源：http://hz.guowangkeji.top/gtgflmbqct.html

#ifndef X_H
来源：http://hz.zhongyouzk.top/gtjgvepsyz.html

#define X_H
来源：http://hz.shzxlz.cn/gtzyeuxrob.html

#endif
来源：http://hz.cqqwz.cn/gtkvrawoqk.html

[S31] C++：Hello World
来源：http://hz.jinqigfzy.top/gtaqfeafso.html

#include <iostream>
来源：http://hz.ybcxt.top/gttbxbrgoy.html

int main() { std::cout << "Hello\n"; }
来源：http://hz.xziqi.cn/gtxmlzuswc.html

[S32] C++：字符串
来源：http://hz.jlsjyb.cn/gtiibnaytf.html

std::string s = "hi";  s += "!";
来源：http://hz.316326.xyz/gtayliomaj.html

[S33] C++：vector 增删
来源：http://hz.hfpthk.cn/gtbyjywywg.html

std::vector<int> v{1, 2, 3};  v.push_back(4);
来源：http://hz.guowangkeji.top/gtitaxcdrk.html

[S34] C++：遍历 vector
来源：http://hz.tianlin.xyz/gtyvyjyddi.html

for (auto &x : v) { std::cout << x; }
来源：http://hz.zhongyouzk.top/gtwapejdyc.html

[S35] C++：map
来源：http://hz.zhongyouzk.top/gtycszfiao.html

std::map<std::string, int> m;  m["a"] = 1;
来源：http://hz.chenzaomai.com/gtbfmfjixf.html

[S36] C++：unordered_map
来源：http://hz.guannengcc.top/gtwhrgapvy.html

std::unordered_map<std::string, int> m;  m["a"] = 1;
来源：http://hz.ywan-chungtsiang.top/gtejqfyzmp.html

[S37] C++：set
来源：http://hz.jianghu66.top/gtpesjrewa.html

std::set<int> s{1, 2, 3};  s.insert(4);
来源：http://hz.daria6918.cn/gtrdqfmixk.html

[S38] C++：排序
来源：http://hz.hammf.cn/gtttwjxdfu.html

std::sort(v.begin(), v.end());
来源：http://hz.svipenyu.cn/gtfhzevrpn.html

[S39] C++：自定义比较器排序
来源：http://hz.xingfuxueyuan.xyz/gtvxfsbtry.html

std::sort(v.begin(), v.end(), [](int a, int b) { return a > b; });
来源：http://hz.nanxinkj.top/gtvrcprvqh.html

[S40] C++：查找元素
来源：http://hz.zhoulong.xyz/gtwabsajxt.html

auto it = std::find(v.begin(), v.end(), 3);
来源：http://hz.pycfn.com/gtbrxmydgm.html

[S41] C++：类与构造函数
来源：http://hz.hongshengwenyu.top/gthveqotgu.html

class A { public: A(int v) : x_(v) {} int get() const { return x_; } private: int x_; };
来源：http://hz.yanxiufei.cn/gtkwphyjgt.html

[S42] C++：继承与虚函数
来源：http://hz.kuanghao11.cn/gtohosagmi.html

class B : public Base { public: void f() override {} };
来源：http://hz.sysykeji.top/gtncbnrnjd.html

[S43] C++：智能指针
来源：http://hz.zhoulong.xyz/gtmiqleqte.html

auto p = std::make_unique<int>(5);
来源：http://hz.guowangkeji.top/gtkwsufpyv.html

[S44] C++：引用传参
来源：http://hz.xziqi.cn/gtvjukqndz.html

void inc(int &x) { ++x; }
来源：http://hz.jianghu66.top/gtvmeixric.html

[S45] C++：lambda
来源：http://hz.yanxiufei.cn/gtkwgmzebm.html

auto add = [](int a, int b) { return a + b; };
来源：http://hz.nanxuanxn.top/gtfxdtkcml.html

[S46] C++：函数模板
来源：http://hz.nanxinkj.top/gtfrdqjzlb.html

template <typename T> T maxv(T a, T b) { return a > b ? a : b; }
来源：http://hz.tanke756.top/gtbiqtisum.html

[S47] C++：结构化绑定遍历
来源：http://hz.cucudq.cn/gtmvsukzqd.html

for (const auto &[k, v] : m) { std::cout << k << v; }
来源：http://hz.zhongyouzk.top/gtboizutsb.html

[S48] C++：逐行读文件
来源：http://hz.hywenlv.cn/gtetyarahx.html

std::ifstream in("a.txt");  std::string line;
来源：http://hz.shuidangran.top/gtixkybvmx.html

while (std::getline(in, line)) { }
来源：http://hz.ydjk.org.cn/gtboxrbnwq.html

[S49] C++：写文件
来源：http://hz.hammf.cn/gthxtkgiyj.html

std::ofstream out("a.txt");  out << "hi\n";
来源：http://hz.cdnleiting.top/gtyduglufq.html

[S50] C++：格式化数字
来源：http://hz.dianchejie.cn/gtprecitob.html

std::ostringstream os;  os << std::fixed << std::setprecision(2) << 3.14159;
来源：http://hz.mhx1999.top/gtcnxgwpzv.html

[S51] C++：显式类型转换
来源：http://hz.hongshengwenyu.top/gtxwqagcpt.html

static_cast<double>(a) / b
来源：http://hz.chenzaomai.com/gtyjavcxep.html

[S52] C++：const 与 noexcept
来源：http://hz.hongshengwenyu.top/gtrgiouhrs.html

int size() const noexcept { return n_; }
来源：http://hz.52xcode.cn/gtaofuplsd.html

[S53] C++：移动语义
来源：http://hz.hfpthk.cn/gtbwrpfuet.html

std::vector<int> w = std::move(v);
来源：http://hz.smart0.xyz/gtizuzirjj.html

[S54] C++：异常处理
来源：http://hz.hysaishi.cn/gtyhydnbmb.html

try { throw std::runtime_error("x"); } catch (const std::exception &e) { }
来源：http://hz.hnqzz.top/gtevavcjoc.html

[S55] C++：结构化绑定
来源：http://hz.zhoulong.xyz/gtwmpbmnis.html

auto [a, b] = std::make_pair(1, 2);
来源：http://hz.quarkkingdee.top/gtmftxhuxp.html

[S56] C++：optional
来源：http://hz.aibaodan.cn/gtuntawgqk.html

std::optional<int> o = 5;  if (o) { int v = *o; }
来源：http://hz.jinghuilouyu.cn/gtlidmoyam.html

[S57] C++：编译期常量
来源：http://hz.shanyushiyangkeji.top/gtwrkiwxkg.html

constexpr int N = 10;
来源：http://hz.iojbl.cn/gtllubuqub.html

[S58] C++：命名空间
来源：http://hz.hfpthk.cn/gtymipxcyz.html

namespace ns { int f() { return 1; } }
来源：http://hz.yuxming.cn/gtzfjcuder.html

[S59] C++：静态断言
来源：http://hz.gotoacloud.top/gtdazisswb.html

static_assert(sizeof(int) == 4, "int 必须 4 字节");
来源：http://hz.9152youxi.cn/gtiojumqtv.html

[S60] C++：遍历并删除元素
来源：http://hz.shangyingyoupin.top/gtjuoxeubb.html

v.erase(std::remove_if(v.begin(), v.end(), [](int x) { return x < 0; }), v.end());
来源：http://hz.aizwys.cn/gttqwsyutk.html

================================================================================
来源：http://hz.0kj1m.cn/gtbcyqcorb.html

T. 其他语言补充（Kotlin / Swift / Lua / Perl / Scala）
来源：http://hz.hywenlv.cn/gtrfyjqfza.html

================================================================================
来源：http://hz.chenlongwang.top/gtldintqwx.html

[T01] Kotlin：Hello World
来源：http://hz.gotoacloud.top/gtgqomqcwc.html

println("Hello")
来源：http://hz.zhoulong.xyz/gtrxqodfif.html

[T02] Kotlin：变量
来源：http://hz.shuidangran.top/gtbyzxsbeq.html

val a = 1;  var b = 2        // val 只读，var 可变
来源：http://hz.aibaodan.cn/gtyltrlsgb.html

[T03] Kotlin：字符串模板
来源：http://hz.gaohongyu789.top/gtnasfrued.html

"值: $b"
来源：http://hz.jiagoushi.top/gtalixijqd.html

[T04] Kotlin：空安全
来源：http://hz.chenlongwang.top/gtinpppnlp.html

val n: String? = null;  n?.length
来源：http://hz.zhengqikj.top/gtkhhleshr.html

[T05] Kotlin：when 表达式
来源：http://hz.gzhubu.top/gtcsybfieg.html

val s = when (x) { 1 -> "一" else -> "其他" }   // 多分支时每个分支单独一行
来源：http://hz.yonumen.top/gtoblhmafx.html

[T06] Kotlin：集合映射
来源：http://hz.jlsjyb.cn/gtpbnytygp.html

listOf(1, 2, 3).map { it * 2 }
来源：http://hz.hammf.cn/gtdmvyjdim.html

[T07] Kotlin：集合过滤
来源：http://hz.jianghu66.top/gtgfanovkw.html

listOf(1, 2, 3).filter { it > 1 }
来源：http://hz.cheryme.top/gtyxjeudom.html

[T08] Kotlin：数据类
来源：http://hz.redwolf501.top/gtpclbkmua.html

data class User(val name: String, val age: Int)
来源：http://hz.zhijiandao.cn/gtkvtldajp.html

[T09] Kotlin：扩展函数
来源：http://hz.yanxiufei.cn/gtxkumjgev.html

fun String.exclaim() = this + "!"
来源：http://hz.ywan-chungtsiang.top/gtlxvvkfrq.html

[T10] Kotlin：默认参数
来源：http://hz.sysykeji.top/gtxioeutwl.html

fun greet(name: String = "World") = "Hi $name"
来源：http://hz.hywenlv.cn/gtfnrbesjo.html

[T11] Kotlin：协程
来源：http://hz.xylfe.cn/gtrehdzkqx.html

GlobalScope.launch { delay(1000); println("done") }
来源：http://hz.bjfxy.top/gtmfyfhtna.html

[T12] Kotlin：解构声明
来源：http://hz.shuidangran.top/gtxwcddubx.html

val (a, b) = Pair(1, 2)
来源：http://hz.nanxuanxn.top/gtddclzugy.html

[T13] Kotlin：只读 Map
来源：http://hz.chenjidiqi.icu/gttvvidnyh.html

val m = mapOf("a" to 1)
来源：http://hz.jinghuilouyu.cn/gtwsbexumj.html

[T14] Kotlin：循环
来源：http://hz.jinghuilouyu.cn/gtqzplrhva.html

for (i in 1..10) println(i)
来源：http://hz.bjfxy.top/gtqeqlavjg.html

[T15] Kotlin：接口
来源：http://hz.hfpthk.cn/gtmpqzzcal.html

interface Shape { fun area(): Double }
来源：http://hz.smart0.xyz/gtzxrsoehf.html

[T16] Swift：Hello World
来源：http://hz.ydjk.org.cn/gtmsaquaqc.html

print("Hello")
来源：http://hz.sysykeji.top/gtjfizmbht.html

[T17] Swift：变量与常量
来源：http://hz.ybcxt.top/gtojazcccm.html

var a = 1;  let b = 2
来源：http://hz.fengsongda.top/gtpjglwmdi.html

[T18] Swift：字符串插值
来源：http://hz.shangyingyoupin.top/gtuivseddq.html

"值: \(b)"
来源：http://hz.quarkkingdee.top/gtvedgtiqj.html

[T19] Swift：可选绑定
来源：http://hz.yvedp.cn/gtwaoyxsou.html

if let n = opt { print(n) }
来源：http://hz.guannengcc.top/gttrugzmvm.html

[T20] Swift：数组操作
来源：http://hz.pengpengdd.cyou/gtrreogabd.html

var a = [1, 2, 3];  a.append(4)
来源：http://hz.sufxvd.cn/gtswenrihe.html

[T21] Swift：遍历
来源：http://hz.shuidangran.top/gtelqkjekk.html

for x in a { print(x) }
来源：http://hz.dashuyun.cn/gtwlakzikk.html

[T22] Swift：字典
来源：http://hz.yj20258888.top/gtlkmtmdbz.html

var d = ["a": 1];  d["b"] = 2
来源：http://hz.snrcjt.cn/gtcvwgteea.html

[T23] Swift：函数
来源：http://hz.daxiang520.top/gtvbikcqxu.html

func add(_ a: Int, _ b: Int) -> Int { a + b }
来源：http://hz.xinyue.icu/gtelmkbhlh.html

[T24] Swift：闭包
来源：http://hz.smart0.xyz/gtxfsrlacy.html

let f = { (x: Int) -> Int in x * 2 }
来源：http://hz.yongpay.top/gttomqirxm.html

[T25] Swift：结构体
来源：http://hz.pengpengdd.cyou/gtgjimocdq.html

struct P { var x: Int }
来源：http://hz.jinyuanbaomall.cn/gtgnijtiig.html

[T26] Swift：类与重写
来源：http://hz.hnqzz.top/gtosjkyoyc.html

class A: Base { override func f() {} }
来源：http://hz.daria6918.cn/gtnwpgihcq.html

[T27] Swift：错误处理
来源：http://hz.aizwys.cn/gtreqzjwku.html

do { try f() } catch { print(error) }
来源：http://hz.0kj1m.cn/gturvkuarq.html

[T28] Swift：枚举
来源：http://hz.cheryme.top/gtghxvfzfc.html

enum Color { case red, green }
来源：http://hz.svipenyu.cn/gtuihqimit.html

[T29] Swift：guard 提前返回
来源：http://hz.chenlongwang.top/gtszuixkoi.html

guard let x = opt else { return }
来源：http://hz.xziqi.cn/gtkoronilz.html

[T30] Swift：协议
来源：http://hz.jlsjyb.cn/gtxoqilnxb.html

protocol Shape { func area() -> Double }
来源：http://hz.cashguo.top/gtsbtyhmur.html

[T31] Lua：Hello World
来源：http://hz.svipenyu.cn/gtnomjamve.html

print("Hello")
来源：http://hz.quarkkingdee.top/gtbjslxdsb.html

[T32] Lua：局部变量
来源：http://hz.yj20258888.top/gtmyxrhfwr.html

local a = 1
来源：http://hz.haohaochexian.top/gtdywelhnl.html

[T33] Lua：表（数组）
来源：http://hz.yangfankeji.com/gtifvgvhkk.html

local t = {1, 2, 3};  t[4] = 4
来源：http://hz.haohaochexian.top/gtjycongjm.html

[T34] Lua：遍历表
来源：http://hz.yanxiufei.cn/gtigacxzvh.html

for i, v in ipairs(t) do print(i, v) end
来源：http://hz.chenjidiqi.icu/gtczzbbmpt.html

[T35] Lua：字典表
来源：http://hz.smart0.xyz/gthmhpbkur.html

local d = { a = 1 };  d.b = 2
来源：http://hz.ywan-chungtsiang.top/gttcqizyab.html

[T36] Lua：函数
来源：http://hz.cheryme.top/gtgwiqsxjq.html

function add(a, b) return a + b end
来源：http://hz.wangshuangyany.cn/gtisyhztbj.html

[T37] Lua：字符串拼接
来源：http://hz.tian-w.cn/gtmgkcfvpt.html

"a" .. "b"
来源：http://hz.c1oappe.top/gtuofgmloi.html

[T38] Lua：条件
来源：http://hz.ppjwa.cn/gtycggzioe.html

if x > 0 then print("正") end
来源：http://hz.nanxinkj.top/gtcatxwohy.html

[T39] Lua：模式匹配
来源：http://hz.fengsongda.top/gtbjcljkss.html

string.find(s, "%d+")
来源：http://hz.sweek.top/gthtmaatax.html

[T40] Lua：元表
来源：http://hz.cheryme.top/gtuzdbhtgq.html

setmetatable({}, { __index = base })
来源：http://hz.smart0.xyz/gtntccjjwn.html

[T41] Perl：Hello World
来源：http://hz.hysaishi.cn/gtjnveusqz.html

print "Hello\n";
来源：http://hz.andypj.xyz/gtgczutlkr.html

[T42] Perl：变量类型
来源：http://hz.zhixingplan.top/gtwkausdgu.html

my $a = 1;  my @arr = (1, 2, 3);  my %h = (a => 1);
来源：http://hz.zhiwuduotai.top/gtijpzbkoo.html

[T43] Perl：字符串插值
来源：http://hz.andypj.xyz/gtgwfamijs.html

"值: $a"
来源：http://hz.guannengcc.top/gtdmlqtpon.html

[T44] Perl：条件
来源：http://hz.shanyushiyangkeji.top/gtcumtkbik.html

if ($a > 0) { print "正"; }
来源：http://hz.shanyushiyangtech.top/gtondjgelw.html

[T45] Perl：数组遍历
来源：http://hz.ydjk.org.cn/gtlenvymsv.html

for my $x (@arr) { print $x; }
来源：http://hz.cheryme.top/gtzbmyuuup.html

[T46] Perl：哈希操作
来源：http://hz.tanke756.top/gtilprbaod.html

$h{b} = 2;  for my $k (keys %h) { print "$k=$h{$k}"; }
来源：http://hz.gaohongyu789.top/gtbczxbjlb.html

[T47] Perl：正则捕获
来源：http://hz.shangyingyoupin.top/gtahqooubb.html

if ($s =~ /(\d+)/) { print $1; }
来源：http://hz.dashuyun.cn/gtvnoyahme.html

[T48] Perl：正则替换
来源：http://hz.zhixingplan.top/gtinkuniyq.html

$s =~ s/old/new/g;
来源：http://hz.sweek.top/gtesgdtmjy.html

[T49] Perl：函数
来源：http://hz.vqdsnc.cn/gtlvyqyakv.html

sub add { my ($a, $b) = @_; return $a + $b; }
来源：http://hz.hnxiangtu.top/gtewvhgzfd.html

[T50] Perl：逐行读文件
来源：http://hz.xylfe.cn/gtirznvcgw.html

open my $fh, "<", "a.txt" or die $!;
来源：http://hz.tanke756.top/gtjeyeqjbl.html

while (my $line = <$fh>) { print $line; }
来源：http://hz.jinyuanbaomall.cn/gtqbbyxszz.html

[T51] Scala：Hello World
来源：http://hz.yj20258.top/gtjgweoecv.html

println("Hello")
来源：http://hz.fzhhl.top/gtqwfahiuh.html

[T52] Scala：变量
来源：http://hz.jyoumei.cn/gtuzlchulz.html

val a = 1;  var b = 2
来源：http://hz.kuanghao11.cn/gtxvpvlkdb.html

[T53] Scala：字符串插值
来源：http://hz.sysykeji.top/gtqmonvhvb.html

s"值: $b"
来源：http://hz.0kj1m.cn/gtmerimpau.html

[T54] Scala：集合映射
来源：http://hz.zhiwuduotai.top/gtlqtnkdei.html

List(1, 2, 3).map(_ * 2)
来源：http://hz.daxiang520.top/gtjkgrjpvc.html

[T55] Scala：集合过滤
来源：http://hz.gotoacloud.top/gtmihgkrqf.html

List(1, 2, 3).filter(_ > 1)
来源：http://hz.9152youxi.cn/gtkvqktjwy.html

[T56] Scala：样例类
来源：http://hz.daria6918.cn/gtpqswtzpa.html

case class User(name: String, age: Int)
来源：http://hz.ppjwa.cn/gtywcbxqwg.html

[T57] Scala：模式匹配
来源：http://hz.sysykeji.top/gtqsauhpax.html

x match { case 1 => "一"; case _ => "其他" }
来源：http://hz.vqdsnc.cn/gtwhfymnmu.html

[T58] Scala：函数定义
来源：http://hz.zhoulong.xyz/gttfyzfmhk.html

def add(a: Int, b: Int): Int = a + b
来源：http://hz.shuidangran.top/gtuzymgfke.html

[T59] Scala：循环
来源：http://hz.andypj.xyz/gthezqoueb.html

for (i <- 1 to 10) println(i)
来源：http://hz.0kj1m.cn/gtjmpiquvr.html

[T60] Scala：折叠
来源：http://hz.havefunace.top/gttiqqzqpx.html

List(1, 2, 3).foldLeft(0)(_ + _)
来源：http://hz.xuanzx.com/gttkzhkvcd.html

================================================================================
来源：http://hz.cqqwz.cn/gtkxuxklcw.html

U. 高频实用片段（Python / PHP / JavaScript 各 40 条）
来源：http://hz.tian-w.cn/gtidfaawuf.html

================================================================================
来源：http://hz.xingfuxueyuan.xyz/gtyhbvyray.html

[U01] Py：创建虚拟环境
来源：http://hz.yvedp.cn/gtdkmoajtr.html

python -m venv .venv && source .venv/bin/activate
来源：http://hz.quarkkingdee.top/gtgncknrxa.html

[U02] Py：导出 / 安装依赖
来源：http://hz.xuetiantiany.cn/gtiotfgfkq.html

pip freeze > requirements.txt;  pip install -r requirements.txt
来源：http://hz.52xcode.cn/gtzxgvxdvi.html

[U03] Py：加载 .env 配置
来源：http://hz.hongshengwenyu.top/gtxjclkpxt.html

from dotenv import load_dotenv; load_dotenv()
来源：http://hz.yj202588.top/gtfatvvlnz.html

[U04] Py：变量调试打印
来源：http://hz.smart0.xyz/gtemwcxsdx.html

print(f"{x=}")            # 输出 x=值，Python 3.8+
来源：http://hz.xinyue.icu/gteerrltgt.html

[U05] Py：列表去重且保序
来源：http://hz.yangfankeji.com/gtamrishtx.html

list(dict.fromkeys(arr))
来源：http://hz.fzhhl.top/gtgwcfzkkm.html

[U06] Py：合并两个字典
来源：http://hz.yj20258888.top/gtadoltezf.html

{**a, **b}
来源：http://hz.cucudq.cn/gtlsqiwlnh.html

[U07] Py：反转字典键值
来源：http://hz.yanxiufei.cn/gtrnyfybkv.html

{v: k for k, v in d.items()}
来源：http://hz.hfpthk.cn/gtevsqixlq.html

[U08] Py：展平二维列表
来源：http://hz.jqgfzy.top/gtdqyyakzk.html

[y for x in nested for y in x]
来源：http://hz.ppjwa.cn/gtijawxaqn.html

[U09] Py：字典取最大值的键
来源：http://hz.hysaishi.cn/gteddjobjm.html

max(d, key=d.get)
来源：http://hz.hysaishi.cn/gtlphvljmt.html

[U10] Py：按值排序字典
来源：http://hz.haohaochexian.top/gtbhmgzkcd.html

dict(sorted(d.items(), key=lambda kv: kv[1]))
来源：http://hz.shangyingyoupin.top/gtasgeatvx.html

[U11] Py：生成器表达式
来源：http://hz.ydzc1.top/gtkfxhqgoj.html

(x * 2 for x in arr)
来源：http://hz.birdmap.top/gtcimqnaxs.html

[U12] Py：取出现最多的 3 个元素
来源：http://hz.yueranfly.top/gtwfoeipvk.html

Counter(arr).most_common(3)
来源：http://hz.9152youxi.cn/gtzfspiufz.html

[U13] Py：固定长度队列
来源：http://hz.hysaishi.cn/gtgqytknuo.html

deque(maxlen=10)
来源：http://hz.shangyingyoupin.top/gtccksdnow.html

[U14] Py：分组收集到列表
来源：http://hz.zhixingplan.top/gtoqkewnak.html

defaultdict(list)
来源：http://hz.zhoulong.xyz/gtyxuddwuk.html

[U15] Py：高精度计时
来源：http://hz.cqqwz.cn/gtndjngoiw.html

t = time.perf_counter()
来源：http://hz.yueranfly.top/gtdetmntqa.html

[U16] Py：命令行参数解析
来源：http://hz.zhiwuduotai.top/gtnysfnqxm.html

ap = argparse.ArgumentParser();  ap.add_argument("--name");  args = ap.parse_args()
来源：http://hz.jqgfzy.top/gtcqisqjbf.html

[U17] Py：初始化日志
来源：http://hz.cheryme.top/gtcailkvlf.html

logging.basicConfig(level=logging.INFO)
来源：http://hz.pengpengdd.cyou/gtxjqlqhub.html

[U18] Py：预编译正则
来源：http://hz.jinqigfzy.top/gtxxionzca.html

pat = re.compile(r"\d+")
来源：http://hz.gzhubu.top/gtbmgalflk.html

[U19] Py：正则替换带回调
来源：http://hz.xuanzx.com/gtyzzjcthe.html

re.sub(r"\d+", lambda m: str(int(m.group()) * 2), s)
来源：http://hz.wangdashe.top/gtmjedpugh.html

[U20] Py：缓存函数结果
来源：http://hz.vqdsnc.cn/gtqvpzkwyf.html

@functools.lru_cache(maxsize=None)
来源：http://hz.yangfankeji.com/gtgzzcvdeb.html

[U21] Py：自定义上下文管理器
来源：http://hz.andypj.xyz/gtzyvpbmag.html

@contextlib.contextmanager
来源：http://hz.yanxiufei.cn/gtqiuthanp.html

[U22] Py：矩阵转置
来源：http://hz.shanyushiyangtech.top/gtoexuonvk.html

list(zip(*m))
来源：http://hz.kuanghao11.cn/gtliockces.html

[U23] Py：分块读取大文件
来源：http://hz.ivvv.top/gtaezshlev.html

for chunk in iter(lambda: f.read(8192), b""):
来源：http://hz.yuanzhike.top/gtrglcmsyg.html

[U24] Py：路径操作
来源：http://hz.haohaochexian.top/gtluaippid.html

Path("a/b.txt").parent.mkdir(parents=True, exist_ok=True)
来源：http://hz.kuanghao11.cn/gthekugzvr.html

[U25] Py：CSV 按字典读
来源：http://hz.havefunace.top/gtptscriqn.html

csv.DictReader(f)
来源：http://hz.yvedp.cn/gtoudhyxcb.html

[U26] Py：并发下载
来源：http://hz.zhengqikj.top/gtpejbfspa.html

ThreadPoolExecutor(max_workers=8).map(fetch, urls)
来源：http://hz.yanxiufei.cn/gtaquqmxok.html

[U27] Py：异步 HTTP
来源：http://hz.yanxiufei.cn/gtqprdivdh.html

aiohttp.ClientSession() 配合 async with
来源：http://hz.snrcjt.cn/gtdppskitm.html

[U28] Py：类型别名
来源：http://hz.jinyuanbaomall.cn/gtxlkvbhru.html

UserId = int
来源：http://hz.hysaishi.cn/gtkdrmxmkx.html

[U29] Py：属性校验
来源：http://hz.yueranfly.top/gtqtgjlast.html

@property 与 @x.setter 配合
来源：http://hz.sxryk.cn/gtxfkfymzn.html

[U30] Py：数据类
来源：http://hz.hywenlv.cn/gttlgqqcuj.html

@dataclass(slots=True)
来源：http://hz.gaohongyu789.top/gtnmarrkmz.html

[U31] Py：单测
来源：http://hz.yangfankeji.com/gtkcsialhj.html

python -m pytest -q
来源：http://hz.zhongyouzk.top/gtnpcrhlko.html

[U32] Py：代码格式化
来源：http://hz.birdmap.top/gtzspribgl.html

ruff format . && ruff check --fix .
来源：http://hz.pengpengdd.cyou/gtcfkkbrxt.html

[U33] Py：打包发布
来源：http://hz.fzhhl.top/gtizjomddo.html

python -m build  （依赖 pyproject.toml）
来源：http://hz.bjfxy.top/gtnhucwqev.html

[U34] Py：判断编码
来源：http://hz.ivvv.top/gtrkecqpeq.html

chardet.detect(raw)
来源：http://hz.shangyingyoupin.top/gtfudsgxeq.html

[U35] Py：发送邮件
来源：http://hz.fzhhl.top/gtljkvaoop.html

smtplib.SMTP_SSL(...).send_message(msg)
来源：http://hz.yuxming.cn/gtnopwwjof.html

[U36] Py：定时任务
来源：http://hz.meibo888.top/gtovkzxmne.html

schedule.every(10).minutes.do(job)
来源：http://hz.svipenyu.cn/gtbqcfmqsg.html

[U37] Py：读写 Excel
来源：http://hz.dianchejie.cn/gtlsckngxk.html

pandas.read_excel / DataFrame.to_excel
来源：http://hz.jianghu66.top/gtprnfjfts.html

[U38] Py：获取脚本所在目录
来源：http://hz.quarkkingdee.top/gtzsdrvfys.html

Path(__file__).resolve().parent
来源：http://hz.hnqzz.top/gtrjnvmekk.html

[U39] Py：判断是否在交互环境
来源：http://hz.yvedp.cn/gtmyarmorm.html

sys.stdout.isatty()
来源：http://hz.ywan-chungtsiang.top/gtkczjnzbv.html

[U40] Py：打印到标准错误
来源：http://hz.kuanghao11.cn/gtmbzvaozx.html

print("err", file=sys.stderr)
来源：http://hz.jianghu66.top/gtzbsetqug.html

[U41] PHP：初始化 Composer 项目
来源：http://hz.jinghuilouyu.cn/gtdqmrikzc.html

composer init;  composer require guzzlehttp/guzzle
来源：http://hz.chenjidiqi.icu/gtirtcolqr.html

[U42] PHP：PSR-4 自动加载
来源：http://hz.dashuyun.cn/gtvwwsrotv.html

"autoload": { "psr-4": { "App\\": "src/" } }
来源：http://hz.jinyuanbaomall.cn/gtssaomfnq.html

[U43] PHP：声明命名空间
来源：http://hz.bjfxy.top/gtobhvnvro.html

namespace App\Http;
来源：http://hz.jinyuanbaomall.cn/gtuvdspyva.html

[U44] PHP：开启严格类型
来源：http://hz.jlsjyb.cn/gtvqvsofbe.html

declare(strict_types=1);
来源：http://hz.dianchejie.cn/gtpzpcbnzj.html

[U45] PHP：类型声明与返回类型
来源：http://hz.snrcjt.cn/gtuurtfuxb.html

function add(int $a, int $b): int { return $a + $b; }
来源：http://hz.hfpthk.cn/gteghompor.html

[U46] PHP：可空类型
来源：http://hz.zhaomingkeji.xyz/gtahjiuxwt.html

?string $name = null
来源：http://hz.zhijiandao.cn/gtjhcterbd.html


<!-- 参考信息 -->