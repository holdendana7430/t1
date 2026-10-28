代发 wailian999

[S41] C++：类与构造函数
来源：http://hz.yuxming.cn/gtdzhvbgll.html

class A { public: A(int v) : x_(v) {} int get() const { return x_; } private: int x_; };
来源：http://hz.nwbrower.top/gtjygrakar.html

[S42] C++：继承与虚函数
来源：http://hz.redwolf501.top/gtcljxwqql.html

class B : public Base { public: void f() override {} };
来源：http://hz.nanxinkj.top/gtvihnlmbc.html

[S43] C++：智能指针
来源：http://hz.hongshengwenyu.top/gtbefxmapv.html

auto p = std::make_unique<int>(5);
来源：http://hz.daxiang520.top/gtzorktaxq.html

[S44] C++：引用传参
来源：http://hz.cdnleiting.top/gtprhgyzhb.html

void inc(int &x) { ++x; }
来源：http://hz.jlsjyb.cn/gtdaqoztst.html

[S45] C++：lambda
来源：http://hz.cashguo.top/gtyauefrfi.html

auto add = [](int a, int b) { return a + b; };
来源：http://hz.hysaishi.cn/gtmtfxnvfi.html

[S46] C++：函数模板
来源：http://hz.nanxinkj.top/gtsbycxyav.html

template <typename T> T maxv(T a, T b) { return a > b ? a : b; }
来源：http://hz.xinyue.icu/gttrpurfaq.html

[S47] C++：结构化绑定遍历
来源：http://hz.xuanzx.com/gtsxsmopax.html

for (const auto &[k, v] : m) { std::cout << k << v; }
来源：http://hz.nanxinkj.top/gtpecozdzc.html

[S48] C++：逐行读文件
来源：http://hz.52xcode.cn/gtzliptvoz.html

std::ifstream in("a.txt");  std::string line;
来源：http://hz.xuanzx.com/gtbjcwnhqg.html

while (std::getline(in, line)) { }
来源：http://hz.tian-w.cn/gtnytmvuod.html

[S49] C++：写文件
来源：http://hz.cheryme.top/gtpioagkxt.html

std::ofstream out("a.txt");  out << "hi\n";
来源：http://hz.jlsjyb.cn/gtalzujsok.html

[S50] C++：格式化数字
来源：http://hz.gogol.net.cn/gtvbpakuhs.html

std::ostringstream os;  os << std::fixed << std::setprecision(2) << 3.14159;
来源：http://hz.fzhhl.top/gtxmwgnkvi.html

[S51] C++：显式类型转换
来源：http://hz.sysykeji.top/gtenrvkoyk.html

static_cast<double>(a) / b
来源：http://hz.cqqwz.cn/gtooinwzmu.html

[S52] C++：const 与 noexcept
来源：http://hz.birdmap.top/gtrnwxwlvs.html

int size() const noexcept { return n_; }
来源：http://hz.c1oappe.top/gtxkkuarxe.html

[S53] C++：移动语义
来源：http://hz.jinghuilouyu.cn/gttzvetivb.html

std::vector<int> w = std::move(v);
来源：http://hz.zhongyouzk.top/gtdebvrygp.html

[S54] C++：异常处理
来源：http://hz.iojbl.cn/gtmspznlty.html

try { throw std::runtime_error("x"); } catch (const std::exception &e) { }
来源：http://hz.iojbl.cn/gthtuqkyfh.html

[S55] C++：结构化绑定
来源：http://hz.yongpay.top/gtmjihucqb.html

auto [a, b] = std::make_pair(1, 2);
来源：http://hz.gotoacloud.top/gtdwcdrorq.html

[S56] C++：optional
来源：http://hz.birdmap.top/gtwrwmmwqe.html

std::optional<int> o = 5;  if (o) { int v = *o; }
来源：http://hz.smart0.xyz/gtjgpmbqhw.html

[S57] C++：编译期常量
来源：http://hz.shangyingyoupin.top/gtfnrnuuof.html

constexpr int N = 10;
来源：http://hz.sysykeji.top/gtkcqocmzt.html

[S58] C++：命名空间
来源：http://hz.316326.xyz/gttbgrfdqb.html

namespace ns { int f() { return 1; } }
来源：http://hz.zhixingplan.top/gtdoyqefky.html

[S59] C++：静态断言
来源：http://hz.yj20258.top/gtoxnsgvwo.html

static_assert(sizeof(int) == 4, "int 必须 4 字节");
来源：http://hz.shuidangran.top/gttehgnvjw.html

[S60] C++：遍历并删除元素
来源：http://hz.vqdsnc.cn/gtubeqkwlq.html

v.erase(std::remove_if(v.begin(), v.end(), [](int x) { return x < 0; }), v.end());
来源：http://hz.feifeiyinyue.top/gtppcxniak.html

================================================================================
来源：http://hz.chenlongwang.top/gtdvlflrdj.html

T. 其他语言补充（Kotlin / Swift / Lua / Perl / Scala）
来源：http://hz.redwolf501.top/gtdlmslofd.html

================================================================================
来源：http://hz.xziqi.cn/gtopymvdlz.html

[T01] Kotlin：Hello World
来源：http://hz.birdmap.top/gtqxmhvhwo.html

println("Hello")
来源：http://hz.aibaodan.cn/gtdkqpvonj.html

[T02] Kotlin：变量
来源：http://hz.svipenyu.cn/gtzlkmivgo.html

val a = 1;  var b = 2        // val 只读，var 可变
来源：http://hz.sufxvd.cn/gtblofbmsd.html

[T03] Kotlin：字符串模板
来源：http://hz.shanyushiyangkeji.top/gtlgmnxsyk.html

"值: $b"
来源：http://hz.0kj1m.cn/gtcdoijtef.html

[T04] Kotlin：空安全
来源：http://hz.cqqwz.cn/gtactdbycw.html

val n: String? = null;  n?.length
来源：http://hz.redwolf501.top/gtjihijhqw.html

[T05] Kotlin：when 表达式
来源：http://hz.jinqigufen.top/gtpbvmdutl.html

val s = when (x) { 1 -> "一" else -> "其他" }   // 多分支时每个分支单独一行
来源：http://hz.pycfn.com/gtnsvgbult.html

[T06] Kotlin：集合映射
来源：http://hz.smart0.xyz/gtpxcwldwj.html

listOf(1, 2, 3).map { it * 2 }
来源：http://hz.nanxinkj.top/gtltdnyeli.html

[T07] Kotlin：集合过滤
来源：http://hz.chenlongwang.top/gtayxterve.html

listOf(1, 2, 3).filter { it > 1 }
来源：http://hz.ydjk.org.cn/gtzjtnyrqj.html

[T08] Kotlin：数据类
来源：http://hz.birdmap.top/gtqrxniced.html

data class User(val name: String, val age: Int)
来源：http://hz.0kj1m.cn/gtkirkxuuy.html

[T09] Kotlin：扩展函数
来源：http://hz.ppjwa.cn/gtjxxszqhs.html

fun String.exclaim() = this + "!"
来源：http://hz.snrcjt.cn/gtfnfdbbwu.html

[T10] Kotlin：默认参数
来源：http://hz.feifeiyinyue.top/gtyjegjnyg.html

fun greet(name: String = "World") = "Hi $name"
来源：http://hz.ehwqpu.com/gtqshkzzne.html

[T11] Kotlin：协程
来源：http://hz.iojbl.cn/gtxpmqzqnb.html

GlobalScope.launch { delay(1000); println("done") }
来源：http://hz.xinyue.icu/gthgbvhtmd.html

[T12] Kotlin：解构声明
来源：http://hz.yvedp.cn/gtefxchhxm.html

val (a, b) = Pair(1, 2)
来源：http://hz.hammf.cn/gtyqlsnlnv.html

[T13] Kotlin：只读 Map
来源：http://hz.hfpthk.cn/gtfkkxkedt.html

val m = mapOf("a" to 1)
来源：http://hz.jinghuilouyu.cn/gtflkobssq.html

[T14] Kotlin：循环
来源：http://hz.daria6918.cn/gtyafdamvh.html

for (i in 1..10) println(i)
来源：http://hz.cdnleiting.top/gtsoahycnn.html

[T15] Kotlin：接口
来源：http://hz.zhengqikj.top/gtewigdhkw.html

interface Shape { fun area(): Double }
来源：http://hz.jinqigufen.top/gttpgvubaw.html

[T16] Swift：Hello World
来源：http://hz.cucudq.cn/gtxomwkuhw.html

print("Hello")
来源：http://hz.shanyushiyangtech.top/gtdqyxkxob.html

[T17] Swift：变量与常量
来源：http://hz.xingfuxueyuan.xyz/gtttqridth.html

var a = 1;  let b = 2
来源：http://hz.ydzc1.top/gtntafzyys.html

[T18] Swift：字符串插值
来源：http://hz.tianlin.xyz/gtxepuuuqd.html

"值: \(b)"
来源：http://hz.tian-w.cn/gtappuuahe.html

[T19] Swift：可选绑定
来源：http://hz.shanyushiyangkeji.top/gtqawhaqbh.html

if let n = opt { print(n) }
来源：http://hz.tianlin.xyz/gtcoaxsbsj.html

[T20] Swift：数组操作
来源：http://hz.svipenyu.cn/gtpoyxkutq.html

var a = [1, 2, 3];  a.append(4)
来源：http://hz.chenzaomai.com/gtyctwecir.html

[T21] Swift：遍历
来源：http://hz.zycfv.cn/gtbxzlswpi.html

for x in a { print(x) }
来源：http://hz.zhoulong.xyz/gtoyecfvoo.html

[T22] Swift：字典
来源：http://hz.snrcjt.cn/gtxhscqusc.html

var d = ["a": 1];  d["b"] = 2
来源：http://hz.iojbl.cn/gtijmrbmzo.html

[T23] Swift：函数
来源：http://hz.jinghuilouyu.cn/gtafajgjrj.html

func add(_ a: Int, _ b: Int) -> Int { a + b }
来源：http://hz.9152youxi.cn/gtrgjslzse.html

[T24] Swift：闭包
来源：http://hz.zhoulong.xyz/gtiwsiuase.html

let f = { (x: Int) -> Int in x * 2 }
来源：http://hz.zycfv.cn/gtdkhitwsj.html

[T25] Swift：结构体
来源：http://hz.ybcxt.top/gtuacvqhld.html

struct P { var x: Int }
来源：http://hz.gotoacloud.top/gtvqxhltfy.html

[T26] Swift：类与重写
来源：http://hz.jyoumei.cn/gtubfhficu.html

class A: Base { override func f() {} }
来源：http://hz.birdmap.top/gtxkbcltmw.html

[T27] Swift：错误处理
来源：http://hz.cheryme.top/gtxfpppbou.html

do { try f() } catch { print(error) }
来源：http://hz.xinyue.icu/gtxulfwedc.html

[T28] Swift：枚举
来源：http://hz.daria6918.cn/gtudvvcnyp.html

enum Color { case red, green }
来源：http://hz.zycfv.cn/gtrmnpuuvv.html

[T29] Swift：guard 提前返回
来源：http://hz.ppjwa.cn/gtaevcitvh.html

guard let x = opt else { return }
来源：http://hz.hnqzz.top/gtqpoqxtlo.html

[T30] Swift：协议
来源：http://hz.c1oappe.top/gtpiigvknn.html

protocol Shape { func area() -> Double }
来源：http://hz.redwolf501.top/gtmlscjvsm.html

[T31] Lua：Hello World
来源：http://hz.yongpay.top/gtlumwxwmx.html

print("Hello")
来源：http://hz.chenzaomai.com/gtlbvxvknh.html

[T32] Lua：局部变量
来源：http://hz.aizwys.cn/gtekgwiwje.html

local a = 1
来源：http://hz.hywenlv.cn/gtonhpdntm.html

[T33] Lua：表（数组）
来源：http://hz.nwbrower.top/gthgvrzgxb.html

local t = {1, 2, 3};  t[4] = 4
来源：http://hz.cucudq.cn/gteaodyspq.html

[T34] Lua：遍历表
来源：http://hz.tianlin.xyz/gtefztloaq.html

for i, v in ipairs(t) do print(i, v) end
来源：http://hz.zhaomingkeji.xyz/gtbnijinmk.html

[T35] Lua：字典表
来源：http://hz.pengpengdd.cyou/gtjaaicvko.html

local d = { a = 1 };  d.b = 2
来源：http://hz.wangshuangyany.cn/gtaxqwzhys.html

[T36] Lua：函数
来源：http://hz.ivvv.top/gtgflryhoe.html

function add(a, b) return a + b end
来源：http://hz.tian-w.cn/gtbnexbwox.html

[T37] Lua：字符串拼接
来源：http://hz.yongpay.top/gtgmowjyhn.html

"a" .. "b"
来源：http://hz.ybcxt.top/gtjbkpffql.html

[T38] Lua：条件
来源：http://hz.nanxinkj.top/gtzfkwpoau.html

if x > 0 then print("正") end
来源：http://hz.hammf.cn/gtkjkjgjgw.html

[T39] Lua：模式匹配
来源：http://hz.guannengcc.top/gtucmwcuuf.html

string.find(s, "%d+")
来源：http://hz.yuanzhike.top/gtjwryomqg.html

[T40] Lua：元表
来源：http://hz.sweek.top/gtkdrmsblr.html

setmetatable({}, { __index = base })
来源：http://hz.xylfe.cn/gtzesqjcis.html

[T41] Perl：Hello World
来源：http://hz.zdqjudy.top/gtrpjnubdx.html

print "Hello\n";
来源：http://hz.bjfxy.top/gtrpshryqz.html

[T42] Perl：变量类型
来源：http://hz.yongpay.top/gtwnwklulb.html

my $a = 1;  my @arr = (1, 2, 3);  my %h = (a => 1);
来源：http://hz.0kj1m.cn/gtvxwoixqc.html

[T43] Perl：字符串插值
来源：http://hz.meibo888.top/gtakdelmye.html

"值: $a"
来源：http://hz.yvedp.cn/gtpynzrciy.html

[T44] Perl：条件
来源：http://hz.wangshuangyany.cn/gtuqgorbys.html

if ($a > 0) { print "正"; }
来源：http://hz.jianghu66.top/gtepkgqnzb.html

[T45] Perl：数组遍历
来源：http://hz.fengsongda.top/gtrsgdevnd.html

for my $x (@arr) { print $x; }
来源：http://hz.tian-w.cn/gttyylcsng.html

[T46] Perl：哈希操作
来源：http://hz.iojbl.cn/gtbtguscyc.html

$h{b} = 2;  for my $k (keys %h) { print "$k=$h{$k}"; }
来源：http://hz.pycfn.com/gtcdfravbp.html

[T47] Perl：正则捕获
来源：http://hz.daria6918.cn/gtivbkrpvw.html

if ($s =~ /(\d+)/) { print $1; }
来源：http://hz.pycfn.com/gtqyzwmdjo.html

[T48] Perl：正则替换
来源：http://hz.guannengcc.top/gtezorahuw.html

$s =~ s/old/new/g;
来源：http://hz.zhengqikj.top/gtwyfsiiar.html

[T49] Perl：函数
来源：http://hz.guowangkeji.top/gttogvgkyu.html

sub add { my ($a, $b) = @_; return $a + $b; }
来源：http://hz.hnqzz.top/gtcmkwmxss.html

[T50] Perl：逐行读文件
来源：http://hz.xuetiantiany.cn/gtxhrgwekb.html

open my $fh, "<", "a.txt" or die $!;
来源：http://hz.yuxming.cn/gttnybpuet.html

while (my $line = <$fh>) { print $line; }
来源：http://hz.ppjwa.cn/gtfffxuzzy.html

[T51] Scala：Hello World
来源：http://hz.hfpthk.cn/gtlgkhomev.html

println("Hello")
来源：http://hz.ywan-chungtsiang.top/gtzntomfgb.html

[T52] Scala：变量
来源：http://hz.gaohongyu789.top/gtuixexehf.html

val a = 1;  var b = 2
来源：http://hz.yongpay.top/gtksnxkrxv.html

[T53] Scala：字符串插值
来源：http://hz.yuxming.cn/gtrckmmhna.html

s"值: $b"
来源：http://hz.c1oappe.top/gtugmytlto.html

[T54] Scala：集合映射
来源：http://hz.jinyuanbaomall.cn/gtljjeypte.html

List(1, 2, 3).map(_ * 2)
来源：http://hz.ydzc1.top/gtwhaeohvb.html

[T55] Scala：集合过滤
来源：http://hz.tanke756.top/gtkccsbizo.html

List(1, 2, 3).filter(_ > 1)
来源：http://hz.316326.xyz/gtiydjmnzw.html

[T56] Scala：样例类
来源：http://hz.ehwqpu.com/gtojkxoahj.html

case class User(name: String, age: Int)
来源：http://hz.yj20258888.top/gtfhunsqyb.html

[T57] Scala：模式匹配
来源：http://hz.xylfe.cn/gtdryifmed.html

x match { case 1 => "一"; case _ => "其他" }
来源：http://hz.bjfxy.top/gttkknchlu.html

[T58] Scala：函数定义
来源：http://hz.zhiwuduotai.top/gtiwtaedfz.html

def add(a: Int, b: Int): Int = a + b
来源：http://hz.guowangkeji.top/gtplinyyeu.html

[T59] Scala：循环
来源：http://hz.zhengqikj.top/gtzmsrjvhb.html

for (i <- 1 to 10) println(i)
来源：http://hz.mhx1999.top/gtymdwenir.html

[T60] Scala：折叠
来源：http://hz.xziqi.cn/gtmgoafkvd.html

List(1, 2, 3).foldLeft(0)(_ + _)
来源：http://hz.vqdsnc.cn/gtuxhltqpv.html

================================================================================
来源：http://hz.cashguo.top/gtfbaufuaq.html

U. 高频实用片段（Python / PHP / JavaScript 各 40 条）
来源：http://hz.ivvv.top/gtvrxqkgfr.html

================================================================================
来源：http://hz.jyoumei.cn/gtnbcxidet.html

[U01] Py：创建虚拟环境
来源：http://hz.tianlin.xyz/gtbicjmvut.html

python -m venv .venv && source .venv/bin/activate
来源：http://hz.cashguo.top/gtmzhmlhdg.html

[U02] Py：导出 / 安装依赖
来源：http://hz.yueranfly.top/gtajsnxlrn.html

pip freeze > requirements.txt;  pip install -r requirements.txt
来源：http://hz.redwolf501.top/gtuuxgleeq.html

[U03] Py：加载 .env 配置
来源：http://hz.fzhhl.top/gtznbeedxw.html

from dotenv import load_dotenv; load_dotenv()
来源：http://hz.yuxming.cn/gtmdnlahgz.html

[U04] Py：变量调试打印
来源：http://hz.jinqigufen.top/gtuszwtxoz.html

print(f"{x=}")            # 输出 x=值，Python 3.8+
来源：http://hz.daria6918.cn/gthnyglvge.html

[U05] Py：列表去重且保序
来源：http://hz.zhongyouzk.top/gtwcjkofqp.html

list(dict.fromkeys(arr))
来源：http://hz.yongpay.top/gtvlhpnmww.html

[U06] Py：合并两个字典
来源：http://hz.yj20258888.top/gtumprajef.html

{**a, **b}
来源：http://hz.cashguo.top/gtibokjxcv.html

[U07] Py：反转字典键值
来源：http://hz.hammf.cn/gtjytnwncj.html

{v: k for k, v in d.items()}
来源：http://hz.jqgfzy.top/gteaivzdwx.html

[U08] Py：展平二维列表
来源：http://hz.pycfn.com/gtnpyeswgu.html

[y for x in nested for y in x]
来源：http://hz.chenlongwang.top/gtaozdbauh.html

[U09] Py：字典取最大值的键
来源：http://hz.smart0.xyz/gtladfgcuf.html

max(d, key=d.get)
来源：http://hz.fengsongda.top/gtscnmcjco.html

[U10] Py：按值排序字典
来源：http://hz.hysaishi.cn/gtnsuakhrm.html

dict(sorted(d.items(), key=lambda kv: kv[1]))
来源：http://hz.tianlin.xyz/gtdarmblra.html

[U11] Py：生成器表达式
来源：http://hz.sweek.top/gtadckaree.html

(x * 2 for x in arr)
来源：http://hz.yj20258.top/gtzcmqnvjk.html

[U12] Py：取出现最多的 3 个元素
来源：http://hz.yj202588.top/gtdkrdsrlu.html

Counter(arr).most_common(3)
来源：http://hz.mhx1999.top/gtakrzcpnv.html

[U13] Py：固定长度队列
来源：http://hz.jinqigufen.top/gtrqcchzxj.html

deque(maxlen=10)
来源：http://hz.shangyingyoupin.top/gtlbecuvym.html

[U14] Py：分组收集到列表
来源：http://hz.ivvv.top/gtxjytmgbh.html

defaultdict(list)
来源：http://hz.c1oappe.top/gtyvglrxmp.html

[U15] Py：高精度计时
来源：http://hz.chenzaomai.com/gtoxdjybbw.html

t = time.perf_counter()
来源：http://hz.tianlin.xyz/gtyztufqma.html

[U16] Py：命令行参数解析
来源：http://hz.dianchejie.cn/gtpngqxrkn.html

ap = argparse.ArgumentParser();  ap.add_argument("--name");  args = ap.parse_args()
来源：http://hz.ehwqpu.com/gtwhuycrgu.html

[U17] Py：初始化日志
来源：http://hz.zhaomingkeji.xyz/gtyfyshhlq.html

logging.basicConfig(level=logging.INFO)
来源：http://hz.xingfuxueyuan.xyz/gtihlqvebf.html

[U18] Py：预编译正则
来源：http://hz.zdqjudy.top/gtmviovyia.html

pat = re.compile(r"\d+")
来源：http://hz.zhixingplan.top/gtujvwqaur.html

[U19] Py：正则替换带回调
来源：http://hz.ydjk.org.cn/gtpejxyqkt.html

re.sub(r"\d+", lambda m: str(int(m.group()) * 2), s)
来源：http://hz.jyoumei.cn/gtsqwlhmvy.html

[U20] Py：缓存函数结果
来源：http://hz.jianghu66.top/gtzpinusia.html

@functools.lru_cache(maxsize=None)
来源：http://hz.shanyushiyangtech.top/gtaernsdau.html

[U21] Py：自定义上下文管理器
来源：http://hz.shanyushiyangtech.top/gtnjgedkba.html

@contextlib.contextmanager
来源：http://hz.shzxlz.cn/gtuopohddn.html

[U22] Py：矩阵转置
来源：http://hz.yuxming.cn/gtawzfnguv.html

list(zip(*m))
来源：http://hz.9152youxi.cn/gtsbgdicje.html

[U23] Py：分块读取大文件
来源：http://hz.havefunace.top/gtmvlwyamk.html

for chunk in iter(lambda: f.read(8192), b""):
来源：http://hz.dashuyun.cn/gtdyvbsupx.html

[U24] Py：路径操作
来源：http://hz.guannengcc.top/gtdxvyhgeq.html

Path("a/b.txt").parent.mkdir(parents=True, exist_ok=True)
来源：http://hz.0kj1m.cn/gtlypbesbf.html

[U25] Py：CSV 按字典读
来源：http://hz.birdmap.top/gtweqnxpua.html

csv.DictReader(f)
来源：http://hz.zhengqikj.top/gtbouyfttm.html

[U26] Py：并发下载
来源：http://hz.dashuyun.cn/gtfzddvmam.html

ThreadPoolExecutor(max_workers=8).map(fetch, urls)
来源：http://hz.bjfxy.top/gtahfpsvuo.html

[U27] Py：异步 HTTP
来源：http://hz.chenzaomai.com/gtkgdpsraz.html

aiohttp.ClientSession() 配合 async with
来源：http://hz.jqgfzy.top/gtrvqhorqa.html

[U28] Py：类型别名
来源：http://hz.jianghu66.top/gtgzkholge.html

UserId = int
来源：http://hz.zhongyouzk.top/gttlqsxdji.html

[U29] Py：属性校验
来源：http://hz.zhixingplan.top/gtcujtoftf.html

@property 与 @x.setter 配合
来源：http://hz.daria6918.cn/gtxmzhumuy.html

[U30] Py：数据类
来源：http://hz.yanxiufei.cn/gtkbvufobg.html

@dataclass(slots=True)
来源：http://hz.jlsjyb.cn/gtmmrcibvv.html

[U31] Py：单测
来源：http://hz.meibo888.top/gtbnkmnpdn.html

python -m pytest -q
来源：http://hz.guannengcc.top/gtzgqedkpu.html

[U32] Py：代码格式化
来源：http://hz.zhijiandao.cn/gtunjzmjwg.html

ruff format . && ruff check --fix .
来源：http://hz.gaohongyu789.top/gtynzkbjvi.html

[U33] Py：打包发布
来源：http://hz.cqqwz.cn/gtsncrpgah.html

python -m build  （依赖 pyproject.toml）
来源：http://hz.ybcxt.top/gtzakzijaw.html

[U34] Py：判断编码
来源：http://hz.jinghuilouyu.cn/gtvnbpwrko.html

chardet.detect(raw)
来源：http://hz.jianghu66.top/gtlmbnojoi.html

[U35] Py：发送邮件
来源：http://hz.jiagoushi.top/gtpdyheubt.html

smtplib.SMTP_SSL(...).send_message(msg)
来源：http://hz.cheryme.top/gtnkoqmbog.html

[U36] Py：定时任务
来源：http://hz.zdqjudy.top/gtkjvdbjgi.html

schedule.every(10).minutes.do(job)
来源：http://hz.jqgfzy.top/gtczpyuwsi.html

[U37] Py：读写 Excel
来源：http://hz.zhixingplan.top/gtjgntppzm.html

pandas.read_excel / DataFrame.to_excel
来源：http://hz.hammf.cn/gtwvjilloe.html

[U38] Py：获取脚本所在目录
来源：http://hz.shuidangran.top/gtfenhczgc.html

Path(__file__).resolve().parent
来源：http://hz.xuetiantiany.cn/gtgyshbwao.html

[U39] Py：判断是否在交互环境
来源：http://hz.cheryme.top/gtlnudbevi.html

sys.stdout.isatty()
来源：http://hz.cqqwz.cn/gtxfcbxxrf.html

[U40] Py：打印到标准错误
来源：http://hz.xingfuxueyuan.xyz/gtkhnbhehe.html

print("err", file=sys.stderr)
来源：http://hz.gogol.net.cn/gtqwnkrgcd.html

[U41] PHP：初始化 Composer 项目
来源：http://hz.jinqigfzy.top/gtyewwikww.html

composer init;  composer require guzzlehttp/guzzle
来源：http://hz.snrcjt.cn/gtczjyjmnb.html

[U42] PHP：PSR-4 自动加载
来源：http://hz.chenzaomai.com/gttglrfejz.html

"autoload": { "psr-4": { "App\\": "src/" } }
来源：http://hz.hfpthk.cn/gtwoedvesa.html

[U43] PHP：声明命名空间
来源：http://hz.ywan-chungtsiang.top/gtagkntouf.html

namespace App\Http;
来源：http://hz.cucudq.cn/gtxglmbrap.html

[U44] PHP：开启严格类型
来源：http://hz.9152youxi.cn/gtcjdyiyay.html

declare(strict_types=1);
来源：http://hz.9152youxi.cn/gtvjunqoot.html

[U45] PHP：类型声明与返回类型
来源：http://hz.kuanghao11.cn/gtmjgzteyl.html

function add(int $a, int $b): int { return $a + $b; }
来源：http://hz.cqqwz.cn/gtlhfdhtel.html

[U46] PHP：可空类型
来源：http://hz.yuxming.cn/gtptlawbmd.html

?string $name = null
来源：http://hz.gzhubu.top/gtcmzulajz.html

[U47] PHP：联合类型
来源：http://hz.xylfe.cn/gturvdbvgk.html

int|string $id
来源：http://hz.xuanzx.com/gtjzjnptrh.html

[U48] PHP：纯枚举
来源：http://hz.zhengqikj.top/gtzisyxxda.html

enum Status: string { case Active = "active"; case Off = "off"; }
来源：http://hz.xylfe.cn/gtaaazvjtv.html

[U49] PHP：只读属性
来源：http://hz.aizwys.cn/gtxpzbxwme.html

public readonly string $name
来源：http://hz.zhijiandao.cn/gtcfbuxlnf.html

[U50] PHP：构造器属性提升
来源：http://hz.zhaomingkeji.xyz/gttflhgwwf.html

public function __construct(private int $id) {}
来源：http://hz.ppjwa.cn/gttqyhowqx.html

[U51] PHP：数组解构
来源：http://hz.birdmap.top/gtpmitgptg.html

[$a, $b] = $arr;
来源：http://hz.xuetiantiany.cn/gtodgjvftd.html

[U52] PHP：箭头函数
来源：http://hz.hfpthk.cn/gtjouokcti.html

$double = fn($x) => $x * 2;
来源：http://hz.ydjk.org.cn/gtxvgiexer.html

[U53] PHP：空合并运算符
来源：http://hz.meibo888.top/gtzexqjvjd.html

$v = $a ?? $b ?? "default";
来源：http://hz.kuanghao11.cn/gtgkliesqw.html

[U54] PHP：空安全调用
来源：http://hz.cqqwz.cn/gtqhholvsq.html

$obj?->method()
来源：http://hz.gaohongyu789.top/gtiifqxuoo.html

[U55] PHP：match 表达式
来源：http://hz.gotoacloud.top/gttuwedrwh.html

$s = match($x) { 1 => "一", default => "其他" };
来源：http://hz.xuanzx.com/gtmallbjmm.html

[U56] PHP：命名参数
来源：http://hz.daria6918.cn/gtszvrsbiw.html

f(a: 1, b: 2)
来源：http://hz.jinyuanbaomall.cn/gthefsuvjt.html

[U57] PHP：字符串插值
来源：http://hz.cqqwz.cn/gtkwuryicn.html

"值: {$a}"
来源：http://hz.tanke756.top/gtslbrztut.html

[U58] PHP：数组三件套
来源：http://hz.smart0.xyz/gthvqsexfs.html

array_map($f, $a);  array_filter($a, $f);  array_reduce($a, $f, 0);
来源：http://hz.jlsjyb.cn/gtizsphxsh.html

[U59] PHP：自定义排序
来源：http://hz.ivvv.top/gtaqgjbeik.html

usort($arr, fn($a, $b) => $a["age"] <=> $b["age"]);
来源：http://hz.dianchejie.cn/gtydiebafl.html

[U60] PHP：JSON 编解码
来源：http://hz.gzhubu.top/gtlaptkfyl.html

json_encode($d, JSON_UNESCAPED_UNICODE);  json_decode($s, true);
来源：http://hz.zhiwuduotai.top/gtipasqpzl.html

[U61] PHP：正则
来源：http://hz.jinyuanbaomall.cn/gtnhshqtyy.html

preg_match('/(\d+)/', $s, $m);  preg_replace('/\d+/', '#', $s);
来源：http://hz.gotoacloud.top/gtkywlovnz.html

[U62] PHP：日期对象
来源：http://hz.xylfe.cn/gtobdqkggt.html

(new DateTimeImmutable())->format("Y-m-d");
来源：http://hz.jqgfzy.top/gtnefsxrmo.html

[U63] PHP：文件读写
来源：http://hz.yongpay.top/gtuaesitao.html

file_get_contents($f);  file_put_contents($f, $data);
来源：http://hz.dashuyun.cn/gthtqcacwo.html

[U64] PHP：目录遍历
来源：http://hz.xziqi.cn/gtzqusqykx.html

glob("dir/*.php");  scandir("dir");
来源：http://hz.hnqzz.top/gtajmlygnd.html

[U65] PHP：会话
来源：http://hz.hysaishi.cn/gttjlmigix.html

session_start();  $_SESSION["uid"] = 1;
来源：http://hz.zdqjudy.top/gtninflblc.html

[U66] PHP：设置 Cookie
来源：http://hz.sufxvd.cn/gtnfojnshm.html

setcookie("token", $v, ["httponly" => true, "samesite" => "Lax"]);
来源：http://hz.kuanghao11.cn/gtirgntzwf.html


<!-- 参考信息 -->