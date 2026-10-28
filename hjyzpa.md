代发 wailian999

[S45] C++：lambda
来源：http://hz.c1oappe.top/gtajdrkxvg.html

auto add = [](int a, int b) { return a + b; };
来源：http://hz.316326.xyz/gtwfvkzlcn.html

[S46] C++：函数模板
来源：http://hz.jinqigfzy.top/gtuepucutw.html

template <typename T> T maxv(T a, T b) { return a > b ? a : b; }
来源：http://hz.zycfv.cn/gtyptkrpqd.html

[S47] C++：结构化绑定遍历
来源：http://hz.yonumen.top/gtweqglmjz.html

for (const auto &[k, v] : m) { std::cout << k << v; }
来源：http://hz.xuetiantiany.cn/gtklirfrzd.html

[S48] C++：逐行读文件
来源：http://hz.hfpthk.cn/gtibpxskwj.html

std::ifstream in("a.txt");  std::string line;
来源：http://hz.dashuyun.cn/gtijgkpdjm.html

while (std::getline(in, line)) { }
来源：http://hz.hfpthk.cn/gtgtinistk.html

[S49] C++：写文件
来源：http://hz.xuetiantiany.cn/gtmtslzugm.html

std::ofstream out("a.txt");  out << "hi\n";
来源：http://hz.dashuyun.cn/gtsoepkekq.html

[S50] C++：格式化数字
来源：http://hz.cheryme.top/gtwolowwgs.html

std::ostringstream os;  os << std::fixed << std::setprecision(2) << 3.14159;
来源：http://hz.pycfn.com/gtkahttizc.html

[S51] C++：显式类型转换
来源：http://hz.birdmap.top/gtjaiokjlq.html

static_cast<double>(a) / b
来源：http://hz.iojbl.cn/gtjdfwwfkt.html

[S52] C++：const 与 noexcept
来源：http://hz.sufxvd.cn/gtbupheilt.html

int size() const noexcept { return n_; }
来源：http://hz.xingfuxueyuan.xyz/gthpefadfv.html

[S53] C++：移动语义
来源：http://hz.chenjidiqi.icu/gtriuyfmnl.html

std::vector<int> w = std::move(v);
来源：http://hz.yj20258.top/gtvpriwfdl.html

[S54] C++：异常处理
来源：http://hz.snrcjt.cn/gtrbmvsmvt.html

try { throw std::runtime_error("x"); } catch (const std::exception &e) { }
来源：http://hz.mhx1999.top/gtcmizuymn.html

[S55] C++：结构化绑定
来源：http://hz.gzhubu.top/gtdeuufjme.html

auto [a, b] = std::make_pair(1, 2);
来源：http://hz.ywan-chungtsiang.top/gtwpxauopi.html

[S56] C++：optional
来源：http://hz.sxryk.cn/gtmhvqgzwx.html

std::optional<int> o = 5;  if (o) { int v = *o; }
来源：http://hz.vqdsnc.cn/gtlknzayrp.html

[S57] C++：编译期常量
来源：http://hz.bjfxy.top/gtqhrmspft.html

constexpr int N = 10;
来源：http://hz.sysykeji.top/gtgwtdniaj.html

[S58] C++：命名空间
来源：http://hz.ydzc1.top/gtijpjffje.html

namespace ns { int f() { return 1; } }
来源：http://hz.yonumen.top/gtytceiahh.html

[S59] C++：静态断言
来源：http://hz.gaohongyu789.top/gtolivyqnz.html

static_assert(sizeof(int) == 4, "int 必须 4 字节");
来源：http://hz.zhixingplan.top/gtagnvpjhn.html

[S60] C++：遍历并删除元素
来源：http://hz.ydzc1.top/gtvemjeesz.html

v.erase(std::remove_if(v.begin(), v.end(), [](int x) { return x < 0; }), v.end());
来源：http://hz.yuanzhike.top/gtpixyoyyf.html

================================================================================
来源：http://hz.andypj.xyz/gtflkbcfjb.html

T. 其他语言补充（Kotlin / Swift / Lua / Perl / Scala）
来源：http://hz.nanxinkj.top/gtihcyjbxh.html

================================================================================
来源：http://hz.dianchejie.cn/gtbefmmiio.html

[T01] Kotlin：Hello World
来源：http://hz.nwbrower.top/gtyvkiovsl.html

println("Hello")
来源：http://hz.xingfuxueyuan.xyz/gtmlbiocvo.html

[T02] Kotlin：变量
来源：http://hz.xuanzx.com/gtwddsjhmn.html

val a = 1;  var b = 2        // val 只读，var 可变
来源：http://hz.ppjwa.cn/gtznvujjbt.html

[T03] Kotlin：字符串模板
来源：http://hz.dashuyun.cn/gttewflfzy.html

"值: $b"
来源：http://hz.pengpengdd.cyou/gthfbemxkn.html

[T04] Kotlin：空安全
来源：http://hz.yuxming.cn/gtpvqsvcjk.html

val n: String? = null;  n?.length
来源：http://hz.316326.xyz/gtohaksxzb.html

[T05] Kotlin：when 表达式
来源：http://hz.jiagoushi.top/gtdhzmpmpy.html

val s = when (x) { 1 -> "一" else -> "其他" }   // 多分支时每个分支单独一行
来源：http://hz.jinghuilouyu.cn/gtqgqetbgu.html

[T06] Kotlin：集合映射
来源：http://hz.xinyue.icu/gtzzobfhcf.html

listOf(1, 2, 3).map { it * 2 }
来源：http://hz.chenzaomai.com/gtftyrummu.html

[T07] Kotlin：集合过滤
来源：http://hz.meibo888.top/gtzroqlarr.html

listOf(1, 2, 3).filter { it > 1 }
来源：http://hz.quarkkingdee.top/gttabeiqdm.html

[T08] Kotlin：数据类
来源：http://hz.redwolf501.top/gthocgqpnv.html

data class User(val name: String, val age: Int)
来源：http://hz.jiagoushi.top/gtrbypypnj.html

[T09] Kotlin：扩展函数
来源：http://hz.hysaishi.cn/gttiyklegv.html

fun String.exclaim() = this + "!"
来源：http://hz.zycfv.cn/gtjggqlcgh.html

[T10] Kotlin：默认参数
来源：http://hz.nwbrower.top/gtnqokgkxa.html

fun greet(name: String = "World") = "Hi $name"
来源：http://hz.jinqigfzy.top/gtpyiiswnn.html

[T11] Kotlin：协程
来源：http://hz.chenlongwang.top/gtuycqflww.html

GlobalScope.launch { delay(1000); println("done") }
来源：http://hz.ydjk.org.cn/gtbyubseod.html

[T12] Kotlin：解构声明
来源：http://hz.sweek.top/gtedoublke.html

val (a, b) = Pair(1, 2)
来源：http://hz.316326.xyz/gtlmwisepv.html

[T13] Kotlin：只读 Map
来源：http://hz.hnxiangtu.top/gtdxdfymbd.html

val m = mapOf("a" to 1)
来源：http://hz.nanxuanxn.top/gtviltzzfv.html

[T14] Kotlin：循环
来源：http://hz.zhiwuduotai.top/gtbjqnvfay.html

for (i in 1..10) println(i)
来源：http://hz.dianchejie.cn/gtaycileex.html

[T15] Kotlin：接口
来源：http://hz.redwolf501.top/gtawhdsoug.html

interface Shape { fun area(): Double }
来源：http://hz.xuetiantiany.cn/gtdvknznhv.html

[T16] Swift：Hello World
来源：http://hz.yanxiufei.cn/gtjregwfwu.html

print("Hello")
来源：http://hz.guowangkeji.top/gttxdgurwt.html

[T17] Swift：变量与常量
来源：http://hz.hnxiangtu.top/gtmmelmoxz.html

var a = 1;  let b = 2
来源：http://hz.svipenyu.cn/gtlykvbmeg.html

[T18] Swift：字符串插值
来源：http://hz.bjfxy.top/gtrhxldpbt.html

"值: \(b)"
来源：http://hz.jinqigufen.top/gtufmrrxvs.html

[T19] Swift：可选绑定
来源：http://hz.shanyushiyangkeji.top/gthnjzavwf.html

if let n = opt { print(n) }
来源：http://hz.xingfuxueyuan.xyz/gtkrldwdec.html

[T20] Swift：数组操作
来源：http://hz.jinghuilouyu.cn/gtxndyrutk.html

var a = [1, 2, 3];  a.append(4)
来源：http://hz.guowangkeji.top/gtusxozfig.html

[T21] Swift：遍历
来源：http://hz.svipenyu.cn/gtvvziihbs.html

for x in a { print(x) }
来源：http://hz.yanxiufei.cn/gtiarehxxe.html

[T22] Swift：字典
来源：http://hz.quarkkingdee.top/gtyorkoqao.html

var d = ["a": 1];  d["b"] = 2
来源：http://hz.0kj1m.cn/gtsmeskxua.html

[T23] Swift：函数
来源：http://hz.hnqzz.top/gtjcirathv.html

func add(_ a: Int, _ b: Int) -> Int { a + b }
来源：http://hz.svipenyu.cn/gtkhelkqps.html

[T24] Swift：闭包
来源：http://hz.cqqwz.cn/gtrhledtka.html

let f = { (x: Int) -> Int in x * 2 }
来源：http://hz.hammf.cn/gthbdmfaaj.html

[T25] Swift：结构体
来源：http://hz.jqgufenzy.top/gtgqucbahf.html

struct P { var x: Int }
来源：http://hz.zhaomingkeji.xyz/gtwrlsmdmq.html

[T26] Swift：类与重写
来源：http://hz.andypj.xyz/gtanpcyvhf.html

class A: Base { override func f() {} }
来源：http://hz.hysaishi.cn/gtdyqptiro.html

[T27] Swift：错误处理
来源：http://hz.chenjidiqi.icu/gtrgjiuwsg.html

do { try f() } catch { print(error) }
来源：http://hz.jinqigufen.top/gtxleteumx.html

[T28] Swift：枚举
来源：http://hz.guowangkeji.top/gtzdzcbapu.html

enum Color { case red, green }
来源：http://hz.zycfv.cn/gtvpzvmagm.html

[T29] Swift：guard 提前返回
来源：http://hz.andypj.xyz/gtfnhsgjux.html

guard let x = opt else { return }
来源：http://hz.zhaomingkeji.xyz/gtozifybng.html

[T30] Swift：协议
来源：http://hz.dashuyun.cn/gtjiuernps.html

protocol Shape { func area() -> Double }
来源：http://hz.tianlin.xyz/gtpgmlqlse.html

[T31] Lua：Hello World
来源：http://hz.mhx1999.top/gtbgnhekuk.html

print("Hello")
来源：http://hz.jqgufenzy.top/gtkwopbfdf.html

[T32] Lua：局部变量
来源：http://hz.yangfankeji.com/gtuuwzkxcp.html

local a = 1
来源：http://hz.xylfe.cn/gtosdnwazx.html

[T33] Lua：表（数组）
来源：http://hz.haohaochexian.top/gtxxaevtuz.html

local t = {1, 2, 3};  t[4] = 4
来源：http://hz.iojbl.cn/gtajwvqvbo.html

[T34] Lua：遍历表
来源：http://hz.shangyingyoupin.top/gtcvadamws.html

for i, v in ipairs(t) do print(i, v) end
来源：http://hz.jinqigufen.top/gtcasxodwd.html

[T35] Lua：字典表
来源：http://hz.cashguo.top/gtspacvbnw.html

local d = { a = 1 };  d.b = 2
来源：http://hz.xuetiantiany.cn/gterbzpngf.html

[T36] Lua：函数
来源：http://hz.yj20258888.top/gtbvwojyzx.html

function add(a, b) return a + b end
来源：http://hz.ydzc1.top/gtysvmrmna.html

[T37] Lua：字符串拼接
来源：http://hz.shzxlz.cn/gtyeyrmgqi.html

"a" .. "b"
来源：http://hz.guannengcc.top/gtzwmfneqh.html

[T38] Lua：条件
来源：http://hz.tian-w.cn/gtxruopapi.html

if x > 0 then print("正") end
来源：http://hz.hnqzz.top/gtjxuccnou.html

[T39] Lua：模式匹配
来源：http://hz.zhixingplan.top/gtyfhjnxtd.html

string.find(s, "%d+")
来源：http://hz.yonumen.top/gtlkhzsaof.html

[T40] Lua：元表
来源：http://hz.pengpengdd.cyou/gtqudconfk.html

setmetatable({}, { __index = base })
来源：http://hz.jyoumei.cn/gtqjztoxgc.html

[T41] Perl：Hello World
来源：http://hz.yueranfly.top/gtuwjjbffd.html

print "Hello\n";
来源：http://hz.aibaodan.cn/gtlpevgmmt.html

[T42] Perl：变量类型
来源：http://hz.zhixingplan.top/gtldkfepps.html

my $a = 1;  my @arr = (1, 2, 3);  my %h = (a => 1);
来源：http://hz.0kj1m.cn/gtmdhnpaci.html

[T43] Perl：字符串插值
来源：http://hz.cdnleiting.top/gtqtbdnupo.html

"值: $a"
来源：http://hz.xylfe.cn/gtkmxjivrg.html

[T44] Perl：条件
来源：http://hz.sweek.top/gttjsfolgn.html

if ($a > 0) { print "正"; }
来源：http://hz.jinyuanbaomall.cn/gtwgkbpyhv.html

[T45] Perl：数组遍历
来源：http://hz.xinyue.icu/gtsxzfmgdk.html

for my $x (@arr) { print $x; }
来源：http://hz.vqdsnc.cn/gttrlelcxw.html

[T46] Perl：哈希操作
来源：http://hz.wangdashe.top/gtsragmsog.html

$h{b} = 2;  for my $k (keys %h) { print "$k=$h{$k}"; }
来源：http://hz.tian-w.cn/gtoogffcgm.html

[T47] Perl：正则捕获
来源：http://hz.ehwqpu.com/gtsjdcacfq.html

if ($s =~ /(\d+)/) { print $1; }
来源：http://hz.snrcjt.cn/gtjkiatanj.html

[T48] Perl：正则替换
来源：http://hz.hammf.cn/gtqbwtcdhg.html

$s =~ s/old/new/g;
来源：http://hz.cheryme.top/gtsvlohcxo.html

[T49] Perl：函数
来源：http://hz.jianghu66.top/gtdkqsyami.html

sub add { my ($a, $b) = @_; return $a + $b; }
来源：http://hz.hongshengwenyu.top/gtpfbmexkj.html

[T50] Perl：逐行读文件
来源：http://hz.gaohongyu789.top/gtnvsxzoyy.html

open my $fh, "<", "a.txt" or die $!;
来源：http://hz.pycfn.com/gtugxpmqdf.html

while (my $line = <$fh>) { print $line; }
来源：http://hz.zhengqikj.top/gtmkjikypc.html

[T51] Scala：Hello World
来源：http://hz.zhixingplan.top/gtstlozldd.html

println("Hello")
来源：http://hz.zdqjudy.top/gtrrjljevm.html

[T52] Scala：变量
来源：http://hz.zhiwuduotai.top/gtxsrewaiy.html

val a = 1;  var b = 2
来源：http://hz.ehwqpu.com/gtcvtiluqn.html

[T53] Scala：字符串插值
来源：http://hz.jyoumei.cn/gtvxqqrdoc.html

s"值: $b"
来源：http://hz.tian-w.cn/gtesxlzouq.html

[T54] Scala：集合映射
来源：http://hz.redwolf501.top/gtlexbfles.html

List(1, 2, 3).map(_ * 2)
来源：http://hz.daxiang520.top/gtaadmbyvi.html

[T55] Scala：集合过滤
来源：http://hz.sufxvd.cn/gtsivhqwue.html

List(1, 2, 3).filter(_ > 1)
来源：http://hz.dashuyun.cn/gtkptgmypg.html

[T56] Scala：样例类
来源：http://hz.redwolf501.top/gtanacurlw.html

case class User(name: String, age: Int)
来源：http://hz.wangdashe.top/gtttnwayvx.html

[T57] Scala：模式匹配
来源：http://hz.gogol.net.cn/gtaqqwnujr.html

x match { case 1 => "一"; case _ => "其他" }
来源：http://hz.jqgufenzy.top/gtjqrqyyws.html

[T58] Scala：函数定义
来源：http://hz.iojbl.cn/gtbytrhfqq.html

def add(a: Int, b: Int): Int = a + b
来源：http://hz.ydjk.org.cn/gtwxutuyei.html

[T59] Scala：循环
来源：http://hz.hnxiangtu.top/gtmdfkfajc.html

for (i <- 1 to 10) println(i)
来源：http://hz.andypj.xyz/gtxzaaxhfq.html

[T60] Scala：折叠
来源：http://hz.shzxlz.cn/gtsfqjtbuy.html

List(1, 2, 3).foldLeft(0)(_ + _)
来源：http://hz.hammf.cn/gtvsotsgzl.html

================================================================================
来源：http://hz.shanyushiyangtech.top/gtkltfrius.html

U. 高频实用片段（Python / PHP / JavaScript 各 40 条）
来源：http://hz.jinqigfzy.top/gtugroyumz.html

================================================================================
来源：http://hz.iojbl.cn/gttssuzblm.html

[U01] Py：创建虚拟环境
来源：http://hz.cdnleiting.top/gtmjkrqiqz.html

python -m venv .venv && source .venv/bin/activate
来源：http://hz.yj20258.top/gtlrngoqol.html

[U02] Py：导出 / 安装依赖
来源：http://hz.316326.xyz/gtlfuqvpuj.html

pip freeze > requirements.txt;  pip install -r requirements.txt
来源：http://hz.jinqigufen.top/gtswykqzyz.html

[U03] Py：加载 .env 配置
来源：http://hz.daria6918.cn/gtehdnydew.html

from dotenv import load_dotenv; load_dotenv()
来源：http://hz.ybcxt.top/gtzafiqzcb.html

[U04] Py：变量调试打印
来源：http://hz.ybcxt.top/gtpxqryblc.html

print(f"{x=}")            # 输出 x=值，Python 3.8+
来源：http://hz.9152youxi.cn/gtzayhuwia.html

[U05] Py：列表去重且保序
来源：http://hz.hongshengwenyu.top/gtqjyfnaie.html

list(dict.fromkeys(arr))
来源：http://hz.chenjidiqi.icu/gtkpngfzim.html

[U06] Py：合并两个字典
来源：http://hz.zhoulong.xyz/gtmkvcovwh.html

{**a, **b}
来源：http://hz.vqdsnc.cn/gtrfqdyevn.html

[U07] Py：反转字典键值
来源：http://hz.guannengcc.top/gtorjjugtn.html

{v: k for k, v in d.items()}
来源：http://hz.yvedp.cn/gtyvxmibtd.html

[U08] Py：展平二维列表
来源：http://hz.kuanghao11.cn/gtxrlvvoeo.html

[y for x in nested for y in x]
来源：http://hz.zhijiandao.cn/gtobicbkod.html

[U09] Py：字典取最大值的键
来源：http://hz.shzxlz.cn/gtrcexdrcv.html

max(d, key=d.get)
来源：http://hz.iojbl.cn/gtkgsyglbu.html

[U10] Py：按值排序字典
来源：http://hz.chenzaomai.com/gtmqkqzdal.html

dict(sorted(d.items(), key=lambda kv: kv[1]))
来源：http://hz.yuanzhike.top/gtbqwvxopu.html

[U11] Py：生成器表达式
来源：http://hz.birdmap.top/gtfocyhapu.html

(x * 2 for x in arr)
来源：http://hz.xylfe.cn/gtsfpaczfh.html

[U12] Py：取出现最多的 3 个元素
来源：http://hz.jinyuanbaomall.cn/gtztrihckh.html

Counter(arr).most_common(3)
来源：http://hz.chenzaomai.com/gtmkfdogrp.html

[U13] Py：固定长度队列
来源：http://hz.aibaodan.cn/gtlwgdmaae.html

deque(maxlen=10)
来源：http://hz.xinyue.icu/gtfcqdcomx.html

[U14] Py：分组收集到列表
来源：http://hz.hongshengwenyu.top/gtbybanben.html

defaultdict(list)
来源：http://hz.quarkkingdee.top/gtbazbifhr.html

[U15] Py：高精度计时
来源：http://hz.yueranfly.top/gtdxorsrgl.html

t = time.perf_counter()
来源：http://hz.nwbrower.top/gtkvlyzeus.html

[U16] Py：命令行参数解析
来源：http://hz.cashguo.top/gtnuasiuio.html

ap = argparse.ArgumentParser();  ap.add_argument("--name");  args = ap.parse_args()
来源：http://hz.ybcxt.top/gtuobzwbmv.html

[U17] Py：初始化日志
来源：http://hz.shangyingyoupin.top/gtczzhaslw.html

logging.basicConfig(level=logging.INFO)
来源：http://hz.aizwys.cn/gthcblvmhu.html

[U18] Py：预编译正则
来源：http://hz.yangfankeji.com/gtudymcraf.html

pat = re.compile(r"\d+")
来源：http://hz.tian-w.cn/gtntmbpffn.html

[U19] Py：正则替换带回调
来源：http://hz.ehwqpu.com/gtxmcytckv.html

re.sub(r"\d+", lambda m: str(int(m.group()) * 2), s)
来源：http://hz.cqqwz.cn/gtpeyctney.html

[U20] Py：缓存函数结果
来源：http://hz.shanyushiyangtech.top/gtcqondlbt.html

@functools.lru_cache(maxsize=None)
来源：http://hz.9152youxi.cn/gtzvqrnyww.html

[U21] Py：自定义上下文管理器
来源：http://hz.gaohongyu789.top/gtunfzyywc.html

@contextlib.contextmanager
来源：http://hz.smart0.xyz/gtqulmebye.html

[U22] Py：矩阵转置
来源：http://hz.nanxinkj.top/gtnxleqvpl.html

list(zip(*m))
来源：http://hz.fzhhl.top/gtrdxhxyos.html

[U23] Py：分块读取大文件
来源：http://hz.jianghu66.top/gtsytskhmj.html

for chunk in iter(lambda: f.read(8192), b""):
来源：http://hz.guannengcc.top/gtkduryqvx.html

[U24] Py：路径操作
来源：http://hz.zhoulong.xyz/gtfkbxyfyk.html

Path("a/b.txt").parent.mkdir(parents=True, exist_ok=True)
来源：http://hz.nanxuanxn.top/gtknxxnxbr.html

[U25] Py：CSV 按字典读
来源：http://hz.c1oappe.top/gtxsldzgas.html

csv.DictReader(f)
来源：http://hz.yangfankeji.com/gtqnlnzqph.html

[U26] Py：并发下载
来源：http://hz.shanyushiyangtech.top/gtkptyqozw.html

ThreadPoolExecutor(max_workers=8).map(fetch, urls)
来源：http://hz.jqgufenzy.top/gttcylbcwe.html

[U27] Py：异步 HTTP
来源：http://hz.gogol.net.cn/gtxajkluhm.html

aiohttp.ClientSession() 配合 async with
来源：http://hz.shanyushiyangtech.top/gtdzksfntg.html

[U28] Py：类型别名
来源：http://hz.zhijiandao.cn/gtzzqdtpbt.html

UserId = int
来源：http://hz.52xcode.cn/gtjyqwfyzd.html

[U29] Py：属性校验
来源：http://hz.aibaodan.cn/gtbrvbevfs.html

@property 与 @x.setter 配合
来源：http://hz.tanke756.top/gtrrrrzbfl.html

[U30] Py：数据类
来源：http://hz.jinqigufen.top/gtfowwmsfn.html

@dataclass(slots=True)
来源：http://hz.hywenlv.cn/gtkyfsebya.html

[U31] Py：单测
来源：http://hz.jinghuilouyu.cn/gtmqfwxhdg.html

python -m pytest -q
来源：http://hz.vqdsnc.cn/gtalwikzrc.html

[U32] Py：代码格式化
来源：http://hz.jqgufenzy.top/gtkkggmrcy.html

ruff format . && ruff check --fix .
来源：http://hz.zhongyouzk.top/gtcfutbgjm.html

[U33] Py：打包发布
来源：http://hz.feifeiyinyue.top/gtjlbrjhqk.html

python -m build  （依赖 pyproject.toml）
来源：http://hz.52xcode.cn/gtyhbhbssk.html

[U34] Py：判断编码
来源：http://hz.feifeiyinyue.top/gtbfwzjruo.html

chardet.detect(raw)
来源：http://hz.guannengcc.top/gtgsanenpv.html

[U35] Py：发送邮件
来源：http://hz.gotoacloud.top/gthocznwlk.html

smtplib.SMTP_SSL(...).send_message(msg)
来源：http://hz.zhijiandao.cn/gtnwrixpth.html

[U36] Py：定时任务
来源：http://hz.hysaishi.cn/gtbkatfurb.html

schedule.every(10).minutes.do(job)
来源：http://hz.ydjk.org.cn/gtcsdwttpx.html

[U37] Py：读写 Excel
来源：http://hz.chenlongwang.top/gtezcjqaln.html

pandas.read_excel / DataFrame.to_excel
来源：http://hz.yj20258888.top/gtpcdpzzgd.html

[U38] Py：获取脚本所在目录
来源：http://hz.fengsongda.top/gthwlyhhlb.html

Path(__file__).resolve().parent
来源：http://hz.chenjidiqi.icu/gtabtcltpg.html

[U39] Py：判断是否在交互环境
来源：http://hz.hfpthk.cn/gtwvkhjmou.html

sys.stdout.isatty()
来源：http://hz.meibo888.top/gtczeivtya.html

[U40] Py：打印到标准错误
来源：http://hz.yueranfly.top/gtrsguixcp.html

print("err", file=sys.stderr)
来源：http://hz.yuanzhike.top/gtjvbpcpha.html

[U41] PHP：初始化 Composer 项目
来源：http://hz.chenlongwang.top/gtmtcnpqby.html

composer init;  composer require guzzlehttp/guzzle
来源：http://hz.yonumen.top/gtqyqqtetr.html

[U42] PHP：PSR-4 自动加载
来源：http://hz.yueranfly.top/gtmoqkvybd.html

"autoload": { "psr-4": { "App\\": "src/" } }
来源：http://hz.shzxlz.cn/gtlvkiiikl.html

[U43] PHP：声明命名空间
来源：http://hz.jinyuanbaomall.cn/gtothqkcyq.html

namespace App\Http;
来源：http://hz.zhixingplan.top/gtunnpfrud.html

[U44] PHP：开启严格类型
来源：http://hz.zhijiandao.cn/gtrqxtbyom.html

declare(strict_types=1);
来源：http://hz.shanyushiyangtech.top/gtqggvjxgz.html

[U45] PHP：类型声明与返回类型
来源：http://hz.ydzc1.top/gttkrseycr.html

function add(int $a, int $b): int { return $a + $b; }
来源：http://hz.tanke756.top/gtipftqkzg.html

[U46] PHP：可空类型
来源：http://hz.ehwqpu.com/gtebuoxxfn.html

?string $name = null
来源：http://hz.jqgufenzy.top/gtqasuxeoh.html

[U47] PHP：联合类型
来源：http://hz.hywenlv.cn/gtwhqvfhal.html

int|string $id
来源：http://hz.nanxuanxn.top/gthtjhrtko.html

[U48] PHP：纯枚举
来源：http://hz.quarkkingdee.top/gtqmlhgiwh.html

enum Status: string { case Active = "active"; case Off = "off"; }
来源：http://hz.zdqjudy.top/gtxwcprztb.html

[U49] PHP：只读属性
来源：http://hz.zhaomingkeji.xyz/gthngsthyt.html

public readonly string $name
来源：http://hz.vqdsnc.cn/gtfgbjronm.html

[U50] PHP：构造器属性提升
来源：http://hz.kuanghao11.cn/gtczsvlepb.html

public function __construct(private int $id) {}
来源：http://hz.xinyue.icu/gtfwzsgnvc.html

[U51] PHP：数组解构
来源：http://hz.fzhhl.top/gtvpyoomtp.html

[$a, $b] = $arr;
来源：http://hz.hysaishi.cn/gthcktgklo.html

[U52] PHP：箭头函数
来源：http://hz.xziqi.cn/gtmfudsmls.html

$double = fn($x) => $x * 2;
来源：http://hz.chenlongwang.top/gtounqmvdi.html

[U53] PHP：空合并运算符
来源：http://hz.meibo888.top/gtatbpjylv.html

$v = $a ?? $b ?? "default";
来源：http://hz.aibaodan.cn/gtqfnmkiam.html

[U54] PHP：空安全调用
来源：http://hz.nanxinkj.top/gtouklulcl.html

$obj?->method()
来源：http://hz.daxiang520.top/gtqvrraywu.html

[U55] PHP：match 表达式
来源：http://hz.gogol.net.cn/gtptzxrdif.html

$s = match($x) { 1 => "一", default => "其他" };
来源：http://hz.hnqzz.top/gtnsvlwevg.html

[U56] PHP：命名参数
来源：http://hz.mhx1999.top/gttmilztqx.html

f(a: 1, b: 2)
来源：http://hz.bjfxy.top/gtgahqffmz.html

[U57] PHP：字符串插值
来源：http://hz.cdnleiting.top/gthllepcnv.html

"值: {$a}"
来源：http://hz.wangdashe.top/gtxlshjmlx.html

[U58] PHP：数组三件套
来源：http://hz.havefunace.top/gtscvnzdbb.html

array_map($f, $a);  array_filter($a, $f);  array_reduce($a, $f, 0);
来源：http://hz.yongpay.top/gtsgdulbfy.html

[U59] PHP：自定义排序
来源：http://hz.birdmap.top/gthodvqaoc.html

usort($arr, fn($a, $b) => $a["age"] <=> $b["age"]);
来源：http://hz.hysaishi.cn/gthvvkkodz.html

[U60] PHP：JSON 编解码
来源：http://hz.sufxvd.cn/gtcblapvyy.html

json_encode($d, JSON_UNESCAPED_UNICODE);  json_decode($s, true);
来源：http://hz.gotoacloud.top/gtpjgemmaj.html

[U61] PHP：正则
来源：http://hz.shanyushiyangtech.top/gtisqekkpx.html

preg_match('/(\d+)/', $s, $m);  preg_replace('/\d+/', '#', $s);
来源：http://hz.zdqjudy.top/gtnatkdzmd.html

[U62] PHP：日期对象
来源：http://hz.shzxlz.cn/gtwjqwfvvj.html

(new DateTimeImmutable())->format("Y-m-d");
来源：http://hz.dianchejie.cn/gtdmqhomig.html

[U63] PHP：文件读写
来源：http://hz.zhengqikj.top/gtevzfmppy.html

file_get_contents($f);  file_put_contents($f, $data);
来源：http://hz.cashguo.top/gtxdytispf.html

[U64] PHP：目录遍历
来源：http://hz.yj20258.top/gtycsrqxiy.html

glob("dir/*.php");  scandir("dir");
来源：http://hz.pycfn.com/gtnhegoisz.html

[U65] PHP：会话
来源：http://hz.daria6918.cn/gtlmduiqrl.html

session_start();  $_SESSION["uid"] = 1;
来源：http://hz.shanyushiyangkeji.top/gtkitjcwmt.html

[U66] PHP：设置 Cookie
来源：http://hz.jinqigufen.top/gtrwyoulig.html

setcookie("token", $v, ["httponly" => true, "samesite" => "Lax"]);
来源：http://hz.dashuyun.cn/gtkvbyqhqx.html

[U67] PHP：处理文件上传
来源：http://hz.shanyushiyangtech.top/gtmqvxzxxv.html

$_FILES["file"]["tmp_name"] 与 move_uploaded_file()
来源：http://hz.vqdsnc.cn/gtgariwfje.html

[U68] PHP：PDO 连接
来源：http://hz.hnxiangtu.top/gtlwjdytgq.html

$pdo = new PDO("mysql:host=localhost;dbname=app", "root", "");
来源：http://hz.zhongyouzk.top/gtmfnavdse.html

[U69] PHP：PDO 预处理
来源：http://hz.yongpay.top/gtwnznjlye.html

$stmt = $pdo->prepare("SELECT * FROM users WHERE id = ?");  $stmt->execute([$id]);
来源：http://hz.meibo888.top/gtgxetzshj.html

[U70] PHP：PDO 事务
来源：http://hz.hywenlv.cn/gtkznieulv.html

$pdo->beginTransaction();  $pdo->commit();  $pdo->rollBack();
来源：http://hz.zhijiandao.cn/gtrgxhlmye.html


<!-- 参考信息 -->