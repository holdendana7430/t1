代发 wailian999

[S45] C++：lambda
来源：http://hz.sxryk.cn/gtogjwtemz.html

auto add = [](int a, int b) { return a + b; };
来源：http://hz.yuxming.cn/gtbbqqeecz.html

[S46] C++：函数模板
来源：http://hz.yuxming.cn/gtiptcyegs.html

template <typename T> T maxv(T a, T b) { return a > b ? a : b; }
来源：http://hz.fzhhl.top/gtdrjydvej.html

[S47] C++：结构化绑定遍历
来源：http://hz.cucudq.cn/gtvvqjqslp.html

for (const auto &[k, v] : m) { std::cout << k << v; }
来源：http://hz.cqqwz.cn/gtdpgfybrr.html

[S48] C++：逐行读文件
来源：http://hz.cheryme.top/gtpcamtgqv.html

std::ifstream in("a.txt");  std::string line;
来源：http://hz.sufxvd.cn/gtfjujiybu.html

while (std::getline(in, line)) { }
来源：http://hz.daria6918.cn/gtbpixujed.html

[S49] C++：写文件
来源：http://hz.vqdsnc.cn/gtquzecjmu.html

std::ofstream out("a.txt");  out << "hi\n";
来源：http://hz.zycfv.cn/gtrwcthgqk.html

[S50] C++：格式化数字
来源：http://hz.jinqigufen.top/gtlbdwbpjj.html

std::ostringstream os;  os << std::fixed << std::setprecision(2) << 3.14159;
来源：http://hz.sufxvd.cn/gtjkasicta.html

[S51] C++：显式类型转换
来源：http://hz.hfpthk.cn/gtfeeekqzm.html

static_cast<double>(a) / b
来源：http://hz.fengsongda.top/gtyywjuuuu.html

[S52] C++：const 与 noexcept
来源：http://hz.cdnleiting.top/gtzydatihz.html

int size() const noexcept { return n_; }
来源：http://hz.snrcjt.cn/gtuymwtcra.html

[S53] C++：移动语义
来源：http://hz.yangfankeji.com/gtsrzquazj.html

std::vector<int> w = std::move(v);
来源：http://hz.fengsongda.top/gtwowwvihc.html

[S54] C++：异常处理
来源：http://hz.jiagoushi.top/gtbshmfqwx.html

try { throw std::runtime_error("x"); } catch (const std::exception &e) { }
来源：http://hz.cucudq.cn/gtyaivqjns.html

[S55] C++：结构化绑定
来源：http://hz.yonumen.top/gtqelryqjg.html

auto [a, b] = std::make_pair(1, 2);
来源：http://hz.haohaochexian.top/gtxntjdjdj.html

[S56] C++：optional
来源：http://hz.cdnleiting.top/gttqfdpezk.html

std::optional<int> o = 5;  if (o) { int v = *o; }
来源：http://hz.xuanzx.com/gtpoiqrhyb.html

[S57] C++：编译期常量
来源：http://hz.sweek.top/gtazesoigb.html

constexpr int N = 10;
来源：http://hz.shanyushiyangtech.top/gtongixipz.html

[S58] C++：命名空间
来源：http://hz.yonumen.top/gtkmegjxlk.html

namespace ns { int f() { return 1; } }
来源：http://hz.aibaodan.cn/gtyalqrfrt.html

[S59] C++：静态断言
来源：http://hz.hongshengwenyu.top/gtjsiphtpg.html

static_assert(sizeof(int) == 4, "int 必须 4 字节");
来源：http://hz.sufxvd.cn/gtombxlsvf.html

[S60] C++：遍历并删除元素
来源：http://hz.hammf.cn/gtgsznscog.html

v.erase(std::remove_if(v.begin(), v.end(), [](int x) { return x < 0; }), v.end());
来源：http://hz.chenlongwang.top/gtibsezjpo.html

================================================================================
来源：http://hz.hnxiangtu.top/gtdhamnzdm.html

T. 其他语言补充（Kotlin / Swift / Lua / Perl / Scala）
来源：http://hz.shzxlz.cn/gtzcnzpbkn.html

================================================================================
来源：http://hz.chenzaomai.com/gtdiluzkap.html

[T01] Kotlin：Hello World
来源：http://hz.jlsjyb.cn/gtndoumsxr.html

println("Hello")
来源：http://hz.yvedp.cn/gtirfyihtl.html

[T02] Kotlin：变量
来源：http://hz.shangyingyoupin.top/gtwoyvpyme.html

val a = 1;  var b = 2        // val 只读，var 可变
来源：http://hz.52xcode.cn/gtagrwpuzm.html

[T03] Kotlin：字符串模板
来源：http://hz.jinyuanbaomall.cn/gttvtzkxxl.html

"值: $b"
来源：http://hz.xuetiantiany.cn/gtfricerco.html

[T04] Kotlin：空安全
来源：http://hz.yvedp.cn/gtdvxdhwof.html

val n: String? = null;  n?.length
来源：http://hz.cdnleiting.top/gtjqkwdbwx.html

[T05] Kotlin：when 表达式
来源：http://hz.yueranfly.top/gtrceujjxr.html

val s = when (x) { 1 -> "一" else -> "其他" }   // 多分支时每个分支单独一行
来源：http://hz.jinqigufen.top/gtiykskoid.html

[T06] Kotlin：集合映射
来源：http://hz.chenzaomai.com/gttuznjslj.html

listOf(1, 2, 3).map { it * 2 }
来源：http://hz.chenzaomai.com/gtuoacfzhe.html

[T07] Kotlin：集合过滤
来源：http://hz.cdnleiting.top/gtyhmfawpy.html

listOf(1, 2, 3).filter { it > 1 }
来源：http://hz.smart0.xyz/gtbbkyxtqz.html

[T08] Kotlin：数据类
来源：http://hz.hnqzz.top/gtnhwqvqbs.html

data class User(val name: String, val age: Int)
来源：http://hz.birdmap.top/gtpdarhxyl.html

[T09] Kotlin：扩展函数
来源：http://hz.yongpay.top/gtqtmllgqf.html

fun String.exclaim() = this + "!"
来源：http://hz.jinghuilouyu.cn/gtjmfynodv.html

[T10] Kotlin：默认参数
来源：http://hz.yuxming.cn/gtjmzwjrss.html

fun greet(name: String = "World") = "Hi $name"
来源：http://hz.zhijiandao.cn/gtseteewis.html

[T11] Kotlin：协程
来源：http://hz.jinghuilouyu.cn/gtufazrklu.html

GlobalScope.launch { delay(1000); println("done") }
来源：http://hz.316326.xyz/gtfwifnukh.html

[T12] Kotlin：解构声明
来源：http://hz.ivvv.top/gtsjmfecrl.html

val (a, b) = Pair(1, 2)
来源：http://hz.hysaishi.cn/gtgdfycqxj.html

[T13] Kotlin：只读 Map
来源：http://hz.havefunace.top/gtrvagxqhu.html

val m = mapOf("a" to 1)
来源：http://hz.zhijiandao.cn/gtamymnqov.html

[T14] Kotlin：循环
来源：http://hz.ehwqpu.com/gtixyanlvp.html

for (i in 1..10) println(i)
来源：http://hz.sweek.top/gtawbcmqhj.html

[T15] Kotlin：接口
来源：http://hz.cucudq.cn/gtkqwkgwia.html

interface Shape { fun area(): Double }
来源：http://hz.ivvv.top/gtwafjdqbn.html

[T16] Swift：Hello World
来源：http://hz.hongshengwenyu.top/gtuctpvoco.html

print("Hello")
来源：http://hz.xylfe.cn/gtrvakiqyh.html

[T17] Swift：变量与常量
来源：http://hz.jqgufenzy.top/gtczfowsuy.html

var a = 1;  let b = 2
来源：http://hz.yj20258.top/gtjklobxow.html

[T18] Swift：字符串插值
来源：http://hz.ehwqpu.com/gtfynfukve.html

"值: \(b)"
来源：http://hz.shangyingyoupin.top/gtwwnuthbt.html

[T19] Swift：可选绑定
来源：http://hz.andypj.xyz/gtqqbkccey.html

if let n = opt { print(n) }
来源：http://hz.hysaishi.cn/gtazjilwue.html

[T20] Swift：数组操作
来源：http://hz.hammf.cn/gtfesosuvj.html

var a = [1, 2, 3];  a.append(4)
来源：http://hz.daxiang520.top/gtnekrrrfx.html

[T21] Swift：遍历
来源：http://hz.ehwqpu.com/gttkxnhcme.html

for x in a { print(x) }
来源：http://hz.wangshuangyany.cn/gtmdzstbzi.html

[T22] Swift：字典
来源：http://hz.shuidangran.top/gtvvscxwul.html

var d = ["a": 1];  d["b"] = 2
来源：http://hz.ydzc1.top/gtyptlijrd.html

[T23] Swift：函数
来源：http://hz.haohaochexian.top/gtgwalppud.html

func add(_ a: Int, _ b: Int) -> Int { a + b }
来源：http://hz.ivvv.top/gterzctiso.html

[T24] Swift：闭包
来源：http://hz.nanxinkj.top/gtobfafkcc.html

let f = { (x: Int) -> Int in x * 2 }
来源：http://hz.dashuyun.cn/gtmosclxai.html

[T25] Swift：结构体
来源：http://hz.yvedp.cn/gtsfroxtkx.html

struct P { var x: Int }
来源：http://hz.feifeiyinyue.top/gtmuaqucqy.html

[T26] Swift：类与重写
来源：http://hz.ywan-chungtsiang.top/gtzmgwgebw.html

class A: Base { override func f() {} }
来源：http://hz.yuxming.cn/gtoeafeclq.html

[T27] Swift：错误处理
来源：http://hz.xuetiantiany.cn/gtbiskcllc.html

do { try f() } catch { print(error) }
来源：http://hz.cheryme.top/gtheiapyzj.html

[T28] Swift：枚举
来源：http://hz.shzxlz.cn/gtbcryzwmz.html

enum Color { case red, green }
来源：http://hz.jinqigufen.top/gtqeyoxlne.html

[T29] Swift：guard 提前返回
来源：http://hz.cdnleiting.top/gtojvlacis.html

guard let x = opt else { return }
来源：http://hz.ybcxt.top/gthjewujvv.html

[T30] Swift：协议
来源：http://hz.shanyushiyangtech.top/gtbpyvqqdm.html

protocol Shape { func area() -> Double }
来源：http://hz.sxryk.cn/gtmtzssdxj.html

[T31] Lua：Hello World
来源：http://hz.meibo888.top/gtrvbxwhck.html

print("Hello")
来源：http://hz.guowangkeji.top/gtvnkuzsck.html

[T32] Lua：局部变量
来源：http://hz.xuetiantiany.cn/gtkadgvhui.html

local a = 1
来源：http://hz.hongshengwenyu.top/gtsjxnngkn.html

[T33] Lua：表（数组）
来源：http://hz.zdqjudy.top/gtrxpwlmbf.html

local t = {1, 2, 3};  t[4] = 4
来源：http://hz.sweek.top/gtayjrdkjf.html

[T34] Lua：遍历表
来源：http://hz.smart0.xyz/gtfuxpuqrq.html

for i, v in ipairs(t) do print(i, v) end
来源：http://hz.jlsjyb.cn/gtkveodoee.html

[T35] Lua：字典表
来源：http://hz.nwbrower.top/gtrqmpekjf.html

local d = { a = 1 };  d.b = 2
来源：http://hz.meibo888.top/gtnsgdhhez.html

[T36] Lua：函数
来源：http://hz.mhx1999.top/gtpujkupuh.html

function add(a, b) return a + b end
来源：http://hz.0kj1m.cn/gtwcrzdunh.html

[T37] Lua：字符串拼接
来源：http://hz.xingfuxueyuan.xyz/gtjlxwmfrn.html

"a" .. "b"
来源：http://hz.cheryme.top/gtrygmsxta.html

[T38] Lua：条件
来源：http://hz.zhoulong.xyz/gtnatzrnjq.html

if x > 0 then print("正") end
来源：http://hz.jqgufenzy.top/gtckleozej.html

[T39] Lua：模式匹配
来源：http://hz.cdnleiting.top/gtxhqekhti.html

string.find(s, "%d+")
来源：http://hz.shanyushiyangtech.top/gtlylwrcoc.html

[T40] Lua：元表
来源：http://hz.xylfe.cn/gtbuafzgkq.html

setmetatable({}, { __index = base })
来源：http://hz.jqgfzy.top/gtkktbvidz.html

[T41] Perl：Hello World
来源：http://hz.havefunace.top/gtdfthqcxk.html

print "Hello\n";
来源：http://hz.jinqigfzy.top/gtplejsktp.html

[T42] Perl：变量类型
来源：http://hz.bjfxy.top/gtculsmfmx.html

my $a = 1;  my @arr = (1, 2, 3);  my %h = (a => 1);
来源：http://hz.yj20258.top/gtevwqsovw.html

[T43] Perl：字符串插值
来源：http://hz.haohaochexian.top/gtwrhdvdnj.html

"值: $a"
来源：http://hz.yueranfly.top/gtddzeqcve.html

[T44] Perl：条件
来源：http://hz.tianlin.xyz/gtunqoviqw.html

if ($a > 0) { print "正"; }
来源：http://hz.52xcode.cn/gtrlpmmakr.html

[T45] Perl：数组遍历
来源：http://hz.tanke756.top/gtbrexezvb.html

for my $x (@arr) { print $x; }
来源：http://hz.zhiwuduotai.top/gtnywyevmu.html

[T46] Perl：哈希操作
来源：http://hz.ybcxt.top/gtvpatwcgc.html

$h{b} = 2;  for my $k (keys %h) { print "$k=$h{$k}"; }
来源：http://hz.svipenyu.cn/gtvkclxhmh.html

[T47] Perl：正则捕获
来源：http://hz.shuidangran.top/gtsjkbbmia.html

if ($s =~ /(\d+)/) { print $1; }
来源：http://hz.gogol.net.cn/gttjnefkmp.html

[T48] Perl：正则替换
来源：http://hz.sweek.top/gthipanyte.html

$s =~ s/old/new/g;
来源：http://hz.smart0.xyz/gtivhfaryp.html

[T49] Perl：函数
来源：http://hz.dianchejie.cn/gtegodiobl.html

sub add { my ($a, $b) = @_; return $a + $b; }
来源：http://hz.tianlin.xyz/gtnxsiskwz.html

[T50] Perl：逐行读文件
来源：http://hz.sufxvd.cn/gtkjtxffur.html

open my $fh, "<", "a.txt" or die $!;
来源：http://hz.chenjidiqi.icu/gtxgbtamiu.html

while (my $line = <$fh>) { print $line; }
来源：http://hz.ivvv.top/gtuefnzrjj.html

[T51] Scala：Hello World
来源：http://hz.gotoacloud.top/gthkfugqgq.html

println("Hello")
来源：http://hz.gotoacloud.top/gtiljjemtd.html

[T52] Scala：变量
来源：http://hz.chenlongwang.top/gtjbgtfehz.html

val a = 1;  var b = 2
来源：http://hz.quarkkingdee.top/gtjosudxto.html

[T53] Scala：字符串插值
来源：http://hz.yongpay.top/gtoctdbdfp.html

s"值: $b"
来源：http://hz.shangyingyoupin.top/gtmpnpdgmz.html

[T54] Scala：集合映射
来源：http://hz.daria6918.cn/gtywnvjxva.html

List(1, 2, 3).map(_ * 2)
来源：http://hz.guannengcc.top/gtombisisv.html

[T55] Scala：集合过滤
来源：http://hz.feifeiyinyue.top/gtigwmyggq.html

List(1, 2, 3).filter(_ > 1)
来源：http://hz.mhx1999.top/gtphjajfwv.html

[T56] Scala：样例类
来源：http://hz.svipenyu.cn/gtctwykrcc.html

case class User(name: String, age: Int)
来源：http://hz.hnxiangtu.top/gtpqoslmkk.html

[T57] Scala：模式匹配
来源：http://hz.xziqi.cn/gtxncishsm.html

x match { case 1 => "一"; case _ => "其他" }
来源：http://hz.tian-w.cn/gtsombdfqq.html

[T58] Scala：函数定义
来源：http://hz.pengpengdd.cyou/gtwatdavdu.html

def add(a: Int, b: Int): Int = a + b
来源：http://hz.yj202588.top/gtuwkwroiq.html

[T59] Scala：循环
来源：http://hz.guannengcc.top/gtizsjughg.html

for (i <- 1 to 10) println(i)
来源：http://hz.316326.xyz/gttyspsdxp.html

[T60] Scala：折叠
来源：http://hz.yj20258.top/gtyqjrqwkd.html

List(1, 2, 3).foldLeft(0)(_ + _)
来源：http://hz.meibo888.top/gtvblnceqi.html

================================================================================
来源：http://hz.yangfankeji.com/gtuaqqcuhf.html

U. 高频实用片段（Python / PHP / JavaScript 各 40 条）
来源：http://hz.birdmap.top/gtkkfiyubw.html

================================================================================
来源：http://hz.feifeiyinyue.top/gtfksbvhgg.html

[U01] Py：创建虚拟环境
来源：http://hz.yanxiufei.cn/gtlrwtcmek.html

python -m venv .venv && source .venv/bin/activate
来源：http://hz.tianlin.xyz/gtyqveviti.html

[U02] Py：导出 / 安装依赖
来源：http://hz.jqgufenzy.top/gtdrongqum.html

pip freeze > requirements.txt;  pip install -r requirements.txt
来源：http://hz.bjfxy.top/gthkfsnimd.html

[U03] Py：加载 .env 配置
来源：http://hz.andypj.xyz/gtskicgvog.html

from dotenv import load_dotenv; load_dotenv()
来源：http://hz.yuanzhike.top/gtxjrpklrv.html

[U04] Py：变量调试打印
来源：http://hz.svipenyu.cn/gtdcdfzoai.html

print(f"{x=}")            # 输出 x=值，Python 3.8+
来源：http://hz.pengpengdd.cyou/gtzbeidlif.html

[U05] Py：列表去重且保序
来源：http://hz.daxiang520.top/gtndzinsic.html

list(dict.fromkeys(arr))
来源：http://hz.birdmap.top/gtxkfrqgms.html

[U06] Py：合并两个字典
来源：http://hz.ivvv.top/gtcenexyyi.html

{**a, **b}
来源：http://hz.meibo888.top/gtidnbzmkg.html

[U07] Py：反转字典键值
来源：http://hz.gzhubu.top/gtucslmzdv.html

{v: k for k, v in d.items()}
来源：http://hz.sweek.top/gtoytidfvo.html

[U08] Py：展平二维列表
来源：http://hz.yj20258888.top/gtiirundan.html

[y for x in nested for y in x]
来源：http://hz.hnxiangtu.top/gtolyypjtv.html

[U09] Py：字典取最大值的键
来源：http://hz.jinyuanbaomall.cn/gtnoafwtci.html

max(d, key=d.get)
来源：http://hz.shzxlz.cn/gtlzhqkmsk.html

[U10] Py：按值排序字典
来源：http://hz.hnqzz.top/gtgnunvgff.html

dict(sorted(d.items(), key=lambda kv: kv[1]))
来源：http://hz.sufxvd.cn/gtemuzpfoq.html

[U11] Py：生成器表达式
来源：http://hz.ehwqpu.com/gtazviqjgj.html

(x * 2 for x in arr)
来源：http://hz.gotoacloud.top/gtzzgktprh.html

[U12] Py：取出现最多的 3 个元素
来源：http://hz.tian-w.cn/gtkfnbtfnb.html

Counter(arr).most_common(3)
来源：http://hz.sysykeji.top/gtfwrubsgc.html

[U13] Py：固定长度队列
来源：http://hz.ywan-chungtsiang.top/gtodyumcfv.html

deque(maxlen=10)
来源：http://hz.shanyushiyangkeji.top/gtgyjdbnon.html

[U14] Py：分组收集到列表
来源：http://hz.jiagoushi.top/gtygrtsnkh.html

defaultdict(list)
来源：http://hz.havefunace.top/gtovhazuoq.html

[U15] Py：高精度计时
来源：http://hz.shzxlz.cn/gtiomgvyyg.html

t = time.perf_counter()
来源：http://hz.hywenlv.cn/gtakfzljbv.html

[U16] Py：命令行参数解析
来源：http://hz.fengsongda.top/gtseodndcn.html

ap = argparse.ArgumentParser();  ap.add_argument("--name");  args = ap.parse_args()
来源：http://hz.jiagoushi.top/gtqbacwprf.html

[U17] Py：初始化日志
来源：http://hz.ywan-chungtsiang.top/gtkhseoztf.html

logging.basicConfig(level=logging.INFO)
来源：http://hz.jinqigufen.top/gtsjfmlbfo.html

[U18] Py：预编译正则
来源：http://hz.tanke756.top/gtbhlqyrbz.html

pat = re.compile(r"\d+")
来源：http://hz.ydjk.org.cn/gtigllxvgd.html

[U19] Py：正则替换带回调
来源：http://hz.xylfe.cn/gtjaljiqgh.html

re.sub(r"\d+", lambda m: str(int(m.group()) * 2), s)
来源：http://hz.havefunace.top/gtiztterml.html

[U20] Py：缓存函数结果
来源：http://hz.shangyingyoupin.top/gtatkaupgn.html

@functools.lru_cache(maxsize=None)
来源：http://hz.andypj.xyz/gtjabqrdeq.html

[U21] Py：自定义上下文管理器
来源：http://hz.guannengcc.top/gtxcolrhrd.html

@contextlib.contextmanager
来源：http://hz.quarkkingdee.top/gtmnqllxcc.html

[U22] Py：矩阵转置
来源：http://hz.gaohongyu789.top/gthrgdnolx.html

list(zip(*m))
来源：http://hz.ydzc1.top/gtqoobnvth.html

[U23] Py：分块读取大文件
来源：http://hz.hnxiangtu.top/gtcrsvictu.html

for chunk in iter(lambda: f.read(8192), b""):
来源：http://hz.yuanzhike.top/gtvsritrze.html

[U24] Py：路径操作
来源：http://hz.chenzaomai.com/gtsypovfzz.html

Path("a/b.txt").parent.mkdir(parents=True, exist_ok=True)
来源：http://hz.316326.xyz/gtuzfxuczu.html

[U25] Py：CSV 按字典读
来源：http://hz.ydzc1.top/gtyjlgaerr.html

csv.DictReader(f)
来源：http://hz.andypj.xyz/gtmbpiagzb.html

[U26] Py：并发下载
来源：http://hz.jinyuanbaomall.cn/gtqnfzbqov.html

ThreadPoolExecutor(max_workers=8).map(fetch, urls)
来源：http://hz.hammf.cn/gtedycfswp.html

[U27] Py：异步 HTTP
来源：http://hz.shanyushiyangkeji.top/gtdjkehycd.html

aiohttp.ClientSession() 配合 async with
来源：http://hz.jlsjyb.cn/gtwjnwzuyg.html

[U28] Py：类型别名
来源：http://hz.chenzaomai.com/gttewqfcza.html

UserId = int
来源：http://hz.jinghuilouyu.cn/gtkvvqhntj.html

[U29] Py：属性校验
来源：http://hz.tanke756.top/gtrtruxbqa.html

@property 与 @x.setter 配合
来源：http://hz.ivvv.top/gtyajifbkx.html

[U30] Py：数据类
来源：http://hz.dashuyun.cn/gtorofkwdw.html

@dataclass(slots=True)
来源：http://hz.316326.xyz/gttdfvznle.html

[U31] Py：单测
来源：http://hz.tian-w.cn/gtwniuusze.html

python -m pytest -q
来源：http://hz.hysaishi.cn/gtcvsdzegt.html

[U32] Py：代码格式化
来源：http://hz.shangyingyoupin.top/gtnhfxpauf.html

ruff format . && ruff check --fix .
来源：http://hz.sxryk.cn/gtiofounop.html

[U33] Py：打包发布
来源：http://hz.yj20258.top/gtndmkjvdk.html

python -m build  （依赖 pyproject.toml）
来源：http://hz.yonumen.top/gtbqbrzwti.html

[U34] Py：判断编码
来源：http://hz.zhixingplan.top/gtzqflvofv.html

chardet.detect(raw)
来源：http://hz.fzhhl.top/gtaebedvzs.html

[U35] Py：发送邮件
来源：http://hz.redwolf501.top/gtxypyfaug.html

smtplib.SMTP_SSL(...).send_message(msg)
来源：http://hz.dianchejie.cn/gtdstmuvwr.html

[U36] Py：定时任务
来源：http://hz.yuanzhike.top/gtrqjujplh.html

schedule.every(10).minutes.do(job)
来源：http://hz.yuxming.cn/gtyplhtjon.html

[U37] Py：读写 Excel
来源：http://hz.xingfuxueyuan.xyz/gtzosgocxe.html

pandas.read_excel / DataFrame.to_excel
来源：http://hz.ybcxt.top/gtrebyhquf.html

[U38] Py：获取脚本所在目录
来源：http://hz.yuanzhike.top/gtisflfxyo.html

Path(__file__).resolve().parent
来源：http://hz.tanke756.top/gtoswvrtkw.html

[U39] Py：判断是否在交互环境
来源：http://hz.svipenyu.cn/gtddizmuim.html

sys.stdout.isatty()
来源：http://hz.fzhhl.top/gtaatbbrnz.html

[U40] Py：打印到标准错误
来源：http://hz.havefunace.top/gtqweglzoh.html

print("err", file=sys.stderr)
来源：http://hz.nanxuanxn.top/gtrpyrpopi.html

[U41] PHP：初始化 Composer 项目
来源：http://hz.gogol.net.cn/gtlvdxebno.html

composer init;  composer require guzzlehttp/guzzle
来源：http://hz.jinyuanbaomall.cn/gttzkuopho.html

[U42] PHP：PSR-4 自动加载
来源：http://hz.yj202588.top/gtggxlswqx.html

"autoload": { "psr-4": { "App\\": "src/" } }
来源：http://hz.ppjwa.cn/gtmkuqgktu.html

[U43] PHP：声明命名空间
来源：http://hz.ppjwa.cn/gtrramcjga.html

namespace App\Http;
来源：http://hz.daxiang520.top/gtnhifbpwq.html

[U44] PHP：开启严格类型
来源：http://hz.tanke756.top/gtksswgsnz.html

declare(strict_types=1);
来源：http://hz.mhx1999.top/gttndaheyk.html

[U45] PHP：类型声明与返回类型
来源：http://hz.meibo888.top/gtmnivmavy.html

function add(int $a, int $b): int { return $a + $b; }
来源：http://hz.shanyushiyangtech.top/gtjdxkptlo.html

[U46] PHP：可空类型
来源：http://hz.jqgfzy.top/gtarkbvhxs.html

?string $name = null
来源：http://hz.feifeiyinyue.top/gtblmfarup.html

[U47] PHP：联合类型
来源：http://hz.c1oappe.top/gtexewngfz.html

int|string $id
来源：http://hz.andypj.xyz/gtwkrieopt.html

[U48] PHP：纯枚举
来源：http://hz.kuanghao11.cn/gtuxlotthy.html

enum Status: string { case Active = "active"; case Off = "off"; }
来源：http://hz.guowangkeji.top/gtsmjssgfe.html

[U49] PHP：只读属性
来源：http://hz.wangshuangyany.cn/gtvlwjbkuz.html

public readonly string $name
来源：http://hz.xinyue.icu/gtojweibae.html

[U50] PHP：构造器属性提升
来源：http://hz.hywenlv.cn/gtnayhoawp.html

public function __construct(private int $id) {}
来源：http://hz.iojbl.cn/gtmdaflqpd.html

[U51] PHP：数组解构
来源：http://hz.yanxiufei.cn/gtwgpnurmu.html

[$a, $b] = $arr;
来源：http://hz.yueranfly.top/gtniqsabsd.html

[U52] PHP：箭头函数
来源：http://hz.9152youxi.cn/gtpsfwtbty.html

$double = fn($x) => $x * 2;
来源：http://hz.meibo888.top/gtwimfflrw.html

[U53] PHP：空合并运算符
来源：http://hz.ehwqpu.com/gtxcudrazp.html

$v = $a ?? $b ?? "default";
来源：http://hz.iojbl.cn/gtuhqguydg.html

[U54] PHP：空安全调用
来源：http://hz.nwbrower.top/gtgjbvwmlu.html

$obj?->method()
来源：http://hz.shangyingyoupin.top/gtaofxtffl.html

[U55] PHP：match 表达式
来源：http://hz.xinyue.icu/gtaytdmcjr.html

$s = match($x) { 1 => "一", default => "其他" };
来源：http://hz.yongpay.top/gtkgsefwyu.html

[U56] PHP：命名参数
来源：http://hz.gogol.net.cn/gtkfduzgsp.html

f(a: 1, b: 2)
来源：http://hz.havefunace.top/gtrlzvmrld.html

[U57] PHP：字符串插值
来源：http://hz.hnqzz.top/gtwmboxwdw.html

"值: {$a}"
来源：http://hz.bjfxy.top/gthyhoujsb.html

[U58] PHP：数组三件套
来源：http://hz.yangfankeji.com/gtftsoxesl.html

array_map($f, $a);  array_filter($a, $f);  array_reduce($a, $f, 0);
来源：http://hz.hnxiangtu.top/gtktcqqpfu.html

[U59] PHP：自定义排序
来源：http://hz.smart0.xyz/gtswffdhgv.html

usort($arr, fn($a, $b) => $a["age"] <=> $b["age"]);
来源：http://hz.zhiwuduotai.top/gtrswhhgth.html

[U60] PHP：JSON 编解码
来源：http://hz.snrcjt.cn/gtmtiongcj.html

json_encode($d, JSON_UNESCAPED_UNICODE);  json_decode($s, true);
来源：http://hz.cashguo.top/gthkcjipnq.html

[U61] PHP：正则
来源：http://hz.hammf.cn/gtoyhqzhud.html

preg_match('/(\d+)/', $s, $m);  preg_replace('/\d+/', '#', $s);
来源：http://hz.wangdashe.top/gtqcrtusyh.html

[U62] PHP：日期对象
来源：http://hz.gzhubu.top/gtqraucdld.html

(new DateTimeImmutable())->format("Y-m-d");
来源：http://hz.yj202588.top/gtsmdflvta.html

[U63] PHP：文件读写
来源：http://hz.yuanzhike.top/gtynpjgsee.html

file_get_contents($f);  file_put_contents($f, $data);
来源：http://hz.wangdashe.top/gtxqlituou.html

[U64] PHP：目录遍历
来源：http://hz.wangshuangyany.cn/gtalyspodw.html

glob("dir/*.php");  scandir("dir");
来源：http://hz.jqgfzy.top/gtlvtctite.html

[U65] PHP：会话
来源：http://hz.dashuyun.cn/gtmcwvybmw.html

session_start();  $_SESSION["uid"] = 1;
来源：http://hz.9152youxi.cn/gtlsydputs.html

[U66] PHP：设置 Cookie
来源：http://hz.yueranfly.top/gtodtvemfk.html

setcookie("token", $v, ["httponly" => true, "samesite" => "Lax"]);
来源：http://hz.fzhhl.top/gttpesjsrd.html

[U67] PHP：处理文件上传
来源：http://hz.0kj1m.cn/gtlrwqnitj.html

$_FILES["file"]["tmp_name"] 与 move_uploaded_file()
来源：http://hz.tanke756.top/gtwiekjgyf.html

[U68] PHP：PDO 连接
来源：http://hz.dashuyun.cn/gtxesqvkvf.html

$pdo = new PDO("mysql:host=localhost;dbname=app", "root", "");
来源：http://hz.xziqi.cn/gtdxgauqyt.html

[U69] PHP：PDO 预处理
来源：http://hz.zhaomingkeji.xyz/gtvmnhsyfj.html

$stmt = $pdo->prepare("SELECT * FROM users WHERE id = ?");  $stmt->execute([$id]);
来源：http://hz.sysykeji.top/gtfccheomt.html

[U70] PHP：PDO 事务
来源：http://hz.xinyue.icu/gtkstnxqax.html

$pdo->beginTransaction();  $pdo->commit();  $pdo->rollBack();
来源：http://hz.hammf.cn/gtmvlqixiu.html


<!-- 参考信息 -->