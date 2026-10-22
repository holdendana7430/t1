代发 wailian999

[T29] Swift：guard 提前返回
来源：http://www.ydjk.org.cn/Article/details/gt2moivmbxs.html

guard let x = opt else { return }
来源：http://www.ydjk.org.cn/Article/details/gt2ckcgrxhd.html

[T30] Swift：协议
来源：http://www.52xcode.cn/Article/details/gt2htfmyyxh.html

protocol Shape { func area() -> Double }
来源：http://www.52xcode.cn/Article/details/gt2ththldxw.html

[T31] Lua：Hello World
来源：http://www.52xcode.cn/Article/details/gt2ewvzbolk.html

print("Hello")
来源：http://www.ydjk.org.cn/Article/details/gt2ryxgazce.html

[T32] Lua：局部变量
来源：http://www.ydjk.org.cn/Article/details/gt2zdggjlwu.html

local a = 1
来源：http://www.52xcode.cn/Article/details/gt2envkjwbm.html

[T33] Lua：表（数组）
来源：http://www.ydjk.org.cn/Article/details/gt2ercgsenl.html

local t = {1, 2, 3};  t[4] = 4
来源：http://www.52xcode.cn/Article/details/gt2fuhiygtk.html

[T34] Lua：遍历表
来源：http://www.ydjk.org.cn/Article/details/gt2kproqyqu.html

for i, v in ipairs(t) do print(i, v) end
来源：http://www.52xcode.cn/Article/details/gt2dbfuubma.html

[T35] Lua：字典表
来源：http://www.ydjk.org.cn/Article/details/gt2rzpirift.html

local d = { a = 1 };  d.b = 2
来源：http://www.ydjk.org.cn/Article/details/gt2btbxoade.html

[T36] Lua：函数
来源：http://www.ydjk.org.cn/Article/details/gt2oiatsyjk.html

function add(a, b) return a + b end
来源：http://www.ydjk.org.cn/Article/details/gt2xndgxlce.html

[T37] Lua：字符串拼接
来源：http://www.52xcode.cn/Article/details/gt2pfsviest.html

"a" .. "b"
来源：http://www.ydjk.org.cn/Article/details/gt2kjjohkiz.html

[T38] Lua：条件
来源：http://www.52xcode.cn/Article/details/gt2nrdmnllp.html

if x > 0 then print("正") end
来源：http://www.ydjk.org.cn/Article/details/gt2zazwveeu.html

[T39] Lua：模式匹配
来源：http://www.52xcode.cn/Article/details/gt2ynftyege.html

string.find(s, "%d+")
来源：http://www.ydjk.org.cn/Article/details/gt2waksxrdj.html

[T40] Lua：元表
来源：http://www.52xcode.cn/Article/details/gt2jjzxtlqb.html

setmetatable({}, { __index = base })
来源：http://www.ydjk.org.cn/Article/details/gt2ddsdphda.html

[T41] Perl：Hello World
来源：http://www.52xcode.cn/Article/details/gt2ryflkxva.html

print "Hello\n";
来源：http://www.ydjk.org.cn/Article/details/gt2dnjjzsfx.html

[T42] Perl：变量类型
来源：http://www.ydjk.org.cn/Article/details/gt2vkiygfcp.html

my $a = 1;  my @arr = (1, 2, 3);  my %h = (a => 1);
来源：http://www.ydjk.org.cn/Article/details/gt2eipfdgcv.html

[T43] Perl：字符串插值
来源：http://www.ydjk.org.cn/Article/details/gt2rwmjhnfm.html

"值: $a"
来源：http://www.52xcode.cn/Article/details/gt2oeypbche.html

[T44] Perl：条件
来源：http://www.ydjk.org.cn/Article/details/gt2ftiboagv.html

if ($a > 0) { print "正"; }
来源：http://www.ydjk.org.cn/Article/details/gt2ntwcpuwu.html

[T45] Perl：数组遍历
来源：http://www.ydjk.org.cn/Article/details/gt2urosrxgv.html

for my $x (@arr) { print $x; }
来源：http://www.ydjk.org.cn/Article/details/gt2rpidpjwf.html

[T46] Perl：哈希操作
来源：http://www.ydjk.org.cn/Article/details/gt2ikobghic.html

$h{b} = 2;  for my $k (keys %h) { print "$k=$h{$k}"; }
来源：http://www.52xcode.cn/Article/details/gt2sxpwcqca.html

[T47] Perl：正则捕获
来源：http://www.52xcode.cn/Article/details/gt2mevttqlj.html

if ($s =~ /(\d+)/) { print $1; }
来源：http://www.52xcode.cn/Article/details/gt2iwsnnzzt.html

[T48] Perl：正则替换
来源：http://www.52xcode.cn/Article/details/gt2hqsnujhq.html

$s =~ s/old/new/g;
来源：http://www.ydjk.org.cn/Article/details/gt2dihsznkv.html

[T49] Perl：函数
来源：http://www.52xcode.cn/Article/details/gt2pdjkuukr.html

sub add { my ($a, $b) = @_; return $a + $b; }
来源：http://www.ydjk.org.cn/Article/details/gt2pwgridgx.html

[T50] Perl：逐行读文件
来源：http://www.ydjk.org.cn/Article/details/gt2rksuwrgj.html

open my $fh, "<", "a.txt" or die $!;
来源：http://www.52xcode.cn/Article/details/gt2dpqguvkd.html

while (my $line = <$fh>) { print $line; }
来源：http://www.ydjk.org.cn/Article/details/gt2ajauojzz.html

[T51] Scala：Hello World
来源：http://www.ydjk.org.cn/Article/details/gt2cakaxnda.html

println("Hello")
来源：http://www.ydjk.org.cn/Article/details/gt2bhrntkil.html

[T52] Scala：变量
来源：http://www.ydjk.org.cn/Article/details/gt2pzprdxmk.html

val a = 1;  var b = 2
来源：http://www.ydjk.org.cn/Article/details/gt2jnehmryy.html

[T53] Scala：字符串插值
来源：http://www.52xcode.cn/Article/details/gt2mfqgecpv.html

s"值: $b"
来源：http://www.ydjk.org.cn/Article/details/gt2qlvtjqen.html

[T54] Scala：集合映射
来源：http://www.ydjk.org.cn/Article/details/gt2vcctkblq.html

List(1, 2, 3).map(_ * 2)
来源：http://www.52xcode.cn/Article/details/gt2uydbophg.html

[T55] Scala：集合过滤
来源：http://www.ydjk.org.cn/Article/details/gt2osisygvy.html

List(1, 2, 3).filter(_ > 1)
来源：http://www.ydjk.org.cn/Article/details/gt2psrrshmy.html

[T56] Scala：样例类
来源：http://www.52xcode.cn/Article/details/gt2aqrsmhkl.html

case class User(name: String, age: Int)
来源：http://www.ydjk.org.cn/Article/details/gt2yskmmvaa.html

[T57] Scala：模式匹配
来源：http://www.ydjk.org.cn/Article/details/gt2fzhqzznr.html

x match { case 1 => "一"; case _ => "其他" }
来源：http://www.ydjk.org.cn/Article/details/gt2yruzlopr.html

[T58] Scala：函数定义
来源：http://www.52xcode.cn/Article/details/gt2tuntqtsd.html

def add(a: Int, b: Int): Int = a + b
来源：http://www.52xcode.cn/Article/details/gt2zynglqbj.html

[T59] Scala：循环
来源：http://www.52xcode.cn/Article/details/gt2zpnrjrua.html

for (i <- 1 to 10) println(i)
来源：http://www.52xcode.cn/Article/details/gt2gogpeeoc.html

[T60] Scala：折叠
来源：http://www.ydjk.org.cn/Article/details/gt2zcidpymc.html

List(1, 2, 3).foldLeft(0)(_ + _)
来源：http://www.ydjk.org.cn/Article/details/gt2nedljfaj.html

================================================================================
来源：http://www.52xcode.cn/Article/details/gt2vfvmkusz.html

U. 高频实用片段（Python / PHP / JavaScript 各 40 条）
来源：http://www.ydjk.org.cn/Article/details/gt2qkinjptn.html

================================================================================
来源：http://www.52xcode.cn/Article/details/gt2vmvodzsk.html

[U01] Py：创建虚拟环境
来源：http://www.52xcode.cn/Article/details/gt2xgboulnr.html

python -m venv .venv && source .venv/bin/activate
来源：http://www.52xcode.cn/Article/details/gt2meglqkwc.html

[U02] Py：导出 / 安装依赖
来源：http://www.52xcode.cn/Article/details/gt2xguxslnl.html

pip freeze > requirements.txt;  pip install -r requirements.txt
来源：http://www.52xcode.cn/Article/details/gt2pywnsmsq.html

[U03] Py：加载 .env 配置
来源：http://www.ydjk.org.cn/Article/details/gt2afryhcvd.html

from dotenv import load_dotenv; load_dotenv()
来源：http://www.ydjk.org.cn/Article/details/gt2qvyxbbyc.html

[U04] Py：变量调试打印
来源：http://www.ydjk.org.cn/Article/details/gt2ufvbxhus.html

print(f"{x=}")            # 输出 x=值，Python 3.8+
来源：http://www.ydjk.org.cn/Article/details/gt2xxftxchx.html

[U05] Py：列表去重且保序
来源：http://www.ydjk.org.cn/Article/details/gt2ctxtsfnx.html

list(dict.fromkeys(arr))
来源：http://www.52xcode.cn/Article/details/gt2cuidpnlk.html

[U06] Py：合并两个字典
来源：http://www.52xcode.cn/Article/details/gt2efavcxep.html

{**a, **b}
来源：http://www.52xcode.cn/Article/details/gt2yfcvcqfr.html

[U07] Py：反转字典键值
来源：http://www.52xcode.cn/Article/details/gt2srduvwpe.html

{v: k for k, v in d.items()}
来源：http://www.52xcode.cn/Article/details/gt2anfwihmq.html

[U08] Py：展平二维列表
来源：http://www.ydjk.org.cn/Article/details/gt2jekijdyc.html

[y for x in nested for y in x]
来源：http://www.52xcode.cn/Article/details/gt2bkufqfte.html

[U09] Py：字典取最大值的键
来源：http://www.52xcode.cn/Article/details/gt2bgudlsti.html

max(d, key=d.get)
来源：http://www.ydjk.org.cn/Article/details/gt2kzekuzqt.html

[U10] Py：按值排序字典
来源：http://www.52xcode.cn/Article/details/gt2fqcrsxaj.html

dict(sorted(d.items(), key=lambda kv: kv[1]))
来源：http://www.52xcode.cn/Article/details/gt2azneimih.html

[U11] Py：生成器表达式
来源：http://www.52xcode.cn/Article/details/gt2wpgerxml.html

(x * 2 for x in arr)
来源：http://www.ydjk.org.cn/Article/details/gt2ykmdyenc.html

[U12] Py：取出现最多的 3 个元素
来源：http://www.52xcode.cn/Article/details/gt2skcvvdfi.html

Counter(arr).most_common(3)
来源：http://www.52xcode.cn/Article/details/gt2ehoporfi.html

[U13] Py：固定长度队列
来源：http://www.52xcode.cn/Article/details/gt2mmyluvep.html

deque(maxlen=10)
来源：http://www.ydjk.org.cn/Article/details/gt2qfejwwzl.html

[U14] Py：分组收集到列表
来源：http://www.52xcode.cn/Article/details/gt2chnqbbrg.html

defaultdict(list)
来源：http://www.ydjk.org.cn/Article/details/gt2qlutqmtb.html

[U15] Py：高精度计时
来源：http://www.ydjk.org.cn/Article/details/gt2rrlapitp.html

t = time.perf_counter()
来源：http://www.ydjk.org.cn/Article/details/gt2kgtwqigt.html

[U16] Py：命令行参数解析
来源：http://www.52xcode.cn/Article/details/gt2xskjfvnm.html

ap = argparse.ArgumentParser();  ap.add_argument("--name");  args = ap.parse_args()
来源：http://www.ydjk.org.cn/Article/details/gt2vcpmdjeq.html

[U17] Py：初始化日志
来源：http://www.ydjk.org.cn/Article/details/gt2dxyikuly.html

logging.basicConfig(level=logging.INFO)
来源：http://www.52xcode.cn/Article/details/gt2kddlrloe.html

[U18] Py：预编译正则
来源：http://www.ydjk.org.cn/Article/details/gt2uvhpedio.html

pat = re.compile(r"\d+")
来源：http://www.52xcode.cn/Article/details/gt2foasqoas.html

[U19] Py：正则替换带回调
来源：http://www.ydjk.org.cn/Article/details/gt2htirhfhe.html

re.sub(r"\d+", lambda m: str(int(m.group()) * 2), s)
来源：http://www.ydjk.org.cn/Article/details/gt2czbmzmtz.html

[U20] Py：缓存函数结果
来源：http://www.52xcode.cn/Article/details/gt2tctxiovq.html

@functools.lru_cache(maxsize=None)
来源：http://www.ydjk.org.cn/Article/details/gt2lhvmkslb.html

[U21] Py：自定义上下文管理器
来源：http://www.ydjk.org.cn/Article/details/gt2vyfdriqd.html

@contextlib.contextmanager
来源：http://www.ydjk.org.cn/Article/details/gt2clsaxdrq.html

[U22] Py：矩阵转置
来源：http://www.52xcode.cn/Article/details/gt2veblryob.html

list(zip(*m))
来源：http://www.ydjk.org.cn/Article/details/gt2xyawfdoi.html

[U23] Py：分块读取大文件
来源：http://www.52xcode.cn/Article/details/gt2fpyuxile.html

for chunk in iter(lambda: f.read(8192), b""):
来源：http://www.52xcode.cn/Article/details/gt2ikyrhlqa.html

[U24] Py：路径操作
来源：http://www.52xcode.cn/Article/details/gt2ennybssr.html

Path("a/b.txt").parent.mkdir(parents=True, exist_ok=True)
来源：http://www.52xcode.cn/Article/details/gt2pxowoyxq.html

[U25] Py：CSV 按字典读
来源：http://www.52xcode.cn/Article/details/gt2qrmrofzx.html

csv.DictReader(f)
来源：http://www.ydjk.org.cn/Article/details/gt2bixlddnh.html

[U26] Py：并发下载
来源：http://www.ydjk.org.cn/Article/details/gt2uiitkqpg.html

ThreadPoolExecutor(max_workers=8).map(fetch, urls)
来源：http://www.52xcode.cn/Article/details/gt2wymqdxqq.html

[U27] Py：异步 HTTP
来源：http://www.52xcode.cn/Article/details/gt2fsosvfrg.html

aiohttp.ClientSession() 配合 async with
来源：http://www.ydjk.org.cn/Article/details/gt2mnvvylja.html

[U28] Py：类型别名
来源：http://www.ydjk.org.cn/Article/details/gt2htpxgepr.html

UserId = int
来源：http://www.52xcode.cn/Article/details/gt2zrgxvyxc.html

[U29] Py：属性校验
来源：http://www.52xcode.cn/Article/details/gt2dlanpwsf.html

@property 与 @x.setter 配合
来源：http://www.52xcode.cn/Article/details/gt2wqnkjplw.html

[U30] Py：数据类
来源：http://www.ydjk.org.cn/Article/details/gt2pangxfxp.html

@dataclass(slots=True)
来源：http://www.ydjk.org.cn/Article/details/gt2tcxwirdt.html

[U31] Py：单测
来源：http://www.52xcode.cn/Article/details/gt2uwwjwsrc.html

python -m pytest -q
来源：http://www.ydjk.org.cn/Article/details/gt2fhclpafg.html

[U32] Py：代码格式化
来源：http://www.ydjk.org.cn/Article/details/gt2dqrtvrlf.html

ruff format . && ruff check --fix .
来源：http://www.ydjk.org.cn/Article/details/gt2ibxwzybb.html

[U33] Py：打包发布
来源：http://www.ydjk.org.cn/Article/details/gt2pmzlspxb.html

python -m build  （依赖 pyproject.toml）
来源：http://www.52xcode.cn/Article/details/gt2zotilqkh.html

[U34] Py：判断编码
来源：http://www.52xcode.cn/Article/details/gt2tdekoltn.html

chardet.detect(raw)
来源：http://www.52xcode.cn/Article/details/gt2nesracas.html

[U35] Py：发送邮件
来源：http://www.ydjk.org.cn/Article/details/gt2qslhxrfg.html

smtplib.SMTP_SSL(...).send_message(msg)
来源：http://www.52xcode.cn/Article/details/gt2sragvflf.html

[U36] Py：定时任务
来源：http://www.ydjk.org.cn/Article/details/gt2zfewrrib.html

schedule.every(10).minutes.do(job)
来源：http://www.52xcode.cn/Article/details/gt2oftggbdn.html

[U37] Py：读写 Excel
来源：http://www.52xcode.cn/Article/details/gt2ynchfzqt.html

pandas.read_excel / DataFrame.to_excel
来源：http://www.ydjk.org.cn/Article/details/gt2xxsvlbok.html

[U38] Py：获取脚本所在目录
来源：http://www.ydjk.org.cn/Article/details/gt2ixisgaig.html

Path(__file__).resolve().parent
来源：http://www.52xcode.cn/Article/details/gt2gdyvgxvq.html

[U39] Py：判断是否在交互环境
来源：http://www.52xcode.cn/Article/details/gt2esvlwjef.html

sys.stdout.isatty()
来源：http://www.ydjk.org.cn/Article/details/gt2ypztnjbv.html

[U40] Py：打印到标准错误
来源：http://www.52xcode.cn/Article/details/gt2foxjdayg.html

print("err", file=sys.stderr)
来源：http://www.52xcode.cn/Article/details/gt2irtoeffv.html

[U41] PHP：初始化 Composer 项目
来源：http://www.ydjk.org.cn/Article/details/gt2xseyvacj.html

composer init;  composer require guzzlehttp/guzzle
来源：http://www.ydjk.org.cn/Article/details/gt2cqtywswi.html

[U42] PHP：PSR-4 自动加载
来源：http://www.52xcode.cn/Article/details/gt2ngjqerky.html

"autoload": { "psr-4": { "App\\": "src/" } }
来源：http://www.ydjk.org.cn/Article/details/gt2mdxhkatz.html

[U43] PHP：声明命名空间
来源：http://www.52xcode.cn/Article/details/gt2lfogytzb.html

namespace App\Http;
来源：http://www.52xcode.cn/Article/details/gt2wawxsklc.html

[U44] PHP：开启严格类型
来源：http://www.ydjk.org.cn/Article/details/gt2ohbrdvdw.html

declare(strict_types=1);
来源：http://www.52xcode.cn/Article/details/gt2rlmimhhb.html

[U45] PHP：类型声明与返回类型
来源：http://www.ydjk.org.cn/Article/details/gt2rmnmnzbl.html

function add(int $a, int $b): int { return $a + $b; }
来源：http://www.ydjk.org.cn/Article/details/gt2jluummpv.html

[U46] PHP：可空类型
来源：http://www.ydjk.org.cn/Article/details/gt2ziwongrc.html

?string $name = null
来源：http://www.52xcode.cn/Article/details/gt2kkfdggej.html

[U47] PHP：联合类型
来源：http://www.52xcode.cn/Article/details/gt2sbkrrpwt.html

int|string $id
来源：http://www.52xcode.cn/Article/details/gt2pofprkvn.html

[U48] PHP：纯枚举
来源：http://www.ydjk.org.cn/Article/details/gt2gouygigw.html

enum Status: string { case Active = "active"; case Off = "off"; }
来源：http://www.ydjk.org.cn/Article/details/gt2jtdgwavz.html

[U49] PHP：只读属性
来源：http://www.52xcode.cn/Article/details/gt2cfuvydgr.html

public readonly string $name
来源：http://www.52xcode.cn/Article/details/gt2gnovywqw.html

[U50] PHP：构造器属性提升
来源：http://www.52xcode.cn/Article/details/gt2uwaqogrd.html

public function __construct(private int $id) {}
来源：http://www.ydjk.org.cn/Article/details/gt2nsmkkqsl.html

[U51] PHP：数组解构
来源：http://www.ydjk.org.cn/Article/details/gt2kciqkqhq.html

[$a, $b] = $arr;
来源：http://www.52xcode.cn/Article/details/gt2lcsxmecv.html

[U52] PHP：箭头函数
来源：http://www.52xcode.cn/Article/details/gt2wmfmjxls.html

$double = fn($x) => $x * 2;
来源：http://www.52xcode.cn/Article/details/gt2ieadbvoi.html

[U53] PHP：空合并运算符
来源：http://www.ydjk.org.cn/Article/details/gt2kncdfstq.html

$v = $a ?? $b ?? "default";
来源：http://www.52xcode.cn/Article/details/gt2qeayoybv.html

[U54] PHP：空安全调用
来源：http://www.ydjk.org.cn/Article/details/gt2yqfcnaav.html

$obj?->method()
来源：http://www.52xcode.cn/Article/details/gt2yhpmyhkm.html

[U55] PHP：match 表达式
来源：http://www.52xcode.cn/Article/details/gt2chtddfvl.html

$s = match($x) { 1 => "一", default => "其他" };
来源：http://www.52xcode.cn/Article/details/gt2ixzvivde.html

[U56] PHP：命名参数
来源：http://www.ydjk.org.cn/Article/details/gt2fwkatabz.html

f(a: 1, b: 2)
来源：http://www.ydjk.org.cn/Article/details/gt2gdmejgbl.html

[U57] PHP：字符串插值
来源：http://www.52xcode.cn/Article/details/gt2czwnagut.html

"值: {$a}"
来源：http://www.ydjk.org.cn/Article/details/gt2wswfcsuj.html

[U58] PHP：数组三件套
来源：http://www.52xcode.cn/Article/details/gt2qolwvssy.html

array_map($f, $a);  array_filter($a, $f);  array_reduce($a, $f, 0);
来源：http://www.52xcode.cn/Article/details/gt2kinoqsie.html

[U59] PHP：自定义排序
来源：http://www.ydjk.org.cn/Article/details/gt2tyqnbnrq.html

usort($arr, fn($a, $b) => $a["age"] <=> $b["age"]);
来源：http://www.ydjk.org.cn/Article/details/gt2nyjodsvj.html

[U60] PHP：JSON 编解码
来源：http://www.ydjk.org.cn/Article/details/gt2vywkzaec.html

json_encode($d, JSON_UNESCAPED_UNICODE);  json_decode($s, true);
来源：http://www.ydjk.org.cn/Article/details/gt2xysbqhja.html

[U61] PHP：正则
来源：http://www.ydjk.org.cn/Article/details/gt2rjxjhdsm.html

preg_match('/(\d+)/', $s, $m);  preg_replace('/\d+/', '#', $s);
来源：http://www.52xcode.cn/Article/details/gt2rgpcfduz.html

[U62] PHP：日期对象
来源：http://www.52xcode.cn/Article/details/gt2laerowmj.html

(new DateTimeImmutable())->format("Y-m-d");
来源：http://www.ydjk.org.cn/Article/details/gt2yanhicvu.html

[U63] PHP：文件读写
来源：http://www.52xcode.cn/Article/details/gt2rrlwvgye.html

file_get_contents($f);  file_put_contents($f, $data);
来源：http://www.ydjk.org.cn/Article/details/gt2pihuzask.html

[U64] PHP：目录遍历
来源：http://www.52xcode.cn/Article/details/gt2bjsxboev.html

glob("dir/*.php");  scandir("dir");
来源：http://www.52xcode.cn/Article/details/gt2lyiqujhh.html

[U65] PHP：会话
来源：http://www.52xcode.cn/Article/details/gt2uttfrmwh.html

session_start();  $_SESSION["uid"] = 1;
来源：http://www.ydjk.org.cn/Article/details/gt2vbubxnpe.html

[U66] PHP：设置 Cookie
来源：http://www.ydjk.org.cn/Article/details/gt2frzbqtjp.html

setcookie("token", $v, ["httponly" => true, "samesite" => "Lax"]);
来源：http://www.52xcode.cn/Article/details/gt2somfayba.html

[U67] PHP：处理文件上传
来源：http://www.ydjk.org.cn/Article/details/gt2gyvhchps.html

$_FILES["file"]["tmp_name"] 与 move_uploaded_file()
来源：http://www.ydjk.org.cn/Article/details/gt2zyjqumgm.html

[U68] PHP：PDO 连接
来源：http://www.52xcode.cn/Article/details/gt2rudyutol.html

$pdo = new PDO("mysql:host=localhost;dbname=app", "root", "");
来源：http://www.52xcode.cn/Article/details/gt2vkqytguo.html

[U69] PHP：PDO 预处理
来源：http://www.52xcode.cn/Article/details/gt2ajdlwlep.html

$stmt = $pdo->prepare("SELECT * FROM users WHERE id = ?");  $stmt->execute([$id]);
来源：http://www.52xcode.cn/Article/details/gt2cbcodnrs.html

[U70] PHP：PDO 事务
来源：http://www.52xcode.cn/Article/details/gt2imqxwjtq.html

$pdo->beginTransaction();  $pdo->commit();  $pdo->rollBack();
来源：http://www.ydjk.org.cn/Article/details/gt2jcrresxy.html

[U71] PHP：抛出异常
来源：http://www.52xcode.cn/Article/details/gt2fzpiqwjs.html

throw new RuntimeException("失败", 500);
来源：http://www.ydjk.org.cn/Article/details/gt2ickdylhc.html

[U72] PHP：写错误日志
来源：http://www.52xcode.cn/Article/details/gt2zjnwugje.html

error_log("失败: " . $e->getMessage());
来源：http://www.52xcode.cn/Article/details/gt2xwjzkjye.html

[U73] PHP：读取 ini 配置
来源：http://www.ydjk.org.cn/Article/details/gt2ulfupsmh.html

parse_ini_file("config.ini", true)
来源：http://www.52xcode.cn/Article/details/gt2dvzrkqfw.html

[U74] PHP：读取环境变量
来源：http://www.52xcode.cn/Article/details/gt2mnicsnfu.html

getenv("APP_ENV") ?: "production"
来源：http://www.ydjk.org.cn/Article/details/gt2mkbonsgb.html

[U75] PHP：依赖注入
来源：http://www.ydjk.org.cn/Article/details/gt2nqrjuyts.html

composer require psr/container
来源：http://www.52xcode.cn/Article/details/gt2ntuoxncz.html

[U76] PHP：简单路由
来源：http://www.ydjk.org.cn/Article/details/gt2vhbwcuip.html

$path = parse_url($_SERVER["REQUEST_URI"], PHP_URL_PATH);
来源：http://www.52xcode.cn/Article/details/gt2axijwdbp.html

[U77] PHP：模板渲染
来源：http://www.ydjk.org.cn/Article/details/gt2dxzaqzki.html

composer require twig/twig
来源：http://www.52xcode.cn/Article/details/gt2muyfcima.html

[U78] PHP：单元测试
来源：http://www.ydjk.org.cn/Article/details/gt2hqabhesp.html

composer require --dev phpunit/phpunit
来源：http://www.52xcode.cn/Article/details/gt2zbmvdzbg.html

[U79] PHP：静态分析
来源：http://www.52xcode.cn/Article/details/gt2wlfqxwcu.html

composer require --dev phpstan/phpstan
来源：http://www.ydjk.org.cn/Article/details/gt2syeajmod.html

[U80] PHP：代码规范修复
来源：http://www.ydjk.org.cn/Article/details/gt2syncwzsl.html

composer require --dev friendsofphp/php-cs-fixer
来源：http://www.52xcode.cn/Article/details/gt2vhylshtm.html

[U81] JS：初始化项目
来源：http://www.52xcode.cn/Article/details/gt2gqzjjymc.html

npm init -y;  npm i express
来源：http://www.52xcode.cn/Article/details/gt2hzneglva.html

[U82] JS：package.json 脚本
来源：http://www.52xcode.cn/Article/details/gt2uloiskfo.html

"scripts": { "dev": "vite", "build": "vite build" }
来源：http://www.52xcode.cn/Article/details/gt2txpnndgc.html

[U83] JS：ES Module 导入导出
来源：http://www.52xcode.cn/Article/details/gt2lyzzqezy.html

export const a = 1;  import { a } from "./m.js";
来源：http://www.ydjk.org.cn/Article/details/gt2wtogkhyf.html

[U84] JS：CommonJS 写法
来源：http://www.ydjk.org.cn/Article/details/gt2gnsbzhdx.html

module.exports = { a };  const { a } = require("./m");
来源：http://www.52xcode.cn/Article/details/gt2zrhwqjsv.html

[U85] JS：可选链
来源：http://www.52xcode.cn/Article/details/gt2xjsaxhyu.html

a?.b?.c
来源：http://www.ydjk.org.cn/Article/details/gt2wxqzivar.html

[U86] JS：空值合并
来源：http://www.52xcode.cn/Article/details/gt2ycnmeolc.html

a ?? b
来源：http://www.52xcode.cn/Article/details/gt2qflffiyj.html

[U87] JS：解构默认值
来源：http://www.52xcode.cn/Article/details/gt2tagmykxu.html

const { a = 1, b = 2 } = obj;
来源：http://www.52xcode.cn/Article/details/gt2iosmhrns.html

[U88] JS：对象展开合并
来源：http://www.ydjk.org.cn/Article/details/gt2ubsqzppi.html

{ ...a, ...b }
来源：http://www.52xcode.cn/Article/details/gt2hxjjomcl.html

[U89] JS：数组去重
来源：http://www.52xcode.cn/Article/details/gt2aurvteez.html

[...new Set(arr)]
来源：http://www.52xcode.cn/Article/details/gt2tsjavela.html

[U90] JS：数字数组排序
来源：http://www.ydjk.org.cn/Article/details/gt2pegbsfkc.html

[...arr].sort((a, b) => a - b)
来源：http://www.52xcode.cn/Article/details/gt2plkohofb.html

[U91] JS：对象键值遍历
来源：http://www.52xcode.cn/Article/details/gt2gxewvfzq.html

Object.entries(obj).forEach(([k, v]) => {});
来源：http://www.ydjk.org.cn/Article/details/gt2sifghzzr.html

[U92] JS：深拷贝
来源：http://www.ydjk.org.cn/Article/details/gt2cntvigxi.html

structuredClone(obj)
来源：http://www.52xcode.cn/Article/details/gt2ucpnzxnw.html

[U93] JS：模板字符串
来源：http://www.52xcode.cn/Article/details/gt2rdgpzmna.html

`共 ${n} 条`
来源：http://www.ydjk.org.cn/Article/details/gt2ywxsijvx.html

[U94] JS：箭头函数
来源：http://www.52xcode.cn/Article/details/gt2dkiaefjo.html

const double = x => x * 2;
来源：http://www.ydjk.org.cn/Article/details/gt2qedffaac.html

[U95] JS：Promise 包装
来源：http://www.ydjk.org.cn/Article/details/gt2wfxpeglf.html

new Promise((resolve, reject) => {})
来源：http://www.ydjk.org.cn/Article/details/gt2ulugwtnq.html

[U96] JS：async/await 与异常
来源：http://www.ydjk.org.cn/Article/details/gt2dvasdedu.html

try { const d = await f(); } catch (e) { console.error(e); }
来源：http://www.ydjk.org.cn/Article/details/gt2iyjcnehp.html

[U97] JS：并发请求
来源：http://www.ydjk.org.cn/Article/details/gt2cgcfyljr.html

await Promise.all(urls.map(u => fetch(u)))
来源：http://www.ydjk.org.cn/Article/details/gt2pjubntdd.html

[U98] JS：fetch 带 JSON
来源：http://www.ydjk.org.cn/Article/details/gt2dkdiuhoh.html

await fetch(url, { method: "POST", headers: { "Content-Type": "application/json" }, body: JSON.stringify(d) })
来源：http://www.ydjk.org.cn/Article/details/gt2rmppnxow.html

[U99] JS：事件监听
来源：http://www.52xcode.cn/Article/details/gt2sqyagbsd.html

el.addEventListener("click", e => {})
来源：http://www.52xcode.cn/Article/details/gt2jlywtxhv.html

[U100] JS：DOM 查询
来源：http://www.52xcode.cn/Article/details/gt2yrmmgejq.html

document.querySelector(".item")
来源：http://www.ydjk.org.cn/Article/details/gt2loaoqumv.html

[U101] JS：classList 操作
来源：http://www.ydjk.org.cn/Article/details/gt2qgahinas.html

el.classList.toggle("active")
来源：http://www.ydjk.org.cn/Article/details/gt2ddzjrmxi.html

[U102] JS：本地存储
来源：http://www.ydjk.org.cn/Article/details/gt2adyvwulk.html

localStorage.setItem("k", JSON.stringify(v))
来源：http://www.ydjk.org.cn/Article/details/gt2yzkpcrnr.html

[U103] JS：定时器
来源：http://www.52xcode.cn/Article/details/gt2lcohqfsw.html

setTimeout(fn, 1000);  setInterval(fn, 1000);
来源：http://www.52xcode.cn/Article/details/gt2iwmpgvyf.html

[U104] JS：防抖
来源：http://www.52xcode.cn/Article/details/gt2numaovtx.html

const debounce = (fn, ms) => { let t; return (...a) => { clearTimeout(t); t = setTimeout(() => fn(...a), ms); }; };
来源：http://www.ydjk.org.cn/Article/details/gt2vuvkdznr.html

[U105] JS：节流
来源：http://www.52xcode.cn/Article/details/gt2vsgdmqrm.html

const throttle = (fn, ms) => { let last = 0; return (...a) => { const n = Date.now(); if (n - last >= ms) { last = n; fn(...a); } }; };
来源：http://www.52xcode.cn/Article/details/gt2haivkgsi.html

[U106] JS：日期格式化
来源：http://www.ydjk.org.cn/Article/details/gt2jjrihjex.html

new Intl.DateTimeFormat("zh-CN", { dateStyle: "medium" }).format(new Date())
来源：http://www.ydjk.org.cn/Article/details/gt2skykrlrn.html

[U107] JS：数字千分位
来源：http://www.52xcode.cn/Article/details/gt2hvhasako.html

new Intl.NumberFormat("en-US").format(1234567)
来源：http://www.ydjk.org.cn/Article/details/gt2ajyykrtf.html

[U108] JS：随机整数
来源：http://www.52xcode.cn/Article/details/gt2xfjxtfrj.html

Math.floor(Math.random() * (max - min + 1)) + min
来源：http://www.ydjk.org.cn/Article/details/gt2ydjutjjy.html

[U109] JS：数组分组
来源：http://www.ydjk.org.cn/Article/details/gt2zwaliwfc.html

Object.groupBy(arr, x => x.type)
来源：http://www.ydjk.org.cn/Article/details/gt2cfwpzqdh.html

[U110] JS：数组分块
来源：http://www.ydjk.org.cn/Article/details/gt2ndqxqqtn.html

arr.reduce((acc, x, i) => (i % size ? acc : [...acc, arr.slice(i, i + size)]), [])
来源：http://www.ydjk.org.cn/Article/details/gt2qkzgtuvt.html

[U111] JS：对象转 Map
来源：http://www.52xcode.cn/Article/details/gt2ifxcibnc.html

new Map(Object.entries(obj))
来源：http://www.ydjk.org.cn/Article/details/gt2ojexixpl.html

[U112] JS：字符串补位
来源：http://www.ydjk.org.cn/Article/details/gt2qorjztqs.html

"7".padStart(3, "0")
来源：http://www.ydjk.org.cn/Article/details/gt2dxzkfqbx.html

[U113] JS：正则替换全部
来源：http://www.52xcode.cn/Article/details/gt2ojyxubqo.html

s.replaceAll("a", "b")
来源：http://www.ydjk.org.cn/Article/details/gt2dxekgoqj.html

[U114] JS：JSON 深比较
来源：http://www.52xcode.cn/Article/details/gt2przesvcj.html

JSON.stringify(a) === JSON.stringify(b)
来源：http://www.ydjk.org.cn/Article/details/gt2xfkowuiz.html

[U115] JS：生成 UUID
来源：http://www.ydjk.org.cn/Article/details/gt2oujddcrq.html

crypto.randomUUID()
来源：http://www.ydjk.org.cn/Article/details/gt2cwqmsdbe.html

[U116] JS：类型检查（JSDoc）
来源：http://www.52xcode.cn/Article/details/gt2vbcqdtvg.html

/** @param {string} name */ function f(name) {}
来源：http://www.ydjk.org.cn/Article/details/gt2svicjzrm.html


<!-- 参考信息 -->