代发 wailian999

[T35] Lua：字典表
来源：http://www.52xcode.cn/Article/details/gt3epidbojg.html

local d = { a = 1 };  d.b = 2
来源：http://www.52xcode.cn/Article/details/gt3rqappjog.html

[T36] Lua：函数
来源：http://www.ydjk.org.cn/Article/details/gt3xktyhifb.html

function add(a, b) return a + b end
来源：http://www.ydjk.org.cn/Article/details/gt3hvqtvpxy.html

[T37] Lua：字符串拼接
来源：http://www.ydjk.org.cn/Article/details/gt3iibaexgc.html

"a" .. "b"
来源：http://www.ydjk.org.cn/Article/details/gt3ajyoysav.html

[T38] Lua：条件
来源：http://www.ydjk.org.cn/Article/details/gt3rowrpnjd.html

if x > 0 then print("正") end
来源：http://www.ydjk.org.cn/Article/details/gt3kaiyqumn.html

[T39] Lua：模式匹配
来源：http://www.52xcode.cn/Article/details/gt3sbbhrqmw.html

string.find(s, "%d+")
来源：http://www.52xcode.cn/Article/details/gt3wfhotnuf.html

[T40] Lua：元表
来源：http://www.52xcode.cn/Article/details/gt3wndmofsy.html

setmetatable({}, { __index = base })
来源：http://www.ydjk.org.cn/Article/details/gt3jvoybfgt.html

[T41] Perl：Hello World
来源：http://www.ydjk.org.cn/Article/details/gt3pvysqjxa.html

print "Hello\n";
来源：http://www.ydjk.org.cn/Article/details/gt3idqcajkd.html

[T42] Perl：变量类型
来源：http://www.ydjk.org.cn/Article/details/gt3exsscxph.html

my $a = 1;  my @arr = (1, 2, 3);  my %h = (a => 1);
来源：http://www.52xcode.cn/Article/details/gt3daihljxk.html

[T43] Perl：字符串插值
来源：http://www.52xcode.cn/Article/details/gt3xsgubocv.html

"值: $a"
来源：http://www.ydjk.org.cn/Article/details/gt3pucdtdew.html

[T44] Perl：条件
来源：http://www.52xcode.cn/Article/details/gt3ljiczqkx.html

if ($a > 0) { print "正"; }
来源：http://www.ydjk.org.cn/Article/details/gt3bdcyeyrd.html

[T45] Perl：数组遍历
来源：http://www.ydjk.org.cn/Article/details/gt3uaicxzam.html

for my $x (@arr) { print $x; }
来源：http://www.52xcode.cn/Article/details/gt3bjadbyzo.html

[T46] Perl：哈希操作
来源：http://www.52xcode.cn/Article/details/gt3enhmyale.html

$h{b} = 2;  for my $k (keys %h) { print "$k=$h{$k}"; }
来源：http://www.52xcode.cn/Article/details/gt3wvrbvter.html

[T47] Perl：正则捕获
来源：http://www.52xcode.cn/Article/details/gt3uzpjmify.html

if ($s =~ /(\d+)/) { print $1; }
来源：http://www.ydjk.org.cn/Article/details/gt3dmxnklym.html

[T48] Perl：正则替换
来源：http://www.52xcode.cn/Article/details/gt3qfbanbhe.html

$s =~ s/old/new/g;
来源：http://www.ydjk.org.cn/Article/details/gt3gpinaosr.html

[T49] Perl：函数
来源：http://www.52xcode.cn/Article/details/gt3wwyhegqd.html

sub add { my ($a, $b) = @_; return $a + $b; }
来源：http://www.ydjk.org.cn/Article/details/gt3hzdlruzt.html

[T50] Perl：逐行读文件
来源：http://www.52xcode.cn/Article/details/gt3jlewigot.html

open my $fh, "<", "a.txt" or die $!;
来源：http://www.ydjk.org.cn/Article/details/gt3hgbnbdoh.html

while (my $line = <$fh>) { print $line; }
来源：http://www.52xcode.cn/Article/details/gt3uzszeioz.html

[T51] Scala：Hello World
来源：http://www.ydjk.org.cn/Article/details/gt3xwsdjzzg.html

println("Hello")
来源：http://www.52xcode.cn/Article/details/gt3mcxhullt.html

[T52] Scala：变量
来源：http://www.ydjk.org.cn/Article/details/gt3dqxfagrt.html

val a = 1;  var b = 2
来源：http://www.ydjk.org.cn/Article/details/gt3xhsdcftj.html

[T53] Scala：字符串插值
来源：http://www.52xcode.cn/Article/details/gt3gihnkgjy.html

s"值: $b"
来源：http://www.52xcode.cn/Article/details/gt3unrfnioy.html

[T54] Scala：集合映射
来源：http://www.52xcode.cn/Article/details/gt3hgrsuafr.html

List(1, 2, 3).map(_ * 2)
来源：http://www.ydjk.org.cn/Article/details/gt3iuxdikov.html

[T55] Scala：集合过滤
来源：http://www.52xcode.cn/Article/details/gt3tttisgqy.html

List(1, 2, 3).filter(_ > 1)
来源：http://www.52xcode.cn/Article/details/gt3zorndkna.html

[T56] Scala：样例类
来源：http://www.52xcode.cn/Article/details/gt3jbuzjdun.html

case class User(name: String, age: Int)
来源：http://www.52xcode.cn/Article/details/gt3vghfzilu.html

[T57] Scala：模式匹配
来源：http://www.ydjk.org.cn/Article/details/gt3sekwolfn.html

x match { case 1 => "一"; case _ => "其他" }
来源：http://www.52xcode.cn/Article/details/gt3exoyutuk.html

[T58] Scala：函数定义
来源：http://www.52xcode.cn/Article/details/gt3rzjuoplo.html

def add(a: Int, b: Int): Int = a + b
来源：http://www.ydjk.org.cn/Article/details/gt3auvluxdu.html

[T59] Scala：循环
来源：http://www.52xcode.cn/Article/details/gt3jmwvygdp.html

for (i <- 1 to 10) println(i)
来源：http://www.ydjk.org.cn/Article/details/gt3gmkyflwq.html

[T60] Scala：折叠
来源：http://www.52xcode.cn/Article/details/gt3kvnzwlzk.html

List(1, 2, 3).foldLeft(0)(_ + _)
来源：http://www.52xcode.cn/Article/details/gt3nhkvpmjt.html

================================================================================
来源：http://www.ydjk.org.cn/Article/details/gt3xebpymnf.html

U. 高频实用片段（Python / PHP / JavaScript 各 40 条）
来源：http://www.ydjk.org.cn/Article/details/gt3zpaevutg.html

================================================================================
来源：http://www.ydjk.org.cn/Article/details/gt3iwslupnz.html

[U01] Py：创建虚拟环境
来源：http://www.52xcode.cn/Article/details/gt3yaapvbyv.html

python -m venv .venv && source .venv/bin/activate
来源：http://www.52xcode.cn/Article/details/gt3cyrmfxlu.html

[U02] Py：导出 / 安装依赖
来源：http://www.52xcode.cn/Article/details/gt3lnlevqax.html

pip freeze > requirements.txt;  pip install -r requirements.txt
来源：http://www.ydjk.org.cn/Article/details/gt3ryvhxdkd.html

[U03] Py：加载 .env 配置
来源：http://www.52xcode.cn/Article/details/gt3wnkfgggw.html

from dotenv import load_dotenv; load_dotenv()
来源：http://www.52xcode.cn/Article/details/gt3kbchnsvv.html

[U04] Py：变量调试打印
来源：http://www.52xcode.cn/Article/details/gt3wyyhkkfh.html

print(f"{x=}")            # 输出 x=值，Python 3.8+
来源：http://www.ydjk.org.cn/Article/details/gt3uefxialb.html

[U05] Py：列表去重且保序
来源：http://www.52xcode.cn/Article/details/gt3wbvjiapf.html

list(dict.fromkeys(arr))
来源：http://www.52xcode.cn/Article/details/gt3utueoitn.html

[U06] Py：合并两个字典
来源：http://www.ydjk.org.cn/Article/details/gt3zvrlcfgq.html

{**a, **b}
来源：http://www.ydjk.org.cn/Article/details/gt3mvnwsdju.html

[U07] Py：反转字典键值
来源：http://www.ydjk.org.cn/Article/details/gt3lqgjcsbx.html

{v: k for k, v in d.items()}
来源：http://www.52xcode.cn/Article/details/gt3ufedzfvk.html

[U08] Py：展平二维列表
来源：http://www.52xcode.cn/Article/details/gt3rrfgaxao.html

[y for x in nested for y in x]
来源：http://www.52xcode.cn/Article/details/gt3qhrtnedu.html

[U09] Py：字典取最大值的键
来源：http://www.52xcode.cn/Article/details/gt3iqliirwr.html

max(d, key=d.get)
来源：http://www.52xcode.cn/Article/details/gt3uqiqdbdv.html

[U10] Py：按值排序字典
来源：http://www.ydjk.org.cn/Article/details/gt3wtqdxjni.html

dict(sorted(d.items(), key=lambda kv: kv[1]))
来源：http://www.52xcode.cn/Article/details/gt3bizsgimm.html

[U11] Py：生成器表达式
来源：http://www.52xcode.cn/Article/details/gt3tlvjpvwt.html

(x * 2 for x in arr)
来源：http://www.ydjk.org.cn/Article/details/gt3dqfcwrgm.html

[U12] Py：取出现最多的 3 个元素
来源：http://www.52xcode.cn/Article/details/gt3ftafipah.html

Counter(arr).most_common(3)
来源：http://www.52xcode.cn/Article/details/gt3qhyvnfma.html

[U13] Py：固定长度队列
来源：http://www.ydjk.org.cn/Article/details/gt3ngldyqmi.html

deque(maxlen=10)
来源：http://www.52xcode.cn/Article/details/gt3vdrysekn.html

[U14] Py：分组收集到列表
来源：http://www.ydjk.org.cn/Article/details/gt3wyediksz.html

defaultdict(list)
来源：http://www.52xcode.cn/Article/details/gt3dycrocyj.html

[U15] Py：高精度计时
来源：http://www.52xcode.cn/Article/details/gt3duqpgvkv.html

t = time.perf_counter()
来源：http://www.ydjk.org.cn/Article/details/gt3jyuhbfnd.html

[U16] Py：命令行参数解析
来源：http://www.ydjk.org.cn/Article/details/gt3cayttycb.html

ap = argparse.ArgumentParser();  ap.add_argument("--name");  args = ap.parse_args()
来源：http://www.52xcode.cn/Article/details/gt3rwmjlmzk.html

[U17] Py：初始化日志
来源：http://www.ydjk.org.cn/Article/details/gt3fbinolqz.html

logging.basicConfig(level=logging.INFO)
来源：http://www.ydjk.org.cn/Article/details/gt3sxakrqba.html

[U18] Py：预编译正则
来源：http://www.ydjk.org.cn/Article/details/gt3gudhxjea.html

pat = re.compile(r"\d+")
来源：http://www.ydjk.org.cn/Article/details/gt3kcblavpp.html

[U19] Py：正则替换带回调
来源：http://www.ydjk.org.cn/Article/details/gt3ixlpfqrh.html

re.sub(r"\d+", lambda m: str(int(m.group()) * 2), s)
来源：http://www.ydjk.org.cn/Article/details/gt3syrmtuyj.html

[U20] Py：缓存函数结果
来源：http://www.52xcode.cn/Article/details/gt3vgfubqdk.html

@functools.lru_cache(maxsize=None)
来源：http://www.ydjk.org.cn/Article/details/gt3gddvqsln.html

[U21] Py：自定义上下文管理器
来源：http://www.52xcode.cn/Article/details/gt3qdwsakxo.html

@contextlib.contextmanager
来源：http://www.ydjk.org.cn/Article/details/gt3gboomngt.html

[U22] Py：矩阵转置
来源：http://www.ydjk.org.cn/Article/details/gt3wkmibqcd.html

list(zip(*m))
来源：http://www.52xcode.cn/Article/details/gt3jfygatvj.html

[U23] Py：分块读取大文件
来源：http://www.ydjk.org.cn/Article/details/gt3ehyvsqzt.html

for chunk in iter(lambda: f.read(8192), b""):
来源：http://www.52xcode.cn/Article/details/gt3tnbypjgw.html

[U24] Py：路径操作
来源：http://www.ydjk.org.cn/Article/details/gt3rbhopmbs.html

Path("a/b.txt").parent.mkdir(parents=True, exist_ok=True)
来源：http://www.ydjk.org.cn/Article/details/gt3uethcptx.html

[U25] Py：CSV 按字典读
来源：http://www.52xcode.cn/Article/details/gt3hmoefvdd.html

csv.DictReader(f)
来源：http://www.52xcode.cn/Article/details/gt3snxbfhxl.html

[U26] Py：并发下载
来源：http://www.ydjk.org.cn/Article/details/gt3yusqrauo.html

ThreadPoolExecutor(max_workers=8).map(fetch, urls)
来源：http://www.ydjk.org.cn/Article/details/gt3ubaqyuhp.html

[U27] Py：异步 HTTP
来源：http://www.52xcode.cn/Article/details/gt3quxtbcta.html

aiohttp.ClientSession() 配合 async with
来源：http://www.ydjk.org.cn/Article/details/gt3xtnkaedx.html

[U28] Py：类型别名
来源：http://www.52xcode.cn/Article/details/gt3doqnpgnn.html

UserId = int
来源：http://www.ydjk.org.cn/Article/details/gt3avcqqtsh.html

[U29] Py：属性校验
来源：http://www.ydjk.org.cn/Article/details/gt3xvzxhkno.html

@property 与 @x.setter 配合
来源：http://www.ydjk.org.cn/Article/details/gt3jdevittz.html

[U30] Py：数据类
来源：http://www.ydjk.org.cn/Article/details/gt3iezbmcsi.html

@dataclass(slots=True)
来源：http://www.52xcode.cn/Article/details/gt3oalgbbfn.html

[U31] Py：单测
来源：http://www.ydjk.org.cn/Article/details/gt3gdvhsxmg.html

python -m pytest -q
来源：http://www.52xcode.cn/Article/details/gt3bmkawavb.html

[U32] Py：代码格式化
来源：http://www.ydjk.org.cn/Article/details/gt3reblzrgb.html

ruff format . && ruff check --fix .
来源：http://www.52xcode.cn/Article/details/gt3htebggav.html

[U33] Py：打包发布
来源：http://www.ydjk.org.cn/Article/details/gt3nvnuhsuh.html

python -m build  （依赖 pyproject.toml）
来源：http://www.ydjk.org.cn/Article/details/gt3gucxgsdi.html

[U34] Py：判断编码
来源：http://www.52xcode.cn/Article/details/gt3nfolvkdk.html

chardet.detect(raw)
来源：http://www.ydjk.org.cn/Article/details/gt3kkictbxc.html

[U35] Py：发送邮件
来源：http://www.ydjk.org.cn/Article/details/gt3qqenqlnq.html

smtplib.SMTP_SSL(...).send_message(msg)
来源：http://www.52xcode.cn/Article/details/gt3stonerza.html

[U36] Py：定时任务
来源：http://www.ydjk.org.cn/Article/details/gt3djtkggjv.html

schedule.every(10).minutes.do(job)
来源：http://www.52xcode.cn/Article/details/gt3zguovlhc.html

[U37] Py：读写 Excel
来源：http://www.52xcode.cn/Article/details/gt3oazqvmvx.html

pandas.read_excel / DataFrame.to_excel
来源：http://www.ydjk.org.cn/Article/details/gt3toefzxzs.html

[U38] Py：获取脚本所在目录
来源：http://www.52xcode.cn/Article/details/gt3nafpgzyh.html

Path(__file__).resolve().parent
来源：http://www.ydjk.org.cn/Article/details/gt3sygjphte.html

[U39] Py：判断是否在交互环境
来源：http://www.ydjk.org.cn/Article/details/gt3vepvznid.html

sys.stdout.isatty()
来源：http://www.52xcode.cn/Article/details/gt3npvyahhk.html

[U40] Py：打印到标准错误
来源：http://www.52xcode.cn/Article/details/gt3ihladgpz.html

print("err", file=sys.stderr)
来源：http://www.52xcode.cn/Article/details/gt3gpbkshso.html

[U41] PHP：初始化 Composer 项目
来源：http://www.52xcode.cn/Article/details/gt3jpkfnqpb.html

composer init;  composer require guzzlehttp/guzzle
来源：http://www.52xcode.cn/Article/details/gt3xhaktazz.html

[U42] PHP：PSR-4 自动加载
来源：http://www.52xcode.cn/Article/details/gt3ogipzwoq.html

"autoload": { "psr-4": { "App\\": "src/" } }
来源：http://www.ydjk.org.cn/Article/details/gt3qsqmvcvc.html

[U43] PHP：声明命名空间
来源：http://www.ydjk.org.cn/Article/details/gt3qlznsqbb.html

namespace App\Http;
来源：http://www.52xcode.cn/Article/details/gt3tgdhhhvd.html

[U44] PHP：开启严格类型
来源：http://www.ydjk.org.cn/Article/details/gt3ipbymwgh.html

declare(strict_types=1);
来源：http://www.ydjk.org.cn/Article/details/gt3brrvzfro.html

[U45] PHP：类型声明与返回类型
来源：http://www.ydjk.org.cn/Article/details/gt3ohrkxxnd.html

function add(int $a, int $b): int { return $a + $b; }
来源：http://www.ydjk.org.cn/Article/details/gt3xqxupcso.html

[U46] PHP：可空类型
来源：http://www.ydjk.org.cn/Article/details/gt3uqvtpxsw.html

?string $name = null
来源：http://www.ydjk.org.cn/Article/details/gt3xhcqgfqx.html

[U47] PHP：联合类型
来源：http://www.ydjk.org.cn/Article/details/gt3hqzdbrdc.html

int|string $id
来源：http://www.52xcode.cn/Article/details/gt3wqwefaci.html

[U48] PHP：纯枚举
来源：http://www.52xcode.cn/Article/details/gt3pthyfdja.html

enum Status: string { case Active = "active"; case Off = "off"; }
来源：http://www.52xcode.cn/Article/details/gt3sfmiykwq.html

[U49] PHP：只读属性
来源：http://www.ydjk.org.cn/Article/details/gt3ycfqqniy.html

public readonly string $name
来源：http://www.ydjk.org.cn/Article/details/gt3wjkpijxz.html

[U50] PHP：构造器属性提升
来源：http://www.ydjk.org.cn/Article/details/gt3ojrojwdm.html

public function __construct(private int $id) {}
来源：http://www.ydjk.org.cn/Article/details/gt3zjhrxeoq.html

[U51] PHP：数组解构
来源：http://www.ydjk.org.cn/Article/details/gt3ozhtwpat.html

[$a, $b] = $arr;
来源：http://www.52xcode.cn/Article/details/gt3mrzmajwj.html

[U52] PHP：箭头函数
来源：http://www.ydjk.org.cn/Article/details/gt3iamebzeb.html

$double = fn($x) => $x * 2;
来源：http://www.52xcode.cn/Article/details/gt3qxfduopf.html

[U53] PHP：空合并运算符
来源：http://www.ydjk.org.cn/Article/details/gt3uzugstjk.html

$v = $a ?? $b ?? "default";
来源：http://www.ydjk.org.cn/Article/details/gt3aynamecb.html

[U54] PHP：空安全调用
来源：http://www.52xcode.cn/Article/details/gt3aambassx.html

$obj?->method()
来源：http://www.52xcode.cn/Article/details/gt3fikmryag.html

[U55] PHP：match 表达式
来源：http://www.52xcode.cn/Article/details/gt3hnjcjlwo.html

$s = match($x) { 1 => "一", default => "其他" };
来源：http://www.52xcode.cn/Article/details/gt3lokuqquw.html

[U56] PHP：命名参数
来源：http://www.ydjk.org.cn/Article/details/gt3elwmyxjx.html

f(a: 1, b: 2)
来源：http://www.ydjk.org.cn/Article/details/gt3wrtphhzm.html

[U57] PHP：字符串插值
来源：http://www.ydjk.org.cn/Article/details/gt3fbznpbxm.html

"值: {$a}"
来源：http://www.ydjk.org.cn/Article/details/gt3kgzrusra.html

[U58] PHP：数组三件套
来源：http://www.ydjk.org.cn/Article/details/gt3hrnyuetq.html

array_map($f, $a);  array_filter($a, $f);  array_reduce($a, $f, 0);
来源：http://www.ydjk.org.cn/Article/details/gt3ujizbesv.html

[U59] PHP：自定义排序
来源：http://www.52xcode.cn/Article/details/gt3hsunmkgd.html

usort($arr, fn($a, $b) => $a["age"] <=> $b["age"]);
来源：http://www.ydjk.org.cn/Article/details/gt3etxectgp.html

[U60] PHP：JSON 编解码
来源：http://www.ydjk.org.cn/Article/details/gt3agvzuolr.html

json_encode($d, JSON_UNESCAPED_UNICODE);  json_decode($s, true);
来源：http://www.52xcode.cn/Article/details/gt3ofzyupek.html

[U61] PHP：正则
来源：http://www.ydjk.org.cn/Article/details/gt3jblunbgr.html

preg_match('/(\d+)/', $s, $m);  preg_replace('/\d+/', '#', $s);
来源：http://www.ydjk.org.cn/Article/details/gt3zofuzzkh.html

[U62] PHP：日期对象
来源：http://www.52xcode.cn/Article/details/gt3hvsebqgu.html

(new DateTimeImmutable())->format("Y-m-d");
来源：http://www.52xcode.cn/Article/details/gt3muoaibta.html

[U63] PHP：文件读写
来源：http://www.52xcode.cn/Article/details/gt3qnrgppyx.html

file_get_contents($f);  file_put_contents($f, $data);
来源：http://www.52xcode.cn/Article/details/gt3chxthzlq.html

[U64] PHP：目录遍历
来源：http://www.ydjk.org.cn/Article/details/gt3jcykietg.html

glob("dir/*.php");  scandir("dir");
来源：http://www.ydjk.org.cn/Article/details/gt3oswyyfjm.html

[U65] PHP：会话
来源：http://www.ydjk.org.cn/Article/details/gt3pvvkclxo.html

session_start();  $_SESSION["uid"] = 1;
来源：http://www.52xcode.cn/Article/details/gt3cwzodqwj.html

[U66] PHP：设置 Cookie
来源：http://www.52xcode.cn/Article/details/gt3ilbcxece.html

setcookie("token", $v, ["httponly" => true, "samesite" => "Lax"]);
来源：http://www.52xcode.cn/Article/details/gt3qavumzsa.html

[U67] PHP：处理文件上传
来源：http://www.ydjk.org.cn/Article/details/gt3wfqnrogf.html

$_FILES["file"]["tmp_name"] 与 move_uploaded_file()
来源：http://www.ydjk.org.cn/Article/details/gt3kiqacizh.html

[U68] PHP：PDO 连接
来源：http://www.ydjk.org.cn/Article/details/gt3dhbqgzle.html

$pdo = new PDO("mysql:host=localhost;dbname=app", "root", "");
来源：http://www.ydjk.org.cn/Article/details/gt3silzlffr.html

[U69] PHP：PDO 预处理
来源：http://www.52xcode.cn/Article/details/gt3abidsssj.html

$stmt = $pdo->prepare("SELECT * FROM users WHERE id = ?");  $stmt->execute([$id]);
来源：http://www.ydjk.org.cn/Article/details/gt3iepvveyd.html

[U70] PHP：PDO 事务
来源：http://www.ydjk.org.cn/Article/details/gt3ugqamkii.html

$pdo->beginTransaction();  $pdo->commit();  $pdo->rollBack();
来源：http://www.52xcode.cn/Article/details/gt3qfdzwisa.html

[U71] PHP：抛出异常
来源：http://www.52xcode.cn/Article/details/gt3obxcnctd.html

throw new RuntimeException("失败", 500);
来源：http://www.52xcode.cn/Article/details/gt3vmcyhwrr.html

[U72] PHP：写错误日志
来源：http://www.ydjk.org.cn/Article/details/gt3kladdrxa.html

error_log("失败: " . $e->getMessage());
来源：http://www.ydjk.org.cn/Article/details/gt3vwmmdnsh.html

[U73] PHP：读取 ini 配置
来源：http://www.52xcode.cn/Article/details/gt3ikowznrj.html

parse_ini_file("config.ini", true)
来源：http://www.52xcode.cn/Article/details/gt3njjjjbql.html

[U74] PHP：读取环境变量
来源：http://www.ydjk.org.cn/Article/details/gt3kczmmjlp.html

getenv("APP_ENV") ?: "production"
来源：http://www.52xcode.cn/Article/details/gt3zbulcbew.html

[U75] PHP：依赖注入
来源：http://www.ydjk.org.cn/Article/details/gt3kgcjnoar.html

composer require psr/container
来源：http://www.52xcode.cn/Article/details/gt3vdgmwjqo.html

[U76] PHP：简单路由
来源：http://www.52xcode.cn/Article/details/gt3tzrpqzrr.html

$path = parse_url($_SERVER["REQUEST_URI"], PHP_URL_PATH);
来源：http://www.ydjk.org.cn/Article/details/gt3ssxabwqt.html

[U77] PHP：模板渲染
来源：http://www.52xcode.cn/Article/details/gt3kdurykqp.html

composer require twig/twig
来源：http://www.52xcode.cn/Article/details/gt3jplgumdo.html

[U78] PHP：单元测试
来源：http://www.ydjk.org.cn/Article/details/gt3gxsrsqse.html

composer require --dev phpunit/phpunit
来源：http://www.ydjk.org.cn/Article/details/gt3mizhfwve.html

[U79] PHP：静态分析
来源：http://www.ydjk.org.cn/Article/details/gt3pdsbxlkm.html

composer require --dev phpstan/phpstan
来源：http://www.52xcode.cn/Article/details/gt3ogschekb.html

[U80] PHP：代码规范修复
来源：http://www.52xcode.cn/Article/details/gt3hodotajv.html

composer require --dev friendsofphp/php-cs-fixer
来源：http://www.52xcode.cn/Article/details/gt3vgxkxese.html

[U81] JS：初始化项目
来源：http://www.52xcode.cn/Article/details/gt3kxgeoukq.html

npm init -y;  npm i express
来源：http://www.ydjk.org.cn/Article/details/gt3egqruzjg.html

[U82] JS：package.json 脚本
来源：http://www.52xcode.cn/Article/details/gt3eggjwfbm.html

"scripts": { "dev": "vite", "build": "vite build" }
来源：http://www.ydjk.org.cn/Article/details/gt3hjsrrmxe.html

[U83] JS：ES Module 导入导出
来源：http://www.ydjk.org.cn/Article/details/gt3gpwdapya.html

export const a = 1;  import { a } from "./m.js";
来源：http://www.ydjk.org.cn/Article/details/gt3chbrczxe.html

[U84] JS：CommonJS 写法
来源：http://www.ydjk.org.cn/Article/details/gt3rqbgzgaz.html

module.exports = { a };  const { a } = require("./m");
来源：http://www.52xcode.cn/Article/details/gt3vcqqmgxg.html

[U85] JS：可选链
来源：http://www.52xcode.cn/Article/details/gt3cpluqgoq.html

a?.b?.c
来源：http://www.ydjk.org.cn/Article/details/gt3iotjsfzq.html

[U86] JS：空值合并
来源：http://www.ydjk.org.cn/Article/details/gt3wetssfsh.html

a ?? b
来源：http://www.52xcode.cn/Article/details/gt3vuwyeaov.html

[U87] JS：解构默认值
来源：http://www.52xcode.cn/Article/details/gt3erwpdvpq.html

const { a = 1, b = 2 } = obj;
来源：http://www.52xcode.cn/Article/details/gt3kxxgtvtr.html

[U88] JS：对象展开合并
来源：http://www.52xcode.cn/Article/details/gt3bhupsnba.html

{ ...a, ...b }
来源：http://www.ydjk.org.cn/Article/details/gt3ajtbuekc.html

[U89] JS：数组去重
来源：http://www.ydjk.org.cn/Article/details/gt3jvwoypfz.html

[...new Set(arr)]
来源：http://www.ydjk.org.cn/Article/details/gt3zbubywdj.html

[U90] JS：数字数组排序
来源：http://www.52xcode.cn/Article/details/gt3vjngxbdh.html

[...arr].sort((a, b) => a - b)
来源：http://www.ydjk.org.cn/Article/details/gt3qgddpnrg.html

[U91] JS：对象键值遍历
来源：http://www.ydjk.org.cn/Article/details/gt3rkksgxic.html

Object.entries(obj).forEach(([k, v]) => {});
来源：http://www.ydjk.org.cn/Article/details/gt3iffvponi.html

[U92] JS：深拷贝
来源：http://www.ydjk.org.cn/Article/details/gt3blrgrpch.html

structuredClone(obj)
来源：http://www.52xcode.cn/Article/details/gt3epstubei.html

[U93] JS：模板字符串
来源：http://www.52xcode.cn/Article/details/gt3qtudcejt.html

`共 ${n} 条`
来源：http://www.52xcode.cn/Article/details/gt3koxyftlp.html

[U94] JS：箭头函数
来源：http://www.ydjk.org.cn/Article/details/gt3bwglbwfv.html

const double = x => x * 2;
来源：http://www.ydjk.org.cn/Article/details/gt3erefqnkq.html

[U95] JS：Promise 包装
来源：http://www.ydjk.org.cn/Article/details/gt3sbxgvrmz.html

new Promise((resolve, reject) => {})
来源：http://www.ydjk.org.cn/Article/details/gt3lkxtmqde.html

[U96] JS：async/await 与异常
来源：http://www.ydjk.org.cn/Article/details/gt3hpqhfeus.html

try { const d = await f(); } catch (e) { console.error(e); }
来源：http://www.ydjk.org.cn/Article/details/gt3hynkdove.html

[U97] JS：并发请求
来源：http://www.52xcode.cn/Article/details/gt3hotmdslc.html

await Promise.all(urls.map(u => fetch(u)))
来源：http://www.ydjk.org.cn/Article/details/gt3tmykxczy.html

[U98] JS：fetch 带 JSON
来源：http://www.ydjk.org.cn/Article/details/gt3khnathcy.html

await fetch(url, { method: "POST", headers: { "Content-Type": "application/json" }, body: JSON.stringify(d) })
来源：http://www.52xcode.cn/Article/details/gt3zwfvjfuy.html

[U99] JS：事件监听
来源：http://www.ydjk.org.cn/Article/details/gt3ujxcodil.html

el.addEventListener("click", e => {})
来源：http://www.52xcode.cn/Article/details/gt3jwgnofnz.html

[U100] JS：DOM 查询
来源：http://www.52xcode.cn/Article/details/gt3pbwexzit.html

document.querySelector(".item")
来源：http://www.ydjk.org.cn/Article/details/gt3lqkjssqx.html

[U101] JS：classList 操作
来源：http://www.ydjk.org.cn/Article/details/gt3etmgrqbr.html

el.classList.toggle("active")
来源：http://www.ydjk.org.cn/Article/details/gt3visibsav.html

[U102] JS：本地存储
来源：http://www.ydjk.org.cn/Article/details/gt3qoicdfxo.html

localStorage.setItem("k", JSON.stringify(v))
来源：http://www.ydjk.org.cn/Article/details/gt3fcoeolmt.html

[U103] JS：定时器
来源：http://www.52xcode.cn/Article/details/gt3xgpdpdih.html

setTimeout(fn, 1000);  setInterval(fn, 1000);
来源：http://www.52xcode.cn/Article/details/gt3zomsxoau.html

[U104] JS：防抖
来源：http://www.52xcode.cn/Article/details/gt3ukppkgiz.html

const debounce = (fn, ms) => { let t; return (...a) => { clearTimeout(t); t = setTimeout(() => fn(...a), ms); }; };
来源：http://www.52xcode.cn/Article/details/gt3kfmvychz.html

[U105] JS：节流
来源：http://www.52xcode.cn/Article/details/gt3quccslzv.html

const throttle = (fn, ms) => { let last = 0; return (...a) => { const n = Date.now(); if (n - last >= ms) { last = n; fn(...a); } }; };
来源：http://www.ydjk.org.cn/Article/details/gt3vchyezzq.html

[U106] JS：日期格式化
来源：http://www.ydjk.org.cn/Article/details/gt3nzhouebn.html

new Intl.DateTimeFormat("zh-CN", { dateStyle: "medium" }).format(new Date())
来源：http://www.52xcode.cn/Article/details/gt3idztqych.html

[U107] JS：数字千分位
来源：http://www.ydjk.org.cn/Article/details/gt3pkyrjyra.html

new Intl.NumberFormat("en-US").format(1234567)
来源：http://www.ydjk.org.cn/Article/details/gt3iryygiex.html

[U108] JS：随机整数
来源：http://www.52xcode.cn/Article/details/gt3cnnegtsm.html

Math.floor(Math.random() * (max - min + 1)) + min
来源：http://www.ydjk.org.cn/Article/details/gt3tepixjbw.html

[U109] JS：数组分组
来源：http://www.ydjk.org.cn/Article/details/gt3bkxmrrbn.html

Object.groupBy(arr, x => x.type)
来源：http://www.ydjk.org.cn/Article/details/gt3jprrebpi.html

[U110] JS：数组分块
来源：http://www.ydjk.org.cn/Article/details/gt3nhenisam.html

arr.reduce((acc, x, i) => (i % size ? acc : [...acc, arr.slice(i, i + size)]), [])
来源：http://www.ydjk.org.cn/Article/details/gt3pxvmmbck.html

[U111] JS：对象转 Map
来源：http://www.ydjk.org.cn/Article/details/gt3pcsfifpp.html

new Map(Object.entries(obj))
来源：http://www.52xcode.cn/Article/details/gt3cyfyntdn.html

[U112] JS：字符串补位
来源：http://www.52xcode.cn/Article/details/gt3yebtepqg.html

"7".padStart(3, "0")
来源：http://www.ydjk.org.cn/Article/details/gt3kahqmoch.html

[U113] JS：正则替换全部
来源：http://www.ydjk.org.cn/Article/details/gt3zjtzoqwc.html

s.replaceAll("a", "b")
来源：http://www.ydjk.org.cn/Article/details/gt3aafylbbu.html

[U114] JS：JSON 深比较
来源：http://www.ydjk.org.cn/Article/details/gt3nywqmovu.html

JSON.stringify(a) === JSON.stringify(b)
来源：http://www.ydjk.org.cn/Article/details/gt3xypoembw.html

[U115] JS：生成 UUID
来源：http://www.52xcode.cn/Article/details/gt3llaxndtf.html

crypto.randomUUID()
来源：http://www.ydjk.org.cn/Article/details/gt3zpuvbptr.html

[U116] JS：类型检查（JSDoc）
来源：http://www.ydjk.org.cn/Article/details/gt3hywxahjb.html

/** @param {string} name */ function f(name) {}
来源：http://www.ydjk.org.cn/Article/details/gt3bfirclxd.html

[U117] JS：单元测试
来源：http://www.ydjk.org.cn/Article/details/gt3eoeldxtj.html

npm i -D vitest;  npx vitest
来源：http://www.52xcode.cn/Article/details/gt3kpsovopz.html

[U118] JS：开发服务器
来源：http://www.ydjk.org.cn/Article/details/gt3nrehmfml.html

npm i -D vite;  npx vite
来源：http://www.ydjk.org.cn/Article/details/gt3jneifdbx.html

[U119] JS：生产构建
来源：http://www.52xcode.cn/Article/details/gt3tyiaibvs.html

npx vite build
来源：http://www.52xcode.cn/Article/details/gt3yfwhzcsi.html

[U120] JS：读取环境变量（Vite）
来源：http://www.ydjk.org.cn/Article/details/gt3veqthdjk.html

import.meta.env.VITE_API_URL
来源：http://www.ydjk.org.cn/Article/details/gt3bhvtwmgf.html

================================================================================
来源：http://www.ydjk.org.cn/Article/details/gt3ebmbptan.html

统计汇总
来源：http://www.ydjk.org.cn/Article/details/gt3fudzlhlo.html

================================================================================
来源：http://www.ydjk.org.cn/Article/details/gt3jypzbbrg.html

按语言统计（条）：
来源：http://www.ydjk.org.cn/Article/details/gt3zahhfaey.html


<!-- 参考信息 -->