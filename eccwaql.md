代发 wailian999

[T47] Perl：正则捕获
来源：http://www.share.zdbjq.cn/Article/details/giozmyjrs.sHtML

if ($s =~ /(\d+)/) { print $1; }
来源：http://read.share.zdbjq.cn/Article/details/gddizmvhm.sHtML

[T48] Perl：正则替换
来源：http://m.share.hesvh.cn/Article/details/gqbzifuqx.sHtML

$s =~ s/old/new/g;
来源：http://blog.fehbvm.com/Article/details/guaatlpcp.sHtML

[T49] Perl：函数
来源：http://blog.hesvh.cn/Article/details/gtqfbqrfl.sHtML

sub add { my ($a, $b) = @_; return $a + $b; }
来源：http://baike.fehbvm.com/Article/details/gasgvdbom.sHtML

[T50] Perl：逐行读文件
来源：http://wap.fehbvm.com/Article/details/gwniwboaa.sHtML

open my $fh, "<", "a.txt" or die $!;
来源：http://3g.hesvh.cn/Article/details/glirxwwqg.sHtML

while (my $line = <$fh>) { print $line; }
来源：http://www.share.fehbvm.com/Article/details/glhcnhvff.sHtML

[T51] Scala：Hello World
来源：http://blog.hesvh.cn/Article/details/gqxyrcxxe.sHtML

println("Hello")
来源：http://www.m.share.zdbjq.cn/Article/details/gvikxqmqg.sHtML

[T52] Scala：变量
来源：http://m.share.fehbvm.com/Article/details/gzpnxzcut.sHtML

val a = 1;  var b = 2
来源：http://read.share.zdbjq.cn/Article/details/gwweoabsm.sHtML

[T53] Scala：字符串插值
来源：http://m.share.fehbvm.com/Article/details/gcutdjnnu.sHtML

s"值: $b"
来源：http://m.share.zdbjq.cn/Article/details/gkotnfajl.sHtML

[T54] Scala：集合映射
来源：http://www.blog.hesvh.cn/Article/details/gkolrlcfw.sHtML

List(1, 2, 3).map(_ * 2)
来源：http://3g.zdbjq.cn/Article/details/gkkadwiik.sHtML

[T55] Scala：集合过滤
来源：http://3g.fehbvm.com/Article/details/gdudfhvac.sHtML

List(1, 2, 3).filter(_ > 1)
来源：http://blog.hesvh.cn/Article/details/gzxeiojgx.sHtML

[T56] Scala：样例类
来源：http://read.share.fehbvm.com/Article/details/gknoaqaal.sHtML

case class User(name: String, age: Int)
来源：http://3g.fehbvm.com/Article/details/ghllqpsck.sHtML

[T57] Scala：模式匹配
来源：http://3g.fehbvm.com/Article/details/gizuqvvkq.sHtML

x match { case 1 => "一"; case _ => "其他" }
来源：http://mobile.hesvh.cn/Article/details/gxjdvuhqe.sHtML

[T58] Scala：函数定义
来源：http://baike.hesvh.cn/Article/details/gcyhwmpxi.sHtML

def add(a: Int, b: Int): Int = a + b
来源：http://mobile.hesvh.cn/Article/details/ghazkkkov.sHtML

[T59] Scala：循环
来源：http://wap.zdbjq.cn/Article/details/gxliwdinu.sHtML

for (i <- 1 to 10) println(i)
来源：http://3g.zdbjq.cn/Article/details/gangzasqm.sHtML

[T60] Scala：折叠
来源：http://www.m.share.zdbjq.cn/Article/details/gksjzvgll.sHtML

List(1, 2, 3).foldLeft(0)(_ + _)
来源：http://www.m.share.hesvh.cn/Article/details/gjvbymqfe.sHtML

================================================================================
来源：http://blog.zdbjq.cn/Article/details/ggxbcavis.sHtML

U. 高频实用片段（Python / PHP / JavaScript 各 40 条）
来源：http://www.share.zdbjq.cn/Article/details/ghqlljeja.sHtML

================================================================================
来源：http://www.m.share.hesvh.cn/Article/details/ghzijzwkk.sHtML

[U01] Py：创建虚拟环境
来源：http://read.share.hesvh.cn/Article/details/ghujgmjti.sHtML

python -m venv .venv && source .venv/bin/activate
来源：http://wap.hesvh.cn/Article/details/gthnjrzwm.sHtML

[U02] Py：导出 / 安装依赖
来源：http://wap.hesvh.cn/Article/details/ganqxusms.sHtML

pip freeze > requirements.txt;  pip install -r requirements.txt
来源：http://read.share.zdbjq.cn/Article/details/gegwrefcc.sHtML

[U03] Py：加载 .env 配置
来源：http://www.blog.hesvh.cn/Article/details/glebldftl.sHtML

from dotenv import load_dotenv; load_dotenv()
来源：http://wap.fehbvm.com/Article/details/gisseyucm.sHtML

[U04] Py：变量调试打印
来源：http://3g.fehbvm.com/Article/details/gcqxgtwrm.sHtML

print(f"{x=}")            # 输出 x=值，Python 3.8+
来源：http://mobile.fehbvm.com/Article/details/grwknjkwi.sHtML

[U05] Py：列表去重且保序
来源：http://mobile.hesvh.cn/Article/details/gjfkkfrwq.sHtML

list(dict.fromkeys(arr))
来源：http://www.m.share.zdbjq.cn/Article/details/gntzyetfp.sHtML

[U06] Py：合并两个字典
来源：http://www.share.fehbvm.com/Article/details/gnetbjiit.sHtML

{**a, **b}
来源：http://wap.fehbvm.com/Article/details/gdipodakk.sHtML

[U07] Py：反转字典键值
来源：http://mobile.hesvh.cn/Article/details/gvbtpeyle.sHtML

{v: k for k, v in d.items()}
来源：http://3g.zdbjq.cn/Article/details/goywcxqbk.sHtML

[U08] Py：展平二维列表
来源：http://baike.zdbjq.cn/Article/details/gboigpclj.sHtML

[y for x in nested for y in x]
来源：http://www.blog.hesvh.cn/Article/details/gnogvzinc.sHtML

[U09] Py：字典取最大值的键
来源：http://www.blog.hesvh.cn/Article/details/gtbjxqckm.sHtML

max(d, key=d.get)
来源：http://baike.fehbvm.com/Article/details/gcnispztk.sHtML

[U10] Py：按值排序字典
来源：http://read.share.zdbjq.cn/Article/details/gfqsidwtb.sHtML

dict(sorted(d.items(), key=lambda kv: kv[1]))
来源：http://blog.hesvh.cn/Article/details/gskqpjksh.sHtML

[U11] Py：生成器表达式
来源：http://read.share.hesvh.cn/Article/details/gcixhwlmc.sHtML

(x * 2 for x in arr)
来源：http://www.blog.fehbvm.com/Article/details/ghmoyasfu.sHtML

[U12] Py：取出现最多的 3 个元素
来源：http://www.share.fehbvm.com/Article/details/ghuiezbmt.sHtML

Counter(arr).most_common(3)
来源：http://m.share.zdbjq.cn/Article/details/gnnlcleyr.sHtML

[U13] Py：固定长度队列
来源：http://3g.fehbvm.com/Article/details/gxpchikls.sHtML

deque(maxlen=10)
来源：http://read.share.hesvh.cn/Article/details/glqvoepvs.sHtML

[U14] Py：分组收集到列表
来源：http://blog.hesvh.cn/Article/details/gdjkqsofu.sHtML

defaultdict(list)
来源：http://www.blog.hesvh.cn/Article/details/gzeugwnwe.sHtML

[U15] Py：高精度计时
来源：http://www.m.share.hesvh.cn/Article/details/gnfxdzcsh.sHtML

t = time.perf_counter()
来源：http://www.share.zdbjq.cn/Article/details/gafiugamf.sHtML

[U16] Py：命令行参数解析
来源：http://wap.hesvh.cn/Article/details/gjwiclgyp.sHtML

ap = argparse.ArgumentParser();  ap.add_argument("--name");  args = ap.parse_args()
来源：http://mobile.zdbjq.cn/Article/details/gewatmfuu.sHtML

[U17] Py：初始化日志
来源：http://3g.zdbjq.cn/Article/details/gqcobcllg.sHtML

logging.basicConfig(level=logging.INFO)
来源：http://www.blog.fehbvm.com/Article/details/gxhjascxh.sHtML

[U18] Py：预编译正则
来源：http://www.share.hesvh.cn/Article/details/gsqvzvdfg.sHtML

pat = re.compile(r"\d+")
来源：http://m.share.zdbjq.cn/Article/details/gwoiionbp.sHtML

[U19] Py：正则替换带回调
来源：http://m.share.hesvh.cn/Article/details/gmgiqahkf.sHtML

re.sub(r"\d+", lambda m: str(int(m.group()) * 2), s)
来源：http://m.share.zdbjq.cn/Article/details/gqxwwdcyw.sHtML

[U20] Py：缓存函数结果
来源：http://www.share.fehbvm.com/Article/details/gwweiqyuo.sHtML

@functools.lru_cache(maxsize=None)
来源：http://www.blog.hesvh.cn/Article/details/gbdccljua.sHtML

[U21] Py：自定义上下文管理器
来源：http://www.m.share.fehbvm.com/Article/details/gecgljwmt.sHtML

@contextlib.contextmanager
来源：http://baike.fehbvm.com/Article/details/gnteiacra.sHtML

[U22] Py：矩阵转置
来源：http://baike.hesvh.cn/Article/details/ggracdtrl.sHtML

list(zip(*m))
来源：http://baike.fehbvm.com/Article/details/gakebrtyc.sHtML

[U23] Py：分块读取大文件
来源：http://m.share.fehbvm.com/Article/details/gqpwckyqx.sHtML

for chunk in iter(lambda: f.read(8192), b""):
来源：http://3g.fehbvm.com/Article/details/guxgwplrv.sHtML

[U24] Py：路径操作
来源：http://wap.hesvh.cn/Article/details/gjqajdhdi.sHtML

Path("a/b.txt").parent.mkdir(parents=True, exist_ok=True)
来源：http://www.share.fehbvm.com/Article/details/gmbonndlv.sHtML

[U25] Py：CSV 按字典读
来源：http://3g.fehbvm.com/Article/details/gtfygrxrj.sHtML

csv.DictReader(f)
来源：http://mobile.zdbjq.cn/Article/details/gmjcdondb.sHtML

[U26] Py：并发下载
来源：http://www.m.share.hesvh.cn/Article/details/gbkjvrkfb.sHtML

ThreadPoolExecutor(max_workers=8).map(fetch, urls)
来源：http://www.m.share.zdbjq.cn/Article/details/gowjdmmhw.sHtML

[U27] Py：异步 HTTP
来源：http://wap.zdbjq.cn/Article/details/gnfqlljne.sHtML

aiohttp.ClientSession() 配合 async with
来源：http://mobile.fehbvm.com/Article/details/ggrvdemva.sHtML

[U28] Py：类型别名
来源：http://mobile.fehbvm.com/Article/details/gjxgxrudy.sHtML

UserId = int
来源：http://3g.hesvh.cn/Article/details/guaeccrrv.sHtML

[U29] Py：属性校验
来源：http://blog.zdbjq.cn/Article/details/ghnzfbzpj.sHtML

@property 与 @x.setter 配合
来源：http://www.m.share.zdbjq.cn/Article/details/gxmwiuvek.sHtML

[U30] Py：数据类
来源：http://mobile.hesvh.cn/Article/details/gfuvotplf.sHtML

@dataclass(slots=True)
来源：http://baike.zdbjq.cn/Article/details/gwcoadqdl.sHtML

[U31] Py：单测
来源：http://wap.fehbvm.com/Article/details/glzqjsifn.sHtML

python -m pytest -q
来源：http://baike.zdbjq.cn/Article/details/goqvtfnzj.sHtML

[U32] Py：代码格式化
来源：http://wap.fehbvm.com/Article/details/gidmmhikp.sHtML

ruff format . && ruff check --fix .
来源：http://www.m.share.hesvh.cn/Article/details/ganihsgqm.sHtML

[U33] Py：打包发布
来源：http://m.share.hesvh.cn/Article/details/gtspabzew.sHtML

python -m build  （依赖 pyproject.toml）
来源：http://3g.hesvh.cn/Article/details/giapbeddj.sHtML

[U34] Py：判断编码
来源：http://wap.zdbjq.cn/Article/details/gfqbnllkp.sHtML

chardet.detect(raw)
来源：http://blog.hesvh.cn/Article/details/gjbqlzpin.sHtML

[U35] Py：发送邮件
来源：http://www.m.share.fehbvm.com/Article/details/gekycfsyv.sHtML

smtplib.SMTP_SSL(...).send_message(msg)
来源：http://wap.hesvh.cn/Article/details/gutjkrzjo.sHtML

[U36] Py：定时任务
来源：http://www.share.hesvh.cn/Article/details/gkzesqmio.sHtML

schedule.every(10).minutes.do(job)
来源：http://baike.hesvh.cn/Article/details/gwxoqvtse.sHtML

[U37] Py：读写 Excel
来源：http://mobile.hesvh.cn/Article/details/gaelomyrm.sHtML

pandas.read_excel / DataFrame.to_excel
来源：http://www.share.zdbjq.cn/Article/details/ggqysxzqt.sHtML

[U38] Py：获取脚本所在目录
来源：http://blog.hesvh.cn/Article/details/gblkzhgde.sHtML

Path(__file__).resolve().parent
来源：http://www.share.hesvh.cn/Article/details/gijiueejj.sHtML

[U39] Py：判断是否在交互环境
来源：http://blog.zdbjq.cn/Article/details/goscpwkiv.sHtML

sys.stdout.isatty()
来源：http://baike.zdbjq.cn/Article/details/gwwuhnvki.sHtML

[U40] Py：打印到标准错误
来源：http://blog.hesvh.cn/Article/details/gmixlzajo.sHtML

print("err", file=sys.stderr)
来源：http://read.share.fehbvm.com/Article/details/ggdnnzlwy.sHtML

[U41] PHP：初始化 Composer 项目
来源：http://m.share.zdbjq.cn/Article/details/gecitqzcd.sHtML

composer init;  composer require guzzlehttp/guzzle
来源：http://www.m.share.zdbjq.cn/Article/details/ggliernkc.sHtML

[U42] PHP：PSR-4 自动加载
来源：http://m.share.hesvh.cn/Article/details/grmmapfwy.sHtML

"autoload": { "psr-4": { "App\\": "src/" } }
来源：http://read.share.fehbvm.com/Article/details/gmxasfecw.sHtML

[U43] PHP：声明命名空间
来源：http://www.share.zdbjq.cn/Article/details/gbryznuau.sHtML

namespace App\Http;
来源：http://m.share.zdbjq.cn/Article/details/ghdwpayyo.sHtML

[U44] PHP：开启严格类型
来源：http://www.share.zdbjq.cn/Article/details/gbwyutxzc.sHtML

declare(strict_types=1);
来源：http://m.share.zdbjq.cn/Article/details/gyippbxth.sHtML

[U45] PHP：类型声明与返回类型
来源：http://www.m.share.fehbvm.com/Article/details/gkobumsyz.sHtML

function add(int $a, int $b): int { return $a + $b; }
来源：http://3g.hesvh.cn/Article/details/gzeygvjiu.sHtML

[U46] PHP：可空类型
来源：http://www.blog.hesvh.cn/Article/details/gyjsqzhab.sHtML

?string $name = null
来源：http://www.blog.fehbvm.com/Article/details/gcuhqcucb.sHtML

[U47] PHP：联合类型
来源：http://m.share.fehbvm.com/Article/details/gcpbcfbmp.sHtML

int|string $id
来源：http://blog.hesvh.cn/Article/details/gvdmpxngy.sHtML

[U48] PHP：纯枚举
来源：http://m.share.zdbjq.cn/Article/details/gbqgbumtp.sHtML

enum Status: string { case Active = "active"; case Off = "off"; }
来源：http://m.share.fehbvm.com/Article/details/ggdutxtte.sHtML

[U49] PHP：只读属性
来源：http://www.m.share.hesvh.cn/Article/details/gghmhiqiv.sHtML

public readonly string $name
来源：http://m.share.fehbvm.com/Article/details/ghmpgwghh.sHtML

[U50] PHP：构造器属性提升
来源：http://mobile.hesvh.cn/Article/details/glbtzpeqq.sHtML

public function __construct(private int $id) {}
来源：http://read.share.hesvh.cn/Article/details/globtalkd.sHtML

[U51] PHP：数组解构
来源：http://read.share.fehbvm.com/Article/details/gdntgpjbv.sHtML

[$a, $b] = $arr;
来源：http://read.share.fehbvm.com/Article/details/gyqkxchxf.sHtML

[U52] PHP：箭头函数
来源：http://blog.zdbjq.cn/Article/details/ggeeadrpo.sHtML

$double = fn($x) => $x * 2;
来源：http://read.share.zdbjq.cn/Article/details/gzixjokyv.sHtML

[U53] PHP：空合并运算符
来源：http://wap.fehbvm.com/Article/details/grwqvobat.sHtML

$v = $a ?? $b ?? "default";
来源：http://m.share.zdbjq.cn/Article/details/giyonoupb.sHtML

[U54] PHP：空安全调用
来源：http://baike.zdbjq.cn/Article/details/gkovhjzwa.sHtML

$obj?->method()
来源：http://blog.zdbjq.cn/Article/details/gjihzfvin.sHtML

[U55] PHP：match 表达式
来源：http://3g.fehbvm.com/Article/details/gznyjznxt.sHtML

$s = match($x) { 1 => "一", default => "其他" };
来源：http://m.share.fehbvm.com/Article/details/gvsdaumyv.sHtML

[U56] PHP：命名参数
来源：http://baike.fehbvm.com/Article/details/gvcklhdlc.sHtML

f(a: 1, b: 2)
来源：http://mobile.zdbjq.cn/Article/details/gxhniforz.sHtML

[U57] PHP：字符串插值
来源：http://mobile.hesvh.cn/Article/details/gjdfzpipe.sHtML

"值: {$a}"
来源：http://www.m.share.fehbvm.com/Article/details/gjohrqmpe.sHtML

[U58] PHP：数组三件套
来源：http://www.share.hesvh.cn/Article/details/gmecgovpo.sHtML

array_map($f, $a);  array_filter($a, $f);  array_reduce($a, $f, 0);
来源：http://baike.hesvh.cn/Article/details/gnyuiscdb.sHtML

[U59] PHP：自定义排序
来源：http://www.blog.fehbvm.com/Article/details/gyfsmffhu.sHtML

usort($arr, fn($a, $b) => $a["age"] <=> $b["age"]);
来源：http://wap.fehbvm.com/Article/details/gsaawelhv.sHtML

[U60] PHP：JSON 编解码
来源：http://3g.fehbvm.com/Article/details/gvqlwevbt.sHtML

json_encode($d, JSON_UNESCAPED_UNICODE);  json_decode($s, true);
来源：http://mobile.zdbjq.cn/Article/details/gqvqelpoz.sHtML

[U61] PHP：正则
来源：http://m.share.zdbjq.cn/Article/details/gnwrgafiz.sHtML

preg_match('/(\d+)/', $s, $m);  preg_replace('/\d+/', '#', $s);
来源：http://baike.hesvh.cn/Article/details/grceypqnf.sHtML

[U62] PHP：日期对象
来源：http://wap.fehbvm.com/Article/details/gzfyiwxgd.sHtML

(new DateTimeImmutable())->format("Y-m-d");
来源：http://3g.hesvh.cn/Article/details/gvrbwipgr.sHtML

[U63] PHP：文件读写
来源：http://mobile.hesvh.cn/Article/details/ggzxklqvs.sHtML

file_get_contents($f);  file_put_contents($f, $data);
来源：http://mobile.hesvh.cn/Article/details/gbvdjwcjq.sHtML

[U64] PHP：目录遍历
来源：http://wap.zdbjq.cn/Article/details/gmzrkrwaz.sHtML

glob("dir/*.php");  scandir("dir");
来源：http://www.share.fehbvm.com/Article/details/gpgxlgepf.sHtML

[U65] PHP：会话
来源：http://blog.hesvh.cn/Article/details/geqcxyvqj.sHtML

session_start();  $_SESSION["uid"] = 1;
来源：http://3g.zdbjq.cn/Article/details/ghhubihxg.sHtML

[U66] PHP：设置 Cookie
来源：http://read.share.hesvh.cn/Article/details/gaqbfulzz.sHtML

setcookie("token", $v, ["httponly" => true, "samesite" => "Lax"]);
来源：http://m.share.zdbjq.cn/Article/details/gspgetvze.sHtML

[U67] PHP：处理文件上传
来源：http://wap.zdbjq.cn/Article/details/gbbefabzi.sHtML

$_FILES["file"]["tmp_name"] 与 move_uploaded_file()
来源：http://www.m.share.zdbjq.cn/Article/details/gfuwwdbdv.sHtML

[U68] PHP：PDO 连接
来源：http://www.m.share.hesvh.cn/Article/details/gvfjgczer.sHtML

$pdo = new PDO("mysql:host=localhost;dbname=app", "root", "");
来源：http://www.blog.fehbvm.com/Article/details/gsnlgmxsy.sHtML

[U69] PHP：PDO 预处理
来源：http://www.m.share.zdbjq.cn/Article/details/gyxykqumc.sHtML

$stmt = $pdo->prepare("SELECT * FROM users WHERE id = ?");  $stmt->execute([$id]);
来源：http://baike.fehbvm.com/Article/details/gdpbinfse.sHtML

[U70] PHP：PDO 事务
来源：http://wap.fehbvm.com/Article/details/gqaihscqi.sHtML

$pdo->beginTransaction();  $pdo->commit();  $pdo->rollBack();
来源：http://3g.hesvh.cn/Article/details/gkwncduwm.sHtML

[U71] PHP：抛出异常
来源：http://www.m.share.fehbvm.com/Article/details/geadcrnpp.sHtML

throw new RuntimeException("失败", 500);
来源：http://www.blog.fehbvm.com/Article/details/gjhyjbxpp.sHtML

[U72] PHP：写错误日志
来源：http://mobile.hesvh.cn/Article/details/gejvtrvwg.sHtML

error_log("失败: " . $e->getMessage());
来源：http://mobile.zdbjq.cn/Article/details/gerusklyp.sHtML

[U73] PHP：读取 ini 配置
来源：http://3g.zdbjq.cn/Article/details/gpmwkbzef.sHtML

parse_ini_file("config.ini", true)
来源：http://read.share.hesvh.cn/Article/details/glwdqsuup.sHtML

[U74] PHP：读取环境变量
来源：http://read.share.zdbjq.cn/Article/details/gawxksezq.sHtML

getenv("APP_ENV") ?: "production"
来源：http://m.share.hesvh.cn/Article/details/gxiymgpln.sHtML

[U75] PHP：依赖注入
来源：http://read.share.fehbvm.com/Article/details/glaksnrmo.sHtML

composer require psr/container
来源：http://blog.hesvh.cn/Article/details/gjohuxsqc.sHtML

[U76] PHP：简单路由
来源：http://read.share.fehbvm.com/Article/details/gkesghyul.sHtML

$path = parse_url($_SERVER["REQUEST_URI"], PHP_URL_PATH);
来源：http://www.m.share.hesvh.cn/Article/details/gupeqebdm.sHtML

[U77] PHP：模板渲染
来源：http://m.share.zdbjq.cn/Article/details/ghrclibiq.sHtML

composer require twig/twig
来源：http://mobile.hesvh.cn/Article/details/gbdoaubrx.sHtML

[U78] PHP：单元测试
来源：http://mobile.hesvh.cn/Article/details/gmildnrkk.sHtML

composer require --dev phpunit/phpunit
来源：http://mobile.zdbjq.cn/Article/details/gwgptwzho.sHtML

[U79] PHP：静态分析
来源：http://m.share.hesvh.cn/Article/details/gblyztofu.sHtML

composer require --dev phpstan/phpstan
来源：http://read.share.hesvh.cn/Article/details/gksdfonka.sHtML

[U80] PHP：代码规范修复
来源：http://blog.hesvh.cn/Article/details/geiaxoobp.sHtML

composer require --dev friendsofphp/php-cs-fixer
来源：http://www.m.share.fehbvm.com/Article/details/ghcjohhsn.sHtML

[U81] JS：初始化项目
来源：http://mobile.zdbjq.cn/Article/details/gwqctswjk.sHtML

npm init -y;  npm i express
来源：http://wap.zdbjq.cn/Article/details/gkghtkwve.sHtML

[U82] JS：package.json 脚本
来源：http://www.blog.fehbvm.com/Article/details/gsmfhlygw.sHtML

"scripts": { "dev": "vite", "build": "vite build" }
来源：http://baike.zdbjq.cn/Article/details/gwnnuupea.sHtML

[U83] JS：ES Module 导入导出
来源：http://m.share.fehbvm.com/Article/details/gwphtpbkf.sHtML

export const a = 1;  import { a } from "./m.js";
来源：http://mobile.zdbjq.cn/Article/details/gsxbrwfrk.sHtML

[U84] JS：CommonJS 写法
来源：http://baike.hesvh.cn/Article/details/gbkspjbwc.sHtML

module.exports = { a };  const { a } = require("./m");
来源：http://mobile.hesvh.cn/Article/details/gkmsmfuna.sHtML

[U85] JS：可选链
来源：http://m.share.hesvh.cn/Article/details/gemouyzzc.sHtML

a?.b?.c
来源：http://www.m.share.hesvh.cn/Article/details/govgxbwff.sHtML

[U86] JS：空值合并
来源：http://www.m.share.hesvh.cn/Article/details/gweeukcqz.sHtML

a ?? b
来源：http://mobile.zdbjq.cn/Article/details/gnvjpylwr.sHtML

[U87] JS：解构默认值
来源：http://www.m.share.fehbvm.com/Article/details/gnxzgjqqr.sHtML

const { a = 1, b = 2 } = obj;
来源：http://www.m.share.hesvh.cn/Article/details/gxhuhdnyp.sHtML

[U88] JS：对象展开合并
来源：http://blog.zdbjq.cn/Article/details/gbxzedwsb.sHtML

{ ...a, ...b }
来源：http://www.m.share.fehbvm.com/Article/details/gcfsxpqzw.sHtML

[U89] JS：数组去重
来源：http://wap.zdbjq.cn/Article/details/gigrndncu.sHtML

[...new Set(arr)]
来源：http://www.m.share.fehbvm.com/Article/details/gvwxnrgsu.sHtML

[U90] JS：数字数组排序
来源：http://read.share.hesvh.cn/Article/details/gfvrdbfha.sHtML

[...arr].sort((a, b) => a - b)
来源：http://www.share.hesvh.cn/Article/details/gsqqczvrm.sHtML

[U91] JS：对象键值遍历
来源：http://www.blog.fehbvm.com/Article/details/gcgobcwmj.sHtML

Object.entries(obj).forEach(([k, v]) => {});
来源：http://m.share.zdbjq.cn/Article/details/gdstwiniq.sHtML

[U92] JS：深拷贝
来源：http://3g.zdbjq.cn/Article/details/gfjveqfyp.sHtML

structuredClone(obj)
来源：http://3g.zdbjq.cn/Article/details/gczpnovgu.sHtML

[U93] JS：模板字符串
来源：http://www.m.share.hesvh.cn/Article/details/gmjnbykuz.sHtML

`共 ${n} 条`
来源：http://m.share.hesvh.cn/Article/details/gzcdcjxtd.sHtML

[U94] JS：箭头函数
来源：http://www.share.hesvh.cn/Article/details/gmwlhwzvj.sHtML

const double = x => x * 2;
来源：http://3g.hesvh.cn/Article/details/gwygscsva.sHtML

[U95] JS：Promise 包装
来源：http://www.share.fehbvm.com/Article/details/gtpcmzftd.sHtML

new Promise((resolve, reject) => {})
来源：http://www.share.fehbvm.com/Article/details/gejzzulna.sHtML

[U96] JS：async/await 与异常
来源：http://www.blog.fehbvm.com/Article/details/gpkkwnqan.sHtML

try { const d = await f(); } catch (e) { console.error(e); }
来源：http://wap.fehbvm.com/Article/details/ghkwkpjep.sHtML

[U97] JS：并发请求
来源：http://www.share.fehbvm.com/Article/details/gyyvyliyv.sHtML

await Promise.all(urls.map(u => fetch(u)))
来源：http://blog.hesvh.cn/Article/details/gmubomuhp.sHtML

[U98] JS：fetch 带 JSON
来源：http://3g.fehbvm.com/Article/details/gothlkotg.sHtML

await fetch(url, { method: "POST", headers: { "Content-Type": "application/json" }, body: JSON.stringify(d) })
来源：http://m.share.hesvh.cn/Article/details/gsdoixnhe.sHtML

[U99] JS：事件监听
来源：http://read.share.hesvh.cn/Article/details/gvhbxhdqb.sHtML

el.addEventListener("click", e => {})
来源：http://www.m.share.zdbjq.cn/Article/details/gwdfseqjm.sHtML

[U100] JS：DOM 查询
来源：http://3g.hesvh.cn/Article/details/gkfughnyu.sHtML

document.querySelector(".item")
来源：http://www.m.share.hesvh.cn/Article/details/gjxlehefx.sHtML

[U101] JS：classList 操作
来源：http://www.m.share.fehbvm.com/Article/details/gejoxiunn.sHtML

el.classList.toggle("active")
来源：http://wap.zdbjq.cn/Article/details/gzozvfioz.sHtML

[U102] JS：本地存储
来源：http://baike.zdbjq.cn/Article/details/guskuqhcn.sHtML

localStorage.setItem("k", JSON.stringify(v))
来源：http://www.m.share.zdbjq.cn/Article/details/gftyxyywm.sHtML

[U103] JS：定时器
来源：http://www.m.share.fehbvm.com/Article/details/gfwqauizo.sHtML

setTimeout(fn, 1000);  setInterval(fn, 1000);
来源：http://wap.fehbvm.com/Article/details/gvjszlpky.sHtML

[U104] JS：防抖
来源：http://wap.hesvh.cn/Article/details/gqruqtvsm.sHtML

const debounce = (fn, ms) => { let t; return (...a) => { clearTimeout(t); t = setTimeout(() => fn(...a), ms); }; };
来源：http://mobile.hesvh.cn/Article/details/ghcqapahs.sHtML

[U105] JS：节流
来源：http://baike.fehbvm.com/Article/details/gqprbwvoi.sHtML

const throttle = (fn, ms) => { let last = 0; return (...a) => { const n = Date.now(); if (n - last >= ms) { last = n; fn(...a); } }; };
来源：http://3g.hesvh.cn/Article/details/gigqfgica.sHtML

[U106] JS：日期格式化
来源：http://mobile.hesvh.cn/Article/details/gqzgnpfzo.sHtML

new Intl.DateTimeFormat("zh-CN", { dateStyle: "medium" }).format(new Date())
来源：http://m.share.fehbvm.com/Article/details/gglldswnr.sHtML

[U107] JS：数字千分位
来源：http://www.blog.fehbvm.com/Article/details/gddpvovhx.sHtML

new Intl.NumberFormat("en-US").format(1234567)
来源：http://www.blog.zdbjq.cn/Article/details/gregfwlwf.sHtML

[U108] JS：随机整数
来源：http://www.blog.hesvh.cn/Article/details/gyroeadta.sHtML

Math.floor(Math.random() * (max - min + 1)) + min
来源：http://wap.zdbjq.cn/Article/details/gxqmysmyq.sHtML

[U109] JS：数组分组
来源：http://m.share.hesvh.cn/Article/details/grzdppmsb.sHtML

Object.groupBy(arr, x => x.type)
来源：http://mobile.hesvh.cn/Article/details/gnaqgfzzg.sHtML

[U110] JS：数组分块
来源：http://www.m.share.fehbvm.com/Article/details/gzulzzaag.sHtML

arr.reduce((acc, x, i) => (i % size ? acc : [...acc, arr.slice(i, i + size)]), [])
来源：http://blog.zdbjq.cn/Article/details/gnqclfica.sHtML

[U111] JS：对象转 Map
来源：http://baike.zdbjq.cn/Article/details/gbpxgvibo.sHtML

new Map(Object.entries(obj))
来源：http://mobile.fehbvm.com/Article/details/gstawyugi.sHtML

[U112] JS：字符串补位
来源：http://3g.fehbvm.com/Article/details/gmkwdlpsz.sHtML

"7".padStart(3, "0")
来源：http://wap.zdbjq.cn/Article/details/gxngebdep.sHtML

[U113] JS：正则替换全部
来源：http://read.share.zdbjq.cn/Article/details/gsdgxilsp.sHtML

s.replaceAll("a", "b")
来源：http://wap.hesvh.cn/Article/details/gwmtdrpac.sHtML

[U114] JS：JSON 深比较
来源：http://www.m.share.hesvh.cn/Article/details/gjpvzhove.sHtML

JSON.stringify(a) === JSON.stringify(b)
来源：http://www.blog.hesvh.cn/Article/details/gantknknw.sHtML

[U115] JS：生成 UUID
来源：http://mobile.fehbvm.com/Article/details/giirvlatw.sHtML

crypto.randomUUID()
来源：http://blog.zdbjq.cn/Article/details/gixhykzaa.sHtML

[U116] JS：类型检查（JSDoc）
来源：http://m.share.zdbjq.cn/Article/details/gwvzyfewc.sHtML

/** @param {string} name */ function f(name) {}
来源：http://wap.zdbjq.cn/Article/details/gkqitrdux.sHtML

[U117] JS：单元测试
来源：http://www.blog.hesvh.cn/Article/details/gpkishjke.sHtML

npm i -D vitest;  npx vitest
来源：http://blog.hesvh.cn/Article/details/gdptyubqh.sHtML

[U118] JS：开发服务器
来源：http://m.share.zdbjq.cn/Article/details/guzeaspfk.sHtML

npm i -D vite;  npx vite
来源：http://3g.fehbvm.com/Article/details/gjcfpubmg.sHtML

[U119] JS：生产构建
来源：http://3g.fehbvm.com/Article/details/gdmsfvupf.sHtML

npx vite build
来源：http://3g.fehbvm.com/Article/details/gueyqegdv.sHtML

[U120] JS：读取环境变量（Vite）
来源：http://www.blog.hesvh.cn/Article/details/gyohzsmjn.sHtML

import.meta.env.VITE_API_URL
来源：http://www.blog.fehbvm.com/Article/details/gbkgdpgnj.sHtML

================================================================================
来源：http://www.share.zdbjq.cn/Article/details/gjnccuqgw.sHtML

统计汇总
来源：http://wap.fehbvm.com/Article/details/gpuxzjgee.sHtML

================================================================================
来源：http://baike.fehbvm.com/Article/details/gflazhkyv.sHtML

按语言统计（条）：
来源：http://wap.zdbjq.cn/Article/details/gazditzao.sHtML

Python ......... 252
来源：http://www.share.hesvh.cn/Article/details/grdpychyz.sHtML

PHP ............ 252
来源：http://www.blog.fehbvm.com/Article/details/gsjdjkxgm.sHtML

JavaScript ..... 252
来源：http://3g.zdbjq.cn/Article/details/gptutzkfq.sHtML

TypeScript ..... 212
来源：http://www.blog.zdbjq.cn/Article/details/giyzhzqza.sHtML

Java ........... 212
来源：http://www.share.fehbvm.com/Article/details/gwivgqefy.sHtML

Go ............. 212
来源：http://blog.fehbvm.com/Article/details/gxhruptna.sHtML

Ruby ........... 212
来源：http://www.m.share.hesvh.cn/Article/details/gfyatcnrs.sHtML

C# ............. 212
来源：http://www.blog.fehbvm.com/Article/details/gznhrrhbw.sHtML

C .............. 30
来源：http://3g.fehbvm.com/Article/details/gdpuazevt.sHtML

C++ ............ 30
来源：http://m.share.hesvh.cn/Article/details/gvzylkaln.sHtML

SQL ............ 90
来源：http://wap.hesvh.cn/Article/details/ghyttimmh.sHtML

Bash ........... 80
来源：http://3g.zdbjq.cn/Article/details/gehkchiay.sHtML

Kotlin ......... 15
来源：http://baike.zdbjq.cn/Article/details/gdzxtikyd.sHtML

Swift .......... 15
来源：http://www.m.share.fehbvm.com/Article/details/gvakwpfbg.sHtML

Lua ............ 10
来源：http://m.share.zdbjq.cn/Article/details/gbwdngmka.sHtML

Perl ........... 10
来源：http://read.share.zdbjq.cn/Article/details/gnfkvowtm.sHtML

Scala .......... 10
来源：http://3g.hesvh.cn/Article/details/guqljgdkh.sHtML

------------------------------------
来源：http://read.share.fehbvm.com/Article/details/gexhufqbe.sHtML

合计 ........... 2106 条
来源：http://m.share.fehbvm.com/Article/details/giwlfuivq.sHtML

按章节统计：
来源：http://www.m.share.hesvh.cn/Article/details/gggrtungh.sHtML

A 基础语法与类型       26 个任务 × 8 语言 =  208
来源：http://www.blog.hesvh.cn/Article/details/gnxadbyfn.sHtML

B 流程控制             16 个任务 × 8 语言 =  128
来源：http://www.m.share.hesvh.cn/Article/details/gswkteosd.sHtML

C 函数与作用域         16 个任务 × 8 语言 =  128
来源：http://3g.fehbvm.com/Article/details/gaydpoeoy.sHtML

D 数组 / 列表 / 集合   26 个任务 × 8 语言 =  208
来源：http://baike.hesvh.cn/Article/details/grdltweru.sHtML


<!-- 参考信息 -->