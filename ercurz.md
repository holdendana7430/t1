代发 wailian999

[S41] C++：类与构造函数
来源：http://hz.tanke756.top/gtcduaqivj.html

class A { public: A(int v) : x_(v) {} int get() const { return x_; } private: int x_; };
来源：http://hz.sweek.top/gtrzbvaata.html

[S42] C++：继承与虚函数
来源：http://hz.yvedp.cn/gtfguobyws.html

class B : public Base { public: void f() override {} };
来源：http://hz.yuxming.cn/gtfnkcrskw.html

[S43] C++：智能指针
来源：http://hz.gotoacloud.top/gtubeazcvs.html

auto p = std::make_unique<int>(5);
来源：http://hz.yangfankeji.com/gtjaixfpva.html

[S44] C++：引用传参
来源：http://hz.gaohongyu789.top/gtotzwveep.html

void inc(int &x) { ++x; }
来源：http://hz.yonumen.top/gtmfqkrehx.html

[S45] C++：lambda
来源：http://hz.hywenlv.cn/gtctrikafx.html

auto add = [](int a, int b) { return a + b; };
来源：http://hz.zhiwuduotai.top/gtdhfxzmzd.html

[S46] C++：函数模板
来源：http://hz.quarkkingdee.top/gtdkzopppv.html

template <typename T> T maxv(T a, T b) { return a > b ? a : b; }
来源：http://hz.xuetiantiany.cn/gthnxqnovb.html

[S47] C++：结构化绑定遍历
来源：http://hz.ywan-chungtsiang.top/gttananzcz.html

for (const auto &[k, v] : m) { std::cout << k << v; }
来源：http://hz.xuetiantiany.cn/gthtmcibpt.html

[S48] C++：逐行读文件
来源：http://hz.jyoumei.cn/gtawdxjvmu.html

std::ifstream in("a.txt");  std::string line;
来源：http://hz.ydzc1.top/gtwyrrbmsr.html

while (std::getline(in, line)) { }
来源：http://hz.wangshuangyany.cn/gtouwuetfe.html

[S49] C++：写文件
来源：http://hz.shuidangran.top/gthfosbqij.html

std::ofstream out("a.txt");  out << "hi\n";
来源：http://hz.cdnleiting.top/gtllzuuayk.html

[S50] C++：格式化数字
来源：http://hz.ppjwa.cn/gtsspkhcwr.html

std::ostringstream os;  os << std::fixed << std::setprecision(2) << 3.14159;
来源：http://hz.xinyue.icu/gtactuamwy.html

[S51] C++：显式类型转换
来源：http://hz.sweek.top/gtgeitsiov.html

static_cast<double>(a) / b
来源：http://hz.sxryk.cn/gtxgaakdgp.html

[S52] C++：const 与 noexcept
来源：http://hz.yangfankeji.com/gtlfyttfql.html

int size() const noexcept { return n_; }
来源：http://hz.gogol.net.cn/gtzwisbjzm.html

[S53] C++：移动语义
来源：http://hz.mhx1999.top/gtybrvqoii.html

std::vector<int> w = std::move(v);
来源：http://hz.andypj.xyz/gtazwgprtc.html

[S54] C++：异常处理
来源：http://hz.ivvv.top/gtcmbpfjkx.html

try { throw std::runtime_error("x"); } catch (const std::exception &e) { }
来源：http://hz.sxryk.cn/gtruvykjzw.html

[S55] C++：结构化绑定
来源：http://hz.wangshuangyany.cn/gttqpjzdyf.html

auto [a, b] = std::make_pair(1, 2);
来源：http://hz.wangshuangyany.cn/gttjpsxwez.html

[S56] C++：optional
来源：http://hz.snrcjt.cn/gtgtaburgo.html

std::optional<int> o = 5;  if (o) { int v = *o; }
来源：http://hz.redwolf501.top/gtwejnkpma.html

[S57] C++：编译期常量
来源：http://hz.snrcjt.cn/gttkehpooo.html

constexpr int N = 10;
来源：http://hz.guannengcc.top/gtgvskezwk.html

[S58] C++：命名空间
来源：http://hz.zycfv.cn/gtgcwsejhp.html

namespace ns { int f() { return 1; } }
来源：http://hz.nanxuanxn.top/gtpgpvmtre.html

[S59] C++：静态断言
来源：http://hz.sysykeji.top/gtkurssskw.html

static_assert(sizeof(int) == 4, "int 必须 4 字节");
来源：http://hz.jyoumei.cn/gtsefzlkvp.html

[S60] C++：遍历并删除元素
来源：http://hz.hywenlv.cn/gtxlvssyrl.html

v.erase(std::remove_if(v.begin(), v.end(), [](int x) { return x < 0; }), v.end());
来源：http://hz.yuxming.cn/gtqyujnfku.html

================================================================================
来源：http://hz.bjfxy.top/gtxmvxhnfq.html

T. 其他语言补充（Kotlin / Swift / Lua / Perl / Scala）
来源：http://hz.wangshuangyany.cn/gtjgqocmun.html

================================================================================
来源：http://hz.chenzaomai.com/gtlpcmdedc.html

[T01] Kotlin：Hello World
来源：http://hz.mhx1999.top/gtkbxxaixu.html

println("Hello")
来源：http://hz.shuidangran.top/gteglpgqkl.html

[T02] Kotlin：变量
来源：http://hz.zdqjudy.top/gtqbnzqnvf.html

val a = 1;  var b = 2        // val 只读，var 可变
来源：http://hz.chenjidiqi.icu/gtdocujxjq.html

[T03] Kotlin：字符串模板
来源：http://hz.havefunace.top/gtsdonuhgb.html

"值: $b"
来源：http://hz.quarkkingdee.top/gtglbjrtsn.html

[T04] Kotlin：空安全
来源：http://hz.gotoacloud.top/gtkcvcnlao.html

val n: String? = null;  n?.length
来源：http://hz.redwolf501.top/gtbeqlitzq.html

[T05] Kotlin：when 表达式
来源：http://hz.shanyushiyangkeji.top/gtatxadgzo.html

val s = when (x) { 1 -> "一" else -> "其他" }   // 多分支时每个分支单独一行
来源：http://hz.chenjidiqi.icu/gtqsovncjp.html

[T06] Kotlin：集合映射
来源：http://hz.gogol.net.cn/gtqpyjvour.html

listOf(1, 2, 3).map { it * 2 }
来源：http://hz.pengpengdd.cyou/gtpsjzxmey.html

[T07] Kotlin：集合过滤
来源：http://hz.jiagoushi.top/gtvcxhasrj.html

listOf(1, 2, 3).filter { it > 1 }
来源：http://hz.xylfe.cn/gtspfljhkp.html

[T08] Kotlin：数据类
来源：http://hz.zycfv.cn/gtyzelford.html

data class User(val name: String, val age: Int)
来源：http://hz.cqqwz.cn/gtfeszgsqe.html

[T09] Kotlin：扩展函数
来源：http://hz.iojbl.cn/gtjtdgqscq.html

fun String.exclaim() = this + "!"
来源：http://hz.zhixingplan.top/gtfinmfnlr.html

[T10] Kotlin：默认参数
来源：http://hz.yj20258.top/gtgdjrktwi.html

fun greet(name: String = "World") = "Hi $name"
来源：http://hz.jinghuilouyu.cn/gthyxdifme.html

[T11] Kotlin：协程
来源：http://hz.ydzc1.top/gtyubznlki.html

GlobalScope.launch { delay(1000); println("done") }
来源：http://hz.zhengqikj.top/gtfuhrjjor.html

[T12] Kotlin：解构声明
来源：http://hz.andypj.xyz/gtukcsvotd.html

val (a, b) = Pair(1, 2)
来源：http://hz.havefunace.top/gtideirdbb.html

[T13] Kotlin：只读 Map
来源：http://hz.nanxuanxn.top/gtczicgaol.html

val m = mapOf("a" to 1)
来源：http://hz.yangfankeji.com/gtqhzvooyg.html

[T14] Kotlin：循环
来源：http://hz.jqgfzy.top/gtlvlhroti.html

for (i in 1..10) println(i)
来源：http://hz.dianchejie.cn/gtkacnsnqy.html

[T15] Kotlin：接口
来源：http://hz.hnqzz.top/gtqyrboisn.html

interface Shape { fun area(): Double }
来源：http://hz.sufxvd.cn/gtrfrqgxmc.html

[T16] Swift：Hello World
来源：http://hz.hammf.cn/gtmopqznez.html

print("Hello")
来源：http://hz.cqqwz.cn/gtmgaojukw.html

[T17] Swift：变量与常量
来源：http://hz.hywenlv.cn/gtncvofetg.html

var a = 1;  let b = 2
来源：http://hz.daria6918.cn/gthlpewtwv.html

[T18] Swift：字符串插值
来源：http://hz.zhengqikj.top/gtpybmmyck.html

"值: \(b)"
来源：http://hz.yonumen.top/gtkkrlplob.html

[T19] Swift：可选绑定
来源：http://hz.svipenyu.cn/gtrgiijxrf.html

if let n = opt { print(n) }
来源：http://hz.0kj1m.cn/gtjiymkvva.html

[T20] Swift：数组操作
来源：http://hz.zhengqikj.top/gthgsswpyn.html

var a = [1, 2, 3];  a.append(4)
来源：http://hz.ivvv.top/gtqyirslvx.html

[T21] Swift：遍历
来源：http://hz.snrcjt.cn/gtmpuxtloj.html

for x in a { print(x) }
来源：http://hz.yuxming.cn/gtgjdetxsi.html

[T22] Swift：字典
来源：http://hz.zdqjudy.top/gthqskatou.html

var d = ["a": 1];  d["b"] = 2
来源：http://hz.jqgufenzy.top/gtbvesufpc.html

[T23] Swift：函数
来源：http://hz.nanxinkj.top/gtrijbxltc.html

func add(_ a: Int, _ b: Int) -> Int { a + b }
来源：http://hz.mhx1999.top/gtjmowalfw.html

[T24] Swift：闭包
来源：http://hz.c1oappe.top/gtlzbycfrr.html

let f = { (x: Int) -> Int in x * 2 }
来源：http://hz.yangfankeji.com/gtfkjjuvmu.html

[T25] Swift：结构体
来源：http://hz.jinyuanbaomall.cn/gtfuzkdkal.html

struct P { var x: Int }
来源：http://hz.feifeiyinyue.top/gtwxlouumx.html

[T26] Swift：类与重写
来源：http://hz.xylfe.cn/gtiyuwisjs.html

class A: Base { override func f() {} }
来源：http://hz.daxiang520.top/gtdhgozxcs.html

[T27] Swift：错误处理
来源：http://hz.hnxiangtu.top/gtfzpasboe.html

do { try f() } catch { print(error) }
来源：http://hz.gaohongyu789.top/gtqcrrrmhj.html

[T28] Swift：枚举
来源：http://hz.guowangkeji.top/gtywqyyzpv.html

enum Color { case red, green }
来源：http://hz.tanke756.top/gtsvomuhts.html

[T29] Swift：guard 提前返回
来源：http://hz.yanxiufei.cn/gtevceexty.html

guard let x = opt else { return }
来源：http://hz.nwbrower.top/gtklvlbdjo.html

[T30] Swift：协议
来源：http://hz.sweek.top/gtkcqaodwe.html

protocol Shape { func area() -> Double }
来源：http://hz.nanxinkj.top/gtraanpmge.html

[T31] Lua：Hello World
来源：http://hz.snrcjt.cn/gtxheimgrv.html

print("Hello")
来源：http://hz.bjfxy.top/gtlutedpzo.html

[T32] Lua：局部变量
来源：http://hz.zhoulong.xyz/gtlkdvyfoa.html

local a = 1
来源：http://hz.jiagoushi.top/gthkqocemd.html

[T33] Lua：表（数组）
来源：http://hz.jyoumei.cn/gtncpecmfj.html

local t = {1, 2, 3};  t[4] = 4
来源：http://hz.yangfankeji.com/gtmsmzprgb.html

[T34] Lua：遍历表
来源：http://hz.ivvv.top/gtmhzasyzx.html

for i, v in ipairs(t) do print(i, v) end
来源：http://hz.daxiang520.top/gtduzdenmk.html

[T35] Lua：字典表
来源：http://hz.dianchejie.cn/gtbzjgysip.html

local d = { a = 1 };  d.b = 2
来源：http://hz.yvedp.cn/gtxrratrie.html

[T36] Lua：函数
来源：http://hz.pycfn.com/gtkrfkwrzp.html

function add(a, b) return a + b end
来源：http://hz.yangfankeji.com/gtcdmhxxkd.html

[T37] Lua：字符串拼接
来源：http://hz.chenjidiqi.icu/gtcmiuyvqj.html

"a" .. "b"
来源：http://hz.yj20258888.top/gtbxkergej.html

[T38] Lua：条件
来源：http://hz.yj202588.top/gtxixzflgo.html

if x > 0 then print("正") end
来源：http://hz.nanxuanxn.top/gtocjflurp.html

[T39] Lua：模式匹配
来源：http://hz.nanxinkj.top/gttgtzgxyo.html

string.find(s, "%d+")
来源：http://hz.gaohongyu789.top/gtktqjsgjs.html

[T40] Lua：元表
来源：http://hz.haohaochexian.top/gtmhirmybk.html

setmetatable({}, { __index = base })
来源：http://hz.wangshuangyany.cn/gtbctcnxpe.html

[T41] Perl：Hello World
来源：http://hz.hnxiangtu.top/gtdtpejmgt.html

print "Hello\n";
来源：http://hz.shanyushiyangtech.top/gtidwajxox.html

[T42] Perl：变量类型
来源：http://hz.zhengqikj.top/gtdrjvedwa.html

my $a = 1;  my @arr = (1, 2, 3);  my %h = (a => 1);
来源：http://hz.dashuyun.cn/gtnolgorvq.html

[T43] Perl：字符串插值
来源：http://hz.zhengqikj.top/gtolfvbiun.html

"值: $a"
来源：http://hz.tianlin.xyz/gtjwmepggh.html

[T44] Perl：条件
来源：http://hz.smart0.xyz/gtfqjjwbrj.html

if ($a > 0) { print "正"; }
来源：http://hz.aizwys.cn/gtxkgsftbi.html

[T45] Perl：数组遍历
来源：http://hz.52xcode.cn/gtsikgusgc.html

for my $x (@arr) { print $x; }
来源：http://hz.sufxvd.cn/gtehmfayrl.html

[T46] Perl：哈希操作
来源：http://hz.gaohongyu789.top/gtnrkomkxw.html

$h{b} = 2;  for my $k (keys %h) { print "$k=$h{$k}"; }
来源：http://hz.hammf.cn/gthefvccji.html

[T47] Perl：正则捕获
来源：http://hz.cqqwz.cn/gtcxckipwx.html

if ($s =~ /(\d+)/) { print $1; }
来源：http://hz.jinqigufen.top/gtdgtvztuz.html

[T48] Perl：正则替换
来源：http://hz.sweek.top/gtelutuhcz.html

$s =~ s/old/new/g;
来源：http://hz.yueranfly.top/gtkmnfnynx.html

[T49] Perl：函数
来源：http://hz.0kj1m.cn/gthhkhectb.html

sub add { my ($a, $b) = @_; return $a + $b; }
来源：http://hz.sweek.top/gtzcdadnlg.html

[T50] Perl：逐行读文件
来源：http://hz.meibo888.top/gtbmfrurra.html

open my $fh, "<", "a.txt" or die $!;
来源：http://hz.ybcxt.top/gtpmrktrfj.html

while (my $line = <$fh>) { print $line; }
来源：http://hz.guannengcc.top/gtpdstukdv.html

[T51] Scala：Hello World
来源：http://hz.ydjk.org.cn/gtzkxojgcb.html

println("Hello")
来源：http://hz.hongshengwenyu.top/gtqoexvfnw.html

[T52] Scala：变量
来源：http://hz.c1oappe.top/gtifxttxbq.html

val a = 1;  var b = 2
来源：http://hz.sweek.top/gtdpipgzxq.html

[T53] Scala：字符串插值
来源：http://hz.xuetiantiany.cn/gtndqjsxxf.html

s"值: $b"
来源：http://hz.haohaochexian.top/gtjqfxqusw.html

[T54] Scala：集合映射
来源：http://hz.xinyue.icu/gtbzglwbqs.html

List(1, 2, 3).map(_ * 2)
来源：http://hz.xingfuxueyuan.xyz/gtlcksueje.html

[T55] Scala：集合过滤
来源：http://hz.zhoulong.xyz/gtcccqhexk.html

List(1, 2, 3).filter(_ > 1)
来源：http://hz.shanyushiyangkeji.top/gtsbnuytjd.html

[T56] Scala：样例类
来源：http://hz.jqgufenzy.top/gtfihybdpo.html

case class User(name: String, age: Int)
来源：http://hz.hywenlv.cn/gtkewbdryv.html

[T57] Scala：模式匹配
来源：http://hz.xuanzx.com/gtgosindcr.html

x match { case 1 => "一"; case _ => "其他" }
来源：http://hz.zhoulong.xyz/gtuncthzut.html

[T58] Scala：函数定义
来源：http://hz.cheryme.top/gtwvrfxkbp.html

def add(a: Int, b: Int): Int = a + b
来源：http://hz.yonumen.top/gtfoowjnjw.html

[T59] Scala：循环
来源：http://hz.vqdsnc.cn/gtempjxydw.html

for (i <- 1 to 10) println(i)
来源：http://hz.vqdsnc.cn/gtfeevssfq.html

[T60] Scala：折叠
来源：http://hz.zhijiandao.cn/gtdhmrfouy.html

List(1, 2, 3).foldLeft(0)(_ + _)
来源：http://hz.jinghuilouyu.cn/gtqbtnmbzj.html

================================================================================
来源：http://hz.sufxvd.cn/gtlwjpunto.html

U. 高频实用片段（Python / PHP / JavaScript 各 40 条）
来源：http://hz.jlsjyb.cn/gtawyobqan.html

================================================================================
来源：http://hz.mhx1999.top/gtxjrqhovt.html

[U01] Py：创建虚拟环境
来源：http://hz.jlsjyb.cn/gtunnguhih.html

python -m venv .venv && source .venv/bin/activate
来源：http://hz.jiagoushi.top/gttbbjtilv.html

[U02] Py：导出 / 安装依赖
来源：http://hz.xylfe.cn/gtuvpqotfq.html

pip freeze > requirements.txt;  pip install -r requirements.txt
来源：http://hz.jinqigufen.top/gtlaehjkcv.html

[U03] Py：加载 .env 配置
来源：http://hz.jyoumei.cn/gtuqeueoif.html

from dotenv import load_dotenv; load_dotenv()
来源：http://hz.tanke756.top/gtogsolvga.html

[U04] Py：变量调试打印
来源：http://hz.sysykeji.top/gtanvunqzr.html

print(f"{x=}")            # 输出 x=值，Python 3.8+
来源：http://hz.cashguo.top/gtlpxjptpk.html

[U05] Py：列表去重且保序
来源：http://hz.cheryme.top/gtxaryuamy.html

list(dict.fromkeys(arr))
来源：http://hz.sysykeji.top/gtzohprzdp.html

[U06] Py：合并两个字典
来源：http://hz.jinqigfzy.top/gtpluesded.html

{**a, **b}
来源：http://hz.haohaochexian.top/gtwzaqcavm.html

[U07] Py：反转字典键值
来源：http://hz.zhongyouzk.top/gtyvkvmmzp.html

{v: k for k, v in d.items()}
来源：http://hz.yuanzhike.top/gtvnfwxmvc.html

[U08] Py：展平二维列表
来源：http://hz.ehwqpu.com/gtddhkmagl.html

[y for x in nested for y in x]
来源：http://hz.jqgfzy.top/gtjgjyivhq.html

[U09] Py：字典取最大值的键
来源：http://hz.zhiwuduotai.top/gtjnwrquic.html

max(d, key=d.get)
来源：http://hz.yanxiufei.cn/gtvvvxdgtk.html

[U10] Py：按值排序字典
来源：http://hz.hysaishi.cn/gtgdkismrg.html

dict(sorted(d.items(), key=lambda kv: kv[1]))
来源：http://hz.vqdsnc.cn/gtdgnxxlan.html

[U11] Py：生成器表达式
来源：http://hz.hysaishi.cn/gtozhvedyu.html

(x * 2 for x in arr)
来源：http://hz.feifeiyinyue.top/gtkhvwdasc.html

[U12] Py：取出现最多的 3 个元素
来源：http://hz.wangdashe.top/gtdmponxuv.html

Counter(arr).most_common(3)
来源：http://hz.yangfankeji.com/gtgypsjdvz.html

[U13] Py：固定长度队列
来源：http://hz.feifeiyinyue.top/gtfxpyzqtq.html

deque(maxlen=10)
来源：http://hz.pengpengdd.cyou/gthgizyixx.html

[U14] Py：分组收集到列表
来源：http://hz.wangdashe.top/gtkbqvlioy.html

defaultdict(list)
来源：http://hz.fzhhl.top/gtnvrknnra.html

[U15] Py：高精度计时
来源：http://hz.yj20258.top/gtgikgqxnz.html

t = time.perf_counter()
来源：http://hz.zhengqikj.top/gtvnqjeyzy.html

[U16] Py：命令行参数解析
来源：http://hz.nanxinkj.top/gtyarqfupo.html

ap = argparse.ArgumentParser();  ap.add_argument("--name");  args = ap.parse_args()
来源：http://hz.pengpengdd.cyou/gtnphlgzjw.html

[U17] Py：初始化日志
来源：http://hz.ehwqpu.com/gtsjdksmsr.html

logging.basicConfig(level=logging.INFO)
来源：http://hz.wangshuangyany.cn/gtvwkivbvi.html

[U18] Py：预编译正则
来源：http://hz.yj20258888.top/gthksbyjhz.html

pat = re.compile(r"\d+")
来源：http://hz.yj20258888.top/gtaghwypba.html

[U19] Py：正则替换带回调
来源：http://hz.birdmap.top/gtekwgoikw.html

re.sub(r"\d+", lambda m: str(int(m.group()) * 2), s)
来源：http://hz.snrcjt.cn/gtztcwxccv.html

[U20] Py：缓存函数结果
来源：http://hz.jyoumei.cn/gtfbdpnjmw.html

@functools.lru_cache(maxsize=None)
来源：http://hz.sxryk.cn/gtdbckdkca.html

[U21] Py：自定义上下文管理器
来源：http://hz.xinyue.icu/gtagnmvaft.html

@contextlib.contextmanager
来源：http://hz.gotoacloud.top/gtwxnqruwq.html

[U22] Py：矩阵转置
来源：http://hz.hongshengwenyu.top/gtcuzjgaee.html

list(zip(*m))
来源：http://hz.shzxlz.cn/gtjiqhdubs.html

[U23] Py：分块读取大文件
来源：http://hz.c1oappe.top/gtclwlzlvk.html

for chunk in iter(lambda: f.read(8192), b""):
来源：http://hz.svipenyu.cn/gtlrkozzdw.html

[U24] Py：路径操作
来源：http://hz.hfpthk.cn/gtvugvmmay.html

Path("a/b.txt").parent.mkdir(parents=True, exist_ok=True)
来源：http://hz.nanxinkj.top/gtchgzmdcx.html

[U25] Py：CSV 按字典读
来源：http://hz.yuanzhike.top/gtxdqaexst.html

csv.DictReader(f)
来源：http://hz.sxryk.cn/gtcuvnjipj.html

[U26] Py：并发下载
来源：http://hz.gotoacloud.top/gtppkifwke.html

ThreadPoolExecutor(max_workers=8).map(fetch, urls)
来源：http://hz.yuxming.cn/gtvrlrrvfq.html

[U27] Py：异步 HTTP
来源：http://hz.zhixingplan.top/gtskqmkjwc.html

aiohttp.ClientSession() 配合 async with
来源：http://hz.feifeiyinyue.top/gtoclqjvnj.html

[U28] Py：类型别名
来源：http://hz.zhongyouzk.top/gtccsmoyey.html

UserId = int
来源：http://hz.jiagoushi.top/gtkytniqdd.html

[U29] Py：属性校验
来源：http://hz.jlsjyb.cn/gtvrbbidhk.html

@property 与 @x.setter 配合
来源：http://hz.mhx1999.top/gtjztnuipf.html

[U30] Py：数据类
来源：http://hz.zhoulong.xyz/gtrndabdxe.html

@dataclass(slots=True)
来源：http://hz.zhiwuduotai.top/gtcktrlwev.html

[U31] Py：单测
来源：http://hz.cheryme.top/gtxnbbmzbc.html

python -m pytest -q
来源：http://hz.sufxvd.cn/gtshtzdhcs.html

[U32] Py：代码格式化
来源：http://hz.yuanzhike.top/gtrjxrnnsn.html

ruff format . && ruff check --fix .
来源：http://hz.xuetiantiany.cn/gthfaoanho.html

[U33] Py：打包发布
来源：http://hz.iojbl.cn/gtqaemdwyj.html

python -m build  （依赖 pyproject.toml）
来源：http://hz.dianchejie.cn/gthhgpoemn.html

[U34] Py：判断编码
来源：http://hz.hywenlv.cn/gtgvycpkvd.html

chardet.detect(raw)
来源：http://hz.meibo888.top/gttvtpmpip.html

[U35] Py：发送邮件
来源：http://hz.yuanzhike.top/gtchqejpne.html

smtplib.SMTP_SSL(...).send_message(msg)
来源：http://hz.smart0.xyz/gtzdzaibek.html

[U36] Py：定时任务
来源：http://hz.yj202588.top/gtpifylhfb.html

schedule.every(10).minutes.do(job)
来源：http://hz.yj202588.top/gtsttipusk.html

[U37] Py：读写 Excel
来源：http://hz.cashguo.top/gtapazhqsg.html

pandas.read_excel / DataFrame.to_excel
来源：http://hz.yj202588.top/gtdhbaoylg.html

[U38] Py：获取脚本所在目录
来源：http://hz.pycfn.com/gtkgvtjuay.html

Path(__file__).resolve().parent
来源：http://hz.sweek.top/gtovbuhwwv.html

[U39] Py：判断是否在交互环境
来源：http://hz.nanxinkj.top/gtusburdhk.html

sys.stdout.isatty()
来源：http://hz.chenlongwang.top/gtjnczyhla.html

[U40] Py：打印到标准错误
来源：http://hz.wangdashe.top/gtmzvrmrlr.html

print("err", file=sys.stderr)
来源：http://hz.xziqi.cn/gthtsakxko.html

[U41] PHP：初始化 Composer 项目
来源：http://hz.jqgfzy.top/gtistxjboo.html

composer init;  composer require guzzlehttp/guzzle
来源：http://hz.hysaishi.cn/gtyqojpyjz.html

[U42] PHP：PSR-4 自动加载
来源：http://hz.gaohongyu789.top/gtvpprumxv.html

"autoload": { "psr-4": { "App\\": "src/" } }
来源：http://hz.birdmap.top/gtekqvckzn.html

[U43] PHP：声明命名空间
来源：http://hz.zhongyouzk.top/gtyqbtaalb.html

namespace App\Http;
来源：http://hz.c1oappe.top/gtyajxxgyf.html

[U44] PHP：开启严格类型
来源：http://hz.tianlin.xyz/gtptvrhtoh.html

declare(strict_types=1);
来源：http://hz.c1oappe.top/gttrpquhft.html

[U45] PHP：类型声明与返回类型
来源：http://hz.cdnleiting.top/gtnhbbbkuu.html

function add(int $a, int $b): int { return $a + $b; }
来源：http://hz.jqgfzy.top/gttbtjhcds.html

[U46] PHP：可空类型
来源：http://hz.nanxinkj.top/gtxnlnahxg.html

?string $name = null
来源：http://hz.tian-w.cn/gtggntjlfm.html

[U47] PHP：联合类型
来源：http://hz.hnqzz.top/gtuqssbpjw.html

int|string $id
来源：http://hz.tanke756.top/gtjujwgxwu.html

[U48] PHP：纯枚举
来源：http://hz.zhengqikj.top/gtklelgdsj.html

enum Status: string { case Active = "active"; case Off = "off"; }
来源：http://hz.nanxuanxn.top/gtfbczqlht.html

[U49] PHP：只读属性
来源：http://hz.aibaodan.cn/gtdegkwcyd.html

public readonly string $name
来源：http://hz.gzhubu.top/gtxsfdcazt.html

[U50] PHP：构造器属性提升
来源：http://hz.hysaishi.cn/gtbtllwzfd.html

public function __construct(private int $id) {}
来源：http://hz.nanxinkj.top/gthrrzbbbd.html

[U51] PHP：数组解构
来源：http://hz.tianlin.xyz/gtnwfnrmxx.html

[$a, $b] = $arr;
来源：http://hz.ehwqpu.com/gttfetfuxa.html

[U52] PHP：箭头函数
来源：http://hz.0kj1m.cn/gtpgyccifa.html

$double = fn($x) => $x * 2;
来源：http://hz.ppjwa.cn/gtrmuejxff.html

[U53] PHP：空合并运算符
来源：http://hz.quarkkingdee.top/gtyxejnobs.html

$v = $a ?? $b ?? "default";
来源：http://hz.bjfxy.top/gtwcrrhjdy.html

[U54] PHP：空安全调用
来源：http://hz.ywan-chungtsiang.top/gtpmgftdxt.html

$obj?->method()
来源：http://hz.guowangkeji.top/gtohcbtszr.html

[U55] PHP：match 表达式
来源：http://hz.gogol.net.cn/gtshxnezdh.html

$s = match($x) { 1 => "一", default => "其他" };
来源：http://hz.dianchejie.cn/gtatsyvdxv.html

[U56] PHP：命名参数
来源：http://hz.dianchejie.cn/gtdqfuadbk.html

f(a: 1, b: 2)
来源：http://hz.hnxiangtu.top/gtabbsocdz.html

[U57] PHP：字符串插值
来源：http://hz.cashguo.top/gtuvzqcmml.html

"值: {$a}"
来源：http://hz.hammf.cn/gtpdmitrci.html

[U58] PHP：数组三件套
来源：http://hz.jqgufenzy.top/gtiyavegoh.html

array_map($f, $a);  array_filter($a, $f);  array_reduce($a, $f, 0);
来源：http://hz.havefunace.top/gtvuraflmz.html

[U59] PHP：自定义排序
来源：http://hz.smart0.xyz/gtjkhneqig.html

usort($arr, fn($a, $b) => $a["age"] <=> $b["age"]);
来源：http://hz.cashguo.top/gttmblgthu.html

[U60] PHP：JSON 编解码
来源：http://hz.xinyue.icu/gtoiiweibk.html

json_encode($d, JSON_UNESCAPED_UNICODE);  json_decode($s, true);
来源：http://hz.fengsongda.top/gtcmpccqig.html

[U61] PHP：正则
来源：http://hz.zhoulong.xyz/gtuhxfggvd.html

preg_match('/(\d+)/', $s, $m);  preg_replace('/\d+/', '#', $s);
来源：http://hz.redwolf501.top/gtkwijhxye.html

[U62] PHP：日期对象
来源：http://hz.nanxinkj.top/gtwmveohwi.html

(new DateTimeImmutable())->format("Y-m-d");
来源：http://hz.c1oappe.top/gtljvcyzrs.html

[U63] PHP：文件读写
来源：http://hz.jinqigfzy.top/gtfllrteir.html

file_get_contents($f);  file_put_contents($f, $data);
来源：http://hz.ywan-chungtsiang.top/gtxdzyzysc.html

[U64] PHP：目录遍历
来源：http://hz.gaohongyu789.top/gtpmrhymso.html

glob("dir/*.php");  scandir("dir");
来源：http://hz.feifeiyinyue.top/gtzsnvggyn.html

[U65] PHP：会话
来源：http://hz.andypj.xyz/gtdsdangha.html

session_start();  $_SESSION["uid"] = 1;
来源：http://hz.jiagoushi.top/gtgcagvpgf.html

[U66] PHP：设置 Cookie
来源：http://hz.nanxinkj.top/gteveifvcu.html

setcookie("token", $v, ["httponly" => true, "samesite" => "Lax"]);
来源：http://hz.vqdsnc.cn/gtsnwqtqta.html


<!-- 参考信息 -->