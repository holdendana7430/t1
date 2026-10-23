代发 wailian999

[T05] Kotlin：when 表达式
来源：http://www.ydjk.org.cn/Article/details/gt3kevtzlts.html

val s = when (x) { 1 -> "一" else -> "其他" }   // 多分支时每个分支单独一行
来源：http://www.52xcode.cn/Article/details/gt3eikzteea.html

[T06] Kotlin：集合映射
来源：http://www.ydjk.org.cn/Article/details/gt3nesuldsm.html

listOf(1, 2, 3).map { it * 2 }
来源：http://www.ydjk.org.cn/Article/details/gt3vezubakw.html

[T07] Kotlin：集合过滤
来源：http://www.ydjk.org.cn/Article/details/gt3ovnphcek.html

listOf(1, 2, 3).filter { it > 1 }
来源：http://www.ydjk.org.cn/Article/details/gt3uffxrawx.html

[T08] Kotlin：数据类
来源：http://www.ydjk.org.cn/Article/details/gt3uxmwquhn.html

data class User(val name: String, val age: Int)
来源：http://www.ydjk.org.cn/Article/details/gt3hukcqwcr.html

[T09] Kotlin：扩展函数
来源：http://www.52xcode.cn/Article/details/gt3ejjkvyuk.html

fun String.exclaim() = this + "!"
来源：http://www.ydjk.org.cn/Article/details/gt3wesyrlqk.html

[T10] Kotlin：默认参数
来源：http://www.ydjk.org.cn/Article/details/gt3bzywcsuv.html

fun greet(name: String = "World") = "Hi $name"
来源：http://www.52xcode.cn/Article/details/gt3mhkapvxr.html

[T11] Kotlin：协程
来源：http://www.52xcode.cn/Article/details/gt3rpqmtwjl.html

GlobalScope.launch { delay(1000); println("done") }
来源：http://www.52xcode.cn/Article/details/gt3hiqcvmfp.html

[T12] Kotlin：解构声明
来源：http://www.ydjk.org.cn/Article/details/gt3wqkodtfp.html

val (a, b) = Pair(1, 2)
来源：http://www.52xcode.cn/Article/details/gt3yaioypeg.html

[T13] Kotlin：只读 Map
来源：http://www.ydjk.org.cn/Article/details/gt3whrpwour.html

val m = mapOf("a" to 1)
来源：http://www.52xcode.cn/Article/details/gt3wjngbrir.html

[T14] Kotlin：循环
来源：http://www.52xcode.cn/Article/details/gt3umbqolho.html

for (i in 1..10) println(i)
来源：http://www.52xcode.cn/Article/details/gt3sslfpqwl.html

[T15] Kotlin：接口
来源：http://www.52xcode.cn/Article/details/gt3zbvirnrc.html

interface Shape { fun area(): Double }
来源：http://www.52xcode.cn/Article/details/gt3kfclqoqx.html

[T16] Swift：Hello World
来源：http://www.ydjk.org.cn/Article/details/gt3rypoxabj.html

print("Hello")
来源：http://www.ydjk.org.cn/Article/details/gt3ceddslwm.html

[T17] Swift：变量与常量
来源：http://www.ydjk.org.cn/Article/details/gt3xbsnarid.html

var a = 1;  let b = 2
来源：http://www.52xcode.cn/Article/details/gt3rjfsdppi.html

[T18] Swift：字符串插值
来源：http://www.52xcode.cn/Article/details/gt3jbblkoad.html

"值: \(b)"
来源：http://www.52xcode.cn/Article/details/gt3ycgvyocm.html

[T19] Swift：可选绑定
来源：http://www.52xcode.cn/Article/details/gt3hbbkopvc.html

if let n = opt { print(n) }
来源：http://www.ydjk.org.cn/Article/details/gt3ngoewzvo.html

[T20] Swift：数组操作
来源：http://www.52xcode.cn/Article/details/gt3zbnzxcby.html

var a = [1, 2, 3];  a.append(4)
来源：http://www.ydjk.org.cn/Article/details/gt3gzvlghjv.html

[T21] Swift：遍历
来源：http://www.ydjk.org.cn/Article/details/gt3emqghycd.html

for x in a { print(x) }
来源：http://www.ydjk.org.cn/Article/details/gt3yzrtiitw.html

[T22] Swift：字典
来源：http://www.52xcode.cn/Article/details/gt3hbcapjfn.html

var d = ["a": 1];  d["b"] = 2
来源：http://www.ydjk.org.cn/Article/details/gt3wuhyditr.html

[T23] Swift：函数
来源：http://www.52xcode.cn/Article/details/gt3shypyumj.html

func add(_ a: Int, _ b: Int) -> Int { a + b }
来源：http://www.52xcode.cn/Article/details/gt3sbgtbhql.html

[T24] Swift：闭包
来源：http://www.52xcode.cn/Article/details/gt3whnpbzvf.html

let f = { (x: Int) -> Int in x * 2 }
来源：http://www.52xcode.cn/Article/details/gt3ywrcnzky.html

[T25] Swift：结构体
来源：http://www.52xcode.cn/Article/details/gt3dbtxktro.html

struct P { var x: Int }
来源：http://www.52xcode.cn/Article/details/gt3pewdlzvm.html

[T26] Swift：类与重写
来源：http://www.52xcode.cn/Article/details/gt3xqfsdckd.html

class A: Base { override func f() {} }
来源：http://www.ydjk.org.cn/Article/details/gt3iuwavhyz.html

[T27] Swift：错误处理
来源：http://www.ydjk.org.cn/Article/details/gt3xyzopgmp.html

do { try f() } catch { print(error) }
来源：http://www.52xcode.cn/Article/details/gt3veapcxoj.html

[T28] Swift：枚举
来源：http://www.ydjk.org.cn/Article/details/gt3hwazunrt.html

enum Color { case red, green }
来源：http://www.52xcode.cn/Article/details/gt3gjwwpizn.html

[T29] Swift：guard 提前返回
来源：http://www.ydjk.org.cn/Article/details/gt3admlygrb.html

guard let x = opt else { return }
来源：http://www.ydjk.org.cn/Article/details/gt3knpmggbx.html

[T30] Swift：协议
来源：http://www.52xcode.cn/Article/details/gt3yxoigoyn.html

protocol Shape { func area() -> Double }
来源：http://www.ydjk.org.cn/Article/details/gt3iojyzpah.html

[T31] Lua：Hello World
来源：http://www.ydjk.org.cn/Article/details/gt3bghnzzzo.html

print("Hello")
来源：http://www.52xcode.cn/Article/details/gt3msarsvnc.html

[T32] Lua：局部变量
来源：http://www.ydjk.org.cn/Article/details/gt3ujvrleug.html

local a = 1
来源：http://www.ydjk.org.cn/Article/details/gt3mrvszixy.html

[T33] Lua：表（数组）
来源：http://www.ydjk.org.cn/Article/details/gt3umgyeram.html

local t = {1, 2, 3};  t[4] = 4
来源：http://www.ydjk.org.cn/Article/details/gt3kyewmfkq.html

[T34] Lua：遍历表
来源：http://www.52xcode.cn/Article/details/gt3dnuzlwjn.html

for i, v in ipairs(t) do print(i, v) end
来源：http://www.52xcode.cn/Article/details/gt3zsxtugca.html

[T35] Lua：字典表
来源：http://www.52xcode.cn/Article/details/gt3fxsymfkm.html

local d = { a = 1 };  d.b = 2
来源：http://www.52xcode.cn/Article/details/gt3upsxvege.html

[T36] Lua：函数
来源：http://www.52xcode.cn/Article/details/gt3kgwjgrvx.html

function add(a, b) return a + b end
来源：http://www.ydjk.org.cn/Article/details/gt3pmaixgml.html

[T37] Lua：字符串拼接
来源：http://www.ydjk.org.cn/Article/details/gt3mudcgwrt.html

"a" .. "b"
来源：http://www.52xcode.cn/Article/details/gt3cfjqwnqu.html

[T38] Lua：条件
来源：http://www.ydjk.org.cn/Article/details/gt3muugsfqr.html

if x > 0 then print("正") end
来源：http://www.ydjk.org.cn/Article/details/gt3xoqvspro.html

[T39] Lua：模式匹配
来源：http://www.52xcode.cn/Article/details/gt3nshpnwip.html

string.find(s, "%d+")
来源：http://www.52xcode.cn/Article/details/gt3xuhmjevs.html

[T40] Lua：元表
来源：http://www.52xcode.cn/Article/details/gt3vnzdjxqe.html

setmetatable({}, { __index = base })
来源：http://www.ydjk.org.cn/Article/details/gt3mkujqsmn.html

[T41] Perl：Hello World
来源：http://www.52xcode.cn/Article/details/gt3ixojaemq.html

print "Hello\n";
来源：http://www.52xcode.cn/Article/details/gt3ashibfkp.html

[T42] Perl：变量类型
来源：http://www.ydjk.org.cn/Article/details/gt3zmoddsjp.html

my $a = 1;  my @arr = (1, 2, 3);  my %h = (a => 1);
来源：http://www.52xcode.cn/Article/details/gt3dzcilzib.html

[T43] Perl：字符串插值
来源：http://www.52xcode.cn/Article/details/gt3mwaprqvs.html

"值: $a"
来源：http://www.52xcode.cn/Article/details/gt3wjsegurg.html

[T44] Perl：条件
来源：http://www.ydjk.org.cn/Article/details/gt3mrdipfdw.html

if ($a > 0) { print "正"; }
来源：http://www.52xcode.cn/Article/details/gt3lvdfdtyi.html

[T45] Perl：数组遍历
来源：http://www.ydjk.org.cn/Article/details/gt3jwgdzvsx.html

for my $x (@arr) { print $x; }
来源：http://www.52xcode.cn/Article/details/gt3cckgzalt.html

[T46] Perl：哈希操作
来源：http://www.52xcode.cn/Article/details/gt3cxicrjyn.html

$h{b} = 2;  for my $k (keys %h) { print "$k=$h{$k}"; }
来源：http://www.ydjk.org.cn/Article/details/gt3ggitupiy.html

[T47] Perl：正则捕获
来源：http://www.52xcode.cn/Article/details/gt3epabrqir.html

if ($s =~ /(\d+)/) { print $1; }
来源：http://www.52xcode.cn/Article/details/gt3ecthmtid.html

[T48] Perl：正则替换
来源：http://www.ydjk.org.cn/Article/details/gt3jiojmedm.html

$s =~ s/old/new/g;
来源：http://www.ydjk.org.cn/Article/details/gt3eygmrzoz.html

[T49] Perl：函数
来源：http://www.ydjk.org.cn/Article/details/gt3nfikrcin.html

sub add { my ($a, $b) = @_; return $a + $b; }
来源：http://www.ydjk.org.cn/Article/details/gt3vkamtesn.html

[T50] Perl：逐行读文件
来源：http://www.ydjk.org.cn/Article/details/gt3fppruppg.html

open my $fh, "<", "a.txt" or die $!;
来源：http://www.52xcode.cn/Article/details/gt3kycuibrj.html

while (my $line = <$fh>) { print $line; }
来源：http://www.52xcode.cn/Article/details/gt3mmvbedhv.html

[T51] Scala：Hello World
来源：http://www.ydjk.org.cn/Article/details/gt3hfniwywy.html

println("Hello")
来源：http://www.52xcode.cn/Article/details/gt3rswwcebg.html

[T52] Scala：变量
来源：http://www.ydjk.org.cn/Article/details/gt3tvwtjauz.html

val a = 1;  var b = 2
来源：http://www.ydjk.org.cn/Article/details/gt3rbhrfhkf.html

[T53] Scala：字符串插值
来源：http://www.52xcode.cn/Article/details/gt3sjkclwnf.html

s"值: $b"
来源：http://www.52xcode.cn/Article/details/gt3yyyvynty.html

[T54] Scala：集合映射
来源：http://www.ydjk.org.cn/Article/details/gt3nqaqysqi.html

List(1, 2, 3).map(_ * 2)
来源：http://www.52xcode.cn/Article/details/gt3mlrwdodn.html

[T55] Scala：集合过滤
来源：http://www.ydjk.org.cn/Article/details/gt3zrvkbxaa.html

List(1, 2, 3).filter(_ > 1)
来源：http://www.ydjk.org.cn/Article/details/gt3czfshndb.html

[T56] Scala：样例类
来源：http://www.52xcode.cn/Article/details/gt3buyokjwf.html

case class User(name: String, age: Int)
来源：http://www.ydjk.org.cn/Article/details/gt3pfaymftz.html

[T57] Scala：模式匹配
来源：http://www.ydjk.org.cn/Article/details/gt3vdrjsxzq.html

x match { case 1 => "一"; case _ => "其他" }
来源：http://www.52xcode.cn/Article/details/gt3qrjdhiah.html

[T58] Scala：函数定义
来源：http://www.ydjk.org.cn/Article/details/gt3xbwuggjm.html

def add(a: Int, b: Int): Int = a + b
来源：http://www.52xcode.cn/Article/details/gt3bqolowvh.html

[T59] Scala：循环
来源：http://www.ydjk.org.cn/Article/details/gt3gnmjvvha.html

for (i <- 1 to 10) println(i)
来源：http://www.ydjk.org.cn/Article/details/gt3anuebycl.html

[T60] Scala：折叠
来源：http://www.ydjk.org.cn/Article/details/gt3cptpzzgc.html

List(1, 2, 3).foldLeft(0)(_ + _)
来源：http://www.ydjk.org.cn/Article/details/gt3obtgrfgq.html

================================================================================
来源：http://www.52xcode.cn/Article/details/gt3qmufoftg.html

U. 高频实用片段（Python / PHP / JavaScript 各 40 条）
来源：http://www.52xcode.cn/Article/details/gt3zdterscb.html

================================================================================
来源：http://www.ydjk.org.cn/Article/details/gt3kcdklqvg.html

[U01] Py：创建虚拟环境
来源：http://www.52xcode.cn/Article/details/gt3tobxmxog.html

python -m venv .venv && source .venv/bin/activate
来源：http://www.52xcode.cn/Article/details/gt3ptfsopyn.html

[U02] Py：导出 / 安装依赖
来源：http://www.ydjk.org.cn/Article/details/gt3xxasgqmf.html

pip freeze > requirements.txt;  pip install -r requirements.txt
来源：http://www.52xcode.cn/Article/details/gt3sgimysqf.html

[U03] Py：加载 .env 配置
来源：http://www.ydjk.org.cn/Article/details/gt3jfllkiut.html

from dotenv import load_dotenv; load_dotenv()
来源：http://www.ydjk.org.cn/Article/details/gt3xhtaykzh.html

[U04] Py：变量调试打印
来源：http://www.ydjk.org.cn/Article/details/gt3yoronokk.html

print(f"{x=}")            # 输出 x=值，Python 3.8+
来源：http://www.52xcode.cn/Article/details/gt3hdxpszjd.html

[U05] Py：列表去重且保序
来源：http://www.52xcode.cn/Article/details/gt3wmwlwyvj.html

list(dict.fromkeys(arr))
来源：http://www.ydjk.org.cn/Article/details/gt3rbhepstr.html

[U06] Py：合并两个字典
来源：http://www.ydjk.org.cn/Article/details/gt3pvhxicss.html

{**a, **b}
来源：http://www.52xcode.cn/Article/details/gt3ifryczug.html

[U07] Py：反转字典键值
来源：http://www.52xcode.cn/Article/details/gt3gwioghxk.html

{v: k for k, v in d.items()}
来源：http://www.52xcode.cn/Article/details/gt3nqpkrzhe.html

[U08] Py：展平二维列表
来源：http://www.ydjk.org.cn/Article/details/gt3yxfyzqdr.html

[y for x in nested for y in x]
来源：http://www.52xcode.cn/Article/details/gt3blclvoje.html

[U09] Py：字典取最大值的键
来源：http://www.ydjk.org.cn/Article/details/gt3ajfdywdz.html

max(d, key=d.get)
来源：http://www.52xcode.cn/Article/details/gt3opdnttxm.html

[U10] Py：按值排序字典
来源：http://www.ydjk.org.cn/Article/details/gt3bxbnmnsg.html

dict(sorted(d.items(), key=lambda kv: kv[1]))
来源：http://www.ydjk.org.cn/Article/details/gt3uvkgalty.html

[U11] Py：生成器表达式
来源：http://www.ydjk.org.cn/Article/details/gt3josfyjac.html

(x * 2 for x in arr)
来源：http://www.52xcode.cn/Article/details/gt3mqdwlagk.html

[U12] Py：取出现最多的 3 个元素
来源：http://www.ydjk.org.cn/Article/details/gt3dzevfoqy.html

Counter(arr).most_common(3)
来源：http://www.52xcode.cn/Article/details/gt3edtbsawq.html

[U13] Py：固定长度队列
来源：http://www.ydjk.org.cn/Article/details/gt3hpijhidg.html

deque(maxlen=10)
来源：http://www.52xcode.cn/Article/details/gt3sdolsaef.html

[U14] Py：分组收集到列表
来源：http://www.ydjk.org.cn/Article/details/gt3lkwpoocj.html

defaultdict(list)
来源：http://www.52xcode.cn/Article/details/gt3llztocif.html

[U15] Py：高精度计时
来源：http://www.ydjk.org.cn/Article/details/gt3zbemthdd.html

t = time.perf_counter()
来源：http://www.ydjk.org.cn/Article/details/gt3jjphgvzn.html

[U16] Py：命令行参数解析
来源：http://www.ydjk.org.cn/Article/details/gt3caftpvsd.html

ap = argparse.ArgumentParser();  ap.add_argument("--name");  args = ap.parse_args()
来源：http://www.52xcode.cn/Article/details/gt3jeldkzuq.html

[U17] Py：初始化日志
来源：http://www.52xcode.cn/Article/details/gt3zinlzlwa.html

logging.basicConfig(level=logging.INFO)
来源：http://www.ydjk.org.cn/Article/details/gt3rtyaycnz.html

[U18] Py：预编译正则
来源：http://www.ydjk.org.cn/Article/details/gt3rtnhjoal.html

pat = re.compile(r"\d+")
来源：http://www.52xcode.cn/Article/details/gt3fveadyeb.html

[U19] Py：正则替换带回调
来源：http://www.ydjk.org.cn/Article/details/gt3oclunodx.html

re.sub(r"\d+", lambda m: str(int(m.group()) * 2), s)
来源：http://www.ydjk.org.cn/Article/details/gt3lbazpxem.html

[U20] Py：缓存函数结果
来源：http://www.52xcode.cn/Article/details/gt3ozzkvkmm.html

@functools.lru_cache(maxsize=None)
来源：http://www.ydjk.org.cn/Article/details/gt3elpaxwfz.html

[U21] Py：自定义上下文管理器
来源：http://www.ydjk.org.cn/Article/details/gt3nduefwqz.html

@contextlib.contextmanager
来源：http://www.52xcode.cn/Article/details/gt3hodauzjk.html

[U22] Py：矩阵转置
来源：http://www.ydjk.org.cn/Article/details/gt3lntsyqbg.html

list(zip(*m))
来源：http://www.52xcode.cn/Article/details/gt3xlkydkda.html

[U23] Py：分块读取大文件
来源：http://www.ydjk.org.cn/Article/details/gt3gxpwjuyc.html

for chunk in iter(lambda: f.read(8192), b""):
来源：http://www.ydjk.org.cn/Article/details/gt3mhqrzjai.html

[U24] Py：路径操作
来源：http://www.ydjk.org.cn/Article/details/gt3gnfeowiy.html

Path("a/b.txt").parent.mkdir(parents=True, exist_ok=True)
来源：http://www.52xcode.cn/Article/details/gt3moqqetbh.html

[U25] Py：CSV 按字典读
来源：http://www.52xcode.cn/Article/details/gt3dpqkfcun.html

csv.DictReader(f)
来源：http://www.ydjk.org.cn/Article/details/gt3auamyyxo.html

[U26] Py：并发下载
来源：http://www.ydjk.org.cn/Article/details/gt3jeegpawj.html

ThreadPoolExecutor(max_workers=8).map(fetch, urls)
来源：http://www.ydjk.org.cn/Article/details/gt3flgltqpd.html

[U27] Py：异步 HTTP
来源：http://www.ydjk.org.cn/Article/details/gt3xrkaylge.html

aiohttp.ClientSession() 配合 async with
来源：http://www.ydjk.org.cn/Article/details/gt3yfyadvht.html

[U28] Py：类型别名
来源：http://www.52xcode.cn/Article/details/gt3wmwfzkuu.html

UserId = int
来源：http://www.52xcode.cn/Article/details/gt3epyjefzw.html

[U29] Py：属性校验
来源：http://www.52xcode.cn/Article/details/gt3jewnddmf.html

@property 与 @x.setter 配合
来源：http://www.52xcode.cn/Article/details/gt3jpqnlqcb.html

[U30] Py：数据类
来源：http://www.52xcode.cn/Article/details/gt3hrlcfbjp.html

@dataclass(slots=True)
来源：http://www.ydjk.org.cn/Article/details/gt3kjcefxqh.html

[U31] Py：单测
来源：http://www.52xcode.cn/Article/details/gt3oolorvxw.html

python -m pytest -q
来源：http://www.52xcode.cn/Article/details/gt3emvfxdmy.html

[U32] Py：代码格式化
来源：http://www.52xcode.cn/Article/details/gt3gxrkypjc.html

ruff format . && ruff check --fix .
来源：http://www.52xcode.cn/Article/details/gt3dzspgrwc.html

[U33] Py：打包发布
来源：http://www.ydjk.org.cn/Article/details/gt3dcrfwhdc.html

python -m build  （依赖 pyproject.toml）
来源：http://www.ydjk.org.cn/Article/details/gt3tjudrszw.html

[U34] Py：判断编码
来源：http://www.ydjk.org.cn/Article/details/gt3bzybwujk.html

chardet.detect(raw)
来源：http://www.ydjk.org.cn/Article/details/gt3kmojkphm.html

[U35] Py：发送邮件
来源：http://www.52xcode.cn/Article/details/gt3cbbpfhbq.html

smtplib.SMTP_SSL(...).send_message(msg)
来源：http://www.ydjk.org.cn/Article/details/gt3avcwijks.html

[U36] Py：定时任务
来源：http://www.ydjk.org.cn/Article/details/gt3pnfadmdb.html

schedule.every(10).minutes.do(job)
来源：http://www.ydjk.org.cn/Article/details/gt3jocjaris.html

[U37] Py：读写 Excel
来源：http://www.52xcode.cn/Article/details/gt3nwhomvef.html

pandas.read_excel / DataFrame.to_excel
来源：http://www.ydjk.org.cn/Article/details/gt3nynljynw.html

[U38] Py：获取脚本所在目录
来源：http://www.ydjk.org.cn/Article/details/gt3wgcrpjfw.html

Path(__file__).resolve().parent
来源：http://www.52xcode.cn/Article/details/gt3utpvzemk.html

[U39] Py：判断是否在交互环境
来源：http://www.52xcode.cn/Article/details/gt3ckfchvik.html

sys.stdout.isatty()
来源：http://www.52xcode.cn/Article/details/gt3nyjavaac.html

[U40] Py：打印到标准错误
来源：http://www.52xcode.cn/Article/details/gt3iucmhsco.html

print("err", file=sys.stderr)
来源：http://www.52xcode.cn/Article/details/gt3eanejcwz.html

[U41] PHP：初始化 Composer 项目
来源：http://www.ydjk.org.cn/Article/details/gt3ozovirmh.html

composer init;  composer require guzzlehttp/guzzle
来源：http://www.ydjk.org.cn/Article/details/gt3ppoczeco.html

[U42] PHP：PSR-4 自动加载
来源：http://www.52xcode.cn/Article/details/gt3kqondsyu.html

"autoload": { "psr-4": { "App\\": "src/" } }
来源：http://www.ydjk.org.cn/Article/details/gt3ugmhlejg.html

[U43] PHP：声明命名空间
来源：http://www.52xcode.cn/Article/details/gt3tcwthvsa.html

namespace App\Http;
来源：http://www.ydjk.org.cn/Article/details/gt3bsgtjzfs.html

[U44] PHP：开启严格类型
来源：http://www.ydjk.org.cn/Article/details/gt3mveivzyx.html

declare(strict_types=1);
来源：http://www.52xcode.cn/Article/details/gt3ynymzeeg.html

[U45] PHP：类型声明与返回类型
来源：http://www.ydjk.org.cn/Article/details/gt3gghdotui.html

function add(int $a, int $b): int { return $a + $b; }
来源：http://www.52xcode.cn/Article/details/gt3johpjlkd.html

[U46] PHP：可空类型
来源：http://www.52xcode.cn/Article/details/gt3xvmijukx.html

?string $name = null
来源：http://www.52xcode.cn/Article/details/gt3jpswwqlg.html

[U47] PHP：联合类型
来源：http://www.52xcode.cn/Article/details/gt3nivbybnb.html

int|string $id
来源：http://www.52xcode.cn/Article/details/gt3egtirhqz.html

[U48] PHP：纯枚举
来源：http://www.ydjk.org.cn/Article/details/gt3szodwwsi.html

enum Status: string { case Active = "active"; case Off = "off"; }
来源：http://www.52xcode.cn/Article/details/gt3hnexooin.html

[U49] PHP：只读属性
来源：http://www.ydjk.org.cn/Article/details/gt3lbsskxxs.html

public readonly string $name
来源：http://www.ydjk.org.cn/Article/details/gt3rjmuongj.html

[U50] PHP：构造器属性提升
来源：http://www.52xcode.cn/Article/details/gt3aegqnsqe.html

public function __construct(private int $id) {}
来源：http://www.ydjk.org.cn/Article/details/gt3vkcwentx.html

[U51] PHP：数组解构
来源：http://www.ydjk.org.cn/Article/details/gt3rygtxiii.html

[$a, $b] = $arr;
来源：http://www.52xcode.cn/Article/details/gt3hxvykhkf.html

[U52] PHP：箭头函数
来源：http://www.ydjk.org.cn/Article/details/gt3opivznsr.html

$double = fn($x) => $x * 2;
来源：http://www.52xcode.cn/Article/details/gt3bjgqgmqx.html

[U53] PHP：空合并运算符
来源：http://www.ydjk.org.cn/Article/details/gt3iaentukc.html

$v = $a ?? $b ?? "default";
来源：http://www.52xcode.cn/Article/details/gt3wzmvbpgx.html

[U54] PHP：空安全调用
来源：http://www.ydjk.org.cn/Article/details/gt3rbsspxod.html

$obj?->method()
来源：http://www.52xcode.cn/Article/details/gt3yjbczgea.html

[U55] PHP：match 表达式
来源：http://www.52xcode.cn/Article/details/gt3sbjevadj.html

$s = match($x) { 1 => "一", default => "其他" };
来源：http://www.52xcode.cn/Article/details/gt3idhttkqw.html

[U56] PHP：命名参数
来源：http://www.ydjk.org.cn/Article/details/gt3unewytky.html

f(a: 1, b: 2)
来源：http://www.ydjk.org.cn/Article/details/gt3hebptmzk.html

[U57] PHP：字符串插值
来源：http://www.52xcode.cn/Article/details/gt3bagghwim.html

"值: {$a}"
来源：http://www.ydjk.org.cn/Article/details/gt3lahdxsnj.html

[U58] PHP：数组三件套
来源：http://www.52xcode.cn/Article/details/gt3xekkrgbz.html

array_map($f, $a);  array_filter($a, $f);  array_reduce($a, $f, 0);
来源：http://www.ydjk.org.cn/Article/details/gt3dvvsuyhe.html

[U59] PHP：自定义排序
来源：http://www.52xcode.cn/Article/details/gt3plgghqwv.html

usort($arr, fn($a, $b) => $a["age"] <=> $b["age"]);
来源：http://www.52xcode.cn/Article/details/gt3lqsnmnqm.html

[U60] PHP：JSON 编解码
来源：http://www.52xcode.cn/Article/details/gt3hskxfgal.html

json_encode($d, JSON_UNESCAPED_UNICODE);  json_decode($s, true);
来源：http://www.52xcode.cn/Article/details/gt3hlmufykd.html

[U61] PHP：正则
来源：http://www.52xcode.cn/Article/details/gt3lfjsdnjh.html

preg_match('/(\d+)/', $s, $m);  preg_replace('/\d+/', '#', $s);
来源：http://www.ydjk.org.cn/Article/details/gt3ahpdalzp.html

[U62] PHP：日期对象
来源：http://www.ydjk.org.cn/Article/details/gt3rrblshyw.html

(new DateTimeImmutable())->format("Y-m-d");
来源：http://www.52xcode.cn/Article/details/gt3tgyxdytr.html

[U63] PHP：文件读写
来源：http://www.52xcode.cn/Article/details/gt3gzdgvbhd.html

file_get_contents($f);  file_put_contents($f, $data);
来源：http://www.ydjk.org.cn/Article/details/gt3bhnzmvsc.html

[U64] PHP：目录遍历
来源：http://www.52xcode.cn/Article/details/gt3lolagfhc.html

glob("dir/*.php");  scandir("dir");
来源：http://www.52xcode.cn/Article/details/gt3quwidglk.html

[U65] PHP：会话
来源：http://www.52xcode.cn/Article/details/gt3ndpezebi.html

session_start();  $_SESSION["uid"] = 1;
来源：http://www.52xcode.cn/Article/details/gt3rmolwzpi.html

[U66] PHP：设置 Cookie
来源：http://www.52xcode.cn/Article/details/gt3dlhplipm.html

setcookie("token", $v, ["httponly" => true, "samesite" => "Lax"]);
来源：http://www.52xcode.cn/Article/details/gt3gyzflbds.html

[U67] PHP：处理文件上传
来源：http://www.52xcode.cn/Article/details/gt3ugprvuep.html

$_FILES["file"]["tmp_name"] 与 move_uploaded_file()
来源：http://www.52xcode.cn/Article/details/gt3rjuwhmgw.html

[U68] PHP：PDO 连接
来源：http://www.52xcode.cn/Article/details/gt3kimeugdj.html

$pdo = new PDO("mysql:host=localhost;dbname=app", "root", "");
来源：http://www.52xcode.cn/Article/details/gt3ctdahjrr.html

[U69] PHP：PDO 预处理
来源：http://www.ydjk.org.cn/Article/details/gt3mdebvllm.html

$stmt = $pdo->prepare("SELECT * FROM users WHERE id = ?");  $stmt->execute([$id]);
来源：http://www.ydjk.org.cn/Article/details/gt3pawrsnxe.html

[U70] PHP：PDO 事务
来源：http://www.52xcode.cn/Article/details/gt3bqxmtyma.html

$pdo->beginTransaction();  $pdo->commit();  $pdo->rollBack();
来源：http://www.ydjk.org.cn/Article/details/gt3gjgzjjqk.html

[U71] PHP：抛出异常
来源：http://www.ydjk.org.cn/Article/details/gt3xkzmzlun.html

throw new RuntimeException("失败", 500);
来源：http://www.ydjk.org.cn/Article/details/gt3wbakddqx.html

[U72] PHP：写错误日志
来源：http://www.ydjk.org.cn/Article/details/gt3mxggutkw.html

error_log("失败: " . $e->getMessage());
来源：http://www.52xcode.cn/Article/details/gt3oyjxdujq.html

[U73] PHP：读取 ini 配置
来源：http://www.ydjk.org.cn/Article/details/gt3jnublkzx.html

parse_ini_file("config.ini", true)
来源：http://www.ydjk.org.cn/Article/details/gt3wzybpyww.html

[U74] PHP：读取环境变量
来源：http://www.52xcode.cn/Article/details/gt3pfzcatsn.html

getenv("APP_ENV") ?: "production"
来源：http://www.52xcode.cn/Article/details/gt3ppdjotkv.html

[U75] PHP：依赖注入
来源：http://www.ydjk.org.cn/Article/details/gt3ddenydea.html

composer require psr/container
来源：http://www.ydjk.org.cn/Article/details/gt3takgxbnw.html

[U76] PHP：简单路由
来源：http://www.ydjk.org.cn/Article/details/gt3puwymznl.html

$path = parse_url($_SERVER["REQUEST_URI"], PHP_URL_PATH);
来源：http://www.52xcode.cn/Article/details/gt3oanhbbel.html

[U77] PHP：模板渲染
来源：http://www.ydjk.org.cn/Article/details/gt3cjcltnuk.html

composer require twig/twig
来源：http://www.ydjk.org.cn/Article/details/gt3ghhautpo.html

[U78] PHP：单元测试
来源：http://www.52xcode.cn/Article/details/gt3qwxxgmcq.html

composer require --dev phpunit/phpunit
来源：http://www.ydjk.org.cn/Article/details/gt3odwutowf.html

[U79] PHP：静态分析
来源：http://www.52xcode.cn/Article/details/gt3senqzhac.html

composer require --dev phpstan/phpstan
来源：http://www.ydjk.org.cn/Article/details/gt3uiwsctus.html

[U80] PHP：代码规范修复
来源：http://www.52xcode.cn/Article/details/gt3txdykftm.html

composer require --dev friendsofphp/php-cs-fixer
来源：http://www.52xcode.cn/Article/details/gt3tapktomo.html

[U81] JS：初始化项目
来源：http://www.ydjk.org.cn/Article/details/gt3iktecsoa.html

npm init -y;  npm i express
来源：http://www.52xcode.cn/Article/details/gt3helkapxq.html

[U82] JS：package.json 脚本
来源：http://www.ydjk.org.cn/Article/details/gt3waxgcadm.html

"scripts": { "dev": "vite", "build": "vite build" }
来源：http://www.52xcode.cn/Article/details/gt3pxumzayk.html

[U83] JS：ES Module 导入导出
来源：http://www.ydjk.org.cn/Article/details/gt3uqasgbek.html

export const a = 1;  import { a } from "./m.js";
来源：http://www.ydjk.org.cn/Article/details/gt3yeviacbt.html

[U84] JS：CommonJS 写法
来源：http://www.52xcode.cn/Article/details/gt3ukhocmpu.html

module.exports = { a };  const { a } = require("./m");
来源：http://www.ydjk.org.cn/Article/details/gt3ivwedbmo.html

[U85] JS：可选链
来源：http://www.52xcode.cn/Article/details/gt3wsipbsuv.html

a?.b?.c
来源：http://www.52xcode.cn/Article/details/gt3dyiovtdd.html

[U86] JS：空值合并
来源：http://www.ydjk.org.cn/Article/details/gt3cjkspmax.html

a ?? b
来源：http://www.52xcode.cn/Article/details/gt3slhmfoqu.html

[U87] JS：解构默认值
来源：http://www.52xcode.cn/Article/details/gt3gaaxwzdt.html

const { a = 1, b = 2 } = obj;
来源：http://www.52xcode.cn/Article/details/gt3wbifxoee.html

[U88] JS：对象展开合并
来源：http://www.ydjk.org.cn/Article/details/gt3wkposjmx.html

{ ...a, ...b }
来源：http://www.ydjk.org.cn/Article/details/gt3czwjvzdu.html

[U89] JS：数组去重
来源：http://www.52xcode.cn/Article/details/gt3qnbgubvv.html

[...new Set(arr)]
来源：http://www.ydjk.org.cn/Article/details/gt3orlkdezd.html

[U90] JS：数字数组排序
来源：http://www.52xcode.cn/Article/details/gt3xznfhfvl.html

[...arr].sort((a, b) => a - b)
来源：http://www.52xcode.cn/Article/details/gt3cbvtfxqk.html

[U91] JS：对象键值遍历
来源：http://www.ydjk.org.cn/Article/details/gt3yzlknggv.html

Object.entries(obj).forEach(([k, v]) => {});
来源：http://www.ydjk.org.cn/Article/details/gt3jdtuhoyv.html

[U92] JS：深拷贝
来源：http://www.52xcode.cn/Article/details/gt3ajfvnzgd.html

structuredClone(obj)
来源：http://www.52xcode.cn/Article/details/gt3hsduuhza.html


<!-- 参考信息 -->