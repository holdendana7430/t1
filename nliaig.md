代发 wailian999

[T01] Kotlin：Hello World
来源：http://www.ydjk.org.cn/Article/details/gt2ekdgpewo.html

println("Hello")
来源：http://www.52xcode.cn/Article/details/gt2kkxzienh.html

[T02] Kotlin：变量
来源：http://www.ydjk.org.cn/Article/details/gt2mnujmzmz.html

val a = 1;  var b = 2        // val 只读，var 可变
来源：http://www.ydjk.org.cn/Article/details/gt2lbqijinj.html

[T03] Kotlin：字符串模板
来源：http://www.ydjk.org.cn/Article/details/gt2ymvwerzl.html

"值: $b"
来源：http://www.52xcode.cn/Article/details/gt2ujinyvep.html

[T04] Kotlin：空安全
来源：http://www.ydjk.org.cn/Article/details/gt2jymnkrvd.html

val n: String? = null;  n?.length
来源：http://www.ydjk.org.cn/Article/details/gt2djewcfux.html

[T05] Kotlin：when 表达式
来源：http://www.ydjk.org.cn/Article/details/gt2mrspohvg.html

val s = when (x) { 1 -> "一" else -> "其他" }   // 多分支时每个分支单独一行
来源：http://www.52xcode.cn/Article/details/gt2wryptlja.html

[T06] Kotlin：集合映射
来源：http://www.ydjk.org.cn/Article/details/gt2uosuojef.html

listOf(1, 2, 3).map { it * 2 }
来源：http://www.ydjk.org.cn/Article/details/gt2quktgnae.html

[T07] Kotlin：集合过滤
来源：http://www.ydjk.org.cn/Article/details/gt2gyasyqro.html

listOf(1, 2, 3).filter { it > 1 }
来源：http://www.52xcode.cn/Article/details/gt2rukumeeq.html

[T08] Kotlin：数据类
来源：http://www.ydjk.org.cn/Article/details/gt2wdcrkvnf.html

data class User(val name: String, val age: Int)
来源：http://www.52xcode.cn/Article/details/gt2ptigztgx.html

[T09] Kotlin：扩展函数
来源：http://www.ydjk.org.cn/Article/details/gt2supwvmwf.html

fun String.exclaim() = this + "!"
来源：http://www.ydjk.org.cn/Article/details/gt2hnqlnstr.html

[T10] Kotlin：默认参数
来源：http://www.ydjk.org.cn/Article/details/gt2fdptmxdj.html

fun greet(name: String = "World") = "Hi $name"
来源：http://www.ydjk.org.cn/Article/details/gt2whxdnolf.html

[T11] Kotlin：协程
来源：http://www.52xcode.cn/Article/details/gt2kpkotbjx.html

GlobalScope.launch { delay(1000); println("done") }
来源：http://www.52xcode.cn/Article/details/gt2hezoajap.html

[T12] Kotlin：解构声明
来源：http://www.ydjk.org.cn/Article/details/gt2pvnmnlbq.html

val (a, b) = Pair(1, 2)
来源：http://www.52xcode.cn/Article/details/gt2nxndhbog.html

[T13] Kotlin：只读 Map
来源：http://www.ydjk.org.cn/Article/details/gt2prnyqsyf.html

val m = mapOf("a" to 1)
来源：http://www.52xcode.cn/Article/details/gt2tqpxwtoa.html

[T14] Kotlin：循环
来源：http://www.52xcode.cn/Article/details/gt2ugvnmxsj.html

for (i in 1..10) println(i)
来源：http://www.52xcode.cn/Article/details/gt2negionqn.html

[T15] Kotlin：接口
来源：http://www.ydjk.org.cn/Article/details/gt2vpzkxgln.html

interface Shape { fun area(): Double }
来源：http://www.ydjk.org.cn/Article/details/gt2hziddygz.html

[T16] Swift：Hello World
来源：http://www.52xcode.cn/Article/details/gt2walryeia.html

print("Hello")
来源：http://www.ydjk.org.cn/Article/details/gt2qlgnegxh.html

[T17] Swift：变量与常量
来源：http://www.ydjk.org.cn/Article/details/gt2uinasljo.html

var a = 1;  let b = 2
来源：http://www.ydjk.org.cn/Article/details/gt2zfrcgofb.html

[T18] Swift：字符串插值
来源：http://www.ydjk.org.cn/Article/details/gt2mawokibs.html

"值: \(b)"
来源：http://www.ydjk.org.cn/Article/details/gt2bqcnsqkd.html

[T19] Swift：可选绑定
来源：http://www.ydjk.org.cn/Article/details/gt2ntkdutul.html

if let n = opt { print(n) }
来源：http://www.ydjk.org.cn/Article/details/gt2grkepowy.html

[T20] Swift：数组操作
来源：http://www.ydjk.org.cn/Article/details/gt2gwpufyyj.html

var a = [1, 2, 3];  a.append(4)
来源：http://www.52xcode.cn/Article/details/gt2uwnwhedz.html

[T21] Swift：遍历
来源：http://www.52xcode.cn/Article/details/gt2jslnqrpe.html

for x in a { print(x) }
来源：http://www.ydjk.org.cn/Article/details/gt2dyfdmnaz.html

[T22] Swift：字典
来源：http://www.ydjk.org.cn/Article/details/gt2gqtaqqcj.html

var d = ["a": 1];  d["b"] = 2
来源：http://www.52xcode.cn/Article/details/gt2ljmtqbnv.html

[T23] Swift：函数
来源：http://www.ydjk.org.cn/Article/details/gt2xvwgysqb.html

func add(_ a: Int, _ b: Int) -> Int { a + b }
来源：http://www.52xcode.cn/Article/details/gt2qhthherk.html

[T24] Swift：闭包
来源：http://www.ydjk.org.cn/Article/details/gt2ctenkngv.html

let f = { (x: Int) -> Int in x * 2 }
来源：http://www.ydjk.org.cn/Article/details/gt2nicmgkrz.html

[T25] Swift：结构体
来源：http://www.ydjk.org.cn/Article/details/gt2nqtbgysh.html

struct P { var x: Int }
来源：http://www.ydjk.org.cn/Article/details/gt2cxktmmik.html

[T26] Swift：类与重写
来源：http://www.52xcode.cn/Article/details/gt2ulkwhjvh.html

class A: Base { override func f() {} }
来源：http://www.52xcode.cn/Article/details/gt2uyawydoc.html

[T27] Swift：错误处理
来源：http://www.52xcode.cn/Article/details/gt2okhppkks.html

do { try f() } catch { print(error) }
来源：http://www.ydjk.org.cn/Article/details/gt2jjahqsyw.html

[T28] Swift：枚举
来源：http://www.ydjk.org.cn/Article/details/gt2plkczjsp.html

enum Color { case red, green }
来源：http://www.52xcode.cn/Article/details/gt2cunsgiff.html

[T29] Swift：guard 提前返回
来源：http://www.52xcode.cn/Article/details/gt2bainmzdj.html

guard let x = opt else { return }
来源：http://www.ydjk.org.cn/Article/details/gt2brnlumcq.html

[T30] Swift：协议
来源：http://www.52xcode.cn/Article/details/gt2yqbdwwoo.html

protocol Shape { func area() -> Double }
来源：http://www.52xcode.cn/Article/details/gt2kzgaykmr.html

[T31] Lua：Hello World
来源：http://www.52xcode.cn/Article/details/gt2ftdggdil.html

print("Hello")
来源：http://www.52xcode.cn/Article/details/gt2wwzehmxe.html

[T32] Lua：局部变量
来源：http://www.52xcode.cn/Article/details/gt2brimgeuv.html

local a = 1
来源：http://www.ydjk.org.cn/Article/details/gt2rxmbusvc.html

[T33] Lua：表（数组）
来源：http://www.ydjk.org.cn/Article/details/gt2urmiabcf.html

local t = {1, 2, 3};  t[4] = 4
来源：http://www.ydjk.org.cn/Article/details/gt2grptnkmp.html

[T34] Lua：遍历表
来源：http://www.52xcode.cn/Article/details/gt2tbuejrkf.html

for i, v in ipairs(t) do print(i, v) end
来源：http://www.52xcode.cn/Article/details/gt2pmbwjfhk.html

[T35] Lua：字典表
来源：http://www.52xcode.cn/Article/details/gt2gwpnbltf.html

local d = { a = 1 };  d.b = 2
来源：http://www.ydjk.org.cn/Article/details/gt2owcimdph.html

[T36] Lua：函数
来源：http://www.52xcode.cn/Article/details/gt2kvhwfonv.html

function add(a, b) return a + b end
来源：http://www.ydjk.org.cn/Article/details/gt2crlfewrd.html

[T37] Lua：字符串拼接
来源：http://www.ydjk.org.cn/Article/details/gt2qgsqzdcj.html

"a" .. "b"
来源：http://www.ydjk.org.cn/Article/details/gt2uytdwaxb.html

[T38] Lua：条件
来源：http://www.52xcode.cn/Article/details/gt2sxgpgwgf.html

if x > 0 then print("正") end
来源：http://www.52xcode.cn/Article/details/gt2krneeplq.html

[T39] Lua：模式匹配
来源：http://www.52xcode.cn/Article/details/gt2vyapyceg.html

string.find(s, "%d+")
来源：http://www.52xcode.cn/Article/details/gt2dkvwmpeo.html

[T40] Lua：元表
来源：http://www.ydjk.org.cn/Article/details/gt2nbtprlch.html

setmetatable({}, { __index = base })
来源：http://www.52xcode.cn/Article/details/gt2guucatbv.html

[T41] Perl：Hello World
来源：http://www.ydjk.org.cn/Article/details/gt2hyrbugcm.html

print "Hello\n";
来源：http://www.ydjk.org.cn/Article/details/gt2qenkigvk.html

[T42] Perl：变量类型
来源：http://www.ydjk.org.cn/Article/details/gt2tfsndxgz.html

my $a = 1;  my @arr = (1, 2, 3);  my %h = (a => 1);
来源：http://www.ydjk.org.cn/Article/details/gt2ezkjfxva.html

[T43] Perl：字符串插值
来源：http://www.52xcode.cn/Article/details/gt2ubwivuxe.html

"值: $a"
来源：http://www.52xcode.cn/Article/details/gt2bwrdmfxl.html

[T44] Perl：条件
来源：http://www.ydjk.org.cn/Article/details/gt2mnewjwci.html

if ($a > 0) { print "正"; }
来源：http://www.52xcode.cn/Article/details/gt2pmmzmghj.html

[T45] Perl：数组遍历
来源：http://www.ydjk.org.cn/Article/details/gt2ohoqqiel.html

for my $x (@arr) { print $x; }
来源：http://www.52xcode.cn/Article/details/gt2nsmgxlwg.html

[T46] Perl：哈希操作
来源：http://www.52xcode.cn/Article/details/gt2zkbnfhkd.html

$h{b} = 2;  for my $k (keys %h) { print "$k=$h{$k}"; }
来源：http://www.52xcode.cn/Article/details/gt2glmwoevf.html

[T47] Perl：正则捕获
来源：http://www.52xcode.cn/Article/details/gt2lmcjfhjq.html

if ($s =~ /(\d+)/) { print $1; }
来源：http://www.ydjk.org.cn/Article/details/gt2eafbpqde.html

[T48] Perl：正则替换
来源：http://www.ydjk.org.cn/Article/details/gt2rnydstmj.html

$s =~ s/old/new/g;
来源：http://www.ydjk.org.cn/Article/details/gt2lbekhpvw.html

[T49] Perl：函数
来源：http://www.ydjk.org.cn/Article/details/gt2slxhntup.html

sub add { my ($a, $b) = @_; return $a + $b; }
来源：http://www.ydjk.org.cn/Article/details/gt2kirrooxx.html

[T50] Perl：逐行读文件
来源：http://www.52xcode.cn/Article/details/gt2srqtawfa.html

open my $fh, "<", "a.txt" or die $!;
来源：http://www.52xcode.cn/Article/details/gt2yrgcwwzc.html

while (my $line = <$fh>) { print $line; }
来源：http://www.52xcode.cn/Article/details/gt2moscwdpy.html

[T51] Scala：Hello World
来源：http://www.52xcode.cn/Article/details/gt2cdtmvpjd.html

println("Hello")
来源：http://www.52xcode.cn/Article/details/gt2mwvgaubt.html

[T52] Scala：变量
来源：http://www.52xcode.cn/Article/details/gt2pftsqisk.html

val a = 1;  var b = 2
来源：http://www.ydjk.org.cn/Article/details/gt2npulswsz.html

[T53] Scala：字符串插值
来源：http://www.52xcode.cn/Article/details/gt2rqqueuoo.html

s"值: $b"
来源：http://www.ydjk.org.cn/Article/details/gt2xeosgdua.html

[T54] Scala：集合映射
来源：http://www.52xcode.cn/Article/details/gt2ovpwocjt.html

List(1, 2, 3).map(_ * 2)
来源：http://www.ydjk.org.cn/Article/details/gt2qpfarnxy.html

[T55] Scala：集合过滤
来源：http://www.52xcode.cn/Article/details/gt2dquiqrbq.html

List(1, 2, 3).filter(_ > 1)
来源：http://www.52xcode.cn/Article/details/gt2zpywblsd.html

[T56] Scala：样例类
来源：http://www.ydjk.org.cn/Article/details/gt2brrgvrps.html

case class User(name: String, age: Int)
来源：http://www.52xcode.cn/Article/details/gt2curslihf.html

[T57] Scala：模式匹配
来源：http://www.52xcode.cn/Article/details/gt2hcmdkrkj.html

x match { case 1 => "一"; case _ => "其他" }
来源：http://www.ydjk.org.cn/Article/details/gt2uhzmfcqj.html

[T58] Scala：函数定义
来源：http://www.52xcode.cn/Article/details/gt2feuwubkj.html

def add(a: Int, b: Int): Int = a + b
来源：http://www.ydjk.org.cn/Article/details/gt2dmfqlbui.html

[T59] Scala：循环
来源：http://www.52xcode.cn/Article/details/gt2iwjowjpu.html

for (i <- 1 to 10) println(i)
来源：http://www.52xcode.cn/Article/details/gt2fhpwdidh.html

[T60] Scala：折叠
来源：http://www.ydjk.org.cn/Article/details/gt2ebwxbouo.html

List(1, 2, 3).foldLeft(0)(_ + _)
来源：http://www.52xcode.cn/Article/details/gt2xekugojc.html

================================================================================
来源：http://www.52xcode.cn/Article/details/gt2jkttghpx.html

U. 高频实用片段（Python / PHP / JavaScript 各 40 条）
来源：http://www.52xcode.cn/Article/details/gt2ylgquqms.html

================================================================================
来源：http://www.ydjk.org.cn/Article/details/gt2caddepsw.html

[U01] Py：创建虚拟环境
来源：http://www.52xcode.cn/Article/details/gt2rykkvacd.html

python -m venv .venv && source .venv/bin/activate
来源：http://www.52xcode.cn/Article/details/gt2nxnrknmm.html

[U02] Py：导出 / 安装依赖
来源：http://www.52xcode.cn/Article/details/gt2oskurjmf.html

pip freeze > requirements.txt;  pip install -r requirements.txt
来源：http://www.52xcode.cn/Article/details/gt2xwdligrz.html

[U03] Py：加载 .env 配置
来源：http://www.52xcode.cn/Article/details/gt2cyljeztp.html

from dotenv import load_dotenv; load_dotenv()
来源：http://www.ydjk.org.cn/Article/details/gt2atotuebw.html

[U04] Py：变量调试打印
来源：http://www.ydjk.org.cn/Article/details/gt2hkfjtaqa.html

print(f"{x=}")            # 输出 x=值，Python 3.8+
来源：http://www.ydjk.org.cn/Article/details/gt2wdkbdlop.html

[U05] Py：列表去重且保序
来源：http://www.ydjk.org.cn/Article/details/gt2hmjpdjdr.html

list(dict.fromkeys(arr))
来源：http://www.ydjk.org.cn/Article/details/gt2viaitcbv.html

[U06] Py：合并两个字典
来源：http://www.ydjk.org.cn/Article/details/gt2diumbedk.html

{**a, **b}
来源：http://www.ydjk.org.cn/Article/details/gt2xnporpuj.html

[U07] Py：反转字典键值
来源：http://www.ydjk.org.cn/Article/details/gt2begarwzt.html

{v: k for k, v in d.items()}
来源：http://www.ydjk.org.cn/Article/details/gt2quizakqk.html

[U08] Py：展平二维列表
来源：http://www.ydjk.org.cn/Article/details/gt2husipsfq.html

[y for x in nested for y in x]
来源：http://www.52xcode.cn/Article/details/gt2tjhlplji.html

[U09] Py：字典取最大值的键
来源：http://www.ydjk.org.cn/Article/details/gt2uvvfuedk.html

max(d, key=d.get)
来源：http://www.ydjk.org.cn/Article/details/gt2xhejfomt.html

[U10] Py：按值排序字典
来源：http://www.ydjk.org.cn/Article/details/gt2gdggvmhz.html

dict(sorted(d.items(), key=lambda kv: kv[1]))
来源：http://www.ydjk.org.cn/Article/details/gt2fycpjvev.html

[U11] Py：生成器表达式
来源：http://www.ydjk.org.cn/Article/details/gt2mmqovuwq.html

(x * 2 for x in arr)
来源：http://www.52xcode.cn/Article/details/gt2dqqyprjs.html

[U12] Py：取出现最多的 3 个元素
来源：http://www.ydjk.org.cn/Article/details/gt2ymudvfyc.html

Counter(arr).most_common(3)
来源：http://www.ydjk.org.cn/Article/details/gt2jollvdax.html

[U13] Py：固定长度队列
来源：http://www.ydjk.org.cn/Article/details/gt2gnhncdkg.html

deque(maxlen=10)
来源：http://www.ydjk.org.cn/Article/details/gt2hmsrcxbi.html

[U14] Py：分组收集到列表
来源：http://www.ydjk.org.cn/Article/details/gt2cuzbljfp.html

defaultdict(list)
来源：http://www.ydjk.org.cn/Article/details/gt2eznxfdvl.html

[U15] Py：高精度计时
来源：http://www.ydjk.org.cn/Article/details/gt2cehuvmzo.html

t = time.perf_counter()
来源：http://www.ydjk.org.cn/Article/details/gt2ubouovgs.html

[U16] Py：命令行参数解析
来源：http://www.52xcode.cn/Article/details/gt2tlvdwjfs.html

ap = argparse.ArgumentParser();  ap.add_argument("--name");  args = ap.parse_args()
来源：http://www.ydjk.org.cn/Article/details/gt2bqwcvqqb.html

[U17] Py：初始化日志
来源：http://www.52xcode.cn/Article/details/gt2sufiwmxl.html

logging.basicConfig(level=logging.INFO)
来源：http://www.ydjk.org.cn/Article/details/gt2wvykofgv.html

[U18] Py：预编译正则
来源：http://www.ydjk.org.cn/Article/details/gt2fdpoojsk.html

pat = re.compile(r"\d+")
来源：http://www.52xcode.cn/Article/details/gt2elauxgdf.html

[U19] Py：正则替换带回调
来源：http://www.52xcode.cn/Article/details/gt2ueundynf.html

re.sub(r"\d+", lambda m: str(int(m.group()) * 2), s)
来源：http://www.52xcode.cn/Article/details/gt2wqbgqmrt.html

[U20] Py：缓存函数结果
来源：http://www.52xcode.cn/Article/details/gt2abfljgjb.html

@functools.lru_cache(maxsize=None)
来源：http://www.52xcode.cn/Article/details/gt2dusnjree.html

[U21] Py：自定义上下文管理器
来源：http://www.52xcode.cn/Article/details/gt2llbhtihu.html

@contextlib.contextmanager
来源：http://www.ydjk.org.cn/Article/details/gt2ujcmllvd.html

[U22] Py：矩阵转置
来源：http://www.ydjk.org.cn/Article/details/gt2xztxfiwy.html

list(zip(*m))
来源：http://www.ydjk.org.cn/Article/details/gt2iewxpjmw.html

[U23] Py：分块读取大文件
来源：http://www.52xcode.cn/Article/details/gt2pentudkk.html

for chunk in iter(lambda: f.read(8192), b""):
来源：http://www.ydjk.org.cn/Article/details/gt2xpjuicjq.html

[U24] Py：路径操作
来源：http://www.ydjk.org.cn/Article/details/gt2kcfxnflv.html

Path("a/b.txt").parent.mkdir(parents=True, exist_ok=True)
来源：http://www.ydjk.org.cn/Article/details/gt2eqwijkiy.html

[U25] Py：CSV 按字典读
来源：http://www.ydjk.org.cn/Article/details/gt2bulbyvwq.html

csv.DictReader(f)
来源：http://www.ydjk.org.cn/Article/details/gt2kkivnjvr.html

[U26] Py：并发下载
来源：http://www.52xcode.cn/Article/details/gt2mchcygip.html

ThreadPoolExecutor(max_workers=8).map(fetch, urls)
来源：http://www.52xcode.cn/Article/details/gt2avnqrtjv.html

[U27] Py：异步 HTTP
来源：http://www.52xcode.cn/Article/details/gt2rvfvoyyd.html

aiohttp.ClientSession() 配合 async with
来源：http://www.52xcode.cn/Article/details/gt2nmosiudm.html

[U28] Py：类型别名
来源：http://www.ydjk.org.cn/Article/details/gt2rfyoamwb.html

UserId = int
来源：http://www.52xcode.cn/Article/details/gt2rzawefnr.html

[U29] Py：属性校验
来源：http://www.52xcode.cn/Article/details/gt2indethjx.html

@property 与 @x.setter 配合
来源：http://www.52xcode.cn/Article/details/gt2qxoeqhlb.html

[U30] Py：数据类
来源：http://www.ydjk.org.cn/Article/details/gt2wwezreak.html

@dataclass(slots=True)
来源：http://www.52xcode.cn/Article/details/gt2hjipvpay.html

[U31] Py：单测
来源：http://www.ydjk.org.cn/Article/details/gt2qkjmdefc.html

python -m pytest -q
来源：http://www.ydjk.org.cn/Article/details/gt2lrtohyfw.html

[U32] Py：代码格式化
来源：http://www.ydjk.org.cn/Article/details/gt2sooybzef.html

ruff format . && ruff check --fix .
来源：http://www.ydjk.org.cn/Article/details/gt2gvnowktv.html

[U33] Py：打包发布
来源：http://www.52xcode.cn/Article/details/gt2sqtpyqtf.html

python -m build  （依赖 pyproject.toml）
来源：http://www.ydjk.org.cn/Article/details/gt2uyyxhsew.html

[U34] Py：判断编码
来源：http://www.ydjk.org.cn/Article/details/gt2jikojreb.html

chardet.detect(raw)
来源：http://www.52xcode.cn/Article/details/gt2tdataoul.html

[U35] Py：发送邮件
来源：http://www.52xcode.cn/Article/details/gt2tcrfdsqz.html

smtplib.SMTP_SSL(...).send_message(msg)
来源：http://www.52xcode.cn/Article/details/gt2sqrzrgco.html

[U36] Py：定时任务
来源：http://www.52xcode.cn/Article/details/gt2qdmtypve.html

schedule.every(10).minutes.do(job)
来源：http://www.ydjk.org.cn/Article/details/gt2czqvckhz.html

[U37] Py：读写 Excel
来源：http://www.ydjk.org.cn/Article/details/gt2dvomsboz.html

pandas.read_excel / DataFrame.to_excel
来源：http://www.ydjk.org.cn/Article/details/gt2ghgqepko.html

[U38] Py：获取脚本所在目录
来源：http://www.52xcode.cn/Article/details/gt2ipfsslgz.html

Path(__file__).resolve().parent
来源：http://www.ydjk.org.cn/Article/details/gt2iljjnqih.html

[U39] Py：判断是否在交互环境
来源：http://www.ydjk.org.cn/Article/details/gt2qbosdnnb.html

sys.stdout.isatty()
来源：http://www.ydjk.org.cn/Article/details/gt2pnbcmyds.html

[U40] Py：打印到标准错误
来源：http://www.ydjk.org.cn/Article/details/gt2ovrvmwnd.html

print("err", file=sys.stderr)
来源：http://www.ydjk.org.cn/Article/details/gt2mkhxhhrd.html

[U41] PHP：初始化 Composer 项目
来源：http://www.ydjk.org.cn/Article/details/gt2lplufpcf.html

composer init;  composer require guzzlehttp/guzzle
来源：http://www.ydjk.org.cn/Article/details/gt2obmuneiv.html

[U42] PHP：PSR-4 自动加载
来源：http://www.ydjk.org.cn/Article/details/gt2jwawgufi.html

"autoload": { "psr-4": { "App\\": "src/" } }
来源：http://www.ydjk.org.cn/Article/details/gt2wcfvspyf.html

[U43] PHP：声明命名空间
来源：http://www.ydjk.org.cn/Article/details/gt2fstoxuhy.html

namespace App\Http;
来源：http://www.ydjk.org.cn/Article/details/gt2purvgngf.html

[U44] PHP：开启严格类型
来源：http://www.ydjk.org.cn/Article/details/gt2uysdynob.html

declare(strict_types=1);
来源：http://www.52xcode.cn/Article/details/gt2txomjyqc.html

[U45] PHP：类型声明与返回类型
来源：http://www.ydjk.org.cn/Article/details/gt2soiruthr.html

function add(int $a, int $b): int { return $a + $b; }
来源：http://www.ydjk.org.cn/Article/details/gt2ceuicoal.html

[U46] PHP：可空类型
来源：http://www.52xcode.cn/Article/details/gt2ivcapfcq.html

?string $name = null
来源：http://www.ydjk.org.cn/Article/details/gt2xpxodpfc.html

[U47] PHP：联合类型
来源：http://www.ydjk.org.cn/Article/details/gt2fpbjdgrf.html

int|string $id
来源：http://www.52xcode.cn/Article/details/gt2gcrbhhop.html

[U48] PHP：纯枚举
来源：http://www.ydjk.org.cn/Article/details/gt2lzqksxjt.html

enum Status: string { case Active = "active"; case Off = "off"; }
来源：http://www.ydjk.org.cn/Article/details/gt2bomgqpbr.html

[U49] PHP：只读属性
来源：http://www.52xcode.cn/Article/details/gt2rjgxdwny.html

public readonly string $name
来源：http://www.ydjk.org.cn/Article/details/gt2fnyvoeez.html

[U50] PHP：构造器属性提升
来源：http://www.ydjk.org.cn/Article/details/gt2mmukdldb.html

public function __construct(private int $id) {}
来源：http://www.52xcode.cn/Article/details/gt2qnatzplb.html

[U51] PHP：数组解构
来源：http://www.52xcode.cn/Article/details/gt2ctqavppq.html

[$a, $b] = $arr;
来源：http://www.ydjk.org.cn/Article/details/gt2snqlkxra.html

[U52] PHP：箭头函数
来源：http://www.ydjk.org.cn/Article/details/gt2wvdhutij.html

$double = fn($x) => $x * 2;
来源：http://www.52xcode.cn/Article/details/gt2adkbsetp.html

[U53] PHP：空合并运算符
来源：http://www.52xcode.cn/Article/details/gt2owabenyr.html

$v = $a ?? $b ?? "default";
来源：http://www.ydjk.org.cn/Article/details/gt2swsyijsw.html

[U54] PHP：空安全调用
来源：http://www.52xcode.cn/Article/details/gt2uzxetngp.html

$obj?->method()
来源：http://www.ydjk.org.cn/Article/details/gt2mpkdtahm.html

[U55] PHP：match 表达式
来源：http://www.52xcode.cn/Article/details/gt2hpzvrdch.html

$s = match($x) { 1 => "一", default => "其他" };
来源：http://www.ydjk.org.cn/Article/details/gt2tggebnuz.html

[U56] PHP：命名参数
来源：http://www.52xcode.cn/Article/details/gt2mkongiil.html

f(a: 1, b: 2)
来源：http://www.ydjk.org.cn/Article/details/gt2zklqoonn.html

[U57] PHP：字符串插值
来源：http://www.52xcode.cn/Article/details/gt2gnjzuqof.html

"值: {$a}"
来源：http://www.ydjk.org.cn/Article/details/gt2ohxxikjm.html

[U58] PHP：数组三件套
来源：http://www.52xcode.cn/Article/details/gt2orzuomld.html

array_map($f, $a);  array_filter($a, $f);  array_reduce($a, $f, 0);
来源：http://www.ydjk.org.cn/Article/details/gt2lwkrhypi.html

[U59] PHP：自定义排序
来源：http://www.ydjk.org.cn/Article/details/gt2dradujsy.html

usort($arr, fn($a, $b) => $a["age"] <=> $b["age"]);
来源：http://www.ydjk.org.cn/Article/details/gt2jpoqmnbv.html

[U60] PHP：JSON 编解码
来源：http://www.52xcode.cn/Article/details/gt2oznbmhrx.html

json_encode($d, JSON_UNESCAPED_UNICODE);  json_decode($s, true);
来源：http://www.ydjk.org.cn/Article/details/gt2edsssbwg.html

[U61] PHP：正则
来源：http://www.52xcode.cn/Article/details/gt2zbrjmeje.html

preg_match('/(\d+)/', $s, $m);  preg_replace('/\d+/', '#', $s);
来源：http://www.52xcode.cn/Article/details/gt2hyinsutq.html

[U62] PHP：日期对象
来源：http://www.ydjk.org.cn/Article/details/gt2pueigyyu.html

(new DateTimeImmutable())->format("Y-m-d");
来源：http://www.ydjk.org.cn/Article/details/gt2ejxtmnuk.html

[U63] PHP：文件读写
来源：http://www.52xcode.cn/Article/details/gt2brxhuukd.html

file_get_contents($f);  file_put_contents($f, $data);
来源：http://www.ydjk.org.cn/Article/details/gt2ililfyur.html

[U64] PHP：目录遍历
来源：http://www.52xcode.cn/Article/details/gt2ajqlatjj.html

glob("dir/*.php");  scandir("dir");
来源：http://www.52xcode.cn/Article/details/gt2tdbtsfdh.html

[U65] PHP：会话
来源：http://www.ydjk.org.cn/Article/details/gt2sugqhqnn.html

session_start();  $_SESSION["uid"] = 1;
来源：http://www.ydjk.org.cn/Article/details/gt2lflbdipr.html

[U66] PHP：设置 Cookie
来源：http://www.52xcode.cn/Article/details/gt2ehczwkix.html

setcookie("token", $v, ["httponly" => true, "samesite" => "Lax"]);
来源：http://www.ydjk.org.cn/Article/details/gt2ojifoksr.html

[U67] PHP：处理文件上传
来源：http://www.52xcode.cn/Article/details/gt2xaohhrnc.html

$_FILES["file"]["tmp_name"] 与 move_uploaded_file()
来源：http://www.52xcode.cn/Article/details/gt2boynhmaz.html

[U68] PHP：PDO 连接
来源：http://www.52xcode.cn/Article/details/gt2abgoviqr.html

$pdo = new PDO("mysql:host=localhost;dbname=app", "root", "");
来源：http://www.52xcode.cn/Article/details/gt2xlteneiz.html

[U69] PHP：PDO 预处理
来源：http://www.ydjk.org.cn/Article/details/gt2rfnjzppy.html

$stmt = $pdo->prepare("SELECT * FROM users WHERE id = ?");  $stmt->execute([$id]);
来源：http://www.52xcode.cn/Article/details/gt2ahvvjnag.html

[U70] PHP：PDO 事务
来源：http://www.52xcode.cn/Article/details/gt2zyjfjuqs.html

$pdo->beginTransaction();  $pdo->commit();  $pdo->rollBack();
来源：http://www.52xcode.cn/Article/details/gt2pvrruful.html

[U71] PHP：抛出异常
来源：http://www.ydjk.org.cn/Article/details/gt2flfhdkeo.html

throw new RuntimeException("失败", 500);
来源：http://www.ydjk.org.cn/Article/details/gt2qoqifjcb.html

[U72] PHP：写错误日志
来源：http://www.52xcode.cn/Article/details/gt2zsmdccqe.html

error_log("失败: " . $e->getMessage());
来源：http://www.52xcode.cn/Article/details/gt2gmfvcufg.html

[U73] PHP：读取 ini 配置
来源：http://www.52xcode.cn/Article/details/gt2efitdzml.html

parse_ini_file("config.ini", true)
来源：http://www.52xcode.cn/Article/details/gt2bprwzhao.html

[U74] PHP：读取环境变量
来源：http://www.52xcode.cn/Article/details/gt2pafpzemq.html

getenv("APP_ENV") ?: "production"
来源：http://www.ydjk.org.cn/Article/details/gt2iqiwwytb.html

[U75] PHP：依赖注入
来源：http://www.52xcode.cn/Article/details/gt2jaisblpw.html

composer require psr/container
来源：http://www.52xcode.cn/Article/details/gt2pvisagan.html

[U76] PHP：简单路由
来源：http://www.ydjk.org.cn/Article/details/gt2mjmytyyo.html

$path = parse_url($_SERVER["REQUEST_URI"], PHP_URL_PATH);
来源：http://www.ydjk.org.cn/Article/details/gt2zamculwt.html

[U77] PHP：模板渲染
来源：http://www.ydjk.org.cn/Article/details/gt2gartfrmv.html

composer require twig/twig
来源：http://www.ydjk.org.cn/Article/details/gt2mgtmpyvm.html

[U78] PHP：单元测试
来源：http://www.52xcode.cn/Article/details/gt2relkyfhs.html

composer require --dev phpunit/phpunit
来源：http://www.ydjk.org.cn/Article/details/gt2bexebsqs.html

[U79] PHP：静态分析
来源：http://www.ydjk.org.cn/Article/details/gt2srtripno.html

composer require --dev phpstan/phpstan
来源：http://www.52xcode.cn/Article/details/gt2jgwivxlv.html

[U80] PHP：代码规范修复
来源：http://www.ydjk.org.cn/Article/details/gt2dzibkxmf.html

composer require --dev friendsofphp/php-cs-fixer
来源：http://www.ydjk.org.cn/Article/details/gt2trbrebde.html

[U81] JS：初始化项目
来源：http://www.52xcode.cn/Article/details/gt2xuyufjkc.html

npm init -y;  npm i express
来源：http://www.52xcode.cn/Article/details/gt2lyabehls.html

[U82] JS：package.json 脚本
来源：http://www.ydjk.org.cn/Article/details/gt2axkqcrje.html

"scripts": { "dev": "vite", "build": "vite build" }
来源：http://www.52xcode.cn/Article/details/gt2lttaoryt.html

[U83] JS：ES Module 导入导出
来源：http://www.ydjk.org.cn/Article/details/gt2lvefncvd.html

export const a = 1;  import { a } from "./m.js";
来源：http://www.52xcode.cn/Article/details/gt2gdcgomtj.html

[U84] JS：CommonJS 写法
来源：http://www.52xcode.cn/Article/details/gt2kvfxzhae.html

module.exports = { a };  const { a } = require("./m");
来源：http://www.52xcode.cn/Article/details/gt2ygvuudqb.html

[U85] JS：可选链
来源：http://www.ydjk.org.cn/Article/details/gt2ohgzikqr.html

a?.b?.c
来源：http://www.ydjk.org.cn/Article/details/gt2fjbcuqzj.html

[U86] JS：空值合并
来源：http://www.52xcode.cn/Article/details/gt2lvsuafib.html

a ?? b
来源：http://www.ydjk.org.cn/Article/details/gt2ybxyhsii.html

[U87] JS：解构默认值
来源：http://www.52xcode.cn/Article/details/gt2pybmsrob.html

const { a = 1, b = 2 } = obj;
来源：http://www.ydjk.org.cn/Article/details/gt2dsagjbjw.html

[U88] JS：对象展开合并
来源：http://www.ydjk.org.cn/Article/details/gt2zazpnoxc.html

{ ...a, ...b }
来源：http://www.ydjk.org.cn/Article/details/gt2dsiaivsh.html


<!-- 参考信息 -->