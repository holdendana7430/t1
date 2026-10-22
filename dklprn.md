代发 wailian999

[T21] Swift：遍历
来源：http://www.ydjk.org.cn/Article/details/gt2gqanqhhd.html

for x in a { print(x) }
来源：http://www.ydjk.org.cn/Article/details/gt2isikjvrz.html

[T22] Swift：字典
来源：http://www.ydjk.org.cn/Article/details/gt2cfhgqovs.html

var d = ["a": 1];  d["b"] = 2
来源：http://www.ydjk.org.cn/Article/details/gt2cisnhwow.html

[T23] Swift：函数
来源：http://www.52xcode.cn/Article/details/gt2mebbdvkg.html

func add(_ a: Int, _ b: Int) -> Int { a + b }
来源：http://www.ydjk.org.cn/Article/details/gt2xkkmcgsh.html

[T24] Swift：闭包
来源：http://www.52xcode.cn/Article/details/gt2yhpxfphg.html

let f = { (x: Int) -> Int in x * 2 }
来源：http://www.52xcode.cn/Article/details/gt2fvoasvbz.html

[T25] Swift：结构体
来源：http://www.ydjk.org.cn/Article/details/gt2yzjlfgdc.html

struct P { var x: Int }
来源：http://www.ydjk.org.cn/Article/details/gt2dlpnihce.html

[T26] Swift：类与重写
来源：http://www.ydjk.org.cn/Article/details/gt2iaiqlxqy.html

class A: Base { override func f() {} }
来源：http://www.ydjk.org.cn/Article/details/gt2oumbmkpt.html

[T27] Swift：错误处理
来源：http://www.ydjk.org.cn/Article/details/gt2hpojjqhj.html

do { try f() } catch { print(error) }
来源：http://www.52xcode.cn/Article/details/gt2jsvpcfuq.html

[T28] Swift：枚举
来源：http://www.ydjk.org.cn/Article/details/gt2bjsnuirj.html

enum Color { case red, green }
来源：http://www.52xcode.cn/Article/details/gt2elhkxpxk.html

[T29] Swift：guard 提前返回
来源：http://www.52xcode.cn/Article/details/gt2tefdauak.html

guard let x = opt else { return }
来源：http://www.ydjk.org.cn/Article/details/gt2trekdzcq.html

[T30] Swift：协议
来源：http://www.52xcode.cn/Article/details/gt2mnelfyni.html

protocol Shape { func area() -> Double }
来源：http://www.52xcode.cn/Article/details/gt2xpogwjrp.html

[T31] Lua：Hello World
来源：http://www.52xcode.cn/Article/details/gt2ntpswque.html

print("Hello")
来源：http://www.52xcode.cn/Article/details/gt2xbjhjokf.html

[T32] Lua：局部变量
来源：http://www.52xcode.cn/Article/details/gt2cnfohsal.html

local a = 1
来源：http://www.ydjk.org.cn/Article/details/gt2sxxpmsky.html

[T33] Lua：表（数组）
来源：http://www.ydjk.org.cn/Article/details/gt2psgnhskk.html

local t = {1, 2, 3};  t[4] = 4
来源：http://www.52xcode.cn/Article/details/gt2gpazhrwv.html

[T34] Lua：遍历表
来源：http://www.ydjk.org.cn/Article/details/gt2mrwjcdhq.html

for i, v in ipairs(t) do print(i, v) end
来源：http://www.ydjk.org.cn/Article/details/gt2hwfrepwj.html

[T35] Lua：字典表
来源：http://www.52xcode.cn/Article/details/gt2axeufmon.html

local d = { a = 1 };  d.b = 2
来源：http://www.52xcode.cn/Article/details/gt2zcuafhty.html

[T36] Lua：函数
来源：http://www.52xcode.cn/Article/details/gt2ywmeizfk.html

function add(a, b) return a + b end
来源：http://www.52xcode.cn/Article/details/gt2wxwreczw.html

[T37] Lua：字符串拼接
来源：http://www.ydjk.org.cn/Article/details/gt2fktivhzl.html

"a" .. "b"
来源：http://www.52xcode.cn/Article/details/gt2uchmnpfe.html

[T38] Lua：条件
来源：http://www.ydjk.org.cn/Article/details/gt2vkbcswlt.html

if x > 0 then print("正") end
来源：http://www.52xcode.cn/Article/details/gt2fiqbygmb.html

[T39] Lua：模式匹配
来源：http://www.ydjk.org.cn/Article/details/gt2ypiplnwl.html

string.find(s, "%d+")
来源：http://www.52xcode.cn/Article/details/gt2dxarsagw.html

[T40] Lua：元表
来源：http://www.ydjk.org.cn/Article/details/gt2lnfzsbld.html

setmetatable({}, { __index = base })
来源：http://www.ydjk.org.cn/Article/details/gt2eejplxqj.html

[T41] Perl：Hello World
来源：http://www.ydjk.org.cn/Article/details/gt2mbjfplwy.html

print "Hello\n";
来源：http://www.ydjk.org.cn/Article/details/gt2lqzngamu.html

[T42] Perl：变量类型
来源：http://www.ydjk.org.cn/Article/details/gt2tjmolrpd.html

my $a = 1;  my @arr = (1, 2, 3);  my %h = (a => 1);
来源：http://www.ydjk.org.cn/Article/details/gt2osfuabzd.html

[T43] Perl：字符串插值
来源：http://www.ydjk.org.cn/Article/details/gt2grdcamed.html

"值: $a"
来源：http://www.ydjk.org.cn/Article/details/gt2dmcmuodt.html

[T44] Perl：条件
来源：http://www.52xcode.cn/Article/details/gt2jgloahtv.html

if ($a > 0) { print "正"; }
来源：http://www.ydjk.org.cn/Article/details/gt2tmglrpeb.html

[T45] Perl：数组遍历
来源：http://www.52xcode.cn/Article/details/gt2mqcxpuec.html

for my $x (@arr) { print $x; }
来源：http://www.52xcode.cn/Article/details/gt2gmigefwz.html

[T46] Perl：哈希操作
来源：http://www.ydjk.org.cn/Article/details/gt2qrjshqde.html

$h{b} = 2;  for my $k (keys %h) { print "$k=$h{$k}"; }
来源：http://www.ydjk.org.cn/Article/details/gt2wquwlaxo.html

[T47] Perl：正则捕获
来源：http://www.ydjk.org.cn/Article/details/gt2vdyeeagc.html

if ($s =~ /(\d+)/) { print $1; }
来源：http://www.ydjk.org.cn/Article/details/gt2nzdynbme.html

[T48] Perl：正则替换
来源：http://www.52xcode.cn/Article/details/gt2nmvnotcq.html

$s =~ s/old/new/g;
来源：http://www.ydjk.org.cn/Article/details/gt2ogmqqrjf.html

[T49] Perl：函数
来源：http://www.ydjk.org.cn/Article/details/gt2ndxmvxfg.html

sub add { my ($a, $b) = @_; return $a + $b; }
来源：http://www.ydjk.org.cn/Article/details/gt2fijcijsi.html

[T50] Perl：逐行读文件
来源：http://www.52xcode.cn/Article/details/gt2mumqvryd.html

open my $fh, "<", "a.txt" or die $!;
来源：http://www.ydjk.org.cn/Article/details/gt2cmtxibld.html

while (my $line = <$fh>) { print $line; }
来源：http://www.ydjk.org.cn/Article/details/gt2mfrpvlhi.html

[T51] Scala：Hello World
来源：http://www.52xcode.cn/Article/details/gt2saqskxbn.html

println("Hello")
来源：http://www.52xcode.cn/Article/details/gt2wjyunrag.html

[T52] Scala：变量
来源：http://www.ydjk.org.cn/Article/details/gt2obrxfofe.html

val a = 1;  var b = 2
来源：http://www.ydjk.org.cn/Article/details/gt2gasxtxgm.html

[T53] Scala：字符串插值
来源：http://www.ydjk.org.cn/Article/details/gt2okormdau.html

s"值: $b"
来源：http://www.ydjk.org.cn/Article/details/gt2ncuxxlif.html

[T54] Scala：集合映射
来源：http://www.52xcode.cn/Article/details/gt2bedtyhck.html

List(1, 2, 3).map(_ * 2)
来源：http://www.52xcode.cn/Article/details/gt2uwpjjxpo.html

[T55] Scala：集合过滤
来源：http://www.52xcode.cn/Article/details/gt2bpxhisqa.html

List(1, 2, 3).filter(_ > 1)
来源：http://www.ydjk.org.cn/Article/details/gt2dswxuguu.html

[T56] Scala：样例类
来源：http://www.ydjk.org.cn/Article/details/gt2wikvgdya.html

case class User(name: String, age: Int)
来源：http://www.52xcode.cn/Article/details/gt2grbzxlhn.html

[T57] Scala：模式匹配
来源：http://www.52xcode.cn/Article/details/gt2ubrgzlgk.html

x match { case 1 => "一"; case _ => "其他" }
来源：http://www.ydjk.org.cn/Article/details/gt2lynfuyfs.html

[T58] Scala：函数定义
来源：http://www.52xcode.cn/Article/details/gt2yhdbzynb.html

def add(a: Int, b: Int): Int = a + b
来源：http://www.52xcode.cn/Article/details/gt2koaawmjn.html

[T59] Scala：循环
来源：http://www.52xcode.cn/Article/details/gt2tzuvyrif.html

for (i <- 1 to 10) println(i)
来源：http://www.52xcode.cn/Article/details/gt2rcgyqulh.html

[T60] Scala：折叠
来源：http://www.52xcode.cn/Article/details/gt2mrgmuqit.html

List(1, 2, 3).foldLeft(0)(_ + _)
来源：http://www.ydjk.org.cn/Article/details/gt2lcikfwjq.html

================================================================================
来源：http://www.ydjk.org.cn/Article/details/gt2oftwpttf.html

U. 高频实用片段（Python / PHP / JavaScript 各 40 条）
来源：http://www.ydjk.org.cn/Article/details/gt2dmkmfgaj.html

================================================================================
来源：http://www.ydjk.org.cn/Article/details/gt2dcbmcvqz.html

[U01] Py：创建虚拟环境
来源：http://www.ydjk.org.cn/Article/details/gt2rjenahpz.html

python -m venv .venv && source .venv/bin/activate
来源：http://www.52xcode.cn/Article/details/gt2qriznzje.html

[U02] Py：导出 / 安装依赖
来源：http://www.52xcode.cn/Article/details/gt2mmhjbmwz.html

pip freeze > requirements.txt;  pip install -r requirements.txt
来源：http://www.52xcode.cn/Article/details/gt2zzirjkrw.html

[U03] Py：加载 .env 配置
来源：http://www.52xcode.cn/Article/details/gt2opdafyta.html

from dotenv import load_dotenv; load_dotenv()
来源：http://www.52xcode.cn/Article/details/gt2kdusfeso.html

[U04] Py：变量调试打印
来源：http://www.ydjk.org.cn/Article/details/gt2xybtdtfn.html

print(f"{x=}")            # 输出 x=值，Python 3.8+
来源：http://www.ydjk.org.cn/Article/details/gt2tqbitlmq.html

[U05] Py：列表去重且保序
来源：http://www.52xcode.cn/Article/details/gt2wuhnbika.html

list(dict.fromkeys(arr))
来源：http://www.ydjk.org.cn/Article/details/gt2xmdwcnnv.html

[U06] Py：合并两个字典
来源：http://www.ydjk.org.cn/Article/details/gt2atpomavd.html

{**a, **b}
来源：http://www.52xcode.cn/Article/details/gt2gdwxhadn.html

[U07] Py：反转字典键值
来源：http://www.52xcode.cn/Article/details/gt2nyodlzzt.html

{v: k for k, v in d.items()}
来源：http://www.52xcode.cn/Article/details/gt2ialiuonx.html

[U08] Py：展平二维列表
来源：http://www.52xcode.cn/Article/details/gt2dmalahyd.html

[y for x in nested for y in x]
来源：http://www.ydjk.org.cn/Article/details/gt2fomoywot.html

[U09] Py：字典取最大值的键
来源：http://www.52xcode.cn/Article/details/gt2hjucwfmk.html

max(d, key=d.get)
来源：http://www.52xcode.cn/Article/details/gt2bkfkzcqo.html

[U10] Py：按值排序字典
来源：http://www.52xcode.cn/Article/details/gt2fqplctev.html

dict(sorted(d.items(), key=lambda kv: kv[1]))
来源：http://www.52xcode.cn/Article/details/gt2qlugxkvn.html

[U11] Py：生成器表达式
来源：http://www.52xcode.cn/Article/details/gt2pznhfviw.html

(x * 2 for x in arr)
来源：http://www.52xcode.cn/Article/details/gt2prghpaab.html

[U12] Py：取出现最多的 3 个元素
来源：http://www.52xcode.cn/Article/details/gt2hgicjryj.html

Counter(arr).most_common(3)
来源：http://www.ydjk.org.cn/Article/details/gt2qbuycjpt.html

[U13] Py：固定长度队列
来源：http://www.ydjk.org.cn/Article/details/gt2wfijavsw.html

deque(maxlen=10)
来源：http://www.ydjk.org.cn/Article/details/gt2lsefmixt.html

[U14] Py：分组收集到列表
来源：http://www.ydjk.org.cn/Article/details/gt2egepyaim.html

defaultdict(list)
来源：http://www.52xcode.cn/Article/details/gt2ugchrwsv.html

[U15] Py：高精度计时
来源：http://www.ydjk.org.cn/Article/details/gt2dmcymsmm.html

t = time.perf_counter()
来源：http://www.ydjk.org.cn/Article/details/gt2ianycrxa.html

[U16] Py：命令行参数解析
来源：http://www.52xcode.cn/Article/details/gt2fobpomij.html

ap = argparse.ArgumentParser();  ap.add_argument("--name");  args = ap.parse_args()
来源：http://www.52xcode.cn/Article/details/gt2wzlnfxgv.html

[U17] Py：初始化日志
来源：http://www.ydjk.org.cn/Article/details/gt2bedbkdrc.html

logging.basicConfig(level=logging.INFO)
来源：http://www.ydjk.org.cn/Article/details/gt2uyizhaho.html

[U18] Py：预编译正则
来源：http://www.52xcode.cn/Article/details/gt2dgqvzeve.html

pat = re.compile(r"\d+")
来源：http://www.ydjk.org.cn/Article/details/gt2dufisllh.html

[U19] Py：正则替换带回调
来源：http://www.ydjk.org.cn/Article/details/gt2uvpkadmh.html

re.sub(r"\d+", lambda m: str(int(m.group()) * 2), s)
来源：http://www.ydjk.org.cn/Article/details/gt2kvnuabtw.html

[U20] Py：缓存函数结果
来源：http://www.52xcode.cn/Article/details/gt2ozqzlnon.html

@functools.lru_cache(maxsize=None)
来源：http://www.52xcode.cn/Article/details/gt2thluriru.html

[U21] Py：自定义上下文管理器
来源：http://www.ydjk.org.cn/Article/details/gt2rtobmoii.html

@contextlib.contextmanager
来源：http://www.ydjk.org.cn/Article/details/gt2xbcmptsn.html

[U22] Py：矩阵转置
来源：http://www.52xcode.cn/Article/details/gt2fokabhnn.html

list(zip(*m))
来源：http://www.52xcode.cn/Article/details/gt2jhgkwses.html

[U23] Py：分块读取大文件
来源：http://www.ydjk.org.cn/Article/details/gt2axrhmylz.html

for chunk in iter(lambda: f.read(8192), b""):
来源：http://www.ydjk.org.cn/Article/details/gt2jmirciqt.html

[U24] Py：路径操作
来源：http://www.ydjk.org.cn/Article/details/gt2elgxnejh.html

Path("a/b.txt").parent.mkdir(parents=True, exist_ok=True)
来源：http://www.ydjk.org.cn/Article/details/gt2mzhnotsl.html

[U25] Py：CSV 按字典读
来源：http://www.52xcode.cn/Article/details/gt2efhmaikz.html

csv.DictReader(f)
来源：http://www.ydjk.org.cn/Article/details/gt2uxewafxk.html

[U26] Py：并发下载
来源：http://www.52xcode.cn/Article/details/gt2gynumeps.html

ThreadPoolExecutor(max_workers=8).map(fetch, urls)
来源：http://www.ydjk.org.cn/Article/details/gt2xcvnjkle.html

[U27] Py：异步 HTTP
来源：http://www.ydjk.org.cn/Article/details/gt2svgzekkt.html

aiohttp.ClientSession() 配合 async with
来源：http://www.52xcode.cn/Article/details/gt2yyxifjft.html

[U28] Py：类型别名
来源：http://www.ydjk.org.cn/Article/details/gt2iwnykzps.html

UserId = int
来源：http://www.ydjk.org.cn/Article/details/gt2rqkscpjq.html

[U29] Py：属性校验
来源：http://www.52xcode.cn/Article/details/gt2lofkhlbz.html

@property 与 @x.setter 配合
来源：http://www.52xcode.cn/Article/details/gt2fkldhfhn.html

[U30] Py：数据类
来源：http://www.52xcode.cn/Article/details/gt2wdujtyja.html

@dataclass(slots=True)
来源：http://www.52xcode.cn/Article/details/gt2mwfkemuu.html

[U31] Py：单测
来源：http://www.52xcode.cn/Article/details/gt2yevbxbhl.html

python -m pytest -q
来源：http://www.52xcode.cn/Article/details/gt2kwyxffts.html

[U32] Py：代码格式化
来源：http://www.52xcode.cn/Article/details/gt2gbjtkbeo.html

ruff format . && ruff check --fix .
来源：http://www.52xcode.cn/Article/details/gt2hipllrkm.html

[U33] Py：打包发布
来源：http://www.ydjk.org.cn/Article/details/gt2bdnolfye.html

python -m build  （依赖 pyproject.toml）
来源：http://www.ydjk.org.cn/Article/details/gt2lpozodbf.html

[U34] Py：判断编码
来源：http://www.52xcode.cn/Article/details/gt2qfbqvyfo.html

chardet.detect(raw)
来源：http://www.ydjk.org.cn/Article/details/gt2dsggiyhs.html

[U35] Py：发送邮件
来源：http://www.52xcode.cn/Article/details/gt2dvtwkggw.html

smtplib.SMTP_SSL(...).send_message(msg)
来源：http://www.52xcode.cn/Article/details/gt2gnlckwkv.html

[U36] Py：定时任务
来源：http://www.52xcode.cn/Article/details/gt2fgzmyumh.html

schedule.every(10).minutes.do(job)
来源：http://www.ydjk.org.cn/Article/details/gt2izfftkks.html

[U37] Py：读写 Excel
来源：http://www.52xcode.cn/Article/details/gt2zzzcndrd.html

pandas.read_excel / DataFrame.to_excel
来源：http://www.52xcode.cn/Article/details/gt2wuumolhf.html

[U38] Py：获取脚本所在目录
来源：http://www.ydjk.org.cn/Article/details/gt2krqcyxmb.html

Path(__file__).resolve().parent
来源：http://www.52xcode.cn/Article/details/gt2tbbbowjn.html

[U39] Py：判断是否在交互环境
来源：http://www.52xcode.cn/Article/details/gt2opekasuo.html

sys.stdout.isatty()
来源：http://www.ydjk.org.cn/Article/details/gt2xnuuvyve.html

[U40] Py：打印到标准错误
来源：http://www.52xcode.cn/Article/details/gt2qvncfpmv.html

print("err", file=sys.stderr)
来源：http://www.52xcode.cn/Article/details/gt2wxddooof.html

[U41] PHP：初始化 Composer 项目
来源：http://www.52xcode.cn/Article/details/gt2eckxhwgm.html

composer init;  composer require guzzlehttp/guzzle
来源：http://www.52xcode.cn/Article/details/gt2hwivpvff.html

[U42] PHP：PSR-4 自动加载
来源：http://www.ydjk.org.cn/Article/details/gt2toqodyia.html

"autoload": { "psr-4": { "App\\": "src/" } }
来源：http://www.ydjk.org.cn/Article/details/gt2sioknggi.html

[U43] PHP：声明命名空间
来源：http://www.52xcode.cn/Article/details/gt2ilohqbav.html

namespace App\Http;
来源：http://www.52xcode.cn/Article/details/gt2dupiccnq.html

[U44] PHP：开启严格类型
来源：http://www.52xcode.cn/Article/details/gt2zchrckyf.html

declare(strict_types=1);
来源：http://www.ydjk.org.cn/Article/details/gt2dlxqachz.html

[U45] PHP：类型声明与返回类型
来源：http://www.ydjk.org.cn/Article/details/gt2pmnffhrd.html

function add(int $a, int $b): int { return $a + $b; }
来源：http://www.52xcode.cn/Article/details/gt2blawkuey.html

[U46] PHP：可空类型
来源：http://www.52xcode.cn/Article/details/gt2vflozvoj.html

?string $name = null
来源：http://www.52xcode.cn/Article/details/gt2onggtpqb.html

[U47] PHP：联合类型
来源：http://www.52xcode.cn/Article/details/gt2lfoqrsif.html

int|string $id
来源：http://www.ydjk.org.cn/Article/details/gt2vhcknfve.html

[U48] PHP：纯枚举
来源：http://www.52xcode.cn/Article/details/gt2zvxqswim.html

enum Status: string { case Active = "active"; case Off = "off"; }
来源：http://www.ydjk.org.cn/Article/details/gt2fzsfqvai.html

[U49] PHP：只读属性
来源：http://www.52xcode.cn/Article/details/gt2jafismox.html

public readonly string $name
来源：http://www.52xcode.cn/Article/details/gt2edmzgkxp.html

[U50] PHP：构造器属性提升
来源：http://www.52xcode.cn/Article/details/gt2uxktgfte.html

public function __construct(private int $id) {}
来源：http://www.ydjk.org.cn/Article/details/gt2wvlcvnan.html

[U51] PHP：数组解构
来源：http://www.52xcode.cn/Article/details/gt2brnvmypy.html

[$a, $b] = $arr;
来源：http://www.52xcode.cn/Article/details/gt2cwjptqlw.html

[U52] PHP：箭头函数
来源：http://www.52xcode.cn/Article/details/gt2tuyvcewm.html

$double = fn($x) => $x * 2;
来源：http://www.52xcode.cn/Article/details/gt2ijfbumtw.html

[U53] PHP：空合并运算符
来源：http://www.ydjk.org.cn/Article/details/gt2llummdka.html

$v = $a ?? $b ?? "default";
来源：http://www.ydjk.org.cn/Article/details/gt2smcykiiw.html

[U54] PHP：空安全调用
来源：http://www.52xcode.cn/Article/details/gt2mkdsubcv.html

$obj?->method()
来源：http://www.ydjk.org.cn/Article/details/gt2xofumxvs.html

[U55] PHP：match 表达式
来源：http://www.52xcode.cn/Article/details/gt2kxifvnst.html

$s = match($x) { 1 => "一", default => "其他" };
来源：http://www.52xcode.cn/Article/details/gt2njhjcgah.html

[U56] PHP：命名参数
来源：http://www.ydjk.org.cn/Article/details/gt2advhdwsd.html

f(a: 1, b: 2)
来源：http://www.ydjk.org.cn/Article/details/gt2llqvntel.html

[U57] PHP：字符串插值
来源：http://www.ydjk.org.cn/Article/details/gt2gkfhcuno.html

"值: {$a}"
来源：http://www.ydjk.org.cn/Article/details/gt2urjxargy.html

[U58] PHP：数组三件套
来源：http://www.52xcode.cn/Article/details/gt2ndkfpcmg.html

array_map($f, $a);  array_filter($a, $f);  array_reduce($a, $f, 0);
来源：http://www.ydjk.org.cn/Article/details/gt2fxlwrctb.html

[U59] PHP：自定义排序
来源：http://www.52xcode.cn/Article/details/gt2wquotznn.html

usort($arr, fn($a, $b) => $a["age"] <=> $b["age"]);
来源：http://www.ydjk.org.cn/Article/details/gt2iskwcuqy.html

[U60] PHP：JSON 编解码
来源：http://www.52xcode.cn/Article/details/gt2ztlqynzn.html

json_encode($d, JSON_UNESCAPED_UNICODE);  json_decode($s, true);
来源：http://www.ydjk.org.cn/Article/details/gt2kmlnrhko.html

[U61] PHP：正则
来源：http://www.52xcode.cn/Article/details/gt2ckrrrqiw.html

preg_match('/(\d+)/', $s, $m);  preg_replace('/\d+/', '#', $s);
来源：http://www.52xcode.cn/Article/details/gt2noczavby.html

[U62] PHP：日期对象
来源：http://www.ydjk.org.cn/Article/details/gt2ascnissk.html

(new DateTimeImmutable())->format("Y-m-d");
来源：http://www.ydjk.org.cn/Article/details/gt2oappyxly.html

[U63] PHP：文件读写
来源：http://www.ydjk.org.cn/Article/details/gt2exnrtsuy.html

file_get_contents($f);  file_put_contents($f, $data);
来源：http://www.ydjk.org.cn/Article/details/gt2jplmqvyd.html

[U64] PHP：目录遍历
来源：http://www.ydjk.org.cn/Article/details/gt2ywvndity.html

glob("dir/*.php");  scandir("dir");
来源：http://www.ydjk.org.cn/Article/details/gt2wtmarkvj.html

[U65] PHP：会话
来源：http://www.ydjk.org.cn/Article/details/gt2exovclng.html

session_start();  $_SESSION["uid"] = 1;
来源：http://www.52xcode.cn/Article/details/gt2nvmynqwv.html

[U66] PHP：设置 Cookie
来源：http://www.ydjk.org.cn/Article/details/gt2zsgbvyvh.html

setcookie("token", $v, ["httponly" => true, "samesite" => "Lax"]);
来源：http://www.52xcode.cn/Article/details/gt2obprcepk.html

[U67] PHP：处理文件上传
来源：http://www.52xcode.cn/Article/details/gt2rrwxkwfc.html

$_FILES["file"]["tmp_name"] 与 move_uploaded_file()
来源：http://www.ydjk.org.cn/Article/details/gt2evmdufsw.html

[U68] PHP：PDO 连接
来源：http://www.ydjk.org.cn/Article/details/gt2aaaaaltq.html

$pdo = new PDO("mysql:host=localhost;dbname=app", "root", "");
来源：http://www.52xcode.cn/Article/details/gt2lcoyadaf.html

[U69] PHP：PDO 预处理
来源：http://www.52xcode.cn/Article/details/gt2kzxnosza.html

$stmt = $pdo->prepare("SELECT * FROM users WHERE id = ?");  $stmt->execute([$id]);
来源：http://www.52xcode.cn/Article/details/gt2rsbsfiuf.html

[U70] PHP：PDO 事务
来源：http://www.ydjk.org.cn/Article/details/gt2lzqpaauz.html

$pdo->beginTransaction();  $pdo->commit();  $pdo->rollBack();
来源：http://www.ydjk.org.cn/Article/details/gt2xdbmebgm.html

[U71] PHP：抛出异常
来源：http://www.ydjk.org.cn/Article/details/gt2hapuxutj.html

throw new RuntimeException("失败", 500);
来源：http://www.52xcode.cn/Article/details/gt2xiljpxon.html

[U72] PHP：写错误日志
来源：http://www.52xcode.cn/Article/details/gt2wxaakkdg.html

error_log("失败: " . $e->getMessage());
来源：http://www.ydjk.org.cn/Article/details/gt2mdupazzp.html

[U73] PHP：读取 ini 配置
来源：http://www.ydjk.org.cn/Article/details/gt2lcgtpwxb.html

parse_ini_file("config.ini", true)
来源：http://www.52xcode.cn/Article/details/gt2dwajuqhg.html

[U74] PHP：读取环境变量
来源：http://www.ydjk.org.cn/Article/details/gt2zqvoqlxu.html

getenv("APP_ENV") ?: "production"
来源：http://www.52xcode.cn/Article/details/gt2qftzgitb.html

[U75] PHP：依赖注入
来源：http://www.52xcode.cn/Article/details/gt2ptslendh.html

composer require psr/container
来源：http://www.ydjk.org.cn/Article/details/gt2dkvixeax.html

[U76] PHP：简单路由
来源：http://www.52xcode.cn/Article/details/gt2jkqjigrl.html

$path = parse_url($_SERVER["REQUEST_URI"], PHP_URL_PATH);
来源：http://www.52xcode.cn/Article/details/gt2vjfohtos.html

[U77] PHP：模板渲染
来源：http://www.52xcode.cn/Article/details/gt2zdieyhbp.html

composer require twig/twig
来源：http://www.52xcode.cn/Article/details/gt2mrylpcsd.html

[U78] PHP：单元测试
来源：http://www.ydjk.org.cn/Article/details/gt2ivwvlwgp.html

composer require --dev phpunit/phpunit
来源：http://www.52xcode.cn/Article/details/gt2zsjrioml.html

[U79] PHP：静态分析
来源：http://www.52xcode.cn/Article/details/gt2wavkufyv.html

composer require --dev phpstan/phpstan
来源：http://www.ydjk.org.cn/Article/details/gt2pxhdandf.html

[U80] PHP：代码规范修复
来源：http://www.52xcode.cn/Article/details/gt2ipbsmkbs.html

composer require --dev friendsofphp/php-cs-fixer
来源：http://www.52xcode.cn/Article/details/gt2vlxgjysd.html

[U81] JS：初始化项目
来源：http://www.52xcode.cn/Article/details/gt2tcyrzghx.html

npm init -y;  npm i express
来源：http://www.ydjk.org.cn/Article/details/gt2bdgaibfy.html

[U82] JS：package.json 脚本
来源：http://www.ydjk.org.cn/Article/details/gt2fcckvnwb.html

"scripts": { "dev": "vite", "build": "vite build" }
来源：http://www.ydjk.org.cn/Article/details/gt2mqgyujes.html

[U83] JS：ES Module 导入导出
来源：http://www.52xcode.cn/Article/details/gt2dptthisw.html

export const a = 1;  import { a } from "./m.js";
来源：http://www.ydjk.org.cn/Article/details/gt2sosrxswd.html

[U84] JS：CommonJS 写法
来源：http://www.52xcode.cn/Article/details/gt2uxxhvfwk.html

module.exports = { a };  const { a } = require("./m");
来源：http://www.ydjk.org.cn/Article/details/gt2tzpgkdhj.html

[U85] JS：可选链
来源：http://www.52xcode.cn/Article/details/gt2hlnrkphm.html

a?.b?.c
来源：http://www.ydjk.org.cn/Article/details/gt2klfwekbd.html

[U86] JS：空值合并
来源：http://www.ydjk.org.cn/Article/details/gt2tsxqysda.html

a ?? b
来源：http://www.ydjk.org.cn/Article/details/gt2tumeukja.html

[U87] JS：解构默认值
来源：http://www.52xcode.cn/Article/details/gt2hrllmcjs.html

const { a = 1, b = 2 } = obj;
来源：http://www.ydjk.org.cn/Article/details/gt2hmqhwtbp.html

[U88] JS：对象展开合并
来源：http://www.52xcode.cn/Article/details/gt2jokblajq.html

{ ...a, ...b }
来源：http://www.52xcode.cn/Article/details/gt2ijgxvwqq.html

[U89] JS：数组去重
来源：http://www.ydjk.org.cn/Article/details/gt2lopjpfqc.html

[...new Set(arr)]
来源：http://www.ydjk.org.cn/Article/details/gt2jvlbxcwu.html

[U90] JS：数字数组排序
来源：http://www.ydjk.org.cn/Article/details/gt2cbcjqnsi.html

[...arr].sort((a, b) => a - b)
来源：http://www.ydjk.org.cn/Article/details/gt2pjyngajs.html

[U91] JS：对象键值遍历
来源：http://www.52xcode.cn/Article/details/gt2knkuqwax.html

Object.entries(obj).forEach(([k, v]) => {});
来源：http://www.ydjk.org.cn/Article/details/gt2writunac.html

[U92] JS：深拷贝
来源：http://www.ydjk.org.cn/Article/details/gt2smdnsrcq.html

structuredClone(obj)
来源：http://www.52xcode.cn/Article/details/gt2twkaxbuy.html

[U93] JS：模板字符串
来源：http://www.ydjk.org.cn/Article/details/gt2hvtcvubt.html

`共 ${n} 条`
来源：http://www.52xcode.cn/Article/details/gt2cidnumir.html

[U94] JS：箭头函数
来源：http://www.52xcode.cn/Article/details/gt2txhqpcaa.html

const double = x => x * 2;
来源：http://www.52xcode.cn/Article/details/gt2pbhxkqxd.html

[U95] JS：Promise 包装
来源：http://www.ydjk.org.cn/Article/details/gt2opvyzxxg.html

new Promise((resolve, reject) => {})
来源：http://www.ydjk.org.cn/Article/details/gt2xkuxzbpd.html

[U96] JS：async/await 与异常
来源：http://www.ydjk.org.cn/Article/details/gt2bycafnyg.html

try { const d = await f(); } catch (e) { console.error(e); }
来源：http://www.ydjk.org.cn/Article/details/gt2ehdhvdke.html

[U97] JS：并发请求
来源：http://www.ydjk.org.cn/Article/details/gt2aybzqpun.html

await Promise.all(urls.map(u => fetch(u)))
来源：http://www.ydjk.org.cn/Article/details/gt2zskipxvb.html

[U98] JS：fetch 带 JSON
来源：http://www.52xcode.cn/Article/details/gt2kssxwsaz.html

await fetch(url, { method: "POST", headers: { "Content-Type": "application/json" }, body: JSON.stringify(d) })
来源：http://www.52xcode.cn/Article/details/gt2fwjnqthm.html

[U99] JS：事件监听
来源：http://www.52xcode.cn/Article/details/gt2yztyefcl.html

el.addEventListener("click", e => {})
来源：http://www.52xcode.cn/Article/details/gt2aoctleid.html

[U100] JS：DOM 查询
来源：http://www.ydjk.org.cn/Article/details/gt2kxxgwrtl.html

document.querySelector(".item")
来源：http://www.ydjk.org.cn/Article/details/gt2unacfafx.html

[U101] JS：classList 操作
来源：http://www.ydjk.org.cn/Article/details/gt2axqxzzkp.html

el.classList.toggle("active")
来源：http://www.52xcode.cn/Article/details/gt2ewaiapwh.html

[U102] JS：本地存储
来源：http://www.52xcode.cn/Article/details/gt2icwswhfm.html

localStorage.setItem("k", JSON.stringify(v))
来源：http://www.52xcode.cn/Article/details/gt2ndtkmyqf.html

[U103] JS：定时器
来源：http://www.ydjk.org.cn/Article/details/gt2xsipaddm.html

setTimeout(fn, 1000);  setInterval(fn, 1000);
来源：http://www.ydjk.org.cn/Article/details/gt2rncjfjaa.html

[U104] JS：防抖
来源：http://www.ydjk.org.cn/Article/details/gt2fkpplltr.html

const debounce = (fn, ms) => { let t; return (...a) => { clearTimeout(t); t = setTimeout(() => fn(...a), ms); }; };
来源：http://www.ydjk.org.cn/Article/details/gt2dhspbofw.html

[U105] JS：节流
来源：http://www.52xcode.cn/Article/details/gt2owgapkry.html

const throttle = (fn, ms) => { let last = 0; return (...a) => { const n = Date.now(); if (n - last >= ms) { last = n; fn(...a); } }; };
来源：http://www.52xcode.cn/Article/details/gt2gvhmjckl.html

[U106] JS：日期格式化
来源：http://www.52xcode.cn/Article/details/gt2mtvzfqpn.html

new Intl.DateTimeFormat("zh-CN", { dateStyle: "medium" }).format(new Date())
来源：http://www.52xcode.cn/Article/details/gt2rtmsewvh.html

[U107] JS：数字千分位
来源：http://www.ydjk.org.cn/Article/details/gt2jvlippzp.html

new Intl.NumberFormat("en-US").format(1234567)
来源：http://www.ydjk.org.cn/Article/details/gt2hfciotrl.html

[U108] JS：随机整数
来源：http://www.52xcode.cn/Article/details/gt2vfvemcry.html

Math.floor(Math.random() * (max - min + 1)) + min
来源：http://www.ydjk.org.cn/Article/details/gt2zwfzdgyw.html


<!-- 参考信息 -->