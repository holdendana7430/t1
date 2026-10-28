代发 wailian999

[S35] C++：map
来源：http://hz.cqqwz.cn/gtxkmaqhtt.html

std::map<std::string, int> m;  m["a"] = 1;
来源：http://hz.ybcxt.top/gtgsaxwseg.html

[S36] C++：unordered_map
来源：http://hz.nanxuanxn.top/gtssabteyz.html

std::unordered_map<std::string, int> m;  m["a"] = 1;
来源：http://hz.yj202588.top/gtepweblyo.html

[S37] C++：set
来源：http://hz.chenlongwang.top/gtrnwzuykr.html

std::set<int> s{1, 2, 3};  s.insert(4);
来源：http://hz.xziqi.cn/gtwulvadtr.html

[S38] C++：排序
来源：http://hz.yueranfly.top/gtaavulmvn.html

std::sort(v.begin(), v.end());
来源：http://hz.wangdashe.top/gtjijpxyul.html

[S39] C++：自定义比较器排序
来源：http://hz.guannengcc.top/gtdtswkqzs.html

std::sort(v.begin(), v.end(), [](int a, int b) { return a > b; });
来源：http://hz.hammf.cn/gtyhumxjeg.html

[S40] C++：查找元素
来源：http://hz.sweek.top/gtqonfrtyo.html

auto it = std::find(v.begin(), v.end(), 3);
来源：http://hz.smart0.xyz/gtvtduijaa.html

[S41] C++：类与构造函数
来源：http://hz.sufxvd.cn/gttfojjolu.html

class A { public: A(int v) : x_(v) {} int get() const { return x_; } private: int x_; };
来源：http://hz.yj202588.top/gtpdkwudrr.html

[S42] C++：继承与虚函数
来源：http://hz.yuanzhike.top/gtaofgycej.html

class B : public Base { public: void f() override {} };
来源：http://hz.smart0.xyz/gtpcqjyjdq.html

[S43] C++：智能指针
来源：http://hz.xziqi.cn/gtietwbslq.html

auto p = std::make_unique<int>(5);
来源：http://hz.meibo888.top/gtptsucllh.html

[S44] C++：引用传参
来源：http://hz.xuanzx.com/gtexbhvxnq.html

void inc(int &x) { ++x; }
来源：http://hz.52xcode.cn/gtpjecvipb.html

[S45] C++：lambda
来源：http://hz.tianlin.xyz/gtnsqhqybk.html

auto add = [](int a, int b) { return a + b; };
来源：http://hz.jinyuanbaomall.cn/gtlebljtmt.html

[S46] C++：函数模板
来源：http://hz.gaohongyu789.top/gtgoaghvqb.html

template <typename T> T maxv(T a, T b) { return a > b ? a : b; }
来源：http://hz.shanyushiyangtech.top/gtenfqifxj.html

[S47] C++：结构化绑定遍历
来源：http://hz.guannengcc.top/gtgbfunisf.html

for (const auto &[k, v] : m) { std::cout << k << v; }
来源：http://hz.cashguo.top/gthkfaybww.html

[S48] C++：逐行读文件
来源：http://hz.jinghuilouyu.cn/gthdvkwplx.html

std::ifstream in("a.txt");  std::string line;
来源：http://hz.hfpthk.cn/gtfnjqumou.html

while (std::getline(in, line)) { }
来源：http://hz.gotoacloud.top/gtvvtxfwyb.html

[S49] C++：写文件
来源：http://hz.sxryk.cn/gtraccnwvx.html

std::ofstream out("a.txt");  out << "hi\n";
来源：http://hz.yvedp.cn/gtdnxtkuod.html

[S50] C++：格式化数字
来源：http://hz.iojbl.cn/gtvqesrwez.html

std::ostringstream os;  os << std::fixed << std::setprecision(2) << 3.14159;
来源：http://hz.shzxlz.cn/gtugzfooeb.html

[S51] C++：显式类型转换
来源：http://hz.ehwqpu.com/gtwosbyrnk.html

static_cast<double>(a) / b
来源：http://hz.nwbrower.top/gtfbqqpmzu.html

[S52] C++：const 与 noexcept
来源：http://hz.9152youxi.cn/gtvqvbzoim.html

int size() const noexcept { return n_; }
来源：http://hz.pengpengdd.cyou/gtaipdkydl.html

[S53] C++：移动语义
来源：http://hz.andypj.xyz/gthuqismud.html

std::vector<int> w = std::move(v);
来源：http://hz.yuxming.cn/gtfepuqrfy.html

[S54] C++：异常处理
来源：http://hz.guowangkeji.top/gtalxxwncd.html

try { throw std::runtime_error("x"); } catch (const std::exception &e) { }
来源：http://hz.zhiwuduotai.top/gtajdlfade.html

[S55] C++：结构化绑定
来源：http://hz.hnqzz.top/gtorpsawyd.html

auto [a, b] = std::make_pair(1, 2);
来源：http://hz.yueranfly.top/gtbzldegvj.html

[S56] C++：optional
来源：http://hz.yvedp.cn/gtgfbxmtsz.html

std::optional<int> o = 5;  if (o) { int v = *o; }
来源：http://hz.gzhubu.top/gtofzcfhpa.html

[S57] C++：编译期常量
来源：http://hz.xuanzx.com/gtadsxmepq.html

constexpr int N = 10;
来源：http://hz.jinqigufen.top/gtfmkbkurt.html

[S58] C++：命名空间
来源：http://hz.jinqigfzy.top/gtfqlhsjgc.html

namespace ns { int f() { return 1; } }
来源：http://hz.zhongyouzk.top/gtbvwnymls.html

[S59] C++：静态断言
来源：http://hz.wangshuangyany.cn/gtgiwxvatf.html

static_assert(sizeof(int) == 4, "int 必须 4 字节");
来源：http://hz.jianghu66.top/gtwyeomnvj.html

[S60] C++：遍历并删除元素
来源：http://hz.havefunace.top/gthrkeqmos.html

v.erase(std::remove_if(v.begin(), v.end(), [](int x) { return x < 0; }), v.end());
来源：http://hz.zhiwuduotai.top/gtnhnhpfnx.html

================================================================================
来源：http://hz.zhoulong.xyz/gtcebczdrk.html

T. 其他语言补充（Kotlin / Swift / Lua / Perl / Scala）
来源：http://hz.snrcjt.cn/gtbmsvadyj.html

================================================================================
来源：http://hz.jyoumei.cn/gtkvovhjou.html

[T01] Kotlin：Hello World
来源：http://hz.yanxiufei.cn/gtjzyamwpv.html

println("Hello")
来源：http://hz.guowangkeji.top/gtomrmovub.html

[T02] Kotlin：变量
来源：http://hz.chenlongwang.top/gtgckclhty.html

val a = 1;  var b = 2        // val 只读，var 可变
来源：http://hz.zhoulong.xyz/gtftsnwjcj.html

[T03] Kotlin：字符串模板
来源：http://hz.chenlongwang.top/gtdtthlepr.html

"值: $b"
来源：http://hz.0kj1m.cn/gturzvgyfg.html

[T04] Kotlin：空安全
来源：http://hz.dianchejie.cn/gtlyhdpuab.html

val n: String? = null;  n?.length
来源：http://hz.hnqzz.top/gtllrtwzrp.html

[T05] Kotlin：when 表达式
来源：http://hz.jinqigfzy.top/gtflvkhoxt.html

val s = when (x) { 1 -> "一" else -> "其他" }   // 多分支时每个分支单独一行
来源：http://hz.hongshengwenyu.top/gtupuktrqa.html

[T06] Kotlin：集合映射
来源：http://hz.fzhhl.top/gtuhzztbtm.html

listOf(1, 2, 3).map { it * 2 }
来源：http://hz.jinqigufen.top/gtqvrocqyk.html

[T07] Kotlin：集合过滤
来源：http://hz.redwolf501.top/gteuvpfszg.html

listOf(1, 2, 3).filter { it > 1 }
来源：http://hz.sufxvd.cn/gtiipbrmcv.html

[T08] Kotlin：数据类
来源：http://hz.aibaodan.cn/gtggbwqtlo.html

data class User(val name: String, val age: Int)
来源：http://hz.tian-w.cn/gttrkdrxwv.html

[T09] Kotlin：扩展函数
来源：http://hz.tianlin.xyz/gtyjydstik.html

fun String.exclaim() = this + "!"
来源：http://hz.havefunace.top/gtjixkntww.html

[T10] Kotlin：默认参数
来源：http://hz.snrcjt.cn/gtqepleacm.html

fun greet(name: String = "World") = "Hi $name"
来源：http://hz.316326.xyz/gtpfejawze.html

[T11] Kotlin：协程
来源：http://hz.9152youxi.cn/gtlmcittsc.html

GlobalScope.launch { delay(1000); println("done") }
来源：http://hz.zhoulong.xyz/gtswqkdgps.html

[T12] Kotlin：解构声明
来源：http://hz.hnqzz.top/gtfbtexowu.html

val (a, b) = Pair(1, 2)
来源：http://hz.yvedp.cn/gtobeipshg.html

[T13] Kotlin：只读 Map
来源：http://hz.kuanghao11.cn/gtbsewmoti.html

val m = mapOf("a" to 1)
来源：http://hz.mhx1999.top/gtmgiohywr.html

[T14] Kotlin：循环
来源：http://hz.smart0.xyz/gtwzfgsxko.html

for (i in 1..10) println(i)
来源：http://hz.hfpthk.cn/gttjbcwauw.html

[T15] Kotlin：接口
来源：http://hz.chenzaomai.com/gtxjtgzwhy.html

interface Shape { fun area(): Double }
来源：http://hz.jinqigufen.top/gtelpkxlch.html

[T16] Swift：Hello World
来源：http://hz.jiagoushi.top/gtqrfburjc.html

print("Hello")
来源：http://hz.jqgfzy.top/gtiysqteyo.html

[T17] Swift：变量与常量
来源：http://hz.yonumen.top/gtktatsxsv.html

var a = 1;  let b = 2
来源：http://hz.jqgfzy.top/gtjgdepulc.html

[T18] Swift：字符串插值
来源：http://hz.smart0.xyz/gtavynmbxq.html

"值: \(b)"
来源：http://hz.birdmap.top/gtuxishyjc.html

[T19] Swift：可选绑定
来源：http://hz.andypj.xyz/gtvhfrmtlc.html

if let n = opt { print(n) }
来源：http://hz.yanxiufei.cn/gtleyjofbe.html

[T20] Swift：数组操作
来源：http://hz.pengpengdd.cyou/gtspxsctgw.html

var a = [1, 2, 3];  a.append(4)
来源：http://hz.pycfn.com/gtolocksvk.html

[T21] Swift：遍历
来源：http://hz.daria6918.cn/gtrjwtemee.html

for x in a { print(x) }
来源：http://hz.zhengqikj.top/gtgzerzkpk.html

[T22] Swift：字典
来源：http://hz.andypj.xyz/gtdxdfvrid.html

var d = ["a": 1];  d["b"] = 2
来源：http://hz.birdmap.top/gtmbpphsyb.html

[T23] Swift：函数
来源：http://hz.yvedp.cn/gtkspjkppp.html

func add(_ a: Int, _ b: Int) -> Int { a + b }
来源：http://hz.yangfankeji.com/gtdcrpzmmp.html

[T24] Swift：闭包
来源：http://hz.zhoulong.xyz/gtcpzzuwpd.html

let f = { (x: Int) -> Int in x * 2 }
来源：http://hz.redwolf501.top/gtwpleuzag.html

[T25] Swift：结构体
来源：http://hz.fzhhl.top/gtzqvsiszb.html

struct P { var x: Int }
来源：http://hz.tian-w.cn/gtpvuutnvl.html

[T26] Swift：类与重写
来源：http://hz.zhiwuduotai.top/gtyixfywgm.html

class A: Base { override func f() {} }
来源：http://hz.cheryme.top/gtwjlcrlci.html

[T27] Swift：错误处理
来源：http://hz.ivvv.top/gtmtfgcxai.html

do { try f() } catch { print(error) }
来源：http://hz.vqdsnc.cn/gtxflcvxzl.html

[T28] Swift：枚举
来源：http://hz.fengsongda.top/gtktbyzbzi.html

enum Color { case red, green }
来源：http://hz.pycfn.com/gtukzaxqas.html

[T29] Swift：guard 提前返回
来源：http://hz.jyoumei.cn/gtkcbddolo.html

guard let x = opt else { return }
来源：http://hz.zhijiandao.cn/gtdthgsmta.html

[T30] Swift：协议
来源：http://hz.jlsjyb.cn/gtprmbzdbt.html

protocol Shape { func area() -> Double }
来源：http://hz.hysaishi.cn/gtkyvtqdsv.html

[T31] Lua：Hello World
来源：http://hz.jinghuilouyu.cn/gteeyzkjib.html

print("Hello")
来源：http://hz.shuidangran.top/gtforyheqg.html

[T32] Lua：局部变量
来源：http://hz.yvedp.cn/gtsqzqitmj.html

local a = 1
来源：http://hz.gaohongyu789.top/gtrrengdon.html

[T33] Lua：表（数组）
来源：http://hz.bjfxy.top/gtrgpvckmz.html

local t = {1, 2, 3};  t[4] = 4
来源：http://hz.yj20258.top/gtvlcvdfpr.html

[T34] Lua：遍历表
来源：http://hz.ydjk.org.cn/gtlhwdoftb.html

for i, v in ipairs(t) do print(i, v) end
来源：http://hz.fengsongda.top/gtfdhsnihs.html

[T35] Lua：字典表
来源：http://hz.dianchejie.cn/gtopxqnwdf.html

local d = { a = 1 };  d.b = 2
来源：http://hz.pengpengdd.cyou/gtpntdhpam.html

[T36] Lua：函数
来源：http://hz.sxryk.cn/gtiamstuzp.html

function add(a, b) return a + b end
来源：http://hz.yueranfly.top/gtamkbryfi.html

[T37] Lua：字符串拼接
来源：http://hz.andypj.xyz/gtvayxnbuy.html

"a" .. "b"
来源：http://hz.zhiwuduotai.top/gtlbagsjli.html

[T38] Lua：条件
来源：http://hz.havefunace.top/gtqfltrpme.html

if x > 0 then print("正") end
来源：http://hz.shuidangran.top/gtrwouhzry.html

[T39] Lua：模式匹配
来源：http://hz.cheryme.top/gtyjqgjuhg.html

string.find(s, "%d+")
来源：http://hz.hongshengwenyu.top/gtcgqihiop.html

[T40] Lua：元表
来源：http://hz.hammf.cn/gtggxqitgk.html

setmetatable({}, { __index = base })
来源：http://hz.zhengqikj.top/gtufxgctcz.html

[T41] Perl：Hello World
来源：http://hz.haohaochexian.top/gtfmgjigll.html

print "Hello\n";
来源：http://hz.feifeiyinyue.top/gtvjaywdnu.html

[T42] Perl：变量类型
来源：http://hz.chenlongwang.top/gtjmazujpu.html

my $a = 1;  my @arr = (1, 2, 3);  my %h = (a => 1);
来源：http://hz.jiagoushi.top/gtdiyqrunu.html

[T43] Perl：字符串插值
来源：http://hz.zdqjudy.top/gtdqyvnpqd.html

"值: $a"
来源：http://hz.gaohongyu789.top/gtfchzbjfj.html

[T44] Perl：条件
来源：http://hz.gogol.net.cn/gtollbgyht.html

if ($a > 0) { print "正"; }
来源：http://hz.jianghu66.top/gtktnjmcqf.html

[T45] Perl：数组遍历
来源：http://hz.pycfn.com/gtktfdjyta.html

for my $x (@arr) { print $x; }
来源：http://hz.jqgufenzy.top/gtaitcqojx.html

[T46] Perl：哈希操作
来源：http://hz.yj202588.top/gtcrnbhjyh.html

$h{b} = 2;  for my $k (keys %h) { print "$k=$h{$k}"; }
来源：http://hz.guannengcc.top/gtmrxwihrn.html

[T47] Perl：正则捕获
来源：http://hz.yueranfly.top/gtpcjxdzzn.html

if ($s =~ /(\d+)/) { print $1; }
来源：http://hz.zhijiandao.cn/gtqhxcsfit.html

[T48] Perl：正则替换
来源：http://hz.hywenlv.cn/gtqimsgnuq.html

$s =~ s/old/new/g;
来源：http://hz.316326.xyz/gttceztcra.html

[T49] Perl：函数
来源：http://hz.feifeiyinyue.top/gtopvuyxdv.html

sub add { my ($a, $b) = @_; return $a + $b; }
来源：http://hz.vqdsnc.cn/gtofstkata.html

[T50] Perl：逐行读文件
来源：http://hz.yonumen.top/gtcundjitx.html

open my $fh, "<", "a.txt" or die $!;
来源：http://hz.wangshuangyany.cn/gtognuwqcl.html

while (my $line = <$fh>) { print $line; }
来源：http://hz.gogol.net.cn/gtueutbdlj.html

[T51] Scala：Hello World
来源：http://hz.gaohongyu789.top/gtjifmjrec.html

println("Hello")
来源：http://hz.ywan-chungtsiang.top/gtbqseidjb.html

[T52] Scala：变量
来源：http://hz.mhx1999.top/gtlbqgsxjh.html

val a = 1;  var b = 2
来源：http://hz.cashguo.top/gtldalsewk.html

[T53] Scala：字符串插值
来源：http://hz.yongpay.top/gtdcxgfypi.html

s"值: $b"
来源：http://hz.shuidangran.top/gtbwdtulwd.html

[T54] Scala：集合映射
来源：http://hz.svipenyu.cn/gtdoxiphoq.html

List(1, 2, 3).map(_ * 2)
来源：http://hz.dianchejie.cn/gtdtqymiye.html

[T55] Scala：集合过滤
来源：http://hz.mhx1999.top/gtpktnazxl.html

List(1, 2, 3).filter(_ > 1)
来源：http://hz.cdnleiting.top/gtopgvuqei.html

[T56] Scala：样例类
来源：http://hz.jlsjyb.cn/gtipgvfbpg.html

case class User(name: String, age: Int)
来源：http://hz.jlsjyb.cn/gtihdrypni.html

[T57] Scala：模式匹配
来源：http://hz.dashuyun.cn/gtowftlonp.html

x match { case 1 => "一"; case _ => "其他" }
来源：http://hz.iojbl.cn/gtxyyvlxxc.html

[T58] Scala：函数定义
来源：http://hz.hongshengwenyu.top/gtzbumjgjp.html

def add(a: Int, b: Int): Int = a + b
来源：http://hz.guowangkeji.top/gtrzvbteug.html

[T59] Scala：循环
来源：http://hz.zhengqikj.top/gtuvwdliyi.html

for (i <- 1 to 10) println(i)
来源：http://hz.9152youxi.cn/gtqgkdaprt.html

[T60] Scala：折叠
来源：http://hz.andypj.xyz/gtzjnmyvwl.html

List(1, 2, 3).foldLeft(0)(_ + _)
来源：http://hz.svipenyu.cn/gtfxhqboxi.html

================================================================================
来源：http://hz.daria6918.cn/gtxnlpvrfp.html

U. 高频实用片段（Python / PHP / JavaScript 各 40 条）
来源：http://hz.kuanghao11.cn/gtqbbdmdfl.html

================================================================================
来源：http://hz.pengpengdd.cyou/gtjjckutps.html

[U01] Py：创建虚拟环境
来源：http://hz.ivvv.top/gtwfsfkoqh.html

python -m venv .venv && source .venv/bin/activate
来源：http://hz.hammf.cn/gtvtzjwjxj.html

[U02] Py：导出 / 安装依赖
来源：http://hz.zdqjudy.top/gtfyxeftcd.html

pip freeze > requirements.txt;  pip install -r requirements.txt
来源：http://hz.jinqigufen.top/gtpldgbbuz.html

[U03] Py：加载 .env 配置
来源：http://hz.shzxlz.cn/gtufvblhof.html

from dotenv import load_dotenv; load_dotenv()
来源：http://hz.c1oappe.top/gtjtkczyrb.html

[U04] Py：变量调试打印
来源：http://hz.xingfuxueyuan.xyz/gtukihznin.html

print(f"{x=}")            # 输出 x=值，Python 3.8+
来源：http://hz.dashuyun.cn/gtcghzxdne.html

[U05] Py：列表去重且保序
来源：http://hz.cdnleiting.top/gtofupojvm.html

list(dict.fromkeys(arr))
来源：http://hz.aibaodan.cn/gtbketimtx.html

[U06] Py：合并两个字典
来源：http://hz.tanke756.top/gtxmiezmem.html

{**a, **b}
来源：http://hz.tianlin.xyz/gtpsqhvrlp.html

[U07] Py：反转字典键值
来源：http://hz.zhengqikj.top/gtbrbndjhf.html

{v: k for k, v in d.items()}
来源：http://hz.cheryme.top/gtiuapflix.html

[U08] Py：展平二维列表
来源：http://hz.jqgfzy.top/gtmgggngat.html

[y for x in nested for y in x]
来源：http://hz.wangshuangyany.cn/gtwjggjbts.html

[U09] Py：字典取最大值的键
来源：http://hz.wangdashe.top/gttujpizdd.html

max(d, key=d.get)
来源：http://hz.andypj.xyz/gthdjydkvh.html

[U10] Py：按值排序字典
来源：http://hz.hnxiangtu.top/gtmchomeec.html

dict(sorted(d.items(), key=lambda kv: kv[1]))
来源：http://hz.ppjwa.cn/gtgtyrulpw.html

[U11] Py：生成器表达式
来源：http://hz.9152youxi.cn/gtkfzxqtrq.html

(x * 2 for x in arr)
来源：http://hz.zhaomingkeji.xyz/gtdvertowz.html

[U12] Py：取出现最多的 3 个元素
来源：http://hz.wangshuangyany.cn/gtujomuigg.html

Counter(arr).most_common(3)
来源：http://hz.sweek.top/gthalcoduc.html

[U13] Py：固定长度队列
来源：http://hz.chenlongwang.top/gttmajcuca.html

deque(maxlen=10)
来源：http://hz.feifeiyinyue.top/gtyuttctjo.html

[U14] Py：分组收集到列表
来源：http://hz.svipenyu.cn/gtmpuypvxb.html

defaultdict(list)
来源：http://hz.shanyushiyangkeji.top/gthkoizsli.html

[U15] Py：高精度计时
来源：http://hz.zhaomingkeji.xyz/gtwnehwrna.html

t = time.perf_counter()
来源：http://hz.xziqi.cn/gtjaismuwi.html

[U16] Py：命令行参数解析
来源：http://hz.hysaishi.cn/gtfdattqcr.html

ap = argparse.ArgumentParser();  ap.add_argument("--name");  args = ap.parse_args()
来源：http://hz.yuxming.cn/gtvrhwljpl.html

[U17] Py：初始化日志
来源：http://hz.vqdsnc.cn/gtkoltljvw.html

logging.basicConfig(level=logging.INFO)
来源：http://hz.yuanzhike.top/gtpwhuxoho.html

[U18] Py：预编译正则
来源：http://hz.tanke756.top/gtwhvajfhb.html

pat = re.compile(r"\d+")
来源：http://hz.shangyingyoupin.top/gttuwhwqef.html

[U19] Py：正则替换带回调
来源：http://hz.xingfuxueyuan.xyz/gtxeytippk.html

re.sub(r"\d+", lambda m: str(int(m.group()) * 2), s)
来源：http://hz.redwolf501.top/gtulxgndqb.html

[U20] Py：缓存函数结果
来源：http://hz.hammf.cn/gtrqxgnkxe.html

@functools.lru_cache(maxsize=None)
来源：http://hz.fengsongda.top/gtyctdgqln.html

[U21] Py：自定义上下文管理器
来源：http://hz.vqdsnc.cn/gteqdvzrcq.html

@contextlib.contextmanager
来源：http://hz.nanxinkj.top/gtfpakmeaj.html

[U22] Py：矩阵转置
来源：http://hz.zhijiandao.cn/gtvyavftwa.html

list(zip(*m))
来源：http://hz.shuidangran.top/gtevlwcixj.html

[U23] Py：分块读取大文件
来源：http://hz.guowangkeji.top/gtgynjdwbr.html

for chunk in iter(lambda: f.read(8192), b""):
来源：http://hz.zdqjudy.top/gtaqokqhly.html

[U24] Py：路径操作
来源：http://hz.hammf.cn/gtnckrzgnz.html

Path("a/b.txt").parent.mkdir(parents=True, exist_ok=True)
来源：http://hz.chenzaomai.com/gtlubmvqll.html

[U25] Py：CSV 按字典读
来源：http://hz.yuxming.cn/gtvflohuzw.html

csv.DictReader(f)
来源：http://hz.jyoumei.cn/gtxprpocru.html

[U26] Py：并发下载
来源：http://hz.shanyushiyangkeji.top/gtripujkjz.html

ThreadPoolExecutor(max_workers=8).map(fetch, urls)
来源：http://hz.hongshengwenyu.top/gtxoqxmvdr.html

[U27] Py：异步 HTTP
来源：http://hz.yuxming.cn/gtszvmkcww.html

aiohttp.ClientSession() 配合 async with
来源：http://hz.ybcxt.top/gttwdhvoig.html

[U28] Py：类型别名
来源：http://hz.shuidangran.top/gtgeyadphv.html

UserId = int
来源：http://hz.cheryme.top/gtkjihyakj.html

[U29] Py：属性校验
来源：http://hz.gzhubu.top/gthykkomub.html

@property 与 @x.setter 配合
来源：http://hz.jyoumei.cn/gtddhzwrfv.html

[U30] Py：数据类
来源：http://hz.bjfxy.top/gtkcmpeimn.html

@dataclass(slots=True)
来源：http://hz.iojbl.cn/gtwjktmsib.html

[U31] Py：单测
来源：http://hz.sweek.top/gteagxcmpc.html

python -m pytest -q
来源：http://hz.xuanzx.com/gtkczwimfw.html

[U32] Py：代码格式化
来源：http://hz.smart0.xyz/gtmwdbldje.html

ruff format . && ruff check --fix .
来源：http://hz.zhiwuduotai.top/gtofmlpxsd.html

[U33] Py：打包发布
来源：http://hz.nanxuanxn.top/gtludpieno.html

python -m build  （依赖 pyproject.toml）
来源：http://hz.zhijiandao.cn/gtlflatupo.html

[U34] Py：判断编码
来源：http://hz.shanyushiyangtech.top/gtnjtdkolc.html

chardet.detect(raw)
来源：http://hz.gaohongyu789.top/gtiamyrkti.html

[U35] Py：发送邮件
来源：http://hz.jinqigfzy.top/gtvxoshbqq.html

smtplib.SMTP_SSL(...).send_message(msg)
来源：http://hz.0kj1m.cn/gtiwbgntpz.html

[U36] Py：定时任务
来源：http://hz.haohaochexian.top/gtenpugdti.html

schedule.every(10).minutes.do(job)
来源：http://hz.0kj1m.cn/gtemvvbslk.html

[U37] Py：读写 Excel
来源：http://hz.pengpengdd.cyou/gtxboyjaef.html

pandas.read_excel / DataFrame.to_excel
来源：http://hz.bjfxy.top/gtbbazftih.html

[U38] Py：获取脚本所在目录
来源：http://hz.daxiang520.top/gtwygvxble.html

Path(__file__).resolve().parent
来源：http://hz.sysykeji.top/gtkztkdefv.html

[U39] Py：判断是否在交互环境
来源：http://hz.cucudq.cn/gttqclimzc.html

sys.stdout.isatty()
来源：http://hz.jiagoushi.top/gtumxjviwu.html

[U40] Py：打印到标准错误
来源：http://hz.hysaishi.cn/gtamrasbfb.html

print("err", file=sys.stderr)
来源：http://hz.yj202588.top/gtdcudqoby.html

[U41] PHP：初始化 Composer 项目
来源：http://hz.daria6918.cn/gtmrfugnvw.html

composer init;  composer require guzzlehttp/guzzle
来源：http://hz.andypj.xyz/gtzqneelfe.html

[U42] PHP：PSR-4 自动加载
来源：http://hz.hywenlv.cn/gtekujruxp.html

"autoload": { "psr-4": { "App\\": "src/" } }
来源：http://hz.jinqigfzy.top/gtdqwxwunw.html

[U43] PHP：声明命名空间
来源：http://hz.jinqigfzy.top/gtvjjilvlc.html

namespace App\Http;
来源：http://hz.jianghu66.top/gtxobxfxew.html

[U44] PHP：开启严格类型
来源：http://hz.ppjwa.cn/gtjxcbamup.html

declare(strict_types=1);
来源：http://hz.yonumen.top/gtjjkzllpv.html

[U45] PHP：类型声明与返回类型
来源：http://hz.yj20258.top/gtgtxuqxxu.html

function add(int $a, int $b): int { return $a + $b; }
来源：http://hz.fzhhl.top/gttrcmkwmw.html

[U46] PHP：可空类型
来源：http://hz.jqgufenzy.top/gtsydpruyb.html

?string $name = null
来源：http://hz.hnxiangtu.top/gtctabszps.html

[U47] PHP：联合类型
来源：http://hz.yueranfly.top/gtpgbuzshz.html

int|string $id
来源：http://hz.xuetiantiany.cn/gtebpelkxv.html

[U48] PHP：纯枚举
来源：http://hz.nanxuanxn.top/gtrwfvizef.html

enum Status: string { case Active = "active"; case Off = "off"; }
来源：http://hz.jinghuilouyu.cn/gttwyravij.html

[U49] PHP：只读属性
来源：http://hz.ydzc1.top/gtktwndmwf.html

public readonly string $name
来源：http://hz.jlsjyb.cn/gtazcnqebq.html

[U50] PHP：构造器属性提升
来源：http://hz.hammf.cn/gtbkqyreol.html

public function __construct(private int $id) {}
来源：http://hz.yuanzhike.top/gtxdencagc.html

[U51] PHP：数组解构
来源：http://hz.daria6918.cn/gtqrroexlw.html

[$a, $b] = $arr;
来源：http://hz.cashguo.top/gtdeuoqski.html

[U52] PHP：箭头函数
来源：http://hz.chenzaomai.com/gthhquciik.html

$double = fn($x) => $x * 2;
来源：http://hz.aibaodan.cn/gtjooxpnnz.html

[U53] PHP：空合并运算符
来源：http://hz.xingfuxueyuan.xyz/gtnxrcmdtg.html

$v = $a ?? $b ?? "default";
来源：http://hz.daxiang520.top/gtluuipceh.html

[U54] PHP：空安全调用
来源：http://hz.jinqigufen.top/gtifduplfj.html

$obj?->method()
来源：http://hz.xuetiantiany.cn/gtjfxffidi.html

[U55] PHP：match 表达式
来源：http://hz.jianghu66.top/gtzegavdaf.html

$s = match($x) { 1 => "一", default => "其他" };
来源：http://hz.ybcxt.top/gtropeorqv.html

[U56] PHP：命名参数
来源：http://hz.ywan-chungtsiang.top/gtadugwibp.html

f(a: 1, b: 2)
来源：http://hz.hongshengwenyu.top/gtxtvmkfkw.html

[U57] PHP：字符串插值
来源：http://hz.snrcjt.cn/gtsxibozqc.html

"值: {$a}"
来源：http://hz.shanyushiyangkeji.top/gtioekkwdt.html

[U58] PHP：数组三件套
来源：http://hz.ehwqpu.com/gthaibnnyb.html

array_map($f, $a);  array_filter($a, $f);  array_reduce($a, $f, 0);
来源：http://hz.havefunace.top/gtsxcuepfc.html

[U59] PHP：自定义排序
来源：http://hz.shzxlz.cn/gtwwhjfvsy.html

usort($arr, fn($a, $b) => $a["age"] <=> $b["age"]);
来源：http://hz.jinyuanbaomall.cn/gttumsvlvv.html

[U60] PHP：JSON 编解码
来源：http://hz.bjfxy.top/gtmmwskjwl.html

json_encode($d, JSON_UNESCAPED_UNICODE);  json_decode($s, true);
来源：http://hz.snrcjt.cn/gtpexvoxab.html


<!-- 参考信息 -->