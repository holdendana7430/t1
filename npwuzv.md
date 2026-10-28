代发 wailian999

[S37] C++：set
来源：http://hz.fzhhl.top/gtzsecjbnp.html

std::set<int> s{1, 2, 3};  s.insert(4);
来源：http://hz.cheryme.top/gtainlcqjj.html

[S38] C++：排序
来源：http://hz.chenlongwang.top/gtfoqshfan.html

std::sort(v.begin(), v.end());
来源：http://hz.snrcjt.cn/gtthhldzss.html

[S39] C++：自定义比较器排序
来源：http://hz.yuxming.cn/gtanvsrwyp.html

std::sort(v.begin(), v.end(), [](int a, int b) { return a > b; });
来源：http://hz.jinqigufen.top/gtbtuifyww.html

[S40] C++：查找元素
来源：http://hz.hnxiangtu.top/gtbrrndcrr.html

auto it = std::find(v.begin(), v.end(), 3);
来源：http://hz.hongshengwenyu.top/gtjvmrhufm.html

[S41] C++：类与构造函数
来源：http://hz.chenjidiqi.icu/gttuharrfz.html

class A { public: A(int v) : x_(v) {} int get() const { return x_; } private: int x_; };
来源：http://hz.xinyue.icu/gtlaadrzvn.html

[S42] C++：继承与虚函数
来源：http://hz.zdqjudy.top/gtsprsiygz.html

class B : public Base { public: void f() override {} };
来源：http://hz.hnxiangtu.top/gtliqyicin.html

[S43] C++：智能指针
来源：http://hz.316326.xyz/gttyedhwvm.html

auto p = std::make_unique<int>(5);
来源：http://hz.shzxlz.cn/gtxykstccd.html

[S44] C++：引用传参
来源：http://hz.bjfxy.top/gtdnfqkbhb.html

void inc(int &x) { ++x; }
来源：http://hz.ydjk.org.cn/gtxmbvadkp.html

[S45] C++：lambda
来源：http://hz.jianghu66.top/gtbrbacjif.html

auto add = [](int a, int b) { return a + b; };
来源：http://hz.ydjk.org.cn/gtjnwwqiss.html

[S46] C++：函数模板
来源：http://hz.smart0.xyz/gtplovqmwl.html

template <typename T> T maxv(T a, T b) { return a > b ? a : b; }
来源：http://hz.jianghu66.top/gtomodmlzo.html

[S47] C++：结构化绑定遍历
来源：http://hz.zhongyouzk.top/gtlcdjphua.html

for (const auto &[k, v] : m) { std::cout << k << v; }
来源：http://hz.pycfn.com/gtktexcgyp.html

[S48] C++：逐行读文件
来源：http://hz.ywan-chungtsiang.top/gtangkrvus.html

std::ifstream in("a.txt");  std::string line;
来源：http://hz.xuanzx.com/gtbmvmsxix.html

while (std::getline(in, line)) { }
来源：http://hz.smart0.xyz/gtrlayxqzk.html

[S49] C++：写文件
来源：http://hz.zhijiandao.cn/gtxpxujkao.html

std::ofstream out("a.txt");  out << "hi\n";
来源：http://hz.zhijiandao.cn/gtqkikcvuf.html

[S50] C++：格式化数字
来源：http://hz.zhengqikj.top/gtowonjbap.html

std::ostringstream os;  os << std::fixed << std::setprecision(2) << 3.14159;
来源：http://hz.zhoulong.xyz/gtlaehfqwc.html

[S51] C++：显式类型转换
来源：http://hz.quarkkingdee.top/gtbbmemxdj.html

static_cast<double>(a) / b
来源：http://hz.zhiwuduotai.top/gttndpoinm.html

[S52] C++：const 与 noexcept
来源：http://hz.cdnleiting.top/gtvxgbccou.html

int size() const noexcept { return n_; }
来源：http://hz.hnxiangtu.top/gtcjooaehj.html

[S53] C++：移动语义
来源：http://hz.nanxinkj.top/gtamfayiea.html

std::vector<int> w = std::move(v);
来源：http://hz.zhiwuduotai.top/gtwjqaxbpw.html

[S54] C++：异常处理
来源：http://hz.chenzaomai.com/gtqrlqdhtk.html

try { throw std::runtime_error("x"); } catch (const std::exception &e) { }
来源：http://hz.shanyushiyangkeji.top/gtgdeoaayq.html

[S55] C++：结构化绑定
来源：http://hz.zycfv.cn/gthqlkaiod.html

auto [a, b] = std::make_pair(1, 2);
来源：http://hz.ydjk.org.cn/gtsqktcfjz.html

[S56] C++：optional
来源：http://hz.quarkkingdee.top/gtsktuybem.html

std::optional<int> o = 5;  if (o) { int v = *o; }
来源：http://hz.tanke756.top/gtikraojet.html

[S57] C++：编译期常量
来源：http://hz.gotoacloud.top/gtmolkpdrd.html

constexpr int N = 10;
来源：http://hz.chenlongwang.top/gtxvsqgmmj.html

[S58] C++：命名空间
来源：http://hz.shuidangran.top/gtnijsvbbu.html

namespace ns { int f() { return 1; } }
来源：http://hz.quarkkingdee.top/gtzmgjpuii.html

[S59] C++：静态断言
来源：http://hz.ybcxt.top/gtnuafodzv.html

static_assert(sizeof(int) == 4, "int 必须 4 字节");
来源：http://hz.hywenlv.cn/gtglvsqnnx.html

[S60] C++：遍历并删除元素
来源：http://hz.xziqi.cn/gtrunxudph.html

v.erase(std::remove_if(v.begin(), v.end(), [](int x) { return x < 0; }), v.end());
来源：http://hz.cucudq.cn/gtivfmrmvf.html

================================================================================
来源：http://hz.yj20258.top/gtotmvsxxz.html

T. 其他语言补充（Kotlin / Swift / Lua / Perl / Scala）
来源：http://hz.jiagoushi.top/gtuaeibvfq.html

================================================================================
来源：http://hz.yonumen.top/gtoqhroikb.html

[T01] Kotlin：Hello World
来源：http://hz.cucudq.cn/gttttsjijo.html

println("Hello")
来源：http://hz.cqqwz.cn/gtldsdopqg.html

[T02] Kotlin：变量
来源：http://hz.zhaomingkeji.xyz/gtzcjedfqo.html

val a = 1;  var b = 2        // val 只读，var 可变
来源：http://hz.nwbrower.top/gtwfrqattr.html

[T03] Kotlin：字符串模板
来源：http://hz.smart0.xyz/gtnpmjrusd.html

"值: $b"
来源：http://hz.gaohongyu789.top/gtqbaiziuk.html

[T04] Kotlin：空安全
来源：http://hz.jlsjyb.cn/gtpyinejfr.html

val n: String? = null;  n?.length
来源：http://hz.nanxinkj.top/gtaocsehnh.html

[T05] Kotlin：when 表达式
来源：http://hz.pengpengdd.cyou/gticdbenhw.html

val s = when (x) { 1 -> "一" else -> "其他" }   // 多分支时每个分支单独一行
来源：http://hz.yangfankeji.com/gtogzffwyi.html

[T06] Kotlin：集合映射
来源：http://hz.hnqzz.top/gtauifhjgd.html

listOf(1, 2, 3).map { it * 2 }
来源：http://hz.yj20258888.top/gtaprewbxg.html

[T07] Kotlin：集合过滤
来源：http://hz.jinqigufen.top/gtzupzqwqo.html

listOf(1, 2, 3).filter { it > 1 }
来源：http://hz.xylfe.cn/gtsdbpijsm.html

[T08] Kotlin：数据类
来源：http://hz.tianlin.xyz/gttqaabizl.html

data class User(val name: String, val age: Int)
来源：http://hz.dianchejie.cn/gtjqmsxfdq.html

[T09] Kotlin：扩展函数
来源：http://hz.cheryme.top/gtxaafaxlu.html

fun String.exclaim() = this + "!"
来源：http://hz.yvedp.cn/gtrmwftgcc.html

[T10] Kotlin：默认参数
来源：http://hz.zhixingplan.top/gtoumdaicu.html

fun greet(name: String = "World") = "Hi $name"
来源：http://hz.jiagoushi.top/gtcocepijb.html

[T11] Kotlin：协程
来源：http://hz.fzhhl.top/gtvmthohzz.html

GlobalScope.launch { delay(1000); println("done") }
来源：http://hz.jiagoushi.top/gtcecvyloh.html

[T12] Kotlin：解构声明
来源：http://hz.bjfxy.top/gtplfnqdzc.html

val (a, b) = Pair(1, 2)
来源：http://hz.yvedp.cn/gtiwbcywyl.html

[T13] Kotlin：只读 Map
来源：http://hz.ybcxt.top/gtkgbfljwd.html

val m = mapOf("a" to 1)
来源：http://hz.zhiwuduotai.top/gtjndvkexv.html

[T14] Kotlin：循环
来源：http://hz.yongpay.top/gtqhhegzhm.html

for (i in 1..10) println(i)
来源：http://hz.yonumen.top/gtbhzxsaph.html

[T15] Kotlin：接口
来源：http://hz.wangshuangyany.cn/gtwwjhjafs.html

interface Shape { fun area(): Double }
来源：http://hz.snrcjt.cn/gtsbeyapev.html

[T16] Swift：Hello World
来源：http://hz.yj20258888.top/gtfcepbohy.html

print("Hello")
来源：http://hz.cdnleiting.top/gtoczynlfv.html

[T17] Swift：变量与常量
来源：http://hz.hnxiangtu.top/gtfbrprqio.html

var a = 1;  let b = 2
来源：http://hz.quarkkingdee.top/gtgrzfhryx.html

[T18] Swift：字符串插值
来源：http://hz.yj20258.top/gtruoixcth.html

"值: \(b)"
来源：http://hz.jyoumei.cn/gtuwptopvs.html

[T19] Swift：可选绑定
来源：http://hz.daria6918.cn/gttudxuoto.html

if let n = opt { print(n) }
来源：http://hz.xuanzx.com/gtrpspcame.html

[T20] Swift：数组操作
来源：http://hz.cheryme.top/gtlujzqzng.html

var a = [1, 2, 3];  a.append(4)
来源：http://hz.hnqzz.top/gtshtgxwfa.html

[T21] Swift：遍历
来源：http://hz.hnxiangtu.top/gtqalgroki.html

for x in a { print(x) }
来源：http://hz.ywan-chungtsiang.top/gtelenmfca.html

[T22] Swift：字典
来源：http://hz.sufxvd.cn/gtxrcpbtvn.html

var d = ["a": 1];  d["b"] = 2
来源：http://hz.zycfv.cn/gtpoennbur.html

[T23] Swift：函数
来源：http://hz.kuanghao11.cn/gtkfdbdebk.html

func add(_ a: Int, _ b: Int) -> Int { a + b }
来源：http://hz.jlsjyb.cn/gtrljacaaw.html

[T24] Swift：闭包
来源：http://hz.hywenlv.cn/gtvxdhevzq.html

let f = { (x: Int) -> Int in x * 2 }
来源：http://hz.zhiwuduotai.top/gttoccgnxk.html

[T25] Swift：结构体
来源：http://hz.hammf.cn/gtvbhssqtv.html

struct P { var x: Int }
来源：http://hz.yuxming.cn/gtzkzxwhoh.html

[T26] Swift：类与重写
来源：http://hz.jyoumei.cn/gtklzqvftn.html

class A: Base { override func f() {} }
来源：http://hz.jiagoushi.top/gtubfcprhe.html

[T27] Swift：错误处理
来源：http://hz.jyoumei.cn/gtnkofdiuy.html

do { try f() } catch { print(error) }
来源：http://hz.0kj1m.cn/gtxjwdprnq.html

[T28] Swift：枚举
来源：http://hz.xinyue.icu/gtrobezlld.html

enum Color { case red, green }
来源：http://hz.yueranfly.top/gtmgqmtqvo.html

[T29] Swift：guard 提前返回
来源：http://hz.dianchejie.cn/gtjpyljkas.html

guard let x = opt else { return }
来源：http://hz.shangyingyoupin.top/gtsohgzdry.html

[T30] Swift：协议
来源：http://hz.svipenyu.cn/gtqnbsiftm.html

protocol Shape { func area() -> Double }
来源：http://hz.xylfe.cn/gtiyjsbawe.html

[T31] Lua：Hello World
来源：http://hz.jianghu66.top/gtmaavauwm.html

print("Hello")
来源：http://hz.jyoumei.cn/gtwqzgiwrm.html

[T32] Lua：局部变量
来源：http://hz.haohaochexian.top/gtanccudlk.html

local a = 1
来源：http://hz.mhx1999.top/gtfkdvwdoa.html

[T33] Lua：表（数组）
来源：http://hz.zhongyouzk.top/gtqoshwgrd.html

local t = {1, 2, 3};  t[4] = 4
来源：http://hz.yvedp.cn/gtdifaaevl.html

[T34] Lua：遍历表
来源：http://hz.hnxiangtu.top/gtykurycpy.html

for i, v in ipairs(t) do print(i, v) end
来源：http://hz.tanke756.top/gtvriqyouv.html

[T35] Lua：字典表
来源：http://hz.shzxlz.cn/gtoqnhwcxo.html

local d = { a = 1 };  d.b = 2
来源：http://hz.zhaomingkeji.xyz/gttqunegcq.html

[T36] Lua：函数
来源：http://hz.ydzc1.top/gtclcknshk.html

function add(a, b) return a + b end
来源：http://hz.dianchejie.cn/gtkxrygnyo.html

[T37] Lua：字符串拼接
来源：http://hz.xylfe.cn/gttdsowmjs.html

"a" .. "b"
来源：http://hz.jinyuanbaomall.cn/gtziwpjjyd.html

[T38] Lua：条件
来源：http://hz.yanxiufei.cn/gtcpcdmruz.html

if x > 0 then print("正") end
来源：http://hz.fzhhl.top/gtcitgeyum.html

[T39] Lua：模式匹配
来源：http://hz.zhoulong.xyz/gtzjvtnefc.html

string.find(s, "%d+")
来源：http://hz.yuxming.cn/gtkryydkqt.html

[T40] Lua：元表
来源：http://hz.jyoumei.cn/gthugbasds.html

setmetatable({}, { __index = base })
来源：http://hz.tanke756.top/gtcxoyukff.html

[T41] Perl：Hello World
来源：http://hz.yueranfly.top/gtlskltpdj.html

print "Hello\n";
来源：http://hz.chenjidiqi.icu/gtikeyypmr.html

[T42] Perl：变量类型
来源：http://hz.pycfn.com/gtvsyaahzx.html

my $a = 1;  my @arr = (1, 2, 3);  my %h = (a => 1);
来源：http://hz.guowangkeji.top/gtmkxlyopj.html

[T43] Perl：字符串插值
来源：http://hz.ydzc1.top/gtrlycfsez.html

"值: $a"
来源：http://hz.smart0.xyz/gtmtwdtebv.html

[T44] Perl：条件
来源：http://hz.yj202588.top/gtfsbbbuvp.html

if ($a > 0) { print "正"; }
来源：http://hz.xylfe.cn/gtnudwpahs.html

[T45] Perl：数组遍历
来源：http://hz.shanyushiyangkeji.top/gtdvqbtwmw.html

for my $x (@arr) { print $x; }
来源：http://hz.xylfe.cn/gtcjvbpycn.html

[T46] Perl：哈希操作
来源：http://hz.havefunace.top/gtruyyiqwl.html

$h{b} = 2;  for my $k (keys %h) { print "$k=$h{$k}"; }
来源：http://hz.tanke756.top/gtxqhvulco.html

[T47] Perl：正则捕获
来源：http://hz.wangdashe.top/gtamtxkvtb.html

if ($s =~ /(\d+)/) { print $1; }
来源：http://hz.feifeiyinyue.top/gtwkdjmedp.html

[T48] Perl：正则替换
来源：http://hz.daria6918.cn/gtgxzlevbf.html

$s =~ s/old/new/g;
来源：http://hz.nanxinkj.top/gtekdysgof.html

[T49] Perl：函数
来源：http://hz.jqgfzy.top/gttvsipodn.html

sub add { my ($a, $b) = @_; return $a + $b; }
来源：http://hz.jinghuilouyu.cn/gtguswsfod.html

[T50] Perl：逐行读文件
来源：http://hz.yuxming.cn/gtuigokppw.html

open my $fh, "<", "a.txt" or die $!;
来源：http://hz.gotoacloud.top/gtfsiwlwmt.html

while (my $line = <$fh>) { print $line; }
来源：http://hz.haohaochexian.top/gtbccbqxxe.html

[T51] Scala：Hello World
来源：http://hz.ywan-chungtsiang.top/gtnvsinild.html

println("Hello")
来源：http://hz.svipenyu.cn/gtfdsjuzur.html

[T52] Scala：变量
来源：http://hz.zhiwuduotai.top/gtefpxghkg.html

val a = 1;  var b = 2
来源：http://hz.nwbrower.top/gtkhmmhsja.html

[T53] Scala：字符串插值
来源：http://hz.pycfn.com/gtepsbtmcv.html

s"值: $b"
来源：http://hz.yuxming.cn/gtbumwwvpu.html

[T54] Scala：集合映射
来源：http://hz.meibo888.top/gtwulsqzni.html

List(1, 2, 3).map(_ * 2)
来源：http://hz.chenzaomai.com/gtqcgmrhut.html

[T55] Scala：集合过滤
来源：http://hz.zhengqikj.top/gteyrnpjxy.html

List(1, 2, 3).filter(_ > 1)
来源：http://hz.jinyuanbaomall.cn/gtrmpecfqi.html

[T56] Scala：样例类
来源：http://hz.guannengcc.top/gtojwxxrkl.html

case class User(name: String, age: Int)
来源：http://hz.jianghu66.top/gtnkqeixrt.html

[T57] Scala：模式匹配
来源：http://hz.c1oappe.top/gtvxyaskkw.html

x match { case 1 => "一"; case _ => "其他" }
来源：http://hz.tian-w.cn/gtkwuonjgu.html

[T58] Scala：函数定义
来源：http://hz.sysykeji.top/gtsxtidtkq.html

def add(a: Int, b: Int): Int = a + b
来源：http://hz.snrcjt.cn/gtxrkpcoao.html

[T59] Scala：循环
来源：http://hz.zhoulong.xyz/gtpcfcgkmg.html

for (i <- 1 to 10) println(i)
来源：http://hz.jinghuilouyu.cn/gtjivpjual.html

[T60] Scala：折叠
来源：http://hz.yuanzhike.top/gtqtduaazc.html

List(1, 2, 3).foldLeft(0)(_ + _)
来源：http://hz.0kj1m.cn/gtefmkfupj.html

================================================================================
来源：http://hz.shuidangran.top/gtpewbkiwo.html

U. 高频实用片段（Python / PHP / JavaScript 各 40 条）
来源：http://hz.316326.xyz/gtefsjiwqa.html

================================================================================
来源：http://hz.yonumen.top/gtqsdbyqeb.html

[U01] Py：创建虚拟环境
来源：http://hz.shanyushiyangtech.top/gtzwtxqiav.html

python -m venv .venv && source .venv/bin/activate
来源：http://hz.daria6918.cn/gtlkoearjl.html

[U02] Py：导出 / 安装依赖
来源：http://hz.smart0.xyz/gtvgbuqhqd.html

pip freeze > requirements.txt;  pip install -r requirements.txt
来源：http://hz.quarkkingdee.top/gtaauisqfb.html

[U03] Py：加载 .env 配置
来源：http://hz.9152youxi.cn/gtxgmpizxu.html

from dotenv import load_dotenv; load_dotenv()
来源：http://hz.zdqjudy.top/gtugqalazl.html

[U04] Py：变量调试打印
来源：http://hz.fzhhl.top/gtsgeglbnu.html

print(f"{x=}")            # 输出 x=值，Python 3.8+
来源：http://hz.cdnleiting.top/gtlzzblucj.html

[U05] Py：列表去重且保序
来源：http://hz.zhoulong.xyz/gtwcxgjoxl.html

list(dict.fromkeys(arr))
来源：http://hz.zhaomingkeji.xyz/gtdsfbryhm.html

[U06] Py：合并两个字典
来源：http://hz.dianchejie.cn/gttxmfjyyc.html

{**a, **b}
来源：http://hz.jqgufenzy.top/gtdfjzgunu.html

[U07] Py：反转字典键值
来源：http://hz.tianlin.xyz/gtuiwkuooq.html

{v: k for k, v in d.items()}
来源：http://hz.xziqi.cn/gtwwfqmwfz.html

[U08] Py：展平二维列表
来源：http://hz.zhoulong.xyz/gtxmpdsrqz.html

[y for x in nested for y in x]
来源：http://hz.yuxming.cn/gtorsmqrny.html

[U09] Py：字典取最大值的键
来源：http://hz.haohaochexian.top/gtoxyvilyd.html

max(d, key=d.get)
来源：http://hz.pengpengdd.cyou/gtbotjihql.html

[U10] Py：按值排序字典
来源：http://hz.redwolf501.top/gtxjltonbp.html

dict(sorted(d.items(), key=lambda kv: kv[1]))
来源：http://hz.yanxiufei.cn/gtqbhwawbm.html

[U11] Py：生成器表达式
来源：http://hz.c1oappe.top/gtulhjktoo.html

(x * 2 for x in arr)
来源：http://hz.pycfn.com/gtgfanixon.html

[U12] Py：取出现最多的 3 个元素
来源：http://hz.nwbrower.top/gtugjpmnde.html

Counter(arr).most_common(3)
来源：http://hz.yuanzhike.top/gtmhtisvyo.html

[U13] Py：固定长度队列
来源：http://hz.shanyushiyangkeji.top/gthkjmphaa.html

deque(maxlen=10)
来源：http://hz.xingfuxueyuan.xyz/gtbcytskks.html

[U14] Py：分组收集到列表
来源：http://hz.bjfxy.top/gtlvcuefbt.html

defaultdict(list)
来源：http://hz.yanxiufei.cn/gtwlnrmbrc.html

[U15] Py：高精度计时
来源：http://hz.ivvv.top/gtzjwmjxhd.html

t = time.perf_counter()
来源：http://hz.redwolf501.top/gtkorniutq.html

[U16] Py：命令行参数解析
来源：http://hz.daxiang520.top/gtooedzgkw.html

ap = argparse.ArgumentParser();  ap.add_argument("--name");  args = ap.parse_args()
来源：http://hz.redwolf501.top/gtlqpobapa.html

[U17] Py：初始化日志
来源：http://hz.bjfxy.top/gtefjaxrfz.html

logging.basicConfig(level=logging.INFO)
来源：http://hz.yj20258888.top/gtjxwvygkp.html

[U18] Py：预编译正则
来源：http://hz.nwbrower.top/gtikeloena.html

pat = re.compile(r"\d+")
来源：http://hz.hongshengwenyu.top/gttjlswlmg.html

[U19] Py：正则替换带回调
来源：http://hz.gogol.net.cn/gteyruvsqe.html

re.sub(r"\d+", lambda m: str(int(m.group()) * 2), s)
来源：http://hz.chenlongwang.top/gtoriscded.html

[U20] Py：缓存函数结果
来源：http://hz.chenjidiqi.icu/gtecqvvtif.html

@functools.lru_cache(maxsize=None)
来源：http://hz.hammf.cn/gtmwdkwnhf.html

[U21] Py：自定义上下文管理器
来源：http://hz.hywenlv.cn/gtojmazqga.html

@contextlib.contextmanager
来源：http://hz.ehwqpu.com/gtluwfwzbz.html

[U22] Py：矩阵转置
来源：http://hz.gotoacloud.top/gtrrvdgjot.html

list(zip(*m))
来源：http://hz.hongshengwenyu.top/gthkwymqkg.html

[U23] Py：分块读取大文件
来源：http://hz.jiagoushi.top/gtxuhfgwsy.html

for chunk in iter(lambda: f.read(8192), b""):
来源：http://hz.andypj.xyz/gtmxmibacz.html

[U24] Py：路径操作
来源：http://hz.xingfuxueyuan.xyz/gtvdstvhhj.html

Path("a/b.txt").parent.mkdir(parents=True, exist_ok=True)
来源：http://hz.hnqzz.top/gtejnorqog.html

[U25] Py：CSV 按字典读
来源：http://hz.hywenlv.cn/gtuhmmladb.html

csv.DictReader(f)
来源：http://hz.hammf.cn/gthejtycjl.html

[U26] Py：并发下载
来源：http://hz.yueranfly.top/gtkqtedkxj.html

ThreadPoolExecutor(max_workers=8).map(fetch, urls)
来源：http://hz.ybcxt.top/gtpmqbfiro.html

[U27] Py：异步 HTTP
来源：http://hz.cucudq.cn/gtcgsqpfbg.html

aiohttp.ClientSession() 配合 async with
来源：http://hz.tianlin.xyz/gtaylunydl.html

[U28] Py：类型别名
来源：http://hz.jqgfzy.top/gtezavdtyw.html

UserId = int
来源：http://hz.chenjidiqi.icu/gtnoidqwap.html

[U29] Py：属性校验
来源：http://hz.guannengcc.top/gtljpijuyf.html

@property 与 @x.setter 配合
来源：http://hz.yvedp.cn/gtbyssbolf.html

[U30] Py：数据类
来源：http://hz.hongshengwenyu.top/gtpsckgjgv.html

@dataclass(slots=True)
来源：http://hz.gaohongyu789.top/gthrzghuqq.html

[U31] Py：单测
来源：http://hz.chenjidiqi.icu/gtwqmbdihz.html

python -m pytest -q
来源：http://hz.haohaochexian.top/gtanpctvdz.html

[U32] Py：代码格式化
来源：http://hz.fzhhl.top/gtwmkmpang.html

ruff format . && ruff check --fix .
来源：http://hz.jianghu66.top/gtesudlpct.html

[U33] Py：打包发布
来源：http://hz.guannengcc.top/gtsdsgkyvh.html

python -m build  （依赖 pyproject.toml）
来源：http://hz.daria6918.cn/gtpvrciwdi.html

[U34] Py：判断编码
来源：http://hz.jinqigufen.top/gtibfcahsq.html

chardet.detect(raw)
来源：http://hz.andypj.xyz/gtxoyuklpo.html

[U35] Py：发送邮件
来源：http://hz.jiagoushi.top/gtkfuyicxr.html

smtplib.SMTP_SSL(...).send_message(msg)
来源：http://hz.vqdsnc.cn/gtbeahwjke.html

[U36] Py：定时任务
来源：http://hz.aibaodan.cn/gtqkgdemjq.html

schedule.every(10).minutes.do(job)
来源：http://hz.hongshengwenyu.top/gtwylznrth.html

[U37] Py：读写 Excel
来源：http://hz.yangfankeji.com/gtnugscyzb.html

pandas.read_excel / DataFrame.to_excel
来源：http://hz.yvedp.cn/gtyympndgt.html

[U38] Py：获取脚本所在目录
来源：http://hz.jyoumei.cn/gtxcdusbuc.html

Path(__file__).resolve().parent
来源：http://hz.nanxinkj.top/gtrhjwdgpf.html

[U39] Py：判断是否在交互环境
来源：http://hz.hammf.cn/gtfbobzask.html

sys.stdout.isatty()
来源：http://hz.havefunace.top/gtyocveflk.html

[U40] Py：打印到标准错误
来源：http://hz.jinyuanbaomall.cn/gtuokgenad.html

print("err", file=sys.stderr)
来源：http://hz.zhoulong.xyz/gtqzbnjaxh.html

[U41] PHP：初始化 Composer 项目
来源：http://hz.tanke756.top/gtkiwzmtin.html

composer init;  composer require guzzlehttp/guzzle
来源：http://hz.jinyuanbaomall.cn/gtvoxsavge.html

[U42] PHP：PSR-4 自动加载
来源：http://hz.jiagoushi.top/gtkrhsfybz.html

"autoload": { "psr-4": { "App\\": "src/" } }
来源：http://hz.chenzaomai.com/gtcjuevbaf.html

[U43] PHP：声明命名空间
来源：http://hz.0kj1m.cn/gtmigknoiv.html

namespace App\Http;
来源：http://hz.cucudq.cn/gtpdjwcjvx.html

[U44] PHP：开启严格类型
来源：http://hz.gzhubu.top/gtvyazfnrj.html

declare(strict_types=1);
来源：http://hz.gzhubu.top/gtbxnvwpoi.html

[U45] PHP：类型声明与返回类型
来源：http://hz.zhoulong.xyz/gthetfhuiz.html

function add(int $a, int $b): int { return $a + $b; }
来源：http://hz.bjfxy.top/gtrcpegmee.html

[U46] PHP：可空类型
来源：http://hz.zhiwuduotai.top/gtckunzkel.html

?string $name = null
来源：http://hz.ydjk.org.cn/gtziyhtavs.html

[U47] PHP：联合类型
来源：http://hz.9152youxi.cn/gtbqezjfbx.html

int|string $id
来源：http://hz.meibo888.top/gtendjofra.html

[U48] PHP：纯枚举
来源：http://hz.316326.xyz/gtncsqwvdm.html

enum Status: string { case Active = "active"; case Off = "off"; }
来源：http://hz.sufxvd.cn/gtfxfvzdto.html

[U49] PHP：只读属性
来源：http://hz.iojbl.cn/gtriolslgw.html

public readonly string $name
来源：http://hz.dianchejie.cn/gtpdhvsjtu.html

[U50] PHP：构造器属性提升
来源：http://hz.dianchejie.cn/gtlayyiejj.html

public function __construct(private int $id) {}
来源：http://hz.yj20258888.top/gtrmbbqtls.html

[U51] PHP：数组解构
来源：http://hz.yj202588.top/gtrpgftewp.html

[$a, $b] = $arr;
来源：http://hz.sufxvd.cn/gtndxxjphe.html

[U52] PHP：箭头函数
来源：http://hz.pycfn.com/gtlzhygmmw.html

$double = fn($x) => $x * 2;
来源：http://hz.xuanzx.com/gtfpmrsgnd.html

[U53] PHP：空合并运算符
来源：http://hz.hammf.cn/gtvkrpxhcx.html

$v = $a ?? $b ?? "default";
来源：http://hz.chenzaomai.com/gtsqzgltgx.html

[U54] PHP：空安全调用
来源：http://hz.nwbrower.top/gtpoihenef.html

$obj?->method()
来源：http://hz.tanke756.top/gtdavlzpkv.html

[U55] PHP：match 表达式
来源：http://hz.zhixingplan.top/gtztkndkxw.html

$s = match($x) { 1 => "一", default => "其他" };
来源：http://hz.52xcode.cn/gtvyfnxcym.html

[U56] PHP：命名参数
来源：http://hz.gaohongyu789.top/gtmhvcmmcp.html

f(a: 1, b: 2)
来源：http://hz.cdnleiting.top/gtnfwxomju.html

[U57] PHP：字符串插值
来源：http://hz.shuidangran.top/gtnnfqnhlp.html

"值: {$a}"
来源：http://hz.havefunace.top/gtibhokfjj.html

[U58] PHP：数组三件套
来源：http://hz.gzhubu.top/gtqtqhlvei.html

array_map($f, $a);  array_filter($a, $f);  array_reduce($a, $f, 0);
来源：http://hz.shuidangran.top/gteclxzisu.html

[U59] PHP：自定义排序
来源：http://hz.cheryme.top/gtolhmvcsp.html

usort($arr, fn($a, $b) => $a["age"] <=> $b["age"]);
来源：http://hz.fzhhl.top/gtlgoykxqj.html

[U60] PHP：JSON 编解码
来源：http://hz.zhixingplan.top/gtxvnhucxg.html

json_encode($d, JSON_UNESCAPED_UNICODE);  json_decode($s, true);
来源：http://hz.fengsongda.top/gtzetoljwa.html

[U61] PHP：正则
来源：http://hz.nanxuanxn.top/gtijnmygcm.html

preg_match('/(\d+)/', $s, $m);  preg_replace('/\d+/', '#', $s);
来源：http://hz.hammf.cn/gtfdmblvlw.html

[U62] PHP：日期对象
来源：http://hz.cucudq.cn/gtkahdnbct.html

(new DateTimeImmutable())->format("Y-m-d");
来源：http://hz.guannengcc.top/gtgfxjtokv.html


<!-- 参考信息 -->