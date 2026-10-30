代发 wailian999

[T47] Perl：正则捕获
来源：http://baike.zdbjq.cn/Article/details/gocbfxici.sHtML

if ($s =~ /(\d+)/) { print $1; }
来源：http://wap.zdbjq.cn/Article/details/gdtfjxlyw.sHtML

[T48] Perl：正则替换
来源：http://read.share.fehbvm.com/Article/details/gudusxouv.sHtML

$s =~ s/old/new/g;
来源：http://blog.hesvh.cn/Article/details/gddryjrbd.sHtML

[T49] Perl：函数
来源：http://www.blog.zdbjq.cn/Article/details/gslfnxela.sHtML

sub add { my ($a, $b) = @_; return $a + $b; }
来源：http://m.share.fehbvm.com/Article/details/glycdwtcs.sHtML

[T50] Perl：逐行读文件
来源：http://m.share.hesvh.cn/Article/details/gmihmlskr.sHtML

open my $fh, "<", "a.txt" or die $!;
来源：http://read.share.hesvh.cn/Article/details/gxomtokox.sHtML

while (my $line = <$fh>) { print $line; }
来源：http://www.m.share.zdbjq.cn/Article/details/gxjljvcdr.sHtML

[T51] Scala：Hello World
来源：http://wap.zdbjq.cn/Article/details/gebwfjzgo.sHtML

println("Hello")
来源：http://blog.fehbvm.com/Article/details/gxvpgkxdu.sHtML

[T52] Scala：变量
来源：http://mobile.fehbvm.com/Article/details/ghohytxtz.sHtML

val a = 1;  var b = 2
来源：http://www.m.share.hesvh.cn/Article/details/gpirwqowv.sHtML

[T53] Scala：字符串插值
来源：http://mobile.hesvh.cn/Article/details/ghjvkzfgp.sHtML

s"值: $b"
来源：http://mobile.zdbjq.cn/Article/details/gwdpolaaw.sHtML

[T54] Scala：集合映射
来源：http://www.share.zdbjq.cn/Article/details/gydagihzi.sHtML

List(1, 2, 3).map(_ * 2)
来源：http://baike.zdbjq.cn/Article/details/golylahkr.sHtML

[T55] Scala：集合过滤
来源：http://www.share.fehbvm.com/Article/details/gibwylcfx.sHtML

List(1, 2, 3).filter(_ > 1)
来源：http://3g.hesvh.cn/Article/details/gunoezrui.sHtML

[T56] Scala：样例类
来源：http://mobile.hesvh.cn/Article/details/gnlpjtqss.sHtML

case class User(name: String, age: Int)
来源：http://www.share.zdbjq.cn/Article/details/goyvmoczv.sHtML

[T57] Scala：模式匹配
来源：http://blog.hesvh.cn/Article/details/gzygnxrwq.sHtML

x match { case 1 => "一"; case _ => "其他" }
来源：http://wap.fehbvm.com/Article/details/gkzwxlstx.sHtML

[T58] Scala：函数定义
来源：http://www.m.share.fehbvm.com/Article/details/gnnqpdget.sHtML

def add(a: Int, b: Int): Int = a + b
来源：http://wap.fehbvm.com/Article/details/grkerpsob.sHtML

[T59] Scala：循环
来源：http://read.share.hesvh.cn/Article/details/glvpfgozp.sHtML

for (i <- 1 to 10) println(i)
来源：http://www.share.hesvh.cn/Article/details/gsndhnxoc.sHtML

[T60] Scala：折叠
来源：http://wap.zdbjq.cn/Article/details/gwwvuxbyx.sHtML

List(1, 2, 3).foldLeft(0)(_ + _)
来源：http://blog.fehbvm.com/Article/details/gttsinprj.sHtML

================================================================================
来源：http://baike.zdbjq.cn/Article/details/gsasnpibp.sHtML

U. 高频实用片段（Python / PHP / JavaScript 各 40 条）
来源：http://read.share.hesvh.cn/Article/details/gqnurzpoo.sHtML

================================================================================
来源：http://3g.hesvh.cn/Article/details/gsqwekfff.sHtML

[U01] Py：创建虚拟环境
来源：http://3g.hesvh.cn/Article/details/gmtdbiaim.sHtML

python -m venv .venv && source .venv/bin/activate
来源：http://www.m.share.zdbjq.cn/Article/details/gxadgncsq.sHtML

[U02] Py：导出 / 安装依赖
来源：http://3g.hesvh.cn/Article/details/gyqainmxf.sHtML

pip freeze > requirements.txt;  pip install -r requirements.txt
来源：http://mobile.hesvh.cn/Article/details/ghvqruvxc.sHtML

[U03] Py：加载 .env 配置
来源：http://m.share.zdbjq.cn/Article/details/gxahmjvxv.sHtML

from dotenv import load_dotenv; load_dotenv()
来源：http://www.m.share.hesvh.cn/Article/details/gsseuqbfe.sHtML

[U04] Py：变量调试打印
来源：http://mobile.zdbjq.cn/Article/details/gdjtyebrs.sHtML

print(f"{x=}")            # 输出 x=值，Python 3.8+
来源：http://wap.hesvh.cn/Article/details/gfchvadkn.sHtML

[U05] Py：列表去重且保序
来源：http://m.share.fehbvm.com/Article/details/gioingfmy.sHtML

list(dict.fromkeys(arr))
来源：http://mobile.hesvh.cn/Article/details/gmsickoao.sHtML

[U06] Py：合并两个字典
来源：http://read.share.hesvh.cn/Article/details/gblzhfrju.sHtML

{**a, **b}
来源：http://read.share.fehbvm.com/Article/details/gpugysnho.sHtML

[U07] Py：反转字典键值
来源：http://3g.hesvh.cn/Article/details/gegjqpokr.sHtML

{v: k for k, v in d.items()}
来源：http://www.share.zdbjq.cn/Article/details/gtwzbaogd.sHtML

[U08] Py：展平二维列表
来源：http://read.share.zdbjq.cn/Article/details/gfohkulyj.sHtML

[y for x in nested for y in x]
来源：http://baike.fehbvm.com/Article/details/gjtafarkj.sHtML

[U09] Py：字典取最大值的键
来源：http://blog.hesvh.cn/Article/details/gbfbkgoxl.sHtML

max(d, key=d.get)
来源：http://mobile.fehbvm.com/Article/details/gctlwtuem.sHtML

[U10] Py：按值排序字典
来源：http://baike.hesvh.cn/Article/details/gxnmtamux.sHtML

dict(sorted(d.items(), key=lambda kv: kv[1]))
来源：http://blog.hesvh.cn/Article/details/gzbtntaag.sHtML

[U11] Py：生成器表达式
来源：http://m.share.fehbvm.com/Article/details/gjyuikepe.sHtML

(x * 2 for x in arr)
来源：http://wap.zdbjq.cn/Article/details/gvuhasxtr.sHtML

[U12] Py：取出现最多的 3 个元素
来源：http://www.blog.hesvh.cn/Article/details/gkcdkbekh.sHtML

Counter(arr).most_common(3)
来源：http://m.share.hesvh.cn/Article/details/gnldujbgz.sHtML

[U13] Py：固定长度队列
来源：http://read.share.hesvh.cn/Article/details/gppvohcqq.sHtML

deque(maxlen=10)
来源：http://www.m.share.fehbvm.com/Article/details/grxlnzvcw.sHtML

[U14] Py：分组收集到列表
来源：http://www.blog.fehbvm.com/Article/details/gkswyusxv.sHtML

defaultdict(list)
来源：http://mobile.fehbvm.com/Article/details/gclbefogx.sHtML

[U15] Py：高精度计时
来源：http://www.m.share.zdbjq.cn/Article/details/glwxndhan.sHtML

t = time.perf_counter()
来源：http://wap.fehbvm.com/Article/details/ghmntifjl.sHtML

[U16] Py：命令行参数解析
来源：http://read.share.fehbvm.com/Article/details/glvbcbqwp.sHtML

ap = argparse.ArgumentParser();  ap.add_argument("--name");  args = ap.parse_args()
来源：http://www.share.fehbvm.com/Article/details/gqgcghcko.sHtML

[U17] Py：初始化日志
来源：http://www.blog.zdbjq.cn/Article/details/gjamvqzjc.sHtML

logging.basicConfig(level=logging.INFO)
来源：http://www.m.share.zdbjq.cn/Article/details/giknvmzdk.sHtML

[U18] Py：预编译正则
来源：http://m.share.hesvh.cn/Article/details/gtlqjgofp.sHtML

pat = re.compile(r"\d+")
来源：http://blog.hesvh.cn/Article/details/gugqqikdf.sHtML

[U19] Py：正则替换带回调
来源：http://wap.hesvh.cn/Article/details/gcfhilypu.sHtML

re.sub(r"\d+", lambda m: str(int(m.group()) * 2), s)
来源：http://read.share.hesvh.cn/Article/details/geevfjdxj.sHtML

[U20] Py：缓存函数结果
来源：http://baike.hesvh.cn/Article/details/grbgxqfft.sHtML

@functools.lru_cache(maxsize=None)
来源：http://www.blog.zdbjq.cn/Article/details/gmipriizr.sHtML

[U21] Py：自定义上下文管理器
来源：http://baike.hesvh.cn/Article/details/gxidesjbe.sHtML

@contextlib.contextmanager
来源：http://www.blog.fehbvm.com/Article/details/gaoyoohcq.sHtML

[U22] Py：矩阵转置
来源：http://www.share.hesvh.cn/Article/details/giinlrald.sHtML

list(zip(*m))
来源：http://www.share.fehbvm.com/Article/details/gsgicmhsa.sHtML

[U23] Py：分块读取大文件
来源：http://blog.fehbvm.com/Article/details/ggkbsbcit.sHtML

for chunk in iter(lambda: f.read(8192), b""):
来源：http://www.m.share.zdbjq.cn/Article/details/gqbxvvgur.sHtML

[U24] Py：路径操作
来源：http://mobile.fehbvm.com/Article/details/godxaffxu.sHtML

Path("a/b.txt").parent.mkdir(parents=True, exist_ok=True)
来源：http://www.blog.hesvh.cn/Article/details/gvwdvyblm.sHtML

[U25] Py：CSV 按字典读
来源：http://wap.zdbjq.cn/Article/details/gwgpvmvvs.sHtML

csv.DictReader(f)
来源：http://m.share.zdbjq.cn/Article/details/gmdkabcab.sHtML

[U26] Py：并发下载
来源：http://read.share.fehbvm.com/Article/details/gimrfcwkl.sHtML

ThreadPoolExecutor(max_workers=8).map(fetch, urls)
来源：http://www.share.zdbjq.cn/Article/details/gcuvalfyb.sHtML

[U27] Py：异步 HTTP
来源：http://baike.hesvh.cn/Article/details/gvyxqptar.sHtML

aiohttp.ClientSession() 配合 async with
来源：http://www.blog.hesvh.cn/Article/details/gohlebdzm.sHtML

[U28] Py：类型别名
来源：http://wap.hesvh.cn/Article/details/gnhxdnaug.sHtML

UserId = int
来源：http://blog.fehbvm.com/Article/details/gsykikbjy.sHtML

[U29] Py：属性校验
来源：http://www.blog.hesvh.cn/Article/details/grxgebtis.sHtML

@property 与 @x.setter 配合
来源：http://wap.zdbjq.cn/Article/details/govhacqgm.sHtML

[U30] Py：数据类
来源：http://3g.hesvh.cn/Article/details/gdthotdqx.sHtML

@dataclass(slots=True)
来源：http://baike.fehbvm.com/Article/details/gkmnszvuc.sHtML

[U31] Py：单测
来源：http://3g.hesvh.cn/Article/details/gggyfanbc.sHtML

python -m pytest -q
来源：http://mobile.zdbjq.cn/Article/details/ghfxtoimd.sHtML

[U32] Py：代码格式化
来源：http://www.m.share.zdbjq.cn/Article/details/gtyzsrven.sHtML

ruff format . && ruff check --fix .
来源：http://baike.hesvh.cn/Article/details/gwmuwwvap.sHtML

[U33] Py：打包发布
来源：http://www.m.share.zdbjq.cn/Article/details/gcrwkyzml.sHtML

python -m build  （依赖 pyproject.toml）
来源：http://baike.hesvh.cn/Article/details/gwfifoyhu.sHtML

[U34] Py：判断编码
来源：http://www.share.zdbjq.cn/Article/details/gpjmbouck.sHtML

chardet.detect(raw)
来源：http://m.share.zdbjq.cn/Article/details/gijvjohhx.sHtML

[U35] Py：发送邮件
来源：http://baike.zdbjq.cn/Article/details/gryduvqkz.sHtML

smtplib.SMTP_SSL(...).send_message(msg)
来源：http://wap.fehbvm.com/Article/details/gztbinpgi.sHtML

[U36] Py：定时任务
来源：http://mobile.hesvh.cn/Article/details/gfgvfqvru.sHtML

schedule.every(10).minutes.do(job)
来源：http://www.share.hesvh.cn/Article/details/gpgilnhci.sHtML

[U37] Py：读写 Excel
来源：http://baike.fehbvm.com/Article/details/gmexzttka.sHtML

pandas.read_excel / DataFrame.to_excel
来源：http://baike.zdbjq.cn/Article/details/gekeimvit.sHtML

[U38] Py：获取脚本所在目录
来源：http://3g.zdbjq.cn/Article/details/gcyuvsnlx.sHtML

Path(__file__).resolve().parent
来源：http://blog.zdbjq.cn/Article/details/gaokcaxsv.sHtML

[U39] Py：判断是否在交互环境
来源：http://www.m.share.zdbjq.cn/Article/details/gidnozgur.sHtML

sys.stdout.isatty()
来源：http://baike.fehbvm.com/Article/details/grmtkcdzi.sHtML

[U40] Py：打印到标准错误
来源：http://m.share.zdbjq.cn/Article/details/gtbozbkeq.sHtML

print("err", file=sys.stderr)
来源：http://m.share.zdbjq.cn/Article/details/grbbzliuq.sHtML

[U41] PHP：初始化 Composer 项目
来源：http://baike.zdbjq.cn/Article/details/gebppgbiw.sHtML

composer init;  composer require guzzlehttp/guzzle
来源：http://wap.fehbvm.com/Article/details/gokdzpors.sHtML

[U42] PHP：PSR-4 自动加载
来源：http://blog.fehbvm.com/Article/details/gjqoeexcu.sHtML

"autoload": { "psr-4": { "App\\": "src/" } }
来源：http://blog.fehbvm.com/Article/details/gmkiclxyc.sHtML

[U43] PHP：声明命名空间
来源：http://www.blog.fehbvm.com/Article/details/gagaceues.sHtML

namespace App\Http;
来源：http://m.share.zdbjq.cn/Article/details/gqiaiiflj.sHtML

[U44] PHP：开启严格类型
来源：http://www.m.share.fehbvm.com/Article/details/gkubtpzad.sHtML

declare(strict_types=1);
来源：http://www.m.share.hesvh.cn/Article/details/gqurnhgbp.sHtML

[U45] PHP：类型声明与返回类型
来源：http://m.share.zdbjq.cn/Article/details/gozkelpvu.sHtML

function add(int $a, int $b): int { return $a + $b; }
来源：http://www.blog.fehbvm.com/Article/details/gydvxpkrk.sHtML

[U46] PHP：可空类型
来源：http://wap.hesvh.cn/Article/details/gtskxnhfc.sHtML

?string $name = null
来源：http://mobile.zdbjq.cn/Article/details/gfmwnncpu.sHtML

[U47] PHP：联合类型
来源：http://blog.hesvh.cn/Article/details/ggzcvvira.sHtML

int|string $id
来源：http://blog.zdbjq.cn/Article/details/gzquxujsc.sHtML

[U48] PHP：纯枚举
来源：http://www.blog.zdbjq.cn/Article/details/gphciiapx.sHtML

enum Status: string { case Active = "active"; case Off = "off"; }
来源：http://www.blog.fehbvm.com/Article/details/gmtxvbrda.sHtML

[U49] PHP：只读属性
来源：http://blog.zdbjq.cn/Article/details/goycdatwi.sHtML

public readonly string $name
来源：http://www.share.fehbvm.com/Article/details/ggcbhjzli.sHtML

[U50] PHP：构造器属性提升
来源：http://wap.zdbjq.cn/Article/details/gfdkwqabc.sHtML

public function __construct(private int $id) {}
来源：http://blog.fehbvm.com/Article/details/giidjieiw.sHtML

[U51] PHP：数组解构
来源：http://read.share.zdbjq.cn/Article/details/gqgxogfhl.sHtML

[$a, $b] = $arr;
来源：http://wap.fehbvm.com/Article/details/getsunwop.sHtML

[U52] PHP：箭头函数
来源：http://www.m.share.fehbvm.com/Article/details/gygniwdlh.sHtML

$double = fn($x) => $x * 2;
来源：http://blog.fehbvm.com/Article/details/glzewxvsd.sHtML

[U53] PHP：空合并运算符
来源：http://baike.zdbjq.cn/Article/details/gzfyixuop.sHtML

$v = $a ?? $b ?? "default";
来源：http://mobile.hesvh.cn/Article/details/glpcskxfn.sHtML

[U54] PHP：空安全调用
来源：http://m.share.hesvh.cn/Article/details/gyvkawudu.sHtML

$obj?->method()
来源：http://www.blog.hesvh.cn/Article/details/gkcmoiunk.sHtML

[U55] PHP：match 表达式
来源：http://blog.fehbvm.com/Article/details/guzzkpngq.sHtML

$s = match($x) { 1 => "一", default => "其他" };
来源：http://m.share.fehbvm.com/Article/details/giosiwehg.sHtML

[U56] PHP：命名参数
来源：http://read.share.hesvh.cn/Article/details/gzxdedjef.sHtML

f(a: 1, b: 2)
来源：http://m.share.fehbvm.com/Article/details/gtuokjjrb.sHtML

[U57] PHP：字符串插值
来源：http://read.share.fehbvm.com/Article/details/gmxtevjua.sHtML

"值: {$a}"
来源：http://www.share.hesvh.cn/Article/details/gktercpzv.sHtML

[U58] PHP：数组三件套
来源：http://m.share.zdbjq.cn/Article/details/groumztdl.sHtML

array_map($f, $a);  array_filter($a, $f);  array_reduce($a, $f, 0);
来源：http://m.share.fehbvm.com/Article/details/gmoidqeqp.sHtML

[U59] PHP：自定义排序
来源：http://3g.zdbjq.cn/Article/details/gulhddruy.sHtML

usort($arr, fn($a, $b) => $a["age"] <=> $b["age"]);
来源：http://mobile.fehbvm.com/Article/details/gmgrbhywj.sHtML

[U60] PHP：JSON 编解码
来源：http://baike.zdbjq.cn/Article/details/gpeobjzif.sHtML

json_encode($d, JSON_UNESCAPED_UNICODE);  json_decode($s, true);
来源：http://www.m.share.hesvh.cn/Article/details/ggiqbbyhl.sHtML

[U61] PHP：正则
来源：http://www.share.zdbjq.cn/Article/details/gevvllpgh.sHtML

preg_match('/(\d+)/', $s, $m);  preg_replace('/\d+/', '#', $s);
来源：http://wap.fehbvm.com/Article/details/gghqvqumt.sHtML

[U62] PHP：日期对象
来源：http://3g.zdbjq.cn/Article/details/gazrehtis.sHtML

(new DateTimeImmutable())->format("Y-m-d");
来源：http://3g.zdbjq.cn/Article/details/gglibsisn.sHtML

[U63] PHP：文件读写
来源：http://read.share.fehbvm.com/Article/details/gewmenecu.sHtML

file_get_contents($f);  file_put_contents($f, $data);
来源：http://blog.zdbjq.cn/Article/details/gueqzasgo.sHtML

[U64] PHP：目录遍历
来源：http://www.m.share.zdbjq.cn/Article/details/gxwhrnbvf.sHtML

glob("dir/*.php");  scandir("dir");
来源：http://wap.zdbjq.cn/Article/details/gzuhmrtju.sHtML

[U65] PHP：会话
来源：http://mobile.hesvh.cn/Article/details/gbcnamyca.sHtML

session_start();  $_SESSION["uid"] = 1;
来源：http://read.share.fehbvm.com/Article/details/gdvranxss.sHtML

[U66] PHP：设置 Cookie
来源：http://read.share.fehbvm.com/Article/details/gpyykzdnj.sHtML

setcookie("token", $v, ["httponly" => true, "samesite" => "Lax"]);
来源：http://read.share.zdbjq.cn/Article/details/grjknyuka.sHtML

[U67] PHP：处理文件上传
来源：http://blog.zdbjq.cn/Article/details/gizgxzrtu.sHtML

$_FILES["file"]["tmp_name"] 与 move_uploaded_file()
来源：http://3g.hesvh.cn/Article/details/gowandstq.sHtML

[U68] PHP：PDO 连接
来源：http://3g.zdbjq.cn/Article/details/gddkzbztt.sHtML

$pdo = new PDO("mysql:host=localhost;dbname=app", "root", "");
来源：http://www.blog.zdbjq.cn/Article/details/gwvrsaiay.sHtML

[U69] PHP：PDO 预处理
来源：http://wap.hesvh.cn/Article/details/gtspvpsbo.sHtML

$stmt = $pdo->prepare("SELECT * FROM users WHERE id = ?");  $stmt->execute([$id]);
来源：http://baike.hesvh.cn/Article/details/gpaoyttay.sHtML

[U70] PHP：PDO 事务
来源：http://www.share.hesvh.cn/Article/details/gyptpntjx.sHtML

$pdo->beginTransaction();  $pdo->commit();  $pdo->rollBack();
来源：http://m.share.fehbvm.com/Article/details/gmsggpbsh.sHtML

[U71] PHP：抛出异常
来源：http://baike.hesvh.cn/Article/details/glntnxjzy.sHtML

throw new RuntimeException("失败", 500);
来源：http://wap.hesvh.cn/Article/details/gacqtrrix.sHtML

[U72] PHP：写错误日志
来源：http://wap.fehbvm.com/Article/details/gliohoeju.sHtML

error_log("失败: " . $e->getMessage());
来源：http://www.blog.hesvh.cn/Article/details/gqpoumcly.sHtML

[U73] PHP：读取 ini 配置
来源：http://www.blog.hesvh.cn/Article/details/gtwqdyrhp.sHtML

parse_ini_file("config.ini", true)
来源：http://www.blog.zdbjq.cn/Article/details/gjpagiqnm.sHtML

[U74] PHP：读取环境变量
来源：http://m.share.hesvh.cn/Article/details/glwnseups.sHtML

getenv("APP_ENV") ?: "production"
来源：http://blog.fehbvm.com/Article/details/gcwjbzjro.sHtML

[U75] PHP：依赖注入
来源：http://3g.hesvh.cn/Article/details/gkjycokuf.sHtML

composer require psr/container
来源：http://www.m.share.fehbvm.com/Article/details/gdupislrx.sHtML

[U76] PHP：简单路由
来源：http://www.m.share.hesvh.cn/Article/details/gquahpyzs.sHtML

$path = parse_url($_SERVER["REQUEST_URI"], PHP_URL_PATH);
来源：http://3g.hesvh.cn/Article/details/gfenhuaui.sHtML

[U77] PHP：模板渲染
来源：http://www.blog.fehbvm.com/Article/details/gidkmqhib.sHtML

composer require twig/twig
来源：http://baike.zdbjq.cn/Article/details/gqyhivebr.sHtML

[U78] PHP：单元测试
来源：http://wap.zdbjq.cn/Article/details/gciylgwzw.sHtML

composer require --dev phpunit/phpunit
来源：http://www.share.fehbvm.com/Article/details/gjmylngwo.sHtML

[U79] PHP：静态分析
来源：http://mobile.zdbjq.cn/Article/details/grngsvoce.sHtML

composer require --dev phpstan/phpstan
来源：http://www.blog.fehbvm.com/Article/details/gdxfgfhdv.sHtML

[U80] PHP：代码规范修复
来源：http://wap.hesvh.cn/Article/details/gwscqvnke.sHtML

composer require --dev friendsofphp/php-cs-fixer
来源：http://m.share.fehbvm.com/Article/details/gockkjcje.sHtML

[U81] JS：初始化项目
来源：http://mobile.fehbvm.com/Article/details/gzpjeklne.sHtML

npm init -y;  npm i express
来源：http://wap.hesvh.cn/Article/details/gstfurtyo.sHtML

[U82] JS：package.json 脚本
来源：http://m.share.hesvh.cn/Article/details/gglmsavrd.sHtML

"scripts": { "dev": "vite", "build": "vite build" }
来源：http://m.share.hesvh.cn/Article/details/gwtdypcub.sHtML

[U83] JS：ES Module 导入导出
来源：http://3g.hesvh.cn/Article/details/gqhcutmab.sHtML

export const a = 1;  import { a } from "./m.js";
来源：http://www.share.fehbvm.com/Article/details/gxcxhzldx.sHtML

[U84] JS：CommonJS 写法
来源：http://3g.zdbjq.cn/Article/details/gisplhqtk.sHtML

module.exports = { a };  const { a } = require("./m");
来源：http://www.m.share.zdbjq.cn/Article/details/gyiehhvqb.sHtML

[U85] JS：可选链
来源：http://wap.hesvh.cn/Article/details/gnckysual.sHtML

a?.b?.c
来源：http://blog.hesvh.cn/Article/details/getlwadjh.sHtML

[U86] JS：空值合并
来源：http://read.share.hesvh.cn/Article/details/gnulbdusf.sHtML

a ?? b
来源：http://read.share.fehbvm.com/Article/details/gwrscujgy.sHtML

[U87] JS：解构默认值
来源：http://www.m.share.hesvh.cn/Article/details/gvqgwdije.sHtML

const { a = 1, b = 2 } = obj;
来源：http://mobile.zdbjq.cn/Article/details/gwhyqqsco.sHtML

[U88] JS：对象展开合并
来源：http://www.share.hesvh.cn/Article/details/gghdazkbg.sHtML

{ ...a, ...b }
来源：http://blog.zdbjq.cn/Article/details/gsgcpctyo.sHtML

[U89] JS：数组去重
来源：http://wap.zdbjq.cn/Article/details/gylyxylty.sHtML

[...new Set(arr)]
来源：http://www.share.zdbjq.cn/Article/details/gqzmnzxqw.sHtML

[U90] JS：数字数组排序
来源：http://baike.zdbjq.cn/Article/details/gesfbsuju.sHtML

[...arr].sort((a, b) => a - b)
来源：http://3g.hesvh.cn/Article/details/ghqsdgtoh.sHtML

[U91] JS：对象键值遍历
来源：http://www.blog.fehbvm.com/Article/details/gmqnvehfc.sHtML

Object.entries(obj).forEach(([k, v]) => {});
来源：http://www.m.share.zdbjq.cn/Article/details/gcjmauclr.sHtML

[U92] JS：深拷贝
来源：http://blog.fehbvm.com/Article/details/gyzbaxxaj.sHtML

structuredClone(obj)
来源：http://www.share.zdbjq.cn/Article/details/gvxrdzwug.sHtML

[U93] JS：模板字符串
来源：http://baike.zdbjq.cn/Article/details/gzoxuxyon.sHtML

`共 ${n} 条`
来源：http://wap.zdbjq.cn/Article/details/gtfinjjjv.sHtML

[U94] JS：箭头函数
来源：http://www.share.fehbvm.com/Article/details/ghfjcxcvm.sHtML

const double = x => x * 2;
来源：http://www.blog.fehbvm.com/Article/details/gnuvzcffx.sHtML

[U95] JS：Promise 包装
来源：http://mobile.hesvh.cn/Article/details/gndzaaasy.sHtML

new Promise((resolve, reject) => {})
来源：http://m.share.hesvh.cn/Article/details/gcajbekgc.sHtML

[U96] JS：async/await 与异常
来源：http://baike.zdbjq.cn/Article/details/gkfqpkflg.sHtML

try { const d = await f(); } catch (e) { console.error(e); }
来源：http://www.blog.fehbvm.com/Article/details/gyfsjvhzf.sHtML

[U97] JS：并发请求
来源：http://blog.fehbvm.com/Article/details/gzrloykjr.sHtML

await Promise.all(urls.map(u => fetch(u)))
来源：http://baike.zdbjq.cn/Article/details/gjpltyqbd.sHtML

[U98] JS：fetch 带 JSON
来源：http://mobile.hesvh.cn/Article/details/gtajoidav.sHtML

await fetch(url, { method: "POST", headers: { "Content-Type": "application/json" }, body: JSON.stringify(d) })
来源：http://www.share.zdbjq.cn/Article/details/gyktkldag.sHtML

[U99] JS：事件监听
来源：http://www.blog.zdbjq.cn/Article/details/gafoslsly.sHtML

el.addEventListener("click", e => {})
来源：http://mobile.fehbvm.com/Article/details/gjrcljsoi.sHtML

[U100] JS：DOM 查询
来源：http://wap.zdbjq.cn/Article/details/gpkvqwaku.sHtML

document.querySelector(".item")
来源：http://www.blog.fehbvm.com/Article/details/gqqtxfjzr.sHtML

[U101] JS：classList 操作
来源：http://blog.hesvh.cn/Article/details/gzbsckbtk.sHtML

el.classList.toggle("active")
来源：http://wap.fehbvm.com/Article/details/gswijzwqz.sHtML

[U102] JS：本地存储
来源：http://www.m.share.hesvh.cn/Article/details/gvutxxyfh.sHtML

localStorage.setItem("k", JSON.stringify(v))
来源：http://blog.hesvh.cn/Article/details/gbormxwuo.sHtML

[U103] JS：定时器
来源：http://m.share.fehbvm.com/Article/details/gdfecqeur.sHtML

setTimeout(fn, 1000);  setInterval(fn, 1000);
来源：http://m.share.hesvh.cn/Article/details/gakvmmtms.sHtML

[U104] JS：防抖
来源：http://blog.fehbvm.com/Article/details/gcnkvuzew.sHtML

const debounce = (fn, ms) => { let t; return (...a) => { clearTimeout(t); t = setTimeout(() => fn(...a), ms); }; };
来源：http://www.m.share.fehbvm.com/Article/details/gvwmvjmip.sHtML

[U105] JS：节流
来源：http://3g.hesvh.cn/Article/details/gjaeawdjc.sHtML

const throttle = (fn, ms) => { let last = 0; return (...a) => { const n = Date.now(); if (n - last >= ms) { last = n; fn(...a); } }; };
来源：http://m.share.zdbjq.cn/Article/details/grhruogvx.sHtML

[U106] JS：日期格式化
来源：http://blog.hesvh.cn/Article/details/giijnlejz.sHtML

new Intl.DateTimeFormat("zh-CN", { dateStyle: "medium" }).format(new Date())
来源：http://wap.zdbjq.cn/Article/details/gufpprnsr.sHtML

[U107] JS：数字千分位
来源：http://baike.hesvh.cn/Article/details/gpdkanjmc.sHtML

new Intl.NumberFormat("en-US").format(1234567)
来源：http://3g.zdbjq.cn/Article/details/gzzfcasug.sHtML

[U108] JS：随机整数
来源：http://3g.zdbjq.cn/Article/details/gpmexuurz.sHtML

Math.floor(Math.random() * (max - min + 1)) + min
来源：http://www.m.share.zdbjq.cn/Article/details/gcnniegan.sHtML

[U109] JS：数组分组
来源：http://blog.zdbjq.cn/Article/details/gmdykmnpm.sHtML

Object.groupBy(arr, x => x.type)
来源：http://www.share.zdbjq.cn/Article/details/gvcnojzhc.sHtML

[U110] JS：数组分块
来源：http://blog.hesvh.cn/Article/details/groeoyndr.sHtML

arr.reduce((acc, x, i) => (i % size ? acc : [...acc, arr.slice(i, i + size)]), [])
来源：http://read.share.hesvh.cn/Article/details/guuqdjetc.sHtML

[U111] JS：对象转 Map
来源：http://baike.fehbvm.com/Article/details/gftttwabs.sHtML

new Map(Object.entries(obj))
来源：http://blog.hesvh.cn/Article/details/gevlipjka.sHtML

[U112] JS：字符串补位
来源：http://blog.fehbvm.com/Article/details/guxtcdsda.sHtML

"7".padStart(3, "0")
来源：http://m.share.fehbvm.com/Article/details/ghinnlstf.sHtML

[U113] JS：正则替换全部
来源：http://3g.zdbjq.cn/Article/details/gxligbouy.sHtML

s.replaceAll("a", "b")
来源：http://3g.fehbvm.com/Article/details/gctjriveg.sHtML

[U114] JS：JSON 深比较
来源：http://www.blog.fehbvm.com/Article/details/gjkrxfzty.sHtML

JSON.stringify(a) === JSON.stringify(b)
来源：http://mobile.zdbjq.cn/Article/details/guvtthoak.sHtML

[U115] JS：生成 UUID
来源：http://wap.fehbvm.com/Article/details/gpwupommo.sHtML

crypto.randomUUID()
来源：http://wap.zdbjq.cn/Article/details/ghqrpkdct.sHtML

[U116] JS：类型检查（JSDoc）
来源：http://www.m.share.fehbvm.com/Article/details/gamwxieex.sHtML

/** @param {string} name */ function f(name) {}
来源：http://3g.fehbvm.com/Article/details/gnplerlgn.sHtML

[U117] JS：单元测试
来源：http://baike.zdbjq.cn/Article/details/gpjbvogxp.sHtML

npm i -D vitest;  npx vitest
来源：http://baike.fehbvm.com/Article/details/gajqyzrfi.sHtML

[U118] JS：开发服务器
来源：http://www.m.share.fehbvm.com/Article/details/gajyflfyh.sHtML

npm i -D vite;  npx vite
来源：http://blog.hesvh.cn/Article/details/gtsgrxmiz.sHtML

[U119] JS：生产构建
来源：http://www.blog.zdbjq.cn/Article/details/gxokmeqce.sHtML

npx vite build
来源：http://www.m.share.fehbvm.com/Article/details/gscclmdop.sHtML

[U120] JS：读取环境变量（Vite）
来源：http://www.blog.fehbvm.com/Article/details/gnqjjmkyg.sHtML

import.meta.env.VITE_API_URL
来源：http://www.m.share.zdbjq.cn/Article/details/gpwruhlsh.sHtML

================================================================================
来源：http://m.share.hesvh.cn/Article/details/gulnkzxyi.sHtML

统计汇总
来源：http://wap.hesvh.cn/Article/details/gzzmoxolz.sHtML

================================================================================
来源：http://mobile.zdbjq.cn/Article/details/gegussqfp.sHtML

按语言统计（条）：
来源：http://read.share.fehbvm.com/Article/details/glzdxmqiu.sHtML

Python ......... 252
来源：http://www.share.hesvh.cn/Article/details/gqxfvcnvm.sHtML

PHP ............ 252
来源：http://3g.zdbjq.cn/Article/details/gomrqtbfu.sHtML

JavaScript ..... 252
来源：http://mobile.hesvh.cn/Article/details/geruqhxeq.sHtML

TypeScript ..... 212
来源：http://baike.zdbjq.cn/Article/details/gjuuyawtc.sHtML

Java ........... 212
来源：http://m.share.zdbjq.cn/Article/details/gdzohofpq.sHtML

Go ............. 212
来源：http://3g.zdbjq.cn/Article/details/gipwukkgr.sHtML

Ruby ........... 212
来源：http://read.share.hesvh.cn/Article/details/gxiejqsfw.sHtML

C# ............. 212
来源：http://baike.fehbvm.com/Article/details/gfypvfzme.sHtML

C .............. 30
来源：http://mobile.zdbjq.cn/Article/details/gzplvvsek.sHtML

C++ ............ 30
来源：http://read.share.hesvh.cn/Article/details/gzvmzkbtk.sHtML

SQL ............ 90
来源：http://www.m.share.fehbvm.com/Article/details/gamzoplxb.sHtML

Bash ........... 80
来源：http://m.share.zdbjq.cn/Article/details/gqsjttruu.sHtML

Kotlin ......... 15
来源：http://www.blog.fehbvm.com/Article/details/gqgpvhfog.sHtML

Swift .......... 15
来源：http://www.m.share.fehbvm.com/Article/details/gdltvdkjz.sHtML

Lua ............ 10
来源：http://blog.fehbvm.com/Article/details/gydrahrbh.sHtML

Perl ........... 10
来源：http://m.share.fehbvm.com/Article/details/gxyseuwja.sHtML

Scala .......... 10
来源：http://www.blog.zdbjq.cn/Article/details/gefbmtkoy.sHtML

------------------------------------
来源：http://3g.hesvh.cn/Article/details/gwoheltqt.sHtML

合计 ........... 2106 条
来源：http://3g.zdbjq.cn/Article/details/gtzefcsqo.sHtML

按章节统计：
来源：http://blog.fehbvm.com/Article/details/gkffmwvys.sHtML

A 基础语法与类型       26 个任务 × 8 语言 =  208
来源：http://wap.zdbjq.cn/Article/details/gwsxnirzr.sHtML

B 流程控制             16 个任务 × 8 语言 =  128
来源：http://3g.fehbvm.com/Article/details/gbtqjclcn.sHtML

C 函数与作用域         16 个任务 × 8 语言 =  128
来源：http://www.m.share.zdbjq.cn/Article/details/gnsfhswxx.sHtML

D 数组 / 列表 / 集合   26 个任务 × 8 语言 =  208
来源：http://mobile.hesvh.cn/Article/details/gthijbdbp.sHtML


<!-- 参考信息 -->