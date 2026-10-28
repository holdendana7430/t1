代发 wailian999

atoi("42");  strtod("3.14", NULL);
来源：http://hz.pengpengdd.cyou/gtsnmxpydp.html

[S23] C：随机数
来源：http://hz.cdnleiting.top/gtajwlzrmk.html

srand(time(NULL));  int r = rand() % 100;
来源：http://hz.gogol.net.cn/gtvbvrxdem.html

[S24] C：获取本地时间
来源：http://hz.jlsjyb.cn/gtsmoulgwo.html

time_t t = time(NULL);  struct tm *tm = localtime(&t);
来源：http://hz.ehwqpu.com/gtfonzzprp.html

[S25] C：内存拷贝
来源：http://hz.zhengqikj.top/gtgiuowido.html

memcpy(dst, src, n);
来源：http://hz.jinghuilouyu.cn/gtpovhhkib.html

[S26] C：内存清零
来源：http://hz.svipenyu.cn/gtwiyiqpsg.html

memset(a, 0, sizeof a);
来源：http://hz.nanxuanxn.top/gtsfymblgd.html

[S27] C：定义常量
来源：http://hz.zhaomingkeji.xyz/gtofhoovjc.html

const double PI = 3.14159;
来源：http://hz.hfpthk.cn/gtpfxwprjt.html

[S28] C：静态变量
来源：http://hz.fzhhl.top/gttojdkova.html

static int counter = 0;
来源：http://hz.316326.xyz/gtqmajucvg.html

[S29] C：变参函数
来源：http://hz.iojbl.cn/gtlgpugqcl.html

va_list ap; va_start(ap, fmt); vprintf(fmt, ap); va_end(ap);
来源：http://hz.yueranfly.top/gtzdafqkhc.html

[S30] C：头文件保护
来源：http://hz.hfpthk.cn/gtadujtwgk.html

#ifndef X_H
来源：http://hz.sweek.top/gtcbepvflw.html

#define X_H
来源：http://hz.dianchejie.cn/gtgkpjlyxw.html

#endif
来源：http://hz.vqdsnc.cn/gtrthmozji.html

[S31] C++：Hello World
来源：http://hz.cqqwz.cn/gtefjfdwpm.html

#include <iostream>
来源：http://hz.hongshengwenyu.top/gticpcokev.html

int main() { std::cout << "Hello\n"; }
来源：http://hz.zhongyouzk.top/gtzrfouhhj.html

[S32] C++：字符串
来源：http://hz.zhaomingkeji.xyz/gtzelnaldv.html

std::string s = "hi";  s += "!";
来源：http://hz.316326.xyz/gtaxsbnlja.html

[S33] C++：vector 增删
来源：http://hz.hywenlv.cn/gtqpkwyhtq.html

std::vector<int> v{1, 2, 3};  v.push_back(4);
来源：http://hz.jianghu66.top/gtbhpgljbo.html

[S34] C++：遍历 vector
来源：http://hz.ydjk.org.cn/gtmbdpwmfr.html

for (auto &x : v) { std::cout << x; }
来源：http://hz.shanyushiyangtech.top/gteqnfinoq.html

[S35] C++：map
来源：http://hz.aizwys.cn/gticrqwnps.html

std::map<std::string, int> m;  m["a"] = 1;
来源：http://hz.jlsjyb.cn/gtnnohjefm.html

[S36] C++：unordered_map
来源：http://hz.yj202588.top/gtejetuyku.html

std::unordered_map<std::string, int> m;  m["a"] = 1;
来源：http://hz.jlsjyb.cn/gtelngznxe.html

[S37] C++：set
来源：http://hz.jinghuilouyu.cn/gtuhqxpsvn.html

std::set<int> s{1, 2, 3};  s.insert(4);
来源：http://hz.sxryk.cn/gtlrzxsjap.html

[S38] C++：排序
来源：http://hz.sxryk.cn/gttblvywor.html

std::sort(v.begin(), v.end());
来源：http://hz.sufxvd.cn/gthandvvtn.html

[S39] C++：自定义比较器排序
来源：http://hz.svipenyu.cn/gtplqoxziw.html

std::sort(v.begin(), v.end(), [](int a, int b) { return a > b; });
来源：http://hz.hysaishi.cn/gteklluajy.html

[S40] C++：查找元素
来源：http://hz.tanke756.top/gtbwdtcgln.html

auto it = std::find(v.begin(), v.end(), 3);
来源：http://hz.havefunace.top/gtcgwnrzbx.html

[S41] C++：类与构造函数
来源：http://hz.yvedp.cn/gtbleopkhv.html

class A { public: A(int v) : x_(v) {} int get() const { return x_; } private: int x_; };
来源：http://hz.nwbrower.top/gtmerjwfwf.html

[S42] C++：继承与虚函数
来源：http://hz.bjfxy.top/gtvzkqbwdc.html

class B : public Base { public: void f() override {} };
来源：http://hz.zhongyouzk.top/gtdnqlokuq.html

[S43] C++：智能指针
来源：http://hz.hfpthk.cn/gtpxqpizvw.html

auto p = std::make_unique<int>(5);
来源：http://hz.sysykeji.top/gtlywzhdfj.html

[S44] C++：引用传参
来源：http://hz.wangshuangyany.cn/gtbnvifgbm.html

void inc(int &x) { ++x; }
来源：http://hz.zdqjudy.top/gtphtkkvep.html

[S45] C++：lambda
来源：http://hz.gzhubu.top/gtrlfwpiky.html

auto add = [](int a, int b) { return a + b; };
来源：http://hz.pengpengdd.cyou/gtvfztvntr.html

[S46] C++：函数模板
来源：http://hz.aizwys.cn/gttaypzkka.html

template <typename T> T maxv(T a, T b) { return a > b ? a : b; }
来源：http://hz.haohaochexian.top/gtafjgejws.html

[S47] C++：结构化绑定遍历
来源：http://hz.52xcode.cn/gtfuykhnug.html

for (const auto &[k, v] : m) { std::cout << k << v; }
来源：http://hz.andypj.xyz/gtrrhrdgbf.html

[S48] C++：逐行读文件
来源：http://hz.shanyushiyangkeji.top/gtlpbsdsxt.html

std::ifstream in("a.txt");  std::string line;
来源：http://hz.yj20258888.top/gtuglmftgf.html

while (std::getline(in, line)) { }
来源：http://hz.hywenlv.cn/gtumbzlwgq.html

[S49] C++：写文件
来源：http://hz.yuxming.cn/gtrnhzlltk.html

std::ofstream out("a.txt");  out << "hi\n";
来源：http://hz.52xcode.cn/gtgavajdbc.html

[S50] C++：格式化数字
来源：http://hz.xingfuxueyuan.xyz/gtoobbcdua.html

std::ostringstream os;  os << std::fixed << std::setprecision(2) << 3.14159;
来源：http://hz.shzxlz.cn/gtvgoqrsts.html

[S51] C++：显式类型转换
来源：http://hz.9152youxi.cn/gtpcimkqjk.html

static_cast<double>(a) / b
来源：http://hz.zhaomingkeji.xyz/gthyenzuem.html

[S52] C++：const 与 noexcept
来源：http://hz.xingfuxueyuan.xyz/gtfgixslxq.html

int size() const noexcept { return n_; }
来源：http://hz.quarkkingdee.top/gtdtelohvb.html

[S53] C++：移动语义
来源：http://hz.hammf.cn/gtophpvdkp.html

std::vector<int> w = std::move(v);
来源：http://hz.hnqzz.top/gtnzfirgwy.html

[S54] C++：异常处理
来源：http://hz.sxryk.cn/gtfckalcjp.html

try { throw std::runtime_error("x"); } catch (const std::exception &e) { }
来源：http://hz.ybcxt.top/gtaegyrgur.html

[S55] C++：结构化绑定
来源：http://hz.hammf.cn/gtyzohzpwy.html

auto [a, b] = std::make_pair(1, 2);
来源：http://hz.haohaochexian.top/gtuafnwyut.html

[S56] C++：optional
来源：http://hz.hysaishi.cn/gtyhgawxjg.html

std::optional<int> o = 5;  if (o) { int v = *o; }
来源：http://hz.gogol.net.cn/gteprdrbmy.html

[S57] C++：编译期常量
来源：http://hz.gotoacloud.top/gtmclvizyp.html

constexpr int N = 10;
来源：http://hz.shanyushiyangtech.top/gtnvppijkq.html

[S58] C++：命名空间
来源：http://hz.wangshuangyany.cn/gtnlpehvne.html

namespace ns { int f() { return 1; } }
来源：http://hz.hnqzz.top/gtjzthglug.html

[S59] C++：静态断言
来源：http://hz.ydzc1.top/gtwuwxilhs.html

static_assert(sizeof(int) == 4, "int 必须 4 字节");
来源：http://hz.zdqjudy.top/gtbgnndaqs.html

[S60] C++：遍历并删除元素
来源：http://hz.quarkkingdee.top/gtfnmvitmf.html

v.erase(std::remove_if(v.begin(), v.end(), [](int x) { return x < 0; }), v.end());
来源：http://hz.nanxuanxn.top/gtakzybghg.html

================================================================================
来源：http://hz.svipenyu.cn/gtxzvprahi.html

T. 其他语言补充（Kotlin / Swift / Lua / Perl / Scala）
来源：http://hz.yvedp.cn/gtbupgwrsc.html

================================================================================
来源：http://hz.ppjwa.cn/gtyxqdushr.html

[T01] Kotlin：Hello World
来源：http://hz.tianlin.xyz/gtuqexysmb.html

println("Hello")
来源：http://hz.cucudq.cn/gtjasrfjhp.html

[T02] Kotlin：变量
来源：http://hz.gotoacloud.top/gtzbytqonu.html

val a = 1;  var b = 2        // val 只读，var 可变
来源：http://hz.hywenlv.cn/gthqqdaraj.html

[T03] Kotlin：字符串模板
来源：http://hz.snrcjt.cn/gtnknmjepc.html

"值: $b"
来源：http://hz.nwbrower.top/gtwlnbvriy.html

[T04] Kotlin：空安全
来源：http://hz.jyoumei.cn/gtkwvzcmsi.html

val n: String? = null;  n?.length
来源：http://hz.jqgufenzy.top/gtqyfgshtf.html

[T05] Kotlin：when 表达式
来源：http://hz.ydjk.org.cn/gtjhrkwckk.html

val s = when (x) { 1 -> "一" else -> "其他" }   // 多分支时每个分支单独一行
来源：http://hz.gogol.net.cn/gtbtawbaoj.html

[T06] Kotlin：集合映射
来源：http://hz.xingfuxueyuan.xyz/gtcysmmfyv.html

listOf(1, 2, 3).map { it * 2 }
来源：http://hz.ydzc1.top/gthimtmtgn.html

[T07] Kotlin：集合过滤
来源：http://hz.jqgufenzy.top/gtejkfqfjf.html

listOf(1, 2, 3).filter { it > 1 }
来源：http://hz.yj202588.top/gtsbqqyzul.html

[T08] Kotlin：数据类
来源：http://hz.zhengqikj.top/gturetzeet.html

data class User(val name: String, val age: Int)
来源：http://hz.gotoacloud.top/gtxkjvcasp.html

[T09] Kotlin：扩展函数
来源：http://hz.nanxuanxn.top/gtbxusderu.html

fun String.exclaim() = this + "!"
来源：http://hz.yonumen.top/gtgspkczsc.html

[T10] Kotlin：默认参数
来源：http://hz.sufxvd.cn/gtgaxlkmtw.html

fun greet(name: String = "World") = "Hi $name"
来源：http://hz.0kj1m.cn/gtrcxduzfe.html

[T11] Kotlin：协程
来源：http://hz.chenjidiqi.icu/gtriifffer.html

GlobalScope.launch { delay(1000); println("done") }
来源：http://hz.jinghuilouyu.cn/gtdgiuoosb.html

[T12] Kotlin：解构声明
来源：http://hz.yuanzhike.top/gtdkstysiz.html

val (a, b) = Pair(1, 2)
来源：http://hz.iojbl.cn/gtpfqbglyo.html

[T13] Kotlin：只读 Map
来源：http://hz.smart0.xyz/gtzesailfs.html

val m = mapOf("a" to 1)
来源：http://hz.xylfe.cn/gtytxobbds.html

[T14] Kotlin：循环
来源：http://hz.fengsongda.top/gthmmowhoq.html

for (i in 1..10) println(i)
来源：http://hz.hongshengwenyu.top/gtjovsdbng.html

[T15] Kotlin：接口
来源：http://hz.tian-w.cn/gtongwzdrm.html

interface Shape { fun area(): Double }
来源：http://hz.chenzaomai.com/gttqcmlkei.html

[T16] Swift：Hello World
来源：http://hz.xuetiantiany.cn/gtxfbdvidr.html

print("Hello")
来源：http://hz.jianghu66.top/gtcetfcqez.html

[T17] Swift：变量与常量
来源：http://hz.ywan-chungtsiang.top/gtrintlokv.html

var a = 1;  let b = 2
来源：http://hz.daria6918.cn/gtuypoemtn.html

[T18] Swift：字符串插值
来源：http://hz.sufxvd.cn/gtwbmnlpzz.html

"值: \(b)"
来源：http://hz.jiagoushi.top/gtcwlwpzgp.html

[T19] Swift：可选绑定
来源：http://hz.jqgfzy.top/gtuqkktors.html

if let n = opt { print(n) }
来源：http://hz.zhijiandao.cn/gtmugydqxk.html

[T20] Swift：数组操作
来源：http://hz.mhx1999.top/gtjcqxhtiu.html

var a = [1, 2, 3];  a.append(4)
来源：http://hz.cashguo.top/gtcybelsjh.html

[T21] Swift：遍历
来源：http://hz.chenjidiqi.icu/gtuewqbqon.html

for x in a { print(x) }
来源：http://hz.gaohongyu789.top/gtptaxirdf.html

[T22] Swift：字典
来源：http://hz.guowangkeji.top/gtvgaiwsao.html

var d = ["a": 1];  d["b"] = 2
来源：http://hz.bjfxy.top/gtviszvilg.html

[T23] Swift：函数
来源：http://hz.pycfn.com/gtrehanvpr.html

func add(_ a: Int, _ b: Int) -> Int { a + b }
来源：http://hz.zhixingplan.top/gtzngcgcaz.html

[T24] Swift：闭包
来源：http://hz.yangfankeji.com/gtyxemgsuv.html

let f = { (x: Int) -> Int in x * 2 }
来源：http://hz.nanxuanxn.top/gtcfuscjht.html

[T25] Swift：结构体
来源：http://hz.xziqi.cn/gtvhaonfgt.html

struct P { var x: Int }
来源：http://hz.xuetiantiany.cn/gtgoqgviba.html

[T26] Swift：类与重写
来源：http://hz.jqgfzy.top/gtnclpkafr.html

class A: Base { override func f() {} }
来源：http://hz.ywan-chungtsiang.top/gtcxmyyoke.html

[T27] Swift：错误处理
来源：http://hz.xylfe.cn/gtwycmpyuf.html

do { try f() } catch { print(error) }
来源：http://hz.c1oappe.top/gtdcnbauwj.html

[T28] Swift：枚举
来源：http://hz.mhx1999.top/gtmatnyopn.html

enum Color { case red, green }
来源：http://hz.xuanzx.com/gtatviuwgy.html

[T29] Swift：guard 提前返回
来源：http://hz.birdmap.top/gtiznhpoin.html

guard let x = opt else { return }
来源：http://hz.jyoumei.cn/gtthvbhpvf.html

[T30] Swift：协议
来源：http://hz.ehwqpu.com/gtyxwfkdsr.html

protocol Shape { func area() -> Double }
来源：http://hz.316326.xyz/gtbpnvffnn.html

[T31] Lua：Hello World
来源：http://hz.gzhubu.top/gtpqztaepr.html

print("Hello")
来源：http://hz.c1oappe.top/gtiikrjsmm.html

[T32] Lua：局部变量
来源：http://hz.nwbrower.top/gtrlsrcbqe.html

local a = 1
来源：http://hz.shangyingyoupin.top/gtrkkswuer.html

[T33] Lua：表（数组）
来源：http://hz.jinqigufen.top/gtlfvgrayq.html

local t = {1, 2, 3};  t[4] = 4
来源：http://hz.redwolf501.top/gtelhdzozi.html

[T34] Lua：遍历表
来源：http://hz.fengsongda.top/gtpkkyyjer.html

for i, v in ipairs(t) do print(i, v) end
来源：http://hz.jqgfzy.top/gtzaxceaqj.html

[T35] Lua：字典表
来源：http://hz.xinyue.icu/gtyraqewyr.html

local d = { a = 1 };  d.b = 2
来源：http://hz.jinqigfzy.top/gtdwhbqoaj.html

[T36] Lua：函数
来源：http://hz.ivvv.top/gtybplsdfa.html

function add(a, b) return a + b end
来源：http://hz.birdmap.top/gtsfxowehj.html

[T37] Lua：字符串拼接
来源：http://hz.zhoulong.xyz/gtohdelexl.html

"a" .. "b"
来源：http://hz.svipenyu.cn/gtaqncolbr.html

[T38] Lua：条件
来源：http://hz.cucudq.cn/gtqnlfbrcl.html

if x > 0 then print("正") end
来源：http://hz.andypj.xyz/gtegnxrwdv.html

[T39] Lua：模式匹配
来源：http://hz.guowangkeji.top/gtthuabxzv.html

string.find(s, "%d+")
来源：http://hz.jianghu66.top/gtkvfmdmyp.html

[T40] Lua：元表
来源：http://hz.tanke756.top/gtpgdqmrhs.html

setmetatable({}, { __index = base })
来源：http://hz.tanke756.top/gtkmcukawf.html

[T41] Perl：Hello World
来源：http://hz.yueranfly.top/gtgejiwcon.html

print "Hello\n";
来源：http://hz.xziqi.cn/gtijfqfxgn.html

[T42] Perl：变量类型
来源：http://hz.hammf.cn/gtuovxjnym.html

my $a = 1;  my @arr = (1, 2, 3);  my %h = (a => 1);
来源：http://hz.shangyingyoupin.top/gtaljlouhb.html

[T43] Perl：字符串插值
来源：http://hz.ivvv.top/gtbaaljqxw.html

"值: $a"
来源：http://hz.aizwys.cn/gtpowijxey.html

[T44] Perl：条件
来源：http://hz.jianghu66.top/gtbmvghekh.html

if ($a > 0) { print "正"; }
来源：http://hz.dianchejie.cn/gtzzbyofyx.html

[T45] Perl：数组遍历
来源：http://hz.jqgufenzy.top/gtgyrnvmgz.html

for my $x (@arr) { print $x; }
来源：http://hz.mhx1999.top/gtomfymthj.html

[T46] Perl：哈希操作
来源：http://hz.bjfxy.top/gtgytzjcvg.html

$h{b} = 2;  for my $k (keys %h) { print "$k=$h{$k}"; }
来源：http://hz.0kj1m.cn/gtvmfiqgrt.html

[T47] Perl：正则捕获
来源：http://hz.fzhhl.top/gtdjhxyuzj.html

if ($s =~ /(\d+)/) { print $1; }
来源：http://hz.nanxuanxn.top/gtsvpkubxl.html

[T48] Perl：正则替换
来源：http://hz.hnxiangtu.top/gtykaeacov.html

$s =~ s/old/new/g;
来源：http://hz.pengpengdd.cyou/gtdyrbiamx.html

[T49] Perl：函数
来源：http://hz.cqqwz.cn/gthmelodrf.html

sub add { my ($a, $b) = @_; return $a + $b; }
来源：http://hz.yj20258.top/gtjohtzmcl.html

[T50] Perl：逐行读文件
来源：http://hz.yanxiufei.cn/gthlwzxckf.html

open my $fh, "<", "a.txt" or die $!;
来源：http://hz.bjfxy.top/gtyavdwmey.html

while (my $line = <$fh>) { print $line; }
来源：http://hz.bjfxy.top/gtzpsypdtu.html

[T51] Scala：Hello World
来源：http://hz.0kj1m.cn/gtwqtzgnvx.html

println("Hello")
来源：http://hz.jqgufenzy.top/gtsepgdmps.html

[T52] Scala：变量
来源：http://hz.yangfankeji.com/gtptpyfysr.html

val a = 1;  var b = 2
来源：http://hz.zhaomingkeji.xyz/gtvzqzhfpi.html

[T53] Scala：字符串插值
来源：http://hz.jlsjyb.cn/gtnbezyorl.html

s"值: $b"
来源：http://hz.ybcxt.top/gtriorgarf.html

[T54] Scala：集合映射
来源：http://hz.cheryme.top/gtvdumfssn.html

List(1, 2, 3).map(_ * 2)
来源：http://hz.wangdashe.top/gtkzgzxirz.html

[T55] Scala：集合过滤
来源：http://hz.guannengcc.top/gtihywlwqq.html

List(1, 2, 3).filter(_ > 1)
来源：http://hz.zhixingplan.top/gtgzcavahz.html

[T56] Scala：样例类
来源：http://hz.cqqwz.cn/gtcjdxpujm.html

case class User(name: String, age: Int)
来源：http://hz.shuidangran.top/gtvfsnnsde.html

[T57] Scala：模式匹配
来源：http://hz.guowangkeji.top/gtfrwvxcir.html

x match { case 1 => "一"; case _ => "其他" }
来源：http://hz.yuxming.cn/gtvjopupcu.html

[T58] Scala：函数定义
来源：http://hz.cdnleiting.top/gtrrupalhp.html

def add(a: Int, b: Int): Int = a + b
来源：http://hz.chenjidiqi.icu/gtxyvzzxaa.html

[T59] Scala：循环
来源：http://hz.jiagoushi.top/gtfwplydpo.html

for (i <- 1 to 10) println(i)
来源：http://hz.zhijiandao.cn/gtzjcvjnrj.html

[T60] Scala：折叠
来源：http://hz.zhengqikj.top/gtardileoj.html

List(1, 2, 3).foldLeft(0)(_ + _)
来源：http://hz.haohaochexian.top/gtcsseywyl.html

================================================================================
来源：http://hz.yj202588.top/gtivjyuuph.html

U. 高频实用片段（Python / PHP / JavaScript 各 40 条）
来源：http://hz.snrcjt.cn/gtoaosbczi.html

================================================================================
来源：http://hz.haohaochexian.top/gtalgqkewv.html

[U01] Py：创建虚拟环境
来源：http://hz.smart0.xyz/gtgwmfqubh.html

python -m venv .venv && source .venv/bin/activate
来源：http://hz.havefunace.top/gtvkjnkznz.html

[U02] Py：导出 / 安装依赖
来源：http://hz.nanxuanxn.top/gtzddpdhva.html

pip freeze > requirements.txt;  pip install -r requirements.txt
来源：http://hz.iojbl.cn/gtziqnsegj.html

[U03] Py：加载 .env 配置
来源：http://hz.feifeiyinyue.top/gtckklialq.html

from dotenv import load_dotenv; load_dotenv()
来源：http://hz.xylfe.cn/gtrqlxhzmn.html

[U04] Py：变量调试打印
来源：http://hz.jinqigfzy.top/gtdjakojxa.html

print(f"{x=}")            # 输出 x=值，Python 3.8+
来源：http://hz.jinyuanbaomall.cn/gtccfgutfj.html

[U05] Py：列表去重且保序
来源：http://hz.hammf.cn/gtmzbsliqj.html

list(dict.fromkeys(arr))
来源：http://hz.tanke756.top/gtnkbvksps.html

[U06] Py：合并两个字典
来源：http://hz.hnxiangtu.top/gtdexghbfc.html

{**a, **b}
来源：http://hz.jqgufenzy.top/gthdsbxjns.html

[U07] Py：反转字典键值
来源：http://hz.chenzaomai.com/gtjhhmdlpp.html

{v: k for k, v in d.items()}
来源：http://hz.haohaochexian.top/gtwnefsyfu.html

[U08] Py：展平二维列表
来源：http://hz.aizwys.cn/gtaboqdltz.html

[y for x in nested for y in x]
来源：http://hz.yanxiufei.cn/gtgewosvcb.html

[U09] Py：字典取最大值的键
来源：http://hz.c1oappe.top/gtmqculgwg.html

max(d, key=d.get)
来源：http://hz.sxryk.cn/gtyhdqrmpr.html

[U10] Py：按值排序字典
来源：http://hz.xingfuxueyuan.xyz/gtdeeecpsy.html

dict(sorted(d.items(), key=lambda kv: kv[1]))
来源：http://hz.birdmap.top/gtnthohifm.html

[U11] Py：生成器表达式
来源：http://hz.nanxuanxn.top/gtxdnoiowj.html

(x * 2 for x in arr)
来源：http://hz.ehwqpu.com/gtcokmsmcj.html

[U12] Py：取出现最多的 3 个元素
来源：http://hz.0kj1m.cn/gttxmditoi.html

Counter(arr).most_common(3)
来源：http://hz.chenlongwang.top/gtqytzjkln.html

[U13] Py：固定长度队列
来源：http://hz.smart0.xyz/gttqgrbahz.html

deque(maxlen=10)
来源：http://hz.shanyushiyangkeji.top/gtrmfnxlxl.html

[U14] Py：分组收集到列表
来源：http://hz.jianghu66.top/gtuyeeumfv.html

defaultdict(list)
来源：http://hz.tian-w.cn/gtuhznhtui.html

[U15] Py：高精度计时
来源：http://hz.yangfankeji.com/gtnhmzyydp.html

t = time.perf_counter()
来源：http://hz.yanxiufei.cn/gtaobontvk.html

[U16] Py：命令行参数解析
来源：http://hz.pengpengdd.cyou/gtzggbjwtn.html

ap = argparse.ArgumentParser();  ap.add_argument("--name");  args = ap.parse_args()
来源：http://hz.dashuyun.cn/gtrtqzrncq.html

[U17] Py：初始化日志
来源：http://hz.daxiang520.top/gtpymcbswf.html

logging.basicConfig(level=logging.INFO)
来源：http://hz.chenzaomai.com/gtbauejpsq.html

[U18] Py：预编译正则
来源：http://hz.yangfankeji.com/gtlgfivrvs.html

pat = re.compile(r"\d+")
来源：http://hz.zhengqikj.top/gttgupvdfi.html

[U19] Py：正则替换带回调
来源：http://hz.jianghu66.top/gtvfzaomur.html

re.sub(r"\d+", lambda m: str(int(m.group()) * 2), s)
来源：http://hz.shzxlz.cn/gtxayzvpft.html

[U20] Py：缓存函数结果
来源：http://hz.jianghu66.top/gtbjzxomfd.html

@functools.lru_cache(maxsize=None)
来源：http://hz.yj20258888.top/gtuahpteji.html

[U21] Py：自定义上下文管理器
来源：http://hz.gogol.net.cn/gthefxxoqq.html

@contextlib.contextmanager
来源：http://hz.meibo888.top/gthergorsd.html

[U22] Py：矩阵转置
来源：http://hz.meibo888.top/gtlgaahdvi.html

list(zip(*m))
来源：http://hz.ydjk.org.cn/gtcqrjlsgs.html

[U23] Py：分块读取大文件
来源：http://hz.chenjidiqi.icu/gteobydqfo.html

for chunk in iter(lambda: f.read(8192), b""):
来源：http://hz.birdmap.top/gtehuvdgtu.html

[U24] Py：路径操作
来源：http://hz.daxiang520.top/gtyifncxwb.html

Path("a/b.txt").parent.mkdir(parents=True, exist_ok=True)
来源：http://hz.haohaochexian.top/gteevshzdk.html

[U25] Py：CSV 按字典读
来源：http://hz.hammf.cn/gtbtmgmybk.html

csv.DictReader(f)
来源：http://hz.52xcode.cn/gthgdyoihe.html

[U26] Py：并发下载
来源：http://hz.hysaishi.cn/gtlrhpwndd.html

ThreadPoolExecutor(max_workers=8).map(fetch, urls)
来源：http://hz.hysaishi.cn/gtaunutbrn.html

[U27] Py：异步 HTTP
来源：http://hz.jinqigfzy.top/gtdhcbgwkb.html

aiohttp.ClientSession() 配合 async with
来源：http://hz.daria6918.cn/gtiyrshoul.html

[U28] Py：类型别名
来源：http://hz.sufxvd.cn/gtghsjuvye.html

UserId = int
来源：http://hz.xylfe.cn/gtuhhtjtil.html

[U29] Py：属性校验
来源：http://hz.ehwqpu.com/gtzpabsfug.html

@property 与 @x.setter 配合
来源：http://hz.yongpay.top/gtqcylbscb.html

[U30] Py：数据类
来源：http://hz.daria6918.cn/gtuzapqjxs.html

@dataclass(slots=True)
来源：http://hz.ehwqpu.com/gtfxjrjpun.html

[U31] Py：单测
来源：http://hz.zhijiandao.cn/gtronaifuk.html

python -m pytest -q
来源：http://hz.yueranfly.top/gtoqaqpcdl.html

[U32] Py：代码格式化
来源：http://hz.zhongyouzk.top/gtyzbytdjg.html

ruff format . && ruff check --fix .
来源：http://hz.zhaomingkeji.xyz/gtetcyiagg.html

[U33] Py：打包发布
来源：http://hz.gzhubu.top/gtubmgdawe.html

python -m build  （依赖 pyproject.toml）
来源：http://hz.tianlin.xyz/gtnhuswkql.html

[U34] Py：判断编码
来源：http://hz.xinyue.icu/gtmlgjqqlm.html

chardet.detect(raw)
来源：http://hz.ybcxt.top/gtkgbiivhi.html

[U35] Py：发送邮件
来源：http://hz.yvedp.cn/gtocffrinq.html

smtplib.SMTP_SSL(...).send_message(msg)
来源：http://hz.daxiang520.top/gtyeddqtwj.html

[U36] Py：定时任务
来源：http://hz.9152youxi.cn/gtnkmcunne.html

schedule.every(10).minutes.do(job)
来源：http://hz.yanxiufei.cn/gtruetpuhl.html

[U37] Py：读写 Excel
来源：http://hz.cucudq.cn/gtncnthxva.html

pandas.read_excel / DataFrame.to_excel
来源：http://hz.yangfankeji.com/gtystvdnmu.html

[U38] Py：获取脚本所在目录
来源：http://hz.kuanghao11.cn/gtokrpibgr.html

Path(__file__).resolve().parent
来源：http://hz.hfpthk.cn/gtdyztuwwu.html

[U39] Py：判断是否在交互环境
来源：http://hz.hysaishi.cn/gtzmuroydd.html

sys.stdout.isatty()
来源：http://hz.wangdashe.top/gtnwtcwuke.html

[U40] Py：打印到标准错误
来源：http://hz.mhx1999.top/gtxpwbvdpm.html

print("err", file=sys.stderr)
来源：http://hz.ppjwa.cn/gtisucbubr.html

[U41] PHP：初始化 Composer 项目
来源：http://hz.fzhhl.top/gtmhquwfzj.html

composer init;  composer require guzzlehttp/guzzle
来源：http://hz.zhongyouzk.top/gtpmitaqgi.html

[U42] PHP：PSR-4 自动加载
来源：http://hz.tian-w.cn/gtosuxdutf.html

"autoload": { "psr-4": { "App\\": "src/" } }
来源：http://hz.jinqigfzy.top/gtmzgtxelj.html

[U43] PHP：声明命名空间
来源：http://hz.daria6918.cn/gthqcceykz.html

namespace App\Http;
来源：http://hz.daria6918.cn/gtoieagtpn.html

[U44] PHP：开启严格类型
来源：http://hz.birdmap.top/gtacqswvxx.html

declare(strict_types=1);
来源：http://hz.yueranfly.top/gteugisnnt.html

[U45] PHP：类型声明与返回类型
来源：http://hz.0kj1m.cn/gtlmbhimpp.html

function add(int $a, int $b): int { return $a + $b; }
来源：http://hz.shanyushiyangkeji.top/gtkhdfkbri.html

[U46] PHP：可空类型
来源：http://hz.jlsjyb.cn/gttmxjxtbr.html

?string $name = null
来源：http://hz.vqdsnc.cn/gttsntgbfn.html


<!-- 参考信息 -->