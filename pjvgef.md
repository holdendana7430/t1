代发 wailian999

[S35] C++：map
来源：http://hz.hfpthk.cn/gtmzmdwtjf.html

std::map<std::string, int> m;  m["a"] = 1;
来源：http://hz.nwbrower.top/gthshxfsiy.html

[S36] C++：unordered_map
来源：http://hz.sxryk.cn/gtzqwiojka.html

std::unordered_map<std::string, int> m;  m["a"] = 1;
来源：http://hz.hnqzz.top/gtanpmupuu.html

[S37] C++：set
来源：http://hz.pycfn.com/gtxuhdivsj.html

std::set<int> s{1, 2, 3};  s.insert(4);
来源：http://hz.aizwys.cn/gtxxxlrkfk.html

[S38] C++：排序
来源：http://hz.xuanzx.com/gtshnbsouh.html

std::sort(v.begin(), v.end());
来源：http://hz.nanxinkj.top/gthixnkpar.html

[S39] C++：自定义比较器排序
来源：http://hz.zhixingplan.top/gtqzxnimdz.html

std::sort(v.begin(), v.end(), [](int a, int b) { return a > b; });
来源：http://hz.shanyushiyangkeji.top/gtweynuloe.html

[S40] C++：查找元素
来源：http://hz.snrcjt.cn/gtdevsyfvd.html

auto it = std::find(v.begin(), v.end(), 3);
来源：http://hz.jyoumei.cn/gtqvfjegte.html

[S41] C++：类与构造函数
来源：http://hz.zhoulong.xyz/gthlvshrpv.html

class A { public: A(int v) : x_(v) {} int get() const { return x_; } private: int x_; };
来源：http://hz.yj202588.top/gtbpvznwdu.html

[S42] C++：继承与虚函数
来源：http://hz.ydjk.org.cn/gtwhtcztfv.html

class B : public Base { public: void f() override {} };
来源：http://hz.aibaodan.cn/gtuvtcfqts.html

[S43] C++：智能指针
来源：http://hz.yj20258888.top/gtxilovsrq.html

auto p = std::make_unique<int>(5);
来源：http://hz.cheryme.top/gtxrxssoyt.html

[S44] C++：引用传参
来源：http://hz.nwbrower.top/gtlictrsgz.html

void inc(int &x) { ++x; }
来源：http://hz.yueranfly.top/gtbtcmnkhl.html

[S45] C++：lambda
来源：http://hz.haohaochexian.top/gtiuhmogtk.html

auto add = [](int a, int b) { return a + b; };
来源：http://hz.cdnleiting.top/gthrlfzmmn.html

[S46] C++：函数模板
来源：http://hz.zhijiandao.cn/gtlaxanzzo.html

template <typename T> T maxv(T a, T b) { return a > b ? a : b; }
来源：http://hz.shzxlz.cn/gtttrqkiww.html

[S47] C++：结构化绑定遍历
来源：http://hz.bjfxy.top/gteshzjhmi.html

for (const auto &[k, v] : m) { std::cout << k << v; }
来源：http://hz.jqgfzy.top/gtgkrmosnj.html

[S48] C++：逐行读文件
来源：http://hz.daxiang520.top/gteirczyoo.html

std::ifstream in("a.txt");  std::string line;
来源：http://hz.jqgfzy.top/gtsoixsikd.html

while (std::getline(in, line)) { }
来源：http://hz.chenzaomai.com/gtkzngbplu.html

[S49] C++：写文件
来源：http://hz.aibaodan.cn/gtbgxzzckc.html

std::ofstream out("a.txt");  out << "hi\n";
来源：http://hz.zhiwuduotai.top/gtollgwiaz.html

[S50] C++：格式化数字
来源：http://hz.pycfn.com/gtqwtlzebz.html

std::ostringstream os;  os << std::fixed << std::setprecision(2) << 3.14159;
来源：http://hz.meibo888.top/gtulzdfyiw.html

[S51] C++：显式类型转换
来源：http://hz.ppjwa.cn/gtgswrrzmx.html

static_cast<double>(a) / b
来源：http://hz.sxryk.cn/gtdmniackl.html

[S52] C++：const 与 noexcept
来源：http://hz.tian-w.cn/gtylcunier.html

int size() const noexcept { return n_; }
来源：http://hz.316326.xyz/gtrkhhoves.html

[S53] C++：移动语义
来源：http://hz.yonumen.top/gthyfbyvpv.html

std::vector<int> w = std::move(v);
来源：http://hz.iojbl.cn/gtnyltpxpf.html

[S54] C++：异常处理
来源：http://hz.jinghuilouyu.cn/gtafdqdzxk.html

try { throw std::runtime_error("x"); } catch (const std::exception &e) { }
来源：http://hz.pengpengdd.cyou/gtlmiehocd.html

[S55] C++：结构化绑定
来源：http://hz.smart0.xyz/gtgfzykoct.html

auto [a, b] = std::make_pair(1, 2);
来源：http://hz.ehwqpu.com/gtokkagrbz.html

[S56] C++：optional
来源：http://hz.cqqwz.cn/gtdptgtgfb.html

std::optional<int> o = 5;  if (o) { int v = *o; }
来源：http://hz.hnxiangtu.top/gtacerucja.html

[S57] C++：编译期常量
来源：http://hz.daxiang520.top/gtkhoyqaul.html

constexpr int N = 10;
来源：http://hz.xuanzx.com/gtrwngbfvb.html

[S58] C++：命名空间
来源：http://hz.chenjidiqi.icu/gtgckqzupw.html

namespace ns { int f() { return 1; } }
来源：http://hz.hongshengwenyu.top/gtdgmhthgl.html

[S59] C++：静态断言
来源：http://hz.ydzc1.top/gtnjoiwtyb.html

static_assert(sizeof(int) == 4, "int 必须 4 字节");
来源：http://hz.xingfuxueyuan.xyz/gtbkkyyzqz.html

[S60] C++：遍历并删除元素
来源：http://hz.guowangkeji.top/gtydtiuack.html

v.erase(std::remove_if(v.begin(), v.end(), [](int x) { return x < 0; }), v.end());
来源：http://hz.yuxming.cn/gtvlkjluvg.html

================================================================================
来源：http://hz.hfpthk.cn/gtexccwrpk.html

T. 其他语言补充（Kotlin / Swift / Lua / Perl / Scala）
来源：http://hz.ybcxt.top/gtjxuyzytk.html

================================================================================
来源：http://hz.zhoulong.xyz/gtoxasxfld.html

[T01] Kotlin：Hello World
来源：http://hz.tianlin.xyz/gtcozgbafk.html

println("Hello")
来源：http://hz.jiagoushi.top/gtajlhbdta.html

[T02] Kotlin：变量
来源：http://hz.cqqwz.cn/gtaornrvap.html

val a = 1;  var b = 2        // val 只读，var 可变
来源：http://hz.chenzaomai.com/gtgjpmogqh.html

[T03] Kotlin：字符串模板
来源：http://hz.yanxiufei.cn/gtykdtdxgt.html

"值: $b"
来源：http://hz.zhoulong.xyz/gtbwwzrldx.html

[T04] Kotlin：空安全
来源：http://hz.cqqwz.cn/gtausmcdiz.html

val n: String? = null;  n?.length
来源：http://hz.shuidangran.top/gtluqzohio.html

[T05] Kotlin：when 表达式
来源：http://hz.bjfxy.top/gtesmbykhd.html

val s = when (x) { 1 -> "一" else -> "其他" }   // 多分支时每个分支单独一行
来源：http://hz.iojbl.cn/gtvphsmltb.html

[T06] Kotlin：集合映射
来源：http://hz.jqgufenzy.top/gtccirjskq.html

listOf(1, 2, 3).map { it * 2 }
来源：http://hz.jyoumei.cn/gtofzsebgc.html

[T07] Kotlin：集合过滤
来源：http://hz.svipenyu.cn/gtoinsuqdj.html

listOf(1, 2, 3).filter { it > 1 }
来源：http://hz.jqgufenzy.top/gtiztfgura.html

[T08] Kotlin：数据类
来源：http://hz.hnqzz.top/gtbilxxxzj.html

data class User(val name: String, val age: Int)
来源：http://hz.zycfv.cn/gtbxjrumqx.html

[T09] Kotlin：扩展函数
来源：http://hz.aizwys.cn/gthozvmuzd.html

fun String.exclaim() = this + "!"
来源：http://hz.cdnleiting.top/gtqinlpcht.html

[T10] Kotlin：默认参数
来源：http://hz.pycfn.com/gtdkrcisyo.html

fun greet(name: String = "World") = "Hi $name"
来源：http://hz.ppjwa.cn/gtbshxxymu.html

[T11] Kotlin：协程
来源：http://hz.andypj.xyz/gtvqmusyds.html

GlobalScope.launch { delay(1000); println("done") }
来源：http://hz.xylfe.cn/gtrffchoxl.html

[T12] Kotlin：解构声明
来源：http://hz.yj202588.top/gtvlducbpq.html

val (a, b) = Pair(1, 2)
来源：http://hz.yvedp.cn/gtiaecntlo.html

[T13] Kotlin：只读 Map
来源：http://hz.shanyushiyangtech.top/gtbiytvtub.html

val m = mapOf("a" to 1)
来源：http://hz.yueranfly.top/gtuysqpecp.html

[T14] Kotlin：循环
来源：http://hz.ydzc1.top/gtqacnkect.html

for (i in 1..10) println(i)
来源：http://hz.haohaochexian.top/gtimmydcko.html

[T15] Kotlin：接口
来源：http://hz.haohaochexian.top/gtxrmzmsju.html

interface Shape { fun area(): Double }
来源：http://hz.jinqigufen.top/gtbnonolvi.html

[T16] Swift：Hello World
来源：http://hz.redwolf501.top/gtgbrafgyg.html

print("Hello")
来源：http://hz.yueranfly.top/gtwggnzbdl.html

[T17] Swift：变量与常量
来源：http://hz.hongshengwenyu.top/gtxcjwpukf.html

var a = 1;  let b = 2
来源：http://hz.zhengqikj.top/gtwmavolvt.html

[T18] Swift：字符串插值
来源：http://hz.zhaomingkeji.xyz/gtxdesehrs.html

"值: \(b)"
来源：http://hz.iojbl.cn/gtntijhyin.html

[T19] Swift：可选绑定
来源：http://hz.zhiwuduotai.top/gtvuveevbb.html

if let n = opt { print(n) }
来源：http://hz.shzxlz.cn/gtlcehpzvl.html

[T20] Swift：数组操作
来源：http://hz.quarkkingdee.top/gtsjtvmymo.html

var a = [1, 2, 3];  a.append(4)
来源：http://hz.cheryme.top/gtmewywzwh.html

[T21] Swift：遍历
来源：http://hz.feifeiyinyue.top/gttydzszif.html

for x in a { print(x) }
来源：http://hz.hongshengwenyu.top/gtywmlxgjc.html

[T22] Swift：字典
来源：http://hz.feifeiyinyue.top/gtqmovctyy.html

var d = ["a": 1];  d["b"] = 2
来源：http://hz.ivvv.top/gtqaroyydl.html

[T23] Swift：函数
来源：http://hz.iojbl.cn/gtkulhnrex.html

func add(_ a: Int, _ b: Int) -> Int { a + b }
来源：http://hz.zhongyouzk.top/gtasjzumww.html

[T24] Swift：闭包
来源：http://hz.fengsongda.top/gtisnorhlx.html

let f = { (x: Int) -> Int in x * 2 }
来源：http://hz.cheryme.top/gtsplorapo.html

[T25] Swift：结构体
来源：http://hz.zhongyouzk.top/gtsrrgblkb.html

struct P { var x: Int }
来源：http://hz.cheryme.top/gtzfpiuwmi.html

[T26] Swift：类与重写
来源：http://hz.shzxlz.cn/gtbiwcefoi.html

class A: Base { override func f() {} }
来源：http://hz.nanxuanxn.top/gtzmbrewmh.html

[T27] Swift：错误处理
来源：http://hz.fzhhl.top/gtqfbzyewt.html

do { try f() } catch { print(error) }
来源：http://hz.wangdashe.top/gtoecaxdpk.html

[T28] Swift：枚举
来源：http://hz.ydjk.org.cn/gtquhsxngh.html

enum Color { case red, green }
来源：http://hz.chenzaomai.com/gtmssgogmi.html

[T29] Swift：guard 提前返回
来源：http://hz.fengsongda.top/gtkwmthjog.html

guard let x = opt else { return }
来源：http://hz.shangyingyoupin.top/gtckdzrpvg.html

[T30] Swift：协议
来源：http://hz.yonumen.top/gtiksdxzoo.html

protocol Shape { func area() -> Double }
来源：http://hz.sweek.top/gtvpkynfnq.html

[T31] Lua：Hello World
来源：http://hz.zycfv.cn/gtmfqewfrt.html

print("Hello")
来源：http://hz.sxryk.cn/gttboqqlho.html

[T32] Lua：局部变量
来源：http://hz.feifeiyinyue.top/gtaxputkwy.html

local a = 1
来源：http://hz.ppjwa.cn/gtbnfbdtlg.html

[T33] Lua：表（数组）
来源：http://hz.yonumen.top/gtvpjxsjsw.html

local t = {1, 2, 3};  t[4] = 4
来源：http://hz.redwolf501.top/gtiwvkgaoc.html

[T34] Lua：遍历表
来源：http://hz.cucudq.cn/gtohmleyzc.html

for i, v in ipairs(t) do print(i, v) end
来源：http://hz.jinqigufen.top/gtxdxrvfug.html

[T35] Lua：字典表
来源：http://hz.birdmap.top/gtyxtmqsgz.html

local d = { a = 1 };  d.b = 2
来源：http://hz.yuxming.cn/gtjiheiukq.html

[T36] Lua：函数
来源：http://hz.zhoulong.xyz/gtdvipmavq.html

function add(a, b) return a + b end
来源：http://hz.sufxvd.cn/gtfirrknvl.html

[T37] Lua：字符串拼接
来源：http://hz.cashguo.top/gtesqwkuxn.html

"a" .. "b"
来源：http://hz.ybcxt.top/gttyjizvxm.html

[T38] Lua：条件
来源：http://hz.dashuyun.cn/gtjesjwucz.html

if x > 0 then print("正") end
来源：http://hz.zhixingplan.top/gtkvyfmahg.html

[T39] Lua：模式匹配
来源：http://hz.fengsongda.top/gtzwtdnheu.html

string.find(s, "%d+")
来源：http://hz.zhijiandao.cn/gthburhqcp.html

[T40] Lua：元表
来源：http://hz.wangshuangyany.cn/gtlkllqlhj.html

setmetatable({}, { __index = base })
来源：http://hz.havefunace.top/gtqggaowle.html

[T41] Perl：Hello World
来源：http://hz.gzhubu.top/gtgxecyncq.html

print "Hello\n";
来源：http://hz.jianghu66.top/gttfolxvim.html

[T42] Perl：变量类型
来源：http://hz.0kj1m.cn/gtqynesdxu.html

my $a = 1;  my @arr = (1, 2, 3);  my %h = (a => 1);
来源：http://hz.jqgufenzy.top/gtnzuazfqf.html

[T43] Perl：字符串插值
来源：http://hz.fengsongda.top/gtyzonozdb.html

"值: $a"
来源：http://hz.bjfxy.top/gtvoqknwci.html

[T44] Perl：条件
来源：http://hz.yongpay.top/gtfdqdvogw.html

if ($a > 0) { print "正"; }
来源：http://hz.jinqigufen.top/gtjcvbcywe.html

[T45] Perl：数组遍历
来源：http://hz.zhijiandao.cn/gtvywttxyi.html

for my $x (@arr) { print $x; }
来源：http://hz.yj202588.top/gtpxfnyord.html

[T46] Perl：哈希操作
来源：http://hz.wangdashe.top/gtvujwitzr.html

$h{b} = 2;  for my $k (keys %h) { print "$k=$h{$k}"; }
来源：http://hz.xinyue.icu/gtmaeecxnl.html

[T47] Perl：正则捕获
来源：http://hz.jiagoushi.top/gtcsvwxhbe.html

if ($s =~ /(\d+)/) { print $1; }
来源：http://hz.yueranfly.top/gtrdzgspfv.html

[T48] Perl：正则替换
来源：http://hz.zhaomingkeji.xyz/gtkkdkqbam.html

$s =~ s/old/new/g;
来源：http://hz.hfpthk.cn/gtntwnvypp.html

[T49] Perl：函数
来源：http://hz.quarkkingdee.top/gtfukapqgr.html

sub add { my ($a, $b) = @_; return $a + $b; }
来源：http://hz.nwbrower.top/gtyjorbufn.html

[T50] Perl：逐行读文件
来源：http://hz.wangshuangyany.cn/gtpizmjkzh.html

open my $fh, "<", "a.txt" or die $!;
来源：http://hz.yongpay.top/gtrxvowhpl.html

while (my $line = <$fh>) { print $line; }
来源：http://hz.ybcxt.top/gtlrgmtrzh.html

[T51] Scala：Hello World
来源：http://hz.birdmap.top/gtjfpjrmrx.html

println("Hello")
来源：http://hz.yanxiufei.cn/gtqlbrsqwv.html

[T52] Scala：变量
来源：http://hz.gotoacloud.top/gtbsotivnb.html

val a = 1;  var b = 2
来源：http://hz.dashuyun.cn/gteivcpjzj.html

[T53] Scala：字符串插值
来源：http://hz.xinyue.icu/gtaxvyqgdr.html

s"值: $b"
来源：http://hz.hysaishi.cn/gttbmexoth.html

[T54] Scala：集合映射
来源：http://hz.sysykeji.top/gtyvwpuxeo.html

List(1, 2, 3).map(_ * 2)
来源：http://hz.mhx1999.top/gtdkxigmja.html

[T55] Scala：集合过滤
来源：http://hz.ydzc1.top/gthiulkvhm.html

List(1, 2, 3).filter(_ > 1)
来源：http://hz.jianghu66.top/gtylslsbqu.html

[T56] Scala：样例类
来源：http://hz.52xcode.cn/gtqbndocli.html

case class User(name: String, age: Int)
来源：http://hz.bjfxy.top/gtefwkxghr.html

[T57] Scala：模式匹配
来源：http://hz.9152youxi.cn/gtnmtawwyz.html

x match { case 1 => "一"; case _ => "其他" }
来源：http://hz.kuanghao11.cn/gtpuznkwpi.html

[T58] Scala：函数定义
来源：http://hz.cqqwz.cn/gtyxthnfht.html

def add(a: Int, b: Int): Int = a + b
来源：http://hz.jinghuilouyu.cn/gtlmvlbggv.html

[T59] Scala：循环
来源：http://hz.chenzaomai.com/gtnjzpbxcw.html

for (i <- 1 to 10) println(i)
来源：http://hz.9152youxi.cn/gtbkriqbfj.html

[T60] Scala：折叠
来源：http://hz.ydzc1.top/gtbuipwnqh.html

List(1, 2, 3).foldLeft(0)(_ + _)
来源：http://hz.sxryk.cn/gtxkhuxnaj.html

================================================================================
来源：http://hz.bjfxy.top/gtetgttlvb.html

U. 高频实用片段（Python / PHP / JavaScript 各 40 条）
来源：http://hz.jiagoushi.top/gtrsgvgwxq.html

================================================================================
来源：http://hz.cdnleiting.top/gtpfzphnzw.html

[U01] Py：创建虚拟环境
来源：http://hz.tianlin.xyz/gtsllyggsk.html

python -m venv .venv && source .venv/bin/activate
来源：http://hz.hfpthk.cn/gtuqwkcmbp.html

[U02] Py：导出 / 安装依赖
来源：http://hz.dashuyun.cn/gtcinpxafq.html

pip freeze > requirements.txt;  pip install -r requirements.txt
来源：http://hz.zycfv.cn/gtxlunyfzs.html

[U03] Py：加载 .env 配置
来源：http://hz.guannengcc.top/gtzyvhkfxh.html

from dotenv import load_dotenv; load_dotenv()
来源：http://hz.jianghu66.top/gtuorujsbg.html

[U04] Py：变量调试打印
来源：http://hz.havefunace.top/gtgpqkbjlk.html

print(f"{x=}")            # 输出 x=值，Python 3.8+
来源：http://hz.xylfe.cn/gtddhhjjug.html

[U05] Py：列表去重且保序
来源：http://hz.shangyingyoupin.top/gtyutdftbg.html

list(dict.fromkeys(arr))
来源：http://hz.yangfankeji.com/gtqnxyxsys.html

[U06] Py：合并两个字典
来源：http://hz.quarkkingdee.top/gtowemllrm.html

{**a, **b}
来源：http://hz.yuxming.cn/gtenvmsjnz.html

[U07] Py：反转字典键值
来源：http://hz.0kj1m.cn/gtpxtxyokr.html

{v: k for k, v in d.items()}
来源：http://hz.smart0.xyz/gtxoofmios.html

[U08] Py：展平二维列表
来源：http://hz.gotoacloud.top/gtimdqtuvt.html

[y for x in nested for y in x]
来源：http://hz.yanxiufei.cn/gtcbmslant.html

[U09] Py：字典取最大值的键
来源：http://hz.c1oappe.top/gtaavhszlo.html

max(d, key=d.get)
来源：http://hz.wangshuangyany.cn/gtscpgxjam.html

[U10] Py：按值排序字典
来源：http://hz.tianlin.xyz/gtdmtwyvvg.html

dict(sorted(d.items(), key=lambda kv: kv[1]))
来源：http://hz.xylfe.cn/gtuxvdcxcm.html

[U11] Py：生成器表达式
来源：http://hz.hysaishi.cn/gtoyfewzgu.html

(x * 2 for x in arr)
来源：http://hz.snrcjt.cn/gttvtflxad.html

[U12] Py：取出现最多的 3 个元素
来源：http://hz.zhiwuduotai.top/gtrufylgdo.html

Counter(arr).most_common(3)
来源：http://hz.cqqwz.cn/gtfkyxjymj.html

[U13] Py：固定长度队列
来源：http://hz.andypj.xyz/gtfwgqcxhr.html

deque(maxlen=10)
来源：http://hz.yangfankeji.com/gtdlakdwpx.html

[U14] Py：分组收集到列表
来源：http://hz.tian-w.cn/gtswhjijsy.html

defaultdict(list)
来源：http://hz.tanke756.top/gtsnmkuguo.html

[U15] Py：高精度计时
来源：http://hz.wangdashe.top/gtybnramrf.html

t = time.perf_counter()
来源：http://hz.yvedp.cn/gtytqpgxjx.html

[U16] Py：命令行参数解析
来源：http://hz.cdnleiting.top/gtjttgsjyb.html

ap = argparse.ArgumentParser();  ap.add_argument("--name");  args = ap.parse_args()
来源：http://hz.tanke756.top/gtktkrhqgj.html

[U17] Py：初始化日志
来源：http://hz.quarkkingdee.top/gtapikglrk.html

logging.basicConfig(level=logging.INFO)
来源：http://hz.sufxvd.cn/gtmjpoewqk.html

[U18] Py：预编译正则
来源：http://hz.shangyingyoupin.top/gtjlngjmhw.html

pat = re.compile(r"\d+")
来源：http://hz.yuxming.cn/gtgcvcjrnw.html

[U19] Py：正则替换带回调
来源：http://hz.yueranfly.top/gtczxbhcyu.html

re.sub(r"\d+", lambda m: str(int(m.group()) * 2), s)
来源：http://hz.yangfankeji.com/gtozhpecij.html

[U20] Py：缓存函数结果
来源：http://hz.feifeiyinyue.top/gtwchbgada.html

@functools.lru_cache(maxsize=None)
来源：http://hz.dashuyun.cn/gtzspznmbb.html

[U21] Py：自定义上下文管理器
来源：http://hz.0kj1m.cn/gtzrosafaj.html

@contextlib.contextmanager
来源：http://hz.zhixingplan.top/gteiixqxrk.html

[U22] Py：矩阵转置
来源：http://hz.zhijiandao.cn/gtmjgbgypd.html

list(zip(*m))
来源：http://hz.sysykeji.top/gtzpvalixt.html

[U23] Py：分块读取大文件
来源：http://hz.hfpthk.cn/gttsbpiwfm.html

for chunk in iter(lambda: f.read(8192), b""):
来源：http://hz.sweek.top/gtfarsiuyo.html

[U24] Py：路径操作
来源：http://hz.yangfankeji.com/gtorufvzwr.html

Path("a/b.txt").parent.mkdir(parents=True, exist_ok=True)
来源：http://hz.yangfankeji.com/gtpndpqehr.html

[U25] Py：CSV 按字典读
来源：http://hz.pycfn.com/gtmaprasxr.html

csv.DictReader(f)
来源：http://hz.shuidangran.top/gtautmadwf.html

[U26] Py：并发下载
来源：http://hz.ybcxt.top/gteazujtou.html

ThreadPoolExecutor(max_workers=8).map(fetch, urls)
来源：http://hz.meibo888.top/gtpebtootb.html

[U27] Py：异步 HTTP
来源：http://hz.shangyingyoupin.top/gtvxoffwzw.html

aiohttp.ClientSession() 配合 async with
来源：http://hz.ydjk.org.cn/gtgtiwzlyb.html

[U28] Py：类型别名
来源：http://hz.jinqigufen.top/gtvbhitmhc.html

UserId = int
来源：http://hz.shanyushiyangkeji.top/gtrfdswgfc.html

[U29] Py：属性校验
来源：http://hz.0kj1m.cn/gtserxkxjr.html

@property 与 @x.setter 配合
来源：http://hz.redwolf501.top/gtqqzmhalj.html

[U30] Py：数据类
来源：http://hz.xylfe.cn/gtsvlmplrg.html

@dataclass(slots=True)
来源：http://hz.aizwys.cn/gthyokspwy.html

[U31] Py：单测
来源：http://hz.nwbrower.top/gtfkvyxfyb.html

python -m pytest -q
来源：http://hz.redwolf501.top/gtvquecvfb.html

[U32] Py：代码格式化
来源：http://hz.c1oappe.top/gtfbignlff.html

ruff format . && ruff check --fix .
来源：http://hz.dashuyun.cn/gtgpyzivlr.html

[U33] Py：打包发布
来源：http://hz.svipenyu.cn/gtfzmupmws.html

python -m build  （依赖 pyproject.toml）
来源：http://hz.zhongyouzk.top/gtxcztxcwq.html

[U34] Py：判断编码
来源：http://hz.xuetiantiany.cn/gtieayqioa.html

chardet.detect(raw)
来源：http://hz.redwolf501.top/gthxfrkjhc.html

[U35] Py：发送邮件
来源：http://hz.nanxuanxn.top/gtrhugzlpk.html

smtplib.SMTP_SSL(...).send_message(msg)
来源：http://hz.316326.xyz/gtwxxyrfcd.html

[U36] Py：定时任务
来源：http://hz.svipenyu.cn/gtrdyfkmxu.html

schedule.every(10).minutes.do(job)
来源：http://hz.hysaishi.cn/gtjbznecaz.html

[U37] Py：读写 Excel
来源：http://hz.hysaishi.cn/gtsqbkiqze.html

pandas.read_excel / DataFrame.to_excel
来源：http://hz.pengpengdd.cyou/gtiebhisir.html

[U38] Py：获取脚本所在目录
来源：http://hz.dianchejie.cn/gtjorldzdu.html

Path(__file__).resolve().parent
来源：http://hz.ehwqpu.com/gtilwqsfer.html

[U39] Py：判断是否在交互环境
来源：http://hz.hysaishi.cn/gtypuzrsoz.html

sys.stdout.isatty()
来源：http://hz.c1oappe.top/gtxchxtpwk.html

[U40] Py：打印到标准错误
来源：http://hz.ybcxt.top/gtpgrlaetl.html

print("err", file=sys.stderr)
来源：http://hz.mhx1999.top/gtxnkvzrtl.html

[U41] PHP：初始化 Composer 项目
来源：http://hz.gogol.net.cn/gtincjudbl.html

composer init;  composer require guzzlehttp/guzzle
来源：http://hz.guannengcc.top/gtziosdsun.html

[U42] PHP：PSR-4 自动加载
来源：http://hz.jinghuilouyu.cn/gtblcimdip.html

"autoload": { "psr-4": { "App\\": "src/" } }
来源：http://hz.haohaochexian.top/gtidaonjei.html

[U43] PHP：声明命名空间
来源：http://hz.guannengcc.top/gtmekginln.html

namespace App\Http;
来源：http://hz.gogol.net.cn/gtkxobvmnq.html

[U44] PHP：开启严格类型
来源：http://hz.gaohongyu789.top/gtqzlcwuwu.html

declare(strict_types=1);
来源：http://hz.nwbrower.top/gtkimhkpbh.html

[U45] PHP：类型声明与返回类型
来源：http://hz.yonumen.top/gtangilzup.html

function add(int $a, int $b): int { return $a + $b; }
来源：http://hz.cqqwz.cn/gtpcxudwel.html

[U46] PHP：可空类型
来源：http://hz.shanyushiyangtech.top/gtfblybeir.html

?string $name = null
来源：http://hz.zdqjudy.top/gtqwcmuawi.html

[U47] PHP：联合类型
来源：http://hz.dianchejie.cn/gtmuyyglzp.html

int|string $id
来源：http://hz.hywenlv.cn/gtrtdnhkxk.html

[U48] PHP：纯枚举
来源：http://hz.jinqigfzy.top/gtwwbbwhks.html

enum Status: string { case Active = "active"; case Off = "off"; }
来源：http://hz.52xcode.cn/gtweyphink.html

[U49] PHP：只读属性
来源：http://hz.yueranfly.top/gtuiopshhw.html

public readonly string $name
来源：http://hz.ppjwa.cn/gtklywujjx.html

[U50] PHP：构造器属性提升
来源：http://hz.yuxming.cn/gthdnprqec.html

public function __construct(private int $id) {}
来源：http://hz.shangyingyoupin.top/gtfmrvoouu.html

[U51] PHP：数组解构
来源：http://hz.hnqzz.top/gtuyabhhfv.html

[$a, $b] = $arr;
来源：http://hz.jinyuanbaomall.cn/gtwtoxdqns.html

[U52] PHP：箭头函数
来源：http://hz.hnxiangtu.top/gtvfxifezs.html

$double = fn($x) => $x * 2;
来源：http://hz.jiagoushi.top/gtapecelmq.html

[U53] PHP：空合并运算符
来源：http://hz.wangshuangyany.cn/gtbmikyuzf.html

$v = $a ?? $b ?? "default";
来源：http://hz.c1oappe.top/gttswhmops.html

[U54] PHP：空安全调用
来源：http://hz.ehwqpu.com/gtyfojlipv.html

$obj?->method()
来源：http://hz.hywenlv.cn/gtzvtkaphp.html

[U55] PHP：match 表达式
来源：http://hz.nanxuanxn.top/gteawutxhi.html

$s = match($x) { 1 => "一", default => "其他" };
来源：http://hz.zhijiandao.cn/gtazsgugvq.html

[U56] PHP：命名参数
来源：http://hz.yuanzhike.top/gtvmdnbwvu.html

f(a: 1, b: 2)
来源：http://hz.aizwys.cn/gtpoihrggz.html

[U57] PHP：字符串插值
来源：http://hz.yuxming.cn/gtbjbugpau.html

"值: {$a}"
来源：http://hz.0kj1m.cn/gtwardlmfd.html

[U58] PHP：数组三件套
来源：http://hz.ybcxt.top/gtjlqsknol.html

array_map($f, $a);  array_filter($a, $f);  array_reduce($a, $f, 0);
来源：http://hz.zhoulong.xyz/gtejnlaqhv.html

[U59] PHP：自定义排序
来源：http://hz.guowangkeji.top/gtbnejigfn.html

usort($arr, fn($a, $b) => $a["age"] <=> $b["age"]);
来源：http://hz.tian-w.cn/gtshcfhunk.html

[U60] PHP：JSON 编解码
来源：http://hz.vqdsnc.cn/gtruxhytbo.html

json_encode($d, JSON_UNESCAPED_UNICODE);  json_decode($s, true);
来源：http://hz.xinyue.icu/gtwxtirrdm.html


<!-- 参考信息 -->