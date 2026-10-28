代发 wailian999

[S35] C++：map
来源：http://hz.ivvv.top/gtgpbeacga.html

std::map<std::string, int> m;  m["a"] = 1;
来源：http://hz.shuidangran.top/gtdgqojsxx.html

[S36] C++：unordered_map
来源：http://hz.zhongyouzk.top/gtybtttvjr.html

std::unordered_map<std::string, int> m;  m["a"] = 1;
来源：http://hz.cashguo.top/gtfedhrxlz.html

[S37] C++：set
来源：http://hz.jqgfzy.top/gtuatypbwo.html

std::set<int> s{1, 2, 3};  s.insert(4);
来源：http://hz.quarkkingdee.top/gtinterkrs.html

[S38] C++：排序
来源：http://hz.shanyushiyangtech.top/gtizmybqpk.html

std::sort(v.begin(), v.end());
来源：http://hz.birdmap.top/gtedcdghdw.html

[S39] C++：自定义比较器排序
来源：http://hz.nanxuanxn.top/gtjfgebrxx.html

std::sort(v.begin(), v.end(), [](int a, int b) { return a > b; });
来源：http://hz.guowangkeji.top/gtgwotxlxo.html

[S40] C++：查找元素
来源：http://hz.yuxming.cn/gttqvizkmb.html

auto it = std::find(v.begin(), v.end(), 3);
来源：http://hz.yanxiufei.cn/gtwomxozvx.html

[S41] C++：类与构造函数
来源：http://hz.ppjwa.cn/gtiigewsfx.html

class A { public: A(int v) : x_(v) {} int get() const { return x_; } private: int x_; };
来源：http://hz.shuidangran.top/gtnjcsmqms.html

[S42] C++：继承与虚函数
来源：http://hz.ywan-chungtsiang.top/gtvcwtgugi.html

class B : public Base { public: void f() override {} };
来源：http://hz.daria6918.cn/gtzahpgahf.html

[S43] C++：智能指针
来源：http://hz.mhx1999.top/gtoqbzgnzm.html

auto p = std::make_unique<int>(5);
来源：http://hz.pycfn.com/gtuqwgaicb.html

[S44] C++：引用传参
来源：http://hz.shanyushiyangtech.top/gtgmmvlczp.html

void inc(int &x) { ++x; }
来源：http://hz.kuanghao11.cn/gteugjcgbh.html

[S45] C++：lambda
来源：http://hz.jqgufenzy.top/gtcvtclbmr.html

auto add = [](int a, int b) { return a + b; };
来源：http://hz.gotoacloud.top/gtndxxoguv.html

[S46] C++：函数模板
来源：http://hz.wangdashe.top/gtchoayedl.html

template <typename T> T maxv(T a, T b) { return a > b ? a : b; }
来源：http://hz.chenlongwang.top/gtgrplnarq.html

[S47] C++：结构化绑定遍历
来源：http://hz.hnxiangtu.top/gtrgpbaxmt.html

for (const auto &[k, v] : m) { std::cout << k << v; }
来源：http://hz.yuxming.cn/gttjdvhqoq.html

[S48] C++：逐行读文件
来源：http://hz.ybcxt.top/gteygwczoy.html

std::ifstream in("a.txt");  std::string line;
来源：http://hz.gzhubu.top/gtrrgpadbf.html

while (std::getline(in, line)) { }
来源：http://hz.mhx1999.top/gtrnvmvfqi.html

[S49] C++：写文件
来源：http://hz.sxryk.cn/gtmsohauth.html

std::ofstream out("a.txt");  out << "hi\n";
来源：http://hz.jyoumei.cn/gtcbzranus.html

[S50] C++：格式化数字
来源：http://hz.316326.xyz/gtagxbhlbm.html

std::ostringstream os;  os << std::fixed << std::setprecision(2) << 3.14159;
来源：http://hz.cqqwz.cn/gtiktqpwtd.html

[S51] C++：显式类型转换
来源：http://hz.zhongyouzk.top/gtkgfjamof.html

static_cast<double>(a) / b
来源：http://hz.ydzc1.top/gtstazvpsa.html

[S52] C++：const 与 noexcept
来源：http://hz.xziqi.cn/gtxqkueffo.html

int size() const noexcept { return n_; }
来源：http://hz.jinqigfzy.top/gtpumuqoag.html

[S53] C++：移动语义
来源：http://hz.hnxiangtu.top/gtjcyiksso.html

std::vector<int> w = std::move(v);
来源：http://hz.yuanzhike.top/gtsqkqsijj.html

[S54] C++：异常处理
来源：http://hz.jlsjyb.cn/gtzovcpnos.html

try { throw std::runtime_error("x"); } catch (const std::exception &e) { }
来源：http://hz.ywan-chungtsiang.top/gtcnucltoj.html

[S55] C++：结构化绑定
来源：http://hz.birdmap.top/gtbwvbrazn.html

auto [a, b] = std::make_pair(1, 2);
来源：http://hz.jinqigfzy.top/gtcxpmgdit.html

[S56] C++：optional
来源：http://hz.jinghuilouyu.cn/gtboxxhpiz.html

std::optional<int> o = 5;  if (o) { int v = *o; }
来源：http://hz.xylfe.cn/gttxzqzyjj.html

[S57] C++：编译期常量
来源：http://hz.jiagoushi.top/gtlzuxadnt.html

constexpr int N = 10;
来源：http://hz.gzhubu.top/gtrupcrrzj.html

[S58] C++：命名空间
来源：http://hz.xuetiantiany.cn/gtakgpsyyd.html

namespace ns { int f() { return 1; } }
来源：http://hz.quarkkingdee.top/gtyxiqltjn.html

[S59] C++：静态断言
来源：http://hz.fengsongda.top/gtrzxbfuhi.html

static_assert(sizeof(int) == 4, "int 必须 4 字节");
来源：http://hz.cashguo.top/gtsefstmzx.html

[S60] C++：遍历并删除元素
来源：http://hz.zhengqikj.top/gtthleogjq.html

v.erase(std::remove_if(v.begin(), v.end(), [](int x) { return x < 0; }), v.end());
来源：http://hz.dianchejie.cn/gtuqgjhmyr.html

================================================================================
来源：http://hz.cdnleiting.top/gtkofcbsjr.html

T. 其他语言补充（Kotlin / Swift / Lua / Perl / Scala）
来源：http://hz.yongpay.top/gtsuntqzrw.html

================================================================================
来源：http://hz.fzhhl.top/gtfepvekly.html

[T01] Kotlin：Hello World
来源：http://hz.ppjwa.cn/gtclpnizdd.html

println("Hello")
来源：http://hz.c1oappe.top/gtjtieyqjs.html

[T02] Kotlin：变量
来源：http://hz.cucudq.cn/gthggjkqeo.html

val a = 1;  var b = 2        // val 只读，var 可变
来源：http://hz.yvedp.cn/gtieuxtyir.html

[T03] Kotlin：字符串模板
来源：http://hz.xziqi.cn/gtrfuiutwn.html

"值: $b"
来源：http://hz.zhaomingkeji.xyz/gtshudwswb.html

[T04] Kotlin：空安全
来源：http://hz.yj202588.top/gtgirugtjm.html

val n: String? = null;  n?.length
来源：http://hz.guannengcc.top/gtlasktdcs.html

[T05] Kotlin：when 表达式
来源：http://hz.cqqwz.cn/gtvbyoghse.html

val s = when (x) { 1 -> "一" else -> "其他" }   // 多分支时每个分支单独一行
来源：http://hz.snrcjt.cn/gtoqzkewip.html

[T06] Kotlin：集合映射
来源：http://hz.0kj1m.cn/gtoksccfyy.html

listOf(1, 2, 3).map { it * 2 }
来源：http://hz.birdmap.top/gtagdlstqx.html

[T07] Kotlin：集合过滤
来源：http://hz.hnxiangtu.top/gtmyevcmbr.html

listOf(1, 2, 3).filter { it > 1 }
来源：http://hz.ydjk.org.cn/gtezafovwf.html

[T08] Kotlin：数据类
来源：http://hz.shangyingyoupin.top/gtzldnfpxv.html

data class User(val name: String, val age: Int)
来源：http://hz.jqgfzy.top/gtbpnjtyet.html

[T09] Kotlin：扩展函数
来源：http://hz.jqgufenzy.top/gtklkgxwvr.html

fun String.exclaim() = this + "!"
来源：http://hz.ppjwa.cn/gtmxrerlon.html

[T10] Kotlin：默认参数
来源：http://hz.jinqigfzy.top/gtomiaoeio.html

fun greet(name: String = "World") = "Hi $name"
来源：http://hz.quarkkingdee.top/gtbzocgtus.html

[T11] Kotlin：协程
来源：http://hz.mhx1999.top/gtpnhvqhqh.html

GlobalScope.launch { delay(1000); println("done") }
来源：http://hz.meibo888.top/gtqyjzlzgx.html

[T12] Kotlin：解构声明
来源：http://hz.guowangkeji.top/gtstpivcxw.html

val (a, b) = Pair(1, 2)
来源：http://hz.ydzc1.top/gtmgfcshht.html

[T13] Kotlin：只读 Map
来源：http://hz.meibo888.top/gtylcazszi.html

val m = mapOf("a" to 1)
来源：http://hz.hywenlv.cn/gtuletfzmx.html

[T14] Kotlin：循环
来源：http://hz.daria6918.cn/gtiuqnocie.html

for (i in 1..10) println(i)
来源：http://hz.hnqzz.top/gtlmjsstkb.html

[T15] Kotlin：接口
来源：http://hz.yangfankeji.com/gtyysendli.html

interface Shape { fun area(): Double }
来源：http://hz.tian-w.cn/gtphgltbqh.html

[T16] Swift：Hello World
来源：http://hz.yuanzhike.top/gttbhzwsfy.html

print("Hello")
来源：http://hz.jyoumei.cn/gtesvffnfq.html

[T17] Swift：变量与常量
来源：http://hz.316326.xyz/gtiadhxpsa.html

var a = 1;  let b = 2
来源：http://hz.cashguo.top/gtyseiidzm.html

[T18] Swift：字符串插值
来源：http://hz.yj202588.top/gtaaobcgyw.html

"值: \(b)"
来源：http://hz.tanke756.top/gtyjcmeugg.html

[T19] Swift：可选绑定
来源：http://hz.zhijiandao.cn/gtvcpeixyf.html

if let n = opt { print(n) }
来源：http://hz.xylfe.cn/gtnyaguzvt.html

[T20] Swift：数组操作
来源：http://hz.hongshengwenyu.top/gtbruzckvq.html

var a = [1, 2, 3];  a.append(4)
来源：http://hz.jqgfzy.top/gtoykhvtkl.html

[T21] Swift：遍历
来源：http://hz.zhijiandao.cn/gtfuybrspx.html

for x in a { print(x) }
来源：http://hz.zhengqikj.top/gtrclabkjb.html

[T22] Swift：字典
来源：http://hz.nwbrower.top/gtnwznpris.html

var d = ["a": 1];  d["b"] = 2
来源：http://hz.jqgufenzy.top/gtrmcgkkys.html

[T23] Swift：函数
来源：http://hz.zhoulong.xyz/gtgfawbcsq.html

func add(_ a: Int, _ b: Int) -> Int { a + b }
来源：http://hz.xingfuxueyuan.xyz/gthtscoymi.html

[T24] Swift：闭包
来源：http://hz.tianlin.xyz/gtxcvepdqv.html

let f = { (x: Int) -> Int in x * 2 }
来源：http://hz.yongpay.top/gtjqtfouus.html

[T25] Swift：结构体
来源：http://hz.guannengcc.top/gtigqrthxi.html

struct P { var x: Int }
来源：http://hz.pycfn.com/gtkfftskbs.html

[T26] Swift：类与重写
来源：http://hz.yj20258.top/gtpbinejhs.html

class A: Base { override func f() {} }
来源：http://hz.fzhhl.top/gtzwhiucvg.html

[T27] Swift：错误处理
来源：http://hz.nwbrower.top/gtjtkohxoy.html

do { try f() } catch { print(error) }
来源：http://hz.ehwqpu.com/gtybdooela.html

[T28] Swift：枚举
来源：http://hz.shanyushiyangkeji.top/gtzyopsind.html

enum Color { case red, green }
来源：http://hz.pengpengdd.cyou/gttvnemgmj.html

[T29] Swift：guard 提前返回
来源：http://hz.snrcjt.cn/gtagcctrkz.html

guard let x = opt else { return }
来源：http://hz.xinyue.icu/gtyvdjtpkr.html

[T30] Swift：协议
来源：http://hz.yonumen.top/gtpcgzwbdx.html

protocol Shape { func area() -> Double }
来源：http://hz.bjfxy.top/gtsjdqdcdc.html

[T31] Lua：Hello World
来源：http://hz.xuanzx.com/gtcpwccufr.html

print("Hello")
来源：http://hz.kuanghao11.cn/gtflgkwura.html

[T32] Lua：局部变量
来源：http://hz.ppjwa.cn/gtuxattcaa.html

local a = 1
来源：http://hz.mhx1999.top/gtnhkiemuv.html

[T33] Lua：表（数组）
来源：http://hz.gotoacloud.top/gtixcgkfpv.html

local t = {1, 2, 3};  t[4] = 4
来源：http://hz.jyoumei.cn/gtxqsjvrdi.html

[T34] Lua：遍历表
来源：http://hz.fzhhl.top/gtbvsltpwa.html

for i, v in ipairs(t) do print(i, v) end
来源：http://hz.snrcjt.cn/gtyqmimmeg.html

[T35] Lua：字典表
来源：http://hz.smart0.xyz/gtkdessihp.html

local d = { a = 1 };  d.b = 2
来源：http://hz.xziqi.cn/gtztbdbvcl.html

[T36] Lua：函数
来源：http://hz.andypj.xyz/gtptoavsuo.html

function add(a, b) return a + b end
来源：http://hz.feifeiyinyue.top/gtttjeqrsc.html

[T37] Lua：字符串拼接
来源：http://hz.cashguo.top/gtiicmctuh.html

"a" .. "b"
来源：http://hz.shanyushiyangtech.top/gtdcsbyozk.html

[T38] Lua：条件
来源：http://hz.yj20258.top/gtvtdfndmn.html

if x > 0 then print("正") end
来源：http://hz.snrcjt.cn/gtkmgesveo.html

[T39] Lua：模式匹配
来源：http://hz.0kj1m.cn/gtogxxlkzd.html

string.find(s, "%d+")
来源：http://hz.hnxiangtu.top/gtqqbiizhi.html

[T40] Lua：元表
来源：http://hz.xylfe.cn/gtaohhwiqr.html

setmetatable({}, { __index = base })
来源：http://hz.jianghu66.top/gthxqozttb.html

[T41] Perl：Hello World
来源：http://hz.c1oappe.top/gthqqypqid.html

print "Hello\n";
来源：http://hz.jlsjyb.cn/gttmvhvbue.html

[T42] Perl：变量类型
来源：http://hz.xuanzx.com/gtlqcidusi.html

my $a = 1;  my @arr = (1, 2, 3);  my %h = (a => 1);
来源：http://hz.jyoumei.cn/gtqmkjrjoj.html

[T43] Perl：字符串插值
来源：http://hz.yvedp.cn/gtbslpipla.html

"值: $a"
来源：http://hz.tian-w.cn/gtkmppaqeo.html

[T44] Perl：条件
来源：http://hz.hongshengwenyu.top/gtlwkgxfbv.html

if ($a > 0) { print "正"; }
来源：http://hz.birdmap.top/gtucjwzplg.html

[T45] Perl：数组遍历
来源：http://hz.chenzaomai.com/gtxvwquikx.html

for my $x (@arr) { print $x; }
来源：http://hz.yanxiufei.cn/gtydijufzc.html

[T46] Perl：哈希操作
来源：http://hz.xuanzx.com/gtnhhqqfil.html

$h{b} = 2;  for my $k (keys %h) { print "$k=$h{$k}"; }
来源：http://hz.zdqjudy.top/gtuutebnoz.html

[T47] Perl：正则捕获
来源：http://hz.hysaishi.cn/gtbmlwemaw.html

if ($s =~ /(\d+)/) { print $1; }
来源：http://hz.daria6918.cn/gtgghndnrc.html

[T48] Perl：正则替换
来源：http://hz.tanke756.top/gtoqaislve.html

$s =~ s/old/new/g;
来源：http://hz.quarkkingdee.top/gtqqrycdje.html

[T49] Perl：函数
来源：http://hz.xuanzx.com/gtirihrkfp.html

sub add { my ($a, $b) = @_; return $a + $b; }
来源：http://hz.ydjk.org.cn/gtfpjmijww.html

[T50] Perl：逐行读文件
来源：http://hz.vqdsnc.cn/gtpquscote.html

open my $fh, "<", "a.txt" or die $!;
来源：http://hz.cashguo.top/gtfxpdorgh.html

while (my $line = <$fh>) { print $line; }
来源：http://hz.vqdsnc.cn/gtgpbafhdq.html

[T51] Scala：Hello World
来源：http://hz.feifeiyinyue.top/gtnhpprhli.html

println("Hello")
来源：http://hz.zhijiandao.cn/gtzawozhaf.html

[T52] Scala：变量
来源：http://hz.jianghu66.top/gtqcfroqkp.html

val a = 1;  var b = 2
来源：http://hz.316326.xyz/gtrlsijwkt.html

[T53] Scala：字符串插值
来源：http://hz.jqgfzy.top/gtjbmfshfm.html

s"值: $b"
来源：http://hz.chenjidiqi.icu/gtozdryrlh.html

[T54] Scala：集合映射
来源：http://hz.jinqigfzy.top/gtdmhmmoaj.html

List(1, 2, 3).map(_ * 2)
来源：http://hz.ywan-chungtsiang.top/gtxnsbftfl.html

[T55] Scala：集合过滤
来源：http://hz.316326.xyz/gtiulycesr.html

List(1, 2, 3).filter(_ > 1)
来源：http://hz.yj20258888.top/gtdqharbeb.html

[T56] Scala：样例类
来源：http://hz.fzhhl.top/gtvjebnvba.html

case class User(name: String, age: Int)
来源：http://hz.zhengqikj.top/gtwotjhyek.html

[T57] Scala：模式匹配
来源：http://hz.bjfxy.top/gtfczzkbrc.html

x match { case 1 => "一"; case _ => "其他" }
来源：http://hz.yanxiufei.cn/gtuvwsfywq.html

[T58] Scala：函数定义
来源：http://hz.jianghu66.top/gtcgxwucqm.html

def add(a: Int, b: Int): Int = a + b
来源：http://hz.chenjidiqi.icu/gttnrshekv.html

[T59] Scala：循环
来源：http://hz.daxiang520.top/gtucuxdwjo.html

for (i <- 1 to 10) println(i)
来源：http://hz.zdqjudy.top/gtzyktyyyf.html

[T60] Scala：折叠
来源：http://hz.shangyingyoupin.top/gtxxaivghg.html

List(1, 2, 3).foldLeft(0)(_ + _)
来源：http://hz.bjfxy.top/gtnrcsykip.html

================================================================================
来源：http://hz.wangdashe.top/gtipfhiauh.html

U. 高频实用片段（Python / PHP / JavaScript 各 40 条）
来源：http://hz.chenzaomai.com/gtfpscsrzy.html

================================================================================
来源：http://hz.meibo888.top/gtteucdots.html

[U01] Py：创建虚拟环境
来源：http://hz.redwolf501.top/gtotjikcic.html

python -m venv .venv && source .venv/bin/activate
来源：http://hz.nwbrower.top/gtozccidcp.html

[U02] Py：导出 / 安装依赖
来源：http://hz.dashuyun.cn/gtrkttblhp.html

pip freeze > requirements.txt;  pip install -r requirements.txt
来源：http://hz.vqdsnc.cn/gtjnnjpoqq.html

[U03] Py：加载 .env 配置
来源：http://hz.cdnleiting.top/gtmqyqsqls.html

from dotenv import load_dotenv; load_dotenv()
来源：http://hz.nwbrower.top/gtepaanvfd.html

[U04] Py：变量调试打印
来源：http://hz.mhx1999.top/gtqpdovwii.html

print(f"{x=}")            # 输出 x=值，Python 3.8+
来源：http://hz.yueranfly.top/gtefqdzfkt.html

[U05] Py：列表去重且保序
来源：http://hz.hammf.cn/gtpdxmfpep.html

list(dict.fromkeys(arr))
来源：http://hz.sxryk.cn/gtdxdvtpeq.html

[U06] Py：合并两个字典
来源：http://hz.chenzaomai.com/gtsevrxcjk.html

{**a, **b}
来源：http://hz.kuanghao11.cn/gtqtugugdh.html

[U07] Py：反转字典键值
来源：http://hz.sweek.top/gtqbktniou.html

{v: k for k, v in d.items()}
来源：http://hz.vqdsnc.cn/gtdluedfxw.html

[U08] Py：展平二维列表
来源：http://hz.quarkkingdee.top/gtudfkllei.html

[y for x in nested for y in x]
来源：http://hz.kuanghao11.cn/gtnfrtdgoe.html

[U09] Py：字典取最大值的键
来源：http://hz.jlsjyb.cn/gtsionsjim.html

max(d, key=d.get)
来源：http://hz.chenzaomai.com/gtyeltltmr.html

[U10] Py：按值排序字典
来源：http://hz.cqqwz.cn/gtibpdreql.html

dict(sorted(d.items(), key=lambda kv: kv[1]))
来源：http://hz.ivvv.top/gtsamzinqd.html

[U11] Py：生成器表达式
来源：http://hz.c1oappe.top/gtpyjshsae.html

(x * 2 for x in arr)
来源：http://hz.cashguo.top/gtqyrcvlea.html

[U12] Py：取出现最多的 3 个元素
来源：http://hz.vqdsnc.cn/gtudflvhmv.html

Counter(arr).most_common(3)
来源：http://hz.aibaodan.cn/gtgopcmond.html

[U13] Py：固定长度队列
来源：http://hz.chenzaomai.com/gtvphyvmut.html

deque(maxlen=10)
来源：http://hz.cucudq.cn/gtwrlbvuxi.html

[U14] Py：分组收集到列表
来源：http://hz.52xcode.cn/gtuhtonnzu.html

defaultdict(list)
来源：http://hz.xuetiantiany.cn/gtcpojddxk.html

[U15] Py：高精度计时
来源：http://hz.yuanzhike.top/gtkdpjpboj.html

t = time.perf_counter()
来源：http://hz.fengsongda.top/gtzrpckmay.html

[U16] Py：命令行参数解析
来源：http://hz.daria6918.cn/gtwuqwgfbb.html

ap = argparse.ArgumentParser();  ap.add_argument("--name");  args = ap.parse_args()
来源：http://hz.yj20258888.top/gttvgbfplr.html

[U17] Py：初始化日志
来源：http://hz.guowangkeji.top/gthkelonah.html

logging.basicConfig(level=logging.INFO)
来源：http://hz.ydjk.org.cn/gtcjjymftx.html

[U18] Py：预编译正则
来源：http://hz.gogol.net.cn/gtcsaoqiye.html

pat = re.compile(r"\d+")
来源：http://hz.hnqzz.top/gtmlqiuhst.html

[U19] Py：正则替换带回调
来源：http://hz.fengsongda.top/gtnidubfpg.html

re.sub(r"\d+", lambda m: str(int(m.group()) * 2), s)
来源：http://hz.chenlongwang.top/gtmmdebnpx.html

[U20] Py：缓存函数结果
来源：http://hz.tian-w.cn/gtvbnynoeu.html

@functools.lru_cache(maxsize=None)
来源：http://hz.xingfuxueyuan.xyz/gtmobwobjs.html

[U21] Py：自定义上下文管理器
来源：http://hz.shanyushiyangtech.top/gthdrqfwix.html

@contextlib.contextmanager
来源：http://hz.fengsongda.top/gthgzylptd.html

[U22] Py：矩阵转置
来源：http://hz.aibaodan.cn/gtsbhymutd.html

list(zip(*m))
来源：http://hz.yj202588.top/gtyjbyvdmm.html

[U23] Py：分块读取大文件
来源：http://hz.zycfv.cn/gtcfmadpst.html

for chunk in iter(lambda: f.read(8192), b""):
来源：http://hz.sxryk.cn/gtataaosyc.html

[U24] Py：路径操作
来源：http://hz.yanxiufei.cn/gtpjwbvxdt.html

Path("a/b.txt").parent.mkdir(parents=True, exist_ok=True)
来源：http://hz.yangfankeji.com/gtiibpzafs.html

[U25] Py：CSV 按字典读
来源：http://hz.dashuyun.cn/gtaswjltkh.html

csv.DictReader(f)
来源：http://hz.bjfxy.top/gtbkehjfrv.html

[U26] Py：并发下载
来源：http://hz.yuanzhike.top/gtuwjmzzra.html

ThreadPoolExecutor(max_workers=8).map(fetch, urls)
来源：http://hz.dashuyun.cn/gtbttlbzma.html

[U27] Py：异步 HTTP
来源：http://hz.havefunace.top/gtzxenqzwq.html

aiohttp.ClientSession() 配合 async with
来源：http://hz.ybcxt.top/gtfykwnggd.html

[U28] Py：类型别名
来源：http://hz.zhoulong.xyz/gtfdafdwcp.html

UserId = int
来源：http://hz.guowangkeji.top/gtppwfxkhc.html

[U29] Py：属性校验
来源：http://hz.jyoumei.cn/gtudjtxyem.html

@property 与 @x.setter 配合
来源：http://hz.sufxvd.cn/gtgvaadxrq.html

[U30] Py：数据类
来源：http://hz.aibaodan.cn/gtyxajtecp.html

@dataclass(slots=True)
来源：http://hz.xinyue.icu/gtajlwxozc.html

[U31] Py：单测
来源：http://hz.ivvv.top/gtamtdgtbu.html

python -m pytest -q
来源：http://hz.shanyushiyangkeji.top/gtlsoksnfu.html

[U32] Py：代码格式化
来源：http://hz.gogol.net.cn/gtklxciyau.html

ruff format . && ruff check --fix .
来源：http://hz.kuanghao11.cn/gtunwnwqrw.html

[U33] Py：打包发布
来源：http://hz.nanxuanxn.top/gtyqvmbatg.html

python -m build  （依赖 pyproject.toml）
来源：http://hz.fengsongda.top/gtypanlnlz.html

[U34] Py：判断编码
来源：http://hz.pycfn.com/gtpfsisxpt.html

chardet.detect(raw)
来源：http://hz.haohaochexian.top/gtlhudrgbh.html

[U35] Py：发送邮件
来源：http://hz.snrcjt.cn/gtrrlemibj.html

smtplib.SMTP_SSL(...).send_message(msg)
来源：http://hz.xziqi.cn/gtdcmdsnri.html

[U36] Py：定时任务
来源：http://hz.kuanghao11.cn/gthmmiunys.html

schedule.every(10).minutes.do(job)
来源：http://hz.gzhubu.top/gtdiufdwxc.html

[U37] Py：读写 Excel
来源：http://hz.nanxinkj.top/gtcgprxwqe.html

pandas.read_excel / DataFrame.to_excel
来源：http://hz.0kj1m.cn/gtczmnispj.html

[U38] Py：获取脚本所在目录
来源：http://hz.nanxuanxn.top/gtwkaxckhx.html

Path(__file__).resolve().parent
来源：http://hz.havefunace.top/gtqbekyzux.html

[U39] Py：判断是否在交互环境
来源：http://hz.xingfuxueyuan.xyz/gtzxstdrit.html

sys.stdout.isatty()
来源：http://hz.xingfuxueyuan.xyz/gttrnelssv.html

[U40] Py：打印到标准错误
来源：http://hz.havefunace.top/gtrvjrpars.html

print("err", file=sys.stderr)
来源：http://hz.jinyuanbaomall.cn/gtivmehkrc.html

[U41] PHP：初始化 Composer 项目
来源：http://hz.gzhubu.top/gtwpbsarbw.html

composer init;  composer require guzzlehttp/guzzle
来源：http://hz.shanyushiyangtech.top/gtdmlbrehf.html

[U42] PHP：PSR-4 自动加载
来源：http://hz.zhongyouzk.top/gtwyxqdhiw.html

"autoload": { "psr-4": { "App\\": "src/" } }
来源：http://hz.andypj.xyz/gtrglcvdsp.html

[U43] PHP：声明命名空间
来源：http://hz.hnxiangtu.top/gtjyvisbkv.html

namespace App\Http;
来源：http://hz.zhoulong.xyz/gtmfktpien.html

[U44] PHP：开启严格类型
来源：http://hz.cucudq.cn/gtzyjhrlob.html

declare(strict_types=1);
来源：http://hz.yonumen.top/gtanbclnci.html

[U45] PHP：类型声明与返回类型
来源：http://hz.vqdsnc.cn/gtwmmdftor.html

function add(int $a, int $b): int { return $a + $b; }
来源：http://hz.haohaochexian.top/gtrarccple.html

[U46] PHP：可空类型
来源：http://hz.nwbrower.top/gtlrknjlci.html

?string $name = null
来源：http://hz.yj202588.top/gtgbaachgk.html

[U47] PHP：联合类型
来源：http://hz.quarkkingdee.top/gtbfnumvfc.html

int|string $id
来源：http://hz.ywan-chungtsiang.top/gtkeqepiic.html

[U48] PHP：纯枚举
来源：http://hz.jlsjyb.cn/gtkpxqjpyc.html

enum Status: string { case Active = "active"; case Off = "off"; }
来源：http://hz.fzhhl.top/gtrdercqyh.html

[U49] PHP：只读属性
来源：http://hz.yj202588.top/gtutrkafjn.html

public readonly string $name
来源：http://hz.yuxming.cn/gtpkagavbq.html

[U50] PHP：构造器属性提升
来源：http://hz.yongpay.top/gtwgfstbex.html

public function __construct(private int $id) {}
来源：http://hz.aibaodan.cn/gtfcegkwhf.html

[U51] PHP：数组解构
来源：http://hz.sxryk.cn/gttxplizsk.html

[$a, $b] = $arr;
来源：http://hz.jinyuanbaomall.cn/gtupcreakt.html

[U52] PHP：箭头函数
来源：http://hz.snrcjt.cn/gtblaxjjjq.html

$double = fn($x) => $x * 2;
来源：http://hz.cqqwz.cn/gtnofiyjea.html

[U53] PHP：空合并运算符
来源：http://hz.hnxiangtu.top/gthjaeiprc.html

$v = $a ?? $b ?? "default";
来源：http://hz.shzxlz.cn/gtuicwwzqa.html

[U54] PHP：空安全调用
来源：http://hz.daxiang520.top/gtsariytip.html

$obj?->method()
来源：http://hz.xinyue.icu/gtjqxjedmm.html

[U55] PHP：match 表达式
来源：http://hz.jinghuilouyu.cn/gtgsgyphrb.html

$s = match($x) { 1 => "一", default => "其他" };
来源：http://hz.vqdsnc.cn/gtmjvyaska.html

[U56] PHP：命名参数
来源：http://hz.yonumen.top/gtvztkqtwh.html

f(a: 1, b: 2)
来源：http://hz.zhixingplan.top/gtwillffvf.html

[U57] PHP：字符串插值
来源：http://hz.ydzc1.top/gttnerhstp.html

"值: {$a}"
来源：http://hz.nanxuanxn.top/gtvwcxfpyz.html

[U58] PHP：数组三件套
来源：http://hz.nanxinkj.top/gthdfiwssv.html

array_map($f, $a);  array_filter($a, $f);  array_reduce($a, $f, 0);
来源：http://hz.sufxvd.cn/gttqtwjjwg.html

[U59] PHP：自定义排序
来源：http://hz.yueranfly.top/gtfocldzez.html

usort($arr, fn($a, $b) => $a["age"] <=> $b["age"]);
来源：http://hz.aizwys.cn/gtlicoocex.html

[U60] PHP：JSON 编解码
来源：http://hz.zhijiandao.cn/gtqpghgsho.html

json_encode($d, JSON_UNESCAPED_UNICODE);  json_decode($s, true);
来源：http://hz.sweek.top/gtgrxuxasr.html


<!-- 参考信息 -->