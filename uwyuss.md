代发 wailian999

[S35] C++：map
来源：http://hz.hysaishi.cn/gtoiveyvsd.html

std::map<std::string, int> m;  m["a"] = 1;
来源：http://hz.shanyushiyangkeji.top/gtmutxejtx.html

[S36] C++：unordered_map
来源：http://hz.jinghuilouyu.cn/gtvrqopmhg.html

std::unordered_map<std::string, int> m;  m["a"] = 1;
来源：http://hz.jinghuilouyu.cn/gtxsboqxbf.html

[S37] C++：set
来源：http://hz.pycfn.com/gttfikmfrh.html

std::set<int> s{1, 2, 3};  s.insert(4);
来源：http://hz.yuxming.cn/gtzaooujfl.html

[S38] C++：排序
来源：http://hz.meibo888.top/gtmjawhtvq.html

std::sort(v.begin(), v.end());
来源：http://hz.yanxiufei.cn/gtowvvwwef.html

[S39] C++：自定义比较器排序
来源：http://hz.meibo888.top/gtrwkpgcwb.html

std::sort(v.begin(), v.end(), [](int a, int b) { return a > b; });
来源：http://hz.nanxuanxn.top/gtmljgxdzn.html

[S40] C++：查找元素
来源：http://hz.chenlongwang.top/gtamtojkmj.html

auto it = std::find(v.begin(), v.end(), 3);
来源：http://hz.ppjwa.cn/gtdrmgppvm.html

[S41] C++：类与构造函数
来源：http://hz.shanyushiyangtech.top/gtpvanturf.html

class A { public: A(int v) : x_(v) {} int get() const { return x_; } private: int x_; };
来源：http://hz.aizwys.cn/gtgzbwvvts.html

[S42] C++：继承与虚函数
来源：http://hz.52xcode.cn/gtjlaxrpek.html

class B : public Base { public: void f() override {} };
来源：http://hz.xingfuxueyuan.xyz/gtbksljhli.html

[S43] C++：智能指针
来源：http://hz.redwolf501.top/gtqbkwqcgt.html

auto p = std::make_unique<int>(5);
来源：http://hz.aizwys.cn/gtkekohqbh.html

[S44] C++：引用传参
来源：http://hz.gotoacloud.top/gtlxbnnwvv.html

void inc(int &x) { ++x; }
来源：http://hz.shanyushiyangkeji.top/gtzujqcncs.html

[S45] C++：lambda
来源：http://hz.jinghuilouyu.cn/gtbglokmfy.html

auto add = [](int a, int b) { return a + b; };
来源：http://hz.xuetiantiany.cn/gtjktfgrwl.html

[S46] C++：函数模板
来源：http://hz.jinqigufen.top/gtokztycbq.html

template <typename T> T maxv(T a, T b) { return a > b ? a : b; }
来源：http://hz.ywan-chungtsiang.top/gtfbpadbvu.html

[S47] C++：结构化绑定遍历
来源：http://hz.havefunace.top/gtkzsqikrt.html

for (const auto &[k, v] : m) { std::cout << k << v; }
来源：http://hz.chenzaomai.com/gtvanwilim.html

[S48] C++：逐行读文件
来源：http://hz.bjfxy.top/gtdweqbmvc.html

std::ifstream in("a.txt");  std::string line;
来源：http://hz.yvedp.cn/gtrcaqckwc.html

while (std::getline(in, line)) { }
来源：http://hz.yuanzhike.top/gtnmqwdszl.html

[S49] C++：写文件
来源：http://hz.shanyushiyangtech.top/gtdadcpyfc.html

std::ofstream out("a.txt");  out << "hi\n";
来源：http://hz.chenlongwang.top/gtccpzcnda.html

[S50] C++：格式化数字
来源：http://hz.havefunace.top/gtqdhdkxpu.html

std::ostringstream os;  os << std::fixed << std::setprecision(2) << 3.14159;
来源：http://hz.xuetiantiany.cn/gtpyaeesgg.html

[S51] C++：显式类型转换
来源：http://hz.shuidangran.top/gtqpepmmri.html

static_cast<double>(a) / b
来源：http://hz.mhx1999.top/gtpvglyplk.html

[S52] C++：const 与 noexcept
来源：http://hz.shzxlz.cn/gtqkcmwwjm.html

int size() const noexcept { return n_; }
来源：http://hz.yj20258888.top/gtgnpndrag.html

[S53] C++：移动语义
来源：http://hz.shzxlz.cn/gtaapkgrdv.html

std::vector<int> w = std::move(v);
来源：http://hz.hnqzz.top/gtrkumvllc.html

[S54] C++：异常处理
来源：http://hz.tian-w.cn/gtlkyjapsm.html

try { throw std::runtime_error("x"); } catch (const std::exception &e) { }
来源：http://hz.cdnleiting.top/gtlaygkwjd.html

[S55] C++：结构化绑定
来源：http://hz.cashguo.top/gtacnjuluy.html

auto [a, b] = std::make_pair(1, 2);
来源：http://hz.cheryme.top/gttfjufpna.html

[S56] C++：optional
来源：http://hz.zhaomingkeji.xyz/gtzjatmozl.html

std::optional<int> o = 5;  if (o) { int v = *o; }
来源：http://hz.meibo888.top/gtahytfmpe.html

[S57] C++：编译期常量
来源：http://hz.sysykeji.top/gtwkwzhuft.html

constexpr int N = 10;
来源：http://hz.cqqwz.cn/gtzcvoyoko.html

[S58] C++：命名空间
来源：http://hz.tianlin.xyz/gttktehlew.html

namespace ns { int f() { return 1; } }
来源：http://hz.tian-w.cn/gthgwftnfb.html

[S59] C++：静态断言
来源：http://hz.xuanzx.com/gtoxenayqt.html

static_assert(sizeof(int) == 4, "int 必须 4 字节");
来源：http://hz.gogol.net.cn/gtmxrshfxu.html

[S60] C++：遍历并删除元素
来源：http://hz.jqgfzy.top/gtoqjhzvdd.html

v.erase(std::remove_if(v.begin(), v.end(), [](int x) { return x < 0; }), v.end());
来源：http://hz.c1oappe.top/gtsueasemz.html

================================================================================
来源：http://hz.xinyue.icu/gtlnmaoqwb.html

T. 其他语言补充（Kotlin / Swift / Lua / Perl / Scala）
来源：http://hz.yuxming.cn/gtczpxcael.html

================================================================================
来源：http://hz.redwolf501.top/gtzdthdvza.html

[T01] Kotlin：Hello World
来源：http://hz.yj20258888.top/gtviihqefd.html

println("Hello")
来源：http://hz.kuanghao11.cn/gtdyiqfgum.html

[T02] Kotlin：变量
来源：http://hz.jyoumei.cn/gtobazbiyp.html

val a = 1;  var b = 2        // val 只读，var 可变
来源：http://hz.shzxlz.cn/gtqnmhnzku.html

[T03] Kotlin：字符串模板
来源：http://hz.iojbl.cn/gtzapbzlhz.html

"值: $b"
来源：http://hz.dianchejie.cn/gtpftnjjdk.html

[T04] Kotlin：空安全
来源：http://hz.shzxlz.cn/gthsfziwnb.html

val n: String? = null;  n?.length
来源：http://hz.zhongyouzk.top/gtnsrcnvrk.html

[T05] Kotlin：when 表达式
来源：http://hz.hywenlv.cn/gttjoapitv.html

val s = when (x) { 1 -> "一" else -> "其他" }   // 多分支时每个分支单独一行
来源：http://hz.jinqigfzy.top/gtmwfomqva.html

[T06] Kotlin：集合映射
来源：http://hz.jinqigfzy.top/gtbqojktdf.html

listOf(1, 2, 3).map { it * 2 }
来源：http://hz.jlsjyb.cn/gtpjbqiiik.html

[T07] Kotlin：集合过滤
来源：http://hz.hywenlv.cn/gtvcujvfla.html

listOf(1, 2, 3).filter { it > 1 }
来源：http://hz.cqqwz.cn/gtafrpxogp.html

[T08] Kotlin：数据类
来源：http://hz.guannengcc.top/gtpdxwuzrg.html

data class User(val name: String, val age: Int)
来源：http://hz.guannengcc.top/gtfrsfachr.html

[T09] Kotlin：扩展函数
来源：http://hz.yuanzhike.top/gtvojgagfn.html

fun String.exclaim() = this + "!"
来源：http://hz.hywenlv.cn/gtgzvkbgwk.html

[T10] Kotlin：默认参数
来源：http://hz.ybcxt.top/gttbkgvqzo.html

fun greet(name: String = "World") = "Hi $name"
来源：http://hz.ehwqpu.com/gtbwffytgm.html

[T11] Kotlin：协程
来源：http://hz.pengpengdd.cyou/gtpwooczqm.html

GlobalScope.launch { delay(1000); println("done") }
来源：http://hz.ydjk.org.cn/gtdyiqwxir.html

[T12] Kotlin：解构声明
来源：http://hz.andypj.xyz/gtewwrptlo.html

val (a, b) = Pair(1, 2)
来源：http://hz.havefunace.top/gthtlztddk.html

[T13] Kotlin：只读 Map
来源：http://hz.mhx1999.top/gtnedhruso.html

val m = mapOf("a" to 1)
来源：http://hz.sysykeji.top/gtuckrtcfe.html

[T14] Kotlin：循环
来源：http://hz.cheryme.top/gtggywgodr.html

for (i in 1..10) println(i)
来源：http://hz.redwolf501.top/gthfmijeac.html

[T15] Kotlin：接口
来源：http://hz.fzhhl.top/gtqurdxowf.html

interface Shape { fun area(): Double }
来源：http://hz.bjfxy.top/gttxrhyoco.html

[T16] Swift：Hello World
来源：http://hz.yj202588.top/gtyluzuvod.html

print("Hello")
来源：http://hz.hfpthk.cn/gtlzqjgeny.html

[T17] Swift：变量与常量
来源：http://hz.jqgufenzy.top/gtfptfgdfc.html

var a = 1;  let b = 2
来源：http://hz.sufxvd.cn/gtyvzbjeee.html

[T18] Swift：字符串插值
来源：http://hz.ybcxt.top/gthqewmwnk.html

"值: \(b)"
来源：http://hz.cucudq.cn/gtpcuccldj.html

[T19] Swift：可选绑定
来源：http://hz.yvedp.cn/gtstgpwwrx.html

if let n = opt { print(n) }
来源：http://hz.cheryme.top/gtffnlixan.html

[T20] Swift：数组操作
来源：http://hz.jlsjyb.cn/gtayagkmmc.html

var a = [1, 2, 3];  a.append(4)
来源：http://hz.nanxinkj.top/gtuggjgnau.html

[T21] Swift：遍历
来源：http://hz.zhiwuduotai.top/gtypwsjzcj.html

for x in a { print(x) }
来源：http://hz.redwolf501.top/gtphviagxv.html

[T22] Swift：字典
来源：http://hz.gotoacloud.top/gtnkyyzhmg.html

var d = ["a": 1];  d["b"] = 2
来源：http://hz.snrcjt.cn/gtomwcaxpl.html

[T23] Swift：函数
来源：http://hz.hnqzz.top/gtlotfuxgp.html

func add(_ a: Int, _ b: Int) -> Int { a + b }
来源：http://hz.ydjk.org.cn/gtysdsvvib.html

[T24] Swift：闭包
来源：http://hz.316326.xyz/gtgebzjyxo.html

let f = { (x: Int) -> Int in x * 2 }
来源：http://hz.yongpay.top/gtdqedigie.html

[T25] Swift：结构体
来源：http://hz.jinyuanbaomall.cn/gtekctrztz.html

struct P { var x: Int }
来源：http://hz.chenlongwang.top/gtdenrollz.html

[T26] Swift：类与重写
来源：http://hz.zhaomingkeji.xyz/gtbysqhmzm.html

class A: Base { override func f() {} }
来源：http://hz.yj20258.top/gtblrnhbtk.html

[T27] Swift：错误处理
来源：http://hz.zhixingplan.top/gtmsfmljdj.html

do { try f() } catch { print(error) }
来源：http://hz.hongshengwenyu.top/gtlglybibd.html

[T28] Swift：枚举
来源：http://hz.52xcode.cn/gtpihbgajb.html

enum Color { case red, green }
来源：http://hz.xingfuxueyuan.xyz/gthuhnryna.html

[T29] Swift：guard 提前返回
来源：http://hz.nanxinkj.top/gtbfsrkzhq.html

guard let x = opt else { return }
来源：http://hz.xingfuxueyuan.xyz/gtdyltiups.html

[T30] Swift：协议
来源：http://hz.quarkkingdee.top/gtnorbzuqw.html

protocol Shape { func area() -> Double }
来源：http://hz.dashuyun.cn/gteiuhrwfm.html

[T31] Lua：Hello World
来源：http://hz.ydzc1.top/gtxgaivozy.html

print("Hello")
来源：http://hz.nwbrower.top/gtvayhsffj.html

[T32] Lua：局部变量
来源：http://hz.guowangkeji.top/gtimgrdazd.html

local a = 1
来源：http://hz.zhengqikj.top/gtekziztip.html

[T33] Lua：表（数组）
来源：http://hz.svipenyu.cn/gtspqerdzh.html

local t = {1, 2, 3};  t[4] = 4
来源：http://hz.kuanghao11.cn/gtblgdaqgp.html

[T34] Lua：遍历表
来源：http://hz.zdqjudy.top/gtxktuvtpr.html

for i, v in ipairs(t) do print(i, v) end
来源：http://hz.cucudq.cn/gtocytdozq.html

[T35] Lua：字典表
来源：http://hz.yangfankeji.com/gteuzjfvex.html

local d = { a = 1 };  d.b = 2
来源：http://hz.ywan-chungtsiang.top/gtkvfbxbcr.html

[T36] Lua：函数
来源：http://hz.cdnleiting.top/gtbokifltg.html

function add(a, b) return a + b end
来源：http://hz.cheryme.top/gtkwturjor.html

[T37] Lua：字符串拼接
来源：http://hz.jinqigufen.top/gtwfioafeb.html

"a" .. "b"
来源：http://hz.pycfn.com/gtzusyngpc.html

[T38] Lua：条件
来源：http://hz.redwolf501.top/gtnvwdvuzf.html

if x > 0 then print("正") end
来源：http://hz.zhijiandao.cn/gtvrudviso.html

[T39] Lua：模式匹配
来源：http://hz.yj202588.top/gtwlxvhfmx.html

string.find(s, "%d+")
来源：http://hz.zdqjudy.top/gtfctxrzft.html

[T40] Lua：元表
来源：http://hz.gogol.net.cn/gtcdhgbllg.html

setmetatable({}, { __index = base })
来源：http://hz.cashguo.top/gtkprlrfay.html

[T41] Perl：Hello World
来源：http://hz.ydjk.org.cn/gtvyociapx.html

print "Hello\n";
来源：http://hz.ppjwa.cn/gtgupyzbab.html

[T42] Perl：变量类型
来源：http://hz.shangyingyoupin.top/gtkerdybjk.html

my $a = 1;  my @arr = (1, 2, 3);  my %h = (a => 1);
来源：http://hz.yj20258.top/gtmrbgxdcd.html

[T43] Perl：字符串插值
来源：http://hz.tianlin.xyz/gtnfeiddsq.html

"值: $a"
来源：http://hz.wangdashe.top/gtxnucrlit.html

[T44] Perl：条件
来源：http://hz.ydzc1.top/gtrhofulxf.html

if ($a > 0) { print "正"; }
来源：http://hz.chenlongwang.top/gtlnulyhwj.html

[T45] Perl：数组遍历
来源：http://hz.svipenyu.cn/gtitlnkiip.html

for my $x (@arr) { print $x; }
来源：http://hz.yj20258888.top/gteekwqtfl.html

[T46] Perl：哈希操作
来源：http://hz.xuanzx.com/gtitgywmnm.html

$h{b} = 2;  for my $k (keys %h) { print "$k=$h{$k}"; }
来源：http://hz.jiagoushi.top/gtoksdiugj.html

[T47] Perl：正则捕获
来源：http://hz.ydjk.org.cn/gtxumlnelv.html

if ($s =~ /(\d+)/) { print $1; }
来源：http://hz.sweek.top/gthsustmww.html

[T48] Perl：正则替换
来源：http://hz.xuetiantiany.cn/gtrudxksye.html

$s =~ s/old/new/g;
来源：http://hz.zhaomingkeji.xyz/gtkfupsmvc.html

[T49] Perl：函数
来源：http://hz.chenzaomai.com/gthhlgjczp.html

sub add { my ($a, $b) = @_; return $a + $b; }
来源：http://hz.sysykeji.top/gtcnagtrcd.html

[T50] Perl：逐行读文件
来源：http://hz.zhongyouzk.top/gtjpheptnh.html

open my $fh, "<", "a.txt" or die $!;
来源：http://hz.xuanzx.com/gtxevgfnkd.html

while (my $line = <$fh>) { print $line; }
来源：http://hz.zhijiandao.cn/gtvqkjrxgn.html

[T51] Scala：Hello World
来源：http://hz.zhengqikj.top/gtcmmjapcn.html

println("Hello")
来源：http://hz.shanyushiyangkeji.top/gtzbdyxyti.html

[T52] Scala：变量
来源：http://hz.nanxinkj.top/gtwbdzoibm.html

val a = 1;  var b = 2
来源：http://hz.yanxiufei.cn/gtyjndszbt.html

[T53] Scala：字符串插值
来源：http://hz.c1oappe.top/gtzomnkcgn.html

s"值: $b"
来源：http://hz.hywenlv.cn/gtrpieikyb.html

[T54] Scala：集合映射
来源：http://hz.jyoumei.cn/gtlroehvuq.html

List(1, 2, 3).map(_ * 2)
来源：http://hz.ywan-chungtsiang.top/gtvlwtobyj.html

[T55] Scala：集合过滤
来源：http://hz.jiagoushi.top/gtfmsjcwtw.html

List(1, 2, 3).filter(_ > 1)
来源：http://hz.meibo888.top/gtglhbqlsc.html

[T56] Scala：样例类
来源：http://hz.snrcjt.cn/gtbzuqgkig.html

case class User(name: String, age: Int)
来源：http://hz.ybcxt.top/gtxyicteix.html

[T57] Scala：模式匹配
来源：http://hz.ydjk.org.cn/gtfmvmpger.html

x match { case 1 => "一"; case _ => "其他" }
来源：http://hz.ybcxt.top/gtibrnlqda.html

[T58] Scala：函数定义
来源：http://hz.hnqzz.top/gtuebbumwl.html

def add(a: Int, b: Int): Int = a + b
来源：http://hz.zhiwuduotai.top/gtvjggokwv.html

[T59] Scala：循环
来源：http://hz.cheryme.top/gtzmvcnxkt.html

for (i <- 1 to 10) println(i)
来源：http://hz.jinqigufen.top/gtpuhbqxjv.html

[T60] Scala：折叠
来源：http://hz.wangshuangyany.cn/gtyoaurxsd.html

List(1, 2, 3).foldLeft(0)(_ + _)
来源：http://hz.jinyuanbaomall.cn/gtcyzukniu.html

================================================================================
来源：http://hz.9152youxi.cn/gtyfbscyaj.html

U. 高频实用片段（Python / PHP / JavaScript 各 40 条）
来源：http://hz.aibaodan.cn/gtautdpcwc.html

================================================================================
来源：http://hz.c1oappe.top/gtwmfwmfwr.html

[U01] Py：创建虚拟环境
来源：http://hz.vqdsnc.cn/gtiqnelvin.html

python -m venv .venv && source .venv/bin/activate
来源：http://hz.tanke756.top/gtkqrqyxds.html

[U02] Py：导出 / 安装依赖
来源：http://hz.guannengcc.top/gtbupeytxh.html

pip freeze > requirements.txt;  pip install -r requirements.txt
来源：http://hz.hongshengwenyu.top/gtkeorkxwy.html

[U03] Py：加载 .env 配置
来源：http://hz.gzhubu.top/gtzbmdalhn.html

from dotenv import load_dotenv; load_dotenv()
来源：http://hz.yonumen.top/gtseafuicm.html

[U04] Py：变量调试打印
来源：http://hz.sysykeji.top/gtbeeuclgx.html

print(f"{x=}")            # 输出 x=值，Python 3.8+
来源：http://hz.birdmap.top/gtwofzfxif.html

[U05] Py：列表去重且保序
来源：http://hz.hysaishi.cn/gtftvowcaj.html

list(dict.fromkeys(arr))
来源：http://hz.wangshuangyany.cn/gtepxjqtgu.html

[U06] Py：合并两个字典
来源：http://hz.birdmap.top/gtkqckxdld.html

{**a, **b}
来源：http://hz.jlsjyb.cn/gtxaaeuppb.html

[U07] Py：反转字典键值
来源：http://hz.svipenyu.cn/gtnhlflbdo.html

{v: k for k, v in d.items()}
来源：http://hz.cdnleiting.top/gtzpohmoum.html

[U08] Py：展平二维列表
来源：http://hz.zhixingplan.top/gttxuxayka.html

[y for x in nested for y in x]
来源：http://hz.yanxiufei.cn/gtgrvjfpfl.html

[U09] Py：字典取最大值的键
来源：http://hz.chenzaomai.com/gtvrmjexeg.html

max(d, key=d.get)
来源：http://hz.jinyuanbaomall.cn/gtlcbhqqzb.html

[U10] Py：按值排序字典
来源：http://hz.yangfankeji.com/gtabvetyff.html

dict(sorted(d.items(), key=lambda kv: kv[1]))
来源：http://hz.zhiwuduotai.top/gtrfpiqdir.html

[U11] Py：生成器表达式
来源：http://hz.hfpthk.cn/gtjhlgvsot.html

(x * 2 for x in arr)
来源：http://hz.nwbrower.top/gtvbsmaqkf.html

[U12] Py：取出现最多的 3 个元素
来源：http://hz.havefunace.top/gtzasffaus.html

Counter(arr).most_common(3)
来源：http://hz.xylfe.cn/gthnucyhhr.html

[U13] Py：固定长度队列
来源：http://hz.redwolf501.top/gtkkyttcut.html

deque(maxlen=10)
来源：http://hz.316326.xyz/gticlopwbb.html

[U14] Py：分组收集到列表
来源：http://hz.yongpay.top/gtntxahboc.html

defaultdict(list)
来源：http://hz.bjfxy.top/gtiuhixrkv.html

[U15] Py：高精度计时
来源：http://hz.cashguo.top/gtkmlfbsaj.html

t = time.perf_counter()
来源：http://hz.zhixingplan.top/gttmlqvbii.html

[U16] Py：命令行参数解析
来源：http://hz.tianlin.xyz/gtzpnqpbwr.html

ap = argparse.ArgumentParser();  ap.add_argument("--name");  args = ap.parse_args()
来源：http://hz.tian-w.cn/gtqyjmfzdv.html

[U17] Py：初始化日志
来源：http://hz.fengsongda.top/gttdxqnqnp.html

logging.basicConfig(level=logging.INFO)
来源：http://hz.52xcode.cn/gtegerfzvm.html

[U18] Py：预编译正则
来源：http://hz.zhaomingkeji.xyz/gtylpwikin.html

pat = re.compile(r"\d+")
来源：http://hz.yuanzhike.top/gtjfzykork.html

[U19] Py：正则替换带回调
来源：http://hz.cdnleiting.top/gtzuickwvg.html

re.sub(r"\d+", lambda m: str(int(m.group()) * 2), s)
来源：http://hz.shangyingyoupin.top/gticdbzojk.html

[U20] Py：缓存函数结果
来源：http://hz.jianghu66.top/gtcheifpve.html

@functools.lru_cache(maxsize=None)
来源：http://hz.jyoumei.cn/gtjncwdpte.html

[U21] Py：自定义上下文管理器
来源：http://hz.9152youxi.cn/gtrohxzizq.html

@contextlib.contextmanager
来源：http://hz.zhengqikj.top/gtmzquefbx.html

[U22] Py：矩阵转置
来源：http://hz.sysykeji.top/gtznlkoacl.html

list(zip(*m))
来源：http://hz.zdqjudy.top/gtmotszdgg.html

[U23] Py：分块读取大文件
来源：http://hz.jqgfzy.top/gtcromlexq.html

for chunk in iter(lambda: f.read(8192), b""):
来源：http://hz.chenjidiqi.icu/gtzlpsruja.html

[U24] Py：路径操作
来源：http://hz.tian-w.cn/gtbrtxfrmy.html

Path("a/b.txt").parent.mkdir(parents=True, exist_ok=True)
来源：http://hz.dianchejie.cn/gtoyveygvf.html

[U25] Py：CSV 按字典读
来源：http://hz.feifeiyinyue.top/gtwjslijax.html

csv.DictReader(f)
来源：http://hz.316326.xyz/gtufrswefl.html

[U26] Py：并发下载
来源：http://hz.redwolf501.top/gttoqfyvay.html

ThreadPoolExecutor(max_workers=8).map(fetch, urls)
来源：http://hz.shanyushiyangkeji.top/gtqeglhyon.html

[U27] Py：异步 HTTP
来源：http://hz.xylfe.cn/gthhgolhzd.html

aiohttp.ClientSession() 配合 async with
来源：http://hz.kuanghao11.cn/gtzpfpzznh.html

[U28] Py：类型别名
来源：http://hz.guannengcc.top/gtvfprlhub.html

UserId = int
来源：http://hz.gotoacloud.top/gtqhqpjbhq.html

[U29] Py：属性校验
来源：http://hz.yongpay.top/gttxephxfl.html

@property 与 @x.setter 配合
来源：http://hz.daxiang520.top/gttahpvonl.html

[U30] Py：数据类
来源：http://hz.xingfuxueyuan.xyz/gtwifenpwe.html

@dataclass(slots=True)
来源：http://hz.gaohongyu789.top/gtesnjgrmz.html

[U31] Py：单测
来源：http://hz.yonumen.top/gtqoniabkw.html

python -m pytest -q
来源：http://hz.dashuyun.cn/gtcjgbrnov.html

[U32] Py：代码格式化
来源：http://hz.xuanzx.com/gtqybytwac.html

ruff format . && ruff check --fix .
来源：http://hz.aizwys.cn/gtwucvmbgt.html

[U33] Py：打包发布
来源：http://hz.svipenyu.cn/gtyxhzwmwv.html

python -m build  （依赖 pyproject.toml）
来源：http://hz.shanyushiyangtech.top/gtspstodor.html

[U34] Py：判断编码
来源：http://hz.pycfn.com/gtmwefompz.html

chardet.detect(raw)
来源：http://hz.zhiwuduotai.top/gtjqdbkuhw.html

[U35] Py：发送邮件
来源：http://hz.haohaochexian.top/gtdrzymemj.html

smtplib.SMTP_SSL(...).send_message(msg)
来源：http://hz.guowangkeji.top/gttbgamqte.html

[U36] Py：定时任务
来源：http://hz.shzxlz.cn/gtvcoqivnb.html

schedule.every(10).minutes.do(job)
来源：http://hz.tian-w.cn/gtgdftqcrl.html

[U37] Py：读写 Excel
来源：http://hz.hnqzz.top/gtxixgpeoi.html

pandas.read_excel / DataFrame.to_excel
来源：http://hz.feifeiyinyue.top/gttkowutni.html

[U38] Py：获取脚本所在目录
来源：http://hz.jinqigfzy.top/gtzniyeaxu.html

Path(__file__).resolve().parent
来源：http://hz.mhx1999.top/gtikdgxvar.html

[U39] Py：判断是否在交互环境
来源：http://hz.cqqwz.cn/gthcyyaijk.html

sys.stdout.isatty()
来源：http://hz.jinyuanbaomall.cn/gtbafozird.html

[U40] Py：打印到标准错误
来源：http://hz.gotoacloud.top/gtsmaaqfeh.html

print("err", file=sys.stderr)
来源：http://hz.jqgfzy.top/gtaghcifix.html

[U41] PHP：初始化 Composer 项目
来源：http://hz.52xcode.cn/gttxmomwwd.html

composer init;  composer require guzzlehttp/guzzle
来源：http://hz.zhijiandao.cn/gtybsxjibd.html

[U42] PHP：PSR-4 自动加载
来源：http://hz.yongpay.top/gtsbjjlfcl.html

"autoload": { "psr-4": { "App\\": "src/" } }
来源：http://hz.hammf.cn/gtpbmdnoih.html

[U43] PHP：声明命名空间
来源：http://hz.yanxiufei.cn/gtmjmjsgee.html

namespace App\Http;
来源：http://hz.chenzaomai.com/gtncvasfma.html

[U44] PHP：开启严格类型
来源：http://hz.0kj1m.cn/gtodqioxap.html

declare(strict_types=1);
来源：http://hz.haohaochexian.top/gtirhrjdge.html

[U45] PHP：类型声明与返回类型
来源：http://hz.iojbl.cn/gtllexkhpa.html

function add(int $a, int $b): int { return $a + $b; }
来源：http://hz.redwolf501.top/gtwhkaibgn.html

[U46] PHP：可空类型
来源：http://hz.gogol.net.cn/gtltaeufsh.html

?string $name = null
来源：http://hz.gogol.net.cn/gtjzvdylmw.html

[U47] PHP：联合类型
来源：http://hz.ybcxt.top/gtwoqzpdbz.html

int|string $id
来源：http://hz.jinqigfzy.top/gtplmsvclg.html

[U48] PHP：纯枚举
来源：http://hz.ydzc1.top/gtrfxcppiy.html

enum Status: string { case Active = "active"; case Off = "off"; }
来源：http://hz.kuanghao11.cn/gtcwftqlpb.html

[U49] PHP：只读属性
来源：http://hz.ydzc1.top/gtiqxnqflo.html

public readonly string $name
来源：http://hz.feifeiyinyue.top/gtdhtpqkri.html

[U50] PHP：构造器属性提升
来源：http://hz.meibo888.top/gtjrlxcnif.html

public function __construct(private int $id) {}
来源：http://hz.gotoacloud.top/gtahuadvkn.html

[U51] PHP：数组解构
来源：http://hz.gzhubu.top/gtzcymmvlh.html

[$a, $b] = $arr;
来源：http://hz.yueranfly.top/gtuwwsercv.html

[U52] PHP：箭头函数
来源：http://hz.snrcjt.cn/gtesrdpept.html

$double = fn($x) => $x * 2;
来源：http://hz.mhx1999.top/gtpjuiplcw.html

[U53] PHP：空合并运算符
来源：http://hz.daxiang520.top/gtsmmizhuj.html

$v = $a ?? $b ?? "default";
来源：http://hz.zhiwuduotai.top/gtyygqybyq.html

[U54] PHP：空安全调用
来源：http://hz.nanxinkj.top/gtjfkrdaii.html

$obj?->method()
来源：http://hz.sysykeji.top/gtthhrwgog.html

[U55] PHP：match 表达式
来源：http://hz.zhaomingkeji.xyz/gteyftfkni.html

$s = match($x) { 1 => "一", default => "其他" };
来源：http://hz.shzxlz.cn/gtkkaojggo.html

[U56] PHP：命名参数
来源：http://hz.jiagoushi.top/gtuotyxllo.html

f(a: 1, b: 2)
来源：http://hz.c1oappe.top/gtvsfqxrya.html

[U57] PHP：字符串插值
来源：http://hz.gzhubu.top/gtjntywggv.html

"值: {$a}"
来源：http://hz.meibo888.top/gtenrrzjox.html

[U58] PHP：数组三件套
来源：http://hz.nanxuanxn.top/gtwjjjkqws.html

array_map($f, $a);  array_filter($a, $f);  array_reduce($a, $f, 0);
来源：http://hz.sysykeji.top/gtczjnshqm.html

[U59] PHP：自定义排序
来源：http://hz.ydjk.org.cn/gtyudprrkj.html

usort($arr, fn($a, $b) => $a["age"] <=> $b["age"]);
来源：http://hz.zhiwuduotai.top/gtvutklhzp.html

[U60] PHP：JSON 编解码
来源：http://hz.yueranfly.top/gtjctgextc.html

json_encode($d, JSON_UNESCAPED_UNICODE);  json_decode($s, true);
来源：http://hz.0kj1m.cn/gtadilcxoa.html


<!-- 参考信息 -->