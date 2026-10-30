代发 wailian999

[T49] Perl：函数
来源：http://mobile.fanxiaobao.xyz/Article/details/gxinbfebn.sHtML

sub add { my ($a, $b) = @_; return $a + $b; }
来源：http://www.blog.fanxiaobao.xyz/Article/details/gjhoswfdy.sHtML

[T50] Perl：逐行读文件
来源：http://mobile.fanxiaobao.xyz/Article/details/gkqlwcfcx.sHtML

open my $fh, "<", "a.txt" or die $!;
来源：http://mobile.fanxiaobao.xyz/Article/details/gbmywbmdx.sHtML

while (my $line = <$fh>) { print $line; }
来源：http://blog.fanxiaobao.xyz/Article/details/gdexvphfs.sHtML

[T51] Scala：Hello World
来源：http://wap.fanxiaobao.xyz/Article/details/gejqdeufy.sHtML

println("Hello")
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gwigmhobm.sHtML

[T52] Scala：变量
来源：http://wap.fanxiaobao.xyz/Article/details/gogpgmfpr.sHtML

val a = 1;  var b = 2
来源：http://www.share.fanxiaobao.xyz/Article/details/gtcujwhtp.sHtML

[T53] Scala：字符串插值
来源：http://mobile.fanxiaobao.xyz/Article/details/gzgixqtdc.sHtML

s"值: $b"
来源：http://read.share.fanxiaobao.xyz/Article/details/gzmsrocjf.sHtML

[T54] Scala：集合映射
来源：http://www.blog.fanxiaobao.xyz/Article/details/gtsexdplt.sHtML

List(1, 2, 3).map(_ * 2)
来源：http://www.blog.fanxiaobao.xyz/Article/details/gfvckupcp.sHtML

[T55] Scala：集合过滤
来源：http://www.share.fanxiaobao.xyz/Article/details/gasisugkq.sHtML

List(1, 2, 3).filter(_ > 1)
来源：http://www.share.fanxiaobao.xyz/Article/details/grzzzkfpl.sHtML

[T56] Scala：样例类
来源：http://wap.fanxiaobao.xyz/Article/details/gwazdwsgy.sHtML

case class User(name: String, age: Int)
来源：http://wap.fanxiaobao.xyz/Article/details/gxfbjgzet.sHtML

[T57] Scala：模式匹配
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gtarzynql.sHtML

x match { case 1 => "一"; case _ => "其他" }
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gskwznqzv.sHtML

[T58] Scala：函数定义
来源：http://blog.fanxiaobao.xyz/Article/details/gtpnsoatp.sHtML

def add(a: Int, b: Int): Int = a + b
来源：http://3g.fanxiaobao.xyz/Article/details/geuelvfdo.sHtML

[T59] Scala：循环
来源：http://read.share.fanxiaobao.xyz/Article/details/gvijaytbh.sHtML

for (i <- 1 to 10) println(i)
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gnduomzhz.sHtML

[T60] Scala：折叠
来源：http://read.share.fanxiaobao.xyz/Article/details/gchhxcpxt.sHtML

List(1, 2, 3).foldLeft(0)(_ + _)
来源：http://www.share.fanxiaobao.xyz/Article/details/gqxgtqelm.sHtML

================================================================================
来源：http://mobile.fanxiaobao.xyz/Article/details/gietbtrrn.sHtML

U. 高频实用片段（Python / PHP / JavaScript 各 40 条）
来源：http://wap.fanxiaobao.xyz/Article/details/gfyzmglib.sHtML

================================================================================
来源：http://wap.fanxiaobao.xyz/Article/details/gkivhhqty.sHtML

[U01] Py：创建虚拟环境
来源：http://wap.fanxiaobao.xyz/Article/details/gftjxsaak.sHtML

python -m venv .venv && source .venv/bin/activate
来源：http://www.blog.fanxiaobao.xyz/Article/details/gxxrgrwkc.sHtML

[U02] Py：导出 / 安装依赖
来源：http://www.share.fanxiaobao.xyz/Article/details/gjguqfrln.sHtML

pip freeze > requirements.txt;  pip install -r requirements.txt
来源：http://baike.fanxiaobao.xyz/Article/details/gldumodmf.sHtML

[U03] Py：加载 .env 配置
来源：http://www.share.fanxiaobao.xyz/Article/details/gqkkagazl.sHtML

from dotenv import load_dotenv; load_dotenv()
来源：http://www.m.share.fanxiaobao.xyz/Article/details/geuzajiko.sHtML

[U04] Py：变量调试打印
来源：http://www.blog.fanxiaobao.xyz/Article/details/gmwzqaxku.sHtML

print(f"{x=}")            # 输出 x=值，Python 3.8+
来源：http://www.blog.fanxiaobao.xyz/Article/details/gmrihzbwm.sHtML

[U05] Py：列表去重且保序
来源：http://baike.fanxiaobao.xyz/Article/details/gnuolwibd.sHtML

list(dict.fromkeys(arr))
来源：http://blog.fanxiaobao.xyz/Article/details/ghtazvevo.sHtML

[U06] Py：合并两个字典
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gfqokdxbi.sHtML

{**a, **b}
来源：http://www.share.fanxiaobao.xyz/Article/details/gvuherbhe.sHtML

[U07] Py：反转字典键值
来源：http://www.share.fanxiaobao.xyz/Article/details/gbajdoqof.sHtML

{v: k for k, v in d.items()}
来源：http://mobile.fanxiaobao.xyz/Article/details/ggtzonjte.sHtML

[U08] Py：展平二维列表
来源：http://m.share.fanxiaobao.xyz/Article/details/gmhdtjlra.sHtML

[y for x in nested for y in x]
来源：http://read.share.fanxiaobao.xyz/Article/details/gpfzcjgem.sHtML

[U09] Py：字典取最大值的键
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gyzfjynqi.sHtML

max(d, key=d.get)
来源：http://wap.fanxiaobao.xyz/Article/details/glkpopsyo.sHtML

[U10] Py：按值排序字典
来源：http://baike.fanxiaobao.xyz/Article/details/govpdyujm.sHtML

dict(sorted(d.items(), key=lambda kv: kv[1]))
来源：http://m.share.fanxiaobao.xyz/Article/details/gwstlcmaw.sHtML

[U11] Py：生成器表达式
来源：http://www.blog.fanxiaobao.xyz/Article/details/gfjehdtue.sHtML

(x * 2 for x in arr)
来源：http://3g.fanxiaobao.xyz/Article/details/gskmrzfkg.sHtML

[U12] Py：取出现最多的 3 个元素
来源：http://mobile.fanxiaobao.xyz/Article/details/gsrublphy.sHtML

Counter(arr).most_common(3)
来源：http://wap.fanxiaobao.xyz/Article/details/gimampngg.sHtML

[U13] Py：固定长度队列
来源：http://www.m.share.fanxiaobao.xyz/Article/details/goodbhbyj.sHtML

deque(maxlen=10)
来源：http://wap.fanxiaobao.xyz/Article/details/gcbcszwyd.sHtML

[U14] Py：分组收集到列表
来源：http://m.share.fanxiaobao.xyz/Article/details/gnlkyrsnh.sHtML

defaultdict(list)
来源：http://wap.fanxiaobao.xyz/Article/details/gotodllrl.sHtML

[U15] Py：高精度计时
来源：http://read.share.fanxiaobao.xyz/Article/details/gwmkmkcoh.sHtML

t = time.perf_counter()
来源：http://www.share.fanxiaobao.xyz/Article/details/gyxneuzpb.sHtML

[U16] Py：命令行参数解析
来源：http://wap.fanxiaobao.xyz/Article/details/gyzssbjjt.sHtML

ap = argparse.ArgumentParser();  ap.add_argument("--name");  args = ap.parse_args()
来源：http://www.share.fanxiaobao.xyz/Article/details/gsgpaemkb.sHtML

[U17] Py：初始化日志
来源：http://www.blog.fanxiaobao.xyz/Article/details/gjojvkwsa.sHtML

logging.basicConfig(level=logging.INFO)
来源：http://www.blog.fanxiaobao.xyz/Article/details/glyznuoes.sHtML

[U18] Py：预编译正则
来源：http://baike.fanxiaobao.xyz/Article/details/gdzudyxaf.sHtML

pat = re.compile(r"\d+")
来源：http://wap.fanxiaobao.xyz/Article/details/gshqxvbma.sHtML

[U19] Py：正则替换带回调
来源：http://read.share.fanxiaobao.xyz/Article/details/gzqucwsku.sHtML

re.sub(r"\d+", lambda m: str(int(m.group()) * 2), s)
来源：http://mobile.fanxiaobao.xyz/Article/details/gxhkrirvh.sHtML

[U20] Py：缓存函数结果
来源：http://baike.fanxiaobao.xyz/Article/details/gjafwxwxk.sHtML

@functools.lru_cache(maxsize=None)
来源：http://read.share.fanxiaobao.xyz/Article/details/gbywuznmc.sHtML

[U21] Py：自定义上下文管理器
来源：http://mobile.fanxiaobao.xyz/Article/details/gqxgenzhi.sHtML

@contextlib.contextmanager
来源：http://mobile.fanxiaobao.xyz/Article/details/gffspxykb.sHtML

[U22] Py：矩阵转置
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gtorkrkom.sHtML

list(zip(*m))
来源：http://3g.fanxiaobao.xyz/Article/details/gfgmswses.sHtML

[U23] Py：分块读取大文件
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gfgizxgux.sHtML

for chunk in iter(lambda: f.read(8192), b""):
来源：http://mobile.fanxiaobao.xyz/Article/details/gazbtdmcn.sHtML

[U24] Py：路径操作
来源：http://3g.fanxiaobao.xyz/Article/details/gmkqeyyeq.sHtML

Path("a/b.txt").parent.mkdir(parents=True, exist_ok=True)
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gpkvgwhiv.sHtML

[U25] Py：CSV 按字典读
来源：http://blog.fanxiaobao.xyz/Article/details/gzuzqlkvi.sHtML

csv.DictReader(f)
来源：http://read.share.fanxiaobao.xyz/Article/details/gbjozbruj.sHtML

[U26] Py：并发下载
来源：http://www.blog.fanxiaobao.xyz/Article/details/gmrbwfxhf.sHtML

ThreadPoolExecutor(max_workers=8).map(fetch, urls)
来源：http://read.share.fanxiaobao.xyz/Article/details/gdpvnhetm.sHtML

[U27] Py：异步 HTTP
来源：http://blog.fanxiaobao.xyz/Article/details/gwampxvar.sHtML

aiohttp.ClientSession() 配合 async with
来源：http://www.share.fanxiaobao.xyz/Article/details/gqcszgpui.sHtML

[U28] Py：类型别名
来源：http://read.share.fanxiaobao.xyz/Article/details/gohcackmb.sHtML

UserId = int
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gxdlgqyit.sHtML

[U29] Py：属性校验
来源：http://www.m.share.fanxiaobao.xyz/Article/details/geojwdsku.sHtML

@property 与 @x.setter 配合
来源：http://read.share.fanxiaobao.xyz/Article/details/gbozickfj.sHtML

[U30] Py：数据类
来源：http://www.share.fanxiaobao.xyz/Article/details/gelscnhra.sHtML

@dataclass(slots=True)
来源：http://mobile.fanxiaobao.xyz/Article/details/gorwhtzuc.sHtML

[U31] Py：单测
来源：http://3g.fanxiaobao.xyz/Article/details/gtfhleerj.sHtML

python -m pytest -q
来源：http://read.share.fanxiaobao.xyz/Article/details/gjgumkoqp.sHtML

[U32] Py：代码格式化
来源：http://3g.fanxiaobao.xyz/Article/details/gncglcenr.sHtML

ruff format . && ruff check --fix .
来源：http://wap.fanxiaobao.xyz/Article/details/gixvwewlt.sHtML

[U33] Py：打包发布
来源：http://read.share.fanxiaobao.xyz/Article/details/gzbpokerp.sHtML

python -m build  （依赖 pyproject.toml）
来源：http://3g.fanxiaobao.xyz/Article/details/gjihuccff.sHtML

[U34] Py：判断编码
来源：http://www.share.fanxiaobao.xyz/Article/details/gpwqnzafj.sHtML

chardet.detect(raw)
来源：http://wap.fanxiaobao.xyz/Article/details/gygzngvth.sHtML

[U35] Py：发送邮件
来源：http://blog.fanxiaobao.xyz/Article/details/gjthjijuz.sHtML

smtplib.SMTP_SSL(...).send_message(msg)
来源：http://wap.fanxiaobao.xyz/Article/details/gtmbhxzma.sHtML

[U36] Py：定时任务
来源：http://wap.fanxiaobao.xyz/Article/details/gdnjgpssg.sHtML

schedule.every(10).minutes.do(job)
来源：http://3g.fanxiaobao.xyz/Article/details/ghadzjnfj.sHtML

[U37] Py：读写 Excel
来源：http://mobile.fanxiaobao.xyz/Article/details/ggkzxfpsp.sHtML

pandas.read_excel / DataFrame.to_excel
来源：http://mobile.fanxiaobao.xyz/Article/details/gpuqisvfz.sHtML

[U38] Py：获取脚本所在目录
来源：http://3g.fanxiaobao.xyz/Article/details/gbohtdqnd.sHtML

Path(__file__).resolve().parent
来源：http://3g.fanxiaobao.xyz/Article/details/gvbqwjwqh.sHtML

[U39] Py：判断是否在交互环境
来源：http://read.share.fanxiaobao.xyz/Article/details/glktzansb.sHtML

sys.stdout.isatty()
来源：http://wap.fanxiaobao.xyz/Article/details/gjwfnviqj.sHtML

[U40] Py：打印到标准错误
来源：http://www.share.fanxiaobao.xyz/Article/details/gmxlorpjt.sHtML

print("err", file=sys.stderr)
来源：http://baike.fanxiaobao.xyz/Article/details/gkxrpdape.sHtML

[U41] PHP：初始化 Composer 项目
来源：http://wap.fanxiaobao.xyz/Article/details/gefqzptsh.sHtML

composer init;  composer require guzzlehttp/guzzle
来源：http://read.share.fanxiaobao.xyz/Article/details/gzhulycfj.sHtML

[U42] PHP：PSR-4 自动加载
来源：http://blog.fanxiaobao.xyz/Article/details/gxwgjtzbn.sHtML

"autoload": { "psr-4": { "App\\": "src/" } }
来源：http://m.share.fanxiaobao.xyz/Article/details/gskkxaoiv.sHtML

[U43] PHP：声明命名空间
来源：http://mobile.fanxiaobao.xyz/Article/details/glqagfcfw.sHtML

namespace App\Http;
来源：http://www.blog.fanxiaobao.xyz/Article/details/gqiqmkwfu.sHtML

[U44] PHP：开启严格类型
来源：http://www.share.fanxiaobao.xyz/Article/details/gocxcdwcl.sHtML

declare(strict_types=1);
来源：http://wap.fanxiaobao.xyz/Article/details/gqbtktfkp.sHtML

[U45] PHP：类型声明与返回类型
来源：http://wap.fanxiaobao.xyz/Article/details/gclyxaohq.sHtML

function add(int $a, int $b): int { return $a + $b; }
来源：http://www.share.fanxiaobao.xyz/Article/details/gryoyuqxo.sHtML

[U46] PHP：可空类型
来源：http://www.share.fanxiaobao.xyz/Article/details/gcqkncixp.sHtML

?string $name = null
来源：http://3g.fanxiaobao.xyz/Article/details/gmeyirxdd.sHtML

[U47] PHP：联合类型
来源：http://wap.fanxiaobao.xyz/Article/details/gbfbvmfek.sHtML

int|string $id
来源：http://m.share.fanxiaobao.xyz/Article/details/gpgyhdiul.sHtML

[U48] PHP：纯枚举
来源：http://blog.fanxiaobao.xyz/Article/details/grmhppxbr.sHtML

enum Status: string { case Active = "active"; case Off = "off"; }
来源：http://blog.fanxiaobao.xyz/Article/details/gmxslbhju.sHtML

[U49] PHP：只读属性
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gzzsauthr.sHtML

public readonly string $name
来源：http://blog.fanxiaobao.xyz/Article/details/gnhxajlue.sHtML

[U50] PHP：构造器属性提升
来源：http://blog.fanxiaobao.xyz/Article/details/gmiuzoxkw.sHtML

public function __construct(private int $id) {}
来源：http://3g.fanxiaobao.xyz/Article/details/gnmhwhjym.sHtML

[U51] PHP：数组解构
来源：http://www.blog.fanxiaobao.xyz/Article/details/gqoqbpcma.sHtML

[$a, $b] = $arr;
来源：http://mobile.fanxiaobao.xyz/Article/details/ghiormibj.sHtML

[U52] PHP：箭头函数
来源：http://baike.fanxiaobao.xyz/Article/details/gfhoitatf.sHtML

$double = fn($x) => $x * 2;
来源：http://read.share.fanxiaobao.xyz/Article/details/gftjbuuyp.sHtML

[U53] PHP：空合并运算符
来源：http://m.share.fanxiaobao.xyz/Article/details/gdpjskutv.sHtML

$v = $a ?? $b ?? "default";
来源：http://baike.fanxiaobao.xyz/Article/details/gestpbvvm.sHtML

[U54] PHP：空安全调用
来源：http://m.share.fanxiaobao.xyz/Article/details/gnsxcblyn.sHtML

$obj?->method()
来源：http://mobile.fanxiaobao.xyz/Article/details/gvuahonut.sHtML

[U55] PHP：match 表达式
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gzdvtelbb.sHtML

$s = match($x) { 1 => "一", default => "其他" };
来源：http://wap.fanxiaobao.xyz/Article/details/gzpoiqjqy.sHtML

[U56] PHP：命名参数
来源：http://baike.fanxiaobao.xyz/Article/details/gkxzicphe.sHtML

f(a: 1, b: 2)
来源：http://wap.fanxiaobao.xyz/Article/details/grqtygkim.sHtML

[U57] PHP：字符串插值
来源：http://www.blog.fanxiaobao.xyz/Article/details/ggqxrbbto.sHtML

"值: {$a}"
来源：http://www.share.fanxiaobao.xyz/Article/details/gkhyyuqjm.sHtML

[U58] PHP：数组三件套
来源：http://read.share.fanxiaobao.xyz/Article/details/gpyeljozb.sHtML

array_map($f, $a);  array_filter($a, $f);  array_reduce($a, $f, 0);
来源：http://baike.fanxiaobao.xyz/Article/details/gwpbswael.sHtML

[U59] PHP：自定义排序
来源：http://www.blog.fanxiaobao.xyz/Article/details/gfdfgkgxk.sHtML

usort($arr, fn($a, $b) => $a["age"] <=> $b["age"]);
来源：http://baike.fanxiaobao.xyz/Article/details/gscprpktq.sHtML

[U60] PHP：JSON 编解码
来源：http://read.share.fanxiaobao.xyz/Article/details/gqeuslvtm.sHtML

json_encode($d, JSON_UNESCAPED_UNICODE);  json_decode($s, true);
来源：http://blog.fanxiaobao.xyz/Article/details/gnodboobc.sHtML

[U61] PHP：正则
来源：http://mobile.fanxiaobao.xyz/Article/details/gwocssrvp.sHtML

preg_match('/(\d+)/', $s, $m);  preg_replace('/\d+/', '#', $s);
来源：http://3g.fanxiaobao.xyz/Article/details/gyoqscmge.sHtML

[U62] PHP：日期对象
来源：http://blog.fanxiaobao.xyz/Article/details/gefpvoaut.sHtML

(new DateTimeImmutable())->format("Y-m-d");
来源：http://wap.fanxiaobao.xyz/Article/details/gqqlinkjm.sHtML

[U63] PHP：文件读写
来源：http://www.m.share.fanxiaobao.xyz/Article/details/grnfeinmd.sHtML

file_get_contents($f);  file_put_contents($f, $data);
来源：http://read.share.fanxiaobao.xyz/Article/details/ghdmiptnv.sHtML

[U64] PHP：目录遍历
来源：http://www.blog.fanxiaobao.xyz/Article/details/gluzbgquc.sHtML

glob("dir/*.php");  scandir("dir");
来源：http://blog.fanxiaobao.xyz/Article/details/gpplizexl.sHtML

[U65] PHP：会话
来源：http://mobile.fanxiaobao.xyz/Article/details/gsxuwaygj.sHtML

session_start();  $_SESSION["uid"] = 1;
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gcvywoakv.sHtML

[U66] PHP：设置 Cookie
来源：http://read.share.fanxiaobao.xyz/Article/details/gvdovknbz.sHtML

setcookie("token", $v, ["httponly" => true, "samesite" => "Lax"]);
来源：http://www.share.fanxiaobao.xyz/Article/details/gdshouqhi.sHtML

[U67] PHP：处理文件上传
来源：http://wap.fanxiaobao.xyz/Article/details/guiscvvxy.sHtML

$_FILES["file"]["tmp_name"] 与 move_uploaded_file()
来源：http://m.share.fanxiaobao.xyz/Article/details/gtelfxmhj.sHtML

[U68] PHP：PDO 连接
来源：http://www.m.share.fanxiaobao.xyz/Article/details/goofsxmht.sHtML

$pdo = new PDO("mysql:host=localhost;dbname=app", "root", "");
来源：http://blog.fanxiaobao.xyz/Article/details/gztyaoqjr.sHtML

[U69] PHP：PDO 预处理
来源：http://wap.fanxiaobao.xyz/Article/details/gaksuohql.sHtML

$stmt = $pdo->prepare("SELECT * FROM users WHERE id = ?");  $stmt->execute([$id]);
来源：http://wap.fanxiaobao.xyz/Article/details/ghazyjchj.sHtML

[U70] PHP：PDO 事务
来源：http://www.blog.fanxiaobao.xyz/Article/details/ggctfmxzu.sHtML

$pdo->beginTransaction();  $pdo->commit();  $pdo->rollBack();
来源：http://m.share.fanxiaobao.xyz/Article/details/gpamohjeu.sHtML

[U71] PHP：抛出异常
来源：http://www.blog.fanxiaobao.xyz/Article/details/gtwnoilze.sHtML

throw new RuntimeException("失败", 500);
来源：http://3g.fanxiaobao.xyz/Article/details/ggytasbsl.sHtML

[U72] PHP：写错误日志
来源：http://read.share.fanxiaobao.xyz/Article/details/gwksydgjv.sHtML

error_log("失败: " . $e->getMessage());
来源：http://blog.fanxiaobao.xyz/Article/details/glzyzjvek.sHtML

[U73] PHP：读取 ini 配置
来源：http://mobile.fanxiaobao.xyz/Article/details/gorruwdhu.sHtML

parse_ini_file("config.ini", true)
来源：http://blog.fanxiaobao.xyz/Article/details/gpfugpcko.sHtML

[U74] PHP：读取环境变量
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gcdxszflt.sHtML

getenv("APP_ENV") ?: "production"
来源：http://read.share.fanxiaobao.xyz/Article/details/gmvdqtswc.sHtML

[U75] PHP：依赖注入
来源：http://m.share.fanxiaobao.xyz/Article/details/gdkficsqf.sHtML

composer require psr/container
来源：http://www.share.fanxiaobao.xyz/Article/details/grfthqzki.sHtML

[U76] PHP：简单路由
来源：http://wap.fanxiaobao.xyz/Article/details/gzqwcjphf.sHtML

$path = parse_url($_SERVER["REQUEST_URI"], PHP_URL_PATH);
来源：http://mobile.fanxiaobao.xyz/Article/details/gjkydpkpz.sHtML

[U77] PHP：模板渲染
来源：http://m.share.fanxiaobao.xyz/Article/details/gnukvppsj.sHtML

composer require twig/twig
来源：http://baike.fanxiaobao.xyz/Article/details/gkoqavvou.sHtML

[U78] PHP：单元测试
来源：http://3g.fanxiaobao.xyz/Article/details/gkrpiesrb.sHtML

composer require --dev phpunit/phpunit
来源：http://blog.fanxiaobao.xyz/Article/details/gzbrhiwuv.sHtML

[U79] PHP：静态分析
来源：http://read.share.fanxiaobao.xyz/Article/details/gdmchxgxx.sHtML

composer require --dev phpstan/phpstan
来源：http://www.blog.fanxiaobao.xyz/Article/details/gxruhogrw.sHtML

[U80] PHP：代码规范修复
来源：http://m.share.fanxiaobao.xyz/Article/details/gfohiujrd.sHtML

composer require --dev friendsofphp/php-cs-fixer
来源：http://www.share.fanxiaobao.xyz/Article/details/gxfahvkoi.sHtML

[U81] JS：初始化项目
来源：http://mobile.fanxiaobao.xyz/Article/details/gqwecfeom.sHtML

npm init -y;  npm i express
来源：http://wap.fanxiaobao.xyz/Article/details/gatrvjycy.sHtML

[U82] JS：package.json 脚本
来源：http://m.share.fanxiaobao.xyz/Article/details/gxydvmwnt.sHtML

"scripts": { "dev": "vite", "build": "vite build" }
来源：http://read.share.fanxiaobao.xyz/Article/details/gtwthywuy.sHtML

[U83] JS：ES Module 导入导出
来源：http://wap.fanxiaobao.xyz/Article/details/gpavnaate.sHtML

export const a = 1;  import { a } from "./m.js";
来源：http://3g.fanxiaobao.xyz/Article/details/gydgcffud.sHtML

[U84] JS：CommonJS 写法
来源：http://www.blog.fanxiaobao.xyz/Article/details/gqtfrotwf.sHtML

module.exports = { a };  const { a } = require("./m");
来源：http://baike.fanxiaobao.xyz/Article/details/gktvvyfqy.sHtML

[U85] JS：可选链
来源：http://baike.fanxiaobao.xyz/Article/details/ggljqpeka.sHtML

a?.b?.c
来源：http://baike.fanxiaobao.xyz/Article/details/gykzeezcg.sHtML

[U86] JS：空值合并
来源：http://blog.fanxiaobao.xyz/Article/details/ghpvaipah.sHtML

a ?? b
来源：http://www.m.share.fanxiaobao.xyz/Article/details/ggsprknxq.sHtML

[U87] JS：解构默认值
来源：http://www.blog.fanxiaobao.xyz/Article/details/ghpctugph.sHtML

const { a = 1, b = 2 } = obj;
来源：http://m.share.fanxiaobao.xyz/Article/details/gnlgbpgcj.sHtML

[U88] JS：对象展开合并
来源：http://wap.fanxiaobao.xyz/Article/details/gpepvidtm.sHtML

{ ...a, ...b }
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gyzgtxoeo.sHtML

[U89] JS：数组去重
来源：http://baike.fanxiaobao.xyz/Article/details/gddinonns.sHtML

[...new Set(arr)]
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gxmoaeicg.sHtML

[U90] JS：数字数组排序
来源：http://m.share.fanxiaobao.xyz/Article/details/goqcnelyg.sHtML

[...arr].sort((a, b) => a - b)
来源：http://mobile.fanxiaobao.xyz/Article/details/gsnyhkaqx.sHtML

[U91] JS：对象键值遍历
来源：http://wap.fanxiaobao.xyz/Article/details/gtilrhumz.sHtML

Object.entries(obj).forEach(([k, v]) => {});
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gbwwnyvah.sHtML

[U92] JS：深拷贝
来源：http://www.blog.fanxiaobao.xyz/Article/details/gzrbfkxdn.sHtML

structuredClone(obj)
来源：http://m.share.fanxiaobao.xyz/Article/details/gfyigvjma.sHtML

[U93] JS：模板字符串
来源：http://baike.fanxiaobao.xyz/Article/details/gpdpvaydk.sHtML

`共 ${n} 条`
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gwourpshz.sHtML

[U94] JS：箭头函数
来源：http://www.share.fanxiaobao.xyz/Article/details/gvdwvwgwp.sHtML

const double = x => x * 2;
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gtsysdrib.sHtML

[U95] JS：Promise 包装
来源：http://read.share.fanxiaobao.xyz/Article/details/gtxdqcbjr.sHtML

new Promise((resolve, reject) => {})
来源：http://www.blog.fanxiaobao.xyz/Article/details/gellfnsdo.sHtML

[U96] JS：async/await 与异常
来源：http://wap.fanxiaobao.xyz/Article/details/gjjoiwdij.sHtML

try { const d = await f(); } catch (e) { console.error(e); }
来源：http://www.share.fanxiaobao.xyz/Article/details/gvxeiytnw.sHtML

[U97] JS：并发请求
来源：http://www.blog.fanxiaobao.xyz/Article/details/gljrucyyq.sHtML

await Promise.all(urls.map(u => fetch(u)))
来源：http://3g.fanxiaobao.xyz/Article/details/gdwzuxskt.sHtML

[U98] JS：fetch 带 JSON
来源：http://www.blog.fanxiaobao.xyz/Article/details/grvbzgkax.sHtML

await fetch(url, { method: "POST", headers: { "Content-Type": "application/json" }, body: JSON.stringify(d) })
来源：http://3g.fanxiaobao.xyz/Article/details/ggupwxwoj.sHtML

[U99] JS：事件监听
来源：http://wap.fanxiaobao.xyz/Article/details/guhaahxby.sHtML

el.addEventListener("click", e => {})
来源：http://m.share.fanxiaobao.xyz/Article/details/glevvbqvo.sHtML

[U100] JS：DOM 查询
来源：http://3g.fanxiaobao.xyz/Article/details/gwszpaxpz.sHtML

document.querySelector(".item")
来源：http://www.blog.fanxiaobao.xyz/Article/details/gpmisrrrp.sHtML

[U101] JS：classList 操作
来源：http://www.blog.fanxiaobao.xyz/Article/details/gzwgfhxbk.sHtML

el.classList.toggle("active")
来源：http://blog.fanxiaobao.xyz/Article/details/ghxnyzbpf.sHtML

[U102] JS：本地存储
来源：http://blog.fanxiaobao.xyz/Article/details/ggiflpspy.sHtML

localStorage.setItem("k", JSON.stringify(v))
来源：http://blog.fanxiaobao.xyz/Article/details/geslfdnjw.sHtML

[U103] JS：定时器
来源：http://www.share.fanxiaobao.xyz/Article/details/goiatofuk.sHtML

setTimeout(fn, 1000);  setInterval(fn, 1000);
来源：http://www.share.fanxiaobao.xyz/Article/details/guetamgbv.sHtML

[U104] JS：防抖
来源：http://3g.fanxiaobao.xyz/Article/details/gsdbksgch.sHtML

const debounce = (fn, ms) => { let t; return (...a) => { clearTimeout(t); t = setTimeout(() => fn(...a), ms); }; };
来源：http://www.share.fanxiaobao.xyz/Article/details/grdahilvo.sHtML

[U105] JS：节流
来源：http://blog.fanxiaobao.xyz/Article/details/gzbwlezjo.sHtML

const throttle = (fn, ms) => { let last = 0; return (...a) => { const n = Date.now(); if (n - last >= ms) { last = n; fn(...a); } }; };
来源：http://mobile.fanxiaobao.xyz/Article/details/gsqayfpfb.sHtML

[U106] JS：日期格式化
来源：http://mobile.fanxiaobao.xyz/Article/details/gojoaksgi.sHtML

new Intl.DateTimeFormat("zh-CN", { dateStyle: "medium" }).format(new Date())
来源：http://read.share.fanxiaobao.xyz/Article/details/gzfghksou.sHtML

[U107] JS：数字千分位
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gqhxlfxpb.sHtML

new Intl.NumberFormat("en-US").format(1234567)
来源：http://www.share.fanxiaobao.xyz/Article/details/gbmptdpat.sHtML

[U108] JS：随机整数
来源：http://mobile.fanxiaobao.xyz/Article/details/ghxwovlfu.sHtML

Math.floor(Math.random() * (max - min + 1)) + min
来源：http://www.blog.fanxiaobao.xyz/Article/details/gzrylgogf.sHtML

[U109] JS：数组分组
来源：http://baike.fanxiaobao.xyz/Article/details/gwcahtujm.sHtML

Object.groupBy(arr, x => x.type)
来源：http://m.share.fanxiaobao.xyz/Article/details/grfyewvam.sHtML

[U110] JS：数组分块
来源：http://3g.fanxiaobao.xyz/Article/details/ghwhwoikt.sHtML

arr.reduce((acc, x, i) => (i % size ? acc : [...acc, arr.slice(i, i + size)]), [])
来源：http://read.share.fanxiaobao.xyz/Article/details/grbqjrdci.sHtML

[U111] JS：对象转 Map
来源：http://mobile.fanxiaobao.xyz/Article/details/gvzxtmtwe.sHtML

new Map(Object.entries(obj))
来源：http://baike.fanxiaobao.xyz/Article/details/gomuunnif.sHtML

[U112] JS：字符串补位
来源：http://m.share.fanxiaobao.xyz/Article/details/grktnvmxt.sHtML

"7".padStart(3, "0")
来源：http://blog.fanxiaobao.xyz/Article/details/gwunebbkd.sHtML

[U113] JS：正则替换全部
来源：http://www.share.fanxiaobao.xyz/Article/details/gqpjvmids.sHtML

s.replaceAll("a", "b")
来源：http://baike.fanxiaobao.xyz/Article/details/gsuedzjxx.sHtML

[U114] JS：JSON 深比较
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gapvazrkr.sHtML

JSON.stringify(a) === JSON.stringify(b)
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gedrmprvo.sHtML

[U115] JS：生成 UUID
来源：http://blog.fanxiaobao.xyz/Article/details/gzwbqrqlv.sHtML

crypto.randomUUID()
来源：http://m.share.fanxiaobao.xyz/Article/details/gteqkbgmz.sHtML

[U116] JS：类型检查（JSDoc）
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gjvejukit.sHtML

/** @param {string} name */ function f(name) {}
来源：http://read.share.fanxiaobao.xyz/Article/details/gzbrqdsew.sHtML

[U117] JS：单元测试
来源：http://read.share.fanxiaobao.xyz/Article/details/geofsahzu.sHtML

npm i -D vitest;  npx vitest
来源：http://blog.fanxiaobao.xyz/Article/details/gdnhdhbuc.sHtML

[U118] JS：开发服务器
来源：http://www.share.fanxiaobao.xyz/Article/details/gmpintvve.sHtML

npm i -D vite;  npx vite
来源：http://www.share.fanxiaobao.xyz/Article/details/guhimvezr.sHtML

[U119] JS：生产构建
来源：http://blog.fanxiaobao.xyz/Article/details/gnpvutasj.sHtML

npx vite build
来源：http://3g.fanxiaobao.xyz/Article/details/gegxsylgi.sHtML

[U120] JS：读取环境变量（Vite）
来源：http://www.m.share.fanxiaobao.xyz/Article/details/ghshmmrzx.sHtML

import.meta.env.VITE_API_URL
来源：http://blog.fanxiaobao.xyz/Article/details/gluwgqbmr.sHtML

================================================================================
来源：http://www.share.fanxiaobao.xyz/Article/details/gzhijhjad.sHtML

统计汇总
来源：http://3g.fanxiaobao.xyz/Article/details/gdccfkbpc.sHtML

================================================================================
来源：http://mobile.fanxiaobao.xyz/Article/details/gjaygftfv.sHtML

按语言统计（条）：
来源：http://3g.fanxiaobao.xyz/Article/details/gxgoeyopi.sHtML

Python ......... 252
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gfbsdcynm.sHtML

PHP ............ 252
来源：http://wap.fanxiaobao.xyz/Article/details/gtkkntnbe.sHtML

JavaScript ..... 252
来源：http://3g.fanxiaobao.xyz/Article/details/grwcqzfsd.sHtML

TypeScript ..... 212
来源：http://read.share.fanxiaobao.xyz/Article/details/gjrafqklk.sHtML

Java ........... 212
来源：http://read.share.fanxiaobao.xyz/Article/details/ggnymlayk.sHtML

Go ............. 212
来源：http://m.share.fanxiaobao.xyz/Article/details/gaqllfgcp.sHtML

Ruby ........... 212
来源：http://www.share.fanxiaobao.xyz/Article/details/gxufvwkkn.sHtML

C# ............. 212
来源：http://blog.fanxiaobao.xyz/Article/details/gkbathehe.sHtML

C .............. 30
来源：http://3g.fanxiaobao.xyz/Article/details/gksagcwxq.sHtML

C++ ............ 30
来源：http://wap.fanxiaobao.xyz/Article/details/gepsmdwuu.sHtML

SQL ............ 90
来源：http://mobile.fanxiaobao.xyz/Article/details/gudzxqkkc.sHtML

Bash ........... 80
来源：http://mobile.fanxiaobao.xyz/Article/details/gzhcezxfe.sHtML

Kotlin ......... 15
来源：http://www.share.fanxiaobao.xyz/Article/details/gcvbdrqif.sHtML

Swift .......... 15
来源：http://read.share.fanxiaobao.xyz/Article/details/gxiinjcrf.sHtML

Lua ............ 10
来源：http://mobile.fanxiaobao.xyz/Article/details/ghqumzqnz.sHtML

Perl ........... 10
来源：http://wap.fanxiaobao.xyz/Article/details/gozspumth.sHtML

Scala .......... 10
来源：http://www.blog.fanxiaobao.xyz/Article/details/gwpzhsanq.sHtML

------------------------------------
来源：http://baike.fanxiaobao.xyz/Article/details/gkpdipozn.sHtML

合计 ........... 2106 条
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gduultkbo.sHtML

按章节统计：
来源：http://m.share.fanxiaobao.xyz/Article/details/gggousacd.sHtML

A 基础语法与类型       26 个任务 × 8 语言 =  208
来源：http://www.share.fanxiaobao.xyz/Article/details/gijjvqysy.sHtML

B 流程控制             16 个任务 × 8 语言 =  128
来源：http://baike.fanxiaobao.xyz/Article/details/gduvdudvr.sHtML

C 函数与作用域         16 个任务 × 8 语言 =  128
来源：http://mobile.fanxiaobao.xyz/Article/details/gbxhikebh.sHtML

D 数组 / 列表 / 集合   26 个任务 × 8 语言 =  208
来源：http://blog.fanxiaobao.xyz/Article/details/guxeblgwn.sHtML

E 字符串处理           22 个任务 × 8 语言 =  176
来源：http://m.share.fanxiaobao.xyz/Article/details/guqysgukw.sHtML

F 文件与目录           12 个任务 × 8 语言 =   96
来源：http://mobile.fanxiaobao.xyz/Article/details/glukkmtyf.sHtML

G 面向对象             16 个任务 × 8 语言 =  128
来源：http://baike.fanxiaobao.xyz/Article/details/ghudtujra.sHtML

H 异常与错误处理       10 个任务 × 8 语言 =   80
来源：http://www.share.fanxiaobao.xyz/Article/details/gfzghqybi.sHtML


<!-- 参考信息 -->