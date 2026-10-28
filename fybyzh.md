代发 wailian999

time_t t = time(NULL);  struct tm *tm = localtime(&t);
来源：http://hz.nanxinkj.top/gtaxqkgyxp.html

[S25] C：内存拷贝
来源：http://hz.jyoumei.cn/gtnwbxagfc.html

memcpy(dst, src, n);
来源：http://hz.chenzaomai.com/gthgxhtqxi.html

[S26] C：内存清零
来源：http://hz.iojbl.cn/gtspltfuzp.html

memset(a, 0, sizeof a);
来源：http://hz.pycfn.com/gtywfsflqi.html

[S27] C：定义常量
来源：http://hz.hnqzz.top/gtkwbuokev.html

const double PI = 3.14159;
来源：http://hz.andypj.xyz/gtyzxcmguo.html

[S28] C：静态变量
来源：http://hz.nwbrower.top/gtplvinnkl.html

static int counter = 0;
来源：http://hz.zhoulong.xyz/gtujjbdtzd.html

[S29] C：变参函数
来源：http://hz.svipenyu.cn/gtjcdtdxbd.html

va_list ap; va_start(ap, fmt); vprintf(fmt, ap); va_end(ap);
来源：http://hz.cdnleiting.top/gtcbrsylsw.html

[S30] C：头文件保护
来源：http://hz.tianlin.xyz/gtvqlgaysd.html

#ifndef X_H
来源：http://hz.yuanzhike.top/gtrsgtjoxg.html

#define X_H
来源：http://hz.redwolf501.top/gtjlimxvay.html

#endif
来源：http://hz.shanyushiyangtech.top/gtwjfwxxne.html

[S31] C++：Hello World
来源：http://hz.nwbrower.top/gtxbtfprbg.html

#include <iostream>
来源：http://hz.sxryk.cn/gtqycbkbkk.html

int main() { std::cout << "Hello\n"; }
来源：http://hz.bjfxy.top/gtempvpavt.html

[S32] C++：字符串
来源：http://hz.dianchejie.cn/gtnwkbloxk.html

std::string s = "hi";  s += "!";
来源：http://hz.mhx1999.top/gtvquhxqnp.html

[S33] C++：vector 增删
来源：http://hz.cdnleiting.top/gtqmirsozl.html

std::vector<int> v{1, 2, 3};  v.push_back(4);
来源：http://hz.yuanzhike.top/gtiemiyopa.html

[S34] C++：遍历 vector
来源：http://hz.zhongyouzk.top/gtrnazhiaj.html

for (auto &x : v) { std::cout << x; }
来源：http://hz.jinyuanbaomall.cn/gtzibkoaor.html

[S35] C++：map
来源：http://hz.jlsjyb.cn/gtqdihjflb.html

std::map<std::string, int> m;  m["a"] = 1;
来源：http://hz.hywenlv.cn/gthuldyuqj.html

[S36] C++：unordered_map
来源：http://hz.daria6918.cn/gtnlgjkcsp.html

std::unordered_map<std::string, int> m;  m["a"] = 1;
来源：http://hz.havefunace.top/gtafumptby.html

[S37] C++：set
来源：http://hz.andypj.xyz/gtqfvivpko.html

std::set<int> s{1, 2, 3};  s.insert(4);
来源：http://hz.yangfankeji.com/gtwyprysdr.html

[S38] C++：排序
来源：http://hz.gzhubu.top/gtvktllzbj.html

std::sort(v.begin(), v.end());
来源：http://hz.cucudq.cn/gtqwnwpvyv.html

[S39] C++：自定义比较器排序
来源：http://hz.0kj1m.cn/gtfnkrttcv.html

std::sort(v.begin(), v.end(), [](int a, int b) { return a > b; });
来源：http://hz.gaohongyu789.top/gtzbneziho.html

[S40] C++：查找元素
来源：http://hz.shuidangran.top/gtetrxmnqp.html

auto it = std::find(v.begin(), v.end(), 3);
来源：http://hz.yj20258.top/gthyuzwsxa.html

[S41] C++：类与构造函数
来源：http://hz.zhiwuduotai.top/gtjrbqdsio.html

class A { public: A(int v) : x_(v) {} int get() const { return x_; } private: int x_; };
来源：http://hz.guowangkeji.top/gtwsnitgux.html

[S42] C++：继承与虚函数
来源：http://hz.yuanzhike.top/gtnzkmcxvj.html

class B : public Base { public: void f() override {} };
来源：http://hz.sweek.top/gttypioneh.html

[S43] C++：智能指针
来源：http://hz.shanyushiyangkeji.top/gtxpdshqce.html

auto p = std::make_unique<int>(5);
来源：http://hz.yonumen.top/gtqdwjnwpy.html

[S44] C++：引用传参
来源：http://hz.havefunace.top/gtlhunoyok.html

void inc(int &x) { ++x; }
来源：http://hz.jqgfzy.top/gtcxcspiuk.html

[S45] C++：lambda
来源：http://hz.ppjwa.cn/gtrlhgumqe.html

auto add = [](int a, int b) { return a + b; };
来源：http://hz.cucudq.cn/gtdedtehrd.html

[S46] C++：函数模板
来源：http://hz.dashuyun.cn/gtniisekhm.html

template <typename T> T maxv(T a, T b) { return a > b ? a : b; }
来源：http://hz.daxiang520.top/gtznbmbylr.html

[S47] C++：结构化绑定遍历
来源：http://hz.kuanghao11.cn/gtppxkorcf.html

for (const auto &[k, v] : m) { std::cout << k << v; }
来源：http://hz.svipenyu.cn/gtyglknohz.html

[S48] C++：逐行读文件
来源：http://hz.mhx1999.top/gtgohznewu.html

std::ifstream in("a.txt");  std::string line;
来源：http://hz.hammf.cn/gtsmfvatvr.html

while (std::getline(in, line)) { }
来源：http://hz.zycfv.cn/gtsjwjnewj.html

[S49] C++：写文件
来源：http://hz.feifeiyinyue.top/gtzxrpapcq.html

std::ofstream out("a.txt");  out << "hi\n";
来源：http://hz.ybcxt.top/gtvpongzpg.html

[S50] C++：格式化数字
来源：http://hz.shzxlz.cn/gtrdalbdth.html

std::ostringstream os;  os << std::fixed << std::setprecision(2) << 3.14159;
来源：http://hz.nanxuanxn.top/gtfvjfiqpc.html

[S51] C++：显式类型转换
来源：http://hz.52xcode.cn/gteehxxbsw.html

static_cast<double>(a) / b
来源：http://hz.haohaochexian.top/gtmoeofdju.html

[S52] C++：const 与 noexcept
来源：http://hz.zycfv.cn/gtcdeujlhc.html

int size() const noexcept { return n_; }
来源：http://hz.gotoacloud.top/gtpddgsnwf.html

[S53] C++：移动语义
来源：http://hz.sweek.top/gtdpysuchh.html

std::vector<int> w = std::move(v);
来源：http://hz.hnxiangtu.top/gtddaugwql.html

[S54] C++：异常处理
来源：http://hz.yueranfly.top/gtqbrwoyyq.html

try { throw std::runtime_error("x"); } catch (const std::exception &e) { }
来源：http://hz.yj202588.top/gtjttqxpux.html

[S55] C++：结构化绑定
来源：http://hz.wangshuangyany.cn/gtqkgvjfwl.html

auto [a, b] = std::make_pair(1, 2);
来源：http://hz.cdnleiting.top/gtmbxaanrn.html

[S56] C++：optional
来源：http://hz.ywan-chungtsiang.top/gtrzkvqrac.html

std::optional<int> o = 5;  if (o) { int v = *o; }
来源：http://hz.aizwys.cn/gtnqskvcqh.html

[S57] C++：编译期常量
来源：http://hz.aibaodan.cn/gttmejewyh.html

constexpr int N = 10;
来源：http://hz.aibaodan.cn/gtvxsknwyz.html

[S58] C++：命名空间
来源：http://hz.sxryk.cn/gthtiqefhd.html

namespace ns { int f() { return 1; } }
来源：http://hz.nanxuanxn.top/gtojxhocjy.html

[S59] C++：静态断言
来源：http://hz.yanxiufei.cn/gtjifsjkon.html

static_assert(sizeof(int) == 4, "int 必须 4 字节");
来源：http://hz.aibaodan.cn/gtcgvrbwcg.html

[S60] C++：遍历并删除元素
来源：http://hz.hysaishi.cn/gtjvkdteji.html

v.erase(std::remove_if(v.begin(), v.end(), [](int x) { return x < 0; }), v.end());
来源：http://hz.yueranfly.top/gtkwblpwem.html

================================================================================
来源：http://hz.hammf.cn/gtdaaqijpq.html

T. 其他语言补充（Kotlin / Swift / Lua / Perl / Scala）
来源：http://hz.birdmap.top/gtastcctad.html

================================================================================
来源：http://hz.chenzaomai.com/gtwzcpdnzd.html

[T01] Kotlin：Hello World
来源：http://hz.daxiang520.top/gtrcchlqrk.html

println("Hello")
来源：http://hz.yuxming.cn/gtosnallqi.html

[T02] Kotlin：变量
来源：http://hz.sweek.top/gtffdmsaxf.html

val a = 1;  var b = 2        // val 只读，var 可变
来源：http://hz.havefunace.top/gtjyuvmcbk.html

[T03] Kotlin：字符串模板
来源：http://hz.jlsjyb.cn/gtwwgrjeuq.html

"值: $b"
来源：http://hz.shanyushiyangtech.top/gticdyxgsq.html

[T04] Kotlin：空安全
来源：http://hz.xziqi.cn/gtvtdtsbno.html

val n: String? = null;  n?.length
来源：http://hz.feifeiyinyue.top/gtijcjjmiy.html

[T05] Kotlin：when 表达式
来源：http://hz.tianlin.xyz/gtekxoqfkf.html

val s = when (x) { 1 -> "一" else -> "其他" }   // 多分支时每个分支单独一行
来源：http://hz.gogol.net.cn/gtulqwjinp.html

[T06] Kotlin：集合映射
来源：http://hz.zhengqikj.top/gtfjulcrjk.html

listOf(1, 2, 3).map { it * 2 }
来源：http://hz.316326.xyz/gtcsmcywrj.html

[T07] Kotlin：集合过滤
来源：http://hz.hywenlv.cn/gtgykbsibr.html

listOf(1, 2, 3).filter { it > 1 }
来源：http://hz.sysykeji.top/gtuhdjwvzf.html

[T08] Kotlin：数据类
来源：http://hz.cdnleiting.top/gtsrhhpnoj.html

data class User(val name: String, val age: Int)
来源：http://hz.ehwqpu.com/gtykyoneld.html

[T09] Kotlin：扩展函数
来源：http://hz.yvedp.cn/gtepdvtvgc.html

fun String.exclaim() = this + "!"
来源：http://hz.hammf.cn/gtimodypsn.html

[T10] Kotlin：默认参数
来源：http://hz.zdqjudy.top/gtzvtxieyi.html

fun greet(name: String = "World") = "Hi $name"
来源：http://hz.yj20258.top/gtiyepdigl.html

[T11] Kotlin：协程
来源：http://hz.hywenlv.cn/gtstsqzqqy.html

GlobalScope.launch { delay(1000); println("done") }
来源：http://hz.0kj1m.cn/gttuqlelcm.html

[T12] Kotlin：解构声明
来源：http://hz.cheryme.top/gtatnytlxp.html

val (a, b) = Pair(1, 2)
来源：http://hz.aibaodan.cn/gtkourzjcm.html

[T13] Kotlin：只读 Map
来源：http://hz.pycfn.com/gtnbbqshkj.html

val m = mapOf("a" to 1)
来源：http://hz.aibaodan.cn/gtqwwktpns.html

[T14] Kotlin：循环
来源：http://hz.shanyushiyangkeji.top/gtrwspvxfy.html

for (i in 1..10) println(i)
来源：http://hz.zycfv.cn/gtpnimznsa.html

[T15] Kotlin：接口
来源：http://hz.shanyushiyangtech.top/gtrzehcgbo.html

interface Shape { fun area(): Double }
来源：http://hz.guowangkeji.top/gtcewxzela.html

[T16] Swift：Hello World
来源：http://hz.andypj.xyz/gticbrrmay.html

print("Hello")
来源：http://hz.yuxming.cn/gtryausdkl.html

[T17] Swift：变量与常量
来源：http://hz.chenjidiqi.icu/gtmswmwzdj.html

var a = 1;  let b = 2
来源：http://hz.xziqi.cn/gtwsyoszsd.html

[T18] Swift：字符串插值
来源：http://hz.jinqigufen.top/gtqjeaqsdu.html

"值: \(b)"
来源：http://hz.ydzc1.top/gtsjkhmmta.html

[T19] Swift：可选绑定
来源：http://hz.pycfn.com/gtcjgkpblq.html

if let n = opt { print(n) }
来源：http://hz.sxryk.cn/gtlvtfjwjl.html

[T20] Swift：数组操作
来源：http://hz.daria6918.cn/gthkfjtnrn.html

var a = [1, 2, 3];  a.append(4)
来源：http://hz.hysaishi.cn/gtnxzwcfbj.html

[T21] Swift：遍历
来源：http://hz.zycfv.cn/gtyfyydlqv.html

for x in a { print(x) }
来源：http://hz.aibaodan.cn/gtuegamrtp.html

[T22] Swift：字典
来源：http://hz.sweek.top/gtwrozjqng.html

var d = ["a": 1];  d["b"] = 2
来源：http://hz.kuanghao11.cn/gtezxdprhk.html

[T23] Swift：函数
来源：http://hz.tanke756.top/gtwanzcdgk.html

func add(_ a: Int, _ b: Int) -> Int { a + b }
来源：http://hz.zhoulong.xyz/gtvrcjebcz.html

[T24] Swift：闭包
来源：http://hz.zhiwuduotai.top/gtgaicqxhl.html

let f = { (x: Int) -> Int in x * 2 }
来源：http://hz.guannengcc.top/gtmplbhxre.html

[T25] Swift：结构体
来源：http://hz.tianlin.xyz/gtgchpdwbl.html

struct P { var x: Int }
来源：http://hz.yongpay.top/gtpaktaojx.html

[T26] Swift：类与重写
来源：http://hz.snrcjt.cn/gthmurprar.html

class A: Base { override func f() {} }
来源：http://hz.jinqigfzy.top/gtadjogvtc.html

[T27] Swift：错误处理
来源：http://hz.jinyuanbaomall.cn/gtpattftxg.html

do { try f() } catch { print(error) }
来源：http://hz.xuetiantiany.cn/gtcgalasil.html

[T28] Swift：枚举
来源：http://hz.zycfv.cn/gtxyflgazj.html

enum Color { case red, green }
来源：http://hz.ppjwa.cn/gtrzqkrfdr.html

[T29] Swift：guard 提前返回
来源：http://hz.sweek.top/gtrurinvdd.html

guard let x = opt else { return }
来源：http://hz.tianlin.xyz/gthqeghbea.html

[T30] Swift：协议
来源：http://hz.ivvv.top/gtqbzmmmjf.html

protocol Shape { func area() -> Double }
来源：http://hz.iojbl.cn/gtfmbuhsqp.html

[T31] Lua：Hello World
来源：http://hz.shanyushiyangtech.top/gtnktrehmt.html

print("Hello")
来源：http://hz.shanyushiyangtech.top/gthogwpkbo.html

[T32] Lua：局部变量
来源：http://hz.xziqi.cn/gthifrywza.html

local a = 1
来源：http://hz.quarkkingdee.top/gtynchflvo.html

[T33] Lua：表（数组）
来源：http://hz.sweek.top/gthzoiwfga.html

local t = {1, 2, 3};  t[4] = 4
来源：http://hz.jyoumei.cn/gtqiwabsjr.html

[T34] Lua：遍历表
来源：http://hz.sweek.top/gtznptlkbt.html

for i, v in ipairs(t) do print(i, v) end
来源：http://hz.pengpengdd.cyou/gtlpkqjgzt.html

[T35] Lua：字典表
来源：http://hz.xylfe.cn/gtkdbryxxc.html

local d = { a = 1 };  d.b = 2
来源：http://hz.jlsjyb.cn/gtiqqottkf.html

[T36] Lua：函数
来源：http://hz.bjfxy.top/gtacsmtizs.html

function add(a, b) return a + b end
来源：http://hz.zhoulong.xyz/gtznaspmvn.html

[T37] Lua：字符串拼接
来源：http://hz.pycfn.com/gtrcvcupdn.html

"a" .. "b"
来源：http://hz.ydjk.org.cn/gtdezrqxms.html

[T38] Lua：条件
来源：http://hz.hywenlv.cn/gtdshwvkoz.html

if x > 0 then print("正") end
来源：http://hz.yuxming.cn/gtxjzltlid.html

[T39] Lua：模式匹配
来源：http://hz.xuanzx.com/gtocrerwfr.html

string.find(s, "%d+")
来源：http://hz.guowangkeji.top/gtjmwmfown.html

[T40] Lua：元表
来源：http://hz.gogol.net.cn/gtbjzbznow.html

setmetatable({}, { __index = base })
来源：http://hz.aizwys.cn/gtcuindzzh.html

[T41] Perl：Hello World
来源：http://hz.birdmap.top/gtukhxwqbk.html

print "Hello\n";
来源：http://hz.zhongyouzk.top/gtffnoympz.html

[T42] Perl：变量类型
来源：http://hz.mhx1999.top/gtlfxfmogr.html

my $a = 1;  my @arr = (1, 2, 3);  my %h = (a => 1);
来源：http://hz.tanke756.top/gtbinjkegj.html

[T43] Perl：字符串插值
来源：http://hz.chenzaomai.com/gtlmvcrsys.html

"值: $a"
来源：http://hz.zhijiandao.cn/gttkibfgkd.html

[T44] Perl：条件
来源：http://hz.zhijiandao.cn/gtlurwighy.html

if ($a > 0) { print "正"; }
来源：http://hz.pycfn.com/gtwwjetqci.html

[T45] Perl：数组遍历
来源：http://hz.jinyuanbaomall.cn/gtnjkimvcn.html

for my $x (@arr) { print $x; }
来源：http://hz.ivvv.top/gtnlwchkkc.html

[T46] Perl：哈希操作
来源：http://hz.yj20258.top/gtndoxtzhn.html

$h{b} = 2;  for my $k (keys %h) { print "$k=$h{$k}"; }
来源：http://hz.ydjk.org.cn/gtepbdjzfg.html

[T47] Perl：正则捕获
来源：http://hz.gotoacloud.top/gtelhrpjgv.html

if ($s =~ /(\d+)/) { print $1; }
来源：http://hz.feifeiyinyue.top/gtlsmdccii.html

[T48] Perl：正则替换
来源：http://hz.ybcxt.top/gthcebjuxh.html

$s =~ s/old/new/g;
来源：http://hz.9152youxi.cn/gtkcicfzio.html

[T49] Perl：函数
来源：http://hz.zhoulong.xyz/gtipuvbbwt.html

sub add { my ($a, $b) = @_; return $a + $b; }
来源：http://hz.guowangkeji.top/gtfpyfqntm.html

[T50] Perl：逐行读文件
来源：http://hz.yangfankeji.com/gteedtxeos.html

open my $fh, "<", "a.txt" or die $!;
来源：http://hz.havefunace.top/gtuamhaarh.html

while (my $line = <$fh>) { print $line; }
来源：http://hz.sufxvd.cn/gtgalxytjv.html

[T51] Scala：Hello World
来源：http://hz.havefunace.top/gtyqsxukfd.html

println("Hello")
来源：http://hz.nwbrower.top/gtdtrobggv.html

[T52] Scala：变量
来源：http://hz.mhx1999.top/gteqolxyka.html

val a = 1;  var b = 2
来源：http://hz.hongshengwenyu.top/gtpqgnmxhm.html

[T53] Scala：字符串插值
来源：http://hz.dashuyun.cn/gtibnquqsh.html

s"值: $b"
来源：http://hz.pengpengdd.cyou/gtvovkbhzf.html

[T54] Scala：集合映射
来源：http://hz.yj20258.top/gtlnjkvgzh.html

List(1, 2, 3).map(_ * 2)
来源：http://hz.xziqi.cn/gtzbzxxebt.html

[T55] Scala：集合过滤
来源：http://hz.kuanghao11.cn/gtsequlrvd.html

List(1, 2, 3).filter(_ > 1)
来源：http://hz.dianchejie.cn/gtsnfmmgha.html

[T56] Scala：样例类
来源：http://hz.ybcxt.top/gtmbapaweh.html

case class User(name: String, age: Int)
来源：http://hz.52xcode.cn/gtywezgakz.html

[T57] Scala：模式匹配
来源：http://hz.ehwqpu.com/gtzhsbzkhh.html

x match { case 1 => "一"; case _ => "其他" }
来源：http://hz.dianchejie.cn/gtmkpvawgi.html

[T58] Scala：函数定义
来源：http://hz.jianghu66.top/gtpxyhxybp.html

def add(a: Int, b: Int): Int = a + b
来源：http://hz.yvedp.cn/gthjjgsxsa.html

[T59] Scala：循环
来源：http://hz.c1oappe.top/gtkgvvaucr.html

for (i <- 1 to 10) println(i)
来源：http://hz.jyoumei.cn/gtxttvcijl.html

[T60] Scala：折叠
来源：http://hz.vqdsnc.cn/gtvsdnrsna.html

List(1, 2, 3).foldLeft(0)(_ + _)
来源：http://hz.shuidangran.top/gtxewasvij.html

================================================================================
来源：http://hz.xuetiantiany.cn/gtapwekwks.html

U. 高频实用片段（Python / PHP / JavaScript 各 40 条）
来源：http://hz.nanxinkj.top/gtzukzxyik.html

================================================================================
来源：http://hz.nwbrower.top/gttoxxglle.html

[U01] Py：创建虚拟环境
来源：http://hz.tian-w.cn/gtnypwzjrh.html

python -m venv .venv && source .venv/bin/activate
来源：http://hz.daria6918.cn/gtxkfpoeqv.html

[U02] Py：导出 / 安装依赖
来源：http://hz.daxiang520.top/gttkswhgyu.html

pip freeze > requirements.txt;  pip install -r requirements.txt
来源：http://hz.yanxiufei.cn/gtmzhahqxg.html

[U03] Py：加载 .env 配置
来源：http://hz.hongshengwenyu.top/gtqbymtdoj.html

from dotenv import load_dotenv; load_dotenv()
来源：http://hz.gzhubu.top/gtzjcawvya.html

[U04] Py：变量调试打印
来源：http://hz.daxiang520.top/gtmfqkyayj.html

print(f"{x=}")            # 输出 x=值，Python 3.8+
来源：http://hz.zycfv.cn/gtzwcpmtby.html

[U05] Py：列表去重且保序
来源：http://hz.sufxvd.cn/gtylmkyghz.html

list(dict.fromkeys(arr))
来源：http://hz.jianghu66.top/gtfxmnjtze.html

[U06] Py：合并两个字典
来源：http://hz.yj202588.top/gtbbzrhyov.html

{**a, **b}
来源：http://hz.sweek.top/gttqzvdzze.html

[U07] Py：反转字典键值
来源：http://hz.zhijiandao.cn/gttijhzpqs.html

{v: k for k, v in d.items()}
来源：http://hz.shanyushiyangkeji.top/gtioyszkov.html

[U08] Py：展平二维列表
来源：http://hz.xuetiantiany.cn/gtgaraermq.html

[y for x in nested for y in x]
来源：http://hz.xingfuxueyuan.xyz/gththpjtyr.html

[U09] Py：字典取最大值的键
来源：http://hz.jinqigfzy.top/gtfkqwdzog.html

max(d, key=d.get)
来源：http://hz.fzhhl.top/gttbaeeaxc.html

[U10] Py：按值排序字典
来源：http://hz.zhongyouzk.top/gtfpitccmc.html

dict(sorted(d.items(), key=lambda kv: kv[1]))
来源：http://hz.zhixingplan.top/gtazeoidoh.html

[U11] Py：生成器表达式
来源：http://hz.zhiwuduotai.top/gthanpyhxu.html

(x * 2 for x in arr)
来源：http://hz.haohaochexian.top/gtdgwxzdsq.html

[U12] Py：取出现最多的 3 个元素
来源：http://hz.yuanzhike.top/gtjbpqilmq.html

Counter(arr).most_common(3)
来源：http://hz.shuidangran.top/gtozuafuxe.html

[U13] Py：固定长度队列
来源：http://hz.iojbl.cn/gtuetbkqbz.html

deque(maxlen=10)
来源：http://hz.zhiwuduotai.top/gtekupgsgy.html

[U14] Py：分组收集到列表
来源：http://hz.jinqigfzy.top/gtvxnzzksj.html

defaultdict(list)
来源：http://hz.cheryme.top/gtfpokmpjk.html

[U15] Py：高精度计时
来源：http://hz.jqgufenzy.top/gtwfbgjksw.html

t = time.perf_counter()
来源：http://hz.sufxvd.cn/gtnljnrenm.html

[U16] Py：命令行参数解析
来源：http://hz.zhongyouzk.top/gtfguemans.html

ap = argparse.ArgumentParser();  ap.add_argument("--name");  args = ap.parse_args()
来源：http://hz.xingfuxueyuan.xyz/gtimyhmqml.html

[U17] Py：初始化日志
来源：http://hz.yongpay.top/gthiqussur.html

logging.basicConfig(level=logging.INFO)
来源：http://hz.fengsongda.top/gtvfgdphdp.html

[U18] Py：预编译正则
来源：http://hz.yj20258.top/gtguiqqmko.html

pat = re.compile(r"\d+")
来源：http://hz.jqgufenzy.top/gtfgdghxqs.html

[U19] Py：正则替换带回调
来源：http://hz.cdnleiting.top/gtiharlmjz.html

re.sub(r"\d+", lambda m: str(int(m.group()) * 2), s)
来源：http://hz.sweek.top/gtczndvzcf.html

[U20] Py：缓存函数结果
来源：http://hz.fzhhl.top/gtackxcxtz.html

@functools.lru_cache(maxsize=None)
来源：http://hz.dianchejie.cn/gtljjnccsd.html

[U21] Py：自定义上下文管理器
来源：http://hz.yanxiufei.cn/gtujfegcma.html

@contextlib.contextmanager
来源：http://hz.dashuyun.cn/gtxwpftnsn.html

[U22] Py：矩阵转置
来源：http://hz.fzhhl.top/gtvuhdmqrm.html

list(zip(*m))
来源：http://hz.ybcxt.top/gtlglwptpd.html

[U23] Py：分块读取大文件
来源：http://hz.zhixingplan.top/gtllfxbsud.html

for chunk in iter(lambda: f.read(8192), b""):
来源：http://hz.gogol.net.cn/gtvdvdemrr.html

[U24] Py：路径操作
来源：http://hz.ydjk.org.cn/gtunovvell.html

Path("a/b.txt").parent.mkdir(parents=True, exist_ok=True)
来源：http://hz.jqgufenzy.top/gtlwwkowjb.html

[U25] Py：CSV 按字典读
来源：http://hz.jqgfzy.top/gtyhmkyhyi.html

csv.DictReader(f)
来源：http://hz.hywenlv.cn/gtkzvkagja.html

[U26] Py：并发下载
来源：http://hz.bjfxy.top/gtbqqrtgbs.html

ThreadPoolExecutor(max_workers=8).map(fetch, urls)
来源：http://hz.shangyingyoupin.top/gtkegycqkq.html

[U27] Py：异步 HTTP
来源：http://hz.nanxuanxn.top/gtiddxtlxh.html

aiohttp.ClientSession() 配合 async with
来源：http://hz.zycfv.cn/gtgypgfbsq.html

[U28] Py：类型别名
来源：http://hz.yuanzhike.top/gtqjchukfd.html

UserId = int
来源：http://hz.fzhhl.top/gtxdsxvzah.html

[U29] Py：属性校验
来源：http://hz.hammf.cn/gtwgegklkb.html

@property 与 @x.setter 配合
来源：http://hz.hnxiangtu.top/gtpfhvigfy.html

[U30] Py：数据类
来源：http://hz.tanke756.top/gtkfllnkpq.html

@dataclass(slots=True)
来源：http://hz.9152youxi.cn/gtltjguzdc.html

[U31] Py：单测
来源：http://hz.yanxiufei.cn/gtjiblyuhq.html

python -m pytest -q
来源：http://hz.hywenlv.cn/gtjbrsnowy.html

[U32] Py：代码格式化
来源：http://hz.smart0.xyz/gtvrucbkxa.html

ruff format . && ruff check --fix .
来源：http://hz.snrcjt.cn/gtwwnlxrps.html

[U33] Py：打包发布
来源：http://hz.aibaodan.cn/gtdvaqokqf.html

python -m build  （依赖 pyproject.toml）
来源：http://hz.ywan-chungtsiang.top/gttvbfljsv.html

[U34] Py：判断编码
来源：http://hz.quarkkingdee.top/gtnlweuxrr.html

chardet.detect(raw)
来源：http://hz.haohaochexian.top/gtajejutjq.html

[U35] Py：发送邮件
来源：http://hz.ywan-chungtsiang.top/gthyrwznnf.html

smtplib.SMTP_SSL(...).send_message(msg)
来源：http://hz.xuanzx.com/gtbhlbmaou.html

[U36] Py：定时任务
来源：http://hz.jinghuilouyu.cn/gteunliunm.html

schedule.every(10).minutes.do(job)
来源：http://hz.gotoacloud.top/gtannfcnmk.html

[U37] Py：读写 Excel
来源：http://hz.zdqjudy.top/gtlnazpnth.html

pandas.read_excel / DataFrame.to_excel
来源：http://hz.jqgfzy.top/gtuqracffj.html

[U38] Py：获取脚本所在目录
来源：http://hz.yj202588.top/gtbsaqadxv.html

Path(__file__).resolve().parent
来源：http://hz.jqgufenzy.top/gtfvvavqop.html

[U39] Py：判断是否在交互环境
来源：http://hz.tanke756.top/gtnacfvjab.html

sys.stdout.isatty()
来源：http://hz.zhiwuduotai.top/gtwvpwvqap.html

[U40] Py：打印到标准错误
来源：http://hz.jinqigfzy.top/gtbwwzpuea.html

print("err", file=sys.stderr)
来源：http://hz.tanke756.top/gthvqtfail.html

[U41] PHP：初始化 Composer 项目
来源：http://hz.jinghuilouyu.cn/gtjeyrzyag.html

composer init;  composer require guzzlehttp/guzzle
来源：http://hz.sxryk.cn/gtivtmpyna.html

[U42] PHP：PSR-4 自动加载
来源：http://hz.jqgufenzy.top/gtirosprif.html

"autoload": { "psr-4": { "App\\": "src/" } }
来源：http://hz.jinghuilouyu.cn/gtpjsfvxvv.html

[U43] PHP：声明命名空间
来源：http://hz.havefunace.top/gtvfcgjkkf.html

namespace App\Http;
来源：http://hz.316326.xyz/gtmclsqrfe.html

[U44] PHP：开启严格类型
来源：http://hz.guowangkeji.top/gtoowdwdbo.html

declare(strict_types=1);
来源：http://hz.xylfe.cn/gtdwjondfo.html

[U45] PHP：类型声明与返回类型
来源：http://hz.cheryme.top/gtvmxhgzgt.html

function add(int $a, int $b): int { return $a + $b; }
来源：http://hz.sxryk.cn/gtuqvuesdv.html

[U46] PHP：可空类型
来源：http://hz.xinyue.icu/gtvntpsory.html

?string $name = null
来源：http://hz.jqgfzy.top/gtohuacgkm.html

[U47] PHP：联合类型
来源：http://hz.yongpay.top/gtccmywydt.html

int|string $id
来源：http://hz.hongshengwenyu.top/gtokeddwht.html

[U48] PHP：纯枚举
来源：http://hz.yonumen.top/gtqodzlmbq.html

enum Status: string { case Active = "active"; case Off = "off"; }
来源：http://hz.nanxinkj.top/gtpqegnosc.html


<!-- 参考信息 -->