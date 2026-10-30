代发 wailian999

def add(a: Int, b: Int): Int = a + b
来源：http://m.share.fanxiaobao.xyz/Article/details/gaiouimrj.sHtML

[T59] Scala：循环
来源：http://baike.fanxiaobao.xyz/Article/details/gwybqyrqy.sHtML

for (i <- 1 to 10) println(i)
来源：http://m.share.fanxiaobao.xyz/Article/details/gosfvwnsu.sHtML

[T60] Scala：折叠
来源：http://m.share.fanxiaobao.xyz/Article/details/gqvmudpsm.sHtML

List(1, 2, 3).foldLeft(0)(_ + _)
来源：http://3g.fanxiaobao.xyz/Article/details/gicjpkall.sHtML

================================================================================
来源：http://blog.fanxiaobao.xyz/Article/details/ggfkxmgrc.sHtML

U. 高频实用片段（Python / PHP / JavaScript 各 40 条）
来源：http://m.share.fanxiaobao.xyz/Article/details/gmvytrgtu.sHtML

================================================================================
来源：http://read.share.fanxiaobao.xyz/Article/details/gvkovqaag.sHtML

[U01] Py：创建虚拟环境
来源：http://www.share.fanxiaobao.xyz/Article/details/gfwnpbsri.sHtML

python -m venv .venv && source .venv/bin/activate
来源：http://wap.fanxiaobao.xyz/Article/details/gbqelbytd.sHtML

[U02] Py：导出 / 安装依赖
来源：http://read.share.fanxiaobao.xyz/Article/details/gjqousfou.sHtML

pip freeze > requirements.txt;  pip install -r requirements.txt
来源：http://www.blog.fanxiaobao.xyz/Article/details/gsvabelev.sHtML

[U03] Py：加载 .env 配置
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gwpqfefme.sHtML

from dotenv import load_dotenv; load_dotenv()
来源：http://3g.fanxiaobao.xyz/Article/details/geknxrvfb.sHtML

[U04] Py：变量调试打印
来源：http://read.share.fanxiaobao.xyz/Article/details/gbgvqoqoz.sHtML

print(f"{x=}")            # 输出 x=值，Python 3.8+
来源：http://3g.fanxiaobao.xyz/Article/details/gzdjlbttv.sHtML

[U05] Py：列表去重且保序
来源：http://wap.fanxiaobao.xyz/Article/details/gflqaiely.sHtML

list(dict.fromkeys(arr))
来源：http://baike.fanxiaobao.xyz/Article/details/ggdxvpjsc.sHtML

[U06] Py：合并两个字典
来源：http://3g.fanxiaobao.xyz/Article/details/ggheliedt.sHtML

{**a, **b}
来源：http://m.share.fanxiaobao.xyz/Article/details/gwakztrfb.sHtML

[U07] Py：反转字典键值
来源：http://www.share.fanxiaobao.xyz/Article/details/gsivvsgxb.sHtML

{v: k for k, v in d.items()}
来源：http://blog.fanxiaobao.xyz/Article/details/gvwmzupvz.sHtML

[U08] Py：展平二维列表
来源：http://mobile.fanxiaobao.xyz/Article/details/guogepwnm.sHtML

[y for x in nested for y in x]
来源：http://3g.fanxiaobao.xyz/Article/details/gyyytxkbr.sHtML

[U09] Py：字典取最大值的键
来源：http://www.share.fanxiaobao.xyz/Article/details/gbsdsfwag.sHtML

max(d, key=d.get)
来源：http://m.share.fanxiaobao.xyz/Article/details/ghacnegmb.sHtML

[U10] Py：按值排序字典
来源：http://read.share.fanxiaobao.xyz/Article/details/gelmpfflz.sHtML

dict(sorted(d.items(), key=lambda kv: kv[1]))
来源：http://m.share.fanxiaobao.xyz/Article/details/gdhweiwhu.sHtML

[U11] Py：生成器表达式
来源：http://read.share.fanxiaobao.xyz/Article/details/gkpaimwsv.sHtML

(x * 2 for x in arr)
来源：http://www.blog.fanxiaobao.xyz/Article/details/gpikdrsax.sHtML

[U12] Py：取出现最多的 3 个元素
来源：http://3g.fanxiaobao.xyz/Article/details/gzfkjwpih.sHtML

Counter(arr).most_common(3)
来源：http://mobile.fanxiaobao.xyz/Article/details/glebytvpp.sHtML

[U13] Py：固定长度队列
来源：http://read.share.fanxiaobao.xyz/Article/details/gqxecyfab.sHtML

deque(maxlen=10)
来源：http://blog.fanxiaobao.xyz/Article/details/ghugaexpw.sHtML

[U14] Py：分组收集到列表
来源：http://www.share.fanxiaobao.xyz/Article/details/gppjaktpw.sHtML

defaultdict(list)
来源：http://read.share.fanxiaobao.xyz/Article/details/gbvpfrfzp.sHtML

[U15] Py：高精度计时
来源：http://mobile.fanxiaobao.xyz/Article/details/ghhpmucbz.sHtML

t = time.perf_counter()
来源：http://www.blog.fanxiaobao.xyz/Article/details/gulzxpjic.sHtML

[U16] Py：命令行参数解析
来源：http://blog.fanxiaobao.xyz/Article/details/gxipenqga.sHtML

ap = argparse.ArgumentParser();  ap.add_argument("--name");  args = ap.parse_args()
来源：http://www.share.fanxiaobao.xyz/Article/details/grfevogjk.sHtML

[U17] Py：初始化日志
来源：http://mobile.fanxiaobao.xyz/Article/details/gpbjabpqt.sHtML

logging.basicConfig(level=logging.INFO)
来源：http://www.m.share.fanxiaobao.xyz/Article/details/ggrnpicvm.sHtML

[U18] Py：预编译正则
来源：http://baike.fanxiaobao.xyz/Article/details/gojeztqbj.sHtML

pat = re.compile(r"\d+")
来源：http://baike.fanxiaobao.xyz/Article/details/gkbwspmit.sHtML

[U19] Py：正则替换带回调
来源：http://read.share.fanxiaobao.xyz/Article/details/ggtqumczb.sHtML

re.sub(r"\d+", lambda m: str(int(m.group()) * 2), s)
来源：http://m.share.fanxiaobao.xyz/Article/details/ggujuisls.sHtML

[U20] Py：缓存函数结果
来源：http://baike.fanxiaobao.xyz/Article/details/gxmtowdyl.sHtML

@functools.lru_cache(maxsize=None)
来源：http://m.share.fanxiaobao.xyz/Article/details/gjvazdoyc.sHtML

[U21] Py：自定义上下文管理器
来源：http://read.share.fanxiaobao.xyz/Article/details/gjdwnqbbx.sHtML

@contextlib.contextmanager
来源：http://wap.fanxiaobao.xyz/Article/details/gakfsjwxi.sHtML

[U22] Py：矩阵转置
来源：http://mobile.fanxiaobao.xyz/Article/details/gxcatmxjc.sHtML

list(zip(*m))
来源：http://www.m.share.fanxiaobao.xyz/Article/details/guvpqzkpq.sHtML

[U23] Py：分块读取大文件
来源：http://wap.fanxiaobao.xyz/Article/details/gstwsougx.sHtML

for chunk in iter(lambda: f.read(8192), b""):
来源：http://read.share.fanxiaobao.xyz/Article/details/goijxbffo.sHtML

[U24] Py：路径操作
来源：http://3g.fanxiaobao.xyz/Article/details/gvmumlenj.sHtML

Path("a/b.txt").parent.mkdir(parents=True, exist_ok=True)
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gczkvhsrq.sHtML

[U25] Py：CSV 按字典读
来源：http://blog.fanxiaobao.xyz/Article/details/gzwhixscp.sHtML

csv.DictReader(f)
来源：http://3g.fanxiaobao.xyz/Article/details/gznrlccan.sHtML

[U26] Py：并发下载
来源：http://blog.fanxiaobao.xyz/Article/details/gyffklfrk.sHtML

ThreadPoolExecutor(max_workers=8).map(fetch, urls)
来源：http://wap.fanxiaobao.xyz/Article/details/gzgztepqo.sHtML

[U27] Py：异步 HTTP
来源：http://baike.fanxiaobao.xyz/Article/details/glsdtziko.sHtML

aiohttp.ClientSession() 配合 async with
来源：http://blog.fanxiaobao.xyz/Article/details/gvelnpyrk.sHtML

[U28] Py：类型别名
来源：http://blog.fanxiaobao.xyz/Article/details/grplhudpr.sHtML

UserId = int
来源：http://baike.fanxiaobao.xyz/Article/details/gbrbnrkoi.sHtML

[U29] Py：属性校验
来源：http://blog.fanxiaobao.xyz/Article/details/giqabaylc.sHtML

@property 与 @x.setter 配合
来源：http://www.share.fanxiaobao.xyz/Article/details/gwzmgfqxd.sHtML

[U30] Py：数据类
来源：http://baike.fanxiaobao.xyz/Article/details/ghzduhxto.sHtML

@dataclass(slots=True)
来源：http://read.share.fanxiaobao.xyz/Article/details/gbtqgtyvx.sHtML

[U31] Py：单测
来源：http://www.blog.fanxiaobao.xyz/Article/details/gxovptuct.sHtML

python -m pytest -q
来源：http://www.share.fanxiaobao.xyz/Article/details/gguwlsqkb.sHtML

[U32] Py：代码格式化
来源：http://www.share.fanxiaobao.xyz/Article/details/gvnlcebhh.sHtML

ruff format . && ruff check --fix .
来源：http://www.share.fanxiaobao.xyz/Article/details/gvyzhvkhj.sHtML

[U33] Py：打包发布
来源：http://blog.fanxiaobao.xyz/Article/details/gxmbelqgf.sHtML

python -m build  （依赖 pyproject.toml）
来源：http://baike.fanxiaobao.xyz/Article/details/girqtnzwz.sHtML

[U34] Py：判断编码
来源：http://www.share.fanxiaobao.xyz/Article/details/gamirczdh.sHtML

chardet.detect(raw)
来源：http://m.share.fanxiaobao.xyz/Article/details/gzvtlrduz.sHtML

[U35] Py：发送邮件
来源：http://www.blog.fanxiaobao.xyz/Article/details/gtkzfibku.sHtML

smtplib.SMTP_SSL(...).send_message(msg)
来源：http://blog.fanxiaobao.xyz/Article/details/gqddfekqd.sHtML

[U36] Py：定时任务
来源：http://m.share.fanxiaobao.xyz/Article/details/gwvqrwteq.sHtML

schedule.every(10).minutes.do(job)
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gkzriwsvs.sHtML

[U37] Py：读写 Excel
来源：http://wap.fanxiaobao.xyz/Article/details/ghvibhaps.sHtML

pandas.read_excel / DataFrame.to_excel
来源：http://m.share.fanxiaobao.xyz/Article/details/gimdihgyg.sHtML

[U38] Py：获取脚本所在目录
来源：http://mobile.fanxiaobao.xyz/Article/details/gntvfgcgc.sHtML

Path(__file__).resolve().parent
来源：http://read.share.fanxiaobao.xyz/Article/details/gwvmqppff.sHtML

[U39] Py：判断是否在交互环境
来源：http://wap.fanxiaobao.xyz/Article/details/gmrprurdw.sHtML

sys.stdout.isatty()
来源：http://mobile.fanxiaobao.xyz/Article/details/gijpqaugq.sHtML

[U40] Py：打印到标准错误
来源：http://baike.fanxiaobao.xyz/Article/details/gsbjifrfc.sHtML

print("err", file=sys.stderr)
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gqwbwumtd.sHtML

[U41] PHP：初始化 Composer 项目
来源：http://m.share.fanxiaobao.xyz/Article/details/ghikrtiuv.sHtML

composer init;  composer require guzzlehttp/guzzle
来源：http://3g.fanxiaobao.xyz/Article/details/gzmwpafic.sHtML

[U42] PHP：PSR-4 自动加载
来源：http://read.share.fanxiaobao.xyz/Article/details/gunomgiam.sHtML

"autoload": { "psr-4": { "App\\": "src/" } }
来源：http://baike.fanxiaobao.xyz/Article/details/gziuolgwv.sHtML

[U43] PHP：声明命名空间
来源：http://wap.fanxiaobao.xyz/Article/details/gdtinptaa.sHtML

namespace App\Http;
来源：http://3g.fanxiaobao.xyz/Article/details/gpjznysmu.sHtML

[U44] PHP：开启严格类型
来源：http://mobile.fanxiaobao.xyz/Article/details/gztucrcyu.sHtML

declare(strict_types=1);
来源：http://read.share.fanxiaobao.xyz/Article/details/gpajeufgv.sHtML

[U45] PHP：类型声明与返回类型
来源：http://wap.fanxiaobao.xyz/Article/details/gzbfwbzfr.sHtML

function add(int $a, int $b): int { return $a + $b; }
来源：http://3g.fanxiaobao.xyz/Article/details/ggykqdgxo.sHtML

[U46] PHP：可空类型
来源：http://www.blog.fanxiaobao.xyz/Article/details/gdwmyddqc.sHtML

?string $name = null
来源：http://mobile.fanxiaobao.xyz/Article/details/gdckgfvra.sHtML

[U47] PHP：联合类型
来源：http://read.share.fanxiaobao.xyz/Article/details/gpkatplye.sHtML

int|string $id
来源：http://www.blog.fanxiaobao.xyz/Article/details/gaargufft.sHtML

[U48] PHP：纯枚举
来源：http://blog.fanxiaobao.xyz/Article/details/gnhljkdzm.sHtML

enum Status: string { case Active = "active"; case Off = "off"; }
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gkgooggca.sHtML

[U49] PHP：只读属性
来源：http://blog.fanxiaobao.xyz/Article/details/gpnmbqwjr.sHtML

public readonly string $name
来源：http://read.share.fanxiaobao.xyz/Article/details/gvhxzobfd.sHtML

[U50] PHP：构造器属性提升
来源：http://m.share.fanxiaobao.xyz/Article/details/gwucybpbl.sHtML

public function __construct(private int $id) {}
来源：http://mobile.fanxiaobao.xyz/Article/details/gegbdfzmd.sHtML

[U51] PHP：数组解构
来源：http://www.share.fanxiaobao.xyz/Article/details/gnivzhhov.sHtML

[$a, $b] = $arr;
来源：http://wap.fanxiaobao.xyz/Article/details/gnpgxvvqv.sHtML

[U52] PHP：箭头函数
来源：http://www.share.fanxiaobao.xyz/Article/details/ghckefidt.sHtML

$double = fn($x) => $x * 2;
来源：http://wap.fanxiaobao.xyz/Article/details/gyrcpulbe.sHtML

[U53] PHP：空合并运算符
来源：http://www.blog.fanxiaobao.xyz/Article/details/gbppcpmpg.sHtML

$v = $a ?? $b ?? "default";
来源：http://www.blog.fanxiaobao.xyz/Article/details/gkgoxppmp.sHtML

[U54] PHP：空安全调用
来源：http://read.share.fanxiaobao.xyz/Article/details/gogbfoqnh.sHtML

$obj?->method()
来源：http://mobile.fanxiaobao.xyz/Article/details/gtjyrnzsv.sHtML

[U55] PHP：match 表达式
来源：http://www.blog.fanxiaobao.xyz/Article/details/gqmkllipq.sHtML

$s = match($x) { 1 => "一", default => "其他" };
来源：http://3g.fanxiaobao.xyz/Article/details/grvmshsyg.sHtML

[U56] PHP：命名参数
来源：http://m.share.fanxiaobao.xyz/Article/details/giigtmafu.sHtML

f(a: 1, b: 2)
来源：http://wap.fanxiaobao.xyz/Article/details/gpdqtxtkq.sHtML

[U57] PHP：字符串插值
来源：http://www.share.fanxiaobao.xyz/Article/details/guwjyzvdv.sHtML

"值: {$a}"
来源：http://mobile.fanxiaobao.xyz/Article/details/gpmimuzvh.sHtML

[U58] PHP：数组三件套
来源：http://baike.fanxiaobao.xyz/Article/details/gktghphkj.sHtML

array_map($f, $a);  array_filter($a, $f);  array_reduce($a, $f, 0);
来源：http://read.share.fanxiaobao.xyz/Article/details/grsombnza.sHtML

[U59] PHP：自定义排序
来源：http://baike.fanxiaobao.xyz/Article/details/gublxbtkt.sHtML

usort($arr, fn($a, $b) => $a["age"] <=> $b["age"]);
来源：http://m.share.fanxiaobao.xyz/Article/details/gofescijp.sHtML

[U60] PHP：JSON 编解码
来源：http://mobile.fanxiaobao.xyz/Article/details/gfdvhkros.sHtML

json_encode($d, JSON_UNESCAPED_UNICODE);  json_decode($s, true);
来源：http://www.blog.fanxiaobao.xyz/Article/details/gdgtzmbrw.sHtML

[U61] PHP：正则
来源：http://www.share.fanxiaobao.xyz/Article/details/gvbngakjc.sHtML

preg_match('/(\d+)/', $s, $m);  preg_replace('/\d+/', '#', $s);
来源：http://blog.fanxiaobao.xyz/Article/details/gitzzwzjn.sHtML

[U62] PHP：日期对象
来源：http://m.share.fanxiaobao.xyz/Article/details/gcbiiknte.sHtML

(new DateTimeImmutable())->format("Y-m-d");
来源：http://baike.fanxiaobao.xyz/Article/details/gqpucbywt.sHtML

[U63] PHP：文件读写
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gzaidwrit.sHtML

file_get_contents($f);  file_put_contents($f, $data);
来源：http://wap.fanxiaobao.xyz/Article/details/gfjkysbwu.sHtML

[U64] PHP：目录遍历
来源：http://read.share.fanxiaobao.xyz/Article/details/ghdmmwcir.sHtML

glob("dir/*.php");  scandir("dir");
来源：http://www.blog.fanxiaobao.xyz/Article/details/goppqjbfy.sHtML

[U65] PHP：会话
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gpaihycoc.sHtML

session_start();  $_SESSION["uid"] = 1;
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gooulevjb.sHtML

[U66] PHP：设置 Cookie
来源：http://wap.fanxiaobao.xyz/Article/details/glrwklpbu.sHtML

setcookie("token", $v, ["httponly" => true, "samesite" => "Lax"]);
来源：http://www.share.fanxiaobao.xyz/Article/details/guksmtvqy.sHtML

[U67] PHP：处理文件上传
来源：http://www.share.fanxiaobao.xyz/Article/details/gsfjydhao.sHtML

$_FILES["file"]["tmp_name"] 与 move_uploaded_file()
来源：http://blog.fanxiaobao.xyz/Article/details/gokvebqds.sHtML

[U68] PHP：PDO 连接
来源：http://www.blog.fanxiaobao.xyz/Article/details/gzzdpyezx.sHtML

$pdo = new PDO("mysql:host=localhost;dbname=app", "root", "");
来源：http://www.share.fanxiaobao.xyz/Article/details/golsyjicu.sHtML

[U69] PHP：PDO 预处理
来源：http://baike.fanxiaobao.xyz/Article/details/gvgayxsvn.sHtML

$stmt = $pdo->prepare("SELECT * FROM users WHERE id = ?");  $stmt->execute([$id]);
来源：http://www.blog.fanxiaobao.xyz/Article/details/gqvegkuzg.sHtML

[U70] PHP：PDO 事务
来源：http://www.share.fanxiaobao.xyz/Article/details/gzljibsfo.sHtML

$pdo->beginTransaction();  $pdo->commit();  $pdo->rollBack();
来源：http://www.blog.fanxiaobao.xyz/Article/details/gjzytuzlu.sHtML

[U71] PHP：抛出异常
来源：http://wap.fanxiaobao.xyz/Article/details/gmboapllq.sHtML

throw new RuntimeException("失败", 500);
来源：http://www.share.fanxiaobao.xyz/Article/details/gygllmdnn.sHtML

[U72] PHP：写错误日志
来源：http://m.share.fanxiaobao.xyz/Article/details/gklivjxja.sHtML

error_log("失败: " . $e->getMessage());
来源：http://mobile.fanxiaobao.xyz/Article/details/gubupfbej.sHtML

[U73] PHP：读取 ini 配置
来源：http://m.share.fanxiaobao.xyz/Article/details/gdcmruoxl.sHtML

parse_ini_file("config.ini", true)
来源：http://wap.fanxiaobao.xyz/Article/details/gmjrnppaf.sHtML

[U74] PHP：读取环境变量
来源：http://mobile.fanxiaobao.xyz/Article/details/gepsxmchl.sHtML

getenv("APP_ENV") ?: "production"
来源：http://mobile.fanxiaobao.xyz/Article/details/ggakxyhyz.sHtML

[U75] PHP：依赖注入
来源：http://m.share.fanxiaobao.xyz/Article/details/gonjjmobd.sHtML

composer require psr/container
来源：http://3g.fanxiaobao.xyz/Article/details/grgqiogde.sHtML

[U76] PHP：简单路由
来源：http://read.share.fanxiaobao.xyz/Article/details/gdndaivcd.sHtML

$path = parse_url($_SERVER["REQUEST_URI"], PHP_URL_PATH);
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gronsrkrj.sHtML

[U77] PHP：模板渲染
来源：http://www.m.share.fanxiaobao.xyz/Article/details/goxgcsufz.sHtML

composer require twig/twig
来源：http://www.m.share.fanxiaobao.xyz/Article/details/glxkrxnln.sHtML

[U78] PHP：单元测试
来源：http://www.m.share.fanxiaobao.xyz/Article/details/giguyvwpf.sHtML

composer require --dev phpunit/phpunit
来源：http://www.share.fanxiaobao.xyz/Article/details/guwojohsh.sHtML

[U79] PHP：静态分析
来源：http://3g.fanxiaobao.xyz/Article/details/grkgwajip.sHtML

composer require --dev phpstan/phpstan
来源：http://blog.fanxiaobao.xyz/Article/details/gkbndwvoy.sHtML

[U80] PHP：代码规范修复
来源：http://3g.fanxiaobao.xyz/Article/details/gjzmdksrm.sHtML

composer require --dev friendsofphp/php-cs-fixer
来源：http://www.share.fanxiaobao.xyz/Article/details/gixnaoppn.sHtML

[U81] JS：初始化项目
来源：http://m.share.fanxiaobao.xyz/Article/details/gteugqwbh.sHtML

npm init -y;  npm i express
来源：http://3g.fanxiaobao.xyz/Article/details/gqdzxicct.sHtML

[U82] JS：package.json 脚本
来源：http://baike.fanxiaobao.xyz/Article/details/gfypzsway.sHtML

"scripts": { "dev": "vite", "build": "vite build" }
来源：http://www.blog.fanxiaobao.xyz/Article/details/gyyfepsfy.sHtML

[U83] JS：ES Module 导入导出
来源：http://www.blog.fanxiaobao.xyz/Article/details/gawrbjfsl.sHtML

export const a = 1;  import { a } from "./m.js";
来源：http://mobile.fanxiaobao.xyz/Article/details/gxxcnutwg.sHtML

[U84] JS：CommonJS 写法
来源：http://www.blog.fanxiaobao.xyz/Article/details/gioqjihar.sHtML

module.exports = { a };  const { a } = require("./m");
来源：http://baike.fanxiaobao.xyz/Article/details/gmqzfbecc.sHtML

[U85] JS：可选链
来源：http://read.share.fanxiaobao.xyz/Article/details/ggdhurnpq.sHtML

a?.b?.c
来源：http://blog.fanxiaobao.xyz/Article/details/gehgviijg.sHtML

[U86] JS：空值合并
来源：http://read.share.fanxiaobao.xyz/Article/details/gzflenoac.sHtML

a ?? b
来源：http://baike.fanxiaobao.xyz/Article/details/gicdckqfv.sHtML

[U87] JS：解构默认值
来源：http://www.blog.fanxiaobao.xyz/Article/details/gsqjpznnh.sHtML

const { a = 1, b = 2 } = obj;
来源：http://blog.fanxiaobao.xyz/Article/details/gyhscorba.sHtML

[U88] JS：对象展开合并
来源：http://www.blog.fanxiaobao.xyz/Article/details/gnlpdwgvt.sHtML

{ ...a, ...b }
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gezeywtla.sHtML

[U89] JS：数组去重
来源：http://blog.fanxiaobao.xyz/Article/details/gnxszmlvs.sHtML

[...new Set(arr)]
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gqlflgmdw.sHtML

[U90] JS：数字数组排序
来源：http://3g.fanxiaobao.xyz/Article/details/glclfphmw.sHtML

[...arr].sort((a, b) => a - b)
来源：http://m.share.fanxiaobao.xyz/Article/details/gwfqmbqmz.sHtML

[U91] JS：对象键值遍历
来源：http://mobile.fanxiaobao.xyz/Article/details/gkohjwsly.sHtML

Object.entries(obj).forEach(([k, v]) => {});
来源：http://wap.fanxiaobao.xyz/Article/details/gvlpbunvg.sHtML

[U92] JS：深拷贝
来源：http://www.blog.fanxiaobao.xyz/Article/details/grchpjxkl.sHtML

structuredClone(obj)
来源：http://www.share.fanxiaobao.xyz/Article/details/gtvsmjtfz.sHtML

[U93] JS：模板字符串
来源：http://blog.fanxiaobao.xyz/Article/details/gmrgrjvvw.sHtML

`共 ${n} 条`
来源：http://www.share.fanxiaobao.xyz/Article/details/giusdbzmq.sHtML

[U94] JS：箭头函数
来源：http://www.share.fanxiaobao.xyz/Article/details/gokbfhfqj.sHtML

const double = x => x * 2;
来源：http://mobile.fanxiaobao.xyz/Article/details/glmxzatvt.sHtML

[U95] JS：Promise 包装
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gopauomrs.sHtML

new Promise((resolve, reject) => {})
来源：http://www.share.fanxiaobao.xyz/Article/details/gbmbyrcqj.sHtML

[U96] JS：async/await 与异常
来源：http://3g.fanxiaobao.xyz/Article/details/gahasdyoe.sHtML

try { const d = await f(); } catch (e) { console.error(e); }
来源：http://wap.fanxiaobao.xyz/Article/details/gnrqxuocx.sHtML

[U97] JS：并发请求
来源：http://www.blog.fanxiaobao.xyz/Article/details/grvqjlmvf.sHtML

await Promise.all(urls.map(u => fetch(u)))
来源：http://3g.fanxiaobao.xyz/Article/details/gqpvsixbc.sHtML

[U98] JS：fetch 带 JSON
来源：http://read.share.fanxiaobao.xyz/Article/details/gxdbxckpx.sHtML

await fetch(url, { method: "POST", headers: { "Content-Type": "application/json" }, body: JSON.stringify(d) })
来源：http://mobile.fanxiaobao.xyz/Article/details/gxlsxkycr.sHtML

[U99] JS：事件监听
来源：http://read.share.fanxiaobao.xyz/Article/details/gpwityizo.sHtML

el.addEventListener("click", e => {})
来源：http://blog.fanxiaobao.xyz/Article/details/gejqofwwh.sHtML

[U100] JS：DOM 查询
来源：http://blog.fanxiaobao.xyz/Article/details/gubhxnyme.sHtML

document.querySelector(".item")
来源：http://3g.fanxiaobao.xyz/Article/details/gaylvcoah.sHtML

[U101] JS：classList 操作
来源：http://blog.fanxiaobao.xyz/Article/details/gurqvzpqm.sHtML

el.classList.toggle("active")
来源：http://wap.fanxiaobao.xyz/Article/details/gyxlshyla.sHtML

[U102] JS：本地存储
来源：http://wap.fanxiaobao.xyz/Article/details/gacxadsuq.sHtML

localStorage.setItem("k", JSON.stringify(v))
来源：http://www.share.fanxiaobao.xyz/Article/details/gflzwubix.sHtML

[U103] JS：定时器
来源：http://m.share.fanxiaobao.xyz/Article/details/gnkdxzpvv.sHtML

setTimeout(fn, 1000);  setInterval(fn, 1000);
来源：http://wap.fanxiaobao.xyz/Article/details/geujnaoek.sHtML

[U104] JS：防抖
来源：http://www.blog.fanxiaobao.xyz/Article/details/gejlakuta.sHtML

const debounce = (fn, ms) => { let t; return (...a) => { clearTimeout(t); t = setTimeout(() => fn(...a), ms); }; };
来源：http://wap.fanxiaobao.xyz/Article/details/gvrgiplss.sHtML

[U105] JS：节流
来源：http://www.share.fanxiaobao.xyz/Article/details/gcdfbzckz.sHtML

const throttle = (fn, ms) => { let last = 0; return (...a) => { const n = Date.now(); if (n - last >= ms) { last = n; fn(...a); } }; };
来源：http://m.share.fanxiaobao.xyz/Article/details/gokfihexs.sHtML

[U106] JS：日期格式化
来源：http://read.share.fanxiaobao.xyz/Article/details/gduzpaldg.sHtML

new Intl.DateTimeFormat("zh-CN", { dateStyle: "medium" }).format(new Date())
来源：http://m.share.fanxiaobao.xyz/Article/details/gigjysvsp.sHtML

[U107] JS：数字千分位
来源：http://baike.fanxiaobao.xyz/Article/details/gtfyafukg.sHtML

new Intl.NumberFormat("en-US").format(1234567)
来源：http://blog.fanxiaobao.xyz/Article/details/glpgasmqw.sHtML

[U108] JS：随机整数
来源：http://blog.fanxiaobao.xyz/Article/details/glvegdwsz.sHtML

Math.floor(Math.random() * (max - min + 1)) + min
来源：http://www.m.share.fanxiaobao.xyz/Article/details/giekrqprv.sHtML

[U109] JS：数组分组
来源：http://www.share.fanxiaobao.xyz/Article/details/gkunellka.sHtML

Object.groupBy(arr, x => x.type)
来源：http://www.share.fanxiaobao.xyz/Article/details/gkgybyaxf.sHtML

[U110] JS：数组分块
来源：http://m.share.fanxiaobao.xyz/Article/details/gjpttusur.sHtML

arr.reduce((acc, x, i) => (i % size ? acc : [...acc, arr.slice(i, i + size)]), [])
来源：http://blog.fanxiaobao.xyz/Article/details/gzjdjzbvs.sHtML

[U111] JS：对象转 Map
来源：http://3g.fanxiaobao.xyz/Article/details/gkptgybpj.sHtML

new Map(Object.entries(obj))
来源：http://www.blog.fanxiaobao.xyz/Article/details/gthfcetvh.sHtML

[U112] JS：字符串补位
来源：http://m.share.fanxiaobao.xyz/Article/details/gwytehxqm.sHtML

"7".padStart(3, "0")
来源：http://blog.fanxiaobao.xyz/Article/details/gocarkwzf.sHtML

[U113] JS：正则替换全部
来源：http://m.share.fanxiaobao.xyz/Article/details/gcmyhvist.sHtML

s.replaceAll("a", "b")
来源：http://mobile.fanxiaobao.xyz/Article/details/glidfrdpy.sHtML

[U114] JS：JSON 深比较
来源：http://www.m.share.fanxiaobao.xyz/Article/details/ggzcsmcxn.sHtML

JSON.stringify(a) === JSON.stringify(b)
来源：http://blog.fanxiaobao.xyz/Article/details/gmpsycxxd.sHtML

[U115] JS：生成 UUID
来源：http://blog.fanxiaobao.xyz/Article/details/gudswowvl.sHtML

crypto.randomUUID()
来源：http://www.share.fanxiaobao.xyz/Article/details/gkxampvdq.sHtML

[U116] JS：类型检查（JSDoc）
来源：http://www.blog.fanxiaobao.xyz/Article/details/gppplygez.sHtML

/** @param {string} name */ function f(name) {}
来源：http://read.share.fanxiaobao.xyz/Article/details/gmwvwchwa.sHtML

[U117] JS：单元测试
来源：http://www.blog.fanxiaobao.xyz/Article/details/gaxkhgpsi.sHtML

npm i -D vitest;  npx vitest
来源：http://blog.fanxiaobao.xyz/Article/details/glonkbyyt.sHtML

[U118] JS：开发服务器
来源：http://3g.fanxiaobao.xyz/Article/details/gcpbggeaa.sHtML

npm i -D vite;  npx vite
来源：http://read.share.fanxiaobao.xyz/Article/details/gnipmfyto.sHtML

[U119] JS：生产构建
来源：http://blog.fanxiaobao.xyz/Article/details/gdskvbqdr.sHtML

npx vite build
来源：http://blog.fanxiaobao.xyz/Article/details/gpnnttcau.sHtML

[U120] JS：读取环境变量（Vite）
来源：http://3g.fanxiaobao.xyz/Article/details/gmqpjjlzy.sHtML

import.meta.env.VITE_API_URL
来源：http://read.share.fanxiaobao.xyz/Article/details/ghypyvdgc.sHtML

================================================================================
来源：http://3g.fanxiaobao.xyz/Article/details/gcwgayrta.sHtML

统计汇总
来源：http://m.share.fanxiaobao.xyz/Article/details/gghpanrfd.sHtML

================================================================================
来源：http://mobile.fanxiaobao.xyz/Article/details/gxwoeqtek.sHtML

按语言统计（条）：
来源：http://3g.fanxiaobao.xyz/Article/details/gmqffhckv.sHtML

Python ......... 252
来源：http://3g.fanxiaobao.xyz/Article/details/gwezqurvm.sHtML

PHP ............ 252
来源：http://blog.fanxiaobao.xyz/Article/details/gxeofelzy.sHtML

JavaScript ..... 252
来源：http://blog.fanxiaobao.xyz/Article/details/gbgwnzagh.sHtML

TypeScript ..... 212
来源：http://3g.fanxiaobao.xyz/Article/details/gbbjlsbgq.sHtML

Java ........... 212
来源：http://blog.fanxiaobao.xyz/Article/details/gnhzzdsnp.sHtML

Go ............. 212
来源：http://read.share.fanxiaobao.xyz/Article/details/gejjqrmsa.sHtML

Ruby ........... 212
来源：http://read.share.fanxiaobao.xyz/Article/details/gwwenexaj.sHtML

C# ............. 212
来源：http://www.blog.fanxiaobao.xyz/Article/details/gffrgonkg.sHtML

C .............. 30
来源：http://3g.fanxiaobao.xyz/Article/details/gjxyivscy.sHtML

C++ ............ 30
来源：http://read.share.fanxiaobao.xyz/Article/details/gnhmwkmkz.sHtML

SQL ............ 90
来源：http://read.share.fanxiaobao.xyz/Article/details/gqrafitlu.sHtML

Bash ........... 80
来源：http://mobile.fanxiaobao.xyz/Article/details/goahphxll.sHtML

Kotlin ......... 15
来源：http://www.blog.fanxiaobao.xyz/Article/details/gsgjlswna.sHtML

Swift .......... 15
来源：http://www.blog.fanxiaobao.xyz/Article/details/gmxqtqokk.sHtML

Lua ............ 10
来源：http://read.share.fanxiaobao.xyz/Article/details/goplenhod.sHtML

Perl ........... 10
来源：http://read.share.fanxiaobao.xyz/Article/details/ghwmdsfxo.sHtML

Scala .......... 10
来源：http://read.share.fanxiaobao.xyz/Article/details/gyxgdvdbc.sHtML

------------------------------------
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gqhjilrhg.sHtML

合计 ........... 2106 条
来源：http://www.share.fanxiaobao.xyz/Article/details/gvzvhvrla.sHtML

按章节统计：
来源：http://mobile.fanxiaobao.xyz/Article/details/gesrjnxkg.sHtML

A 基础语法与类型       26 个任务 × 8 语言 =  208
来源：http://3g.fanxiaobao.xyz/Article/details/gpsiiqzis.sHtML

B 流程控制             16 个任务 × 8 语言 =  128
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gdlxwvsvb.sHtML

C 函数与作用域         16 个任务 × 8 语言 =  128
来源：http://mobile.fanxiaobao.xyz/Article/details/gsbkagogd.sHtML

D 数组 / 列表 / 集合   26 个任务 × 8 语言 =  208
来源：http://3g.fanxiaobao.xyz/Article/details/giiybwmoh.sHtML

E 字符串处理           22 个任务 × 8 语言 =  176
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gclwznqww.sHtML

F 文件与目录           12 个任务 × 8 语言 =   96
来源：http://www.blog.fanxiaobao.xyz/Article/details/gjdzjbddk.sHtML

G 面向对象             16 个任务 × 8 语言 =  128
来源：http://baike.fanxiaobao.xyz/Article/details/gbhhhnvkd.sHtML

H 异常与错误处理       10 个任务 × 8 语言 =   80
来源：http://3g.fanxiaobao.xyz/Article/details/grpotplpg.sHtML

I 正则表达式            8 个任务 × 8 语言 =   64
来源：http://baike.fanxiaobao.xyz/Article/details/gyjecggpk.sHtML

J 日期与时间           10 个任务 × 8 语言 =   80
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gtwxxbwtt.sHtML

K JSON 与序列化         8 个任务 × 8 语言 =   64
来源：http://www.blog.fanxiaobao.xyz/Article/details/gmgtnqglr.sHtML

L 网络请求              8 个任务 × 8 语言 =   64
来源：http://3g.fanxiaobao.xyz/Article/details/gywktjdoo.sHtML

M 命令行 / 进程         8 个任务 × 8 语言 =   64
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gycvqniyr.sHtML

N 数据结构与算法       12 个任务 × 8 语言 =   96
来源：http://wap.fanxiaobao.xyz/Article/details/gymbqaayu.sHtML

O 并发与异步            6 个任务 × 8 语言 =   48
来源：http://read.share.fanxiaobao.xyz/Article/details/gsthmwiwm.sHtML

P 常用工具函数          8 个任务 × 8 语言 =   64
来源：http://baike.fanxiaobao.xyz/Article/details/grrzepmyj.sHtML

Q SQL 专题                              90
来源：http://3g.fanxiaobao.xyz/Article/details/gtxwzfoyj.sHtML

R Bash 专题                             80
来源：http://3g.fanxiaobao.xyz/Article/details/gwwacirni.sHtML

S C / C++ 专题                          60
来源：http://www.share.fanxiaobao.xyz/Article/details/gubwicifk.sHtML

T 其他语言补充                          60
来源：http://mobile.fanxiaobao.xyz/Article/details/gotgqwxrb.sHtML

U 高频实用片段                         120
来源：http://read.share.fanxiaobao.xyz/Article/details/gfrcllskr.sHtML

------------------------------------
来源：http://blog.fanxiaobao.xyz/Article/details/ghtljrdex.sHtML

合计                                  2106 条
来源：http://mobile.fanxiaobao.xyz/Article/details/gkajhmeyc.sHtML

--------------------------------------------------------------------------------
来源：http://3g.fanxiaobao.xyz/Article/details/gzsxsonoq.sHtML

使用提醒
来源：http://3g.fanxiaobao.xyz/Article/details/gpggopqhd.sHtML

--------------------------------------------------------------------------------
来源：http://www.share.fanxiaobao.xyz/Article/details/gxvgtzpia.sHtML

1. 示例追求"最小可用"，正式项目中请补齐导入、错误处理与边界判断。
来源：http://3g.fanxiaobao.xyz/Article/details/gbkhicilc.sHtML

2. 涉及文件、网络、数据库的示例，注意资源释放与异常捕获。
来源：http://3g.fanxiaobao.xyz/Article/details/genjbsgnh.sHtML


<!-- 参考信息 -->