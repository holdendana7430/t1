代发 wailian999

time_t t = time(NULL);  struct tm *tm = localtime(&t);
来源：http://hz.xziqi.cn/gtrggqdyzn.html

[S25] C：内存拷贝
来源：http://hz.quarkkingdee.top/gtddquubqm.html

memcpy(dst, src, n);
来源：http://hz.zhijiandao.cn/gtslenbxbg.html

[S26] C：内存清零
来源：http://hz.cashguo.top/gtjclldzyy.html

memset(a, 0, sizeof a);
来源：http://hz.jinqigfzy.top/gtxzcgweth.html

[S27] C：定义常量
来源：http://hz.zhaomingkeji.xyz/gtigqzvcib.html

const double PI = 3.14159;
来源：http://hz.yanxiufei.cn/gttsgdebmt.html

[S28] C：静态变量
来源：http://hz.redwolf501.top/gtxnloffkd.html

static int counter = 0;
来源：http://hz.vqdsnc.cn/gtcvfgeqja.html

[S29] C：变参函数
来源：http://hz.hfpthk.cn/gtyuifuvkm.html

va_list ap; va_start(ap, fmt); vprintf(fmt, ap); va_end(ap);
来源：http://hz.kuanghao11.cn/gttfbqdlwe.html

[S30] C：头文件保护
来源：http://hz.fengsongda.top/gtdojpesuj.html

#ifndef X_H
来源：http://hz.zhixingplan.top/gtdhhlfowq.html

#define X_H
来源：http://hz.zhixingplan.top/gtkeufqhfs.html

#endif
来源：http://hz.daria6918.cn/gtyhccrmfr.html

[S31] C++：Hello World
来源：http://hz.bjfxy.top/gtopykuaes.html

#include <iostream>
来源：http://hz.xinyue.icu/gtvpgrmhxo.html

int main() { std::cout << "Hello\n"; }
来源：http://hz.daria6918.cn/gthifwfdmx.html

[S32] C++：字符串
来源：http://hz.yuxming.cn/gtvnpajqtp.html

std::string s = "hi";  s += "!";
来源：http://hz.chenlongwang.top/gturmzxmwf.html

[S33] C++：vector 增删
来源：http://hz.shzxlz.cn/gtmzympkze.html

std::vector<int> v{1, 2, 3};  v.push_back(4);
来源：http://hz.zhijiandao.cn/gtxdjdgydy.html

[S34] C++：遍历 vector
来源：http://hz.dashuyun.cn/gtfkwbxhvj.html

for (auto &x : v) { std::cout << x; }
来源：http://hz.yuxming.cn/gtytcmhaxg.html

[S35] C++：map
来源：http://hz.pengpengdd.cyou/gtrfslxaiy.html

std::map<std::string, int> m;  m["a"] = 1;
来源：http://hz.52xcode.cn/gtdobtaswp.html

[S36] C++：unordered_map
来源：http://hz.316326.xyz/gtqxyamuey.html

std::unordered_map<std::string, int> m;  m["a"] = 1;
来源：http://hz.chenlongwang.top/gtzmlswwxj.html

[S37] C++：set
来源：http://hz.zhiwuduotai.top/gtqrmlacfz.html

std::set<int> s{1, 2, 3};  s.insert(4);
来源：http://hz.hammf.cn/gtulctemlf.html

[S38] C++：排序
来源：http://hz.jinqigfzy.top/gtchagvaca.html

std::sort(v.begin(), v.end());
来源：http://hz.snrcjt.cn/gtyeijndtw.html

[S39] C++：自定义比较器排序
来源：http://hz.shangyingyoupin.top/gtpsurukpc.html

std::sort(v.begin(), v.end(), [](int a, int b) { return a > b; });
来源：http://hz.wangdashe.top/gtjxwalhto.html

[S40] C++：查找元素
来源：http://hz.shanyushiyangtech.top/gtgfwletjj.html

auto it = std::find(v.begin(), v.end(), 3);
来源：http://hz.jianghu66.top/gtmstijqgs.html

[S41] C++：类与构造函数
来源：http://hz.dashuyun.cn/gtblisiyzt.html

class A { public: A(int v) : x_(v) {} int get() const { return x_; } private: int x_; };
来源：http://hz.svipenyu.cn/gtlpkvytuy.html

[S42] C++：继承与虚函数
来源：http://hz.iojbl.cn/gtoawaqrbg.html

class B : public Base { public: void f() override {} };
来源：http://hz.sufxvd.cn/gthxyngbtz.html

[S43] C++：智能指针
来源：http://hz.hongshengwenyu.top/gtlqadkgeu.html

auto p = std::make_unique<int>(5);
来源：http://hz.nwbrower.top/gtfuawincz.html

[S44] C++：引用传参
来源：http://hz.ivvv.top/gthdocohyh.html

void inc(int &x) { ++x; }
来源：http://hz.cdnleiting.top/gtcnthrlho.html

[S45] C++：lambda
来源：http://hz.zycfv.cn/gthwumpaum.html

auto add = [](int a, int b) { return a + b; };
来源：http://hz.zhijiandao.cn/gtcgyyndfa.html

[S46] C++：函数模板
来源：http://hz.andypj.xyz/gtqqiwalpm.html

template <typename T> T maxv(T a, T b) { return a > b ? a : b; }
来源：http://hz.yanxiufei.cn/gtudztwiro.html

[S47] C++：结构化绑定遍历
来源：http://hz.snrcjt.cn/gtcrnxgtgq.html

for (const auto &[k, v] : m) { std::cout << k << v; }
来源：http://hz.iojbl.cn/gttwtvncwc.html

[S48] C++：逐行读文件
来源：http://hz.vqdsnc.cn/gtrblrpfow.html

std::ifstream in("a.txt");  std::string line;
来源：http://hz.yanxiufei.cn/gtoralionu.html

while (std::getline(in, line)) { }
来源：http://hz.0kj1m.cn/gtrooejlxn.html

[S49] C++：写文件
来源：http://hz.sufxvd.cn/gtrpgedtok.html

std::ofstream out("a.txt");  out << "hi\n";
来源：http://hz.yuxming.cn/gtkeyffzyi.html

[S50] C++：格式化数字
来源：http://hz.haohaochexian.top/gtmtmiryek.html

std::ostringstream os;  os << std::fixed << std::setprecision(2) << 3.14159;
来源：http://hz.nanxinkj.top/gtcsfsochi.html

[S51] C++：显式类型转换
来源：http://hz.yongpay.top/gtfsmhsefn.html

static_cast<double>(a) / b
来源：http://hz.fzhhl.top/gtecvwsxmi.html

[S52] C++：const 与 noexcept
来源：http://hz.jqgfzy.top/gtjeiydmdq.html

int size() const noexcept { return n_; }
来源：http://hz.gzhubu.top/gthorzkwmb.html

[S53] C++：移动语义
来源：http://hz.daria6918.cn/gtmzjkkpwj.html

std::vector<int> w = std::move(v);
来源：http://hz.jinqigfzy.top/gtpdmbkwyh.html

[S54] C++：异常处理
来源：http://hz.nanxinkj.top/gtcqokrrcx.html

try { throw std::runtime_error("x"); } catch (const std::exception &e) { }
来源：http://hz.ydjk.org.cn/gtmmswsuux.html

[S55] C++：结构化绑定
来源：http://hz.cheryme.top/gtihbqmofn.html

auto [a, b] = std::make_pair(1, 2);
来源：http://hz.fzhhl.top/gthgstrnuw.html

[S56] C++：optional
来源：http://hz.jianghu66.top/gtkxwasxsy.html

std::optional<int> o = 5;  if (o) { int v = *o; }
来源：http://hz.nanxinkj.top/gtrqtjdvaa.html

[S57] C++：编译期常量
来源：http://hz.tanke756.top/gtgotpzxsg.html

constexpr int N = 10;
来源：http://hz.pycfn.com/gtfohqhrje.html

[S58] C++：命名空间
来源：http://hz.zhiwuduotai.top/gtcyshknrt.html

namespace ns { int f() { return 1; } }
来源：http://hz.kuanghao11.cn/gtvbssdezv.html

[S59] C++：静态断言
来源：http://hz.xinyue.icu/gticzmmvsa.html

static_assert(sizeof(int) == 4, "int 必须 4 字节");
来源：http://hz.9152youxi.cn/gtegbemhwd.html

[S60] C++：遍历并删除元素
来源：http://hz.yuanzhike.top/gtwfhckiou.html

v.erase(std::remove_if(v.begin(), v.end(), [](int x) { return x < 0; }), v.end());
来源：http://hz.guannengcc.top/gtlwsnyvxe.html

================================================================================
来源：http://hz.ppjwa.cn/gtifvrgfyn.html

T. 其他语言补充（Kotlin / Swift / Lua / Perl / Scala）
来源：http://hz.fengsongda.top/gtdvzfyvpz.html

================================================================================
来源：http://hz.c1oappe.top/gtpzakaaos.html

[T01] Kotlin：Hello World
来源：http://hz.zhixingplan.top/gtdlxtlowp.html

println("Hello")
来源：http://hz.andypj.xyz/gtbwsvacwp.html

[T02] Kotlin：变量
来源：http://hz.xuanzx.com/gtgaiuodbi.html

val a = 1;  var b = 2        // val 只读，var 可变
来源：http://hz.daxiang520.top/gttcuudern.html

[T03] Kotlin：字符串模板
来源：http://hz.andypj.xyz/gtteztqbzx.html

"值: $b"
来源：http://hz.cucudq.cn/gtqhnegphy.html

[T04] Kotlin：空安全
来源：http://hz.guannengcc.top/gtbtlsyurd.html

val n: String? = null;  n?.length
来源：http://hz.sufxvd.cn/gtwlcfrxid.html

[T05] Kotlin：when 表达式
来源：http://hz.ppjwa.cn/gtfthpkpij.html

val s = when (x) { 1 -> "一" else -> "其他" }   // 多分支时每个分支单独一行
来源：http://hz.andypj.xyz/gtajaofzhz.html

[T06] Kotlin：集合映射
来源：http://hz.cheryme.top/gtwkjancpx.html

listOf(1, 2, 3).map { it * 2 }
来源：http://hz.xinyue.icu/gtlatmkylx.html

[T07] Kotlin：集合过滤
来源：http://hz.52xcode.cn/gtdvkirnzr.html

listOf(1, 2, 3).filter { it > 1 }
来源：http://hz.ydjk.org.cn/gtcxxpvyry.html

[T08] Kotlin：数据类
来源：http://hz.ybcxt.top/gtggwpkhvp.html

data class User(val name: String, val age: Int)
来源：http://hz.hongshengwenyu.top/gtmwhtuqzo.html

[T09] Kotlin：扩展函数
来源：http://hz.ywan-chungtsiang.top/gtcopppgcp.html

fun String.exclaim() = this + "!"
来源：http://hz.hfpthk.cn/gtqatxkohy.html

[T10] Kotlin：默认参数
来源：http://hz.zhongyouzk.top/gtrcgbttzo.html

fun greet(name: String = "World") = "Hi $name"
来源：http://hz.ydzc1.top/gteubdxxgg.html

[T11] Kotlin：协程
来源：http://hz.aibaodan.cn/gtingnsons.html

GlobalScope.launch { delay(1000); println("done") }
来源：http://hz.quarkkingdee.top/gtzztmqsbu.html

[T12] Kotlin：解构声明
来源：http://hz.yvedp.cn/gtjroeywuh.html

val (a, b) = Pair(1, 2)
来源：http://hz.jiagoushi.top/gtqhrsccjm.html

[T13] Kotlin：只读 Map
来源：http://hz.yj20258.top/gtmonpxmrk.html

val m = mapOf("a" to 1)
来源：http://hz.zhoulong.xyz/gtvnfcyqeb.html

[T14] Kotlin：循环
来源：http://hz.bjfxy.top/gtumkyrqin.html

for (i in 1..10) println(i)
来源：http://hz.xingfuxueyuan.xyz/gtjrhwxixl.html

[T15] Kotlin：接口
来源：http://hz.sweek.top/gtmvivyvdy.html

interface Shape { fun area(): Double }
来源：http://hz.yuanzhike.top/gtbhctider.html

[T16] Swift：Hello World
来源：http://hz.yueranfly.top/gtnteygsuk.html

print("Hello")
来源：http://hz.xylfe.cn/gtmpjcapyp.html

[T17] Swift：变量与常量
来源：http://hz.pengpengdd.cyou/gtjkablmkl.html

var a = 1;  let b = 2
来源：http://hz.sxryk.cn/gtjlsxsxyi.html

[T18] Swift：字符串插值
来源：http://hz.ppjwa.cn/gtggevqxox.html

"值: \(b)"
来源：http://hz.wangshuangyany.cn/gtlgfmsxao.html

[T19] Swift：可选绑定
来源：http://hz.nwbrower.top/gtwdxuyiap.html

if let n = opt { print(n) }
来源：http://hz.jyoumei.cn/gtvieehwcq.html

[T20] Swift：数组操作
来源：http://hz.daria6918.cn/gtelydcwrk.html

var a = [1, 2, 3];  a.append(4)
来源：http://hz.cucudq.cn/gtauzlbpkf.html

[T21] Swift：遍历
来源：http://hz.316326.xyz/gtzjaghjqg.html

for x in a { print(x) }
来源：http://hz.hammf.cn/gtjszyaolg.html

[T22] Swift：字典
来源：http://hz.gotoacloud.top/gtkkflfmdc.html

var d = ["a": 1];  d["b"] = 2
来源：http://hz.pycfn.com/gtidtwoukr.html

[T23] Swift：函数
来源：http://hz.snrcjt.cn/gtpqwbpqhz.html

func add(_ a: Int, _ b: Int) -> Int { a + b }
来源：http://hz.dianchejie.cn/gtrjyysief.html

[T24] Swift：闭包
来源：http://hz.daxiang520.top/gtlntpwxml.html

let f = { (x: Int) -> Int in x * 2 }
来源：http://hz.sufxvd.cn/gtromgrbqy.html

[T25] Swift：结构体
来源：http://hz.gotoacloud.top/gttprmswsm.html

struct P { var x: Int }
来源：http://hz.birdmap.top/gtmkbaryco.html

[T26] Swift：类与重写
来源：http://hz.feifeiyinyue.top/gtijvxnbwb.html

class A: Base { override func f() {} }
来源：http://hz.cucudq.cn/gtylfrnoza.html

[T27] Swift：错误处理
来源：http://hz.0kj1m.cn/gtzqdzqhuj.html

do { try f() } catch { print(error) }
来源：http://hz.c1oappe.top/gtrcpremsu.html

[T28] Swift：枚举
来源：http://hz.meibo888.top/gtsqaqouxa.html

enum Color { case red, green }
来源：http://hz.mhx1999.top/gtiyvohsao.html

[T29] Swift：guard 提前返回
来源：http://hz.kuanghao11.cn/gtfrlfsyhg.html

guard let x = opt else { return }
来源：http://hz.smart0.xyz/gtmzaqfxsz.html

[T30] Swift：协议
来源：http://hz.yj20258.top/gtavpapndz.html

protocol Shape { func area() -> Double }
来源：http://hz.sweek.top/gtdtbdhqav.html

[T31] Lua：Hello World
来源：http://hz.jinqigfzy.top/gtdfrmvijs.html

print("Hello")
来源：http://hz.jinghuilouyu.cn/gtffawauru.html

[T32] Lua：局部变量
来源：http://hz.pycfn.com/gtucmqsfvi.html

local a = 1
来源：http://hz.chenzaomai.com/gtrwbxvkvg.html

[T33] Lua：表（数组）
来源：http://hz.ybcxt.top/gtoikdgzmz.html

local t = {1, 2, 3};  t[4] = 4
来源：http://hz.shanyushiyangtech.top/gtajleddqs.html

[T34] Lua：遍历表
来源：http://hz.nanxuanxn.top/gthjxpocdn.html

for i, v in ipairs(t) do print(i, v) end
来源：http://hz.wangdashe.top/gtxyhlpejf.html

[T35] Lua：字典表
来源：http://hz.zhengqikj.top/gtufxvcvwm.html

local d = { a = 1 };  d.b = 2
来源：http://hz.zycfv.cn/gtapbzpbno.html

[T36] Lua：函数
来源：http://hz.bjfxy.top/gtqumydnjv.html

function add(a, b) return a + b end
来源：http://hz.smart0.xyz/gtcfssvqlr.html

[T37] Lua：字符串拼接
来源：http://hz.bjfxy.top/gtbuphtzsx.html

"a" .. "b"
来源：http://hz.zhiwuduotai.top/gtqdmuddmd.html

[T38] Lua：条件
来源：http://hz.ppjwa.cn/gtroyrtldc.html

if x > 0 then print("正") end
来源：http://hz.daria6918.cn/gtxzehefmp.html

[T39] Lua：模式匹配
来源：http://hz.hongshengwenyu.top/gtgguqutdj.html

string.find(s, "%d+")
来源：http://hz.316326.xyz/gtjqbfpfus.html

[T40] Lua：元表
来源：http://hz.nanxuanxn.top/gtfankvhvr.html

setmetatable({}, { __index = base })
来源：http://hz.meibo888.top/gtlcjxcluq.html

[T41] Perl：Hello World
来源：http://hz.tian-w.cn/gtcbbdkwam.html

print "Hello\n";
来源：http://hz.ybcxt.top/gtoevkekft.html

[T42] Perl：变量类型
来源：http://hz.hammf.cn/gtpuicacvn.html

my $a = 1;  my @arr = (1, 2, 3);  my %h = (a => 1);
来源：http://hz.wangshuangyany.cn/gtenfjgfcd.html

[T43] Perl：字符串插值
来源：http://hz.jinyuanbaomall.cn/gtoqujdizs.html

"值: $a"
来源：http://hz.tian-w.cn/gtfhyhkeep.html

[T44] Perl：条件
来源：http://hz.ivvv.top/gtmlppkquk.html

if ($a > 0) { print "正"; }
来源：http://hz.hammf.cn/gtuxolbndc.html

[T45] Perl：数组遍历
来源：http://hz.yj20258888.top/gtwnevfakk.html

for my $x (@arr) { print $x; }
来源：http://hz.nanxuanxn.top/gtbulnckar.html

[T46] Perl：哈希操作
来源：http://hz.haohaochexian.top/gtntghrzrb.html

$h{b} = 2;  for my $k (keys %h) { print "$k=$h{$k}"; }
来源：http://hz.yuanzhike.top/gtlhngzjgp.html

[T47] Perl：正则捕获
来源：http://hz.birdmap.top/gtsdygsxai.html

if ($s =~ /(\d+)/) { print $1; }
来源：http://hz.jinghuilouyu.cn/gtqkfjsxrg.html

[T48] Perl：正则替换
来源：http://hz.ppjwa.cn/gtptckpqfk.html

$s =~ s/old/new/g;
来源：http://hz.zhaomingkeji.xyz/gtgmesoidq.html

[T49] Perl：函数
来源：http://hz.yvedp.cn/gtzycefgox.html

sub add { my ($a, $b) = @_; return $a + $b; }
来源：http://hz.zhixingplan.top/gtwvurfumt.html

[T50] Perl：逐行读文件
来源：http://hz.hnqzz.top/gttwhbecxm.html

open my $fh, "<", "a.txt" or die $!;
来源：http://hz.gzhubu.top/gtcabraiqm.html

while (my $line = <$fh>) { print $line; }
来源：http://hz.guannengcc.top/gtnosnhohx.html

[T51] Scala：Hello World
来源：http://hz.hnqzz.top/gtuqwgoylc.html

println("Hello")
来源：http://hz.smart0.xyz/gtitxczchf.html

[T52] Scala：变量
来源：http://hz.wangdashe.top/gtiehupero.html

val a = 1;  var b = 2
来源：http://hz.xuanzx.com/gthiwhoywr.html

[T53] Scala：字符串插值
来源：http://hz.chenzaomai.com/gtrbobxdzk.html

s"值: $b"
来源：http://hz.ehwqpu.com/gtgisgrtnf.html

[T54] Scala：集合映射
来源：http://hz.xingfuxueyuan.xyz/gtafekitxb.html

List(1, 2, 3).map(_ * 2)
来源：http://hz.aizwys.cn/gtqklvolsf.html

[T55] Scala：集合过滤
来源：http://hz.gotoacloud.top/gtesioyxwk.html

List(1, 2, 3).filter(_ > 1)
来源：http://hz.iojbl.cn/gtktqlmgpx.html

[T56] Scala：样例类
来源：http://hz.jinyuanbaomall.cn/gtntvnyjrb.html

case class User(name: String, age: Int)
来源：http://hz.xziqi.cn/gtpapjplqd.html

[T57] Scala：模式匹配
来源：http://hz.yuanzhike.top/gtzwjbxhza.html

x match { case 1 => "一"; case _ => "其他" }
来源：http://hz.hammf.cn/gtihfouaom.html

[T58] Scala：函数定义
来源：http://hz.dianchejie.cn/gtldvtxpil.html

def add(a: Int, b: Int): Int = a + b
来源：http://hz.zhongyouzk.top/gtpucarems.html

[T59] Scala：循环
来源：http://hz.jinqigufen.top/gtnfrwgbpm.html

for (i <- 1 to 10) println(i)
来源：http://hz.zhiwuduotai.top/gttpaoazmn.html

[T60] Scala：折叠
来源：http://hz.tanke756.top/gtwoarwpty.html

List(1, 2, 3).foldLeft(0)(_ + _)
来源：http://hz.hfpthk.cn/gtgiqreryd.html

================================================================================
来源：http://hz.tian-w.cn/gtexwnolox.html

U. 高频实用片段（Python / PHP / JavaScript 各 40 条）
来源：http://hz.jinghuilouyu.cn/gtbiugdknk.html

================================================================================
来源：http://hz.ivvv.top/gtfqibstpd.html

[U01] Py：创建虚拟环境
来源：http://hz.havefunace.top/gtntbxghrr.html

python -m venv .venv && source .venv/bin/activate
来源：http://hz.chenlongwang.top/gtgskzqnss.html

[U02] Py：导出 / 安装依赖
来源：http://hz.ppjwa.cn/gtoidmkdqv.html

pip freeze > requirements.txt;  pip install -r requirements.txt
来源：http://hz.gotoacloud.top/gtlkloyape.html

[U03] Py：加载 .env 配置
来源：http://hz.zdqjudy.top/gtsxbibljw.html

from dotenv import load_dotenv; load_dotenv()
来源：http://hz.hammf.cn/gtzgklmavp.html

[U04] Py：变量调试打印
来源：http://hz.nanxuanxn.top/gtvinnjiyz.html

print(f"{x=}")            # 输出 x=值，Python 3.8+
来源：http://hz.kuanghao11.cn/gtfaxomypn.html

[U05] Py：列表去重且保序
来源：http://hz.kuanghao11.cn/gthmagnmej.html

list(dict.fromkeys(arr))
来源：http://hz.mhx1999.top/gtwrcufhee.html

[U06] Py：合并两个字典
来源：http://hz.hfpthk.cn/gtcnygavtr.html

{**a, **b}
来源：http://hz.dashuyun.cn/gtbqajuuyj.html

[U07] Py：反转字典键值
来源：http://hz.ydjk.org.cn/gtcxbasfgf.html

{v: k for k, v in d.items()}
来源：http://hz.ybcxt.top/gthwxeyfrr.html

[U08] Py：展平二维列表
来源：http://hz.iojbl.cn/gtxojtpvsi.html

[y for x in nested for y in x]
来源：http://hz.sxryk.cn/gtsbytqrbe.html

[U09] Py：字典取最大值的键
来源：http://hz.cucudq.cn/gtigkzmhmw.html

max(d, key=d.get)
来源：http://hz.yueranfly.top/gtanbecrzf.html

[U10] Py：按值排序字典
来源：http://hz.ehwqpu.com/gtwpdxpxqz.html

dict(sorted(d.items(), key=lambda kv: kv[1]))
来源：http://hz.yj20258.top/gtzrfsjulk.html

[U11] Py：生成器表达式
来源：http://hz.xziqi.cn/gtxbbcchtb.html

(x * 2 for x in arr)
来源：http://hz.aizwys.cn/gtraqkiqms.html

[U12] Py：取出现最多的 3 个元素
来源：http://hz.jlsjyb.cn/gtkckttkef.html

Counter(arr).most_common(3)
来源：http://hz.shzxlz.cn/gtnwjxrkxe.html

[U13] Py：固定长度队列
来源：http://hz.ydjk.org.cn/gtkjpiyhtl.html

deque(maxlen=10)
来源：http://hz.andypj.xyz/gtokiiuhxr.html

[U14] Py：分组收集到列表
来源：http://hz.xuetiantiany.cn/gtptikxwqx.html

defaultdict(list)
来源：http://hz.yanxiufei.cn/gtesvrspvh.html

[U15] Py：高精度计时
来源：http://hz.smart0.xyz/gtuntpiczp.html

t = time.perf_counter()
来源：http://hz.chenzaomai.com/gtulncgyqf.html

[U16] Py：命令行参数解析
来源：http://hz.ydzc1.top/gtwxwnyamx.html

ap = argparse.ArgumentParser();  ap.add_argument("--name");  args = ap.parse_args()
来源：http://hz.ywan-chungtsiang.top/gtkcgclyew.html

[U17] Py：初始化日志
来源：http://hz.xziqi.cn/gtccbkxmbs.html

logging.basicConfig(level=logging.INFO)
来源：http://hz.tianlin.xyz/gtbdeszuqz.html

[U18] Py：预编译正则
来源：http://hz.shangyingyoupin.top/gtppdvjcqu.html

pat = re.compile(r"\d+")
来源：http://hz.chenjidiqi.icu/gtlozmzwvw.html

[U19] Py：正则替换带回调
来源：http://hz.zhixingplan.top/gtloruwzvq.html

re.sub(r"\d+", lambda m: str(int(m.group()) * 2), s)
来源：http://hz.hammf.cn/gtibraoqke.html

[U20] Py：缓存函数结果
来源：http://hz.zhixingplan.top/gtgvwiqqpx.html

@functools.lru_cache(maxsize=None)
来源：http://hz.guowangkeji.top/gtxdsigxhn.html

[U21] Py：自定义上下文管理器
来源：http://hz.c1oappe.top/gtmbxvqypa.html

@contextlib.contextmanager
来源：http://hz.bjfxy.top/gtzqsahsxe.html

[U22] Py：矩阵转置
来源：http://hz.fengsongda.top/gtokoovmno.html

list(zip(*m))
来源：http://hz.guowangkeji.top/gtsrrulker.html

[U23] Py：分块读取大文件
来源：http://hz.zhixingplan.top/gtjxkmowlm.html

for chunk in iter(lambda: f.read(8192), b""):
来源：http://hz.yuanzhike.top/gtwwfivqec.html

[U24] Py：路径操作
来源：http://hz.cdnleiting.top/gtlqlyiois.html

Path("a/b.txt").parent.mkdir(parents=True, exist_ok=True)
来源：http://hz.316326.xyz/gtieahtohz.html

[U25] Py：CSV 按字典读
来源：http://hz.hongshengwenyu.top/gtayykbxhd.html

csv.DictReader(f)
来源：http://hz.hnxiangtu.top/gtqmcslkkn.html

[U26] Py：并发下载
来源：http://hz.ivvv.top/gtfsonkmqa.html

ThreadPoolExecutor(max_workers=8).map(fetch, urls)
来源：http://hz.zycfv.cn/gtyuuzzdnx.html

[U27] Py：异步 HTTP
来源：http://hz.vqdsnc.cn/gtkyeupwdq.html

aiohttp.ClientSession() 配合 async with
来源：http://hz.zhixingplan.top/gtfrwhelth.html

[U28] Py：类型别名
来源：http://hz.xingfuxueyuan.xyz/gtvthdlwos.html

UserId = int
来源：http://hz.zdqjudy.top/gtmibxkiqo.html

[U29] Py：属性校验
来源：http://hz.nanxinkj.top/gtfswtacgc.html

@property 与 @x.setter 配合
来源：http://hz.jianghu66.top/gtukamvaco.html

[U30] Py：数据类
来源：http://hz.hywenlv.cn/gtkxdplmfx.html

@dataclass(slots=True)
来源：http://hz.ivvv.top/gtaaetyofq.html

[U31] Py：单测
来源：http://hz.xuanzx.com/gtjiulbixn.html

python -m pytest -q
来源：http://hz.316326.xyz/gtcxsomqig.html

[U32] Py：代码格式化
来源：http://hz.hnxiangtu.top/gtuzshuyed.html

ruff format . && ruff check --fix .
来源：http://hz.gotoacloud.top/gtblengxgg.html

[U33] Py：打包发布
来源：http://hz.jinyuanbaomall.cn/gtpebugfoa.html

python -m build  （依赖 pyproject.toml）
来源：http://hz.ehwqpu.com/gtjulcmnif.html

[U34] Py：判断编码
来源：http://hz.zhoulong.xyz/gtawzgyxlr.html

chardet.detect(raw)
来源：http://hz.haohaochexian.top/gtwixddwaz.html

[U35] Py：发送邮件
来源：http://hz.sxryk.cn/gtgkyjktdr.html

smtplib.SMTP_SSL(...).send_message(msg)
来源：http://hz.zhixingplan.top/gtnikqxsxy.html

[U36] Py：定时任务
来源：http://hz.jinqigfzy.top/gtflsbqbcq.html

schedule.every(10).minutes.do(job)
来源：http://hz.zhongyouzk.top/gtrnxbjolm.html

[U37] Py：读写 Excel
来源：http://hz.hnxiangtu.top/gteudbrpzr.html

pandas.read_excel / DataFrame.to_excel
来源：http://hz.ybcxt.top/gtvwfamiml.html

[U38] Py：获取脚本所在目录
来源：http://hz.smart0.xyz/gtxlpjqtnf.html

Path(__file__).resolve().parent
来源：http://hz.yangfankeji.com/gtxmvvnctq.html

[U39] Py：判断是否在交互环境
来源：http://hz.pycfn.com/gtxvwfdzom.html

sys.stdout.isatty()
来源：http://hz.cucudq.cn/gtlijqplzk.html

[U40] Py：打印到标准错误
来源：http://hz.jyoumei.cn/gttbxtjpaj.html

print("err", file=sys.stderr)
来源：http://hz.cucudq.cn/gtleekbmmb.html

[U41] PHP：初始化 Composer 项目
来源：http://hz.cqqwz.cn/gtsopdrzix.html

composer init;  composer require guzzlehttp/guzzle
来源：http://hz.ydzc1.top/gtmjwzjasg.html

[U42] PHP：PSR-4 自动加载
来源：http://hz.zhongyouzk.top/gtsnqhzqoq.html

"autoload": { "psr-4": { "App\\": "src/" } }
来源：http://hz.hongshengwenyu.top/gtatlrlavp.html

[U43] PHP：声明命名空间
来源：http://hz.iojbl.cn/gthkaydiac.html

namespace App\Http;
来源：http://hz.c1oappe.top/gtbfjlawga.html

[U44] PHP：开启严格类型
来源：http://hz.hammf.cn/gtuoibycli.html

declare(strict_types=1);
来源：http://hz.gzhubu.top/gtjdzedcsd.html

[U45] PHP：类型声明与返回类型
来源：http://hz.316326.xyz/gtmiqnifbz.html

function add(int $a, int $b): int { return $a + $b; }
来源：http://hz.0kj1m.cn/gtwzegtbnj.html

[U46] PHP：可空类型
来源：http://hz.cqqwz.cn/gtqnycmtne.html

?string $name = null
来源：http://hz.yonumen.top/gtwiftxsnt.html

[U47] PHP：联合类型
来源：http://hz.yueranfly.top/gtzwmqvsbn.html

int|string $id
来源：http://hz.jinqigfzy.top/gtaplgztax.html

[U48] PHP：纯枚举
来源：http://hz.ydzc1.top/gtutqshrdf.html

enum Status: string { case Active = "active"; case Off = "off"; }
来源：http://hz.aizwys.cn/gtsnkswwre.html


<!-- 参考信息 -->