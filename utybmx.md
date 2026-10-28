代发 wailian999

enum Color { RED, GREEN, BLUE };
来源：http://hz.dianchejie.cn/gtttggqrji.html

[S15] C：类型转换
来源：http://hz.gogol.net.cn/gtxwxqzvjh.html

(double) a / b
来源：http://hz.zycfv.cn/gtffyqporb.html

[S16] C：位操作置位
来源：http://hz.jinqigufen.top/gtmcrogmpj.html

x |= (1 << 3);
来源：http://hz.52xcode.cn/gtjqbzjweo.html

[S17] C：安全拼接字符串
来源：http://hz.daxiang520.top/gtlofvhmmk.html

snprintf(buf, sizeof buf, "%s%s", a, b);
来源：http://hz.sufxvd.cn/gtdjkhjoit.html

[S18] C：命令行参数
来源：http://hz.guannengcc.top/gtyballrfj.html

int main(int argc, char **argv)
来源：http://hz.aizwys.cn/gtcvtdfvek.html

[S19] C：快速排序
来源：http://hz.aibaodan.cn/gtricnztbf.html

qsort(a, n, sizeof(int), cmp);
来源：http://hz.9152youxi.cn/gtbchrxvgr.html

[S20] C：二分查找
来源：http://hz.shuidangran.top/gttcuqeqvr.html

bsearch(&key, a, n, sizeof(int), cmp);
来源：http://hz.zdqjudy.top/gtshrntgok.html

[S21] C：字符类别判断
来源：http://hz.yueranfly.top/gtdnnmpzwx.html

isdigit(c);  isalpha(c);  isspace(c);
来源：http://hz.pengpengdd.cyou/gtwbfcvzko.html

[S22] C：字符串转数字
来源：http://hz.hfpthk.cn/gttfqvlfau.html

atoi("42");  strtod("3.14", NULL);
来源：http://hz.aibaodan.cn/gtutpzmnpo.html

[S23] C：随机数
来源：http://hz.daria6918.cn/gtaamtgsju.html

srand(time(NULL));  int r = rand() % 100;
来源：http://hz.daxiang520.top/gtczydgtbw.html

[S24] C：获取本地时间
来源：http://hz.yj202588.top/gtoyiioscm.html

time_t t = time(NULL);  struct tm *tm = localtime(&t);
来源：http://hz.chenzaomai.com/gtadzjkglm.html

[S25] C：内存拷贝
来源：http://hz.c1oappe.top/gtfqdqmwds.html

memcpy(dst, src, n);
来源：http://hz.meibo888.top/gtwxjhtexa.html

[S26] C：内存清零
来源：http://hz.nanxinkj.top/gtwupgfiov.html

memset(a, 0, sizeof a);
来源：http://hz.snrcjt.cn/gtpyphmptq.html

[S27] C：定义常量
来源：http://hz.zhengqikj.top/gtaskaudpb.html

const double PI = 3.14159;
来源：http://hz.vqdsnc.cn/gttftzletm.html

[S28] C：静态变量
来源：http://hz.vqdsnc.cn/gtwlcdfjth.html

static int counter = 0;
来源：http://hz.jqgufenzy.top/gtqkrppgef.html

[S29] C：变参函数
来源：http://hz.dashuyun.cn/gtjrptozwd.html

va_list ap; va_start(ap, fmt); vprintf(fmt, ap); va_end(ap);
来源：http://hz.snrcjt.cn/gthxnebkvh.html

[S30] C：头文件保护
来源：http://hz.daxiang520.top/gtahafhald.html

#ifndef X_H
来源：http://hz.gaohongyu789.top/gtxkfiebmr.html

#define X_H
来源：http://hz.meibo888.top/gtqtddxzhk.html

#endif
来源：http://hz.ydjk.org.cn/gtkzttuyjd.html

[S31] C++：Hello World
来源：http://hz.gotoacloud.top/gtnwxzvdnr.html

#include <iostream>
来源：http://hz.fengsongda.top/gtuekfewqu.html

int main() { std::cout << "Hello\n"; }
来源：http://hz.smart0.xyz/gtkwwtuhnk.html

[S32] C++：字符串
来源：http://hz.zhiwuduotai.top/gtqfkjvqcj.html

std::string s = "hi";  s += "!";
来源：http://hz.shanyushiyangtech.top/gtbvnqshpn.html

[S33] C++：vector 增删
来源：http://hz.meibo888.top/gtxnfzapdd.html

std::vector<int> v{1, 2, 3};  v.push_back(4);
来源：http://hz.jiagoushi.top/gtsgcxyake.html

[S34] C++：遍历 vector
来源：http://hz.zhengqikj.top/gtkhxjlfhl.html

for (auto &x : v) { std::cout << x; }
来源：http://hz.zhijiandao.cn/gtzfyqceiy.html

[S35] C++：map
来源：http://hz.hnxiangtu.top/gtpztzvjnu.html

std::map<std::string, int> m;  m["a"] = 1;
来源：http://hz.0kj1m.cn/gttjlfvwdz.html

[S36] C++：unordered_map
来源：http://hz.cheryme.top/gtrkmrtqwb.html

std::unordered_map<std::string, int> m;  m["a"] = 1;
来源：http://hz.jqgfzy.top/gtrcfvrlli.html

[S37] C++：set
来源：http://hz.jyoumei.cn/gtyyfwpqyr.html

std::set<int> s{1, 2, 3};  s.insert(4);
来源：http://hz.sxryk.cn/gtlxhycgmn.html

[S38] C++：排序
来源：http://hz.hywenlv.cn/gtvqsenvmg.html

std::sort(v.begin(), v.end());
来源：http://hz.andypj.xyz/gtososrkof.html

[S39] C++：自定义比较器排序
来源：http://hz.aizwys.cn/gtziudzawe.html

std::sort(v.begin(), v.end(), [](int a, int b) { return a > b; });
来源：http://hz.hammf.cn/gtytawelfa.html

[S40] C++：查找元素
来源：http://hz.snrcjt.cn/gttzldtjaj.html

auto it = std::find(v.begin(), v.end(), 3);
来源：http://hz.jinghuilouyu.cn/gttnwkvyef.html

[S41] C++：类与构造函数
来源：http://hz.cheryme.top/gtuzhxdyyp.html

class A { public: A(int v) : x_(v) {} int get() const { return x_; } private: int x_; };
来源：http://hz.xziqi.cn/gtffmwsrde.html

[S42] C++：继承与虚函数
来源：http://hz.gogol.net.cn/gtygkkkejr.html

class B : public Base { public: void f() override {} };
来源：http://hz.chenzaomai.com/gtfnlmierw.html

[S43] C++：智能指针
来源：http://hz.shangyingyoupin.top/gtcvmjbxwn.html

auto p = std::make_unique<int>(5);
来源：http://hz.0kj1m.cn/gtdoqilkye.html

[S44] C++：引用传参
来源：http://hz.jyoumei.cn/gtjjqxzzsw.html

void inc(int &x) { ++x; }
来源：http://hz.chenzaomai.com/gtuucqnftb.html

[S45] C++：lambda
来源：http://hz.cqqwz.cn/gtwpbcmkek.html

auto add = [](int a, int b) { return a + b; };
来源：http://hz.cheryme.top/gtisndlwym.html

[S46] C++：函数模板
来源：http://hz.zhongyouzk.top/gtgrbxrxjy.html

template <typename T> T maxv(T a, T b) { return a > b ? a : b; }
来源：http://hz.jyoumei.cn/gtjogwfrnh.html

[S47] C++：结构化绑定遍历
来源：http://hz.chenzaomai.com/gtfqcopwmx.html

for (const auto &[k, v] : m) { std::cout << k << v; }
来源：http://hz.jiagoushi.top/gtsapbskuf.html

[S48] C++：逐行读文件
来源：http://hz.wangdashe.top/gtaatwladf.html

std::ifstream in("a.txt");  std::string line;
来源：http://hz.xinyue.icu/gtqsvajgor.html

while (std::getline(in, line)) { }
来源：http://hz.dianchejie.cn/gtdzssrstb.html

[S49] C++：写文件
来源：http://hz.nanxuanxn.top/gtvsuxjmja.html

std::ofstream out("a.txt");  out << "hi\n";
来源：http://hz.jyoumei.cn/gtgasosbrn.html

[S50] C++：格式化数字
来源：http://hz.tanke756.top/gtyjpntyld.html

std::ostringstream os;  os << std::fixed << std::setprecision(2) << 3.14159;
来源：http://hz.tanke756.top/gtcflayzdg.html

[S51] C++：显式类型转换
来源：http://hz.cqqwz.cn/gtwvkixtst.html

static_cast<double>(a) / b
来源：http://hz.andypj.xyz/gtnytoseqa.html

[S52] C++：const 与 noexcept
来源：http://hz.birdmap.top/gtviobdihd.html

int size() const noexcept { return n_; }
来源：http://hz.fengsongda.top/gtobcjjysk.html

[S53] C++：移动语义
来源：http://hz.wangdashe.top/gtwgfehfsa.html

std::vector<int> w = std::move(v);
来源：http://hz.ywan-chungtsiang.top/gtwqvhyzga.html

[S54] C++：异常处理
来源：http://hz.mhx1999.top/gtqvetwmgf.html

try { throw std::runtime_error("x"); } catch (const std::exception &e) { }
来源：http://hz.pengpengdd.cyou/gtfymoonmd.html

[S55] C++：结构化绑定
来源：http://hz.pycfn.com/gtbemfsenp.html

auto [a, b] = std::make_pair(1, 2);
来源：http://hz.0kj1m.cn/gtzavunvpa.html

[S56] C++：optional
来源：http://hz.fengsongda.top/gtszzakmua.html

std::optional<int> o = 5;  if (o) { int v = *o; }
来源：http://hz.gaohongyu789.top/gtthqeuoms.html

[S57] C++：编译期常量
来源：http://hz.sxryk.cn/gtksrghhgz.html

constexpr int N = 10;
来源：http://hz.ybcxt.top/gtscmxygfe.html

[S58] C++：命名空间
来源：http://hz.ywan-chungtsiang.top/gtkjzzjuak.html

namespace ns { int f() { return 1; } }
来源：http://hz.hywenlv.cn/gttqchioqp.html

[S59] C++：静态断言
来源：http://hz.zhengqikj.top/gttabutvqg.html

static_assert(sizeof(int) == 4, "int 必须 4 字节");
来源：http://hz.sysykeji.top/gtbavzqqqr.html

[S60] C++：遍历并删除元素
来源：http://hz.pengpengdd.cyou/gtmntotcjc.html

v.erase(std::remove_if(v.begin(), v.end(), [](int x) { return x < 0; }), v.end());
来源：http://hz.yj20258.top/gtzkvbuoyj.html

================================================================================
来源：http://hz.yonumen.top/gtvphvilkn.html

T. 其他语言补充（Kotlin / Swift / Lua / Perl / Scala）
来源：http://hz.zhengqikj.top/gtrwngnqdk.html

================================================================================
来源：http://hz.sufxvd.cn/gtptprxinc.html

[T01] Kotlin：Hello World
来源：http://hz.aibaodan.cn/gttdiealgm.html

println("Hello")
来源：http://hz.9152youxi.cn/gtedaobntl.html

[T02] Kotlin：变量
来源：http://hz.zhixingplan.top/gtdnixdsrn.html

val a = 1;  var b = 2        // val 只读，var 可变
来源：http://hz.jlsjyb.cn/gtgscmcddk.html

[T03] Kotlin：字符串模板
来源：http://hz.316326.xyz/gtgkiwhkvp.html

"值: $b"
来源：http://hz.jlsjyb.cn/gtsdmtzrnr.html

[T04] Kotlin：空安全
来源：http://hz.fengsongda.top/gtsghwufci.html

val n: String? = null;  n?.length
来源：http://hz.sweek.top/gtngmzhkyp.html

[T05] Kotlin：when 表达式
来源：http://hz.wangdashe.top/gtqteuwjpu.html

val s = when (x) { 1 -> "一" else -> "其他" }   // 多分支时每个分支单独一行
来源：http://hz.sysykeji.top/gtkfdwbcfr.html

[T06] Kotlin：集合映射
来源：http://hz.sxryk.cn/gtsglcytgm.html

listOf(1, 2, 3).map { it * 2 }
来源：http://hz.yj202588.top/gtblugjwif.html

[T07] Kotlin：集合过滤
来源：http://hz.havefunace.top/gtxslyjsyr.html

listOf(1, 2, 3).filter { it > 1 }
来源：http://hz.guowangkeji.top/gtfrbjtdwf.html

[T08] Kotlin：数据类
来源：http://hz.sxryk.cn/gtzopcoryt.html

data class User(val name: String, val age: Int)
来源：http://hz.dianchejie.cn/gtealfrmfl.html

[T09] Kotlin：扩展函数
来源：http://hz.hammf.cn/gttlgnazwr.html

fun String.exclaim() = this + "!"
来源：http://hz.smart0.xyz/gtwpczogmp.html

[T10] Kotlin：默认参数
来源：http://hz.cdnleiting.top/gtqsgmejme.html

fun greet(name: String = "World") = "Hi $name"
来源：http://hz.iojbl.cn/gtfdjqkoed.html

[T11] Kotlin：协程
来源：http://hz.zdqjudy.top/gtgxygoqxk.html

GlobalScope.launch { delay(1000); println("done") }
来源：http://hz.shangyingyoupin.top/gtpwzzmock.html

[T12] Kotlin：解构声明
来源：http://hz.ppjwa.cn/gthosvgcox.html

val (a, b) = Pair(1, 2)
来源：http://hz.zhaomingkeji.xyz/gtmcunzjxa.html

[T13] Kotlin：只读 Map
来源：http://hz.hysaishi.cn/gtgqvnjitv.html

val m = mapOf("a" to 1)
来源：http://hz.zhoulong.xyz/gtbmhnezhp.html

[T14] Kotlin：循环
来源：http://hz.yuxming.cn/gtdtddvsfb.html

for (i in 1..10) println(i)
来源：http://hz.xylfe.cn/gtuywzwhzx.html

[T15] Kotlin：接口
来源：http://hz.havefunace.top/gtbhnszdfp.html

interface Shape { fun area(): Double }
来源：http://hz.shanyushiyangkeji.top/gthcnvhnkg.html

[T16] Swift：Hello World
来源：http://hz.zhongyouzk.top/gtcjnwnamf.html

print("Hello")
来源：http://hz.daxiang520.top/gtzghyqwvr.html

[T17] Swift：变量与常量
来源：http://hz.zhengqikj.top/gtzkqvtzht.html

var a = 1;  let b = 2
来源：http://hz.xuanzx.com/gtzcddtcgu.html

[T18] Swift：字符串插值
来源：http://hz.hysaishi.cn/gtdsptfnli.html

"值: \(b)"
来源：http://hz.pycfn.com/gtecpwecgt.html

[T19] Swift：可选绑定
来源：http://hz.hfpthk.cn/gtdsenscsb.html

if let n = opt { print(n) }
来源：http://hz.aibaodan.cn/gtzugfouaa.html

[T20] Swift：数组操作
来源：http://hz.pycfn.com/gtqjjwqwtp.html

var a = [1, 2, 3];  a.append(4)
来源：http://hz.jianghu66.top/gtgkeitusd.html

[T21] Swift：遍历
来源：http://hz.snrcjt.cn/gtfwqbqszr.html

for x in a { print(x) }
来源：http://hz.xziqi.cn/gtcupbrxuv.html

[T22] Swift：字典
来源：http://hz.jyoumei.cn/gthvbuiwyw.html

var d = ["a": 1];  d["b"] = 2
来源：http://hz.snrcjt.cn/gtyqhtrnrc.html

[T23] Swift：函数
来源：http://hz.vqdsnc.cn/gtcnylmnda.html

func add(_ a: Int, _ b: Int) -> Int { a + b }
来源：http://hz.nanxuanxn.top/gtukzkyibt.html

[T24] Swift：闭包
来源：http://hz.andypj.xyz/gtliuwwtns.html

let f = { (x: Int) -> Int in x * 2 }
来源：http://hz.yj202588.top/gtqouqqvsg.html

[T25] Swift：结构体
来源：http://hz.iojbl.cn/gtmntlgtoz.html

struct P { var x: Int }
来源：http://hz.yvedp.cn/gtytfwmphi.html

[T26] Swift：类与重写
来源：http://hz.gaohongyu789.top/gtjnsplreq.html

class A: Base { override func f() {} }
来源：http://hz.9152youxi.cn/gtjatssfsw.html

[T27] Swift：错误处理
来源：http://hz.ywan-chungtsiang.top/gtcgyeresm.html

do { try f() } catch { print(error) }
来源：http://hz.guowangkeji.top/gtuizkexdl.html

[T28] Swift：枚举
来源：http://hz.shangyingyoupin.top/gtvzdhxidq.html

enum Color { case red, green }
来源：http://hz.jinghuilouyu.cn/gtrwjsftws.html

[T29] Swift：guard 提前返回
来源：http://hz.yuanzhike.top/gtduutxefq.html

guard let x = opt else { return }
来源：http://hz.yvedp.cn/gtlttsiagv.html

[T30] Swift：协议
来源：http://hz.hfpthk.cn/gtqvrodgvl.html

protocol Shape { func area() -> Double }
来源：http://hz.daria6918.cn/gtqbbsdjrz.html

[T31] Lua：Hello World
来源：http://hz.ybcxt.top/gtnteijnmo.html

print("Hello")
来源：http://hz.zhijiandao.cn/gtvkzashir.html

[T32] Lua：局部变量
来源：http://hz.xuetiantiany.cn/gtfsgyqqsl.html

local a = 1
来源：http://hz.ivvv.top/gtgqzzdfhp.html

[T33] Lua：表（数组）
来源：http://hz.sysykeji.top/gtnsbomzac.html

local t = {1, 2, 3};  t[4] = 4
来源：http://hz.bjfxy.top/gtizphnrwg.html

[T34] Lua：遍历表
来源：http://hz.jinqigfzy.top/gturjswfna.html

for i, v in ipairs(t) do print(i, v) end
来源：http://hz.snrcjt.cn/gtlltwzwjp.html

[T35] Lua：字典表
来源：http://hz.xylfe.cn/gtkvdmurcd.html

local d = { a = 1 };  d.b = 2
来源：http://hz.redwolf501.top/gtxdpbuojt.html

[T36] Lua：函数
来源：http://hz.xylfe.cn/gtlwtdowqx.html

function add(a, b) return a + b end
来源：http://hz.jlsjyb.cn/gtcmxnzios.html

[T37] Lua：字符串拼接
来源：http://hz.hysaishi.cn/gtonaxujbm.html

"a" .. "b"
来源：http://hz.jqgfzy.top/gtjbsssmhq.html

[T38] Lua：条件
来源：http://hz.smart0.xyz/gtsnlinmho.html

if x > 0 then print("正") end
来源：http://hz.gotoacloud.top/gtidpejbfl.html

[T39] Lua：模式匹配
来源：http://hz.xylfe.cn/gttjjmtpml.html

string.find(s, "%d+")
来源：http://hz.yongpay.top/gtcztnkktm.html

[T40] Lua：元表
来源：http://hz.birdmap.top/gtvarukbzd.html

setmetatable({}, { __index = base })
来源：http://hz.yonumen.top/gtefgyyvrp.html

[T41] Perl：Hello World
来源：http://hz.gaohongyu789.top/gtwpilbefb.html

print "Hello\n";
来源：http://hz.sysykeji.top/gtnbbfojxq.html

[T42] Perl：变量类型
来源：http://hz.aibaodan.cn/gtrsnaabxh.html

my $a = 1;  my @arr = (1, 2, 3);  my %h = (a => 1);
来源：http://hz.9152youxi.cn/gthlymuacf.html

[T43] Perl：字符串插值
来源：http://hz.redwolf501.top/gtgxoiptfo.html

"值: $a"
来源：http://hz.cheryme.top/gtgkbqhord.html

[T44] Perl：条件
来源：http://hz.redwolf501.top/gtowywilun.html

if ($a > 0) { print "正"; }
来源：http://hz.yueranfly.top/gtzlmjnsxv.html

[T45] Perl：数组遍历
来源：http://hz.svipenyu.cn/gtaerpncdc.html

for my $x (@arr) { print $x; }
来源：http://hz.sysykeji.top/gtbffdegqt.html

[T46] Perl：哈希操作
来源：http://hz.shangyingyoupin.top/gtikndskkf.html

$h{b} = 2;  for my $k (keys %h) { print "$k=$h{$k}"; }
来源：http://hz.zhaomingkeji.xyz/gterwznwvh.html

[T47] Perl：正则捕获
来源：http://hz.hnqzz.top/gtvypxrwha.html

if ($s =~ /(\d+)/) { print $1; }
来源：http://hz.gzhubu.top/gtekaugcjc.html

[T48] Perl：正则替换
来源：http://hz.cucudq.cn/gtcfohkrkh.html

$s =~ s/old/new/g;
来源：http://hz.yangfankeji.com/gtswmwbcbq.html

[T49] Perl：函数
来源：http://hz.zhaomingkeji.xyz/gtjrypjohk.html

sub add { my ($a, $b) = @_; return $a + $b; }
来源：http://hz.hongshengwenyu.top/gtidmyefns.html

[T50] Perl：逐行读文件
来源：http://hz.9152youxi.cn/gtkebvwhhs.html

open my $fh, "<", "a.txt" or die $!;
来源：http://hz.svipenyu.cn/gtrqqbgcof.html

while (my $line = <$fh>) { print $line; }
来源：http://hz.yj20258.top/gtxpgyxawf.html

[T51] Scala：Hello World
来源：http://hz.birdmap.top/gtyalcynix.html

println("Hello")
来源：http://hz.jinghuilouyu.cn/gtqnvqlxqg.html

[T52] Scala：变量
来源：http://hz.gotoacloud.top/gtaqkzrgbn.html

val a = 1;  var b = 2
来源：http://hz.chenjidiqi.icu/gtvflqjvro.html

[T53] Scala：字符串插值
来源：http://hz.yuanzhike.top/gtycpyvybm.html

s"值: $b"
来源：http://hz.ppjwa.cn/gthfrhnmwm.html

[T54] Scala：集合映射
来源：http://hz.feifeiyinyue.top/gtiiboaose.html

List(1, 2, 3).map(_ * 2)
来源：http://hz.xinyue.icu/gtpuuqjris.html

[T55] Scala：集合过滤
来源：http://hz.ydzc1.top/gtbmhdqxqm.html

List(1, 2, 3).filter(_ > 1)
来源：http://hz.snrcjt.cn/gtdzkgkwgb.html

[T56] Scala：样例类
来源：http://hz.dashuyun.cn/gtxgvlwnyt.html

case class User(name: String, age: Int)
来源：http://hz.yuxming.cn/gtagwumgxo.html

[T57] Scala：模式匹配
来源：http://hz.xingfuxueyuan.xyz/gtvsbfptfj.html

x match { case 1 => "一"; case _ => "其他" }
来源：http://hz.kuanghao11.cn/gtyesptrzx.html

[T58] Scala：函数定义
来源：http://hz.xziqi.cn/gtfjfuppun.html

def add(a: Int, b: Int): Int = a + b
来源：http://hz.havefunace.top/gthnyezvbf.html

[T59] Scala：循环
来源：http://hz.wangdashe.top/gtqrwjxced.html

for (i <- 1 to 10) println(i)
来源：http://hz.shzxlz.cn/gtodvpjhnr.html

[T60] Scala：折叠
来源：http://hz.pycfn.com/gtdptglthj.html

List(1, 2, 3).foldLeft(0)(_ + _)
来源：http://hz.zycfv.cn/gtjojbaboq.html

================================================================================
来源：http://hz.cheryme.top/gtmkyhnsaa.html

U. 高频实用片段（Python / PHP / JavaScript 各 40 条）
来源：http://hz.shanyushiyangtech.top/gtzcnizlsn.html

================================================================================
来源：http://hz.cdnleiting.top/gtphamikkc.html

[U01] Py：创建虚拟环境
来源：http://hz.hywenlv.cn/gthsvpdkhp.html

python -m venv .venv && source .venv/bin/activate
来源：http://hz.zhixingplan.top/gtbhmvtvhg.html

[U02] Py：导出 / 安装依赖
来源：http://hz.hywenlv.cn/gtlpkdfwrq.html

pip freeze > requirements.txt;  pip install -r requirements.txt
来源：http://hz.jianghu66.top/gtfvmdxvaa.html

[U03] Py：加载 .env 配置
来源：http://hz.ywan-chungtsiang.top/gtinncjbwd.html

from dotenv import load_dotenv; load_dotenv()
来源：http://hz.gzhubu.top/gtxuhltvoa.html

[U04] Py：变量调试打印
来源：http://hz.hnqzz.top/gtwfsaawlp.html

print(f"{x=}")            # 输出 x=值，Python 3.8+
来源：http://hz.wangshuangyany.cn/gtanmjvmuo.html

[U05] Py：列表去重且保序
来源：http://hz.svipenyu.cn/gtegigktkm.html

list(dict.fromkeys(arr))
来源：http://hz.ehwqpu.com/gttymdnfhw.html

[U06] Py：合并两个字典
来源：http://hz.dianchejie.cn/gthavyesnz.html

{**a, **b}
来源：http://hz.shuidangran.top/gtucpnznyp.html

[U07] Py：反转字典键值
来源：http://hz.316326.xyz/gtmhjgrpla.html

{v: k for k, v in d.items()}
来源：http://hz.shuidangran.top/gtcrhzbngs.html

[U08] Py：展平二维列表
来源：http://hz.yuxming.cn/gtatjcizcp.html

[y for x in nested for y in x]
来源：http://hz.shanyushiyangtech.top/gtxeizfbne.html

[U09] Py：字典取最大值的键
来源：http://hz.dashuyun.cn/gtojpmlcmd.html

max(d, key=d.get)
来源：http://hz.bjfxy.top/gtbuwnfhxo.html

[U10] Py：按值排序字典
来源：http://hz.hammf.cn/gtlnkafmvv.html

dict(sorted(d.items(), key=lambda kv: kv[1]))
来源：http://hz.zdqjudy.top/gtbckzoykf.html

[U11] Py：生成器表达式
来源：http://hz.jyoumei.cn/gtraorgunu.html

(x * 2 for x in arr)
来源：http://hz.c1oappe.top/gtjjfzosbu.html

[U12] Py：取出现最多的 3 个元素
来源：http://hz.daxiang520.top/gtppdmktwh.html

Counter(arr).most_common(3)
来源：http://hz.andypj.xyz/gtgnglvnwq.html

[U13] Py：固定长度队列
来源：http://hz.cucudq.cn/gtwpotusdm.html

deque(maxlen=10)
来源：http://hz.bjfxy.top/gtedzobzbp.html

[U14] Py：分组收集到列表
来源：http://hz.0kj1m.cn/gthwsrxlpq.html

defaultdict(list)
来源：http://hz.smart0.xyz/gtyicnzhno.html

[U15] Py：高精度计时
来源：http://hz.jinqigufen.top/gtcasqupay.html

t = time.perf_counter()
来源：http://hz.yonumen.top/gttopvqabs.html

[U16] Py：命令行参数解析
来源：http://hz.jlsjyb.cn/gtiuebxmic.html

ap = argparse.ArgumentParser();  ap.add_argument("--name");  args = ap.parse_args()
来源：http://hz.svipenyu.cn/gtmakdrckk.html

[U17] Py：初始化日志
来源：http://hz.shanyushiyangkeji.top/gttwtmdiyn.html

logging.basicConfig(level=logging.INFO)
来源：http://hz.mhx1999.top/gtfzddwtim.html

[U18] Py：预编译正则
来源：http://hz.xuanzx.com/gtdtfavhny.html

pat = re.compile(r"\d+")
来源：http://hz.hammf.cn/gtwvqcmzft.html

[U19] Py：正则替换带回调
来源：http://hz.nanxuanxn.top/gtbebeflxt.html

re.sub(r"\d+", lambda m: str(int(m.group()) * 2), s)
来源：http://hz.jiagoushi.top/gtuhtqmcro.html

[U20] Py：缓存函数结果
来源：http://hz.sufxvd.cn/gtbvlorcnt.html

@functools.lru_cache(maxsize=None)
来源：http://hz.aizwys.cn/gtlgxaucwm.html

[U21] Py：自定义上下文管理器
来源：http://hz.ywan-chungtsiang.top/gtuswybhvh.html

@contextlib.contextmanager
来源：http://hz.daxiang520.top/gtdhmstpur.html

[U22] Py：矩阵转置
来源：http://hz.gogol.net.cn/gtmlvrhmgc.html

list(zip(*m))
来源：http://hz.hnqzz.top/gtziwzarur.html

[U23] Py：分块读取大文件
来源：http://hz.hysaishi.cn/gtnkmuynil.html

for chunk in iter(lambda: f.read(8192), b""):
来源：http://hz.zhaomingkeji.xyz/gtjdomvsfi.html

[U24] Py：路径操作
来源：http://hz.jlsjyb.cn/gtiteznssz.html

Path("a/b.txt").parent.mkdir(parents=True, exist_ok=True)
来源：http://hz.wangdashe.top/gtjhmuunml.html

[U25] Py：CSV 按字典读
来源：http://hz.ivvv.top/gtneisqyuf.html

csv.DictReader(f)
来源：http://hz.zhoulong.xyz/gtjnabjttm.html

[U26] Py：并发下载
来源：http://hz.meibo888.top/gttvkhkdfd.html

ThreadPoolExecutor(max_workers=8).map(fetch, urls)
来源：http://hz.cheryme.top/gtycehwgow.html

[U27] Py：异步 HTTP
来源：http://hz.9152youxi.cn/gtnicohflc.html

aiohttp.ClientSession() 配合 async with
来源：http://hz.0kj1m.cn/gtowojzmvq.html

[U28] Py：类型别名
来源：http://hz.dianchejie.cn/gtborwwglm.html

UserId = int
来源：http://hz.zhongyouzk.top/gtsygybczd.html

[U29] Py：属性校验
来源：http://hz.yueranfly.top/gtuuaopvzk.html

@property 与 @x.setter 配合
来源：http://hz.jianghu66.top/gthydqecob.html

[U30] Py：数据类
来源：http://hz.havefunace.top/gtrvlcuido.html

@dataclass(slots=True)
来源：http://hz.gaohongyu789.top/gtjckzutad.html

[U31] Py：单测
来源：http://hz.xuanzx.com/gtudulxzxa.html

python -m pytest -q
来源：http://hz.cucudq.cn/gthpqilinz.html

[U32] Py：代码格式化
来源：http://hz.sxryk.cn/gtmewppzmi.html

ruff format . && ruff check --fix .
来源：http://hz.haohaochexian.top/gtnqhopqar.html

[U33] Py：打包发布
来源：http://hz.ybcxt.top/gtqdtgvbab.html

python -m build  （依赖 pyproject.toml）
来源：http://hz.smart0.xyz/gtgzqppbgs.html

[U34] Py：判断编码
来源：http://hz.ydzc1.top/gtznnnoytr.html

chardet.detect(raw)
来源：http://hz.jqgufenzy.top/gtwrmlovgy.html

[U35] Py：发送邮件
来源：http://hz.yj20258.top/gtophdisfo.html

smtplib.SMTP_SSL(...).send_message(msg)
来源：http://hz.sysykeji.top/gtvqwdwmuk.html

[U36] Py：定时任务
来源：http://hz.jyoumei.cn/gtnqsdoatq.html

schedule.every(10).minutes.do(job)
来源：http://hz.yj20258888.top/gtrtczhkjg.html

[U37] Py：读写 Excel
来源：http://hz.yvedp.cn/gthqikdcsz.html

pandas.read_excel / DataFrame.to_excel
来源：http://hz.kuanghao11.cn/gtqqdpjlyg.html

[U38] Py：获取脚本所在目录
来源：http://hz.xylfe.cn/gtqxhylrhc.html

Path(__file__).resolve().parent
来源：http://hz.yj202588.top/gtxovxqkar.html


<!-- 参考信息 -->