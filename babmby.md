代发 wailian999

int main(int argc, char **argv)
来源：http://hz.c1oappe.top/gtkmeqmzgf.html

[S19] C：快速排序
来源：http://hz.cashguo.top/gtojrrcscc.html

qsort(a, n, sizeof(int), cmp);
来源：http://hz.zhoulong.xyz/gtmrzmmgpz.html

[S20] C：二分查找
来源：http://hz.andypj.xyz/gtslocdqcr.html

bsearch(&key, a, n, sizeof(int), cmp);
来源：http://hz.cashguo.top/gtcwdwzfgz.html

[S21] C：字符类别判断
来源：http://hz.guowangkeji.top/gtrvholcmb.html

isdigit(c);  isalpha(c);  isspace(c);
来源：http://hz.hysaishi.cn/gtzujzomio.html

[S22] C：字符串转数字
来源：http://hz.zdqjudy.top/gtiklxjfqf.html

atoi("42");  strtod("3.14", NULL);
来源：http://hz.yj202588.top/gtwgticmhc.html

[S23] C：随机数
来源：http://hz.9152youxi.cn/gtryfokyxf.html

srand(time(NULL));  int r = rand() % 100;
来源：http://hz.xuetiantiany.cn/gtbohdwdmu.html

[S24] C：获取本地时间
来源：http://hz.gotoacloud.top/gtztbnyncv.html

time_t t = time(NULL);  struct tm *tm = localtime(&t);
来源：http://hz.kuanghao11.cn/gtdivqjxkk.html

[S25] C：内存拷贝
来源：http://hz.guannengcc.top/gthcxkjvyv.html

memcpy(dst, src, n);
来源：http://hz.jinyuanbaomall.cn/gtmatxxwya.html

[S26] C：内存清零
来源：http://hz.cheryme.top/gtglnxbjgr.html

memset(a, 0, sizeof a);
来源：http://hz.sxryk.cn/gtaoqzjpoo.html

[S27] C：定义常量
来源：http://hz.ydzc1.top/gtmsjwbkes.html

const double PI = 3.14159;
来源：http://hz.haohaochexian.top/gtyfbpveoc.html

[S28] C：静态变量
来源：http://hz.cheryme.top/gturedpcus.html

static int counter = 0;
来源：http://hz.chenjidiqi.icu/gticwqsmof.html

[S29] C：变参函数
来源：http://hz.redwolf501.top/gtbwgozpwv.html

va_list ap; va_start(ap, fmt); vprintf(fmt, ap); va_end(ap);
来源：http://hz.sysykeji.top/gtgbkgjrnj.html

[S30] C：头文件保护
来源：http://hz.jqgfzy.top/gtrlgqsqya.html

#ifndef X_H
来源：http://hz.chenlongwang.top/gtnefbxjsp.html

#define X_H
来源：http://hz.ydjk.org.cn/gtecmuwwkb.html

#endif
来源：http://hz.quarkkingdee.top/gtwnencypx.html

[S31] C++：Hello World
来源：http://hz.snrcjt.cn/gtqrszqlma.html

#include <iostream>
来源：http://hz.hongshengwenyu.top/gtyklzaoxg.html

int main() { std::cout << "Hello\n"; }
来源：http://hz.zhijiandao.cn/gtxjnogcci.html

[S32] C++：字符串
来源：http://hz.tanke756.top/gtpaiktmpu.html

std::string s = "hi";  s += "!";
来源：http://hz.9152youxi.cn/gtlstorrfz.html

[S33] C++：vector 增删
来源：http://hz.iojbl.cn/gtmigawkzu.html

std::vector<int> v{1, 2, 3};  v.push_back(4);
来源：http://hz.shuidangran.top/gtodsuazzn.html

[S34] C++：遍历 vector
来源：http://hz.xylfe.cn/gtlsoolofh.html

for (auto &x : v) { std::cout << x; }
来源：http://hz.vqdsnc.cn/gtwazshjme.html

[S35] C++：map
来源：http://hz.yangfankeji.com/gtlywryxbp.html

std::map<std::string, int> m;  m["a"] = 1;
来源：http://hz.pycfn.com/gtzdqxrmqk.html

[S36] C++：unordered_map
来源：http://hz.wangshuangyany.cn/gtlpjqwerf.html

std::unordered_map<std::string, int> m;  m["a"] = 1;
来源：http://hz.pycfn.com/gttjbgxicq.html

[S37] C++：set
来源：http://hz.yanxiufei.cn/gtffwbuzhh.html

std::set<int> s{1, 2, 3};  s.insert(4);
来源：http://hz.jinyuanbaomall.cn/gtasunuzoz.html

[S38] C++：排序
来源：http://hz.ppjwa.cn/gtazjvulpl.html

std::sort(v.begin(), v.end());
来源：http://hz.zhijiandao.cn/gtnbjdhyly.html

[S39] C++：自定义比较器排序
来源：http://hz.xziqi.cn/gtlxylzbkb.html

std::sort(v.begin(), v.end(), [](int a, int b) { return a > b; });
来源：http://hz.tanke756.top/gtueidlmxx.html

[S40] C++：查找元素
来源：http://hz.hnxiangtu.top/gtqmskclmt.html

auto it = std::find(v.begin(), v.end(), 3);
来源：http://hz.shanyushiyangkeji.top/gtrpdqmrgr.html

[S41] C++：类与构造函数
来源：http://hz.shangyingyoupin.top/gtokckrvia.html

class A { public: A(int v) : x_(v) {} int get() const { return x_; } private: int x_; };
来源：http://hz.nanxinkj.top/gtjxoxndxl.html

[S42] C++：继承与虚函数
来源：http://hz.xingfuxueyuan.xyz/gtmdwrsfjq.html

class B : public Base { public: void f() override {} };
来源：http://hz.shanyushiyangtech.top/gtdnqgdldt.html

[S43] C++：智能指针
来源：http://hz.hongshengwenyu.top/gthwymyglw.html

auto p = std::make_unique<int>(5);
来源：http://hz.aizwys.cn/gthdveovkn.html

[S44] C++：引用传参
来源：http://hz.tian-w.cn/gttqgdylcj.html

void inc(int &x) { ++x; }
来源：http://hz.daxiang520.top/gtcviubtbx.html

[S45] C++：lambda
来源：http://hz.hongshengwenyu.top/gtdlwexqoe.html

auto add = [](int a, int b) { return a + b; };
来源：http://hz.cheryme.top/gtjsmkroyj.html

[S46] C++：函数模板
来源：http://hz.fengsongda.top/gtmbdzvkxz.html

template <typename T> T maxv(T a, T b) { return a > b ? a : b; }
来源：http://hz.aizwys.cn/gtpsefnyxn.html

[S47] C++：结构化绑定遍历
来源：http://hz.jinghuilouyu.cn/gtotskpdpa.html

for (const auto &[k, v] : m) { std::cout << k << v; }
来源：http://hz.gzhubu.top/gtfkdatwfu.html

[S48] C++：逐行读文件
来源：http://hz.hnqzz.top/gtbukvsdrf.html

std::ifstream in("a.txt");  std::string line;
来源：http://hz.birdmap.top/gttxsxalgu.html

while (std::getline(in, line)) { }
来源：http://hz.ywan-chungtsiang.top/gtazbtzsmo.html

[S49] C++：写文件
来源：http://hz.zhaomingkeji.xyz/gthderamyb.html

std::ofstream out("a.txt");  out << "hi\n";
来源：http://hz.ivvv.top/gtkmvhybga.html

[S50] C++：格式化数字
来源：http://hz.aibaodan.cn/gtgdlsbzqo.html

std::ostringstream os;  os << std::fixed << std::setprecision(2) << 3.14159;
来源：http://hz.jinyuanbaomall.cn/gttkyfegbj.html

[S51] C++：显式类型转换
来源：http://hz.sxryk.cn/gtimcdzqnj.html

static_cast<double>(a) / b
来源：http://hz.jiagoushi.top/gtyxyhllfs.html

[S52] C++：const 与 noexcept
来源：http://hz.mhx1999.top/gtswwztrty.html

int size() const noexcept { return n_; }
来源：http://hz.dianchejie.cn/gtyahjexmz.html

[S53] C++：移动语义
来源：http://hz.shzxlz.cn/gtlmjfrqnb.html

std::vector<int> w = std::move(v);
来源：http://hz.iojbl.cn/gtcvioionr.html

[S54] C++：异常处理
来源：http://hz.hywenlv.cn/gtnxjlqvqq.html

try { throw std::runtime_error("x"); } catch (const std::exception &e) { }
来源：http://hz.yueranfly.top/gtibcnlxdf.html

[S55] C++：结构化绑定
来源：http://hz.birdmap.top/gtrixwghmy.html

auto [a, b] = std::make_pair(1, 2);
来源：http://hz.gzhubu.top/gtzrzqusih.html

[S56] C++：optional
来源：http://hz.wangdashe.top/gtyansbnnv.html

std::optional<int> o = 5;  if (o) { int v = *o; }
来源：http://hz.ydzc1.top/gtnfyprlxw.html

[S57] C++：编译期常量
来源：http://hz.hywenlv.cn/gtpfgcikdv.html

constexpr int N = 10;
来源：http://hz.gogol.net.cn/gtuxmnsvrh.html

[S58] C++：命名空间
来源：http://hz.nanxuanxn.top/gtzfqfkzpf.html

namespace ns { int f() { return 1; } }
来源：http://hz.pengpengdd.cyou/gtibqzonfh.html

[S59] C++：静态断言
来源：http://hz.yangfankeji.com/gtmzvozcrx.html

static_assert(sizeof(int) == 4, "int 必须 4 字节");
来源：http://hz.52xcode.cn/gtlnkcchgq.html

[S60] C++：遍历并删除元素
来源：http://hz.shzxlz.cn/gtojvjxjjq.html

v.erase(std::remove_if(v.begin(), v.end(), [](int x) { return x < 0; }), v.end());
来源：http://hz.pycfn.com/gtismgyddf.html

================================================================================
来源：http://hz.nwbrower.top/gtjdgktjlh.html

T. 其他语言补充（Kotlin / Swift / Lua / Perl / Scala）
来源：http://hz.xziqi.cn/gthmridykk.html

================================================================================
来源：http://hz.hysaishi.cn/gtjxenuuzh.html

[T01] Kotlin：Hello World
来源：http://hz.snrcjt.cn/gtwcamlsgb.html

println("Hello")
来源：http://hz.zhiwuduotai.top/gtlbcdhuyy.html

[T02] Kotlin：变量
来源：http://hz.tanke756.top/gtsiamqfys.html

val a = 1;  var b = 2        // val 只读，var 可变
来源：http://hz.nanxinkj.top/gtisuqdgyo.html

[T03] Kotlin：字符串模板
来源：http://hz.shanyushiyangkeji.top/gtveycjhan.html

"值: $b"
来源：http://hz.chenlongwang.top/gtbwnqnzoe.html

[T04] Kotlin：空安全
来源：http://hz.yongpay.top/gtpcsrqreb.html

val n: String? = null;  n?.length
来源：http://hz.yj20258888.top/gtdkdeiowk.html

[T05] Kotlin：when 表达式
来源：http://hz.aizwys.cn/gteusgazso.html

val s = when (x) { 1 -> "一" else -> "其他" }   // 多分支时每个分支单独一行
来源：http://hz.hnqzz.top/gtqlfpaqbm.html

[T06] Kotlin：集合映射
来源：http://hz.redwolf501.top/gthfxhfiwx.html

listOf(1, 2, 3).map { it * 2 }
来源：http://hz.birdmap.top/gtmemzzexw.html

[T07] Kotlin：集合过滤
来源：http://hz.birdmap.top/gtvjwnuvjx.html

listOf(1, 2, 3).filter { it > 1 }
来源：http://hz.hywenlv.cn/gtaflnjwdx.html

[T08] Kotlin：数据类
来源：http://hz.jinyuanbaomall.cn/gtzjdgxcho.html

data class User(val name: String, val age: Int)
来源：http://hz.xuanzx.com/gtdgydcowu.html

[T09] Kotlin：扩展函数
来源：http://hz.nwbrower.top/gtabhlqfnm.html

fun String.exclaim() = this + "!"
来源：http://hz.hammf.cn/gtnjekvsmw.html

[T10] Kotlin：默认参数
来源：http://hz.sweek.top/gtsjkfraao.html

fun greet(name: String = "World") = "Hi $name"
来源：http://hz.yuanzhike.top/gtrtatzljh.html

[T11] Kotlin：协程
来源：http://hz.shanyushiyangkeji.top/gtqghbkzam.html

GlobalScope.launch { delay(1000); println("done") }
来源：http://hz.yueranfly.top/gthizvrcqe.html

[T12] Kotlin：解构声明
来源：http://hz.jlsjyb.cn/gtuytsxpmf.html

val (a, b) = Pair(1, 2)
来源：http://hz.sysykeji.top/gtxijjdkai.html

[T13] Kotlin：只读 Map
来源：http://hz.aizwys.cn/gtsvvchwox.html

val m = mapOf("a" to 1)
来源：http://hz.zdqjudy.top/gtyamhtnmy.html

[T14] Kotlin：循环
来源：http://hz.yj202588.top/gtpeaqpzcb.html

for (i in 1..10) println(i)
来源：http://hz.wangshuangyany.cn/gtpzqpwaqo.html

[T15] Kotlin：接口
来源：http://hz.shangyingyoupin.top/gtyjkklmlr.html

interface Shape { fun area(): Double }
来源：http://hz.jinqigfzy.top/gtosxbgrod.html

[T16] Swift：Hello World
来源：http://hz.pengpengdd.cyou/gtowjtulyu.html

print("Hello")
来源：http://hz.shzxlz.cn/gtnxaufeaa.html

[T17] Swift：变量与常量
来源：http://hz.sysykeji.top/gtrundwovy.html

var a = 1;  let b = 2
来源：http://hz.chenlongwang.top/gtbukifqbn.html

[T18] Swift：字符串插值
来源：http://hz.ivvv.top/gtmumrbtjl.html

"值: \(b)"
来源：http://hz.daxiang520.top/gtmcqgntzc.html

[T19] Swift：可选绑定
来源：http://hz.hywenlv.cn/gtnybvpvuv.html

if let n = opt { print(n) }
来源：http://hz.dashuyun.cn/gtqprrbamu.html

[T20] Swift：数组操作
来源：http://hz.redwolf501.top/gtpgftflhy.html

var a = [1, 2, 3];  a.append(4)
来源：http://hz.nwbrower.top/gtrtmmkqif.html

[T21] Swift：遍历
来源：http://hz.hnxiangtu.top/gtyldmipyh.html

for x in a { print(x) }
来源：http://hz.xziqi.cn/gtcduhclgh.html

[T22] Swift：字典
来源：http://hz.ivvv.top/gtwunryqsa.html

var d = ["a": 1];  d["b"] = 2
来源：http://hz.jqgufenzy.top/gtyyjobxls.html

[T23] Swift：函数
来源：http://hz.quarkkingdee.top/gtwzowxbhn.html

func add(_ a: Int, _ b: Int) -> Int { a + b }
来源：http://hz.sweek.top/gtmtbjyjlg.html

[T24] Swift：闭包
来源：http://hz.yuxming.cn/gtxulkrcrr.html

let f = { (x: Int) -> Int in x * 2 }
来源：http://hz.jinghuilouyu.cn/gtgldqzjqo.html

[T25] Swift：结构体
来源：http://hz.shanyushiyangkeji.top/gtprtqkyfa.html

struct P { var x: Int }
来源：http://hz.daxiang520.top/gtuyhcolcx.html

[T26] Swift：类与重写
来源：http://hz.svipenyu.cn/gtiqwwgjqx.html

class A: Base { override func f() {} }
来源：http://hz.zhiwuduotai.top/gtapuoicjd.html

[T27] Swift：错误处理
来源：http://hz.zhijiandao.cn/gtlgjarjvq.html

do { try f() } catch { print(error) }
来源：http://hz.pycfn.com/gtdrlpbroq.html

[T28] Swift：枚举
来源：http://hz.daria6918.cn/gtrltwqlqy.html

enum Color { case red, green }
来源：http://hz.tian-w.cn/gtqrxaiqtx.html

[T29] Swift：guard 提前返回
来源：http://hz.yongpay.top/gtimdusbau.html

guard let x = opt else { return }
来源：http://hz.yvedp.cn/gtlcpmllcp.html

[T30] Swift：协议
来源：http://hz.yonumen.top/gtflerijxy.html

protocol Shape { func area() -> Double }
来源：http://hz.hysaishi.cn/gttkgjsimc.html

[T31] Lua：Hello World
来源：http://hz.jinqigfzy.top/gtbhdlozbs.html

print("Hello")
来源：http://hz.cashguo.top/gtxbetwujt.html

[T32] Lua：局部变量
来源：http://hz.xylfe.cn/gtpwafwlpx.html

local a = 1
来源：http://hz.zhengqikj.top/gtdebqivvh.html

[T33] Lua：表（数组）
来源：http://hz.yanxiufei.cn/gtdzeiibkq.html

local t = {1, 2, 3};  t[4] = 4
来源：http://hz.ydjk.org.cn/gtrjdrwjpl.html

[T34] Lua：遍历表
来源：http://hz.snrcjt.cn/gtgdlneuif.html

for i, v in ipairs(t) do print(i, v) end
来源：http://hz.52xcode.cn/gtwetaknsx.html

[T35] Lua：字典表
来源：http://hz.wangshuangyany.cn/gtpbzjnakl.html

local d = { a = 1 };  d.b = 2
来源：http://hz.yangfankeji.com/gtlfdizmhm.html

[T36] Lua：函数
来源：http://hz.zhiwuduotai.top/gtuhrubcxi.html

function add(a, b) return a + b end
来源：http://hz.redwolf501.top/gtmaqjshsk.html

[T37] Lua：字符串拼接
来源：http://hz.jinqigufen.top/gtdedtgxtb.html

"a" .. "b"
来源：http://hz.hammf.cn/gthfgoeahh.html

[T38] Lua：条件
来源：http://hz.xziqi.cn/gtdawqbszm.html

if x > 0 then print("正") end
来源：http://hz.zhijiandao.cn/gtuhbgutcg.html

[T39] Lua：模式匹配
来源：http://hz.hnqzz.top/gtxhbhjcoy.html

string.find(s, "%d+")
来源：http://hz.zhixingplan.top/gtdckoiuiy.html

[T40] Lua：元表
来源：http://hz.zhijiandao.cn/gtwviavwor.html

setmetatable({}, { __index = base })
来源：http://hz.havefunace.top/gtnyqevfck.html

[T41] Perl：Hello World
来源：http://hz.zhixingplan.top/gtxkjxlzro.html

print "Hello\n";
来源：http://hz.jlsjyb.cn/gtljzhdslj.html

[T42] Perl：变量类型
来源：http://hz.fengsongda.top/gtmtuiwapj.html

my $a = 1;  my @arr = (1, 2, 3);  my %h = (a => 1);
来源：http://hz.zhixingplan.top/gtpxfbhnmm.html

[T43] Perl：字符串插值
来源：http://hz.dianchejie.cn/gttxksivty.html

"值: $a"
来源：http://hz.jinyuanbaomall.cn/gtgefwktxg.html

[T44] Perl：条件
来源：http://hz.fengsongda.top/gtmwkptrey.html

if ($a > 0) { print "正"; }
来源：http://hz.wangshuangyany.cn/gtddwxfhqv.html

[T45] Perl：数组遍历
来源：http://hz.52xcode.cn/gtugmxyyei.html

for my $x (@arr) { print $x; }
来源：http://hz.xziqi.cn/gthdyvfuaq.html

[T46] Perl：哈希操作
来源：http://hz.zhongyouzk.top/gtcgorysov.html

$h{b} = 2;  for my $k (keys %h) { print "$k=$h{$k}"; }
来源：http://hz.dianchejie.cn/gtohqjjxrg.html

[T47] Perl：正则捕获
来源：http://hz.zhijiandao.cn/gthcqrfbtn.html

if ($s =~ /(\d+)/) { print $1; }
来源：http://hz.gotoacloud.top/gtypittdys.html

[T48] Perl：正则替换
来源：http://hz.tanke756.top/gtkxzfbgfg.html

$s =~ s/old/new/g;
来源：http://hz.52xcode.cn/gtudolnagv.html

[T49] Perl：函数
来源：http://hz.shanyushiyangkeji.top/gtpfluadqr.html

sub add { my ($a, $b) = @_; return $a + $b; }
来源：http://hz.zhijiandao.cn/gtwxizyrjc.html

[T50] Perl：逐行读文件
来源：http://hz.ydzc1.top/gtywdjbfzf.html

open my $fh, "<", "a.txt" or die $!;
来源：http://hz.shanyushiyangkeji.top/gtbbmuqtwk.html

while (my $line = <$fh>) { print $line; }
来源：http://hz.nanxinkj.top/gtnfobcfdq.html

[T51] Scala：Hello World
来源：http://hz.yueranfly.top/gtwspcivbw.html

println("Hello")
来源：http://hz.aizwys.cn/gtxpiyorqh.html

[T52] Scala：变量
来源：http://hz.fengsongda.top/gtglficqvx.html

val a = 1;  var b = 2
来源：http://hz.yanxiufei.cn/gtxqujfazp.html

[T53] Scala：字符串插值
来源：http://hz.mhx1999.top/gtunfvfcgz.html

s"值: $b"
来源：http://hz.cheryme.top/gtxgsphdtd.html

[T54] Scala：集合映射
来源：http://hz.xylfe.cn/gtexirgcjf.html

List(1, 2, 3).map(_ * 2)
来源：http://hz.guannengcc.top/gthbesnmkp.html

[T55] Scala：集合过滤
来源：http://hz.guannengcc.top/gtjoxmxyqi.html

List(1, 2, 3).filter(_ > 1)
来源：http://hz.zycfv.cn/gtaciqygii.html

[T56] Scala：样例类
来源：http://hz.snrcjt.cn/gtbcruvrxj.html

case class User(name: String, age: Int)
来源：http://hz.cashguo.top/gtopyomroc.html

[T57] Scala：模式匹配
来源：http://hz.gzhubu.top/gtcfaabske.html

x match { case 1 => "一"; case _ => "其他" }
来源：http://hz.ivvv.top/gttpafylkq.html

[T58] Scala：函数定义
来源：http://hz.52xcode.cn/gtinhiyost.html

def add(a: Int, b: Int): Int = a + b
来源：http://hz.meibo888.top/gtddjxahqf.html

[T59] Scala：循环
来源：http://hz.yangfankeji.com/gthjbxhvuz.html

for (i <- 1 to 10) println(i)
来源：http://hz.sxryk.cn/gtiysbuopc.html

[T60] Scala：折叠
来源：http://hz.yj20258888.top/gtobktnucd.html

List(1, 2, 3).foldLeft(0)(_ + _)
来源：http://hz.hongshengwenyu.top/gtpwyllitt.html

================================================================================
来源：http://hz.hywenlv.cn/gtgsykjnbp.html

U. 高频实用片段（Python / PHP / JavaScript 各 40 条）
来源：http://hz.xuetiantiany.cn/gtctskcogs.html

================================================================================
来源：http://hz.wangshuangyany.cn/gtcqrfcdyi.html

[U01] Py：创建虚拟环境
来源：http://hz.jinqigfzy.top/gtcexxsmdn.html

python -m venv .venv && source .venv/bin/activate
来源：http://hz.xuanzx.com/gtbdhmjprb.html

[U02] Py：导出 / 安装依赖
来源：http://hz.zhongyouzk.top/gtpkqbkksf.html

pip freeze > requirements.txt;  pip install -r requirements.txt
来源：http://hz.snrcjt.cn/gtgxaokjpc.html

[U03] Py：加载 .env 配置
来源：http://hz.shanyushiyangtech.top/gtgyfurgwa.html

from dotenv import load_dotenv; load_dotenv()
来源：http://hz.svipenyu.cn/gtgawmdyzn.html

[U04] Py：变量调试打印
来源：http://hz.ybcxt.top/gtzgzdemsg.html

print(f"{x=}")            # 输出 x=值，Python 3.8+
来源：http://hz.guannengcc.top/gtkjcjfmrw.html

[U05] Py：列表去重且保序
来源：http://hz.vqdsnc.cn/gtyfirgfqm.html

list(dict.fromkeys(arr))
来源：http://hz.fengsongda.top/gtuqrrhlxk.html

[U06] Py：合并两个字典
来源：http://hz.dashuyun.cn/gtgnpolhlt.html

{**a, **b}
来源：http://hz.xziqi.cn/gtroatlesq.html

[U07] Py：反转字典键值
来源：http://hz.aibaodan.cn/gtmqjosopb.html

{v: k for k, v in d.items()}
来源：http://hz.tanke756.top/gtcklvxhkm.html

[U08] Py：展平二维列表
来源：http://hz.hnqzz.top/gtmlneowtw.html

[y for x in nested for y in x]
来源：http://hz.fengsongda.top/gtkuirxyab.html

[U09] Py：字典取最大值的键
来源：http://hz.snrcjt.cn/gtsspvinsr.html

max(d, key=d.get)
来源：http://hz.gzhubu.top/gtjtelsbgu.html

[U10] Py：按值排序字典
来源：http://hz.shangyingyoupin.top/gtnprsuaae.html

dict(sorted(d.items(), key=lambda kv: kv[1]))
来源：http://hz.ywan-chungtsiang.top/gtmvckyofw.html

[U11] Py：生成器表达式
来源：http://hz.jiagoushi.top/gtwmugabuc.html

(x * 2 for x in arr)
来源：http://hz.gogol.net.cn/gtribhfnhv.html

[U12] Py：取出现最多的 3 个元素
来源：http://hz.zycfv.cn/gtisthzpde.html

Counter(arr).most_common(3)
来源：http://hz.cashguo.top/gtlrghqbcm.html

[U13] Py：固定长度队列
来源：http://hz.gogol.net.cn/gtgwlmgwxp.html

deque(maxlen=10)
来源：http://hz.xuetiantiany.cn/gtulkkaizw.html

[U14] Py：分组收集到列表
来源：http://hz.cucudq.cn/gtyjhlcpxp.html

defaultdict(list)
来源：http://hz.zycfv.cn/gtqjsnwdei.html

[U15] Py：高精度计时
来源：http://hz.jqgfzy.top/gtiqebglli.html

t = time.perf_counter()
来源：http://hz.tanke756.top/gtncnlhytk.html

[U16] Py：命令行参数解析
来源：http://hz.tanke756.top/gtikkdrtke.html

ap = argparse.ArgumentParser();  ap.add_argument("--name");  args = ap.parse_args()
来源：http://hz.nwbrower.top/gtxvntlmuf.html

[U17] Py：初始化日志
来源：http://hz.jqgufenzy.top/gtczcuzcns.html

logging.basicConfig(level=logging.INFO)
来源：http://hz.daxiang520.top/gtwfebowdh.html

[U18] Py：预编译正则
来源：http://hz.vqdsnc.cn/gtwgppduki.html

pat = re.compile(r"\d+")
来源：http://hz.tanke756.top/gteotemxzf.html

[U19] Py：正则替换带回调
来源：http://hz.hywenlv.cn/gttddommlp.html

re.sub(r"\d+", lambda m: str(int(m.group()) * 2), s)
来源：http://hz.shanyushiyangtech.top/gtpgdsgzku.html

[U20] Py：缓存函数结果
来源：http://hz.jqgfzy.top/gtxzmvkwnd.html

@functools.lru_cache(maxsize=None)
来源：http://hz.ehwqpu.com/gtrlbaxgwh.html

[U21] Py：自定义上下文管理器
来源：http://hz.cdnleiting.top/gthxyqprlf.html

@contextlib.contextmanager
来源：http://hz.chenzaomai.com/gtydjlmsvc.html

[U22] Py：矩阵转置
来源：http://hz.ywan-chungtsiang.top/gtryzyruuo.html

list(zip(*m))
来源：http://hz.nwbrower.top/gtemiiyhre.html

[U23] Py：分块读取大文件
来源：http://hz.chenzaomai.com/gtblyrftgg.html

for chunk in iter(lambda: f.read(8192), b""):
来源：http://hz.hnqzz.top/gtgexoetwv.html

[U24] Py：路径操作
来源：http://hz.xziqi.cn/gtcliiulmk.html

Path("a/b.txt").parent.mkdir(parents=True, exist_ok=True)
来源：http://hz.hongshengwenyu.top/gthigvdckd.html

[U25] Py：CSV 按字典读
来源：http://hz.9152youxi.cn/gtlbxtrjev.html

csv.DictReader(f)
来源：http://hz.jyoumei.cn/gthvudyfzk.html

[U26] Py：并发下载
来源：http://hz.pengpengdd.cyou/gtoahfndff.html

ThreadPoolExecutor(max_workers=8).map(fetch, urls)
来源：http://hz.ppjwa.cn/gtxvqovoac.html

[U27] Py：异步 HTTP
来源：http://hz.shzxlz.cn/gtvwualtcm.html

aiohttp.ClientSession() 配合 async with
来源：http://hz.xingfuxueyuan.xyz/gtbvdpfgsz.html

[U28] Py：类型别名
来源：http://hz.jinqigfzy.top/gtxhprieey.html

UserId = int
来源：http://hz.xuanzx.com/gtabfnbhbm.html

[U29] Py：属性校验
来源：http://hz.nanxuanxn.top/gtjgfphncw.html

@property 与 @x.setter 配合
来源：http://hz.cucudq.cn/gtnhymmnqh.html

[U30] Py：数据类
来源：http://hz.zycfv.cn/gtmtoniheb.html

@dataclass(slots=True)
来源：http://hz.yj20258.top/gtmgkouilr.html

[U31] Py：单测
来源：http://hz.yanxiufei.cn/gtcwsesexw.html

python -m pytest -q
来源：http://hz.jinqigfzy.top/gtewizbbxf.html

[U32] Py：代码格式化
来源：http://hz.yuanzhike.top/gtaqvsqsam.html

ruff format . && ruff check --fix .
来源：http://hz.cqqwz.cn/gtueunrwms.html

[U33] Py：打包发布
来源：http://hz.jqgufenzy.top/gtxczxokob.html

python -m build  （依赖 pyproject.toml）
来源：http://hz.snrcjt.cn/gtmzwnlcmm.html

[U34] Py：判断编码
来源：http://hz.tian-w.cn/gtyoqdjnus.html

chardet.detect(raw)
来源：http://hz.haohaochexian.top/gtoyysiwyb.html

[U35] Py：发送邮件
来源：http://hz.9152youxi.cn/gtvkxiojnp.html

smtplib.SMTP_SSL(...).send_message(msg)
来源：http://hz.ybcxt.top/gtlflqwgqm.html

[U36] Py：定时任务
来源：http://hz.yj202588.top/gtlcaplzia.html

schedule.every(10).minutes.do(job)
来源：http://hz.guowangkeji.top/gtextbjbar.html

[U37] Py：读写 Excel
来源：http://hz.jinghuilouyu.cn/gtjxbrwyra.html

pandas.read_excel / DataFrame.to_excel
来源：http://hz.tian-w.cn/gtwdntbedt.html

[U38] Py：获取脚本所在目录
来源：http://hz.yvedp.cn/gtgkkzeafu.html

Path(__file__).resolve().parent
来源：http://hz.shangyingyoupin.top/gtpqpjctff.html

[U39] Py：判断是否在交互环境
来源：http://hz.jinghuilouyu.cn/gttcjhezus.html

sys.stdout.isatty()
来源：http://hz.jinyuanbaomall.cn/gtjwxebefe.html

[U40] Py：打印到标准错误
来源：http://hz.xuanzx.com/gtubujquyf.html

print("err", file=sys.stderr)
来源：http://hz.pycfn.com/gtytwzevem.html

[U41] PHP：初始化 Composer 项目
来源：http://hz.daria6918.cn/gtafxosspv.html

composer init;  composer require guzzlehttp/guzzle
来源：http://hz.shuidangran.top/gtvpitowmm.html

[U42] PHP：PSR-4 自动加载
来源：http://hz.chenzaomai.com/gttofcpvue.html

"autoload": { "psr-4": { "App\\": "src/" } }
来源：http://hz.mhx1999.top/gttikikvcl.html


<!-- 参考信息 -->