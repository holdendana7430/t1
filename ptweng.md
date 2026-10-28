代发 wailian999

[S41] C++：类与构造函数
来源：http://hz.hongshengwenyu.top/gtjxdcbsby.html

class A { public: A(int v) : x_(v) {} int get() const { return x_; } private: int x_; };
来源：http://hz.xuetiantiany.cn/gtslkphkjf.html

[S42] C++：继承与虚函数
来源：http://hz.nanxuanxn.top/gtzibmhvtq.html

class B : public Base { public: void f() override {} };
来源：http://hz.yj20258.top/gtlrtbzgxo.html

[S43] C++：智能指针
来源：http://hz.pycfn.com/gtpkujhypt.html

auto p = std::make_unique<int>(5);
来源：http://hz.xuanzx.com/gtrsqvpntb.html

[S44] C++：引用传参
来源：http://hz.jiagoushi.top/gtmxwagzje.html

void inc(int &x) { ++x; }
来源：http://hz.hywenlv.cn/gtywecjskc.html

[S45] C++：lambda
来源：http://hz.wangshuangyany.cn/gtydlfctes.html

auto add = [](int a, int b) { return a + b; };
来源：http://hz.hongshengwenyu.top/gtwnaadgzz.html

[S46] C++：函数模板
来源：http://hz.nwbrower.top/gtgysybkya.html

template <typename T> T maxv(T a, T b) { return a > b ? a : b; }
来源：http://hz.jqgfzy.top/gtbvrwdzji.html

[S47] C++：结构化绑定遍历
来源：http://hz.jlsjyb.cn/gtgiuuxtpp.html

for (const auto &[k, v] : m) { std::cout << k << v; }
来源：http://hz.cqqwz.cn/gtljbdlqct.html

[S48] C++：逐行读文件
来源：http://hz.zhoulong.xyz/gtyjpuczpr.html

std::ifstream in("a.txt");  std::string line;
来源：http://hz.ehwqpu.com/gtxuyrhqgw.html

while (std::getline(in, line)) { }
来源：http://hz.hammf.cn/gtbwkzttpb.html

[S49] C++：写文件
来源：http://hz.hysaishi.cn/gtmxenhjxn.html

std::ofstream out("a.txt");  out << "hi\n";
来源：http://hz.feifeiyinyue.top/gtrsnsprnl.html

[S50] C++：格式化数字
来源：http://hz.cucudq.cn/gtbnrofwda.html

std::ostringstream os;  os << std::fixed << std::setprecision(2) << 3.14159;
来源：http://hz.chenlongwang.top/gtbieksnnn.html

[S51] C++：显式类型转换
来源：http://hz.mhx1999.top/gtvhrvfrmv.html

static_cast<double>(a) / b
来源：http://hz.fzhhl.top/gtpszvbofe.html

[S52] C++：const 与 noexcept
来源：http://hz.xinyue.icu/gtbktecryj.html

int size() const noexcept { return n_; }
来源：http://hz.aizwys.cn/gtbvvlgpkw.html

[S53] C++：移动语义
来源：http://hz.sysykeji.top/gtiygllpqo.html

std::vector<int> w = std::move(v);
来源：http://hz.sufxvd.cn/gtmybbjjly.html

[S54] C++：异常处理
来源：http://hz.yangfankeji.com/gtqgtmitgg.html

try { throw std::runtime_error("x"); } catch (const std::exception &e) { }
来源：http://hz.fzhhl.top/gtxhnchjpu.html

[S55] C++：结构化绑定
来源：http://hz.jinqigufen.top/gtsahleicu.html

auto [a, b] = std::make_pair(1, 2);
来源：http://hz.tanke756.top/gtzmujbnop.html

[S56] C++：optional
来源：http://hz.xuanzx.com/gtclroazrf.html

std::optional<int> o = 5;  if (o) { int v = *o; }
来源：http://hz.ivvv.top/gtyrrgzlnv.html

[S57] C++：编译期常量
来源：http://hz.jinghuilouyu.cn/gtartyhdkd.html

constexpr int N = 10;
来源：http://hz.fzhhl.top/gtlsxobrjq.html

[S58] C++：命名空间
来源：http://hz.birdmap.top/gtkjcryvab.html

namespace ns { int f() { return 1; } }
来源：http://hz.xylfe.cn/gtshbptwlr.html

[S59] C++：静态断言
来源：http://hz.zdqjudy.top/gtngantbjw.html

static_assert(sizeof(int) == 4, "int 必须 4 字节");
来源：http://hz.ehwqpu.com/gtoagtqaag.html

[S60] C++：遍历并删除元素
来源：http://hz.fzhhl.top/gtwxyfexwj.html

v.erase(std::remove_if(v.begin(), v.end(), [](int x) { return x < 0; }), v.end());
来源：http://hz.0kj1m.cn/gtzgnvfqej.html

================================================================================
来源：http://hz.jinyuanbaomall.cn/gtmbqusral.html

T. 其他语言补充（Kotlin / Swift / Lua / Perl / Scala）
来源：http://hz.9152youxi.cn/gtfoarpkct.html

================================================================================
来源：http://hz.yj20258.top/gtpdzubppn.html

[T01] Kotlin：Hello World
来源：http://hz.andypj.xyz/gthlrjpwtn.html

println("Hello")
来源：http://hz.shanyushiyangtech.top/gtmwbjebwv.html

[T02] Kotlin：变量
来源：http://hz.shanyushiyangkeji.top/gtpvamgedp.html

val a = 1;  var b = 2        // val 只读，var 可变
来源：http://hz.sxryk.cn/gtvscqhpua.html

[T03] Kotlin：字符串模板
来源：http://hz.nanxuanxn.top/gtpjqwrdxy.html

"值: $b"
来源：http://hz.xylfe.cn/gtmnxuftbk.html

[T04] Kotlin：空安全
来源：http://hz.zdqjudy.top/gtmitijxva.html

val n: String? = null;  n?.length
来源：http://hz.hywenlv.cn/gtuvgsropm.html

[T05] Kotlin：when 表达式
来源：http://hz.52xcode.cn/gthvbhzhyj.html

val s = when (x) { 1 -> "一" else -> "其他" }   // 多分支时每个分支单独一行
来源：http://hz.jinyuanbaomall.cn/gtzxokbjyj.html

[T06] Kotlin：集合映射
来源：http://hz.cheryme.top/gtupptvtmx.html

listOf(1, 2, 3).map { it * 2 }
来源：http://hz.c1oappe.top/gthgkqwrip.html

[T07] Kotlin：集合过滤
来源：http://hz.fengsongda.top/gtnflyxlzy.html

listOf(1, 2, 3).filter { it > 1 }
来源：http://hz.shangyingyoupin.top/gtlefdhqjd.html

[T08] Kotlin：数据类
来源：http://hz.zycfv.cn/gtworjqevs.html

data class User(val name: String, val age: Int)
来源：http://hz.zhijiandao.cn/gtxgsjqhbz.html

[T09] Kotlin：扩展函数
来源：http://hz.ydjk.org.cn/gtvkmxwdwz.html

fun String.exclaim() = this + "!"
来源：http://hz.zhengqikj.top/gtirubtrgu.html

[T10] Kotlin：默认参数
来源：http://hz.dianchejie.cn/gthbgewira.html

fun greet(name: String = "World") = "Hi $name"
来源：http://hz.bjfxy.top/gtsmgggyro.html

[T11] Kotlin：协程
来源：http://hz.shzxlz.cn/gtuemmpukj.html

GlobalScope.launch { delay(1000); println("done") }
来源：http://hz.zdqjudy.top/gtipufedva.html

[T12] Kotlin：解构声明
来源：http://hz.ppjwa.cn/gtkfqivvsj.html

val (a, b) = Pair(1, 2)
来源：http://hz.chenjidiqi.icu/gtnimsrxwk.html

[T13] Kotlin：只读 Map
来源：http://hz.kuanghao11.cn/gtfidklokr.html

val m = mapOf("a" to 1)
来源：http://hz.jyoumei.cn/gtqqlhtikc.html

[T14] Kotlin：循环
来源：http://hz.ppjwa.cn/gthpmyvkjv.html

for (i in 1..10) println(i)
来源：http://hz.jqgfzy.top/gtyowzqltw.html

[T15] Kotlin：接口
来源：http://hz.chenlongwang.top/gtabkfqiet.html

interface Shape { fun area(): Double }
来源：http://hz.tian-w.cn/gtlszypsok.html

[T16] Swift：Hello World
来源：http://hz.nanxinkj.top/gtbgtmrbdu.html

print("Hello")
来源：http://hz.chenzaomai.com/gtqozloifs.html

[T17] Swift：变量与常量
来源：http://hz.hnxiangtu.top/gtymgkgzcq.html

var a = 1;  let b = 2
来源：http://hz.nwbrower.top/gtbvyyjgyd.html

[T18] Swift：字符串插值
来源：http://hz.iojbl.cn/gtqdfqwuuq.html

"值: \(b)"
来源：http://hz.gaohongyu789.top/gtgfjsawot.html

[T19] Swift：可选绑定
来源：http://hz.gaohongyu789.top/gtvgpzvqjy.html

if let n = opt { print(n) }
来源：http://hz.bjfxy.top/gtomzftdde.html

[T20] Swift：数组操作
来源：http://hz.shanyushiyangtech.top/gtrhgrcpmc.html

var a = [1, 2, 3];  a.append(4)
来源：http://hz.ivvv.top/gthvzyztgv.html

[T21] Swift：遍历
来源：http://hz.guannengcc.top/gtknsjvyjt.html

for x in a { print(x) }
来源：http://hz.zhaomingkeji.xyz/gtuzfkyker.html

[T22] Swift：字典
来源：http://hz.yanxiufei.cn/gtmjxsvfhn.html

var d = ["a": 1];  d["b"] = 2
来源：http://hz.snrcjt.cn/gtxubabnvm.html

[T23] Swift：函数
来源：http://hz.birdmap.top/gtnmqjbfuv.html

func add(_ a: Int, _ b: Int) -> Int { a + b }
来源：http://hz.yvedp.cn/gtlmvmonrh.html

[T24] Swift：闭包
来源：http://hz.iojbl.cn/gtxcwgmhtn.html

let f = { (x: Int) -> Int in x * 2 }
来源：http://hz.shanyushiyangtech.top/gtsvigpyfd.html

[T25] Swift：结构体
来源：http://hz.haohaochexian.top/gtkypqgfki.html

struct P { var x: Int }
来源：http://hz.nanxinkj.top/gtluxyknly.html

[T26] Swift：类与重写
来源：http://hz.yuanzhike.top/gtxmrvzkjs.html

class A: Base { override func f() {} }
来源：http://hz.jinghuilouyu.cn/gtbvsxqkcy.html

[T27] Swift：错误处理
来源：http://hz.tanke756.top/gtvhnjzccc.html

do { try f() } catch { print(error) }
来源：http://hz.yvedp.cn/gtwcwmwrfa.html

[T28] Swift：枚举
来源：http://hz.hammf.cn/gtupinesma.html

enum Color { case red, green }
来源：http://hz.yueranfly.top/gtfyyytbuw.html

[T29] Swift：guard 提前返回
来源：http://hz.vqdsnc.cn/gtxjcglvwl.html

guard let x = opt else { return }
来源：http://hz.yuxming.cn/gttlxxitgf.html

[T30] Swift：协议
来源：http://hz.feifeiyinyue.top/gtyxujpqrn.html

protocol Shape { func area() -> Double }
来源：http://hz.shzxlz.cn/gtoziqguiq.html

[T31] Lua：Hello World
来源：http://hz.andypj.xyz/gtmoryjwcv.html

print("Hello")
来源：http://hz.yj202588.top/gtonkfxwlv.html

[T32] Lua：局部变量
来源：http://hz.xinyue.icu/gthvlkztek.html

local a = 1
来源：http://hz.cdnleiting.top/gtwrkyhiqh.html

[T33] Lua：表（数组）
来源：http://hz.ybcxt.top/gtjwnpjosr.html

local t = {1, 2, 3};  t[4] = 4
来源：http://hz.pengpengdd.cyou/gtokkklqss.html

[T34] Lua：遍历表
来源：http://hz.daria6918.cn/gtdsanvebh.html

for i, v in ipairs(t) do print(i, v) end
来源：http://hz.zhijiandao.cn/gtedhssctk.html

[T35] Lua：字典表
来源：http://hz.jinqigfzy.top/gtcuqrqunl.html

local d = { a = 1 };  d.b = 2
来源：http://hz.yongpay.top/gtndmxduoj.html

[T36] Lua：函数
来源：http://hz.jianghu66.top/gtwvkvajjg.html

function add(a, b) return a + b end
来源：http://hz.zdqjudy.top/gtbbjifqoo.html

[T37] Lua：字符串拼接
来源：http://hz.haohaochexian.top/gtfkxiajal.html

"a" .. "b"
来源：http://hz.xingfuxueyuan.xyz/gtmtrdpmiu.html

[T38] Lua：条件
来源：http://hz.jianghu66.top/gtciuuthcz.html

if x > 0 then print("正") end
来源：http://hz.zdqjudy.top/gtxtftnkqs.html

[T39] Lua：模式匹配
来源：http://hz.feifeiyinyue.top/gtnqyjapgd.html

string.find(s, "%d+")
来源：http://hz.hammf.cn/gtvjrdsdtx.html

[T40] Lua：元表
来源：http://hz.sysykeji.top/gtgksbfsnt.html

setmetatable({}, { __index = base })
来源：http://hz.pycfn.com/gtmajvrfhq.html

[T41] Perl：Hello World
来源：http://hz.shuidangran.top/gtthjameic.html

print "Hello\n";
来源：http://hz.pengpengdd.cyou/gtpywcmrue.html

[T42] Perl：变量类型
来源：http://hz.zhijiandao.cn/gtookxuajo.html

my $a = 1;  my @arr = (1, 2, 3);  my %h = (a => 1);
来源：http://hz.xingfuxueyuan.xyz/gtgyoqkpgg.html

[T43] Perl：字符串插值
来源：http://hz.cdnleiting.top/gtxhpunwrh.html

"值: $a"
来源：http://hz.hysaishi.cn/gtfxaeaskf.html

[T44] Perl：条件
来源：http://hz.yongpay.top/gtoymgvdpq.html

if ($a > 0) { print "正"; }
来源：http://hz.ppjwa.cn/gtvemsbtqi.html

[T45] Perl：数组遍历
来源：http://hz.snrcjt.cn/gthcihjzcj.html

for my $x (@arr) { print $x; }
来源：http://hz.yonumen.top/gtmjeecvzr.html

[T46] Perl：哈希操作
来源：http://hz.zhiwuduotai.top/gtvownsjrc.html

$h{b} = 2;  for my $k (keys %h) { print "$k=$h{$k}"; }
来源：http://hz.zhengqikj.top/gteepkpfdp.html

[T47] Perl：正则捕获
来源：http://hz.wangshuangyany.cn/gtvjteuwhb.html

if ($s =~ /(\d+)/) { print $1; }
来源：http://hz.sysykeji.top/gtomcikqpj.html

[T48] Perl：正则替换
来源：http://hz.dashuyun.cn/gtvebaozgf.html

$s =~ s/old/new/g;
来源：http://hz.dashuyun.cn/gtvawbibjf.html

[T49] Perl：函数
来源：http://hz.shzxlz.cn/gtkzuxrkyn.html

sub add { my ($a, $b) = @_; return $a + $b; }
来源：http://hz.yongpay.top/gtriospvbz.html

[T50] Perl：逐行读文件
来源：http://hz.meibo888.top/gtuenzmaxs.html

open my $fh, "<", "a.txt" or die $!;
来源：http://hz.zhijiandao.cn/gtjotqutqq.html

while (my $line = <$fh>) { print $line; }
来源：http://hz.tianlin.xyz/gtsedygbyv.html

[T51] Scala：Hello World
来源：http://hz.iojbl.cn/gtkwzogilc.html

println("Hello")
来源：http://hz.cucudq.cn/gtqqfnqtdb.html

[T52] Scala：变量
来源：http://hz.zhiwuduotai.top/gttuzbdwir.html

val a = 1;  var b = 2
来源：http://hz.jiagoushi.top/gtkkaebhul.html

[T53] Scala：字符串插值
来源：http://hz.shzxlz.cn/gtqdbwxmzy.html

s"值: $b"
来源：http://hz.guannengcc.top/gtnvoyioiq.html

[T54] Scala：集合映射
来源：http://hz.kuanghao11.cn/gtzqiylbvl.html

List(1, 2, 3).map(_ * 2)
来源：http://hz.gaohongyu789.top/gtfxvdjbbq.html

[T55] Scala：集合过滤
来源：http://hz.zhongyouzk.top/gtwqndbzod.html

List(1, 2, 3).filter(_ > 1)
来源：http://hz.wangshuangyany.cn/gteqgdoplk.html

[T56] Scala：样例类
来源：http://hz.yvedp.cn/gtuxdvnfso.html

case class User(name: String, age: Int)
来源：http://hz.ydzc1.top/gtjfkrbmwn.html

[T57] Scala：模式匹配
来源：http://hz.xingfuxueyuan.xyz/gtxbjwdkjb.html

x match { case 1 => "一"; case _ => "其他" }
来源：http://hz.zhixingplan.top/gtioodkxqm.html

[T58] Scala：函数定义
来源：http://hz.smart0.xyz/gtfoghrymi.html

def add(a: Int, b: Int): Int = a + b
来源：http://hz.ivvv.top/gtvikhzrbd.html

[T59] Scala：循环
来源：http://hz.cqqwz.cn/gtrhzodjls.html

for (i <- 1 to 10) println(i)
来源：http://hz.guowangkeji.top/gtvgswkxdo.html

[T60] Scala：折叠
来源：http://hz.gotoacloud.top/gtypinivsf.html

List(1, 2, 3).foldLeft(0)(_ + _)
来源：http://hz.gaohongyu789.top/gtsssmlkmy.html

================================================================================
来源：http://hz.wangshuangyany.cn/gtxbvrzmgc.html

U. 高频实用片段（Python / PHP / JavaScript 各 40 条）
来源：http://hz.jiagoushi.top/gtdjdkmxcp.html

================================================================================
来源：http://hz.haohaochexian.top/gtggimlwiw.html

[U01] Py：创建虚拟环境
来源：http://hz.zhengqikj.top/gtntnvqwcy.html

python -m venv .venv && source .venv/bin/activate
来源：http://hz.kuanghao11.cn/gtbiynihlc.html

[U02] Py：导出 / 安装依赖
来源：http://hz.0kj1m.cn/gtprcfsjbp.html

pip freeze > requirements.txt;  pip install -r requirements.txt
来源：http://hz.jyoumei.cn/gtnthzalyu.html

[U03] Py：加载 .env 配置
来源：http://hz.chenzaomai.com/gtlpxloway.html

from dotenv import load_dotenv; load_dotenv()
来源：http://hz.gotoacloud.top/gtzwmgdmyq.html

[U04] Py：变量调试打印
来源：http://hz.redwolf501.top/gtvdhefawd.html

print(f"{x=}")            # 输出 x=值，Python 3.8+
来源：http://hz.jiagoushi.top/gtaqdwsyuf.html

[U05] Py：列表去重且保序
来源：http://hz.birdmap.top/gtzslkcwsw.html

list(dict.fromkeys(arr))
来源：http://hz.yj202588.top/gtogajvnwj.html

[U06] Py：合并两个字典
来源：http://hz.pycfn.com/gtjvaqsyrx.html

{**a, **b}
来源：http://hz.xinyue.icu/gtbezpdxdk.html

[U07] Py：反转字典键值
来源：http://hz.yj202588.top/gtzhrhglhq.html

{v: k for k, v in d.items()}
来源：http://hz.jianghu66.top/gtwvmkbwpv.html

[U08] Py：展平二维列表
来源：http://hz.sufxvd.cn/gtqrhktabd.html

[y for x in nested for y in x]
来源：http://hz.jinyuanbaomall.cn/gtptlgcxgq.html

[U09] Py：字典取最大值的键
来源：http://hz.guannengcc.top/gtikkzeedj.html

max(d, key=d.get)
来源：http://hz.yj202588.top/gtxkcyesch.html

[U10] Py：按值排序字典
来源：http://hz.cdnleiting.top/gtxhzhdpeb.html

dict(sorted(d.items(), key=lambda kv: kv[1]))
来源：http://hz.kuanghao11.cn/gtikepenup.html

[U11] Py：生成器表达式
来源：http://hz.meibo888.top/gtjpxzfcdk.html

(x * 2 for x in arr)
来源：http://hz.aibaodan.cn/gtelorxhlo.html

[U12] Py：取出现最多的 3 个元素
来源：http://hz.yueranfly.top/gtjpptjuva.html

Counter(arr).most_common(3)
来源：http://hz.zdqjudy.top/gtiorodxkl.html

[U13] Py：固定长度队列
来源：http://hz.hongshengwenyu.top/gtthygmyyi.html

deque(maxlen=10)
来源：http://hz.chenjidiqi.icu/gtvochmjht.html

[U14] Py：分组收集到列表
来源：http://hz.sxryk.cn/gtribhepzn.html

defaultdict(list)
来源：http://hz.yj202588.top/gtbcpzojgs.html

[U15] Py：高精度计时
来源：http://hz.shuidangran.top/gtctgfjfky.html

t = time.perf_counter()
来源：http://hz.ppjwa.cn/gtayelhvmj.html

[U16] Py：命令行参数解析
来源：http://hz.hnxiangtu.top/gtzbgzzupk.html

ap = argparse.ArgumentParser();  ap.add_argument("--name");  args = ap.parse_args()
来源：http://hz.cheryme.top/gtmmazuzfw.html

[U17] Py：初始化日志
来源：http://hz.guowangkeji.top/gtijcxzbwd.html

logging.basicConfig(level=logging.INFO)
来源：http://hz.chenlongwang.top/gtfjkcubzm.html

[U18] Py：预编译正则
来源：http://hz.sweek.top/gtbfgkoxzw.html

pat = re.compile(r"\d+")
来源：http://hz.yongpay.top/gtspjirshz.html

[U19] Py：正则替换带回调
来源：http://hz.jinyuanbaomall.cn/gtolijcjbm.html

re.sub(r"\d+", lambda m: str(int(m.group()) * 2), s)
来源：http://hz.shzxlz.cn/gtgzeercqb.html

[U20] Py：缓存函数结果
来源：http://hz.fzhhl.top/gtcnwqpnbp.html

@functools.lru_cache(maxsize=None)
来源：http://hz.zhengqikj.top/gtboacmzpx.html

[U21] Py：自定义上下文管理器
来源：http://hz.hammf.cn/gtwbauuwkl.html

@contextlib.contextmanager
来源：http://hz.tanke756.top/gtzrydhbfs.html

[U22] Py：矩阵转置
来源：http://hz.aizwys.cn/gteodettze.html

list(zip(*m))
来源：http://hz.tianlin.xyz/gtaxjbunaf.html

[U23] Py：分块读取大文件
来源：http://hz.wangdashe.top/gtxoxgnnoq.html

for chunk in iter(lambda: f.read(8192), b""):
来源：http://hz.sweek.top/gtrcjyanux.html

[U24] Py：路径操作
来源：http://hz.jinqigfzy.top/gtxaxqyssv.html

Path("a/b.txt").parent.mkdir(parents=True, exist_ok=True)
来源：http://hz.hammf.cn/gtpmnzotfr.html

[U25] Py：CSV 按字典读
来源：http://hz.sweek.top/gtvidhakhz.html

csv.DictReader(f)
来源：http://hz.0kj1m.cn/gtxyfqnpyg.html

[U26] Py：并发下载
来源：http://hz.kuanghao11.cn/gtaibrhvty.html

ThreadPoolExecutor(max_workers=8).map(fetch, urls)
来源：http://hz.316326.xyz/gtjqnapmcl.html

[U27] Py：异步 HTTP
来源：http://hz.yj202588.top/gtzevlukpr.html

aiohttp.ClientSession() 配合 async with
来源：http://hz.cqqwz.cn/gtbahdzdta.html

[U28] Py：类型别名
来源：http://hz.jlsjyb.cn/gttozulcis.html

UserId = int
来源：http://hz.ydjk.org.cn/gtzdragrms.html

[U29] Py：属性校验
来源：http://hz.yangfankeji.com/gtubuqnayj.html

@property 与 @x.setter 配合
来源：http://hz.ywan-chungtsiang.top/gtavpjwegt.html

[U30] Py：数据类
来源：http://hz.wangdashe.top/gtekgmmevu.html

@dataclass(slots=True)
来源：http://hz.smart0.xyz/gtqiieqqzg.html

[U31] Py：单测
来源：http://hz.ppjwa.cn/gtcpawilvh.html

python -m pytest -q
来源：http://hz.dashuyun.cn/gtsmzmqtzs.html

[U32] Py：代码格式化
来源：http://hz.sweek.top/gtmvpzgtxb.html

ruff format . && ruff check --fix .
来源：http://hz.jinyuanbaomall.cn/gtmggzwhmn.html

[U33] Py：打包发布
来源：http://hz.hfpthk.cn/gtmmvgvimu.html

python -m build  （依赖 pyproject.toml）
来源：http://hz.andypj.xyz/gtozbyexpr.html

[U34] Py：判断编码
来源：http://hz.ehwqpu.com/gtlzejmpbt.html

chardet.detect(raw)
来源：http://hz.yanxiufei.cn/gthhuqbkyi.html

[U35] Py：发送邮件
来源：http://hz.chenlongwang.top/gtauuafwwg.html

smtplib.SMTP_SSL(...).send_message(msg)
来源：http://hz.ybcxt.top/gtxfetgvkm.html

[U36] Py：定时任务
来源：http://hz.dashuyun.cn/gtfohpnygt.html

schedule.every(10).minutes.do(job)
来源：http://hz.guannengcc.top/gtvxhnbidc.html

[U37] Py：读写 Excel
来源：http://hz.hammf.cn/gtlsnbutak.html

pandas.read_excel / DataFrame.to_excel
来源：http://hz.smart0.xyz/gthnyrysgq.html

[U38] Py：获取脚本所在目录
来源：http://hz.52xcode.cn/gteydowasv.html

Path(__file__).resolve().parent
来源：http://hz.zhoulong.xyz/gtnvwgahbn.html

[U39] Py：判断是否在交互环境
来源：http://hz.smart0.xyz/gthbvfixkt.html

sys.stdout.isatty()
来源：http://hz.redwolf501.top/gtpbaubycy.html

[U40] Py：打印到标准错误
来源：http://hz.redwolf501.top/gtwfbzznmp.html

print("err", file=sys.stderr)
来源：http://hz.jinyuanbaomall.cn/gtgwnxdqzd.html

[U41] PHP：初始化 Composer 项目
来源：http://hz.cheryme.top/gtbzdoeoly.html

composer init;  composer require guzzlehttp/guzzle
来源：http://hz.guowangkeji.top/gtzaxtzfzr.html

[U42] PHP：PSR-4 自动加载
来源：http://hz.jlsjyb.cn/gtzlfreunj.html

"autoload": { "psr-4": { "App\\": "src/" } }
来源：http://hz.pycfn.com/gtwrspvwpv.html

[U43] PHP：声明命名空间
来源：http://hz.9152youxi.cn/gtglcdtvur.html

namespace App\Http;
来源：http://hz.snrcjt.cn/gtpbtjwtgb.html

[U44] PHP：开启严格类型
来源：http://hz.0kj1m.cn/gtyfviiqmx.html

declare(strict_types=1);
来源：http://hz.jinyuanbaomall.cn/gtbexfvnwt.html

[U45] PHP：类型声明与返回类型
来源：http://hz.0kj1m.cn/gtcesvrero.html

function add(int $a, int $b): int { return $a + $b; }
来源：http://hz.iojbl.cn/gtpxkaxojq.html

[U46] PHP：可空类型
来源：http://hz.andypj.xyz/gtvwhfvlfk.html

?string $name = null
来源：http://hz.sxryk.cn/gtuuqrzfke.html

[U47] PHP：联合类型
来源：http://hz.nwbrower.top/gtzomszris.html

int|string $id
来源：http://hz.gogol.net.cn/gtuwbpmohb.html

[U48] PHP：纯枚举
来源：http://hz.yonumen.top/gtrgsbttjn.html

enum Status: string { case Active = "active"; case Off = "off"; }
来源：http://hz.vqdsnc.cn/gtpjmurdsv.html

[U49] PHP：只读属性
来源：http://hz.xylfe.cn/gtbghcnuue.html

public readonly string $name
来源：http://hz.sufxvd.cn/gtfovbwefc.html

[U50] PHP：构造器属性提升
来源：http://hz.cheryme.top/gtrhwdhfde.html

public function __construct(private int $id) {}
来源：http://hz.tanke756.top/gtqfefedjv.html

[U51] PHP：数组解构
来源：http://hz.zhongyouzk.top/gtuqgfpcyn.html

[$a, $b] = $arr;
来源：http://hz.jinqigufen.top/gtgoplmfed.html

[U52] PHP：箭头函数
来源：http://hz.cheryme.top/gtzyazlkfd.html

$double = fn($x) => $x * 2;
来源：http://hz.jyoumei.cn/gtelbsklsa.html

[U53] PHP：空合并运算符
来源：http://hz.ybcxt.top/gtpnaxmdga.html

$v = $a ?? $b ?? "default";
来源：http://hz.xziqi.cn/gthytppgnw.html

[U54] PHP：空安全调用
来源：http://hz.fengsongda.top/gtvxiizsrq.html

$obj?->method()
来源：http://hz.tanke756.top/gtskmhaapw.html

[U55] PHP：match 表达式
来源：http://hz.ydzc1.top/gtktvehmvr.html

$s = match($x) { 1 => "一", default => "其他" };
来源：http://hz.jlsjyb.cn/gtxlvyoihv.html

[U56] PHP：命名参数
来源：http://hz.52xcode.cn/gtzyraalja.html

f(a: 1, b: 2)
来源：http://hz.ybcxt.top/gtogelntbg.html

[U57] PHP：字符串插值
来源：http://hz.hnqzz.top/gtaqfuykny.html

"值: {$a}"
来源：http://hz.ehwqpu.com/gtbxcaumvk.html

[U58] PHP：数组三件套
来源：http://hz.yvedp.cn/gtmbtgztyx.html

array_map($f, $a);  array_filter($a, $f);  array_reduce($a, $f, 0);
来源：http://hz.feifeiyinyue.top/gtwygoplfq.html

[U59] PHP：自定义排序
来源：http://hz.pycfn.com/gtmlzlshuz.html

usort($arr, fn($a, $b) => $a["age"] <=> $b["age"]);
来源：http://hz.redwolf501.top/gtcbmgybxu.html

[U60] PHP：JSON 编解码
来源：http://hz.kuanghao11.cn/gtrhompsjl.html

json_encode($d, JSON_UNESCAPED_UNICODE);  json_decode($s, true);
来源：http://hz.guowangkeji.top/gtovfxamaj.html

[U61] PHP：正则
来源：http://hz.zhongyouzk.top/gtwiwseyka.html

preg_match('/(\d+)/', $s, $m);  preg_replace('/\d+/', '#', $s);
来源：http://hz.yonumen.top/gtnphmdpqf.html

[U62] PHP：日期对象
来源：http://hz.jlsjyb.cn/gtiocurpxe.html

(new DateTimeImmutable())->format("Y-m-d");
来源：http://hz.yanxiufei.cn/gtvymarywt.html

[U63] PHP：文件读写
来源：http://hz.feifeiyinyue.top/gtyoasvroq.html

file_get_contents($f);  file_put_contents($f, $data);
来源：http://hz.shuidangran.top/gtojyzttgr.html

[U64] PHP：目录遍历
来源：http://hz.ppjwa.cn/gtqxiyjwna.html

glob("dir/*.php");  scandir("dir");
来源：http://hz.9152youxi.cn/gthtyfzhqh.html

[U65] PHP：会话
来源：http://hz.jianghu66.top/gtyhozzbyq.html

session_start();  $_SESSION["uid"] = 1;
来源：http://hz.iojbl.cn/gtqtygirzj.html

[U66] PHP：设置 Cookie
来源：http://hz.yj20258888.top/gtlqqhxvan.html

setcookie("token", $v, ["httponly" => true, "samesite" => "Lax"]);
来源：http://hz.yuxming.cn/gtctmyhwzk.html


<!-- 参考信息 -->