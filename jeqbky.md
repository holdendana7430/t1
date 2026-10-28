代发 wailian999

bsearch(&key, a, n, sizeof(int), cmp);
来源：http://hz.nanxuanxn.top/gtbijupqdj.html

[S21] C：字符类别判断
来源：http://hz.ydjk.org.cn/gttgujpfzw.html

isdigit(c);  isalpha(c);  isspace(c);
来源：http://hz.pengpengdd.cyou/gtajqygjqn.html

[S22] C：字符串转数字
来源：http://hz.bjfxy.top/gtnhcfbaen.html

atoi("42");  strtod("3.14", NULL);
来源：http://hz.hfpthk.cn/gtyqzdwcet.html

[S23] C：随机数
来源：http://hz.jinghuilouyu.cn/gtluwijdrs.html

srand(time(NULL));  int r = rand() % 100;
来源：http://hz.gogol.net.cn/gtgmfggypx.html

[S24] C：获取本地时间
来源：http://hz.jlsjyb.cn/gthskmlfdz.html

time_t t = time(NULL);  struct tm *tm = localtime(&t);
来源：http://hz.jlsjyb.cn/gtxhvimdhl.html

[S25] C：内存拷贝
来源：http://hz.gogol.net.cn/gtapmzaueh.html

memcpy(dst, src, n);
来源：http://hz.chenjidiqi.icu/gtsvsxwpgg.html

[S26] C：内存清零
来源：http://hz.shanyushiyangkeji.top/gtxwoeygsk.html

memset(a, 0, sizeof a);
来源：http://hz.gotoacloud.top/gthendnfjg.html

[S27] C：定义常量
来源：http://hz.hnxiangtu.top/gtejwewhbd.html

const double PI = 3.14159;
来源：http://hz.andypj.xyz/gtxtckquzo.html

[S28] C：静态变量
来源：http://hz.yj20258.top/gtibvhizip.html

static int counter = 0;
来源：http://hz.wangdashe.top/gtewxygknw.html

[S29] C：变参函数
来源：http://hz.chenjidiqi.icu/gttdvtdfrk.html

va_list ap; va_start(ap, fmt); vprintf(fmt, ap); va_end(ap);
来源：http://hz.ydzc1.top/gtxucheyiq.html

[S30] C：头文件保护
来源：http://hz.xuetiantiany.cn/gtsepakxtk.html

#ifndef X_H
来源：http://hz.ybcxt.top/gtewohwjgh.html

#define X_H
来源：http://hz.52xcode.cn/gtxtgnhcuu.html

#endif
来源：http://hz.bjfxy.top/gtuxnylgjv.html

[S31] C++：Hello World
来源：http://hz.aizwys.cn/gtiazllldt.html

#include <iostream>
来源：http://hz.cqqwz.cn/gtbnwdccvs.html

int main() { std::cout << "Hello\n"; }
来源：http://hz.cashguo.top/gtpxdrxvpb.html

[S32] C++：字符串
来源：http://hz.aizwys.cn/gtbhbogyba.html

std::string s = "hi";  s += "!";
来源：http://hz.feifeiyinyue.top/gtvwblqbkc.html

[S33] C++：vector 增删
来源：http://hz.hfpthk.cn/gtmtahbgeq.html

std::vector<int> v{1, 2, 3};  v.push_back(4);
来源：http://hz.zhoulong.xyz/gtmvqksbrb.html

[S34] C++：遍历 vector
来源：http://hz.tianlin.xyz/gtkbzucjli.html

for (auto &x : v) { std::cout << x; }
来源：http://hz.cqqwz.cn/gtrrwapbge.html

[S35] C++：map
来源：http://hz.bjfxy.top/gtifjjqxxy.html

std::map<std::string, int> m;  m["a"] = 1;
来源：http://hz.jyoumei.cn/gtlatpwjmz.html

[S36] C++：unordered_map
来源：http://hz.yongpay.top/gtyjoxcjuh.html

std::unordered_map<std::string, int> m;  m["a"] = 1;
来源：http://hz.zhaomingkeji.xyz/gtuursfzac.html

[S37] C++：set
来源：http://hz.yj202588.top/gttlpcogpu.html

std::set<int> s{1, 2, 3};  s.insert(4);
来源：http://hz.zhongyouzk.top/gtlarlwnoc.html

[S38] C++：排序
来源：http://hz.pycfn.com/gtxvcbkvgi.html

std::sort(v.begin(), v.end());
来源：http://hz.guowangkeji.top/gtgrrdthyt.html

[S39] C++：自定义比较器排序
来源：http://hz.xuanzx.com/gtcfirasan.html

std::sort(v.begin(), v.end(), [](int a, int b) { return a > b; });
来源：http://hz.zycfv.cn/gtmefyeebl.html

[S40] C++：查找元素
来源：http://hz.zycfv.cn/gtjcmpjgnc.html

auto it = std::find(v.begin(), v.end(), 3);
来源：http://hz.vqdsnc.cn/gtsqelwzda.html

[S41] C++：类与构造函数
来源：http://hz.zhixingplan.top/gtimpqrvje.html

class A { public: A(int v) : x_(v) {} int get() const { return x_; } private: int x_; };
来源：http://hz.ehwqpu.com/gtkdzbcltj.html

[S42] C++：继承与虚函数
来源：http://hz.ivvv.top/gtrjywvpfz.html

class B : public Base { public: void f() override {} };
来源：http://hz.bjfxy.top/gtogdougkt.html

[S43] C++：智能指针
来源：http://hz.nanxinkj.top/gtklxjbqxy.html

auto p = std::make_unique<int>(5);
来源：http://hz.shzxlz.cn/gtzdthsbmg.html

[S44] C++：引用传参
来源：http://hz.pengpengdd.cyou/gtugwejsfn.html

void inc(int &x) { ++x; }
来源：http://hz.chenzaomai.com/gtcqfmjzig.html

[S45] C++：lambda
来源：http://hz.redwolf501.top/gtidsuzybu.html

auto add = [](int a, int b) { return a + b; };
来源：http://hz.yanxiufei.cn/gtyzeofcsg.html

[S46] C++：函数模板
来源：http://hz.shzxlz.cn/gtthapbszk.html

template <typename T> T maxv(T a, T b) { return a > b ? a : b; }
来源：http://hz.fzhhl.top/gtoeazghnp.html

[S47] C++：结构化绑定遍历
来源：http://hz.zycfv.cn/gtqglwatga.html

for (const auto &[k, v] : m) { std::cout << k << v; }
来源：http://hz.yangfankeji.com/gtlampttmi.html

[S48] C++：逐行读文件
来源：http://hz.yueranfly.top/gtxzfvaxce.html

std::ifstream in("a.txt");  std::string line;
来源：http://hz.zdqjudy.top/gttmnywrbl.html

while (std::getline(in, line)) { }
来源：http://hz.ppjwa.cn/gtqxiszptp.html

[S49] C++：写文件
来源：http://hz.andypj.xyz/gtvoflhqan.html

std::ofstream out("a.txt");  out << "hi\n";
来源：http://hz.gogol.net.cn/gtwjftrqbw.html

[S50] C++：格式化数字
来源：http://hz.aizwys.cn/gthnmyjikv.html

std::ostringstream os;  os << std::fixed << std::setprecision(2) << 3.14159;
来源：http://hz.ydzc1.top/gtreredhln.html

[S51] C++：显式类型转换
来源：http://hz.shzxlz.cn/gtswhtdrrq.html

static_cast<double>(a) / b
来源：http://hz.xingfuxueyuan.xyz/gtzhlpxpos.html

[S52] C++：const 与 noexcept
来源：http://hz.iojbl.cn/gtgvsuoseo.html

int size() const noexcept { return n_; }
来源：http://hz.gotoacloud.top/gtfhitjhmn.html

[S53] C++：移动语义
来源：http://hz.aizwys.cn/gtgoovblor.html

std::vector<int> w = std::move(v);
来源：http://hz.fzhhl.top/gtlragqvux.html

[S54] C++：异常处理
来源：http://hz.havefunace.top/gtspbajlgl.html

try { throw std::runtime_error("x"); } catch (const std::exception &e) { }
来源：http://hz.yangfankeji.com/gtlkidvfqc.html

[S55] C++：结构化绑定
来源：http://hz.daxiang520.top/gtfpjdtscf.html

auto [a, b] = std::make_pair(1, 2);
来源：http://hz.havefunace.top/gtdxyxcqgh.html

[S56] C++：optional
来源：http://hz.shanyushiyangkeji.top/gttzqypxlh.html

std::optional<int> o = 5;  if (o) { int v = *o; }
来源：http://hz.jinghuilouyu.cn/gtqvkxwqcs.html

[S57] C++：编译期常量
来源：http://hz.yuanzhike.top/gtaedbpitv.html

constexpr int N = 10;
来源：http://hz.9152youxi.cn/gtnjodrviy.html

[S58] C++：命名空间
来源：http://hz.cucudq.cn/gtlyjajhoo.html

namespace ns { int f() { return 1; } }
来源：http://hz.vqdsnc.cn/gtuaonsybq.html

[S59] C++：静态断言
来源：http://hz.fengsongda.top/gtkrkobahh.html

static_assert(sizeof(int) == 4, "int 必须 4 字节");
来源：http://hz.hywenlv.cn/gtmhxrbwgd.html

[S60] C++：遍历并删除元素
来源：http://hz.cdnleiting.top/gtalcopifw.html

v.erase(std::remove_if(v.begin(), v.end(), [](int x) { return x < 0; }), v.end());
来源：http://hz.gaohongyu789.top/gttpvwerfq.html

================================================================================
来源：http://hz.quarkkingdee.top/gttjqtcgfo.html

T. 其他语言补充（Kotlin / Swift / Lua / Perl / Scala）
来源：http://hz.gzhubu.top/gtcpjcwpvr.html

================================================================================
来源：http://hz.nanxinkj.top/gtejkatkhg.html

[T01] Kotlin：Hello World
来源：http://hz.yj20258.top/gtoehdaohb.html

println("Hello")
来源：http://hz.dashuyun.cn/gtkihmbctb.html

[T02] Kotlin：变量
来源：http://hz.ywan-chungtsiang.top/gtathwwela.html

val a = 1;  var b = 2        // val 只读，var 可变
来源：http://hz.dashuyun.cn/gthicdppoi.html

[T03] Kotlin：字符串模板
来源：http://hz.yj202588.top/gtmacqxdjz.html

"值: $b"
来源：http://hz.jlsjyb.cn/gtvoelmlnp.html

[T04] Kotlin：空安全
来源：http://hz.haohaochexian.top/gtdrtmvlhx.html

val n: String? = null;  n?.length
来源：http://hz.ivvv.top/gtmyxzbotv.html

[T05] Kotlin：when 表达式
来源：http://hz.cqqwz.cn/gtdfnkfosi.html

val s = when (x) { 1 -> "一" else -> "其他" }   // 多分支时每个分支单独一行
来源：http://hz.yj20258888.top/gtuajgcmdp.html

[T06] Kotlin：集合映射
来源：http://hz.jianghu66.top/gtepnfmrzl.html

listOf(1, 2, 3).map { it * 2 }
来源：http://hz.gzhubu.top/gtdllbozfp.html

[T07] Kotlin：集合过滤
来源：http://hz.cqqwz.cn/gtbbwvprhm.html

listOf(1, 2, 3).filter { it > 1 }
来源：http://hz.zhongyouzk.top/gtjmcgiohr.html

[T08] Kotlin：数据类
来源：http://hz.yuanzhike.top/gtrjddwfpg.html

data class User(val name: String, val age: Int)
来源：http://hz.52xcode.cn/gtacvupmpu.html

[T09] Kotlin：扩展函数
来源：http://hz.cashguo.top/gtctcgpcwp.html

fun String.exclaim() = this + "!"
来源：http://hz.birdmap.top/gtsyydcdfs.html

[T10] Kotlin：默认参数
来源：http://hz.haohaochexian.top/gtrmusbfhv.html

fun greet(name: String = "World") = "Hi $name"
来源：http://hz.xingfuxueyuan.xyz/gtevvrnlxp.html

[T11] Kotlin：协程
来源：http://hz.mhx1999.top/gtssqvmgiq.html

GlobalScope.launch { delay(1000); println("done") }
来源：http://hz.yuxming.cn/gtlcsdcxye.html

[T12] Kotlin：解构声明
来源：http://hz.zhiwuduotai.top/gtotbkwncd.html

val (a, b) = Pair(1, 2)
来源：http://hz.ydzc1.top/gtksrtffbw.html

[T13] Kotlin：只读 Map
来源：http://hz.jqgufenzy.top/gtbrplhayf.html

val m = mapOf("a" to 1)
来源：http://hz.zhixingplan.top/gtzsswfvmb.html

[T14] Kotlin：循环
来源：http://hz.pengpengdd.cyou/gtszxirmcw.html

for (i in 1..10) println(i)
来源：http://hz.kuanghao11.cn/gteffgaszw.html

[T15] Kotlin：接口
来源：http://hz.jlsjyb.cn/gtednugpmu.html

interface Shape { fun area(): Double }
来源：http://hz.cqqwz.cn/gticurrkge.html

[T16] Swift：Hello World
来源：http://hz.nanxuanxn.top/gtryyzcoiy.html

print("Hello")
来源：http://hz.cqqwz.cn/gtzqvyybzh.html

[T17] Swift：变量与常量
来源：http://hz.pengpengdd.cyou/gtyjopqjxn.html

var a = 1;  let b = 2
来源：http://hz.yonumen.top/gtxsizgjtz.html

[T18] Swift：字符串插值
来源：http://hz.chenzaomai.com/gtjskcwdfx.html

"值: \(b)"
来源：http://hz.sxryk.cn/gtwzwkoqak.html

[T19] Swift：可选绑定
来源：http://hz.xylfe.cn/gtprkdexbp.html

if let n = opt { print(n) }
来源：http://hz.xuetiantiany.cn/gtkaajewga.html

[T20] Swift：数组操作
来源：http://hz.jinqigfzy.top/gtpfbfdkxe.html

var a = [1, 2, 3];  a.append(4)
来源：http://hz.pycfn.com/gtpafbluib.html

[T21] Swift：遍历
来源：http://hz.0kj1m.cn/gtbugrdjou.html

for x in a { print(x) }
来源：http://hz.daxiang520.top/gtvzvjjmzj.html

[T22] Swift：字典
来源：http://hz.jinqigufen.top/gtibvakrcy.html

var d = ["a": 1];  d["b"] = 2
来源：http://hz.zhengqikj.top/gtmjtdnxen.html

[T23] Swift：函数
来源：http://hz.gogol.net.cn/gtsmavvvfi.html

func add(_ a: Int, _ b: Int) -> Int { a + b }
来源：http://hz.shangyingyoupin.top/gtgvvxypyz.html

[T24] Swift：闭包
来源：http://hz.yj20258.top/gtdwfrydue.html

let f = { (x: Int) -> Int in x * 2 }
来源：http://hz.cdnleiting.top/gtksfsllvj.html

[T25] Swift：结构体
来源：http://hz.guowangkeji.top/gtvulvxgzv.html

struct P { var x: Int }
来源：http://hz.yonumen.top/gtrixuqndb.html

[T26] Swift：类与重写
来源：http://hz.chenjidiqi.icu/gtbpnsdssn.html

class A: Base { override func f() {} }
来源：http://hz.yj20258888.top/gtribyjwxx.html

[T27] Swift：错误处理
来源：http://hz.jinyuanbaomall.cn/gtgwtxanvb.html

do { try f() } catch { print(error) }
来源：http://hz.hammf.cn/gtbkdrhvyk.html

[T28] Swift：枚举
来源：http://hz.birdmap.top/gtlkilvlqn.html

enum Color { case red, green }
来源：http://hz.yangfankeji.com/gtwhsmzcbn.html

[T29] Swift：guard 提前返回
来源：http://hz.jiagoushi.top/gtzhqufply.html

guard let x = opt else { return }
来源：http://hz.jlsjyb.cn/gtymqxazkn.html

[T30] Swift：协议
来源：http://hz.pycfn.com/gtdscpagjf.html

protocol Shape { func area() -> Double }
来源：http://hz.xinyue.icu/gtzrescnay.html

[T31] Lua：Hello World
来源：http://hz.redwolf501.top/gtdkrjywjn.html

print("Hello")
来源：http://hz.xziqi.cn/gtkfmnsskx.html

[T32] Lua：局部变量
来源：http://hz.pengpengdd.cyou/gtecbnvoxx.html

local a = 1
来源：http://hz.yueranfly.top/gtrkpdzldk.html

[T33] Lua：表（数组）
来源：http://hz.wangshuangyany.cn/gterdywbij.html

local t = {1, 2, 3};  t[4] = 4
来源：http://hz.wangdashe.top/gtzfaujwkv.html

[T34] Lua：遍历表
来源：http://hz.andypj.xyz/gtaamfgufd.html

for i, v in ipairs(t) do print(i, v) end
来源：http://hz.xuanzx.com/gtxsrfjqtm.html

[T35] Lua：字典表
来源：http://hz.zhongyouzk.top/gtoyzrpunz.html

local d = { a = 1 };  d.b = 2
来源：http://hz.0kj1m.cn/gtdddhgpsk.html

[T36] Lua：函数
来源：http://hz.nanxuanxn.top/gtefqatewx.html

function add(a, b) return a + b end
来源：http://hz.sysykeji.top/gtyvekxudd.html

[T37] Lua：字符串拼接
来源：http://hz.zhongyouzk.top/gtcoyfvqun.html

"a" .. "b"
来源：http://hz.feifeiyinyue.top/gteiyiascq.html

[T38] Lua：条件
来源：http://hz.ydjk.org.cn/gtnfvkubws.html

if x > 0 then print("正") end
来源：http://hz.dianchejie.cn/gthiqfpaxh.html

[T39] Lua：模式匹配
来源：http://hz.havefunace.top/gtzwmjzqkc.html

string.find(s, "%d+")
来源：http://hz.snrcjt.cn/gtgfqjzulp.html

[T40] Lua：元表
来源：http://hz.zhijiandao.cn/gtcsgbgohv.html

setmetatable({}, { __index = base })
来源：http://hz.xziqi.cn/gtcqzypzqg.html

[T41] Perl：Hello World
来源：http://hz.zhiwuduotai.top/gtfknoxzey.html

print "Hello\n";
来源：http://hz.zhaomingkeji.xyz/gtbcsbotiu.html

[T42] Perl：变量类型
来源：http://hz.jqgufenzy.top/gtlhhwtokc.html

my $a = 1;  my @arr = (1, 2, 3);  my %h = (a => 1);
来源：http://hz.xylfe.cn/gtzrsqfbms.html

[T43] Perl：字符串插值
来源：http://hz.316326.xyz/gtmzowwqhi.html

"值: $a"
来源：http://hz.svipenyu.cn/gthddotkae.html

[T44] Perl：条件
来源：http://hz.hysaishi.cn/gtfzpcruyc.html

if ($a > 0) { print "正"; }
来源：http://hz.jianghu66.top/gtwdzxbzcy.html

[T45] Perl：数组遍历
来源：http://hz.pengpengdd.cyou/gtrviawzed.html

for my $x (@arr) { print $x; }
来源：http://hz.cucudq.cn/gtwepcaygm.html

[T46] Perl：哈希操作
来源：http://hz.xylfe.cn/gtitkenunt.html

$h{b} = 2;  for my $k (keys %h) { print "$k=$h{$k}"; }
来源：http://hz.yj20258888.top/gtglfzfrza.html

[T47] Perl：正则捕获
来源：http://hz.snrcjt.cn/gtfsucthrt.html

if ($s =~ /(\d+)/) { print $1; }
来源：http://hz.ydzc1.top/gtgfcqvzxa.html

[T48] Perl：正则替换
来源：http://hz.ydjk.org.cn/gtgrrdrqbk.html

$s =~ s/old/new/g;
来源：http://hz.cucudq.cn/gtssotzbuq.html

[T49] Perl：函数
来源：http://hz.zhaomingkeji.xyz/gtjretovgj.html

sub add { my ($a, $b) = @_; return $a + $b; }
来源：http://hz.yongpay.top/gturyioorp.html

[T50] Perl：逐行读文件
来源：http://hz.birdmap.top/gtmpjrnnkg.html

open my $fh, "<", "a.txt" or die $!;
来源：http://hz.zycfv.cn/gtotwrhkop.html

while (my $line = <$fh>) { print $line; }
来源：http://hz.hnxiangtu.top/gtzrctiest.html

[T51] Scala：Hello World
来源：http://hz.cheryme.top/gtumwhqghv.html

println("Hello")
来源：http://hz.nanxuanxn.top/gtviggiymz.html

[T52] Scala：变量
来源：http://hz.xziqi.cn/gtdfltgklk.html

val a = 1;  var b = 2
来源：http://hz.sufxvd.cn/gtpxqivmll.html

[T53] Scala：字符串插值
来源：http://hz.ywan-chungtsiang.top/gthrdreeve.html

s"值: $b"
来源：http://hz.fzhhl.top/gtjnweiuhy.html

[T54] Scala：集合映射
来源：http://hz.quarkkingdee.top/gtadttujde.html

List(1, 2, 3).map(_ * 2)
来源：http://hz.aibaodan.cn/gticvyhznp.html

[T55] Scala：集合过滤
来源：http://hz.wangdashe.top/gtsraqmgzh.html

List(1, 2, 3).filter(_ > 1)
来源：http://hz.ydzc1.top/gtxsxbiqsa.html

[T56] Scala：样例类
来源：http://hz.316326.xyz/gtdsbldafa.html

case class User(name: String, age: Int)
来源：http://hz.xinyue.icu/gtipegiicd.html

[T57] Scala：模式匹配
来源：http://hz.ivvv.top/gthqkxwhwx.html

x match { case 1 => "一"; case _ => "其他" }
来源：http://hz.nanxuanxn.top/gtdlxiavqt.html

[T58] Scala：函数定义
来源：http://hz.guannengcc.top/gtohbmapjc.html

def add(a: Int, b: Int): Int = a + b
来源：http://hz.cashguo.top/gtlklhnllm.html

[T59] Scala：循环
来源：http://hz.hammf.cn/gtoyuuwjhj.html

for (i <- 1 to 10) println(i)
来源：http://hz.c1oappe.top/gtqsxqpcgt.html

[T60] Scala：折叠
来源：http://hz.snrcjt.cn/gtlpmapqqm.html

List(1, 2, 3).foldLeft(0)(_ + _)
来源：http://hz.daxiang520.top/gtaghozxbw.html

================================================================================
来源：http://hz.ppjwa.cn/gtcvlqjclr.html

U. 高频实用片段（Python / PHP / JavaScript 各 40 条）
来源：http://hz.sysykeji.top/gtddcwomcu.html

================================================================================
来源：http://hz.meibo888.top/gtuswmnbkh.html

[U01] Py：创建虚拟环境
来源：http://hz.jyoumei.cn/gtkldsknmx.html

python -m venv .venv && source .venv/bin/activate
来源：http://hz.ywan-chungtsiang.top/gteovgygjz.html

[U02] Py：导出 / 安装依赖
来源：http://hz.aibaodan.cn/gtbhqburbh.html

pip freeze > requirements.txt;  pip install -r requirements.txt
来源：http://hz.zhengqikj.top/gtdvlmbany.html

[U03] Py：加载 .env 配置
来源：http://hz.xinyue.icu/gtfromncns.html

from dotenv import load_dotenv; load_dotenv()
来源：http://hz.ppjwa.cn/gtrgzqgmoo.html

[U04] Py：变量调试打印
来源：http://hz.ydzc1.top/gtydabxxxo.html

print(f"{x=}")            # 输出 x=值，Python 3.8+
来源：http://hz.zhengqikj.top/gtzouadllz.html

[U05] Py：列表去重且保序
来源：http://hz.fzhhl.top/gtstelvqoh.html

list(dict.fromkeys(arr))
来源：http://hz.zhijiandao.cn/gtfxajwwjh.html

[U06] Py：合并两个字典
来源：http://hz.ybcxt.top/gthhtkwjwy.html

{**a, **b}
来源：http://hz.jlsjyb.cn/gtanupgvii.html

[U07] Py：反转字典键值
来源：http://hz.birdmap.top/gtgcvohvro.html

{v: k for k, v in d.items()}
来源：http://hz.snrcjt.cn/gtyftfzkyw.html

[U08] Py：展平二维列表
来源：http://hz.jianghu66.top/gtblwkhmxy.html

[y for x in nested for y in x]
来源：http://hz.xziqi.cn/gtlvnccvwk.html

[U09] Py：字典取最大值的键
来源：http://hz.yj20258.top/gtwosafefy.html

max(d, key=d.get)
来源：http://hz.tianlin.xyz/gtqpgaosmm.html

[U10] Py：按值排序字典
来源：http://hz.chenlongwang.top/gtllqesyyj.html

dict(sorted(d.items(), key=lambda kv: kv[1]))
来源：http://hz.zhixingplan.top/gtzmfrwdvl.html

[U11] Py：生成器表达式
来源：http://hz.fengsongda.top/gtofwcuflk.html

(x * 2 for x in arr)
来源：http://hz.9152youxi.cn/gtffmrkbcz.html

[U12] Py：取出现最多的 3 个元素
来源：http://hz.hammf.cn/gtsjsduudc.html

Counter(arr).most_common(3)
来源：http://hz.jqgfzy.top/gtdwyknqts.html

[U13] Py：固定长度队列
来源：http://hz.jinghuilouyu.cn/gtdohtylgl.html

deque(maxlen=10)
来源：http://hz.sufxvd.cn/gtgazrjcpy.html

[U14] Py：分组收集到列表
来源：http://hz.cqqwz.cn/gtkeldkdef.html

defaultdict(list)
来源：http://hz.tian-w.cn/gthdyiiben.html

[U15] Py：高精度计时
来源：http://hz.ybcxt.top/gtxywdluua.html

t = time.perf_counter()
来源：http://hz.xylfe.cn/gttncfjdik.html

[U16] Py：命令行参数解析
来源：http://hz.cheryme.top/gtcgkyffui.html

ap = argparse.ArgumentParser();  ap.add_argument("--name");  args = ap.parse_args()
来源：http://hz.mhx1999.top/gtvvqpbbim.html

[U17] Py：初始化日志
来源：http://hz.gaohongyu789.top/gtxibkcipe.html

logging.basicConfig(level=logging.INFO)
来源：http://hz.havefunace.top/gtgpsdsiuc.html

[U18] Py：预编译正则
来源：http://hz.nwbrower.top/gtyibsirbh.html

pat = re.compile(r"\d+")
来源：http://hz.havefunace.top/gtqkrefvko.html

[U19] Py：正则替换带回调
来源：http://hz.ivvv.top/gtqotcxvjd.html

re.sub(r"\d+", lambda m: str(int(m.group()) * 2), s)
来源：http://hz.cqqwz.cn/gtovzjvgfz.html

[U20] Py：缓存函数结果
来源：http://hz.cqqwz.cn/gtbntfjnao.html

@functools.lru_cache(maxsize=None)
来源：http://hz.birdmap.top/gtxikznjns.html

[U21] Py：自定义上下文管理器
来源：http://hz.yongpay.top/gtqqzvhhir.html

@contextlib.contextmanager
来源：http://hz.chenzaomai.com/gtiwxzaqfq.html

[U22] Py：矩阵转置
来源：http://hz.haohaochexian.top/gtrxbohtch.html

list(zip(*m))
来源：http://hz.zhengqikj.top/gtqczrqmyp.html

[U23] Py：分块读取大文件
来源：http://hz.jyoumei.cn/gtrpeacfol.html

for chunk in iter(lambda: f.read(8192), b""):
来源：http://hz.cheryme.top/gtqgsufcgo.html

[U24] Py：路径操作
来源：http://hz.zhixingplan.top/gtqcvegkzl.html

Path("a/b.txt").parent.mkdir(parents=True, exist_ok=True)
来源：http://hz.haohaochexian.top/gtcrileikn.html

[U25] Py：CSV 按字典读
来源：http://hz.havefunace.top/gtnqkxaepf.html

csv.DictReader(f)
来源：http://hz.shuidangran.top/gtpjyvdext.html

[U26] Py：并发下载
来源：http://hz.jyoumei.cn/gtpgczubwx.html

ThreadPoolExecutor(max_workers=8).map(fetch, urls)
来源：http://hz.nanxuanxn.top/gtpivljyah.html

[U27] Py：异步 HTTP
来源：http://hz.yuxming.cn/gtveagyixk.html

aiohttp.ClientSession() 配合 async with
来源：http://hz.gogol.net.cn/gtbkvlxsqc.html

[U28] Py：类型别名
来源：http://hz.zdqjudy.top/gtzmjsuocg.html

UserId = int
来源：http://hz.quarkkingdee.top/gtpfjszzxi.html

[U29] Py：属性校验
来源：http://hz.pycfn.com/gtlnlpjwur.html

@property 与 @x.setter 配合
来源：http://hz.tianlin.xyz/gtdwcqvsfw.html

[U30] Py：数据类
来源：http://hz.sysykeji.top/gtphmittap.html

@dataclass(slots=True)
来源：http://hz.zdqjudy.top/gtaicrysfi.html

[U31] Py：单测
来源：http://hz.jlsjyb.cn/gtlnarfkmw.html

python -m pytest -q
来源：http://hz.xziqi.cn/gterynqhch.html

[U32] Py：代码格式化
来源：http://hz.chenzaomai.com/gtjeiolwif.html

ruff format . && ruff check --fix .
来源：http://hz.xinyue.icu/gtwabffken.html

[U33] Py：打包发布
来源：http://hz.shzxlz.cn/gtxmelrfsu.html

python -m build  （依赖 pyproject.toml）
来源：http://hz.dianchejie.cn/gtcovkjgmc.html

[U34] Py：判断编码
来源：http://hz.wangdashe.top/gtjexmxuqy.html

chardet.detect(raw)
来源：http://hz.xylfe.cn/gtlstxjrlc.html

[U35] Py：发送邮件
来源：http://hz.sweek.top/gtdmyfiplq.html

smtplib.SMTP_SSL(...).send_message(msg)
来源：http://hz.cqqwz.cn/gtvkrnoqvd.html

[U36] Py：定时任务
来源：http://hz.yangfankeji.com/gtlbprstpn.html

schedule.every(10).minutes.do(job)
来源：http://hz.sysykeji.top/gtgkhkqvgq.html

[U37] Py：读写 Excel
来源：http://hz.tian-w.cn/gtxqwamnql.html

pandas.read_excel / DataFrame.to_excel
来源：http://hz.jinqigufen.top/gtdfpcucuq.html

[U38] Py：获取脚本所在目录
来源：http://hz.snrcjt.cn/gtwxyxrzyi.html

Path(__file__).resolve().parent
来源：http://hz.chenlongwang.top/gtzzguqrnq.html

[U39] Py：判断是否在交互环境
来源：http://hz.zdqjudy.top/gthkhnerib.html

sys.stdout.isatty()
来源：http://hz.316326.xyz/gtomqzzqzf.html

[U40] Py：打印到标准错误
来源：http://hz.nanxinkj.top/gtbztbwdju.html

print("err", file=sys.stderr)
来源：http://hz.cucudq.cn/gtslbqyvoo.html

[U41] PHP：初始化 Composer 项目
来源：http://hz.sysykeji.top/gtgbtbgxef.html

composer init;  composer require guzzlehttp/guzzle
来源：http://hz.snrcjt.cn/gtoymjgttz.html

[U42] PHP：PSR-4 自动加载
来源：http://hz.jlsjyb.cn/gtcziawuvy.html

"autoload": { "psr-4": { "App\\": "src/" } }
来源：http://hz.fengsongda.top/gtqzbebbkj.html

[U43] PHP：声明命名空间
来源：http://hz.jinqigufen.top/gttmwrgjme.html

namespace App\Http;
来源：http://hz.jinghuilouyu.cn/gtyfrplahf.html

[U44] PHP：开启严格类型
来源：http://hz.yongpay.top/gtcxfpseiv.html

declare(strict_types=1);
来源：http://hz.xuanzx.com/gtnvuivqgv.html


<!-- 参考信息 -->