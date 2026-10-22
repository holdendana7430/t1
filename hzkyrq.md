代发 wailian999

[T05] Kotlin：when 表达式
来源：http://www.ydjk.org.cn/Article/details/gt2pniauojc.html

val s = when (x) { 1 -> "一" else -> "其他" }   // 多分支时每个分支单独一行
来源：http://www.ydjk.org.cn/Article/details/gt2jvgldumg.html

[T06] Kotlin：集合映射
来源：http://www.ydjk.org.cn/Article/details/gt2hyzpaqxb.html

listOf(1, 2, 3).map { it * 2 }
来源：http://www.52xcode.cn/Article/details/gt2blrrgxct.html

[T07] Kotlin：集合过滤
来源：http://www.52xcode.cn/Article/details/gt2uonvnqdo.html

listOf(1, 2, 3).filter { it > 1 }
来源：http://www.ydjk.org.cn/Article/details/gt2ffvufhis.html

[T08] Kotlin：数据类
来源：http://www.52xcode.cn/Article/details/gt2qjkuhjya.html

data class User(val name: String, val age: Int)
来源：http://www.ydjk.org.cn/Article/details/gt2egyyyqht.html

[T09] Kotlin：扩展函数
来源：http://www.52xcode.cn/Article/details/gt2gptpzbql.html

fun String.exclaim() = this + "!"
来源：http://www.52xcode.cn/Article/details/gt2mrxfpxsz.html

[T10] Kotlin：默认参数
来源：http://www.52xcode.cn/Article/details/gt2jzxqmjit.html

fun greet(name: String = "World") = "Hi $name"
来源：http://www.52xcode.cn/Article/details/gt2qapjovhi.html

[T11] Kotlin：协程
来源：http://www.52xcode.cn/Article/details/gt2abvqemmk.html

GlobalScope.launch { delay(1000); println("done") }
来源：http://www.52xcode.cn/Article/details/gt2ktyijsnl.html

[T12] Kotlin：解构声明
来源：http://www.52xcode.cn/Article/details/gt2luofzsww.html

val (a, b) = Pair(1, 2)
来源：http://www.ydjk.org.cn/Article/details/gt2cvijdtjd.html

[T13] Kotlin：只读 Map
来源：http://www.ydjk.org.cn/Article/details/gt2uvusmvqr.html

val m = mapOf("a" to 1)
来源：http://www.52xcode.cn/Article/details/gt2guaqdhbl.html

[T14] Kotlin：循环
来源：http://www.52xcode.cn/Article/details/gt2fvudkqur.html

for (i in 1..10) println(i)
来源：http://www.52xcode.cn/Article/details/gt2dvoqrjqd.html

[T15] Kotlin：接口
来源：http://www.ydjk.org.cn/Article/details/gt2djhimtad.html

interface Shape { fun area(): Double }
来源：http://www.52xcode.cn/Article/details/gt2vomyhhzi.html

[T16] Swift：Hello World
来源：http://www.ydjk.org.cn/Article/details/gt2qebtgvoi.html

print("Hello")
来源：http://www.52xcode.cn/Article/details/gt2ffzremve.html

[T17] Swift：变量与常量
来源：http://www.52xcode.cn/Article/details/gt2heorhnag.html

var a = 1;  let b = 2
来源：http://www.ydjk.org.cn/Article/details/gt2iacbjwqu.html

[T18] Swift：字符串插值
来源：http://www.52xcode.cn/Article/details/gt2anabuwkk.html

"值: \(b)"
来源：http://www.52xcode.cn/Article/details/gt2libgosyv.html

[T19] Swift：可选绑定
来源：http://www.ydjk.org.cn/Article/details/gt2xiablaez.html

if let n = opt { print(n) }
来源：http://www.ydjk.org.cn/Article/details/gt2rjoorflk.html

[T20] Swift：数组操作
来源：http://www.52xcode.cn/Article/details/gt2nptgjyrk.html

var a = [1, 2, 3];  a.append(4)
来源：http://www.ydjk.org.cn/Article/details/gt2qjhkpxck.html

[T21] Swift：遍历
来源：http://www.52xcode.cn/Article/details/gt2ejltdauz.html

for x in a { print(x) }
来源：http://www.ydjk.org.cn/Article/details/gt2yhqxfgzh.html

[T22] Swift：字典
来源：http://www.ydjk.org.cn/Article/details/gt2mromvjpa.html

var d = ["a": 1];  d["b"] = 2
来源：http://www.ydjk.org.cn/Article/details/gt2idxbmhyc.html

[T23] Swift：函数
来源：http://www.52xcode.cn/Article/details/gt2hwopdxpp.html

func add(_ a: Int, _ b: Int) -> Int { a + b }
来源：http://www.ydjk.org.cn/Article/details/gt2xmkoptzn.html

[T24] Swift：闭包
来源：http://www.52xcode.cn/Article/details/gt2ybsictmo.html

let f = { (x: Int) -> Int in x * 2 }
来源：http://www.ydjk.org.cn/Article/details/gt2wpswxstc.html

[T25] Swift：结构体
来源：http://www.ydjk.org.cn/Article/details/gt2qsvnmceq.html

struct P { var x: Int }
来源：http://www.52xcode.cn/Article/details/gt2ammpccku.html

[T26] Swift：类与重写
来源：http://www.52xcode.cn/Article/details/gt2cmxfzuce.html

class A: Base { override func f() {} }
来源：http://www.52xcode.cn/Article/details/gt2ofpzxrrh.html

[T27] Swift：错误处理
来源：http://www.ydjk.org.cn/Article/details/gt2jvbacdfa.html

do { try f() } catch { print(error) }
来源：http://www.52xcode.cn/Article/details/gt2aoixtzhs.html

[T28] Swift：枚举
来源：http://www.52xcode.cn/Article/details/gt2nnvkzalf.html

enum Color { case red, green }
来源：http://www.ydjk.org.cn/Article/details/gt2kchcnidy.html

[T29] Swift：guard 提前返回
来源：http://www.ydjk.org.cn/Article/details/gt2obkkneth.html

guard let x = opt else { return }
来源：http://www.ydjk.org.cn/Article/details/gt2zbrsipse.html

[T30] Swift：协议
来源：http://www.52xcode.cn/Article/details/gt2cmicerdj.html

protocol Shape { func area() -> Double }
来源：http://www.52xcode.cn/Article/details/gt2eitiumke.html

[T31] Lua：Hello World
来源：http://www.52xcode.cn/Article/details/gt2nwlyjapq.html

print("Hello")
来源：http://www.ydjk.org.cn/Article/details/gt2gzoyupwp.html

[T32] Lua：局部变量
来源：http://www.ydjk.org.cn/Article/details/gt2ufhlluax.html

local a = 1
来源：http://www.52xcode.cn/Article/details/gt2pubrecks.html

[T33] Lua：表（数组）
来源：http://www.52xcode.cn/Article/details/gt2apmjwlcb.html

local t = {1, 2, 3};  t[4] = 4
来源：http://www.52xcode.cn/Article/details/gt2kwzpfzsw.html

[T34] Lua：遍历表
来源：http://www.ydjk.org.cn/Article/details/gt2ukpxjzsm.html

for i, v in ipairs(t) do print(i, v) end
来源：http://www.ydjk.org.cn/Article/details/gt2fxcenpnp.html

[T35] Lua：字典表
来源：http://www.ydjk.org.cn/Article/details/gt2ybqiigcu.html

local d = { a = 1 };  d.b = 2
来源：http://www.52xcode.cn/Article/details/gt2mbaixosg.html

[T36] Lua：函数
来源：http://www.52xcode.cn/Article/details/gt2ymoufviu.html

function add(a, b) return a + b end
来源：http://www.ydjk.org.cn/Article/details/gt2oklhbztv.html

[T37] Lua：字符串拼接
来源：http://www.52xcode.cn/Article/details/gt2kftgfxcd.html

"a" .. "b"
来源：http://www.ydjk.org.cn/Article/details/gt2iushgvum.html

[T38] Lua：条件
来源：http://www.52xcode.cn/Article/details/gt2kqyalxnt.html

if x > 0 then print("正") end
来源：http://www.ydjk.org.cn/Article/details/gt2prcionjb.html

[T39] Lua：模式匹配
来源：http://www.52xcode.cn/Article/details/gt2osqlcoou.html

string.find(s, "%d+")
来源：http://www.ydjk.org.cn/Article/details/gt2ioyrhrtj.html

[T40] Lua：元表
来源：http://www.ydjk.org.cn/Article/details/gt2vdkngykn.html

setmetatable({}, { __index = base })
来源：http://www.ydjk.org.cn/Article/details/gt2onbnsfsv.html

[T41] Perl：Hello World
来源：http://www.ydjk.org.cn/Article/details/gt2rmrkscrv.html

print "Hello\n";
来源：http://www.ydjk.org.cn/Article/details/gt2acltypcn.html

[T42] Perl：变量类型
来源：http://www.ydjk.org.cn/Article/details/gt2bmifqfwi.html

my $a = 1;  my @arr = (1, 2, 3);  my %h = (a => 1);
来源：http://www.52xcode.cn/Article/details/gt2gbyxymyt.html

[T43] Perl：字符串插值
来源：http://www.ydjk.org.cn/Article/details/gt2gydqmess.html

"值: $a"
来源：http://www.52xcode.cn/Article/details/gt2atieqhjq.html

[T44] Perl：条件
来源：http://www.52xcode.cn/Article/details/gt2oqnynzff.html

if ($a > 0) { print "正"; }
来源：http://www.ydjk.org.cn/Article/details/gt2zesinvcm.html

[T45] Perl：数组遍历
来源：http://www.52xcode.cn/Article/details/gt2kmctdeyh.html

for my $x (@arr) { print $x; }
来源：http://www.52xcode.cn/Article/details/gt2izenmfgu.html

[T46] Perl：哈希操作
来源：http://www.52xcode.cn/Article/details/gt2kufhzdyl.html

$h{b} = 2;  for my $k (keys %h) { print "$k=$h{$k}"; }
来源：http://www.52xcode.cn/Article/details/gt2praufxmn.html

[T47] Perl：正则捕获
来源：http://www.ydjk.org.cn/Article/details/gt2xuxyccbs.html

if ($s =~ /(\d+)/) { print $1; }
来源：http://www.ydjk.org.cn/Article/details/gt2sifaplja.html

[T48] Perl：正则替换
来源：http://www.ydjk.org.cn/Article/details/gt2heulbled.html

$s =~ s/old/new/g;
来源：http://www.52xcode.cn/Article/details/gt2rlzxuoeg.html

[T49] Perl：函数
来源：http://www.52xcode.cn/Article/details/gt2tpgyzjrm.html

sub add { my ($a, $b) = @_; return $a + $b; }
来源：http://www.52xcode.cn/Article/details/gt2jbgpoous.html

[T50] Perl：逐行读文件
来源：http://www.ydjk.org.cn/Article/details/gt2mspffhxk.html

open my $fh, "<", "a.txt" or die $!;
来源：http://www.ydjk.org.cn/Article/details/gt2mpwiwfpl.html

while (my $line = <$fh>) { print $line; }
来源：http://www.52xcode.cn/Article/details/gt2yoihiflu.html

[T51] Scala：Hello World
来源：http://www.ydjk.org.cn/Article/details/gt2uiypvwgw.html

println("Hello")
来源：http://www.52xcode.cn/Article/details/gt2yzpbteyj.html

[T52] Scala：变量
来源：http://www.52xcode.cn/Article/details/gt2nccuiskn.html

val a = 1;  var b = 2
来源：http://www.ydjk.org.cn/Article/details/gt2wzrmkskj.html

[T53] Scala：字符串插值
来源：http://www.52xcode.cn/Article/details/gt2wcitjibp.html

s"值: $b"
来源：http://www.ydjk.org.cn/Article/details/gt2tlhkcshx.html

[T54] Scala：集合映射
来源：http://www.52xcode.cn/Article/details/gt2affukiet.html

List(1, 2, 3).map(_ * 2)
来源：http://www.ydjk.org.cn/Article/details/gt2ixugviad.html

[T55] Scala：集合过滤
来源：http://www.52xcode.cn/Article/details/gt2gcydsxsv.html

List(1, 2, 3).filter(_ > 1)
来源：http://www.52xcode.cn/Article/details/gt2dbdjtvik.html

[T56] Scala：样例类
来源：http://www.52xcode.cn/Article/details/gt2pydqkwym.html

case class User(name: String, age: Int)
来源：http://www.ydjk.org.cn/Article/details/gt2bzeuqhtb.html

[T57] Scala：模式匹配
来源：http://www.ydjk.org.cn/Article/details/gt2khvyepax.html

x match { case 1 => "一"; case _ => "其他" }
来源：http://www.ydjk.org.cn/Article/details/gt2dajgdelv.html

[T58] Scala：函数定义
来源：http://www.ydjk.org.cn/Article/details/gt2kezegrvh.html

def add(a: Int, b: Int): Int = a + b
来源：http://www.52xcode.cn/Article/details/gt2gfrayaau.html

[T59] Scala：循环
来源：http://www.52xcode.cn/Article/details/gt2muxnkicy.html

for (i <- 1 to 10) println(i)
来源：http://www.ydjk.org.cn/Article/details/gt2mqaeqykn.html

[T60] Scala：折叠
来源：http://www.52xcode.cn/Article/details/gt2ubasgjrp.html

List(1, 2, 3).foldLeft(0)(_ + _)
来源：http://www.52xcode.cn/Article/details/gt2rzmhnwop.html

================================================================================
来源：http://www.ydjk.org.cn/Article/details/gt2cccnmjmc.html

U. 高频实用片段（Python / PHP / JavaScript 各 40 条）
来源：http://www.ydjk.org.cn/Article/details/gt2zcxvdpcn.html

================================================================================
来源：http://www.ydjk.org.cn/Article/details/gt2kenryhmw.html

[U01] Py：创建虚拟环境
来源：http://www.ydjk.org.cn/Article/details/gt2cdpyulso.html

python -m venv .venv && source .venv/bin/activate
来源：http://www.52xcode.cn/Article/details/gt2jamytlrv.html

[U02] Py：导出 / 安装依赖
来源：http://www.52xcode.cn/Article/details/gt2xgfcfsxt.html

pip freeze > requirements.txt;  pip install -r requirements.txt
来源：http://www.52xcode.cn/Article/details/gt2akujgjqw.html

[U03] Py：加载 .env 配置
来源：http://www.52xcode.cn/Article/details/gt2cshnecct.html

from dotenv import load_dotenv; load_dotenv()
来源：http://www.ydjk.org.cn/Article/details/gt2dekmgfpt.html

[U04] Py：变量调试打印
来源：http://www.52xcode.cn/Article/details/gt2zmydfsdp.html

print(f"{x=}")            # 输出 x=值，Python 3.8+
来源：http://www.ydjk.org.cn/Article/details/gt2fxlkrxsb.html

[U05] Py：列表去重且保序
来源：http://www.ydjk.org.cn/Article/details/gt2firkcjdx.html

list(dict.fromkeys(arr))
来源：http://www.52xcode.cn/Article/details/gt2tcjtnuvp.html

[U06] Py：合并两个字典
来源：http://www.ydjk.org.cn/Article/details/gt2qmlkvpex.html

{**a, **b}
来源：http://www.ydjk.org.cn/Article/details/gt2bagdpzwq.html

[U07] Py：反转字典键值
来源：http://www.52xcode.cn/Article/details/gt2cpkhkzun.html

{v: k for k, v in d.items()}
来源：http://www.52xcode.cn/Article/details/gt2cooyqmpj.html

[U08] Py：展平二维列表
来源：http://www.ydjk.org.cn/Article/details/gt2nqrdudyh.html

[y for x in nested for y in x]
来源：http://www.ydjk.org.cn/Article/details/gt2djyxjybn.html

[U09] Py：字典取最大值的键
来源：http://www.52xcode.cn/Article/details/gt2unrlwzxg.html

max(d, key=d.get)
来源：http://www.ydjk.org.cn/Article/details/gt2jqrxbcwx.html

[U10] Py：按值排序字典
来源：http://www.ydjk.org.cn/Article/details/gt2toftsfny.html

dict(sorted(d.items(), key=lambda kv: kv[1]))
来源：http://www.ydjk.org.cn/Article/details/gt2pdzmhqtu.html

[U11] Py：生成器表达式
来源：http://www.52xcode.cn/Article/details/gt2vrjjbhgx.html

(x * 2 for x in arr)
来源：http://www.52xcode.cn/Article/details/gt2yumylkzz.html

[U12] Py：取出现最多的 3 个元素
来源：http://www.52xcode.cn/Article/details/gt2mixtauuq.html

Counter(arr).most_common(3)
来源：http://www.52xcode.cn/Article/details/gt2ajbjmbbp.html

[U13] Py：固定长度队列
来源：http://www.52xcode.cn/Article/details/gt2wetcjmhs.html

deque(maxlen=10)
来源：http://www.52xcode.cn/Article/details/gt2tglcvkif.html

[U14] Py：分组收集到列表
来源：http://www.ydjk.org.cn/Article/details/gt2cvtjwhib.html

defaultdict(list)
来源：http://www.52xcode.cn/Article/details/gt2zrjbvmyw.html

[U15] Py：高精度计时
来源：http://www.52xcode.cn/Article/details/gt2kabisecm.html

t = time.perf_counter()
来源：http://www.ydjk.org.cn/Article/details/gt2mnaniosh.html

[U16] Py：命令行参数解析
来源：http://www.ydjk.org.cn/Article/details/gt2vaydhnzw.html

ap = argparse.ArgumentParser();  ap.add_argument("--name");  args = ap.parse_args()
来源：http://www.ydjk.org.cn/Article/details/gt2zonnklbj.html

[U17] Py：初始化日志
来源：http://www.ydjk.org.cn/Article/details/gt2esunndsb.html

logging.basicConfig(level=logging.INFO)
来源：http://www.52xcode.cn/Article/details/gt2ytdzfghe.html

[U18] Py：预编译正则
来源：http://www.ydjk.org.cn/Article/details/gt2xeakwnjz.html

pat = re.compile(r"\d+")
来源：http://www.52xcode.cn/Article/details/gt2icnopgbg.html

[U19] Py：正则替换带回调
来源：http://www.ydjk.org.cn/Article/details/gt2qgfqnygl.html

re.sub(r"\d+", lambda m: str(int(m.group()) * 2), s)
来源：http://www.ydjk.org.cn/Article/details/gt2opouvoum.html

[U20] Py：缓存函数结果
来源：http://www.ydjk.org.cn/Article/details/gt2jqssbbgf.html

@functools.lru_cache(maxsize=None)
来源：http://www.ydjk.org.cn/Article/details/gt2iouvarzj.html

[U21] Py：自定义上下文管理器
来源：http://www.52xcode.cn/Article/details/gt2okjodmih.html

@contextlib.contextmanager
来源：http://www.ydjk.org.cn/Article/details/gt2aubnajwu.html

[U22] Py：矩阵转置
来源：http://www.52xcode.cn/Article/details/gt2oxymeclk.html

list(zip(*m))
来源：http://www.ydjk.org.cn/Article/details/gt2umfgzeyv.html

[U23] Py：分块读取大文件
来源：http://www.ydjk.org.cn/Article/details/gt2bapxoawb.html

for chunk in iter(lambda: f.read(8192), b""):
来源：http://www.52xcode.cn/Article/details/gt2dgaazxhn.html

[U24] Py：路径操作
来源：http://www.52xcode.cn/Article/details/gt2fraqhecf.html

Path("a/b.txt").parent.mkdir(parents=True, exist_ok=True)
来源：http://www.ydjk.org.cn/Article/details/gt2wpekloor.html

[U25] Py：CSV 按字典读
来源：http://www.52xcode.cn/Article/details/gt2kqeiiabu.html

csv.DictReader(f)
来源：http://www.ydjk.org.cn/Article/details/gt2lzxehmif.html

[U26] Py：并发下载
来源：http://www.ydjk.org.cn/Article/details/gt2tehbjvlu.html

ThreadPoolExecutor(max_workers=8).map(fetch, urls)
来源：http://www.ydjk.org.cn/Article/details/gt2gdfmvbnk.html

[U27] Py：异步 HTTP
来源：http://www.ydjk.org.cn/Article/details/gt2stfacwzq.html

aiohttp.ClientSession() 配合 async with
来源：http://www.ydjk.org.cn/Article/details/gt2tkqljesl.html

[U28] Py：类型别名
来源：http://www.ydjk.org.cn/Article/details/gt2sywywqxe.html

UserId = int
来源：http://www.52xcode.cn/Article/details/gt2aozamejl.html

[U29] Py：属性校验
来源：http://www.ydjk.org.cn/Article/details/gt2fyrhqzay.html

@property 与 @x.setter 配合
来源：http://www.ydjk.org.cn/Article/details/gt2tzkrazzp.html

[U30] Py：数据类
来源：http://www.ydjk.org.cn/Article/details/gt2oxvooxbq.html

@dataclass(slots=True)
来源：http://www.52xcode.cn/Article/details/gt2secukupm.html

[U31] Py：单测
来源：http://www.ydjk.org.cn/Article/details/gt2xtosxpmc.html

python -m pytest -q
来源：http://www.52xcode.cn/Article/details/gt2xisrtykz.html

[U32] Py：代码格式化
来源：http://www.ydjk.org.cn/Article/details/gt2mjbazkdh.html

ruff format . && ruff check --fix .
来源：http://www.52xcode.cn/Article/details/gt2cdzfybkl.html

[U33] Py：打包发布
来源：http://www.ydjk.org.cn/Article/details/gt2sebvqzpg.html

python -m build  （依赖 pyproject.toml）
来源：http://www.ydjk.org.cn/Article/details/gt2zoxeywfc.html

[U34] Py：判断编码
来源：http://www.52xcode.cn/Article/details/gt2ysbyxnsv.html

chardet.detect(raw)
来源：http://www.52xcode.cn/Article/details/gt2cgwgrixj.html

[U35] Py：发送邮件
来源：http://www.ydjk.org.cn/Article/details/gt2jhouofxj.html

smtplib.SMTP_SSL(...).send_message(msg)
来源：http://www.ydjk.org.cn/Article/details/gt2nywdxoge.html

[U36] Py：定时任务
来源：http://www.ydjk.org.cn/Article/details/gt2vukyvzuq.html

schedule.every(10).minutes.do(job)
来源：http://www.ydjk.org.cn/Article/details/gt2ndhttzdw.html

[U37] Py：读写 Excel
来源：http://www.ydjk.org.cn/Article/details/gt2elmzdnmm.html

pandas.read_excel / DataFrame.to_excel
来源：http://www.52xcode.cn/Article/details/gt2qqfslhxm.html

[U38] Py：获取脚本所在目录
来源：http://www.52xcode.cn/Article/details/gt2tryaqtcq.html

Path(__file__).resolve().parent
来源：http://www.52xcode.cn/Article/details/gt2khfsxaxw.html

[U39] Py：判断是否在交互环境
来源：http://www.52xcode.cn/Article/details/gt2qsofhxjq.html

sys.stdout.isatty()
来源：http://www.52xcode.cn/Article/details/gt2juwfyvad.html

[U40] Py：打印到标准错误
来源：http://www.52xcode.cn/Article/details/gt2fkzqnrzr.html

print("err", file=sys.stderr)
来源：http://www.52xcode.cn/Article/details/gt2vitsgppb.html

[U41] PHP：初始化 Composer 项目
来源：http://www.52xcode.cn/Article/details/gt2kawcoqjd.html

composer init;  composer require guzzlehttp/guzzle
来源：http://www.52xcode.cn/Article/details/gt2kmwpuftt.html

[U42] PHP：PSR-4 自动加载
来源：http://www.52xcode.cn/Article/details/gt2powlyjjo.html

"autoload": { "psr-4": { "App\\": "src/" } }
来源：http://www.ydjk.org.cn/Article/details/gt2xqwagmsg.html

[U43] PHP：声明命名空间
来源：http://www.52xcode.cn/Article/details/gt2wckgxkhx.html

namespace App\Http;
来源：http://www.ydjk.org.cn/Article/details/gt2aopxauhh.html

[U44] PHP：开启严格类型
来源：http://www.52xcode.cn/Article/details/gt2eavqigkt.html

declare(strict_types=1);
来源：http://www.ydjk.org.cn/Article/details/gt2odkkjanl.html

[U45] PHP：类型声明与返回类型
来源：http://www.52xcode.cn/Article/details/gt2ekjfizwc.html

function add(int $a, int $b): int { return $a + $b; }
来源：http://www.ydjk.org.cn/Article/details/gt2jocwupyg.html

[U46] PHP：可空类型
来源：http://www.52xcode.cn/Article/details/gt2lfvbtpyd.html

?string $name = null
来源：http://www.52xcode.cn/Article/details/gt2telvlfhx.html

[U47] PHP：联合类型
来源：http://www.52xcode.cn/Article/details/gt2nfvnuifq.html

int|string $id
来源：http://www.ydjk.org.cn/Article/details/gt2aulljtki.html

[U48] PHP：纯枚举
来源：http://www.ydjk.org.cn/Article/details/gt2hdqxjdaz.html

enum Status: string { case Active = "active"; case Off = "off"; }
来源：http://www.ydjk.org.cn/Article/details/gt2fwgphist.html

[U49] PHP：只读属性
来源：http://www.ydjk.org.cn/Article/details/gt2mftmsepq.html

public readonly string $name
来源：http://www.ydjk.org.cn/Article/details/gt2jdslmibv.html

[U50] PHP：构造器属性提升
来源：http://www.ydjk.org.cn/Article/details/gt2jrjahipg.html

public function __construct(private int $id) {}
来源：http://www.52xcode.cn/Article/details/gt2ioagkyve.html

[U51] PHP：数组解构
来源：http://www.ydjk.org.cn/Article/details/gt2avbrgmnq.html

[$a, $b] = $arr;
来源：http://www.ydjk.org.cn/Article/details/gt2eyttmrkk.html

[U52] PHP：箭头函数
来源：http://www.52xcode.cn/Article/details/gt2gmtmlbxj.html

$double = fn($x) => $x * 2;
来源：http://www.52xcode.cn/Article/details/gt2hipbttuc.html

[U53] PHP：空合并运算符
来源：http://www.ydjk.org.cn/Article/details/gt2vnepybso.html

$v = $a ?? $b ?? "default";
来源：http://www.52xcode.cn/Article/details/gt2wbfeuhdc.html

[U54] PHP：空安全调用
来源：http://www.ydjk.org.cn/Article/details/gt2ehovgavx.html

$obj?->method()
来源：http://www.ydjk.org.cn/Article/details/gt2ccmhwcky.html

[U55] PHP：match 表达式
来源：http://www.ydjk.org.cn/Article/details/gt2mzqkgvgw.html

$s = match($x) { 1 => "一", default => "其他" };
来源：http://www.52xcode.cn/Article/details/gt2oqvqdnua.html

[U56] PHP：命名参数
来源：http://www.ydjk.org.cn/Article/details/gt2tsglcfea.html

f(a: 1, b: 2)
来源：http://www.52xcode.cn/Article/details/gt2vxrrbxqe.html

[U57] PHP：字符串插值
来源：http://www.ydjk.org.cn/Article/details/gt2tfovubmy.html

"值: {$a}"
来源：http://www.ydjk.org.cn/Article/details/gt2geibfrej.html

[U58] PHP：数组三件套
来源：http://www.ydjk.org.cn/Article/details/gt2cexkkrth.html

array_map($f, $a);  array_filter($a, $f);  array_reduce($a, $f, 0);
来源：http://www.52xcode.cn/Article/details/gt2lamzrpok.html

[U59] PHP：自定义排序
来源：http://www.52xcode.cn/Article/details/gt2guuljmia.html

usort($arr, fn($a, $b) => $a["age"] <=> $b["age"]);
来源：http://www.ydjk.org.cn/Article/details/gt2ksxccjuj.html

[U60] PHP：JSON 编解码
来源：http://www.ydjk.org.cn/Article/details/gt2dmugjflc.html

json_encode($d, JSON_UNESCAPED_UNICODE);  json_decode($s, true);
来源：http://www.ydjk.org.cn/Article/details/gt2zbedrkwc.html

[U61] PHP：正则
来源：http://www.52xcode.cn/Article/details/gt2admtqcos.html

preg_match('/(\d+)/', $s, $m);  preg_replace('/\d+/', '#', $s);
来源：http://www.ydjk.org.cn/Article/details/gt2wrjjeqju.html

[U62] PHP：日期对象
来源：http://www.ydjk.org.cn/Article/details/gt2lcxkevzx.html

(new DateTimeImmutable())->format("Y-m-d");
来源：http://www.ydjk.org.cn/Article/details/gt2ccziblcr.html

[U63] PHP：文件读写
来源：http://www.ydjk.org.cn/Article/details/gt2kbpctkfc.html

file_get_contents($f);  file_put_contents($f, $data);
来源：http://www.ydjk.org.cn/Article/details/gt2jvbjjdig.html

[U64] PHP：目录遍历
来源：http://www.ydjk.org.cn/Article/details/gt2akoifosb.html

glob("dir/*.php");  scandir("dir");
来源：http://www.52xcode.cn/Article/details/gt2gxxnfiut.html

[U65] PHP：会话
来源：http://www.ydjk.org.cn/Article/details/gt2zvluqwnw.html

session_start();  $_SESSION["uid"] = 1;
来源：http://www.ydjk.org.cn/Article/details/gt2qyiotovy.html

[U66] PHP：设置 Cookie
来源：http://www.ydjk.org.cn/Article/details/gt2ejmenxnf.html

setcookie("token", $v, ["httponly" => true, "samesite" => "Lax"]);
来源：http://www.ydjk.org.cn/Article/details/gt2rdieibfx.html

[U67] PHP：处理文件上传
来源：http://www.ydjk.org.cn/Article/details/gt2ffgdgcdo.html

$_FILES["file"]["tmp_name"] 与 move_uploaded_file()
来源：http://www.52xcode.cn/Article/details/gt2vjvygwgo.html

[U68] PHP：PDO 连接
来源：http://www.ydjk.org.cn/Article/details/gt2elpexfmh.html

$pdo = new PDO("mysql:host=localhost;dbname=app", "root", "");
来源：http://www.ydjk.org.cn/Article/details/gt2zsdlsrzl.html

[U69] PHP：PDO 预处理
来源：http://www.52xcode.cn/Article/details/gt2ykdqdxpg.html

$stmt = $pdo->prepare("SELECT * FROM users WHERE id = ?");  $stmt->execute([$id]);
来源：http://www.52xcode.cn/Article/details/gt2bwayhvkz.html

[U70] PHP：PDO 事务
来源：http://www.52xcode.cn/Article/details/gt2hqheidbr.html

$pdo->beginTransaction();  $pdo->commit();  $pdo->rollBack();
来源：http://www.ydjk.org.cn/Article/details/gt2lrmwkoiz.html

[U71] PHP：抛出异常
来源：http://www.ydjk.org.cn/Article/details/gt2ctuimlgm.html

throw new RuntimeException("失败", 500);
来源：http://www.ydjk.org.cn/Article/details/gt2vzdgqkpb.html

[U72] PHP：写错误日志
来源：http://www.52xcode.cn/Article/details/gt2yulkauys.html

error_log("失败: " . $e->getMessage());
来源：http://www.ydjk.org.cn/Article/details/gt2nkcssesg.html

[U73] PHP：读取 ini 配置
来源：http://www.ydjk.org.cn/Article/details/gt2zcjtjjmv.html

parse_ini_file("config.ini", true)
来源：http://www.ydjk.org.cn/Article/details/gt2yfaceakk.html

[U74] PHP：读取环境变量
来源：http://www.52xcode.cn/Article/details/gt2qttgewcv.html

getenv("APP_ENV") ?: "production"
来源：http://www.52xcode.cn/Article/details/gt2vrqkpktb.html

[U75] PHP：依赖注入
来源：http://www.52xcode.cn/Article/details/gt2eqiufmyv.html

composer require psr/container
来源：http://www.52xcode.cn/Article/details/gt2souyoxam.html

[U76] PHP：简单路由
来源：http://www.ydjk.org.cn/Article/details/gt2trrmnqul.html

$path = parse_url($_SERVER["REQUEST_URI"], PHP_URL_PATH);
来源：http://www.52xcode.cn/Article/details/gt2lqqhjiup.html

[U77] PHP：模板渲染
来源：http://www.ydjk.org.cn/Article/details/gt2eridxwiu.html

composer require twig/twig
来源：http://www.52xcode.cn/Article/details/gt2rfdrxxei.html

[U78] PHP：单元测试
来源：http://www.ydjk.org.cn/Article/details/gt2fzzglgeu.html

composer require --dev phpunit/phpunit
来源：http://www.ydjk.org.cn/Article/details/gt2sjgivcca.html

[U79] PHP：静态分析
来源：http://www.ydjk.org.cn/Article/details/gt2xkouipmo.html

composer require --dev phpstan/phpstan
来源：http://www.ydjk.org.cn/Article/details/gt2fuijhxwm.html

[U80] PHP：代码规范修复
来源：http://www.ydjk.org.cn/Article/details/gt2zmwjklpa.html

composer require --dev friendsofphp/php-cs-fixer
来源：http://www.52xcode.cn/Article/details/gt2xvudchou.html

[U81] JS：初始化项目
来源：http://www.ydjk.org.cn/Article/details/gt2okbhcfpd.html

npm init -y;  npm i express
来源：http://www.ydjk.org.cn/Article/details/gt2xdyfvdqq.html

[U82] JS：package.json 脚本
来源：http://www.52xcode.cn/Article/details/gt2vfrqjjad.html

"scripts": { "dev": "vite", "build": "vite build" }
来源：http://www.ydjk.org.cn/Article/details/gt2ecuxvwnv.html

[U83] JS：ES Module 导入导出
来源：http://www.52xcode.cn/Article/details/gt2tkdtsczd.html

export const a = 1;  import { a } from "./m.js";
来源：http://www.52xcode.cn/Article/details/gt2zsxqwvrl.html

[U84] JS：CommonJS 写法
来源：http://www.52xcode.cn/Article/details/gt2csvhftdu.html

module.exports = { a };  const { a } = require("./m");
来源：http://www.52xcode.cn/Article/details/gt2ylajvlvi.html

[U85] JS：可选链
来源：http://www.52xcode.cn/Article/details/gt2cbeqgpnu.html

a?.b?.c
来源：http://www.ydjk.org.cn/Article/details/gt2hriazsbp.html

[U86] JS：空值合并
来源：http://www.ydjk.org.cn/Article/details/gt2kxklzpuf.html

a ?? b
来源：http://www.ydjk.org.cn/Article/details/gt2lwlrvkud.html

[U87] JS：解构默认值
来源：http://www.52xcode.cn/Article/details/gt2wkeurxvc.html

const { a = 1, b = 2 } = obj;
来源：http://www.52xcode.cn/Article/details/gt2luwtccnh.html

[U88] JS：对象展开合并
来源：http://www.52xcode.cn/Article/details/gt2ykygolar.html

{ ...a, ...b }
来源：http://www.52xcode.cn/Article/details/gt2ywmqrpza.html

[U89] JS：数组去重
来源：http://www.ydjk.org.cn/Article/details/gt2fgcmowlb.html

[...new Set(arr)]
来源：http://www.ydjk.org.cn/Article/details/gt2rxbzlsxp.html

[U90] JS：数字数组排序
来源：http://www.52xcode.cn/Article/details/gt2czcxarxu.html

[...arr].sort((a, b) => a - b)
来源：http://www.52xcode.cn/Article/details/gt2icbshhbd.html

[U91] JS：对象键值遍历
来源：http://www.52xcode.cn/Article/details/gt2yvtkpbog.html

Object.entries(obj).forEach(([k, v]) => {});
来源：http://www.ydjk.org.cn/Article/details/gt2vejobndi.html

[U92] JS：深拷贝
来源：http://www.52xcode.cn/Article/details/gt2uzhivmmb.html

structuredClone(obj)
来源：http://www.52xcode.cn/Article/details/gt2kkaavmsj.html


<!-- 参考信息 -->