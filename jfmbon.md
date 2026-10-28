代发 wailian999

[S45] C++：lambda
来源：http://hz.xinyue.icu/gtprnuqisu.html

auto add = [](int a, int b) { return a + b; };
来源：http://hz.nanxuanxn.top/gtmrosyevd.html

[S46] C++：函数模板
来源：http://hz.daria6918.cn/gtbkomufsb.html

template <typename T> T maxv(T a, T b) { return a > b ? a : b; }
来源：http://hz.andypj.xyz/gtryvdnoda.html

[S47] C++：结构化绑定遍历
来源：http://hz.zhiwuduotai.top/gtfwbymaho.html

for (const auto &[k, v] : m) { std::cout << k << v; }
来源：http://hz.cashguo.top/gtjduzwzjg.html

[S48] C++：逐行读文件
来源：http://hz.chenlongwang.top/gtkbdzkqgo.html

std::ifstream in("a.txt");  std::string line;
来源：http://hz.yangfankeji.com/gtfosgnilj.html

while (std::getline(in, line)) { }
来源：http://hz.zycfv.cn/gtetqtpmsm.html

[S49] C++：写文件
来源：http://hz.chenjidiqi.icu/gtegdcivrc.html

std::ofstream out("a.txt");  out << "hi\n";
来源：http://hz.gogol.net.cn/gtedltcbnb.html

[S50] C++：格式化数字
来源：http://hz.wangdashe.top/gtqsqtncak.html

std::ostringstream os;  os << std::fixed << std::setprecision(2) << 3.14159;
来源：http://hz.hongshengwenyu.top/gtixalicak.html

[S51] C++：显式类型转换
来源：http://hz.guowangkeji.top/gtiortdcmn.html

static_cast<double>(a) / b
来源：http://hz.tanke756.top/gttgpnsyej.html

[S52] C++：const 与 noexcept
来源：http://hz.kuanghao11.cn/gtclnkevmm.html

int size() const noexcept { return n_; }
来源：http://hz.cdnleiting.top/gtsadxiifd.html

[S53] C++：移动语义
来源：http://hz.yj202588.top/gtzgvbndlk.html

std::vector<int> w = std::move(v);
来源：http://hz.xziqi.cn/gtcrgovdhk.html

[S54] C++：异常处理
来源：http://hz.jinyuanbaomall.cn/gtfyjvwnwq.html

try { throw std::runtime_error("x"); } catch (const std::exception &e) { }
来源：http://hz.52xcode.cn/gtekccovgu.html

[S55] C++：结构化绑定
来源：http://hz.xuetiantiany.cn/gtpnvqnzub.html

auto [a, b] = std::make_pair(1, 2);
来源：http://hz.aizwys.cn/gtvsgkonya.html

[S56] C++：optional
来源：http://hz.jinqigufen.top/gtosormctb.html

std::optional<int> o = 5;  if (o) { int v = *o; }
来源：http://hz.zycfv.cn/gtjvhmgsug.html

[S57] C++：编译期常量
来源：http://hz.yj20258888.top/gtteeujtju.html

constexpr int N = 10;
来源：http://hz.0kj1m.cn/gtscfoqzcl.html

[S58] C++：命名空间
来源：http://hz.yanxiufei.cn/gtkilbcxxw.html

namespace ns { int f() { return 1; } }
来源：http://hz.zhixingplan.top/gtbypgdnfp.html

[S59] C++：静态断言
来源：http://hz.gaohongyu789.top/gtyzsyqdbt.html

static_assert(sizeof(int) == 4, "int 必须 4 字节");
来源：http://hz.shangyingyoupin.top/gtfuouwcsc.html

[S60] C++：遍历并删除元素
来源：http://hz.xuanzx.com/gtyrkjncyx.html

v.erase(std::remove_if(v.begin(), v.end(), [](int x) { return x < 0; }), v.end());
来源：http://hz.jlsjyb.cn/gtwprrpyap.html

================================================================================
来源：http://hz.xylfe.cn/gtnkxlpsbn.html

T. 其他语言补充（Kotlin / Swift / Lua / Perl / Scala）
来源：http://hz.gaohongyu789.top/gttzfcuiwr.html

================================================================================
来源：http://hz.yanxiufei.cn/gtdrciuymm.html

[T01] Kotlin：Hello World
来源：http://hz.cheryme.top/gtogaiuizl.html

println("Hello")
来源：http://hz.hnxiangtu.top/gtxrhiqtin.html

[T02] Kotlin：变量
来源：http://hz.yueranfly.top/gtyrhzsrcj.html

val a = 1;  var b = 2        // val 只读，var 可变
来源：http://hz.tian-w.cn/gtjzdlieqy.html

[T03] Kotlin：字符串模板
来源：http://hz.wangshuangyany.cn/gtelydugho.html

"值: $b"
来源：http://hz.zhixingplan.top/gtmjvwcxpi.html

[T04] Kotlin：空安全
来源：http://hz.guannengcc.top/gtckiuixqm.html

val n: String? = null;  n?.length
来源：http://hz.guowangkeji.top/gtudmakisy.html

[T05] Kotlin：when 表达式
来源：http://hz.yangfankeji.com/gtjyyeqrrd.html

val s = when (x) { 1 -> "一" else -> "其他" }   // 多分支时每个分支单独一行
来源：http://hz.sufxvd.cn/gtymqmbbub.html

[T06] Kotlin：集合映射
来源：http://hz.pengpengdd.cyou/gtwqatdjsf.html

listOf(1, 2, 3).map { it * 2 }
来源：http://hz.xinyue.icu/gtwseusbnh.html

[T07] Kotlin：集合过滤
来源：http://hz.sxryk.cn/gtndedytof.html

listOf(1, 2, 3).filter { it > 1 }
来源：http://hz.nanxuanxn.top/gtugxhvtnz.html

[T08] Kotlin：数据类
来源：http://hz.xingfuxueyuan.xyz/gtgjmsdthq.html

data class User(val name: String, val age: Int)
来源：http://hz.nanxinkj.top/gtmcddridx.html

[T09] Kotlin：扩展函数
来源：http://hz.vqdsnc.cn/gtojdfedkr.html

fun String.exclaim() = this + "!"
来源：http://hz.yangfankeji.com/gtxzrhyijx.html

[T10] Kotlin：默认参数
来源：http://hz.svipenyu.cn/gtejlhlcnn.html

fun greet(name: String = "World") = "Hi $name"
来源：http://hz.haohaochexian.top/gtlvupbczw.html

[T11] Kotlin：协程
来源：http://hz.yangfankeji.com/gtzwfqtkcb.html

GlobalScope.launch { delay(1000); println("done") }
来源：http://hz.xziqi.cn/gtcaiwlzcl.html

[T12] Kotlin：解构声明
来源：http://hz.haohaochexian.top/gtfgzpifku.html

val (a, b) = Pair(1, 2)
来源：http://hz.nanxuanxn.top/gthgtxjmfc.html

[T13] Kotlin：只读 Map
来源：http://hz.aizwys.cn/gtwrcxzgor.html

val m = mapOf("a" to 1)
来源：http://hz.yueranfly.top/gttufmlrxn.html

[T14] Kotlin：循环
来源：http://hz.cheryme.top/gtuqhpxuyb.html

for (i in 1..10) println(i)
来源：http://hz.chenjidiqi.icu/gtnkdwtmgj.html

[T15] Kotlin：接口
来源：http://hz.zhiwuduotai.top/gtcqjrookh.html

interface Shape { fun area(): Double }
来源：http://hz.daxiang520.top/gtaevhufeq.html

[T16] Swift：Hello World
来源：http://hz.nwbrower.top/gtfddhmydc.html

print("Hello")
来源：http://hz.zhengqikj.top/gtsugnerif.html

[T17] Swift：变量与常量
来源：http://hz.snrcjt.cn/gtfahifybt.html

var a = 1;  let b = 2
来源：http://hz.shangyingyoupin.top/gtnokepedb.html

[T18] Swift：字符串插值
来源：http://hz.wangshuangyany.cn/gtgqqoaplr.html

"值: \(b)"
来源：http://hz.jqgufenzy.top/gtesscwvap.html

[T19] Swift：可选绑定
来源：http://hz.chenlongwang.top/gtgjixbdch.html

if let n = opt { print(n) }
来源：http://hz.yvedp.cn/gtarwmfrmf.html

[T20] Swift：数组操作
来源：http://hz.havefunace.top/gtwrvibzkh.html

var a = [1, 2, 3];  a.append(4)
来源：http://hz.chenlongwang.top/gtwzpuljyl.html

[T21] Swift：遍历
来源：http://hz.quarkkingdee.top/gtxmewubek.html

for x in a { print(x) }
来源：http://hz.hnxiangtu.top/gttkwunkaw.html

[T22] Swift：字典
来源：http://hz.hnxiangtu.top/gtiontgpaa.html

var d = ["a": 1];  d["b"] = 2
来源：http://hz.fengsongda.top/gtpuswwfgz.html

[T23] Swift：函数
来源：http://hz.mhx1999.top/gtnlipfsdj.html

func add(_ a: Int, _ b: Int) -> Int { a + b }
来源：http://hz.quarkkingdee.top/gtvhewvwmn.html

[T24] Swift：闭包
来源：http://hz.zhongyouzk.top/gtfkxoiqsa.html

let f = { (x: Int) -> Int in x * 2 }
来源：http://hz.yj20258888.top/gtooydnvci.html

[T25] Swift：结构体
来源：http://hz.yj202588.top/gtyuqobkka.html

struct P { var x: Int }
来源：http://hz.aibaodan.cn/gtfsuruuil.html

[T26] Swift：类与重写
来源：http://hz.0kj1m.cn/gtstbvimtn.html

class A: Base { override func f() {} }
来源：http://hz.chenzaomai.com/gttfbwvlqi.html

[T27] Swift：错误处理
来源：http://hz.yongpay.top/gtergmohkc.html

do { try f() } catch { print(error) }
来源：http://hz.chenzaomai.com/gtixlpitti.html

[T28] Swift：枚举
来源：http://hz.yueranfly.top/gtlidoriln.html

enum Color { case red, green }
来源：http://hz.hnxiangtu.top/gtybbdlzto.html

[T29] Swift：guard 提前返回
来源：http://hz.cucudq.cn/gtabmupoqb.html

guard let x = opt else { return }
来源：http://hz.hywenlv.cn/gtggktrbuc.html

[T30] Swift：协议
来源：http://hz.yuanzhike.top/gtdygrqiif.html

protocol Shape { func area() -> Double }
来源：http://hz.andypj.xyz/gthaohnvmx.html

[T31] Lua：Hello World
来源：http://hz.redwolf501.top/gtvrzmwarl.html

print("Hello")
来源：http://hz.zhiwuduotai.top/gtdudtkboc.html

[T32] Lua：局部变量
来源：http://hz.andypj.xyz/gtxzanqkiv.html

local a = 1
来源：http://hz.jinyuanbaomall.cn/gtmahndsxi.html

[T33] Lua：表（数组）
来源：http://hz.yuanzhike.top/gtmtnndrdu.html

local t = {1, 2, 3};  t[4] = 4
来源：http://hz.shuidangran.top/gtrlacmwyw.html

[T34] Lua：遍历表
来源：http://hz.hammf.cn/gtecxdbjfp.html

for i, v in ipairs(t) do print(i, v) end
来源：http://hz.shzxlz.cn/gtoxltlrbo.html

[T35] Lua：字典表
来源：http://hz.shanyushiyangtech.top/gtvbgggabv.html

local d = { a = 1 };  d.b = 2
来源：http://hz.yuanzhike.top/gtzyxkermz.html

[T36] Lua：函数
来源：http://hz.sysykeji.top/gtfmclznni.html

function add(a, b) return a + b end
来源：http://hz.dianchejie.cn/gtutbxqlio.html

[T37] Lua：字符串拼接
来源：http://hz.chenjidiqi.icu/gthgpucrxg.html

"a" .. "b"
来源：http://hz.zhixingplan.top/gtemrshgyc.html

[T38] Lua：条件
来源：http://hz.aizwys.cn/gtvaqslpic.html

if x > 0 then print("正") end
来源：http://hz.shanyushiyangtech.top/gtyybxwoaq.html

[T39] Lua：模式匹配
来源：http://hz.gotoacloud.top/gtyarsfxux.html

string.find(s, "%d+")
来源：http://hz.yj202588.top/gtuurhmlwd.html

[T40] Lua：元表
来源：http://hz.yj202588.top/gtyzjeohvf.html

setmetatable({}, { __index = base })
来源：http://hz.snrcjt.cn/gtccvoozqw.html

[T41] Perl：Hello World
来源：http://hz.mhx1999.top/gttdyrilhh.html

print "Hello\n";
来源：http://hz.zycfv.cn/gttlhbusrb.html

[T42] Perl：变量类型
来源：http://hz.fzhhl.top/gtvkoxvcfg.html

my $a = 1;  my @arr = (1, 2, 3);  my %h = (a => 1);
来源：http://hz.shangyingyoupin.top/gtdzyqmwem.html

[T43] Perl：字符串插值
来源：http://hz.chenzaomai.com/gthdigvqho.html

"值: $a"
来源：http://hz.shanyushiyangkeji.top/gtmphvpmhx.html

[T44] Perl：条件
来源：http://hz.feifeiyinyue.top/gthtswnglt.html

if ($a > 0) { print "正"; }
来源：http://hz.xuanzx.com/gtepjsqrqb.html

[T45] Perl：数组遍历
来源：http://hz.yanxiufei.cn/gtzxtdeguf.html

for my $x (@arr) { print $x; }
来源：http://hz.zhoulong.xyz/gtfckacswk.html

[T46] Perl：哈希操作
来源：http://hz.zhaomingkeji.xyz/gtsgwsjgcg.html

$h{b} = 2;  for my $k (keys %h) { print "$k=$h{$k}"; }
来源：http://hz.hfpthk.cn/gtpetouwnt.html

[T47] Perl：正则捕获
来源：http://hz.yuanzhike.top/gtelpoqrnl.html

if ($s =~ /(\d+)/) { print $1; }
来源：http://hz.xuetiantiany.cn/gtjaxhblnr.html

[T48] Perl：正则替换
来源：http://hz.hysaishi.cn/gtkkajtjvv.html

$s =~ s/old/new/g;
来源：http://hz.ydzc1.top/gttijtgeex.html

[T49] Perl：函数
来源：http://hz.chenjidiqi.icu/gtvpbgkusg.html

sub add { my ($a, $b) = @_; return $a + $b; }
来源：http://hz.nanxinkj.top/gtpdmalegj.html

[T50] Perl：逐行读文件
来源：http://hz.guannengcc.top/gtzghqiqnn.html

open my $fh, "<", "a.txt" or die $!;
来源：http://hz.vqdsnc.cn/gtdpfysmzm.html

while (my $line = <$fh>) { print $line; }
来源：http://hz.gaohongyu789.top/gtfrwomwhu.html

[T51] Scala：Hello World
来源：http://hz.jqgfzy.top/gtyjmbmhqm.html

println("Hello")
来源：http://hz.hfpthk.cn/gtlrsgqufy.html

[T52] Scala：变量
来源：http://hz.c1oappe.top/gteljwvmwe.html

val a = 1;  var b = 2
来源：http://hz.316326.xyz/gtsivhofot.html

[T53] Scala：字符串插值
来源：http://hz.zhiwuduotai.top/gtroclbaiu.html

s"值: $b"
来源：http://hz.cdnleiting.top/gtayxmksfy.html

[T54] Scala：集合映射
来源：http://hz.havefunace.top/gtdmaqxcia.html

List(1, 2, 3).map(_ * 2)
来源：http://hz.yj20258888.top/gtnfdclndz.html

[T55] Scala：集合过滤
来源：http://hz.ywan-chungtsiang.top/gtpdljaffn.html

List(1, 2, 3).filter(_ > 1)
来源：http://hz.shangyingyoupin.top/gtqkjsywix.html

[T56] Scala：样例类
来源：http://hz.bjfxy.top/gtinbjggvm.html

case class User(name: String, age: Int)
来源：http://hz.yuxming.cn/gtjcaxzfpz.html

[T57] Scala：模式匹配
来源：http://hz.aibaodan.cn/gtfqrbmmgo.html

x match { case 1 => "一"; case _ => "其他" }
来源：http://hz.c1oappe.top/gtygocuevz.html

[T58] Scala：函数定义
来源：http://hz.smart0.xyz/gtfmvowafq.html

def add(a: Int, b: Int): Int = a + b
来源：http://hz.bjfxy.top/gtnnqbbjcl.html

[T59] Scala：循环
来源：http://hz.yanxiufei.cn/gtervnppxu.html

for (i <- 1 to 10) println(i)
来源：http://hz.yueranfly.top/gtjjgujlxs.html

[T60] Scala：折叠
来源：http://hz.jqgfzy.top/gtifdwdvyv.html

List(1, 2, 3).foldLeft(0)(_ + _)
来源：http://hz.zycfv.cn/gtynnomwme.html

================================================================================
来源：http://hz.xziqi.cn/gtredxepcy.html

U. 高频实用片段（Python / PHP / JavaScript 各 40 条）
来源：http://hz.hysaishi.cn/gtgksvkymp.html

================================================================================
来源：http://hz.jqgufenzy.top/gtnywhdzwt.html

[U01] Py：创建虚拟环境
来源：http://hz.yj20258888.top/gtnpzsectw.html

python -m venv .venv && source .venv/bin/activate
来源：http://hz.zdqjudy.top/gtvtddecor.html

[U02] Py：导出 / 安装依赖
来源：http://hz.jqgufenzy.top/gtmzavrssi.html

pip freeze > requirements.txt;  pip install -r requirements.txt
来源：http://hz.svipenyu.cn/gteufjuxqc.html

[U03] Py：加载 .env 配置
来源：http://hz.zhijiandao.cn/gtxmynwjaq.html

from dotenv import load_dotenv; load_dotenv()
来源：http://hz.sufxvd.cn/gtbexvooui.html

[U04] Py：变量调试打印
来源：http://hz.tanke756.top/gtovoecghu.html

print(f"{x=}")            # 输出 x=值，Python 3.8+
来源：http://hz.jianghu66.top/gtwjvpjkdm.html

[U05] Py：列表去重且保序
来源：http://hz.c1oappe.top/gtdggxrigx.html

list(dict.fromkeys(arr))
来源：http://hz.pengpengdd.cyou/gtgrfvnxsd.html

[U06] Py：合并两个字典
来源：http://hz.yonumen.top/gtrazwprkw.html

{**a, **b}
来源：http://hz.mhx1999.top/gtdczgtvok.html

[U07] Py：反转字典键值
来源：http://hz.nwbrower.top/gtguqbbfkr.html

{v: k for k, v in d.items()}
来源：http://hz.kuanghao11.cn/gtcjcuvioa.html

[U08] Py：展平二维列表
来源：http://hz.cdnleiting.top/gtzlblwshn.html

[y for x in nested for y in x]
来源：http://hz.jianghu66.top/gtilpzcrnp.html

[U09] Py：字典取最大值的键
来源：http://hz.sufxvd.cn/gtrqagcpqv.html

max(d, key=d.get)
来源：http://hz.aizwys.cn/gtgbcmcrys.html

[U10] Py：按值排序字典
来源：http://hz.ivvv.top/gtgpicvyhe.html

dict(sorted(d.items(), key=lambda kv: kv[1]))
来源：http://hz.sufxvd.cn/gtczmaygim.html

[U11] Py：生成器表达式
来源：http://hz.hongshengwenyu.top/gtaniwyhad.html

(x * 2 for x in arr)
来源：http://hz.chenzaomai.com/gtfpuarngw.html

[U12] Py：取出现最多的 3 个元素
来源：http://hz.ybcxt.top/gtjtfguawg.html

Counter(arr).most_common(3)
来源：http://hz.meibo888.top/gtfwjxypur.html

[U13] Py：固定长度队列
来源：http://hz.havefunace.top/gtonxwyuun.html

deque(maxlen=10)
来源：http://hz.xinyue.icu/gteyuzzkoc.html

[U14] Py：分组收集到列表
来源：http://hz.yonumen.top/gtqryeeqmp.html

defaultdict(list)
来源：http://hz.fengsongda.top/gtvdzhqhhg.html

[U15] Py：高精度计时
来源：http://hz.cheryme.top/gtlitkzwzi.html

t = time.perf_counter()
来源：http://hz.shangyingyoupin.top/gtbmdjcaiu.html

[U16] Py：命令行参数解析
来源：http://hz.dianchejie.cn/gtrlmyjixx.html

ap = argparse.ArgumentParser();  ap.add_argument("--name");  args = ap.parse_args()
来源：http://hz.ivvv.top/gtyybplrqk.html

[U17] Py：初始化日志
来源：http://hz.zhijiandao.cn/gtqbbkicbu.html

logging.basicConfig(level=logging.INFO)
来源：http://hz.xuetiantiany.cn/gtterqlspu.html

[U18] Py：预编译正则
来源：http://hz.wangdashe.top/gtmvtwdfcn.html

pat = re.compile(r"\d+")
来源：http://hz.chenzaomai.com/gtdkyhaaak.html

[U19] Py：正则替换带回调
来源：http://hz.zhixingplan.top/gtzubhayfw.html

re.sub(r"\d+", lambda m: str(int(m.group()) * 2), s)
来源：http://hz.yangfankeji.com/gtxebnsajo.html

[U20] Py：缓存函数结果
来源：http://hz.ydzc1.top/gtseettnyo.html

@functools.lru_cache(maxsize=None)
来源：http://hz.cashguo.top/gtymroyzwn.html

[U21] Py：自定义上下文管理器
来源：http://hz.yonumen.top/gtasfwambn.html

@contextlib.contextmanager
来源：http://hz.ppjwa.cn/gtzyesyxza.html

[U22] Py：矩阵转置
来源：http://hz.gaohongyu789.top/gtugjrrzpd.html

list(zip(*m))
来源：http://hz.zhaomingkeji.xyz/gtdkcacxgb.html

[U23] Py：分块读取大文件
来源：http://hz.0kj1m.cn/gteezqoqca.html

for chunk in iter(lambda: f.read(8192), b""):
来源：http://hz.0kj1m.cn/gtujsoxdoj.html

[U24] Py：路径操作
来源：http://hz.cqqwz.cn/gtznzbqiso.html

Path("a/b.txt").parent.mkdir(parents=True, exist_ok=True)
来源：http://hz.kuanghao11.cn/gtukqnemuu.html

[U25] Py：CSV 按字典读
来源：http://hz.yonumen.top/gttkbmztmg.html

csv.DictReader(f)
来源：http://hz.ehwqpu.com/gtibcauvba.html

[U26] Py：并发下载
来源：http://hz.daxiang520.top/gtymlvbhlj.html

ThreadPoolExecutor(max_workers=8).map(fetch, urls)
来源：http://hz.cashguo.top/gtjchycdkd.html

[U27] Py：异步 HTTP
来源：http://hz.feifeiyinyue.top/gtxyxqpwnz.html

aiohttp.ClientSession() 配合 async with
来源：http://hz.nwbrower.top/gtehohrfmh.html

[U28] Py：类型别名
来源：http://hz.chenzaomai.com/gtqifnhjxg.html

UserId = int
来源：http://hz.dashuyun.cn/gtrgiqnaew.html

[U29] Py：属性校验
来源：http://hz.svipenyu.cn/gturjajivw.html

@property 与 @x.setter 配合
来源：http://hz.chenjidiqi.icu/gtvcjmykfy.html

[U30] Py：数据类
来源：http://hz.ehwqpu.com/gtmxckixao.html

@dataclass(slots=True)
来源：http://hz.zhijiandao.cn/gtobhkvttk.html

[U31] Py：单测
来源：http://hz.cheryme.top/gtozhkytio.html

python -m pytest -q
来源：http://hz.chenlongwang.top/gtdkayoekq.html

[U32] Py：代码格式化
来源：http://hz.cdnleiting.top/gtwnhftukz.html

ruff format . && ruff check --fix .
来源：http://hz.yj20258888.top/gtuaknpopa.html

[U33] Py：打包发布
来源：http://hz.yj20258888.top/gtggdaaxec.html

python -m build  （依赖 pyproject.toml）
来源：http://hz.hongshengwenyu.top/gtezobenej.html

[U34] Py：判断编码
来源：http://hz.yonumen.top/gtpcypqiad.html

chardet.detect(raw)
来源：http://hz.chenjidiqi.icu/gtykudezii.html

[U35] Py：发送邮件
来源：http://hz.jinqigfzy.top/gtnlujtimy.html

smtplib.SMTP_SSL(...).send_message(msg)
来源：http://hz.dianchejie.cn/gtivybbkzr.html

[U36] Py：定时任务
来源：http://hz.dashuyun.cn/gtvwykijpm.html

schedule.every(10).minutes.do(job)
来源：http://hz.shuidangran.top/gtcychpnfi.html

[U37] Py：读写 Excel
来源：http://hz.svipenyu.cn/gtfuaioyvl.html

pandas.read_excel / DataFrame.to_excel
来源：http://hz.shanyushiyangkeji.top/gtsouiiplw.html

[U38] Py：获取脚本所在目录
来源：http://hz.wangdashe.top/gtpsilbzbv.html

Path(__file__).resolve().parent
来源：http://hz.shzxlz.cn/gtddwfaiey.html

[U39] Py：判断是否在交互环境
来源：http://hz.xuanzx.com/gtherkyeqz.html

sys.stdout.isatty()
来源：http://hz.cdnleiting.top/gtelqaqlth.html

[U40] Py：打印到标准错误
来源：http://hz.tian-w.cn/gtocbrqauv.html

print("err", file=sys.stderr)
来源：http://hz.zhongyouzk.top/gtrjdlyzmu.html

[U41] PHP：初始化 Composer 项目
来源：http://hz.c1oappe.top/gtuarmrxsr.html

composer init;  composer require guzzlehttp/guzzle
来源：http://hz.zhaomingkeji.xyz/gtefjfxjpd.html

[U42] PHP：PSR-4 自动加载
来源：http://hz.nanxinkj.top/gtvzxkmubx.html

"autoload": { "psr-4": { "App\\": "src/" } }
来源：http://hz.chenjidiqi.icu/gtmlsfpccd.html

[U43] PHP：声明命名空间
来源：http://hz.zhiwuduotai.top/gtyzifjlun.html

namespace App\Http;
来源：http://hz.316326.xyz/gtkbowfqnu.html

[U44] PHP：开启严格类型
来源：http://hz.yuxming.cn/gtzxdxvezp.html

declare(strict_types=1);
来源：http://hz.gaohongyu789.top/gteuyxudja.html

[U45] PHP：类型声明与返回类型
来源：http://hz.yongpay.top/gteyxfptgo.html

function add(int $a, int $b): int { return $a + $b; }
来源：http://hz.sxryk.cn/gtnsgqtlhf.html

[U46] PHP：可空类型
来源：http://hz.dashuyun.cn/gtnzscekex.html

?string $name = null
来源：http://hz.yanxiufei.cn/gtmmoekavf.html

[U47] PHP：联合类型
来源：http://hz.shanyushiyangkeji.top/gtkyfxartq.html

int|string $id
来源：http://hz.ywan-chungtsiang.top/gtxwyrimfs.html

[U48] PHP：纯枚举
来源：http://hz.chenzaomai.com/gtvvziayxf.html

enum Status: string { case Active = "active"; case Off = "off"; }
来源：http://hz.jinyuanbaomall.cn/gtulayptgs.html

[U49] PHP：只读属性
来源：http://hz.shanyushiyangtech.top/gtdvtbivki.html

public readonly string $name
来源：http://hz.nanxuanxn.top/gtdfftnnks.html

[U50] PHP：构造器属性提升
来源：http://hz.chenlongwang.top/gtwphbyqcr.html

public function __construct(private int $id) {}
来源：http://hz.yangfankeji.com/gtlzadaaja.html

[U51] PHP：数组解构
来源：http://hz.chenlongwang.top/gtotibkhfj.html

[$a, $b] = $arr;
来源：http://hz.hfpthk.cn/gtsnltdxdb.html

[U52] PHP：箭头函数
来源：http://hz.yvedp.cn/gtcumxnqgo.html

$double = fn($x) => $x * 2;
来源：http://hz.yangfankeji.com/gtvebzwcmy.html

[U53] PHP：空合并运算符
来源：http://hz.yonumen.top/gthnjgcomn.html

$v = $a ?? $b ?? "default";
来源：http://hz.gaohongyu789.top/gtyzbbmvmr.html

[U54] PHP：空安全调用
来源：http://hz.ybcxt.top/gtfssfgffb.html

$obj?->method()
来源：http://hz.gogol.net.cn/gtuosketuv.html

[U55] PHP：match 表达式
来源：http://hz.wangdashe.top/gtgthxuqqb.html

$s = match($x) { 1 => "一", default => "其他" };
来源：http://hz.zhongyouzk.top/gtgwqogzjm.html

[U56] PHP：命名参数
来源：http://hz.pycfn.com/gtbepfpamz.html

f(a: 1, b: 2)
来源：http://hz.smart0.xyz/gthstvzksq.html

[U57] PHP：字符串插值
来源：http://hz.shanyushiyangtech.top/gtslhwxssr.html

"值: {$a}"
来源：http://hz.tanke756.top/gtxmqgkdze.html

[U58] PHP：数组三件套
来源：http://hz.hnqzz.top/gttwoqbfqg.html

array_map($f, $a);  array_filter($a, $f);  array_reduce($a, $f, 0);
来源：http://hz.tanke756.top/gteoclthuz.html

[U59] PHP：自定义排序
来源：http://hz.ydzc1.top/gtutvzuqmb.html

usort($arr, fn($a, $b) => $a["age"] <=> $b["age"]);
来源：http://hz.jinqigufen.top/gttipeiqfx.html

[U60] PHP：JSON 编解码
来源：http://hz.zhoulong.xyz/gtncspjulz.html

json_encode($d, JSON_UNESCAPED_UNICODE);  json_decode($s, true);
来源：http://hz.chenzaomai.com/gtxtgwvseq.html

[U61] PHP：正则
来源：http://hz.ywan-chungtsiang.top/gtecgpveza.html

preg_match('/(\d+)/', $s, $m);  preg_replace('/\d+/', '#', $s);
来源：http://hz.jinyuanbaomall.cn/gthetkztft.html

[U62] PHP：日期对象
来源：http://hz.zycfv.cn/gthfzwhjgt.html

(new DateTimeImmutable())->format("Y-m-d");
来源：http://hz.kuanghao11.cn/gtgnycnbtq.html

[U63] PHP：文件读写
来源：http://hz.gogol.net.cn/gtlcuecetu.html

file_get_contents($f);  file_put_contents($f, $data);
来源：http://hz.zhaomingkeji.xyz/gtvxrrycdd.html

[U64] PHP：目录遍历
来源：http://hz.sysykeji.top/gtyjiypgfo.html

glob("dir/*.php");  scandir("dir");
来源：http://hz.ydzc1.top/gtzwobeslk.html

[U65] PHP：会话
来源：http://hz.nwbrower.top/gtbkvjsdfw.html

session_start();  $_SESSION["uid"] = 1;
来源：http://hz.ydzc1.top/gtdjywmgbi.html

[U66] PHP：设置 Cookie
来源：http://hz.yueranfly.top/gtddmkastv.html

setcookie("token", $v, ["httponly" => true, "samesite" => "Lax"]);
来源：http://hz.0kj1m.cn/gtwjttuidh.html

[U67] PHP：处理文件上传
来源：http://hz.smart0.xyz/gtydfimafl.html

$_FILES["file"]["tmp_name"] 与 move_uploaded_file()
来源：http://hz.gotoacloud.top/gtdoogwzsb.html

[U68] PHP：PDO 连接
来源：http://hz.tanke756.top/gtqebelyrt.html

$pdo = new PDO("mysql:host=localhost;dbname=app", "root", "");
来源：http://hz.kuanghao11.cn/gtuedcthxr.html

[U69] PHP：PDO 预处理
来源：http://hz.meibo888.top/gtituoxldw.html

$stmt = $pdo->prepare("SELECT * FROM users WHERE id = ?");  $stmt->execute([$id]);
来源：http://hz.xziqi.cn/gtlxxgocxn.html

[U70] PHP：PDO 事务
来源：http://hz.jinyuanbaomall.cn/gtbhxcckxb.html

$pdo->beginTransaction();  $pdo->commit();  $pdo->rollBack();
来源：http://hz.zhongyouzk.top/gtqtkhlcvf.html


<!-- 参考信息 -->