代发 wailian999

[T13] Kotlin：只读 Map
来源：http://www.52xcode.cn/Article/details/gt3vptdnduj.html

val m = mapOf("a" to 1)
来源：http://www.52xcode.cn/Article/details/gt3rwovtite.html

[T14] Kotlin：循环
来源：http://www.ydjk.org.cn/Article/details/gt3xazxplft.html

for (i in 1..10) println(i)
来源：http://www.52xcode.cn/Article/details/gt3gyssbvvv.html

[T15] Kotlin：接口
来源：http://www.ydjk.org.cn/Article/details/gt3sxcbwuma.html

interface Shape { fun area(): Double }
来源：http://www.52xcode.cn/Article/details/gt3glvzklcl.html

[T16] Swift：Hello World
来源：http://www.ydjk.org.cn/Article/details/gt3wawxfntq.html

print("Hello")
来源：http://www.ydjk.org.cn/Article/details/gt3vdhytgwf.html

[T17] Swift：变量与常量
来源：http://www.ydjk.org.cn/Article/details/gt3kqqrcfyz.html

var a = 1;  let b = 2
来源：http://www.ydjk.org.cn/Article/details/gt3wdivpmus.html

[T18] Swift：字符串插值
来源：http://www.52xcode.cn/Article/details/gt3jztfwmqm.html

"值: \(b)"
来源：http://www.52xcode.cn/Article/details/gt3oyahwawn.html

[T19] Swift：可选绑定
来源：http://www.52xcode.cn/Article/details/gt3qrhxlzde.html

if let n = opt { print(n) }
来源：http://www.ydjk.org.cn/Article/details/gt3hqgybjoa.html

[T20] Swift：数组操作
来源：http://www.ydjk.org.cn/Article/details/gt3drvmxqdp.html

var a = [1, 2, 3];  a.append(4)
来源：http://www.52xcode.cn/Article/details/gt3bnunqgwe.html

[T21] Swift：遍历
来源：http://www.52xcode.cn/Article/details/gt3kawxbxse.html

for x in a { print(x) }
来源：http://www.52xcode.cn/Article/details/gt3crtelfrr.html

[T22] Swift：字典
来源：http://www.52xcode.cn/Article/details/gt3nfzlxqil.html

var d = ["a": 1];  d["b"] = 2
来源：http://www.ydjk.org.cn/Article/details/gt3qxojaghv.html

[T23] Swift：函数
来源：http://www.ydjk.org.cn/Article/details/gt3ptzflauu.html

func add(_ a: Int, _ b: Int) -> Int { a + b }
来源：http://www.52xcode.cn/Article/details/gt3twbbhqdi.html

[T24] Swift：闭包
来源：http://www.52xcode.cn/Article/details/gt3kjidawnh.html

let f = { (x: Int) -> Int in x * 2 }
来源：http://www.ydjk.org.cn/Article/details/gt3piwxfjvr.html

[T25] Swift：结构体
来源：http://www.52xcode.cn/Article/details/gt3uowbajrn.html

struct P { var x: Int }
来源：http://www.52xcode.cn/Article/details/gt3bqyxyndd.html

[T26] Swift：类与重写
来源：http://www.52xcode.cn/Article/details/gt3zyledxce.html

class A: Base { override func f() {} }
来源：http://www.ydjk.org.cn/Article/details/gt3zpzkhgkt.html

[T27] Swift：错误处理
来源：http://www.ydjk.org.cn/Article/details/gt3ugmlniia.html

do { try f() } catch { print(error) }
来源：http://www.52xcode.cn/Article/details/gt3kvjzbaex.html

[T28] Swift：枚举
来源：http://www.52xcode.cn/Article/details/gt3guprknfp.html

enum Color { case red, green }
来源：http://www.ydjk.org.cn/Article/details/gt3ouoesrob.html

[T29] Swift：guard 提前返回
来源：http://www.ydjk.org.cn/Article/details/gt3loredvee.html

guard let x = opt else { return }
来源：http://www.ydjk.org.cn/Article/details/gt3bytnislg.html

[T30] Swift：协议
来源：http://www.52xcode.cn/Article/details/gt3qfbobitb.html

protocol Shape { func area() -> Double }
来源：http://www.52xcode.cn/Article/details/gt3mkofxplx.html

[T31] Lua：Hello World
来源：http://www.52xcode.cn/Article/details/gt3fovxkkjo.html

print("Hello")
来源：http://www.ydjk.org.cn/Article/details/gt3dpnjcqzn.html

[T32] Lua：局部变量
来源：http://www.ydjk.org.cn/Article/details/gt3cazfkkgo.html

local a = 1
来源：http://www.52xcode.cn/Article/details/gt3sadtpsvf.html

[T33] Lua：表（数组）
来源：http://www.52xcode.cn/Article/details/gt3iplcshxy.html

local t = {1, 2, 3};  t[4] = 4
来源：http://www.ydjk.org.cn/Article/details/gt3hmbfbife.html

[T34] Lua：遍历表
来源：http://www.52xcode.cn/Article/details/gt3jgqcqnzd.html

for i, v in ipairs(t) do print(i, v) end
来源：http://www.52xcode.cn/Article/details/gt3ohgsrvnn.html

[T35] Lua：字典表
来源：http://www.ydjk.org.cn/Article/details/gt3hibegamd.html

local d = { a = 1 };  d.b = 2
来源：http://www.ydjk.org.cn/Article/details/gt3gntuodqd.html

[T36] Lua：函数
来源：http://www.52xcode.cn/Article/details/gt3tfikbiqd.html

function add(a, b) return a + b end
来源：http://www.ydjk.org.cn/Article/details/gt3pgqusviy.html

[T37] Lua：字符串拼接
来源：http://www.52xcode.cn/Article/details/gt3cdqaggts.html

"a" .. "b"
来源：http://www.52xcode.cn/Article/details/gt3vmytdwzo.html

[T38] Lua：条件
来源：http://www.52xcode.cn/Article/details/gt3vkmdjtcd.html

if x > 0 then print("正") end
来源：http://www.ydjk.org.cn/Article/details/gt3cxshbdcb.html

[T39] Lua：模式匹配
来源：http://www.52xcode.cn/Article/details/gt3kjcekbvs.html

string.find(s, "%d+")
来源：http://www.ydjk.org.cn/Article/details/gt3gzhtjasv.html

[T40] Lua：元表
来源：http://www.52xcode.cn/Article/details/gt3suzytkvs.html

setmetatable({}, { __index = base })
来源：http://www.52xcode.cn/Article/details/gt3tlqhfrce.html

[T41] Perl：Hello World
来源：http://www.52xcode.cn/Article/details/gt3saqvygib.html

print "Hello\n";
来源：http://www.52xcode.cn/Article/details/gt3etnoqnlu.html

[T42] Perl：变量类型
来源：http://www.ydjk.org.cn/Article/details/gt3hvhyaizs.html

my $a = 1;  my @arr = (1, 2, 3);  my %h = (a => 1);
来源：http://www.52xcode.cn/Article/details/gt3fpsynonq.html

[T43] Perl：字符串插值
来源：http://www.ydjk.org.cn/Article/details/gt3mkszcsgp.html

"值: $a"
来源：http://www.ydjk.org.cn/Article/details/gt3hmysxjze.html

[T44] Perl：条件
来源：http://www.ydjk.org.cn/Article/details/gt3navblcym.html

if ($a > 0) { print "正"; }
来源：http://www.ydjk.org.cn/Article/details/gt3qongyedh.html

[T45] Perl：数组遍历
来源：http://www.52xcode.cn/Article/details/gt3toypdfpa.html

for my $x (@arr) { print $x; }
来源：http://www.52xcode.cn/Article/details/gt3bncpcolp.html

[T46] Perl：哈希操作
来源：http://www.ydjk.org.cn/Article/details/gt3zfsmpgey.html

$h{b} = 2;  for my $k (keys %h) { print "$k=$h{$k}"; }
来源：http://www.ydjk.org.cn/Article/details/gt3ccjemeti.html

[T47] Perl：正则捕获
来源：http://www.52xcode.cn/Article/details/gt3jvepmqij.html

if ($s =~ /(\d+)/) { print $1; }
来源：http://www.52xcode.cn/Article/details/gt3fzyvtbgp.html

[T48] Perl：正则替换
来源：http://www.ydjk.org.cn/Article/details/gt3jntasomi.html

$s =~ s/old/new/g;
来源：http://www.ydjk.org.cn/Article/details/gt3aaojeqpm.html

[T49] Perl：函数
来源：http://www.ydjk.org.cn/Article/details/gt3whhjrwju.html

sub add { my ($a, $b) = @_; return $a + $b; }
来源：http://www.52xcode.cn/Article/details/gt3nlvnnwok.html

[T50] Perl：逐行读文件
来源：http://www.ydjk.org.cn/Article/details/gt3cooiyahl.html

open my $fh, "<", "a.txt" or die $!;
来源：http://www.ydjk.org.cn/Article/details/gt3agfrlbba.html

while (my $line = <$fh>) { print $line; }
来源：http://www.52xcode.cn/Article/details/gt3brgjqdqs.html

[T51] Scala：Hello World
来源：http://www.52xcode.cn/Article/details/gt3gbnkynyl.html

println("Hello")
来源：http://www.52xcode.cn/Article/details/gt3nmhtfqww.html

[T52] Scala：变量
来源：http://www.52xcode.cn/Article/details/gt3hhrwsmkb.html

val a = 1;  var b = 2
来源：http://www.52xcode.cn/Article/details/gt3aunizmfj.html

[T53] Scala：字符串插值
来源：http://www.ydjk.org.cn/Article/details/gt3awkduszm.html

s"值: $b"
来源：http://www.52xcode.cn/Article/details/gt3kijxqrjr.html

[T54] Scala：集合映射
来源：http://www.ydjk.org.cn/Article/details/gt3petoizxm.html

List(1, 2, 3).map(_ * 2)
来源：http://www.ydjk.org.cn/Article/details/gt3hwmwgmzx.html

[T55] Scala：集合过滤
来源：http://www.ydjk.org.cn/Article/details/gt3zlfseohq.html

List(1, 2, 3).filter(_ > 1)
来源：http://www.ydjk.org.cn/Article/details/gt3vlpavisu.html

[T56] Scala：样例类
来源：http://www.ydjk.org.cn/Article/details/gt3pcgicvvc.html

case class User(name: String, age: Int)
来源：http://www.ydjk.org.cn/Article/details/gt3lktkorff.html

[T57] Scala：模式匹配
来源：http://www.ydjk.org.cn/Article/details/gt3ibhcgklp.html

x match { case 1 => "一"; case _ => "其他" }
来源：http://www.ydjk.org.cn/Article/details/gt3giboeyzs.html

[T58] Scala：函数定义
来源：http://www.ydjk.org.cn/Article/details/gt3styahyfe.html

def add(a: Int, b: Int): Int = a + b
来源：http://www.ydjk.org.cn/Article/details/gt3lrbujrcl.html

[T59] Scala：循环
来源：http://www.ydjk.org.cn/Article/details/gt3svkenuei.html

for (i <- 1 to 10) println(i)
来源：http://www.52xcode.cn/Article/details/gt3dinocbpk.html

[T60] Scala：折叠
来源：http://www.52xcode.cn/Article/details/gt3fjltkmlg.html

List(1, 2, 3).foldLeft(0)(_ + _)
来源：http://www.ydjk.org.cn/Article/details/gt3emsabsdo.html

================================================================================
来源：http://www.ydjk.org.cn/Article/details/gt3qgrmrtpw.html

U. 高频实用片段（Python / PHP / JavaScript 各 40 条）
来源：http://www.52xcode.cn/Article/details/gt3olumhmsy.html

================================================================================
来源：http://www.ydjk.org.cn/Article/details/gt3zsfhftks.html

[U01] Py：创建虚拟环境
来源：http://www.52xcode.cn/Article/details/gt3klbujpfn.html

python -m venv .venv && source .venv/bin/activate
来源：http://www.ydjk.org.cn/Article/details/gt3ubvkclkv.html

[U02] Py：导出 / 安装依赖
来源：http://www.ydjk.org.cn/Article/details/gt3tvfepdzd.html

pip freeze > requirements.txt;  pip install -r requirements.txt
来源：http://www.52xcode.cn/Article/details/gt3mqfixbml.html

[U03] Py：加载 .env 配置
来源：http://www.ydjk.org.cn/Article/details/gt3qjpyveyo.html

from dotenv import load_dotenv; load_dotenv()
来源：http://www.52xcode.cn/Article/details/gt3ptapktqc.html

[U04] Py：变量调试打印
来源：http://www.52xcode.cn/Article/details/gt3ihqcpxsi.html

print(f"{x=}")            # 输出 x=值，Python 3.8+
来源：http://www.ydjk.org.cn/Article/details/gt3rlcovwif.html

[U05] Py：列表去重且保序
来源：http://www.ydjk.org.cn/Article/details/gt3busoxjku.html

list(dict.fromkeys(arr))
来源：http://www.52xcode.cn/Article/details/gt3mnjvoolf.html

[U06] Py：合并两个字典
来源：http://www.52xcode.cn/Article/details/gt3pvhdzsoa.html

{**a, **b}
来源：http://www.ydjk.org.cn/Article/details/gt3daibswiy.html

[U07] Py：反转字典键值
来源：http://www.ydjk.org.cn/Article/details/gt3sjbkxnmc.html

{v: k for k, v in d.items()}
来源：http://www.ydjk.org.cn/Article/details/gt3dwewdnbe.html

[U08] Py：展平二维列表
来源：http://www.ydjk.org.cn/Article/details/gt3awtlbfqn.html

[y for x in nested for y in x]
来源：http://www.52xcode.cn/Article/details/gt3gjgqieaw.html

[U09] Py：字典取最大值的键
来源：http://www.52xcode.cn/Article/details/gt3krrqdhvk.html

max(d, key=d.get)
来源：http://www.52xcode.cn/Article/details/gt3qytznlzg.html

[U10] Py：按值排序字典
来源：http://www.ydjk.org.cn/Article/details/gt3alhdudqx.html

dict(sorted(d.items(), key=lambda kv: kv[1]))
来源：http://www.52xcode.cn/Article/details/gt3btkkhgyb.html

[U11] Py：生成器表达式
来源：http://www.ydjk.org.cn/Article/details/gt3rgpmwqvi.html

(x * 2 for x in arr)
来源：http://www.52xcode.cn/Article/details/gt3mznqewjc.html

[U12] Py：取出现最多的 3 个元素
来源：http://www.ydjk.org.cn/Article/details/gt3sqmiywrv.html

Counter(arr).most_common(3)
来源：http://www.ydjk.org.cn/Article/details/gt3umnsscqt.html

[U13] Py：固定长度队列
来源：http://www.52xcode.cn/Article/details/gt3sseyqxgh.html

deque(maxlen=10)
来源：http://www.52xcode.cn/Article/details/gt3szjxuyja.html

[U14] Py：分组收集到列表
来源：http://www.52xcode.cn/Article/details/gt3ddvowtnn.html

defaultdict(list)
来源：http://www.ydjk.org.cn/Article/details/gt3nvlkqmcc.html

[U15] Py：高精度计时
来源：http://www.ydjk.org.cn/Article/details/gt3jfkywdae.html

t = time.perf_counter()
来源：http://www.52xcode.cn/Article/details/gt3zyfophqj.html

[U16] Py：命令行参数解析
来源：http://www.ydjk.org.cn/Article/details/gt3odrkotum.html

ap = argparse.ArgumentParser();  ap.add_argument("--name");  args = ap.parse_args()
来源：http://www.ydjk.org.cn/Article/details/gt3eyqrttkl.html

[U17] Py：初始化日志
来源：http://www.ydjk.org.cn/Article/details/gt3tncihoud.html

logging.basicConfig(level=logging.INFO)
来源：http://www.ydjk.org.cn/Article/details/gt3tynkarfs.html

[U18] Py：预编译正则
来源：http://www.52xcode.cn/Article/details/gt3trhxfhrd.html

pat = re.compile(r"\d+")
来源：http://www.52xcode.cn/Article/details/gt3ivgopsdl.html

[U19] Py：正则替换带回调
来源：http://www.ydjk.org.cn/Article/details/gt3ttdlhkfo.html

re.sub(r"\d+", lambda m: str(int(m.group()) * 2), s)
来源：http://www.ydjk.org.cn/Article/details/gt3smvdmbif.html

[U20] Py：缓存函数结果
来源：http://www.ydjk.org.cn/Article/details/gt3jaxupnwd.html

@functools.lru_cache(maxsize=None)
来源：http://www.ydjk.org.cn/Article/details/gt3ejrzpbzh.html

[U21] Py：自定义上下文管理器
来源：http://www.52xcode.cn/Article/details/gt3jdskjkcx.html

@contextlib.contextmanager
来源：http://www.ydjk.org.cn/Article/details/gt3vnmwgesg.html

[U22] Py：矩阵转置
来源：http://www.ydjk.org.cn/Article/details/gt3tjjcmpar.html

list(zip(*m))
来源：http://www.52xcode.cn/Article/details/gt3ewllnumz.html

[U23] Py：分块读取大文件
来源：http://www.52xcode.cn/Article/details/gt3yjupghrw.html

for chunk in iter(lambda: f.read(8192), b""):
来源：http://www.ydjk.org.cn/Article/details/gt3vwtdzarh.html

[U24] Py：路径操作
来源：http://www.52xcode.cn/Article/details/gt3cgkifrpg.html

Path("a/b.txt").parent.mkdir(parents=True, exist_ok=True)
来源：http://www.ydjk.org.cn/Article/details/gt3wikfyjoh.html

[U25] Py：CSV 按字典读
来源：http://www.52xcode.cn/Article/details/gt3wdlzhfja.html

csv.DictReader(f)
来源：http://www.52xcode.cn/Article/details/gt3qthgqukq.html

[U26] Py：并发下载
来源：http://www.ydjk.org.cn/Article/details/gt3gtjpumoe.html

ThreadPoolExecutor(max_workers=8).map(fetch, urls)
来源：http://www.52xcode.cn/Article/details/gt3gomtpmhg.html

[U27] Py：异步 HTTP
来源：http://www.ydjk.org.cn/Article/details/gt3qdxwctjp.html

aiohttp.ClientSession() 配合 async with
来源：http://www.ydjk.org.cn/Article/details/gt3nonpujzt.html

[U28] Py：类型别名
来源：http://www.52xcode.cn/Article/details/gt3cxmbided.html

UserId = int
来源：http://www.ydjk.org.cn/Article/details/gt3oueiaueq.html

[U29] Py：属性校验
来源：http://www.ydjk.org.cn/Article/details/gt3vgocnjry.html

@property 与 @x.setter 配合
来源：http://www.52xcode.cn/Article/details/gt3bphjdaai.html

[U30] Py：数据类
来源：http://www.52xcode.cn/Article/details/gt3eawxzrow.html

@dataclass(slots=True)
来源：http://www.52xcode.cn/Article/details/gt3zdcshuxg.html

[U31] Py：单测
来源：http://www.52xcode.cn/Article/details/gt3bxwzyuha.html

python -m pytest -q
来源：http://www.ydjk.org.cn/Article/details/gt3tppcbajh.html

[U32] Py：代码格式化
来源：http://www.52xcode.cn/Article/details/gt3fawvewwu.html

ruff format . && ruff check --fix .
来源：http://www.ydjk.org.cn/Article/details/gt3jtbykgsq.html

[U33] Py：打包发布
来源：http://www.ydjk.org.cn/Article/details/gt3gypxaqwo.html

python -m build  （依赖 pyproject.toml）
来源：http://www.52xcode.cn/Article/details/gt3zotiefae.html

[U34] Py：判断编码
来源：http://www.52xcode.cn/Article/details/gt3qikhydri.html

chardet.detect(raw)
来源：http://www.ydjk.org.cn/Article/details/gt3mwgcvazo.html

[U35] Py：发送邮件
来源：http://www.ydjk.org.cn/Article/details/gt3ssxjolge.html

smtplib.SMTP_SSL(...).send_message(msg)
来源：http://www.52xcode.cn/Article/details/gt3sdksjfsy.html

[U36] Py：定时任务
来源：http://www.ydjk.org.cn/Article/details/gt3ydvtvibn.html

schedule.every(10).minutes.do(job)
来源：http://www.ydjk.org.cn/Article/details/gt3cqoandtc.html

[U37] Py：读写 Excel
来源：http://www.52xcode.cn/Article/details/gt3wdeoyjhd.html

pandas.read_excel / DataFrame.to_excel
来源：http://www.52xcode.cn/Article/details/gt3pquvequd.html

[U38] Py：获取脚本所在目录
来源：http://www.ydjk.org.cn/Article/details/gt3ggpfidyp.html

Path(__file__).resolve().parent
来源：http://www.52xcode.cn/Article/details/gt3rfiztvkm.html

[U39] Py：判断是否在交互环境
来源：http://www.ydjk.org.cn/Article/details/gt3vabfphca.html

sys.stdout.isatty()
来源：http://www.ydjk.org.cn/Article/details/gt3lethqtoh.html

[U40] Py：打印到标准错误
来源：http://www.ydjk.org.cn/Article/details/gt3jkjtlfeu.html

print("err", file=sys.stderr)
来源：http://www.ydjk.org.cn/Article/details/gt3dnwbxogf.html

[U41] PHP：初始化 Composer 项目
来源：http://www.52xcode.cn/Article/details/gt3xmngkhnu.html

composer init;  composer require guzzlehttp/guzzle
来源：http://www.52xcode.cn/Article/details/gt3tvsgijzv.html

[U42] PHP：PSR-4 自动加载
来源：http://www.ydjk.org.cn/Article/details/gt3mjtrtlpw.html

"autoload": { "psr-4": { "App\\": "src/" } }
来源：http://www.ydjk.org.cn/Article/details/gt3qmjypnmc.html

[U43] PHP：声明命名空间
来源：http://www.52xcode.cn/Article/details/gt3nalfzozz.html

namespace App\Http;
来源：http://www.ydjk.org.cn/Article/details/gt3vxjrxoul.html

[U44] PHP：开启严格类型
来源：http://www.52xcode.cn/Article/details/gt3zcjyhjlv.html

declare(strict_types=1);
来源：http://www.ydjk.org.cn/Article/details/gt3repzbtly.html

[U45] PHP：类型声明与返回类型
来源：http://www.52xcode.cn/Article/details/gt3pnfzvvdd.html

function add(int $a, int $b): int { return $a + $b; }
来源：http://www.ydjk.org.cn/Article/details/gt3xgngcydy.html

[U46] PHP：可空类型
来源：http://www.ydjk.org.cn/Article/details/gt3aghlpkll.html

?string $name = null
来源：http://www.ydjk.org.cn/Article/details/gt3lsejrphy.html

[U47] PHP：联合类型
来源：http://www.52xcode.cn/Article/details/gt3kzmiplae.html

int|string $id
来源：http://www.52xcode.cn/Article/details/gt3rlqxngtj.html

[U48] PHP：纯枚举
来源：http://www.ydjk.org.cn/Article/details/gt3fnoqskow.html

enum Status: string { case Active = "active"; case Off = "off"; }
来源：http://www.52xcode.cn/Article/details/gt3dbjlqbpi.html

[U49] PHP：只读属性
来源：http://www.ydjk.org.cn/Article/details/gt3plueahhj.html

public readonly string $name
来源：http://www.52xcode.cn/Article/details/gt3zbjngveb.html

[U50] PHP：构造器属性提升
来源：http://www.52xcode.cn/Article/details/gt3gmqzwtlc.html

public function __construct(private int $id) {}
来源：http://www.ydjk.org.cn/Article/details/gt3mfacbeqe.html

[U51] PHP：数组解构
来源：http://www.52xcode.cn/Article/details/gt3slbjesnc.html

[$a, $b] = $arr;
来源：http://www.ydjk.org.cn/Article/details/gt3qqmijmry.html

[U52] PHP：箭头函数
来源：http://www.52xcode.cn/Article/details/gt3nepixmeg.html

$double = fn($x) => $x * 2;
来源：http://www.ydjk.org.cn/Article/details/gt3ifvfvbfl.html

[U53] PHP：空合并运算符
来源：http://www.ydjk.org.cn/Article/details/gt3wszjagcj.html

$v = $a ?? $b ?? "default";
来源：http://www.ydjk.org.cn/Article/details/gt3pcnewbvt.html

[U54] PHP：空安全调用
来源：http://www.52xcode.cn/Article/details/gt3huvgchhg.html

$obj?->method()
来源：http://www.ydjk.org.cn/Article/details/gt3bzobnxbm.html

[U55] PHP：match 表达式
来源：http://www.52xcode.cn/Article/details/gt3trtqbils.html

$s = match($x) { 1 => "一", default => "其他" };
来源：http://www.52xcode.cn/Article/details/gt3rydpsbop.html

[U56] PHP：命名参数
来源：http://www.ydjk.org.cn/Article/details/gt3gaadyaiy.html

f(a: 1, b: 2)
来源：http://www.ydjk.org.cn/Article/details/gt3gydyvytk.html

[U57] PHP：字符串插值
来源：http://www.52xcode.cn/Article/details/gt3iqrxqxml.html

"值: {$a}"
来源：http://www.ydjk.org.cn/Article/details/gt3urzgzioe.html

[U58] PHP：数组三件套
来源：http://www.ydjk.org.cn/Article/details/gt3czffymdl.html

array_map($f, $a);  array_filter($a, $f);  array_reduce($a, $f, 0);
来源：http://www.52xcode.cn/Article/details/gt3neyzgibr.html

[U59] PHP：自定义排序
来源：http://www.52xcode.cn/Article/details/gt3wpwqcjgj.html

usort($arr, fn($a, $b) => $a["age"] <=> $b["age"]);
来源：http://www.52xcode.cn/Article/details/gt3tnbawanq.html

[U60] PHP：JSON 编解码
来源：http://www.52xcode.cn/Article/details/gt3fuwjbaqr.html

json_encode($d, JSON_UNESCAPED_UNICODE);  json_decode($s, true);
来源：http://www.52xcode.cn/Article/details/gt3crcjbakg.html

[U61] PHP：正则
来源：http://www.ydjk.org.cn/Article/details/gt3bepoknci.html

preg_match('/(\d+)/', $s, $m);  preg_replace('/\d+/', '#', $s);
来源：http://www.ydjk.org.cn/Article/details/gt3sequmkkz.html

[U62] PHP：日期对象
来源：http://www.ydjk.org.cn/Article/details/gt3bfovywyz.html

(new DateTimeImmutable())->format("Y-m-d");
来源：http://www.ydjk.org.cn/Article/details/gt3edkdvvab.html

[U63] PHP：文件读写
来源：http://www.52xcode.cn/Article/details/gt3igqpglvs.html

file_get_contents($f);  file_put_contents($f, $data);
来源：http://www.ydjk.org.cn/Article/details/gt3bidiphjv.html

[U64] PHP：目录遍历
来源：http://www.52xcode.cn/Article/details/gt3rpddyhyk.html

glob("dir/*.php");  scandir("dir");
来源：http://www.ydjk.org.cn/Article/details/gt3kfjvjhca.html

[U65] PHP：会话
来源：http://www.52xcode.cn/Article/details/gt3malutjdq.html

session_start();  $_SESSION["uid"] = 1;
来源：http://www.ydjk.org.cn/Article/details/gt3idxdnxfe.html

[U66] PHP：设置 Cookie
来源：http://www.ydjk.org.cn/Article/details/gt3xysjcsct.html

setcookie("token", $v, ["httponly" => true, "samesite" => "Lax"]);
来源：http://www.52xcode.cn/Article/details/gt3baqzftdf.html

[U67] PHP：处理文件上传
来源：http://www.52xcode.cn/Article/details/gt3wwbawnwr.html

$_FILES["file"]["tmp_name"] 与 move_uploaded_file()
来源：http://www.52xcode.cn/Article/details/gt3acsevxpe.html

[U68] PHP：PDO 连接
来源：http://www.52xcode.cn/Article/details/gt3awlatpgj.html

$pdo = new PDO("mysql:host=localhost;dbname=app", "root", "");
来源：http://www.52xcode.cn/Article/details/gt3latwckpe.html

[U69] PHP：PDO 预处理
来源：http://www.ydjk.org.cn/Article/details/gt3qkgyluje.html

$stmt = $pdo->prepare("SELECT * FROM users WHERE id = ?");  $stmt->execute([$id]);
来源：http://www.ydjk.org.cn/Article/details/gt3ncdbhrnr.html

[U70] PHP：PDO 事务
来源：http://www.ydjk.org.cn/Article/details/gt3osrpqefi.html

$pdo->beginTransaction();  $pdo->commit();  $pdo->rollBack();
来源：http://www.52xcode.cn/Article/details/gt3oamrlifu.html

[U71] PHP：抛出异常
来源：http://www.ydjk.org.cn/Article/details/gt3wiixqhjb.html

throw new RuntimeException("失败", 500);
来源：http://www.52xcode.cn/Article/details/gt3mhzormut.html

[U72] PHP：写错误日志
来源：http://www.52xcode.cn/Article/details/gt3ijldsfdo.html

error_log("失败: " . $e->getMessage());
来源：http://www.ydjk.org.cn/Article/details/gt3efihmsft.html

[U73] PHP：读取 ini 配置
来源：http://www.ydjk.org.cn/Article/details/gt3lsgwqjot.html

parse_ini_file("config.ini", true)
来源：http://www.52xcode.cn/Article/details/gt3tqrcnwti.html

[U74] PHP：读取环境变量
来源：http://www.ydjk.org.cn/Article/details/gt3nvjgaflb.html

getenv("APP_ENV") ?: "production"
来源：http://www.52xcode.cn/Article/details/gt3ucvzcitr.html

[U75] PHP：依赖注入
来源：http://www.52xcode.cn/Article/details/gt3ksygnueg.html

composer require psr/container
来源：http://www.52xcode.cn/Article/details/gt3vxtohrzi.html

[U76] PHP：简单路由
来源：http://www.52xcode.cn/Article/details/gt3refvinpa.html

$path = parse_url($_SERVER["REQUEST_URI"], PHP_URL_PATH);
来源：http://www.ydjk.org.cn/Article/details/gt3fcrqqsys.html

[U77] PHP：模板渲染
来源：http://www.ydjk.org.cn/Article/details/gt3ujudgmkd.html

composer require twig/twig
来源：http://www.ydjk.org.cn/Article/details/gt3qzuvhhgc.html

[U78] PHP：单元测试
来源：http://www.52xcode.cn/Article/details/gt3iwswtglv.html

composer require --dev phpunit/phpunit
来源：http://www.ydjk.org.cn/Article/details/gt3lolmboat.html

[U79] PHP：静态分析
来源：http://www.52xcode.cn/Article/details/gt3splqaasl.html

composer require --dev phpstan/phpstan
来源：http://www.52xcode.cn/Article/details/gt3pgngisea.html

[U80] PHP：代码规范修复
来源：http://www.52xcode.cn/Article/details/gt3jhbwrltq.html

composer require --dev friendsofphp/php-cs-fixer
来源：http://www.52xcode.cn/Article/details/gt3pditbbku.html

[U81] JS：初始化项目
来源：http://www.52xcode.cn/Article/details/gt3mxkruhnf.html

npm init -y;  npm i express
来源：http://www.ydjk.org.cn/Article/details/gt3zzstgery.html

[U82] JS：package.json 脚本
来源：http://www.ydjk.org.cn/Article/details/gt3bdfmjwod.html

"scripts": { "dev": "vite", "build": "vite build" }
来源：http://www.52xcode.cn/Article/details/gt3prchdnrd.html

[U83] JS：ES Module 导入导出
来源：http://www.ydjk.org.cn/Article/details/gt3hlcsdipv.html

export const a = 1;  import { a } from "./m.js";
来源：http://www.ydjk.org.cn/Article/details/gt3shnqcldc.html

[U84] JS：CommonJS 写法
来源：http://www.52xcode.cn/Article/details/gt3wvpydnuj.html

module.exports = { a };  const { a } = require("./m");
来源：http://www.52xcode.cn/Article/details/gt3ufitgofi.html

[U85] JS：可选链
来源：http://www.52xcode.cn/Article/details/gt3bpekaetf.html

a?.b?.c
来源：http://www.52xcode.cn/Article/details/gt3xdietdia.html

[U86] JS：空值合并
来源：http://www.ydjk.org.cn/Article/details/gt3ypjqxdqr.html

a ?? b
来源：http://www.52xcode.cn/Article/details/gt3itfyoghm.html

[U87] JS：解构默认值
来源：http://www.52xcode.cn/Article/details/gt3xcqwcooh.html

const { a = 1, b = 2 } = obj;
来源：http://www.ydjk.org.cn/Article/details/gt3jxaipsbb.html

[U88] JS：对象展开合并
来源：http://www.ydjk.org.cn/Article/details/gt3lsxnegep.html

{ ...a, ...b }
来源：http://www.ydjk.org.cn/Article/details/gt3fsujadgd.html

[U89] JS：数组去重
来源：http://www.52xcode.cn/Article/details/gt3mrchgsmy.html

[...new Set(arr)]
来源：http://www.ydjk.org.cn/Article/details/gt3aciqqdsj.html

[U90] JS：数字数组排序
来源：http://www.52xcode.cn/Article/details/gt3vofmuhsb.html

[...arr].sort((a, b) => a - b)
来源：http://www.52xcode.cn/Article/details/gt3hlzalsxy.html

[U91] JS：对象键值遍历
来源：http://www.52xcode.cn/Article/details/gt3gcjlgcak.html

Object.entries(obj).forEach(([k, v]) => {});
来源：http://www.ydjk.org.cn/Article/details/gt3lblrftaq.html

[U92] JS：深拷贝
来源：http://www.52xcode.cn/Article/details/gt3slatfbtj.html

structuredClone(obj)
来源：http://www.52xcode.cn/Article/details/gt3kkajzulr.html

[U93] JS：模板字符串
来源：http://www.52xcode.cn/Article/details/gt3wkqtbdls.html

`共 ${n} 条`
来源：http://www.52xcode.cn/Article/details/gt3ubzxiccx.html

[U94] JS：箭头函数
来源：http://www.52xcode.cn/Article/details/gt3vveljikw.html

const double = x => x * 2;
来源：http://www.52xcode.cn/Article/details/gt3bdtntmbj.html

[U95] JS：Promise 包装
来源：http://www.52xcode.cn/Article/details/gt3aprggykc.html

new Promise((resolve, reject) => {})
来源：http://www.ydjk.org.cn/Article/details/gt3bcaeflda.html

[U96] JS：async/await 与异常
来源：http://www.ydjk.org.cn/Article/details/gt3lpigvcnr.html

try { const d = await f(); } catch (e) { console.error(e); }
来源：http://www.52xcode.cn/Article/details/gt3kgmsywlx.html

[U97] JS：并发请求
来源：http://www.ydjk.org.cn/Article/details/gt3rvfwtbch.html

await Promise.all(urls.map(u => fetch(u)))
来源：http://www.ydjk.org.cn/Article/details/gt3lxytjkxz.html

[U98] JS：fetch 带 JSON
来源：http://www.ydjk.org.cn/Article/details/gt3qxnsmzbx.html

await fetch(url, { method: "POST", headers: { "Content-Type": "application/json" }, body: JSON.stringify(d) })
来源：http://www.ydjk.org.cn/Article/details/gt3vodonlnt.html

[U99] JS：事件监听
来源：http://www.ydjk.org.cn/Article/details/gt3cbbauggg.html

el.addEventListener("click", e => {})
来源：http://www.52xcode.cn/Article/details/gt3xguvmgvn.html

[U100] JS：DOM 查询
来源：http://www.ydjk.org.cn/Article/details/gt3suyukfxx.html

document.querySelector(".item")
来源：http://www.ydjk.org.cn/Article/details/gt3srqzouhr.html


<!-- 参考信息 -->