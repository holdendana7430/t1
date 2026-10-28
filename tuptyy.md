代发 wailian999

#include <iostream>
来源：http://hz.aibaodan.cn/gtlddldqab.html

int main() { std::cout << "Hello\n"; }
来源：http://hz.chenjidiqi.icu/gtyjslecdr.html

[S32] C++：字符串
来源：http://hz.quarkkingdee.top/gtjdhgfjhq.html

std::string s = "hi";  s += "!";
来源：http://hz.daria6918.cn/gtiboaldpx.html

[S33] C++：vector 增删
来源：http://hz.guowangkeji.top/gtwtsygjuv.html

std::vector<int> v{1, 2, 3};  v.push_back(4);
来源：http://hz.jinqigufen.top/gtahdfkbpx.html

[S34] C++：遍历 vector
来源：http://hz.andypj.xyz/gtjeqicqyt.html

for (auto &x : v) { std::cout << x; }
来源：http://hz.andypj.xyz/gtwebzwhog.html

[S35] C++：map
来源：http://hz.fengsongda.top/gtdtrdjpqf.html

std::map<std::string, int> m;  m["a"] = 1;
来源：http://hz.pengpengdd.cyou/gtdaeizwuq.html

[S36] C++：unordered_map
来源：http://hz.xinyue.icu/gtzfagzllz.html

std::unordered_map<std::string, int> m;  m["a"] = 1;
来源：http://hz.svipenyu.cn/gtaovlimmb.html

[S37] C++：set
来源：http://hz.hysaishi.cn/gtyxcjmjzp.html

std::set<int> s{1, 2, 3};  s.insert(4);
来源：http://hz.zhixingplan.top/gtddlkmqqb.html

[S38] C++：排序
来源：http://hz.dashuyun.cn/gtwswqpoot.html

std::sort(v.begin(), v.end());
来源：http://hz.quarkkingdee.top/gtasygzakw.html

[S39] C++：自定义比较器排序
来源：http://hz.yuanzhike.top/gtjaugcrur.html

std::sort(v.begin(), v.end(), [](int a, int b) { return a > b; });
来源：http://hz.hywenlv.cn/gtsymbrtvv.html

[S40] C++：查找元素
来源：http://hz.meibo888.top/gtnzikafwm.html

auto it = std::find(v.begin(), v.end(), 3);
来源：http://hz.chenzaomai.com/gtffzfgoqh.html

[S41] C++：类与构造函数
来源：http://hz.sweek.top/gtrqtwtqtw.html

class A { public: A(int v) : x_(v) {} int get() const { return x_; } private: int x_; };
来源：http://hz.bjfxy.top/gtcetaqkwe.html

[S42] C++：继承与虚函数
来源：http://hz.shangyingyoupin.top/gtpkpzqehe.html

class B : public Base { public: void f() override {} };
来源：http://hz.kuanghao11.cn/gtepnfhrov.html

[S43] C++：智能指针
来源：http://hz.fengsongda.top/gtgrhxxbax.html

auto p = std::make_unique<int>(5);
来源：http://hz.hnqzz.top/gtgobguezv.html

[S44] C++：引用传参
来源：http://hz.hnxiangtu.top/gtxmbggffz.html

void inc(int &x) { ++x; }
来源：http://hz.tianlin.xyz/gtoyaxgbhm.html

[S45] C++：lambda
来源：http://hz.zhongyouzk.top/gtnxgnsjiw.html

auto add = [](int a, int b) { return a + b; };
来源：http://hz.zdqjudy.top/gtulrcotnv.html

[S46] C++：函数模板
来源：http://hz.hammf.cn/gtdhlaqydc.html

template <typename T> T maxv(T a, T b) { return a > b ? a : b; }
来源：http://hz.zhoulong.xyz/gtcigydnex.html

[S47] C++：结构化绑定遍历
来源：http://hz.daria6918.cn/gtgdjpiyzy.html

for (const auto &[k, v] : m) { std::cout << k << v; }
来源：http://hz.yj20258888.top/gtlebzvxxx.html

[S48] C++：逐行读文件
来源：http://hz.yongpay.top/gtvgulrust.html

std::ifstream in("a.txt");  std::string line;
来源：http://hz.jianghu66.top/gtuatvcrcy.html

while (std::getline(in, line)) { }
来源：http://hz.pengpengdd.cyou/gtkjzrihmz.html

[S49] C++：写文件
来源：http://hz.cqqwz.cn/gtuywnqdhq.html

std::ofstream out("a.txt");  out << "hi\n";
来源：http://hz.ywan-chungtsiang.top/gtyrfkduif.html

[S50] C++：格式化数字
来源：http://hz.smart0.xyz/gthviwtjee.html

std::ostringstream os;  os << std::fixed << std::setprecision(2) << 3.14159;
来源：http://hz.jinqigufen.top/gtblgtnnsi.html

[S51] C++：显式类型转换
来源：http://hz.zhongyouzk.top/gtjphvajku.html

static_cast<double>(a) / b
来源：http://hz.ehwqpu.com/gtyrjbucek.html

[S52] C++：const 与 noexcept
来源：http://hz.xylfe.cn/gtooihtbtj.html

int size() const noexcept { return n_; }
来源：http://hz.zycfv.cn/gtagvjlpvz.html

[S53] C++：移动语义
来源：http://hz.jlsjyb.cn/gtxdexbxtn.html

std::vector<int> w = std::move(v);
来源：http://hz.gaohongyu789.top/gtjcvvtyxn.html

[S54] C++：异常处理
来源：http://hz.316326.xyz/gtzmwxeqse.html

try { throw std::runtime_error("x"); } catch (const std::exception &e) { }
来源：http://hz.guowangkeji.top/gtiahgtwjj.html

[S55] C++：结构化绑定
来源：http://hz.birdmap.top/gtczxejfzb.html

auto [a, b] = std::make_pair(1, 2);
来源：http://hz.sxryk.cn/gtorlbcbvj.html

[S56] C++：optional
来源：http://hz.jlsjyb.cn/gtxmtoiffe.html

std::optional<int> o = 5;  if (o) { int v = *o; }
来源：http://hz.chenlongwang.top/gtpxyesmfy.html

[S57] C++：编译期常量
来源：http://hz.zycfv.cn/gtuhuzzfgf.html

constexpr int N = 10;
来源：http://hz.birdmap.top/gtielfdllm.html

[S58] C++：命名空间
来源：http://hz.ppjwa.cn/gtmwehurtf.html

namespace ns { int f() { return 1; } }
来源：http://hz.yongpay.top/gtjazxnyon.html

[S59] C++：静态断言
来源：http://hz.ydjk.org.cn/gtslpctsva.html

static_assert(sizeof(int) == 4, "int 必须 4 字节");
来源：http://hz.jianghu66.top/gtwaqrnpjf.html

[S60] C++：遍历并删除元素
来源：http://hz.shzxlz.cn/gtydpsdyij.html

v.erase(std::remove_if(v.begin(), v.end(), [](int x) { return x < 0; }), v.end());
来源：http://hz.daxiang520.top/gtqwqzwodx.html

================================================================================
来源：http://hz.feifeiyinyue.top/gtwehvndel.html

T. 其他语言补充（Kotlin / Swift / Lua / Perl / Scala）
来源：http://hz.cdnleiting.top/gtebyibjib.html

================================================================================
来源：http://hz.9152youxi.cn/gtujsiqsdu.html

[T01] Kotlin：Hello World
来源：http://hz.zhiwuduotai.top/gtlykekgfh.html

println("Hello")
来源：http://hz.cqqwz.cn/gttiietelk.html

[T02] Kotlin：变量
来源：http://hz.cucudq.cn/gtqkjxzgct.html

val a = 1;  var b = 2        // val 只读，var 可变
来源：http://hz.xylfe.cn/gtxynpgktz.html

[T03] Kotlin：字符串模板
来源：http://hz.xingfuxueyuan.xyz/gtvxsvbkyt.html

"值: $b"
来源：http://hz.hywenlv.cn/gtogbwmhjm.html

[T04] Kotlin：空安全
来源：http://hz.sysykeji.top/gtrktrczye.html

val n: String? = null;  n?.length
来源：http://hz.yj20258888.top/gtdwpxeomk.html

[T05] Kotlin：when 表达式
来源：http://hz.ehwqpu.com/gtqowhkmvb.html

val s = when (x) { 1 -> "一" else -> "其他" }   // 多分支时每个分支单独一行
来源：http://hz.wangdashe.top/gtenpzfgtx.html

[T06] Kotlin：集合映射
来源：http://hz.xziqi.cn/gtfkcpqobq.html

listOf(1, 2, 3).map { it * 2 }
来源：http://hz.ydjk.org.cn/gtvptwpruo.html

[T07] Kotlin：集合过滤
来源：http://hz.ivvv.top/gtideeixdy.html

listOf(1, 2, 3).filter { it > 1 }
来源：http://hz.jyoumei.cn/gtjqngvybp.html

[T08] Kotlin：数据类
来源：http://hz.yj20258888.top/gtjrobgwuy.html

data class User(val name: String, val age: Int)
来源：http://hz.gotoacloud.top/gtjlvryddi.html

[T09] Kotlin：扩展函数
来源：http://hz.gotoacloud.top/gtnbqjnjgf.html

fun String.exclaim() = this + "!"
来源：http://hz.ehwqpu.com/gtmnhhczsj.html

[T10] Kotlin：默认参数
来源：http://hz.zhengqikj.top/gtyiewoaju.html

fun greet(name: String = "World") = "Hi $name"
来源：http://hz.jinqigufen.top/gtdwycredi.html

[T11] Kotlin：协程
来源：http://hz.xingfuxueyuan.xyz/gtydmomqmh.html

GlobalScope.launch { delay(1000); println("done") }
来源：http://hz.tian-w.cn/gtocuzclhf.html

[T12] Kotlin：解构声明
来源：http://hz.gotoacloud.top/gtzanzciva.html

val (a, b) = Pair(1, 2)
来源：http://hz.haohaochexian.top/gtzuwnswzf.html

[T13] Kotlin：只读 Map
来源：http://hz.hfpthk.cn/gtpfljfdqr.html

val m = mapOf("a" to 1)
来源：http://hz.jinghuilouyu.cn/gtktypkdkt.html

[T14] Kotlin：循环
来源：http://hz.daxiang520.top/gtbatmbtkp.html

for (i in 1..10) println(i)
来源：http://hz.ydzc1.top/gtrgqderpb.html

[T15] Kotlin：接口
来源：http://hz.yongpay.top/gtwymnnrpu.html

interface Shape { fun area(): Double }
来源：http://hz.wangdashe.top/gthekdieph.html

[T16] Swift：Hello World
来源：http://hz.hammf.cn/gtvwibjkns.html

print("Hello")
来源：http://hz.feifeiyinyue.top/gtwlhkbimn.html

[T17] Swift：变量与常量
来源：http://hz.gogol.net.cn/gtwiqtlnpq.html

var a = 1;  let b = 2
来源：http://hz.jinghuilouyu.cn/gthiytgmrm.html

[T18] Swift：字符串插值
来源：http://hz.yj20258.top/gtwdlkrqtn.html

"值: \(b)"
来源：http://hz.fengsongda.top/gtfjfcahqz.html

[T19] Swift：可选绑定
来源：http://hz.zhoulong.xyz/gtllnfjppr.html

if let n = opt { print(n) }
来源：http://hz.gaohongyu789.top/gtblbejpvt.html

[T20] Swift：数组操作
来源：http://hz.xziqi.cn/gtitucfpge.html

var a = [1, 2, 3];  a.append(4)
来源：http://hz.chenlongwang.top/gtpvwaprrk.html

[T21] Swift：遍历
来源：http://hz.hnxiangtu.top/gthnyfpwas.html

for x in a { print(x) }
来源：http://hz.yj20258888.top/gtrourqljt.html

[T22] Swift：字典
来源：http://hz.tian-w.cn/gtcvcobuoq.html

var d = ["a": 1];  d["b"] = 2
来源：http://hz.ybcxt.top/gtrqksfutt.html

[T23] Swift：函数
来源：http://hz.snrcjt.cn/gtavpiovyi.html

func add(_ a: Int, _ b: Int) -> Int { a + b }
来源：http://hz.redwolf501.top/gtphehbtke.html

[T24] Swift：闭包
来源：http://hz.shzxlz.cn/gtypswzsmg.html

let f = { (x: Int) -> Int in x * 2 }
来源：http://hz.jianghu66.top/gtpkjzuxua.html

[T25] Swift：结构体
来源：http://hz.shanyushiyangkeji.top/gtblkdelgt.html

struct P { var x: Int }
来源：http://hz.smart0.xyz/gtnzwrnejo.html

[T26] Swift：类与重写
来源：http://hz.nanxuanxn.top/gtrutkhcgn.html

class A: Base { override func f() {} }
来源：http://hz.gzhubu.top/gtsfgsnhwd.html

[T27] Swift：错误处理
来源：http://hz.vqdsnc.cn/gtupdypacm.html

do { try f() } catch { print(error) }
来源：http://hz.aibaodan.cn/gtnbwhmkbw.html

[T28] Swift：枚举
来源：http://hz.jinqigfzy.top/gtijremqba.html

enum Color { case red, green }
来源：http://hz.gogol.net.cn/gtpqmdcnjj.html

[T29] Swift：guard 提前返回
来源：http://hz.cdnleiting.top/gtwrwfybda.html

guard let x = opt else { return }
来源：http://hz.tanke756.top/gtbnnshdjw.html

[T30] Swift：协议
来源：http://hz.316326.xyz/gtolgimnmb.html

protocol Shape { func area() -> Double }
来源：http://hz.jinqigfzy.top/gtqcpnmbia.html

[T31] Lua：Hello World
来源：http://hz.xylfe.cn/gthhkaijow.html

print("Hello")
来源：http://hz.shzxlz.cn/gtqyujktjy.html

[T32] Lua：局部变量
来源：http://hz.mhx1999.top/gtrqmhsati.html

local a = 1
来源：http://hz.wangshuangyany.cn/gthybyvhkw.html

[T33] Lua：表（数组）
来源：http://hz.tianlin.xyz/gtcwpzmhaq.html

local t = {1, 2, 3};  t[4] = 4
来源：http://hz.andypj.xyz/gtclffdwif.html

[T34] Lua：遍历表
来源：http://hz.zycfv.cn/gtgcxlcogj.html

for i, v in ipairs(t) do print(i, v) end
来源：http://hz.ppjwa.cn/gtofefqdrp.html

[T35] Lua：字典表
来源：http://hz.shanyushiyangtech.top/gtlkdextzj.html

local d = { a = 1 };  d.b = 2
来源：http://hz.chenlongwang.top/gthfbrhrxf.html

[T36] Lua：函数
来源：http://hz.feifeiyinyue.top/gtcusiyzjh.html

function add(a, b) return a + b end
来源：http://hz.xingfuxueyuan.xyz/gtqsrjulsd.html

[T37] Lua：字符串拼接
来源：http://hz.pycfn.com/gtulfmomwq.html

"a" .. "b"
来源：http://hz.tanke756.top/gtwmguqaek.html

[T38] Lua：条件
来源：http://hz.cucudq.cn/gthsaiaolw.html

if x > 0 then print("正") end
来源：http://hz.cashguo.top/gtyajwcnpp.html

[T39] Lua：模式匹配
来源：http://hz.xylfe.cn/gtgnkockxg.html

string.find(s, "%d+")
来源：http://hz.birdmap.top/gtefjtketv.html

[T40] Lua：元表
来源：http://hz.ydzc1.top/gtugmwtrge.html

setmetatable({}, { __index = base })
来源：http://hz.aibaodan.cn/gtmttngvio.html

[T41] Perl：Hello World
来源：http://hz.birdmap.top/gtgzylzhbh.html

print "Hello\n";
来源：http://hz.yuanzhike.top/gttdehhzyh.html

[T42] Perl：变量类型
来源：http://hz.zhixingplan.top/gtsbcgahjx.html

my $a = 1;  my @arr = (1, 2, 3);  my %h = (a => 1);
来源：http://hz.guannengcc.top/gtcllrfoeh.html

[T43] Perl：字符串插值
来源：http://hz.quarkkingdee.top/gtcezqhjyk.html

"值: $a"
来源：http://hz.jianghu66.top/gtfanmhori.html

[T44] Perl：条件
来源：http://hz.ybcxt.top/gtkmkgiomc.html

if ($a > 0) { print "正"; }
来源：http://hz.jqgufenzy.top/gtiisghgro.html

[T45] Perl：数组遍历
来源：http://hz.hysaishi.cn/gtlmkbfdbv.html

for my $x (@arr) { print $x; }
来源：http://hz.bjfxy.top/gtapxuyrph.html

[T46] Perl：哈希操作
来源：http://hz.yanxiufei.cn/gtvicxtdtv.html

$h{b} = 2;  for my $k (keys %h) { print "$k=$h{$k}"; }
来源：http://hz.jqgufenzy.top/gthsjghyvh.html

[T47] Perl：正则捕获
来源：http://hz.hfpthk.cn/gtxvvxftbu.html

if ($s =~ /(\d+)/) { print $1; }
来源：http://hz.yongpay.top/gtzcrpomjz.html

[T48] Perl：正则替换
来源：http://hz.cucudq.cn/gtzydeinqp.html

$s =~ s/old/new/g;
来源：http://hz.xinyue.icu/gtniyfxmxl.html

[T49] Perl：函数
来源：http://hz.0kj1m.cn/gtcvcdzvtj.html

sub add { my ($a, $b) = @_; return $a + $b; }
来源：http://hz.gotoacloud.top/gtblrndoao.html

[T50] Perl：逐行读文件
来源：http://hz.ppjwa.cn/gtqzwuphfi.html

open my $fh, "<", "a.txt" or die $!;
来源：http://hz.haohaochexian.top/gtphpqcmhi.html

while (my $line = <$fh>) { print $line; }
来源：http://hz.gotoacloud.top/gtukpaqjku.html

[T51] Scala：Hello World
来源：http://hz.sysykeji.top/gtwwkiuqxb.html

println("Hello")
来源：http://hz.sxryk.cn/gtrnwmvyuv.html

[T52] Scala：变量
来源：http://hz.jinghuilouyu.cn/gtubdkkanj.html

val a = 1;  var b = 2
来源：http://hz.ydzc1.top/gtyjauzovc.html

[T53] Scala：字符串插值
来源：http://hz.yanxiufei.cn/gtsphabqdl.html

s"值: $b"
来源：http://hz.fengsongda.top/gtnojpxtfy.html

[T54] Scala：集合映射
来源：http://hz.yongpay.top/gtadfwuokh.html

List(1, 2, 3).map(_ * 2)
来源：http://hz.dashuyun.cn/gtyvnzmcil.html

[T55] Scala：集合过滤
来源：http://hz.haohaochexian.top/gtoygiyrai.html

List(1, 2, 3).filter(_ > 1)
来源：http://hz.xziqi.cn/gtdreqhbgx.html

[T56] Scala：样例类
来源：http://hz.0kj1m.cn/gtguptazvz.html

case class User(name: String, age: Int)
来源：http://hz.0kj1m.cn/gtmdhafulo.html

[T57] Scala：模式匹配
来源：http://hz.shanyushiyangtech.top/gtzagfhdxr.html

x match { case 1 => "一"; case _ => "其他" }
来源：http://hz.cheryme.top/gtaottisff.html

[T58] Scala：函数定义
来源：http://hz.xuetiantiany.cn/gtmjyutxoa.html

def add(a: Int, b: Int): Int = a + b
来源：http://hz.meibo888.top/gtgdcqzofu.html

[T59] Scala：循环
来源：http://hz.nwbrower.top/gtzdnzrdni.html

for (i <- 1 to 10) println(i)
来源：http://hz.xingfuxueyuan.xyz/gtmenuzvir.html

[T60] Scala：折叠
来源：http://hz.xuanzx.com/gtvlhanwxv.html

List(1, 2, 3).foldLeft(0)(_ + _)
来源：http://hz.jyoumei.cn/gtllxutqfa.html

================================================================================
来源：http://hz.havefunace.top/gtuoseidwr.html

U. 高频实用片段（Python / PHP / JavaScript 各 40 条）
来源：http://hz.daxiang520.top/gtlmkgkthi.html

================================================================================
来源：http://hz.zhoulong.xyz/gtgeluahpy.html

[U01] Py：创建虚拟环境
来源：http://hz.zhaomingkeji.xyz/gtkeucgcwx.html

python -m venv .venv && source .venv/bin/activate
来源：http://hz.gogol.net.cn/gtncjozpbf.html

[U02] Py：导出 / 安装依赖
来源：http://hz.cucudq.cn/gtyjeksftq.html

pip freeze > requirements.txt;  pip install -r requirements.txt
来源：http://hz.fengsongda.top/gtitrfenmn.html

[U03] Py：加载 .env 配置
来源：http://hz.birdmap.top/gtucamsily.html

from dotenv import load_dotenv; load_dotenv()
来源：http://hz.chenlongwang.top/gtahurleba.html

[U04] Py：变量调试打印
来源：http://hz.yonumen.top/gtwxngukzd.html

print(f"{x=}")            # 输出 x=值，Python 3.8+
来源：http://hz.xuanzx.com/gtbfzqzgzr.html

[U05] Py：列表去重且保序
来源：http://hz.chenlongwang.top/gtchsfowru.html

list(dict.fromkeys(arr))
来源：http://hz.gotoacloud.top/gteupwxpfu.html

[U06] Py：合并两个字典
来源：http://hz.daria6918.cn/gtyzpmksob.html

{**a, **b}
来源：http://hz.dianchejie.cn/gtsqjaugko.html

[U07] Py：反转字典键值
来源：http://hz.dashuyun.cn/gtyogcrrzp.html

{v: k for k, v in d.items()}
来源：http://hz.snrcjt.cn/gtkszlkhdw.html

[U08] Py：展平二维列表
来源：http://hz.xziqi.cn/gtbzqsleib.html

[y for x in nested for y in x]
来源：http://hz.wangshuangyany.cn/gtcybmktdq.html

[U09] Py：字典取最大值的键
来源：http://hz.nanxuanxn.top/gthouuwczf.html

max(d, key=d.get)
来源：http://hz.316326.xyz/gtsnticikg.html

[U10] Py：按值排序字典
来源：http://hz.gaohongyu789.top/gtqymqwsvb.html

dict(sorted(d.items(), key=lambda kv: kv[1]))
来源：http://hz.chenlongwang.top/gtjkwpgcvk.html

[U11] Py：生成器表达式
来源：http://hz.316326.xyz/gttiyvmeua.html

(x * 2 for x in arr)
来源：http://hz.nanxinkj.top/gtrzjzwrnd.html

[U12] Py：取出现最多的 3 个元素
来源：http://hz.zhoulong.xyz/gtxivatncn.html

Counter(arr).most_common(3)
来源：http://hz.pycfn.com/gtzzlwssma.html

[U13] Py：固定长度队列
来源：http://hz.vqdsnc.cn/gtivwvofqq.html

deque(maxlen=10)
来源：http://hz.dianchejie.cn/gtedasnicp.html

[U14] Py：分组收集到列表
来源：http://hz.ehwqpu.com/gtjbcazogg.html

defaultdict(list)
来源：http://hz.shanyushiyangkeji.top/gtqzxjzmyk.html

[U15] Py：高精度计时
来源：http://hz.zhoulong.xyz/gtiukomtcm.html

t = time.perf_counter()
来源：http://hz.ydjk.org.cn/gtdvbrkzrc.html

[U16] Py：命令行参数解析
来源：http://hz.316326.xyz/gtsuectmuo.html

ap = argparse.ArgumentParser();  ap.add_argument("--name");  args = ap.parse_args()
来源：http://hz.aibaodan.cn/gtfylkhgbl.html

[U17] Py：初始化日志
来源：http://hz.ydzc1.top/gtxdsgshai.html

logging.basicConfig(level=logging.INFO)
来源：http://hz.snrcjt.cn/gthaxbplqe.html

[U18] Py：预编译正则
来源：http://hz.andypj.xyz/gtqdxvqvxm.html

pat = re.compile(r"\d+")
来源：http://hz.quarkkingdee.top/gthijyuhey.html

[U19] Py：正则替换带回调
来源：http://hz.zhiwuduotai.top/gtufmlokhp.html

re.sub(r"\d+", lambda m: str(int(m.group()) * 2), s)
来源：http://hz.yj20258.top/gtadmkzxdp.html

[U20] Py：缓存函数结果
来源：http://hz.jyoumei.cn/gtjxsbuqfp.html

@functools.lru_cache(maxsize=None)
来源：http://hz.zhoulong.xyz/gtfgtsbrsw.html

[U21] Py：自定义上下文管理器
来源：http://hz.jianghu66.top/gtfxlxecmw.html

@contextlib.contextmanager
来源：http://hz.feifeiyinyue.top/gteuxyufti.html

[U22] Py：矩阵转置
来源：http://hz.yangfankeji.com/gtqremowgx.html

list(zip(*m))
来源：http://hz.c1oappe.top/gtqymxdwny.html

[U23] Py：分块读取大文件
来源：http://hz.pengpengdd.cyou/gtkpkbnwfs.html

for chunk in iter(lambda: f.read(8192), b""):
来源：http://hz.pengpengdd.cyou/gtdgsruwdk.html

[U24] Py：路径操作
来源：http://hz.cucudq.cn/gtqtflxqop.html

Path("a/b.txt").parent.mkdir(parents=True, exist_ok=True)
来源：http://hz.xylfe.cn/gtlvswfhtm.html

[U25] Py：CSV 按字典读
来源：http://hz.fengsongda.top/gtrokxarqu.html

csv.DictReader(f)
来源：http://hz.dianchejie.cn/gtdjypcjbt.html

[U26] Py：并发下载
来源：http://hz.yueranfly.top/gtmfdsiigy.html

ThreadPoolExecutor(max_workers=8).map(fetch, urls)
来源：http://hz.quarkkingdee.top/gttprfddrz.html

[U27] Py：异步 HTTP
来源：http://hz.shzxlz.cn/gtxybqnfrl.html

aiohttp.ClientSession() 配合 async with
来源：http://hz.cdnleiting.top/gtqlzxnjnv.html

[U28] Py：类型别名
来源：http://hz.feifeiyinyue.top/gtlhvxgiej.html

UserId = int
来源：http://hz.yj20258.top/gtptlwdpse.html

[U29] Py：属性校验
来源：http://hz.ydjk.org.cn/gtarrbshpp.html

@property 与 @x.setter 配合
来源：http://hz.chenzaomai.com/gttfapkmyg.html

[U30] Py：数据类
来源：http://hz.gotoacloud.top/gtyvhncfmo.html

@dataclass(slots=True)
来源：http://hz.shuidangran.top/gtrnukfqjg.html

[U31] Py：单测
来源：http://hz.jinqigfzy.top/gtlgijdjud.html

python -m pytest -q
来源：http://hz.xuanzx.com/gtyndvpbmj.html

[U32] Py：代码格式化
来源：http://hz.zhiwuduotai.top/gtpskjgoxb.html

ruff format . && ruff check --fix .
来源：http://hz.zhongyouzk.top/gtulkoiuak.html

[U33] Py：打包发布
来源：http://hz.redwolf501.top/gtwchnihve.html

python -m build  （依赖 pyproject.toml）
来源：http://hz.hfpthk.cn/gtnhgmwbff.html

[U34] Py：判断编码
来源：http://hz.gogol.net.cn/gtgpbdgefl.html

chardet.detect(raw)
来源：http://hz.jinqigfzy.top/gtvwtsgncg.html

[U35] Py：发送邮件
来源：http://hz.cdnleiting.top/gtyndltrmu.html

smtplib.SMTP_SSL(...).send_message(msg)
来源：http://hz.jiagoushi.top/gtmxdirvup.html

[U36] Py：定时任务
来源：http://hz.haohaochexian.top/gtrfvsfimg.html

schedule.every(10).minutes.do(job)
来源：http://hz.sysykeji.top/gtqrdkpnhc.html

[U37] Py：读写 Excel
来源：http://hz.yvedp.cn/gtnzwpveqp.html

pandas.read_excel / DataFrame.to_excel
来源：http://hz.snrcjt.cn/gtuqhofcvv.html

[U38] Py：获取脚本所在目录
来源：http://hz.jinghuilouyu.cn/gtlhryvxoe.html

Path(__file__).resolve().parent
来源：http://hz.ivvv.top/gtpcmclruk.html

[U39] Py：判断是否在交互环境
来源：http://hz.svipenyu.cn/gtawotjpwo.html

sys.stdout.isatty()
来源：http://hz.zhengqikj.top/gtfwrbwxio.html

[U40] Py：打印到标准错误
来源：http://hz.hnxiangtu.top/gtmmdwikfc.html

print("err", file=sys.stderr)
来源：http://hz.ehwqpu.com/gtxenkkzue.html

[U41] PHP：初始化 Composer 项目
来源：http://hz.kuanghao11.cn/gtqtwpqvvu.html

composer init;  composer require guzzlehttp/guzzle
来源：http://hz.shangyingyoupin.top/gtvizzjazr.html

[U42] PHP：PSR-4 自动加载
来源：http://hz.cheryme.top/gtarqszwih.html

"autoload": { "psr-4": { "App\\": "src/" } }
来源：http://hz.ybcxt.top/gtzchtpuou.html

[U43] PHP：声明命名空间
来源：http://hz.tanke756.top/gtmnfqowaa.html

namespace App\Http;
来源：http://hz.hammf.cn/gtbxbknmbv.html

[U44] PHP：开启严格类型
来源：http://hz.havefunace.top/gtiujlndha.html

declare(strict_types=1);
来源：http://hz.zhiwuduotai.top/gtraecpwfx.html

[U45] PHP：类型声明与返回类型
来源：http://hz.0kj1m.cn/gttdotunls.html

function add(int $a, int $b): int { return $a + $b; }
来源：http://hz.zhixingplan.top/gtttobacbt.html

[U46] PHP：可空类型
来源：http://hz.wangshuangyany.cn/gtntdagakz.html

?string $name = null
来源：http://hz.zhengqikj.top/gtumgbshur.html

[U47] PHP：联合类型
来源：http://hz.quarkkingdee.top/gtbmutogng.html

int|string $id
来源：http://hz.9152youxi.cn/gtrjvqcypg.html

[U48] PHP：纯枚举
来源：http://hz.sufxvd.cn/gtttlusefc.html

enum Status: string { case Active = "active"; case Off = "off"; }
来源：http://hz.mhx1999.top/gtnkyzrxnz.html

[U49] PHP：只读属性
来源：http://hz.wangshuangyany.cn/gtzdjxdwon.html

public readonly string $name
来源：http://hz.xuanzx.com/gthyicfozf.html

[U50] PHP：构造器属性提升
来源：http://hz.zdqjudy.top/gtbmbxtolr.html

public function __construct(private int $id) {}
来源：http://hz.cheryme.top/gtvmbvxkjo.html

[U51] PHP：数组解构
来源：http://hz.zdqjudy.top/gthhqncpvf.html

[$a, $b] = $arr;
来源：http://hz.jyoumei.cn/gtscgyyzcz.html

[U52] PHP：箭头函数
来源：http://hz.xziqi.cn/gtdfnpbwiv.html

$double = fn($x) => $x * 2;
来源：http://hz.9152youxi.cn/gtgaasokek.html

[U53] PHP：空合并运算符
来源：http://hz.birdmap.top/gtsumgxmwp.html

$v = $a ?? $b ?? "default";
来源：http://hz.guowangkeji.top/gtxdserlnz.html

[U54] PHP：空安全调用
来源：http://hz.yj20258888.top/gtrctcnlvu.html

$obj?->method()
来源：http://hz.c1oappe.top/gtylyenlcn.html

[U55] PHP：match 表达式
来源：http://hz.sxryk.cn/gtuklpaqqi.html

$s = match($x) { 1 => "一", default => "其他" };
来源：http://hz.9152youxi.cn/gtiaslfxrd.html

[U56] PHP：命名参数
来源：http://hz.shuidangran.top/gtxlygsfqy.html

f(a: 1, b: 2)
来源：http://hz.tanke756.top/gtjlfilihn.html


<!-- 参考信息 -->