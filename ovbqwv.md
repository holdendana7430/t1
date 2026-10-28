代发 wailian999

bsearch(&key, a, n, sizeof(int), cmp);
来源：http://hz.xingfuxueyuan.xyz/gtwigtyjob.html

[S21] C：字符类别判断
来源：http://hz.hywenlv.cn/gtyzdqgvuv.html

isdigit(c);  isalpha(c);  isspace(c);
来源：http://hz.zhongyouzk.top/gtfyodatdi.html

[S22] C：字符串转数字
来源：http://hz.pengpengdd.cyou/gtrcmjcmps.html

atoi("42");  strtod("3.14", NULL);
来源：http://hz.cqqwz.cn/gtdacalkpy.html

[S23] C：随机数
来源：http://hz.cashguo.top/gtbqzgaroz.html

srand(time(NULL));  int r = rand() % 100;
来源：http://hz.zhaomingkeji.xyz/gtnavyvbud.html

[S24] C：获取本地时间
来源：http://hz.gogol.net.cn/gtztefdhqv.html

time_t t = time(NULL);  struct tm *tm = localtime(&t);
来源：http://hz.xingfuxueyuan.xyz/gtkakdbawb.html

[S25] C：内存拷贝
来源：http://hz.chenjidiqi.icu/gtlkcckjtb.html

memcpy(dst, src, n);
来源：http://hz.redwolf501.top/gtkvhbhhst.html

[S26] C：内存清零
来源：http://hz.hammf.cn/gttzshvqte.html

memset(a, 0, sizeof a);
来源：http://hz.yvedp.cn/gtfkvxzhao.html

[S27] C：定义常量
来源：http://hz.ywan-chungtsiang.top/gtjjyqxgvz.html

const double PI = 3.14159;
来源：http://hz.tanke756.top/gtlzxmiuup.html

[S28] C：静态变量
来源：http://hz.zhaomingkeji.xyz/gtayfelekf.html

static int counter = 0;
来源：http://hz.wangshuangyany.cn/gtyjdzawnw.html

[S29] C：变参函数
来源：http://hz.gaohongyu789.top/gteupfscxt.html

va_list ap; va_start(ap, fmt); vprintf(fmt, ap); va_end(ap);
来源：http://hz.sweek.top/gtnbknkzci.html

[S30] C：头文件保护
来源：http://hz.zdqjudy.top/gtvfubnbda.html

#ifndef X_H
来源：http://hz.fengsongda.top/gtusabxeti.html

#define X_H
来源：http://hz.pycfn.com/gtiknmknsi.html

#endif
来源：http://hz.tian-w.cn/gtvqhjtqum.html

[S31] C++：Hello World
来源：http://hz.yongpay.top/gtloqzlssr.html

#include <iostream>
来源：http://hz.cashguo.top/gtrwgqgwoe.html

int main() { std::cout << "Hello\n"; }
来源：http://hz.wangdashe.top/gtprdcmrrq.html

[S32] C++：字符串
来源：http://hz.hnqzz.top/gtteisvwjb.html

std::string s = "hi";  s += "!";
来源：http://hz.jiagoushi.top/gtphcstepw.html

[S33] C++：vector 增删
来源：http://hz.yuxming.cn/gthfbohkwy.html

std::vector<int> v{1, 2, 3};  v.push_back(4);
来源：http://hz.hfpthk.cn/gtlsajpaso.html

[S34] C++：遍历 vector
来源：http://hz.jyoumei.cn/gtetkvwuds.html

for (auto &x : v) { std::cout << x; }
来源：http://hz.ivvv.top/gtatgyspza.html

[S35] C++：map
来源：http://hz.birdmap.top/gtaqfiajsn.html

std::map<std::string, int> m;  m["a"] = 1;
来源：http://hz.xingfuxueyuan.xyz/gtebrhvcjn.html

[S36] C++：unordered_map
来源：http://hz.jinqigfzy.top/gtecivgraq.html

std::unordered_map<std::string, int> m;  m["a"] = 1;
来源：http://hz.pengpengdd.cyou/gtorphhwog.html

[S37] C++：set
来源：http://hz.meibo888.top/gtyyzribzb.html

std::set<int> s{1, 2, 3};  s.insert(4);
来源：http://hz.vqdsnc.cn/gtrvefmatj.html

[S38] C++：排序
来源：http://hz.dashuyun.cn/gtcmobelvl.html

std::sort(v.begin(), v.end());
来源：http://hz.ivvv.top/gtavqrkdvu.html

[S39] C++：自定义比较器排序
来源：http://hz.nwbrower.top/gtjjgzhtki.html

std::sort(v.begin(), v.end(), [](int a, int b) { return a > b; });
来源：http://hz.tianlin.xyz/gtndgbcfci.html

[S40] C++：查找元素
来源：http://hz.xuetiantiany.cn/gtyhennbzn.html

auto it = std::find(v.begin(), v.end(), 3);
来源：http://hz.c1oappe.top/gtmtdlhfls.html

[S41] C++：类与构造函数
来源：http://hz.zycfv.cn/gtbljskond.html

class A { public: A(int v) : x_(v) {} int get() const { return x_; } private: int x_; };
来源：http://hz.xuetiantiany.cn/gtxfmxwogy.html

[S42] C++：继承与虚函数
来源：http://hz.c1oappe.top/gtdbubdmcc.html

class B : public Base { public: void f() override {} };
来源：http://hz.hongshengwenyu.top/gtagoaqmsw.html

[S43] C++：智能指针
来源：http://hz.xuanzx.com/gtdnkhnxzi.html

auto p = std::make_unique<int>(5);
来源：http://hz.iojbl.cn/gtqxapjrfk.html

[S44] C++：引用传参
来源：http://hz.hywenlv.cn/gtsajbodxx.html

void inc(int &x) { ++x; }
来源：http://hz.wangdashe.top/gtqclucvdo.html

[S45] C++：lambda
来源：http://hz.shanyushiyangtech.top/gtyhxobhst.html

auto add = [](int a, int b) { return a + b; };
来源：http://hz.wangshuangyany.cn/gtgeiwznqr.html

[S46] C++：函数模板
来源：http://hz.jqgufenzy.top/gtcqzlssan.html

template <typename T> T maxv(T a, T b) { return a > b ? a : b; }
来源：http://hz.jianghu66.top/gtcczflvbd.html

[S47] C++：结构化绑定遍历
来源：http://hz.pengpengdd.cyou/gtqvkoiqmc.html

for (const auto &[k, v] : m) { std::cout << k << v; }
来源：http://hz.jianghu66.top/gteclzsxdg.html

[S48] C++：逐行读文件
来源：http://hz.tanke756.top/gtdxrhcocl.html

std::ifstream in("a.txt");  std::string line;
来源：http://hz.wangshuangyany.cn/gtmjpkavls.html

while (std::getline(in, line)) { }
来源：http://hz.ydzc1.top/gtbiktfgbi.html

[S49] C++：写文件
来源：http://hz.xinyue.icu/gtwttovqfu.html

std::ofstream out("a.txt");  out << "hi\n";
来源：http://hz.tian-w.cn/gtakzodjjp.html

[S50] C++：格式化数字
来源：http://hz.fzhhl.top/gtpcqrrbyd.html

std::ostringstream os;  os << std::fixed << std::setprecision(2) << 3.14159;
来源：http://hz.cheryme.top/gttcbepirw.html

[S51] C++：显式类型转换
来源：http://hz.jiagoushi.top/gtfpodtdph.html

static_cast<double>(a) / b
来源：http://hz.tanke756.top/gtxmfrntpg.html

[S52] C++：const 与 noexcept
来源：http://hz.meibo888.top/gtcmqlzmyu.html

int size() const noexcept { return n_; }
来源：http://hz.svipenyu.cn/gthurtjmwf.html

[S53] C++：移动语义
来源：http://hz.zhixingplan.top/gtkjhuauin.html

std::vector<int> w = std::move(v);
来源：http://hz.meibo888.top/gtkmgvfndz.html

[S54] C++：异常处理
来源：http://hz.cdnleiting.top/gtcwafijor.html

try { throw std::runtime_error("x"); } catch (const std::exception &e) { }
来源：http://hz.dashuyun.cn/gtvpvrpbpc.html

[S55] C++：结构化绑定
来源：http://hz.yj20258888.top/gtnmcdfmvi.html

auto [a, b] = std::make_pair(1, 2);
来源：http://hz.tian-w.cn/gtjbvnhtbk.html

[S56] C++：optional
来源：http://hz.zhengqikj.top/gtnmqsiumh.html

std::optional<int> o = 5;  if (o) { int v = *o; }
来源：http://hz.feifeiyinyue.top/gtuxswvuzf.html

[S57] C++：编译期常量
来源：http://hz.svipenyu.cn/gtbehtslfw.html

constexpr int N = 10;
来源：http://hz.redwolf501.top/gtixgysqvh.html

[S58] C++：命名空间
来源：http://hz.xinyue.icu/gtdjilkfqp.html

namespace ns { int f() { return 1; } }
来源：http://hz.sysykeji.top/gtfnhwgoxv.html

[S59] C++：静态断言
来源：http://hz.yuanzhike.top/gtpwgzebln.html

static_assert(sizeof(int) == 4, "int 必须 4 字节");
来源：http://hz.jlsjyb.cn/gtqhojbzkw.html

[S60] C++：遍历并删除元素
来源：http://hz.xuetiantiany.cn/gtmtudjeii.html

v.erase(std::remove_if(v.begin(), v.end(), [](int x) { return x < 0; }), v.end());
来源：http://hz.redwolf501.top/gtjerhdkxj.html

================================================================================
来源：http://hz.shuidangran.top/gtmlgpqbhh.html

T. 其他语言补充（Kotlin / Swift / Lua / Perl / Scala）
来源：http://hz.nwbrower.top/gtmqpmmoiy.html

================================================================================
来源：http://hz.aibaodan.cn/gtbszgkbqs.html

[T01] Kotlin：Hello World
来源：http://hz.svipenyu.cn/gturtyqapo.html

println("Hello")
来源：http://hz.sufxvd.cn/gtrmmqcuep.html

[T02] Kotlin：变量
来源：http://hz.ywan-chungtsiang.top/gtigbukrfm.html

val a = 1;  var b = 2        // val 只读，var 可变
来源：http://hz.zycfv.cn/gtrnnpxejx.html

[T03] Kotlin：字符串模板
来源：http://hz.xuanzx.com/gtjjbeigtg.html

"值: $b"
来源：http://hz.tian-w.cn/gtxxmkteic.html

[T04] Kotlin：空安全
来源：http://hz.fzhhl.top/gtsrfmbexk.html

val n: String? = null;  n?.length
来源：http://hz.jinqigfzy.top/gtsbxaflvo.html

[T05] Kotlin：when 表达式
来源：http://hz.c1oappe.top/gthcksmtbv.html

val s = when (x) { 1 -> "一" else -> "其他" }   // 多分支时每个分支单独一行
来源：http://hz.xylfe.cn/gtwpzhvmhj.html

[T06] Kotlin：集合映射
来源：http://hz.zycfv.cn/gtoukhufty.html

listOf(1, 2, 3).map { it * 2 }
来源：http://hz.yuanzhike.top/gtlbezinen.html

[T07] Kotlin：集合过滤
来源：http://hz.hnqzz.top/gtoqgzfdvf.html

listOf(1, 2, 3).filter { it > 1 }
来源：http://hz.nwbrower.top/gttvarrntb.html

[T08] Kotlin：数据类
来源：http://hz.tanke756.top/gtfywwxnjj.html

data class User(val name: String, val age: Int)
来源：http://hz.cashguo.top/gtenvnbbax.html

[T09] Kotlin：扩展函数
来源：http://hz.xziqi.cn/gtdctesdjs.html

fun String.exclaim() = this + "!"
来源：http://hz.yj20258.top/gtsgkpouvx.html

[T10] Kotlin：默认参数
来源：http://hz.yanxiufei.cn/gthbnfzahk.html

fun greet(name: String = "World") = "Hi $name"
来源：http://hz.fengsongda.top/gtshwwpndm.html

[T11] Kotlin：协程
来源：http://hz.fengsongda.top/gtfrtaymfw.html

GlobalScope.launch { delay(1000); println("done") }
来源：http://hz.haohaochexian.top/gtjqyzpdrr.html

[T12] Kotlin：解构声明
来源：http://hz.xuanzx.com/gthtxcscov.html

val (a, b) = Pair(1, 2)
来源：http://hz.ywan-chungtsiang.top/gtaguiuvyp.html

[T13] Kotlin：只读 Map
来源：http://hz.ppjwa.cn/gtzliqnuib.html

val m = mapOf("a" to 1)
来源：http://hz.jinqigufen.top/gthqieozmc.html

[T14] Kotlin：循环
来源：http://hz.gzhubu.top/gtwcbdpmkc.html

for (i in 1..10) println(i)
来源：http://hz.fengsongda.top/gtrgfcdijs.html

[T15] Kotlin：接口
来源：http://hz.chenlongwang.top/gtdicpkcra.html

interface Shape { fun area(): Double }
来源：http://hz.hnqzz.top/gtfrnmdjaa.html

[T16] Swift：Hello World
来源：http://hz.sweek.top/gtmatrnxhv.html

print("Hello")
来源：http://hz.redwolf501.top/gtqgzdgunb.html

[T17] Swift：变量与常量
来源：http://hz.zhijiandao.cn/gtvdqgaomb.html

var a = 1;  let b = 2
来源：http://hz.guannengcc.top/gtnrpqheiv.html

[T18] Swift：字符串插值
来源：http://hz.wangdashe.top/gtkriafqki.html

"值: \(b)"
来源：http://hz.jqgufenzy.top/gtegtexwbj.html

[T19] Swift：可选绑定
来源：http://hz.tian-w.cn/gtqihjfpzl.html

if let n = opt { print(n) }
来源：http://hz.ydzc1.top/gtypldrkki.html

[T20] Swift：数组操作
来源：http://hz.zhaomingkeji.xyz/gtvyrxlcim.html

var a = [1, 2, 3];  a.append(4)
来源：http://hz.tianlin.xyz/gtarznnqqm.html

[T21] Swift：遍历
来源：http://hz.fengsongda.top/gtsaiocpay.html

for x in a { print(x) }
来源：http://hz.yonumen.top/gtxjlqukdb.html

[T22] Swift：字典
来源：http://hz.fengsongda.top/gtvicopcgc.html

var d = ["a": 1];  d["b"] = 2
来源：http://hz.cheryme.top/gtskfdiwqt.html

[T23] Swift：函数
来源：http://hz.zhoulong.xyz/gtfwxontze.html

func add(_ a: Int, _ b: Int) -> Int { a + b }
来源：http://hz.daria6918.cn/gtmosedztz.html

[T24] Swift：闭包
来源：http://hz.nanxuanxn.top/gttqiuwgxz.html

let f = { (x: Int) -> Int in x * 2 }
来源：http://hz.jqgfzy.top/gtubltsdnp.html

[T25] Swift：结构体
来源：http://hz.gotoacloud.top/gtpsifwcxa.html

struct P { var x: Int }
来源：http://hz.andypj.xyz/gtlhescwxl.html

[T26] Swift：类与重写
来源：http://hz.svipenyu.cn/gthtjqyqms.html

class A: Base { override func f() {} }
来源：http://hz.yj20258888.top/gtdvknqcpu.html

[T27] Swift：错误处理
来源：http://hz.hnxiangtu.top/gtepywpjou.html

do { try f() } catch { print(error) }
来源：http://hz.yonumen.top/gtraufetee.html

[T28] Swift：枚举
来源：http://hz.9152youxi.cn/gtjylurchz.html

enum Color { case red, green }
来源：http://hz.dashuyun.cn/gtkrzzdvtd.html

[T29] Swift：guard 提前返回
来源：http://hz.ywan-chungtsiang.top/gttamnybdu.html

guard let x = opt else { return }
来源：http://hz.wangshuangyany.cn/gticghbksu.html

[T30] Swift：协议
来源：http://hz.jinqigfzy.top/gtqgtlwsld.html

protocol Shape { func area() -> Double }
来源：http://hz.meibo888.top/gtrgsznrrf.html

[T31] Lua：Hello World
来源：http://hz.chenjidiqi.icu/gtzbmxwtyq.html

print("Hello")
来源：http://hz.andypj.xyz/gtwffboqgb.html

[T32] Lua：局部变量
来源：http://hz.nwbrower.top/gtbfvojkse.html

local a = 1
来源：http://hz.feifeiyinyue.top/gtdbfoatce.html

[T33] Lua：表（数组）
来源：http://hz.vqdsnc.cn/gtifebfadm.html

local t = {1, 2, 3};  t[4] = 4
来源：http://hz.yongpay.top/gttknxfikl.html

[T34] Lua：遍历表
来源：http://hz.c1oappe.top/gtqmwnuymn.html

for i, v in ipairs(t) do print(i, v) end
来源：http://hz.yangfankeji.com/gtwobxbvhw.html

[T35] Lua：字典表
来源：http://hz.hongshengwenyu.top/gtfgegdlye.html

local d = { a = 1 };  d.b = 2
来源：http://hz.zhoulong.xyz/gtfhgxhkjo.html

[T36] Lua：函数
来源：http://hz.zhixingplan.top/gtigkiknkc.html

function add(a, b) return a + b end
来源：http://hz.chenlongwang.top/gtiltjavyc.html

[T37] Lua：字符串拼接
来源：http://hz.shanyushiyangkeji.top/gteccjepvt.html

"a" .. "b"
来源：http://hz.sxryk.cn/gttvbnqzut.html

[T38] Lua：条件
来源：http://hz.wangdashe.top/gtwcmhlmvu.html

if x > 0 then print("正") end
来源：http://hz.jlsjyb.cn/gtffznmtdl.html

[T39] Lua：模式匹配
来源：http://hz.guannengcc.top/gtribnljmh.html

string.find(s, "%d+")
来源：http://hz.zhixingplan.top/gtdababxqr.html

[T40] Lua：元表
来源：http://hz.tian-w.cn/gtdpbuqjax.html

setmetatable({}, { __index = base })
来源：http://hz.andypj.xyz/gtnxrrkgwk.html

[T41] Perl：Hello World
来源：http://hz.xuanzx.com/gthwfebpso.html

print "Hello\n";
来源：http://hz.hywenlv.cn/gthkktpyby.html

[T42] Perl：变量类型
来源：http://hz.cheryme.top/gtntbczvci.html

my $a = 1;  my @arr = (1, 2, 3);  my %h = (a => 1);
来源：http://hz.vqdsnc.cn/gtmavsxyqi.html

[T43] Perl：字符串插值
来源：http://hz.dianchejie.cn/gthqjqpxhp.html

"值: $a"
来源：http://hz.jinyuanbaomall.cn/gtpiyvqynl.html

[T44] Perl：条件
来源：http://hz.xuanzx.com/gtrfulcjda.html

if ($a > 0) { print "正"; }
来源：http://hz.shanyushiyangkeji.top/gtriofubhl.html

[T45] Perl：数组遍历
来源：http://hz.zhaomingkeji.xyz/gtkouvrsav.html

for my $x (@arr) { print $x; }
来源：http://hz.jinqigfzy.top/gtuilipoqv.html

[T46] Perl：哈希操作
来源：http://hz.yj202588.top/gtpebklktj.html

$h{b} = 2;  for my $k (keys %h) { print "$k=$h{$k}"; }
来源：http://hz.ywan-chungtsiang.top/gtixctfvja.html

[T47] Perl：正则捕获
来源：http://hz.jiagoushi.top/gtffvneamm.html

if ($s =~ /(\d+)/) { print $1; }
来源：http://hz.haohaochexian.top/gtjamgdawa.html

[T48] Perl：正则替换
来源：http://hz.pycfn.com/gtqhyqyrgn.html

$s =~ s/old/new/g;
来源：http://hz.guannengcc.top/gtwsjgaudc.html

[T49] Perl：函数
来源：http://hz.ydzc1.top/gtjntiydfb.html

sub add { my ($a, $b) = @_; return $a + $b; }
来源：http://hz.ehwqpu.com/gtmzmkilhp.html

[T50] Perl：逐行读文件
来源：http://hz.yuxming.cn/gtrrchhijg.html

open my $fh, "<", "a.txt" or die $!;
来源：http://hz.ydjk.org.cn/gthnnekrxd.html

while (my $line = <$fh>) { print $line; }
来源：http://hz.zycfv.cn/gtcoaguayl.html

[T51] Scala：Hello World
来源：http://hz.zhaomingkeji.xyz/gtdnbrzlgm.html

println("Hello")
来源：http://hz.chenzaomai.com/gtduwzxbed.html

[T52] Scala：变量
来源：http://hz.ppjwa.cn/gtqwzjiudm.html

val a = 1;  var b = 2
来源：http://hz.ybcxt.top/gtkkzwtsdt.html

[T53] Scala：字符串插值
来源：http://hz.guannengcc.top/gtfxqcmiwo.html

s"值: $b"
来源：http://hz.zhengqikj.top/gtiganngol.html

[T54] Scala：集合映射
来源：http://hz.chenjidiqi.icu/gtuiarlafb.html

List(1, 2, 3).map(_ * 2)
来源：http://hz.52xcode.cn/gtlgnelnni.html

[T55] Scala：集合过滤
来源：http://hz.tianlin.xyz/gtqswnqoqz.html

List(1, 2, 3).filter(_ > 1)
来源：http://hz.iojbl.cn/gtqrpajwco.html

[T56] Scala：样例类
来源：http://hz.c1oappe.top/gtlnzroeig.html

case class User(name: String, age: Int)
来源：http://hz.9152youxi.cn/gtcqsqxfhb.html

[T57] Scala：模式匹配
来源：http://hz.hfpthk.cn/gtywdplqwf.html

x match { case 1 => "一"; case _ => "其他" }
来源：http://hz.gotoacloud.top/gtibcmtnia.html

[T58] Scala：函数定义
来源：http://hz.iojbl.cn/gtyeoasdps.html

def add(a: Int, b: Int): Int = a + b
来源：http://hz.ydzc1.top/gtromiapxj.html

[T59] Scala：循环
来源：http://hz.nanxuanxn.top/gtjcaspukn.html

for (i <- 1 to 10) println(i)
来源：http://hz.aizwys.cn/gtalihvdog.html

[T60] Scala：折叠
来源：http://hz.dianchejie.cn/gtvmoziioy.html

List(1, 2, 3).foldLeft(0)(_ + _)
来源：http://hz.ppjwa.cn/gtwyieyktn.html

================================================================================
来源：http://hz.shanyushiyangkeji.top/gtfumpogon.html

U. 高频实用片段（Python / PHP / JavaScript 各 40 条）
来源：http://hz.xylfe.cn/gtrezimeka.html

================================================================================
来源：http://hz.vqdsnc.cn/gtoegsgheu.html

[U01] Py：创建虚拟环境
来源：http://hz.sysykeji.top/gtsyyzfumu.html

python -m venv .venv && source .venv/bin/activate
来源：http://hz.sweek.top/gtousrpwxo.html

[U02] Py：导出 / 安装依赖
来源：http://hz.chenzaomai.com/gtxpgvurwh.html

pip freeze > requirements.txt;  pip install -r requirements.txt
来源：http://hz.gzhubu.top/gtaivgtcmo.html

[U03] Py：加载 .env 配置
来源：http://hz.yueranfly.top/gtipawrvvl.html

from dotenv import load_dotenv; load_dotenv()
来源：http://hz.xylfe.cn/gtkcsrlork.html

[U04] Py：变量调试打印
来源：http://hz.meibo888.top/gtklsldsci.html

print(f"{x=}")            # 输出 x=值，Python 3.8+
来源：http://hz.hfpthk.cn/gtfdoilpxj.html

[U05] Py：列表去重且保序
来源：http://hz.bjfxy.top/gtavondmka.html

list(dict.fromkeys(arr))
来源：http://hz.snrcjt.cn/gturyrhjan.html

[U06] Py：合并两个字典
来源：http://hz.ppjwa.cn/gtjtzxhrbn.html

{**a, **b}
来源：http://hz.tanke756.top/gtwdirtsgl.html

[U07] Py：反转字典键值
来源：http://hz.zhijiandao.cn/gtmfpyzlzb.html

{v: k for k, v in d.items()}
来源：http://hz.yj202588.top/gtzmnyyxzj.html

[U08] Py：展平二维列表
来源：http://hz.zhijiandao.cn/gtxhdbtyyl.html

[y for x in nested for y in x]
来源：http://hz.kuanghao11.cn/gtuwkjecwd.html

[U09] Py：字典取最大值的键
来源：http://hz.hfpthk.cn/gtostbxfxy.html

max(d, key=d.get)
来源：http://hz.ehwqpu.com/gtgzvbzgat.html

[U10] Py：按值排序字典
来源：http://hz.aizwys.cn/gtqwkvvrcr.html

dict(sorted(d.items(), key=lambda kv: kv[1]))
来源：http://hz.guowangkeji.top/gtsynvefyg.html

[U11] Py：生成器表达式
来源：http://hz.c1oappe.top/gtbvyukgfq.html

(x * 2 for x in arr)
来源：http://hz.daria6918.cn/gtnpzjrelf.html

[U12] Py：取出现最多的 3 个元素
来源：http://hz.fengsongda.top/gtpnavwpcq.html

Counter(arr).most_common(3)
来源：http://hz.tianlin.xyz/gteiqtaimg.html

[U13] Py：固定长度队列
来源：http://hz.hongshengwenyu.top/gtltqiiqrt.html

deque(maxlen=10)
来源：http://hz.bjfxy.top/gttmqnlfky.html

[U14] Py：分组收集到列表
来源：http://hz.jqgfzy.top/gthtudfztl.html

defaultdict(list)
来源：http://hz.shanyushiyangkeji.top/gtsqhgitrl.html

[U15] Py：高精度计时
来源：http://hz.shanyushiyangkeji.top/gtyxpzosih.html

t = time.perf_counter()
来源：http://hz.nanxinkj.top/gtcnujazmf.html

[U16] Py：命令行参数解析
来源：http://hz.hfpthk.cn/gtkmpcyqlh.html

ap = argparse.ArgumentParser();  ap.add_argument("--name");  args = ap.parse_args()
来源：http://hz.yueranfly.top/gtitvscuum.html

[U17] Py：初始化日志
来源：http://hz.jiagoushi.top/gtzskgfvpt.html

logging.basicConfig(level=logging.INFO)
来源：http://hz.hongshengwenyu.top/gtnczrifav.html

[U18] Py：预编译正则
来源：http://hz.mhx1999.top/gtpqunaplc.html

pat = re.compile(r"\d+")
来源：http://hz.shanyushiyangkeji.top/gtkeppzfsx.html

[U19] Py：正则替换带回调
来源：http://hz.tianlin.xyz/gtspswtlor.html

re.sub(r"\d+", lambda m: str(int(m.group()) * 2), s)
来源：http://hz.zhaomingkeji.xyz/gtdqqhgeyq.html

[U20] Py：缓存函数结果
来源：http://hz.zdqjudy.top/gtohlcnhbp.html

@functools.lru_cache(maxsize=None)
来源：http://hz.aizwys.cn/gtrflcrvjo.html

[U21] Py：自定义上下文管理器
来源：http://hz.jinqigufen.top/gtwtvngjof.html

@contextlib.contextmanager
来源：http://hz.sweek.top/gtlrkfcwoa.html

[U22] Py：矩阵转置
来源：http://hz.hfpthk.cn/gtpivrgvas.html

list(zip(*m))
来源：http://hz.zhengqikj.top/gtoknwbrqo.html

[U23] Py：分块读取大文件
来源：http://hz.c1oappe.top/gtcjjrzioe.html

for chunk in iter(lambda: f.read(8192), b""):
来源：http://hz.jqgfzy.top/gtszojgwgf.html

[U24] Py：路径操作
来源：http://hz.daxiang520.top/gtxflugqcq.html

Path("a/b.txt").parent.mkdir(parents=True, exist_ok=True)
来源：http://hz.bjfxy.top/gtfohhswok.html

[U25] Py：CSV 按字典读
来源：http://hz.ppjwa.cn/gtdaoviysp.html

csv.DictReader(f)
来源：http://hz.smart0.xyz/gtgpzbfbde.html

[U26] Py：并发下载
来源：http://hz.jinyuanbaomall.cn/gtfszgvvrs.html

ThreadPoolExecutor(max_workers=8).map(fetch, urls)
来源：http://hz.jinghuilouyu.cn/gtbrqkgytt.html

[U27] Py：异步 HTTP
来源：http://hz.chenzaomai.com/gtsvaqysok.html

aiohttp.ClientSession() 配合 async with
来源：http://hz.ivvv.top/gtjtprfxgr.html

[U28] Py：类型别名
来源：http://hz.yanxiufei.cn/gtrtottzrt.html

UserId = int
来源：http://hz.tian-w.cn/gtnwolibzd.html

[U29] Py：属性校验
来源：http://hz.hywenlv.cn/gtiwmwjwue.html

@property 与 @x.setter 配合
来源：http://hz.zdqjudy.top/gtgdpdxfeg.html

[U30] Py：数据类
来源：http://hz.jianghu66.top/gtfmvzostj.html

@dataclass(slots=True)
来源：http://hz.haohaochexian.top/gtjffmypbz.html

[U31] Py：单测
来源：http://hz.jqgufenzy.top/gtagzztktv.html

python -m pytest -q
来源：http://hz.bjfxy.top/gtxgsgqevi.html

[U32] Py：代码格式化
来源：http://hz.shangyingyoupin.top/gtivagkzuc.html

ruff format . && ruff check --fix .
来源：http://hz.cheryme.top/gtjuiiacov.html

[U33] Py：打包发布
来源：http://hz.zdqjudy.top/gtpogzbidz.html

python -m build  （依赖 pyproject.toml）
来源：http://hz.smart0.xyz/gtgwqopdmw.html

[U34] Py：判断编码
来源：http://hz.cqqwz.cn/gtaejxpwta.html

chardet.detect(raw)
来源：http://hz.yanxiufei.cn/gtfqgrqqqs.html

[U35] Py：发送邮件
来源：http://hz.kuanghao11.cn/gtmavxgghn.html

smtplib.SMTP_SSL(...).send_message(msg)
来源：http://hz.nwbrower.top/gtbtcrgpcu.html

[U36] Py：定时任务
来源：http://hz.daria6918.cn/gtgyvqjwpl.html

schedule.every(10).minutes.do(job)
来源：http://hz.pengpengdd.cyou/gtxeizamqg.html

[U37] Py：读写 Excel
来源：http://hz.daxiang520.top/gtxomudnqw.html

pandas.read_excel / DataFrame.to_excel
来源：http://hz.aibaodan.cn/gtznrutztc.html

[U38] Py：获取脚本所在目录
来源：http://hz.jlsjyb.cn/gtlguzcrnq.html

Path(__file__).resolve().parent
来源：http://hz.dianchejie.cn/gtouvarcim.html

[U39] Py：判断是否在交互环境
来源：http://hz.gotoacloud.top/gtddqylzfz.html

sys.stdout.isatty()
来源：http://hz.cqqwz.cn/gtkwjxglzq.html

[U40] Py：打印到标准错误
来源：http://hz.yvedp.cn/gtfsbdupur.html

print("err", file=sys.stderr)
来源：http://hz.zhoulong.xyz/gtqrrunhlv.html

[U41] PHP：初始化 Composer 项目
来源：http://hz.chenlongwang.top/gtxxdiqliu.html

composer init;  composer require guzzlehttp/guzzle
来源：http://hz.bjfxy.top/gtjbjlpxce.html

[U42] PHP：PSR-4 自动加载
来源：http://hz.hywenlv.cn/gtrslkyrqz.html

"autoload": { "psr-4": { "App\\": "src/" } }
来源：http://hz.gzhubu.top/gtzlducber.html

[U43] PHP：声明命名空间
来源：http://hz.ydjk.org.cn/gtdhhgokac.html

namespace App\Http;
来源：http://hz.iojbl.cn/gtksdtacbr.html

[U44] PHP：开启严格类型
来源：http://hz.mhx1999.top/gtatnhmona.html

declare(strict_types=1);
来源：http://hz.guannengcc.top/gtshgherjp.html


<!-- 参考信息 -->