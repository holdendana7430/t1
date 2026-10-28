代发 wailian999

bsearch(&key, a, n, sizeof(int), cmp);
来源：http://hz.gogol.net.cn/gtpnuhujak.html

[S21] C：字符类别判断
来源：http://hz.shanyushiyangkeji.top/gtwdsmobkd.html

isdigit(c);  isalpha(c);  isspace(c);
来源：http://hz.zhiwuduotai.top/gtlkjrefkp.html

[S22] C：字符串转数字
来源：http://hz.tian-w.cn/gtlcyawnae.html

atoi("42");  strtod("3.14", NULL);
来源：http://hz.xinyue.icu/gtxszxgfvo.html

[S23] C：随机数
来源：http://hz.jqgufenzy.top/gtmkefaeav.html

srand(time(NULL));  int r = rand() % 100;
来源：http://hz.haohaochexian.top/gtnvuzhiza.html

[S24] C：获取本地时间
来源：http://hz.ehwqpu.com/gtqgetwziv.html

time_t t = time(NULL);  struct tm *tm = localtime(&t);
来源：http://hz.quarkkingdee.top/gtrfnstqaq.html

[S25] C：内存拷贝
来源：http://hz.kuanghao11.cn/gtfypovjsv.html

memcpy(dst, src, n);
来源：http://hz.hysaishi.cn/gtggpztfuu.html

[S26] C：内存清零
来源：http://hz.cqqwz.cn/gtfxxkvcer.html

memset(a, 0, sizeof a);
来源：http://hz.zycfv.cn/gtrzjsjadb.html

[S27] C：定义常量
来源：http://hz.quarkkingdee.top/gtzdgscypd.html

const double PI = 3.14159;
来源：http://hz.jianghu66.top/gtfkobmvmj.html

[S28] C：静态变量
来源：http://hz.hfpthk.cn/gtuvkkyxfa.html

static int counter = 0;
来源：http://hz.tian-w.cn/gtjclmcwqs.html

[S29] C：变参函数
来源：http://hz.xingfuxueyuan.xyz/gtgxiyzcxf.html

va_list ap; va_start(ap, fmt); vprintf(fmt, ap); va_end(ap);
来源：http://hz.jinghuilouyu.cn/gtdmrjcqwc.html

[S30] C：头文件保护
来源：http://hz.jyoumei.cn/gtseahkpde.html

#ifndef X_H
来源：http://hz.wangshuangyany.cn/gtfybkemhz.html

#define X_H
来源：http://hz.quarkkingdee.top/gtaalbcouk.html

#endif
来源：http://hz.hfpthk.cn/gtcizgrimh.html

[S31] C++：Hello World
来源：http://hz.gotoacloud.top/gtvpcqbbri.html

#include <iostream>
来源：http://hz.shanyushiyangtech.top/gtchoxdiek.html

int main() { std::cout << "Hello\n"; }
来源：http://hz.fzhhl.top/gtizsksjpg.html

[S32] C++：字符串
来源：http://hz.gogol.net.cn/gtcgtjocve.html

std::string s = "hi";  s += "!";
来源：http://hz.zhaomingkeji.xyz/gtdamojwsn.html

[S33] C++：vector 增删
来源：http://hz.zhaomingkeji.xyz/gtahvrrqmt.html

std::vector<int> v{1, 2, 3};  v.push_back(4);
来源：http://hz.jinqigfzy.top/gtteedvgjy.html

[S34] C++：遍历 vector
来源：http://hz.iojbl.cn/gtcjepatts.html

for (auto &x : v) { std::cout << x; }
来源：http://hz.ydzc1.top/gtdofmwsvo.html

[S35] C++：map
来源：http://hz.9152youxi.cn/gtxjwhdvxp.html

std::map<std::string, int> m;  m["a"] = 1;
来源：http://hz.daxiang520.top/gtpxbaepwb.html

[S36] C++：unordered_map
来源：http://hz.tanke756.top/gtgvliinbt.html

std::unordered_map<std::string, int> m;  m["a"] = 1;
来源：http://hz.yonumen.top/gtzoqjksyv.html

[S37] C++：set
来源：http://hz.hammf.cn/gtepggrbkt.html

std::set<int> s{1, 2, 3};  s.insert(4);
来源：http://hz.zhongyouzk.top/gtivylotfh.html

[S38] C++：排序
来源：http://hz.shzxlz.cn/gtcfisyzpo.html

std::sort(v.begin(), v.end());
来源：http://hz.ydjk.org.cn/gthgzlcvzd.html

[S39] C++：自定义比较器排序
来源：http://hz.bjfxy.top/gtmsxvsgct.html

std::sort(v.begin(), v.end(), [](int a, int b) { return a > b; });
来源：http://hz.nwbrower.top/gtwrjdgsgf.html

[S40] C++：查找元素
来源：http://hz.zdqjudy.top/gtqbykicrk.html

auto it = std::find(v.begin(), v.end(), 3);
来源：http://hz.jinyuanbaomall.cn/gthvmtdbae.html

[S41] C++：类与构造函数
来源：http://hz.jqgfzy.top/gtzvzdidhq.html

class A { public: A(int v) : x_(v) {} int get() const { return x_; } private: int x_; };
来源：http://hz.gogol.net.cn/gtdukszmjn.html

[S42] C++：继承与虚函数
来源：http://hz.chenlongwang.top/gttbhxeitl.html

class B : public Base { public: void f() override {} };
来源：http://hz.xylfe.cn/gtqmorovze.html

[S43] C++：智能指针
来源：http://hz.shanyushiyangtech.top/gtptrnuwme.html

auto p = std::make_unique<int>(5);
来源：http://hz.zdqjudy.top/gtxrlexqdy.html

[S44] C++：引用传参
来源：http://hz.shangyingyoupin.top/gtpazkehku.html

void inc(int &x) { ++x; }
来源：http://hz.wangdashe.top/gtuzokdweo.html

[S45] C++：lambda
来源：http://hz.jlsjyb.cn/gtxzzhtouc.html

auto add = [](int a, int b) { return a + b; };
来源：http://hz.hywenlv.cn/gtayjladtf.html

[S46] C++：函数模板
来源：http://hz.cashguo.top/gtftvqboaw.html

template <typename T> T maxv(T a, T b) { return a > b ? a : b; }
来源：http://hz.yangfankeji.com/gtbspnwwlw.html

[S47] C++：结构化绑定遍历
来源：http://hz.dashuyun.cn/gtuddpqryi.html

for (const auto &[k, v] : m) { std::cout << k << v; }
来源：http://hz.shzxlz.cn/gtdmldehrz.html

[S48] C++：逐行读文件
来源：http://hz.hongshengwenyu.top/gtmrtiweug.html

std::ifstream in("a.txt");  std::string line;
来源：http://hz.shanyushiyangkeji.top/gtkxqztqlp.html

while (std::getline(in, line)) { }
来源：http://hz.ywan-chungtsiang.top/gtkdssziod.html

[S49] C++：写文件
来源：http://hz.svipenyu.cn/gtauwpsxsj.html

std::ofstream out("a.txt");  out << "hi\n";
来源：http://hz.hongshengwenyu.top/gtlvjpyoqx.html

[S50] C++：格式化数字
来源：http://hz.xziqi.cn/gtbphslatr.html

std::ostringstream os;  os << std::fixed << std::setprecision(2) << 3.14159;
来源：http://hz.dianchejie.cn/gttmgiqzmb.html

[S51] C++：显式类型转换
来源：http://hz.hysaishi.cn/gtcfrwvnop.html

static_cast<double>(a) / b
来源：http://hz.gogol.net.cn/gtldvhibep.html

[S52] C++：const 与 noexcept
来源：http://hz.tanke756.top/gtqzaduuyf.html

int size() const noexcept { return n_; }
来源：http://hz.yj20258.top/gtwyowplnv.html

[S53] C++：移动语义
来源：http://hz.hysaishi.cn/gtzhyazlqf.html

std::vector<int> w = std::move(v);
来源：http://hz.fzhhl.top/gthgfttlnh.html

[S54] C++：异常处理
来源：http://hz.xylfe.cn/gtxbdbgfgg.html

try { throw std::runtime_error("x"); } catch (const std::exception &e) { }
来源：http://hz.yanxiufei.cn/gtiqffalmw.html

[S55] C++：结构化绑定
来源：http://hz.ybcxt.top/gtfanjndhq.html

auto [a, b] = std::make_pair(1, 2);
来源：http://hz.guowangkeji.top/gtjopnnkuq.html

[S56] C++：optional
来源：http://hz.shangyingyoupin.top/gtdbrwfzqy.html

std::optional<int> o = 5;  if (o) { int v = *o; }
来源：http://hz.nanxinkj.top/gtevtbwhhl.html

[S57] C++：编译期常量
来源：http://hz.jinqigfzy.top/gtejrcialp.html

constexpr int N = 10;
来源：http://hz.yuxming.cn/gtuqhmxjjf.html

[S58] C++：命名空间
来源：http://hz.yuxming.cn/gtdrnqpgvc.html

namespace ns { int f() { return 1; } }
来源：http://hz.zhongyouzk.top/gtmndfoagw.html

[S59] C++：静态断言
来源：http://hz.ehwqpu.com/gtywbtwwim.html

static_assert(sizeof(int) == 4, "int 必须 4 字节");
来源：http://hz.chenlongwang.top/gtigsxades.html

[S60] C++：遍历并删除元素
来源：http://hz.xingfuxueyuan.xyz/gtvmyetbis.html

v.erase(std::remove_if(v.begin(), v.end(), [](int x) { return x < 0; }), v.end());
来源：http://hz.hywenlv.cn/gtribelksx.html

================================================================================
来源：http://hz.aibaodan.cn/gttxiyevlv.html

T. 其他语言补充（Kotlin / Swift / Lua / Perl / Scala）
来源：http://hz.jqgfzy.top/gtwegctdnb.html

================================================================================
来源：http://hz.hammf.cn/gttuxfhame.html

[T01] Kotlin：Hello World
来源：http://hz.chenjidiqi.icu/gtmihrfwqs.html

println("Hello")
来源：http://hz.0kj1m.cn/gtvuezkdnn.html

[T02] Kotlin：变量
来源：http://hz.yanxiufei.cn/gtijvsfkxa.html

val a = 1;  var b = 2        // val 只读，var 可变
来源：http://hz.aibaodan.cn/gtzfpmcwnt.html

[T03] Kotlin：字符串模板
来源：http://hz.dashuyun.cn/gtvmmjoypn.html

"值: $b"
来源：http://hz.sweek.top/gtutahvjhk.html

[T04] Kotlin：空安全
来源：http://hz.fengsongda.top/gtlolllrrp.html

val n: String? = null;  n?.length
来源：http://hz.zhaomingkeji.xyz/gtlapgqfga.html

[T05] Kotlin：when 表达式
来源：http://hz.jianghu66.top/gtbmgvwknv.html

val s = when (x) { 1 -> "一" else -> "其他" }   // 多分支时每个分支单独一行
来源：http://hz.yanxiufei.cn/gtumvnhpit.html

[T06] Kotlin：集合映射
来源：http://hz.dashuyun.cn/gtxedjkgzd.html

listOf(1, 2, 3).map { it * 2 }
来源：http://hz.yongpay.top/gtfknqukcx.html

[T07] Kotlin：集合过滤
来源：http://hz.hywenlv.cn/gtyphmhlua.html

listOf(1, 2, 3).filter { it > 1 }
来源：http://hz.shanyushiyangkeji.top/gtachgjnkf.html

[T08] Kotlin：数据类
来源：http://hz.hnxiangtu.top/gthmgawvdj.html

data class User(val name: String, val age: Int)
来源：http://hz.jinyuanbaomall.cn/gtyskyrupz.html

[T09] Kotlin：扩展函数
来源：http://hz.svipenyu.cn/gtlowdruvs.html

fun String.exclaim() = this + "!"
来源：http://hz.pycfn.com/gtdunkcocf.html

[T10] Kotlin：默认参数
来源：http://hz.pengpengdd.cyou/gtmbhobnxi.html

fun greet(name: String = "World") = "Hi $name"
来源：http://hz.redwolf501.top/gtnmdsqobe.html

[T11] Kotlin：协程
来源：http://hz.zhoulong.xyz/gtxbwqdngb.html

GlobalScope.launch { delay(1000); println("done") }
来源：http://hz.birdmap.top/gtxvgxztlo.html

[T12] Kotlin：解构声明
来源：http://hz.feifeiyinyue.top/gtvpzshfhb.html

val (a, b) = Pair(1, 2)
来源：http://hz.gaohongyu789.top/gtsbwvqiam.html

[T13] Kotlin：只读 Map
来源：http://hz.jyoumei.cn/gtjrfbcwyg.html

val m = mapOf("a" to 1)
来源：http://hz.gzhubu.top/gtcaepussp.html

[T14] Kotlin：循环
来源：http://hz.nanxuanxn.top/gtwanfytua.html

for (i in 1..10) println(i)
来源：http://hz.snrcjt.cn/gtkcyjkatu.html

[T15] Kotlin：接口
来源：http://hz.jianghu66.top/gtcsousxko.html

interface Shape { fun area(): Double }
来源：http://hz.ydjk.org.cn/gtyilhzqot.html

[T16] Swift：Hello World
来源：http://hz.guannengcc.top/gtddfapojo.html

print("Hello")
来源：http://hz.xinyue.icu/gthiltmpxl.html

[T17] Swift：变量与常量
来源：http://hz.hywenlv.cn/gtbwhpdxrg.html

var a = 1;  let b = 2
来源：http://hz.guowangkeji.top/gtuthxmnyr.html

[T18] Swift：字符串插值
来源：http://hz.ywan-chungtsiang.top/gtxfohitht.html

"值: \(b)"
来源：http://hz.pengpengdd.cyou/gtmxjhvwcj.html

[T19] Swift：可选绑定
来源：http://hz.zhoulong.xyz/gttvyfteeq.html

if let n = opt { print(n) }
来源：http://hz.hammf.cn/gtgmnmtfxm.html

[T20] Swift：数组操作
来源：http://hz.yanxiufei.cn/gtajqdfxzo.html

var a = [1, 2, 3];  a.append(4)
来源：http://hz.chenlongwang.top/gtbchxncqp.html

[T21] Swift：遍历
来源：http://hz.xingfuxueyuan.xyz/gtbhksrbkc.html

for x in a { print(x) }
来源：http://hz.0kj1m.cn/gtxzxpysbp.html

[T22] Swift：字典
来源：http://hz.kuanghao11.cn/gttwbtotux.html

var d = ["a": 1];  d["b"] = 2
来源：http://hz.cucudq.cn/gtuqardfgj.html

[T23] Swift：函数
来源：http://hz.aibaodan.cn/gtdvgvmvzj.html

func add(_ a: Int, _ b: Int) -> Int { a + b }
来源：http://hz.daria6918.cn/gtafzcsysa.html

[T24] Swift：闭包
来源：http://hz.yuxming.cn/gtgodzcmts.html

let f = { (x: Int) -> Int in x * 2 }
来源：http://hz.guowangkeji.top/gteounvpyk.html

[T25] Swift：结构体
来源：http://hz.ywan-chungtsiang.top/gtgspgzecq.html

struct P { var x: Int }
来源：http://hz.guannengcc.top/gtimwfxadk.html

[T26] Swift：类与重写
来源：http://hz.c1oappe.top/gttsiwnadp.html

class A: Base { override func f() {} }
来源：http://hz.hysaishi.cn/gtjqvkszeb.html

[T27] Swift：错误处理
来源：http://hz.cdnleiting.top/gtvpwnisru.html

do { try f() } catch { print(error) }
来源：http://hz.guannengcc.top/gtzgxttzsm.html

[T28] Swift：枚举
来源：http://hz.gaohongyu789.top/gtuysiqgqo.html

enum Color { case red, green }
来源：http://hz.cucudq.cn/gtnpdwjwwz.html

[T29] Swift：guard 提前返回
来源：http://hz.zhiwuduotai.top/gtpxwtmzjw.html

guard let x = opt else { return }
来源：http://hz.wangshuangyany.cn/gtbxavbwng.html

[T30] Swift：协议
来源：http://hz.xinyue.icu/gtdmpvxvgw.html

protocol Shape { func area() -> Double }
来源：http://hz.yvedp.cn/gtnpyyogpr.html

[T31] Lua：Hello World
来源：http://hz.cucudq.cn/gtktcgcrki.html

print("Hello")
来源：http://hz.kuanghao11.cn/gtaminefom.html

[T32] Lua：局部变量
来源：http://hz.tianlin.xyz/gtwtntbvnv.html

local a = 1
来源：http://hz.ivvv.top/gtkkldyask.html

[T33] Lua：表（数组）
来源：http://hz.hongshengwenyu.top/gtwzvfqxua.html

local t = {1, 2, 3};  t[4] = 4
来源：http://hz.zhongyouzk.top/gthjdgtalx.html

[T34] Lua：遍历表
来源：http://hz.nanxuanxn.top/gtddkztnev.html

for i, v in ipairs(t) do print(i, v) end
来源：http://hz.redwolf501.top/gtwyflowax.html

[T35] Lua：字典表
来源：http://hz.bjfxy.top/gtgigqygzu.html

local d = { a = 1 };  d.b = 2
来源：http://hz.shzxlz.cn/gtdeekpnhh.html

[T36] Lua：函数
来源：http://hz.hammf.cn/gtfygyrcdc.html

function add(a, b) return a + b end
来源：http://hz.hammf.cn/gtvithzwbb.html

[T37] Lua：字符串拼接
来源：http://hz.vqdsnc.cn/gtfdgurdgk.html

"a" .. "b"
来源：http://hz.mhx1999.top/gtvqsboovo.html

[T38] Lua：条件
来源：http://hz.zhongyouzk.top/gtywkbbqlf.html

if x > 0 then print("正") end
来源：http://hz.zycfv.cn/gtxtomkrtj.html

[T39] Lua：模式匹配
来源：http://hz.aibaodan.cn/gtvlnpnabg.html

string.find(s, "%d+")
来源：http://hz.zhixingplan.top/gtnadgcfjs.html

[T40] Lua：元表
来源：http://hz.zycfv.cn/gttpovwson.html

setmetatable({}, { __index = base })
来源：http://hz.aibaodan.cn/gttsammqbr.html

[T41] Perl：Hello World
来源：http://hz.shuidangran.top/gtsphkintn.html

print "Hello\n";
来源：http://hz.yonumen.top/gtoeqxrndy.html

[T42] Perl：变量类型
来源：http://hz.shanyushiyangtech.top/gtctxvtwcs.html

my $a = 1;  my @arr = (1, 2, 3);  my %h = (a => 1);
来源：http://hz.fengsongda.top/gtbxwmfcdc.html

[T43] Perl：字符串插值
来源：http://hz.cheryme.top/gtcbztbolh.html

"值: $a"
来源：http://hz.cucudq.cn/gtoihwqxia.html

[T44] Perl：条件
来源：http://hz.zycfv.cn/gtcglsnbvo.html

if ($a > 0) { print "正"; }
来源：http://hz.tanke756.top/gtbjozeesx.html

[T45] Perl：数组遍历
来源：http://hz.cdnleiting.top/gtgycjlicm.html

for my $x (@arr) { print $x; }
来源：http://hz.jinyuanbaomall.cn/gtzyjfrlqx.html

[T46] Perl：哈希操作
来源：http://hz.haohaochexian.top/gtubzntofc.html

$h{b} = 2;  for my $k (keys %h) { print "$k=$h{$k}"; }
来源：http://hz.zhijiandao.cn/gtzjcejrpp.html

[T47] Perl：正则捕获
来源：http://hz.0kj1m.cn/gtqazlmnjz.html

if ($s =~ /(\d+)/) { print $1; }
来源：http://hz.yueranfly.top/gtqtqnviis.html

[T48] Perl：正则替换
来源：http://hz.shanyushiyangtech.top/gtpzrouvvl.html

$s =~ s/old/new/g;
来源：http://hz.hnqzz.top/gtxwtvlipn.html

[T49] Perl：函数
来源：http://hz.cdnleiting.top/gtsfifyaky.html

sub add { my ($a, $b) = @_; return $a + $b; }
来源：http://hz.316326.xyz/gtmrsutnqf.html

[T50] Perl：逐行读文件
来源：http://hz.xuanzx.com/gttafmzcvr.html

open my $fh, "<", "a.txt" or die $!;
来源：http://hz.ehwqpu.com/gtvgaeojdv.html

while (my $line = <$fh>) { print $line; }
来源：http://hz.jiagoushi.top/gtgtdxvhvl.html

[T51] Scala：Hello World
来源：http://hz.sweek.top/gthyqxpqgi.html

println("Hello")
来源：http://hz.chenlongwang.top/gtnerymqyu.html

[T52] Scala：变量
来源：http://hz.zycfv.cn/gtlckpuoft.html

val a = 1;  var b = 2
来源：http://hz.havefunace.top/gtlqkvgtpy.html

[T53] Scala：字符串插值
来源：http://hz.0kj1m.cn/gtopetnokz.html

s"值: $b"
来源：http://hz.chenzaomai.com/gtralhaazs.html

[T54] Scala：集合映射
来源：http://hz.hammf.cn/gtpuydveji.html

List(1, 2, 3).map(_ * 2)
来源：http://hz.zhongyouzk.top/gtikizbepf.html

[T55] Scala：集合过滤
来源：http://hz.yuanzhike.top/gtxdxcsrxw.html

List(1, 2, 3).filter(_ > 1)
来源：http://hz.gzhubu.top/gtvhwdnqwk.html

[T56] Scala：样例类
来源：http://hz.zhijiandao.cn/gttkmgneoe.html

case class User(name: String, age: Int)
来源：http://hz.cqqwz.cn/gtockgwcxd.html

[T57] Scala：模式匹配
来源：http://hz.jqgfzy.top/gtdozbgdny.html

x match { case 1 => "一"; case _ => "其他" }
来源：http://hz.hongshengwenyu.top/gtcndamvvp.html

[T58] Scala：函数定义
来源：http://hz.chenlongwang.top/gtavasjayj.html

def add(a: Int, b: Int): Int = a + b
来源：http://hz.shuidangran.top/gtvqsfklml.html

[T59] Scala：循环
来源：http://hz.hongshengwenyu.top/gtctzmqvbq.html

for (i <- 1 to 10) println(i)
来源：http://hz.ywan-chungtsiang.top/gtxcfldvsd.html

[T60] Scala：折叠
来源：http://hz.shuidangran.top/gtqdyrtmzu.html

List(1, 2, 3).foldLeft(0)(_ + _)
来源：http://hz.chenjidiqi.icu/gtfxoelrkl.html

================================================================================
来源：http://hz.zhoulong.xyz/gtzbihzsaf.html

U. 高频实用片段（Python / PHP / JavaScript 各 40 条）
来源：http://hz.kuanghao11.cn/gtutggohla.html

================================================================================
来源：http://hz.sweek.top/gtufsutrxy.html

[U01] Py：创建虚拟环境
来源：http://hz.fzhhl.top/gtgkifvrhf.html

python -m venv .venv && source .venv/bin/activate
来源：http://hz.pycfn.com/gtycftujxl.html

[U02] Py：导出 / 安装依赖
来源：http://hz.wangdashe.top/gtmdnznnli.html

pip freeze > requirements.txt;  pip install -r requirements.txt
来源：http://hz.mhx1999.top/gtkelhhfmh.html

[U03] Py：加载 .env 配置
来源：http://hz.316326.xyz/gtbaflfgbb.html

from dotenv import load_dotenv; load_dotenv()
来源：http://hz.jinghuilouyu.cn/gtyjeucgdx.html

[U04] Py：变量调试打印
来源：http://hz.yongpay.top/gtpghtzvbg.html

print(f"{x=}")            # 输出 x=值，Python 3.8+
来源：http://hz.hfpthk.cn/gtkubgprti.html

[U05] Py：列表去重且保序
来源：http://hz.pengpengdd.cyou/gtfiycgkvo.html

list(dict.fromkeys(arr))
来源：http://hz.xuetiantiany.cn/gtzdtrryrd.html

[U06] Py：合并两个字典
来源：http://hz.sufxvd.cn/gtkkvefbmp.html

{**a, **b}
来源：http://hz.dashuyun.cn/gtvbfcwqjr.html

[U07] Py：反转字典键值
来源：http://hz.c1oappe.top/gtweqdzlba.html

{v: k for k, v in d.items()}
来源：http://hz.yj20258888.top/gtvatayzky.html

[U08] Py：展平二维列表
来源：http://hz.chenzaomai.com/gtkhuhwoqp.html

[y for x in nested for y in x]
来源：http://hz.xuanzx.com/gtnowplpbb.html

[U09] Py：字典取最大值的键
来源：http://hz.daxiang520.top/gtwxdfuyrq.html

max(d, key=d.get)
来源：http://hz.snrcjt.cn/gthncrhdop.html

[U10] Py：按值排序字典
来源：http://hz.cucudq.cn/gtzsdsafjw.html

dict(sorted(d.items(), key=lambda kv: kv[1]))
来源：http://hz.redwolf501.top/gtbfrpohos.html

[U11] Py：生成器表达式
来源：http://hz.hnqzz.top/gtjuldjcnn.html

(x * 2 for x in arr)
来源：http://hz.jqgfzy.top/gtncwykoqx.html

[U12] Py：取出现最多的 3 个元素
来源：http://hz.zhoulong.xyz/gtpkngnlbh.html

Counter(arr).most_common(3)
来源：http://hz.kuanghao11.cn/gtnmefeamq.html

[U13] Py：固定长度队列
来源：http://hz.yj20258888.top/gtgsueoziu.html

deque(maxlen=10)
来源：http://hz.jinqigufen.top/gtxnqmxuls.html

[U14] Py：分组收集到列表
来源：http://hz.jinqigfzy.top/gtexhdhlar.html

defaultdict(list)
来源：http://hz.yanxiufei.cn/gthanzeumr.html

[U15] Py：高精度计时
来源：http://hz.wangdashe.top/gtuvbercff.html

t = time.perf_counter()
来源：http://hz.wangdashe.top/gtfggohqzn.html

[U16] Py：命令行参数解析
来源：http://hz.nanxinkj.top/gttotyvcww.html

ap = argparse.ArgumentParser();  ap.add_argument("--name");  args = ap.parse_args()
来源：http://hz.smart0.xyz/gtwirdtrwu.html

[U17] Py：初始化日志
来源：http://hz.havefunace.top/gtoikqgqgm.html

logging.basicConfig(level=logging.INFO)
来源：http://hz.svipenyu.cn/gtyqsepqak.html

[U18] Py：预编译正则
来源：http://hz.zhengqikj.top/gthayaykbd.html

pat = re.compile(r"\d+")
来源：http://hz.quarkkingdee.top/gtkygbnzrw.html

[U19] Py：正则替换带回调
来源：http://hz.sysykeji.top/gtevulynsv.html

re.sub(r"\d+", lambda m: str(int(m.group()) * 2), s)
来源：http://hz.andypj.xyz/gtoiskczwc.html

[U20] Py：缓存函数结果
来源：http://hz.chenlongwang.top/gtvsekqeql.html

@functools.lru_cache(maxsize=None)
来源：http://hz.wangdashe.top/gtwcfbuevl.html

[U21] Py：自定义上下文管理器
来源：http://hz.gotoacloud.top/gtapnsvkdl.html

@contextlib.contextmanager
来源：http://hz.52xcode.cn/gtmservuog.html

[U22] Py：矩阵转置
来源：http://hz.smart0.xyz/gttwydddac.html

list(zip(*m))
来源：http://hz.jlsjyb.cn/gtuidttfwu.html

[U23] Py：分块读取大文件
来源：http://hz.iojbl.cn/gtdhygxoia.html

for chunk in iter(lambda: f.read(8192), b""):
来源：http://hz.wangdashe.top/gtieglouis.html

[U24] Py：路径操作
来源：http://hz.sysykeji.top/gtiyjulixi.html

Path("a/b.txt").parent.mkdir(parents=True, exist_ok=True)
来源：http://hz.chenlongwang.top/gtghdzhdxc.html

[U25] Py：CSV 按字典读
来源：http://hz.yangfankeji.com/gtjgyrtsbd.html

csv.DictReader(f)
来源：http://hz.smart0.xyz/gtgsghluat.html

[U26] Py：并发下载
来源：http://hz.hongshengwenyu.top/gtearzmqzb.html

ThreadPoolExecutor(max_workers=8).map(fetch, urls)
来源：http://hz.jqgfzy.top/gtsqtkiiif.html

[U27] Py：异步 HTTP
来源：http://hz.yvedp.cn/gtekazehgq.html

aiohttp.ClientSession() 配合 async with
来源：http://hz.tian-w.cn/gtwgasxqip.html

[U28] Py：类型别名
来源：http://hz.52xcode.cn/gtvqhpghya.html

UserId = int
来源：http://hz.tanke756.top/gttboymwyw.html

[U29] Py：属性校验
来源：http://hz.jlsjyb.cn/gtwndzbqbo.html

@property 与 @x.setter 配合
来源：http://hz.hongshengwenyu.top/gtnziecdfx.html

[U30] Py：数据类
来源：http://hz.aizwys.cn/gtqdlylits.html

@dataclass(slots=True)
来源：http://hz.tian-w.cn/gtfboemlfh.html

[U31] Py：单测
来源：http://hz.gotoacloud.top/gtikhyzakc.html

python -m pytest -q
来源：http://hz.birdmap.top/gtlcftlbdk.html

[U32] Py：代码格式化
来源：http://hz.meibo888.top/gtnlhlwyvw.html

ruff format . && ruff check --fix .
来源：http://hz.yongpay.top/gtkrzocbkh.html

[U33] Py：打包发布
来源：http://hz.dashuyun.cn/gtmqxsuoid.html

python -m build  （依赖 pyproject.toml）
来源：http://hz.ehwqpu.com/gtquwbrysh.html

[U34] Py：判断编码
来源：http://hz.hfpthk.cn/gtnnhnvrar.html

chardet.detect(raw)
来源：http://hz.shanyushiyangkeji.top/gttnjjgyex.html

[U35] Py：发送邮件
来源：http://hz.gzhubu.top/gtzhzmpjag.html

smtplib.SMTP_SSL(...).send_message(msg)
来源：http://hz.xuanzx.com/gtxgseveea.html

[U36] Py：定时任务
来源：http://hz.jlsjyb.cn/gtdskaeezk.html

schedule.every(10).minutes.do(job)
来源：http://hz.bjfxy.top/gtvtwcvqcc.html

[U37] Py：读写 Excel
来源：http://hz.nanxinkj.top/gtfyenlyma.html

pandas.read_excel / DataFrame.to_excel
来源：http://hz.ydzc1.top/gtvetchckn.html

[U38] Py：获取脚本所在目录
来源：http://hz.hfpthk.cn/gtrrmbkikp.html

Path(__file__).resolve().parent
来源：http://hz.zhoulong.xyz/gtivhkijbs.html

[U39] Py：判断是否在交互环境
来源：http://hz.birdmap.top/gtkltnxdih.html

sys.stdout.isatty()
来源：http://hz.aibaodan.cn/gtuyzwxtcj.html

[U40] Py：打印到标准错误
来源：http://hz.zhijiandao.cn/gtumoammei.html

print("err", file=sys.stderr)
来源：http://hz.chenzaomai.com/gtlticicjj.html

[U41] PHP：初始化 Composer 项目
来源：http://hz.mhx1999.top/gtqpciozlu.html

composer init;  composer require guzzlehttp/guzzle
来源：http://hz.chenzaomai.com/gtskadaelc.html

[U42] PHP：PSR-4 自动加载
来源：http://hz.andypj.xyz/gttwvotrxj.html

"autoload": { "psr-4": { "App\\": "src/" } }
来源：http://hz.52xcode.cn/gtucjpbkor.html

[U43] PHP：声明命名空间
来源：http://hz.nanxinkj.top/gtollfhybu.html

namespace App\Http;
来源：http://hz.svipenyu.cn/gtjuibdujt.html

[U44] PHP：开启严格类型
来源：http://hz.zhongyouzk.top/gtyupyatfd.html

declare(strict_types=1);
来源：http://hz.shzxlz.cn/gtufgrtzwq.html


<!-- 参考信息 -->