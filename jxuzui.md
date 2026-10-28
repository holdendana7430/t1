代发 wailian999

int size() const noexcept { return n_; }
来源：http://hz.gzhubu.top/gtgofhjccy.html

[S53] C++：移动语义
来源：http://hz.xuanzx.com/gtwjlvpzaf.html

std::vector<int> w = std::move(v);
来源：http://hz.andypj.xyz/gtfkyboupc.html

[S54] C++：异常处理
来源：http://hz.snrcjt.cn/gtckfmznla.html

try { throw std::runtime_error("x"); } catch (const std::exception &e) { }
来源：http://hz.fengsongda.top/gtekoijomt.html

[S55] C++：结构化绑定
来源：http://hz.dashuyun.cn/gtnlaitblr.html

auto [a, b] = std::make_pair(1, 2);
来源：http://hz.chenlongwang.top/gtztvfogeb.html

[S56] C++：optional
来源：http://hz.tianlin.xyz/gtppzywamr.html

std::optional<int> o = 5;  if (o) { int v = *o; }
来源：http://hz.xinyue.icu/gtdeiurtyq.html

[S57] C++：编译期常量
来源：http://hz.ivvv.top/gtuyxhukio.html

constexpr int N = 10;
来源：http://hz.ehwqpu.com/gtzxcvjphd.html

[S58] C++：命名空间
来源：http://hz.shanyushiyangtech.top/gtdnuyajdo.html

namespace ns { int f() { return 1; } }
来源：http://hz.aibaodan.cn/gtfqmldpon.html

[S59] C++：静态断言
来源：http://hz.mhx1999.top/gtfptmmgnn.html

static_assert(sizeof(int) == 4, "int 必须 4 字节");
来源：http://hz.sweek.top/gtuxrhufeu.html

[S60] C++：遍历并删除元素
来源：http://hz.gaohongyu789.top/gtrxwrdoyw.html

v.erase(std::remove_if(v.begin(), v.end(), [](int x) { return x < 0; }), v.end());
来源：http://hz.xuetiantiany.cn/gtnmbjybkk.html

================================================================================
来源：http://hz.shanyushiyangtech.top/gtolpgtsda.html

T. 其他语言补充（Kotlin / Swift / Lua / Perl / Scala）
来源：http://hz.fzhhl.top/gtfvrllpth.html

================================================================================
来源：http://hz.aibaodan.cn/gtjvpcawmr.html

[T01] Kotlin：Hello World
来源：http://hz.wangshuangyany.cn/gtlweocztr.html

println("Hello")
来源：http://hz.iojbl.cn/gtisdmianx.html

[T02] Kotlin：变量
来源：http://hz.zycfv.cn/gtosbulium.html

val a = 1;  var b = 2        // val 只读，var 可变
来源：http://hz.yvedp.cn/gtqblrixex.html

[T03] Kotlin：字符串模板
来源：http://hz.redwolf501.top/gtaoogazfj.html

"值: $b"
来源：http://hz.yj20258888.top/gtrhnzgonm.html

[T04] Kotlin：空安全
来源：http://hz.ydjk.org.cn/gtwyjrnkyn.html

val n: String? = null;  n?.length
来源：http://hz.yangfankeji.com/gtsqcfcqze.html

[T05] Kotlin：when 表达式
来源：http://hz.iojbl.cn/gtvdjxdipp.html

val s = when (x) { 1 -> "一" else -> "其他" }   // 多分支时每个分支单独一行
来源：http://hz.zycfv.cn/gteiunahxf.html

[T06] Kotlin：集合映射
来源：http://hz.andypj.xyz/gtjkiiviwg.html

listOf(1, 2, 3).map { it * 2 }
来源：http://hz.gzhubu.top/gtjfxezmye.html

[T07] Kotlin：集合过滤
来源：http://hz.xziqi.cn/gtysmumhib.html

listOf(1, 2, 3).filter { it > 1 }
来源：http://hz.hammf.cn/gtewtskibx.html

[T08] Kotlin：数据类
来源：http://hz.gzhubu.top/gteavvmqqd.html

data class User(val name: String, val age: Int)
来源：http://hz.birdmap.top/gtiivhrzjn.html

[T09] Kotlin：扩展函数
来源：http://hz.jinghuilouyu.cn/gtzowubtfl.html

fun String.exclaim() = this + "!"
来源：http://hz.daxiang520.top/gtevhahtak.html

[T10] Kotlin：默认参数
来源：http://hz.jinghuilouyu.cn/gtidgrcgvu.html

fun greet(name: String = "World") = "Hi $name"
来源：http://hz.yueranfly.top/gtlzdmamgc.html

[T11] Kotlin：协程
来源：http://hz.sxryk.cn/gtaxfremtx.html

GlobalScope.launch { delay(1000); println("done") }
来源：http://hz.yuxming.cn/gtdyqsgvct.html

[T12] Kotlin：解构声明
来源：http://hz.jinghuilouyu.cn/gtectousep.html

val (a, b) = Pair(1, 2)
来源：http://hz.bjfxy.top/gtbntwmrkh.html

[T13] Kotlin：只读 Map
来源：http://hz.jinqigufen.top/gtqxgcqhlf.html

val m = mapOf("a" to 1)
来源：http://hz.ydjk.org.cn/gtfnsrrqly.html

[T14] Kotlin：循环
来源：http://hz.gotoacloud.top/gtwrpqmyil.html

for (i in 1..10) println(i)
来源：http://hz.yueranfly.top/gtsztcsmdj.html

[T15] Kotlin：接口
来源：http://hz.yuxming.cn/gtkpwpfbwa.html

interface Shape { fun area(): Double }
来源：http://hz.jqgufenzy.top/gtcfpporxw.html

[T16] Swift：Hello World
来源：http://hz.xylfe.cn/gtygzpcryg.html

print("Hello")
来源：http://hz.xylfe.cn/gtmbsnclpb.html

[T17] Swift：变量与常量
来源：http://hz.yj202588.top/gtuakxjpla.html

var a = 1;  let b = 2
来源：http://hz.jinqigfzy.top/gtiivpwsax.html

[T18] Swift：字符串插值
来源：http://hz.ydzc1.top/gtvyuxlyro.html

"值: \(b)"
来源：http://hz.wangdashe.top/gtxvxgemic.html

[T19] Swift：可选绑定
来源：http://hz.quarkkingdee.top/gtoodiqxdm.html

if let n = opt { print(n) }
来源：http://hz.tian-w.cn/gtbmzmbpmb.html

[T20] Swift：数组操作
来源：http://hz.yuxming.cn/gtxhkbahlg.html

var a = [1, 2, 3];  a.append(4)
来源：http://hz.wangshuangyany.cn/gtgvltrpmg.html

[T21] Swift：遍历
来源：http://hz.sysykeji.top/gtduviickd.html

for x in a { print(x) }
来源：http://hz.hnqzz.top/gtjruqextn.html

[T22] Swift：字典
来源：http://hz.tian-w.cn/gtzhyagrqi.html

var d = ["a": 1];  d["b"] = 2
来源：http://hz.zdqjudy.top/gtewjtpspn.html

[T23] Swift：函数
来源：http://hz.c1oappe.top/gtlcrrfnnl.html

func add(_ a: Int, _ b: Int) -> Int { a + b }
来源：http://hz.ydjk.org.cn/gtdmfnvquc.html

[T24] Swift：闭包
来源：http://hz.feifeiyinyue.top/gtfnstijoj.html

let f = { (x: Int) -> Int in x * 2 }
来源：http://hz.sysykeji.top/gtykjhurmy.html

[T25] Swift：结构体
来源：http://hz.jinqigfzy.top/gtejaewqcf.html

struct P { var x: Int }
来源：http://hz.xinyue.icu/gtfenebkje.html

[T26] Swift：类与重写
来源：http://hz.haohaochexian.top/gtoepzgjns.html

class A: Base { override func f() {} }
来源：http://hz.sweek.top/gtbrydkjtc.html

[T27] Swift：错误处理
来源：http://hz.gzhubu.top/gtvcwohqeu.html

do { try f() } catch { print(error) }
来源：http://hz.jinqigfzy.top/gtztnctinq.html

[T28] Swift：枚举
来源：http://hz.zhongyouzk.top/gtgjurtnnk.html

enum Color { case red, green }
来源：http://hz.zhixingplan.top/gteoybjozz.html

[T29] Swift：guard 提前返回
来源：http://hz.shuidangran.top/gtqmhrwrko.html

guard let x = opt else { return }
来源：http://hz.daria6918.cn/gtckqaaije.html

[T30] Swift：协议
来源：http://hz.yangfankeji.com/gtixasbiyo.html

protocol Shape { func area() -> Double }
来源：http://hz.wangdashe.top/gtuwosxbas.html

[T31] Lua：Hello World
来源：http://hz.xylfe.cn/gtcumyrtud.html

print("Hello")
来源：http://hz.ydzc1.top/gtejchmnlc.html

[T32] Lua：局部变量
来源：http://hz.svipenyu.cn/gtztifyfya.html

local a = 1
来源：http://hz.jlsjyb.cn/gtiqhfjeqs.html

[T33] Lua：表（数组）
来源：http://hz.shuidangran.top/gtzqgvkxll.html

local t = {1, 2, 3};  t[4] = 4
来源：http://hz.xingfuxueyuan.xyz/gtuoujhner.html

[T34] Lua：遍历表
来源：http://hz.chenjidiqi.icu/gtabumbmuy.html

for i, v in ipairs(t) do print(i, v) end
来源：http://hz.yueranfly.top/gtyptmbgkg.html

[T35] Lua：字典表
来源：http://hz.xziqi.cn/gthvwpitjg.html

local d = { a = 1 };  d.b = 2
来源：http://hz.sufxvd.cn/gtnowqflti.html

[T36] Lua：函数
来源：http://hz.cqqwz.cn/gtpyivczux.html

function add(a, b) return a + b end
来源：http://hz.yj20258888.top/gtggdzebcb.html

[T37] Lua：字符串拼接
来源：http://hz.smart0.xyz/gtjlfqtezd.html

"a" .. "b"
来源：http://hz.guowangkeji.top/gtqwhtoado.html

[T38] Lua：条件
来源：http://hz.shuidangran.top/gtvmmkwnqz.html

if x > 0 then print("正") end
来源：http://hz.sxryk.cn/gtbnfdgctj.html

[T39] Lua：模式匹配
来源：http://hz.havefunace.top/gtkpqcichg.html

string.find(s, "%d+")
来源：http://hz.ivvv.top/gtwmmpcjgz.html

[T40] Lua：元表
来源：http://hz.yj20258.top/gtyohxsrze.html

setmetatable({}, { __index = base })
来源：http://hz.shzxlz.cn/gtkxkhikme.html

[T41] Perl：Hello World
来源：http://hz.chenjidiqi.icu/gtzesccsjn.html

print "Hello\n";
来源：http://hz.sxryk.cn/gtxqescrzm.html

[T42] Perl：变量类型
来源：http://hz.zhaomingkeji.xyz/gtjxhqumov.html

my $a = 1;  my @arr = (1, 2, 3);  my %h = (a => 1);
来源：http://hz.xylfe.cn/gtztskzgeo.html

[T43] Perl：字符串插值
来源：http://hz.9152youxi.cn/gtdpgebozr.html

"值: $a"
来源：http://hz.bjfxy.top/gtotipqzaz.html

[T44] Perl：条件
来源：http://hz.hongshengwenyu.top/gtknlnjoop.html

if ($a > 0) { print "正"; }
来源：http://hz.smart0.xyz/gtsxerprru.html

[T45] Perl：数组遍历
来源：http://hz.zhaomingkeji.xyz/gtvqixvqdc.html

for my $x (@arr) { print $x; }
来源：http://hz.xylfe.cn/gtnckxrtzd.html

[T46] Perl：哈希操作
来源：http://hz.zhiwuduotai.top/gtdywlnyla.html

$h{b} = 2;  for my $k (keys %h) { print "$k=$h{$k}"; }
来源：http://hz.hysaishi.cn/gtwyrqdmrr.html

[T47] Perl：正则捕获
来源：http://hz.zhongyouzk.top/gtqncjjyny.html

if ($s =~ /(\d+)/) { print $1; }
来源：http://hz.ybcxt.top/gtbutcnlem.html

[T48] Perl：正则替换
来源：http://hz.zhengqikj.top/gtfhsrysbn.html

$s =~ s/old/new/g;
来源：http://hz.jinqigfzy.top/gtedrjxtxi.html

[T49] Perl：函数
来源：http://hz.hysaishi.cn/gtihiafdqv.html

sub add { my ($a, $b) = @_; return $a + $b; }
来源：http://hz.iojbl.cn/gttplwptel.html

[T50] Perl：逐行读文件
来源：http://hz.gotoacloud.top/gthtpxtihx.html

open my $fh, "<", "a.txt" or die $!;
来源：http://hz.gaohongyu789.top/gtupaewjzp.html

while (my $line = <$fh>) { print $line; }
来源：http://hz.andypj.xyz/gtqrssaqnf.html

[T51] Scala：Hello World
来源：http://hz.gzhubu.top/gtxneozosu.html

println("Hello")
来源：http://hz.hongshengwenyu.top/gtbaunqxmf.html

[T52] Scala：变量
来源：http://hz.haohaochexian.top/gtmhijjkpm.html

val a = 1;  var b = 2
来源：http://hz.pengpengdd.cyou/gtcnnlvtzy.html

[T53] Scala：字符串插值
来源：http://hz.ppjwa.cn/gtmqkilqoe.html

s"值: $b"
来源：http://hz.tianlin.xyz/gtmvxouysk.html

[T54] Scala：集合映射
来源：http://hz.ydzc1.top/gtpegkfzdp.html

List(1, 2, 3).map(_ * 2)
来源：http://hz.jinghuilouyu.cn/gtufxlfram.html

[T55] Scala：集合过滤
来源：http://hz.yj202588.top/gtdnorcdlc.html

List(1, 2, 3).filter(_ > 1)
来源：http://hz.hywenlv.cn/gttrjybhyl.html

[T56] Scala：样例类
来源：http://hz.c1oappe.top/gtmxwpfplb.html

case class User(name: String, age: Int)
来源：http://hz.jinghuilouyu.cn/gtwzvmdhdw.html

[T57] Scala：模式匹配
来源：http://hz.ppjwa.cn/gtyvhmkgff.html

x match { case 1 => "一"; case _ => "其他" }
来源：http://hz.redwolf501.top/gtmjwvsssd.html

[T58] Scala：函数定义
来源：http://hz.wangshuangyany.cn/gtvfwomgdw.html

def add(a: Int, b: Int): Int = a + b
来源：http://hz.jqgufenzy.top/gtepuxlhxd.html

[T59] Scala：循环
来源：http://hz.xylfe.cn/gtenmndpqb.html

for (i <- 1 to 10) println(i)
来源：http://hz.mhx1999.top/gtlysgccuc.html

[T60] Scala：折叠
来源：http://hz.wangdashe.top/gtzpmpdwex.html

List(1, 2, 3).foldLeft(0)(_ + _)
来源：http://hz.ivvv.top/gtzqlvhqjy.html

================================================================================
来源：http://hz.sxryk.cn/gtzijhpodt.html

U. 高频实用片段（Python / PHP / JavaScript 各 40 条）
来源：http://hz.sufxvd.cn/gtoxgygkfj.html

================================================================================
来源：http://hz.sweek.top/gtawdzmcng.html

[U01] Py：创建虚拟环境
来源：http://hz.xinyue.icu/gtmavqkaqx.html

python -m venv .venv && source .venv/bin/activate
来源：http://hz.yuanzhike.top/gtdvcpsiiu.html

[U02] Py：导出 / 安装依赖
来源：http://hz.jyoumei.cn/gtwkxgfvax.html

pip freeze > requirements.txt;  pip install -r requirements.txt
来源：http://hz.aizwys.cn/gtgqojfgyh.html

[U03] Py：加载 .env 配置
来源：http://hz.daria6918.cn/gtdtkldyue.html

from dotenv import load_dotenv; load_dotenv()
来源：http://hz.gotoacloud.top/gtutelddwl.html

[U04] Py：变量调试打印
来源：http://hz.ydzc1.top/gtkzcnoycx.html

print(f"{x=}")            # 输出 x=值，Python 3.8+
来源：http://hz.9152youxi.cn/gtjkjafwrr.html

[U05] Py：列表去重且保序
来源：http://hz.aibaodan.cn/gtnklbozgc.html

list(dict.fromkeys(arr))
来源：http://hz.shanyushiyangtech.top/gtuiulzcks.html

[U06] Py：合并两个字典
来源：http://hz.gzhubu.top/gtnvvxuiet.html

{**a, **b}
来源：http://hz.xinyue.icu/gtvslxegkz.html

[U07] Py：反转字典键值
来源：http://hz.cheryme.top/gtullasgik.html

{v: k for k, v in d.items()}
来源：http://hz.sxryk.cn/gtnjzuzyfi.html

[U08] Py：展平二维列表
来源：http://hz.zhoulong.xyz/gtqrmbdmfx.html

[y for x in nested for y in x]
来源：http://hz.jianghu66.top/gtkenvwbqg.html

[U09] Py：字典取最大值的键
来源：http://hz.hnqzz.top/gtxplrmyoi.html

max(d, key=d.get)
来源：http://hz.ydjk.org.cn/gtmhowvggf.html

[U10] Py：按值排序字典
来源：http://hz.zhixingplan.top/gttbhbokkp.html

dict(sorted(d.items(), key=lambda kv: kv[1]))
来源：http://hz.jinqigufen.top/gtokwcdffo.html

[U11] Py：生成器表达式
来源：http://hz.yj20258.top/gtvvlsolvz.html

(x * 2 for x in arr)
来源：http://hz.gaohongyu789.top/gthkyykknl.html

[U12] Py：取出现最多的 3 个元素
来源：http://hz.jinqigfzy.top/gtutrevbrf.html

Counter(arr).most_common(3)
来源：http://hz.gzhubu.top/gtwgjnjjcp.html

[U13] Py：固定长度队列
来源：http://hz.bjfxy.top/gtguzukrfp.html

deque(maxlen=10)
来源：http://hz.havefunace.top/gtdhsxnatc.html

[U14] Py：分组收集到列表
来源：http://hz.hammf.cn/gtnnvcnbcd.html

defaultdict(list)
来源：http://hz.hnxiangtu.top/gtqepmpbdm.html

[U15] Py：高精度计时
来源：http://hz.mhx1999.top/gtdevozwnb.html

t = time.perf_counter()
来源：http://hz.wangdashe.top/gtxexehgws.html

[U16] Py：命令行参数解析
来源：http://hz.xylfe.cn/gtbprqoywo.html

ap = argparse.ArgumentParser();  ap.add_argument("--name");  args = ap.parse_args()
来源：http://hz.yangfankeji.com/gtjtqaqpda.html

[U17] Py：初始化日志
来源：http://hz.wangshuangyany.cn/gtkpugwnyh.html

logging.basicConfig(level=logging.INFO)
来源：http://hz.dashuyun.cn/gtzugtyzhj.html

[U18] Py：预编译正则
来源：http://hz.guowangkeji.top/gtlzynozgo.html

pat = re.compile(r"\d+")
来源：http://hz.nwbrower.top/gtsanmmaou.html

[U19] Py：正则替换带回调
来源：http://hz.hammf.cn/gtdpgokyel.html

re.sub(r"\d+", lambda m: str(int(m.group()) * 2), s)
来源：http://hz.dashuyun.cn/gtarlbeyhz.html

[U20] Py：缓存函数结果
来源：http://hz.havefunace.top/gtmrkkqmkc.html

@functools.lru_cache(maxsize=None)
来源：http://hz.zycfv.cn/gtbvecmjvc.html

[U21] Py：自定义上下文管理器
来源：http://hz.shzxlz.cn/gthltbalvr.html

@contextlib.contextmanager
来源：http://hz.jyoumei.cn/gtvljvruyr.html

[U22] Py：矩阵转置
来源：http://hz.zdqjudy.top/gtyfzymykc.html

list(zip(*m))
来源：http://hz.cucudq.cn/gtedvgfkut.html

[U23] Py：分块读取大文件
来源：http://hz.mhx1999.top/gtasxrqdzt.html

for chunk in iter(lambda: f.read(8192), b""):
来源：http://hz.feifeiyinyue.top/gtxnzsbhyk.html

[U24] Py：路径操作
来源：http://hz.yueranfly.top/gtpykhdfuj.html

Path("a/b.txt").parent.mkdir(parents=True, exist_ok=True)
来源：http://hz.zhaomingkeji.xyz/gtzouvcoiz.html

[U25] Py：CSV 按字典读
来源：http://hz.zhengqikj.top/gtfvuztqti.html

csv.DictReader(f)
来源：http://hz.shangyingyoupin.top/gttzpxpfuh.html

[U26] Py：并发下载
来源：http://hz.kuanghao11.cn/gtuzlinxus.html

ThreadPoolExecutor(max_workers=8).map(fetch, urls)
来源：http://hz.pengpengdd.cyou/gtquooajhm.html

[U27] Py：异步 HTTP
来源：http://hz.0kj1m.cn/gtglizhbbx.html

aiohttp.ClientSession() 配合 async with
来源：http://hz.cdnleiting.top/gtryezihoo.html

[U28] Py：类型别名
来源：http://hz.jqgufenzy.top/gtmallyrgh.html

UserId = int
来源：http://hz.hysaishi.cn/gtfbprrxdd.html

[U29] Py：属性校验
来源：http://hz.wangshuangyany.cn/gtrtgvaqpi.html

@property 与 @x.setter 配合
来源：http://hz.meibo888.top/gtnchdoptj.html

[U30] Py：数据类
来源：http://hz.gogol.net.cn/gtgqkwvrvx.html

@dataclass(slots=True)
来源：http://hz.ywan-chungtsiang.top/gttlmoouqb.html

[U31] Py：单测
来源：http://hz.hfpthk.cn/gtpmtaydkq.html

python -m pytest -q
来源：http://hz.cashguo.top/gtuqstfuui.html

[U32] Py：代码格式化
来源：http://hz.zycfv.cn/gtkdtaryjp.html

ruff format . && ruff check --fix .
来源：http://hz.jyoumei.cn/gtsdocxjzn.html

[U33] Py：打包发布
来源：http://hz.daxiang520.top/gtowhgkgea.html

python -m build  （依赖 pyproject.toml）
来源：http://hz.zhengqikj.top/gtcqdalfvy.html

[U34] Py：判断编码
来源：http://hz.hywenlv.cn/gtjvbgufjq.html

chardet.detect(raw)
来源：http://hz.meibo888.top/gtsxqrzvln.html

[U35] Py：发送邮件
来源：http://hz.chenzaomai.com/gtjwgxaxcj.html

smtplib.SMTP_SSL(...).send_message(msg)
来源：http://hz.jlsjyb.cn/gtvzfnzbnv.html

[U36] Py：定时任务
来源：http://hz.yongpay.top/gtfpfhxgpp.html

schedule.every(10).minutes.do(job)
来源：http://hz.hongshengwenyu.top/gtwblghffe.html

[U37] Py：读写 Excel
来源：http://hz.tianlin.xyz/gtgqphxqcb.html

pandas.read_excel / DataFrame.to_excel
来源：http://hz.redwolf501.top/gtyrdmaimh.html

[U38] Py：获取脚本所在目录
来源：http://hz.dashuyun.cn/gtmubizsve.html

Path(__file__).resolve().parent
来源：http://hz.zhixingplan.top/gtlrfticvl.html

[U39] Py：判断是否在交互环境
来源：http://hz.daria6918.cn/gtjdktszdi.html

sys.stdout.isatty()
来源：http://hz.meibo888.top/gtsdnaviym.html

[U40] Py：打印到标准错误
来源：http://hz.nanxuanxn.top/gtyszosail.html

print("err", file=sys.stderr)
来源：http://hz.tanke756.top/gtajveeqwo.html

[U41] PHP：初始化 Composer 项目
来源：http://hz.xuetiantiany.cn/gtxrwfslay.html

composer init;  composer require guzzlehttp/guzzle
来源：http://hz.zycfv.cn/gtpuhqurwg.html

[U42] PHP：PSR-4 自动加载
来源：http://hz.feifeiyinyue.top/gtnmnkggci.html

"autoload": { "psr-4": { "App\\": "src/" } }
来源：http://hz.nanxuanxn.top/gtbkjjbfdc.html

[U43] PHP：声明命名空间
来源：http://hz.c1oappe.top/gtqepwfigr.html

namespace App\Http;
来源：http://hz.tian-w.cn/gtzzpgxrut.html

[U44] PHP：开启严格类型
来源：http://hz.dashuyun.cn/gtyuhkcktr.html

declare(strict_types=1);
来源：http://hz.havefunace.top/gtlkptzozg.html

[U45] PHP：类型声明与返回类型
来源：http://hz.zdqjudy.top/gtnsvqaovn.html

function add(int $a, int $b): int { return $a + $b; }
来源：http://hz.zhengqikj.top/gtzdsfrgib.html

[U46] PHP：可空类型
来源：http://hz.yuxming.cn/gtbbbchszu.html

?string $name = null
来源：http://hz.shuidangran.top/gtepkvmxez.html

[U47] PHP：联合类型
来源：http://hz.pycfn.com/gtqdwmwpqm.html

int|string $id
来源：http://hz.mhx1999.top/gtuttulzek.html

[U48] PHP：纯枚举
来源：http://hz.sysykeji.top/gtaygrbajn.html

enum Status: string { case Active = "active"; case Off = "off"; }
来源：http://hz.meibo888.top/gtsopldxpw.html

[U49] PHP：只读属性
来源：http://hz.chenjidiqi.icu/gtcxhtklwp.html

public readonly string $name
来源：http://hz.hysaishi.cn/gtpcgunojg.html

[U50] PHP：构造器属性提升
来源：http://hz.c1oappe.top/gtbjktesrj.html

public function __construct(private int $id) {}
来源：http://hz.vqdsnc.cn/gtleglgedz.html

[U51] PHP：数组解构
来源：http://hz.shuidangran.top/gtsairnuxf.html

[$a, $b] = $arr;
来源：http://hz.hnqzz.top/gtztfggquo.html

[U52] PHP：箭头函数
来源：http://hz.aizwys.cn/gtpgaedhtf.html

$double = fn($x) => $x * 2;
来源：http://hz.0kj1m.cn/gtiuwrdywb.html

[U53] PHP：空合并运算符
来源：http://hz.shzxlz.cn/gtquezvhlc.html

$v = $a ?? $b ?? "default";
来源：http://hz.smart0.xyz/gtzqghunif.html

[U54] PHP：空安全调用
来源：http://hz.zhijiandao.cn/gtgoemzumy.html

$obj?->method()
来源：http://hz.ywan-chungtsiang.top/gtuvcvnwne.html

[U55] PHP：match 表达式
来源：http://hz.yj20258.top/gtvwgsmrsj.html

$s = match($x) { 1 => "一", default => "其他" };
来源：http://hz.ivvv.top/gthnjwbmlq.html

[U56] PHP：命名参数
来源：http://hz.feifeiyinyue.top/gtkiahokma.html

f(a: 1, b: 2)
来源：http://hz.ywan-chungtsiang.top/gtlslzetyx.html

[U57] PHP：字符串插值
来源：http://hz.fzhhl.top/gteyqpgmty.html

"值: {$a}"
来源：http://hz.xuetiantiany.cn/gtcluhnwdq.html

[U58] PHP：数组三件套
来源：http://hz.316326.xyz/gttzrrhnxm.html

array_map($f, $a);  array_filter($a, $f);  array_reduce($a, $f, 0);
来源：http://hz.zhaomingkeji.xyz/gtrlpjicdt.html

[U59] PHP：自定义排序
来源：http://hz.zycfv.cn/gtagxuewjc.html

usort($arr, fn($a, $b) => $a["age"] <=> $b["age"]);
来源：http://hz.sysykeji.top/gtaeowedwe.html

[U60] PHP：JSON 编解码
来源：http://hz.xuanzx.com/gthswqvniq.html

json_encode($d, JSON_UNESCAPED_UNICODE);  json_decode($s, true);
来源：http://hz.yj20258.top/gtqbyeovoa.html

[U61] PHP：正则
来源：http://hz.yj20258888.top/gteflxrvkk.html

preg_match('/(\d+)/', $s, $m);  preg_replace('/\d+/', '#', $s);
来源：http://hz.chenjidiqi.icu/gtjgxudprc.html

[U62] PHP：日期对象
来源：http://hz.fengsongda.top/gtpzqkqmsp.html

(new DateTimeImmutable())->format("Y-m-d");
来源：http://hz.cucudq.cn/gtobwvfcqo.html

[U63] PHP：文件读写
来源：http://hz.gaohongyu789.top/gtboacfjnt.html

file_get_contents($f);  file_put_contents($f, $data);
来源：http://hz.bjfxy.top/gtvjhdkoss.html

[U64] PHP：目录遍历
来源：http://hz.nanxinkj.top/gtzqqkuhpe.html

glob("dir/*.php");  scandir("dir");
来源：http://hz.ppjwa.cn/gtpxcuubui.html

[U65] PHP：会话
来源：http://hz.shuidangran.top/gtqitrjvbe.html

session_start();  $_SESSION["uid"] = 1;
来源：http://hz.yuxming.cn/gtjzehqelq.html

[U66] PHP：设置 Cookie
来源：http://hz.zhoulong.xyz/gtiluvmaub.html

setcookie("token", $v, ["httponly" => true, "samesite" => "Lax"]);
来源：http://hz.c1oappe.top/gtllibrqac.html

[U67] PHP：处理文件上传
来源：http://hz.birdmap.top/gtpoagkiwg.html

$_FILES["file"]["tmp_name"] 与 move_uploaded_file()
来源：http://hz.fengsongda.top/gtoougpmur.html

[U68] PHP：PDO 连接
来源：http://hz.yonumen.top/gtyefgsbzx.html

$pdo = new PDO("mysql:host=localhost;dbname=app", "root", "");
来源：http://hz.cucudq.cn/gtswudaowb.html

[U69] PHP：PDO 预处理
来源：http://hz.ydjk.org.cn/gtfkjbynrs.html

$stmt = $pdo->prepare("SELECT * FROM users WHERE id = ?");  $stmt->execute([$id]);
来源：http://hz.gzhubu.top/gtdttqjwxk.html

[U70] PHP：PDO 事务
来源：http://hz.gogol.net.cn/gtpaetmywm.html

$pdo->beginTransaction();  $pdo->commit();  $pdo->rollBack();
来源：http://hz.wangdashe.top/gtsakhqpoa.html

[U71] PHP：抛出异常
来源：http://hz.pycfn.com/gtfmkqjqeq.html

throw new RuntimeException("失败", 500);
来源：http://hz.haohaochexian.top/gtdegxrwpm.html

[U72] PHP：写错误日志
来源：http://hz.guannengcc.top/gtsmmcqweq.html

error_log("失败: " . $e->getMessage());
来源：http://hz.pycfn.com/gtyzdirnps.html

[U73] PHP：读取 ini 配置
来源：http://hz.52xcode.cn/gtdkljoarj.html

parse_ini_file("config.ini", true)
来源：http://hz.redwolf501.top/gtaxjafzsr.html

[U74] PHP：读取环境变量
来源：http://hz.pengpengdd.cyou/gthakfawyo.html

getenv("APP_ENV") ?: "production"
来源：http://hz.wangdashe.top/gtqgoimklu.html

[U75] PHP：依赖注入
来源：http://hz.cucudq.cn/gtmcsgmkzz.html

composer require psr/container
来源：http://hz.nanxinkj.top/gtzwljhawm.html

[U76] PHP：简单路由
来源：http://hz.wangdashe.top/gtozyqrlrb.html

$path = parse_url($_SERVER["REQUEST_URI"], PHP_URL_PATH);
来源：http://hz.hfpthk.cn/gthaewvyon.html

[U77] PHP：模板渲染
来源：http://hz.jiagoushi.top/gtevjkxzkj.html

composer require twig/twig
来源：http://hz.redwolf501.top/gtnmnmfsel.html

[U78] PHP：单元测试
来源：http://hz.yvedp.cn/gtdrddqhhq.html

composer require --dev phpunit/phpunit
来源：http://hz.jianghu66.top/gtdepvqlig.html


<!-- 参考信息 -->