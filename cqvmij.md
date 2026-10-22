代发 wailian999

[T29] Swift：guard 提前返回
来源：http://www.ydjk.org.cn/Article/details/gt2bxrkicpd.html

guard let x = opt else { return }
来源：http://www.ydjk.org.cn/Article/details/gt2qxfgfgpd.html

[T30] Swift：协议
来源：http://www.ydjk.org.cn/Article/details/gt2cohkpxld.html

protocol Shape { func area() -> Double }
来源：http://www.ydjk.org.cn/Article/details/gt2kzmssxbz.html

[T31] Lua：Hello World
来源：http://www.ydjk.org.cn/Article/details/gt2ahvwkzdl.html

print("Hello")
来源：http://www.ydjk.org.cn/Article/details/gt2cguobjwd.html

[T32] Lua：局部变量
来源：http://www.ydjk.org.cn/Article/details/gt2sovmbtbz.html

local a = 1
来源：http://www.ydjk.org.cn/Article/details/gt2bjavwbia.html

[T33] Lua：表（数组）
来源：http://www.ydjk.org.cn/Article/details/gt2yfheklyd.html

local t = {1, 2, 3};  t[4] = 4
来源：http://www.52xcode.cn/Article/details/gt2uefkkxov.html

[T34] Lua：遍历表
来源：http://www.ydjk.org.cn/Article/details/gt2getfkbao.html

for i, v in ipairs(t) do print(i, v) end
来源：http://www.ydjk.org.cn/Article/details/gt2yaaxjtnn.html

[T35] Lua：字典表
来源：http://www.ydjk.org.cn/Article/details/gt2vplpgyed.html

local d = { a = 1 };  d.b = 2
来源：http://www.52xcode.cn/Article/details/gt2jjpgrlox.html

[T36] Lua：函数
来源：http://www.52xcode.cn/Article/details/gt2zqhdbqiv.html

function add(a, b) return a + b end
来源：http://www.ydjk.org.cn/Article/details/gt2wrfnrmzx.html

[T37] Lua：字符串拼接
来源：http://www.52xcode.cn/Article/details/gt2qujzcvta.html

"a" .. "b"
来源：http://www.ydjk.org.cn/Article/details/gt2pgpzuhte.html

[T38] Lua：条件
来源：http://www.ydjk.org.cn/Article/details/gt2uoevucot.html

if x > 0 then print("正") end
来源：http://www.ydjk.org.cn/Article/details/gt2jljtiiwj.html

[T39] Lua：模式匹配
来源：http://www.ydjk.org.cn/Article/details/gt2plyjjcdx.html

string.find(s, "%d+")
来源：http://www.52xcode.cn/Article/details/gt2qeuzilty.html

[T40] Lua：元表
来源：http://www.52xcode.cn/Article/details/gt2iictczxu.html

setmetatable({}, { __index = base })
来源：http://www.52xcode.cn/Article/details/gt2ocymrebh.html

[T41] Perl：Hello World
来源：http://www.ydjk.org.cn/Article/details/gt2yunihjtu.html

print "Hello\n";
来源：http://www.52xcode.cn/Article/details/gt2pzvnmavn.html

[T42] Perl：变量类型
来源：http://www.ydjk.org.cn/Article/details/gt2rrpuiigh.html

my $a = 1;  my @arr = (1, 2, 3);  my %h = (a => 1);
来源：http://www.52xcode.cn/Article/details/gt2avdklhry.html

[T43] Perl：字符串插值
来源：http://www.ydjk.org.cn/Article/details/gt2zjkbchaa.html

"值: $a"
来源：http://www.52xcode.cn/Article/details/gt2myxyhuvp.html

[T44] Perl：条件
来源：http://www.ydjk.org.cn/Article/details/gt2tiiaiayz.html

if ($a > 0) { print "正"; }
来源：http://www.52xcode.cn/Article/details/gt2vhguqhil.html

[T45] Perl：数组遍历
来源：http://www.52xcode.cn/Article/details/gt2gulfltbb.html

for my $x (@arr) { print $x; }
来源：http://www.52xcode.cn/Article/details/gt2tldjzoks.html

[T46] Perl：哈希操作
来源：http://www.52xcode.cn/Article/details/gt2pbhavkdm.html

$h{b} = 2;  for my $k (keys %h) { print "$k=$h{$k}"; }
来源：http://www.52xcode.cn/Article/details/gt2idkixkyn.html

[T47] Perl：正则捕获
来源：http://www.52xcode.cn/Article/details/gt2wbzposnd.html

if ($s =~ /(\d+)/) { print $1; }
来源：http://www.52xcode.cn/Article/details/gt2ljazkecb.html

[T48] Perl：正则替换
来源：http://www.52xcode.cn/Article/details/gt2siavxcbr.html

$s =~ s/old/new/g;
来源：http://www.52xcode.cn/Article/details/gt2alztvwth.html

[T49] Perl：函数
来源：http://www.52xcode.cn/Article/details/gt2btwjbomt.html

sub add { my ($a, $b) = @_; return $a + $b; }
来源：http://www.52xcode.cn/Article/details/gt2ldpkmtdr.html

[T50] Perl：逐行读文件
来源：http://www.52xcode.cn/Article/details/gt2bcpnzdjc.html

open my $fh, "<", "a.txt" or die $!;
来源：http://www.ydjk.org.cn/Article/details/gt2ucqmxcgs.html

while (my $line = <$fh>) { print $line; }
来源：http://www.52xcode.cn/Article/details/gt2drgtvcop.html

[T51] Scala：Hello World
来源：http://www.ydjk.org.cn/Article/details/gt2nfgajnrl.html

println("Hello")
来源：http://www.ydjk.org.cn/Article/details/gt2xxgflmoh.html

[T52] Scala：变量
来源：http://www.ydjk.org.cn/Article/details/gt2nzhdjujo.html

val a = 1;  var b = 2
来源：http://www.ydjk.org.cn/Article/details/gt2nwmregoq.html

[T53] Scala：字符串插值
来源：http://www.52xcode.cn/Article/details/gt2riyboald.html

s"值: $b"
来源：http://www.52xcode.cn/Article/details/gt2cdlbzpjf.html

[T54] Scala：集合映射
来源：http://www.52xcode.cn/Article/details/gt2eucuzpkn.html

List(1, 2, 3).map(_ * 2)
来源：http://www.ydjk.org.cn/Article/details/gt2qdjnzxyi.html

[T55] Scala：集合过滤
来源：http://www.ydjk.org.cn/Article/details/gt2wnjiwqlf.html

List(1, 2, 3).filter(_ > 1)
来源：http://www.ydjk.org.cn/Article/details/gt2atgebcqf.html

[T56] Scala：样例类
来源：http://www.52xcode.cn/Article/details/gt2dazklgpa.html

case class User(name: String, age: Int)
来源：http://www.52xcode.cn/Article/details/gt2vdymskvc.html

[T57] Scala：模式匹配
来源：http://www.ydjk.org.cn/Article/details/gt2ngiggvjo.html

x match { case 1 => "一"; case _ => "其他" }
来源：http://www.ydjk.org.cn/Article/details/gt2zfdnfjia.html

[T58] Scala：函数定义
来源：http://www.ydjk.org.cn/Article/details/gt2xafhrmsn.html

def add(a: Int, b: Int): Int = a + b
来源：http://www.52xcode.cn/Article/details/gt2jyakrqjo.html

[T59] Scala：循环
来源：http://www.52xcode.cn/Article/details/gt2bfntprtz.html

for (i <- 1 to 10) println(i)
来源：http://www.52xcode.cn/Article/details/gt2tgocskat.html

[T60] Scala：折叠
来源：http://www.ydjk.org.cn/Article/details/gt2aejdpons.html

List(1, 2, 3).foldLeft(0)(_ + _)
来源：http://www.ydjk.org.cn/Article/details/gt2gpmpcvot.html

================================================================================
来源：http://www.ydjk.org.cn/Article/details/gt2miekjirl.html

U. 高频实用片段（Python / PHP / JavaScript 各 40 条）
来源：http://www.52xcode.cn/Article/details/gt2xapmploj.html

================================================================================
来源：http://www.52xcode.cn/Article/details/gt2woaqvkww.html

[U01] Py：创建虚拟环境
来源：http://www.52xcode.cn/Article/details/gt2myimssze.html

python -m venv .venv && source .venv/bin/activate
来源：http://www.52xcode.cn/Article/details/gt2eiiwyzsg.html

[U02] Py：导出 / 安装依赖
来源：http://www.52xcode.cn/Article/details/gt2wpmdmjmg.html

pip freeze > requirements.txt;  pip install -r requirements.txt
来源：http://www.ydjk.org.cn/Article/details/gt2bwzlcche.html

[U03] Py：加载 .env 配置
来源：http://www.52xcode.cn/Article/details/gt2xxwlssoj.html

from dotenv import load_dotenv; load_dotenv()
来源：http://www.52xcode.cn/Article/details/gt2dbuhxaid.html

[U04] Py：变量调试打印
来源：http://www.52xcode.cn/Article/details/gt2vssqoesa.html

print(f"{x=}")            # 输出 x=值，Python 3.8+
来源：http://www.52xcode.cn/Article/details/gt2vqtdujag.html

[U05] Py：列表去重且保序
来源：http://www.52xcode.cn/Article/details/gt2wnmmeblc.html

list(dict.fromkeys(arr))
来源：http://www.ydjk.org.cn/Article/details/gt2rfrjnloz.html

[U06] Py：合并两个字典
来源：http://www.ydjk.org.cn/Article/details/gt2bswytmjm.html

{**a, **b}
来源：http://www.ydjk.org.cn/Article/details/gt2smnvfjyv.html

[U07] Py：反转字典键值
来源：http://www.52xcode.cn/Article/details/gt2nxgapobx.html

{v: k for k, v in d.items()}
来源：http://www.ydjk.org.cn/Article/details/gt2ighmzpnc.html

[U08] Py：展平二维列表
来源：http://www.ydjk.org.cn/Article/details/gt2nntrjsuv.html

[y for x in nested for y in x]
来源：http://www.52xcode.cn/Article/details/gt2gnvuumvq.html

[U09] Py：字典取最大值的键
来源：http://www.ydjk.org.cn/Article/details/gt2jugivfhp.html

max(d, key=d.get)
来源：http://www.ydjk.org.cn/Article/details/gt2jalpmrks.html

[U10] Py：按值排序字典
来源：http://www.ydjk.org.cn/Article/details/gt2fdmqxxfi.html

dict(sorted(d.items(), key=lambda kv: kv[1]))
来源：http://www.52xcode.cn/Article/details/gt2fcsbedrj.html

[U11] Py：生成器表达式
来源：http://www.52xcode.cn/Article/details/gt2oamwmpmx.html

(x * 2 for x in arr)
来源：http://www.ydjk.org.cn/Article/details/gt2zkzouzav.html

[U12] Py：取出现最多的 3 个元素
来源：http://www.52xcode.cn/Article/details/gt2yuhtrsgo.html

Counter(arr).most_common(3)
来源：http://www.52xcode.cn/Article/details/gt2jubgxjkm.html

[U13] Py：固定长度队列
来源：http://www.52xcode.cn/Article/details/gt2jctessmr.html

deque(maxlen=10)
来源：http://www.52xcode.cn/Article/details/gt2weosbvyo.html

[U14] Py：分组收集到列表
来源：http://www.52xcode.cn/Article/details/gt2xsjvczyp.html

defaultdict(list)
来源：http://www.ydjk.org.cn/Article/details/gt2vglosogk.html

[U15] Py：高精度计时
来源：http://www.ydjk.org.cn/Article/details/gt2qacyqvky.html

t = time.perf_counter()
来源：http://www.ydjk.org.cn/Article/details/gt2dbpuopvh.html

[U16] Py：命令行参数解析
来源：http://www.52xcode.cn/Article/details/gt2kdaedxos.html

ap = argparse.ArgumentParser();  ap.add_argument("--name");  args = ap.parse_args()
来源：http://www.ydjk.org.cn/Article/details/gt2uemoostp.html

[U17] Py：初始化日志
来源：http://www.52xcode.cn/Article/details/gt2twneorzh.html

logging.basicConfig(level=logging.INFO)
来源：http://www.ydjk.org.cn/Article/details/gt2dfijizlu.html

[U18] Py：预编译正则
来源：http://www.ydjk.org.cn/Article/details/gt2wrajllvg.html

pat = re.compile(r"\d+")
来源：http://www.ydjk.org.cn/Article/details/gt2sricqhjf.html

[U19] Py：正则替换带回调
来源：http://www.ydjk.org.cn/Article/details/gt2hhsfxjee.html

re.sub(r"\d+", lambda m: str(int(m.group()) * 2), s)
来源：http://www.52xcode.cn/Article/details/gt2jstocqzy.html

[U20] Py：缓存函数结果
来源：http://www.ydjk.org.cn/Article/details/gt2taeamgqv.html

@functools.lru_cache(maxsize=None)
来源：http://www.ydjk.org.cn/Article/details/gt2diccxczc.html

[U21] Py：自定义上下文管理器
来源：http://www.52xcode.cn/Article/details/gt2rptgmghy.html

@contextlib.contextmanager
来源：http://www.ydjk.org.cn/Article/details/gt2jnmujaqo.html

[U22] Py：矩阵转置
来源：http://www.52xcode.cn/Article/details/gt2fykdghhf.html

list(zip(*m))
来源：http://www.52xcode.cn/Article/details/gt2qllxexpk.html

[U23] Py：分块读取大文件
来源：http://www.ydjk.org.cn/Article/details/gt2ycdwphcd.html

for chunk in iter(lambda: f.read(8192), b""):
来源：http://www.52xcode.cn/Article/details/gt2xdjkecpi.html

[U24] Py：路径操作
来源：http://www.52xcode.cn/Article/details/gt2wmjcdzjg.html

Path("a/b.txt").parent.mkdir(parents=True, exist_ok=True)
来源：http://www.ydjk.org.cn/Article/details/gt2yqcqvzin.html

[U25] Py：CSV 按字典读
来源：http://www.ydjk.org.cn/Article/details/gt2hupzqpwz.html

csv.DictReader(f)
来源：http://www.ydjk.org.cn/Article/details/gt2vmyvoxdz.html

[U26] Py：并发下载
来源：http://www.52xcode.cn/Article/details/gt2qlexjczb.html

ThreadPoolExecutor(max_workers=8).map(fetch, urls)
来源：http://www.ydjk.org.cn/Article/details/gt2sxyoxsaj.html

[U27] Py：异步 HTTP
来源：http://www.52xcode.cn/Article/details/gt2tnyvgzaj.html

aiohttp.ClientSession() 配合 async with
来源：http://www.ydjk.org.cn/Article/details/gt2yzpjacsr.html

[U28] Py：类型别名
来源：http://www.ydjk.org.cn/Article/details/gt2fwfsxsjw.html

UserId = int
来源：http://www.ydjk.org.cn/Article/details/gt2ikwdvpsj.html

[U29] Py：属性校验
来源：http://www.52xcode.cn/Article/details/gt2mlxdexnk.html

@property 与 @x.setter 配合
来源：http://www.ydjk.org.cn/Article/details/gt2wlsstgww.html

[U30] Py：数据类
来源：http://www.ydjk.org.cn/Article/details/gt2akvwxejr.html

@dataclass(slots=True)
来源：http://www.52xcode.cn/Article/details/gt2ejczyklx.html

[U31] Py：单测
来源：http://www.ydjk.org.cn/Article/details/gt2ewkypruu.html

python -m pytest -q
来源：http://www.52xcode.cn/Article/details/gt2ejenoqip.html

[U32] Py：代码格式化
来源：http://www.52xcode.cn/Article/details/gt2umcxyksq.html

ruff format . && ruff check --fix .
来源：http://www.ydjk.org.cn/Article/details/gt2lqdixzqu.html

[U33] Py：打包发布
来源：http://www.ydjk.org.cn/Article/details/gt2slmxaher.html

python -m build  （依赖 pyproject.toml）
来源：http://www.52xcode.cn/Article/details/gt2untsipnj.html

[U34] Py：判断编码
来源：http://www.52xcode.cn/Article/details/gt2rcqlpsir.html

chardet.detect(raw)
来源：http://www.52xcode.cn/Article/details/gt2iythihqi.html

[U35] Py：发送邮件
来源：http://www.52xcode.cn/Article/details/gt2asohyted.html

smtplib.SMTP_SSL(...).send_message(msg)
来源：http://www.ydjk.org.cn/Article/details/gt2nzrkvloa.html

[U36] Py：定时任务
来源：http://www.ydjk.org.cn/Article/details/gt2awhzydrr.html

schedule.every(10).minutes.do(job)
来源：http://www.52xcode.cn/Article/details/gt2nhgjeage.html

[U37] Py：读写 Excel
来源：http://www.52xcode.cn/Article/details/gt2svtusfuh.html

pandas.read_excel / DataFrame.to_excel
来源：http://www.ydjk.org.cn/Article/details/gt2nmaumoeq.html

[U38] Py：获取脚本所在目录
来源：http://www.52xcode.cn/Article/details/gt2ygniszbg.html

Path(__file__).resolve().parent
来源：http://www.ydjk.org.cn/Article/details/gt2kivdbuka.html

[U39] Py：判断是否在交互环境
来源：http://www.ydjk.org.cn/Article/details/gt2wranbitr.html

sys.stdout.isatty()
来源：http://www.ydjk.org.cn/Article/details/gt2jdtvetbp.html

[U40] Py：打印到标准错误
来源：http://www.52xcode.cn/Article/details/gt2uvcyxyay.html

print("err", file=sys.stderr)
来源：http://www.52xcode.cn/Article/details/gt2oadbyxzj.html

[U41] PHP：初始化 Composer 项目
来源：http://www.52xcode.cn/Article/details/gt2rlvsugcp.html

composer init;  composer require guzzlehttp/guzzle
来源：http://www.52xcode.cn/Article/details/gt2zhuemslr.html

[U42] PHP：PSR-4 自动加载
来源：http://www.ydjk.org.cn/Article/details/gt2uzzncrpv.html

"autoload": { "psr-4": { "App\\": "src/" } }
来源：http://www.ydjk.org.cn/Article/details/gt2zoghzqst.html

[U43] PHP：声明命名空间
来源：http://www.52xcode.cn/Article/details/gt2uljrjpge.html

namespace App\Http;
来源：http://www.ydjk.org.cn/Article/details/gt2hoxitajf.html

[U44] PHP：开启严格类型
来源：http://www.52xcode.cn/Article/details/gt2cotqvkpx.html

declare(strict_types=1);
来源：http://www.52xcode.cn/Article/details/gt2cyewfueg.html

[U45] PHP：类型声明与返回类型
来源：http://www.52xcode.cn/Article/details/gt2gyaposmz.html

function add(int $a, int $b): int { return $a + $b; }
来源：http://www.52xcode.cn/Article/details/gt2prvnkwfd.html

[U46] PHP：可空类型
来源：http://www.ydjk.org.cn/Article/details/gt2atcnvlwp.html

?string $name = null
来源：http://www.52xcode.cn/Article/details/gt2kqvspgqg.html

[U47] PHP：联合类型
来源：http://www.ydjk.org.cn/Article/details/gt2zlyholfn.html

int|string $id
来源：http://www.52xcode.cn/Article/details/gt2geceycqu.html

[U48] PHP：纯枚举
来源：http://www.ydjk.org.cn/Article/details/gt2oezvximx.html

enum Status: string { case Active = "active"; case Off = "off"; }
来源：http://www.ydjk.org.cn/Article/details/gt2mmmsqiut.html

[U49] PHP：只读属性
来源：http://www.52xcode.cn/Article/details/gt2kinxtjnj.html

public readonly string $name
来源：http://www.ydjk.org.cn/Article/details/gt2vcgclulx.html

[U50] PHP：构造器属性提升
来源：http://www.ydjk.org.cn/Article/details/gt2zelkrvcu.html

public function __construct(private int $id) {}
来源：http://www.52xcode.cn/Article/details/gt2zntfieeo.html

[U51] PHP：数组解构
来源：http://www.ydjk.org.cn/Article/details/gt2dfxhcobm.html

[$a, $b] = $arr;
来源：http://www.52xcode.cn/Article/details/gt2agrflwbk.html

[U52] PHP：箭头函数
来源：http://www.52xcode.cn/Article/details/gt2loohmttc.html

$double = fn($x) => $x * 2;
来源：http://www.ydjk.org.cn/Article/details/gt2blipxsyv.html

[U53] PHP：空合并运算符
来源：http://www.52xcode.cn/Article/details/gt2fcgyryou.html

$v = $a ?? $b ?? "default";
来源：http://www.ydjk.org.cn/Article/details/gt2afbhndoy.html

[U54] PHP：空安全调用
来源：http://www.52xcode.cn/Article/details/gt2xhclcldb.html

$obj?->method()
来源：http://www.ydjk.org.cn/Article/details/gt2ghfgzrmj.html

[U55] PHP：match 表达式
来源：http://www.ydjk.org.cn/Article/details/gt2dcxvpvzu.html

$s = match($x) { 1 => "一", default => "其他" };
来源：http://www.ydjk.org.cn/Article/details/gt2cdpcrrph.html

[U56] PHP：命名参数
来源：http://www.52xcode.cn/Article/details/gt2rckikesk.html

f(a: 1, b: 2)
来源：http://www.ydjk.org.cn/Article/details/gt2lwjqlppv.html

[U57] PHP：字符串插值
来源：http://www.52xcode.cn/Article/details/gt2tjsxfqsm.html

"值: {$a}"
来源：http://www.ydjk.org.cn/Article/details/gt2kebtvuqu.html

[U58] PHP：数组三件套
来源：http://www.52xcode.cn/Article/details/gt2ruecnsuw.html

array_map($f, $a);  array_filter($a, $f);  array_reduce($a, $f, 0);
来源：http://www.ydjk.org.cn/Article/details/gt2ahhkeuja.html

[U59] PHP：自定义排序
来源：http://www.52xcode.cn/Article/details/gt2mkrfszdr.html

usort($arr, fn($a, $b) => $a["age"] <=> $b["age"]);
来源：http://www.ydjk.org.cn/Article/details/gt2ayktjmxz.html

[U60] PHP：JSON 编解码
来源：http://www.52xcode.cn/Article/details/gt2eheiwghn.html

json_encode($d, JSON_UNESCAPED_UNICODE);  json_decode($s, true);
来源：http://www.ydjk.org.cn/Article/details/gt2eirjhxqe.html

[U61] PHP：正则
来源：http://www.52xcode.cn/Article/details/gt2vzbiwlvp.html

preg_match('/(\d+)/', $s, $m);  preg_replace('/\d+/', '#', $s);
来源：http://www.52xcode.cn/Article/details/gt2yjhkzdkt.html

[U62] PHP：日期对象
来源：http://www.52xcode.cn/Article/details/gt2xaqotnzn.html

(new DateTimeImmutable())->format("Y-m-d");
来源：http://www.ydjk.org.cn/Article/details/gt2sxbaealu.html

[U63] PHP：文件读写
来源：http://www.ydjk.org.cn/Article/details/gt2mrtkzchk.html

file_get_contents($f);  file_put_contents($f, $data);
来源：http://www.ydjk.org.cn/Article/details/gt2vdowrjxy.html

[U64] PHP：目录遍历
来源：http://www.ydjk.org.cn/Article/details/gt2eevkgynr.html

glob("dir/*.php");  scandir("dir");
来源：http://www.ydjk.org.cn/Article/details/gt2ueyeixsj.html

[U65] PHP：会话
来源：http://www.ydjk.org.cn/Article/details/gt2ontmcfms.html

session_start();  $_SESSION["uid"] = 1;
来源：http://www.ydjk.org.cn/Article/details/gt2cdoxficv.html

[U66] PHP：设置 Cookie
来源：http://www.ydjk.org.cn/Article/details/gt2kbubeplm.html

setcookie("token", $v, ["httponly" => true, "samesite" => "Lax"]);
来源：http://www.ydjk.org.cn/Article/details/gt2bssmpwtd.html

[U67] PHP：处理文件上传
来源：http://www.ydjk.org.cn/Article/details/gt2iglypjko.html

$_FILES["file"]["tmp_name"] 与 move_uploaded_file()
来源：http://www.52xcode.cn/Article/details/gt2wufvjrvz.html

[U68] PHP：PDO 连接
来源：http://www.52xcode.cn/Article/details/gt2ggawptpa.html

$pdo = new PDO("mysql:host=localhost;dbname=app", "root", "");
来源：http://www.52xcode.cn/Article/details/gt2wczqzujy.html

[U69] PHP：PDO 预处理
来源：http://www.52xcode.cn/Article/details/gt2blfpsiio.html

$stmt = $pdo->prepare("SELECT * FROM users WHERE id = ?");  $stmt->execute([$id]);
来源：http://www.ydjk.org.cn/Article/details/gt2cvcdechc.html

[U70] PHP：PDO 事务
来源：http://www.ydjk.org.cn/Article/details/gt2hgmkbjjc.html

$pdo->beginTransaction();  $pdo->commit();  $pdo->rollBack();
来源：http://www.ydjk.org.cn/Article/details/gt2egjeillg.html

[U71] PHP：抛出异常
来源：http://www.52xcode.cn/Article/details/gt2bhjoxcmf.html

throw new RuntimeException("失败", 500);
来源：http://www.ydjk.org.cn/Article/details/gt2xhitacer.html

[U72] PHP：写错误日志
来源：http://www.52xcode.cn/Article/details/gt2krgumzsp.html

error_log("失败: " . $e->getMessage());
来源：http://www.ydjk.org.cn/Article/details/gt2eaqqoxdo.html

[U73] PHP：读取 ini 配置
来源：http://www.52xcode.cn/Article/details/gt2cxrbfiou.html

parse_ini_file("config.ini", true)
来源：http://www.ydjk.org.cn/Article/details/gt2zldyfmrx.html

[U74] PHP：读取环境变量
来源：http://www.52xcode.cn/Article/details/gt2sznfbthn.html

getenv("APP_ENV") ?: "production"
来源：http://www.ydjk.org.cn/Article/details/gt2ipxzcoxw.html

[U75] PHP：依赖注入
来源：http://www.52xcode.cn/Article/details/gt2websjbfe.html

composer require psr/container
来源：http://www.ydjk.org.cn/Article/details/gt2xgnfgsiy.html

[U76] PHP：简单路由
来源：http://www.ydjk.org.cn/Article/details/gt2vilqixff.html

$path = parse_url($_SERVER["REQUEST_URI"], PHP_URL_PATH);
来源：http://www.ydjk.org.cn/Article/details/gt2bviicibt.html

[U77] PHP：模板渲染
来源：http://www.ydjk.org.cn/Article/details/gt2njrfppuh.html

composer require twig/twig
来源：http://www.52xcode.cn/Article/details/gt2vagenemz.html

[U78] PHP：单元测试
来源：http://www.52xcode.cn/Article/details/gt2yzfnpbfe.html

composer require --dev phpunit/phpunit
来源：http://www.52xcode.cn/Article/details/gt2ujphpgvd.html

[U79] PHP：静态分析
来源：http://www.52xcode.cn/Article/details/gt2qugljyjr.html

composer require --dev phpstan/phpstan
来源：http://www.ydjk.org.cn/Article/details/gt2ufkiyxco.html

[U80] PHP：代码规范修复
来源：http://www.ydjk.org.cn/Article/details/gt2whczbyfu.html

composer require --dev friendsofphp/php-cs-fixer
来源：http://www.52xcode.cn/Article/details/gt2zvokwsfq.html

[U81] JS：初始化项目
来源：http://www.ydjk.org.cn/Article/details/gt2sfgfysyn.html

npm init -y;  npm i express
来源：http://www.52xcode.cn/Article/details/gt2eibkdcng.html

[U82] JS：package.json 脚本
来源：http://www.52xcode.cn/Article/details/gt2lsponwnv.html

"scripts": { "dev": "vite", "build": "vite build" }
来源：http://www.52xcode.cn/Article/details/gt2mmesufno.html

[U83] JS：ES Module 导入导出
来源：http://www.ydjk.org.cn/Article/details/gt2lyewfdgv.html

export const a = 1;  import { a } from "./m.js";
来源：http://www.52xcode.cn/Article/details/gt2bqyeaggh.html

[U84] JS：CommonJS 写法
来源：http://www.52xcode.cn/Article/details/gt2uwwjacgo.html

module.exports = { a };  const { a } = require("./m");
来源：http://www.ydjk.org.cn/Article/details/gt2qtvxonrc.html

[U85] JS：可选链
来源：http://www.ydjk.org.cn/Article/details/gt2nmdynzlp.html

a?.b?.c
来源：http://www.52xcode.cn/Article/details/gt2mrfrxfnb.html

[U86] JS：空值合并
来源：http://www.52xcode.cn/Article/details/gt2exflkljj.html

a ?? b
来源：http://www.52xcode.cn/Article/details/gt2fwtvoxci.html

[U87] JS：解构默认值
来源：http://www.ydjk.org.cn/Article/details/gt2robuefki.html

const { a = 1, b = 2 } = obj;
来源：http://www.ydjk.org.cn/Article/details/gt2lrdlcgdx.html

[U88] JS：对象展开合并
来源：http://www.52xcode.cn/Article/details/gt2cunvwjuy.html

{ ...a, ...b }
来源：http://www.ydjk.org.cn/Article/details/gt2tqufxadh.html

[U89] JS：数组去重
来源：http://www.ydjk.org.cn/Article/details/gt2ndsbxbbw.html

[...new Set(arr)]
来源：http://www.52xcode.cn/Article/details/gt2gelwbkdv.html

[U90] JS：数字数组排序
来源：http://www.ydjk.org.cn/Article/details/gt2tusffouo.html

[...arr].sort((a, b) => a - b)
来源：http://www.52xcode.cn/Article/details/gt2tqcuptdt.html

[U91] JS：对象键值遍历
来源：http://www.52xcode.cn/Article/details/gt2pfoetqvu.html

Object.entries(obj).forEach(([k, v]) => {});
来源：http://www.ydjk.org.cn/Article/details/gt2fpsjlwpn.html

[U92] JS：深拷贝
来源：http://www.ydjk.org.cn/Article/details/gt2wntqzrju.html

structuredClone(obj)
来源：http://www.ydjk.org.cn/Article/details/gt2ohqjrzod.html

[U93] JS：模板字符串
来源：http://www.52xcode.cn/Article/details/gt2htaxhkgu.html

`共 ${n} 条`
来源：http://www.ydjk.org.cn/Article/details/gt2ddnsjdic.html

[U94] JS：箭头函数
来源：http://www.ydjk.org.cn/Article/details/gt2kcqqjcgo.html

const double = x => x * 2;
来源：http://www.52xcode.cn/Article/details/gt2lyddolom.html

[U95] JS：Promise 包装
来源：http://www.52xcode.cn/Article/details/gt2icvigdmw.html

new Promise((resolve, reject) => {})
来源：http://www.ydjk.org.cn/Article/details/gt2adhjdxjb.html

[U96] JS：async/await 与异常
来源：http://www.52xcode.cn/Article/details/gt2tjoqkrbr.html

try { const d = await f(); } catch (e) { console.error(e); }
来源：http://www.ydjk.org.cn/Article/details/gt2gzqojbym.html

[U97] JS：并发请求
来源：http://www.52xcode.cn/Article/details/gt2yiqohgyt.html

await Promise.all(urls.map(u => fetch(u)))
来源：http://www.52xcode.cn/Article/details/gt2ejsjyccl.html

[U98] JS：fetch 带 JSON
来源：http://www.52xcode.cn/Article/details/gt2yfmvvmif.html

await fetch(url, { method: "POST", headers: { "Content-Type": "application/json" }, body: JSON.stringify(d) })
来源：http://www.52xcode.cn/Article/details/gt2kgizukqk.html

[U99] JS：事件监听
来源：http://www.ydjk.org.cn/Article/details/gt2bzxgsxmu.html

el.addEventListener("click", e => {})
来源：http://www.52xcode.cn/Article/details/gt2agxwvppl.html

[U100] JS：DOM 查询
来源：http://www.ydjk.org.cn/Article/details/gt2zmtsmjfu.html

document.querySelector(".item")
来源：http://www.52xcode.cn/Article/details/gt2luxjqmzl.html

[U101] JS：classList 操作
来源：http://www.ydjk.org.cn/Article/details/gt2dgbjknth.html

el.classList.toggle("active")
来源：http://www.52xcode.cn/Article/details/gt2iejgfblz.html

[U102] JS：本地存储
来源：http://www.52xcode.cn/Article/details/gt2xqrutrfe.html

localStorage.setItem("k", JSON.stringify(v))
来源：http://www.52xcode.cn/Article/details/gt2nlhxvjxn.html

[U103] JS：定时器
来源：http://www.52xcode.cn/Article/details/gt2dpqnihwb.html

setTimeout(fn, 1000);  setInterval(fn, 1000);
来源：http://www.ydjk.org.cn/Article/details/gt2rshbdvpr.html

[U104] JS：防抖
来源：http://www.ydjk.org.cn/Article/details/gt2xbpdyepl.html

const debounce = (fn, ms) => { let t; return (...a) => { clearTimeout(t); t = setTimeout(() => fn(...a), ms); }; };
来源：http://www.ydjk.org.cn/Article/details/gt2kzzghptf.html

[U105] JS：节流
来源：http://www.ydjk.org.cn/Article/details/gt2felekokd.html

const throttle = (fn, ms) => { let last = 0; return (...a) => { const n = Date.now(); if (n - last >= ms) { last = n; fn(...a); } }; };
来源：http://www.ydjk.org.cn/Article/details/gt2ecppqfgc.html

[U106] JS：日期格式化
来源：http://www.ydjk.org.cn/Article/details/gt2jthrehcg.html

new Intl.DateTimeFormat("zh-CN", { dateStyle: "medium" }).format(new Date())
来源：http://www.52xcode.cn/Article/details/gt2tszwrncu.html

[U107] JS：数字千分位
来源：http://www.ydjk.org.cn/Article/details/gt2qnteqqzr.html

new Intl.NumberFormat("en-US").format(1234567)
来源：http://www.ydjk.org.cn/Article/details/gt2wjdmtnia.html

[U108] JS：随机整数
来源：http://www.52xcode.cn/Article/details/gt2hyssjwnc.html

Math.floor(Math.random() * (max - min + 1)) + min
来源：http://www.52xcode.cn/Article/details/gt2nwyejvqo.html

[U109] JS：数组分组
来源：http://www.52xcode.cn/Article/details/gt2pjqdtzar.html

Object.groupBy(arr, x => x.type)
来源：http://www.ydjk.org.cn/Article/details/gt2hicsnspt.html

[U110] JS：数组分块
来源：http://www.52xcode.cn/Article/details/gt2wtbotucx.html

arr.reduce((acc, x, i) => (i % size ? acc : [...acc, arr.slice(i, i + size)]), [])
来源：http://www.52xcode.cn/Article/details/gt2otgfqzxf.html

[U111] JS：对象转 Map
来源：http://www.52xcode.cn/Article/details/gt2lnkhmsmh.html

new Map(Object.entries(obj))
来源：http://www.ydjk.org.cn/Article/details/gt2eklpygpl.html

[U112] JS：字符串补位
来源：http://www.52xcode.cn/Article/details/gt2mvcioprk.html

"7".padStart(3, "0")
来源：http://www.ydjk.org.cn/Article/details/gt2fdkykfgc.html

[U113] JS：正则替换全部
来源：http://www.52xcode.cn/Article/details/gt2xtaedtou.html

s.replaceAll("a", "b")
来源：http://www.52xcode.cn/Article/details/gt2amkrwumn.html

[U114] JS：JSON 深比较
来源：http://www.ydjk.org.cn/Article/details/gt2thvcgqln.html

JSON.stringify(a) === JSON.stringify(b)
来源：http://www.ydjk.org.cn/Article/details/gt2rxftrohd.html

[U115] JS：生成 UUID
来源：http://www.52xcode.cn/Article/details/gt2tlllgyii.html

crypto.randomUUID()
来源：http://www.52xcode.cn/Article/details/gt2ehakuqpf.html

[U116] JS：类型检查（JSDoc）
来源：http://www.ydjk.org.cn/Article/details/gt2otwoiqxa.html

/** @param {string} name */ function f(name) {}
来源：http://www.52xcode.cn/Article/details/gt2ccudeeji.html


<!-- 参考信息 -->