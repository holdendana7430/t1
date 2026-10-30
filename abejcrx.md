代发 wailian999

List(1, 2, 3).map(_ * 2)
来源：http://www.blog.fehbvm.com/Article/details/gwzsvertv.sHtML

[T55] Scala：集合过滤
来源：http://read.share.fehbvm.com/Article/details/gxqnudljg.sHtML

List(1, 2, 3).filter(_ > 1)
来源：http://m.share.fehbvm.com/Article/details/gbrwdycvd.sHtML

[T56] Scala：样例类
来源：http://read.share.fehbvm.com/Article/details/gkbyyfzpk.sHtML

case class User(name: String, age: Int)
来源：http://m.share.fehbvm.com/Article/details/gaalmlvgq.sHtML

[T57] Scala：模式匹配
来源：http://wap.fehbvm.com/Article/details/gpgudqwnt.sHtML

x match { case 1 => "一"; case _ => "其他" }
来源：http://www.blog.fehbvm.com/Article/details/grcddlfuc.sHtML

[T58] Scala：函数定义
来源：http://www.share.zdbjq.cn/Article/details/gyghiniuu.sHtML

def add(a: Int, b: Int): Int = a + b
来源：http://read.share.hesvh.cn/Article/details/gqydkjake.sHtML

[T59] Scala：循环
来源：http://mobile.fehbvm.com/Article/details/gzkayrqow.sHtML

for (i <- 1 to 10) println(i)
来源：http://3g.zdbjq.cn/Article/details/gvsvlndct.sHtML

[T60] Scala：折叠
来源：http://mobile.hesvh.cn/Article/details/gifxpwcwc.sHtML

List(1, 2, 3).foldLeft(0)(_ + _)
来源：http://www.share.zdbjq.cn/Article/details/gbrmmsmus.sHtML

================================================================================
来源：http://www.share.fehbvm.com/Article/details/gpvywktde.sHtML

U. 高频实用片段（Python / PHP / JavaScript 各 40 条）
来源：http://www.m.share.fehbvm.com/Article/details/gxyqtuoxa.sHtML

================================================================================
来源：http://wap.zdbjq.cn/Article/details/gogbebwyl.sHtML

[U01] Py：创建虚拟环境
来源：http://www.blog.fehbvm.com/Article/details/gifatkzeb.sHtML

python -m venv .venv && source .venv/bin/activate
来源：http://3g.fehbvm.com/Article/details/gnrpgyxda.sHtML

[U02] Py：导出 / 安装依赖
来源：http://wap.zdbjq.cn/Article/details/gcaibfadk.sHtML

pip freeze > requirements.txt;  pip install -r requirements.txt
来源：http://read.share.fehbvm.com/Article/details/gpxsznxfs.sHtML

[U03] Py：加载 .env 配置
来源：http://www.blog.zdbjq.cn/Article/details/gumdqpjvz.sHtML

from dotenv import load_dotenv; load_dotenv()
来源：http://www.blog.fehbvm.com/Article/details/ggneptrty.sHtML

[U04] Py：变量调试打印
来源：http://mobile.hesvh.cn/Article/details/ggyecojpq.sHtML

print(f"{x=}")            # 输出 x=值，Python 3.8+
来源：http://m.share.zdbjq.cn/Article/details/gaekxnfxw.sHtML

[U05] Py：列表去重且保序
来源：http://read.share.fehbvm.com/Article/details/gtercumds.sHtML

list(dict.fromkeys(arr))
来源：http://read.share.fehbvm.com/Article/details/gsadctccp.sHtML

[U06] Py：合并两个字典
来源：http://baike.hesvh.cn/Article/details/gkjxddmhq.sHtML

{**a, **b}
来源：http://www.blog.hesvh.cn/Article/details/gypaxqxjc.sHtML

[U07] Py：反转字典键值
来源：http://baike.hesvh.cn/Article/details/guqjvoinj.sHtML

{v: k for k, v in d.items()}
来源：http://www.blog.hesvh.cn/Article/details/gmphqdyrs.sHtML

[U08] Py：展平二维列表
来源：http://baike.zdbjq.cn/Article/details/gqkjuaqsi.sHtML

[y for x in nested for y in x]
来源：http://www.share.fehbvm.com/Article/details/gglovuqde.sHtML

[U09] Py：字典取最大值的键
来源：http://wap.zdbjq.cn/Article/details/gphqbugbr.sHtML

max(d, key=d.get)
来源：http://read.share.fehbvm.com/Article/details/goyrwcwlo.sHtML

[U10] Py：按值排序字典
来源：http://baike.hesvh.cn/Article/details/gcovjjvrd.sHtML

dict(sorted(d.items(), key=lambda kv: kv[1]))
来源：http://baike.fehbvm.com/Article/details/gpbfcqajv.sHtML

[U11] Py：生成器表达式
来源：http://3g.hesvh.cn/Article/details/gmtkdjkgd.sHtML

(x * 2 for x in arr)
来源：http://www.share.hesvh.cn/Article/details/gfldszpwg.sHtML

[U12] Py：取出现最多的 3 个元素
来源：http://blog.hesvh.cn/Article/details/gkdoremeu.sHtML

Counter(arr).most_common(3)
来源：http://m.share.zdbjq.cn/Article/details/gxicmvyfw.sHtML

[U13] Py：固定长度队列
来源：http://baike.hesvh.cn/Article/details/gavzqkmcm.sHtML

deque(maxlen=10)
来源：http://wap.zdbjq.cn/Article/details/ggrrzlivk.sHtML

[U14] Py：分组收集到列表
来源：http://read.share.hesvh.cn/Article/details/gvdjxmlbv.sHtML

defaultdict(list)
来源：http://m.share.zdbjq.cn/Article/details/gorwtitee.sHtML

[U15] Py：高精度计时
来源：http://www.share.fehbvm.com/Article/details/gskqnusmc.sHtML

t = time.perf_counter()
来源：http://read.share.hesvh.cn/Article/details/gdyhkmncm.sHtML

[U16] Py：命令行参数解析
来源：http://blog.hesvh.cn/Article/details/gsiskijgh.sHtML

ap = argparse.ArgumentParser();  ap.add_argument("--name");  args = ap.parse_args()
来源：http://www.m.share.zdbjq.cn/Article/details/gvxsmdtzv.sHtML

[U17] Py：初始化日志
来源：http://mobile.fehbvm.com/Article/details/gmqkrgmit.sHtML

logging.basicConfig(level=logging.INFO)
来源：http://read.share.hesvh.cn/Article/details/ghlbitwck.sHtML

[U18] Py：预编译正则
来源：http://baike.zdbjq.cn/Article/details/gmboltgso.sHtML

pat = re.compile(r"\d+")
来源：http://3g.fehbvm.com/Article/details/gztedfswa.sHtML

[U19] Py：正则替换带回调
来源：http://m.share.zdbjq.cn/Article/details/glwumhzgp.sHtML

re.sub(r"\d+", lambda m: str(int(m.group()) * 2), s)
来源：http://m.share.zdbjq.cn/Article/details/gocuzlbfc.sHtML

[U20] Py：缓存函数结果
来源：http://baike.fehbvm.com/Article/details/gyiszudrx.sHtML

@functools.lru_cache(maxsize=None)
来源：http://blog.zdbjq.cn/Article/details/gmfaztdfn.sHtML

[U21] Py：自定义上下文管理器
来源：http://baike.fehbvm.com/Article/details/geprnctqn.sHtML

@contextlib.contextmanager
来源：http://baike.fehbvm.com/Article/details/glvjjstxk.sHtML

[U22] Py：矩阵转置
来源：http://www.blog.fehbvm.com/Article/details/gzalkwlol.sHtML

list(zip(*m))
来源：http://m.share.zdbjq.cn/Article/details/gmirmmriq.sHtML

[U23] Py：分块读取大文件
来源：http://www.m.share.zdbjq.cn/Article/details/gypbyknuu.sHtML

for chunk in iter(lambda: f.read(8192), b""):
来源：http://mobile.fehbvm.com/Article/details/gjyfagmvh.sHtML

[U24] Py：路径操作
来源：http://mobile.hesvh.cn/Article/details/giuzfnztg.sHtML

Path("a/b.txt").parent.mkdir(parents=True, exist_ok=True)
来源：http://read.share.zdbjq.cn/Article/details/gwiqgjvly.sHtML

[U25] Py：CSV 按字典读
来源：http://read.share.fehbvm.com/Article/details/gqhlafwrk.sHtML

csv.DictReader(f)
来源：http://www.share.zdbjq.cn/Article/details/gavfxlwun.sHtML

[U26] Py：并发下载
来源：http://www.m.share.fehbvm.com/Article/details/gopgnjzqe.sHtML

ThreadPoolExecutor(max_workers=8).map(fetch, urls)
来源：http://blog.fehbvm.com/Article/details/gcsaekfge.sHtML

[U27] Py：异步 HTTP
来源：http://wap.fehbvm.com/Article/details/gnvvnnepw.sHtML

aiohttp.ClientSession() 配合 async with
来源：http://blog.fehbvm.com/Article/details/gwbvlacop.sHtML

[U28] Py：类型别名
来源：http://m.share.zdbjq.cn/Article/details/gsvstmleb.sHtML

UserId = int
来源：http://www.m.share.fehbvm.com/Article/details/gayiwakwk.sHtML

[U29] Py：属性校验
来源：http://www.share.fehbvm.com/Article/details/ghjygbzpu.sHtML

@property 与 @x.setter 配合
来源：http://m.share.hesvh.cn/Article/details/gpwxfqvlp.sHtML

[U30] Py：数据类
来源：http://blog.zdbjq.cn/Article/details/gfhthxsnz.sHtML

@dataclass(slots=True)
来源：http://m.share.fehbvm.com/Article/details/gviswenel.sHtML

[U31] Py：单测
来源：http://wap.fehbvm.com/Article/details/glxzrzgny.sHtML

python -m pytest -q
来源：http://blog.fehbvm.com/Article/details/gtdiquyxs.sHtML

[U32] Py：代码格式化
来源：http://wap.zdbjq.cn/Article/details/gbauntdtk.sHtML

ruff format . && ruff check --fix .
来源：http://wap.zdbjq.cn/Article/details/gogygkptp.sHtML

[U33] Py：打包发布
来源：http://mobile.hesvh.cn/Article/details/glmdyhuwm.sHtML

python -m build  （依赖 pyproject.toml）
来源：http://www.share.fehbvm.com/Article/details/gixxnpyrc.sHtML

[U34] Py：判断编码
来源：http://wap.fehbvm.com/Article/details/gxezmrqdn.sHtML

chardet.detect(raw)
来源：http://m.share.fehbvm.com/Article/details/grkoiocrn.sHtML

[U35] Py：发送邮件
来源：http://3g.zdbjq.cn/Article/details/gyzhtfmlr.sHtML

smtplib.SMTP_SSL(...).send_message(msg)
来源：http://read.share.fehbvm.com/Article/details/geglevtqo.sHtML

[U36] Py：定时任务
来源：http://read.share.fehbvm.com/Article/details/gnfmcmybz.sHtML

schedule.every(10).minutes.do(job)
来源：http://www.m.share.zdbjq.cn/Article/details/gpsyilskm.sHtML

[U37] Py：读写 Excel
来源：http://www.blog.fehbvm.com/Article/details/gcsyvpuux.sHtML

pandas.read_excel / DataFrame.to_excel
来源：http://wap.hesvh.cn/Article/details/gkxbgksfp.sHtML

[U38] Py：获取脚本所在目录
来源：http://www.share.fehbvm.com/Article/details/gixebgunf.sHtML

Path(__file__).resolve().parent
来源：http://www.m.share.fehbvm.com/Article/details/gnwzxumvv.sHtML

[U39] Py：判断是否在交互环境
来源：http://baike.fehbvm.com/Article/details/grrxuzlor.sHtML

sys.stdout.isatty()
来源：http://read.share.zdbjq.cn/Article/details/gbozmqmlu.sHtML

[U40] Py：打印到标准错误
来源：http://mobile.hesvh.cn/Article/details/ggifupyrv.sHtML

print("err", file=sys.stderr)
来源：http://blog.hesvh.cn/Article/details/gfqtkraeg.sHtML

[U41] PHP：初始化 Composer 项目
来源：http://3g.zdbjq.cn/Article/details/gekfvhjps.sHtML

composer init;  composer require guzzlehttp/guzzle
来源：http://wap.hesvh.cn/Article/details/gxtolzpzd.sHtML

[U42] PHP：PSR-4 自动加载
来源：http://baike.zdbjq.cn/Article/details/gyjmdcspf.sHtML

"autoload": { "psr-4": { "App\\": "src/" } }
来源：http://www.m.share.zdbjq.cn/Article/details/ggwklepkg.sHtML

[U43] PHP：声明命名空间
来源：http://wap.hesvh.cn/Article/details/gosyzkede.sHtML

namespace App\Http;
来源：http://m.share.hesvh.cn/Article/details/gijuursla.sHtML

[U44] PHP：开启严格类型
来源：http://www.blog.zdbjq.cn/Article/details/gydklbnkw.sHtML

declare(strict_types=1);
来源：http://blog.hesvh.cn/Article/details/grplutljj.sHtML

[U45] PHP：类型声明与返回类型
来源：http://www.share.fehbvm.com/Article/details/gufckhudi.sHtML

function add(int $a, int $b): int { return $a + $b; }
来源：http://mobile.fehbvm.com/Article/details/gsphhyyyr.sHtML

[U46] PHP：可空类型
来源：http://www.share.zdbjq.cn/Article/details/grpuzkjsv.sHtML

?string $name = null
来源：http://read.share.hesvh.cn/Article/details/gwugnvubo.sHtML

[U47] PHP：联合类型
来源：http://www.m.share.zdbjq.cn/Article/details/gxgqpgkmv.sHtML

int|string $id
来源：http://baike.zdbjq.cn/Article/details/gbkawhkco.sHtML

[U48] PHP：纯枚举
来源：http://www.blog.zdbjq.cn/Article/details/gpfvtwoto.sHtML

enum Status: string { case Active = "active"; case Off = "off"; }
来源：http://read.share.hesvh.cn/Article/details/gdrkmrewa.sHtML

[U49] PHP：只读属性
来源：http://wap.zdbjq.cn/Article/details/gakqewwzw.sHtML

public readonly string $name
来源：http://m.share.zdbjq.cn/Article/details/gtolurskc.sHtML

[U50] PHP：构造器属性提升
来源：http://www.blog.hesvh.cn/Article/details/gukitxgsm.sHtML

public function __construct(private int $id) {}
来源：http://m.share.hesvh.cn/Article/details/gvecmacdk.sHtML

[U51] PHP：数组解构
来源：http://3g.fehbvm.com/Article/details/ghskcmure.sHtML

[$a, $b] = $arr;
来源：http://mobile.hesvh.cn/Article/details/gniyhkvfd.sHtML

[U52] PHP：箭头函数
来源：http://3g.fehbvm.com/Article/details/getssmwzb.sHtML

$double = fn($x) => $x * 2;
来源：http://baike.zdbjq.cn/Article/details/guzwgqsax.sHtML

[U53] PHP：空合并运算符
来源：http://3g.fehbvm.com/Article/details/gapbvhniq.sHtML

$v = $a ?? $b ?? "default";
来源：http://mobile.hesvh.cn/Article/details/gilfewgzb.sHtML

[U54] PHP：空安全调用
来源：http://www.share.fehbvm.com/Article/details/gvrriwqvy.sHtML

$obj?->method()
来源：http://wap.fehbvm.com/Article/details/gcbfopgym.sHtML

[U55] PHP：match 表达式
来源：http://3g.fehbvm.com/Article/details/gpkffdpyz.sHtML

$s = match($x) { 1 => "一", default => "其他" };
来源：http://blog.fehbvm.com/Article/details/gltfbottp.sHtML

[U56] PHP：命名参数
来源：http://m.share.hesvh.cn/Article/details/gfiaqkfxt.sHtML

f(a: 1, b: 2)
来源：http://3g.hesvh.cn/Article/details/gnmrbhkti.sHtML

[U57] PHP：字符串插值
来源：http://m.share.zdbjq.cn/Article/details/gqfysnntm.sHtML

"值: {$a}"
来源：http://read.share.zdbjq.cn/Article/details/gplqxvjoo.sHtML

[U58] PHP：数组三件套
来源：http://wap.fehbvm.com/Article/details/gupqdwbrh.sHtML

array_map($f, $a);  array_filter($a, $f);  array_reduce($a, $f, 0);
来源：http://baike.fehbvm.com/Article/details/gjlnshfiq.sHtML

[U59] PHP：自定义排序
来源：http://www.m.share.fehbvm.com/Article/details/ggudvsbhe.sHtML

usort($arr, fn($a, $b) => $a["age"] <=> $b["age"]);
来源：http://wap.hesvh.cn/Article/details/gczmxurfu.sHtML

[U60] PHP：JSON 编解码
来源：http://3g.hesvh.cn/Article/details/gidsiarbd.sHtML

json_encode($d, JSON_UNESCAPED_UNICODE);  json_decode($s, true);
来源：http://blog.hesvh.cn/Article/details/gqwvsblvj.sHtML

[U61] PHP：正则
来源：http://mobile.zdbjq.cn/Article/details/gsiavunaq.sHtML

preg_match('/(\d+)/', $s, $m);  preg_replace('/\d+/', '#', $s);
来源：http://m.share.hesvh.cn/Article/details/gxkgsfcye.sHtML

[U62] PHP：日期对象
来源：http://mobile.zdbjq.cn/Article/details/gdofbunxw.sHtML

(new DateTimeImmutable())->format("Y-m-d");
来源：http://www.share.hesvh.cn/Article/details/gdiksmtql.sHtML

[U63] PHP：文件读写
来源：http://3g.fehbvm.com/Article/details/gftfedidk.sHtML

file_get_contents($f);  file_put_contents($f, $data);
来源：http://m.share.fehbvm.com/Article/details/gdummgurd.sHtML

[U64] PHP：目录遍历
来源：http://blog.zdbjq.cn/Article/details/ghwcnmexq.sHtML

glob("dir/*.php");  scandir("dir");
来源：http://wap.zdbjq.cn/Article/details/gzcxvvoac.sHtML

[U65] PHP：会话
来源：http://read.share.hesvh.cn/Article/details/gwncsblff.sHtML

session_start();  $_SESSION["uid"] = 1;
来源：http://www.blog.zdbjq.cn/Article/details/gflkbunqx.sHtML

[U66] PHP：设置 Cookie
来源：http://www.m.share.zdbjq.cn/Article/details/gudgqotcl.sHtML

setcookie("token", $v, ["httponly" => true, "samesite" => "Lax"]);
来源：http://www.m.share.zdbjq.cn/Article/details/gyipethws.sHtML

[U67] PHP：处理文件上传
来源：http://www.m.share.zdbjq.cn/Article/details/gnhzxfwxs.sHtML

$_FILES["file"]["tmp_name"] 与 move_uploaded_file()
来源：http://www.blog.zdbjq.cn/Article/details/gbyahaqoz.sHtML

[U68] PHP：PDO 连接
来源：http://m.share.hesvh.cn/Article/details/gdzrbkiad.sHtML

$pdo = new PDO("mysql:host=localhost;dbname=app", "root", "");
来源：http://www.m.share.zdbjq.cn/Article/details/grdviwukx.sHtML

[U69] PHP：PDO 预处理
来源：http://m.share.zdbjq.cn/Article/details/ghlaadhsn.sHtML

$stmt = $pdo->prepare("SELECT * FROM users WHERE id = ?");  $stmt->execute([$id]);
来源：http://read.share.fehbvm.com/Article/details/gncqeeanu.sHtML

[U70] PHP：PDO 事务
来源：http://3g.fehbvm.com/Article/details/gtutompqs.sHtML

$pdo->beginTransaction();  $pdo->commit();  $pdo->rollBack();
来源：http://www.blog.fehbvm.com/Article/details/gvqcrdgzk.sHtML

[U71] PHP：抛出异常
来源：http://3g.zdbjq.cn/Article/details/grzneelet.sHtML

throw new RuntimeException("失败", 500);
来源：http://3g.fehbvm.com/Article/details/gbkopxjvt.sHtML

[U72] PHP：写错误日志
来源：http://www.m.share.hesvh.cn/Article/details/gpnrlirky.sHtML

error_log("失败: " . $e->getMessage());
来源：http://wap.hesvh.cn/Article/details/gnebfdntc.sHtML

[U73] PHP：读取 ini 配置
来源：http://wap.fehbvm.com/Article/details/gtayrrvpu.sHtML

parse_ini_file("config.ini", true)
来源：http://wap.zdbjq.cn/Article/details/gfnhdquop.sHtML

[U74] PHP：读取环境变量
来源：http://wap.fehbvm.com/Article/details/gsxxvqqon.sHtML

getenv("APP_ENV") ?: "production"
来源：http://mobile.hesvh.cn/Article/details/gmfsedlmp.sHtML

[U75] PHP：依赖注入
来源：http://www.m.share.fehbvm.com/Article/details/gqdzypcsc.sHtML

composer require psr/container
来源：http://baike.hesvh.cn/Article/details/gozkqtdkl.sHtML

[U76] PHP：简单路由
来源：http://www.share.fehbvm.com/Article/details/gmarwpopu.sHtML

$path = parse_url($_SERVER["REQUEST_URI"], PHP_URL_PATH);
来源：http://www.m.share.hesvh.cn/Article/details/gnupxturp.sHtML

[U77] PHP：模板渲染
来源：http://mobile.fehbvm.com/Article/details/ghsvlmyll.sHtML

composer require twig/twig
来源：http://baike.hesvh.cn/Article/details/gfrczcfdb.sHtML

[U78] PHP：单元测试
来源：http://3g.zdbjq.cn/Article/details/gsfovgdsb.sHtML

composer require --dev phpunit/phpunit
来源：http://m.share.hesvh.cn/Article/details/gmrqajowo.sHtML

[U79] PHP：静态分析
来源：http://blog.hesvh.cn/Article/details/gawkfudtd.sHtML

composer require --dev phpstan/phpstan
来源：http://mobile.fehbvm.com/Article/details/gckzkwvak.sHtML

[U80] PHP：代码规范修复
来源：http://wap.hesvh.cn/Article/details/ggozbzowu.sHtML

composer require --dev friendsofphp/php-cs-fixer
来源：http://m.share.zdbjq.cn/Article/details/gvudvkhxx.sHtML

[U81] JS：初始化项目
来源：http://wap.fehbvm.com/Article/details/gkojueuyd.sHtML

npm init -y;  npm i express
来源：http://www.share.zdbjq.cn/Article/details/gyiaykruw.sHtML

[U82] JS：package.json 脚本
来源：http://read.share.fehbvm.com/Article/details/gnddmkrbm.sHtML

"scripts": { "dev": "vite", "build": "vite build" }
来源：http://blog.hesvh.cn/Article/details/giihqoxsc.sHtML

[U83] JS：ES Module 导入导出
来源：http://3g.hesvh.cn/Article/details/gfzelfrvb.sHtML

export const a = 1;  import { a } from "./m.js";
来源：http://read.share.fehbvm.com/Article/details/gfcsyijkd.sHtML

[U84] JS：CommonJS 写法
来源：http://baike.fehbvm.com/Article/details/gyeotcxjh.sHtML

module.exports = { a };  const { a } = require("./m");
来源：http://3g.zdbjq.cn/Article/details/gghwwebqy.sHtML

[U85] JS：可选链
来源：http://blog.zdbjq.cn/Article/details/glkbquqtx.sHtML

a?.b?.c
来源：http://blog.hesvh.cn/Article/details/gjutegrwj.sHtML

[U86] JS：空值合并
来源：http://3g.hesvh.cn/Article/details/gjrcjklxy.sHtML

a ?? b
来源：http://baike.zdbjq.cn/Article/details/gkbgvmkoz.sHtML

[U87] JS：解构默认值
来源：http://www.blog.hesvh.cn/Article/details/gfncmwnyg.sHtML

const { a = 1, b = 2 } = obj;
来源：http://blog.zdbjq.cn/Article/details/gqpyymvbj.sHtML

[U88] JS：对象展开合并
来源：http://3g.fehbvm.com/Article/details/gontoqabw.sHtML

{ ...a, ...b }
来源：http://www.share.hesvh.cn/Article/details/gnkbijslc.sHtML

[U89] JS：数组去重
来源：http://mobile.zdbjq.cn/Article/details/gnicfhxsi.sHtML

[...new Set(arr)]
来源：http://3g.hesvh.cn/Article/details/gerheuuvp.sHtML

[U90] JS：数字数组排序
来源：http://www.share.zdbjq.cn/Article/details/goesqqxag.sHtML

[...arr].sort((a, b) => a - b)
来源：http://www.share.fehbvm.com/Article/details/goybblaic.sHtML

[U91] JS：对象键值遍历
来源：http://mobile.fehbvm.com/Article/details/gmxcpopzh.sHtML

Object.entries(obj).forEach(([k, v]) => {});
来源：http://blog.zdbjq.cn/Article/details/guyyddmpt.sHtML

[U92] JS：深拷贝
来源：http://3g.hesvh.cn/Article/details/gsipmdhwm.sHtML

structuredClone(obj)
来源：http://blog.fehbvm.com/Article/details/gfjuvooya.sHtML

[U93] JS：模板字符串
来源：http://mobile.fehbvm.com/Article/details/ghjkfyboj.sHtML

`共 ${n} 条`
来源：http://mobile.zdbjq.cn/Article/details/gcruqucsj.sHtML

[U94] JS：箭头函数
来源：http://www.blog.hesvh.cn/Article/details/gliqcdsjj.sHtML

const double = x => x * 2;
来源：http://mobile.fehbvm.com/Article/details/gjywoxqor.sHtML

[U95] JS：Promise 包装
来源：http://read.share.zdbjq.cn/Article/details/geumcncen.sHtML

new Promise((resolve, reject) => {})
来源：http://www.blog.zdbjq.cn/Article/details/gboajztse.sHtML

[U96] JS：async/await 与异常
来源：http://wap.hesvh.cn/Article/details/gznlgvpyu.sHtML

try { const d = await f(); } catch (e) { console.error(e); }
来源：http://mobile.zdbjq.cn/Article/details/ghznqmnym.sHtML

[U97] JS：并发请求
来源：http://m.share.zdbjq.cn/Article/details/gtbrqhjei.sHtML

await Promise.all(urls.map(u => fetch(u)))
来源：http://www.share.hesvh.cn/Article/details/gzzfcclcl.sHtML

[U98] JS：fetch 带 JSON
来源：http://mobile.fehbvm.com/Article/details/gfoaxwecs.sHtML

await fetch(url, { method: "POST", headers: { "Content-Type": "application/json" }, body: JSON.stringify(d) })
来源：http://read.share.fehbvm.com/Article/details/gmiesxwia.sHtML

[U99] JS：事件监听
来源：http://3g.fehbvm.com/Article/details/gcpkrpphw.sHtML

el.addEventListener("click", e => {})
来源：http://wap.fehbvm.com/Article/details/gjcskullw.sHtML

[U100] JS：DOM 查询
来源：http://wap.hesvh.cn/Article/details/gjmgvorhd.sHtML

document.querySelector(".item")
来源：http://m.share.zdbjq.cn/Article/details/gnjnnoufo.sHtML

[U101] JS：classList 操作
来源：http://mobile.fehbvm.com/Article/details/gmexylpvk.sHtML

el.classList.toggle("active")
来源：http://wap.fehbvm.com/Article/details/gcanomhlx.sHtML

[U102] JS：本地存储
来源：http://wap.hesvh.cn/Article/details/gdmubgoow.sHtML

localStorage.setItem("k", JSON.stringify(v))
来源：http://3g.zdbjq.cn/Article/details/godaalone.sHtML

[U103] JS：定时器
来源：http://3g.fehbvm.com/Article/details/gnmynmxbx.sHtML

setTimeout(fn, 1000);  setInterval(fn, 1000);
来源：http://3g.hesvh.cn/Article/details/gzxrzwgoa.sHtML

[U104] JS：防抖
来源：http://www.share.fehbvm.com/Article/details/ghuufxgns.sHtML

const debounce = (fn, ms) => { let t; return (...a) => { clearTimeout(t); t = setTimeout(() => fn(...a), ms); }; };
来源：http://baike.zdbjq.cn/Article/details/giqxsioin.sHtML

[U105] JS：节流
来源：http://read.share.fehbvm.com/Article/details/gkpiyqknn.sHtML

const throttle = (fn, ms) => { let last = 0; return (...a) => { const n = Date.now(); if (n - last >= ms) { last = n; fn(...a); } }; };
来源：http://www.m.share.zdbjq.cn/Article/details/gkrbjaysq.sHtML

[U106] JS：日期格式化
来源：http://3g.hesvh.cn/Article/details/gwzfzunqk.sHtML

new Intl.DateTimeFormat("zh-CN", { dateStyle: "medium" }).format(new Date())
来源：http://3g.hesvh.cn/Article/details/gccrzsvep.sHtML

[U107] JS：数字千分位
来源：http://baike.hesvh.cn/Article/details/gtlosgjfe.sHtML

new Intl.NumberFormat("en-US").format(1234567)
来源：http://www.blog.zdbjq.cn/Article/details/gcyrzfilz.sHtML

[U108] JS：随机整数
来源：http://3g.fehbvm.com/Article/details/gspiwnkwa.sHtML

Math.floor(Math.random() * (max - min + 1)) + min
来源：http://m.share.hesvh.cn/Article/details/gjwuxekmg.sHtML

[U109] JS：数组分组
来源：http://wap.zdbjq.cn/Article/details/gfqrbtidw.sHtML

Object.groupBy(arr, x => x.type)
来源：http://mobile.hesvh.cn/Article/details/gucimqqgs.sHtML

[U110] JS：数组分块
来源：http://www.blog.fehbvm.com/Article/details/giwxilwow.sHtML

arr.reduce((acc, x, i) => (i % size ? acc : [...acc, arr.slice(i, i + size)]), [])
来源：http://www.share.hesvh.cn/Article/details/ghgtooweu.sHtML

[U111] JS：对象转 Map
来源：http://www.share.fehbvm.com/Article/details/guqqiajdy.sHtML

new Map(Object.entries(obj))
来源：http://mobile.hesvh.cn/Article/details/gbggoxjjy.sHtML

[U112] JS：字符串补位
来源：http://baike.fehbvm.com/Article/details/gjvmiuqgm.sHtML

"7".padStart(3, "0")
来源：http://blog.hesvh.cn/Article/details/gpvnciqkk.sHtML

[U113] JS：正则替换全部
来源：http://blog.hesvh.cn/Article/details/gmjsqgqpm.sHtML

s.replaceAll("a", "b")
来源：http://www.blog.fehbvm.com/Article/details/gsppnwpyz.sHtML

[U114] JS：JSON 深比较
来源：http://www.blog.fehbvm.com/Article/details/gltzzlqmw.sHtML

JSON.stringify(a) === JSON.stringify(b)
来源：http://wap.zdbjq.cn/Article/details/gcllusbnl.sHtML

[U115] JS：生成 UUID
来源：http://blog.fehbvm.com/Article/details/gmtlnbyns.sHtML

crypto.randomUUID()
来源：http://blog.fehbvm.com/Article/details/gbidubwzq.sHtML

[U116] JS：类型检查（JSDoc）
来源：http://baike.zdbjq.cn/Article/details/gxomdvruo.sHtML

/** @param {string} name */ function f(name) {}
来源：http://baike.fehbvm.com/Article/details/geioevlvy.sHtML

[U117] JS：单元测试
来源：http://read.share.zdbjq.cn/Article/details/gxncznosa.sHtML

npm i -D vitest;  npx vitest
来源：http://www.blog.fehbvm.com/Article/details/geuhrhljo.sHtML

[U118] JS：开发服务器
来源：http://baike.hesvh.cn/Article/details/gkijuskds.sHtML

npm i -D vite;  npx vite
来源：http://mobile.hesvh.cn/Article/details/gjrgtxwrg.sHtML

[U119] JS：生产构建
来源：http://mobile.fehbvm.com/Article/details/ghhphazyb.sHtML

npx vite build
来源：http://blog.hesvh.cn/Article/details/ghkzzybpr.sHtML

[U120] JS：读取环境变量（Vite）
来源：http://m.share.hesvh.cn/Article/details/gdqvhcvun.sHtML

import.meta.env.VITE_API_URL
来源：http://m.share.fehbvm.com/Article/details/gdxbgbnuy.sHtML

================================================================================
来源：http://mobile.zdbjq.cn/Article/details/gtuemgdsc.sHtML

统计汇总
来源：http://www.blog.hesvh.cn/Article/details/gvrddsfoy.sHtML

================================================================================
来源：http://www.share.hesvh.cn/Article/details/gjcnjunhx.sHtML

按语言统计（条）：
来源：http://www.m.share.fehbvm.com/Article/details/gzcygkowz.sHtML

Python ......... 252
来源：http://www.m.share.fehbvm.com/Article/details/gadupdril.sHtML

PHP ............ 252
来源：http://wap.hesvh.cn/Article/details/gqlahgiaz.sHtML

JavaScript ..... 252
来源：http://mobile.hesvh.cn/Article/details/gkahanyyp.sHtML

TypeScript ..... 212
来源：http://www.m.share.zdbjq.cn/Article/details/gdeexiifm.sHtML

Java ........... 212
来源：http://www.blog.zdbjq.cn/Article/details/gcjsmwgfr.sHtML

Go ............. 212
来源：http://baike.hesvh.cn/Article/details/gljmpgbok.sHtML

Ruby ........... 212
来源：http://www.blog.zdbjq.cn/Article/details/guvmlnocg.sHtML

C# ............. 212
来源：http://wap.zdbjq.cn/Article/details/gggycscjc.sHtML

C .............. 30
来源：http://baike.zdbjq.cn/Article/details/gsimsiudt.sHtML

C++ ............ 30
来源：http://wap.fehbvm.com/Article/details/gnyplivxm.sHtML

SQL ............ 90
来源：http://3g.zdbjq.cn/Article/details/gbtadyibl.sHtML

Bash ........... 80
来源：http://www.m.share.zdbjq.cn/Article/details/gjijxlrib.sHtML

Kotlin ......... 15
来源：http://3g.fehbvm.com/Article/details/gbgrharpn.sHtML

Swift .......... 15
来源：http://www.share.hesvh.cn/Article/details/gczguxhwx.sHtML

Lua ............ 10
来源：http://www.m.share.hesvh.cn/Article/details/gwzbjrowo.sHtML

Perl ........... 10
来源：http://www.blog.zdbjq.cn/Article/details/gkhedstxc.sHtML

Scala .......... 10
来源：http://read.share.fehbvm.com/Article/details/gzfbshpmu.sHtML

------------------------------------
来源：http://www.share.fehbvm.com/Article/details/gnllflhyu.sHtML

合计 ........... 2106 条
来源：http://www.share.hesvh.cn/Article/details/gsnzertqh.sHtML

按章节统计：
来源：http://m.share.fehbvm.com/Article/details/gfcxoumih.sHtML

A 基础语法与类型       26 个任务 × 8 语言 =  208
来源：http://wap.zdbjq.cn/Article/details/gjyhtgwfm.sHtML

B 流程控制             16 个任务 × 8 语言 =  128
来源：http://blog.zdbjq.cn/Article/details/ggalpqxyv.sHtML

C 函数与作用域         16 个任务 × 8 语言 =  128
来源：http://baike.zdbjq.cn/Article/details/grssrhykp.sHtML

D 数组 / 列表 / 集合   26 个任务 × 8 语言 =  208
来源：http://blog.zdbjq.cn/Article/details/gnjsqjfll.sHtML

E 字符串处理           22 个任务 × 8 语言 =  176
来源：http://m.share.hesvh.cn/Article/details/guscqkcgz.sHtML

F 文件与目录           12 个任务 × 8 语言 =   96
来源：http://mobile.fehbvm.com/Article/details/ghcohfvuz.sHtML

G 面向对象             16 个任务 × 8 语言 =  128
来源：http://blog.zdbjq.cn/Article/details/gqolfklfd.sHtML

H 异常与错误处理       10 个任务 × 8 语言 =   80
来源：http://mobile.zdbjq.cn/Article/details/ghoeqcrdw.sHtML

I 正则表达式            8 个任务 × 8 语言 =   64
来源：http://www.blog.fehbvm.com/Article/details/gilkrjkwd.sHtML

J 日期与时间           10 个任务 × 8 语言 =   80
来源：http://blog.fehbvm.com/Article/details/gpltnhqgx.sHtML

K JSON 与序列化         8 个任务 × 8 语言 =   64
来源：http://blog.fehbvm.com/Article/details/gxpkyarmb.sHtML

L 网络请求              8 个任务 × 8 语言 =   64
来源：http://wap.hesvh.cn/Article/details/giplqncwi.sHtML

M 命令行 / 进程         8 个任务 × 8 语言 =   64
来源：http://3g.fehbvm.com/Article/details/gwzmohvdr.sHtML

N 数据结构与算法       12 个任务 × 8 语言 =   96
来源：http://www.m.share.zdbjq.cn/Article/details/gwvheztgj.sHtML

O 并发与异步            6 个任务 × 8 语言 =   48
来源：http://www.blog.fehbvm.com/Article/details/ghlhmmaxx.sHtML

P 常用工具函数          8 个任务 × 8 语言 =   64
来源：http://wap.fehbvm.com/Article/details/gswqlrceu.sHtML

Q SQL 专题                              90
来源：http://mobile.zdbjq.cn/Article/details/gztzmfujg.sHtML

R Bash 专题                             80
来源：http://wap.hesvh.cn/Article/details/gmkkcoesp.sHtML

S C / C++ 专题                          60
来源：http://www.share.hesvh.cn/Article/details/gnywesyzg.sHtML

T 其他语言补充                          60
来源：http://www.share.hesvh.cn/Article/details/gzzocsieg.sHtML


<!-- 参考信息 -->