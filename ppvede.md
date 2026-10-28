代发 wailian999

[S37] C++：set
来源：http://hz.hongshengwenyu.top/gtqtehbxla.html

std::set<int> s{1, 2, 3};  s.insert(4);
来源：http://hz.zhoulong.xyz/gtisaihxka.html

[S38] C++：排序
来源：http://hz.hywenlv.cn/gtfvtvazvy.html

std::sort(v.begin(), v.end());
来源：http://hz.jyoumei.cn/gtuqsfbryd.html

[S39] C++：自定义比较器排序
来源：http://hz.chenlongwang.top/gtiprmzrqh.html

std::sort(v.begin(), v.end(), [](int a, int b) { return a > b; });
来源：http://hz.gotoacloud.top/gtqmoutlzl.html

[S40] C++：查找元素
来源：http://hz.yuanzhike.top/gtsjcsoydd.html

auto it = std::find(v.begin(), v.end(), 3);
来源：http://hz.dianchejie.cn/gtxyctfsoc.html

[S41] C++：类与构造函数
来源：http://hz.hnqzz.top/gtnpgfcmch.html

class A { public: A(int v) : x_(v) {} int get() const { return x_; } private: int x_; };
来源：http://hz.zhiwuduotai.top/gtprnwmikr.html

[S42] C++：继承与虚函数
来源：http://hz.fzhhl.top/gtjzvtnyej.html

class B : public Base { public: void f() override {} };
来源：http://hz.tanke756.top/gtgioqyqiu.html

[S43] C++：智能指针
来源：http://hz.tianlin.xyz/gtngsjhhio.html

auto p = std::make_unique<int>(5);
来源：http://hz.0kj1m.cn/gtxehckayb.html

[S44] C++：引用传参
来源：http://hz.shanyushiyangkeji.top/gtyruotmiw.html

void inc(int &x) { ++x; }
来源：http://hz.fzhhl.top/gtxgpacgmd.html

[S45] C++：lambda
来源：http://hz.shzxlz.cn/gtlicomnet.html

auto add = [](int a, int b) { return a + b; };
来源：http://hz.wangdashe.top/gtuqidmewj.html

[S46] C++：函数模板
来源：http://hz.hfpthk.cn/gtwbmvlrol.html

template <typename T> T maxv(T a, T b) { return a > b ? a : b; }
来源：http://hz.aibaodan.cn/gtjiwpatjp.html

[S47] C++：结构化绑定遍历
来源：http://hz.chenzaomai.com/gtvvamyevg.html

for (const auto &[k, v] : m) { std::cout << k << v; }
来源：http://hz.bjfxy.top/gtgbnujaor.html

[S48] C++：逐行读文件
来源：http://hz.chenlongwang.top/gtfbokcvre.html

std::ifstream in("a.txt");  std::string line;
来源：http://hz.meibo888.top/gtjqfsiimn.html

while (std::getline(in, line)) { }
来源：http://hz.sxryk.cn/gtaarjzfwn.html

[S49] C++：写文件
来源：http://hz.jinyuanbaomall.cn/gtboxupasu.html

std::ofstream out("a.txt");  out << "hi\n";
来源：http://hz.cucudq.cn/gttlyxglcf.html

[S50] C++：格式化数字
来源：http://hz.shuidangran.top/gttejtdbco.html

std::ostringstream os;  os << std::fixed << std::setprecision(2) << 3.14159;
来源：http://hz.jinghuilouyu.cn/gtqwurqznm.html

[S51] C++：显式类型转换
来源：http://hz.dashuyun.cn/gtwqelxdec.html

static_cast<double>(a) / b
来源：http://hz.yonumen.top/gtnnzevwxd.html

[S52] C++：const 与 noexcept
来源：http://hz.nanxuanxn.top/gtrgoobfdq.html

int size() const noexcept { return n_; }
来源：http://hz.hywenlv.cn/gtluzehwyn.html

[S53] C++：移动语义
来源：http://hz.gaohongyu789.top/gtxnuyckap.html

std::vector<int> w = std::move(v);
来源：http://hz.zhiwuduotai.top/gtfhykwvht.html

[S54] C++：异常处理
来源：http://hz.mhx1999.top/gtvmyxfyaq.html

try { throw std::runtime_error("x"); } catch (const std::exception &e) { }
来源：http://hz.jqgfzy.top/gtunboxjix.html

[S55] C++：结构化绑定
来源：http://hz.quarkkingdee.top/gtipmnxxqg.html

auto [a, b] = std::make_pair(1, 2);
来源：http://hz.xuetiantiany.cn/gtocwgqekn.html

[S56] C++：optional
来源：http://hz.guowangkeji.top/gtbkhfjhkv.html

std::optional<int> o = 5;  if (o) { int v = *o; }
来源：http://hz.nanxuanxn.top/gtzernmxex.html

[S57] C++：编译期常量
来源：http://hz.jianghu66.top/gtxsmeknzz.html

constexpr int N = 10;
来源：http://hz.aizwys.cn/gtkqccglve.html

[S58] C++：命名空间
来源：http://hz.jinyuanbaomall.cn/gtvqwdbkdt.html

namespace ns { int f() { return 1; } }
来源：http://hz.jinqigufen.top/gterxcenic.html

[S59] C++：静态断言
来源：http://hz.daxiang520.top/gtffdoldbb.html

static_assert(sizeof(int) == 4, "int 必须 4 字节");
来源：http://hz.316326.xyz/gtnuumfgao.html

[S60] C++：遍历并删除元素
来源：http://hz.zhongyouzk.top/gtqfhqxsfq.html

v.erase(std::remove_if(v.begin(), v.end(), [](int x) { return x < 0; }), v.end());
来源：http://hz.zhengqikj.top/gtrxfqiily.html

================================================================================
来源：http://hz.zhaomingkeji.xyz/gtkwxvgocz.html

T. 其他语言补充（Kotlin / Swift / Lua / Perl / Scala）
来源：http://hz.pengpengdd.cyou/gtbfstoodj.html

================================================================================
来源：http://hz.shanyushiyangkeji.top/gtjktozime.html

[T01] Kotlin：Hello World
来源：http://hz.aizwys.cn/gtejveesrc.html

println("Hello")
来源：http://hz.xziqi.cn/gtpnpnpehd.html

[T02] Kotlin：变量
来源：http://hz.hysaishi.cn/gtwwtilxqr.html

val a = 1;  var b = 2        // val 只读，var 可变
来源：http://hz.yj20258.top/gtvjngcpso.html

[T03] Kotlin：字符串模板
来源：http://hz.mhx1999.top/gtwddsebei.html

"值: $b"
来源：http://hz.haohaochexian.top/gtyrxadvlh.html

[T04] Kotlin：空安全
来源：http://hz.zhengqikj.top/gtsumofojl.html

val n: String? = null;  n?.length
来源：http://hz.dianchejie.cn/gthhmqqzkg.html

[T05] Kotlin：when 表达式
来源：http://hz.nwbrower.top/gtuckzzywv.html

val s = when (x) { 1 -> "一" else -> "其他" }   // 多分支时每个分支单独一行
来源：http://hz.yongpay.top/gtjciybjgk.html

[T06] Kotlin：集合映射
来源：http://hz.cucudq.cn/gtifbcrqha.html

listOf(1, 2, 3).map { it * 2 }
来源：http://hz.zhixingplan.top/gtqvvwkniq.html

[T07] Kotlin：集合过滤
来源：http://hz.shanyushiyangkeji.top/gtjpqbwqnf.html

listOf(1, 2, 3).filter { it > 1 }
来源：http://hz.feifeiyinyue.top/gthsgjtxoy.html

[T08] Kotlin：数据类
来源：http://hz.jqgfzy.top/gtjbwrslfu.html

data class User(val name: String, val age: Int)
来源：http://hz.yueranfly.top/gtdrwfjcga.html

[T09] Kotlin：扩展函数
来源：http://hz.yanxiufei.cn/gtazljlqpv.html

fun String.exclaim() = this + "!"
来源：http://hz.0kj1m.cn/gtabauuuek.html

[T10] Kotlin：默认参数
来源：http://hz.yanxiufei.cn/gteehpaoii.html

fun greet(name: String = "World") = "Hi $name"
来源：http://hz.hongshengwenyu.top/gtgthtgynz.html

[T11] Kotlin：协程
来源：http://hz.bjfxy.top/gtcjhfqkay.html

GlobalScope.launch { delay(1000); println("done") }
来源：http://hz.cqqwz.cn/gtahstqnrf.html

[T12] Kotlin：解构声明
来源：http://hz.birdmap.top/gtmfrdugvo.html

val (a, b) = Pair(1, 2)
来源：http://hz.hammf.cn/gtgmcbywyo.html

[T13] Kotlin：只读 Map
来源：http://hz.xingfuxueyuan.xyz/gtelxtvfpm.html

val m = mapOf("a" to 1)
来源：http://hz.wangdashe.top/gtfghlamqb.html

[T14] Kotlin：循环
来源：http://hz.jiagoushi.top/gtiugrvuay.html

for (i in 1..10) println(i)
来源：http://hz.xinyue.icu/gtavqgousx.html

[T15] Kotlin：接口
来源：http://hz.chenlongwang.top/gtjwxbszrm.html

interface Shape { fun area(): Double }
来源：http://hz.guowangkeji.top/gtmtkuzjqw.html

[T16] Swift：Hello World
来源：http://hz.gotoacloud.top/gtmkchjjol.html

print("Hello")
来源：http://hz.tianlin.xyz/gtgesajugk.html

[T17] Swift：变量与常量
来源：http://hz.zhengqikj.top/gtomgzulix.html

var a = 1;  let b = 2
来源：http://hz.tian-w.cn/gtkcwtbkob.html

[T18] Swift：字符串插值
来源：http://hz.smart0.xyz/gtdcgxkwts.html

"值: \(b)"
来源：http://hz.xingfuxueyuan.xyz/gtbgionptc.html

[T19] Swift：可选绑定
来源：http://hz.sweek.top/gtklcdvegb.html

if let n = opt { print(n) }
来源：http://hz.zhongyouzk.top/gtqmlruses.html

[T20] Swift：数组操作
来源：http://hz.jinqigfzy.top/gtjaydcene.html

var a = [1, 2, 3];  a.append(4)
来源：http://hz.shzxlz.cn/gtgdodbwbq.html

[T21] Swift：遍历
来源：http://hz.0kj1m.cn/gttyenigtj.html

for x in a { print(x) }
来源：http://hz.316326.xyz/gtmqhpdomh.html

[T22] Swift：字典
来源：http://hz.wangshuangyany.cn/gtfjpvnirn.html

var d = ["a": 1];  d["b"] = 2
来源：http://hz.cashguo.top/gtlzjztght.html

[T23] Swift：函数
来源：http://hz.yonumen.top/gtdkcqctgf.html

func add(_ a: Int, _ b: Int) -> Int { a + b }
来源：http://hz.jinghuilouyu.cn/gtvlsqkobc.html

[T24] Swift：闭包
来源：http://hz.ivvv.top/gtykdjypei.html

let f = { (x: Int) -> Int in x * 2 }
来源：http://hz.zhijiandao.cn/gtmzhxodks.html

[T25] Swift：结构体
来源：http://hz.ydjk.org.cn/gtbtujpycd.html

struct P { var x: Int }
来源：http://hz.hfpthk.cn/gtwgzkwugk.html

[T26] Swift：类与重写
来源：http://hz.xziqi.cn/gtceizucqo.html

class A: Base { override func f() {} }
来源：http://hz.gaohongyu789.top/gtlezafloo.html

[T27] Swift：错误处理
来源：http://hz.yvedp.cn/gtvqjbdqll.html

do { try f() } catch { print(error) }
来源：http://hz.aizwys.cn/gtmoseektq.html

[T28] Swift：枚举
来源：http://hz.gogol.net.cn/gtdotmfraq.html

enum Color { case red, green }
来源：http://hz.tanke756.top/gthihoqguf.html

[T29] Swift：guard 提前返回
来源：http://hz.tanke756.top/gtanrhrykm.html

guard let x = opt else { return }
来源：http://hz.ivvv.top/gtiwrtxdie.html

[T30] Swift：协议
来源：http://hz.tanke756.top/gtpndwhndj.html

protocol Shape { func area() -> Double }
来源：http://hz.shangyingyoupin.top/gthrorcanf.html

[T31] Lua：Hello World
来源：http://hz.yanxiufei.cn/gtxkbsphjx.html

print("Hello")
来源：http://hz.pengpengdd.cyou/gtsmqbmcyf.html

[T32] Lua：局部变量
来源：http://hz.yj202588.top/gtqbbeahgq.html

local a = 1
来源：http://hz.sxryk.cn/gtloamrokr.html

[T33] Lua：表（数组）
来源：http://hz.chenjidiqi.icu/gtajocqvho.html

local t = {1, 2, 3};  t[4] = 4
来源：http://hz.gzhubu.top/gtrqfslwrw.html

[T34] Lua：遍历表
来源：http://hz.pengpengdd.cyou/gtwxxdaqlo.html

for i, v in ipairs(t) do print(i, v) end
来源：http://hz.52xcode.cn/gtcvvntyeb.html

[T35] Lua：字典表
来源：http://hz.kuanghao11.cn/gtidcvqjbp.html

local d = { a = 1 };  d.b = 2
来源：http://hz.feifeiyinyue.top/gtjmxovedw.html

[T36] Lua：函数
来源：http://hz.smart0.xyz/gtbfgxrziu.html

function add(a, b) return a + b end
来源：http://hz.jinqigfzy.top/gttzvtwpkk.html

[T37] Lua：字符串拼接
来源：http://hz.guowangkeji.top/gtvcipzksz.html

"a" .. "b"
来源：http://hz.xuanzx.com/gtzfzshgru.html

[T38] Lua：条件
来源：http://hz.cqqwz.cn/gtxnrgyqqe.html

if x > 0 then print("正") end
来源：http://hz.zhiwuduotai.top/gtwzklgwcp.html

[T39] Lua：模式匹配
来源：http://hz.bjfxy.top/gtfjljejij.html

string.find(s, "%d+")
来源：http://hz.jqgufenzy.top/gtlxdzbeas.html

[T40] Lua：元表
来源：http://hz.zhixingplan.top/gtxaupksuf.html

setmetatable({}, { __index = base })
来源：http://hz.mhx1999.top/gtkjseisab.html

[T41] Perl：Hello World
来源：http://hz.cqqwz.cn/gtqvwgzapn.html

print "Hello\n";
来源：http://hz.gzhubu.top/gtednrqtzq.html

[T42] Perl：变量类型
来源：http://hz.gzhubu.top/gtuijxdddt.html

my $a = 1;  my @arr = (1, 2, 3);  my %h = (a => 1);
来源：http://hz.fzhhl.top/gtumiwklig.html

[T43] Perl：字符串插值
来源：http://hz.yj20258888.top/gtwemfljmw.html

"值: $a"
来源：http://hz.yangfankeji.com/gtjgnqyxej.html

[T44] Perl：条件
来源：http://hz.vqdsnc.cn/gtsoekmfrj.html

if ($a > 0) { print "正"; }
来源：http://hz.yonumen.top/gtsaxnmkpc.html

[T45] Perl：数组遍历
来源：http://hz.tian-w.cn/gtpwkavvfv.html

for my $x (@arr) { print $x; }
来源：http://hz.zhengqikj.top/gtqzwtwusx.html

[T46] Perl：哈希操作
来源：http://hz.ppjwa.cn/gtlbwlsfkv.html

$h{b} = 2;  for my $k (keys %h) { print "$k=$h{$k}"; }
来源：http://hz.svipenyu.cn/gtrtkdskwh.html

[T47] Perl：正则捕获
来源：http://hz.0kj1m.cn/gtkhytpxzr.html

if ($s =~ /(\d+)/) { print $1; }
来源：http://hz.snrcjt.cn/gthkjcvoef.html

[T48] Perl：正则替换
来源：http://hz.quarkkingdee.top/gtdcdpfbys.html

$s =~ s/old/new/g;
来源：http://hz.yanxiufei.cn/gtpawksurs.html

[T49] Perl：函数
来源：http://hz.xuetiantiany.cn/gtrchoejay.html

sub add { my ($a, $b) = @_; return $a + $b; }
来源：http://hz.mhx1999.top/gtgnsoefxv.html

[T50] Perl：逐行读文件
来源：http://hz.guannengcc.top/gtlhyqfnuf.html

open my $fh, "<", "a.txt" or die $!;
来源：http://hz.dianchejie.cn/gtpcxdmosb.html

while (my $line = <$fh>) { print $line; }
来源：http://hz.hywenlv.cn/gtnahetzic.html

[T51] Scala：Hello World
来源：http://hz.snrcjt.cn/gtghulnrmf.html

println("Hello")
来源：http://hz.ppjwa.cn/gtziavqswb.html

[T52] Scala：变量
来源：http://hz.yj202588.top/gtmqarmgfp.html

val a = 1;  var b = 2
来源：http://hz.nanxuanxn.top/gtdtqdgehs.html

[T53] Scala：字符串插值
来源：http://hz.shanyushiyangkeji.top/gtogcuwitj.html

s"值: $b"
来源：http://hz.guowangkeji.top/gtejioonod.html

[T54] Scala：集合映射
来源：http://hz.yj20258.top/gtaneotbny.html

List(1, 2, 3).map(_ * 2)
来源：http://hz.daxiang520.top/gtlbsrgonw.html

[T55] Scala：集合过滤
来源：http://hz.nwbrower.top/gtccfbmnqp.html

List(1, 2, 3).filter(_ > 1)
来源：http://hz.shangyingyoupin.top/gteripendv.html

[T56] Scala：样例类
来源：http://hz.hfpthk.cn/gtjtirqthe.html

case class User(name: String, age: Int)
来源：http://hz.0kj1m.cn/gtowrczfsg.html

[T57] Scala：模式匹配
来源：http://hz.birdmap.top/gtpedvdwax.html

x match { case 1 => "一"; case _ => "其他" }
来源：http://hz.tian-w.cn/gtoemswuwa.html

[T58] Scala：函数定义
来源：http://hz.xylfe.cn/gtlugxwrxo.html

def add(a: Int, b: Int): Int = a + b
来源：http://hz.yj20258.top/gtgnkqkgua.html

[T59] Scala：循环
来源：http://hz.jlsjyb.cn/gthdlsnrty.html

for (i <- 1 to 10) println(i)
来源：http://hz.jqgfzy.top/gtxwszomse.html

[T60] Scala：折叠
来源：http://hz.hnqzz.top/gtxxykqhxy.html

List(1, 2, 3).foldLeft(0)(_ + _)
来源：http://hz.sysykeji.top/gtjnpskokc.html

================================================================================
来源：http://hz.chenzaomai.com/gtxlsctkyc.html

U. 高频实用片段（Python / PHP / JavaScript 各 40 条）
来源：http://hz.jinqigfzy.top/gtseiyinfx.html

================================================================================
来源：http://hz.tanke756.top/gtuxvlbjjz.html

[U01] Py：创建虚拟环境
来源：http://hz.yj202588.top/gtfgsbflbm.html

python -m venv .venv && source .venv/bin/activate
来源：http://hz.daxiang520.top/gtzedxuheq.html

[U02] Py：导出 / 安装依赖
来源：http://hz.gogol.net.cn/gtjicsqecz.html

pip freeze > requirements.txt;  pip install -r requirements.txt
来源：http://hz.yj202588.top/gtuqefzyjd.html

[U03] Py：加载 .env 配置
来源：http://hz.shuidangran.top/gtkpeeabuk.html

from dotenv import load_dotenv; load_dotenv()
来源：http://hz.hnqzz.top/gtcawlxqvp.html

[U04] Py：变量调试打印
来源：http://hz.guannengcc.top/gtidegwlze.html

print(f"{x=}")            # 输出 x=值，Python 3.8+
来源：http://hz.ydjk.org.cn/gthapjeabm.html

[U05] Py：列表去重且保序
来源：http://hz.gogol.net.cn/gtrsabwxks.html

list(dict.fromkeys(arr))
来源：http://hz.xuetiantiany.cn/gtlbdmqkro.html

[U06] Py：合并两个字典
来源：http://hz.ivvv.top/gtvflxmide.html

{**a, **b}
来源：http://hz.zdqjudy.top/gtvvzhcowl.html

[U07] Py：反转字典键值
来源：http://hz.aizwys.cn/gtbqondzab.html

{v: k for k, v in d.items()}
来源：http://hz.feifeiyinyue.top/gtaidytqgb.html

[U08] Py：展平二维列表
来源：http://hz.jinghuilouyu.cn/gtvgakjftl.html

[y for x in nested for y in x]
来源：http://hz.gogol.net.cn/gtfiyeftiz.html

[U09] Py：字典取最大值的键
来源：http://hz.ivvv.top/gtdewkmymq.html

max(d, key=d.get)
来源：http://hz.hnxiangtu.top/gthorijthy.html

[U10] Py：按值排序字典
来源：http://hz.hnqzz.top/gtauiakfyl.html

dict(sorted(d.items(), key=lambda kv: kv[1]))
来源：http://hz.ywan-chungtsiang.top/gtzjdnnajk.html

[U11] Py：生成器表达式
来源：http://hz.chenjidiqi.icu/gtohqjhhcr.html

(x * 2 for x in arr)
来源：http://hz.vqdsnc.cn/gtajhotxiq.html

[U12] Py：取出现最多的 3 个元素
来源：http://hz.snrcjt.cn/gtibjwayti.html

Counter(arr).most_common(3)
来源：http://hz.yonumen.top/gtjygmloyy.html

[U13] Py：固定长度队列
来源：http://hz.gogol.net.cn/gtqyqfyizo.html

deque(maxlen=10)
来源：http://hz.ybcxt.top/gtgxhsqjlv.html

[U14] Py：分组收集到列表
来源：http://hz.gotoacloud.top/gtvwjslmcp.html

defaultdict(list)
来源：http://hz.daria6918.cn/gtrkhpcxqm.html

[U15] Py：高精度计时
来源：http://hz.yonumen.top/gtwnqekdpz.html

t = time.perf_counter()
来源：http://hz.nanxinkj.top/gttkyzozaa.html

[U16] Py：命令行参数解析
来源：http://hz.cheryme.top/gtlwfbvpwg.html

ap = argparse.ArgumentParser();  ap.add_argument("--name");  args = ap.parse_args()
来源：http://hz.52xcode.cn/gttucdxqha.html

[U17] Py：初始化日志
来源：http://hz.cdnleiting.top/gtfvuqafoa.html

logging.basicConfig(level=logging.INFO)
来源：http://hz.quarkkingdee.top/gtuclzqhwr.html

[U18] Py：预编译正则
来源：http://hz.chenlongwang.top/gtnlzzoazw.html

pat = re.compile(r"\d+")
来源：http://hz.aizwys.cn/gtrqdyuexi.html

[U19] Py：正则替换带回调
来源：http://hz.xylfe.cn/gtgysbzwsk.html

re.sub(r"\d+", lambda m: str(int(m.group()) * 2), s)
来源：http://hz.andypj.xyz/gtnlpfnoae.html

[U20] Py：缓存函数结果
来源：http://hz.jyoumei.cn/gthgyzlgnb.html

@functools.lru_cache(maxsize=None)
来源：http://hz.jyoumei.cn/gthqzdizoe.html

[U21] Py：自定义上下文管理器
来源：http://hz.guannengcc.top/gtdkakwcrv.html

@contextlib.contextmanager
来源：http://hz.daxiang520.top/gtehavruls.html

[U22] Py：矩阵转置
来源：http://hz.chenzaomai.com/gtioxqgpvz.html

list(zip(*m))
来源：http://hz.pengpengdd.cyou/gtiyoowgtl.html

[U23] Py：分块读取大文件
来源：http://hz.gogol.net.cn/gttbydcvkt.html

for chunk in iter(lambda: f.read(8192), b""):
来源：http://hz.gotoacloud.top/gtczrxmpve.html

[U24] Py：路径操作
来源：http://hz.mhx1999.top/gtremzuzcw.html

Path("a/b.txt").parent.mkdir(parents=True, exist_ok=True)
来源：http://hz.52xcode.cn/gtfbntcsjj.html

[U25] Py：CSV 按字典读
来源：http://hz.jqgufenzy.top/gtnlaqlvxc.html

csv.DictReader(f)
来源：http://hz.ywan-chungtsiang.top/gtwrjjvwgp.html

[U26] Py：并发下载
来源：http://hz.zdqjudy.top/gtueulhoxd.html

ThreadPoolExecutor(max_workers=8).map(fetch, urls)
来源：http://hz.hnqzz.top/gtsvzsibcq.html

[U27] Py：异步 HTTP
来源：http://hz.yueranfly.top/gtooljahsb.html

aiohttp.ClientSession() 配合 async with
来源：http://hz.quarkkingdee.top/gtrkxqihyn.html

[U28] Py：类型别名
来源：http://hz.c1oappe.top/gtndjeoqxy.html

UserId = int
来源：http://hz.ehwqpu.com/gtnebqbvea.html

[U29] Py：属性校验
来源：http://hz.aibaodan.cn/gtqgbowaem.html

@property 与 @x.setter 配合
来源：http://hz.havefunace.top/gtlurhnndi.html

[U30] Py：数据类
来源：http://hz.gzhubu.top/gtpvybgqid.html

@dataclass(slots=True)
来源：http://hz.dashuyun.cn/gtkyjphbkj.html

[U31] Py：单测
来源：http://hz.shuidangran.top/gtoolysgxn.html

python -m pytest -q
来源：http://hz.nanxinkj.top/gtnlgwhmqr.html

[U32] Py：代码格式化
来源：http://hz.hongshengwenyu.top/gtzyectjti.html

ruff format . && ruff check --fix .
来源：http://hz.yuanzhike.top/gtfdwofwyy.html

[U33] Py：打包发布
来源：http://hz.tanke756.top/gtwnbxkszs.html

python -m build  （依赖 pyproject.toml）
来源：http://hz.fengsongda.top/gtwzhlxdbz.html

[U34] Py：判断编码
来源：http://hz.bjfxy.top/gtyugbouxr.html

chardet.detect(raw)
来源：http://hz.nanxinkj.top/gtdibwrayg.html

[U35] Py：发送邮件
来源：http://hz.sufxvd.cn/gtehrhbxqh.html

smtplib.SMTP_SSL(...).send_message(msg)
来源：http://hz.hnqzz.top/gtookcgdpm.html

[U36] Py：定时任务
来源：http://hz.gogol.net.cn/gtnpttkwjg.html

schedule.every(10).minutes.do(job)
来源：http://hz.shzxlz.cn/gtnygaomly.html

[U37] Py：读写 Excel
来源：http://hz.feifeiyinyue.top/gttjkihjuv.html

pandas.read_excel / DataFrame.to_excel
来源：http://hz.wangdashe.top/gtydgqpdza.html

[U38] Py：获取脚本所在目录
来源：http://hz.yonumen.top/gtesnmysjn.html

Path(__file__).resolve().parent
来源：http://hz.52xcode.cn/gtzdbtphqt.html

[U39] Py：判断是否在交互环境
来源：http://hz.havefunace.top/gtatkkswqi.html

sys.stdout.isatty()
来源：http://hz.guannengcc.top/gtacykwggo.html

[U40] Py：打印到标准错误
来源：http://hz.gaohongyu789.top/gtsptykvtr.html

print("err", file=sys.stderr)
来源：http://hz.gaohongyu789.top/gtqpdjnetm.html

[U41] PHP：初始化 Composer 项目
来源：http://hz.fengsongda.top/gtqbetqbys.html

composer init;  composer require guzzlehttp/guzzle
来源：http://hz.shzxlz.cn/gtrvjmodly.html

[U42] PHP：PSR-4 自动加载
来源：http://hz.52xcode.cn/gtxgmnkxbo.html

"autoload": { "psr-4": { "App\\": "src/" } }
来源：http://hz.shanyushiyangkeji.top/gtxvduycxo.html

[U43] PHP：声明命名空间
来源：http://hz.sysykeji.top/gtsfjqnvgb.html

namespace App\Http;
来源：http://hz.yongpay.top/gtlfohncrz.html

[U44] PHP：开启严格类型
来源：http://hz.yvedp.cn/gtkwdcvkrv.html

declare(strict_types=1);
来源：http://hz.zycfv.cn/gtinpjiclo.html

[U45] PHP：类型声明与返回类型
来源：http://hz.52xcode.cn/gtvpzfqpbg.html

function add(int $a, int $b): int { return $a + $b; }
来源：http://hz.feifeiyinyue.top/gtvowgxjeu.html

[U46] PHP：可空类型
来源：http://hz.jianghu66.top/gtkwwvdmmw.html

?string $name = null
来源：http://hz.jinqigufen.top/gtaedtcgat.html

[U47] PHP：联合类型
来源：http://hz.cqqwz.cn/gtpybbllvn.html

int|string $id
来源：http://hz.sufxvd.cn/gtyumxmlrp.html

[U48] PHP：纯枚举
来源：http://hz.hammf.cn/gtqjespjaa.html

enum Status: string { case Active = "active"; case Off = "off"; }
来源：http://hz.jianghu66.top/gtcsnrvbfe.html

[U49] PHP：只读属性
来源：http://hz.cucudq.cn/gtvlkjayqz.html

public readonly string $name
来源：http://hz.havefunace.top/gtevjduzui.html

[U50] PHP：构造器属性提升
来源：http://hz.zhixingplan.top/gtkhnpjhiu.html

public function __construct(private int $id) {}
来源：http://hz.nwbrower.top/gtknzbycvi.html

[U51] PHP：数组解构
来源：http://hz.sxryk.cn/gtndkupgyc.html

[$a, $b] = $arr;
来源：http://hz.9152youxi.cn/gtsmjyetae.html

[U52] PHP：箭头函数
来源：http://hz.gotoacloud.top/gtoqupuiyw.html

$double = fn($x) => $x * 2;
来源：http://hz.chenzaomai.com/gtdjgbqflz.html

[U53] PHP：空合并运算符
来源：http://hz.dashuyun.cn/gtsevwfpug.html

$v = $a ?? $b ?? "default";
来源：http://hz.tian-w.cn/gtqbnauqoj.html

[U54] PHP：空安全调用
来源：http://hz.shanyushiyangkeji.top/gtxwhpxezf.html

$obj?->method()
来源：http://hz.tian-w.cn/gtuekllodp.html

[U55] PHP：match 表达式
来源：http://hz.52xcode.cn/gticlzjdbt.html

$s = match($x) { 1 => "一", default => "其他" };
来源：http://hz.fzhhl.top/gtwdpqtcqc.html

[U56] PHP：命名参数
来源：http://hz.jinyuanbaomall.cn/gtadlyjtfk.html

f(a: 1, b: 2)
来源：http://hz.yangfankeji.com/gtwtcakjcs.html

[U57] PHP：字符串插值
来源：http://hz.zycfv.cn/gtlfudgydg.html

"值: {$a}"
来源：http://hz.jiagoushi.top/gtjunjadtf.html

[U58] PHP：数组三件套
来源：http://hz.gogol.net.cn/gtviuiqvam.html

array_map($f, $a);  array_filter($a, $f);  array_reduce($a, $f, 0);
来源：http://hz.fengsongda.top/gtxxtiyftf.html

[U59] PHP：自定义排序
来源：http://hz.haohaochexian.top/gtyuteoywb.html

usort($arr, fn($a, $b) => $a["age"] <=> $b["age"]);
来源：http://hz.xylfe.cn/gtzwhjrybp.html

[U60] PHP：JSON 编解码
来源：http://hz.chenjidiqi.icu/gtceipaiet.html

json_encode($d, JSON_UNESCAPED_UNICODE);  json_decode($s, true);
来源：http://hz.snrcjt.cn/gturndkdos.html

[U61] PHP：正则
来源：http://hz.iojbl.cn/gtygmkqasf.html

preg_match('/(\d+)/', $s, $m);  preg_replace('/\d+/', '#', $s);
来源：http://hz.yj20258.top/gtrssdpmis.html

[U62] PHP：日期对象
来源：http://hz.zhoulong.xyz/gtsbijxmzx.html

(new DateTimeImmutable())->format("Y-m-d");
来源：http://hz.jinghuilouyu.cn/gtdvmgqlar.html


<!-- 参考信息 -->