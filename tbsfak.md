代发 wailian999

[S43] C++：智能指针
来源：http://hz.xingfuxueyuan.xyz/gtnfbghosz.html

auto p = std::make_unique<int>(5);
来源：http://hz.guowangkeji.top/gtoczbgowy.html

[S44] C++：引用传参
来源：http://hz.zycfv.cn/gtxjuodjez.html

void inc(int &x) { ++x; }
来源：http://hz.gaohongyu789.top/gtcoctptpz.html

[S45] C++：lambda
来源：http://hz.ehwqpu.com/gtegrvteej.html

auto add = [](int a, int b) { return a + b; };
来源：http://hz.yj202588.top/gttxydzplk.html

[S46] C++：函数模板
来源：http://hz.c1oappe.top/gtpecfkeqb.html

template <typename T> T maxv(T a, T b) { return a > b ? a : b; }
来源：http://hz.haohaochexian.top/gtrfztogoz.html

[S47] C++：结构化绑定遍历
来源：http://hz.yangfankeji.com/gtcqahksli.html

for (const auto &[k, v] : m) { std::cout << k << v; }
来源：http://hz.hysaishi.cn/gtwtelsmdl.html

[S48] C++：逐行读文件
来源：http://hz.daxiang520.top/gtnzomjxks.html

std::ifstream in("a.txt");  std::string line;
来源：http://hz.havefunace.top/gtlgujsfka.html

while (std::getline(in, line)) { }
来源：http://hz.yueranfly.top/gtdtymzhgd.html

[S49] C++：写文件
来源：http://hz.hfpthk.cn/gtpompwdhd.html

std::ofstream out("a.txt");  out << "hi\n";
来源：http://hz.dashuyun.cn/gtwdxksnap.html

[S50] C++：格式化数字
来源：http://hz.shanyushiyangkeji.top/gtzjwqzipx.html

std::ostringstream os;  os << std::fixed << std::setprecision(2) << 3.14159;
来源：http://hz.guowangkeji.top/gtfhyxsdwb.html

[S51] C++：显式类型转换
来源：http://hz.yonumen.top/gtuvdlkuxv.html

static_cast<double>(a) / b
来源：http://hz.haohaochexian.top/gtfzaeroke.html

[S52] C++：const 与 noexcept
来源：http://hz.0kj1m.cn/gtqcicwkek.html

int size() const noexcept { return n_; }
来源：http://hz.yuxming.cn/gteewrmejz.html

[S53] C++：移动语义
来源：http://hz.sysykeji.top/gtkurgwixv.html

std::vector<int> w = std::move(v);
来源：http://hz.jianghu66.top/gtemyvmewm.html

[S54] C++：异常处理
来源：http://hz.zhijiandao.cn/gttrvqfjfe.html

try { throw std::runtime_error("x"); } catch (const std::exception &e) { }
来源：http://hz.zhixingplan.top/gtjdtdopks.html

[S55] C++：结构化绑定
来源：http://hz.cucudq.cn/gtoyuxfawm.html

auto [a, b] = std::make_pair(1, 2);
来源：http://hz.cqqwz.cn/gtlhsofmqo.html

[S56] C++：optional
来源：http://hz.ppjwa.cn/gtcqaagala.html

std::optional<int> o = 5;  if (o) { int v = *o; }
来源：http://hz.yj20258.top/gtzkczwfbv.html

[S57] C++：编译期常量
来源：http://hz.meibo888.top/gtlxlcfadi.html

constexpr int N = 10;
来源：http://hz.bjfxy.top/gthhvcssij.html

[S58] C++：命名空间
来源：http://hz.cashguo.top/gtpqmtyckk.html

namespace ns { int f() { return 1; } }
来源：http://hz.jlsjyb.cn/gtitidbszi.html

[S59] C++：静态断言
来源：http://hz.ydzc1.top/gtxxgkgljx.html

static_assert(sizeof(int) == 4, "int 必须 4 字节");
来源：http://hz.sysykeji.top/gtrxywiitj.html

[S60] C++：遍历并删除元素
来源：http://hz.iojbl.cn/gtydazstos.html

v.erase(std::remove_if(v.begin(), v.end(), [](int x) { return x < 0; }), v.end());
来源：http://hz.smart0.xyz/gtqqmdgaaw.html

================================================================================
来源：http://hz.xuanzx.com/gtpenveaco.html

T. 其他语言补充（Kotlin / Swift / Lua / Perl / Scala）
来源：http://hz.shangyingyoupin.top/gtngbooalx.html

================================================================================
来源：http://hz.52xcode.cn/gtziuexkcx.html

[T01] Kotlin：Hello World
来源：http://hz.aibaodan.cn/gtqmazpblf.html

println("Hello")
来源：http://hz.iojbl.cn/gtiwawuket.html

[T02] Kotlin：变量
来源：http://hz.hongshengwenyu.top/gtfnflwhpt.html

val a = 1;  var b = 2        // val 只读，var 可变
来源：http://hz.fzhhl.top/gttbxllghi.html

[T03] Kotlin：字符串模板
来源：http://hz.jinyuanbaomall.cn/gtahjyxnxz.html

"值: $b"
来源：http://hz.redwolf501.top/gtmydyaavr.html

[T04] Kotlin：空安全
来源：http://hz.vqdsnc.cn/gtdfntorot.html

val n: String? = null;  n?.length
来源：http://hz.sweek.top/gteslxcwgu.html

[T05] Kotlin：when 表达式
来源：http://hz.hfpthk.cn/gtwadkijnt.html

val s = when (x) { 1 -> "一" else -> "其他" }   // 多分支时每个分支单独一行
来源：http://hz.hongshengwenyu.top/gtolnbxken.html

[T06] Kotlin：集合映射
来源：http://hz.chenzaomai.com/gttdfsnoaf.html

listOf(1, 2, 3).map { it * 2 }
来源：http://hz.bjfxy.top/gtilaetkbj.html

[T07] Kotlin：集合过滤
来源：http://hz.cheryme.top/gtrgncnxgk.html

listOf(1, 2, 3).filter { it > 1 }
来源：http://hz.jinqigufen.top/gtqhwrkovd.html

[T08] Kotlin：数据类
来源：http://hz.zhoulong.xyz/gtactmmroo.html

data class User(val name: String, val age: Int)
来源：http://hz.aizwys.cn/gtzzmzfqge.html

[T09] Kotlin：扩展函数
来源：http://hz.zhoulong.xyz/gtqbbekbwo.html

fun String.exclaim() = this + "!"
来源：http://hz.zhongyouzk.top/gttpdvjoog.html

[T10] Kotlin：默认参数
来源：http://hz.yonumen.top/gtotdvyfnq.html

fun greet(name: String = "World") = "Hi $name"
来源：http://hz.jqgufenzy.top/gtircszkov.html

[T11] Kotlin：协程
来源：http://hz.bjfxy.top/gtajrolqdp.html

GlobalScope.launch { delay(1000); println("done") }
来源：http://hz.hnqzz.top/gtyztvkhob.html

[T12] Kotlin：解构声明
来源：http://hz.jiagoushi.top/gtuknqjoai.html

val (a, b) = Pair(1, 2)
来源：http://hz.xingfuxueyuan.xyz/gtkbwqoksn.html

[T13] Kotlin：只读 Map
来源：http://hz.gaohongyu789.top/gtryqfuwcp.html

val m = mapOf("a" to 1)
来源：http://hz.hongshengwenyu.top/gtwnsqsyxu.html

[T14] Kotlin：循环
来源：http://hz.xylfe.cn/gtltmhrgrq.html

for (i in 1..10) println(i)
来源：http://hz.yuanzhike.top/gtrninbrnb.html

[T15] Kotlin：接口
来源：http://hz.yonumen.top/gtxvtsvjcn.html

interface Shape { fun area(): Double }
来源：http://hz.cucudq.cn/gtgyfwhirm.html

[T16] Swift：Hello World
来源：http://hz.jianghu66.top/gtvtrpvxmy.html

print("Hello")
来源：http://hz.hywenlv.cn/gtqkzeycdp.html

[T17] Swift：变量与常量
来源：http://hz.jinqigfzy.top/gtqrtfztuk.html

var a = 1;  let b = 2
来源：http://hz.yangfankeji.com/gtzcnmyhsj.html

[T18] Swift：字符串插值
来源：http://hz.bjfxy.top/gtnncfpxbi.html

"值: \(b)"
来源：http://hz.chenlongwang.top/gtsfrqllot.html

[T19] Swift：可选绑定
来源：http://hz.jqgfzy.top/gtdfwbbsxk.html

if let n = opt { print(n) }
来源：http://hz.yangfankeji.com/gtygiambak.html

[T20] Swift：数组操作
来源：http://hz.zycfv.cn/gtfcliwltb.html

var a = [1, 2, 3];  a.append(4)
来源：http://hz.zdqjudy.top/gtnuzqxjcd.html

[T21] Swift：遍历
来源：http://hz.sysykeji.top/gtgsyuwzat.html

for x in a { print(x) }
来源：http://hz.zdqjudy.top/gtrrafaoek.html

[T22] Swift：字典
来源：http://hz.fzhhl.top/gtvflanplx.html

var d = ["a": 1];  d["b"] = 2
来源：http://hz.yueranfly.top/gtmlahqali.html

[T23] Swift：函数
来源：http://hz.0kj1m.cn/gtydtdgekp.html

func add(_ a: Int, _ b: Int) -> Int { a + b }
来源：http://hz.andypj.xyz/gtgcwhzsvd.html

[T24] Swift：闭包
来源：http://hz.daria6918.cn/gtlnogksfi.html

let f = { (x: Int) -> Int in x * 2 }
来源：http://hz.jinqigfzy.top/gtplmzeivd.html

[T25] Swift：结构体
来源：http://hz.gogol.net.cn/gtibwqvwli.html

struct P { var x: Int }
来源：http://hz.havefunace.top/gtwnscxueo.html

[T26] Swift：类与重写
来源：http://hz.yj20258888.top/gtpqnquomx.html

class A: Base { override func f() {} }
来源：http://hz.dashuyun.cn/gtewewiarf.html

[T27] Swift：错误处理
来源：http://hz.zhaomingkeji.xyz/gtqmigqkbp.html

do { try f() } catch { print(error) }
来源：http://hz.xingfuxueyuan.xyz/gttvcywmyn.html

[T28] Swift：枚举
来源：http://hz.jyoumei.cn/gtlkmvaehk.html

enum Color { case red, green }
来源：http://hz.shangyingyoupin.top/gtonmzyfkq.html

[T29] Swift：guard 提前返回
来源：http://hz.yanxiufei.cn/gtyuyaajaa.html

guard let x = opt else { return }
来源：http://hz.zhongyouzk.top/gtonfxvagl.html

[T30] Swift：协议
来源：http://hz.xingfuxueyuan.xyz/gtbgbzkqjj.html

protocol Shape { func area() -> Double }
来源：http://hz.snrcjt.cn/gtjnwakpym.html

[T31] Lua：Hello World
来源：http://hz.sweek.top/gtpcdjqxix.html

print("Hello")
来源：http://hz.0kj1m.cn/gtkrmccjuo.html

[T32] Lua：局部变量
来源：http://hz.c1oappe.top/gtwdhgjvgj.html

local a = 1
来源：http://hz.yongpay.top/gtqvzafzxj.html

[T33] Lua：表（数组）
来源：http://hz.0kj1m.cn/gtuqiaxykl.html

local t = {1, 2, 3};  t[4] = 4
来源：http://hz.meibo888.top/gtkzxgjydp.html

[T34] Lua：遍历表
来源：http://hz.guowangkeji.top/gtbrgiguov.html

for i, v in ipairs(t) do print(i, v) end
来源：http://hz.dianchejie.cn/gtyygbvcyn.html

[T35] Lua：字典表
来源：http://hz.ydzc1.top/gtrojjnmwh.html

local d = { a = 1 };  d.b = 2
来源：http://hz.shanyushiyangkeji.top/gtxuetirrv.html

[T36] Lua：函数
来源：http://hz.chenlongwang.top/gtcimaspza.html

function add(a, b) return a + b end
来源：http://hz.jiagoushi.top/gtxgjjgupe.html

[T37] Lua：字符串拼接
来源：http://hz.cucudq.cn/gtyzytthrq.html

"a" .. "b"
来源：http://hz.xuanzx.com/gtbpdmopbx.html

[T38] Lua：条件
来源：http://hz.haohaochexian.top/gtopsrfmeq.html

if x > 0 then print("正") end
来源：http://hz.daria6918.cn/gtdjjehphc.html

[T39] Lua：模式匹配
来源：http://hz.chenjidiqi.icu/gtvnmhlmmy.html

string.find(s, "%d+")
来源：http://hz.aizwys.cn/gtwkqspwik.html

[T40] Lua：元表
来源：http://hz.svipenyu.cn/gtweciletl.html

setmetatable({}, { __index = base })
来源：http://hz.havefunace.top/gtiqwswuta.html

[T41] Perl：Hello World
来源：http://hz.ppjwa.cn/gtwipejgqs.html

print "Hello\n";
来源：http://hz.wangdashe.top/gtapkicohi.html

[T42] Perl：变量类型
来源：http://hz.shanyushiyangkeji.top/gtrtnzvmme.html

my $a = 1;  my @arr = (1, 2, 3);  my %h = (a => 1);
来源：http://hz.jiagoushi.top/gtjngyejaj.html

[T43] Perl：字符串插值
来源：http://hz.c1oappe.top/gtpmcaifby.html

"值: $a"
来源：http://hz.xuanzx.com/gtpsnhjmzj.html

[T44] Perl：条件
来源：http://hz.havefunace.top/gtrkerxdwi.html

if ($a > 0) { print "正"; }
来源：http://hz.nanxuanxn.top/gtzroxvren.html

[T45] Perl：数组遍历
来源：http://hz.ppjwa.cn/gtnznbrdmu.html

for my $x (@arr) { print $x; }
来源：http://hz.mhx1999.top/gtxkmqxqzs.html

[T46] Perl：哈希操作
来源：http://hz.vqdsnc.cn/gtqpphenao.html

$h{b} = 2;  for my $k (keys %h) { print "$k=$h{$k}"; }
来源：http://hz.xingfuxueyuan.xyz/gtskpkkdso.html

[T47] Perl：正则捕获
来源：http://hz.daria6918.cn/gtptsrxdgr.html

if ($s =~ /(\d+)/) { print $1; }
来源：http://hz.sxryk.cn/gtvxbjhqhx.html

[T48] Perl：正则替换
来源：http://hz.zhijiandao.cn/gtxtnijzez.html

$s =~ s/old/new/g;
来源：http://hz.52xcode.cn/gtcncdasju.html

[T49] Perl：函数
来源：http://hz.zycfv.cn/gtuqwoyfqq.html

sub add { my ($a, $b) = @_; return $a + $b; }
来源：http://hz.yongpay.top/gtkopdyfoq.html

[T50] Perl：逐行读文件
来源：http://hz.jyoumei.cn/gtujuaukdz.html

open my $fh, "<", "a.txt" or die $!;
来源：http://hz.zycfv.cn/gtudtmusdb.html

while (my $line = <$fh>) { print $line; }
来源：http://hz.yangfankeji.com/gttffcrjcu.html

[T51] Scala：Hello World
来源：http://hz.316326.xyz/gtaunefvmx.html

println("Hello")
来源：http://hz.xziqi.cn/gtbxgdxoft.html

[T52] Scala：变量
来源：http://hz.havefunace.top/gtenzcgofq.html

val a = 1;  var b = 2
来源：http://hz.jlsjyb.cn/gtrcqvpsjz.html

[T53] Scala：字符串插值
来源：http://hz.ydjk.org.cn/gtjcwrroty.html

s"值: $b"
来源：http://hz.cucudq.cn/gtjzjzrpvy.html

[T54] Scala：集合映射
来源：http://hz.yonumen.top/gtzuuhzwku.html

List(1, 2, 3).map(_ * 2)
来源：http://hz.gogol.net.cn/gtpwkrhgal.html

[T55] Scala：集合过滤
来源：http://hz.gogol.net.cn/gtggwyalbt.html

List(1, 2, 3).filter(_ > 1)
来源：http://hz.xingfuxueyuan.xyz/gtpzffkysg.html

[T56] Scala：样例类
来源：http://hz.cdnleiting.top/gtwdmgjrhl.html

case class User(name: String, age: Int)
来源：http://hz.zhijiandao.cn/gtinchcyyh.html

[T57] Scala：模式匹配
来源：http://hz.xylfe.cn/gtogbphgip.html

x match { case 1 => "一"; case _ => "其他" }
来源：http://hz.yj202588.top/gthgcjnznr.html

[T58] Scala：函数定义
来源：http://hz.hnqzz.top/gtvvhoxxey.html

def add(a: Int, b: Int): Int = a + b
来源：http://hz.fzhhl.top/gtuhdphfmw.html

[T59] Scala：循环
来源：http://hz.yuanzhike.top/gtczsdinja.html

for (i <- 1 to 10) println(i)
来源：http://hz.vqdsnc.cn/gtldqyowlf.html

[T60] Scala：折叠
来源：http://hz.xuanzx.com/gttbyuosya.html

List(1, 2, 3).foldLeft(0)(_ + _)
来源：http://hz.quarkkingdee.top/gtwwgfncwg.html

================================================================================
来源：http://hz.jqgfzy.top/gtgazexigb.html

U. 高频实用片段（Python / PHP / JavaScript 各 40 条）
来源：http://hz.jinghuilouyu.cn/gttdmghehr.html

================================================================================
来源：http://hz.chenjidiqi.icu/gtsvjqgeia.html

[U01] Py：创建虚拟环境
来源：http://hz.quarkkingdee.top/gtguxwkhnu.html

python -m venv .venv && source .venv/bin/activate
来源：http://hz.daria6918.cn/gtuvgshheo.html

[U02] Py：导出 / 安装依赖
来源：http://hz.nwbrower.top/gtctcitdzd.html

pip freeze > requirements.txt;  pip install -r requirements.txt
来源：http://hz.nanxuanxn.top/gtdgawuyzm.html

[U03] Py：加载 .env 配置
来源：http://hz.quarkkingdee.top/gtitiklxez.html

from dotenv import load_dotenv; load_dotenv()
来源：http://hz.cashguo.top/gtdoertvre.html

[U04] Py：变量调试打印
来源：http://hz.dashuyun.cn/gtgjdtnavq.html

print(f"{x=}")            # 输出 x=值，Python 3.8+
来源：http://hz.meibo888.top/gtdnvgdprj.html

[U05] Py：列表去重且保序
来源：http://hz.cucudq.cn/gtqdbcaowe.html

list(dict.fromkeys(arr))
来源：http://hz.yueranfly.top/gtauqkvjge.html

[U06] Py：合并两个字典
来源：http://hz.52xcode.cn/gtoijczmym.html

{**a, **b}
来源：http://hz.hnxiangtu.top/gteojdxsmw.html

[U07] Py：反转字典键值
来源：http://hz.cheryme.top/gtmnnlchpj.html

{v: k for k, v in d.items()}
来源：http://hz.sufxvd.cn/gthqxyfrnz.html

[U08] Py：展平二维列表
来源：http://hz.aibaodan.cn/gtgukovleb.html

[y for x in nested for y in x]
来源：http://hz.gzhubu.top/gtnffccepc.html

[U09] Py：字典取最大值的键
来源：http://hz.ywan-chungtsiang.top/gtyivjisdk.html

max(d, key=d.get)
来源：http://hz.birdmap.top/gtiwjdtuqb.html

[U10] Py：按值排序字典
来源：http://hz.jqgufenzy.top/gtnmogrovv.html

dict(sorted(d.items(), key=lambda kv: kv[1]))
来源：http://hz.cdnleiting.top/gtndzypazp.html

[U11] Py：生成器表达式
来源：http://hz.yvedp.cn/gtvqoisdzz.html

(x * 2 for x in arr)
来源：http://hz.svipenyu.cn/gtialcikyk.html

[U12] Py：取出现最多的 3 个元素
来源：http://hz.ybcxt.top/gtqiqbahvd.html

Counter(arr).most_common(3)
来源：http://hz.gaohongyu789.top/gtzfsalujz.html

[U13] Py：固定长度队列
来源：http://hz.zhixingplan.top/gtpfaeuwee.html

deque(maxlen=10)
来源：http://hz.andypj.xyz/gtcplbmzmg.html

[U14] Py：分组收集到列表
来源：http://hz.ydjk.org.cn/gthahecmrf.html

defaultdict(list)
来源：http://hz.quarkkingdee.top/gtnsntnlvc.html

[U15] Py：高精度计时
来源：http://hz.zhengqikj.top/gtgpjjxwox.html

t = time.perf_counter()
来源：http://hz.xziqi.cn/gtnkormfjs.html

[U16] Py：命令行参数解析
来源：http://hz.gotoacloud.top/gtrmjefbya.html

ap = argparse.ArgumentParser();  ap.add_argument("--name");  args = ap.parse_args()
来源：http://hz.52xcode.cn/gttillgvay.html

[U17] Py：初始化日志
来源：http://hz.hnxiangtu.top/gtjfgvltwm.html

logging.basicConfig(level=logging.INFO)
来源：http://hz.yj20258888.top/gtbafogenj.html

[U18] Py：预编译正则
来源：http://hz.0kj1m.cn/gtfxxkhcev.html

pat = re.compile(r"\d+")
来源：http://hz.gogol.net.cn/gtahlrjgvj.html

[U19] Py：正则替换带回调
来源：http://hz.xziqi.cn/gtgsfgxncz.html

re.sub(r"\d+", lambda m: str(int(m.group()) * 2), s)
来源：http://hz.c1oappe.top/gtetayrapc.html

[U20] Py：缓存函数结果
来源：http://hz.sweek.top/gtxwfvxlms.html

@functools.lru_cache(maxsize=None)
来源：http://hz.cashguo.top/gtefvowswv.html

[U21] Py：自定义上下文管理器
来源：http://hz.zhixingplan.top/gtcykvxwvv.html

@contextlib.contextmanager
来源：http://hz.aizwys.cn/gtksgqripj.html

[U22] Py：矩阵转置
来源：http://hz.xuanzx.com/gtvaomutgt.html

list(zip(*m))
来源：http://hz.iojbl.cn/gtuwzozwza.html

[U23] Py：分块读取大文件
来源：http://hz.yangfankeji.com/gtfqlkextl.html

for chunk in iter(lambda: f.read(8192), b""):
来源：http://hz.yj20258888.top/gtrnbklapr.html

[U24] Py：路径操作
来源：http://hz.zhixingplan.top/gtnlzfmynj.html

Path("a/b.txt").parent.mkdir(parents=True, exist_ok=True)
来源：http://hz.cucudq.cn/gtcishosdc.html

[U25] Py：CSV 按字典读
来源：http://hz.cqqwz.cn/gtrwlsyhaj.html

csv.DictReader(f)
来源：http://hz.xuetiantiany.cn/gtyymrhcyu.html

[U26] Py：并发下载
来源：http://hz.tianlin.xyz/gtnaidhlqg.html

ThreadPoolExecutor(max_workers=8).map(fetch, urls)
来源：http://hz.c1oappe.top/gtmdihjxdv.html

[U27] Py：异步 HTTP
来源：http://hz.cheryme.top/gtlgmyrthr.html

aiohttp.ClientSession() 配合 async with
来源：http://hz.sysykeji.top/gtiiduazsl.html

[U28] Py：类型别名
来源：http://hz.meibo888.top/gtmmeerhlb.html

UserId = int
来源：http://hz.gzhubu.top/gtedkxbzwr.html

[U29] Py：属性校验
来源：http://hz.jlsjyb.cn/gtyxnkdksy.html

@property 与 @x.setter 配合
来源：http://hz.xylfe.cn/gtktvwndym.html

[U30] Py：数据类
来源：http://hz.sysykeji.top/gtsunrvijj.html

@dataclass(slots=True)
来源：http://hz.daria6918.cn/gtkhkzsjxw.html

[U31] Py：单测
来源：http://hz.daria6918.cn/gtavtvvvut.html

python -m pytest -q
来源：http://hz.jlsjyb.cn/gtzlgauobz.html

[U32] Py：代码格式化
来源：http://hz.cucudq.cn/gtzoieedft.html

ruff format . && ruff check --fix .
来源：http://hz.shanyushiyangtech.top/gtdmofgjqx.html

[U33] Py：打包发布
来源：http://hz.ybcxt.top/gtrgzclvly.html

python -m build  （依赖 pyproject.toml）
来源：http://hz.yueranfly.top/gtwplyvugm.html

[U34] Py：判断编码
来源：http://hz.jinghuilouyu.cn/gtfcyoqvvv.html

chardet.detect(raw)
来源：http://hz.wangshuangyany.cn/gtddkvxtkr.html

[U35] Py：发送邮件
来源：http://hz.shzxlz.cn/gthayullzy.html

smtplib.SMTP_SSL(...).send_message(msg)
来源：http://hz.cheryme.top/gtkcgfhxjg.html

[U36] Py：定时任务
来源：http://hz.sxryk.cn/gteexafdut.html

schedule.every(10).minutes.do(job)
来源：http://hz.aibaodan.cn/gtddvtrmsp.html

[U37] Py：读写 Excel
来源：http://hz.hammf.cn/gtyngzpldg.html

pandas.read_excel / DataFrame.to_excel
来源：http://hz.ywan-chungtsiang.top/gtwxcpvsnj.html

[U38] Py：获取脚本所在目录
来源：http://hz.nanxinkj.top/gtcyvllgiy.html

Path(__file__).resolve().parent
来源：http://hz.pengpengdd.cyou/gtugftjgdn.html

[U39] Py：判断是否在交互环境
来源：http://hz.nwbrower.top/gteluahnim.html

sys.stdout.isatty()
来源：http://hz.gogol.net.cn/gtyhnfqaem.html

[U40] Py：打印到标准错误
来源：http://hz.cucudq.cn/gtudpahywf.html

print("err", file=sys.stderr)
来源：http://hz.shanyushiyangkeji.top/gtzlcgxvij.html

[U41] PHP：初始化 Composer 项目
来源：http://hz.bjfxy.top/gtewrjdegb.html

composer init;  composer require guzzlehttp/guzzle
来源：http://hz.pycfn.com/gtroggwrkm.html

[U42] PHP：PSR-4 自动加载
来源：http://hz.xziqi.cn/gtuchfrbmh.html

"autoload": { "psr-4": { "App\\": "src/" } }
来源：http://hz.shzxlz.cn/gtxhyvisin.html

[U43] PHP：声明命名空间
来源：http://hz.wangdashe.top/gtbrohdtdj.html

namespace App\Http;
来源：http://hz.yueranfly.top/gtyunbmcsz.html

[U44] PHP：开启严格类型
来源：http://hz.jinqigfzy.top/gtadqpnmbr.html

declare(strict_types=1);
来源：http://hz.xuanzx.com/gtnfocwopy.html

[U45] PHP：类型声明与返回类型
来源：http://hz.hysaishi.cn/gtjlhxullh.html

function add(int $a, int $b): int { return $a + $b; }
来源：http://hz.gotoacloud.top/gtzlbmthlf.html

[U46] PHP：可空类型
来源：http://hz.gotoacloud.top/gtwighzkyy.html

?string $name = null
来源：http://hz.9152youxi.cn/gtprvtucol.html

[U47] PHP：联合类型
来源：http://hz.chenzaomai.com/gtcdaxtffv.html

int|string $id
来源：http://hz.ydjk.org.cn/gtrmluvqaz.html

[U48] PHP：纯枚举
来源：http://hz.daria6918.cn/gtsggzoefe.html

enum Status: string { case Active = "active"; case Off = "off"; }
来源：http://hz.gotoacloud.top/gtucfshptq.html

[U49] PHP：只读属性
来源：http://hz.zhijiandao.cn/gtqgbnjise.html

public readonly string $name
来源：http://hz.dashuyun.cn/gtjanbigjh.html

[U50] PHP：构造器属性提升
来源：http://hz.jinyuanbaomall.cn/gtmiejquvt.html

public function __construct(private int $id) {}
来源：http://hz.zdqjudy.top/gtwkwamxnf.html

[U51] PHP：数组解构
来源：http://hz.ybcxt.top/gtaesmuamg.html

[$a, $b] = $arr;
来源：http://hz.smart0.xyz/gtqivmlioz.html

[U52] PHP：箭头函数
来源：http://hz.jyoumei.cn/gtbrelouzn.html

$double = fn($x) => $x * 2;
来源：http://hz.xziqi.cn/gtthzcwdvf.html

[U53] PHP：空合并运算符
来源：http://hz.jinghuilouyu.cn/gtfubsdtiv.html

$v = $a ?? $b ?? "default";
来源：http://hz.yangfankeji.com/gtdpkvpodw.html

[U54] PHP：空安全调用
来源：http://hz.zdqjudy.top/gtihraivmv.html

$obj?->method()
来源：http://hz.ivvv.top/gtdjorpflm.html

[U55] PHP：match 表达式
来源：http://hz.feifeiyinyue.top/gtysxkzzgz.html

$s = match($x) { 1 => "一", default => "其他" };
来源：http://hz.ywan-chungtsiang.top/gtqictofob.html

[U56] PHP：命名参数
来源：http://hz.hnxiangtu.top/gtunlxcphx.html

f(a: 1, b: 2)
来源：http://hz.jinghuilouyu.cn/gtpjenxjbf.html

[U57] PHP：字符串插值
来源：http://hz.zycfv.cn/gtuyenerxf.html

"值: {$a}"
来源：http://hz.quarkkingdee.top/gtjjdyfxln.html

[U58] PHP：数组三件套
来源：http://hz.cucudq.cn/gtvqyhhtuz.html

array_map($f, $a);  array_filter($a, $f);  array_reduce($a, $f, 0);
来源：http://hz.ivvv.top/gtqofivmqx.html

[U59] PHP：自定义排序
来源：http://hz.xinyue.icu/gteccknzeo.html

usort($arr, fn($a, $b) => $a["age"] <=> $b["age"]);
来源：http://hz.shuidangran.top/gtmeabmgqa.html

[U60] PHP：JSON 编解码
来源：http://hz.feifeiyinyue.top/gtqppvtnhk.html

json_encode($d, JSON_UNESCAPED_UNICODE);  json_decode($s, true);
来源：http://hz.sufxvd.cn/gtftlvzxwd.html

[U61] PHP：正则
来源：http://hz.ivvv.top/gtdodzfzfa.html

preg_match('/(\d+)/', $s, $m);  preg_replace('/\d+/', '#', $s);
来源：http://hz.shuidangran.top/gtxihatiug.html

[U62] PHP：日期对象
来源：http://hz.xziqi.cn/gtmzywzmsd.html

(new DateTimeImmutable())->format("Y-m-d");
来源：http://hz.aizwys.cn/gtubgryvrv.html

[U63] PHP：文件读写
来源：http://hz.hfpthk.cn/gtikcrccdt.html

file_get_contents($f);  file_put_contents($f, $data);
来源：http://hz.tanke756.top/gtiuvalkbi.html

[U64] PHP：目录遍历
来源：http://hz.nanxinkj.top/gtseegpkuq.html

glob("dir/*.php");  scandir("dir");
来源：http://hz.sweek.top/gtsnfvhupr.html

[U65] PHP：会话
来源：http://hz.kuanghao11.cn/gtvknamcln.html

session_start();  $_SESSION["uid"] = 1;
来源：http://hz.zhijiandao.cn/gtywguotvp.html

[U66] PHP：设置 Cookie
来源：http://hz.jqgfzy.top/gtxokgjsir.html

setcookie("token", $v, ["httponly" => true, "samesite" => "Lax"]);
来源：http://hz.ydjk.org.cn/gtbelpwhrp.html

[U67] PHP：处理文件上传
来源：http://hz.iojbl.cn/gtjikgsaua.html

$_FILES["file"]["tmp_name"] 与 move_uploaded_file()
来源：http://hz.yangfankeji.com/gtgvqticgh.html

[U68] PHP：PDO 连接
来源：http://hz.cqqwz.cn/gtgxhhuoqh.html

$pdo = new PDO("mysql:host=localhost;dbname=app", "root", "");
来源：http://hz.hongshengwenyu.top/gtanvgjztd.html


<!-- 参考信息 -->