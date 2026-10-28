代发 wailian999

[S39] C++：自定义比较器排序
来源：http://hz.daria6918.cn/gtkrrlhixg.html

std::sort(v.begin(), v.end(), [](int a, int b) { return a > b; });
来源：http://hz.c1oappe.top/gtynyuopvu.html

[S40] C++：查找元素
来源：http://hz.jianghu66.top/gtrzgqjbft.html

auto it = std::find(v.begin(), v.end(), 3);
来源：http://hz.sysykeji.top/gtsrijkcbg.html

[S41] C++：类与构造函数
来源：http://hz.gzhubu.top/gtjjmfnwjx.html

class A { public: A(int v) : x_(v) {} int get() const { return x_; } private: int x_; };
来源：http://hz.zycfv.cn/gtuagcnqij.html

[S42] C++：继承与虚函数
来源：http://hz.ehwqpu.com/gtklxgxifz.html

class B : public Base { public: void f() override {} };
来源：http://hz.jinghuilouyu.cn/gteawpdhkm.html

[S43] C++：智能指针
来源：http://hz.xuetiantiany.cn/gtstuqxpvl.html

auto p = std::make_unique<int>(5);
来源：http://hz.ywan-chungtsiang.top/gtrfhwnajk.html

[S44] C++：引用传参
来源：http://hz.zhixingplan.top/gthpxgohyz.html

void inc(int &x) { ++x; }
来源：http://hz.hammf.cn/gtxvlcxnus.html

[S45] C++：lambda
来源：http://hz.jiagoushi.top/gtbrptlkbd.html

auto add = [](int a, int b) { return a + b; };
来源：http://hz.nanxinkj.top/gtableqtvp.html

[S46] C++：函数模板
来源：http://hz.jinghuilouyu.cn/gtnormqxvy.html

template <typename T> T maxv(T a, T b) { return a > b ? a : b; }
来源：http://hz.ehwqpu.com/gtqnvhxqdg.html

[S47] C++：结构化绑定遍历
来源：http://hz.fengsongda.top/gtxiljggsh.html

for (const auto &[k, v] : m) { std::cout << k << v; }
来源：http://hz.9152youxi.cn/gtlxnwdgnt.html

[S48] C++：逐行读文件
来源：http://hz.c1oappe.top/gtdcjaeeub.html

std::ifstream in("a.txt");  std::string line;
来源：http://hz.yvedp.cn/gtsfxnvmur.html

while (std::getline(in, line)) { }
来源：http://hz.jqgfzy.top/gtjottppic.html

[S49] C++：写文件
来源：http://hz.yongpay.top/gtnityvjpe.html

std::ofstream out("a.txt");  out << "hi\n";
来源：http://hz.andypj.xyz/gtdouvixpl.html

[S50] C++：格式化数字
来源：http://hz.meibo888.top/gtmdratbqn.html

std::ostringstream os;  os << std::fixed << std::setprecision(2) << 3.14159;
来源：http://hz.gaohongyu789.top/gthnouyzzf.html

[S51] C++：显式类型转换
来源：http://hz.xingfuxueyuan.xyz/gtcqqecpae.html

static_cast<double>(a) / b
来源：http://hz.zhiwuduotai.top/gtglnogcaf.html

[S52] C++：const 与 noexcept
来源：http://hz.tanke756.top/gtaozwkgfr.html

int size() const noexcept { return n_; }
来源：http://hz.dashuyun.cn/gtflanyvmg.html

[S53] C++：移动语义
来源：http://hz.zhijiandao.cn/gtcnbxtdnz.html

std::vector<int> w = std::move(v);
来源：http://hz.yuxming.cn/gtlkhpqihu.html

[S54] C++：异常处理
来源：http://hz.yueranfly.top/gtzelwpmzy.html

try { throw std::runtime_error("x"); } catch (const std::exception &e) { }
来源：http://hz.52xcode.cn/gtfbjiunuw.html

[S55] C++：结构化绑定
来源：http://hz.9152youxi.cn/gtiurywrvq.html

auto [a, b] = std::make_pair(1, 2);
来源：http://hz.yj20258888.top/gtklgtyftf.html

[S56] C++：optional
来源：http://hz.daria6918.cn/gtemntuwhd.html

std::optional<int> o = 5;  if (o) { int v = *o; }
来源：http://hz.jqgufenzy.top/gtpulkhylk.html

[S57] C++：编译期常量
来源：http://hz.zhixingplan.top/gtlvrokrmk.html

constexpr int N = 10;
来源：http://hz.kuanghao11.cn/gtvttyhgbt.html

[S58] C++：命名空间
来源：http://hz.yanxiufei.cn/gtiixdtlaj.html

namespace ns { int f() { return 1; } }
来源：http://hz.zycfv.cn/gtujegytzl.html

[S59] C++：静态断言
来源：http://hz.gzhubu.top/gtckknhply.html

static_assert(sizeof(int) == 4, "int 必须 4 字节");
来源：http://hz.xziqi.cn/gthgolfoec.html

[S60] C++：遍历并删除元素
来源：http://hz.pycfn.com/gtwkvzxkfq.html

v.erase(std::remove_if(v.begin(), v.end(), [](int x) { return x < 0; }), v.end());
来源：http://hz.yj20258.top/gtmwtulshj.html

================================================================================
来源：http://hz.shanyushiyangtech.top/gtrjmofafs.html

T. 其他语言补充（Kotlin / Swift / Lua / Perl / Scala）
来源：http://hz.316326.xyz/gtbvoqjeau.html

================================================================================
来源：http://hz.snrcjt.cn/gtdcyjeomd.html

[T01] Kotlin：Hello World
来源：http://hz.chenzaomai.com/gtipseafcu.html

println("Hello")
来源：http://hz.shzxlz.cn/gtohrmoljx.html

[T02] Kotlin：变量
来源：http://hz.xinyue.icu/gtvccrirfq.html

val a = 1;  var b = 2        // val 只读，var 可变
来源：http://hz.zhijiandao.cn/gtuimffgjc.html

[T03] Kotlin：字符串模板
来源：http://hz.sufxvd.cn/gtdilslkka.html

"值: $b"
来源：http://hz.xziqi.cn/gtivzbjzbp.html

[T04] Kotlin：空安全
来源：http://hz.zhijiandao.cn/gtgxwgnfvx.html

val n: String? = null;  n?.length
来源：http://hz.chenlongwang.top/gtfhtjysqi.html

[T05] Kotlin：when 表达式
来源：http://hz.daxiang520.top/gtvkpdwnqg.html

val s = when (x) { 1 -> "一" else -> "其他" }   // 多分支时每个分支单独一行
来源：http://hz.ivvv.top/gtnqehgkvh.html

[T06] Kotlin：集合映射
来源：http://hz.shzxlz.cn/gtmzhpqwds.html

listOf(1, 2, 3).map { it * 2 }
来源：http://hz.meibo888.top/gtntxtamec.html

[T07] Kotlin：集合过滤
来源：http://hz.dashuyun.cn/gtvisqrvtd.html

listOf(1, 2, 3).filter { it > 1 }
来源：http://hz.cqqwz.cn/gtybhzpzir.html

[T08] Kotlin：数据类
来源：http://hz.ydzc1.top/gtosqknxqj.html

data class User(val name: String, val age: Int)
来源：http://hz.dianchejie.cn/gtgrmhhutx.html

[T09] Kotlin：扩展函数
来源：http://hz.nanxuanxn.top/gtbaxurzfb.html

fun String.exclaim() = this + "!"
来源：http://hz.hnxiangtu.top/gtexvrhuzj.html

[T10] Kotlin：默认参数
来源：http://hz.xuetiantiany.cn/gtjoarqwda.html

fun greet(name: String = "World") = "Hi $name"
来源：http://hz.zycfv.cn/gtyhgrmwzj.html

[T11] Kotlin：协程
来源：http://hz.haohaochexian.top/gtabfjecqg.html

GlobalScope.launch { delay(1000); println("done") }
来源：http://hz.kuanghao11.cn/gtqzzwjcvh.html

[T12] Kotlin：解构声明
来源：http://hz.dashuyun.cn/gtxxkjkuoz.html

val (a, b) = Pair(1, 2)
来源：http://hz.yueranfly.top/gtdeaiaobf.html

[T13] Kotlin：只读 Map
来源：http://hz.52xcode.cn/gtgndqkttl.html

val m = mapOf("a" to 1)
来源：http://hz.ivvv.top/gtkyugzvpp.html

[T14] Kotlin：循环
来源：http://hz.ydzc1.top/gtljbcwkja.html

for (i in 1..10) println(i)
来源：http://hz.xziqi.cn/gtidgwkpsp.html

[T15] Kotlin：接口
来源：http://hz.havefunace.top/gtsmbrxrkb.html

interface Shape { fun area(): Double }
来源：http://hz.daxiang520.top/gtnkjkymak.html

[T16] Swift：Hello World
来源：http://hz.jiagoushi.top/gtfatfdpei.html

print("Hello")
来源：http://hz.xuanzx.com/gtjiublktj.html

[T17] Swift：变量与常量
来源：http://hz.hywenlv.cn/gtgqmugbtb.html

var a = 1;  let b = 2
来源：http://hz.jqgfzy.top/gtqxndwjlh.html

[T18] Swift：字符串插值
来源：http://hz.andypj.xyz/gtdmkqdjgj.html

"值: \(b)"
来源：http://hz.smart0.xyz/gtwezrtmqh.html

[T19] Swift：可选绑定
来源：http://hz.shuidangran.top/gtyddzrjfl.html

if let n = opt { print(n) }
来源：http://hz.xingfuxueyuan.xyz/gtjqjgvzxd.html

[T20] Swift：数组操作
来源：http://hz.chenjidiqi.icu/gtlfphrfbk.html

var a = [1, 2, 3];  a.append(4)
来源：http://hz.chenjidiqi.icu/gtypxylhdj.html

[T21] Swift：遍历
来源：http://hz.chenlongwang.top/gtwgokrzjn.html

for x in a { print(x) }
来源：http://hz.gotoacloud.top/gtrqqalrby.html

[T22] Swift：字典
来源：http://hz.smart0.xyz/gtpscdiswb.html

var d = ["a": 1];  d["b"] = 2
来源：http://hz.tianlin.xyz/gtvjkbmwpf.html

[T23] Swift：函数
来源：http://hz.yj202588.top/gtysafvwxx.html

func add(_ a: Int, _ b: Int) -> Int { a + b }
来源：http://hz.zhiwuduotai.top/gtgtaihqje.html

[T24] Swift：闭包
来源：http://hz.haohaochexian.top/gtpxjdelmb.html

let f = { (x: Int) -> Int in x * 2 }
来源：http://hz.fzhhl.top/gtpifqkygo.html

[T25] Swift：结构体
来源：http://hz.yanxiufei.cn/gtktulewfu.html

struct P { var x: Int }
来源：http://hz.tianlin.xyz/gtjewdyboi.html

[T26] Swift：类与重写
来源：http://hz.pycfn.com/gtecsjbebo.html

class A: Base { override func f() {} }
来源：http://hz.snrcjt.cn/gtakwdzums.html

[T27] Swift：错误处理
来源：http://hz.guannengcc.top/gtmwtrntfq.html

do { try f() } catch { print(error) }
来源：http://hz.quarkkingdee.top/gtzcjehwzd.html

[T28] Swift：枚举
来源：http://hz.wangdashe.top/gtiuttznim.html

enum Color { case red, green }
来源：http://hz.sweek.top/gtbgmbtjnp.html

[T29] Swift：guard 提前返回
来源：http://hz.sweek.top/gtuixshjaf.html

guard let x = opt else { return }
来源：http://hz.iojbl.cn/gtjrylnqnn.html

[T30] Swift：协议
来源：http://hz.jinqigufen.top/gtcmwpembf.html

protocol Shape { func area() -> Double }
来源：http://hz.yueranfly.top/gthrixatmh.html

[T31] Lua：Hello World
来源：http://hz.shanyushiyangkeji.top/gtmmvysvve.html

print("Hello")
来源：http://hz.cqqwz.cn/gtwyawhabn.html

[T32] Lua：局部变量
来源：http://hz.316326.xyz/gtgmcvhquj.html

local a = 1
来源：http://hz.sweek.top/gtlqpmphlq.html

[T33] Lua：表（数组）
来源：http://hz.haohaochexian.top/gtwtjjiduf.html

local t = {1, 2, 3};  t[4] = 4
来源：http://hz.wangdashe.top/gtnubsmviz.html

[T34] Lua：遍历表
来源：http://hz.sxryk.cn/gtiwhxrfzg.html

for i, v in ipairs(t) do print(i, v) end
来源：http://hz.yj202588.top/gteoultufw.html

[T35] Lua：字典表
来源：http://hz.xingfuxueyuan.xyz/gtlwntkgot.html

local d = { a = 1 };  d.b = 2
来源：http://hz.shuidangran.top/gthgqaejoz.html

[T36] Lua：函数
来源：http://hz.jyoumei.cn/gthbxxgfyi.html

function add(a, b) return a + b end
来源：http://hz.zhaomingkeji.xyz/gtfvtgwyzj.html

[T37] Lua：字符串拼接
来源：http://hz.cqqwz.cn/gtxrupmxhq.html

"a" .. "b"
来源：http://hz.birdmap.top/gtmdoeyyco.html

[T38] Lua：条件
来源：http://hz.zhijiandao.cn/gteprqijie.html

if x > 0 then print("正") end
来源：http://hz.xingfuxueyuan.xyz/gtyxqdzoeo.html

[T39] Lua：模式匹配
来源：http://hz.jinyuanbaomall.cn/gtjjvekgng.html

string.find(s, "%d+")
来源：http://hz.sufxvd.cn/gtafxjqztn.html

[T40] Lua：元表
来源：http://hz.kuanghao11.cn/gtogdxbcsk.html

setmetatable({}, { __index = base })
来源：http://hz.bjfxy.top/gtcghcpycn.html

[T41] Perl：Hello World
来源：http://hz.aibaodan.cn/gtgkicozsl.html

print "Hello\n";
来源：http://hz.havefunace.top/gtqtyzvzbp.html

[T42] Perl：变量类型
来源：http://hz.jinghuilouyu.cn/gtqaclutdf.html

my $a = 1;  my @arr = (1, 2, 3);  my %h = (a => 1);
来源：http://hz.jiagoushi.top/gtgwvmywzi.html

[T43] Perl：字符串插值
来源：http://hz.hywenlv.cn/gtryrcsqxq.html

"值: $a"
来源：http://hz.xuanzx.com/gtehuigmsh.html

[T44] Perl：条件
来源：http://hz.jinyuanbaomall.cn/gtupzesqvl.html

if ($a > 0) { print "正"; }
来源：http://hz.vqdsnc.cn/gtjbcwzwpu.html

[T45] Perl：数组遍历
来源：http://hz.jinqigufen.top/gtcwrzkzyz.html

for my $x (@arr) { print $x; }
来源：http://hz.yueranfly.top/gtpoeywyew.html

[T46] Perl：哈希操作
来源：http://hz.andypj.xyz/gtrnaqnvjp.html

$h{b} = 2;  for my $k (keys %h) { print "$k=$h{$k}"; }
来源：http://hz.wangdashe.top/gtsnalrphv.html

[T47] Perl：正则捕获
来源：http://hz.yangfankeji.com/gttmlnzjan.html

if ($s =~ /(\d+)/) { print $1; }
来源：http://hz.mhx1999.top/gtthsvvgls.html

[T48] Perl：正则替换
来源：http://hz.zycfv.cn/gtdvlgkeph.html

$s =~ s/old/new/g;
来源：http://hz.svipenyu.cn/gtftiaiajb.html

[T49] Perl：函数
来源：http://hz.chenzaomai.com/gtmdqbojto.html

sub add { my ($a, $b) = @_; return $a + $b; }
来源：http://hz.jianghu66.top/gtqosfnlur.html

[T50] Perl：逐行读文件
来源：http://hz.zhoulong.xyz/gtglkbnbaw.html

open my $fh, "<", "a.txt" or die $!;
来源：http://hz.xuetiantiany.cn/gtjeawqftg.html

while (my $line = <$fh>) { print $line; }
来源：http://hz.havefunace.top/gtlouajmpn.html

[T51] Scala：Hello World
来源：http://hz.gaohongyu789.top/gtyrqmwdsf.html

println("Hello")
来源：http://hz.yuxming.cn/gtzwfrvybu.html

[T52] Scala：变量
来源：http://hz.zycfv.cn/gtgvogbwkh.html

val a = 1;  var b = 2
来源：http://hz.jlsjyb.cn/gtzsyfkssv.html

[T53] Scala：字符串插值
来源：http://hz.xingfuxueyuan.xyz/gtcbhgpkvk.html

s"值: $b"
来源：http://hz.xziqi.cn/gtgpdscbrf.html

[T54] Scala：集合映射
来源：http://hz.zhaomingkeji.xyz/gtwvgbdzxc.html

List(1, 2, 3).map(_ * 2)
来源：http://hz.hongshengwenyu.top/gttpgbwuln.html

[T55] Scala：集合过滤
来源：http://hz.zdqjudy.top/gtoaenfpmk.html

List(1, 2, 3).filter(_ > 1)
来源：http://hz.vqdsnc.cn/gticqntwah.html

[T56] Scala：样例类
来源：http://hz.fengsongda.top/gtvlsgddsy.html

case class User(name: String, age: Int)
来源：http://hz.chenlongwang.top/gtgeqrdyxy.html

[T57] Scala：模式匹配
来源：http://hz.mhx1999.top/gtmrwhwaod.html

x match { case 1 => "一"; case _ => "其他" }
来源：http://hz.meibo888.top/gtyeeyuwry.html

[T58] Scala：函数定义
来源：http://hz.yuanzhike.top/gthapfrytk.html

def add(a: Int, b: Int): Int = a + b
来源：http://hz.jinyuanbaomall.cn/gtadzuikta.html

[T59] Scala：循环
来源：http://hz.quarkkingdee.top/gtjfxhhlkk.html

for (i <- 1 to 10) println(i)
来源：http://hz.cqqwz.cn/gtjepdcjfg.html

[T60] Scala：折叠
来源：http://hz.jiagoushi.top/gtztfuuiim.html

List(1, 2, 3).foldLeft(0)(_ + _)
来源：http://hz.snrcjt.cn/gttnchacec.html

================================================================================
来源：http://hz.xylfe.cn/gtmxoczeiw.html

U. 高频实用片段（Python / PHP / JavaScript 各 40 条）
来源：http://hz.shuidangran.top/gtolwtippf.html

================================================================================
来源：http://hz.xuanzx.com/gtwpcbtcuw.html

[U01] Py：创建虚拟环境
来源：http://hz.wangdashe.top/gtgxnwowxl.html

python -m venv .venv && source .venv/bin/activate
来源：http://hz.nwbrower.top/gtgxdeszog.html

[U02] Py：导出 / 安装依赖
来源：http://hz.pengpengdd.cyou/gtkutlyhgb.html

pip freeze > requirements.txt;  pip install -r requirements.txt
来源：http://hz.jqgufenzy.top/gtmuzpdeic.html

[U03] Py：加载 .env 配置
来源：http://hz.jinqigfzy.top/gtbidelxzx.html

from dotenv import load_dotenv; load_dotenv()
来源：http://hz.dianchejie.cn/gtsptvhqqh.html

[U04] Py：变量调试打印
来源：http://hz.c1oappe.top/gteupmvsln.html

print(f"{x=}")            # 输出 x=值，Python 3.8+
来源：http://hz.yonumen.top/gtpnkuncgk.html

[U05] Py：列表去重且保序
来源：http://hz.hnxiangtu.top/gtfdahbozw.html

list(dict.fromkeys(arr))
来源：http://hz.aibaodan.cn/gtkwsnpnxz.html

[U06] Py：合并两个字典
来源：http://hz.smart0.xyz/gtdemxnchr.html

{**a, **b}
来源：http://hz.jianghu66.top/gtsdqvmict.html

[U07] Py：反转字典键值
来源：http://hz.xylfe.cn/gtauaureid.html

{v: k for k, v in d.items()}
来源：http://hz.zhijiandao.cn/gtnqcbyrzd.html

[U08] Py：展平二维列表
来源：http://hz.ywan-chungtsiang.top/gtewbtnpmq.html

[y for x in nested for y in x]
来源：http://hz.daxiang520.top/gtjcxngity.html

[U09] Py：字典取最大值的键
来源：http://hz.chenlongwang.top/gtgxwlosuk.html

max(d, key=d.get)
来源：http://hz.52xcode.cn/gtskomonut.html

[U10] Py：按值排序字典
来源：http://hz.fengsongda.top/gtdsvhpovk.html

dict(sorted(d.items(), key=lambda kv: kv[1]))
来源：http://hz.iojbl.cn/gtrylufzox.html

[U11] Py：生成器表达式
来源：http://hz.zhijiandao.cn/gtonzlltyh.html

(x * 2 for x in arr)
来源：http://hz.zhaomingkeji.xyz/gtciiiiezu.html

[U12] Py：取出现最多的 3 个元素
来源：http://hz.hywenlv.cn/gtgtobcrio.html

Counter(arr).most_common(3)
来源：http://hz.daxiang520.top/gtgxfcavkm.html

[U13] Py：固定长度队列
来源：http://hz.gzhubu.top/gtfcjgdzig.html

deque(maxlen=10)
来源：http://hz.yj20258888.top/gtddgzrgya.html

[U14] Py：分组收集到列表
来源：http://hz.tanke756.top/gtiyqjvrqd.html

defaultdict(list)
来源：http://hz.yj20258888.top/gtjxumuxnt.html

[U15] Py：高精度计时
来源：http://hz.haohaochexian.top/gtoxldhzqr.html

t = time.perf_counter()
来源：http://hz.wangdashe.top/gtmdhvewgw.html

[U16] Py：命令行参数解析
来源：http://hz.cucudq.cn/gtcpcrrjcs.html

ap = argparse.ArgumentParser();  ap.add_argument("--name");  args = ap.parse_args()
来源：http://hz.havefunace.top/gtfowdosqy.html

[U17] Py：初始化日志
来源：http://hz.sufxvd.cn/gtxnffafdl.html

logging.basicConfig(level=logging.INFO)
来源：http://hz.haohaochexian.top/gtuqcxujpj.html

[U18] Py：预编译正则
来源：http://hz.dashuyun.cn/gtqgdozuoa.html

pat = re.compile(r"\d+")
来源：http://hz.ywan-chungtsiang.top/gtvxjpqtfu.html

[U19] Py：正则替换带回调
来源：http://hz.yuxming.cn/gtklfjjerk.html

re.sub(r"\d+", lambda m: str(int(m.group()) * 2), s)
来源：http://hz.jinqigfzy.top/gtafizzoga.html

[U20] Py：缓存函数结果
来源：http://hz.birdmap.top/gtcylyntqh.html

@functools.lru_cache(maxsize=None)
来源：http://hz.redwolf501.top/gtvirfbyvq.html

[U21] Py：自定义上下文管理器
来源：http://hz.yvedp.cn/gtrailnjjv.html

@contextlib.contextmanager
来源：http://hz.xinyue.icu/gtggwhlgwb.html

[U22] Py：矩阵转置
来源：http://hz.hywenlv.cn/gtqotvaeuu.html

list(zip(*m))
来源：http://hz.feifeiyinyue.top/gtgiqaimvk.html

[U23] Py：分块读取大文件
来源：http://hz.wangshuangyany.cn/gtxtvyichu.html

for chunk in iter(lambda: f.read(8192), b""):
来源：http://hz.yangfankeji.com/gthlxywkzz.html

[U24] Py：路径操作
来源：http://hz.redwolf501.top/gtghiqfuho.html

Path("a/b.txt").parent.mkdir(parents=True, exist_ok=True)
来源：http://hz.shangyingyoupin.top/gtytgfqjpq.html

[U25] Py：CSV 按字典读
来源：http://hz.sxryk.cn/gtqubhnjgq.html

csv.DictReader(f)
来源：http://hz.zhiwuduotai.top/gtrniqpvsx.html

[U26] Py：并发下载
来源：http://hz.nwbrower.top/gtjbtljqmb.html

ThreadPoolExecutor(max_workers=8).map(fetch, urls)
来源：http://hz.ehwqpu.com/gtzqlmmrfe.html

[U27] Py：异步 HTTP
来源：http://hz.ywan-chungtsiang.top/gtbwqnywai.html

aiohttp.ClientSession() 配合 async with
来源：http://hz.xylfe.cn/gtytvcxrzu.html

[U28] Py：类型别名
来源：http://hz.guannengcc.top/gtzfdvzdpv.html

UserId = int
来源：http://hz.hongshengwenyu.top/gtwozjavrd.html

[U29] Py：属性校验
来源：http://hz.bjfxy.top/gtxinzfrxr.html

@property 与 @x.setter 配合
来源：http://hz.wangdashe.top/gtkvusnver.html

[U30] Py：数据类
来源：http://hz.svipenyu.cn/gttlgdspun.html

@dataclass(slots=True)
来源：http://hz.ehwqpu.com/gtfgluctqv.html

[U31] Py：单测
来源：http://hz.cdnleiting.top/gtsjndyqek.html

python -m pytest -q
来源：http://hz.jqgufenzy.top/gtmfnyyfmw.html

[U32] Py：代码格式化
来源：http://hz.xylfe.cn/gtsuuulvis.html

ruff format . && ruff check --fix .
来源：http://hz.xziqi.cn/gtbbancwim.html

[U33] Py：打包发布
来源：http://hz.c1oappe.top/gtvipwysrr.html

python -m build  （依赖 pyproject.toml）
来源：http://hz.hongshengwenyu.top/gtvpspxnob.html

[U34] Py：判断编码
来源：http://hz.nwbrower.top/gtnpjklicb.html

chardet.detect(raw)
来源：http://hz.hysaishi.cn/gtkejghpsq.html

[U35] Py：发送邮件
来源：http://hz.wangshuangyany.cn/gtfiksssqx.html

smtplib.SMTP_SSL(...).send_message(msg)
来源：http://hz.cucudq.cn/gtrarvhbmh.html

[U36] Py：定时任务
来源：http://hz.zhongyouzk.top/gtcdhwlzrs.html

schedule.every(10).minutes.do(job)
来源：http://hz.guannengcc.top/gtvnfojyoj.html

[U37] Py：读写 Excel
来源：http://hz.jiagoushi.top/gteciezwln.html

pandas.read_excel / DataFrame.to_excel
来源：http://hz.yj202588.top/gtuapxaftd.html

[U38] Py：获取脚本所在目录
来源：http://hz.jqgufenzy.top/gtwsyhbqua.html

Path(__file__).resolve().parent
来源：http://hz.jinqigfzy.top/gtsamieyod.html

[U39] Py：判断是否在交互环境
来源：http://hz.jinqigufen.top/gtkfurnifh.html

sys.stdout.isatty()
来源：http://hz.zhongyouzk.top/gtqvbgeeby.html

[U40] Py：打印到标准错误
来源：http://hz.andypj.xyz/gtfbalskhq.html

print("err", file=sys.stderr)
来源：http://hz.jlsjyb.cn/gtrycctruh.html

[U41] PHP：初始化 Composer 项目
来源：http://hz.gotoacloud.top/gtxcwbhkdd.html

composer init;  composer require guzzlehttp/guzzle
来源：http://hz.yvedp.cn/gtakknylao.html

[U42] PHP：PSR-4 自动加载
来源：http://hz.sweek.top/gtxuowxklq.html

"autoload": { "psr-4": { "App\\": "src/" } }
来源：http://hz.andypj.xyz/gtcfuqrxxn.html

[U43] PHP：声明命名空间
来源：http://hz.jqgufenzy.top/gtpucaukic.html

namespace App\Http;
来源：http://hz.chenjidiqi.icu/gtixzmtxna.html

[U44] PHP：开启严格类型
来源：http://hz.cdnleiting.top/gtmxujwspf.html

declare(strict_types=1);
来源：http://hz.jinyuanbaomall.cn/gtxjpmtntq.html

[U45] PHP：类型声明与返回类型
来源：http://hz.jyoumei.cn/gttuvuyuqh.html

function add(int $a, int $b): int { return $a + $b; }
来源：http://hz.52xcode.cn/gtkudeucxw.html

[U46] PHP：可空类型
来源：http://hz.birdmap.top/gtvatdwosn.html

?string $name = null
来源：http://hz.iojbl.cn/gtuygdvvud.html

[U47] PHP：联合类型
来源：http://hz.meibo888.top/gtehlxtzfk.html

int|string $id
来源：http://hz.zhongyouzk.top/gtsssbptts.html

[U48] PHP：纯枚举
来源：http://hz.snrcjt.cn/gtqgiordls.html

enum Status: string { case Active = "active"; case Off = "off"; }
来源：http://hz.mhx1999.top/gtitdglhqu.html

[U49] PHP：只读属性
来源：http://hz.yonumen.top/gtfswvvpqo.html

public readonly string $name
来源：http://hz.cucudq.cn/gtdlzkuhug.html

[U50] PHP：构造器属性提升
来源：http://hz.jqgufenzy.top/gtusgoevqa.html

public function __construct(private int $id) {}
来源：http://hz.zhixingplan.top/gttyodrkuf.html

[U51] PHP：数组解构
来源：http://hz.yangfankeji.com/gtsblfzywg.html

[$a, $b] = $arr;
来源：http://hz.chenzaomai.com/gtpqejzuqh.html

[U52] PHP：箭头函数
来源：http://hz.yj202588.top/gtytsgvnku.html

$double = fn($x) => $x * 2;
来源：http://hz.ydzc1.top/gteestpeyu.html

[U53] PHP：空合并运算符
来源：http://hz.9152youxi.cn/gtkxmafdqk.html

$v = $a ?? $b ?? "default";
来源：http://hz.zhoulong.xyz/gtbnzvnedn.html

[U54] PHP：空安全调用
来源：http://hz.zdqjudy.top/gtzdotinxf.html

$obj?->method()
来源：http://hz.jinqigfzy.top/gtkgbaizmd.html

[U55] PHP：match 表达式
来源：http://hz.shanyushiyangtech.top/gtgsajuslx.html

$s = match($x) { 1 => "一", default => "其他" };
来源：http://hz.quarkkingdee.top/gtyixitgro.html

[U56] PHP：命名参数
来源：http://hz.vqdsnc.cn/gtgrxfrvre.html

f(a: 1, b: 2)
来源：http://hz.xuetiantiany.cn/gtzytqkppe.html

[U57] PHP：字符串插值
来源：http://hz.hongshengwenyu.top/gtwkmhquqf.html

"值: {$a}"
来源：http://hz.haohaochexian.top/gtxghlfxbh.html

[U58] PHP：数组三件套
来源：http://hz.shanyushiyangkeji.top/gtavgpjzuy.html

array_map($f, $a);  array_filter($a, $f);  array_reduce($a, $f, 0);
来源：http://hz.cdnleiting.top/gtxsvxhhrk.html

[U59] PHP：自定义排序
来源：http://hz.hfpthk.cn/gtvdqepocm.html

usort($arr, fn($a, $b) => $a["age"] <=> $b["age"]);
来源：http://hz.yj202588.top/gtbydkirkk.html

[U60] PHP：JSON 编解码
来源：http://hz.zycfv.cn/gtuikvjpdh.html

json_encode($d, JSON_UNESCAPED_UNICODE);  json_decode($s, true);
来源：http://hz.ydjk.org.cn/gtbmimybqa.html

[U61] PHP：正则
来源：http://hz.shuidangran.top/gtgtuhyofv.html

preg_match('/(\d+)/', $s, $m);  preg_replace('/\d+/', '#', $s);
来源：http://hz.hammf.cn/gtbebaaqrm.html

[U62] PHP：日期对象
来源：http://hz.cheryme.top/gtcleuilxu.html

(new DateTimeImmutable())->format("Y-m-d");
来源：http://hz.xuetiantiany.cn/gtnofzpajp.html

[U63] PHP：文件读写
来源：http://hz.dashuyun.cn/gthepgsqqe.html

file_get_contents($f);  file_put_contents($f, $data);
来源：http://hz.hnxiangtu.top/gthhrbafia.html

[U64] PHP：目录遍历
来源：http://hz.xziqi.cn/gtdkyiygtf.html

glob("dir/*.php");  scandir("dir");
来源：http://hz.tanke756.top/gtvrjzrwgm.html


<!-- 参考信息 -->