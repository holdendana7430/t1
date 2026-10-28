代发 wailian999

[S41] C++：类与构造函数
来源：http://hz.xuetiantiany.cn/gtrtcvrida.html

class A { public: A(int v) : x_(v) {} int get() const { return x_; } private: int x_; };
来源：http://hz.aizwys.cn/gtdzqkznfe.html

[S42] C++：继承与虚函数
来源：http://hz.daria6918.cn/gtprnxvvba.html

class B : public Base { public: void f() override {} };
来源：http://hz.0kj1m.cn/gtdzapsrsc.html

[S43] C++：智能指针
来源：http://hz.yanxiufei.cn/gtdygxoeaq.html

auto p = std::make_unique<int>(5);
来源：http://hz.meibo888.top/gtlldbcxbt.html

[S44] C++：引用传参
来源：http://hz.gaohongyu789.top/gtxkshtemg.html

void inc(int &x) { ++x; }
来源：http://hz.hongshengwenyu.top/gtutjdluoh.html

[S45] C++：lambda
来源：http://hz.jqgufenzy.top/gtwfiqbjdh.html

auto add = [](int a, int b) { return a + b; };
来源：http://hz.cqqwz.cn/gtmnngnliw.html

[S46] C++：函数模板
来源：http://hz.feifeiyinyue.top/gthqnxkubl.html

template <typename T> T maxv(T a, T b) { return a > b ? a : b; }
来源：http://hz.jyoumei.cn/gtxgferodv.html

[S47] C++：结构化绑定遍历
来源：http://hz.aibaodan.cn/gtqymufvqd.html

for (const auto &[k, v] : m) { std::cout << k << v; }
来源：http://hz.ivvv.top/gtjanekhjr.html

[S48] C++：逐行读文件
来源：http://hz.hammf.cn/gttnsjwxsk.html

std::ifstream in("a.txt");  std::string line;
来源：http://hz.shuidangran.top/gtmvfpwkqs.html

while (std::getline(in, line)) { }
来源：http://hz.tianlin.xyz/gtvxfmpzkg.html

[S49] C++：写文件
来源：http://hz.sufxvd.cn/gtcstmpjbo.html

std::ofstream out("a.txt");  out << "hi\n";
来源：http://hz.zhoulong.xyz/gtgnyxsien.html

[S50] C++：格式化数字
来源：http://hz.sufxvd.cn/gtqokifsoh.html

std::ostringstream os;  os << std::fixed << std::setprecision(2) << 3.14159;
来源：http://hz.yuanzhike.top/gttofpohzh.html

[S51] C++：显式类型转换
来源：http://hz.jinqigufen.top/gtxqffcknt.html

static_cast<double>(a) / b
来源：http://hz.tian-w.cn/gtyahbvxzz.html

[S52] C++：const 与 noexcept
来源：http://hz.gotoacloud.top/gticqsxecb.html

int size() const noexcept { return n_; }
来源：http://hz.redwolf501.top/gtzvlkjrqk.html

[S53] C++：移动语义
来源：http://hz.jqgfzy.top/gtgvgtfkrm.html

std::vector<int> w = std::move(v);
来源：http://hz.dashuyun.cn/gtosggomqo.html

[S54] C++：异常处理
来源：http://hz.birdmap.top/gtrylrymem.html

try { throw std::runtime_error("x"); } catch (const std::exception &e) { }
来源：http://hz.guowangkeji.top/gtdcghkliv.html

[S55] C++：结构化绑定
来源：http://hz.gogol.net.cn/gtxaqsvtlu.html

auto [a, b] = std::make_pair(1, 2);
来源：http://hz.yueranfly.top/gtgbokenvk.html

[S56] C++：optional
来源：http://hz.yuanzhike.top/gtmlxxzzhn.html

std::optional<int> o = 5;  if (o) { int v = *o; }
来源：http://hz.zhongyouzk.top/gtziqydbkr.html

[S57] C++：编译期常量
来源：http://hz.daria6918.cn/gtawtzjbav.html

constexpr int N = 10;
来源：http://hz.shanyushiyangtech.top/gtsnkkptmk.html

[S58] C++：命名空间
来源：http://hz.cheryme.top/gtubbhimum.html

namespace ns { int f() { return 1; } }
来源：http://hz.jinyuanbaomall.cn/gtekxtohqy.html

[S59] C++：静态断言
来源：http://hz.zhijiandao.cn/gtyvbapggh.html

static_assert(sizeof(int) == 4, "int 必须 4 字节");
来源：http://hz.hysaishi.cn/gtdjbpfypq.html

[S60] C++：遍历并删除元素
来源：http://hz.c1oappe.top/gtxzdhbkdx.html

v.erase(std::remove_if(v.begin(), v.end(), [](int x) { return x < 0; }), v.end());
来源：http://hz.aizwys.cn/gtjetvjdun.html

================================================================================
来源：http://hz.jianghu66.top/gtvfbdtqsr.html

T. 其他语言补充（Kotlin / Swift / Lua / Perl / Scala）
来源：http://hz.cashguo.top/gtmytqnfeb.html

================================================================================
来源：http://hz.gzhubu.top/gtgkazktfp.html

[T01] Kotlin：Hello World
来源：http://hz.nanxuanxn.top/gtsvlhtznv.html

println("Hello")
来源：http://hz.cucudq.cn/gtzkkgvcij.html

[T02] Kotlin：变量
来源：http://hz.hysaishi.cn/gtxwcwyfwv.html

val a = 1;  var b = 2        // val 只读，var 可变
来源：http://hz.ehwqpu.com/gtztydhtzs.html

[T03] Kotlin：字符串模板
来源：http://hz.andypj.xyz/gtwtrxiqxr.html

"值: $b"
来源：http://hz.hnxiangtu.top/gtqnroygqy.html

[T04] Kotlin：空安全
来源：http://hz.yuanzhike.top/gtishnidag.html

val n: String? = null;  n?.length
来源：http://hz.pengpengdd.cyou/gtabvsxteu.html

[T05] Kotlin：when 表达式
来源：http://hz.nanxinkj.top/gtwmqhpgse.html

val s = when (x) { 1 -> "一" else -> "其他" }   // 多分支时每个分支单独一行
来源：http://hz.ydjk.org.cn/gtyrwjlkuc.html

[T06] Kotlin：集合映射
来源：http://hz.jiagoushi.top/gthdnoekyw.html

listOf(1, 2, 3).map { it * 2 }
来源：http://hz.mhx1999.top/gtjosplfsc.html

[T07] Kotlin：集合过滤
来源：http://hz.xuetiantiany.cn/gtpjgvknph.html

listOf(1, 2, 3).filter { it > 1 }
来源：http://hz.yuanzhike.top/gtovbuyypa.html

[T08] Kotlin：数据类
来源：http://hz.nanxuanxn.top/gtlyvezmth.html

data class User(val name: String, val age: Int)
来源：http://hz.ehwqpu.com/gtaawqiqoc.html

[T09] Kotlin：扩展函数
来源：http://hz.dianchejie.cn/gtmrrjhvju.html

fun String.exclaim() = this + "!"
来源：http://hz.feifeiyinyue.top/gtfnclkzlf.html

[T10] Kotlin：默认参数
来源：http://hz.jlsjyb.cn/gtzinzdhpi.html

fun greet(name: String = "World") = "Hi $name"
来源：http://hz.xuanzx.com/gtnkcsguuk.html

[T11] Kotlin：协程
来源：http://hz.316326.xyz/gtmdwrjssy.html

GlobalScope.launch { delay(1000); println("done") }
来源：http://hz.tanke756.top/gtjuhdmgqp.html

[T12] Kotlin：解构声明
来源：http://hz.yongpay.top/gteenkimke.html

val (a, b) = Pair(1, 2)
来源：http://hz.gaohongyu789.top/gtrkaartmd.html

[T13] Kotlin：只读 Map
来源：http://hz.feifeiyinyue.top/gtezbpbosx.html

val m = mapOf("a" to 1)
来源：http://hz.sufxvd.cn/gtpebffwva.html

[T14] Kotlin：循环
来源：http://hz.c1oappe.top/gtltygnrzv.html

for (i in 1..10) println(i)
来源：http://hz.jqgfzy.top/gtuffpyraz.html

[T15] Kotlin：接口
来源：http://hz.kuanghao11.cn/gtjnkmwhrw.html

interface Shape { fun area(): Double }
来源：http://hz.yvedp.cn/gtiqfrlcjs.html

[T16] Swift：Hello World
来源：http://hz.ydjk.org.cn/gtsbpzopig.html

print("Hello")
来源：http://hz.jlsjyb.cn/gtujnktiwz.html

[T17] Swift：变量与常量
来源：http://hz.sysykeji.top/gtmttqypsv.html

var a = 1;  let b = 2
来源：http://hz.tianlin.xyz/gtaupknlrs.html

[T18] Swift：字符串插值
来源：http://hz.yonumen.top/gtbwduwexz.html

"值: \(b)"
来源：http://hz.gaohongyu789.top/gtcdkjcqiy.html

[T19] Swift：可选绑定
来源：http://hz.jianghu66.top/gtqmdxfysp.html

if let n = opt { print(n) }
来源：http://hz.shanyushiyangkeji.top/gtwylnrntm.html

[T20] Swift：数组操作
来源：http://hz.dianchejie.cn/gtwphqjvdh.html

var a = [1, 2, 3];  a.append(4)
来源：http://hz.zycfv.cn/gtmuapgtir.html

[T21] Swift：遍历
来源：http://hz.wangdashe.top/gtcsbmfsxh.html

for x in a { print(x) }
来源：http://hz.jyoumei.cn/gtmwpzvmno.html

[T22] Swift：字典
来源：http://hz.ywan-chungtsiang.top/gtlvrchcud.html

var d = ["a": 1];  d["b"] = 2
来源：http://hz.cucudq.cn/gtqosesfiz.html

[T23] Swift：函数
来源：http://hz.xinyue.icu/gtjfngtgtq.html

func add(_ a: Int, _ b: Int) -> Int { a + b }
来源：http://hz.tianlin.xyz/gtvzkrjpfn.html

[T24] Swift：闭包
来源：http://hz.zycfv.cn/gtcdhcjghe.html

let f = { (x: Int) -> Int in x * 2 }
来源：http://hz.zycfv.cn/gtnswyxthy.html

[T25] Swift：结构体
来源：http://hz.redwolf501.top/gtwkjeoowv.html

struct P { var x: Int }
来源：http://hz.nwbrower.top/gtcazzxgav.html

[T26] Swift：类与重写
来源：http://hz.ydjk.org.cn/gtavfsijgn.html

class A: Base { override func f() {} }
来源：http://hz.redwolf501.top/gtthuznlgj.html

[T27] Swift：错误处理
来源：http://hz.hnqzz.top/gttfoxpcrt.html

do { try f() } catch { print(error) }
来源：http://hz.redwolf501.top/gtcrppjlcu.html

[T28] Swift：枚举
来源：http://hz.tanke756.top/gtgrtlllhn.html

enum Color { case red, green }
来源：http://hz.jinyuanbaomall.cn/gtylkmxrce.html

[T29] Swift：guard 提前返回
来源：http://hz.ydjk.org.cn/gtlmclloit.html

guard let x = opt else { return }
来源：http://hz.tian-w.cn/gtlbhlowsq.html

[T30] Swift：协议
来源：http://hz.ppjwa.cn/gtsdjynrfv.html

protocol Shape { func area() -> Double }
来源：http://hz.snrcjt.cn/gtdyzzozyw.html

[T31] Lua：Hello World
来源：http://hz.quarkkingdee.top/gtcudblnkz.html

print("Hello")
来源：http://hz.ehwqpu.com/gtnoisgbjv.html

[T32] Lua：局部变量
来源：http://hz.jyoumei.cn/gtxpcgnail.html

local a = 1
来源：http://hz.ivvv.top/gtiasavnjs.html

[T33] Lua：表（数组）
来源：http://hz.hywenlv.cn/gtxcojlcom.html

local t = {1, 2, 3};  t[4] = 4
来源：http://hz.gzhubu.top/gtxypihuxb.html

[T34] Lua：遍历表
来源：http://hz.zhongyouzk.top/gtrjsnwxud.html

for i, v in ipairs(t) do print(i, v) end
来源：http://hz.yuanzhike.top/gtgywrjlmq.html

[T35] Lua：字典表
来源：http://hz.mhx1999.top/gtafvmdufp.html

local d = { a = 1 };  d.b = 2
来源：http://hz.gaohongyu789.top/gtbcuvlcdz.html

[T36] Lua：函数
来源：http://hz.cdnleiting.top/gthmuvmiiw.html

function add(a, b) return a + b end
来源：http://hz.fengsongda.top/gtwhvgdykm.html

[T37] Lua：字符串拼接
来源：http://hz.xingfuxueyuan.xyz/gtranusyfr.html

"a" .. "b"
来源：http://hz.smart0.xyz/gtdcdswxxt.html

[T38] Lua：条件
来源：http://hz.chenjidiqi.icu/gtpgfapqtk.html

if x > 0 then print("正") end
来源：http://hz.cheryme.top/gtevzxxcde.html

[T39] Lua：模式匹配
来源：http://hz.ppjwa.cn/gtqgcdpbhj.html

string.find(s, "%d+")
来源：http://hz.gaohongyu789.top/gtmerwwmpy.html

[T40] Lua：元表
来源：http://hz.xuetiantiany.cn/gtgkeagdsc.html

setmetatable({}, { __index = base })
来源：http://hz.yongpay.top/gtpkeawdqg.html

[T41] Perl：Hello World
来源：http://hz.yonumen.top/gtgjxhoclb.html

print "Hello\n";
来源：http://hz.kuanghao11.cn/gtszfqzlks.html

[T42] Perl：变量类型
来源：http://hz.cqqwz.cn/gtdyswiged.html

my $a = 1;  my @arr = (1, 2, 3);  my %h = (a => 1);
来源：http://hz.nanxinkj.top/gtuzrpbnix.html

[T43] Perl：字符串插值
来源：http://hz.tanke756.top/gtblqakdzh.html

"值: $a"
来源：http://hz.daria6918.cn/gtwssiesst.html

[T44] Perl：条件
来源：http://hz.ydzc1.top/gtgcpoircs.html

if ($a > 0) { print "正"; }
来源：http://hz.shangyingyoupin.top/gtmiqcsgji.html

[T45] Perl：数组遍历
来源：http://hz.jianghu66.top/gtdtqgcfwx.html

for my $x (@arr) { print $x; }
来源：http://hz.hysaishi.cn/gtvcdddozj.html

[T46] Perl：哈希操作
来源：http://hz.cucudq.cn/gtfrghqgcc.html

$h{b} = 2;  for my $k (keys %h) { print "$k=$h{$k}"; }
来源：http://hz.zycfv.cn/gtryhcorkk.html

[T47] Perl：正则捕获
来源：http://hz.yj20258.top/gtyebuobqb.html

if ($s =~ /(\d+)/) { print $1; }
来源：http://hz.shuidangran.top/gtrpsubhze.html

[T48] Perl：正则替换
来源：http://hz.iojbl.cn/gtfwibbphm.html

$s =~ s/old/new/g;
来源：http://hz.chenlongwang.top/gtubporjhy.html

[T49] Perl：函数
来源：http://hz.yongpay.top/gtbkdgcdcs.html

sub add { my ($a, $b) = @_; return $a + $b; }
来源：http://hz.chenjidiqi.icu/gtquzgxscg.html

[T50] Perl：逐行读文件
来源：http://hz.daria6918.cn/gtzdzyumqp.html

open my $fh, "<", "a.txt" or die $!;
来源：http://hz.ydjk.org.cn/gtpowuiwqh.html

while (my $line = <$fh>) { print $line; }
来源：http://hz.hnqzz.top/gtxiwtdqhs.html

[T51] Scala：Hello World
来源：http://hz.yj20258.top/gtcsxcttcs.html

println("Hello")
来源：http://hz.sxryk.cn/gtljqymjre.html

[T52] Scala：变量
来源：http://hz.xinyue.icu/gtrmjgrwqt.html

val a = 1;  var b = 2
来源：http://hz.yj202588.top/gtvjgqceic.html

[T53] Scala：字符串插值
来源：http://hz.jiagoushi.top/gtcsmrfjbu.html

s"值: $b"
来源：http://hz.meibo888.top/gthsffkaqq.html

[T54] Scala：集合映射
来源：http://hz.cashguo.top/gtmozqgapy.html

List(1, 2, 3).map(_ * 2)
来源：http://hz.gzhubu.top/gtoxuphsgd.html

[T55] Scala：集合过滤
来源：http://hz.yanxiufei.cn/gtanlgvgaz.html

List(1, 2, 3).filter(_ > 1)
来源：http://hz.xuetiantiany.cn/gtncpvpywk.html

[T56] Scala：样例类
来源：http://hz.xingfuxueyuan.xyz/gtwuzpnxfm.html

case class User(name: String, age: Int)
来源：http://hz.guowangkeji.top/gtkuighnax.html

[T57] Scala：模式匹配
来源：http://hz.hnxiangtu.top/gtjnixzxyk.html

x match { case 1 => "一"; case _ => "其他" }
来源：http://hz.cheryme.top/gtunaokscl.html

[T58] Scala：函数定义
来源：http://hz.aibaodan.cn/gtqbofnyxk.html

def add(a: Int, b: Int): Int = a + b
来源：http://hz.gogol.net.cn/gtmiewevie.html

[T59] Scala：循环
来源：http://hz.ydzc1.top/gtpohbaaed.html

for (i <- 1 to 10) println(i)
来源：http://hz.shanyushiyangtech.top/gtfnybdszr.html

[T60] Scala：折叠
来源：http://hz.pycfn.com/gtcirnruki.html

List(1, 2, 3).foldLeft(0)(_ + _)
来源：http://hz.kuanghao11.cn/gtjurxrdkl.html

================================================================================
来源：http://hz.xziqi.cn/gtyaxkheij.html

U. 高频实用片段（Python / PHP / JavaScript 各 40 条）
来源：http://hz.nwbrower.top/gtgalxgmnn.html

================================================================================
来源：http://hz.hnxiangtu.top/gtbmmfzmnk.html

[U01] Py：创建虚拟环境
来源：http://hz.jiagoushi.top/gtvxjlsxhy.html

python -m venv .venv && source .venv/bin/activate
来源：http://hz.kuanghao11.cn/gtwbxrojde.html

[U02] Py：导出 / 安装依赖
来源：http://hz.yuanzhike.top/gtfnyircoj.html

pip freeze > requirements.txt;  pip install -r requirements.txt
来源：http://hz.hnqzz.top/gtomeahhll.html

[U03] Py：加载 .env 配置
来源：http://hz.jianghu66.top/gtcwxrsvxz.html

from dotenv import load_dotenv; load_dotenv()
来源：http://hz.jiagoushi.top/gtabuxvsxz.html

[U04] Py：变量调试打印
来源：http://hz.wangdashe.top/gtteogwvbn.html

print(f"{x=}")            # 输出 x=值，Python 3.8+
来源：http://hz.shuidangran.top/gtslebaokj.html

[U05] Py：列表去重且保序
来源：http://hz.tanke756.top/gtsmbuazxm.html

list(dict.fromkeys(arr))
来源：http://hz.jyoumei.cn/gthcvrovui.html

[U06] Py：合并两个字典
来源：http://hz.sweek.top/gtiqualapn.html

{**a, **b}
来源：http://hz.yangfankeji.com/gtgyjtzgxg.html

[U07] Py：反转字典键值
来源：http://hz.ivvv.top/gtdwhrhgyc.html

{v: k for k, v in d.items()}
来源：http://hz.mhx1999.top/gtjjkqllfp.html

[U08] Py：展平二维列表
来源：http://hz.pengpengdd.cyou/gtpgxsiznz.html

[y for x in nested for y in x]
来源：http://hz.cdnleiting.top/gtqbgmeous.html

[U09] Py：字典取最大值的键
来源：http://hz.xziqi.cn/gtsdoogdrf.html

max(d, key=d.get)
来源：http://hz.9152youxi.cn/gtlgmaefem.html

[U10] Py：按值排序字典
来源：http://hz.jinqigufen.top/gtlacqdgkg.html

dict(sorted(d.items(), key=lambda kv: kv[1]))
来源：http://hz.hongshengwenyu.top/gtfmvgnlqj.html

[U11] Py：生成器表达式
来源：http://hz.vqdsnc.cn/gtfvusbawg.html

(x * 2 for x in arr)
来源：http://hz.yj202588.top/gtunoharxg.html

[U12] Py：取出现最多的 3 个元素
来源：http://hz.yonumen.top/gtemwhgxgx.html

Counter(arr).most_common(3)
来源：http://hz.nanxinkj.top/gtvbfbvmzf.html

[U13] Py：固定长度队列
来源：http://hz.iojbl.cn/gtkrjownlf.html

deque(maxlen=10)
来源：http://hz.jqgufenzy.top/gtluucbstc.html

[U14] Py：分组收集到列表
来源：http://hz.shuidangran.top/gtzujpottn.html

defaultdict(list)
来源：http://hz.yanxiufei.cn/gtqeqdooqh.html

[U15] Py：高精度计时
来源：http://hz.ppjwa.cn/gteaxitmvn.html

t = time.perf_counter()
来源：http://hz.dianchejie.cn/gtsivmdarx.html

[U16] Py：命令行参数解析
来源：http://hz.jinyuanbaomall.cn/gtijgwomua.html

ap = argparse.ArgumentParser();  ap.add_argument("--name");  args = ap.parse_args()
来源：http://hz.yongpay.top/gtaczqidzt.html

[U17] Py：初始化日志
来源：http://hz.yangfankeji.com/gtmnvxdkwl.html

logging.basicConfig(level=logging.INFO)
来源：http://hz.birdmap.top/gtikvbofdc.html

[U18] Py：预编译正则
来源：http://hz.pengpengdd.cyou/gtthrxbrjc.html

pat = re.compile(r"\d+")
来源：http://hz.fzhhl.top/gtmzcgwpos.html

[U19] Py：正则替换带回调
来源：http://hz.zhengqikj.top/gtacsgujyv.html

re.sub(r"\d+", lambda m: str(int(m.group()) * 2), s)
来源：http://hz.kuanghao11.cn/gtezrxkxgs.html

[U20] Py：缓存函数结果
来源：http://hz.cheryme.top/gtrvuemzoz.html

@functools.lru_cache(maxsize=None)
来源：http://hz.sweek.top/gthddmkrnm.html

[U21] Py：自定义上下文管理器
来源：http://hz.redwolf501.top/gtypvjjowu.html

@contextlib.contextmanager
来源：http://hz.jyoumei.cn/gtealrmvpv.html

[U22] Py：矩阵转置
来源：http://hz.daxiang520.top/gtnrbycura.html

list(zip(*m))
来源：http://hz.yuxming.cn/gtomtquuof.html

[U23] Py：分块读取大文件
来源：http://hz.gzhubu.top/gtiiicdyqa.html

for chunk in iter(lambda: f.read(8192), b""):
来源：http://hz.jinyuanbaomall.cn/gtmkdfvxvz.html

[U24] Py：路径操作
来源：http://hz.pengpengdd.cyou/gtxzycmgsf.html

Path("a/b.txt").parent.mkdir(parents=True, exist_ok=True)
来源：http://hz.svipenyu.cn/gtpqxqncgd.html

[U25] Py：CSV 按字典读
来源：http://hz.zhengqikj.top/gtznwubnmj.html

csv.DictReader(f)
来源：http://hz.xziqi.cn/gtitrikznr.html

[U26] Py：并发下载
来源：http://hz.nwbrower.top/gtjnqmwbqz.html

ThreadPoolExecutor(max_workers=8).map(fetch, urls)
来源：http://hz.yj202588.top/gtylhmzjgl.html

[U27] Py：异步 HTTP
来源：http://hz.hnqzz.top/gtuweojopb.html

aiohttp.ClientSession() 配合 async with
来源：http://hz.cdnleiting.top/gtftyilxxf.html

[U28] Py：类型别名
来源：http://hz.daria6918.cn/gtetmqfhqh.html

UserId = int
来源：http://hz.hnqzz.top/gtzbwoxkqt.html

[U29] Py：属性校验
来源：http://hz.sysykeji.top/gtkucoxtpc.html

@property 与 @x.setter 配合
来源：http://hz.feifeiyinyue.top/gtxvmokkeo.html

[U30] Py：数据类
来源：http://hz.fzhhl.top/gtpzocterw.html

@dataclass(slots=True)
来源：http://hz.jlsjyb.cn/gtmsqudxff.html

[U31] Py：单测
来源：http://hz.yongpay.top/gtzfiwyybu.html

python -m pytest -q
来源：http://hz.yangfankeji.com/gtjwjqtjfz.html

[U32] Py：代码格式化
来源：http://hz.zhaomingkeji.xyz/gtcynflmyd.html

ruff format . && ruff check --fix .
来源：http://hz.zhoulong.xyz/gtthnyjoes.html

[U33] Py：打包发布
来源：http://hz.ppjwa.cn/gtpamofxgw.html

python -m build  （依赖 pyproject.toml）
来源：http://hz.ywan-chungtsiang.top/gtckekfsst.html

[U34] Py：判断编码
来源：http://hz.yanxiufei.cn/gtgrylexjy.html

chardet.detect(raw)
来源：http://hz.haohaochexian.top/gtdbvefgii.html

[U35] Py：发送邮件
来源：http://hz.zhengqikj.top/gtwqpccatr.html

smtplib.SMTP_SSL(...).send_message(msg)
来源：http://hz.gogol.net.cn/gtoshymlxf.html

[U36] Py：定时任务
来源：http://hz.pengpengdd.cyou/gtgpgyxuaq.html

schedule.every(10).minutes.do(job)
来源：http://hz.yangfankeji.com/gtgbvovcdg.html

[U37] Py：读写 Excel
来源：http://hz.nwbrower.top/gtfkxlyfxi.html

pandas.read_excel / DataFrame.to_excel
来源：http://hz.gotoacloud.top/gtdfpxpcnl.html

[U38] Py：获取脚本所在目录
来源：http://hz.bjfxy.top/gtszkcckie.html

Path(__file__).resolve().parent
来源：http://hz.yuanzhike.top/gttcxaraok.html

[U39] Py：判断是否在交互环境
来源：http://hz.redwolf501.top/gtoalagirn.html

sys.stdout.isatty()
来源：http://hz.jinqigufen.top/gtgljecwmu.html

[U40] Py：打印到标准错误
来源：http://hz.aibaodan.cn/gtrjkrxzsu.html

print("err", file=sys.stderr)
来源：http://hz.xylfe.cn/gtrsoeoljh.html

[U41] PHP：初始化 Composer 项目
来源：http://hz.chenlongwang.top/gtbqbxdhht.html

composer init;  composer require guzzlehttp/guzzle
来源：http://hz.cqqwz.cn/gtighiiunj.html

[U42] PHP：PSR-4 自动加载
来源：http://hz.haohaochexian.top/gtuhffijqx.html

"autoload": { "psr-4": { "App\\": "src/" } }
来源：http://hz.hnqzz.top/gtggozbyfm.html

[U43] PHP：声明命名空间
来源：http://hz.yj202588.top/gtmhzwtzuv.html

namespace App\Http;
来源：http://hz.ehwqpu.com/gtmyrhgrki.html

[U44] PHP：开启严格类型
来源：http://hz.tian-w.cn/gtfhjmnwbm.html

declare(strict_types=1);
来源：http://hz.chenzaomai.com/gtcdazscfs.html

[U45] PHP：类型声明与返回类型
来源：http://hz.jinyuanbaomall.cn/gtlcmmafzv.html

function add(int $a, int $b): int { return $a + $b; }
来源：http://hz.zhoulong.xyz/gtaddboyrw.html

[U46] PHP：可空类型
来源：http://hz.daria6918.cn/gtdlrcehcn.html

?string $name = null
来源：http://hz.zhaomingkeji.xyz/gtyotshkhn.html

[U47] PHP：联合类型
来源：http://hz.jqgufenzy.top/gtxcswjmih.html

int|string $id
来源：http://hz.havefunace.top/gtiryjejch.html

[U48] PHP：纯枚举
来源：http://hz.gotoacloud.top/gtsslfkmin.html

enum Status: string { case Active = "active"; case Off = "off"; }
来源：http://hz.zhijiandao.cn/gtojtrgfik.html

[U49] PHP：只读属性
来源：http://hz.zhixingplan.top/gtwijzyxhd.html

public readonly string $name
来源：http://hz.52xcode.cn/gtsravmfrb.html

[U50] PHP：构造器属性提升
来源：http://hz.iojbl.cn/gthzrgkzzg.html

public function __construct(private int $id) {}
来源：http://hz.52xcode.cn/gtsosbtgfn.html

[U51] PHP：数组解构
来源：http://hz.tanke756.top/gtlpfzhurp.html

[$a, $b] = $arr;
来源：http://hz.yanxiufei.cn/gtmibnksvg.html

[U52] PHP：箭头函数
来源：http://hz.jinqigufen.top/gtxfviupjx.html

$double = fn($x) => $x * 2;
来源：http://hz.tanke756.top/gtlkjxbxoq.html

[U53] PHP：空合并运算符
来源：http://hz.xziqi.cn/gtlgnfgpfb.html

$v = $a ?? $b ?? "default";
来源：http://hz.pengpengdd.cyou/gtpuqvtmfv.html

[U54] PHP：空安全调用
来源：http://hz.tanke756.top/gthtnvfhiv.html

$obj?->method()
来源：http://hz.sysykeji.top/gtdtllzvzl.html

[U55] PHP：match 表达式
来源：http://hz.pycfn.com/gtqfrgqrnj.html

$s = match($x) { 1 => "一", default => "其他" };
来源：http://hz.ydzc1.top/gtwwmmuxrs.html

[U56] PHP：命名参数
来源：http://hz.iojbl.cn/gtxzbymjgz.html

f(a: 1, b: 2)
来源：http://hz.cdnleiting.top/gtnvcwbxlj.html

[U57] PHP：字符串插值
来源：http://hz.ivvv.top/gtzgrhxvfn.html

"值: {$a}"
来源：http://hz.havefunace.top/gtjxrurpdp.html

[U58] PHP：数组三件套
来源：http://hz.gotoacloud.top/gtstbqzyvr.html

array_map($f, $a);  array_filter($a, $f);  array_reduce($a, $f, 0);
来源：http://hz.zhoulong.xyz/gtagvgtvrz.html

[U59] PHP：自定义排序
来源：http://hz.xziqi.cn/gtsjbhziid.html

usort($arr, fn($a, $b) => $a["age"] <=> $b["age"]);
来源：http://hz.guannengcc.top/gttghuvqek.html

[U60] PHP：JSON 编解码
来源：http://hz.52xcode.cn/gtcuavphko.html

json_encode($d, JSON_UNESCAPED_UNICODE);  json_decode($s, true);
来源：http://hz.zhongyouzk.top/gtdaapnmsd.html

[U61] PHP：正则
来源：http://hz.fengsongda.top/gtrecfbyat.html

preg_match('/(\d+)/', $s, $m);  preg_replace('/\d+/', '#', $s);
来源：http://hz.0kj1m.cn/gtbsukpikk.html

[U62] PHP：日期对象
来源：http://hz.xuetiantiany.cn/gtsuflnrat.html

(new DateTimeImmutable())->format("Y-m-d");
来源：http://hz.yvedp.cn/gtgfrqvanm.html

[U63] PHP：文件读写
来源：http://hz.vqdsnc.cn/gtjuwzzlot.html

file_get_contents($f);  file_put_contents($f, $data);
来源：http://hz.snrcjt.cn/gtcmsglrrs.html

[U64] PHP：目录遍历
来源：http://hz.mhx1999.top/gtbxqtxxnv.html

glob("dir/*.php");  scandir("dir");
来源：http://hz.zhengqikj.top/gtevikajdl.html

[U65] PHP：会话
来源：http://hz.feifeiyinyue.top/gtgccauoxy.html

session_start();  $_SESSION["uid"] = 1;
来源：http://hz.meibo888.top/gtuegnzrhm.html

[U66] PHP：设置 Cookie
来源：http://hz.havefunace.top/gtusviwtsc.html

setcookie("token", $v, ["httponly" => true, "samesite" => "Lax"]);
来源：http://hz.svipenyu.cn/gtawbqtasg.html


<!-- 参考信息 -->