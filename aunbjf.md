代发 wailian999

[S37] C++：set
来源：http://hz.gogol.net.cn/gtvkhmyffq.html

std::set<int> s{1, 2, 3};  s.insert(4);
来源：http://hz.jinyuanbaomall.cn/gtkahklrtm.html

[S38] C++：排序
来源：http://hz.zdqjudy.top/gthidpgtso.html

std::sort(v.begin(), v.end());
来源：http://hz.fzhhl.top/gtwokfobzg.html

[S39] C++：自定义比较器排序
来源：http://hz.zdqjudy.top/gtqrqjlrce.html

std::sort(v.begin(), v.end(), [](int a, int b) { return a > b; });
来源：http://hz.jiagoushi.top/gtroyeauuq.html

[S40] C++：查找元素
来源：http://hz.shanyushiyangtech.top/gtvaeaavnn.html

auto it = std::find(v.begin(), v.end(), 3);
来源：http://hz.cqqwz.cn/gtlzyifbtc.html

[S41] C++：类与构造函数
来源：http://hz.ybcxt.top/gtewrewkav.html

class A { public: A(int v) : x_(v) {} int get() const { return x_; } private: int x_; };
来源：http://hz.gaohongyu789.top/gtxjwceeed.html

[S42] C++：继承与虚函数
来源：http://hz.zhaomingkeji.xyz/gtlvupstyo.html

class B : public Base { public: void f() override {} };
来源：http://hz.shanyushiyangkeji.top/gtkzypxcgc.html

[S43] C++：智能指针
来源：http://hz.cheryme.top/gtsjdlmuhh.html

auto p = std::make_unique<int>(5);
来源：http://hz.wangdashe.top/gtvhfazjqa.html

[S44] C++：引用传参
来源：http://hz.gogol.net.cn/gtcykhebzc.html

void inc(int &x) { ++x; }
来源：http://hz.sweek.top/gtyjuloybg.html

[S45] C++：lambda
来源：http://hz.jinqigfzy.top/gtoonpaewa.html

auto add = [](int a, int b) { return a + b; };
来源：http://hz.sxryk.cn/gtkhkxegfr.html

[S46] C++：函数模板
来源：http://hz.c1oappe.top/gthotdqqzq.html

template <typename T> T maxv(T a, T b) { return a > b ? a : b; }
来源：http://hz.yj20258888.top/gtymyrpzdy.html

[S47] C++：结构化绑定遍历
来源：http://hz.cqqwz.cn/gtdmvudlog.html

for (const auto &[k, v] : m) { std::cout << k << v; }
来源：http://hz.xinyue.icu/gtoazkqszq.html

[S48] C++：逐行读文件
来源：http://hz.zhoulong.xyz/gtsdusspcz.html

std::ifstream in("a.txt");  std::string line;
来源：http://hz.tianlin.xyz/gtdrtebqcq.html

while (std::getline(in, line)) { }
来源：http://hz.feifeiyinyue.top/gtgeeixxrf.html

[S49] C++：写文件
来源：http://hz.yvedp.cn/gtmokpurwc.html

std::ofstream out("a.txt");  out << "hi\n";
来源：http://hz.yangfankeji.com/gturdyvply.html

[S50] C++：格式化数字
来源：http://hz.quarkkingdee.top/gtdqbzdlhp.html

std::ostringstream os;  os << std::fixed << std::setprecision(2) << 3.14159;
来源：http://hz.dashuyun.cn/gtmzdcczjb.html

[S51] C++：显式类型转换
来源：http://hz.zhaomingkeji.xyz/gtovtizoyy.html

static_cast<double>(a) / b
来源：http://hz.chenzaomai.com/gtluqnvzth.html

[S52] C++：const 与 noexcept
来源：http://hz.shuidangran.top/gtedsffwbm.html

int size() const noexcept { return n_; }
来源：http://hz.zhiwuduotai.top/gtrobocvvx.html

[S53] C++：移动语义
来源：http://hz.shangyingyoupin.top/gtkwskzwdg.html

std::vector<int> w = std::move(v);
来源：http://hz.dashuyun.cn/gtfbhpzinm.html

[S54] C++：异常处理
来源：http://hz.316326.xyz/gtollmzrni.html

try { throw std::runtime_error("x"); } catch (const std::exception &e) { }
来源：http://hz.yj202588.top/gtmtalfrrc.html

[S55] C++：结构化绑定
来源：http://hz.zhiwuduotai.top/gtakfohwiy.html

auto [a, b] = std::make_pair(1, 2);
来源：http://hz.jyoumei.cn/gthxmcvajb.html

[S56] C++：optional
来源：http://hz.mhx1999.top/gtfxdkwbga.html

std::optional<int> o = 5;  if (o) { int v = *o; }
来源：http://hz.snrcjt.cn/gtxngrivmq.html

[S57] C++：编译期常量
来源：http://hz.jqgufenzy.top/gtbiktxaqm.html

constexpr int N = 10;
来源：http://hz.cheryme.top/gtytesksws.html

[S58] C++：命名空间
来源：http://hz.jqgufenzy.top/gtnjwfuskb.html

namespace ns { int f() { return 1; } }
来源：http://hz.zhengqikj.top/gthzmzeoue.html

[S59] C++：静态断言
来源：http://hz.jiagoushi.top/gtcecdmwtu.html

static_assert(sizeof(int) == 4, "int 必须 4 字节");
来源：http://hz.hfpthk.cn/gtmtpdsubr.html

[S60] C++：遍历并删除元素
来源：http://hz.zhixingplan.top/gtlseagghq.html

v.erase(std::remove_if(v.begin(), v.end(), [](int x) { return x < 0; }), v.end());
来源：http://hz.jqgufenzy.top/gtvjxayedk.html

================================================================================
来源：http://hz.wangshuangyany.cn/gtvkzrridq.html

T. 其他语言补充（Kotlin / Swift / Lua / Perl / Scala）
来源：http://hz.yonumen.top/gtybhjmuio.html

================================================================================
来源：http://hz.yongpay.top/gthfltqryy.html

[T01] Kotlin：Hello World
来源：http://hz.ybcxt.top/gtunnqrjba.html

println("Hello")
来源：http://hz.yj20258.top/gtdzpeolze.html

[T02] Kotlin：变量
来源：http://hz.jianghu66.top/gtzdrnxwfx.html

val a = 1;  var b = 2        // val 只读，var 可变
来源：http://hz.ppjwa.cn/gtvuicxgea.html

[T03] Kotlin：字符串模板
来源：http://hz.jinyuanbaomall.cn/gtglrscutp.html

"值: $b"
来源：http://hz.9152youxi.cn/gtluagbzik.html

[T04] Kotlin：空安全
来源：http://hz.zhixingplan.top/gtczakpzsf.html

val n: String? = null;  n?.length
来源：http://hz.nanxuanxn.top/gtgmsgmtgf.html

[T05] Kotlin：when 表达式
来源：http://hz.hysaishi.cn/gtgndnfhpk.html

val s = when (x) { 1 -> "一" else -> "其他" }   // 多分支时每个分支单独一行
来源：http://hz.zhaomingkeji.xyz/gtqxuerznj.html

[T06] Kotlin：集合映射
来源：http://hz.ybcxt.top/gtbkampppi.html

listOf(1, 2, 3).map { it * 2 }
来源：http://hz.yj20258888.top/gtdmomdaso.html

[T07] Kotlin：集合过滤
来源：http://hz.cheryme.top/gtfefogyyb.html

listOf(1, 2, 3).filter { it > 1 }
来源：http://hz.feifeiyinyue.top/gttksfepej.html

[T08] Kotlin：数据类
来源：http://hz.xziqi.cn/gtqrdoxlrq.html

data class User(val name: String, val age: Int)
来源：http://hz.cheryme.top/gtkplmoaxj.html

[T09] Kotlin：扩展函数
来源：http://hz.xylfe.cn/gtqwndbdmd.html

fun String.exclaim() = this + "!"
来源：http://hz.c1oappe.top/gtpkmbfrso.html

[T10] Kotlin：默认参数
来源：http://hz.aibaodan.cn/gtddsjhfbk.html

fun greet(name: String = "World") = "Hi $name"
来源：http://hz.xylfe.cn/gtulegyecy.html

[T11] Kotlin：协程
来源：http://hz.jqgufenzy.top/gttkyzerxf.html

GlobalScope.launch { delay(1000); println("done") }
来源：http://hz.cqqwz.cn/gtbwwxvtue.html

[T12] Kotlin：解构声明
来源：http://hz.xuetiantiany.cn/gtdaakboll.html

val (a, b) = Pair(1, 2)
来源：http://hz.jinqigfzy.top/gtbmgcbgkl.html

[T13] Kotlin：只读 Map
来源：http://hz.jqgfzy.top/gtmzjlsvlu.html

val m = mapOf("a" to 1)
来源：http://hz.andypj.xyz/gtegrwdpwu.html

[T14] Kotlin：循环
来源：http://hz.zhixingplan.top/gtboggnjjs.html

for (i in 1..10) println(i)
来源：http://hz.hysaishi.cn/gtkgmnsnmn.html

[T15] Kotlin：接口
来源：http://hz.gaohongyu789.top/gthtsddvdt.html

interface Shape { fun area(): Double }
来源：http://hz.jianghu66.top/gthjzxhzcz.html

[T16] Swift：Hello World
来源：http://hz.yonumen.top/gtvteiinxm.html

print("Hello")
来源：http://hz.jiagoushi.top/gtakwzhubx.html

[T17] Swift：变量与常量
来源：http://hz.zhongyouzk.top/gtjqskgagn.html

var a = 1;  let b = 2
来源：http://hz.xylfe.cn/gtmitxqwoz.html

[T18] Swift：字符串插值
来源：http://hz.yanxiufei.cn/gtlpdscqfw.html

"值: \(b)"
来源：http://hz.cheryme.top/gtzluqnrzi.html

[T19] Swift：可选绑定
来源：http://hz.hnxiangtu.top/gtamihxhey.html

if let n = opt { print(n) }
来源：http://hz.ydzc1.top/gtbhkiqicn.html

[T20] Swift：数组操作
来源：http://hz.xuanzx.com/gtammdpjor.html

var a = [1, 2, 3];  a.append(4)
来源：http://hz.jqgufenzy.top/gtlelyblqk.html

[T21] Swift：遍历
来源：http://hz.aibaodan.cn/gtaxljorrk.html

for x in a { print(x) }
来源：http://hz.gzhubu.top/gttzkvaltt.html

[T22] Swift：字典
来源：http://hz.ybcxt.top/gtxdavqqjn.html

var d = ["a": 1];  d["b"] = 2
来源：http://hz.ybcxt.top/gtzufrvhrj.html

[T23] Swift：函数
来源：http://hz.yonumen.top/gtqhlghbqw.html

func add(_ a: Int, _ b: Int) -> Int { a + b }
来源：http://hz.zhongyouzk.top/gtlmfjxwbr.html

[T24] Swift：闭包
来源：http://hz.andypj.xyz/gtmazqdsye.html

let f = { (x: Int) -> Int in x * 2 }
来源：http://hz.nanxinkj.top/gtibjwquxm.html

[T25] Swift：结构体
来源：http://hz.zhixingplan.top/gtxabpsgng.html

struct P { var x: Int }
来源：http://hz.shzxlz.cn/gtkyrwbfnr.html

[T26] Swift：类与重写
来源：http://hz.nanxinkj.top/gtjgowfzvp.html

class A: Base { override func f() {} }
来源：http://hz.feifeiyinyue.top/gtrvhteuyw.html

[T27] Swift：错误处理
来源：http://hz.daxiang520.top/gtufibltdy.html

do { try f() } catch { print(error) }
来源：http://hz.bjfxy.top/gtbchigitk.html

[T28] Swift：枚举
来源：http://hz.jyoumei.cn/gtswwzkvzf.html

enum Color { case red, green }
来源：http://hz.ywan-chungtsiang.top/gtzvzootjn.html

[T29] Swift：guard 提前返回
来源：http://hz.sxryk.cn/gtyfnoudng.html

guard let x = opt else { return }
来源：http://hz.xuetiantiany.cn/gtdlxevtos.html

[T30] Swift：协议
来源：http://hz.jqgufenzy.top/gtjzpwflcy.html

protocol Shape { func area() -> Double }
来源：http://hz.sysykeji.top/gtmwhdsyzx.html

[T31] Lua：Hello World
来源：http://hz.quarkkingdee.top/gttpoddkap.html

print("Hello")
来源：http://hz.jinqigufen.top/gtfjkqlnxw.html

[T32] Lua：局部变量
来源：http://hz.tian-w.cn/gtsmncitlx.html

local a = 1
来源：http://hz.ivvv.top/gtnzbzqnsp.html

[T33] Lua：表（数组）
来源：http://hz.hongshengwenyu.top/gthfhrkdor.html

local t = {1, 2, 3};  t[4] = 4
来源：http://hz.guannengcc.top/gtjmpukkyw.html

[T34] Lua：遍历表
来源：http://hz.cashguo.top/gtqclhbquw.html

for i, v in ipairs(t) do print(i, v) end
来源：http://hz.hnxiangtu.top/gtlficxcqw.html

[T35] Lua：字典表
来源：http://hz.zhaomingkeji.xyz/gtndihefjb.html

local d = { a = 1 };  d.b = 2
来源：http://hz.yj20258888.top/gtlpqrngzp.html

[T36] Lua：函数
来源：http://hz.pengpengdd.cyou/gtsnyugbsl.html

function add(a, b) return a + b end
来源：http://hz.xuanzx.com/gtpqplwamr.html

[T37] Lua：字符串拼接
来源：http://hz.chenzaomai.com/gtzrcyhykd.html

"a" .. "b"
来源：http://hz.mhx1999.top/gtsttbfblu.html

[T38] Lua：条件
来源：http://hz.shanyushiyangtech.top/gtvcpsqbmu.html

if x > 0 then print("正") end
来源：http://hz.gzhubu.top/gtgpyjckfv.html

[T39] Lua：模式匹配
来源：http://hz.vqdsnc.cn/gtzjommogz.html

string.find(s, "%d+")
来源：http://hz.ivvv.top/gtnyoulwsk.html

[T40] Lua：元表
来源：http://hz.shuidangran.top/gtluomgtlr.html

setmetatable({}, { __index = base })
来源：http://hz.wangdashe.top/gtobyetwoy.html

[T41] Perl：Hello World
来源：http://hz.haohaochexian.top/gtwbhhhxoj.html

print "Hello\n";
来源：http://hz.guowangkeji.top/gtzwotemyp.html

[T42] Perl：变量类型
来源：http://hz.yj202588.top/gtoqryokyy.html

my $a = 1;  my @arr = (1, 2, 3);  my %h = (a => 1);
来源：http://hz.hfpthk.cn/gtngdlyxko.html

[T43] Perl：字符串插值
来源：http://hz.zhiwuduotai.top/gtzvewcbcr.html

"值: $a"
来源：http://hz.andypj.xyz/gtllkwzgzd.html

[T44] Perl：条件
来源：http://hz.zhengqikj.top/gtqtgoekxg.html

if ($a > 0) { print "正"; }
来源：http://hz.shuidangran.top/gtjzpunvbq.html

[T45] Perl：数组遍历
来源：http://hz.jiagoushi.top/gtowrkcatj.html

for my $x (@arr) { print $x; }
来源：http://hz.daria6918.cn/gtobzhyrwi.html

[T46] Perl：哈希操作
来源：http://hz.smart0.xyz/gtesychqng.html

$h{b} = 2;  for my $k (keys %h) { print "$k=$h{$k}"; }
来源：http://hz.yueranfly.top/gtxhqufvoo.html

[T47] Perl：正则捕获
来源：http://hz.xuanzx.com/gtmirjicge.html

if ($s =~ /(\d+)/) { print $1; }
来源：http://hz.yuxming.cn/gtwqwiocix.html

[T48] Perl：正则替换
来源：http://hz.yangfankeji.com/gtdbnbjdpt.html

$s =~ s/old/new/g;
来源：http://hz.jyoumei.cn/gtfyfpyacp.html

[T49] Perl：函数
来源：http://hz.hfpthk.cn/gtornyvuaa.html

sub add { my ($a, $b) = @_; return $a + $b; }
来源：http://hz.daria6918.cn/gtufkfdhmq.html

[T50] Perl：逐行读文件
来源：http://hz.shanyushiyangtech.top/gtxipadgfy.html

open my $fh, "<", "a.txt" or die $!;
来源：http://hz.pycfn.com/gtjyuurzbu.html

while (my $line = <$fh>) { print $line; }
来源：http://hz.tanke756.top/gtkwwxkrdf.html

[T51] Scala：Hello World
来源：http://hz.fzhhl.top/gtaxgxayru.html

println("Hello")
来源：http://hz.jinyuanbaomall.cn/gtaxbtened.html

[T52] Scala：变量
来源：http://hz.guowangkeji.top/gtaijduknt.html

val a = 1;  var b = 2
来源：http://hz.ydjk.org.cn/gtddafngoo.html

[T53] Scala：字符串插值
来源：http://hz.zhoulong.xyz/gtxvfrndwh.html

s"值: $b"
来源：http://hz.0kj1m.cn/gtvvstiywx.html

[T54] Scala：集合映射
来源：http://hz.aibaodan.cn/gtudimsgrj.html

List(1, 2, 3).map(_ * 2)
来源：http://hz.yangfankeji.com/gttoqaeram.html

[T55] Scala：集合过滤
来源：http://hz.jinyuanbaomall.cn/gtnbbuidbb.html

List(1, 2, 3).filter(_ > 1)
来源：http://hz.yangfankeji.com/gtjvpmnxos.html

[T56] Scala：样例类
来源：http://hz.jinghuilouyu.cn/gtemgnrubq.html

case class User(name: String, age: Int)
来源：http://hz.fengsongda.top/gtnatqcgeg.html

[T57] Scala：模式匹配
来源：http://hz.zhaomingkeji.xyz/gticzngpkw.html

x match { case 1 => "一"; case _ => "其他" }
来源：http://hz.jianghu66.top/gtxkgcgjnl.html

[T58] Scala：函数定义
来源：http://hz.yj20258888.top/gtuaxeofwo.html

def add(a: Int, b: Int): Int = a + b
来源：http://hz.pycfn.com/gtqdwulcyb.html

[T59] Scala：循环
来源：http://hz.cheryme.top/gtjxkwznio.html

for (i <- 1 to 10) println(i)
来源：http://hz.birdmap.top/gtiqevxybl.html

[T60] Scala：折叠
来源：http://hz.xuanzx.com/gtdmvehtpg.html

List(1, 2, 3).foldLeft(0)(_ + _)
来源：http://hz.xuetiantiany.cn/gtthjhvkvp.html

================================================================================
来源：http://hz.havefunace.top/gtfleohnel.html

U. 高频实用片段（Python / PHP / JavaScript 各 40 条）
来源：http://hz.wangshuangyany.cn/gtmugbwapz.html

================================================================================
来源：http://hz.gotoacloud.top/gtsrnpavue.html

[U01] Py：创建虚拟环境
来源：http://hz.tanke756.top/gthfntngvn.html

python -m venv .venv && source .venv/bin/activate
来源：http://hz.zhixingplan.top/gtkqdvvtfw.html

[U02] Py：导出 / 安装依赖
来源：http://hz.xuetiantiany.cn/gtfippejmg.html

pip freeze > requirements.txt;  pip install -r requirements.txt
来源：http://hz.zhijiandao.cn/gtnrymjtsx.html

[U03] Py：加载 .env 配置
来源：http://hz.pengpengdd.cyou/gtvdydbkrw.html

from dotenv import load_dotenv; load_dotenv()
来源：http://hz.yuanzhike.top/gtasifqvbf.html

[U04] Py：变量调试打印
来源：http://hz.vqdsnc.cn/gtcsxpzkyk.html

print(f"{x=}")            # 输出 x=值，Python 3.8+
来源：http://hz.zhaomingkeji.xyz/gtxsjqbdgc.html

[U05] Py：列表去重且保序
来源：http://hz.guannengcc.top/gtlpvefewz.html

list(dict.fromkeys(arr))
来源：http://hz.sxryk.cn/gtbvpzezhn.html

[U06] Py：合并两个字典
来源：http://hz.sysykeji.top/gtegmyrsnj.html

{**a, **b}
来源：http://hz.gogol.net.cn/gtavmomlsx.html

[U07] Py：反转字典键值
来源：http://hz.snrcjt.cn/gtarvteuyk.html

{v: k for k, v in d.items()}
来源：http://hz.52xcode.cn/gtnmbksngj.html

[U08] Py：展平二维列表
来源：http://hz.ppjwa.cn/gtxtycwfsf.html

[y for x in nested for y in x]
来源：http://hz.birdmap.top/gtgoblfowq.html

[U09] Py：字典取最大值的键
来源：http://hz.zhijiandao.cn/gttxycxexs.html

max(d, key=d.get)
来源：http://hz.zhijiandao.cn/gtuuqrxdtm.html

[U10] Py：按值排序字典
来源：http://hz.sufxvd.cn/gtaxslcwek.html

dict(sorted(d.items(), key=lambda kv: kv[1]))
来源：http://hz.cqqwz.cn/gtpdnsmfqp.html

[U11] Py：生成器表达式
来源：http://hz.meibo888.top/gtdynkjwku.html

(x * 2 for x in arr)
来源：http://hz.zhijiandao.cn/gtmuyobspy.html

[U12] Py：取出现最多的 3 个元素
来源：http://hz.kuanghao11.cn/gttdoliibp.html

Counter(arr).most_common(3)
来源：http://hz.aizwys.cn/gtwkafvgte.html

[U13] Py：固定长度队列
来源：http://hz.smart0.xyz/gtsgczvkgp.html

deque(maxlen=10)
来源：http://hz.fengsongda.top/gtcfymtxjr.html

[U14] Py：分组收集到列表
来源：http://hz.cdnleiting.top/gtzhcfdrph.html

defaultdict(list)
来源：http://hz.yj20258888.top/gtylhchakj.html

[U15] Py：高精度计时
来源：http://hz.wangshuangyany.cn/gtkmqngcfw.html

t = time.perf_counter()
来源：http://hz.ydzc1.top/gtvujmlerp.html

[U16] Py：命令行参数解析
来源：http://hz.hfpthk.cn/gtbcvhbimr.html

ap = argparse.ArgumentParser();  ap.add_argument("--name");  args = ap.parse_args()
来源：http://hz.nanxuanxn.top/gtubdcmcok.html

[U17] Py：初始化日志
来源：http://hz.zhongyouzk.top/gtfseawalf.html

logging.basicConfig(level=logging.INFO)
来源：http://hz.zhaomingkeji.xyz/gteeiscwzr.html

[U18] Py：预编译正则
来源：http://hz.gogol.net.cn/gtltevojrh.html

pat = re.compile(r"\d+")
来源：http://hz.tian-w.cn/gtraqbptcm.html

[U19] Py：正则替换带回调
来源：http://hz.gaohongyu789.top/gtotozxmja.html

re.sub(r"\d+", lambda m: str(int(m.group()) * 2), s)
来源：http://hz.yvedp.cn/gtjbvgelgp.html

[U20] Py：缓存函数结果
来源：http://hz.ydjk.org.cn/gtwpgopefv.html

@functools.lru_cache(maxsize=None)
来源：http://hz.jinqigfzy.top/gtgxqxbleg.html

[U21] Py：自定义上下文管理器
来源：http://hz.chenlongwang.top/gtbfqcmkok.html

@contextlib.contextmanager
来源：http://hz.ehwqpu.com/gtdqlhgdio.html

[U22] Py：矩阵转置
来源：http://hz.chenjidiqi.icu/gterssldfv.html

list(zip(*m))
来源：http://hz.xziqi.cn/gtwwbizbab.html

[U23] Py：分块读取大文件
来源：http://hz.smart0.xyz/gtllsdyksc.html

for chunk in iter(lambda: f.read(8192), b""):
来源：http://hz.shuidangran.top/gtqwvfrltp.html

[U24] Py：路径操作
来源：http://hz.316326.xyz/gtxjpaxzly.html

Path("a/b.txt").parent.mkdir(parents=True, exist_ok=True)
来源：http://hz.guannengcc.top/gtuovrnofh.html

[U25] Py：CSV 按字典读
来源：http://hz.cheryme.top/gtpyqiosad.html

csv.DictReader(f)
来源：http://hz.yonumen.top/gtjnsjcren.html

[U26] Py：并发下载
来源：http://hz.aizwys.cn/gtbnnpclli.html

ThreadPoolExecutor(max_workers=8).map(fetch, urls)
来源：http://hz.cqqwz.cn/gthxsdzltz.html

[U27] Py：异步 HTTP
来源：http://hz.jinghuilouyu.cn/gtyxluutqb.html

aiohttp.ClientSession() 配合 async with
来源：http://hz.hnxiangtu.top/gtyoyafaup.html

[U28] Py：类型别名
来源：http://hz.xziqi.cn/gtzmhqtgsy.html

UserId = int
来源：http://hz.cucudq.cn/gtmgcnzkjn.html

[U29] Py：属性校验
来源：http://hz.gogol.net.cn/gtefvxlqbq.html

@property 与 @x.setter 配合
来源：http://hz.birdmap.top/gtzdgtjbap.html

[U30] Py：数据类
来源：http://hz.feifeiyinyue.top/gtriebzsca.html

@dataclass(slots=True)
来源：http://hz.aizwys.cn/gtkwxchcqr.html

[U31] Py：单测
来源：http://hz.svipenyu.cn/gtqfdahsbr.html

python -m pytest -q
来源：http://hz.yonumen.top/gtshedyoci.html

[U32] Py：代码格式化
来源：http://hz.yonumen.top/gtjqypigyn.html

ruff format . && ruff check --fix .
来源：http://hz.smart0.xyz/gtejsmxzor.html

[U33] Py：打包发布
来源：http://hz.aizwys.cn/gtaqgwlhbu.html

python -m build  （依赖 pyproject.toml）
来源：http://hz.gotoacloud.top/gtqsrkqnwf.html

[U34] Py：判断编码
来源：http://hz.yj20258888.top/gtufrkiwkl.html

chardet.detect(raw)
来源：http://hz.gogol.net.cn/gtqljcvwdw.html

[U35] Py：发送邮件
来源：http://hz.jlsjyb.cn/gtyjjepuhu.html

smtplib.SMTP_SSL(...).send_message(msg)
来源：http://hz.fengsongda.top/gteyyweirh.html

[U36] Py：定时任务
来源：http://hz.kuanghao11.cn/gtfxohdiba.html

schedule.every(10).minutes.do(job)
来源：http://hz.birdmap.top/gtmxtnjlgc.html

[U37] Py：读写 Excel
来源：http://hz.jqgfzy.top/gtqwpjpazm.html

pandas.read_excel / DataFrame.to_excel
来源：http://hz.hammf.cn/gttobxeyns.html

[U38] Py：获取脚本所在目录
来源：http://hz.andypj.xyz/gttakrzuwn.html

Path(__file__).resolve().parent
来源：http://hz.dianchejie.cn/gtmgmthmsr.html

[U39] Py：判断是否在交互环境
来源：http://hz.zhengqikj.top/gtutrzvsij.html

sys.stdout.isatty()
来源：http://hz.xinyue.icu/gtwidpjjys.html

[U40] Py：打印到标准错误
来源：http://hz.smart0.xyz/gtatxdakkx.html

print("err", file=sys.stderr)
来源：http://hz.haohaochexian.top/gterdqpcly.html

[U41] PHP：初始化 Composer 项目
来源：http://hz.xinyue.icu/gtxcoxnzni.html

composer init;  composer require guzzlehttp/guzzle
来源：http://hz.fzhhl.top/gtunbvbbdl.html

[U42] PHP：PSR-4 自动加载
来源：http://hz.cdnleiting.top/gtnpdfevad.html

"autoload": { "psr-4": { "App\\": "src/" } }
来源：http://hz.sufxvd.cn/gtdmtgjphl.html

[U43] PHP：声明命名空间
来源：http://hz.sxryk.cn/gtfgezgyfu.html

namespace App\Http;
来源：http://hz.0kj1m.cn/gtlkzwsjqp.html

[U44] PHP：开启严格类型
来源：http://hz.smart0.xyz/gthpcepqnc.html

declare(strict_types=1);
来源：http://hz.nanxuanxn.top/gtryomgbim.html

[U45] PHP：类型声明与返回类型
来源：http://hz.meibo888.top/gtlqrwgnko.html

function add(int $a, int $b): int { return $a + $b; }
来源：http://hz.9152youxi.cn/gtrauvmagh.html

[U46] PHP：可空类型
来源：http://hz.gogol.net.cn/gtqwotsnki.html

?string $name = null
来源：http://hz.yj202588.top/gtvhohnrbl.html

[U47] PHP：联合类型
来源：http://hz.jlsjyb.cn/gtrenbnmbn.html

int|string $id
来源：http://hz.xuanzx.com/gtnafugbgf.html

[U48] PHP：纯枚举
来源：http://hz.bjfxy.top/gtarldyutx.html

enum Status: string { case Active = "active"; case Off = "off"; }
来源：http://hz.feifeiyinyue.top/gtqitqabfr.html

[U49] PHP：只读属性
来源：http://hz.zhongyouzk.top/gtromybnch.html

public readonly string $name
来源：http://hz.zhixingplan.top/gtuatszuqq.html

[U50] PHP：构造器属性提升
来源：http://hz.zhiwuduotai.top/gtmrvnzkkc.html

public function __construct(private int $id) {}
来源：http://hz.tian-w.cn/gtbvacmlit.html

[U51] PHP：数组解构
来源：http://hz.smart0.xyz/gtrsotultw.html

[$a, $b] = $arr;
来源：http://hz.xuanzx.com/gtagxqsllj.html

[U52] PHP：箭头函数
来源：http://hz.yangfankeji.com/gtxvgzcdsv.html

$double = fn($x) => $x * 2;
来源：http://hz.bjfxy.top/gtnozwhicj.html

[U53] PHP：空合并运算符
来源：http://hz.yj20258.top/gtydsqgbei.html

$v = $a ?? $b ?? "default";
来源：http://hz.zhixingplan.top/gtpylfwpaf.html

[U54] PHP：空安全调用
来源：http://hz.hammf.cn/gtlhojnahx.html

$obj?->method()
来源：http://hz.jinqigfzy.top/gtjsemxgul.html

[U55] PHP：match 表达式
来源：http://hz.zhongyouzk.top/gtkulmpyis.html

$s = match($x) { 1 => "一", default => "其他" };
来源：http://hz.gaohongyu789.top/gtzbauvsvc.html

[U56] PHP：命名参数
来源：http://hz.xuetiantiany.cn/gtjuzxqwss.html

f(a: 1, b: 2)
来源：http://hz.jlsjyb.cn/gtmzvqmnom.html

[U57] PHP：字符串插值
来源：http://hz.yj20258888.top/gttffinmia.html

"值: {$a}"
来源：http://hz.feifeiyinyue.top/gtlumufeal.html

[U58] PHP：数组三件套
来源：http://hz.jinqigfzy.top/gtvxjqutwg.html

array_map($f, $a);  array_filter($a, $f);  array_reduce($a, $f, 0);
来源：http://hz.zhengqikj.top/gtfdyifeid.html

[U59] PHP：自定义排序
来源：http://hz.fzhhl.top/gtguhfveyz.html

usort($arr, fn($a, $b) => $a["age"] <=> $b["age"]);
来源：http://hz.zhiwuduotai.top/gtuvnvbnhq.html

[U60] PHP：JSON 编解码
来源：http://hz.gzhubu.top/gtubschytc.html

json_encode($d, JSON_UNESCAPED_UNICODE);  json_decode($s, true);
来源：http://hz.sweek.top/gtthsazkvn.html

[U61] PHP：正则
来源：http://hz.svipenyu.cn/gtrdecaqpb.html

preg_match('/(\d+)/', $s, $m);  preg_replace('/\d+/', '#', $s);
来源：http://hz.shangyingyoupin.top/gtqfiwwiyo.html

[U62] PHP：日期对象
来源：http://hz.wangdashe.top/gttghsihfg.html

(new DateTimeImmutable())->format("Y-m-d");
来源：http://hz.yj202588.top/gtzkiydcuu.html


<!-- 参考信息 -->