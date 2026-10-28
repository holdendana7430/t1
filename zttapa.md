代发 wailian999

time_t t = time(NULL);  struct tm *tm = localtime(&t);
来源：http://hz.xingfuxueyuan.xyz/gtuzhohddp.html

[S25] C：内存拷贝
来源：http://hz.dianchejie.cn/gtbxqkafef.html

memcpy(dst, src, n);
来源：http://hz.jlsjyb.cn/gtdgkuioxn.html

[S26] C：内存清零
来源：http://hz.jinghuilouyu.cn/gtpeeacbqb.html

memset(a, 0, sizeof a);
来源：http://hz.mhx1999.top/gtnjzvcrrm.html

[S27] C：定义常量
来源：http://hz.hywenlv.cn/gtvgqxtobo.html

const double PI = 3.14159;
来源：http://hz.xuetiantiany.cn/gttthohhju.html

[S28] C：静态变量
来源：http://hz.iojbl.cn/gttckxhjtv.html

static int counter = 0;
来源：http://hz.birdmap.top/gtfgntzmcx.html

[S29] C：变参函数
来源：http://hz.jinghuilouyu.cn/gtavadhlnc.html

va_list ap; va_start(ap, fmt); vprintf(fmt, ap); va_end(ap);
来源：http://hz.hysaishi.cn/gtsboaljmz.html

[S30] C：头文件保护
来源：http://hz.ywan-chungtsiang.top/gtrnmibukm.html

#ifndef X_H
来源：http://hz.pycfn.com/gtaergbwjw.html

#define X_H
来源：http://hz.cucudq.cn/gtyliebyca.html

#endif
来源：http://hz.hfpthk.cn/gthkzfahyx.html

[S31] C++：Hello World
来源：http://hz.hammf.cn/gtftgpegzm.html

#include <iostream>
来源：http://hz.yj20258888.top/gtspniavdz.html

int main() { std::cout << "Hello\n"; }
来源：http://hz.jianghu66.top/gtsbdwydpr.html

[S32] C++：字符串
来源：http://hz.haohaochexian.top/gtbdcbuwdw.html

std::string s = "hi";  s += "!";
来源：http://hz.316326.xyz/gtyutlaqri.html

[S33] C++：vector 增删
来源：http://hz.dianchejie.cn/gtdzsvsexk.html

std::vector<int> v{1, 2, 3};  v.push_back(4);
来源：http://hz.wangdashe.top/gttxwhfqyg.html

[S34] C++：遍历 vector
来源：http://hz.zhoulong.xyz/gtspbrjwug.html

for (auto &x : v) { std::cout << x; }
来源：http://hz.fengsongda.top/gtdkkvmfwe.html

[S35] C++：map
来源：http://hz.jiagoushi.top/gtizhumvdh.html

std::map<std::string, int> m;  m["a"] = 1;
来源：http://hz.pengpengdd.cyou/gtligkmliq.html

[S36] C++：unordered_map
来源：http://hz.quarkkingdee.top/gtkwpfarga.html

std::unordered_map<std::string, int> m;  m["a"] = 1;
来源：http://hz.9152youxi.cn/gtuxyxdxbk.html

[S37] C++：set
来源：http://hz.chenjidiqi.icu/gthezgbswt.html

std::set<int> s{1, 2, 3};  s.insert(4);
来源：http://hz.cashguo.top/gtvxissutx.html

[S38] C++：排序
来源：http://hz.ydzc1.top/gtxkkrjmka.html

std::sort(v.begin(), v.end());
来源：http://hz.quarkkingdee.top/gtixbvmcoo.html

[S39] C++：自定义比较器排序
来源：http://hz.kuanghao11.cn/gtegnpcgan.html

std::sort(v.begin(), v.end(), [](int a, int b) { return a > b; });
来源：http://hz.ivvv.top/gtxizctcqm.html

[S40] C++：查找元素
来源：http://hz.hammf.cn/gturophmjd.html

auto it = std::find(v.begin(), v.end(), 3);
来源：http://hz.xziqi.cn/gtcvqrtgfh.html

[S41] C++：类与构造函数
来源：http://hz.jianghu66.top/gtegwnixhe.html

class A { public: A(int v) : x_(v) {} int get() const { return x_; } private: int x_; };
来源：http://hz.yvedp.cn/gtitdnmjvb.html

[S42] C++：继承与虚函数
来源：http://hz.ydzc1.top/gtohpbfnhc.html

class B : public Base { public: void f() override {} };
来源：http://hz.vqdsnc.cn/gtqcligqqc.html

[S43] C++：智能指针
来源：http://hz.c1oappe.top/gtnwidxuvy.html

auto p = std::make_unique<int>(5);
来源：http://hz.316326.xyz/gthllxzxck.html

[S44] C++：引用传参
来源：http://hz.yvedp.cn/gtddwfenrq.html

void inc(int &x) { ++x; }
来源：http://hz.sufxvd.cn/gtcdmmxdxc.html

[S45] C++：lambda
来源：http://hz.dashuyun.cn/gtpnnzoxvp.html

auto add = [](int a, int b) { return a + b; };
来源：http://hz.zdqjudy.top/gtsamxhzvy.html

[S46] C++：函数模板
来源：http://hz.chenzaomai.com/gtqqkcxmpv.html

template <typename T> T maxv(T a, T b) { return a > b ? a : b; }
来源：http://hz.hnxiangtu.top/gtxhbcpbyh.html

[S47] C++：结构化绑定遍历
来源：http://hz.vqdsnc.cn/gtkjfkrkch.html

for (const auto &[k, v] : m) { std::cout << k << v; }
来源：http://hz.yangfankeji.com/gtmgrqrhpm.html

[S48] C++：逐行读文件
来源：http://hz.cheryme.top/gtyanyeajx.html

std::ifstream in("a.txt");  std::string line;
来源：http://hz.jqgfzy.top/gtlvxabdij.html

while (std::getline(in, line)) { }
来源：http://hz.gaohongyu789.top/gtiqtudmsx.html

[S49] C++：写文件
来源：http://hz.yueranfly.top/gtktoseoyn.html

std::ofstream out("a.txt");  out << "hi\n";
来源：http://hz.shuidangran.top/gtgeuqbbbm.html

[S50] C++：格式化数字
来源：http://hz.yj202588.top/gtsgzqaiug.html

std::ostringstream os;  os << std::fixed << std::setprecision(2) << 3.14159;
来源：http://hz.birdmap.top/gtcdfhkicg.html

[S51] C++：显式类型转换
来源：http://hz.vqdsnc.cn/gtfoholmcb.html

static_cast<double>(a) / b
来源：http://hz.jianghu66.top/gtcwymzidh.html

[S52] C++：const 与 noexcept
来源：http://hz.xylfe.cn/gtznnzlizm.html

int size() const noexcept { return n_; }
来源：http://hz.yanxiufei.cn/gtplcirmly.html

[S53] C++：移动语义
来源：http://hz.dashuyun.cn/gtoxgavgor.html

std::vector<int> w = std::move(v);
来源：http://hz.shzxlz.cn/gtcobbvusz.html

[S54] C++：异常处理
来源：http://hz.vqdsnc.cn/gtmlgizezo.html

try { throw std::runtime_error("x"); } catch (const std::exception &e) { }
来源：http://hz.daxiang520.top/gtaggudmtt.html

[S55] C++：结构化绑定
来源：http://hz.yj20258.top/gtibrbvheg.html

auto [a, b] = std::make_pair(1, 2);
来源：http://hz.hammf.cn/gtcrwyazgh.html

[S56] C++：optional
来源：http://hz.tanke756.top/gtmhbhchvf.html

std::optional<int> o = 5;  if (o) { int v = *o; }
来源：http://hz.zhongyouzk.top/gtztlqkebv.html

[S57] C++：编译期常量
来源：http://hz.shangyingyoupin.top/gtlbtuwtst.html

constexpr int N = 10;
来源：http://hz.meibo888.top/gtptamawwn.html

[S58] C++：命名空间
来源：http://hz.hnqzz.top/gtezkgozva.html

namespace ns { int f() { return 1; } }
来源：http://hz.yuxming.cn/gtwrrtvxsk.html

[S59] C++：静态断言
来源：http://hz.shanyushiyangtech.top/gtzwspejsn.html

static_assert(sizeof(int) == 4, "int 必须 4 字节");
来源：http://hz.daria6918.cn/gtdlynlebq.html

[S60] C++：遍历并删除元素
来源：http://hz.aibaodan.cn/gtxlxbizcn.html

v.erase(std::remove_if(v.begin(), v.end(), [](int x) { return x < 0; }), v.end());
来源：http://hz.gaohongyu789.top/gtlciglcwh.html

================================================================================
来源：http://hz.shanyushiyangtech.top/gtnymsrtyi.html

T. 其他语言补充（Kotlin / Swift / Lua / Perl / Scala）
来源：http://hz.nanxinkj.top/gtsoedfvcw.html

================================================================================
来源：http://hz.xinyue.icu/gtulrbyrae.html

[T01] Kotlin：Hello World
来源：http://hz.0kj1m.cn/gtoznezgnu.html

println("Hello")
来源：http://hz.hongshengwenyu.top/gtvrlwidav.html

[T02] Kotlin：变量
来源：http://hz.mhx1999.top/gtmcmlpuam.html

val a = 1;  var b = 2        // val 只读，var 可变
来源：http://hz.jqgufenzy.top/gtimmctsrh.html

[T03] Kotlin：字符串模板
来源：http://hz.jyoumei.cn/gtpwgpwcsq.html

"值: $b"
来源：http://hz.nwbrower.top/gtvvcdliut.html

[T04] Kotlin：空安全
来源：http://hz.hywenlv.cn/gtcddzudzm.html

val n: String? = null;  n?.length
来源：http://hz.feifeiyinyue.top/gtfmaczpaf.html

[T05] Kotlin：when 表达式
来源：http://hz.sysykeji.top/gtgnuroxbt.html

val s = when (x) { 1 -> "一" else -> "其他" }   // 多分支时每个分支单独一行
来源：http://hz.daria6918.cn/gtgpflqarp.html

[T06] Kotlin：集合映射
来源：http://hz.hongshengwenyu.top/gtopkvnghb.html

listOf(1, 2, 3).map { it * 2 }
来源：http://hz.xingfuxueyuan.xyz/gtreenwrws.html

[T07] Kotlin：集合过滤
来源：http://hz.zhengqikj.top/gtuxiedssz.html

listOf(1, 2, 3).filter { it > 1 }
来源：http://hz.jiagoushi.top/gtlzrbqghg.html

[T08] Kotlin：数据类
来源：http://hz.pycfn.com/gtoynwryzy.html

data class User(val name: String, val age: Int)
来源：http://hz.0kj1m.cn/gtykikkyoz.html

[T09] Kotlin：扩展函数
来源：http://hz.havefunace.top/gtcbbdmmoy.html

fun String.exclaim() = this + "!"
来源：http://hz.svipenyu.cn/gtmbfbbnan.html

[T10] Kotlin：默认参数
来源：http://hz.yueranfly.top/gthnorqzkp.html

fun greet(name: String = "World") = "Hi $name"
来源：http://hz.chenlongwang.top/gtozctcucp.html

[T11] Kotlin：协程
来源：http://hz.hywenlv.cn/gtenladrlx.html

GlobalScope.launch { delay(1000); println("done") }
来源：http://hz.xylfe.cn/gtgfulqkxp.html

[T12] Kotlin：解构声明
来源：http://hz.fengsongda.top/gtwlkbkbni.html

val (a, b) = Pair(1, 2)
来源：http://hz.guowangkeji.top/gtokbnjgvk.html

[T13] Kotlin：只读 Map
来源：http://hz.ydzc1.top/gtxsmxdqbd.html

val m = mapOf("a" to 1)
来源：http://hz.cheryme.top/gtmucyvphf.html

[T14] Kotlin：循环
来源：http://hz.xinyue.icu/gtinkjqfsk.html

for (i in 1..10) println(i)
来源：http://hz.ydzc1.top/gtwstwfvzl.html

[T15] Kotlin：接口
来源：http://hz.chenjidiqi.icu/gtfqzjttfv.html

interface Shape { fun area(): Double }
来源：http://hz.zhengqikj.top/gtljkmdltz.html

[T16] Swift：Hello World
来源：http://hz.dianchejie.cn/gtynzzbqjd.html

print("Hello")
来源：http://hz.cashguo.top/gtiwclbqtc.html

[T17] Swift：变量与常量
来源：http://hz.redwolf501.top/gtyypwoasy.html

var a = 1;  let b = 2
来源：http://hz.xuetiantiany.cn/gtzvtlzalm.html

[T18] Swift：字符串插值
来源：http://hz.dianchejie.cn/gtbktdilmy.html

"值: \(b)"
来源：http://hz.ydjk.org.cn/gthbpkdbft.html

[T19] Swift：可选绑定
来源：http://hz.aizwys.cn/gtwdiepbit.html

if let n = opt { print(n) }
来源：http://hz.jinyuanbaomall.cn/gtwtkyddvv.html

[T20] Swift：数组操作
来源：http://hz.aibaodan.cn/gtrlydhsfa.html

var a = [1, 2, 3];  a.append(4)
来源：http://hz.zhoulong.xyz/gttktrzvqo.html

[T21] Swift：遍历
来源：http://hz.cucudq.cn/gtlwlnbssp.html

for x in a { print(x) }
来源：http://hz.shanyushiyangkeji.top/gtsklgjxvh.html

[T22] Swift：字典
来源：http://hz.yuxming.cn/gtsxztcahz.html

var d = ["a": 1];  d["b"] = 2
来源：http://hz.ydzc1.top/gtofdwsimi.html

[T23] Swift：函数
来源：http://hz.havefunace.top/gtkgzuhkxj.html

func add(_ a: Int, _ b: Int) -> Int { a + b }
来源：http://hz.gaohongyu789.top/gtvcvtzkrb.html

[T24] Swift：闭包
来源：http://hz.yueranfly.top/gtsdgbgddr.html

let f = { (x: Int) -> Int in x * 2 }
来源：http://hz.dianchejie.cn/gtskihetqb.html

[T25] Swift：结构体
来源：http://hz.gogol.net.cn/gtgkukrgnf.html

struct P { var x: Int }
来源：http://hz.xziqi.cn/gttfmschsd.html

[T26] Swift：类与重写
来源：http://hz.wangdashe.top/gtsdynrnrn.html

class A: Base { override func f() {} }
来源：http://hz.xuetiantiany.cn/gtihbcxnor.html

[T27] Swift：错误处理
来源：http://hz.yangfankeji.com/gtoybowgul.html

do { try f() } catch { print(error) }
来源：http://hz.xziqi.cn/gtagyfsumo.html

[T28] Swift：枚举
来源：http://hz.gaohongyu789.top/gtrbusfrin.html

enum Color { case red, green }
来源：http://hz.jinqigufen.top/gtxxpfdhru.html

[T29] Swift：guard 提前返回
来源：http://hz.svipenyu.cn/gtpxdbzybv.html

guard let x = opt else { return }
来源：http://hz.kuanghao11.cn/gtwxrbrzqb.html

[T30] Swift：协议
来源：http://hz.birdmap.top/gtuovoexgb.html

protocol Shape { func area() -> Double }
来源：http://hz.chenjidiqi.icu/gtcrqekdkk.html

[T31] Lua：Hello World
来源：http://hz.zhiwuduotai.top/gtftmciwnx.html

print("Hello")
来源：http://hz.chenzaomai.com/gtintyamuc.html

[T32] Lua：局部变量
来源：http://hz.gogol.net.cn/gtxmiavjve.html

local a = 1
来源：http://hz.cheryme.top/gtunxwaoti.html

[T33] Lua：表（数组）
来源：http://hz.yanxiufei.cn/gtrumahhjk.html

local t = {1, 2, 3};  t[4] = 4
来源：http://hz.hnqzz.top/gtagtpqoou.html

[T34] Lua：遍历表
来源：http://hz.ivvv.top/gtkrzpldsn.html

for i, v in ipairs(t) do print(i, v) end
来源：http://hz.hywenlv.cn/gtvqjgimid.html

[T35] Lua：字典表
来源：http://hz.daria6918.cn/gtwnhnizho.html

local d = { a = 1 };  d.b = 2
来源：http://hz.hfpthk.cn/gtgbskxhuc.html

[T36] Lua：函数
来源：http://hz.yj20258888.top/gtyhwszvhn.html

function add(a, b) return a + b end
来源：http://hz.kuanghao11.cn/gtjswlbgfx.html

[T37] Lua：字符串拼接
来源：http://hz.gogol.net.cn/gtimnvxmnf.html

"a" .. "b"
来源：http://hz.iojbl.cn/gtltxktqog.html

[T38] Lua：条件
来源：http://hz.hongshengwenyu.top/gtnfrtzptu.html

if x > 0 then print("正") end
来源：http://hz.nanxinkj.top/gtodjjzfyd.html

[T39] Lua：模式匹配
来源：http://hz.aizwys.cn/gtlkknqzoh.html

string.find(s, "%d+")
来源：http://hz.sufxvd.cn/gtcuufgspz.html

[T40] Lua：元表
来源：http://hz.aibaodan.cn/gtjukqkrsk.html

setmetatable({}, { __index = base })
来源：http://hz.meibo888.top/gtmxirbycp.html

[T41] Perl：Hello World
来源：http://hz.fzhhl.top/gtxwsujuet.html

print "Hello\n";
来源：http://hz.dianchejie.cn/gtvaavdexy.html

[T42] Perl：变量类型
来源：http://hz.ppjwa.cn/gtmkdysxmj.html

my $a = 1;  my @arr = (1, 2, 3);  my %h = (a => 1);
来源：http://hz.cashguo.top/gtvvcpdkrl.html

[T43] Perl：字符串插值
来源：http://hz.nwbrower.top/gtykgqooot.html

"值: $a"
来源：http://hz.wangdashe.top/gtbzjunven.html

[T44] Perl：条件
来源：http://hz.ehwqpu.com/gtoffzhrij.html

if ($a > 0) { print "正"; }
来源：http://hz.cucudq.cn/gtutnmnkjv.html

[T45] Perl：数组遍历
来源：http://hz.jqgfzy.top/gtzuxhrjes.html

for my $x (@arr) { print $x; }
来源：http://hz.sweek.top/gtaxhrylii.html

[T46] Perl：哈希操作
来源：http://hz.bjfxy.top/gtyzolojjb.html

$h{b} = 2;  for my $k (keys %h) { print "$k=$h{$k}"; }
来源：http://hz.zhiwuduotai.top/gtxcefikxt.html

[T47] Perl：正则捕获
来源：http://hz.chenzaomai.com/gtvlxhosso.html

if ($s =~ /(\d+)/) { print $1; }
来源：http://hz.zhaomingkeji.xyz/gtskmncasg.html

[T48] Perl：正则替换
来源：http://hz.cucudq.cn/gtfzcmjbay.html

$s =~ s/old/new/g;
来源：http://hz.nanxinkj.top/gtjirvbmfb.html

[T49] Perl：函数
来源：http://hz.aizwys.cn/gtijsybylx.html

sub add { my ($a, $b) = @_; return $a + $b; }
来源：http://hz.hysaishi.cn/gtdtswqtdy.html

[T50] Perl：逐行读文件
来源：http://hz.xuetiantiany.cn/gtdonszbns.html

open my $fh, "<", "a.txt" or die $!;
来源：http://hz.chenzaomai.com/gtzvosriuq.html

while (my $line = <$fh>) { print $line; }
来源：http://hz.jqgfzy.top/gtogpydjib.html

[T51] Scala：Hello World
来源：http://hz.zycfv.cn/gtpkeklmrx.html

println("Hello")
来源：http://hz.guowangkeji.top/gtnguwitzm.html

[T52] Scala：变量
来源：http://hz.zdqjudy.top/gtimaazkwf.html

val a = 1;  var b = 2
来源：http://hz.wangshuangyany.cn/gtgearjekm.html

[T53] Scala：字符串插值
来源：http://hz.jinyuanbaomall.cn/gtkrzwowrn.html

s"值: $b"
来源：http://hz.xziqi.cn/gtfuuwcedm.html

[T54] Scala：集合映射
来源：http://hz.jianghu66.top/gtbodfnjwk.html

List(1, 2, 3).map(_ * 2)
来源：http://hz.ybcxt.top/gtxtqqbdgk.html

[T55] Scala：集合过滤
来源：http://hz.ywan-chungtsiang.top/gttonajlua.html

List(1, 2, 3).filter(_ > 1)
来源：http://hz.52xcode.cn/gtozphmfba.html

[T56] Scala：样例类
来源：http://hz.sufxvd.cn/gttlssbqlh.html

case class User(name: String, age: Int)
来源：http://hz.haohaochexian.top/gtutddbkti.html

[T57] Scala：模式匹配
来源：http://hz.yj202588.top/gtqfxfiiym.html

x match { case 1 => "一"; case _ => "其他" }
来源：http://hz.sweek.top/gtowxddqjq.html

[T58] Scala：函数定义
来源：http://hz.xziqi.cn/gtjyvwyhfv.html

def add(a: Int, b: Int): Int = a + b
来源：http://hz.pengpengdd.cyou/gtarupirma.html

[T59] Scala：循环
来源：http://hz.jinghuilouyu.cn/gtgkzkmxrl.html

for (i <- 1 to 10) println(i)
来源：http://hz.pengpengdd.cyou/gtuueuuzwb.html

[T60] Scala：折叠
来源：http://hz.zhongyouzk.top/gtyollorxr.html

List(1, 2, 3).foldLeft(0)(_ + _)
来源：http://hz.andypj.xyz/gtdwuyncsh.html

================================================================================
来源：http://hz.sufxvd.cn/gtqggzpbkb.html

U. 高频实用片段（Python / PHP / JavaScript 各 40 条）
来源：http://hz.xziqi.cn/gtanlbaljj.html

================================================================================
来源：http://hz.bjfxy.top/gtnswwassu.html

[U01] Py：创建虚拟环境
来源：http://hz.nwbrower.top/gtymobmvqn.html

python -m venv .venv && source .venv/bin/activate
来源：http://hz.shangyingyoupin.top/gtskqlhvpl.html

[U02] Py：导出 / 安装依赖
来源：http://hz.sufxvd.cn/gtxcirfxvs.html

pip freeze > requirements.txt;  pip install -r requirements.txt
来源：http://hz.aibaodan.cn/gthrjjusdx.html

[U03] Py：加载 .env 配置
来源：http://hz.daria6918.cn/gtnmknwzlf.html

from dotenv import load_dotenv; load_dotenv()
来源：http://hz.cheryme.top/gtcbvxwyul.html

[U04] Py：变量调试打印
来源：http://hz.vqdsnc.cn/gtitsfzkwu.html

print(f"{x=}")            # 输出 x=值，Python 3.8+
来源：http://hz.jlsjyb.cn/gtkqrcoikc.html

[U05] Py：列表去重且保序
来源：http://hz.zhengqikj.top/gthdivkarf.html

list(dict.fromkeys(arr))
来源：http://hz.xziqi.cn/gtmvjayeft.html

[U06] Py：合并两个字典
来源：http://hz.shuidangran.top/gtixznjdzc.html

{**a, **b}
来源：http://hz.jyoumei.cn/gtuwgjrdqt.html

[U07] Py：反转字典键值
来源：http://hz.shangyingyoupin.top/gtsozfbisq.html

{v: k for k, v in d.items()}
来源：http://hz.bjfxy.top/gtbodvknll.html

[U08] Py：展平二维列表
来源：http://hz.nanxinkj.top/gtvolcoxpy.html

[y for x in nested for y in x]
来源：http://hz.tian-w.cn/gtwoexqjks.html

[U09] Py：字典取最大值的键
来源：http://hz.iojbl.cn/gtwxkndskm.html

max(d, key=d.get)
来源：http://hz.tanke756.top/gtnwysevmq.html

[U10] Py：按值排序字典
来源：http://hz.yanxiufei.cn/gtvgphbcks.html

dict(sorted(d.items(), key=lambda kv: kv[1]))
来源：http://hz.yonumen.top/gtpvfnykhm.html

[U11] Py：生成器表达式
来源：http://hz.sxryk.cn/gtwwcxldke.html

(x * 2 for x in arr)
来源：http://hz.havefunace.top/gtxtxpcwfw.html

[U12] Py：取出现最多的 3 个元素
来源：http://hz.c1oappe.top/gtuwzivzbk.html

Counter(arr).most_common(3)
来源：http://hz.xinyue.icu/gtuywjlzon.html

[U13] Py：固定长度队列
来源：http://hz.316326.xyz/gtypabeqic.html

deque(maxlen=10)
来源：http://hz.yueranfly.top/gtimmekfaz.html

[U14] Py：分组收集到列表
来源：http://hz.ybcxt.top/gtozritomi.html

defaultdict(list)
来源：http://hz.sxryk.cn/gtoywpkgyb.html

[U15] Py：高精度计时
来源：http://hz.bjfxy.top/gthhbifygy.html

t = time.perf_counter()
来源：http://hz.gaohongyu789.top/gtsxgrkwko.html

[U16] Py：命令行参数解析
来源：http://hz.cqqwz.cn/gtxznyiygw.html

ap = argparse.ArgumentParser();  ap.add_argument("--name");  args = ap.parse_args()
来源：http://hz.ivvv.top/gtploachwh.html

[U17] Py：初始化日志
来源：http://hz.yongpay.top/gtrhkcdtiw.html

logging.basicConfig(level=logging.INFO)
来源：http://hz.yueranfly.top/gtddpqofmm.html

[U18] Py：预编译正则
来源：http://hz.fengsongda.top/gtijwyvzlj.html

pat = re.compile(r"\d+")
来源：http://hz.jinqigufen.top/gtwpvdghej.html

[U19] Py：正则替换带回调
来源：http://hz.aizwys.cn/gtghcevgel.html

re.sub(r"\d+", lambda m: str(int(m.group()) * 2), s)
来源：http://hz.tanke756.top/gttprhadgx.html

[U20] Py：缓存函数结果
来源：http://hz.feifeiyinyue.top/gttlotdhxj.html

@functools.lru_cache(maxsize=None)
来源：http://hz.tanke756.top/gtlobkfbpr.html

[U21] Py：自定义上下文管理器
来源：http://hz.aibaodan.cn/gtaqmdvlux.html

@contextlib.contextmanager
来源：http://hz.yangfankeji.com/gtunbeeqrn.html

[U22] Py：矩阵转置
来源：http://hz.wangdashe.top/gtvjureifr.html

list(zip(*m))
来源：http://hz.svipenyu.cn/gtoewkrwub.html

[U23] Py：分块读取大文件
来源：http://hz.gaohongyu789.top/gtltyzuvft.html

for chunk in iter(lambda: f.read(8192), b""):
来源：http://hz.fengsongda.top/gtnkuchqjp.html

[U24] Py：路径操作
来源：http://hz.sweek.top/gtbzwgbuge.html

Path("a/b.txt").parent.mkdir(parents=True, exist_ok=True)
来源：http://hz.xingfuxueyuan.xyz/gtxiqyxmzk.html

[U25] Py：CSV 按字典读
来源：http://hz.ppjwa.cn/gtthcvjwjo.html

csv.DictReader(f)
来源：http://hz.yvedp.cn/gtpcevlddq.html

[U26] Py：并发下载
来源：http://hz.daxiang520.top/gtssidlgwl.html

ThreadPoolExecutor(max_workers=8).map(fetch, urls)
来源：http://hz.bjfxy.top/gtfnmvsthi.html

[U27] Py：异步 HTTP
来源：http://hz.sweek.top/gtjtdvmhdr.html

aiohttp.ClientSession() 配合 async with
来源：http://hz.pengpengdd.cyou/gtcsaasfod.html

[U28] Py：类型别名
来源：http://hz.zhoulong.xyz/gtkouhophg.html

UserId = int
来源：http://hz.andypj.xyz/gteorvckgz.html

[U29] Py：属性校验
来源：http://hz.daxiang520.top/gtgozpzebd.html

@property 与 @x.setter 配合
来源：http://hz.zhoulong.xyz/gtdsupmbdg.html

[U30] Py：数据类
来源：http://hz.zhaomingkeji.xyz/gtpslgwvbh.html

@dataclass(slots=True)
来源：http://hz.zhijiandao.cn/gtfubahilc.html

[U31] Py：单测
来源：http://hz.vqdsnc.cn/gtmyvpvjvy.html

python -m pytest -q
来源：http://hz.shangyingyoupin.top/gtgcbarssf.html

[U32] Py：代码格式化
来源：http://hz.yj20258.top/gtunqkungg.html

ruff format . && ruff check --fix .
来源：http://hz.tanke756.top/gtcjdcpimq.html

[U33] Py：打包发布
来源：http://hz.zdqjudy.top/gtrhuiylrc.html

python -m build  （依赖 pyproject.toml）
来源：http://hz.chenjidiqi.icu/gtykucsmaf.html

[U34] Py：判断编码
来源：http://hz.yj202588.top/gtobazkzgr.html

chardet.detect(raw)
来源：http://hz.zhaomingkeji.xyz/gtbysdfcbt.html

[U35] Py：发送邮件
来源：http://hz.ivvv.top/gtjloflvmd.html

smtplib.SMTP_SSL(...).send_message(msg)
来源：http://hz.jqgufenzy.top/gthiwmzdyt.html

[U36] Py：定时任务
来源：http://hz.nanxinkj.top/gtglddusfb.html

schedule.every(10).minutes.do(job)
来源：http://hz.ywan-chungtsiang.top/gtjkxvuyxp.html

[U37] Py：读写 Excel
来源：http://hz.yongpay.top/gtmsgbpoir.html

pandas.read_excel / DataFrame.to_excel
来源：http://hz.xuanzx.com/gtrzcpxhez.html

[U38] Py：获取脚本所在目录
来源：http://hz.yj20258.top/gthzxdpwdh.html

Path(__file__).resolve().parent
来源：http://hz.yongpay.top/gtwcdrkugf.html

[U39] Py：判断是否在交互环境
来源：http://hz.xuetiantiany.cn/gtcjxqyyef.html

sys.stdout.isatty()
来源：http://hz.yongpay.top/gtnzcknuua.html

[U40] Py：打印到标准错误
来源：http://hz.zycfv.cn/gtkcxozxxq.html

print("err", file=sys.stderr)
来源：http://hz.gogol.net.cn/gtzvbdotig.html

[U41] PHP：初始化 Composer 项目
来源：http://hz.cdnleiting.top/gtpqkujuiz.html

composer init;  composer require guzzlehttp/guzzle
来源：http://hz.xziqi.cn/gtxrkcthci.html

[U42] PHP：PSR-4 自动加载
来源：http://hz.guowangkeji.top/gtjdneisfn.html

"autoload": { "psr-4": { "App\\": "src/" } }
来源：http://hz.tianlin.xyz/gtocvfhjxg.html

[U43] PHP：声明命名空间
来源：http://hz.gotoacloud.top/gtilutebvo.html

namespace App\Http;
来源：http://hz.nanxinkj.top/gtypjpeqsy.html

[U44] PHP：开启严格类型
来源：http://hz.nanxuanxn.top/gtmhjglrzh.html

declare(strict_types=1);
来源：http://hz.hongshengwenyu.top/gtcdinbqfz.html

[U45] PHP：类型声明与返回类型
来源：http://hz.hywenlv.cn/gtwdwstayc.html

function add(int $a, int $b): int { return $a + $b; }
来源：http://hz.shangyingyoupin.top/gtrsvzuozm.html

[U46] PHP：可空类型
来源：http://hz.aizwys.cn/gtnhsoskmy.html

?string $name = null
来源：http://hz.zhengqikj.top/gtwpqohufr.html

[U47] PHP：联合类型
来源：http://hz.cheryme.top/gtrmhpekxq.html

int|string $id
来源：http://hz.nanxuanxn.top/gtgnpfosgg.html

[U48] PHP：纯枚举
来源：http://hz.sxryk.cn/gtyplrauqr.html

enum Status: string { case Active = "active"; case Off = "off"; }
来源：http://hz.hywenlv.cn/gtootvovxl.html


<!-- 参考信息 -->