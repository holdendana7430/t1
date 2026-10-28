代发 wailian999

[S37] C++：set
来源：http://hz.cashguo.top/gtcyqdvdip.html

std::set<int> s{1, 2, 3};  s.insert(4);
来源：http://hz.iojbl.cn/gtvbqlxhww.html

[S38] C++：排序
来源：http://hz.gzhubu.top/gtnoiwagzp.html

std::sort(v.begin(), v.end());
来源：http://hz.aibaodan.cn/gtvluckvus.html

[S39] C++：自定义比较器排序
来源：http://hz.birdmap.top/gtuoxbxvxt.html

std::sort(v.begin(), v.end(), [](int a, int b) { return a > b; });
来源：http://hz.fengsongda.top/gtxagptgdf.html

[S40] C++：查找元素
来源：http://hz.ywan-chungtsiang.top/gtvbncdnxu.html

auto it = std::find(v.begin(), v.end(), 3);
来源：http://hz.snrcjt.cn/gtencgzdps.html

[S41] C++：类与构造函数
来源：http://hz.yanxiufei.cn/gtqxppqgtv.html

class A { public: A(int v) : x_(v) {} int get() const { return x_; } private: int x_; };
来源：http://hz.shanyushiyangkeji.top/gtcyrydkdn.html

[S42] C++：继承与虚函数
来源：http://hz.ydjk.org.cn/gtwvrikurb.html

class B : public Base { public: void f() override {} };
来源：http://hz.zhiwuduotai.top/gtqrioeytf.html

[S43] C++：智能指针
来源：http://hz.yangfankeji.com/gtlxgwjndd.html

auto p = std::make_unique<int>(5);
来源：http://hz.nanxuanxn.top/gtxdhyicij.html

[S44] C++：引用传参
来源：http://hz.kuanghao11.cn/gtwxcflwyx.html

void inc(int &x) { ++x; }
来源：http://hz.mhx1999.top/gtjesvwowz.html

[S45] C++：lambda
来源：http://hz.gogol.net.cn/gtmjlokgfb.html

auto add = [](int a, int b) { return a + b; };
来源：http://hz.tianlin.xyz/gtxqhcueib.html

[S46] C++：函数模板
来源：http://hz.9152youxi.cn/gtdduhppfp.html

template <typename T> T maxv(T a, T b) { return a > b ? a : b; }
来源：http://hz.yonumen.top/gtusuvpbmi.html

[S47] C++：结构化绑定遍历
来源：http://hz.andypj.xyz/gtscwblsmx.html

for (const auto &[k, v] : m) { std::cout << k << v; }
来源：http://hz.sysykeji.top/gtulrqctrt.html

[S48] C++：逐行读文件
来源：http://hz.shuidangran.top/gtmkdrrxdq.html

std::ifstream in("a.txt");  std::string line;
来源：http://hz.jqgfzy.top/gtuhpesegt.html

while (std::getline(in, line)) { }
来源：http://hz.xuetiantiany.cn/gtckhfgtez.html

[S49] C++：写文件
来源：http://hz.c1oappe.top/gtqyivyzoa.html

std::ofstream out("a.txt");  out << "hi\n";
来源：http://hz.mhx1999.top/gtgokxbvue.html

[S50] C++：格式化数字
来源：http://hz.yj202588.top/gttvmydcpt.html

std::ostringstream os;  os << std::fixed << std::setprecision(2) << 3.14159;
来源：http://hz.shuidangran.top/gtqcyjpvpp.html

[S51] C++：显式类型转换
来源：http://hz.52xcode.cn/gttwpryjrq.html

static_cast<double>(a) / b
来源：http://hz.redwolf501.top/gtjqyxtfza.html

[S52] C++：const 与 noexcept
来源：http://hz.hammf.cn/gtsjrqombx.html

int size() const noexcept { return n_; }
来源：http://hz.chenlongwang.top/gtmxwbsczg.html

[S53] C++：移动语义
来源：http://hz.tian-w.cn/gtwfjxeioq.html

std::vector<int> w = std::move(v);
来源：http://hz.feifeiyinyue.top/gtymxynaiq.html

[S54] C++：异常处理
来源：http://hz.zhoulong.xyz/gtphujkosi.html

try { throw std::runtime_error("x"); } catch (const std::exception &e) { }
来源：http://hz.yj20258888.top/gtqewedpsy.html

[S55] C++：结构化绑定
来源：http://hz.fengsongda.top/gtebqcqfhk.html

auto [a, b] = std::make_pair(1, 2);
来源：http://hz.pycfn.com/gtwupusskz.html

[S56] C++：optional
来源：http://hz.ppjwa.cn/gttpiomwfb.html

std::optional<int> o = 5;  if (o) { int v = *o; }
来源：http://hz.hywenlv.cn/gtvqzeqoaw.html

[S57] C++：编译期常量
来源：http://hz.fengsongda.top/gtigszewkm.html

constexpr int N = 10;
来源：http://hz.52xcode.cn/gtvxzhkcjk.html

[S58] C++：命名空间
来源：http://hz.jyoumei.cn/gtifmbwtwf.html

namespace ns { int f() { return 1; } }
来源：http://hz.zhiwuduotai.top/gtwnmmflii.html

[S59] C++：静态断言
来源：http://hz.gaohongyu789.top/gtvkdscggx.html

static_assert(sizeof(int) == 4, "int 必须 4 字节");
来源：http://hz.hfpthk.cn/gtmqlpxmnd.html

[S60] C++：遍历并删除元素
来源：http://hz.ydjk.org.cn/gteufqvksv.html

v.erase(std::remove_if(v.begin(), v.end(), [](int x) { return x < 0; }), v.end());
来源：http://hz.zhoulong.xyz/gtsutqlody.html

================================================================================
来源：http://hz.yj20258.top/gteaahkkzk.html

T. 其他语言补充（Kotlin / Swift / Lua / Perl / Scala）
来源：http://hz.shanyushiyangkeji.top/gthocbvwde.html

================================================================================
来源：http://hz.shuidangran.top/gtiygzakxz.html

[T01] Kotlin：Hello World
来源：http://hz.birdmap.top/gtoucpicsq.html

println("Hello")
来源：http://hz.yuanzhike.top/gtoeeuogax.html

[T02] Kotlin：变量
来源：http://hz.tianlin.xyz/gtlmxbiivc.html

val a = 1;  var b = 2        // val 只读，var 可变
来源：http://hz.shzxlz.cn/gtdmswanxa.html

[T03] Kotlin：字符串模板
来源：http://hz.sweek.top/gtngxoxzyg.html

"值: $b"
来源：http://hz.tanke756.top/gtxqgvtdoz.html

[T04] Kotlin：空安全
来源：http://hz.snrcjt.cn/gtyyikeikg.html

val n: String? = null;  n?.length
来源：http://hz.guannengcc.top/gtnnzxmaxd.html

[T05] Kotlin：when 表达式
来源：http://hz.jianghu66.top/gtxkzikrkn.html

val s = when (x) { 1 -> "一" else -> "其他" }   // 多分支时每个分支单独一行
来源：http://hz.xingfuxueyuan.xyz/gtiuvcvojl.html

[T06] Kotlin：集合映射
来源：http://hz.nwbrower.top/gtnqspgwvc.html

listOf(1, 2, 3).map { it * 2 }
来源：http://hz.redwolf501.top/gtrgkpbbgw.html

[T07] Kotlin：集合过滤
来源：http://hz.xuetiantiany.cn/gtgiiabzpi.html

listOf(1, 2, 3).filter { it > 1 }
来源：http://hz.jinqigufen.top/gtmfqeltlw.html

[T08] Kotlin：数据类
来源：http://hz.yonumen.top/gtoosnyomx.html

data class User(val name: String, val age: Int)
来源：http://hz.quarkkingdee.top/gtsoxlzzuq.html

[T09] Kotlin：扩展函数
来源：http://hz.haohaochexian.top/gtwlqjfzsp.html

fun String.exclaim() = this + "!"
来源：http://hz.gzhubu.top/gtdvkwcurb.html

[T10] Kotlin：默认参数
来源：http://hz.hongshengwenyu.top/gtenwileyf.html

fun greet(name: String = "World") = "Hi $name"
来源：http://hz.yongpay.top/gtlizwpglr.html

[T11] Kotlin：协程
来源：http://hz.hfpthk.cn/gtnysqqhhr.html

GlobalScope.launch { delay(1000); println("done") }
来源：http://hz.shanyushiyangtech.top/gtwyjgyxge.html

[T12] Kotlin：解构声明
来源：http://hz.guannengcc.top/gtbomtqsfc.html

val (a, b) = Pair(1, 2)
来源：http://hz.zdqjudy.top/gtlfsfagin.html

[T13] Kotlin：只读 Map
来源：http://hz.shangyingyoupin.top/gtspnigqhp.html

val m = mapOf("a" to 1)
来源：http://hz.sxryk.cn/gtgujwkywq.html

[T14] Kotlin：循环
来源：http://hz.tian-w.cn/gtvexgmofp.html

for (i in 1..10) println(i)
来源：http://hz.nanxuanxn.top/gtuxxvofet.html

[T15] Kotlin：接口
来源：http://hz.ybcxt.top/gthztdlavm.html

interface Shape { fun area(): Double }
来源：http://hz.gotoacloud.top/gtxmzojium.html

[T16] Swift：Hello World
来源：http://hz.shanyushiyangkeji.top/gtcdenznas.html

print("Hello")
来源：http://hz.shangyingyoupin.top/gtnursnbcq.html

[T17] Swift：变量与常量
来源：http://hz.hysaishi.cn/gttoqcntrg.html

var a = 1;  let b = 2
来源：http://hz.jqgufenzy.top/gtmjvomksz.html

[T18] Swift：字符串插值
来源：http://hz.vqdsnc.cn/gtubwmbioc.html

"值: \(b)"
来源：http://hz.vqdsnc.cn/gtuzmptwrp.html

[T19] Swift：可选绑定
来源：http://hz.tanke756.top/gtheaqzkrt.html

if let n = opt { print(n) }
来源：http://hz.havefunace.top/gtsnkughfk.html

[T20] Swift：数组操作
来源：http://hz.snrcjt.cn/gtxckgksik.html

var a = [1, 2, 3];  a.append(4)
来源：http://hz.chenjidiqi.icu/gtgustfdht.html

[T21] Swift：遍历
来源：http://hz.xziqi.cn/gtddlpklgx.html

for x in a { print(x) }
来源：http://hz.gaohongyu789.top/gtshetmese.html

[T22] Swift：字典
来源：http://hz.quarkkingdee.top/gtthacjvhf.html

var d = ["a": 1];  d["b"] = 2
来源：http://hz.sysykeji.top/gtxjpaqjxc.html

[T23] Swift：函数
来源：http://hz.xingfuxueyuan.xyz/gtnfeudyzk.html

func add(_ a: Int, _ b: Int) -> Int { a + b }
来源：http://hz.jinyuanbaomall.cn/gttjalfbhw.html

[T24] Swift：闭包
来源：http://hz.shanyushiyangtech.top/gtxcsxgknv.html

let f = { (x: Int) -> Int in x * 2 }
来源：http://hz.yangfankeji.com/gtgjrbistp.html

[T25] Swift：结构体
来源：http://hz.fzhhl.top/gtmrqgoqbv.html

struct P { var x: Int }
来源：http://hz.chenzaomai.com/gttigwftkk.html

[T26] Swift：类与重写
来源：http://hz.yongpay.top/gtvqqnovkp.html

class A: Base { override func f() {} }
来源：http://hz.zhiwuduotai.top/gtptuyqpep.html

[T27] Swift：错误处理
来源：http://hz.yonumen.top/gthedzboxt.html

do { try f() } catch { print(error) }
来源：http://hz.jqgufenzy.top/gtxucptozc.html

[T28] Swift：枚举
来源：http://hz.zhaomingkeji.xyz/gtlvupitnq.html

enum Color { case red, green }
来源：http://hz.jqgfzy.top/gtudiwcfvy.html

[T29] Swift：guard 提前返回
来源：http://hz.yuxming.cn/gtbscisxtg.html

guard let x = opt else { return }
来源：http://hz.sufxvd.cn/gtrmyubooc.html

[T30] Swift：协议
来源：http://hz.yongpay.top/gtmyjmdwxi.html

protocol Shape { func area() -> Double }
来源：http://hz.xinyue.icu/gtldsfpdfo.html

[T31] Lua：Hello World
来源：http://hz.tianlin.xyz/gtjvaehpmo.html

print("Hello")
来源：http://hz.jqgufenzy.top/gtbjqildvj.html

[T32] Lua：局部变量
来源：http://hz.jinyuanbaomall.cn/gtrhbgdyry.html

local a = 1
来源：http://hz.wangshuangyany.cn/gtlbngcfbj.html

[T33] Lua：表（数组）
来源：http://hz.havefunace.top/gtrcwssubi.html

local t = {1, 2, 3};  t[4] = 4
来源：http://hz.ywan-chungtsiang.top/gttrajlvee.html

[T34] Lua：遍历表
来源：http://hz.shangyingyoupin.top/gtqdjpaavf.html

for i, v in ipairs(t) do print(i, v) end
来源：http://hz.cucudq.cn/gtvkaangbc.html

[T35] Lua：字典表
来源：http://hz.hammf.cn/gtlkyrvwmd.html

local d = { a = 1 };  d.b = 2
来源：http://hz.birdmap.top/gtzieonwqf.html

[T36] Lua：函数
来源：http://hz.fengsongda.top/gtojyjafsc.html

function add(a, b) return a + b end
来源：http://hz.zhoulong.xyz/gtahtvalec.html

[T37] Lua：字符串拼接
来源：http://hz.yj202588.top/gtfpqbhbym.html

"a" .. "b"
来源：http://hz.yuanzhike.top/gtvwlesgxf.html

[T38] Lua：条件
来源：http://hz.cheryme.top/gtlfulwljc.html

if x > 0 then print("正") end
来源：http://hz.ydjk.org.cn/gtvlfqfwts.html

[T39] Lua：模式匹配
来源：http://hz.bjfxy.top/gtgdvmdchw.html

string.find(s, "%d+")
来源：http://hz.xuanzx.com/gtpjzunzga.html

[T40] Lua：元表
来源：http://hz.52xcode.cn/gttnrajait.html

setmetatable({}, { __index = base })
来源：http://hz.hysaishi.cn/gtjekeopfl.html

[T41] Perl：Hello World
来源：http://hz.daxiang520.top/gtrlsegoco.html

print "Hello\n";
来源：http://hz.sweek.top/gttevsuftp.html

[T42] Perl：变量类型
来源：http://hz.shzxlz.cn/gtfbsfmpxh.html

my $a = 1;  my @arr = (1, 2, 3);  my %h = (a => 1);
来源：http://hz.cucudq.cn/gtsephkrpj.html

[T43] Perl：字符串插值
来源：http://hz.jinghuilouyu.cn/gtdzoeqpya.html

"值: $a"
来源：http://hz.fengsongda.top/gtblopfbas.html

[T44] Perl：条件
来源：http://hz.kuanghao11.cn/gtledqqtfi.html

if ($a > 0) { print "正"; }
来源：http://hz.316326.xyz/gtippaxzha.html

[T45] Perl：数组遍历
来源：http://hz.hysaishi.cn/gtxarojvmv.html

for my $x (@arr) { print $x; }
来源：http://hz.zycfv.cn/gtomvvlqcs.html

[T46] Perl：哈希操作
来源：http://hz.nanxuanxn.top/gtqtuubuce.html

$h{b} = 2;  for my $k (keys %h) { print "$k=$h{$k}"; }
来源：http://hz.jinqigfzy.top/gtylymkzgw.html

[T47] Perl：正则捕获
来源：http://hz.kuanghao11.cn/gtzmnpykfe.html

if ($s =~ /(\d+)/) { print $1; }
来源：http://hz.yanxiufei.cn/gtugaghcol.html

[T48] Perl：正则替换
来源：http://hz.gaohongyu789.top/gtzrzewpuz.html

$s =~ s/old/new/g;
来源：http://hz.jinqigfzy.top/gturnemxpo.html

[T49] Perl：函数
来源：http://hz.tianlin.xyz/gtimivppkv.html

sub add { my ($a, $b) = @_; return $a + $b; }
来源：http://hz.yongpay.top/gtytjzbqba.html

[T50] Perl：逐行读文件
来源：http://hz.wangdashe.top/gtyakrsysj.html

open my $fh, "<", "a.txt" or die $!;
来源：http://hz.shanyushiyangkeji.top/gtmcwbzeoh.html

while (my $line = <$fh>) { print $line; }
来源：http://hz.hysaishi.cn/gtyhuunovh.html

[T51] Scala：Hello World
来源：http://hz.andypj.xyz/gtzcgbyiih.html

println("Hello")
来源：http://hz.ywan-chungtsiang.top/gtzusqnywi.html

[T52] Scala：变量
来源：http://hz.shanyushiyangtech.top/gtlfdnbrhn.html

val a = 1;  var b = 2
来源：http://hz.smart0.xyz/gtnfcxwrgl.html

[T53] Scala：字符串插值
来源：http://hz.yvedp.cn/gtkxcxklbu.html

s"值: $b"
来源：http://hz.jinqigufen.top/gtgzkpuobx.html

[T54] Scala：集合映射
来源：http://hz.shuidangran.top/gtsfbglavq.html

List(1, 2, 3).map(_ * 2)
来源：http://hz.zhengqikj.top/gtefolkhiy.html

[T55] Scala：集合过滤
来源：http://hz.jqgufenzy.top/gtoxxzpmie.html

List(1, 2, 3).filter(_ > 1)
来源：http://hz.sweek.top/gtmvqdkrbl.html

[T56] Scala：样例类
来源：http://hz.pengpengdd.cyou/gtklsiriap.html

case class User(name: String, age: Int)
来源：http://hz.zhixingplan.top/gtfnftzhyq.html

[T57] Scala：模式匹配
来源：http://hz.hywenlv.cn/gtbmoblrga.html

x match { case 1 => "一"; case _ => "其他" }
来源：http://hz.sxryk.cn/gtossxrlnw.html

[T58] Scala：函数定义
来源：http://hz.xylfe.cn/gterqeqtxy.html

def add(a: Int, b: Int): Int = a + b
来源：http://hz.hywenlv.cn/gtckpkxmdk.html

[T59] Scala：循环
来源：http://hz.hnqzz.top/gtplapwleb.html

for (i <- 1 to 10) println(i)
来源：http://hz.chenzaomai.com/gtxrwkgnyb.html

[T60] Scala：折叠
来源：http://hz.jiagoushi.top/gtjjizjerz.html

List(1, 2, 3).foldLeft(0)(_ + _)
来源：http://hz.fzhhl.top/gtgnznomwg.html

================================================================================
来源：http://hz.tian-w.cn/gtkxsuqpqy.html

U. 高频实用片段（Python / PHP / JavaScript 各 40 条）
来源：http://hz.fzhhl.top/gtksuazutj.html

================================================================================
来源：http://hz.chenzaomai.com/gtdgwoqpmo.html

[U01] Py：创建虚拟环境
来源：http://hz.feifeiyinyue.top/gtwokxgpgw.html

python -m venv .venv && source .venv/bin/activate
来源：http://hz.zhaomingkeji.xyz/gtniicmswt.html

[U02] Py：导出 / 安装依赖
来源：http://hz.quarkkingdee.top/gtwlskpmbs.html

pip freeze > requirements.txt;  pip install -r requirements.txt
来源：http://hz.yuanzhike.top/gtvepmtlhm.html

[U03] Py：加载 .env 配置
来源：http://hz.c1oappe.top/gtgbpsmdfl.html

from dotenv import load_dotenv; load_dotenv()
来源：http://hz.316326.xyz/gtedyoebmj.html

[U04] Py：变量调试打印
来源：http://hz.yj20258888.top/gtrwuurkfw.html

print(f"{x=}")            # 输出 x=值，Python 3.8+
来源：http://hz.xziqi.cn/gtjegetqii.html

[U05] Py：列表去重且保序
来源：http://hz.hnxiangtu.top/gtrvxmbjyj.html

list(dict.fromkeys(arr))
来源：http://hz.vqdsnc.cn/gtpbcxtssr.html

[U06] Py：合并两个字典
来源：http://hz.yj20258.top/gtfmohfvue.html

{**a, **b}
来源：http://hz.aizwys.cn/gtwkpyzldx.html

[U07] Py：反转字典键值
来源：http://hz.tianlin.xyz/gthtenwkoj.html

{v: k for k, v in d.items()}
来源：http://hz.hfpthk.cn/gtckramiqn.html

[U08] Py：展平二维列表
来源：http://hz.yuanzhike.top/gteiaieuxd.html

[y for x in nested for y in x]
来源：http://hz.hammf.cn/gtsittxrmw.html

[U09] Py：字典取最大值的键
来源：http://hz.guowangkeji.top/gtuhoasdve.html

max(d, key=d.get)
来源：http://hz.dashuyun.cn/gtpcktdebf.html

[U10] Py：按值排序字典
来源：http://hz.mhx1999.top/gttawwzaho.html

dict(sorted(d.items(), key=lambda kv: kv[1]))
来源：http://hz.shzxlz.cn/gtfudlvrdk.html

[U11] Py：生成器表达式
来源：http://hz.zhixingplan.top/gtakdagrtj.html

(x * 2 for x in arr)
来源：http://hz.yonumen.top/gtytavhtri.html

[U12] Py：取出现最多的 3 个元素
来源：http://hz.guannengcc.top/gtytgdkrbq.html

Counter(arr).most_common(3)
来源：http://hz.xziqi.cn/gtthfxxjrc.html

[U13] Py：固定长度队列
来源：http://hz.sufxvd.cn/gtekrjrweo.html

deque(maxlen=10)
来源：http://hz.iojbl.cn/gtbzhdyvty.html

[U14] Py：分组收集到列表
来源：http://hz.kuanghao11.cn/gtxgkhwjrf.html

defaultdict(list)
来源：http://hz.ppjwa.cn/gtimtudenf.html

[U15] Py：高精度计时
来源：http://hz.cucudq.cn/gtiubwqkah.html

t = time.perf_counter()
来源：http://hz.birdmap.top/gtoxosmvnk.html

[U16] Py：命令行参数解析
来源：http://hz.zhijiandao.cn/gttuybdweb.html

ap = argparse.ArgumentParser();  ap.add_argument("--name");  args = ap.parse_args()
来源：http://hz.cdnleiting.top/gtljwzywbd.html

[U17] Py：初始化日志
来源：http://hz.ivvv.top/gtlnxhcrig.html

logging.basicConfig(level=logging.INFO)
来源：http://hz.redwolf501.top/gteexwnkaf.html

[U18] Py：预编译正则
来源：http://hz.cucudq.cn/gtxzuabdoy.html

pat = re.compile(r"\d+")
来源：http://hz.ppjwa.cn/gtcidkfogz.html

[U19] Py：正则替换带回调
来源：http://hz.zhoulong.xyz/gtvpaoczlq.html

re.sub(r"\d+", lambda m: str(int(m.group()) * 2), s)
来源：http://hz.zhijiandao.cn/gtzjlftjsr.html

[U20] Py：缓存函数结果
来源：http://hz.yongpay.top/gtszhqzuwn.html

@functools.lru_cache(maxsize=None)
来源：http://hz.yuanzhike.top/gtesijrteg.html

[U21] Py：自定义上下文管理器
来源：http://hz.nwbrower.top/gthafnepuk.html

@contextlib.contextmanager
来源：http://hz.wangshuangyany.cn/gtpjroozwc.html

[U22] Py：矩阵转置
来源：http://hz.xingfuxueyuan.xyz/gtbrltzsec.html

list(zip(*m))
来源：http://hz.zhaomingkeji.xyz/gtaipqsoxh.html

[U23] Py：分块读取大文件
来源：http://hz.9152youxi.cn/gtgfiuftkz.html

for chunk in iter(lambda: f.read(8192), b""):
来源：http://hz.cheryme.top/gtihbeebwz.html

[U24] Py：路径操作
来源：http://hz.ybcxt.top/gtwkgjnylp.html

Path("a/b.txt").parent.mkdir(parents=True, exist_ok=True)
来源：http://hz.gaohongyu789.top/gtuqkxwaww.html

[U25] Py：CSV 按字典读
来源：http://hz.birdmap.top/gtteyadqih.html

csv.DictReader(f)
来源：http://hz.mhx1999.top/gtojunbwwn.html

[U26] Py：并发下载
来源：http://hz.gogol.net.cn/gtiilhyaof.html

ThreadPoolExecutor(max_workers=8).map(fetch, urls)
来源：http://hz.kuanghao11.cn/gtxpaxiqwy.html

[U27] Py：异步 HTTP
来源：http://hz.xinyue.icu/gtndvlpoqx.html

aiohttp.ClientSession() 配合 async with
来源：http://hz.jlsjyb.cn/gtiykwxoed.html

[U28] Py：类型别名
来源：http://hz.shanyushiyangkeji.top/gtmumqjlhw.html

UserId = int
来源：http://hz.zhongyouzk.top/gtmmxcneub.html

[U29] Py：属性校验
来源：http://hz.ywan-chungtsiang.top/gtptamhaaq.html

@property 与 @x.setter 配合
来源：http://hz.pengpengdd.cyou/gthzmjwday.html

[U30] Py：数据类
来源：http://hz.pengpengdd.cyou/gtkfsoysqe.html

@dataclass(slots=True)
来源：http://hz.zdqjudy.top/gtcmyvmmmb.html

[U31] Py：单测
来源：http://hz.gotoacloud.top/gtkvmqerey.html

python -m pytest -q
来源：http://hz.jinyuanbaomall.cn/gtihmpezqv.html

[U32] Py：代码格式化
来源：http://hz.tanke756.top/gtamnnyiib.html

ruff format . && ruff check --fix .
来源：http://hz.ppjwa.cn/gtllapsscl.html

[U33] Py：打包发布
来源：http://hz.bjfxy.top/gtuiodqpmv.html

python -m build  （依赖 pyproject.toml）
来源：http://hz.zhijiandao.cn/gtercaxlvp.html

[U34] Py：判断编码
来源：http://hz.shanyushiyangtech.top/gtomcbssua.html

chardet.detect(raw)
来源：http://hz.hywenlv.cn/gtqkwloixu.html

[U35] Py：发送邮件
来源：http://hz.yj20258.top/gtpnbvjymb.html

smtplib.SMTP_SSL(...).send_message(msg)
来源：http://hz.cqqwz.cn/gtfvhzxllw.html

[U36] Py：定时任务
来源：http://hz.jianghu66.top/gtwvtatcrr.html

schedule.every(10).minutes.do(job)
来源：http://hz.gotoacloud.top/gtbrqhxuiv.html

[U37] Py：读写 Excel
来源：http://hz.xziqi.cn/gtgqzlnmrm.html

pandas.read_excel / DataFrame.to_excel
来源：http://hz.aibaodan.cn/gtmanlufmx.html

[U38] Py：获取脚本所在目录
来源：http://hz.gzhubu.top/gtdbbykcdf.html

Path(__file__).resolve().parent
来源：http://hz.havefunace.top/gttoaqhdpk.html

[U39] Py：判断是否在交互环境
来源：http://hz.dashuyun.cn/gtycbnyzfl.html

sys.stdout.isatty()
来源：http://hz.andypj.xyz/gtsrbgrpiu.html

[U40] Py：打印到标准错误
来源：http://hz.xuetiantiany.cn/gtoqqhrqnw.html

print("err", file=sys.stderr)
来源：http://hz.feifeiyinyue.top/gtozzqtfca.html

[U41] PHP：初始化 Composer 项目
来源：http://hz.jinyuanbaomall.cn/gtauvttors.html

composer init;  composer require guzzlehttp/guzzle
来源：http://hz.shanyushiyangtech.top/gtsnxetsaw.html

[U42] PHP：PSR-4 自动加载
来源：http://hz.ehwqpu.com/gtpydkykqp.html

"autoload": { "psr-4": { "App\\": "src/" } }
来源：http://hz.fzhhl.top/gtqlyqwuvk.html

[U43] PHP：声明命名空间
来源：http://hz.cqqwz.cn/gtcwyoutnb.html

namespace App\Http;
来源：http://hz.shuidangran.top/gtqgmboitf.html

[U44] PHP：开启严格类型
来源：http://hz.pengpengdd.cyou/gtqczhlvbp.html

declare(strict_types=1);
来源：http://hz.yangfankeji.com/gtqetjdxef.html

[U45] PHP：类型声明与返回类型
来源：http://hz.zhengqikj.top/gtgiwgexny.html

function add(int $a, int $b): int { return $a + $b; }
来源：http://hz.aizwys.cn/gtrhmbjuwq.html

[U46] PHP：可空类型
来源：http://hz.sysykeji.top/gtsyepcvtk.html

?string $name = null
来源：http://hz.vqdsnc.cn/gtmxrvuipt.html

[U47] PHP：联合类型
来源：http://hz.hysaishi.cn/gtplznzyvi.html

int|string $id
来源：http://hz.hnxiangtu.top/gtyynrkixh.html

[U48] PHP：纯枚举
来源：http://hz.yj20258888.top/gtjfvbsvkr.html

enum Status: string { case Active = "active"; case Off = "off"; }
来源：http://hz.daria6918.cn/gtvnkmnlvn.html

[U49] PHP：只读属性
来源：http://hz.hongshengwenyu.top/gtojtwrsqy.html

public readonly string $name
来源：http://hz.xuanzx.com/gtircbepgi.html

[U50] PHP：构造器属性提升
来源：http://hz.jyoumei.cn/gtlmsegflj.html

public function __construct(private int $id) {}
来源：http://hz.shzxlz.cn/gtnqkastoq.html

[U51] PHP：数组解构
来源：http://hz.aizwys.cn/gtxlwdrqfe.html

[$a, $b] = $arr;
来源：http://hz.sysykeji.top/gtxcweltxl.html

[U52] PHP：箭头函数
来源：http://hz.yongpay.top/gtzchymedi.html

$double = fn($x) => $x * 2;
来源：http://hz.jinqigufen.top/gtrddlkwtm.html

[U53] PHP：空合并运算符
来源：http://hz.jyoumei.cn/gtfmdtcajp.html

$v = $a ?? $b ?? "default";
来源：http://hz.cdnleiting.top/gtifxoxvsm.html

[U54] PHP：空安全调用
来源：http://hz.chenjidiqi.icu/gtfqntwony.html

$obj?->method()
来源：http://hz.hongshengwenyu.top/gttitfmdvn.html

[U55] PHP：match 表达式
来源：http://hz.kuanghao11.cn/gtspyipidh.html

$s = match($x) { 1 => "一", default => "其他" };
来源：http://hz.chenjidiqi.icu/gtelqzyevv.html

[U56] PHP：命名参数
来源：http://hz.jinqigufen.top/gtxwfchsoz.html

f(a: 1, b: 2)
来源：http://hz.zhiwuduotai.top/gtqipoqalf.html

[U57] PHP：字符串插值
来源：http://hz.zhaomingkeji.xyz/gtjfwloykm.html

"值: {$a}"
来源：http://hz.feifeiyinyue.top/gtqftcyvgu.html

[U58] PHP：数组三件套
来源：http://hz.hnxiangtu.top/gtpobgpizu.html

array_map($f, $a);  array_filter($a, $f);  array_reduce($a, $f, 0);
来源：http://hz.zhengqikj.top/gtlgbqonhf.html

[U59] PHP：自定义排序
来源：http://hz.jyoumei.cn/gtdotlntyy.html

usort($arr, fn($a, $b) => $a["age"] <=> $b["age"]);
来源：http://hz.nanxinkj.top/gtqlootzso.html

[U60] PHP：JSON 编解码
来源：http://hz.snrcjt.cn/gtznddpbfk.html

json_encode($d, JSON_UNESCAPED_UNICODE);  json_decode($s, true);
来源：http://hz.tianlin.xyz/gttwjckiug.html

[U61] PHP：正则
来源：http://hz.xinyue.icu/gttvnflrpi.html

preg_match('/(\d+)/', $s, $m);  preg_replace('/\d+/', '#', $s);
来源：http://hz.9152youxi.cn/gtfiskzkew.html

[U62] PHP：日期对象
来源：http://hz.chenjidiqi.icu/gtemtcvtjp.html

(new DateTimeImmutable())->format("Y-m-d");
来源：http://hz.yueranfly.top/gtdzehqalb.html


<!-- 参考信息 -->