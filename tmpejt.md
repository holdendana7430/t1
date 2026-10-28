代发 wailian999

[S33] C++：vector 增删
来源：http://hz.jinghuilouyu.cn/gtbaeeoqlm.html

std::vector<int> v{1, 2, 3};  v.push_back(4);
来源：http://hz.yuanzhike.top/gtbnsugmyo.html

[S34] C++：遍历 vector
来源：http://hz.xylfe.cn/gtwchbgzpb.html

for (auto &x : v) { std::cout << x; }
来源：http://hz.mhx1999.top/gtfuciqvrw.html

[S35] C++：map
来源：http://hz.iojbl.cn/gtppvmzmfa.html

std::map<std::string, int> m;  m["a"] = 1;
来源：http://hz.havefunace.top/gtyfinkddk.html

[S36] C++：unordered_map
来源：http://hz.gotoacloud.top/gtzxhtszvb.html

std::unordered_map<std::string, int> m;  m["a"] = 1;
来源：http://hz.tanke756.top/gtqndmpxgh.html

[S37] C++：set
来源：http://hz.ehwqpu.com/gtmfskhyqw.html

std::set<int> s{1, 2, 3};  s.insert(4);
来源：http://hz.guannengcc.top/gtriyjcyvk.html

[S38] C++：排序
来源：http://hz.gotoacloud.top/gthskpdapj.html

std::sort(v.begin(), v.end());
来源：http://hz.sweek.top/gtqfzvgubn.html

[S39] C++：自定义比较器排序
来源：http://hz.guannengcc.top/gtxmlwcmtw.html

std::sort(v.begin(), v.end(), [](int a, int b) { return a > b; });
来源：http://hz.gogol.net.cn/gtckhlaopw.html

[S40] C++：查找元素
来源：http://hz.zhiwuduotai.top/gtpkpwtbnp.html

auto it = std::find(v.begin(), v.end(), 3);
来源：http://hz.guannengcc.top/gtcssebupi.html

[S41] C++：类与构造函数
来源：http://hz.hfpthk.cn/gtptarpdpm.html

class A { public: A(int v) : x_(v) {} int get() const { return x_; } private: int x_; };
来源：http://hz.sufxvd.cn/gtbyvvrwzb.html

[S42] C++：继承与虚函数
来源：http://hz.cheryme.top/gtavbzyohd.html

class B : public Base { public: void f() override {} };
来源：http://hz.redwolf501.top/gtcsajevrc.html

[S43] C++：智能指针
来源：http://hz.meibo888.top/gthwzskfci.html

auto p = std::make_unique<int>(5);
来源：http://hz.hfpthk.cn/gtixnxowrs.html

[S44] C++：引用传参
来源：http://hz.wangshuangyany.cn/gthjytjzna.html

void inc(int &x) { ++x; }
来源：http://hz.nwbrower.top/gtmwkkbjqe.html

[S45] C++：lambda
来源：http://hz.zhengqikj.top/gtqqxvutkm.html

auto add = [](int a, int b) { return a + b; };
来源：http://hz.daxiang520.top/gtuaklwgqw.html

[S46] C++：函数模板
来源：http://hz.ywan-chungtsiang.top/gtypqmbmqv.html

template <typename T> T maxv(T a, T b) { return a > b ? a : b; }
来源：http://hz.shanyushiyangtech.top/gtxpiijtqr.html

[S47] C++：结构化绑定遍历
来源：http://hz.birdmap.top/gttsepeiuf.html

for (const auto &[k, v] : m) { std::cout << k << v; }
来源：http://hz.snrcjt.cn/gtkfqpsbkx.html

[S48] C++：逐行读文件
来源：http://hz.yuanzhike.top/gtdwqanmda.html

std::ifstream in("a.txt");  std::string line;
来源：http://hz.cheryme.top/gtoewnavuo.html

while (std::getline(in, line)) { }
来源：http://hz.vqdsnc.cn/gtheemoslw.html

[S49] C++：写文件
来源：http://hz.snrcjt.cn/gtggwauaco.html

std::ofstream out("a.txt");  out << "hi\n";
来源：http://hz.nanxuanxn.top/gtlzllufpf.html

[S50] C++：格式化数字
来源：http://hz.svipenyu.cn/gtpvnxjsuz.html

std::ostringstream os;  os << std::fixed << std::setprecision(2) << 3.14159;
来源：http://hz.tian-w.cn/gtkrknsgsq.html

[S51] C++：显式类型转换
来源：http://hz.ppjwa.cn/gtrodrpntv.html

static_cast<double>(a) / b
来源：http://hz.daria6918.cn/gtflargkvq.html

[S52] C++：const 与 noexcept
来源：http://hz.yvedp.cn/gtrlajuduj.html

int size() const noexcept { return n_; }
来源：http://hz.cdnleiting.top/gtbpfcdcnc.html

[S53] C++：移动语义
来源：http://hz.chenlongwang.top/gtrrmatnfe.html

std::vector<int> w = std::move(v);
来源：http://hz.cucudq.cn/gtqqfkucwl.html

[S54] C++：异常处理
来源：http://hz.c1oappe.top/gtztexxrcx.html

try { throw std::runtime_error("x"); } catch (const std::exception &e) { }
来源：http://hz.c1oappe.top/gtooghayho.html

[S55] C++：结构化绑定
来源：http://hz.feifeiyinyue.top/gtwqebilst.html

auto [a, b] = std::make_pair(1, 2);
来源：http://hz.ywan-chungtsiang.top/gtxdsilipq.html

[S56] C++：optional
来源：http://hz.hongshengwenyu.top/gtvqtsbyyu.html

std::optional<int> o = 5;  if (o) { int v = *o; }
来源：http://hz.jqgfzy.top/gtxwirjwuv.html

[S57] C++：编译期常量
来源：http://hz.nanxuanxn.top/gtquxvnzhk.html

constexpr int N = 10;
来源：http://hz.cucudq.cn/gtqdwgeabu.html

[S58] C++：命名空间
来源：http://hz.ywan-chungtsiang.top/gtyjyxakkw.html

namespace ns { int f() { return 1; } }
来源：http://hz.zhijiandao.cn/gtrgjkkclj.html

[S59] C++：静态断言
来源：http://hz.gotoacloud.top/gtejidiemn.html

static_assert(sizeof(int) == 4, "int 必须 4 字节");
来源：http://hz.sufxvd.cn/gtmqlpvavx.html

[S60] C++：遍历并删除元素
来源：http://hz.sufxvd.cn/gtvheuwaru.html

v.erase(std::remove_if(v.begin(), v.end(), [](int x) { return x < 0; }), v.end());
来源：http://hz.jinqigfzy.top/gtrewyorrp.html

================================================================================
来源：http://hz.xuetiantiany.cn/gtkxaorlzq.html

T. 其他语言补充（Kotlin / Swift / Lua / Perl / Scala）
来源：http://hz.daxiang520.top/gtakzlsiay.html

================================================================================
来源：http://hz.ydzc1.top/gtnkakbhqb.html

[T01] Kotlin：Hello World
来源：http://hz.xuanzx.com/gtyzpopfiv.html

println("Hello")
来源：http://hz.wangshuangyany.cn/gtlljqftdc.html

[T02] Kotlin：变量
来源：http://hz.zhijiandao.cn/gtmodpggxl.html

val a = 1;  var b = 2        // val 只读，var 可变
来源：http://hz.zhaomingkeji.xyz/gtnbeewlzk.html

[T03] Kotlin：字符串模板
来源：http://hz.hongshengwenyu.top/gtoyuobmpj.html

"值: $b"
来源：http://hz.0kj1m.cn/gtuwrimzic.html

[T04] Kotlin：空安全
来源：http://hz.hysaishi.cn/gtvezuuefl.html

val n: String? = null;  n?.length
来源：http://hz.nwbrower.top/gtiqjsylgs.html

[T05] Kotlin：when 表达式
来源：http://hz.meibo888.top/gtagpjhpql.html

val s = when (x) { 1 -> "一" else -> "其他" }   // 多分支时每个分支单独一行
来源：http://hz.daxiang520.top/gtgymoehlo.html

[T06] Kotlin：集合映射
来源：http://hz.yj20258888.top/gtjhjzurie.html

listOf(1, 2, 3).map { it * 2 }
来源：http://hz.zhiwuduotai.top/gtjkkkevfn.html

[T07] Kotlin：集合过滤
来源：http://hz.chenlongwang.top/gtxgleddbe.html

listOf(1, 2, 3).filter { it > 1 }
来源：http://hz.iojbl.cn/gtyjcefaih.html

[T08] Kotlin：数据类
来源：http://hz.zhiwuduotai.top/gtrbityefl.html

data class User(val name: String, val age: Int)
来源：http://hz.jianghu66.top/gtjfbvvwbn.html

[T09] Kotlin：扩展函数
来源：http://hz.hywenlv.cn/gtdkjjqsvy.html

fun String.exclaim() = this + "!"
来源：http://hz.dashuyun.cn/gtroszpden.html

[T10] Kotlin：默认参数
来源：http://hz.bjfxy.top/gtrcnwobbt.html

fun greet(name: String = "World") = "Hi $name"
来源：http://hz.meibo888.top/gtnawooghv.html

[T11] Kotlin：协程
来源：http://hz.ppjwa.cn/gtxvbyvuem.html

GlobalScope.launch { delay(1000); println("done") }
来源：http://hz.sufxvd.cn/gthcwuxcqq.html

[T12] Kotlin：解构声明
来源：http://hz.dianchejie.cn/gthaaisyjs.html

val (a, b) = Pair(1, 2)
来源：http://hz.haohaochexian.top/gtrwjywhhc.html

[T13] Kotlin：只读 Map
来源：http://hz.fzhhl.top/gtuolabmie.html

val m = mapOf("a" to 1)
来源：http://hz.kuanghao11.cn/gtbvnlaolz.html

[T14] Kotlin：循环
来源：http://hz.sweek.top/gtrslngqyp.html

for (i in 1..10) println(i)
来源：http://hz.daxiang520.top/gtxehxziqt.html

[T15] Kotlin：接口
来源：http://hz.havefunace.top/gtuwnaefyo.html

interface Shape { fun area(): Double }
来源：http://hz.yj20258.top/gtsjvuigmd.html

[T16] Swift：Hello World
来源：http://hz.zhongyouzk.top/gtpjlkwkhx.html

print("Hello")
来源：http://hz.zhongyouzk.top/gtkbpxlgvp.html

[T17] Swift：变量与常量
来源：http://hz.hammf.cn/gtezoczbvn.html

var a = 1;  let b = 2
来源：http://hz.ydjk.org.cn/gtdsaurdid.html

[T18] Swift：字符串插值
来源：http://hz.yj20258.top/gtlyzdhrth.html

"值: \(b)"
来源：http://hz.jqgufenzy.top/gtledzkqtn.html

[T19] Swift：可选绑定
来源：http://hz.zhongyouzk.top/gtjbfxuhwf.html

if let n = opt { print(n) }
来源：http://hz.aizwys.cn/gtillhxtlt.html

[T20] Swift：数组操作
来源：http://hz.yj20258888.top/gtusjjodtp.html

var a = [1, 2, 3];  a.append(4)
来源：http://hz.svipenyu.cn/gtatafocph.html

[T21] Swift：遍历
来源：http://hz.xuanzx.com/gtmqqciyxb.html

for x in a { print(x) }
来源：http://hz.shanyushiyangtech.top/gtlhywmyam.html

[T22] Swift：字典
来源：http://hz.yj202588.top/gtsofdtppq.html

var d = ["a": 1];  d["b"] = 2
来源：http://hz.ppjwa.cn/gtcrbmommg.html

[T23] Swift：函数
来源：http://hz.yangfankeji.com/gtqtcgdfwd.html

func add(_ a: Int, _ b: Int) -> Int { a + b }
来源：http://hz.shangyingyoupin.top/gtgbnfjtgr.html

[T24] Swift：闭包
来源：http://hz.c1oappe.top/gtajtjtasc.html

let f = { (x: Int) -> Int in x * 2 }
来源：http://hz.chenjidiqi.icu/gtlzmmpefr.html

[T25] Swift：结构体
来源：http://hz.hammf.cn/gtqifxlelr.html

struct P { var x: Int }
来源：http://hz.hnqzz.top/gtnlnrevqh.html

[T26] Swift：类与重写
来源：http://hz.xziqi.cn/gtbgalntjr.html

class A: Base { override func f() {} }
来源：http://hz.jianghu66.top/gtnwgcdupb.html

[T27] Swift：错误处理
来源：http://hz.zhaomingkeji.xyz/gtihwdhkft.html

do { try f() } catch { print(error) }
来源：http://hz.hongshengwenyu.top/gtujxysvac.html

[T28] Swift：枚举
来源：http://hz.shanyushiyangkeji.top/gtzgzoyflh.html

enum Color { case red, green }
来源：http://hz.dashuyun.cn/gtdfuccsci.html

[T29] Swift：guard 提前返回
来源：http://hz.pengpengdd.cyou/gtlwpmjrpc.html

guard let x = opt else { return }
来源：http://hz.cashguo.top/gtfadikhcp.html

[T30] Swift：协议
来源：http://hz.yonumen.top/gtfyjvwmyz.html

protocol Shape { func area() -> Double }
来源：http://hz.c1oappe.top/gtfedqrdyk.html

[T31] Lua：Hello World
来源：http://hz.iojbl.cn/gttexlzbmo.html

print("Hello")
来源：http://hz.ybcxt.top/gtzcmtkcfq.html

[T32] Lua：局部变量
来源：http://hz.xuetiantiany.cn/gtyhhevrbg.html

local a = 1
来源：http://hz.dianchejie.cn/gtgzjcacon.html

[T33] Lua：表（数组）
来源：http://hz.vqdsnc.cn/gtmwqdmthb.html

local t = {1, 2, 3};  t[4] = 4
来源：http://hz.yj202588.top/gtyzlggpmn.html

[T34] Lua：遍历表
来源：http://hz.pycfn.com/gtwpcbgddl.html

for i, v in ipairs(t) do print(i, v) end
来源：http://hz.sysykeji.top/gtqxqumhsk.html

[T35] Lua：字典表
来源：http://hz.cqqwz.cn/gtlredfzxc.html

local d = { a = 1 };  d.b = 2
来源：http://hz.yuanzhike.top/gtlvnyoeqr.html

[T36] Lua：函数
来源：http://hz.yangfankeji.com/gtdannjpza.html

function add(a, b) return a + b end
来源：http://hz.0kj1m.cn/gtujdlcvez.html

[T37] Lua：字符串拼接
来源：http://hz.mhx1999.top/gtldacfkbq.html

"a" .. "b"
来源：http://hz.zhijiandao.cn/gtqhlygbgs.html

[T38] Lua：条件
来源：http://hz.zhongyouzk.top/gtnnaxzkjm.html

if x > 0 then print("正") end
来源：http://hz.fengsongda.top/gtsdkfdctm.html

[T39] Lua：模式匹配
来源：http://hz.dashuyun.cn/gtwxkvhith.html

string.find(s, "%d+")
来源：http://hz.gogol.net.cn/gtsrefzzdc.html

[T40] Lua：元表
来源：http://hz.jqgfzy.top/gtstoednhm.html

setmetatable({}, { __index = base })
来源：http://hz.yonumen.top/gtzhztykge.html

[T41] Perl：Hello World
来源：http://hz.yj20258888.top/gtavlklkzm.html

print "Hello\n";
来源：http://hz.aibaodan.cn/gtstkmbwot.html

[T42] Perl：变量类型
来源：http://hz.jiagoushi.top/gtcirsjmxs.html

my $a = 1;  my @arr = (1, 2, 3);  my %h = (a => 1);
来源：http://hz.fengsongda.top/gtwrhiticr.html

[T43] Perl：字符串插值
来源：http://hz.birdmap.top/gtbnubzmge.html

"值: $a"
来源：http://hz.quarkkingdee.top/gtzntckcun.html

[T44] Perl：条件
来源：http://hz.hnqzz.top/gtfdioupmp.html

if ($a > 0) { print "正"; }
来源：http://hz.kuanghao11.cn/gtnazebgoq.html

[T45] Perl：数组遍历
来源：http://hz.daxiang520.top/gtiegnynzj.html

for my $x (@arr) { print $x; }
来源：http://hz.hfpthk.cn/gtxnteeqko.html

[T46] Perl：哈希操作
来源：http://hz.yuxming.cn/gtzyrlravw.html

$h{b} = 2;  for my $k (keys %h) { print "$k=$h{$k}"; }
来源：http://hz.ivvv.top/gtihksvurm.html

[T47] Perl：正则捕获
来源：http://hz.daxiang520.top/gtisulbyks.html

if ($s =~ /(\d+)/) { print $1; }
来源：http://hz.wangshuangyany.cn/gtpcuoqgie.html

[T48] Perl：正则替换
来源：http://hz.cucudq.cn/gtqwjbdhsh.html

$s =~ s/old/new/g;
来源：http://hz.svipenyu.cn/gtvcxmgipf.html

[T49] Perl：函数
来源：http://hz.jyoumei.cn/gtgimzckyc.html

sub add { my ($a, $b) = @_; return $a + $b; }
来源：http://hz.jlsjyb.cn/gtvoenrvng.html

[T50] Perl：逐行读文件
来源：http://hz.0kj1m.cn/gtygdzoiwj.html

open my $fh, "<", "a.txt" or die $!;
来源：http://hz.vqdsnc.cn/gtfqopmwjb.html

while (my $line = <$fh>) { print $line; }
来源：http://hz.9152youxi.cn/gtcyrkplvb.html

[T51] Scala：Hello World
来源：http://hz.jyoumei.cn/gtftlxjvil.html

println("Hello")
来源：http://hz.mhx1999.top/gtvjyznkpl.html

[T52] Scala：变量
来源：http://hz.redwolf501.top/gtijotqcun.html

val a = 1;  var b = 2
来源：http://hz.jqgufenzy.top/gtzsxaesmx.html

[T53] Scala：字符串插值
来源：http://hz.hongshengwenyu.top/gtjzpolrhb.html

s"值: $b"
来源：http://hz.52xcode.cn/gtpmjujmus.html

[T54] Scala：集合映射
来源：http://hz.jinghuilouyu.cn/gtkubtkson.html

List(1, 2, 3).map(_ * 2)
来源：http://hz.zycfv.cn/gtsujmbver.html

[T55] Scala：集合过滤
来源：http://hz.zycfv.cn/gtfkegybxw.html

List(1, 2, 3).filter(_ > 1)
来源：http://hz.jyoumei.cn/gtoqrahomz.html

[T56] Scala：样例类
来源：http://hz.chenjidiqi.icu/gtfrgkmnou.html

case class User(name: String, age: Int)
来源：http://hz.hongshengwenyu.top/gtrttpkpdc.html

[T57] Scala：模式匹配
来源：http://hz.hysaishi.cn/gtuutowyiv.html

x match { case 1 => "一"; case _ => "其他" }
来源：http://hz.ivvv.top/gthzimmpxy.html

[T58] Scala：函数定义
来源：http://hz.hammf.cn/gtyytnfdfv.html

def add(a: Int, b: Int): Int = a + b
来源：http://hz.cucudq.cn/gttphlgymv.html

[T59] Scala：循环
来源：http://hz.yonumen.top/gtjigvqfhx.html

for (i <- 1 to 10) println(i)
来源：http://hz.xziqi.cn/gtxjiqjmpo.html

[T60] Scala：折叠
来源：http://hz.shanyushiyangtech.top/gtizefnjox.html

List(1, 2, 3).foldLeft(0)(_ + _)
来源：http://hz.xuetiantiany.cn/gtdjqvabhz.html

================================================================================
来源：http://hz.shanyushiyangtech.top/gtzambluxz.html

U. 高频实用片段（Python / PHP / JavaScript 各 40 条）
来源：http://hz.guannengcc.top/gtjlvlcftb.html

================================================================================
来源：http://hz.guannengcc.top/gtekbcuskh.html

[U01] Py：创建虚拟环境
来源：http://hz.sysykeji.top/gtyrkwkspg.html

python -m venv .venv && source .venv/bin/activate
来源：http://hz.cheryme.top/gtrzbvlkij.html

[U02] Py：导出 / 安装依赖
来源：http://hz.shanyushiyangkeji.top/gtlhxrzcie.html

pip freeze > requirements.txt;  pip install -r requirements.txt
来源：http://hz.shanyushiyangkeji.top/gtcxbumqda.html

[U03] Py：加载 .env 配置
来源：http://hz.sysykeji.top/gtyvwksxvi.html

from dotenv import load_dotenv; load_dotenv()
来源：http://hz.yj202588.top/gtakmbtcox.html

[U04] Py：变量调试打印
来源：http://hz.zhiwuduotai.top/gticnaxspf.html

print(f"{x=}")            # 输出 x=值，Python 3.8+
来源：http://hz.chenlongwang.top/gtklcqwqwb.html

[U05] Py：列表去重且保序
来源：http://hz.hammf.cn/gtrzdmvgya.html

list(dict.fromkeys(arr))
来源：http://hz.havefunace.top/gtqhxtraay.html

[U06] Py：合并两个字典
来源：http://hz.pycfn.com/gtemkeocqk.html

{**a, **b}
来源：http://hz.52xcode.cn/gtuiereumb.html

[U07] Py：反转字典键值
来源：http://hz.chenlongwang.top/gtihpobxgt.html

{v: k for k, v in d.items()}
来源：http://hz.cqqwz.cn/gtwyvvuajb.html

[U08] Py：展平二维列表
来源：http://hz.yj20258888.top/gtjmpvhxvx.html

[y for x in nested for y in x]
来源：http://hz.c1oappe.top/gttxgogptw.html

[U09] Py：字典取最大值的键
来源：http://hz.daxiang520.top/gtwrkbiiuj.html

max(d, key=d.get)
来源：http://hz.aizwys.cn/gtbsvsbtta.html

[U10] Py：按值排序字典
来源：http://hz.gotoacloud.top/gtlopmkcbr.html

dict(sorted(d.items(), key=lambda kv: kv[1]))
来源：http://hz.dianchejie.cn/gttkqghgnx.html

[U11] Py：生成器表达式
来源：http://hz.yongpay.top/gtjgdhghjl.html

(x * 2 for x in arr)
来源：http://hz.pycfn.com/gtpzcgkgzb.html

[U12] Py：取出现最多的 3 个元素
来源：http://hz.guowangkeji.top/gtmgdptune.html

Counter(arr).most_common(3)
来源：http://hz.hnqzz.top/gttzxskgnh.html

[U13] Py：固定长度队列
来源：http://hz.ehwqpu.com/gtqwjvbkmh.html

deque(maxlen=10)
来源：http://hz.hysaishi.cn/gtdekyjgwi.html

[U14] Py：分组收集到列表
来源：http://hz.cucudq.cn/gtvvofnxrh.html

defaultdict(list)
来源：http://hz.yj202588.top/gthwgyzouh.html

[U15] Py：高精度计时
来源：http://hz.quarkkingdee.top/gtiaqevvzr.html

t = time.perf_counter()
来源：http://hz.nanxuanxn.top/gtcybrzdgu.html

[U16] Py：命令行参数解析
来源：http://hz.shanyushiyangtech.top/gtcrxnlofr.html

ap = argparse.ArgumentParser();  ap.add_argument("--name");  args = ap.parse_args()
来源：http://hz.hywenlv.cn/gtutobhonh.html

[U17] Py：初始化日志
来源：http://hz.xuanzx.com/gtvmphgpuj.html

logging.basicConfig(level=logging.INFO)
来源：http://hz.xylfe.cn/gtgapdmzdp.html

[U18] Py：预编译正则
来源：http://hz.jinqigfzy.top/gtykmhcmxv.html

pat = re.compile(r"\d+")
来源：http://hz.52xcode.cn/gtzuzymyry.html

[U19] Py：正则替换带回调
来源：http://hz.haohaochexian.top/gtuyrppdkj.html

re.sub(r"\d+", lambda m: str(int(m.group()) * 2), s)
来源：http://hz.c1oappe.top/gtbkchaogw.html

[U20] Py：缓存函数结果
来源：http://hz.jinghuilouyu.cn/gtxqladbwm.html

@functools.lru_cache(maxsize=None)
来源：http://hz.jianghu66.top/gtabraywvt.html

[U21] Py：自定义上下文管理器
来源：http://hz.zhengqikj.top/gtkteyxflx.html

@contextlib.contextmanager
来源：http://hz.hfpthk.cn/gtuqycskzu.html

[U22] Py：矩阵转置
来源：http://hz.sxryk.cn/gtxiptmvrp.html

list(zip(*m))
来源：http://hz.vqdsnc.cn/gtmhgpoysc.html

[U23] Py：分块读取大文件
来源：http://hz.jianghu66.top/gtyzyeookp.html

for chunk in iter(lambda: f.read(8192), b""):
来源：http://hz.0kj1m.cn/gthvpbamvz.html

[U24] Py：路径操作
来源：http://hz.jinqigfzy.top/gtxeobnukh.html

Path("a/b.txt").parent.mkdir(parents=True, exist_ok=True)
来源：http://hz.jinyuanbaomall.cn/gtdnamuclo.html

[U25] Py：CSV 按字典读
来源：http://hz.sweek.top/gtanrfdjhe.html

csv.DictReader(f)
来源：http://hz.ppjwa.cn/gtfbywyfeh.html

[U26] Py：并发下载
来源：http://hz.zhoulong.xyz/gtuchmutah.html

ThreadPoolExecutor(max_workers=8).map(fetch, urls)
来源：http://hz.316326.xyz/gtpsgvtlcg.html

[U27] Py：异步 HTTP
来源：http://hz.jiagoushi.top/gtwdmjznhr.html

aiohttp.ClientSession() 配合 async with
来源：http://hz.c1oappe.top/gtopvvbzhj.html

[U28] Py：类型别名
来源：http://hz.yvedp.cn/gtetswfrcl.html

UserId = int
来源：http://hz.ydzc1.top/gtcbzzwbar.html

[U29] Py：属性校验
来源：http://hz.sufxvd.cn/gtoczljfem.html

@property 与 @x.setter 配合
来源：http://hz.cashguo.top/gtnbmyctvp.html

[U30] Py：数据类
来源：http://hz.yonumen.top/gtygqdupxy.html

@dataclass(slots=True)
来源：http://hz.zhijiandao.cn/gteyswjslm.html

[U31] Py：单测
来源：http://hz.smart0.xyz/gthhbhlglt.html

python -m pytest -q
来源：http://hz.zhoulong.xyz/gttqdnhjkv.html

[U32] Py：代码格式化
来源：http://hz.9152youxi.cn/gthbxjwyez.html

ruff format . && ruff check --fix .
来源：http://hz.bjfxy.top/gtljuoqmag.html

[U33] Py：打包发布
来源：http://hz.cashguo.top/gttquwuwyn.html

python -m build  （依赖 pyproject.toml）
来源：http://hz.pengpengdd.cyou/gttgdratnc.html

[U34] Py：判断编码
来源：http://hz.daxiang520.top/gttwuhcyey.html

chardet.detect(raw)
来源：http://hz.yuxming.cn/gtazseniiq.html

[U35] Py：发送邮件
来源：http://hz.0kj1m.cn/gtxspeojke.html

smtplib.SMTP_SSL(...).send_message(msg)
来源：http://hz.shzxlz.cn/gtiezgzxzz.html

[U36] Py：定时任务
来源：http://hz.redwolf501.top/gthcxawlxh.html

schedule.every(10).minutes.do(job)
来源：http://hz.c1oappe.top/gtcbkgipyt.html

[U37] Py：读写 Excel
来源：http://hz.sufxvd.cn/gttwrgilhe.html

pandas.read_excel / DataFrame.to_excel
来源：http://hz.gogol.net.cn/gtubfhyqij.html

[U38] Py：获取脚本所在目录
来源：http://hz.jlsjyb.cn/gtqnchhsrb.html

Path(__file__).resolve().parent
来源：http://hz.gogol.net.cn/gtvqfoyczr.html

[U39] Py：判断是否在交互环境
来源：http://hz.hnxiangtu.top/gtrbzbbrlr.html

sys.stdout.isatty()
来源：http://hz.quarkkingdee.top/gtwqbmmyfb.html

[U40] Py：打印到标准错误
来源：http://hz.ehwqpu.com/gtpdjnbako.html

print("err", file=sys.stderr)
来源：http://hz.zycfv.cn/gtnbrmmhus.html

[U41] PHP：初始化 Composer 项目
来源：http://hz.chenlongwang.top/gtxnpulbxs.html

composer init;  composer require guzzlehttp/guzzle
来源：http://hz.jiagoushi.top/gtuwhmlkxg.html

[U42] PHP：PSR-4 自动加载
来源：http://hz.zhixingplan.top/gtlwdhwtwd.html

"autoload": { "psr-4": { "App\\": "src/" } }
来源：http://hz.aibaodan.cn/gtjihanhzy.html

[U43] PHP：声明命名空间
来源：http://hz.guannengcc.top/gtdbykwuzs.html

namespace App\Http;
来源：http://hz.hammf.cn/gtjduerrdf.html

[U44] PHP：开启严格类型
来源：http://hz.chenzaomai.com/gtyzsvjeme.html

declare(strict_types=1);
来源：http://hz.jinqigfzy.top/gtlurdrzzi.html

[U45] PHP：类型声明与返回类型
来源：http://hz.kuanghao11.cn/gtsdszmpcm.html

function add(int $a, int $b): int { return $a + $b; }
来源：http://hz.daria6918.cn/gtoidysucl.html

[U46] PHP：可空类型
来源：http://hz.xylfe.cn/gtvsllizxe.html

?string $name = null
来源：http://hz.meibo888.top/gtbbexgbkx.html

[U47] PHP：联合类型
来源：http://hz.zdqjudy.top/gtvxquxukt.html

int|string $id
来源：http://hz.pycfn.com/gtdjbrufvc.html

[U48] PHP：纯枚举
来源：http://hz.shuidangran.top/gtejsbmrgr.html

enum Status: string { case Active = "active"; case Off = "off"; }
来源：http://hz.316326.xyz/gtiwjilcly.html

[U49] PHP：只读属性
来源：http://hz.yvedp.cn/gthtlxogiv.html

public readonly string $name
来源：http://hz.zycfv.cn/gtqaimxbhz.html

[U50] PHP：构造器属性提升
来源：http://hz.birdmap.top/gtdrdotgoo.html

public function __construct(private int $id) {}
来源：http://hz.9152youxi.cn/gtgoptlydz.html

[U51] PHP：数组解构
来源：http://hz.shangyingyoupin.top/gtpfheduyn.html

[$a, $b] = $arr;
来源：http://hz.zhaomingkeji.xyz/gtdkvnaxyb.html

[U52] PHP：箭头函数
来源：http://hz.meibo888.top/gtskcgeqct.html

$double = fn($x) => $x * 2;
来源：http://hz.iojbl.cn/gtdiqgkzvn.html

[U53] PHP：空合并运算符
来源：http://hz.c1oappe.top/gtowiatgfq.html

$v = $a ?? $b ?? "default";
来源：http://hz.jyoumei.cn/gtuzsxjhwj.html

[U54] PHP：空安全调用
来源：http://hz.daxiang520.top/gthuqpkhtv.html

$obj?->method()
来源：http://hz.yuxming.cn/gtnvffoelc.html

[U55] PHP：match 表达式
来源：http://hz.shanyushiyangtech.top/gtmfxyqqlo.html

$s = match($x) { 1 => "一", default => "其他" };
来源：http://hz.jlsjyb.cn/gtztlajozi.html

[U56] PHP：命名参数
来源：http://hz.guowangkeji.top/gtkloaxhxb.html

f(a: 1, b: 2)
来源：http://hz.pengpengdd.cyou/gthrgnyntq.html

[U57] PHP：字符串插值
来源：http://hz.ydjk.org.cn/gtolztfuha.html

"值: {$a}"
来源：http://hz.shzxlz.cn/gturvqqvfr.html

[U58] PHP：数组三件套
来源：http://hz.feifeiyinyue.top/gtamrzuvik.html

array_map($f, $a);  array_filter($a, $f);  array_reduce($a, $f, 0);
来源：http://hz.mhx1999.top/gtyskssdlo.html


<!-- 参考信息 -->