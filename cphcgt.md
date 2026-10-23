代发 wailian999

[T35] Lua：字典表
来源：http://www.ydjk.org.cn/Article/details/gt3fhuilujc.html

local d = { a = 1 };  d.b = 2
来源：http://www.52xcode.cn/Article/details/gt3cmgfgnkc.html

[T36] Lua：函数
来源：http://www.ydjk.org.cn/Article/details/gt3oldciqth.html

function add(a, b) return a + b end
来源：http://www.ydjk.org.cn/Article/details/gt3krfvuvtn.html

[T37] Lua：字符串拼接
来源：http://www.ydjk.org.cn/Article/details/gt3aekmhloo.html

"a" .. "b"
来源：http://www.52xcode.cn/Article/details/gt3ckmxocku.html

[T38] Lua：条件
来源：http://www.52xcode.cn/Article/details/gt3pgemgekn.html

if x > 0 then print("正") end
来源：http://www.ydjk.org.cn/Article/details/gt3neqaawza.html

[T39] Lua：模式匹配
来源：http://www.52xcode.cn/Article/details/gt3solovfda.html

string.find(s, "%d+")
来源：http://www.52xcode.cn/Article/details/gt3iutwgwab.html

[T40] Lua：元表
来源：http://www.52xcode.cn/Article/details/gt3ricntcmv.html

setmetatable({}, { __index = base })
来源：http://www.ydjk.org.cn/Article/details/gt3hwqfhhmq.html

[T41] Perl：Hello World
来源：http://www.ydjk.org.cn/Article/details/gt3axqqtlij.html

print "Hello\n";
来源：http://www.52xcode.cn/Article/details/gt3ibivviim.html

[T42] Perl：变量类型
来源：http://www.52xcode.cn/Article/details/gt3yhdmmjkv.html

my $a = 1;  my @arr = (1, 2, 3);  my %h = (a => 1);
来源：http://www.ydjk.org.cn/Article/details/gt3uhjazfxa.html

[T43] Perl：字符串插值
来源：http://www.52xcode.cn/Article/details/gt3klcnmfyc.html

"值: $a"
来源：http://www.52xcode.cn/Article/details/gt3sveubjvt.html

[T44] Perl：条件
来源：http://www.52xcode.cn/Article/details/gt3qdqsxfor.html

if ($a > 0) { print "正"; }
来源：http://www.ydjk.org.cn/Article/details/gt3fhirpaow.html

[T45] Perl：数组遍历
来源：http://www.52xcode.cn/Article/details/gt3vgtlesdn.html

for my $x (@arr) { print $x; }
来源：http://www.52xcode.cn/Article/details/gt3wmdmyjqw.html

[T46] Perl：哈希操作
来源：http://www.ydjk.org.cn/Article/details/gt3ivxdjnjg.html

$h{b} = 2;  for my $k (keys %h) { print "$k=$h{$k}"; }
来源：http://www.ydjk.org.cn/Article/details/gt3spxcgxyd.html

[T47] Perl：正则捕获
来源：http://www.ydjk.org.cn/Article/details/gt3xlvndysm.html

if ($s =~ /(\d+)/) { print $1; }
来源：http://www.52xcode.cn/Article/details/gt3sshnalha.html

[T48] Perl：正则替换
来源：http://www.52xcode.cn/Article/details/gt3cylqahxu.html

$s =~ s/old/new/g;
来源：http://www.ydjk.org.cn/Article/details/gt3sdbirvuu.html

[T49] Perl：函数
来源：http://www.52xcode.cn/Article/details/gt3xpnankzr.html

sub add { my ($a, $b) = @_; return $a + $b; }
来源：http://www.52xcode.cn/Article/details/gt3jmhhvrym.html

[T50] Perl：逐行读文件
来源：http://www.52xcode.cn/Article/details/gt3hbozbxlw.html

open my $fh, "<", "a.txt" or die $!;
来源：http://www.52xcode.cn/Article/details/gt3drlcdrtf.html

while (my $line = <$fh>) { print $line; }
来源：http://www.ydjk.org.cn/Article/details/gt3xeeorgus.html

[T51] Scala：Hello World
来源：http://www.52xcode.cn/Article/details/gt3wyaagwyc.html

println("Hello")
来源：http://www.52xcode.cn/Article/details/gt3hksafeod.html

[T52] Scala：变量
来源：http://www.52xcode.cn/Article/details/gt3vtmxhsvj.html

val a = 1;  var b = 2
来源：http://www.52xcode.cn/Article/details/gt3rrgmupmi.html

[T53] Scala：字符串插值
来源：http://www.ydjk.org.cn/Article/details/gt3mdgvpdis.html

s"值: $b"
来源：http://www.52xcode.cn/Article/details/gt3nfbohrtu.html

[T54] Scala：集合映射
来源：http://www.ydjk.org.cn/Article/details/gt3pdcmhmdk.html

List(1, 2, 3).map(_ * 2)
来源：http://www.52xcode.cn/Article/details/gt3kdjipagf.html

[T55] Scala：集合过滤
来源：http://www.ydjk.org.cn/Article/details/gt3lxxagvqj.html

List(1, 2, 3).filter(_ > 1)
来源：http://www.ydjk.org.cn/Article/details/gt3okfrlvil.html

[T56] Scala：样例类
来源：http://www.52xcode.cn/Article/details/gt3tsqwzgwd.html

case class User(name: String, age: Int)
来源：http://www.ydjk.org.cn/Article/details/gt3pyxuilvt.html

[T57] Scala：模式匹配
来源：http://www.52xcode.cn/Article/details/gt3gpqslvjc.html

x match { case 1 => "一"; case _ => "其他" }
来源：http://www.52xcode.cn/Article/details/gt3sopplqkm.html

[T58] Scala：函数定义
来源：http://www.52xcode.cn/Article/details/gt3lyysvrgd.html

def add(a: Int, b: Int): Int = a + b
来源：http://www.52xcode.cn/Article/details/gt3xdzhpdma.html

[T59] Scala：循环
来源：http://www.ydjk.org.cn/Article/details/gt3vtkszpfj.html

for (i <- 1 to 10) println(i)
来源：http://www.ydjk.org.cn/Article/details/gt3izpibohn.html

[T60] Scala：折叠
来源：http://www.ydjk.org.cn/Article/details/gt3napfdusk.html

List(1, 2, 3).foldLeft(0)(_ + _)
来源：http://www.ydjk.org.cn/Article/details/gt3ktwxwgvr.html

================================================================================
来源：http://www.52xcode.cn/Article/details/gt3oexfqajk.html

U. 高频实用片段（Python / PHP / JavaScript 各 40 条）
来源：http://www.ydjk.org.cn/Article/details/gt3cucxehzr.html

================================================================================
来源：http://www.52xcode.cn/Article/details/gt3vktfbpje.html

[U01] Py：创建虚拟环境
来源：http://www.52xcode.cn/Article/details/gt3trxhybea.html

python -m venv .venv && source .venv/bin/activate
来源：http://www.ydjk.org.cn/Article/details/gt3zyintdup.html

[U02] Py：导出 / 安装依赖
来源：http://www.52xcode.cn/Article/details/gt3yugksosr.html

pip freeze > requirements.txt;  pip install -r requirements.txt
来源：http://www.ydjk.org.cn/Article/details/gt3qkagjthd.html

[U03] Py：加载 .env 配置
来源：http://www.52xcode.cn/Article/details/gt3gbexasft.html

from dotenv import load_dotenv; load_dotenv()
来源：http://www.ydjk.org.cn/Article/details/gt3awdyakmk.html

[U04] Py：变量调试打印
来源：http://www.ydjk.org.cn/Article/details/gt3szrbfqkg.html

print(f"{x=}")            # 输出 x=值，Python 3.8+
来源：http://www.52xcode.cn/Article/details/gt3pdfqlkdw.html

[U05] Py：列表去重且保序
来源：http://www.52xcode.cn/Article/details/gt3ovfingme.html

list(dict.fromkeys(arr))
来源：http://www.ydjk.org.cn/Article/details/gt3kwiwbjfd.html

[U06] Py：合并两个字典
来源：http://www.ydjk.org.cn/Article/details/gt3rvrosodr.html

{**a, **b}
来源：http://www.52xcode.cn/Article/details/gt3tnbtuncf.html

[U07] Py：反转字典键值
来源：http://www.52xcode.cn/Article/details/gt3frlwfnup.html

{v: k for k, v in d.items()}
来源：http://www.ydjk.org.cn/Article/details/gt3qnuiuken.html

[U08] Py：展平二维列表
来源：http://www.ydjk.org.cn/Article/details/gt3sxubcfxi.html

[y for x in nested for y in x]
来源：http://www.52xcode.cn/Article/details/gt3mjsoaxdy.html

[U09] Py：字典取最大值的键
来源：http://www.ydjk.org.cn/Article/details/gt3kmyksllj.html

max(d, key=d.get)
来源：http://www.ydjk.org.cn/Article/details/gt3zmmdvvmn.html

[U10] Py：按值排序字典
来源：http://www.ydjk.org.cn/Article/details/gt3kvojdlvv.html

dict(sorted(d.items(), key=lambda kv: kv[1]))
来源：http://www.ydjk.org.cn/Article/details/gt3hkneikgy.html

[U11] Py：生成器表达式
来源：http://www.ydjk.org.cn/Article/details/gt3ajbnaseh.html

(x * 2 for x in arr)
来源：http://www.ydjk.org.cn/Article/details/gt3rgqopjnv.html

[U12] Py：取出现最多的 3 个元素
来源：http://www.52xcode.cn/Article/details/gt3qbozbdyh.html

Counter(arr).most_common(3)
来源：http://www.52xcode.cn/Article/details/gt3mhwoftis.html

[U13] Py：固定长度队列
来源：http://www.52xcode.cn/Article/details/gt3vjrxlzhr.html

deque(maxlen=10)
来源：http://www.52xcode.cn/Article/details/gt3cdveprvu.html

[U14] Py：分组收集到列表
来源：http://www.52xcode.cn/Article/details/gt3twoqpuos.html

defaultdict(list)
来源：http://www.52xcode.cn/Article/details/gt3issiqvvy.html

[U15] Py：高精度计时
来源：http://www.ydjk.org.cn/Article/details/gt3trvgeewu.html

t = time.perf_counter()
来源：http://www.ydjk.org.cn/Article/details/gt3rtampvwd.html

[U16] Py：命令行参数解析
来源：http://www.ydjk.org.cn/Article/details/gt3tpykwzel.html

ap = argparse.ArgumentParser();  ap.add_argument("--name");  args = ap.parse_args()
来源：http://www.ydjk.org.cn/Article/details/gt3skcdgdli.html

[U17] Py：初始化日志
来源：http://www.ydjk.org.cn/Article/details/gt3aigeoagq.html

logging.basicConfig(level=logging.INFO)
来源：http://www.ydjk.org.cn/Article/details/gt3ziuuosxb.html

[U18] Py：预编译正则
来源：http://www.52xcode.cn/Article/details/gt3lmnakpuu.html

pat = re.compile(r"\d+")
来源：http://www.ydjk.org.cn/Article/details/gt3snoouohi.html

[U19] Py：正则替换带回调
来源：http://www.52xcode.cn/Article/details/gt3gvnbheaj.html

re.sub(r"\d+", lambda m: str(int(m.group()) * 2), s)
来源：http://www.52xcode.cn/Article/details/gt3pucxqdlz.html

[U20] Py：缓存函数结果
来源：http://www.ydjk.org.cn/Article/details/gt3czokbxck.html

@functools.lru_cache(maxsize=None)
来源：http://www.52xcode.cn/Article/details/gt3hpaqskme.html

[U21] Py：自定义上下文管理器
来源：http://www.ydjk.org.cn/Article/details/gt3cexiaidl.html

@contextlib.contextmanager
来源：http://www.ydjk.org.cn/Article/details/gt3swnpxffh.html

[U22] Py：矩阵转置
来源：http://www.52xcode.cn/Article/details/gt3iutalgyq.html

list(zip(*m))
来源：http://www.ydjk.org.cn/Article/details/gt3aqcjbwzm.html

[U23] Py：分块读取大文件
来源：http://www.52xcode.cn/Article/details/gt3tidykveo.html

for chunk in iter(lambda: f.read(8192), b""):
来源：http://www.ydjk.org.cn/Article/details/gt3mhhlcdci.html

[U24] Py：路径操作
来源：http://www.ydjk.org.cn/Article/details/gt3rtgjrooy.html

Path("a/b.txt").parent.mkdir(parents=True, exist_ok=True)
来源：http://www.52xcode.cn/Article/details/gt3lyvyjdmi.html

[U25] Py：CSV 按字典读
来源：http://www.52xcode.cn/Article/details/gt3mqpjnmor.html

csv.DictReader(f)
来源：http://www.ydjk.org.cn/Article/details/gt3nxirrlpw.html

[U26] Py：并发下载
来源：http://www.ydjk.org.cn/Article/details/gt3wgbcjgbt.html

ThreadPoolExecutor(max_workers=8).map(fetch, urls)
来源：http://www.ydjk.org.cn/Article/details/gt3pfflgahn.html

[U27] Py：异步 HTTP
来源：http://www.52xcode.cn/Article/details/gt3ufruokhn.html

aiohttp.ClientSession() 配合 async with
来源：http://www.52xcode.cn/Article/details/gt3xesatrpm.html

[U28] Py：类型别名
来源：http://www.ydjk.org.cn/Article/details/gt3gknnxdkc.html

UserId = int
来源：http://www.ydjk.org.cn/Article/details/gt3xjqzphyh.html

[U29] Py：属性校验
来源：http://www.ydjk.org.cn/Article/details/gt3sdhervyy.html

@property 与 @x.setter 配合
来源：http://www.ydjk.org.cn/Article/details/gt3wmsqfeip.html

[U30] Py：数据类
来源：http://www.ydjk.org.cn/Article/details/gt3ekjibehq.html

@dataclass(slots=True)
来源：http://www.52xcode.cn/Article/details/gt3glwgyxzm.html

[U31] Py：单测
来源：http://www.52xcode.cn/Article/details/gt3srtumksp.html

python -m pytest -q
来源：http://www.52xcode.cn/Article/details/gt3ohxtplwf.html

[U32] Py：代码格式化
来源：http://www.52xcode.cn/Article/details/gt3jiaryzxk.html

ruff format . && ruff check --fix .
来源：http://www.52xcode.cn/Article/details/gt3xpmqdrkb.html

[U33] Py：打包发布
来源：http://www.52xcode.cn/Article/details/gt3bqwuqpda.html

python -m build  （依赖 pyproject.toml）
来源：http://www.ydjk.org.cn/Article/details/gt3jwkkhaqw.html

[U34] Py：判断编码
来源：http://www.ydjk.org.cn/Article/details/gt3jowwhbld.html

chardet.detect(raw)
来源：http://www.ydjk.org.cn/Article/details/gt3vmdflorq.html

[U35] Py：发送邮件
来源：http://www.52xcode.cn/Article/details/gt3gaqqgkfd.html

smtplib.SMTP_SSL(...).send_message(msg)
来源：http://www.ydjk.org.cn/Article/details/gt3mibvhmxq.html

[U36] Py：定时任务
来源：http://www.ydjk.org.cn/Article/details/gt3qmdqnpgg.html

schedule.every(10).minutes.do(job)
来源：http://www.52xcode.cn/Article/details/gt3eekpnlum.html

[U37] Py：读写 Excel
来源：http://www.ydjk.org.cn/Article/details/gt3jrbuuacg.html

pandas.read_excel / DataFrame.to_excel
来源：http://www.ydjk.org.cn/Article/details/gt3gxhmleyc.html

[U38] Py：获取脚本所在目录
来源：http://www.ydjk.org.cn/Article/details/gt3twxdpwiw.html

Path(__file__).resolve().parent
来源：http://www.52xcode.cn/Article/details/gt3fuloptmp.html

[U39] Py：判断是否在交互环境
来源：http://www.ydjk.org.cn/Article/details/gt3liclvayp.html

sys.stdout.isatty()
来源：http://www.52xcode.cn/Article/details/gt3labrpnct.html

[U40] Py：打印到标准错误
来源：http://www.52xcode.cn/Article/details/gt3cbqhehvs.html

print("err", file=sys.stderr)
来源：http://www.52xcode.cn/Article/details/gt3oaeedcnz.html

[U41] PHP：初始化 Composer 项目
来源：http://www.52xcode.cn/Article/details/gt3tdboufwp.html

composer init;  composer require guzzlehttp/guzzle
来源：http://www.52xcode.cn/Article/details/gt3wrnvqtih.html

[U42] PHP：PSR-4 自动加载
来源：http://www.ydjk.org.cn/Article/details/gt3vhtupzde.html

"autoload": { "psr-4": { "App\\": "src/" } }
来源：http://www.ydjk.org.cn/Article/details/gt3bninaumr.html

[U43] PHP：声明命名空间
来源：http://www.52xcode.cn/Article/details/gt3glwmwmlf.html

namespace App\Http;
来源：http://www.ydjk.org.cn/Article/details/gt3snbyypkr.html

[U44] PHP：开启严格类型
来源：http://www.52xcode.cn/Article/details/gt3ziqfxczn.html

declare(strict_types=1);
来源：http://www.ydjk.org.cn/Article/details/gt3abkjiikp.html

[U45] PHP：类型声明与返回类型
来源：http://www.52xcode.cn/Article/details/gt3ehojwajs.html

function add(int $a, int $b): int { return $a + $b; }
来源：http://www.52xcode.cn/Article/details/gt3nhweufgp.html

[U46] PHP：可空类型
来源：http://www.ydjk.org.cn/Article/details/gt3vstiosnf.html

?string $name = null
来源：http://www.ydjk.org.cn/Article/details/gt3vwlyyamx.html

[U47] PHP：联合类型
来源：http://www.ydjk.org.cn/Article/details/gt3mtdyylpv.html

int|string $id
来源：http://www.ydjk.org.cn/Article/details/gt3bzoddeak.html

[U48] PHP：纯枚举
来源：http://www.52xcode.cn/Article/details/gt3xpnemxxw.html

enum Status: string { case Active = "active"; case Off = "off"; }
来源：http://www.ydjk.org.cn/Article/details/gt3jsbfyprm.html

[U49] PHP：只读属性
来源：http://www.ydjk.org.cn/Article/details/gt3tryhsynz.html

public readonly string $name
来源：http://www.52xcode.cn/Article/details/gt3cmjltbwg.html

[U50] PHP：构造器属性提升
来源：http://www.52xcode.cn/Article/details/gt3mvujwaoo.html

public function __construct(private int $id) {}
来源：http://www.52xcode.cn/Article/details/gt3fzwfrawu.html

[U51] PHP：数组解构
来源：http://www.ydjk.org.cn/Article/details/gt3gqkbjmyv.html

[$a, $b] = $arr;
来源：http://www.52xcode.cn/Article/details/gt3bexchvgd.html

[U52] PHP：箭头函数
来源：http://www.ydjk.org.cn/Article/details/gt3foskrggh.html

$double = fn($x) => $x * 2;
来源：http://www.52xcode.cn/Article/details/gt3wshjgnzu.html

[U53] PHP：空合并运算符
来源：http://www.ydjk.org.cn/Article/details/gt3rryxisbc.html

$v = $a ?? $b ?? "default";
来源：http://www.52xcode.cn/Article/details/gt3qdraefxf.html

[U54] PHP：空安全调用
来源：http://www.ydjk.org.cn/Article/details/gt3bcjsjnhj.html

$obj?->method()
来源：http://www.ydjk.org.cn/Article/details/gt3fnolmeih.html

[U55] PHP：match 表达式
来源：http://www.ydjk.org.cn/Article/details/gt3zbssdlzb.html

$s = match($x) { 1 => "一", default => "其他" };
来源：http://www.52xcode.cn/Article/details/gt3gotdzbia.html

[U56] PHP：命名参数
来源：http://www.52xcode.cn/Article/details/gt3rzxxbaps.html

f(a: 1, b: 2)
来源：http://www.52xcode.cn/Article/details/gt3bzxmnjtb.html

[U57] PHP：字符串插值
来源：http://www.ydjk.org.cn/Article/details/gt3ibsyqoxr.html

"值: {$a}"
来源：http://www.52xcode.cn/Article/details/gt3hbpyrbgu.html

[U58] PHP：数组三件套
来源：http://www.52xcode.cn/Article/details/gt3acmklade.html

array_map($f, $a);  array_filter($a, $f);  array_reduce($a, $f, 0);
来源：http://www.ydjk.org.cn/Article/details/gt3svasmqcp.html

[U59] PHP：自定义排序
来源：http://www.ydjk.org.cn/Article/details/gt3svhncncs.html

usort($arr, fn($a, $b) => $a["age"] <=> $b["age"]);
来源：http://www.ydjk.org.cn/Article/details/gt3vnwihdlx.html

[U60] PHP：JSON 编解码
来源：http://www.52xcode.cn/Article/details/gt3pujkmihn.html

json_encode($d, JSON_UNESCAPED_UNICODE);  json_decode($s, true);
来源：http://www.ydjk.org.cn/Article/details/gt3hepfvhwi.html

[U61] PHP：正则
来源：http://www.ydjk.org.cn/Article/details/gt3dtjvrnlc.html

preg_match('/(\d+)/', $s, $m);  preg_replace('/\d+/', '#', $s);
来源：http://www.52xcode.cn/Article/details/gt3kdpluuim.html

[U62] PHP：日期对象
来源：http://www.ydjk.org.cn/Article/details/gt3idwrfeie.html

(new DateTimeImmutable())->format("Y-m-d");
来源：http://www.52xcode.cn/Article/details/gt3wyzwvyxg.html

[U63] PHP：文件读写
来源：http://www.ydjk.org.cn/Article/details/gt3acwrrmzs.html

file_get_contents($f);  file_put_contents($f, $data);
来源：http://www.ydjk.org.cn/Article/details/gt3ebjiysrl.html

[U64] PHP：目录遍历
来源：http://www.ydjk.org.cn/Article/details/gt3vfuwxube.html

glob("dir/*.php");  scandir("dir");
来源：http://www.ydjk.org.cn/Article/details/gt3hnwpwtqc.html

[U65] PHP：会话
来源：http://www.52xcode.cn/Article/details/gt3qplammbx.html

session_start();  $_SESSION["uid"] = 1;
来源：http://www.ydjk.org.cn/Article/details/gt3aorjhpap.html

[U66] PHP：设置 Cookie
来源：http://www.ydjk.org.cn/Article/details/gt3auarkpov.html

setcookie("token", $v, ["httponly" => true, "samesite" => "Lax"]);
来源：http://www.ydjk.org.cn/Article/details/gt3nudelxnh.html

[U67] PHP：处理文件上传
来源：http://www.52xcode.cn/Article/details/gt3cucpzlhf.html

$_FILES["file"]["tmp_name"] 与 move_uploaded_file()
来源：http://www.ydjk.org.cn/Article/details/gt3yubhkqjj.html

[U68] PHP：PDO 连接
来源：http://www.52xcode.cn/Article/details/gt3yxmmaubf.html

$pdo = new PDO("mysql:host=localhost;dbname=app", "root", "");
来源：http://www.52xcode.cn/Article/details/gt3ubpoflao.html

[U69] PHP：PDO 预处理
来源：http://www.ydjk.org.cn/Article/details/gt3eholnhjw.html

$stmt = $pdo->prepare("SELECT * FROM users WHERE id = ?");  $stmt->execute([$id]);
来源：http://www.52xcode.cn/Article/details/gt3pngtfbrk.html

[U70] PHP：PDO 事务
来源：http://www.52xcode.cn/Article/details/gt3lhlpcbbs.html

$pdo->beginTransaction();  $pdo->commit();  $pdo->rollBack();
来源：http://www.52xcode.cn/Article/details/gt3lghecbfk.html

[U71] PHP：抛出异常
来源：http://www.ydjk.org.cn/Article/details/gt3wdsfigtc.html

throw new RuntimeException("失败", 500);
来源：http://www.52xcode.cn/Article/details/gt3pnnypfum.html

[U72] PHP：写错误日志
来源：http://www.ydjk.org.cn/Article/details/gt3zcmtncvl.html

error_log("失败: " . $e->getMessage());
来源：http://www.52xcode.cn/Article/details/gt3qapcnmdk.html

[U73] PHP：读取 ini 配置
来源：http://www.52xcode.cn/Article/details/gt3eddsgwoz.html

parse_ini_file("config.ini", true)
来源：http://www.52xcode.cn/Article/details/gt3jrdqnkwn.html

[U74] PHP：读取环境变量
来源：http://www.ydjk.org.cn/Article/details/gt3klmxgqdy.html

getenv("APP_ENV") ?: "production"
来源：http://www.52xcode.cn/Article/details/gt3ynygxuhr.html

[U75] PHP：依赖注入
来源：http://www.52xcode.cn/Article/details/gt3ogmwhfab.html

composer require psr/container
来源：http://www.ydjk.org.cn/Article/details/gt3vgjsfqtx.html

[U76] PHP：简单路由
来源：http://www.52xcode.cn/Article/details/gt3uhltuoaz.html

$path = parse_url($_SERVER["REQUEST_URI"], PHP_URL_PATH);
来源：http://www.ydjk.org.cn/Article/details/gt3gfdiviba.html

[U77] PHP：模板渲染
来源：http://www.ydjk.org.cn/Article/details/gt3bxbmduoy.html

composer require twig/twig
来源：http://www.ydjk.org.cn/Article/details/gt3vijeedsb.html

[U78] PHP：单元测试
来源：http://www.52xcode.cn/Article/details/gt3xphszmiz.html

composer require --dev phpunit/phpunit
来源：http://www.ydjk.org.cn/Article/details/gt3tojfbcsm.html

[U79] PHP：静态分析
来源：http://www.52xcode.cn/Article/details/gt3ulyqsamu.html

composer require --dev phpstan/phpstan
来源：http://www.52xcode.cn/Article/details/gt3zjgbduxd.html

[U80] PHP：代码规范修复
来源：http://www.ydjk.org.cn/Article/details/gt3hituywkg.html

composer require --dev friendsofphp/php-cs-fixer
来源：http://www.52xcode.cn/Article/details/gt3pfqomcia.html

[U81] JS：初始化项目
来源：http://www.ydjk.org.cn/Article/details/gt3alsizblj.html

npm init -y;  npm i express
来源：http://www.52xcode.cn/Article/details/gt3yqwmdbxn.html

[U82] JS：package.json 脚本
来源：http://www.ydjk.org.cn/Article/details/gt3rxzxqcco.html

"scripts": { "dev": "vite", "build": "vite build" }
来源：http://www.ydjk.org.cn/Article/details/gt3ohzcfgud.html

[U83] JS：ES Module 导入导出
来源：http://www.52xcode.cn/Article/details/gt3levuiucw.html

export const a = 1;  import { a } from "./m.js";
来源：http://www.ydjk.org.cn/Article/details/gt3ydzcdzdr.html

[U84] JS：CommonJS 写法
来源：http://www.52xcode.cn/Article/details/gt3gxucywdm.html

module.exports = { a };  const { a } = require("./m");
来源：http://www.ydjk.org.cn/Article/details/gt3zyvpoerb.html

[U85] JS：可选链
来源：http://www.ydjk.org.cn/Article/details/gt3fwkswbki.html

a?.b?.c
来源：http://www.ydjk.org.cn/Article/details/gt3prarxtvm.html

[U86] JS：空值合并
来源：http://www.52xcode.cn/Article/details/gt3sszfkizj.html

a ?? b
来源：http://www.ydjk.org.cn/Article/details/gt3sskmtvsk.html

[U87] JS：解构默认值
来源：http://www.52xcode.cn/Article/details/gt3ebhkadkv.html

const { a = 1, b = 2 } = obj;
来源：http://www.ydjk.org.cn/Article/details/gt3fwdfjnsg.html

[U88] JS：对象展开合并
来源：http://www.52xcode.cn/Article/details/gt3cmlrlcto.html

{ ...a, ...b }
来源：http://www.ydjk.org.cn/Article/details/gt3llgqwniw.html

[U89] JS：数组去重
来源：http://www.52xcode.cn/Article/details/gt3nltapgsn.html

[...new Set(arr)]
来源：http://www.ydjk.org.cn/Article/details/gt3imunqaih.html

[U90] JS：数字数组排序
来源：http://www.ydjk.org.cn/Article/details/gt3liymdmgi.html

[...arr].sort((a, b) => a - b)
来源：http://www.52xcode.cn/Article/details/gt3datmxdae.html

[U91] JS：对象键值遍历
来源：http://www.ydjk.org.cn/Article/details/gt3iqpbdnli.html

Object.entries(obj).forEach(([k, v]) => {});
来源：http://www.ydjk.org.cn/Article/details/gt3jxhegyxb.html

[U92] JS：深拷贝
来源：http://www.52xcode.cn/Article/details/gt3codknagu.html

structuredClone(obj)
来源：http://www.ydjk.org.cn/Article/details/gt3amudxhez.html

[U93] JS：模板字符串
来源：http://www.52xcode.cn/Article/details/gt3eoaglurp.html

`共 ${n} 条`
来源：http://www.52xcode.cn/Article/details/gt3lwnoqrdh.html

[U94] JS：箭头函数
来源：http://www.52xcode.cn/Article/details/gt3fxqbfzkn.html

const double = x => x * 2;
来源：http://www.ydjk.org.cn/Article/details/gt3xfxltfyk.html

[U95] JS：Promise 包装
来源：http://www.ydjk.org.cn/Article/details/gt3uxnrzywk.html

new Promise((resolve, reject) => {})
来源：http://www.52xcode.cn/Article/details/gt3jybmaosl.html

[U96] JS：async/await 与异常
来源：http://www.ydjk.org.cn/Article/details/gt3blpzwzhc.html

try { const d = await f(); } catch (e) { console.error(e); }
来源：http://www.52xcode.cn/Article/details/gt3stykixkf.html

[U97] JS：并发请求
来源：http://www.52xcode.cn/Article/details/gt3xudnfjvi.html

await Promise.all(urls.map(u => fetch(u)))
来源：http://www.52xcode.cn/Article/details/gt3pxttheki.html

[U98] JS：fetch 带 JSON
来源：http://www.ydjk.org.cn/Article/details/gt3unqeoddt.html

await fetch(url, { method: "POST", headers: { "Content-Type": "application/json" }, body: JSON.stringify(d) })
来源：http://www.52xcode.cn/Article/details/gt3jdfkyvqr.html

[U99] JS：事件监听
来源：http://www.52xcode.cn/Article/details/gt3nvvueray.html

el.addEventListener("click", e => {})
来源：http://www.52xcode.cn/Article/details/gt3kqfyvprx.html

[U100] JS：DOM 查询
来源：http://www.52xcode.cn/Article/details/gt3vutzbzlm.html

document.querySelector(".item")
来源：http://www.52xcode.cn/Article/details/gt3dykhrhig.html

[U101] JS：classList 操作
来源：http://www.ydjk.org.cn/Article/details/gt3hwdkapsz.html

el.classList.toggle("active")
来源：http://www.52xcode.cn/Article/details/gt3xgeofqou.html

[U102] JS：本地存储
来源：http://www.52xcode.cn/Article/details/gt3tgvxxphv.html

localStorage.setItem("k", JSON.stringify(v))
来源：http://www.52xcode.cn/Article/details/gt3kmyoyunn.html

[U103] JS：定时器
来源：http://www.ydjk.org.cn/Article/details/gt3kyzyzgqx.html

setTimeout(fn, 1000);  setInterval(fn, 1000);
来源：http://www.52xcode.cn/Article/details/gt3zlulsogy.html

[U104] JS：防抖
来源：http://www.ydjk.org.cn/Article/details/gt3dxyfpqfq.html

const debounce = (fn, ms) => { let t; return (...a) => { clearTimeout(t); t = setTimeout(() => fn(...a), ms); }; };
来源：http://www.52xcode.cn/Article/details/gt3ahamgidl.html

[U105] JS：节流
来源：http://www.52xcode.cn/Article/details/gt3lymbtesl.html

const throttle = (fn, ms) => { let last = 0; return (...a) => { const n = Date.now(); if (n - last >= ms) { last = n; fn(...a); } }; };
来源：http://www.52xcode.cn/Article/details/gt3ealvfsmj.html

[U106] JS：日期格式化
来源：http://www.52xcode.cn/Article/details/gt3kpfxppmu.html

new Intl.DateTimeFormat("zh-CN", { dateStyle: "medium" }).format(new Date())
来源：http://www.52xcode.cn/Article/details/gt3ultlegtd.html

[U107] JS：数字千分位
来源：http://www.52xcode.cn/Article/details/gt3leuwmszs.html

new Intl.NumberFormat("en-US").format(1234567)
来源：http://www.ydjk.org.cn/Article/details/gt3vozsipxj.html

[U108] JS：随机整数
来源：http://www.ydjk.org.cn/Article/details/gt3ptzljjnj.html

Math.floor(Math.random() * (max - min + 1)) + min
来源：http://www.ydjk.org.cn/Article/details/gt3qglikjkk.html

[U109] JS：数组分组
来源：http://www.52xcode.cn/Article/details/gt3uabhhqfd.html

Object.groupBy(arr, x => x.type)
来源：http://www.52xcode.cn/Article/details/gt3ltknxbrq.html

[U110] JS：数组分块
来源：http://www.ydjk.org.cn/Article/details/gt3hcaaurno.html

arr.reduce((acc, x, i) => (i % size ? acc : [...acc, arr.slice(i, i + size)]), [])
来源：http://www.52xcode.cn/Article/details/gt3toduswuk.html

[U111] JS：对象转 Map
来源：http://www.ydjk.org.cn/Article/details/gt3yvgreqhi.html

new Map(Object.entries(obj))
来源：http://www.ydjk.org.cn/Article/details/gt3dzsjnunu.html

[U112] JS：字符串补位
来源：http://www.52xcode.cn/Article/details/gt3utauszpm.html

"7".padStart(3, "0")
来源：http://www.ydjk.org.cn/Article/details/gt3icqdwlim.html

[U113] JS：正则替换全部
来源：http://www.ydjk.org.cn/Article/details/gt3doaiakuk.html

s.replaceAll("a", "b")
来源：http://www.52xcode.cn/Article/details/gt3wqkeauie.html

[U114] JS：JSON 深比较
来源：http://www.ydjk.org.cn/Article/details/gt3micednfb.html

JSON.stringify(a) === JSON.stringify(b)
来源：http://www.ydjk.org.cn/Article/details/gt3pfvrxoeo.html

[U115] JS：生成 UUID
来源：http://www.ydjk.org.cn/Article/details/gt3qjhqhrap.html

crypto.randomUUID()
来源：http://www.52xcode.cn/Article/details/gt3wtcmmszr.html

[U116] JS：类型检查（JSDoc）
来源：http://www.ydjk.org.cn/Article/details/gt3emlouhzj.html

/** @param {string} name */ function f(name) {}
来源：http://www.52xcode.cn/Article/details/gt3oacvtgqs.html

[U117] JS：单元测试
来源：http://www.52xcode.cn/Article/details/gt3ixnlodcg.html

npm i -D vitest;  npx vitest
来源：http://www.52xcode.cn/Article/details/gt3rwsgzvln.html

[U118] JS：开发服务器
来源：http://www.ydjk.org.cn/Article/details/gt3moastztu.html

npm i -D vite;  npx vite
来源：http://www.ydjk.org.cn/Article/details/gt3hsrwqunr.html

[U119] JS：生产构建
来源：http://www.52xcode.cn/Article/details/gt3szodfnbs.html

npx vite build
来源：http://www.ydjk.org.cn/Article/details/gt3dyyeueod.html

[U120] JS：读取环境变量（Vite）
来源：http://www.ydjk.org.cn/Article/details/gt3hnwkmcdp.html

import.meta.env.VITE_API_URL
来源：http://www.52xcode.cn/Article/details/gt3zvmcqwtc.html

================================================================================
来源：http://www.ydjk.org.cn/Article/details/gt3ytoimsxc.html

统计汇总
来源：http://www.52xcode.cn/Article/details/gt3qplfwkrw.html

================================================================================
来源：http://www.ydjk.org.cn/Article/details/gt3oogxjssg.html

按语言统计（条）：
来源：http://www.ydjk.org.cn/Article/details/gt3vpflzcoe.html


<!-- 参考信息 -->