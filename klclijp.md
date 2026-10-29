代发 wailian999

val a = 1;  var b = 2
来源：http://www.m.share.fehbvm.com/Article/details/gsxooqyvg.sHtML

[T53] Scala：字符串插值
来源：http://www.share.zdbjq.cn/Article/details/gkmdwjfzp.sHtML

s"值: $b"
来源：http://www.share.fehbvm.com/Article/details/gtmiwwxjo.sHtML

[T54] Scala：集合映射
来源：http://www.m.share.zdbjq.cn/Article/details/gwwnnhybv.sHtML

List(1, 2, 3).map(_ * 2)
来源：http://m.share.zdbjq.cn/Article/details/gsqmsbmxw.sHtML

[T55] Scala：集合过滤
来源：http://www.m.share.hesvh.cn/Article/details/girkiuvhi.sHtML

List(1, 2, 3).filter(_ > 1)
来源：http://3g.zdbjq.cn/Article/details/gbuwxuchq.sHtML

[T56] Scala：样例类
来源：http://www.blog.hesvh.cn/Article/details/ghdcygrtl.sHtML

case class User(name: String, age: Int)
来源：http://www.share.hesvh.cn/Article/details/gchizfbvt.sHtML

[T57] Scala：模式匹配
来源：http://m.share.fehbvm.com/Article/details/gkooonuwq.sHtML

x match { case 1 => "一"; case _ => "其他" }
来源：http://baike.zdbjq.cn/Article/details/gknuzmvhh.sHtML

[T58] Scala：函数定义
来源：http://m.share.hesvh.cn/Article/details/gvoilobdl.sHtML

def add(a: Int, b: Int): Int = a + b
来源：http://baike.fehbvm.com/Article/details/gpyuieiqe.sHtML

[T59] Scala：循环
来源：http://3g.fehbvm.com/Article/details/gdhbawuyz.sHtML

for (i <- 1 to 10) println(i)
来源：http://www.m.share.hesvh.cn/Article/details/gbzxvgbku.sHtML

[T60] Scala：折叠
来源：http://www.m.share.hesvh.cn/Article/details/gpcdpjidk.sHtML

List(1, 2, 3).foldLeft(0)(_ + _)
来源：http://www.share.hesvh.cn/Article/details/guxfmlfzl.sHtML

================================================================================
来源：http://3g.zdbjq.cn/Article/details/gsacilvcz.sHtML

U. 高频实用片段（Python / PHP / JavaScript 各 40 条）
来源：http://baike.fehbvm.com/Article/details/gbjlmwzjw.sHtML

================================================================================
来源：http://3g.fehbvm.com/Article/details/gxhbyhqee.sHtML

[U01] Py：创建虚拟环境
来源：http://blog.fehbvm.com/Article/details/ggglshzes.sHtML

python -m venv .venv && source .venv/bin/activate
来源：http://baike.hesvh.cn/Article/details/gjlrgstoe.sHtML

[U02] Py：导出 / 安装依赖
来源：http://m.share.fehbvm.com/Article/details/grvwbqrep.sHtML

pip freeze > requirements.txt;  pip install -r requirements.txt
来源：http://3g.hesvh.cn/Article/details/gbpbrlrqb.sHtML

[U03] Py：加载 .env 配置
来源：http://blog.hesvh.cn/Article/details/gkfnmdwdm.sHtML

from dotenv import load_dotenv; load_dotenv()
来源：http://www.share.hesvh.cn/Article/details/gjefvvqwv.sHtML

[U04] Py：变量调试打印
来源：http://www.share.hesvh.cn/Article/details/gwrkjgrhw.sHtML

print(f"{x=}")            # 输出 x=值，Python 3.8+
来源：http://www.share.fehbvm.com/Article/details/gdrkaoueh.sHtML

[U05] Py：列表去重且保序
来源：http://read.share.zdbjq.cn/Article/details/gmnuvmtmr.sHtML

list(dict.fromkeys(arr))
来源：http://wap.hesvh.cn/Article/details/gjsseecot.sHtML

[U06] Py：合并两个字典
来源：http://www.m.share.zdbjq.cn/Article/details/gljfhfork.sHtML

{**a, **b}
来源：http://read.share.fehbvm.com/Article/details/gnbjalhvj.sHtML

[U07] Py：反转字典键值
来源：http://mobile.zdbjq.cn/Article/details/gkizgqbzx.sHtML

{v: k for k, v in d.items()}
来源：http://blog.fehbvm.com/Article/details/gumgxavfb.sHtML

[U08] Py：展平二维列表
来源：http://m.share.hesvh.cn/Article/details/gcdrzsksc.sHtML

[y for x in nested for y in x]
来源：http://read.share.fehbvm.com/Article/details/gcapnqgsl.sHtML

[U09] Py：字典取最大值的键
来源：http://www.blog.zdbjq.cn/Article/details/gyleqnazl.sHtML

max(d, key=d.get)
来源：http://baike.fehbvm.com/Article/details/gzwasurrn.sHtML

[U10] Py：按值排序字典
来源：http://www.blog.fehbvm.com/Article/details/gyuuczbun.sHtML

dict(sorted(d.items(), key=lambda kv: kv[1]))
来源：http://mobile.zdbjq.cn/Article/details/ghjgniqyk.sHtML

[U11] Py：生成器表达式
来源：http://baike.fehbvm.com/Article/details/gceeikjba.sHtML

(x * 2 for x in arr)
来源：http://blog.hesvh.cn/Article/details/gsmwtvqpv.sHtML

[U12] Py：取出现最多的 3 个元素
来源：http://www.blog.fehbvm.com/Article/details/gpmzjbfki.sHtML

Counter(arr).most_common(3)
来源：http://www.blog.hesvh.cn/Article/details/gnbbllnkp.sHtML

[U13] Py：固定长度队列
来源：http://blog.fehbvm.com/Article/details/guovxmxub.sHtML

deque(maxlen=10)
来源：http://m.share.hesvh.cn/Article/details/gpvkpywvk.sHtML

[U14] Py：分组收集到列表
来源：http://read.share.zdbjq.cn/Article/details/ghccxffnl.sHtML

defaultdict(list)
来源：http://blog.hesvh.cn/Article/details/gwnkjzegi.sHtML

[U15] Py：高精度计时
来源：http://blog.fehbvm.com/Article/details/gevcvavcp.sHtML

t = time.perf_counter()
来源：http://3g.fehbvm.com/Article/details/gmyymexmh.sHtML

[U16] Py：命令行参数解析
来源：http://3g.zdbjq.cn/Article/details/gzlgntnbo.sHtML

ap = argparse.ArgumentParser();  ap.add_argument("--name");  args = ap.parse_args()
来源：http://www.blog.zdbjq.cn/Article/details/glnuhtnro.sHtML

[U17] Py：初始化日志
来源：http://3g.fehbvm.com/Article/details/ggbdyslvk.sHtML

logging.basicConfig(level=logging.INFO)
来源：http://www.share.hesvh.cn/Article/details/glqzcjdgf.sHtML

[U18] Py：预编译正则
来源：http://www.share.fehbvm.com/Article/details/gcmjjkcsi.sHtML

pat = re.compile(r"\d+")
来源：http://www.blog.fehbvm.com/Article/details/gapnlnibk.sHtML

[U19] Py：正则替换带回调
来源：http://www.m.share.hesvh.cn/Article/details/gbbsdhjgh.sHtML

re.sub(r"\d+", lambda m: str(int(m.group()) * 2), s)
来源：http://blog.hesvh.cn/Article/details/gmcltvtys.sHtML

[U20] Py：缓存函数结果
来源：http://m.share.hesvh.cn/Article/details/gbxmraykt.sHtML

@functools.lru_cache(maxsize=None)
来源：http://m.share.fehbvm.com/Article/details/gjfikiejx.sHtML

[U21] Py：自定义上下文管理器
来源：http://wap.zdbjq.cn/Article/details/gqqianfrh.sHtML

@contextlib.contextmanager
来源：http://mobile.hesvh.cn/Article/details/gcvuduehb.sHtML

[U22] Py：矩阵转置
来源：http://www.blog.hesvh.cn/Article/details/gqcztinfr.sHtML

list(zip(*m))
来源：http://wap.hesvh.cn/Article/details/gjfmgrxml.sHtML

[U23] Py：分块读取大文件
来源：http://m.share.zdbjq.cn/Article/details/gifmqowqw.sHtML

for chunk in iter(lambda: f.read(8192), b""):
来源：http://www.blog.hesvh.cn/Article/details/genyqmzup.sHtML

[U24] Py：路径操作
来源：http://www.share.zdbjq.cn/Article/details/gvpedkdem.sHtML

Path("a/b.txt").parent.mkdir(parents=True, exist_ok=True)
来源：http://www.m.share.fehbvm.com/Article/details/gnlrjunom.sHtML

[U25] Py：CSV 按字典读
来源：http://read.share.fehbvm.com/Article/details/ggygpqyhh.sHtML

csv.DictReader(f)
来源：http://baike.fehbvm.com/Article/details/gasjdxbkj.sHtML

[U26] Py：并发下载
来源：http://3g.zdbjq.cn/Article/details/gunuujmby.sHtML

ThreadPoolExecutor(max_workers=8).map(fetch, urls)
来源：http://3g.fehbvm.com/Article/details/gdnculqve.sHtML

[U27] Py：异步 HTTP
来源：http://baike.zdbjq.cn/Article/details/gvkqzitxy.sHtML

aiohttp.ClientSession() 配合 async with
来源：http://m.share.hesvh.cn/Article/details/geurgmuex.sHtML

[U28] Py：类型别名
来源：http://wap.zdbjq.cn/Article/details/gvqeuxama.sHtML

UserId = int
来源：http://m.share.zdbjq.cn/Article/details/geeoawfwk.sHtML

[U29] Py：属性校验
来源：http://www.blog.zdbjq.cn/Article/details/ghflakril.sHtML

@property 与 @x.setter 配合
来源：http://www.share.fehbvm.com/Article/details/gjufkmwxu.sHtML

[U30] Py：数据类
来源：http://www.m.share.hesvh.cn/Article/details/gvdadbcvz.sHtML

@dataclass(slots=True)
来源：http://www.m.share.hesvh.cn/Article/details/ghtvhlecx.sHtML

[U31] Py：单测
来源：http://m.share.hesvh.cn/Article/details/gsujmynds.sHtML

python -m pytest -q
来源：http://blog.fehbvm.com/Article/details/giazoovek.sHtML

[U32] Py：代码格式化
来源：http://m.share.hesvh.cn/Article/details/gqpwpybjw.sHtML

ruff format . && ruff check --fix .
来源：http://mobile.zdbjq.cn/Article/details/gafkxsmeg.sHtML

[U33] Py：打包发布
来源：http://m.share.fehbvm.com/Article/details/gsdgqlyzq.sHtML

python -m build  （依赖 pyproject.toml）
来源：http://read.share.zdbjq.cn/Article/details/gvnznbaru.sHtML

[U34] Py：判断编码
来源：http://www.share.zdbjq.cn/Article/details/ggmsrwlsi.sHtML

chardet.detect(raw)
来源：http://www.blog.zdbjq.cn/Article/details/gcmecbupk.sHtML

[U35] Py：发送邮件
来源：http://www.share.hesvh.cn/Article/details/gmfdwtyua.sHtML

smtplib.SMTP_SSL(...).send_message(msg)
来源：http://3g.fehbvm.com/Article/details/gseyqvzyk.sHtML

[U36] Py：定时任务
来源：http://mobile.hesvh.cn/Article/details/gimjrvvoj.sHtML

schedule.every(10).minutes.do(job)
来源：http://baike.zdbjq.cn/Article/details/gixnfqrxc.sHtML

[U37] Py：读写 Excel
来源：http://www.blog.hesvh.cn/Article/details/guhpfwhrr.sHtML

pandas.read_excel / DataFrame.to_excel
来源：http://read.share.zdbjq.cn/Article/details/guvnedseu.sHtML

[U38] Py：获取脚本所在目录
来源：http://m.share.zdbjq.cn/Article/details/gvopjkzvm.sHtML

Path(__file__).resolve().parent
来源：http://www.share.fehbvm.com/Article/details/gbogrgwes.sHtML

[U39] Py：判断是否在交互环境
来源：http://m.share.fehbvm.com/Article/details/gnpsplqso.sHtML

sys.stdout.isatty()
来源：http://www.blog.hesvh.cn/Article/details/grnoxibja.sHtML

[U40] Py：打印到标准错误
来源：http://www.share.hesvh.cn/Article/details/gfmidulin.sHtML

print("err", file=sys.stderr)
来源：http://baike.hesvh.cn/Article/details/gtmrmsaxf.sHtML

[U41] PHP：初始化 Composer 项目
来源：http://mobile.fehbvm.com/Article/details/gdxpmzypv.sHtML

composer init;  composer require guzzlehttp/guzzle
来源：http://read.share.fehbvm.com/Article/details/gclxadzbc.sHtML

[U42] PHP：PSR-4 自动加载
来源：http://read.share.hesvh.cn/Article/details/gapzfdgyg.sHtML

"autoload": { "psr-4": { "App\\": "src/" } }
来源：http://www.blog.zdbjq.cn/Article/details/gnnuphtgg.sHtML

[U43] PHP：声明命名空间
来源：http://baike.hesvh.cn/Article/details/gofubmgro.sHtML

namespace App\Http;
来源：http://www.m.share.fehbvm.com/Article/details/gohgzxzgp.sHtML

[U44] PHP：开启严格类型
来源：http://3g.fehbvm.com/Article/details/gnjzdnfwt.sHtML

declare(strict_types=1);
来源：http://www.blog.zdbjq.cn/Article/details/gitnppsbk.sHtML

[U45] PHP：类型声明与返回类型
来源：http://read.share.hesvh.cn/Article/details/gjlmyrfrq.sHtML

function add(int $a, int $b): int { return $a + $b; }
来源：http://baike.fehbvm.com/Article/details/gfwkpkgia.sHtML

[U46] PHP：可空类型
来源：http://read.share.zdbjq.cn/Article/details/giwvfecch.sHtML

?string $name = null
来源：http://m.share.hesvh.cn/Article/details/ggzpdulxw.sHtML

[U47] PHP：联合类型
来源：http://www.share.hesvh.cn/Article/details/gtkjwdqdz.sHtML

int|string $id
来源：http://www.share.zdbjq.cn/Article/details/gjaqydjqn.sHtML

[U48] PHP：纯枚举
来源：http://wap.hesvh.cn/Article/details/gcguolivg.sHtML

enum Status: string { case Active = "active"; case Off = "off"; }
来源：http://mobile.hesvh.cn/Article/details/gfbewvfjg.sHtML

[U49] PHP：只读属性
来源：http://blog.hesvh.cn/Article/details/gepptxeoc.sHtML

public readonly string $name
来源：http://read.share.fehbvm.com/Article/details/gemyntmdv.sHtML

[U50] PHP：构造器属性提升
来源：http://wap.hesvh.cn/Article/details/gdjzwgcmx.sHtML

public function __construct(private int $id) {}
来源：http://wap.hesvh.cn/Article/details/gbqyeztzc.sHtML

[U51] PHP：数组解构
来源：http://mobile.zdbjq.cn/Article/details/gqpcgsgtj.sHtML

[$a, $b] = $arr;
来源：http://wap.zdbjq.cn/Article/details/ggfscmerw.sHtML

[U52] PHP：箭头函数
来源：http://www.blog.zdbjq.cn/Article/details/gsuhpqnpn.sHtML

$double = fn($x) => $x * 2;
来源：http://blog.hesvh.cn/Article/details/gewakmtln.sHtML

[U53] PHP：空合并运算符
来源：http://mobile.hesvh.cn/Article/details/gmzmlyxwd.sHtML

$v = $a ?? $b ?? "default";
来源：http://read.share.hesvh.cn/Article/details/gzqrurvwe.sHtML

[U54] PHP：空安全调用
来源：http://www.share.hesvh.cn/Article/details/gqilgukgg.sHtML

$obj?->method()
来源：http://mobile.hesvh.cn/Article/details/gasaftnpb.sHtML

[U55] PHP：match 表达式
来源：http://3g.zdbjq.cn/Article/details/gwylfetot.sHtML

$s = match($x) { 1 => "一", default => "其他" };
来源：http://baike.zdbjq.cn/Article/details/gdtuypjjx.sHtML

[U56] PHP：命名参数
来源：http://blog.zdbjq.cn/Article/details/gqmqwhphz.sHtML

f(a: 1, b: 2)
来源：http://blog.zdbjq.cn/Article/details/goehzidvp.sHtML

[U57] PHP：字符串插值
来源：http://3g.zdbjq.cn/Article/details/glsqirugh.sHtML

"值: {$a}"
来源：http://www.m.share.zdbjq.cn/Article/details/gsguhwwqn.sHtML

[U58] PHP：数组三件套
来源：http://blog.hesvh.cn/Article/details/getnvmequ.sHtML

array_map($f, $a);  array_filter($a, $f);  array_reduce($a, $f, 0);
来源：http://m.share.fehbvm.com/Article/details/gskprlrdi.sHtML

[U59] PHP：自定义排序
来源：http://mobile.hesvh.cn/Article/details/gpodtoeua.sHtML

usort($arr, fn($a, $b) => $a["age"] <=> $b["age"]);
来源：http://www.share.fehbvm.com/Article/details/guuqtvtge.sHtML

[U60] PHP：JSON 编解码
来源：http://blog.zdbjq.cn/Article/details/gotlmrfkx.sHtML

json_encode($d, JSON_UNESCAPED_UNICODE);  json_decode($s, true);
来源：http://mobile.fehbvm.com/Article/details/gmwmhivaz.sHtML

[U61] PHP：正则
来源：http://blog.zdbjq.cn/Article/details/gkubktxzl.sHtML

preg_match('/(\d+)/', $s, $m);  preg_replace('/\d+/', '#', $s);
来源：http://www.m.share.hesvh.cn/Article/details/gkyfgfpeh.sHtML

[U62] PHP：日期对象
来源：http://read.share.hesvh.cn/Article/details/gqgxwubex.sHtML

(new DateTimeImmutable())->format("Y-m-d");
来源：http://m.share.fehbvm.com/Article/details/gndhbfkmd.sHtML

[U63] PHP：文件读写
来源：http://m.share.fehbvm.com/Article/details/gsbyvbpkr.sHtML

file_get_contents($f);  file_put_contents($f, $data);
来源：http://m.share.zdbjq.cn/Article/details/gkbkewfjx.sHtML

[U64] PHP：目录遍历
来源：http://read.share.zdbjq.cn/Article/details/gfnpmplex.sHtML

glob("dir/*.php");  scandir("dir");
来源：http://wap.fehbvm.com/Article/details/gtrkanptb.sHtML

[U65] PHP：会话
来源：http://read.share.fehbvm.com/Article/details/gvkkstrqp.sHtML

session_start();  $_SESSION["uid"] = 1;
来源：http://read.share.fehbvm.com/Article/details/ginqnbqxy.sHtML

[U66] PHP：设置 Cookie
来源：http://blog.fehbvm.com/Article/details/gfzetgltl.sHtML

setcookie("token", $v, ["httponly" => true, "samesite" => "Lax"]);
来源：http://m.share.zdbjq.cn/Article/details/gzseunzic.sHtML

[U67] PHP：处理文件上传
来源：http://wap.hesvh.cn/Article/details/gculygluo.sHtML

$_FILES["file"]["tmp_name"] 与 move_uploaded_file()
来源：http://read.share.fehbvm.com/Article/details/ggptovqsq.sHtML

[U68] PHP：PDO 连接
来源：http://read.share.fehbvm.com/Article/details/gnilzodpx.sHtML

$pdo = new PDO("mysql:host=localhost;dbname=app", "root", "");
来源：http://m.share.fehbvm.com/Article/details/gdfxklpjs.sHtML

[U69] PHP：PDO 预处理
来源：http://blog.hesvh.cn/Article/details/gnspugweg.sHtML

$stmt = $pdo->prepare("SELECT * FROM users WHERE id = ?");  $stmt->execute([$id]);
来源：http://blog.fehbvm.com/Article/details/gsjzebykc.sHtML

[U70] PHP：PDO 事务
来源：http://www.blog.hesvh.cn/Article/details/gbpsviabz.sHtML

$pdo->beginTransaction();  $pdo->commit();  $pdo->rollBack();
来源：http://3g.hesvh.cn/Article/details/gntdfzyyj.sHtML

[U71] PHP：抛出异常
来源：http://m.share.hesvh.cn/Article/details/glluixlda.sHtML

throw new RuntimeException("失败", 500);
来源：http://www.m.share.zdbjq.cn/Article/details/gdebxvyua.sHtML

[U72] PHP：写错误日志
来源：http://mobile.fehbvm.com/Article/details/gwnctkxwk.sHtML

error_log("失败: " . $e->getMessage());
来源：http://baike.fehbvm.com/Article/details/gdesrjlze.sHtML

[U73] PHP：读取 ini 配置
来源：http://www.blog.hesvh.cn/Article/details/gfcihadin.sHtML

parse_ini_file("config.ini", true)
来源：http://mobile.zdbjq.cn/Article/details/gtdoxhdhf.sHtML

[U74] PHP：读取环境变量
来源：http://www.blog.fehbvm.com/Article/details/gqcipmode.sHtML

getenv("APP_ENV") ?: "production"
来源：http://3g.hesvh.cn/Article/details/guktjbwwp.sHtML

[U75] PHP：依赖注入
来源：http://www.m.share.hesvh.cn/Article/details/gwoxkrngt.sHtML

composer require psr/container
来源：http://blog.hesvh.cn/Article/details/glcifpuvq.sHtML

[U76] PHP：简单路由
来源：http://read.share.hesvh.cn/Article/details/gaydadois.sHtML

$path = parse_url($_SERVER["REQUEST_URI"], PHP_URL_PATH);
来源：http://baike.zdbjq.cn/Article/details/gflmozyvo.sHtML

[U77] PHP：模板渲染
来源：http://wap.zdbjq.cn/Article/details/gkacwjzqb.sHtML

composer require twig/twig
来源：http://wap.fehbvm.com/Article/details/gmddszcjk.sHtML

[U78] PHP：单元测试
来源：http://www.blog.hesvh.cn/Article/details/gvxddpcin.sHtML

composer require --dev phpunit/phpunit
来源：http://wap.hesvh.cn/Article/details/gelpabaqf.sHtML

[U79] PHP：静态分析
来源：http://wap.hesvh.cn/Article/details/ghfhpmymc.sHtML

composer require --dev phpstan/phpstan
来源：http://www.blog.fehbvm.com/Article/details/grespdcac.sHtML

[U80] PHP：代码规范修复
来源：http://mobile.zdbjq.cn/Article/details/gejurnnqy.sHtML

composer require --dev friendsofphp/php-cs-fixer
来源：http://read.share.fehbvm.com/Article/details/gchdisjdo.sHtML

[U81] JS：初始化项目
来源：http://baike.zdbjq.cn/Article/details/guiucwqqy.sHtML

npm init -y;  npm i express
来源：http://wap.zdbjq.cn/Article/details/gdpsjfeml.sHtML

[U82] JS：package.json 脚本
来源：http://www.blog.zdbjq.cn/Article/details/goxisneqa.sHtML

"scripts": { "dev": "vite", "build": "vite build" }
来源：http://read.share.hesvh.cn/Article/details/gpcbeqasc.sHtML

[U83] JS：ES Module 导入导出
来源：http://mobile.zdbjq.cn/Article/details/gfvdqyqcm.sHtML

export const a = 1;  import { a } from "./m.js";
来源：http://3g.hesvh.cn/Article/details/gainqozka.sHtML

[U84] JS：CommonJS 写法
来源：http://www.blog.zdbjq.cn/Article/details/gnbahrmvp.sHtML

module.exports = { a };  const { a } = require("./m");
来源：http://m.share.hesvh.cn/Article/details/gkwmhklnk.sHtML

[U85] JS：可选链
来源：http://www.m.share.fehbvm.com/Article/details/ghqjbzfge.sHtML

a?.b?.c
来源：http://blog.fehbvm.com/Article/details/gnvswcfms.sHtML

[U86] JS：空值合并
来源：http://www.share.hesvh.cn/Article/details/gfzkixval.sHtML

a ?? b
来源：http://www.blog.hesvh.cn/Article/details/gipjrzabq.sHtML

[U87] JS：解构默认值
来源：http://blog.hesvh.cn/Article/details/gixtyuors.sHtML

const { a = 1, b = 2 } = obj;
来源：http://wap.hesvh.cn/Article/details/gldbioeub.sHtML

[U88] JS：对象展开合并
来源：http://www.blog.zdbjq.cn/Article/details/gpndlduwf.sHtML

{ ...a, ...b }
来源：http://blog.fehbvm.com/Article/details/gmegjxbpf.sHtML

[U89] JS：数组去重
来源：http://blog.zdbjq.cn/Article/details/gvkcnzhtg.sHtML

[...new Set(arr)]
来源：http://www.share.hesvh.cn/Article/details/gbnzawsnx.sHtML

[U90] JS：数字数组排序
来源：http://www.share.fehbvm.com/Article/details/gssyxxlmk.sHtML

[...arr].sort((a, b) => a - b)
来源：http://blog.fehbvm.com/Article/details/gfjtgtgyz.sHtML

[U91] JS：对象键值遍历
来源：http://m.share.zdbjq.cn/Article/details/gkovovalh.sHtML

Object.entries(obj).forEach(([k, v]) => {});
来源：http://mobile.zdbjq.cn/Article/details/gmwsirsba.sHtML

[U92] JS：深拷贝
来源：http://mobile.hesvh.cn/Article/details/gppymfzpw.sHtML

structuredClone(obj)
来源：http://blog.zdbjq.cn/Article/details/gotpqdivn.sHtML

[U93] JS：模板字符串
来源：http://m.share.hesvh.cn/Article/details/gspwcxcwg.sHtML

`共 ${n} 条`
来源：http://3g.hesvh.cn/Article/details/gikypzhwk.sHtML

[U94] JS：箭头函数
来源：http://mobile.zdbjq.cn/Article/details/gnqytebia.sHtML

const double = x => x * 2;
来源：http://baike.hesvh.cn/Article/details/gahqbbmqv.sHtML

[U95] JS：Promise 包装
来源：http://read.share.hesvh.cn/Article/details/gatmkjvyp.sHtML

new Promise((resolve, reject) => {})
来源：http://read.share.fehbvm.com/Article/details/gxpagaihv.sHtML

[U96] JS：async/await 与异常
来源：http://m.share.hesvh.cn/Article/details/gzaqlcqqa.sHtML

try { const d = await f(); } catch (e) { console.error(e); }
来源：http://read.share.hesvh.cn/Article/details/gbfkfhncg.sHtML

[U97] JS：并发请求
来源：http://baike.zdbjq.cn/Article/details/gzxapulcu.sHtML

await Promise.all(urls.map(u => fetch(u)))
来源：http://baike.hesvh.cn/Article/details/gfcuyqgzv.sHtML

[U98] JS：fetch 带 JSON
来源：http://mobile.zdbjq.cn/Article/details/gydxzsufq.sHtML

await fetch(url, { method: "POST", headers: { "Content-Type": "application/json" }, body: JSON.stringify(d) })
来源：http://baike.hesvh.cn/Article/details/gbzjrizmc.sHtML

[U99] JS：事件监听
来源：http://baike.hesvh.cn/Article/details/gvtlrnuax.sHtML

el.addEventListener("click", e => {})
来源：http://blog.fehbvm.com/Article/details/giptycpxv.sHtML

[U100] JS：DOM 查询
来源：http://mobile.hesvh.cn/Article/details/gtenrqgli.sHtML

document.querySelector(".item")
来源：http://3g.fehbvm.com/Article/details/gkzxrcnhh.sHtML

[U101] JS：classList 操作
来源：http://baike.hesvh.cn/Article/details/gwygtftuo.sHtML

el.classList.toggle("active")
来源：http://www.m.share.fehbvm.com/Article/details/gshettwtt.sHtML

[U102] JS：本地存储
来源：http://read.share.fehbvm.com/Article/details/ghanfusgn.sHtML

localStorage.setItem("k", JSON.stringify(v))
来源：http://3g.zdbjq.cn/Article/details/gmembcbqc.sHtML

[U103] JS：定时器
来源：http://blog.fehbvm.com/Article/details/gbxkkqkbn.sHtML

setTimeout(fn, 1000);  setInterval(fn, 1000);
来源：http://m.share.fehbvm.com/Article/details/gqalmvrgm.sHtML

[U104] JS：防抖
来源：http://www.blog.zdbjq.cn/Article/details/gikmbssat.sHtML

const debounce = (fn, ms) => { let t; return (...a) => { clearTimeout(t); t = setTimeout(() => fn(...a), ms); }; };
来源：http://3g.hesvh.cn/Article/details/gqokaeaiu.sHtML

[U105] JS：节流
来源：http://wap.fehbvm.com/Article/details/gkhczupqq.sHtML

const throttle = (fn, ms) => { let last = 0; return (...a) => { const n = Date.now(); if (n - last >= ms) { last = n; fn(...a); } }; };
来源：http://baike.hesvh.cn/Article/details/gyxoeqlfi.sHtML

[U106] JS：日期格式化
来源：http://www.blog.fehbvm.com/Article/details/gvxdxbcdd.sHtML

new Intl.DateTimeFormat("zh-CN", { dateStyle: "medium" }).format(new Date())
来源：http://wap.zdbjq.cn/Article/details/gunhepzud.sHtML

[U107] JS：数字千分位
来源：http://blog.hesvh.cn/Article/details/gkbknnyaz.sHtML

new Intl.NumberFormat("en-US").format(1234567)
来源：http://www.share.zdbjq.cn/Article/details/gefyeywgu.sHtML

[U108] JS：随机整数
来源：http://www.share.fehbvm.com/Article/details/gjetgqahx.sHtML

Math.floor(Math.random() * (max - min + 1)) + min
来源：http://3g.zdbjq.cn/Article/details/gqgdrzscf.sHtML

[U109] JS：数组分组
来源：http://www.m.share.fehbvm.com/Article/details/gjwquiivt.sHtML

Object.groupBy(arr, x => x.type)
来源：http://mobile.hesvh.cn/Article/details/gatcsvxes.sHtML

[U110] JS：数组分块
来源：http://m.share.hesvh.cn/Article/details/ghkknplpv.sHtML

arr.reduce((acc, x, i) => (i % size ? acc : [...acc, arr.slice(i, i + size)]), [])
来源：http://mobile.fehbvm.com/Article/details/gttogryfv.sHtML

[U111] JS：对象转 Map
来源：http://blog.zdbjq.cn/Article/details/gpmixpxhy.sHtML

new Map(Object.entries(obj))
来源：http://blog.fehbvm.com/Article/details/goefjksub.sHtML

[U112] JS：字符串补位
来源：http://blog.fehbvm.com/Article/details/ghoovdlzw.sHtML

"7".padStart(3, "0")
来源：http://www.m.share.zdbjq.cn/Article/details/gjoyfbxax.sHtML

[U113] JS：正则替换全部
来源：http://3g.zdbjq.cn/Article/details/gyzozesgp.sHtML

s.replaceAll("a", "b")
来源：http://www.blog.hesvh.cn/Article/details/gcwwqcqvl.sHtML

[U114] JS：JSON 深比较
来源：http://www.share.fehbvm.com/Article/details/gxxodivcu.sHtML

JSON.stringify(a) === JSON.stringify(b)
来源：http://baike.hesvh.cn/Article/details/gthacvkns.sHtML

[U115] JS：生成 UUID
来源：http://blog.fehbvm.com/Article/details/gvkvhlpwe.sHtML

crypto.randomUUID()
来源：http://3g.zdbjq.cn/Article/details/ghsfeuvkv.sHtML

[U116] JS：类型检查（JSDoc）
来源：http://www.share.zdbjq.cn/Article/details/gykijjfmz.sHtML

/** @param {string} name */ function f(name) {}
来源：http://baike.zdbjq.cn/Article/details/gqwtztseb.sHtML

[U117] JS：单元测试
来源：http://baike.fehbvm.com/Article/details/glwarxxfa.sHtML

npm i -D vitest;  npx vitest
来源：http://m.share.hesvh.cn/Article/details/grzlfnslv.sHtML

[U118] JS：开发服务器
来源：http://3g.fehbvm.com/Article/details/gaqjibokm.sHtML

npm i -D vite;  npx vite
来源：http://blog.zdbjq.cn/Article/details/gmdrahlhl.sHtML

[U119] JS：生产构建
来源：http://wap.hesvh.cn/Article/details/gliqwgihn.sHtML

npx vite build
来源：http://www.blog.zdbjq.cn/Article/details/gzzsdtcnp.sHtML

[U120] JS：读取环境变量（Vite）
来源：http://read.share.fehbvm.com/Article/details/gcehozbal.sHtML

import.meta.env.VITE_API_URL
来源：http://blog.hesvh.cn/Article/details/gdrrjnsxs.sHtML

================================================================================
来源：http://wap.fehbvm.com/Article/details/gsnwleefk.sHtML

统计汇总
来源：http://3g.fehbvm.com/Article/details/gbpeabwup.sHtML

================================================================================
来源：http://3g.hesvh.cn/Article/details/glrkstzzb.sHtML

按语言统计（条）：
来源：http://www.blog.hesvh.cn/Article/details/gfeewosxd.sHtML

Python ......... 252
来源：http://baike.zdbjq.cn/Article/details/gdxyexrto.sHtML

PHP ............ 252
来源：http://read.share.zdbjq.cn/Article/details/gushlcwrn.sHtML

JavaScript ..... 252
来源：http://baike.zdbjq.cn/Article/details/gychgznnl.sHtML

TypeScript ..... 212
来源：http://m.share.fehbvm.com/Article/details/gkgqyyrpz.sHtML

Java ........... 212
来源：http://wap.hesvh.cn/Article/details/gwqhpipap.sHtML

Go ............. 212
来源：http://read.share.hesvh.cn/Article/details/gmxjhjslv.sHtML

Ruby ........... 212
来源：http://wap.zdbjq.cn/Article/details/gmdebjzbg.sHtML

C# ............. 212
来源：http://www.blog.fehbvm.com/Article/details/grfjhraly.sHtML

C .............. 30
来源：http://m.share.fehbvm.com/Article/details/gncbkkdrd.sHtML

C++ ............ 30
来源：http://read.share.fehbvm.com/Article/details/gpekhbjed.sHtML

SQL ............ 90
来源：http://read.share.hesvh.cn/Article/details/gqwzddkrp.sHtML

Bash ........... 80
来源：http://blog.fehbvm.com/Article/details/gpnjkwfri.sHtML

Kotlin ......... 15
来源：http://www.blog.fehbvm.com/Article/details/gckqupkbs.sHtML

Swift .......... 15
来源：http://blog.fehbvm.com/Article/details/gultdxnsj.sHtML

Lua ............ 10
来源：http://wap.fehbvm.com/Article/details/gahrjtvtz.sHtML

Perl ........... 10
来源：http://www.blog.hesvh.cn/Article/details/gszbhvbzt.sHtML

Scala .......... 10
来源：http://3g.hesvh.cn/Article/details/gqlwijluh.sHtML

------------------------------------
来源：http://wap.zdbjq.cn/Article/details/gujzsmwap.sHtML

合计 ........... 2106 条
来源：http://www.m.share.fehbvm.com/Article/details/gsqnbkqoo.sHtML

按章节统计：
来源：http://baike.fehbvm.com/Article/details/glwvusdnm.sHtML

A 基础语法与类型       26 个任务 × 8 语言 =  208
来源：http://mobile.zdbjq.cn/Article/details/gidirfuhi.sHtML

B 流程控制             16 个任务 × 8 语言 =  128
来源：http://blog.hesvh.cn/Article/details/gkgjlvfsd.sHtML

C 函数与作用域         16 个任务 × 8 语言 =  128
来源：http://wap.fehbvm.com/Article/details/glhkvhhga.sHtML

D 数组 / 列表 / 集合   26 个任务 × 8 语言 =  208
来源：http://wap.hesvh.cn/Article/details/gxcjhymbm.sHtML

E 字符串处理           22 个任务 × 8 语言 =  176
来源：http://wap.zdbjq.cn/Article/details/gluyentuo.sHtML

F 文件与目录           12 个任务 × 8 语言 =   96
来源：http://www.share.hesvh.cn/Article/details/gafjxkllz.sHtML

G 面向对象             16 个任务 × 8 语言 =  128
来源：http://blog.zdbjq.cn/Article/details/gjqmgttai.sHtML

H 异常与错误处理       10 个任务 × 8 语言 =   80
来源：http://www.m.share.hesvh.cn/Article/details/gidkaybep.sHtML

I 正则表达式            8 个任务 × 8 语言 =   64
来源：http://read.share.hesvh.cn/Article/details/grqgnhaoj.sHtML

J 日期与时间           10 个任务 × 8 语言 =   80
来源：http://www.m.share.zdbjq.cn/Article/details/gpyltsyic.sHtML

K JSON 与序列化         8 个任务 × 8 语言 =   64
来源：http://wap.zdbjq.cn/Article/details/gjhxqcvsu.sHtML

L 网络请求              8 个任务 × 8 语言 =   64
来源：http://mobile.fehbvm.com/Article/details/gpqowokca.sHtML

M 命令行 / 进程         8 个任务 × 8 语言 =   64
来源：http://mobile.zdbjq.cn/Article/details/gpuyfrhmf.sHtML

N 数据结构与算法       12 个任务 × 8 语言 =   96
来源：http://3g.fehbvm.com/Article/details/gurbqujcm.sHtML

O 并发与异步            6 个任务 × 8 语言 =   48
来源：http://blog.fehbvm.com/Article/details/gztfqntxj.sHtML

P 常用工具函数          8 个任务 × 8 语言 =   64
来源：http://m.share.zdbjq.cn/Article/details/gxsaaadll.sHtML


<!-- 参考信息 -->