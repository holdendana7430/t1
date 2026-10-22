代发 wailian999

[T05] Kotlin：when 表达式
来源：http://www.52xcode.cn/Article/details/gt2ngtxiyrd.html

val s = when (x) { 1 -> "一" else -> "其他" }   // 多分支时每个分支单独一行
来源：http://www.ydjk.org.cn/Article/details/gt2xxpamzns.html

[T06] Kotlin：集合映射
来源：http://www.52xcode.cn/Article/details/gt2pkbirfut.html

listOf(1, 2, 3).map { it * 2 }
来源：http://www.52xcode.cn/Article/details/gt2mczmhigp.html

[T07] Kotlin：集合过滤
来源：http://www.ydjk.org.cn/Article/details/gt2iyfhslmj.html

listOf(1, 2, 3).filter { it > 1 }
来源：http://www.52xcode.cn/Article/details/gt2trlkecjj.html

[T08] Kotlin：数据类
来源：http://www.ydjk.org.cn/Article/details/gt2zjuzxhap.html

data class User(val name: String, val age: Int)
来源：http://www.52xcode.cn/Article/details/gt2gsbxmeon.html

[T09] Kotlin：扩展函数
来源：http://www.52xcode.cn/Article/details/gt2kgfvponl.html

fun String.exclaim() = this + "!"
来源：http://www.ydjk.org.cn/Article/details/gt2vchpnsdd.html

[T10] Kotlin：默认参数
来源：http://www.52xcode.cn/Article/details/gt2djltiyik.html

fun greet(name: String = "World") = "Hi $name"
来源：http://www.52xcode.cn/Article/details/gt2axxqfvam.html

[T11] Kotlin：协程
来源：http://www.ydjk.org.cn/Article/details/gt2xfydsmaw.html

GlobalScope.launch { delay(1000); println("done") }
来源：http://www.ydjk.org.cn/Article/details/gt2bklztfeu.html

[T12] Kotlin：解构声明
来源：http://www.ydjk.org.cn/Article/details/gt2bwcobseg.html

val (a, b) = Pair(1, 2)
来源：http://www.ydjk.org.cn/Article/details/gt2muotgbrj.html

[T13] Kotlin：只读 Map
来源：http://www.ydjk.org.cn/Article/details/gt2zheassjf.html

val m = mapOf("a" to 1)
来源：http://www.52xcode.cn/Article/details/gt2txoafqea.html

[T14] Kotlin：循环
来源：http://www.ydjk.org.cn/Article/details/gt2jddaruqm.html

for (i in 1..10) println(i)
来源：http://www.ydjk.org.cn/Article/details/gt2qvynogbv.html

[T15] Kotlin：接口
来源：http://www.52xcode.cn/Article/details/gt2gueoqqpi.html

interface Shape { fun area(): Double }
来源：http://www.52xcode.cn/Article/details/gt2qujccfnm.html

[T16] Swift：Hello World
来源：http://www.52xcode.cn/Article/details/gt2alfxntqc.html

print("Hello")
来源：http://www.52xcode.cn/Article/details/gt2bsvcpilu.html

[T17] Swift：变量与常量
来源：http://www.ydjk.org.cn/Article/details/gt2mwswfvqt.html

var a = 1;  let b = 2
来源：http://www.ydjk.org.cn/Article/details/gt2hjvmpkvm.html

[T18] Swift：字符串插值
来源：http://www.52xcode.cn/Article/details/gt2utsqnygg.html

"值: \(b)"
来源：http://www.ydjk.org.cn/Article/details/gt2oenjqcik.html

[T19] Swift：可选绑定
来源：http://www.ydjk.org.cn/Article/details/gt2ahquwccc.html

if let n = opt { print(n) }
来源：http://www.ydjk.org.cn/Article/details/gt2epkckhml.html

[T20] Swift：数组操作
来源：http://www.52xcode.cn/Article/details/gt2ydcxsron.html

var a = [1, 2, 3];  a.append(4)
来源：http://www.52xcode.cn/Article/details/gt2suufkpqb.html

[T21] Swift：遍历
来源：http://www.52xcode.cn/Article/details/gt2yriprrgk.html

for x in a { print(x) }
来源：http://www.52xcode.cn/Article/details/gt2fibmxlap.html

[T22] Swift：字典
来源：http://www.52xcode.cn/Article/details/gt2ooakbibs.html

var d = ["a": 1];  d["b"] = 2
来源：http://www.52xcode.cn/Article/details/gt2zvwytmvw.html

[T23] Swift：函数
来源：http://www.ydjk.org.cn/Article/details/gt2vavrtdqq.html

func add(_ a: Int, _ b: Int) -> Int { a + b }
来源：http://www.52xcode.cn/Article/details/gt2lqmflsam.html

[T24] Swift：闭包
来源：http://www.52xcode.cn/Article/details/gt2hnpnwpkd.html

let f = { (x: Int) -> Int in x * 2 }
来源：http://www.52xcode.cn/Article/details/gt2kqeizvcj.html

[T25] Swift：结构体
来源：http://www.ydjk.org.cn/Article/details/gt2igvwpevm.html

struct P { var x: Int }
来源：http://www.52xcode.cn/Article/details/gt2qbuxwpci.html

[T26] Swift：类与重写
来源：http://www.52xcode.cn/Article/details/gt2mlwewotz.html

class A: Base { override func f() {} }
来源：http://www.ydjk.org.cn/Article/details/gt2pgmxbsqw.html

[T27] Swift：错误处理
来源：http://www.ydjk.org.cn/Article/details/gt2gclvumkw.html

do { try f() } catch { print(error) }
来源：http://www.ydjk.org.cn/Article/details/gt2xjayexwd.html

[T28] Swift：枚举
来源：http://www.ydjk.org.cn/Article/details/gt2pnzepfau.html

enum Color { case red, green }
来源：http://www.ydjk.org.cn/Article/details/gt2lumzgrmp.html

[T29] Swift：guard 提前返回
来源：http://www.ydjk.org.cn/Article/details/gt2lakikros.html

guard let x = opt else { return }
来源：http://www.52xcode.cn/Article/details/gt2xokubvat.html

[T30] Swift：协议
来源：http://www.ydjk.org.cn/Article/details/gt2famoeawd.html

protocol Shape { func area() -> Double }
来源：http://www.52xcode.cn/Article/details/gt2kokbmykn.html

[T31] Lua：Hello World
来源：http://www.52xcode.cn/Article/details/gt2czdyiplg.html

print("Hello")
来源：http://www.ydjk.org.cn/Article/details/gt2vzomjfcq.html

[T32] Lua：局部变量
来源：http://www.ydjk.org.cn/Article/details/gt2pmsedhqf.html

local a = 1
来源：http://www.ydjk.org.cn/Article/details/gt2nowkfnqm.html

[T33] Lua：表（数组）
来源：http://www.52xcode.cn/Article/details/gt2rkbcfmez.html

local t = {1, 2, 3};  t[4] = 4
来源：http://www.52xcode.cn/Article/details/gt2ndvczufw.html

[T34] Lua：遍历表
来源：http://www.ydjk.org.cn/Article/details/gt2dwfranfd.html

for i, v in ipairs(t) do print(i, v) end
来源：http://www.52xcode.cn/Article/details/gt2hheurqvg.html

[T35] Lua：字典表
来源：http://www.52xcode.cn/Article/details/gt2shsxqnpf.html

local d = { a = 1 };  d.b = 2
来源：http://www.52xcode.cn/Article/details/gt2mvirzfjz.html

[T36] Lua：函数
来源：http://www.ydjk.org.cn/Article/details/gt2euhxyctx.html

function add(a, b) return a + b end
来源：http://www.ydjk.org.cn/Article/details/gt2ztbegeoy.html

[T37] Lua：字符串拼接
来源：http://www.ydjk.org.cn/Article/details/gt2lyjsguqe.html

"a" .. "b"
来源：http://www.52xcode.cn/Article/details/gt2rjxhpwcq.html

[T38] Lua：条件
来源：http://www.ydjk.org.cn/Article/details/gt2mmponbxp.html

if x > 0 then print("正") end
来源：http://www.ydjk.org.cn/Article/details/gt2dysmoobi.html

[T39] Lua：模式匹配
来源：http://www.52xcode.cn/Article/details/gt2kqmsesbb.html

string.find(s, "%d+")
来源：http://www.ydjk.org.cn/Article/details/gt2zebpbdxf.html

[T40] Lua：元表
来源：http://www.52xcode.cn/Article/details/gt2qzcnnlbz.html

setmetatable({}, { __index = base })
来源：http://www.ydjk.org.cn/Article/details/gt2begkugqc.html

[T41] Perl：Hello World
来源：http://www.ydjk.org.cn/Article/details/gt2tjynfrcn.html

print "Hello\n";
来源：http://www.52xcode.cn/Article/details/gt2zupqgwdx.html

[T42] Perl：变量类型
来源：http://www.52xcode.cn/Article/details/gt2pymjdyzw.html

my $a = 1;  my @arr = (1, 2, 3);  my %h = (a => 1);
来源：http://www.ydjk.org.cn/Article/details/gt2ufroihjj.html

[T43] Perl：字符串插值
来源：http://www.ydjk.org.cn/Article/details/gt2tpmmpdhh.html

"值: $a"
来源：http://www.52xcode.cn/Article/details/gt2akhqgzfo.html

[T44] Perl：条件
来源：http://www.ydjk.org.cn/Article/details/gt2pcogyzjo.html

if ($a > 0) { print "正"; }
来源：http://www.ydjk.org.cn/Article/details/gt2izbpteiu.html

[T45] Perl：数组遍历
来源：http://www.ydjk.org.cn/Article/details/gt2piwdtchc.html

for my $x (@arr) { print $x; }
来源：http://www.52xcode.cn/Article/details/gt2qqemxlpo.html

[T46] Perl：哈希操作
来源：http://www.ydjk.org.cn/Article/details/gt2qlelhxlc.html

$h{b} = 2;  for my $k (keys %h) { print "$k=$h{$k}"; }
来源：http://www.52xcode.cn/Article/details/gt2mqdxqlzq.html

[T47] Perl：正则捕获
来源：http://www.ydjk.org.cn/Article/details/gt2ymxhdiir.html

if ($s =~ /(\d+)/) { print $1; }
来源：http://www.52xcode.cn/Article/details/gt2vlpbcszm.html

[T48] Perl：正则替换
来源：http://www.52xcode.cn/Article/details/gt2mfbvmfei.html

$s =~ s/old/new/g;
来源：http://www.ydjk.org.cn/Article/details/gt2hpmqfwim.html

[T49] Perl：函数
来源：http://www.52xcode.cn/Article/details/gt2fpsysyas.html

sub add { my ($a, $b) = @_; return $a + $b; }
来源：http://www.52xcode.cn/Article/details/gt2zkikjdcl.html

[T50] Perl：逐行读文件
来源：http://www.52xcode.cn/Article/details/gt2beamnjgk.html

open my $fh, "<", "a.txt" or die $!;
来源：http://www.ydjk.org.cn/Article/details/gt2nmxgdfjg.html

while (my $line = <$fh>) { print $line; }
来源：http://www.ydjk.org.cn/Article/details/gt2proflkuv.html

[T51] Scala：Hello World
来源：http://www.52xcode.cn/Article/details/gt2kmkcmbjw.html

println("Hello")
来源：http://www.52xcode.cn/Article/details/gt2qdkmfluj.html

[T52] Scala：变量
来源：http://www.52xcode.cn/Article/details/gt2tjxgxkbo.html

val a = 1;  var b = 2
来源：http://www.ydjk.org.cn/Article/details/gt2kwlbkthf.html

[T53] Scala：字符串插值
来源：http://www.ydjk.org.cn/Article/details/gt2hffnchmg.html

s"值: $b"
来源：http://www.ydjk.org.cn/Article/details/gt2xrngpajt.html

[T54] Scala：集合映射
来源：http://www.52xcode.cn/Article/details/gt2tmwybazd.html

List(1, 2, 3).map(_ * 2)
来源：http://www.52xcode.cn/Article/details/gt2qfaserja.html

[T55] Scala：集合过滤
来源：http://www.52xcode.cn/Article/details/gt2zveyghyr.html

List(1, 2, 3).filter(_ > 1)
来源：http://www.52xcode.cn/Article/details/gt2mjjyqqax.html

[T56] Scala：样例类
来源：http://www.52xcode.cn/Article/details/gt2igbydsox.html

case class User(name: String, age: Int)
来源：http://www.ydjk.org.cn/Article/details/gt2imkoidrz.html

[T57] Scala：模式匹配
来源：http://www.ydjk.org.cn/Article/details/gt2hwomxunr.html

x match { case 1 => "一"; case _ => "其他" }
来源：http://www.ydjk.org.cn/Article/details/gt2futuuzyl.html

[T58] Scala：函数定义
来源：http://www.ydjk.org.cn/Article/details/gt2ejiohgyv.html

def add(a: Int, b: Int): Int = a + b
来源：http://www.52xcode.cn/Article/details/gt2lbuqrxwn.html

[T59] Scala：循环
来源：http://www.ydjk.org.cn/Article/details/gt2ysxsundp.html

for (i <- 1 to 10) println(i)
来源：http://www.ydjk.org.cn/Article/details/gt2ztpnpcaz.html

[T60] Scala：折叠
来源：http://www.52xcode.cn/Article/details/gt2iaajyfsh.html

List(1, 2, 3).foldLeft(0)(_ + _)
来源：http://www.ydjk.org.cn/Article/details/gt2zfhfmewg.html

================================================================================
来源：http://www.ydjk.org.cn/Article/details/gt2lvmqzyjd.html

U. 高频实用片段（Python / PHP / JavaScript 各 40 条）
来源：http://www.52xcode.cn/Article/details/gt2zpkyfenf.html

================================================================================
来源：http://www.52xcode.cn/Article/details/gt2gaykkqvm.html

[U01] Py：创建虚拟环境
来源：http://www.ydjk.org.cn/Article/details/gt2mckcjyfl.html

python -m venv .venv && source .venv/bin/activate
来源：http://www.ydjk.org.cn/Article/details/gt2xqbrnppb.html

[U02] Py：导出 / 安装依赖
来源：http://www.ydjk.org.cn/Article/details/gt2zdsvdqhg.html

pip freeze > requirements.txt;  pip install -r requirements.txt
来源：http://www.ydjk.org.cn/Article/details/gt2vgijwrmv.html

[U03] Py：加载 .env 配置
来源：http://www.ydjk.org.cn/Article/details/gt2utorthyn.html

from dotenv import load_dotenv; load_dotenv()
来源：http://www.52xcode.cn/Article/details/gt2mfkauxbe.html

[U04] Py：变量调试打印
来源：http://www.52xcode.cn/Article/details/gt2clttykwe.html

print(f"{x=}")            # 输出 x=值，Python 3.8+
来源：http://www.52xcode.cn/Article/details/gt2zbwuwwzr.html

[U05] Py：列表去重且保序
来源：http://www.52xcode.cn/Article/details/gt2nlzwanbx.html

list(dict.fromkeys(arr))
来源：http://www.52xcode.cn/Article/details/gt2dkuibgjq.html

[U06] Py：合并两个字典
来源：http://www.52xcode.cn/Article/details/gt2qbjwawjo.html

{**a, **b}
来源：http://www.52xcode.cn/Article/details/gt2cxxsvpnm.html

[U07] Py：反转字典键值
来源：http://www.52xcode.cn/Article/details/gt2htgsvpcz.html

{v: k for k, v in d.items()}
来源：http://www.52xcode.cn/Article/details/gt2bqkqkvlh.html

[U08] Py：展平二维列表
来源：http://www.ydjk.org.cn/Article/details/gt2rrxumtbx.html

[y for x in nested for y in x]
来源：http://www.52xcode.cn/Article/details/gt2tavsqzvw.html

[U09] Py：字典取最大值的键
来源：http://www.52xcode.cn/Article/details/gt2dnlxuzin.html

max(d, key=d.get)
来源：http://www.ydjk.org.cn/Article/details/gt2svxapysw.html

[U10] Py：按值排序字典
来源：http://www.ydjk.org.cn/Article/details/gt2catdsjjj.html

dict(sorted(d.items(), key=lambda kv: kv[1]))
来源：http://www.52xcode.cn/Article/details/gt2ztdeliay.html

[U11] Py：生成器表达式
来源：http://www.52xcode.cn/Article/details/gt2fxxuusxj.html

(x * 2 for x in arr)
来源：http://www.52xcode.cn/Article/details/gt2jeguzqgq.html

[U12] Py：取出现最多的 3 个元素
来源：http://www.ydjk.org.cn/Article/details/gt2jabknjjj.html

Counter(arr).most_common(3)
来源：http://www.ydjk.org.cn/Article/details/gt2kywqfzrw.html

[U13] Py：固定长度队列
来源：http://www.52xcode.cn/Article/details/gt2xogjvwsz.html

deque(maxlen=10)
来源：http://www.52xcode.cn/Article/details/gt2pigurfyx.html

[U14] Py：分组收集到列表
来源：http://www.52xcode.cn/Article/details/gt2aphlrtpv.html

defaultdict(list)
来源：http://www.52xcode.cn/Article/details/gt2mqgdzjun.html

[U15] Py：高精度计时
来源：http://www.52xcode.cn/Article/details/gt2uaqbsxxv.html

t = time.perf_counter()
来源：http://www.52xcode.cn/Article/details/gt2odkulwzw.html

[U16] Py：命令行参数解析
来源：http://www.ydjk.org.cn/Article/details/gt2znwedbeq.html

ap = argparse.ArgumentParser();  ap.add_argument("--name");  args = ap.parse_args()
来源：http://www.ydjk.org.cn/Article/details/gt2vrhxzjwc.html

[U17] Py：初始化日志
来源：http://www.ydjk.org.cn/Article/details/gt2vbakxwoi.html

logging.basicConfig(level=logging.INFO)
来源：http://www.ydjk.org.cn/Article/details/gt2vqsljohf.html

[U18] Py：预编译正则
来源：http://www.52xcode.cn/Article/details/gt2kylivtrk.html

pat = re.compile(r"\d+")
来源：http://www.52xcode.cn/Article/details/gt2sydafqin.html

[U19] Py：正则替换带回调
来源：http://www.52xcode.cn/Article/details/gt2fomfymhp.html

re.sub(r"\d+", lambda m: str(int(m.group()) * 2), s)
来源：http://www.ydjk.org.cn/Article/details/gt2zrjdkyji.html

[U20] Py：缓存函数结果
来源：http://www.52xcode.cn/Article/details/gt2hcfwhpam.html

@functools.lru_cache(maxsize=None)
来源：http://www.ydjk.org.cn/Article/details/gt2rogctqol.html

[U21] Py：自定义上下文管理器
来源：http://www.52xcode.cn/Article/details/gt2tzzmoypd.html

@contextlib.contextmanager
来源：http://www.52xcode.cn/Article/details/gt2iuzjepzr.html

[U22] Py：矩阵转置
来源：http://www.ydjk.org.cn/Article/details/gt2dcidywxi.html

list(zip(*m))
来源：http://www.ydjk.org.cn/Article/details/gt2uqksrwhu.html

[U23] Py：分块读取大文件
来源：http://www.52xcode.cn/Article/details/gt2pblublyu.html

for chunk in iter(lambda: f.read(8192), b""):
来源：http://www.ydjk.org.cn/Article/details/gt2qzujpqsi.html

[U24] Py：路径操作
来源：http://www.ydjk.org.cn/Article/details/gt2bxtxxuxn.html

Path("a/b.txt").parent.mkdir(parents=True, exist_ok=True)
来源：http://www.52xcode.cn/Article/details/gt2kwmwqvhl.html

[U25] Py：CSV 按字典读
来源：http://www.52xcode.cn/Article/details/gt2dckqdmuj.html

csv.DictReader(f)
来源：http://www.ydjk.org.cn/Article/details/gt2jwtbsjcc.html

[U26] Py：并发下载
来源：http://www.ydjk.org.cn/Article/details/gt2qavaesgq.html

ThreadPoolExecutor(max_workers=8).map(fetch, urls)
来源：http://www.52xcode.cn/Article/details/gt2nmmpgrxi.html

[U27] Py：异步 HTTP
来源：http://www.ydjk.org.cn/Article/details/gt2wznnqjaz.html

aiohttp.ClientSession() 配合 async with
来源：http://www.52xcode.cn/Article/details/gt2qckqqsij.html

[U28] Py：类型别名
来源：http://www.52xcode.cn/Article/details/gt2oerieupp.html

UserId = int
来源：http://www.52xcode.cn/Article/details/gt2ipllswlm.html

[U29] Py：属性校验
来源：http://www.ydjk.org.cn/Article/details/gt2cobnxitt.html

@property 与 @x.setter 配合
来源：http://www.ydjk.org.cn/Article/details/gt2vrkldtly.html

[U30] Py：数据类
来源：http://www.52xcode.cn/Article/details/gt2nfkhvsiy.html

@dataclass(slots=True)
来源：http://www.ydjk.org.cn/Article/details/gt2unpagoqj.html

[U31] Py：单测
来源：http://www.ydjk.org.cn/Article/details/gt2cbcvwtey.html

python -m pytest -q
来源：http://www.ydjk.org.cn/Article/details/gt2eqvbwwlm.html

[U32] Py：代码格式化
来源：http://www.ydjk.org.cn/Article/details/gt2uumcjbks.html

ruff format . && ruff check --fix .
来源：http://www.ydjk.org.cn/Article/details/gt2vzgzqkkv.html

[U33] Py：打包发布
来源：http://www.ydjk.org.cn/Article/details/gt2pksasxnv.html

python -m build  （依赖 pyproject.toml）
来源：http://www.52xcode.cn/Article/details/gt2bykhcccl.html

[U34] Py：判断编码
来源：http://www.52xcode.cn/Article/details/gt2ligxbshf.html

chardet.detect(raw)
来源：http://www.52xcode.cn/Article/details/gt2qkjvpdlw.html

[U35] Py：发送邮件
来源：http://www.52xcode.cn/Article/details/gt2zulpcjdt.html

smtplib.SMTP_SSL(...).send_message(msg)
来源：http://www.52xcode.cn/Article/details/gt2hcgxgnqn.html

[U36] Py：定时任务
来源：http://www.52xcode.cn/Article/details/gt2utvbmhga.html

schedule.every(10).minutes.do(job)
来源：http://www.52xcode.cn/Article/details/gt2vcralfuc.html

[U37] Py：读写 Excel
来源：http://www.ydjk.org.cn/Article/details/gt2ogdfdavj.html

pandas.read_excel / DataFrame.to_excel
来源：http://www.52xcode.cn/Article/details/gt2hrpmlmnm.html

[U38] Py：获取脚本所在目录
来源：http://www.ydjk.org.cn/Article/details/gt2iwhpjvuy.html

Path(__file__).resolve().parent
来源：http://www.ydjk.org.cn/Article/details/gt2jvddxvsb.html

[U39] Py：判断是否在交互环境
来源：http://www.52xcode.cn/Article/details/gt2krkdhfrr.html

sys.stdout.isatty()
来源：http://www.ydjk.org.cn/Article/details/gt2pjvpbjnk.html

[U40] Py：打印到标准错误
来源：http://www.52xcode.cn/Article/details/gt2zyzqmkyt.html

print("err", file=sys.stderr)
来源：http://www.52xcode.cn/Article/details/gt2demrayxu.html

[U41] PHP：初始化 Composer 项目
来源：http://www.52xcode.cn/Article/details/gt2aqvsmujh.html

composer init;  composer require guzzlehttp/guzzle
来源：http://www.52xcode.cn/Article/details/gt2tywlmsyj.html

[U42] PHP：PSR-4 自动加载
来源：http://www.ydjk.org.cn/Article/details/gt2fjpcldbg.html

"autoload": { "psr-4": { "App\\": "src/" } }
来源：http://www.ydjk.org.cn/Article/details/gt2nuebrdgp.html

[U43] PHP：声明命名空间
来源：http://www.ydjk.org.cn/Article/details/gt2dxdixsyt.html

namespace App\Http;
来源：http://www.52xcode.cn/Article/details/gt2oicyydcg.html

[U44] PHP：开启严格类型
来源：http://www.52xcode.cn/Article/details/gt2fuwxsrtx.html

declare(strict_types=1);
来源：http://www.52xcode.cn/Article/details/gt2zjczqojv.html

[U45] PHP：类型声明与返回类型
来源：http://www.ydjk.org.cn/Article/details/gt2tqqhzjky.html

function add(int $a, int $b): int { return $a + $b; }
来源：http://www.52xcode.cn/Article/details/gt2pgnqxvgq.html

[U46] PHP：可空类型
来源：http://www.52xcode.cn/Article/details/gt2eooeiufj.html

?string $name = null
来源：http://www.52xcode.cn/Article/details/gt2hxwjkysx.html

[U47] PHP：联合类型
来源：http://www.ydjk.org.cn/Article/details/gt2ojbtitwp.html

int|string $id
来源：http://www.ydjk.org.cn/Article/details/gt2ibrxiaqt.html

[U48] PHP：纯枚举
来源：http://www.52xcode.cn/Article/details/gt2nxzcxnpw.html

enum Status: string { case Active = "active"; case Off = "off"; }
来源：http://www.52xcode.cn/Article/details/gt2eevpjcdh.html

[U49] PHP：只读属性
来源：http://www.52xcode.cn/Article/details/gt2tpmdlndp.html

public readonly string $name
来源：http://www.52xcode.cn/Article/details/gt2ywrjhjtk.html

[U50] PHP：构造器属性提升
来源：http://www.52xcode.cn/Article/details/gt2dzjqngcn.html

public function __construct(private int $id) {}
来源：http://www.ydjk.org.cn/Article/details/gt2iolkhidp.html

[U51] PHP：数组解构
来源：http://www.52xcode.cn/Article/details/gt2lmzitszb.html

[$a, $b] = $arr;
来源：http://www.ydjk.org.cn/Article/details/gt2punsxoel.html

[U52] PHP：箭头函数
来源：http://www.ydjk.org.cn/Article/details/gt2syrcjwkm.html

$double = fn($x) => $x * 2;
来源：http://www.52xcode.cn/Article/details/gt2czcjkelf.html

[U53] PHP：空合并运算符
来源：http://www.ydjk.org.cn/Article/details/gt2jcczoraq.html

$v = $a ?? $b ?? "default";
来源：http://www.ydjk.org.cn/Article/details/gt2bsfoettb.html

[U54] PHP：空安全调用
来源：http://www.52xcode.cn/Article/details/gt2uhorzpoe.html

$obj?->method()
来源：http://www.ydjk.org.cn/Article/details/gt2smpnnohr.html

[U55] PHP：match 表达式
来源：http://www.ydjk.org.cn/Article/details/gt2xnkmympu.html

$s = match($x) { 1 => "一", default => "其他" };
来源：http://www.ydjk.org.cn/Article/details/gt2airiamff.html

[U56] PHP：命名参数
来源：http://www.ydjk.org.cn/Article/details/gt2htbohfoa.html

f(a: 1, b: 2)
来源：http://www.52xcode.cn/Article/details/gt2iesvqwok.html

[U57] PHP：字符串插值
来源：http://www.ydjk.org.cn/Article/details/gt2jvmvfqhd.html

"值: {$a}"
来源：http://www.ydjk.org.cn/Article/details/gt2yofjmdzk.html

[U58] PHP：数组三件套
来源：http://www.52xcode.cn/Article/details/gt2ucsohhod.html

array_map($f, $a);  array_filter($a, $f);  array_reduce($a, $f, 0);
来源：http://www.ydjk.org.cn/Article/details/gt2aqwtmxag.html

[U59] PHP：自定义排序
来源：http://www.ydjk.org.cn/Article/details/gt2lgwymhqn.html

usort($arr, fn($a, $b) => $a["age"] <=> $b["age"]);
来源：http://www.52xcode.cn/Article/details/gt2tsllbxyn.html

[U60] PHP：JSON 编解码
来源：http://www.ydjk.org.cn/Article/details/gt2iasthepz.html

json_encode($d, JSON_UNESCAPED_UNICODE);  json_decode($s, true);
来源：http://www.ydjk.org.cn/Article/details/gt2uzczqlku.html

[U61] PHP：正则
来源：http://www.52xcode.cn/Article/details/gt2khmfjfke.html

preg_match('/(\d+)/', $s, $m);  preg_replace('/\d+/', '#', $s);
来源：http://www.ydjk.org.cn/Article/details/gt2ksgtlupe.html

[U62] PHP：日期对象
来源：http://www.52xcode.cn/Article/details/gt2zoiimyjc.html

(new DateTimeImmutable())->format("Y-m-d");
来源：http://www.52xcode.cn/Article/details/gt2uqlslxbg.html

[U63] PHP：文件读写
来源：http://www.52xcode.cn/Article/details/gt2etjjextd.html

file_get_contents($f);  file_put_contents($f, $data);
来源：http://www.52xcode.cn/Article/details/gt2xdizmsau.html

[U64] PHP：目录遍历
来源：http://www.52xcode.cn/Article/details/gt2thglswsx.html

glob("dir/*.php");  scandir("dir");
来源：http://www.ydjk.org.cn/Article/details/gt2bdaetqyb.html

[U65] PHP：会话
来源：http://www.52xcode.cn/Article/details/gt2oluwlafr.html

session_start();  $_SESSION["uid"] = 1;
来源：http://www.52xcode.cn/Article/details/gt2vgpujkho.html

[U66] PHP：设置 Cookie
来源：http://www.ydjk.org.cn/Article/details/gt2gaieksom.html

setcookie("token", $v, ["httponly" => true, "samesite" => "Lax"]);
来源：http://www.52xcode.cn/Article/details/gt2mixaeicd.html

[U67] PHP：处理文件上传
来源：http://www.52xcode.cn/Article/details/gt2odggnbuc.html

$_FILES["file"]["tmp_name"] 与 move_uploaded_file()
来源：http://www.52xcode.cn/Article/details/gt2vdflzsuo.html

[U68] PHP：PDO 连接
来源：http://www.ydjk.org.cn/Article/details/gt2ksxzkftw.html

$pdo = new PDO("mysql:host=localhost;dbname=app", "root", "");
来源：http://www.ydjk.org.cn/Article/details/gt2pzqprwxd.html

[U69] PHP：PDO 预处理
来源：http://www.52xcode.cn/Article/details/gt2lnqkscnr.html

$stmt = $pdo->prepare("SELECT * FROM users WHERE id = ?");  $stmt->execute([$id]);
来源：http://www.ydjk.org.cn/Article/details/gt2gsxmwlvi.html

[U70] PHP：PDO 事务
来源：http://www.52xcode.cn/Article/details/gt2fcjhdzvx.html

$pdo->beginTransaction();  $pdo->commit();  $pdo->rollBack();
来源：http://www.52xcode.cn/Article/details/gt2ecalyrfn.html

[U71] PHP：抛出异常
来源：http://www.52xcode.cn/Article/details/gt2zqdydkko.html

throw new RuntimeException("失败", 500);
来源：http://www.ydjk.org.cn/Article/details/gt2vqsxkjtx.html

[U72] PHP：写错误日志
来源：http://www.ydjk.org.cn/Article/details/gt2ocoxfyim.html

error_log("失败: " . $e->getMessage());
来源：http://www.52xcode.cn/Article/details/gt2chbfhuoh.html

[U73] PHP：读取 ini 配置
来源：http://www.ydjk.org.cn/Article/details/gt2alklymrm.html

parse_ini_file("config.ini", true)
来源：http://www.52xcode.cn/Article/details/gt2tpqxabdi.html

[U74] PHP：读取环境变量
来源：http://www.ydjk.org.cn/Article/details/gt2jujxqugw.html

getenv("APP_ENV") ?: "production"
来源：http://www.ydjk.org.cn/Article/details/gt2dxemoelx.html

[U75] PHP：依赖注入
来源：http://www.52xcode.cn/Article/details/gt2nkcsihhg.html

composer require psr/container
来源：http://www.ydjk.org.cn/Article/details/gt2ycpnbkfu.html

[U76] PHP：简单路由
来源：http://www.52xcode.cn/Article/details/gt2coipisiy.html

$path = parse_url($_SERVER["REQUEST_URI"], PHP_URL_PATH);
来源：http://www.52xcode.cn/Article/details/gt2ycqqmpne.html

[U77] PHP：模板渲染
来源：http://www.ydjk.org.cn/Article/details/gt2ktxpaxtw.html

composer require twig/twig
来源：http://www.ydjk.org.cn/Article/details/gt2fnmvhnos.html

[U78] PHP：单元测试
来源：http://www.52xcode.cn/Article/details/gt2spkrjzue.html

composer require --dev phpunit/phpunit
来源：http://www.ydjk.org.cn/Article/details/gt2pyorhzqq.html

[U79] PHP：静态分析
来源：http://www.52xcode.cn/Article/details/gt2ickequup.html

composer require --dev phpstan/phpstan
来源：http://www.ydjk.org.cn/Article/details/gt2fjvzgxdj.html

[U80] PHP：代码规范修复
来源：http://www.ydjk.org.cn/Article/details/gt2laycsefh.html

composer require --dev friendsofphp/php-cs-fixer
来源：http://www.ydjk.org.cn/Article/details/gt2ytelfpxw.html

[U81] JS：初始化项目
来源：http://www.52xcode.cn/Article/details/gt2ckeaefzd.html

npm init -y;  npm i express
来源：http://www.52xcode.cn/Article/details/gt2kvhgrtcl.html

[U82] JS：package.json 脚本
来源：http://www.ydjk.org.cn/Article/details/gt2blehdazt.html

"scripts": { "dev": "vite", "build": "vite build" }
来源：http://www.52xcode.cn/Article/details/gt2pvaazljf.html

[U83] JS：ES Module 导入导出
来源：http://www.52xcode.cn/Article/details/gt2bomkdcpw.html

export const a = 1;  import { a } from "./m.js";
来源：http://www.ydjk.org.cn/Article/details/gt2dcliuvsz.html

[U84] JS：CommonJS 写法
来源：http://www.52xcode.cn/Article/details/gt2ggbhbbtg.html

module.exports = { a };  const { a } = require("./m");
来源：http://www.52xcode.cn/Article/details/gt2bxvrkwcv.html

[U85] JS：可选链
来源：http://www.ydjk.org.cn/Article/details/gt2hitcmqcs.html

a?.b?.c
来源：http://www.52xcode.cn/Article/details/gt2plukfdbb.html

[U86] JS：空值合并
来源：http://www.ydjk.org.cn/Article/details/gt2kqnmjijm.html

a ?? b
来源：http://www.52xcode.cn/Article/details/gt2hjuueiub.html

[U87] JS：解构默认值
来源：http://www.ydjk.org.cn/Article/details/gt2prqlzuxu.html

const { a = 1, b = 2 } = obj;
来源：http://www.ydjk.org.cn/Article/details/gt2ehfrkbul.html

[U88] JS：对象展开合并
来源：http://www.ydjk.org.cn/Article/details/gt2fsryyyqo.html

{ ...a, ...b }
来源：http://www.52xcode.cn/Article/details/gt2nnnwensl.html

[U89] JS：数组去重
来源：http://www.ydjk.org.cn/Article/details/gt2usfpzsnt.html

[...new Set(arr)]
来源：http://www.ydjk.org.cn/Article/details/gt2hvsuniai.html

[U90] JS：数字数组排序
来源：http://www.52xcode.cn/Article/details/gt2hhwffixx.html

[...arr].sort((a, b) => a - b)
来源：http://www.52xcode.cn/Article/details/gt2reeqgdrk.html

[U91] JS：对象键值遍历
来源：http://www.52xcode.cn/Article/details/gt2oaqrcfup.html

Object.entries(obj).forEach(([k, v]) => {});
来源：http://www.52xcode.cn/Article/details/gt2xsouqlof.html

[U92] JS：深拷贝
来源：http://www.52xcode.cn/Article/details/gt2mtdkwqwe.html

structuredClone(obj)
来源：http://www.ydjk.org.cn/Article/details/gt2jamyofpo.html


<!-- 参考信息 -->