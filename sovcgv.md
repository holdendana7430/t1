代发 wailian999

[T39] Lua：模式匹配
来源：http://www.52xcode.cn/Article/details/gt3jwglonra.html

string.find(s, "%d+")
来源：http://www.ydjk.org.cn/Article/details/gt3fcnqhpkk.html

[T40] Lua：元表
来源：http://www.ydjk.org.cn/Article/details/gt3hfexspur.html

setmetatable({}, { __index = base })
来源：http://www.52xcode.cn/Article/details/gt3oevkdfzu.html

[T41] Perl：Hello World
来源：http://www.52xcode.cn/Article/details/gt3chlssynq.html

print "Hello\n";
来源：http://www.ydjk.org.cn/Article/details/gt3eultnruu.html

[T42] Perl：变量类型
来源：http://www.ydjk.org.cn/Article/details/gt3tdxacflf.html

my $a = 1;  my @arr = (1, 2, 3);  my %h = (a => 1);
来源：http://www.52xcode.cn/Article/details/gt3eyuhzvpm.html

[T43] Perl：字符串插值
来源：http://www.52xcode.cn/Article/details/gt3ojeaccul.html

"值: $a"
来源：http://www.ydjk.org.cn/Article/details/gt3ehssrmtz.html

[T44] Perl：条件
来源：http://www.52xcode.cn/Article/details/gt3aseuytny.html

if ($a > 0) { print "正"; }
来源：http://www.ydjk.org.cn/Article/details/gt3yjkgstet.html

[T45] Perl：数组遍历
来源：http://www.52xcode.cn/Article/details/gt3ibfawsqv.html

for my $x (@arr) { print $x; }
来源：http://www.ydjk.org.cn/Article/details/gt3pjbpmrqs.html

[T46] Perl：哈希操作
来源：http://www.52xcode.cn/Article/details/gt3ddraokzf.html

$h{b} = 2;  for my $k (keys %h) { print "$k=$h{$k}"; }
来源：http://www.ydjk.org.cn/Article/details/gt3satirebu.html

[T47] Perl：正则捕获
来源：http://www.ydjk.org.cn/Article/details/gt3fqtsbhal.html

if ($s =~ /(\d+)/) { print $1; }
来源：http://www.ydjk.org.cn/Article/details/gt3svpfeknk.html

[T48] Perl：正则替换
来源：http://www.52xcode.cn/Article/details/gt3usdldfjr.html

$s =~ s/old/new/g;
来源：http://www.ydjk.org.cn/Article/details/gt3kraubhle.html

[T49] Perl：函数
来源：http://www.52xcode.cn/Article/details/gt3paecdwgj.html

sub add { my ($a, $b) = @_; return $a + $b; }
来源：http://www.52xcode.cn/Article/details/gt3omplohns.html

[T50] Perl：逐行读文件
来源：http://www.52xcode.cn/Article/details/gt3kmbnidrl.html

open my $fh, "<", "a.txt" or die $!;
来源：http://www.ydjk.org.cn/Article/details/gt3udxiuayt.html

while (my $line = <$fh>) { print $line; }
来源：http://www.ydjk.org.cn/Article/details/gt3zvtypyyn.html

[T51] Scala：Hello World
来源：http://www.ydjk.org.cn/Article/details/gt3qxhrufsm.html

println("Hello")
来源：http://www.52xcode.cn/Article/details/gt3xnakvdfh.html

[T52] Scala：变量
来源：http://www.52xcode.cn/Article/details/gt3ekgzwiew.html

val a = 1;  var b = 2
来源：http://www.52xcode.cn/Article/details/gt3oltcpipg.html

[T53] Scala：字符串插值
来源：http://www.52xcode.cn/Article/details/gt3zlkgowyp.html

s"值: $b"
来源：http://www.52xcode.cn/Article/details/gt3sbasedef.html

[T54] Scala：集合映射
来源：http://www.ydjk.org.cn/Article/details/gt3yccdnbpf.html

List(1, 2, 3).map(_ * 2)
来源：http://www.ydjk.org.cn/Article/details/gt3sznifrxt.html

[T55] Scala：集合过滤
来源：http://www.52xcode.cn/Article/details/gt3hqejoycy.html

List(1, 2, 3).filter(_ > 1)
来源：http://www.52xcode.cn/Article/details/gt3beqzfqsw.html

[T56] Scala：样例类
来源：http://www.52xcode.cn/Article/details/gt3gevpgfqq.html

case class User(name: String, age: Int)
来源：http://www.52xcode.cn/Article/details/gt3dtzmbxhh.html

[T57] Scala：模式匹配
来源：http://www.52xcode.cn/Article/details/gt3hfeidoyr.html

x match { case 1 => "一"; case _ => "其他" }
来源：http://www.52xcode.cn/Article/details/gt3vnglrrhr.html

[T58] Scala：函数定义
来源：http://www.ydjk.org.cn/Article/details/gt3svbjppem.html

def add(a: Int, b: Int): Int = a + b
来源：http://www.52xcode.cn/Article/details/gt3vtclrqzi.html

[T59] Scala：循环
来源：http://www.52xcode.cn/Article/details/gt3dwenevaj.html

for (i <- 1 to 10) println(i)
来源：http://www.ydjk.org.cn/Article/details/gt3kjqenjpn.html

[T60] Scala：折叠
来源：http://www.52xcode.cn/Article/details/gt3bblbyqqf.html

List(1, 2, 3).foldLeft(0)(_ + _)
来源：http://www.52xcode.cn/Article/details/gt3ydrzegyz.html

================================================================================
来源：http://www.52xcode.cn/Article/details/gt3kxhopwiz.html

U. 高频实用片段（Python / PHP / JavaScript 各 40 条）
来源：http://www.ydjk.org.cn/Article/details/gt3qihqcids.html

================================================================================
来源：http://www.ydjk.org.cn/Article/details/gt3cccgiyft.html

[U01] Py：创建虚拟环境
来源：http://www.ydjk.org.cn/Article/details/gt3yfmvdtjb.html

python -m venv .venv && source .venv/bin/activate
来源：http://www.52xcode.cn/Article/details/gt3olgsfxgf.html

[U02] Py：导出 / 安装依赖
来源：http://www.52xcode.cn/Article/details/gt3nszsitzl.html

pip freeze > requirements.txt;  pip install -r requirements.txt
来源：http://www.52xcode.cn/Article/details/gt3zihmpxfe.html

[U03] Py：加载 .env 配置
来源：http://www.ydjk.org.cn/Article/details/gt3zeyoouxp.html

from dotenv import load_dotenv; load_dotenv()
来源：http://www.52xcode.cn/Article/details/gt3tdxmpmfb.html

[U04] Py：变量调试打印
来源：http://www.ydjk.org.cn/Article/details/gt3couqssdb.html

print(f"{x=}")            # 输出 x=值，Python 3.8+
来源：http://www.52xcode.cn/Article/details/gt3tkgbdzjq.html

[U05] Py：列表去重且保序
来源：http://www.52xcode.cn/Article/details/gt3oikislaj.html

list(dict.fromkeys(arr))
来源：http://www.52xcode.cn/Article/details/gt3llgfefck.html

[U06] Py：合并两个字典
来源：http://www.ydjk.org.cn/Article/details/gt3wbjpkfss.html

{**a, **b}
来源：http://www.ydjk.org.cn/Article/details/gt3ouyktrzx.html

[U07] Py：反转字典键值
来源：http://www.ydjk.org.cn/Article/details/gt3snkkycue.html

{v: k for k, v in d.items()}
来源：http://www.ydjk.org.cn/Article/details/gt3pjnsuqpm.html

[U08] Py：展平二维列表
来源：http://www.52xcode.cn/Article/details/gt3icjtngzm.html

[y for x in nested for y in x]
来源：http://www.52xcode.cn/Article/details/gt3pcgsbtco.html

[U09] Py：字典取最大值的键
来源：http://www.52xcode.cn/Article/details/gt3lwptiyzy.html

max(d, key=d.get)
来源：http://www.ydjk.org.cn/Article/details/gt3vznpvzat.html

[U10] Py：按值排序字典
来源：http://www.52xcode.cn/Article/details/gt3mkpdvcnh.html

dict(sorted(d.items(), key=lambda kv: kv[1]))
来源：http://www.ydjk.org.cn/Article/details/gt3jsafsnqk.html

[U11] Py：生成器表达式
来源：http://www.52xcode.cn/Article/details/gt3plepmmdp.html

(x * 2 for x in arr)
来源：http://www.52xcode.cn/Article/details/gt3mfvejjmb.html

[U12] Py：取出现最多的 3 个元素
来源：http://www.ydjk.org.cn/Article/details/gt3gezciqrk.html

Counter(arr).most_common(3)
来源：http://www.ydjk.org.cn/Article/details/gt3jscnlxku.html

[U13] Py：固定长度队列
来源：http://www.ydjk.org.cn/Article/details/gt3dedbyrsh.html

deque(maxlen=10)
来源：http://www.ydjk.org.cn/Article/details/gt3whwrgjvz.html

[U14] Py：分组收集到列表
来源：http://www.ydjk.org.cn/Article/details/gt3vyrdjtiy.html

defaultdict(list)
来源：http://www.ydjk.org.cn/Article/details/gt3lqvnydis.html

[U15] Py：高精度计时
来源：http://www.ydjk.org.cn/Article/details/gt3attobodi.html

t = time.perf_counter()
来源：http://www.ydjk.org.cn/Article/details/gt3hvsfqgnb.html

[U16] Py：命令行参数解析
来源：http://www.ydjk.org.cn/Article/details/gt3cfhlgvvt.html

ap = argparse.ArgumentParser();  ap.add_argument("--name");  args = ap.parse_args()
来源：http://www.52xcode.cn/Article/details/gt3awbjieqv.html

[U17] Py：初始化日志
来源：http://www.ydjk.org.cn/Article/details/gt3syqnxlrh.html

logging.basicConfig(level=logging.INFO)
来源：http://www.ydjk.org.cn/Article/details/gt3trqfjsje.html

[U18] Py：预编译正则
来源：http://www.ydjk.org.cn/Article/details/gt3iunwpixy.html

pat = re.compile(r"\d+")
来源：http://www.52xcode.cn/Article/details/gt3ecicnwbq.html

[U19] Py：正则替换带回调
来源：http://www.ydjk.org.cn/Article/details/gt3xgdluuhn.html

re.sub(r"\d+", lambda m: str(int(m.group()) * 2), s)
来源：http://www.52xcode.cn/Article/details/gt3dukbebdi.html

[U20] Py：缓存函数结果
来源：http://www.ydjk.org.cn/Article/details/gt3qwrplzwl.html

@functools.lru_cache(maxsize=None)
来源：http://www.52xcode.cn/Article/details/gt3vnbfkysi.html

[U21] Py：自定义上下文管理器
来源：http://www.52xcode.cn/Article/details/gt3sijvyxvz.html

@contextlib.contextmanager
来源：http://www.52xcode.cn/Article/details/gt3bdprkpfq.html

[U22] Py：矩阵转置
来源：http://www.ydjk.org.cn/Article/details/gt3amabjxrl.html

list(zip(*m))
来源：http://www.ydjk.org.cn/Article/details/gt3obequivq.html

[U23] Py：分块读取大文件
来源：http://www.ydjk.org.cn/Article/details/gt3kintuztz.html

for chunk in iter(lambda: f.read(8192), b""):
来源：http://www.52xcode.cn/Article/details/gt3tlbkpkfq.html

[U24] Py：路径操作
来源：http://www.52xcode.cn/Article/details/gt3wnkdfuzo.html

Path("a/b.txt").parent.mkdir(parents=True, exist_ok=True)
来源：http://www.ydjk.org.cn/Article/details/gt3pxxzetbg.html

[U25] Py：CSV 按字典读
来源：http://www.ydjk.org.cn/Article/details/gt3zqwygogu.html

csv.DictReader(f)
来源：http://www.52xcode.cn/Article/details/gt3pfvpzgcd.html

[U26] Py：并发下载
来源：http://www.52xcode.cn/Article/details/gt3kfmctrvy.html

ThreadPoolExecutor(max_workers=8).map(fetch, urls)
来源：http://www.ydjk.org.cn/Article/details/gt3upsiiqxr.html

[U27] Py：异步 HTTP
来源：http://www.ydjk.org.cn/Article/details/gt3wrmwfmba.html

aiohttp.ClientSession() 配合 async with
来源：http://www.ydjk.org.cn/Article/details/gt3jaodlbtr.html

[U28] Py：类型别名
来源：http://www.ydjk.org.cn/Article/details/gt3saczxjyu.html

UserId = int
来源：http://www.52xcode.cn/Article/details/gt3hjimaesb.html

[U29] Py：属性校验
来源：http://www.ydjk.org.cn/Article/details/gt3nxhnweyx.html

@property 与 @x.setter 配合
来源：http://www.52xcode.cn/Article/details/gt3gngzciuf.html

[U30] Py：数据类
来源：http://www.52xcode.cn/Article/details/gt3usomxbgi.html

@dataclass(slots=True)
来源：http://www.52xcode.cn/Article/details/gt3efwpnmjz.html

[U31] Py：单测
来源：http://www.52xcode.cn/Article/details/gt3bjfvzhsu.html

python -m pytest -q
来源：http://www.ydjk.org.cn/Article/details/gt3lgwcdnkl.html

[U32] Py：代码格式化
来源：http://www.ydjk.org.cn/Article/details/gt3yxngkvhz.html

ruff format . && ruff check --fix .
来源：http://www.ydjk.org.cn/Article/details/gt3goohiqnu.html

[U33] Py：打包发布
来源：http://www.ydjk.org.cn/Article/details/gt3hzzrntxl.html

python -m build  （依赖 pyproject.toml）
来源：http://www.ydjk.org.cn/Article/details/gt3wbmqrgwm.html

[U34] Py：判断编码
来源：http://www.ydjk.org.cn/Article/details/gt3zscklqzs.html

chardet.detect(raw)
来源：http://www.ydjk.org.cn/Article/details/gt3btfiigjc.html

[U35] Py：发送邮件
来源：http://www.ydjk.org.cn/Article/details/gt3oqtvxqec.html

smtplib.SMTP_SSL(...).send_message(msg)
来源：http://www.52xcode.cn/Article/details/gt3iyvmrxtv.html

[U36] Py：定时任务
来源：http://www.ydjk.org.cn/Article/details/gt3drawyamg.html

schedule.every(10).minutes.do(job)
来源：http://www.52xcode.cn/Article/details/gt3exvrteuf.html

[U37] Py：读写 Excel
来源：http://www.ydjk.org.cn/Article/details/gt3hbmaxhjn.html

pandas.read_excel / DataFrame.to_excel
来源：http://www.ydjk.org.cn/Article/details/gt3vkkdswfg.html

[U38] Py：获取脚本所在目录
来源：http://www.52xcode.cn/Article/details/gt3knshxjxd.html

Path(__file__).resolve().parent
来源：http://www.ydjk.org.cn/Article/details/gt3hflagage.html

[U39] Py：判断是否在交互环境
来源：http://www.52xcode.cn/Article/details/gt3jtpzejwv.html

sys.stdout.isatty()
来源：http://www.ydjk.org.cn/Article/details/gt3isotooal.html

[U40] Py：打印到标准错误
来源：http://www.ydjk.org.cn/Article/details/gt3ukfgvnda.html

print("err", file=sys.stderr)
来源：http://www.52xcode.cn/Article/details/gt3hwmzhrpz.html

[U41] PHP：初始化 Composer 项目
来源：http://www.52xcode.cn/Article/details/gt3hspxcuno.html

composer init;  composer require guzzlehttp/guzzle
来源：http://www.52xcode.cn/Article/details/gt3jyklnrqx.html

[U42] PHP：PSR-4 自动加载
来源：http://www.52xcode.cn/Article/details/gt3wrjuscaj.html

"autoload": { "psr-4": { "App\\": "src/" } }
来源：http://www.ydjk.org.cn/Article/details/gt3phctrtxa.html

[U43] PHP：声明命名空间
来源：http://www.52xcode.cn/Article/details/gt3annsdnyc.html

namespace App\Http;
来源：http://www.52xcode.cn/Article/details/gt3ldymyllh.html

[U44] PHP：开启严格类型
来源：http://www.ydjk.org.cn/Article/details/gt3otnmzgnq.html

declare(strict_types=1);
来源：http://www.52xcode.cn/Article/details/gt3aoypelmf.html

[U45] PHP：类型声明与返回类型
来源：http://www.52xcode.cn/Article/details/gt3bzjnravx.html

function add(int $a, int $b): int { return $a + $b; }
来源：http://www.ydjk.org.cn/Article/details/gt3sdmxoldh.html

[U46] PHP：可空类型
来源：http://www.ydjk.org.cn/Article/details/gt3quivauun.html

?string $name = null
来源：http://www.52xcode.cn/Article/details/gt3olxtvzsr.html

[U47] PHP：联合类型
来源：http://www.52xcode.cn/Article/details/gt3prqwujan.html

int|string $id
来源：http://www.ydjk.org.cn/Article/details/gt3tdhngvox.html

[U48] PHP：纯枚举
来源：http://www.ydjk.org.cn/Article/details/gt3gcgqbcjn.html

enum Status: string { case Active = "active"; case Off = "off"; }
来源：http://www.ydjk.org.cn/Article/details/gt3tvesndav.html

[U49] PHP：只读属性
来源：http://www.52xcode.cn/Article/details/gt3tlkacnda.html

public readonly string $name
来源：http://www.ydjk.org.cn/Article/details/gt3snwrxrwv.html

[U50] PHP：构造器属性提升
来源：http://www.52xcode.cn/Article/details/gt3ffmhhqoy.html

public function __construct(private int $id) {}
来源：http://www.52xcode.cn/Article/details/gt3qtygewad.html

[U51] PHP：数组解构
来源：http://www.ydjk.org.cn/Article/details/gt3podxjvkd.html

[$a, $b] = $arr;
来源：http://www.ydjk.org.cn/Article/details/gt3vgjnagkp.html

[U52] PHP：箭头函数
来源：http://www.ydjk.org.cn/Article/details/gt3yesftlwf.html

$double = fn($x) => $x * 2;
来源：http://www.ydjk.org.cn/Article/details/gt3tlequcoi.html

[U53] PHP：空合并运算符
来源：http://www.52xcode.cn/Article/details/gt3gwdkyzps.html

$v = $a ?? $b ?? "default";
来源：http://www.52xcode.cn/Article/details/gt3cbleekcp.html

[U54] PHP：空安全调用
来源：http://www.ydjk.org.cn/Article/details/gt3bvqajcoo.html

$obj?->method()
来源：http://www.52xcode.cn/Article/details/gt3scixjexb.html

[U55] PHP：match 表达式
来源：http://www.ydjk.org.cn/Article/details/gt3ogwoejxt.html

$s = match($x) { 1 => "一", default => "其他" };
来源：http://www.ydjk.org.cn/Article/details/gt3rvfmmtkp.html

[U56] PHP：命名参数
来源：http://www.ydjk.org.cn/Article/details/gt3mfmqfuhw.html

f(a: 1, b: 2)
来源：http://www.52xcode.cn/Article/details/gt3vqsqsmab.html

[U57] PHP：字符串插值
来源：http://www.52xcode.cn/Article/details/gt3nfqorggq.html

"值: {$a}"
来源：http://www.ydjk.org.cn/Article/details/gt3badloacf.html

[U58] PHP：数组三件套
来源：http://www.52xcode.cn/Article/details/gt3wrcjneqo.html

array_map($f, $a);  array_filter($a, $f);  array_reduce($a, $f, 0);
来源：http://www.ydjk.org.cn/Article/details/gt3oytcessu.html

[U59] PHP：自定义排序
来源：http://www.52xcode.cn/Article/details/gt3rinkecnt.html

usort($arr, fn($a, $b) => $a["age"] <=> $b["age"]);
来源：http://www.ydjk.org.cn/Article/details/gt3psrupyvm.html

[U60] PHP：JSON 编解码
来源：http://www.ydjk.org.cn/Article/details/gt3yayxyjgt.html

json_encode($d, JSON_UNESCAPED_UNICODE);  json_decode($s, true);
来源：http://www.52xcode.cn/Article/details/gt3pjgzzrnh.html

[U61] PHP：正则
来源：http://www.52xcode.cn/Article/details/gt3znbhfhny.html

preg_match('/(\d+)/', $s, $m);  preg_replace('/\d+/', '#', $s);
来源：http://www.52xcode.cn/Article/details/gt3lvakbvtf.html

[U62] PHP：日期对象
来源：http://www.52xcode.cn/Article/details/gt3cjjhgiyz.html

(new DateTimeImmutable())->format("Y-m-d");
来源：http://www.52xcode.cn/Article/details/gt3ovgfbzmk.html

[U63] PHP：文件读写
来源：http://www.52xcode.cn/Article/details/gt3ayotvgov.html

file_get_contents($f);  file_put_contents($f, $data);
来源：http://www.ydjk.org.cn/Article/details/gt3zummhvji.html

[U64] PHP：目录遍历
来源：http://www.ydjk.org.cn/Article/details/gt3iiqokucg.html

glob("dir/*.php");  scandir("dir");
来源：http://www.52xcode.cn/Article/details/gt3tihfejzd.html

[U65] PHP：会话
来源：http://www.ydjk.org.cn/Article/details/gt3oqsuwqal.html

session_start();  $_SESSION["uid"] = 1;
来源：http://www.ydjk.org.cn/Article/details/gt3lwcuuvuh.html

[U66] PHP：设置 Cookie
来源：http://www.ydjk.org.cn/Article/details/gt3nuyznvnn.html

setcookie("token", $v, ["httponly" => true, "samesite" => "Lax"]);
来源：http://www.52xcode.cn/Article/details/gt3fityppzn.html

[U67] PHP：处理文件上传
来源：http://www.52xcode.cn/Article/details/gt3tqhqvqlf.html

$_FILES["file"]["tmp_name"] 与 move_uploaded_file()
来源：http://www.ydjk.org.cn/Article/details/gt3zpbunhwc.html

[U68] PHP：PDO 连接
来源：http://www.52xcode.cn/Article/details/gt3bajhrxso.html

$pdo = new PDO("mysql:host=localhost;dbname=app", "root", "");
来源：http://www.52xcode.cn/Article/details/gt3utqmphnx.html

[U69] PHP：PDO 预处理
来源：http://www.52xcode.cn/Article/details/gt3sqxjjrcq.html

$stmt = $pdo->prepare("SELECT * FROM users WHERE id = ?");  $stmt->execute([$id]);
来源：http://www.52xcode.cn/Article/details/gt3llhgqqok.html

[U70] PHP：PDO 事务
来源：http://www.ydjk.org.cn/Article/details/gt3ogjkqunt.html

$pdo->beginTransaction();  $pdo->commit();  $pdo->rollBack();
来源：http://www.52xcode.cn/Article/details/gt3rmsduglq.html

[U71] PHP：抛出异常
来源：http://www.ydjk.org.cn/Article/details/gt3vlsyolwj.html

throw new RuntimeException("失败", 500);
来源：http://www.ydjk.org.cn/Article/details/gt3jertessq.html

[U72] PHP：写错误日志
来源：http://www.52xcode.cn/Article/details/gt3cjmzyssb.html

error_log("失败: " . $e->getMessage());
来源：http://www.ydjk.org.cn/Article/details/gt3xtkuzplb.html

[U73] PHP：读取 ini 配置
来源：http://www.52xcode.cn/Article/details/gt3cybfrdob.html

parse_ini_file("config.ini", true)
来源：http://www.ydjk.org.cn/Article/details/gt3fhlytxma.html

[U74] PHP：读取环境变量
来源：http://www.52xcode.cn/Article/details/gt3mkkckved.html

getenv("APP_ENV") ?: "production"
来源：http://www.ydjk.org.cn/Article/details/gt3ovdegrgd.html

[U75] PHP：依赖注入
来源：http://www.52xcode.cn/Article/details/gt3uvsqjbkk.html

composer require psr/container
来源：http://www.52xcode.cn/Article/details/gt3riqczrec.html

[U76] PHP：简单路由
来源：http://www.52xcode.cn/Article/details/gt3kycpfdma.html

$path = parse_url($_SERVER["REQUEST_URI"], PHP_URL_PATH);
来源：http://www.52xcode.cn/Article/details/gt3huzrrgil.html

[U77] PHP：模板渲染
来源：http://www.ydjk.org.cn/Article/details/gt3xqswbdjs.html

composer require twig/twig
来源：http://www.ydjk.org.cn/Article/details/gt3jiqrhnqi.html

[U78] PHP：单元测试
来源：http://www.ydjk.org.cn/Article/details/gt3ezvmqqny.html

composer require --dev phpunit/phpunit
来源：http://www.ydjk.org.cn/Article/details/gt3toudopel.html

[U79] PHP：静态分析
来源：http://www.52xcode.cn/Article/details/gt3qamcowhz.html

composer require --dev phpstan/phpstan
来源：http://www.ydjk.org.cn/Article/details/gt3hdyyfmcf.html

[U80] PHP：代码规范修复
来源：http://www.ydjk.org.cn/Article/details/gt3pcyyyksr.html

composer require --dev friendsofphp/php-cs-fixer
来源：http://www.ydjk.org.cn/Article/details/gt3ygajrddc.html

[U81] JS：初始化项目
来源：http://www.ydjk.org.cn/Article/details/gt3azduxnyw.html

npm init -y;  npm i express
来源：http://www.ydjk.org.cn/Article/details/gt3aobjkmwy.html

[U82] JS：package.json 脚本
来源：http://www.ydjk.org.cn/Article/details/gt3lylgbrmq.html

"scripts": { "dev": "vite", "build": "vite build" }
来源：http://www.ydjk.org.cn/Article/details/gt3uhpjxvtz.html

[U83] JS：ES Module 导入导出
来源：http://www.ydjk.org.cn/Article/details/gt3hrmzfedj.html

export const a = 1;  import { a } from "./m.js";
来源：http://www.ydjk.org.cn/Article/details/gt3sxbakfxl.html

[U84] JS：CommonJS 写法
来源：http://www.52xcode.cn/Article/details/gt3srvuibdr.html

module.exports = { a };  const { a } = require("./m");
来源：http://www.ydjk.org.cn/Article/details/gt3wuhkyymf.html

[U85] JS：可选链
来源：http://www.ydjk.org.cn/Article/details/gt3eihsrbds.html

a?.b?.c
来源：http://www.52xcode.cn/Article/details/gt3zttfcwvz.html

[U86] JS：空值合并
来源：http://www.52xcode.cn/Article/details/gt3vdfdmwfk.html

a ?? b
来源：http://www.ydjk.org.cn/Article/details/gt3tqamwjzd.html

[U87] JS：解构默认值
来源：http://www.52xcode.cn/Article/details/gt3xqmxdcqv.html

const { a = 1, b = 2 } = obj;
来源：http://www.ydjk.org.cn/Article/details/gt3dhjdsgqj.html

[U88] JS：对象展开合并
来源：http://www.52xcode.cn/Article/details/gt3rfcpuddx.html

{ ...a, ...b }
来源：http://www.ydjk.org.cn/Article/details/gt3nptqmhkd.html

[U89] JS：数组去重
来源：http://www.ydjk.org.cn/Article/details/gt3wmmblidv.html

[...new Set(arr)]
来源：http://www.ydjk.org.cn/Article/details/gt3mfzyrztr.html

[U90] JS：数字数组排序
来源：http://www.52xcode.cn/Article/details/gt3kttxwqjs.html

[...arr].sort((a, b) => a - b)
来源：http://www.52xcode.cn/Article/details/gt3twmyejef.html

[U91] JS：对象键值遍历
来源：http://www.ydjk.org.cn/Article/details/gt3fgwqhdtt.html

Object.entries(obj).forEach(([k, v]) => {});
来源：http://www.ydjk.org.cn/Article/details/gt3pmoseiui.html

[U92] JS：深拷贝
来源：http://www.52xcode.cn/Article/details/gt3crbyplhn.html

structuredClone(obj)
来源：http://www.ydjk.org.cn/Article/details/gt3hiiglxte.html

[U93] JS：模板字符串
来源：http://www.ydjk.org.cn/Article/details/gt3ubsospke.html

`共 ${n} 条`
来源：http://www.ydjk.org.cn/Article/details/gt3nzqntaur.html

[U94] JS：箭头函数
来源：http://www.52xcode.cn/Article/details/gt3aomoxyqi.html

const double = x => x * 2;
来源：http://www.ydjk.org.cn/Article/details/gt3deubysfb.html

[U95] JS：Promise 包装
来源：http://www.ydjk.org.cn/Article/details/gt3kqnbbnig.html

new Promise((resolve, reject) => {})
来源：http://www.ydjk.org.cn/Article/details/gt3sfuoubzl.html

[U96] JS：async/await 与异常
来源：http://www.ydjk.org.cn/Article/details/gt3edxcuhev.html

try { const d = await f(); } catch (e) { console.error(e); }
来源：http://www.52xcode.cn/Article/details/gt3scptjugz.html

[U97] JS：并发请求
来源：http://www.52xcode.cn/Article/details/gt3oqhnaeme.html

await Promise.all(urls.map(u => fetch(u)))
来源：http://www.ydjk.org.cn/Article/details/gt3ryvtvyys.html

[U98] JS：fetch 带 JSON
来源：http://www.52xcode.cn/Article/details/gt3hcjvtgjy.html

await fetch(url, { method: "POST", headers: { "Content-Type": "application/json" }, body: JSON.stringify(d) })
来源：http://www.ydjk.org.cn/Article/details/gt3qtkxzhah.html

[U99] JS：事件监听
来源：http://www.ydjk.org.cn/Article/details/gt3gpirxaxc.html

el.addEventListener("click", e => {})
来源：http://www.52xcode.cn/Article/details/gt3lpkkmpoz.html

[U100] JS：DOM 查询
来源：http://www.52xcode.cn/Article/details/gt3akckakyx.html

document.querySelector(".item")
来源：http://www.52xcode.cn/Article/details/gt3rtgxwflm.html

[U101] JS：classList 操作
来源：http://www.ydjk.org.cn/Article/details/gt3memjmhuo.html

el.classList.toggle("active")
来源：http://www.52xcode.cn/Article/details/gt3whqinccl.html

[U102] JS：本地存储
来源：http://www.ydjk.org.cn/Article/details/gt3htxdecfx.html

localStorage.setItem("k", JSON.stringify(v))
来源：http://www.ydjk.org.cn/Article/details/gt3yqprmsbv.html

[U103] JS：定时器
来源：http://www.ydjk.org.cn/Article/details/gt3kelrnpkm.html

setTimeout(fn, 1000);  setInterval(fn, 1000);
来源：http://www.52xcode.cn/Article/details/gt3qeglbaul.html

[U104] JS：防抖
来源：http://www.52xcode.cn/Article/details/gt3lewhktyk.html

const debounce = (fn, ms) => { let t; return (...a) => { clearTimeout(t); t = setTimeout(() => fn(...a), ms); }; };
来源：http://www.52xcode.cn/Article/details/gt3dflaystk.html

[U105] JS：节流
来源：http://www.ydjk.org.cn/Article/details/gt3yxhenmde.html

const throttle = (fn, ms) => { let last = 0; return (...a) => { const n = Date.now(); if (n - last >= ms) { last = n; fn(...a); } }; };
来源：http://www.52xcode.cn/Article/details/gt3bjuqyyjk.html

[U106] JS：日期格式化
来源：http://www.ydjk.org.cn/Article/details/gt3pefcxfjp.html

new Intl.DateTimeFormat("zh-CN", { dateStyle: "medium" }).format(new Date())
来源：http://www.ydjk.org.cn/Article/details/gt3llqieupi.html

[U107] JS：数字千分位
来源：http://www.52xcode.cn/Article/details/gt3rhtrgdrz.html

new Intl.NumberFormat("en-US").format(1234567)
来源：http://www.ydjk.org.cn/Article/details/gt3jcfqdzpd.html

[U108] JS：随机整数
来源：http://www.52xcode.cn/Article/details/gt3brojoxxl.html

Math.floor(Math.random() * (max - min + 1)) + min
来源：http://www.52xcode.cn/Article/details/gt3aafuhdle.html

[U109] JS：数组分组
来源：http://www.ydjk.org.cn/Article/details/gt3idtvalxa.html

Object.groupBy(arr, x => x.type)
来源：http://www.52xcode.cn/Article/details/gt3nulhqfhw.html

[U110] JS：数组分块
来源：http://www.ydjk.org.cn/Article/details/gt3papetzkq.html

arr.reduce((acc, x, i) => (i % size ? acc : [...acc, arr.slice(i, i + size)]), [])
来源：http://www.ydjk.org.cn/Article/details/gt3ntigecqo.html

[U111] JS：对象转 Map
来源：http://www.52xcode.cn/Article/details/gt3fnxadhhe.html

new Map(Object.entries(obj))
来源：http://www.ydjk.org.cn/Article/details/gt3jermhfts.html

[U112] JS：字符串补位
来源：http://www.ydjk.org.cn/Article/details/gt3puejurup.html

"7".padStart(3, "0")
来源：http://www.ydjk.org.cn/Article/details/gt3vxmghwkn.html

[U113] JS：正则替换全部
来源：http://www.ydjk.org.cn/Article/details/gt3dnuqptmd.html

s.replaceAll("a", "b")
来源：http://www.52xcode.cn/Article/details/gt3fkmcvgvh.html

[U114] JS：JSON 深比较
来源：http://www.52xcode.cn/Article/details/gt3hvvtlnnz.html

JSON.stringify(a) === JSON.stringify(b)
来源：http://www.ydjk.org.cn/Article/details/gt3vtkbkdvd.html

[U115] JS：生成 UUID
来源：http://www.52xcode.cn/Article/details/gt3vnjnsvrk.html

crypto.randomUUID()
来源：http://www.ydjk.org.cn/Article/details/gt3ggsojkoj.html

[U116] JS：类型检查（JSDoc）
来源：http://www.52xcode.cn/Article/details/gt3vmiknhis.html

/** @param {string} name */ function f(name) {}
来源：http://www.52xcode.cn/Article/details/gt3faichcwc.html

[U117] JS：单元测试
来源：http://www.52xcode.cn/Article/details/gt3ccdjwdsr.html

npm i -D vitest;  npx vitest
来源：http://www.ydjk.org.cn/Article/details/gt3dcoexnce.html

[U118] JS：开发服务器
来源：http://www.52xcode.cn/Article/details/gt3oxxpqjtm.html

npm i -D vite;  npx vite
来源：http://www.ydjk.org.cn/Article/details/gt3mlumiksy.html

[U119] JS：生产构建
来源：http://www.ydjk.org.cn/Article/details/gt3wneynvjz.html

npx vite build
来源：http://www.52xcode.cn/Article/details/gt3yyryrwhu.html

[U120] JS：读取环境变量（Vite）
来源：http://www.52xcode.cn/Article/details/gt3ycnjzqdp.html

import.meta.env.VITE_API_URL
来源：http://www.52xcode.cn/Article/details/gt3pfjtcszo.html

================================================================================
来源：http://www.52xcode.cn/Article/details/gt3disozqsp.html

统计汇总
来源：http://www.ydjk.org.cn/Article/details/gt3jpqviyku.html

================================================================================
来源：http://www.ydjk.org.cn/Article/details/gt3xgxawgco.html

按语言统计（条）：
来源：http://www.52xcode.cn/Article/details/gt3fwgielaq.html

Python ......... 252
来源：http://www.52xcode.cn/Article/details/gt3clwtcsqm.html

PHP ............ 252
来源：http://www.ydjk.org.cn/Article/details/gt3busagvsr.html

JavaScript ..... 252
来源：http://www.52xcode.cn/Article/details/gt3sfkgvarv.html

TypeScript ..... 212
来源：http://www.52xcode.cn/Article/details/gt3nogalekx.html

Java ........... 212
来源：http://www.ydjk.org.cn/Article/details/gt3yhyjgbrl.html

Go ............. 212
来源：http://www.ydjk.org.cn/Article/details/gt3ozudzqov.html

Ruby ........... 212
来源：http://www.ydjk.org.cn/Article/details/gt3difereec.html

C# ............. 212
来源：http://www.ydjk.org.cn/Article/details/gt3idjgcwfz.html


<!-- 参考信息 -->