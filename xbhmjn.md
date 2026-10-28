代发 wailian999

atoi("42");  strtod("3.14", NULL);
来源：http://hz.yangfankeji.com/gtijvwddam.html

[S23] C：随机数
来源：http://hz.xuetiantiany.cn/gtjzxemwng.html

srand(time(NULL));  int r = rand() % 100;
来源：http://hz.yuxming.cn/gtgnqcovue.html

[S24] C：获取本地时间
来源：http://hz.snrcjt.cn/gtzmyrbtzh.html

time_t t = time(NULL);  struct tm *tm = localtime(&t);
来源：http://hz.fengsongda.top/gtjhszofuk.html

[S25] C：内存拷贝
来源：http://hz.zdqjudy.top/gtphtmoxhe.html

memcpy(dst, src, n);
来源：http://hz.gogol.net.cn/gtsczmarzf.html

[S26] C：内存清零
来源：http://hz.xziqi.cn/gtratvxjvg.html

memset(a, 0, sizeof a);
来源：http://hz.cdnleiting.top/gtddbqdwfh.html

[S27] C：定义常量
来源：http://hz.cdnleiting.top/gtibsrakxs.html

const double PI = 3.14159;
来源：http://hz.xuanzx.com/gtekhxolbv.html

[S28] C：静态变量
来源：http://hz.havefunace.top/gtfqcxrsuw.html

static int counter = 0;
来源：http://hz.yuanzhike.top/gthixsvcqy.html

[S29] C：变参函数
来源：http://hz.haohaochexian.top/gtimitprfy.html

va_list ap; va_start(ap, fmt); vprintf(fmt, ap); va_end(ap);
来源：http://hz.shzxlz.cn/gtkffylwrf.html

[S30] C：头文件保护
来源：http://hz.mhx1999.top/gtukbrytgu.html

#ifndef X_H
来源：http://hz.fengsongda.top/gtrmyeayob.html

#define X_H
来源：http://hz.zhongyouzk.top/gtzyaqpslp.html

#endif
来源：http://hz.zhiwuduotai.top/gtnkanmfyp.html

[S31] C++：Hello World
来源：http://hz.yangfankeji.com/gtykglatox.html

#include <iostream>
来源：http://hz.bjfxy.top/gtzygysthn.html

int main() { std::cout << "Hello\n"; }
来源：http://hz.gotoacloud.top/gtrowyeuyr.html

[S32] C++：字符串
来源：http://hz.hnqzz.top/gtxqraajrg.html

std::string s = "hi";  s += "!";
来源：http://hz.hywenlv.cn/gtpsegbodm.html

[S33] C++：vector 增删
来源：http://hz.hnxiangtu.top/gtxaivxolw.html

std::vector<int> v{1, 2, 3};  v.push_back(4);
来源：http://hz.shanyushiyangkeji.top/gthfvovrbt.html

[S34] C++：遍历 vector
来源：http://hz.pengpengdd.cyou/gtnezynhrt.html

for (auto &x : v) { std::cout << x; }
来源：http://hz.gaohongyu789.top/gtpdpjnzwg.html

[S35] C++：map
来源：http://hz.quarkkingdee.top/gtomzbvefk.html

std::map<std::string, int> m;  m["a"] = 1;
来源：http://hz.vqdsnc.cn/gtyyxsaqji.html

[S36] C++：unordered_map
来源：http://hz.kuanghao11.cn/gtxyysokpa.html

std::unordered_map<std::string, int> m;  m["a"] = 1;
来源：http://hz.havefunace.top/gtmipiiawb.html

[S37] C++：set
来源：http://hz.daria6918.cn/gtsonudpqz.html

std::set<int> s{1, 2, 3};  s.insert(4);
来源：http://hz.jinqigfzy.top/gtqgbbdsmx.html

[S38] C++：排序
来源：http://hz.hnqzz.top/gtjkfwxikj.html

std::sort(v.begin(), v.end());
来源：http://hz.hysaishi.cn/gteicwefnk.html

[S39] C++：自定义比较器排序
来源：http://hz.shanyushiyangkeji.top/gtrgwpacjg.html

std::sort(v.begin(), v.end(), [](int a, int b) { return a > b; });
来源：http://hz.redwolf501.top/gtlvroazfj.html

[S40] C++：查找元素
来源：http://hz.316326.xyz/gtztlobnwu.html

auto it = std::find(v.begin(), v.end(), 3);
来源：http://hz.ydjk.org.cn/gtezpnjnur.html

[S41] C++：类与构造函数
来源：http://hz.shzxlz.cn/gtanazimyg.html

class A { public: A(int v) : x_(v) {} int get() const { return x_; } private: int x_; };
来源：http://hz.jianghu66.top/gtzbipbwiz.html

[S42] C++：继承与虚函数
来源：http://hz.zhijiandao.cn/gtbjnsngiv.html

class B : public Base { public: void f() override {} };
来源：http://hz.bjfxy.top/gteylhzjir.html

[S43] C++：智能指针
来源：http://hz.zycfv.cn/gtlofaxvxz.html

auto p = std::make_unique<int>(5);
来源：http://hz.zhoulong.xyz/gtlflimngj.html

[S44] C++：引用传参
来源：http://hz.cqqwz.cn/gtmsgzdfio.html

void inc(int &x) { ++x; }
来源：http://hz.haohaochexian.top/gtnnnxkilp.html

[S45] C++：lambda
来源：http://hz.jiagoushi.top/gtprwffudf.html

auto add = [](int a, int b) { return a + b; };
来源：http://hz.yueranfly.top/gthxgfardt.html

[S46] C++：函数模板
来源：http://hz.feifeiyinyue.top/gtwkoxbplt.html

template <typename T> T maxv(T a, T b) { return a > b ? a : b; }
来源：http://hz.haohaochexian.top/gtdzbtbnjp.html

[S47] C++：结构化绑定遍历
来源：http://hz.cashguo.top/gtvqlolwjj.html

for (const auto &[k, v] : m) { std::cout << k << v; }
来源：http://hz.gaohongyu789.top/gtcvhxuwjn.html

[S48] C++：逐行读文件
来源：http://hz.jianghu66.top/gtmyznqtsg.html

std::ifstream in("a.txt");  std::string line;
来源：http://hz.dianchejie.cn/gtmzafecki.html

while (std::getline(in, line)) { }
来源：http://hz.pengpengdd.cyou/gtzxbtqyca.html

[S49] C++：写文件
来源：http://hz.smart0.xyz/gtgqucdlqq.html

std::ofstream out("a.txt");  out << "hi\n";
来源：http://hz.shanyushiyangkeji.top/gtchogqabd.html

[S50] C++：格式化数字
来源：http://hz.pycfn.com/gtrpzmujbp.html

std::ostringstream os;  os << std::fixed << std::setprecision(2) << 3.14159;
来源：http://hz.9152youxi.cn/gtpxadjhui.html

[S51] C++：显式类型转换
来源：http://hz.dashuyun.cn/gtvbhvlvcf.html

static_cast<double>(a) / b
来源：http://hz.shangyingyoupin.top/gtpwqzajib.html

[S52] C++：const 与 noexcept
来源：http://hz.vqdsnc.cn/gtxpwpddup.html

int size() const noexcept { return n_; }
来源：http://hz.daria6918.cn/gttkpmzgci.html

[S53] C++：移动语义
来源：http://hz.tian-w.cn/gtjexgoffc.html

std::vector<int> w = std::move(v);
来源：http://hz.tianlin.xyz/gtcnrgpwif.html

[S54] C++：异常处理
来源：http://hz.zhijiandao.cn/gtmbmfhsmh.html

try { throw std::runtime_error("x"); } catch (const std::exception &e) { }
来源：http://hz.mhx1999.top/gtzyqdzlxb.html

[S55] C++：结构化绑定
来源：http://hz.yj20258.top/gtfnsjpalj.html

auto [a, b] = std::make_pair(1, 2);
来源：http://hz.haohaochexian.top/gthsewmnco.html

[S56] C++：optional
来源：http://hz.dashuyun.cn/gthdecbekx.html

std::optional<int> o = 5;  if (o) { int v = *o; }
来源：http://hz.zhengqikj.top/gtfiemauey.html

[S57] C++：编译期常量
来源：http://hz.yueranfly.top/gteianfbob.html

constexpr int N = 10;
来源：http://hz.shanyushiyangtech.top/gteceykfhj.html

[S58] C++：命名空间
来源：http://hz.yongpay.top/gtuokgcrau.html

namespace ns { int f() { return 1; } }
来源：http://hz.0kj1m.cn/gtqblamrht.html

[S59] C++：静态断言
来源：http://hz.yangfankeji.com/gtqjtrvvnj.html

static_assert(sizeof(int) == 4, "int 必须 4 字节");
来源：http://hz.svipenyu.cn/gtfhjyigfm.html

[S60] C++：遍历并删除元素
来源：http://hz.zhixingplan.top/gtpkslgehb.html

v.erase(std::remove_if(v.begin(), v.end(), [](int x) { return x < 0; }), v.end());
来源：http://hz.jlsjyb.cn/gtlvzbbhxk.html

================================================================================
来源：http://hz.yuxming.cn/gtdzxalvsn.html

T. 其他语言补充（Kotlin / Swift / Lua / Perl / Scala）
来源：http://hz.gogol.net.cn/gtlshfnmwz.html

================================================================================
来源：http://hz.gzhubu.top/gttsqcidvf.html

[T01] Kotlin：Hello World
来源：http://hz.hnqzz.top/gtizpndimx.html

println("Hello")
来源：http://hz.pengpengdd.cyou/gtwbeqjdyu.html

[T02] Kotlin：变量
来源：http://hz.kuanghao11.cn/gtgmtmipop.html

val a = 1;  var b = 2        // val 只读，var 可变
来源：http://hz.sysykeji.top/gtpoqrkehj.html

[T03] Kotlin：字符串模板
来源：http://hz.yueranfly.top/gtrfavkjlv.html

"值: $b"
来源：http://hz.yj20258888.top/gtrwvdjrnb.html

[T04] Kotlin：空安全
来源：http://hz.bjfxy.top/gtflnwiuqe.html

val n: String? = null;  n?.length
来源：http://hz.shanyushiyangkeji.top/gtlooykkzz.html

[T05] Kotlin：when 表达式
来源：http://hz.sxryk.cn/gtddvoyqkq.html

val s = when (x) { 1 -> "一" else -> "其他" }   // 多分支时每个分支单独一行
来源：http://hz.316326.xyz/gtgsvjetak.html

[T06] Kotlin：集合映射
来源：http://hz.yangfankeji.com/gtcpyeqawk.html

listOf(1, 2, 3).map { it * 2 }
来源：http://hz.ppjwa.cn/gttzyoxfgt.html

[T07] Kotlin：集合过滤
来源：http://hz.cheryme.top/gtfvuchsvl.html

listOf(1, 2, 3).filter { it > 1 }
来源：http://hz.jlsjyb.cn/gthyrridbh.html

[T08] Kotlin：数据类
来源：http://hz.birdmap.top/gterulntwk.html

data class User(val name: String, val age: Int)
来源：http://hz.hongshengwenyu.top/gtxnktzrpg.html

[T09] Kotlin：扩展函数
来源：http://hz.jinyuanbaomall.cn/gtxnfizuic.html

fun String.exclaim() = this + "!"
来源：http://hz.zhongyouzk.top/gtzsytyaqp.html

[T10] Kotlin：默认参数
来源：http://hz.ywan-chungtsiang.top/gtklcmdwwg.html

fun greet(name: String = "World") = "Hi $name"
来源：http://hz.hywenlv.cn/gtfxqwfohx.html

[T11] Kotlin：协程
来源：http://hz.zycfv.cn/gtlnpbhotx.html

GlobalScope.launch { delay(1000); println("done") }
来源：http://hz.mhx1999.top/gtzizekkbp.html

[T12] Kotlin：解构声明
来源：http://hz.zhengqikj.top/gtmxkmpqqj.html

val (a, b) = Pair(1, 2)
来源：http://hz.hongshengwenyu.top/gtyyygdlpv.html

[T13] Kotlin：只读 Map
来源：http://hz.yangfankeji.com/gtmerlobyr.html

val m = mapOf("a" to 1)
来源：http://hz.wangshuangyany.cn/gttdcfjwpb.html

[T14] Kotlin：循环
来源：http://hz.xuanzx.com/gtsunktafs.html

for (i in 1..10) println(i)
来源：http://hz.hnxiangtu.top/gtqodtcgce.html

[T15] Kotlin：接口
来源：http://hz.hysaishi.cn/gtkgwkdgyb.html

interface Shape { fun area(): Double }
来源：http://hz.316326.xyz/gttgseumut.html

[T16] Swift：Hello World
来源：http://hz.yueranfly.top/gtdyhkfpkw.html

print("Hello")
来源：http://hz.zhixingplan.top/gttxsvfycq.html

[T17] Swift：变量与常量
来源：http://hz.jinqigfzy.top/gtcdvljfqb.html

var a = 1;  let b = 2
来源：http://hz.gzhubu.top/gtnuiemwlt.html

[T18] Swift：字符串插值
来源：http://hz.jinqigufen.top/gtmdarcgot.html

"值: \(b)"
来源：http://hz.tanke756.top/gtgrjexfki.html

[T19] Swift：可选绑定
来源：http://hz.yonumen.top/gtsoqifmml.html

if let n = opt { print(n) }
来源：http://hz.andypj.xyz/gtsfqftgti.html

[T20] Swift：数组操作
来源：http://hz.birdmap.top/gtdrsipzzw.html

var a = [1, 2, 3];  a.append(4)
来源：http://hz.chenzaomai.com/gtyrczjwir.html

[T21] Swift：遍历
来源：http://hz.jinqigufen.top/gtbgqntkql.html

for x in a { print(x) }
来源：http://hz.smart0.xyz/gtdeeulwlf.html

[T22] Swift：字典
来源：http://hz.ydzc1.top/gtzwfcqbda.html

var d = ["a": 1];  d["b"] = 2
来源：http://hz.sxryk.cn/gttaoscanz.html

[T23] Swift：函数
来源：http://hz.aibaodan.cn/gtfylkqewp.html

func add(_ a: Int, _ b: Int) -> Int { a + b }
来源：http://hz.c1oappe.top/gtoasgbutr.html

[T24] Swift：闭包
来源：http://hz.xylfe.cn/gtcmyxwljq.html

let f = { (x: Int) -> Int in x * 2 }
来源：http://hz.shanyushiyangkeji.top/gtwiwkygaj.html

[T25] Swift：结构体
来源：http://hz.vqdsnc.cn/gtlzhgtmko.html

struct P { var x: Int }
来源：http://hz.yonumen.top/gtdtghtibm.html

[T26] Swift：类与重写
来源：http://hz.guowangkeji.top/gtudowjytl.html

class A: Base { override func f() {} }
来源：http://hz.xuetiantiany.cn/gtedjkavhk.html

[T27] Swift：错误处理
来源：http://hz.daria6918.cn/gtcjszdxxl.html

do { try f() } catch { print(error) }
来源：http://hz.gotoacloud.top/gtaycibbeh.html

[T28] Swift：枚举
来源：http://hz.yj202588.top/gtrfbbltpo.html

enum Color { case red, green }
来源：http://hz.mhx1999.top/gtfrasmpzt.html

[T29] Swift：guard 提前返回
来源：http://hz.yanxiufei.cn/gtruqzkyon.html

guard let x = opt else { return }
来源：http://hz.shangyingyoupin.top/gtkwgpscwn.html

[T30] Swift：协议
来源：http://hz.zhoulong.xyz/gtjssdgajt.html

protocol Shape { func area() -> Double }
来源：http://hz.ehwqpu.com/gtppdlsaxl.html

[T31] Lua：Hello World
来源：http://hz.ppjwa.cn/gtswummqji.html

print("Hello")
来源：http://hz.xingfuxueyuan.xyz/gtjkbgtgry.html

[T32] Lua：局部变量
来源：http://hz.sysykeji.top/gtqqkhochl.html

local a = 1
来源：http://hz.feifeiyinyue.top/gtmzfbaokb.html

[T33] Lua：表（数组）
来源：http://hz.zdqjudy.top/gtrechrsav.html

local t = {1, 2, 3};  t[4] = 4
来源：http://hz.yuxming.cn/gtdoouoygv.html

[T34] Lua：遍历表
来源：http://hz.tianlin.xyz/gtalaoczkx.html

for i, v in ipairs(t) do print(i, v) end
来源：http://hz.yueranfly.top/gttdesljqr.html

[T35] Lua：字典表
来源：http://hz.sysykeji.top/gtbltyckqq.html

local d = { a = 1 };  d.b = 2
来源：http://hz.yanxiufei.cn/gtedjxwanf.html

[T36] Lua：函数
来源：http://hz.meibo888.top/gtmqzxaxjq.html

function add(a, b) return a + b end
来源：http://hz.chenjidiqi.icu/gtnxbbtkaq.html

[T37] Lua：字符串拼接
来源：http://hz.tanke756.top/gttivgvgqi.html

"a" .. "b"
来源：http://hz.pengpengdd.cyou/gtirfsxehj.html

[T38] Lua：条件
来源：http://hz.ppjwa.cn/gtpuuzeklg.html

if x > 0 then print("正") end
来源：http://hz.zhengqikj.top/gtthnjfxec.html

[T39] Lua：模式匹配
来源：http://hz.hfpthk.cn/gtrrpkwdzx.html

string.find(s, "%d+")
来源：http://hz.daxiang520.top/gtldohoafv.html

[T40] Lua：元表
来源：http://hz.yuxming.cn/gtksbvkutl.html

setmetatable({}, { __index = base })
来源：http://hz.316326.xyz/gtqgxxvyhv.html

[T41] Perl：Hello World
来源：http://hz.yvedp.cn/gtucgpjcwf.html

print "Hello\n";
来源：http://hz.guannengcc.top/gtlnpdeoln.html

[T42] Perl：变量类型
来源：http://hz.svipenyu.cn/gtegeexjck.html

my $a = 1;  my @arr = (1, 2, 3);  my %h = (a => 1);
来源：http://hz.mhx1999.top/gtnpnsyubz.html

[T43] Perl：字符串插值
来源：http://hz.chenlongwang.top/gtiwhkicmy.html

"值: $a"
来源：http://hz.fengsongda.top/gtogzqedbl.html

[T44] Perl：条件
来源：http://hz.jinqigfzy.top/gtcplsbcnp.html

if ($a > 0) { print "正"; }
来源：http://hz.shangyingyoupin.top/gtpfmbtuzy.html

[T45] Perl：数组遍历
来源：http://hz.andypj.xyz/gtvtaxijve.html

for my $x (@arr) { print $x; }
来源：http://hz.52xcode.cn/gtjfqrrnrv.html

[T46] Perl：哈希操作
来源：http://hz.shuidangran.top/gticlmfbda.html

$h{b} = 2;  for my $k (keys %h) { print "$k=$h{$k}"; }
来源：http://hz.hfpthk.cn/gtfffuhbbz.html

[T47] Perl：正则捕获
来源：http://hz.shanyushiyangkeji.top/gtsuwthvsd.html

if ($s =~ /(\d+)/) { print $1; }
来源：http://hz.dashuyun.cn/gtqilvjwno.html

[T48] Perl：正则替换
来源：http://hz.zhiwuduotai.top/gtwzmrilcv.html

$s =~ s/old/new/g;
来源：http://hz.hongshengwenyu.top/gtegqjnmnz.html

[T49] Perl：函数
来源：http://hz.jinqigfzy.top/gtgcstwowx.html

sub add { my ($a, $b) = @_; return $a + $b; }
来源：http://hz.zdqjudy.top/gtxnonvwra.html

[T50] Perl：逐行读文件
来源：http://hz.sxryk.cn/gtcoetmudt.html

open my $fh, "<", "a.txt" or die $!;
来源：http://hz.9152youxi.cn/gtyzfqrism.html

while (my $line = <$fh>) { print $line; }
来源：http://hz.ivvv.top/gtiixmhrkv.html

[T51] Scala：Hello World
来源：http://hz.cheryme.top/gtzjjvwqug.html

println("Hello")
来源：http://hz.nwbrower.top/gtbjehzlum.html

[T52] Scala：变量
来源：http://hz.zhoulong.xyz/gtmqroojfz.html

val a = 1;  var b = 2
来源：http://hz.jqgufenzy.top/gtwgasgxyp.html

[T53] Scala：字符串插值
来源：http://hz.zhoulong.xyz/gtzcxdkiir.html

s"值: $b"
来源：http://hz.haohaochexian.top/gtemqhkrqy.html

[T54] Scala：集合映射
来源：http://hz.zhoulong.xyz/gtsrcxgwln.html

List(1, 2, 3).map(_ * 2)
来源：http://hz.mhx1999.top/gtcqxahhtu.html

[T55] Scala：集合过滤
来源：http://hz.birdmap.top/gtoucscdgd.html

List(1, 2, 3).filter(_ > 1)
来源：http://hz.iojbl.cn/gtfuferzcc.html

[T56] Scala：样例类
来源：http://hz.yongpay.top/gtxpqetmkw.html

case class User(name: String, age: Int)
来源：http://hz.ydzc1.top/gtjdidllli.html

[T57] Scala：模式匹配
来源：http://hz.yanxiufei.cn/gtqmgrjdzg.html

x match { case 1 => "一"; case _ => "其他" }
来源：http://hz.fengsongda.top/gtkytrugkr.html

[T58] Scala：函数定义
来源：http://hz.zhiwuduotai.top/gtngwbuyhe.html

def add(a: Int, b: Int): Int = a + b
来源：http://hz.hammf.cn/gtbmoboigm.html

[T59] Scala：循环
来源：http://hz.yonumen.top/gtwnlbtwmd.html

for (i <- 1 to 10) println(i)
来源：http://hz.yj20258.top/gtargcjcym.html

[T60] Scala：折叠
来源：http://hz.hysaishi.cn/gtyoffkuzd.html

List(1, 2, 3).foldLeft(0)(_ + _)
来源：http://hz.gaohongyu789.top/gtgdjlopns.html

================================================================================
来源：http://hz.nanxinkj.top/gtdwxqvvek.html

U. 高频实用片段（Python / PHP / JavaScript 各 40 条）
来源：http://hz.cheryme.top/gtemjowfjm.html

================================================================================
来源：http://hz.cucudq.cn/gthmfyvkof.html

[U01] Py：创建虚拟环境
来源：http://hz.yj20258888.top/gtzcinjijs.html

python -m venv .venv && source .venv/bin/activate
来源：http://hz.sxryk.cn/gtytgrpsbd.html

[U02] Py：导出 / 安装依赖
来源：http://hz.gzhubu.top/gtjoqbpcvo.html

pip freeze > requirements.txt;  pip install -r requirements.txt
来源：http://hz.ppjwa.cn/gtwvivdpve.html

[U03] Py：加载 .env 配置
来源：http://hz.cdnleiting.top/gtfjfbsfvv.html

from dotenv import load_dotenv; load_dotenv()
来源：http://hz.cheryme.top/gtjazmgowh.html

[U04] Py：变量调试打印
来源：http://hz.zhijiandao.cn/gteoroyupk.html

print(f"{x=}")            # 输出 x=值，Python 3.8+
来源：http://hz.yj20258888.top/gtngrjasyd.html

[U05] Py：列表去重且保序
来源：http://hz.jiagoushi.top/gtivxvgtln.html

list(dict.fromkeys(arr))
来源：http://hz.wangdashe.top/gttegrlerx.html

[U06] Py：合并两个字典
来源：http://hz.haohaochexian.top/gtavoxrilr.html

{**a, **b}
来源：http://hz.daxiang520.top/gtaijkflcr.html

[U07] Py：反转字典键值
来源：http://hz.52xcode.cn/gtuagcxjam.html

{v: k for k, v in d.items()}
来源：http://hz.dianchejie.cn/gtxxzperhy.html

[U08] Py：展平二维列表
来源：http://hz.c1oappe.top/gtxnxvcjpm.html

[y for x in nested for y in x]
来源：http://hz.snrcjt.cn/gtgklkzgrj.html

[U09] Py：字典取最大值的键
来源：http://hz.daxiang520.top/gtktaxabdr.html

max(d, key=d.get)
来源：http://hz.aibaodan.cn/gtlzgmhenq.html

[U10] Py：按值排序字典
来源：http://hz.hnqzz.top/gtjloqoetj.html

dict(sorted(d.items(), key=lambda kv: kv[1]))
来源：http://hz.dashuyun.cn/gtwzdpnsdp.html

[U11] Py：生成器表达式
来源：http://hz.shanyushiyangtech.top/gtqpivojzf.html

(x * 2 for x in arr)
来源：http://hz.shanyushiyangtech.top/gtzsxbreox.html

[U12] Py：取出现最多的 3 个元素
来源：http://hz.hywenlv.cn/gtzjiloqnv.html

Counter(arr).most_common(3)
来源：http://hz.jqgufenzy.top/gtdrqbvbfn.html

[U13] Py：固定长度队列
来源：http://hz.zhengqikj.top/gtkugyeqcm.html

deque(maxlen=10)
来源：http://hz.yanxiufei.cn/gtusqaleom.html

[U14] Py：分组收集到列表
来源：http://hz.sweek.top/gtmpfstuan.html

defaultdict(list)
来源：http://hz.zhiwuduotai.top/gttlegvnzj.html

[U15] Py：高精度计时
来源：http://hz.yueranfly.top/gtuvsykalq.html

t = time.perf_counter()
来源：http://hz.sweek.top/gtekcaunie.html

[U16] Py：命令行参数解析
来源：http://hz.zhiwuduotai.top/gtodnnhsxc.html

ap = argparse.ArgumentParser();  ap.add_argument("--name");  args = ap.parse_args()
来源：http://hz.yueranfly.top/gtlmywfhde.html

[U17] Py：初始化日志
来源：http://hz.cucudq.cn/gtnzlghadf.html

logging.basicConfig(level=logging.INFO)
来源：http://hz.yonumen.top/gtffacnhbn.html

[U18] Py：预编译正则
来源：http://hz.gzhubu.top/gtfictrcpb.html

pat = re.compile(r"\d+")
来源：http://hz.nwbrower.top/gtvqchrhlu.html

[U19] Py：正则替换带回调
来源：http://hz.gotoacloud.top/gtrijmhwvn.html

re.sub(r"\d+", lambda m: str(int(m.group()) * 2), s)
来源：http://hz.shuidangran.top/gtznlctnsl.html

[U20] Py：缓存函数结果
来源：http://hz.yanxiufei.cn/gtezbdqsql.html

@functools.lru_cache(maxsize=None)
来源：http://hz.gzhubu.top/gtobizlhvb.html

[U21] Py：自定义上下文管理器
来源：http://hz.shzxlz.cn/gtwoknvpsb.html

@contextlib.contextmanager
来源：http://hz.shuidangran.top/gtrgpevhnk.html

[U22] Py：矩阵转置
来源：http://hz.xziqi.cn/gtkvthedbd.html

list(zip(*m))
来源：http://hz.zhongyouzk.top/gtoymqjpts.html

[U23] Py：分块读取大文件
来源：http://hz.xingfuxueyuan.xyz/gttmxzgtev.html

for chunk in iter(lambda: f.read(8192), b""):
来源：http://hz.cqqwz.cn/gtfvpynofy.html

[U24] Py：路径操作
来源：http://hz.hywenlv.cn/gtwlfyowju.html

Path("a/b.txt").parent.mkdir(parents=True, exist_ok=True)
来源：http://hz.nanxinkj.top/gtybjfjfxp.html

[U25] Py：CSV 按字典读
来源：http://hz.iojbl.cn/gtmqrzjqdw.html

csv.DictReader(f)
来源：http://hz.tianlin.xyz/gtvfaqpkde.html

[U26] Py：并发下载
来源：http://hz.ybcxt.top/gtrstjhpeg.html

ThreadPoolExecutor(max_workers=8).map(fetch, urls)
来源：http://hz.gzhubu.top/gtbnscytlg.html

[U27] Py：异步 HTTP
来源：http://hz.wangdashe.top/gtzaexgufs.html

aiohttp.ClientSession() 配合 async with
来源：http://hz.daria6918.cn/gtgifioybb.html

[U28] Py：类型别名
来源：http://hz.chenjidiqi.icu/gtdcjwniyc.html

UserId = int
来源：http://hz.gotoacloud.top/gtdoagpsqo.html

[U29] Py：属性校验
来源：http://hz.yangfankeji.com/gtpfifotva.html

@property 与 @x.setter 配合
来源：http://hz.hnqzz.top/gtiyotpkqm.html

[U30] Py：数据类
来源：http://hz.wangshuangyany.cn/gtranbzeou.html

@dataclass(slots=True)
来源：http://hz.sufxvd.cn/gtjqqzwvus.html

[U31] Py：单测
来源：http://hz.smart0.xyz/gtihjeawyr.html

python -m pytest -q
来源：http://hz.zhijiandao.cn/gtuzubuslg.html

[U32] Py：代码格式化
来源：http://hz.quarkkingdee.top/gtlchavvtv.html

ruff format . && ruff check --fix .
来源：http://hz.pycfn.com/gtvgiulblc.html

[U33] Py：打包发布
来源：http://hz.ppjwa.cn/gtapzbupan.html

python -m build  （依赖 pyproject.toml）
来源：http://hz.jinqigufen.top/gtknnopxiw.html

[U34] Py：判断编码
来源：http://hz.dianchejie.cn/gtttrowrwg.html

chardet.detect(raw)
来源：http://hz.gaohongyu789.top/gtldgidpph.html

[U35] Py：发送邮件
来源：http://hz.jiagoushi.top/gtsyyomhxm.html

smtplib.SMTP_SSL(...).send_message(msg)
来源：http://hz.mhx1999.top/gtdgnsjstm.html

[U36] Py：定时任务
来源：http://hz.0kj1m.cn/gtgvppnsef.html

schedule.every(10).minutes.do(job)
来源：http://hz.pengpengdd.cyou/gthsxeznfm.html

[U37] Py：读写 Excel
来源：http://hz.aibaodan.cn/gtnummfiiz.html

pandas.read_excel / DataFrame.to_excel
来源：http://hz.shanyushiyangtech.top/gtdmvrynhk.html

[U38] Py：获取脚本所在目录
来源：http://hz.nanxinkj.top/gtzzgfuavv.html

Path(__file__).resolve().parent
来源：http://hz.shangyingyoupin.top/gtldcdadje.html

[U39] Py：判断是否在交互环境
来源：http://hz.ywan-chungtsiang.top/gtugsiawpk.html

sys.stdout.isatty()
来源：http://hz.cheryme.top/gtnwpctdja.html

[U40] Py：打印到标准错误
来源：http://hz.sxryk.cn/gtnriibvkw.html

print("err", file=sys.stderr)
来源：http://hz.yj202588.top/gtpzmpfutl.html

[U41] PHP：初始化 Composer 项目
来源：http://hz.zhixingplan.top/gtcsuiywxw.html

composer init;  composer require guzzlehttp/guzzle
来源：http://hz.yj202588.top/gtugiyzmen.html

[U42] PHP：PSR-4 自动加载
来源：http://hz.wangshuangyany.cn/gtdizztyku.html

"autoload": { "psr-4": { "App\\": "src/" } }
来源：http://hz.jyoumei.cn/gtpjcgjpou.html

[U43] PHP：声明命名空间
来源：http://hz.hfpthk.cn/gtujeymfrh.html

namespace App\Http;
来源：http://hz.sysykeji.top/gtojvdjroh.html

[U44] PHP：开启严格类型
来源：http://hz.cdnleiting.top/gtrlhebbwp.html

declare(strict_types=1);
来源：http://hz.mhx1999.top/gtnwwhfltf.html

[U45] PHP：类型声明与返回类型
来源：http://hz.shuidangran.top/gtzfmboiia.html

function add(int $a, int $b): int { return $a + $b; }
来源：http://hz.birdmap.top/gtqsebtome.html

[U46] PHP：可空类型
来源：http://hz.hongshengwenyu.top/gtacrphhrl.html

?string $name = null
来源：http://hz.snrcjt.cn/gtbcwcgawl.html


<!-- 参考信息 -->