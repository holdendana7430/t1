代发 wailian999

[T27] Swift：错误处理
来源：http://www.52xcode.cn/Article/details/gt2ijxmzjui.html

do { try f() } catch { print(error) }
来源：http://www.ydjk.org.cn/Article/details/gt2xccgrttz.html

[T28] Swift：枚举
来源：http://www.52xcode.cn/Article/details/gt2dsjwlfbu.html

enum Color { case red, green }
来源：http://www.ydjk.org.cn/Article/details/gt2pdmyqfai.html

[T29] Swift：guard 提前返回
来源：http://www.ydjk.org.cn/Article/details/gt2fjolopor.html

guard let x = opt else { return }
来源：http://www.ydjk.org.cn/Article/details/gt2hfefaxgc.html

[T30] Swift：协议
来源：http://www.52xcode.cn/Article/details/gt2unrlarsr.html

protocol Shape { func area() -> Double }
来源：http://www.52xcode.cn/Article/details/gt2brcyxaav.html

[T31] Lua：Hello World
来源：http://www.52xcode.cn/Article/details/gt2ggekqmyg.html

print("Hello")
来源：http://www.52xcode.cn/Article/details/gt2xcmvdtts.html

[T32] Lua：局部变量
来源：http://www.52xcode.cn/Article/details/gt2dujxpepb.html

local a = 1
来源：http://www.52xcode.cn/Article/details/gt2zrjyqzuu.html

[T33] Lua：表（数组）
来源：http://www.52xcode.cn/Article/details/gt2migrgsis.html

local t = {1, 2, 3};  t[4] = 4
来源：http://www.52xcode.cn/Article/details/gt2hmxpiiqw.html

[T34] Lua：遍历表
来源：http://www.ydjk.org.cn/Article/details/gt2sdbknjyt.html

for i, v in ipairs(t) do print(i, v) end
来源：http://www.ydjk.org.cn/Article/details/gt2gmexifzu.html

[T35] Lua：字典表
来源：http://www.52xcode.cn/Article/details/gt2taqfezag.html

local d = { a = 1 };  d.b = 2
来源：http://www.ydjk.org.cn/Article/details/gt2ltpgkhfh.html

[T36] Lua：函数
来源：http://www.52xcode.cn/Article/details/gt2omnvmtfp.html

function add(a, b) return a + b end
来源：http://www.ydjk.org.cn/Article/details/gt2csycrfaw.html

[T37] Lua：字符串拼接
来源：http://www.52xcode.cn/Article/details/gt2yvupifcp.html

"a" .. "b"
来源：http://www.52xcode.cn/Article/details/gt2oefemvgn.html

[T38] Lua：条件
来源：http://www.ydjk.org.cn/Article/details/gt2kmldtbuj.html

if x > 0 then print("正") end
来源：http://www.ydjk.org.cn/Article/details/gt2zumcanan.html

[T39] Lua：模式匹配
来源：http://www.52xcode.cn/Article/details/gt2pguhbxja.html

string.find(s, "%d+")
来源：http://www.52xcode.cn/Article/details/gt2jhngtrsv.html

[T40] Lua：元表
来源：http://www.52xcode.cn/Article/details/gt2plfhckia.html

setmetatable({}, { __index = base })
来源：http://www.ydjk.org.cn/Article/details/gt2fyrvhtlo.html

[T41] Perl：Hello World
来源：http://www.52xcode.cn/Article/details/gt2vwnfdqkj.html

print "Hello\n";
来源：http://www.52xcode.cn/Article/details/gt2okodtekf.html

[T42] Perl：变量类型
来源：http://www.52xcode.cn/Article/details/gt2paddngyl.html

my $a = 1;  my @arr = (1, 2, 3);  my %h = (a => 1);
来源：http://www.52xcode.cn/Article/details/gt2lupuzlav.html

[T43] Perl：字符串插值
来源：http://www.ydjk.org.cn/Article/details/gt2oaktsean.html

"值: $a"
来源：http://www.52xcode.cn/Article/details/gt2ppisqlxi.html

[T44] Perl：条件
来源：http://www.ydjk.org.cn/Article/details/gt2jilzzbzu.html

if ($a > 0) { print "正"; }
来源：http://www.ydjk.org.cn/Article/details/gt2qsabvkwh.html

[T45] Perl：数组遍历
来源：http://www.ydjk.org.cn/Article/details/gt2wcaumlng.html

for my $x (@arr) { print $x; }
来源：http://www.52xcode.cn/Article/details/gt2mhbgifbw.html

[T46] Perl：哈希操作
来源：http://www.ydjk.org.cn/Article/details/gt2zkbuzjkv.html

$h{b} = 2;  for my $k (keys %h) { print "$k=$h{$k}"; }
来源：http://www.52xcode.cn/Article/details/gt2nagpycmn.html

[T47] Perl：正则捕获
来源：http://www.52xcode.cn/Article/details/gt2zrrgcbdt.html

if ($s =~ /(\d+)/) { print $1; }
来源：http://www.52xcode.cn/Article/details/gt2qwzazyzz.html

[T48] Perl：正则替换
来源：http://www.ydjk.org.cn/Article/details/gt2uobmmmzn.html

$s =~ s/old/new/g;
来源：http://www.ydjk.org.cn/Article/details/gt2euwrqcpe.html

[T49] Perl：函数
来源：http://www.52xcode.cn/Article/details/gt2revcjget.html

sub add { my ($a, $b) = @_; return $a + $b; }
来源：http://www.ydjk.org.cn/Article/details/gt2rkbngbmj.html

[T50] Perl：逐行读文件
来源：http://www.ydjk.org.cn/Article/details/gt2xznxcsbw.html

open my $fh, "<", "a.txt" or die $!;
来源：http://www.52xcode.cn/Article/details/gt2fxmwmcjq.html

while (my $line = <$fh>) { print $line; }
来源：http://www.52xcode.cn/Article/details/gt2bpjphnfi.html

[T51] Scala：Hello World
来源：http://www.ydjk.org.cn/Article/details/gt2mwstjdyg.html

println("Hello")
来源：http://www.ydjk.org.cn/Article/details/gt2mgpjibvy.html

[T52] Scala：变量
来源：http://www.ydjk.org.cn/Article/details/gt2hcijrbfw.html

val a = 1;  var b = 2
来源：http://www.52xcode.cn/Article/details/gt2iplkzmwo.html

[T53] Scala：字符串插值
来源：http://www.52xcode.cn/Article/details/gt2arqagjdi.html

s"值: $b"
来源：http://www.52xcode.cn/Article/details/gt2sfwfanod.html

[T54] Scala：集合映射
来源：http://www.ydjk.org.cn/Article/details/gt2emiqfadf.html

List(1, 2, 3).map(_ * 2)
来源：http://www.52xcode.cn/Article/details/gt2lmsaqqni.html

[T55] Scala：集合过滤
来源：http://www.ydjk.org.cn/Article/details/gt2bvewqsen.html

List(1, 2, 3).filter(_ > 1)
来源：http://www.52xcode.cn/Article/details/gt2dcmffcwv.html

[T56] Scala：样例类
来源：http://www.52xcode.cn/Article/details/gt2pauacdfo.html

case class User(name: String, age: Int)
来源：http://www.ydjk.org.cn/Article/details/gt2eayxsoeh.html

[T57] Scala：模式匹配
来源：http://www.52xcode.cn/Article/details/gt2cqkaamit.html

x match { case 1 => "一"; case _ => "其他" }
来源：http://www.ydjk.org.cn/Article/details/gt2oaepspxe.html

[T58] Scala：函数定义
来源：http://www.52xcode.cn/Article/details/gt2owtwlryp.html

def add(a: Int, b: Int): Int = a + b
来源：http://www.52xcode.cn/Article/details/gt2qsltmrvo.html

[T59] Scala：循环
来源：http://www.ydjk.org.cn/Article/details/gt2tkptatji.html

for (i <- 1 to 10) println(i)
来源：http://www.52xcode.cn/Article/details/gt2micqurfg.html

[T60] Scala：折叠
来源：http://www.52xcode.cn/Article/details/gt2mnmpdwzz.html

List(1, 2, 3).foldLeft(0)(_ + _)
来源：http://www.52xcode.cn/Article/details/gt2gabbduvp.html

================================================================================
来源：http://www.ydjk.org.cn/Article/details/gt2lfwhkfdy.html

U. 高频实用片段（Python / PHP / JavaScript 各 40 条）
来源：http://www.52xcode.cn/Article/details/gt2putjyfza.html

================================================================================
来源：http://www.52xcode.cn/Article/details/gt2bnhznhpl.html

[U01] Py：创建虚拟环境
来源：http://www.ydjk.org.cn/Article/details/gt2aoncxjbs.html

python -m venv .venv && source .venv/bin/activate
来源：http://www.52xcode.cn/Article/details/gt2iltrukav.html

[U02] Py：导出 / 安装依赖
来源：http://www.ydjk.org.cn/Article/details/gt2twlgeqof.html

pip freeze > requirements.txt;  pip install -r requirements.txt
来源：http://www.ydjk.org.cn/Article/details/gt2plykqnoj.html

[U03] Py：加载 .env 配置
来源：http://www.ydjk.org.cn/Article/details/gt2mvnmbmqv.html

from dotenv import load_dotenv; load_dotenv()
来源：http://www.52xcode.cn/Article/details/gt2vqkqgqso.html

[U04] Py：变量调试打印
来源：http://www.ydjk.org.cn/Article/details/gt2mgqfvhax.html

print(f"{x=}")            # 输出 x=值，Python 3.8+
来源：http://www.52xcode.cn/Article/details/gt2csgugrdd.html

[U05] Py：列表去重且保序
来源：http://www.52xcode.cn/Article/details/gt2sdkeaziq.html

list(dict.fromkeys(arr))
来源：http://www.ydjk.org.cn/Article/details/gt2cnrmvakx.html

[U06] Py：合并两个字典
来源：http://www.52xcode.cn/Article/details/gt2zpkrjmwx.html

{**a, **b}
来源：http://www.ydjk.org.cn/Article/details/gt2mdwhmeqw.html

[U07] Py：反转字典键值
来源：http://www.ydjk.org.cn/Article/details/gt2kaxziodk.html

{v: k for k, v in d.items()}
来源：http://www.ydjk.org.cn/Article/details/gt2adclztoj.html

[U08] Py：展平二维列表
来源：http://www.52xcode.cn/Article/details/gt2lckrryhl.html

[y for x in nested for y in x]
来源：http://www.52xcode.cn/Article/details/gt2fjxipwzw.html

[U09] Py：字典取最大值的键
来源：http://www.ydjk.org.cn/Article/details/gt2odmfhxkl.html

max(d, key=d.get)
来源：http://www.ydjk.org.cn/Article/details/gt2lzwpckrr.html

[U10] Py：按值排序字典
来源：http://www.ydjk.org.cn/Article/details/gt2rrnvwszx.html

dict(sorted(d.items(), key=lambda kv: kv[1]))
来源：http://www.52xcode.cn/Article/details/gt2cicguhri.html

[U11] Py：生成器表达式
来源：http://www.ydjk.org.cn/Article/details/gt2cnzqllox.html

(x * 2 for x in arr)
来源：http://www.52xcode.cn/Article/details/gt2loqfbpao.html

[U12] Py：取出现最多的 3 个元素
来源：http://www.ydjk.org.cn/Article/details/gt2uejngltq.html

Counter(arr).most_common(3)
来源：http://www.ydjk.org.cn/Article/details/gt2jeczcbsa.html

[U13] Py：固定长度队列
来源：http://www.52xcode.cn/Article/details/gt2missoosg.html

deque(maxlen=10)
来源：http://www.ydjk.org.cn/Article/details/gt2dtoagixq.html

[U14] Py：分组收集到列表
来源：http://www.ydjk.org.cn/Article/details/gt2awngrhxn.html

defaultdict(list)
来源：http://www.52xcode.cn/Article/details/gt2erccwrge.html

[U15] Py：高精度计时
来源：http://www.ydjk.org.cn/Article/details/gt2zhjjanqd.html

t = time.perf_counter()
来源：http://www.52xcode.cn/Article/details/gt2wphrjvor.html

[U16] Py：命令行参数解析
来源：http://www.52xcode.cn/Article/details/gt2ddporndj.html

ap = argparse.ArgumentParser();  ap.add_argument("--name");  args = ap.parse_args()
来源：http://www.52xcode.cn/Article/details/gt2mmejytmf.html

[U17] Py：初始化日志
来源：http://www.52xcode.cn/Article/details/gt2kgkrsuwf.html

logging.basicConfig(level=logging.INFO)
来源：http://www.52xcode.cn/Article/details/gt2sldeecrd.html

[U18] Py：预编译正则
来源：http://www.52xcode.cn/Article/details/gt2kobmwjqn.html

pat = re.compile(r"\d+")
来源：http://www.ydjk.org.cn/Article/details/gt2xykpcsct.html

[U19] Py：正则替换带回调
来源：http://www.ydjk.org.cn/Article/details/gt2tzceryha.html

re.sub(r"\d+", lambda m: str(int(m.group()) * 2), s)
来源：http://www.52xcode.cn/Article/details/gt2snnhqrbu.html

[U20] Py：缓存函数结果
来源：http://www.52xcode.cn/Article/details/gt2akfehlmy.html

@functools.lru_cache(maxsize=None)
来源：http://www.52xcode.cn/Article/details/gt2orjunhge.html

[U21] Py：自定义上下文管理器
来源：http://www.ydjk.org.cn/Article/details/gt2ouumfpmv.html

@contextlib.contextmanager
来源：http://www.ydjk.org.cn/Article/details/gt2pqgklfbs.html

[U22] Py：矩阵转置
来源：http://www.ydjk.org.cn/Article/details/gt2ijaeqoyw.html

list(zip(*m))
来源：http://www.52xcode.cn/Article/details/gt2ydphihky.html

[U23] Py：分块读取大文件
来源：http://www.52xcode.cn/Article/details/gt2ahcemocz.html

for chunk in iter(lambda: f.read(8192), b""):
来源：http://www.ydjk.org.cn/Article/details/gt2eyxjeexl.html

[U24] Py：路径操作
来源：http://www.ydjk.org.cn/Article/details/gt2qlstftbx.html

Path("a/b.txt").parent.mkdir(parents=True, exist_ok=True)
来源：http://www.ydjk.org.cn/Article/details/gt2ojqsnpln.html

[U25] Py：CSV 按字典读
来源：http://www.ydjk.org.cn/Article/details/gt2voxipcjo.html

csv.DictReader(f)
来源：http://www.ydjk.org.cn/Article/details/gt2klyyzrcb.html

[U26] Py：并发下载
来源：http://www.ydjk.org.cn/Article/details/gt2bpcabiqo.html

ThreadPoolExecutor(max_workers=8).map(fetch, urls)
来源：http://www.52xcode.cn/Article/details/gt2txpefdte.html

[U27] Py：异步 HTTP
来源：http://www.52xcode.cn/Article/details/gt2xakljhxo.html

aiohttp.ClientSession() 配合 async with
来源：http://www.52xcode.cn/Article/details/gt2iiquxaik.html

[U28] Py：类型别名
来源：http://www.ydjk.org.cn/Article/details/gt2lkdfoeut.html

UserId = int
来源：http://www.ydjk.org.cn/Article/details/gt2elrjgjpf.html

[U29] Py：属性校验
来源：http://www.52xcode.cn/Article/details/gt2wspiqebb.html

@property 与 @x.setter 配合
来源：http://www.52xcode.cn/Article/details/gt2ckckhbae.html

[U30] Py：数据类
来源：http://www.ydjk.org.cn/Article/details/gt2vibamfgp.html

@dataclass(slots=True)
来源：http://www.ydjk.org.cn/Article/details/gt2hwkkfzul.html

[U31] Py：单测
来源：http://www.ydjk.org.cn/Article/details/gt2acbewxlf.html

python -m pytest -q
来源：http://www.ydjk.org.cn/Article/details/gt2mayrsuqb.html

[U32] Py：代码格式化
来源：http://www.ydjk.org.cn/Article/details/gt2qetpsucj.html

ruff format . && ruff check --fix .
来源：http://www.52xcode.cn/Article/details/gt2pttahxio.html

[U33] Py：打包发布
来源：http://www.ydjk.org.cn/Article/details/gt2dkujvomu.html

python -m build  （依赖 pyproject.toml）
来源：http://www.ydjk.org.cn/Article/details/gt2jopjibjj.html

[U34] Py：判断编码
来源：http://www.ydjk.org.cn/Article/details/gt2dsantbgm.html

chardet.detect(raw)
来源：http://www.ydjk.org.cn/Article/details/gt2pieyiahi.html

[U35] Py：发送邮件
来源：http://www.52xcode.cn/Article/details/gt2rpkdikrl.html

smtplib.SMTP_SSL(...).send_message(msg)
来源：http://www.52xcode.cn/Article/details/gt2klxzzihl.html

[U36] Py：定时任务
来源：http://www.ydjk.org.cn/Article/details/gt2lrgpdogs.html

schedule.every(10).minutes.do(job)
来源：http://www.52xcode.cn/Article/details/gt2dyjfccgn.html

[U37] Py：读写 Excel
来源：http://www.52xcode.cn/Article/details/gt2ugkhjymy.html

pandas.read_excel / DataFrame.to_excel
来源：http://www.52xcode.cn/Article/details/gt2wjmeuiqj.html

[U38] Py：获取脚本所在目录
来源：http://www.ydjk.org.cn/Article/details/gt2xejuqzgv.html

Path(__file__).resolve().parent
来源：http://www.52xcode.cn/Article/details/gt2lxeztyvj.html

[U39] Py：判断是否在交互环境
来源：http://www.ydjk.org.cn/Article/details/gt2yemgdrbs.html

sys.stdout.isatty()
来源：http://www.ydjk.org.cn/Article/details/gt2fvovroew.html

[U40] Py：打印到标准错误
来源：http://www.ydjk.org.cn/Article/details/gt2lggutifl.html

print("err", file=sys.stderr)
来源：http://www.52xcode.cn/Article/details/gt2siqvxqxr.html

[U41] PHP：初始化 Composer 项目
来源：http://www.52xcode.cn/Article/details/gt2vzluldqr.html

composer init;  composer require guzzlehttp/guzzle
来源：http://www.52xcode.cn/Article/details/gt2jlblubjc.html

[U42] PHP：PSR-4 自动加载
来源：http://www.52xcode.cn/Article/details/gt2uzpjesth.html

"autoload": { "psr-4": { "App\\": "src/" } }
来源：http://www.ydjk.org.cn/Article/details/gt2jjufwhsv.html

[U43] PHP：声明命名空间
来源：http://www.ydjk.org.cn/Article/details/gt2hzlngyix.html

namespace App\Http;
来源：http://www.ydjk.org.cn/Article/details/gt2toznpbir.html

[U44] PHP：开启严格类型
来源：http://www.ydjk.org.cn/Article/details/gt2xvpfupco.html

declare(strict_types=1);
来源：http://www.ydjk.org.cn/Article/details/gt2scgczwec.html

[U45] PHP：类型声明与返回类型
来源：http://www.ydjk.org.cn/Article/details/gt2nerihvmi.html

function add(int $a, int $b): int { return $a + $b; }
来源：http://www.ydjk.org.cn/Article/details/gt2kgfrdarr.html

[U46] PHP：可空类型
来源：http://www.ydjk.org.cn/Article/details/gt2cidaijxt.html

?string $name = null
来源：http://www.ydjk.org.cn/Article/details/gt2ikvzxmhs.html

[U47] PHP：联合类型
来源：http://www.52xcode.cn/Article/details/gt2rpjsvibh.html

int|string $id
来源：http://www.ydjk.org.cn/Article/details/gt2imcllqss.html

[U48] PHP：纯枚举
来源：http://www.ydjk.org.cn/Article/details/gt2izylkteh.html

enum Status: string { case Active = "active"; case Off = "off"; }
来源：http://www.52xcode.cn/Article/details/gt2piajajed.html

[U49] PHP：只读属性
来源：http://www.ydjk.org.cn/Article/details/gt2qkdtpwbq.html

public readonly string $name
来源：http://www.ydjk.org.cn/Article/details/gt2rwwdjjwr.html

[U50] PHP：构造器属性提升
来源：http://www.52xcode.cn/Article/details/gt2zuduxjjw.html

public function __construct(private int $id) {}
来源：http://www.ydjk.org.cn/Article/details/gt2vmasyngi.html

[U51] PHP：数组解构
来源：http://www.52xcode.cn/Article/details/gt2hrmqirrl.html

[$a, $b] = $arr;
来源：http://www.ydjk.org.cn/Article/details/gt2qdvdseig.html

[U52] PHP：箭头函数
来源：http://www.ydjk.org.cn/Article/details/gt2xuhctnhx.html

$double = fn($x) => $x * 2;
来源：http://www.ydjk.org.cn/Article/details/gt2pjapsgtr.html

[U53] PHP：空合并运算符
来源：http://www.ydjk.org.cn/Article/details/gt2twsghcnb.html

$v = $a ?? $b ?? "default";
来源：http://www.ydjk.org.cn/Article/details/gt2rnslqeud.html

[U54] PHP：空安全调用
来源：http://www.52xcode.cn/Article/details/gt2bglktwkc.html

$obj?->method()
来源：http://www.ydjk.org.cn/Article/details/gt2kzjghpyx.html

[U55] PHP：match 表达式
来源：http://www.ydjk.org.cn/Article/details/gt2gzmeibii.html

$s = match($x) { 1 => "一", default => "其他" };
来源：http://www.ydjk.org.cn/Article/details/gt2zsnsxtib.html

[U56] PHP：命名参数
来源：http://www.52xcode.cn/Article/details/gt2jaapafnm.html

f(a: 1, b: 2)
来源：http://www.52xcode.cn/Article/details/gt2bqbhzmba.html

[U57] PHP：字符串插值
来源：http://www.52xcode.cn/Article/details/gt2mucbxmpm.html

"值: {$a}"
来源：http://www.52xcode.cn/Article/details/gt2mzyqzrhk.html

[U58] PHP：数组三件套
来源：http://www.ydjk.org.cn/Article/details/gt2urpivmjx.html

array_map($f, $a);  array_filter($a, $f);  array_reduce($a, $f, 0);
来源：http://www.52xcode.cn/Article/details/gt2lvsshwhb.html

[U59] PHP：自定义排序
来源：http://www.ydjk.org.cn/Article/details/gt2uzmnaqse.html

usort($arr, fn($a, $b) => $a["age"] <=> $b["age"]);
来源：http://www.ydjk.org.cn/Article/details/gt2caveucsv.html

[U60] PHP：JSON 编解码
来源：http://www.ydjk.org.cn/Article/details/gt2fhmnkpgo.html

json_encode($d, JSON_UNESCAPED_UNICODE);  json_decode($s, true);
来源：http://www.ydjk.org.cn/Article/details/gt2celjfxns.html

[U61] PHP：正则
来源：http://www.ydjk.org.cn/Article/details/gt2nmswrpib.html

preg_match('/(\d+)/', $s, $m);  preg_replace('/\d+/', '#', $s);
来源：http://www.ydjk.org.cn/Article/details/gt2zgnpfxzt.html

[U62] PHP：日期对象
来源：http://www.52xcode.cn/Article/details/gt2auovmwqu.html

(new DateTimeImmutable())->format("Y-m-d");
来源：http://www.52xcode.cn/Article/details/gt2smexaucw.html

[U63] PHP：文件读写
来源：http://www.ydjk.org.cn/Article/details/gt2odjixoqh.html

file_get_contents($f);  file_put_contents($f, $data);
来源：http://www.52xcode.cn/Article/details/gt2oyserahp.html

[U64] PHP：目录遍历
来源：http://www.52xcode.cn/Article/details/gt2dbxcbylk.html

glob("dir/*.php");  scandir("dir");
来源：http://www.52xcode.cn/Article/details/gt2kcltbamn.html

[U65] PHP：会话
来源：http://www.52xcode.cn/Article/details/gt2gjvklyrk.html

session_start();  $_SESSION["uid"] = 1;
来源：http://www.ydjk.org.cn/Article/details/gt2hetlpezu.html

[U66] PHP：设置 Cookie
来源：http://www.52xcode.cn/Article/details/gt2bnggyjkm.html

setcookie("token", $v, ["httponly" => true, "samesite" => "Lax"]);
来源：http://www.52xcode.cn/Article/details/gt2crshuwao.html

[U67] PHP：处理文件上传
来源：http://www.52xcode.cn/Article/details/gt2gowzysqc.html

$_FILES["file"]["tmp_name"] 与 move_uploaded_file()
来源：http://www.52xcode.cn/Article/details/gt2qohfzyru.html

[U68] PHP：PDO 连接
来源：http://www.ydjk.org.cn/Article/details/gt2fsagcabu.html

$pdo = new PDO("mysql:host=localhost;dbname=app", "root", "");
来源：http://www.52xcode.cn/Article/details/gt2gtgwprsc.html

[U69] PHP：PDO 预处理
来源：http://www.52xcode.cn/Article/details/gt2qjgcvejo.html

$stmt = $pdo->prepare("SELECT * FROM users WHERE id = ?");  $stmt->execute([$id]);
来源：http://www.ydjk.org.cn/Article/details/gt2bvkfflja.html

[U70] PHP：PDO 事务
来源：http://www.ydjk.org.cn/Article/details/gt2xhcrokdi.html

$pdo->beginTransaction();  $pdo->commit();  $pdo->rollBack();
来源：http://www.52xcode.cn/Article/details/gt2ezufppzh.html

[U71] PHP：抛出异常
来源：http://www.52xcode.cn/Article/details/gt2bpfaaeqk.html

throw new RuntimeException("失败", 500);
来源：http://www.52xcode.cn/Article/details/gt2bptooydh.html

[U72] PHP：写错误日志
来源：http://www.ydjk.org.cn/Article/details/gt2rkwqcoua.html

error_log("失败: " . $e->getMessage());
来源：http://www.ydjk.org.cn/Article/details/gt2bxfvkjpl.html

[U73] PHP：读取 ini 配置
来源：http://www.52xcode.cn/Article/details/gt2hxxutbcq.html

parse_ini_file("config.ini", true)
来源：http://www.52xcode.cn/Article/details/gt2mwnwgdfr.html

[U74] PHP：读取环境变量
来源：http://www.ydjk.org.cn/Article/details/gt2zpblrmer.html

getenv("APP_ENV") ?: "production"
来源：http://www.ydjk.org.cn/Article/details/gt2tzahlbey.html

[U75] PHP：依赖注入
来源：http://www.ydjk.org.cn/Article/details/gt2bhepxfno.html

composer require psr/container
来源：http://www.52xcode.cn/Article/details/gt2rlupexhs.html

[U76] PHP：简单路由
来源：http://www.ydjk.org.cn/Article/details/gt2jnupsjht.html

$path = parse_url($_SERVER["REQUEST_URI"], PHP_URL_PATH);
来源：http://www.52xcode.cn/Article/details/gt2zslmqyrq.html

[U77] PHP：模板渲染
来源：http://www.52xcode.cn/Article/details/gt2wvmbdbcx.html

composer require twig/twig
来源：http://www.52xcode.cn/Article/details/gt2eieifree.html

[U78] PHP：单元测试
来源：http://www.52xcode.cn/Article/details/gt2hirymuwv.html

composer require --dev phpunit/phpunit
来源：http://www.ydjk.org.cn/Article/details/gt2pickxpyl.html

[U79] PHP：静态分析
来源：http://www.ydjk.org.cn/Article/details/gt2elpocywy.html

composer require --dev phpstan/phpstan
来源：http://www.52xcode.cn/Article/details/gt2ubvuagud.html

[U80] PHP：代码规范修复
来源：http://www.52xcode.cn/Article/details/gt2ccsxicqg.html

composer require --dev friendsofphp/php-cs-fixer
来源：http://www.52xcode.cn/Article/details/gt2sjgjxpax.html

[U81] JS：初始化项目
来源：http://www.52xcode.cn/Article/details/gt2eihdmlos.html

npm init -y;  npm i express
来源：http://www.52xcode.cn/Article/details/gt2hnjhhaxk.html

[U82] JS：package.json 脚本
来源：http://www.52xcode.cn/Article/details/gt2nhhdcypa.html

"scripts": { "dev": "vite", "build": "vite build" }
来源：http://www.52xcode.cn/Article/details/gt2nnrwghzc.html

[U83] JS：ES Module 导入导出
来源：http://www.52xcode.cn/Article/details/gt2eqnglmgj.html

export const a = 1;  import { a } from "./m.js";
来源：http://www.52xcode.cn/Article/details/gt2bjbaykdt.html

[U84] JS：CommonJS 写法
来源：http://www.ydjk.org.cn/Article/details/gt2worsdfue.html

module.exports = { a };  const { a } = require("./m");
来源：http://www.52xcode.cn/Article/details/gt2tvpzbigw.html

[U85] JS：可选链
来源：http://www.ydjk.org.cn/Article/details/gt2izkbqvac.html

a?.b?.c
来源：http://www.52xcode.cn/Article/details/gt2hcgwcsqf.html

[U86] JS：空值合并
来源：http://www.52xcode.cn/Article/details/gt2kweebftw.html

a ?? b
来源：http://www.52xcode.cn/Article/details/gt2iqcctjmc.html

[U87] JS：解构默认值
来源：http://www.ydjk.org.cn/Article/details/gt2hgvayvbc.html

const { a = 1, b = 2 } = obj;
来源：http://www.ydjk.org.cn/Article/details/gt2hkzazccg.html

[U88] JS：对象展开合并
来源：http://www.52xcode.cn/Article/details/gt2dkdgqyhj.html

{ ...a, ...b }
来源：http://www.52xcode.cn/Article/details/gt2anorblyp.html

[U89] JS：数组去重
来源：http://www.ydjk.org.cn/Article/details/gt2gpotfozc.html

[...new Set(arr)]
来源：http://www.52xcode.cn/Article/details/gt2kscgukgx.html

[U90] JS：数字数组排序
来源：http://www.ydjk.org.cn/Article/details/gt2nxqcvvhi.html

[...arr].sort((a, b) => a - b)
来源：http://www.52xcode.cn/Article/details/gt2xrgsvahp.html

[U91] JS：对象键值遍历
来源：http://www.ydjk.org.cn/Article/details/gt2kxroonkt.html

Object.entries(obj).forEach(([k, v]) => {});
来源：http://www.52xcode.cn/Article/details/gt2mqhxhqnf.html

[U92] JS：深拷贝
来源：http://www.52xcode.cn/Article/details/gt2gjqhwlke.html

structuredClone(obj)
来源：http://www.ydjk.org.cn/Article/details/gt2qnudbtse.html

[U93] JS：模板字符串
来源：http://www.52xcode.cn/Article/details/gt2gqhdbkio.html

`共 ${n} 条`
来源：http://www.52xcode.cn/Article/details/gt2bbujckso.html

[U94] JS：箭头函数
来源：http://www.ydjk.org.cn/Article/details/gt2sjolowdm.html

const double = x => x * 2;
来源：http://www.52xcode.cn/Article/details/gt2tommixsn.html

[U95] JS：Promise 包装
来源：http://www.52xcode.cn/Article/details/gt2bmddzxbr.html

new Promise((resolve, reject) => {})
来源：http://www.ydjk.org.cn/Article/details/gt2okcdnyti.html

[U96] JS：async/await 与异常
来源：http://www.ydjk.org.cn/Article/details/gt2ueuyijeo.html

try { const d = await f(); } catch (e) { console.error(e); }
来源：http://www.52xcode.cn/Article/details/gt2awnzhhmj.html

[U97] JS：并发请求
来源：http://www.ydjk.org.cn/Article/details/gt2kcffkljl.html

await Promise.all(urls.map(u => fetch(u)))
来源：http://www.ydjk.org.cn/Article/details/gt2vayembla.html

[U98] JS：fetch 带 JSON
来源：http://www.ydjk.org.cn/Article/details/gt2cukzlhvl.html

await fetch(url, { method: "POST", headers: { "Content-Type": "application/json" }, body: JSON.stringify(d) })
来源：http://www.ydjk.org.cn/Article/details/gt2wlnnbxmk.html

[U99] JS：事件监听
来源：http://www.52xcode.cn/Article/details/gt2onsjdifs.html

el.addEventListener("click", e => {})
来源：http://www.ydjk.org.cn/Article/details/gt2ajswodhv.html

[U100] JS：DOM 查询
来源：http://www.ydjk.org.cn/Article/details/gt2imgmicyb.html

document.querySelector(".item")
来源：http://www.ydjk.org.cn/Article/details/gt2igcawyin.html

[U101] JS：classList 操作
来源：http://www.ydjk.org.cn/Article/details/gt2kiaojuft.html

el.classList.toggle("active")
来源：http://www.ydjk.org.cn/Article/details/gt2ykvbwlnc.html

[U102] JS：本地存储
来源：http://www.ydjk.org.cn/Article/details/gt2vkdxaxoy.html

localStorage.setItem("k", JSON.stringify(v))
来源：http://www.ydjk.org.cn/Article/details/gt2kgewrnhm.html

[U103] JS：定时器
来源：http://www.52xcode.cn/Article/details/gt2ygdepjui.html

setTimeout(fn, 1000);  setInterval(fn, 1000);
来源：http://www.52xcode.cn/Article/details/gt2vuksjcei.html

[U104] JS：防抖
来源：http://www.52xcode.cn/Article/details/gt2fngrjhtq.html

const debounce = (fn, ms) => { let t; return (...a) => { clearTimeout(t); t = setTimeout(() => fn(...a), ms); }; };
来源：http://www.52xcode.cn/Article/details/gt2tildlory.html

[U105] JS：节流
来源：http://www.52xcode.cn/Article/details/gt2hwwvyunb.html

const throttle = (fn, ms) => { let last = 0; return (...a) => { const n = Date.now(); if (n - last >= ms) { last = n; fn(...a); } }; };
来源：http://www.ydjk.org.cn/Article/details/gt2krxjgvmb.html

[U106] JS：日期格式化
来源：http://www.52xcode.cn/Article/details/gt2cmvqbxxj.html

new Intl.DateTimeFormat("zh-CN", { dateStyle: "medium" }).format(new Date())
来源：http://www.52xcode.cn/Article/details/gt2ypslable.html

[U107] JS：数字千分位
来源：http://www.52xcode.cn/Article/details/gt2ndefslxn.html

new Intl.NumberFormat("en-US").format(1234567)
来源：http://www.ydjk.org.cn/Article/details/gt2vgxfhtrk.html

[U108] JS：随机整数
来源：http://www.52xcode.cn/Article/details/gt2mcmjfdhu.html

Math.floor(Math.random() * (max - min + 1)) + min
来源：http://www.ydjk.org.cn/Article/details/gt2oggosjyd.html

[U109] JS：数组分组
来源：http://www.ydjk.org.cn/Article/details/gt2iujcfljw.html

Object.groupBy(arr, x => x.type)
来源：http://www.ydjk.org.cn/Article/details/gt2xifsnkyi.html

[U110] JS：数组分块
来源：http://www.52xcode.cn/Article/details/gt2jpqehupp.html

arr.reduce((acc, x, i) => (i % size ? acc : [...acc, arr.slice(i, i + size)]), [])
来源：http://www.52xcode.cn/Article/details/gt2nzirsver.html

[U111] JS：对象转 Map
来源：http://www.52xcode.cn/Article/details/gt2zvuwvlkl.html

new Map(Object.entries(obj))
来源：http://www.ydjk.org.cn/Article/details/gt2nbvlktho.html

[U112] JS：字符串补位
来源：http://www.52xcode.cn/Article/details/gt2hmffgwum.html

"7".padStart(3, "0")
来源：http://www.ydjk.org.cn/Article/details/gt2acymhgwa.html

[U113] JS：正则替换全部
来源：http://www.ydjk.org.cn/Article/details/gt2arcopgkx.html

s.replaceAll("a", "b")
来源：http://www.ydjk.org.cn/Article/details/gt2lirokegc.html

[U114] JS：JSON 深比较
来源：http://www.ydjk.org.cn/Article/details/gt2jxzbgnga.html

JSON.stringify(a) === JSON.stringify(b)
来源：http://www.52xcode.cn/Article/details/gt2motbsggi.html


<!-- 参考信息 -->