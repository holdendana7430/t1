代发 wailian999

[T23] Swift：函数
来源：http://www.52xcode.cn/Article/details/gt2upigjspv.html

func add(_ a: Int, _ b: Int) -> Int { a + b }
来源：http://www.ydjk.org.cn/Article/details/gt2hsdnhwub.html

[T24] Swift：闭包
来源：http://www.52xcode.cn/Article/details/gt2sqqbxcnq.html

let f = { (x: Int) -> Int in x * 2 }
来源：http://www.ydjk.org.cn/Article/details/gt2lttdzhtd.html

[T25] Swift：结构体
来源：http://www.ydjk.org.cn/Article/details/gt2ruorjvug.html

struct P { var x: Int }
来源：http://www.52xcode.cn/Article/details/gt2pomxnech.html

[T26] Swift：类与重写
来源：http://www.ydjk.org.cn/Article/details/gt2cbxxzqtn.html

class A: Base { override func f() {} }
来源：http://www.ydjk.org.cn/Article/details/gt2bawwbzvj.html

[T27] Swift：错误处理
来源：http://www.52xcode.cn/Article/details/gt2luzttzxb.html

do { try f() } catch { print(error) }
来源：http://www.52xcode.cn/Article/details/gt2sptzjjun.html

[T28] Swift：枚举
来源：http://www.ydjk.org.cn/Article/details/gt2eukmxaqc.html

enum Color { case red, green }
来源：http://www.ydjk.org.cn/Article/details/gt2isxfwepr.html

[T29] Swift：guard 提前返回
来源：http://www.ydjk.org.cn/Article/details/gt2vkwahztq.html

guard let x = opt else { return }
来源：http://www.ydjk.org.cn/Article/details/gt2twvufsls.html

[T30] Swift：协议
来源：http://www.52xcode.cn/Article/details/gt2yicfxrsy.html

protocol Shape { func area() -> Double }
来源：http://www.ydjk.org.cn/Article/details/gt2dqctuuoh.html

[T31] Lua：Hello World
来源：http://www.52xcode.cn/Article/details/gt2scbgmcqs.html

print("Hello")
来源：http://www.52xcode.cn/Article/details/gt2drkaepam.html

[T32] Lua：局部变量
来源：http://www.ydjk.org.cn/Article/details/gt2lhfqfamj.html

local a = 1
来源：http://www.ydjk.org.cn/Article/details/gt2eflcjcxi.html

[T33] Lua：表（数组）
来源：http://www.ydjk.org.cn/Article/details/gt2mbsgwhqp.html

local t = {1, 2, 3};  t[4] = 4
来源：http://www.ydjk.org.cn/Article/details/gt2ujigufck.html

[T34] Lua：遍历表
来源：http://www.52xcode.cn/Article/details/gt2rngimuux.html

for i, v in ipairs(t) do print(i, v) end
来源：http://www.ydjk.org.cn/Article/details/gt2aprtyusf.html

[T35] Lua：字典表
来源：http://www.52xcode.cn/Article/details/gt2yvcfzvqs.html

local d = { a = 1 };  d.b = 2
来源：http://www.52xcode.cn/Article/details/gt2wqblctal.html

[T36] Lua：函数
来源：http://www.ydjk.org.cn/Article/details/gt2nthipayq.html

function add(a, b) return a + b end
来源：http://www.ydjk.org.cn/Article/details/gt2jjpdkixh.html

[T37] Lua：字符串拼接
来源：http://www.52xcode.cn/Article/details/gt2rpylugej.html

"a" .. "b"
来源：http://www.52xcode.cn/Article/details/gt2zhspbcho.html

[T38] Lua：条件
来源：http://www.52xcode.cn/Article/details/gt2fdicwbuk.html

if x > 0 then print("正") end
来源：http://www.ydjk.org.cn/Article/details/gt2zghtfcct.html

[T39] Lua：模式匹配
来源：http://www.ydjk.org.cn/Article/details/gt2bfvekjik.html

string.find(s, "%d+")
来源：http://www.ydjk.org.cn/Article/details/gt2qaftjeny.html

[T40] Lua：元表
来源：http://www.52xcode.cn/Article/details/gt2uiafzwen.html

setmetatable({}, { __index = base })
来源：http://www.52xcode.cn/Article/details/gt2dslruhya.html

[T41] Perl：Hello World
来源：http://www.ydjk.org.cn/Article/details/gt2vpstbjsn.html

print "Hello\n";
来源：http://www.ydjk.org.cn/Article/details/gt2hhlverhi.html

[T42] Perl：变量类型
来源：http://www.52xcode.cn/Article/details/gt2jatxvcrc.html

my $a = 1;  my @arr = (1, 2, 3);  my %h = (a => 1);
来源：http://www.52xcode.cn/Article/details/gt2ejgrxwmv.html

[T43] Perl：字符串插值
来源：http://www.52xcode.cn/Article/details/gt2rdimueol.html

"值: $a"
来源：http://www.ydjk.org.cn/Article/details/gt2ierkxpio.html

[T44] Perl：条件
来源：http://www.52xcode.cn/Article/details/gt2euiavamc.html

if ($a > 0) { print "正"; }
来源：http://www.ydjk.org.cn/Article/details/gt2mntijvic.html

[T45] Perl：数组遍历
来源：http://www.ydjk.org.cn/Article/details/gt2idccquog.html

for my $x (@arr) { print $x; }
来源：http://www.52xcode.cn/Article/details/gt2kvfyuakr.html

[T46] Perl：哈希操作
来源：http://www.52xcode.cn/Article/details/gt2gdmypmnc.html

$h{b} = 2;  for my $k (keys %h) { print "$k=$h{$k}"; }
来源：http://www.52xcode.cn/Article/details/gt2vohxxzgh.html

[T47] Perl：正则捕获
来源：http://www.52xcode.cn/Article/details/gt2cpsymesg.html

if ($s =~ /(\d+)/) { print $1; }
来源：http://www.ydjk.org.cn/Article/details/gt2pxlsnqjo.html

[T48] Perl：正则替换
来源：http://www.ydjk.org.cn/Article/details/gt2zizvihse.html

$s =~ s/old/new/g;
来源：http://www.52xcode.cn/Article/details/gt2stnhehnq.html

[T49] Perl：函数
来源：http://www.ydjk.org.cn/Article/details/gt2iteennyy.html

sub add { my ($a, $b) = @_; return $a + $b; }
来源：http://www.52xcode.cn/Article/details/gt2ufjggxpz.html

[T50] Perl：逐行读文件
来源：http://www.52xcode.cn/Article/details/gt2sazyrifh.html

open my $fh, "<", "a.txt" or die $!;
来源：http://www.ydjk.org.cn/Article/details/gt2wyvinvso.html

while (my $line = <$fh>) { print $line; }
来源：http://www.ydjk.org.cn/Article/details/gt2figyplpw.html

[T51] Scala：Hello World
来源：http://www.ydjk.org.cn/Article/details/gt2dogwufac.html

println("Hello")
来源：http://www.52xcode.cn/Article/details/gt2vqyuatbx.html

[T52] Scala：变量
来源：http://www.ydjk.org.cn/Article/details/gt2cwxfrttw.html

val a = 1;  var b = 2
来源：http://www.52xcode.cn/Article/details/gt2rfxyymws.html

[T53] Scala：字符串插值
来源：http://www.ydjk.org.cn/Article/details/gt2zktewkiy.html

s"值: $b"
来源：http://www.ydjk.org.cn/Article/details/gt2ygozwanc.html

[T54] Scala：集合映射
来源：http://www.ydjk.org.cn/Article/details/gt2ijueucax.html

List(1, 2, 3).map(_ * 2)
来源：http://www.52xcode.cn/Article/details/gt2fjhdgggu.html

[T55] Scala：集合过滤
来源：http://www.52xcode.cn/Article/details/gt2looorohp.html

List(1, 2, 3).filter(_ > 1)
来源：http://www.52xcode.cn/Article/details/gt2bqnumvjs.html

[T56] Scala：样例类
来源：http://www.ydjk.org.cn/Article/details/gt2vtahkjte.html

case class User(name: String, age: Int)
来源：http://www.52xcode.cn/Article/details/gt2pruthcrv.html

[T57] Scala：模式匹配
来源：http://www.ydjk.org.cn/Article/details/gt2dcfmqcfu.html

x match { case 1 => "一"; case _ => "其他" }
来源：http://www.52xcode.cn/Article/details/gt2wnibnzmv.html

[T58] Scala：函数定义
来源：http://www.ydjk.org.cn/Article/details/gt2gifuphij.html

def add(a: Int, b: Int): Int = a + b
来源：http://www.ydjk.org.cn/Article/details/gt2jakvvscl.html

[T59] Scala：循环
来源：http://www.ydjk.org.cn/Article/details/gt2ghrstvhr.html

for (i <- 1 to 10) println(i)
来源：http://www.ydjk.org.cn/Article/details/gt2bvdfbynu.html

[T60] Scala：折叠
来源：http://www.ydjk.org.cn/Article/details/gt2ftbpudzy.html

List(1, 2, 3).foldLeft(0)(_ + _)
来源：http://www.ydjk.org.cn/Article/details/gt2qmvciecl.html

================================================================================
来源：http://www.ydjk.org.cn/Article/details/gt2rkovqssq.html

U. 高频实用片段（Python / PHP / JavaScript 各 40 条）
来源：http://www.ydjk.org.cn/Article/details/gt2vdyjyejo.html

================================================================================
来源：http://www.52xcode.cn/Article/details/gt2aoazfdhm.html

[U01] Py：创建虚拟环境
来源：http://www.ydjk.org.cn/Article/details/gt2jhlofrrz.html

python -m venv .venv && source .venv/bin/activate
来源：http://www.52xcode.cn/Article/details/gt2sgfocdqq.html

[U02] Py：导出 / 安装依赖
来源：http://www.ydjk.org.cn/Article/details/gt2rwljvbyi.html

pip freeze > requirements.txt;  pip install -r requirements.txt
来源：http://www.ydjk.org.cn/Article/details/gt2qaiotonp.html

[U03] Py：加载 .env 配置
来源：http://www.ydjk.org.cn/Article/details/gt2akpogcqm.html

from dotenv import load_dotenv; load_dotenv()
来源：http://www.52xcode.cn/Article/details/gt2umspziff.html

[U04] Py：变量调试打印
来源：http://www.ydjk.org.cn/Article/details/gt2iwwzkcyn.html

print(f"{x=}")            # 输出 x=值，Python 3.8+
来源：http://www.52xcode.cn/Article/details/gt2dcckqeoj.html

[U05] Py：列表去重且保序
来源：http://www.52xcode.cn/Article/details/gt2byfralnr.html

list(dict.fromkeys(arr))
来源：http://www.52xcode.cn/Article/details/gt2rqwsglgq.html

[U06] Py：合并两个字典
来源：http://www.52xcode.cn/Article/details/gt2qsvwlhup.html

{**a, **b}
来源：http://www.52xcode.cn/Article/details/gt2zwmrdbob.html

[U07] Py：反转字典键值
来源：http://www.ydjk.org.cn/Article/details/gt2puttnwdv.html

{v: k for k, v in d.items()}
来源：http://www.ydjk.org.cn/Article/details/gt2avcelpww.html

[U08] Py：展平二维列表
来源：http://www.52xcode.cn/Article/details/gt2cbgolivh.html

[y for x in nested for y in x]
来源：http://www.52xcode.cn/Article/details/gt2svdohetg.html

[U09] Py：字典取最大值的键
来源：http://www.ydjk.org.cn/Article/details/gt2nhvmalcn.html

max(d, key=d.get)
来源：http://www.52xcode.cn/Article/details/gt2sfmjdflm.html

[U10] Py：按值排序字典
来源：http://www.52xcode.cn/Article/details/gt2koaohlds.html

dict(sorted(d.items(), key=lambda kv: kv[1]))
来源：http://www.52xcode.cn/Article/details/gt2slvbvoae.html

[U11] Py：生成器表达式
来源：http://www.ydjk.org.cn/Article/details/gt2wuexomit.html

(x * 2 for x in arr)
来源：http://www.52xcode.cn/Article/details/gt2gseaxaiq.html

[U12] Py：取出现最多的 3 个元素
来源：http://www.52xcode.cn/Article/details/gt2fbtkgqer.html

Counter(arr).most_common(3)
来源：http://www.52xcode.cn/Article/details/gt2snbdqvaz.html

[U13] Py：固定长度队列
来源：http://www.52xcode.cn/Article/details/gt2whuubpwt.html

deque(maxlen=10)
来源：http://www.52xcode.cn/Article/details/gt2aetzhgms.html

[U14] Py：分组收集到列表
来源：http://www.ydjk.org.cn/Article/details/gt2wwpkjodc.html

defaultdict(list)
来源：http://www.52xcode.cn/Article/details/gt2atvcfohs.html

[U15] Py：高精度计时
来源：http://www.52xcode.cn/Article/details/gt2frwlvzop.html

t = time.perf_counter()
来源：http://www.52xcode.cn/Article/details/gt2knwkveeh.html

[U16] Py：命令行参数解析
来源：http://www.52xcode.cn/Article/details/gt2vghpdogq.html

ap = argparse.ArgumentParser();  ap.add_argument("--name");  args = ap.parse_args()
来源：http://www.ydjk.org.cn/Article/details/gt2ippipixw.html

[U17] Py：初始化日志
来源：http://www.ydjk.org.cn/Article/details/gt2aqerdpdd.html

logging.basicConfig(level=logging.INFO)
来源：http://www.52xcode.cn/Article/details/gt2yuwvfsej.html

[U18] Py：预编译正则
来源：http://www.52xcode.cn/Article/details/gt2fpdgwptl.html

pat = re.compile(r"\d+")
来源：http://www.ydjk.org.cn/Article/details/gt2mgihjhyt.html

[U19] Py：正则替换带回调
来源：http://www.52xcode.cn/Article/details/gt2tvzgwgzu.html

re.sub(r"\d+", lambda m: str(int(m.group()) * 2), s)
来源：http://www.ydjk.org.cn/Article/details/gt2kefddkmb.html

[U20] Py：缓存函数结果
来源：http://www.52xcode.cn/Article/details/gt2tqchetjq.html

@functools.lru_cache(maxsize=None)
来源：http://www.ydjk.org.cn/Article/details/gt2yoqmmswm.html

[U21] Py：自定义上下文管理器
来源：http://www.ydjk.org.cn/Article/details/gt2nytxzwfx.html

@contextlib.contextmanager
来源：http://www.ydjk.org.cn/Article/details/gt2cgwnvnka.html

[U22] Py：矩阵转置
来源：http://www.52xcode.cn/Article/details/gt2yibycxlu.html

list(zip(*m))
来源：http://www.52xcode.cn/Article/details/gt2umzqgjed.html

[U23] Py：分块读取大文件
来源：http://www.52xcode.cn/Article/details/gt2lcxexreq.html

for chunk in iter(lambda: f.read(8192), b""):
来源：http://www.ydjk.org.cn/Article/details/gt2uwlemhoj.html

[U24] Py：路径操作
来源：http://www.ydjk.org.cn/Article/details/gt2zoiorvfr.html

Path("a/b.txt").parent.mkdir(parents=True, exist_ok=True)
来源：http://www.ydjk.org.cn/Article/details/gt2hdjqbhqx.html

[U25] Py：CSV 按字典读
来源：http://www.52xcode.cn/Article/details/gt2rhffwdfy.html

csv.DictReader(f)
来源：http://www.ydjk.org.cn/Article/details/gt2ldwwmqjf.html

[U26] Py：并发下载
来源：http://www.ydjk.org.cn/Article/details/gt2uxbouyjb.html

ThreadPoolExecutor(max_workers=8).map(fetch, urls)
来源：http://www.52xcode.cn/Article/details/gt2ebtsmwuy.html

[U27] Py：异步 HTTP
来源：http://www.52xcode.cn/Article/details/gt2hesivinb.html

aiohttp.ClientSession() 配合 async with
来源：http://www.ydjk.org.cn/Article/details/gt2zidjqiqs.html

[U28] Py：类型别名
来源：http://www.52xcode.cn/Article/details/gt2eurlbtjd.html

UserId = int
来源：http://www.52xcode.cn/Article/details/gt2hlzkrtgg.html

[U29] Py：属性校验
来源：http://www.52xcode.cn/Article/details/gt2unpvtzvd.html

@property 与 @x.setter 配合
来源：http://www.ydjk.org.cn/Article/details/gt2kynuorbl.html

[U30] Py：数据类
来源：http://www.52xcode.cn/Article/details/gt2devgujbi.html

@dataclass(slots=True)
来源：http://www.ydjk.org.cn/Article/details/gt2fmebxgzh.html

[U31] Py：单测
来源：http://www.52xcode.cn/Article/details/gt2cgjjscua.html

python -m pytest -q
来源：http://www.ydjk.org.cn/Article/details/gt2jljltkmv.html

[U32] Py：代码格式化
来源：http://www.52xcode.cn/Article/details/gt2jxiebrnn.html

ruff format . && ruff check --fix .
来源：http://www.ydjk.org.cn/Article/details/gt2hcrtrnyy.html

[U33] Py：打包发布
来源：http://www.ydjk.org.cn/Article/details/gt2hiyliifd.html

python -m build  （依赖 pyproject.toml）
来源：http://www.52xcode.cn/Article/details/gt2gktrvbtv.html

[U34] Py：判断编码
来源：http://www.ydjk.org.cn/Article/details/gt2ubrxdwul.html

chardet.detect(raw)
来源：http://www.52xcode.cn/Article/details/gt2wwappdrs.html

[U35] Py：发送邮件
来源：http://www.ydjk.org.cn/Article/details/gt2ebvpfsny.html

smtplib.SMTP_SSL(...).send_message(msg)
来源：http://www.ydjk.org.cn/Article/details/gt2kohoptmw.html

[U36] Py：定时任务
来源：http://www.52xcode.cn/Article/details/gt2lzehkdyf.html

schedule.every(10).minutes.do(job)
来源：http://www.ydjk.org.cn/Article/details/gt2yswzzfoe.html

[U37] Py：读写 Excel
来源：http://www.52xcode.cn/Article/details/gt2xfcurixc.html

pandas.read_excel / DataFrame.to_excel
来源：http://www.52xcode.cn/Article/details/gt2mxgvjdla.html

[U38] Py：获取脚本所在目录
来源：http://www.52xcode.cn/Article/details/gt2ubyszzyy.html

Path(__file__).resolve().parent
来源：http://www.52xcode.cn/Article/details/gt2sobgxupr.html

[U39] Py：判断是否在交互环境
来源：http://www.52xcode.cn/Article/details/gt2oyzikhng.html

sys.stdout.isatty()
来源：http://www.ydjk.org.cn/Article/details/gt2pupcsfap.html

[U40] Py：打印到标准错误
来源：http://www.52xcode.cn/Article/details/gt2uxateaui.html

print("err", file=sys.stderr)
来源：http://www.ydjk.org.cn/Article/details/gt2rlbexyma.html

[U41] PHP：初始化 Composer 项目
来源：http://www.ydjk.org.cn/Article/details/gt2nawipzkw.html

composer init;  composer require guzzlehttp/guzzle
来源：http://www.52xcode.cn/Article/details/gt2ijzbfanb.html

[U42] PHP：PSR-4 自动加载
来源：http://www.52xcode.cn/Article/details/gt2tjxioiuz.html

"autoload": { "psr-4": { "App\\": "src/" } }
来源：http://www.52xcode.cn/Article/details/gt2fyqpmpfi.html

[U43] PHP：声明命名空间
来源：http://www.52xcode.cn/Article/details/gt2abpasndk.html

namespace App\Http;
来源：http://www.52xcode.cn/Article/details/gt2omceazwe.html

[U44] PHP：开启严格类型
来源：http://www.52xcode.cn/Article/details/gt2qsddybov.html

declare(strict_types=1);
来源：http://www.ydjk.org.cn/Article/details/gt2zioetbho.html

[U45] PHP：类型声明与返回类型
来源：http://www.52xcode.cn/Article/details/gt2lqdapghy.html

function add(int $a, int $b): int { return $a + $b; }
来源：http://www.52xcode.cn/Article/details/gt2koyyjvua.html

[U46] PHP：可空类型
来源：http://www.52xcode.cn/Article/details/gt2eevyikgx.html

?string $name = null
来源：http://www.ydjk.org.cn/Article/details/gt2oqnlrikp.html

[U47] PHP：联合类型
来源：http://www.52xcode.cn/Article/details/gt2dzevydat.html

int|string $id
来源：http://www.ydjk.org.cn/Article/details/gt2svvccjvh.html

[U48] PHP：纯枚举
来源：http://www.52xcode.cn/Article/details/gt2sdunhawj.html

enum Status: string { case Active = "active"; case Off = "off"; }
来源：http://www.52xcode.cn/Article/details/gt2vbekghmg.html

[U49] PHP：只读属性
来源：http://www.52xcode.cn/Article/details/gt2ozujbbxf.html

public readonly string $name
来源：http://www.ydjk.org.cn/Article/details/gt2vuiionhh.html

[U50] PHP：构造器属性提升
来源：http://www.ydjk.org.cn/Article/details/gt2phtaqane.html

public function __construct(private int $id) {}
来源：http://www.52xcode.cn/Article/details/gt2dprtspuq.html

[U51] PHP：数组解构
来源：http://www.52xcode.cn/Article/details/gt2eiddfxwc.html

[$a, $b] = $arr;
来源：http://www.52xcode.cn/Article/details/gt2mucuxsmu.html

[U52] PHP：箭头函数
来源：http://www.ydjk.org.cn/Article/details/gt2nahwjckd.html

$double = fn($x) => $x * 2;
来源：http://www.52xcode.cn/Article/details/gt2pvmszjis.html

[U53] PHP：空合并运算符
来源：http://www.ydjk.org.cn/Article/details/gt2coxzttoh.html

$v = $a ?? $b ?? "default";
来源：http://www.ydjk.org.cn/Article/details/gt2yuvihukp.html

[U54] PHP：空安全调用
来源：http://www.52xcode.cn/Article/details/gt2ptjmgmnf.html

$obj?->method()
来源：http://www.52xcode.cn/Article/details/gt2twtdsnle.html

[U55] PHP：match 表达式
来源：http://www.ydjk.org.cn/Article/details/gt2azhcpcdl.html

$s = match($x) { 1 => "一", default => "其他" };
来源：http://www.ydjk.org.cn/Article/details/gt2zobvqcwv.html

[U56] PHP：命名参数
来源：http://www.52xcode.cn/Article/details/gt2muccvocd.html

f(a: 1, b: 2)
来源：http://www.52xcode.cn/Article/details/gt2qfhtbevu.html

[U57] PHP：字符串插值
来源：http://www.52xcode.cn/Article/details/gt2gllecsqq.html

"值: {$a}"
来源：http://www.52xcode.cn/Article/details/gt2ezuqkjlx.html

[U58] PHP：数组三件套
来源：http://www.ydjk.org.cn/Article/details/gt2dpsbmfrw.html

array_map($f, $a);  array_filter($a, $f);  array_reduce($a, $f, 0);
来源：http://www.ydjk.org.cn/Article/details/gt2dibwpugf.html

[U59] PHP：自定义排序
来源：http://www.ydjk.org.cn/Article/details/gt2hkmosamt.html

usort($arr, fn($a, $b) => $a["age"] <=> $b["age"]);
来源：http://www.ydjk.org.cn/Article/details/gt2hzzetwtg.html

[U60] PHP：JSON 编解码
来源：http://www.52xcode.cn/Article/details/gt2ieogelmy.html

json_encode($d, JSON_UNESCAPED_UNICODE);  json_decode($s, true);
来源：http://www.52xcode.cn/Article/details/gt2dieallio.html

[U61] PHP：正则
来源：http://www.ydjk.org.cn/Article/details/gt2eufsweic.html

preg_match('/(\d+)/', $s, $m);  preg_replace('/\d+/', '#', $s);
来源：http://www.ydjk.org.cn/Article/details/gt2gjxdoidc.html

[U62] PHP：日期对象
来源：http://www.ydjk.org.cn/Article/details/gt2agkjciuh.html

(new DateTimeImmutable())->format("Y-m-d");
来源：http://www.52xcode.cn/Article/details/gt2sphxmlhv.html

[U63] PHP：文件读写
来源：http://www.ydjk.org.cn/Article/details/gt2ocmvhnru.html

file_get_contents($f);  file_put_contents($f, $data);
来源：http://www.52xcode.cn/Article/details/gt2aqimiier.html

[U64] PHP：目录遍历
来源：http://www.52xcode.cn/Article/details/gt2qlpamkbj.html

glob("dir/*.php");  scandir("dir");
来源：http://www.52xcode.cn/Article/details/gt2nosrprov.html

[U65] PHP：会话
来源：http://www.ydjk.org.cn/Article/details/gt2ppipljic.html

session_start();  $_SESSION["uid"] = 1;
来源：http://www.52xcode.cn/Article/details/gt2zstgchui.html

[U66] PHP：设置 Cookie
来源：http://www.52xcode.cn/Article/details/gt2xzwhdbyy.html

setcookie("token", $v, ["httponly" => true, "samesite" => "Lax"]);
来源：http://www.52xcode.cn/Article/details/gt2djrsappw.html

[U67] PHP：处理文件上传
来源：http://www.ydjk.org.cn/Article/details/gt2nwixloag.html

$_FILES["file"]["tmp_name"] 与 move_uploaded_file()
来源：http://www.ydjk.org.cn/Article/details/gt2cgxocrvq.html

[U68] PHP：PDO 连接
来源：http://www.52xcode.cn/Article/details/gt2puptudou.html

$pdo = new PDO("mysql:host=localhost;dbname=app", "root", "");
来源：http://www.ydjk.org.cn/Article/details/gt2leqfvmub.html

[U69] PHP：PDO 预处理
来源：http://www.ydjk.org.cn/Article/details/gt2sdwmphbn.html

$stmt = $pdo->prepare("SELECT * FROM users WHERE id = ?");  $stmt->execute([$id]);
来源：http://www.52xcode.cn/Article/details/gt2nhchvnnt.html

[U70] PHP：PDO 事务
来源：http://www.52xcode.cn/Article/details/gt2bnxggsmp.html

$pdo->beginTransaction();  $pdo->commit();  $pdo->rollBack();
来源：http://www.52xcode.cn/Article/details/gt2nrppxuyv.html

[U71] PHP：抛出异常
来源：http://www.ydjk.org.cn/Article/details/gt2xdfuwqit.html

throw new RuntimeException("失败", 500);
来源：http://www.ydjk.org.cn/Article/details/gt2gfsgnpcb.html

[U72] PHP：写错误日志
来源：http://www.ydjk.org.cn/Article/details/gt2eahyzvog.html

error_log("失败: " . $e->getMessage());
来源：http://www.52xcode.cn/Article/details/gt2uxjrtyal.html

[U73] PHP：读取 ini 配置
来源：http://www.ydjk.org.cn/Article/details/gt2inokzbjk.html

parse_ini_file("config.ini", true)
来源：http://www.ydjk.org.cn/Article/details/gt2sxprdpwe.html

[U74] PHP：读取环境变量
来源：http://www.ydjk.org.cn/Article/details/gt2mqrjobdp.html

getenv("APP_ENV") ?: "production"
来源：http://www.52xcode.cn/Article/details/gt2hpcljmxu.html

[U75] PHP：依赖注入
来源：http://www.52xcode.cn/Article/details/gt2nfsgovkn.html

composer require psr/container
来源：http://www.ydjk.org.cn/Article/details/gt2offkgbxm.html

[U76] PHP：简单路由
来源：http://www.ydjk.org.cn/Article/details/gt2mhyfvshs.html

$path = parse_url($_SERVER["REQUEST_URI"], PHP_URL_PATH);
来源：http://www.ydjk.org.cn/Article/details/gt2syvuoyyi.html

[U77] PHP：模板渲染
来源：http://www.ydjk.org.cn/Article/details/gt2zkcmpkeg.html

composer require twig/twig
来源：http://www.ydjk.org.cn/Article/details/gt2ggjcbxzt.html

[U78] PHP：单元测试
来源：http://www.52xcode.cn/Article/details/gt2whuztkun.html

composer require --dev phpunit/phpunit
来源：http://www.52xcode.cn/Article/details/gt2bvylgbbq.html

[U79] PHP：静态分析
来源：http://www.ydjk.org.cn/Article/details/gt2mumrbquo.html

composer require --dev phpstan/phpstan
来源：http://www.52xcode.cn/Article/details/gt2vhfovkeh.html

[U80] PHP：代码规范修复
来源：http://www.52xcode.cn/Article/details/gt2slzbtqtp.html

composer require --dev friendsofphp/php-cs-fixer
来源：http://www.52xcode.cn/Article/details/gt2agrdqgzl.html

[U81] JS：初始化项目
来源：http://www.ydjk.org.cn/Article/details/gt2qryktace.html

npm init -y;  npm i express
来源：http://www.ydjk.org.cn/Article/details/gt2bzzbfmav.html

[U82] JS：package.json 脚本
来源：http://www.52xcode.cn/Article/details/gt2xuxvsapj.html

"scripts": { "dev": "vite", "build": "vite build" }
来源：http://www.ydjk.org.cn/Article/details/gt2yxvknald.html

[U83] JS：ES Module 导入导出
来源：http://www.ydjk.org.cn/Article/details/gt2cksdiaqm.html

export const a = 1;  import { a } from "./m.js";
来源：http://www.52xcode.cn/Article/details/gt2hnvlhyjv.html

[U84] JS：CommonJS 写法
来源：http://www.ydjk.org.cn/Article/details/gt2ldtnxggv.html

module.exports = { a };  const { a } = require("./m");
来源：http://www.52xcode.cn/Article/details/gt2petnwvst.html

[U85] JS：可选链
来源：http://www.52xcode.cn/Article/details/gt2zepsinmx.html

a?.b?.c
来源：http://www.52xcode.cn/Article/details/gt2pnippayq.html

[U86] JS：空值合并
来源：http://www.52xcode.cn/Article/details/gt2uodxrtqd.html

a ?? b
来源：http://www.ydjk.org.cn/Article/details/gt2kpnbwvie.html

[U87] JS：解构默认值
来源：http://www.52xcode.cn/Article/details/gt2mqrnzyzs.html

const { a = 1, b = 2 } = obj;
来源：http://www.ydjk.org.cn/Article/details/gt2glbscbja.html

[U88] JS：对象展开合并
来源：http://www.ydjk.org.cn/Article/details/gt2ekrhpbwo.html

{ ...a, ...b }
来源：http://www.52xcode.cn/Article/details/gt2omijrudo.html

[U89] JS：数组去重
来源：http://www.52xcode.cn/Article/details/gt2yaqafoso.html

[...new Set(arr)]
来源：http://www.ydjk.org.cn/Article/details/gt2aqmbxzfu.html

[U90] JS：数字数组排序
来源：http://www.ydjk.org.cn/Article/details/gt2huykvsob.html

[...arr].sort((a, b) => a - b)
来源：http://www.52xcode.cn/Article/details/gt2mkcbqolk.html

[U91] JS：对象键值遍历
来源：http://www.52xcode.cn/Article/details/gt2tsptuqli.html

Object.entries(obj).forEach(([k, v]) => {});
来源：http://www.52xcode.cn/Article/details/gt2pecnqjah.html

[U92] JS：深拷贝
来源：http://www.ydjk.org.cn/Article/details/gt2ywbtaeff.html

structuredClone(obj)
来源：http://www.52xcode.cn/Article/details/gt2wknthntw.html

[U93] JS：模板字符串
来源：http://www.52xcode.cn/Article/details/gt2pjnwmnbx.html

`共 ${n} 条`
来源：http://www.ydjk.org.cn/Article/details/gt2crxhcgks.html

[U94] JS：箭头函数
来源：http://www.ydjk.org.cn/Article/details/gt2zsmgdbej.html

const double = x => x * 2;
来源：http://www.52xcode.cn/Article/details/gt2axflyoyt.html

[U95] JS：Promise 包装
来源：http://www.52xcode.cn/Article/details/gt2jmkbjhqo.html

new Promise((resolve, reject) => {})
来源：http://www.ydjk.org.cn/Article/details/gt2lmkzoumg.html

[U96] JS：async/await 与异常
来源：http://www.ydjk.org.cn/Article/details/gt2tomrtbfa.html

try { const d = await f(); } catch (e) { console.error(e); }
来源：http://www.52xcode.cn/Article/details/gt2ntmqsmdn.html

[U97] JS：并发请求
来源：http://www.52xcode.cn/Article/details/gt2ixokpfgi.html

await Promise.all(urls.map(u => fetch(u)))
来源：http://www.52xcode.cn/Article/details/gt2ljnnqbzq.html

[U98] JS：fetch 带 JSON
来源：http://www.ydjk.org.cn/Article/details/gt2hxmuevkd.html

await fetch(url, { method: "POST", headers: { "Content-Type": "application/json" }, body: JSON.stringify(d) })
来源：http://www.52xcode.cn/Article/details/gt2fxrdwuyf.html

[U99] JS：事件监听
来源：http://www.ydjk.org.cn/Article/details/gt2haljzbhl.html

el.addEventListener("click", e => {})
来源：http://www.ydjk.org.cn/Article/details/gt2bypmjjed.html

[U100] JS：DOM 查询
来源：http://www.52xcode.cn/Article/details/gt2mnrcfprg.html

document.querySelector(".item")
来源：http://www.52xcode.cn/Article/details/gt2rlxgnvmv.html

[U101] JS：classList 操作
来源：http://www.ydjk.org.cn/Article/details/gt2sacybtom.html

el.classList.toggle("active")
来源：http://www.52xcode.cn/Article/details/gt2mspiwymd.html

[U102] JS：本地存储
来源：http://www.ydjk.org.cn/Article/details/gt2wekptsjx.html

localStorage.setItem("k", JSON.stringify(v))
来源：http://www.ydjk.org.cn/Article/details/gt2cmeeybxj.html

[U103] JS：定时器
来源：http://www.52xcode.cn/Article/details/gt2qmzmtzht.html

setTimeout(fn, 1000);  setInterval(fn, 1000);
来源：http://www.52xcode.cn/Article/details/gt2xwyrkjqe.html

[U104] JS：防抖
来源：http://www.ydjk.org.cn/Article/details/gt2kseuaqhi.html

const debounce = (fn, ms) => { let t; return (...a) => { clearTimeout(t); t = setTimeout(() => fn(...a), ms); }; };
来源：http://www.ydjk.org.cn/Article/details/gt2gvdtqkwz.html

[U105] JS：节流
来源：http://www.52xcode.cn/Article/details/gt2rmzdfnfn.html

const throttle = (fn, ms) => { let last = 0; return (...a) => { const n = Date.now(); if (n - last >= ms) { last = n; fn(...a); } }; };
来源：http://www.52xcode.cn/Article/details/gt2ewaqzvta.html

[U106] JS：日期格式化
来源：http://www.52xcode.cn/Article/details/gt2ackvnvcx.html

new Intl.DateTimeFormat("zh-CN", { dateStyle: "medium" }).format(new Date())
来源：http://www.52xcode.cn/Article/details/gt2hoprdgup.html

[U107] JS：数字千分位
来源：http://www.52xcode.cn/Article/details/gt2uhwpwjcp.html

new Intl.NumberFormat("en-US").format(1234567)
来源：http://www.ydjk.org.cn/Article/details/gt2pawvhbvl.html

[U108] JS：随机整数
来源：http://www.52xcode.cn/Article/details/gt2wpsdbzwa.html

Math.floor(Math.random() * (max - min + 1)) + min
来源：http://www.52xcode.cn/Article/details/gt2zbywusyi.html

[U109] JS：数组分组
来源：http://www.52xcode.cn/Article/details/gt2acihvyab.html

Object.groupBy(arr, x => x.type)
来源：http://www.ydjk.org.cn/Article/details/gt2sylmnsgd.html

[U110] JS：数组分块
来源：http://www.52xcode.cn/Article/details/gt2yiplejkv.html

arr.reduce((acc, x, i) => (i % size ? acc : [...acc, arr.slice(i, i + size)]), [])
来源：http://www.52xcode.cn/Article/details/gt2vmwjlubl.html


<!-- 参考信息 -->