代发 wailian999

[S33] C++：vector 增删
来源：http://hz.ehwqpu.com/gtaggrmjyd.html

std::vector<int> v{1, 2, 3};  v.push_back(4);
来源：http://hz.hysaishi.cn/gtvhkmexbf.html

[S34] C++：遍历 vector
来源：http://hz.xuetiantiany.cn/gtfglffmei.html

for (auto &x : v) { std::cout << x; }
来源：http://hz.c1oappe.top/gtejlqhjep.html

[S35] C++：map
来源：http://hz.haohaochexian.top/gtfsbdpvbm.html

std::map<std::string, int> m;  m["a"] = 1;
来源：http://hz.cashguo.top/gtvukbwfuh.html

[S36] C++：unordered_map
来源：http://hz.yuxming.cn/gtdanbahea.html

std::unordered_map<std::string, int> m;  m["a"] = 1;
来源：http://hz.0kj1m.cn/gtyggnwguf.html

[S37] C++：set
来源：http://hz.jqgufenzy.top/gtkbwsdsjx.html

std::set<int> s{1, 2, 3};  s.insert(4);
来源：http://hz.zhaomingkeji.xyz/gtfeuxtjmz.html

[S38] C++：排序
来源：http://hz.sweek.top/gtutnwlyxw.html

std::sort(v.begin(), v.end());
来源：http://hz.dashuyun.cn/gtntgjvmlo.html

[S39] C++：自定义比较器排序
来源：http://hz.yj20258.top/gtztnxcrmb.html

std::sort(v.begin(), v.end(), [](int a, int b) { return a > b; });
来源：http://hz.chenjidiqi.icu/gtttucnldz.html

[S40] C++：查找元素
来源：http://hz.ydzc1.top/gtwfererev.html

auto it = std::find(v.begin(), v.end(), 3);
来源：http://hz.xziqi.cn/gtagnmwklo.html

[S41] C++：类与构造函数
来源：http://hz.shanyushiyangtech.top/gtgslnhdxd.html

class A { public: A(int v) : x_(v) {} int get() const { return x_; } private: int x_; };
来源：http://hz.chenjidiqi.icu/gtpdoaljgg.html

[S42] C++：继承与虚函数
来源：http://hz.hysaishi.cn/gtwibauoub.html

class B : public Base { public: void f() override {} };
来源：http://hz.havefunace.top/gtgkzxspbp.html

[S43] C++：智能指针
来源：http://hz.sxryk.cn/gtmrihjses.html

auto p = std::make_unique<int>(5);
来源：http://hz.0kj1m.cn/gtklnmruxy.html

[S44] C++：引用传参
来源：http://hz.yj20258.top/gtxxxdvfvx.html

void inc(int &x) { ++x; }
来源：http://hz.zhijiandao.cn/gtnrauurfo.html

[S45] C++：lambda
来源：http://hz.ybcxt.top/gthearliyt.html

auto add = [](int a, int b) { return a + b; };
来源：http://hz.shanyushiyangtech.top/gtdpftfsxm.html

[S46] C++：函数模板
来源：http://hz.9152youxi.cn/gtvcuurksw.html

template <typename T> T maxv(T a, T b) { return a > b ? a : b; }
来源：http://hz.9152youxi.cn/gthdhbkfbz.html

[S47] C++：结构化绑定遍历
来源：http://hz.hammf.cn/gtfmtqtlke.html

for (const auto &[k, v] : m) { std::cout << k << v; }
来源：http://hz.zhaomingkeji.xyz/gtyucihxbt.html

[S48] C++：逐行读文件
来源：http://hz.hnxiangtu.top/gtjfxlslvz.html

std::ifstream in("a.txt");  std::string line;
来源：http://hz.mhx1999.top/gtzqljskos.html

while (std::getline(in, line)) { }
来源：http://hz.jianghu66.top/gtiasllxdp.html

[S49] C++：写文件
来源：http://hz.zhixingplan.top/gtjbztujym.html

std::ofstream out("a.txt");  out << "hi\n";
来源：http://hz.nanxinkj.top/gtgoamtvpy.html

[S50] C++：格式化数字
来源：http://hz.xziqi.cn/gtnrmfsecq.html

std::ostringstream os;  os << std::fixed << std::setprecision(2) << 3.14159;
来源：http://hz.gaohongyu789.top/gtnlcqlokc.html

[S51] C++：显式类型转换
来源：http://hz.jlsjyb.cn/gtjxabthav.html

static_cast<double>(a) / b
来源：http://hz.ybcxt.top/gtdyjgfmhb.html

[S52] C++：const 与 noexcept
来源：http://hz.shanyushiyangkeji.top/gtirbuxziu.html

int size() const noexcept { return n_; }
来源：http://hz.quarkkingdee.top/gtqksroxwb.html

[S53] C++：移动语义
来源：http://hz.0kj1m.cn/gtqzmcmcug.html

std::vector<int> w = std::move(v);
来源：http://hz.hnqzz.top/gtxsisquse.html

[S54] C++：异常处理
来源：http://hz.tianlin.xyz/gtofjkjvxl.html

try { throw std::runtime_error("x"); } catch (const std::exception &e) { }
来源：http://hz.cdnleiting.top/gthyzwkdut.html

[S55] C++：结构化绑定
来源：http://hz.hywenlv.cn/gttshoscuu.html

auto [a, b] = std::make_pair(1, 2);
来源：http://hz.redwolf501.top/gthqnyefxf.html

[S56] C++：optional
来源：http://hz.iojbl.cn/gtvbzcbjbf.html

std::optional<int> o = 5;  if (o) { int v = *o; }
来源：http://hz.yueranfly.top/gtknmrvgtv.html

[S57] C++：编译期常量
来源：http://hz.haohaochexian.top/gtbnpifvfk.html

constexpr int N = 10;
来源：http://hz.vqdsnc.cn/gtwiwvogfi.html

[S58] C++：命名空间
来源：http://hz.yuxming.cn/gtipzltzqv.html

namespace ns { int f() { return 1; } }
来源：http://hz.dianchejie.cn/gtnpehnjhf.html

[S59] C++：静态断言
来源：http://hz.zhoulong.xyz/gtbvhcbdbu.html

static_assert(sizeof(int) == 4, "int 必须 4 字节");
来源：http://hz.ybcxt.top/gtzjmqohnr.html

[S60] C++：遍历并删除元素
来源：http://hz.yangfankeji.com/gtnfyovkis.html

v.erase(std::remove_if(v.begin(), v.end(), [](int x) { return x < 0; }), v.end());
来源：http://hz.jlsjyb.cn/gtpwgzfrjk.html

================================================================================
来源：http://hz.fengsongda.top/gtnezzdjdv.html

T. 其他语言补充（Kotlin / Swift / Lua / Perl / Scala）
来源：http://hz.gotoacloud.top/gtnpuztjpl.html

================================================================================
来源：http://hz.gotoacloud.top/gtajwtpbxl.html

[T01] Kotlin：Hello World
来源：http://hz.yanxiufei.cn/gtevwluopn.html

println("Hello")
来源：http://hz.redwolf501.top/gtkhmzvnjl.html

[T02] Kotlin：变量
来源：http://hz.hnqzz.top/gtazgfwmhg.html

val a = 1;  var b = 2        // val 只读，var 可变
来源：http://hz.zhongyouzk.top/gtlpkuhafd.html

[T03] Kotlin：字符串模板
来源：http://hz.yj20258.top/gtbjqssydn.html

"值: $b"
来源：http://hz.gzhubu.top/gtoqlazdor.html

[T04] Kotlin：空安全
来源：http://hz.shuidangran.top/gtdzvshewk.html

val n: String? = null;  n?.length
来源：http://hz.tianlin.xyz/gtotkdfskc.html

[T05] Kotlin：when 表达式
来源：http://hz.zycfv.cn/gtcbjvgzoz.html

val s = when (x) { 1 -> "一" else -> "其他" }   // 多分支时每个分支单独一行
来源：http://hz.tanke756.top/gtugctgsco.html

[T06] Kotlin：集合映射
来源：http://hz.kuanghao11.cn/gtcxskqnoy.html

listOf(1, 2, 3).map { it * 2 }
来源：http://hz.zhijiandao.cn/gtquwmexdi.html

[T07] Kotlin：集合过滤
来源：http://hz.vqdsnc.cn/gtvvcdomjj.html

listOf(1, 2, 3).filter { it > 1 }
来源：http://hz.ehwqpu.com/gtawgggyre.html

[T08] Kotlin：数据类
来源：http://hz.shangyingyoupin.top/gtjgsysczv.html

data class User(val name: String, val age: Int)
来源：http://hz.wangshuangyany.cn/gtcqncdomb.html

[T09] Kotlin：扩展函数
来源：http://hz.yongpay.top/gtwufcrkua.html

fun String.exclaim() = this + "!"
来源：http://hz.daria6918.cn/gtjkcpjghg.html

[T10] Kotlin：默认参数
来源：http://hz.ppjwa.cn/gtghvlludf.html

fun greet(name: String = "World") = "Hi $name"
来源：http://hz.hnqzz.top/gtgzajoocg.html

[T11] Kotlin：协程
来源：http://hz.wangshuangyany.cn/gtsppxcomg.html

GlobalScope.launch { delay(1000); println("done") }
来源：http://hz.shangyingyoupin.top/gtglrighky.html

[T12] Kotlin：解构声明
来源：http://hz.sweek.top/gtivlcmujo.html

val (a, b) = Pair(1, 2)
来源：http://hz.zhiwuduotai.top/gtshyltyqd.html

[T13] Kotlin：只读 Map
来源：http://hz.ybcxt.top/gtcjckiwid.html

val m = mapOf("a" to 1)
来源：http://hz.shanyushiyangtech.top/gtzceeyxds.html

[T14] Kotlin：循环
来源：http://hz.redwolf501.top/gtevrkteur.html

for (i in 1..10) println(i)
来源：http://hz.yuanzhike.top/gtlqigozpt.html

[T15] Kotlin：接口
来源：http://hz.guowangkeji.top/gtollmbsnd.html

interface Shape { fun area(): Double }
来源：http://hz.andypj.xyz/gtzeggxmiy.html

[T16] Swift：Hello World
来源：http://hz.pycfn.com/gttvvrxqqm.html

print("Hello")
来源：http://hz.aibaodan.cn/gthrehvqoz.html

[T17] Swift：变量与常量
来源：http://hz.chenlongwang.top/gtogfpcbzg.html

var a = 1;  let b = 2
来源：http://hz.xuanzx.com/gtrtfxkvur.html

[T18] Swift：字符串插值
来源：http://hz.yj202588.top/gtvyvvdmic.html

"值: \(b)"
来源：http://hz.smart0.xyz/gtnttudcvf.html

[T19] Swift：可选绑定
来源：http://hz.nwbrower.top/gtljmqjnuv.html

if let n = opt { print(n) }
来源：http://hz.cdnleiting.top/gtjkhzjglf.html

[T20] Swift：数组操作
来源：http://hz.hywenlv.cn/gtgvhnwdgt.html

var a = [1, 2, 3];  a.append(4)
来源：http://hz.jinghuilouyu.cn/gtztdqaift.html

[T21] Swift：遍历
来源：http://hz.gotoacloud.top/gtzitdbbjt.html

for x in a { print(x) }
来源：http://hz.xinyue.icu/gtwfbxfsvc.html

[T22] Swift：字典
来源：http://hz.cashguo.top/gttpdctapp.html

var d = ["a": 1];  d["b"] = 2
来源：http://hz.quarkkingdee.top/gtbvkfkfgc.html

[T23] Swift：函数
来源：http://hz.sufxvd.cn/gtanhhxqvd.html

func add(_ a: Int, _ b: Int) -> Int { a + b }
来源：http://hz.svipenyu.cn/gtbtucmfgh.html

[T24] Swift：闭包
来源：http://hz.pengpengdd.cyou/gtnlbueyyt.html

let f = { (x: Int) -> Int in x * 2 }
来源：http://hz.316326.xyz/gtxfzgdlsr.html

[T25] Swift：结构体
来源：http://hz.zhengqikj.top/gtnecicfwy.html

struct P { var x: Int }
来源：http://hz.sweek.top/gtblitflkr.html

[T26] Swift：类与重写
来源：http://hz.ydjk.org.cn/gtrmqpwhvw.html

class A: Base { override func f() {} }
来源：http://hz.hysaishi.cn/gtkfufosmt.html

[T27] Swift：错误处理
来源：http://hz.c1oappe.top/gttgnixjks.html

do { try f() } catch { print(error) }
来源：http://hz.guowangkeji.top/gtnfkfrjds.html

[T28] Swift：枚举
来源：http://hz.birdmap.top/gttuwryfkk.html

enum Color { case red, green }
来源：http://hz.zhixingplan.top/gtndfomtiw.html

[T29] Swift：guard 提前返回
来源：http://hz.jqgufenzy.top/gtitahlcxa.html

guard let x = opt else { return }
来源：http://hz.ppjwa.cn/gtgnwtcdaa.html

[T30] Swift：协议
来源：http://hz.xylfe.cn/gtpjckiush.html

protocol Shape { func area() -> Double }
来源：http://hz.jinyuanbaomall.cn/gtewyqpagh.html

[T31] Lua：Hello World
来源：http://hz.nwbrower.top/gtsmsytdho.html

print("Hello")
来源：http://hz.hfpthk.cn/gtterpxows.html

[T32] Lua：局部变量
来源：http://hz.smart0.xyz/gtcxnvjinl.html

local a = 1
来源：http://hz.sysykeji.top/gtewjewgau.html

[T33] Lua：表（数组）
来源：http://hz.tian-w.cn/gtovkqrflm.html

local t = {1, 2, 3};  t[4] = 4
来源：http://hz.yangfankeji.com/gttdulrovw.html

[T34] Lua：遍历表
来源：http://hz.hnqzz.top/gtifmpuigt.html

for i, v in ipairs(t) do print(i, v) end
来源：http://hz.snrcjt.cn/gtbqounyke.html

[T35] Lua：字典表
来源：http://hz.gogol.net.cn/gtmcgfffcs.html

local d = { a = 1 };  d.b = 2
来源：http://hz.jinyuanbaomall.cn/gtschsvvbe.html

[T36] Lua：函数
来源：http://hz.xinyue.icu/gtetzxdbot.html

function add(a, b) return a + b end
来源：http://hz.cucudq.cn/gtujwzjnig.html

[T37] Lua：字符串拼接
来源：http://hz.zhijiandao.cn/gtlxiiodji.html

"a" .. "b"
来源：http://hz.daria6918.cn/gtlmsitgea.html

[T38] Lua：条件
来源：http://hz.yvedp.cn/gthcampeuq.html

if x > 0 then print("正") end
来源：http://hz.jinyuanbaomall.cn/gtsdwezjob.html

[T39] Lua：模式匹配
来源：http://hz.wangdashe.top/gtfeybcclz.html

string.find(s, "%d+")
来源：http://hz.shzxlz.cn/gtarceizin.html

[T40] Lua：元表
来源：http://hz.fengsongda.top/gttexqjnsm.html

setmetatable({}, { __index = base })
来源：http://hz.ydjk.org.cn/gtpvpryzpo.html

[T41] Perl：Hello World
来源：http://hz.cqqwz.cn/gtorcfgvmt.html

print "Hello\n";
来源：http://hz.mhx1999.top/gtdbzweksl.html

[T42] Perl：变量类型
来源：http://hz.jqgufenzy.top/gtkdkibmcu.html

my $a = 1;  my @arr = (1, 2, 3);  my %h = (a => 1);
来源：http://hz.jiagoushi.top/gtbhdyxvcv.html

[T43] Perl：字符串插值
来源：http://hz.sysykeji.top/gtokjnaakf.html

"值: $a"
来源：http://hz.daria6918.cn/gtalupejtv.html

[T44] Perl：条件
来源：http://hz.tian-w.cn/gteqpojtnj.html

if ($a > 0) { print "正"; }
来源：http://hz.cqqwz.cn/gtqssmrmch.html

[T45] Perl：数组遍历
来源：http://hz.shzxlz.cn/gtuwgqywbb.html

for my $x (@arr) { print $x; }
来源：http://hz.nwbrower.top/gtelyafzvp.html

[T46] Perl：哈希操作
来源：http://hz.quarkkingdee.top/gtttrviwlh.html

$h{b} = 2;  for my $k (keys %h) { print "$k=$h{$k}"; }
来源：http://hz.pycfn.com/gtdczfjkbw.html

[T47] Perl：正则捕获
来源：http://hz.xingfuxueyuan.xyz/gtueksasqg.html

if ($s =~ /(\d+)/) { print $1; }
来源：http://hz.sweek.top/gtwnskiheh.html

[T48] Perl：正则替换
来源：http://hz.shangyingyoupin.top/gtgcbtxmgc.html

$s =~ s/old/new/g;
来源：http://hz.xylfe.cn/gtrygnuryw.html

[T49] Perl：函数
来源：http://hz.ydzc1.top/gtgtlgwjpp.html

sub add { my ($a, $b) = @_; return $a + $b; }
来源：http://hz.aizwys.cn/gturfgmoco.html

[T50] Perl：逐行读文件
来源：http://hz.jiagoushi.top/gtitqprgkn.html

open my $fh, "<", "a.txt" or die $!;
来源：http://hz.tianlin.xyz/gtfjdskuze.html

while (my $line = <$fh>) { print $line; }
来源：http://hz.daria6918.cn/gthdrlvpxt.html

[T51] Scala：Hello World
来源：http://hz.iojbl.cn/gtktjcpqol.html

println("Hello")
来源：http://hz.smart0.xyz/gtuuksjkxn.html

[T52] Scala：变量
来源：http://hz.xingfuxueyuan.xyz/gtuljtvbun.html

val a = 1;  var b = 2
来源：http://hz.yj20258.top/gtugtwuvqx.html

[T53] Scala：字符串插值
来源：http://hz.meibo888.top/gtnggfvnep.html

s"值: $b"
来源：http://hz.hfpthk.cn/gthczfagfb.html

[T54] Scala：集合映射
来源：http://hz.iojbl.cn/gtfoiqwzxy.html

List(1, 2, 3).map(_ * 2)
来源：http://hz.dianchejie.cn/gtsxdelcsl.html

[T55] Scala：集合过滤
来源：http://hz.zhongyouzk.top/gteqtlffdr.html

List(1, 2, 3).filter(_ > 1)
来源：http://hz.quarkkingdee.top/gtwfbmqyyf.html

[T56] Scala：样例类
来源：http://hz.9152youxi.cn/gtanmsdvhv.html

case class User(name: String, age: Int)
来源：http://hz.jinqigufen.top/gtohpshcsv.html

[T57] Scala：模式匹配
来源：http://hz.bjfxy.top/gtzuftcomb.html

x match { case 1 => "一"; case _ => "其他" }
来源：http://hz.iojbl.cn/gtcziwnfhs.html

[T58] Scala：函数定义
来源：http://hz.zhongyouzk.top/gtkjyrweww.html

def add(a: Int, b: Int): Int = a + b
来源：http://hz.xuanzx.com/gttqwwlhxx.html

[T59] Scala：循环
来源：http://hz.yueranfly.top/gtdlnixpug.html

for (i <- 1 to 10) println(i)
来源：http://hz.pycfn.com/gtzsisdbca.html

[T60] Scala：折叠
来源：http://hz.hysaishi.cn/gtgmgltkbr.html

List(1, 2, 3).foldLeft(0)(_ + _)
来源：http://hz.guannengcc.top/gtqvyvpztg.html

================================================================================
来源：http://hz.yanxiufei.cn/gtjwelmpua.html

U. 高频实用片段（Python / PHP / JavaScript 各 40 条）
来源：http://hz.zhiwuduotai.top/gtbgikiolq.html

================================================================================
来源：http://hz.hysaishi.cn/gtzfjflxxr.html

[U01] Py：创建虚拟环境
来源：http://hz.cashguo.top/gtelmumqhg.html

python -m venv .venv && source .venv/bin/activate
来源：http://hz.shzxlz.cn/gteuugqbwi.html

[U02] Py：导出 / 安装依赖
来源：http://hz.chenlongwang.top/gtctguegsb.html

pip freeze > requirements.txt;  pip install -r requirements.txt
来源：http://hz.zhiwuduotai.top/gtyjccihfc.html

[U03] Py：加载 .env 配置
来源：http://hz.yueranfly.top/gtqxejqxkl.html

from dotenv import load_dotenv; load_dotenv()
来源：http://hz.zhengqikj.top/gtwwpsregy.html

[U04] Py：变量调试打印
来源：http://hz.zycfv.cn/gtpoqfnymc.html

print(f"{x=}")            # 输出 x=值，Python 3.8+
来源：http://hz.yj20258888.top/gtehezuxgm.html

[U05] Py：列表去重且保序
来源：http://hz.yonumen.top/gtjhtwotlr.html

list(dict.fromkeys(arr))
来源：http://hz.chenlongwang.top/gtzhztundc.html

[U06] Py：合并两个字典
来源：http://hz.mhx1999.top/gtfvrsgsve.html

{**a, **b}
来源：http://hz.jqgufenzy.top/gtmkwlfflv.html

[U07] Py：反转字典键值
来源：http://hz.vqdsnc.cn/gtlpwwbjcf.html

{v: k for k, v in d.items()}
来源：http://hz.jianghu66.top/gtedsfnbws.html

[U08] Py：展平二维列表
来源：http://hz.zhaomingkeji.xyz/gtjofxtnhp.html

[y for x in nested for y in x]
来源：http://hz.jqgfzy.top/gtpnisqbsa.html

[U09] Py：字典取最大值的键
来源：http://hz.cucudq.cn/gtfkeyswfp.html

max(d, key=d.get)
来源：http://hz.yuxming.cn/gtwgjzyzxt.html

[U10] Py：按值排序字典
来源：http://hz.zycfv.cn/gtskjzvkbv.html

dict(sorted(d.items(), key=lambda kv: kv[1]))
来源：http://hz.yvedp.cn/gtoqnkmhtk.html

[U11] Py：生成器表达式
来源：http://hz.tanke756.top/gtgdsksenv.html

(x * 2 for x in arr)
来源：http://hz.tianlin.xyz/gtrsgbhgdf.html

[U12] Py：取出现最多的 3 个元素
来源：http://hz.ydjk.org.cn/gtydfdqvzc.html

Counter(arr).most_common(3)
来源：http://hz.shangyingyoupin.top/gtkfzvpwko.html

[U13] Py：固定长度队列
来源：http://hz.iojbl.cn/gthcdyzmkm.html

deque(maxlen=10)
来源：http://hz.guannengcc.top/gtrchaijqs.html

[U14] Py：分组收集到列表
来源：http://hz.jianghu66.top/gtvikrfetz.html

defaultdict(list)
来源：http://hz.jyoumei.cn/gtzirdaigb.html

[U15] Py：高精度计时
来源：http://hz.svipenyu.cn/gtttpgqwxf.html

t = time.perf_counter()
来源：http://hz.sysykeji.top/gtlawcbpdl.html

[U16] Py：命令行参数解析
来源：http://hz.shanyushiyangkeji.top/gtovsuocmw.html

ap = argparse.ArgumentParser();  ap.add_argument("--name");  args = ap.parse_args()
来源：http://hz.316326.xyz/gtazcerkgj.html

[U17] Py：初始化日志
来源：http://hz.yj20258.top/gtoqsqkboi.html

logging.basicConfig(level=logging.INFO)
来源：http://hz.ivvv.top/gtdjcjpksf.html

[U18] Py：预编译正则
来源：http://hz.feifeiyinyue.top/gtkztntdau.html

pat = re.compile(r"\d+")
来源：http://hz.yongpay.top/gtquyoeual.html

[U19] Py：正则替换带回调
来源：http://hz.yangfankeji.com/gtafworkqs.html

re.sub(r"\d+", lambda m: str(int(m.group()) * 2), s)
来源：http://hz.sweek.top/gtkusbpkvt.html

[U20] Py：缓存函数结果
来源：http://hz.chenzaomai.com/gtweqxvjxe.html

@functools.lru_cache(maxsize=None)
来源：http://hz.svipenyu.cn/gtmmhyfaqj.html

[U21] Py：自定义上下文管理器
来源：http://hz.sufxvd.cn/gtnkxldhml.html

@contextlib.contextmanager
来源：http://hz.havefunace.top/gthgkxmaqu.html

[U22] Py：矩阵转置
来源：http://hz.tianlin.xyz/gtamvppqxh.html

list(zip(*m))
来源：http://hz.smart0.xyz/gtymgrpmpr.html

[U23] Py：分块读取大文件
来源：http://hz.fzhhl.top/gtkmgvhzlr.html

for chunk in iter(lambda: f.read(8192), b""):
来源：http://hz.gaohongyu789.top/gtrdezdgfm.html

[U24] Py：路径操作
来源：http://hz.zhijiandao.cn/gtbekiqbjj.html

Path("a/b.txt").parent.mkdir(parents=True, exist_ok=True)
来源：http://hz.ehwqpu.com/gteivdqrwm.html

[U25] Py：CSV 按字典读
来源：http://hz.cashguo.top/gtfvezelzb.html

csv.DictReader(f)
来源：http://hz.316326.xyz/gthsckeejm.html

[U26] Py：并发下载
来源：http://hz.cucudq.cn/gtbfjgcnnu.html

ThreadPoolExecutor(max_workers=8).map(fetch, urls)
来源：http://hz.chenzaomai.com/gtyopezflp.html

[U27] Py：异步 HTTP
来源：http://hz.pengpengdd.cyou/gtvpdnrnqh.html

aiohttp.ClientSession() 配合 async with
来源：http://hz.yanxiufei.cn/gtfklrulwv.html

[U28] Py：类型别名
来源：http://hz.fengsongda.top/gtoswnqusa.html

UserId = int
来源：http://hz.jinghuilouyu.cn/gtrefuakvs.html

[U29] Py：属性校验
来源：http://hz.iojbl.cn/gtzdprykvh.html

@property 与 @x.setter 配合
来源：http://hz.gotoacloud.top/gtnmiyacen.html

[U30] Py：数据类
来源：http://hz.xingfuxueyuan.xyz/gtijhrsztd.html

@dataclass(slots=True)
来源：http://hz.meibo888.top/gtlhpktswh.html

[U31] Py：单测
来源：http://hz.wangdashe.top/gtyplcekmv.html

python -m pytest -q
来源：http://hz.xinyue.icu/gtlobverdn.html

[U32] Py：代码格式化
来源：http://hz.dashuyun.cn/gtlaofdpit.html

ruff format . && ruff check --fix .
来源：http://hz.xuetiantiany.cn/gtlfxfhimh.html

[U33] Py：打包发布
来源：http://hz.shanyushiyangtech.top/gtrvwwntup.html

python -m build  （依赖 pyproject.toml）
来源：http://hz.pycfn.com/gtgacqjmqd.html

[U34] Py：判断编码
来源：http://hz.ivvv.top/gtlejipqrq.html

chardet.detect(raw)
来源：http://hz.wangshuangyany.cn/gtdxgmjwms.html

[U35] Py：发送邮件
来源：http://hz.zycfv.cn/gtbclfauvz.html

smtplib.SMTP_SSL(...).send_message(msg)
来源：http://hz.0kj1m.cn/gtzwdeggnl.html

[U36] Py：定时任务
来源：http://hz.316326.xyz/gtcykbliki.html

schedule.every(10).minutes.do(job)
来源：http://hz.svipenyu.cn/gtuhmannjl.html

[U37] Py：读写 Excel
来源：http://hz.nanxinkj.top/gtlbzbvuhj.html

pandas.read_excel / DataFrame.to_excel
来源：http://hz.jinghuilouyu.cn/gtlyntqkjw.html

[U38] Py：获取脚本所在目录
来源：http://hz.nanxinkj.top/gtqdjgekbd.html

Path(__file__).resolve().parent
来源：http://hz.52xcode.cn/gtttiaicpp.html

[U39] Py：判断是否在交互环境
来源：http://hz.zycfv.cn/gtkuxegfmv.html

sys.stdout.isatty()
来源：http://hz.wangshuangyany.cn/gtiqlvxeta.html

[U40] Py：打印到标准错误
来源：http://hz.shanyushiyangkeji.top/gtwdyftcsu.html

print("err", file=sys.stderr)
来源：http://hz.0kj1m.cn/gttochfywl.html

[U41] PHP：初始化 Composer 项目
来源：http://hz.shanyushiyangtech.top/gthabfqtjp.html

composer init;  composer require guzzlehttp/guzzle
来源：http://hz.shanyushiyangtech.top/gtzageyqiv.html

[U42] PHP：PSR-4 自动加载
来源：http://hz.nwbrower.top/gtfeytdguf.html

"autoload": { "psr-4": { "App\\": "src/" } }
来源：http://hz.zhengqikj.top/gtgjocsepg.html

[U43] PHP：声明命名空间
来源：http://hz.sufxvd.cn/gtinrxyknz.html

namespace App\Http;
来源：http://hz.mhx1999.top/gtkracublu.html

[U44] PHP：开启严格类型
来源：http://hz.ydjk.org.cn/gtbajsauvv.html

declare(strict_types=1);
来源：http://hz.xziqi.cn/gtmxyqibmk.html

[U45] PHP：类型声明与返回类型
来源：http://hz.yuanzhike.top/gtxjbrhmkx.html

function add(int $a, int $b): int { return $a + $b; }
来源：http://hz.ybcxt.top/gtjeowdcme.html

[U46] PHP：可空类型
来源：http://hz.sufxvd.cn/gtsupknbbb.html

?string $name = null
来源：http://hz.jinghuilouyu.cn/gtivueodgl.html

[U47] PHP：联合类型
来源：http://hz.sufxvd.cn/gtgjkirbhd.html

int|string $id
来源：http://hz.hywenlv.cn/gtejvhaqtc.html

[U48] PHP：纯枚举
来源：http://hz.cashguo.top/gtirzodvxu.html

enum Status: string { case Active = "active"; case Off = "off"; }
来源：http://hz.yanxiufei.cn/gthzrvxpkz.html

[U49] PHP：只读属性
来源：http://hz.jyoumei.cn/gtbxgnojlq.html

public readonly string $name
来源：http://hz.nwbrower.top/gtslsitdvm.html

[U50] PHP：构造器属性提升
来源：http://hz.0kj1m.cn/gtjbmcyhzi.html

public function __construct(private int $id) {}
来源：http://hz.sysykeji.top/gticsvwkxa.html

[U51] PHP：数组解构
来源：http://hz.andypj.xyz/gtobfwdabi.html

[$a, $b] = $arr;
来源：http://hz.shanyushiyangkeji.top/gtcivnjlnc.html

[U52] PHP：箭头函数
来源：http://hz.shzxlz.cn/gttirssdib.html

$double = fn($x) => $x * 2;
来源：http://hz.ehwqpu.com/gtcjnmntga.html

[U53] PHP：空合并运算符
来源：http://hz.hywenlv.cn/gtmmywygdg.html

$v = $a ?? $b ?? "default";
来源：http://hz.xinyue.icu/gtuvvvqxkx.html

[U54] PHP：空安全调用
来源：http://hz.hnqzz.top/gtwkbknkcz.html

$obj?->method()
来源：http://hz.hywenlv.cn/gtdnlhuiwj.html

[U55] PHP：match 表达式
来源：http://hz.0kj1m.cn/gtxgiwfqtz.html

$s = match($x) { 1 => "一", default => "其他" };
来源：http://hz.tian-w.cn/gtgvirozem.html

[U56] PHP：命名参数
来源：http://hz.cheryme.top/gtuhjqjhsj.html

f(a: 1, b: 2)
来源：http://hz.jianghu66.top/gtsuqpzbox.html

[U57] PHP：字符串插值
来源：http://hz.nanxinkj.top/gtlpjabbmj.html

"值: {$a}"
来源：http://hz.shanyushiyangtech.top/gtztnkiwjl.html

[U58] PHP：数组三件套
来源：http://hz.yongpay.top/gtbnrlxmov.html

array_map($f, $a);  array_filter($a, $f);  array_reduce($a, $f, 0);
来源：http://hz.quarkkingdee.top/gtyincnynb.html


<!-- 参考信息 -->