代发 wailian999

[T41] Perl：Hello World
来源：http://m.share.hesvh.cn/Article/details/gevvbeofc.sHtML

print "Hello\n";
来源：http://www.share.fehbvm.com/Article/details/gctrtqjkn.sHtML

[T42] Perl：变量类型
来源：http://blog.hesvh.cn/Article/details/gjtqqithl.sHtML

my $a = 1;  my @arr = (1, 2, 3);  my %h = (a => 1);
来源：http://mobile.zdbjq.cn/Article/details/gpyoajssr.sHtML

[T43] Perl：字符串插值
来源：http://read.share.zdbjq.cn/Article/details/gotrgekrr.sHtML

"值: $a"
来源：http://blog.zdbjq.cn/Article/details/gveuxuxgj.sHtML

[T44] Perl：条件
来源：http://www.m.share.fehbvm.com/Article/details/grufjrbjy.sHtML

if ($a > 0) { print "正"; }
来源：http://blog.fehbvm.com/Article/details/gnoybzgmx.sHtML

[T45] Perl：数组遍历
来源：http://read.share.fehbvm.com/Article/details/gwtwpnwkw.sHtML

for my $x (@arr) { print $x; }
来源：http://blog.hesvh.cn/Article/details/gpblssqob.sHtML

[T46] Perl：哈希操作
来源：http://blog.fehbvm.com/Article/details/gmutxueqk.sHtML

$h{b} = 2;  for my $k (keys %h) { print "$k=$h{$k}"; }
来源：http://mobile.fehbvm.com/Article/details/gkntxfqyz.sHtML

[T47] Perl：正则捕获
来源：http://3g.zdbjq.cn/Article/details/graphfrha.sHtML

if ($s =~ /(\d+)/) { print $1; }
来源：http://m.share.zdbjq.cn/Article/details/gbjhxhprb.sHtML

[T48] Perl：正则替换
来源：http://3g.zdbjq.cn/Article/details/gdpqgmsts.sHtML

$s =~ s/old/new/g;
来源：http://read.share.zdbjq.cn/Article/details/gcwqmzmxs.sHtML

[T49] Perl：函数
来源：http://baike.fehbvm.com/Article/details/gsupuumsq.sHtML

sub add { my ($a, $b) = @_; return $a + $b; }
来源：http://www.share.zdbjq.cn/Article/details/gmszispkg.sHtML

[T50] Perl：逐行读文件
来源：http://3g.hesvh.cn/Article/details/gfhlffwuz.sHtML

open my $fh, "<", "a.txt" or die $!;
来源：http://baike.zdbjq.cn/Article/details/grgrmrrzk.sHtML

while (my $line = <$fh>) { print $line; }
来源：http://baike.fehbvm.com/Article/details/gkrshfyex.sHtML

[T51] Scala：Hello World
来源：http://www.blog.zdbjq.cn/Article/details/gzlhjdlsl.sHtML

println("Hello")
来源：http://www.blog.hesvh.cn/Article/details/grspljmfp.sHtML

[T52] Scala：变量
来源：http://wap.hesvh.cn/Article/details/gduqxmzvk.sHtML

val a = 1;  var b = 2
来源：http://www.blog.zdbjq.cn/Article/details/gkybmcjpp.sHtML

[T53] Scala：字符串插值
来源：http://www.m.share.fehbvm.com/Article/details/ghydyyhcg.sHtML

s"值: $b"
来源：http://blog.fehbvm.com/Article/details/gsezevfpc.sHtML

[T54] Scala：集合映射
来源：http://wap.fehbvm.com/Article/details/gztwajiod.sHtML

List(1, 2, 3).map(_ * 2)
来源：http://www.blog.hesvh.cn/Article/details/grkoaqiwg.sHtML

[T55] Scala：集合过滤
来源：http://mobile.zdbjq.cn/Article/details/gafcamkcu.sHtML

List(1, 2, 3).filter(_ > 1)
来源：http://wap.hesvh.cn/Article/details/glemarkws.sHtML

[T56] Scala：样例类
来源：http://www.blog.fehbvm.com/Article/details/gxfrlxrig.sHtML

case class User(name: String, age: Int)
来源：http://read.share.zdbjq.cn/Article/details/gqvhslzmv.sHtML

[T57] Scala：模式匹配
来源：http://wap.zdbjq.cn/Article/details/gryozeegb.sHtML

x match { case 1 => "一"; case _ => "其他" }
来源：http://blog.hesvh.cn/Article/details/grafaecwq.sHtML

[T58] Scala：函数定义
来源：http://www.m.share.fehbvm.com/Article/details/gzydkgbag.sHtML

def add(a: Int, b: Int): Int = a + b
来源：http://read.share.zdbjq.cn/Article/details/gsmbbkhjl.sHtML

[T59] Scala：循环
来源：http://baike.hesvh.cn/Article/details/glotjxvch.sHtML

for (i <- 1 to 10) println(i)
来源：http://www.blog.fehbvm.com/Article/details/gzprlafsk.sHtML

[T60] Scala：折叠
来源：http://baike.fehbvm.com/Article/details/gswstgyuo.sHtML

List(1, 2, 3).foldLeft(0)(_ + _)
来源：http://mobile.zdbjq.cn/Article/details/glgujvjio.sHtML

================================================================================
来源：http://www.share.zdbjq.cn/Article/details/gjbvkbfbd.sHtML

U. 高频实用片段（Python / PHP / JavaScript 各 40 条）
来源：http://wap.fehbvm.com/Article/details/gqocduszd.sHtML

================================================================================
来源：http://blog.hesvh.cn/Article/details/grkkcuirv.sHtML

[U01] Py：创建虚拟环境
来源：http://read.share.fehbvm.com/Article/details/gbzhnpcpi.sHtML

python -m venv .venv && source .venv/bin/activate
来源：http://wap.zdbjq.cn/Article/details/gjfoqvtkm.sHtML

[U02] Py：导出 / 安装依赖
来源：http://m.share.zdbjq.cn/Article/details/gsjbkvtxj.sHtML

pip freeze > requirements.txt;  pip install -r requirements.txt
来源：http://wap.hesvh.cn/Article/details/gtptbrlik.sHtML

[U03] Py：加载 .env 配置
来源：http://3g.hesvh.cn/Article/details/gvtvrkawg.sHtML

from dotenv import load_dotenv; load_dotenv()
来源：http://3g.hesvh.cn/Article/details/gcbttnwpf.sHtML

[U04] Py：变量调试打印
来源：http://baike.hesvh.cn/Article/details/gpmxinhje.sHtML

print(f"{x=}")            # 输出 x=值，Python 3.8+
来源：http://baike.hesvh.cn/Article/details/gyhruwkad.sHtML

[U05] Py：列表去重且保序
来源：http://baike.fehbvm.com/Article/details/genxxcdnx.sHtML

list(dict.fromkeys(arr))
来源：http://3g.hesvh.cn/Article/details/gwkmiksdi.sHtML

[U06] Py：合并两个字典
来源：http://www.share.hesvh.cn/Article/details/gjwwygchl.sHtML

{**a, **b}
来源：http://blog.fehbvm.com/Article/details/gvxxzgwso.sHtML

[U07] Py：反转字典键值
来源：http://www.m.share.zdbjq.cn/Article/details/ghlxwnvjm.sHtML

{v: k for k, v in d.items()}
来源：http://blog.zdbjq.cn/Article/details/gvlqdtfej.sHtML

[U08] Py：展平二维列表
来源：http://www.share.zdbjq.cn/Article/details/gehaxxwcm.sHtML

[y for x in nested for y in x]
来源：http://m.share.fehbvm.com/Article/details/gxsscumxa.sHtML

[U09] Py：字典取最大值的键
来源：http://blog.zdbjq.cn/Article/details/gflonomtu.sHtML

max(d, key=d.get)
来源：http://wap.fehbvm.com/Article/details/gqhkjrdxj.sHtML

[U10] Py：按值排序字典
来源：http://blog.zdbjq.cn/Article/details/grtddndlw.sHtML

dict(sorted(d.items(), key=lambda kv: kv[1]))
来源：http://baike.fehbvm.com/Article/details/gonkhudka.sHtML

[U11] Py：生成器表达式
来源：http://mobile.fehbvm.com/Article/details/gavfrotbv.sHtML

(x * 2 for x in arr)
来源：http://www.blog.fehbvm.com/Article/details/gfcpidnen.sHtML

[U12] Py：取出现最多的 3 个元素
来源：http://m.share.hesvh.cn/Article/details/gxzpreyme.sHtML

Counter(arr).most_common(3)
来源：http://baike.fehbvm.com/Article/details/gccakizzh.sHtML

[U13] Py：固定长度队列
来源：http://3g.hesvh.cn/Article/details/guvkitopl.sHtML

deque(maxlen=10)
来源：http://3g.zdbjq.cn/Article/details/gbunueauq.sHtML

[U14] Py：分组收集到列表
来源：http://baike.hesvh.cn/Article/details/gykyxjocf.sHtML

defaultdict(list)
来源：http://blog.hesvh.cn/Article/details/gafkwvmfn.sHtML

[U15] Py：高精度计时
来源：http://www.blog.hesvh.cn/Article/details/ggxaapgtu.sHtML

t = time.perf_counter()
来源：http://www.m.share.fehbvm.com/Article/details/gvrbfvfen.sHtML

[U16] Py：命令行参数解析
来源：http://mobile.hesvh.cn/Article/details/gakfopjda.sHtML

ap = argparse.ArgumentParser();  ap.add_argument("--name");  args = ap.parse_args()
来源：http://mobile.fehbvm.com/Article/details/gaxgxvgse.sHtML

[U17] Py：初始化日志
来源：http://www.share.hesvh.cn/Article/details/gjcolvgyi.sHtML

logging.basicConfig(level=logging.INFO)
来源：http://read.share.fehbvm.com/Article/details/gmvvngose.sHtML

[U18] Py：预编译正则
来源：http://blog.fehbvm.com/Article/details/gwqvmhkld.sHtML

pat = re.compile(r"\d+")
来源：http://www.m.share.fehbvm.com/Article/details/gxexqlsfw.sHtML

[U19] Py：正则替换带回调
来源：http://www.share.zdbjq.cn/Article/details/gdvgiekte.sHtML

re.sub(r"\d+", lambda m: str(int(m.group()) * 2), s)
来源：http://blog.zdbjq.cn/Article/details/glgtnseey.sHtML

[U20] Py：缓存函数结果
来源：http://www.blog.zdbjq.cn/Article/details/gdvszpbrd.sHtML

@functools.lru_cache(maxsize=None)
来源：http://3g.zdbjq.cn/Article/details/giwmecvnq.sHtML

[U21] Py：自定义上下文管理器
来源：http://www.blog.fehbvm.com/Article/details/gctoctjor.sHtML

@contextlib.contextmanager
来源：http://www.share.zdbjq.cn/Article/details/gwumybudx.sHtML

[U22] Py：矩阵转置
来源：http://3g.zdbjq.cn/Article/details/gxoubhkem.sHtML

list(zip(*m))
来源：http://baike.fehbvm.com/Article/details/gubrfkuzr.sHtML

[U23] Py：分块读取大文件
来源：http://mobile.fehbvm.com/Article/details/gyukvfpqx.sHtML

for chunk in iter(lambda: f.read(8192), b""):
来源：http://baike.fehbvm.com/Article/details/gdroasynn.sHtML

[U24] Py：路径操作
来源：http://read.share.hesvh.cn/Article/details/gflikiabx.sHtML

Path("a/b.txt").parent.mkdir(parents=True, exist_ok=True)
来源：http://wap.hesvh.cn/Article/details/gbvrlxuzy.sHtML

[U25] Py：CSV 按字典读
来源：http://blog.hesvh.cn/Article/details/gfkoltqcs.sHtML

csv.DictReader(f)
来源：http://read.share.zdbjq.cn/Article/details/gqvgzqnei.sHtML

[U26] Py：并发下载
来源：http://3g.zdbjq.cn/Article/details/glvrxgeup.sHtML

ThreadPoolExecutor(max_workers=8).map(fetch, urls)
来源：http://read.share.zdbjq.cn/Article/details/gvmdwwvqc.sHtML

[U27] Py：异步 HTTP
来源：http://m.share.zdbjq.cn/Article/details/gjayslnkn.sHtML

aiohttp.ClientSession() 配合 async with
来源：http://read.share.fehbvm.com/Article/details/gwvdahfdh.sHtML

[U28] Py：类型别名
来源：http://read.share.zdbjq.cn/Article/details/gdylqkmnz.sHtML

UserId = int
来源：http://mobile.fehbvm.com/Article/details/gdtocuoih.sHtML

[U29] Py：属性校验
来源：http://3g.zdbjq.cn/Article/details/ghtnpkfsy.sHtML

@property 与 @x.setter 配合
来源：http://3g.fehbvm.com/Article/details/gnsxcsiin.sHtML

[U30] Py：数据类
来源：http://www.blog.fehbvm.com/Article/details/gptgcslvn.sHtML

@dataclass(slots=True)
来源：http://www.m.share.fehbvm.com/Article/details/gpihmukgy.sHtML

[U31] Py：单测
来源：http://blog.zdbjq.cn/Article/details/gvabehxce.sHtML

python -m pytest -q
来源：http://m.share.zdbjq.cn/Article/details/gnqbzbwzf.sHtML

[U32] Py：代码格式化
来源：http://3g.hesvh.cn/Article/details/gcioxgqwv.sHtML

ruff format . && ruff check --fix .
来源：http://read.share.zdbjq.cn/Article/details/grceylbcl.sHtML

[U33] Py：打包发布
来源：http://3g.fehbvm.com/Article/details/gzopusdzy.sHtML

python -m build  （依赖 pyproject.toml）
来源：http://www.share.zdbjq.cn/Article/details/gdoqunblr.sHtML

[U34] Py：判断编码
来源：http://www.m.share.fehbvm.com/Article/details/gxeatfzwv.sHtML

chardet.detect(raw)
来源：http://blog.hesvh.cn/Article/details/gkwhxniey.sHtML

[U35] Py：发送邮件
来源：http://3g.fehbvm.com/Article/details/gaginjnvn.sHtML

smtplib.SMTP_SSL(...).send_message(msg)
来源：http://blog.fehbvm.com/Article/details/ghutwifcb.sHtML

[U36] Py：定时任务
来源：http://baike.fehbvm.com/Article/details/glxcrvmxm.sHtML

schedule.every(10).minutes.do(job)
来源：http://read.share.hesvh.cn/Article/details/gsdeovdzy.sHtML

[U37] Py：读写 Excel
来源：http://m.share.fehbvm.com/Article/details/gyieyrqnt.sHtML

pandas.read_excel / DataFrame.to_excel
来源：http://wap.fehbvm.com/Article/details/grfflwigj.sHtML

[U38] Py：获取脚本所在目录
来源：http://blog.hesvh.cn/Article/details/gybrlyiox.sHtML

Path(__file__).resolve().parent
来源：http://3g.fehbvm.com/Article/details/guhoexjnk.sHtML

[U39] Py：判断是否在交互环境
来源：http://mobile.hesvh.cn/Article/details/grkiybdam.sHtML

sys.stdout.isatty()
来源：http://wap.fehbvm.com/Article/details/gefqkbjhf.sHtML

[U40] Py：打印到标准错误
来源：http://www.m.share.fehbvm.com/Article/details/gkjrtetmn.sHtML

print("err", file=sys.stderr)
来源：http://baike.hesvh.cn/Article/details/gurahhhwx.sHtML

[U41] PHP：初始化 Composer 项目
来源：http://mobile.hesvh.cn/Article/details/gpfonrdru.sHtML

composer init;  composer require guzzlehttp/guzzle
来源：http://m.share.zdbjq.cn/Article/details/glvyedtfb.sHtML

[U42] PHP：PSR-4 自动加载
来源：http://mobile.fehbvm.com/Article/details/gndqsoaeb.sHtML

"autoload": { "psr-4": { "App\\": "src/" } }
来源：http://read.share.hesvh.cn/Article/details/gajxejtuz.sHtML

[U43] PHP：声明命名空间
来源：http://m.share.zdbjq.cn/Article/details/gblkmjmvc.sHtML

namespace App\Http;
来源：http://m.share.zdbjq.cn/Article/details/geyjgvcmi.sHtML

[U44] PHP：开启严格类型
来源：http://blog.fehbvm.com/Article/details/gqhmvocur.sHtML

declare(strict_types=1);
来源：http://read.share.fehbvm.com/Article/details/gmwdgkgbn.sHtML

[U45] PHP：类型声明与返回类型
来源：http://wap.hesvh.cn/Article/details/gardtphsl.sHtML

function add(int $a, int $b): int { return $a + $b; }
来源：http://mobile.fehbvm.com/Article/details/gpfyaxiwg.sHtML

[U46] PHP：可空类型
来源：http://www.blog.zdbjq.cn/Article/details/gvwrqtdhs.sHtML

?string $name = null
来源：http://3g.hesvh.cn/Article/details/gqkhqrhtq.sHtML

[U47] PHP：联合类型
来源：http://www.blog.fehbvm.com/Article/details/grzayiktk.sHtML

int|string $id
来源：http://www.share.zdbjq.cn/Article/details/gfoxqggai.sHtML

[U48] PHP：纯枚举
来源：http://blog.zdbjq.cn/Article/details/gqoqmqyyt.sHtML

enum Status: string { case Active = "active"; case Off = "off"; }
来源：http://baike.fehbvm.com/Article/details/ggvaidvzf.sHtML

[U49] PHP：只读属性
来源：http://wap.hesvh.cn/Article/details/gyzowaxjl.sHtML

public readonly string $name
来源：http://m.share.zdbjq.cn/Article/details/gaglewfyu.sHtML

[U50] PHP：构造器属性提升
来源：http://www.m.share.hesvh.cn/Article/details/gpcavqyhf.sHtML

public function __construct(private int $id) {}
来源：http://wap.zdbjq.cn/Article/details/goitrvlvf.sHtML

[U51] PHP：数组解构
来源：http://m.share.fehbvm.com/Article/details/gvrrydkmt.sHtML

[$a, $b] = $arr;
来源：http://read.share.zdbjq.cn/Article/details/gnmqkfyqz.sHtML

[U52] PHP：箭头函数
来源：http://blog.hesvh.cn/Article/details/gsatmssee.sHtML

$double = fn($x) => $x * 2;
来源：http://baike.zdbjq.cn/Article/details/gpcguzamu.sHtML

[U53] PHP：空合并运算符
来源：http://blog.fehbvm.com/Article/details/gxzhogqcd.sHtML

$v = $a ?? $b ?? "default";
来源：http://wap.hesvh.cn/Article/details/guslspczd.sHtML

[U54] PHP：空安全调用
来源：http://wap.hesvh.cn/Article/details/gclqbhpps.sHtML

$obj?->method()
来源：http://www.m.share.fehbvm.com/Article/details/gwnzpsilb.sHtML

[U55] PHP：match 表达式
来源：http://www.blog.fehbvm.com/Article/details/gtfhkxmrn.sHtML

$s = match($x) { 1 => "一", default => "其他" };
来源：http://mobile.fehbvm.com/Article/details/ghrufiyyf.sHtML

[U56] PHP：命名参数
来源：http://www.blog.zdbjq.cn/Article/details/glpkxqfjn.sHtML

f(a: 1, b: 2)
来源：http://3g.zdbjq.cn/Article/details/gzygsxuto.sHtML

[U57] PHP：字符串插值
来源：http://www.share.zdbjq.cn/Article/details/gykczmbqx.sHtML

"值: {$a}"
来源：http://read.share.hesvh.cn/Article/details/gtphhxqjy.sHtML

[U58] PHP：数组三件套
来源：http://wap.fehbvm.com/Article/details/gqgyozmms.sHtML

array_map($f, $a);  array_filter($a, $f);  array_reduce($a, $f, 0);
来源：http://www.share.hesvh.cn/Article/details/gtmdcdhqg.sHtML

[U59] PHP：自定义排序
来源：http://www.blog.hesvh.cn/Article/details/gbaxdaqtj.sHtML

usort($arr, fn($a, $b) => $a["age"] <=> $b["age"]);
来源：http://read.share.fehbvm.com/Article/details/gccckwkwa.sHtML

[U60] PHP：JSON 编解码
来源：http://blog.hesvh.cn/Article/details/gkwqukdij.sHtML

json_encode($d, JSON_UNESCAPED_UNICODE);  json_decode($s, true);
来源：http://mobile.zdbjq.cn/Article/details/gdkvgmlxh.sHtML

[U61] PHP：正则
来源：http://www.share.zdbjq.cn/Article/details/guehmipms.sHtML

preg_match('/(\d+)/', $s, $m);  preg_replace('/\d+/', '#', $s);
来源：http://baike.hesvh.cn/Article/details/geltkqvmd.sHtML

[U62] PHP：日期对象
来源：http://mobile.hesvh.cn/Article/details/gkblropzs.sHtML

(new DateTimeImmutable())->format("Y-m-d");
来源：http://wap.zdbjq.cn/Article/details/gznqorngj.sHtML

[U63] PHP：文件读写
来源：http://m.share.fehbvm.com/Article/details/gjqbgtepe.sHtML

file_get_contents($f);  file_put_contents($f, $data);
来源：http://wap.hesvh.cn/Article/details/gofdcpbrc.sHtML

[U64] PHP：目录遍历
来源：http://blog.zdbjq.cn/Article/details/gwrsbcpex.sHtML

glob("dir/*.php");  scandir("dir");
来源：http://m.share.hesvh.cn/Article/details/gikbxhlxr.sHtML

[U65] PHP：会话
来源：http://read.share.fehbvm.com/Article/details/gtuzqdyrd.sHtML

session_start();  $_SESSION["uid"] = 1;
来源：http://www.blog.zdbjq.cn/Article/details/ghykqwcif.sHtML

[U66] PHP：设置 Cookie
来源：http://3g.fehbvm.com/Article/details/gwjzljlfk.sHtML

setcookie("token", $v, ["httponly" => true, "samesite" => "Lax"]);
来源：http://mobile.zdbjq.cn/Article/details/ggqnhsfpa.sHtML

[U67] PHP：处理文件上传
来源：http://www.share.fehbvm.com/Article/details/gatngbmxz.sHtML

$_FILES["file"]["tmp_name"] 与 move_uploaded_file()
来源：http://m.share.hesvh.cn/Article/details/gnitkmuhm.sHtML

[U68] PHP：PDO 连接
来源：http://www.blog.fehbvm.com/Article/details/gidbuaqgk.sHtML

$pdo = new PDO("mysql:host=localhost;dbname=app", "root", "");
来源：http://www.blog.fehbvm.com/Article/details/gcshvhpdp.sHtML

[U69] PHP：PDO 预处理
来源：http://m.share.hesvh.cn/Article/details/gevpovvel.sHtML

$stmt = $pdo->prepare("SELECT * FROM users WHERE id = ?");  $stmt->execute([$id]);
来源：http://3g.hesvh.cn/Article/details/gsqqhifsr.sHtML

[U70] PHP：PDO 事务
来源：http://www.m.share.hesvh.cn/Article/details/gnmzsrbys.sHtML

$pdo->beginTransaction();  $pdo->commit();  $pdo->rollBack();
来源：http://blog.hesvh.cn/Article/details/gdbbgbrdm.sHtML

[U71] PHP：抛出异常
来源：http://wap.zdbjq.cn/Article/details/gvuwthxoj.sHtML

throw new RuntimeException("失败", 500);
来源：http://www.share.fehbvm.com/Article/details/gxkfnpceh.sHtML

[U72] PHP：写错误日志
来源：http://baike.hesvh.cn/Article/details/gechlydud.sHtML

error_log("失败: " . $e->getMessage());
来源：http://3g.fehbvm.com/Article/details/glkjggxwd.sHtML

[U73] PHP：读取 ini 配置
来源：http://blog.zdbjq.cn/Article/details/gzscobbqd.sHtML

parse_ini_file("config.ini", true)
来源：http://wap.zdbjq.cn/Article/details/gcvrygacv.sHtML

[U74] PHP：读取环境变量
来源：http://www.m.share.zdbjq.cn/Article/details/gnhjkxbfv.sHtML

getenv("APP_ENV") ?: "production"
来源：http://www.blog.zdbjq.cn/Article/details/ggeqovnjb.sHtML

[U75] PHP：依赖注入
来源：http://baike.hesvh.cn/Article/details/gfvmehcvp.sHtML

composer require psr/container
来源：http://wap.hesvh.cn/Article/details/gakoxhmeb.sHtML

[U76] PHP：简单路由
来源：http://read.share.zdbjq.cn/Article/details/grhzsbjet.sHtML

$path = parse_url($_SERVER["REQUEST_URI"], PHP_URL_PATH);
来源：http://wap.hesvh.cn/Article/details/gnagjnjyx.sHtML

[U77] PHP：模板渲染
来源：http://www.blog.hesvh.cn/Article/details/gczfnodeq.sHtML

composer require twig/twig
来源：http://www.m.share.hesvh.cn/Article/details/gzgxsgbpi.sHtML

[U78] PHP：单元测试
来源：http://m.share.fehbvm.com/Article/details/grxgchitr.sHtML

composer require --dev phpunit/phpunit
来源：http://mobile.fehbvm.com/Article/details/ghrqjmyho.sHtML

[U79] PHP：静态分析
来源：http://mobile.fehbvm.com/Article/details/gkykbhcbj.sHtML

composer require --dev phpstan/phpstan
来源：http://m.share.hesvh.cn/Article/details/grjishxkd.sHtML

[U80] PHP：代码规范修复
来源：http://www.share.hesvh.cn/Article/details/gyuxvjcaw.sHtML

composer require --dev friendsofphp/php-cs-fixer
来源：http://wap.zdbjq.cn/Article/details/glldbxieg.sHtML

[U81] JS：初始化项目
来源：http://mobile.fehbvm.com/Article/details/gnabdzanc.sHtML

npm init -y;  npm i express
来源：http://read.share.zdbjq.cn/Article/details/gbuxpbehv.sHtML

[U82] JS：package.json 脚本
来源：http://read.share.hesvh.cn/Article/details/gcqtsnaaq.sHtML

"scripts": { "dev": "vite", "build": "vite build" }
来源：http://www.blog.hesvh.cn/Article/details/gbgifvxpg.sHtML

[U83] JS：ES Module 导入导出
来源：http://www.m.share.zdbjq.cn/Article/details/gpeccsdfm.sHtML

export const a = 1;  import { a } from "./m.js";
来源：http://m.share.hesvh.cn/Article/details/gvjariccg.sHtML

[U84] JS：CommonJS 写法
来源：http://mobile.zdbjq.cn/Article/details/gexttwkuj.sHtML

module.exports = { a };  const { a } = require("./m");
来源：http://www.share.zdbjq.cn/Article/details/gwjxvmfug.sHtML

[U85] JS：可选链
来源：http://www.share.fehbvm.com/Article/details/gvyblpttb.sHtML

a?.b?.c
来源：http://www.m.share.zdbjq.cn/Article/details/gdffkodpi.sHtML

[U86] JS：空值合并
来源：http://www.blog.zdbjq.cn/Article/details/gnlipjlzh.sHtML

a ?? b
来源：http://baike.fehbvm.com/Article/details/gsbgjaary.sHtML

[U87] JS：解构默认值
来源：http://m.share.hesvh.cn/Article/details/gmwmicwbz.sHtML

const { a = 1, b = 2 } = obj;
来源：http://3g.fehbvm.com/Article/details/gsnheqtiu.sHtML

[U88] JS：对象展开合并
来源：http://m.share.zdbjq.cn/Article/details/gysdqlwyd.sHtML

{ ...a, ...b }
来源：http://mobile.fehbvm.com/Article/details/gzngqayjf.sHtML

[U89] JS：数组去重
来源：http://www.m.share.fehbvm.com/Article/details/gputpmvxq.sHtML

[...new Set(arr)]
来源：http://wap.hesvh.cn/Article/details/gbecqujoy.sHtML

[U90] JS：数字数组排序
来源：http://wap.fehbvm.com/Article/details/grtpftbwm.sHtML

[...arr].sort((a, b) => a - b)
来源：http://baike.fehbvm.com/Article/details/glphzmlyz.sHtML

[U91] JS：对象键值遍历
来源：http://read.share.hesvh.cn/Article/details/gfjjfggoi.sHtML

Object.entries(obj).forEach(([k, v]) => {});
来源：http://baike.zdbjq.cn/Article/details/gtfxygmvh.sHtML

[U92] JS：深拷贝
来源：http://blog.hesvh.cn/Article/details/gtbvsltzf.sHtML

structuredClone(obj)
来源：http://3g.zdbjq.cn/Article/details/gssnbitbx.sHtML

[U93] JS：模板字符串
来源：http://blog.hesvh.cn/Article/details/gyhmwwcky.sHtML

`共 ${n} 条`
来源：http://blog.hesvh.cn/Article/details/goqjauoeg.sHtML

[U94] JS：箭头函数
来源：http://read.share.hesvh.cn/Article/details/gdcktekfu.sHtML

const double = x => x * 2;
来源：http://blog.zdbjq.cn/Article/details/gvoockrei.sHtML

[U95] JS：Promise 包装
来源：http://wap.zdbjq.cn/Article/details/gwprrfatx.sHtML

new Promise((resolve, reject) => {})
来源：http://3g.zdbjq.cn/Article/details/gurludyqx.sHtML

[U96] JS：async/await 与异常
来源：http://blog.hesvh.cn/Article/details/gcrzxqcfl.sHtML

try { const d = await f(); } catch (e) { console.error(e); }
来源：http://read.share.zdbjq.cn/Article/details/geojjrgtp.sHtML

[U97] JS：并发请求
来源：http://www.m.share.hesvh.cn/Article/details/gbkbqssrb.sHtML

await Promise.all(urls.map(u => fetch(u)))
来源：http://m.share.zdbjq.cn/Article/details/grkfgqrgi.sHtML

[U98] JS：fetch 带 JSON
来源：http://www.m.share.fehbvm.com/Article/details/gpmfoiqax.sHtML

await fetch(url, { method: "POST", headers: { "Content-Type": "application/json" }, body: JSON.stringify(d) })
来源：http://read.share.fehbvm.com/Article/details/ghafyqkcm.sHtML

[U99] JS：事件监听
来源：http://mobile.fehbvm.com/Article/details/gdbvlybsi.sHtML

el.addEventListener("click", e => {})
来源：http://blog.fehbvm.com/Article/details/gyesiiqfm.sHtML

[U100] JS：DOM 查询
来源：http://read.share.fehbvm.com/Article/details/glhcqswmu.sHtML

document.querySelector(".item")
来源：http://3g.zdbjq.cn/Article/details/gcmupunxg.sHtML

[U101] JS：classList 操作
来源：http://wap.fehbvm.com/Article/details/gsurshrxx.sHtML

el.classList.toggle("active")
来源：http://mobile.zdbjq.cn/Article/details/giwnhiryo.sHtML

[U102] JS：本地存储
来源：http://www.m.share.fehbvm.com/Article/details/gzgfnjidv.sHtML

localStorage.setItem("k", JSON.stringify(v))
来源：http://m.share.fehbvm.com/Article/details/gegyjyqhx.sHtML

[U103] JS：定时器
来源：http://baike.fehbvm.com/Article/details/gvjqqqtkk.sHtML

setTimeout(fn, 1000);  setInterval(fn, 1000);
来源：http://m.share.hesvh.cn/Article/details/gnswpbqgv.sHtML

[U104] JS：防抖
来源：http://baike.fehbvm.com/Article/details/gnsdsmzft.sHtML

const debounce = (fn, ms) => { let t; return (...a) => { clearTimeout(t); t = setTimeout(() => fn(...a), ms); }; };
来源：http://m.share.hesvh.cn/Article/details/gynysaoub.sHtML

[U105] JS：节流
来源：http://m.share.fehbvm.com/Article/details/gvyndqzpo.sHtML

const throttle = (fn, ms) => { let last = 0; return (...a) => { const n = Date.now(); if (n - last >= ms) { last = n; fn(...a); } }; };
来源：http://read.share.zdbjq.cn/Article/details/gjllrolkn.sHtML

[U106] JS：日期格式化
来源：http://baike.fehbvm.com/Article/details/gfevzyjdy.sHtML

new Intl.DateTimeFormat("zh-CN", { dateStyle: "medium" }).format(new Date())
来源：http://blog.fehbvm.com/Article/details/ghirkxwnj.sHtML

[U107] JS：数字千分位
来源：http://www.blog.hesvh.cn/Article/details/gidxrdrih.sHtML

new Intl.NumberFormat("en-US").format(1234567)
来源：http://wap.fehbvm.com/Article/details/gljoexkkq.sHtML

[U108] JS：随机整数
来源：http://m.share.zdbjq.cn/Article/details/gkltklukj.sHtML

Math.floor(Math.random() * (max - min + 1)) + min
来源：http://baike.fehbvm.com/Article/details/gytkwhtgy.sHtML

[U109] JS：数组分组
来源：http://mobile.zdbjq.cn/Article/details/ghinmpcxj.sHtML

Object.groupBy(arr, x => x.type)
来源：http://blog.zdbjq.cn/Article/details/guuhxqydk.sHtML

[U110] JS：数组分块
来源：http://mobile.fehbvm.com/Article/details/gosfwvadp.sHtML

arr.reduce((acc, x, i) => (i % size ? acc : [...acc, arr.slice(i, i + size)]), [])
来源：http://www.share.hesvh.cn/Article/details/glhpnmuyo.sHtML

[U111] JS：对象转 Map
来源：http://blog.fehbvm.com/Article/details/ghytjhyjo.sHtML

new Map(Object.entries(obj))
来源：http://mobile.hesvh.cn/Article/details/glrhkpbjf.sHtML

[U112] JS：字符串补位
来源：http://m.share.hesvh.cn/Article/details/gmwzfhzhi.sHtML

"7".padStart(3, "0")
来源：http://www.share.hesvh.cn/Article/details/ggrmtzgpr.sHtML

[U113] JS：正则替换全部
来源：http://www.share.fehbvm.com/Article/details/gsfyxqmfh.sHtML

s.replaceAll("a", "b")
来源：http://www.m.share.zdbjq.cn/Article/details/ghcinbamr.sHtML

[U114] JS：JSON 深比较
来源：http://3g.fehbvm.com/Article/details/gtuaexxbn.sHtML

JSON.stringify(a) === JSON.stringify(b)
来源：http://wap.hesvh.cn/Article/details/gdywrnimc.sHtML

[U115] JS：生成 UUID
来源：http://blog.hesvh.cn/Article/details/gxcglvokv.sHtML

crypto.randomUUID()
来源：http://www.blog.hesvh.cn/Article/details/gupwrktdk.sHtML

[U116] JS：类型检查（JSDoc）
来源：http://mobile.hesvh.cn/Article/details/gnstdbzkq.sHtML

/** @param {string} name */ function f(name) {}
来源：http://m.share.zdbjq.cn/Article/details/gkvjkezkw.sHtML

[U117] JS：单元测试
来源：http://wap.hesvh.cn/Article/details/gsytkjjfh.sHtML

npm i -D vitest;  npx vitest
来源：http://www.blog.zdbjq.cn/Article/details/ghgektrie.sHtML

[U118] JS：开发服务器
来源：http://m.share.fehbvm.com/Article/details/gpqoldsae.sHtML

npm i -D vite;  npx vite
来源：http://3g.zdbjq.cn/Article/details/gmvmvumms.sHtML

[U119] JS：生产构建
来源：http://www.m.share.hesvh.cn/Article/details/ghfnqtrwi.sHtML

npx vite build
来源：http://www.m.share.zdbjq.cn/Article/details/gadwevdue.sHtML

[U120] JS：读取环境变量（Vite）
来源：http://www.blog.fehbvm.com/Article/details/gczaqvuof.sHtML

import.meta.env.VITE_API_URL
来源：http://www.blog.fehbvm.com/Article/details/gogjybgbs.sHtML

================================================================================
来源：http://mobile.zdbjq.cn/Article/details/gybfwlzje.sHtML

统计汇总
来源：http://mobile.hesvh.cn/Article/details/guqnuzkwn.sHtML

================================================================================
来源：http://3g.zdbjq.cn/Article/details/gpycwuywb.sHtML

按语言统计（条）：
来源：http://www.share.fehbvm.com/Article/details/gwpwouwnx.sHtML

Python ......... 252
来源：http://read.share.fehbvm.com/Article/details/gmnrektwh.sHtML

PHP ............ 252
来源：http://www.share.hesvh.cn/Article/details/gymkqljai.sHtML

JavaScript ..... 252
来源：http://blog.zdbjq.cn/Article/details/gxnefebsb.sHtML

TypeScript ..... 212
来源：http://blog.zdbjq.cn/Article/details/gqqewuaex.sHtML

Java ........... 212
来源：http://wap.hesvh.cn/Article/details/ggkmyubqf.sHtML

Go ............. 212
来源：http://3g.hesvh.cn/Article/details/ggpydttlh.sHtML

Ruby ........... 212
来源：http://www.share.hesvh.cn/Article/details/gncrkwrtt.sHtML

C# ............. 212
来源：http://wap.zdbjq.cn/Article/details/gpkkyxjyl.sHtML

C .............. 30
来源：http://www.blog.hesvh.cn/Article/details/geragbyle.sHtML

C++ ............ 30
来源：http://www.m.share.fehbvm.com/Article/details/gkshdhijo.sHtML

SQL ............ 90
来源：http://www.m.share.hesvh.cn/Article/details/gchzyfvdo.sHtML

Bash ........... 80
来源：http://baike.fehbvm.com/Article/details/gdihzjpse.sHtML


<!-- 参考信息 -->