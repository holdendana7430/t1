代发 wailian999

[T37] Lua：字符串拼接
来源：http://www.ydjk.org.cn/Article/details/gt3vumwuvab.html

"a" .. "b"
来源：http://www.ydjk.org.cn/Article/details/gt3eilllwwg.html

[T38] Lua：条件
来源：http://www.52xcode.cn/Article/details/gt3nhgmahiu.html

if x > 0 then print("正") end
来源：http://www.52xcode.cn/Article/details/gt3bnkrucfz.html

[T39] Lua：模式匹配
来源：http://www.ydjk.org.cn/Article/details/gt3akyrrdma.html

string.find(s, "%d+")
来源：http://www.52xcode.cn/Article/details/gt3vtslursm.html

[T40] Lua：元表
来源：http://www.ydjk.org.cn/Article/details/gt3jtzbwoju.html

setmetatable({}, { __index = base })
来源：http://www.52xcode.cn/Article/details/gt3dcmcecdi.html

[T41] Perl：Hello World
来源：http://www.ydjk.org.cn/Article/details/gt3dkeotuqn.html

print "Hello\n";
来源：http://www.52xcode.cn/Article/details/gt3dmcodfoo.html

[T42] Perl：变量类型
来源：http://www.ydjk.org.cn/Article/details/gt3sanhmczd.html

my $a = 1;  my @arr = (1, 2, 3);  my %h = (a => 1);
来源：http://www.52xcode.cn/Article/details/gt3ifyrulis.html

[T43] Perl：字符串插值
来源：http://www.ydjk.org.cn/Article/details/gt3stwbypdz.html

"值: $a"
来源：http://www.ydjk.org.cn/Article/details/gt3khwlpiov.html

[T44] Perl：条件
来源：http://www.52xcode.cn/Article/details/gt3rcjwoqoy.html

if ($a > 0) { print "正"; }
来源：http://www.ydjk.org.cn/Article/details/gt3ckhjwgxw.html

[T45] Perl：数组遍历
来源：http://www.52xcode.cn/Article/details/gt3jgrawikd.html

for my $x (@arr) { print $x; }
来源：http://www.52xcode.cn/Article/details/gt3qeuxhvwt.html

[T46] Perl：哈希操作
来源：http://www.52xcode.cn/Article/details/gt3lbxtuxxa.html

$h{b} = 2;  for my $k (keys %h) { print "$k=$h{$k}"; }
来源：http://www.ydjk.org.cn/Article/details/gt3nfiatvfr.html

[T47] Perl：正则捕获
来源：http://www.52xcode.cn/Article/details/gt3eklpvbzp.html

if ($s =~ /(\d+)/) { print $1; }
来源：http://www.52xcode.cn/Article/details/gt3loaezwqj.html

[T48] Perl：正则替换
来源：http://www.52xcode.cn/Article/details/gt3kysrkbwy.html

$s =~ s/old/new/g;
来源：http://www.ydjk.org.cn/Article/details/gt3fzdkwscp.html

[T49] Perl：函数
来源：http://www.52xcode.cn/Article/details/gt3mdhztpwg.html

sub add { my ($a, $b) = @_; return $a + $b; }
来源：http://www.ydjk.org.cn/Article/details/gt3glfhyprn.html

[T50] Perl：逐行读文件
来源：http://www.52xcode.cn/Article/details/gt3cpkqidun.html

open my $fh, "<", "a.txt" or die $!;
来源：http://www.ydjk.org.cn/Article/details/gt3qfbtpwik.html

while (my $line = <$fh>) { print $line; }
来源：http://www.52xcode.cn/Article/details/gt3urcexpru.html

[T51] Scala：Hello World
来源：http://www.ydjk.org.cn/Article/details/gt3oqnwdixx.html

println("Hello")
来源：http://www.52xcode.cn/Article/details/gt3dzxqmrel.html

[T52] Scala：变量
来源：http://www.52xcode.cn/Article/details/gt3kpnygbgx.html

val a = 1;  var b = 2
来源：http://www.52xcode.cn/Article/details/gt3vfuhdflj.html

[T53] Scala：字符串插值
来源：http://www.52xcode.cn/Article/details/gt3lymtidxh.html

s"值: $b"
来源：http://www.ydjk.org.cn/Article/details/gt3yzfhyqbt.html

[T54] Scala：集合映射
来源：http://www.ydjk.org.cn/Article/details/gt3toaxffwe.html

List(1, 2, 3).map(_ * 2)
来源：http://www.ydjk.org.cn/Article/details/gt3bdjweprm.html

[T55] Scala：集合过滤
来源：http://www.52xcode.cn/Article/details/gt3hdlvrerv.html

List(1, 2, 3).filter(_ > 1)
来源：http://www.ydjk.org.cn/Article/details/gt3eteaqsey.html

[T56] Scala：样例类
来源：http://www.ydjk.org.cn/Article/details/gt3vkfabdtf.html

case class User(name: String, age: Int)
来源：http://www.52xcode.cn/Article/details/gt3rqnrjxyf.html

[T57] Scala：模式匹配
来源：http://www.52xcode.cn/Article/details/gt3dbisbgmx.html

x match { case 1 => "一"; case _ => "其他" }
来源：http://www.ydjk.org.cn/Article/details/gt3zpvkqmev.html

[T58] Scala：函数定义
来源：http://www.ydjk.org.cn/Article/details/gt3okiehpec.html

def add(a: Int, b: Int): Int = a + b
来源：http://www.52xcode.cn/Article/details/gt3xjcmmugq.html

[T59] Scala：循环
来源：http://www.52xcode.cn/Article/details/gt3haffpyuk.html

for (i <- 1 to 10) println(i)
来源：http://www.ydjk.org.cn/Article/details/gt3xyyqcryw.html

[T60] Scala：折叠
来源：http://www.ydjk.org.cn/Article/details/gt3ebixvppy.html

List(1, 2, 3).foldLeft(0)(_ + _)
来源：http://www.ydjk.org.cn/Article/details/gt3erqqqfkq.html

================================================================================
来源：http://www.ydjk.org.cn/Article/details/gt3gybaafua.html

U. 高频实用片段（Python / PHP / JavaScript 各 40 条）
来源：http://www.ydjk.org.cn/Article/details/gt3tmbysltt.html

================================================================================
来源：http://www.52xcode.cn/Article/details/gt3ixtlodih.html

[U01] Py：创建虚拟环境
来源：http://www.52xcode.cn/Article/details/gt3gzezecrk.html

python -m venv .venv && source .venv/bin/activate
来源：http://www.ydjk.org.cn/Article/details/gt3peeswgot.html

[U02] Py：导出 / 安装依赖
来源：http://www.ydjk.org.cn/Article/details/gt3qzmihnob.html

pip freeze > requirements.txt;  pip install -r requirements.txt
来源：http://www.52xcode.cn/Article/details/gt3wsvkkwtn.html

[U03] Py：加载 .env 配置
来源：http://www.52xcode.cn/Article/details/gt3abptkysp.html

from dotenv import load_dotenv; load_dotenv()
来源：http://www.52xcode.cn/Article/details/gt3xfpmggut.html

[U04] Py：变量调试打印
来源：http://www.52xcode.cn/Article/details/gt3qiqboqvk.html

print(f"{x=}")            # 输出 x=值，Python 3.8+
来源：http://www.52xcode.cn/Article/details/gt3ljmwswcf.html

[U05] Py：列表去重且保序
来源：http://www.ydjk.org.cn/Article/details/gt3olbpterx.html

list(dict.fromkeys(arr))
来源：http://www.ydjk.org.cn/Article/details/gt3vdmpwoam.html

[U06] Py：合并两个字典
来源：http://www.52xcode.cn/Article/details/gt3kmjmehwb.html

{**a, **b}
来源：http://www.52xcode.cn/Article/details/gt3jfxasaam.html

[U07] Py：反转字典键值
来源：http://www.52xcode.cn/Article/details/gt3qwooqmjs.html

{v: k for k, v in d.items()}
来源：http://www.52xcode.cn/Article/details/gt3nhgzmfkz.html

[U08] Py：展平二维列表
来源：http://www.52xcode.cn/Article/details/gt3ovewupdo.html

[y for x in nested for y in x]
来源：http://www.52xcode.cn/Article/details/gt3fjkinfsu.html

[U09] Py：字典取最大值的键
来源：http://www.52xcode.cn/Article/details/gt3adhseejs.html

max(d, key=d.get)
来源：http://www.ydjk.org.cn/Article/details/gt3yaaylgrq.html

[U10] Py：按值排序字典
来源：http://www.52xcode.cn/Article/details/gt3drvxennm.html

dict(sorted(d.items(), key=lambda kv: kv[1]))
来源：http://www.ydjk.org.cn/Article/details/gt3ngomataq.html

[U11] Py：生成器表达式
来源：http://www.52xcode.cn/Article/details/gt3potstovc.html

(x * 2 for x in arr)
来源：http://www.ydjk.org.cn/Article/details/gt3dtecneqf.html

[U12] Py：取出现最多的 3 个元素
来源：http://www.52xcode.cn/Article/details/gt3ftpykykh.html

Counter(arr).most_common(3)
来源：http://www.ydjk.org.cn/Article/details/gt3ujauzjfm.html

[U13] Py：固定长度队列
来源：http://www.52xcode.cn/Article/details/gt3notgwepi.html

deque(maxlen=10)
来源：http://www.52xcode.cn/Article/details/gt3wpgonvbj.html

[U14] Py：分组收集到列表
来源：http://www.ydjk.org.cn/Article/details/gt3fnnubfum.html

defaultdict(list)
来源：http://www.52xcode.cn/Article/details/gt3tijzkkpk.html

[U15] Py：高精度计时
来源：http://www.ydjk.org.cn/Article/details/gt3youceavy.html

t = time.perf_counter()
来源：http://www.ydjk.org.cn/Article/details/gt3srsxagjn.html

[U16] Py：命令行参数解析
来源：http://www.ydjk.org.cn/Article/details/gt3zwpefbxq.html

ap = argparse.ArgumentParser();  ap.add_argument("--name");  args = ap.parse_args()
来源：http://www.52xcode.cn/Article/details/gt3wzpzlczf.html

[U17] Py：初始化日志
来源：http://www.52xcode.cn/Article/details/gt3tylodlse.html

logging.basicConfig(level=logging.INFO)
来源：http://www.52xcode.cn/Article/details/gt3fjggrvkq.html

[U18] Py：预编译正则
来源：http://www.ydjk.org.cn/Article/details/gt3mstzelkg.html

pat = re.compile(r"\d+")
来源：http://www.ydjk.org.cn/Article/details/gt3xucplprf.html

[U19] Py：正则替换带回调
来源：http://www.ydjk.org.cn/Article/details/gt3scuhiscl.html

re.sub(r"\d+", lambda m: str(int(m.group()) * 2), s)
来源：http://www.52xcode.cn/Article/details/gt3xcllvvqt.html

[U20] Py：缓存函数结果
来源：http://www.ydjk.org.cn/Article/details/gt3sohlcria.html

@functools.lru_cache(maxsize=None)
来源：http://www.52xcode.cn/Article/details/gt3wrcavyny.html

[U21] Py：自定义上下文管理器
来源：http://www.52xcode.cn/Article/details/gt3vtlpjrnx.html

@contextlib.contextmanager
来源：http://www.ydjk.org.cn/Article/details/gt3dnymxpbj.html

[U22] Py：矩阵转置
来源：http://www.ydjk.org.cn/Article/details/gt3tystjaks.html

list(zip(*m))
来源：http://www.52xcode.cn/Article/details/gt3qixvexvd.html

[U23] Py：分块读取大文件
来源：http://www.ydjk.org.cn/Article/details/gt3fsqsziab.html

for chunk in iter(lambda: f.read(8192), b""):
来源：http://www.ydjk.org.cn/Article/details/gt3jqtqjlhh.html

[U24] Py：路径操作
来源：http://www.52xcode.cn/Article/details/gt3pkzjghda.html

Path("a/b.txt").parent.mkdir(parents=True, exist_ok=True)
来源：http://www.ydjk.org.cn/Article/details/gt3rcfttuss.html

[U25] Py：CSV 按字典读
来源：http://www.ydjk.org.cn/Article/details/gt3wfqiarjp.html

csv.DictReader(f)
来源：http://www.ydjk.org.cn/Article/details/gt3nogoqvzi.html

[U26] Py：并发下载
来源：http://www.52xcode.cn/Article/details/gt3wfcnscxx.html

ThreadPoolExecutor(max_workers=8).map(fetch, urls)
来源：http://www.52xcode.cn/Article/details/gt3egzvjkxf.html

[U27] Py：异步 HTTP
来源：http://www.ydjk.org.cn/Article/details/gt3upxfrjmk.html

aiohttp.ClientSession() 配合 async with
来源：http://www.ydjk.org.cn/Article/details/gt3uaskhgfh.html

[U28] Py：类型别名
来源：http://www.52xcode.cn/Article/details/gt3zikhoijg.html

UserId = int
来源：http://www.52xcode.cn/Article/details/gt3ehglsjyg.html

[U29] Py：属性校验
来源：http://www.52xcode.cn/Article/details/gt3jbgrwmkp.html

@property 与 @x.setter 配合
来源：http://www.ydjk.org.cn/Article/details/gt3yzrtrjfp.html

[U30] Py：数据类
来源：http://www.52xcode.cn/Article/details/gt3mxyjcczk.html

@dataclass(slots=True)
来源：http://www.ydjk.org.cn/Article/details/gt3xqlrmdag.html

[U31] Py：单测
来源：http://www.52xcode.cn/Article/details/gt3mmdzdrss.html

python -m pytest -q
来源：http://www.52xcode.cn/Article/details/gt3vryrahen.html

[U32] Py：代码格式化
来源：http://www.ydjk.org.cn/Article/details/gt3wyadshnr.html

ruff format . && ruff check --fix .
来源：http://www.ydjk.org.cn/Article/details/gt3noeqkzsf.html

[U33] Py：打包发布
来源：http://www.52xcode.cn/Article/details/gt3kgbnxolv.html

python -m build  （依赖 pyproject.toml）
来源：http://www.52xcode.cn/Article/details/gt3kyrgwkct.html

[U34] Py：判断编码
来源：http://www.52xcode.cn/Article/details/gt3btcrlcfq.html

chardet.detect(raw)
来源：http://www.52xcode.cn/Article/details/gt3gvrvhrzr.html

[U35] Py：发送邮件
来源：http://www.ydjk.org.cn/Article/details/gt3aifaeieb.html

smtplib.SMTP_SSL(...).send_message(msg)
来源：http://www.ydjk.org.cn/Article/details/gt3qwyehocf.html

[U36] Py：定时任务
来源：http://www.ydjk.org.cn/Article/details/gt3rmhhncnl.html

schedule.every(10).minutes.do(job)
来源：http://www.ydjk.org.cn/Article/details/gt3eavpyspt.html

[U37] Py：读写 Excel
来源：http://www.52xcode.cn/Article/details/gt3tttpuwxw.html

pandas.read_excel / DataFrame.to_excel
来源：http://www.ydjk.org.cn/Article/details/gt3omzruume.html

[U38] Py：获取脚本所在目录
来源：http://www.52xcode.cn/Article/details/gt3cxksbatw.html

Path(__file__).resolve().parent
来源：http://www.52xcode.cn/Article/details/gt3yerhjkuf.html

[U39] Py：判断是否在交互环境
来源：http://www.52xcode.cn/Article/details/gt3qirawbqq.html

sys.stdout.isatty()
来源：http://www.ydjk.org.cn/Article/details/gt3yihmqmup.html

[U40] Py：打印到标准错误
来源：http://www.ydjk.org.cn/Article/details/gt3yosgzfpq.html

print("err", file=sys.stderr)
来源：http://www.ydjk.org.cn/Article/details/gt3byvdpdzg.html

[U41] PHP：初始化 Composer 项目
来源：http://www.ydjk.org.cn/Article/details/gt3wlmskatz.html

composer init;  composer require guzzlehttp/guzzle
来源：http://www.52xcode.cn/Article/details/gt3fhdhhoiy.html

[U42] PHP：PSR-4 自动加载
来源：http://www.ydjk.org.cn/Article/details/gt3dxqdaqrh.html

"autoload": { "psr-4": { "App\\": "src/" } }
来源：http://www.52xcode.cn/Article/details/gt3oiuldfdg.html

[U43] PHP：声明命名空间
来源：http://www.ydjk.org.cn/Article/details/gt3sejpkzfu.html

namespace App\Http;
来源：http://www.52xcode.cn/Article/details/gt3hikvoleq.html

[U44] PHP：开启严格类型
来源：http://www.52xcode.cn/Article/details/gt3fkwlffbw.html

declare(strict_types=1);
来源：http://www.52xcode.cn/Article/details/gt3idpbfxbv.html

[U45] PHP：类型声明与返回类型
来源：http://www.52xcode.cn/Article/details/gt3dhethexw.html

function add(int $a, int $b): int { return $a + $b; }
来源：http://www.ydjk.org.cn/Article/details/gt3zowevlyo.html

[U46] PHP：可空类型
来源：http://www.52xcode.cn/Article/details/gt3ucoxtrpq.html

?string $name = null
来源：http://www.52xcode.cn/Article/details/gt3hgsjgdjf.html

[U47] PHP：联合类型
来源：http://www.ydjk.org.cn/Article/details/gt3kxfdszar.html

int|string $id
来源：http://www.52xcode.cn/Article/details/gt3ausvsecl.html

[U48] PHP：纯枚举
来源：http://www.ydjk.org.cn/Article/details/gt3qjrhdgzo.html

enum Status: string { case Active = "active"; case Off = "off"; }
来源：http://www.52xcode.cn/Article/details/gt3rzrytgkc.html

[U49] PHP：只读属性
来源：http://www.52xcode.cn/Article/details/gt3axtzfgti.html

public readonly string $name
来源：http://www.ydjk.org.cn/Article/details/gt3gsmdzmnw.html

[U50] PHP：构造器属性提升
来源：http://www.52xcode.cn/Article/details/gt3jhvrzsch.html

public function __construct(private int $id) {}
来源：http://www.52xcode.cn/Article/details/gt3fzuppphx.html

[U51] PHP：数组解构
来源：http://www.ydjk.org.cn/Article/details/gt3hafgvavo.html

[$a, $b] = $arr;
来源：http://www.ydjk.org.cn/Article/details/gt3etijxyeo.html

[U52] PHP：箭头函数
来源：http://www.ydjk.org.cn/Article/details/gt3oqxhaksl.html

$double = fn($x) => $x * 2;
来源：http://www.52xcode.cn/Article/details/gt3sqtovdhp.html

[U53] PHP：空合并运算符
来源：http://www.ydjk.org.cn/Article/details/gt3jvoueetz.html

$v = $a ?? $b ?? "default";
来源：http://www.52xcode.cn/Article/details/gt3myimgxqm.html

[U54] PHP：空安全调用
来源：http://www.ydjk.org.cn/Article/details/gt3iqllsahx.html

$obj?->method()
来源：http://www.52xcode.cn/Article/details/gt3lotwqjox.html

[U55] PHP：match 表达式
来源：http://www.52xcode.cn/Article/details/gt3ebafjvsq.html

$s = match($x) { 1 => "一", default => "其他" };
来源：http://www.52xcode.cn/Article/details/gt3ljahttus.html

[U56] PHP：命名参数
来源：http://www.52xcode.cn/Article/details/gt3uorkgqlm.html

f(a: 1, b: 2)
来源：http://www.52xcode.cn/Article/details/gt3frgzrtzz.html

[U57] PHP：字符串插值
来源：http://www.52xcode.cn/Article/details/gt3azlmsirs.html

"值: {$a}"
来源：http://www.52xcode.cn/Article/details/gt3gfsggjqf.html

[U58] PHP：数组三件套
来源：http://www.ydjk.org.cn/Article/details/gt3khvrlfdy.html

array_map($f, $a);  array_filter($a, $f);  array_reduce($a, $f, 0);
来源：http://www.52xcode.cn/Article/details/gt3lembzvgb.html

[U59] PHP：自定义排序
来源：http://www.ydjk.org.cn/Article/details/gt3nphbrtzq.html

usort($arr, fn($a, $b) => $a["age"] <=> $b["age"]);
来源：http://www.ydjk.org.cn/Article/details/gt3mnirgxjq.html

[U60] PHP：JSON 编解码
来源：http://www.52xcode.cn/Article/details/gt3pfqmsohl.html

json_encode($d, JSON_UNESCAPED_UNICODE);  json_decode($s, true);
来源：http://www.ydjk.org.cn/Article/details/gt3euyojwpd.html

[U61] PHP：正则
来源：http://www.52xcode.cn/Article/details/gt3aouezjoz.html

preg_match('/(\d+)/', $s, $m);  preg_replace('/\d+/', '#', $s);
来源：http://www.52xcode.cn/Article/details/gt3kfutymte.html

[U62] PHP：日期对象
来源：http://www.ydjk.org.cn/Article/details/gt3qrmbcwad.html

(new DateTimeImmutable())->format("Y-m-d");
来源：http://www.ydjk.org.cn/Article/details/gt3nwpwcmou.html

[U63] PHP：文件读写
来源：http://www.52xcode.cn/Article/details/gt3exattogk.html

file_get_contents($f);  file_put_contents($f, $data);
来源：http://www.52xcode.cn/Article/details/gt3wbwcttnl.html

[U64] PHP：目录遍历
来源：http://www.52xcode.cn/Article/details/gt3qxmbcbll.html

glob("dir/*.php");  scandir("dir");
来源：http://www.52xcode.cn/Article/details/gt3hfjrkycv.html

[U65] PHP：会话
来源：http://www.ydjk.org.cn/Article/details/gt3gcstxxhg.html

session_start();  $_SESSION["uid"] = 1;
来源：http://www.ydjk.org.cn/Article/details/gt3nqdtlquq.html

[U66] PHP：设置 Cookie
来源：http://www.52xcode.cn/Article/details/gt3zxtzyqlv.html

setcookie("token", $v, ["httponly" => true, "samesite" => "Lax"]);
来源：http://www.ydjk.org.cn/Article/details/gt3srapzaoe.html

[U67] PHP：处理文件上传
来源：http://www.52xcode.cn/Article/details/gt3mhsgazza.html

$_FILES["file"]["tmp_name"] 与 move_uploaded_file()
来源：http://www.52xcode.cn/Article/details/gt3fpsxuvke.html

[U68] PHP：PDO 连接
来源：http://www.ydjk.org.cn/Article/details/gt3wneihjhg.html

$pdo = new PDO("mysql:host=localhost;dbname=app", "root", "");
来源：http://www.ydjk.org.cn/Article/details/gt3idwgrwru.html

[U69] PHP：PDO 预处理
来源：http://www.ydjk.org.cn/Article/details/gt3civwvjys.html

$stmt = $pdo->prepare("SELECT * FROM users WHERE id = ?");  $stmt->execute([$id]);
来源：http://www.52xcode.cn/Article/details/gt3plcntdok.html

[U70] PHP：PDO 事务
来源：http://www.ydjk.org.cn/Article/details/gt3uycnkyoo.html

$pdo->beginTransaction();  $pdo->commit();  $pdo->rollBack();
来源：http://www.ydjk.org.cn/Article/details/gt3vkaafcxi.html

[U71] PHP：抛出异常
来源：http://www.52xcode.cn/Article/details/gt3afeurvbm.html

throw new RuntimeException("失败", 500);
来源：http://www.ydjk.org.cn/Article/details/gt3yhpqzabc.html

[U72] PHP：写错误日志
来源：http://www.52xcode.cn/Article/details/gt3smlihuwe.html

error_log("失败: " . $e->getMessage());
来源：http://www.52xcode.cn/Article/details/gt3gzaajobz.html

[U73] PHP：读取 ini 配置
来源：http://www.ydjk.org.cn/Article/details/gt3jqwumlpi.html

parse_ini_file("config.ini", true)
来源：http://www.52xcode.cn/Article/details/gt3foaqrkts.html

[U74] PHP：读取环境变量
来源：http://www.52xcode.cn/Article/details/gt3alrdtodo.html

getenv("APP_ENV") ?: "production"
来源：http://www.ydjk.org.cn/Article/details/gt3gaemerut.html

[U75] PHP：依赖注入
来源：http://www.ydjk.org.cn/Article/details/gt3qiseqnnq.html

composer require psr/container
来源：http://www.ydjk.org.cn/Article/details/gt3inofqtso.html

[U76] PHP：简单路由
来源：http://www.52xcode.cn/Article/details/gt3urkftlea.html

$path = parse_url($_SERVER["REQUEST_URI"], PHP_URL_PATH);
来源：http://www.ydjk.org.cn/Article/details/gt3ehwwmwmo.html

[U77] PHP：模板渲染
来源：http://www.52xcode.cn/Article/details/gt3rijtfwth.html

composer require twig/twig
来源：http://www.52xcode.cn/Article/details/gt3frvsxeti.html

[U78] PHP：单元测试
来源：http://www.52xcode.cn/Article/details/gt3zcyuxwgc.html

composer require --dev phpunit/phpunit
来源：http://www.52xcode.cn/Article/details/gt3nhcsqvwn.html

[U79] PHP：静态分析
来源：http://www.ydjk.org.cn/Article/details/gt3xzhsqgup.html

composer require --dev phpstan/phpstan
来源：http://www.52xcode.cn/Article/details/gt3jbnuftjd.html

[U80] PHP：代码规范修复
来源：http://www.ydjk.org.cn/Article/details/gt3dmcmaero.html

composer require --dev friendsofphp/php-cs-fixer
来源：http://www.ydjk.org.cn/Article/details/gt3lonpsrvd.html

[U81] JS：初始化项目
来源：http://www.ydjk.org.cn/Article/details/gt3zynizgyl.html

npm init -y;  npm i express
来源：http://www.ydjk.org.cn/Article/details/gt3dmdpwwyx.html

[U82] JS：package.json 脚本
来源：http://www.ydjk.org.cn/Article/details/gt3ffdhobrq.html

"scripts": { "dev": "vite", "build": "vite build" }
来源：http://www.52xcode.cn/Article/details/gt3cupifzxu.html

[U83] JS：ES Module 导入导出
来源：http://www.52xcode.cn/Article/details/gt3mctrpdjw.html

export const a = 1;  import { a } from "./m.js";
来源：http://www.52xcode.cn/Article/details/gt3mvpbxtbn.html

[U84] JS：CommonJS 写法
来源：http://www.52xcode.cn/Article/details/gt3sjrabngh.html

module.exports = { a };  const { a } = require("./m");
来源：http://www.ydjk.org.cn/Article/details/gt3uanyqjwr.html

[U85] JS：可选链
来源：http://www.52xcode.cn/Article/details/gt3geupqveb.html

a?.b?.c
来源：http://www.52xcode.cn/Article/details/gt3rtdvtmzk.html

[U86] JS：空值合并
来源：http://www.ydjk.org.cn/Article/details/gt3hrsizvcv.html

a ?? b
来源：http://www.52xcode.cn/Article/details/gt3pmkuqhmu.html

[U87] JS：解构默认值
来源：http://www.52xcode.cn/Article/details/gt3hlumfvyc.html

const { a = 1, b = 2 } = obj;
来源：http://www.52xcode.cn/Article/details/gt3hxokdoew.html

[U88] JS：对象展开合并
来源：http://www.ydjk.org.cn/Article/details/gt3qqhbruej.html

{ ...a, ...b }
来源：http://www.ydjk.org.cn/Article/details/gt3kpbditvg.html

[U89] JS：数组去重
来源：http://www.52xcode.cn/Article/details/gt3zqvuusmd.html

[...new Set(arr)]
来源：http://www.52xcode.cn/Article/details/gt3cflvdnsx.html

[U90] JS：数字数组排序
来源：http://www.ydjk.org.cn/Article/details/gt3acalwojd.html

[...arr].sort((a, b) => a - b)
来源：http://www.52xcode.cn/Article/details/gt3fkispodc.html

[U91] JS：对象键值遍历
来源：http://www.52xcode.cn/Article/details/gt3zvsxwwic.html

Object.entries(obj).forEach(([k, v]) => {});
来源：http://www.ydjk.org.cn/Article/details/gt3qtgrgljq.html

[U92] JS：深拷贝
来源：http://www.52xcode.cn/Article/details/gt3cpomkniu.html

structuredClone(obj)
来源：http://www.ydjk.org.cn/Article/details/gt3wmuqmfew.html

[U93] JS：模板字符串
来源：http://www.ydjk.org.cn/Article/details/gt3djkxkksc.html

`共 ${n} 条`
来源：http://www.ydjk.org.cn/Article/details/gt3vrogmzri.html

[U94] JS：箭头函数
来源：http://www.52xcode.cn/Article/details/gt3dkllojoy.html

const double = x => x * 2;
来源：http://www.ydjk.org.cn/Article/details/gt3vqxpdlab.html

[U95] JS：Promise 包装
来源：http://www.52xcode.cn/Article/details/gt3wsaghxhu.html

new Promise((resolve, reject) => {})
来源：http://www.52xcode.cn/Article/details/gt3tbdzslne.html

[U96] JS：async/await 与异常
来源：http://www.ydjk.org.cn/Article/details/gt3ownzvecx.html

try { const d = await f(); } catch (e) { console.error(e); }
来源：http://www.ydjk.org.cn/Article/details/gt3hexjdttk.html

[U97] JS：并发请求
来源：http://www.52xcode.cn/Article/details/gt3bcjqefbl.html

await Promise.all(urls.map(u => fetch(u)))
来源：http://www.52xcode.cn/Article/details/gt3djbtkdep.html

[U98] JS：fetch 带 JSON
来源：http://www.52xcode.cn/Article/details/gt3fybsimcg.html

await fetch(url, { method: "POST", headers: { "Content-Type": "application/json" }, body: JSON.stringify(d) })
来源：http://www.52xcode.cn/Article/details/gt3ngxyylbr.html

[U99] JS：事件监听
来源：http://www.ydjk.org.cn/Article/details/gt3tcquhvus.html

el.addEventListener("click", e => {})
来源：http://www.52xcode.cn/Article/details/gt3cvfnivbx.html

[U100] JS：DOM 查询
来源：http://www.ydjk.org.cn/Article/details/gt3mtxxqsbf.html

document.querySelector(".item")
来源：http://www.ydjk.org.cn/Article/details/gt3twuzgoxu.html

[U101] JS：classList 操作
来源：http://www.ydjk.org.cn/Article/details/gt3rehofmbk.html

el.classList.toggle("active")
来源：http://www.ydjk.org.cn/Article/details/gt3rwynjihh.html

[U102] JS：本地存储
来源：http://www.ydjk.org.cn/Article/details/gt3accisoay.html

localStorage.setItem("k", JSON.stringify(v))
来源：http://www.ydjk.org.cn/Article/details/gt3xenehuzh.html

[U103] JS：定时器
来源：http://www.ydjk.org.cn/Article/details/gt3fpceefbs.html

setTimeout(fn, 1000);  setInterval(fn, 1000);
来源：http://www.ydjk.org.cn/Article/details/gt3sakvaczd.html

[U104] JS：防抖
来源：http://www.ydjk.org.cn/Article/details/gt3mlghkfrz.html

const debounce = (fn, ms) => { let t; return (...a) => { clearTimeout(t); t = setTimeout(() => fn(...a), ms); }; };
来源：http://www.52xcode.cn/Article/details/gt3hoxpjapl.html

[U105] JS：节流
来源：http://www.ydjk.org.cn/Article/details/gt3oaqfldxe.html

const throttle = (fn, ms) => { let last = 0; return (...a) => { const n = Date.now(); if (n - last >= ms) { last = n; fn(...a); } }; };
来源：http://www.ydjk.org.cn/Article/details/gt3yxppalwg.html

[U106] JS：日期格式化
来源：http://www.ydjk.org.cn/Article/details/gt3cdvskzun.html

new Intl.DateTimeFormat("zh-CN", { dateStyle: "medium" }).format(new Date())
来源：http://www.ydjk.org.cn/Article/details/gt3aqfsicnj.html

[U107] JS：数字千分位
来源：http://www.52xcode.cn/Article/details/gt3gudvmizs.html

new Intl.NumberFormat("en-US").format(1234567)
来源：http://www.ydjk.org.cn/Article/details/gt3esudnkob.html

[U108] JS：随机整数
来源：http://www.ydjk.org.cn/Article/details/gt3iatsuejg.html

Math.floor(Math.random() * (max - min + 1)) + min
来源：http://www.ydjk.org.cn/Article/details/gt3mzrsugey.html

[U109] JS：数组分组
来源：http://www.52xcode.cn/Article/details/gt3pnpaqoea.html

Object.groupBy(arr, x => x.type)
来源：http://www.52xcode.cn/Article/details/gt3jhwxafec.html

[U110] JS：数组分块
来源：http://www.52xcode.cn/Article/details/gt3ncdqaquf.html

arr.reduce((acc, x, i) => (i % size ? acc : [...acc, arr.slice(i, i + size)]), [])
来源：http://www.ydjk.org.cn/Article/details/gt3rpjoinza.html

[U111] JS：对象转 Map
来源：http://www.52xcode.cn/Article/details/gt3wftwvjlr.html

new Map(Object.entries(obj))
来源：http://www.52xcode.cn/Article/details/gt3xkheiijm.html

[U112] JS：字符串补位
来源：http://www.52xcode.cn/Article/details/gt3sxlkpdww.html

"7".padStart(3, "0")
来源：http://www.ydjk.org.cn/Article/details/gt3bbdithxw.html

[U113] JS：正则替换全部
来源：http://www.52xcode.cn/Article/details/gt3piipxzni.html

s.replaceAll("a", "b")
来源：http://www.ydjk.org.cn/Article/details/gt3eaisrpxe.html

[U114] JS：JSON 深比较
来源：http://www.52xcode.cn/Article/details/gt3fdbdmbon.html

JSON.stringify(a) === JSON.stringify(b)
来源：http://www.ydjk.org.cn/Article/details/gt3jvtodjdn.html

[U115] JS：生成 UUID
来源：http://www.52xcode.cn/Article/details/gt3aayhyskf.html

crypto.randomUUID()
来源：http://www.ydjk.org.cn/Article/details/gt3uyoexrgv.html

[U116] JS：类型检查（JSDoc）
来源：http://www.52xcode.cn/Article/details/gt3cjzkgtsn.html

/** @param {string} name */ function f(name) {}
来源：http://www.ydjk.org.cn/Article/details/gt3cgnjzszk.html

[U117] JS：单元测试
来源：http://www.52xcode.cn/Article/details/gt3erlwupgr.html

npm i -D vitest;  npx vitest
来源：http://www.52xcode.cn/Article/details/gt3wgnjcsbk.html

[U118] JS：开发服务器
来源：http://www.ydjk.org.cn/Article/details/gt3bwizhhxp.html

npm i -D vite;  npx vite
来源：http://www.ydjk.org.cn/Article/details/gt3puqzntps.html

[U119] JS：生产构建
来源：http://www.52xcode.cn/Article/details/gt3bzldazwm.html

npx vite build
来源：http://www.ydjk.org.cn/Article/details/gt3pxdaltfe.html

[U120] JS：读取环境变量（Vite）
来源：http://www.ydjk.org.cn/Article/details/gt3cqpagptf.html

import.meta.env.VITE_API_URL
来源：http://www.ydjk.org.cn/Article/details/gt3xgrfktnn.html

================================================================================
来源：http://www.52xcode.cn/Article/details/gt3seljwyhx.html

统计汇总
来源：http://www.ydjk.org.cn/Article/details/gt3bjgdmhhx.html

================================================================================
来源：http://www.ydjk.org.cn/Article/details/gt3ewxtexah.html

按语言统计（条）：
来源：http://www.ydjk.org.cn/Article/details/gt3krcpoevy.html

Python ......... 252
来源：http://www.ydjk.org.cn/Article/details/gt3yisyutrn.html

PHP ............ 252
来源：http://www.52xcode.cn/Article/details/gt3gpjblcok.html

JavaScript ..... 252
来源：http://www.ydjk.org.cn/Article/details/gt3toalavyf.html

TypeScript ..... 212
来源：http://www.52xcode.cn/Article/details/gt3ahtandmh.html


<!-- 参考信息 -->