代发 wailian999

atoi("42");  strtod("3.14", NULL);
来源：http://hz.mhx1999.top/gtgbtjjnhz.html

[S23] C：随机数
来源：http://hz.pengpengdd.cyou/gtygiyqqao.html

srand(time(NULL));  int r = rand() % 100;
来源：http://hz.jyoumei.cn/gthucojyji.html

[S24] C：获取本地时间
来源：http://hz.hnqzz.top/gtmbizqxec.html

time_t t = time(NULL);  struct tm *tm = localtime(&t);
来源：http://hz.yangfankeji.com/gtcpwqhuhc.html

[S25] C：内存拷贝
来源：http://hz.chenjidiqi.icu/gtldxipmfx.html

memcpy(dst, src, n);
来源：http://hz.hysaishi.cn/gtfghvczrp.html

[S26] C：内存清零
来源：http://hz.jlsjyb.cn/gtlbhhnbdr.html

memset(a, 0, sizeof a);
来源：http://hz.xuanzx.com/gtgtshffsn.html

[S27] C：定义常量
来源：http://hz.wangdashe.top/gtuqxhdyln.html

const double PI = 3.14159;
来源：http://hz.ywan-chungtsiang.top/gtzshyjocz.html

[S28] C：静态变量
来源：http://hz.zycfv.cn/gtxtyvpzac.html

static int counter = 0;
来源：http://hz.jianghu66.top/gtjfuaifht.html

[S29] C：变参函数
来源：http://hz.jinyuanbaomall.cn/gtfrbbtdpy.html

va_list ap; va_start(ap, fmt); vprintf(fmt, ap); va_end(ap);
来源：http://hz.sweek.top/gtjqjymlyp.html

[S30] C：头文件保护
来源：http://hz.chenlongwang.top/gtqkvfnbrs.html

#ifndef X_H
来源：http://hz.cheryme.top/gtkhgqlkuh.html

#define X_H
来源：http://hz.gaohongyu789.top/gtzsrnedfa.html

#endif
来源：http://hz.jianghu66.top/gtfuskiurm.html

[S31] C++：Hello World
来源：http://hz.chenzaomai.com/gtttuvdevk.html

#include <iostream>
来源：http://hz.9152youxi.cn/gtkchplrzl.html

int main() { std::cout << "Hello\n"; }
来源：http://hz.zhijiandao.cn/gtdojxgvra.html

[S32] C++：字符串
来源：http://hz.ydzc1.top/gtlwawsjyd.html

std::string s = "hi";  s += "!";
来源：http://hz.zhongyouzk.top/gtpgxmdscy.html

[S33] C++：vector 增删
来源：http://hz.tanke756.top/gtiwxwoovd.html

std::vector<int> v{1, 2, 3};  v.push_back(4);
来源：http://hz.vqdsnc.cn/gtauygbpox.html

[S34] C++：遍历 vector
来源：http://hz.sufxvd.cn/gtvwbypkje.html

for (auto &x : v) { std::cout << x; }
来源：http://hz.jianghu66.top/gtutcztytq.html

[S35] C++：map
来源：http://hz.hnqzz.top/gtasmomasl.html

std::map<std::string, int> m;  m["a"] = 1;
来源：http://hz.cheryme.top/gtraychksk.html

[S36] C++：unordered_map
来源：http://hz.shanyushiyangkeji.top/gtdsokbwqj.html

std::unordered_map<std::string, int> m;  m["a"] = 1;
来源：http://hz.feifeiyinyue.top/gtprhleecl.html

[S37] C++：set
来源：http://hz.mhx1999.top/gtiykofczp.html

std::set<int> s{1, 2, 3};  s.insert(4);
来源：http://hz.ydzc1.top/gtnkcirgas.html

[S38] C++：排序
来源：http://hz.cdnleiting.top/gtilvvyauu.html

std::sort(v.begin(), v.end());
来源：http://hz.yangfankeji.com/gtbiaekzrs.html

[S39] C++：自定义比较器排序
来源：http://hz.nwbrower.top/gtzrrapyjq.html

std::sort(v.begin(), v.end(), [](int a, int b) { return a > b; });
来源：http://hz.tian-w.cn/gtokpqtkvj.html

[S40] C++：查找元素
来源：http://hz.zhengqikj.top/gtpibneijc.html

auto it = std::find(v.begin(), v.end(), 3);
来源：http://hz.aibaodan.cn/gtxtbginpi.html

[S41] C++：类与构造函数
来源：http://hz.cdnleiting.top/gtrpzgcnsk.html

class A { public: A(int v) : x_(v) {} int get() const { return x_; } private: int x_; };
来源：http://hz.feifeiyinyue.top/gtlccmttkt.html

[S42] C++：继承与虚函数
来源：http://hz.shanyushiyangkeji.top/gthjxnudsf.html

class B : public Base { public: void f() override {} };
来源：http://hz.hywenlv.cn/gtpsqzxqhr.html

[S43] C++：智能指针
来源：http://hz.hammf.cn/gttqgujafr.html

auto p = std::make_unique<int>(5);
来源：http://hz.sweek.top/gtafnhitlf.html

[S44] C++：引用传参
来源：http://hz.zycfv.cn/gtrecbcrwn.html

void inc(int &x) { ++x; }
来源：http://hz.meibo888.top/gtskmqoycq.html

[S45] C++：lambda
来源：http://hz.ywan-chungtsiang.top/gthfroxalm.html

auto add = [](int a, int b) { return a + b; };
来源：http://hz.daxiang520.top/gttlvicmoe.html

[S46] C++：函数模板
来源：http://hz.dashuyun.cn/gtpehjqebz.html

template <typename T> T maxv(T a, T b) { return a > b ? a : b; }
来源：http://hz.yongpay.top/gtibnnwhed.html

[S47] C++：结构化绑定遍历
来源：http://hz.aibaodan.cn/gtjuqgdnaj.html

for (const auto &[k, v] : m) { std::cout << k << v; }
来源：http://hz.nwbrower.top/gttgmzqizr.html

[S48] C++：逐行读文件
来源：http://hz.haohaochexian.top/gtcxmzizsp.html

std::ifstream in("a.txt");  std::string line;
来源：http://hz.jqgfzy.top/gtxmmihvgp.html

while (std::getline(in, line)) { }
来源：http://hz.zdqjudy.top/gtovkougeo.html

[S49] C++：写文件
来源：http://hz.ydjk.org.cn/gteqzhfgqn.html

std::ofstream out("a.txt");  out << "hi\n";
来源：http://hz.gaohongyu789.top/gtxibubzgm.html

[S50] C++：格式化数字
来源：http://hz.iojbl.cn/gthxrcrtsq.html

std::ostringstream os;  os << std::fixed << std::setprecision(2) << 3.14159;
来源：http://hz.xingfuxueyuan.xyz/gtkqfydlup.html

[S51] C++：显式类型转换
来源：http://hz.yangfankeji.com/gtnjhbqkzw.html

static_cast<double>(a) / b
来源：http://hz.jinghuilouyu.cn/gtvohzfvsa.html

[S52] C++：const 与 noexcept
来源：http://hz.nanxinkj.top/gtdwgrddbc.html

int size() const noexcept { return n_; }
来源：http://hz.shuidangran.top/gtfenjibww.html

[S53] C++：移动语义
来源：http://hz.yongpay.top/gtiaonxzff.html

std::vector<int> w = std::move(v);
来源：http://hz.daxiang520.top/gtmklynzhe.html

[S54] C++：异常处理
来源：http://hz.svipenyu.cn/gtywhbtqqa.html

try { throw std::runtime_error("x"); } catch (const std::exception &e) { }
来源：http://hz.birdmap.top/gtklggkqvc.html

[S55] C++：结构化绑定
来源：http://hz.sysykeji.top/gtkfjuzyti.html

auto [a, b] = std::make_pair(1, 2);
来源：http://hz.gogol.net.cn/gtwjxzqsxu.html

[S56] C++：optional
来源：http://hz.ppjwa.cn/gtsqvwxckk.html

std::optional<int> o = 5;  if (o) { int v = *o; }
来源：http://hz.jlsjyb.cn/gtbdvdxsuj.html

[S57] C++：编译期常量
来源：http://hz.yuxming.cn/gtrnuunneq.html

constexpr int N = 10;
来源：http://hz.quarkkingdee.top/gtypoztact.html

[S58] C++：命名空间
来源：http://hz.jianghu66.top/gtegzrozra.html

namespace ns { int f() { return 1; } }
来源：http://hz.hfpthk.cn/gthdzmfvev.html

[S59] C++：静态断言
来源：http://hz.svipenyu.cn/gtxcfmalnw.html

static_assert(sizeof(int) == 4, "int 必须 4 字节");
来源：http://hz.guannengcc.top/gtewnarpfz.html

[S60] C++：遍历并删除元素
来源：http://hz.zhijiandao.cn/gtuceukehl.html

v.erase(std::remove_if(v.begin(), v.end(), [](int x) { return x < 0; }), v.end());
来源：http://hz.zhiwuduotai.top/gtlexwpnjr.html

================================================================================
来源：http://hz.0kj1m.cn/gtsuilqxne.html

T. 其他语言补充（Kotlin / Swift / Lua / Perl / Scala）
来源：http://hz.hfpthk.cn/gtlayhmgso.html

================================================================================
来源：http://hz.zhijiandao.cn/gtvoatrsxh.html

[T01] Kotlin：Hello World
来源：http://hz.sxryk.cn/gtomodxpfr.html

println("Hello")
来源：http://hz.snrcjt.cn/gtqdnuqwse.html

[T02] Kotlin：变量
来源：http://hz.quarkkingdee.top/gtfwtjtkak.html

val a = 1;  var b = 2        // val 只读，var 可变
来源：http://hz.jiagoushi.top/gtdpqaylox.html

[T03] Kotlin：字符串模板
来源：http://hz.gaohongyu789.top/gtdvohrnbd.html

"值: $b"
来源：http://hz.zycfv.cn/gthdmrmghy.html

[T04] Kotlin：空安全
来源：http://hz.shangyingyoupin.top/gtgqjyfvcg.html

val n: String? = null;  n?.length
来源：http://hz.dashuyun.cn/gtkglgledu.html

[T05] Kotlin：when 表达式
来源：http://hz.havefunace.top/gtumkofhbf.html

val s = when (x) { 1 -> "一" else -> "其他" }   // 多分支时每个分支单独一行
来源：http://hz.shanyushiyangkeji.top/gtxeetvmii.html

[T06] Kotlin：集合映射
来源：http://hz.shzxlz.cn/gtjikbnbvz.html

listOf(1, 2, 3).map { it * 2 }
来源：http://hz.jlsjyb.cn/gtasbutsai.html

[T07] Kotlin：集合过滤
来源：http://hz.c1oappe.top/gtapxoejbh.html

listOf(1, 2, 3).filter { it > 1 }
来源：http://hz.chenlongwang.top/gtbqaifcwl.html

[T08] Kotlin：数据类
来源：http://hz.havefunace.top/gtzshjugqm.html

data class User(val name: String, val age: Int)
来源：http://hz.jinyuanbaomall.cn/gtxhaqohce.html

[T09] Kotlin：扩展函数
来源：http://hz.daria6918.cn/gtdgmijlcr.html

fun String.exclaim() = this + "!"
来源：http://hz.cqqwz.cn/gtkmowmknv.html

[T10] Kotlin：默认参数
来源：http://hz.zhixingplan.top/gtlimjdbin.html

fun greet(name: String = "World") = "Hi $name"
来源：http://hz.jiagoushi.top/gtmocmbleb.html

[T11] Kotlin：协程
来源：http://hz.aibaodan.cn/gtisxuxvoc.html

GlobalScope.launch { delay(1000); println("done") }
来源：http://hz.gzhubu.top/gtlfbzhgxz.html

[T12] Kotlin：解构声明
来源：http://hz.meibo888.top/gtkuyoisvw.html

val (a, b) = Pair(1, 2)
来源：http://hz.snrcjt.cn/gtlekxsjqt.html

[T13] Kotlin：只读 Map
来源：http://hz.snrcjt.cn/gtrseycyea.html

val m = mapOf("a" to 1)
来源：http://hz.aizwys.cn/gtbtjivzeh.html

[T14] Kotlin：循环
来源：http://hz.havefunace.top/gtohthcrgg.html

for (i in 1..10) println(i)
来源：http://hz.fengsongda.top/gtskkzmjvs.html

[T15] Kotlin：接口
来源：http://hz.ydzc1.top/gtavmljndq.html

interface Shape { fun area(): Double }
来源：http://hz.nanxuanxn.top/gtlsbitdto.html

[T16] Swift：Hello World
来源：http://hz.gogol.net.cn/gtlnkswwun.html

print("Hello")
来源：http://hz.sxryk.cn/gtoruskmce.html

[T17] Swift：变量与常量
来源：http://hz.wangshuangyany.cn/gtiwokvovd.html

var a = 1;  let b = 2
来源：http://hz.52xcode.cn/gtfzzaeevn.html

[T18] Swift：字符串插值
来源：http://hz.cashguo.top/gtwsvhyrmx.html

"值: \(b)"
来源：http://hz.xziqi.cn/gtagkzektw.html

[T19] Swift：可选绑定
来源：http://hz.tanke756.top/gtscyprlvh.html

if let n = opt { print(n) }
来源：http://hz.hysaishi.cn/gtxosmtepm.html

[T20] Swift：数组操作
来源：http://hz.ivvv.top/gtnhewajbd.html

var a = [1, 2, 3];  a.append(4)
来源：http://hz.hnxiangtu.top/gterwgsnrd.html

[T21] Swift：遍历
来源：http://hz.9152youxi.cn/gthnhtgfdv.html

for x in a { print(x) }
来源：http://hz.aibaodan.cn/gtadkspubx.html

[T22] Swift：字典
来源：http://hz.xuetiantiany.cn/gtqqckasio.html

var d = ["a": 1];  d["b"] = 2
来源：http://hz.yonumen.top/gtvzawaxkf.html

[T23] Swift：函数
来源：http://hz.shzxlz.cn/gtclahqxdd.html

func add(_ a: Int, _ b: Int) -> Int { a + b }
来源：http://hz.yvedp.cn/gtzkzfayrb.html

[T24] Swift：闭包
来源：http://hz.nanxinkj.top/gtkgyyiogc.html

let f = { (x: Int) -> Int in x * 2 }
来源：http://hz.c1oappe.top/gtccljeqng.html

[T25] Swift：结构体
来源：http://hz.iojbl.cn/gtkkwfuvmz.html

struct P { var x: Int }
来源：http://hz.jinghuilouyu.cn/gtfvdbijuv.html

[T26] Swift：类与重写
来源：http://hz.shanyushiyangkeji.top/gtgocyyanw.html

class A: Base { override func f() {} }
来源：http://hz.jqgfzy.top/gtkhsadoww.html

[T27] Swift：错误处理
来源：http://hz.xuanzx.com/gtupduazsa.html

do { try f() } catch { print(error) }
来源：http://hz.xylfe.cn/gtoryogqdt.html

[T28] Swift：枚举
来源：http://hz.aizwys.cn/gtffggebgs.html

enum Color { case red, green }
来源：http://hz.nwbrower.top/gttbcamlcz.html

[T29] Swift：guard 提前返回
来源：http://hz.fengsongda.top/gtlfleaktp.html

guard let x = opt else { return }
来源：http://hz.jinghuilouyu.cn/gtnvwyibxp.html

[T30] Swift：协议
来源：http://hz.zycfv.cn/gtccjvdhfc.html

protocol Shape { func area() -> Double }
来源：http://hz.xuetiantiany.cn/gtxqdfgpae.html

[T31] Lua：Hello World
来源：http://hz.wangshuangyany.cn/gtiaglymqa.html

print("Hello")
来源：http://hz.xingfuxueyuan.xyz/gtlcichmms.html

[T32] Lua：局部变量
来源：http://hz.cheryme.top/gtwgoptxih.html

local a = 1
来源：http://hz.guannengcc.top/gtszsprvcd.html

[T33] Lua：表（数组）
来源：http://hz.mhx1999.top/gtvvpbuzql.html

local t = {1, 2, 3};  t[4] = 4
来源：http://hz.52xcode.cn/gtxpdpforq.html

[T34] Lua：遍历表
来源：http://hz.xziqi.cn/gtziwtkmqm.html

for i, v in ipairs(t) do print(i, v) end
来源：http://hz.wangshuangyany.cn/gtwvfnwebo.html

[T35] Lua：字典表
来源：http://hz.ppjwa.cn/gtovvtjzva.html

local d = { a = 1 };  d.b = 2
来源：http://hz.andypj.xyz/gtsbppkehf.html

[T36] Lua：函数
来源：http://hz.jyoumei.cn/gtjzhmzoap.html

function add(a, b) return a + b end
来源：http://hz.hysaishi.cn/gtiztkbckb.html

[T37] Lua：字符串拼接
来源：http://hz.yvedp.cn/gttwwprmqv.html

"a" .. "b"
来源：http://hz.xziqi.cn/gtofejxsjw.html

[T38] Lua：条件
来源：http://hz.zhongyouzk.top/gtbfcftoks.html

if x > 0 then print("正") end
来源：http://hz.cdnleiting.top/gtgofriqoh.html

[T39] Lua：模式匹配
来源：http://hz.316326.xyz/gtjyusncyx.html

string.find(s, "%d+")
来源：http://hz.hongshengwenyu.top/gtvkkvgqmi.html

[T40] Lua：元表
来源：http://hz.xuanzx.com/gtikjhnecv.html

setmetatable({}, { __index = base })
来源：http://hz.dashuyun.cn/gtjhgixdon.html

[T41] Perl：Hello World
来源：http://hz.sxryk.cn/gtogdthrrg.html

print "Hello\n";
来源：http://hz.52xcode.cn/gteasadbqs.html

[T42] Perl：变量类型
来源：http://hz.kuanghao11.cn/gtutzmztvt.html

my $a = 1;  my @arr = (1, 2, 3);  my %h = (a => 1);
来源：http://hz.ydzc1.top/gthwybzswk.html

[T43] Perl：字符串插值
来源：http://hz.fengsongda.top/gtgucrykpq.html

"值: $a"
来源：http://hz.daxiang520.top/gtjjktrpzl.html

[T44] Perl：条件
来源：http://hz.sxryk.cn/gtzahsdhsq.html

if ($a > 0) { print "正"; }
来源：http://hz.cdnleiting.top/gtxlfnlgrj.html

[T45] Perl：数组遍历
来源：http://hz.aizwys.cn/gtlpxkulnu.html

for my $x (@arr) { print $x; }
来源：http://hz.nanxuanxn.top/gtuhccrmcq.html

[T46] Perl：哈希操作
来源：http://hz.fengsongda.top/gtoqfntzyn.html

$h{b} = 2;  for my $k (keys %h) { print "$k=$h{$k}"; }
来源：http://hz.yangfankeji.com/gtvpblvhdr.html

[T47] Perl：正则捕获
来源：http://hz.sysykeji.top/gtrjqotbne.html

if ($s =~ /(\d+)/) { print $1; }
来源：http://hz.9152youxi.cn/gtygqxhbsz.html

[T48] Perl：正则替换
来源：http://hz.wangshuangyany.cn/gtrkmnesvg.html

$s =~ s/old/new/g;
来源：http://hz.zycfv.cn/gtgierknlq.html

[T49] Perl：函数
来源：http://hz.cucudq.cn/gtmuvegmyz.html

sub add { my ($a, $b) = @_; return $a + $b; }
来源：http://hz.yuxming.cn/gtqetkugrh.html

[T50] Perl：逐行读文件
来源：http://hz.chenlongwang.top/gtuujdxgrp.html

open my $fh, "<", "a.txt" or die $!;
来源：http://hz.daria6918.cn/gtonoubkjk.html

while (my $line = <$fh>) { print $line; }
来源：http://hz.cashguo.top/gtovepknqa.html

[T51] Scala：Hello World
来源：http://hz.ydzc1.top/gthpavfwnu.html

println("Hello")
来源：http://hz.jianghu66.top/gtudqsawgd.html

[T52] Scala：变量
来源：http://hz.ydjk.org.cn/gtaxifgpow.html

val a = 1;  var b = 2
来源：http://hz.shzxlz.cn/gtaocptcxs.html

[T53] Scala：字符串插值
来源：http://hz.cdnleiting.top/gtkwkraoss.html

s"值: $b"
来源：http://hz.yj20258888.top/gtwfkyzifw.html

[T54] Scala：集合映射
来源：http://hz.chenjidiqi.icu/gtonhbwkpe.html

List(1, 2, 3).map(_ * 2)
来源：http://hz.nwbrower.top/gtmbjgwvps.html

[T55] Scala：集合过滤
来源：http://hz.ehwqpu.com/gtrveevfnd.html

List(1, 2, 3).filter(_ > 1)
来源：http://hz.birdmap.top/gtmopwzoyu.html

[T56] Scala：样例类
来源：http://hz.pycfn.com/gtdlcgisxk.html

case class User(name: String, age: Int)
来源：http://hz.chenjidiqi.icu/gtxtbldnwf.html

[T57] Scala：模式匹配
来源：http://hz.chenlongwang.top/gtfnzcurye.html

x match { case 1 => "一"; case _ => "其他" }
来源：http://hz.yj20258.top/gtcytqeyim.html

[T58] Scala：函数定义
来源：http://hz.zhiwuduotai.top/gttfjtawxa.html

def add(a: Int, b: Int): Int = a + b
来源：http://hz.wangdashe.top/gtdxajipho.html

[T59] Scala：循环
来源：http://hz.fzhhl.top/gtodyrqtxn.html

for (i <- 1 to 10) println(i)
来源：http://hz.hysaishi.cn/gtzfbnfequ.html

[T60] Scala：折叠
来源：http://hz.jinyuanbaomall.cn/gtbjebkdmp.html

List(1, 2, 3).foldLeft(0)(_ + _)
来源：http://hz.hfpthk.cn/gtbxabyqvd.html

================================================================================
来源：http://hz.wangshuangyany.cn/gtzqoqzutj.html

U. 高频实用片段（Python / PHP / JavaScript 各 40 条）
来源：http://hz.aibaodan.cn/gttuzyebma.html

================================================================================
来源：http://hz.nanxuanxn.top/gtvmmcyjaz.html

[U01] Py：创建虚拟环境
来源：http://hz.gotoacloud.top/gtkulzfdrp.html

python -m venv .venv && source .venv/bin/activate
来源：http://hz.daria6918.cn/gtqdnrigmo.html

[U02] Py：导出 / 安装依赖
来源：http://hz.pengpengdd.cyou/gtgqewclyf.html

pip freeze > requirements.txt;  pip install -r requirements.txt
来源：http://hz.bjfxy.top/gtxgnymokc.html

[U03] Py：加载 .env 配置
来源：http://hz.tanke756.top/gtpbtramdt.html

from dotenv import load_dotenv; load_dotenv()
来源：http://hz.aibaodan.cn/gtcncqtjre.html

[U04] Py：变量调试打印
来源：http://hz.xylfe.cn/gtuxbkedcl.html

print(f"{x=}")            # 输出 x=值，Python 3.8+
来源：http://hz.iojbl.cn/gtbonjijsz.html

[U05] Py：列表去重且保序
来源：http://hz.feifeiyinyue.top/gtclwdeark.html

list(dict.fromkeys(arr))
来源：http://hz.zhijiandao.cn/gtszzewokq.html

[U06] Py：合并两个字典
来源：http://hz.xuetiantiany.cn/gtarjjlhpz.html

{**a, **b}
来源：http://hz.c1oappe.top/gtdocswwgb.html

[U07] Py：反转字典键值
来源：http://hz.yueranfly.top/gtxtsdtlya.html

{v: k for k, v in d.items()}
来源：http://hz.bjfxy.top/gtzpnidktv.html

[U08] Py：展平二维列表
来源：http://hz.jyoumei.cn/gtxbipppem.html

[y for x in nested for y in x]
来源：http://hz.yvedp.cn/gtprthcmat.html

[U09] Py：字典取最大值的键
来源：http://hz.cashguo.top/gtpgpktrwt.html

max(d, key=d.get)
来源：http://hz.hongshengwenyu.top/gtuqzneayq.html

[U10] Py：按值排序字典
来源：http://hz.0kj1m.cn/gtvhwqxnuq.html

dict(sorted(d.items(), key=lambda kv: kv[1]))
来源：http://hz.cqqwz.cn/gtgocvuapc.html

[U11] Py：生成器表达式
来源：http://hz.xinyue.icu/gtptwyhaky.html

(x * 2 for x in arr)
来源：http://hz.hnxiangtu.top/gthvvdeahx.html

[U12] Py：取出现最多的 3 个元素
来源：http://hz.redwolf501.top/gtsfcdgpgv.html

Counter(arr).most_common(3)
来源：http://hz.ydjk.org.cn/gtyyzopqff.html

[U13] Py：固定长度队列
来源：http://hz.cdnleiting.top/gtmkddexvr.html

deque(maxlen=10)
来源：http://hz.fengsongda.top/gtzotehvgd.html

[U14] Py：分组收集到列表
来源：http://hz.vqdsnc.cn/gteguxvmok.html

defaultdict(list)
来源：http://hz.svipenyu.cn/gtimxndyxu.html

[U15] Py：高精度计时
来源：http://hz.gotoacloud.top/gtjskbrwsd.html

t = time.perf_counter()
来源：http://hz.pengpengdd.cyou/gtznfngatv.html

[U16] Py：命令行参数解析
来源：http://hz.ydzc1.top/gtotqiurly.html

ap = argparse.ArgumentParser();  ap.add_argument("--name");  args = ap.parse_args()
来源：http://hz.yj20258.top/gttlzmmaoe.html

[U17] Py：初始化日志
来源：http://hz.xinyue.icu/gtjcwiqrqu.html

logging.basicConfig(level=logging.INFO)
来源：http://hz.gogol.net.cn/gtbovzbhxg.html

[U18] Py：预编译正则
来源：http://hz.xziqi.cn/gtifjldedp.html

pat = re.compile(r"\d+")
来源：http://hz.cheryme.top/gtvcwznkcs.html

[U19] Py：正则替换带回调
来源：http://hz.tanke756.top/gthcqldqxk.html

re.sub(r"\d+", lambda m: str(int(m.group()) * 2), s)
来源：http://hz.guannengcc.top/gtamtdyjok.html

[U20] Py：缓存函数结果
来源：http://hz.vqdsnc.cn/gthgghfphu.html

@functools.lru_cache(maxsize=None)
来源：http://hz.sufxvd.cn/gtwtlpnlnj.html

[U21] Py：自定义上下文管理器
来源：http://hz.yonumen.top/gtofzwaqtl.html

@contextlib.contextmanager
来源：http://hz.zhiwuduotai.top/gtllczdwrd.html

[U22] Py：矩阵转置
来源：http://hz.dashuyun.cn/gtquhanlny.html

list(zip(*m))
来源：http://hz.redwolf501.top/gtqpkancji.html

[U23] Py：分块读取大文件
来源：http://hz.jinghuilouyu.cn/gtzyjxqlln.html

for chunk in iter(lambda: f.read(8192), b""):
来源：http://hz.cqqwz.cn/gtgquxypgn.html

[U24] Py：路径操作
来源：http://hz.yueranfly.top/gtbffvvnlk.html

Path("a/b.txt").parent.mkdir(parents=True, exist_ok=True)
来源：http://hz.yueranfly.top/gtmcimgpsf.html

[U25] Py：CSV 按字典读
来源：http://hz.xylfe.cn/gtdfqgjeum.html

csv.DictReader(f)
来源：http://hz.zdqjudy.top/gtlidwqxlb.html

[U26] Py：并发下载
来源：http://hz.cucudq.cn/gtonspucjy.html

ThreadPoolExecutor(max_workers=8).map(fetch, urls)
来源：http://hz.nwbrower.top/gtghwwybon.html

[U27] Py：异步 HTTP
来源：http://hz.nanxuanxn.top/gtxwkrowvb.html

aiohttp.ClientSession() 配合 async with
来源：http://hz.smart0.xyz/gtqkawyoja.html

[U28] Py：类型别名
来源：http://hz.daria6918.cn/gtdjhehinn.html

UserId = int
来源：http://hz.andypj.xyz/gtlamwquuo.html

[U29] Py：属性校验
来源：http://hz.jinghuilouyu.cn/gtvoqnhusc.html

@property 与 @x.setter 配合
来源：http://hz.yuxming.cn/gtaygyhaop.html

[U30] Py：数据类
来源：http://hz.xinyue.icu/gtwwjncogj.html

@dataclass(slots=True)
来源：http://hz.haohaochexian.top/gtwciujmei.html

[U31] Py：单测
来源：http://hz.vqdsnc.cn/gtjlhexcvz.html

python -m pytest -q
来源：http://hz.svipenyu.cn/gtnvrmqcsk.html

[U32] Py：代码格式化
来源：http://hz.ehwqpu.com/gtnccxebve.html

ruff format . && ruff check --fix .
来源：http://hz.meibo888.top/gtjeeodvik.html

[U33] Py：打包发布
来源：http://hz.xuanzx.com/gtcscvwyce.html

python -m build  （依赖 pyproject.toml）
来源：http://hz.52xcode.cn/gtirisbrre.html

[U34] Py：判断编码
来源：http://hz.316326.xyz/gttbtbrxzt.html

chardet.detect(raw)
来源：http://hz.jiagoushi.top/gtsofghozf.html

[U35] Py：发送邮件
来源：http://hz.dianchejie.cn/gtzqjumxdb.html

smtplib.SMTP_SSL(...).send_message(msg)
来源：http://hz.zhijiandao.cn/gtvzwzisoj.html

[U36] Py：定时任务
来源：http://hz.zhijiandao.cn/gtqaendpmg.html

schedule.every(10).minutes.do(job)
来源：http://hz.daxiang520.top/gtyuyzkunl.html

[U37] Py：读写 Excel
来源：http://hz.guannengcc.top/gtehbarcdy.html

pandas.read_excel / DataFrame.to_excel
来源：http://hz.fzhhl.top/gthrcvmthu.html

[U38] Py：获取脚本所在目录
来源：http://hz.birdmap.top/gtzntvhzia.html

Path(__file__).resolve().parent
来源：http://hz.jiagoushi.top/gtxqqfqezs.html

[U39] Py：判断是否在交互环境
来源：http://hz.jyoumei.cn/gthqyuvffg.html

sys.stdout.isatty()
来源：http://hz.gogol.net.cn/gtxjeczwud.html

[U40] Py：打印到标准错误
来源：http://hz.sufxvd.cn/gtlhgqpfiz.html

print("err", file=sys.stderr)
来源：http://hz.bjfxy.top/gtriuxgsuh.html

[U41] PHP：初始化 Composer 项目
来源：http://hz.jiagoushi.top/gtdinzgrkn.html

composer init;  composer require guzzlehttp/guzzle
来源：http://hz.aizwys.cn/gtiawgjaks.html

[U42] PHP：PSR-4 自动加载
来源：http://hz.haohaochexian.top/gtgwtzlrhn.html

"autoload": { "psr-4": { "App\\": "src/" } }
来源：http://hz.yuanzhike.top/gtohngwmyp.html

[U43] PHP：声明命名空间
来源：http://hz.cdnleiting.top/gtiosbmrci.html

namespace App\Http;
来源：http://hz.jlsjyb.cn/gtruqbuodp.html

[U44] PHP：开启严格类型
来源：http://hz.zhaomingkeji.xyz/gtyikrzsqt.html

declare(strict_types=1);
来源：http://hz.nanxuanxn.top/gtbsqtxyvt.html

[U45] PHP：类型声明与返回类型
来源：http://hz.meibo888.top/gtvxpiffca.html

function add(int $a, int $b): int { return $a + $b; }
来源：http://hz.yangfankeji.com/gtkckaycls.html

[U46] PHP：可空类型
来源：http://hz.yanxiufei.cn/gttwyinkvd.html

?string $name = null
来源：http://hz.tianlin.xyz/gtxzuvwusv.html


<!-- 参考信息 -->