代发 wailian999

bsearch(&key, a, n, sizeof(int), cmp);
来源：http://hz.daria6918.cn/gteazoflfl.html

[S21] C：字符类别判断
来源：http://hz.aizwys.cn/gtiqdksymh.html

isdigit(c);  isalpha(c);  isspace(c);
来源：http://hz.tianlin.xyz/gtczjhpamq.html

[S22] C：字符串转数字
来源：http://hz.ppjwa.cn/gtgconzxvz.html

atoi("42");  strtod("3.14", NULL);
来源：http://hz.52xcode.cn/gtnypgntib.html

[S23] C：随机数
来源：http://hz.yueranfly.top/gtjznupeum.html

srand(time(NULL));  int r = rand() % 100;
来源：http://hz.zhixingplan.top/gtsyntwybu.html

[S24] C：获取本地时间
来源：http://hz.xuetiantiany.cn/gtehiumyyf.html

time_t t = time(NULL);  struct tm *tm = localtime(&t);
来源：http://hz.ybcxt.top/gtmtkmjwbq.html

[S25] C：内存拷贝
来源：http://hz.pengpengdd.cyou/gtrndwvasd.html

memcpy(dst, src, n);
来源：http://hz.zhaomingkeji.xyz/gtslmkderq.html

[S26] C：内存清零
来源：http://hz.mhx1999.top/gtfwxlsshc.html

memset(a, 0, sizeof a);
来源：http://hz.dashuyun.cn/gtftxnvogd.html

[S27] C：定义常量
来源：http://hz.hysaishi.cn/gtbzkzoele.html

const double PI = 3.14159;
来源：http://hz.ivvv.top/gteakqbnoy.html

[S28] C：静态变量
来源：http://hz.svipenyu.cn/gtirejuxap.html

static int counter = 0;
来源：http://hz.jqgufenzy.top/gtrnfamwfn.html

[S29] C：变参函数
来源：http://hz.fengsongda.top/gtulfopinc.html

va_list ap; va_start(ap, fmt); vprintf(fmt, ap); va_end(ap);
来源：http://hz.xuetiantiany.cn/gtwikufswa.html

[S30] C：头文件保护
来源：http://hz.nwbrower.top/gthhbwerfh.html

#ifndef X_H
来源：http://hz.svipenyu.cn/gtogypcczw.html

#define X_H
来源：http://hz.smart0.xyz/gtsmkirovm.html

#endif
来源：http://hz.tanke756.top/gthxoulvqd.html

[S31] C++：Hello World
来源：http://hz.zhengqikj.top/gtneklghyr.html

#include <iostream>
来源：http://hz.shzxlz.cn/gtobajcujw.html

int main() { std::cout << "Hello\n"; }
来源：http://hz.yonumen.top/gtzunjaihk.html

[S32] C++：字符串
来源：http://hz.0kj1m.cn/gtthdsbunw.html

std::string s = "hi";  s += "!";
来源：http://hz.xziqi.cn/gtpqjcbeke.html

[S33] C++：vector 增删
来源：http://hz.aibaodan.cn/gtfdvqdmdu.html

std::vector<int> v{1, 2, 3};  v.push_back(4);
来源：http://hz.316326.xyz/gtwdjxxulw.html

[S34] C++：遍历 vector
来源：http://hz.guannengcc.top/gtotijtwza.html

for (auto &x : v) { std::cout << x; }
来源：http://hz.hnqzz.top/gtrjsimkpv.html

[S35] C++：map
来源：http://hz.ehwqpu.com/gthidydfhz.html

std::map<std::string, int> m;  m["a"] = 1;
来源：http://hz.jianghu66.top/gtmwhidwzj.html

[S36] C++：unordered_map
来源：http://hz.yonumen.top/gtjxxohmfu.html

std::unordered_map<std::string, int> m;  m["a"] = 1;
来源：http://hz.haohaochexian.top/gthsoiacvj.html

[S37] C++：set
来源：http://hz.daria6918.cn/gtxcvcaadn.html

std::set<int> s{1, 2, 3};  s.insert(4);
来源：http://hz.jianghu66.top/gtdcnyrsgs.html

[S38] C++：排序
来源：http://hz.ybcxt.top/gtgaberaqd.html

std::sort(v.begin(), v.end());
来源：http://hz.zhoulong.xyz/gtzjjteyzg.html

[S39] C++：自定义比较器排序
来源：http://hz.jinghuilouyu.cn/gtcpgnvsmm.html

std::sort(v.begin(), v.end(), [](int a, int b) { return a > b; });
来源：http://hz.cdnleiting.top/gtflaxjlhg.html

[S40] C++：查找元素
来源：http://hz.shangyingyoupin.top/gtwqxcldaf.html

auto it = std::find(v.begin(), v.end(), 3);
来源：http://hz.ppjwa.cn/gtfrwdqkxg.html

[S41] C++：类与构造函数
来源：http://hz.zhaomingkeji.xyz/gtpnrcazag.html

class A { public: A(int v) : x_(v) {} int get() const { return x_; } private: int x_; };
来源：http://hz.iojbl.cn/gttjldvukk.html

[S42] C++：继承与虚函数
来源：http://hz.jqgfzy.top/gtppejiilz.html

class B : public Base { public: void f() override {} };
来源：http://hz.sufxvd.cn/gtjqyqklzj.html

[S43] C++：智能指针
来源：http://hz.jinqigfzy.top/gtcmgjepms.html

auto p = std::make_unique<int>(5);
来源：http://hz.daria6918.cn/gtyhxyonmj.html

[S44] C++：引用传参
来源：http://hz.gogol.net.cn/gtfhqhnygc.html

void inc(int &x) { ++x; }
来源：http://hz.hnxiangtu.top/gtutxnvktt.html

[S45] C++：lambda
来源：http://hz.jinqigfzy.top/gtobbljeyw.html

auto add = [](int a, int b) { return a + b; };
来源：http://hz.birdmap.top/gtnkayapie.html

[S46] C++：函数模板
来源：http://hz.xuetiantiany.cn/gtovtwbepi.html

template <typename T> T maxv(T a, T b) { return a > b ? a : b; }
来源：http://hz.hnqzz.top/gtvippjovh.html

[S47] C++：结构化绑定遍历
来源：http://hz.ybcxt.top/gtaljvxfef.html

for (const auto &[k, v] : m) { std::cout << k << v; }
来源：http://hz.gotoacloud.top/gtfqwcpqmr.html

[S48] C++：逐行读文件
来源：http://hz.sufxvd.cn/gtzfrqyvkl.html

std::ifstream in("a.txt");  std::string line;
来源：http://hz.yuanzhike.top/gtjqhzzayj.html

while (std::getline(in, line)) { }
来源：http://hz.yonumen.top/gtpgpvozoe.html

[S49] C++：写文件
来源：http://hz.ywan-chungtsiang.top/gtlgxacyji.html

std::ofstream out("a.txt");  out << "hi\n";
来源：http://hz.yueranfly.top/gtsdsuysuy.html

[S50] C++：格式化数字
来源：http://hz.sysykeji.top/gthbipgxwp.html

std::ostringstream os;  os << std::fixed << std::setprecision(2) << 3.14159;
来源：http://hz.mhx1999.top/gtzfznleek.html

[S51] C++：显式类型转换
来源：http://hz.daria6918.cn/gtxcgjkwcg.html

static_cast<double>(a) / b
来源：http://hz.chenjidiqi.icu/gtnfjbicph.html

[S52] C++：const 与 noexcept
来源：http://hz.quarkkingdee.top/gttzozmrea.html

int size() const noexcept { return n_; }
来源：http://hz.tian-w.cn/gtlxhuvilt.html

[S53] C++：移动语义
来源：http://hz.redwolf501.top/gtlspwtubi.html

std::vector<int> w = std::move(v);
来源：http://hz.feifeiyinyue.top/gtpytaycbs.html

[S54] C++：异常处理
来源：http://hz.chenzaomai.com/gtjqmnnppg.html

try { throw std::runtime_error("x"); } catch (const std::exception &e) { }
来源：http://hz.jinyuanbaomall.cn/gtvafzjtbr.html

[S55] C++：结构化绑定
来源：http://hz.jinqigfzy.top/gtbamsggfo.html

auto [a, b] = std::make_pair(1, 2);
来源：http://hz.yuxming.cn/gtyxyctgvt.html

[S56] C++：optional
来源：http://hz.52xcode.cn/gtbarhsgnz.html

std::optional<int> o = 5;  if (o) { int v = *o; }
来源：http://hz.haohaochexian.top/gtoahwfuzd.html

[S57] C++：编译期常量
来源：http://hz.ywan-chungtsiang.top/gtnvlqbroy.html

constexpr int N = 10;
来源：http://hz.yangfankeji.com/gtjvpxmlfa.html

[S58] C++：命名空间
来源：http://hz.pengpengdd.cyou/gtttzpdrqc.html

namespace ns { int f() { return 1; } }
来源：http://hz.fzhhl.top/gtcklqqwtx.html

[S59] C++：静态断言
来源：http://hz.haohaochexian.top/gtzypxleke.html

static_assert(sizeof(int) == 4, "int 必须 4 字节");
来源：http://hz.ivvv.top/gtnqaeblsf.html

[S60] C++：遍历并删除元素
来源：http://hz.jinyuanbaomall.cn/gtszkordlb.html

v.erase(std::remove_if(v.begin(), v.end(), [](int x) { return x < 0; }), v.end());
来源：http://hz.jinqigfzy.top/gtozhsruse.html

================================================================================
来源：http://hz.guowangkeji.top/gtotlrwbwu.html

T. 其他语言补充（Kotlin / Swift / Lua / Perl / Scala）
来源：http://hz.zycfv.cn/gtpglfzfeg.html

================================================================================
来源：http://hz.ywan-chungtsiang.top/gtqxbcximz.html

[T01] Kotlin：Hello World
来源：http://hz.tianlin.xyz/gtwokfopvj.html

println("Hello")
来源：http://hz.gzhubu.top/gtmpzufabw.html

[T02] Kotlin：变量
来源：http://hz.jiagoushi.top/gtzvbkhgrw.html

val a = 1;  var b = 2        // val 只读，var 可变
来源：http://hz.shzxlz.cn/gtjmuewtau.html

[T03] Kotlin：字符串模板
来源：http://hz.aibaodan.cn/gtzkojjzsl.html

"值: $b"
来源：http://hz.yueranfly.top/gtzbeosolw.html

[T04] Kotlin：空安全
来源：http://hz.hfpthk.cn/gtbgodjvlj.html

val n: String? = null;  n?.length
来源：http://hz.jinqigufen.top/gtxrkofhog.html

[T05] Kotlin：when 表达式
来源：http://hz.jinghuilouyu.cn/gtoezfemrz.html

val s = when (x) { 1 -> "一" else -> "其他" }   // 多分支时每个分支单独一行
来源：http://hz.9152youxi.cn/gtldwakmhh.html

[T06] Kotlin：集合映射
来源：http://hz.feifeiyinyue.top/gtvzovlrox.html

listOf(1, 2, 3).map { it * 2 }
来源：http://hz.yanxiufei.cn/gtwwtyeawu.html

[T07] Kotlin：集合过滤
来源：http://hz.cheryme.top/gtxbfgsshp.html

listOf(1, 2, 3).filter { it > 1 }
来源：http://hz.xingfuxueyuan.xyz/gtqephvgfe.html

[T08] Kotlin：数据类
来源：http://hz.smart0.xyz/gtjnbxqodd.html

data class User(val name: String, val age: Int)
来源：http://hz.tanke756.top/gtwhhotetk.html

[T09] Kotlin：扩展函数
来源：http://hz.hywenlv.cn/gtonwyogud.html

fun String.exclaim() = this + "!"
来源：http://hz.zhoulong.xyz/gtmmywyxpq.html

[T10] Kotlin：默认参数
来源：http://hz.kuanghao11.cn/gtwnzmnibn.html

fun greet(name: String = "World") = "Hi $name"
来源：http://hz.cheryme.top/gtpgusxyrk.html

[T11] Kotlin：协程
来源：http://hz.nanxuanxn.top/gtxdxovtjs.html

GlobalScope.launch { delay(1000); println("done") }
来源：http://hz.zdqjudy.top/gtgdttvvum.html

[T12] Kotlin：解构声明
来源：http://hz.gaohongyu789.top/gttajpncll.html

val (a, b) = Pair(1, 2)
来源：http://hz.yonumen.top/gtgmoovvyn.html

[T13] Kotlin：只读 Map
来源：http://hz.ppjwa.cn/gtwcogyyfr.html

val m = mapOf("a" to 1)
来源：http://hz.jinqigufen.top/gtazlksvpd.html

[T14] Kotlin：循环
来源：http://hz.jinyuanbaomall.cn/gtduqlzbmj.html

for (i in 1..10) println(i)
来源：http://hz.shanyushiyangkeji.top/gtckyfvalx.html

[T15] Kotlin：接口
来源：http://hz.daxiang520.top/gtxgbyyvka.html

interface Shape { fun area(): Double }
来源：http://hz.zhaomingkeji.xyz/gtjuearvut.html

[T16] Swift：Hello World
来源：http://hz.yonumen.top/gtfyewlxza.html

print("Hello")
来源：http://hz.shanyushiyangtech.top/gtrhidsxup.html

[T17] Swift：变量与常量
来源：http://hz.dianchejie.cn/gtqzlxxhke.html

var a = 1;  let b = 2
来源：http://hz.hongshengwenyu.top/gtuutndqrq.html

[T18] Swift：字符串插值
来源：http://hz.gaohongyu789.top/gtogfeelpv.html

"值: \(b)"
来源：http://hz.iojbl.cn/gtvavstdox.html

[T19] Swift：可选绑定
来源：http://hz.0kj1m.cn/gtpbaxmlbz.html

if let n = opt { print(n) }
来源：http://hz.zhengqikj.top/gthlpxfvfg.html

[T20] Swift：数组操作
来源：http://hz.xylfe.cn/gtdonmjtzr.html

var a = [1, 2, 3];  a.append(4)
来源：http://hz.cdnleiting.top/gtjrwowerl.html

[T21] Swift：遍历
来源：http://hz.xingfuxueyuan.xyz/gttaxjoxar.html

for x in a { print(x) }
来源：http://hz.zhongyouzk.top/gtbvkwvoxd.html

[T22] Swift：字典
来源：http://hz.xziqi.cn/gtovnscadw.html

var d = ["a": 1];  d["b"] = 2
来源：http://hz.hongshengwenyu.top/gtixyahunv.html

[T23] Swift：函数
来源：http://hz.shuidangran.top/gtsqlbocpd.html

func add(_ a: Int, _ b: Int) -> Int { a + b }
来源：http://hz.xuetiantiany.cn/gtlqndiqim.html

[T24] Swift：闭包
来源：http://hz.hnqzz.top/gtmfgwojfq.html

let f = { (x: Int) -> Int in x * 2 }
来源：http://hz.wangdashe.top/gttzupigbr.html

[T25] Swift：结构体
来源：http://hz.jinyuanbaomall.cn/gtlukonklc.html

struct P { var x: Int }
来源：http://hz.feifeiyinyue.top/gtwcqhkhba.html

[T26] Swift：类与重写
来源：http://hz.jlsjyb.cn/gtxoytqsmp.html

class A: Base { override func f() {} }
来源：http://hz.jqgfzy.top/gtwtzztaar.html

[T27] Swift：错误处理
来源：http://hz.snrcjt.cn/gtwwtjdrxn.html

do { try f() } catch { print(error) }
来源：http://hz.nwbrower.top/gtmftnyjbp.html

[T28] Swift：枚举
来源：http://hz.ywan-chungtsiang.top/gtutjxqmpp.html

enum Color { case red, green }
来源：http://hz.xuetiantiany.cn/gtsmqfacaz.html

[T29] Swift：guard 提前返回
来源：http://hz.yuxming.cn/gtohzbmkeg.html

guard let x = opt else { return }
来源：http://hz.daxiang520.top/gtjozszext.html

[T30] Swift：协议
来源：http://hz.zhongyouzk.top/gtdxsifwxn.html

protocol Shape { func area() -> Double }
来源：http://hz.jianghu66.top/gtlxvwfhbj.html

[T31] Lua：Hello World
来源：http://hz.c1oappe.top/gtcbadqkkq.html

print("Hello")
来源：http://hz.hongshengwenyu.top/gtrobhwmye.html

[T32] Lua：局部变量
来源：http://hz.jyoumei.cn/gtttrjhtjk.html

local a = 1
来源：http://hz.hnxiangtu.top/gtkburycpb.html

[T33] Lua：表（数组）
来源：http://hz.jinqigfzy.top/gtlgugyzqf.html

local t = {1, 2, 3};  t[4] = 4
来源：http://hz.meibo888.top/gtnkhkuzxw.html

[T34] Lua：遍历表
来源：http://hz.snrcjt.cn/gtbfewgzhj.html

for i, v in ipairs(t) do print(i, v) end
来源：http://hz.jinyuanbaomall.cn/gtncasluoc.html

[T35] Lua：字典表
来源：http://hz.xylfe.cn/gthurncvno.html

local d = { a = 1 };  d.b = 2
来源：http://hz.guowangkeji.top/gtnitbghtu.html

[T36] Lua：函数
来源：http://hz.shanyushiyangtech.top/gtizbxqjra.html

function add(a, b) return a + b end
来源：http://hz.quarkkingdee.top/gtwdaunbvp.html

[T37] Lua：字符串拼接
来源：http://hz.tanke756.top/gtgvrjjqwt.html

"a" .. "b"
来源：http://hz.birdmap.top/gtwpgxeajw.html

[T38] Lua：条件
来源：http://hz.shanyushiyangkeji.top/gtfadoglse.html

if x > 0 then print("正") end
来源：http://hz.ehwqpu.com/gteaxeqmks.html

[T39] Lua：模式匹配
来源：http://hz.nanxuanxn.top/gtwsntjmtc.html

string.find(s, "%d+")
来源：http://hz.mhx1999.top/gtucvauxfp.html

[T40] Lua：元表
来源：http://hz.gotoacloud.top/gthrvqdaar.html

setmetatable({}, { __index = base })
来源：http://hz.andypj.xyz/gtbdpkarlw.html

[T41] Perl：Hello World
来源：http://hz.yj20258.top/gttuuhzdsx.html

print "Hello\n";
来源：http://hz.hongshengwenyu.top/gtpzskpskq.html

[T42] Perl：变量类型
来源：http://hz.tian-w.cn/gtwcreowwx.html

my $a = 1;  my @arr = (1, 2, 3);  my %h = (a => 1);
来源：http://hz.cashguo.top/gthfvbsodh.html

[T43] Perl：字符串插值
来源：http://hz.yongpay.top/gtmywvycdc.html

"值: $a"
来源：http://hz.sysykeji.top/gtqcrktfym.html

[T44] Perl：条件
来源：http://hz.kuanghao11.cn/gtwuroxfts.html

if ($a > 0) { print "正"; }
来源：http://hz.pengpengdd.cyou/gthlwymtwh.html

[T45] Perl：数组遍历
来源：http://hz.andypj.xyz/gtzcdktakc.html

for my $x (@arr) { print $x; }
来源：http://hz.ydzc1.top/gtafkauidj.html

[T46] Perl：哈希操作
来源：http://hz.jqgufenzy.top/gtpnfaqjda.html

$h{b} = 2;  for my $k (keys %h) { print "$k=$h{$k}"; }
来源：http://hz.hywenlv.cn/gtwtfhhmfq.html

[T47] Perl：正则捕获
来源：http://hz.redwolf501.top/gthzqbffbb.html

if ($s =~ /(\d+)/) { print $1; }
来源：http://hz.sxryk.cn/gtannkvsos.html

[T48] Perl：正则替换
来源：http://hz.ivvv.top/gtbhqjpzwe.html

$s =~ s/old/new/g;
来源：http://hz.9152youxi.cn/gtjyupxyjg.html

[T49] Perl：函数
来源：http://hz.cucudq.cn/gtalhfvwco.html

sub add { my ($a, $b) = @_; return $a + $b; }
来源：http://hz.ehwqpu.com/gtogboawpy.html

[T50] Perl：逐行读文件
来源：http://hz.shangyingyoupin.top/gtlcoixmzi.html

open my $fh, "<", "a.txt" or die $!;
来源：http://hz.kuanghao11.cn/gtwozkfxqd.html

while (my $line = <$fh>) { print $line; }
来源：http://hz.9152youxi.cn/gtlmmbwlty.html

[T51] Scala：Hello World
来源：http://hz.ydjk.org.cn/gtnjrtyxpm.html

println("Hello")
来源：http://hz.jyoumei.cn/gtnenzsrcz.html

[T52] Scala：变量
来源：http://hz.jiagoushi.top/gtrtazvebu.html

val a = 1;  var b = 2
来源：http://hz.zhaomingkeji.xyz/gtfykayeww.html

[T53] Scala：字符串插值
来源：http://hz.jinqigufen.top/gtlbqfoycu.html

s"值: $b"
来源：http://hz.jqgufenzy.top/gtdhajciba.html

[T54] Scala：集合映射
来源：http://hz.9152youxi.cn/gtjjcwgbuu.html

List(1, 2, 3).map(_ * 2)
来源：http://hz.feifeiyinyue.top/gtvpmyognp.html

[T55] Scala：集合过滤
来源：http://hz.bjfxy.top/gtjfneznbp.html

List(1, 2, 3).filter(_ > 1)
来源：http://hz.yvedp.cn/gtzwdyuyaq.html

[T56] Scala：样例类
来源：http://hz.chenlongwang.top/gtpnobuhjq.html

case class User(name: String, age: Int)
来源：http://hz.gzhubu.top/gtqxlbnytz.html

[T57] Scala：模式匹配
来源：http://hz.zdqjudy.top/gtkeubujua.html

x match { case 1 => "一"; case _ => "其他" }
来源：http://hz.pycfn.com/gtewmadzsg.html

[T58] Scala：函数定义
来源：http://hz.yuxming.cn/gtcgrozbyn.html

def add(a: Int, b: Int): Int = a + b
来源：http://hz.cheryme.top/gtmttagdnl.html

[T59] Scala：循环
来源：http://hz.aizwys.cn/gtxegkhwrd.html

for (i <- 1 to 10) println(i)
来源：http://hz.xuetiantiany.cn/gtlauzmmlz.html

[T60] Scala：折叠
来源：http://hz.jinghuilouyu.cn/gtzzdpbzya.html

List(1, 2, 3).foldLeft(0)(_ + _)
来源：http://hz.hnxiangtu.top/gtjytvjstj.html

================================================================================
来源：http://hz.cashguo.top/gtigqbrlyu.html

U. 高频实用片段（Python / PHP / JavaScript 各 40 条）
来源：http://hz.c1oappe.top/gtdgceesdu.html

================================================================================
来源：http://hz.cucudq.cn/gtkshvcoyp.html

[U01] Py：创建虚拟环境
来源：http://hz.yuxming.cn/gtypoytrvi.html

python -m venv .venv && source .venv/bin/activate
来源：http://hz.chenlongwang.top/gtnjgxedal.html

[U02] Py：导出 / 安装依赖
来源：http://hz.shuidangran.top/gtbimdfgbs.html

pip freeze > requirements.txt;  pip install -r requirements.txt
来源：http://hz.yueranfly.top/gtcurmzvwh.html

[U03] Py：加载 .env 配置
来源：http://hz.tian-w.cn/gtpidzivki.html

from dotenv import load_dotenv; load_dotenv()
来源：http://hz.shuidangran.top/gthdsuqahl.html

[U04] Py：变量调试打印
来源：http://hz.daxiang520.top/gtarrjolzz.html

print(f"{x=}")            # 输出 x=值，Python 3.8+
来源：http://hz.yueranfly.top/gtifyhuxyo.html

[U05] Py：列表去重且保序
来源：http://hz.xylfe.cn/gtulcinpqu.html

list(dict.fromkeys(arr))
来源：http://hz.pycfn.com/gtmcbunsva.html

[U06] Py：合并两个字典
来源：http://hz.zdqjudy.top/gtnweycwgd.html

{**a, **b}
来源：http://hz.iojbl.cn/gtmdggndjs.html

[U07] Py：反转字典键值
来源：http://hz.gaohongyu789.top/gttcmwmwsr.html

{v: k for k, v in d.items()}
来源：http://hz.jianghu66.top/gtzsukpcio.html

[U08] Py：展平二维列表
来源：http://hz.jinqigufen.top/gtvswhdrlg.html

[y for x in nested for y in x]
来源：http://hz.fzhhl.top/gtttusbiyr.html

[U09] Py：字典取最大值的键
来源：http://hz.shzxlz.cn/gtgrwodmmq.html

max(d, key=d.get)
来源：http://hz.316326.xyz/gtyewijtad.html

[U10] Py：按值排序字典
来源：http://hz.wangdashe.top/gtllflcgob.html

dict(sorted(d.items(), key=lambda kv: kv[1]))
来源：http://hz.pengpengdd.cyou/gtjktuxpav.html

[U11] Py：生成器表达式
来源：http://hz.jqgufenzy.top/gtelhliyxj.html

(x * 2 for x in arr)
来源：http://hz.daria6918.cn/gtjtspaifn.html

[U12] Py：取出现最多的 3 个元素
来源：http://hz.nanxuanxn.top/gtusyactxl.html

Counter(arr).most_common(3)
来源：http://hz.ybcxt.top/gtzagoybsh.html

[U13] Py：固定长度队列
来源：http://hz.tianlin.xyz/gtahvqymmt.html

deque(maxlen=10)
来源：http://hz.sufxvd.cn/gtpvejdwcd.html

[U14] Py：分组收集到列表
来源：http://hz.cheryme.top/gtfyjtzjqc.html

defaultdict(list)
来源：http://hz.dianchejie.cn/gtxlarsude.html

[U15] Py：高精度计时
来源：http://hz.daria6918.cn/gtmewnffgj.html

t = time.perf_counter()
来源：http://hz.pengpengdd.cyou/gtuexlusuo.html

[U16] Py：命令行参数解析
来源：http://hz.nanxinkj.top/gtpkuixyev.html

ap = argparse.ArgumentParser();  ap.add_argument("--name");  args = ap.parse_args()
来源：http://hz.redwolf501.top/gtmuacxqsa.html

[U17] Py：初始化日志
来源：http://hz.hammf.cn/gtvercljay.html

logging.basicConfig(level=logging.INFO)
来源：http://hz.mhx1999.top/gtmwmmmxya.html

[U18] Py：预编译正则
来源：http://hz.zhongyouzk.top/gtqtijgqfh.html

pat = re.compile(r"\d+")
来源：http://hz.ydjk.org.cn/gtafgardbw.html

[U19] Py：正则替换带回调
来源：http://hz.gogol.net.cn/gtrgwttkjq.html

re.sub(r"\d+", lambda m: str(int(m.group()) * 2), s)
来源：http://hz.yanxiufei.cn/gtymwjcbbk.html

[U20] Py：缓存函数结果
来源：http://hz.zhoulong.xyz/gtebehwaxi.html

@functools.lru_cache(maxsize=None)
来源：http://hz.zdqjudy.top/gtqnggxbwh.html

[U21] Py：自定义上下文管理器
来源：http://hz.aizwys.cn/gtnrdvurqb.html

@contextlib.contextmanager
来源：http://hz.hnqzz.top/gtdgafswzv.html

[U22] Py：矩阵转置
来源：http://hz.xuanzx.com/gtuyeacyin.html

list(zip(*m))
来源：http://hz.haohaochexian.top/gtjuxuhwbi.html

[U23] Py：分块读取大文件
来源：http://hz.zycfv.cn/gtmggehlqw.html

for chunk in iter(lambda: f.read(8192), b""):
来源：http://hz.guowangkeji.top/gtyqajbjnr.html

[U24] Py：路径操作
来源：http://hz.kuanghao11.cn/gtmthpyfcc.html

Path("a/b.txt").parent.mkdir(parents=True, exist_ok=True)
来源：http://hz.ydzc1.top/gtjbhvvflf.html

[U25] Py：CSV 按字典读
来源：http://hz.cheryme.top/gtqlwjwkyq.html

csv.DictReader(f)
来源：http://hz.smart0.xyz/gtzwljltxo.html

[U26] Py：并发下载
来源：http://hz.dianchejie.cn/gtzpflzube.html

ThreadPoolExecutor(max_workers=8).map(fetch, urls)
来源：http://hz.yanxiufei.cn/gtoeusfqqs.html

[U27] Py：异步 HTTP
来源：http://hz.tian-w.cn/gthmtcjrtg.html

aiohttp.ClientSession() 配合 async with
来源：http://hz.ydzc1.top/gtftlpejvw.html

[U28] Py：类型别名
来源：http://hz.gogol.net.cn/gtlmieesep.html

UserId = int
来源：http://hz.andypj.xyz/gtqzboitta.html

[U29] Py：属性校验
来源：http://hz.aibaodan.cn/gtyubnqpis.html

@property 与 @x.setter 配合
来源：http://hz.ydzc1.top/gtrqvpzknk.html

[U30] Py：数据类
来源：http://hz.zhongyouzk.top/gtsolebigw.html

@dataclass(slots=True)
来源：http://hz.xingfuxueyuan.xyz/gtbkbqmori.html

[U31] Py：单测
来源：http://hz.gogol.net.cn/gtxvoooots.html

python -m pytest -q
来源：http://hz.shzxlz.cn/gtpuuhtwle.html

[U32] Py：代码格式化
来源：http://hz.sufxvd.cn/gtcxovfbkj.html

ruff format . && ruff check --fix .
来源：http://hz.birdmap.top/gtreznkklg.html

[U33] Py：打包发布
来源：http://hz.cucudq.cn/gtwfpjetno.html

python -m build  （依赖 pyproject.toml）
来源：http://hz.xylfe.cn/gtlkquhifg.html

[U34] Py：判断编码
来源：http://hz.xingfuxueyuan.xyz/gtbeknvcgs.html

chardet.detect(raw)
来源：http://hz.zhongyouzk.top/gtpqbsrdta.html

[U35] Py：发送邮件
来源：http://hz.yangfankeji.com/gttybhkzxd.html

smtplib.SMTP_SSL(...).send_message(msg)
来源：http://hz.meibo888.top/gtpchnoimy.html

[U36] Py：定时任务
来源：http://hz.shanyushiyangtech.top/gtoidenqut.html

schedule.every(10).minutes.do(job)
来源：http://hz.cqqwz.cn/gtrqebulsn.html

[U37] Py：读写 Excel
来源：http://hz.svipenyu.cn/gtegxasxmx.html

pandas.read_excel / DataFrame.to_excel
来源：http://hz.zhixingplan.top/gtnacbelpp.html

[U38] Py：获取脚本所在目录
来源：http://hz.tianlin.xyz/gtzhvvnegi.html

Path(__file__).resolve().parent
来源：http://hz.yangfankeji.com/gtvfokcdae.html

[U39] Py：判断是否在交互环境
来源：http://hz.yueranfly.top/gtrclkpwsy.html

sys.stdout.isatty()
来源：http://hz.fengsongda.top/gtmxhmevjh.html

[U40] Py：打印到标准错误
来源：http://hz.andypj.xyz/gtfmbjryrd.html

print("err", file=sys.stderr)
来源：http://hz.tanke756.top/gtfnmspuir.html

[U41] PHP：初始化 Composer 项目
来源：http://hz.shanyushiyangtech.top/gtkorqdhuo.html

composer init;  composer require guzzlehttp/guzzle
来源：http://hz.tianlin.xyz/gtsuuynsju.html

[U42] PHP：PSR-4 自动加载
来源：http://hz.shuidangran.top/gttydytsfv.html

"autoload": { "psr-4": { "App\\": "src/" } }
来源：http://hz.yj20258888.top/gtsdpbpztk.html

[U43] PHP：声明命名空间
来源：http://hz.xuetiantiany.cn/gtvltnpjwm.html

namespace App\Http;
来源：http://hz.ppjwa.cn/gtzxhgiffc.html

[U44] PHP：开启严格类型
来源：http://hz.sufxvd.cn/gtaturmrtr.html

declare(strict_types=1);
来源：http://hz.guannengcc.top/gttrsucxdr.html


<!-- 参考信息 -->