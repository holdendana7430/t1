代发 wailian999

[T41] Perl：Hello World
来源：http://www.ydjk.org.cn/Article/details/gt3bwajgnqg.html

print "Hello\n";
来源：http://www.52xcode.cn/Article/details/gt3serkvzhn.html

[T42] Perl：变量类型
来源：http://www.52xcode.cn/Article/details/gt3mpvywtwm.html

my $a = 1;  my @arr = (1, 2, 3);  my %h = (a => 1);
来源：http://www.ydjk.org.cn/Article/details/gt3locdrllo.html

[T43] Perl：字符串插值
来源：http://www.52xcode.cn/Article/details/gt3ndhwdonv.html

"值: $a"
来源：http://www.52xcode.cn/Article/details/gt3irtssblh.html

[T44] Perl：条件
来源：http://www.ydjk.org.cn/Article/details/gt3bymldrqb.html

if ($a > 0) { print "正"; }
来源：http://www.ydjk.org.cn/Article/details/gt3dmhexuzm.html

[T45] Perl：数组遍历
来源：http://www.ydjk.org.cn/Article/details/gt3abxfgiqg.html

for my $x (@arr) { print $x; }
来源：http://www.ydjk.org.cn/Article/details/gt3xvpzzrqe.html

[T46] Perl：哈希操作
来源：http://www.52xcode.cn/Article/details/gt3hmqbbohb.html

$h{b} = 2;  for my $k (keys %h) { print "$k=$h{$k}"; }
来源：http://www.52xcode.cn/Article/details/gt3mfzqyaty.html

[T47] Perl：正则捕获
来源：http://www.52xcode.cn/Article/details/gt3tcekssym.html

if ($s =~ /(\d+)/) { print $1; }
来源：http://www.52xcode.cn/Article/details/gt3niuwayos.html

[T48] Perl：正则替换
来源：http://www.ydjk.org.cn/Article/details/gt3rsxgzyhq.html

$s =~ s/old/new/g;
来源：http://www.52xcode.cn/Article/details/gt3yratcnfv.html

[T49] Perl：函数
来源：http://www.52xcode.cn/Article/details/gt3pyfawsdw.html

sub add { my ($a, $b) = @_; return $a + $b; }
来源：http://www.ydjk.org.cn/Article/details/gt3sdkblmyr.html

[T50] Perl：逐行读文件
来源：http://www.ydjk.org.cn/Article/details/gt3nlnmgruj.html

open my $fh, "<", "a.txt" or die $!;
来源：http://www.ydjk.org.cn/Article/details/gt3awtzazrh.html

while (my $line = <$fh>) { print $line; }
来源：http://www.ydjk.org.cn/Article/details/gt3smdadnil.html

[T51] Scala：Hello World
来源：http://www.52xcode.cn/Article/details/gt3gkrxituq.html

println("Hello")
来源：http://www.ydjk.org.cn/Article/details/gt3kcnunlzz.html

[T52] Scala：变量
来源：http://www.52xcode.cn/Article/details/gt3vqsygzxl.html

val a = 1;  var b = 2
来源：http://www.52xcode.cn/Article/details/gt3fnfnhuvj.html

[T53] Scala：字符串插值
来源：http://www.52xcode.cn/Article/details/gt3amaooyym.html

s"值: $b"
来源：http://www.52xcode.cn/Article/details/gt3shwtfktv.html

[T54] Scala：集合映射
来源：http://www.ydjk.org.cn/Article/details/gt3kewciwtr.html

List(1, 2, 3).map(_ * 2)
来源：http://www.ydjk.org.cn/Article/details/gt3qmbxpeqs.html

[T55] Scala：集合过滤
来源：http://www.52xcode.cn/Article/details/gt3fiwtvgbm.html

List(1, 2, 3).filter(_ > 1)
来源：http://www.52xcode.cn/Article/details/gt3venmokkq.html

[T56] Scala：样例类
来源：http://www.ydjk.org.cn/Article/details/gt3brrhtetv.html

case class User(name: String, age: Int)
来源：http://www.ydjk.org.cn/Article/details/gt3mhmlbuuk.html

[T57] Scala：模式匹配
来源：http://www.ydjk.org.cn/Article/details/gt3kdknnhfx.html

x match { case 1 => "一"; case _ => "其他" }
来源：http://www.ydjk.org.cn/Article/details/gt3koupomja.html

[T58] Scala：函数定义
来源：http://www.ydjk.org.cn/Article/details/gt3izhbsmph.html

def add(a: Int, b: Int): Int = a + b
来源：http://www.ydjk.org.cn/Article/details/gt3dpxyoqlo.html

[T59] Scala：循环
来源：http://www.ydjk.org.cn/Article/details/gt3ivnxzzvf.html

for (i <- 1 to 10) println(i)
来源：http://www.ydjk.org.cn/Article/details/gt3fzqzlpke.html

[T60] Scala：折叠
来源：http://www.52xcode.cn/Article/details/gt3vjlprntj.html

List(1, 2, 3).foldLeft(0)(_ + _)
来源：http://www.52xcode.cn/Article/details/gt3olsninyk.html

================================================================================
来源：http://www.52xcode.cn/Article/details/gt3trffxgcy.html

U. 高频实用片段（Python / PHP / JavaScript 各 40 条）
来源：http://www.52xcode.cn/Article/details/gt3zqlfbmvp.html

================================================================================
来源：http://www.ydjk.org.cn/Article/details/gt3lxzcwfsr.html

[U01] Py：创建虚拟环境
来源：http://www.52xcode.cn/Article/details/gt3apqwajud.html

python -m venv .venv && source .venv/bin/activate
来源：http://www.52xcode.cn/Article/details/gt3iltgrtfg.html

[U02] Py：导出 / 安装依赖
来源：http://www.ydjk.org.cn/Article/details/gt3mscdkxbo.html

pip freeze > requirements.txt;  pip install -r requirements.txt
来源：http://www.52xcode.cn/Article/details/gt3zakmbbpa.html

[U03] Py：加载 .env 配置
来源：http://www.ydjk.org.cn/Article/details/gt3jhgvkdwi.html

from dotenv import load_dotenv; load_dotenv()
来源：http://www.52xcode.cn/Article/details/gt3befegwic.html

[U04] Py：变量调试打印
来源：http://www.ydjk.org.cn/Article/details/gt3jizzqdwl.html

print(f"{x=}")            # 输出 x=值，Python 3.8+
来源：http://www.ydjk.org.cn/Article/details/gt3lencltud.html

[U05] Py：列表去重且保序
来源：http://www.52xcode.cn/Article/details/gt3ibqxkykc.html

list(dict.fromkeys(arr))
来源：http://www.52xcode.cn/Article/details/gt3utiiqval.html

[U06] Py：合并两个字典
来源：http://www.52xcode.cn/Article/details/gt3tdnlfxhg.html

{**a, **b}
来源：http://www.52xcode.cn/Article/details/gt3nahrhsaz.html

[U07] Py：反转字典键值
来源：http://www.ydjk.org.cn/Article/details/gt3mkubnpiy.html

{v: k for k, v in d.items()}
来源：http://www.52xcode.cn/Article/details/gt3wtnvizlp.html

[U08] Py：展平二维列表
来源：http://www.52xcode.cn/Article/details/gt3wxbqybky.html

[y for x in nested for y in x]
来源：http://www.ydjk.org.cn/Article/details/gt3jlqzpyaq.html

[U09] Py：字典取最大值的键
来源：http://www.52xcode.cn/Article/details/gt3yysvfjgl.html

max(d, key=d.get)
来源：http://www.ydjk.org.cn/Article/details/gt3qzvkvkys.html

[U10] Py：按值排序字典
来源：http://www.52xcode.cn/Article/details/gt3lbajdmbt.html

dict(sorted(d.items(), key=lambda kv: kv[1]))
来源：http://www.52xcode.cn/Article/details/gt3jpmotusv.html

[U11] Py：生成器表达式
来源：http://www.52xcode.cn/Article/details/gt3lipkarpq.html

(x * 2 for x in arr)
来源：http://www.ydjk.org.cn/Article/details/gt3cewfbmgx.html

[U12] Py：取出现最多的 3 个元素
来源：http://www.52xcode.cn/Article/details/gt3gsdswtke.html

Counter(arr).most_common(3)
来源：http://www.ydjk.org.cn/Article/details/gt3soubgpqd.html

[U13] Py：固定长度队列
来源：http://www.ydjk.org.cn/Article/details/gt3nfzefmnm.html

deque(maxlen=10)
来源：http://www.ydjk.org.cn/Article/details/gt3omiumymh.html

[U14] Py：分组收集到列表
来源：http://www.ydjk.org.cn/Article/details/gt3mjhwguii.html

defaultdict(list)
来源：http://www.52xcode.cn/Article/details/gt3mtxncztx.html

[U15] Py：高精度计时
来源：http://www.ydjk.org.cn/Article/details/gt3uyltkybc.html

t = time.perf_counter()
来源：http://www.ydjk.org.cn/Article/details/gt3xizofdhc.html

[U16] Py：命令行参数解析
来源：http://www.52xcode.cn/Article/details/gt3gxeeurah.html

ap = argparse.ArgumentParser();  ap.add_argument("--name");  args = ap.parse_args()
来源：http://www.52xcode.cn/Article/details/gt3ihhqiusp.html

[U17] Py：初始化日志
来源：http://www.ydjk.org.cn/Article/details/gt3uaccuwkt.html

logging.basicConfig(level=logging.INFO)
来源：http://www.ydjk.org.cn/Article/details/gt3brtxopwu.html

[U18] Py：预编译正则
来源：http://www.52xcode.cn/Article/details/gt3pyaavqsg.html

pat = re.compile(r"\d+")
来源：http://www.52xcode.cn/Article/details/gt3pzjfxcdf.html

[U19] Py：正则替换带回调
来源：http://www.52xcode.cn/Article/details/gt3ojkkquan.html

re.sub(r"\d+", lambda m: str(int(m.group()) * 2), s)
来源：http://www.ydjk.org.cn/Article/details/gt3rcumqwoy.html

[U20] Py：缓存函数结果
来源：http://www.52xcode.cn/Article/details/gt3pgqwwfos.html

@functools.lru_cache(maxsize=None)
来源：http://www.52xcode.cn/Article/details/gt3fdgsrmhi.html

[U21] Py：自定义上下文管理器
来源：http://www.52xcode.cn/Article/details/gt3gzbutknr.html

@contextlib.contextmanager
来源：http://www.ydjk.org.cn/Article/details/gt3zjhbtixj.html

[U22] Py：矩阵转置
来源：http://www.ydjk.org.cn/Article/details/gt3xxmllcqu.html

list(zip(*m))
来源：http://www.ydjk.org.cn/Article/details/gt3dohlthxk.html

[U23] Py：分块读取大文件
来源：http://www.ydjk.org.cn/Article/details/gt3zwlagbdk.html

for chunk in iter(lambda: f.read(8192), b""):
来源：http://www.ydjk.org.cn/Article/details/gt3qvctpkwa.html

[U24] Py：路径操作
来源：http://www.ydjk.org.cn/Article/details/gt3fxytyxjy.html

Path("a/b.txt").parent.mkdir(parents=True, exist_ok=True)
来源：http://www.52xcode.cn/Article/details/gt3vdibszzr.html

[U25] Py：CSV 按字典读
来源：http://www.52xcode.cn/Article/details/gt3bniifbpr.html

csv.DictReader(f)
来源：http://www.ydjk.org.cn/Article/details/gt3izjmlazp.html

[U26] Py：并发下载
来源：http://www.52xcode.cn/Article/details/gt3hvsqbtis.html

ThreadPoolExecutor(max_workers=8).map(fetch, urls)
来源：http://www.ydjk.org.cn/Article/details/gt3bgtacssn.html

[U27] Py：异步 HTTP
来源：http://www.ydjk.org.cn/Article/details/gt3xnecafyf.html

aiohttp.ClientSession() 配合 async with
来源：http://www.ydjk.org.cn/Article/details/gt3dyzjutdf.html

[U28] Py：类型别名
来源：http://www.52xcode.cn/Article/details/gt3zogxxuya.html

UserId = int
来源：http://www.ydjk.org.cn/Article/details/gt3hxorduak.html

[U29] Py：属性校验
来源：http://www.ydjk.org.cn/Article/details/gt3oqzjjdqr.html

@property 与 @x.setter 配合
来源：http://www.ydjk.org.cn/Article/details/gt3keeokmpi.html

[U30] Py：数据类
来源：http://www.52xcode.cn/Article/details/gt3ivqixuzd.html

@dataclass(slots=True)
来源：http://www.52xcode.cn/Article/details/gt3nlmquwsw.html

[U31] Py：单测
来源：http://www.52xcode.cn/Article/details/gt3qdlvmywt.html

python -m pytest -q
来源：http://www.52xcode.cn/Article/details/gt3zgbnkpcp.html

[U32] Py：代码格式化
来源：http://www.ydjk.org.cn/Article/details/gt3rkeabbcf.html

ruff format . && ruff check --fix .
来源：http://www.ydjk.org.cn/Article/details/gt3ofmyqwcj.html

[U33] Py：打包发布
来源：http://www.ydjk.org.cn/Article/details/gt3jztpheeq.html

python -m build  （依赖 pyproject.toml）
来源：http://www.ydjk.org.cn/Article/details/gt3qafwqrly.html

[U34] Py：判断编码
来源：http://www.52xcode.cn/Article/details/gt3rpfauwhx.html

chardet.detect(raw)
来源：http://www.ydjk.org.cn/Article/details/gt3tsobzoio.html

[U35] Py：发送邮件
来源：http://www.ydjk.org.cn/Article/details/gt3ubwcxphs.html

smtplib.SMTP_SSL(...).send_message(msg)
来源：http://www.52xcode.cn/Article/details/gt3dpadaclx.html

[U36] Py：定时任务
来源：http://www.52xcode.cn/Article/details/gt3geetxbby.html

schedule.every(10).minutes.do(job)
来源：http://www.52xcode.cn/Article/details/gt3opewekds.html

[U37] Py：读写 Excel
来源：http://www.ydjk.org.cn/Article/details/gt3lposwiab.html

pandas.read_excel / DataFrame.to_excel
来源：http://www.ydjk.org.cn/Article/details/gt3utinemon.html

[U38] Py：获取脚本所在目录
来源：http://www.52xcode.cn/Article/details/gt3slbeblql.html

Path(__file__).resolve().parent
来源：http://www.ydjk.org.cn/Article/details/gt3ojeweqyk.html

[U39] Py：判断是否在交互环境
来源：http://www.ydjk.org.cn/Article/details/gt3mkkvqdns.html

sys.stdout.isatty()
来源：http://www.ydjk.org.cn/Article/details/gt3qbogcvfh.html

[U40] Py：打印到标准错误
来源：http://www.ydjk.org.cn/Article/details/gt3xrhpdkmp.html

print("err", file=sys.stderr)
来源：http://www.52xcode.cn/Article/details/gt3hyktcadb.html

[U41] PHP：初始化 Composer 项目
来源：http://www.52xcode.cn/Article/details/gt3yolwashy.html

composer init;  composer require guzzlehttp/guzzle
来源：http://www.52xcode.cn/Article/details/gt3rvdunjif.html

[U42] PHP：PSR-4 自动加载
来源：http://www.ydjk.org.cn/Article/details/gt3hmrchscs.html

"autoload": { "psr-4": { "App\\": "src/" } }
来源：http://www.52xcode.cn/Article/details/gt3yaqzrdbb.html

[U43] PHP：声明命名空间
来源：http://www.52xcode.cn/Article/details/gt3baybbuhm.html

namespace App\Http;
来源：http://www.52xcode.cn/Article/details/gt3bbpkfegs.html

[U44] PHP：开启严格类型
来源：http://www.ydjk.org.cn/Article/details/gt3qcdxrmhd.html

declare(strict_types=1);
来源：http://www.ydjk.org.cn/Article/details/gt3sshictrd.html

[U45] PHP：类型声明与返回类型
来源：http://www.ydjk.org.cn/Article/details/gt3bkmpaliq.html

function add(int $a, int $b): int { return $a + $b; }
来源：http://www.52xcode.cn/Article/details/gt3ddkexpln.html

[U46] PHP：可空类型
来源：http://www.ydjk.org.cn/Article/details/gt3eqdwmsuh.html

?string $name = null
来源：http://www.52xcode.cn/Article/details/gt3szkiffzm.html

[U47] PHP：联合类型
来源：http://www.ydjk.org.cn/Article/details/gt3zdskqabf.html

int|string $id
来源：http://www.ydjk.org.cn/Article/details/gt3ibcwifos.html

[U48] PHP：纯枚举
来源：http://www.ydjk.org.cn/Article/details/gt3kojuyjck.html

enum Status: string { case Active = "active"; case Off = "off"; }
来源：http://www.ydjk.org.cn/Article/details/gt3terlqusq.html

[U49] PHP：只读属性
来源：http://www.ydjk.org.cn/Article/details/gt3ujliiczj.html

public readonly string $name
来源：http://www.ydjk.org.cn/Article/details/gt3gqpfeanz.html

[U50] PHP：构造器属性提升
来源：http://www.ydjk.org.cn/Article/details/gt3fjjjozys.html

public function __construct(private int $id) {}
来源：http://www.ydjk.org.cn/Article/details/gt3eoqmcwny.html

[U51] PHP：数组解构
来源：http://www.52xcode.cn/Article/details/gt3kymphjkw.html

[$a, $b] = $arr;
来源：http://www.ydjk.org.cn/Article/details/gt3ouglqwby.html

[U52] PHP：箭头函数
来源：http://www.ydjk.org.cn/Article/details/gt3egtedrmu.html

$double = fn($x) => $x * 2;
来源：http://www.52xcode.cn/Article/details/gt3gvqfzffm.html

[U53] PHP：空合并运算符
来源：http://www.ydjk.org.cn/Article/details/gt3ikxznhzz.html

$v = $a ?? $b ?? "default";
来源：http://www.52xcode.cn/Article/details/gt3efevliud.html

[U54] PHP：空安全调用
来源：http://www.ydjk.org.cn/Article/details/gt3aoqvvefs.html

$obj?->method()
来源：http://www.ydjk.org.cn/Article/details/gt3sqomaziw.html

[U55] PHP：match 表达式
来源：http://www.52xcode.cn/Article/details/gt3ebxqwrws.html

$s = match($x) { 1 => "一", default => "其他" };
来源：http://www.ydjk.org.cn/Article/details/gt3jyqnkkaq.html

[U56] PHP：命名参数
来源：http://www.52xcode.cn/Article/details/gt3dbrbvbaw.html

f(a: 1, b: 2)
来源：http://www.52xcode.cn/Article/details/gt3osnlaxht.html

[U57] PHP：字符串插值
来源：http://www.52xcode.cn/Article/details/gt3hzejquvg.html

"值: {$a}"
来源：http://www.ydjk.org.cn/Article/details/gt3xxvzclhz.html

[U58] PHP：数组三件套
来源：http://www.52xcode.cn/Article/details/gt3tyqsyeej.html

array_map($f, $a);  array_filter($a, $f);  array_reduce($a, $f, 0);
来源：http://www.ydjk.org.cn/Article/details/gt3zmaghjls.html

[U59] PHP：自定义排序
来源：http://www.52xcode.cn/Article/details/gt3azcvabza.html

usort($arr, fn($a, $b) => $a["age"] <=> $b["age"]);
来源：http://www.ydjk.org.cn/Article/details/gt3otmkjbpk.html

[U60] PHP：JSON 编解码
来源：http://www.52xcode.cn/Article/details/gt3urwtrbun.html

json_encode($d, JSON_UNESCAPED_UNICODE);  json_decode($s, true);
来源：http://www.ydjk.org.cn/Article/details/gt3prjefmev.html

[U61] PHP：正则
来源：http://www.ydjk.org.cn/Article/details/gt3gtkyzswi.html

preg_match('/(\d+)/', $s, $m);  preg_replace('/\d+/', '#', $s);
来源：http://www.52xcode.cn/Article/details/gt3mbhcmfpp.html

[U62] PHP：日期对象
来源：http://www.52xcode.cn/Article/details/gt3muumdtno.html

(new DateTimeImmutable())->format("Y-m-d");
来源：http://www.52xcode.cn/Article/details/gt3grabijqc.html

[U63] PHP：文件读写
来源：http://www.ydjk.org.cn/Article/details/gt3egakkkeq.html

file_get_contents($f);  file_put_contents($f, $data);
来源：http://www.52xcode.cn/Article/details/gt3mjprqdxz.html

[U64] PHP：目录遍历
来源：http://www.52xcode.cn/Article/details/gt3jfhnxgtp.html

glob("dir/*.php");  scandir("dir");
来源：http://www.ydjk.org.cn/Article/details/gt3pnhygurr.html

[U65] PHP：会话
来源：http://www.ydjk.org.cn/Article/details/gt3ahyghxst.html

session_start();  $_SESSION["uid"] = 1;
来源：http://www.52xcode.cn/Article/details/gt3difdgrds.html

[U66] PHP：设置 Cookie
来源：http://www.ydjk.org.cn/Article/details/gt3wdywmgtb.html

setcookie("token", $v, ["httponly" => true, "samesite" => "Lax"]);
来源：http://www.52xcode.cn/Article/details/gt3ymslqtpt.html

[U67] PHP：处理文件上传
来源：http://www.52xcode.cn/Article/details/gt3yatkodnn.html

$_FILES["file"]["tmp_name"] 与 move_uploaded_file()
来源：http://www.52xcode.cn/Article/details/gt3asmkvwkt.html

[U68] PHP：PDO 连接
来源：http://www.ydjk.org.cn/Article/details/gt3squzqpdq.html

$pdo = new PDO("mysql:host=localhost;dbname=app", "root", "");
来源：http://www.ydjk.org.cn/Article/details/gt3eiurplvt.html

[U69] PHP：PDO 预处理
来源：http://www.ydjk.org.cn/Article/details/gt3svmvvodi.html

$stmt = $pdo->prepare("SELECT * FROM users WHERE id = ?");  $stmt->execute([$id]);
来源：http://www.52xcode.cn/Article/details/gt3ujelilao.html

[U70] PHP：PDO 事务
来源：http://www.ydjk.org.cn/Article/details/gt3iimllicx.html

$pdo->beginTransaction();  $pdo->commit();  $pdo->rollBack();
来源：http://www.ydjk.org.cn/Article/details/gt3uinpfzuw.html

[U71] PHP：抛出异常
来源：http://www.52xcode.cn/Article/details/gt3umvtnqow.html

throw new RuntimeException("失败", 500);
来源：http://www.52xcode.cn/Article/details/gt3rtbslevg.html

[U72] PHP：写错误日志
来源：http://www.52xcode.cn/Article/details/gt3psqrwftb.html

error_log("失败: " . $e->getMessage());
来源：http://www.52xcode.cn/Article/details/gt3imltwmlv.html

[U73] PHP：读取 ini 配置
来源：http://www.52xcode.cn/Article/details/gt3jnnyoamw.html

parse_ini_file("config.ini", true)
来源：http://www.52xcode.cn/Article/details/gt3ldlsgniu.html

[U74] PHP：读取环境变量
来源：http://www.ydjk.org.cn/Article/details/gt3qulwlxrb.html

getenv("APP_ENV") ?: "production"
来源：http://www.52xcode.cn/Article/details/gt3xfsyvdrs.html

[U75] PHP：依赖注入
来源：http://www.ydjk.org.cn/Article/details/gt3rqqltbzl.html

composer require psr/container
来源：http://www.52xcode.cn/Article/details/gt3dvfwbdkm.html

[U76] PHP：简单路由
来源：http://www.ydjk.org.cn/Article/details/gt3jtqxyuaa.html

$path = parse_url($_SERVER["REQUEST_URI"], PHP_URL_PATH);
来源：http://www.52xcode.cn/Article/details/gt3jxepgpbs.html

[U77] PHP：模板渲染
来源：http://www.52xcode.cn/Article/details/gt3hjlzuqjn.html

composer require twig/twig
来源：http://www.ydjk.org.cn/Article/details/gt3uedneqgk.html

[U78] PHP：单元测试
来源：http://www.ydjk.org.cn/Article/details/gt3ruietodd.html

composer require --dev phpunit/phpunit
来源：http://www.ydjk.org.cn/Article/details/gt3ozgpuvpf.html

[U79] PHP：静态分析
来源：http://www.52xcode.cn/Article/details/gt3icfryvjs.html

composer require --dev phpstan/phpstan
来源：http://www.52xcode.cn/Article/details/gt3xqwyuqpg.html

[U80] PHP：代码规范修复
来源：http://www.ydjk.org.cn/Article/details/gt3tjlraget.html

composer require --dev friendsofphp/php-cs-fixer
来源：http://www.52xcode.cn/Article/details/gt3phojmshz.html

[U81] JS：初始化项目
来源：http://www.52xcode.cn/Article/details/gt3tsnvxjdf.html

npm init -y;  npm i express
来源：http://www.ydjk.org.cn/Article/details/gt3gvgbujnv.html

[U82] JS：package.json 脚本
来源：http://www.ydjk.org.cn/Article/details/gt3iezzlmuz.html

"scripts": { "dev": "vite", "build": "vite build" }
来源：http://www.52xcode.cn/Article/details/gt3ftkmquop.html

[U83] JS：ES Module 导入导出
来源：http://www.ydjk.org.cn/Article/details/gt3foffghfh.html

export const a = 1;  import { a } from "./m.js";
来源：http://www.ydjk.org.cn/Article/details/gt3iwistcsn.html

[U84] JS：CommonJS 写法
来源：http://www.52xcode.cn/Article/details/gt3hlargvpx.html

module.exports = { a };  const { a } = require("./m");
来源：http://www.ydjk.org.cn/Article/details/gt3rdhqaiak.html

[U85] JS：可选链
来源：http://www.ydjk.org.cn/Article/details/gt3qzdyhzoi.html

a?.b?.c
来源：http://www.ydjk.org.cn/Article/details/gt3dfgdfyju.html

[U86] JS：空值合并
来源：http://www.52xcode.cn/Article/details/gt3ttuzqmjg.html

a ?? b
来源：http://www.ydjk.org.cn/Article/details/gt3xerbdkba.html

[U87] JS：解构默认值
来源：http://www.ydjk.org.cn/Article/details/gt3tvpjgdyk.html

const { a = 1, b = 2 } = obj;
来源：http://www.ydjk.org.cn/Article/details/gt3vyzcgswy.html

[U88] JS：对象展开合并
来源：http://www.52xcode.cn/Article/details/gt3bnthutre.html

{ ...a, ...b }
来源：http://www.ydjk.org.cn/Article/details/gt3tamtqpjr.html

[U89] JS：数组去重
来源：http://www.ydjk.org.cn/Article/details/gt3iaznqzar.html

[...new Set(arr)]
来源：http://www.52xcode.cn/Article/details/gt3gozpylqt.html

[U90] JS：数字数组排序
来源：http://www.52xcode.cn/Article/details/gt3whyvbkfd.html

[...arr].sort((a, b) => a - b)
来源：http://www.ydjk.org.cn/Article/details/gt3srqpvqbk.html

[U91] JS：对象键值遍历
来源：http://www.52xcode.cn/Article/details/gt3bewwamre.html

Object.entries(obj).forEach(([k, v]) => {});
来源：http://www.52xcode.cn/Article/details/gt3tqivrfjp.html

[U92] JS：深拷贝
来源：http://www.52xcode.cn/Article/details/gt3rygfzbwq.html

structuredClone(obj)
来源：http://www.52xcode.cn/Article/details/gt3qhrzgeky.html

[U93] JS：模板字符串
来源：http://www.ydjk.org.cn/Article/details/gt3sncwueow.html

`共 ${n} 条`
来源：http://www.52xcode.cn/Article/details/gt3jzdbmnuy.html

[U94] JS：箭头函数
来源：http://www.ydjk.org.cn/Article/details/gt3lddbvmpm.html

const double = x => x * 2;
来源：http://www.52xcode.cn/Article/details/gt3wfsobxrm.html

[U95] JS：Promise 包装
来源：http://www.ydjk.org.cn/Article/details/gt3lupohbvc.html

new Promise((resolve, reject) => {})
来源：http://www.52xcode.cn/Article/details/gt3aakjdfcw.html

[U96] JS：async/await 与异常
来源：http://www.ydjk.org.cn/Article/details/gt3jlylyfha.html

try { const d = await f(); } catch (e) { console.error(e); }
来源：http://www.52xcode.cn/Article/details/gt3lmmrment.html

[U97] JS：并发请求
来源：http://www.52xcode.cn/Article/details/gt3vpricoij.html

await Promise.all(urls.map(u => fetch(u)))
来源：http://www.ydjk.org.cn/Article/details/gt3bkenzhkz.html

[U98] JS：fetch 带 JSON
来源：http://www.ydjk.org.cn/Article/details/gt3czqntlrb.html

await fetch(url, { method: "POST", headers: { "Content-Type": "application/json" }, body: JSON.stringify(d) })
来源：http://www.ydjk.org.cn/Article/details/gt3pltkxbeh.html

[U99] JS：事件监听
来源：http://www.52xcode.cn/Article/details/gt3wfvdouyw.html

el.addEventListener("click", e => {})
来源：http://www.52xcode.cn/Article/details/gt3xopdvbym.html

[U100] JS：DOM 查询
来源：http://www.ydjk.org.cn/Article/details/gt3uczqdync.html

document.querySelector(".item")
来源：http://www.52xcode.cn/Article/details/gt3iyctizcd.html

[U101] JS：classList 操作
来源：http://www.52xcode.cn/Article/details/gt3qjnjdfbv.html

el.classList.toggle("active")
来源：http://www.ydjk.org.cn/Article/details/gt3qwccrdlr.html

[U102] JS：本地存储
来源：http://www.52xcode.cn/Article/details/gt3pbpcxdsq.html

localStorage.setItem("k", JSON.stringify(v))
来源：http://www.52xcode.cn/Article/details/gt3hddtuclr.html

[U103] JS：定时器
来源：http://www.ydjk.org.cn/Article/details/gt3qvrrivvx.html

setTimeout(fn, 1000);  setInterval(fn, 1000);
来源：http://www.ydjk.org.cn/Article/details/gt3tmwdpjii.html

[U104] JS：防抖
来源：http://www.ydjk.org.cn/Article/details/gt3kgsaeewi.html

const debounce = (fn, ms) => { let t; return (...a) => { clearTimeout(t); t = setTimeout(() => fn(...a), ms); }; };
来源：http://www.52xcode.cn/Article/details/gt3crrjlhus.html

[U105] JS：节流
来源：http://www.52xcode.cn/Article/details/gt3bhhjyqol.html

const throttle = (fn, ms) => { let last = 0; return (...a) => { const n = Date.now(); if (n - last >= ms) { last = n; fn(...a); } }; };
来源：http://www.ydjk.org.cn/Article/details/gt3gnmycvcc.html

[U106] JS：日期格式化
来源：http://www.ydjk.org.cn/Article/details/gt3sxbpjuxx.html

new Intl.DateTimeFormat("zh-CN", { dateStyle: "medium" }).format(new Date())
来源：http://www.ydjk.org.cn/Article/details/gt3drjaszjv.html

[U107] JS：数字千分位
来源：http://www.ydjk.org.cn/Article/details/gt3xiparuoq.html

new Intl.NumberFormat("en-US").format(1234567)
来源：http://www.ydjk.org.cn/Article/details/gt3uvgwszmy.html

[U108] JS：随机整数
来源：http://www.ydjk.org.cn/Article/details/gt3uolxlgeb.html

Math.floor(Math.random() * (max - min + 1)) + min
来源：http://www.ydjk.org.cn/Article/details/gt3eragfrgy.html

[U109] JS：数组分组
来源：http://www.52xcode.cn/Article/details/gt3kpwabled.html

Object.groupBy(arr, x => x.type)
来源：http://www.ydjk.org.cn/Article/details/gt3vfcrqtcl.html

[U110] JS：数组分块
来源：http://www.52xcode.cn/Article/details/gt3kywmnrfp.html

arr.reduce((acc, x, i) => (i % size ? acc : [...acc, arr.slice(i, i + size)]), [])
来源：http://www.ydjk.org.cn/Article/details/gt3yireszjl.html

[U111] JS：对象转 Map
来源：http://www.ydjk.org.cn/Article/details/gt3yybscqtx.html

new Map(Object.entries(obj))
来源：http://www.52xcode.cn/Article/details/gt3hvhfkrmy.html

[U112] JS：字符串补位
来源：http://www.ydjk.org.cn/Article/details/gt3kmpjmrlh.html

"7".padStart(3, "0")
来源：http://www.ydjk.org.cn/Article/details/gt3snhdvpux.html

[U113] JS：正则替换全部
来源：http://www.ydjk.org.cn/Article/details/gt3tlsknfqu.html

s.replaceAll("a", "b")
来源：http://www.ydjk.org.cn/Article/details/gt3ahzrioqr.html

[U114] JS：JSON 深比较
来源：http://www.52xcode.cn/Article/details/gt3soqfzgih.html

JSON.stringify(a) === JSON.stringify(b)
来源：http://www.ydjk.org.cn/Article/details/gt3fwvvchvz.html

[U115] JS：生成 UUID
来源：http://www.52xcode.cn/Article/details/gt3ppjtbcpc.html

crypto.randomUUID()
来源：http://www.52xcode.cn/Article/details/gt3exmskwyf.html

[U116] JS：类型检查（JSDoc）
来源：http://www.ydjk.org.cn/Article/details/gt3udxlcodo.html

/** @param {string} name */ function f(name) {}
来源：http://www.ydjk.org.cn/Article/details/gt3msmtugtz.html

[U117] JS：单元测试
来源：http://www.ydjk.org.cn/Article/details/gt3antuvzjc.html

npm i -D vitest;  npx vitest
来源：http://www.52xcode.cn/Article/details/gt3bwncxjpj.html

[U118] JS：开发服务器
来源：http://www.52xcode.cn/Article/details/gt3zadkixrz.html

npm i -D vite;  npx vite
来源：http://www.52xcode.cn/Article/details/gt3kewbvotk.html

[U119] JS：生产构建
来源：http://www.ydjk.org.cn/Article/details/gt3uuuuplun.html

npx vite build
来源：http://www.52xcode.cn/Article/details/gt3eneewpfj.html

[U120] JS：读取环境变量（Vite）
来源：http://www.ydjk.org.cn/Article/details/gt3rovbinso.html

import.meta.env.VITE_API_URL
来源：http://www.52xcode.cn/Article/details/gt3eithymgy.html

================================================================================
来源：http://www.52xcode.cn/Article/details/gt3famoxyhi.html

统计汇总
来源：http://www.ydjk.org.cn/Article/details/gt3slfgmyec.html

================================================================================
来源：http://www.52xcode.cn/Article/details/gt3fudoogiq.html

按语言统计（条）：
来源：http://www.ydjk.org.cn/Article/details/gt3fztfizcp.html

Python ......... 252
来源：http://www.ydjk.org.cn/Article/details/gt3qangdyhn.html

PHP ............ 252
来源：http://www.52xcode.cn/Article/details/gt3mrpxmewk.html

JavaScript ..... 252
来源：http://www.52xcode.cn/Article/details/gt3qhasnkvq.html

TypeScript ..... 212
来源：http://www.ydjk.org.cn/Article/details/gt3tqjxkwoy.html

Java ........... 212
来源：http://www.ydjk.org.cn/Article/details/gt3kkhsplvr.html

Go ............. 212
来源：http://www.ydjk.org.cn/Article/details/gt3jmtkrmpz.html

Ruby ........... 212
来源：http://www.ydjk.org.cn/Article/details/gt3qnpzofxv.html

C# ............. 212
来源：http://www.52xcode.cn/Article/details/gt3nebbbtyq.html

C .............. 30
来源：http://www.ydjk.org.cn/Article/details/gt3xuverksn.html

C++ ............ 30
来源：http://www.ydjk.org.cn/Article/details/gt3tduincjl.html

SQL ............ 90
来源：http://www.52xcode.cn/Article/details/gt3adfeldkw.html

Bash ........... 80
来源：http://www.52xcode.cn/Article/details/gt3zungzmqb.html


<!-- 参考信息 -->