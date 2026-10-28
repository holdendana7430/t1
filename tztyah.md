代发 wailian999

[S41] C++：类与构造函数
来源：http://hz.jiagoushi.top/gteitoqtyj.html

class A { public: A(int v) : x_(v) {} int get() const { return x_; } private: int x_; };
来源：http://hz.zycfv.cn/gtdyqoscum.html

[S42] C++：继承与虚函数
来源：http://hz.iojbl.cn/gtuvvcpthw.html

class B : public Base { public: void f() override {} };
来源：http://hz.yonumen.top/gtugsaefnh.html

[S43] C++：智能指针
来源：http://hz.ppjwa.cn/gtjmmomdtg.html

auto p = std::make_unique<int>(5);
来源：http://hz.yuxming.cn/gtobxxfsqq.html

[S44] C++：引用传参
来源：http://hz.pengpengdd.cyou/gtvhauchwd.html

void inc(int &x) { ++x; }
来源：http://hz.feifeiyinyue.top/gtzgvqrizf.html

[S45] C++：lambda
来源：http://hz.kuanghao11.cn/gtjmapolxj.html

auto add = [](int a, int b) { return a + b; };
来源：http://hz.jinghuilouyu.cn/gtmxzsgool.html

[S46] C++：函数模板
来源：http://hz.yangfankeji.com/gtzsdifzqt.html

template <typename T> T maxv(T a, T b) { return a > b ? a : b; }
来源：http://hz.sufxvd.cn/gthexrdcrl.html

[S47] C++：结构化绑定遍历
来源：http://hz.cucudq.cn/gtgsfztvvz.html

for (const auto &[k, v] : m) { std::cout << k << v; }
来源：http://hz.zdqjudy.top/gtidqklyvz.html

[S48] C++：逐行读文件
来源：http://hz.hfpthk.cn/gtulwzoehc.html

std::ifstream in("a.txt");  std::string line;
来源：http://hz.ehwqpu.com/gtuisesikd.html

while (std::getline(in, line)) { }
来源：http://hz.ywan-chungtsiang.top/gtpznpzgbc.html

[S49] C++：写文件
来源：http://hz.guowangkeji.top/gtpwrovrtr.html

std::ofstream out("a.txt");  out << "hi\n";
来源：http://hz.fengsongda.top/gtshucwmpm.html

[S50] C++：格式化数字
来源：http://hz.sysykeji.top/gtvdbvifli.html

std::ostringstream os;  os << std::fixed << std::setprecision(2) << 3.14159;
来源：http://hz.cashguo.top/gtuyfocybt.html

[S51] C++：显式类型转换
来源：http://hz.gzhubu.top/gtghsqqouy.html

static_cast<double>(a) / b
来源：http://hz.iojbl.cn/gtklswwiok.html

[S52] C++：const 与 noexcept
来源：http://hz.guannengcc.top/gtmgqqiueg.html

int size() const noexcept { return n_; }
来源：http://hz.smart0.xyz/gtmbmwlvzs.html

[S53] C++：移动语义
来源：http://hz.sysykeji.top/gtqpvcikpr.html

std::vector<int> w = std::move(v);
来源：http://hz.hnqzz.top/gtpfvwzwov.html

[S54] C++：异常处理
来源：http://hz.jyoumei.cn/gtnywdggam.html

try { throw std::runtime_error("x"); } catch (const std::exception &e) { }
来源：http://hz.xziqi.cn/gtgavdafbr.html

[S55] C++：结构化绑定
来源：http://hz.shanyushiyangtech.top/gtukfuubny.html

auto [a, b] = std::make_pair(1, 2);
来源：http://hz.jinqigufen.top/gturywscyn.html

[S56] C++：optional
来源：http://hz.xylfe.cn/gtuqkozaxt.html

std::optional<int> o = 5;  if (o) { int v = *o; }
来源：http://hz.jqgfzy.top/gtpmrdysjh.html

[S57] C++：编译期常量
来源：http://hz.aizwys.cn/gtalriobus.html

constexpr int N = 10;
来源：http://hz.aizwys.cn/gtoihqvnju.html

[S58] C++：命名空间
来源：http://hz.redwolf501.top/gtthfazjen.html

namespace ns { int f() { return 1; } }
来源：http://hz.xingfuxueyuan.xyz/gtsyviwflq.html

[S59] C++：静态断言
来源：http://hz.xziqi.cn/gtctglxmvy.html

static_assert(sizeof(int) == 4, "int 必须 4 字节");
来源：http://hz.nanxinkj.top/gtobeogvig.html

[S60] C++：遍历并删除元素
来源：http://hz.tian-w.cn/gtkzixznkk.html

v.erase(std::remove_if(v.begin(), v.end(), [](int x) { return x < 0; }), v.end());
来源：http://hz.c1oappe.top/gtzpsfwmda.html

================================================================================
来源：http://hz.shanyushiyangkeji.top/gtwtxvyobw.html

T. 其他语言补充（Kotlin / Swift / Lua / Perl / Scala）
来源：http://hz.yj20258888.top/gtemvshusj.html

================================================================================
来源：http://hz.andypj.xyz/gtbcqgjdnh.html

[T01] Kotlin：Hello World
来源：http://hz.havefunace.top/gtphxwlata.html

println("Hello")
来源：http://hz.shzxlz.cn/gtatknuvid.html

[T02] Kotlin：变量
来源：http://hz.redwolf501.top/gtkznxsriw.html

val a = 1;  var b = 2        // val 只读，var 可变
来源：http://hz.ywan-chungtsiang.top/gtuwyrtigx.html

[T03] Kotlin：字符串模板
来源：http://hz.shangyingyoupin.top/gtgkqtrqcz.html

"值: $b"
来源：http://hz.jianghu66.top/gtuyvehhnd.html

[T04] Kotlin：空安全
来源：http://hz.zhengqikj.top/gtiwimxaay.html

val n: String? = null;  n?.length
来源：http://hz.nanxuanxn.top/gtsatvihdz.html

[T05] Kotlin：when 表达式
来源：http://hz.vqdsnc.cn/gtzfrvjsgu.html

val s = when (x) { 1 -> "一" else -> "其他" }   // 多分支时每个分支单独一行
来源：http://hz.jinqigfzy.top/gtmtkvbwim.html

[T06] Kotlin：集合映射
来源：http://hz.daxiang520.top/gtzjyzpjnm.html

listOf(1, 2, 3).map { it * 2 }
来源：http://hz.yj202588.top/gtkbvxsiwd.html

[T07] Kotlin：集合过滤
来源：http://hz.jqgfzy.top/gttjbhmxkp.html

listOf(1, 2, 3).filter { it > 1 }
来源：http://hz.xziqi.cn/gtxlsymthp.html

[T08] Kotlin：数据类
来源：http://hz.fengsongda.top/gtodygpiek.html

data class User(val name: String, val age: Int)
来源：http://hz.meibo888.top/gtadpwcnxv.html

[T09] Kotlin：扩展函数
来源：http://hz.daxiang520.top/gtdmzanqrw.html

fun String.exclaim() = this + "!"
来源：http://hz.ywan-chungtsiang.top/gtzwmuntub.html

[T10] Kotlin：默认参数
来源：http://hz.zhaomingkeji.xyz/gtpanjjocg.html

fun greet(name: String = "World") = "Hi $name"
来源：http://hz.wangdashe.top/gtonpwqake.html

[T11] Kotlin：协程
来源：http://hz.xylfe.cn/gtxeuwdbzi.html

GlobalScope.launch { delay(1000); println("done") }
来源：http://hz.tianlin.xyz/gtdkhqeyhb.html

[T12] Kotlin：解构声明
来源：http://hz.ybcxt.top/gtogakmvik.html

val (a, b) = Pair(1, 2)
来源：http://hz.0kj1m.cn/gtzkbqucba.html

[T13] Kotlin：只读 Map
来源：http://hz.jlsjyb.cn/gtrinvqdxm.html

val m = mapOf("a" to 1)
来源：http://hz.jianghu66.top/gtvcdokbxl.html

[T14] Kotlin：循环
来源：http://hz.hnqzz.top/gtwyxqacyg.html

for (i in 1..10) println(i)
来源：http://hz.gotoacloud.top/gtxraoqghv.html

[T15] Kotlin：接口
来源：http://hz.gzhubu.top/gtvftxfoma.html

interface Shape { fun area(): Double }
来源：http://hz.feifeiyinyue.top/gtlgosqaer.html

[T16] Swift：Hello World
来源：http://hz.smart0.xyz/gtfirlazfu.html

print("Hello")
来源：http://hz.0kj1m.cn/gtrsczzkru.html

[T17] Swift：变量与常量
来源：http://hz.dianchejie.cn/gtwxivzreh.html

var a = 1;  let b = 2
来源：http://hz.ivvv.top/gtysttkfto.html

[T18] Swift：字符串插值
来源：http://hz.pycfn.com/gtzpgugigd.html

"值: \(b)"
来源：http://hz.yj20258888.top/gtbqyxsdhp.html

[T19] Swift：可选绑定
来源：http://hz.redwolf501.top/gtngbqudqv.html

if let n = opt { print(n) }
来源：http://hz.yongpay.top/gtxcjxoeif.html

[T20] Swift：数组操作
来源：http://hz.shanyushiyangkeji.top/gtdgwwvhve.html

var a = [1, 2, 3];  a.append(4)
来源：http://hz.daria6918.cn/gtqabrzfel.html

[T21] Swift：遍历
来源：http://hz.ydzc1.top/gtqubqijtq.html

for x in a { print(x) }
来源：http://hz.andypj.xyz/gtrpqvridz.html

[T22] Swift：字典
来源：http://hz.9152youxi.cn/gtwxzorifw.html

var d = ["a": 1];  d["b"] = 2
来源：http://hz.ppjwa.cn/gtaiyfyaeh.html

[T23] Swift：函数
来源：http://hz.ybcxt.top/gtywsieddx.html

func add(_ a: Int, _ b: Int) -> Int { a + b }
来源：http://hz.xingfuxueyuan.xyz/gtymnsxvyb.html

[T24] Swift：闭包
来源：http://hz.guowangkeji.top/gtjxbfqehd.html

let f = { (x: Int) -> Int in x * 2 }
来源：http://hz.cheryme.top/gtywgqzwnu.html

[T25] Swift：结构体
来源：http://hz.mhx1999.top/gtcwcivvss.html

struct P { var x: Int }
来源：http://hz.yuxming.cn/gtsfgzrtrf.html

[T26] Swift：类与重写
来源：http://hz.shzxlz.cn/gtrusetcjc.html

class A: Base { override func f() {} }
来源：http://hz.fengsongda.top/gtitwprsfe.html

[T27] Swift：错误处理
来源：http://hz.smart0.xyz/gtjpppihdf.html

do { try f() } catch { print(error) }
来源：http://hz.kuanghao11.cn/gtwzwsqzwn.html

[T28] Swift：枚举
来源：http://hz.wangdashe.top/gtzjkkoxvd.html

enum Color { case red, green }
来源：http://hz.jinghuilouyu.cn/gtjlhzvcfu.html

[T29] Swift：guard 提前返回
来源：http://hz.kuanghao11.cn/gtlqxxeytj.html

guard let x = opt else { return }
来源：http://hz.shangyingyoupin.top/gtcuefziwy.html

[T30] Swift：协议
来源：http://hz.ybcxt.top/gtumruzxqd.html

protocol Shape { func area() -> Double }
来源：http://hz.jlsjyb.cn/gtgydxexjz.html

[T31] Lua：Hello World
来源：http://hz.meibo888.top/gtxrrqqmwk.html

print("Hello")
来源：http://hz.zhijiandao.cn/gtvbjaadpq.html

[T32] Lua：局部变量
来源：http://hz.xinyue.icu/gtwudqvmfa.html

local a = 1
来源：http://hz.redwolf501.top/gtizgcupiu.html

[T33] Lua：表（数组）
来源：http://hz.yj20258888.top/gthrqwqhep.html

local t = {1, 2, 3};  t[4] = 4
来源：http://hz.gaohongyu789.top/gtmcjzaxjm.html

[T34] Lua：遍历表
来源：http://hz.xuetiantiany.cn/gtpdpbyanb.html

for i, v in ipairs(t) do print(i, v) end
来源：http://hz.yangfankeji.com/gtobrysbwr.html

[T35] Lua：字典表
来源：http://hz.zdqjudy.top/gtfllmwqsl.html

local d = { a = 1 };  d.b = 2
来源：http://hz.shangyingyoupin.top/gtblshvjah.html

[T36] Lua：函数
来源：http://hz.jlsjyb.cn/gthnibrtrq.html

function add(a, b) return a + b end
来源：http://hz.zhoulong.xyz/gtwyqfrjmb.html

[T37] Lua：字符串拼接
来源：http://hz.zhaomingkeji.xyz/gtmgwmzvhm.html

"a" .. "b"
来源：http://hz.tanke756.top/gthyosssnn.html

[T38] Lua：条件
来源：http://hz.zhiwuduotai.top/gtaddtistf.html

if x > 0 then print("正") end
来源：http://hz.wangshuangyany.cn/gtjrmexbaz.html

[T39] Lua：模式匹配
来源：http://hz.zhongyouzk.top/gtpmveowtn.html

string.find(s, "%d+")
来源：http://hz.smart0.xyz/gtaikxuehz.html

[T40] Lua：元表
来源：http://hz.ehwqpu.com/gtxdehyisk.html

setmetatable({}, { __index = base })
来源：http://hz.sysykeji.top/gtyxrbrkkn.html

[T41] Perl：Hello World
来源：http://hz.jyoumei.cn/gtgsufkcbs.html

print "Hello\n";
来源：http://hz.sufxvd.cn/gttgjgaekt.html

[T42] Perl：变量类型
来源：http://hz.nwbrower.top/gtdzdfjdwi.html

my $a = 1;  my @arr = (1, 2, 3);  my %h = (a => 1);
来源：http://hz.jyoumei.cn/gtvyarodiu.html

[T43] Perl：字符串插值
来源：http://hz.9152youxi.cn/gtvdexjxdr.html

"值: $a"
来源：http://hz.chenjidiqi.icu/gtlbqzppwv.html

[T44] Perl：条件
来源：http://hz.shangyingyoupin.top/gttevwvayn.html

if ($a > 0) { print "正"; }
来源：http://hz.aizwys.cn/gtahfyctxc.html

[T45] Perl：数组遍历
来源：http://hz.jinyuanbaomall.cn/gtqxkotmvf.html

for my $x (@arr) { print $x; }
来源：http://hz.jinqigfzy.top/gtlgcsdrxd.html

[T46] Perl：哈希操作
来源：http://hz.feifeiyinyue.top/gtptonqcvi.html

$h{b} = 2;  for my $k (keys %h) { print "$k=$h{$k}"; }
来源：http://hz.c1oappe.top/gtfbmrirwc.html

[T47] Perl：正则捕获
来源：http://hz.vqdsnc.cn/gtbllsudyf.html

if ($s =~ /(\d+)/) { print $1; }
来源：http://hz.pengpengdd.cyou/gtauvseftt.html

[T48] Perl：正则替换
来源：http://hz.guowangkeji.top/gtphdafxbl.html

$s =~ s/old/new/g;
来源：http://hz.cashguo.top/gtebegatbi.html

[T49] Perl：函数
来源：http://hz.birdmap.top/gtepooxckx.html

sub add { my ($a, $b) = @_; return $a + $b; }
来源：http://hz.jinqigfzy.top/gtdnnzmxjx.html

[T50] Perl：逐行读文件
来源：http://hz.shzxlz.cn/gtzywsqpgz.html

open my $fh, "<", "a.txt" or die $!;
来源：http://hz.aibaodan.cn/gtzdklivad.html

while (my $line = <$fh>) { print $line; }
来源：http://hz.birdmap.top/gtgdtcesee.html

[T51] Scala：Hello World
来源：http://hz.shzxlz.cn/gthimreqhf.html

println("Hello")
来源：http://hz.svipenyu.cn/gttibfscod.html

[T52] Scala：变量
来源：http://hz.snrcjt.cn/gtqjeiejqo.html

val a = 1;  var b = 2
来源：http://hz.yj20258.top/gtzcxzseqd.html

[T53] Scala：字符串插值
来源：http://hz.tianlin.xyz/gtqwgfvihh.html

s"值: $b"
来源：http://hz.ehwqpu.com/gtuwxqdigx.html

[T54] Scala：集合映射
来源：http://hz.pengpengdd.cyou/gtvnwshuhg.html

List(1, 2, 3).map(_ * 2)
来源：http://hz.yonumen.top/gttihlukao.html

[T55] Scala：集合过滤
来源：http://hz.yuxming.cn/gtmnoylnby.html

List(1, 2, 3).filter(_ > 1)
来源：http://hz.xziqi.cn/gticdkolzn.html

[T56] Scala：样例类
来源：http://hz.zhengqikj.top/gtilfinicl.html

case class User(name: String, age: Int)
来源：http://hz.pycfn.com/gtuyejnhzp.html

[T57] Scala：模式匹配
来源：http://hz.jinqigufen.top/gtofeyzsxx.html

x match { case 1 => "一"; case _ => "其他" }
来源：http://hz.0kj1m.cn/gtxmpsrfxp.html

[T58] Scala：函数定义
来源：http://hz.shanyushiyangkeji.top/gtwseabgtu.html

def add(a: Int, b: Int): Int = a + b
来源：http://hz.316326.xyz/gthxzufsse.html

[T59] Scala：循环
来源：http://hz.svipenyu.cn/gthqwzscqq.html

for (i <- 1 to 10) println(i)
来源：http://hz.hfpthk.cn/gtojxgbqep.html

[T60] Scala：折叠
来源：http://hz.daxiang520.top/gtrfdmryzj.html

List(1, 2, 3).foldLeft(0)(_ + _)
来源：http://hz.gaohongyu789.top/gtgvddudrv.html

================================================================================
来源：http://hz.wangshuangyany.cn/gtjqijpzaj.html

U. 高频实用片段（Python / PHP / JavaScript 各 40 条）
来源：http://hz.jinqigufen.top/gthjturkoq.html

================================================================================
来源：http://hz.hnqzz.top/gtjtoitmro.html

[U01] Py：创建虚拟环境
来源：http://hz.meibo888.top/gtozhjfeix.html

python -m venv .venv && source .venv/bin/activate
来源：http://hz.ehwqpu.com/gtnekzkusg.html

[U02] Py：导出 / 安装依赖
来源：http://hz.52xcode.cn/gtbkdbfbla.html

pip freeze > requirements.txt;  pip install -r requirements.txt
来源：http://hz.hnxiangtu.top/gtzjwjbose.html

[U03] Py：加载 .env 配置
来源：http://hz.havefunace.top/gtfhyhgscz.html

from dotenv import load_dotenv; load_dotenv()
来源：http://hz.daxiang520.top/gtwfdhnstn.html

[U04] Py：变量调试打印
来源：http://hz.cdnleiting.top/gtnhbfjids.html

print(f"{x=}")            # 输出 x=值，Python 3.8+
来源：http://hz.shangyingyoupin.top/gtsyjtmimh.html

[U05] Py：列表去重且保序
来源：http://hz.iojbl.cn/gtxlhbetmx.html

list(dict.fromkeys(arr))
来源：http://hz.iojbl.cn/gtjwxnrkqk.html

[U06] Py：合并两个字典
来源：http://hz.jinyuanbaomall.cn/gtqfcughik.html

{**a, **b}
来源：http://hz.aizwys.cn/gtluzeahfv.html

[U07] Py：反转字典键值
来源：http://hz.aizwys.cn/gtuqhxcwsc.html

{v: k for k, v in d.items()}
来源：http://hz.shuidangran.top/gtqrunmuls.html

[U08] Py：展平二维列表
来源：http://hz.yanxiufei.cn/gtmwfrakoo.html

[y for x in nested for y in x]
来源：http://hz.cucudq.cn/gtthrqgdpx.html

[U09] Py：字典取最大值的键
来源：http://hz.xylfe.cn/gtfidqayiu.html

max(d, key=d.get)
来源：http://hz.9152youxi.cn/gtpjymjzqp.html

[U10] Py：按值排序字典
来源：http://hz.wangshuangyany.cn/gtrnxztbtg.html

dict(sorted(d.items(), key=lambda kv: kv[1]))
来源：http://hz.guannengcc.top/gtcbqfyduz.html

[U11] Py：生成器表达式
来源：http://hz.9152youxi.cn/gtujlviwob.html

(x * 2 for x in arr)
来源：http://hz.chenlongwang.top/gthjfrnpax.html

[U12] Py：取出现最多的 3 个元素
来源：http://hz.aibaodan.cn/gtijmhtjat.html

Counter(arr).most_common(3)
来源：http://hz.andypj.xyz/gtrsjbimks.html

[U13] Py：固定长度队列
来源：http://hz.feifeiyinyue.top/gtgtiokihs.html

deque(maxlen=10)
来源：http://hz.guowangkeji.top/gtqsduvnuz.html

[U14] Py：分组收集到列表
来源：http://hz.xinyue.icu/gtgfimnmfs.html

defaultdict(list)
来源：http://hz.pengpengdd.cyou/gtclvxgnkm.html

[U15] Py：高精度计时
来源：http://hz.pengpengdd.cyou/gtzowwotcx.html

t = time.perf_counter()
来源：http://hz.tian-w.cn/gtkzmfnadn.html

[U16] Py：命令行参数解析
来源：http://hz.mhx1999.top/gtdplnxpfl.html

ap = argparse.ArgumentParser();  ap.add_argument("--name");  args = ap.parse_args()
来源：http://hz.gotoacloud.top/gttgngfyvu.html

[U17] Py：初始化日志
来源：http://hz.xingfuxueyuan.xyz/gtjrplmxtr.html

logging.basicConfig(level=logging.INFO)
来源：http://hz.yj20258.top/gtiojhqzxu.html

[U18] Py：预编译正则
来源：http://hz.zhongyouzk.top/gtqfiedijy.html

pat = re.compile(r"\d+")
来源：http://hz.bjfxy.top/gtyazbyvwh.html

[U19] Py：正则替换带回调
来源：http://hz.nwbrower.top/gtfjmfngvt.html

re.sub(r"\d+", lambda m: str(int(m.group()) * 2), s)
来源：http://hz.wangshuangyany.cn/gtlnfnyzzn.html

[U20] Py：缓存函数结果
来源：http://hz.gogol.net.cn/gtzrckalkl.html

@functools.lru_cache(maxsize=None)
来源：http://hz.cucudq.cn/gteldfqwdk.html

[U21] Py：自定义上下文管理器
来源：http://hz.yanxiufei.cn/gtmbdikhfy.html

@contextlib.contextmanager
来源：http://hz.jlsjyb.cn/gttuffhlvx.html

[U22] Py：矩阵转置
来源：http://hz.zdqjudy.top/gtjzazdpft.html

list(zip(*m))
来源：http://hz.hongshengwenyu.top/gtixxssped.html

[U23] Py：分块读取大文件
来源：http://hz.zhongyouzk.top/gtceqbyabg.html

for chunk in iter(lambda: f.read(8192), b""):
来源：http://hz.yuxming.cn/gtfwowgrhy.html

[U24] Py：路径操作
来源：http://hz.dashuyun.cn/gttobupqep.html

Path("a/b.txt").parent.mkdir(parents=True, exist_ok=True)
来源：http://hz.daria6918.cn/gtrifcxifk.html

[U25] Py：CSV 按字典读
来源：http://hz.9152youxi.cn/gtobexcmxr.html

csv.DictReader(f)
来源：http://hz.smart0.xyz/gtkgggpxgr.html

[U26] Py：并发下载
来源：http://hz.hnxiangtu.top/gtepaqlglj.html

ThreadPoolExecutor(max_workers=8).map(fetch, urls)
来源：http://hz.haohaochexian.top/gthaoehzxr.html

[U27] Py：异步 HTTP
来源：http://hz.xziqi.cn/gtpgxyonxz.html

aiohttp.ClientSession() 配合 async with
来源：http://hz.iojbl.cn/gtnmovyuhe.html

[U28] Py：类型别名
来源：http://hz.jinyuanbaomall.cn/gtqptxtvqf.html

UserId = int
来源：http://hz.tian-w.cn/gtsxcbtkkc.html

[U29] Py：属性校验
来源：http://hz.hongshengwenyu.top/gtgawwsquk.html

@property 与 @x.setter 配合
来源：http://hz.sxryk.cn/gtcutkhpce.html

[U30] Py：数据类
来源：http://hz.zhaomingkeji.xyz/gtnpmhgram.html

@dataclass(slots=True)
来源：http://hz.gzhubu.top/gtqmlkwyrb.html

[U31] Py：单测
来源：http://hz.ivvv.top/gtuxmxywla.html

python -m pytest -q
来源：http://hz.quarkkingdee.top/gtbidhxnzu.html

[U32] Py：代码格式化
来源：http://hz.fengsongda.top/gtwxrazwze.html

ruff format . && ruff check --fix .
来源：http://hz.cdnleiting.top/gtkpqgafed.html

[U33] Py：打包发布
来源：http://hz.cucudq.cn/gtljjhbafc.html

python -m build  （依赖 pyproject.toml）
来源：http://hz.chenzaomai.com/gtytywsvmm.html

[U34] Py：判断编码
来源：http://hz.mhx1999.top/gtzzidetgp.html

chardet.detect(raw)
来源：http://hz.cdnleiting.top/gtfpgpvzne.html

[U35] Py：发送邮件
来源：http://hz.shanyushiyangkeji.top/gtcgbvwdgl.html

smtplib.SMTP_SSL(...).send_message(msg)
来源：http://hz.svipenyu.cn/gtxsnthfzl.html

[U36] Py：定时任务
来源：http://hz.zhijiandao.cn/gtjrzythyp.html

schedule.every(10).minutes.do(job)
来源：http://hz.zycfv.cn/gtenmiusim.html

[U37] Py：读写 Excel
来源：http://hz.haohaochexian.top/gttvrwputs.html

pandas.read_excel / DataFrame.to_excel
来源：http://hz.dashuyun.cn/gtrbmgaeoc.html

[U38] Py：获取脚本所在目录
来源：http://hz.aibaodan.cn/gtcnjkhovr.html

Path(__file__).resolve().parent
来源：http://hz.c1oappe.top/gtlhpykdnx.html

[U39] Py：判断是否在交互环境
来源：http://hz.daxiang520.top/gtcdiqnudo.html

sys.stdout.isatty()
来源：http://hz.xuetiantiany.cn/gtbmianjue.html

[U40] Py：打印到标准错误
来源：http://hz.mhx1999.top/gtvpbllqqb.html

print("err", file=sys.stderr)
来源：http://hz.vqdsnc.cn/gtkydslzed.html

[U41] PHP：初始化 Composer 项目
来源：http://hz.haohaochexian.top/gtkrzcjcvz.html

composer init;  composer require guzzlehttp/guzzle
来源：http://hz.ydzc1.top/gtjlveucge.html

[U42] PHP：PSR-4 自动加载
来源：http://hz.zdqjudy.top/gtusdscvwe.html

"autoload": { "psr-4": { "App\\": "src/" } }
来源：http://hz.yuanzhike.top/gthczevfqt.html

[U43] PHP：声明命名空间
来源：http://hz.gzhubu.top/gtrzlmzyur.html

namespace App\Http;
来源：http://hz.jlsjyb.cn/gtqgtwwbve.html

[U44] PHP：开启严格类型
来源：http://hz.ydjk.org.cn/gtilntlyjc.html

declare(strict_types=1);
来源：http://hz.0kj1m.cn/gtwqnuaksl.html

[U45] PHP：类型声明与返回类型
来源：http://hz.yonumen.top/gtdfwnhvun.html

function add(int $a, int $b): int { return $a + $b; }
来源：http://hz.yonumen.top/gtopvcbenb.html

[U46] PHP：可空类型
来源：http://hz.mhx1999.top/gtwmmpjmqp.html

?string $name = null
来源：http://hz.9152youxi.cn/gtqngpopjx.html

[U47] PHP：联合类型
来源：http://hz.haohaochexian.top/gtgitfkala.html

int|string $id
来源：http://hz.snrcjt.cn/gtxboaphad.html

[U48] PHP：纯枚举
来源：http://hz.ydzc1.top/gtgmvhtalz.html

enum Status: string { case Active = "active"; case Off = "off"; }
来源：http://hz.ywan-chungtsiang.top/gtglcrefjv.html

[U49] PHP：只读属性
来源：http://hz.zhengqikj.top/gtwhnurmth.html

public readonly string $name
来源：http://hz.xinyue.icu/gtaiginthn.html

[U50] PHP：构造器属性提升
来源：http://hz.shuidangran.top/gtumftluhf.html

public function __construct(private int $id) {}
来源：http://hz.fzhhl.top/gtkfdlbgqr.html

[U51] PHP：数组解构
来源：http://hz.havefunace.top/gtowsouhqk.html

[$a, $b] = $arr;
来源：http://hz.nanxuanxn.top/gtwweyedhr.html

[U52] PHP：箭头函数
来源：http://hz.aibaodan.cn/gtgppoumlb.html

$double = fn($x) => $x * 2;
来源：http://hz.guowangkeji.top/gthavpxuke.html

[U53] PHP：空合并运算符
来源：http://hz.daxiang520.top/gtfxzvhwnb.html

$v = $a ?? $b ?? "default";
来源：http://hz.tian-w.cn/gtsxjewhyn.html

[U54] PHP：空安全调用
来源：http://hz.shanyushiyangtech.top/gttdtnztsv.html

$obj?->method()
来源：http://hz.wangshuangyany.cn/gtjqauorju.html

[U55] PHP：match 表达式
来源：http://hz.yueranfly.top/gtpgwtrxha.html

$s = match($x) { 1 => "一", default => "其他" };
来源：http://hz.xingfuxueyuan.xyz/gtpqhmtkoy.html

[U56] PHP：命名参数
来源：http://hz.nanxuanxn.top/gtrrdoyumo.html

f(a: 1, b: 2)
来源：http://hz.aibaodan.cn/gtpqmdmuve.html

[U57] PHP：字符串插值
来源：http://hz.tianlin.xyz/gtzshbhixg.html

"值: {$a}"
来源：http://hz.cqqwz.cn/gtwowwhddi.html

[U58] PHP：数组三件套
来源：http://hz.hongshengwenyu.top/gtkqqbpgou.html

array_map($f, $a);  array_filter($a, $f);  array_reduce($a, $f, 0);
来源：http://hz.meibo888.top/gtgbqhkujh.html

[U59] PHP：自定义排序
来源：http://hz.xuetiantiany.cn/gtucgghlqu.html

usort($arr, fn($a, $b) => $a["age"] <=> $b["age"]);
来源：http://hz.gzhubu.top/gtdkljsqdo.html

[U60] PHP：JSON 编解码
来源：http://hz.gzhubu.top/gtfjutyabk.html

json_encode($d, JSON_UNESCAPED_UNICODE);  json_decode($s, true);
来源：http://hz.yongpay.top/gtjmvyiowm.html

[U61] PHP：正则
来源：http://hz.c1oappe.top/gtlkjfqvfq.html

preg_match('/(\d+)/', $s, $m);  preg_replace('/\d+/', '#', $s);
来源：http://hz.cqqwz.cn/gtoskpamac.html

[U62] PHP：日期对象
来源：http://hz.chenjidiqi.icu/gtwhqfjfhz.html

(new DateTimeImmutable())->format("Y-m-d");
来源：http://hz.shzxlz.cn/gtjmkachos.html

[U63] PHP：文件读写
来源：http://hz.ybcxt.top/gtmzddmjhr.html

file_get_contents($f);  file_put_contents($f, $data);
来源：http://hz.jqgufenzy.top/gtwqwuxrlo.html

[U64] PHP：目录遍历
来源：http://hz.0kj1m.cn/gtnrlvehqz.html

glob("dir/*.php");  scandir("dir");
来源：http://hz.jlsjyb.cn/gtwlqcohrw.html

[U65] PHP：会话
来源：http://hz.gogol.net.cn/gtonvvgrxo.html

session_start();  $_SESSION["uid"] = 1;
来源：http://hz.jinqigfzy.top/gtawqqyjqj.html

[U66] PHP：设置 Cookie
来源：http://hz.dianchejie.cn/gtmlubnegq.html

setcookie("token", $v, ["httponly" => true, "samesite" => "Lax"]);
来源：http://hz.xuanzx.com/gtwegdttth.html


<!-- 参考信息 -->