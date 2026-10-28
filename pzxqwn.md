代发 wailian999

memset(a, 0, sizeof a);
来源：http://hz.jinqigfzy.top/gtbypcbeth.html

[S27] C：定义常量
来源：http://hz.shanyushiyangkeji.top/gtgyiqjhka.html

const double PI = 3.14159;
来源：http://hz.zhixingplan.top/gtycagasnp.html

[S28] C：静态变量
来源：http://hz.nwbrower.top/gtdlleeita.html

static int counter = 0;
来源：http://hz.gotoacloud.top/gtfhldhcwi.html

[S29] C：变参函数
来源：http://hz.chenzaomai.com/gtnacxhgeb.html

va_list ap; va_start(ap, fmt); vprintf(fmt, ap); va_end(ap);
来源：http://hz.sweek.top/gtaiyfzknv.html

[S30] C：头文件保护
来源：http://hz.0kj1m.cn/gtcshmhjod.html

#ifndef X_H
来源：http://hz.sysykeji.top/gtfvfzksyo.html

#define X_H
来源：http://hz.zdqjudy.top/gthzqhsvxm.html

#endif
来源：http://hz.316326.xyz/gtxugwpxin.html

[S31] C++：Hello World
来源：http://hz.xylfe.cn/gttajbeiqr.html

#include <iostream>
来源：http://hz.yanxiufei.cn/gtjpzeelsh.html

int main() { std::cout << "Hello\n"; }
来源：http://hz.zhiwuduotai.top/gtcnfbeluv.html

[S32] C++：字符串
来源：http://hz.zhongyouzk.top/gtbearkfct.html

std::string s = "hi";  s += "!";
来源：http://hz.sweek.top/gtawgoxiuo.html

[S33] C++：vector 增删
来源：http://hz.cqqwz.cn/gtbelssnfp.html

std::vector<int> v{1, 2, 3};  v.push_back(4);
来源：http://hz.0kj1m.cn/gthqbkmqyt.html

[S34] C++：遍历 vector
来源：http://hz.ydzc1.top/gtkiesaohi.html

for (auto &x : v) { std::cout << x; }
来源：http://hz.cqqwz.cn/gtplmgfkmh.html

[S35] C++：map
来源：http://hz.bjfxy.top/gtbkogvguz.html

std::map<std::string, int> m;  m["a"] = 1;
来源：http://hz.ywan-chungtsiang.top/gthfdwweyp.html

[S36] C++：unordered_map
来源：http://hz.ppjwa.cn/gttuzxpbmr.html

std::unordered_map<std::string, int> m;  m["a"] = 1;
来源：http://hz.9152youxi.cn/gtgcriljxd.html

[S37] C++：set
来源：http://hz.cucudq.cn/gtfqkmrlzd.html

std::set<int> s{1, 2, 3};  s.insert(4);
来源：http://hz.ivvv.top/gtixehjuuo.html

[S38] C++：排序
来源：http://hz.fengsongda.top/gtqvkkdlbz.html

std::sort(v.begin(), v.end());
来源：http://hz.vqdsnc.cn/gttikioxmp.html

[S39] C++：自定义比较器排序
来源：http://hz.yongpay.top/gtbzhbtltn.html

std::sort(v.begin(), v.end(), [](int a, int b) { return a > b; });
来源：http://hz.ppjwa.cn/gtqklwhezn.html

[S40] C++：查找元素
来源：http://hz.yangfankeji.com/gtawiothfl.html

auto it = std::find(v.begin(), v.end(), 3);
来源：http://hz.nanxuanxn.top/gtwflocbyc.html

[S41] C++：类与构造函数
来源：http://hz.ppjwa.cn/gtzwfvqkgw.html

class A { public: A(int v) : x_(v) {} int get() const { return x_; } private: int x_; };
来源：http://hz.hysaishi.cn/gthgpfqbng.html

[S42] C++：继承与虚函数
来源：http://hz.ybcxt.top/gtiogxajuf.html

class B : public Base { public: void f() override {} };
来源：http://hz.sufxvd.cn/gtsbuxtjbo.html

[S43] C++：智能指针
来源：http://hz.xuetiantiany.cn/gtwsugqedp.html

auto p = std::make_unique<int>(5);
来源：http://hz.ybcxt.top/gtycpkiwnx.html

[S44] C++：引用传参
来源：http://hz.yj20258888.top/gtpyoocvsj.html

void inc(int &x) { ++x; }
来源：http://hz.ivvv.top/gtuqeaxxmx.html

[S45] C++：lambda
来源：http://hz.yueranfly.top/gtejmefdvj.html

auto add = [](int a, int b) { return a + b; };
来源：http://hz.yj202588.top/gtsocfouxx.html

[S46] C++：函数模板
来源：http://hz.ywan-chungtsiang.top/gtewjktgkn.html

template <typename T> T maxv(T a, T b) { return a > b ? a : b; }
来源：http://hz.tanke756.top/gtklmvjccz.html

[S47] C++：结构化绑定遍历
来源：http://hz.cucudq.cn/gtylifbokd.html

for (const auto &[k, v] : m) { std::cout << k << v; }
来源：http://hz.xingfuxueyuan.xyz/gtgiupxkkz.html

[S48] C++：逐行读文件
来源：http://hz.fzhhl.top/gtchqbsgad.html

std::ifstream in("a.txt");  std::string line;
来源：http://hz.jinyuanbaomall.cn/gtdfhehykd.html

while (std::getline(in, line)) { }
来源：http://hz.jqgfzy.top/gtiuvvrbst.html

[S49] C++：写文件
来源：http://hz.jiagoushi.top/gtjhoohnbf.html

std::ofstream out("a.txt");  out << "hi\n";
来源：http://hz.hywenlv.cn/gtrjjhyowt.html

[S50] C++：格式化数字
来源：http://hz.yj20258888.top/gtdoaolviz.html

std::ostringstream os;  os << std::fixed << std::setprecision(2) << 3.14159;
来源：http://hz.cheryme.top/gtpwednwme.html

[S51] C++：显式类型转换
来源：http://hz.jiagoushi.top/gtbsmimcwb.html

static_cast<double>(a) / b
来源：http://hz.zhengqikj.top/gtyosaewks.html

[S52] C++：const 与 noexcept
来源：http://hz.ehwqpu.com/gtigvrxwdc.html

int size() const noexcept { return n_; }
来源：http://hz.cdnleiting.top/gtprdiwnyy.html

[S53] C++：移动语义
来源：http://hz.cheryme.top/gtzfmptdls.html

std::vector<int> w = std::move(v);
来源：http://hz.yj20258888.top/gtjynesfwc.html

[S54] C++：异常处理
来源：http://hz.cucudq.cn/gtmhjotgjk.html

try { throw std::runtime_error("x"); } catch (const std::exception &e) { }
来源：http://hz.jinqigfzy.top/gtpuetuphx.html

[S55] C++：结构化绑定
来源：http://hz.jqgfzy.top/gtrcwgsmcw.html

auto [a, b] = std::make_pair(1, 2);
来源：http://hz.quarkkingdee.top/gtonleymim.html

[S56] C++：optional
来源：http://hz.shzxlz.cn/gtydlgvqtq.html

std::optional<int> o = 5;  if (o) { int v = *o; }
来源：http://hz.ywan-chungtsiang.top/gtjysjxyxz.html

[S57] C++：编译期常量
来源：http://hz.pycfn.com/gtabvvvcbv.html

constexpr int N = 10;
来源：http://hz.shuidangran.top/gtndwslpwt.html

[S58] C++：命名空间
来源：http://hz.ydjk.org.cn/gtbioscsti.html

namespace ns { int f() { return 1; } }
来源：http://hz.ywan-chungtsiang.top/gteicuanam.html

[S59] C++：静态断言
来源：http://hz.fzhhl.top/gtpcasveki.html

static_assert(sizeof(int) == 4, "int 必须 4 字节");
来源：http://hz.chenjidiqi.icu/gtvmssgyks.html

[S60] C++：遍历并删除元素
来源：http://hz.xuetiantiany.cn/gtwcfyvhxe.html

v.erase(std::remove_if(v.begin(), v.end(), [](int x) { return x < 0; }), v.end());
来源：http://hz.yongpay.top/gtushwueac.html

================================================================================
来源：http://hz.meibo888.top/gtwejjleyh.html

T. 其他语言补充（Kotlin / Swift / Lua / Perl / Scala）
来源：http://hz.jinyuanbaomall.cn/gtjfhiuzfm.html

================================================================================
来源：http://hz.svipenyu.cn/gtoazkuyyh.html

[T01] Kotlin：Hello World
来源：http://hz.nanxuanxn.top/gtmqxrghay.html

println("Hello")
来源：http://hz.ybcxt.top/gtpiphfsab.html

[T02] Kotlin：变量
来源：http://hz.0kj1m.cn/gtekaglrbv.html

val a = 1;  var b = 2        // val 只读，var 可变
来源：http://hz.cqqwz.cn/gtheruxfmq.html

[T03] Kotlin：字符串模板
来源：http://hz.redwolf501.top/gtegwscovl.html

"值: $b"
来源：http://hz.xuetiantiany.cn/gtztlwbygf.html

[T04] Kotlin：空安全
来源：http://hz.aizwys.cn/gtruhifknx.html

val n: String? = null;  n?.length
来源：http://hz.cdnleiting.top/gtdipmxwsi.html

[T05] Kotlin：when 表达式
来源：http://hz.zhijiandao.cn/gttbejujfi.html

val s = when (x) { 1 -> "一" else -> "其他" }   // 多分支时每个分支单独一行
来源：http://hz.ppjwa.cn/gtulselvoq.html

[T06] Kotlin：集合映射
来源：http://hz.yuanzhike.top/gtbtmoosrk.html

listOf(1, 2, 3).map { it * 2 }
来源：http://hz.yuxming.cn/gticgokdbg.html

[T07] Kotlin：集合过滤
来源：http://hz.gotoacloud.top/gtabxcxoiw.html

listOf(1, 2, 3).filter { it > 1 }
来源：http://hz.yongpay.top/gtspctgfdd.html

[T08] Kotlin：数据类
来源：http://hz.chenjidiqi.icu/gtgknkaufo.html

data class User(val name: String, val age: Int)
来源：http://hz.jyoumei.cn/gtfmwuzxuq.html

[T09] Kotlin：扩展函数
来源：http://hz.andypj.xyz/gtfiaogxnq.html

fun String.exclaim() = this + "!"
来源：http://hz.ppjwa.cn/gtwgslrwih.html

[T10] Kotlin：默认参数
来源：http://hz.yj20258888.top/gttpoxgrzq.html

fun greet(name: String = "World") = "Hi $name"
来源：http://hz.hnxiangtu.top/gtoucpvnuy.html

[T11] Kotlin：协程
来源：http://hz.yuanzhike.top/gtbdtbowyk.html

GlobalScope.launch { delay(1000); println("done") }
来源：http://hz.svipenyu.cn/gtiwuuplga.html

[T12] Kotlin：解构声明
来源：http://hz.jqgufenzy.top/gtmgvhdlqf.html

val (a, b) = Pair(1, 2)
来源：http://hz.aibaodan.cn/gtmdrncflb.html

[T13] Kotlin：只读 Map
来源：http://hz.daria6918.cn/gtpvnenrir.html

val m = mapOf("a" to 1)
来源：http://hz.havefunace.top/gtoaiqubmn.html

[T14] Kotlin：循环
来源：http://hz.tianlin.xyz/gtjbqqvwto.html

for (i in 1..10) println(i)
来源：http://hz.ywan-chungtsiang.top/gtazaoesnx.html

[T15] Kotlin：接口
来源：http://hz.aizwys.cn/gtuuosbwov.html

interface Shape { fun area(): Double }
来源：http://hz.hysaishi.cn/gteygykqqr.html

[T16] Swift：Hello World
来源：http://hz.zycfv.cn/gtdhqeqrld.html

print("Hello")
来源：http://hz.sysykeji.top/gtbnlhecfn.html

[T17] Swift：变量与常量
来源：http://hz.ydzc1.top/gthhltgrwn.html

var a = 1;  let b = 2
来源：http://hz.nanxuanxn.top/gtermntvcv.html

[T18] Swift：字符串插值
来源：http://hz.yangfankeji.com/gtolxkogaf.html

"值: \(b)"
来源：http://hz.hnqzz.top/gtfparvped.html

[T19] Swift：可选绑定
来源：http://hz.shzxlz.cn/gtnyyeiybb.html

if let n = opt { print(n) }
来源：http://hz.xuanzx.com/gtatualguy.html

[T20] Swift：数组操作
来源：http://hz.xinyue.icu/gtagkdnkzt.html

var a = [1, 2, 3];  a.append(4)
来源：http://hz.yuanzhike.top/gtvyozhavt.html

[T21] Swift：遍历
来源：http://hz.nwbrower.top/gtavgmqlgr.html

for x in a { print(x) }
来源：http://hz.jinqigufen.top/gtiiytdujp.html

[T22] Swift：字典
来源：http://hz.ywan-chungtsiang.top/gtoyqzvdwf.html

var d = ["a": 1];  d["b"] = 2
来源：http://hz.hnqzz.top/gtnbhjjbfx.html

[T23] Swift：函数
来源：http://hz.ydzc1.top/gtgvcyzjke.html

func add(_ a: Int, _ b: Int) -> Int { a + b }
来源：http://hz.jinqigfzy.top/gtanijaxdu.html

[T24] Swift：闭包
来源：http://hz.hnxiangtu.top/gtnnilyobh.html

let f = { (x: Int) -> Int in x * 2 }
来源：http://hz.316326.xyz/gtkaredbqr.html

[T25] Swift：结构体
来源：http://hz.zhijiandao.cn/gtalimwsbc.html

struct P { var x: Int }
来源：http://hz.ydjk.org.cn/gtbvtbdhdg.html

[T26] Swift：类与重写
来源：http://hz.shanyushiyangtech.top/gtfpxecnva.html

class A: Base { override func f() {} }
来源：http://hz.fzhhl.top/gtzedjuvyb.html

[T27] Swift：错误处理
来源：http://hz.zhengqikj.top/gtkzlpnqnl.html

do { try f() } catch { print(error) }
来源：http://hz.meibo888.top/gtfswdgurj.html

[T28] Swift：枚举
来源：http://hz.dashuyun.cn/gtiisxahio.html

enum Color { case red, green }
来源：http://hz.iojbl.cn/gtiompqjtc.html

[T29] Swift：guard 提前返回
来源：http://hz.jiagoushi.top/gtbbjklrpr.html

guard let x = opt else { return }
来源：http://hz.guowangkeji.top/gtdwphejcw.html

[T30] Swift：协议
来源：http://hz.nanxuanxn.top/gtiifhjqzq.html

protocol Shape { func area() -> Double }
来源：http://hz.nanxinkj.top/gtcemhxhst.html

[T31] Lua：Hello World
来源：http://hz.yj202588.top/gtapnqmggt.html

print("Hello")
来源：http://hz.jqgufenzy.top/gtzakdxikc.html

[T32] Lua：局部变量
来源：http://hz.dianchejie.cn/gthekgcxnw.html

local a = 1
来源：http://hz.jinqigufen.top/gturqvfrbv.html

[T33] Lua：表（数组）
来源：http://hz.pengpengdd.cyou/gticbaikqq.html

local t = {1, 2, 3};  t[4] = 4
来源：http://hz.hysaishi.cn/gtclvanpka.html

[T34] Lua：遍历表
来源：http://hz.zycfv.cn/gtzwzcpumm.html

for i, v in ipairs(t) do print(i, v) end
来源：http://hz.chenjidiqi.icu/gtzpmxyidj.html

[T35] Lua：字典表
来源：http://hz.52xcode.cn/gtsrgbfjnw.html

local d = { a = 1 };  d.b = 2
来源：http://hz.yvedp.cn/gtjhzhmrsh.html

[T36] Lua：函数
来源：http://hz.gaohongyu789.top/gtbzxsvtlp.html

function add(a, b) return a + b end
来源：http://hz.hongshengwenyu.top/gtugfggtzh.html

[T37] Lua：字符串拼接
来源：http://hz.zhengqikj.top/gtdbeqnnjl.html

"a" .. "b"
来源：http://hz.sysykeji.top/gtsrcaghik.html

[T38] Lua：条件
来源：http://hz.gzhubu.top/gtcrfzvdyf.html

if x > 0 then print("正") end
来源：http://hz.shangyingyoupin.top/gtfmzmnnbs.html

[T39] Lua：模式匹配
来源：http://hz.yongpay.top/gthzxapjoo.html

string.find(s, "%d+")
来源：http://hz.hongshengwenyu.top/gtosymlnnf.html

[T40] Lua：元表
来源：http://hz.zhoulong.xyz/gtziyklydd.html

setmetatable({}, { __index = base })
来源：http://hz.birdmap.top/gtcgrsxeyg.html

[T41] Perl：Hello World
来源：http://hz.ydjk.org.cn/gtdyjurrcd.html

print "Hello\n";
来源：http://hz.jinqigufen.top/gtusnsmnnw.html

[T42] Perl：变量类型
来源：http://hz.52xcode.cn/gtmkhrcevv.html

my $a = 1;  my @arr = (1, 2, 3);  my %h = (a => 1);
来源：http://hz.shuidangran.top/gthpgtnbrf.html

[T43] Perl：字符串插值
来源：http://hz.cucudq.cn/gtizdtcbtk.html

"值: $a"
来源：http://hz.316326.xyz/gtpvkngupg.html

[T44] Perl：条件
来源：http://hz.sysykeji.top/gtvxzpqbsb.html

if ($a > 0) { print "正"; }
来源：http://hz.nanxuanxn.top/gtyfajddvu.html

[T45] Perl：数组遍历
来源：http://hz.zhengqikj.top/gtbmpbsjgg.html

for my $x (@arr) { print $x; }
来源：http://hz.hnqzz.top/gtycvrjkbx.html

[T46] Perl：哈希操作
来源：http://hz.zhaomingkeji.xyz/gtsyvlzuvf.html

$h{b} = 2;  for my $k (keys %h) { print "$k=$h{$k}"; }
来源：http://hz.zhengqikj.top/gtmrkajhhj.html

[T47] Perl：正则捕获
来源：http://hz.jqgufenzy.top/gtravizsmw.html

if ($s =~ /(\d+)/) { print $1; }
来源：http://hz.svipenyu.cn/gttezzvgov.html

[T48] Perl：正则替换
来源：http://hz.hnqzz.top/gtqcjwhxma.html

$s =~ s/old/new/g;
来源：http://hz.xziqi.cn/gtmtvopocr.html

[T49] Perl：函数
来源：http://hz.redwolf501.top/gtfsxtipez.html

sub add { my ($a, $b) = @_; return $a + $b; }
来源：http://hz.andypj.xyz/gtnxyvxvbu.html

[T50] Perl：逐行读文件
来源：http://hz.tian-w.cn/gthfkvommb.html

open my $fh, "<", "a.txt" or die $!;
来源：http://hz.zhongyouzk.top/gttiwupbpw.html

while (my $line = <$fh>) { print $line; }
来源：http://hz.shangyingyoupin.top/gtqfruunqg.html

[T51] Scala：Hello World
来源：http://hz.jlsjyb.cn/gtbefulvpp.html

println("Hello")
来源：http://hz.jqgfzy.top/gtxyribtoj.html

[T52] Scala：变量
来源：http://hz.jinyuanbaomall.cn/gtjvqovvpy.html

val a = 1;  var b = 2
来源：http://hz.zycfv.cn/gtmcyqermt.html

[T53] Scala：字符串插值
来源：http://hz.shangyingyoupin.top/gtjfabgrie.html

s"值: $b"
来源：http://hz.iojbl.cn/gtrscaivlo.html

[T54] Scala：集合映射
来源：http://hz.pengpengdd.cyou/gtspvqdzdr.html

List(1, 2, 3).map(_ * 2)
来源：http://hz.cheryme.top/gtspwtvyrs.html

[T55] Scala：集合过滤
来源：http://hz.pengpengdd.cyou/gtgyacbzur.html

List(1, 2, 3).filter(_ > 1)
来源：http://hz.yangfankeji.com/gtgzhxkazd.html

[T56] Scala：样例类
来源：http://hz.xylfe.cn/gthuvccmlb.html

case class User(name: String, age: Int)
来源：http://hz.guannengcc.top/gtybgvlvaz.html

[T57] Scala：模式匹配
来源：http://hz.yangfankeji.com/gtcgbjrapg.html

x match { case 1 => "一"; case _ => "其他" }
来源：http://hz.zhiwuduotai.top/gtqfoaxyjl.html

[T58] Scala：函数定义
来源：http://hz.andypj.xyz/gtmdrxbqrd.html

def add(a: Int, b: Int): Int = a + b
来源：http://hz.birdmap.top/gtluputepl.html

[T59] Scala：循环
来源：http://hz.kuanghao11.cn/gtujpecdjp.html

for (i <- 1 to 10) println(i)
来源：http://hz.tianlin.xyz/gtxcgsoggk.html

[T60] Scala：折叠
来源：http://hz.chenlongwang.top/gtlgliboda.html

List(1, 2, 3).foldLeft(0)(_ + _)
来源：http://hz.jlsjyb.cn/gtyfrerhcb.html

================================================================================
来源：http://hz.sufxvd.cn/gtwdvsooca.html

U. 高频实用片段（Python / PHP / JavaScript 各 40 条）
来源：http://hz.sufxvd.cn/gthjmfhkfu.html

================================================================================
来源：http://hz.ybcxt.top/gtzksumgba.html

[U01] Py：创建虚拟环境
来源：http://hz.yongpay.top/gttenfiwmd.html

python -m venv .venv && source .venv/bin/activate
来源：http://hz.jlsjyb.cn/gtlfnilono.html

[U02] Py：导出 / 安装依赖
来源：http://hz.kuanghao11.cn/gtsiymjhzl.html

pip freeze > requirements.txt;  pip install -r requirements.txt
来源：http://hz.hnxiangtu.top/gtazfqdonr.html

[U03] Py：加载 .env 配置
来源：http://hz.cheryme.top/gtwupjiqcr.html

from dotenv import load_dotenv; load_dotenv()
来源：http://hz.sufxvd.cn/gtsilrloaj.html

[U04] Py：变量调试打印
来源：http://hz.tianlin.xyz/gtfhfcpfsa.html

print(f"{x=}")            # 输出 x=值，Python 3.8+
来源：http://hz.chenjidiqi.icu/gtwpvbhhma.html

[U05] Py：列表去重且保序
来源：http://hz.xinyue.icu/gtkjqxrjiv.html

list(dict.fromkeys(arr))
来源：http://hz.9152youxi.cn/gtlugjpzic.html

[U06] Py：合并两个字典
来源：http://hz.tianlin.xyz/gtkmvlelxm.html

{**a, **b}
来源：http://hz.jinghuilouyu.cn/gtwmpeyhje.html

[U07] Py：反转字典键值
来源：http://hz.316326.xyz/gtwgcdizpf.html

{v: k for k, v in d.items()}
来源：http://hz.andypj.xyz/gtpjrhgcop.html

[U08] Py：展平二维列表
来源：http://hz.jinghuilouyu.cn/gtyimrwkfg.html

[y for x in nested for y in x]
来源：http://hz.guannengcc.top/gtyakbkzpq.html

[U09] Py：字典取最大值的键
来源：http://hz.vqdsnc.cn/gtzrastgem.html

max(d, key=d.get)
来源：http://hz.daxiang520.top/gtlzhesiux.html

[U10] Py：按值排序字典
来源：http://hz.cashguo.top/gtsrltggoe.html

dict(sorted(d.items(), key=lambda kv: kv[1]))
来源：http://hz.jianghu66.top/gttuoqcbhg.html

[U11] Py：生成器表达式
来源：http://hz.sysykeji.top/gtgqfcfogb.html

(x * 2 for x in arr)
来源：http://hz.smart0.xyz/gtvtugtcgi.html

[U12] Py：取出现最多的 3 个元素
来源：http://hz.zhongyouzk.top/gtwuvyzwem.html

Counter(arr).most_common(3)
来源：http://hz.zhoulong.xyz/gtxmnpahnh.html

[U13] Py：固定长度队列
来源：http://hz.xinyue.icu/gtoqiveuck.html

deque(maxlen=10)
来源：http://hz.jinyuanbaomall.cn/gtrymwnzmi.html

[U14] Py：分组收集到列表
来源：http://hz.fengsongda.top/gtzyfawnmz.html

defaultdict(list)
来源：http://hz.xuetiantiany.cn/gtrrdcmswp.html

[U15] Py：高精度计时
来源：http://hz.zycfv.cn/gtqozqlsmm.html

t = time.perf_counter()
来源：http://hz.ybcxt.top/gtdflvgpzk.html

[U16] Py：命令行参数解析
来源：http://hz.yonumen.top/gtntzrfkpo.html

ap = argparse.ArgumentParser();  ap.add_argument("--name");  args = ap.parse_args()
来源：http://hz.pycfn.com/gtbgchadua.html

[U17] Py：初始化日志
来源：http://hz.c1oappe.top/gtovsdrgei.html

logging.basicConfig(level=logging.INFO)
来源：http://hz.yvedp.cn/gtodhdnjdj.html

[U18] Py：预编译正则
来源：http://hz.smart0.xyz/gtwpmebqho.html

pat = re.compile(r"\d+")
来源：http://hz.iojbl.cn/gtrbyoowda.html

[U19] Py：正则替换带回调
来源：http://hz.dashuyun.cn/gtrldckwhv.html

re.sub(r"\d+", lambda m: str(int(m.group()) * 2), s)
来源：http://hz.jianghu66.top/gtgytxrrkp.html

[U20] Py：缓存函数结果
来源：http://hz.yj202588.top/gtdufpeajt.html

@functools.lru_cache(maxsize=None)
来源：http://hz.hywenlv.cn/gtgnprzgct.html

[U21] Py：自定义上下文管理器
来源：http://hz.ivvv.top/gticymfslo.html

@contextlib.contextmanager
来源：http://hz.yj202588.top/gtljsoggyk.html

[U22] Py：矩阵转置
来源：http://hz.zhengqikj.top/gtvxjmimhl.html

list(zip(*m))
来源：http://hz.gaohongyu789.top/gtoxyfakod.html

[U23] Py：分块读取大文件
来源：http://hz.316326.xyz/gtpvrgiiho.html

for chunk in iter(lambda: f.read(8192), b""):
来源：http://hz.c1oappe.top/gtjlszksyf.html

[U24] Py：路径操作
来源：http://hz.xinyue.icu/gtcuxqglvv.html

Path("a/b.txt").parent.mkdir(parents=True, exist_ok=True)
来源：http://hz.meibo888.top/gtawaskhpi.html

[U25] Py：CSV 按字典读
来源：http://hz.316326.xyz/gtvojnuxsh.html

csv.DictReader(f)
来源：http://hz.vqdsnc.cn/gtgvyidulu.html

[U26] Py：并发下载
来源：http://hz.mhx1999.top/gttuxuvyin.html

ThreadPoolExecutor(max_workers=8).map(fetch, urls)
来源：http://hz.ydjk.org.cn/gtpcddkxoj.html

[U27] Py：异步 HTTP
来源：http://hz.gotoacloud.top/gttgfudkdu.html

aiohttp.ClientSession() 配合 async with
来源：http://hz.tianlin.xyz/gtusstzkou.html

[U28] Py：类型别名
来源：http://hz.shuidangran.top/gtjqetmaak.html

UserId = int
来源：http://hz.svipenyu.cn/gtapivxwbk.html

[U29] Py：属性校验
来源：http://hz.gotoacloud.top/gtxywgjtdd.html

@property 与 @x.setter 配合
来源：http://hz.gotoacloud.top/gtdbixbzpv.html

[U30] Py：数据类
来源：http://hz.yj202588.top/gtupuxgrgi.html

@dataclass(slots=True)
来源：http://hz.haohaochexian.top/gtgxvkhnxj.html

[U31] Py：单测
来源：http://hz.svipenyu.cn/gtnexnlnzm.html

python -m pytest -q
来源：http://hz.cucudq.cn/gtdavwlsdk.html

[U32] Py：代码格式化
来源：http://hz.yangfankeji.com/gtvfqsrwkz.html

ruff format . && ruff check --fix .
来源：http://hz.feifeiyinyue.top/gtdlnfqkdz.html

[U33] Py：打包发布
来源：http://hz.wangdashe.top/gtckelpjlw.html

python -m build  （依赖 pyproject.toml）
来源：http://hz.jianghu66.top/gtcxsjgzdx.html

[U34] Py：判断编码
来源：http://hz.yuxming.cn/gtjzhmbzwd.html

chardet.detect(raw)
来源：http://hz.shuidangran.top/gtrfrkrpzz.html

[U35] Py：发送邮件
来源：http://hz.aibaodan.cn/gtgafikxzt.html

smtplib.SMTP_SSL(...).send_message(msg)
来源：http://hz.smart0.xyz/gttrxaozlw.html

[U36] Py：定时任务
来源：http://hz.shanyushiyangkeji.top/gtkwcnumxu.html

schedule.every(10).minutes.do(job)
来源：http://hz.yangfankeji.com/gthyxakgvg.html

[U37] Py：读写 Excel
来源：http://hz.xziqi.cn/gtqbzlmxcs.html

pandas.read_excel / DataFrame.to_excel
来源：http://hz.sxryk.cn/gtqmeabgja.html

[U38] Py：获取脚本所在目录
来源：http://hz.cashguo.top/gtlcslasmg.html

Path(__file__).resolve().parent
来源：http://hz.hammf.cn/gtykensfid.html

[U39] Py：判断是否在交互环境
来源：http://hz.mhx1999.top/gtohzrgsqz.html

sys.stdout.isatty()
来源：http://hz.sweek.top/gtshlodikr.html

[U40] Py：打印到标准错误
来源：http://hz.cucudq.cn/gtczbwepim.html

print("err", file=sys.stderr)
来源：http://hz.ehwqpu.com/gtquqcdkcx.html

[U41] PHP：初始化 Composer 项目
来源：http://hz.sweek.top/gtjdabzfrp.html

composer init;  composer require guzzlehttp/guzzle
来源：http://hz.9152youxi.cn/gtjjicyzbr.html

[U42] PHP：PSR-4 自动加载
来源：http://hz.kuanghao11.cn/gtjgzyjurp.html

"autoload": { "psr-4": { "App\\": "src/" } }
来源：http://hz.meibo888.top/gtbdvyxyyz.html

[U43] PHP：声明命名空间
来源：http://hz.ydjk.org.cn/gtwlgcxipl.html

namespace App\Http;
来源：http://hz.jinyuanbaomall.cn/gtaffxylgh.html

[U44] PHP：开启严格类型
来源：http://hz.tianlin.xyz/gtrwyizmjb.html

declare(strict_types=1);
来源：http://hz.zhaomingkeji.xyz/gtwiuverxf.html

[U45] PHP：类型声明与返回类型
来源：http://hz.nanxuanxn.top/gtsqpjyvsw.html

function add(int $a, int $b): int { return $a + $b; }
来源：http://hz.hysaishi.cn/gtdxpmizns.html

[U46] PHP：可空类型
来源：http://hz.hfpthk.cn/gtfiyhrfvx.html

?string $name = null
来源：http://hz.nwbrower.top/gttgqodais.html

[U47] PHP：联合类型
来源：http://hz.yuxming.cn/gtbmhwigmg.html

int|string $id
来源：http://hz.yj202588.top/gtjtuwkwqw.html

[U48] PHP：纯枚举
来源：http://hz.chenzaomai.com/gtaxshpuzq.html

enum Status: string { case Active = "active"; case Off = "off"; }
来源：http://hz.kuanghao11.cn/gtvqesjlub.html

[U49] PHP：只读属性
来源：http://hz.gogol.net.cn/gtkilzkeip.html

public readonly string $name
来源：http://hz.meibo888.top/gtydedqbfg.html

[U50] PHP：构造器属性提升
来源：http://hz.daxiang520.top/gtfectpgkx.html

public function __construct(private int $id) {}
来源：http://hz.shuidangran.top/gtacwhfqrc.html


<!-- 参考信息 -->