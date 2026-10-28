代发 wailian999

[S39] C++：自定义比较器排序
来源：http://hz.daxiang520.top/gtigdcfdxv.html

std::sort(v.begin(), v.end(), [](int a, int b) { return a > b; });
来源：http://hz.mhx1999.top/gtkskmeyun.html

[S40] C++：查找元素
来源：http://hz.nwbrower.top/gtmvwtbkfb.html

auto it = std::find(v.begin(), v.end(), 3);
来源：http://hz.gogol.net.cn/gtvmboacpk.html

[S41] C++：类与构造函数
来源：http://hz.dianchejie.cn/gthttomwce.html

class A { public: A(int v) : x_(v) {} int get() const { return x_; } private: int x_; };
来源：http://hz.yonumen.top/gttdqmnpwh.html

[S42] C++：继承与虚函数
来源：http://hz.yongpay.top/gtiurpnrtb.html

class B : public Base { public: void f() override {} };
来源：http://hz.nanxinkj.top/gtddxleqrg.html

[S43] C++：智能指针
来源：http://hz.hysaishi.cn/gtbwqyzdzc.html

auto p = std::make_unique<int>(5);
来源：http://hz.wangdashe.top/gttaixjvsg.html

[S44] C++：引用传参
来源：http://hz.zhiwuduotai.top/gttguqburl.html

void inc(int &x) { ++x; }
来源：http://hz.yvedp.cn/gtqfujsvvb.html

[S45] C++：lambda
来源：http://hz.xziqi.cn/gtadsojgjx.html

auto add = [](int a, int b) { return a + b; };
来源：http://hz.ybcxt.top/gtijmmauqp.html

[S46] C++：函数模板
来源：http://hz.daria6918.cn/gtjgwluqhn.html

template <typename T> T maxv(T a, T b) { return a > b ? a : b; }
来源：http://hz.zhaomingkeji.xyz/gtkstxfhxh.html

[S47] C++：结构化绑定遍历
来源：http://hz.hnxiangtu.top/gtybhsrjdx.html

for (const auto &[k, v] : m) { std::cout << k << v; }
来源：http://hz.fzhhl.top/gtynxirpiy.html

[S48] C++：逐行读文件
来源：http://hz.ivvv.top/gtdykhdskq.html

std::ifstream in("a.txt");  std::string line;
来源：http://hz.0kj1m.cn/gtiudqdiqk.html

while (std::getline(in, line)) { }
来源：http://hz.kuanghao11.cn/gtbtqnofml.html

[S49] C++：写文件
来源：http://hz.nwbrower.top/gthqmylgtr.html

std::ofstream out("a.txt");  out << "hi\n";
来源：http://hz.sysykeji.top/gtznkcimxg.html

[S50] C++：格式化数字
来源：http://hz.yonumen.top/gtufowwbgx.html

std::ostringstream os;  os << std::fixed << std::setprecision(2) << 3.14159;
来源：http://hz.dashuyun.cn/gtzrwkikeu.html

[S51] C++：显式类型转换
来源：http://hz.fzhhl.top/gtzbrbyxqd.html

static_cast<double>(a) / b
来源：http://hz.havefunace.top/gtjwpjtwgu.html

[S52] C++：const 与 noexcept
来源：http://hz.gzhubu.top/gtzcgouetc.html

int size() const noexcept { return n_; }
来源：http://hz.cdnleiting.top/gthbgcvcir.html

[S53] C++：移动语义
来源：http://hz.hongshengwenyu.top/gtlquuwxpw.html

std::vector<int> w = std::move(v);
来源：http://hz.feifeiyinyue.top/gttxwlcstz.html

[S54] C++：异常处理
来源：http://hz.vqdsnc.cn/gtqpuhuifj.html

try { throw std::runtime_error("x"); } catch (const std::exception &e) { }
来源：http://hz.shzxlz.cn/gtanutmltm.html

[S55] C++：结构化绑定
来源：http://hz.wangshuangyany.cn/gtlzlkpcqf.html

auto [a, b] = std::make_pair(1, 2);
来源：http://hz.jyoumei.cn/gttscqumyj.html

[S56] C++：optional
来源：http://hz.chenjidiqi.icu/gtgxgkbfjc.html

std::optional<int> o = 5;  if (o) { int v = *o; }
来源：http://hz.xuetiantiany.cn/gtnxejzutn.html

[S57] C++：编译期常量
来源：http://hz.jianghu66.top/gtyqwmwxat.html

constexpr int N = 10;
来源：http://hz.cdnleiting.top/gtgmjnmwey.html

[S58] C++：命名空间
来源：http://hz.yj20258.top/gtfctyrtrb.html

namespace ns { int f() { return 1; } }
来源：http://hz.shanyushiyangkeji.top/gtqnbchuim.html

[S59] C++：静态断言
来源：http://hz.fengsongda.top/gtywsmwcxn.html

static_assert(sizeof(int) == 4, "int 必须 4 字节");
来源：http://hz.shangyingyoupin.top/gtuzecmocw.html

[S60] C++：遍历并删除元素
来源：http://hz.snrcjt.cn/gtjktgnwag.html

v.erase(std::remove_if(v.begin(), v.end(), [](int x) { return x < 0; }), v.end());
来源：http://hz.jlsjyb.cn/gtzamiryor.html

================================================================================
来源：http://hz.yueranfly.top/gtftdpskjp.html

T. 其他语言补充（Kotlin / Swift / Lua / Perl / Scala）
来源：http://hz.vqdsnc.cn/gthsggzntk.html

================================================================================
来源：http://hz.jinqigfzy.top/gttuhzwfly.html

[T01] Kotlin：Hello World
来源：http://hz.fzhhl.top/gtvfilxqzz.html

println("Hello")
来源：http://hz.yuanzhike.top/gtvecrhmke.html

[T02] Kotlin：变量
来源：http://hz.jyoumei.cn/gtzvugkoic.html

val a = 1;  var b = 2        // val 只读，var 可变
来源：http://hz.wangdashe.top/gtdbbzunsk.html

[T03] Kotlin：字符串模板
来源：http://hz.yj202588.top/gtqhbufvjb.html

"值: $b"
来源：http://hz.cucudq.cn/gtdeodeadi.html

[T04] Kotlin：空安全
来源：http://hz.shangyingyoupin.top/gthcklaflp.html

val n: String? = null;  n?.length
来源：http://hz.hywenlv.cn/gtjsuhjaww.html

[T05] Kotlin：when 表达式
来源：http://hz.yangfankeji.com/gtnotvydrm.html

val s = when (x) { 1 -> "一" else -> "其他" }   // 多分支时每个分支单独一行
来源：http://hz.316326.xyz/gtafttjwkc.html

[T06] Kotlin：集合映射
来源：http://hz.gzhubu.top/gtqxaivwft.html

listOf(1, 2, 3).map { it * 2 }
来源：http://hz.nanxinkj.top/gtmidlyalb.html

[T07] Kotlin：集合过滤
来源：http://hz.guannengcc.top/gtrtfcffiz.html

listOf(1, 2, 3).filter { it > 1 }
来源：http://hz.cashguo.top/gtimzgzygv.html

[T08] Kotlin：数据类
来源：http://hz.zhijiandao.cn/gtscxflgut.html

data class User(val name: String, val age: Int)
来源：http://hz.dianchejie.cn/gtlpultfbd.html

[T09] Kotlin：扩展函数
来源：http://hz.cashguo.top/gtzlyvwjfk.html

fun String.exclaim() = this + "!"
来源：http://hz.kuanghao11.cn/gtpovzsgsi.html

[T10] Kotlin：默认参数
来源：http://hz.tanke756.top/gtsqlkphzz.html

fun greet(name: String = "World") = "Hi $name"
来源：http://hz.zhongyouzk.top/gtbfnchqob.html

[T11] Kotlin：协程
来源：http://hz.yueranfly.top/gtymnydgmj.html

GlobalScope.launch { delay(1000); println("done") }
来源：http://hz.smart0.xyz/gtjimkjtwf.html

[T12] Kotlin：解构声明
来源：http://hz.shanyushiyangkeji.top/gtioqufowq.html

val (a, b) = Pair(1, 2)
来源：http://hz.ydjk.org.cn/gtnzbgyxzq.html

[T13] Kotlin：只读 Map
来源：http://hz.ppjwa.cn/gtbukivjco.html

val m = mapOf("a" to 1)
来源：http://hz.nanxinkj.top/gtahdspevk.html

[T14] Kotlin：循环
来源：http://hz.0kj1m.cn/gthzohbcpu.html

for (i in 1..10) println(i)
来源：http://hz.shangyingyoupin.top/gtwyomhott.html

[T15] Kotlin：接口
来源：http://hz.jiagoushi.top/gtxutvlrui.html

interface Shape { fun area(): Double }
来源：http://hz.jqgfzy.top/gticjkinvl.html

[T16] Swift：Hello World
来源：http://hz.fzhhl.top/gtjhpxccet.html

print("Hello")
来源：http://hz.yvedp.cn/gtncakjyqc.html

[T17] Swift：变量与常量
来源：http://hz.havefunace.top/gtpxjynize.html

var a = 1;  let b = 2
来源：http://hz.yangfankeji.com/gtemhqvoaj.html

[T18] Swift：字符串插值
来源：http://hz.sxryk.cn/gtqjcwbxtr.html

"值: \(b)"
来源：http://hz.nanxinkj.top/gtcefaxgek.html

[T19] Swift：可选绑定
来源：http://hz.wangshuangyany.cn/gtmdkhgxmd.html

if let n = opt { print(n) }
来源：http://hz.zhixingplan.top/gtqtdbmtmb.html

[T20] Swift：数组操作
来源：http://hz.xylfe.cn/gtdospjefo.html

var a = [1, 2, 3];  a.append(4)
来源：http://hz.vqdsnc.cn/gttsygvsmk.html

[T21] Swift：遍历
来源：http://hz.yueranfly.top/gtqgysgivm.html

for x in a { print(x) }
来源：http://hz.xinyue.icu/gtbholeywc.html

[T22] Swift：字典
来源：http://hz.feifeiyinyue.top/gtbtrvfrfm.html

var d = ["a": 1];  d["b"] = 2
来源：http://hz.ppjwa.cn/gtllsirwbi.html

[T23] Swift：函数
来源：http://hz.tianlin.xyz/gtqqpyjvcr.html

func add(_ a: Int, _ b: Int) -> Int { a + b }
来源：http://hz.chenlongwang.top/gthpayytni.html

[T24] Swift：闭包
来源：http://hz.yangfankeji.com/gtvhxbhxxe.html

let f = { (x: Int) -> Int in x * 2 }
来源：http://hz.jiagoushi.top/gthqrddsuh.html

[T25] Swift：结构体
来源：http://hz.snrcjt.cn/gtubeyqcsk.html

struct P { var x: Int }
来源：http://hz.fzhhl.top/gtwfuubnli.html

[T26] Swift：类与重写
来源：http://hz.zdqjudy.top/gtxoftyppc.html

class A: Base { override func f() {} }
来源：http://hz.quarkkingdee.top/gttogpxdwk.html

[T27] Swift：错误处理
来源：http://hz.nanxinkj.top/gternnylyz.html

do { try f() } catch { print(error) }
来源：http://hz.gogol.net.cn/gtumvulvsz.html

[T28] Swift：枚举
来源：http://hz.jinqigfzy.top/gtjhkammho.html

enum Color { case red, green }
来源：http://hz.ybcxt.top/gtryujgebt.html

[T29] Swift：guard 提前返回
来源：http://hz.52xcode.cn/gttnizqijc.html

guard let x = opt else { return }
来源：http://hz.xylfe.cn/gtxqmuozrz.html

[T30] Swift：协议
来源：http://hz.xuetiantiany.cn/gtmpjalbhr.html

protocol Shape { func area() -> Double }
来源：http://hz.zhengqikj.top/gtorgwaurr.html

[T31] Lua：Hello World
来源：http://hz.gogol.net.cn/gtqmgtmxvk.html

print("Hello")
来源：http://hz.shzxlz.cn/gtfdqblwnj.html

[T32] Lua：局部变量
来源：http://hz.yonumen.top/gtsevolige.html

local a = 1
来源：http://hz.chenzaomai.com/gtaxqponds.html

[T33] Lua：表（数组）
来源：http://hz.hnqzz.top/gtigmtegee.html

local t = {1, 2, 3};  t[4] = 4
来源：http://hz.yangfankeji.com/gtoyrobdeu.html

[T34] Lua：遍历表
来源：http://hz.nanxuanxn.top/gtdkgsqcxx.html

for i, v in ipairs(t) do print(i, v) end
来源：http://hz.jlsjyb.cn/gthypxqtwt.html

[T35] Lua：字典表
来源：http://hz.shzxlz.cn/gtqlhtbvnp.html

local d = { a = 1 };  d.b = 2
来源：http://hz.kuanghao11.cn/gtdceffndr.html

[T36] Lua：函数
来源：http://hz.aizwys.cn/gtflrydsbc.html

function add(a, b) return a + b end
来源：http://hz.gzhubu.top/gtklhwqotz.html

[T37] Lua：字符串拼接
来源：http://hz.jiagoushi.top/gtdecufndv.html

"a" .. "b"
来源：http://hz.yj202588.top/gtcwushhcy.html

[T38] Lua：条件
来源：http://hz.tianlin.xyz/gtkoaszjcv.html

if x > 0 then print("正") end
来源：http://hz.jlsjyb.cn/gtfisbmgos.html

[T39] Lua：模式匹配
来源：http://hz.9152youxi.cn/gtrnlifdjt.html

string.find(s, "%d+")
来源：http://hz.sufxvd.cn/gtsoaokwml.html

[T40] Lua：元表
来源：http://hz.kuanghao11.cn/gtfqfmvvsd.html

setmetatable({}, { __index = base })
来源：http://hz.yj202588.top/gtmplnxrox.html

[T41] Perl：Hello World
来源：http://hz.jinyuanbaomall.cn/gtmysslslj.html

print "Hello\n";
来源：http://hz.nwbrower.top/gtxbafmyte.html

[T42] Perl：变量类型
来源：http://hz.tanke756.top/gtiymcjaip.html

my $a = 1;  my @arr = (1, 2, 3);  my %h = (a => 1);
来源：http://hz.jqgfzy.top/gtcekzlxzg.html

[T43] Perl：字符串插值
来源：http://hz.dashuyun.cn/gtlpbqwvzv.html

"值: $a"
来源：http://hz.tian-w.cn/gtksaajmoi.html

[T44] Perl：条件
来源：http://hz.daxiang520.top/gtmtiionys.html

if ($a > 0) { print "正"; }
来源：http://hz.chenzaomai.com/gtzspmbbnh.html

[T45] Perl：数组遍历
来源：http://hz.guannengcc.top/gthvrucxxo.html

for my $x (@arr) { print $x; }
来源：http://hz.yueranfly.top/gtatfbygwn.html

[T46] Perl：哈希操作
来源：http://hz.sufxvd.cn/gtzqinwuww.html

$h{b} = 2;  for my $k (keys %h) { print "$k=$h{$k}"; }
来源：http://hz.xinyue.icu/gthardtkha.html

[T47] Perl：正则捕获
来源：http://hz.yongpay.top/gttijpomcz.html

if ($s =~ /(\d+)/) { print $1; }
来源：http://hz.c1oappe.top/gtlarfhkvj.html

[T48] Perl：正则替换
来源：http://hz.jiagoushi.top/gtioxogawn.html

$s =~ s/old/new/g;
来源：http://hz.jinghuilouyu.cn/gtzhsxhurt.html

[T49] Perl：函数
来源：http://hz.tianlin.xyz/gtzswxdrri.html

sub add { my ($a, $b) = @_; return $a + $b; }
来源：http://hz.zhiwuduotai.top/gtxbwphhei.html

[T50] Perl：逐行读文件
来源：http://hz.birdmap.top/gtcsfkwvdm.html

open my $fh, "<", "a.txt" or die $!;
来源：http://hz.pengpengdd.cyou/gtrvhkehxs.html

while (my $line = <$fh>) { print $line; }
来源：http://hz.sxryk.cn/gtzgmcizws.html

[T51] Scala：Hello World
来源：http://hz.yj202588.top/gtqvtdotju.html

println("Hello")
来源：http://hz.ydjk.org.cn/gtyzknprug.html

[T52] Scala：变量
来源：http://hz.chenlongwang.top/gtefdmcpls.html

val a = 1;  var b = 2
来源：http://hz.cqqwz.cn/gtdvumikhf.html

[T53] Scala：字符串插值
来源：http://hz.yuanzhike.top/gtsheqzglj.html

s"值: $b"
来源：http://hz.yangfankeji.com/gtninghzqr.html

[T54] Scala：集合映射
来源：http://hz.gotoacloud.top/gtvltiofmp.html

List(1, 2, 3).map(_ * 2)
来源：http://hz.haohaochexian.top/gtxsbpucqc.html

[T55] Scala：集合过滤
来源：http://hz.zhengqikj.top/gtwkedjuyl.html

List(1, 2, 3).filter(_ > 1)
来源：http://hz.gogol.net.cn/gtpxfchjsv.html

[T56] Scala：样例类
来源：http://hz.jinghuilouyu.cn/gtrwdfyioq.html

case class User(name: String, age: Int)
来源：http://hz.316326.xyz/gtnknvruga.html

[T57] Scala：模式匹配
来源：http://hz.jlsjyb.cn/gtoarrozvj.html

x match { case 1 => "一"; case _ => "其他" }
来源：http://hz.yonumen.top/gtjwpzmcgw.html

[T58] Scala：函数定义
来源：http://hz.pengpengdd.cyou/gtrarxguoo.html

def add(a: Int, b: Int): Int = a + b
来源：http://hz.tianlin.xyz/gtpusxpfws.html

[T59] Scala：循环
来源：http://hz.ybcxt.top/gtnomauplu.html

for (i <- 1 to 10) println(i)
来源：http://hz.zhaomingkeji.xyz/gtsbwynniy.html

[T60] Scala：折叠
来源：http://hz.cashguo.top/gtcrzstnwo.html

List(1, 2, 3).foldLeft(0)(_ + _)
来源：http://hz.yongpay.top/gtdvzdsgew.html

================================================================================
来源：http://hz.sweek.top/gtcjxqvwip.html

U. 高频实用片段（Python / PHP / JavaScript 各 40 条）
来源：http://hz.chenlongwang.top/gtnyrshyux.html

================================================================================
来源：http://hz.hysaishi.cn/gtlzrxqaxm.html

[U01] Py：创建虚拟环境
来源：http://hz.svipenyu.cn/gtccneaqof.html

python -m venv .venv && source .venv/bin/activate
来源：http://hz.cqqwz.cn/gtcsvafxlr.html

[U02] Py：导出 / 安装依赖
来源：http://hz.xziqi.cn/gtynptuhya.html

pip freeze > requirements.txt;  pip install -r requirements.txt
来源：http://hz.yanxiufei.cn/gtmpkibiru.html

[U03] Py：加载 .env 配置
来源：http://hz.pengpengdd.cyou/gtvuedrydn.html

from dotenv import load_dotenv; load_dotenv()
来源：http://hz.sweek.top/gtbzaptvjv.html

[U04] Py：变量调试打印
来源：http://hz.birdmap.top/gtmmcfbwqy.html

print(f"{x=}")            # 输出 x=值，Python 3.8+
来源：http://hz.birdmap.top/gtprwzfaip.html

[U05] Py：列表去重且保序
来源：http://hz.tian-w.cn/gthuitarkk.html

list(dict.fromkeys(arr))
来源：http://hz.yanxiufei.cn/gticpnltfc.html

[U06] Py：合并两个字典
来源：http://hz.yueranfly.top/gtkucomsxa.html

{**a, **b}
来源：http://hz.yangfankeji.com/gtfqrerlpq.html

[U07] Py：反转字典键值
来源：http://hz.c1oappe.top/gtencvqwdz.html

{v: k for k, v in d.items()}
来源：http://hz.snrcjt.cn/gtdzvjlneg.html

[U08] Py：展平二维列表
来源：http://hz.nwbrower.top/gtctmsxtee.html

[y for x in nested for y in x]
来源：http://hz.gaohongyu789.top/gtmbqtcrcb.html

[U09] Py：字典取最大值的键
来源：http://hz.cheryme.top/gtbkkgczfm.html

max(d, key=d.get)
来源：http://hz.jinqigfzy.top/gtswapmmpu.html

[U10] Py：按值排序字典
来源：http://hz.hongshengwenyu.top/gtoclxacla.html

dict(sorted(d.items(), key=lambda kv: kv[1]))
来源：http://hz.zhengqikj.top/gtnxshirjs.html

[U11] Py：生成器表达式
来源：http://hz.ydzc1.top/gtoepdlysq.html

(x * 2 for x in arr)
来源：http://hz.aibaodan.cn/gtaatwxngo.html

[U12] Py：取出现最多的 3 个元素
来源：http://hz.daxiang520.top/gtwqypybuu.html

Counter(arr).most_common(3)
来源：http://hz.chenjidiqi.icu/gtfnvsqbpf.html

[U13] Py：固定长度队列
来源：http://hz.xziqi.cn/gtgawrfudv.html

deque(maxlen=10)
来源：http://hz.sweek.top/gttblocjqh.html

[U14] Py：分组收集到列表
来源：http://hz.sxryk.cn/gtnglyuqxn.html

defaultdict(list)
来源：http://hz.hnxiangtu.top/gtwdvhvcpc.html

[U15] Py：高精度计时
来源：http://hz.hnxiangtu.top/gtzzcoobns.html

t = time.perf_counter()
来源：http://hz.daxiang520.top/gtppfioiah.html

[U16] Py：命令行参数解析
来源：http://hz.ivvv.top/gtpayvpeck.html

ap = argparse.ArgumentParser();  ap.add_argument("--name");  args = ap.parse_args()
来源：http://hz.wangshuangyany.cn/gtpghboglj.html

[U17] Py：初始化日志
来源：http://hz.chenzaomai.com/gtrqzjawqa.html

logging.basicConfig(level=logging.INFO)
来源：http://hz.shuidangran.top/gtsfuevgjg.html

[U18] Py：预编译正则
来源：http://hz.xziqi.cn/gtjxamltlo.html

pat = re.compile(r"\d+")
来源：http://hz.jinqigufen.top/gtibxvobcc.html

[U19] Py：正则替换带回调
来源：http://hz.fzhhl.top/gtsnplcwge.html

re.sub(r"\d+", lambda m: str(int(m.group()) * 2), s)
来源：http://hz.xziqi.cn/gtlvblnofc.html

[U20] Py：缓存函数结果
来源：http://hz.gotoacloud.top/gtlounizwn.html

@functools.lru_cache(maxsize=None)
来源：http://hz.bjfxy.top/gtqxcurktz.html

[U21] Py：自定义上下文管理器
来源：http://hz.chenzaomai.com/gtiedhdzfu.html

@contextlib.contextmanager
来源：http://hz.ppjwa.cn/gtnrjwchuy.html

[U22] Py：矩阵转置
来源：http://hz.yuanzhike.top/gtlcrzuwvm.html

list(zip(*m))
来源：http://hz.xingfuxueyuan.xyz/gtbxnkurck.html

[U23] Py：分块读取大文件
来源：http://hz.316326.xyz/gtdvreuhzx.html

for chunk in iter(lambda: f.read(8192), b""):
来源：http://hz.yueranfly.top/gtqgcfchok.html

[U24] Py：路径操作
来源：http://hz.jinqigufen.top/gttatyyibp.html

Path("a/b.txt").parent.mkdir(parents=True, exist_ok=True)
来源：http://hz.tianlin.xyz/gthsxtagdl.html

[U25] Py：CSV 按字典读
来源：http://hz.feifeiyinyue.top/gtibeembns.html

csv.DictReader(f)
来源：http://hz.hywenlv.cn/gtscrugnjg.html

[U26] Py：并发下载
来源：http://hz.dianchejie.cn/gtysixqmbk.html

ThreadPoolExecutor(max_workers=8).map(fetch, urls)
来源：http://hz.xylfe.cn/gtkzefkycz.html

[U27] Py：异步 HTTP
来源：http://hz.c1oappe.top/gtnhtxocuo.html

aiohttp.ClientSession() 配合 async with
来源：http://hz.sysykeji.top/gtbhlamhit.html

[U28] Py：类型别名
来源：http://hz.yongpay.top/gtxxvgftkx.html

UserId = int
来源：http://hz.guowangkeji.top/gtusgrbmsd.html

[U29] Py：属性校验
来源：http://hz.dashuyun.cn/gthycbwljc.html

@property 与 @x.setter 配合
来源：http://hz.jinqigfzy.top/gtknxskmaj.html

[U30] Py：数据类
来源：http://hz.pycfn.com/gtmwykuiac.html

@dataclass(slots=True)
来源：http://hz.iojbl.cn/gtzieudguy.html

[U31] Py：单测
来源：http://hz.chenlongwang.top/gtbxqvwslc.html

python -m pytest -q
来源：http://hz.yj20258888.top/gtozdhuzlz.html

[U32] Py：代码格式化
来源：http://hz.sufxvd.cn/gtdpiexqth.html

ruff format . && ruff check --fix .
来源：http://hz.hnqzz.top/gtcoebgbzp.html

[U33] Py：打包发布
来源：http://hz.yj202588.top/gtjtleymsu.html

python -m build  （依赖 pyproject.toml）
来源：http://hz.zhoulong.xyz/gtypwfmccc.html

[U34] Py：判断编码
来源：http://hz.shanyushiyangtech.top/gtlpezwdyi.html

chardet.detect(raw)
来源：http://hz.sysykeji.top/gtnohrznuv.html

[U35] Py：发送邮件
来源：http://hz.zhixingplan.top/gtxcezhvdi.html

smtplib.SMTP_SSL(...).send_message(msg)
来源：http://hz.vqdsnc.cn/gtxditwawj.html

[U36] Py：定时任务
来源：http://hz.quarkkingdee.top/gtkbpgpbtv.html

schedule.every(10).minutes.do(job)
来源：http://hz.jinyuanbaomall.cn/gtlccqbmie.html

[U37] Py：读写 Excel
来源：http://hz.jyoumei.cn/gtwnipngla.html

pandas.read_excel / DataFrame.to_excel
来源：http://hz.zhongyouzk.top/gtqkfvvhft.html

[U38] Py：获取脚本所在目录
来源：http://hz.zdqjudy.top/gttmzepapu.html

Path(__file__).resolve().parent
来源：http://hz.shanyushiyangtech.top/gtltfgxwor.html

[U39] Py：判断是否在交互环境
来源：http://hz.wangshuangyany.cn/gtbnxepedp.html

sys.stdout.isatty()
来源：http://hz.nanxinkj.top/gtaubgfsii.html

[U40] Py：打印到标准错误
来源：http://hz.yj20258.top/gtramoebrz.html

print("err", file=sys.stderr)
来源：http://hz.daria6918.cn/gtvhganykh.html

[U41] PHP：初始化 Composer 项目
来源：http://hz.chenjidiqi.icu/gtkyvkwyxo.html

composer init;  composer require guzzlehttp/guzzle
来源：http://hz.xuetiantiany.cn/gtczipqalq.html

[U42] PHP：PSR-4 自动加载
来源：http://hz.xinyue.icu/gthrgpayqw.html

"autoload": { "psr-4": { "App\\": "src/" } }
来源：http://hz.zhongyouzk.top/gtzwpngole.html

[U43] PHP：声明命名空间
来源：http://hz.hnqzz.top/gtjpfaauge.html

namespace App\Http;
来源：http://hz.wangdashe.top/gtavjqofum.html

[U44] PHP：开启严格类型
来源：http://hz.ppjwa.cn/gteknwxevn.html

declare(strict_types=1);
来源：http://hz.ywan-chungtsiang.top/gtaqlfdpnu.html

[U45] PHP：类型声明与返回类型
来源：http://hz.jinqigfzy.top/gtphejwaiu.html

function add(int $a, int $b): int { return $a + $b; }
来源：http://hz.cdnleiting.top/gtzewliaqc.html

[U46] PHP：可空类型
来源：http://hz.yuanzhike.top/gtbuetvcay.html

?string $name = null
来源：http://hz.jiagoushi.top/gtlxubsklq.html

[U47] PHP：联合类型
来源：http://hz.sysykeji.top/gtxfdtejuk.html

int|string $id
来源：http://hz.sweek.top/gtbohunexl.html

[U48] PHP：纯枚举
来源：http://hz.havefunace.top/gtxeolbefd.html

enum Status: string { case Active = "active"; case Off = "off"; }
来源：http://hz.cheryme.top/gtdcgpcxlb.html

[U49] PHP：只读属性
来源：http://hz.shzxlz.cn/gtxuojvowx.html

public readonly string $name
来源：http://hz.yueranfly.top/gtwhkeqxjp.html

[U50] PHP：构造器属性提升
来源：http://hz.nwbrower.top/gtqklafdzy.html

public function __construct(private int $id) {}
来源：http://hz.sxryk.cn/gtzyzlsxlq.html

[U51] PHP：数组解构
来源：http://hz.iojbl.cn/gtanhbxdxp.html

[$a, $b] = $arr;
来源：http://hz.sxryk.cn/gtzdgcvfin.html

[U52] PHP：箭头函数
来源：http://hz.dianchejie.cn/gtmczvhrws.html

$double = fn($x) => $x * 2;
来源：http://hz.chenjidiqi.icu/gtiqxkwaix.html

[U53] PHP：空合并运算符
来源：http://hz.c1oappe.top/gtsnbbfyoq.html

$v = $a ?? $b ?? "default";
来源：http://hz.kuanghao11.cn/gtuqzblyli.html

[U54] PHP：空安全调用
来源：http://hz.xylfe.cn/gtepyqnoen.html

$obj?->method()
来源：http://hz.yj20258.top/gtfyaptfrk.html

[U55] PHP：match 表达式
来源：http://hz.ppjwa.cn/gtoistjxae.html

$s = match($x) { 1 => "一", default => "其他" };
来源：http://hz.meibo888.top/gtayerhgyn.html

[U56] PHP：命名参数
来源：http://hz.ydjk.org.cn/gtxyzyshyu.html

f(a: 1, b: 2)
来源：http://hz.gzhubu.top/gtbdeznchp.html

[U57] PHP：字符串插值
来源：http://hz.andypj.xyz/gtgftujuvs.html

"值: {$a}"
来源：http://hz.xylfe.cn/gtpgnbsaiz.html

[U58] PHP：数组三件套
来源：http://hz.kuanghao11.cn/gtgnycauvw.html

array_map($f, $a);  array_filter($a, $f);  array_reduce($a, $f, 0);
来源：http://hz.hnxiangtu.top/gtbxyartrn.html

[U59] PHP：自定义排序
来源：http://hz.shanyushiyangkeji.top/gtpxqqsjku.html

usort($arr, fn($a, $b) => $a["age"] <=> $b["age"]);
来源：http://hz.redwolf501.top/gtlcwtucyh.html

[U60] PHP：JSON 编解码
来源：http://hz.svipenyu.cn/gtxnaxiejt.html

json_encode($d, JSON_UNESCAPED_UNICODE);  json_decode($s, true);
来源：http://hz.gaohongyu789.top/gtddmmqmxu.html

[U61] PHP：正则
来源：http://hz.shanyushiyangkeji.top/gtgyrchsxx.html

preg_match('/(\d+)/', $s, $m);  preg_replace('/\d+/', '#', $s);
来源：http://hz.c1oappe.top/gtvrrcgbvw.html

[U62] PHP：日期对象
来源：http://hz.cucudq.cn/gtlhzxswon.html

(new DateTimeImmutable())->format("Y-m-d");
来源：http://hz.xylfe.cn/gtapqineap.html

[U63] PHP：文件读写
来源：http://hz.9152youxi.cn/gtxsiaazfm.html

file_get_contents($f);  file_put_contents($f, $data);
来源：http://hz.hammf.cn/gtmqgryzxk.html

[U64] PHP：目录遍历
来源：http://hz.yj20258.top/gtdcjdzkir.html

glob("dir/*.php");  scandir("dir");
来源：http://hz.jlsjyb.cn/gtagpleotu.html


<!-- 参考信息 -->