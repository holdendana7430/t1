代发 wailian999

[T29] Swift：guard 提前返回
来源：http://www.ydjk.org.cn/Article/details/gt2humymjjc.html

guard let x = opt else { return }
来源：http://www.52xcode.cn/Article/details/gt2fvehjggc.html

[T30] Swift：协议
来源：http://www.52xcode.cn/Article/details/gt2pxzvjrsc.html

protocol Shape { func area() -> Double }
来源：http://www.ydjk.org.cn/Article/details/gt2grsefqbv.html

[T31] Lua：Hello World
来源：http://www.52xcode.cn/Article/details/gt2xeurexmc.html

print("Hello")
来源：http://www.ydjk.org.cn/Article/details/gt2qzquxqdd.html

[T32] Lua：局部变量
来源：http://www.ydjk.org.cn/Article/details/gt2ecjtkiif.html

local a = 1
来源：http://www.52xcode.cn/Article/details/gt2tgwnmzyo.html

[T33] Lua：表（数组）
来源：http://www.52xcode.cn/Article/details/gt2mjilafwc.html

local t = {1, 2, 3};  t[4] = 4
来源：http://www.ydjk.org.cn/Article/details/gt2usvocusw.html

[T34] Lua：遍历表
来源：http://www.52xcode.cn/Article/details/gt2ldsxzsdx.html

for i, v in ipairs(t) do print(i, v) end
来源：http://www.52xcode.cn/Article/details/gt2ufbomoud.html

[T35] Lua：字典表
来源：http://www.ydjk.org.cn/Article/details/gt2lodvsbff.html

local d = { a = 1 };  d.b = 2
来源：http://www.ydjk.org.cn/Article/details/gt2speqktde.html

[T36] Lua：函数
来源：http://www.ydjk.org.cn/Article/details/gt2oifkcmee.html

function add(a, b) return a + b end
来源：http://www.ydjk.org.cn/Article/details/gt2aejpisnf.html

[T37] Lua：字符串拼接
来源：http://www.52xcode.cn/Article/details/gt2gygcrfyy.html

"a" .. "b"
来源：http://www.52xcode.cn/Article/details/gt2rvquxied.html

[T38] Lua：条件
来源：http://www.52xcode.cn/Article/details/gt2mutknntg.html

if x > 0 then print("正") end
来源：http://www.52xcode.cn/Article/details/gt2erseedoi.html

[T39] Lua：模式匹配
来源：http://www.ydjk.org.cn/Article/details/gt2svuotzty.html

string.find(s, "%d+")
来源：http://www.ydjk.org.cn/Article/details/gt2yqkixyde.html

[T40] Lua：元表
来源：http://www.ydjk.org.cn/Article/details/gt2sauruanp.html

setmetatable({}, { __index = base })
来源：http://www.ydjk.org.cn/Article/details/gt2vakjnxpo.html

[T41] Perl：Hello World
来源：http://www.52xcode.cn/Article/details/gt2uqqfzhye.html

print "Hello\n";
来源：http://www.ydjk.org.cn/Article/details/gt2ngpfmsll.html

[T42] Perl：变量类型
来源：http://www.ydjk.org.cn/Article/details/gt2dgsifsmu.html

my $a = 1;  my @arr = (1, 2, 3);  my %h = (a => 1);
来源：http://www.52xcode.cn/Article/details/gt2ljrpeajb.html

[T43] Perl：字符串插值
来源：http://www.ydjk.org.cn/Article/details/gt2mwzmeiyf.html

"值: $a"
来源：http://www.ydjk.org.cn/Article/details/gt2mnlpzrks.html

[T44] Perl：条件
来源：http://www.ydjk.org.cn/Article/details/gt2gjsyhdna.html

if ($a > 0) { print "正"; }
来源：http://www.52xcode.cn/Article/details/gt2ylpmensz.html

[T45] Perl：数组遍历
来源：http://www.52xcode.cn/Article/details/gt2ewtheqrb.html

for my $x (@arr) { print $x; }
来源：http://www.ydjk.org.cn/Article/details/gt2rtugbinr.html

[T46] Perl：哈希操作
来源：http://www.ydjk.org.cn/Article/details/gt2owcbfsim.html

$h{b} = 2;  for my $k (keys %h) { print "$k=$h{$k}"; }
来源：http://www.ydjk.org.cn/Article/details/gt2cxzvnzau.html

[T47] Perl：正则捕获
来源：http://www.52xcode.cn/Article/details/gt2pgarkymn.html

if ($s =~ /(\d+)/) { print $1; }
来源：http://www.52xcode.cn/Article/details/gt2shnskcly.html

[T48] Perl：正则替换
来源：http://www.ydjk.org.cn/Article/details/gt2jkeyjexp.html

$s =~ s/old/new/g;
来源：http://www.52xcode.cn/Article/details/gt2mixwiums.html

[T49] Perl：函数
来源：http://www.ydjk.org.cn/Article/details/gt2itbtxhow.html

sub add { my ($a, $b) = @_; return $a + $b; }
来源：http://www.ydjk.org.cn/Article/details/gt2bltneztc.html

[T50] Perl：逐行读文件
来源：http://www.52xcode.cn/Article/details/gt2jyfabaya.html

open my $fh, "<", "a.txt" or die $!;
来源：http://www.52xcode.cn/Article/details/gt2nofxtyjn.html

while (my $line = <$fh>) { print $line; }
来源：http://www.52xcode.cn/Article/details/gt2dagzlqow.html

[T51] Scala：Hello World
来源：http://www.52xcode.cn/Article/details/gt2ibjtvrbc.html

println("Hello")
来源：http://www.52xcode.cn/Article/details/gt2eioduxjr.html

[T52] Scala：变量
来源：http://www.52xcode.cn/Article/details/gt2nawgebwy.html

val a = 1;  var b = 2
来源：http://www.ydjk.org.cn/Article/details/gt2yltmfdus.html

[T53] Scala：字符串插值
来源：http://www.ydjk.org.cn/Article/details/gt2noivfmhz.html

s"值: $b"
来源：http://www.52xcode.cn/Article/details/gt2lrypjvlk.html

[T54] Scala：集合映射
来源：http://www.52xcode.cn/Article/details/gt2khrqporo.html

List(1, 2, 3).map(_ * 2)
来源：http://www.52xcode.cn/Article/details/gt2uxxyezzm.html

[T55] Scala：集合过滤
来源：http://www.ydjk.org.cn/Article/details/gt2fibtonlq.html

List(1, 2, 3).filter(_ > 1)
来源：http://www.ydjk.org.cn/Article/details/gt2yogefvbl.html

[T56] Scala：样例类
来源：http://www.52xcode.cn/Article/details/gt2sgqolewm.html

case class User(name: String, age: Int)
来源：http://www.ydjk.org.cn/Article/details/gt2dlbzxbfz.html

[T57] Scala：模式匹配
来源：http://www.ydjk.org.cn/Article/details/gt2ephdncnj.html

x match { case 1 => "一"; case _ => "其他" }
来源：http://www.ydjk.org.cn/Article/details/gt2gzplbviv.html

[T58] Scala：函数定义
来源：http://www.ydjk.org.cn/Article/details/gt2rmqpcmvq.html

def add(a: Int, b: Int): Int = a + b
来源：http://www.52xcode.cn/Article/details/gt2fpiaygno.html

[T59] Scala：循环
来源：http://www.ydjk.org.cn/Article/details/gt2rgbpmgyi.html

for (i <- 1 to 10) println(i)
来源：http://www.ydjk.org.cn/Article/details/gt2gkmlrqpj.html

[T60] Scala：折叠
来源：http://www.ydjk.org.cn/Article/details/gt2ehbhidwp.html

List(1, 2, 3).foldLeft(0)(_ + _)
来源：http://www.52xcode.cn/Article/details/gt2whdwpsik.html

================================================================================
来源：http://www.52xcode.cn/Article/details/gt2sglxbaqo.html

U. 高频实用片段（Python / PHP / JavaScript 各 40 条）
来源：http://www.52xcode.cn/Article/details/gt2hnemxpjd.html

================================================================================
来源：http://www.52xcode.cn/Article/details/gt2mdeqtszf.html

[U01] Py：创建虚拟环境
来源：http://www.ydjk.org.cn/Article/details/gt2srnwbxlw.html

python -m venv .venv && source .venv/bin/activate
来源：http://www.ydjk.org.cn/Article/details/gt2jhctqemz.html

[U02] Py：导出 / 安装依赖
来源：http://www.ydjk.org.cn/Article/details/gt2nlckvwsb.html

pip freeze > requirements.txt;  pip install -r requirements.txt
来源：http://www.ydjk.org.cn/Article/details/gt2lrkemhvw.html

[U03] Py：加载 .env 配置
来源：http://www.ydjk.org.cn/Article/details/gt2khnxmrki.html

from dotenv import load_dotenv; load_dotenv()
来源：http://www.52xcode.cn/Article/details/gt2sijxnniq.html

[U04] Py：变量调试打印
来源：http://www.ydjk.org.cn/Article/details/gt2jgswtzcc.html

print(f"{x=}")            # 输出 x=值，Python 3.8+
来源：http://www.52xcode.cn/Article/details/gt2ifqvpxea.html

[U05] Py：列表去重且保序
来源：http://www.52xcode.cn/Article/details/gt2wfhgbwws.html

list(dict.fromkeys(arr))
来源：http://www.ydjk.org.cn/Article/details/gt2tevgvkvq.html

[U06] Py：合并两个字典
来源：http://www.52xcode.cn/Article/details/gt2gyxtjntf.html

{**a, **b}
来源：http://www.ydjk.org.cn/Article/details/gt2yxrcdbyw.html

[U07] Py：反转字典键值
来源：http://www.ydjk.org.cn/Article/details/gt2pgyjekdn.html

{v: k for k, v in d.items()}
来源：http://www.52xcode.cn/Article/details/gt2cjprocaw.html

[U08] Py：展平二维列表
来源：http://www.52xcode.cn/Article/details/gt2jliikwmj.html

[y for x in nested for y in x]
来源：http://www.ydjk.org.cn/Article/details/gt2dzvzgwes.html

[U09] Py：字典取最大值的键
来源：http://www.ydjk.org.cn/Article/details/gt2njtqqywv.html

max(d, key=d.get)
来源：http://www.52xcode.cn/Article/details/gt2icokeakn.html

[U10] Py：按值排序字典
来源：http://www.ydjk.org.cn/Article/details/gt2qcpgxeno.html

dict(sorted(d.items(), key=lambda kv: kv[1]))
来源：http://www.52xcode.cn/Article/details/gt2jnzwhbwo.html

[U11] Py：生成器表达式
来源：http://www.ydjk.org.cn/Article/details/gt2zihvnccp.html

(x * 2 for x in arr)
来源：http://www.ydjk.org.cn/Article/details/gt2vhgykogf.html

[U12] Py：取出现最多的 3 个元素
来源：http://www.52xcode.cn/Article/details/gt2mxknxajk.html

Counter(arr).most_common(3)
来源：http://www.ydjk.org.cn/Article/details/gt2golqcwyp.html

[U13] Py：固定长度队列
来源：http://www.ydjk.org.cn/Article/details/gt2fqvlrqca.html

deque(maxlen=10)
来源：http://www.52xcode.cn/Article/details/gt2umlrkpkz.html

[U14] Py：分组收集到列表
来源：http://www.52xcode.cn/Article/details/gt2yrjbocai.html

defaultdict(list)
来源：http://www.52xcode.cn/Article/details/gt2qxkxvbev.html

[U15] Py：高精度计时
来源：http://www.52xcode.cn/Article/details/gt2fskrmnxg.html

t = time.perf_counter()
来源：http://www.ydjk.org.cn/Article/details/gt2yprevgjz.html

[U16] Py：命令行参数解析
来源：http://www.ydjk.org.cn/Article/details/gt2nhadmqkt.html

ap = argparse.ArgumentParser();  ap.add_argument("--name");  args = ap.parse_args()
来源：http://www.52xcode.cn/Article/details/gt2vbhxylnp.html

[U17] Py：初始化日志
来源：http://www.52xcode.cn/Article/details/gt2pflscjdm.html

logging.basicConfig(level=logging.INFO)
来源：http://www.ydjk.org.cn/Article/details/gt2vxpbhqke.html

[U18] Py：预编译正则
来源：http://www.ydjk.org.cn/Article/details/gt2uyzuqxkx.html

pat = re.compile(r"\d+")
来源：http://www.52xcode.cn/Article/details/gt2nqkzunyp.html

[U19] Py：正则替换带回调
来源：http://www.ydjk.org.cn/Article/details/gt2cccqixfb.html

re.sub(r"\d+", lambda m: str(int(m.group()) * 2), s)
来源：http://www.ydjk.org.cn/Article/details/gt2ztbeltbh.html

[U20] Py：缓存函数结果
来源：http://www.ydjk.org.cn/Article/details/gt2wwbilvga.html

@functools.lru_cache(maxsize=None)
来源：http://www.52xcode.cn/Article/details/gt2vjdewtbe.html

[U21] Py：自定义上下文管理器
来源：http://www.52xcode.cn/Article/details/gt2tqkahunm.html

@contextlib.contextmanager
来源：http://www.ydjk.org.cn/Article/details/gt2gvfcgspn.html

[U22] Py：矩阵转置
来源：http://www.52xcode.cn/Article/details/gt2vqelzznh.html

list(zip(*m))
来源：http://www.52xcode.cn/Article/details/gt2xehmbmnl.html

[U23] Py：分块读取大文件
来源：http://www.ydjk.org.cn/Article/details/gt2iyfexsoc.html

for chunk in iter(lambda: f.read(8192), b""):
来源：http://www.52xcode.cn/Article/details/gt2hshopola.html

[U24] Py：路径操作
来源：http://www.ydjk.org.cn/Article/details/gt2rutxurdh.html

Path("a/b.txt").parent.mkdir(parents=True, exist_ok=True)
来源：http://www.ydjk.org.cn/Article/details/gt2zilwsfcq.html

[U25] Py：CSV 按字典读
来源：http://www.ydjk.org.cn/Article/details/gt2fpaznkby.html

csv.DictReader(f)
来源：http://www.ydjk.org.cn/Article/details/gt2dnybylqy.html

[U26] Py：并发下载
来源：http://www.ydjk.org.cn/Article/details/gt2hbrzjxrt.html

ThreadPoolExecutor(max_workers=8).map(fetch, urls)
来源：http://www.ydjk.org.cn/Article/details/gt2gzftkted.html

[U27] Py：异步 HTTP
来源：http://www.ydjk.org.cn/Article/details/gt2srxkmcpy.html

aiohttp.ClientSession() 配合 async with
来源：http://www.52xcode.cn/Article/details/gt2ogfoilay.html

[U28] Py：类型别名
来源：http://www.52xcode.cn/Article/details/gt2cvldfllp.html

UserId = int
来源：http://www.52xcode.cn/Article/details/gt2ymqsmayt.html

[U29] Py：属性校验
来源：http://www.52xcode.cn/Article/details/gt2zmqzalcj.html

@property 与 @x.setter 配合
来源：http://www.ydjk.org.cn/Article/details/gt2juntdlpv.html

[U30] Py：数据类
来源：http://www.52xcode.cn/Article/details/gt2jegwpdta.html

@dataclass(slots=True)
来源：http://www.52xcode.cn/Article/details/gt2rzgubmwh.html

[U31] Py：单测
来源：http://www.52xcode.cn/Article/details/gt2wqtocuux.html

python -m pytest -q
来源：http://www.ydjk.org.cn/Article/details/gt2xwaplnrz.html

[U32] Py：代码格式化
来源：http://www.52xcode.cn/Article/details/gt2wghhmerr.html

ruff format . && ruff check --fix .
来源：http://www.52xcode.cn/Article/details/gt2pquykvba.html

[U33] Py：打包发布
来源：http://www.ydjk.org.cn/Article/details/gt2bpvmdmld.html

python -m build  （依赖 pyproject.toml）
来源：http://www.52xcode.cn/Article/details/gt2ykjglgux.html

[U34] Py：判断编码
来源：http://www.ydjk.org.cn/Article/details/gt2wczvuygr.html

chardet.detect(raw)
来源：http://www.52xcode.cn/Article/details/gt2hqoeuzyj.html

[U35] Py：发送邮件
来源：http://www.ydjk.org.cn/Article/details/gt2edgbbkib.html

smtplib.SMTP_SSL(...).send_message(msg)
来源：http://www.52xcode.cn/Article/details/gt2zwzhxmti.html

[U36] Py：定时任务
来源：http://www.ydjk.org.cn/Article/details/gt2ouldwacp.html

schedule.every(10).minutes.do(job)
来源：http://www.52xcode.cn/Article/details/gt2evjozunz.html

[U37] Py：读写 Excel
来源：http://www.ydjk.org.cn/Article/details/gt2ectduqbs.html

pandas.read_excel / DataFrame.to_excel
来源：http://www.ydjk.org.cn/Article/details/gt2dpzpbkbs.html

[U38] Py：获取脚本所在目录
来源：http://www.52xcode.cn/Article/details/gt2aqejmorn.html

Path(__file__).resolve().parent
来源：http://www.ydjk.org.cn/Article/details/gt2ucfmxrny.html

[U39] Py：判断是否在交互环境
来源：http://www.ydjk.org.cn/Article/details/gt2uhkpbemz.html

sys.stdout.isatty()
来源：http://www.ydjk.org.cn/Article/details/gt2yptegolh.html

[U40] Py：打印到标准错误
来源：http://www.52xcode.cn/Article/details/gt2arnozjmf.html

print("err", file=sys.stderr)
来源：http://www.52xcode.cn/Article/details/gt2htgdlxdr.html

[U41] PHP：初始化 Composer 项目
来源：http://www.52xcode.cn/Article/details/gt2nuwajvzy.html

composer init;  composer require guzzlehttp/guzzle
来源：http://www.ydjk.org.cn/Article/details/gt2bffqgdti.html

[U42] PHP：PSR-4 自动加载
来源：http://www.ydjk.org.cn/Article/details/gt2ludebouq.html

"autoload": { "psr-4": { "App\\": "src/" } }
来源：http://www.52xcode.cn/Article/details/gt2jxfevayc.html

[U43] PHP：声明命名空间
来源：http://www.52xcode.cn/Article/details/gt2ldyoprzi.html

namespace App\Http;
来源：http://www.52xcode.cn/Article/details/gt2evapzpac.html

[U44] PHP：开启严格类型
来源：http://www.52xcode.cn/Article/details/gt2oaywtudb.html

declare(strict_types=1);
来源：http://www.52xcode.cn/Article/details/gt2fhrgvifn.html

[U45] PHP：类型声明与返回类型
来源：http://www.52xcode.cn/Article/details/gt2gnkgegxi.html

function add(int $a, int $b): int { return $a + $b; }
来源：http://www.52xcode.cn/Article/details/gt2oxboilvb.html

[U46] PHP：可空类型
来源：http://www.ydjk.org.cn/Article/details/gt2bhhcmkjy.html

?string $name = null
来源：http://www.ydjk.org.cn/Article/details/gt2fqcmuxyi.html

[U47] PHP：联合类型
来源：http://www.ydjk.org.cn/Article/details/gt2rwncazyv.html

int|string $id
来源：http://www.ydjk.org.cn/Article/details/gt2rldhnxlj.html

[U48] PHP：纯枚举
来源：http://www.52xcode.cn/Article/details/gt2gpokkdmt.html

enum Status: string { case Active = "active"; case Off = "off"; }
来源：http://www.52xcode.cn/Article/details/gt2sfcmvyea.html

[U49] PHP：只读属性
来源：http://www.ydjk.org.cn/Article/details/gt2hvdszhko.html

public readonly string $name
来源：http://www.52xcode.cn/Article/details/gt2hcrodiwt.html

[U50] PHP：构造器属性提升
来源：http://www.ydjk.org.cn/Article/details/gt2wbazfiex.html

public function __construct(private int $id) {}
来源：http://www.52xcode.cn/Article/details/gt2xjzrjhom.html

[U51] PHP：数组解构
来源：http://www.52xcode.cn/Article/details/gt2dcsmeicb.html

[$a, $b] = $arr;
来源：http://www.52xcode.cn/Article/details/gt2ckjusdkl.html

[U52] PHP：箭头函数
来源：http://www.ydjk.org.cn/Article/details/gt2rdvtmrce.html

$double = fn($x) => $x * 2;
来源：http://www.52xcode.cn/Article/details/gt2xgiemguc.html

[U53] PHP：空合并运算符
来源：http://www.ydjk.org.cn/Article/details/gt2ngcljeew.html

$v = $a ?? $b ?? "default";
来源：http://www.ydjk.org.cn/Article/details/gt2gjivxhvd.html

[U54] PHP：空安全调用
来源：http://www.ydjk.org.cn/Article/details/gt2birfntmz.html

$obj?->method()
来源：http://www.ydjk.org.cn/Article/details/gt2xkkizpgd.html

[U55] PHP：match 表达式
来源：http://www.52xcode.cn/Article/details/gt2xfblnqwg.html

$s = match($x) { 1 => "一", default => "其他" };
来源：http://www.52xcode.cn/Article/details/gt2yaechwow.html

[U56] PHP：命名参数
来源：http://www.52xcode.cn/Article/details/gt2fcxcawfi.html

f(a: 1, b: 2)
来源：http://www.52xcode.cn/Article/details/gt2vjdurceh.html

[U57] PHP：字符串插值
来源：http://www.ydjk.org.cn/Article/details/gt2oxnnvela.html

"值: {$a}"
来源：http://www.ydjk.org.cn/Article/details/gt2ouristin.html

[U58] PHP：数组三件套
来源：http://www.ydjk.org.cn/Article/details/gt2wbqfqbym.html

array_map($f, $a);  array_filter($a, $f);  array_reduce($a, $f, 0);
来源：http://www.ydjk.org.cn/Article/details/gt2bohoithu.html

[U59] PHP：自定义排序
来源：http://www.ydjk.org.cn/Article/details/gt2lnjslpli.html

usort($arr, fn($a, $b) => $a["age"] <=> $b["age"]);
来源：http://www.ydjk.org.cn/Article/details/gt2aktjdodj.html

[U60] PHP：JSON 编解码
来源：http://www.ydjk.org.cn/Article/details/gt2nfhrpwmr.html

json_encode($d, JSON_UNESCAPED_UNICODE);  json_decode($s, true);
来源：http://www.ydjk.org.cn/Article/details/gt2ntpnhnxv.html

[U61] PHP：正则
来源：http://www.52xcode.cn/Article/details/gt2bkhtrobv.html

preg_match('/(\d+)/', $s, $m);  preg_replace('/\d+/', '#', $s);
来源：http://www.ydjk.org.cn/Article/details/gt2ozlxyizk.html

[U62] PHP：日期对象
来源：http://www.52xcode.cn/Article/details/gt2vmmleuso.html

(new DateTimeImmutable())->format("Y-m-d");
来源：http://www.ydjk.org.cn/Article/details/gt2ibnwykqh.html

[U63] PHP：文件读写
来源：http://www.ydjk.org.cn/Article/details/gt2vxzakgwj.html

file_get_contents($f);  file_put_contents($f, $data);
来源：http://www.52xcode.cn/Article/details/gt2asdtwgpi.html

[U64] PHP：目录遍历
来源：http://www.ydjk.org.cn/Article/details/gt2guzmgach.html

glob("dir/*.php");  scandir("dir");
来源：http://www.ydjk.org.cn/Article/details/gt2hoorsznh.html

[U65] PHP：会话
来源：http://www.52xcode.cn/Article/details/gt2jqhdpbut.html

session_start();  $_SESSION["uid"] = 1;
来源：http://www.ydjk.org.cn/Article/details/gt2mmmfqvds.html

[U66] PHP：设置 Cookie
来源：http://www.52xcode.cn/Article/details/gt2bvkcmhwh.html

setcookie("token", $v, ["httponly" => true, "samesite" => "Lax"]);
来源：http://www.52xcode.cn/Article/details/gt2izeouzny.html

[U67] PHP：处理文件上传
来源：http://www.ydjk.org.cn/Article/details/gt2ncofdgke.html

$_FILES["file"]["tmp_name"] 与 move_uploaded_file()
来源：http://www.52xcode.cn/Article/details/gt2bseereca.html

[U68] PHP：PDO 连接
来源：http://www.52xcode.cn/Article/details/gt2gxnagajr.html

$pdo = new PDO("mysql:host=localhost;dbname=app", "root", "");
来源：http://www.52xcode.cn/Article/details/gt2emqrxsyf.html

[U69] PHP：PDO 预处理
来源：http://www.ydjk.org.cn/Article/details/gt2ueqzrwtw.html

$stmt = $pdo->prepare("SELECT * FROM users WHERE id = ?");  $stmt->execute([$id]);
来源：http://www.ydjk.org.cn/Article/details/gt2rrrvphlx.html

[U70] PHP：PDO 事务
来源：http://www.ydjk.org.cn/Article/details/gt2slwczjsu.html

$pdo->beginTransaction();  $pdo->commit();  $pdo->rollBack();
来源：http://www.ydjk.org.cn/Article/details/gt2rkhthiny.html

[U71] PHP：抛出异常
来源：http://www.ydjk.org.cn/Article/details/gt2njsyhzzo.html

throw new RuntimeException("失败", 500);
来源：http://www.52xcode.cn/Article/details/gt2hwgqewpl.html

[U72] PHP：写错误日志
来源：http://www.52xcode.cn/Article/details/gt2knwpfurf.html

error_log("失败: " . $e->getMessage());
来源：http://www.ydjk.org.cn/Article/details/gt2swgsjoab.html

[U73] PHP：读取 ini 配置
来源：http://www.52xcode.cn/Article/details/gt2fqpghjlf.html

parse_ini_file("config.ini", true)
来源：http://www.ydjk.org.cn/Article/details/gt2kqdxlscr.html

[U74] PHP：读取环境变量
来源：http://www.52xcode.cn/Article/details/gt2qubmehxa.html

getenv("APP_ENV") ?: "production"
来源：http://www.52xcode.cn/Article/details/gt2fdnwvzza.html

[U75] PHP：依赖注入
来源：http://www.52xcode.cn/Article/details/gt2itbzcpus.html

composer require psr/container
来源：http://www.ydjk.org.cn/Article/details/gt2sszsddhm.html

[U76] PHP：简单路由
来源：http://www.ydjk.org.cn/Article/details/gt2hunewutl.html

$path = parse_url($_SERVER["REQUEST_URI"], PHP_URL_PATH);
来源：http://www.52xcode.cn/Article/details/gt2crdepadw.html

[U77] PHP：模板渲染
来源：http://www.ydjk.org.cn/Article/details/gt2hdkdaibl.html

composer require twig/twig
来源：http://www.52xcode.cn/Article/details/gt2sccbiufl.html

[U78] PHP：单元测试
来源：http://www.ydjk.org.cn/Article/details/gt2vbdglgrc.html

composer require --dev phpunit/phpunit
来源：http://www.52xcode.cn/Article/details/gt2pzwesolj.html

[U79] PHP：静态分析
来源：http://www.52xcode.cn/Article/details/gt2auvkomvx.html

composer require --dev phpstan/phpstan
来源：http://www.ydjk.org.cn/Article/details/gt2luednkkw.html

[U80] PHP：代码规范修复
来源：http://www.ydjk.org.cn/Article/details/gt2wywzlqed.html

composer require --dev friendsofphp/php-cs-fixer
来源：http://www.ydjk.org.cn/Article/details/gt2aujeaqxh.html

[U81] JS：初始化项目
来源：http://www.52xcode.cn/Article/details/gt2estomasr.html

npm init -y;  npm i express
来源：http://www.ydjk.org.cn/Article/details/gt2cjhqrtoz.html

[U82] JS：package.json 脚本
来源：http://www.52xcode.cn/Article/details/gt2nikqkgwi.html

"scripts": { "dev": "vite", "build": "vite build" }
来源：http://www.ydjk.org.cn/Article/details/gt2ddcjtlrp.html

[U83] JS：ES Module 导入导出
来源：http://www.52xcode.cn/Article/details/gt2daugrjfx.html

export const a = 1;  import { a } from "./m.js";
来源：http://www.52xcode.cn/Article/details/gt2tslyzqtf.html

[U84] JS：CommonJS 写法
来源：http://www.52xcode.cn/Article/details/gt2qrfttsqy.html

module.exports = { a };  const { a } = require("./m");
来源：http://www.52xcode.cn/Article/details/gt2pwmxzjdj.html

[U85] JS：可选链
来源：http://www.52xcode.cn/Article/details/gt2jocvyjrs.html

a?.b?.c
来源：http://www.52xcode.cn/Article/details/gt2tlfehkkv.html

[U86] JS：空值合并
来源：http://www.52xcode.cn/Article/details/gt2iphzlmtn.html

a ?? b
来源：http://www.ydjk.org.cn/Article/details/gt2biahznqp.html

[U87] JS：解构默认值
来源：http://www.52xcode.cn/Article/details/gt2ehzoqcvi.html

const { a = 1, b = 2 } = obj;
来源：http://www.ydjk.org.cn/Article/details/gt2xzfmejut.html

[U88] JS：对象展开合并
来源：http://www.ydjk.org.cn/Article/details/gt2wfqazggb.html

{ ...a, ...b }
来源：http://www.ydjk.org.cn/Article/details/gt2dyankdsf.html

[U89] JS：数组去重
来源：http://www.ydjk.org.cn/Article/details/gt2jliodwiy.html

[...new Set(arr)]
来源：http://www.52xcode.cn/Article/details/gt2xcathmef.html

[U90] JS：数字数组排序
来源：http://www.ydjk.org.cn/Article/details/gt2kxxnfqvl.html

[...arr].sort((a, b) => a - b)
来源：http://www.ydjk.org.cn/Article/details/gt2ywlotecg.html

[U91] JS：对象键值遍历
来源：http://www.52xcode.cn/Article/details/gt2dxybtyed.html

Object.entries(obj).forEach(([k, v]) => {});
来源：http://www.ydjk.org.cn/Article/details/gt2dbncwjrz.html

[U92] JS：深拷贝
来源：http://www.52xcode.cn/Article/details/gt2dgxmxlqj.html

structuredClone(obj)
来源：http://www.ydjk.org.cn/Article/details/gt2lmdtilsn.html

[U93] JS：模板字符串
来源：http://www.52xcode.cn/Article/details/gt2lgiphvhw.html

`共 ${n} 条`
来源：http://www.ydjk.org.cn/Article/details/gt2atjvhnij.html

[U94] JS：箭头函数
来源：http://www.52xcode.cn/Article/details/gt2unvqfefh.html

const double = x => x * 2;
来源：http://www.ydjk.org.cn/Article/details/gt2fhvnbufy.html

[U95] JS：Promise 包装
来源：http://www.ydjk.org.cn/Article/details/gt2vofjaqcf.html

new Promise((resolve, reject) => {})
来源：http://www.52xcode.cn/Article/details/gt2obohcgpp.html

[U96] JS：async/await 与异常
来源：http://www.52xcode.cn/Article/details/gt2yfdzttjq.html

try { const d = await f(); } catch (e) { console.error(e); }
来源：http://www.ydjk.org.cn/Article/details/gt2cwqjagpe.html

[U97] JS：并发请求
来源：http://www.ydjk.org.cn/Article/details/gt2hgrdekcd.html

await Promise.all(urls.map(u => fetch(u)))
来源：http://www.52xcode.cn/Article/details/gt2fqzddsln.html

[U98] JS：fetch 带 JSON
来源：http://www.52xcode.cn/Article/details/gt2jpesvsvu.html

await fetch(url, { method: "POST", headers: { "Content-Type": "application/json" }, body: JSON.stringify(d) })
来源：http://www.ydjk.org.cn/Article/details/gt2sraxolkm.html

[U99] JS：事件监听
来源：http://www.ydjk.org.cn/Article/details/gt2jqkuwslh.html

el.addEventListener("click", e => {})
来源：http://www.ydjk.org.cn/Article/details/gt2fndrycqu.html

[U100] JS：DOM 查询
来源：http://www.52xcode.cn/Article/details/gt2pgfntemm.html

document.querySelector(".item")
来源：http://www.52xcode.cn/Article/details/gt2tskbabnf.html

[U101] JS：classList 操作
来源：http://www.52xcode.cn/Article/details/gt2wiqvgbig.html

el.classList.toggle("active")
来源：http://www.ydjk.org.cn/Article/details/gt2llxfoncy.html

[U102] JS：本地存储
来源：http://www.52xcode.cn/Article/details/gt2gveglnjf.html

localStorage.setItem("k", JSON.stringify(v))
来源：http://www.52xcode.cn/Article/details/gt2rixeyscm.html

[U103] JS：定时器
来源：http://www.52xcode.cn/Article/details/gt2uqrfgbqu.html

setTimeout(fn, 1000);  setInterval(fn, 1000);
来源：http://www.52xcode.cn/Article/details/gt2witborzf.html

[U104] JS：防抖
来源：http://www.ydjk.org.cn/Article/details/gt2hwgevqtn.html

const debounce = (fn, ms) => { let t; return (...a) => { clearTimeout(t); t = setTimeout(() => fn(...a), ms); }; };
来源：http://www.52xcode.cn/Article/details/gt2mkeswjvc.html

[U105] JS：节流
来源：http://www.ydjk.org.cn/Article/details/gt2wewltyra.html

const throttle = (fn, ms) => { let last = 0; return (...a) => { const n = Date.now(); if (n - last >= ms) { last = n; fn(...a); } }; };
来源：http://www.52xcode.cn/Article/details/gt2dghxqtux.html

[U106] JS：日期格式化
来源：http://www.ydjk.org.cn/Article/details/gt2gczsbjbm.html

new Intl.DateTimeFormat("zh-CN", { dateStyle: "medium" }).format(new Date())
来源：http://www.ydjk.org.cn/Article/details/gt2wzrttlwo.html

[U107] JS：数字千分位
来源：http://www.52xcode.cn/Article/details/gt2zrwminmw.html

new Intl.NumberFormat("en-US").format(1234567)
来源：http://www.52xcode.cn/Article/details/gt2smurghyt.html

[U108] JS：随机整数
来源：http://www.ydjk.org.cn/Article/details/gt2crdzxrnw.html

Math.floor(Math.random() * (max - min + 1)) + min
来源：http://www.52xcode.cn/Article/details/gt2hrbdujgj.html

[U109] JS：数组分组
来源：http://www.ydjk.org.cn/Article/details/gt2bziqqzlu.html

Object.groupBy(arr, x => x.type)
来源：http://www.52xcode.cn/Article/details/gt2cuqxhoso.html

[U110] JS：数组分块
来源：http://www.52xcode.cn/Article/details/gt2ptjwiplz.html

arr.reduce((acc, x, i) => (i % size ? acc : [...acc, arr.slice(i, i + size)]), [])
来源：http://www.52xcode.cn/Article/details/gt2xanllnhl.html

[U111] JS：对象转 Map
来源：http://www.ydjk.org.cn/Article/details/gt2ordjxptl.html

new Map(Object.entries(obj))
来源：http://www.ydjk.org.cn/Article/details/gt2fqxxuibz.html

[U112] JS：字符串补位
来源：http://www.ydjk.org.cn/Article/details/gt2zegnnabe.html

"7".padStart(3, "0")
来源：http://www.52xcode.cn/Article/details/gt2ammucdmk.html

[U113] JS：正则替换全部
来源：http://www.52xcode.cn/Article/details/gt2eucwazid.html

s.replaceAll("a", "b")
来源：http://www.52xcode.cn/Article/details/gt2joemznpk.html

[U114] JS：JSON 深比较
来源：http://www.52xcode.cn/Article/details/gt2czvyitmk.html

JSON.stringify(a) === JSON.stringify(b)
来源：http://www.52xcode.cn/Article/details/gt2xqikrlfd.html

[U115] JS：生成 UUID
来源：http://www.52xcode.cn/Article/details/gt2hdwivnbw.html

crypto.randomUUID()
来源：http://www.52xcode.cn/Article/details/gt2yktlppli.html

[U116] JS：类型检查（JSDoc）
来源：http://www.52xcode.cn/Article/details/gt2nwjecesh.html

/** @param {string} name */ function f(name) {}
来源：http://www.ydjk.org.cn/Article/details/gt2oisaihbr.html


<!-- 参考信息 -->