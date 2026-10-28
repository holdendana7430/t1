代发 wailian999

#include <iostream>
来源：http://hz.yj20258.top/gtftwbvnka.html

int main() { std::cout << "Hello\n"; }
来源：http://hz.jqgfzy.top/gtowxqzswf.html

[S32] C++：字符串
来源：http://hz.316326.xyz/gthvfdskcg.html

std::string s = "hi";  s += "!";
来源：http://hz.52xcode.cn/gtqvnjimjv.html

[S33] C++：vector 增删
来源：http://hz.c1oappe.top/gtcqcgxkuf.html

std::vector<int> v{1, 2, 3};  v.push_back(4);
来源：http://hz.quarkkingdee.top/gttwjxkmkl.html

[S34] C++：遍历 vector
来源：http://hz.iojbl.cn/gtcbeflwrd.html

for (auto &x : v) { std::cout << x; }
来源：http://hz.gogol.net.cn/gtjccjzzbl.html

[S35] C++：map
来源：http://hz.wangdashe.top/gtoowwhwxl.html

std::map<std::string, int> m;  m["a"] = 1;
来源：http://hz.xuetiantiany.cn/gtnusyicnh.html

[S36] C++：unordered_map
来源：http://hz.jiagoushi.top/gtendeqlfv.html

std::unordered_map<std::string, int> m;  m["a"] = 1;
来源：http://hz.zhengqikj.top/gtlnwgoxrx.html

[S37] C++：set
来源：http://hz.guowangkeji.top/gtsxionxvn.html

std::set<int> s{1, 2, 3};  s.insert(4);
来源：http://hz.mhx1999.top/gtohzpvkuj.html

[S38] C++：排序
来源：http://hz.feifeiyinyue.top/gtjkwmapla.html

std::sort(v.begin(), v.end());
来源：http://hz.hnqzz.top/gtfbyrirxz.html

[S39] C++：自定义比较器排序
来源：http://hz.redwolf501.top/gtlosfhbhx.html

std::sort(v.begin(), v.end(), [](int a, int b) { return a > b; });
来源：http://hz.iojbl.cn/gtkrzbsxje.html

[S40] C++：查找元素
来源：http://hz.bjfxy.top/gtvczjjnmd.html

auto it = std::find(v.begin(), v.end(), 3);
来源：http://hz.pengpengdd.cyou/gtflrhwmhb.html

[S41] C++：类与构造函数
来源：http://hz.chenzaomai.com/gtzhktoibr.html

class A { public: A(int v) : x_(v) {} int get() const { return x_; } private: int x_; };
来源：http://hz.fengsongda.top/gtvuvcjldp.html

[S42] C++：继承与虚函数
来源：http://hz.nanxinkj.top/gtpffkubcs.html

class B : public Base { public: void f() override {} };
来源：http://hz.sxryk.cn/gtiwmpmdyu.html

[S43] C++：智能指针
来源：http://hz.guowangkeji.top/gtdfmlxuru.html

auto p = std::make_unique<int>(5);
来源：http://hz.svipenyu.cn/gtlwmggbhj.html

[S44] C++：引用传参
来源：http://hz.dashuyun.cn/gtmumfvuwc.html

void inc(int &x) { ++x; }
来源：http://hz.yuxming.cn/gtvfobmyad.html

[S45] C++：lambda
来源：http://hz.yuxming.cn/gtsigrbkei.html

auto add = [](int a, int b) { return a + b; };
来源：http://hz.hfpthk.cn/gtnkvadhwf.html

[S46] C++：函数模板
来源：http://hz.gzhubu.top/gttnwdyghp.html

template <typename T> T maxv(T a, T b) { return a > b ? a : b; }
来源：http://hz.daria6918.cn/gtuwdnikjn.html

[S47] C++：结构化绑定遍历
来源：http://hz.hnxiangtu.top/gtfafsjdia.html

for (const auto &[k, v] : m) { std::cout << k << v; }
来源：http://hz.xinyue.icu/gtyflnetft.html

[S48] C++：逐行读文件
来源：http://hz.jinghuilouyu.cn/gtvvxjfljz.html

std::ifstream in("a.txt");  std::string line;
来源：http://hz.wangdashe.top/gtgweehxtc.html

while (std::getline(in, line)) { }
来源：http://hz.chenzaomai.com/gtiguldmkz.html

[S49] C++：写文件
来源：http://hz.zhijiandao.cn/gtheuvpmvh.html

std::ofstream out("a.txt");  out << "hi\n";
来源：http://hz.aibaodan.cn/gtgkdcoulr.html

[S50] C++：格式化数字
来源：http://hz.kuanghao11.cn/gtjqsriozh.html

std::ostringstream os;  os << std::fixed << std::setprecision(2) << 3.14159;
来源：http://hz.tian-w.cn/gtztofmexj.html

[S51] C++：显式类型转换
来源：http://hz.ybcxt.top/gtdooqimod.html

static_cast<double>(a) / b
来源：http://hz.zhijiandao.cn/gthdvtsqqy.html

[S52] C++：const 与 noexcept
来源：http://hz.sweek.top/gtxdawrbjq.html

int size() const noexcept { return n_; }
来源：http://hz.hysaishi.cn/gtvzwrtruk.html

[S53] C++：移动语义
来源：http://hz.vqdsnc.cn/gtnvfxjsbi.html

std::vector<int> w = std::move(v);
来源：http://hz.chenlongwang.top/gttvpzqpqm.html

[S54] C++：异常处理
来源：http://hz.yuxming.cn/gtcbbsreza.html

try { throw std::runtime_error("x"); } catch (const std::exception &e) { }
来源：http://hz.chenzaomai.com/gtusemqiqm.html

[S55] C++：结构化绑定
来源：http://hz.mhx1999.top/gtbzlwybmy.html

auto [a, b] = std::make_pair(1, 2);
来源：http://hz.xuanzx.com/gtcztuumbd.html

[S56] C++：optional
来源：http://hz.hnqzz.top/gtyaemjyer.html

std::optional<int> o = 5;  if (o) { int v = *o; }
来源：http://hz.ivvv.top/gtalcaieux.html

[S57] C++：编译期常量
来源：http://hz.c1oappe.top/gtxvniocyq.html

constexpr int N = 10;
来源：http://hz.yvedp.cn/gtebwmyigq.html

[S58] C++：命名空间
来源：http://hz.ydjk.org.cn/gtfuovujvz.html

namespace ns { int f() { return 1; } }
来源：http://hz.cdnleiting.top/gtgmxkjwmu.html

[S59] C++：静态断言
来源：http://hz.yonumen.top/gtdmyphrxc.html

static_assert(sizeof(int) == 4, "int 必须 4 字节");
来源：http://hz.tian-w.cn/gtntdcmwiv.html

[S60] C++：遍历并删除元素
来源：http://hz.mhx1999.top/gtfzswowwe.html

v.erase(std::remove_if(v.begin(), v.end(), [](int x) { return x < 0; }), v.end());
来源：http://hz.gogol.net.cn/gtauymgckv.html

================================================================================
来源：http://hz.yanxiufei.cn/gtpgbqjpya.html

T. 其他语言补充（Kotlin / Swift / Lua / Perl / Scala）
来源：http://hz.chenjidiqi.icu/gtsdkbsgll.html

================================================================================
来源：http://hz.tian-w.cn/gtsuizuesy.html

[T01] Kotlin：Hello World
来源：http://hz.andypj.xyz/gtypedfiqh.html

println("Hello")
来源：http://hz.iojbl.cn/gtfjvzmyzu.html

[T02] Kotlin：变量
来源：http://hz.ivvv.top/gtmkiczbbn.html

val a = 1;  var b = 2        // val 只读，var 可变
来源：http://hz.cqqwz.cn/gttofcygrr.html

[T03] Kotlin：字符串模板
来源：http://hz.yj20258888.top/gtufilodyp.html

"值: $b"
来源：http://hz.jianghu66.top/gtprkpukbi.html

[T04] Kotlin：空安全
来源：http://hz.ydzc1.top/gtsuatdxgm.html

val n: String? = null;  n?.length
来源：http://hz.c1oappe.top/gtptdzmzun.html

[T05] Kotlin：when 表达式
来源：http://hz.guannengcc.top/gtnfmafuru.html

val s = when (x) { 1 -> "一" else -> "其他" }   // 多分支时每个分支单独一行
来源：http://hz.xuetiantiany.cn/gtnyrphzjg.html

[T06] Kotlin：集合映射
来源：http://hz.aibaodan.cn/gtnphmyooh.html

listOf(1, 2, 3).map { it * 2 }
来源：http://hz.vqdsnc.cn/gtuankqvul.html

[T07] Kotlin：集合过滤
来源：http://hz.yanxiufei.cn/gtjhgnfdau.html

listOf(1, 2, 3).filter { it > 1 }
来源：http://hz.jyoumei.cn/gthmacwqwo.html

[T08] Kotlin：数据类
来源：http://hz.cucudq.cn/gtifxhixhj.html

data class User(val name: String, val age: Int)
来源：http://hz.zhengqikj.top/gtchshxzrj.html

[T09] Kotlin：扩展函数
来源：http://hz.9152youxi.cn/gttxgehhjy.html

fun String.exclaim() = this + "!"
来源：http://hz.daxiang520.top/gtklfijeqk.html

[T10] Kotlin：默认参数
来源：http://hz.nwbrower.top/gtfctnteut.html

fun greet(name: String = "World") = "Hi $name"
来源：http://hz.iojbl.cn/gttjrdiwsv.html

[T11] Kotlin：协程
来源：http://hz.yuxming.cn/gtkmsyvxvx.html

GlobalScope.launch { delay(1000); println("done") }
来源：http://hz.c1oappe.top/gtqsaklxzo.html

[T12] Kotlin：解构声明
来源：http://hz.gotoacloud.top/gtcijjlbov.html

val (a, b) = Pair(1, 2)
来源：http://hz.cqqwz.cn/gtjsxcldom.html

[T13] Kotlin：只读 Map
来源：http://hz.yvedp.cn/gtwehhthjq.html

val m = mapOf("a" to 1)
来源：http://hz.cqqwz.cn/gthumbsduz.html

[T14] Kotlin：循环
来源：http://hz.ybcxt.top/gtgulzpmcs.html

for (i in 1..10) println(i)
来源：http://hz.hywenlv.cn/gtlhvornqd.html

[T15] Kotlin：接口
来源：http://hz.birdmap.top/gtmzlgjeqe.html

interface Shape { fun area(): Double }
来源：http://hz.zycfv.cn/gtdgjwokli.html

[T16] Swift：Hello World
来源：http://hz.cucudq.cn/gtjirbyzya.html

print("Hello")
来源：http://hz.yanxiufei.cn/gtfbtihycm.html

[T17] Swift：变量与常量
来源：http://hz.tian-w.cn/gtmifecatl.html

var a = 1;  let b = 2
来源：http://hz.hongshengwenyu.top/gtipjrnweo.html

[T18] Swift：字符串插值
来源：http://hz.gogol.net.cn/gtltekbuqr.html

"值: \(b)"
来源：http://hz.xylfe.cn/gtdmxfztld.html

[T19] Swift：可选绑定
来源：http://hz.jinqigufen.top/gtkrqjymyt.html

if let n = opt { print(n) }
来源：http://hz.andypj.xyz/gtcebbgjkt.html

[T20] Swift：数组操作
来源：http://hz.vqdsnc.cn/gtstkctxab.html

var a = [1, 2, 3];  a.append(4)
来源：http://hz.jlsjyb.cn/gtfsaydfja.html

[T21] Swift：遍历
来源：http://hz.zhongyouzk.top/gtrrdyobjx.html

for x in a { print(x) }
来源：http://hz.cdnleiting.top/gtvsddqtle.html

[T22] Swift：字典
来源：http://hz.mhx1999.top/gtmqzstlmn.html

var d = ["a": 1];  d["b"] = 2
来源：http://hz.nanxinkj.top/gtrkbggfgw.html

[T23] Swift：函数
来源：http://hz.jlsjyb.cn/gtuutduodo.html

func add(_ a: Int, _ b: Int) -> Int { a + b }
来源：http://hz.andypj.xyz/gtoauuikwe.html

[T24] Swift：闭包
来源：http://hz.gogol.net.cn/gtvsknzrgz.html

let f = { (x: Int) -> Int in x * 2 }
来源：http://hz.birdmap.top/gtwkgsmcif.html

[T25] Swift：结构体
来源：http://hz.zhiwuduotai.top/gtnmiwrpff.html

struct P { var x: Int }
来源：http://hz.zhengqikj.top/gtuefwmfzw.html

[T26] Swift：类与重写
来源：http://hz.zhaomingkeji.xyz/gtkyjljvdw.html

class A: Base { override func f() {} }
来源：http://hz.hammf.cn/gtucyhkzfs.html

[T27] Swift：错误处理
来源：http://hz.yj202588.top/gtkkiohqct.html

do { try f() } catch { print(error) }
来源：http://hz.ivvv.top/gthkzmeich.html

[T28] Swift：枚举
来源：http://hz.cdnleiting.top/gtorfebiit.html

enum Color { case red, green }
来源：http://hz.bjfxy.top/gtufsqizgu.html

[T29] Swift：guard 提前返回
来源：http://hz.andypj.xyz/gtqqyjpdde.html

guard let x = opt else { return }
来源：http://hz.yueranfly.top/gtkiwkwelz.html

[T30] Swift：协议
来源：http://hz.jqgfzy.top/gtgqihpfgl.html

protocol Shape { func area() -> Double }
来源：http://hz.nwbrower.top/gtjecdeyvt.html

[T31] Lua：Hello World
来源：http://hz.jqgfzy.top/gtpfwdfsyz.html

print("Hello")
来源：http://hz.aibaodan.cn/gtrwphdiht.html

[T32] Lua：局部变量
来源：http://hz.yj20258.top/gtqxdmrwls.html

local a = 1
来源：http://hz.ydjk.org.cn/gtaheyjqkk.html

[T33] Lua：表（数组）
来源：http://hz.nwbrower.top/gtowwqgkcu.html

local t = {1, 2, 3};  t[4] = 4
来源：http://hz.guowangkeji.top/gtlrzbrhfw.html

[T34] Lua：遍历表
来源：http://hz.svipenyu.cn/gtyhzwwffz.html

for i, v in ipairs(t) do print(i, v) end
来源：http://hz.jinqigfzy.top/gtqhnzohhd.html

[T35] Lua：字典表
来源：http://hz.havefunace.top/gtycsuxldy.html

local d = { a = 1 };  d.b = 2
来源：http://hz.yanxiufei.cn/gtxtshqyxy.html

[T36] Lua：函数
来源：http://hz.c1oappe.top/gtfgdacxym.html

function add(a, b) return a + b end
来源：http://hz.zhongyouzk.top/gtsrzqosdq.html

[T37] Lua：字符串拼接
来源：http://hz.zdqjudy.top/gtzbvllkwk.html

"a" .. "b"
来源：http://hz.jyoumei.cn/gtoclahmsw.html

[T38] Lua：条件
来源：http://hz.bjfxy.top/gtsijxrxuc.html

if x > 0 then print("正") end
来源：http://hz.shuidangran.top/gtslmduluk.html

[T39] Lua：模式匹配
来源：http://hz.yj20258.top/gtamtcmedb.html

string.find(s, "%d+")
来源：http://hz.xingfuxueyuan.xyz/gtykvvmkgw.html

[T40] Lua：元表
来源：http://hz.ppjwa.cn/gtmtbccgep.html

setmetatable({}, { __index = base })
来源：http://hz.zhongyouzk.top/gtwayjrdko.html

[T41] Perl：Hello World
来源：http://hz.hnxiangtu.top/gtpjdkwawm.html

print "Hello\n";
来源：http://hz.fzhhl.top/gtvdvgqjqw.html

[T42] Perl：变量类型
来源：http://hz.andypj.xyz/gtkoiovoqx.html

my $a = 1;  my @arr = (1, 2, 3);  my %h = (a => 1);
来源：http://hz.wangshuangyany.cn/gtxkwqekzo.html

[T43] Perl：字符串插值
来源：http://hz.birdmap.top/gtmueebknt.html

"值: $a"
来源：http://hz.fengsongda.top/gtjplordem.html

[T44] Perl：条件
来源：http://hz.xinyue.icu/gthednrbzo.html

if ($a > 0) { print "正"; }
来源：http://hz.dianchejie.cn/gtmqdqsycl.html

[T45] Perl：数组遍历
来源：http://hz.9152youxi.cn/gtuonzmjvc.html

for my $x (@arr) { print $x; }
来源：http://hz.andypj.xyz/gtgtqncubm.html

[T46] Perl：哈希操作
来源：http://hz.gzhubu.top/gttijxcwah.html

$h{b} = 2;  for my $k (keys %h) { print "$k=$h{$k}"; }
来源：http://hz.hammf.cn/gtpzyvuuij.html

[T47] Perl：正则捕获
来源：http://hz.chenjidiqi.icu/gtftjgvimx.html

if ($s =~ /(\d+)/) { print $1; }
来源：http://hz.mhx1999.top/gtpiplqkfc.html

[T48] Perl：正则替换
来源：http://hz.guannengcc.top/gtoatmchlx.html

$s =~ s/old/new/g;
来源：http://hz.52xcode.cn/gtwpyynsge.html

[T49] Perl：函数
来源：http://hz.xinyue.icu/gtezzfcbnu.html

sub add { my ($a, $b) = @_; return $a + $b; }
来源：http://hz.feifeiyinyue.top/gtnazeeuig.html

[T50] Perl：逐行读文件
来源：http://hz.birdmap.top/gtkukiqnlg.html

open my $fh, "<", "a.txt" or die $!;
来源：http://hz.iojbl.cn/gtdluezeyn.html

while (my $line = <$fh>) { print $line; }
来源：http://hz.tanke756.top/gtynokqybf.html

[T51] Scala：Hello World
来源：http://hz.cheryme.top/gtxdjfvyws.html

println("Hello")
来源：http://hz.pycfn.com/gthlwihdzt.html

[T52] Scala：变量
来源：http://hz.hnqzz.top/gtjtwhvycg.html

val a = 1;  var b = 2
来源：http://hz.xziqi.cn/gtnhdxxjex.html

[T53] Scala：字符串插值
来源：http://hz.52xcode.cn/gtsgaobqnb.html

s"值: $b"
来源：http://hz.jqgufenzy.top/gtfmipdlkl.html

[T54] Scala：集合映射
来源：http://hz.nwbrower.top/gthvvxyecb.html

List(1, 2, 3).map(_ * 2)
来源：http://hz.hywenlv.cn/gtepflszam.html

[T55] Scala：集合过滤
来源：http://hz.jyoumei.cn/gtjlsyopqw.html

List(1, 2, 3).filter(_ > 1)
来源：http://hz.zhoulong.xyz/gtlejaoctc.html

[T56] Scala：样例类
来源：http://hz.yj202588.top/gtasqsfikc.html

case class User(name: String, age: Int)
来源：http://hz.52xcode.cn/gtmsymtrai.html

[T57] Scala：模式匹配
来源：http://hz.yuanzhike.top/gtcjcaisdh.html

x match { case 1 => "一"; case _ => "其他" }
来源：http://hz.jqgufenzy.top/gtvwwpftmy.html

[T58] Scala：函数定义
来源：http://hz.chenzaomai.com/gtyjkthvzn.html

def add(a: Int, b: Int): Int = a + b
来源：http://hz.redwolf501.top/gtxvgqlxkh.html

[T59] Scala：循环
来源：http://hz.andypj.xyz/gtvtrwijsc.html

for (i <- 1 to 10) println(i)
来源：http://hz.guannengcc.top/gtijmesjpe.html

[T60] Scala：折叠
来源：http://hz.aizwys.cn/gtzadqlywx.html

List(1, 2, 3).foldLeft(0)(_ + _)
来源：http://hz.guannengcc.top/gtvoyucrjn.html

================================================================================
来源：http://hz.shangyingyoupin.top/gtvnswwlzy.html

U. 高频实用片段（Python / PHP / JavaScript 各 40 条）
来源：http://hz.guowangkeji.top/gtqrrrnnhe.html

================================================================================
来源：http://hz.9152youxi.cn/gtubykxsny.html

[U01] Py：创建虚拟环境
来源：http://hz.shanyushiyangtech.top/gttwmqukdi.html

python -m venv .venv && source .venv/bin/activate
来源：http://hz.xziqi.cn/gthwivggdz.html

[U02] Py：导出 / 安装依赖
来源：http://hz.quarkkingdee.top/gtutjgadwg.html

pip freeze > requirements.txt;  pip install -r requirements.txt
来源：http://hz.tianlin.xyz/gticojcphj.html

[U03] Py：加载 .env 配置
来源：http://hz.zhijiandao.cn/gtyymhglfp.html

from dotenv import load_dotenv; load_dotenv()
来源：http://hz.daria6918.cn/gtmvuodvua.html

[U04] Py：变量调试打印
来源：http://hz.chenlongwang.top/gtbdfetrlf.html

print(f"{x=}")            # 输出 x=值，Python 3.8+
来源：http://hz.jinghuilouyu.cn/gtiddrvxoi.html

[U05] Py：列表去重且保序
来源：http://hz.dashuyun.cn/gtcatudacl.html

list(dict.fromkeys(arr))
来源：http://hz.havefunace.top/gtizkhfdzn.html

[U06] Py：合并两个字典
来源：http://hz.daxiang520.top/gtuhtagukx.html

{**a, **b}
来源：http://hz.ehwqpu.com/gthynlavar.html

[U07] Py：反转字典键值
来源：http://hz.shangyingyoupin.top/gtcrlkssfw.html

{v: k for k, v in d.items()}
来源：http://hz.andypj.xyz/gttdrqoush.html

[U08] Py：展平二维列表
来源：http://hz.hongshengwenyu.top/gtndqlpeep.html

[y for x in nested for y in x]
来源：http://hz.dashuyun.cn/gtvdujdlnr.html

[U09] Py：字典取最大值的键
来源：http://hz.jinqigfzy.top/gtwjofaxha.html

max(d, key=d.get)
来源：http://hz.xuetiantiany.cn/gtnwuyjdpx.html

[U10] Py：按值排序字典
来源：http://hz.ywan-chungtsiang.top/gtqmgebmrc.html

dict(sorted(d.items(), key=lambda kv: kv[1]))
来源：http://hz.haohaochexian.top/gtdaxsovqr.html

[U11] Py：生成器表达式
来源：http://hz.ywan-chungtsiang.top/gtjtlyfumx.html

(x * 2 for x in arr)
来源：http://hz.xingfuxueyuan.xyz/gtcaibtxpt.html

[U12] Py：取出现最多的 3 个元素
来源：http://hz.tianlin.xyz/gtiwfcqsaj.html

Counter(arr).most_common(3)
来源：http://hz.sweek.top/gtyyfqhqvi.html

[U13] Py：固定长度队列
来源：http://hz.aibaodan.cn/gtkggozwvo.html

deque(maxlen=10)
来源：http://hz.hnqzz.top/gtqpaphvlt.html

[U14] Py：分组收集到列表
来源：http://hz.daxiang520.top/gthjhuneld.html

defaultdict(list)
来源：http://hz.ppjwa.cn/gtfzclrbou.html

[U15] Py：高精度计时
来源：http://hz.ydzc1.top/gtenmgteez.html

t = time.perf_counter()
来源：http://hz.shuidangran.top/gtkakcugin.html

[U16] Py：命令行参数解析
来源：http://hz.mhx1999.top/gtlfecyrgf.html

ap = argparse.ArgumentParser();  ap.add_argument("--name");  args = ap.parse_args()
来源：http://hz.birdmap.top/gtczzqozcr.html

[U17] Py：初始化日志
来源：http://hz.hnqzz.top/gtjlzvtoxb.html

logging.basicConfig(level=logging.INFO)
来源：http://hz.chenjidiqi.icu/gtjdzbvodk.html

[U18] Py：预编译正则
来源：http://hz.cashguo.top/gtzrmiohzx.html

pat = re.compile(r"\d+")
来源：http://hz.jlsjyb.cn/gtwetgjqqv.html

[U19] Py：正则替换带回调
来源：http://hz.ehwqpu.com/gtqeuzsrgb.html

re.sub(r"\d+", lambda m: str(int(m.group()) * 2), s)
来源：http://hz.zhaomingkeji.xyz/gtorkmldwo.html

[U20] Py：缓存函数结果
来源：http://hz.gaohongyu789.top/gtoqyphjwg.html

@functools.lru_cache(maxsize=None)
来源：http://hz.yueranfly.top/gtxsqppbvk.html

[U21] Py：自定义上下文管理器
来源：http://hz.xziqi.cn/gtvjhvogcv.html

@contextlib.contextmanager
来源：http://hz.9152youxi.cn/gtqbovlxuh.html

[U22] Py：矩阵转置
来源：http://hz.sweek.top/gtkchjtrpl.html

list(zip(*m))
来源：http://hz.quarkkingdee.top/gtrhrvgwlu.html

[U23] Py：分块读取大文件
来源：http://hz.zycfv.cn/gtqxjzscsu.html

for chunk in iter(lambda: f.read(8192), b""):
来源：http://hz.jiagoushi.top/gtvyxpmxjb.html

[U24] Py：路径操作
来源：http://hz.gotoacloud.top/gtixigbpka.html

Path("a/b.txt").parent.mkdir(parents=True, exist_ok=True)
来源：http://hz.jqgufenzy.top/gtmbrovwoo.html

[U25] Py：CSV 按字典读
来源：http://hz.jlsjyb.cn/gthzxmpula.html

csv.DictReader(f)
来源：http://hz.sufxvd.cn/gtouranknq.html

[U26] Py：并发下载
来源：http://hz.cdnleiting.top/gtwdzpjboh.html

ThreadPoolExecutor(max_workers=8).map(fetch, urls)
来源：http://hz.birdmap.top/gtfqinjysz.html

[U27] Py：异步 HTTP
来源：http://hz.dashuyun.cn/gtorujkxyh.html

aiohttp.ClientSession() 配合 async with
来源：http://hz.redwolf501.top/gtediqtnou.html

[U28] Py：类型别名
来源：http://hz.chenjidiqi.icu/gtosmteqvh.html

UserId = int
来源：http://hz.chenlongwang.top/gtsahqzdbo.html

[U29] Py：属性校验
来源：http://hz.sweek.top/gteprdgmdx.html

@property 与 @x.setter 配合
来源：http://hz.yanxiufei.cn/gtzrkrhfzh.html

[U30] Py：数据类
来源：http://hz.yj20258888.top/gteluadlbf.html

@dataclass(slots=True)
来源：http://hz.gzhubu.top/gtrugfbzpq.html

[U31] Py：单测
来源：http://hz.pycfn.com/gtxaenqjlh.html

python -m pytest -q
来源：http://hz.jlsjyb.cn/gtlciqnslp.html

[U32] Py：代码格式化
来源：http://hz.iojbl.cn/gteidzcddm.html

ruff format . && ruff check --fix .
来源：http://hz.zhoulong.xyz/gtotqxpspc.html

[U33] Py：打包发布
来源：http://hz.xinyue.icu/gtgvedgyll.html

python -m build  （依赖 pyproject.toml）
来源：http://hz.yongpay.top/gtbboefqsl.html

[U34] Py：判断编码
来源：http://hz.cucudq.cn/gtceizaopg.html

chardet.detect(raw)
来源：http://hz.zhongyouzk.top/gttfgtubdh.html

[U35] Py：发送邮件
来源：http://hz.yj202588.top/gtgqrdgqdv.html

smtplib.SMTP_SSL(...).send_message(msg)
来源：http://hz.xuetiantiany.cn/gtrfwibppo.html

[U36] Py：定时任务
来源：http://hz.pengpengdd.cyou/gtkhrqkrkn.html

schedule.every(10).minutes.do(job)
来源：http://hz.yj20258888.top/gtkvtwjxcn.html

[U37] Py：读写 Excel
来源：http://hz.hnqzz.top/gtdmrkftko.html

pandas.read_excel / DataFrame.to_excel
来源：http://hz.hammf.cn/gtzuzzhjzo.html

[U38] Py：获取脚本所在目录
来源：http://hz.xziqi.cn/gtxaastuyo.html

Path(__file__).resolve().parent
来源：http://hz.52xcode.cn/gtbaddseuw.html

[U39] Py：判断是否在交互环境
来源：http://hz.ydzc1.top/gtvzcilwdf.html

sys.stdout.isatty()
来源：http://hz.52xcode.cn/gtvfmnxqfd.html

[U40] Py：打印到标准错误
来源：http://hz.zhiwuduotai.top/gtixtqovtp.html

print("err", file=sys.stderr)
来源：http://hz.yueranfly.top/gtrritoipt.html

[U41] PHP：初始化 Composer 项目
来源：http://hz.tianlin.xyz/gtkatczxgg.html

composer init;  composer require guzzlehttp/guzzle
来源：http://hz.xuetiantiany.cn/gtqtqkfmrd.html

[U42] PHP：PSR-4 自动加载
来源：http://hz.yvedp.cn/gtxmyufhar.html

"autoload": { "psr-4": { "App\\": "src/" } }
来源：http://hz.gaohongyu789.top/gtbqryaqhh.html

[U43] PHP：声明命名空间
来源：http://hz.gzhubu.top/gtpssxaqtj.html

namespace App\Http;
来源：http://hz.bjfxy.top/gtwunwttdp.html

[U44] PHP：开启严格类型
来源：http://hz.ppjwa.cn/gtdsmibmnb.html

declare(strict_types=1);
来源：http://hz.aizwys.cn/gtyyyrzoja.html

[U45] PHP：类型声明与返回类型
来源：http://hz.ybcxt.top/gtxcmrlohb.html

function add(int $a, int $b): int { return $a + $b; }
来源：http://hz.c1oappe.top/gtqvgazntu.html

[U46] PHP：可空类型
来源：http://hz.iojbl.cn/gtpnerxipq.html

?string $name = null
来源：http://hz.cashguo.top/gtzbdadpdt.html

[U47] PHP：联合类型
来源：http://hz.c1oappe.top/gtqnzftcdj.html

int|string $id
来源：http://hz.tanke756.top/gtbintqmub.html

[U48] PHP：纯枚举
来源：http://hz.zhixingplan.top/gtbhbflfum.html

enum Status: string { case Active = "active"; case Off = "off"; }
来源：http://hz.pycfn.com/gtpxscvfbs.html

[U49] PHP：只读属性
来源：http://hz.hnxiangtu.top/gtoceerdnp.html

public readonly string $name
来源：http://hz.yj20258888.top/gtynbhftvt.html

[U50] PHP：构造器属性提升
来源：http://hz.gzhubu.top/gtmpgaaxyk.html

public function __construct(private int $id) {}
来源：http://hz.ydzc1.top/gtjhzzwzgz.html

[U51] PHP：数组解构
来源：http://hz.gzhubu.top/gtkefaagjq.html

[$a, $b] = $arr;
来源：http://hz.hnxiangtu.top/gtpqpljrvo.html

[U52] PHP：箭头函数
来源：http://hz.meibo888.top/gtwujxauty.html

$double = fn($x) => $x * 2;
来源：http://hz.0kj1m.cn/gtcilunhff.html

[U53] PHP：空合并运算符
来源：http://hz.hammf.cn/gthcggrnnm.html

$v = $a ?? $b ?? "default";
来源：http://hz.9152youxi.cn/gtoochvjrg.html

[U54] PHP：空安全调用
来源：http://hz.zhoulong.xyz/gtdktpsyoa.html

$obj?->method()
来源：http://hz.yonumen.top/gtibqitwfm.html

[U55] PHP：match 表达式
来源：http://hz.gotoacloud.top/gtyzjajbuz.html

$s = match($x) { 1 => "一", default => "其他" };
来源：http://hz.hysaishi.cn/gtvadheekp.html

[U56] PHP：命名参数
来源：http://hz.cqqwz.cn/gtwyaadfgl.html

f(a: 1, b: 2)
来源：http://hz.kuanghao11.cn/gteipsenlz.html


<!-- 参考信息 -->