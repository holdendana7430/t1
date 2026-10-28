代发 wailian999

#ifndef X_H
来源：http://hz.ehwqpu.com/gthkvyhpkv.html

#define X_H
来源：http://hz.chenzaomai.com/gtztptfbvy.html

#endif
来源：http://hz.shangyingyoupin.top/gtqhthwofm.html

[S31] C++：Hello World
来源：http://hz.hfpthk.cn/gtiwcxcatb.html

#include <iostream>
来源：http://hz.ydjk.org.cn/gtjrpgfokq.html

int main() { std::cout << "Hello\n"; }
来源：http://hz.dashuyun.cn/gtxnwluwfh.html

[S32] C++：字符串
来源：http://hz.aizwys.cn/gtbbvxnhzc.html

std::string s = "hi";  s += "!";
来源：http://hz.andypj.xyz/gtffooljqw.html

[S33] C++：vector 增删
来源：http://hz.tianlin.xyz/gtaylcbdez.html

std::vector<int> v{1, 2, 3};  v.push_back(4);
来源：http://hz.shzxlz.cn/gtaxtljovc.html

[S34] C++：遍历 vector
来源：http://hz.svipenyu.cn/gtfspwawfy.html

for (auto &x : v) { std::cout << x; }
来源：http://hz.zhengqikj.top/gtejyotyan.html

[S35] C++：map
来源：http://hz.ybcxt.top/gtxyjhotdj.html

std::map<std::string, int> m;  m["a"] = 1;
来源：http://hz.xylfe.cn/gtlhzrjeib.html

[S36] C++：unordered_map
来源：http://hz.yj20258.top/gtidkiuuii.html

std::unordered_map<std::string, int> m;  m["a"] = 1;
来源：http://hz.jqgfzy.top/gtjfbvejgg.html

[S37] C++：set
来源：http://hz.sweek.top/gtolflpbfk.html

std::set<int> s{1, 2, 3};  s.insert(4);
来源：http://hz.feifeiyinyue.top/gtjbovamfh.html

[S38] C++：排序
来源：http://hz.gzhubu.top/gtrpbvcqst.html

std::sort(v.begin(), v.end());
来源：http://hz.iojbl.cn/gtgplbwgcj.html

[S39] C++：自定义比较器排序
来源：http://hz.shzxlz.cn/gtgkpwajlu.html

std::sort(v.begin(), v.end(), [](int a, int b) { return a > b; });
来源：http://hz.andypj.xyz/gtkhmomrsd.html

[S40] C++：查找元素
来源：http://hz.52xcode.cn/gtznctwsja.html

auto it = std::find(v.begin(), v.end(), 3);
来源：http://hz.hammf.cn/gtiufgtxkr.html

[S41] C++：类与构造函数
来源：http://hz.smart0.xyz/gtbdaxnlkk.html

class A { public: A(int v) : x_(v) {} int get() const { return x_; } private: int x_; };
来源：http://hz.cashguo.top/gtweubgsyz.html

[S42] C++：继承与虚函数
来源：http://hz.bjfxy.top/gtqybdmyzy.html

class B : public Base { public: void f() override {} };
来源：http://hz.pycfn.com/gtwayoxfko.html

[S43] C++：智能指针
来源：http://hz.daxiang520.top/gtwqelnrqg.html

auto p = std::make_unique<int>(5);
来源：http://hz.jianghu66.top/gtwoenaxju.html

[S44] C++：引用传参
来源：http://hz.zhiwuduotai.top/gtxpmtbcqz.html

void inc(int &x) { ++x; }
来源：http://hz.zhoulong.xyz/gtskgseruk.html

[S45] C++：lambda
来源：http://hz.zdqjudy.top/gtouopvqdw.html

auto add = [](int a, int b) { return a + b; };
来源：http://hz.shanyushiyangkeji.top/gtixvchwtm.html

[S46] C++：函数模板
来源：http://hz.mhx1999.top/gtjtnkwxdp.html

template <typename T> T maxv(T a, T b) { return a > b ? a : b; }
来源：http://hz.snrcjt.cn/gtdfmxamou.html

[S47] C++：结构化绑定遍历
来源：http://hz.yonumen.top/gtmfhgcpbj.html

for (const auto &[k, v] : m) { std::cout << k << v; }
来源：http://hz.fzhhl.top/gtvbwobwva.html

[S48] C++：逐行读文件
来源：http://hz.shangyingyoupin.top/gtrudwncug.html

std::ifstream in("a.txt");  std::string line;
来源：http://hz.yuxming.cn/gtymanvbtz.html

while (std::getline(in, line)) { }
来源：http://hz.fzhhl.top/gtgceqxbtc.html

[S49] C++：写文件
来源：http://hz.jlsjyb.cn/gtkekpwefr.html

std::ofstream out("a.txt");  out << "hi\n";
来源：http://hz.fzhhl.top/gtlwiowfvo.html

[S50] C++：格式化数字
来源：http://hz.yj202588.top/gtsztohenz.html

std::ostringstream os;  os << std::fixed << std::setprecision(2) << 3.14159;
来源：http://hz.xuanzx.com/gtebdeqrrj.html

[S51] C++：显式类型转换
来源：http://hz.yuanzhike.top/gtfztgqwpg.html

static_cast<double>(a) / b
来源：http://hz.nwbrower.top/gtcdisrvua.html

[S52] C++：const 与 noexcept
来源：http://hz.ydzc1.top/gtjexzdxnv.html

int size() const noexcept { return n_; }
来源：http://hz.feifeiyinyue.top/gtafyrnbsp.html

[S53] C++：移动语义
来源：http://hz.aibaodan.cn/gtvzkiqepm.html

std::vector<int> w = std::move(v);
来源：http://hz.chenzaomai.com/gtvlzbsrmo.html

[S54] C++：异常处理
来源：http://hz.yangfankeji.com/gtyupbzqtd.html

try { throw std::runtime_error("x"); } catch (const std::exception &e) { }
来源：http://hz.52xcode.cn/gtypfayrod.html

[S55] C++：结构化绑定
来源：http://hz.guannengcc.top/gtxtoglczx.html

auto [a, b] = std::make_pair(1, 2);
来源：http://hz.wangshuangyany.cn/gtcbhrbapg.html

[S56] C++：optional
来源：http://hz.gaohongyu789.top/gtltvttmuo.html

std::optional<int> o = 5;  if (o) { int v = *o; }
来源：http://hz.yuxming.cn/gtycmeugnk.html

[S57] C++：编译期常量
来源：http://hz.xuanzx.com/gtvqjlxlaq.html

constexpr int N = 10;
来源：http://hz.bjfxy.top/gtqrkdpmah.html

[S58] C++：命名空间
来源：http://hz.ywan-chungtsiang.top/gtxuyatprg.html

namespace ns { int f() { return 1; } }
来源：http://hz.zdqjudy.top/gtbqhnoocu.html

[S59] C++：静态断言
来源：http://hz.iojbl.cn/gtcxibcgob.html

static_assert(sizeof(int) == 4, "int 必须 4 字节");
来源：http://hz.meibo888.top/gtawsmjuyj.html

[S60] C++：遍历并删除元素
来源：http://hz.zhoulong.xyz/gtsbwubprr.html

v.erase(std::remove_if(v.begin(), v.end(), [](int x) { return x < 0; }), v.end());
来源：http://hz.ehwqpu.com/gtdlgbprqg.html

================================================================================
来源：http://hz.dianchejie.cn/gtaxndxntx.html

T. 其他语言补充（Kotlin / Swift / Lua / Perl / Scala）
来源：http://hz.fzhhl.top/gtrqdxrjwa.html

================================================================================
来源：http://hz.chenzaomai.com/gtmkntuggy.html

[T01] Kotlin：Hello World
来源：http://hz.yj202588.top/gtcdxadhpk.html

println("Hello")
来源：http://hz.meibo888.top/gtlyayifwf.html

[T02] Kotlin：变量
来源：http://hz.cheryme.top/gtcmgxhltw.html

val a = 1;  var b = 2        // val 只读，var 可变
来源：http://hz.zhengqikj.top/gtmfcwcbbe.html

[T03] Kotlin：字符串模板
来源：http://hz.hfpthk.cn/gtfaytmncd.html

"值: $b"
来源：http://hz.zhiwuduotai.top/gtzbcdrbdo.html

[T04] Kotlin：空安全
来源：http://hz.0kj1m.cn/gtoqmhnlzt.html

val n: String? = null;  n?.length
来源：http://hz.xuetiantiany.cn/gtfrgxwxpc.html

[T05] Kotlin：when 表达式
来源：http://hz.meibo888.top/gttagwzzlg.html

val s = when (x) { 1 -> "一" else -> "其他" }   // 多分支时每个分支单独一行
来源：http://hz.fengsongda.top/gtaodxioea.html

[T06] Kotlin：集合映射
来源：http://hz.birdmap.top/gtughlwymi.html

listOf(1, 2, 3).map { it * 2 }
来源：http://hz.cqqwz.cn/gtqnvhzeai.html

[T07] Kotlin：集合过滤
来源：http://hz.aibaodan.cn/gtzydxgmmv.html

listOf(1, 2, 3).filter { it > 1 }
来源：http://hz.xinyue.icu/gtsokwdopf.html

[T08] Kotlin：数据类
来源：http://hz.jianghu66.top/gtfjffgsfv.html

data class User(val name: String, val age: Int)
来源：http://hz.hammf.cn/gtylilxehv.html

[T09] Kotlin：扩展函数
来源：http://hz.hnqzz.top/gtmcsuftlt.html

fun String.exclaim() = this + "!"
来源：http://hz.quarkkingdee.top/gtrfoysvwt.html

[T10] Kotlin：默认参数
来源：http://hz.guannengcc.top/gttcqsjjov.html

fun greet(name: String = "World") = "Hi $name"
来源：http://hz.dashuyun.cn/gtyfeyxzxu.html

[T11] Kotlin：协程
来源：http://hz.jianghu66.top/gtpgzaggpd.html

GlobalScope.launch { delay(1000); println("done") }
来源：http://hz.jinqigufen.top/gtmxlawhlb.html

[T12] Kotlin：解构声明
来源：http://hz.pengpengdd.cyou/gthqlezvjo.html

val (a, b) = Pair(1, 2)
来源：http://hz.52xcode.cn/gtciuzacgq.html

[T13] Kotlin：只读 Map
来源：http://hz.sufxvd.cn/gtynsacaie.html

val m = mapOf("a" to 1)
来源：http://hz.dianchejie.cn/gtnqqnrmxt.html

[T14] Kotlin：循环
来源：http://hz.wangshuangyany.cn/gtyknovume.html

for (i in 1..10) println(i)
来源：http://hz.fzhhl.top/gtmbgphdoc.html

[T15] Kotlin：接口
来源：http://hz.dashuyun.cn/gtwctlirlo.html

interface Shape { fun area(): Double }
来源：http://hz.jlsjyb.cn/gttkpigqop.html

[T16] Swift：Hello World
来源：http://hz.sysykeji.top/gtcmxfxhai.html

print("Hello")
来源：http://hz.andypj.xyz/gtxfsltopj.html

[T17] Swift：变量与常量
来源：http://hz.zhiwuduotai.top/gtcizjyxeu.html

var a = 1;  let b = 2
来源：http://hz.shanyushiyangtech.top/gtrrrihxdt.html

[T18] Swift：字符串插值
来源：http://hz.jiagoushi.top/gtehvekbrz.html

"值: \(b)"
来源：http://hz.tanke756.top/gtgjnsiuka.html

[T19] Swift：可选绑定
来源：http://hz.xuanzx.com/gtdqjoubxm.html

if let n = opt { print(n) }
来源：http://hz.yj202588.top/gtxtwxrjau.html

[T20] Swift：数组操作
来源：http://hz.ydzc1.top/gtaospanmk.html

var a = [1, 2, 3];  a.append(4)
来源：http://hz.yj202588.top/gtzohxalnn.html

[T21] Swift：遍历
来源：http://hz.cqqwz.cn/gttxaqoodd.html

for x in a { print(x) }
来源：http://hz.zdqjudy.top/gtzwbobaku.html

[T22] Swift：字典
来源：http://hz.pengpengdd.cyou/gtsgbehmxq.html

var d = ["a": 1];  d["b"] = 2
来源：http://hz.shanyushiyangkeji.top/gtrqllbyxm.html

[T23] Swift：函数
来源：http://hz.meibo888.top/gtjytwcjbn.html

func add(_ a: Int, _ b: Int) -> Int { a + b }
来源：http://hz.sweek.top/gtfwmwnhll.html

[T24] Swift：闭包
来源：http://hz.jinqigufen.top/gtildgvaws.html

let f = { (x: Int) -> Int in x * 2 }
来源：http://hz.sysykeji.top/gtmpxonfvq.html

[T25] Swift：结构体
来源：http://hz.yongpay.top/gtmygekvqo.html

struct P { var x: Int }
来源：http://hz.jiagoushi.top/gtfwihaofs.html

[T26] Swift：类与重写
来源：http://hz.pycfn.com/gtsqoscrkn.html

class A: Base { override func f() {} }
来源：http://hz.shanyushiyangkeji.top/gtdqwpyooq.html

[T27] Swift：错误处理
来源：http://hz.ivvv.top/gthutauszt.html

do { try f() } catch { print(error) }
来源：http://hz.nanxuanxn.top/gtetmhsgci.html

[T28] Swift：枚举
来源：http://hz.svipenyu.cn/gtjwdjqeeh.html

enum Color { case red, green }
来源：http://hz.xuanzx.com/gtbwaoonfi.html

[T29] Swift：guard 提前返回
来源：http://hz.ydzc1.top/gtzwockitf.html

guard let x = opt else { return }
来源：http://hz.zhaomingkeji.xyz/gtscrggukt.html

[T30] Swift：协议
来源：http://hz.yj202588.top/gtynfdcxde.html

protocol Shape { func area() -> Double }
来源：http://hz.jqgufenzy.top/gtbyikmnwv.html

[T31] Lua：Hello World
来源：http://hz.ydzc1.top/gtfxingqie.html

print("Hello")
来源：http://hz.yueranfly.top/gtrioijamu.html

[T32] Lua：局部变量
来源：http://hz.zhixingplan.top/gtpttbhmlb.html

local a = 1
来源：http://hz.hammf.cn/gtylfrdboq.html

[T33] Lua：表（数组）
来源：http://hz.jlsjyb.cn/gtfoffkxiq.html

local t = {1, 2, 3};  t[4] = 4
来源：http://hz.sysykeji.top/gtwozadqkm.html

[T34] Lua：遍历表
来源：http://hz.ehwqpu.com/gtoupyzljj.html

for i, v in ipairs(t) do print(i, v) end
来源：http://hz.kuanghao11.cn/gthmibrunt.html

[T35] Lua：字典表
来源：http://hz.chenjidiqi.icu/gtomrtcywh.html

local d = { a = 1 };  d.b = 2
来源：http://hz.sufxvd.cn/gtkxidvmdj.html

[T36] Lua：函数
来源：http://hz.ehwqpu.com/gtestqeerw.html

function add(a, b) return a + b end
来源：http://hz.xingfuxueyuan.xyz/gtbyqyvyji.html

[T37] Lua：字符串拼接
来源：http://hz.andypj.xyz/gtfrockqlg.html

"a" .. "b"
来源：http://hz.hywenlv.cn/gtpeljoncd.html

[T38] Lua：条件
来源：http://hz.hongshengwenyu.top/gtopbgqeis.html

if x > 0 then print("正") end
来源：http://hz.jiagoushi.top/gtkvqrpgso.html

[T39] Lua：模式匹配
来源：http://hz.jiagoushi.top/gtourrawyi.html

string.find(s, "%d+")
来源：http://hz.snrcjt.cn/gthfmhtlnq.html

[T40] Lua：元表
来源：http://hz.gogol.net.cn/gtxinppity.html

setmetatable({}, { __index = base })
来源：http://hz.jinqigufen.top/gtgixinzdn.html

[T41] Perl：Hello World
来源：http://hz.yj20258.top/gtwfartmmc.html

print "Hello\n";
来源：http://hz.cashguo.top/gtfnofgbyo.html

[T42] Perl：变量类型
来源：http://hz.zdqjudy.top/gtusazuvog.html

my $a = 1;  my @arr = (1, 2, 3);  my %h = (a => 1);
来源：http://hz.guowangkeji.top/gtbrtpscuh.html

[T43] Perl：字符串插值
来源：http://hz.ywan-chungtsiang.top/gtgftjnvqh.html

"值: $a"
来源：http://hz.zhiwuduotai.top/gtpxyxsfoq.html

[T44] Perl：条件
来源：http://hz.wangshuangyany.cn/gtzalsfagy.html

if ($a > 0) { print "正"; }
来源：http://hz.chenjidiqi.icu/gtzlzmubge.html

[T45] Perl：数组遍历
来源：http://hz.ydjk.org.cn/gthuzzrexj.html

for my $x (@arr) { print $x; }
来源：http://hz.jlsjyb.cn/gtkakstqah.html

[T46] Perl：哈希操作
来源：http://hz.shanyushiyangkeji.top/gtuwiqcecs.html

$h{b} = 2;  for my $k (keys %h) { print "$k=$h{$k}"; }
来源：http://hz.bjfxy.top/gtblswlemr.html

[T47] Perl：正则捕获
来源：http://hz.chenlongwang.top/gtdgzomewp.html

if ($s =~ /(\d+)/) { print $1; }
来源：http://hz.nanxinkj.top/gtjyyzqpyv.html

[T48] Perl：正则替换
来源：http://hz.aibaodan.cn/gtvpkbjmdo.html

$s =~ s/old/new/g;
来源：http://hz.nwbrower.top/gtjgwjumev.html

[T49] Perl：函数
来源：http://hz.pengpengdd.cyou/gtcwuhajce.html

sub add { my ($a, $b) = @_; return $a + $b; }
来源：http://hz.ivvv.top/gtbxgkinzk.html

[T50] Perl：逐行读文件
来源：http://hz.aibaodan.cn/gtnurnkuxd.html

open my $fh, "<", "a.txt" or die $!;
来源：http://hz.yj20258.top/gtrjizgbjx.html

while (my $line = <$fh>) { print $line; }
来源：http://hz.jianghu66.top/gtzwiobffw.html

[T51] Scala：Hello World
来源：http://hz.316326.xyz/gtdxipwoaa.html

println("Hello")
来源：http://hz.pycfn.com/gtwwjdjddx.html

[T52] Scala：变量
来源：http://hz.zdqjudy.top/gtkmhzenqq.html

val a = 1;  var b = 2
来源：http://hz.aibaodan.cn/gtabdfnvyq.html

[T53] Scala：字符串插值
来源：http://hz.sweek.top/gtkamsirzk.html

s"值: $b"
来源：http://hz.nwbrower.top/gtxppspdqv.html

[T54] Scala：集合映射
来源：http://hz.xinyue.icu/gtljwlbqdg.html

List(1, 2, 3).map(_ * 2)
来源：http://hz.guannengcc.top/gthuzzmzgs.html

[T55] Scala：集合过滤
来源：http://hz.jiagoushi.top/gtwnavulfi.html

List(1, 2, 3).filter(_ > 1)
来源：http://hz.svipenyu.cn/gtupfitrav.html

[T56] Scala：样例类
来源：http://hz.xylfe.cn/gtvstwvsqd.html

case class User(name: String, age: Int)
来源：http://hz.chenjidiqi.icu/gtlkmshgah.html

[T57] Scala：模式匹配
来源：http://hz.andypj.xyz/gtcxhtbifp.html

x match { case 1 => "一"; case _ => "其他" }
来源：http://hz.zhijiandao.cn/gtlisauuhs.html

[T58] Scala：函数定义
来源：http://hz.ydjk.org.cn/gteselaxng.html

def add(a: Int, b: Int): Int = a + b
来源：http://hz.yj20258888.top/gtpqmzirvu.html

[T59] Scala：循环
来源：http://hz.quarkkingdee.top/gtyketuwdi.html

for (i <- 1 to 10) println(i)
来源：http://hz.gzhubu.top/gtgwzzorsv.html

[T60] Scala：折叠
来源：http://hz.hnxiangtu.top/gthiarjfws.html

List(1, 2, 3).foldLeft(0)(_ + _)
来源：http://hz.chenzaomai.com/gtsiqruejc.html

================================================================================
来源：http://hz.yvedp.cn/gtjiqqppsn.html

U. 高频实用片段（Python / PHP / JavaScript 各 40 条）
来源：http://hz.ydjk.org.cn/gtihrsafig.html

================================================================================
来源：http://hz.yvedp.cn/gtbtletqzr.html

[U01] Py：创建虚拟环境
来源：http://hz.yongpay.top/gtsgqajyct.html

python -m venv .venv && source .venv/bin/activate
来源：http://hz.zdqjudy.top/gtkqhmfrsc.html

[U02] Py：导出 / 安装依赖
来源：http://hz.kuanghao11.cn/gtnyjnalcs.html

pip freeze > requirements.txt;  pip install -r requirements.txt
来源：http://hz.jinqigufen.top/gtwrwenxkt.html

[U03] Py：加载 .env 配置
来源：http://hz.jlsjyb.cn/gtswqxheiq.html

from dotenv import load_dotenv; load_dotenv()
来源：http://hz.fzhhl.top/gthmmuzbco.html

[U04] Py：变量调试打印
来源：http://hz.wangshuangyany.cn/gtfqlsykvz.html

print(f"{x=}")            # 输出 x=值，Python 3.8+
来源：http://hz.feifeiyinyue.top/gtrafntgrq.html

[U05] Py：列表去重且保序
来源：http://hz.cqqwz.cn/gtsuxhkzme.html

list(dict.fromkeys(arr))
来源：http://hz.zhixingplan.top/gtchsnanex.html

[U06] Py：合并两个字典
来源：http://hz.kuanghao11.cn/gtiojvebcm.html

{**a, **b}
来源：http://hz.quarkkingdee.top/gtsllulpdq.html

[U07] Py：反转字典键值
来源：http://hz.ywan-chungtsiang.top/gtnvklvnwo.html

{v: k for k, v in d.items()}
来源：http://hz.tanke756.top/gttoiydcxr.html

[U08] Py：展平二维列表
来源：http://hz.chenlongwang.top/gtvxuaikom.html

[y for x in nested for y in x]
来源：http://hz.gogol.net.cn/gtgabdgyqe.html

[U09] Py：字典取最大值的键
来源：http://hz.jlsjyb.cn/gtfnhvmkkc.html

max(d, key=d.get)
来源：http://hz.nanxinkj.top/gtqqrbyyys.html

[U10] Py：按值排序字典
来源：http://hz.wangdashe.top/gtctksymoa.html

dict(sorted(d.items(), key=lambda kv: kv[1]))
来源：http://hz.xuetiantiany.cn/gtschzgmri.html

[U11] Py：生成器表达式
来源：http://hz.guannengcc.top/gtnzistjjo.html

(x * 2 for x in arr)
来源：http://hz.sufxvd.cn/gtfcofakhb.html

[U12] Py：取出现最多的 3 个元素
来源：http://hz.hysaishi.cn/gterftrcbw.html

Counter(arr).most_common(3)
来源：http://hz.cqqwz.cn/gtiuslowwh.html

[U13] Py：固定长度队列
来源：http://hz.gzhubu.top/gtdvmaualz.html

deque(maxlen=10)
来源：http://hz.daxiang520.top/gtbaoylrhc.html

[U14] Py：分组收集到列表
来源：http://hz.shanyushiyangkeji.top/gtylymzqpc.html

defaultdict(list)
来源：http://hz.zhoulong.xyz/gtvdnuqxtz.html

[U15] Py：高精度计时
来源：http://hz.kuanghao11.cn/gtirtfqvet.html

t = time.perf_counter()
来源：http://hz.dianchejie.cn/gtkhmwndxf.html

[U16] Py：命令行参数解析
来源：http://hz.iojbl.cn/gtijhfmxnc.html

ap = argparse.ArgumentParser();  ap.add_argument("--name");  args = ap.parse_args()
来源：http://hz.shzxlz.cn/gtksjitedi.html

[U17] Py：初始化日志
来源：http://hz.wangshuangyany.cn/gtuanvdqjx.html

logging.basicConfig(level=logging.INFO)
来源：http://hz.shanyushiyangtech.top/gtyegmopah.html

[U18] Py：预编译正则
来源：http://hz.cqqwz.cn/gtxqelwgsw.html

pat = re.compile(r"\d+")
来源：http://hz.hammf.cn/gtohtcwmij.html

[U19] Py：正则替换带回调
来源：http://hz.xuanzx.com/gtwxjmqvbf.html

re.sub(r"\d+", lambda m: str(int(m.group()) * 2), s)
来源：http://hz.dashuyun.cn/gtsqjkyrvd.html

[U20] Py：缓存函数结果
来源：http://hz.snrcjt.cn/gtdalpvvjp.html

@functools.lru_cache(maxsize=None)
来源：http://hz.ybcxt.top/gtqaexurpy.html

[U21] Py：自定义上下文管理器
来源：http://hz.c1oappe.top/gthxpmxjcz.html

@contextlib.contextmanager
来源：http://hz.wangshuangyany.cn/gtqcgzyulb.html

[U22] Py：矩阵转置
来源：http://hz.jinqigfzy.top/gtjyhyazln.html

list(zip(*m))
来源：http://hz.ywan-chungtsiang.top/gtoejwufhw.html

[U23] Py：分块读取大文件
来源：http://hz.yueranfly.top/gtwkdiiaxo.html

for chunk in iter(lambda: f.read(8192), b""):
来源：http://hz.yonumen.top/gtphqeeylu.html

[U24] Py：路径操作
来源：http://hz.ywan-chungtsiang.top/gtudprdbti.html

Path("a/b.txt").parent.mkdir(parents=True, exist_ok=True)
来源：http://hz.xinyue.icu/gtmklwupci.html

[U25] Py：CSV 按字典读
来源：http://hz.yvedp.cn/gtuccztlid.html

csv.DictReader(f)
来源：http://hz.yvedp.cn/gtmpbqjczs.html

[U26] Py：并发下载
来源：http://hz.hnxiangtu.top/gtkvblkktp.html

ThreadPoolExecutor(max_workers=8).map(fetch, urls)
来源：http://hz.jqgfzy.top/gtcmcvgoqr.html

[U27] Py：异步 HTTP
来源：http://hz.ivvv.top/gtybeuisjg.html

aiohttp.ClientSession() 配合 async with
来源：http://hz.hnqzz.top/gtvmjnmmnj.html

[U28] Py：类型别名
来源：http://hz.zhiwuduotai.top/gttppntxqc.html

UserId = int
来源：http://hz.hysaishi.cn/gtidlzrmns.html

[U29] Py：属性校验
来源：http://hz.hnxiangtu.top/gtzoblilnl.html

@property 与 @x.setter 配合
来源：http://hz.xuetiantiany.cn/gtkjyvymlg.html

[U30] Py：数据类
来源：http://hz.quarkkingdee.top/gtskadgdis.html

@dataclass(slots=True)
来源：http://hz.nanxuanxn.top/gtkvyzhtmg.html

[U31] Py：单测
来源：http://hz.sufxvd.cn/gtihnlnuqc.html

python -m pytest -q
来源：http://hz.ydjk.org.cn/gtnndoarzl.html

[U32] Py：代码格式化
来源：http://hz.shuidangran.top/gtrsplvwis.html

ruff format . && ruff check --fix .
来源：http://hz.feifeiyinyue.top/gtyeceucsi.html

[U33] Py：打包发布
来源：http://hz.yuxming.cn/gtuuewpqlu.html

python -m build  （依赖 pyproject.toml）
来源：http://hz.zhongyouzk.top/gtdxbhybdl.html

[U34] Py：判断编码
来源：http://hz.jyoumei.cn/gtvqndlshb.html

chardet.detect(raw)
来源：http://hz.wangshuangyany.cn/gtsybmcuul.html

[U35] Py：发送邮件
来源：http://hz.jinqigfzy.top/gtrafcwkrw.html

smtplib.SMTP_SSL(...).send_message(msg)
来源：http://hz.cashguo.top/gtqrwdozhd.html

[U36] Py：定时任务
来源：http://hz.zhongyouzk.top/gtbvogwyhh.html

schedule.every(10).minutes.do(job)
来源：http://hz.jqgfzy.top/gtggfuziol.html

[U37] Py：读写 Excel
来源：http://hz.yueranfly.top/gtrlzfdtim.html

pandas.read_excel / DataFrame.to_excel
来源：http://hz.shzxlz.cn/gtbzpeewqg.html

[U38] Py：获取脚本所在目录
来源：http://hz.ehwqpu.com/gtilqfhpzn.html

Path(__file__).resolve().parent
来源：http://hz.chenlongwang.top/gtqwdxqygs.html

[U39] Py：判断是否在交互环境
来源：http://hz.hnqzz.top/gtqvtghszj.html

sys.stdout.isatty()
来源：http://hz.cashguo.top/gtjneyctjw.html

[U40] Py：打印到标准错误
来源：http://hz.cdnleiting.top/gtdplifbre.html

print("err", file=sys.stderr)
来源：http://hz.feifeiyinyue.top/gtpdafimdw.html

[U41] PHP：初始化 Composer 项目
来源：http://hz.9152youxi.cn/gtggnnwlqz.html

composer init;  composer require guzzlehttp/guzzle
来源：http://hz.hammf.cn/gtvkuuxkkl.html

[U42] PHP：PSR-4 自动加载
来源：http://hz.quarkkingdee.top/gtwxhbaxhs.html

"autoload": { "psr-4": { "App\\": "src/" } }
来源：http://hz.shzxlz.cn/gtbckilqfw.html

[U43] PHP：声明命名空间
来源：http://hz.svipenyu.cn/gtzcwitvpv.html

namespace App\Http;
来源：http://hz.andypj.xyz/gtoaldrekg.html

[U44] PHP：开启严格类型
来源：http://hz.yonumen.top/gtkxreulhu.html

declare(strict_types=1);
来源：http://hz.sysykeji.top/gtukdtdrym.html

[U45] PHP：类型声明与返回类型
来源：http://hz.jiagoushi.top/gtllkjpgjm.html

function add(int $a, int $b): int { return $a + $b; }
来源：http://hz.zhiwuduotai.top/gtqxaoktbt.html

[U46] PHP：可空类型
来源：http://hz.shanyushiyangtech.top/gtwkfgnwfh.html

?string $name = null
来源：http://hz.shanyushiyangtech.top/gtyqjydhfz.html

[U47] PHP：联合类型
来源：http://hz.gotoacloud.top/gtonaclswo.html

int|string $id
来源：http://hz.hnxiangtu.top/gttkwbplkx.html

[U48] PHP：纯枚举
来源：http://hz.jqgufenzy.top/gtejnfywpz.html

enum Status: string { case Active = "active"; case Off = "off"; }
来源：http://hz.yangfankeji.com/gtukysdmpa.html

[U49] PHP：只读属性
来源：http://hz.xylfe.cn/gtqrisdrsx.html

public readonly string $name
来源：http://hz.cheryme.top/gtgpfhtcfq.html

[U50] PHP：构造器属性提升
来源：http://hz.guowangkeji.top/gthqoonuwp.html

public function __construct(private int $id) {}
来源：http://hz.smart0.xyz/gtuxbuyaoj.html

[U51] PHP：数组解构
来源：http://hz.zhixingplan.top/gtxgbznvyc.html

[$a, $b] = $arr;
来源：http://hz.tanke756.top/gteljvwrkz.html

[U52] PHP：箭头函数
来源：http://hz.sufxvd.cn/gtnxplqttx.html

$double = fn($x) => $x * 2;
来源：http://hz.ehwqpu.com/gtlbhvdtoo.html

[U53] PHP：空合并运算符
来源：http://hz.shanyushiyangtech.top/gtmisumqch.html

$v = $a ?? $b ?? "default";
来源：http://hz.shuidangran.top/gtygnjcute.html

[U54] PHP：空安全调用
来源：http://hz.tian-w.cn/gtfzjznmcb.html

$obj?->method()
来源：http://hz.hysaishi.cn/gtpmrpzuvz.html


<!-- 参考信息 -->