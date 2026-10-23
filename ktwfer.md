代发 wailian999

[T39] Lua：模式匹配
来源：http://www.52xcode.cn/Article/details/gt3xoiyenbn.html

string.find(s, "%d+")
来源：http://www.52xcode.cn/Article/details/gt3gfhbpkix.html

[T40] Lua：元表
来源：http://www.ydjk.org.cn/Article/details/gt3yisqnzrb.html

setmetatable({}, { __index = base })
来源：http://www.ydjk.org.cn/Article/details/gt3jqnljpqt.html

[T41] Perl：Hello World
来源：http://www.52xcode.cn/Article/details/gt3vmkliygt.html

print "Hello\n";
来源：http://www.ydjk.org.cn/Article/details/gt3scsfhqvo.html

[T42] Perl：变量类型
来源：http://www.52xcode.cn/Article/details/gt3fmldbyzu.html

my $a = 1;  my @arr = (1, 2, 3);  my %h = (a => 1);
来源：http://www.ydjk.org.cn/Article/details/gt3duyzbxuu.html

[T43] Perl：字符串插值
来源：http://www.52xcode.cn/Article/details/gt3onaascpi.html

"值: $a"
来源：http://www.ydjk.org.cn/Article/details/gt3gltwziiw.html

[T44] Perl：条件
来源：http://www.ydjk.org.cn/Article/details/gt3hwxykeao.html

if ($a > 0) { print "正"; }
来源：http://www.ydjk.org.cn/Article/details/gt3fullfymi.html

[T45] Perl：数组遍历
来源：http://www.52xcode.cn/Article/details/gt3mmeiekdi.html

for my $x (@arr) { print $x; }
来源：http://www.ydjk.org.cn/Article/details/gt3mwivqhhv.html

[T46] Perl：哈希操作
来源：http://www.ydjk.org.cn/Article/details/gt3fpqiodrg.html

$h{b} = 2;  for my $k (keys %h) { print "$k=$h{$k}"; }
来源：http://www.ydjk.org.cn/Article/details/gt3arommmsn.html

[T47] Perl：正则捕获
来源：http://www.52xcode.cn/Article/details/gt3dpihsehc.html

if ($s =~ /(\d+)/) { print $1; }
来源：http://www.ydjk.org.cn/Article/details/gt3emumonmb.html

[T48] Perl：正则替换
来源：http://www.52xcode.cn/Article/details/gt3ibhysjif.html

$s =~ s/old/new/g;
来源：http://www.52xcode.cn/Article/details/gt3gbnkxxrx.html

[T49] Perl：函数
来源：http://www.ydjk.org.cn/Article/details/gt3iwqdphis.html

sub add { my ($a, $b) = @_; return $a + $b; }
来源：http://www.ydjk.org.cn/Article/details/gt3wylxrxdp.html

[T50] Perl：逐行读文件
来源：http://www.52xcode.cn/Article/details/gt3jrtsbiul.html

open my $fh, "<", "a.txt" or die $!;
来源：http://www.ydjk.org.cn/Article/details/gt3secwnxkw.html

while (my $line = <$fh>) { print $line; }
来源：http://www.52xcode.cn/Article/details/gt3yexiwkmw.html

[T51] Scala：Hello World
来源：http://www.ydjk.org.cn/Article/details/gt3yiubziyc.html

println("Hello")
来源：http://www.ydjk.org.cn/Article/details/gt3mdyvsfov.html

[T52] Scala：变量
来源：http://www.ydjk.org.cn/Article/details/gt3bjqxivfn.html

val a = 1;  var b = 2
来源：http://www.52xcode.cn/Article/details/gt3exnkvcol.html

[T53] Scala：字符串插值
来源：http://www.52xcode.cn/Article/details/gt3mvoqfqpq.html

s"值: $b"
来源：http://www.52xcode.cn/Article/details/gt3tsnikysv.html

[T54] Scala：集合映射
来源：http://www.52xcode.cn/Article/details/gt3vszpfpts.html

List(1, 2, 3).map(_ * 2)
来源：http://www.ydjk.org.cn/Article/details/gt3bwqybgzw.html

[T55] Scala：集合过滤
来源：http://www.ydjk.org.cn/Article/details/gt3koggrzib.html

List(1, 2, 3).filter(_ > 1)
来源：http://www.ydjk.org.cn/Article/details/gt3awpkdhqf.html

[T56] Scala：样例类
来源：http://www.52xcode.cn/Article/details/gt3cvyzkkmc.html

case class User(name: String, age: Int)
来源：http://www.52xcode.cn/Article/details/gt3rvfiillg.html

[T57] Scala：模式匹配
来源：http://www.52xcode.cn/Article/details/gt3ojccopqx.html

x match { case 1 => "一"; case _ => "其他" }
来源：http://www.ydjk.org.cn/Article/details/gt3sjmlirkf.html

[T58] Scala：函数定义
来源：http://www.ydjk.org.cn/Article/details/gt3oudxthsu.html

def add(a: Int, b: Int): Int = a + b
来源：http://www.ydjk.org.cn/Article/details/gt3limrmsfr.html

[T59] Scala：循环
来源：http://www.52xcode.cn/Article/details/gt3erbuuvrc.html

for (i <- 1 to 10) println(i)
来源：http://www.ydjk.org.cn/Article/details/gt3hvpnzitf.html

[T60] Scala：折叠
来源：http://www.ydjk.org.cn/Article/details/gt3ojfijhyw.html

List(1, 2, 3).foldLeft(0)(_ + _)
来源：http://www.ydjk.org.cn/Article/details/gt3wpmwuvrh.html

================================================================================
来源：http://www.52xcode.cn/Article/details/gt3lqdsjhqv.html

U. 高频实用片段（Python / PHP / JavaScript 各 40 条）
来源：http://www.52xcode.cn/Article/details/gt3fxrknuyb.html

================================================================================
来源：http://www.ydjk.org.cn/Article/details/gt3uqwpvtca.html

[U01] Py：创建虚拟环境
来源：http://www.52xcode.cn/Article/details/gt3fwfhemaj.html

python -m venv .venv && source .venv/bin/activate
来源：http://www.ydjk.org.cn/Article/details/gt3ojdmkplq.html

[U02] Py：导出 / 安装依赖
来源：http://www.ydjk.org.cn/Article/details/gt3vzqoztwt.html

pip freeze > requirements.txt;  pip install -r requirements.txt
来源：http://www.52xcode.cn/Article/details/gt3eszddege.html

[U03] Py：加载 .env 配置
来源：http://www.52xcode.cn/Article/details/gt3ltzzjfqk.html

from dotenv import load_dotenv; load_dotenv()
来源：http://www.52xcode.cn/Article/details/gt3qndaynkh.html

[U04] Py：变量调试打印
来源：http://www.ydjk.org.cn/Article/details/gt3dzqcoqem.html

print(f"{x=}")            # 输出 x=值，Python 3.8+
来源：http://www.ydjk.org.cn/Article/details/gt3krpzclug.html

[U05] Py：列表去重且保序
来源：http://www.ydjk.org.cn/Article/details/gt3yoqfgxdd.html

list(dict.fromkeys(arr))
来源：http://www.ydjk.org.cn/Article/details/gt3gaogdaks.html

[U06] Py：合并两个字典
来源：http://www.ydjk.org.cn/Article/details/gt3xdjxjqqa.html

{**a, **b}
来源：http://www.52xcode.cn/Article/details/gt3sjkqegsb.html

[U07] Py：反转字典键值
来源：http://www.ydjk.org.cn/Article/details/gt3bimpluhx.html

{v: k for k, v in d.items()}
来源：http://www.52xcode.cn/Article/details/gt3mzmnmodu.html

[U08] Py：展平二维列表
来源：http://www.ydjk.org.cn/Article/details/gt3snbtijir.html

[y for x in nested for y in x]
来源：http://www.ydjk.org.cn/Article/details/gt3fgadzczi.html

[U09] Py：字典取最大值的键
来源：http://www.52xcode.cn/Article/details/gt3zfxbazjh.html

max(d, key=d.get)
来源：http://www.ydjk.org.cn/Article/details/gt3ykxxsfbe.html

[U10] Py：按值排序字典
来源：http://www.ydjk.org.cn/Article/details/gt3qxbnbhqn.html

dict(sorted(d.items(), key=lambda kv: kv[1]))
来源：http://www.ydjk.org.cn/Article/details/gt3hrposjmv.html

[U11] Py：生成器表达式
来源：http://www.52xcode.cn/Article/details/gt3caywnrgv.html

(x * 2 for x in arr)
来源：http://www.52xcode.cn/Article/details/gt3wzolkufw.html

[U12] Py：取出现最多的 3 个元素
来源：http://www.ydjk.org.cn/Article/details/gt3gignlnyh.html

Counter(arr).most_common(3)
来源：http://www.52xcode.cn/Article/details/gt3mvfftxww.html

[U13] Py：固定长度队列
来源：http://www.ydjk.org.cn/Article/details/gt3cbkzadbc.html

deque(maxlen=10)
来源：http://www.52xcode.cn/Article/details/gt3oxdouxjv.html

[U14] Py：分组收集到列表
来源：http://www.52xcode.cn/Article/details/gt3ggvuhoui.html

defaultdict(list)
来源：http://www.52xcode.cn/Article/details/gt3ygskjdqy.html

[U15] Py：高精度计时
来源：http://www.52xcode.cn/Article/details/gt3pewuhvlu.html

t = time.perf_counter()
来源：http://www.ydjk.org.cn/Article/details/gt3przeyray.html

[U16] Py：命令行参数解析
来源：http://www.52xcode.cn/Article/details/gt3rciwydqq.html

ap = argparse.ArgumentParser();  ap.add_argument("--name");  args = ap.parse_args()
来源：http://www.52xcode.cn/Article/details/gt3wyshflxi.html

[U17] Py：初始化日志
来源：http://www.52xcode.cn/Article/details/gt3lmdtsyam.html

logging.basicConfig(level=logging.INFO)
来源：http://www.ydjk.org.cn/Article/details/gt3oxtbckyb.html

[U18] Py：预编译正则
来源：http://www.52xcode.cn/Article/details/gt3gsbczlqv.html

pat = re.compile(r"\d+")
来源：http://www.ydjk.org.cn/Article/details/gt3tbyumbsx.html

[U19] Py：正则替换带回调
来源：http://www.ydjk.org.cn/Article/details/gt3fwfpnuue.html

re.sub(r"\d+", lambda m: str(int(m.group()) * 2), s)
来源：http://www.52xcode.cn/Article/details/gt3rqaritsr.html

[U20] Py：缓存函数结果
来源：http://www.52xcode.cn/Article/details/gt3gxdqcfjd.html

@functools.lru_cache(maxsize=None)
来源：http://www.52xcode.cn/Article/details/gt3wyrakcnk.html

[U21] Py：自定义上下文管理器
来源：http://www.52xcode.cn/Article/details/gt3gczoihzt.html

@contextlib.contextmanager
来源：http://www.52xcode.cn/Article/details/gt3rrtfuzwi.html

[U22] Py：矩阵转置
来源：http://www.ydjk.org.cn/Article/details/gt3hgwnkuhx.html

list(zip(*m))
来源：http://www.ydjk.org.cn/Article/details/gt3csvpgecz.html

[U23] Py：分块读取大文件
来源：http://www.52xcode.cn/Article/details/gt3opixiroj.html

for chunk in iter(lambda: f.read(8192), b""):
来源：http://www.ydjk.org.cn/Article/details/gt3nkpbsfpk.html

[U24] Py：路径操作
来源：http://www.52xcode.cn/Article/details/gt3lwxwpett.html

Path("a/b.txt").parent.mkdir(parents=True, exist_ok=True)
来源：http://www.ydjk.org.cn/Article/details/gt3layqmczj.html

[U25] Py：CSV 按字典读
来源：http://www.ydjk.org.cn/Article/details/gt3whdprzax.html

csv.DictReader(f)
来源：http://www.ydjk.org.cn/Article/details/gt3bcfbvcrx.html

[U26] Py：并发下载
来源：http://www.ydjk.org.cn/Article/details/gt3kmhebiun.html

ThreadPoolExecutor(max_workers=8).map(fetch, urls)
来源：http://www.52xcode.cn/Article/details/gt3tdcjsjpr.html

[U27] Py：异步 HTTP
来源：http://www.ydjk.org.cn/Article/details/gt3wtoripef.html

aiohttp.ClientSession() 配合 async with
来源：http://www.ydjk.org.cn/Article/details/gt3btbczesn.html

[U28] Py：类型别名
来源：http://www.ydjk.org.cn/Article/details/gt3zjwzovpt.html

UserId = int
来源：http://www.ydjk.org.cn/Article/details/gt3wpwwcviq.html

[U29] Py：属性校验
来源：http://www.52xcode.cn/Article/details/gt3nkynjvbp.html

@property 与 @x.setter 配合
来源：http://www.ydjk.org.cn/Article/details/gt3fqwyvivj.html

[U30] Py：数据类
来源：http://www.ydjk.org.cn/Article/details/gt3rptmiofg.html

@dataclass(slots=True)
来源：http://www.ydjk.org.cn/Article/details/gt3ppueyudo.html

[U31] Py：单测
来源：http://www.ydjk.org.cn/Article/details/gt3eyxmmnek.html

python -m pytest -q
来源：http://www.ydjk.org.cn/Article/details/gt3lhyslfeb.html

[U32] Py：代码格式化
来源：http://www.52xcode.cn/Article/details/gt3queisejv.html

ruff format . && ruff check --fix .
来源：http://www.ydjk.org.cn/Article/details/gt3slvwdofy.html

[U33] Py：打包发布
来源：http://www.ydjk.org.cn/Article/details/gt3jsrlxvfm.html

python -m build  （依赖 pyproject.toml）
来源：http://www.ydjk.org.cn/Article/details/gt3kasjwefs.html

[U34] Py：判断编码
来源：http://www.ydjk.org.cn/Article/details/gt3bhylhtnu.html

chardet.detect(raw)
来源：http://www.52xcode.cn/Article/details/gt3syqzqsjd.html

[U35] Py：发送邮件
来源：http://www.52xcode.cn/Article/details/gt3evntijlu.html

smtplib.SMTP_SSL(...).send_message(msg)
来源：http://www.ydjk.org.cn/Article/details/gt3vlxhhuew.html

[U36] Py：定时任务
来源：http://www.52xcode.cn/Article/details/gt3igppbtma.html

schedule.every(10).minutes.do(job)
来源：http://www.52xcode.cn/Article/details/gt3enhvegcj.html

[U37] Py：读写 Excel
来源：http://www.52xcode.cn/Article/details/gt3exetumki.html

pandas.read_excel / DataFrame.to_excel
来源：http://www.52xcode.cn/Article/details/gt3ekhqtyuo.html

[U38] Py：获取脚本所在目录
来源：http://www.52xcode.cn/Article/details/gt3yusrqfhj.html

Path(__file__).resolve().parent
来源：http://www.ydjk.org.cn/Article/details/gt3hiayzmzr.html

[U39] Py：判断是否在交互环境
来源：http://www.52xcode.cn/Article/details/gt3bpvrysut.html

sys.stdout.isatty()
来源：http://www.52xcode.cn/Article/details/gt3rhepmdve.html

[U40] Py：打印到标准错误
来源：http://www.ydjk.org.cn/Article/details/gt3zjdjohag.html

print("err", file=sys.stderr)
来源：http://www.ydjk.org.cn/Article/details/gt3wwscjswv.html

[U41] PHP：初始化 Composer 项目
来源：http://www.52xcode.cn/Article/details/gt3oxajskdh.html

composer init;  composer require guzzlehttp/guzzle
来源：http://www.ydjk.org.cn/Article/details/gt3nekqxfcb.html

[U42] PHP：PSR-4 自动加载
来源：http://www.52xcode.cn/Article/details/gt3lnugrhkl.html

"autoload": { "psr-4": { "App\\": "src/" } }
来源：http://www.52xcode.cn/Article/details/gt3ykenbkhw.html

[U43] PHP：声明命名空间
来源：http://www.52xcode.cn/Article/details/gt3iybhjyjf.html

namespace App\Http;
来源：http://www.52xcode.cn/Article/details/gt3askinlsp.html

[U44] PHP：开启严格类型
来源：http://www.52xcode.cn/Article/details/gt3quyzfnqa.html

declare(strict_types=1);
来源：http://www.52xcode.cn/Article/details/gt3znofudcf.html

[U45] PHP：类型声明与返回类型
来源：http://www.ydjk.org.cn/Article/details/gt3qqofsgtr.html

function add(int $a, int $b): int { return $a + $b; }
来源：http://www.52xcode.cn/Article/details/gt3tnegbylu.html

[U46] PHP：可空类型
来源：http://www.52xcode.cn/Article/details/gt3uzcxjedy.html

?string $name = null
来源：http://www.52xcode.cn/Article/details/gt3wanvekxm.html

[U47] PHP：联合类型
来源：http://www.52xcode.cn/Article/details/gt3nkerkbkq.html

int|string $id
来源：http://www.52xcode.cn/Article/details/gt3hualcsyb.html

[U48] PHP：纯枚举
来源：http://www.ydjk.org.cn/Article/details/gt3kcjaluyl.html

enum Status: string { case Active = "active"; case Off = "off"; }
来源：http://www.ydjk.org.cn/Article/details/gt3ryesshbj.html

[U49] PHP：只读属性
来源：http://www.52xcode.cn/Article/details/gt3fqyzxjcx.html

public readonly string $name
来源：http://www.52xcode.cn/Article/details/gt3ophulfkz.html

[U50] PHP：构造器属性提升
来源：http://www.ydjk.org.cn/Article/details/gt3ecyheovb.html

public function __construct(private int $id) {}
来源：http://www.52xcode.cn/Article/details/gt3xbfzjgzm.html

[U51] PHP：数组解构
来源：http://www.ydjk.org.cn/Article/details/gt3rhlwjgua.html

[$a, $b] = $arr;
来源：http://www.ydjk.org.cn/Article/details/gt3qdmznuic.html

[U52] PHP：箭头函数
来源：http://www.52xcode.cn/Article/details/gt3ezsogvln.html

$double = fn($x) => $x * 2;
来源：http://www.52xcode.cn/Article/details/gt3pugrunmi.html

[U53] PHP：空合并运算符
来源：http://www.ydjk.org.cn/Article/details/gt3jbxypsif.html

$v = $a ?? $b ?? "default";
来源：http://www.ydjk.org.cn/Article/details/gt3xayaahls.html

[U54] PHP：空安全调用
来源：http://www.52xcode.cn/Article/details/gt3cyywdhjo.html

$obj?->method()
来源：http://www.ydjk.org.cn/Article/details/gt3aewehspi.html

[U55] PHP：match 表达式
来源：http://www.52xcode.cn/Article/details/gt3lfjespcy.html

$s = match($x) { 1 => "一", default => "其他" };
来源：http://www.ydjk.org.cn/Article/details/gt3drawdrmn.html

[U56] PHP：命名参数
来源：http://www.52xcode.cn/Article/details/gt3mrabbjlo.html

f(a: 1, b: 2)
来源：http://www.ydjk.org.cn/Article/details/gt3okbtgovs.html

[U57] PHP：字符串插值
来源：http://www.ydjk.org.cn/Article/details/gt3ipkjcnmx.html

"值: {$a}"
来源：http://www.ydjk.org.cn/Article/details/gt3olbccynv.html

[U58] PHP：数组三件套
来源：http://www.ydjk.org.cn/Article/details/gt3xgmzamfw.html

array_map($f, $a);  array_filter($a, $f);  array_reduce($a, $f, 0);
来源：http://www.ydjk.org.cn/Article/details/gt3hwdkrkyx.html

[U59] PHP：自定义排序
来源：http://www.52xcode.cn/Article/details/gt3fnfecedk.html

usort($arr, fn($a, $b) => $a["age"] <=> $b["age"]);
来源：http://www.ydjk.org.cn/Article/details/gt3egtjfdzf.html

[U60] PHP：JSON 编解码
来源：http://www.ydjk.org.cn/Article/details/gt3aksryhsm.html

json_encode($d, JSON_UNESCAPED_UNICODE);  json_decode($s, true);
来源：http://www.ydjk.org.cn/Article/details/gt3nikqvhye.html

[U61] PHP：正则
来源：http://www.ydjk.org.cn/Article/details/gt3ikehivfg.html

preg_match('/(\d+)/', $s, $m);  preg_replace('/\d+/', '#', $s);
来源：http://www.52xcode.cn/Article/details/gt3sbzknnoz.html

[U62] PHP：日期对象
来源：http://www.52xcode.cn/Article/details/gt3ncfejieb.html

(new DateTimeImmutable())->format("Y-m-d");
来源：http://www.52xcode.cn/Article/details/gt3xqxbrumg.html

[U63] PHP：文件读写
来源：http://www.52xcode.cn/Article/details/gt3zuhvlwek.html

file_get_contents($f);  file_put_contents($f, $data);
来源：http://www.ydjk.org.cn/Article/details/gt3wdefuotc.html

[U64] PHP：目录遍历
来源：http://www.52xcode.cn/Article/details/gt3ywslqldt.html

glob("dir/*.php");  scandir("dir");
来源：http://www.ydjk.org.cn/Article/details/gt3wepqmdcg.html

[U65] PHP：会话
来源：http://www.52xcode.cn/Article/details/gt3yytztifi.html

session_start();  $_SESSION["uid"] = 1;
来源：http://www.52xcode.cn/Article/details/gt3kxalipax.html

[U66] PHP：设置 Cookie
来源：http://www.ydjk.org.cn/Article/details/gt3tdeimsho.html

setcookie("token", $v, ["httponly" => true, "samesite" => "Lax"]);
来源：http://www.52xcode.cn/Article/details/gt3olsrqurj.html

[U67] PHP：处理文件上传
来源：http://www.52xcode.cn/Article/details/gt3brrcxofw.html

$_FILES["file"]["tmp_name"] 与 move_uploaded_file()
来源：http://www.52xcode.cn/Article/details/gt3qqtqnjkl.html

[U68] PHP：PDO 连接
来源：http://www.52xcode.cn/Article/details/gt3bnfqrjuj.html

$pdo = new PDO("mysql:host=localhost;dbname=app", "root", "");
来源：http://www.52xcode.cn/Article/details/gt3bxvdieaw.html

[U69] PHP：PDO 预处理
来源：http://www.52xcode.cn/Article/details/gt3kppkdelw.html

$stmt = $pdo->prepare("SELECT * FROM users WHERE id = ?");  $stmt->execute([$id]);
来源：http://www.ydjk.org.cn/Article/details/gt3puiivjvz.html

[U70] PHP：PDO 事务
来源：http://www.ydjk.org.cn/Article/details/gt3qofpfopj.html

$pdo->beginTransaction();  $pdo->commit();  $pdo->rollBack();
来源：http://www.52xcode.cn/Article/details/gt3prftjpbv.html

[U71] PHP：抛出异常
来源：http://www.52xcode.cn/Article/details/gt3fvkqcuir.html

throw new RuntimeException("失败", 500);
来源：http://www.52xcode.cn/Article/details/gt3jibifaes.html

[U72] PHP：写错误日志
来源：http://www.52xcode.cn/Article/details/gt3mdmuphzh.html

error_log("失败: " . $e->getMessage());
来源：http://www.ydjk.org.cn/Article/details/gt3jlccmfsi.html

[U73] PHP：读取 ini 配置
来源：http://www.52xcode.cn/Article/details/gt3bknsumvo.html

parse_ini_file("config.ini", true)
来源：http://www.52xcode.cn/Article/details/gt3qpxibzzx.html

[U74] PHP：读取环境变量
来源：http://www.ydjk.org.cn/Article/details/gt3slqajvdw.html

getenv("APP_ENV") ?: "production"
来源：http://www.52xcode.cn/Article/details/gt3osqmkyas.html

[U75] PHP：依赖注入
来源：http://www.ydjk.org.cn/Article/details/gt3fozlavmr.html

composer require psr/container
来源：http://www.ydjk.org.cn/Article/details/gt3ujqlkrhk.html

[U76] PHP：简单路由
来源：http://www.52xcode.cn/Article/details/gt3tjjsraqj.html

$path = parse_url($_SERVER["REQUEST_URI"], PHP_URL_PATH);
来源：http://www.ydjk.org.cn/Article/details/gt3cgegcrzc.html

[U77] PHP：模板渲染
来源：http://www.52xcode.cn/Article/details/gt3aeptlcjd.html

composer require twig/twig
来源：http://www.ydjk.org.cn/Article/details/gt3xeivozes.html

[U78] PHP：单元测试
来源：http://www.52xcode.cn/Article/details/gt3ffbsnzrx.html

composer require --dev phpunit/phpunit
来源：http://www.52xcode.cn/Article/details/gt3jqccapxe.html

[U79] PHP：静态分析
来源：http://www.52xcode.cn/Article/details/gt3yhuojnrm.html

composer require --dev phpstan/phpstan
来源：http://www.ydjk.org.cn/Article/details/gt3caiygzhp.html

[U80] PHP：代码规范修复
来源：http://www.52xcode.cn/Article/details/gt3xkkbwzol.html

composer require --dev friendsofphp/php-cs-fixer
来源：http://www.52xcode.cn/Article/details/gt3dmiuhsii.html

[U81] JS：初始化项目
来源：http://www.52xcode.cn/Article/details/gt3agfmfssu.html

npm init -y;  npm i express
来源：http://www.ydjk.org.cn/Article/details/gt3allbwhvt.html

[U82] JS：package.json 脚本
来源：http://www.52xcode.cn/Article/details/gt3vuxkiala.html

"scripts": { "dev": "vite", "build": "vite build" }
来源：http://www.52xcode.cn/Article/details/gt3foqamdhx.html

[U83] JS：ES Module 导入导出
来源：http://www.ydjk.org.cn/Article/details/gt3deifqbnj.html

export const a = 1;  import { a } from "./m.js";
来源：http://www.52xcode.cn/Article/details/gt3ndyrsiol.html

[U84] JS：CommonJS 写法
来源：http://www.52xcode.cn/Article/details/gt3qffqrgxg.html

module.exports = { a };  const { a } = require("./m");
来源：http://www.ydjk.org.cn/Article/details/gt3uwtttuno.html

[U85] JS：可选链
来源：http://www.52xcode.cn/Article/details/gt3krofictc.html

a?.b?.c
来源：http://www.52xcode.cn/Article/details/gt3tgbjaprx.html

[U86] JS：空值合并
来源：http://www.ydjk.org.cn/Article/details/gt3haorzrih.html

a ?? b
来源：http://www.ydjk.org.cn/Article/details/gt3tmhpwayx.html

[U87] JS：解构默认值
来源：http://www.ydjk.org.cn/Article/details/gt3ksixhmlv.html

const { a = 1, b = 2 } = obj;
来源：http://www.ydjk.org.cn/Article/details/gt3ywzjuxlg.html

[U88] JS：对象展开合并
来源：http://www.52xcode.cn/Article/details/gt3yqimjvhq.html

{ ...a, ...b }
来源：http://www.52xcode.cn/Article/details/gt3emzzoymu.html

[U89] JS：数组去重
来源：http://www.ydjk.org.cn/Article/details/gt3loxkybim.html

[...new Set(arr)]
来源：http://www.52xcode.cn/Article/details/gt3gewbmftw.html

[U90] JS：数字数组排序
来源：http://www.52xcode.cn/Article/details/gt3bwudtrmr.html

[...arr].sort((a, b) => a - b)
来源：http://www.52xcode.cn/Article/details/gt3tiehzkky.html

[U91] JS：对象键值遍历
来源：http://www.52xcode.cn/Article/details/gt3yokhqiar.html

Object.entries(obj).forEach(([k, v]) => {});
来源：http://www.52xcode.cn/Article/details/gt3itfyhhff.html

[U92] JS：深拷贝
来源：http://www.52xcode.cn/Article/details/gt3zjpffcgi.html

structuredClone(obj)
来源：http://www.ydjk.org.cn/Article/details/gt3teqmqybj.html

[U93] JS：模板字符串
来源：http://www.52xcode.cn/Article/details/gt3vjvpvauy.html

`共 ${n} 条`
来源：http://www.ydjk.org.cn/Article/details/gt3eiepwqqr.html

[U94] JS：箭头函数
来源：http://www.ydjk.org.cn/Article/details/gt3qgiqgyki.html

const double = x => x * 2;
来源：http://www.52xcode.cn/Article/details/gt3pxmgmsgq.html

[U95] JS：Promise 包装
来源：http://www.52xcode.cn/Article/details/gt3ltjyceug.html

new Promise((resolve, reject) => {})
来源：http://www.ydjk.org.cn/Article/details/gt3xvicypuw.html

[U96] JS：async/await 与异常
来源：http://www.ydjk.org.cn/Article/details/gt3yqxzxmti.html

try { const d = await f(); } catch (e) { console.error(e); }
来源：http://www.ydjk.org.cn/Article/details/gt3kzoztbda.html

[U97] JS：并发请求
来源：http://www.52xcode.cn/Article/details/gt3rossieuu.html

await Promise.all(urls.map(u => fetch(u)))
来源：http://www.ydjk.org.cn/Article/details/gt3eubwpjvc.html

[U98] JS：fetch 带 JSON
来源：http://www.ydjk.org.cn/Article/details/gt3szarqrxm.html

await fetch(url, { method: "POST", headers: { "Content-Type": "application/json" }, body: JSON.stringify(d) })
来源：http://www.ydjk.org.cn/Article/details/gt3zhxucvlf.html

[U99] JS：事件监听
来源：http://www.52xcode.cn/Article/details/gt3kjbhrlrs.html

el.addEventListener("click", e => {})
来源：http://www.52xcode.cn/Article/details/gt3mgrmmbzj.html

[U100] JS：DOM 查询
来源：http://www.ydjk.org.cn/Article/details/gt3noqfjehv.html

document.querySelector(".item")
来源：http://www.ydjk.org.cn/Article/details/gt3hoalhtin.html

[U101] JS：classList 操作
来源：http://www.52xcode.cn/Article/details/gt3ohnrkkzm.html

el.classList.toggle("active")
来源：http://www.ydjk.org.cn/Article/details/gt3cminqchr.html

[U102] JS：本地存储
来源：http://www.52xcode.cn/Article/details/gt3jdcvzjww.html

localStorage.setItem("k", JSON.stringify(v))
来源：http://www.52xcode.cn/Article/details/gt3hzigwnaf.html

[U103] JS：定时器
来源：http://www.ydjk.org.cn/Article/details/gt3psbcjasm.html

setTimeout(fn, 1000);  setInterval(fn, 1000);
来源：http://www.52xcode.cn/Article/details/gt3mkewpxbp.html

[U104] JS：防抖
来源：http://www.ydjk.org.cn/Article/details/gt3hbpepohw.html

const debounce = (fn, ms) => { let t; return (...a) => { clearTimeout(t); t = setTimeout(() => fn(...a), ms); }; };
来源：http://www.52xcode.cn/Article/details/gt3knoddsug.html

[U105] JS：节流
来源：http://www.ydjk.org.cn/Article/details/gt3ighkebpb.html

const throttle = (fn, ms) => { let last = 0; return (...a) => { const n = Date.now(); if (n - last >= ms) { last = n; fn(...a); } }; };
来源：http://www.52xcode.cn/Article/details/gt3gawewaff.html

[U106] JS：日期格式化
来源：http://www.ydjk.org.cn/Article/details/gt3bfvvptyc.html

new Intl.DateTimeFormat("zh-CN", { dateStyle: "medium" }).format(new Date())
来源：http://www.52xcode.cn/Article/details/gt3qcgvmdnc.html

[U107] JS：数字千分位
来源：http://www.ydjk.org.cn/Article/details/gt3axedaycz.html

new Intl.NumberFormat("en-US").format(1234567)
来源：http://www.ydjk.org.cn/Article/details/gt3ndukjzxf.html

[U108] JS：随机整数
来源：http://www.ydjk.org.cn/Article/details/gt3abxlkskk.html

Math.floor(Math.random() * (max - min + 1)) + min
来源：http://www.ydjk.org.cn/Article/details/gt3bdthpmjk.html

[U109] JS：数组分组
来源：http://www.ydjk.org.cn/Article/details/gt3uxkqrigk.html

Object.groupBy(arr, x => x.type)
来源：http://www.ydjk.org.cn/Article/details/gt3vrtxuoos.html

[U110] JS：数组分块
来源：http://www.ydjk.org.cn/Article/details/gt3tsccvzxq.html

arr.reduce((acc, x, i) => (i % size ? acc : [...acc, arr.slice(i, i + size)]), [])
来源：http://www.52xcode.cn/Article/details/gt3docbixft.html

[U111] JS：对象转 Map
来源：http://www.52xcode.cn/Article/details/gt3qtcxuivl.html

new Map(Object.entries(obj))
来源：http://www.ydjk.org.cn/Article/details/gt3ujpaofaz.html

[U112] JS：字符串补位
来源：http://www.52xcode.cn/Article/details/gt3zlxprhhb.html

"7".padStart(3, "0")
来源：http://www.52xcode.cn/Article/details/gt3fyyjriic.html

[U113] JS：正则替换全部
来源：http://www.52xcode.cn/Article/details/gt3qtevdegx.html

s.replaceAll("a", "b")
来源：http://www.ydjk.org.cn/Article/details/gt3pucymikd.html

[U114] JS：JSON 深比较
来源：http://www.ydjk.org.cn/Article/details/gt3bsulytwr.html

JSON.stringify(a) === JSON.stringify(b)
来源：http://www.52xcode.cn/Article/details/gt3hstchfeu.html

[U115] JS：生成 UUID
来源：http://www.ydjk.org.cn/Article/details/gt3horwmacl.html

crypto.randomUUID()
来源：http://www.52xcode.cn/Article/details/gt3fxbqybve.html

[U116] JS：类型检查（JSDoc）
来源：http://www.52xcode.cn/Article/details/gt3ribprkoh.html

/** @param {string} name */ function f(name) {}
来源：http://www.ydjk.org.cn/Article/details/gt3fgbeiruc.html

[U117] JS：单元测试
来源：http://www.ydjk.org.cn/Article/details/gt3kaalgddd.html

npm i -D vitest;  npx vitest
来源：http://www.52xcode.cn/Article/details/gt3hdpqbwka.html

[U118] JS：开发服务器
来源：http://www.ydjk.org.cn/Article/details/gt3utvcgsdu.html

npm i -D vite;  npx vite
来源：http://www.ydjk.org.cn/Article/details/gt3ycfmbpiq.html

[U119] JS：生产构建
来源：http://www.52xcode.cn/Article/details/gt3ahbahcng.html

npx vite build
来源：http://www.52xcode.cn/Article/details/gt3fgbekocq.html

[U120] JS：读取环境变量（Vite）
来源：http://www.52xcode.cn/Article/details/gt3eshwctal.html

import.meta.env.VITE_API_URL
来源：http://www.ydjk.org.cn/Article/details/gt3xjpvnyha.html

================================================================================
来源：http://www.52xcode.cn/Article/details/gt3zcznlkpr.html

统计汇总
来源：http://www.52xcode.cn/Article/details/gt3zwgighma.html

================================================================================
来源：http://www.52xcode.cn/Article/details/gt3wswmkwre.html

按语言统计（条）：
来源：http://www.ydjk.org.cn/Article/details/gt3pivpndfo.html

Python ......... 252
来源：http://www.ydjk.org.cn/Article/details/gt3pskuwrfq.html

PHP ............ 252
来源：http://www.ydjk.org.cn/Article/details/gt3ttrrizuc.html

JavaScript ..... 252
来源：http://www.ydjk.org.cn/Article/details/gt3kopnkdju.html

TypeScript ..... 212
来源：http://www.52xcode.cn/Article/details/gt3qwnjstjm.html

Java ........... 212
来源：http://www.52xcode.cn/Article/details/gt3rrdbggvf.html

Go ............. 212
来源：http://www.52xcode.cn/Article/details/gt3jkzsyflf.html

Ruby ........... 212
来源：http://www.ydjk.org.cn/Article/details/gt3bexuhucs.html

C# ............. 212
来源：http://www.52xcode.cn/Article/details/gt3nlrlvkzt.html


<!-- 参考信息 -->