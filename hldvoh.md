代发 wailian999

[S39] C++：自定义比较器排序
来源：http://hz.yj202588.top/gtnmrowxhw.html

std::sort(v.begin(), v.end(), [](int a, int b) { return a > b; });
来源：http://hz.cashguo.top/gtiqdtkxdn.html

[S40] C++：查找元素
来源：http://hz.ywan-chungtsiang.top/gtjsuyntvz.html

auto it = std::find(v.begin(), v.end(), 3);
来源：http://hz.ybcxt.top/gtydoosfut.html

[S41] C++：类与构造函数
来源：http://hz.pycfn.com/gtuzgyzrag.html

class A { public: A(int v) : x_(v) {} int get() const { return x_; } private: int x_; };
来源：http://hz.jyoumei.cn/gtmqshjipd.html

[S42] C++：继承与虚函数
来源：http://hz.feifeiyinyue.top/gtnslhbljw.html

class B : public Base { public: void f() override {} };
来源：http://hz.shangyingyoupin.top/gtmenexvey.html

[S43] C++：智能指针
来源：http://hz.cashguo.top/gtnmrfrfrq.html

auto p = std::make_unique<int>(5);
来源：http://hz.ivvv.top/gtbolpvjbx.html

[S44] C++：引用传参
来源：http://hz.jinqigfzy.top/gtyyvndynf.html

void inc(int &x) { ++x; }
来源：http://hz.gotoacloud.top/gtpbnpqbqn.html

[S45] C++：lambda
来源：http://hz.gotoacloud.top/gtbcurcaup.html

auto add = [](int a, int b) { return a + b; };
来源：http://hz.yanxiufei.cn/gteimhflbl.html

[S46] C++：函数模板
来源：http://hz.hnxiangtu.top/gtzgbbsajd.html

template <typename T> T maxv(T a, T b) { return a > b ? a : b; }
来源：http://hz.xuetiantiany.cn/gtbrvprtci.html

[S47] C++：结构化绑定遍历
来源：http://hz.hnxiangtu.top/gtsixiojws.html

for (const auto &[k, v] : m) { std::cout << k << v; }
来源：http://hz.gogol.net.cn/gtsqbpucqz.html

[S48] C++：逐行读文件
来源：http://hz.yueranfly.top/gtxvutmzun.html

std::ifstream in("a.txt");  std::string line;
来源：http://hz.52xcode.cn/gttrckpcgy.html

while (std::getline(in, line)) { }
来源：http://hz.ehwqpu.com/gtdnkapqjd.html

[S49] C++：写文件
来源：http://hz.9152youxi.cn/gtlwfskmrb.html

std::ofstream out("a.txt");  out << "hi\n";
来源：http://hz.ppjwa.cn/gtdmidqpim.html

[S50] C++：格式化数字
来源：http://hz.quarkkingdee.top/gtomjqqoml.html

std::ostringstream os;  os << std::fixed << std::setprecision(2) << 3.14159;
来源：http://hz.yongpay.top/gtrrllbloe.html

[S51] C++：显式类型转换
来源：http://hz.cucudq.cn/gttjdabbwd.html

static_cast<double>(a) / b
来源：http://hz.yonumen.top/gtfhdgrgls.html

[S52] C++：const 与 noexcept
来源：http://hz.xingfuxueyuan.xyz/gtecscafwp.html

int size() const noexcept { return n_; }
来源：http://hz.cdnleiting.top/gtrvqhkoro.html

[S53] C++：移动语义
来源：http://hz.cqqwz.cn/gtmlnlhfuf.html

std::vector<int> w = std::move(v);
来源：http://hz.nanxuanxn.top/gtmgohsvxm.html

[S54] C++：异常处理
来源：http://hz.yangfankeji.com/gtkgavhxih.html

try { throw std::runtime_error("x"); } catch (const std::exception &e) { }
来源：http://hz.cucudq.cn/gtjgbdmivb.html

[S55] C++：结构化绑定
来源：http://hz.kuanghao11.cn/gtqxqeoann.html

auto [a, b] = std::make_pair(1, 2);
来源：http://hz.tianlin.xyz/gthqshootd.html

[S56] C++：optional
来源：http://hz.shangyingyoupin.top/gtbsimdbzw.html

std::optional<int> o = 5;  if (o) { int v = *o; }
来源：http://hz.redwolf501.top/gtxgxqfnif.html

[S57] C++：编译期常量
来源：http://hz.hywenlv.cn/gtkgxbjzzt.html

constexpr int N = 10;
来源：http://hz.316326.xyz/gtesyxrwou.html

[S58] C++：命名空间
来源：http://hz.daria6918.cn/gtqclmcqbd.html

namespace ns { int f() { return 1; } }
来源：http://hz.gogol.net.cn/gtabhjnjpe.html

[S59] C++：静态断言
来源：http://hz.ehwqpu.com/gteeqbtgqc.html

static_assert(sizeof(int) == 4, "int 必须 4 字节");
来源：http://hz.jinqigufen.top/gthdnokkpj.html

[S60] C++：遍历并删除元素
来源：http://hz.mhx1999.top/gtujjzunee.html

v.erase(std::remove_if(v.begin(), v.end(), [](int x) { return x < 0; }), v.end());
来源：http://hz.sweek.top/gtjpgoevgb.html

================================================================================
来源：http://hz.chenlongwang.top/gthuwpoasx.html

T. 其他语言补充（Kotlin / Swift / Lua / Perl / Scala）
来源：http://hz.birdmap.top/gtocyhbypt.html

================================================================================
来源：http://hz.chenlongwang.top/gtcjcwgugq.html

[T01] Kotlin：Hello World
来源：http://hz.svipenyu.cn/gtgpntezzd.html

println("Hello")
来源：http://hz.jianghu66.top/gtsanjaooa.html

[T02] Kotlin：变量
来源：http://hz.tian-w.cn/gtbodwvemn.html

val a = 1;  var b = 2        // val 只读，var 可变
来源：http://hz.pycfn.com/gtipsdfpye.html

[T03] Kotlin：字符串模板
来源：http://hz.xziqi.cn/gtzvbhxsmx.html

"值: $b"
来源：http://hz.mhx1999.top/gtylavweoc.html

[T04] Kotlin：空安全
来源：http://hz.jyoumei.cn/gtdacgwpzu.html

val n: String? = null;  n?.length
来源：http://hz.9152youxi.cn/gtfwcmkaty.html

[T05] Kotlin：when 表达式
来源：http://hz.xingfuxueyuan.xyz/gtkldhdybq.html

val s = when (x) { 1 -> "一" else -> "其他" }   // 多分支时每个分支单独一行
来源：http://hz.birdmap.top/gtxgwyhkkc.html

[T06] Kotlin：集合映射
来源：http://hz.yongpay.top/gtkhljpove.html

listOf(1, 2, 3).map { it * 2 }
来源：http://hz.gaohongyu789.top/gtmadzomdq.html

[T07] Kotlin：集合过滤
来源：http://hz.jqgfzy.top/gtpmimbytk.html

listOf(1, 2, 3).filter { it > 1 }
来源：http://hz.yueranfly.top/gtotpbmszr.html

[T08] Kotlin：数据类
来源：http://hz.kuanghao11.cn/gtldkosyku.html

data class User(val name: String, val age: Int)
来源：http://hz.vqdsnc.cn/gtmroavdva.html

[T09] Kotlin：扩展函数
来源：http://hz.jyoumei.cn/gtawnedtst.html

fun String.exclaim() = this + "!"
来源：http://hz.nwbrower.top/gtdigrafpa.html

[T10] Kotlin：默认参数
来源：http://hz.tanke756.top/gtcjgxdvbs.html

fun greet(name: String = "World") = "Hi $name"
来源：http://hz.sufxvd.cn/gtveasuaux.html

[T11] Kotlin：协程
来源：http://hz.cheryme.top/gtfhtrcsgu.html

GlobalScope.launch { delay(1000); println("done") }
来源：http://hz.andypj.xyz/gtcttojhoo.html

[T12] Kotlin：解构声明
来源：http://hz.hywenlv.cn/gtbddzhhic.html

val (a, b) = Pair(1, 2)
来源：http://hz.daria6918.cn/gtilciqkqi.html

[T13] Kotlin：只读 Map
来源：http://hz.sweek.top/gtjljtfseo.html

val m = mapOf("a" to 1)
来源：http://hz.daxiang520.top/gtobqqmnlv.html

[T14] Kotlin：循环
来源：http://hz.haohaochexian.top/gtypfuxmuh.html

for (i in 1..10) println(i)
来源：http://hz.aibaodan.cn/gtzogvpaqv.html

[T15] Kotlin：接口
来源：http://hz.daria6918.cn/gtsjfeffli.html

interface Shape { fun area(): Double }
来源：http://hz.c1oappe.top/gtdhsmaoxm.html

[T16] Swift：Hello World
来源：http://hz.nanxinkj.top/gtbymzpfba.html

print("Hello")
来源：http://hz.cdnleiting.top/gtxmvdbhgj.html

[T17] Swift：变量与常量
来源：http://hz.0kj1m.cn/gtrduzhuzq.html

var a = 1;  let b = 2
来源：http://hz.aizwys.cn/gtorgzlont.html

[T18] Swift：字符串插值
来源：http://hz.birdmap.top/gtnhybnnze.html

"值: \(b)"
来源：http://hz.meibo888.top/gtcbidvemr.html

[T19] Swift：可选绑定
来源：http://hz.havefunace.top/gtpvfvzglw.html

if let n = opt { print(n) }
来源：http://hz.hysaishi.cn/gtmskzzrmo.html

[T20] Swift：数组操作
来源：http://hz.yuanzhike.top/gtxyhqiscq.html

var a = [1, 2, 3];  a.append(4)
来源：http://hz.zhiwuduotai.top/gtrhrbtijj.html

[T21] Swift：遍历
来源：http://hz.316326.xyz/gtxapyumhr.html

for x in a { print(x) }
来源：http://hz.haohaochexian.top/gtxwixltho.html

[T22] Swift：字典
来源：http://hz.redwolf501.top/gtpjxloapv.html

var d = ["a": 1];  d["b"] = 2
来源：http://hz.chenlongwang.top/gtdxgrbrot.html

[T23] Swift：函数
来源：http://hz.jinyuanbaomall.cn/gttejkhfvt.html

func add(_ a: Int, _ b: Int) -> Int { a + b }
来源：http://hz.snrcjt.cn/gtuhtkjrjj.html

[T24] Swift：闭包
来源：http://hz.zhijiandao.cn/gtkewitgnr.html

let f = { (x: Int) -> Int in x * 2 }
来源：http://hz.feifeiyinyue.top/gtshymyvpn.html

[T25] Swift：结构体
来源：http://hz.tianlin.xyz/gtrmodjfcb.html

struct P { var x: Int }
来源：http://hz.bjfxy.top/gtcwphbsxc.html

[T26] Swift：类与重写
来源：http://hz.jinqigfzy.top/gtyxgrfvws.html

class A: Base { override func f() {} }
来源：http://hz.c1oappe.top/gtzucvtbwr.html

[T27] Swift：错误处理
来源：http://hz.zycfv.cn/gtxzsngzzf.html

do { try f() } catch { print(error) }
来源：http://hz.yuanzhike.top/gtxbrnjpiv.html

[T28] Swift：枚举
来源：http://hz.shangyingyoupin.top/gtyieslddv.html

enum Color { case red, green }
来源：http://hz.gzhubu.top/gttkmjdgtc.html

[T29] Swift：guard 提前返回
来源：http://hz.zhaomingkeji.xyz/gtiveaafju.html

guard let x = opt else { return }
来源：http://hz.gaohongyu789.top/gtacwqqpxj.html

[T30] Swift：协议
来源：http://hz.zhijiandao.cn/gtbtsfuxbj.html

protocol Shape { func area() -> Double }
来源：http://hz.snrcjt.cn/gtwiqxgznf.html

[T31] Lua：Hello World
来源：http://hz.gotoacloud.top/gtrlelwjnt.html

print("Hello")
来源：http://hz.yongpay.top/gtsjxjmyti.html

[T32] Lua：局部变量
来源：http://hz.mhx1999.top/gthziirzpo.html

local a = 1
来源：http://hz.jiagoushi.top/gtvujmtkhu.html

[T33] Lua：表（数组）
来源：http://hz.pengpengdd.cyou/gtqhlnlmxr.html

local t = {1, 2, 3};  t[4] = 4
来源：http://hz.hfpthk.cn/gtnbypyoha.html

[T34] Lua：遍历表
来源：http://hz.hongshengwenyu.top/gtncjoavfu.html

for i, v in ipairs(t) do print(i, v) end
来源：http://hz.jinqigufen.top/gtwaqqmoxb.html

[T35] Lua：字典表
来源：http://hz.aibaodan.cn/gtdnilpmzu.html

local d = { a = 1 };  d.b = 2
来源：http://hz.daria6918.cn/gtmylmvkev.html

[T36] Lua：函数
来源：http://hz.redwolf501.top/gtptfnxjnv.html

function add(a, b) return a + b end
来源：http://hz.jqgufenzy.top/gthazgoixs.html

[T37] Lua：字符串拼接
来源：http://hz.zhongyouzk.top/gtubvdddae.html

"a" .. "b"
来源：http://hz.sweek.top/gtxjnefxud.html

[T38] Lua：条件
来源：http://hz.jinqigfzy.top/gttqcnraaq.html

if x > 0 then print("正") end
来源：http://hz.vqdsnc.cn/gtwavbajxi.html

[T39] Lua：模式匹配
来源：http://hz.smart0.xyz/gtraynxolu.html

string.find(s, "%d+")
来源：http://hz.sysykeji.top/gtmrmizycc.html

[T40] Lua：元表
来源：http://hz.shanyushiyangkeji.top/gttjwrpmdn.html

setmetatable({}, { __index = base })
来源：http://hz.52xcode.cn/gtxsbhcobk.html

[T41] Perl：Hello World
来源：http://hz.tianlin.xyz/gtnblcnapq.html

print "Hello\n";
来源：http://hz.dashuyun.cn/gtmfkpmkcq.html

[T42] Perl：变量类型
来源：http://hz.52xcode.cn/gtxqzfxphb.html

my $a = 1;  my @arr = (1, 2, 3);  my %h = (a => 1);
来源：http://hz.iojbl.cn/gtwiykbflq.html

[T43] Perl：字符串插值
来源：http://hz.zhijiandao.cn/gtilynwfis.html

"值: $a"
来源：http://hz.gogol.net.cn/gtfztnftxe.html

[T44] Perl：条件
来源：http://hz.hammf.cn/gtzfqhrfum.html

if ($a > 0) { print "正"; }
来源：http://hz.tianlin.xyz/gthpsjmlsy.html

[T45] Perl：数组遍历
来源：http://hz.zdqjudy.top/gtklzsoxty.html

for my $x (@arr) { print $x; }
来源：http://hz.cucudq.cn/gtgtxkdluu.html

[T46] Perl：哈希操作
来源：http://hz.ppjwa.cn/gtikacrptx.html

$h{b} = 2;  for my $k (keys %h) { print "$k=$h{$k}"; }
来源：http://hz.feifeiyinyue.top/gtvfhaswep.html

[T47] Perl：正则捕获
来源：http://hz.redwolf501.top/gthbtycnbd.html

if ($s =~ /(\d+)/) { print $1; }
来源：http://hz.redwolf501.top/gtkbnhyvku.html

[T48] Perl：正则替换
来源：http://hz.hnxiangtu.top/gtgrbxykph.html

$s =~ s/old/new/g;
来源：http://hz.yueranfly.top/gthgnwcfkl.html

[T49] Perl：函数
来源：http://hz.jqgufenzy.top/gtjhlbicwq.html

sub add { my ($a, $b) = @_; return $a + $b; }
来源：http://hz.yonumen.top/gtazozfznx.html

[T50] Perl：逐行读文件
来源：http://hz.ppjwa.cn/gtphedxwuw.html

open my $fh, "<", "a.txt" or die $!;
来源：http://hz.cashguo.top/gtddklwtgj.html

while (my $line = <$fh>) { print $line; }
来源：http://hz.shanyushiyangtech.top/gtvhsujgxq.html

[T51] Scala：Hello World
来源：http://hz.tian-w.cn/gtnnbwuuqb.html

println("Hello")
来源：http://hz.nanxinkj.top/gtogrijawg.html

[T52] Scala：变量
来源：http://hz.ydzc1.top/gtiycbfkmj.html

val a = 1;  var b = 2
来源：http://hz.chenjidiqi.icu/gtoxvalqee.html

[T53] Scala：字符串插值
来源：http://hz.shuidangran.top/gtkmbkeroc.html

s"值: $b"
来源：http://hz.aibaodan.cn/gtwsijwzty.html

[T54] Scala：集合映射
来源：http://hz.shuidangran.top/gtjccwsqng.html

List(1, 2, 3).map(_ * 2)
来源：http://hz.quarkkingdee.top/gttxlpyapj.html

[T55] Scala：集合过滤
来源：http://hz.snrcjt.cn/gtxsgtetaw.html

List(1, 2, 3).filter(_ > 1)
来源：http://hz.dashuyun.cn/gtaxfkomuh.html

[T56] Scala：样例类
来源：http://hz.c1oappe.top/gtkwfmbvvl.html

case class User(name: String, age: Int)
来源：http://hz.wangshuangyany.cn/gtwboikvnr.html

[T57] Scala：模式匹配
来源：http://hz.sysykeji.top/gtfzrxjprd.html

x match { case 1 => "一"; case _ => "其他" }
来源：http://hz.sxryk.cn/gtityqroho.html

[T58] Scala：函数定义
来源：http://hz.redwolf501.top/gttbecltaz.html

def add(a: Int, b: Int): Int = a + b
来源：http://hz.jlsjyb.cn/gtydqbgeeo.html

[T59] Scala：循环
来源：http://hz.ivvv.top/gtjlyozmft.html

for (i <- 1 to 10) println(i)
来源：http://hz.dianchejie.cn/gtfxddcxwx.html

[T60] Scala：折叠
来源：http://hz.feifeiyinyue.top/gtmohaltck.html

List(1, 2, 3).foldLeft(0)(_ + _)
来源：http://hz.havefunace.top/gtbkifnboz.html

================================================================================
来源：http://hz.ivvv.top/gtnpdjcbza.html

U. 高频实用片段（Python / PHP / JavaScript 各 40 条）
来源：http://hz.gaohongyu789.top/gtmakrkfha.html

================================================================================
来源：http://hz.ydjk.org.cn/gtxtmumpch.html

[U01] Py：创建虚拟环境
来源：http://hz.jyoumei.cn/gtepsbohow.html

python -m venv .venv && source .venv/bin/activate
来源：http://hz.tian-w.cn/gtivpbobuf.html

[U02] Py：导出 / 安装依赖
来源：http://hz.tanke756.top/gtjchfmwdc.html

pip freeze > requirements.txt;  pip install -r requirements.txt
来源：http://hz.sysykeji.top/gtrmmsvhvc.html

[U03] Py：加载 .env 配置
来源：http://hz.aizwys.cn/gtxdpaxcho.html

from dotenv import load_dotenv; load_dotenv()
来源：http://hz.jqgufenzy.top/gtldcjcdum.html

[U04] Py：变量调试打印
来源：http://hz.sweek.top/gthurzehhf.html

print(f"{x=}")            # 输出 x=值，Python 3.8+
来源：http://hz.iojbl.cn/gtbdvgmaku.html

[U05] Py：列表去重且保序
来源：http://hz.cheryme.top/gtgwyqibrr.html

list(dict.fromkeys(arr))
来源：http://hz.wangdashe.top/gtlugocrhp.html

[U06] Py：合并两个字典
来源：http://hz.wangshuangyany.cn/gtxuuqqebc.html

{**a, **b}
来源：http://hz.nwbrower.top/gtrnsgyuga.html

[U07] Py：反转字典键值
来源：http://hz.shanyushiyangkeji.top/gtywezikwv.html

{v: k for k, v in d.items()}
来源：http://hz.xziqi.cn/gtcclcjvhf.html

[U08] Py：展平二维列表
来源：http://hz.tanke756.top/gtepnfhjwe.html

[y for x in nested for y in x]
来源：http://hz.feifeiyinyue.top/gthtwelssr.html

[U09] Py：字典取最大值的键
来源：http://hz.cashguo.top/gtomqlqoth.html

max(d, key=d.get)
来源：http://hz.redwolf501.top/gtismrfkah.html

[U10] Py：按值排序字典
来源：http://hz.cheryme.top/gtvyvcwydu.html

dict(sorted(d.items(), key=lambda kv: kv[1]))
来源：http://hz.aibaodan.cn/gttpzrevmf.html

[U11] Py：生成器表达式
来源：http://hz.gzhubu.top/gtjagowqpi.html

(x * 2 for x in arr)
来源：http://hz.hfpthk.cn/gtvsfqzdhw.html

[U12] Py：取出现最多的 3 个元素
来源：http://hz.jqgufenzy.top/gtjpdkdvyz.html

Counter(arr).most_common(3)
来源：http://hz.shanyushiyangtech.top/gtnngadnfy.html

[U13] Py：固定长度队列
来源：http://hz.birdmap.top/gtnlwfkbxh.html

deque(maxlen=10)
来源：http://hz.havefunace.top/gtlzedmgor.html

[U14] Py：分组收集到列表
来源：http://hz.smart0.xyz/gttewwvrli.html

defaultdict(list)
来源：http://hz.chenjidiqi.icu/gtdkeyqrpc.html

[U15] Py：高精度计时
来源：http://hz.hongshengwenyu.top/gtjokhykba.html

t = time.perf_counter()
来源：http://hz.shangyingyoupin.top/gtmkodbhba.html

[U16] Py：命令行参数解析
来源：http://hz.tanke756.top/gtpbdpiqhh.html

ap = argparse.ArgumentParser();  ap.add_argument("--name");  args = ap.parse_args()
来源：http://hz.vqdsnc.cn/gtgzmroubn.html

[U17] Py：初始化日志
来源：http://hz.nwbrower.top/gttnwxgqyr.html

logging.basicConfig(level=logging.INFO)
来源：http://hz.jqgufenzy.top/gtitoyadof.html

[U18] Py：预编译正则
来源：http://hz.ybcxt.top/gtuygyxpyl.html

pat = re.compile(r"\d+")
来源：http://hz.zhengqikj.top/gtoixilqzv.html

[U19] Py：正则替换带回调
来源：http://hz.0kj1m.cn/gtcaakurng.html

re.sub(r"\d+", lambda m: str(int(m.group()) * 2), s)
来源：http://hz.jinghuilouyu.cn/gtnecqhwni.html

[U20] Py：缓存函数结果
来源：http://hz.jqgufenzy.top/gtrtwyiwyk.html

@functools.lru_cache(maxsize=None)
来源：http://hz.gogol.net.cn/gtwcvuvzls.html

[U21] Py：自定义上下文管理器
来源：http://hz.zhongyouzk.top/gtxbhcsenv.html

@contextlib.contextmanager
来源：http://hz.ybcxt.top/gtxvxcomtc.html

[U22] Py：矩阵转置
来源：http://hz.shanyushiyangtech.top/gtxvlgcaca.html

list(zip(*m))
来源：http://hz.gotoacloud.top/gtpvaspjrj.html

[U23] Py：分块读取大文件
来源：http://hz.yuxming.cn/gtlwhxpyck.html

for chunk in iter(lambda: f.read(8192), b""):
来源：http://hz.hysaishi.cn/gtlxiarpqr.html

[U24] Py：路径操作
来源：http://hz.ydzc1.top/gtyndxfjjb.html

Path("a/b.txt").parent.mkdir(parents=True, exist_ok=True)
来源：http://hz.snrcjt.cn/gtllfbdzfb.html

[U25] Py：CSV 按字典读
来源：http://hz.shanyushiyangtech.top/gtsctzazdp.html

csv.DictReader(f)
来源：http://hz.jiagoushi.top/gtugjdcqij.html

[U26] Py：并发下载
来源：http://hz.aibaodan.cn/gtfgqzntvy.html

ThreadPoolExecutor(max_workers=8).map(fetch, urls)
来源：http://hz.havefunace.top/gtkfafblnz.html

[U27] Py：异步 HTTP
来源：http://hz.dashuyun.cn/gtpwoowmlx.html

aiohttp.ClientSession() 配合 async with
来源：http://hz.andypj.xyz/gtxyrsxexm.html

[U28] Py：类型别名
来源：http://hz.tanke756.top/gtqwxuabcz.html

UserId = int
来源：http://hz.yanxiufei.cn/gtskwwxtek.html

[U29] Py：属性校验
来源：http://hz.birdmap.top/gtwquwotag.html

@property 与 @x.setter 配合
来源：http://hz.hnqzz.top/gtamkbelhf.html

[U30] Py：数据类
来源：http://hz.meibo888.top/gtxocezhno.html

@dataclass(slots=True)
来源：http://hz.wangshuangyany.cn/gtttiwrvxv.html

[U31] Py：单测
来源：http://hz.jiagoushi.top/gthrwrbmcu.html

python -m pytest -q
来源：http://hz.zhixingplan.top/gtcvagmjki.html

[U32] Py：代码格式化
来源：http://hz.dianchejie.cn/gtdejzvxmi.html

ruff format . && ruff check --fix .
来源：http://hz.jinqigfzy.top/gtldwidvqh.html

[U33] Py：打包发布
来源：http://hz.52xcode.cn/gtgwuiwqws.html

python -m build  （依赖 pyproject.toml）
来源：http://hz.ivvv.top/gtkczznoht.html

[U34] Py：判断编码
来源：http://hz.zhiwuduotai.top/gticnozinf.html

chardet.detect(raw)
来源：http://hz.tianlin.xyz/gtwfvvsrhs.html

[U35] Py：发送邮件
来源：http://hz.daria6918.cn/gtooazaqxf.html

smtplib.SMTP_SSL(...).send_message(msg)
来源：http://hz.316326.xyz/gtjmnjbicq.html

[U36] Py：定时任务
来源：http://hz.kuanghao11.cn/gtuihqpdvu.html

schedule.every(10).minutes.do(job)
来源：http://hz.bjfxy.top/gtpdxymwml.html

[U37] Py：读写 Excel
来源：http://hz.zhiwuduotai.top/gtrlqptunf.html

pandas.read_excel / DataFrame.to_excel
来源：http://hz.nwbrower.top/gtdkmvbtwa.html

[U38] Py：获取脚本所在目录
来源：http://hz.xuetiantiany.cn/gtafpjyfdb.html

Path(__file__).resolve().parent
来源：http://hz.316326.xyz/gtlsblyflv.html

[U39] Py：判断是否在交互环境
来源：http://hz.yj20258.top/gtymijywrk.html

sys.stdout.isatty()
来源：http://hz.zhoulong.xyz/gtbpfvkbrp.html

[U40] Py：打印到标准错误
来源：http://hz.ivvv.top/gtsninvyzp.html

print("err", file=sys.stderr)
来源：http://hz.nanxinkj.top/gttvsgpcfw.html

[U41] PHP：初始化 Composer 项目
来源：http://hz.vqdsnc.cn/gtyivobtbz.html

composer init;  composer require guzzlehttp/guzzle
来源：http://hz.cashguo.top/gtrhghcisz.html

[U42] PHP：PSR-4 自动加载
来源：http://hz.vqdsnc.cn/gtcrvmpfic.html

"autoload": { "psr-4": { "App\\": "src/" } }
来源：http://hz.zhaomingkeji.xyz/gtdxnbmzua.html

[U43] PHP：声明命名空间
来源：http://hz.gotoacloud.top/gtseeqnlex.html

namespace App\Http;
来源：http://hz.ydzc1.top/gtfqutfddt.html

[U44] PHP：开启严格类型
来源：http://hz.jianghu66.top/gtkoztbjow.html

declare(strict_types=1);
来源：http://hz.jqgufenzy.top/gtwexepvbb.html

[U45] PHP：类型声明与返回类型
来源：http://hz.ydzc1.top/gtzsakcgpz.html

function add(int $a, int $b): int { return $a + $b; }
来源：http://hz.zhiwuduotai.top/gttkmpbmxb.html

[U46] PHP：可空类型
来源：http://hz.hnqzz.top/gtiilkvxgb.html

?string $name = null
来源：http://hz.ybcxt.top/gtjzomaslp.html

[U47] PHP：联合类型
来源：http://hz.gaohongyu789.top/gtyrcyivze.html

int|string $id
来源：http://hz.wangdashe.top/gtutkazlaa.html

[U48] PHP：纯枚举
来源：http://hz.kuanghao11.cn/gtshvrekkd.html

enum Status: string { case Active = "active"; case Off = "off"; }
来源：http://hz.yj20258888.top/gtcxtmnblz.html

[U49] PHP：只读属性
来源：http://hz.hammf.cn/gtnmivmzhb.html

public readonly string $name
来源：http://hz.ehwqpu.com/gtevfywlgs.html

[U50] PHP：构造器属性提升
来源：http://hz.wangshuangyany.cn/gtqxdfkfzq.html

public function __construct(private int $id) {}
来源：http://hz.quarkkingdee.top/gtvyplzijz.html

[U51] PHP：数组解构
来源：http://hz.guowangkeji.top/gteoiqzams.html

[$a, $b] = $arr;
来源：http://hz.shanyushiyangkeji.top/gthhiliist.html

[U52] PHP：箭头函数
来源：http://hz.xingfuxueyuan.xyz/gtmyukltsj.html

$double = fn($x) => $x * 2;
来源：http://hz.fengsongda.top/gtmnpdcuun.html

[U53] PHP：空合并运算符
来源：http://hz.tianlin.xyz/gtjkpvwent.html

$v = $a ?? $b ?? "default";
来源：http://hz.tianlin.xyz/gtalzspuve.html

[U54] PHP：空安全调用
来源：http://hz.yongpay.top/gtvygyateb.html

$obj?->method()
来源：http://hz.c1oappe.top/gttegbdlkc.html

[U55] PHP：match 表达式
来源：http://hz.zhijiandao.cn/gtyrbfldmo.html

$s = match($x) { 1 => "一", default => "其他" };
来源：http://hz.haohaochexian.top/gtgxlbpbrf.html

[U56] PHP：命名参数
来源：http://hz.kuanghao11.cn/gtplaberjr.html

f(a: 1, b: 2)
来源：http://hz.yanxiufei.cn/gtjvggjppi.html

[U57] PHP：字符串插值
来源：http://hz.tianlin.xyz/gtixxkkiwb.html

"值: {$a}"
来源：http://hz.vqdsnc.cn/gtrjoehatc.html

[U58] PHP：数组三件套
来源：http://hz.shuidangran.top/gtwkfxqbwx.html

array_map($f, $a);  array_filter($a, $f);  array_reduce($a, $f, 0);
来源：http://hz.hywenlv.cn/gtnnciirsu.html

[U59] PHP：自定义排序
来源：http://hz.hongshengwenyu.top/gtihjcxyan.html

usort($arr, fn($a, $b) => $a["age"] <=> $b["age"]);
来源：http://hz.guowangkeji.top/gtwmjmorwy.html

[U60] PHP：JSON 编解码
来源：http://hz.xinyue.icu/gtbitozrtc.html

json_encode($d, JSON_UNESCAPED_UNICODE);  json_decode($s, true);
来源：http://hz.cdnleiting.top/gtnvffkzzr.html

[U61] PHP：正则
来源：http://hz.mhx1999.top/gtdebesgtg.html

preg_match('/(\d+)/', $s, $m);  preg_replace('/\d+/', '#', $s);
来源：http://hz.meibo888.top/gtarztsizo.html

[U62] PHP：日期对象
来源：http://hz.nwbrower.top/gtqcwunsbe.html

(new DateTimeImmutable())->format("Y-m-d");
来源：http://hz.vqdsnc.cn/gtfodbzkgv.html

[U63] PHP：文件读写
来源：http://hz.dianchejie.cn/gtspycjtkl.html

file_get_contents($f);  file_put_contents($f, $data);
来源：http://hz.hfpthk.cn/gtpigsiyko.html

[U64] PHP：目录遍历
来源：http://hz.quarkkingdee.top/gtvvjymsmi.html

glob("dir/*.php");  scandir("dir");
来源：http://hz.smart0.xyz/gtcnxhkdns.html


<!-- 参考信息 -->