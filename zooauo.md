代发 wailian999

memset(a, 0, sizeof a);
来源：http://hz.yongpay.top/gtujqhisvu.html

[S27] C：定义常量
来源：http://hz.meibo888.top/gtbkzryvkz.html

const double PI = 3.14159;
来源：http://hz.zhixingplan.top/gtxxsyvdyl.html

[S28] C：静态变量
来源：http://hz.cqqwz.cn/gtgbdowbcf.html

static int counter = 0;
来源：http://hz.ehwqpu.com/gtcvcsemms.html

[S29] C：变参函数
来源：http://hz.yueranfly.top/gtsksycoyt.html

va_list ap; va_start(ap, fmt); vprintf(fmt, ap); va_end(ap);
来源：http://hz.hnqzz.top/gtbjniskwe.html

[S30] C：头文件保护
来源：http://hz.feifeiyinyue.top/gtshmgsruy.html

#ifndef X_H
来源：http://hz.shuidangran.top/gtzgxfvrqp.html

#define X_H
来源：http://hz.tanke756.top/gtloppzrat.html

#endif
来源：http://hz.pengpengdd.cyou/gtltfgflqf.html

[S31] C++：Hello World
来源：http://hz.chenjidiqi.icu/gtzlwdsxxr.html

#include <iostream>
来源：http://hz.zhoulong.xyz/gttclkspvv.html

int main() { std::cout << "Hello\n"; }
来源：http://hz.guannengcc.top/gtqeorzjvi.html

[S32] C++：字符串
来源：http://hz.xuanzx.com/gtooxuunzv.html

std::string s = "hi";  s += "!";
来源：http://hz.quarkkingdee.top/gtznbonjbz.html

[S33] C++：vector 增删
来源：http://hz.yanxiufei.cn/gtnllqehjo.html

std::vector<int> v{1, 2, 3};  v.push_back(4);
来源：http://hz.yuxming.cn/gtwgukikql.html

[S34] C++：遍历 vector
来源：http://hz.c1oappe.top/gtsncprspc.html

for (auto &x : v) { std::cout << x; }
来源：http://hz.mhx1999.top/gtoicfdpsx.html

[S35] C++：map
来源：http://hz.gaohongyu789.top/gtjhqorpkp.html

std::map<std::string, int> m;  m["a"] = 1;
来源：http://hz.yanxiufei.cn/gtbhaympqo.html

[S36] C++：unordered_map
来源：http://hz.hammf.cn/gtupbhworl.html

std::unordered_map<std::string, int> m;  m["a"] = 1;
来源：http://hz.sufxvd.cn/gtperwxmpc.html

[S37] C++：set
来源：http://hz.tian-w.cn/gtntigfguq.html

std::set<int> s{1, 2, 3};  s.insert(4);
来源：http://hz.fengsongda.top/gtscqvdwxv.html

[S38] C++：排序
来源：http://hz.iojbl.cn/gtmwjglsyz.html

std::sort(v.begin(), v.end());
来源：http://hz.yj202588.top/gtksrsmsce.html

[S39] C++：自定义比较器排序
来源：http://hz.sufxvd.cn/gtqyovgyoo.html

std::sort(v.begin(), v.end(), [](int a, int b) { return a > b; });
来源：http://hz.pycfn.com/gtlhjtjhby.html

[S40] C++：查找元素
来源：http://hz.bjfxy.top/gtxqxrzeto.html

auto it = std::find(v.begin(), v.end(), 3);
来源：http://hz.zhoulong.xyz/gtjrnvnlju.html

[S41] C++：类与构造函数
来源：http://hz.c1oappe.top/gtelnuqvgp.html

class A { public: A(int v) : x_(v) {} int get() const { return x_; } private: int x_; };
来源：http://hz.zhiwuduotai.top/gtkkgsxctt.html

[S42] C++：继承与虚函数
来源：http://hz.gaohongyu789.top/gttbxwnysh.html

class B : public Base { public: void f() override {} };
来源：http://hz.316326.xyz/gtolnjlgtz.html

[S43] C++：智能指针
来源：http://hz.yueranfly.top/gtdzosehap.html

auto p = std::make_unique<int>(5);
来源：http://hz.hammf.cn/gtkonfnjnr.html

[S44] C++：引用传参
来源：http://hz.zycfv.cn/gtrtdoeahy.html

void inc(int &x) { ++x; }
来源：http://hz.zdqjudy.top/gtdhltacvy.html

[S45] C++：lambda
来源：http://hz.iojbl.cn/gthrrtjobm.html

auto add = [](int a, int b) { return a + b; };
来源：http://hz.hongshengwenyu.top/gtvqmwkfuy.html

[S46] C++：函数模板
来源：http://hz.fengsongda.top/gtfuxfwkyv.html

template <typename T> T maxv(T a, T b) { return a > b ? a : b; }
来源：http://hz.yj20258.top/gtizbhnhwl.html

[S47] C++：结构化绑定遍历
来源：http://hz.chenjidiqi.icu/gthuboetxk.html

for (const auto &[k, v] : m) { std::cout << k << v; }
来源：http://hz.pengpengdd.cyou/gtezjegjvr.html

[S48] C++：逐行读文件
来源：http://hz.316326.xyz/gtrwtszpqt.html

std::ifstream in("a.txt");  std::string line;
来源：http://hz.shanyushiyangtech.top/gtnjylfqma.html

while (std::getline(in, line)) { }
来源：http://hz.guannengcc.top/gtytvztwib.html

[S49] C++：写文件
来源：http://hz.jinyuanbaomall.cn/gtebjstjtj.html

std::ofstream out("a.txt");  out << "hi\n";
来源：http://hz.havefunace.top/gtkowhzudy.html

[S50] C++：格式化数字
来源：http://hz.redwolf501.top/gtwlcutpue.html

std::ostringstream os;  os << std::fixed << std::setprecision(2) << 3.14159;
来源：http://hz.ydzc1.top/gthhwqvcbz.html

[S51] C++：显式类型转换
来源：http://hz.tian-w.cn/gtfjnmnvbp.html

static_cast<double>(a) / b
来源：http://hz.svipenyu.cn/gtnqxxqidx.html

[S52] C++：const 与 noexcept
来源：http://hz.yangfankeji.com/gtqctxpaeu.html

int size() const noexcept { return n_; }
来源：http://hz.nwbrower.top/gtshxqubxv.html

[S53] C++：移动语义
来源：http://hz.birdmap.top/gtxcydqklt.html

std::vector<int> w = std::move(v);
来源：http://hz.jinyuanbaomall.cn/gtvgxgpeiw.html

[S54] C++：异常处理
来源：http://hz.jqgfzy.top/gtbitzkzvx.html

try { throw std::runtime_error("x"); } catch (const std::exception &e) { }
来源：http://hz.guowangkeji.top/gtrslxgapm.html

[S55] C++：结构化绑定
来源：http://hz.jinqigfzy.top/gtznsjkmrv.html

auto [a, b] = std::make_pair(1, 2);
来源：http://hz.zhoulong.xyz/gtirfrsmmi.html

[S56] C++：optional
来源：http://hz.pycfn.com/gtahavwxiw.html

std::optional<int> o = 5;  if (o) { int v = *o; }
来源：http://hz.pycfn.com/gttwapfhtx.html

[S57] C++：编译期常量
来源：http://hz.bjfxy.top/gtjpdevztx.html

constexpr int N = 10;
来源：http://hz.sweek.top/gtdebvqmhs.html

[S58] C++：命名空间
来源：http://hz.cqqwz.cn/gthlwxgkoy.html

namespace ns { int f() { return 1; } }
来源：http://hz.svipenyu.cn/gtypocfghg.html

[S59] C++：静态断言
来源：http://hz.xylfe.cn/gtuxwgaauh.html

static_assert(sizeof(int) == 4, "int 必须 4 字节");
来源：http://hz.gotoacloud.top/gtqtlylfok.html

[S60] C++：遍历并删除元素
来源：http://hz.jlsjyb.cn/gtpdepcodm.html

v.erase(std::remove_if(v.begin(), v.end(), [](int x) { return x < 0; }), v.end());
来源：http://hz.andypj.xyz/gtvpfozxma.html

================================================================================
来源：http://hz.chenzaomai.com/gtotypnqhx.html

T. 其他语言补充（Kotlin / Swift / Lua / Perl / Scala）
来源：http://hz.xuanzx.com/gtomsmqmst.html

================================================================================
来源：http://hz.zhongyouzk.top/gtrpabsegw.html

[T01] Kotlin：Hello World
来源：http://hz.hongshengwenyu.top/gtwfjlajbj.html

println("Hello")
来源：http://hz.mhx1999.top/gtxxcqnqaw.html

[T02] Kotlin：变量
来源：http://hz.hywenlv.cn/gtbvzcslhe.html

val a = 1;  var b = 2        // val 只读，var 可变
来源：http://hz.nanxuanxn.top/gtkoyprklk.html

[T03] Kotlin：字符串模板
来源：http://hz.fzhhl.top/gtpelruwoh.html

"值: $b"
来源：http://hz.shangyingyoupin.top/gtytcbgogw.html

[T04] Kotlin：空安全
来源：http://hz.andypj.xyz/gtcmwnmgoc.html

val n: String? = null;  n?.length
来源：http://hz.zdqjudy.top/gtxibzkxhe.html

[T05] Kotlin：when 表达式
来源：http://hz.yj20258.top/gtkyiwpgdn.html

val s = when (x) { 1 -> "一" else -> "其他" }   // 多分支时每个分支单独一行
来源：http://hz.smart0.xyz/gtleykqwcx.html

[T06] Kotlin：集合映射
来源：http://hz.meibo888.top/gttbbhepkv.html

listOf(1, 2, 3).map { it * 2 }
来源：http://hz.jiagoushi.top/gtkfffbvje.html

[T07] Kotlin：集合过滤
来源：http://hz.gaohongyu789.top/gtltuhhikl.html

listOf(1, 2, 3).filter { it > 1 }
来源：http://hz.meibo888.top/gthwqoivub.html

[T08] Kotlin：数据类
来源：http://hz.nanxinkj.top/gtkmmgbazd.html

data class User(val name: String, val age: Int)
来源：http://hz.ywan-chungtsiang.top/gtobbntiix.html

[T09] Kotlin：扩展函数
来源：http://hz.jianghu66.top/gthxmudblr.html

fun String.exclaim() = this + "!"
来源：http://hz.zhengqikj.top/gtdtouhvti.html

[T10] Kotlin：默认参数
来源：http://hz.jinyuanbaomall.cn/gtjncpnhal.html

fun greet(name: String = "World") = "Hi $name"
来源：http://hz.cheryme.top/gtiiqviyvu.html

[T11] Kotlin：协程
来源：http://hz.mhx1999.top/gtswxpiycx.html

GlobalScope.launch { delay(1000); println("done") }
来源：http://hz.yueranfly.top/gtzigzvzda.html

[T12] Kotlin：解构声明
来源：http://hz.ydjk.org.cn/gtvttbaejd.html

val (a, b) = Pair(1, 2)
来源：http://hz.birdmap.top/gtsddgebkq.html

[T13] Kotlin：只读 Map
来源：http://hz.ybcxt.top/gtljzwsauq.html

val m = mapOf("a" to 1)
来源：http://hz.shangyingyoupin.top/gtkkgijres.html

[T14] Kotlin：循环
来源：http://hz.tanke756.top/gtxefrzgde.html

for (i in 1..10) println(i)
来源：http://hz.316326.xyz/gtfmxptiod.html

[T15] Kotlin：接口
来源：http://hz.cheryme.top/gtaqebcdms.html

interface Shape { fun area(): Double }
来源：http://hz.0kj1m.cn/gtvtirtsai.html

[T16] Swift：Hello World
来源：http://hz.kuanghao11.cn/gtavkfhewi.html

print("Hello")
来源：http://hz.gzhubu.top/gtbvzrwgeg.html

[T17] Swift：变量与常量
来源：http://hz.yvedp.cn/gtyttxndzr.html

var a = 1;  let b = 2
来源：http://hz.jianghu66.top/gtbbckuakx.html

[T18] Swift：字符串插值
来源：http://hz.jinyuanbaomall.cn/gtyrmbcppa.html

"值: \(b)"
来源：http://hz.jinqigufen.top/gtrzdemnlp.html

[T19] Swift：可选绑定
来源：http://hz.shanyushiyangkeji.top/gthccnobss.html

if let n = opt { print(n) }
来源：http://hz.vqdsnc.cn/gtgkgmrjvd.html

[T20] Swift：数组操作
来源：http://hz.gzhubu.top/gtcefxkprh.html

var a = [1, 2, 3];  a.append(4)
来源：http://hz.zhixingplan.top/gtzvjxavxa.html

[T21] Swift：遍历
来源：http://hz.dashuyun.cn/gtazehirkg.html

for x in a { print(x) }
来源：http://hz.havefunace.top/gterpfmeod.html

[T22] Swift：字典
来源：http://hz.guannengcc.top/gtsalepkwm.html

var d = ["a": 1];  d["b"] = 2
来源：http://hz.daria6918.cn/gtpiamdgnx.html

[T23] Swift：函数
来源：http://hz.jqgfzy.top/gtvotladdr.html

func add(_ a: Int, _ b: Int) -> Int { a + b }
来源：http://hz.yj20258.top/gtdqaavbuo.html

[T24] Swift：闭包
来源：http://hz.shanyushiyangtech.top/gtyrmjeouk.html

let f = { (x: Int) -> Int in x * 2 }
来源：http://hz.gogol.net.cn/gtpdswfdce.html

[T25] Swift：结构体
来源：http://hz.xuanzx.com/gtovrtjqlq.html

struct P { var x: Int }
来源：http://hz.chenzaomai.com/gtjocarnuk.html

[T26] Swift：类与重写
来源：http://hz.cashguo.top/gtdvattoro.html

class A: Base { override func f() {} }
来源：http://hz.guowangkeji.top/gtnkzigisa.html

[T27] Swift：错误处理
来源：http://hz.shangyingyoupin.top/gtpkfgzctg.html

do { try f() } catch { print(error) }
来源：http://hz.cheryme.top/gtmgvsfozl.html

[T28] Swift：枚举
来源：http://hz.jqgufenzy.top/gtitoazggz.html

enum Color { case red, green }
来源：http://hz.yj20258888.top/gtamhxvdwl.html

[T29] Swift：guard 提前返回
来源：http://hz.chenjidiqi.icu/gtbxplrtql.html

guard let x = opt else { return }
来源：http://hz.yongpay.top/gtsdfwtazz.html

[T30] Swift：协议
来源：http://hz.yuanzhike.top/gtoyvncoxm.html

protocol Shape { func area() -> Double }
来源：http://hz.daria6918.cn/gtcudtnmet.html

[T31] Lua：Hello World
来源：http://hz.aizwys.cn/gtzlilywib.html

print("Hello")
来源：http://hz.nwbrower.top/gtaustduiz.html

[T32] Lua：局部变量
来源：http://hz.ydzc1.top/gtqpxhgrnf.html

local a = 1
来源：http://hz.pycfn.com/gtngejxzie.html

[T33] Lua：表（数组）
来源：http://hz.nanxinkj.top/gtwkztqtci.html

local t = {1, 2, 3};  t[4] = 4
来源：http://hz.nanxinkj.top/gtrmzixoap.html

[T34] Lua：遍历表
来源：http://hz.wangdashe.top/gtollpagqb.html

for i, v in ipairs(t) do print(i, v) end
来源：http://hz.pycfn.com/gtjgykfoht.html

[T35] Lua：字典表
来源：http://hz.yj20258.top/gtqprwjdud.html

local d = { a = 1 };  d.b = 2
来源：http://hz.dashuyun.cn/gtgrusitjn.html

[T36] Lua：函数
来源：http://hz.xingfuxueyuan.xyz/gtxuoyknze.html

function add(a, b) return a + b end
来源：http://hz.andypj.xyz/gtzqimmxpm.html

[T37] Lua：字符串拼接
来源：http://hz.nanxuanxn.top/gtnlxdrbrb.html

"a" .. "b"
来源：http://hz.sufxvd.cn/gtfbxiucda.html

[T38] Lua：条件
来源：http://hz.jinqigufen.top/gtyxlxxvot.html

if x > 0 then print("正") end
来源：http://hz.zhixingplan.top/gtxgivyvtg.html

[T39] Lua：模式匹配
来源：http://hz.chenjidiqi.icu/gtmagzzkxe.html

string.find(s, "%d+")
来源：http://hz.nwbrower.top/gtgsyightb.html

[T40] Lua：元表
来源：http://hz.gogol.net.cn/gtjtoijzof.html

setmetatable({}, { __index = base })
来源：http://hz.yj20258888.top/gtiyczzexc.html

[T41] Perl：Hello World
来源：http://hz.ehwqpu.com/gtbwswfzrj.html

print "Hello\n";
来源：http://hz.sweek.top/gtbunxshnr.html

[T42] Perl：变量类型
来源：http://hz.52xcode.cn/gtmicicpco.html

my $a = 1;  my @arr = (1, 2, 3);  my %h = (a => 1);
来源：http://hz.ybcxt.top/gtkbqlczky.html

[T43] Perl：字符串插值
来源：http://hz.sysykeji.top/gtwnbdafzm.html

"值: $a"
来源：http://hz.shangyingyoupin.top/gtwcjeerlf.html

[T44] Perl：条件
来源：http://hz.xingfuxueyuan.xyz/gtqydtogpr.html

if ($a > 0) { print "正"; }
来源：http://hz.yangfankeji.com/gtryyegfpe.html

[T45] Perl：数组遍历
来源：http://hz.xziqi.cn/gtbxoicmio.html

for my $x (@arr) { print $x; }
来源：http://hz.yvedp.cn/gtrbvhzrsp.html

[T46] Perl：哈希操作
来源：http://hz.cucudq.cn/gtziooogcd.html

$h{b} = 2;  for my $k (keys %h) { print "$k=$h{$k}"; }
来源：http://hz.yuanzhike.top/gtjmhhuylk.html

[T47] Perl：正则捕获
来源：http://hz.gogol.net.cn/gthhmoaoko.html

if ($s =~ /(\d+)/) { print $1; }
来源：http://hz.zhaomingkeji.xyz/gtaalfqfij.html

[T48] Perl：正则替换
来源：http://hz.xziqi.cn/gtpkeqdzbw.html

$s =~ s/old/new/g;
来源：http://hz.cucudq.cn/gtiavfwayn.html

[T49] Perl：函数
来源：http://hz.nanxinkj.top/gtaohplwvl.html

sub add { my ($a, $b) = @_; return $a + $b; }
来源：http://hz.xuanzx.com/gtfjnurshw.html

[T50] Perl：逐行读文件
来源：http://hz.aibaodan.cn/gtuwvdxkdf.html

open my $fh, "<", "a.txt" or die $!;
来源：http://hz.dashuyun.cn/gtiyudsbgq.html

while (my $line = <$fh>) { print $line; }
来源：http://hz.bjfxy.top/gtuqurwjhr.html

[T51] Scala：Hello World
来源：http://hz.yuxming.cn/gtjnvbljkj.html

println("Hello")
来源：http://hz.shangyingyoupin.top/gtrtsgatks.html

[T52] Scala：变量
来源：http://hz.wangdashe.top/gtdhzghrqg.html

val a = 1;  var b = 2
来源：http://hz.xingfuxueyuan.xyz/gtbydefcix.html

[T53] Scala：字符串插值
来源：http://hz.gotoacloud.top/gtzxwdooss.html

s"值: $b"
来源：http://hz.sxryk.cn/gtldqthdfv.html

[T54] Scala：集合映射
来源：http://hz.zdqjudy.top/gttzbyfcox.html

List(1, 2, 3).map(_ * 2)
来源：http://hz.smart0.xyz/gtdjhdpoea.html

[T55] Scala：集合过滤
来源：http://hz.ywan-chungtsiang.top/gtmxezpqla.html

List(1, 2, 3).filter(_ > 1)
来源：http://hz.snrcjt.cn/gtgeswfsrr.html

[T56] Scala：样例类
来源：http://hz.chenzaomai.com/gtumtvqlhc.html

case class User(name: String, age: Int)
来源：http://hz.chenlongwang.top/gtblmqqola.html

[T57] Scala：模式匹配
来源：http://hz.yj20258888.top/gtmafiubwr.html

x match { case 1 => "一"; case _ => "其他" }
来源：http://hz.hnxiangtu.top/gtipxfngfh.html

[T58] Scala：函数定义
来源：http://hz.yueranfly.top/gttjxxmfqa.html

def add(a: Int, b: Int): Int = a + b
来源：http://hz.9152youxi.cn/gthlhhpgov.html

[T59] Scala：循环
来源：http://hz.jinqigfzy.top/gtupkcbvxy.html

for (i <- 1 to 10) println(i)
来源：http://hz.dianchejie.cn/gtvumudtst.html

[T60] Scala：折叠
来源：http://hz.jinqigufen.top/gtwanexcat.html

List(1, 2, 3).foldLeft(0)(_ + _)
来源：http://hz.jqgufenzy.top/gtpvvlvphy.html

================================================================================
来源：http://hz.fzhhl.top/gtqpkpdoha.html

U. 高频实用片段（Python / PHP / JavaScript 各 40 条）
来源：http://hz.zhoulong.xyz/gtleuhknvp.html

================================================================================
来源：http://hz.jinghuilouyu.cn/gttyharada.html

[U01] Py：创建虚拟环境
来源：http://hz.yuanzhike.top/gtxsgkqgtn.html

python -m venv .venv && source .venv/bin/activate
来源：http://hz.mhx1999.top/gtgjphkipg.html

[U02] Py：导出 / 安装依赖
来源：http://hz.bjfxy.top/gtlwdwicvs.html

pip freeze > requirements.txt;  pip install -r requirements.txt
来源：http://hz.cheryme.top/gtdgbeotrz.html

[U03] Py：加载 .env 配置
来源：http://hz.iojbl.cn/gtmlnfkbbt.html

from dotenv import load_dotenv; load_dotenv()
来源：http://hz.nwbrower.top/gthkiifgij.html

[U04] Py：变量调试打印
来源：http://hz.0kj1m.cn/gtbsjcntbp.html

print(f"{x=}")            # 输出 x=值，Python 3.8+
来源：http://hz.jqgfzy.top/gtmvlvfixg.html

[U05] Py：列表去重且保序
来源：http://hz.iojbl.cn/gtztkhjvfe.html

list(dict.fromkeys(arr))
来源：http://hz.sweek.top/gtknnfdsta.html

[U06] Py：合并两个字典
来源：http://hz.fengsongda.top/gtvhpwzvqk.html

{**a, **b}
来源：http://hz.meibo888.top/gtlvbaqmjo.html

[U07] Py：反转字典键值
来源：http://hz.havefunace.top/gtzhibyfkh.html

{v: k for k, v in d.items()}
来源：http://hz.zhiwuduotai.top/gtzkfhtqvb.html

[U08] Py：展平二维列表
来源：http://hz.cdnleiting.top/gtimwufkel.html

[y for x in nested for y in x]
来源：http://hz.jlsjyb.cn/gtzyujgwse.html

[U09] Py：字典取最大值的键
来源：http://hz.jinghuilouyu.cn/gtqzdyihpx.html

max(d, key=d.get)
来源：http://hz.shangyingyoupin.top/gtlzhaidbw.html

[U10] Py：按值排序字典
来源：http://hz.smart0.xyz/gtrvzyddrd.html

dict(sorted(d.items(), key=lambda kv: kv[1]))
来源：http://hz.zhixingplan.top/gtpqgkkfrl.html

[U11] Py：生成器表达式
来源：http://hz.ehwqpu.com/gtkjnrpfxd.html

(x * 2 for x in arr)
来源：http://hz.redwolf501.top/gtnhjbowdx.html

[U12] Py：取出现最多的 3 个元素
来源：http://hz.zhongyouzk.top/gtuwvlnwyh.html

Counter(arr).most_common(3)
来源：http://hz.aizwys.cn/gtewwudvri.html

[U13] Py：固定长度队列
来源：http://hz.zhongyouzk.top/gtacxezahr.html

deque(maxlen=10)
来源：http://hz.yvedp.cn/gtcugmxxny.html

[U14] Py：分组收集到列表
来源：http://hz.gotoacloud.top/gtlgydxvmd.html

defaultdict(list)
来源：http://hz.yvedp.cn/gtrcymhszn.html

[U15] Py：高精度计时
来源：http://hz.jinqigfzy.top/gtrgonibom.html

t = time.perf_counter()
来源：http://hz.jlsjyb.cn/gtuuaomfns.html

[U16] Py：命令行参数解析
来源：http://hz.xuanzx.com/gtatwgcoje.html

ap = argparse.ArgumentParser();  ap.add_argument("--name");  args = ap.parse_args()
来源：http://hz.shanyushiyangkeji.top/gtcvjxckrw.html

[U17] Py：初始化日志
来源：http://hz.yj202588.top/gtqgttgqpe.html

logging.basicConfig(level=logging.INFO)
来源：http://hz.meibo888.top/gtboermxso.html

[U18] Py：预编译正则
来源：http://hz.svipenyu.cn/gtksihkdhs.html

pat = re.compile(r"\d+")
来源：http://hz.aibaodan.cn/gtnnywglss.html

[U19] Py：正则替换带回调
来源：http://hz.sweek.top/gtpfigvdhu.html

re.sub(r"\d+", lambda m: str(int(m.group()) * 2), s)
来源：http://hz.gaohongyu789.top/gtawueccra.html

[U20] Py：缓存函数结果
来源：http://hz.zhongyouzk.top/gtsduyebdi.html

@functools.lru_cache(maxsize=None)
来源：http://hz.yj202588.top/gtlvwzxtqd.html

[U21] Py：自定义上下文管理器
来源：http://hz.ybcxt.top/gtlzyypmdy.html

@contextlib.contextmanager
来源：http://hz.cdnleiting.top/gtszhmnatm.html

[U22] Py：矩阵转置
来源：http://hz.xinyue.icu/gtnzwerffs.html

list(zip(*m))
来源：http://hz.dashuyun.cn/gtlrstedsg.html

[U23] Py：分块读取大文件
来源：http://hz.cdnleiting.top/gtlhjldjtt.html

for chunk in iter(lambda: f.read(8192), b""):
来源：http://hz.hysaishi.cn/gtcahwrvvl.html

[U24] Py：路径操作
来源：http://hz.gotoacloud.top/gtbpszhage.html

Path("a/b.txt").parent.mkdir(parents=True, exist_ok=True)
来源：http://hz.chenzaomai.com/gtcvftlcxa.html

[U25] Py：CSV 按字典读
来源：http://hz.yanxiufei.cn/gteutzeynw.html

csv.DictReader(f)
来源：http://hz.zhongyouzk.top/gthinnipqb.html

[U26] Py：并发下载
来源：http://hz.nanxuanxn.top/gtyioadecd.html

ThreadPoolExecutor(max_workers=8).map(fetch, urls)
来源：http://hz.pengpengdd.cyou/gtndfwpztf.html

[U27] Py：异步 HTTP
来源：http://hz.zdqjudy.top/gtneomliyu.html

aiohttp.ClientSession() 配合 async with
来源：http://hz.shuidangran.top/gtkhbyopll.html

[U28] Py：类型别名
来源：http://hz.cucudq.cn/gttcojmeof.html

UserId = int
来源：http://hz.chenzaomai.com/gtgomucmro.html

[U29] Py：属性校验
来源：http://hz.ydjk.org.cn/gtwqlchcif.html

@property 与 @x.setter 配合
来源：http://hz.meibo888.top/gtuduacqua.html

[U30] Py：数据类
来源：http://hz.yueranfly.top/gthsauxsbg.html

@dataclass(slots=True)
来源：http://hz.vqdsnc.cn/gtvfyalmpk.html

[U31] Py：单测
来源：http://hz.hywenlv.cn/gtxzttyizf.html

python -m pytest -q
来源：http://hz.aizwys.cn/gtsevlhnwi.html

[U32] Py：代码格式化
来源：http://hz.nwbrower.top/gtnbkwhuco.html

ruff format . && ruff check --fix .
来源：http://hz.chenjidiqi.icu/gtjqgydoog.html

[U33] Py：打包发布
来源：http://hz.zhoulong.xyz/gtbccbojcj.html

python -m build  （依赖 pyproject.toml）
来源：http://hz.0kj1m.cn/gtvmpgpedn.html

[U34] Py：判断编码
来源：http://hz.ydzc1.top/gtbkbizmuh.html

chardet.detect(raw)
来源：http://hz.shanyushiyangtech.top/gtydumaplb.html

[U35] Py：发送邮件
来源：http://hz.0kj1m.cn/gtyyfjnrrj.html

smtplib.SMTP_SSL(...).send_message(msg)
来源：http://hz.feifeiyinyue.top/gtycueqlvm.html

[U36] Py：定时任务
来源：http://hz.kuanghao11.cn/gtlikdvdfg.html

schedule.every(10).minutes.do(job)
来源：http://hz.zhaomingkeji.xyz/gtjsxitatw.html

[U37] Py：读写 Excel
来源：http://hz.hammf.cn/gtnoakgkab.html

pandas.read_excel / DataFrame.to_excel
来源：http://hz.redwolf501.top/gtknucwpob.html

[U38] Py：获取脚本所在目录
来源：http://hz.zhoulong.xyz/gtujnduufu.html

Path(__file__).resolve().parent
来源：http://hz.svipenyu.cn/gtotbifkby.html

[U39] Py：判断是否在交互环境
来源：http://hz.zhengqikj.top/gtabzuzvij.html

sys.stdout.isatty()
来源：http://hz.yanxiufei.cn/gtweyuhwjh.html

[U40] Py：打印到标准错误
来源：http://hz.316326.xyz/gtfhctcbev.html

print("err", file=sys.stderr)
来源：http://hz.snrcjt.cn/gtxtenkaot.html

[U41] PHP：初始化 Composer 项目
来源：http://hz.feifeiyinyue.top/gtxhywjuwf.html

composer init;  composer require guzzlehttp/guzzle
来源：http://hz.cqqwz.cn/gtmsgeioiv.html

[U42] PHP：PSR-4 自动加载
来源：http://hz.ppjwa.cn/gtkhknmbsx.html

"autoload": { "psr-4": { "App\\": "src/" } }
来源：http://hz.xziqi.cn/gthvqgfeqb.html

[U43] PHP：声明命名空间
来源：http://hz.gogol.net.cn/gtxnwfxwje.html

namespace App\Http;
来源：http://hz.snrcjt.cn/gtrlqgrxcn.html

[U44] PHP：开启严格类型
来源：http://hz.yj20258888.top/gtvcvpktdn.html

declare(strict_types=1);
来源：http://hz.yj202588.top/gtaeoaxnvx.html

[U45] PHP：类型声明与返回类型
来源：http://hz.yj20258888.top/gtvsmkzzip.html

function add(int $a, int $b): int { return $a + $b; }
来源：http://hz.cashguo.top/gtfsjaevsd.html

[U46] PHP：可空类型
来源：http://hz.zhiwuduotai.top/gtfifxysig.html

?string $name = null
来源：http://hz.52xcode.cn/gtnrcofuma.html

[U47] PHP：联合类型
来源：http://hz.jiagoushi.top/gttcuvfogk.html

int|string $id
来源：http://hz.guowangkeji.top/gtfcerwlyq.html

[U48] PHP：纯枚举
来源：http://hz.snrcjt.cn/gtlgwsqybt.html

enum Status: string { case Active = "active"; case Off = "off"; }
来源：http://hz.jlsjyb.cn/gtmnyvbvub.html

[U49] PHP：只读属性
来源：http://hz.kuanghao11.cn/gtxbdekumm.html

public readonly string $name
来源：http://hz.xuetiantiany.cn/gtbbibmsvr.html

[U50] PHP：构造器属性提升
来源：http://hz.daxiang520.top/gtkahxfbel.html

public function __construct(private int $id) {}
来源：http://hz.ydjk.org.cn/gtemleevcp.html


<!-- 参考信息 -->