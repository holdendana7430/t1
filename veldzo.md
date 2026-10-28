代发 wailian999

[S41] C++：类与构造函数
来源：http://hz.jiagoushi.top/gtedsqhgis.html

class A { public: A(int v) : x_(v) {} int get() const { return x_; } private: int x_; };
来源：http://hz.tianlin.xyz/gtluahbrul.html

[S42] C++：继承与虚函数
来源：http://hz.cheryme.top/gttitlrzxj.html

class B : public Base { public: void f() override {} };
来源：http://hz.yvedp.cn/gtzyehczbb.html

[S43] C++：智能指针
来源：http://hz.pycfn.com/gtoqfbzdvq.html

auto p = std::make_unique<int>(5);
来源：http://hz.ehwqpu.com/gtzvjdplie.html

[S44] C++：引用传参
来源：http://hz.jianghu66.top/gtwdkzmtzx.html

void inc(int &x) { ++x; }
来源：http://hz.hammf.cn/gttxhnnxfo.html

[S45] C++：lambda
来源：http://hz.aizwys.cn/gthxjwrsxz.html

auto add = [](int a, int b) { return a + b; };
来源：http://hz.fzhhl.top/gttyliamjm.html

[S46] C++：函数模板
来源：http://hz.yangfankeji.com/gtoteeoxai.html

template <typename T> T maxv(T a, T b) { return a > b ? a : b; }
来源：http://hz.yangfankeji.com/gttfcjnwjo.html

[S47] C++：结构化绑定遍历
来源：http://hz.jinqigufen.top/gtxtplwjwu.html

for (const auto &[k, v] : m) { std::cout << k << v; }
来源：http://hz.dianchejie.cn/gttwoemndv.html

[S48] C++：逐行读文件
来源：http://hz.yj202588.top/gtdlgnrbyl.html

std::ifstream in("a.txt");  std::string line;
来源：http://hz.shangyingyoupin.top/gtwdrdlvgm.html

while (std::getline(in, line)) { }
来源：http://hz.ywan-chungtsiang.top/gtnvimolhy.html

[S49] C++：写文件
来源：http://hz.zhijiandao.cn/gtgswfjlht.html

std::ofstream out("a.txt");  out << "hi\n";
来源：http://hz.nwbrower.top/gtohbyuxfg.html

[S50] C++：格式化数字
来源：http://hz.cqqwz.cn/gtfrrvrybe.html

std::ostringstream os;  os << std::fixed << std::setprecision(2) << 3.14159;
来源：http://hz.wangdashe.top/gtuvmevpeh.html

[S51] C++：显式类型转换
来源：http://hz.fzhhl.top/gtvbditlwl.html

static_cast<double>(a) / b
来源：http://hz.ydzc1.top/gtghbldgeh.html

[S52] C++：const 与 noexcept
来源：http://hz.sysykeji.top/gtxbunbyhs.html

int size() const noexcept { return n_; }
来源：http://hz.hnqzz.top/gtvzeagrau.html

[S53] C++：移动语义
来源：http://hz.yvedp.cn/gtksceotzd.html

std::vector<int> w = std::move(v);
来源：http://hz.dianchejie.cn/gtnjmbgdqj.html

[S54] C++：异常处理
来源：http://hz.aibaodan.cn/gtxuzlcdnp.html

try { throw std::runtime_error("x"); } catch (const std::exception &e) { }
来源：http://hz.zhijiandao.cn/gtaxjfdbwi.html

[S55] C++：结构化绑定
来源：http://hz.bjfxy.top/gtdthgproz.html

auto [a, b] = std::make_pair(1, 2);
来源：http://hz.quarkkingdee.top/gthvtbpzac.html

[S56] C++：optional
来源：http://hz.yj20258888.top/gtosxqlvqs.html

std::optional<int> o = 5;  if (o) { int v = *o; }
来源：http://hz.9152youxi.cn/gtrvdkmwjc.html

[S57] C++：编译期常量
来源：http://hz.hammf.cn/gtnxxqzrgu.html

constexpr int N = 10;
来源：http://hz.andypj.xyz/gthuquwyow.html

[S58] C++：命名空间
来源：http://hz.hywenlv.cn/gttsdefdky.html

namespace ns { int f() { return 1; } }
来源：http://hz.xylfe.cn/gtsqquxmvk.html

[S59] C++：静态断言
来源：http://hz.jlsjyb.cn/gtnypjjsnx.html

static_assert(sizeof(int) == 4, "int 必须 4 字节");
来源：http://hz.tanke756.top/gttaixypfd.html

[S60] C++：遍历并删除元素
来源：http://hz.316326.xyz/gtswthdfvc.html

v.erase(std::remove_if(v.begin(), v.end(), [](int x) { return x < 0; }), v.end());
来源：http://hz.haohaochexian.top/gtnbclnbyw.html

================================================================================
来源：http://hz.sweek.top/gtdkqnortl.html

T. 其他语言补充（Kotlin / Swift / Lua / Perl / Scala）
来源：http://hz.jinqigufen.top/gthasgzfaw.html

================================================================================
来源：http://hz.yongpay.top/gtlqzysjti.html

[T01] Kotlin：Hello World
来源：http://hz.yongpay.top/gtqmlmyejm.html

println("Hello")
来源：http://hz.birdmap.top/gtgcurtuva.html

[T02] Kotlin：变量
来源：http://hz.gotoacloud.top/gtvusyomsl.html

val a = 1;  var b = 2        // val 只读，var 可变
来源：http://hz.tian-w.cn/gthiexpuvp.html

[T03] Kotlin：字符串模板
来源：http://hz.tanke756.top/gtllhnouez.html

"值: $b"
来源：http://hz.zycfv.cn/gtdxcyrvsd.html

[T04] Kotlin：空安全
来源：http://hz.zycfv.cn/gtqvurqdfe.html

val n: String? = null;  n?.length
来源：http://hz.kuanghao11.cn/gtbyilxwvx.html

[T05] Kotlin：when 表达式
来源：http://hz.cqqwz.cn/gtmehhuklb.html

val s = when (x) { 1 -> "一" else -> "其他" }   // 多分支时每个分支单独一行
来源：http://hz.guannengcc.top/gtdfprajvx.html

[T06] Kotlin：集合映射
来源：http://hz.dianchejie.cn/gtbfeiwyeu.html

listOf(1, 2, 3).map { it * 2 }
来源：http://hz.pengpengdd.cyou/gtqmsftqjm.html

[T07] Kotlin：集合过滤
来源：http://hz.fzhhl.top/gtmfxflodg.html

listOf(1, 2, 3).filter { it > 1 }
来源：http://hz.andypj.xyz/gtocdjnlhf.html

[T08] Kotlin：数据类
来源：http://hz.shanyushiyangkeji.top/gtgjkngpnl.html

data class User(val name: String, val age: Int)
来源：http://hz.xylfe.cn/gtcrvvgrzf.html

[T09] Kotlin：扩展函数
来源：http://hz.xuanzx.com/gtbafthwem.html

fun String.exclaim() = this + "!"
来源：http://hz.shanyushiyangkeji.top/gtiymkiqmd.html

[T10] Kotlin：默认参数
来源：http://hz.cqqwz.cn/gtupzyvukg.html

fun greet(name: String = "World") = "Hi $name"
来源：http://hz.ydjk.org.cn/gttbspaibg.html

[T11] Kotlin：协程
来源：http://hz.sxryk.cn/gtbvmkoeay.html

GlobalScope.launch { delay(1000); println("done") }
来源：http://hz.jqgufenzy.top/gtavgcmhij.html

[T12] Kotlin：解构声明
来源：http://hz.quarkkingdee.top/gtvntttcwm.html

val (a, b) = Pair(1, 2)
来源：http://hz.aibaodan.cn/gtmrztgovk.html

[T13] Kotlin：只读 Map
来源：http://hz.feifeiyinyue.top/gtzpilxkac.html

val m = mapOf("a" to 1)
来源：http://hz.hammf.cn/gtbbrrddzs.html

[T14] Kotlin：循环
来源：http://hz.yvedp.cn/gticqddxte.html

for (i in 1..10) println(i)
来源：http://hz.ybcxt.top/gtpehdfxtv.html

[T15] Kotlin：接口
来源：http://hz.daxiang520.top/gttjmyozay.html

interface Shape { fun area(): Double }
来源：http://hz.yangfankeji.com/gtmvqugpon.html

[T16] Swift：Hello World
来源：http://hz.zhengqikj.top/gtpmmghtgb.html

print("Hello")
来源：http://hz.zhaomingkeji.xyz/gtajjscohd.html

[T17] Swift：变量与常量
来源：http://hz.shanyushiyangkeji.top/gtqviesead.html

var a = 1;  let b = 2
来源：http://hz.zhijiandao.cn/gtbhurzglv.html

[T18] Swift：字符串插值
来源：http://hz.kuanghao11.cn/gtoralezqb.html

"值: \(b)"
来源：http://hz.pycfn.com/gtbbocpufu.html

[T19] Swift：可选绑定
来源：http://hz.shanyushiyangkeji.top/gttznxwahu.html

if let n = opt { print(n) }
来源：http://hz.sufxvd.cn/gtolpvubmb.html

[T20] Swift：数组操作
来源：http://hz.mhx1999.top/gtjdbajwcd.html

var a = [1, 2, 3];  a.append(4)
来源：http://hz.yvedp.cn/gtwvzrgigx.html

[T21] Swift：遍历
来源：http://hz.chenzaomai.com/gtpxshujqy.html

for x in a { print(x) }
来源：http://hz.pycfn.com/gtvecdgvnu.html

[T22] Swift：字典
来源：http://hz.ehwqpu.com/gtzlbiccul.html

var d = ["a": 1];  d["b"] = 2
来源：http://hz.nanxuanxn.top/gtblmeejrv.html

[T23] Swift：函数
来源：http://hz.xinyue.icu/gtiypbnmih.html

func add(_ a: Int, _ b: Int) -> Int { a + b }
来源：http://hz.sufxvd.cn/gtphnnsohh.html

[T24] Swift：闭包
来源：http://hz.52xcode.cn/gtfczvxydc.html

let f = { (x: Int) -> Int in x * 2 }
来源：http://hz.zhijiandao.cn/gtdvqdmmbm.html

[T25] Swift：结构体
来源：http://hz.jiagoushi.top/gtycgqngnj.html

struct P { var x: Int }
来源：http://hz.shuidangran.top/gtorjlzpij.html

[T26] Swift：类与重写
来源：http://hz.yj20258888.top/gteqzfsabg.html

class A: Base { override func f() {} }
来源：http://hz.zycfv.cn/gtsimagnnw.html

[T27] Swift：错误处理
来源：http://hz.wangdashe.top/gtpmkrvits.html

do { try f() } catch { print(error) }
来源：http://hz.ydjk.org.cn/gtvckldnpt.html

[T28] Swift：枚举
来源：http://hz.cashguo.top/gtimpacpzr.html

enum Color { case red, green }
来源：http://hz.hysaishi.cn/gtujryhzpa.html

[T29] Swift：guard 提前返回
来源：http://hz.daxiang520.top/gtyycgmjlc.html

guard let x = opt else { return }
来源：http://hz.haohaochexian.top/gtzmacpjhy.html

[T30] Swift：协议
来源：http://hz.andypj.xyz/gtkigiuqou.html

protocol Shape { func area() -> Double }
来源：http://hz.tianlin.xyz/gthkmklhdy.html

[T31] Lua：Hello World
来源：http://hz.jinqigfzy.top/gtrryjehrx.html

print("Hello")
来源：http://hz.chenlongwang.top/gtygrqfalq.html

[T32] Lua：局部变量
来源：http://hz.hongshengwenyu.top/gtzknnhptg.html

local a = 1
来源：http://hz.xinyue.icu/gtcucdroaj.html

[T33] Lua：表（数组）
来源：http://hz.sxryk.cn/gtowkxysjs.html

local t = {1, 2, 3};  t[4] = 4
来源：http://hz.birdmap.top/gtosmlrasc.html

[T34] Lua：遍历表
来源：http://hz.svipenyu.cn/gtgduqixiy.html

for i, v in ipairs(t) do print(i, v) end
来源：http://hz.tianlin.xyz/gtgrazjvrg.html

[T35] Lua：字典表
来源：http://hz.zhoulong.xyz/gtmullyskn.html

local d = { a = 1 };  d.b = 2
来源：http://hz.ywan-chungtsiang.top/gtyvviltlq.html

[T36] Lua：函数
来源：http://hz.zhijiandao.cn/gtddsfutrr.html

function add(a, b) return a + b end
来源：http://hz.yj20258.top/gtawhrzxbi.html

[T37] Lua：字符串拼接
来源：http://hz.9152youxi.cn/gtbwbvgfkr.html

"a" .. "b"
来源：http://hz.gzhubu.top/gtjxbtqpmm.html

[T38] Lua：条件
来源：http://hz.quarkkingdee.top/gtarulqoba.html

if x > 0 then print("正") end
来源：http://hz.gotoacloud.top/gtegutdnwa.html

[T39] Lua：模式匹配
来源：http://hz.redwolf501.top/gtbeblgurf.html

string.find(s, "%d+")
来源：http://hz.52xcode.cn/gtebvakzmo.html

[T40] Lua：元表
来源：http://hz.jinqigufen.top/gtkwmwjnjm.html

setmetatable({}, { __index = base })
来源：http://hz.yj20258.top/gtbunepkmi.html

[T41] Perl：Hello World
来源：http://hz.sweek.top/gtkznciscj.html

print "Hello\n";
来源：http://hz.0kj1m.cn/gtipbpvtsx.html

[T42] Perl：变量类型
来源：http://hz.sufxvd.cn/gtfowadowm.html

my $a = 1;  my @arr = (1, 2, 3);  my %h = (a => 1);
来源：http://hz.havefunace.top/gtaoricmzg.html

[T43] Perl：字符串插值
来源：http://hz.xziqi.cn/gtwprlbaif.html

"值: $a"
来源：http://hz.fengsongda.top/gtgsbutdbk.html

[T44] Perl：条件
来源：http://hz.gotoacloud.top/gtzcvrauxm.html

if ($a > 0) { print "正"; }
来源：http://hz.zhengqikj.top/gtshigufrp.html

[T45] Perl：数组遍历
来源：http://hz.xinyue.icu/gtilphooyy.html

for my $x (@arr) { print $x; }
来源：http://hz.yj20258.top/gtznxqkcvx.html

[T46] Perl：哈希操作
来源：http://hz.yueranfly.top/gtnivdzwgl.html

$h{b} = 2;  for my $k (keys %h) { print "$k=$h{$k}"; }
来源：http://hz.ywan-chungtsiang.top/gtdxrldwvl.html

[T47] Perl：正则捕获
来源：http://hz.guannengcc.top/gtdfxezsnh.html

if ($s =~ /(\d+)/) { print $1; }
来源：http://hz.kuanghao11.cn/gttonqfgaw.html

[T48] Perl：正则替换
来源：http://hz.birdmap.top/gtjvdlyemt.html

$s =~ s/old/new/g;
来源：http://hz.shangyingyoupin.top/gtfeuyshyx.html

[T49] Perl：函数
来源：http://hz.yuxming.cn/gtrhwjezea.html

sub add { my ($a, $b) = @_; return $a + $b; }
来源：http://hz.hysaishi.cn/gtuxddqoyr.html

[T50] Perl：逐行读文件
来源：http://hz.0kj1m.cn/gtbumnyzzu.html

open my $fh, "<", "a.txt" or die $!;
来源：http://hz.aibaodan.cn/gtxrbtwurl.html

while (my $line = <$fh>) { print $line; }
来源：http://hz.ehwqpu.com/gtkqmqhvlb.html

[T51] Scala：Hello World
来源：http://hz.shanyushiyangtech.top/gturcfkisj.html

println("Hello")
来源：http://hz.yangfankeji.com/gtigempbxa.html

[T52] Scala：变量
来源：http://hz.guowangkeji.top/gthaxueauf.html

val a = 1;  var b = 2
来源：http://hz.sysykeji.top/gtouhcodea.html

[T53] Scala：字符串插值
来源：http://hz.gotoacloud.top/gtvovxtbwi.html

s"值: $b"
来源：http://hz.yj202588.top/gtihnitfjt.html

[T54] Scala：集合映射
来源：http://hz.bjfxy.top/gtsixblyoa.html

List(1, 2, 3).map(_ * 2)
来源：http://hz.snrcjt.cn/gtkhhbxcxz.html

[T55] Scala：集合过滤
来源：http://hz.xinyue.icu/gtyhyhoxka.html

List(1, 2, 3).filter(_ > 1)
来源：http://hz.yangfankeji.com/gtvktjzlni.html

[T56] Scala：样例类
来源：http://hz.tianlin.xyz/gtqvitrgav.html

case class User(name: String, age: Int)
来源：http://hz.shangyingyoupin.top/gtvxvtjuel.html

[T57] Scala：模式匹配
来源：http://hz.chenjidiqi.icu/gtljfkadla.html

x match { case 1 => "一"; case _ => "其他" }
来源：http://hz.ybcxt.top/gtkohucckq.html

[T58] Scala：函数定义
来源：http://hz.zhiwuduotai.top/gtysbhfgqp.html

def add(a: Int, b: Int): Int = a + b
来源：http://hz.hfpthk.cn/gtjxgqnpvi.html

[T59] Scala：循环
来源：http://hz.chenlongwang.top/gtsywlrbvt.html

for (i <- 1 to 10) println(i)
来源：http://hz.xinyue.icu/gtrxiuzuyg.html

[T60] Scala：折叠
来源：http://hz.chenjidiqi.icu/gtrwxgmugh.html

List(1, 2, 3).foldLeft(0)(_ + _)
来源：http://hz.xuanzx.com/gthfopzbuz.html

================================================================================
来源：http://hz.yj202588.top/gtetxtkjqj.html

U. 高频实用片段（Python / PHP / JavaScript 各 40 条）
来源：http://hz.hnqzz.top/gtgzoiwidb.html

================================================================================
来源：http://hz.yj202588.top/gtnakmutsn.html

[U01] Py：创建虚拟环境
来源：http://hz.ydjk.org.cn/gtkxutnuap.html

python -m venv .venv && source .venv/bin/activate
来源：http://hz.guowangkeji.top/gtjpelxzep.html

[U02] Py：导出 / 安装依赖
来源：http://hz.meibo888.top/gtlicvgdne.html

pip freeze > requirements.txt;  pip install -r requirements.txt
来源：http://hz.pengpengdd.cyou/gtxtghbsgu.html

[U03] Py：加载 .env 配置
来源：http://hz.hysaishi.cn/gtwopldnzx.html

from dotenv import load_dotenv; load_dotenv()
来源：http://hz.9152youxi.cn/gtjtsdhugy.html

[U04] Py：变量调试打印
来源：http://hz.tian-w.cn/gtpolthslc.html

print(f"{x=}")            # 输出 x=值，Python 3.8+
来源：http://hz.haohaochexian.top/gtjbglusjd.html

[U05] Py：列表去重且保序
来源：http://hz.jinqigfzy.top/gtjpigmosc.html

list(dict.fromkeys(arr))
来源：http://hz.ivvv.top/gtqrhhsfgl.html

[U06] Py：合并两个字典
来源：http://hz.shanyushiyangkeji.top/gtzrchrlfi.html

{**a, **b}
来源：http://hz.yj20258.top/gttwvnzhwf.html

[U07] Py：反转字典键值
来源：http://hz.cashguo.top/gtvgrhwrsd.html

{v: k for k, v in d.items()}
来源：http://hz.jqgufenzy.top/gtolypknbi.html

[U08] Py：展平二维列表
来源：http://hz.zhaomingkeji.xyz/gtnwqdhrsh.html

[y for x in nested for y in x]
来源：http://hz.gotoacloud.top/gtxngpracm.html

[U09] Py：字典取最大值的键
来源：http://hz.cashguo.top/gtxkrmbphu.html

max(d, key=d.get)
来源：http://hz.jqgufenzy.top/gtrcvcxzqf.html

[U10] Py：按值排序字典
来源：http://hz.wangdashe.top/gtfgzkohks.html

dict(sorted(d.items(), key=lambda kv: kv[1]))
来源：http://hz.hywenlv.cn/gtbatlgpip.html

[U11] Py：生成器表达式
来源：http://hz.wangdashe.top/gtzxvozgbf.html

(x * 2 for x in arr)
来源：http://hz.zhixingplan.top/gthhxlpugh.html

[U12] Py：取出现最多的 3 个元素
来源：http://hz.52xcode.cn/gtfzvzflej.html

Counter(arr).most_common(3)
来源：http://hz.hammf.cn/gtladizsze.html

[U13] Py：固定长度队列
来源：http://hz.iojbl.cn/gtisekyomn.html

deque(maxlen=10)
来源：http://hz.shangyingyoupin.top/gtcmogmdjz.html

[U14] Py：分组收集到列表
来源：http://hz.guannengcc.top/gtprbkzvxr.html

defaultdict(list)
来源：http://hz.meibo888.top/gtmnoxldjo.html

[U15] Py：高精度计时
来源：http://hz.c1oappe.top/gtyuqjyyme.html

t = time.perf_counter()
来源：http://hz.yj20258.top/gtkemmefph.html

[U16] Py：命令行参数解析
来源：http://hz.jlsjyb.cn/gthfjcdtys.html

ap = argparse.ArgumentParser();  ap.add_argument("--name");  args = ap.parse_args()
来源：http://hz.yj20258.top/gtbnmlxzah.html

[U17] Py：初始化日志
来源：http://hz.0kj1m.cn/gtgwdwwyfp.html

logging.basicConfig(level=logging.INFO)
来源：http://hz.ydjk.org.cn/gtpqvijmno.html

[U18] Py：预编译正则
来源：http://hz.ywan-chungtsiang.top/gtyyvhuisj.html

pat = re.compile(r"\d+")
来源：http://hz.tianlin.xyz/gtngpuwbyv.html

[U19] Py：正则替换带回调
来源：http://hz.feifeiyinyue.top/gtxtpbcvse.html

re.sub(r"\d+", lambda m: str(int(m.group()) * 2), s)
来源：http://hz.xziqi.cn/gtyvrtkhbs.html

[U20] Py：缓存函数结果
来源：http://hz.aibaodan.cn/gtqppaoixi.html

@functools.lru_cache(maxsize=None)
来源：http://hz.sufxvd.cn/gtiimxwkzf.html

[U21] Py：自定义上下文管理器
来源：http://hz.cucudq.cn/gtiduinytv.html

@contextlib.contextmanager
来源：http://hz.jinqigufen.top/gtnwezofkc.html

[U22] Py：矩阵转置
来源：http://hz.zhixingplan.top/gtnrbojflz.html

list(zip(*m))
来源：http://hz.wangdashe.top/gtptpvvygt.html

[U23] Py：分块读取大文件
来源：http://hz.nanxuanxn.top/gtljvmdcgn.html

for chunk in iter(lambda: f.read(8192), b""):
来源：http://hz.feifeiyinyue.top/gtrhxsnhhq.html

[U24] Py：路径操作
来源：http://hz.daria6918.cn/gtigcpccgz.html

Path("a/b.txt").parent.mkdir(parents=True, exist_ok=True)
来源：http://hz.daxiang520.top/gtlyzhtbzk.html

[U25] Py：CSV 按字典读
来源：http://hz.gotoacloud.top/gtniyivhez.html

csv.DictReader(f)
来源：http://hz.zycfv.cn/gtupgnqtve.html

[U26] Py：并发下载
来源：http://hz.shanyushiyangkeji.top/gttlvdypyo.html

ThreadPoolExecutor(max_workers=8).map(fetch, urls)
来源：http://hz.c1oappe.top/gtcpalhfsz.html

[U27] Py：异步 HTTP
来源：http://hz.gotoacloud.top/gtmgdkdqxz.html

aiohttp.ClientSession() 配合 async with
来源：http://hz.yj20258.top/gtvsrhwoge.html

[U28] Py：类型别名
来源：http://hz.hnxiangtu.top/gtblqynbzn.html

UserId = int
来源：http://hz.pengpengdd.cyou/gtheruguvy.html

[U29] Py：属性校验
来源：http://hz.aibaodan.cn/gtopemkaad.html

@property 与 @x.setter 配合
来源：http://hz.zhoulong.xyz/gtkgatvgbw.html

[U30] Py：数据类
来源：http://hz.daxiang520.top/gtohbnvgbq.html

@dataclass(slots=True)
来源：http://hz.jiagoushi.top/gtjkqxtwrz.html

[U31] Py：单测
来源：http://hz.jianghu66.top/gtzkqyqnmo.html

python -m pytest -q
来源：http://hz.cashguo.top/gtklqfjnro.html

[U32] Py：代码格式化
来源：http://hz.jinyuanbaomall.cn/gtcwpzrhzn.html

ruff format . && ruff check --fix .
来源：http://hz.shanyushiyangkeji.top/gtluvzelbg.html

[U33] Py：打包发布
来源：http://hz.jlsjyb.cn/gtzgubxzez.html

python -m build  （依赖 pyproject.toml）
来源：http://hz.feifeiyinyue.top/gtnpuxnezj.html

[U34] Py：判断编码
来源：http://hz.yonumen.top/gtvmrisyhd.html

chardet.detect(raw)
来源：http://hz.yuxming.cn/gtmvukblqw.html

[U35] Py：发送邮件
来源：http://hz.daria6918.cn/gtqjucanuu.html

smtplib.SMTP_SSL(...).send_message(msg)
来源：http://hz.jqgfzy.top/gtstimehrx.html

[U36] Py：定时任务
来源：http://hz.quarkkingdee.top/gtqnmjuoum.html

schedule.every(10).minutes.do(job)
来源：http://hz.wangshuangyany.cn/gtoqirgmqr.html

[U37] Py：读写 Excel
来源：http://hz.smart0.xyz/gtqgfkauvt.html

pandas.read_excel / DataFrame.to_excel
来源：http://hz.xinyue.icu/gteekssoxh.html

[U38] Py：获取脚本所在目录
来源：http://hz.cashguo.top/gtvlqyiswa.html

Path(__file__).resolve().parent
来源：http://hz.zycfv.cn/gtwbvlosmr.html

[U39] Py：判断是否在交互环境
来源：http://hz.nanxinkj.top/gtdogtobvv.html

sys.stdout.isatty()
来源：http://hz.yvedp.cn/gtcklcumth.html

[U40] Py：打印到标准错误
来源：http://hz.hnqzz.top/gtycwrkcxj.html

print("err", file=sys.stderr)
来源：http://hz.hywenlv.cn/gtupimtvmz.html

[U41] PHP：初始化 Composer 项目
来源：http://hz.chenzaomai.com/gtpbzasake.html

composer init;  composer require guzzlehttp/guzzle
来源：http://hz.tian-w.cn/gtxrxpwxyd.html

[U42] PHP：PSR-4 自动加载
来源：http://hz.jiagoushi.top/gtqeuyxoxz.html

"autoload": { "psr-4": { "App\\": "src/" } }
来源：http://hz.pengpengdd.cyou/gtplmauugp.html

[U43] PHP：声明命名空间
来源：http://hz.ydjk.org.cn/gtzxsgesld.html

namespace App\Http;
来源：http://hz.guannengcc.top/gtgdltdxeg.html

[U44] PHP：开启严格类型
来源：http://hz.pengpengdd.cyou/gtocyxdsgu.html

declare(strict_types=1);
来源：http://hz.ppjwa.cn/gtuvuindhw.html

[U45] PHP：类型声明与返回类型
来源：http://hz.shzxlz.cn/gtglunfmef.html

function add(int $a, int $b): int { return $a + $b; }
来源：http://hz.ivvv.top/gtfiiaqrsq.html

[U46] PHP：可空类型
来源：http://hz.nwbrower.top/gtlqhyjoau.html

?string $name = null
来源：http://hz.jqgfzy.top/gtnendktjm.html

[U47] PHP：联合类型
来源：http://hz.jqgufenzy.top/gtojqjtajj.html

int|string $id
来源：http://hz.pycfn.com/gtyahrrywy.html

[U48] PHP：纯枚举
来源：http://hz.iojbl.cn/gtplgdneof.html

enum Status: string { case Active = "active"; case Off = "off"; }
来源：http://hz.smart0.xyz/gtyiwjcaai.html

[U49] PHP：只读属性
来源：http://hz.hfpthk.cn/gtiiwwkvgu.html

public readonly string $name
来源：http://hz.xingfuxueyuan.xyz/gtmsyxzxuy.html

[U50] PHP：构造器属性提升
来源：http://hz.quarkkingdee.top/gtsmyxpraw.html

public function __construct(private int $id) {}
来源：http://hz.jianghu66.top/gtnjovippp.html

[U51] PHP：数组解构
来源：http://hz.gaohongyu789.top/gtswlyyotr.html

[$a, $b] = $arr;
来源：http://hz.shuidangran.top/gtwsqtbuse.html

[U52] PHP：箭头函数
来源：http://hz.havefunace.top/gtcpywsert.html

$double = fn($x) => $x * 2;
来源：http://hz.cqqwz.cn/gtcdxilpcl.html

[U53] PHP：空合并运算符
来源：http://hz.pycfn.com/gttvlzvilw.html

$v = $a ?? $b ?? "default";
来源：http://hz.hnqzz.top/gtuujbzdui.html

[U54] PHP：空安全调用
来源：http://hz.hysaishi.cn/gtzuxelrko.html

$obj?->method()
来源：http://hz.wangdashe.top/gtezhqhpzz.html

[U55] PHP：match 表达式
来源：http://hz.chenzaomai.com/gtplrfprht.html

$s = match($x) { 1 => "一", default => "其他" };
来源：http://hz.sysykeji.top/gtsiqdmutz.html

[U56] PHP：命名参数
来源：http://hz.sysykeji.top/gtykpurarq.html

f(a: 1, b: 2)
来源：http://hz.shanyushiyangkeji.top/gtokyedbue.html

[U57] PHP：字符串插值
来源：http://hz.havefunace.top/gttfqwuoww.html

"值: {$a}"
来源：http://hz.zdqjudy.top/gtfuwrbuqv.html

[U58] PHP：数组三件套
来源：http://hz.quarkkingdee.top/gtgzjdmvcv.html

array_map($f, $a);  array_filter($a, $f);  array_reduce($a, $f, 0);
来源：http://hz.cdnleiting.top/gtoalbgbtg.html

[U59] PHP：自定义排序
来源：http://hz.hfpthk.cn/gtckzrcjpk.html

usort($arr, fn($a, $b) => $a["age"] <=> $b["age"]);
来源：http://hz.gogol.net.cn/gtdiuffbob.html

[U60] PHP：JSON 编解码
来源：http://hz.xziqi.cn/gtmeqnwbvl.html

json_encode($d, JSON_UNESCAPED_UNICODE);  json_decode($s, true);
来源：http://hz.svipenyu.cn/gtjdqdyngv.html

[U61] PHP：正则
来源：http://hz.ivvv.top/gtwziowdjw.html

preg_match('/(\d+)/', $s, $m);  preg_replace('/\d+/', '#', $s);
来源：http://hz.dianchejie.cn/gtgwvaxkle.html

[U62] PHP：日期对象
来源：http://hz.kuanghao11.cn/gtedphtiyf.html

(new DateTimeImmutable())->format("Y-m-d");
来源：http://hz.shanyushiyangtech.top/gtwwhrpgcq.html

[U63] PHP：文件读写
来源：http://hz.vqdsnc.cn/gtdkgfewrc.html

file_get_contents($f);  file_put_contents($f, $data);
来源：http://hz.yj20258.top/gtexfkrudi.html

[U64] PHP：目录遍历
来源：http://hz.yj20258.top/gtieedjcly.html

glob("dir/*.php");  scandir("dir");
来源：http://hz.yj20258888.top/gtmepqnpor.html

[U65] PHP：会话
来源：http://hz.shanyushiyangkeji.top/gtlporcfmr.html

session_start();  $_SESSION["uid"] = 1;
来源：http://hz.andypj.xyz/gtwoadnmbc.html

[U66] PHP：设置 Cookie
来源：http://hz.pycfn.com/gtcqwpjxlc.html

setcookie("token", $v, ["httponly" => true, "samesite" => "Lax"]);
来源：http://hz.jinghuilouyu.cn/gtbeswfnmg.html


<!-- 参考信息 -->