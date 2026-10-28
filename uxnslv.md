代发 wailian999

[S41] C++：类与构造函数
来源：http://hz.smart0.xyz/gtoqmdsunm.html

class A { public: A(int v) : x_(v) {} int get() const { return x_; } private: int x_; };
来源：http://hz.cheryme.top/gtfuliifjx.html

[S42] C++：继承与虚函数
来源：http://hz.ybcxt.top/gtuyzqsadt.html

class B : public Base { public: void f() override {} };
来源：http://hz.hysaishi.cn/gtfbtnxnlg.html

[S43] C++：智能指针
来源：http://hz.pycfn.com/gthompelbq.html

auto p = std::make_unique<int>(5);
来源：http://hz.yuanzhike.top/gtbuzkqtvx.html

[S44] C++：引用传参
来源：http://hz.svipenyu.cn/gtwrovifev.html

void inc(int &x) { ++x; }
来源：http://hz.zhongyouzk.top/gtxorsgzzu.html

[S45] C++：lambda
来源：http://hz.yj20258888.top/gtaubzuoaf.html

auto add = [](int a, int b) { return a + b; };
来源：http://hz.316326.xyz/gtgjdtxlup.html

[S46] C++：函数模板
来源：http://hz.pengpengdd.cyou/gtgfrmffgj.html

template <typename T> T maxv(T a, T b) { return a > b ? a : b; }
来源：http://hz.sxryk.cn/gtynhahscu.html

[S47] C++：结构化绑定遍历
来源：http://hz.yj20258.top/gthceilwmr.html

for (const auto &[k, v] : m) { std::cout << k << v; }
来源：http://hz.kuanghao11.cn/gtzwjbgypc.html

[S48] C++：逐行读文件
来源：http://hz.cheryme.top/gtautgjhcx.html

std::ifstream in("a.txt");  std::string line;
来源：http://hz.jinqigfzy.top/gtwunotcwa.html

while (std::getline(in, line)) { }
来源：http://hz.zycfv.cn/gtidsehxsw.html

[S49] C++：写文件
来源：http://hz.meibo888.top/gtpofuaahz.html

std::ofstream out("a.txt");  out << "hi\n";
来源：http://hz.gotoacloud.top/gtxhreecif.html

[S50] C++：格式化数字
来源：http://hz.ivvv.top/gtklmcssvc.html

std::ostringstream os;  os << std::fixed << std::setprecision(2) << 3.14159;
来源：http://hz.yonumen.top/gtoarbvury.html

[S51] C++：显式类型转换
来源：http://hz.yj20258.top/gtajfzkfze.html

static_cast<double>(a) / b
来源：http://hz.guowangkeji.top/gtbmqebpfg.html

[S52] C++：const 与 noexcept
来源：http://hz.hfpthk.cn/gtospxfzrn.html

int size() const noexcept { return n_; }
来源：http://hz.zhengqikj.top/gtfvsevwva.html

[S53] C++：移动语义
来源：http://hz.hysaishi.cn/gtsthdmpko.html

std::vector<int> w = std::move(v);
来源：http://hz.chenlongwang.top/gtnhlthkci.html

[S54] C++：异常处理
来源：http://hz.shangyingyoupin.top/gtngerkhxc.html

try { throw std::runtime_error("x"); } catch (const std::exception &e) { }
来源：http://hz.zycfv.cn/gtbjgsnhej.html

[S55] C++：结构化绑定
来源：http://hz.nwbrower.top/gtonguilti.html

auto [a, b] = std::make_pair(1, 2);
来源：http://hz.jiagoushi.top/gtgspjbjpe.html

[S56] C++：optional
来源：http://hz.cucudq.cn/gtxfbvfmsi.html

std::optional<int> o = 5;  if (o) { int v = *o; }
来源：http://hz.wangshuangyany.cn/gtycfnsaay.html

[S57] C++：编译期常量
来源：http://hz.yj20258888.top/gtdlpetatg.html

constexpr int N = 10;
来源：http://hz.hywenlv.cn/gtnbgmnsuo.html

[S58] C++：命名空间
来源：http://hz.fzhhl.top/gtjvhrynbb.html

namespace ns { int f() { return 1; } }
来源：http://hz.yuxming.cn/gtsjiwtqgn.html

[S59] C++：静态断言
来源：http://hz.yuxming.cn/gtwkhrvdgw.html

static_assert(sizeof(int) == 4, "int 必须 4 字节");
来源：http://hz.dianchejie.cn/gtfwrpyhde.html

[S60] C++：遍历并删除元素
来源：http://hz.havefunace.top/gtxxctidqn.html

v.erase(std::remove_if(v.begin(), v.end(), [](int x) { return x < 0; }), v.end());
来源：http://hz.svipenyu.cn/gtwdhcdsqg.html

================================================================================
来源：http://hz.quarkkingdee.top/gtyplevopk.html

T. 其他语言补充（Kotlin / Swift / Lua / Perl / Scala）
来源：http://hz.sxryk.cn/gttzyafwxx.html

================================================================================
来源：http://hz.zhaomingkeji.xyz/gtsffvxbng.html

[T01] Kotlin：Hello World
来源：http://hz.xuetiantiany.cn/gtwosftxzx.html

println("Hello")
来源：http://hz.jianghu66.top/gtlfvnuuwk.html

[T02] Kotlin：变量
来源：http://hz.cqqwz.cn/gtcqklzfmo.html

val a = 1;  var b = 2        // val 只读，var 可变
来源：http://hz.sweek.top/gtvinrkmuu.html

[T03] Kotlin：字符串模板
来源：http://hz.shangyingyoupin.top/gtpestvoet.html

"值: $b"
来源：http://hz.ybcxt.top/gtdqhikaqp.html

[T04] Kotlin：空安全
来源：http://hz.zdqjudy.top/gtonkgffgl.html

val n: String? = null;  n?.length
来源：http://hz.zdqjudy.top/gtvstcyjwv.html

[T05] Kotlin：when 表达式
来源：http://hz.ydzc1.top/gtlbgraxgw.html

val s = when (x) { 1 -> "一" else -> "其他" }   // 多分支时每个分支单独一行
来源：http://hz.kuanghao11.cn/gtvauozgwn.html

[T06] Kotlin：集合映射
来源：http://hz.jinyuanbaomall.cn/gtcqyrvkej.html

listOf(1, 2, 3).map { it * 2 }
来源：http://hz.guannengcc.top/gtvokfzwhu.html

[T07] Kotlin：集合过滤
来源：http://hz.xingfuxueyuan.xyz/gtmxsuwkkm.html

listOf(1, 2, 3).filter { it > 1 }
来源：http://hz.ehwqpu.com/gtcvuzrwwz.html

[T08] Kotlin：数据类
来源：http://hz.gotoacloud.top/gtaazjjktb.html

data class User(val name: String, val age: Int)
来源：http://hz.ehwqpu.com/gtjwoopkpb.html

[T09] Kotlin：扩展函数
来源：http://hz.yonumen.top/gtitjjzayq.html

fun String.exclaim() = this + "!"
来源：http://hz.wangshuangyany.cn/gtrsttvdxr.html

[T10] Kotlin：默认参数
来源：http://hz.cdnleiting.top/gtbztokvgg.html

fun greet(name: String = "World") = "Hi $name"
来源：http://hz.hnqzz.top/gthglqrehy.html

[T11] Kotlin：协程
来源：http://hz.vqdsnc.cn/gtdzmgqwfu.html

GlobalScope.launch { delay(1000); println("done") }
来源：http://hz.jinyuanbaomall.cn/gtknjigzrh.html

[T12] Kotlin：解构声明
来源：http://hz.xingfuxueyuan.xyz/gtbxcowedk.html

val (a, b) = Pair(1, 2)
来源：http://hz.aizwys.cn/gtslsmcgns.html

[T13] Kotlin：只读 Map
来源：http://hz.daxiang520.top/gtxxjcylpt.html

val m = mapOf("a" to 1)
来源：http://hz.pengpengdd.cyou/gtjpqkhyih.html

[T14] Kotlin：循环
来源：http://hz.mhx1999.top/gtcvkchvcz.html

for (i in 1..10) println(i)
来源：http://hz.fzhhl.top/gtbodutwhg.html

[T15] Kotlin：接口
来源：http://hz.xuanzx.com/gtnulpogct.html

interface Shape { fun area(): Double }
来源：http://hz.jinqigfzy.top/gtcztfzukj.html

[T16] Swift：Hello World
来源：http://hz.yueranfly.top/gtsjtktgkd.html

print("Hello")
来源：http://hz.yueranfly.top/gtgnggluus.html

[T17] Swift：变量与常量
来源：http://hz.zhengqikj.top/gtvvmfkyok.html

var a = 1;  let b = 2
来源：http://hz.zhiwuduotai.top/gtkjqhecvv.html

[T18] Swift：字符串插值
来源：http://hz.jianghu66.top/gtgekqubxf.html

"值: \(b)"
来源：http://hz.hammf.cn/gtbjdqqzxs.html

[T19] Swift：可选绑定
来源：http://hz.ydzc1.top/gtzqnxbivp.html

if let n = opt { print(n) }
来源：http://hz.xinyue.icu/gtnwpcwouk.html

[T20] Swift：数组操作
来源：http://hz.sysykeji.top/gtlqxlublj.html

var a = [1, 2, 3];  a.append(4)
来源：http://hz.dianchejie.cn/gtijqjidlc.html

[T21] Swift：遍历
来源：http://hz.dashuyun.cn/gtnypsxscj.html

for x in a { print(x) }
来源：http://hz.jlsjyb.cn/gtdvxmukvz.html

[T22] Swift：字典
来源：http://hz.cdnleiting.top/gtacllprnl.html

var d = ["a": 1];  d["b"] = 2
来源：http://hz.dianchejie.cn/gtqoafewlo.html

[T23] Swift：函数
来源：http://hz.jinqigufen.top/gtktxmuiop.html

func add(_ a: Int, _ b: Int) -> Int { a + b }
来源：http://hz.jianghu66.top/gttkzqsgtx.html

[T24] Swift：闭包
来源：http://hz.sysykeji.top/gtdbiibvee.html

let f = { (x: Int) -> Int in x * 2 }
来源：http://hz.yj20258888.top/gtcgxnhiku.html

[T25] Swift：结构体
来源：http://hz.hfpthk.cn/gtfpffpoah.html

struct P { var x: Int }
来源：http://hz.xingfuxueyuan.xyz/gtvkzzzkcm.html

[T26] Swift：类与重写
来源：http://hz.svipenyu.cn/gtxmjkrsvy.html

class A: Base { override func f() {} }
来源：http://hz.nanxuanxn.top/gtyxaamjmk.html

[T27] Swift：错误处理
来源：http://hz.jqgfzy.top/gtlcaraecl.html

do { try f() } catch { print(error) }
来源：http://hz.yangfankeji.com/gtnnmkznow.html

[T28] Swift：枚举
来源：http://hz.nwbrower.top/gtdtuweemg.html

enum Color { case red, green }
来源：http://hz.zhengqikj.top/gtinorvzwt.html

[T29] Swift：guard 提前返回
来源：http://hz.sxryk.cn/gtcopmqydd.html

guard let x = opt else { return }
来源：http://hz.cucudq.cn/gtstrzjine.html

[T30] Swift：协议
来源：http://hz.daria6918.cn/gtxgyoxzrq.html

protocol Shape { func area() -> Double }
来源：http://hz.xuanzx.com/gtmewcpqnk.html

[T31] Lua：Hello World
来源：http://hz.shangyingyoupin.top/gtfkwzdhyh.html

print("Hello")
来源：http://hz.ivvv.top/gtxzlsqajy.html

[T32] Lua：局部变量
来源：http://hz.ivvv.top/gtbgyclpxs.html

local a = 1
来源：http://hz.wangdashe.top/gtqpzxekmx.html

[T33] Lua：表（数组）
来源：http://hz.ydjk.org.cn/gtjrulllvv.html

local t = {1, 2, 3};  t[4] = 4
来源：http://hz.guowangkeji.top/gtluxqhcyc.html

[T34] Lua：遍历表
来源：http://hz.jinghuilouyu.cn/gtddrmaugb.html

for i, v in ipairs(t) do print(i, v) end
来源：http://hz.cashguo.top/gtffjberfv.html

[T35] Lua：字典表
来源：http://hz.hfpthk.cn/gtydiutjip.html

local d = { a = 1 };  d.b = 2
来源：http://hz.gzhubu.top/gtvopkzwck.html

[T36] Lua：函数
来源：http://hz.wangshuangyany.cn/gthbmzgucd.html

function add(a, b) return a + b end
来源：http://hz.ydzc1.top/gtqrdzvnnf.html

[T37] Lua：字符串拼接
来源：http://hz.yvedp.cn/gtxcndadaw.html

"a" .. "b"
来源：http://hz.yuxming.cn/gtrwrfpxtc.html

[T38] Lua：条件
来源：http://hz.iojbl.cn/gtjjgpeovj.html

if x > 0 then print("正") end
来源：http://hz.chenzaomai.com/gtzxkylcpo.html

[T39] Lua：模式匹配
来源：http://hz.ydzc1.top/gtxnodvkzw.html

string.find(s, "%d+")
来源：http://hz.daxiang520.top/gthzfgrmbx.html

[T40] Lua：元表
来源：http://hz.tian-w.cn/gtcbmdhdxg.html

setmetatable({}, { __index = base })
来源：http://hz.jinqigfzy.top/gtcmlgdxkt.html

[T41] Perl：Hello World
来源：http://hz.aizwys.cn/gtfiozoahi.html

print "Hello\n";
来源：http://hz.hnxiangtu.top/gtfyaojyqr.html

[T42] Perl：变量类型
来源：http://hz.ppjwa.cn/gtbadoyxnc.html

my $a = 1;  my @arr = (1, 2, 3);  my %h = (a => 1);
来源：http://hz.52xcode.cn/gtivimfywe.html

[T43] Perl：字符串插值
来源：http://hz.xziqi.cn/gtxcqukjqe.html

"值: $a"
来源：http://hz.jinqigufen.top/gtnuxtofke.html

[T44] Perl：条件
来源：http://hz.birdmap.top/gtrjewfmet.html

if ($a > 0) { print "正"; }
来源：http://hz.ywan-chungtsiang.top/gtngvpnrvt.html

[T45] Perl：数组遍历
来源：http://hz.yj20258888.top/gtzfdmdars.html

for my $x (@arr) { print $x; }
来源：http://hz.cashguo.top/gtewzzajqq.html

[T46] Perl：哈希操作
来源：http://hz.haohaochexian.top/gtibljdxmm.html

$h{b} = 2;  for my $k (keys %h) { print "$k=$h{$k}"; }
来源：http://hz.sysykeji.top/gticbeknkd.html

[T47] Perl：正则捕获
来源：http://hz.jiagoushi.top/gtnohtnmqa.html

if ($s =~ /(\d+)/) { print $1; }
来源：http://hz.yvedp.cn/gtdzgzwfzc.html

[T48] Perl：正则替换
来源：http://hz.yangfankeji.com/gtqvhmjroy.html

$s =~ s/old/new/g;
来源：http://hz.zhongyouzk.top/gtewlwzcbh.html

[T49] Perl：函数
来源：http://hz.yj202588.top/gtuukyawat.html

sub add { my ($a, $b) = @_; return $a + $b; }
来源：http://hz.hywenlv.cn/gtwjwbotgd.html

[T50] Perl：逐行读文件
来源：http://hz.cheryme.top/gtokwwwtbz.html

open my $fh, "<", "a.txt" or die $!;
来源：http://hz.cheryme.top/gtzzrungsz.html

while (my $line = <$fh>) { print $line; }
来源：http://hz.hfpthk.cn/gtstbzjjsv.html

[T51] Scala：Hello World
来源：http://hz.tanke756.top/gtcpvneudo.html

println("Hello")
来源：http://hz.aizwys.cn/gtonprugmo.html

[T52] Scala：变量
来源：http://hz.pengpengdd.cyou/gtqopwptdb.html

val a = 1;  var b = 2
来源：http://hz.zhoulong.xyz/gtgosgmwgm.html

[T53] Scala：字符串插值
来源：http://hz.zhongyouzk.top/gtublmmfxi.html

s"值: $b"
来源：http://hz.havefunace.top/gtwnbsweqd.html

[T54] Scala：集合映射
来源：http://hz.zhongyouzk.top/gtaytxtkre.html

List(1, 2, 3).map(_ * 2)
来源：http://hz.hywenlv.cn/gttoymtopf.html

[T55] Scala：集合过滤
来源：http://hz.316326.xyz/gtzodxhiov.html

List(1, 2, 3).filter(_ > 1)
来源：http://hz.zhoulong.xyz/gthlzrpird.html

[T56] Scala：样例类
来源：http://hz.cheryme.top/gttporuofk.html

case class User(name: String, age: Int)
来源：http://hz.sxryk.cn/gtwyzupbkg.html

[T57] Scala：模式匹配
来源：http://hz.jinqigufen.top/gtwclkerlz.html

x match { case 1 => "一"; case _ => "其他" }
来源：http://hz.nwbrower.top/gtnlcvkzsm.html

[T58] Scala：函数定义
来源：http://hz.jyoumei.cn/gtrozyeink.html

def add(a: Int, b: Int): Int = a + b
来源：http://hz.jlsjyb.cn/gtiafwmbvd.html

[T59] Scala：循环
来源：http://hz.zycfv.cn/gtmgaomygc.html

for (i <- 1 to 10) println(i)
来源：http://hz.tianlin.xyz/gtyyfxolwk.html

[T60] Scala：折叠
来源：http://hz.hywenlv.cn/gtuadzyhjm.html

List(1, 2, 3).foldLeft(0)(_ + _)
来源：http://hz.dashuyun.cn/gtrsvjikpf.html

================================================================================
来源：http://hz.feifeiyinyue.top/gturhqaogr.html

U. 高频实用片段（Python / PHP / JavaScript 各 40 条）
来源：http://hz.gogol.net.cn/gtrkdwetkp.html

================================================================================
来源：http://hz.nanxuanxn.top/gtglhdhakx.html

[U01] Py：创建虚拟环境
来源：http://hz.316326.xyz/gtuxpdgdur.html

python -m venv .venv && source .venv/bin/activate
来源：http://hz.9152youxi.cn/gtaogqszqx.html

[U02] Py：导出 / 安装依赖
来源：http://hz.fzhhl.top/gtlgdcngvk.html

pip freeze > requirements.txt;  pip install -r requirements.txt
来源：http://hz.wangdashe.top/gtqkcugkar.html

[U03] Py：加载 .env 配置
来源：http://hz.yonumen.top/gthsaqjunk.html

from dotenv import load_dotenv; load_dotenv()
来源：http://hz.quarkkingdee.top/gthvkjmnud.html

[U04] Py：变量调试打印
来源：http://hz.aibaodan.cn/gttilqtfur.html

print(f"{x=}")            # 输出 x=值，Python 3.8+
来源：http://hz.hywenlv.cn/gtznomtxgf.html

[U05] Py：列表去重且保序
来源：http://hz.havefunace.top/gtdpqrqssr.html

list(dict.fromkeys(arr))
来源：http://hz.jqgufenzy.top/gtmlhsmkqc.html

[U06] Py：合并两个字典
来源：http://hz.sysykeji.top/gtnquhptfb.html

{**a, **b}
来源：http://hz.haohaochexian.top/gtvwlgakgw.html

[U07] Py：反转字典键值
来源：http://hz.gaohongyu789.top/gtwimlbjgx.html

{v: k for k, v in d.items()}
来源：http://hz.snrcjt.cn/gtnxijvcul.html

[U08] Py：展平二维列表
来源：http://hz.guannengcc.top/gtmytckdxh.html

[y for x in nested for y in x]
来源：http://hz.52xcode.cn/gttulqerpi.html

[U09] Py：字典取最大值的键
来源：http://hz.sxryk.cn/gtbhcihaxo.html

max(d, key=d.get)
来源：http://hz.nanxinkj.top/gtygdqhaff.html

[U10] Py：按值排序字典
来源：http://hz.wangdashe.top/gtwmwvasqe.html

dict(sorted(d.items(), key=lambda kv: kv[1]))
来源：http://hz.ppjwa.cn/gthrxqjvda.html

[U11] Py：生成器表达式
来源：http://hz.nanxinkj.top/gtitjpbwev.html

(x * 2 for x in arr)
来源：http://hz.feifeiyinyue.top/gtovfxqyfz.html

[U12] Py：取出现最多的 3 个元素
来源：http://hz.hfpthk.cn/gtuceojkai.html

Counter(arr).most_common(3)
来源：http://hz.chenjidiqi.icu/gthkfprtba.html

[U13] Py：固定长度队列
来源：http://hz.xuetiantiany.cn/gtxqskanpo.html

deque(maxlen=10)
来源：http://hz.cucudq.cn/gtuxnsoqeo.html

[U14] Py：分组收集到列表
来源：http://hz.yj202588.top/gtcxmynmoo.html

defaultdict(list)
来源：http://hz.zhengqikj.top/gtjpthbmmu.html

[U15] Py：高精度计时
来源：http://hz.jinqigufen.top/gtjlvlpclt.html

t = time.perf_counter()
来源：http://hz.sxryk.cn/gtyiapsqos.html

[U16] Py：命令行参数解析
来源：http://hz.hysaishi.cn/gtdnwppeyt.html

ap = argparse.ArgumentParser();  ap.add_argument("--name");  args = ap.parse_args()
来源：http://hz.nanxinkj.top/gtvfmpndcg.html

[U17] Py：初始化日志
来源：http://hz.52xcode.cn/gtjzediwho.html

logging.basicConfig(level=logging.INFO)
来源：http://hz.nanxinkj.top/gthjbjmotl.html

[U18] Py：预编译正则
来源：http://hz.daria6918.cn/gtrqwxkyzh.html

pat = re.compile(r"\d+")
来源：http://hz.shanyushiyangtech.top/gtklkedjqs.html

[U19] Py：正则替换带回调
来源：http://hz.vqdsnc.cn/gtckulpkoc.html

re.sub(r"\d+", lambda m: str(int(m.group()) * 2), s)
来源：http://hz.chenjidiqi.icu/gtynwiflnt.html

[U20] Py：缓存函数结果
来源：http://hz.xuanzx.com/gtsclebmnd.html

@functools.lru_cache(maxsize=None)
来源：http://hz.c1oappe.top/gtjzncmato.html

[U21] Py：自定义上下文管理器
来源：http://hz.yuxming.cn/gtejfyuizg.html

@contextlib.contextmanager
来源：http://hz.chenzaomai.com/gtcmenxsac.html

[U22] Py：矩阵转置
来源：http://hz.kuanghao11.cn/gtyrlsweln.html

list(zip(*m))
来源：http://hz.haohaochexian.top/gtxegiemlt.html

[U23] Py：分块读取大文件
来源：http://hz.316326.xyz/gtcozpcjwa.html

for chunk in iter(lambda: f.read(8192), b""):
来源：http://hz.c1oappe.top/gtobmnlcid.html

[U24] Py：路径操作
来源：http://hz.birdmap.top/gtfpujhjul.html

Path("a/b.txt").parent.mkdir(parents=True, exist_ok=True)
来源：http://hz.hnxiangtu.top/gtjcgdfzfg.html

[U25] Py：CSV 按字典读
来源：http://hz.guannengcc.top/gtwbzhjxwl.html

csv.DictReader(f)
来源：http://hz.haohaochexian.top/gtfqgnwmxf.html

[U26] Py：并发下载
来源：http://hz.andypj.xyz/gtchtftwmb.html

ThreadPoolExecutor(max_workers=8).map(fetch, urls)
来源：http://hz.sysykeji.top/gtoyqgxxsk.html

[U27] Py：异步 HTTP
来源：http://hz.aibaodan.cn/gtyllwvwjp.html

aiohttp.ClientSession() 配合 async with
来源：http://hz.yonumen.top/gtlvhwdvfa.html

[U28] Py：类型别名
来源：http://hz.xingfuxueyuan.xyz/gtbquqsqum.html

UserId = int
来源：http://hz.yj20258888.top/gtolxhjnrv.html

[U29] Py：属性校验
来源：http://hz.dashuyun.cn/gtxhcalmwy.html

@property 与 @x.setter 配合
来源：http://hz.pycfn.com/gttnpryvvy.html

[U30] Py：数据类
来源：http://hz.zdqjudy.top/gtdsbgpefc.html

@dataclass(slots=True)
来源：http://hz.sweek.top/gtyyzseitc.html

[U31] Py：单测
来源：http://hz.shzxlz.cn/gtueqrmxlr.html

python -m pytest -q
来源：http://hz.wangshuangyany.cn/gtxdjgjzjk.html

[U32] Py：代码格式化
来源：http://hz.chenjidiqi.icu/gtiplmfljv.html

ruff format . && ruff check --fix .
来源：http://hz.zhaomingkeji.xyz/gtffwqysmg.html

[U33] Py：打包发布
来源：http://hz.guowangkeji.top/gtvqkpyngf.html

python -m build  （依赖 pyproject.toml）
来源：http://hz.gogol.net.cn/gtgekdkqxv.html

[U34] Py：判断编码
来源：http://hz.zhiwuduotai.top/gtqtxdqtsp.html

chardet.detect(raw)
来源：http://hz.ivvv.top/gtsoqhcxij.html

[U35] Py：发送邮件
来源：http://hz.meibo888.top/gtoslbxpin.html

smtplib.SMTP_SSL(...).send_message(msg)
来源：http://hz.daxiang520.top/gtenfzpmmm.html

[U36] Py：定时任务
来源：http://hz.guowangkeji.top/gtoumnbhjq.html

schedule.every(10).minutes.do(job)
来源：http://hz.jqgfzy.top/gtjcfhxgij.html

[U37] Py：读写 Excel
来源：http://hz.gaohongyu789.top/gtaejpwyqe.html

pandas.read_excel / DataFrame.to_excel
来源：http://hz.aibaodan.cn/gtvwvepioj.html

[U38] Py：获取脚本所在目录
来源：http://hz.shanyushiyangtech.top/gtihpuwjsm.html

Path(__file__).resolve().parent
来源：http://hz.chenlongwang.top/gtzzsqkluk.html

[U39] Py：判断是否在交互环境
来源：http://hz.aizwys.cn/gtkomtelna.html

sys.stdout.isatty()
来源：http://hz.9152youxi.cn/gtzcmmadtf.html

[U40] Py：打印到标准错误
来源：http://hz.cashguo.top/gtbgahynek.html

print("err", file=sys.stderr)
来源：http://hz.pycfn.com/gtxoimfnqg.html

[U41] PHP：初始化 Composer 项目
来源：http://hz.redwolf501.top/gtjsdudyuo.html

composer init;  composer require guzzlehttp/guzzle
来源：http://hz.jlsjyb.cn/gtymlermdl.html

[U42] PHP：PSR-4 自动加载
来源：http://hz.jlsjyb.cn/gtlzrokled.html

"autoload": { "psr-4": { "App\\": "src/" } }
来源：http://hz.yj202588.top/gtxmixacss.html

[U43] PHP：声明命名空间
来源：http://hz.jianghu66.top/gtucuxulvg.html

namespace App\Http;
来源：http://hz.shuidangran.top/gtoyrwpjzs.html

[U44] PHP：开启严格类型
来源：http://hz.xziqi.cn/gtkxmpinvv.html

declare(strict_types=1);
来源：http://hz.shanyushiyangkeji.top/gtofebsjki.html

[U45] PHP：类型声明与返回类型
来源：http://hz.hammf.cn/gtdjkvhdsx.html

function add(int $a, int $b): int { return $a + $b; }
来源：http://hz.ivvv.top/gtrpjcwuhy.html

[U46] PHP：可空类型
来源：http://hz.yueranfly.top/gtzsuktymu.html

?string $name = null
来源：http://hz.iojbl.cn/gtinijprev.html

[U47] PHP：联合类型
来源：http://hz.hongshengwenyu.top/gtaoifzsrl.html

int|string $id
来源：http://hz.yj202588.top/gtcbokvcsr.html

[U48] PHP：纯枚举
来源：http://hz.wangdashe.top/gtmkdsxmpm.html

enum Status: string { case Active = "active"; case Off = "off"; }
来源：http://hz.dashuyun.cn/gtodoupeas.html

[U49] PHP：只读属性
来源：http://hz.xziqi.cn/gtxpnzzvvh.html

public readonly string $name
来源：http://hz.yj20258888.top/gtuquscuio.html

[U50] PHP：构造器属性提升
来源：http://hz.mhx1999.top/gteieihklg.html

public function __construct(private int $id) {}
来源：http://hz.shanyushiyangtech.top/gthmuvconv.html

[U51] PHP：数组解构
来源：http://hz.shanyushiyangkeji.top/gtretxvavm.html

[$a, $b] = $arr;
来源：http://hz.cqqwz.cn/gtfjrwatuk.html

[U52] PHP：箭头函数
来源：http://hz.yvedp.cn/gtmuvcfioo.html

$double = fn($x) => $x * 2;
来源：http://hz.hnqzz.top/gtfftzewey.html

[U53] PHP：空合并运算符
来源：http://hz.jinqigufen.top/gtnoruasex.html

$v = $a ?? $b ?? "default";
来源：http://hz.hongshengwenyu.top/gthwydnccl.html

[U54] PHP：空安全调用
来源：http://hz.xuanzx.com/gtooakjidk.html

$obj?->method()
来源：http://hz.ydjk.org.cn/gtytmnwggp.html

[U55] PHP：match 表达式
来源：http://hz.zhaomingkeji.xyz/gtkzrnatmc.html

$s = match($x) { 1 => "一", default => "其他" };
来源：http://hz.haohaochexian.top/gtsfnxzsuf.html

[U56] PHP：命名参数
来源：http://hz.yj20258888.top/gtiwonikiv.html

f(a: 1, b: 2)
来源：http://hz.jinqigfzy.top/gtwiircwmz.html

[U57] PHP：字符串插值
来源：http://hz.yanxiufei.cn/gtzewxveyc.html

"值: {$a}"
来源：http://hz.hammf.cn/gtzvzkjtxl.html

[U58] PHP：数组三件套
来源：http://hz.snrcjt.cn/gtpictylhc.html

array_map($f, $a);  array_filter($a, $f);  array_reduce($a, $f, 0);
来源：http://hz.pengpengdd.cyou/gtfnwptsao.html

[U59] PHP：自定义排序
来源：http://hz.quarkkingdee.top/gtqkgtdjmz.html

usort($arr, fn($a, $b) => $a["age"] <=> $b["age"]);
来源：http://hz.xuanzx.com/gtobeqketl.html

[U60] PHP：JSON 编解码
来源：http://hz.xingfuxueyuan.xyz/gtzpkgncml.html

json_encode($d, JSON_UNESCAPED_UNICODE);  json_decode($s, true);
来源：http://hz.vqdsnc.cn/gtcvsdegye.html

[U61] PHP：正则
来源：http://hz.jinyuanbaomall.cn/gtkojieliw.html

preg_match('/(\d+)/', $s, $m);  preg_replace('/\d+/', '#', $s);
来源：http://hz.hammf.cn/gtfdtfjfcn.html

[U62] PHP：日期对象
来源：http://hz.xinyue.icu/gtbobmchug.html

(new DateTimeImmutable())->format("Y-m-d");
来源：http://hz.yj202588.top/gtqvkllsdk.html

[U63] PHP：文件读写
来源：http://hz.pycfn.com/gtspkpqotz.html

file_get_contents($f);  file_put_contents($f, $data);
来源：http://hz.gzhubu.top/gtcddpxzrn.html

[U64] PHP：目录遍历
来源：http://hz.dashuyun.cn/gthgxxtczl.html

glob("dir/*.php");  scandir("dir");
来源：http://hz.sysykeji.top/gtdkenjwzy.html

[U65] PHP：会话
来源：http://hz.nwbrower.top/gtbbglocyf.html

session_start();  $_SESSION["uid"] = 1;
来源：http://hz.52xcode.cn/gtzamunbuy.html

[U66] PHP：设置 Cookie
来源：http://hz.hongshengwenyu.top/gtgevilloy.html

setcookie("token", $v, ["httponly" => true, "samesite" => "Lax"]);
来源：http://hz.aizwys.cn/gtdsvjawth.html


<!-- 参考信息 -->