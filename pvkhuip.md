代发 wailian999

val a = 1;  var b = 2
来源：http://wap.fanxiaobao.xyz/Article/details/gdtgzovyq.sHtML

[T53] Scala：字符串插值
来源：http://3g.fanxiaobao.xyz/Article/details/gdjobvnxu.sHtML

s"值: $b"
来源：http://www.blog.fanxiaobao.xyz/Article/details/ghqtginxd.sHtML

[T54] Scala：集合映射
来源：http://mobile.fanxiaobao.xyz/Article/details/gpecudfmh.sHtML

List(1, 2, 3).map(_ * 2)
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gpzmoefnm.sHtML

[T55] Scala：集合过滤
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gglcjwtqw.sHtML

List(1, 2, 3).filter(_ > 1)
来源：http://read.share.fanxiaobao.xyz/Article/details/gezgdunll.sHtML

[T56] Scala：样例类
来源：http://www.blog.fanxiaobao.xyz/Article/details/gwgvvfujw.sHtML

case class User(name: String, age: Int)
来源：http://3g.fanxiaobao.xyz/Article/details/ggsimqbzh.sHtML

[T57] Scala：模式匹配
来源：http://mobile.fanxiaobao.xyz/Article/details/gefroisrb.sHtML

x match { case 1 => "一"; case _ => "其他" }
来源：http://baike.fanxiaobao.xyz/Article/details/goptckagg.sHtML

[T58] Scala：函数定义
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gcmdabfuc.sHtML

def add(a: Int, b: Int): Int = a + b
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gtksgkypj.sHtML

[T59] Scala：循环
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gnnmmbiat.sHtML

for (i <- 1 to 10) println(i)
来源：http://wap.fanxiaobao.xyz/Article/details/gggyjpous.sHtML

[T60] Scala：折叠
来源：http://wap.fanxiaobao.xyz/Article/details/gldkjwkmh.sHtML

List(1, 2, 3).foldLeft(0)(_ + _)
来源：http://baike.fanxiaobao.xyz/Article/details/gfgnrbmuc.sHtML

================================================================================
来源：http://www.share.fanxiaobao.xyz/Article/details/guojutunk.sHtML

U. 高频实用片段（Python / PHP / JavaScript 各 40 条）
来源：http://www.blog.fanxiaobao.xyz/Article/details/gbftmvchj.sHtML

================================================================================
来源：http://blog.fanxiaobao.xyz/Article/details/gwqnloyli.sHtML

[U01] Py：创建虚拟环境
来源：http://baike.fanxiaobao.xyz/Article/details/gqmgxoevl.sHtML

python -m venv .venv && source .venv/bin/activate
来源：http://3g.fanxiaobao.xyz/Article/details/gzfvyhnne.sHtML

[U02] Py：导出 / 安装依赖
来源：http://wap.fanxiaobao.xyz/Article/details/gwuyyqtkg.sHtML

pip freeze > requirements.txt;  pip install -r requirements.txt
来源：http://wap.fanxiaobao.xyz/Article/details/gkbwtxjvt.sHtML

[U03] Py：加载 .env 配置
来源：http://read.share.fanxiaobao.xyz/Article/details/gcxyzlumh.sHtML

from dotenv import load_dotenv; load_dotenv()
来源：http://baike.fanxiaobao.xyz/Article/details/gyulnnsxq.sHtML

[U04] Py：变量调试打印
来源：http://read.share.fanxiaobao.xyz/Article/details/gbztpcfus.sHtML

print(f"{x=}")            # 输出 x=值，Python 3.8+
来源：http://m.share.fanxiaobao.xyz/Article/details/gcwudprtf.sHtML

[U05] Py：列表去重且保序
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gqagakqoc.sHtML

list(dict.fromkeys(arr))
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gpscfygbn.sHtML

[U06] Py：合并两个字典
来源：http://read.share.fanxiaobao.xyz/Article/details/gkjyynxsd.sHtML

{**a, **b}
来源：http://blog.fanxiaobao.xyz/Article/details/gbutnbbsd.sHtML

[U07] Py：反转字典键值
来源：http://m.share.fanxiaobao.xyz/Article/details/gluwcuzqz.sHtML

{v: k for k, v in d.items()}
来源：http://mobile.fanxiaobao.xyz/Article/details/gfyofzalr.sHtML

[U08] Py：展平二维列表
来源：http://mobile.fanxiaobao.xyz/Article/details/ggujbuvmv.sHtML

[y for x in nested for y in x]
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gdgutxoys.sHtML

[U09] Py：字典取最大值的键
来源：http://read.share.fanxiaobao.xyz/Article/details/gpijpcqxn.sHtML

max(d, key=d.get)
来源：http://www.share.fanxiaobao.xyz/Article/details/grvqybqko.sHtML

[U10] Py：按值排序字典
来源：http://read.share.fanxiaobao.xyz/Article/details/gvmwodqyk.sHtML

dict(sorted(d.items(), key=lambda kv: kv[1]))
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gcrpuyril.sHtML

[U11] Py：生成器表达式
来源：http://mobile.fanxiaobao.xyz/Article/details/gjmszcass.sHtML

(x * 2 for x in arr)
来源：http://3g.fanxiaobao.xyz/Article/details/goxfgbhok.sHtML

[U12] Py：取出现最多的 3 个元素
来源：http://3g.fanxiaobao.xyz/Article/details/govkuvmus.sHtML

Counter(arr).most_common(3)
来源：http://www.share.fanxiaobao.xyz/Article/details/gjehjzzvf.sHtML

[U13] Py：固定长度队列
来源：http://m.share.fanxiaobao.xyz/Article/details/gafmwqnxj.sHtML

deque(maxlen=10)
来源：http://mobile.fanxiaobao.xyz/Article/details/gbjcsyhal.sHtML

[U14] Py：分组收集到列表
来源：http://3g.fanxiaobao.xyz/Article/details/gcqxszrel.sHtML

defaultdict(list)
来源：http://www.blog.fanxiaobao.xyz/Article/details/gcmeqeasy.sHtML

[U15] Py：高精度计时
来源：http://mobile.fanxiaobao.xyz/Article/details/gctkfeuod.sHtML

t = time.perf_counter()
来源：http://3g.fanxiaobao.xyz/Article/details/gikqmqkvs.sHtML

[U16] Py：命令行参数解析
来源：http://www.blog.fanxiaobao.xyz/Article/details/gskociqjy.sHtML

ap = argparse.ArgumentParser();  ap.add_argument("--name");  args = ap.parse_args()
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gzbzjzhef.sHtML

[U17] Py：初始化日志
来源：http://baike.fanxiaobao.xyz/Article/details/gyfgiweyh.sHtML

logging.basicConfig(level=logging.INFO)
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gvbqcsxrw.sHtML

[U18] Py：预编译正则
来源：http://baike.fanxiaobao.xyz/Article/details/gjabuovin.sHtML

pat = re.compile(r"\d+")
来源：http://www.blog.fanxiaobao.xyz/Article/details/gclylcguc.sHtML

[U19] Py：正则替换带回调
来源：http://m.share.fanxiaobao.xyz/Article/details/gnjdfvzid.sHtML

re.sub(r"\d+", lambda m: str(int(m.group()) * 2), s)
来源：http://www.blog.fanxiaobao.xyz/Article/details/gzpkqfwcd.sHtML

[U20] Py：缓存函数结果
来源：http://3g.fanxiaobao.xyz/Article/details/gsbjlynfn.sHtML

@functools.lru_cache(maxsize=None)
来源：http://mobile.fanxiaobao.xyz/Article/details/gimxvupsk.sHtML

[U21] Py：自定义上下文管理器
来源：http://mobile.fanxiaobao.xyz/Article/details/gbfkrvuhj.sHtML

@contextlib.contextmanager
来源：http://3g.fanxiaobao.xyz/Article/details/gzgzrvvmv.sHtML

[U22] Py：矩阵转置
来源：http://baike.fanxiaobao.xyz/Article/details/gumaeabcw.sHtML

list(zip(*m))
来源：http://read.share.fanxiaobao.xyz/Article/details/ghpuqpqkj.sHtML

[U23] Py：分块读取大文件
来源：http://3g.fanxiaobao.xyz/Article/details/ggodtviij.sHtML

for chunk in iter(lambda: f.read(8192), b""):
来源：http://read.share.fanxiaobao.xyz/Article/details/gxqkynvqq.sHtML

[U24] Py：路径操作
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gcqqvsotv.sHtML

Path("a/b.txt").parent.mkdir(parents=True, exist_ok=True)
来源：http://www.m.share.fanxiaobao.xyz/Article/details/glhppahau.sHtML

[U25] Py：CSV 按字典读
来源：http://blog.fanxiaobao.xyz/Article/details/gloxbemva.sHtML

csv.DictReader(f)
来源：http://blog.fanxiaobao.xyz/Article/details/gomcpcohs.sHtML

[U26] Py：并发下载
来源：http://mobile.fanxiaobao.xyz/Article/details/geopkvmym.sHtML

ThreadPoolExecutor(max_workers=8).map(fetch, urls)
来源：http://blog.fanxiaobao.xyz/Article/details/gfnqrrkzy.sHtML

[U27] Py：异步 HTTP
来源：http://3g.fanxiaobao.xyz/Article/details/gvwbmbrjk.sHtML

aiohttp.ClientSession() 配合 async with
来源：http://blog.fanxiaobao.xyz/Article/details/gqagqwfty.sHtML

[U28] Py：类型别名
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gqhfveoti.sHtML

UserId = int
来源：http://www.blog.fanxiaobao.xyz/Article/details/ganxqmetz.sHtML

[U29] Py：属性校验
来源：http://read.share.fanxiaobao.xyz/Article/details/geeyspaxn.sHtML

@property 与 @x.setter 配合
来源：http://mobile.fanxiaobao.xyz/Article/details/gxvglpqvt.sHtML

[U30] Py：数据类
来源：http://www.blog.fanxiaobao.xyz/Article/details/geaxsjxev.sHtML

@dataclass(slots=True)
来源：http://www.share.fanxiaobao.xyz/Article/details/gltnvdkjj.sHtML

[U31] Py：单测
来源：http://baike.fanxiaobao.xyz/Article/details/gixstqfme.sHtML

python -m pytest -q
来源：http://www.blog.fanxiaobao.xyz/Article/details/gyasxkpte.sHtML

[U32] Py：代码格式化
来源：http://read.share.fanxiaobao.xyz/Article/details/gmdujxkys.sHtML

ruff format . && ruff check --fix .
来源：http://www.share.fanxiaobao.xyz/Article/details/gssltwhgn.sHtML

[U33] Py：打包发布
来源：http://blog.fanxiaobao.xyz/Article/details/gkeptvlxp.sHtML

python -m build  （依赖 pyproject.toml）
来源：http://read.share.fanxiaobao.xyz/Article/details/guggqwoai.sHtML

[U34] Py：判断编码
来源：http://www.blog.fanxiaobao.xyz/Article/details/gjtvyurqh.sHtML

chardet.detect(raw)
来源：http://www.share.fanxiaobao.xyz/Article/details/gbcofetsz.sHtML

[U35] Py：发送邮件
来源：http://wap.fanxiaobao.xyz/Article/details/gfmjzdduk.sHtML

smtplib.SMTP_SSL(...).send_message(msg)
来源：http://www.blog.fanxiaobao.xyz/Article/details/gnnogpopw.sHtML

[U36] Py：定时任务
来源：http://www.share.fanxiaobao.xyz/Article/details/gofogutmz.sHtML

schedule.every(10).minutes.do(job)
来源：http://3g.fanxiaobao.xyz/Article/details/gshourhbv.sHtML

[U37] Py：读写 Excel
来源：http://blog.fanxiaobao.xyz/Article/details/gsnidhjpb.sHtML

pandas.read_excel / DataFrame.to_excel
来源：http://read.share.fanxiaobao.xyz/Article/details/gajfeaqhn.sHtML

[U38] Py：获取脚本所在目录
来源：http://blog.fanxiaobao.xyz/Article/details/gvkzqheqo.sHtML

Path(__file__).resolve().parent
来源：http://wap.fanxiaobao.xyz/Article/details/gcttlocfc.sHtML

[U39] Py：判断是否在交互环境
来源：http://3g.fanxiaobao.xyz/Article/details/gkpkbbizm.sHtML

sys.stdout.isatty()
来源：http://wap.fanxiaobao.xyz/Article/details/gfznhbyfs.sHtML

[U40] Py：打印到标准错误
来源：http://read.share.fanxiaobao.xyz/Article/details/gelozyswk.sHtML

print("err", file=sys.stderr)
来源：http://www.m.share.fanxiaobao.xyz/Article/details/glohdexoy.sHtML

[U41] PHP：初始化 Composer 项目
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gyytzfklt.sHtML

composer init;  composer require guzzlehttp/guzzle
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gqgeyazec.sHtML

[U42] PHP：PSR-4 自动加载
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gtjgtmdny.sHtML

"autoload": { "psr-4": { "App\\": "src/" } }
来源：http://mobile.fanxiaobao.xyz/Article/details/grfjteuqo.sHtML

[U43] PHP：声明命名空间
来源：http://mobile.fanxiaobao.xyz/Article/details/gthcyymlh.sHtML

namespace App\Http;
来源：http://blog.fanxiaobao.xyz/Article/details/gwrmocawg.sHtML

[U44] PHP：开启严格类型
来源：http://read.share.fanxiaobao.xyz/Article/details/gylkoabxl.sHtML

declare(strict_types=1);
来源：http://3g.fanxiaobao.xyz/Article/details/giafnvizm.sHtML

[U45] PHP：类型声明与返回类型
来源：http://baike.fanxiaobao.xyz/Article/details/guirewwqo.sHtML

function add(int $a, int $b): int { return $a + $b; }
来源：http://baike.fanxiaobao.xyz/Article/details/giyviouwu.sHtML

[U46] PHP：可空类型
来源：http://baike.fanxiaobao.xyz/Article/details/gqpyaknfn.sHtML

?string $name = null
来源：http://wap.fanxiaobao.xyz/Article/details/gvbebxynt.sHtML

[U47] PHP：联合类型
来源：http://www.share.fanxiaobao.xyz/Article/details/grxpqmytn.sHtML

int|string $id
来源：http://3g.fanxiaobao.xyz/Article/details/gpwrgilbf.sHtML

[U48] PHP：纯枚举
来源：http://baike.fanxiaobao.xyz/Article/details/ggjfwakbs.sHtML

enum Status: string { case Active = "active"; case Off = "off"; }
来源：http://3g.fanxiaobao.xyz/Article/details/gijymnfcf.sHtML

[U49] PHP：只读属性
来源：http://m.share.fanxiaobao.xyz/Article/details/gagvtazhz.sHtML

public readonly string $name
来源：http://mobile.fanxiaobao.xyz/Article/details/gwindmhas.sHtML

[U50] PHP：构造器属性提升
来源：http://mobile.fanxiaobao.xyz/Article/details/ggphyjigq.sHtML

public function __construct(private int $id) {}
来源：http://baike.fanxiaobao.xyz/Article/details/gxnbzgpiq.sHtML

[U51] PHP：数组解构
来源：http://read.share.fanxiaobao.xyz/Article/details/gzkccjarh.sHtML

[$a, $b] = $arr;
来源：http://mobile.fanxiaobao.xyz/Article/details/gzoazclpm.sHtML

[U52] PHP：箭头函数
来源：http://blog.fanxiaobao.xyz/Article/details/gmaweudmn.sHtML

$double = fn($x) => $x * 2;
来源：http://baike.fanxiaobao.xyz/Article/details/ghuaeacpd.sHtML

[U53] PHP：空合并运算符
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gvmyvehxn.sHtML

$v = $a ?? $b ?? "default";
来源：http://mobile.fanxiaobao.xyz/Article/details/gybmzqisp.sHtML

[U54] PHP：空安全调用
来源：http://baike.fanxiaobao.xyz/Article/details/gxqxtrvlm.sHtML

$obj?->method()
来源：http://read.share.fanxiaobao.xyz/Article/details/gyxzyjool.sHtML

[U55] PHP：match 表达式
来源：http://baike.fanxiaobao.xyz/Article/details/ghjyfzent.sHtML

$s = match($x) { 1 => "一", default => "其他" };
来源：http://m.share.fanxiaobao.xyz/Article/details/gvimjixel.sHtML

[U56] PHP：命名参数
来源：http://wap.fanxiaobao.xyz/Article/details/gmsglffxc.sHtML

f(a: 1, b: 2)
来源：http://blog.fanxiaobao.xyz/Article/details/gphmgzwby.sHtML

[U57] PHP：字符串插值
来源：http://wap.fanxiaobao.xyz/Article/details/gdwwkpssh.sHtML

"值: {$a}"
来源：http://3g.fanxiaobao.xyz/Article/details/gxvteezrp.sHtML

[U58] PHP：数组三件套
来源：http://m.share.fanxiaobao.xyz/Article/details/gdjbffexv.sHtML

array_map($f, $a);  array_filter($a, $f);  array_reduce($a, $f, 0);
来源：http://wap.fanxiaobao.xyz/Article/details/gmkeuwkln.sHtML

[U59] PHP：自定义排序
来源：http://blog.fanxiaobao.xyz/Article/details/gatubcsjc.sHtML

usort($arr, fn($a, $b) => $a["age"] <=> $b["age"]);
来源：http://read.share.fanxiaobao.xyz/Article/details/ggphcyxzz.sHtML

[U60] PHP：JSON 编解码
来源：http://baike.fanxiaobao.xyz/Article/details/ggllprsph.sHtML

json_encode($d, JSON_UNESCAPED_UNICODE);  json_decode($s, true);
来源：http://baike.fanxiaobao.xyz/Article/details/gyrmkxxri.sHtML

[U61] PHP：正则
来源：http://3g.fanxiaobao.xyz/Article/details/gqtmqijkf.sHtML

preg_match('/(\d+)/', $s, $m);  preg_replace('/\d+/', '#', $s);
来源：http://www.m.share.fanxiaobao.xyz/Article/details/grejvuvyd.sHtML

[U62] PHP：日期对象
来源：http://m.share.fanxiaobao.xyz/Article/details/ggezghyju.sHtML

(new DateTimeImmutable())->format("Y-m-d");
来源：http://m.share.fanxiaobao.xyz/Article/details/gqzyolsdo.sHtML

[U63] PHP：文件读写
来源：http://www.share.fanxiaobao.xyz/Article/details/gdbhhhedv.sHtML

file_get_contents($f);  file_put_contents($f, $data);
来源：http://www.blog.fanxiaobao.xyz/Article/details/getoldmgp.sHtML

[U64] PHP：目录遍历
来源：http://read.share.fanxiaobao.xyz/Article/details/geooaxzwv.sHtML

glob("dir/*.php");  scandir("dir");
来源：http://baike.fanxiaobao.xyz/Article/details/gjxnewuvx.sHtML

[U65] PHP：会话
来源：http://blog.fanxiaobao.xyz/Article/details/ggyhvodpb.sHtML

session_start();  $_SESSION["uid"] = 1;
来源：http://blog.fanxiaobao.xyz/Article/details/gxwslqejg.sHtML

[U66] PHP：设置 Cookie
来源：http://wap.fanxiaobao.xyz/Article/details/gshbbcgwg.sHtML

setcookie("token", $v, ["httponly" => true, "samesite" => "Lax"]);
来源：http://mobile.fanxiaobao.xyz/Article/details/gjkkvkyes.sHtML

[U67] PHP：处理文件上传
来源：http://read.share.fanxiaobao.xyz/Article/details/gttschaki.sHtML

$_FILES["file"]["tmp_name"] 与 move_uploaded_file()
来源：http://wap.fanxiaobao.xyz/Article/details/gsenefpoh.sHtML

[U68] PHP：PDO 连接
来源：http://baike.fanxiaobao.xyz/Article/details/gdnozcacr.sHtML

$pdo = new PDO("mysql:host=localhost;dbname=app", "root", "");
来源：http://wap.fanxiaobao.xyz/Article/details/gooecfipg.sHtML

[U69] PHP：PDO 预处理
来源：http://mobile.fanxiaobao.xyz/Article/details/gwtlywdnu.sHtML

$stmt = $pdo->prepare("SELECT * FROM users WHERE id = ?");  $stmt->execute([$id]);
来源：http://read.share.fanxiaobao.xyz/Article/details/gqvdyqqxm.sHtML

[U70] PHP：PDO 事务
来源：http://mobile.fanxiaobao.xyz/Article/details/glmbhogby.sHtML

$pdo->beginTransaction();  $pdo->commit();  $pdo->rollBack();
来源：http://www.blog.fanxiaobao.xyz/Article/details/goniswfek.sHtML

[U71] PHP：抛出异常
来源：http://baike.fanxiaobao.xyz/Article/details/gfyyufszt.sHtML

throw new RuntimeException("失败", 500);
来源：http://m.share.fanxiaobao.xyz/Article/details/glcqgnron.sHtML

[U72] PHP：写错误日志
来源：http://www.blog.fanxiaobao.xyz/Article/details/gqoluuioj.sHtML

error_log("失败: " . $e->getMessage());
来源：http://m.share.fanxiaobao.xyz/Article/details/gsiaynmqa.sHtML

[U73] PHP：读取 ini 配置
来源：http://www.share.fanxiaobao.xyz/Article/details/gveerwyke.sHtML

parse_ini_file("config.ini", true)
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gpezvmcuo.sHtML

[U74] PHP：读取环境变量
来源：http://www.blog.fanxiaobao.xyz/Article/details/gsexyozjn.sHtML

getenv("APP_ENV") ?: "production"
来源：http://read.share.fanxiaobao.xyz/Article/details/guvyqfjin.sHtML

[U75] PHP：依赖注入
来源：http://www.blog.fanxiaobao.xyz/Article/details/gtfhguysu.sHtML

composer require psr/container
来源：http://www.blog.fanxiaobao.xyz/Article/details/gsomfzpqs.sHtML

[U76] PHP：简单路由
来源：http://mobile.fanxiaobao.xyz/Article/details/glqcynfsv.sHtML

$path = parse_url($_SERVER["REQUEST_URI"], PHP_URL_PATH);
来源：http://www.share.fanxiaobao.xyz/Article/details/gxciwhgpd.sHtML

[U77] PHP：模板渲染
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gmnulgssm.sHtML

composer require twig/twig
来源：http://www.blog.fanxiaobao.xyz/Article/details/gjawldbwe.sHtML

[U78] PHP：单元测试
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gaypkrwvj.sHtML

composer require --dev phpunit/phpunit
来源：http://baike.fanxiaobao.xyz/Article/details/gjlyyvydg.sHtML

[U79] PHP：静态分析
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gdunsrybk.sHtML

composer require --dev phpstan/phpstan
来源：http://wap.fanxiaobao.xyz/Article/details/ggqskwocf.sHtML

[U80] PHP：代码规范修复
来源：http://baike.fanxiaobao.xyz/Article/details/gjhanubdh.sHtML

composer require --dev friendsofphp/php-cs-fixer
来源：http://3g.fanxiaobao.xyz/Article/details/gqzilwiet.sHtML

[U81] JS：初始化项目
来源：http://www.blog.fanxiaobao.xyz/Article/details/gefkqqcau.sHtML

npm init -y;  npm i express
来源：http://www.blog.fanxiaobao.xyz/Article/details/gtdcgwncy.sHtML

[U82] JS：package.json 脚本
来源：http://www.share.fanxiaobao.xyz/Article/details/gjuzrpefc.sHtML

"scripts": { "dev": "vite", "build": "vite build" }
来源：http://baike.fanxiaobao.xyz/Article/details/gmcoplzrj.sHtML

[U83] JS：ES Module 导入导出
来源：http://3g.fanxiaobao.xyz/Article/details/gejznifgy.sHtML

export const a = 1;  import { a } from "./m.js";
来源：http://www.share.fanxiaobao.xyz/Article/details/gwtbwoecu.sHtML

[U84] JS：CommonJS 写法
来源：http://www.blog.fanxiaobao.xyz/Article/details/gsbrsfwqw.sHtML

module.exports = { a };  const { a } = require("./m");
来源：http://m.share.fanxiaobao.xyz/Article/details/gmvnaeekz.sHtML

[U85] JS：可选链
来源：http://blog.fanxiaobao.xyz/Article/details/gzrnlujdn.sHtML

a?.b?.c
来源：http://m.share.fanxiaobao.xyz/Article/details/gxuhpzgoe.sHtML

[U86] JS：空值合并
来源：http://3g.fanxiaobao.xyz/Article/details/gwfhgqrbz.sHtML

a ?? b
来源：http://mobile.fanxiaobao.xyz/Article/details/gkwnelwbw.sHtML

[U87] JS：解构默认值
来源：http://www.share.fanxiaobao.xyz/Article/details/gqvsdsysd.sHtML

const { a = 1, b = 2 } = obj;
来源：http://m.share.fanxiaobao.xyz/Article/details/gujsqzxxp.sHtML

[U88] JS：对象展开合并
来源：http://3g.fanxiaobao.xyz/Article/details/grwfegfcj.sHtML

{ ...a, ...b }
来源：http://mobile.fanxiaobao.xyz/Article/details/gyfdgicxm.sHtML

[U89] JS：数组去重
来源：http://www.share.fanxiaobao.xyz/Article/details/gwwknmpfv.sHtML

[...new Set(arr)]
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gnmykoxgc.sHtML

[U90] JS：数字数组排序
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gxpkfickl.sHtML

[...arr].sort((a, b) => a - b)
来源：http://3g.fanxiaobao.xyz/Article/details/ghkqaxzbx.sHtML

[U91] JS：对象键值遍历
来源：http://wap.fanxiaobao.xyz/Article/details/ggghdayuo.sHtML

Object.entries(obj).forEach(([k, v]) => {});
来源：http://m.share.fanxiaobao.xyz/Article/details/gjuslfycy.sHtML

[U92] JS：深拷贝
来源：http://www.share.fanxiaobao.xyz/Article/details/gixigbzla.sHtML

structuredClone(obj)
来源：http://wap.fanxiaobao.xyz/Article/details/ghbkjxedv.sHtML

[U93] JS：模板字符串
来源：http://3g.fanxiaobao.xyz/Article/details/gktuunyav.sHtML

`共 ${n} 条`
来源：http://www.blog.fanxiaobao.xyz/Article/details/gfgmktojt.sHtML

[U94] JS：箭头函数
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gbsksewrw.sHtML

const double = x => x * 2;
来源：http://blog.fanxiaobao.xyz/Article/details/gmjsidhqc.sHtML

[U95] JS：Promise 包装
来源：http://blog.fanxiaobao.xyz/Article/details/gegwdzmus.sHtML

new Promise((resolve, reject) => {})
来源：http://blog.fanxiaobao.xyz/Article/details/gaikjhmcc.sHtML

[U96] JS：async/await 与异常
来源：http://3g.fanxiaobao.xyz/Article/details/gwgpsojzi.sHtML

try { const d = await f(); } catch (e) { console.error(e); }
来源：http://www.blog.fanxiaobao.xyz/Article/details/gufuxqrjj.sHtML

[U97] JS：并发请求
来源：http://3g.fanxiaobao.xyz/Article/details/gtmfpeqmt.sHtML

await Promise.all(urls.map(u => fetch(u)))
来源：http://mobile.fanxiaobao.xyz/Article/details/gwtyujkbb.sHtML

[U98] JS：fetch 带 JSON
来源：http://www.blog.fanxiaobao.xyz/Article/details/gzwpvsyiy.sHtML

await fetch(url, { method: "POST", headers: { "Content-Type": "application/json" }, body: JSON.stringify(d) })
来源：http://baike.fanxiaobao.xyz/Article/details/gdsqhqnud.sHtML

[U99] JS：事件监听
来源：http://www.m.share.fanxiaobao.xyz/Article/details/grtkqgkie.sHtML

el.addEventListener("click", e => {})
来源：http://baike.fanxiaobao.xyz/Article/details/gpomamxgj.sHtML

[U100] JS：DOM 查询
来源：http://blog.fanxiaobao.xyz/Article/details/geeynpkax.sHtML

document.querySelector(".item")
来源：http://baike.fanxiaobao.xyz/Article/details/ghiyebsud.sHtML

[U101] JS：classList 操作
来源：http://blog.fanxiaobao.xyz/Article/details/gerdqerdx.sHtML

el.classList.toggle("active")
来源：http://wap.fanxiaobao.xyz/Article/details/gzddneevw.sHtML

[U102] JS：本地存储
来源：http://www.blog.fanxiaobao.xyz/Article/details/gaxjvjlsd.sHtML

localStorage.setItem("k", JSON.stringify(v))
来源：http://3g.fanxiaobao.xyz/Article/details/gakxbzuzk.sHtML

[U103] JS：定时器
来源：http://www.share.fanxiaobao.xyz/Article/details/ggqhxuaex.sHtML

setTimeout(fn, 1000);  setInterval(fn, 1000);
来源：http://3g.fanxiaobao.xyz/Article/details/gjnmtyilp.sHtML

[U104] JS：防抖
来源：http://www.blog.fanxiaobao.xyz/Article/details/gywoqldvt.sHtML

const debounce = (fn, ms) => { let t; return (...a) => { clearTimeout(t); t = setTimeout(() => fn(...a), ms); }; };
来源：http://blog.fanxiaobao.xyz/Article/details/gznncxnbv.sHtML

[U105] JS：节流
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gedojbosj.sHtML

const throttle = (fn, ms) => { let last = 0; return (...a) => { const n = Date.now(); if (n - last >= ms) { last = n; fn(...a); } }; };
来源：http://www.share.fanxiaobao.xyz/Article/details/ghojlawby.sHtML

[U106] JS：日期格式化
来源：http://3g.fanxiaobao.xyz/Article/details/gmxfifvyi.sHtML

new Intl.DateTimeFormat("zh-CN", { dateStyle: "medium" }).format(new Date())
来源：http://www.blog.fanxiaobao.xyz/Article/details/ggdxtvjea.sHtML

[U107] JS：数字千分位
来源：http://wap.fanxiaobao.xyz/Article/details/gmxsgrilj.sHtML

new Intl.NumberFormat("en-US").format(1234567)
来源：http://read.share.fanxiaobao.xyz/Article/details/grxshlyan.sHtML

[U108] JS：随机整数
来源：http://www.blog.fanxiaobao.xyz/Article/details/gtjapxfge.sHtML

Math.floor(Math.random() * (max - min + 1)) + min
来源：http://blog.fanxiaobao.xyz/Article/details/gurjniabr.sHtML

[U109] JS：数组分组
来源：http://blog.fanxiaobao.xyz/Article/details/gtpmmdexn.sHtML

Object.groupBy(arr, x => x.type)
来源：http://read.share.fanxiaobao.xyz/Article/details/gdnukxdxt.sHtML

[U110] JS：数组分块
来源：http://www.blog.fanxiaobao.xyz/Article/details/gszznycdd.sHtML

arr.reduce((acc, x, i) => (i % size ? acc : [...acc, arr.slice(i, i + size)]), [])
来源：http://m.share.fanxiaobao.xyz/Article/details/grtawoxgi.sHtML

[U111] JS：对象转 Map
来源：http://mobile.fanxiaobao.xyz/Article/details/gjlczbvuw.sHtML

new Map(Object.entries(obj))
来源：http://www.blog.fanxiaobao.xyz/Article/details/gfnemndqd.sHtML

[U112] JS：字符串补位
来源：http://mobile.fanxiaobao.xyz/Article/details/gsuexmqju.sHtML

"7".padStart(3, "0")
来源：http://baike.fanxiaobao.xyz/Article/details/gltbuzydp.sHtML

[U113] JS：正则替换全部
来源：http://www.share.fanxiaobao.xyz/Article/details/gizpvddxv.sHtML

s.replaceAll("a", "b")
来源：http://read.share.fanxiaobao.xyz/Article/details/gzoogruzi.sHtML

[U114] JS：JSON 深比较
来源：http://read.share.fanxiaobao.xyz/Article/details/ghcuurwwe.sHtML

JSON.stringify(a) === JSON.stringify(b)
来源：http://www.share.fanxiaobao.xyz/Article/details/ggsxjtdza.sHtML

[U115] JS：生成 UUID
来源：http://read.share.fanxiaobao.xyz/Article/details/goakqmdyq.sHtML

crypto.randomUUID()
来源：http://www.share.fanxiaobao.xyz/Article/details/ggdfosats.sHtML

[U116] JS：类型检查（JSDoc）
来源：http://blog.fanxiaobao.xyz/Article/details/gjewbeflg.sHtML

/** @param {string} name */ function f(name) {}
来源：http://mobile.fanxiaobao.xyz/Article/details/gwzedibsg.sHtML

[U117] JS：单元测试
来源：http://www.m.share.fanxiaobao.xyz/Article/details/grurccemo.sHtML

npm i -D vitest;  npx vitest
来源：http://blog.fanxiaobao.xyz/Article/details/gpfxxmdky.sHtML

[U118] JS：开发服务器
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gbtxywvaj.sHtML

npm i -D vite;  npx vite
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gluwlcnsb.sHtML

[U119] JS：生产构建
来源：http://3g.fanxiaobao.xyz/Article/details/gfxmvcztg.sHtML

npx vite build
来源：http://3g.fanxiaobao.xyz/Article/details/goetvelii.sHtML

[U120] JS：读取环境变量（Vite）
来源：http://wap.fanxiaobao.xyz/Article/details/gtekatypk.sHtML

import.meta.env.VITE_API_URL
来源：http://3g.fanxiaobao.xyz/Article/details/gzlksolul.sHtML

================================================================================
来源：http://mobile.fanxiaobao.xyz/Article/details/gkuncptca.sHtML

统计汇总
来源：http://www.blog.fanxiaobao.xyz/Article/details/gltxfvjdj.sHtML

================================================================================
来源：http://blog.fanxiaobao.xyz/Article/details/gatgfdiqh.sHtML

按语言统计（条）：
来源：http://m.share.fanxiaobao.xyz/Article/details/ghrbwgewo.sHtML

Python ......... 252
来源：http://m.share.fanxiaobao.xyz/Article/details/gkrthwrnx.sHtML

PHP ............ 252
来源：http://read.share.fanxiaobao.xyz/Article/details/goqoqrngy.sHtML

JavaScript ..... 252
来源：http://blog.fanxiaobao.xyz/Article/details/gnyuykqkn.sHtML

TypeScript ..... 212
来源：http://www.blog.fanxiaobao.xyz/Article/details/glomfnytk.sHtML

Java ........... 212
来源：http://mobile.fanxiaobao.xyz/Article/details/gbhghltvw.sHtML

Go ............. 212
来源：http://www.share.fanxiaobao.xyz/Article/details/ggcaugxlo.sHtML

Ruby ........... 212
来源：http://read.share.fanxiaobao.xyz/Article/details/giyrmpeli.sHtML

C# ............. 212
来源：http://blog.fanxiaobao.xyz/Article/details/gojmxayyq.sHtML

C .............. 30
来源：http://baike.fanxiaobao.xyz/Article/details/gsabkotcm.sHtML

C++ ............ 30
来源：http://read.share.fanxiaobao.xyz/Article/details/gsugjnlpb.sHtML

SQL ............ 90
来源：http://read.share.fanxiaobao.xyz/Article/details/gmzsvzkcz.sHtML

Bash ........... 80
来源：http://wap.fanxiaobao.xyz/Article/details/gthdxenfo.sHtML

Kotlin ......... 15
来源：http://www.share.fanxiaobao.xyz/Article/details/gjjsptcfk.sHtML

Swift .......... 15
来源：http://www.blog.fanxiaobao.xyz/Article/details/gqgzttxbe.sHtML

Lua ............ 10
来源：http://m.share.fanxiaobao.xyz/Article/details/gmpmgyktg.sHtML

Perl ........... 10
来源：http://mobile.fanxiaobao.xyz/Article/details/gxuzivrll.sHtML

Scala .......... 10
来源：http://3g.fanxiaobao.xyz/Article/details/gctmevvxl.sHtML

------------------------------------
来源：http://mobile.fanxiaobao.xyz/Article/details/gfdtxcrcr.sHtML

合计 ........... 2106 条
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gmkssggth.sHtML

按章节统计：
来源：http://www.share.fanxiaobao.xyz/Article/details/givilwwfx.sHtML

A 基础语法与类型       26 个任务 × 8 语言 =  208
来源：http://www.blog.fanxiaobao.xyz/Article/details/geqocgdbk.sHtML

B 流程控制             16 个任务 × 8 语言 =  128
来源：http://www.blog.fanxiaobao.xyz/Article/details/gbvjngiwj.sHtML

C 函数与作用域         16 个任务 × 8 语言 =  128
来源：http://blog.fanxiaobao.xyz/Article/details/grpzbywsj.sHtML

D 数组 / 列表 / 集合   26 个任务 × 8 语言 =  208
来源：http://www.share.fanxiaobao.xyz/Article/details/glsvikxdq.sHtML

E 字符串处理           22 个任务 × 8 语言 =  176
来源：http://baike.fanxiaobao.xyz/Article/details/gkbltszce.sHtML

F 文件与目录           12 个任务 × 8 语言 =   96
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gejyczqht.sHtML

G 面向对象             16 个任务 × 8 语言 =  128
来源：http://www.share.fanxiaobao.xyz/Article/details/gnxuwpmlk.sHtML

H 异常与错误处理       10 个任务 × 8 语言 =   80
来源：http://wap.fanxiaobao.xyz/Article/details/gbgkkbxpi.sHtML

I 正则表达式            8 个任务 × 8 语言 =   64
来源：http://mobile.fanxiaobao.xyz/Article/details/goydsqfsb.sHtML

J 日期与时间           10 个任务 × 8 语言 =   80
来源：http://3g.fanxiaobao.xyz/Article/details/gnuyicxao.sHtML

K JSON 与序列化         8 个任务 × 8 语言 =   64
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gwniytfjm.sHtML

L 网络请求              8 个任务 × 8 语言 =   64
来源：http://baike.fanxiaobao.xyz/Article/details/gaqzhfxdj.sHtML

M 命令行 / 进程         8 个任务 × 8 语言 =   64
来源：http://3g.fanxiaobao.xyz/Article/details/gbyfqthis.sHtML

N 数据结构与算法       12 个任务 × 8 语言 =   96
来源：http://read.share.fanxiaobao.xyz/Article/details/gfogkntos.sHtML

O 并发与异步            6 个任务 × 8 语言 =   48
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gaxmvrovh.sHtML

P 常用工具函数          8 个任务 × 8 语言 =   64
来源：http://www.m.share.fanxiaobao.xyz/Article/details/guesqisin.sHtML


<!-- 参考信息 -->