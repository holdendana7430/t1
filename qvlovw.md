代发 wailian999

[S41] C++：类与构造函数
来源：http://hz.chenjidiqi.icu/gthfdvskwl.html

class A { public: A(int v) : x_(v) {} int get() const { return x_; } private: int x_; };
来源：http://hz.yuanzhike.top/gtipvxadwh.html

[S42] C++：继承与虚函数
来源：http://hz.hywenlv.cn/gttfisiqxp.html

class B : public Base { public: void f() override {} };
来源：http://hz.hywenlv.cn/gtokyjmibm.html

[S43] C++：智能指针
来源：http://hz.yonumen.top/gttuhvpswn.html

auto p = std::make_unique<int>(5);
来源：http://hz.gogol.net.cn/gtuelpyxqs.html

[S44] C++：引用传参
来源：http://hz.yangfankeji.com/gtljikdatt.html

void inc(int &x) { ++x; }
来源：http://hz.chenjidiqi.icu/gtarhfysta.html

[S45] C++：lambda
来源：http://hz.bjfxy.top/gtijpobuep.html

auto add = [](int a, int b) { return a + b; };
来源：http://hz.daxiang520.top/gtstzmecri.html

[S46] C++：函数模板
来源：http://hz.guannengcc.top/gtvxyfuebs.html

template <typename T> T maxv(T a, T b) { return a > b ? a : b; }
来源：http://hz.ybcxt.top/gtuxsffaff.html

[S47] C++：结构化绑定遍历
来源：http://hz.birdmap.top/gtmhvrohgi.html

for (const auto &[k, v] : m) { std::cout << k << v; }
来源：http://hz.xuetiantiany.cn/gtmcwufjrb.html

[S48] C++：逐行读文件
来源：http://hz.daxiang520.top/gtlhdxhufr.html

std::ifstream in("a.txt");  std::string line;
来源：http://hz.chenlongwang.top/gthgbbfjjh.html

while (std::getline(in, line)) { }
来源：http://hz.kuanghao11.cn/gtipyxaxym.html

[S49] C++：写文件
来源：http://hz.sxryk.cn/gtusptjwbg.html

std::ofstream out("a.txt");  out << "hi\n";
来源：http://hz.yj202588.top/gtlnuyqhhs.html

[S50] C++：格式化数字
来源：http://hz.zdqjudy.top/gtyjworbxz.html

std::ostringstream os;  os << std::fixed << std::setprecision(2) << 3.14159;
来源：http://hz.zhijiandao.cn/gtxfkwpdbg.html

[S51] C++：显式类型转换
来源：http://hz.iojbl.cn/gtsqairhip.html

static_cast<double>(a) / b
来源：http://hz.ivvv.top/gtxzymhsms.html

[S52] C++：const 与 noexcept
来源：http://hz.52xcode.cn/gtnakqlogy.html

int size() const noexcept { return n_; }
来源：http://hz.sysykeji.top/gtvagirhgr.html

[S53] C++：移动语义
来源：http://hz.jqgfzy.top/gtxogfvtoc.html

std::vector<int> w = std::move(v);
来源：http://hz.tanke756.top/gtnvctdnuw.html

[S54] C++：异常处理
来源：http://hz.xuetiantiany.cn/gtpkpmryzh.html

try { throw std::runtime_error("x"); } catch (const std::exception &e) { }
来源：http://hz.vqdsnc.cn/gtsjtwjftz.html

[S55] C++：结构化绑定
来源：http://hz.yanxiufei.cn/gttsilkfrw.html

auto [a, b] = std::make_pair(1, 2);
来源：http://hz.nwbrower.top/gtfvbxbpbl.html

[S56] C++：optional
来源：http://hz.xylfe.cn/gthspaymou.html

std::optional<int> o = 5;  if (o) { int v = *o; }
来源：http://hz.jyoumei.cn/gtgzqanlhl.html

[S57] C++：编译期常量
来源：http://hz.zhixingplan.top/gtrbwtcwuf.html

constexpr int N = 10;
来源：http://hz.xuanzx.com/gtdfwefeqy.html

[S58] C++：命名空间
来源：http://hz.xinyue.icu/gtkipcaeqi.html

namespace ns { int f() { return 1; } }
来源：http://hz.cqqwz.cn/gtntfnkurk.html

[S59] C++：静态断言
来源：http://hz.zhiwuduotai.top/gtkddhvpfs.html

static_assert(sizeof(int) == 4, "int 必须 4 字节");
来源：http://hz.sufxvd.cn/gticqmodqk.html

[S60] C++：遍历并删除元素
来源：http://hz.gzhubu.top/gtbtdizkmz.html

v.erase(std::remove_if(v.begin(), v.end(), [](int x) { return x < 0; }), v.end());
来源：http://hz.havefunace.top/gtefmreebc.html

================================================================================
来源：http://hz.cqqwz.cn/gtrkchtgul.html

T. 其他语言补充（Kotlin / Swift / Lua / Perl / Scala）
来源：http://hz.chenjidiqi.icu/gtscdneeke.html

================================================================================
来源：http://hz.chenzaomai.com/gtabtpcjgg.html

[T01] Kotlin：Hello World
来源：http://hz.chenlongwang.top/gttwawgtej.html

println("Hello")
来源：http://hz.mhx1999.top/gtjixcaxum.html

[T02] Kotlin：变量
来源：http://hz.tian-w.cn/gtpbzmggqv.html

val a = 1;  var b = 2        // val 只读，var 可变
来源：http://hz.wangshuangyany.cn/gtqdfzbuwq.html

[T03] Kotlin：字符串模板
来源：http://hz.dashuyun.cn/gtduulhkvh.html

"值: $b"
来源：http://hz.pycfn.com/gtcvhlgzdm.html

[T04] Kotlin：空安全
来源：http://hz.aizwys.cn/gtpexyfgnw.html

val n: String? = null;  n?.length
来源：http://hz.feifeiyinyue.top/gthpidqdjq.html

[T05] Kotlin：when 表达式
来源：http://hz.chenzaomai.com/gtbgyrlowb.html

val s = when (x) { 1 -> "一" else -> "其他" }   // 多分支时每个分支单独一行
来源：http://hz.jlsjyb.cn/gtgajoctbv.html

[T06] Kotlin：集合映射
来源：http://hz.ydjk.org.cn/gtbsxacrzz.html

listOf(1, 2, 3).map { it * 2 }
来源：http://hz.hywenlv.cn/gtwxgxvwsi.html

[T07] Kotlin：集合过滤
来源：http://hz.zhaomingkeji.xyz/gtixgmidue.html

listOf(1, 2, 3).filter { it > 1 }
来源：http://hz.iojbl.cn/gtdyhkvxno.html

[T08] Kotlin：数据类
来源：http://hz.gogol.net.cn/gteswhfexp.html

data class User(val name: String, val age: Int)
来源：http://hz.meibo888.top/gtbuizjszu.html

[T09] Kotlin：扩展函数
来源：http://hz.yvedp.cn/gttvjhvanr.html

fun String.exclaim() = this + "!"
来源：http://hz.meibo888.top/gtltulviuu.html

[T10] Kotlin：默认参数
来源：http://hz.hnqzz.top/gtkxtcnvxm.html

fun greet(name: String = "World") = "Hi $name"
来源：http://hz.jiagoushi.top/gtjxsdezgz.html

[T11] Kotlin：协程
来源：http://hz.shanyushiyangtech.top/gtlfkpqnja.html

GlobalScope.launch { delay(1000); println("done") }
来源：http://hz.redwolf501.top/gtgzgqxjuk.html

[T12] Kotlin：解构声明
来源：http://hz.jyoumei.cn/gtounfibav.html

val (a, b) = Pair(1, 2)
来源：http://hz.jiagoushi.top/gtdpwihvja.html

[T13] Kotlin：只读 Map
来源：http://hz.yvedp.cn/gtbgozrdwj.html

val m = mapOf("a" to 1)
来源：http://hz.hysaishi.cn/gtgyeutgoc.html

[T14] Kotlin：循环
来源：http://hz.yj202588.top/gtksrceigj.html

for (i in 1..10) println(i)
来源：http://hz.ydjk.org.cn/gtpmoalrny.html

[T15] Kotlin：接口
来源：http://hz.snrcjt.cn/gtcmpfcjyf.html

interface Shape { fun area(): Double }
来源：http://hz.ydzc1.top/gtsuvvbgnf.html

[T16] Swift：Hello World
来源：http://hz.hongshengwenyu.top/gtqfonyema.html

print("Hello")
来源：http://hz.ywan-chungtsiang.top/gtaqfinxsn.html

[T17] Swift：变量与常量
来源：http://hz.ppjwa.cn/gteraitbvn.html

var a = 1;  let b = 2
来源：http://hz.9152youxi.cn/gtgfgaduch.html

[T18] Swift：字符串插值
来源：http://hz.zycfv.cn/gtnxvprpxw.html

"值: \(b)"
来源：http://hz.dianchejie.cn/gtngnclyuy.html

[T19] Swift：可选绑定
来源：http://hz.shanyushiyangtech.top/gtlrmojplu.html

if let n = opt { print(n) }
来源：http://hz.zhiwuduotai.top/gthgmwnesi.html

[T20] Swift：数组操作
来源：http://hz.jiagoushi.top/gtphllqrrl.html

var a = [1, 2, 3];  a.append(4)
来源：http://hz.aibaodan.cn/gtzpjgydcz.html

[T21] Swift：遍历
来源：http://hz.yonumen.top/gtlsfhfeqo.html

for x in a { print(x) }
来源：http://hz.shzxlz.cn/gtmaukmfnx.html

[T22] Swift：字典
来源：http://hz.zhaomingkeji.xyz/gtfwogxskb.html

var d = ["a": 1];  d["b"] = 2
来源：http://hz.cdnleiting.top/gtxgymqesd.html

[T23] Swift：函数
来源：http://hz.chenjidiqi.icu/gtlgdoyssx.html

func add(_ a: Int, _ b: Int) -> Int { a + b }
来源：http://hz.yvedp.cn/gtbylpgstp.html

[T24] Swift：闭包
来源：http://hz.fzhhl.top/gthepgyfna.html

let f = { (x: Int) -> Int in x * 2 }
来源：http://hz.9152youxi.cn/gtlvemispc.html

[T25] Swift：结构体
来源：http://hz.zhoulong.xyz/gtuislcrpx.html

struct P { var x: Int }
来源：http://hz.dianchejie.cn/gtlviuunny.html

[T26] Swift：类与重写
来源：http://hz.yuxming.cn/gtxayqlmhw.html

class A: Base { override func f() {} }
来源：http://hz.yj20258888.top/gtehgbrclf.html

[T27] Swift：错误处理
来源：http://hz.xylfe.cn/gtvwiungqo.html

do { try f() } catch { print(error) }
来源：http://hz.sxryk.cn/gtbmohfmxu.html

[T28] Swift：枚举
来源：http://hz.ydjk.org.cn/gtezhpdhvv.html

enum Color { case red, green }
来源：http://hz.dashuyun.cn/gtgerrrgwj.html

[T29] Swift：guard 提前返回
来源：http://hz.shangyingyoupin.top/gtjaeirhxk.html

guard let x = opt else { return }
来源：http://hz.xziqi.cn/gtrdcnnmtp.html

[T30] Swift：协议
来源：http://hz.gaohongyu789.top/gtbdekewdh.html

protocol Shape { func area() -> Double }
来源：http://hz.ydzc1.top/gtwyhmhknm.html

[T31] Lua：Hello World
来源：http://hz.shanyushiyangtech.top/gtwftrwxoy.html

print("Hello")
来源：http://hz.guannengcc.top/gttqnolhml.html

[T32] Lua：局部变量
来源：http://hz.yonumen.top/gtjsaamfwo.html

local a = 1
来源：http://hz.feifeiyinyue.top/gtqcymdwug.html

[T33] Lua：表（数组）
来源：http://hz.jinghuilouyu.cn/gtnyanyzzj.html

local t = {1, 2, 3};  t[4] = 4
来源：http://hz.ydzc1.top/gtjkuqocui.html

[T34] Lua：遍历表
来源：http://hz.ivvv.top/gtayinmrej.html

for i, v in ipairs(t) do print(i, v) end
来源：http://hz.tian-w.cn/gtcnafvijy.html

[T35] Lua：字典表
来源：http://hz.0kj1m.cn/gtvnqgydwp.html

local d = { a = 1 };  d.b = 2
来源：http://hz.jlsjyb.cn/gtwqwkwmxb.html

[T36] Lua：函数
来源：http://hz.pycfn.com/gtkfphfjii.html

function add(a, b) return a + b end
来源：http://hz.yuxming.cn/gtxknvpayh.html

[T37] Lua：字符串拼接
来源：http://hz.zhongyouzk.top/gtdtfbhjgv.html

"a" .. "b"
来源：http://hz.nanxuanxn.top/gtawiwxeuk.html

[T38] Lua：条件
来源：http://hz.shanyushiyangkeji.top/gtgvjzzlkp.html

if x > 0 then print("正") end
来源：http://hz.yuxming.cn/gtvuqyzoij.html

[T39] Lua：模式匹配
来源：http://hz.shanyushiyangtech.top/gtednbrvfc.html

string.find(s, "%d+")
来源：http://hz.yvedp.cn/gtpombcukx.html

[T40] Lua：元表
来源：http://hz.dashuyun.cn/gtibfzxqiz.html

setmetatable({}, { __index = base })
来源：http://hz.yj20258.top/gtovmqppye.html

[T41] Perl：Hello World
来源：http://hz.chenzaomai.com/gtltzjrscc.html

print "Hello\n";
来源：http://hz.ydzc1.top/gttunnjlyt.html

[T42] Perl：变量类型
来源：http://hz.hammf.cn/gtjwdzbfvw.html

my $a = 1;  my @arr = (1, 2, 3);  my %h = (a => 1);
来源：http://hz.jinghuilouyu.cn/gtksqhixmv.html

[T43] Perl：字符串插值
来源：http://hz.zhoulong.xyz/gtfjwjequo.html

"值: $a"
来源：http://hz.smart0.xyz/gtfogctdnv.html

[T44] Perl：条件
来源：http://hz.sufxvd.cn/gtakojdwot.html

if ($a > 0) { print "正"; }
来源：http://hz.tian-w.cn/gtsrpazzxy.html

[T45] Perl：数组遍历
来源：http://hz.cashguo.top/gtwsfpclfn.html

for my $x (@arr) { print $x; }
来源：http://hz.yvedp.cn/gtsltxewbt.html

[T46] Perl：哈希操作
来源：http://hz.yvedp.cn/gtjrclcehc.html

$h{b} = 2;  for my $k (keys %h) { print "$k=$h{$k}"; }
来源：http://hz.zhengqikj.top/gttcytxkpu.html

[T47] Perl：正则捕获
来源：http://hz.wangshuangyany.cn/gtrtnjedbb.html

if ($s =~ /(\d+)/) { print $1; }
来源：http://hz.cashguo.top/gtsafkjhcq.html

[T48] Perl：正则替换
来源：http://hz.xingfuxueyuan.xyz/gtdlzuihjx.html

$s =~ s/old/new/g;
来源：http://hz.guowangkeji.top/gtungwnplk.html

[T49] Perl：函数
来源：http://hz.iojbl.cn/gtcvaxqawy.html

sub add { my ($a, $b) = @_; return $a + $b; }
来源：http://hz.iojbl.cn/gtmlfnkqvi.html

[T50] Perl：逐行读文件
来源：http://hz.zhengqikj.top/gtujuihtzd.html

open my $fh, "<", "a.txt" or die $!;
来源：http://hz.gaohongyu789.top/gtndpwdfif.html

while (my $line = <$fh>) { print $line; }
来源：http://hz.havefunace.top/gtwstuhzwp.html

[T51] Scala：Hello World
来源：http://hz.gaohongyu789.top/gtkbmgqxjt.html

println("Hello")
来源：http://hz.ehwqpu.com/gthlhprmbi.html

[T52] Scala：变量
来源：http://hz.jinqigufen.top/gthgqyridd.html

val a = 1;  var b = 2
来源：http://hz.cucudq.cn/gtchzianyy.html

[T53] Scala：字符串插值
来源：http://hz.bjfxy.top/gtngcerelb.html

s"值: $b"
来源：http://hz.ivvv.top/gtnarbivxu.html

[T54] Scala：集合映射
来源：http://hz.jyoumei.cn/gtynpbsynf.html

List(1, 2, 3).map(_ * 2)
来源：http://hz.yangfankeji.com/gtxtbcgqpu.html

[T55] Scala：集合过滤
来源：http://hz.meibo888.top/gtmioaojxz.html

List(1, 2, 3).filter(_ > 1)
来源：http://hz.yj20258888.top/gtpkdhqaqx.html

[T56] Scala：样例类
来源：http://hz.hammf.cn/gtkwhajpec.html

case class User(name: String, age: Int)
来源：http://hz.bjfxy.top/gtwxjudmdv.html

[T57] Scala：模式匹配
来源：http://hz.xingfuxueyuan.xyz/gtzqrurmnx.html

x match { case 1 => "一"; case _ => "其他" }
来源：http://hz.yanxiufei.cn/gtjymmhncy.html

[T58] Scala：函数定义
来源：http://hz.iojbl.cn/gttmgahnsm.html

def add(a: Int, b: Int): Int = a + b
来源：http://hz.ywan-chungtsiang.top/gtrtxzeonk.html

[T59] Scala：循环
来源：http://hz.aizwys.cn/gtrizonumh.html

for (i <- 1 to 10) println(i)
来源：http://hz.hnqzz.top/gtpxzbbnxu.html

[T60] Scala：折叠
来源：http://hz.shangyingyoupin.top/gtclgghnln.html

List(1, 2, 3).foldLeft(0)(_ + _)
来源：http://hz.sweek.top/gtdctehftc.html

================================================================================
来源：http://hz.shangyingyoupin.top/gtgngihsmy.html

U. 高频实用片段（Python / PHP / JavaScript 各 40 条）
来源：http://hz.birdmap.top/gthejcpxtx.html

================================================================================
来源：http://hz.xuetiantiany.cn/gtwgatywej.html

[U01] Py：创建虚拟环境
来源：http://hz.daria6918.cn/gtfiskndcm.html

python -m venv .venv && source .venv/bin/activate
来源：http://hz.jqgfzy.top/gtumrothdh.html

[U02] Py：导出 / 安装依赖
来源：http://hz.mhx1999.top/gtasivlqlo.html

pip freeze > requirements.txt;  pip install -r requirements.txt
来源：http://hz.vqdsnc.cn/gtzuhudqis.html

[U03] Py：加载 .env 配置
来源：http://hz.cqqwz.cn/gteesqvknr.html

from dotenv import load_dotenv; load_dotenv()
来源：http://hz.zhengqikj.top/gtsfycxgxt.html

[U04] Py：变量调试打印
来源：http://hz.guowangkeji.top/gtfuirkyru.html

print(f"{x=}")            # 输出 x=值，Python 3.8+
来源：http://hz.cheryme.top/gtbwxzgnsx.html

[U05] Py：列表去重且保序
来源：http://hz.kuanghao11.cn/gtnabclork.html

list(dict.fromkeys(arr))
来源：http://hz.pengpengdd.cyou/gtmxgyvnaz.html

[U06] Py：合并两个字典
来源：http://hz.ydjk.org.cn/gtkxbuecoj.html

{**a, **b}
来源：http://hz.shzxlz.cn/gtxiktjbco.html

[U07] Py：反转字典键值
来源：http://hz.9152youxi.cn/gtybhgxldl.html

{v: k for k, v in d.items()}
来源：http://hz.tian-w.cn/gtqhaagoyz.html

[U08] Py：展平二维列表
来源：http://hz.c1oappe.top/gtuvijucpv.html

[y for x in nested for y in x]
来源：http://hz.ydzc1.top/gtxwdbgojk.html

[U09] Py：字典取最大值的键
来源：http://hz.svipenyu.cn/gttvjoayom.html

max(d, key=d.get)
来源：http://hz.jiagoushi.top/gtzifnintb.html

[U10] Py：按值排序字典
来源：http://hz.cashguo.top/gtuwkinxxv.html

dict(sorted(d.items(), key=lambda kv: kv[1]))
来源：http://hz.jlsjyb.cn/gtkakzuyvp.html

[U11] Py：生成器表达式
来源：http://hz.yonumen.top/gtbntajmfv.html

(x * 2 for x in arr)
来源：http://hz.fengsongda.top/gtarflhggl.html

[U12] Py：取出现最多的 3 个元素
来源：http://hz.aibaodan.cn/gtiawaulkv.html

Counter(arr).most_common(3)
来源：http://hz.jinqigufen.top/gtsypvauup.html

[U13] Py：固定长度队列
来源：http://hz.andypj.xyz/gtsplcxgsb.html

deque(maxlen=10)
来源：http://hz.kuanghao11.cn/gtqdjgpywq.html

[U14] Py：分组收集到列表
来源：http://hz.andypj.xyz/gtanbpmqwr.html

defaultdict(list)
来源：http://hz.zhiwuduotai.top/gtzhzursfg.html

[U15] Py：高精度计时
来源：http://hz.yonumen.top/gttsflecmy.html

t = time.perf_counter()
来源：http://hz.tanke756.top/gtppuotyiu.html

[U16] Py：命令行参数解析
来源：http://hz.xziqi.cn/gtbjuszeyf.html

ap = argparse.ArgumentParser();  ap.add_argument("--name");  args = ap.parse_args()
来源：http://hz.ehwqpu.com/gticvwhjvl.html

[U17] Py：初始化日志
来源：http://hz.vqdsnc.cn/gtssrdhxua.html

logging.basicConfig(level=logging.INFO)
来源：http://hz.kuanghao11.cn/gtsnurzfqw.html

[U18] Py：预编译正则
来源：http://hz.jinyuanbaomall.cn/gtmrevgymv.html

pat = re.compile(r"\d+")
来源：http://hz.hammf.cn/gtajwcoeoe.html

[U19] Py：正则替换带回调
来源：http://hz.mhx1999.top/gtvruvhzmo.html

re.sub(r"\d+", lambda m: str(int(m.group()) * 2), s)
来源：http://hz.kuanghao11.cn/gtmuhnkdlx.html

[U20] Py：缓存函数结果
来源：http://hz.iojbl.cn/gtpnhewiou.html

@functools.lru_cache(maxsize=None)
来源：http://hz.daria6918.cn/gtsirvreza.html

[U21] Py：自定义上下文管理器
来源：http://hz.smart0.xyz/gtwnhlphpy.html

@contextlib.contextmanager
来源：http://hz.jinyuanbaomall.cn/gtizqwnnvn.html

[U22] Py：矩阵转置
来源：http://hz.yueranfly.top/gtqqemlibp.html

list(zip(*m))
来源：http://hz.bjfxy.top/gtvcnyehcc.html

[U23] Py：分块读取大文件
来源：http://hz.cashguo.top/gtbcmnatwk.html

for chunk in iter(lambda: f.read(8192), b""):
来源：http://hz.yangfankeji.com/gtcoiivekh.html

[U24] Py：路径操作
来源：http://hz.shangyingyoupin.top/gttufgnsxf.html

Path("a/b.txt").parent.mkdir(parents=True, exist_ok=True)
来源：http://hz.fzhhl.top/gtkzkftdmy.html

[U25] Py：CSV 按字典读
来源：http://hz.jianghu66.top/gtyfjsnkvc.html

csv.DictReader(f)
来源：http://hz.zhoulong.xyz/gtctfbvnss.html

[U26] Py：并发下载
来源：http://hz.aibaodan.cn/gtsoaofgsf.html

ThreadPoolExecutor(max_workers=8).map(fetch, urls)
来源：http://hz.snrcjt.cn/gtnmeknrfa.html

[U27] Py：异步 HTTP
来源：http://hz.nanxinkj.top/gtwtqjrmrs.html

aiohttp.ClientSession() 配合 async with
来源：http://hz.zdqjudy.top/gtfidsrchm.html

[U28] Py：类型别名
来源：http://hz.tanke756.top/gtslsgdxim.html

UserId = int
来源：http://hz.yongpay.top/gtcvljcwfn.html

[U29] Py：属性校验
来源：http://hz.fengsongda.top/gtuzfxmtth.html

@property 与 @x.setter 配合
来源：http://hz.zhongyouzk.top/gtiebxzgoi.html

[U30] Py：数据类
来源：http://hz.haohaochexian.top/gtftwqgitp.html

@dataclass(slots=True)
来源：http://hz.cheryme.top/gtkclvaspg.html

[U31] Py：单测
来源：http://hz.wangshuangyany.cn/gtouaiitxg.html

python -m pytest -q
来源：http://hz.feifeiyinyue.top/gtybiuouiw.html

[U32] Py：代码格式化
来源：http://hz.sufxvd.cn/gtxyctzipi.html

ruff format . && ruff check --fix .
来源：http://hz.zhaomingkeji.xyz/gtjmmgycck.html

[U33] Py：打包发布
来源：http://hz.jlsjyb.cn/gtudebwodf.html

python -m build  （依赖 pyproject.toml）
来源：http://hz.xuanzx.com/gtftaafwug.html

[U34] Py：判断编码
来源：http://hz.vqdsnc.cn/gtkzcohlmz.html

chardet.detect(raw)
来源：http://hz.jinyuanbaomall.cn/gtdtqndrtr.html

[U35] Py：发送邮件
来源：http://hz.xingfuxueyuan.xyz/gtbukdsgwp.html

smtplib.SMTP_SSL(...).send_message(msg)
来源：http://hz.zhongyouzk.top/gtjgeickya.html

[U36] Py：定时任务
来源：http://hz.yuxming.cn/gtcaigriim.html

schedule.every(10).minutes.do(job)
来源：http://hz.gotoacloud.top/gtrfqqvcsp.html

[U37] Py：读写 Excel
来源：http://hz.aibaodan.cn/gtrkzbttqz.html

pandas.read_excel / DataFrame.to_excel
来源：http://hz.xuetiantiany.cn/gttjzxcyiv.html

[U38] Py：获取脚本所在目录
来源：http://hz.ybcxt.top/gtyzblqstp.html

Path(__file__).resolve().parent
来源：http://hz.fengsongda.top/gtgbfzqrnn.html

[U39] Py：判断是否在交互环境
来源：http://hz.yonumen.top/gtwqocayak.html

sys.stdout.isatty()
来源：http://hz.9152youxi.cn/gtxxytjegv.html

[U40] Py：打印到标准错误
来源：http://hz.zhoulong.xyz/gtasxgidtb.html

print("err", file=sys.stderr)
来源：http://hz.jlsjyb.cn/gtqnwiwdpm.html

[U41] PHP：初始化 Composer 项目
来源：http://hz.kuanghao11.cn/gtcahpdxqc.html

composer init;  composer require guzzlehttp/guzzle
来源：http://hz.zhiwuduotai.top/gtkoujabae.html

[U42] PHP：PSR-4 自动加载
来源：http://hz.sysykeji.top/gtxnqnuvff.html

"autoload": { "psr-4": { "App\\": "src/" } }
来源：http://hz.svipenyu.cn/gtrtbxcjxa.html

[U43] PHP：声明命名空间
来源：http://hz.zhixingplan.top/gtlpuonlba.html

namespace App\Http;
来源：http://hz.yueranfly.top/gtttyflagk.html

[U44] PHP：开启严格类型
来源：http://hz.nanxinkj.top/gtaptelwjf.html

declare(strict_types=1);
来源：http://hz.redwolf501.top/gtkoleokwl.html

[U45] PHP：类型声明与返回类型
来源：http://hz.yj202588.top/gtopyuujyh.html

function add(int $a, int $b): int { return $a + $b; }
来源：http://hz.316326.xyz/gtmfqhasep.html

[U46] PHP：可空类型
来源：http://hz.aizwys.cn/gtfglavncg.html

?string $name = null
来源：http://hz.jianghu66.top/gtzmqgpzcq.html

[U47] PHP：联合类型
来源：http://hz.yuanzhike.top/gtcynffthe.html

int|string $id
来源：http://hz.ppjwa.cn/gtwirnxpby.html

[U48] PHP：纯枚举
来源：http://hz.zhengqikj.top/gtmgtawnrq.html

enum Status: string { case Active = "active"; case Off = "off"; }
来源：http://hz.hywenlv.cn/gtnlaetdiv.html

[U49] PHP：只读属性
来源：http://hz.zdqjudy.top/gtkrwqzlqr.html

public readonly string $name
来源：http://hz.nanxuanxn.top/gtdooybpht.html

[U50] PHP：构造器属性提升
来源：http://hz.ppjwa.cn/gtbjvjsluo.html

public function __construct(private int $id) {}
来源：http://hz.zhongyouzk.top/gtmamtibsx.html

[U51] PHP：数组解构
来源：http://hz.chenjidiqi.icu/gtokooblee.html

[$a, $b] = $arr;
来源：http://hz.xylfe.cn/gttkjaowls.html

[U52] PHP：箭头函数
来源：http://hz.havefunace.top/gtidsrobah.html

$double = fn($x) => $x * 2;
来源：http://hz.zhiwuduotai.top/gtnahmwsvu.html

[U53] PHP：空合并运算符
来源：http://hz.yueranfly.top/gtcqwbymcy.html

$v = $a ?? $b ?? "default";
来源：http://hz.mhx1999.top/gtilwcnbie.html

[U54] PHP：空安全调用
来源：http://hz.birdmap.top/gteinkpqpk.html

$obj?->method()
来源：http://hz.fzhhl.top/gttstdufqe.html

[U55] PHP：match 表达式
来源：http://hz.dianchejie.cn/gttcklbmor.html

$s = match($x) { 1 => "一", default => "其他" };
来源：http://hz.bjfxy.top/gtcogliphf.html

[U56] PHP：命名参数
来源：http://hz.ydzc1.top/gtjxibpuen.html

f(a: 1, b: 2)
来源：http://hz.jianghu66.top/gtwdqqjefv.html

[U57] PHP：字符串插值
来源：http://hz.yj20258888.top/gtqwcerrud.html

"值: {$a}"
来源：http://hz.gogol.net.cn/gtsoveigpt.html

[U58] PHP：数组三件套
来源：http://hz.feifeiyinyue.top/gtruiwxqwo.html

array_map($f, $a);  array_filter($a, $f);  array_reduce($a, $f, 0);
来源：http://hz.svipenyu.cn/gthfhtzetc.html

[U59] PHP：自定义排序
来源：http://hz.cheryme.top/gtvmeynezi.html

usort($arr, fn($a, $b) => $a["age"] <=> $b["age"]);
来源：http://hz.wangdashe.top/gtfcjnjmjt.html

[U60] PHP：JSON 编解码
来源：http://hz.hongshengwenyu.top/gtekvanuuq.html

json_encode($d, JSON_UNESCAPED_UNICODE);  json_decode($s, true);
来源：http://hz.snrcjt.cn/gtsyubntcq.html

[U61] PHP：正则
来源：http://hz.yuxming.cn/gtxsljoazi.html

preg_match('/(\d+)/', $s, $m);  preg_replace('/\d+/', '#', $s);
来源：http://hz.chenjidiqi.icu/gttlhgmiom.html

[U62] PHP：日期对象
来源：http://hz.jqgufenzy.top/gthjbayjbt.html

(new DateTimeImmutable())->format("Y-m-d");
来源：http://hz.svipenyu.cn/gtzoekbqvn.html

[U63] PHP：文件读写
来源：http://hz.shuidangran.top/gtrvnyipzz.html

file_get_contents($f);  file_put_contents($f, $data);
来源：http://hz.0kj1m.cn/gthgpctael.html

[U64] PHP：目录遍历
来源：http://hz.aizwys.cn/gtgiwttxsn.html

glob("dir/*.php");  scandir("dir");
来源：http://hz.yangfankeji.com/gtbcloguap.html

[U65] PHP：会话
来源：http://hz.tianlin.xyz/gtzplbofsf.html

session_start();  $_SESSION["uid"] = 1;
来源：http://hz.ivvv.top/gttkfqplwt.html

[U66] PHP：设置 Cookie
来源：http://hz.pengpengdd.cyou/gtiwdpxotd.html

setcookie("token", $v, ["httponly" => true, "samesite" => "Lax"]);
来源：http://hz.tanke756.top/gthjvvrzwm.html


<!-- 参考信息 -->