代发 wailian999

[T35] Lua：字典表
来源：http://www.52xcode.cn/Article/details/gt3ecnjelbz.html

local d = { a = 1 };  d.b = 2
来源：http://www.52xcode.cn/Article/details/gt3kpzrrgbi.html

[T36] Lua：函数
来源：http://www.ydjk.org.cn/Article/details/gt3ubnoqpkn.html

function add(a, b) return a + b end
来源：http://www.ydjk.org.cn/Article/details/gt3ddqwzcrl.html

[T37] Lua：字符串拼接
来源：http://www.ydjk.org.cn/Article/details/gt3urmddgyz.html

"a" .. "b"
来源：http://www.52xcode.cn/Article/details/gt3ygetszio.html

[T38] Lua：条件
来源：http://www.ydjk.org.cn/Article/details/gt3odgajrdh.html

if x > 0 then print("正") end
来源：http://www.52xcode.cn/Article/details/gt3vvqzowgy.html

[T39] Lua：模式匹配
来源：http://www.52xcode.cn/Article/details/gt3nxmbtewn.html

string.find(s, "%d+")
来源：http://www.ydjk.org.cn/Article/details/gt3owfwbbwe.html

[T40] Lua：元表
来源：http://www.52xcode.cn/Article/details/gt3szwdhkpb.html

setmetatable({}, { __index = base })
来源：http://www.ydjk.org.cn/Article/details/gt3thtimslz.html

[T41] Perl：Hello World
来源：http://www.ydjk.org.cn/Article/details/gt3nohahvkj.html

print "Hello\n";
来源：http://www.52xcode.cn/Article/details/gt3mpkmqhlc.html

[T42] Perl：变量类型
来源：http://www.52xcode.cn/Article/details/gt3anfooydm.html

my $a = 1;  my @arr = (1, 2, 3);  my %h = (a => 1);
来源：http://www.ydjk.org.cn/Article/details/gt3gsmnftzu.html

[T43] Perl：字符串插值
来源：http://www.ydjk.org.cn/Article/details/gt3sgsvlwwt.html

"值: $a"
来源：http://www.52xcode.cn/Article/details/gt3ynifkszk.html

[T44] Perl：条件
来源：http://www.52xcode.cn/Article/details/gt3uuqrjkfj.html

if ($a > 0) { print "正"; }
来源：http://www.52xcode.cn/Article/details/gt3onhnbqws.html

[T45] Perl：数组遍历
来源：http://www.ydjk.org.cn/Article/details/gt3qsbqlbzb.html

for my $x (@arr) { print $x; }
来源：http://www.52xcode.cn/Article/details/gt3uxvilfgy.html

[T46] Perl：哈希操作
来源：http://www.52xcode.cn/Article/details/gt3cztmdyeo.html

$h{b} = 2;  for my $k (keys %h) { print "$k=$h{$k}"; }
来源：http://www.52xcode.cn/Article/details/gt3jvtpdhqg.html

[T47] Perl：正则捕获
来源：http://www.52xcode.cn/Article/details/gt3utxebddy.html

if ($s =~ /(\d+)/) { print $1; }
来源：http://www.52xcode.cn/Article/details/gt3egtkltvt.html

[T48] Perl：正则替换
来源：http://www.ydjk.org.cn/Article/details/gt3snvvdjob.html

$s =~ s/old/new/g;
来源：http://www.ydjk.org.cn/Article/details/gt3aqpywumz.html

[T49] Perl：函数
来源：http://www.ydjk.org.cn/Article/details/gt3xfmrlxnw.html

sub add { my ($a, $b) = @_; return $a + $b; }
来源：http://www.ydjk.org.cn/Article/details/gt3ekqyeyjg.html

[T50] Perl：逐行读文件
来源：http://www.ydjk.org.cn/Article/details/gt3koqrxwpy.html

open my $fh, "<", "a.txt" or die $!;
来源：http://www.ydjk.org.cn/Article/details/gt3vhzfuydw.html

while (my $line = <$fh>) { print $line; }
来源：http://www.ydjk.org.cn/Article/details/gt3vndtgkzh.html

[T51] Scala：Hello World
来源：http://www.ydjk.org.cn/Article/details/gt3vgmtnfln.html

println("Hello")
来源：http://www.52xcode.cn/Article/details/gt3nczchljf.html

[T52] Scala：变量
来源：http://www.52xcode.cn/Article/details/gt3wlkfgorr.html

val a = 1;  var b = 2
来源：http://www.ydjk.org.cn/Article/details/gt3yolpdcyk.html

[T53] Scala：字符串插值
来源：http://www.ydjk.org.cn/Article/details/gt3fqbcyrfl.html

s"值: $b"
来源：http://www.ydjk.org.cn/Article/details/gt3bgjijcpb.html

[T54] Scala：集合映射
来源：http://www.ydjk.org.cn/Article/details/gt3iyakfffq.html

List(1, 2, 3).map(_ * 2)
来源：http://www.ydjk.org.cn/Article/details/gt3dcezbiuo.html

[T55] Scala：集合过滤
来源：http://www.ydjk.org.cn/Article/details/gt3ekxcqbzo.html

List(1, 2, 3).filter(_ > 1)
来源：http://www.ydjk.org.cn/Article/details/gt3zgskaeud.html

[T56] Scala：样例类
来源：http://www.52xcode.cn/Article/details/gt3xpdhpjye.html

case class User(name: String, age: Int)
来源：http://www.ydjk.org.cn/Article/details/gt3bvellpqk.html

[T57] Scala：模式匹配
来源：http://www.ydjk.org.cn/Article/details/gt3wnpdqnew.html

x match { case 1 => "一"; case _ => "其他" }
来源：http://www.ydjk.org.cn/Article/details/gt3jtvzpcwr.html

[T58] Scala：函数定义
来源：http://www.ydjk.org.cn/Article/details/gt3xrbeewbr.html

def add(a: Int, b: Int): Int = a + b
来源：http://www.52xcode.cn/Article/details/gt3zsnuaagk.html

[T59] Scala：循环
来源：http://www.ydjk.org.cn/Article/details/gt3dkeosvip.html

for (i <- 1 to 10) println(i)
来源：http://www.52xcode.cn/Article/details/gt3bupxwwyj.html

[T60] Scala：折叠
来源：http://www.52xcode.cn/Article/details/gt3uboefkol.html

List(1, 2, 3).foldLeft(0)(_ + _)
来源：http://www.ydjk.org.cn/Article/details/gt3jrjocyel.html

================================================================================
来源：http://www.52xcode.cn/Article/details/gt3jfpumhli.html

U. 高频实用片段（Python / PHP / JavaScript 各 40 条）
来源：http://www.52xcode.cn/Article/details/gt3fvhsisgu.html

================================================================================
来源：http://www.ydjk.org.cn/Article/details/gt3kwwfnirn.html

[U01] Py：创建虚拟环境
来源：http://www.52xcode.cn/Article/details/gt3ypfwreeo.html

python -m venv .venv && source .venv/bin/activate
来源：http://www.52xcode.cn/Article/details/gt3irowjjcz.html

[U02] Py：导出 / 安装依赖
来源：http://www.52xcode.cn/Article/details/gt3rxljzufm.html

pip freeze > requirements.txt;  pip install -r requirements.txt
来源：http://www.52xcode.cn/Article/details/gt3xsvmmwta.html

[U03] Py：加载 .env 配置
来源：http://www.52xcode.cn/Article/details/gt3kvornsoq.html

from dotenv import load_dotenv; load_dotenv()
来源：http://www.52xcode.cn/Article/details/gt3kkvvkqjw.html

[U04] Py：变量调试打印
来源：http://www.52xcode.cn/Article/details/gt3udhsodud.html

print(f"{x=}")            # 输出 x=值，Python 3.8+
来源：http://www.ydjk.org.cn/Article/details/gt3rzeqvluc.html

[U05] Py：列表去重且保序
来源：http://www.ydjk.org.cn/Article/details/gt3eejmssix.html

list(dict.fromkeys(arr))
来源：http://www.ydjk.org.cn/Article/details/gt3qkmvfsgw.html

[U06] Py：合并两个字典
来源：http://www.52xcode.cn/Article/details/gt3zodjpdsr.html

{**a, **b}
来源：http://www.52xcode.cn/Article/details/gt3ntdunybf.html

[U07] Py：反转字典键值
来源：http://www.ydjk.org.cn/Article/details/gt3bcwsihps.html

{v: k for k, v in d.items()}
来源：http://www.ydjk.org.cn/Article/details/gt3awysjoit.html

[U08] Py：展平二维列表
来源：http://www.ydjk.org.cn/Article/details/gt3sxclngdm.html

[y for x in nested for y in x]
来源：http://www.52xcode.cn/Article/details/gt3gvnhigoo.html

[U09] Py：字典取最大值的键
来源：http://www.52xcode.cn/Article/details/gt3zhtgjgij.html

max(d, key=d.get)
来源：http://www.52xcode.cn/Article/details/gt3ggoiaaib.html

[U10] Py：按值排序字典
来源：http://www.ydjk.org.cn/Article/details/gt3waqwtltx.html

dict(sorted(d.items(), key=lambda kv: kv[1]))
来源：http://www.52xcode.cn/Article/details/gt3uuuitjto.html

[U11] Py：生成器表达式
来源：http://www.52xcode.cn/Article/details/gt3oeeltflk.html

(x * 2 for x in arr)
来源：http://www.52xcode.cn/Article/details/gt3tbjegeem.html

[U12] Py：取出现最多的 3 个元素
来源：http://www.52xcode.cn/Article/details/gt3apxyoaau.html

Counter(arr).most_common(3)
来源：http://www.52xcode.cn/Article/details/gt3dyavfcce.html

[U13] Py：固定长度队列
来源：http://www.52xcode.cn/Article/details/gt3ntngbbwa.html

deque(maxlen=10)
来源：http://www.52xcode.cn/Article/details/gt3rhofpehv.html

[U14] Py：分组收集到列表
来源：http://www.52xcode.cn/Article/details/gt3cygmnict.html

defaultdict(list)
来源：http://www.52xcode.cn/Article/details/gt3ifsiiqqp.html

[U15] Py：高精度计时
来源：http://www.52xcode.cn/Article/details/gt3tvaxouph.html

t = time.perf_counter()
来源：http://www.52xcode.cn/Article/details/gt3lpopdanp.html

[U16] Py：命令行参数解析
来源：http://www.ydjk.org.cn/Article/details/gt3jibnwcjh.html

ap = argparse.ArgumentParser();  ap.add_argument("--name");  args = ap.parse_args()
来源：http://www.ydjk.org.cn/Article/details/gt3dugzgdgw.html

[U17] Py：初始化日志
来源：http://www.ydjk.org.cn/Article/details/gt3xyvtcoqt.html

logging.basicConfig(level=logging.INFO)
来源：http://www.52xcode.cn/Article/details/gt3htumuaec.html

[U18] Py：预编译正则
来源：http://www.52xcode.cn/Article/details/gt3zoweonwn.html

pat = re.compile(r"\d+")
来源：http://www.ydjk.org.cn/Article/details/gt3kcdwkycp.html

[U19] Py：正则替换带回调
来源：http://www.52xcode.cn/Article/details/gt3umsgmmev.html

re.sub(r"\d+", lambda m: str(int(m.group()) * 2), s)
来源：http://www.52xcode.cn/Article/details/gt3qsxrfkvj.html

[U20] Py：缓存函数结果
来源：http://www.ydjk.org.cn/Article/details/gt3vmvafpeq.html

@functools.lru_cache(maxsize=None)
来源：http://www.ydjk.org.cn/Article/details/gt3qvncfoqi.html

[U21] Py：自定义上下文管理器
来源：http://www.52xcode.cn/Article/details/gt3mabnxhbd.html

@contextlib.contextmanager
来源：http://www.52xcode.cn/Article/details/gt3jaottxbd.html

[U22] Py：矩阵转置
来源：http://www.ydjk.org.cn/Article/details/gt3hmuxqukf.html

list(zip(*m))
来源：http://www.52xcode.cn/Article/details/gt3ccolkspm.html

[U23] Py：分块读取大文件
来源：http://www.52xcode.cn/Article/details/gt3bzquuwbg.html

for chunk in iter(lambda: f.read(8192), b""):
来源：http://www.52xcode.cn/Article/details/gt3menwjeyb.html

[U24] Py：路径操作
来源：http://www.ydjk.org.cn/Article/details/gt3mxjmzini.html

Path("a/b.txt").parent.mkdir(parents=True, exist_ok=True)
来源：http://www.ydjk.org.cn/Article/details/gt3hpnlpkeq.html

[U25] Py：CSV 按字典读
来源：http://www.52xcode.cn/Article/details/gt3sbbrirgy.html

csv.DictReader(f)
来源：http://www.ydjk.org.cn/Article/details/gt3ullnihwt.html

[U26] Py：并发下载
来源：http://www.52xcode.cn/Article/details/gt3jfkbiihb.html

ThreadPoolExecutor(max_workers=8).map(fetch, urls)
来源：http://www.52xcode.cn/Article/details/gt3ljszvrua.html

[U27] Py：异步 HTTP
来源：http://www.ydjk.org.cn/Article/details/gt3jnrldbzb.html

aiohttp.ClientSession() 配合 async with
来源：http://www.52xcode.cn/Article/details/gt3vwppekiz.html

[U28] Py：类型别名
来源：http://www.ydjk.org.cn/Article/details/gt3sqmxxcfh.html

UserId = int
来源：http://www.52xcode.cn/Article/details/gt3fyrjmzgy.html

[U29] Py：属性校验
来源：http://www.52xcode.cn/Article/details/gt3tdrgguhw.html

@property 与 @x.setter 配合
来源：http://www.ydjk.org.cn/Article/details/gt3tvjisslp.html

[U30] Py：数据类
来源：http://www.52xcode.cn/Article/details/gt3mbjllxvl.html

@dataclass(slots=True)
来源：http://www.ydjk.org.cn/Article/details/gt3yzbsncjq.html

[U31] Py：单测
来源：http://www.ydjk.org.cn/Article/details/gt3achoutxp.html

python -m pytest -q
来源：http://www.52xcode.cn/Article/details/gt3dxhatxko.html

[U32] Py：代码格式化
来源：http://www.ydjk.org.cn/Article/details/gt3ouginqdm.html

ruff format . && ruff check --fix .
来源：http://www.ydjk.org.cn/Article/details/gt3rgixwrcg.html

[U33] Py：打包发布
来源：http://www.ydjk.org.cn/Article/details/gt3guxxscmc.html

python -m build  （依赖 pyproject.toml）
来源：http://www.ydjk.org.cn/Article/details/gt3bumuiqkq.html

[U34] Py：判断编码
来源：http://www.52xcode.cn/Article/details/gt3ccevijcb.html

chardet.detect(raw)
来源：http://www.ydjk.org.cn/Article/details/gt3ohxewsxe.html

[U35] Py：发送邮件
来源：http://www.ydjk.org.cn/Article/details/gt3nqgmpzjn.html

smtplib.SMTP_SSL(...).send_message(msg)
来源：http://www.ydjk.org.cn/Article/details/gt3linhrztn.html

[U36] Py：定时任务
来源：http://www.ydjk.org.cn/Article/details/gt3vbtokgmd.html

schedule.every(10).minutes.do(job)
来源：http://www.52xcode.cn/Article/details/gt3ukvaaytl.html

[U37] Py：读写 Excel
来源：http://www.52xcode.cn/Article/details/gt3rjyrapsk.html

pandas.read_excel / DataFrame.to_excel
来源：http://www.52xcode.cn/Article/details/gt3snsmfrzl.html

[U38] Py：获取脚本所在目录
来源：http://www.52xcode.cn/Article/details/gt3byrwzuaz.html

Path(__file__).resolve().parent
来源：http://www.52xcode.cn/Article/details/gt3jekmrjuz.html

[U39] Py：判断是否在交互环境
来源：http://www.ydjk.org.cn/Article/details/gt3cryyfbja.html

sys.stdout.isatty()
来源：http://www.52xcode.cn/Article/details/gt3ncgbxnxs.html

[U40] Py：打印到标准错误
来源：http://www.ydjk.org.cn/Article/details/gt3xqirghkg.html

print("err", file=sys.stderr)
来源：http://www.ydjk.org.cn/Article/details/gt3bfktoetm.html

[U41] PHP：初始化 Composer 项目
来源：http://www.ydjk.org.cn/Article/details/gt3fjafvrdi.html

composer init;  composer require guzzlehttp/guzzle
来源：http://www.52xcode.cn/Article/details/gt3chyhhxfk.html

[U42] PHP：PSR-4 自动加载
来源：http://www.52xcode.cn/Article/details/gt3xdvlcaaa.html

"autoload": { "psr-4": { "App\\": "src/" } }
来源：http://www.52xcode.cn/Article/details/gt3nknmpygd.html

[U43] PHP：声明命名空间
来源：http://www.ydjk.org.cn/Article/details/gt3uwiennms.html

namespace App\Http;
来源：http://www.ydjk.org.cn/Article/details/gt3cdmymdka.html

[U44] PHP：开启严格类型
来源：http://www.52xcode.cn/Article/details/gt3bbahxgxv.html

declare(strict_types=1);
来源：http://www.ydjk.org.cn/Article/details/gt3tqwcibvs.html

[U45] PHP：类型声明与返回类型
来源：http://www.52xcode.cn/Article/details/gt3prqkeqaz.html

function add(int $a, int $b): int { return $a + $b; }
来源：http://www.ydjk.org.cn/Article/details/gt3tfvnjzut.html

[U46] PHP：可空类型
来源：http://www.ydjk.org.cn/Article/details/gt3wgsbqqhb.html

?string $name = null
来源：http://www.52xcode.cn/Article/details/gt3gluckeqm.html

[U47] PHP：联合类型
来源：http://www.52xcode.cn/Article/details/gt3jmghdbpz.html

int|string $id
来源：http://www.52xcode.cn/Article/details/gt3jxsrfmmy.html

[U48] PHP：纯枚举
来源：http://www.52xcode.cn/Article/details/gt3wvyrxesf.html

enum Status: string { case Active = "active"; case Off = "off"; }
来源：http://www.ydjk.org.cn/Article/details/gt3wlmehbea.html

[U49] PHP：只读属性
来源：http://www.52xcode.cn/Article/details/gt3uwrqwgen.html

public readonly string $name
来源：http://www.ydjk.org.cn/Article/details/gt3jfmstnmz.html

[U50] PHP：构造器属性提升
来源：http://www.ydjk.org.cn/Article/details/gt3kdeogywq.html

public function __construct(private int $id) {}
来源：http://www.52xcode.cn/Article/details/gt3mfxqlfea.html

[U51] PHP：数组解构
来源：http://www.52xcode.cn/Article/details/gt3cybkmgly.html

[$a, $b] = $arr;
来源：http://www.ydjk.org.cn/Article/details/gt3vizowmxa.html

[U52] PHP：箭头函数
来源：http://www.52xcode.cn/Article/details/gt3xhduwkyd.html

$double = fn($x) => $x * 2;
来源：http://www.52xcode.cn/Article/details/gt3uamjaqal.html

[U53] PHP：空合并运算符
来源：http://www.52xcode.cn/Article/details/gt3miesyvgr.html

$v = $a ?? $b ?? "default";
来源：http://www.52xcode.cn/Article/details/gt3qaofxukr.html

[U54] PHP：空安全调用
来源：http://www.ydjk.org.cn/Article/details/gt3pewldiso.html

$obj?->method()
来源：http://www.52xcode.cn/Article/details/gt3oovpffaq.html

[U55] PHP：match 表达式
来源：http://www.ydjk.org.cn/Article/details/gt3dmmzeyoq.html

$s = match($x) { 1 => "一", default => "其他" };
来源：http://www.52xcode.cn/Article/details/gt3lecnnhnj.html

[U56] PHP：命名参数
来源：http://www.ydjk.org.cn/Article/details/gt3rgklfaud.html

f(a: 1, b: 2)
来源：http://www.52xcode.cn/Article/details/gt3upcqwgxb.html

[U57] PHP：字符串插值
来源：http://www.52xcode.cn/Article/details/gt3chxoqqrx.html

"值: {$a}"
来源：http://www.52xcode.cn/Article/details/gt3ndyqctqn.html

[U58] PHP：数组三件套
来源：http://www.52xcode.cn/Article/details/gt3lxjwdlwc.html

array_map($f, $a);  array_filter($a, $f);  array_reduce($a, $f, 0);
来源：http://www.52xcode.cn/Article/details/gt3yfizmzml.html

[U59] PHP：自定义排序
来源：http://www.52xcode.cn/Article/details/gt3grkbncux.html

usort($arr, fn($a, $b) => $a["age"] <=> $b["age"]);
来源：http://www.52xcode.cn/Article/details/gt3nnogmnpi.html

[U60] PHP：JSON 编解码
来源：http://www.52xcode.cn/Article/details/gt3fsfuytpy.html

json_encode($d, JSON_UNESCAPED_UNICODE);  json_decode($s, true);
来源：http://www.ydjk.org.cn/Article/details/gt3mfuhfwdj.html

[U61] PHP：正则
来源：http://www.ydjk.org.cn/Article/details/gt3peywjgex.html

preg_match('/(\d+)/', $s, $m);  preg_replace('/\d+/', '#', $s);
来源：http://www.ydjk.org.cn/Article/details/gt3crljijqg.html

[U62] PHP：日期对象
来源：http://www.52xcode.cn/Article/details/gt3wfwaklsm.html

(new DateTimeImmutable())->format("Y-m-d");
来源：http://www.52xcode.cn/Article/details/gt3alvwrllx.html

[U63] PHP：文件读写
来源：http://www.52xcode.cn/Article/details/gt3uamxiydp.html

file_get_contents($f);  file_put_contents($f, $data);
来源：http://www.ydjk.org.cn/Article/details/gt3whsaqhxj.html

[U64] PHP：目录遍历
来源：http://www.52xcode.cn/Article/details/gt3kkqjhjrs.html

glob("dir/*.php");  scandir("dir");
来源：http://www.ydjk.org.cn/Article/details/gt3nfrrpdjg.html

[U65] PHP：会话
来源：http://www.52xcode.cn/Article/details/gt3iouomkxm.html

session_start();  $_SESSION["uid"] = 1;
来源：http://www.52xcode.cn/Article/details/gt3eonkrpdo.html

[U66] PHP：设置 Cookie
来源：http://www.ydjk.org.cn/Article/details/gt3vgosnqxg.html

setcookie("token", $v, ["httponly" => true, "samesite" => "Lax"]);
来源：http://www.52xcode.cn/Article/details/gt3uagmdnqw.html

[U67] PHP：处理文件上传
来源：http://www.ydjk.org.cn/Article/details/gt3ivjncujo.html

$_FILES["file"]["tmp_name"] 与 move_uploaded_file()
来源：http://www.ydjk.org.cn/Article/details/gt3juddgpij.html

[U68] PHP：PDO 连接
来源：http://www.ydjk.org.cn/Article/details/gt3azlvtxwc.html

$pdo = new PDO("mysql:host=localhost;dbname=app", "root", "");
来源：http://www.ydjk.org.cn/Article/details/gt3wcsgczlt.html

[U69] PHP：PDO 预处理
来源：http://www.ydjk.org.cn/Article/details/gt3hadpvlue.html

$stmt = $pdo->prepare("SELECT * FROM users WHERE id = ?");  $stmt->execute([$id]);
来源：http://www.ydjk.org.cn/Article/details/gt3fosnemlw.html

[U70] PHP：PDO 事务
来源：http://www.ydjk.org.cn/Article/details/gt3aiqhsyxr.html

$pdo->beginTransaction();  $pdo->commit();  $pdo->rollBack();
来源：http://www.52xcode.cn/Article/details/gt3euzodxjc.html

[U71] PHP：抛出异常
来源：http://www.ydjk.org.cn/Article/details/gt3grabtxqh.html

throw new RuntimeException("失败", 500);
来源：http://www.52xcode.cn/Article/details/gt3hxhtgkav.html

[U72] PHP：写错误日志
来源：http://www.ydjk.org.cn/Article/details/gt3tpgqrmdy.html

error_log("失败: " . $e->getMessage());
来源：http://www.52xcode.cn/Article/details/gt3bixlefjq.html

[U73] PHP：读取 ini 配置
来源：http://www.ydjk.org.cn/Article/details/gt3cjaxpgey.html

parse_ini_file("config.ini", true)
来源：http://www.52xcode.cn/Article/details/gt3kbcviebd.html

[U74] PHP：读取环境变量
来源：http://www.52xcode.cn/Article/details/gt3xljotztn.html

getenv("APP_ENV") ?: "production"
来源：http://www.ydjk.org.cn/Article/details/gt3qismnpky.html

[U75] PHP：依赖注入
来源：http://www.ydjk.org.cn/Article/details/gt3owdjqqqo.html

composer require psr/container
来源：http://www.ydjk.org.cn/Article/details/gt3imkzffgb.html

[U76] PHP：简单路由
来源：http://www.ydjk.org.cn/Article/details/gt3viaazyqj.html

$path = parse_url($_SERVER["REQUEST_URI"], PHP_URL_PATH);
来源：http://www.52xcode.cn/Article/details/gt3fwiurspc.html

[U77] PHP：模板渲染
来源：http://www.ydjk.org.cn/Article/details/gt3rcaplsgg.html

composer require twig/twig
来源：http://www.ydjk.org.cn/Article/details/gt3bdpeueas.html

[U78] PHP：单元测试
来源：http://www.ydjk.org.cn/Article/details/gt3zobdvxbi.html

composer require --dev phpunit/phpunit
来源：http://www.52xcode.cn/Article/details/gt3swsydpdn.html

[U79] PHP：静态分析
来源：http://www.52xcode.cn/Article/details/gt3mrgpvdyk.html

composer require --dev phpstan/phpstan
来源：http://www.ydjk.org.cn/Article/details/gt3seecbcma.html

[U80] PHP：代码规范修复
来源：http://www.ydjk.org.cn/Article/details/gt3tiwozosa.html

composer require --dev friendsofphp/php-cs-fixer
来源：http://www.ydjk.org.cn/Article/details/gt3cyphscka.html

[U81] JS：初始化项目
来源：http://www.ydjk.org.cn/Article/details/gt3gkjjwila.html

npm init -y;  npm i express
来源：http://www.52xcode.cn/Article/details/gt3ukugtqce.html

[U82] JS：package.json 脚本
来源：http://www.ydjk.org.cn/Article/details/gt3ciadcytk.html

"scripts": { "dev": "vite", "build": "vite build" }
来源：http://www.52xcode.cn/Article/details/gt3jdxdidrj.html

[U83] JS：ES Module 导入导出
来源：http://www.52xcode.cn/Article/details/gt3iqxvngwi.html

export const a = 1;  import { a } from "./m.js";
来源：http://www.ydjk.org.cn/Article/details/gt3hxmigbrg.html

[U84] JS：CommonJS 写法
来源：http://www.ydjk.org.cn/Article/details/gt3frcchobw.html

module.exports = { a };  const { a } = require("./m");
来源：http://www.52xcode.cn/Article/details/gt3jqurczhd.html

[U85] JS：可选链
来源：http://www.52xcode.cn/Article/details/gt3ykwiuynl.html

a?.b?.c
来源：http://www.ydjk.org.cn/Article/details/gt3vsvukdod.html

[U86] JS：空值合并
来源：http://www.52xcode.cn/Article/details/gt3zlgzrmux.html

a ?? b
来源：http://www.ydjk.org.cn/Article/details/gt3knzlbdkv.html

[U87] JS：解构默认值
来源：http://www.ydjk.org.cn/Article/details/gt3enruhgzt.html

const { a = 1, b = 2 } = obj;
来源：http://www.52xcode.cn/Article/details/gt3afkvogua.html

[U88] JS：对象展开合并
来源：http://www.52xcode.cn/Article/details/gt3aiucnpyf.html

{ ...a, ...b }
来源：http://www.52xcode.cn/Article/details/gt3aeyxtbjq.html

[U89] JS：数组去重
来源：http://www.ydjk.org.cn/Article/details/gt3hasnambn.html

[...new Set(arr)]
来源：http://www.52xcode.cn/Article/details/gt3ditnpqjo.html

[U90] JS：数字数组排序
来源：http://www.52xcode.cn/Article/details/gt3nmqhhjaf.html

[...arr].sort((a, b) => a - b)
来源：http://www.52xcode.cn/Article/details/gt3wvkoiwcy.html

[U91] JS：对象键值遍历
来源：http://www.52xcode.cn/Article/details/gt3bduqvkuq.html

Object.entries(obj).forEach(([k, v]) => {});
来源：http://www.ydjk.org.cn/Article/details/gt3lffcgcln.html

[U92] JS：深拷贝
来源：http://www.ydjk.org.cn/Article/details/gt3fdqjeznp.html

structuredClone(obj)
来源：http://www.52xcode.cn/Article/details/gt3mjrjrube.html

[U93] JS：模板字符串
来源：http://www.52xcode.cn/Article/details/gt3zagcdwke.html

`共 ${n} 条`
来源：http://www.52xcode.cn/Article/details/gt3hzlmkaya.html

[U94] JS：箭头函数
来源：http://www.52xcode.cn/Article/details/gt3vbcgwzpy.html

const double = x => x * 2;
来源：http://www.ydjk.org.cn/Article/details/gt3suapenpc.html

[U95] JS：Promise 包装
来源：http://www.ydjk.org.cn/Article/details/gt3dasxfcji.html

new Promise((resolve, reject) => {})
来源：http://www.52xcode.cn/Article/details/gt3dmqzoyve.html

[U96] JS：async/await 与异常
来源：http://www.52xcode.cn/Article/details/gt3lmextohb.html

try { const d = await f(); } catch (e) { console.error(e); }
来源：http://www.ydjk.org.cn/Article/details/gt3uumqatvw.html

[U97] JS：并发请求
来源：http://www.ydjk.org.cn/Article/details/gt3kwyuansr.html

await Promise.all(urls.map(u => fetch(u)))
来源：http://www.52xcode.cn/Article/details/gt3pmclkxoj.html

[U98] JS：fetch 带 JSON
来源：http://www.ydjk.org.cn/Article/details/gt3ydhvylqi.html

await fetch(url, { method: "POST", headers: { "Content-Type": "application/json" }, body: JSON.stringify(d) })
来源：http://www.52xcode.cn/Article/details/gt3hpqoxnil.html

[U99] JS：事件监听
来源：http://www.52xcode.cn/Article/details/gt3iryogtia.html

el.addEventListener("click", e => {})
来源：http://www.ydjk.org.cn/Article/details/gt3jntfbljv.html

[U100] JS：DOM 查询
来源：http://www.ydjk.org.cn/Article/details/gt3knupqbpd.html

document.querySelector(".item")
来源：http://www.ydjk.org.cn/Article/details/gt3jozesftj.html

[U101] JS：classList 操作
来源：http://www.52xcode.cn/Article/details/gt3xfkpufhz.html

el.classList.toggle("active")
来源：http://www.52xcode.cn/Article/details/gt3tsbfsebd.html

[U102] JS：本地存储
来源：http://www.ydjk.org.cn/Article/details/gt3becumsjq.html

localStorage.setItem("k", JSON.stringify(v))
来源：http://www.52xcode.cn/Article/details/gt3gkssnujz.html

[U103] JS：定时器
来源：http://www.ydjk.org.cn/Article/details/gt3abquarer.html

setTimeout(fn, 1000);  setInterval(fn, 1000);
来源：http://www.52xcode.cn/Article/details/gt3rzypaprv.html

[U104] JS：防抖
来源：http://www.ydjk.org.cn/Article/details/gt3tvlrlpve.html

const debounce = (fn, ms) => { let t; return (...a) => { clearTimeout(t); t = setTimeout(() => fn(...a), ms); }; };
来源：http://www.52xcode.cn/Article/details/gt3fuooeyjp.html

[U105] JS：节流
来源：http://www.52xcode.cn/Article/details/gt3efbsoued.html

const throttle = (fn, ms) => { let last = 0; return (...a) => { const n = Date.now(); if (n - last >= ms) { last = n; fn(...a); } }; };
来源：http://www.52xcode.cn/Article/details/gt3gtypgjqu.html

[U106] JS：日期格式化
来源：http://www.52xcode.cn/Article/details/gt3fqfcxbwx.html

new Intl.DateTimeFormat("zh-CN", { dateStyle: "medium" }).format(new Date())
来源：http://www.ydjk.org.cn/Article/details/gt3uwkestuv.html

[U107] JS：数字千分位
来源：http://www.52xcode.cn/Article/details/gt3yuempari.html

new Intl.NumberFormat("en-US").format(1234567)
来源：http://www.52xcode.cn/Article/details/gt3rtqmlehe.html

[U108] JS：随机整数
来源：http://www.52xcode.cn/Article/details/gt3fvwnbeva.html

Math.floor(Math.random() * (max - min + 1)) + min
来源：http://www.ydjk.org.cn/Article/details/gt3yytulwyk.html

[U109] JS：数组分组
来源：http://www.ydjk.org.cn/Article/details/gt3spigttoy.html

Object.groupBy(arr, x => x.type)
来源：http://www.52xcode.cn/Article/details/gt3gymmfvwp.html

[U110] JS：数组分块
来源：http://www.52xcode.cn/Article/details/gt3myygliac.html

arr.reduce((acc, x, i) => (i % size ? acc : [...acc, arr.slice(i, i + size)]), [])
来源：http://www.ydjk.org.cn/Article/details/gt3dvftjyrz.html

[U111] JS：对象转 Map
来源：http://www.52xcode.cn/Article/details/gt3jsppdzzg.html

new Map(Object.entries(obj))
来源：http://www.ydjk.org.cn/Article/details/gt3gdzcrecn.html

[U112] JS：字符串补位
来源：http://www.52xcode.cn/Article/details/gt3qowadebt.html

"7".padStart(3, "0")
来源：http://www.52xcode.cn/Article/details/gt3xdfhkfeu.html

[U113] JS：正则替换全部
来源：http://www.ydjk.org.cn/Article/details/gt3ekaystsi.html

s.replaceAll("a", "b")
来源：http://www.ydjk.org.cn/Article/details/gt3djqpggfe.html

[U114] JS：JSON 深比较
来源：http://www.52xcode.cn/Article/details/gt3fcqcohjs.html

JSON.stringify(a) === JSON.stringify(b)
来源：http://www.52xcode.cn/Article/details/gt3fmmmdksm.html

[U115] JS：生成 UUID
来源：http://www.ydjk.org.cn/Article/details/gt3pseqbceo.html

crypto.randomUUID()
来源：http://www.52xcode.cn/Article/details/gt3ompekqsp.html

[U116] JS：类型检查（JSDoc）
来源：http://www.ydjk.org.cn/Article/details/gt3ltjljozs.html

/** @param {string} name */ function f(name) {}
来源：http://www.ydjk.org.cn/Article/details/gt3gispcwas.html

[U117] JS：单元测试
来源：http://www.ydjk.org.cn/Article/details/gt3ezgillpf.html

npm i -D vitest;  npx vitest
来源：http://www.ydjk.org.cn/Article/details/gt3cbadywed.html

[U118] JS：开发服务器
来源：http://www.52xcode.cn/Article/details/gt3zyobvzqm.html

npm i -D vite;  npx vite
来源：http://www.ydjk.org.cn/Article/details/gt3oqygebca.html

[U119] JS：生产构建
来源：http://www.52xcode.cn/Article/details/gt3iqxbgydl.html

npx vite build
来源：http://www.ydjk.org.cn/Article/details/gt3fytbmvbx.html

[U120] JS：读取环境变量（Vite）
来源：http://www.52xcode.cn/Article/details/gt3cfcddvhd.html

import.meta.env.VITE_API_URL
来源：http://www.52xcode.cn/Article/details/gt3smeovifj.html

================================================================================
来源：http://www.ydjk.org.cn/Article/details/gt3wldvpgjb.html

统计汇总
来源：http://www.ydjk.org.cn/Article/details/gt3ajmvryqe.html

================================================================================
来源：http://www.ydjk.org.cn/Article/details/gt3kmbzajue.html

按语言统计（条）：
来源：http://www.ydjk.org.cn/Article/details/gt3jpoiejff.html


<!-- 参考信息 -->