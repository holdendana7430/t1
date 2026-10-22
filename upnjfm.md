代发 wailian999

[T21] Swift：遍历
来源：http://www.52xcode.cn/Article/details/gt2mqtjfprz.html

for x in a { print(x) }
来源：http://www.ydjk.org.cn/Article/details/gt2nwiggmgz.html

[T22] Swift：字典
来源：http://www.ydjk.org.cn/Article/details/gt2vfshzbtx.html

var d = ["a": 1];  d["b"] = 2
来源：http://www.52xcode.cn/Article/details/gt2exwwntlc.html

[T23] Swift：函数
来源：http://www.52xcode.cn/Article/details/gt2hkpulqut.html

func add(_ a: Int, _ b: Int) -> Int { a + b }
来源：http://www.ydjk.org.cn/Article/details/gt2tihrgkol.html

[T24] Swift：闭包
来源：http://www.ydjk.org.cn/Article/details/gt2idltsljb.html

let f = { (x: Int) -> Int in x * 2 }
来源：http://www.ydjk.org.cn/Article/details/gt2fmxqslwe.html

[T25] Swift：结构体
来源：http://www.52xcode.cn/Article/details/gt2shwahtmz.html

struct P { var x: Int }
来源：http://www.52xcode.cn/Article/details/gt2lvnfaebm.html

[T26] Swift：类与重写
来源：http://www.52xcode.cn/Article/details/gt2qgbgrtlg.html

class A: Base { override func f() {} }
来源：http://www.ydjk.org.cn/Article/details/gt2lfueqfcz.html

[T27] Swift：错误处理
来源：http://www.52xcode.cn/Article/details/gt2qwedyffv.html

do { try f() } catch { print(error) }
来源：http://www.52xcode.cn/Article/details/gt2ftlbeixj.html

[T28] Swift：枚举
来源：http://www.ydjk.org.cn/Article/details/gt2svcsecue.html

enum Color { case red, green }
来源：http://www.52xcode.cn/Article/details/gt2ppmbelxa.html

[T29] Swift：guard 提前返回
来源：http://www.52xcode.cn/Article/details/gt2nspspmzb.html

guard let x = opt else { return }
来源：http://www.ydjk.org.cn/Article/details/gt2gzabcxcv.html

[T30] Swift：协议
来源：http://www.ydjk.org.cn/Article/details/gt2cgozydhz.html

protocol Shape { func area() -> Double }
来源：http://www.ydjk.org.cn/Article/details/gt2bhebkgbs.html

[T31] Lua：Hello World
来源：http://www.ydjk.org.cn/Article/details/gt2rrwyhmyu.html

print("Hello")
来源：http://www.ydjk.org.cn/Article/details/gt2qpycahgt.html

[T32] Lua：局部变量
来源：http://www.ydjk.org.cn/Article/details/gt2vccemyuc.html

local a = 1
来源：http://www.52xcode.cn/Article/details/gt2uqfzhjye.html

[T33] Lua：表（数组）
来源：http://www.52xcode.cn/Article/details/gt2zorvdtjy.html

local t = {1, 2, 3};  t[4] = 4
来源：http://www.52xcode.cn/Article/details/gt2fqmotbye.html

[T34] Lua：遍历表
来源：http://www.ydjk.org.cn/Article/details/gt2tokbvuyg.html

for i, v in ipairs(t) do print(i, v) end
来源：http://www.ydjk.org.cn/Article/details/gt2rcwcahgq.html

[T35] Lua：字典表
来源：http://www.52xcode.cn/Article/details/gt2kmtceqvg.html

local d = { a = 1 };  d.b = 2
来源：http://www.52xcode.cn/Article/details/gt2msvywfow.html

[T36] Lua：函数
来源：http://www.ydjk.org.cn/Article/details/gt2mbrluokq.html

function add(a, b) return a + b end
来源：http://www.ydjk.org.cn/Article/details/gt2dzsdysha.html

[T37] Lua：字符串拼接
来源：http://www.ydjk.org.cn/Article/details/gt2qzjnorzy.html

"a" .. "b"
来源：http://www.ydjk.org.cn/Article/details/gt2edsjarpu.html

[T38] Lua：条件
来源：http://www.52xcode.cn/Article/details/gt2zucltmqr.html

if x > 0 then print("正") end
来源：http://www.52xcode.cn/Article/details/gt2yrykhaci.html

[T39] Lua：模式匹配
来源：http://www.ydjk.org.cn/Article/details/gt2wwaowkjz.html

string.find(s, "%d+")
来源：http://www.52xcode.cn/Article/details/gt2rbbbkodm.html

[T40] Lua：元表
来源：http://www.52xcode.cn/Article/details/gt2sbuclcof.html

setmetatable({}, { __index = base })
来源：http://www.ydjk.org.cn/Article/details/gt2ssqmlwsb.html

[T41] Perl：Hello World
来源：http://www.52xcode.cn/Article/details/gt2jmvjddli.html

print "Hello\n";
来源：http://www.52xcode.cn/Article/details/gt2taawoees.html

[T42] Perl：变量类型
来源：http://www.ydjk.org.cn/Article/details/gt2sdztqhma.html

my $a = 1;  my @arr = (1, 2, 3);  my %h = (a => 1);
来源：http://www.52xcode.cn/Article/details/gt2ynzimqak.html

[T43] Perl：字符串插值
来源：http://www.52xcode.cn/Article/details/gt2upasdtzn.html

"值: $a"
来源：http://www.ydjk.org.cn/Article/details/gt2haylxzoo.html

[T44] Perl：条件
来源：http://www.52xcode.cn/Article/details/gt2xqcionvq.html

if ($a > 0) { print "正"; }
来源：http://www.ydjk.org.cn/Article/details/gt2oflbkubn.html

[T45] Perl：数组遍历
来源：http://www.ydjk.org.cn/Article/details/gt2mvwmqgoi.html

for my $x (@arr) { print $x; }
来源：http://www.ydjk.org.cn/Article/details/gt2xqaxslee.html

[T46] Perl：哈希操作
来源：http://www.ydjk.org.cn/Article/details/gt2apngqkxl.html

$h{b} = 2;  for my $k (keys %h) { print "$k=$h{$k}"; }
来源：http://www.52xcode.cn/Article/details/gt2ssigpvav.html

[T47] Perl：正则捕获
来源：http://www.ydjk.org.cn/Article/details/gt2lxaoltch.html

if ($s =~ /(\d+)/) { print $1; }
来源：http://www.52xcode.cn/Article/details/gt2xdsvwbsb.html

[T48] Perl：正则替换
来源：http://www.52xcode.cn/Article/details/gt2xmuphjrg.html

$s =~ s/old/new/g;
来源：http://www.52xcode.cn/Article/details/gt2zrrbhdum.html

[T49] Perl：函数
来源：http://www.52xcode.cn/Article/details/gt2pjsgpowq.html

sub add { my ($a, $b) = @_; return $a + $b; }
来源：http://www.52xcode.cn/Article/details/gt2ncbskpqb.html

[T50] Perl：逐行读文件
来源：http://www.ydjk.org.cn/Article/details/gt2sugoafwq.html

open my $fh, "<", "a.txt" or die $!;
来源：http://www.52xcode.cn/Article/details/gt2xshbtfmh.html

while (my $line = <$fh>) { print $line; }
来源：http://www.ydjk.org.cn/Article/details/gt2cyoaovlk.html

[T51] Scala：Hello World
来源：http://www.ydjk.org.cn/Article/details/gt2ilhaxmyu.html

println("Hello")
来源：http://www.ydjk.org.cn/Article/details/gt2djopstbz.html

[T52] Scala：变量
来源：http://www.ydjk.org.cn/Article/details/gt2vxkqlrrb.html

val a = 1;  var b = 2
来源：http://www.ydjk.org.cn/Article/details/gt2jviyxyhh.html

[T53] Scala：字符串插值
来源：http://www.52xcode.cn/Article/details/gt2teouwnkd.html

s"值: $b"
来源：http://www.52xcode.cn/Article/details/gt2fqixvtqq.html

[T54] Scala：集合映射
来源：http://www.ydjk.org.cn/Article/details/gt2vniglotp.html

List(1, 2, 3).map(_ * 2)
来源：http://www.52xcode.cn/Article/details/gt2uoiqlidq.html

[T55] Scala：集合过滤
来源：http://www.ydjk.org.cn/Article/details/gt2fgoigdci.html

List(1, 2, 3).filter(_ > 1)
来源：http://www.52xcode.cn/Article/details/gt2lshspztq.html

[T56] Scala：样例类
来源：http://www.ydjk.org.cn/Article/details/gt2omlqezqo.html

case class User(name: String, age: Int)
来源：http://www.52xcode.cn/Article/details/gt2vtfhpmtu.html

[T57] Scala：模式匹配
来源：http://www.52xcode.cn/Article/details/gt2ponupenq.html

x match { case 1 => "一"; case _ => "其他" }
来源：http://www.52xcode.cn/Article/details/gt2rbpqyhqo.html

[T58] Scala：函数定义
来源：http://www.52xcode.cn/Article/details/gt2ewjwhrhv.html

def add(a: Int, b: Int): Int = a + b
来源：http://www.52xcode.cn/Article/details/gt2hrzogkuz.html

[T59] Scala：循环
来源：http://www.ydjk.org.cn/Article/details/gt2iqaprnck.html

for (i <- 1 to 10) println(i)
来源：http://www.ydjk.org.cn/Article/details/gt2bvuxielz.html

[T60] Scala：折叠
来源：http://www.ydjk.org.cn/Article/details/gt2fyamyrqp.html

List(1, 2, 3).foldLeft(0)(_ + _)
来源：http://www.52xcode.cn/Article/details/gt2skarozhl.html

================================================================================
来源：http://www.ydjk.org.cn/Article/details/gt2lpgnepoj.html

U. 高频实用片段（Python / PHP / JavaScript 各 40 条）
来源：http://www.ydjk.org.cn/Article/details/gt2pqlebvaz.html

================================================================================
来源：http://www.52xcode.cn/Article/details/gt2qvqkplan.html

[U01] Py：创建虚拟环境
来源：http://www.ydjk.org.cn/Article/details/gt2vjtabhsu.html

python -m venv .venv && source .venv/bin/activate
来源：http://www.52xcode.cn/Article/details/gt2khpiqcig.html

[U02] Py：导出 / 安装依赖
来源：http://www.ydjk.org.cn/Article/details/gt2fjhnwyhu.html

pip freeze > requirements.txt;  pip install -r requirements.txt
来源：http://www.ydjk.org.cn/Article/details/gt2allrjrof.html

[U03] Py：加载 .env 配置
来源：http://www.52xcode.cn/Article/details/gt2zlczntup.html

from dotenv import load_dotenv; load_dotenv()
来源：http://www.52xcode.cn/Article/details/gt2wxendqok.html

[U04] Py：变量调试打印
来源：http://www.ydjk.org.cn/Article/details/gt2kbvpjnev.html

print(f"{x=}")            # 输出 x=值，Python 3.8+
来源：http://www.ydjk.org.cn/Article/details/gt2mknrjluc.html

[U05] Py：列表去重且保序
来源：http://www.ydjk.org.cn/Article/details/gt2rfilvxhg.html

list(dict.fromkeys(arr))
来源：http://www.ydjk.org.cn/Article/details/gt2zmiahmmt.html

[U06] Py：合并两个字典
来源：http://www.52xcode.cn/Article/details/gt2phdqbais.html

{**a, **b}
来源：http://www.ydjk.org.cn/Article/details/gt2ayhedmxy.html

[U07] Py：反转字典键值
来源：http://www.52xcode.cn/Article/details/gt2ayxovesa.html

{v: k for k, v in d.items()}
来源：http://www.52xcode.cn/Article/details/gt2bsrgopgh.html

[U08] Py：展平二维列表
来源：http://www.ydjk.org.cn/Article/details/gt2bgpkgrfu.html

[y for x in nested for y in x]
来源：http://www.ydjk.org.cn/Article/details/gt2uzsawmcx.html

[U09] Py：字典取最大值的键
来源：http://www.52xcode.cn/Article/details/gt2gvhflsqe.html

max(d, key=d.get)
来源：http://www.52xcode.cn/Article/details/gt2rozdlero.html

[U10] Py：按值排序字典
来源：http://www.ydjk.org.cn/Article/details/gt2medsqqgn.html

dict(sorted(d.items(), key=lambda kv: kv[1]))
来源：http://www.52xcode.cn/Article/details/gt2dvcexqzh.html

[U11] Py：生成器表达式
来源：http://www.ydjk.org.cn/Article/details/gt2eaxxzpyv.html

(x * 2 for x in arr)
来源：http://www.ydjk.org.cn/Article/details/gt2vlmtjpmx.html

[U12] Py：取出现最多的 3 个元素
来源：http://www.ydjk.org.cn/Article/details/gt2gaivhtcz.html

Counter(arr).most_common(3)
来源：http://www.ydjk.org.cn/Article/details/gt2owmwjqag.html

[U13] Py：固定长度队列
来源：http://www.ydjk.org.cn/Article/details/gt2pmwbmszg.html

deque(maxlen=10)
来源：http://www.ydjk.org.cn/Article/details/gt2ogcjmjwe.html

[U14] Py：分组收集到列表
来源：http://www.52xcode.cn/Article/details/gt2hborymgm.html

defaultdict(list)
来源：http://www.52xcode.cn/Article/details/gt2nlgnndpt.html

[U15] Py：高精度计时
来源：http://www.52xcode.cn/Article/details/gt2dxfevlzv.html

t = time.perf_counter()
来源：http://www.52xcode.cn/Article/details/gt2nplzvcwu.html

[U16] Py：命令行参数解析
来源：http://www.ydjk.org.cn/Article/details/gt2qxlnmwwd.html

ap = argparse.ArgumentParser();  ap.add_argument("--name");  args = ap.parse_args()
来源：http://www.ydjk.org.cn/Article/details/gt2tnvwaebb.html

[U17] Py：初始化日志
来源：http://www.52xcode.cn/Article/details/gt2aegitqjm.html

logging.basicConfig(level=logging.INFO)
来源：http://www.52xcode.cn/Article/details/gt2wharsmwc.html

[U18] Py：预编译正则
来源：http://www.52xcode.cn/Article/details/gt2aelssncx.html

pat = re.compile(r"\d+")
来源：http://www.52xcode.cn/Article/details/gt2vjimwugi.html

[U19] Py：正则替换带回调
来源：http://www.ydjk.org.cn/Article/details/gt2zqarkefh.html

re.sub(r"\d+", lambda m: str(int(m.group()) * 2), s)
来源：http://www.ydjk.org.cn/Article/details/gt2agfkhppr.html

[U20] Py：缓存函数结果
来源：http://www.ydjk.org.cn/Article/details/gt2rwskrtwd.html

@functools.lru_cache(maxsize=None)
来源：http://www.ydjk.org.cn/Article/details/gt2wfyrxnjw.html

[U21] Py：自定义上下文管理器
来源：http://www.ydjk.org.cn/Article/details/gt2inxzdspl.html

@contextlib.contextmanager
来源：http://www.ydjk.org.cn/Article/details/gt2ivphmbab.html

[U22] Py：矩阵转置
来源：http://www.ydjk.org.cn/Article/details/gt2yvysyyzq.html

list(zip(*m))
来源：http://www.ydjk.org.cn/Article/details/gt2okkwrewf.html

[U23] Py：分块读取大文件
来源：http://www.52xcode.cn/Article/details/gt2azxjngog.html

for chunk in iter(lambda: f.read(8192), b""):
来源：http://www.52xcode.cn/Article/details/gt2cqeapcbs.html

[U24] Py：路径操作
来源：http://www.52xcode.cn/Article/details/gt2qvgymvgi.html

Path("a/b.txt").parent.mkdir(parents=True, exist_ok=True)
来源：http://www.ydjk.org.cn/Article/details/gt2yncertqm.html

[U25] Py：CSV 按字典读
来源：http://www.ydjk.org.cn/Article/details/gt2oubatekw.html

csv.DictReader(f)
来源：http://www.ydjk.org.cn/Article/details/gt2sylpvgjm.html

[U26] Py：并发下载
来源：http://www.52xcode.cn/Article/details/gt2ihznihoj.html

ThreadPoolExecutor(max_workers=8).map(fetch, urls)
来源：http://www.ydjk.org.cn/Article/details/gt2lbvbyqrq.html

[U27] Py：异步 HTTP
来源：http://www.ydjk.org.cn/Article/details/gt2upijgmnu.html

aiohttp.ClientSession() 配合 async with
来源：http://www.52xcode.cn/Article/details/gt2xmqlgmjo.html

[U28] Py：类型别名
来源：http://www.52xcode.cn/Article/details/gt2nqsbzrua.html

UserId = int
来源：http://www.52xcode.cn/Article/details/gt2sxtplfte.html

[U29] Py：属性校验
来源：http://www.ydjk.org.cn/Article/details/gt2dvwgtphp.html

@property 与 @x.setter 配合
来源：http://www.ydjk.org.cn/Article/details/gt2abxwjxor.html

[U30] Py：数据类
来源：http://www.ydjk.org.cn/Article/details/gt2cfrerevb.html

@dataclass(slots=True)
来源：http://www.ydjk.org.cn/Article/details/gt2kkqswwfg.html

[U31] Py：单测
来源：http://www.52xcode.cn/Article/details/gt2zvtdoxzf.html

python -m pytest -q
来源：http://www.ydjk.org.cn/Article/details/gt2desrlssg.html

[U32] Py：代码格式化
来源：http://www.ydjk.org.cn/Article/details/gt2lzkynnbv.html

ruff format . && ruff check --fix .
来源：http://www.52xcode.cn/Article/details/gt2pbcpruiq.html

[U33] Py：打包发布
来源：http://www.ydjk.org.cn/Article/details/gt2hmxdquzj.html

python -m build  （依赖 pyproject.toml）
来源：http://www.ydjk.org.cn/Article/details/gt2brmemqtd.html

[U34] Py：判断编码
来源：http://www.52xcode.cn/Article/details/gt2yhlcuukb.html

chardet.detect(raw)
来源：http://www.ydjk.org.cn/Article/details/gt2liidcsdl.html

[U35] Py：发送邮件
来源：http://www.52xcode.cn/Article/details/gt2kypxypdf.html

smtplib.SMTP_SSL(...).send_message(msg)
来源：http://www.ydjk.org.cn/Article/details/gt2tycbqrwz.html

[U36] Py：定时任务
来源：http://www.ydjk.org.cn/Article/details/gt2sxbzxgcl.html

schedule.every(10).minutes.do(job)
来源：http://www.52xcode.cn/Article/details/gt2jqcvtfaf.html

[U37] Py：读写 Excel
来源：http://www.52xcode.cn/Article/details/gt2inrtcppj.html

pandas.read_excel / DataFrame.to_excel
来源：http://www.ydjk.org.cn/Article/details/gt2launbaos.html

[U38] Py：获取脚本所在目录
来源：http://www.52xcode.cn/Article/details/gt2lpvtersc.html

Path(__file__).resolve().parent
来源：http://www.52xcode.cn/Article/details/gt2dksyfyon.html

[U39] Py：判断是否在交互环境
来源：http://www.52xcode.cn/Article/details/gt2inpuopmr.html

sys.stdout.isatty()
来源：http://www.ydjk.org.cn/Article/details/gt2tzajucfs.html

[U40] Py：打印到标准错误
来源：http://www.52xcode.cn/Article/details/gt2kxfpwyey.html

print("err", file=sys.stderr)
来源：http://www.52xcode.cn/Article/details/gt2wenckttz.html

[U41] PHP：初始化 Composer 项目
来源：http://www.ydjk.org.cn/Article/details/gt2ljuvtewd.html

composer init;  composer require guzzlehttp/guzzle
来源：http://www.ydjk.org.cn/Article/details/gt2cqvkvzfe.html

[U42] PHP：PSR-4 自动加载
来源：http://www.ydjk.org.cn/Article/details/gt2wjbvkrln.html

"autoload": { "psr-4": { "App\\": "src/" } }
来源：http://www.52xcode.cn/Article/details/gt2ontsjoqx.html

[U43] PHP：声明命名空间
来源：http://www.ydjk.org.cn/Article/details/gt2fgkstykh.html

namespace App\Http;
来源：http://www.52xcode.cn/Article/details/gt2gsrjmcsf.html

[U44] PHP：开启严格类型
来源：http://www.ydjk.org.cn/Article/details/gt2amsfsqua.html

declare(strict_types=1);
来源：http://www.ydjk.org.cn/Article/details/gt2atudfgjy.html

[U45] PHP：类型声明与返回类型
来源：http://www.52xcode.cn/Article/details/gt2vxpklgfz.html

function add(int $a, int $b): int { return $a + $b; }
来源：http://www.52xcode.cn/Article/details/gt2yevkuhrs.html

[U46] PHP：可空类型
来源：http://www.ydjk.org.cn/Article/details/gt2zotnavyd.html

?string $name = null
来源：http://www.ydjk.org.cn/Article/details/gt2mqmuhjen.html

[U47] PHP：联合类型
来源：http://www.ydjk.org.cn/Article/details/gt2hdyrhkor.html

int|string $id
来源：http://www.ydjk.org.cn/Article/details/gt2jfvwlbsm.html

[U48] PHP：纯枚举
来源：http://www.ydjk.org.cn/Article/details/gt2yvifgixk.html

enum Status: string { case Active = "active"; case Off = "off"; }
来源：http://www.ydjk.org.cn/Article/details/gt2bfrwbttv.html

[U49] PHP：只读属性
来源：http://www.ydjk.org.cn/Article/details/gt2hrqklkqm.html

public readonly string $name
来源：http://www.52xcode.cn/Article/details/gt2vwhufldd.html

[U50] PHP：构造器属性提升
来源：http://www.52xcode.cn/Article/details/gt2cscjboid.html

public function __construct(private int $id) {}
来源：http://www.52xcode.cn/Article/details/gt2vohpyzrs.html

[U51] PHP：数组解构
来源：http://www.ydjk.org.cn/Article/details/gt2gbwhvrwf.html

[$a, $b] = $arr;
来源：http://www.52xcode.cn/Article/details/gt2ckgvrlcv.html

[U52] PHP：箭头函数
来源：http://www.52xcode.cn/Article/details/gt2eegszrxt.html

$double = fn($x) => $x * 2;
来源：http://www.52xcode.cn/Article/details/gt2zycumics.html

[U53] PHP：空合并运算符
来源：http://www.52xcode.cn/Article/details/gt2kylxqjgg.html

$v = $a ?? $b ?? "default";
来源：http://www.ydjk.org.cn/Article/details/gt2dkiecfxi.html

[U54] PHP：空安全调用
来源：http://www.52xcode.cn/Article/details/gt2cjknuoya.html

$obj?->method()
来源：http://www.ydjk.org.cn/Article/details/gt2mdkuscwa.html

[U55] PHP：match 表达式
来源：http://www.ydjk.org.cn/Article/details/gt2hanlcsgq.html

$s = match($x) { 1 => "一", default => "其他" };
来源：http://www.ydjk.org.cn/Article/details/gt2ianyvugh.html

[U56] PHP：命名参数
来源：http://www.ydjk.org.cn/Article/details/gt2gevvmeop.html

f(a: 1, b: 2)
来源：http://www.52xcode.cn/Article/details/gt2mrjwtmej.html

[U57] PHP：字符串插值
来源：http://www.ydjk.org.cn/Article/details/gt2dtrgjacy.html

"值: {$a}"
来源：http://www.ydjk.org.cn/Article/details/gt2jkexprve.html

[U58] PHP：数组三件套
来源：http://www.ydjk.org.cn/Article/details/gt2nwvufujc.html

array_map($f, $a);  array_filter($a, $f);  array_reduce($a, $f, 0);
来源：http://www.ydjk.org.cn/Article/details/gt2oirfgraj.html

[U59] PHP：自定义排序
来源：http://www.ydjk.org.cn/Article/details/gt2lcbrgjbj.html

usort($arr, fn($a, $b) => $a["age"] <=> $b["age"]);
来源：http://www.52xcode.cn/Article/details/gt2pqtiunzu.html

[U60] PHP：JSON 编解码
来源：http://www.52xcode.cn/Article/details/gt2tgxwjuei.html

json_encode($d, JSON_UNESCAPED_UNICODE);  json_decode($s, true);
来源：http://www.52xcode.cn/Article/details/gt2hhxkynyx.html

[U61] PHP：正则
来源：http://www.52xcode.cn/Article/details/gt2qhcndojh.html

preg_match('/(\d+)/', $s, $m);  preg_replace('/\d+/', '#', $s);
来源：http://www.52xcode.cn/Article/details/gt2kkvorzkx.html

[U62] PHP：日期对象
来源：http://www.ydjk.org.cn/Article/details/gt2qbtlmdvq.html

(new DateTimeImmutable())->format("Y-m-d");
来源：http://www.ydjk.org.cn/Article/details/gt2tbilntxo.html

[U63] PHP：文件读写
来源：http://www.52xcode.cn/Article/details/gt2mlnjjqpp.html

file_get_contents($f);  file_put_contents($f, $data);
来源：http://www.52xcode.cn/Article/details/gt2hgutlhjc.html

[U64] PHP：目录遍历
来源：http://www.ydjk.org.cn/Article/details/gt2nlmiswtv.html

glob("dir/*.php");  scandir("dir");
来源：http://www.ydjk.org.cn/Article/details/gt2otxemsfu.html

[U65] PHP：会话
来源：http://www.52xcode.cn/Article/details/gt2nnrugdst.html

session_start();  $_SESSION["uid"] = 1;
来源：http://www.ydjk.org.cn/Article/details/gt2mxyqpvjb.html

[U66] PHP：设置 Cookie
来源：http://www.52xcode.cn/Article/details/gt2wkutfdge.html

setcookie("token", $v, ["httponly" => true, "samesite" => "Lax"]);
来源：http://www.ydjk.org.cn/Article/details/gt2bqlhomor.html

[U67] PHP：处理文件上传
来源：http://www.ydjk.org.cn/Article/details/gt2mdsbyajn.html

$_FILES["file"]["tmp_name"] 与 move_uploaded_file()
来源：http://www.52xcode.cn/Article/details/gt2fbkmudfi.html

[U68] PHP：PDO 连接
来源：http://www.ydjk.org.cn/Article/details/gt2ledoepvl.html

$pdo = new PDO("mysql:host=localhost;dbname=app", "root", "");
来源：http://www.ydjk.org.cn/Article/details/gt2caqvgdmy.html

[U69] PHP：PDO 预处理
来源：http://www.52xcode.cn/Article/details/gt2ivnanjne.html

$stmt = $pdo->prepare("SELECT * FROM users WHERE id = ?");  $stmt->execute([$id]);
来源：http://www.ydjk.org.cn/Article/details/gt2vgrwkwov.html

[U70] PHP：PDO 事务
来源：http://www.ydjk.org.cn/Article/details/gt2czfeavnl.html

$pdo->beginTransaction();  $pdo->commit();  $pdo->rollBack();
来源：http://www.52xcode.cn/Article/details/gt2csidihdc.html

[U71] PHP：抛出异常
来源：http://www.ydjk.org.cn/Article/details/gt2zdmjqaug.html

throw new RuntimeException("失败", 500);
来源：http://www.52xcode.cn/Article/details/gt2gyoqpfvf.html

[U72] PHP：写错误日志
来源：http://www.52xcode.cn/Article/details/gt2ablnoier.html

error_log("失败: " . $e->getMessage());
来源：http://www.ydjk.org.cn/Article/details/gt2hcitwgnx.html

[U73] PHP：读取 ini 配置
来源：http://www.52xcode.cn/Article/details/gt2cfyuxiwp.html

parse_ini_file("config.ini", true)
来源：http://www.52xcode.cn/Article/details/gt2xqzxxtlr.html

[U74] PHP：读取环境变量
来源：http://www.ydjk.org.cn/Article/details/gt2wupcbpxj.html

getenv("APP_ENV") ?: "production"
来源：http://www.52xcode.cn/Article/details/gt2dzngxvvj.html

[U75] PHP：依赖注入
来源：http://www.ydjk.org.cn/Article/details/gt2vbksodhf.html

composer require psr/container
来源：http://www.ydjk.org.cn/Article/details/gt2imlwbrjc.html

[U76] PHP：简单路由
来源：http://www.ydjk.org.cn/Article/details/gt2gebplhol.html

$path = parse_url($_SERVER["REQUEST_URI"], PHP_URL_PATH);
来源：http://www.52xcode.cn/Article/details/gt2qmchdkas.html

[U77] PHP：模板渲染
来源：http://www.52xcode.cn/Article/details/gt2eajcpekj.html

composer require twig/twig
来源：http://www.52xcode.cn/Article/details/gt2fzxkrvjh.html

[U78] PHP：单元测试
来源：http://www.ydjk.org.cn/Article/details/gt2kxdibiyw.html

composer require --dev phpunit/phpunit
来源：http://www.52xcode.cn/Article/details/gt2wvbyxkfw.html

[U79] PHP：静态分析
来源：http://www.ydjk.org.cn/Article/details/gt2gnjljqyj.html

composer require --dev phpstan/phpstan
来源：http://www.52xcode.cn/Article/details/gt2vpexudnv.html

[U80] PHP：代码规范修复
来源：http://www.52xcode.cn/Article/details/gt2ppkwehiz.html

composer require --dev friendsofphp/php-cs-fixer
来源：http://www.ydjk.org.cn/Article/details/gt2lvrdbhmt.html

[U81] JS：初始化项目
来源：http://www.ydjk.org.cn/Article/details/gt2fgrbsclv.html

npm init -y;  npm i express
来源：http://www.52xcode.cn/Article/details/gt2stiimcek.html

[U82] JS：package.json 脚本
来源：http://www.ydjk.org.cn/Article/details/gt2huvukthg.html

"scripts": { "dev": "vite", "build": "vite build" }
来源：http://www.52xcode.cn/Article/details/gt2iardethr.html

[U83] JS：ES Module 导入导出
来源：http://www.52xcode.cn/Article/details/gt2aosvqepl.html

export const a = 1;  import { a } from "./m.js";
来源：http://www.52xcode.cn/Article/details/gt2hjeahsvv.html

[U84] JS：CommonJS 写法
来源：http://www.52xcode.cn/Article/details/gt2npdemidf.html

module.exports = { a };  const { a } = require("./m");
来源：http://www.52xcode.cn/Article/details/gt2gaagirsz.html

[U85] JS：可选链
来源：http://www.ydjk.org.cn/Article/details/gt2jfkzrobt.html

a?.b?.c
来源：http://www.ydjk.org.cn/Article/details/gt2avggcdoh.html

[U86] JS：空值合并
来源：http://www.52xcode.cn/Article/details/gt2xpodvyyl.html

a ?? b
来源：http://www.52xcode.cn/Article/details/gt2sujiklba.html

[U87] JS：解构默认值
来源：http://www.ydjk.org.cn/Article/details/gt2msptaiqb.html

const { a = 1, b = 2 } = obj;
来源：http://www.ydjk.org.cn/Article/details/gt2sgdxvlvq.html

[U88] JS：对象展开合并
来源：http://www.ydjk.org.cn/Article/details/gt2dchavozd.html

{ ...a, ...b }
来源：http://www.52xcode.cn/Article/details/gt2jwidnwty.html

[U89] JS：数组去重
来源：http://www.ydjk.org.cn/Article/details/gt2stquaasl.html

[...new Set(arr)]
来源：http://www.ydjk.org.cn/Article/details/gt2ecjnojnl.html

[U90] JS：数字数组排序
来源：http://www.ydjk.org.cn/Article/details/gt2fugoiifk.html

[...arr].sort((a, b) => a - b)
来源：http://www.ydjk.org.cn/Article/details/gt2yxssrogd.html

[U91] JS：对象键值遍历
来源：http://www.ydjk.org.cn/Article/details/gt2aerglodn.html

Object.entries(obj).forEach(([k, v]) => {});
来源：http://www.ydjk.org.cn/Article/details/gt2wyjhcxnr.html

[U92] JS：深拷贝
来源：http://www.ydjk.org.cn/Article/details/gt2znuotszh.html

structuredClone(obj)
来源：http://www.52xcode.cn/Article/details/gt2hofxxogn.html

[U93] JS：模板字符串
来源：http://www.52xcode.cn/Article/details/gt2zonihjen.html

`共 ${n} 条`
来源：http://www.52xcode.cn/Article/details/gt2pyoimjiw.html

[U94] JS：箭头函数
来源：http://www.ydjk.org.cn/Article/details/gt2fwstgdgf.html

const double = x => x * 2;
来源：http://www.ydjk.org.cn/Article/details/gt2vuzcjoom.html

[U95] JS：Promise 包装
来源：http://www.ydjk.org.cn/Article/details/gt2grmqmpcr.html

new Promise((resolve, reject) => {})
来源：http://www.ydjk.org.cn/Article/details/gt2ugtzdmys.html

[U96] JS：async/await 与异常
来源：http://www.52xcode.cn/Article/details/gt2aenlyakd.html

try { const d = await f(); } catch (e) { console.error(e); }
来源：http://www.52xcode.cn/Article/details/gt2syqfenrb.html

[U97] JS：并发请求
来源：http://www.ydjk.org.cn/Article/details/gt2nbeqaqug.html

await Promise.all(urls.map(u => fetch(u)))
来源：http://www.52xcode.cn/Article/details/gt2payfbheu.html

[U98] JS：fetch 带 JSON
来源：http://www.52xcode.cn/Article/details/gt2nrqvnsmm.html

await fetch(url, { method: "POST", headers: { "Content-Type": "application/json" }, body: JSON.stringify(d) })
来源：http://www.52xcode.cn/Article/details/gt2qvpxyxuq.html

[U99] JS：事件监听
来源：http://www.ydjk.org.cn/Article/details/gt2jhsxfxwa.html

el.addEventListener("click", e => {})
来源：http://www.ydjk.org.cn/Article/details/gt2bjlqumlc.html

[U100] JS：DOM 查询
来源：http://www.52xcode.cn/Article/details/gt2hcogjpbd.html

document.querySelector(".item")
来源：http://www.ydjk.org.cn/Article/details/gt2uoadxpzy.html

[U101] JS：classList 操作
来源：http://www.ydjk.org.cn/Article/details/gt2jctyfxss.html

el.classList.toggle("active")
来源：http://www.52xcode.cn/Article/details/gt2cmyvldwj.html

[U102] JS：本地存储
来源：http://www.52xcode.cn/Article/details/gt2suaflftw.html

localStorage.setItem("k", JSON.stringify(v))
来源：http://www.52xcode.cn/Article/details/gt2wjhpebwh.html

[U103] JS：定时器
来源：http://www.52xcode.cn/Article/details/gt2bfmungdt.html

setTimeout(fn, 1000);  setInterval(fn, 1000);
来源：http://www.ydjk.org.cn/Article/details/gt2nogrvwhb.html

[U104] JS：防抖
来源：http://www.52xcode.cn/Article/details/gt2opbfvuig.html

const debounce = (fn, ms) => { let t; return (...a) => { clearTimeout(t); t = setTimeout(() => fn(...a), ms); }; };
来源：http://www.ydjk.org.cn/Article/details/gt2wnzzfyvk.html

[U105] JS：节流
来源：http://www.52xcode.cn/Article/details/gt2vhvziaui.html

const throttle = (fn, ms) => { let last = 0; return (...a) => { const n = Date.now(); if (n - last >= ms) { last = n; fn(...a); } }; };
来源：http://www.52xcode.cn/Article/details/gt2lfqvydcg.html

[U106] JS：日期格式化
来源：http://www.52xcode.cn/Article/details/gt2wyvabpfc.html

new Intl.DateTimeFormat("zh-CN", { dateStyle: "medium" }).format(new Date())
来源：http://www.52xcode.cn/Article/details/gt2icqdolfa.html

[U107] JS：数字千分位
来源：http://www.ydjk.org.cn/Article/details/gt2heyskdkw.html

new Intl.NumberFormat("en-US").format(1234567)
来源：http://www.ydjk.org.cn/Article/details/gt2wndmgqqf.html

[U108] JS：随机整数
来源：http://www.52xcode.cn/Article/details/gt2ecwwzzga.html

Math.floor(Math.random() * (max - min + 1)) + min
来源：http://www.52xcode.cn/Article/details/gt2udqsbsdn.html


<!-- 参考信息 -->