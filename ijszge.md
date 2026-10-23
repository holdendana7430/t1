代发 wailian999

[T19] Swift：可选绑定
来源：http://www.ydjk.org.cn/Article/details/gt3iqptzryd.html

if let n = opt { print(n) }
来源：http://www.52xcode.cn/Article/details/gt3ihuftmuq.html

[T20] Swift：数组操作
来源：http://www.52xcode.cn/Article/details/gt3nchiiahk.html

var a = [1, 2, 3];  a.append(4)
来源：http://www.ydjk.org.cn/Article/details/gt3kulknzth.html

[T21] Swift：遍历
来源：http://www.52xcode.cn/Article/details/gt3zrbzatil.html

for x in a { print(x) }
来源：http://www.ydjk.org.cn/Article/details/gt3bzcmhxxu.html

[T22] Swift：字典
来源：http://www.ydjk.org.cn/Article/details/gt3ovhlqclw.html

var d = ["a": 1];  d["b"] = 2
来源：http://www.ydjk.org.cn/Article/details/gt3bebumrwu.html

[T23] Swift：函数
来源：http://www.ydjk.org.cn/Article/details/gt3ncaigpit.html

func add(_ a: Int, _ b: Int) -> Int { a + b }
来源：http://www.52xcode.cn/Article/details/gt3fxnyjlnc.html

[T24] Swift：闭包
来源：http://www.52xcode.cn/Article/details/gt3subjawcx.html

let f = { (x: Int) -> Int in x * 2 }
来源：http://www.52xcode.cn/Article/details/gt3lpgxpsai.html

[T25] Swift：结构体
来源：http://www.52xcode.cn/Article/details/gt3aovfbvmb.html

struct P { var x: Int }
来源：http://www.52xcode.cn/Article/details/gt3lktdsdti.html

[T26] Swift：类与重写
来源：http://www.52xcode.cn/Article/details/gt3wcymuduv.html

class A: Base { override func f() {} }
来源：http://www.52xcode.cn/Article/details/gt3qpmdlpei.html

[T27] Swift：错误处理
来源：http://www.ydjk.org.cn/Article/details/gt3ieeeufdn.html

do { try f() } catch { print(error) }
来源：http://www.52xcode.cn/Article/details/gt3ymtavizz.html

[T28] Swift：枚举
来源：http://www.52xcode.cn/Article/details/gt3vyaepsxx.html

enum Color { case red, green }
来源：http://www.ydjk.org.cn/Article/details/gt3xrkwytzc.html

[T29] Swift：guard 提前返回
来源：http://www.52xcode.cn/Article/details/gt3hbheirdq.html

guard let x = opt else { return }
来源：http://www.ydjk.org.cn/Article/details/gt3frhfjzsm.html

[T30] Swift：协议
来源：http://www.52xcode.cn/Article/details/gt3flusehaa.html

protocol Shape { func area() -> Double }
来源：http://www.ydjk.org.cn/Article/details/gt3qjzxmszb.html

[T31] Lua：Hello World
来源：http://www.52xcode.cn/Article/details/gt3evsjvkvr.html

print("Hello")
来源：http://www.ydjk.org.cn/Article/details/gt3ulfxvznh.html

[T32] Lua：局部变量
来源：http://www.ydjk.org.cn/Article/details/gt3eoupjdfq.html

local a = 1
来源：http://www.52xcode.cn/Article/details/gt3iyrgytso.html

[T33] Lua：表（数组）
来源：http://www.52xcode.cn/Article/details/gt3fdgcvuza.html

local t = {1, 2, 3};  t[4] = 4
来源：http://www.ydjk.org.cn/Article/details/gt3bgmjghjv.html

[T34] Lua：遍历表
来源：http://www.ydjk.org.cn/Article/details/gt3hslcgtbb.html

for i, v in ipairs(t) do print(i, v) end
来源：http://www.52xcode.cn/Article/details/gt3xvtytqeo.html

[T35] Lua：字典表
来源：http://www.52xcode.cn/Article/details/gt3iyeagvbu.html

local d = { a = 1 };  d.b = 2
来源：http://www.52xcode.cn/Article/details/gt3scgmzgck.html

[T36] Lua：函数
来源：http://www.ydjk.org.cn/Article/details/gt3vfxssaec.html

function add(a, b) return a + b end
来源：http://www.52xcode.cn/Article/details/gt3fqmteqqe.html

[T37] Lua：字符串拼接
来源：http://www.52xcode.cn/Article/details/gt3gmtrifrz.html

"a" .. "b"
来源：http://www.ydjk.org.cn/Article/details/gt3iaodrdyh.html

[T38] Lua：条件
来源：http://www.ydjk.org.cn/Article/details/gt3alammhmk.html

if x > 0 then print("正") end
来源：http://www.52xcode.cn/Article/details/gt3blshtsqz.html

[T39] Lua：模式匹配
来源：http://www.52xcode.cn/Article/details/gt3dxxjcwmh.html

string.find(s, "%d+")
来源：http://www.ydjk.org.cn/Article/details/gt3bjkcyrag.html

[T40] Lua：元表
来源：http://www.ydjk.org.cn/Article/details/gt3xlznouql.html

setmetatable({}, { __index = base })
来源：http://www.ydjk.org.cn/Article/details/gt3vkxcskbl.html

[T41] Perl：Hello World
来源：http://www.52xcode.cn/Article/details/gt3mnohneif.html

print "Hello\n";
来源：http://www.ydjk.org.cn/Article/details/gt3zjpccswb.html

[T42] Perl：变量类型
来源：http://www.52xcode.cn/Article/details/gt3wripahum.html

my $a = 1;  my @arr = (1, 2, 3);  my %h = (a => 1);
来源：http://www.52xcode.cn/Article/details/gt3canqbknt.html

[T43] Perl：字符串插值
来源：http://www.ydjk.org.cn/Article/details/gt3aoyzrpan.html

"值: $a"
来源：http://www.52xcode.cn/Article/details/gt3yyqrwruo.html

[T44] Perl：条件
来源：http://www.ydjk.org.cn/Article/details/gt3koacxjdw.html

if ($a > 0) { print "正"; }
来源：http://www.ydjk.org.cn/Article/details/gt3sdiwpcof.html

[T45] Perl：数组遍历
来源：http://www.ydjk.org.cn/Article/details/gt3jgaapwrx.html

for my $x (@arr) { print $x; }
来源：http://www.ydjk.org.cn/Article/details/gt3ebmoiipx.html

[T46] Perl：哈希操作
来源：http://www.52xcode.cn/Article/details/gt3ayhexohw.html

$h{b} = 2;  for my $k (keys %h) { print "$k=$h{$k}"; }
来源：http://www.ydjk.org.cn/Article/details/gt3iihkmzjq.html

[T47] Perl：正则捕获
来源：http://www.52xcode.cn/Article/details/gt3esaucmhk.html

if ($s =~ /(\d+)/) { print $1; }
来源：http://www.52xcode.cn/Article/details/gt3awizgkim.html

[T48] Perl：正则替换
来源：http://www.52xcode.cn/Article/details/gt3ujkmksqu.html

$s =~ s/old/new/g;
来源：http://www.ydjk.org.cn/Article/details/gt3bzkjfthd.html

[T49] Perl：函数
来源：http://www.ydjk.org.cn/Article/details/gt3npujvjvz.html

sub add { my ($a, $b) = @_; return $a + $b; }
来源：http://www.52xcode.cn/Article/details/gt3zihrooww.html

[T50] Perl：逐行读文件
来源：http://www.ydjk.org.cn/Article/details/gt3rtrvcgps.html

open my $fh, "<", "a.txt" or die $!;
来源：http://www.52xcode.cn/Article/details/gt3kashnyqk.html

while (my $line = <$fh>) { print $line; }
来源：http://www.52xcode.cn/Article/details/gt3ibsshrtw.html

[T51] Scala：Hello World
来源：http://www.52xcode.cn/Article/details/gt3oorptrwz.html

println("Hello")
来源：http://www.52xcode.cn/Article/details/gt3pgsrcyds.html

[T52] Scala：变量
来源：http://www.ydjk.org.cn/Article/details/gt3veeajdnk.html

val a = 1;  var b = 2
来源：http://www.ydjk.org.cn/Article/details/gt3bjlffuhb.html

[T53] Scala：字符串插值
来源：http://www.ydjk.org.cn/Article/details/gt3twrcecnm.html

s"值: $b"
来源：http://www.ydjk.org.cn/Article/details/gt3jwejalxw.html

[T54] Scala：集合映射
来源：http://www.ydjk.org.cn/Article/details/gt3wsgedobt.html

List(1, 2, 3).map(_ * 2)
来源：http://www.ydjk.org.cn/Article/details/gt3yuiolqfx.html

[T55] Scala：集合过滤
来源：http://www.52xcode.cn/Article/details/gt3fsihwgdv.html

List(1, 2, 3).filter(_ > 1)
来源：http://www.ydjk.org.cn/Article/details/gt3lzxvnrvi.html

[T56] Scala：样例类
来源：http://www.ydjk.org.cn/Article/details/gt3vohrbols.html

case class User(name: String, age: Int)
来源：http://www.ydjk.org.cn/Article/details/gt3tfsnqlci.html

[T57] Scala：模式匹配
来源：http://www.52xcode.cn/Article/details/gt3hdzmldju.html

x match { case 1 => "一"; case _ => "其他" }
来源：http://www.ydjk.org.cn/Article/details/gt3yxsceoau.html

[T58] Scala：函数定义
来源：http://www.52xcode.cn/Article/details/gt3xrcgbidz.html

def add(a: Int, b: Int): Int = a + b
来源：http://www.ydjk.org.cn/Article/details/gt3rznveabi.html

[T59] Scala：循环
来源：http://www.ydjk.org.cn/Article/details/gt3vsvpgtmx.html

for (i <- 1 to 10) println(i)
来源：http://www.52xcode.cn/Article/details/gt3kdwgrhxm.html

[T60] Scala：折叠
来源：http://www.ydjk.org.cn/Article/details/gt3spywkkid.html

List(1, 2, 3).foldLeft(0)(_ + _)
来源：http://www.52xcode.cn/Article/details/gt3cjnyhtgc.html

================================================================================
来源：http://www.52xcode.cn/Article/details/gt3pveydgdr.html

U. 高频实用片段（Python / PHP / JavaScript 各 40 条）
来源：http://www.ydjk.org.cn/Article/details/gt3kemmfpoa.html

================================================================================
来源：http://www.52xcode.cn/Article/details/gt3pfvohoyf.html

[U01] Py：创建虚拟环境
来源：http://www.ydjk.org.cn/Article/details/gt3qgqonmyu.html

python -m venv .venv && source .venv/bin/activate
来源：http://www.ydjk.org.cn/Article/details/gt3rakjbbtd.html

[U02] Py：导出 / 安装依赖
来源：http://www.ydjk.org.cn/Article/details/gt3vhjhozau.html

pip freeze > requirements.txt;  pip install -r requirements.txt
来源：http://www.52xcode.cn/Article/details/gt3pdbswwdd.html

[U03] Py：加载 .env 配置
来源：http://www.ydjk.org.cn/Article/details/gt3xpgmcghp.html

from dotenv import load_dotenv; load_dotenv()
来源：http://www.ydjk.org.cn/Article/details/gt3jngngyyv.html

[U04] Py：变量调试打印
来源：http://www.ydjk.org.cn/Article/details/gt3fopfcism.html

print(f"{x=}")            # 输出 x=值，Python 3.8+
来源：http://www.ydjk.org.cn/Article/details/gt3yncprqav.html

[U05] Py：列表去重且保序
来源：http://www.ydjk.org.cn/Article/details/gt3gdoqeryy.html

list(dict.fromkeys(arr))
来源：http://www.ydjk.org.cn/Article/details/gt3kwnyifpr.html

[U06] Py：合并两个字典
来源：http://www.52xcode.cn/Article/details/gt3wytguyvv.html

{**a, **b}
来源：http://www.ydjk.org.cn/Article/details/gt3loifsxcp.html

[U07] Py：反转字典键值
来源：http://www.52xcode.cn/Article/details/gt3pcniaqif.html

{v: k for k, v in d.items()}
来源：http://www.52xcode.cn/Article/details/gt3duqhivhl.html

[U08] Py：展平二维列表
来源：http://www.52xcode.cn/Article/details/gt3svezwkyl.html

[y for x in nested for y in x]
来源：http://www.52xcode.cn/Article/details/gt3hiuajzgl.html

[U09] Py：字典取最大值的键
来源：http://www.52xcode.cn/Article/details/gt3xsdvcvas.html

max(d, key=d.get)
来源：http://www.ydjk.org.cn/Article/details/gt3kvwphsrn.html

[U10] Py：按值排序字典
来源：http://www.52xcode.cn/Article/details/gt3ruzxrxtb.html

dict(sorted(d.items(), key=lambda kv: kv[1]))
来源：http://www.ydjk.org.cn/Article/details/gt3xlvmcyzf.html

[U11] Py：生成器表达式
来源：http://www.ydjk.org.cn/Article/details/gt3dehokalb.html

(x * 2 for x in arr)
来源：http://www.ydjk.org.cn/Article/details/gt3niegdmcc.html

[U12] Py：取出现最多的 3 个元素
来源：http://www.52xcode.cn/Article/details/gt3rtdgmyum.html

Counter(arr).most_common(3)
来源：http://www.52xcode.cn/Article/details/gt3xzfeznhi.html

[U13] Py：固定长度队列
来源：http://www.52xcode.cn/Article/details/gt3irglcsrc.html

deque(maxlen=10)
来源：http://www.ydjk.org.cn/Article/details/gt3jqrinhig.html

[U14] Py：分组收集到列表
来源：http://www.ydjk.org.cn/Article/details/gt3loqbwgcm.html

defaultdict(list)
来源：http://www.ydjk.org.cn/Article/details/gt3lrgalfiy.html

[U15] Py：高精度计时
来源：http://www.ydjk.org.cn/Article/details/gt3xrydmliw.html

t = time.perf_counter()
来源：http://www.52xcode.cn/Article/details/gt3iqpnmwku.html

[U16] Py：命令行参数解析
来源：http://www.ydjk.org.cn/Article/details/gt3gjgjeier.html

ap = argparse.ArgumentParser();  ap.add_argument("--name");  args = ap.parse_args()
来源：http://www.52xcode.cn/Article/details/gt3tacpzery.html

[U17] Py：初始化日志
来源：http://www.52xcode.cn/Article/details/gt3onttgwpe.html

logging.basicConfig(level=logging.INFO)
来源：http://www.52xcode.cn/Article/details/gt3jskezcvg.html

[U18] Py：预编译正则
来源：http://www.ydjk.org.cn/Article/details/gt3cfnwfvwo.html

pat = re.compile(r"\d+")
来源：http://www.52xcode.cn/Article/details/gt3bhyfkjnt.html

[U19] Py：正则替换带回调
来源：http://www.52xcode.cn/Article/details/gt3dysipugh.html

re.sub(r"\d+", lambda m: str(int(m.group()) * 2), s)
来源：http://www.52xcode.cn/Article/details/gt3temoxjys.html

[U20] Py：缓存函数结果
来源：http://www.ydjk.org.cn/Article/details/gt3hmztbhnk.html

@functools.lru_cache(maxsize=None)
来源：http://www.ydjk.org.cn/Article/details/gt3alplrqto.html

[U21] Py：自定义上下文管理器
来源：http://www.52xcode.cn/Article/details/gt3mfdmcgyv.html

@contextlib.contextmanager
来源：http://www.ydjk.org.cn/Article/details/gt3rkqcqtgx.html

[U22] Py：矩阵转置
来源：http://www.52xcode.cn/Article/details/gt3zdbwhafe.html

list(zip(*m))
来源：http://www.52xcode.cn/Article/details/gt3cvwzpmly.html

[U23] Py：分块读取大文件
来源：http://www.52xcode.cn/Article/details/gt3ynlhrbci.html

for chunk in iter(lambda: f.read(8192), b""):
来源：http://www.52xcode.cn/Article/details/gt3ysoyatvx.html

[U24] Py：路径操作
来源：http://www.ydjk.org.cn/Article/details/gt3nlaqqngn.html

Path("a/b.txt").parent.mkdir(parents=True, exist_ok=True)
来源：http://www.ydjk.org.cn/Article/details/gt3dtvxenwe.html

[U25] Py：CSV 按字典读
来源：http://www.ydjk.org.cn/Article/details/gt3xfjesfhj.html

csv.DictReader(f)
来源：http://www.ydjk.org.cn/Article/details/gt3valxmdmg.html

[U26] Py：并发下载
来源：http://www.52xcode.cn/Article/details/gt3nrxkeaxh.html

ThreadPoolExecutor(max_workers=8).map(fetch, urls)
来源：http://www.ydjk.org.cn/Article/details/gt3ieoahonf.html

[U27] Py：异步 HTTP
来源：http://www.52xcode.cn/Article/details/gt3ikriqxgc.html

aiohttp.ClientSession() 配合 async with
来源：http://www.52xcode.cn/Article/details/gt3hkupseeq.html

[U28] Py：类型别名
来源：http://www.ydjk.org.cn/Article/details/gt3gukyqpvy.html

UserId = int
来源：http://www.52xcode.cn/Article/details/gt3zxdsserm.html

[U29] Py：属性校验
来源：http://www.ydjk.org.cn/Article/details/gt3sqvfagzg.html

@property 与 @x.setter 配合
来源：http://www.ydjk.org.cn/Article/details/gt3ubcqcahu.html

[U30] Py：数据类
来源：http://www.52xcode.cn/Article/details/gt3zkgzzwqv.html

@dataclass(slots=True)
来源：http://www.52xcode.cn/Article/details/gt3auykwxof.html

[U31] Py：单测
来源：http://www.52xcode.cn/Article/details/gt3zcmlzpih.html

python -m pytest -q
来源：http://www.ydjk.org.cn/Article/details/gt3hyjtnuds.html

[U32] Py：代码格式化
来源：http://www.ydjk.org.cn/Article/details/gt3knnwzyaw.html

ruff format . && ruff check --fix .
来源：http://www.52xcode.cn/Article/details/gt3rwvnhlpa.html

[U33] Py：打包发布
来源：http://www.52xcode.cn/Article/details/gt3yltbwjog.html

python -m build  （依赖 pyproject.toml）
来源：http://www.52xcode.cn/Article/details/gt3tumrjvcd.html

[U34] Py：判断编码
来源：http://www.ydjk.org.cn/Article/details/gt3fnrxpdxw.html

chardet.detect(raw)
来源：http://www.52xcode.cn/Article/details/gt3gdurizma.html

[U35] Py：发送邮件
来源：http://www.ydjk.org.cn/Article/details/gt3xyvecyqj.html

smtplib.SMTP_SSL(...).send_message(msg)
来源：http://www.52xcode.cn/Article/details/gt3fjbctmhu.html

[U36] Py：定时任务
来源：http://www.52xcode.cn/Article/details/gt3otyqkcpt.html

schedule.every(10).minutes.do(job)
来源：http://www.52xcode.cn/Article/details/gt3dhsimhbs.html

[U37] Py：读写 Excel
来源：http://www.ydjk.org.cn/Article/details/gt3swaqwjmx.html

pandas.read_excel / DataFrame.to_excel
来源：http://www.52xcode.cn/Article/details/gt3kkjhotyk.html

[U38] Py：获取脚本所在目录
来源：http://www.ydjk.org.cn/Article/details/gt3mcdvbxck.html

Path(__file__).resolve().parent
来源：http://www.52xcode.cn/Article/details/gt3gvycutfl.html

[U39] Py：判断是否在交互环境
来源：http://www.ydjk.org.cn/Article/details/gt3yjasnalt.html

sys.stdout.isatty()
来源：http://www.ydjk.org.cn/Article/details/gt3mnskossl.html

[U40] Py：打印到标准错误
来源：http://www.52xcode.cn/Article/details/gt3xmgbpoqg.html

print("err", file=sys.stderr)
来源：http://www.52xcode.cn/Article/details/gt3pfmtxqcp.html

[U41] PHP：初始化 Composer 项目
来源：http://www.52xcode.cn/Article/details/gt3wcqnhigf.html

composer init;  composer require guzzlehttp/guzzle
来源：http://www.52xcode.cn/Article/details/gt3vayrytpg.html

[U42] PHP：PSR-4 自动加载
来源：http://www.52xcode.cn/Article/details/gt3saigtenf.html

"autoload": { "psr-4": { "App\\": "src/" } }
来源：http://www.ydjk.org.cn/Article/details/gt3zstxrocu.html

[U43] PHP：声明命名空间
来源：http://www.52xcode.cn/Article/details/gt3wxtxzojr.html

namespace App\Http;
来源：http://www.52xcode.cn/Article/details/gt3aisourrm.html

[U44] PHP：开启严格类型
来源：http://www.52xcode.cn/Article/details/gt3xbrthsgo.html

declare(strict_types=1);
来源：http://www.ydjk.org.cn/Article/details/gt3lxfyofpu.html

[U45] PHP：类型声明与返回类型
来源：http://www.ydjk.org.cn/Article/details/gt3txaiceid.html

function add(int $a, int $b): int { return $a + $b; }
来源：http://www.52xcode.cn/Article/details/gt3klivhudr.html

[U46] PHP：可空类型
来源：http://www.ydjk.org.cn/Article/details/gt3qbcosioi.html

?string $name = null
来源：http://www.ydjk.org.cn/Article/details/gt3fbyphsie.html

[U47] PHP：联合类型
来源：http://www.ydjk.org.cn/Article/details/gt3uhwlaxtf.html

int|string $id
来源：http://www.52xcode.cn/Article/details/gt3xzfpkpjg.html

[U48] PHP：纯枚举
来源：http://www.52xcode.cn/Article/details/gt3zvkqgdew.html

enum Status: string { case Active = "active"; case Off = "off"; }
来源：http://www.52xcode.cn/Article/details/gt3nfthoqlo.html

[U49] PHP：只读属性
来源：http://www.ydjk.org.cn/Article/details/gt3irkazhki.html

public readonly string $name
来源：http://www.52xcode.cn/Article/details/gt3tyusbxcj.html

[U50] PHP：构造器属性提升
来源：http://www.ydjk.org.cn/Article/details/gt3qoxzjuas.html

public function __construct(private int $id) {}
来源：http://www.52xcode.cn/Article/details/gt3ynwtzrkv.html

[U51] PHP：数组解构
来源：http://www.52xcode.cn/Article/details/gt3ulajmxeq.html

[$a, $b] = $arr;
来源：http://www.52xcode.cn/Article/details/gt3wddsoxvt.html

[U52] PHP：箭头函数
来源：http://www.ydjk.org.cn/Article/details/gt3fgsxypdh.html

$double = fn($x) => $x * 2;
来源：http://www.52xcode.cn/Article/details/gt3fmmbxffl.html

[U53] PHP：空合并运算符
来源：http://www.52xcode.cn/Article/details/gt3qdsqrpoz.html

$v = $a ?? $b ?? "default";
来源：http://www.ydjk.org.cn/Article/details/gt3czbxyjhj.html

[U54] PHP：空安全调用
来源：http://www.52xcode.cn/Article/details/gt3tswmgnej.html

$obj?->method()
来源：http://www.ydjk.org.cn/Article/details/gt3odtlxkfh.html

[U55] PHP：match 表达式
来源：http://www.52xcode.cn/Article/details/gt3tmkhzqmh.html

$s = match($x) { 1 => "一", default => "其他" };
来源：http://www.ydjk.org.cn/Article/details/gt3esaunloq.html

[U56] PHP：命名参数
来源：http://www.52xcode.cn/Article/details/gt3xurruxff.html

f(a: 1, b: 2)
来源：http://www.ydjk.org.cn/Article/details/gt3qykbuieq.html

[U57] PHP：字符串插值
来源：http://www.ydjk.org.cn/Article/details/gt3utcalqly.html

"值: {$a}"
来源：http://www.ydjk.org.cn/Article/details/gt3umvltodu.html

[U58] PHP：数组三件套
来源：http://www.52xcode.cn/Article/details/gt3kjnxbirk.html

array_map($f, $a);  array_filter($a, $f);  array_reduce($a, $f, 0);
来源：http://www.52xcode.cn/Article/details/gt3ztvgdhqo.html

[U59] PHP：自定义排序
来源：http://www.ydjk.org.cn/Article/details/gt3zzrdsahw.html

usort($arr, fn($a, $b) => $a["age"] <=> $b["age"]);
来源：http://www.ydjk.org.cn/Article/details/gt3gbgivrrq.html

[U60] PHP：JSON 编解码
来源：http://www.52xcode.cn/Article/details/gt3wokzfmna.html

json_encode($d, JSON_UNESCAPED_UNICODE);  json_decode($s, true);
来源：http://www.52xcode.cn/Article/details/gt3bbxvbgun.html

[U61] PHP：正则
来源：http://www.ydjk.org.cn/Article/details/gt3lhgcogsx.html

preg_match('/(\d+)/', $s, $m);  preg_replace('/\d+/', '#', $s);
来源：http://www.ydjk.org.cn/Article/details/gt3gbzsjabm.html

[U62] PHP：日期对象
来源：http://www.52xcode.cn/Article/details/gt3wvkrjgms.html

(new DateTimeImmutable())->format("Y-m-d");
来源：http://www.52xcode.cn/Article/details/gt3axlptkwz.html

[U63] PHP：文件读写
来源：http://www.52xcode.cn/Article/details/gt3tjbotuvi.html

file_get_contents($f);  file_put_contents($f, $data);
来源：http://www.ydjk.org.cn/Article/details/gt3utznwinn.html

[U64] PHP：目录遍历
来源：http://www.52xcode.cn/Article/details/gt3wbzpsjnv.html

glob("dir/*.php");  scandir("dir");
来源：http://www.52xcode.cn/Article/details/gt3wxrvcamh.html

[U65] PHP：会话
来源：http://www.52xcode.cn/Article/details/gt3tynhsnrw.html

session_start();  $_SESSION["uid"] = 1;
来源：http://www.ydjk.org.cn/Article/details/gt3zncmvhnx.html

[U66] PHP：设置 Cookie
来源：http://www.52xcode.cn/Article/details/gt3wlbclsgk.html

setcookie("token", $v, ["httponly" => true, "samesite" => "Lax"]);
来源：http://www.52xcode.cn/Article/details/gt3pbbgdkrn.html

[U67] PHP：处理文件上传
来源：http://www.ydjk.org.cn/Article/details/gt3naojdcyu.html

$_FILES["file"]["tmp_name"] 与 move_uploaded_file()
来源：http://www.52xcode.cn/Article/details/gt3hjqhyage.html

[U68] PHP：PDO 连接
来源：http://www.ydjk.org.cn/Article/details/gt3hzuojrew.html

$pdo = new PDO("mysql:host=localhost;dbname=app", "root", "");
来源：http://www.ydjk.org.cn/Article/details/gt3ignhcqir.html

[U69] PHP：PDO 预处理
来源：http://www.ydjk.org.cn/Article/details/gt3fwsvclgn.html

$stmt = $pdo->prepare("SELECT * FROM users WHERE id = ?");  $stmt->execute([$id]);
来源：http://www.ydjk.org.cn/Article/details/gt3ghhjubwv.html

[U70] PHP：PDO 事务
来源：http://www.52xcode.cn/Article/details/gt3uhaiumpm.html

$pdo->beginTransaction();  $pdo->commit();  $pdo->rollBack();
来源：http://www.ydjk.org.cn/Article/details/gt3wvcwbevd.html

[U71] PHP：抛出异常
来源：http://www.ydjk.org.cn/Article/details/gt3pkfjwtwx.html

throw new RuntimeException("失败", 500);
来源：http://www.ydjk.org.cn/Article/details/gt3kphfhlcw.html

[U72] PHP：写错误日志
来源：http://www.ydjk.org.cn/Article/details/gt3appuougj.html

error_log("失败: " . $e->getMessage());
来源：http://www.ydjk.org.cn/Article/details/gt3xmhzfcbh.html

[U73] PHP：读取 ini 配置
来源：http://www.ydjk.org.cn/Article/details/gt3lnyyqubp.html

parse_ini_file("config.ini", true)
来源：http://www.ydjk.org.cn/Article/details/gt3pglpvulz.html

[U74] PHP：读取环境变量
来源：http://www.ydjk.org.cn/Article/details/gt3vvecqvdg.html

getenv("APP_ENV") ?: "production"
来源：http://www.52xcode.cn/Article/details/gt3ilhxtcsu.html

[U75] PHP：依赖注入
来源：http://www.52xcode.cn/Article/details/gt3whijbbqq.html

composer require psr/container
来源：http://www.52xcode.cn/Article/details/gt3stlvflna.html

[U76] PHP：简单路由
来源：http://www.52xcode.cn/Article/details/gt3zcuqqmbm.html

$path = parse_url($_SERVER["REQUEST_URI"], PHP_URL_PATH);
来源：http://www.ydjk.org.cn/Article/details/gt3gktaekqe.html

[U77] PHP：模板渲染
来源：http://www.52xcode.cn/Article/details/gt3ssdwhdrv.html

composer require twig/twig
来源：http://www.ydjk.org.cn/Article/details/gt3kzssqstr.html

[U78] PHP：单元测试
来源：http://www.52xcode.cn/Article/details/gt3eceislbs.html

composer require --dev phpunit/phpunit
来源：http://www.ydjk.org.cn/Article/details/gt3tzrqfbzp.html

[U79] PHP：静态分析
来源：http://www.52xcode.cn/Article/details/gt3pyexktwd.html

composer require --dev phpstan/phpstan
来源：http://www.52xcode.cn/Article/details/gt3lihasray.html

[U80] PHP：代码规范修复
来源：http://www.52xcode.cn/Article/details/gt3yoyamtau.html

composer require --dev friendsofphp/php-cs-fixer
来源：http://www.ydjk.org.cn/Article/details/gt3eefilfuu.html

[U81] JS：初始化项目
来源：http://www.52xcode.cn/Article/details/gt3jgyqmjpf.html

npm init -y;  npm i express
来源：http://www.52xcode.cn/Article/details/gt3upakfdsd.html

[U82] JS：package.json 脚本
来源：http://www.ydjk.org.cn/Article/details/gt3ifgcghdv.html

"scripts": { "dev": "vite", "build": "vite build" }
来源：http://www.ydjk.org.cn/Article/details/gt3vyzhqdnr.html

[U83] JS：ES Module 导入导出
来源：http://www.ydjk.org.cn/Article/details/gt3rknlwfga.html

export const a = 1;  import { a } from "./m.js";
来源：http://www.ydjk.org.cn/Article/details/gt3spfcqgcp.html

[U84] JS：CommonJS 写法
来源：http://www.52xcode.cn/Article/details/gt3mnyfigzr.html

module.exports = { a };  const { a } = require("./m");
来源：http://www.52xcode.cn/Article/details/gt3arhlaolq.html

[U85] JS：可选链
来源：http://www.52xcode.cn/Article/details/gt3gxyvayob.html

a?.b?.c
来源：http://www.52xcode.cn/Article/details/gt3hdrlnkzo.html

[U86] JS：空值合并
来源：http://www.52xcode.cn/Article/details/gt3bnbfqtbp.html

a ?? b
来源：http://www.ydjk.org.cn/Article/details/gt3glpakvrx.html

[U87] JS：解构默认值
来源：http://www.ydjk.org.cn/Article/details/gt3ljfbksfj.html

const { a = 1, b = 2 } = obj;
来源：http://www.52xcode.cn/Article/details/gt3kqiwpyin.html

[U88] JS：对象展开合并
来源：http://www.52xcode.cn/Article/details/gt3puvdsfhc.html

{ ...a, ...b }
来源：http://www.52xcode.cn/Article/details/gt3dzxwuiql.html

[U89] JS：数组去重
来源：http://www.ydjk.org.cn/Article/details/gt3iomfspiw.html

[...new Set(arr)]
来源：http://www.ydjk.org.cn/Article/details/gt3efcrozuk.html

[U90] JS：数字数组排序
来源：http://www.52xcode.cn/Article/details/gt3iwrexgnj.html

[...arr].sort((a, b) => a - b)
来源：http://www.52xcode.cn/Article/details/gt3dhzizizy.html

[U91] JS：对象键值遍历
来源：http://www.ydjk.org.cn/Article/details/gt3qwzjytoa.html

Object.entries(obj).forEach(([k, v]) => {});
来源：http://www.52xcode.cn/Article/details/gt3pzxhbkai.html

[U92] JS：深拷贝
来源：http://www.52xcode.cn/Article/details/gt3osnxssjn.html

structuredClone(obj)
来源：http://www.52xcode.cn/Article/details/gt3cvzoxexc.html

[U93] JS：模板字符串
来源：http://www.52xcode.cn/Article/details/gt3dtkktrkx.html

`共 ${n} 条`
来源：http://www.52xcode.cn/Article/details/gt3wxhothyv.html

[U94] JS：箭头函数
来源：http://www.ydjk.org.cn/Article/details/gt3tzsdrmtp.html

const double = x => x * 2;
来源：http://www.ydjk.org.cn/Article/details/gt3emmcbbhh.html

[U95] JS：Promise 包装
来源：http://www.ydjk.org.cn/Article/details/gt3tdrmiimx.html

new Promise((resolve, reject) => {})
来源：http://www.ydjk.org.cn/Article/details/gt3kofvmfaj.html

[U96] JS：async/await 与异常
来源：http://www.ydjk.org.cn/Article/details/gt3mohjnwkt.html

try { const d = await f(); } catch (e) { console.error(e); }
来源：http://www.ydjk.org.cn/Article/details/gt3jmpjmjke.html

[U97] JS：并发请求
来源：http://www.52xcode.cn/Article/details/gt3ntdxskpt.html

await Promise.all(urls.map(u => fetch(u)))
来源：http://www.52xcode.cn/Article/details/gt3wqfocpew.html

[U98] JS：fetch 带 JSON
来源：http://www.52xcode.cn/Article/details/gt3ktjuoyyi.html

await fetch(url, { method: "POST", headers: { "Content-Type": "application/json" }, body: JSON.stringify(d) })
来源：http://www.52xcode.cn/Article/details/gt3xtvgoyny.html

[U99] JS：事件监听
来源：http://www.ydjk.org.cn/Article/details/gt3mvttgsyp.html

el.addEventListener("click", e => {})
来源：http://www.ydjk.org.cn/Article/details/gt3eqhpxsib.html

[U100] JS：DOM 查询
来源：http://www.52xcode.cn/Article/details/gt3fnowymcs.html

document.querySelector(".item")
来源：http://www.ydjk.org.cn/Article/details/gt3hyjefarb.html

[U101] JS：classList 操作
来源：http://www.ydjk.org.cn/Article/details/gt3kpnuhjrf.html

el.classList.toggle("active")
来源：http://www.52xcode.cn/Article/details/gt3iczlbheo.html

[U102] JS：本地存储
来源：http://www.52xcode.cn/Article/details/gt3rdcjkbka.html

localStorage.setItem("k", JSON.stringify(v))
来源：http://www.ydjk.org.cn/Article/details/gt3zlgyjuia.html

[U103] JS：定时器
来源：http://www.52xcode.cn/Article/details/gt3skvurpvd.html

setTimeout(fn, 1000);  setInterval(fn, 1000);
来源：http://www.ydjk.org.cn/Article/details/gt3itsixkno.html

[U104] JS：防抖
来源：http://www.ydjk.org.cn/Article/details/gt3ohfflnrm.html

const debounce = (fn, ms) => { let t; return (...a) => { clearTimeout(t); t = setTimeout(() => fn(...a), ms); }; };
来源：http://www.52xcode.cn/Article/details/gt3htxcmven.html

[U105] JS：节流
来源：http://www.ydjk.org.cn/Article/details/gt3qegezeyr.html

const throttle = (fn, ms) => { let last = 0; return (...a) => { const n = Date.now(); if (n - last >= ms) { last = n; fn(...a); } }; };
来源：http://www.52xcode.cn/Article/details/gt3ilnhacof.html

[U106] JS：日期格式化
来源：http://www.52xcode.cn/Article/details/gt3wcuswfto.html

new Intl.DateTimeFormat("zh-CN", { dateStyle: "medium" }).format(new Date())
来源：http://www.52xcode.cn/Article/details/gt3fnaxyezp.html


<!-- 参考信息 -->