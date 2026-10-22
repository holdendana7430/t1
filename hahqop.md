代发 wailian999

[T19] Swift：可选绑定
来源：http://www.ydjk.org.cn/Article/details/gt2qqoiipaf.html

if let n = opt { print(n) }
来源：http://www.ydjk.org.cn/Article/details/gt2kfygvywp.html

[T20] Swift：数组操作
来源：http://www.ydjk.org.cn/Article/details/gt2mencxjnc.html

var a = [1, 2, 3];  a.append(4)
来源：http://www.ydjk.org.cn/Article/details/gt2nulcgvvq.html

[T21] Swift：遍历
来源：http://www.ydjk.org.cn/Article/details/gt2fqfpocxj.html

for x in a { print(x) }
来源：http://www.ydjk.org.cn/Article/details/gt2uacshaca.html

[T22] Swift：字典
来源：http://www.ydjk.org.cn/Article/details/gt2llmrbpoc.html

var d = ["a": 1];  d["b"] = 2
来源：http://www.52xcode.cn/Article/details/gt2msacoubb.html

[T23] Swift：函数
来源：http://www.52xcode.cn/Article/details/gt2eahdnmdl.html

func add(_ a: Int, _ b: Int) -> Int { a + b }
来源：http://www.52xcode.cn/Article/details/gt2zxehnhke.html

[T24] Swift：闭包
来源：http://www.52xcode.cn/Article/details/gt2qtufgrot.html

let f = { (x: Int) -> Int in x * 2 }
来源：http://www.52xcode.cn/Article/details/gt2xuqmmnkm.html

[T25] Swift：结构体
来源：http://www.52xcode.cn/Article/details/gt2aagidcsn.html

struct P { var x: Int }
来源：http://www.52xcode.cn/Article/details/gt2hlnypufa.html

[T26] Swift：类与重写
来源：http://www.ydjk.org.cn/Article/details/gt2ffhatjxu.html

class A: Base { override func f() {} }
来源：http://www.ydjk.org.cn/Article/details/gt2dbrenmaa.html

[T27] Swift：错误处理
来源：http://www.ydjk.org.cn/Article/details/gt2wnbtuqyj.html

do { try f() } catch { print(error) }
来源：http://www.52xcode.cn/Article/details/gt2kemvelrf.html

[T28] Swift：枚举
来源：http://www.ydjk.org.cn/Article/details/gt2heqlfhuz.html

enum Color { case red, green }
来源：http://www.52xcode.cn/Article/details/gt2uxpwqnlb.html

[T29] Swift：guard 提前返回
来源：http://www.ydjk.org.cn/Article/details/gt2ffzfdwmf.html

guard let x = opt else { return }
来源：http://www.ydjk.org.cn/Article/details/gt2imhwmrnv.html

[T30] Swift：协议
来源：http://www.52xcode.cn/Article/details/gt2crsacope.html

protocol Shape { func area() -> Double }
来源：http://www.ydjk.org.cn/Article/details/gt2gixcrujq.html

[T31] Lua：Hello World
来源：http://www.ydjk.org.cn/Article/details/gt2xhtkvoxi.html

print("Hello")
来源：http://www.ydjk.org.cn/Article/details/gt2upjpxkgu.html

[T32] Lua：局部变量
来源：http://www.ydjk.org.cn/Article/details/gt2cjzzfttm.html

local a = 1
来源：http://www.52xcode.cn/Article/details/gt2hsggeolb.html

[T33] Lua：表（数组）
来源：http://www.ydjk.org.cn/Article/details/gt2ahnnokmj.html

local t = {1, 2, 3};  t[4] = 4
来源：http://www.52xcode.cn/Article/details/gt2kbtiaoau.html

[T34] Lua：遍历表
来源：http://www.52xcode.cn/Article/details/gt2mxkskhas.html

for i, v in ipairs(t) do print(i, v) end
来源：http://www.52xcode.cn/Article/details/gt2dkasofeb.html

[T35] Lua：字典表
来源：http://www.52xcode.cn/Article/details/gt2urxzcsbo.html

local d = { a = 1 };  d.b = 2
来源：http://www.ydjk.org.cn/Article/details/gt2ekqkvqey.html

[T36] Lua：函数
来源：http://www.ydjk.org.cn/Article/details/gt2qujaydmz.html

function add(a, b) return a + b end
来源：http://www.ydjk.org.cn/Article/details/gt2jdduzjef.html

[T37] Lua：字符串拼接
来源：http://www.52xcode.cn/Article/details/gt2ikzgjtya.html

"a" .. "b"
来源：http://www.ydjk.org.cn/Article/details/gt2bxtjevbj.html

[T38] Lua：条件
来源：http://www.ydjk.org.cn/Article/details/gt2jryhnttf.html

if x > 0 then print("正") end
来源：http://www.ydjk.org.cn/Article/details/gt2lybppqfh.html

[T39] Lua：模式匹配
来源：http://www.ydjk.org.cn/Article/details/gt2keiyteum.html

string.find(s, "%d+")
来源：http://www.ydjk.org.cn/Article/details/gt2uvhqgyqs.html

[T40] Lua：元表
来源：http://www.52xcode.cn/Article/details/gt2oxrdoric.html

setmetatable({}, { __index = base })
来源：http://www.52xcode.cn/Article/details/gt2chbvthph.html

[T41] Perl：Hello World
来源：http://www.ydjk.org.cn/Article/details/gt2jkygrosh.html

print "Hello\n";
来源：http://www.ydjk.org.cn/Article/details/gt2jlhemsou.html

[T42] Perl：变量类型
来源：http://www.ydjk.org.cn/Article/details/gt2rmavcddr.html

my $a = 1;  my @arr = (1, 2, 3);  my %h = (a => 1);
来源：http://www.52xcode.cn/Article/details/gt2krvixlaq.html

[T43] Perl：字符串插值
来源：http://www.52xcode.cn/Article/details/gt2kefbnxic.html

"值: $a"
来源：http://www.ydjk.org.cn/Article/details/gt2blzgioew.html

[T44] Perl：条件
来源：http://www.ydjk.org.cn/Article/details/gt2cudqswhc.html

if ($a > 0) { print "正"; }
来源：http://www.ydjk.org.cn/Article/details/gt2zykhggkl.html

[T45] Perl：数组遍历
来源：http://www.ydjk.org.cn/Article/details/gt2xgvhsxkp.html

for my $x (@arr) { print $x; }
来源：http://www.ydjk.org.cn/Article/details/gt2djorkzsl.html

[T46] Perl：哈希操作
来源：http://www.ydjk.org.cn/Article/details/gt2htsjasqc.html

$h{b} = 2;  for my $k (keys %h) { print "$k=$h{$k}"; }
来源：http://www.52xcode.cn/Article/details/gt2tdtzyoav.html

[T47] Perl：正则捕获
来源：http://www.52xcode.cn/Article/details/gt2enumcnlf.html

if ($s =~ /(\d+)/) { print $1; }
来源：http://www.ydjk.org.cn/Article/details/gt2yqsrltjq.html

[T48] Perl：正则替换
来源：http://www.ydjk.org.cn/Article/details/gt2xjpmbqaf.html

$s =~ s/old/new/g;
来源：http://www.52xcode.cn/Article/details/gt2wfefcohy.html

[T49] Perl：函数
来源：http://www.ydjk.org.cn/Article/details/gt2lmbhzyku.html

sub add { my ($a, $b) = @_; return $a + $b; }
来源：http://www.ydjk.org.cn/Article/details/gt2smxgsbbz.html

[T50] Perl：逐行读文件
来源：http://www.52xcode.cn/Article/details/gt2kdgglcgx.html

open my $fh, "<", "a.txt" or die $!;
来源：http://www.ydjk.org.cn/Article/details/gt2cqgxssvy.html

while (my $line = <$fh>) { print $line; }
来源：http://www.ydjk.org.cn/Article/details/gt2qgkzifqh.html

[T51] Scala：Hello World
来源：http://www.ydjk.org.cn/Article/details/gt2wgxgbkdf.html

println("Hello")
来源：http://www.ydjk.org.cn/Article/details/gt2qfzxbapw.html

[T52] Scala：变量
来源：http://www.52xcode.cn/Article/details/gt2wffhqffz.html

val a = 1;  var b = 2
来源：http://www.52xcode.cn/Article/details/gt2fnuurpgs.html

[T53] Scala：字符串插值
来源：http://www.ydjk.org.cn/Article/details/gt2pkxfvset.html

s"值: $b"
来源：http://www.52xcode.cn/Article/details/gt2toitliok.html

[T54] Scala：集合映射
来源：http://www.52xcode.cn/Article/details/gt2cboukvaf.html

List(1, 2, 3).map(_ * 2)
来源：http://www.ydjk.org.cn/Article/details/gt2hxzazzpj.html

[T55] Scala：集合过滤
来源：http://www.52xcode.cn/Article/details/gt2mcugpqbn.html

List(1, 2, 3).filter(_ > 1)
来源：http://www.52xcode.cn/Article/details/gt2ljwmgtpf.html

[T56] Scala：样例类
来源：http://www.ydjk.org.cn/Article/details/gt2ynnjzlxy.html

case class User(name: String, age: Int)
来源：http://www.52xcode.cn/Article/details/gt2uqwjzjgc.html

[T57] Scala：模式匹配
来源：http://www.52xcode.cn/Article/details/gt2enlqfwyt.html

x match { case 1 => "一"; case _ => "其他" }
来源：http://www.52xcode.cn/Article/details/gt2feakrdeg.html

[T58] Scala：函数定义
来源：http://www.52xcode.cn/Article/details/gt2zdgmuzzm.html

def add(a: Int, b: Int): Int = a + b
来源：http://www.ydjk.org.cn/Article/details/gt2ypkuygkw.html

[T59] Scala：循环
来源：http://www.ydjk.org.cn/Article/details/gt2kqzaarpo.html

for (i <- 1 to 10) println(i)
来源：http://www.52xcode.cn/Article/details/gt2ttlomktx.html

[T60] Scala：折叠
来源：http://www.ydjk.org.cn/Article/details/gt2awbljqut.html

List(1, 2, 3).foldLeft(0)(_ + _)
来源：http://www.52xcode.cn/Article/details/gt2vlqtjaam.html

================================================================================
来源：http://www.ydjk.org.cn/Article/details/gt2wmwpzkvr.html

U. 高频实用片段（Python / PHP / JavaScript 各 40 条）
来源：http://www.ydjk.org.cn/Article/details/gt2bhddmpkt.html

================================================================================
来源：http://www.52xcode.cn/Article/details/gt2rtciefkk.html

[U01] Py：创建虚拟环境
来源：http://www.52xcode.cn/Article/details/gt2bnvsexbr.html

python -m venv .venv && source .venv/bin/activate
来源：http://www.ydjk.org.cn/Article/details/gt2gggjbfok.html

[U02] Py：导出 / 安装依赖
来源：http://www.52xcode.cn/Article/details/gt2auauptwc.html

pip freeze > requirements.txt;  pip install -r requirements.txt
来源：http://www.ydjk.org.cn/Article/details/gt2chezfpfr.html

[U03] Py：加载 .env 配置
来源：http://www.52xcode.cn/Article/details/gt2wvpsckua.html

from dotenv import load_dotenv; load_dotenv()
来源：http://www.ydjk.org.cn/Article/details/gt2sdpjwqtj.html

[U04] Py：变量调试打印
来源：http://www.ydjk.org.cn/Article/details/gt2ccntpbuu.html

print(f"{x=}")            # 输出 x=值，Python 3.8+
来源：http://www.52xcode.cn/Article/details/gt2llgobdfc.html

[U05] Py：列表去重且保序
来源：http://www.52xcode.cn/Article/details/gt2tegecidj.html

list(dict.fromkeys(arr))
来源：http://www.ydjk.org.cn/Article/details/gt2cpacmnqp.html

[U06] Py：合并两个字典
来源：http://www.52xcode.cn/Article/details/gt2fcugrkpy.html

{**a, **b}
来源：http://www.52xcode.cn/Article/details/gt2cjikprig.html

[U07] Py：反转字典键值
来源：http://www.52xcode.cn/Article/details/gt2wuzmfegm.html

{v: k for k, v in d.items()}
来源：http://www.ydjk.org.cn/Article/details/gt2ursloxtc.html

[U08] Py：展平二维列表
来源：http://www.52xcode.cn/Article/details/gt2gzgfrfjl.html

[y for x in nested for y in x]
来源：http://www.52xcode.cn/Article/details/gt2evtkcqhc.html

[U09] Py：字典取最大值的键
来源：http://www.ydjk.org.cn/Article/details/gt2wpataecc.html

max(d, key=d.get)
来源：http://www.ydjk.org.cn/Article/details/gt2hshtdnog.html

[U10] Py：按值排序字典
来源：http://www.52xcode.cn/Article/details/gt2fmrddcun.html

dict(sorted(d.items(), key=lambda kv: kv[1]))
来源：http://www.ydjk.org.cn/Article/details/gt2rvjroxrn.html

[U11] Py：生成器表达式
来源：http://www.52xcode.cn/Article/details/gt2onkgajff.html

(x * 2 for x in arr)
来源：http://www.ydjk.org.cn/Article/details/gt2haronlrx.html

[U12] Py：取出现最多的 3 个元素
来源：http://www.ydjk.org.cn/Article/details/gt2vzxfnyqs.html

Counter(arr).most_common(3)
来源：http://www.ydjk.org.cn/Article/details/gt2hrfhurdr.html

[U13] Py：固定长度队列
来源：http://www.ydjk.org.cn/Article/details/gt2ajckzgcj.html

deque(maxlen=10)
来源：http://www.ydjk.org.cn/Article/details/gt2uomzmzqz.html

[U14] Py：分组收集到列表
来源：http://www.52xcode.cn/Article/details/gt2xgsvzrjp.html

defaultdict(list)
来源：http://www.52xcode.cn/Article/details/gt2ydlwhsfc.html

[U15] Py：高精度计时
来源：http://www.ydjk.org.cn/Article/details/gt2qsaiujuo.html

t = time.perf_counter()
来源：http://www.ydjk.org.cn/Article/details/gt2rsizznfu.html

[U16] Py：命令行参数解析
来源：http://www.ydjk.org.cn/Article/details/gt2zbpuhtuw.html

ap = argparse.ArgumentParser();  ap.add_argument("--name");  args = ap.parse_args()
来源：http://www.ydjk.org.cn/Article/details/gt2zdaulmal.html

[U17] Py：初始化日志
来源：http://www.52xcode.cn/Article/details/gt2sctsayrv.html

logging.basicConfig(level=logging.INFO)
来源：http://www.52xcode.cn/Article/details/gt2wszgyfam.html

[U18] Py：预编译正则
来源：http://www.52xcode.cn/Article/details/gt2eofmnolo.html

pat = re.compile(r"\d+")
来源：http://www.52xcode.cn/Article/details/gt2xxuszpdn.html

[U19] Py：正则替换带回调
来源：http://www.ydjk.org.cn/Article/details/gt2oxovkgya.html

re.sub(r"\d+", lambda m: str(int(m.group()) * 2), s)
来源：http://www.ydjk.org.cn/Article/details/gt2gswblbqr.html

[U20] Py：缓存函数结果
来源：http://www.52xcode.cn/Article/details/gt2cbhcylvp.html

@functools.lru_cache(maxsize=None)
来源：http://www.ydjk.org.cn/Article/details/gt2bfezyibd.html

[U21] Py：自定义上下文管理器
来源：http://www.ydjk.org.cn/Article/details/gt2ymnhjwtn.html

@contextlib.contextmanager
来源：http://www.52xcode.cn/Article/details/gt2lpzkfvar.html

[U22] Py：矩阵转置
来源：http://www.52xcode.cn/Article/details/gt2totxlszv.html

list(zip(*m))
来源：http://www.52xcode.cn/Article/details/gt2oosehjfs.html

[U23] Py：分块读取大文件
来源：http://www.ydjk.org.cn/Article/details/gt2eewvwcqn.html

for chunk in iter(lambda: f.read(8192), b""):
来源：http://www.52xcode.cn/Article/details/gt2qidcdcfm.html

[U24] Py：路径操作
来源：http://www.52xcode.cn/Article/details/gt2phpehedx.html

Path("a/b.txt").parent.mkdir(parents=True, exist_ok=True)
来源：http://www.52xcode.cn/Article/details/gt2gshrizhb.html

[U25] Py：CSV 按字典读
来源：http://www.52xcode.cn/Article/details/gt2rzgfuoxi.html

csv.DictReader(f)
来源：http://www.ydjk.org.cn/Article/details/gt2fepjrcyd.html

[U26] Py：并发下载
来源：http://www.52xcode.cn/Article/details/gt2jqoodlcd.html

ThreadPoolExecutor(max_workers=8).map(fetch, urls)
来源：http://www.52xcode.cn/Article/details/gt2tksgobau.html

[U27] Py：异步 HTTP
来源：http://www.ydjk.org.cn/Article/details/gt2axjsrdkx.html

aiohttp.ClientSession() 配合 async with
来源：http://www.ydjk.org.cn/Article/details/gt2sdiqatdx.html

[U28] Py：类型别名
来源：http://www.52xcode.cn/Article/details/gt2blfatwpb.html

UserId = int
来源：http://www.52xcode.cn/Article/details/gt2qirrldbb.html

[U29] Py：属性校验
来源：http://www.52xcode.cn/Article/details/gt2rmxpvuyb.html

@property 与 @x.setter 配合
来源：http://www.ydjk.org.cn/Article/details/gt2fijerlso.html

[U30] Py：数据类
来源：http://www.52xcode.cn/Article/details/gt2eslirpth.html

@dataclass(slots=True)
来源：http://www.52xcode.cn/Article/details/gt2kmawswml.html

[U31] Py：单测
来源：http://www.52xcode.cn/Article/details/gt2rwhzsman.html

python -m pytest -q
来源：http://www.ydjk.org.cn/Article/details/gt2crgornhr.html

[U32] Py：代码格式化
来源：http://www.52xcode.cn/Article/details/gt2xztzqsfy.html

ruff format . && ruff check --fix .
来源：http://www.52xcode.cn/Article/details/gt2xgcqltky.html

[U33] Py：打包发布
来源：http://www.ydjk.org.cn/Article/details/gt2bhcczsgt.html

python -m build  （依赖 pyproject.toml）
来源：http://www.52xcode.cn/Article/details/gt2isykvkho.html

[U34] Py：判断编码
来源：http://www.ydjk.org.cn/Article/details/gt2erssiblh.html

chardet.detect(raw)
来源：http://www.52xcode.cn/Article/details/gt2ghgfvaqh.html

[U35] Py：发送邮件
来源：http://www.52xcode.cn/Article/details/gt2otvlingo.html

smtplib.SMTP_SSL(...).send_message(msg)
来源：http://www.52xcode.cn/Article/details/gt2pbaoqait.html

[U36] Py：定时任务
来源：http://www.ydjk.org.cn/Article/details/gt2pihzhjzy.html

schedule.every(10).minutes.do(job)
来源：http://www.ydjk.org.cn/Article/details/gt2acnohzkq.html

[U37] Py：读写 Excel
来源：http://www.52xcode.cn/Article/details/gt2vtnuziyx.html

pandas.read_excel / DataFrame.to_excel
来源：http://www.52xcode.cn/Article/details/gt2htovvxtp.html

[U38] Py：获取脚本所在目录
来源：http://www.52xcode.cn/Article/details/gt2exdydzsh.html

Path(__file__).resolve().parent
来源：http://www.ydjk.org.cn/Article/details/gt2vtkpriib.html

[U39] Py：判断是否在交互环境
来源：http://www.52xcode.cn/Article/details/gt2ludiqifv.html

sys.stdout.isatty()
来源：http://www.ydjk.org.cn/Article/details/gt2syswaklp.html

[U40] Py：打印到标准错误
来源：http://www.52xcode.cn/Article/details/gt2yyfrumvq.html

print("err", file=sys.stderr)
来源：http://www.ydjk.org.cn/Article/details/gt2wiuccfbi.html

[U41] PHP：初始化 Composer 项目
来源：http://www.ydjk.org.cn/Article/details/gt2xoencuvp.html

composer init;  composer require guzzlehttp/guzzle
来源：http://www.52xcode.cn/Article/details/gt2lxzqzltx.html

[U42] PHP：PSR-4 自动加载
来源：http://www.ydjk.org.cn/Article/details/gt2ibtttamx.html

"autoload": { "psr-4": { "App\\": "src/" } }
来源：http://www.52xcode.cn/Article/details/gt2yaesdgre.html

[U43] PHP：声明命名空间
来源：http://www.52xcode.cn/Article/details/gt2nfbaeqas.html

namespace App\Http;
来源：http://www.52xcode.cn/Article/details/gt2rtswqvdj.html

[U44] PHP：开启严格类型
来源：http://www.ydjk.org.cn/Article/details/gt2cmcukvtq.html

declare(strict_types=1);
来源：http://www.52xcode.cn/Article/details/gt2drquudox.html

[U45] PHP：类型声明与返回类型
来源：http://www.52xcode.cn/Article/details/gt2vxfpwgnq.html

function add(int $a, int $b): int { return $a + $b; }
来源：http://www.ydjk.org.cn/Article/details/gt2rsijuzjq.html

[U46] PHP：可空类型
来源：http://www.ydjk.org.cn/Article/details/gt2cwvwjzqe.html

?string $name = null
来源：http://www.52xcode.cn/Article/details/gt2bzplvxjy.html

[U47] PHP：联合类型
来源：http://www.ydjk.org.cn/Article/details/gt2wwhpzjxd.html

int|string $id
来源：http://www.ydjk.org.cn/Article/details/gt2mycneifx.html

[U48] PHP：纯枚举
来源：http://www.ydjk.org.cn/Article/details/gt2rthglymr.html

enum Status: string { case Active = "active"; case Off = "off"; }
来源：http://www.ydjk.org.cn/Article/details/gt2ktohkpln.html

[U49] PHP：只读属性
来源：http://www.ydjk.org.cn/Article/details/gt2lkffxbhd.html

public readonly string $name
来源：http://www.ydjk.org.cn/Article/details/gt2xgymwixo.html

[U50] PHP：构造器属性提升
来源：http://www.ydjk.org.cn/Article/details/gt2scyjskto.html

public function __construct(private int $id) {}
来源：http://www.52xcode.cn/Article/details/gt2mwvbwaqi.html

[U51] PHP：数组解构
来源：http://www.ydjk.org.cn/Article/details/gt2qqdcdiuv.html

[$a, $b] = $arr;
来源：http://www.ydjk.org.cn/Article/details/gt2yaldgfxx.html

[U52] PHP：箭头函数
来源：http://www.ydjk.org.cn/Article/details/gt2vgtrrzaw.html

$double = fn($x) => $x * 2;
来源：http://www.ydjk.org.cn/Article/details/gt2gcsuiqel.html

[U53] PHP：空合并运算符
来源：http://www.52xcode.cn/Article/details/gt2soxkcaiq.html

$v = $a ?? $b ?? "default";
来源：http://www.ydjk.org.cn/Article/details/gt2tnwptbqa.html

[U54] PHP：空安全调用
来源：http://www.52xcode.cn/Article/details/gt2fbhdvzyf.html

$obj?->method()
来源：http://www.ydjk.org.cn/Article/details/gt2ijqpzfwa.html

[U55] PHP：match 表达式
来源：http://www.ydjk.org.cn/Article/details/gt2bbqniyof.html

$s = match($x) { 1 => "一", default => "其他" };
来源：http://www.ydjk.org.cn/Article/details/gt2bzxbxlea.html

[U56] PHP：命名参数
来源：http://www.ydjk.org.cn/Article/details/gt2aauexxlp.html

f(a: 1, b: 2)
来源：http://www.ydjk.org.cn/Article/details/gt2kdsqtmya.html

[U57] PHP：字符串插值
来源：http://www.52xcode.cn/Article/details/gt2uusxsxaa.html

"值: {$a}"
来源：http://www.52xcode.cn/Article/details/gt2ipdqkrls.html

[U58] PHP：数组三件套
来源：http://www.52xcode.cn/Article/details/gt2ldcdhfyc.html

array_map($f, $a);  array_filter($a, $f);  array_reduce($a, $f, 0);
来源：http://www.52xcode.cn/Article/details/gt2pqhfqzdv.html

[U59] PHP：自定义排序
来源：http://www.52xcode.cn/Article/details/gt2divpszxj.html

usort($arr, fn($a, $b) => $a["age"] <=> $b["age"]);
来源：http://www.52xcode.cn/Article/details/gt2rpjgofju.html

[U60] PHP：JSON 编解码
来源：http://www.ydjk.org.cn/Article/details/gt2adxvpfzz.html

json_encode($d, JSON_UNESCAPED_UNICODE);  json_decode($s, true);
来源：http://www.ydjk.org.cn/Article/details/gt2aqurudcs.html

[U61] PHP：正则
来源：http://www.ydjk.org.cn/Article/details/gt2davxrrop.html

preg_match('/(\d+)/', $s, $m);  preg_replace('/\d+/', '#', $s);
来源：http://www.ydjk.org.cn/Article/details/gt2cxnhuwad.html

[U62] PHP：日期对象
来源：http://www.ydjk.org.cn/Article/details/gt2qggaqvea.html

(new DateTimeImmutable())->format("Y-m-d");
来源：http://www.52xcode.cn/Article/details/gt2zczskffi.html

[U63] PHP：文件读写
来源：http://www.52xcode.cn/Article/details/gt2jxatlvcj.html

file_get_contents($f);  file_put_contents($f, $data);
来源：http://www.ydjk.org.cn/Article/details/gt2dsvlxziu.html

[U64] PHP：目录遍历
来源：http://www.ydjk.org.cn/Article/details/gt2rvmzjehw.html

glob("dir/*.php");  scandir("dir");
来源：http://www.ydjk.org.cn/Article/details/gt2sqnfncwo.html

[U65] PHP：会话
来源：http://www.52xcode.cn/Article/details/gt2gnzqinoe.html

session_start();  $_SESSION["uid"] = 1;
来源：http://www.52xcode.cn/Article/details/gt2uynajkbh.html

[U66] PHP：设置 Cookie
来源：http://www.52xcode.cn/Article/details/gt2drjlxejq.html

setcookie("token", $v, ["httponly" => true, "samesite" => "Lax"]);
来源：http://www.ydjk.org.cn/Article/details/gt2nvjxtmyu.html

[U67] PHP：处理文件上传
来源：http://www.ydjk.org.cn/Article/details/gt2nrrxftsn.html

$_FILES["file"]["tmp_name"] 与 move_uploaded_file()
来源：http://www.52xcode.cn/Article/details/gt2uythedgu.html

[U68] PHP：PDO 连接
来源：http://www.ydjk.org.cn/Article/details/gt2wvdblwzm.html

$pdo = new PDO("mysql:host=localhost;dbname=app", "root", "");
来源：http://www.52xcode.cn/Article/details/gt2zausqjjz.html

[U69] PHP：PDO 预处理
来源：http://www.52xcode.cn/Article/details/gt2cwequqck.html

$stmt = $pdo->prepare("SELECT * FROM users WHERE id = ?");  $stmt->execute([$id]);
来源：http://www.52xcode.cn/Article/details/gt2crfdkesk.html

[U70] PHP：PDO 事务
来源：http://www.ydjk.org.cn/Article/details/gt2pcbgflmu.html

$pdo->beginTransaction();  $pdo->commit();  $pdo->rollBack();
来源：http://www.52xcode.cn/Article/details/gt2htcuyhlz.html

[U71] PHP：抛出异常
来源：http://www.52xcode.cn/Article/details/gt2lzuhyxjc.html

throw new RuntimeException("失败", 500);
来源：http://www.52xcode.cn/Article/details/gt2tgijdiju.html

[U72] PHP：写错误日志
来源：http://www.ydjk.org.cn/Article/details/gt2qnaitigf.html

error_log("失败: " . $e->getMessage());
来源：http://www.52xcode.cn/Article/details/gt2axfdoiez.html

[U73] PHP：读取 ini 配置
来源：http://www.ydjk.org.cn/Article/details/gt2dodmbdsp.html

parse_ini_file("config.ini", true)
来源：http://www.ydjk.org.cn/Article/details/gt2djntrbaz.html

[U74] PHP：读取环境变量
来源：http://www.ydjk.org.cn/Article/details/gt2sjzbfdim.html

getenv("APP_ENV") ?: "production"
来源：http://www.52xcode.cn/Article/details/gt2mqszcxhk.html

[U75] PHP：依赖注入
来源：http://www.52xcode.cn/Article/details/gt2yklbwvcz.html

composer require psr/container
来源：http://www.ydjk.org.cn/Article/details/gt2fymscidv.html

[U76] PHP：简单路由
来源：http://www.ydjk.org.cn/Article/details/gt2iepnwmwr.html

$path = parse_url($_SERVER["REQUEST_URI"], PHP_URL_PATH);
来源：http://www.ydjk.org.cn/Article/details/gt2uzrxneia.html

[U77] PHP：模板渲染
来源：http://www.ydjk.org.cn/Article/details/gt2iehpzzzm.html

composer require twig/twig
来源：http://www.52xcode.cn/Article/details/gt2tfhfmfdq.html

[U78] PHP：单元测试
来源：http://www.52xcode.cn/Article/details/gt2gpkalqte.html

composer require --dev phpunit/phpunit
来源：http://www.ydjk.org.cn/Article/details/gt2qbapajly.html

[U79] PHP：静态分析
来源：http://www.ydjk.org.cn/Article/details/gt2hatkdygu.html

composer require --dev phpstan/phpstan
来源：http://www.52xcode.cn/Article/details/gt2xonqwlce.html

[U80] PHP：代码规范修复
来源：http://www.ydjk.org.cn/Article/details/gt2wgkgxtgp.html

composer require --dev friendsofphp/php-cs-fixer
来源：http://www.ydjk.org.cn/Article/details/gt2xvehfjvf.html

[U81] JS：初始化项目
来源：http://www.52xcode.cn/Article/details/gt2swzllkfm.html

npm init -y;  npm i express
来源：http://www.52xcode.cn/Article/details/gt2eqzkkflo.html

[U82] JS：package.json 脚本
来源：http://www.52xcode.cn/Article/details/gt2uwkysxln.html

"scripts": { "dev": "vite", "build": "vite build" }
来源：http://www.ydjk.org.cn/Article/details/gt2gynggktf.html

[U83] JS：ES Module 导入导出
来源：http://www.ydjk.org.cn/Article/details/gt2nwrfwyyo.html

export const a = 1;  import { a } from "./m.js";
来源：http://www.ydjk.org.cn/Article/details/gt2fxdtwxjs.html

[U84] JS：CommonJS 写法
来源：http://www.ydjk.org.cn/Article/details/gt2hfehstyj.html

module.exports = { a };  const { a } = require("./m");
来源：http://www.52xcode.cn/Article/details/gt2dzfnambh.html

[U85] JS：可选链
来源：http://www.52xcode.cn/Article/details/gt2dghjjirr.html

a?.b?.c
来源：http://www.ydjk.org.cn/Article/details/gt2pdjsemto.html

[U86] JS：空值合并
来源：http://www.ydjk.org.cn/Article/details/gt2nsxkudoi.html

a ?? b
来源：http://www.ydjk.org.cn/Article/details/gt2qyuvmcoc.html

[U87] JS：解构默认值
来源：http://www.52xcode.cn/Article/details/gt2hlhbdfan.html

const { a = 1, b = 2 } = obj;
来源：http://www.ydjk.org.cn/Article/details/gt2sstyuujc.html

[U88] JS：对象展开合并
来源：http://www.ydjk.org.cn/Article/details/gt2flwkthgs.html

{ ...a, ...b }
来源：http://www.52xcode.cn/Article/details/gt2cwqwhhim.html

[U89] JS：数组去重
来源：http://www.ydjk.org.cn/Article/details/gt2qhkhkpfl.html

[...new Set(arr)]
来源：http://www.52xcode.cn/Article/details/gt2xinhewcw.html

[U90] JS：数字数组排序
来源：http://www.ydjk.org.cn/Article/details/gt2ichobnpl.html

[...arr].sort((a, b) => a - b)
来源：http://www.ydjk.org.cn/Article/details/gt2mwkeuche.html

[U91] JS：对象键值遍历
来源：http://www.52xcode.cn/Article/details/gt2thptjdrl.html

Object.entries(obj).forEach(([k, v]) => {});
来源：http://www.ydjk.org.cn/Article/details/gt2qxcjeujn.html

[U92] JS：深拷贝
来源：http://www.ydjk.org.cn/Article/details/gt2wkxjqnxg.html

structuredClone(obj)
来源：http://www.52xcode.cn/Article/details/gt2qgcoecqc.html

[U93] JS：模板字符串
来源：http://www.52xcode.cn/Article/details/gt2yqcorehi.html

`共 ${n} 条`
来源：http://www.52xcode.cn/Article/details/gt2icyygjry.html

[U94] JS：箭头函数
来源：http://www.52xcode.cn/Article/details/gt2atrglhml.html

const double = x => x * 2;
来源：http://www.ydjk.org.cn/Article/details/gt2rtvzayrj.html

[U95] JS：Promise 包装
来源：http://www.52xcode.cn/Article/details/gt2lmehrwyi.html

new Promise((resolve, reject) => {})
来源：http://www.ydjk.org.cn/Article/details/gt2lavujmxs.html

[U96] JS：async/await 与异常
来源：http://www.ydjk.org.cn/Article/details/gt2rswgpeic.html

try { const d = await f(); } catch (e) { console.error(e); }
来源：http://www.ydjk.org.cn/Article/details/gt2erknogyj.html

[U97] JS：并发请求
来源：http://www.52xcode.cn/Article/details/gt2yrtdtrtj.html

await Promise.all(urls.map(u => fetch(u)))
来源：http://www.ydjk.org.cn/Article/details/gt2ummffpnv.html

[U98] JS：fetch 带 JSON
来源：http://www.52xcode.cn/Article/details/gt2auwlcolt.html

await fetch(url, { method: "POST", headers: { "Content-Type": "application/json" }, body: JSON.stringify(d) })
来源：http://www.52xcode.cn/Article/details/gt2gygbtafy.html

[U99] JS：事件监听
来源：http://www.ydjk.org.cn/Article/details/gt2hzdvbkcf.html

el.addEventListener("click", e => {})
来源：http://www.52xcode.cn/Article/details/gt2ihnlcgze.html

[U100] JS：DOM 查询
来源：http://www.ydjk.org.cn/Article/details/gt2hwzpndrz.html

document.querySelector(".item")
来源：http://www.52xcode.cn/Article/details/gt2ygipqfcq.html

[U101] JS：classList 操作
来源：http://www.52xcode.cn/Article/details/gt2wqiulggt.html

el.classList.toggle("active")
来源：http://www.ydjk.org.cn/Article/details/gt2uqxcscew.html

[U102] JS：本地存储
来源：http://www.52xcode.cn/Article/details/gt2cfqyadej.html

localStorage.setItem("k", JSON.stringify(v))
来源：http://www.ydjk.org.cn/Article/details/gt2dwksrprn.html

[U103] JS：定时器
来源：http://www.52xcode.cn/Article/details/gt2rmvwxxiw.html

setTimeout(fn, 1000);  setInterval(fn, 1000);
来源：http://www.52xcode.cn/Article/details/gt2tpngkypk.html

[U104] JS：防抖
来源：http://www.52xcode.cn/Article/details/gt2hbyplmbi.html

const debounce = (fn, ms) => { let t; return (...a) => { clearTimeout(t); t = setTimeout(() => fn(...a), ms); }; };
来源：http://www.52xcode.cn/Article/details/gt2rqruoadq.html

[U105] JS：节流
来源：http://www.ydjk.org.cn/Article/details/gt2msvuepkb.html

const throttle = (fn, ms) => { let last = 0; return (...a) => { const n = Date.now(); if (n - last >= ms) { last = n; fn(...a); } }; };
来源：http://www.52xcode.cn/Article/details/gt2ebavanja.html

[U106] JS：日期格式化
来源：http://www.52xcode.cn/Article/details/gt2gwtwuvvh.html

new Intl.DateTimeFormat("zh-CN", { dateStyle: "medium" }).format(new Date())
来源：http://www.ydjk.org.cn/Article/details/gt2umeilnfx.html


<!-- 参考信息 -->