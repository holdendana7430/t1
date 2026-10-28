代发 wailian999

[S43] C++：智能指针
来源：http://hz.xuanzx.com/gthafhrjlh.html

auto p = std::make_unique<int>(5);
来源：http://hz.hysaishi.cn/gteqildwld.html

[S44] C++：引用传参
来源：http://hz.yj20258.top/gtugpouawc.html

void inc(int &x) { ++x; }
来源：http://hz.9152youxi.cn/gtisnqcqoo.html

[S45] C++：lambda
来源：http://hz.hysaishi.cn/gtlpxmovsc.html

auto add = [](int a, int b) { return a + b; };
来源：http://hz.mhx1999.top/gtkhcbjjhc.html

[S46] C++：函数模板
来源：http://hz.ydjk.org.cn/gtmseemazd.html

template <typename T> T maxv(T a, T b) { return a > b ? a : b; }
来源：http://hz.feifeiyinyue.top/gtbowvwdcq.html

[S47] C++：结构化绑定遍历
来源：http://hz.sufxvd.cn/gtvkvmujgw.html

for (const auto &[k, v] : m) { std::cout << k << v; }
来源：http://hz.daria6918.cn/gtapwfctuu.html

[S48] C++：逐行读文件
来源：http://hz.redwolf501.top/gtglixusaq.html

std::ifstream in("a.txt");  std::string line;
来源：http://hz.wangshuangyany.cn/gtnyfrmizy.html

while (std::getline(in, line)) { }
来源：http://hz.hongshengwenyu.top/gtkjlmnamq.html

[S49] C++：写文件
来源：http://hz.0kj1m.cn/gtixxuahur.html

std::ofstream out("a.txt");  out << "hi\n";
来源：http://hz.iojbl.cn/gttiebwdjh.html

[S50] C++：格式化数字
来源：http://hz.zdqjudy.top/gtthrcqfog.html

std::ostringstream os;  os << std::fixed << std::setprecision(2) << 3.14159;
来源：http://hz.andypj.xyz/gtmreyqmut.html

[S51] C++：显式类型转换
来源：http://hz.ppjwa.cn/gtndhjzwyh.html

static_cast<double>(a) / b
来源：http://hz.shzxlz.cn/gtxmqxrzow.html

[S52] C++：const 与 noexcept
来源：http://hz.zhoulong.xyz/gtgtynbuux.html

int size() const noexcept { return n_; }
来源：http://hz.cdnleiting.top/gtkzvltwkz.html

[S53] C++：移动语义
来源：http://hz.yueranfly.top/gtwfeyyglw.html

std::vector<int> w = std::move(v);
来源：http://hz.xingfuxueyuan.xyz/gtrfhaderx.html

[S54] C++：异常处理
来源：http://hz.xylfe.cn/gttcfvhbop.html

try { throw std::runtime_error("x"); } catch (const std::exception &e) { }
来源：http://hz.jqgfzy.top/gtiddtdeju.html

[S55] C++：结构化绑定
来源：http://hz.wangdashe.top/gtjxaqnocm.html

auto [a, b] = std::make_pair(1, 2);
来源：http://hz.gogol.net.cn/gtxktfrihn.html

[S56] C++：optional
来源：http://hz.aibaodan.cn/gtjeawarjf.html

std::optional<int> o = 5;  if (o) { int v = *o; }
来源：http://hz.vqdsnc.cn/gtzdlotayp.html

[S57] C++：编译期常量
来源：http://hz.guannengcc.top/gtikmqwlow.html

constexpr int N = 10;
来源：http://hz.guowangkeji.top/gtafbrqqir.html

[S58] C++：命名空间
来源：http://hz.shangyingyoupin.top/gtbnshhccm.html

namespace ns { int f() { return 1; } }
来源：http://hz.nanxuanxn.top/gthrgldpxs.html

[S59] C++：静态断言
来源：http://hz.daxiang520.top/gtvodxjlqh.html

static_assert(sizeof(int) == 4, "int 必须 4 字节");
来源：http://hz.haohaochexian.top/gtzpyupppu.html

[S60] C++：遍历并删除元素
来源：http://hz.feifeiyinyue.top/gtmtrnidqi.html

v.erase(std::remove_if(v.begin(), v.end(), [](int x) { return x < 0; }), v.end());
来源：http://hz.jqgufenzy.top/gtfukrkgou.html

================================================================================
来源：http://hz.xingfuxueyuan.xyz/gtsfqjkuqj.html

T. 其他语言补充（Kotlin / Swift / Lua / Perl / Scala）
来源：http://hz.sxryk.cn/gtlvrqprwz.html

================================================================================
来源：http://hz.gotoacloud.top/gtovcztmhj.html

[T01] Kotlin：Hello World
来源：http://hz.zdqjudy.top/gtgycoijiy.html

println("Hello")
来源：http://hz.daxiang520.top/gthoactfyy.html

[T02] Kotlin：变量
来源：http://hz.zdqjudy.top/gtlbpgrvlv.html

val a = 1;  var b = 2        // val 只读，var 可变
来源：http://hz.jlsjyb.cn/gtmmmezzqi.html

[T03] Kotlin：字符串模板
来源：http://hz.sysykeji.top/gtswmlnknl.html

"值: $b"
来源：http://hz.svipenyu.cn/gtfxpjlydu.html

[T04] Kotlin：空安全
来源：http://hz.iojbl.cn/gtldgdyapi.html

val n: String? = null;  n?.length
来源：http://hz.gaohongyu789.top/gtplncxcuq.html

[T05] Kotlin：when 表达式
来源：http://hz.chenlongwang.top/gtfyilgtxk.html

val s = when (x) { 1 -> "一" else -> "其他" }   // 多分支时每个分支单独一行
来源：http://hz.chenzaomai.com/gtvslqesuf.html

[T06] Kotlin：集合映射
来源：http://hz.shanyushiyangkeji.top/gtcjlfzept.html

listOf(1, 2, 3).map { it * 2 }
来源：http://hz.zhaomingkeji.xyz/gtebxyonvz.html

[T07] Kotlin：集合过滤
来源：http://hz.pengpengdd.cyou/gtzlkhwmgf.html

listOf(1, 2, 3).filter { it > 1 }
来源：http://hz.zhaomingkeji.xyz/gtlcuctmaz.html

[T08] Kotlin：数据类
来源：http://hz.xuanzx.com/gtielgsgly.html

data class User(val name: String, val age: Int)
来源：http://hz.jinyuanbaomall.cn/gtnupjujbl.html

[T09] Kotlin：扩展函数
来源：http://hz.yuanzhike.top/gtkyqbvppe.html

fun String.exclaim() = this + "!"
来源：http://hz.cqqwz.cn/gtoettnkxl.html

[T10] Kotlin：默认参数
来源：http://hz.xuanzx.com/gtowsbrlxs.html

fun greet(name: String = "World") = "Hi $name"
来源：http://hz.cheryme.top/gtqqgfuwdb.html

[T11] Kotlin：协程
来源：http://hz.haohaochexian.top/gteyawsdds.html

GlobalScope.launch { delay(1000); println("done") }
来源：http://hz.mhx1999.top/gttdejrilg.html

[T12] Kotlin：解构声明
来源：http://hz.sufxvd.cn/gtcmpvlrtb.html

val (a, b) = Pair(1, 2)
来源：http://hz.xuanzx.com/gtoeluywex.html

[T13] Kotlin：只读 Map
来源：http://hz.52xcode.cn/gtajcyumxw.html

val m = mapOf("a" to 1)
来源：http://hz.sxryk.cn/gtwzaurvzw.html

[T14] Kotlin：循环
来源：http://hz.iojbl.cn/gtwhvwdqdc.html

for (i in 1..10) println(i)
来源：http://hz.redwolf501.top/gtdpntaapb.html

[T15] Kotlin：接口
来源：http://hz.jiagoushi.top/gtjjzpmswp.html

interface Shape { fun area(): Double }
来源：http://hz.yueranfly.top/gtjixmhqwc.html

[T16] Swift：Hello World
来源：http://hz.guannengcc.top/gtmalfibmy.html

print("Hello")
来源：http://hz.hnqzz.top/gtzynncwyf.html

[T17] Swift：变量与常量
来源：http://hz.zycfv.cn/gtsnvrsxns.html

var a = 1;  let b = 2
来源：http://hz.guannengcc.top/gthcdmclgo.html

[T18] Swift：字符串插值
来源：http://hz.shanyushiyangtech.top/gttdstlyfl.html

"值: \(b)"
来源：http://hz.shuidangran.top/gtijjwvgqw.html

[T19] Swift：可选绑定
来源：http://hz.yj20258.top/gtpejupmqq.html

if let n = opt { print(n) }
来源：http://hz.shzxlz.cn/gtlwfvlops.html

[T20] Swift：数组操作
来源：http://hz.wangdashe.top/gtphsidhzy.html

var a = [1, 2, 3];  a.append(4)
来源：http://hz.shanyushiyangkeji.top/gtrtvoicsd.html

[T21] Swift：遍历
来源：http://hz.snrcjt.cn/gtjxbxjuai.html

for x in a { print(x) }
来源：http://hz.jinyuanbaomall.cn/gtepqelhyw.html

[T22] Swift：字典
来源：http://hz.svipenyu.cn/gtnlonjush.html

var d = ["a": 1];  d["b"] = 2
来源：http://hz.zhengqikj.top/gtlhnvdzpi.html

[T23] Swift：函数
来源：http://hz.ivvv.top/gtfmrczvbl.html

func add(_ a: Int, _ b: Int) -> Int { a + b }
来源：http://hz.jqgufenzy.top/gtephryqds.html

[T24] Swift：闭包
来源：http://hz.shanyushiyangkeji.top/gtmkkhnfwx.html

let f = { (x: Int) -> Int in x * 2 }
来源：http://hz.316326.xyz/gtfyqkluqt.html

[T25] Swift：结构体
来源：http://hz.iojbl.cn/gthschbulw.html

struct P { var x: Int }
来源：http://hz.zhoulong.xyz/gtkrpxxfum.html

[T26] Swift：类与重写
来源：http://hz.shuidangran.top/gtqgrvmlfj.html

class A: Base { override func f() {} }
来源：http://hz.snrcjt.cn/gtzgqknwta.html

[T27] Swift：错误处理
来源：http://hz.jyoumei.cn/gtvcbhkufh.html

do { try f() } catch { print(error) }
来源：http://hz.tian-w.cn/gtdwnlyics.html

[T28] Swift：枚举
来源：http://hz.xinyue.icu/gtytkolaoo.html

enum Color { case red, green }
来源：http://hz.yj20258888.top/gtizqgvtoc.html

[T29] Swift：guard 提前返回
来源：http://hz.jinqigufen.top/gtuccpzszw.html

guard let x = opt else { return }
来源：http://hz.yuanzhike.top/gtljznktog.html

[T30] Swift：协议
来源：http://hz.zycfv.cn/gteezjrfbq.html

protocol Shape { func area() -> Double }
来源：http://hz.jyoumei.cn/gtcznrzzyc.html

[T31] Lua：Hello World
来源：http://hz.yuxming.cn/gtxordkqoy.html

print("Hello")
来源：http://hz.jinghuilouyu.cn/gtpryenwxa.html

[T32] Lua：局部变量
来源：http://hz.svipenyu.cn/gtgsfgemcr.html

local a = 1
来源：http://hz.daria6918.cn/gttscaxjya.html

[T33] Lua：表（数组）
来源：http://hz.snrcjt.cn/gtpzpgnbsu.html

local t = {1, 2, 3};  t[4] = 4
来源：http://hz.yuxming.cn/gtgdacndai.html

[T34] Lua：遍历表
来源：http://hz.yvedp.cn/gtvqisgsvs.html

for i, v in ipairs(t) do print(i, v) end
来源：http://hz.svipenyu.cn/gtgzyprfej.html

[T35] Lua：字典表
来源：http://hz.tian-w.cn/gtjsmtjsce.html

local d = { a = 1 };  d.b = 2
来源：http://hz.xuetiantiany.cn/gtvoouyxir.html

[T36] Lua：函数
来源：http://hz.yj20258.top/gtsfysevhl.html

function add(a, b) return a + b end
来源：http://hz.9152youxi.cn/gtcvhoyywo.html

[T37] Lua：字符串拼接
来源：http://hz.zdqjudy.top/gttohbshkj.html

"a" .. "b"
来源：http://hz.sxryk.cn/gtsmxlaggz.html

[T38] Lua：条件
来源：http://hz.zhaomingkeji.xyz/gtavzgrbyn.html

if x > 0 then print("正") end
来源：http://hz.tianlin.xyz/gtqmqwqdci.html

[T39] Lua：模式匹配
来源：http://hz.hnqzz.top/gtfdneuvkf.html

string.find(s, "%d+")
来源：http://hz.hywenlv.cn/gtypztbvur.html

[T40] Lua：元表
来源：http://hz.shzxlz.cn/gtlnqgovaj.html

setmetatable({}, { __index = base })
来源：http://hz.ivvv.top/gtbzsqzmoz.html

[T41] Perl：Hello World
来源：http://hz.dianchejie.cn/gtlqisfisg.html

print "Hello\n";
来源：http://hz.ydzc1.top/gtsckcyjzk.html

[T42] Perl：变量类型
来源：http://hz.pengpengdd.cyou/gtqjuzkzmq.html

my $a = 1;  my @arr = (1, 2, 3);  my %h = (a => 1);
来源：http://hz.nanxuanxn.top/gtmygzgfoo.html

[T43] Perl：字符串插值
来源：http://hz.feifeiyinyue.top/gtgotssgxg.html

"值: $a"
来源：http://hz.yj202588.top/gtmhwiophn.html

[T44] Perl：条件
来源：http://hz.wangdashe.top/gttczjzqcu.html

if ($a > 0) { print "正"; }
来源：http://hz.xingfuxueyuan.xyz/gtgtbglhaj.html

[T45] Perl：数组遍历
来源：http://hz.svipenyu.cn/gtlecrfhyw.html

for my $x (@arr) { print $x; }
来源：http://hz.xinyue.icu/gtfncyqnai.html

[T46] Perl：哈希操作
来源：http://hz.52xcode.cn/gtryvzqnpx.html

$h{b} = 2;  for my $k (keys %h) { print "$k=$h{$k}"; }
来源：http://hz.feifeiyinyue.top/gtqdpkxajr.html

[T47] Perl：正则捕获
来源：http://hz.hfpthk.cn/gtwrcbclen.html

if ($s =~ /(\d+)/) { print $1; }
来源：http://hz.nwbrower.top/gtmahuspig.html

[T48] Perl：正则替换
来源：http://hz.zycfv.cn/gtkabefvod.html

$s =~ s/old/new/g;
来源：http://hz.jqgufenzy.top/gtdshpqmdd.html

[T49] Perl：函数
来源：http://hz.ppjwa.cn/gtoqnmcvej.html

sub add { my ($a, $b) = @_; return $a + $b; }
来源：http://hz.guannengcc.top/gtoleigtdq.html

[T50] Perl：逐行读文件
来源：http://hz.hywenlv.cn/gtvqchnzuf.html

open my $fh, "<", "a.txt" or die $!;
来源：http://hz.sufxvd.cn/gteufpsmzu.html

while (my $line = <$fh>) { print $line; }
来源：http://hz.snrcjt.cn/gtmfwxjkde.html

[T51] Scala：Hello World
来源：http://hz.gzhubu.top/gtwyvryaej.html

println("Hello")
来源：http://hz.dashuyun.cn/gturzbgzwj.html

[T52] Scala：变量
来源：http://hz.jlsjyb.cn/gtdehiebyg.html

val a = 1;  var b = 2
来源：http://hz.jlsjyb.cn/gtffdbxbna.html

[T53] Scala：字符串插值
来源：http://hz.pycfn.com/gtagdageww.html

s"值: $b"
来源：http://hz.hywenlv.cn/gtmzgivuhy.html

[T54] Scala：集合映射
来源：http://hz.jiagoushi.top/gtlocwbtkz.html

List(1, 2, 3).map(_ * 2)
来源：http://hz.shanyushiyangkeji.top/gtaktsljar.html

[T55] Scala：集合过滤
来源：http://hz.ydjk.org.cn/gtgrwpgooo.html

List(1, 2, 3).filter(_ > 1)
来源：http://hz.xinyue.icu/gtniijswcq.html

[T56] Scala：样例类
来源：http://hz.yangfankeji.com/gtcivqmbwe.html

case class User(name: String, age: Int)
来源：http://hz.zhaomingkeji.xyz/gtjqbocwcf.html

[T57] Scala：模式匹配
来源：http://hz.quarkkingdee.top/gtbauajyzf.html

x match { case 1 => "一"; case _ => "其他" }
来源：http://hz.zdqjudy.top/gtqepzlzhq.html

[T58] Scala：函数定义
来源：http://hz.sweek.top/gthqygdykc.html

def add(a: Int, b: Int): Int = a + b
来源：http://hz.yongpay.top/gtzvudohez.html

[T59] Scala：循环
来源：http://hz.yanxiufei.cn/gtiwfxhsrm.html

for (i <- 1 to 10) println(i)
来源：http://hz.guowangkeji.top/gtucndrrje.html

[T60] Scala：折叠
来源：http://hz.xinyue.icu/gtrdkmsjox.html

List(1, 2, 3).foldLeft(0)(_ + _)
来源：http://hz.yuxming.cn/gtijrrvwig.html

================================================================================
来源：http://hz.havefunace.top/gtwxnjrdxc.html

U. 高频实用片段（Python / PHP / JavaScript 各 40 条）
来源：http://hz.pengpengdd.cyou/gtrfrcejof.html

================================================================================
来源：http://hz.ivvv.top/gtpzkzndfm.html

[U01] Py：创建虚拟环境
来源：http://hz.dianchejie.cn/gthodvachr.html

python -m venv .venv && source .venv/bin/activate
来源：http://hz.hnqzz.top/gtldwhbegk.html

[U02] Py：导出 / 安装依赖
来源：http://hz.fengsongda.top/gtqdhubkhq.html

pip freeze > requirements.txt;  pip install -r requirements.txt
来源：http://hz.ybcxt.top/gthgfddqww.html

[U03] Py：加载 .env 配置
来源：http://hz.haohaochexian.top/gtuupodjgo.html

from dotenv import load_dotenv; load_dotenv()
来源：http://hz.ivvv.top/gtvgllsrmw.html

[U04] Py：变量调试打印
来源：http://hz.tian-w.cn/gtfdilbosu.html

print(f"{x=}")            # 输出 x=值，Python 3.8+
来源：http://hz.316326.xyz/gtngwsxzrp.html

[U05] Py：列表去重且保序
来源：http://hz.yonumen.top/gtdzgjsmxs.html

list(dict.fromkeys(arr))
来源：http://hz.hfpthk.cn/gtuucgmxpq.html

[U06] Py：合并两个字典
来源：http://hz.hnqzz.top/gtqtfykiwb.html

{**a, **b}
来源：http://hz.cdnleiting.top/gthgopmqcd.html

[U07] Py：反转字典键值
来源：http://hz.guannengcc.top/gtsxdoezzx.html

{v: k for k, v in d.items()}
来源：http://hz.jinyuanbaomall.cn/gtbmwxplnr.html

[U08] Py：展平二维列表
来源：http://hz.pengpengdd.cyou/gtfgiezbdn.html

[y for x in nested for y in x]
来源：http://hz.shangyingyoupin.top/gtfolvpsww.html

[U09] Py：字典取最大值的键
来源：http://hz.tian-w.cn/gtlrvmcdsw.html

max(d, key=d.get)
来源：http://hz.shangyingyoupin.top/gtizdldlmy.html

[U10] Py：按值排序字典
来源：http://hz.jiagoushi.top/gtualcbslc.html

dict(sorted(d.items(), key=lambda kv: kv[1]))
来源：http://hz.meibo888.top/gtiwbjleuz.html

[U11] Py：生成器表达式
来源：http://hz.cucudq.cn/gtkysmahxe.html

(x * 2 for x in arr)
来源：http://hz.xuetiantiany.cn/gtwnuprkkj.html

[U12] Py：取出现最多的 3 个元素
来源：http://hz.xuetiantiany.cn/gtqxrfoumf.html

Counter(arr).most_common(3)
来源：http://hz.vqdsnc.cn/gtkfpbjplc.html

[U13] Py：固定长度队列
来源：http://hz.zycfv.cn/gthdvtkcrh.html

deque(maxlen=10)
来源：http://hz.0kj1m.cn/gtpcxaoeog.html

[U14] Py：分组收集到列表
来源：http://hz.jianghu66.top/gtzfxccwzi.html

defaultdict(list)
来源：http://hz.iojbl.cn/gtmjggnmbf.html

[U15] Py：高精度计时
来源：http://hz.jqgufenzy.top/gtjewzgutj.html

t = time.perf_counter()
来源：http://hz.tian-w.cn/gtozfluovv.html

[U16] Py：命令行参数解析
来源：http://hz.zhongyouzk.top/gtgvvipdrd.html

ap = argparse.ArgumentParser();  ap.add_argument("--name");  args = ap.parse_args()
来源：http://hz.zhaomingkeji.xyz/gtmjtatwrb.html

[U17] Py：初始化日志
来源：http://hz.hongshengwenyu.top/gttifwjkwl.html

logging.basicConfig(level=logging.INFO)
来源：http://hz.nwbrower.top/gtejxxzdfi.html

[U18] Py：预编译正则
来源：http://hz.jinqigfzy.top/gteigzjqjo.html

pat = re.compile(r"\d+")
来源：http://hz.0kj1m.cn/gthglwejnk.html

[U19] Py：正则替换带回调
来源：http://hz.zhoulong.xyz/gteszeverg.html

re.sub(r"\d+", lambda m: str(int(m.group()) * 2), s)
来源：http://hz.mhx1999.top/gtxzjifwmd.html

[U20] Py：缓存函数结果
来源：http://hz.zhiwuduotai.top/gtopuzqagr.html

@functools.lru_cache(maxsize=None)
来源：http://hz.ehwqpu.com/gtwzvribxl.html

[U21] Py：自定义上下文管理器
来源：http://hz.316326.xyz/gtjmwartsg.html

@contextlib.contextmanager
来源：http://hz.yuxming.cn/gtxkxiywsl.html

[U22] Py：矩阵转置
来源：http://hz.sysykeji.top/gtymcfczcr.html

list(zip(*m))
来源：http://hz.shanyushiyangtech.top/gtquzntdmw.html

[U23] Py：分块读取大文件
来源：http://hz.zhiwuduotai.top/gtpugiayxl.html

for chunk in iter(lambda: f.read(8192), b""):
来源：http://hz.xingfuxueyuan.xyz/gtrewrnvgs.html

[U24] Py：路径操作
来源：http://hz.fengsongda.top/gtjpcaeojs.html

Path("a/b.txt").parent.mkdir(parents=True, exist_ok=True)
来源：http://hz.meibo888.top/gtgdyprgqh.html

[U25] Py：CSV 按字典读
来源：http://hz.gaohongyu789.top/gtmzbbzpyy.html

csv.DictReader(f)
来源：http://hz.316326.xyz/gtzpbabkgx.html

[U26] Py：并发下载
来源：http://hz.iojbl.cn/gtwskuicez.html

ThreadPoolExecutor(max_workers=8).map(fetch, urls)
来源：http://hz.aizwys.cn/gtbrrinwyn.html

[U27] Py：异步 HTTP
来源：http://hz.sysykeji.top/gtmdzkfqbc.html

aiohttp.ClientSession() 配合 async with
来源：http://hz.chenjidiqi.icu/gtjwgsxuxp.html

[U28] Py：类型别名
来源：http://hz.guannengcc.top/gtxpsonoqg.html

UserId = int
来源：http://hz.chenzaomai.com/gtkopcfpgr.html

[U29] Py：属性校验
来源：http://hz.gogol.net.cn/gtdrteqiea.html

@property 与 @x.setter 配合
来源：http://hz.jlsjyb.cn/gtzrkcxdqc.html

[U30] Py：数据类
来源：http://hz.hongshengwenyu.top/gtvziovvcg.html

@dataclass(slots=True)
来源：http://hz.zhoulong.xyz/gtfjzhlqso.html

[U31] Py：单测
来源：http://hz.nanxuanxn.top/gtwetjwswp.html

python -m pytest -q
来源：http://hz.guannengcc.top/gtpbhykhoa.html

[U32] Py：代码格式化
来源：http://hz.havefunace.top/gtcidxcavx.html

ruff format . && ruff check --fix .
来源：http://hz.bjfxy.top/gtwozrlfkt.html

[U33] Py：打包发布
来源：http://hz.cdnleiting.top/gtoczmqewh.html

python -m build  （依赖 pyproject.toml）
来源：http://hz.52xcode.cn/gtwpijeuxk.html

[U34] Py：判断编码
来源：http://hz.yuanzhike.top/gtxhpohcom.html

chardet.detect(raw)
来源：http://hz.birdmap.top/gtkxdantzi.html

[U35] Py：发送邮件
来源：http://hz.xuetiantiany.cn/gtxananrqr.html

smtplib.SMTP_SSL(...).send_message(msg)
来源：http://hz.sxryk.cn/gtvtdrruzx.html

[U36] Py：定时任务
来源：http://hz.zhijiandao.cn/gtjmklvgbj.html

schedule.every(10).minutes.do(job)
来源：http://hz.feifeiyinyue.top/gtpssmuabu.html

[U37] Py：读写 Excel
来源：http://hz.aizwys.cn/gtsmzoaisc.html

pandas.read_excel / DataFrame.to_excel
来源：http://hz.dashuyun.cn/gtuotyoagr.html

[U38] Py：获取脚本所在目录
来源：http://hz.redwolf501.top/gtblpogrfi.html

Path(__file__).resolve().parent
来源：http://hz.jinqigfzy.top/gtjcgdfjho.html

[U39] Py：判断是否在交互环境
来源：http://hz.shanyushiyangtech.top/gtzurxuwak.html

sys.stdout.isatty()
来源：http://hz.guannengcc.top/gtftaedczw.html

[U40] Py：打印到标准错误
来源：http://hz.gotoacloud.top/gtxezppuge.html

print("err", file=sys.stderr)
来源：http://hz.fzhhl.top/gtyitlnytu.html

[U41] PHP：初始化 Composer 项目
来源：http://hz.zdqjudy.top/gtyhwwvzun.html

composer init;  composer require guzzlehttp/guzzle
来源：http://hz.ybcxt.top/gtkcofrvxi.html

[U42] PHP：PSR-4 自动加载
来源：http://hz.jianghu66.top/gtolpvsywu.html

"autoload": { "psr-4": { "App\\": "src/" } }
来源：http://hz.cucudq.cn/gteutknkga.html

[U43] PHP：声明命名空间
来源：http://hz.yueranfly.top/gthsumvjcp.html

namespace App\Http;
来源：http://hz.birdmap.top/gtkeasytrz.html

[U44] PHP：开启严格类型
来源：http://hz.316326.xyz/gtrgfpbnfn.html

declare(strict_types=1);
来源：http://hz.bjfxy.top/gtbiwuqjju.html

[U45] PHP：类型声明与返回类型
来源：http://hz.xingfuxueyuan.xyz/gtefdzisjv.html

function add(int $a, int $b): int { return $a + $b; }
来源：http://hz.sysykeji.top/gtscvpuqjh.html

[U46] PHP：可空类型
来源：http://hz.yueranfly.top/gtzzjwckgx.html

?string $name = null
来源：http://hz.shuidangran.top/gtfxhaluvz.html

[U47] PHP：联合类型
来源：http://hz.chenjidiqi.icu/gtkfwugxmn.html

int|string $id
来源：http://hz.0kj1m.cn/gtvtnyursi.html

[U48] PHP：纯枚举
来源：http://hz.zhongyouzk.top/gtvirblyoc.html

enum Status: string { case Active = "active"; case Off = "off"; }
来源：http://hz.ivvv.top/gtodyypspy.html

[U49] PHP：只读属性
来源：http://hz.chenjidiqi.icu/gtvdgmwsvm.html

public readonly string $name
来源：http://hz.ywan-chungtsiang.top/gtkriplblu.html

[U50] PHP：构造器属性提升
来源：http://hz.yj202588.top/gteajvsbey.html

public function __construct(private int $id) {}
来源：http://hz.aibaodan.cn/gtzxaqqvfd.html

[U51] PHP：数组解构
来源：http://hz.cqqwz.cn/gtneumdwza.html

[$a, $b] = $arr;
来源：http://hz.guowangkeji.top/gtgbgbptnp.html

[U52] PHP：箭头函数
来源：http://hz.316326.xyz/gtcoyfguxu.html

$double = fn($x) => $x * 2;
来源：http://hz.yj202588.top/gttbuawusj.html

[U53] PHP：空合并运算符
来源：http://hz.dianchejie.cn/gtolacreeq.html

$v = $a ?? $b ?? "default";
来源：http://hz.pengpengdd.cyou/gtuxhofrke.html

[U54] PHP：空安全调用
来源：http://hz.hysaishi.cn/gtaoguydsl.html

$obj?->method()
来源：http://hz.tanke756.top/gtcnpstbyi.html

[U55] PHP：match 表达式
来源：http://hz.jianghu66.top/gtzjaxnghu.html

$s = match($x) { 1 => "一", default => "其他" };
来源：http://hz.9152youxi.cn/gtfmmyfohj.html

[U56] PHP：命名参数
来源：http://hz.yuxming.cn/gtljmjkmyg.html

f(a: 1, b: 2)
来源：http://hz.ydjk.org.cn/gtuqyhugby.html

[U57] PHP：字符串插值
来源：http://hz.xuanzx.com/gtlwncsnza.html

"值: {$a}"
来源：http://hz.tanke756.top/gttmgsoipu.html

[U58] PHP：数组三件套
来源：http://hz.aizwys.cn/gtdoigxxug.html

array_map($f, $a);  array_filter($a, $f);  array_reduce($a, $f, 0);
来源：http://hz.xuetiantiany.cn/gtggxheeem.html

[U59] PHP：自定义排序
来源：http://hz.0kj1m.cn/gtajbvmbol.html

usort($arr, fn($a, $b) => $a["age"] <=> $b["age"]);
来源：http://hz.meibo888.top/gtobqaxtct.html

[U60] PHP：JSON 编解码
来源：http://hz.hfpthk.cn/gtnucjhhgw.html

json_encode($d, JSON_UNESCAPED_UNICODE);  json_decode($s, true);
来源：http://hz.tian-w.cn/gtyvacjvnb.html

[U61] PHP：正则
来源：http://hz.sweek.top/gtohhrzmhi.html

preg_match('/(\d+)/', $s, $m);  preg_replace('/\d+/', '#', $s);
来源：http://hz.shanyushiyangkeji.top/gtfyeslsrx.html

[U62] PHP：日期对象
来源：http://hz.ppjwa.cn/gtkhozesqx.html

(new DateTimeImmutable())->format("Y-m-d");
来源：http://hz.iojbl.cn/gtmjdtmvld.html

[U63] PHP：文件读写
来源：http://hz.jinqigfzy.top/gtnfzxfqww.html

file_get_contents($f);  file_put_contents($f, $data);
来源：http://hz.cashguo.top/gtfdvvwhnq.html

[U64] PHP：目录遍历
来源：http://hz.yuanzhike.top/gtoykgjiaa.html

glob("dir/*.php");  scandir("dir");
来源：http://hz.cheryme.top/gtyicjggoz.html

[U65] PHP：会话
来源：http://hz.wangshuangyany.cn/gtdfzkgrpw.html

session_start();  $_SESSION["uid"] = 1;
来源：http://hz.zycfv.cn/gtnnsrhptq.html

[U66] PHP：设置 Cookie
来源：http://hz.wangdashe.top/gtjetcoryq.html

setcookie("token", $v, ["httponly" => true, "samesite" => "Lax"]);
来源：http://hz.ehwqpu.com/gtyuepvtqd.html

[U67] PHP：处理文件上传
来源：http://hz.xylfe.cn/gtteednakj.html

$_FILES["file"]["tmp_name"] 与 move_uploaded_file()
来源：http://hz.jlsjyb.cn/gteknttxwn.html

[U68] PHP：PDO 连接
来源：http://hz.zhiwuduotai.top/gtueyzlxtu.html

$pdo = new PDO("mysql:host=localhost;dbname=app", "root", "");
来源：http://hz.zycfv.cn/gtrdwrlrpv.html


<!-- 参考信息 -->