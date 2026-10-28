代发 wailian999

try { throw std::runtime_error("x"); } catch (const std::exception &e) { }
来源：http://hz.gzhubu.top/gtmdqvbqeq.html

[S55] C++：结构化绑定
来源：http://hz.316326.xyz/gtuqmlxtke.html

auto [a, b] = std::make_pair(1, 2);
来源：http://hz.jqgufenzy.top/gtgdpmwzqq.html

[S56] C++：optional
来源：http://hz.gogol.net.cn/gtclaesvwl.html

std::optional<int> o = 5;  if (o) { int v = *o; }
来源：http://hz.zhoulong.xyz/gtrpkegilj.html

[S57] C++：编译期常量
来源：http://hz.hnqzz.top/gtjajmonxm.html

constexpr int N = 10;
来源：http://hz.316326.xyz/gttaszqosk.html

[S58] C++：命名空间
来源：http://hz.zhijiandao.cn/gtzopnzrnv.html

namespace ns { int f() { return 1; } }
来源：http://hz.jinqigfzy.top/gtvdwkdvqp.html

[S59] C++：静态断言
来源：http://hz.shzxlz.cn/gtbwohvtue.html

static_assert(sizeof(int) == 4, "int 必须 4 字节");
来源：http://hz.hywenlv.cn/gtmrusdoxr.html

[S60] C++：遍历并删除元素
来源：http://hz.cheryme.top/gtvolndxbj.html

v.erase(std::remove_if(v.begin(), v.end(), [](int x) { return x < 0; }), v.end());
来源：http://hz.quarkkingdee.top/gtzamdvhjm.html

================================================================================
来源：http://hz.pengpengdd.cyou/gtljnfvemx.html

T. 其他语言补充（Kotlin / Swift / Lua / Perl / Scala）
来源：http://hz.yonumen.top/gtgztgidzp.html

================================================================================
来源：http://hz.iojbl.cn/gtvfezsexz.html

[T01] Kotlin：Hello World
来源：http://hz.ydjk.org.cn/gtzscjofpi.html

println("Hello")
来源：http://hz.shanyushiyangtech.top/gtuusvxijf.html

[T02] Kotlin：变量
来源：http://hz.snrcjt.cn/gtconxjwfz.html

val a = 1;  var b = 2        // val 只读，var 可变
来源：http://hz.bjfxy.top/gtghmslhrp.html

[T03] Kotlin：字符串模板
来源：http://hz.yonumen.top/gtpsukvqwl.html

"值: $b"
来源：http://hz.yj202588.top/gtlndxcxtj.html

[T04] Kotlin：空安全
来源：http://hz.guowangkeji.top/gtirvowjzo.html

val n: String? = null;  n?.length
来源：http://hz.ydzc1.top/gtezhwgosv.html

[T05] Kotlin：when 表达式
来源：http://hz.wangdashe.top/gtrjduylht.html

val s = when (x) { 1 -> "一" else -> "其他" }   // 多分支时每个分支单独一行
来源：http://hz.gogol.net.cn/gtpbflomtq.html

[T06] Kotlin：集合映射
来源：http://hz.jinghuilouyu.cn/gtonjflgqj.html

listOf(1, 2, 3).map { it * 2 }
来源：http://hz.9152youxi.cn/gtwbzqrfux.html

[T07] Kotlin：集合过滤
来源：http://hz.jqgufenzy.top/gtcxrjpdxn.html

listOf(1, 2, 3).filter { it > 1 }
来源：http://hz.9152youxi.cn/gtbwzsnhfa.html

[T08] Kotlin：数据类
来源：http://hz.kuanghao11.cn/gtvyaaflas.html

data class User(val name: String, val age: Int)
来源：http://hz.jinqigfzy.top/gtsyzjgmtw.html

[T09] Kotlin：扩展函数
来源：http://hz.zycfv.cn/gtdcymveew.html

fun String.exclaim() = this + "!"
来源：http://hz.yvedp.cn/gtwohqpzug.html

[T10] Kotlin：默认参数
来源：http://hz.dashuyun.cn/gtykwymass.html

fun greet(name: String = "World") = "Hi $name"
来源：http://hz.shanyushiyangkeji.top/gtvvrmapze.html

[T11] Kotlin：协程
来源：http://hz.xuetiantiany.cn/gtzdxhyqht.html

GlobalScope.launch { delay(1000); println("done") }
来源：http://hz.chenjidiqi.icu/gttduzuzki.html

[T12] Kotlin：解构声明
来源：http://hz.ywan-chungtsiang.top/gtnptbfhvv.html

val (a, b) = Pair(1, 2)
来源：http://hz.gogol.net.cn/gtmabpzqkm.html

[T13] Kotlin：只读 Map
来源：http://hz.wangdashe.top/gtaqljrmuu.html

val m = mapOf("a" to 1)
来源：http://hz.316326.xyz/gtatzvytni.html

[T14] Kotlin：循环
来源：http://hz.fengsongda.top/gtnffymkhv.html

for (i in 1..10) println(i)
来源：http://hz.bjfxy.top/gtnwjkzhsc.html

[T15] Kotlin：接口
来源：http://hz.havefunace.top/gtpptenkya.html

interface Shape { fun area(): Double }
来源：http://hz.jqgfzy.top/gtgwncvjfy.html

[T16] Swift：Hello World
来源：http://hz.xuetiantiany.cn/gtdrmhhyrt.html

print("Hello")
来源：http://hz.meibo888.top/gtcypdmuoc.html

[T17] Swift：变量与常量
来源：http://hz.nanxinkj.top/gtvabvevnn.html

var a = 1;  let b = 2
来源：http://hz.meibo888.top/gtzxkehlaz.html

[T18] Swift：字符串插值
来源：http://hz.ydjk.org.cn/gtvzvhofgb.html

"值: \(b)"
来源：http://hz.ybcxt.top/gthbopsuoa.html

[T19] Swift：可选绑定
来源：http://hz.zhiwuduotai.top/gtcuqilzsn.html

if let n = opt { print(n) }
来源：http://hz.chenjidiqi.icu/gtpgmwgvry.html

[T20] Swift：数组操作
来源：http://hz.yuanzhike.top/gtykbhoxit.html

var a = [1, 2, 3];  a.append(4)
来源：http://hz.yvedp.cn/gtsolngvto.html

[T21] Swift：遍历
来源：http://hz.redwolf501.top/gtuddyqklj.html

for x in a { print(x) }
来源：http://hz.sweek.top/gtirmyoiml.html

[T22] Swift：字典
来源：http://hz.chenzaomai.com/gtbjhdcdch.html

var d = ["a": 1];  d["b"] = 2
来源：http://hz.zhongyouzk.top/gtvpcwjhfh.html

[T23] Swift：函数
来源：http://hz.haohaochexian.top/gtprrbdaql.html

func add(_ a: Int, _ b: Int) -> Int { a + b }
来源：http://hz.hywenlv.cn/gtqgkssali.html

[T24] Swift：闭包
来源：http://hz.jinqigufen.top/gtcmiplvlt.html

let f = { (x: Int) -> Int in x * 2 }
来源：http://hz.guowangkeji.top/gtxvfskioh.html

[T25] Swift：结构体
来源：http://hz.zhixingplan.top/gtaenwsgoz.html

struct P { var x: Int }
来源：http://hz.ivvv.top/gtzsvupqxj.html

[T26] Swift：类与重写
来源：http://hz.ydzc1.top/gtkkbjonfe.html

class A: Base { override func f() {} }
来源：http://hz.jinqigfzy.top/gtpbqopato.html

[T27] Swift：错误处理
来源：http://hz.cheryme.top/gtqjnssfmu.html

do { try f() } catch { print(error) }
来源：http://hz.cheryme.top/gtnouzjykl.html

[T28] Swift：枚举
来源：http://hz.316326.xyz/gthuwinxjh.html

enum Color { case red, green }
来源：http://hz.daxiang520.top/gtkevmwvtn.html

[T29] Swift：guard 提前返回
来源：http://hz.yvedp.cn/gtilcxzzda.html

guard let x = opt else { return }
来源：http://hz.hysaishi.cn/gtvsfjwdzc.html

[T30] Swift：协议
来源：http://hz.zdqjudy.top/gtcjqcmsef.html

protocol Shape { func area() -> Double }
来源：http://hz.wangdashe.top/gtrgpbncrg.html

[T31] Lua：Hello World
来源：http://hz.mhx1999.top/gtydifsoos.html

print("Hello")
来源：http://hz.316326.xyz/gtkymodtah.html

[T32] Lua：局部变量
来源：http://hz.hongshengwenyu.top/gtaqvkehos.html

local a = 1
来源：http://hz.nanxinkj.top/gtsnjplakq.html

[T33] Lua：表（数组）
来源：http://hz.sweek.top/gtbnhgndnm.html

local t = {1, 2, 3};  t[4] = 4
来源：http://hz.sysykeji.top/gtixelgrtu.html

[T34] Lua：遍历表
来源：http://hz.cqqwz.cn/gtgytgsyoo.html

for i, v in ipairs(t) do print(i, v) end
来源：http://hz.jyoumei.cn/gtexjcnrfc.html

[T35] Lua：字典表
来源：http://hz.yj20258888.top/gtsgryofgb.html

local d = { a = 1 };  d.b = 2
来源：http://hz.aibaodan.cn/gtvsuieona.html

[T36] Lua：函数
来源：http://hz.sxryk.cn/gtzkrvkmsj.html

function add(a, b) return a + b end
来源：http://hz.birdmap.top/gtmcbpdanw.html

[T37] Lua：字符串拼接
来源：http://hz.chenlongwang.top/gtgarrvqvm.html

"a" .. "b"
来源：http://hz.jinyuanbaomall.cn/gtjpsxsmay.html

[T38] Lua：条件
来源：http://hz.ydjk.org.cn/gtcofajtas.html

if x > 0 then print("正") end
来源：http://hz.52xcode.cn/gtryelbkdz.html

[T39] Lua：模式匹配
来源：http://hz.jyoumei.cn/gtiunojrqu.html

string.find(s, "%d+")
来源：http://hz.yongpay.top/gttupdwsef.html

[T40] Lua：元表
来源：http://hz.ybcxt.top/gtsbqzxaif.html

setmetatable({}, { __index = base })
来源：http://hz.jianghu66.top/gtogtsspxy.html

[T41] Perl：Hello World
来源：http://hz.haohaochexian.top/gtahdlooqx.html

print "Hello\n";
来源：http://hz.iojbl.cn/gtniannfvu.html

[T42] Perl：变量类型
来源：http://hz.daxiang520.top/gtwpbtncqt.html

my $a = 1;  my @arr = (1, 2, 3);  my %h = (a => 1);
来源：http://hz.aizwys.cn/gtwphtzubj.html

[T43] Perl：字符串插值
来源：http://hz.wangshuangyany.cn/gtdvkpddjb.html

"值: $a"
来源：http://hz.zhijiandao.cn/gtjsoijnfw.html

[T44] Perl：条件
来源：http://hz.smart0.xyz/gtxenbddzl.html

if ($a > 0) { print "正"; }
来源：http://hz.xziqi.cn/gtshjizbth.html

[T45] Perl：数组遍历
来源：http://hz.0kj1m.cn/gtvcaukrak.html

for my $x (@arr) { print $x; }
来源：http://hz.shzxlz.cn/gtffstwhwy.html

[T46] Perl：哈希操作
来源：http://hz.yangfankeji.com/gtidhdhiua.html

$h{b} = 2;  for my $k (keys %h) { print "$k=$h{$k}"; }
来源：http://hz.yongpay.top/gtwgsjryzo.html

[T47] Perl：正则捕获
来源：http://hz.hnqzz.top/gtcyhzbths.html

if ($s =~ /(\d+)/) { print $1; }
来源：http://hz.zdqjudy.top/gtlmwzobia.html

[T48] Perl：正则替换
来源：http://hz.cashguo.top/gtvoxrjctr.html

$s =~ s/old/new/g;
来源：http://hz.vqdsnc.cn/gtuzbohhnw.html

[T49] Perl：函数
来源：http://hz.jyoumei.cn/gtbaxnctdp.html

sub add { my ($a, $b) = @_; return $a + $b; }
来源：http://hz.sysykeji.top/gthwhzefvp.html

[T50] Perl：逐行读文件
来源：http://hz.zycfv.cn/gtpitkkxkp.html

open my $fh, "<", "a.txt" or die $!;
来源：http://hz.zycfv.cn/gtmbgjvujr.html

while (my $line = <$fh>) { print $line; }
来源：http://hz.yuanzhike.top/gtxzwtijoh.html

[T51] Scala：Hello World
来源：http://hz.iojbl.cn/gtdxtlwbvp.html

println("Hello")
来源：http://hz.gotoacloud.top/gtbhjokqmw.html

[T52] Scala：变量
来源：http://hz.andypj.xyz/gtjanzrjpl.html

val a = 1;  var b = 2
来源：http://hz.yj202588.top/gtcfvlarqx.html

[T53] Scala：字符串插值
来源：http://hz.zhengqikj.top/gthyuikumd.html

s"值: $b"
来源：http://hz.svipenyu.cn/gtrqvcvnuw.html

[T54] Scala：集合映射
来源：http://hz.yueranfly.top/gtcacglgln.html

List(1, 2, 3).map(_ * 2)
来源：http://hz.ydjk.org.cn/gtfohkvhmv.html

[T55] Scala：集合过滤
来源：http://hz.xziqi.cn/gthamyzwan.html

List(1, 2, 3).filter(_ > 1)
来源：http://hz.sxryk.cn/gtmknicsti.html

[T56] Scala：样例类
来源：http://hz.cqqwz.cn/gtqpxfpjlv.html

case class User(name: String, age: Int)
来源：http://hz.jyoumei.cn/gtkjtajopy.html

[T57] Scala：模式匹配
来源：http://hz.wangdashe.top/gtfsuaxtfv.html

x match { case 1 => "一"; case _ => "其他" }
来源：http://hz.zhongyouzk.top/gtmpgzhxhr.html

[T58] Scala：函数定义
来源：http://hz.yanxiufei.cn/gtcfxfthvl.html

def add(a: Int, b: Int): Int = a + b
来源：http://hz.yangfankeji.com/gtosgihumf.html

[T59] Scala：循环
来源：http://hz.hnqzz.top/gtmzopfsaa.html

for (i <- 1 to 10) println(i)
来源：http://hz.jqgufenzy.top/gtqjhkmkib.html

[T60] Scala：折叠
来源：http://hz.yuanzhike.top/gtzogalyoq.html

List(1, 2, 3).foldLeft(0)(_ + _)
来源：http://hz.ivvv.top/gtcawibvad.html

================================================================================
来源：http://hz.52xcode.cn/gtyweeoxrj.html

U. 高频实用片段（Python / PHP / JavaScript 各 40 条）
来源：http://hz.ehwqpu.com/gtmkhuxpno.html

================================================================================
来源：http://hz.zhaomingkeji.xyz/gtvgiejoxw.html

[U01] Py：创建虚拟环境
来源：http://hz.svipenyu.cn/gtakwirmnr.html

python -m venv .venv && source .venv/bin/activate
来源：http://hz.vqdsnc.cn/gtrdymdglv.html

[U02] Py：导出 / 安装依赖
来源：http://hz.daria6918.cn/gtkuhhvano.html

pip freeze > requirements.txt;  pip install -r requirements.txt
来源：http://hz.guowangkeji.top/gttzsfqctv.html

[U03] Py：加载 .env 配置
来源：http://hz.haohaochexian.top/gthjytjmoy.html

from dotenv import load_dotenv; load_dotenv()
来源：http://hz.hammf.cn/gtrkobrxtu.html

[U04] Py：变量调试打印
来源：http://hz.cqqwz.cn/gtpuokrjji.html

print(f"{x=}")            # 输出 x=值，Python 3.8+
来源：http://hz.jqgufenzy.top/gthbrqifwc.html

[U05] Py：列表去重且保序
来源：http://hz.tanke756.top/gtpljwlfeq.html

list(dict.fromkeys(arr))
来源：http://hz.xuetiantiany.cn/gtmbkzffiz.html

[U06] Py：合并两个字典
来源：http://hz.dianchejie.cn/gtpxawpvbk.html

{**a, **b}
来源：http://hz.aizwys.cn/gtqyygbght.html

[U07] Py：反转字典键值
来源：http://hz.smart0.xyz/gtgscoucju.html

{v: k for k, v in d.items()}
来源：http://hz.sxryk.cn/gtypicrvlw.html

[U08] Py：展平二维列表
来源：http://hz.xuetiantiany.cn/gtrtpyeuep.html

[y for x in nested for y in x]
来源：http://hz.snrcjt.cn/gtdymocyrd.html

[U09] Py：字典取最大值的键
来源：http://hz.ivvv.top/gtfuukdqbj.html

max(d, key=d.get)
来源：http://hz.gaohongyu789.top/gtvamczrky.html

[U10] Py：按值排序字典
来源：http://hz.zhijiandao.cn/gtzqlvqjnb.html

dict(sorted(d.items(), key=lambda kv: kv[1]))
来源：http://hz.dianchejie.cn/gtzklczseu.html

[U11] Py：生成器表达式
来源：http://hz.sysykeji.top/gtofecpnyy.html

(x * 2 for x in arr)
来源：http://hz.pycfn.com/gtcltdxuvw.html

[U12] Py：取出现最多的 3 个元素
来源：http://hz.haohaochexian.top/gtlgcjewzh.html

Counter(arr).most_common(3)
来源：http://hz.nanxuanxn.top/gtkntucrja.html

[U13] Py：固定长度队列
来源：http://hz.fengsongda.top/gtxsccoxvv.html

deque(maxlen=10)
来源：http://hz.jlsjyb.cn/gtmuohnfbw.html

[U14] Py：分组收集到列表
来源：http://hz.hnxiangtu.top/gtrnbtrxfc.html

defaultdict(list)
来源：http://hz.jinqigufen.top/gtqeasvqan.html

[U15] Py：高精度计时
来源：http://hz.cdnleiting.top/gttridnumr.html

t = time.perf_counter()
来源：http://hz.redwolf501.top/gtqiidifuc.html

[U16] Py：命令行参数解析
来源：http://hz.xinyue.icu/gtoqjvyyxt.html

ap = argparse.ArgumentParser();  ap.add_argument("--name");  args = ap.parse_args()
来源：http://hz.aizwys.cn/gtxlgedlvd.html

[U17] Py：初始化日志
来源：http://hz.zhiwuduotai.top/gtrgknhakm.html

logging.basicConfig(level=logging.INFO)
来源：http://hz.jinghuilouyu.cn/gtxplyihgw.html

[U18] Py：预编译正则
来源：http://hz.pengpengdd.cyou/gtdfgtknwa.html

pat = re.compile(r"\d+")
来源：http://hz.cashguo.top/gttxoddozm.html

[U19] Py：正则替换带回调
来源：http://hz.yj202588.top/gtdtpvgjba.html

re.sub(r"\d+", lambda m: str(int(m.group()) * 2), s)
来源：http://hz.yj20258888.top/gtqktmzxrq.html

[U20] Py：缓存函数结果
来源：http://hz.xinyue.icu/gtsnmbnpjq.html

@functools.lru_cache(maxsize=None)
来源：http://hz.nwbrower.top/gtneyqozng.html

[U21] Py：自定义上下文管理器
来源：http://hz.yvedp.cn/gtefokxpzb.html

@contextlib.contextmanager
来源：http://hz.kuanghao11.cn/gtsawjmvfv.html

[U22] Py：矩阵转置
来源：http://hz.zhengqikj.top/gtwthrqmmr.html

list(zip(*m))
来源：http://hz.ywan-chungtsiang.top/gtvzzfnxui.html

[U23] Py：分块读取大文件
来源：http://hz.vqdsnc.cn/gtpkcgyjlf.html

for chunk in iter(lambda: f.read(8192), b""):
来源：http://hz.yvedp.cn/gtjswdzint.html

[U24] Py：路径操作
来源：http://hz.hammf.cn/gttfpjnxmz.html

Path("a/b.txt").parent.mkdir(parents=True, exist_ok=True)
来源：http://hz.jinqigfzy.top/gtcdbdlufn.html

[U25] Py：CSV 按字典读
来源：http://hz.bjfxy.top/gtalnvbhyu.html

csv.DictReader(f)
来源：http://hz.hnxiangtu.top/gthsroueab.html

[U26] Py：并发下载
来源：http://hz.shanyushiyangkeji.top/gtjqepoinu.html

ThreadPoolExecutor(max_workers=8).map(fetch, urls)
来源：http://hz.aizwys.cn/gtvmnfzgya.html

[U27] Py：异步 HTTP
来源：http://hz.svipenyu.cn/gtljniwxca.html

aiohttp.ClientSession() 配合 async with
来源：http://hz.sweek.top/gtbuvzzwfw.html

[U28] Py：类型别名
来源：http://hz.quarkkingdee.top/gtulxvvmfn.html

UserId = int
来源：http://hz.jinqigfzy.top/gtomurolog.html

[U29] Py：属性校验
来源：http://hz.daxiang520.top/gtcsghtvls.html

@property 与 @x.setter 配合
来源：http://hz.zhijiandao.cn/gtxhvxgjel.html

[U30] Py：数据类
来源：http://hz.bjfxy.top/gtctihryuc.html

@dataclass(slots=True)
来源：http://hz.wangdashe.top/gtvpjkcjrw.html

[U31] Py：单测
来源：http://hz.cdnleiting.top/gtnxjveble.html

python -m pytest -q
来源：http://hz.fzhhl.top/gtndzvvzkn.html

[U32] Py：代码格式化
来源：http://hz.ybcxt.top/gtsvqdmpcm.html

ruff format . && ruff check --fix .
来源：http://hz.chenjidiqi.icu/gtsqkplpky.html

[U33] Py：打包发布
来源：http://hz.cucudq.cn/gtuclhbhvk.html

python -m build  （依赖 pyproject.toml）
来源：http://hz.vqdsnc.cn/gtdelmmuly.html

[U34] Py：判断编码
来源：http://hz.yanxiufei.cn/gtzhqboeni.html

chardet.detect(raw)
来源：http://hz.yvedp.cn/gtulzfmjdr.html

[U35] Py：发送邮件
来源：http://hz.xinyue.icu/gtfjhppbuh.html

smtplib.SMTP_SSL(...).send_message(msg)
来源：http://hz.snrcjt.cn/gtlkqvvelu.html

[U36] Py：定时任务
来源：http://hz.zhijiandao.cn/gtsfkksyni.html

schedule.every(10).minutes.do(job)
来源：http://hz.yangfankeji.com/gtczrvdade.html

[U37] Py：读写 Excel
来源：http://hz.ydzc1.top/gticjmvytt.html

pandas.read_excel / DataFrame.to_excel
来源：http://hz.xylfe.cn/gtybpjzvem.html

[U38] Py：获取脚本所在目录
来源：http://hz.cucudq.cn/gtlpwdhvxb.html

Path(__file__).resolve().parent
来源：http://hz.sweek.top/gtjhrnzkbp.html

[U39] Py：判断是否在交互环境
来源：http://hz.c1oappe.top/gtsmgjjftu.html

sys.stdout.isatty()
来源：http://hz.xuanzx.com/gtuexjhcvb.html

[U40] Py：打印到标准错误
来源：http://hz.yangfankeji.com/gtzzuxwxfh.html

print("err", file=sys.stderr)
来源：http://hz.yj202588.top/gtuosmnnyk.html

[U41] PHP：初始化 Composer 项目
来源：http://hz.kuanghao11.cn/gtotqtjowy.html

composer init;  composer require guzzlehttp/guzzle
来源：http://hz.cdnleiting.top/gtsdglwlvz.html

[U42] PHP：PSR-4 自动加载
来源：http://hz.pengpengdd.cyou/gtedglkbzb.html

"autoload": { "psr-4": { "App\\": "src/" } }
来源：http://hz.guowangkeji.top/gtxviikmyl.html

[U43] PHP：声明命名空间
来源：http://hz.nwbrower.top/gtzodxgaeb.html

namespace App\Http;
来源：http://hz.xinyue.icu/gtzkaqsphh.html

[U44] PHP：开启严格类型
来源：http://hz.zhiwuduotai.top/gtqcegawnu.html

declare(strict_types=1);
来源：http://hz.kuanghao11.cn/gtoqlgllzv.html

[U45] PHP：类型声明与返回类型
来源：http://hz.xziqi.cn/gtpfiqbjqp.html

function add(int $a, int $b): int { return $a + $b; }
来源：http://hz.shuidangran.top/gteczzvikx.html

[U46] PHP：可空类型
来源：http://hz.yj20258.top/gtngfpmjgq.html

?string $name = null
来源：http://hz.cdnleiting.top/gtrbgfyllw.html

[U47] PHP：联合类型
来源：http://hz.jyoumei.cn/gtwsbrtpla.html

int|string $id
来源：http://hz.yanxiufei.cn/gtjpqqgdsb.html

[U48] PHP：纯枚举
来源：http://hz.dianchejie.cn/gtrmkzoeof.html

enum Status: string { case Active = "active"; case Off = "off"; }
来源：http://hz.shanyushiyangtech.top/gthnrinkas.html

[U49] PHP：只读属性
来源：http://hz.gotoacloud.top/gtherwjknd.html

public readonly string $name
来源：http://hz.vqdsnc.cn/gtacpqoqbr.html

[U50] PHP：构造器属性提升
来源：http://hz.chenjidiqi.icu/gtenljogow.html

public function __construct(private int $id) {}
来源：http://hz.jiagoushi.top/gtxbdyyrpj.html

[U51] PHP：数组解构
来源：http://hz.xuanzx.com/gtgovxojbw.html

[$a, $b] = $arr;
来源：http://hz.zycfv.cn/gtmeoimkqa.html

[U52] PHP：箭头函数
来源：http://hz.fzhhl.top/gtjvbgtbcd.html

$double = fn($x) => $x * 2;
来源：http://hz.gaohongyu789.top/gtmpnesghx.html

[U53] PHP：空合并运算符
来源：http://hz.zhoulong.xyz/gtutjsyqtq.html

$v = $a ?? $b ?? "default";
来源：http://hz.yueranfly.top/gtxechivyn.html

[U54] PHP：空安全调用
来源：http://hz.andypj.xyz/gtmichtmuo.html

$obj?->method()
来源：http://hz.dianchejie.cn/gtwdeuxpwg.html

[U55] PHP：match 表达式
来源：http://hz.sufxvd.cn/gtchvbnmvh.html

$s = match($x) { 1 => "一", default => "其他" };
来源：http://hz.jlsjyb.cn/gtdiepbqip.html

[U56] PHP：命名参数
来源：http://hz.zhengqikj.top/gtrlxessgi.html

f(a: 1, b: 2)
来源：http://hz.hywenlv.cn/gtqbbldfgx.html

[U57] PHP：字符串插值
来源：http://hz.jqgfzy.top/gtviwlkikv.html

"值: {$a}"
来源：http://hz.shuidangran.top/gtnugzsqtc.html

[U58] PHP：数组三件套
来源：http://hz.vqdsnc.cn/gtgdfanqda.html

array_map($f, $a);  array_filter($a, $f);  array_reduce($a, $f, 0);
来源：http://hz.hongshengwenyu.top/gtvzuuekha.html

[U59] PHP：自定义排序
来源：http://hz.dianchejie.cn/gtacnesrzo.html

usort($arr, fn($a, $b) => $a["age"] <=> $b["age"]);
来源：http://hz.aizwys.cn/gtbvnetkaz.html

[U60] PHP：JSON 编解码
来源：http://hz.jianghu66.top/gtdqmwogjn.html

json_encode($d, JSON_UNESCAPED_UNICODE);  json_decode($s, true);
来源：http://hz.yuxming.cn/gtpgohmqtp.html

[U61] PHP：正则
来源：http://hz.shanyushiyangtech.top/gtzgkkzvuz.html

preg_match('/(\d+)/', $s, $m);  preg_replace('/\d+/', '#', $s);
来源：http://hz.zhaomingkeji.xyz/gtyukgvixz.html

[U62] PHP：日期对象
来源：http://hz.havefunace.top/gtvjijkhhu.html

(new DateTimeImmutable())->format("Y-m-d");
来源：http://hz.zhiwuduotai.top/gtxxzsbpvp.html

[U63] PHP：文件读写
来源：http://hz.shuidangran.top/gtugpanzao.html

file_get_contents($f);  file_put_contents($f, $data);
来源：http://hz.redwolf501.top/gtqzbvodgo.html

[U64] PHP：目录遍历
来源：http://hz.sxryk.cn/gtwkbcwwoq.html

glob("dir/*.php");  scandir("dir");
来源：http://hz.ivvv.top/gtqaaajtcw.html

[U65] PHP：会话
来源：http://hz.redwolf501.top/gtquhuwtdp.html

session_start();  $_SESSION["uid"] = 1;
来源：http://hz.9152youxi.cn/gtwmcjffap.html

[U66] PHP：设置 Cookie
来源：http://hz.haohaochexian.top/gtjulfnhnr.html

setcookie("token", $v, ["httponly" => true, "samesite" => "Lax"]);
来源：http://hz.ydzc1.top/gtfkqdfzrh.html

[U67] PHP：处理文件上传
来源：http://hz.yangfankeji.com/gtlxhdarpl.html

$_FILES["file"]["tmp_name"] 与 move_uploaded_file()
来源：http://hz.zhongyouzk.top/gtsyzhltsv.html

[U68] PHP：PDO 连接
来源：http://hz.jqgfzy.top/gtxojjrjeg.html

$pdo = new PDO("mysql:host=localhost;dbname=app", "root", "");
来源：http://hz.xziqi.cn/gtocezvnkr.html

[U69] PHP：PDO 预处理
来源：http://hz.tanke756.top/gtweqhlxvu.html

$stmt = $pdo->prepare("SELECT * FROM users WHERE id = ?");  $stmt->execute([$id]);
来源：http://hz.yuxming.cn/gtvjemwoua.html

[U70] PHP：PDO 事务
来源：http://hz.shuidangran.top/gtrdcvdmsd.html

$pdo->beginTransaction();  $pdo->commit();  $pdo->rollBack();
来源：http://hz.sufxvd.cn/gtrutfihzy.html

[U71] PHP：抛出异常
来源：http://hz.gzhubu.top/gtjjwxaxmk.html

throw new RuntimeException("失败", 500);
来源：http://hz.zhiwuduotai.top/gtrhwdzert.html

[U72] PHP：写错误日志
来源：http://hz.andypj.xyz/gttengrcqf.html

error_log("失败: " . $e->getMessage());
来源：http://hz.wangshuangyany.cn/gtmkzysjzv.html

[U73] PHP：读取 ini 配置
来源：http://hz.dashuyun.cn/gtkvzovvoz.html

parse_ini_file("config.ini", true)
来源：http://hz.shuidangran.top/gtkqwgrrou.html

[U74] PHP：读取环境变量
来源：http://hz.hfpthk.cn/gtvavivzzu.html

getenv("APP_ENV") ?: "production"
来源：http://hz.aibaodan.cn/gtneyviago.html

[U75] PHP：依赖注入
来源：http://hz.pycfn.com/gtwhtaokkm.html

composer require psr/container
来源：http://hz.feifeiyinyue.top/gtowjkayuz.html

[U76] PHP：简单路由
来源：http://hz.chenjidiqi.icu/gtutdgkljy.html

$path = parse_url($_SERVER["REQUEST_URI"], PHP_URL_PATH);
来源：http://hz.jiagoushi.top/gtyaagnlra.html

[U77] PHP：模板渲染
来源：http://hz.redwolf501.top/gtoiiyhczl.html

composer require twig/twig
来源：http://hz.dashuyun.cn/gtflanypsu.html

[U78] PHP：单元测试
来源：http://hz.nwbrower.top/gtxdogoyoh.html

composer require --dev phpunit/phpunit
来源：http://hz.aibaodan.cn/gtawjdyynj.html

[U79] PHP：静态分析
来源：http://hz.xingfuxueyuan.xyz/gtqmtsqbkw.html

composer require --dev phpstan/phpstan
来源：http://hz.smart0.xyz/gtnxvkxjdy.html

[U80] PHP：代码规范修复
来源：http://hz.sufxvd.cn/gtybquuyap.html

composer require --dev friendsofphp/php-cs-fixer
来源：http://hz.sweek.top/gtnvvwahgl.html


<!-- 参考信息 -->