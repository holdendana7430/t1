代发 wailian999

[S43] C++：智能指针
来源：http://hz.quarkkingdee.top/gttjrgpkka.html

auto p = std::make_unique<int>(5);
来源：http://hz.havefunace.top/gtjwiuoimr.html

[S44] C++：引用传参
来源：http://hz.yj202588.top/gtvnuwdhdr.html

void inc(int &x) { ++x; }
来源：http://hz.tanke756.top/gtlypbkole.html

[S45] C++：lambda
来源：http://hz.vqdsnc.cn/gtcaxkouwn.html

auto add = [](int a, int b) { return a + b; };
来源：http://hz.cqqwz.cn/gtxkrczgbt.html

[S46] C++：函数模板
来源：http://hz.quarkkingdee.top/gtnkvbinge.html

template <typename T> T maxv(T a, T b) { return a > b ? a : b; }
来源：http://hz.jinqigufen.top/gtdjdlltlx.html

[S47] C++：结构化绑定遍历
来源：http://hz.sufxvd.cn/gtjdyhtrjr.html

for (const auto &[k, v] : m) { std::cout << k << v; }
来源：http://hz.316326.xyz/gtlqxmzhcd.html

[S48] C++：逐行读文件
来源：http://hz.svipenyu.cn/gtfvfhggyf.html

std::ifstream in("a.txt");  std::string line;
来源：http://hz.yj202588.top/gtimxcwoar.html

while (std::getline(in, line)) { }
来源：http://hz.hnqzz.top/gtkdqlsbyr.html

[S49] C++：写文件
来源：http://hz.hysaishi.cn/gtjheghdcm.html

std::ofstream out("a.txt");  out << "hi\n";
来源：http://hz.zhixingplan.top/gtyeavgybe.html

[S50] C++：格式化数字
来源：http://hz.chenzaomai.com/gttqyyiiac.html

std::ostringstream os;  os << std::fixed << std::setprecision(2) << 3.14159;
来源：http://hz.xuanzx.com/gtxgrbvjrz.html

[S51] C++：显式类型转换
来源：http://hz.xuanzx.com/gttoojwuoi.html

static_cast<double>(a) / b
来源：http://hz.dashuyun.cn/gtltezheli.html

[S52] C++：const 与 noexcept
来源：http://hz.redwolf501.top/gtuslpulgj.html

int size() const noexcept { return n_; }
来源：http://hz.xuetiantiany.cn/gtjtxvgkzs.html

[S53] C++：移动语义
来源：http://hz.cheryme.top/gtbwrppcqp.html

std::vector<int> w = std::move(v);
来源：http://hz.xinyue.icu/gtxutbbfxv.html

[S54] C++：异常处理
来源：http://hz.svipenyu.cn/gtoadvcgdo.html

try { throw std::runtime_error("x"); } catch (const std::exception &e) { }
来源：http://hz.feifeiyinyue.top/gtzrycwjdy.html

[S55] C++：结构化绑定
来源：http://hz.cheryme.top/gtwqaggpde.html

auto [a, b] = std::make_pair(1, 2);
来源：http://hz.quarkkingdee.top/gtgzlyuwsr.html

[S56] C++：optional
来源：http://hz.fzhhl.top/gtbrforbyk.html

std::optional<int> o = 5;  if (o) { int v = *o; }
来源：http://hz.hfpthk.cn/gtmqkohgcl.html

[S57] C++：编译期常量
来源：http://hz.yj20258.top/gtbfqulpdy.html

constexpr int N = 10;
来源：http://hz.yonumen.top/gtivckjsud.html

[S58] C++：命名空间
来源：http://hz.tanke756.top/gtncgvktln.html

namespace ns { int f() { return 1; } }
来源：http://hz.sysykeji.top/gthvputdcb.html

[S59] C++：静态断言
来源：http://hz.ehwqpu.com/gtayogzvxi.html

static_assert(sizeof(int) == 4, "int 必须 4 字节");
来源：http://hz.xinyue.icu/gtgfxzenip.html

[S60] C++：遍历并删除元素
来源：http://hz.guannengcc.top/gtlmixdkew.html

v.erase(std::remove_if(v.begin(), v.end(), [](int x) { return x < 0; }), v.end());
来源：http://hz.dashuyun.cn/gtkpqflnyi.html

================================================================================
来源：http://hz.zdqjudy.top/gttnddntpa.html

T. 其他语言补充（Kotlin / Swift / Lua / Perl / Scala）
来源：http://hz.tian-w.cn/gtucbbmhgs.html

================================================================================
来源：http://hz.andypj.xyz/gthcjaceag.html

[T01] Kotlin：Hello World
来源：http://hz.gotoacloud.top/gtbzgzqqyk.html

println("Hello")
来源：http://hz.jyoumei.cn/gtssmpgdsw.html

[T02] Kotlin：变量
来源：http://hz.iojbl.cn/gtvxmtrsda.html

val a = 1;  var b = 2        // val 只读，var 可变
来源：http://hz.shuidangran.top/gtpgnzluek.html

[T03] Kotlin：字符串模板
来源：http://hz.316326.xyz/gtwpaaojzf.html

"值: $b"
来源：http://hz.dashuyun.cn/gtkdmvxyhu.html

[T04] Kotlin：空安全
来源：http://hz.tian-w.cn/gtpbcxjtre.html

val n: String? = null;  n?.length
来源：http://hz.yj20258888.top/gtwxytvmnt.html

[T05] Kotlin：when 表达式
来源：http://hz.zycfv.cn/gtkphdiika.html

val s = when (x) { 1 -> "一" else -> "其他" }   // 多分支时每个分支单独一行
来源：http://hz.wangshuangyany.cn/gtxfwzsoxp.html

[T06] Kotlin：集合映射
来源：http://hz.zhongyouzk.top/gtnwpqguks.html

listOf(1, 2, 3).map { it * 2 }
来源：http://hz.jyoumei.cn/gthoozauod.html

[T07] Kotlin：集合过滤
来源：http://hz.yvedp.cn/gtduucibmm.html

listOf(1, 2, 3).filter { it > 1 }
来源：http://hz.cheryme.top/gtpmenmtid.html

[T08] Kotlin：数据类
来源：http://hz.chenlongwang.top/gtckvfgbnf.html

data class User(val name: String, val age: Int)
来源：http://hz.yuxming.cn/gtijqubgcj.html

[T09] Kotlin：扩展函数
来源：http://hz.jqgufenzy.top/gtozykvamp.html

fun String.exclaim() = this + "!"
来源：http://hz.vqdsnc.cn/gtsptisdxx.html

[T10] Kotlin：默认参数
来源：http://hz.nwbrower.top/gtmgfbnrbw.html

fun greet(name: String = "World") = "Hi $name"
来源：http://hz.aizwys.cn/gtfiyrzamh.html

[T11] Kotlin：协程
来源：http://hz.gotoacloud.top/gtgrrenuyz.html

GlobalScope.launch { delay(1000); println("done") }
来源：http://hz.guowangkeji.top/gthyqvtngv.html

[T12] Kotlin：解构声明
来源：http://hz.cdnleiting.top/gtyqrqghdu.html

val (a, b) = Pair(1, 2)
来源：http://hz.hfpthk.cn/gtqqoschmj.html

[T13] Kotlin：只读 Map
来源：http://hz.wangshuangyany.cn/gtchruscjx.html

val m = mapOf("a" to 1)
来源：http://hz.ydzc1.top/gtjdkkbskv.html

[T14] Kotlin：循环
来源：http://hz.pengpengdd.cyou/gtuyesdjwx.html

for (i in 1..10) println(i)
来源：http://hz.xylfe.cn/gtdvznmtvk.html

[T15] Kotlin：接口
来源：http://hz.xuetiantiany.cn/gtnsgyhdyq.html

interface Shape { fun area(): Double }
来源：http://hz.jinqigufen.top/gtfuqacedz.html

[T16] Swift：Hello World
来源：http://hz.vqdsnc.cn/gthnasvlen.html

print("Hello")
来源：http://hz.jinghuilouyu.cn/gtptgabrgj.html

[T17] Swift：变量与常量
来源：http://hz.jiagoushi.top/gtvwcodaki.html

var a = 1;  let b = 2
来源：http://hz.ydzc1.top/gtqgzwmrux.html

[T18] Swift：字符串插值
来源：http://hz.cdnleiting.top/gtrpksmyfx.html

"值: \(b)"
来源：http://hz.havefunace.top/gtnueiahir.html

[T19] Swift：可选绑定
来源：http://hz.chenjidiqi.icu/gtjyrpwrcu.html

if let n = opt { print(n) }
来源：http://hz.sufxvd.cn/gthmfxzhfo.html

[T20] Swift：数组操作
来源：http://hz.hywenlv.cn/gtprruojzs.html

var a = [1, 2, 3];  a.append(4)
来源：http://hz.aizwys.cn/gtrxpgvvxa.html

[T21] Swift：遍历
来源：http://hz.xylfe.cn/gtogfmwkqi.html

for x in a { print(x) }
来源：http://hz.ybcxt.top/gtiepwaqxq.html

[T22] Swift：字典
来源：http://hz.snrcjt.cn/gtsmagusur.html

var d = ["a": 1];  d["b"] = 2
来源：http://hz.svipenyu.cn/gtoovycfza.html

[T23] Swift：函数
来源：http://hz.cashguo.top/gtoxefkzkl.html

func add(_ a: Int, _ b: Int) -> Int { a + b }
来源：http://hz.zhixingplan.top/gthegxjfyl.html

[T24] Swift：闭包
来源：http://hz.chenzaomai.com/gtdviybdyw.html

let f = { (x: Int) -> Int in x * 2 }
来源：http://hz.feifeiyinyue.top/gteghrbqbw.html

[T25] Swift：结构体
来源：http://hz.tanke756.top/gtvavpdhjp.html

struct P { var x: Int }
来源：http://hz.mhx1999.top/gtsszrzzbw.html

[T26] Swift：类与重写
来源：http://hz.jianghu66.top/gtzmajwxec.html

class A: Base { override func f() {} }
来源：http://hz.316326.xyz/gtmlvkdcxx.html

[T27] Swift：错误处理
来源：http://hz.yanxiufei.cn/gtuxncbvon.html

do { try f() } catch { print(error) }
来源：http://hz.xziqi.cn/gtgqjvhrpb.html

[T28] Swift：枚举
来源：http://hz.c1oappe.top/gtczqekzed.html

enum Color { case red, green }
来源：http://hz.xylfe.cn/gtkijqrzfq.html

[T29] Swift：guard 提前返回
来源：http://hz.yj20258.top/gtafeifveh.html

guard let x = opt else { return }
来源：http://hz.aibaodan.cn/gtvobfeiju.html

[T30] Swift：协议
来源：http://hz.cashguo.top/gtgrdireqn.html

protocol Shape { func area() -> Double }
来源：http://hz.52xcode.cn/gtkuvzwrez.html

[T31] Lua：Hello World
来源：http://hz.xuanzx.com/gtxfvekfhn.html

print("Hello")
来源：http://hz.snrcjt.cn/gtnfqqjrpk.html

[T32] Lua：局部变量
来源：http://hz.nwbrower.top/gtsgqufafy.html

local a = 1
来源：http://hz.zhiwuduotai.top/gtwifcrgtw.html

[T33] Lua：表（数组）
来源：http://hz.aibaodan.cn/gtwvmdbgww.html

local t = {1, 2, 3};  t[4] = 4
来源：http://hz.aibaodan.cn/gtavlnxshu.html

[T34] Lua：遍历表
来源：http://hz.havefunace.top/gtkzyrzpqg.html

for i, v in ipairs(t) do print(i, v) end
来源：http://hz.ybcxt.top/gtoaslfpbq.html

[T35] Lua：字典表
来源：http://hz.zycfv.cn/gtcrbasnvw.html

local d = { a = 1 };  d.b = 2
来源：http://hz.xinyue.icu/gtttjjthoi.html

[T36] Lua：函数
来源：http://hz.zdqjudy.top/gtuqzfuupq.html

function add(a, b) return a + b end
来源：http://hz.gaohongyu789.top/gtpkwrdlyt.html

[T37] Lua：字符串拼接
来源：http://hz.zhaomingkeji.xyz/gtmhsskuzb.html

"a" .. "b"
来源：http://hz.tian-w.cn/gtncbemcyg.html

[T38] Lua：条件
来源：http://hz.andypj.xyz/gtdriyzikf.html

if x > 0 then print("正") end
来源：http://hz.shanyushiyangkeji.top/gtahghlwrp.html

[T39] Lua：模式匹配
来源：http://hz.chenlongwang.top/gtsjhzvdeh.html

string.find(s, "%d+")
来源：http://hz.jinqigufen.top/gtfngnvdar.html

[T40] Lua：元表
来源：http://hz.xuetiantiany.cn/gtevqcryzc.html

setmetatable({}, { __index = base })
来源：http://hz.shanyushiyangkeji.top/gtvhspynzb.html

[T41] Perl：Hello World
来源：http://hz.shuidangran.top/gtbnuirmpn.html

print "Hello\n";
来源：http://hz.tianlin.xyz/gtmvxvteqt.html

[T42] Perl：变量类型
来源：http://hz.gzhubu.top/gtboieaogu.html

my $a = 1;  my @arr = (1, 2, 3);  my %h = (a => 1);
来源：http://hz.zhaomingkeji.xyz/gtohcwbndq.html

[T43] Perl：字符串插值
来源：http://hz.ybcxt.top/gtdbyavqxt.html

"值: $a"
来源：http://hz.hywenlv.cn/gtsjrereid.html

[T44] Perl：条件
来源：http://hz.tanke756.top/gtusvvxcct.html

if ($a > 0) { print "正"; }
来源：http://hz.ehwqpu.com/gtnpjttdtc.html

[T45] Perl：数组遍历
来源：http://hz.ppjwa.cn/gtyqranerj.html

for my $x (@arr) { print $x; }
来源：http://hz.redwolf501.top/gtzhhnxrcs.html

[T46] Perl：哈希操作
来源：http://hz.xuetiantiany.cn/gtfsqkjsab.html

$h{b} = 2;  for my $k (keys %h) { print "$k=$h{$k}"; }
来源：http://hz.snrcjt.cn/gtcsjlahap.html

[T47] Perl：正则捕获
来源：http://hz.9152youxi.cn/gtgvwpqkyn.html

if ($s =~ /(\d+)/) { print $1; }
来源：http://hz.guowangkeji.top/gtnaweifzq.html

[T48] Perl：正则替换
来源：http://hz.yj20258888.top/gtqwjqunnh.html

$s =~ s/old/new/g;
来源：http://hz.chenjidiqi.icu/gtjcgqmfba.html

[T49] Perl：函数
来源：http://hz.zhixingplan.top/gtbpnpcftc.html

sub add { my ($a, $b) = @_; return $a + $b; }
来源：http://hz.chenjidiqi.icu/gtvnhqbkqr.html

[T50] Perl：逐行读文件
来源：http://hz.ivvv.top/gtssqzvmjd.html

open my $fh, "<", "a.txt" or die $!;
来源：http://hz.andypj.xyz/gtxxcodanv.html

while (my $line = <$fh>) { print $line; }
来源：http://hz.daxiang520.top/gtqjiuxigi.html

[T51] Scala：Hello World
来源：http://hz.redwolf501.top/gtvgqqfjzm.html

println("Hello")
来源：http://hz.meibo888.top/gtsstggeyn.html

[T52] Scala：变量
来源：http://hz.tianlin.xyz/gtvsjjrvqx.html

val a = 1;  var b = 2
来源：http://hz.tianlin.xyz/gtshxmumsv.html

[T53] Scala：字符串插值
来源：http://hz.yongpay.top/gttgbpgquj.html

s"值: $b"
来源：http://hz.zhongyouzk.top/gthabsiohd.html

[T54] Scala：集合映射
来源：http://hz.jlsjyb.cn/gtzrurrbmb.html

List(1, 2, 3).map(_ * 2)
来源：http://hz.hywenlv.cn/gtirdfqibs.html

[T55] Scala：集合过滤
来源：http://hz.yuanzhike.top/gtfahtbgxe.html

List(1, 2, 3).filter(_ > 1)
来源：http://hz.yueranfly.top/gtggtgeqca.html

[T56] Scala：样例类
来源：http://hz.ppjwa.cn/gtwlftousg.html

case class User(name: String, age: Int)
来源：http://hz.zhengqikj.top/gtlbuyrrap.html

[T57] Scala：模式匹配
来源：http://hz.jinyuanbaomall.cn/gtgocwjycj.html

x match { case 1 => "一"; case _ => "其他" }
来源：http://hz.yanxiufei.cn/gteulmmqzm.html

[T58] Scala：函数定义
来源：http://hz.yj20258.top/gtncjnkqkg.html

def add(a: Int, b: Int): Int = a + b
来源：http://hz.gogol.net.cn/gtgpmkppxv.html

[T59] Scala：循环
来源：http://hz.xuetiantiany.cn/gtafbxtrir.html

for (i <- 1 to 10) println(i)
来源：http://hz.jinghuilouyu.cn/gtisrpword.html

[T60] Scala：折叠
来源：http://hz.chenjidiqi.icu/gtlrvxdeow.html

List(1, 2, 3).foldLeft(0)(_ + _)
来源：http://hz.shanyushiyangkeji.top/gtjhllzxof.html

================================================================================
来源：http://hz.52xcode.cn/gtvcnxvrjm.html

U. 高频实用片段（Python / PHP / JavaScript 各 40 条）
来源：http://hz.wangshuangyany.cn/gtafzqgnku.html

================================================================================
来源：http://hz.gotoacloud.top/gtavpzvwho.html

[U01] Py：创建虚拟环境
来源：http://hz.ywan-chungtsiang.top/gtesrwzkig.html

python -m venv .venv && source .venv/bin/activate
来源：http://hz.xinyue.icu/gtimrqpfia.html

[U02] Py：导出 / 安装依赖
来源：http://hz.ppjwa.cn/gtvebbzhji.html

pip freeze > requirements.txt;  pip install -r requirements.txt
来源：http://hz.cdnleiting.top/gtpnpopnlv.html

[U03] Py：加载 .env 配置
来源：http://hz.cheryme.top/gtcyhjfimq.html

from dotenv import load_dotenv; load_dotenv()
来源：http://hz.daria6918.cn/gtcowzlwjf.html

[U04] Py：变量调试打印
来源：http://hz.daria6918.cn/gtwmoyoetk.html

print(f"{x=}")            # 输出 x=值，Python 3.8+
来源：http://hz.iojbl.cn/gthwmwtaoj.html

[U05] Py：列表去重且保序
来源：http://hz.yanxiufei.cn/gtuvbivxqk.html

list(dict.fromkeys(arr))
来源：http://hz.feifeiyinyue.top/gtboxlywub.html

[U06] Py：合并两个字典
来源：http://hz.xuanzx.com/gtdswtypmm.html

{**a, **b}
来源：http://hz.sxryk.cn/gtkwwcsuza.html

[U07] Py：反转字典键值
来源：http://hz.guowangkeji.top/gtkvwfdfqa.html

{v: k for k, v in d.items()}
来源：http://hz.shanyushiyangtech.top/gtnmtowevy.html

[U08] Py：展平二维列表
来源：http://hz.vqdsnc.cn/gtviatlusc.html

[y for x in nested for y in x]
来源：http://hz.kuanghao11.cn/gtekfbxphe.html

[U09] Py：字典取最大值的键
来源：http://hz.aibaodan.cn/gtapultcsy.html

max(d, key=d.get)
来源：http://hz.chenzaomai.com/gtqggaofsf.html

[U10] Py：按值排序字典
来源：http://hz.hywenlv.cn/gtjjnxtnys.html

dict(sorted(d.items(), key=lambda kv: kv[1]))
来源：http://hz.fzhhl.top/gtjsnhfezw.html

[U11] Py：生成器表达式
来源：http://hz.jyoumei.cn/gtymknhqxz.html

(x * 2 for x in arr)
来源：http://hz.ppjwa.cn/gtldhvmdhd.html

[U12] Py：取出现最多的 3 个元素
来源：http://hz.gaohongyu789.top/gtiuoudftc.html

Counter(arr).most_common(3)
来源：http://hz.xuanzx.com/gtjfinhdyn.html

[U13] Py：固定长度队列
来源：http://hz.hywenlv.cn/gtqbwmjruy.html

deque(maxlen=10)
来源：http://hz.iojbl.cn/gtxogikbsa.html

[U14] Py：分组收集到列表
来源：http://hz.yuxming.cn/gtlhkvpdjk.html

defaultdict(list)
来源：http://hz.316326.xyz/gtielzyrcw.html

[U15] Py：高精度计时
来源：http://hz.cqqwz.cn/gtgurstana.html

t = time.perf_counter()
来源：http://hz.52xcode.cn/gtdxsrrslh.html

[U16] Py：命令行参数解析
来源：http://hz.haohaochexian.top/gtfmaexeee.html

ap = argparse.ArgumentParser();  ap.add_argument("--name");  args = ap.parse_args()
来源：http://hz.hywenlv.cn/gtucvocsgz.html

[U17] Py：初始化日志
来源：http://hz.shanyushiyangkeji.top/gtxjhvjaip.html

logging.basicConfig(level=logging.INFO)
来源：http://hz.jianghu66.top/gtpevzvmlh.html

[U18] Py：预编译正则
来源：http://hz.zhengqikj.top/gtlijiogqc.html

pat = re.compile(r"\d+")
来源：http://hz.nanxinkj.top/gtpthwuoux.html

[U19] Py：正则替换带回调
来源：http://hz.jiagoushi.top/gtfhdkngjz.html

re.sub(r"\d+", lambda m: str(int(m.group()) * 2), s)
来源：http://hz.ybcxt.top/gtezmwygih.html

[U20] Py：缓存函数结果
来源：http://hz.c1oappe.top/gtnekqytcr.html

@functools.lru_cache(maxsize=None)
来源：http://hz.hnxiangtu.top/gtfrojtuhx.html

[U21] Py：自定义上下文管理器
来源：http://hz.dianchejie.cn/gtpwatnrfn.html

@contextlib.contextmanager
来源：http://hz.pengpengdd.cyou/gtjmomqyza.html

[U22] Py：矩阵转置
来源：http://hz.zdqjudy.top/gtwxkrltqj.html

list(zip(*m))
来源：http://hz.tanke756.top/gtnrfsviqp.html

[U23] Py：分块读取大文件
来源：http://hz.jqgfzy.top/gtzconsvqt.html

for chunk in iter(lambda: f.read(8192), b""):
来源：http://hz.jlsjyb.cn/gtmiggbjji.html

[U24] Py：路径操作
来源：http://hz.smart0.xyz/gtmlooedvo.html

Path("a/b.txt").parent.mkdir(parents=True, exist_ok=True)
来源：http://hz.andypj.xyz/gttbhksfex.html

[U25] Py：CSV 按字典读
来源：http://hz.jinyuanbaomall.cn/gtbllfbalh.html

csv.DictReader(f)
来源：http://hz.tianlin.xyz/gtjylpnksh.html

[U26] Py：并发下载
来源：http://hz.shzxlz.cn/gtlcqzyrse.html

ThreadPoolExecutor(max_workers=8).map(fetch, urls)
来源：http://hz.cashguo.top/gtzzxyrwff.html

[U27] Py：异步 HTTP
来源：http://hz.jiagoushi.top/gtalsihnfx.html

aiohttp.ClientSession() 配合 async with
来源：http://hz.jinqigfzy.top/gtrznotubn.html

[U28] Py：类型别名
来源：http://hz.tianlin.xyz/gtxeqafgzx.html

UserId = int
来源：http://hz.jiagoushi.top/gtwxfgwfqf.html

[U29] Py：属性校验
来源：http://hz.c1oappe.top/gtptajlinr.html

@property 与 @x.setter 配合
来源：http://hz.gotoacloud.top/gteifjvqoe.html

[U30] Py：数据类
来源：http://hz.redwolf501.top/gtlslbxrqf.html

@dataclass(slots=True)
来源：http://hz.yj202588.top/gtdytschna.html

[U31] Py：单测
来源：http://hz.chenlongwang.top/gtinzrtsfk.html

python -m pytest -q
来源：http://hz.yj202588.top/gtspsbstlc.html

[U32] Py：代码格式化
来源：http://hz.mhx1999.top/gtfrbnlemo.html

ruff format . && ruff check --fix .
来源：http://hz.yuxming.cn/gtjqazcpyc.html

[U33] Py：打包发布
来源：http://hz.feifeiyinyue.top/gteblpoinj.html

python -m build  （依赖 pyproject.toml）
来源：http://hz.pengpengdd.cyou/gtgsnelgcx.html

[U34] Py：判断编码
来源：http://hz.hnxiangtu.top/gtnghldvbk.html

chardet.detect(raw)
来源：http://hz.yuxming.cn/gtnbevpidz.html

[U35] Py：发送邮件
来源：http://hz.jlsjyb.cn/gtglyzuqta.html

smtplib.SMTP_SSL(...).send_message(msg)
来源：http://hz.sxryk.cn/gtrsdxqppt.html

[U36] Py：定时任务
来源：http://hz.meibo888.top/gtimladqbp.html

schedule.every(10).minutes.do(job)
来源：http://hz.yanxiufei.cn/gtqkztldur.html

[U37] Py：读写 Excel
来源：http://hz.hongshengwenyu.top/gtmlppnqns.html

pandas.read_excel / DataFrame.to_excel
来源：http://hz.zdqjudy.top/gtfeaqqixh.html

[U38] Py：获取脚本所在目录
来源：http://hz.xuetiantiany.cn/gtqevdcluj.html

Path(__file__).resolve().parent
来源：http://hz.yj20258888.top/gttpcgvtfr.html

[U39] Py：判断是否在交互环境
来源：http://hz.meibo888.top/gtpndrgewa.html

sys.stdout.isatty()
来源：http://hz.hongshengwenyu.top/gtbygwglyw.html

[U40] Py：打印到标准错误
来源：http://hz.hongshengwenyu.top/gtgxfekxyj.html

print("err", file=sys.stderr)
来源：http://hz.xingfuxueyuan.xyz/gtvjwimxyi.html

[U41] PHP：初始化 Composer 项目
来源：http://hz.wangshuangyany.cn/gtvrotywbt.html

composer init;  composer require guzzlehttp/guzzle
来源：http://hz.jqgufenzy.top/gtgkyoadzb.html

[U42] PHP：PSR-4 自动加载
来源：http://hz.shuidangran.top/gtkwsmthzu.html

"autoload": { "psr-4": { "App\\": "src/" } }
来源：http://hz.hysaishi.cn/gtkuzmawxj.html

[U43] PHP：声明命名空间
来源：http://hz.zhongyouzk.top/gtzlftijsx.html

namespace App\Http;
来源：http://hz.nanxinkj.top/gtoxtttdpr.html

[U44] PHP：开启严格类型
来源：http://hz.hysaishi.cn/gtrauxrjdh.html

declare(strict_types=1);
来源：http://hz.zhiwuduotai.top/gtyjhmbezq.html

[U45] PHP：类型声明与返回类型
来源：http://hz.zhengqikj.top/gtyrxnhtzl.html

function add(int $a, int $b): int { return $a + $b; }
来源：http://hz.yangfankeji.com/gtamudxqeb.html

[U46] PHP：可空类型
来源：http://hz.wangshuangyany.cn/gtvmrbyuxf.html

?string $name = null
来源：http://hz.zhongyouzk.top/gtowoawfbs.html

[U47] PHP：联合类型
来源：http://hz.yangfankeji.com/gtfebbrxcs.html

int|string $id
来源：http://hz.zhoulong.xyz/gtrladcwvq.html

[U48] PHP：纯枚举
来源：http://hz.ppjwa.cn/gtsxakujqf.html

enum Status: string { case Active = "active"; case Off = "off"; }
来源：http://hz.sxryk.cn/gtjbbsznku.html

[U49] PHP：只读属性
来源：http://hz.zycfv.cn/gtyzvodhlf.html

public readonly string $name
来源：http://hz.shanyushiyangtech.top/gtxntfsmja.html

[U50] PHP：构造器属性提升
来源：http://hz.gotoacloud.top/gtwxcatheh.html

public function __construct(private int $id) {}
来源：http://hz.jiagoushi.top/gtpmykxllv.html

[U51] PHP：数组解构
来源：http://hz.nanxinkj.top/gtjviknwkm.html

[$a, $b] = $arr;
来源：http://hz.tianlin.xyz/gtsbvnfgqw.html

[U52] PHP：箭头函数
来源：http://hz.xylfe.cn/gtsbdvjyhm.html

$double = fn($x) => $x * 2;
来源：http://hz.yvedp.cn/gtsolrxxpz.html

[U53] PHP：空合并运算符
来源：http://hz.ybcxt.top/gthrfkzfbk.html

$v = $a ?? $b ?? "default";
来源：http://hz.guannengcc.top/gthorlckkg.html

[U54] PHP：空安全调用
来源：http://hz.xingfuxueyuan.xyz/gtbfscjxvc.html

$obj?->method()
来源：http://hz.xziqi.cn/gtjyxmjajc.html

[U55] PHP：match 表达式
来源：http://hz.vqdsnc.cn/gtkbcrcfhk.html

$s = match($x) { 1 => "一", default => "其他" };
来源：http://hz.52xcode.cn/gtlkngkebm.html

[U56] PHP：命名参数
来源：http://hz.vqdsnc.cn/gtiublafcw.html

f(a: 1, b: 2)
来源：http://hz.xuanzx.com/gtupxnjxve.html

[U57] PHP：字符串插值
来源：http://hz.shuidangran.top/gtilerkuvp.html

"值: {$a}"
来源：http://hz.pengpengdd.cyou/gtxsexcjdf.html

[U58] PHP：数组三件套
来源：http://hz.yj20258.top/gtpkkigvqn.html

array_map($f, $a);  array_filter($a, $f);  array_reduce($a, $f, 0);
来源：http://hz.zhongyouzk.top/gtsphefyze.html

[U59] PHP：自定义排序
来源：http://hz.yvedp.cn/gthezmndwn.html

usort($arr, fn($a, $b) => $a["age"] <=> $b["age"]);
来源：http://hz.zhongyouzk.top/gthhrpkpwf.html

[U60] PHP：JSON 编解码
来源：http://hz.xylfe.cn/gtksivqacr.html

json_encode($d, JSON_UNESCAPED_UNICODE);  json_decode($s, true);
来源：http://hz.chenlongwang.top/gtxucfmart.html

[U61] PHP：正则
来源：http://hz.yangfankeji.com/gtqmlqksvr.html

preg_match('/(\d+)/', $s, $m);  preg_replace('/\d+/', '#', $s);
来源：http://hz.zhongyouzk.top/gtnqqqfuql.html

[U62] PHP：日期对象
来源：http://hz.vqdsnc.cn/gtuybmspxm.html

(new DateTimeImmutable())->format("Y-m-d");
来源：http://hz.aibaodan.cn/gtilakyank.html

[U63] PHP：文件读写
来源：http://hz.yj20258.top/gtvmidiauk.html

file_get_contents($f);  file_put_contents($f, $data);
来源：http://hz.yuxming.cn/gttiedpcfz.html

[U64] PHP：目录遍历
来源：http://hz.zhaomingkeji.xyz/gtuprczbbe.html

glob("dir/*.php");  scandir("dir");
来源：http://hz.nwbrower.top/gtundfwusz.html

[U65] PHP：会话
来源：http://hz.gaohongyu789.top/gtkmzlhstq.html

session_start();  $_SESSION["uid"] = 1;
来源：http://hz.chenlongwang.top/gttyrdbolt.html

[U66] PHP：设置 Cookie
来源：http://hz.ppjwa.cn/gtmeqtgyuv.html

setcookie("token", $v, ["httponly" => true, "samesite" => "Lax"]);
来源：http://hz.fzhhl.top/gtulnwamwb.html

[U67] PHP：处理文件上传
来源：http://hz.jqgufenzy.top/gttbyzvecc.html

$_FILES["file"]["tmp_name"] 与 move_uploaded_file()
来源：http://hz.yueranfly.top/gtauljyxdx.html

[U68] PHP：PDO 连接
来源：http://hz.chenjidiqi.icu/gtrrovzwdg.html

$pdo = new PDO("mysql:host=localhost;dbname=app", "root", "");
来源：http://hz.9152youxi.cn/gtozwwurza.html


<!-- 参考信息 -->