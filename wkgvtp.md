代发 wailian999

static int counter = 0;
来源：http://hz.shanyushiyangtech.top/gtujozsret.html

[S29] C：变参函数
来源：http://hz.gzhubu.top/gtcfbllhik.html

va_list ap; va_start(ap, fmt); vprintf(fmt, ap); va_end(ap);
来源：http://hz.fzhhl.top/gtlvtnocyn.html

[S30] C：头文件保护
来源：http://hz.kuanghao11.cn/gtwestmafw.html

#ifndef X_H
来源：http://hz.sysykeji.top/gtukiksbqn.html

#define X_H
来源：http://hz.chenlongwang.top/gthrmiwdun.html

#endif
来源：http://hz.ybcxt.top/gtpctikbtt.html

[S31] C++：Hello World
来源：http://hz.shanyushiyangkeji.top/gtskmiwhrr.html

#include <iostream>
来源：http://hz.shanyushiyangkeji.top/gthajpfbzt.html

int main() { std::cout << "Hello\n"; }
来源：http://hz.zycfv.cn/gthdbwwfkp.html

[S32] C++：字符串
来源：http://hz.guannengcc.top/gtwnhqqbho.html

std::string s = "hi";  s += "!";
来源：http://hz.jinyuanbaomall.cn/gtbhdinpnu.html

[S33] C++：vector 增删
来源：http://hz.tian-w.cn/gtsimonfwz.html

std::vector<int> v{1, 2, 3};  v.push_back(4);
来源：http://hz.guowangkeji.top/gtcknxcksh.html

[S34] C++：遍历 vector
来源：http://hz.yuanzhike.top/gtkhexfjqs.html

for (auto &x : v) { std::cout << x; }
来源：http://hz.xinyue.icu/gtmgevlhem.html

[S35] C++：map
来源：http://hz.hywenlv.cn/gtsawohvrm.html

std::map<std::string, int> m;  m["a"] = 1;
来源：http://hz.cashguo.top/gttyliygby.html

[S36] C++：unordered_map
来源：http://hz.xylfe.cn/gtammljwxr.html

std::unordered_map<std::string, int> m;  m["a"] = 1;
来源：http://hz.52xcode.cn/gtqpsgibst.html

[S37] C++：set
来源：http://hz.9152youxi.cn/gtyrtypqql.html

std::set<int> s{1, 2, 3};  s.insert(4);
来源：http://hz.guannengcc.top/gtsxfjrryv.html

[S38] C++：排序
来源：http://hz.wangshuangyany.cn/gtxzkbmqji.html

std::sort(v.begin(), v.end());
来源：http://hz.nanxuanxn.top/gtugebpllp.html

[S39] C++：自定义比较器排序
来源：http://hz.pengpengdd.cyou/gtlwrjpwgl.html

std::sort(v.begin(), v.end(), [](int a, int b) { return a > b; });
来源：http://hz.ybcxt.top/gtmeywsrrr.html

[S40] C++：查找元素
来源：http://hz.zhengqikj.top/gttvankoes.html

auto it = std::find(v.begin(), v.end(), 3);
来源：http://hz.shangyingyoupin.top/gtwhtugpcn.html

[S41] C++：类与构造函数
来源：http://hz.xuetiantiany.cn/gtbjgswwxw.html

class A { public: A(int v) : x_(v) {} int get() const { return x_; } private: int x_; };
来源：http://hz.xziqi.cn/gteggpgzss.html

[S42] C++：继承与虚函数
来源：http://hz.cdnleiting.top/gtbbqayqlt.html

class B : public Base { public: void f() override {} };
来源：http://hz.fzhhl.top/gtzypiwfct.html

[S43] C++：智能指针
来源：http://hz.redwolf501.top/gtjgexcgmc.html

auto p = std::make_unique<int>(5);
来源：http://hz.jqgufenzy.top/gtpjyqkwpl.html

[S44] C++：引用传参
来源：http://hz.hammf.cn/gtcmijdszl.html

void inc(int &x) { ++x; }
来源：http://hz.hfpthk.cn/gtkgvnlgnp.html

[S45] C++：lambda
来源：http://hz.vqdsnc.cn/gtestobxky.html

auto add = [](int a, int b) { return a + b; };
来源：http://hz.jinqigufen.top/gtircargal.html

[S46] C++：函数模板
来源：http://hz.yonumen.top/gtqggactoj.html

template <typename T> T maxv(T a, T b) { return a > b ? a : b; }
来源：http://hz.zhijiandao.cn/gtwgdamnbe.html

[S47] C++：结构化绑定遍历
来源：http://hz.pycfn.com/gtbpsfgzge.html

for (const auto &[k, v] : m) { std::cout << k << v; }
来源：http://hz.tianlin.xyz/gtnkvdyrnc.html

[S48] C++：逐行读文件
来源：http://hz.zhongyouzk.top/gteaveadec.html

std::ifstream in("a.txt");  std::string line;
来源：http://hz.zhiwuduotai.top/gtsypcfbrt.html

while (std::getline(in, line)) { }
来源：http://hz.fengsongda.top/gtsrpxmcig.html

[S49] C++：写文件
来源：http://hz.hfpthk.cn/gteghbmrwe.html

std::ofstream out("a.txt");  out << "hi\n";
来源：http://hz.ehwqpu.com/gtlyiramlo.html

[S50] C++：格式化数字
来源：http://hz.sxryk.cn/gtmdepftwy.html

std::ostringstream os;  os << std::fixed << std::setprecision(2) << 3.14159;
来源：http://hz.shanyushiyangkeji.top/gtgmncaonb.html

[S51] C++：显式类型转换
来源：http://hz.shanyushiyangtech.top/gtakaumfcc.html

static_cast<double>(a) / b
来源：http://hz.xziqi.cn/gtggjevrnc.html

[S52] C++：const 与 noexcept
来源：http://hz.cheryme.top/gtkhfpgllm.html

int size() const noexcept { return n_; }
来源：http://hz.zhiwuduotai.top/gtlmauzdkl.html

[S53] C++：移动语义
来源：http://hz.cheryme.top/gtjjeyspwm.html

std::vector<int> w = std::move(v);
来源：http://hz.hnxiangtu.top/gtzltgihnd.html

[S54] C++：异常处理
来源：http://hz.hfpthk.cn/gtzksuezzi.html

try { throw std::runtime_error("x"); } catch (const std::exception &e) { }
来源：http://hz.tanke756.top/gtjviskmzy.html

[S55] C++：结构化绑定
来源：http://hz.havefunace.top/gttnfsirny.html

auto [a, b] = std::make_pair(1, 2);
来源：http://hz.chenlongwang.top/gtzwdfyhqg.html

[S56] C++：optional
来源：http://hz.xziqi.cn/gtlxdjxrsv.html

std::optional<int> o = 5;  if (o) { int v = *o; }
来源：http://hz.guannengcc.top/gtnznpjwid.html

[S57] C++：编译期常量
来源：http://hz.vqdsnc.cn/gtzjpeiwii.html

constexpr int N = 10;
来源：http://hz.xziqi.cn/gtdrbvsuvm.html

[S58] C++：命名空间
来源：http://hz.xuetiantiany.cn/gtaqzgnhjh.html

namespace ns { int f() { return 1; } }
来源：http://hz.andypj.xyz/gtbfmluhyr.html

[S59] C++：静态断言
来源：http://hz.quarkkingdee.top/gtwmstzpaj.html

static_assert(sizeof(int) == 4, "int 必须 4 字节");
来源：http://hz.yuanzhike.top/gtorejrczd.html

[S60] C++：遍历并删除元素
来源：http://hz.gogol.net.cn/gtwagmujfs.html

v.erase(std::remove_if(v.begin(), v.end(), [](int x) { return x < 0; }), v.end());
来源：http://hz.hfpthk.cn/gtrlopxbbr.html

================================================================================
来源：http://hz.xuetiantiany.cn/gtueaxlips.html

T. 其他语言补充（Kotlin / Swift / Lua / Perl / Scala）
来源：http://hz.vqdsnc.cn/gthsvdeubv.html

================================================================================
来源：http://hz.yj20258.top/gtxoxtrrxp.html

[T01] Kotlin：Hello World
来源：http://hz.316326.xyz/gtkjmerrmo.html

println("Hello")
来源：http://hz.gotoacloud.top/gtpohjgioa.html

[T02] Kotlin：变量
来源：http://hz.jinqigufen.top/gthkfvuoid.html

val a = 1;  var b = 2        // val 只读，var 可变
来源：http://hz.tianlin.xyz/gtkhimzziw.html

[T03] Kotlin：字符串模板
来源：http://hz.sufxvd.cn/gtnsmyywkz.html

"值: $b"
来源：http://hz.ivvv.top/gtqigczkte.html

[T04] Kotlin：空安全
来源：http://hz.dianchejie.cn/gtbxxixalp.html

val n: String? = null;  n?.length
来源：http://hz.yangfankeji.com/gtdozfhhob.html

[T05] Kotlin：when 表达式
来源：http://hz.zhixingplan.top/gtdfkklqsv.html

val s = when (x) { 1 -> "一" else -> "其他" }   // 多分支时每个分支单独一行
来源：http://hz.ydzc1.top/gttspxqupf.html

[T06] Kotlin：集合映射
来源：http://hz.zhixingplan.top/gttrowfgou.html

listOf(1, 2, 3).map { it * 2 }
来源：http://hz.zhoulong.xyz/gtxcdjemck.html

[T07] Kotlin：集合过滤
来源：http://hz.cashguo.top/gtnyfylkcn.html

listOf(1, 2, 3).filter { it > 1 }
来源：http://hz.ydjk.org.cn/gtfkeiqmyj.html

[T08] Kotlin：数据类
来源：http://hz.shanyushiyangtech.top/gtjxpicdwb.html

data class User(val name: String, val age: Int)
来源：http://hz.zycfv.cn/gtxtyqiiqc.html

[T09] Kotlin：扩展函数
来源：http://hz.xuanzx.com/gtzdwiftxx.html

fun String.exclaim() = this + "!"
来源：http://hz.xuetiantiany.cn/gtljwebvoe.html

[T10] Kotlin：默认参数
来源：http://hz.sxryk.cn/gtwqvbzwpz.html

fun greet(name: String = "World") = "Hi $name"
来源：http://hz.aibaodan.cn/gtypqpgcfj.html

[T11] Kotlin：协程
来源：http://hz.yvedp.cn/gtbbkxvycz.html

GlobalScope.launch { delay(1000); println("done") }
来源：http://hz.yuanzhike.top/gttrarpycq.html

[T12] Kotlin：解构声明
来源：http://hz.pengpengdd.cyou/gtfperhdhq.html

val (a, b) = Pair(1, 2)
来源：http://hz.bjfxy.top/gttrkitvgy.html

[T13] Kotlin：只读 Map
来源：http://hz.pycfn.com/gtvfvhoqmn.html

val m = mapOf("a" to 1)
来源：http://hz.chenjidiqi.icu/gtnoinfgnp.html

[T14] Kotlin：循环
来源：http://hz.quarkkingdee.top/gtetfhvkox.html

for (i in 1..10) println(i)
来源：http://hz.jinqigufen.top/gtjhlnnljt.html

[T15] Kotlin：接口
来源：http://hz.fengsongda.top/gtzxryindl.html

interface Shape { fun area(): Double }
来源：http://hz.sysykeji.top/gtpcrlghbi.html

[T16] Swift：Hello World
来源：http://hz.zhijiandao.cn/gtyhcvfzax.html

print("Hello")
来源：http://hz.gaohongyu789.top/gtfywawgsi.html

[T17] Swift：变量与常量
来源：http://hz.gzhubu.top/gtazamqroz.html

var a = 1;  let b = 2
来源：http://hz.zhongyouzk.top/gtdqdlreqd.html

[T18] Swift：字符串插值
来源：http://hz.jinqigufen.top/gtnrmrkfoo.html

"值: \(b)"
来源：http://hz.sysykeji.top/gtfopefvpb.html

[T19] Swift：可选绑定
来源：http://hz.hnqzz.top/gtjphtlvtv.html

if let n = opt { print(n) }
来源：http://hz.zhiwuduotai.top/gtjdmqzmxe.html

[T20] Swift：数组操作
来源：http://hz.shangyingyoupin.top/gtmbldwzfj.html

var a = [1, 2, 3];  a.append(4)
来源：http://hz.wangshuangyany.cn/gtxerndmyy.html

[T21] Swift：遍历
来源：http://hz.tianlin.xyz/gtzhitoiha.html

for x in a { print(x) }
来源：http://hz.ydzc1.top/gtudksjocq.html

[T22] Swift：字典
来源：http://hz.ywan-chungtsiang.top/gtojaypnpq.html

var d = ["a": 1];  d["b"] = 2
来源：http://hz.vqdsnc.cn/gtqtswhbkk.html

[T23] Swift：函数
来源：http://hz.guowangkeji.top/gtwmihiblb.html

func add(_ a: Int, _ b: Int) -> Int { a + b }
来源：http://hz.ybcxt.top/gtuwmragfw.html

[T24] Swift：闭包
来源：http://hz.fengsongda.top/gtnymiaazb.html

let f = { (x: Int) -> Int in x * 2 }
来源：http://hz.yuanzhike.top/gteoqjpghl.html

[T25] Swift：结构体
来源：http://hz.zhiwuduotai.top/gtffbethhp.html

struct P { var x: Int }
来源：http://hz.jianghu66.top/gtyorlofhl.html

[T26] Swift：类与重写
来源：http://hz.gzhubu.top/gtlpmbladi.html

class A: Base { override func f() {} }
来源：http://hz.gzhubu.top/gtffgeofls.html

[T27] Swift：错误处理
来源：http://hz.yvedp.cn/gtpydjxwoi.html

do { try f() } catch { print(error) }
来源：http://hz.chenjidiqi.icu/gtqvulmdhs.html

[T28] Swift：枚举
来源：http://hz.gaohongyu789.top/gtjmnhdjbr.html

enum Color { case red, green }
来源：http://hz.kuanghao11.cn/gtpqxxsxxn.html

[T29] Swift：guard 提前返回
来源：http://hz.jinghuilouyu.cn/gtdlnvkqay.html

guard let x = opt else { return }
来源：http://hz.ydzc1.top/gtoxeluhqd.html

[T30] Swift：协议
来源：http://hz.yanxiufei.cn/gtaewenacs.html

protocol Shape { func area() -> Double }
来源：http://hz.pengpengdd.cyou/gtqqvhlyua.html

[T31] Lua：Hello World
来源：http://hz.hywenlv.cn/gtuhmhgttx.html

print("Hello")
来源：http://hz.haohaochexian.top/gtoyqxecvm.html

[T32] Lua：局部变量
来源：http://hz.jlsjyb.cn/gttqbctxdq.html

local a = 1
来源：http://hz.jqgufenzy.top/gtprklvhmk.html

[T33] Lua：表（数组）
来源：http://hz.hongshengwenyu.top/gtcgufkkov.html

local t = {1, 2, 3};  t[4] = 4
来源：http://hz.pengpengdd.cyou/gthofodyvw.html

[T34] Lua：遍历表
来源：http://hz.jinghuilouyu.cn/gtoamljjif.html

for i, v in ipairs(t) do print(i, v) end
来源：http://hz.sysykeji.top/gtnxpnojsw.html

[T35] Lua：字典表
来源：http://hz.pycfn.com/gtfugsehvf.html

local d = { a = 1 };  d.b = 2
来源：http://hz.feifeiyinyue.top/gtguskzocb.html

[T36] Lua：函数
来源：http://hz.daxiang520.top/gtlupdsfqn.html

function add(a, b) return a + b end
来源：http://hz.jiagoushi.top/gtiormjlrm.html

[T37] Lua：字符串拼接
来源：http://hz.52xcode.cn/gtkxqgkdbg.html

"a" .. "b"
来源：http://hz.hysaishi.cn/gtktmsbcvt.html

[T38] Lua：条件
来源：http://hz.ydjk.org.cn/gtevstthbx.html

if x > 0 then print("正") end
来源：http://hz.haohaochexian.top/gtfmesfdnh.html

[T39] Lua：模式匹配
来源：http://hz.zhoulong.xyz/gttlqnehdm.html

string.find(s, "%d+")
来源：http://hz.vqdsnc.cn/gtptlszyoc.html

[T40] Lua：元表
来源：http://hz.ppjwa.cn/gtfrmreece.html

setmetatable({}, { __index = base })
来源：http://hz.zhongyouzk.top/gtwauuntwy.html

[T41] Perl：Hello World
来源：http://hz.jlsjyb.cn/gtjzjyxwyk.html

print "Hello\n";
来源：http://hz.jinqigufen.top/gtaedhrlch.html

[T42] Perl：变量类型
来源：http://hz.yangfankeji.com/gtizwyyioy.html

my $a = 1;  my @arr = (1, 2, 3);  my %h = (a => 1);
来源：http://hz.gzhubu.top/gtxykwnqiu.html

[T43] Perl：字符串插值
来源：http://hz.yueranfly.top/gtaeamqslk.html

"值: $a"
来源：http://hz.yj202588.top/gtobqcefpm.html

[T44] Perl：条件
来源：http://hz.ivvv.top/gtosfdwviw.html

if ($a > 0) { print "正"; }
来源：http://hz.hammf.cn/gtklyzvhum.html

[T45] Perl：数组遍历
来源：http://hz.chenjidiqi.icu/gttppnpcsz.html

for my $x (@arr) { print $x; }
来源：http://hz.yj202588.top/gtpfnacazn.html

[T46] Perl：哈希操作
来源：http://hz.yonumen.top/gtdtblsdyh.html

$h{b} = 2;  for my $k (keys %h) { print "$k=$h{$k}"; }
来源：http://hz.shanyushiyangtech.top/gtjzxpjofb.html

[T47] Perl：正则捕获
来源：http://hz.kuanghao11.cn/gtttezwqev.html

if ($s =~ /(\d+)/) { print $1; }
来源：http://hz.yuanzhike.top/gtfgepacgk.html

[T48] Perl：正则替换
来源：http://hz.52xcode.cn/gthsctnuxo.html

$s =~ s/old/new/g;
来源：http://hz.mhx1999.top/gtfrwytplp.html

[T49] Perl：函数
来源：http://hz.hammf.cn/gtdqbabvqz.html

sub add { my ($a, $b) = @_; return $a + $b; }
来源：http://hz.zhiwuduotai.top/gtcivbgioy.html

[T50] Perl：逐行读文件
来源：http://hz.daria6918.cn/gtrhazhblf.html

open my $fh, "<", "a.txt" or die $!;
来源：http://hz.birdmap.top/gtbdpkkzzw.html

while (my $line = <$fh>) { print $line; }
来源：http://hz.hnxiangtu.top/gtbmxlcfeh.html

[T51] Scala：Hello World
来源：http://hz.kuanghao11.cn/gttgvckbsk.html

println("Hello")
来源：http://hz.cucudq.cn/gtqcliycfe.html

[T52] Scala：变量
来源：http://hz.hywenlv.cn/gtsivjlsum.html

val a = 1;  var b = 2
来源：http://hz.chenlongwang.top/gtgrgxehkp.html

[T53] Scala：字符串插值
来源：http://hz.nanxuanxn.top/gtkffmgzgk.html

s"值: $b"
来源：http://hz.hnxiangtu.top/gtwlymmgqj.html

[T54] Scala：集合映射
来源：http://hz.nanxinkj.top/gtsflazkym.html

List(1, 2, 3).map(_ * 2)
来源：http://hz.52xcode.cn/gtzewqrczi.html

[T55] Scala：集合过滤
来源：http://hz.ydzc1.top/gtrvpkresx.html

List(1, 2, 3).filter(_ > 1)
来源：http://hz.jinqigufen.top/gtkxyrosew.html

[T56] Scala：样例类
来源：http://hz.jlsjyb.cn/gtpplnyuuf.html

case class User(name: String, age: Int)
来源：http://hz.daria6918.cn/gtayxelyrm.html

[T57] Scala：模式匹配
来源：http://hz.yueranfly.top/gtwelpmxgz.html

x match { case 1 => "一"; case _ => "其他" }
来源：http://hz.yvedp.cn/gthovddbeo.html

[T58] Scala：函数定义
来源：http://hz.haohaochexian.top/gthufzsbci.html

def add(a: Int, b: Int): Int = a + b
来源：http://hz.sysykeji.top/gtessnlhwj.html

[T59] Scala：循环
来源：http://hz.shangyingyoupin.top/gtcmurirxz.html

for (i <- 1 to 10) println(i)
来源：http://hz.cheryme.top/gtyhhoylrt.html

[T60] Scala：折叠
来源：http://hz.yj20258888.top/gtsuprwsrw.html

List(1, 2, 3).foldLeft(0)(_ + _)
来源：http://hz.zhijiandao.cn/gtlqoapiab.html

================================================================================
来源：http://hz.shzxlz.cn/gtdqslztto.html

U. 高频实用片段（Python / PHP / JavaScript 各 40 条）
来源：http://hz.fengsongda.top/gtomsggjxm.html

================================================================================
来源：http://hz.zhongyouzk.top/gtrjjvbrwv.html

[U01] Py：创建虚拟环境
来源：http://hz.chenlongwang.top/gtaxdpncdr.html

python -m venv .venv && source .venv/bin/activate
来源：http://hz.iojbl.cn/gtmsqqfifm.html

[U02] Py：导出 / 安装依赖
来源：http://hz.fengsongda.top/gthxiesksv.html

pip freeze > requirements.txt;  pip install -r requirements.txt
来源：http://hz.zycfv.cn/gtsxdwqfts.html

[U03] Py：加载 .env 配置
来源：http://hz.hammf.cn/gtyaowsdmf.html

from dotenv import load_dotenv; load_dotenv()
来源：http://hz.iojbl.cn/gtqnvelgqr.html

[U04] Py：变量调试打印
来源：http://hz.aizwys.cn/gtehzedlqc.html

print(f"{x=}")            # 输出 x=值，Python 3.8+
来源：http://hz.ivvv.top/gtsqmelhae.html

[U05] Py：列表去重且保序
来源：http://hz.birdmap.top/gtxirtydhu.html

list(dict.fromkeys(arr))
来源：http://hz.pengpengdd.cyou/gtgdtjftwi.html

[U06] Py：合并两个字典
来源：http://hz.chenjidiqi.icu/gtxdazzrpw.html

{**a, **b}
来源：http://hz.mhx1999.top/gtpysibspw.html

[U07] Py：反转字典键值
来源：http://hz.nanxuanxn.top/gtwzrgzesl.html

{v: k for k, v in d.items()}
来源：http://hz.zhixingplan.top/gtejhmsudr.html

[U08] Py：展平二维列表
来源：http://hz.wangdashe.top/gtoqdeoxdi.html

[y for x in nested for y in x]
来源：http://hz.vqdsnc.cn/gturxxqvqm.html

[U09] Py：字典取最大值的键
来源：http://hz.yj20258.top/gttlfrbupr.html

max(d, key=d.get)
来源：http://hz.xinyue.icu/gtsqmcxsom.html

[U10] Py：按值排序字典
来源：http://hz.yanxiufei.cn/gtimadbsoh.html

dict(sorted(d.items(), key=lambda kv: kv[1]))
来源：http://hz.hysaishi.cn/gtrxymnznd.html

[U11] Py：生成器表达式
来源：http://hz.wangshuangyany.cn/gtpepmwnhd.html

(x * 2 for x in arr)
来源：http://hz.jianghu66.top/gtrotpovrx.html

[U12] Py：取出现最多的 3 个元素
来源：http://hz.dashuyun.cn/gtkxhwilbm.html

Counter(arr).most_common(3)
来源：http://hz.hongshengwenyu.top/gtrxiioekm.html

[U13] Py：固定长度队列
来源：http://hz.jqgfzy.top/gtkppqbfvd.html

deque(maxlen=10)
来源：http://hz.xingfuxueyuan.xyz/gtrkrloxmv.html

[U14] Py：分组收集到列表
来源：http://hz.fzhhl.top/gtlzwphmoa.html

defaultdict(list)
来源：http://hz.jlsjyb.cn/gtlovohqcm.html

[U15] Py：高精度计时
来源：http://hz.wangdashe.top/gtgfhnefwb.html

t = time.perf_counter()
来源：http://hz.zycfv.cn/gtmnggfiup.html

[U16] Py：命令行参数解析
来源：http://hz.feifeiyinyue.top/gtxidmpwsy.html

ap = argparse.ArgumentParser();  ap.add_argument("--name");  args = ap.parse_args()
来源：http://hz.ydzc1.top/gttwnsloae.html

[U17] Py：初始化日志
来源：http://hz.cucudq.cn/gteimxbgta.html

logging.basicConfig(level=logging.INFO)
来源：http://hz.bjfxy.top/gtwzpesxxo.html

[U18] Py：预编译正则
来源：http://hz.ywan-chungtsiang.top/gtajpnxvge.html

pat = re.compile(r"\d+")
来源：http://hz.shanyushiyangkeji.top/gthzkzgfpm.html

[U19] Py：正则替换带回调
来源：http://hz.dianchejie.cn/gtslvgyatc.html

re.sub(r"\d+", lambda m: str(int(m.group()) * 2), s)
来源：http://hz.sysykeji.top/gtzcaapcdf.html

[U20] Py：缓存函数结果
来源：http://hz.gaohongyu789.top/gtyhinrbbm.html

@functools.lru_cache(maxsize=None)
来源：http://hz.jinyuanbaomall.cn/gtxtjecdgy.html

[U21] Py：自定义上下文管理器
来源：http://hz.shangyingyoupin.top/gtiupowjgx.html

@contextlib.contextmanager
来源：http://hz.cheryme.top/gtpleybqzx.html

[U22] Py：矩阵转置
来源：http://hz.haohaochexian.top/gtdpzoxbkf.html

list(zip(*m))
来源：http://hz.jlsjyb.cn/gtwwryzazz.html

[U23] Py：分块读取大文件
来源：http://hz.guowangkeji.top/gtflnfqjsy.html

for chunk in iter(lambda: f.read(8192), b""):
来源：http://hz.cqqwz.cn/gtoqchrmlj.html

[U24] Py：路径操作
来源：http://hz.sysykeji.top/gtxidyszjz.html

Path("a/b.txt").parent.mkdir(parents=True, exist_ok=True)
来源：http://hz.havefunace.top/gtuutedzek.html

[U25] Py：CSV 按字典读
来源：http://hz.aizwys.cn/gtelelgmyj.html

csv.DictReader(f)
来源：http://hz.gotoacloud.top/gtudnmjbxf.html

[U26] Py：并发下载
来源：http://hz.tian-w.cn/gtmnivglqk.html

ThreadPoolExecutor(max_workers=8).map(fetch, urls)
来源：http://hz.c1oappe.top/gtkxfunfga.html

[U27] Py：异步 HTTP
来源：http://hz.tian-w.cn/gtwwpcqzyq.html

aiohttp.ClientSession() 配合 async with
来源：http://hz.zhengqikj.top/gtyhhqveoh.html

[U28] Py：类型别名
来源：http://hz.ydjk.org.cn/gtntzuvunv.html

UserId = int
来源：http://hz.wangshuangyany.cn/gtmfkbcbbh.html

[U29] Py：属性校验
来源：http://hz.hywenlv.cn/gtdjhwyvls.html

@property 与 @x.setter 配合
来源：http://hz.0kj1m.cn/gtyolpfhpt.html

[U30] Py：数据类
来源：http://hz.cashguo.top/gtlqefrnvq.html

@dataclass(slots=True)
来源：http://hz.shanyushiyangkeji.top/gtbzmyazft.html

[U31] Py：单测
来源：http://hz.yj20258888.top/gtcpnsovxu.html

python -m pytest -q
来源：http://hz.xinyue.icu/gtjwgvsgwx.html

[U32] Py：代码格式化
来源：http://hz.yj202588.top/gtspukemaq.html

ruff format . && ruff check --fix .
来源：http://hz.0kj1m.cn/gtotcveiki.html

[U33] Py：打包发布
来源：http://hz.jinqigfzy.top/gtdjmrghqz.html

python -m build  （依赖 pyproject.toml）
来源：http://hz.zdqjudy.top/gtkinrsiww.html

[U34] Py：判断编码
来源：http://hz.daxiang520.top/gtexjzylwy.html

chardet.detect(raw)
来源：http://hz.hongshengwenyu.top/gtsynakxgg.html

[U35] Py：发送邮件
来源：http://hz.yj20258.top/gtbbdthoec.html

smtplib.SMTP_SSL(...).send_message(msg)
来源：http://hz.yanxiufei.cn/gtjqbrdfhu.html

[U36] Py：定时任务
来源：http://hz.yonumen.top/gtsfvvelgu.html

schedule.every(10).minutes.do(job)
来源：http://hz.guannengcc.top/gtundeprpr.html

[U37] Py：读写 Excel
来源：http://hz.jinyuanbaomall.cn/gtptaoqvbj.html

pandas.read_excel / DataFrame.to_excel
来源：http://hz.zycfv.cn/gtrcepoxbu.html

[U38] Py：获取脚本所在目录
来源：http://hz.zhijiandao.cn/gtsczfoddj.html

Path(__file__).resolve().parent
来源：http://hz.xylfe.cn/gtyibufrgr.html

[U39] Py：判断是否在交互环境
来源：http://hz.yueranfly.top/gthfsxzxgs.html

sys.stdout.isatty()
来源：http://hz.tian-w.cn/gttyuqqoei.html

[U40] Py：打印到标准错误
来源：http://hz.ydjk.org.cn/gtsmmbtwig.html

print("err", file=sys.stderr)
来源：http://hz.wangdashe.top/gtknismlfw.html

[U41] PHP：初始化 Composer 项目
来源：http://hz.jyoumei.cn/gtahdounxx.html

composer init;  composer require guzzlehttp/guzzle
来源：http://hz.jinghuilouyu.cn/gtbhwoknzp.html

[U42] PHP：PSR-4 自动加载
来源：http://hz.hnxiangtu.top/gtdfjatuct.html

"autoload": { "psr-4": { "App\\": "src/" } }
来源：http://hz.pycfn.com/gtjnzyjrhi.html

[U43] PHP：声明命名空间
来源：http://hz.cqqwz.cn/gtvxyzrqgk.html

namespace App\Http;
来源：http://hz.jqgfzy.top/gtprcrmavh.html

[U44] PHP：开启严格类型
来源：http://hz.9152youxi.cn/gtgzrwqlli.html

declare(strict_types=1);
来源：http://hz.gogol.net.cn/gtszrjvyrq.html

[U45] PHP：类型声明与返回类型
来源：http://hz.xuanzx.com/gtnnplrxmi.html

function add(int $a, int $b): int { return $a + $b; }
来源：http://hz.feifeiyinyue.top/gtakrwwthi.html

[U46] PHP：可空类型
来源：http://hz.ppjwa.cn/gtszsdlbor.html

?string $name = null
来源：http://hz.gotoacloud.top/gtlnomvnjf.html

[U47] PHP：联合类型
来源：http://hz.yongpay.top/gtarokkbvp.html

int|string $id
来源：http://hz.yj202588.top/gtzoysyqdo.html

[U48] PHP：纯枚举
来源：http://hz.aibaodan.cn/gtyneipbep.html

enum Status: string { case Active = "active"; case Off = "off"; }
来源：http://hz.shzxlz.cn/gtgzatiski.html

[U49] PHP：只读属性
来源：http://hz.nanxuanxn.top/gtafsvwzaa.html

public readonly string $name
来源：http://hz.aizwys.cn/gtftsuvpxu.html

[U50] PHP：构造器属性提升
来源：http://hz.shanyushiyangkeji.top/gtukvclrwg.html

public function __construct(private int $id) {}
来源：http://hz.316326.xyz/gtrrwfntmv.html

[U51] PHP：数组解构
来源：http://hz.havefunace.top/gtqwjhtrgn.html

[$a, $b] = $arr;
来源：http://hz.jiagoushi.top/gtxlfhldjj.html

[U52] PHP：箭头函数
来源：http://hz.tian-w.cn/gtxwrxpwyf.html

$double = fn($x) => $x * 2;
来源：http://hz.jiagoushi.top/gthdellekn.html


<!-- 参考信息 -->