代发 wailian999

bsearch(&key, a, n, sizeof(int), cmp);
来源：http://hz.ppjwa.cn/gtcfuujufz.html

[S21] C：字符类别判断
来源：http://hz.pycfn.com/gtwjbfbcwg.html

isdigit(c);  isalpha(c);  isspace(c);
来源：http://hz.yvedp.cn/gtmdftnpwv.html

[S22] C：字符串转数字
来源：http://hz.nanxinkj.top/gtpfloyikc.html

atoi("42");  strtod("3.14", NULL);
来源：http://hz.gaohongyu789.top/gtnqnrjsxg.html

[S23] C：随机数
来源：http://hz.xziqi.cn/gtghrztnov.html

srand(time(NULL));  int r = rand() % 100;
来源：http://hz.nanxinkj.top/gtdgxuijgk.html

[S24] C：获取本地时间
来源：http://hz.xuanzx.com/gtedpanbzc.html

time_t t = time(NULL);  struct tm *tm = localtime(&t);
来源：http://hz.jlsjyb.cn/gtehdeymwg.html

[S25] C：内存拷贝
来源：http://hz.zhongyouzk.top/gtgjavquap.html

memcpy(dst, src, n);
来源：http://hz.hnxiangtu.top/gtoxmmkdyn.html

[S26] C：内存清零
来源：http://hz.nwbrower.top/gtvlhukrzb.html

memset(a, 0, sizeof a);
来源：http://hz.ehwqpu.com/gtweaamdze.html

[S27] C：定义常量
来源：http://hz.ywan-chungtsiang.top/gtrywotnyu.html

const double PI = 3.14159;
来源：http://hz.jinyuanbaomall.cn/gtpdmxrcyj.html

[S28] C：静态变量
来源：http://hz.dianchejie.cn/gtoqnmlkel.html

static int counter = 0;
来源：http://hz.ydjk.org.cn/gtcywtzvoo.html

[S29] C：变参函数
来源：http://hz.tian-w.cn/gtiarvncpv.html

va_list ap; va_start(ap, fmt); vprintf(fmt, ap); va_end(ap);
来源：http://hz.yongpay.top/gtysticdre.html

[S30] C：头文件保护
来源：http://hz.kuanghao11.cn/gtsejjjrfz.html

#ifndef X_H
来源：http://hz.andypj.xyz/gtipbegqne.html

#define X_H
来源：http://hz.wangshuangyany.cn/gtbqymwtlg.html

#endif
来源：http://hz.ivvv.top/gtvllbouqw.html

[S31] C++：Hello World
来源：http://hz.nwbrower.top/gtqrzgiqyp.html

#include <iostream>
来源：http://hz.mhx1999.top/gtjekfudzy.html

int main() { std::cout << "Hello\n"; }
来源：http://hz.nanxuanxn.top/gtztgapgda.html

[S32] C++：字符串
来源：http://hz.zycfv.cn/gtdyhupyrr.html

std::string s = "hi";  s += "!";
来源：http://hz.zhixingplan.top/gtsqhcydjt.html

[S33] C++：vector 增删
来源：http://hz.wangshuangyany.cn/gtvovwkfxo.html

std::vector<int> v{1, 2, 3};  v.push_back(4);
来源：http://hz.hysaishi.cn/gtdunldmiy.html

[S34] C++：遍历 vector
来源：http://hz.cdnleiting.top/gtobmiscxk.html

for (auto &x : v) { std::cout << x; }
来源：http://hz.birdmap.top/gtadguysbf.html

[S35] C++：map
来源：http://hz.shanyushiyangkeji.top/gtrwgaplvu.html

std::map<std::string, int> m;  m["a"] = 1;
来源：http://hz.hfpthk.cn/gtnsbyboae.html

[S36] C++：unordered_map
来源：http://hz.hongshengwenyu.top/gtdtltdebh.html

std::unordered_map<std::string, int> m;  m["a"] = 1;
来源：http://hz.quarkkingdee.top/gtbvbhkxad.html

[S37] C++：set
来源：http://hz.zhijiandao.cn/gtmyvddddp.html

std::set<int> s{1, 2, 3};  s.insert(4);
来源：http://hz.xylfe.cn/gtcxhlyxxp.html

[S38] C++：排序
来源：http://hz.9152youxi.cn/gtjbvibdws.html

std::sort(v.begin(), v.end());
来源：http://hz.zhoulong.xyz/gtksbrxjna.html

[S39] C++：自定义比较器排序
来源：http://hz.yj202588.top/gtistndluy.html

std::sort(v.begin(), v.end(), [](int a, int b) { return a > b; });
来源：http://hz.yvedp.cn/gtznerbkse.html

[S40] C++：查找元素
来源：http://hz.feifeiyinyue.top/gtonmxeeoc.html

auto it = std::find(v.begin(), v.end(), 3);
来源：http://hz.yangfankeji.com/gtucdymusr.html

[S41] C++：类与构造函数
来源：http://hz.shangyingyoupin.top/gtoqzwflhk.html

class A { public: A(int v) : x_(v) {} int get() const { return x_; } private: int x_; };
来源：http://hz.pengpengdd.cyou/gtqslgjrtc.html

[S42] C++：继承与虚函数
来源：http://hz.birdmap.top/gtqhuqnrbh.html

class B : public Base { public: void f() override {} };
来源：http://hz.iojbl.cn/gtfvhprfxi.html

[S43] C++：智能指针
来源：http://hz.dashuyun.cn/gtlpxkzoyp.html

auto p = std::make_unique<int>(5);
来源：http://hz.yangfankeji.com/gtyctbwqzd.html

[S44] C++：引用传参
来源：http://hz.mhx1999.top/gtlaykgmek.html

void inc(int &x) { ++x; }
来源：http://hz.cheryme.top/gtpudbwgyr.html

[S45] C++：lambda
来源：http://hz.daria6918.cn/gtxtazbyhx.html

auto add = [](int a, int b) { return a + b; };
来源：http://hz.xziqi.cn/gtacrafdzc.html

[S46] C++：函数模板
来源：http://hz.yongpay.top/gtofnbpmzn.html

template <typename T> T maxv(T a, T b) { return a > b ? a : b; }
来源：http://hz.shanyushiyangtech.top/gtbpxzajob.html

[S47] C++：结构化绑定遍历
来源：http://hz.9152youxi.cn/gtqeipmgok.html

for (const auto &[k, v] : m) { std::cout << k << v; }
来源：http://hz.pengpengdd.cyou/gtkgqtivdj.html

[S48] C++：逐行读文件
来源：http://hz.ydzc1.top/gtnxyrvhwe.html

std::ifstream in("a.txt");  std::string line;
来源：http://hz.meibo888.top/gtodolosta.html

while (std::getline(in, line)) { }
来源：http://hz.svipenyu.cn/gtgdyiahue.html

[S49] C++：写文件
来源：http://hz.nwbrower.top/gtkunbhtvv.html

std::ofstream out("a.txt");  out << "hi\n";
来源：http://hz.sxryk.cn/gtpwymsayt.html

[S50] C++：格式化数字
来源：http://hz.gzhubu.top/gtsgioxazd.html

std::ostringstream os;  os << std::fixed << std::setprecision(2) << 3.14159;
来源：http://hz.tian-w.cn/gtciewjgih.html

[S51] C++：显式类型转换
来源：http://hz.daxiang520.top/gtvlqvqbte.html

static_cast<double>(a) / b
来源：http://hz.yuxming.cn/gtjkhvwpbb.html

[S52] C++：const 与 noexcept
来源：http://hz.smart0.xyz/gtszkfouaa.html

int size() const noexcept { return n_; }
来源：http://hz.shanyushiyangkeji.top/gtobjjmpzl.html

[S53] C++：移动语义
来源：http://hz.daria6918.cn/gtgljybwpc.html

std::vector<int> w = std::move(v);
来源：http://hz.sxryk.cn/gtkqxmcqvm.html

[S54] C++：异常处理
来源：http://hz.jinghuilouyu.cn/gtfarmwlbu.html

try { throw std::runtime_error("x"); } catch (const std::exception &e) { }
来源：http://hz.zhaomingkeji.xyz/gtxnugoums.html

[S55] C++：结构化绑定
来源：http://hz.fzhhl.top/gtctdbqmoy.html

auto [a, b] = std::make_pair(1, 2);
来源：http://hz.gzhubu.top/gtafnokquc.html

[S56] C++：optional
来源：http://hz.zhixingplan.top/gtsphgvgjk.html

std::optional<int> o = 5;  if (o) { int v = *o; }
来源：http://hz.xziqi.cn/gtofkwetqf.html

[S57] C++：编译期常量
来源：http://hz.ivvv.top/gtyehqzhop.html

constexpr int N = 10;
来源：http://hz.aibaodan.cn/gtufbslwaf.html

[S58] C++：命名空间
来源：http://hz.52xcode.cn/gtkgcntwpx.html

namespace ns { int f() { return 1; } }
来源：http://hz.tianlin.xyz/gtugerhcsu.html

[S59] C++：静态断言
来源：http://hz.tian-w.cn/gtpzyjyggg.html

static_assert(sizeof(int) == 4, "int 必须 4 字节");
来源：http://hz.shanyushiyangtech.top/gtwqohejap.html

[S60] C++：遍历并删除元素
来源：http://hz.yongpay.top/gtjyivtkkp.html

v.erase(std::remove_if(v.begin(), v.end(), [](int x) { return x < 0; }), v.end());
来源：http://hz.fzhhl.top/gtrheleuxj.html

================================================================================
来源：http://hz.yueranfly.top/gtvpjwpthq.html

T. 其他语言补充（Kotlin / Swift / Lua / Perl / Scala）
来源：http://hz.snrcjt.cn/gtyplyrtso.html

================================================================================
来源：http://hz.jianghu66.top/gtzuwzipxx.html

[T01] Kotlin：Hello World
来源：http://hz.zhoulong.xyz/gtajlbuevj.html

println("Hello")
来源：http://hz.chenzaomai.com/gtgobwnfyu.html

[T02] Kotlin：变量
来源：http://hz.hnxiangtu.top/gtrtdhwdkl.html

val a = 1;  var b = 2        // val 只读，var 可变
来源：http://hz.havefunace.top/gteufinxfq.html

[T03] Kotlin：字符串模板
来源：http://hz.pycfn.com/gtrqaeptwu.html

"值: $b"
来源：http://hz.smart0.xyz/gtcqsiqjag.html

[T04] Kotlin：空安全
来源：http://hz.jianghu66.top/gtjohpszev.html

val n: String? = null;  n?.length
来源：http://hz.shzxlz.cn/gtpdwzzrsi.html

[T05] Kotlin：when 表达式
来源：http://hz.ywan-chungtsiang.top/gtxggypmpv.html

val s = when (x) { 1 -> "一" else -> "其他" }   // 多分支时每个分支单独一行
来源：http://hz.jqgfzy.top/gtxjdkzepf.html

[T06] Kotlin：集合映射
来源：http://hz.hfpthk.cn/gthbgvawdd.html

listOf(1, 2, 3).map { it * 2 }
来源：http://hz.dianchejie.cn/gttdlktuha.html

[T07] Kotlin：集合过滤
来源：http://hz.cqqwz.cn/gtipmvftzi.html

listOf(1, 2, 3).filter { it > 1 }
来源：http://hz.tianlin.xyz/gtdqfcsrvz.html

[T08] Kotlin：数据类
来源：http://hz.cdnleiting.top/gtdifqlayg.html

data class User(val name: String, val age: Int)
来源：http://hz.shanyushiyangkeji.top/gtdxxbelrg.html

[T09] Kotlin：扩展函数
来源：http://hz.cqqwz.cn/gtqwuiibzw.html

fun String.exclaim() = this + "!"
来源：http://hz.pengpengdd.cyou/gtazxqycby.html

[T10] Kotlin：默认参数
来源：http://hz.zdqjudy.top/gtsyqfaeai.html

fun greet(name: String = "World") = "Hi $name"
来源：http://hz.aibaodan.cn/gtaikvumdt.html

[T11] Kotlin：协程
来源：http://hz.52xcode.cn/gtsdnzmlef.html

GlobalScope.launch { delay(1000); println("done") }
来源：http://hz.kuanghao11.cn/gttjqzacrp.html

[T12] Kotlin：解构声明
来源：http://hz.aizwys.cn/gttusyvwzi.html

val (a, b) = Pair(1, 2)
来源：http://hz.zhengqikj.top/gtdgttbuif.html

[T13] Kotlin：只读 Map
来源：http://hz.ydjk.org.cn/gtznewxwqy.html

val m = mapOf("a" to 1)
来源：http://hz.yj20258.top/gtacljzisy.html

[T14] Kotlin：循环
来源：http://hz.c1oappe.top/gtquzxeucw.html

for (i in 1..10) println(i)
来源：http://hz.haohaochexian.top/gtkkuykgsz.html

[T15] Kotlin：接口
来源：http://hz.zhijiandao.cn/gtvcyibnlm.html

interface Shape { fun area(): Double }
来源：http://hz.yj202588.top/gtyidxutls.html

[T16] Swift：Hello World
来源：http://hz.jinghuilouyu.cn/gtuubekspj.html

print("Hello")
来源：http://hz.snrcjt.cn/gtwvgdythj.html

[T17] Swift：变量与常量
来源：http://hz.meibo888.top/gtpjkwwgno.html

var a = 1;  let b = 2
来源：http://hz.yuanzhike.top/gtxehllfas.html

[T18] Swift：字符串插值
来源：http://hz.hnxiangtu.top/gtqkfhnybb.html

"值: \(b)"
来源：http://hz.meibo888.top/gtojixakuc.html

[T19] Swift：可选绑定
来源：http://hz.wangdashe.top/gtrjdebhwa.html

if let n = opt { print(n) }
来源：http://hz.daxiang520.top/gtetjdepng.html

[T20] Swift：数组操作
来源：http://hz.daxiang520.top/gtgmfpfbih.html

var a = [1, 2, 3];  a.append(4)
来源：http://hz.meibo888.top/gtoqkepqun.html

[T21] Swift：遍历
来源：http://hz.hywenlv.cn/gtgiulmuzk.html

for x in a { print(x) }
来源：http://hz.feifeiyinyue.top/gtfyhfsozd.html

[T22] Swift：字典
来源：http://hz.chenzaomai.com/gthypfufyc.html

var d = ["a": 1];  d["b"] = 2
来源：http://hz.hnqzz.top/gtqizsysdk.html

[T23] Swift：函数
来源：http://hz.jiagoushi.top/gtarlalpqa.html

func add(_ a: Int, _ b: Int) -> Int { a + b }
来源：http://hz.ydjk.org.cn/gtufkgwddi.html

[T24] Swift：闭包
来源：http://hz.guowangkeji.top/gtzkmzajkc.html

let f = { (x: Int) -> Int in x * 2 }
来源：http://hz.sysykeji.top/gtyqrhsecq.html

[T25] Swift：结构体
来源：http://hz.hfpthk.cn/gtefvgeuzq.html

struct P { var x: Int }
来源：http://hz.andypj.xyz/gtshuepudz.html

[T26] Swift：类与重写
来源：http://hz.pycfn.com/gtkxmlcswc.html

class A: Base { override func f() {} }
来源：http://hz.zdqjudy.top/gtgsllknva.html

[T27] Swift：错误处理
来源：http://hz.jinyuanbaomall.cn/gtewfrvtts.html

do { try f() } catch { print(error) }
来源：http://hz.zhaomingkeji.xyz/gtjsksujuc.html

[T28] Swift：枚举
来源：http://hz.guowangkeji.top/gtrbdyxphv.html

enum Color { case red, green }
来源：http://hz.ehwqpu.com/gtlbrfthwh.html

[T29] Swift：guard 提前返回
来源：http://hz.mhx1999.top/gtdgsduuxi.html

guard let x = opt else { return }
来源：http://hz.zhoulong.xyz/gtzqkymuus.html

[T30] Swift：协议
来源：http://hz.mhx1999.top/gtxochdrju.html

protocol Shape { func area() -> Double }
来源：http://hz.redwolf501.top/gtkcvmxjfi.html

[T31] Lua：Hello World
来源：http://hz.quarkkingdee.top/gtdalibauj.html

print("Hello")
来源：http://hz.zhijiandao.cn/gtrzwewave.html

[T32] Lua：局部变量
来源：http://hz.jiagoushi.top/gtxvrmfcgo.html

local a = 1
来源：http://hz.shanyushiyangtech.top/gtzpaibrbw.html

[T33] Lua：表（数组）
来源：http://hz.jiagoushi.top/gtwlulbwzr.html

local t = {1, 2, 3};  t[4] = 4
来源：http://hz.birdmap.top/gtxzywzqgu.html

[T34] Lua：遍历表
来源：http://hz.sufxvd.cn/gtwiyhkgeg.html

for i, v in ipairs(t) do print(i, v) end
来源：http://hz.guowangkeji.top/gtwchyvyql.html

[T35] Lua：字典表
来源：http://hz.daria6918.cn/gtzdmnxqmf.html

local d = { a = 1 };  d.b = 2
来源：http://hz.hongshengwenyu.top/gttzzholkw.html

[T36] Lua：函数
来源：http://hz.daxiang520.top/gtezywrkar.html

function add(a, b) return a + b end
来源：http://hz.cdnleiting.top/gtnsdlatvr.html

[T37] Lua：字符串拼接
来源：http://hz.pengpengdd.cyou/gtiqlfntpu.html

"a" .. "b"
来源：http://hz.cashguo.top/gtzbatwogq.html

[T38] Lua：条件
来源：http://hz.svipenyu.cn/gtaobjvoga.html

if x > 0 then print("正") end
来源：http://hz.gaohongyu789.top/gtnpnoczzy.html

[T39] Lua：模式匹配
来源：http://hz.jinqigufen.top/gtewglayza.html

string.find(s, "%d+")
来源：http://hz.zhongyouzk.top/gtwyapdfju.html

[T40] Lua：元表
来源：http://hz.hammf.cn/gtduikgglj.html

setmetatable({}, { __index = base })
来源：http://hz.hysaishi.cn/gtycantsbh.html

[T41] Perl：Hello World
来源：http://hz.52xcode.cn/gtryfowftv.html

print "Hello\n";
来源：http://hz.yj20258.top/gtfqrlfihk.html

[T42] Perl：变量类型
来源：http://hz.52xcode.cn/gtimetrpsg.html

my $a = 1;  my @arr = (1, 2, 3);  my %h = (a => 1);
来源：http://hz.yj20258.top/gttzoaonbr.html

[T43] Perl：字符串插值
来源：http://hz.jqgufenzy.top/gtfuoscdfr.html

"值: $a"
来源：http://hz.jinyuanbaomall.cn/gtdstfpqfi.html

[T44] Perl：条件
来源：http://hz.daxiang520.top/gtrrsukidp.html

if ($a > 0) { print "正"; }
来源：http://hz.ppjwa.cn/gtfumujfhi.html

[T45] Perl：数组遍历
来源：http://hz.hongshengwenyu.top/gtedqrnxyk.html

for my $x (@arr) { print $x; }
来源：http://hz.xylfe.cn/gtcjizswlb.html

[T46] Perl：哈希操作
来源：http://hz.jinqigufen.top/gtiprjesrw.html

$h{b} = 2;  for my $k (keys %h) { print "$k=$h{$k}"; }
来源：http://hz.nanxuanxn.top/gtkjmigcpe.html

[T47] Perl：正则捕获
来源：http://hz.yangfankeji.com/gtmffvubta.html

if ($s =~ /(\d+)/) { print $1; }
来源：http://hz.chenlongwang.top/gtctwfribg.html

[T48] Perl：正则替换
来源：http://hz.wangdashe.top/gtnwbobfgs.html

$s =~ s/old/new/g;
来源：http://hz.snrcjt.cn/gturivcpkm.html

[T49] Perl：函数
来源：http://hz.feifeiyinyue.top/gttloehoyk.html

sub add { my ($a, $b) = @_; return $a + $b; }
来源：http://hz.fzhhl.top/gtcwcabxkd.html

[T50] Perl：逐行读文件
来源：http://hz.gaohongyu789.top/gtvltaekxd.html

open my $fh, "<", "a.txt" or die $!;
来源：http://hz.jinqigufen.top/gtmlcpaseo.html

while (my $line = <$fh>) { print $line; }
来源：http://hz.guannengcc.top/gtrgndeyub.html

[T51] Scala：Hello World
来源：http://hz.xinyue.icu/gtppcleqlg.html

println("Hello")
来源：http://hz.zhiwuduotai.top/gttqcvfrvx.html

[T52] Scala：变量
来源：http://hz.dashuyun.cn/gtkhwmjsxn.html

val a = 1;  var b = 2
来源：http://hz.birdmap.top/gtcdjihuas.html

[T53] Scala：字符串插值
来源：http://hz.feifeiyinyue.top/gtnknydxkt.html

s"值: $b"
来源：http://hz.wangshuangyany.cn/gtgktudwjv.html

[T54] Scala：集合映射
来源：http://hz.mhx1999.top/gtvoqjnxhf.html

List(1, 2, 3).map(_ * 2)
来源：http://hz.zhongyouzk.top/gtomzikxyq.html

[T55] Scala：集合过滤
来源：http://hz.hysaishi.cn/gtzqgmccxe.html

List(1, 2, 3).filter(_ > 1)
来源：http://hz.xziqi.cn/gtkzjnrvtg.html

[T56] Scala：样例类
来源：http://hz.ywan-chungtsiang.top/gtahvbjyoa.html

case class User(name: String, age: Int)
来源：http://hz.yongpay.top/gtrmvfvplj.html

[T57] Scala：模式匹配
来源：http://hz.guowangkeji.top/gtpgnxgwql.html

x match { case 1 => "一"; case _ => "其他" }
来源：http://hz.tianlin.xyz/gtzhignucj.html

[T58] Scala：函数定义
来源：http://hz.aizwys.cn/gtkdwugqaa.html

def add(a: Int, b: Int): Int = a + b
来源：http://hz.316326.xyz/gtqscoyfzw.html

[T59] Scala：循环
来源：http://hz.pycfn.com/gttmzjazyc.html

for (i <- 1 to 10) println(i)
来源：http://hz.hongshengwenyu.top/gtpmuttewe.html

[T60] Scala：折叠
来源：http://hz.dianchejie.cn/gtejchiwdu.html

List(1, 2, 3).foldLeft(0)(_ + _)
来源：http://hz.yj202588.top/gtcgzkzxdy.html

================================================================================
来源：http://hz.smart0.xyz/gtyphkyyuo.html

U. 高频实用片段（Python / PHP / JavaScript 各 40 条）
来源：http://hz.jlsjyb.cn/gtehgububk.html

================================================================================
来源：http://hz.gotoacloud.top/gttohzcpvh.html

[U01] Py：创建虚拟环境
来源：http://hz.chenlongwang.top/gtpqqdukhx.html

python -m venv .venv && source .venv/bin/activate
来源：http://hz.guowangkeji.top/gtxngyaefc.html

[U02] Py：导出 / 安装依赖
来源：http://hz.xylfe.cn/gtdyzzvtsq.html

pip freeze > requirements.txt;  pip install -r requirements.txt
来源：http://hz.dianchejie.cn/gtjtfdozph.html

[U03] Py：加载 .env 配置
来源：http://hz.jinghuilouyu.cn/gtymysmmra.html

from dotenv import load_dotenv; load_dotenv()
来源：http://hz.shangyingyoupin.top/gtuqoipfxn.html

[U04] Py：变量调试打印
来源：http://hz.ehwqpu.com/gtjlnkeobn.html

print(f"{x=}")            # 输出 x=值，Python 3.8+
来源：http://hz.52xcode.cn/gtvafaraqc.html

[U05] Py：列表去重且保序
来源：http://hz.quarkkingdee.top/gttobeoyai.html

list(dict.fromkeys(arr))
来源：http://hz.jinghuilouyu.cn/gtnytgcgby.html

[U06] Py：合并两个字典
来源：http://hz.wangdashe.top/gtykskqbim.html

{**a, **b}
来源：http://hz.aizwys.cn/gttlfjreaj.html

[U07] Py：反转字典键值
来源：http://hz.quarkkingdee.top/gtoekrasjj.html

{v: k for k, v in d.items()}
来源：http://hz.chenlongwang.top/gtacycmcsp.html

[U08] Py：展平二维列表
来源：http://hz.shanyushiyangkeji.top/gtquihnhyu.html

[y for x in nested for y in x]
来源：http://hz.yongpay.top/gtiwnbtgkk.html

[U09] Py：字典取最大值的键
来源：http://hz.shzxlz.cn/gtmtgvewio.html

max(d, key=d.get)
来源：http://hz.aizwys.cn/gthgagpsds.html

[U10] Py：按值排序字典
来源：http://hz.cdnleiting.top/gtcdlmgxsh.html

dict(sorted(d.items(), key=lambda kv: kv[1]))
来源：http://hz.xuetiantiany.cn/gtzvaguzec.html

[U11] Py：生成器表达式
来源：http://hz.aizwys.cn/gtpviydkrh.html

(x * 2 for x in arr)
来源：http://hz.jlsjyb.cn/gtwzrbaggo.html

[U12] Py：取出现最多的 3 个元素
来源：http://hz.zhijiandao.cn/gtcxghuabh.html

Counter(arr).most_common(3)
来源：http://hz.shanyushiyangtech.top/gteehvskjx.html

[U13] Py：固定长度队列
来源：http://hz.pycfn.com/gtgdhamvkn.html

deque(maxlen=10)
来源：http://hz.yanxiufei.cn/gtvijgvhjq.html

[U14] Py：分组收集到列表
来源：http://hz.wangdashe.top/gtwoitnpie.html

defaultdict(list)
来源：http://hz.0kj1m.cn/gtfqcolfxa.html

[U15] Py：高精度计时
来源：http://hz.jinghuilouyu.cn/gtjzyjyuus.html

t = time.perf_counter()
来源：http://hz.shuidangran.top/gtdzrczpjd.html

[U16] Py：命令行参数解析
来源：http://hz.gotoacloud.top/gtobdxwnon.html

ap = argparse.ArgumentParser();  ap.add_argument("--name");  args = ap.parse_args()
来源：http://hz.jianghu66.top/gtsjuojavl.html

[U17] Py：初始化日志
来源：http://hz.hysaishi.cn/gtrqqhqwbp.html

logging.basicConfig(level=logging.INFO)
来源：http://hz.jinqigufen.top/gtqkvxwyei.html

[U18] Py：预编译正则
来源：http://hz.shuidangran.top/gtgwunsqyi.html

pat = re.compile(r"\d+")
来源：http://hz.yj202588.top/gtosmgvqlp.html

[U19] Py：正则替换带回调
来源：http://hz.andypj.xyz/gtulbslsxm.html

re.sub(r"\d+", lambda m: str(int(m.group()) * 2), s)
来源：http://hz.shangyingyoupin.top/gtxvjzhjzi.html

[U20] Py：缓存函数结果
来源：http://hz.jinqigfzy.top/gtbgtydcbr.html

@functools.lru_cache(maxsize=None)
来源：http://hz.dashuyun.cn/gthvhhhmrq.html

[U21] Py：自定义上下文管理器
来源：http://hz.chenzaomai.com/gtdzeneebq.html

@contextlib.contextmanager
来源：http://hz.xinyue.icu/gtjioldiac.html

[U22] Py：矩阵转置
来源：http://hz.sxryk.cn/gtskraxkha.html

list(zip(*m))
来源：http://hz.vqdsnc.cn/gtcmhsmwfc.html

[U23] Py：分块读取大文件
来源：http://hz.0kj1m.cn/gtynwwlznw.html

for chunk in iter(lambda: f.read(8192), b""):
来源：http://hz.xuanzx.com/gtoirinebb.html

[U24] Py：路径操作
来源：http://hz.wangshuangyany.cn/gtfahdmvdk.html

Path("a/b.txt").parent.mkdir(parents=True, exist_ok=True)
来源：http://hz.redwolf501.top/gtbojmlaez.html

[U25] Py：CSV 按字典读
来源：http://hz.ydzc1.top/gtndfckfsv.html

csv.DictReader(f)
来源：http://hz.daxiang520.top/gtddoiimbg.html

[U26] Py：并发下载
来源：http://hz.ybcxt.top/gttlrpfpeb.html

ThreadPoolExecutor(max_workers=8).map(fetch, urls)
来源：http://hz.pycfn.com/gtrrocslmz.html

[U27] Py：异步 HTTP
来源：http://hz.feifeiyinyue.top/gtecgezjlh.html

aiohttp.ClientSession() 配合 async with
来源：http://hz.jyoumei.cn/gtjzggcchb.html

[U28] Py：类型别名
来源：http://hz.daria6918.cn/gtqwskpqcs.html

UserId = int
来源：http://hz.andypj.xyz/gtlxnneeju.html

[U29] Py：属性校验
来源：http://hz.zhiwuduotai.top/gtgdlawcse.html

@property 与 @x.setter 配合
来源：http://hz.snrcjt.cn/gtwxlcedct.html

[U30] Py：数据类
来源：http://hz.wangshuangyany.cn/gtezhnjpvo.html

@dataclass(slots=True)
来源：http://hz.hfpthk.cn/gtckxouaec.html

[U31] Py：单测
来源：http://hz.sufxvd.cn/gtfswynsee.html

python -m pytest -q
来源：http://hz.cashguo.top/gtsbuypkcs.html

[U32] Py：代码格式化
来源：http://hz.chenjidiqi.icu/gtirgguaka.html

ruff format . && ruff check --fix .
来源：http://hz.yuxming.cn/gtbxjukabm.html

[U33] Py：打包发布
来源：http://hz.hysaishi.cn/gtmhmjjavq.html

python -m build  （依赖 pyproject.toml）
来源：http://hz.vqdsnc.cn/gtgahihceo.html

[U34] Py：判断编码
来源：http://hz.cucudq.cn/gtnvfbhsgx.html

chardet.detect(raw)
来源：http://hz.9152youxi.cn/gtvcuwecku.html

[U35] Py：发送邮件
来源：http://hz.snrcjt.cn/gttbitcfql.html

smtplib.SMTP_SSL(...).send_message(msg)
来源：http://hz.tanke756.top/gtrqwjmhpf.html

[U36] Py：定时任务
来源：http://hz.c1oappe.top/gtxlqywzhj.html

schedule.every(10).minutes.do(job)
来源：http://hz.jqgfzy.top/gtzxxllwwk.html

[U37] Py：读写 Excel
来源：http://hz.tian-w.cn/gtjgwbqxrg.html

pandas.read_excel / DataFrame.to_excel
来源：http://hz.shanyushiyangtech.top/gtvfchwxme.html

[U38] Py：获取脚本所在目录
来源：http://hz.xingfuxueyuan.xyz/gthgyepyfx.html

Path(__file__).resolve().parent
来源：http://hz.chenlongwang.top/gtclipfdtz.html

[U39] Py：判断是否在交互环境
来源：http://hz.zhengqikj.top/gtgtxfxoti.html

sys.stdout.isatty()
来源：http://hz.tian-w.cn/gtbtddgnad.html

[U40] Py：打印到标准错误
来源：http://hz.hnxiangtu.top/gtqtobmlfe.html

print("err", file=sys.stderr)
来源：http://hz.yj202588.top/gtqgkeauru.html

[U41] PHP：初始化 Composer 项目
来源：http://hz.xinyue.icu/gtdlaqmlnx.html

composer init;  composer require guzzlehttp/guzzle
来源：http://hz.nanxinkj.top/gtpljozdop.html

[U42] PHP：PSR-4 自动加载
来源：http://hz.wangshuangyany.cn/gtwvbfthgb.html

"autoload": { "psr-4": { "App\\": "src/" } }
来源：http://hz.xingfuxueyuan.xyz/gtdierfxnv.html

[U43] PHP：声明命名空间
来源：http://hz.ppjwa.cn/gtuppimlyh.html

namespace App\Http;
来源：http://hz.sxryk.cn/gtqgvkihmw.html

[U44] PHP：开启严格类型
来源：http://hz.feifeiyinyue.top/gtavtcvzpb.html

declare(strict_types=1);
来源：http://hz.ybcxt.top/gtptyirerd.html


<!-- 参考信息 -->