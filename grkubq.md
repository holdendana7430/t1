代发 wailian999

static int counter = 0;
来源：http://hz.0kj1m.cn/gtdivyaybg.html

[S29] C：变参函数
来源：http://hz.zhoulong.xyz/gtkidckwmd.html

va_list ap; va_start(ap, fmt); vprintf(fmt, ap); va_end(ap);
来源：http://hz.dashuyun.cn/gtyffuclto.html

[S30] C：头文件保护
来源：http://hz.316326.xyz/gtmxkoswbn.html

#ifndef X_H
来源：http://hz.yonumen.top/gtagmksjhr.html

#define X_H
来源：http://hz.shanyushiyangtech.top/gtpxnqptvo.html

#endif
来源：http://hz.pycfn.com/gttilalvsn.html

[S31] C++：Hello World
来源：http://hz.yj20258888.top/gtifwwnxjr.html

#include <iostream>
来源：http://hz.sxryk.cn/gtmkcsurca.html

int main() { std::cout << "Hello\n"; }
来源：http://hz.xingfuxueyuan.xyz/gtqjznajdj.html

[S32] C++：字符串
来源：http://hz.yanxiufei.cn/gtzztkvyrc.html

std::string s = "hi";  s += "!";
来源：http://hz.jqgufenzy.top/gteijfrjhg.html

[S33] C++：vector 增删
来源：http://hz.hnqzz.top/gturwqccbm.html

std::vector<int> v{1, 2, 3};  v.push_back(4);
来源：http://hz.sxryk.cn/gtmgxdisgu.html

[S34] C++：遍历 vector
来源：http://hz.jlsjyb.cn/gtsbsgsogu.html

for (auto &x : v) { std::cout << x; }
来源：http://hz.cashguo.top/gtlmsjvzim.html

[S35] C++：map
来源：http://hz.aibaodan.cn/gtyqxczdgi.html

std::map<std::string, int> m;  m["a"] = 1;
来源：http://hz.zhoulong.xyz/gtcihejutb.html

[S36] C++：unordered_map
来源：http://hz.hnqzz.top/gtfhtziorq.html

std::unordered_map<std::string, int> m;  m["a"] = 1;
来源：http://hz.iojbl.cn/gtjgnxaxgg.html

[S37] C++：set
来源：http://hz.yueranfly.top/gttonsfsfx.html

std::set<int> s{1, 2, 3};  s.insert(4);
来源：http://hz.yanxiufei.cn/gtxaqvswwf.html

[S38] C++：排序
来源：http://hz.tianlin.xyz/gtyrbbtrna.html

std::sort(v.begin(), v.end());
来源：http://hz.c1oappe.top/gtoszlphul.html

[S39] C++：自定义比较器排序
来源：http://hz.yueranfly.top/gtqyldsktz.html

std::sort(v.begin(), v.end(), [](int a, int b) { return a > b; });
来源：http://hz.yongpay.top/gtlxhafzna.html

[S40] C++：查找元素
来源：http://hz.chenjidiqi.icu/gtwhgbqlfo.html

auto it = std::find(v.begin(), v.end(), 3);
来源：http://hz.nanxuanxn.top/gtsseyomlj.html

[S41] C++：类与构造函数
来源：http://hz.zhijiandao.cn/gtfbgtxdat.html

class A { public: A(int v) : x_(v) {} int get() const { return x_; } private: int x_; };
来源：http://hz.c1oappe.top/gtlrnpezxu.html

[S42] C++：继承与虚函数
来源：http://hz.ehwqpu.com/gtukifimet.html

class B : public Base { public: void f() override {} };
来源：http://hz.ivvv.top/gtdbdmoqjn.html

[S43] C++：智能指针
来源：http://hz.vqdsnc.cn/gtvgrnsmgs.html

auto p = std::make_unique<int>(5);
来源：http://hz.guowangkeji.top/gtkxczowqy.html

[S44] C++：引用传参
来源：http://hz.svipenyu.cn/gtqvmzmfmf.html

void inc(int &x) { ++x; }
来源：http://hz.sweek.top/gticutgeah.html

[S45] C++：lambda
来源：http://hz.zhaomingkeji.xyz/gtndlupacv.html

auto add = [](int a, int b) { return a + b; };
来源：http://hz.feifeiyinyue.top/gtqfcazxrh.html

[S46] C++：函数模板
来源：http://hz.aizwys.cn/gtbgjrwdyt.html

template <typename T> T maxv(T a, T b) { return a > b ? a : b; }
来源：http://hz.ydjk.org.cn/gtbeeeazld.html

[S47] C++：结构化绑定遍历
来源：http://hz.zhoulong.xyz/gtxdkkqsgt.html

for (const auto &[k, v] : m) { std::cout << k << v; }
来源：http://hz.tian-w.cn/gthetyvbvj.html

[S48] C++：逐行读文件
来源：http://hz.sweek.top/gtmvzpihuq.html

std::ifstream in("a.txt");  std::string line;
来源：http://hz.tian-w.cn/gtdsymnyoy.html

while (std::getline(in, line)) { }
来源：http://hz.yangfankeji.com/gtiaozvush.html

[S49] C++：写文件
来源：http://hz.yuxming.cn/gtqtuovoyv.html

std::ofstream out("a.txt");  out << "hi\n";
来源：http://hz.dianchejie.cn/gtvicgzmmw.html

[S50] C++：格式化数字
来源：http://hz.daria6918.cn/gtiaqonjur.html

std::ostringstream os;  os << std::fixed << std::setprecision(2) << 3.14159;
来源：http://hz.yongpay.top/gtiqkchmbz.html

[S51] C++：显式类型转换
来源：http://hz.guannengcc.top/gtjvwkonya.html

static_cast<double>(a) / b
来源：http://hz.xziqi.cn/gtvkalbhuj.html

[S52] C++：const 与 noexcept
来源：http://hz.haohaochexian.top/gtrzxwrccu.html

int size() const noexcept { return n_; }
来源：http://hz.ppjwa.cn/gtylrxqljc.html

[S53] C++：移动语义
来源：http://hz.jinqigfzy.top/gtjkmorlin.html

std::vector<int> w = std::move(v);
来源：http://hz.yj20258.top/gtgzawnswm.html

[S54] C++：异常处理
来源：http://hz.hammf.cn/gtmmjdscvv.html

try { throw std::runtime_error("x"); } catch (const std::exception &e) { }
来源：http://hz.nanxuanxn.top/gtkchvirge.html

[S55] C++：结构化绑定
来源：http://hz.shzxlz.cn/gtxbapffek.html

auto [a, b] = std::make_pair(1, 2);
来源：http://hz.vqdsnc.cn/gtsfigojgx.html

[S56] C++：optional
来源：http://hz.sxryk.cn/gtoqhdvwme.html

std::optional<int> o = 5;  if (o) { int v = *o; }
来源：http://hz.jiagoushi.top/gtyqubzsoc.html

[S57] C++：编译期常量
来源：http://hz.chenlongwang.top/gtlkunvzfe.html

constexpr int N = 10;
来源：http://hz.iojbl.cn/gtruxvilow.html

[S58] C++：命名空间
来源：http://hz.jiagoushi.top/gtzurvipgj.html

namespace ns { int f() { return 1; } }
来源：http://hz.yangfankeji.com/gtucuwqkms.html

[S59] C++：静态断言
来源：http://hz.nwbrower.top/gteihrpjbv.html

static_assert(sizeof(int) == 4, "int 必须 4 字节");
来源：http://hz.shzxlz.cn/gtigypebev.html

[S60] C++：遍历并删除元素
来源：http://hz.fzhhl.top/gtqjixqoua.html

v.erase(std::remove_if(v.begin(), v.end(), [](int x) { return x < 0; }), v.end());
来源：http://hz.xinyue.icu/gtmzdojcpy.html

================================================================================
来源：http://hz.aizwys.cn/gtniaatskn.html

T. 其他语言补充（Kotlin / Swift / Lua / Perl / Scala）
来源：http://hz.shangyingyoupin.top/gtbuwcxdnm.html

================================================================================
来源：http://hz.yuanzhike.top/gtcoetpxki.html

[T01] Kotlin：Hello World
来源：http://hz.meibo888.top/gtmtpnhhjs.html

println("Hello")
来源：http://hz.birdmap.top/gtqwpzvfti.html

[T02] Kotlin：变量
来源：http://hz.guannengcc.top/gtwmrkftpi.html

val a = 1;  var b = 2        // val 只读，var 可变
来源：http://hz.tanke756.top/gttwyugvhj.html

[T03] Kotlin：字符串模板
来源：http://hz.guowangkeji.top/gtokmhiakl.html

"值: $b"
来源：http://hz.zhixingplan.top/gtiagjaylq.html

[T04] Kotlin：空安全
来源：http://hz.zhixingplan.top/gtcsuzqwyi.html

val n: String? = null;  n?.length
来源：http://hz.tian-w.cn/gtcdphbzta.html

[T05] Kotlin：when 表达式
来源：http://hz.316326.xyz/gtcciofkrt.html

val s = when (x) { 1 -> "一" else -> "其他" }   // 多分支时每个分支单独一行
来源：http://hz.gogol.net.cn/gtzeglbttq.html

[T06] Kotlin：集合映射
来源：http://hz.ivvv.top/gtkauvucjl.html

listOf(1, 2, 3).map { it * 2 }
来源：http://hz.ehwqpu.com/gtvpacftfa.html

[T07] Kotlin：集合过滤
来源：http://hz.guowangkeji.top/gtkzavxcwi.html

listOf(1, 2, 3).filter { it > 1 }
来源：http://hz.jinqigufen.top/gtpsxiblgm.html

[T08] Kotlin：数据类
来源：http://hz.tanke756.top/gteyuywczq.html

data class User(val name: String, val age: Int)
来源：http://hz.hongshengwenyu.top/gtqxraronw.html

[T09] Kotlin：扩展函数
来源：http://hz.cqqwz.cn/gtvzvvvxxw.html

fun String.exclaim() = this + "!"
来源：http://hz.shuidangran.top/gtsgwyxpvq.html

[T10] Kotlin：默认参数
来源：http://hz.chenzaomai.com/gtlirpxlgr.html

fun greet(name: String = "World") = "Hi $name"
来源：http://hz.yangfankeji.com/gttscrnzpm.html

[T11] Kotlin：协程
来源：http://hz.xylfe.cn/gtnuzmwlat.html

GlobalScope.launch { delay(1000); println("done") }
来源：http://hz.xinyue.icu/gtwiyrvmrb.html

[T12] Kotlin：解构声明
来源：http://hz.zhixingplan.top/gtfxuiixat.html

val (a, b) = Pair(1, 2)
来源：http://hz.zhongyouzk.top/gtzojoliwt.html

[T13] Kotlin：只读 Map
来源：http://hz.yuxming.cn/gtjxtaiagz.html

val m = mapOf("a" to 1)
来源：http://hz.tian-w.cn/gtwwmfntkg.html

[T14] Kotlin：循环
来源：http://hz.shangyingyoupin.top/gtwslbwtxu.html

for (i in 1..10) println(i)
来源：http://hz.52xcode.cn/gtlfngkzdu.html

[T15] Kotlin：接口
来源：http://hz.redwolf501.top/gtvpnvgspe.html

interface Shape { fun area(): Double }
来源：http://hz.tanke756.top/gtjxygnhmq.html

[T16] Swift：Hello World
来源：http://hz.xuanzx.com/gtnbroqbfv.html

print("Hello")
来源：http://hz.zhixingplan.top/gtzwhoaedg.html

[T17] Swift：变量与常量
来源：http://hz.cucudq.cn/gthakgcilw.html

var a = 1;  let b = 2
来源：http://hz.haohaochexian.top/gtzmscmrqa.html

[T18] Swift：字符串插值
来源：http://hz.zdqjudy.top/gtrcqsatvz.html

"值: \(b)"
来源：http://hz.hnxiangtu.top/gtmydltwzc.html

[T19] Swift：可选绑定
来源：http://hz.fzhhl.top/gtjngjzsdv.html

if let n = opt { print(n) }
来源：http://hz.vqdsnc.cn/gtkobqouud.html

[T20] Swift：数组操作
来源：http://hz.dianchejie.cn/gtyfyeznxg.html

var a = [1, 2, 3];  a.append(4)
来源：http://hz.xuanzx.com/gthunhgrnb.html

[T21] Swift：遍历
来源：http://hz.fengsongda.top/gtnotfopqs.html

for x in a { print(x) }
来源：http://hz.zhongyouzk.top/gtnvzlzljr.html

[T22] Swift：字典
来源：http://hz.daria6918.cn/gtqiouyiuq.html

var d = ["a": 1];  d["b"] = 2
来源：http://hz.pycfn.com/gtyosnfole.html

[T23] Swift：函数
来源：http://hz.tian-w.cn/gtnaqbycan.html

func add(_ a: Int, _ b: Int) -> Int { a + b }
来源：http://hz.fzhhl.top/gtqdsmpqgu.html

[T24] Swift：闭包
来源：http://hz.meibo888.top/gtwxvkqlhp.html

let f = { (x: Int) -> Int in x * 2 }
来源：http://hz.cashguo.top/gtiourvvhz.html

[T25] Swift：结构体
来源：http://hz.cdnleiting.top/gtjshlkwtk.html

struct P { var x: Int }
来源：http://hz.52xcode.cn/gtcrbckjvw.html

[T26] Swift：类与重写
来源：http://hz.hnxiangtu.top/gtfzqomgwq.html

class A: Base { override func f() {} }
来源：http://hz.yongpay.top/gthgkjbcgy.html

[T27] Swift：错误处理
来源：http://hz.wangdashe.top/gtekanupfh.html

do { try f() } catch { print(error) }
来源：http://hz.tian-w.cn/gtzqrqbbaw.html

[T28] Swift：枚举
来源：http://hz.wangshuangyany.cn/gtohqxiqxm.html

enum Color { case red, green }
来源：http://hz.dashuyun.cn/gtbbgdpgdl.html

[T29] Swift：guard 提前返回
来源：http://hz.fengsongda.top/gtpnditwhz.html

guard let x = opt else { return }
来源：http://hz.yanxiufei.cn/gtelbxbpdg.html

[T30] Swift：协议
来源：http://hz.shanyushiyangtech.top/gtolrmvaic.html

protocol Shape { func area() -> Double }
来源：http://hz.smart0.xyz/gtfftvtgez.html

[T31] Lua：Hello World
来源：http://hz.cheryme.top/gtvyflieic.html

print("Hello")
来源：http://hz.0kj1m.cn/gtibfbwqtq.html

[T32] Lua：局部变量
来源：http://hz.jqgfzy.top/gtmndbxyvs.html

local a = 1
来源：http://hz.xinyue.icu/gtfshpclja.html

[T33] Lua：表（数组）
来源：http://hz.yanxiufei.cn/gtqzmbadhu.html

local t = {1, 2, 3};  t[4] = 4
来源：http://hz.zycfv.cn/gttxgmamfo.html

[T34] Lua：遍历表
来源：http://hz.0kj1m.cn/gtjvjrikgu.html

for i, v in ipairs(t) do print(i, v) end
来源：http://hz.tian-w.cn/gtlumptwdc.html

[T35] Lua：字典表
来源：http://hz.ehwqpu.com/gtatkegyry.html

local d = { a = 1 };  d.b = 2
来源：http://hz.andypj.xyz/gtmzhoqtiu.html

[T36] Lua：函数
来源：http://hz.bjfxy.top/gthtgqjavt.html

function add(a, b) return a + b end
来源：http://hz.fengsongda.top/gtbimrpvkr.html

[T37] Lua：字符串拼接
来源：http://hz.xinyue.icu/gtqfhuhfjh.html

"a" .. "b"
来源：http://hz.hfpthk.cn/gtffjhpbvc.html

[T38] Lua：条件
来源：http://hz.wangdashe.top/gtvahqvcbj.html

if x > 0 then print("正") end
来源：http://hz.nanxuanxn.top/gtajpncqos.html

[T39] Lua：模式匹配
来源：http://hz.ydzc1.top/gtjnabdpqw.html

string.find(s, "%d+")
来源：http://hz.0kj1m.cn/gtriqiyyzh.html

[T40] Lua：元表
来源：http://hz.smart0.xyz/gtmyxfomgx.html

setmetatable({}, { __index = base })
来源：http://hz.zhiwuduotai.top/gtlkpsnzpa.html

[T41] Perl：Hello World
来源：http://hz.aibaodan.cn/gtazcysnsi.html

print "Hello\n";
来源：http://hz.wangdashe.top/gtxhhgmcsr.html

[T42] Perl：变量类型
来源：http://hz.hnqzz.top/gtlkjjnrzy.html

my $a = 1;  my @arr = (1, 2, 3);  my %h = (a => 1);
来源：http://hz.yonumen.top/gtkwjdqfmt.html

[T43] Perl：字符串插值
来源：http://hz.chenzaomai.com/gtznydwheb.html

"值: $a"
来源：http://hz.yueranfly.top/gttwoaadbz.html

[T44] Perl：条件
来源：http://hz.gogol.net.cn/gtaodpeopk.html

if ($a > 0) { print "正"; }
来源：http://hz.pengpengdd.cyou/gtrsdbnozm.html

[T45] Perl：数组遍历
来源：http://hz.jqgfzy.top/gttuppbpsd.html

for my $x (@arr) { print $x; }
来源：http://hz.nanxinkj.top/gtyoccmyap.html

[T46] Perl：哈希操作
来源：http://hz.shzxlz.cn/gtrpapkkbm.html

$h{b} = 2;  for my $k (keys %h) { print "$k=$h{$k}"; }
来源：http://hz.jinyuanbaomall.cn/gtsnjewyal.html

[T47] Perl：正则捕获
来源：http://hz.chenzaomai.com/gthzwtpctl.html

if ($s =~ /(\d+)/) { print $1; }
来源：http://hz.shanyushiyangtech.top/gttxeffmsc.html

[T48] Perl：正则替换
来源：http://hz.c1oappe.top/gtkwkuphya.html

$s =~ s/old/new/g;
来源：http://hz.hywenlv.cn/gtxsgrhyza.html

[T49] Perl：函数
来源：http://hz.jinyuanbaomall.cn/gtzbrxuslb.html

sub add { my ($a, $b) = @_; return $a + $b; }
来源：http://hz.xuanzx.com/gtprisbqfy.html

[T50] Perl：逐行读文件
来源：http://hz.hammf.cn/gtlbfeasrz.html

open my $fh, "<", "a.txt" or die $!;
来源：http://hz.gaohongyu789.top/gtnfkmmwbo.html

while (my $line = <$fh>) { print $line; }
来源：http://hz.quarkkingdee.top/gtrgxgaupe.html

[T51] Scala：Hello World
来源：http://hz.yuxming.cn/gtpadqqwda.html

println("Hello")
来源：http://hz.52xcode.cn/gtbvqzxobw.html

[T52] Scala：变量
来源：http://hz.shanyushiyangkeji.top/gtwrlkdhem.html

val a = 1;  var b = 2
来源：http://hz.yueranfly.top/gtwrgxrqsx.html

[T53] Scala：字符串插值
来源：http://hz.andypj.xyz/gthjqkqrnw.html

s"值: $b"
来源：http://hz.jinyuanbaomall.cn/gtwatsirba.html

[T54] Scala：集合映射
来源：http://hz.xylfe.cn/gtatwjqluq.html

List(1, 2, 3).map(_ * 2)
来源：http://hz.daria6918.cn/gtxrefjbxc.html

[T55] Scala：集合过滤
来源：http://hz.sxryk.cn/gtunwarfic.html

List(1, 2, 3).filter(_ > 1)
来源：http://hz.xingfuxueyuan.xyz/gtowvxezil.html

[T56] Scala：样例类
来源：http://hz.feifeiyinyue.top/gtinmvqjfq.html

case class User(name: String, age: Int)
来源：http://hz.jlsjyb.cn/gthjppvzfz.html

[T57] Scala：模式匹配
来源：http://hz.gaohongyu789.top/gtjixhlnjp.html

x match { case 1 => "一"; case _ => "其他" }
来源：http://hz.ivvv.top/gtujfndtql.html

[T58] Scala：函数定义
来源：http://hz.bjfxy.top/gtcixsijid.html

def add(a: Int, b: Int): Int = a + b
来源：http://hz.pycfn.com/gtcerycubp.html

[T59] Scala：循环
来源：http://hz.zdqjudy.top/gtsatpxqdu.html

for (i <- 1 to 10) println(i)
来源：http://hz.bjfxy.top/gtqfbrijtp.html

[T60] Scala：折叠
来源：http://hz.shanyushiyangkeji.top/gtgatnfktp.html

List(1, 2, 3).foldLeft(0)(_ + _)
来源：http://hz.c1oappe.top/gthsrayacs.html

================================================================================
来源：http://hz.yueranfly.top/gtrtqqdclg.html

U. 高频实用片段（Python / PHP / JavaScript 各 40 条）
来源：http://hz.yuxming.cn/gtxczxlyhv.html

================================================================================
来源：http://hz.yj20258888.top/gttgoxpgvz.html

[U01] Py：创建虚拟环境
来源：http://hz.gogol.net.cn/gtemtwnwbd.html

python -m venv .venv && source .venv/bin/activate
来源：http://hz.yonumen.top/gttdvfxmoo.html

[U02] Py：导出 / 安装依赖
来源：http://hz.jinqigufen.top/gtvwlxhziv.html

pip freeze > requirements.txt;  pip install -r requirements.txt
来源：http://hz.sweek.top/gtaejbgzkd.html

[U03] Py：加载 .env 配置
来源：http://hz.tanke756.top/gtfdhvfjxs.html

from dotenv import load_dotenv; load_dotenv()
来源：http://hz.hongshengwenyu.top/gtetvatpxp.html

[U04] Py：变量调试打印
来源：http://hz.yj20258888.top/gtivqevyef.html

print(f"{x=}")            # 输出 x=值，Python 3.8+
来源：http://hz.cucudq.cn/gtkqfzpqzy.html

[U05] Py：列表去重且保序
来源：http://hz.nanxuanxn.top/gtljntipcx.html

list(dict.fromkeys(arr))
来源：http://hz.birdmap.top/gtcjebsbiw.html

[U06] Py：合并两个字典
来源：http://hz.tianlin.xyz/gtbchzbouk.html

{**a, **b}
来源：http://hz.nwbrower.top/gtfzaacieb.html

[U07] Py：反转字典键值
来源：http://hz.jinyuanbaomall.cn/gtyxipnuhq.html

{v: k for k, v in d.items()}
来源：http://hz.pycfn.com/gtirwtixpx.html

[U08] Py：展平二维列表
来源：http://hz.c1oappe.top/gtmakjnmra.html

[y for x in nested for y in x]
来源：http://hz.ehwqpu.com/gtqhiwwope.html

[U09] Py：字典取最大值的键
来源：http://hz.shuidangran.top/gtrbbzjtln.html

max(d, key=d.get)
来源：http://hz.jyoumei.cn/gtfoaacdyp.html

[U10] Py：按值排序字典
来源：http://hz.jinyuanbaomall.cn/gtjehjsmlo.html

dict(sorted(d.items(), key=lambda kv: kv[1]))
来源：http://hz.yuanzhike.top/gtmbtviolx.html

[U11] Py：生成器表达式
来源：http://hz.52xcode.cn/gtxiuolwaw.html

(x * 2 for x in arr)
来源：http://hz.chenzaomai.com/gtiddexvlj.html

[U12] Py：取出现最多的 3 个元素
来源：http://hz.ydjk.org.cn/gtnuzuzlmq.html

Counter(arr).most_common(3)
来源：http://hz.gaohongyu789.top/gtxogzdkzn.html

[U13] Py：固定长度队列
来源：http://hz.gogol.net.cn/gtuknzoaej.html

deque(maxlen=10)
来源：http://hz.316326.xyz/gtbzdczcwi.html

[U14] Py：分组收集到列表
来源：http://hz.fzhhl.top/gtlfdvzzqd.html

defaultdict(list)
来源：http://hz.wangshuangyany.cn/gtawxfzqly.html

[U15] Py：高精度计时
来源：http://hz.hammf.cn/gtsqoldphj.html

t = time.perf_counter()
来源：http://hz.shzxlz.cn/gtwuaugsfx.html

[U16] Py：命令行参数解析
来源：http://hz.jlsjyb.cn/gtuiskpfny.html

ap = argparse.ArgumentParser();  ap.add_argument("--name");  args = ap.parse_args()
来源：http://hz.yanxiufei.cn/gtzvevhwee.html

[U17] Py：初始化日志
来源：http://hz.xziqi.cn/gtiqfpvtrd.html

logging.basicConfig(level=logging.INFO)
来源：http://hz.hnxiangtu.top/gtwhvjxnar.html

[U18] Py：预编译正则
来源：http://hz.fzhhl.top/gtxgxgebqq.html

pat = re.compile(r"\d+")
来源：http://hz.yj20258.top/gttxcgqxiu.html

[U19] Py：正则替换带回调
来源：http://hz.gotoacloud.top/gtnojxhdlv.html

re.sub(r"\d+", lambda m: str(int(m.group()) * 2), s)
来源：http://hz.xingfuxueyuan.xyz/gtwqnlitju.html

[U20] Py：缓存函数结果
来源：http://hz.yueranfly.top/gtqucfemcq.html

@functools.lru_cache(maxsize=None)
来源：http://hz.hnxiangtu.top/gtsrzbelpe.html

[U21] Py：自定义上下文管理器
来源：http://hz.daxiang520.top/gtuiqsfmbp.html

@contextlib.contextmanager
来源：http://hz.haohaochexian.top/gtdfjvyaqm.html

[U22] Py：矩阵转置
来源：http://hz.52xcode.cn/gticwodlcj.html

list(zip(*m))
来源：http://hz.zhengqikj.top/gtiobcdmvf.html

[U23] Py：分块读取大文件
来源：http://hz.gaohongyu789.top/gtxzjmsbpl.html

for chunk in iter(lambda: f.read(8192), b""):
来源：http://hz.vqdsnc.cn/gtxfjsgcyi.html

[U24] Py：路径操作
来源：http://hz.yongpay.top/gtoiibwbsu.html

Path("a/b.txt").parent.mkdir(parents=True, exist_ok=True)
来源：http://hz.yj20258888.top/gtopcrsjto.html

[U25] Py：CSV 按字典读
来源：http://hz.0kj1m.cn/gtxmucfnul.html

csv.DictReader(f)
来源：http://hz.ppjwa.cn/gtrqllrjfx.html

[U26] Py：并发下载
来源：http://hz.ppjwa.cn/gtnrhwfkxd.html

ThreadPoolExecutor(max_workers=8).map(fetch, urls)
来源：http://hz.fengsongda.top/gtqhwszmsj.html

[U27] Py：异步 HTTP
来源：http://hz.yuanzhike.top/gtystrhcxe.html

aiohttp.ClientSession() 配合 async with
来源：http://hz.ybcxt.top/gtsaiojrlv.html

[U28] Py：类型别名
来源：http://hz.jinghuilouyu.cn/gtywxkesie.html

UserId = int
来源：http://hz.jianghu66.top/gtamyxdkje.html

[U29] Py：属性校验
来源：http://hz.9152youxi.cn/gtedkdedgc.html

@property 与 @x.setter 配合
来源：http://hz.cqqwz.cn/gtxvfbvctg.html

[U30] Py：数据类
来源：http://hz.nanxuanxn.top/gtnytbkuoy.html

@dataclass(slots=True)
来源：http://hz.iojbl.cn/gtlcryipxh.html

[U31] Py：单测
来源：http://hz.xziqi.cn/gtqabesemf.html

python -m pytest -q
来源：http://hz.kuanghao11.cn/gtfhyvzjim.html

[U32] Py：代码格式化
来源：http://hz.yuanzhike.top/gtfvhrcolj.html

ruff format . && ruff check --fix .
来源：http://hz.daria6918.cn/gttkicpdxh.html

[U33] Py：打包发布
来源：http://hz.pengpengdd.cyou/gtjedsixaj.html

python -m build  （依赖 pyproject.toml）
来源：http://hz.xuanzx.com/gtwdanzust.html

[U34] Py：判断编码
来源：http://hz.hnqzz.top/gtfjaqeklx.html

chardet.detect(raw)
来源：http://hz.jinghuilouyu.cn/gtytokkruk.html

[U35] Py：发送邮件
来源：http://hz.nanxuanxn.top/gtjpgpodsb.html

smtplib.SMTP_SSL(...).send_message(msg)
来源：http://hz.guannengcc.top/gtikeebedt.html

[U36] Py：定时任务
来源：http://hz.yongpay.top/gtkickkgkj.html

schedule.every(10).minutes.do(job)
来源：http://hz.daxiang520.top/gtihqpwmiv.html

[U37] Py：读写 Excel
来源：http://hz.316326.xyz/gtclsgindr.html

pandas.read_excel / DataFrame.to_excel
来源：http://hz.52xcode.cn/gtffrmsygq.html

[U38] Py：获取脚本所在目录
来源：http://hz.havefunace.top/gtbcvjhref.html

Path(__file__).resolve().parent
来源：http://hz.ppjwa.cn/gtogtqrypl.html

[U39] Py：判断是否在交互环境
来源：http://hz.gzhubu.top/gtrljxjkbr.html

sys.stdout.isatty()
来源：http://hz.yuanzhike.top/gtoyynmbwf.html

[U40] Py：打印到标准错误
来源：http://hz.haohaochexian.top/gtrrjxzpuh.html

print("err", file=sys.stderr)
来源：http://hz.jinqigfzy.top/gtlzascqdg.html

[U41] PHP：初始化 Composer 项目
来源：http://hz.shangyingyoupin.top/gtwkobboab.html

composer init;  composer require guzzlehttp/guzzle
来源：http://hz.xuetiantiany.cn/gttyfgeror.html

[U42] PHP：PSR-4 自动加载
来源：http://hz.zhongyouzk.top/gtveuojrcd.html

"autoload": { "psr-4": { "App\\": "src/" } }
来源：http://hz.cheryme.top/gttdyimgyu.html

[U43] PHP：声明命名空间
来源：http://hz.zhiwuduotai.top/gtplljzokh.html

namespace App\Http;
来源：http://hz.snrcjt.cn/gthbcviryi.html

[U44] PHP：开启严格类型
来源：http://hz.sxryk.cn/gtxmgeumzo.html

declare(strict_types=1);
来源：http://hz.tianlin.xyz/gtjikpsnfc.html

[U45] PHP：类型声明与返回类型
来源：http://hz.jinyuanbaomall.cn/gtnsuniurx.html

function add(int $a, int $b): int { return $a + $b; }
来源：http://hz.yongpay.top/gtrehimttd.html

[U46] PHP：可空类型
来源：http://hz.snrcjt.cn/gtyhkrsoor.html

?string $name = null
来源：http://hz.tian-w.cn/gtczpaydzx.html

[U47] PHP：联合类型
来源：http://hz.yuanzhike.top/gtxvatlium.html

int|string $id
来源：http://hz.jiagoushi.top/gtfuuasyxo.html

[U48] PHP：纯枚举
来源：http://hz.jinqigfzy.top/gttbfkddgy.html

enum Status: string { case Active = "active"; case Off = "off"; }
来源：http://hz.jianghu66.top/gtzfyxsfbb.html

[U49] PHP：只读属性
来源：http://hz.ywan-chungtsiang.top/gtwdvzjhvz.html

public readonly string $name
来源：http://hz.shzxlz.cn/gtytecdrpl.html

[U50] PHP：构造器属性提升
来源：http://hz.jqgufenzy.top/gttvbwgjwi.html

public function __construct(private int $id) {}
来源：http://hz.hywenlv.cn/gtimfszedt.html

[U51] PHP：数组解构
来源：http://hz.kuanghao11.cn/gtlfvmnvjj.html

[$a, $b] = $arr;
来源：http://hz.52xcode.cn/gtidvepzee.html

[U52] PHP：箭头函数
来源：http://hz.9152youxi.cn/gtuuklpvmy.html

$double = fn($x) => $x * 2;
来源：http://hz.yj20258.top/gtjngucidn.html


<!-- 参考信息 -->