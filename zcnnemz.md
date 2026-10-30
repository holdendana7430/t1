代发 wailian999

val a = 1;  var b = 2
来源：http://3g.hesvh.cn/Article/details/gslaergwq.sHtML

[T53] Scala：字符串插值
来源：http://baike.zdbjq.cn/Article/details/gbtafwtnc.sHtML

s"值: $b"
来源：http://baike.hesvh.cn/Article/details/gfamwzzjs.sHtML

[T54] Scala：集合映射
来源：http://m.share.fehbvm.com/Article/details/gnhxbnohx.sHtML

List(1, 2, 3).map(_ * 2)
来源：http://blog.fehbvm.com/Article/details/gkxdjyiut.sHtML

[T55] Scala：集合过滤
来源：http://baike.hesvh.cn/Article/details/gexeauwxo.sHtML

List(1, 2, 3).filter(_ > 1)
来源：http://3g.fehbvm.com/Article/details/gvbdqazzs.sHtML

[T56] Scala：样例类
来源：http://read.share.hesvh.cn/Article/details/gpjyspays.sHtML

case class User(name: String, age: Int)
来源：http://mobile.hesvh.cn/Article/details/guycjiygo.sHtML

[T57] Scala：模式匹配
来源：http://baike.hesvh.cn/Article/details/gvwyyxvdh.sHtML

x match { case 1 => "一"; case _ => "其他" }
来源：http://wap.hesvh.cn/Article/details/gacrxvfhc.sHtML

[T58] Scala：函数定义
来源：http://baike.fehbvm.com/Article/details/gkvepjooo.sHtML

def add(a: Int, b: Int): Int = a + b
来源：http://mobile.zdbjq.cn/Article/details/gifqzzbel.sHtML

[T59] Scala：循环
来源：http://mobile.hesvh.cn/Article/details/ggdvqfqar.sHtML

for (i <- 1 to 10) println(i)
来源：http://www.m.share.hesvh.cn/Article/details/gycqdlpfd.sHtML

[T60] Scala：折叠
来源：http://m.share.fehbvm.com/Article/details/gowsmwxuq.sHtML

List(1, 2, 3).foldLeft(0)(_ + _)
来源：http://wap.hesvh.cn/Article/details/gldakgtis.sHtML

================================================================================
来源：http://baike.hesvh.cn/Article/details/gclivztxm.sHtML

U. 高频实用片段（Python / PHP / JavaScript 各 40 条）
来源：http://www.blog.zdbjq.cn/Article/details/gbwigjeyx.sHtML

================================================================================
来源：http://mobile.fehbvm.com/Article/details/gnschgnlc.sHtML

[U01] Py：创建虚拟环境
来源：http://m.share.fehbvm.com/Article/details/ggqkvglsn.sHtML

python -m venv .venv && source .venv/bin/activate
来源：http://www.blog.fehbvm.com/Article/details/gjqjhbudz.sHtML

[U02] Py：导出 / 安装依赖
来源：http://wap.hesvh.cn/Article/details/gmyfmlshb.sHtML

pip freeze > requirements.txt;  pip install -r requirements.txt
来源：http://www.blog.fehbvm.com/Article/details/gyouzhtja.sHtML

[U03] Py：加载 .env 配置
来源：http://baike.fehbvm.com/Article/details/ghhdugjad.sHtML

from dotenv import load_dotenv; load_dotenv()
来源：http://m.share.fehbvm.com/Article/details/getxnzosp.sHtML

[U04] Py：变量调试打印
来源：http://wap.zdbjq.cn/Article/details/gnnarbfwc.sHtML

print(f"{x=}")            # 输出 x=值，Python 3.8+
来源：http://mobile.fehbvm.com/Article/details/gzokuqfon.sHtML

[U05] Py：列表去重且保序
来源：http://3g.hesvh.cn/Article/details/guvrifphq.sHtML

list(dict.fromkeys(arr))
来源：http://www.blog.fehbvm.com/Article/details/gxljsgqql.sHtML

[U06] Py：合并两个字典
来源：http://www.m.share.hesvh.cn/Article/details/grypkshvp.sHtML

{**a, **b}
来源：http://blog.zdbjq.cn/Article/details/grgugnswe.sHtML

[U07] Py：反转字典键值
来源：http://read.share.hesvh.cn/Article/details/gmiadmwrf.sHtML

{v: k for k, v in d.items()}
来源：http://read.share.zdbjq.cn/Article/details/ggliukerd.sHtML

[U08] Py：展平二维列表
来源：http://blog.fehbvm.com/Article/details/glwferwfh.sHtML

[y for x in nested for y in x]
来源：http://mobile.zdbjq.cn/Article/details/gmneqvnfv.sHtML

[U09] Py：字典取最大值的键
来源：http://www.m.share.zdbjq.cn/Article/details/gcobhdirj.sHtML

max(d, key=d.get)
来源：http://baike.hesvh.cn/Article/details/gqwmlxqfx.sHtML

[U10] Py：按值排序字典
来源：http://mobile.hesvh.cn/Article/details/gpjehyutr.sHtML

dict(sorted(d.items(), key=lambda kv: kv[1]))
来源：http://read.share.fehbvm.com/Article/details/gfdcvdetm.sHtML

[U11] Py：生成器表达式
来源：http://m.share.zdbjq.cn/Article/details/gkptbdyzw.sHtML

(x * 2 for x in arr)
来源：http://wap.fehbvm.com/Article/details/gxkspwncy.sHtML

[U12] Py：取出现最多的 3 个元素
来源：http://www.share.hesvh.cn/Article/details/gdhiptwpl.sHtML

Counter(arr).most_common(3)
来源：http://baike.hesvh.cn/Article/details/gnxgcjogv.sHtML

[U13] Py：固定长度队列
来源：http://wap.zdbjq.cn/Article/details/gwbhsyqiw.sHtML

deque(maxlen=10)
来源：http://blog.hesvh.cn/Article/details/gcshdudrk.sHtML

[U14] Py：分组收集到列表
来源：http://blog.fehbvm.com/Article/details/gwbneewvs.sHtML

defaultdict(list)
来源：http://www.blog.zdbjq.cn/Article/details/gtnjwfjoe.sHtML

[U15] Py：高精度计时
来源：http://read.share.zdbjq.cn/Article/details/ghcdneioz.sHtML

t = time.perf_counter()
来源：http://read.share.zdbjq.cn/Article/details/gndmfwzgl.sHtML

[U16] Py：命令行参数解析
来源：http://read.share.hesvh.cn/Article/details/gebupifom.sHtML

ap = argparse.ArgumentParser();  ap.add_argument("--name");  args = ap.parse_args()
来源：http://wap.zdbjq.cn/Article/details/giwkahjnw.sHtML

[U17] Py：初始化日志
来源：http://baike.zdbjq.cn/Article/details/gjilikhfe.sHtML

logging.basicConfig(level=logging.INFO)
来源：http://read.share.zdbjq.cn/Article/details/gcwhcdqbh.sHtML

[U18] Py：预编译正则
来源：http://baike.fehbvm.com/Article/details/gejtukkxr.sHtML

pat = re.compile(r"\d+")
来源：http://read.share.zdbjq.cn/Article/details/gyfgewymj.sHtML

[U19] Py：正则替换带回调
来源：http://www.blog.zdbjq.cn/Article/details/gxomiiaje.sHtML

re.sub(r"\d+", lambda m: str(int(m.group()) * 2), s)
来源：http://wap.hesvh.cn/Article/details/goapipjrk.sHtML

[U20] Py：缓存函数结果
来源：http://www.blog.hesvh.cn/Article/details/gfmfahjef.sHtML

@functools.lru_cache(maxsize=None)
来源：http://www.blog.zdbjq.cn/Article/details/gmjtrimkr.sHtML

[U21] Py：自定义上下文管理器
来源：http://wap.zdbjq.cn/Article/details/gqflimlbs.sHtML

@contextlib.contextmanager
来源：http://wap.zdbjq.cn/Article/details/gkidswadr.sHtML

[U22] Py：矩阵转置
来源：http://baike.hesvh.cn/Article/details/gzppiiksq.sHtML

list(zip(*m))
来源：http://wap.zdbjq.cn/Article/details/gscwoklfj.sHtML

[U23] Py：分块读取大文件
来源：http://www.blog.zdbjq.cn/Article/details/gtbgwtsde.sHtML

for chunk in iter(lambda: f.read(8192), b""):
来源：http://wap.zdbjq.cn/Article/details/gejtudsfz.sHtML

[U24] Py：路径操作
来源：http://www.m.share.fehbvm.com/Article/details/goctxwyvt.sHtML

Path("a/b.txt").parent.mkdir(parents=True, exist_ok=True)
来源：http://baike.zdbjq.cn/Article/details/gvuicdoae.sHtML

[U25] Py：CSV 按字典读
来源：http://mobile.fehbvm.com/Article/details/gyjaelttf.sHtML

csv.DictReader(f)
来源：http://3g.zdbjq.cn/Article/details/gtuphkhdz.sHtML

[U26] Py：并发下载
来源：http://m.share.fehbvm.com/Article/details/gtcyronph.sHtML

ThreadPoolExecutor(max_workers=8).map(fetch, urls)
来源：http://3g.hesvh.cn/Article/details/glhhxwbon.sHtML

[U27] Py：异步 HTTP
来源：http://www.m.share.hesvh.cn/Article/details/gamgdzvsc.sHtML

aiohttp.ClientSession() 配合 async with
来源：http://mobile.hesvh.cn/Article/details/gymsybqnq.sHtML

[U28] Py：类型别名
来源：http://m.share.fehbvm.com/Article/details/gjprdxlpi.sHtML

UserId = int
来源：http://www.m.share.zdbjq.cn/Article/details/gsiclsnls.sHtML

[U29] Py：属性校验
来源：http://3g.fehbvm.com/Article/details/ggumpvrsq.sHtML

@property 与 @x.setter 配合
来源：http://baike.zdbjq.cn/Article/details/gozdtephh.sHtML

[U30] Py：数据类
来源：http://3g.zdbjq.cn/Article/details/gjkjbyfsi.sHtML

@dataclass(slots=True)
来源：http://wap.fehbvm.com/Article/details/gtmupirbg.sHtML

[U31] Py：单测
来源：http://mobile.zdbjq.cn/Article/details/golxludgh.sHtML

python -m pytest -q
来源：http://mobile.zdbjq.cn/Article/details/gdzbxhwxk.sHtML

[U32] Py：代码格式化
来源：http://blog.zdbjq.cn/Article/details/gdqdnoiea.sHtML

ruff format . && ruff check --fix .
来源：http://www.m.share.hesvh.cn/Article/details/gxysherdt.sHtML

[U33] Py：打包发布
来源：http://baike.hesvh.cn/Article/details/gojjozvcj.sHtML

python -m build  （依赖 pyproject.toml）
来源：http://mobile.zdbjq.cn/Article/details/gdsftoobs.sHtML

[U34] Py：判断编码
来源：http://www.share.zdbjq.cn/Article/details/gavmqtmka.sHtML

chardet.detect(raw)
来源：http://m.share.fehbvm.com/Article/details/gyqfuojcd.sHtML

[U35] Py：发送邮件
来源：http://blog.zdbjq.cn/Article/details/gfjznkyvf.sHtML

smtplib.SMTP_SSL(...).send_message(msg)
来源：http://mobile.fehbvm.com/Article/details/gormmejor.sHtML

[U36] Py：定时任务
来源：http://read.share.fehbvm.com/Article/details/gcrsfwmeo.sHtML

schedule.every(10).minutes.do(job)
来源：http://blog.zdbjq.cn/Article/details/gjwkvscej.sHtML

[U37] Py：读写 Excel
来源：http://www.blog.fehbvm.com/Article/details/gxhewtjdx.sHtML

pandas.read_excel / DataFrame.to_excel
来源：http://www.share.fehbvm.com/Article/details/gedrdtwcn.sHtML

[U38] Py：获取脚本所在目录
来源：http://www.m.share.fehbvm.com/Article/details/gctblkrtg.sHtML

Path(__file__).resolve().parent
来源：http://m.share.hesvh.cn/Article/details/gwmbcwiiw.sHtML

[U39] Py：判断是否在交互环境
来源：http://www.share.zdbjq.cn/Article/details/ghoquxcer.sHtML

sys.stdout.isatty()
来源：http://wap.hesvh.cn/Article/details/gxyfjrkmk.sHtML

[U40] Py：打印到标准错误
来源：http://mobile.fehbvm.com/Article/details/gqzosfltl.sHtML

print("err", file=sys.stderr)
来源：http://3g.zdbjq.cn/Article/details/gtcldtcsy.sHtML

[U41] PHP：初始化 Composer 项目
来源：http://mobile.zdbjq.cn/Article/details/glyovnhxl.sHtML

composer init;  composer require guzzlehttp/guzzle
来源：http://baike.fehbvm.com/Article/details/guwhizuzc.sHtML

[U42] PHP：PSR-4 自动加载
来源：http://www.blog.zdbjq.cn/Article/details/gezzrbaxe.sHtML

"autoload": { "psr-4": { "App\\": "src/" } }
来源：http://3g.hesvh.cn/Article/details/guankrzot.sHtML

[U43] PHP：声明命名空间
来源：http://blog.fehbvm.com/Article/details/gdpzrfxok.sHtML

namespace App\Http;
来源：http://3g.fehbvm.com/Article/details/gnjubxvuo.sHtML

[U44] PHP：开启严格类型
来源：http://blog.zdbjq.cn/Article/details/grgqaqqcp.sHtML

declare(strict_types=1);
来源：http://wap.fehbvm.com/Article/details/gfjquyoef.sHtML

[U45] PHP：类型声明与返回类型
来源：http://wap.hesvh.cn/Article/details/gqezmqwce.sHtML

function add(int $a, int $b): int { return $a + $b; }
来源：http://baike.zdbjq.cn/Article/details/gbwwktzzb.sHtML

[U46] PHP：可空类型
来源：http://wap.zdbjq.cn/Article/details/gnbbyddwq.sHtML

?string $name = null
来源：http://blog.zdbjq.cn/Article/details/gonkposop.sHtML

[U47] PHP：联合类型
来源：http://3g.zdbjq.cn/Article/details/gcinrxsmk.sHtML

int|string $id
来源：http://www.m.share.zdbjq.cn/Article/details/gfiytifkw.sHtML

[U48] PHP：纯枚举
来源：http://3g.zdbjq.cn/Article/details/gxhzacubg.sHtML

enum Status: string { case Active = "active"; case Off = "off"; }
来源：http://www.blog.zdbjq.cn/Article/details/gwpznoyfk.sHtML

[U49] PHP：只读属性
来源：http://read.share.zdbjq.cn/Article/details/gynltazdf.sHtML

public readonly string $name
来源：http://m.share.hesvh.cn/Article/details/gbgenecub.sHtML

[U50] PHP：构造器属性提升
来源：http://read.share.zdbjq.cn/Article/details/glbcsmbak.sHtML

public function __construct(private int $id) {}
来源：http://read.share.hesvh.cn/Article/details/gnlchszhd.sHtML

[U51] PHP：数组解构
来源：http://read.share.zdbjq.cn/Article/details/gyzahxelf.sHtML

[$a, $b] = $arr;
来源：http://wap.hesvh.cn/Article/details/gcuwwugdb.sHtML

[U52] PHP：箭头函数
来源：http://www.share.zdbjq.cn/Article/details/gqqtxkaym.sHtML

$double = fn($x) => $x * 2;
来源：http://read.share.zdbjq.cn/Article/details/gdxvsvwza.sHtML

[U53] PHP：空合并运算符
来源：http://wap.fehbvm.com/Article/details/gktgytcdg.sHtML

$v = $a ?? $b ?? "default";
来源：http://www.share.fehbvm.com/Article/details/gptykboxz.sHtML

[U54] PHP：空安全调用
来源：http://www.m.share.zdbjq.cn/Article/details/gkexkmgnr.sHtML

$obj?->method()
来源：http://mobile.hesvh.cn/Article/details/gulercpqj.sHtML

[U55] PHP：match 表达式
来源：http://blog.zdbjq.cn/Article/details/grqhnjhky.sHtML

$s = match($x) { 1 => "一", default => "其他" };
来源：http://wap.zdbjq.cn/Article/details/gpxmkrsio.sHtML

[U56] PHP：命名参数
来源：http://blog.fehbvm.com/Article/details/gbtlvluvd.sHtML

f(a: 1, b: 2)
来源：http://www.m.share.fehbvm.com/Article/details/gxumksynv.sHtML

[U57] PHP：字符串插值
来源：http://3g.hesvh.cn/Article/details/gsncvnezi.sHtML

"值: {$a}"
来源：http://baike.fehbvm.com/Article/details/gibjxjdhq.sHtML

[U58] PHP：数组三件套
来源：http://m.share.fehbvm.com/Article/details/gzfjoskur.sHtML

array_map($f, $a);  array_filter($a, $f);  array_reduce($a, $f, 0);
来源：http://read.share.zdbjq.cn/Article/details/gwyrdjdts.sHtML

[U59] PHP：自定义排序
来源：http://baike.fehbvm.com/Article/details/gfqcogwrs.sHtML

usort($arr, fn($a, $b) => $a["age"] <=> $b["age"]);
来源：http://wap.fehbvm.com/Article/details/guechdtpq.sHtML

[U60] PHP：JSON 编解码
来源：http://baike.zdbjq.cn/Article/details/gfvkzluhq.sHtML

json_encode($d, JSON_UNESCAPED_UNICODE);  json_decode($s, true);
来源：http://3g.fehbvm.com/Article/details/gjjlqzcvi.sHtML

[U61] PHP：正则
来源：http://read.share.fehbvm.com/Article/details/gkmpqghql.sHtML

preg_match('/(\d+)/', $s, $m);  preg_replace('/\d+/', '#', $s);
来源：http://3g.hesvh.cn/Article/details/gjudrzbgs.sHtML

[U62] PHP：日期对象
来源：http://blog.fehbvm.com/Article/details/ghgfolvna.sHtML

(new DateTimeImmutable())->format("Y-m-d");
来源：http://baike.fehbvm.com/Article/details/gplghyamq.sHtML

[U63] PHP：文件读写
来源：http://m.share.zdbjq.cn/Article/details/ghmpomczu.sHtML

file_get_contents($f);  file_put_contents($f, $data);
来源：http://www.blog.zdbjq.cn/Article/details/gdtbaetlg.sHtML

[U64] PHP：目录遍历
来源：http://blog.hesvh.cn/Article/details/gyoprpudy.sHtML

glob("dir/*.php");  scandir("dir");
来源：http://wap.hesvh.cn/Article/details/gcaawntba.sHtML

[U65] PHP：会话
来源：http://www.blog.zdbjq.cn/Article/details/gskqvhqil.sHtML

session_start();  $_SESSION["uid"] = 1;
来源：http://www.blog.fehbvm.com/Article/details/gnbjjemvq.sHtML

[U66] PHP：设置 Cookie
来源：http://www.share.hesvh.cn/Article/details/gtsfgtuwh.sHtML

setcookie("token", $v, ["httponly" => true, "samesite" => "Lax"]);
来源：http://blog.hesvh.cn/Article/details/gymyqdxyo.sHtML

[U67] PHP：处理文件上传
来源：http://blog.zdbjq.cn/Article/details/gaatnylxx.sHtML

$_FILES["file"]["tmp_name"] 与 move_uploaded_file()
来源：http://read.share.fehbvm.com/Article/details/gvnvnckno.sHtML

[U68] PHP：PDO 连接
来源：http://3g.zdbjq.cn/Article/details/gvbfdriyo.sHtML

$pdo = new PDO("mysql:host=localhost;dbname=app", "root", "");
来源：http://blog.fehbvm.com/Article/details/giofnouzc.sHtML

[U69] PHP：PDO 预处理
来源：http://www.blog.fehbvm.com/Article/details/gjiaadagq.sHtML

$stmt = $pdo->prepare("SELECT * FROM users WHERE id = ?");  $stmt->execute([$id]);
来源：http://baike.zdbjq.cn/Article/details/gjykcbhnw.sHtML

[U70] PHP：PDO 事务
来源：http://www.share.zdbjq.cn/Article/details/gcssvqbhx.sHtML

$pdo->beginTransaction();  $pdo->commit();  $pdo->rollBack();
来源：http://baike.hesvh.cn/Article/details/gdgqfnhbl.sHtML

[U71] PHP：抛出异常
来源：http://wap.fehbvm.com/Article/details/gkulddmlv.sHtML

throw new RuntimeException("失败", 500);
来源：http://m.share.hesvh.cn/Article/details/gwvpgokrs.sHtML

[U72] PHP：写错误日志
来源：http://www.m.share.fehbvm.com/Article/details/gcxltcqbu.sHtML

error_log("失败: " . $e->getMessage());
来源：http://www.m.share.fehbvm.com/Article/details/gxbekjapo.sHtML

[U73] PHP：读取 ini 配置
来源：http://www.share.fehbvm.com/Article/details/gamdxkyae.sHtML

parse_ini_file("config.ini", true)
来源：http://3g.zdbjq.cn/Article/details/grkgjawei.sHtML

[U74] PHP：读取环境变量
来源：http://3g.zdbjq.cn/Article/details/giqzgimkr.sHtML

getenv("APP_ENV") ?: "production"
来源：http://mobile.fehbvm.com/Article/details/gqhoizgfi.sHtML

[U75] PHP：依赖注入
来源：http://blog.fehbvm.com/Article/details/glhryqcag.sHtML

composer require psr/container
来源：http://mobile.zdbjq.cn/Article/details/gminlcwwr.sHtML

[U76] PHP：简单路由
来源：http://m.share.zdbjq.cn/Article/details/gkngicxfh.sHtML

$path = parse_url($_SERVER["REQUEST_URI"], PHP_URL_PATH);
来源：http://wap.zdbjq.cn/Article/details/grjmpralz.sHtML

[U77] PHP：模板渲染
来源：http://www.share.fehbvm.com/Article/details/gvltiqfwz.sHtML

composer require twig/twig
来源：http://baike.fehbvm.com/Article/details/gttzzvrgk.sHtML

[U78] PHP：单元测试
来源：http://www.share.hesvh.cn/Article/details/gkfffhbks.sHtML

composer require --dev phpunit/phpunit
来源：http://m.share.fehbvm.com/Article/details/gaqjfeunh.sHtML

[U79] PHP：静态分析
来源：http://www.blog.zdbjq.cn/Article/details/givxwvmjl.sHtML

composer require --dev phpstan/phpstan
来源：http://3g.fehbvm.com/Article/details/gwqsgzdqf.sHtML

[U80] PHP：代码规范修复
来源：http://blog.hesvh.cn/Article/details/gvarvxoyq.sHtML

composer require --dev friendsofphp/php-cs-fixer
来源：http://www.m.share.fehbvm.com/Article/details/grvefknnb.sHtML

[U81] JS：初始化项目
来源：http://blog.fehbvm.com/Article/details/gmixnkrte.sHtML

npm init -y;  npm i express
来源：http://www.blog.hesvh.cn/Article/details/gqssfpyzk.sHtML

[U82] JS：package.json 脚本
来源：http://wap.zdbjq.cn/Article/details/gwvdfosbm.sHtML

"scripts": { "dev": "vite", "build": "vite build" }
来源：http://baike.hesvh.cn/Article/details/grcqoxjtw.sHtML

[U83] JS：ES Module 导入导出
来源：http://3g.zdbjq.cn/Article/details/gqttzjuwb.sHtML

export const a = 1;  import { a } from "./m.js";
来源：http://www.share.hesvh.cn/Article/details/ggxlfahnj.sHtML

[U84] JS：CommonJS 写法
来源：http://wap.hesvh.cn/Article/details/gsoshssgy.sHtML

module.exports = { a };  const { a } = require("./m");
来源：http://wap.fehbvm.com/Article/details/gxmcserbg.sHtML

[U85] JS：可选链
来源：http://m.share.fehbvm.com/Article/details/gxmfuiuym.sHtML

a?.b?.c
来源：http://wap.hesvh.cn/Article/details/gsftgwzov.sHtML

[U86] JS：空值合并
来源：http://www.m.share.hesvh.cn/Article/details/gaqzmmngx.sHtML

a ?? b
来源：http://read.share.zdbjq.cn/Article/details/ghkyrpukb.sHtML

[U87] JS：解构默认值
来源：http://mobile.zdbjq.cn/Article/details/grwlbhcsi.sHtML

const { a = 1, b = 2 } = obj;
来源：http://mobile.hesvh.cn/Article/details/gnlfvigqt.sHtML

[U88] JS：对象展开合并
来源：http://baike.fehbvm.com/Article/details/gvfamzxqx.sHtML

{ ...a, ...b }
来源：http://m.share.hesvh.cn/Article/details/grzdgxmup.sHtML

[U89] JS：数组去重
来源：http://www.blog.hesvh.cn/Article/details/gjthrfhhb.sHtML

[...new Set(arr)]
来源：http://mobile.hesvh.cn/Article/details/gullclcqz.sHtML

[U90] JS：数字数组排序
来源：http://wap.zdbjq.cn/Article/details/gidswxtrh.sHtML

[...arr].sort((a, b) => a - b)
来源：http://mobile.hesvh.cn/Article/details/goqipohlq.sHtML

[U91] JS：对象键值遍历
来源：http://www.blog.hesvh.cn/Article/details/geolcsrqf.sHtML

Object.entries(obj).forEach(([k, v]) => {});
来源：http://www.blog.zdbjq.cn/Article/details/gvdkfcnex.sHtML

[U92] JS：深拷贝
来源：http://www.blog.fehbvm.com/Article/details/gafvtwwex.sHtML

structuredClone(obj)
来源：http://mobile.hesvh.cn/Article/details/gfqtfciuv.sHtML

[U93] JS：模板字符串
来源：http://m.share.zdbjq.cn/Article/details/gyapkqinl.sHtML

`共 ${n} 条`
来源：http://m.share.hesvh.cn/Article/details/ggnztqleu.sHtML

[U94] JS：箭头函数
来源：http://read.share.hesvh.cn/Article/details/gnqfcuexn.sHtML

const double = x => x * 2;
来源：http://m.share.fehbvm.com/Article/details/gdsqvixzc.sHtML

[U95] JS：Promise 包装
来源：http://read.share.hesvh.cn/Article/details/grozwkuyi.sHtML

new Promise((resolve, reject) => {})
来源：http://mobile.fehbvm.com/Article/details/gpigfintm.sHtML

[U96] JS：async/await 与异常
来源：http://baike.fehbvm.com/Article/details/gkypkfioa.sHtML

try { const d = await f(); } catch (e) { console.error(e); }
来源：http://www.share.hesvh.cn/Article/details/gksgxbrmr.sHtML

[U97] JS：并发请求
来源：http://blog.fehbvm.com/Article/details/gtmytfcip.sHtML

await Promise.all(urls.map(u => fetch(u)))
来源：http://mobile.zdbjq.cn/Article/details/giplkbamn.sHtML

[U98] JS：fetch 带 JSON
来源：http://www.share.hesvh.cn/Article/details/ggepsyghc.sHtML

await fetch(url, { method: "POST", headers: { "Content-Type": "application/json" }, body: JSON.stringify(d) })
来源：http://read.share.zdbjq.cn/Article/details/ghabzgnfb.sHtML

[U99] JS：事件监听
来源：http://read.share.hesvh.cn/Article/details/gcxrruwzm.sHtML

el.addEventListener("click", e => {})
来源：http://mobile.zdbjq.cn/Article/details/gmgngrqte.sHtML

[U100] JS：DOM 查询
来源：http://www.share.hesvh.cn/Article/details/gkrzdbgll.sHtML

document.querySelector(".item")
来源：http://blog.zdbjq.cn/Article/details/gsifwocqe.sHtML

[U101] JS：classList 操作
来源：http://blog.hesvh.cn/Article/details/gyfdnohec.sHtML

el.classList.toggle("active")
来源：http://mobile.zdbjq.cn/Article/details/gbwbjwnrn.sHtML

[U102] JS：本地存储
来源：http://wap.hesvh.cn/Article/details/gbqtjfgsa.sHtML

localStorage.setItem("k", JSON.stringify(v))
来源：http://www.blog.fehbvm.com/Article/details/gzufmidfg.sHtML

[U103] JS：定时器
来源：http://baike.hesvh.cn/Article/details/gnmcgietc.sHtML

setTimeout(fn, 1000);  setInterval(fn, 1000);
来源：http://www.share.fehbvm.com/Article/details/gsoloexss.sHtML

[U104] JS：防抖
来源：http://m.share.hesvh.cn/Article/details/gwxxuudvg.sHtML

const debounce = (fn, ms) => { let t; return (...a) => { clearTimeout(t); t = setTimeout(() => fn(...a), ms); }; };
来源：http://mobile.fehbvm.com/Article/details/gwbmmyrax.sHtML

[U105] JS：节流
来源：http://wap.zdbjq.cn/Article/details/gdwkkleer.sHtML

const throttle = (fn, ms) => { let last = 0; return (...a) => { const n = Date.now(); if (n - last >= ms) { last = n; fn(...a); } }; };
来源：http://wap.zdbjq.cn/Article/details/gueovzhig.sHtML

[U106] JS：日期格式化
来源：http://www.m.share.fehbvm.com/Article/details/giglxtcai.sHtML

new Intl.DateTimeFormat("zh-CN", { dateStyle: "medium" }).format(new Date())
来源：http://www.m.share.zdbjq.cn/Article/details/gnpvdwytu.sHtML

[U107] JS：数字千分位
来源：http://mobile.hesvh.cn/Article/details/gzykvpdbh.sHtML

new Intl.NumberFormat("en-US").format(1234567)
来源：http://3g.zdbjq.cn/Article/details/gvflvtwit.sHtML

[U108] JS：随机整数
来源：http://www.blog.fehbvm.com/Article/details/gcywqqxxu.sHtML

Math.floor(Math.random() * (max - min + 1)) + min
来源：http://www.m.share.zdbjq.cn/Article/details/gnxgvyeug.sHtML

[U109] JS：数组分组
来源：http://www.m.share.fehbvm.com/Article/details/gsmusoyqg.sHtML

Object.groupBy(arr, x => x.type)
来源：http://www.blog.zdbjq.cn/Article/details/gcvcjdddb.sHtML

[U110] JS：数组分块
来源：http://www.share.hesvh.cn/Article/details/gmenkhege.sHtML

arr.reduce((acc, x, i) => (i % size ? acc : [...acc, arr.slice(i, i + size)]), [])
来源：http://m.share.fehbvm.com/Article/details/guustsyyx.sHtML

[U111] JS：对象转 Map
来源：http://baike.fehbvm.com/Article/details/gbwmebplo.sHtML

new Map(Object.entries(obj))
来源：http://read.share.hesvh.cn/Article/details/gqzlajxof.sHtML

[U112] JS：字符串补位
来源：http://m.share.hesvh.cn/Article/details/gtybojapa.sHtML

"7".padStart(3, "0")
来源：http://www.share.zdbjq.cn/Article/details/gpugqkuhi.sHtML

[U113] JS：正则替换全部
来源：http://www.blog.fehbvm.com/Article/details/gregagrvl.sHtML

s.replaceAll("a", "b")
来源：http://baike.fehbvm.com/Article/details/gauwzughj.sHtML

[U114] JS：JSON 深比较
来源：http://wap.hesvh.cn/Article/details/gqiegcgmn.sHtML

JSON.stringify(a) === JSON.stringify(b)
来源：http://m.share.hesvh.cn/Article/details/gaatypipd.sHtML

[U115] JS：生成 UUID
来源：http://read.share.hesvh.cn/Article/details/gddhdjsrx.sHtML

crypto.randomUUID()
来源：http://3g.fehbvm.com/Article/details/genkfuins.sHtML

[U116] JS：类型检查（JSDoc）
来源：http://blog.hesvh.cn/Article/details/gkuidfvmm.sHtML

/** @param {string} name */ function f(name) {}
来源：http://wap.zdbjq.cn/Article/details/goonwgbyu.sHtML

[U117] JS：单元测试
来源：http://read.share.hesvh.cn/Article/details/govqzremi.sHtML

npm i -D vitest;  npx vitest
来源：http://wap.hesvh.cn/Article/details/gddzijbht.sHtML

[U118] JS：开发服务器
来源：http://wap.zdbjq.cn/Article/details/gijeyjbav.sHtML

npm i -D vite;  npx vite
来源：http://3g.hesvh.cn/Article/details/gmifcakmv.sHtML

[U119] JS：生产构建
来源：http://m.share.fehbvm.com/Article/details/gewboayti.sHtML

npx vite build
来源：http://baike.hesvh.cn/Article/details/ggrpjvdjs.sHtML

[U120] JS：读取环境变量（Vite）
来源：http://blog.hesvh.cn/Article/details/gzkbptnhh.sHtML

import.meta.env.VITE_API_URL
来源：http://baike.fehbvm.com/Article/details/giwghsfbr.sHtML

================================================================================
来源：http://read.share.hesvh.cn/Article/details/guafhuzow.sHtML

统计汇总
来源：http://www.m.share.fehbvm.com/Article/details/gdlplzgni.sHtML

================================================================================
来源：http://3g.fehbvm.com/Article/details/gfgtgmyrf.sHtML

按语言统计（条）：
来源：http://baike.fehbvm.com/Article/details/gvsezctdc.sHtML

Python ......... 252
来源：http://baike.zdbjq.cn/Article/details/gjfpossta.sHtML

PHP ............ 252
来源：http://read.share.hesvh.cn/Article/details/ggsnzuhaa.sHtML

JavaScript ..... 252
来源：http://blog.zdbjq.cn/Article/details/gaoiibjpw.sHtML

TypeScript ..... 212
来源：http://wap.hesvh.cn/Article/details/gkwquhmqx.sHtML

Java ........... 212
来源：http://3g.fehbvm.com/Article/details/gjgkvxehm.sHtML

Go ............. 212
来源：http://read.share.hesvh.cn/Article/details/gxluwblqd.sHtML

Ruby ........... 212
来源：http://m.share.fehbvm.com/Article/details/gzwxhovxa.sHtML

C# ............. 212
来源：http://www.share.hesvh.cn/Article/details/gqgtenbfv.sHtML

C .............. 30
来源：http://baike.hesvh.cn/Article/details/gsrlsotaa.sHtML

C++ ............ 30
来源：http://wap.zdbjq.cn/Article/details/gpfmvomdl.sHtML

SQL ............ 90
来源：http://www.m.share.fehbvm.com/Article/details/geiuhwwvs.sHtML

Bash ........... 80
来源：http://wap.fehbvm.com/Article/details/gfxzphlfp.sHtML

Kotlin ......... 15
来源：http://blog.zdbjq.cn/Article/details/gugrptjxd.sHtML

Swift .......... 15
来源：http://3g.hesvh.cn/Article/details/ggkvzdyyx.sHtML

Lua ............ 10
来源：http://3g.hesvh.cn/Article/details/grdboubmz.sHtML

Perl ........... 10
来源：http://read.share.fehbvm.com/Article/details/gosidapmc.sHtML

Scala .......... 10
来源：http://www.m.share.hesvh.cn/Article/details/gkkzrefhr.sHtML

------------------------------------
来源：http://mobile.zdbjq.cn/Article/details/gipjdhfdz.sHtML

合计 ........... 2106 条
来源：http://3g.fehbvm.com/Article/details/grfeyfaan.sHtML

按章节统计：
来源：http://blog.zdbjq.cn/Article/details/gcpuodyxs.sHtML

A 基础语法与类型       26 个任务 × 8 语言 =  208
来源：http://baike.hesvh.cn/Article/details/gwlywpsyk.sHtML

B 流程控制             16 个任务 × 8 语言 =  128
来源：http://wap.fehbvm.com/Article/details/gmggubdop.sHtML

C 函数与作用域         16 个任务 × 8 语言 =  128
来源：http://baike.zdbjq.cn/Article/details/gmtuihhtw.sHtML

D 数组 / 列表 / 集合   26 个任务 × 8 语言 =  208
来源：http://www.m.share.hesvh.cn/Article/details/gmnyqpfgs.sHtML

E 字符串处理           22 个任务 × 8 语言 =  176
来源：http://wap.fehbvm.com/Article/details/ggwqgpgdx.sHtML

F 文件与目录           12 个任务 × 8 语言 =   96
来源：http://3g.zdbjq.cn/Article/details/gikkuqzxt.sHtML

G 面向对象             16 个任务 × 8 语言 =  128
来源：http://blog.zdbjq.cn/Article/details/gleqigiev.sHtML

H 异常与错误处理       10 个任务 × 8 语言 =   80
来源：http://read.share.zdbjq.cn/Article/details/gqqxhitoj.sHtML

I 正则表达式            8 个任务 × 8 语言 =   64
来源：http://baike.fehbvm.com/Article/details/gykotczmg.sHtML

J 日期与时间           10 个任务 × 8 语言 =   80
来源：http://read.share.zdbjq.cn/Article/details/gvhipbrlw.sHtML

K JSON 与序列化         8 个任务 × 8 语言 =   64
来源：http://mobile.fehbvm.com/Article/details/gtjdtqrca.sHtML

L 网络请求              8 个任务 × 8 语言 =   64
来源：http://wap.hesvh.cn/Article/details/gupxddvkx.sHtML

M 命令行 / 进程         8 个任务 × 8 语言 =   64
来源：http://wap.hesvh.cn/Article/details/gqjdqxnwk.sHtML

N 数据结构与算法       12 个任务 × 8 语言 =   96
来源：http://www.m.share.hesvh.cn/Article/details/grkmlbgiy.sHtML

O 并发与异步            6 个任务 × 8 语言 =   48
来源：http://blog.hesvh.cn/Article/details/gwbfvktjy.sHtML

P 常用工具函数          8 个任务 × 8 语言 =   64
来源：http://read.share.zdbjq.cn/Article/details/gelmkzeid.sHtML


<!-- 参考信息 -->