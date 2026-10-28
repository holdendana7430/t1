代发 wailian999

#include <iostream>
来源：http://hz.shzxlz.cn/gttrnxcnpc.html

int main() { std::cout << "Hello\n"; }
来源：http://hz.zhiwuduotai.top/gtklclmfow.html

[S32] C++：字符串
来源：http://hz.sysykeji.top/gtcvxphtzm.html

std::string s = "hi";  s += "!";
来源：http://hz.chenlongwang.top/gtvrhwdntv.html

[S33] C++：vector 增删
来源：http://hz.wangdashe.top/gtsfmcrozc.html

std::vector<int> v{1, 2, 3};  v.push_back(4);
来源：http://hz.haohaochexian.top/gtumlsmied.html

[S34] C++：遍历 vector
来源：http://hz.zycfv.cn/gtilansfar.html

for (auto &x : v) { std::cout << x; }
来源：http://hz.mhx1999.top/gtvgipflqs.html

[S35] C++：map
来源：http://hz.meibo888.top/gtevewqfmf.html

std::map<std::string, int> m;  m["a"] = 1;
来源：http://hz.xuetiantiany.cn/gtzozvovci.html

[S36] C++：unordered_map
来源：http://hz.wangshuangyany.cn/gtnfbpmbzk.html

std::unordered_map<std::string, int> m;  m["a"] = 1;
来源：http://hz.kuanghao11.cn/gtdgdowsyg.html

[S37] C++：set
来源：http://hz.guowangkeji.top/gtsinppnax.html

std::set<int> s{1, 2, 3};  s.insert(4);
来源：http://hz.zhiwuduotai.top/gtlnefxlur.html

[S38] C++：排序
来源：http://hz.yvedp.cn/gtkgllbolt.html

std::sort(v.begin(), v.end());
来源：http://hz.yongpay.top/gtsofmzatz.html

[S39] C++：自定义比较器排序
来源：http://hz.jianghu66.top/gtaayltfrc.html

std::sort(v.begin(), v.end(), [](int a, int b) { return a > b; });
来源：http://hz.c1oappe.top/gtzemzyled.html

[S40] C++：查找元素
来源：http://hz.shangyingyoupin.top/gtrlalahif.html

auto it = std::find(v.begin(), v.end(), 3);
来源：http://hz.jinqigufen.top/gtumlxkiaf.html

[S41] C++：类与构造函数
来源：http://hz.meibo888.top/gtlnxuqwoa.html

class A { public: A(int v) : x_(v) {} int get() const { return x_; } private: int x_; };
来源：http://hz.zycfv.cn/gtyqzeaxdb.html

[S42] C++：继承与虚函数
来源：http://hz.jqgufenzy.top/gtokdabqlx.html

class B : public Base { public: void f() override {} };
来源：http://hz.snrcjt.cn/gtukcztlro.html

[S43] C++：智能指针
来源：http://hz.sweek.top/gtxrrjyzap.html

auto p = std::make_unique<int>(5);
来源：http://hz.hywenlv.cn/gtckvjebsh.html

[S44] C++：引用传参
来源：http://hz.shangyingyoupin.top/gtqmchanzt.html

void inc(int &x) { ++x; }
来源：http://hz.haohaochexian.top/gttzhzubld.html

[S45] C++：lambda
来源：http://hz.iojbl.cn/gtrnrbykxb.html

auto add = [](int a, int b) { return a + b; };
来源：http://hz.cheryme.top/gtjeqcbahv.html

[S46] C++：函数模板
来源：http://hz.yonumen.top/gtrumkbnnz.html

template <typename T> T maxv(T a, T b) { return a > b ? a : b; }
来源：http://hz.yanxiufei.cn/gtawgdntym.html

[S47] C++：结构化绑定遍历
来源：http://hz.jinyuanbaomall.cn/gtfityfriz.html

for (const auto &[k, v] : m) { std::cout << k << v; }
来源：http://hz.meibo888.top/gtmlcwlcyn.html

[S48] C++：逐行读文件
来源：http://hz.wangshuangyany.cn/gtrvfnxefr.html

std::ifstream in("a.txt");  std::string line;
来源：http://hz.xziqi.cn/gtccufbqjm.html

while (std::getline(in, line)) { }
来源：http://hz.yj20258.top/gtszzrqbwl.html

[S49] C++：写文件
来源：http://hz.yangfankeji.com/gtnqasrmgu.html

std::ofstream out("a.txt");  out << "hi\n";
来源：http://hz.yueranfly.top/gtqueaxtvc.html

[S50] C++：格式化数字
来源：http://hz.iojbl.cn/gtitugjgsl.html

std::ostringstream os;  os << std::fixed << std::setprecision(2) << 3.14159;
来源：http://hz.jyoumei.cn/gtfjymbcrx.html

[S51] C++：显式类型转换
来源：http://hz.redwolf501.top/gtktqnaftq.html

static_cast<double>(a) / b
来源：http://hz.yj202588.top/gtwohijewc.html

[S52] C++：const 与 noexcept
来源：http://hz.yangfankeji.com/gtcbyqjtev.html

int size() const noexcept { return n_; }
来源：http://hz.yongpay.top/gtcdzwlbjm.html

[S53] C++：移动语义
来源：http://hz.feifeiyinyue.top/gtxszokrfd.html

std::vector<int> w = std::move(v);
来源：http://hz.birdmap.top/gtqupvuigm.html

[S54] C++：异常处理
来源：http://hz.redwolf501.top/gtrwfpoald.html

try { throw std::runtime_error("x"); } catch (const std::exception &e) { }
来源：http://hz.zhixingplan.top/gtsiypqclq.html

[S55] C++：结构化绑定
来源：http://hz.andypj.xyz/gtpgigtuls.html

auto [a, b] = std::make_pair(1, 2);
来源：http://hz.aibaodan.cn/gtvuougbvc.html

[S56] C++：optional
来源：http://hz.zhongyouzk.top/gthmgochoc.html

std::optional<int> o = 5;  if (o) { int v = *o; }
来源：http://hz.kuanghao11.cn/gtloxglalv.html

[S57] C++：编译期常量
来源：http://hz.yj202588.top/gtuxbqdziq.html

constexpr int N = 10;
来源：http://hz.gzhubu.top/gtiholbdho.html

[S58] C++：命名空间
来源：http://hz.bjfxy.top/gtzqxhqxjz.html

namespace ns { int f() { return 1; } }
来源：http://hz.jlsjyb.cn/gttdxfcbnv.html

[S59] C++：静态断言
来源：http://hz.jinghuilouyu.cn/gtcvhqczvv.html

static_assert(sizeof(int) == 4, "int 必须 4 字节");
来源：http://hz.fzhhl.top/gtbgtcipai.html

[S60] C++：遍历并删除元素
来源：http://hz.hysaishi.cn/gtzwefcgnn.html

v.erase(std::remove_if(v.begin(), v.end(), [](int x) { return x < 0; }), v.end());
来源：http://hz.tian-w.cn/gtmcweoxqe.html

================================================================================
来源：http://hz.yj20258888.top/gturxwxsvf.html

T. 其他语言补充（Kotlin / Swift / Lua / Perl / Scala）
来源：http://hz.shuidangran.top/gthjhdzlha.html

================================================================================
来源：http://hz.ydjk.org.cn/gtywzrmrpc.html

[T01] Kotlin：Hello World
来源：http://hz.daxiang520.top/gtbmfzadpb.html

println("Hello")
来源：http://hz.cucudq.cn/gtbjipzase.html

[T02] Kotlin：变量
来源：http://hz.hnxiangtu.top/gtcqafrumi.html

val a = 1;  var b = 2        // val 只读，var 可变
来源：http://hz.zhengqikj.top/gtsdncgbmu.html

[T03] Kotlin：字符串模板
来源：http://hz.fengsongda.top/gtpnpzfaiq.html

"值: $b"
来源：http://hz.jyoumei.cn/gtkvnalnam.html

[T04] Kotlin：空安全
来源：http://hz.sweek.top/gttrzdpcvu.html

val n: String? = null;  n?.length
来源：http://hz.cdnleiting.top/gtgbbhrfof.html

[T05] Kotlin：when 表达式
来源：http://hz.yueranfly.top/gtjaiyvsjr.html

val s = when (x) { 1 -> "一" else -> "其他" }   // 多分支时每个分支单独一行
来源：http://hz.feifeiyinyue.top/gtukjaqeqo.html

[T06] Kotlin：集合映射
来源：http://hz.jqgufenzy.top/gtjmadwqto.html

listOf(1, 2, 3).map { it * 2 }
来源：http://hz.shanyushiyangkeji.top/gtusoqthfe.html

[T07] Kotlin：集合过滤
来源：http://hz.nanxinkj.top/gtyidxkxoj.html

listOf(1, 2, 3).filter { it > 1 }
来源：http://hz.jyoumei.cn/gtqhicgkdq.html

[T08] Kotlin：数据类
来源：http://hz.hywenlv.cn/gtggpfkwor.html

data class User(val name: String, val age: Int)
来源：http://hz.shanyushiyangtech.top/gtofornlgh.html

[T09] Kotlin：扩展函数
来源：http://hz.hnxiangtu.top/gtfokgniyd.html

fun String.exclaim() = this + "!"
来源：http://hz.gogol.net.cn/gtjdvkebcd.html

[T10] Kotlin：默认参数
来源：http://hz.hnxiangtu.top/gtugellemq.html

fun greet(name: String = "World") = "Hi $name"
来源：http://hz.guowangkeji.top/gtfyedcezp.html

[T11] Kotlin：协程
来源：http://hz.quarkkingdee.top/gteleaakaw.html

GlobalScope.launch { delay(1000); println("done") }
来源：http://hz.jinghuilouyu.cn/gtbqjauiwn.html

[T12] Kotlin：解构声明
来源：http://hz.xziqi.cn/gtsvegnaly.html

val (a, b) = Pair(1, 2)
来源：http://hz.316326.xyz/gtbuewwyxa.html

[T13] Kotlin：只读 Map
来源：http://hz.jiagoushi.top/gtmhocacti.html

val m = mapOf("a" to 1)
来源：http://hz.chenzaomai.com/gtgcbcuqrj.html

[T14] Kotlin：循环
来源：http://hz.cdnleiting.top/gtupqvgjpn.html

for (i in 1..10) println(i)
来源：http://hz.xziqi.cn/gtedfnhjzv.html

[T15] Kotlin：接口
来源：http://hz.dashuyun.cn/gtjlehhrjs.html

interface Shape { fun area(): Double }
来源：http://hz.chenzaomai.com/gthaniaffh.html

[T16] Swift：Hello World
来源：http://hz.pycfn.com/gtcwaqlsft.html

print("Hello")
来源：http://hz.redwolf501.top/gtzzqccvmm.html

[T17] Swift：变量与常量
来源：http://hz.hammf.cn/gtvxvxuogs.html

var a = 1;  let b = 2
来源：http://hz.pengpengdd.cyou/gtvyfcwtkt.html

[T18] Swift：字符串插值
来源：http://hz.redwolf501.top/gtclhpwygz.html

"值: \(b)"
来源：http://hz.hysaishi.cn/gtrempeefi.html

[T19] Swift：可选绑定
来源：http://hz.jinqigfzy.top/gthhliaufi.html

if let n = opt { print(n) }
来源：http://hz.ywan-chungtsiang.top/gtahheirde.html

[T20] Swift：数组操作
来源：http://hz.svipenyu.cn/gttifsscnb.html

var a = [1, 2, 3];  a.append(4)
来源：http://hz.fzhhl.top/gtrdsvsulh.html

[T21] Swift：遍历
来源：http://hz.iojbl.cn/gtaamwlxiu.html

for x in a { print(x) }
来源：http://hz.guannengcc.top/gtiejcjlle.html

[T22] Swift：字典
来源：http://hz.shzxlz.cn/gtmcxhlceu.html

var d = ["a": 1];  d["b"] = 2
来源：http://hz.fzhhl.top/gtwqepnlnx.html

[T23] Swift：函数
来源：http://hz.pycfn.com/gthujkibga.html

func add(_ a: Int, _ b: Int) -> Int { a + b }
来源：http://hz.gaohongyu789.top/gtodvdzhfu.html

[T24] Swift：闭包
来源：http://hz.gotoacloud.top/gthcvnbuiv.html

let f = { (x: Int) -> Int in x * 2 }
来源：http://hz.bjfxy.top/gtdddiuoms.html

[T25] Swift：结构体
来源：http://hz.jianghu66.top/gtewptpfky.html

struct P { var x: Int }
来源：http://hz.sufxvd.cn/gtkfqlajyj.html

[T26] Swift：类与重写
来源：http://hz.yj20258888.top/gtjvwdrqxs.html

class A: Base { override func f() {} }
来源：http://hz.xylfe.cn/gtijkorutx.html

[T27] Swift：错误处理
来源：http://hz.meibo888.top/gtfndyblop.html

do { try f() } catch { print(error) }
来源：http://hz.shzxlz.cn/gtuzvfexiy.html

[T28] Swift：枚举
来源：http://hz.iojbl.cn/gtyzquptcj.html

enum Color { case red, green }
来源：http://hz.tianlin.xyz/gtgbxkcemy.html

[T29] Swift：guard 提前返回
来源：http://hz.shanyushiyangtech.top/gthwamsauz.html

guard let x = opt else { return }
来源：http://hz.yueranfly.top/gtdbrcdjhl.html

[T30] Swift：协议
来源：http://hz.jqgfzy.top/gtildscmhq.html

protocol Shape { func area() -> Double }
来源：http://hz.shuidangran.top/gtadmzkcnj.html

[T31] Lua：Hello World
来源：http://hz.xuetiantiany.cn/gtvjyjwreb.html

print("Hello")
来源：http://hz.zhengqikj.top/gtkueezmeu.html

[T32] Lua：局部变量
来源：http://hz.yj202588.top/gtjjnhimmg.html

local a = 1
来源：http://hz.jinqigufen.top/gtbxpmsxlq.html

[T33] Lua：表（数组）
来源：http://hz.pycfn.com/gtqbcsmfia.html

local t = {1, 2, 3};  t[4] = 4
来源：http://hz.svipenyu.cn/gtwfswseap.html

[T34] Lua：遍历表
来源：http://hz.xylfe.cn/gtjoriyzlq.html

for i, v in ipairs(t) do print(i, v) end
来源：http://hz.jianghu66.top/gtqflhuzds.html

[T35] Lua：字典表
来源：http://hz.yonumen.top/gtphbpqszr.html

local d = { a = 1 };  d.b = 2
来源：http://hz.tianlin.xyz/gthnzuwijr.html

[T36] Lua：函数
来源：http://hz.hywenlv.cn/gtlmoodmvw.html

function add(a, b) return a + b end
来源：http://hz.jyoumei.cn/gtxpxmdrwj.html

[T37] Lua：字符串拼接
来源：http://hz.zhijiandao.cn/gtekytvjhr.html

"a" .. "b"
来源：http://hz.daxiang520.top/gtquknjxrj.html

[T38] Lua：条件
来源：http://hz.jqgufenzy.top/gtbhjiajod.html

if x > 0 then print("正") end
来源：http://hz.redwolf501.top/gtnjtaevqe.html

[T39] Lua：模式匹配
来源：http://hz.haohaochexian.top/gtcbgsmbad.html

string.find(s, "%d+")
来源：http://hz.shanyushiyangkeji.top/gttoygggvq.html

[T40] Lua：元表
来源：http://hz.chenzaomai.com/gtqwlirnvx.html

setmetatable({}, { __index = base })
来源：http://hz.xylfe.cn/gthaoauiju.html

[T41] Perl：Hello World
来源：http://hz.redwolf501.top/gtecdbloko.html

print "Hello\n";
来源：http://hz.yj202588.top/gtnormpstk.html

[T42] Perl：变量类型
来源：http://hz.aibaodan.cn/gtyrezesnu.html

my $a = 1;  my @arr = (1, 2, 3);  my %h = (a => 1);
来源：http://hz.zhixingplan.top/gtnanopqvt.html

[T43] Perl：字符串插值
来源：http://hz.cheryme.top/gtdcmnbily.html

"值: $a"
来源：http://hz.daxiang520.top/gtwtbhmwyu.html

[T44] Perl：条件
来源：http://hz.birdmap.top/gtwqkfddyb.html

if ($a > 0) { print "正"; }
来源：http://hz.zhaomingkeji.xyz/gtrlpnzzoo.html

[T45] Perl：数组遍历
来源：http://hz.fzhhl.top/gtvgpjszxg.html

for my $x (@arr) { print $x; }
来源：http://hz.gaohongyu789.top/gtmjdsnqil.html

[T46] Perl：哈希操作
来源：http://hz.ydjk.org.cn/gtmtemeweg.html

$h{b} = 2;  for my $k (keys %h) { print "$k=$h{$k}"; }
来源：http://hz.sxryk.cn/gtprscijgb.html

[T47] Perl：正则捕获
来源：http://hz.jianghu66.top/gtptxzzven.html

if ($s =~ /(\d+)/) { print $1; }
来源：http://hz.gogol.net.cn/gtoponbhwn.html

[T48] Perl：正则替换
来源：http://hz.snrcjt.cn/gtpmloemoo.html

$s =~ s/old/new/g;
来源：http://hz.shanyushiyangkeji.top/gtatptthzd.html

[T49] Perl：函数
来源：http://hz.pycfn.com/gtqpfvwacl.html

sub add { my ($a, $b) = @_; return $a + $b; }
来源：http://hz.xuanzx.com/gtpsxtoakz.html

[T50] Perl：逐行读文件
来源：http://hz.yongpay.top/gthnnxwkto.html

open my $fh, "<", "a.txt" or die $!;
来源：http://hz.xuetiantiany.cn/gtwhiyhlak.html

while (my $line = <$fh>) { print $line; }
来源：http://hz.gaohongyu789.top/gtljqsdtmn.html

[T51] Scala：Hello World
来源：http://hz.hysaishi.cn/gtiusliwwy.html

println("Hello")
来源：http://hz.wangshuangyany.cn/gtymauntgv.html

[T52] Scala：变量
来源：http://hz.meibo888.top/gtjmfblvou.html

val a = 1;  var b = 2
来源：http://hz.havefunace.top/gttjbybquc.html

[T53] Scala：字符串插值
来源：http://hz.ywan-chungtsiang.top/gtimyspegd.html

s"值: $b"
来源：http://hz.ivvv.top/gtbtabfnyg.html

[T54] Scala：集合映射
来源：http://hz.zhijiandao.cn/gtdubybbve.html

List(1, 2, 3).map(_ * 2)
来源：http://hz.cheryme.top/gtttkdyjus.html

[T55] Scala：集合过滤
来源：http://hz.iojbl.cn/gtkypuwloa.html

List(1, 2, 3).filter(_ > 1)
来源：http://hz.316326.xyz/gtgoszvthu.html

[T56] Scala：样例类
来源：http://hz.shanyushiyangtech.top/gtmrairlqn.html

case class User(name: String, age: Int)
来源：http://hz.jiagoushi.top/gtyrcmtlxs.html

[T57] Scala：模式匹配
来源：http://hz.xinyue.icu/gtjglwplsg.html

x match { case 1 => "一"; case _ => "其他" }
来源：http://hz.haohaochexian.top/gtvaiqznjp.html

[T58] Scala：函数定义
来源：http://hz.guowangkeji.top/gttohvzvff.html

def add(a: Int, b: Int): Int = a + b
来源：http://hz.fengsongda.top/gtciulwjig.html

[T59] Scala：循环
来源：http://hz.gogol.net.cn/gtzefwhbhe.html

for (i <- 1 to 10) println(i)
来源：http://hz.hnqzz.top/gtqtzidybi.html

[T60] Scala：折叠
来源：http://hz.jiagoushi.top/gtkqepfmiz.html

List(1, 2, 3).foldLeft(0)(_ + _)
来源：http://hz.ybcxt.top/gtwyjiywjd.html

================================================================================
来源：http://hz.hfpthk.cn/gtmfthhywl.html

U. 高频实用片段（Python / PHP / JavaScript 各 40 条）
来源：http://hz.xingfuxueyuan.xyz/gtibtevfiu.html

================================================================================
来源：http://hz.smart0.xyz/gtlyuxksnr.html

[U01] Py：创建虚拟环境
来源：http://hz.yj20258888.top/gtyaihzlwv.html

python -m venv .venv && source .venv/bin/activate
来源：http://hz.guowangkeji.top/gtnqoxxkht.html

[U02] Py：导出 / 安装依赖
来源：http://hz.pycfn.com/gtxqeaggka.html

pip freeze > requirements.txt;  pip install -r requirements.txt
来源：http://hz.tianlin.xyz/gtcwviohey.html

[U03] Py：加载 .env 配置
来源：http://hz.dashuyun.cn/gtftoesjbr.html

from dotenv import load_dotenv; load_dotenv()
来源：http://hz.xylfe.cn/gtkbjrfaqm.html

[U04] Py：变量调试打印
来源：http://hz.fengsongda.top/gttcbltbau.html

print(f"{x=}")            # 输出 x=值，Python 3.8+
来源：http://hz.hfpthk.cn/gtulreajob.html

[U05] Py：列表去重且保序
来源：http://hz.meibo888.top/gtzwunzwxc.html

list(dict.fromkeys(arr))
来源：http://hz.shanyushiyangtech.top/gteqxmrnig.html

[U06] Py：合并两个字典
来源：http://hz.zhixingplan.top/gtpjfnaoxq.html

{**a, **b}
来源：http://hz.jqgfzy.top/gtrqqwakbx.html

[U07] Py：反转字典键值
来源：http://hz.meibo888.top/gtltsgtdpq.html

{v: k for k, v in d.items()}
来源：http://hz.9152youxi.cn/gtluaffsva.html

[U08] Py：展平二维列表
来源：http://hz.andypj.xyz/gtnjricpqy.html

[y for x in nested for y in x]
来源：http://hz.gaohongyu789.top/gtclfhaecd.html

[U09] Py：字典取最大值的键
来源：http://hz.xuetiantiany.cn/gtgbhuebgf.html

max(d, key=d.get)
来源：http://hz.smart0.xyz/gtavqgokhe.html

[U10] Py：按值排序字典
来源：http://hz.xingfuxueyuan.xyz/gtkpboldtg.html

dict(sorted(d.items(), key=lambda kv: kv[1]))
来源：http://hz.chenlongwang.top/gtxzgroiwm.html

[U11] Py：生成器表达式
来源：http://hz.ehwqpu.com/gthfvpamih.html

(x * 2 for x in arr)
来源：http://hz.sufxvd.cn/gtkgnxnapf.html

[U12] Py：取出现最多的 3 个元素
来源：http://hz.havefunace.top/gtvrroqrsg.html

Counter(arr).most_common(3)
来源：http://hz.zdqjudy.top/gtgcknaxqf.html

[U13] Py：固定长度队列
来源：http://hz.ehwqpu.com/gtqxdixuce.html

deque(maxlen=10)
来源：http://hz.yj202588.top/gtmpecxvzp.html

[U14] Py：分组收集到列表
来源：http://hz.sysykeji.top/gtwbyrjzod.html

defaultdict(list)
来源：http://hz.wangdashe.top/gtfmchdmda.html

[U15] Py：高精度计时
来源：http://hz.cdnleiting.top/gtnljkjavw.html

t = time.perf_counter()
来源：http://hz.nanxinkj.top/gtwxuxlqnb.html

[U16] Py：命令行参数解析
来源：http://hz.wangdashe.top/gtzdhpzvgj.html

ap = argparse.ArgumentParser();  ap.add_argument("--name");  args = ap.parse_args()
来源：http://hz.hnqzz.top/gthevqbyee.html

[U17] Py：初始化日志
来源：http://hz.iojbl.cn/gtyrxqhitp.html

logging.basicConfig(level=logging.INFO)
来源：http://hz.yueranfly.top/gtvvnyxfvt.html

[U18] Py：预编译正则
来源：http://hz.hysaishi.cn/gtavbibesx.html

pat = re.compile(r"\d+")
来源：http://hz.xylfe.cn/gtadfgjgpn.html

[U19] Py：正则替换带回调
来源：http://hz.shanyushiyangkeji.top/gtfaotkeqn.html

re.sub(r"\d+", lambda m: str(int(m.group()) * 2), s)
来源：http://hz.hongshengwenyu.top/gtfeksqhne.html

[U20] Py：缓存函数结果
来源：http://hz.ppjwa.cn/gtdylniqul.html

@functools.lru_cache(maxsize=None)
来源：http://hz.yj202588.top/gtegquqphm.html

[U21] Py：自定义上下文管理器
来源：http://hz.fzhhl.top/gtuzdylknr.html

@contextlib.contextmanager
来源：http://hz.andypj.xyz/gtuflqhmqc.html

[U22] Py：矩阵转置
来源：http://hz.cucudq.cn/gtyolydzqp.html

list(zip(*m))
来源：http://hz.tanke756.top/gtgnmxzvds.html

[U23] Py：分块读取大文件
来源：http://hz.sxryk.cn/gtqjjhkdkr.html

for chunk in iter(lambda: f.read(8192), b""):
来源：http://hz.cheryme.top/gtvlwqloik.html

[U24] Py：路径操作
来源：http://hz.feifeiyinyue.top/gtsmpixrvj.html

Path("a/b.txt").parent.mkdir(parents=True, exist_ok=True)
来源：http://hz.xingfuxueyuan.xyz/gtwcvmozjy.html

[U25] Py：CSV 按字典读
来源：http://hz.chenjidiqi.icu/gtyghoyoxc.html

csv.DictReader(f)
来源：http://hz.fengsongda.top/gtdchntvuc.html

[U26] Py：并发下载
来源：http://hz.haohaochexian.top/gtjuoccrdj.html

ThreadPoolExecutor(max_workers=8).map(fetch, urls)
来源：http://hz.jiagoushi.top/gtmkxilood.html

[U27] Py：异步 HTTP
来源：http://hz.shuidangran.top/gtzovbiosd.html

aiohttp.ClientSession() 配合 async with
来源：http://hz.snrcjt.cn/gtilpvxrrc.html

[U28] Py：类型别名
来源：http://hz.c1oappe.top/gtcnuvnoqo.html

UserId = int
来源：http://hz.ydjk.org.cn/gtbltoplob.html

[U29] Py：属性校验
来源：http://hz.wangshuangyany.cn/gtkefivhph.html

@property 与 @x.setter 配合
来源：http://hz.yj20258.top/gtvckntgnd.html

[U30] Py：数据类
来源：http://hz.jinqigfzy.top/gtehkzvtdo.html

@dataclass(slots=True)
来源：http://hz.jinqigfzy.top/gtbhwsrron.html

[U31] Py：单测
来源：http://hz.xuetiantiany.cn/gtkygagdoj.html

python -m pytest -q
来源：http://hz.yj20258888.top/gtstnbhgdu.html

[U32] Py：代码格式化
来源：http://hz.ydzc1.top/gtcqhvkcii.html

ruff format . && ruff check --fix .
来源：http://hz.ydjk.org.cn/gtxnmmpzsg.html

[U33] Py：打包发布
来源：http://hz.zhoulong.xyz/gtjhpbsxhk.html

python -m build  （依赖 pyproject.toml）
来源：http://hz.sxryk.cn/gtfqzkxuuo.html

[U34] Py：判断编码
来源：http://hz.xingfuxueyuan.xyz/gtaqtwwmxk.html

chardet.detect(raw)
来源：http://hz.zhengqikj.top/gthklsbcrx.html

[U35] Py：发送邮件
来源：http://hz.wangshuangyany.cn/gtynvirohc.html

smtplib.SMTP_SSL(...).send_message(msg)
来源：http://hz.chenzaomai.com/gtfgzqbkrn.html

[U36] Py：定时任务
来源：http://hz.yongpay.top/gtqeeilvfr.html

schedule.every(10).minutes.do(job)
来源：http://hz.svipenyu.cn/gtvvsyppsd.html

[U37] Py：读写 Excel
来源：http://hz.zycfv.cn/gtgpxbwtdt.html

pandas.read_excel / DataFrame.to_excel
来源：http://hz.zhixingplan.top/gtfewvsvjw.html

[U38] Py：获取脚本所在目录
来源：http://hz.gotoacloud.top/gtyiguffrz.html

Path(__file__).resolve().parent
来源：http://hz.zdqjudy.top/gtjdkyujmx.html

[U39] Py：判断是否在交互环境
来源：http://hz.wangdashe.top/gtjfrcfsgx.html

sys.stdout.isatty()
来源：http://hz.jiagoushi.top/gtjxcssdzt.html

[U40] Py：打印到标准错误
来源：http://hz.meibo888.top/gtnoenoifu.html

print("err", file=sys.stderr)
来源：http://hz.guannengcc.top/gtwaastmqw.html

[U41] PHP：初始化 Composer 项目
来源：http://hz.nanxuanxn.top/gtjvftuhjk.html

composer init;  composer require guzzlehttp/guzzle
来源：http://hz.xingfuxueyuan.xyz/gtwiqhethw.html

[U42] PHP：PSR-4 自动加载
来源：http://hz.xinyue.icu/gtnqqjaqrt.html

"autoload": { "psr-4": { "App\\": "src/" } }
来源：http://hz.tian-w.cn/gthbaqadlh.html

[U43] PHP：声明命名空间
来源：http://hz.chenzaomai.com/gtududhcqa.html

namespace App\Http;
来源：http://hz.fzhhl.top/gtmceajxin.html

[U44] PHP：开启严格类型
来源：http://hz.dianchejie.cn/gtwxypcdkw.html

declare(strict_types=1);
来源：http://hz.andypj.xyz/gtmnvhbsnk.html

[U45] PHP：类型声明与返回类型
来源：http://hz.zhoulong.xyz/gtpklcbnrz.html

function add(int $a, int $b): int { return $a + $b; }
来源：http://hz.cdnleiting.top/gtlggpldim.html

[U46] PHP：可空类型
来源：http://hz.yangfankeji.com/gtfvyckhej.html

?string $name = null
来源：http://hz.wangdashe.top/gtiidjorhq.html

[U47] PHP：联合类型
来源：http://hz.svipenyu.cn/gttphusjug.html

int|string $id
来源：http://hz.yongpay.top/gtlsljvhnr.html

[U48] PHP：纯枚举
来源：http://hz.redwolf501.top/gtjvborwnn.html

enum Status: string { case Active = "active"; case Off = "off"; }
来源：http://hz.jiagoushi.top/gtldrsffjd.html

[U49] PHP：只读属性
来源：http://hz.smart0.xyz/gtkfevhxeh.html

public readonly string $name
来源：http://hz.xziqi.cn/gttudiakev.html

[U50] PHP：构造器属性提升
来源：http://hz.yangfankeji.com/gtsmokpcyk.html

public function __construct(private int $id) {}
来源：http://hz.shzxlz.cn/gthyysyqgf.html

[U51] PHP：数组解构
来源：http://hz.svipenyu.cn/gtzjieldlf.html

[$a, $b] = $arr;
来源：http://hz.ydzc1.top/gtktetaiux.html

[U52] PHP：箭头函数
来源：http://hz.jinqigufen.top/gttmbravgv.html

$double = fn($x) => $x * 2;
来源：http://hz.hywenlv.cn/gtpuonyxpv.html

[U53] PHP：空合并运算符
来源：http://hz.shanyushiyangkeji.top/gtsvmxljaa.html

$v = $a ?? $b ?? "default";
来源：http://hz.hfpthk.cn/gtihtckxpi.html

[U54] PHP：空安全调用
来源：http://hz.gaohongyu789.top/gtitozrqxp.html

$obj?->method()
来源：http://hz.yj202588.top/gtvahzmwtm.html

[U55] PHP：match 表达式
来源：http://hz.nanxuanxn.top/gtdkvznkmm.html

$s = match($x) { 1 => "一", default => "其他" };
来源：http://hz.svipenyu.cn/gtqiihyrtn.html

[U56] PHP：命名参数
来源：http://hz.snrcjt.cn/gtgrfmgwqy.html

f(a: 1, b: 2)
来源：http://hz.nanxuanxn.top/gtbapinxks.html


<!-- 参考信息 -->