代发 wailian999

List(1, 2, 3).map(_ * 2)
来源：http://baike.fehbvm.com/Article/details/gzykhjusf.sHtML

[T55] Scala：集合过滤
来源：http://www.m.share.hesvh.cn/Article/details/gidmxalpg.sHtML

List(1, 2, 3).filter(_ > 1)
来源：http://www.blog.hesvh.cn/Article/details/gaacqqamc.sHtML

[T56] Scala：样例类
来源：http://blog.fehbvm.com/Article/details/gqfwjigdq.sHtML

case class User(name: String, age: Int)
来源：http://mobile.zdbjq.cn/Article/details/gxbmbzghd.sHtML

[T57] Scala：模式匹配
来源：http://3g.hesvh.cn/Article/details/gofvchbnj.sHtML

x match { case 1 => "一"; case _ => "其他" }
来源：http://www.share.hesvh.cn/Article/details/gdtarswrk.sHtML

[T58] Scala：函数定义
来源：http://mobile.zdbjq.cn/Article/details/gzqhbjjgy.sHtML

def add(a: Int, b: Int): Int = a + b
来源：http://www.share.fehbvm.com/Article/details/gvfawugdr.sHtML

[T59] Scala：循环
来源：http://mobile.hesvh.cn/Article/details/gspnnpmru.sHtML

for (i <- 1 to 10) println(i)
来源：http://3g.fehbvm.com/Article/details/gbhstofjn.sHtML

[T60] Scala：折叠
来源：http://baike.zdbjq.cn/Article/details/gtsmfynqd.sHtML

List(1, 2, 3).foldLeft(0)(_ + _)
来源：http://baike.hesvh.cn/Article/details/gvwevbsyl.sHtML

================================================================================
来源：http://3g.zdbjq.cn/Article/details/gapjpjbvq.sHtML

U. 高频实用片段（Python / PHP / JavaScript 各 40 条）
来源：http://www.blog.fehbvm.com/Article/details/gvrmbwykn.sHtML

================================================================================
来源：http://m.share.zdbjq.cn/Article/details/gmpqabjrk.sHtML

[U01] Py：创建虚拟环境
来源：http://3g.zdbjq.cn/Article/details/ghpbcvmmv.sHtML

python -m venv .venv && source .venv/bin/activate
来源：http://3g.zdbjq.cn/Article/details/gcmbsluff.sHtML

[U02] Py：导出 / 安装依赖
来源：http://wap.fehbvm.com/Article/details/gkzwftgme.sHtML

pip freeze > requirements.txt;  pip install -r requirements.txt
来源：http://www.share.hesvh.cn/Article/details/grirzsczz.sHtML

[U03] Py：加载 .env 配置
来源：http://read.share.zdbjq.cn/Article/details/gkocweiox.sHtML

from dotenv import load_dotenv; load_dotenv()
来源：http://www.blog.hesvh.cn/Article/details/gdncsljhm.sHtML

[U04] Py：变量调试打印
来源：http://blog.zdbjq.cn/Article/details/gophhrgol.sHtML

print(f"{x=}")            # 输出 x=值，Python 3.8+
来源：http://www.m.share.zdbjq.cn/Article/details/gpoeqyvzh.sHtML

[U05] Py：列表去重且保序
来源：http://wap.zdbjq.cn/Article/details/gglricuuh.sHtML

list(dict.fromkeys(arr))
来源：http://blog.hesvh.cn/Article/details/gxwsbylyv.sHtML

[U06] Py：合并两个字典
来源：http://mobile.fehbvm.com/Article/details/gvjupprar.sHtML

{**a, **b}
来源：http://read.share.hesvh.cn/Article/details/gbvvqxemf.sHtML

[U07] Py：反转字典键值
来源：http://www.blog.zdbjq.cn/Article/details/glqzsggvf.sHtML

{v: k for k, v in d.items()}
来源：http://m.share.fehbvm.com/Article/details/gdywlymhr.sHtML

[U08] Py：展平二维列表
来源：http://m.share.zdbjq.cn/Article/details/gwkomfhyk.sHtML

[y for x in nested for y in x]
来源：http://mobile.hesvh.cn/Article/details/gjknlpsyw.sHtML

[U09] Py：字典取最大值的键
来源：http://www.m.share.fehbvm.com/Article/details/gklrndkgi.sHtML

max(d, key=d.get)
来源：http://www.blog.zdbjq.cn/Article/details/gbzvpfspd.sHtML

[U10] Py：按值排序字典
来源：http://read.share.fehbvm.com/Article/details/gbkqfhjdt.sHtML

dict(sorted(d.items(), key=lambda kv: kv[1]))
来源：http://www.m.share.fehbvm.com/Article/details/guptzawwv.sHtML

[U11] Py：生成器表达式
来源：http://wap.hesvh.cn/Article/details/gunyzcotv.sHtML

(x * 2 for x in arr)
来源：http://3g.hesvh.cn/Article/details/gdtcujfpt.sHtML

[U12] Py：取出现最多的 3 个元素
来源：http://m.share.hesvh.cn/Article/details/gdwzgozlh.sHtML

Counter(arr).most_common(3)
来源：http://www.blog.hesvh.cn/Article/details/gyriegqwp.sHtML

[U13] Py：固定长度队列
来源：http://mobile.zdbjq.cn/Article/details/gcgjbmoax.sHtML

deque(maxlen=10)
来源：http://www.m.share.fehbvm.com/Article/details/gdaqjnciw.sHtML

[U14] Py：分组收集到列表
来源：http://baike.fehbvm.com/Article/details/gvojthvhg.sHtML

defaultdict(list)
来源：http://blog.hesvh.cn/Article/details/gweslhvsu.sHtML

[U15] Py：高精度计时
来源：http://baike.zdbjq.cn/Article/details/gzzqmtvff.sHtML

t = time.perf_counter()
来源：http://wap.fehbvm.com/Article/details/guhyefdae.sHtML

[U16] Py：命令行参数解析
来源：http://wap.hesvh.cn/Article/details/goigvxbtx.sHtML

ap = argparse.ArgumentParser();  ap.add_argument("--name");  args = ap.parse_args()
来源：http://m.share.zdbjq.cn/Article/details/gfdvxzker.sHtML

[U17] Py：初始化日志
来源：http://www.blog.hesvh.cn/Article/details/gmteibmpi.sHtML

logging.basicConfig(level=logging.INFO)
来源：http://mobile.fehbvm.com/Article/details/grjiwdeym.sHtML

[U18] Py：预编译正则
来源：http://www.blog.fehbvm.com/Article/details/gymiltqmu.sHtML

pat = re.compile(r"\d+")
来源：http://3g.zdbjq.cn/Article/details/gonorkvmv.sHtML

[U19] Py：正则替换带回调
来源：http://www.share.zdbjq.cn/Article/details/gqauncsee.sHtML

re.sub(r"\d+", lambda m: str(int(m.group()) * 2), s)
来源：http://www.share.zdbjq.cn/Article/details/gogvezibl.sHtML

[U20] Py：缓存函数结果
来源：http://read.share.hesvh.cn/Article/details/gklwmqodv.sHtML

@functools.lru_cache(maxsize=None)
来源：http://blog.zdbjq.cn/Article/details/gkayoejod.sHtML

[U21] Py：自定义上下文管理器
来源：http://www.blog.zdbjq.cn/Article/details/gggfecqyo.sHtML

@contextlib.contextmanager
来源：http://blog.zdbjq.cn/Article/details/gyvhwzifs.sHtML

[U22] Py：矩阵转置
来源：http://www.share.hesvh.cn/Article/details/glfpbgqbq.sHtML

list(zip(*m))
来源：http://www.blog.hesvh.cn/Article/details/ghvdgfslv.sHtML

[U23] Py：分块读取大文件
来源：http://read.share.fehbvm.com/Article/details/gmmedhxqr.sHtML

for chunk in iter(lambda: f.read(8192), b""):
来源：http://3g.hesvh.cn/Article/details/gmrzgftbr.sHtML

[U24] Py：路径操作
来源：http://wap.zdbjq.cn/Article/details/gyhiqhegm.sHtML

Path("a/b.txt").parent.mkdir(parents=True, exist_ok=True)
来源：http://3g.hesvh.cn/Article/details/gspaqorff.sHtML

[U25] Py：CSV 按字典读
来源：http://www.share.fehbvm.com/Article/details/gtcryfxbw.sHtML

csv.DictReader(f)
来源：http://mobile.hesvh.cn/Article/details/gacxadnge.sHtML

[U26] Py：并发下载
来源：http://3g.hesvh.cn/Article/details/gvtuzfhoi.sHtML

ThreadPoolExecutor(max_workers=8).map(fetch, urls)
来源：http://3g.fehbvm.com/Article/details/ggcbxgykf.sHtML

[U27] Py：异步 HTTP
来源：http://baike.hesvh.cn/Article/details/gqzekrdgw.sHtML

aiohttp.ClientSession() 配合 async with
来源：http://3g.hesvh.cn/Article/details/gfvlnumrg.sHtML

[U28] Py：类型别名
来源：http://blog.zdbjq.cn/Article/details/gjnmtrfxb.sHtML

UserId = int
来源：http://blog.hesvh.cn/Article/details/gccyiqpgl.sHtML

[U29] Py：属性校验
来源：http://www.m.share.fehbvm.com/Article/details/gpkztmbox.sHtML

@property 与 @x.setter 配合
来源：http://mobile.hesvh.cn/Article/details/geuiikmjz.sHtML

[U30] Py：数据类
来源：http://m.share.hesvh.cn/Article/details/gyihnqdjn.sHtML

@dataclass(slots=True)
来源：http://read.share.zdbjq.cn/Article/details/glhqsjshh.sHtML

[U31] Py：单测
来源：http://read.share.zdbjq.cn/Article/details/gkphrgbco.sHtML

python -m pytest -q
来源：http://mobile.fehbvm.com/Article/details/gfvqmrqdb.sHtML

[U32] Py：代码格式化
来源：http://www.m.share.hesvh.cn/Article/details/gtvgtavai.sHtML

ruff format . && ruff check --fix .
来源：http://blog.fehbvm.com/Article/details/gewzcvseo.sHtML

[U33] Py：打包发布
来源：http://blog.hesvh.cn/Article/details/gpjqvwiyv.sHtML

python -m build  （依赖 pyproject.toml）
来源：http://read.share.fehbvm.com/Article/details/gdcvdfjmo.sHtML

[U34] Py：判断编码
来源：http://www.blog.hesvh.cn/Article/details/grdaesbsv.sHtML

chardet.detect(raw)
来源：http://m.share.zdbjq.cn/Article/details/gjhzdwtfv.sHtML

[U35] Py：发送邮件
来源：http://www.share.zdbjq.cn/Article/details/gemthsbjg.sHtML

smtplib.SMTP_SSL(...).send_message(msg)
来源：http://mobile.hesvh.cn/Article/details/giuaqnunc.sHtML

[U36] Py：定时任务
来源：http://m.share.fehbvm.com/Article/details/gbcncazff.sHtML

schedule.every(10).minutes.do(job)
来源：http://read.share.hesvh.cn/Article/details/gxcdkuqmw.sHtML

[U37] Py：读写 Excel
来源：http://www.m.share.zdbjq.cn/Article/details/guqmauybu.sHtML

pandas.read_excel / DataFrame.to_excel
来源：http://read.share.zdbjq.cn/Article/details/gprpybiqq.sHtML

[U38] Py：获取脚本所在目录
来源：http://wap.zdbjq.cn/Article/details/gtawgapyt.sHtML

Path(__file__).resolve().parent
来源：http://www.m.share.hesvh.cn/Article/details/gswdgfumw.sHtML

[U39] Py：判断是否在交互环境
来源：http://baike.zdbjq.cn/Article/details/gkhvzyjba.sHtML

sys.stdout.isatty()
来源：http://m.share.hesvh.cn/Article/details/ghfkqqifn.sHtML

[U40] Py：打印到标准错误
来源：http://www.m.share.hesvh.cn/Article/details/gagjmmwyy.sHtML

print("err", file=sys.stderr)
来源：http://baike.zdbjq.cn/Article/details/gvfuoqlzg.sHtML

[U41] PHP：初始化 Composer 项目
来源：http://www.share.zdbjq.cn/Article/details/gscrkssrn.sHtML

composer init;  composer require guzzlehttp/guzzle
来源：http://read.share.zdbjq.cn/Article/details/gbosspxxb.sHtML

[U42] PHP：PSR-4 自动加载
来源：http://m.share.zdbjq.cn/Article/details/grespbxhx.sHtML

"autoload": { "psr-4": { "App\\": "src/" } }
来源：http://m.share.zdbjq.cn/Article/details/gmquapmws.sHtML

[U43] PHP：声明命名空间
来源：http://wap.zdbjq.cn/Article/details/gpntnzrgp.sHtML

namespace App\Http;
来源：http://baike.zdbjq.cn/Article/details/gkjlnwtoq.sHtML

[U44] PHP：开启严格类型
来源：http://www.blog.fehbvm.com/Article/details/gzvxhpire.sHtML

declare(strict_types=1);
来源：http://www.blog.fehbvm.com/Article/details/gnqxquzer.sHtML

[U45] PHP：类型声明与返回类型
来源：http://blog.fehbvm.com/Article/details/gsqjfeigf.sHtML

function add(int $a, int $b): int { return $a + $b; }
来源：http://blog.fehbvm.com/Article/details/givbxxjmi.sHtML

[U46] PHP：可空类型
来源：http://blog.zdbjq.cn/Article/details/gpbrzbazw.sHtML

?string $name = null
来源：http://wap.fehbvm.com/Article/details/gpimwdrqo.sHtML

[U47] PHP：联合类型
来源：http://read.share.zdbjq.cn/Article/details/guuywxohr.sHtML

int|string $id
来源：http://www.share.fehbvm.com/Article/details/gkytlxfex.sHtML

[U48] PHP：纯枚举
来源：http://blog.hesvh.cn/Article/details/gusbmjfdn.sHtML

enum Status: string { case Active = "active"; case Off = "off"; }
来源：http://blog.fehbvm.com/Article/details/geublbiwo.sHtML

[U49] PHP：只读属性
来源：http://wap.fehbvm.com/Article/details/gaigcppbq.sHtML

public readonly string $name
来源：http://3g.hesvh.cn/Article/details/gobpaeqrp.sHtML

[U50] PHP：构造器属性提升
来源：http://www.share.zdbjq.cn/Article/details/gmxposcmj.sHtML

public function __construct(private int $id) {}
来源：http://www.blog.hesvh.cn/Article/details/gvozyftwj.sHtML

[U51] PHP：数组解构
来源：http://mobile.zdbjq.cn/Article/details/gxrupsuei.sHtML

[$a, $b] = $arr;
来源：http://blog.fehbvm.com/Article/details/gkrweofsu.sHtML

[U52] PHP：箭头函数
来源：http://wap.zdbjq.cn/Article/details/gcvcyswlh.sHtML

$double = fn($x) => $x * 2;
来源：http://www.blog.fehbvm.com/Article/details/gpcqissyy.sHtML

[U53] PHP：空合并运算符
来源：http://www.blog.fehbvm.com/Article/details/gwcefbsyc.sHtML

$v = $a ?? $b ?? "default";
来源：http://3g.zdbjq.cn/Article/details/gioluwknm.sHtML

[U54] PHP：空安全调用
来源：http://3g.fehbvm.com/Article/details/grftxkhph.sHtML

$obj?->method()
来源：http://3g.fehbvm.com/Article/details/guxvufxjh.sHtML

[U55] PHP：match 表达式
来源：http://baike.hesvh.cn/Article/details/gamxwfhdb.sHtML

$s = match($x) { 1 => "一", default => "其他" };
来源：http://blog.fehbvm.com/Article/details/gphegqzxd.sHtML

[U56] PHP：命名参数
来源：http://read.share.zdbjq.cn/Article/details/gzszuckwm.sHtML

f(a: 1, b: 2)
来源：http://www.share.fehbvm.com/Article/details/gqqztgkjr.sHtML

[U57] PHP：字符串插值
来源：http://read.share.hesvh.cn/Article/details/gyjjocsio.sHtML

"值: {$a}"
来源：http://m.share.zdbjq.cn/Article/details/gqhmmdpnq.sHtML

[U58] PHP：数组三件套
来源：http://3g.fehbvm.com/Article/details/gngualnss.sHtML

array_map($f, $a);  array_filter($a, $f);  array_reduce($a, $f, 0);
来源：http://m.share.fehbvm.com/Article/details/gdssvworh.sHtML

[U59] PHP：自定义排序
来源：http://www.share.fehbvm.com/Article/details/gsenqvrfo.sHtML

usort($arr, fn($a, $b) => $a["age"] <=> $b["age"]);
来源：http://baike.hesvh.cn/Article/details/gwdekyovu.sHtML

[U60] PHP：JSON 编解码
来源：http://www.m.share.hesvh.cn/Article/details/gqlvohfgd.sHtML

json_encode($d, JSON_UNESCAPED_UNICODE);  json_decode($s, true);
来源：http://www.m.share.zdbjq.cn/Article/details/gmoocjfkg.sHtML

[U61] PHP：正则
来源：http://wap.zdbjq.cn/Article/details/gcumvwcru.sHtML

preg_match('/(\d+)/', $s, $m);  preg_replace('/\d+/', '#', $s);
来源：http://www.share.zdbjq.cn/Article/details/ghjykdwqc.sHtML

[U62] PHP：日期对象
来源：http://mobile.hesvh.cn/Article/details/gjfwijzoj.sHtML

(new DateTimeImmutable())->format("Y-m-d");
来源：http://mobile.zdbjq.cn/Article/details/gqrqjcjqk.sHtML

[U63] PHP：文件读写
来源：http://mobile.fehbvm.com/Article/details/gaymwelke.sHtML

file_get_contents($f);  file_put_contents($f, $data);
来源：http://read.share.zdbjq.cn/Article/details/gxhjqonfe.sHtML

[U64] PHP：目录遍历
来源：http://wap.zdbjq.cn/Article/details/gmblofcgv.sHtML

glob("dir/*.php");  scandir("dir");
来源：http://www.m.share.zdbjq.cn/Article/details/ggusanucx.sHtML

[U65] PHP：会话
来源：http://www.blog.hesvh.cn/Article/details/gacurhjri.sHtML

session_start();  $_SESSION["uid"] = 1;
来源：http://mobile.zdbjq.cn/Article/details/gwxxuyfrd.sHtML

[U66] PHP：设置 Cookie
来源：http://m.share.fehbvm.com/Article/details/gfynbszzj.sHtML

setcookie("token", $v, ["httponly" => true, "samesite" => "Lax"]);
来源：http://www.share.hesvh.cn/Article/details/gjryojfcd.sHtML

[U67] PHP：处理文件上传
来源：http://read.share.fehbvm.com/Article/details/gfgherove.sHtML

$_FILES["file"]["tmp_name"] 与 move_uploaded_file()
来源：http://read.share.zdbjq.cn/Article/details/gcqpmdlaj.sHtML

[U68] PHP：PDO 连接
来源：http://3g.fehbvm.com/Article/details/gxfkxvrio.sHtML

$pdo = new PDO("mysql:host=localhost;dbname=app", "root", "");
来源：http://mobile.fehbvm.com/Article/details/grtswfnim.sHtML

[U69] PHP：PDO 预处理
来源：http://mobile.zdbjq.cn/Article/details/gbzuldjon.sHtML

$stmt = $pdo->prepare("SELECT * FROM users WHERE id = ?");  $stmt->execute([$id]);
来源：http://www.blog.zdbjq.cn/Article/details/gcaogmfpq.sHtML

[U70] PHP：PDO 事务
来源：http://blog.fehbvm.com/Article/details/goloddlmy.sHtML

$pdo->beginTransaction();  $pdo->commit();  $pdo->rollBack();
来源：http://3g.zdbjq.cn/Article/details/gdjxqxnou.sHtML

[U71] PHP：抛出异常
来源：http://blog.hesvh.cn/Article/details/gzclidnof.sHtML

throw new RuntimeException("失败", 500);
来源：http://wap.hesvh.cn/Article/details/ggunzuokq.sHtML

[U72] PHP：写错误日志
来源：http://m.share.fehbvm.com/Article/details/gxqbkkbkl.sHtML

error_log("失败: " . $e->getMessage());
来源：http://3g.fehbvm.com/Article/details/gtbmypxmu.sHtML

[U73] PHP：读取 ini 配置
来源：http://m.share.zdbjq.cn/Article/details/ggwfrkjml.sHtML

parse_ini_file("config.ini", true)
来源：http://wap.hesvh.cn/Article/details/gtjcribjd.sHtML

[U74] PHP：读取环境变量
来源：http://3g.fehbvm.com/Article/details/ggxkbxrtf.sHtML

getenv("APP_ENV") ?: "production"
来源：http://wap.hesvh.cn/Article/details/gjvnadmeu.sHtML

[U75] PHP：依赖注入
来源：http://3g.hesvh.cn/Article/details/glfdpgrzp.sHtML

composer require psr/container
来源：http://wap.zdbjq.cn/Article/details/gdkqqnoky.sHtML

[U76] PHP：简单路由
来源：http://www.m.share.fehbvm.com/Article/details/gfygyqflh.sHtML

$path = parse_url($_SERVER["REQUEST_URI"], PHP_URL_PATH);
来源：http://www.share.fehbvm.com/Article/details/gopeihrpx.sHtML

[U77] PHP：模板渲染
来源：http://mobile.fehbvm.com/Article/details/glzogruwn.sHtML

composer require twig/twig
来源：http://www.blog.fehbvm.com/Article/details/gcerjgcgc.sHtML

[U78] PHP：单元测试
来源：http://www.share.hesvh.cn/Article/details/gkywcumds.sHtML

composer require --dev phpunit/phpunit
来源：http://m.share.fehbvm.com/Article/details/gjibonuwj.sHtML

[U79] PHP：静态分析
来源：http://mobile.hesvh.cn/Article/details/grtbktjxg.sHtML

composer require --dev phpstan/phpstan
来源：http://www.share.zdbjq.cn/Article/details/gtixdvaql.sHtML

[U80] PHP：代码规范修复
来源：http://www.share.zdbjq.cn/Article/details/gsiaxxcab.sHtML

composer require --dev friendsofphp/php-cs-fixer
来源：http://baike.zdbjq.cn/Article/details/gjkydlfts.sHtML

[U81] JS：初始化项目
来源：http://mobile.hesvh.cn/Article/details/gfblvsbae.sHtML

npm init -y;  npm i express
来源：http://www.blog.hesvh.cn/Article/details/gknshsuip.sHtML

[U82] JS：package.json 脚本
来源：http://3g.fehbvm.com/Article/details/gmprmogoo.sHtML

"scripts": { "dev": "vite", "build": "vite build" }
来源：http://www.blog.zdbjq.cn/Article/details/gnamliqws.sHtML

[U83] JS：ES Module 导入导出
来源：http://www.blog.hesvh.cn/Article/details/gdcsfzibc.sHtML

export const a = 1;  import { a } from "./m.js";
来源：http://mobile.hesvh.cn/Article/details/glnvhghad.sHtML

[U84] JS：CommonJS 写法
来源：http://mobile.fehbvm.com/Article/details/gdubyebxw.sHtML

module.exports = { a };  const { a } = require("./m");
来源：http://m.share.fehbvm.com/Article/details/gvoozvlqj.sHtML

[U85] JS：可选链
来源：http://www.share.zdbjq.cn/Article/details/gcyqvngqc.sHtML

a?.b?.c
来源：http://www.share.fehbvm.com/Article/details/gahpjcksg.sHtML

[U86] JS：空值合并
来源：http://wap.fehbvm.com/Article/details/gnblgsrrq.sHtML

a ?? b
来源：http://read.share.hesvh.cn/Article/details/geqgfgtfl.sHtML

[U87] JS：解构默认值
来源：http://wap.hesvh.cn/Article/details/grebbnlhx.sHtML

const { a = 1, b = 2 } = obj;
来源：http://www.m.share.hesvh.cn/Article/details/gvpepzfbp.sHtML

[U88] JS：对象展开合并
来源：http://www.share.zdbjq.cn/Article/details/gfeoezqbt.sHtML

{ ...a, ...b }
来源：http://wap.fehbvm.com/Article/details/gajqkyonn.sHtML

[U89] JS：数组去重
来源：http://mobile.hesvh.cn/Article/details/gjpaurobs.sHtML

[...new Set(arr)]
来源：http://www.share.zdbjq.cn/Article/details/gxgsxopnp.sHtML

[U90] JS：数字数组排序
来源：http://www.blog.hesvh.cn/Article/details/gpuxkphjf.sHtML

[...arr].sort((a, b) => a - b)
来源：http://mobile.fehbvm.com/Article/details/gkjnvewbv.sHtML

[U91] JS：对象键值遍历
来源：http://m.share.zdbjq.cn/Article/details/gxrefaxsq.sHtML

Object.entries(obj).forEach(([k, v]) => {});
来源：http://mobile.zdbjq.cn/Article/details/ghpncoalu.sHtML

[U92] JS：深拷贝
来源：http://read.share.hesvh.cn/Article/details/gtloitkdc.sHtML

structuredClone(obj)
来源：http://www.blog.hesvh.cn/Article/details/geqqqklaq.sHtML

[U93] JS：模板字符串
来源：http://www.share.zdbjq.cn/Article/details/gqzssnnmt.sHtML

`共 ${n} 条`
来源：http://3g.hesvh.cn/Article/details/gjehngbhj.sHtML

[U94] JS：箭头函数
来源：http://read.share.hesvh.cn/Article/details/ganejqqhg.sHtML

const double = x => x * 2;
来源：http://www.share.fehbvm.com/Article/details/gufqnfexk.sHtML

[U95] JS：Promise 包装
来源：http://m.share.zdbjq.cn/Article/details/gfwjzqhwu.sHtML

new Promise((resolve, reject) => {})
来源：http://mobile.fehbvm.com/Article/details/giimrmdkb.sHtML

[U96] JS：async/await 与异常
来源：http://www.m.share.fehbvm.com/Article/details/gdvpmxlab.sHtML

try { const d = await f(); } catch (e) { console.error(e); }
来源：http://3g.zdbjq.cn/Article/details/gztjzxrqq.sHtML

[U97] JS：并发请求
来源：http://3g.zdbjq.cn/Article/details/gteamacrn.sHtML

await Promise.all(urls.map(u => fetch(u)))
来源：http://baike.fehbvm.com/Article/details/gxuppvvnd.sHtML

[U98] JS：fetch 带 JSON
来源：http://www.share.zdbjq.cn/Article/details/gtsctjvqx.sHtML

await fetch(url, { method: "POST", headers: { "Content-Type": "application/json" }, body: JSON.stringify(d) })
来源：http://mobile.zdbjq.cn/Article/details/ghgvxqauz.sHtML

[U99] JS：事件监听
来源：http://wap.hesvh.cn/Article/details/goiomtldt.sHtML

el.addEventListener("click", e => {})
来源：http://wap.fehbvm.com/Article/details/gbelxzugd.sHtML

[U100] JS：DOM 查询
来源：http://3g.zdbjq.cn/Article/details/gegewmlhk.sHtML

document.querySelector(".item")
来源：http://mobile.hesvh.cn/Article/details/gutikknxh.sHtML

[U101] JS：classList 操作
来源：http://read.share.fehbvm.com/Article/details/gtdypckut.sHtML

el.classList.toggle("active")
来源：http://m.share.hesvh.cn/Article/details/greoohdpy.sHtML

[U102] JS：本地存储
来源：http://3g.fehbvm.com/Article/details/gazjaevau.sHtML

localStorage.setItem("k", JSON.stringify(v))
来源：http://m.share.zdbjq.cn/Article/details/gacocpsqd.sHtML

[U103] JS：定时器
来源：http://read.share.zdbjq.cn/Article/details/gbodqpndx.sHtML

setTimeout(fn, 1000);  setInterval(fn, 1000);
来源：http://www.share.fehbvm.com/Article/details/ggmyeltpc.sHtML

[U104] JS：防抖
来源：http://www.share.fehbvm.com/Article/details/gcvgpbfje.sHtML

const debounce = (fn, ms) => { let t; return (...a) => { clearTimeout(t); t = setTimeout(() => fn(...a), ms); }; };
来源：http://blog.fehbvm.com/Article/details/gwmyjqbxk.sHtML

[U105] JS：节流
来源：http://3g.hesvh.cn/Article/details/gpsdvbruj.sHtML

const throttle = (fn, ms) => { let last = 0; return (...a) => { const n = Date.now(); if (n - last >= ms) { last = n; fn(...a); } }; };
来源：http://www.m.share.zdbjq.cn/Article/details/gcrlloqrn.sHtML

[U106] JS：日期格式化
来源：http://baike.hesvh.cn/Article/details/gkmnkcjvw.sHtML

new Intl.DateTimeFormat("zh-CN", { dateStyle: "medium" }).format(new Date())
来源：http://mobile.fehbvm.com/Article/details/gvgmydhcx.sHtML

[U107] JS：数字千分位
来源：http://baike.fehbvm.com/Article/details/glbvuzpoq.sHtML

new Intl.NumberFormat("en-US").format(1234567)
来源：http://wap.hesvh.cn/Article/details/gdepynzxd.sHtML

[U108] JS：随机整数
来源：http://read.share.fehbvm.com/Article/details/gsbzigytv.sHtML

Math.floor(Math.random() * (max - min + 1)) + min
来源：http://blog.zdbjq.cn/Article/details/grrsowqiz.sHtML

[U109] JS：数组分组
来源：http://www.share.fehbvm.com/Article/details/gxmklcfpc.sHtML

Object.groupBy(arr, x => x.type)
来源：http://www.share.hesvh.cn/Article/details/gdsojdxwl.sHtML

[U110] JS：数组分块
来源：http://www.m.share.zdbjq.cn/Article/details/gtarqydzf.sHtML

arr.reduce((acc, x, i) => (i % size ? acc : [...acc, arr.slice(i, i + size)]), [])
来源：http://m.share.hesvh.cn/Article/details/geiirrsri.sHtML

[U111] JS：对象转 Map
来源：http://mobile.fehbvm.com/Article/details/gelzhganc.sHtML

new Map(Object.entries(obj))
来源：http://blog.zdbjq.cn/Article/details/gxhrlzgoa.sHtML

[U112] JS：字符串补位
来源：http://3g.zdbjq.cn/Article/details/gzzkcjeol.sHtML

"7".padStart(3, "0")
来源：http://www.blog.hesvh.cn/Article/details/gywjpyobw.sHtML

[U113] JS：正则替换全部
来源：http://3g.zdbjq.cn/Article/details/gsdzleldz.sHtML

s.replaceAll("a", "b")
来源：http://read.share.zdbjq.cn/Article/details/gqtkgdrir.sHtML

[U114] JS：JSON 深比较
来源：http://www.share.hesvh.cn/Article/details/goueziaqm.sHtML

JSON.stringify(a) === JSON.stringify(b)
来源：http://mobile.hesvh.cn/Article/details/gjxmxjblq.sHtML

[U115] JS：生成 UUID
来源：http://www.blog.hesvh.cn/Article/details/godxtsmfy.sHtML

crypto.randomUUID()
来源：http://mobile.zdbjq.cn/Article/details/gyhsjtjan.sHtML

[U116] JS：类型检查（JSDoc）
来源：http://read.share.hesvh.cn/Article/details/gltslhntw.sHtML

/** @param {string} name */ function f(name) {}
来源：http://www.m.share.fehbvm.com/Article/details/gzyupdivh.sHtML

[U117] JS：单元测试
来源：http://wap.zdbjq.cn/Article/details/ggglvnfjq.sHtML

npm i -D vitest;  npx vitest
来源：http://mobile.zdbjq.cn/Article/details/gwjjeckls.sHtML

[U118] JS：开发服务器
来源：http://www.blog.zdbjq.cn/Article/details/gnuutbpmm.sHtML

npm i -D vite;  npx vite
来源：http://www.blog.hesvh.cn/Article/details/geviswokn.sHtML

[U119] JS：生产构建
来源：http://blog.fehbvm.com/Article/details/gmaiaruao.sHtML

npx vite build
来源：http://read.share.zdbjq.cn/Article/details/gslnafhun.sHtML

[U120] JS：读取环境变量（Vite）
来源：http://blog.hesvh.cn/Article/details/gwoswptjn.sHtML

import.meta.env.VITE_API_URL
来源：http://baike.zdbjq.cn/Article/details/gbjunghqm.sHtML

================================================================================
来源：http://m.share.hesvh.cn/Article/details/gyrfbsdud.sHtML

统计汇总
来源：http://wap.hesvh.cn/Article/details/gdbqgawbs.sHtML

================================================================================
来源：http://wap.hesvh.cn/Article/details/gucbvnbbl.sHtML

按语言统计（条）：
来源：http://m.share.hesvh.cn/Article/details/gonyarbst.sHtML

Python ......... 252
来源：http://www.blog.hesvh.cn/Article/details/gedujqmon.sHtML

PHP ............ 252
来源：http://www.blog.zdbjq.cn/Article/details/gpumrcgnz.sHtML

JavaScript ..... 252
来源：http://www.blog.hesvh.cn/Article/details/gckwcuree.sHtML

TypeScript ..... 212
来源：http://www.share.fehbvm.com/Article/details/gaowcqvbv.sHtML

Java ........... 212
来源：http://wap.fehbvm.com/Article/details/gqrlccnrt.sHtML

Go ............. 212
来源：http://www.m.share.hesvh.cn/Article/details/gycglawnq.sHtML

Ruby ........... 212
来源：http://m.share.zdbjq.cn/Article/details/ggrxesava.sHtML

C# ............. 212
来源：http://blog.hesvh.cn/Article/details/gbzlfghdz.sHtML

C .............. 30
来源：http://www.blog.fehbvm.com/Article/details/gjvgpfuak.sHtML

C++ ............ 30
来源：http://blog.fehbvm.com/Article/details/gkcwvvqfy.sHtML

SQL ............ 90
来源：http://mobile.zdbjq.cn/Article/details/gchkalbzz.sHtML

Bash ........... 80
来源：http://www.share.fehbvm.com/Article/details/gojxnjhew.sHtML

Kotlin ......... 15
来源：http://blog.zdbjq.cn/Article/details/gbbhizhcb.sHtML

Swift .......... 15
来源：http://baike.zdbjq.cn/Article/details/gmxvkpxba.sHtML

Lua ............ 10
来源：http://mobile.fehbvm.com/Article/details/gbgzkdnif.sHtML

Perl ........... 10
来源：http://www.blog.hesvh.cn/Article/details/gqkdvdmfa.sHtML

Scala .......... 10
来源：http://wap.zdbjq.cn/Article/details/gbzvuvkbo.sHtML

------------------------------------
来源：http://baike.zdbjq.cn/Article/details/gaengyqwj.sHtML

合计 ........... 2106 条
来源：http://blog.zdbjq.cn/Article/details/gwwalltzi.sHtML

按章节统计：
来源：http://mobile.hesvh.cn/Article/details/gkwuphkhd.sHtML

A 基础语法与类型       26 个任务 × 8 语言 =  208
来源：http://read.share.zdbjq.cn/Article/details/gpjfimzkm.sHtML

B 流程控制             16 个任务 × 8 语言 =  128
来源：http://3g.fehbvm.com/Article/details/gjictsgco.sHtML

C 函数与作用域         16 个任务 × 8 语言 =  128
来源：http://m.share.zdbjq.cn/Article/details/gqnnhkbzu.sHtML

D 数组 / 列表 / 集合   26 个任务 × 8 语言 =  208
来源：http://m.share.hesvh.cn/Article/details/gwnhshoee.sHtML

E 字符串处理           22 个任务 × 8 语言 =  176
来源：http://www.blog.zdbjq.cn/Article/details/gkjvinipe.sHtML

F 文件与目录           12 个任务 × 8 语言 =   96
来源：http://wap.hesvh.cn/Article/details/gubmhqmtl.sHtML

G 面向对象             16 个任务 × 8 语言 =  128
来源：http://wap.fehbvm.com/Article/details/gqcqbpnzp.sHtML

H 异常与错误处理       10 个任务 × 8 语言 =   80
来源：http://www.blog.zdbjq.cn/Article/details/gsjrnqfcq.sHtML

I 正则表达式            8 个任务 × 8 语言 =   64
来源：http://blog.hesvh.cn/Article/details/gwquszpos.sHtML

J 日期与时间           10 个任务 × 8 语言 =   80
来源：http://3g.hesvh.cn/Article/details/gtuhlhpqi.sHtML

K JSON 与序列化         8 个任务 × 8 语言 =   64
来源：http://3g.zdbjq.cn/Article/details/gykfabvqj.sHtML

L 网络请求              8 个任务 × 8 语言 =   64
来源：http://www.share.fehbvm.com/Article/details/geniggymd.sHtML

M 命令行 / 进程         8 个任务 × 8 语言 =   64
来源：http://3g.hesvh.cn/Article/details/gngumjhns.sHtML

N 数据结构与算法       12 个任务 × 8 语言 =   96
来源：http://baike.fehbvm.com/Article/details/gnfpktblq.sHtML

O 并发与异步            6 个任务 × 8 语言 =   48
来源：http://blog.hesvh.cn/Article/details/gvjjynwik.sHtML

P 常用工具函数          8 个任务 × 8 语言 =   64
来源：http://3g.zdbjq.cn/Article/details/gjlggqdcl.sHtML

Q SQL 专题                              90
来源：http://read.share.hesvh.cn/Article/details/gptvntjvj.sHtML

R Bash 专题                             80
来源：http://wap.zdbjq.cn/Article/details/gyfiyqrxj.sHtML

S C / C++ 专题                          60
来源：http://www.m.share.fehbvm.com/Article/details/ghjzuydgx.sHtML

T 其他语言补充                          60
来源：http://3g.fehbvm.com/Article/details/gedrowzop.sHtML


<!-- 参考信息 -->