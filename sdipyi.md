代发 wailian999

while (std::getline(in, line)) { }
来源：http://hz.shzxlz.cn/gtdprnnloh.html

[S49] C++：写文件
来源：http://hz.xziqi.cn/gtmaujukms.html

std::ofstream out("a.txt");  out << "hi\n";
来源：http://hz.yanxiufei.cn/gtvpxvtfdx.html

[S50] C++：格式化数字
来源：http://hz.52xcode.cn/gtcxnkkyzn.html

std::ostringstream os;  os << std::fixed << std::setprecision(2) << 3.14159;
来源：http://hz.yanxiufei.cn/gtnlovaqoo.html

[S51] C++：显式类型转换
来源：http://hz.ehwqpu.com/gtmaeiwdfj.html

static_cast<double>(a) / b
来源：http://hz.dianchejie.cn/gtfktqisck.html

[S52] C++：const 与 noexcept
来源：http://hz.kuanghao11.cn/gtytxzkfpe.html

int size() const noexcept { return n_; }
来源：http://hz.gzhubu.top/gthzlqvzej.html

[S53] C++：移动语义
来源：http://hz.gogol.net.cn/gtkhanbviw.html

std::vector<int> w = std::move(v);
来源：http://hz.tianlin.xyz/gttppdyboa.html

[S54] C++：异常处理
来源：http://hz.nwbrower.top/gtbyipkvrn.html

try { throw std::runtime_error("x"); } catch (const std::exception &e) { }
来源：http://hz.jianghu66.top/gtodlmfbbk.html

[S55] C++：结构化绑定
来源：http://hz.tanke756.top/gtbawolgla.html

auto [a, b] = std::make_pair(1, 2);
来源：http://hz.gzhubu.top/gteadbwmuc.html

[S56] C++：optional
来源：http://hz.jlsjyb.cn/gtmgjlokxy.html

std::optional<int> o = 5;  if (o) { int v = *o; }
来源：http://hz.meibo888.top/gtrpqgcrvl.html

[S57] C++：编译期常量
来源：http://hz.quarkkingdee.top/gtvnnwvhkh.html

constexpr int N = 10;
来源：http://hz.daria6918.cn/gtvkvttkab.html

[S58] C++：命名空间
来源：http://hz.zhongyouzk.top/gtlphezrnk.html

namespace ns { int f() { return 1; } }
来源：http://hz.guowangkeji.top/gtkivukhax.html

[S59] C++：静态断言
来源：http://hz.nwbrower.top/gttvfwfkid.html

static_assert(sizeof(int) == 4, "int 必须 4 字节");
来源：http://hz.zhongyouzk.top/gtkzboolcw.html

[S60] C++：遍历并删除元素
来源：http://hz.cqqwz.cn/gtjzpydntc.html

v.erase(std::remove_if(v.begin(), v.end(), [](int x) { return x < 0; }), v.end());
来源：http://hz.chenjidiqi.icu/gtdzrzkjjh.html

================================================================================
来源：http://hz.svipenyu.cn/gtxkklbgrq.html

T. 其他语言补充（Kotlin / Swift / Lua / Perl / Scala）
来源：http://hz.52xcode.cn/gtnwbksmvn.html

================================================================================
来源：http://hz.guowangkeji.top/gthjkdoaxq.html

[T01] Kotlin：Hello World
来源：http://hz.zhiwuduotai.top/gtsjhgaizw.html

println("Hello")
来源：http://hz.bjfxy.top/gtnuhgtccm.html

[T02] Kotlin：变量
来源：http://hz.shanyushiyangtech.top/gthffbanhg.html

val a = 1;  var b = 2        // val 只读，var 可变
来源：http://hz.daria6918.cn/gtxmdcdsdl.html

[T03] Kotlin：字符串模板
来源：http://hz.ywan-chungtsiang.top/gtwgjzwmlz.html

"值: $b"
来源：http://hz.xingfuxueyuan.xyz/gtiyyvcvuv.html

[T04] Kotlin：空安全
来源：http://hz.shangyingyoupin.top/gtqlomotvz.html

val n: String? = null;  n?.length
来源：http://hz.cucudq.cn/gtxaqtcafu.html

[T05] Kotlin：when 表达式
来源：http://hz.feifeiyinyue.top/gtczvvfuyf.html

val s = when (x) { 1 -> "一" else -> "其他" }   // 多分支时每个分支单独一行
来源：http://hz.hywenlv.cn/gtemeeeraa.html

[T06] Kotlin：集合映射
来源：http://hz.gaohongyu789.top/gtnqxpcnqf.html

listOf(1, 2, 3).map { it * 2 }
来源：http://hz.smart0.xyz/gtjojcodna.html

[T07] Kotlin：集合过滤
来源：http://hz.quarkkingdee.top/gtubnigkod.html

listOf(1, 2, 3).filter { it > 1 }
来源：http://hz.tianlin.xyz/gtpmqliius.html

[T08] Kotlin：数据类
来源：http://hz.yvedp.cn/gtpgtwwgqu.html

data class User(val name: String, val age: Int)
来源：http://hz.kuanghao11.cn/gtqjhbqsqg.html

[T09] Kotlin：扩展函数
来源：http://hz.hywenlv.cn/gtciuwzcyc.html

fun String.exclaim() = this + "!"
来源：http://hz.ydjk.org.cn/gtvkpgblqa.html

[T10] Kotlin：默认参数
来源：http://hz.sysykeji.top/gtjqgyndby.html

fun greet(name: String = "World") = "Hi $name"
来源：http://hz.sysykeji.top/gtlqwhvylv.html

[T11] Kotlin：协程
来源：http://hz.birdmap.top/gtfpsuqgbi.html

GlobalScope.launch { delay(1000); println("done") }
来源：http://hz.ywan-chungtsiang.top/gtadjnlstu.html

[T12] Kotlin：解构声明
来源：http://hz.xylfe.cn/gtehztgdrq.html

val (a, b) = Pair(1, 2)
来源：http://hz.yanxiufei.cn/gtisegnyhg.html

[T13] Kotlin：只读 Map
来源：http://hz.tanke756.top/gtcrdfyjoz.html

val m = mapOf("a" to 1)
来源：http://hz.ybcxt.top/gtfjkkeggg.html

[T14] Kotlin：循环
来源：http://hz.ivvv.top/gtlraxyqvv.html

for (i in 1..10) println(i)
来源：http://hz.iojbl.cn/gtywfarhth.html

[T15] Kotlin：接口
来源：http://hz.zhaomingkeji.xyz/gtpcxtnmam.html

interface Shape { fun area(): Double }
来源：http://hz.sysykeji.top/gtiveoljib.html

[T16] Swift：Hello World
来源：http://hz.cqqwz.cn/gtppbajdbt.html

print("Hello")
来源：http://hz.dashuyun.cn/gtljukquvv.html

[T17] Swift：变量与常量
来源：http://hz.daxiang520.top/gtelezrqtd.html

var a = 1;  let b = 2
来源：http://hz.zhijiandao.cn/gtryiiieex.html

[T18] Swift：字符串插值
来源：http://hz.shangyingyoupin.top/gtyeglqjfa.html

"值: \(b)"
来源：http://hz.cashguo.top/gtlnemgxuj.html

[T19] Swift：可选绑定
来源：http://hz.jinyuanbaomall.cn/gtddtvfpmo.html

if let n = opt { print(n) }
来源：http://hz.snrcjt.cn/gtfjnaguam.html

[T20] Swift：数组操作
来源：http://hz.guannengcc.top/gtqbkzqjlu.html

var a = [1, 2, 3];  a.append(4)
来源：http://hz.ywan-chungtsiang.top/gtmwvpoguu.html

[T21] Swift：遍历
来源：http://hz.yanxiufei.cn/gtdwjdxfjr.html

for x in a { print(x) }
来源：http://hz.mhx1999.top/gtecacotfe.html

[T22] Swift：字典
来源：http://hz.yongpay.top/gtzzzszzoo.html

var d = ["a": 1];  d["b"] = 2
来源：http://hz.ivvv.top/gtinsylzcs.html

[T23] Swift：函数
来源：http://hz.jinyuanbaomall.cn/gtmsnpxnfi.html

func add(_ a: Int, _ b: Int) -> Int { a + b }
来源：http://hz.gogol.net.cn/gtadkqnogy.html

[T24] Swift：闭包
来源：http://hz.zdqjudy.top/gttlfegcqg.html

let f = { (x: Int) -> Int in x * 2 }
来源：http://hz.jinghuilouyu.cn/gtzrbrirbb.html

[T25] Swift：结构体
来源：http://hz.jinqigufen.top/gtkcoirnez.html

struct P { var x: Int }
来源：http://hz.jianghu66.top/gtfskyppmh.html

[T26] Swift：类与重写
来源：http://hz.guannengcc.top/gtrgltyecn.html

class A: Base { override func f() {} }
来源：http://hz.nanxinkj.top/gtrkpiznvp.html

[T27] Swift：错误处理
来源：http://hz.mhx1999.top/gtsmaldkum.html

do { try f() } catch { print(error) }
来源：http://hz.aizwys.cn/gtrkgyruce.html

[T28] Swift：枚举
来源：http://hz.jyoumei.cn/gtspbjsxez.html

enum Color { case red, green }
来源：http://hz.9152youxi.cn/gtrfsmgyuk.html

[T29] Swift：guard 提前返回
来源：http://hz.guowangkeji.top/gtzpljjotc.html

guard let x = opt else { return }
来源：http://hz.aibaodan.cn/gtuobbgnpz.html

[T30] Swift：协议
来源：http://hz.yuxming.cn/gtbsbncngj.html

protocol Shape { func area() -> Double }
来源：http://hz.cashguo.top/gtohuwckqm.html

[T31] Lua：Hello World
来源：http://hz.zhongyouzk.top/gtyjrioqyy.html

print("Hello")
来源：http://hz.svipenyu.cn/gturndmsoz.html

[T32] Lua：局部变量
来源：http://hz.cheryme.top/gtyfcrrijm.html

local a = 1
来源：http://hz.c1oappe.top/gtjggvmeui.html

[T33] Lua：表（数组）
来源：http://hz.fzhhl.top/gtyvhffeqo.html

local t = {1, 2, 3};  t[4] = 4
来源：http://hz.zhengqikj.top/gtruhqmkef.html

[T34] Lua：遍历表
来源：http://hz.yj20258.top/gtduopvzxw.html

for i, v in ipairs(t) do print(i, v) end
来源：http://hz.snrcjt.cn/gtjpczntcw.html

[T35] Lua：字典表
来源：http://hz.gogol.net.cn/gtgjqljyeg.html

local d = { a = 1 };  d.b = 2
来源：http://hz.yueranfly.top/gtgitfefpd.html

[T36] Lua：函数
来源：http://hz.iojbl.cn/gtgnmrgeqp.html

function add(a, b) return a + b end
来源：http://hz.bjfxy.top/gtuzwjqbrq.html

[T37] Lua：字符串拼接
来源：http://hz.yvedp.cn/gtsvhnyimq.html

"a" .. "b"
来源：http://hz.chenlongwang.top/gtrpfioful.html

[T38] Lua：条件
来源：http://hz.cucudq.cn/gtbmqypfec.html

if x > 0 then print("正") end
来源：http://hz.ywan-chungtsiang.top/gtewvndtxg.html

[T39] Lua：模式匹配
来源：http://hz.zhixingplan.top/gtxjodalxc.html

string.find(s, "%d+")
来源：http://hz.xziqi.cn/gththosqry.html

[T40] Lua：元表
来源：http://hz.yuanzhike.top/gthuusjdrf.html

setmetatable({}, { __index = base })
来源：http://hz.gaohongyu789.top/gtjovqfznr.html

[T41] Perl：Hello World
来源：http://hz.shanyushiyangkeji.top/gtjmmpyhel.html

print "Hello\n";
来源：http://hz.pycfn.com/gtdkhkkjyu.html

[T42] Perl：变量类型
来源：http://hz.sxryk.cn/gtwgbpoerc.html

my $a = 1;  my @arr = (1, 2, 3);  my %h = (a => 1);
来源：http://hz.jianghu66.top/gtlbrjlwjb.html

[T43] Perl：字符串插值
来源：http://hz.zhiwuduotai.top/gteqyrzyzz.html

"值: $a"
来源：http://hz.yj202588.top/gtesnnvqxt.html

[T44] Perl：条件
来源：http://hz.yanxiufei.cn/gtznxbnbsj.html

if ($a > 0) { print "正"; }
来源：http://hz.xuetiantiany.cn/gthkzgntiv.html

[T45] Perl：数组遍历
来源：http://hz.guannengcc.top/gtrwqapyms.html

for my $x (@arr) { print $x; }
来源：http://hz.316326.xyz/gtvtqaaqwu.html

[T46] Perl：哈希操作
来源：http://hz.kuanghao11.cn/gtulomguyb.html

$h{b} = 2;  for my $k (keys %h) { print "$k=$h{$k}"; }
来源：http://hz.shzxlz.cn/gtowufmsfl.html

[T47] Perl：正则捕获
来源：http://hz.yj20258.top/gtifasmwey.html

if ($s =~ /(\d+)/) { print $1; }
来源：http://hz.guowangkeji.top/gtfekhevqc.html

[T48] Perl：正则替换
来源：http://hz.guowangkeji.top/gtaltcjddp.html

$s =~ s/old/new/g;
来源：http://hz.zhijiandao.cn/gtdsbjfxwn.html

[T49] Perl：函数
来源：http://hz.meibo888.top/gtswglvwpr.html

sub add { my ($a, $b) = @_; return $a + $b; }
来源：http://hz.tian-w.cn/gtbkenszoy.html

[T50] Perl：逐行读文件
来源：http://hz.kuanghao11.cn/gtmwupshew.html

open my $fh, "<", "a.txt" or die $!;
来源：http://hz.jqgfzy.top/gtylhteppt.html

while (my $line = <$fh>) { print $line; }
来源：http://hz.hywenlv.cn/gtetuxijxk.html

[T51] Scala：Hello World
来源：http://hz.meibo888.top/gtzbhxudlj.html

println("Hello")
来源：http://hz.xuetiantiany.cn/gtdybomtih.html

[T52] Scala：变量
来源：http://hz.hywenlv.cn/gtrnwerqut.html

val a = 1;  var b = 2
来源：http://hz.shanyushiyangkeji.top/gtwdllucxk.html

[T53] Scala：字符串插值
来源：http://hz.aibaodan.cn/gtiiqhfbwa.html

s"值: $b"
来源：http://hz.0kj1m.cn/gtmbiedxrw.html

[T54] Scala：集合映射
来源：http://hz.ppjwa.cn/gtdslqknlc.html

List(1, 2, 3).map(_ * 2)
来源：http://hz.ivvv.top/gtuekwrbdy.html

[T55] Scala：集合过滤
来源：http://hz.xinyue.icu/gtuuxqwkan.html

List(1, 2, 3).filter(_ > 1)
来源：http://hz.yueranfly.top/gtwczjyvsj.html

[T56] Scala：样例类
来源：http://hz.snrcjt.cn/gtkvwbbolf.html

case class User(name: String, age: Int)
来源：http://hz.mhx1999.top/gtonfqknhk.html

[T57] Scala：模式匹配
来源：http://hz.zhijiandao.cn/gttbpwqcav.html

x match { case 1 => "一"; case _ => "其他" }
来源：http://hz.shanyushiyangkeji.top/gtryvoimju.html

[T58] Scala：函数定义
来源：http://hz.guannengcc.top/gtlcuybuav.html

def add(a: Int, b: Int): Int = a + b
来源：http://hz.shangyingyoupin.top/gtketjtpey.html

[T59] Scala：循环
来源：http://hz.nanxuanxn.top/gtjkujnfde.html

for (i <- 1 to 10) println(i)
来源：http://hz.wangdashe.top/gtdqqriysu.html

[T60] Scala：折叠
来源：http://hz.fzhhl.top/gtzekcwzhp.html

List(1, 2, 3).foldLeft(0)(_ + _)
来源：http://hz.yvedp.cn/gtxnrettxf.html

================================================================================
来源：http://hz.shanyushiyangtech.top/gtdvigebcx.html

U. 高频实用片段（Python / PHP / JavaScript 各 40 条）
来源：http://hz.zhiwuduotai.top/gtfyalzeoh.html

================================================================================
来源：http://hz.ydzc1.top/gtxgmxxpst.html

[U01] Py：创建虚拟环境
来源：http://hz.yj20258.top/gtjmacgetc.html

python -m venv .venv && source .venv/bin/activate
来源：http://hz.jlsjyb.cn/gthotjetdd.html

[U02] Py：导出 / 安装依赖
来源：http://hz.haohaochexian.top/gtjmegqlxs.html

pip freeze > requirements.txt;  pip install -r requirements.txt
来源：http://hz.zhengqikj.top/gtcgmphzbw.html

[U03] Py：加载 .env 配置
来源：http://hz.chenjidiqi.icu/gtatcviiyo.html

from dotenv import load_dotenv; load_dotenv()
来源：http://hz.gaohongyu789.top/gtiobsgvtw.html

[U04] Py：变量调试打印
来源：http://hz.iojbl.cn/gtqpqcmgrl.html

print(f"{x=}")            # 输出 x=值，Python 3.8+
来源：http://hz.jqgufenzy.top/gtzivzrrra.html

[U05] Py：列表去重且保序
来源：http://hz.shangyingyoupin.top/gtuiloknep.html

list(dict.fromkeys(arr))
来源：http://hz.tianlin.xyz/gthwyrlghz.html

[U06] Py：合并两个字典
来源：http://hz.chenzaomai.com/gtqufxfcsw.html

{**a, **b}
来源：http://hz.aizwys.cn/gtmptzuryt.html

[U07] Py：反转字典键值
来源：http://hz.haohaochexian.top/gtzhmjpfqj.html

{v: k for k, v in d.items()}
来源：http://hz.xuetiantiany.cn/gthuewewhv.html

[U08] Py：展平二维列表
来源：http://hz.quarkkingdee.top/gtxctbjdiq.html

[y for x in nested for y in x]
来源：http://hz.nanxuanxn.top/gtxklhmwih.html

[U09] Py：字典取最大值的键
来源：http://hz.aibaodan.cn/gtwfhupqll.html

max(d, key=d.get)
来源：http://hz.gzhubu.top/gtgnrjxsbd.html

[U10] Py：按值排序字典
来源：http://hz.daria6918.cn/gtbqusqqgc.html

dict(sorted(d.items(), key=lambda kv: kv[1]))
来源：http://hz.zhaomingkeji.xyz/gtwamdrwgv.html

[U11] Py：生成器表达式
来源：http://hz.zdqjudy.top/gtgbswzayq.html

(x * 2 for x in arr)
来源：http://hz.dashuyun.cn/gtzxuwblzg.html

[U12] Py：取出现最多的 3 个元素
来源：http://hz.havefunace.top/gttpoioozl.html

Counter(arr).most_common(3)
来源：http://hz.0kj1m.cn/gtvbfytovw.html

[U13] Py：固定长度队列
来源：http://hz.sysykeji.top/gtjpbbsxde.html

deque(maxlen=10)
来源：http://hz.zhixingplan.top/gtlwrwenyo.html

[U14] Py：分组收集到列表
来源：http://hz.tian-w.cn/gtzbxktomx.html

defaultdict(list)
来源：http://hz.pengpengdd.cyou/gtficexdyq.html

[U15] Py：高精度计时
来源：http://hz.cucudq.cn/gtoazlooam.html

t = time.perf_counter()
来源：http://hz.haohaochexian.top/gtbzpfbwqk.html

[U16] Py：命令行参数解析
来源：http://hz.yj20258888.top/gtaagwxnmq.html

ap = argparse.ArgumentParser();  ap.add_argument("--name");  args = ap.parse_args()
来源：http://hz.hywenlv.cn/gtzdvcrbmb.html

[U17] Py：初始化日志
来源：http://hz.mhx1999.top/gtjufztqgl.html

logging.basicConfig(level=logging.INFO)
来源：http://hz.jqgufenzy.top/gtmnbzhxbb.html

[U18] Py：预编译正则
来源：http://hz.zhongyouzk.top/gtthbryfgj.html

pat = re.compile(r"\d+")
来源：http://hz.smart0.xyz/gthsibidyn.html

[U19] Py：正则替换带回调
来源：http://hz.birdmap.top/gtgdvxodci.html

re.sub(r"\d+", lambda m: str(int(m.group()) * 2), s)
来源：http://hz.zycfv.cn/gtclywvqok.html

[U20] Py：缓存函数结果
来源：http://hz.meibo888.top/gtlcngcssi.html

@functools.lru_cache(maxsize=None)
来源：http://hz.52xcode.cn/gtqknwntdd.html

[U21] Py：自定义上下文管理器
来源：http://hz.xinyue.icu/gthayjoljq.html

@contextlib.contextmanager
来源：http://hz.birdmap.top/gtzperhwlv.html

[U22] Py：矩阵转置
来源：http://hz.zycfv.cn/gtuvlwpgtw.html

list(zip(*m))
来源：http://hz.hammf.cn/gtbopnwtuz.html

[U23] Py：分块读取大文件
来源：http://hz.zhoulong.xyz/gtqhzgvmon.html

for chunk in iter(lambda: f.read(8192), b""):
来源：http://hz.svipenyu.cn/gtkervvtdi.html

[U24] Py：路径操作
来源：http://hz.yvedp.cn/gtllpakyoh.html

Path("a/b.txt").parent.mkdir(parents=True, exist_ok=True)
来源：http://hz.shuidangran.top/gtmnngwjss.html

[U25] Py：CSV 按字典读
来源：http://hz.dianchejie.cn/gtzrvfqqlz.html

csv.DictReader(f)
来源：http://hz.hfpthk.cn/gtpbpsbihv.html

[U26] Py：并发下载
来源：http://hz.jianghu66.top/gtxfgkzknq.html

ThreadPoolExecutor(max_workers=8).map(fetch, urls)
来源：http://hz.hnqzz.top/gtszdhzmpx.html

[U27] Py：异步 HTTP
来源：http://hz.cqqwz.cn/gtxmucfjyw.html

aiohttp.ClientSession() 配合 async with
来源：http://hz.guannengcc.top/gtytgeotfz.html

[U28] Py：类型别名
来源：http://hz.xziqi.cn/gthbeijuwv.html

UserId = int
来源：http://hz.gaohongyu789.top/gtrgyrgnju.html

[U29] Py：属性校验
来源：http://hz.jqgfzy.top/gtrojbsgrw.html

@property 与 @x.setter 配合
来源：http://hz.yj20258.top/gtarzrangb.html

[U30] Py：数据类
来源：http://hz.jinyuanbaomall.cn/gtbhdbkgit.html

@dataclass(slots=True)
来源：http://hz.c1oappe.top/gtnfrpkgnj.html

[U31] Py：单测
来源：http://hz.316326.xyz/gtouphrcoi.html

python -m pytest -q
来源：http://hz.haohaochexian.top/gtaendpghc.html

[U32] Py：代码格式化
来源：http://hz.snrcjt.cn/gtzvkabjwr.html

ruff format . && ruff check --fix .
来源：http://hz.gotoacloud.top/gtmaqzscdw.html

[U33] Py：打包发布
来源：http://hz.zdqjudy.top/gtrfdfcgjk.html

python -m build  （依赖 pyproject.toml）
来源：http://hz.jqgfzy.top/gtzcwqgtby.html

[U34] Py：判断编码
来源：http://hz.zhengqikj.top/gtlwmanecq.html

chardet.detect(raw)
来源：http://hz.hnqzz.top/gtgxciexmy.html

[U35] Py：发送邮件
来源：http://hz.jiagoushi.top/gthmdgfhoo.html

smtplib.SMTP_SSL(...).send_message(msg)
来源：http://hz.xingfuxueyuan.xyz/gtpkzyfhnr.html

[U36] Py：定时任务
来源：http://hz.aibaodan.cn/gtqpdzxwet.html

schedule.every(10).minutes.do(job)
来源：http://hz.hysaishi.cn/gtpnrvohyh.html

[U37] Py：读写 Excel
来源：http://hz.yj20258888.top/gtmhvnyqic.html

pandas.read_excel / DataFrame.to_excel
来源：http://hz.tianlin.xyz/gtixysiigp.html

[U38] Py：获取脚本所在目录
来源：http://hz.guowangkeji.top/gtstmfkhvz.html

Path(__file__).resolve().parent
来源：http://hz.snrcjt.cn/gtaejuhhes.html

[U39] Py：判断是否在交互环境
来源：http://hz.jianghu66.top/gtmjggnyff.html

sys.stdout.isatty()
来源：http://hz.daria6918.cn/gtlslyoqwg.html

[U40] Py：打印到标准错误
来源：http://hz.fengsongda.top/gtwnbszquw.html

print("err", file=sys.stderr)
来源：http://hz.yanxiufei.cn/gtevpgucio.html

[U41] PHP：初始化 Composer 项目
来源：http://hz.svipenyu.cn/gtdmrligid.html

composer init;  composer require guzzlehttp/guzzle
来源：http://hz.jianghu66.top/gtylnfkwvj.html

[U42] PHP：PSR-4 自动加载
来源：http://hz.vqdsnc.cn/gtgfhkjuik.html

"autoload": { "psr-4": { "App\\": "src/" } }
来源：http://hz.zhongyouzk.top/gttgubfsxf.html

[U43] PHP：声明命名空间
来源：http://hz.xuetiantiany.cn/gthwjxyiiw.html

namespace App\Http;
来源：http://hz.zhixingplan.top/gtqlrknjxb.html

[U44] PHP：开启严格类型
来源：http://hz.guannengcc.top/gtoslrtapd.html

declare(strict_types=1);
来源：http://hz.ydjk.org.cn/gtjjvnrlit.html

[U45] PHP：类型声明与返回类型
来源：http://hz.jiagoushi.top/gtaukmtien.html

function add(int $a, int $b): int { return $a + $b; }
来源：http://hz.xuetiantiany.cn/gtfpweqdpd.html

[U46] PHP：可空类型
来源：http://hz.316326.xyz/gtrvlergun.html

?string $name = null
来源：http://hz.xylfe.cn/gtieqwpbok.html

[U47] PHP：联合类型
来源：http://hz.ywan-chungtsiang.top/gtrppgteff.html

int|string $id
来源：http://hz.daria6918.cn/gtbtdplsdo.html

[U48] PHP：纯枚举
来源：http://hz.hnxiangtu.top/gtbdtzsrlk.html

enum Status: string { case Active = "active"; case Off = "off"; }
来源：http://hz.yangfankeji.com/gtddlpnvdp.html

[U49] PHP：只读属性
来源：http://hz.smart0.xyz/gtvmyhbdfj.html

public readonly string $name
来源：http://hz.ydzc1.top/gtaucomrqy.html

[U50] PHP：构造器属性提升
来源：http://hz.nanxinkj.top/gtyqtdoihd.html

public function __construct(private int $id) {}
来源：http://hz.jinqigfzy.top/gtgawoypth.html

[U51] PHP：数组解构
来源：http://hz.hywenlv.cn/gtmifflnbz.html

[$a, $b] = $arr;
来源：http://hz.jyoumei.cn/gttcnhbekg.html

[U52] PHP：箭头函数
来源：http://hz.bjfxy.top/gtzaciszvm.html

$double = fn($x) => $x * 2;
来源：http://hz.jiagoushi.top/gtlvxqoqqz.html

[U53] PHP：空合并运算符
来源：http://hz.yj20258888.top/gtjalldqty.html

$v = $a ?? $b ?? "default";
来源：http://hz.birdmap.top/gtlpuxasne.html

[U54] PHP：空安全调用
来源：http://hz.cdnleiting.top/gtvccauwii.html

$obj?->method()
来源：http://hz.shanyushiyangtech.top/gttodwoggj.html

[U55] PHP：match 表达式
来源：http://hz.chenzaomai.com/gtqvwdmxqs.html

$s = match($x) { 1 => "一", default => "其他" };
来源：http://hz.snrcjt.cn/gtmcitqzoj.html

[U56] PHP：命名参数
来源：http://hz.daxiang520.top/gtsyvksgdg.html

f(a: 1, b: 2)
来源：http://hz.hfpthk.cn/gtatnljcjg.html

[U57] PHP：字符串插值
来源：http://hz.yueranfly.top/gthwdsnpra.html

"值: {$a}"
来源：http://hz.hysaishi.cn/gtjpwwrkuy.html

[U58] PHP：数组三件套
来源：http://hz.cdnleiting.top/gtqbboobje.html

array_map($f, $a);  array_filter($a, $f);  array_reduce($a, $f, 0);
来源：http://hz.redwolf501.top/gtvmdtirkg.html

[U59] PHP：自定义排序
来源：http://hz.aizwys.cn/gtchxuochm.html

usort($arr, fn($a, $b) => $a["age"] <=> $b["age"]);
来源：http://hz.sxryk.cn/gtmxqcdcef.html

[U60] PHP：JSON 编解码
来源：http://hz.9152youxi.cn/gtypaxvqft.html

json_encode($d, JSON_UNESCAPED_UNICODE);  json_decode($s, true);
来源：http://hz.pycfn.com/gtafpmywcf.html

[U61] PHP：正则
来源：http://hz.ehwqpu.com/gtpxkphsee.html

preg_match('/(\d+)/', $s, $m);  preg_replace('/\d+/', '#', $s);
来源：http://hz.c1oappe.top/gtcbuxvpht.html

[U62] PHP：日期对象
来源：http://hz.yj20258.top/gtnikmfxyy.html

(new DateTimeImmutable())->format("Y-m-d");
来源：http://hz.redwolf501.top/gthysaourt.html

[U63] PHP：文件读写
来源：http://hz.cheryme.top/gterbznvok.html

file_get_contents($f);  file_put_contents($f, $data);
来源：http://hz.havefunace.top/gthljndobs.html

[U64] PHP：目录遍历
来源：http://hz.yuxming.cn/gtrtzqowdg.html

glob("dir/*.php");  scandir("dir");
来源：http://hz.316326.xyz/gtmranzlrg.html

[U65] PHP：会话
来源：http://hz.sxryk.cn/gtvoxsjpkn.html

session_start();  $_SESSION["uid"] = 1;
来源：http://hz.zdqjudy.top/gtyjmamlyc.html

[U66] PHP：设置 Cookie
来源：http://hz.daria6918.cn/gtgdpicxvq.html

setcookie("token", $v, ["httponly" => true, "samesite" => "Lax"]);
来源：http://hz.shanyushiyangtech.top/gtrevveghg.html

[U67] PHP：处理文件上传
来源：http://hz.xinyue.icu/gtaopocjhy.html

$_FILES["file"]["tmp_name"] 与 move_uploaded_file()
来源：http://hz.hysaishi.cn/gtvkokequm.html

[U68] PHP：PDO 连接
来源：http://hz.jiagoushi.top/gtkuzpbtzy.html

$pdo = new PDO("mysql:host=localhost;dbname=app", "root", "");
来源：http://hz.zdqjudy.top/gtlcsveixb.html

[U69] PHP：PDO 预处理
来源：http://hz.smart0.xyz/gtaompbyed.html

$stmt = $pdo->prepare("SELECT * FROM users WHERE id = ?");  $stmt->execute([$id]);
来源：http://hz.zhixingplan.top/gtjfytjuwu.html

[U70] PHP：PDO 事务
来源：http://hz.ivvv.top/gtvvuosgwq.html

$pdo->beginTransaction();  $pdo->commit();  $pdo->rollBack();
来源：http://hz.chenzaomai.com/gtorhlbzwe.html

[U71] PHP：抛出异常
来源：http://hz.redwolf501.top/gttpntvesr.html

throw new RuntimeException("失败", 500);
来源：http://hz.zhijiandao.cn/gtugequocs.html

[U72] PHP：写错误日志
来源：http://hz.c1oappe.top/gtwszamfpw.html

error_log("失败: " . $e->getMessage());
来源：http://hz.yonumen.top/gtiwfhtkep.html

[U73] PHP：读取 ini 配置
来源：http://hz.gotoacloud.top/gtisealwpg.html

parse_ini_file("config.ini", true)
来源：http://hz.daria6918.cn/gtyrgtiusk.html

[U74] PHP：读取环境变量
来源：http://hz.chenjidiqi.icu/gtysupexhp.html

getenv("APP_ENV") ?: "production"
来源：http://hz.zycfv.cn/gtrgtuqobg.html


<!-- 参考信息 -->