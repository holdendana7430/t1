代发 wailian999

[T21] Swift：遍历
来源：http://www.52xcode.cn/Article/details/gt3ybspemjz.html

for x in a { print(x) }
来源：http://www.52xcode.cn/Article/details/gt3fhjgvwce.html

[T22] Swift：字典
来源：http://www.ydjk.org.cn/Article/details/gt3ostkluld.html

var d = ["a": 1];  d["b"] = 2
来源：http://www.ydjk.org.cn/Article/details/gt3cuzmfmzv.html

[T23] Swift：函数
来源：http://www.52xcode.cn/Article/details/gt3ferykdjs.html

func add(_ a: Int, _ b: Int) -> Int { a + b }
来源：http://www.ydjk.org.cn/Article/details/gt3dbnvpkkn.html

[T24] Swift：闭包
来源：http://www.ydjk.org.cn/Article/details/gt3yaykdidj.html

let f = { (x: Int) -> Int in x * 2 }
来源：http://www.52xcode.cn/Article/details/gt3addwrdyo.html

[T25] Swift：结构体
来源：http://www.52xcode.cn/Article/details/gt3lknnocts.html

struct P { var x: Int }
来源：http://www.ydjk.org.cn/Article/details/gt3smmszhav.html

[T26] Swift：类与重写
来源：http://www.ydjk.org.cn/Article/details/gt3qocsodbd.html

class A: Base { override func f() {} }
来源：http://www.52xcode.cn/Article/details/gt3pkovkqiu.html

[T27] Swift：错误处理
来源：http://www.52xcode.cn/Article/details/gt3elopgtuv.html

do { try f() } catch { print(error) }
来源：http://www.52xcode.cn/Article/details/gt3rghwpdvf.html

[T28] Swift：枚举
来源：http://www.52xcode.cn/Article/details/gt3kroaatha.html

enum Color { case red, green }
来源：http://www.52xcode.cn/Article/details/gt3jeivyewo.html

[T29] Swift：guard 提前返回
来源：http://www.ydjk.org.cn/Article/details/gt3uvzvwnca.html

guard let x = opt else { return }
来源：http://www.ydjk.org.cn/Article/details/gt3pgbblraj.html

[T30] Swift：协议
来源：http://www.52xcode.cn/Article/details/gt3ajcbvhkv.html

protocol Shape { func area() -> Double }
来源：http://www.ydjk.org.cn/Article/details/gt3vaghhvck.html

[T31] Lua：Hello World
来源：http://www.52xcode.cn/Article/details/gt3inlfbmfz.html

print("Hello")
来源：http://www.52xcode.cn/Article/details/gt3ofbfhtwf.html

[T32] Lua：局部变量
来源：http://www.ydjk.org.cn/Article/details/gt3mkdfswco.html

local a = 1
来源：http://www.52xcode.cn/Article/details/gt3kyjxtgqu.html

[T33] Lua：表（数组）
来源：http://www.52xcode.cn/Article/details/gt3qfrwojer.html

local t = {1, 2, 3};  t[4] = 4
来源：http://www.52xcode.cn/Article/details/gt3lniehkrh.html

[T34] Lua：遍历表
来源：http://www.52xcode.cn/Article/details/gt3bgylccph.html

for i, v in ipairs(t) do print(i, v) end
来源：http://www.52xcode.cn/Article/details/gt3judgckkf.html

[T35] Lua：字典表
来源：http://www.ydjk.org.cn/Article/details/gt3ocjlsfnh.html

local d = { a = 1 };  d.b = 2
来源：http://www.ydjk.org.cn/Article/details/gt3odoxuosx.html

[T36] Lua：函数
来源：http://www.ydjk.org.cn/Article/details/gt3uhgolzhp.html

function add(a, b) return a + b end
来源：http://www.ydjk.org.cn/Article/details/gt3eyawkjsp.html

[T37] Lua：字符串拼接
来源：http://www.52xcode.cn/Article/details/gt3ewrrgimh.html

"a" .. "b"
来源：http://www.52xcode.cn/Article/details/gt3ctofdotp.html

[T38] Lua：条件
来源：http://www.52xcode.cn/Article/details/gt3crebktmz.html

if x > 0 then print("正") end
来源：http://www.ydjk.org.cn/Article/details/gt3tzmshkeo.html

[T39] Lua：模式匹配
来源：http://www.52xcode.cn/Article/details/gt3bioldlbn.html

string.find(s, "%d+")
来源：http://www.ydjk.org.cn/Article/details/gt3decflfez.html

[T40] Lua：元表
来源：http://www.ydjk.org.cn/Article/details/gt3mzzebsvl.html

setmetatable({}, { __index = base })
来源：http://www.ydjk.org.cn/Article/details/gt3xboxxcrq.html

[T41] Perl：Hello World
来源：http://www.52xcode.cn/Article/details/gt3ptsdmend.html

print "Hello\n";
来源：http://www.52xcode.cn/Article/details/gt3rghrdilt.html

[T42] Perl：变量类型
来源：http://www.ydjk.org.cn/Article/details/gt3qzzdwhka.html

my $a = 1;  my @arr = (1, 2, 3);  my %h = (a => 1);
来源：http://www.ydjk.org.cn/Article/details/gt3cexvaulo.html

[T43] Perl：字符串插值
来源：http://www.52xcode.cn/Article/details/gt3olusairw.html

"值: $a"
来源：http://www.ydjk.org.cn/Article/details/gt3rcpksjmn.html

[T44] Perl：条件
来源：http://www.ydjk.org.cn/Article/details/gt3avozjihx.html

if ($a > 0) { print "正"; }
来源：http://www.52xcode.cn/Article/details/gt3jedljjrz.html

[T45] Perl：数组遍历
来源：http://www.52xcode.cn/Article/details/gt3ekxikblq.html

for my $x (@arr) { print $x; }
来源：http://www.ydjk.org.cn/Article/details/gt3vbsxixhw.html

[T46] Perl：哈希操作
来源：http://www.52xcode.cn/Article/details/gt3dfkmping.html

$h{b} = 2;  for my $k (keys %h) { print "$k=$h{$k}"; }
来源：http://www.ydjk.org.cn/Article/details/gt3ukuspyzb.html

[T47] Perl：正则捕获
来源：http://www.ydjk.org.cn/Article/details/gt3wsgjxyhq.html

if ($s =~ /(\d+)/) { print $1; }
来源：http://www.ydjk.org.cn/Article/details/gt3nvmfoynj.html

[T48] Perl：正则替换
来源：http://www.52xcode.cn/Article/details/gt3kdemmebw.html

$s =~ s/old/new/g;
来源：http://www.ydjk.org.cn/Article/details/gt3citptmvo.html

[T49] Perl：函数
来源：http://www.ydjk.org.cn/Article/details/gt3alzqymow.html

sub add { my ($a, $b) = @_; return $a + $b; }
来源：http://www.52xcode.cn/Article/details/gt3omcvixqf.html

[T50] Perl：逐行读文件
来源：http://www.ydjk.org.cn/Article/details/gt3vgyhebhd.html

open my $fh, "<", "a.txt" or die $!;
来源：http://www.52xcode.cn/Article/details/gt3gfzabfok.html

while (my $line = <$fh>) { print $line; }
来源：http://www.52xcode.cn/Article/details/gt3sywdosyv.html

[T51] Scala：Hello World
来源：http://www.52xcode.cn/Article/details/gt3coebnsmi.html

println("Hello")
来源：http://www.52xcode.cn/Article/details/gt3rmpojlfm.html

[T52] Scala：变量
来源：http://www.52xcode.cn/Article/details/gt3jzzodtso.html

val a = 1;  var b = 2
来源：http://www.52xcode.cn/Article/details/gt3kvfigavj.html

[T53] Scala：字符串插值
来源：http://www.ydjk.org.cn/Article/details/gt3gbotibgg.html

s"值: $b"
来源：http://www.52xcode.cn/Article/details/gt3ipegakpf.html

[T54] Scala：集合映射
来源：http://www.ydjk.org.cn/Article/details/gt3vwkdialn.html

List(1, 2, 3).map(_ * 2)
来源：http://www.ydjk.org.cn/Article/details/gt3xmljvpvw.html

[T55] Scala：集合过滤
来源：http://www.ydjk.org.cn/Article/details/gt3hzbsnvmh.html

List(1, 2, 3).filter(_ > 1)
来源：http://www.52xcode.cn/Article/details/gt3ltlvgchp.html

[T56] Scala：样例类
来源：http://www.52xcode.cn/Article/details/gt3kyjuulcs.html

case class User(name: String, age: Int)
来源：http://www.52xcode.cn/Article/details/gt3awdhrrsn.html

[T57] Scala：模式匹配
来源：http://www.52xcode.cn/Article/details/gt3tuffggpr.html

x match { case 1 => "一"; case _ => "其他" }
来源：http://www.52xcode.cn/Article/details/gt3znpmbgsc.html

[T58] Scala：函数定义
来源：http://www.ydjk.org.cn/Article/details/gt3bomyysfx.html

def add(a: Int, b: Int): Int = a + b
来源：http://www.ydjk.org.cn/Article/details/gt3wtaubaol.html

[T59] Scala：循环
来源：http://www.ydjk.org.cn/Article/details/gt3ksalmikz.html

for (i <- 1 to 10) println(i)
来源：http://www.52xcode.cn/Article/details/gt3umludytc.html

[T60] Scala：折叠
来源：http://www.ydjk.org.cn/Article/details/gt3rehnelst.html

List(1, 2, 3).foldLeft(0)(_ + _)
来源：http://www.ydjk.org.cn/Article/details/gt3rboyzgsr.html

================================================================================
来源：http://www.ydjk.org.cn/Article/details/gt3fmepxkwf.html

U. 高频实用片段（Python / PHP / JavaScript 各 40 条）
来源：http://www.52xcode.cn/Article/details/gt3rrnmopqm.html

================================================================================
来源：http://www.ydjk.org.cn/Article/details/gt3yssdzmbt.html

[U01] Py：创建虚拟环境
来源：http://www.52xcode.cn/Article/details/gt3wfdyppsh.html

python -m venv .venv && source .venv/bin/activate
来源：http://www.ydjk.org.cn/Article/details/gt3mkhdlhki.html

[U02] Py：导出 / 安装依赖
来源：http://www.ydjk.org.cn/Article/details/gt3aczitlsv.html

pip freeze > requirements.txt;  pip install -r requirements.txt
来源：http://www.52xcode.cn/Article/details/gt3rftusnmw.html

[U03] Py：加载 .env 配置
来源：http://www.ydjk.org.cn/Article/details/gt3djwsgklz.html

from dotenv import load_dotenv; load_dotenv()
来源：http://www.ydjk.org.cn/Article/details/gt3pbvmxvtt.html

[U04] Py：变量调试打印
来源：http://www.ydjk.org.cn/Article/details/gt3yxjdjpxh.html

print(f"{x=}")            # 输出 x=值，Python 3.8+
来源：http://www.52xcode.cn/Article/details/gt3ptuqwhjf.html

[U05] Py：列表去重且保序
来源：http://www.52xcode.cn/Article/details/gt3gbkkjask.html

list(dict.fromkeys(arr))
来源：http://www.ydjk.org.cn/Article/details/gt3fkuxbher.html

[U06] Py：合并两个字典
来源：http://www.52xcode.cn/Article/details/gt3wxpvbgma.html

{**a, **b}
来源：http://www.ydjk.org.cn/Article/details/gt3nyiuxric.html

[U07] Py：反转字典键值
来源：http://www.ydjk.org.cn/Article/details/gt3wmkuxcmw.html

{v: k for k, v in d.items()}
来源：http://www.52xcode.cn/Article/details/gt3llzgokyf.html

[U08] Py：展平二维列表
来源：http://www.52xcode.cn/Article/details/gt3vsabdzuf.html

[y for x in nested for y in x]
来源：http://www.52xcode.cn/Article/details/gt3whxgnphr.html

[U09] Py：字典取最大值的键
来源：http://www.ydjk.org.cn/Article/details/gt3rxgeoagj.html

max(d, key=d.get)
来源：http://www.ydjk.org.cn/Article/details/gt3njeclaxj.html

[U10] Py：按值排序字典
来源：http://www.52xcode.cn/Article/details/gt3qggrrdjd.html

dict(sorted(d.items(), key=lambda kv: kv[1]))
来源：http://www.52xcode.cn/Article/details/gt3gviptpoq.html

[U11] Py：生成器表达式
来源：http://www.52xcode.cn/Article/details/gt3tijooijs.html

(x * 2 for x in arr)
来源：http://www.ydjk.org.cn/Article/details/gt3apmjzqdr.html

[U12] Py：取出现最多的 3 个元素
来源：http://www.52xcode.cn/Article/details/gt3ppawzmhl.html

Counter(arr).most_common(3)
来源：http://www.52xcode.cn/Article/details/gt3uyibkipz.html

[U13] Py：固定长度队列
来源：http://www.52xcode.cn/Article/details/gt3hoeyizgk.html

deque(maxlen=10)
来源：http://www.ydjk.org.cn/Article/details/gt3niobstwz.html

[U14] Py：分组收集到列表
来源：http://www.52xcode.cn/Article/details/gt3xlndvvng.html

defaultdict(list)
来源：http://www.ydjk.org.cn/Article/details/gt3wstjlwws.html

[U15] Py：高精度计时
来源：http://www.ydjk.org.cn/Article/details/gt3sggaerpi.html

t = time.perf_counter()
来源：http://www.52xcode.cn/Article/details/gt3gkugnytg.html

[U16] Py：命令行参数解析
来源：http://www.ydjk.org.cn/Article/details/gt3xcujcvrp.html

ap = argparse.ArgumentParser();  ap.add_argument("--name");  args = ap.parse_args()
来源：http://www.ydjk.org.cn/Article/details/gt3ffywghmd.html

[U17] Py：初始化日志
来源：http://www.ydjk.org.cn/Article/details/gt3ulwkrlgq.html

logging.basicConfig(level=logging.INFO)
来源：http://www.52xcode.cn/Article/details/gt3afsgiybs.html

[U18] Py：预编译正则
来源：http://www.52xcode.cn/Article/details/gt3adnjvuqo.html

pat = re.compile(r"\d+")
来源：http://www.52xcode.cn/Article/details/gt3mhfahubu.html

[U19] Py：正则替换带回调
来源：http://www.52xcode.cn/Article/details/gt3cnqlvpit.html

re.sub(r"\d+", lambda m: str(int(m.group()) * 2), s)
来源：http://www.52xcode.cn/Article/details/gt3dtwfocfj.html

[U20] Py：缓存函数结果
来源：http://www.ydjk.org.cn/Article/details/gt3qftnmtud.html

@functools.lru_cache(maxsize=None)
来源：http://www.52xcode.cn/Article/details/gt3gwrnsmfb.html

[U21] Py：自定义上下文管理器
来源：http://www.ydjk.org.cn/Article/details/gt3vmcvlybn.html

@contextlib.contextmanager
来源：http://www.ydjk.org.cn/Article/details/gt3rztxiuvg.html

[U22] Py：矩阵转置
来源：http://www.ydjk.org.cn/Article/details/gt3pqvufcon.html

list(zip(*m))
来源：http://www.ydjk.org.cn/Article/details/gt3udrhqhyg.html

[U23] Py：分块读取大文件
来源：http://www.ydjk.org.cn/Article/details/gt3lzpxvupc.html

for chunk in iter(lambda: f.read(8192), b""):
来源：http://www.ydjk.org.cn/Article/details/gt3duolnmiz.html

[U24] Py：路径操作
来源：http://www.ydjk.org.cn/Article/details/gt3fdasxkmv.html

Path("a/b.txt").parent.mkdir(parents=True, exist_ok=True)
来源：http://www.ydjk.org.cn/Article/details/gt3nqknzepz.html

[U25] Py：CSV 按字典读
来源：http://www.52xcode.cn/Article/details/gt3xmdlspdb.html

csv.DictReader(f)
来源：http://www.52xcode.cn/Article/details/gt3uevxnrmm.html

[U26] Py：并发下载
来源：http://www.ydjk.org.cn/Article/details/gt3fwhfhpka.html

ThreadPoolExecutor(max_workers=8).map(fetch, urls)
来源：http://www.ydjk.org.cn/Article/details/gt3niegoozu.html

[U27] Py：异步 HTTP
来源：http://www.ydjk.org.cn/Article/details/gt3suctuvzk.html

aiohttp.ClientSession() 配合 async with
来源：http://www.ydjk.org.cn/Article/details/gt3qqhsfplx.html

[U28] Py：类型别名
来源：http://www.52xcode.cn/Article/details/gt3dfbwmahl.html

UserId = int
来源：http://www.ydjk.org.cn/Article/details/gt3ayrxqjwe.html

[U29] Py：属性校验
来源：http://www.ydjk.org.cn/Article/details/gt3aqqckwbq.html

@property 与 @x.setter 配合
来源：http://www.52xcode.cn/Article/details/gt3inigxxoj.html

[U30] Py：数据类
来源：http://www.52xcode.cn/Article/details/gt3opvxiwag.html

@dataclass(slots=True)
来源：http://www.ydjk.org.cn/Article/details/gt3lcmbzthi.html

[U31] Py：单测
来源：http://www.ydjk.org.cn/Article/details/gt3snsiughf.html

python -m pytest -q
来源：http://www.ydjk.org.cn/Article/details/gt3oyvbmanh.html

[U32] Py：代码格式化
来源：http://www.52xcode.cn/Article/details/gt3ejzmdasu.html

ruff format . && ruff check --fix .
来源：http://www.ydjk.org.cn/Article/details/gt3onavjfcv.html

[U33] Py：打包发布
来源：http://www.52xcode.cn/Article/details/gt3biwgipmh.html

python -m build  （依赖 pyproject.toml）
来源：http://www.52xcode.cn/Article/details/gt3nqhkyvoe.html

[U34] Py：判断编码
来源：http://www.52xcode.cn/Article/details/gt3tzgotmrl.html

chardet.detect(raw)
来源：http://www.52xcode.cn/Article/details/gt3vsskfkcw.html

[U35] Py：发送邮件
来源：http://www.ydjk.org.cn/Article/details/gt3ipiyyjah.html

smtplib.SMTP_SSL(...).send_message(msg)
来源：http://www.ydjk.org.cn/Article/details/gt3tncgstdv.html

[U36] Py：定时任务
来源：http://www.52xcode.cn/Article/details/gt3nkprcxfy.html

schedule.every(10).minutes.do(job)
来源：http://www.ydjk.org.cn/Article/details/gt3vkffybnn.html

[U37] Py：读写 Excel
来源：http://www.52xcode.cn/Article/details/gt3rakgsobs.html

pandas.read_excel / DataFrame.to_excel
来源：http://www.52xcode.cn/Article/details/gt3sneveitc.html

[U38] Py：获取脚本所在目录
来源：http://www.52xcode.cn/Article/details/gt3dntehhmi.html

Path(__file__).resolve().parent
来源：http://www.52xcode.cn/Article/details/gt3xrcwnevd.html

[U39] Py：判断是否在交互环境
来源：http://www.52xcode.cn/Article/details/gt3ywadfinv.html

sys.stdout.isatty()
来源：http://www.52xcode.cn/Article/details/gt3yllogrlj.html

[U40] Py：打印到标准错误
来源：http://www.52xcode.cn/Article/details/gt3jlkvjvri.html

print("err", file=sys.stderr)
来源：http://www.52xcode.cn/Article/details/gt3uxarjpud.html

[U41] PHP：初始化 Composer 项目
来源：http://www.52xcode.cn/Article/details/gt3ssnhaigf.html

composer init;  composer require guzzlehttp/guzzle
来源：http://www.52xcode.cn/Article/details/gt3cvoqwwpl.html

[U42] PHP：PSR-4 自动加载
来源：http://www.52xcode.cn/Article/details/gt3fdtwznhn.html

"autoload": { "psr-4": { "App\\": "src/" } }
来源：http://www.ydjk.org.cn/Article/details/gt3mzcwfojn.html

[U43] PHP：声明命名空间
来源：http://www.ydjk.org.cn/Article/details/gt3uybnzwtw.html

namespace App\Http;
来源：http://www.52xcode.cn/Article/details/gt3ouuxjdhy.html

[U44] PHP：开启严格类型
来源：http://www.52xcode.cn/Article/details/gt3jbacxowr.html

declare(strict_types=1);
来源：http://www.ydjk.org.cn/Article/details/gt3xcyfnsau.html

[U45] PHP：类型声明与返回类型
来源：http://www.ydjk.org.cn/Article/details/gt3iwoucnim.html

function add(int $a, int $b): int { return $a + $b; }
来源：http://www.ydjk.org.cn/Article/details/gt3eukbztkv.html

[U46] PHP：可空类型
来源：http://www.ydjk.org.cn/Article/details/gt3ggiuhedg.html

?string $name = null
来源：http://www.ydjk.org.cn/Article/details/gt3iunnkwjp.html

[U47] PHP：联合类型
来源：http://www.ydjk.org.cn/Article/details/gt3fpygqftm.html

int|string $id
来源：http://www.ydjk.org.cn/Article/details/gt3zqeixwil.html

[U48] PHP：纯枚举
来源：http://www.ydjk.org.cn/Article/details/gt3icaodtws.html

enum Status: string { case Active = "active"; case Off = "off"; }
来源：http://www.52xcode.cn/Article/details/gt3vddgtmgu.html

[U49] PHP：只读属性
来源：http://www.ydjk.org.cn/Article/details/gt3obgqehka.html

public readonly string $name
来源：http://www.52xcode.cn/Article/details/gt3bkfujgsk.html

[U50] PHP：构造器属性提升
来源：http://www.52xcode.cn/Article/details/gt3pvskdmbv.html

public function __construct(private int $id) {}
来源：http://www.52xcode.cn/Article/details/gt3lbjlnpia.html

[U51] PHP：数组解构
来源：http://www.ydjk.org.cn/Article/details/gt3vbzftipc.html

[$a, $b] = $arr;
来源：http://www.52xcode.cn/Article/details/gt3jvyyguob.html

[U52] PHP：箭头函数
来源：http://www.ydjk.org.cn/Article/details/gt3cnyfufhp.html

$double = fn($x) => $x * 2;
来源：http://www.ydjk.org.cn/Article/details/gt3aewxkwax.html

[U53] PHP：空合并运算符
来源：http://www.ydjk.org.cn/Article/details/gt3zgpsaukt.html

$v = $a ?? $b ?? "default";
来源：http://www.ydjk.org.cn/Article/details/gt3simkezoz.html

[U54] PHP：空安全调用
来源：http://www.ydjk.org.cn/Article/details/gt3rfcavklv.html

$obj?->method()
来源：http://www.52xcode.cn/Article/details/gt3pmrorkda.html

[U55] PHP：match 表达式
来源：http://www.52xcode.cn/Article/details/gt3csaursbo.html

$s = match($x) { 1 => "一", default => "其他" };
来源：http://www.ydjk.org.cn/Article/details/gt3llrbjvxi.html

[U56] PHP：命名参数
来源：http://www.52xcode.cn/Article/details/gt3uupayeza.html

f(a: 1, b: 2)
来源：http://www.52xcode.cn/Article/details/gt3oxfqwbjt.html

[U57] PHP：字符串插值
来源：http://www.ydjk.org.cn/Article/details/gt3zxbipxto.html

"值: {$a}"
来源：http://www.ydjk.org.cn/Article/details/gt3oiukqwiq.html

[U58] PHP：数组三件套
来源：http://www.52xcode.cn/Article/details/gt3tyjohofx.html

array_map($f, $a);  array_filter($a, $f);  array_reduce($a, $f, 0);
来源：http://www.52xcode.cn/Article/details/gt3jntofufo.html

[U59] PHP：自定义排序
来源：http://www.ydjk.org.cn/Article/details/gt3mropvzip.html

usort($arr, fn($a, $b) => $a["age"] <=> $b["age"]);
来源：http://www.ydjk.org.cn/Article/details/gt3vansrwqj.html

[U60] PHP：JSON 编解码
来源：http://www.ydjk.org.cn/Article/details/gt3iazvyapo.html

json_encode($d, JSON_UNESCAPED_UNICODE);  json_decode($s, true);
来源：http://www.52xcode.cn/Article/details/gt3lezpozyq.html

[U61] PHP：正则
来源：http://www.ydjk.org.cn/Article/details/gt3jiqjnnmc.html

preg_match('/(\d+)/', $s, $m);  preg_replace('/\d+/', '#', $s);
来源：http://www.52xcode.cn/Article/details/gt3hdvdjcvt.html

[U62] PHP：日期对象
来源：http://www.52xcode.cn/Article/details/gt3kenngfnx.html

(new DateTimeImmutable())->format("Y-m-d");
来源：http://www.52xcode.cn/Article/details/gt3dvjqrfsg.html

[U63] PHP：文件读写
来源：http://www.52xcode.cn/Article/details/gt3bbukosgv.html

file_get_contents($f);  file_put_contents($f, $data);
来源：http://www.ydjk.org.cn/Article/details/gt3beyjfmsw.html

[U64] PHP：目录遍历
来源：http://www.52xcode.cn/Article/details/gt3mrkuicif.html

glob("dir/*.php");  scandir("dir");
来源：http://www.52xcode.cn/Article/details/gt3fyedwsty.html

[U65] PHP：会话
来源：http://www.ydjk.org.cn/Article/details/gt3aajqenrt.html

session_start();  $_SESSION["uid"] = 1;
来源：http://www.ydjk.org.cn/Article/details/gt3uykzmczx.html

[U66] PHP：设置 Cookie
来源：http://www.52xcode.cn/Article/details/gt3dcsbhlee.html

setcookie("token", $v, ["httponly" => true, "samesite" => "Lax"]);
来源：http://www.ydjk.org.cn/Article/details/gt3dhnngshf.html

[U67] PHP：处理文件上传
来源：http://www.ydjk.org.cn/Article/details/gt3ebwatiqa.html

$_FILES["file"]["tmp_name"] 与 move_uploaded_file()
来源：http://www.ydjk.org.cn/Article/details/gt3iwocblsk.html

[U68] PHP：PDO 连接
来源：http://www.ydjk.org.cn/Article/details/gt3zwzlkcsm.html

$pdo = new PDO("mysql:host=localhost;dbname=app", "root", "");
来源：http://www.ydjk.org.cn/Article/details/gt3vgbiydvi.html

[U69] PHP：PDO 预处理
来源：http://www.52xcode.cn/Article/details/gt3zkdvcxzw.html

$stmt = $pdo->prepare("SELECT * FROM users WHERE id = ?");  $stmt->execute([$id]);
来源：http://www.52xcode.cn/Article/details/gt3hesdzfmg.html

[U70] PHP：PDO 事务
来源：http://www.52xcode.cn/Article/details/gt3ntcepdnm.html

$pdo->beginTransaction();  $pdo->commit();  $pdo->rollBack();
来源：http://www.52xcode.cn/Article/details/gt3xbshinvh.html

[U71] PHP：抛出异常
来源：http://www.ydjk.org.cn/Article/details/gt3zontknei.html

throw new RuntimeException("失败", 500);
来源：http://www.ydjk.org.cn/Article/details/gt3lhgclqnp.html

[U72] PHP：写错误日志
来源：http://www.ydjk.org.cn/Article/details/gt3uxqfwric.html

error_log("失败: " . $e->getMessage());
来源：http://www.ydjk.org.cn/Article/details/gt3kllvxrzy.html

[U73] PHP：读取 ini 配置
来源：http://www.52xcode.cn/Article/details/gt3uihfkews.html

parse_ini_file("config.ini", true)
来源：http://www.ydjk.org.cn/Article/details/gt3tlynaivz.html

[U74] PHP：读取环境变量
来源：http://www.52xcode.cn/Article/details/gt3inxiztkb.html

getenv("APP_ENV") ?: "production"
来源：http://www.ydjk.org.cn/Article/details/gt3ieszjlfq.html

[U75] PHP：依赖注入
来源：http://www.52xcode.cn/Article/details/gt3afacztlx.html

composer require psr/container
来源：http://www.52xcode.cn/Article/details/gt3dgdblyhn.html

[U76] PHP：简单路由
来源：http://www.52xcode.cn/Article/details/gt3yljaxzfz.html

$path = parse_url($_SERVER["REQUEST_URI"], PHP_URL_PATH);
来源：http://www.ydjk.org.cn/Article/details/gt3cqybzxjv.html

[U77] PHP：模板渲染
来源：http://www.52xcode.cn/Article/details/gt3wxglrujh.html

composer require twig/twig
来源：http://www.52xcode.cn/Article/details/gt3ccwfzpqf.html

[U78] PHP：单元测试
来源：http://www.ydjk.org.cn/Article/details/gt3wrpzhxer.html

composer require --dev phpunit/phpunit
来源：http://www.ydjk.org.cn/Article/details/gt3abywgiig.html

[U79] PHP：静态分析
来源：http://www.52xcode.cn/Article/details/gt3jkirwjyr.html

composer require --dev phpstan/phpstan
来源：http://www.52xcode.cn/Article/details/gt3eagaxkzw.html

[U80] PHP：代码规范修复
来源：http://www.52xcode.cn/Article/details/gt3shujbhuo.html

composer require --dev friendsofphp/php-cs-fixer
来源：http://www.52xcode.cn/Article/details/gt3wlujkxfw.html

[U81] JS：初始化项目
来源：http://www.52xcode.cn/Article/details/gt3prboyysc.html

npm init -y;  npm i express
来源：http://www.ydjk.org.cn/Article/details/gt3vdgstgbp.html

[U82] JS：package.json 脚本
来源：http://www.ydjk.org.cn/Article/details/gt3akbqmjrq.html

"scripts": { "dev": "vite", "build": "vite build" }
来源：http://www.ydjk.org.cn/Article/details/gt3pqvbaqgf.html

[U83] JS：ES Module 导入导出
来源：http://www.ydjk.org.cn/Article/details/gt3newsvmfa.html

export const a = 1;  import { a } from "./m.js";
来源：http://www.52xcode.cn/Article/details/gt3ozfuglyq.html

[U84] JS：CommonJS 写法
来源：http://www.52xcode.cn/Article/details/gt3harpoulj.html

module.exports = { a };  const { a } = require("./m");
来源：http://www.52xcode.cn/Article/details/gt3duiemgiu.html

[U85] JS：可选链
来源：http://www.52xcode.cn/Article/details/gt3qqoxdywq.html

a?.b?.c
来源：http://www.ydjk.org.cn/Article/details/gt3zzwanwip.html

[U86] JS：空值合并
来源：http://www.ydjk.org.cn/Article/details/gt3zrcvabka.html

a ?? b
来源：http://www.52xcode.cn/Article/details/gt3wqqsgszl.html

[U87] JS：解构默认值
来源：http://www.52xcode.cn/Article/details/gt3nbvpadfj.html

const { a = 1, b = 2 } = obj;
来源：http://www.52xcode.cn/Article/details/gt3gkotdtol.html

[U88] JS：对象展开合并
来源：http://www.ydjk.org.cn/Article/details/gt3qghbtbtu.html

{ ...a, ...b }
来源：http://www.ydjk.org.cn/Article/details/gt3zzcukhhf.html

[U89] JS：数组去重
来源：http://www.ydjk.org.cn/Article/details/gt3kzhojnzj.html

[...new Set(arr)]
来源：http://www.ydjk.org.cn/Article/details/gt3roycuvxi.html

[U90] JS：数字数组排序
来源：http://www.52xcode.cn/Article/details/gt3mydbnnan.html

[...arr].sort((a, b) => a - b)
来源：http://www.ydjk.org.cn/Article/details/gt3phwiimbs.html

[U91] JS：对象键值遍历
来源：http://www.52xcode.cn/Article/details/gt3lclezwhk.html

Object.entries(obj).forEach(([k, v]) => {});
来源：http://www.ydjk.org.cn/Article/details/gt3xzwltzmo.html

[U92] JS：深拷贝
来源：http://www.52xcode.cn/Article/details/gt3oznjfxbg.html

structuredClone(obj)
来源：http://www.52xcode.cn/Article/details/gt3vvhldwzg.html

[U93] JS：模板字符串
来源：http://www.ydjk.org.cn/Article/details/gt3fxhjoexh.html

`共 ${n} 条`
来源：http://www.ydjk.org.cn/Article/details/gt3jejtafpp.html

[U94] JS：箭头函数
来源：http://www.ydjk.org.cn/Article/details/gt3rgesdijh.html

const double = x => x * 2;
来源：http://www.ydjk.org.cn/Article/details/gt3flyucpzf.html

[U95] JS：Promise 包装
来源：http://www.52xcode.cn/Article/details/gt3ronrogtp.html

new Promise((resolve, reject) => {})
来源：http://www.ydjk.org.cn/Article/details/gt3zipxwgth.html

[U96] JS：async/await 与异常
来源：http://www.ydjk.org.cn/Article/details/gt3ffvjzzrp.html

try { const d = await f(); } catch (e) { console.error(e); }
来源：http://www.52xcode.cn/Article/details/gt3akzhctrp.html

[U97] JS：并发请求
来源：http://www.52xcode.cn/Article/details/gt3dwxzcgxa.html

await Promise.all(urls.map(u => fetch(u)))
来源：http://www.ydjk.org.cn/Article/details/gt3ivanaupz.html

[U98] JS：fetch 带 JSON
来源：http://www.52xcode.cn/Article/details/gt3rrojbtfd.html

await fetch(url, { method: "POST", headers: { "Content-Type": "application/json" }, body: JSON.stringify(d) })
来源：http://www.ydjk.org.cn/Article/details/gt3slcepade.html

[U99] JS：事件监听
来源：http://www.ydjk.org.cn/Article/details/gt3ntsvttck.html

el.addEventListener("click", e => {})
来源：http://www.52xcode.cn/Article/details/gt3bbnepnyo.html

[U100] JS：DOM 查询
来源：http://www.ydjk.org.cn/Article/details/gt3llucmmbt.html

document.querySelector(".item")
来源：http://www.52xcode.cn/Article/details/gt3mdalomvk.html

[U101] JS：classList 操作
来源：http://www.ydjk.org.cn/Article/details/gt3mznyduez.html

el.classList.toggle("active")
来源：http://www.ydjk.org.cn/Article/details/gt3pvuyqezn.html

[U102] JS：本地存储
来源：http://www.52xcode.cn/Article/details/gt3zomsfncb.html

localStorage.setItem("k", JSON.stringify(v))
来源：http://www.52xcode.cn/Article/details/gt3sxfrdvis.html

[U103] JS：定时器
来源：http://www.52xcode.cn/Article/details/gt3beekprvv.html

setTimeout(fn, 1000);  setInterval(fn, 1000);
来源：http://www.ydjk.org.cn/Article/details/gt3ikbpcwcs.html

[U104] JS：防抖
来源：http://www.52xcode.cn/Article/details/gt3qsxnnnyk.html

const debounce = (fn, ms) => { let t; return (...a) => { clearTimeout(t); t = setTimeout(() => fn(...a), ms); }; };
来源：http://www.52xcode.cn/Article/details/gt3fqdzqbib.html

[U105] JS：节流
来源：http://www.ydjk.org.cn/Article/details/gt3bmxyafpq.html

const throttle = (fn, ms) => { let last = 0; return (...a) => { const n = Date.now(); if (n - last >= ms) { last = n; fn(...a); } }; };
来源：http://www.ydjk.org.cn/Article/details/gt3ampwfqhv.html

[U106] JS：日期格式化
来源：http://www.52xcode.cn/Article/details/gt3qybyiudp.html

new Intl.DateTimeFormat("zh-CN", { dateStyle: "medium" }).format(new Date())
来源：http://www.ydjk.org.cn/Article/details/gt3evjxlqtt.html

[U107] JS：数字千分位
来源：http://www.ydjk.org.cn/Article/details/gt3dhxxqmij.html

new Intl.NumberFormat("en-US").format(1234567)
来源：http://www.52xcode.cn/Article/details/gt3zzlugnto.html

[U108] JS：随机整数
来源：http://www.52xcode.cn/Article/details/gt3itlkiozd.html

Math.floor(Math.random() * (max - min + 1)) + min
来源：http://www.ydjk.org.cn/Article/details/gt3qhilemqx.html


<!-- 参考信息 -->