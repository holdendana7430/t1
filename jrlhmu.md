代发 wailian999

[T09] Kotlin：扩展函数
来源：http://www.52xcode.cn/Article/details/gt3agvicdhb.html

fun String.exclaim() = this + "!"
来源：http://www.ydjk.org.cn/Article/details/gt3seddapap.html

[T10] Kotlin：默认参数
来源：http://www.52xcode.cn/Article/details/gt3gynipsic.html

fun greet(name: String = "World") = "Hi $name"
来源：http://www.52xcode.cn/Article/details/gt3fdwybnqp.html

[T11] Kotlin：协程
来源：http://www.ydjk.org.cn/Article/details/gt3zspnlphm.html

GlobalScope.launch { delay(1000); println("done") }
来源：http://www.52xcode.cn/Article/details/gt3uutjshbe.html

[T12] Kotlin：解构声明
来源：http://www.52xcode.cn/Article/details/gt3titiojzc.html

val (a, b) = Pair(1, 2)
来源：http://www.ydjk.org.cn/Article/details/gt3nezsdfel.html

[T13] Kotlin：只读 Map
来源：http://www.52xcode.cn/Article/details/gt3nknifyak.html

val m = mapOf("a" to 1)
来源：http://www.52xcode.cn/Article/details/gt3jdofseko.html

[T14] Kotlin：循环
来源：http://www.ydjk.org.cn/Article/details/gt3lbhtvboz.html

for (i in 1..10) println(i)
来源：http://www.ydjk.org.cn/Article/details/gt3egqxakhd.html

[T15] Kotlin：接口
来源：http://www.52xcode.cn/Article/details/gt3aoxuopec.html

interface Shape { fun area(): Double }
来源：http://www.ydjk.org.cn/Article/details/gt3ennolvxo.html

[T16] Swift：Hello World
来源：http://www.ydjk.org.cn/Article/details/gt3jhqxklxj.html

print("Hello")
来源：http://www.ydjk.org.cn/Article/details/gt3wpueyaxj.html

[T17] Swift：变量与常量
来源：http://www.52xcode.cn/Article/details/gt3hgxpxpgi.html

var a = 1;  let b = 2
来源：http://www.52xcode.cn/Article/details/gt3akpbfqhe.html

[T18] Swift：字符串插值
来源：http://www.ydjk.org.cn/Article/details/gt3galdwnlf.html

"值: \(b)"
来源：http://www.52xcode.cn/Article/details/gt3uckvmevg.html

[T19] Swift：可选绑定
来源：http://www.52xcode.cn/Article/details/gt3adqdwihn.html

if let n = opt { print(n) }
来源：http://www.ydjk.org.cn/Article/details/gt3aketwath.html

[T20] Swift：数组操作
来源：http://www.52xcode.cn/Article/details/gt3hixeblzu.html

var a = [1, 2, 3];  a.append(4)
来源：http://www.52xcode.cn/Article/details/gt3oxnyvydb.html

[T21] Swift：遍历
来源：http://www.52xcode.cn/Article/details/gt3lmjlpavh.html

for x in a { print(x) }
来源：http://www.52xcode.cn/Article/details/gt3hxzrbapp.html

[T22] Swift：字典
来源：http://www.ydjk.org.cn/Article/details/gt3hoburfdd.html

var d = ["a": 1];  d["b"] = 2
来源：http://www.52xcode.cn/Article/details/gt3fodoaeyx.html

[T23] Swift：函数
来源：http://www.52xcode.cn/Article/details/gt3vtvcwhnu.html

func add(_ a: Int, _ b: Int) -> Int { a + b }
来源：http://www.ydjk.org.cn/Article/details/gt3imafkcvf.html

[T24] Swift：闭包
来源：http://www.52xcode.cn/Article/details/gt3jqzspjis.html

let f = { (x: Int) -> Int in x * 2 }
来源：http://www.ydjk.org.cn/Article/details/gt3jnytqpfb.html

[T25] Swift：结构体
来源：http://www.52xcode.cn/Article/details/gt3zxnlitav.html

struct P { var x: Int }
来源：http://www.52xcode.cn/Article/details/gt3crrffruf.html

[T26] Swift：类与重写
来源：http://www.52xcode.cn/Article/details/gt3mhoauttf.html

class A: Base { override func f() {} }
来源：http://www.52xcode.cn/Article/details/gt3xtmdtoyz.html

[T27] Swift：错误处理
来源：http://www.52xcode.cn/Article/details/gt3dikjbjkr.html

do { try f() } catch { print(error) }
来源：http://www.ydjk.org.cn/Article/details/gt3cslnypuu.html

[T28] Swift：枚举
来源：http://www.ydjk.org.cn/Article/details/gt3fpxthoax.html

enum Color { case red, green }
来源：http://www.52xcode.cn/Article/details/gt3fbpqryyd.html

[T29] Swift：guard 提前返回
来源：http://www.52xcode.cn/Article/details/gt3uqjeehcb.html

guard let x = opt else { return }
来源：http://www.52xcode.cn/Article/details/gt3sokzelxl.html

[T30] Swift：协议
来源：http://www.52xcode.cn/Article/details/gt3xbwendsn.html

protocol Shape { func area() -> Double }
来源：http://www.ydjk.org.cn/Article/details/gt3ohydapxy.html

[T31] Lua：Hello World
来源：http://www.52xcode.cn/Article/details/gt3rlhgsusc.html

print("Hello")
来源：http://www.ydjk.org.cn/Article/details/gt3uthibzea.html

[T32] Lua：局部变量
来源：http://www.52xcode.cn/Article/details/gt3kdcpfbvv.html

local a = 1
来源：http://www.52xcode.cn/Article/details/gt3fkyzabdx.html

[T33] Lua：表（数组）
来源：http://www.52xcode.cn/Article/details/gt3iyrugsqm.html

local t = {1, 2, 3};  t[4] = 4
来源：http://www.52xcode.cn/Article/details/gt3yklneudu.html

[T34] Lua：遍历表
来源：http://www.ydjk.org.cn/Article/details/gt3fqdrvyxf.html

for i, v in ipairs(t) do print(i, v) end
来源：http://www.ydjk.org.cn/Article/details/gt3kbvztkzb.html

[T35] Lua：字典表
来源：http://www.ydjk.org.cn/Article/details/gt3bajzqbfu.html

local d = { a = 1 };  d.b = 2
来源：http://www.52xcode.cn/Article/details/gt3yfbqxmcy.html

[T36] Lua：函数
来源：http://www.52xcode.cn/Article/details/gt3ogcgrhvt.html

function add(a, b) return a + b end
来源：http://www.52xcode.cn/Article/details/gt3tmnvivdg.html

[T37] Lua：字符串拼接
来源：http://www.52xcode.cn/Article/details/gt3bdkqdtcc.html

"a" .. "b"
来源：http://www.52xcode.cn/Article/details/gt3cjpbkyzt.html

[T38] Lua：条件
来源：http://www.52xcode.cn/Article/details/gt3khwsjglk.html

if x > 0 then print("正") end
来源：http://www.ydjk.org.cn/Article/details/gt3lfrhbtvn.html

[T39] Lua：模式匹配
来源：http://www.ydjk.org.cn/Article/details/gt3peohyzww.html

string.find(s, "%d+")
来源：http://www.ydjk.org.cn/Article/details/gt3dyjyfxyf.html

[T40] Lua：元表
来源：http://www.52xcode.cn/Article/details/gt3npcqmjeh.html

setmetatable({}, { __index = base })
来源：http://www.52xcode.cn/Article/details/gt3oswcyicp.html

[T41] Perl：Hello World
来源：http://www.52xcode.cn/Article/details/gt3jzbciune.html

print "Hello\n";
来源：http://www.52xcode.cn/Article/details/gt3iejzuusb.html

[T42] Perl：变量类型
来源：http://www.52xcode.cn/Article/details/gt3zwnrnljk.html

my $a = 1;  my @arr = (1, 2, 3);  my %h = (a => 1);
来源：http://www.52xcode.cn/Article/details/gt3exnrubjx.html

[T43] Perl：字符串插值
来源：http://www.ydjk.org.cn/Article/details/gt3xpygvglw.html

"值: $a"
来源：http://www.ydjk.org.cn/Article/details/gt3zxuwhvpa.html

[T44] Perl：条件
来源：http://www.52xcode.cn/Article/details/gt3nqxdczbr.html

if ($a > 0) { print "正"; }
来源：http://www.52xcode.cn/Article/details/gt3lzacblhu.html

[T45] Perl：数组遍历
来源：http://www.52xcode.cn/Article/details/gt3qkixahhn.html

for my $x (@arr) { print $x; }
来源：http://www.ydjk.org.cn/Article/details/gt3mudlrqiu.html

[T46] Perl：哈希操作
来源：http://www.ydjk.org.cn/Article/details/gt3hbszovaw.html

$h{b} = 2;  for my $k (keys %h) { print "$k=$h{$k}"; }
来源：http://www.52xcode.cn/Article/details/gt3ehvzawgy.html

[T47] Perl：正则捕获
来源：http://www.ydjk.org.cn/Article/details/gt3qrypptgi.html

if ($s =~ /(\d+)/) { print $1; }
来源：http://www.ydjk.org.cn/Article/details/gt3mtufkphn.html

[T48] Perl：正则替换
来源：http://www.ydjk.org.cn/Article/details/gt3eaekkmdh.html

$s =~ s/old/new/g;
来源：http://www.ydjk.org.cn/Article/details/gt3rhbvcyzr.html

[T49] Perl：函数
来源：http://www.ydjk.org.cn/Article/details/gt3kgvawxfi.html

sub add { my ($a, $b) = @_; return $a + $b; }
来源：http://www.52xcode.cn/Article/details/gt3lpydljjl.html

[T50] Perl：逐行读文件
来源：http://www.ydjk.org.cn/Article/details/gt3kqtwmmcc.html

open my $fh, "<", "a.txt" or die $!;
来源：http://www.ydjk.org.cn/Article/details/gt3rgvcxxxm.html

while (my $line = <$fh>) { print $line; }
来源：http://www.52xcode.cn/Article/details/gt3znznfrvy.html

[T51] Scala：Hello World
来源：http://www.52xcode.cn/Article/details/gt3juhvsoga.html

println("Hello")
来源：http://www.52xcode.cn/Article/details/gt3lifeajdd.html

[T52] Scala：变量
来源：http://www.ydjk.org.cn/Article/details/gt3tsznpkey.html

val a = 1;  var b = 2
来源：http://www.ydjk.org.cn/Article/details/gt3lmiyezpg.html

[T53] Scala：字符串插值
来源：http://www.ydjk.org.cn/Article/details/gt3gqczslur.html

s"值: $b"
来源：http://www.ydjk.org.cn/Article/details/gt3qyztvitn.html

[T54] Scala：集合映射
来源：http://www.52xcode.cn/Article/details/gt3khwhrcfi.html

List(1, 2, 3).map(_ * 2)
来源：http://www.ydjk.org.cn/Article/details/gt3qjhfzhuv.html

[T55] Scala：集合过滤
来源：http://www.ydjk.org.cn/Article/details/gt3fogrmqkd.html

List(1, 2, 3).filter(_ > 1)
来源：http://www.52xcode.cn/Article/details/gt3tuwwuwzx.html

[T56] Scala：样例类
来源：http://www.ydjk.org.cn/Article/details/gt3tlpfnsbt.html

case class User(name: String, age: Int)
来源：http://www.52xcode.cn/Article/details/gt3olvjicbm.html

[T57] Scala：模式匹配
来源：http://www.52xcode.cn/Article/details/gt3tmlclviy.html

x match { case 1 => "一"; case _ => "其他" }
来源：http://www.52xcode.cn/Article/details/gt3zlolgkpk.html

[T58] Scala：函数定义
来源：http://www.ydjk.org.cn/Article/details/gt3bytkalry.html

def add(a: Int, b: Int): Int = a + b
来源：http://www.52xcode.cn/Article/details/gt3xnpjpzkz.html

[T59] Scala：循环
来源：http://www.52xcode.cn/Article/details/gt3cfzapnkq.html

for (i <- 1 to 10) println(i)
来源：http://www.52xcode.cn/Article/details/gt3lxirxlvw.html

[T60] Scala：折叠
来源：http://www.52xcode.cn/Article/details/gt3bvczswzf.html

List(1, 2, 3).foldLeft(0)(_ + _)
来源：http://www.52xcode.cn/Article/details/gt3veyfccqh.html

================================================================================
来源：http://www.ydjk.org.cn/Article/details/gt3jqlhdcop.html

U. 高频实用片段（Python / PHP / JavaScript 各 40 条）
来源：http://www.ydjk.org.cn/Article/details/gt3lwxpkdtb.html

================================================================================
来源：http://www.52xcode.cn/Article/details/gt3ukoowgco.html

[U01] Py：创建虚拟环境
来源：http://www.52xcode.cn/Article/details/gt3projsjjk.html

python -m venv .venv && source .venv/bin/activate
来源：http://www.52xcode.cn/Article/details/gt3vompavbh.html

[U02] Py：导出 / 安装依赖
来源：http://www.52xcode.cn/Article/details/gt3hdtmehyk.html

pip freeze > requirements.txt;  pip install -r requirements.txt
来源：http://www.ydjk.org.cn/Article/details/gt3ygaqexgj.html

[U03] Py：加载 .env 配置
来源：http://www.ydjk.org.cn/Article/details/gt3azozxcuw.html

from dotenv import load_dotenv; load_dotenv()
来源：http://www.ydjk.org.cn/Article/details/gt3gffquida.html

[U04] Py：变量调试打印
来源：http://www.ydjk.org.cn/Article/details/gt3phkvmhsd.html

print(f"{x=}")            # 输出 x=值，Python 3.8+
来源：http://www.52xcode.cn/Article/details/gt3ngvqitje.html

[U05] Py：列表去重且保序
来源：http://www.ydjk.org.cn/Article/details/gt3cqievevk.html

list(dict.fromkeys(arr))
来源：http://www.ydjk.org.cn/Article/details/gt3snqyfzuk.html

[U06] Py：合并两个字典
来源：http://www.52xcode.cn/Article/details/gt3hwlbmlmw.html

{**a, **b}
来源：http://www.52xcode.cn/Article/details/gt3iqanlfjo.html

[U07] Py：反转字典键值
来源：http://www.52xcode.cn/Article/details/gt3ebihexyi.html

{v: k for k, v in d.items()}
来源：http://www.52xcode.cn/Article/details/gt3sohunyqo.html

[U08] Py：展平二维列表
来源：http://www.ydjk.org.cn/Article/details/gt3qrnrhrgz.html

[y for x in nested for y in x]
来源：http://www.ydjk.org.cn/Article/details/gt3xvjirzzu.html

[U09] Py：字典取最大值的键
来源：http://www.52xcode.cn/Article/details/gt3heoabzcs.html

max(d, key=d.get)
来源：http://www.52xcode.cn/Article/details/gt3mpmwyspx.html

[U10] Py：按值排序字典
来源：http://www.ydjk.org.cn/Article/details/gt3jqxtygoz.html

dict(sorted(d.items(), key=lambda kv: kv[1]))
来源：http://www.52xcode.cn/Article/details/gt3irbtjjrg.html

[U11] Py：生成器表达式
来源：http://www.52xcode.cn/Article/details/gt3bvydiotu.html

(x * 2 for x in arr)
来源：http://www.52xcode.cn/Article/details/gt3tgzrocvh.html

[U12] Py：取出现最多的 3 个元素
来源：http://www.ydjk.org.cn/Article/details/gt3cazznaiz.html

Counter(arr).most_common(3)
来源：http://www.52xcode.cn/Article/details/gt3rasxzmeq.html

[U13] Py：固定长度队列
来源：http://www.ydjk.org.cn/Article/details/gt3itncelej.html

deque(maxlen=10)
来源：http://www.ydjk.org.cn/Article/details/gt3yqpitqvd.html

[U14] Py：分组收集到列表
来源：http://www.ydjk.org.cn/Article/details/gt3zfbfvmic.html

defaultdict(list)
来源：http://www.52xcode.cn/Article/details/gt3qhpwyaty.html

[U15] Py：高精度计时
来源：http://www.52xcode.cn/Article/details/gt3shoubqzf.html

t = time.perf_counter()
来源：http://www.52xcode.cn/Article/details/gt3hmznbrur.html

[U16] Py：命令行参数解析
来源：http://www.ydjk.org.cn/Article/details/gt3klaunfgu.html

ap = argparse.ArgumentParser();  ap.add_argument("--name");  args = ap.parse_args()
来源：http://www.52xcode.cn/Article/details/gt3eebubetx.html

[U17] Py：初始化日志
来源：http://www.ydjk.org.cn/Article/details/gt3ekxebxgx.html

logging.basicConfig(level=logging.INFO)
来源：http://www.ydjk.org.cn/Article/details/gt3igobxasj.html

[U18] Py：预编译正则
来源：http://www.52xcode.cn/Article/details/gt3aiildori.html

pat = re.compile(r"\d+")
来源：http://www.52xcode.cn/Article/details/gt3hqishtfs.html

[U19] Py：正则替换带回调
来源：http://www.ydjk.org.cn/Article/details/gt3eudrkcgq.html

re.sub(r"\d+", lambda m: str(int(m.group()) * 2), s)
来源：http://www.52xcode.cn/Article/details/gt3cuubbumu.html

[U20] Py：缓存函数结果
来源：http://www.52xcode.cn/Article/details/gt3hejhpccd.html

@functools.lru_cache(maxsize=None)
来源：http://www.ydjk.org.cn/Article/details/gt3ifhmtvcx.html

[U21] Py：自定义上下文管理器
来源：http://www.52xcode.cn/Article/details/gt3dwgwbcmt.html

@contextlib.contextmanager
来源：http://www.ydjk.org.cn/Article/details/gt3cvhqywyt.html

[U22] Py：矩阵转置
来源：http://www.52xcode.cn/Article/details/gt3xatvgbqg.html

list(zip(*m))
来源：http://www.ydjk.org.cn/Article/details/gt3xwsdfiod.html

[U23] Py：分块读取大文件
来源：http://www.52xcode.cn/Article/details/gt3rrtgwzgn.html

for chunk in iter(lambda: f.read(8192), b""):
来源：http://www.ydjk.org.cn/Article/details/gt3moxwtqma.html

[U24] Py：路径操作
来源：http://www.52xcode.cn/Article/details/gt3jsgpufhf.html

Path("a/b.txt").parent.mkdir(parents=True, exist_ok=True)
来源：http://www.52xcode.cn/Article/details/gt3hzpgwxsc.html

[U25] Py：CSV 按字典读
来源：http://www.52xcode.cn/Article/details/gt3kbucpnah.html

csv.DictReader(f)
来源：http://www.52xcode.cn/Article/details/gt3mfvzpkke.html

[U26] Py：并发下载
来源：http://www.ydjk.org.cn/Article/details/gt3uymsviqw.html

ThreadPoolExecutor(max_workers=8).map(fetch, urls)
来源：http://www.ydjk.org.cn/Article/details/gt3ktlajrdf.html

[U27] Py：异步 HTTP
来源：http://www.ydjk.org.cn/Article/details/gt3yvqtpvdo.html

aiohttp.ClientSession() 配合 async with
来源：http://www.52xcode.cn/Article/details/gt3ytdyulmx.html

[U28] Py：类型别名
来源：http://www.52xcode.cn/Article/details/gt3kvmxvixw.html

UserId = int
来源：http://www.52xcode.cn/Article/details/gt3pjiwqzux.html

[U29] Py：属性校验
来源：http://www.ydjk.org.cn/Article/details/gt3yzjymcah.html

@property 与 @x.setter 配合
来源：http://www.ydjk.org.cn/Article/details/gt3frstvkvq.html

[U30] Py：数据类
来源：http://www.ydjk.org.cn/Article/details/gt3rfugyumh.html

@dataclass(slots=True)
来源：http://www.52xcode.cn/Article/details/gt3anwxeagr.html

[U31] Py：单测
来源：http://www.52xcode.cn/Article/details/gt3kvmgizhd.html

python -m pytest -q
来源：http://www.52xcode.cn/Article/details/gt3xdxrxkfa.html

[U32] Py：代码格式化
来源：http://www.ydjk.org.cn/Article/details/gt3wzysiidu.html

ruff format . && ruff check --fix .
来源：http://www.52xcode.cn/Article/details/gt3entnzell.html

[U33] Py：打包发布
来源：http://www.ydjk.org.cn/Article/details/gt3bmikbdqi.html

python -m build  （依赖 pyproject.toml）
来源：http://www.52xcode.cn/Article/details/gt3cuctedea.html

[U34] Py：判断编码
来源：http://www.52xcode.cn/Article/details/gt3pbjmmpmy.html

chardet.detect(raw)
来源：http://www.52xcode.cn/Article/details/gt3ytcdaueq.html

[U35] Py：发送邮件
来源：http://www.52xcode.cn/Article/details/gt3xbwzsang.html

smtplib.SMTP_SSL(...).send_message(msg)
来源：http://www.52xcode.cn/Article/details/gt3xbofvsio.html

[U36] Py：定时任务
来源：http://www.ydjk.org.cn/Article/details/gt3odelfkgt.html

schedule.every(10).minutes.do(job)
来源：http://www.52xcode.cn/Article/details/gt3bozubiwt.html

[U37] Py：读写 Excel
来源：http://www.52xcode.cn/Article/details/gt3fhjqihkd.html

pandas.read_excel / DataFrame.to_excel
来源：http://www.ydjk.org.cn/Article/details/gt3sbhbgplo.html

[U38] Py：获取脚本所在目录
来源：http://www.52xcode.cn/Article/details/gt3qlgfokct.html

Path(__file__).resolve().parent
来源：http://www.ydjk.org.cn/Article/details/gt3fxxbtwuf.html

[U39] Py：判断是否在交互环境
来源：http://www.52xcode.cn/Article/details/gt3idlwbllm.html

sys.stdout.isatty()
来源：http://www.52xcode.cn/Article/details/gt3kqilwywv.html

[U40] Py：打印到标准错误
来源：http://www.ydjk.org.cn/Article/details/gt3crcgxjcb.html

print("err", file=sys.stderr)
来源：http://www.ydjk.org.cn/Article/details/gt3qeoqfnof.html

[U41] PHP：初始化 Composer 项目
来源：http://www.ydjk.org.cn/Article/details/gt3pluuvcrv.html

composer init;  composer require guzzlehttp/guzzle
来源：http://www.ydjk.org.cn/Article/details/gt3srmibepb.html

[U42] PHP：PSR-4 自动加载
来源：http://www.ydjk.org.cn/Article/details/gt3jeenrzws.html

"autoload": { "psr-4": { "App\\": "src/" } }
来源：http://www.52xcode.cn/Article/details/gt3uhfymgfo.html

[U43] PHP：声明命名空间
来源：http://www.ydjk.org.cn/Article/details/gt3mmzgovlu.html

namespace App\Http;
来源：http://www.52xcode.cn/Article/details/gt3sfkepofp.html

[U44] PHP：开启严格类型
来源：http://www.52xcode.cn/Article/details/gt3urathytn.html

declare(strict_types=1);
来源：http://www.52xcode.cn/Article/details/gt3hugrdouu.html

[U45] PHP：类型声明与返回类型
来源：http://www.52xcode.cn/Article/details/gt3curbfvcg.html

function add(int $a, int $b): int { return $a + $b; }
来源：http://www.52xcode.cn/Article/details/gt3jeimgqnz.html

[U46] PHP：可空类型
来源：http://www.52xcode.cn/Article/details/gt3wcdyflyu.html

?string $name = null
来源：http://www.ydjk.org.cn/Article/details/gt3abccuahm.html

[U47] PHP：联合类型
来源：http://www.52xcode.cn/Article/details/gt3yndipvlw.html

int|string $id
来源：http://www.52xcode.cn/Article/details/gt3ceevxdaf.html

[U48] PHP：纯枚举
来源：http://www.ydjk.org.cn/Article/details/gt3cgyqtkyj.html

enum Status: string { case Active = "active"; case Off = "off"; }
来源：http://www.52xcode.cn/Article/details/gt3kkqwojpx.html

[U49] PHP：只读属性
来源：http://www.52xcode.cn/Article/details/gt3tisfnrhy.html

public readonly string $name
来源：http://www.52xcode.cn/Article/details/gt3aastvgdm.html

[U50] PHP：构造器属性提升
来源：http://www.52xcode.cn/Article/details/gt3uflnckri.html

public function __construct(private int $id) {}
来源：http://www.52xcode.cn/Article/details/gt3gpcorbkr.html

[U51] PHP：数组解构
来源：http://www.ydjk.org.cn/Article/details/gt3udzmctrb.html

[$a, $b] = $arr;
来源：http://www.52xcode.cn/Article/details/gt3fekpphpm.html

[U52] PHP：箭头函数
来源：http://www.ydjk.org.cn/Article/details/gt3mlehoimd.html

$double = fn($x) => $x * 2;
来源：http://www.ydjk.org.cn/Article/details/gt3cymqelwl.html

[U53] PHP：空合并运算符
来源：http://www.ydjk.org.cn/Article/details/gt3ptbgexwk.html

$v = $a ?? $b ?? "default";
来源：http://www.52xcode.cn/Article/details/gt3beorwfkn.html

[U54] PHP：空安全调用
来源：http://www.ydjk.org.cn/Article/details/gt3eqikmpup.html

$obj?->method()
来源：http://www.ydjk.org.cn/Article/details/gt3nqeeojit.html

[U55] PHP：match 表达式
来源：http://www.ydjk.org.cn/Article/details/gt3tfpvbwzh.html

$s = match($x) { 1 => "一", default => "其他" };
来源：http://www.ydjk.org.cn/Article/details/gt3gxhbjvmv.html

[U56] PHP：命名参数
来源：http://www.ydjk.org.cn/Article/details/gt3bnrznoxn.html

f(a: 1, b: 2)
来源：http://www.ydjk.org.cn/Article/details/gt3bsqqtaxh.html

[U57] PHP：字符串插值
来源：http://www.ydjk.org.cn/Article/details/gt3dyxidloo.html

"值: {$a}"
来源：http://www.52xcode.cn/Article/details/gt3tozwoufp.html

[U58] PHP：数组三件套
来源：http://www.52xcode.cn/Article/details/gt3ubndwkat.html

array_map($f, $a);  array_filter($a, $f);  array_reduce($a, $f, 0);
来源：http://www.ydjk.org.cn/Article/details/gt3giwvmzrj.html

[U59] PHP：自定义排序
来源：http://www.52xcode.cn/Article/details/gt3xuxctkgp.html

usort($arr, fn($a, $b) => $a["age"] <=> $b["age"]);
来源：http://www.52xcode.cn/Article/details/gt3csddzohk.html

[U60] PHP：JSON 编解码
来源：http://www.ydjk.org.cn/Article/details/gt3mxhgebpi.html

json_encode($d, JSON_UNESCAPED_UNICODE);  json_decode($s, true);
来源：http://www.52xcode.cn/Article/details/gt3eduobfhr.html

[U61] PHP：正则
来源：http://www.52xcode.cn/Article/details/gt3xwhzowsr.html

preg_match('/(\d+)/', $s, $m);  preg_replace('/\d+/', '#', $s);
来源：http://www.52xcode.cn/Article/details/gt3tyapwofh.html

[U62] PHP：日期对象
来源：http://www.ydjk.org.cn/Article/details/gt3glunvxlo.html

(new DateTimeImmutable())->format("Y-m-d");
来源：http://www.52xcode.cn/Article/details/gt3tjidvczd.html

[U63] PHP：文件读写
来源：http://www.52xcode.cn/Article/details/gt3kzgiwfey.html

file_get_contents($f);  file_put_contents($f, $data);
来源：http://www.ydjk.org.cn/Article/details/gt3fvriwhim.html

[U64] PHP：目录遍历
来源：http://www.52xcode.cn/Article/details/gt3laduvxye.html

glob("dir/*.php");  scandir("dir");
来源：http://www.ydjk.org.cn/Article/details/gt3fqjgsgao.html

[U65] PHP：会话
来源：http://www.ydjk.org.cn/Article/details/gt3uolgowqq.html

session_start();  $_SESSION["uid"] = 1;
来源：http://www.52xcode.cn/Article/details/gt3svbhybdn.html

[U66] PHP：设置 Cookie
来源：http://www.52xcode.cn/Article/details/gt3pfjwppdd.html

setcookie("token", $v, ["httponly" => true, "samesite" => "Lax"]);
来源：http://www.ydjk.org.cn/Article/details/gt3gxjwiurv.html

[U67] PHP：处理文件上传
来源：http://www.ydjk.org.cn/Article/details/gt3tlolaexx.html

$_FILES["file"]["tmp_name"] 与 move_uploaded_file()
来源：http://www.ydjk.org.cn/Article/details/gt3njkcnutg.html

[U68] PHP：PDO 连接
来源：http://www.ydjk.org.cn/Article/details/gt3bqeacizb.html

$pdo = new PDO("mysql:host=localhost;dbname=app", "root", "");
来源：http://www.52xcode.cn/Article/details/gt3qouearlv.html

[U69] PHP：PDO 预处理
来源：http://www.ydjk.org.cn/Article/details/gt3owtmaizs.html

$stmt = $pdo->prepare("SELECT * FROM users WHERE id = ?");  $stmt->execute([$id]);
来源：http://www.52xcode.cn/Article/details/gt3eysedmcr.html

[U70] PHP：PDO 事务
来源：http://www.52xcode.cn/Article/details/gt3gugcfvux.html

$pdo->beginTransaction();  $pdo->commit();  $pdo->rollBack();
来源：http://www.52xcode.cn/Article/details/gt3stpovthy.html

[U71] PHP：抛出异常
来源：http://www.ydjk.org.cn/Article/details/gt3ropaqpau.html

throw new RuntimeException("失败", 500);
来源：http://www.ydjk.org.cn/Article/details/gt3fkssmzrr.html

[U72] PHP：写错误日志
来源：http://www.52xcode.cn/Article/details/gt3bcxtrhof.html

error_log("失败: " . $e->getMessage());
来源：http://www.52xcode.cn/Article/details/gt3mlbbpxjm.html

[U73] PHP：读取 ini 配置
来源：http://www.52xcode.cn/Article/details/gt3kjcvtljv.html

parse_ini_file("config.ini", true)
来源：http://www.ydjk.org.cn/Article/details/gt3chajigtu.html

[U74] PHP：读取环境变量
来源：http://www.52xcode.cn/Article/details/gt3umkanspk.html

getenv("APP_ENV") ?: "production"
来源：http://www.52xcode.cn/Article/details/gt3tojixapb.html

[U75] PHP：依赖注入
来源：http://www.ydjk.org.cn/Article/details/gt3gvxtccgq.html

composer require psr/container
来源：http://www.52xcode.cn/Article/details/gt3ihmelldj.html

[U76] PHP：简单路由
来源：http://www.ydjk.org.cn/Article/details/gt3lsjelumc.html

$path = parse_url($_SERVER["REQUEST_URI"], PHP_URL_PATH);
来源：http://www.52xcode.cn/Article/details/gt3jhmikpnc.html

[U77] PHP：模板渲染
来源：http://www.ydjk.org.cn/Article/details/gt3zmnvgwsr.html

composer require twig/twig
来源：http://www.ydjk.org.cn/Article/details/gt3rqeijxkr.html

[U78] PHP：单元测试
来源：http://www.52xcode.cn/Article/details/gt3fxmsishd.html

composer require --dev phpunit/phpunit
来源：http://www.ydjk.org.cn/Article/details/gt3jbjhnmtq.html

[U79] PHP：静态分析
来源：http://www.ydjk.org.cn/Article/details/gt3rofdrznm.html

composer require --dev phpstan/phpstan
来源：http://www.ydjk.org.cn/Article/details/gt3gupcxbtq.html

[U80] PHP：代码规范修复
来源：http://www.52xcode.cn/Article/details/gt3luwawywv.html

composer require --dev friendsofphp/php-cs-fixer
来源：http://www.52xcode.cn/Article/details/gt3krpgkhek.html

[U81] JS：初始化项目
来源：http://www.52xcode.cn/Article/details/gt3rmikinex.html

npm init -y;  npm i express
来源：http://www.ydjk.org.cn/Article/details/gt3irqhaemu.html

[U82] JS：package.json 脚本
来源：http://www.52xcode.cn/Article/details/gt3ijpmjjno.html

"scripts": { "dev": "vite", "build": "vite build" }
来源：http://www.52xcode.cn/Article/details/gt3ksbeftbn.html

[U83] JS：ES Module 导入导出
来源：http://www.ydjk.org.cn/Article/details/gt3ztbrmzss.html

export const a = 1;  import { a } from "./m.js";
来源：http://www.52xcode.cn/Article/details/gt3ttdhjmmh.html

[U84] JS：CommonJS 写法
来源：http://www.52xcode.cn/Article/details/gt3ldlaufpj.html

module.exports = { a };  const { a } = require("./m");
来源：http://www.52xcode.cn/Article/details/gt3pyqqdtqc.html

[U85] JS：可选链
来源：http://www.ydjk.org.cn/Article/details/gt3akdyeovl.html

a?.b?.c
来源：http://www.ydjk.org.cn/Article/details/gt3psfdeqim.html

[U86] JS：空值合并
来源：http://www.ydjk.org.cn/Article/details/gt3aiuxklfd.html

a ?? b
来源：http://www.52xcode.cn/Article/details/gt3jqbjgkkl.html

[U87] JS：解构默认值
来源：http://www.ydjk.org.cn/Article/details/gt3jsgwobqe.html

const { a = 1, b = 2 } = obj;
来源：http://www.ydjk.org.cn/Article/details/gt3enygkrkr.html

[U88] JS：对象展开合并
来源：http://www.ydjk.org.cn/Article/details/gt3duqkebjf.html

{ ...a, ...b }
来源：http://www.ydjk.org.cn/Article/details/gt3owgxgidl.html

[U89] JS：数组去重
来源：http://www.ydjk.org.cn/Article/details/gt3wpzycmww.html

[...new Set(arr)]
来源：http://www.ydjk.org.cn/Article/details/gt3eptorrzi.html

[U90] JS：数字数组排序
来源：http://www.ydjk.org.cn/Article/details/gt3cjggkrdu.html

[...arr].sort((a, b) => a - b)
来源：http://www.52xcode.cn/Article/details/gt3zgypkwol.html

[U91] JS：对象键值遍历
来源：http://www.52xcode.cn/Article/details/gt3drfzpaoh.html

Object.entries(obj).forEach(([k, v]) => {});
来源：http://www.ydjk.org.cn/Article/details/gt3xtmpqkab.html

[U92] JS：深拷贝
来源：http://www.ydjk.org.cn/Article/details/gt3xlchnouo.html

structuredClone(obj)
来源：http://www.ydjk.org.cn/Article/details/gt3jdmcrciw.html

[U93] JS：模板字符串
来源：http://www.52xcode.cn/Article/details/gt3qghnvxfs.html

`共 ${n} 条`
来源：http://www.52xcode.cn/Article/details/gt3lylvmtad.html

[U94] JS：箭头函数
来源：http://www.ydjk.org.cn/Article/details/gt3nqpfhgeq.html

const double = x => x * 2;
来源：http://www.ydjk.org.cn/Article/details/gt3hkjundky.html

[U95] JS：Promise 包装
来源：http://www.52xcode.cn/Article/details/gt3whdteowe.html

new Promise((resolve, reject) => {})
来源：http://www.ydjk.org.cn/Article/details/gt3evwfashd.html

[U96] JS：async/await 与异常
来源：http://www.52xcode.cn/Article/details/gt3cousajpx.html

try { const d = await f(); } catch (e) { console.error(e); }
来源：http://www.ydjk.org.cn/Article/details/gt3rgxvswpj.html


<!-- 参考信息 -->