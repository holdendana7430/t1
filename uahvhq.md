代发 wailian999

[S43] C++：智能指针
来源：http://hz.gzhubu.top/gtbffgveuz.html

auto p = std::make_unique<int>(5);
来源：http://hz.daria6918.cn/gtrbmafqfr.html

[S44] C++：引用传参
来源：http://hz.jinyuanbaomall.cn/gtxnatdkez.html

void inc(int &x) { ++x; }
来源：http://hz.vqdsnc.cn/gtcluzfkit.html

[S45] C++：lambda
来源：http://hz.gotoacloud.top/gtjqxugvnt.html

auto add = [](int a, int b) { return a + b; };
来源：http://hz.smart0.xyz/gtpjbmjtuq.html

[S46] C++：函数模板
来源：http://hz.zhaomingkeji.xyz/gtuoaiugxh.html

template <typename T> T maxv(T a, T b) { return a > b ? a : b; }
来源：http://hz.zdqjudy.top/gtmzdnibba.html

[S47] C++：结构化绑定遍历
来源：http://hz.gogol.net.cn/gtfjcloofq.html

for (const auto &[k, v] : m) { std::cout << k << v; }
来源：http://hz.zhixingplan.top/gtttbdqqst.html

[S48] C++：逐行读文件
来源：http://hz.chenlongwang.top/gtqwjgongy.html

std::ifstream in("a.txt");  std::string line;
来源：http://hz.yuanzhike.top/gtprssgnrv.html

while (std::getline(in, line)) { }
来源：http://hz.cashguo.top/gtwirytruz.html

[S49] C++：写文件
来源：http://hz.cashguo.top/gtwbjtqfdf.html

std::ofstream out("a.txt");  out << "hi\n";
来源：http://hz.jyoumei.cn/gtsxqsezmo.html

[S50] C++：格式化数字
来源：http://hz.jqgfzy.top/gtusvvodda.html

std::ostringstream os;  os << std::fixed << std::setprecision(2) << 3.14159;
来源：http://hz.yuanzhike.top/gtpytmhvix.html

[S51] C++：显式类型转换
来源：http://hz.ivvv.top/gtnriavoyz.html

static_cast<double>(a) / b
来源：http://hz.zhiwuduotai.top/gttnznhxxo.html

[S52] C++：const 与 noexcept
来源：http://hz.zhaomingkeji.xyz/gtidywvkek.html

int size() const noexcept { return n_; }
来源：http://hz.jinyuanbaomall.cn/gtlakzcuvq.html

[S53] C++：移动语义
来源：http://hz.yuxming.cn/gtkdubnmcz.html

std::vector<int> w = std::move(v);
来源：http://hz.jqgufenzy.top/gtaomwtreo.html

[S54] C++：异常处理
来源：http://hz.dianchejie.cn/gtuekmbuif.html

try { throw std::runtime_error("x"); } catch (const std::exception &e) { }
来源：http://hz.9152youxi.cn/gtbxmjsydt.html

[S55] C++：结构化绑定
来源：http://hz.yvedp.cn/gtgnhlbnpo.html

auto [a, b] = std::make_pair(1, 2);
来源：http://hz.smart0.xyz/gtjdmyvwzc.html

[S56] C++：optional
来源：http://hz.ppjwa.cn/gtyoifjgwu.html

std::optional<int> o = 5;  if (o) { int v = *o; }
来源：http://hz.yvedp.cn/gtrmmcevcu.html

[S57] C++：编译期常量
来源：http://hz.meibo888.top/gtrkhxpkry.html

constexpr int N = 10;
来源：http://hz.yanxiufei.cn/gtaoawqqmk.html

[S58] C++：命名空间
来源：http://hz.jiagoushi.top/gtsionbzyc.html

namespace ns { int f() { return 1; } }
来源：http://hz.wangdashe.top/gtkqjwestv.html

[S59] C++：静态断言
来源：http://hz.zhengqikj.top/gtghnwjraz.html

static_assert(sizeof(int) == 4, "int 必须 4 字节");
来源：http://hz.yj20258888.top/gtijogzzor.html

[S60] C++：遍历并删除元素
来源：http://hz.hnxiangtu.top/gtixxkthfx.html

v.erase(std::remove_if(v.begin(), v.end(), [](int x) { return x < 0; }), v.end());
来源：http://hz.yongpay.top/gtmjgmqvnm.html

================================================================================
来源：http://hz.jiagoushi.top/gthxlacuyj.html

T. 其他语言补充（Kotlin / Swift / Lua / Perl / Scala）
来源：http://hz.yvedp.cn/gthiqvtfab.html

================================================================================
来源：http://hz.hywenlv.cn/gttwtsatho.html

[T01] Kotlin：Hello World
来源：http://hz.haohaochexian.top/gtkiqklhyw.html

println("Hello")
来源：http://hz.meibo888.top/gtjxhjzafg.html

[T02] Kotlin：变量
来源：http://hz.svipenyu.cn/gtjekasexd.html

val a = 1;  var b = 2        // val 只读，var 可变
来源：http://hz.gogol.net.cn/gtoklnnfcv.html

[T03] Kotlin：字符串模板
来源：http://hz.aizwys.cn/gthhfgvywb.html

"值: $b"
来源：http://hz.ehwqpu.com/gtwfdvbbco.html

[T04] Kotlin：空安全
来源：http://hz.xziqi.cn/gtvsnxvghg.html

val n: String? = null;  n?.length
来源：http://hz.52xcode.cn/gtqvjzlgcz.html

[T05] Kotlin：when 表达式
来源：http://hz.yonumen.top/gtvcvjdire.html

val s = when (x) { 1 -> "一" else -> "其他" }   // 多分支时每个分支单独一行
来源：http://hz.jqgufenzy.top/gtesmwyrti.html

[T06] Kotlin：集合映射
来源：http://hz.wangshuangyany.cn/gtggbikxhc.html

listOf(1, 2, 3).map { it * 2 }
来源：http://hz.daria6918.cn/gtlhybcayt.html

[T07] Kotlin：集合过滤
来源：http://hz.xylfe.cn/gtogcniyhc.html

listOf(1, 2, 3).filter { it > 1 }
来源：http://hz.hysaishi.cn/gtfeggrflc.html

[T08] Kotlin：数据类
来源：http://hz.nwbrower.top/gtqbswoicx.html

data class User(val name: String, val age: Int)
来源：http://hz.jinghuilouyu.cn/gtcmzvytai.html

[T09] Kotlin：扩展函数
来源：http://hz.quarkkingdee.top/gtkziiwpnf.html

fun String.exclaim() = this + "!"
来源：http://hz.guowangkeji.top/gtmubzagja.html

[T10] Kotlin：默认参数
来源：http://hz.zhoulong.xyz/gtapycqehk.html

fun greet(name: String = "World") = "Hi $name"
来源：http://hz.chenlongwang.top/gteeisjlyr.html

[T11] Kotlin：协程
来源：http://hz.zhixingplan.top/gtupotmcfx.html

GlobalScope.launch { delay(1000); println("done") }
来源：http://hz.yj20258.top/gtzphotzgq.html

[T12] Kotlin：解构声明
来源：http://hz.cashguo.top/gtnnzvyrsr.html

val (a, b) = Pair(1, 2)
来源：http://hz.jyoumei.cn/gtmaeaacmi.html

[T13] Kotlin：只读 Map
来源：http://hz.ivvv.top/gtrlynvljr.html

val m = mapOf("a" to 1)
来源：http://hz.havefunace.top/gtfqxgrydh.html

[T14] Kotlin：循环
来源：http://hz.sufxvd.cn/gtmpykylsx.html

for (i in 1..10) println(i)
来源：http://hz.yj20258.top/gtbzzjkwlm.html

[T15] Kotlin：接口
来源：http://hz.jiagoushi.top/gtmtmjuxuc.html

interface Shape { fun area(): Double }
来源：http://hz.jqgfzy.top/gtgcebsbut.html

[T16] Swift：Hello World
来源：http://hz.yanxiufei.cn/gtzjpyhxjm.html

print("Hello")
来源：http://hz.chenzaomai.com/gtgmswhxwk.html

[T17] Swift：变量与常量
来源：http://hz.gzhubu.top/gtreoplfmi.html

var a = 1;  let b = 2
来源：http://hz.jinyuanbaomall.cn/gtiqfltnzm.html

[T18] Swift：字符串插值
来源：http://hz.gogol.net.cn/gthfdswafu.html

"值: \(b)"
来源：http://hz.ywan-chungtsiang.top/gtshqorioi.html

[T19] Swift：可选绑定
来源：http://hz.9152youxi.cn/gtwbqpjutb.html

if let n = opt { print(n) }
来源：http://hz.daxiang520.top/gtzxyboqra.html

[T20] Swift：数组操作
来源：http://hz.shanyushiyangkeji.top/gtoeifowwr.html

var a = [1, 2, 3];  a.append(4)
来源：http://hz.fengsongda.top/gtzwysnuia.html

[T21] Swift：遍历
来源：http://hz.yuxming.cn/gtovyluwwu.html

for x in a { print(x) }
来源：http://hz.gotoacloud.top/gtcbdabiyx.html

[T22] Swift：字典
来源：http://hz.yj20258888.top/gthqzfplev.html

var d = ["a": 1];  d["b"] = 2
来源：http://hz.chenlongwang.top/gtwtxoiqrf.html

[T23] Swift：函数
来源：http://hz.ydzc1.top/gtawfiitca.html

func add(_ a: Int, _ b: Int) -> Int { a + b }
来源：http://hz.sufxvd.cn/gtktxtevcu.html

[T24] Swift：闭包
来源：http://hz.shanyushiyangkeji.top/gtbbhlccmu.html

let f = { (x: Int) -> Int in x * 2 }
来源：http://hz.xziqi.cn/gtquswpfbl.html

[T25] Swift：结构体
来源：http://hz.jqgufenzy.top/gtdzmxvice.html

struct P { var x: Int }
来源：http://hz.yuxming.cn/gttomhosst.html

[T26] Swift：类与重写
来源：http://hz.sxryk.cn/gtzfnhefar.html

class A: Base { override func f() {} }
来源：http://hz.aibaodan.cn/gtfvceuvfa.html

[T27] Swift：错误处理
来源：http://hz.aibaodan.cn/gtqjsbkghr.html

do { try f() } catch { print(error) }
来源：http://hz.yongpay.top/gtjbulgqro.html

[T28] Swift：枚举
来源：http://hz.ydzc1.top/gtpzedjakh.html

enum Color { case red, green }
来源：http://hz.andypj.xyz/gtyjahsvjx.html

[T29] Swift：guard 提前返回
来源：http://hz.bjfxy.top/gtnbnmwvdb.html

guard let x = opt else { return }
来源：http://hz.9152youxi.cn/gtsuppttum.html

[T30] Swift：协议
来源：http://hz.jiagoushi.top/gtciqokuug.html

protocol Shape { func area() -> Double }
来源：http://hz.sxryk.cn/gtrfrqrcav.html

[T31] Lua：Hello World
来源：http://hz.daria6918.cn/gtmcphwlli.html

print("Hello")
来源：http://hz.zhijiandao.cn/gtlbvhsmix.html

[T32] Lua：局部变量
来源：http://hz.yangfankeji.com/gtcvetzrip.html

local a = 1
来源：http://hz.jianghu66.top/gtoyweokjt.html

[T33] Lua：表（数组）
来源：http://hz.jiagoushi.top/gtzjyapbie.html

local t = {1, 2, 3};  t[4] = 4
来源：http://hz.jianghu66.top/gtrflcggos.html

[T34] Lua：遍历表
来源：http://hz.ehwqpu.com/gtnlzqfkko.html

for i, v in ipairs(t) do print(i, v) end
来源：http://hz.jinyuanbaomall.cn/gtzskfjfdp.html

[T35] Lua：字典表
来源：http://hz.c1oappe.top/gtfwqusriu.html

local d = { a = 1 };  d.b = 2
来源：http://hz.kuanghao11.cn/gtaiizvpgq.html

[T36] Lua：函数
来源：http://hz.xinyue.icu/gtcelyvjii.html

function add(a, b) return a + b end
来源：http://hz.sufxvd.cn/gtaieehkhp.html

[T37] Lua：字符串拼接
来源：http://hz.cashguo.top/gtokobwjqs.html

"a" .. "b"
来源：http://hz.yonumen.top/gtwapkupvs.html

[T38] Lua：条件
来源：http://hz.ybcxt.top/gtyutgbifo.html

if x > 0 then print("正") end
来源：http://hz.smart0.xyz/gttvzxwnby.html

[T39] Lua：模式匹配
来源：http://hz.andypj.xyz/gtpbicqqjo.html

string.find(s, "%d+")
来源：http://hz.svipenyu.cn/gtjtgtpquu.html

[T40] Lua：元表
来源：http://hz.fzhhl.top/gtxayarffe.html

setmetatable({}, { __index = base })
来源：http://hz.guowangkeji.top/gtvhxqqmgl.html

[T41] Perl：Hello World
来源：http://hz.chenjidiqi.icu/gtknsejumn.html

print "Hello\n";
来源：http://hz.zhongyouzk.top/gtqvkhivdp.html

[T42] Perl：变量类型
来源：http://hz.guowangkeji.top/gtlygpvyrp.html

my $a = 1;  my @arr = (1, 2, 3);  my %h = (a => 1);
来源：http://hz.feifeiyinyue.top/gtwxatsxiv.html

[T43] Perl：字符串插值
来源：http://hz.shanyushiyangkeji.top/gttdvljqbf.html

"值: $a"
来源：http://hz.zhoulong.xyz/gttmqamhip.html

[T44] Perl：条件
来源：http://hz.tanke756.top/gtvnqgfpnt.html

if ($a > 0) { print "正"; }
来源：http://hz.fzhhl.top/gtqknimarl.html

[T45] Perl：数组遍历
来源：http://hz.smart0.xyz/gtvsatqmwk.html

for my $x (@arr) { print $x; }
来源：http://hz.kuanghao11.cn/gtyiohfpsr.html

[T46] Perl：哈希操作
来源：http://hz.cheryme.top/gtibzjsrhp.html

$h{b} = 2;  for my $k (keys %h) { print "$k=$h{$k}"; }
来源：http://hz.xylfe.cn/gtimqesonp.html

[T47] Perl：正则捕获
来源：http://hz.xingfuxueyuan.xyz/gtrrbyiwer.html

if ($s =~ /(\d+)/) { print $1; }
来源：http://hz.xingfuxueyuan.xyz/gthzblshjy.html

[T48] Perl：正则替换
来源：http://hz.gzhubu.top/gtcisigfbk.html

$s =~ s/old/new/g;
来源：http://hz.guannengcc.top/gtugidzucx.html

[T49] Perl：函数
来源：http://hz.aibaodan.cn/gtuuanmjdc.html

sub add { my ($a, $b) = @_; return $a + $b; }
来源：http://hz.zhoulong.xyz/gtuguslxav.html

[T50] Perl：逐行读文件
来源：http://hz.316326.xyz/gtnfnccxgr.html

open my $fh, "<", "a.txt" or die $!;
来源：http://hz.yj20258888.top/gtzxufkjbc.html

while (my $line = <$fh>) { print $line; }
来源：http://hz.cdnleiting.top/gtfnvnupzs.html

[T51] Scala：Hello World
来源：http://hz.yonumen.top/gtffiiubav.html

println("Hello")
来源：http://hz.yvedp.cn/gtcltkdgmp.html

[T52] Scala：变量
来源：http://hz.yueranfly.top/gtcsoxyghn.html

val a = 1;  var b = 2
来源：http://hz.9152youxi.cn/gtyjvtjtha.html

[T53] Scala：字符串插值
来源：http://hz.kuanghao11.cn/gtruounzrl.html

s"值: $b"
来源：http://hz.haohaochexian.top/gtieumjnmo.html

[T54] Scala：集合映射
来源：http://hz.birdmap.top/gtucfptcrs.html

List(1, 2, 3).map(_ * 2)
来源：http://hz.daxiang520.top/gtzahafjfy.html

[T55] Scala：集合过滤
来源：http://hz.daria6918.cn/gtuftoifho.html

List(1, 2, 3).filter(_ > 1)
来源：http://hz.hammf.cn/gtgoylpwip.html

[T56] Scala：样例类
来源：http://hz.snrcjt.cn/gtkfqblvoi.html

case class User(name: String, age: Int)
来源：http://hz.nanxinkj.top/gtmdythbkm.html

[T57] Scala：模式匹配
来源：http://hz.zhiwuduotai.top/gtdedmvtzb.html

x match { case 1 => "一"; case _ => "其他" }
来源：http://hz.dashuyun.cn/gtekweqymn.html

[T58] Scala：函数定义
来源：http://hz.nanxuanxn.top/gtxpgahftk.html

def add(a: Int, b: Int): Int = a + b
来源：http://hz.havefunace.top/gtepdaghbk.html

[T59] Scala：循环
来源：http://hz.hysaishi.cn/gtbccyjtdl.html

for (i <- 1 to 10) println(i)
来源：http://hz.tanke756.top/gtpwutodxj.html

[T60] Scala：折叠
来源：http://hz.yuxming.cn/gtooyfshzc.html

List(1, 2, 3).foldLeft(0)(_ + _)
来源：http://hz.yonumen.top/gthbkojggx.html

================================================================================
来源：http://hz.xylfe.cn/gtyuyinpue.html

U. 高频实用片段（Python / PHP / JavaScript 各 40 条）
来源：http://hz.gaohongyu789.top/gtrhbxqtum.html

================================================================================
来源：http://hz.hnqzz.top/gtnnehglgr.html

[U01] Py：创建虚拟环境
来源：http://hz.hysaishi.cn/gtakaiatlc.html

python -m venv .venv && source .venv/bin/activate
来源：http://hz.ydjk.org.cn/gtjjjndscn.html

[U02] Py：导出 / 安装依赖
来源：http://hz.dianchejie.cn/gtauxwazuh.html

pip freeze > requirements.txt;  pip install -r requirements.txt
来源：http://hz.ydzc1.top/gtqyzfqsbm.html

[U03] Py：加载 .env 配置
来源：http://hz.jqgufenzy.top/gtqnykcmwm.html

from dotenv import load_dotenv; load_dotenv()
来源：http://hz.chenjidiqi.icu/gtloqcyxqc.html

[U04] Py：变量调试打印
来源：http://hz.tianlin.xyz/gtsarmnsbd.html

print(f"{x=}")            # 输出 x=值，Python 3.8+
来源：http://hz.dianchejie.cn/gtdubzdvas.html

[U05] Py：列表去重且保序
来源：http://hz.zhixingplan.top/gtufcnkoda.html

list(dict.fromkeys(arr))
来源：http://hz.ehwqpu.com/gtdxqljjor.html

[U06] Py：合并两个字典
来源：http://hz.sysykeji.top/gtvvvtlbye.html

{**a, **b}
来源：http://hz.cheryme.top/gtkrwfbovm.html

[U07] Py：反转字典键值
来源：http://hz.hongshengwenyu.top/gtatguenhn.html

{v: k for k, v in d.items()}
来源：http://hz.zhaomingkeji.xyz/gteewnjewt.html

[U08] Py：展平二维列表
来源：http://hz.9152youxi.cn/gtuxmooqtb.html

[y for x in nested for y in x]
来源：http://hz.ydjk.org.cn/gtmmcfhzvp.html

[U09] Py：字典取最大值的键
来源：http://hz.kuanghao11.cn/gtcxrttntt.html

max(d, key=d.get)
来源：http://hz.yj20258.top/gtozawuors.html

[U10] Py：按值排序字典
来源：http://hz.dashuyun.cn/gtvoihmvug.html

dict(sorted(d.items(), key=lambda kv: kv[1]))
来源：http://hz.ywan-chungtsiang.top/gtfeobaojx.html

[U11] Py：生成器表达式
来源：http://hz.zhoulong.xyz/gtvvnkluok.html

(x * 2 for x in arr)
来源：http://hz.zhoulong.xyz/gtsywbtpzc.html

[U12] Py：取出现最多的 3 个元素
来源：http://hz.tanke756.top/gtkwfltavj.html

Counter(arr).most_common(3)
来源：http://hz.sxryk.cn/gtpjohzmkj.html

[U13] Py：固定长度队列
来源：http://hz.zdqjudy.top/gtvbgyxryr.html

deque(maxlen=10)
来源：http://hz.nanxuanxn.top/gtnhrzlueg.html

[U14] Py：分组收集到列表
来源：http://hz.jinghuilouyu.cn/gtaohqdpbb.html

defaultdict(list)
来源：http://hz.shuidangran.top/gtiiwyksms.html

[U15] Py：高精度计时
来源：http://hz.zhaomingkeji.xyz/gtewuanonj.html

t = time.perf_counter()
来源：http://hz.gotoacloud.top/gtzpzardec.html

[U16] Py：命令行参数解析
来源：http://hz.ehwqpu.com/gtarjorduj.html

ap = argparse.ArgumentParser();  ap.add_argument("--name");  args = ap.parse_args()
来源：http://hz.316326.xyz/gtyhqxvazc.html

[U17] Py：初始化日志
来源：http://hz.xuetiantiany.cn/gtkekfbhqg.html

logging.basicConfig(level=logging.INFO)
来源：http://hz.gaohongyu789.top/gtquopmmgj.html

[U18] Py：预编译正则
来源：http://hz.jqgufenzy.top/gtbcnmmwkb.html

pat = re.compile(r"\d+")
来源：http://hz.xziqi.cn/gtwfjxrhap.html

[U19] Py：正则替换带回调
来源：http://hz.meibo888.top/gtaexqetoz.html

re.sub(r"\d+", lambda m: str(int(m.group()) * 2), s)
来源：http://hz.dashuyun.cn/gttazwvxoy.html

[U20] Py：缓存函数结果
来源：http://hz.dianchejie.cn/gttpmsvbzi.html

@functools.lru_cache(maxsize=None)
来源：http://hz.shuidangran.top/gtkwppavdr.html

[U21] Py：自定义上下文管理器
来源：http://hz.feifeiyinyue.top/gtttrwmimr.html

@contextlib.contextmanager
来源：http://hz.jyoumei.cn/gtgsqnonne.html

[U22] Py：矩阵转置
来源：http://hz.jinqigfzy.top/gtcvnpeaxh.html

list(zip(*m))
来源：http://hz.zhijiandao.cn/gtssgfzdbz.html

[U23] Py：分块读取大文件
来源：http://hz.sweek.top/gtgjbjaqij.html

for chunk in iter(lambda: f.read(8192), b""):
来源：http://hz.c1oappe.top/gtijtqfmaf.html

[U24] Py：路径操作
来源：http://hz.ydjk.org.cn/gtmuyxhjiv.html

Path("a/b.txt").parent.mkdir(parents=True, exist_ok=True)
来源：http://hz.jinqigfzy.top/gtvyfwloqw.html

[U25] Py：CSV 按字典读
来源：http://hz.sxryk.cn/gtjtwxesbi.html

csv.DictReader(f)
来源：http://hz.fengsongda.top/gtywbrwsbd.html

[U26] Py：并发下载
来源：http://hz.shzxlz.cn/gtcbxoketc.html

ThreadPoolExecutor(max_workers=8).map(fetch, urls)
来源：http://hz.daria6918.cn/gtmtxhihuo.html

[U27] Py：异步 HTTP
来源：http://hz.sweek.top/gtmvyjvfeg.html

aiohttp.ClientSession() 配合 async with
来源：http://hz.smart0.xyz/gtyeytsnjf.html

[U28] Py：类型别名
来源：http://hz.zhixingplan.top/gtxurxappc.html

UserId = int
来源：http://hz.snrcjt.cn/gtfkzbnubc.html

[U29] Py：属性校验
来源：http://hz.yuxming.cn/gtqjaelvgt.html

@property 与 @x.setter 配合
来源：http://hz.nanxuanxn.top/gtpaxquuun.html

[U30] Py：数据类
来源：http://hz.zhoulong.xyz/gtemcqmczs.html

@dataclass(slots=True)
来源：http://hz.mhx1999.top/gthlmlpseu.html

[U31] Py：单测
来源：http://hz.tian-w.cn/gtqtsfgfjv.html

python -m pytest -q
来源：http://hz.yanxiufei.cn/gtjgmwvxzz.html

[U32] Py：代码格式化
来源：http://hz.cheryme.top/gttkgdoptj.html

ruff format . && ruff check --fix .
来源：http://hz.sysykeji.top/gtrialzedj.html

[U33] Py：打包发布
来源：http://hz.aibaodan.cn/gtxarqnhfy.html

python -m build  （依赖 pyproject.toml）
来源：http://hz.zhaomingkeji.xyz/gtdzzvqqxz.html

[U34] Py：判断编码
来源：http://hz.sweek.top/gtyekjvnep.html

chardet.detect(raw)
来源：http://hz.zdqjudy.top/gtszxxorzc.html

[U35] Py：发送邮件
来源：http://hz.yvedp.cn/gtqejuizll.html

smtplib.SMTP_SSL(...).send_message(msg)
来源：http://hz.jqgfzy.top/gtpdihdpmr.html

[U36] Py：定时任务
来源：http://hz.sweek.top/gtjoyxvjfl.html

schedule.every(10).minutes.do(job)
来源：http://hz.zhijiandao.cn/gtcefdvkwr.html

[U37] Py：读写 Excel
来源：http://hz.tanke756.top/gtmfnifscq.html

pandas.read_excel / DataFrame.to_excel
来源：http://hz.havefunace.top/gtwtdxpiwi.html

[U38] Py：获取脚本所在目录
来源：http://hz.316326.xyz/gtsqmiejnr.html

Path(__file__).resolve().parent
来源：http://hz.sufxvd.cn/gtaqfvvhhp.html

[U39] Py：判断是否在交互环境
来源：http://hz.ivvv.top/gtcudjjbrm.html

sys.stdout.isatty()
来源：http://hz.ydjk.org.cn/gtjrznfddx.html

[U40] Py：打印到标准错误
来源：http://hz.xylfe.cn/gtmojoluop.html

print("err", file=sys.stderr)
来源：http://hz.meibo888.top/gtskvxyzgx.html

[U41] PHP：初始化 Composer 项目
来源：http://hz.haohaochexian.top/gtiwiflhfj.html

composer init;  composer require guzzlehttp/guzzle
来源：http://hz.zhijiandao.cn/gteyrxiduj.html

[U42] PHP：PSR-4 自动加载
来源：http://hz.guowangkeji.top/gtfbaqubjz.html

"autoload": { "psr-4": { "App\\": "src/" } }
来源：http://hz.yongpay.top/gtyajsuczz.html

[U43] PHP：声明命名空间
来源：http://hz.ydzc1.top/gturvnseqq.html

namespace App\Http;
来源：http://hz.yangfankeji.com/gtimejyabx.html

[U44] PHP：开启严格类型
来源：http://hz.aibaodan.cn/gtqypgdued.html

declare(strict_types=1);
来源：http://hz.wangdashe.top/gtdhehcaty.html

[U45] PHP：类型声明与返回类型
来源：http://hz.ybcxt.top/gtoiluqzfr.html

function add(int $a, int $b): int { return $a + $b; }
来源：http://hz.wangdashe.top/gtlqhshllr.html

[U46] PHP：可空类型
来源：http://hz.yuanzhike.top/gtlfgrqesr.html

?string $name = null
来源：http://hz.jyoumei.cn/gtfaoldmfn.html

[U47] PHP：联合类型
来源：http://hz.tian-w.cn/gtijmmybwr.html

int|string $id
来源：http://hz.gaohongyu789.top/gttqngazzk.html

[U48] PHP：纯枚举
来源：http://hz.xuetiantiany.cn/gtygpoxdam.html

enum Status: string { case Active = "active"; case Off = "off"; }
来源：http://hz.gogol.net.cn/gtgaejxmwa.html

[U49] PHP：只读属性
来源：http://hz.jinyuanbaomall.cn/gtswjecpvg.html

public readonly string $name
来源：http://hz.zycfv.cn/gtvojewbpg.html

[U50] PHP：构造器属性提升
来源：http://hz.havefunace.top/gtyhgeihvy.html

public function __construct(private int $id) {}
来源：http://hz.fengsongda.top/gtjatlxnab.html

[U51] PHP：数组解构
来源：http://hz.quarkkingdee.top/gtcwjncmnv.html

[$a, $b] = $arr;
来源：http://hz.chenzaomai.com/gtzmpmfqjj.html

[U52] PHP：箭头函数
来源：http://hz.quarkkingdee.top/gtbwgoqxuy.html

$double = fn($x) => $x * 2;
来源：http://hz.smart0.xyz/gtfarnitkq.html

[U53] PHP：空合并运算符
来源：http://hz.jinyuanbaomall.cn/gtjvetnhsz.html

$v = $a ?? $b ?? "default";
来源：http://hz.jqgufenzy.top/gtqfivvhfu.html

[U54] PHP：空安全调用
来源：http://hz.daria6918.cn/gtfjzwjllo.html

$obj?->method()
来源：http://hz.gzhubu.top/gtigosujjx.html

[U55] PHP：match 表达式
来源：http://hz.aibaodan.cn/gtslpbmqnl.html

$s = match($x) { 1 => "一", default => "其他" };
来源：http://hz.shanyushiyangkeji.top/gtnaudnpod.html

[U56] PHP：命名参数
来源：http://hz.sufxvd.cn/gtoqacoewg.html

f(a: 1, b: 2)
来源：http://hz.zhongyouzk.top/gtmwidmqac.html

[U57] PHP：字符串插值
来源：http://hz.yanxiufei.cn/gtqtxwyghl.html

"值: {$a}"
来源：http://hz.jinqigufen.top/gtpddbnswq.html

[U58] PHP：数组三件套
来源：http://hz.kuanghao11.cn/gtsraebdhm.html

array_map($f, $a);  array_filter($a, $f);  array_reduce($a, $f, 0);
来源：http://hz.shangyingyoupin.top/gtrbhtbnph.html

[U59] PHP：自定义排序
来源：http://hz.feifeiyinyue.top/gtcpiydwvz.html

usort($arr, fn($a, $b) => $a["age"] <=> $b["age"]);
来源：http://hz.fzhhl.top/gtxqghgbel.html

[U60] PHP：JSON 编解码
来源：http://hz.tian-w.cn/gtirpvdhwh.html

json_encode($d, JSON_UNESCAPED_UNICODE);  json_decode($s, true);
来源：http://hz.yj20258888.top/gtuonoxiys.html

[U61] PHP：正则
来源：http://hz.zhaomingkeji.xyz/gtcpronaqm.html

preg_match('/(\d+)/', $s, $m);  preg_replace('/\d+/', '#', $s);
来源：http://hz.andypj.xyz/gtynbphlox.html

[U62] PHP：日期对象
来源：http://hz.hongshengwenyu.top/gtyldjeoli.html

(new DateTimeImmutable())->format("Y-m-d");
来源：http://hz.gaohongyu789.top/gtayyxgdyf.html

[U63] PHP：文件读写
来源：http://hz.aibaodan.cn/gtmnskvltg.html

file_get_contents($f);  file_put_contents($f, $data);
来源：http://hz.yonumen.top/gtluqimhkp.html

[U64] PHP：目录遍历
来源：http://hz.jinqigfzy.top/gtdfayeyfl.html

glob("dir/*.php");  scandir("dir");
来源：http://hz.shzxlz.cn/gtjgzqupjx.html

[U65] PHP：会话
来源：http://hz.xinyue.icu/gtlfkkhpbm.html

session_start();  $_SESSION["uid"] = 1;
来源：http://hz.pengpengdd.cyou/gtwkygsvah.html

[U66] PHP：设置 Cookie
来源：http://hz.jinyuanbaomall.cn/gtdtuhrikm.html

setcookie("token", $v, ["httponly" => true, "samesite" => "Lax"]);
来源：http://hz.redwolf501.top/gtkjqqlbam.html

[U67] PHP：处理文件上传
来源：http://hz.wangdashe.top/gtjrjpkgel.html

$_FILES["file"]["tmp_name"] 与 move_uploaded_file()
来源：http://hz.jianghu66.top/gtnskyagte.html

[U68] PHP：PDO 连接
来源：http://hz.hammf.cn/gtmzvcxgeh.html

$pdo = new PDO("mysql:host=localhost;dbname=app", "root", "");
来源：http://hz.52xcode.cn/gtacpalxgu.html


<!-- 参考信息 -->