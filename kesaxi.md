代发 wailian999

[S41] C++：类与构造函数
来源：http://hz.ydzc1.top/gthvtsahec.html

class A { public: A(int v) : x_(v) {} int get() const { return x_; } private: int x_; };
来源：http://hz.snrcjt.cn/gtkqplvwvd.html

[S42] C++：继承与虚函数
来源：http://hz.xingfuxueyuan.xyz/gtupjevqpm.html

class B : public Base { public: void f() override {} };
来源：http://hz.sxryk.cn/gtemxdahfz.html

[S43] C++：智能指针
来源：http://hz.yangfankeji.com/gtvxbfgmug.html

auto p = std::make_unique<int>(5);
来源：http://hz.hongshengwenyu.top/gthrpqywbp.html

[S44] C++：引用传参
来源：http://hz.wangshuangyany.cn/gtyanujkbp.html

void inc(int &x) { ++x; }
来源：http://hz.xuetiantiany.cn/gtqstiuaen.html

[S45] C++：lambda
来源：http://hz.jlsjyb.cn/gtmzxyajdx.html

auto add = [](int a, int b) { return a + b; };
来源：http://hz.gotoacloud.top/gtkqennpkd.html

[S46] C++：函数模板
来源：http://hz.jyoumei.cn/gtdowhxvhf.html

template <typename T> T maxv(T a, T b) { return a > b ? a : b; }
来源：http://hz.pengpengdd.cyou/gtsjyvpbqq.html

[S47] C++：结构化绑定遍历
来源：http://hz.ydzc1.top/gtfylrzsqu.html

for (const auto &[k, v] : m) { std::cout << k << v; }
来源：http://hz.xuanzx.com/gtubnljirz.html

[S48] C++：逐行读文件
来源：http://hz.sufxvd.cn/gtplvevimx.html

std::ifstream in("a.txt");  std::string line;
来源：http://hz.yj20258888.top/gtatbzpbjo.html

while (std::getline(in, line)) { }
来源：http://hz.guannengcc.top/gthzbrfszx.html

[S49] C++：写文件
来源：http://hz.wangshuangyany.cn/gtygwekgcn.html

std::ofstream out("a.txt");  out << "hi\n";
来源：http://hz.jlsjyb.cn/gtfjmujkrn.html

[S50] C++：格式化数字
来源：http://hz.tian-w.cn/gtpkpcorda.html

std::ostringstream os;  os << std::fixed << std::setprecision(2) << 3.14159;
来源：http://hz.hammf.cn/gtvhrdfjmz.html

[S51] C++：显式类型转换
来源：http://hz.316326.xyz/gtniyvwvnn.html

static_cast<double>(a) / b
来源：http://hz.cashguo.top/gtlbnqgbhu.html

[S52] C++：const 与 noexcept
来源：http://hz.ivvv.top/gtguxqetfl.html

int size() const noexcept { return n_; }
来源：http://hz.havefunace.top/gtstouvtiv.html

[S53] C++：移动语义
来源：http://hz.sysykeji.top/gttmmgclne.html

std::vector<int> w = std::move(v);
来源：http://hz.hnxiangtu.top/gtsjfmuizs.html

[S54] C++：异常处理
来源：http://hz.tian-w.cn/gtopnovscl.html

try { throw std::runtime_error("x"); } catch (const std::exception &e) { }
来源：http://hz.chenlongwang.top/gtypitjtxa.html

[S55] C++：结构化绑定
来源：http://hz.sxryk.cn/gtoyzreswf.html

auto [a, b] = std::make_pair(1, 2);
来源：http://hz.zhixingplan.top/gtxzebwegb.html

[S56] C++：optional
来源：http://hz.quarkkingdee.top/gtvczaztrz.html

std::optional<int> o = 5;  if (o) { int v = *o; }
来源：http://hz.shangyingyoupin.top/gtekdjdsud.html

[S57] C++：编译期常量
来源：http://hz.hongshengwenyu.top/gthyxlelgl.html

constexpr int N = 10;
来源：http://hz.ydjk.org.cn/gtodibikdz.html

[S58] C++：命名空间
来源：http://hz.kuanghao11.cn/gtvestnpdj.html

namespace ns { int f() { return 1; } }
来源：http://hz.shangyingyoupin.top/gtgndvtwaq.html

[S59] C++：静态断言
来源：http://hz.jlsjyb.cn/gtpwssvxfl.html

static_assert(sizeof(int) == 4, "int 必须 4 字节");
来源：http://hz.cqqwz.cn/gtncpeylak.html

[S60] C++：遍历并删除元素
来源：http://hz.daxiang520.top/gtouhqfawo.html

v.erase(std::remove_if(v.begin(), v.end(), [](int x) { return x < 0; }), v.end());
来源：http://hz.ybcxt.top/gtdyvwyhwy.html

================================================================================
来源：http://hz.ivvv.top/gtsnnyvnhw.html

T. 其他语言补充（Kotlin / Swift / Lua / Perl / Scala）
来源：http://hz.cucudq.cn/gtapysdswn.html

================================================================================
来源：http://hz.cqqwz.cn/gtwyavjrag.html

[T01] Kotlin：Hello World
来源：http://hz.andypj.xyz/gttgnhiiey.html

println("Hello")
来源：http://hz.jinghuilouyu.cn/gtitdmuyvz.html

[T02] Kotlin：变量
来源：http://hz.cucudq.cn/gtdvjpaiaz.html

val a = 1;  var b = 2        // val 只读，var 可变
来源：http://hz.jianghu66.top/gtxslduydd.html

[T03] Kotlin：字符串模板
来源：http://hz.iojbl.cn/gtjjnfczym.html

"值: $b"
来源：http://hz.ywan-chungtsiang.top/gtnzgrcwpb.html

[T04] Kotlin：空安全
来源：http://hz.tanke756.top/gtckktrdmt.html

val n: String? = null;  n?.length
来源：http://hz.tian-w.cn/gtwgityejc.html

[T05] Kotlin：when 表达式
来源：http://hz.nanxuanxn.top/gtgwipfvrl.html

val s = when (x) { 1 -> "一" else -> "其他" }   // 多分支时每个分支单独一行
来源：http://hz.kuanghao11.cn/gtkzuimspd.html

[T06] Kotlin：集合映射
来源：http://hz.jqgufenzy.top/gtnehqxuhp.html

listOf(1, 2, 3).map { it * 2 }
来源：http://hz.zhoulong.xyz/gtafvhofmx.html

[T07] Kotlin：集合过滤
来源：http://hz.yvedp.cn/gtvrkcjrcz.html

listOf(1, 2, 3).filter { it > 1 }
来源：http://hz.havefunace.top/gthqulurbw.html

[T08] Kotlin：数据类
来源：http://hz.mhx1999.top/gthxhmdlnf.html

data class User(val name: String, val age: Int)
来源：http://hz.chenjidiqi.icu/gtcnvyovau.html

[T09] Kotlin：扩展函数
来源：http://hz.yongpay.top/gtbcosgpfy.html

fun String.exclaim() = this + "!"
来源：http://hz.pycfn.com/gtixuqykjx.html

[T10] Kotlin：默认参数
来源：http://hz.daxiang520.top/gtfecjgzur.html

fun greet(name: String = "World") = "Hi $name"
来源：http://hz.zdqjudy.top/gtwokrkapx.html

[T11] Kotlin：协程
来源：http://hz.daxiang520.top/gtkvjjpyca.html

GlobalScope.launch { delay(1000); println("done") }
来源：http://hz.cucudq.cn/gtncxujuki.html

[T12] Kotlin：解构声明
来源：http://hz.aibaodan.cn/gtpzngccon.html

val (a, b) = Pair(1, 2)
来源：http://hz.xuanzx.com/gtkktfquwa.html

[T13] Kotlin：只读 Map
来源：http://hz.jianghu66.top/gtfdvagikx.html

val m = mapOf("a" to 1)
来源：http://hz.nanxinkj.top/gtlgwywtyw.html

[T14] Kotlin：循环
来源：http://hz.zdqjudy.top/gtirwepolo.html

for (i in 1..10) println(i)
来源：http://hz.nwbrower.top/gtxiwubtnc.html

[T15] Kotlin：接口
来源：http://hz.yj202588.top/gtgozgvhhl.html

interface Shape { fun area(): Double }
来源：http://hz.meibo888.top/gtkdmzkctk.html

[T16] Swift：Hello World
来源：http://hz.nwbrower.top/gtntetxtxk.html

print("Hello")
来源：http://hz.sweek.top/gtvpbllked.html

[T17] Swift：变量与常量
来源：http://hz.smart0.xyz/gtlzdecfuy.html

var a = 1;  let b = 2
来源：http://hz.fengsongda.top/gtidhhcvsf.html

[T18] Swift：字符串插值
来源：http://hz.guowangkeji.top/gtmhjrjhvk.html

"值: \(b)"
来源：http://hz.ivvv.top/gtxfxmxhjl.html

[T19] Swift：可选绑定
来源：http://hz.snrcjt.cn/gttrlytxwu.html

if let n = opt { print(n) }
来源：http://hz.52xcode.cn/gtytgswgdh.html

[T20] Swift：数组操作
来源：http://hz.sysykeji.top/gtjwnsacmu.html

var a = [1, 2, 3];  a.append(4)
来源：http://hz.jyoumei.cn/gtqphflbdl.html

[T21] Swift：遍历
来源：http://hz.hnqzz.top/gtucpvtuan.html

for x in a { print(x) }
来源：http://hz.feifeiyinyue.top/gtojfumtve.html

[T22] Swift：字典
来源：http://hz.9152youxi.cn/gtcifnufpt.html

var d = ["a": 1];  d["b"] = 2
来源：http://hz.dashuyun.cn/gtzvskagvn.html

[T23] Swift：函数
来源：http://hz.birdmap.top/gtshlqdrgj.html

func add(_ a: Int, _ b: Int) -> Int { a + b }
来源：http://hz.yj20258.top/gtrgdcthqw.html

[T24] Swift：闭包
来源：http://hz.cdnleiting.top/gtcwayolda.html

let f = { (x: Int) -> Int in x * 2 }
来源：http://hz.ivvv.top/gtemnvmsgy.html

[T25] Swift：结构体
来源：http://hz.ivvv.top/gtqkgmajkc.html

struct P { var x: Int }
来源：http://hz.aibaodan.cn/gtudwgrtzk.html

[T26] Swift：类与重写
来源：http://hz.nanxinkj.top/gtruykmdwl.html

class A: Base { override func f() {} }
来源：http://hz.zhoulong.xyz/gtwdfqsbab.html

[T27] Swift：错误处理
来源：http://hz.fengsongda.top/gtfiskprrw.html

do { try f() } catch { print(error) }
来源：http://hz.haohaochexian.top/gtmmmwrkmm.html

[T28] Swift：枚举
来源：http://hz.316326.xyz/gtyuqtkona.html

enum Color { case red, green }
来源：http://hz.daxiang520.top/gtzohzhjpq.html

[T29] Swift：guard 提前返回
来源：http://hz.ywan-chungtsiang.top/gtjwtbjcbu.html

guard let x = opt else { return }
来源：http://hz.c1oappe.top/gtenxfrcke.html

[T30] Swift：协议
来源：http://hz.cqqwz.cn/gtynsezzat.html

protocol Shape { func area() -> Double }
来源：http://hz.xylfe.cn/gtohudebex.html

[T31] Lua：Hello World
来源：http://hz.ydjk.org.cn/gtyxjoaahw.html

print("Hello")
来源：http://hz.zhengqikj.top/gtkmfpktbv.html

[T32] Lua：局部变量
来源：http://hz.yueranfly.top/gtyedtzgtl.html

local a = 1
来源：http://hz.yonumen.top/gtsduqxkcq.html

[T33] Lua：表（数组）
来源：http://hz.nwbrower.top/gtfjtpwxzh.html

local t = {1, 2, 3};  t[4] = 4
来源：http://hz.yongpay.top/gtswxxkldt.html

[T34] Lua：遍历表
来源：http://hz.ydjk.org.cn/gtbtkihtyz.html

for i, v in ipairs(t) do print(i, v) end
来源：http://hz.zhiwuduotai.top/gtlcqxyodp.html

[T35] Lua：字典表
来源：http://hz.guowangkeji.top/gtnsuwujsj.html

local d = { a = 1 };  d.b = 2
来源：http://hz.jinqigfzy.top/gtfwubrliq.html

[T36] Lua：函数
来源：http://hz.jyoumei.cn/gthbwsmouw.html

function add(a, b) return a + b end
来源：http://hz.hysaishi.cn/gtbtodgryo.html

[T37] Lua：字符串拼接
来源：http://hz.redwolf501.top/gtlpbbtgne.html

"a" .. "b"
来源：http://hz.zhixingplan.top/gtqcfrwwoa.html

[T38] Lua：条件
来源：http://hz.gzhubu.top/gtdhposdmc.html

if x > 0 then print("正") end
来源：http://hz.ybcxt.top/gttmuhmhfg.html

[T39] Lua：模式匹配
来源：http://hz.yj20258.top/gtxjpqcbpx.html

string.find(s, "%d+")
来源：http://hz.guannengcc.top/gtdiiinrrl.html

[T40] Lua：元表
来源：http://hz.hnqzz.top/gteswbohwt.html

setmetatable({}, { __index = base })
来源：http://hz.sufxvd.cn/gtvrvwnqxb.html

[T41] Perl：Hello World
来源：http://hz.jyoumei.cn/gtoqptkpek.html

print "Hello\n";
来源：http://hz.kuanghao11.cn/gtiubdsaqh.html

[T42] Perl：变量类型
来源：http://hz.havefunace.top/gtnmrwuksi.html

my $a = 1;  my @arr = (1, 2, 3);  my %h = (a => 1);
来源：http://hz.cashguo.top/gtobbdmfmu.html

[T43] Perl：字符串插值
来源：http://hz.hammf.cn/gtopenbnqy.html

"值: $a"
来源：http://hz.shangyingyoupin.top/gttbuaegux.html

[T44] Perl：条件
来源：http://hz.hammf.cn/gtrehppptb.html

if ($a > 0) { print "正"; }
来源：http://hz.ehwqpu.com/gtftmmtoan.html

[T45] Perl：数组遍历
来源：http://hz.havefunace.top/gttimpoggk.html

for my $x (@arr) { print $x; }
来源：http://hz.jinghuilouyu.cn/gtonauxziv.html

[T46] Perl：哈希操作
来源：http://hz.smart0.xyz/gtealpyhkp.html

$h{b} = 2;  for my $k (keys %h) { print "$k=$h{$k}"; }
来源：http://hz.sxryk.cn/gtvhypttjn.html

[T47] Perl：正则捕获
来源：http://hz.sweek.top/gtaelojtpr.html

if ($s =~ /(\d+)/) { print $1; }
来源：http://hz.jianghu66.top/gtsfvjhpmb.html

[T48] Perl：正则替换
来源：http://hz.nwbrower.top/gtlclunefh.html

$s =~ s/old/new/g;
来源：http://hz.cucudq.cn/gtvqxzgyad.html

[T49] Perl：函数
来源：http://hz.chenlongwang.top/gtpnmukwug.html

sub add { my ($a, $b) = @_; return $a + $b; }
来源：http://hz.yj20258888.top/gtvgiooemq.html

[T50] Perl：逐行读文件
来源：http://hz.hywenlv.cn/gtcgaapgkf.html

open my $fh, "<", "a.txt" or die $!;
来源：http://hz.snrcjt.cn/gtkrsbcfqu.html

while (my $line = <$fh>) { print $line; }
来源：http://hz.jinghuilouyu.cn/gtpbmnzset.html

[T51] Scala：Hello World
来源：http://hz.xinyue.icu/gtscryevlu.html

println("Hello")
来源：http://hz.xziqi.cn/gtlcorynrc.html

[T52] Scala：变量
来源：http://hz.jinghuilouyu.cn/gtgnttdxbx.html

val a = 1;  var b = 2
来源：http://hz.hywenlv.cn/gturvrcxpx.html

[T53] Scala：字符串插值
来源：http://hz.aibaodan.cn/gtlyakpyrn.html

s"值: $b"
来源：http://hz.jqgufenzy.top/gtdjeuplfb.html

[T54] Scala：集合映射
来源：http://hz.guannengcc.top/gtjoxwzuhu.html

List(1, 2, 3).map(_ * 2)
来源：http://hz.gzhubu.top/gtmebyzgry.html

[T55] Scala：集合过滤
来源：http://hz.tianlin.xyz/gtalmgwyug.html

List(1, 2, 3).filter(_ > 1)
来源：http://hz.cdnleiting.top/gtyvxnocyu.html

[T56] Scala：样例类
来源：http://hz.zdqjudy.top/gtkbddbokd.html

case class User(name: String, age: Int)
来源：http://hz.daxiang520.top/gtkoyfgctt.html

[T57] Scala：模式匹配
来源：http://hz.yuxming.cn/gtpucfyugo.html

x match { case 1 => "一"; case _ => "其他" }
来源：http://hz.zhoulong.xyz/gtnixlaseq.html

[T58] Scala：函数定义
来源：http://hz.pycfn.com/gtoogmqkaw.html

def add(a: Int, b: Int): Int = a + b
来源：http://hz.kuanghao11.cn/gtdftiuybd.html

[T59] Scala：循环
来源：http://hz.gzhubu.top/gtdnrdtxqy.html

for (i <- 1 to 10) println(i)
来源：http://hz.haohaochexian.top/gtdcyxbhsv.html

[T60] Scala：折叠
来源：http://hz.wangdashe.top/gtuwzsrmzt.html

List(1, 2, 3).foldLeft(0)(_ + _)
来源：http://hz.bjfxy.top/gtsomkbmbj.html

================================================================================
来源：http://hz.vqdsnc.cn/gtpfwpxxga.html

U. 高频实用片段（Python / PHP / JavaScript 各 40 条）
来源：http://hz.daxiang520.top/gtruygxprz.html

================================================================================
来源：http://hz.feifeiyinyue.top/gthkyrybgm.html

[U01] Py：创建虚拟环境
来源：http://hz.zdqjudy.top/gtkzktaynk.html

python -m venv .venv && source .venv/bin/activate
来源：http://hz.gotoacloud.top/gtgbvhijna.html

[U02] Py：导出 / 安装依赖
来源：http://hz.andypj.xyz/gtejsichvk.html

pip freeze > requirements.txt;  pip install -r requirements.txt
来源：http://hz.havefunace.top/gteybkuyff.html

[U03] Py：加载 .env 配置
来源：http://hz.xuetiantiany.cn/gtgopfdwfn.html

from dotenv import load_dotenv; load_dotenv()
来源：http://hz.zhixingplan.top/gtaufvlobs.html

[U04] Py：变量调试打印
来源：http://hz.hnqzz.top/gthymjcves.html

print(f"{x=}")            # 输出 x=值，Python 3.8+
来源：http://hz.svipenyu.cn/gtxcfoaekc.html

[U05] Py：列表去重且保序
来源：http://hz.dashuyun.cn/gtntzcggtl.html

list(dict.fromkeys(arr))
来源：http://hz.andypj.xyz/gtlpllukgi.html

[U06] Py：合并两个字典
来源：http://hz.zycfv.cn/gtyhvxlvle.html

{**a, **b}
来源：http://hz.cucudq.cn/gtehtgrtjt.html

[U07] Py：反转字典键值
来源：http://hz.fzhhl.top/gtxkvipkcd.html

{v: k for k, v in d.items()}
来源：http://hz.cheryme.top/gtlryktlki.html

[U08] Py：展平二维列表
来源：http://hz.xziqi.cn/gtmhurtqty.html

[y for x in nested for y in x]
来源：http://hz.jiagoushi.top/gtupyobeck.html

[U09] Py：字典取最大值的键
来源：http://hz.pycfn.com/gtdvkkzjua.html

max(d, key=d.get)
来源：http://hz.cdnleiting.top/gtcmfiotzj.html

[U10] Py：按值排序字典
来源：http://hz.jinqigfzy.top/gtjuhmmmaq.html

dict(sorted(d.items(), key=lambda kv: kv[1]))
来源：http://hz.gaohongyu789.top/gtymmgfcla.html

[U11] Py：生成器表达式
来源：http://hz.xuetiantiany.cn/gtmzbdyggr.html

(x * 2 for x in arr)
来源：http://hz.yuxming.cn/gtmounvyov.html

[U12] Py：取出现最多的 3 个元素
来源：http://hz.yueranfly.top/gtdgfgbylc.html

Counter(arr).most_common(3)
来源：http://hz.zhijiandao.cn/gtbdfkfujn.html

[U13] Py：固定长度队列
来源：http://hz.wangshuangyany.cn/gtzboobpqh.html

deque(maxlen=10)
来源：http://hz.yvedp.cn/gtwhxhwfkq.html

[U14] Py：分组收集到列表
来源：http://hz.cdnleiting.top/gtonzaqomj.html

defaultdict(list)
来源：http://hz.cqqwz.cn/gtrnnhohwz.html

[U15] Py：高精度计时
来源：http://hz.ybcxt.top/gturdnnjnl.html

t = time.perf_counter()
来源：http://hz.zhaomingkeji.xyz/gtjwnyzxja.html

[U16] Py：命令行参数解析
来源：http://hz.xziqi.cn/gtzjstxpkx.html

ap = argparse.ArgumentParser();  ap.add_argument("--name");  args = ap.parse_args()
来源：http://hz.ywan-chungtsiang.top/gttsukpppt.html

[U17] Py：初始化日志
来源：http://hz.mhx1999.top/gtpjcfvpzp.html

logging.basicConfig(level=logging.INFO)
来源：http://hz.wangshuangyany.cn/gtagarvxpq.html

[U18] Py：预编译正则
来源：http://hz.hywenlv.cn/gtxpjdrkzi.html

pat = re.compile(r"\d+")
来源：http://hz.hfpthk.cn/gthklffezn.html

[U19] Py：正则替换带回调
来源：http://hz.yuxming.cn/gtkngyowpj.html

re.sub(r"\d+", lambda m: str(int(m.group()) * 2), s)
来源：http://hz.zhengqikj.top/gtixfqtypx.html

[U20] Py：缓存函数结果
来源：http://hz.316326.xyz/gtdnaxewxx.html

@functools.lru_cache(maxsize=None)
来源：http://hz.hywenlv.cn/gtuztxoqnr.html

[U21] Py：自定义上下文管理器
来源：http://hz.iojbl.cn/gtyxjvmhia.html

@contextlib.contextmanager
来源：http://hz.chenzaomai.com/gtpyxbxxwd.html

[U22] Py：矩阵转置
来源：http://hz.xziqi.cn/gtwnbwzpeg.html

list(zip(*m))
来源：http://hz.gzhubu.top/gtsvmfsuih.html

[U23] Py：分块读取大文件
来源：http://hz.pengpengdd.cyou/gtfgvrvayg.html

for chunk in iter(lambda: f.read(8192), b""):
来源：http://hz.zhiwuduotai.top/gtesodksqo.html

[U24] Py：路径操作
来源：http://hz.xuanzx.com/gtcdullmdv.html

Path("a/b.txt").parent.mkdir(parents=True, exist_ok=True)
来源：http://hz.ehwqpu.com/gtqsbgfiuv.html

[U25] Py：CSV 按字典读
来源：http://hz.shanyushiyangtech.top/gtveeowtwb.html

csv.DictReader(f)
来源：http://hz.dashuyun.cn/gtbbowcdql.html

[U26] Py：并发下载
来源：http://hz.snrcjt.cn/gtgzookoff.html

ThreadPoolExecutor(max_workers=8).map(fetch, urls)
来源：http://hz.cucudq.cn/gtfxnlxljs.html

[U27] Py：异步 HTTP
来源：http://hz.hnqzz.top/gtewtsaxwp.html

aiohttp.ClientSession() 配合 async with
来源：http://hz.dianchejie.cn/gtxpgztoct.html

[U28] Py：类型别名
来源：http://hz.dianchejie.cn/gtsxicixjw.html

UserId = int
来源：http://hz.ehwqpu.com/gtiqwuupdq.html

[U29] Py：属性校验
来源：http://hz.shanyushiyangtech.top/gtqrcdevji.html

@property 与 @x.setter 配合
来源：http://hz.aibaodan.cn/gtndupzlms.html

[U30] Py：数据类
来源：http://hz.ehwqpu.com/gtddaclrqq.html

@dataclass(slots=True)
来源：http://hz.sweek.top/gthhpaaavf.html

[U31] Py：单测
来源：http://hz.tianlin.xyz/gtktmnkvsb.html

python -m pytest -q
来源：http://hz.shzxlz.cn/gtffnirqfh.html

[U32] Py：代码格式化
来源：http://hz.wangdashe.top/gtzttwweww.html

ruff format . && ruff check --fix .
来源：http://hz.nwbrower.top/gtxioivzws.html

[U33] Py：打包发布
来源：http://hz.ybcxt.top/gttjwtrrhq.html

python -m build  （依赖 pyproject.toml）
来源：http://hz.sysykeji.top/gtbbcqiarn.html

[U34] Py：判断编码
来源：http://hz.wangshuangyany.cn/gtalgtgkex.html

chardet.detect(raw)
来源：http://hz.zhiwuduotai.top/gtzkctlwtb.html

[U35] Py：发送邮件
来源：http://hz.shanyushiyangkeji.top/gtocwtydli.html

smtplib.SMTP_SSL(...).send_message(msg)
来源：http://hz.smart0.xyz/gtplkxdtbf.html

[U36] Py：定时任务
来源：http://hz.fengsongda.top/gtysrcddzc.html

schedule.every(10).minutes.do(job)
来源：http://hz.wangdashe.top/gthazlceqz.html

[U37] Py：读写 Excel
来源：http://hz.yuxming.cn/gtlbqavujx.html

pandas.read_excel / DataFrame.to_excel
来源：http://hz.yj20258.top/gtbsheghny.html

[U38] Py：获取脚本所在目录
来源：http://hz.shanyushiyangkeji.top/gtunpjpgly.html

Path(__file__).resolve().parent
来源：http://hz.xziqi.cn/gtmxqqfpbf.html

[U39] Py：判断是否在交互环境
来源：http://hz.gogol.net.cn/gtogyohilu.html

sys.stdout.isatty()
来源：http://hz.smart0.xyz/gtyigxbyeo.html

[U40] Py：打印到标准错误
来源：http://hz.jinqigfzy.top/gtjgiksajw.html

print("err", file=sys.stderr)
来源：http://hz.xinyue.icu/gtonewqrjd.html

[U41] PHP：初始化 Composer 项目
来源：http://hz.fengsongda.top/gthyivqqua.html

composer init;  composer require guzzlehttp/guzzle
来源：http://hz.52xcode.cn/gtasaqprag.html

[U42] PHP：PSR-4 自动加载
来源：http://hz.yongpay.top/gtzoekggfm.html

"autoload": { "psr-4": { "App\\": "src/" } }
来源：http://hz.ybcxt.top/gtjjlkfwms.html

[U43] PHP：声明命名空间
来源：http://hz.jinghuilouyu.cn/gtfrffmvyd.html

namespace App\Http;
来源：http://hz.tian-w.cn/gtiizgfdsf.html

[U44] PHP：开启严格类型
来源：http://hz.yj20258.top/gtpyrpbqwx.html

declare(strict_types=1);
来源：http://hz.fengsongda.top/gthqlqixjl.html

[U45] PHP：类型声明与返回类型
来源：http://hz.hongshengwenyu.top/gtcyqagxws.html

function add(int $a, int $b): int { return $a + $b; }
来源：http://hz.yueranfly.top/gtonocgvwa.html

[U46] PHP：可空类型
来源：http://hz.ywan-chungtsiang.top/gtfzphkqwu.html

?string $name = null
来源：http://hz.xuanzx.com/gtasaxuqsf.html

[U47] PHP：联合类型
来源：http://hz.hywenlv.cn/gtbtnujqve.html

int|string $id
来源：http://hz.xingfuxueyuan.xyz/gtaiwtbfox.html

[U48] PHP：纯枚举
来源：http://hz.chenlongwang.top/gtzgkexbcb.html

enum Status: string { case Active = "active"; case Off = "off"; }
来源：http://hz.ywan-chungtsiang.top/gtvbnixiou.html

[U49] PHP：只读属性
来源：http://hz.vqdsnc.cn/gtwtqsflsv.html

public readonly string $name
来源：http://hz.jinqigufen.top/gtksyqrruo.html

[U50] PHP：构造器属性提升
来源：http://hz.wangshuangyany.cn/gtomqwahsd.html

public function __construct(private int $id) {}
来源：http://hz.kuanghao11.cn/gtvpijgkrp.html

[U51] PHP：数组解构
来源：http://hz.ywan-chungtsiang.top/gtcgpmyhae.html

[$a, $b] = $arr;
来源：http://hz.guannengcc.top/gtysanczxf.html

[U52] PHP：箭头函数
来源：http://hz.xziqi.cn/gtwtnnsbfp.html

$double = fn($x) => $x * 2;
来源：http://hz.aizwys.cn/gttdvmbuja.html

[U53] PHP：空合并运算符
来源：http://hz.svipenyu.cn/gtpcljnzwy.html

$v = $a ?? $b ?? "default";
来源：http://hz.chenjidiqi.icu/gtulahylbj.html

[U54] PHP：空安全调用
来源：http://hz.hnqzz.top/gtsdckisfr.html

$obj?->method()
来源：http://hz.svipenyu.cn/gtfdtvefvr.html

[U55] PHP：match 表达式
来源：http://hz.sweek.top/gtozsbmoqp.html

$s = match($x) { 1 => "一", default => "其他" };
来源：http://hz.yj20258888.top/gttwkatycm.html

[U56] PHP：命名参数
来源：http://hz.316326.xyz/gttcmyuacp.html

f(a: 1, b: 2)
来源：http://hz.havefunace.top/gtmpsywipz.html

[U57] PHP：字符串插值
来源：http://hz.gaohongyu789.top/gtbhnzkoag.html

"值: {$a}"
来源：http://hz.xinyue.icu/gtifckwzcy.html

[U58] PHP：数组三件套
来源：http://hz.daria6918.cn/gtpfidvtwg.html

array_map($f, $a);  array_filter($a, $f);  array_reduce($a, $f, 0);
来源：http://hz.hysaishi.cn/gtvwsbyhqu.html

[U59] PHP：自定义排序
来源：http://hz.cashguo.top/gtyrbffdau.html

usort($arr, fn($a, $b) => $a["age"] <=> $b["age"]);
来源：http://hz.pycfn.com/gtteqshmnr.html

[U60] PHP：JSON 编解码
来源：http://hz.xinyue.icu/gtykabqabg.html

json_encode($d, JSON_UNESCAPED_UNICODE);  json_decode($s, true);
来源：http://hz.pycfn.com/gtdcoplqtd.html

[U61] PHP：正则
来源：http://hz.feifeiyinyue.top/gtwxmbidfs.html

preg_match('/(\d+)/', $s, $m);  preg_replace('/\d+/', '#', $s);
来源：http://hz.cheryme.top/gtkzdzpytn.html

[U62] PHP：日期对象
来源：http://hz.jianghu66.top/gtwbxremji.html

(new DateTimeImmutable())->format("Y-m-d");
来源：http://hz.iojbl.cn/gtnlrgxbbh.html

[U63] PHP：文件读写
来源：http://hz.yongpay.top/gtrgninmsf.html

file_get_contents($f);  file_put_contents($f, $data);
来源：http://hz.xuetiantiany.cn/gtdripvvwo.html

[U64] PHP：目录遍历
来源：http://hz.xziqi.cn/gtqenajyoo.html

glob("dir/*.php");  scandir("dir");
来源：http://hz.fzhhl.top/gtdhpkcpzx.html

[U65] PHP：会话
来源：http://hz.yj20258888.top/gtvnxmppzm.html

session_start();  $_SESSION["uid"] = 1;
来源：http://hz.iojbl.cn/gtbzalsjgn.html

[U66] PHP：设置 Cookie
来源：http://hz.shzxlz.cn/gtrzjbxclc.html

setcookie("token", $v, ["httponly" => true, "samesite" => "Lax"]);
来源：http://hz.jiagoushi.top/gtwflhzzjp.html


<!-- 参考信息 -->