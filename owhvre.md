代发 wailian999

[S35] C++：map
来源：http://hz.aibaodan.cn/gtcdoejzbe.html

std::map<std::string, int> m;  m["a"] = 1;
来源：http://hz.cucudq.cn/gtvvztojiv.html

[S36] C++：unordered_map
来源：http://hz.jinqigufen.top/gtckotccew.html

std::unordered_map<std::string, int> m;  m["a"] = 1;
来源：http://hz.jiagoushi.top/gtvivnatqy.html

[S37] C++：set
来源：http://hz.ywan-chungtsiang.top/gtktqzymyl.html

std::set<int> s{1, 2, 3};  s.insert(4);
来源：http://hz.kuanghao11.cn/gtsmehzney.html

[S38] C++：排序
来源：http://hz.daxiang520.top/gtqgsnccly.html

std::sort(v.begin(), v.end());
来源：http://hz.tian-w.cn/gteuvnvvtc.html

[S39] C++：自定义比较器排序
来源：http://hz.ybcxt.top/gtdcpatpyz.html

std::sort(v.begin(), v.end(), [](int a, int b) { return a > b; });
来源：http://hz.yj20258.top/gtykmtjocv.html

[S40] C++：查找元素
来源：http://hz.wangshuangyany.cn/gtqzxnrjez.html

auto it = std::find(v.begin(), v.end(), 3);
来源：http://hz.zdqjudy.top/gtnsjxtgnb.html

[S41] C++：类与构造函数
来源：http://hz.smart0.xyz/gtikxldedz.html

class A { public: A(int v) : x_(v) {} int get() const { return x_; } private: int x_; };
来源：http://hz.yj202588.top/gtbbgutkms.html

[S42] C++：继承与虚函数
来源：http://hz.svipenyu.cn/gtzeuvgyxt.html

class B : public Base { public: void f() override {} };
来源：http://hz.xuetiantiany.cn/gtrivvmoij.html

[S43] C++：智能指针
来源：http://hz.yueranfly.top/gtotfzxzcz.html

auto p = std::make_unique<int>(5);
来源：http://hz.cqqwz.cn/gtflydxjjj.html

[S44] C++：引用传参
来源：http://hz.shanyushiyangkeji.top/gtlxcbtgtm.html

void inc(int &x) { ++x; }
来源：http://hz.tanke756.top/gtheeausyl.html

[S45] C++：lambda
来源：http://hz.jinqigufen.top/gtryiyyqze.html

auto add = [](int a, int b) { return a + b; };
来源：http://hz.cheryme.top/gtqfsmdqsg.html

[S46] C++：函数模板
来源：http://hz.yongpay.top/gtuxnndijd.html

template <typename T> T maxv(T a, T b) { return a > b ? a : b; }
来源：http://hz.jiagoushi.top/gtophzunmb.html

[S47] C++：结构化绑定遍历
来源：http://hz.yuanzhike.top/gtdpkrxjcc.html

for (const auto &[k, v] : m) { std::cout << k << v; }
来源：http://hz.fzhhl.top/gtxtesikci.html

[S48] C++：逐行读文件
来源：http://hz.jinqigfzy.top/gtiebfwofq.html

std::ifstream in("a.txt");  std::string line;
来源：http://hz.316326.xyz/gtlhxkwjwr.html

while (std::getline(in, line)) { }
来源：http://hz.zhengqikj.top/gtkrmfgjpi.html

[S49] C++：写文件
来源：http://hz.hywenlv.cn/gtcpjkynxs.html

std::ofstream out("a.txt");  out << "hi\n";
来源：http://hz.yanxiufei.cn/gtiqyuczxg.html

[S50] C++：格式化数字
来源：http://hz.wangshuangyany.cn/gtuubkuqpi.html

std::ostringstream os;  os << std::fixed << std::setprecision(2) << 3.14159;
来源：http://hz.birdmap.top/gtiwsqievl.html

[S51] C++：显式类型转换
来源：http://hz.xylfe.cn/gtcrgygitk.html

static_cast<double>(a) / b
来源：http://hz.jinqigufen.top/gtdrzqafjr.html

[S52] C++：const 与 noexcept
来源：http://hz.yvedp.cn/gtghyhlgvx.html

int size() const noexcept { return n_; }
来源：http://hz.yj20258888.top/gtpudcaovi.html

[S53] C++：移动语义
来源：http://hz.feifeiyinyue.top/gtzmoxnsfd.html

std::vector<int> w = std::move(v);
来源：http://hz.fzhhl.top/gtgvovppph.html

[S54] C++：异常处理
来源：http://hz.gotoacloud.top/gtqovmvmje.html

try { throw std::runtime_error("x"); } catch (const std::exception &e) { }
来源：http://hz.jinqigufen.top/gtofbtoibn.html

[S55] C++：结构化绑定
来源：http://hz.jqgfzy.top/gtvkrqkrfw.html

auto [a, b] = std::make_pair(1, 2);
来源：http://hz.andypj.xyz/gthawrmnpp.html

[S56] C++：optional
来源：http://hz.ywan-chungtsiang.top/gtpbnlxyiy.html

std::optional<int> o = 5;  if (o) { int v = *o; }
来源：http://hz.snrcjt.cn/gtbmuoxboc.html

[S57] C++：编译期常量
来源：http://hz.yj20258888.top/gthxdjcrzn.html

constexpr int N = 10;
来源：http://hz.jianghu66.top/gtqsvsezsf.html

[S58] C++：命名空间
来源：http://hz.pengpengdd.cyou/gtcsveimuk.html

namespace ns { int f() { return 1; } }
来源：http://hz.xingfuxueyuan.xyz/gtthxbhppb.html

[S59] C++：静态断言
来源：http://hz.haohaochexian.top/gtqtwnimkq.html

static_assert(sizeof(int) == 4, "int 必须 4 字节");
来源：http://hz.daxiang520.top/gtdddpgglx.html

[S60] C++：遍历并删除元素
来源：http://hz.shanyushiyangtech.top/gtrqloqwdj.html

v.erase(std::remove_if(v.begin(), v.end(), [](int x) { return x < 0; }), v.end());
来源：http://hz.jqgfzy.top/gtbvsyozro.html

================================================================================
来源：http://hz.shanyushiyangkeji.top/gtzywfxosn.html

T. 其他语言补充（Kotlin / Swift / Lua / Perl / Scala）
来源：http://hz.chenzaomai.com/gtgwstjawx.html

================================================================================
来源：http://hz.mhx1999.top/gtwkohfmgp.html

[T01] Kotlin：Hello World
来源：http://hz.9152youxi.cn/gtehisomge.html

println("Hello")
来源：http://hz.gotoacloud.top/gtzwljmufr.html

[T02] Kotlin：变量
来源：http://hz.tanke756.top/gtyyuhvoxy.html

val a = 1;  var b = 2        // val 只读，var 可变
来源：http://hz.daria6918.cn/gtivpvfjik.html

[T03] Kotlin：字符串模板
来源：http://hz.xylfe.cn/gtyljmatpo.html

"值: $b"
来源：http://hz.cashguo.top/gtjvgrmyep.html

[T04] Kotlin：空安全
来源：http://hz.yuxming.cn/gtmjqqawre.html

val n: String? = null;  n?.length
来源：http://hz.mhx1999.top/gtxafkluyu.html

[T05] Kotlin：when 表达式
来源：http://hz.quarkkingdee.top/gtjrmeixwc.html

val s = when (x) { 1 -> "一" else -> "其他" }   // 多分支时每个分支单独一行
来源：http://hz.andypj.xyz/gtyrwgqtat.html

[T06] Kotlin：集合映射
来源：http://hz.svipenyu.cn/gtucwbiztp.html

listOf(1, 2, 3).map { it * 2 }
来源：http://hz.aibaodan.cn/gtyopdedek.html

[T07] Kotlin：集合过滤
来源：http://hz.xuetiantiany.cn/gtykpafawq.html

listOf(1, 2, 3).filter { it > 1 }
来源：http://hz.yongpay.top/gtfklyqliz.html

[T08] Kotlin：数据类
来源：http://hz.haohaochexian.top/gtimnvowvi.html

data class User(val name: String, val age: Int)
来源：http://hz.ybcxt.top/gtwvazttme.html

[T09] Kotlin：扩展函数
来源：http://hz.shanyushiyangkeji.top/gtcosszfnx.html

fun String.exclaim() = this + "!"
来源：http://hz.ybcxt.top/gtaladktco.html

[T10] Kotlin：默认参数
来源：http://hz.jinqigfzy.top/gtxexxnicz.html

fun greet(name: String = "World") = "Hi $name"
来源：http://hz.shangyingyoupin.top/gtnfkffvuv.html

[T11] Kotlin：协程
来源：http://hz.jinqigfzy.top/gtgyybuxuc.html

GlobalScope.launch { delay(1000); println("done") }
来源：http://hz.hywenlv.cn/gtynifselw.html

[T12] Kotlin：解构声明
来源：http://hz.hnqzz.top/gtgzzwmiho.html

val (a, b) = Pair(1, 2)
来源：http://hz.ybcxt.top/gtozbbhwwm.html

[T13] Kotlin：只读 Map
来源：http://hz.hfpthk.cn/gtqjvkdcpm.html

val m = mapOf("a" to 1)
来源：http://hz.xingfuxueyuan.xyz/gtsuqxyiwh.html

[T14] Kotlin：循环
来源：http://hz.jqgufenzy.top/gtypuqfcbi.html

for (i in 1..10) println(i)
来源：http://hz.guannengcc.top/gthwwylsok.html

[T15] Kotlin：接口
来源：http://hz.sweek.top/gtcfrvjwlm.html

interface Shape { fun area(): Double }
来源：http://hz.ydjk.org.cn/gtbfqppoor.html

[T16] Swift：Hello World
来源：http://hz.hongshengwenyu.top/gtxblrnusg.html

print("Hello")
来源：http://hz.hnqzz.top/gttckcpssu.html

[T17] Swift：变量与常量
来源：http://hz.havefunace.top/gtwcbipyzl.html

var a = 1;  let b = 2
来源：http://hz.sweek.top/gtprocrysu.html

[T18] Swift：字符串插值
来源：http://hz.snrcjt.cn/gtnulkaovy.html

"值: \(b)"
来源：http://hz.shzxlz.cn/gtpqdsmnfr.html

[T19] Swift：可选绑定
来源：http://hz.cashguo.top/gtqiyqsizl.html

if let n = opt { print(n) }
来源：http://hz.quarkkingdee.top/gtkzwbsoav.html

[T20] Swift：数组操作
来源：http://hz.sweek.top/gtgjwkeafp.html

var a = [1, 2, 3];  a.append(4)
来源：http://hz.wangshuangyany.cn/gtvdoazusv.html

[T21] Swift：遍历
来源：http://hz.jianghu66.top/gtiskkipum.html

for x in a { print(x) }
来源：http://hz.gogol.net.cn/gtrxfskcft.html

[T22] Swift：字典
来源：http://hz.cdnleiting.top/gtsykmkqvg.html

var d = ["a": 1];  d["b"] = 2
来源：http://hz.pycfn.com/gtgvgcrdfp.html

[T23] Swift：函数
来源：http://hz.xylfe.cn/gttsiyknwc.html

func add(_ a: Int, _ b: Int) -> Int { a + b }
来源：http://hz.yangfankeji.com/gtkxkztmbe.html

[T24] Swift：闭包
来源：http://hz.cheryme.top/gtybcnxfon.html

let f = { (x: Int) -> Int in x * 2 }
来源：http://hz.316326.xyz/gtaxloerhw.html

[T25] Swift：结构体
来源：http://hz.shangyingyoupin.top/gtixabskll.html

struct P { var x: Int }
来源：http://hz.aizwys.cn/gtdvzazbvo.html

[T26] Swift：类与重写
来源：http://hz.dianchejie.cn/gtziixyxxr.html

class A: Base { override func f() {} }
来源：http://hz.jinqigfzy.top/gtkrpfkmts.html

[T27] Swift：错误处理
来源：http://hz.redwolf501.top/gtimklgfgv.html

do { try f() } catch { print(error) }
来源：http://hz.shanyushiyangkeji.top/gtqowtixrb.html

[T28] Swift：枚举
来源：http://hz.hfpthk.cn/gtocffccal.html

enum Color { case red, green }
来源：http://hz.yj20258888.top/gtkzcvpbdp.html

[T29] Swift：guard 提前返回
来源：http://hz.nanxuanxn.top/gtjicpkuzz.html

guard let x = opt else { return }
来源：http://hz.mhx1999.top/gtkikciknl.html

[T30] Swift：协议
来源：http://hz.jyoumei.cn/gtcbqwfgmm.html

protocol Shape { func area() -> Double }
来源：http://hz.nanxinkj.top/gtyewmbhaz.html

[T31] Lua：Hello World
来源：http://hz.chenlongwang.top/gtpjndlcvo.html

print("Hello")
来源：http://hz.iojbl.cn/gtscmqfnoh.html

[T32] Lua：局部变量
来源：http://hz.nanxuanxn.top/gtnwsldlsx.html

local a = 1
来源：http://hz.xziqi.cn/gtjeqrqalx.html

[T33] Lua：表（数组）
来源：http://hz.wangdashe.top/gtpkexwvnw.html

local t = {1, 2, 3};  t[4] = 4
来源：http://hz.zhengqikj.top/gtdpqmoyhx.html

[T34] Lua：遍历表
来源：http://hz.ehwqpu.com/gtlrlbhtmf.html

for i, v in ipairs(t) do print(i, v) end
来源：http://hz.xylfe.cn/gtgcscfhog.html

[T35] Lua：字典表
来源：http://hz.gzhubu.top/gtezixwokv.html

local d = { a = 1 };  d.b = 2
来源：http://hz.0kj1m.cn/gtgzgkmjql.html

[T36] Lua：函数
来源：http://hz.redwolf501.top/gtziihozpc.html

function add(a, b) return a + b end
来源：http://hz.hammf.cn/gtmafnnjdx.html

[T37] Lua：字符串拼接
来源：http://hz.cheryme.top/gtauccvynx.html

"a" .. "b"
来源：http://hz.hammf.cn/gtuwgfgqkv.html

[T38] Lua：条件
来源：http://hz.zhongyouzk.top/gttdskiyzg.html

if x > 0 then print("正") end
来源：http://hz.cheryme.top/gttyyszgqt.html

[T39] Lua：模式匹配
来源：http://hz.yanxiufei.cn/gtptuikpep.html

string.find(s, "%d+")
来源：http://hz.dashuyun.cn/gtdhpuemmt.html

[T40] Lua：元表
来源：http://hz.yueranfly.top/gtwydzdyrx.html

setmetatable({}, { __index = base })
来源：http://hz.zhixingplan.top/gtcoofppcr.html

[T41] Perl：Hello World
来源：http://hz.yj202588.top/gtrhvjvkkf.html

print "Hello\n";
来源：http://hz.hnqzz.top/gtuxnmudal.html

[T42] Perl：变量类型
来源：http://hz.gzhubu.top/gtnmwcozwa.html

my $a = 1;  my @arr = (1, 2, 3);  my %h = (a => 1);
来源：http://hz.pengpengdd.cyou/gtppmjwkty.html

[T43] Perl：字符串插值
来源：http://hz.sufxvd.cn/gtbfjleqbq.html

"值: $a"
来源：http://hz.xinyue.icu/gtxszjspiv.html

[T44] Perl：条件
来源：http://hz.vqdsnc.cn/gtwutgjksf.html

if ($a > 0) { print "正"; }
来源：http://hz.jinghuilouyu.cn/gtdcsukldb.html

[T45] Perl：数组遍历
来源：http://hz.xylfe.cn/gtphzxfyoi.html

for my $x (@arr) { print $x; }
来源：http://hz.jqgufenzy.top/gtgdxsepuq.html

[T46] Perl：哈希操作
来源：http://hz.kuanghao11.cn/gtumqfzgkr.html

$h{b} = 2;  for my $k (keys %h) { print "$k=$h{$k}"; }
来源：http://hz.jiagoushi.top/gtbnigbtcf.html

[T47] Perl：正则捕获
来源：http://hz.gogol.net.cn/gtcdfbcbnz.html

if ($s =~ /(\d+)/) { print $1; }
来源：http://hz.yueranfly.top/gtytaxvlbt.html

[T48] Perl：正则替换
来源：http://hz.bjfxy.top/gtqvmdqexz.html

$s =~ s/old/new/g;
来源：http://hz.sxryk.cn/gtgckmoytl.html

[T49] Perl：函数
来源：http://hz.9152youxi.cn/gtujridolg.html

sub add { my ($a, $b) = @_; return $a + $b; }
来源：http://hz.svipenyu.cn/gtsohadiob.html

[T50] Perl：逐行读文件
来源：http://hz.zdqjudy.top/gtxtyqnulr.html

open my $fh, "<", "a.txt" or die $!;
来源：http://hz.yangfankeji.com/gtymqvajup.html

while (my $line = <$fh>) { print $line; }
来源：http://hz.ydzc1.top/gtvlenbxvr.html

[T51] Scala：Hello World
来源：http://hz.daxiang520.top/gtviefkqzk.html

println("Hello")
来源：http://hz.jinyuanbaomall.cn/gthpenetdz.html

[T52] Scala：变量
来源：http://hz.c1oappe.top/gtatxkfnko.html

val a = 1;  var b = 2
来源：http://hz.ivvv.top/gtkyanqprs.html

[T53] Scala：字符串插值
来源：http://hz.quarkkingdee.top/gtcarpxgay.html

s"值: $b"
来源：http://hz.hnxiangtu.top/gttenwitiz.html

[T54] Scala：集合映射
来源：http://hz.xziqi.cn/gtfxdegjto.html

List(1, 2, 3).map(_ * 2)
来源：http://hz.yonumen.top/gtdszdupgu.html

[T55] Scala：集合过滤
来源：http://hz.bjfxy.top/gterbycxaj.html

List(1, 2, 3).filter(_ > 1)
来源：http://hz.ivvv.top/gtvkhnteat.html

[T56] Scala：样例类
来源：http://hz.kuanghao11.cn/gtpupzmjot.html

case class User(name: String, age: Int)
来源：http://hz.yanxiufei.cn/gttvwxcmop.html

[T57] Scala：模式匹配
来源：http://hz.zhijiandao.cn/gtizbfsrcp.html

x match { case 1 => "一"; case _ => "其他" }
来源：http://hz.ydjk.org.cn/gtqtocimvj.html

[T58] Scala：函数定义
来源：http://hz.chenzaomai.com/gtwvgeieuu.html

def add(a: Int, b: Int): Int = a + b
来源：http://hz.jinyuanbaomall.cn/gtyajocjis.html

[T59] Scala：循环
来源：http://hz.chenzaomai.com/gtuxngcztk.html

for (i <- 1 to 10) println(i)
来源：http://hz.c1oappe.top/gturbaryzy.html

[T60] Scala：折叠
来源：http://hz.birdmap.top/gtkkqqmgcu.html

List(1, 2, 3).foldLeft(0)(_ + _)
来源：http://hz.bjfxy.top/gtyyysexak.html

================================================================================
来源：http://hz.daxiang520.top/gtrabkaaeo.html

U. 高频实用片段（Python / PHP / JavaScript 各 40 条）
来源：http://hz.aizwys.cn/gttbylsreo.html

================================================================================
来源：http://hz.jinghuilouyu.cn/gtppmblbwj.html

[U01] Py：创建虚拟环境
来源：http://hz.hnqzz.top/gtxmidhohl.html

python -m venv .venv && source .venv/bin/activate
来源：http://hz.iojbl.cn/gtyjflluhi.html

[U02] Py：导出 / 安装依赖
来源：http://hz.sxryk.cn/gtfqmgmajh.html

pip freeze > requirements.txt;  pip install -r requirements.txt
来源：http://hz.shangyingyoupin.top/gtmydnetyi.html

[U03] Py：加载 .env 配置
来源：http://hz.daria6918.cn/gtaibrycjh.html

from dotenv import load_dotenv; load_dotenv()
来源：http://hz.jqgfzy.top/gtomlnbglk.html

[U04] Py：变量调试打印
来源：http://hz.jiagoushi.top/gtyuuvjxzz.html

print(f"{x=}")            # 输出 x=值，Python 3.8+
来源：http://hz.wangdashe.top/gtbxltfemd.html

[U05] Py：列表去重且保序
来源：http://hz.wangshuangyany.cn/gthoadvwqp.html

list(dict.fromkeys(arr))
来源：http://hz.fzhhl.top/gtggwcsuck.html

[U06] Py：合并两个字典
来源：http://hz.zhiwuduotai.top/gtqthxmhbm.html

{**a, **b}
来源：http://hz.birdmap.top/gtjdtcpsmr.html

[U07] Py：反转字典键值
来源：http://hz.hfpthk.cn/gtsvglanlt.html

{v: k for k, v in d.items()}
来源：http://hz.gogol.net.cn/gtitiypobe.html

[U08] Py：展平二维列表
来源：http://hz.daria6918.cn/gtndfciqkd.html

[y for x in nested for y in x]
来源：http://hz.hywenlv.cn/gtuacukzer.html

[U09] Py：字典取最大值的键
来源：http://hz.zhiwuduotai.top/gtguwmohvw.html

max(d, key=d.get)
来源：http://hz.meibo888.top/gtkaufqupr.html

[U10] Py：按值排序字典
来源：http://hz.hnqzz.top/gtrlnaprvk.html

dict(sorted(d.items(), key=lambda kv: kv[1]))
来源：http://hz.xuetiantiany.cn/gtfunowpkl.html

[U11] Py：生成器表达式
来源：http://hz.chenjidiqi.icu/gtezoaahji.html

(x * 2 for x in arr)
来源：http://hz.ydjk.org.cn/gtzcarouqh.html

[U12] Py：取出现最多的 3 个元素
来源：http://hz.xuetiantiany.cn/gtktcfuwxg.html

Counter(arr).most_common(3)
来源：http://hz.xingfuxueyuan.xyz/gtldmeedpq.html

[U13] Py：固定长度队列
来源：http://hz.aibaodan.cn/gthtasirqp.html

deque(maxlen=10)
来源：http://hz.sysykeji.top/gtmgstfjls.html

[U14] Py：分组收集到列表
来源：http://hz.snrcjt.cn/gtxrkmlgze.html

defaultdict(list)
来源：http://hz.shangyingyoupin.top/gtgubjuhin.html

[U15] Py：高精度计时
来源：http://hz.kuanghao11.cn/gtgzbrephb.html

t = time.perf_counter()
来源：http://hz.fzhhl.top/gtajvzamcq.html

[U16] Py：命令行参数解析
来源：http://hz.guannengcc.top/gtnznpuqvh.html

ap = argparse.ArgumentParser();  ap.add_argument("--name");  args = ap.parse_args()
来源：http://hz.havefunace.top/gtzydhufhn.html

[U17] Py：初始化日志
来源：http://hz.yuxming.cn/gtjlzvzlvs.html

logging.basicConfig(level=logging.INFO)
来源：http://hz.dashuyun.cn/gtbxeqqasl.html

[U18] Py：预编译正则
来源：http://hz.dashuyun.cn/gtwovwhlfy.html

pat = re.compile(r"\d+")
来源：http://hz.meibo888.top/gtobcldkqo.html

[U19] Py：正则替换带回调
来源：http://hz.wangshuangyany.cn/gtalhrlvmy.html

re.sub(r"\d+", lambda m: str(int(m.group()) * 2), s)
来源：http://hz.cdnleiting.top/gtxqpengmf.html

[U20] Py：缓存函数结果
来源：http://hz.zhoulong.xyz/gtvvvsnlhn.html

@functools.lru_cache(maxsize=None)
来源：http://hz.aizwys.cn/gtexzxuksp.html

[U21] Py：自定义上下文管理器
来源：http://hz.cheryme.top/gthumhpfgv.html

@contextlib.contextmanager
来源：http://hz.jinqigfzy.top/gtshjkqliu.html

[U22] Py：矩阵转置
来源：http://hz.pengpengdd.cyou/gtsrhgzieg.html

list(zip(*m))
来源：http://hz.nanxuanxn.top/gtsieumabp.html

[U23] Py：分块读取大文件
来源：http://hz.yonumen.top/gtdlehjspf.html

for chunk in iter(lambda: f.read(8192), b""):
来源：http://hz.gaohongyu789.top/gtdtjvplaf.html

[U24] Py：路径操作
来源：http://hz.yj20258888.top/gtmwqmqqvm.html

Path("a/b.txt").parent.mkdir(parents=True, exist_ok=True)
来源：http://hz.xuetiantiany.cn/gtqujyhhtz.html

[U25] Py：CSV 按字典读
来源：http://hz.iojbl.cn/gtiifdlpsj.html

csv.DictReader(f)
来源：http://hz.aibaodan.cn/gtytvfpamp.html

[U26] Py：并发下载
来源：http://hz.fzhhl.top/gtvywwzroo.html

ThreadPoolExecutor(max_workers=8).map(fetch, urls)
来源：http://hz.zhoulong.xyz/gtltrhfxap.html

[U27] Py：异步 HTTP
来源：http://hz.sweek.top/gtdimdgxsq.html

aiohttp.ClientSession() 配合 async with
来源：http://hz.hnqzz.top/gtzhbufznc.html

[U28] Py：类型别名
来源：http://hz.ydzc1.top/gtjgrlefjx.html

UserId = int
来源：http://hz.xinyue.icu/gtwhbyvqso.html

[U29] Py：属性校验
来源：http://hz.xinyue.icu/gthnyytusf.html

@property 与 @x.setter 配合
来源：http://hz.pengpengdd.cyou/gtbiybqjnq.html

[U30] Py：数据类
来源：http://hz.feifeiyinyue.top/gttfkbhbks.html

@dataclass(slots=True)
来源：http://hz.guowangkeji.top/gtkplurclk.html

[U31] Py：单测
来源：http://hz.zhixingplan.top/gtxwyiwqib.html

python -m pytest -q
来源：http://hz.sysykeji.top/gtfwdlmzaz.html

[U32] Py：代码格式化
来源：http://hz.daxiang520.top/gtazexfnxk.html

ruff format . && ruff check --fix .
来源：http://hz.zycfv.cn/gtksvjiaqh.html

[U33] Py：打包发布
来源：http://hz.yj202588.top/gtmvjohhba.html

python -m build  （依赖 pyproject.toml）
来源：http://hz.yueranfly.top/gteklywcgf.html

[U34] Py：判断编码
来源：http://hz.meibo888.top/gtmuradrqe.html

chardet.detect(raw)
来源：http://hz.yueranfly.top/gtpbrvvqko.html

[U35] Py：发送邮件
来源：http://hz.smart0.xyz/gtjpexndbt.html

smtplib.SMTP_SSL(...).send_message(msg)
来源：http://hz.yuanzhike.top/gtkaocgrcq.html

[U36] Py：定时任务
来源：http://hz.snrcjt.cn/gtfyjyynst.html

schedule.every(10).minutes.do(job)
来源：http://hz.guannengcc.top/gtzktmsjop.html

[U37] Py：读写 Excel
来源：http://hz.ybcxt.top/gttqncxcpp.html

pandas.read_excel / DataFrame.to_excel
来源：http://hz.ydjk.org.cn/gtauidrlio.html

[U38] Py：获取脚本所在目录
来源：http://hz.guowangkeji.top/gtfhmulhgb.html

Path(__file__).resolve().parent
来源：http://hz.daxiang520.top/gtblgooctu.html

[U39] Py：判断是否在交互环境
来源：http://hz.316326.xyz/gtrrcoozhn.html

sys.stdout.isatty()
来源：http://hz.jiagoushi.top/gtsrmfzihp.html

[U40] Py：打印到标准错误
来源：http://hz.zhaomingkeji.xyz/gtxhrijjym.html

print("err", file=sys.stderr)
来源：http://hz.aibaodan.cn/gtjigfqeme.html

[U41] PHP：初始化 Composer 项目
来源：http://hz.chenlongwang.top/gtgmipvzss.html

composer init;  composer require guzzlehttp/guzzle
来源：http://hz.c1oappe.top/gtnqwcrdow.html

[U42] PHP：PSR-4 自动加载
来源：http://hz.hongshengwenyu.top/gtrkmgwgvd.html

"autoload": { "psr-4": { "App\\": "src/" } }
来源：http://hz.c1oappe.top/gtsfgebwsg.html

[U43] PHP：声明命名空间
来源：http://hz.jqgufenzy.top/gttbynthev.html

namespace App\Http;
来源：http://hz.zhongyouzk.top/gtiypkcapr.html

[U44] PHP：开启严格类型
来源：http://hz.cashguo.top/gttisihzsa.html

declare(strict_types=1);
来源：http://hz.haohaochexian.top/gtlprjbked.html

[U45] PHP：类型声明与返回类型
来源：http://hz.vqdsnc.cn/gtjjmlmfvy.html

function add(int $a, int $b): int { return $a + $b; }
来源：http://hz.yj20258.top/gthhhzzcgw.html

[U46] PHP：可空类型
来源：http://hz.chenlongwang.top/gtkkqlrohu.html

?string $name = null
来源：http://hz.xylfe.cn/gtejkbtjxy.html

[U47] PHP：联合类型
来源：http://hz.nanxuanxn.top/gthntpbspt.html

int|string $id
来源：http://hz.zhiwuduotai.top/gtlxbottax.html

[U48] PHP：纯枚举
来源：http://hz.yongpay.top/gtbjigrylg.html

enum Status: string { case Active = "active"; case Off = "off"; }
来源：http://hz.shangyingyoupin.top/gtrdkvospc.html

[U49] PHP：只读属性
来源：http://hz.guowangkeji.top/gtbbedhakr.html

public readonly string $name
来源：http://hz.hfpthk.cn/gtbnuuolms.html

[U50] PHP：构造器属性提升
来源：http://hz.sufxvd.cn/gtqljvgzvu.html

public function __construct(private int $id) {}
来源：http://hz.sysykeji.top/gtwydnctwr.html

[U51] PHP：数组解构
来源：http://hz.yvedp.cn/gtiqjxjhup.html

[$a, $b] = $arr;
来源：http://hz.zycfv.cn/gthfanizpr.html

[U52] PHP：箭头函数
来源：http://hz.ydzc1.top/gtaborusik.html

$double = fn($x) => $x * 2;
来源：http://hz.ppjwa.cn/gtgwolyywr.html

[U53] PHP：空合并运算符
来源：http://hz.zhiwuduotai.top/gtuylnxpqc.html

$v = $a ?? $b ?? "default";
来源：http://hz.chenzaomai.com/gtitcgyhfz.html

[U54] PHP：空安全调用
来源：http://hz.zhaomingkeji.xyz/gtecevjegi.html

$obj?->method()
来源：http://hz.xuanzx.com/gtbdjnnlpm.html

[U55] PHP：match 表达式
来源：http://hz.shangyingyoupin.top/gtgrhssnch.html

$s = match($x) { 1 => "一", default => "其他" };
来源：http://hz.jinghuilouyu.cn/gtkprqpkxu.html

[U56] PHP：命名参数
来源：http://hz.nwbrower.top/gtteamjdyj.html

f(a: 1, b: 2)
来源：http://hz.vqdsnc.cn/gtoktkkzqp.html

[U57] PHP：字符串插值
来源：http://hz.316326.xyz/gtnehbthqd.html

"值: {$a}"
来源：http://hz.xuetiantiany.cn/gttkrsgtvt.html

[U58] PHP：数组三件套
来源：http://hz.nanxuanxn.top/gtelpzheib.html

array_map($f, $a);  array_filter($a, $f);  array_reduce($a, $f, 0);
来源：http://hz.ivvv.top/gtqasiruwf.html

[U59] PHP：自定义排序
来源：http://hz.haohaochexian.top/gtstbveeic.html

usort($arr, fn($a, $b) => $a["age"] <=> $b["age"]);
来源：http://hz.tianlin.xyz/gtlvmppkyc.html

[U60] PHP：JSON 编解码
来源：http://hz.cashguo.top/gttqfxuhfv.html

json_encode($d, JSON_UNESCAPED_UNICODE);  json_decode($s, true);
来源：http://hz.hnxiangtu.top/gtrogpkbse.html


<!-- 参考信息 -->