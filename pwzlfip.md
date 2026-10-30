代发 wailian999

def add(a: Int, b: Int): Int = a + b
来源：http://mobile.fanxiaobao.xyz/Article/details/gacjdrngq.sHtML

[T59] Scala：循环
来源：http://www.share.fanxiaobao.xyz/Article/details/gbeladqnq.sHtML

for (i <- 1 to 10) println(i)
来源：http://www.share.fanxiaobao.xyz/Article/details/gtowrvotx.sHtML

[T60] Scala：折叠
来源：http://m.share.fanxiaobao.xyz/Article/details/gjqdoqthg.sHtML

List(1, 2, 3).foldLeft(0)(_ + _)
来源：http://www.share.fanxiaobao.xyz/Article/details/gxuqrtdsm.sHtML

================================================================================
来源：http://read.share.fanxiaobao.xyz/Article/details/gqsdcesch.sHtML

U. 高频实用片段（Python / PHP / JavaScript 各 40 条）
来源：http://www.blog.fanxiaobao.xyz/Article/details/gdsyfsmwo.sHtML

================================================================================
来源：http://m.share.fanxiaobao.xyz/Article/details/glarzeioh.sHtML

[U01] Py：创建虚拟环境
来源：http://mobile.fanxiaobao.xyz/Article/details/gmjwgkqqv.sHtML

python -m venv .venv && source .venv/bin/activate
来源：http://3g.fanxiaobao.xyz/Article/details/ggxzqtmih.sHtML

[U02] Py：导出 / 安装依赖
来源：http://mobile.fanxiaobao.xyz/Article/details/gwnaxuxpq.sHtML

pip freeze > requirements.txt;  pip install -r requirements.txt
来源：http://m.share.fanxiaobao.xyz/Article/details/ggougkrbp.sHtML

[U03] Py：加载 .env 配置
来源：http://m.share.fanxiaobao.xyz/Article/details/gtdpossbz.sHtML

from dotenv import load_dotenv; load_dotenv()
来源：http://m.share.fanxiaobao.xyz/Article/details/gjptvuoey.sHtML

[U04] Py：变量调试打印
来源：http://mobile.fanxiaobao.xyz/Article/details/gokmnlywe.sHtML

print(f"{x=}")            # 输出 x=值，Python 3.8+
来源：http://3g.fanxiaobao.xyz/Article/details/gzddkietw.sHtML

[U05] Py：列表去重且保序
来源：http://blog.fanxiaobao.xyz/Article/details/gnwhdzjai.sHtML

list(dict.fromkeys(arr))
来源：http://mobile.fanxiaobao.xyz/Article/details/gghqavesl.sHtML

[U06] Py：合并两个字典
来源：http://3g.fanxiaobao.xyz/Article/details/gsgnunteq.sHtML

{**a, **b}
来源：http://m.share.fanxiaobao.xyz/Article/details/gkipourku.sHtML

[U07] Py：反转字典键值
来源：http://wap.fanxiaobao.xyz/Article/details/gptebqgdj.sHtML

{v: k for k, v in d.items()}
来源：http://blog.fanxiaobao.xyz/Article/details/gsmlwvjxi.sHtML

[U08] Py：展平二维列表
来源：http://baike.fanxiaobao.xyz/Article/details/gupsrwbow.sHtML

[y for x in nested for y in x]
来源：http://baike.fanxiaobao.xyz/Article/details/ghlxiwmsm.sHtML

[U09] Py：字典取最大值的键
来源：http://wap.fanxiaobao.xyz/Article/details/gcgtzckke.sHtML

max(d, key=d.get)
来源：http://m.share.fanxiaobao.xyz/Article/details/gytkbnjtr.sHtML

[U10] Py：按值排序字典
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gjllxjnjc.sHtML

dict(sorted(d.items(), key=lambda kv: kv[1]))
来源：http://wap.fanxiaobao.xyz/Article/details/gahuhrswu.sHtML

[U11] Py：生成器表达式
来源：http://read.share.fanxiaobao.xyz/Article/details/gwcwgvjnh.sHtML

(x * 2 for x in arr)
来源：http://3g.fanxiaobao.xyz/Article/details/giinqunrv.sHtML

[U12] Py：取出现最多的 3 个元素
来源：http://read.share.fanxiaobao.xyz/Article/details/gfriyagbl.sHtML

Counter(arr).most_common(3)
来源：http://blog.fanxiaobao.xyz/Article/details/gshhohfwu.sHtML

[U13] Py：固定长度队列
来源：http://baike.fanxiaobao.xyz/Article/details/grvmeydmb.sHtML

deque(maxlen=10)
来源：http://read.share.fanxiaobao.xyz/Article/details/gacpzbacj.sHtML

[U14] Py：分组收集到列表
来源：http://www.blog.fanxiaobao.xyz/Article/details/geivhuslo.sHtML

defaultdict(list)
来源：http://www.blog.fanxiaobao.xyz/Article/details/gtvwmuynv.sHtML

[U15] Py：高精度计时
来源：http://www.share.fanxiaobao.xyz/Article/details/guztznhgo.sHtML

t = time.perf_counter()
来源：http://www.blog.fanxiaobao.xyz/Article/details/gnwwacbmy.sHtML

[U16] Py：命令行参数解析
来源：http://mobile.fanxiaobao.xyz/Article/details/ggmmfppqn.sHtML

ap = argparse.ArgumentParser();  ap.add_argument("--name");  args = ap.parse_args()
来源：http://wap.fanxiaobao.xyz/Article/details/gqgzctgtr.sHtML

[U17] Py：初始化日志
来源：http://wap.fanxiaobao.xyz/Article/details/gmbewyaho.sHtML

logging.basicConfig(level=logging.INFO)
来源：http://baike.fanxiaobao.xyz/Article/details/gxyjjbkws.sHtML

[U18] Py：预编译正则
来源：http://baike.fanxiaobao.xyz/Article/details/giorreqvi.sHtML

pat = re.compile(r"\d+")
来源：http://m.share.fanxiaobao.xyz/Article/details/gvyzmcyyb.sHtML

[U19] Py：正则替换带回调
来源：http://m.share.fanxiaobao.xyz/Article/details/gbuvywgil.sHtML

re.sub(r"\d+", lambda m: str(int(m.group()) * 2), s)
来源：http://m.share.fanxiaobao.xyz/Article/details/glaluvyyy.sHtML

[U20] Py：缓存函数结果
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gbyudyxus.sHtML

@functools.lru_cache(maxsize=None)
来源：http://read.share.fanxiaobao.xyz/Article/details/gfewdprqy.sHtML

[U21] Py：自定义上下文管理器
来源：http://baike.fanxiaobao.xyz/Article/details/gqvlotefu.sHtML

@contextlib.contextmanager
来源：http://www.share.fanxiaobao.xyz/Article/details/gljowppke.sHtML

[U22] Py：矩阵转置
来源：http://www.blog.fanxiaobao.xyz/Article/details/ghzcitmdv.sHtML

list(zip(*m))
来源：http://www.share.fanxiaobao.xyz/Article/details/gzeicqijn.sHtML

[U23] Py：分块读取大文件
来源：http://baike.fanxiaobao.xyz/Article/details/gdpcnsout.sHtML

for chunk in iter(lambda: f.read(8192), b""):
来源：http://read.share.fanxiaobao.xyz/Article/details/gxedbumzr.sHtML

[U24] Py：路径操作
来源：http://read.share.fanxiaobao.xyz/Article/details/gixjoasgt.sHtML

Path("a/b.txt").parent.mkdir(parents=True, exist_ok=True)
来源：http://baike.fanxiaobao.xyz/Article/details/grshcnctw.sHtML

[U25] Py：CSV 按字典读
来源：http://read.share.fanxiaobao.xyz/Article/details/gptsgiodf.sHtML

csv.DictReader(f)
来源：http://m.share.fanxiaobao.xyz/Article/details/gmvsgwqrl.sHtML

[U26] Py：并发下载
来源：http://read.share.fanxiaobao.xyz/Article/details/gqlglkuvp.sHtML

ThreadPoolExecutor(max_workers=8).map(fetch, urls)
来源：http://blog.fanxiaobao.xyz/Article/details/gytmqbqjn.sHtML

[U27] Py：异步 HTTP
来源：http://baike.fanxiaobao.xyz/Article/details/gwprwmbei.sHtML

aiohttp.ClientSession() 配合 async with
来源：http://mobile.fanxiaobao.xyz/Article/details/glmsmjwch.sHtML

[U28] Py：类型别名
来源：http://baike.fanxiaobao.xyz/Article/details/gwfmyqpdp.sHtML

UserId = int
来源：http://read.share.fanxiaobao.xyz/Article/details/ggzvpkdlr.sHtML

[U29] Py：属性校验
来源：http://www.blog.fanxiaobao.xyz/Article/details/ghhtgkqwg.sHtML

@property 与 @x.setter 配合
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gjfbplkxb.sHtML

[U30] Py：数据类
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gxsielnli.sHtML

@dataclass(slots=True)
来源：http://blog.fanxiaobao.xyz/Article/details/gipgcasab.sHtML

[U31] Py：单测
来源：http://www.share.fanxiaobao.xyz/Article/details/gmkerycxw.sHtML

python -m pytest -q
来源：http://baike.fanxiaobao.xyz/Article/details/gtngxifls.sHtML

[U32] Py：代码格式化
来源：http://m.share.fanxiaobao.xyz/Article/details/gpahiicop.sHtML

ruff format . && ruff check --fix .
来源：http://mobile.fanxiaobao.xyz/Article/details/gbbppmmfn.sHtML

[U33] Py：打包发布
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gfpfzswqu.sHtML

python -m build  （依赖 pyproject.toml）
来源：http://www.blog.fanxiaobao.xyz/Article/details/gligaexaa.sHtML

[U34] Py：判断编码
来源：http://m.share.fanxiaobao.xyz/Article/details/gokdajwan.sHtML

chardet.detect(raw)
来源：http://www.share.fanxiaobao.xyz/Article/details/golluilry.sHtML

[U35] Py：发送邮件
来源：http://3g.fanxiaobao.xyz/Article/details/gmhvhmcdg.sHtML

smtplib.SMTP_SSL(...).send_message(msg)
来源：http://3g.fanxiaobao.xyz/Article/details/gjnotzikn.sHtML

[U36] Py：定时任务
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gzrtfnocm.sHtML

schedule.every(10).minutes.do(job)
来源：http://read.share.fanxiaobao.xyz/Article/details/gxfmsrcbv.sHtML

[U37] Py：读写 Excel
来源：http://3g.fanxiaobao.xyz/Article/details/gnetwkqbj.sHtML

pandas.read_excel / DataFrame.to_excel
来源：http://baike.fanxiaobao.xyz/Article/details/gfmgyskxg.sHtML

[U38] Py：获取脚本所在目录
来源：http://baike.fanxiaobao.xyz/Article/details/gwkinsdkb.sHtML

Path(__file__).resolve().parent
来源：http://blog.fanxiaobao.xyz/Article/details/gkleodzql.sHtML

[U39] Py：判断是否在交互环境
来源：http://read.share.fanxiaobao.xyz/Article/details/gundobrjc.sHtML

sys.stdout.isatty()
来源：http://mobile.fanxiaobao.xyz/Article/details/guoxltmzx.sHtML

[U40] Py：打印到标准错误
来源：http://3g.fanxiaobao.xyz/Article/details/gvbqnnykq.sHtML

print("err", file=sys.stderr)
来源：http://3g.fanxiaobao.xyz/Article/details/guodlhazl.sHtML

[U41] PHP：初始化 Composer 项目
来源：http://3g.fanxiaobao.xyz/Article/details/gdiacmuql.sHtML

composer init;  composer require guzzlehttp/guzzle
来源：http://www.blog.fanxiaobao.xyz/Article/details/gthirtdlw.sHtML

[U42] PHP：PSR-4 自动加载
来源：http://3g.fanxiaobao.xyz/Article/details/goiwptjdx.sHtML

"autoload": { "psr-4": { "App\\": "src/" } }
来源：http://baike.fanxiaobao.xyz/Article/details/ggusyfdth.sHtML

[U43] PHP：声明命名空间
来源：http://wap.fanxiaobao.xyz/Article/details/gksaloglj.sHtML

namespace App\Http;
来源：http://wap.fanxiaobao.xyz/Article/details/gdbgcujyt.sHtML

[U44] PHP：开启严格类型
来源：http://baike.fanxiaobao.xyz/Article/details/grxpoanuv.sHtML

declare(strict_types=1);
来源：http://www.share.fanxiaobao.xyz/Article/details/glcwthedp.sHtML

[U45] PHP：类型声明与返回类型
来源：http://www.blog.fanxiaobao.xyz/Article/details/gpoktdzou.sHtML

function add(int $a, int $b): int { return $a + $b; }
来源：http://read.share.fanxiaobao.xyz/Article/details/gbmxbrkuj.sHtML

[U46] PHP：可空类型
来源：http://baike.fanxiaobao.xyz/Article/details/gnwbfjjjd.sHtML

?string $name = null
来源：http://www.share.fanxiaobao.xyz/Article/details/gqtppofnr.sHtML

[U47] PHP：联合类型
来源：http://blog.fanxiaobao.xyz/Article/details/gtilxbiuy.sHtML

int|string $id
来源：http://3g.fanxiaobao.xyz/Article/details/gzgoelugy.sHtML

[U48] PHP：纯枚举
来源：http://blog.fanxiaobao.xyz/Article/details/gjhmxejao.sHtML

enum Status: string { case Active = "active"; case Off = "off"; }
来源：http://www.blog.fanxiaobao.xyz/Article/details/gegdbzjti.sHtML

[U49] PHP：只读属性
来源：http://read.share.fanxiaobao.xyz/Article/details/gsbgozudw.sHtML

public readonly string $name
来源：http://3g.fanxiaobao.xyz/Article/details/gmuasuihu.sHtML

[U50] PHP：构造器属性提升
来源：http://m.share.fanxiaobao.xyz/Article/details/ggrqmulrv.sHtML

public function __construct(private int $id) {}
来源：http://m.share.fanxiaobao.xyz/Article/details/gldrkddog.sHtML

[U51] PHP：数组解构
来源：http://m.share.fanxiaobao.xyz/Article/details/grqnxpgaa.sHtML

[$a, $b] = $arr;
来源：http://baike.fanxiaobao.xyz/Article/details/ginddodjc.sHtML

[U52] PHP：箭头函数
来源：http://www.blog.fanxiaobao.xyz/Article/details/gpslyxcrb.sHtML

$double = fn($x) => $x * 2;
来源：http://mobile.fanxiaobao.xyz/Article/details/gouvmnpti.sHtML

[U53] PHP：空合并运算符
来源：http://3g.fanxiaobao.xyz/Article/details/ggptpgwby.sHtML

$v = $a ?? $b ?? "default";
来源：http://baike.fanxiaobao.xyz/Article/details/gmkaeklkr.sHtML

[U54] PHP：空安全调用
来源：http://www.blog.fanxiaobao.xyz/Article/details/gcubbhicm.sHtML

$obj?->method()
来源：http://3g.fanxiaobao.xyz/Article/details/ghyismnff.sHtML

[U55] PHP：match 表达式
来源：http://mobile.fanxiaobao.xyz/Article/details/gnlgozuwi.sHtML

$s = match($x) { 1 => "一", default => "其他" };
来源：http://m.share.fanxiaobao.xyz/Article/details/gacglordj.sHtML

[U56] PHP：命名参数
来源：http://www.share.fanxiaobao.xyz/Article/details/goootfbch.sHtML

f(a: 1, b: 2)
来源：http://blog.fanxiaobao.xyz/Article/details/gretbantj.sHtML

[U57] PHP：字符串插值
来源：http://m.share.fanxiaobao.xyz/Article/details/gfxdtbqay.sHtML

"值: {$a}"
来源：http://mobile.fanxiaobao.xyz/Article/details/gllavlqry.sHtML

[U58] PHP：数组三件套
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gerfxiqti.sHtML

array_map($f, $a);  array_filter($a, $f);  array_reduce($a, $f, 0);
来源：http://mobile.fanxiaobao.xyz/Article/details/gtaozxzzq.sHtML

[U59] PHP：自定义排序
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gjmypmgof.sHtML

usort($arr, fn($a, $b) => $a["age"] <=> $b["age"]);
来源：http://3g.fanxiaobao.xyz/Article/details/gobfcfiej.sHtML

[U60] PHP：JSON 编解码
来源：http://www.blog.fanxiaobao.xyz/Article/details/gabqbvymo.sHtML

json_encode($d, JSON_UNESCAPED_UNICODE);  json_decode($s, true);
来源：http://www.blog.fanxiaobao.xyz/Article/details/gvxpizyoq.sHtML

[U61] PHP：正则
来源：http://mobile.fanxiaobao.xyz/Article/details/gaabwaifn.sHtML

preg_match('/(\d+)/', $s, $m);  preg_replace('/\d+/', '#', $s);
来源：http://www.blog.fanxiaobao.xyz/Article/details/gnshsjjud.sHtML

[U62] PHP：日期对象
来源：http://wap.fanxiaobao.xyz/Article/details/geeotdjtw.sHtML

(new DateTimeImmutable())->format("Y-m-d");
来源：http://baike.fanxiaobao.xyz/Article/details/gjeyomlpl.sHtML

[U63] PHP：文件读写
来源：http://read.share.fanxiaobao.xyz/Article/details/gosnzofdx.sHtML

file_get_contents($f);  file_put_contents($f, $data);
来源：http://wap.fanxiaobao.xyz/Article/details/gssaatpzq.sHtML

[U64] PHP：目录遍历
来源：http://www.share.fanxiaobao.xyz/Article/details/gwcdfwxac.sHtML

glob("dir/*.php");  scandir("dir");
来源：http://blog.fanxiaobao.xyz/Article/details/geqdduygs.sHtML

[U65] PHP：会话
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gvyestxsf.sHtML

session_start();  $_SESSION["uid"] = 1;
来源：http://read.share.fanxiaobao.xyz/Article/details/grldlhibf.sHtML

[U66] PHP：设置 Cookie
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gltagbtnl.sHtML

setcookie("token", $v, ["httponly" => true, "samesite" => "Lax"]);
来源：http://blog.fanxiaobao.xyz/Article/details/grxnzziao.sHtML

[U67] PHP：处理文件上传
来源：http://blog.fanxiaobao.xyz/Article/details/goegltqnz.sHtML

$_FILES["file"]["tmp_name"] 与 move_uploaded_file()
来源：http://m.share.fanxiaobao.xyz/Article/details/gouvnvgmb.sHtML

[U68] PHP：PDO 连接
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gvrcuyzvk.sHtML

$pdo = new PDO("mysql:host=localhost;dbname=app", "root", "");
来源：http://blog.fanxiaobao.xyz/Article/details/gmvzflviq.sHtML

[U69] PHP：PDO 预处理
来源：http://www.blog.fanxiaobao.xyz/Article/details/gtqgkqasd.sHtML

$stmt = $pdo->prepare("SELECT * FROM users WHERE id = ?");  $stmt->execute([$id]);
来源：http://m.share.fanxiaobao.xyz/Article/details/gqskdhbnz.sHtML

[U70] PHP：PDO 事务
来源：http://mobile.fanxiaobao.xyz/Article/details/gxexlnzbv.sHtML

$pdo->beginTransaction();  $pdo->commit();  $pdo->rollBack();
来源：http://www.blog.fanxiaobao.xyz/Article/details/gbhcllblm.sHtML

[U71] PHP：抛出异常
来源：http://3g.fanxiaobao.xyz/Article/details/giuagpmyy.sHtML

throw new RuntimeException("失败", 500);
来源：http://blog.fanxiaobao.xyz/Article/details/gieonddpa.sHtML

[U72] PHP：写错误日志
来源：http://www.blog.fanxiaobao.xyz/Article/details/gaonbjdmv.sHtML

error_log("失败: " . $e->getMessage());
来源：http://blog.fanxiaobao.xyz/Article/details/gjfnaujyw.sHtML

[U73] PHP：读取 ini 配置
来源：http://mobile.fanxiaobao.xyz/Article/details/gmncvwqga.sHtML

parse_ini_file("config.ini", true)
来源：http://m.share.fanxiaobao.xyz/Article/details/gxhffqbij.sHtML

[U74] PHP：读取环境变量
来源：http://wap.fanxiaobao.xyz/Article/details/gleehltaq.sHtML

getenv("APP_ENV") ?: "production"
来源：http://read.share.fanxiaobao.xyz/Article/details/gvwcezhxb.sHtML

[U75] PHP：依赖注入
来源：http://wap.fanxiaobao.xyz/Article/details/gxzsmlpex.sHtML

composer require psr/container
来源：http://3g.fanxiaobao.xyz/Article/details/gccvfxfhk.sHtML

[U76] PHP：简单路由
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gsklhlpep.sHtML

$path = parse_url($_SERVER["REQUEST_URI"], PHP_URL_PATH);
来源：http://wap.fanxiaobao.xyz/Article/details/gyhetirmp.sHtML

[U77] PHP：模板渲染
来源：http://3g.fanxiaobao.xyz/Article/details/ggdezhund.sHtML

composer require twig/twig
来源：http://m.share.fanxiaobao.xyz/Article/details/ggyfllhfs.sHtML

[U78] PHP：单元测试
来源：http://blog.fanxiaobao.xyz/Article/details/gjrzhbpip.sHtML

composer require --dev phpunit/phpunit
来源：http://baike.fanxiaobao.xyz/Article/details/gomjbxbpk.sHtML

[U79] PHP：静态分析
来源：http://m.share.fanxiaobao.xyz/Article/details/gxirstmqq.sHtML

composer require --dev phpstan/phpstan
来源：http://wap.fanxiaobao.xyz/Article/details/gxhzarigk.sHtML

[U80] PHP：代码规范修复
来源：http://wap.fanxiaobao.xyz/Article/details/gpfqklgww.sHtML

composer require --dev friendsofphp/php-cs-fixer
来源：http://wap.fanxiaobao.xyz/Article/details/gfsysehlq.sHtML

[U81] JS：初始化项目
来源：http://blog.fanxiaobao.xyz/Article/details/gsgaletlp.sHtML

npm init -y;  npm i express
来源：http://wap.fanxiaobao.xyz/Article/details/grgvmcgwr.sHtML

[U82] JS：package.json 脚本
来源：http://www.share.fanxiaobao.xyz/Article/details/gchxzznnw.sHtML

"scripts": { "dev": "vite", "build": "vite build" }
来源：http://www.share.fanxiaobao.xyz/Article/details/gpdurlkcf.sHtML

[U83] JS：ES Module 导入导出
来源：http://m.share.fanxiaobao.xyz/Article/details/gyotkbkom.sHtML

export const a = 1;  import { a } from "./m.js";
来源：http://3g.fanxiaobao.xyz/Article/details/gpmuaiaof.sHtML

[U84] JS：CommonJS 写法
来源：http://blog.fanxiaobao.xyz/Article/details/gytngexke.sHtML

module.exports = { a };  const { a } = require("./m");
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gvcqzgyrk.sHtML

[U85] JS：可选链
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gvahbahod.sHtML

a?.b?.c
来源：http://www.share.fanxiaobao.xyz/Article/details/gkzuowtbg.sHtML

[U86] JS：空值合并
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gaqpcqybh.sHtML

a ?? b
来源：http://3g.fanxiaobao.xyz/Article/details/gptzygmpf.sHtML

[U87] JS：解构默认值
来源：http://m.share.fanxiaobao.xyz/Article/details/ghzqgdhri.sHtML

const { a = 1, b = 2 } = obj;
来源：http://baike.fanxiaobao.xyz/Article/details/gtwwkbylr.sHtML

[U88] JS：对象展开合并
来源：http://www.blog.fanxiaobao.xyz/Article/details/gzgyueizi.sHtML

{ ...a, ...b }
来源：http://mobile.fanxiaobao.xyz/Article/details/gvezrltwo.sHtML

[U89] JS：数组去重
来源：http://read.share.fanxiaobao.xyz/Article/details/gfqfevorl.sHtML

[...new Set(arr)]
来源：http://baike.fanxiaobao.xyz/Article/details/ghpaibnfk.sHtML

[U90] JS：数字数组排序
来源：http://3g.fanxiaobao.xyz/Article/details/gbnlxzcuo.sHtML

[...arr].sort((a, b) => a - b)
来源：http://www.share.fanxiaobao.xyz/Article/details/gtxlhfgoa.sHtML

[U91] JS：对象键值遍历
来源：http://read.share.fanxiaobao.xyz/Article/details/gczlfrbsm.sHtML

Object.entries(obj).forEach(([k, v]) => {});
来源：http://wap.fanxiaobao.xyz/Article/details/gzatdhiwu.sHtML

[U92] JS：深拷贝
来源：http://baike.fanxiaobao.xyz/Article/details/geosmjmce.sHtML

structuredClone(obj)
来源：http://read.share.fanxiaobao.xyz/Article/details/gkoupebje.sHtML

[U93] JS：模板字符串
来源：http://blog.fanxiaobao.xyz/Article/details/gyovlifef.sHtML

`共 ${n} 条`
来源：http://wap.fanxiaobao.xyz/Article/details/ghodtitgr.sHtML

[U94] JS：箭头函数
来源：http://wap.fanxiaobao.xyz/Article/details/ghimdniqf.sHtML

const double = x => x * 2;
来源：http://m.share.fanxiaobao.xyz/Article/details/glawlwypz.sHtML

[U95] JS：Promise 包装
来源：http://mobile.fanxiaobao.xyz/Article/details/gpkrayfmz.sHtML

new Promise((resolve, reject) => {})
来源：http://m.share.fanxiaobao.xyz/Article/details/gxsywlxnj.sHtML

[U96] JS：async/await 与异常
来源：http://www.share.fanxiaobao.xyz/Article/details/gktulqsge.sHtML

try { const d = await f(); } catch (e) { console.error(e); }
来源：http://baike.fanxiaobao.xyz/Article/details/gdszeunam.sHtML

[U97] JS：并发请求
来源：http://wap.fanxiaobao.xyz/Article/details/gzwdjavpt.sHtML

await Promise.all(urls.map(u => fetch(u)))
来源：http://mobile.fanxiaobao.xyz/Article/details/grckdtixz.sHtML

[U98] JS：fetch 带 JSON
来源：http://wap.fanxiaobao.xyz/Article/details/grppibvdo.sHtML

await fetch(url, { method: "POST", headers: { "Content-Type": "application/json" }, body: JSON.stringify(d) })
来源：http://www.blog.fanxiaobao.xyz/Article/details/guppfwxnc.sHtML

[U99] JS：事件监听
来源：http://www.blog.fanxiaobao.xyz/Article/details/gzltoivzb.sHtML

el.addEventListener("click", e => {})
来源：http://blog.fanxiaobao.xyz/Article/details/gulqnbbme.sHtML

[U100] JS：DOM 查询
来源：http://m.share.fanxiaobao.xyz/Article/details/gnbxdpdei.sHtML

document.querySelector(".item")
来源：http://3g.fanxiaobao.xyz/Article/details/gktvqmymb.sHtML

[U101] JS：classList 操作
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gyxflmarj.sHtML

el.classList.toggle("active")
来源：http://blog.fanxiaobao.xyz/Article/details/gpaysmmma.sHtML

[U102] JS：本地存储
来源：http://blog.fanxiaobao.xyz/Article/details/gvlhipcir.sHtML

localStorage.setItem("k", JSON.stringify(v))
来源：http://www.blog.fanxiaobao.xyz/Article/details/gwfqtcuxr.sHtML

[U103] JS：定时器
来源：http://wap.fanxiaobao.xyz/Article/details/gabvhbnry.sHtML

setTimeout(fn, 1000);  setInterval(fn, 1000);
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gprwvishl.sHtML

[U104] JS：防抖
来源：http://mobile.fanxiaobao.xyz/Article/details/gxglmdgae.sHtML

const debounce = (fn, ms) => { let t; return (...a) => { clearTimeout(t); t = setTimeout(() => fn(...a), ms); }; };
来源：http://www.blog.fanxiaobao.xyz/Article/details/gpwoevqcb.sHtML

[U105] JS：节流
来源：http://m.share.fanxiaobao.xyz/Article/details/gcbbtrqxa.sHtML

const throttle = (fn, ms) => { let last = 0; return (...a) => { const n = Date.now(); if (n - last >= ms) { last = n; fn(...a); } }; };
来源：http://www.blog.fanxiaobao.xyz/Article/details/gnzfktiud.sHtML

[U106] JS：日期格式化
来源：http://www.share.fanxiaobao.xyz/Article/details/gfjtngeza.sHtML

new Intl.DateTimeFormat("zh-CN", { dateStyle: "medium" }).format(new Date())
来源：http://wap.fanxiaobao.xyz/Article/details/glvrexhjw.sHtML

[U107] JS：数字千分位
来源：http://read.share.fanxiaobao.xyz/Article/details/geizvglfj.sHtML

new Intl.NumberFormat("en-US").format(1234567)
来源：http://www.blog.fanxiaobao.xyz/Article/details/gbosvjjfl.sHtML

[U108] JS：随机整数
来源：http://baike.fanxiaobao.xyz/Article/details/gtkerljbo.sHtML

Math.floor(Math.random() * (max - min + 1)) + min
来源：http://read.share.fanxiaobao.xyz/Article/details/gdwyihusg.sHtML

[U109] JS：数组分组
来源：http://read.share.fanxiaobao.xyz/Article/details/guoxdpmrn.sHtML

Object.groupBy(arr, x => x.type)
来源：http://blog.fanxiaobao.xyz/Article/details/gipppqkxj.sHtML

[U110] JS：数组分块
来源：http://baike.fanxiaobao.xyz/Article/details/gsdwvwnhs.sHtML

arr.reduce((acc, x, i) => (i % size ? acc : [...acc, arr.slice(i, i + size)]), [])
来源：http://m.share.fanxiaobao.xyz/Article/details/gjihpdbce.sHtML

[U111] JS：对象转 Map
来源：http://www.blog.fanxiaobao.xyz/Article/details/gpsauhxuu.sHtML

new Map(Object.entries(obj))
来源：http://m.share.fanxiaobao.xyz/Article/details/gfigyfwas.sHtML

[U112] JS：字符串补位
来源：http://blog.fanxiaobao.xyz/Article/details/gerhpvzqt.sHtML

"7".padStart(3, "0")
来源：http://mobile.fanxiaobao.xyz/Article/details/gslnxwoen.sHtML

[U113] JS：正则替换全部
来源：http://blog.fanxiaobao.xyz/Article/details/gywtinsli.sHtML

s.replaceAll("a", "b")
来源：http://www.share.fanxiaobao.xyz/Article/details/gdkipzuad.sHtML

[U114] JS：JSON 深比较
来源：http://m.share.fanxiaobao.xyz/Article/details/gwvnrxcgb.sHtML

JSON.stringify(a) === JSON.stringify(b)
来源：http://blog.fanxiaobao.xyz/Article/details/groqpsigp.sHtML

[U115] JS：生成 UUID
来源：http://3g.fanxiaobao.xyz/Article/details/gjgqigmec.sHtML

crypto.randomUUID()
来源：http://read.share.fanxiaobao.xyz/Article/details/gsfmrfpwo.sHtML

[U116] JS：类型检查（JSDoc）
来源：http://m.share.fanxiaobao.xyz/Article/details/gpbkubjrr.sHtML

/** @param {string} name */ function f(name) {}
来源：http://baike.fanxiaobao.xyz/Article/details/gjjblovii.sHtML

[U117] JS：单元测试
来源：http://www.m.share.fanxiaobao.xyz/Article/details/glbdggwlp.sHtML

npm i -D vitest;  npx vitest
来源：http://mobile.fanxiaobao.xyz/Article/details/gxrubfijl.sHtML

[U118] JS：开发服务器
来源：http://mobile.fanxiaobao.xyz/Article/details/ghygfocno.sHtML

npm i -D vite;  npx vite
来源：http://wap.fanxiaobao.xyz/Article/details/gnwsvqazo.sHtML

[U119] JS：生产构建
来源：http://m.share.fanxiaobao.xyz/Article/details/gtolhykrz.sHtML

npx vite build
来源：http://mobile.fanxiaobao.xyz/Article/details/gparjacqc.sHtML

[U120] JS：读取环境变量（Vite）
来源：http://read.share.fanxiaobao.xyz/Article/details/gvngtcrev.sHtML

import.meta.env.VITE_API_URL
来源：http://3g.fanxiaobao.xyz/Article/details/grhfzmumn.sHtML

================================================================================
来源：http://www.share.fanxiaobao.xyz/Article/details/gbjdizkql.sHtML

统计汇总
来源：http://wap.fanxiaobao.xyz/Article/details/gpomhdtjn.sHtML

================================================================================
来源：http://blog.fanxiaobao.xyz/Article/details/gxxdefohn.sHtML

按语言统计（条）：
来源：http://blog.fanxiaobao.xyz/Article/details/gmufezkyl.sHtML

Python ......... 252
来源：http://mobile.fanxiaobao.xyz/Article/details/gdoughfhz.sHtML

PHP ............ 252
来源：http://www.share.fanxiaobao.xyz/Article/details/gttrhufll.sHtML

JavaScript ..... 252
来源：http://m.share.fanxiaobao.xyz/Article/details/gjzwkhczw.sHtML

TypeScript ..... 212
来源：http://baike.fanxiaobao.xyz/Article/details/gdizkkztk.sHtML

Java ........... 212
来源：http://www.blog.fanxiaobao.xyz/Article/details/gczwdfuyb.sHtML

Go ............. 212
来源：http://www.share.fanxiaobao.xyz/Article/details/gnpzxyjna.sHtML

Ruby ........... 212
来源：http://read.share.fanxiaobao.xyz/Article/details/gxxcmnizy.sHtML

C# ............. 212
来源：http://read.share.fanxiaobao.xyz/Article/details/gfchoiyod.sHtML

C .............. 30
来源：http://www.m.share.fanxiaobao.xyz/Article/details/geqzjiuvq.sHtML

C++ ............ 30
来源：http://mobile.fanxiaobao.xyz/Article/details/gbgfgchbt.sHtML

SQL ............ 90
来源：http://blog.fanxiaobao.xyz/Article/details/gzlwdrfnq.sHtML

Bash ........... 80
来源：http://blog.fanxiaobao.xyz/Article/details/ggylufmom.sHtML

Kotlin ......... 15
来源：http://mobile.fanxiaobao.xyz/Article/details/gcpgeaicg.sHtML

Swift .......... 15
来源：http://read.share.fanxiaobao.xyz/Article/details/guxbdhkez.sHtML

Lua ............ 10
来源：http://www.blog.fanxiaobao.xyz/Article/details/gsvrekwpn.sHtML

Perl ........... 10
来源：http://3g.fanxiaobao.xyz/Article/details/glzuxjzvx.sHtML

Scala .......... 10
来源：http://blog.fanxiaobao.xyz/Article/details/gwwfqvlbx.sHtML

------------------------------------
来源：http://www.blog.fanxiaobao.xyz/Article/details/ghtngluqj.sHtML

合计 ........... 2106 条
来源：http://m.share.fanxiaobao.xyz/Article/details/gjzegccof.sHtML

按章节统计：
来源：http://blog.fanxiaobao.xyz/Article/details/gucazvkbs.sHtML

A 基础语法与类型       26 个任务 × 8 语言 =  208
来源：http://blog.fanxiaobao.xyz/Article/details/gmdcghqnm.sHtML

B 流程控制             16 个任务 × 8 语言 =  128
来源：http://www.blog.fanxiaobao.xyz/Article/details/gcagopzho.sHtML

C 函数与作用域         16 个任务 × 8 语言 =  128
来源：http://mobile.fanxiaobao.xyz/Article/details/gprncfwyf.sHtML

D 数组 / 列表 / 集合   26 个任务 × 8 语言 =  208
来源：http://m.share.fanxiaobao.xyz/Article/details/gomshppkk.sHtML

E 字符串处理           22 个任务 × 8 语言 =  176
来源：http://wap.fanxiaobao.xyz/Article/details/goiyrsdtu.sHtML

F 文件与目录           12 个任务 × 8 语言 =   96
来源：http://www.m.share.fanxiaobao.xyz/Article/details/guezomlvr.sHtML

G 面向对象             16 个任务 × 8 语言 =  128
来源：http://blog.fanxiaobao.xyz/Article/details/gkjkqaefe.sHtML

H 异常与错误处理       10 个任务 × 8 语言 =   80
来源：http://blog.fanxiaobao.xyz/Article/details/gztvijgyh.sHtML

I 正则表达式            8 个任务 × 8 语言 =   64
来源：http://read.share.fanxiaobao.xyz/Article/details/gxeimukbq.sHtML

J 日期与时间           10 个任务 × 8 语言 =   80
来源：http://read.share.fanxiaobao.xyz/Article/details/gyhqtlzxw.sHtML

K JSON 与序列化         8 个任务 × 8 语言 =   64
来源：http://baike.fanxiaobao.xyz/Article/details/ghomtseqb.sHtML

L 网络请求              8 个任务 × 8 语言 =   64
来源：http://baike.fanxiaobao.xyz/Article/details/gvotrnlhv.sHtML

M 命令行 / 进程         8 个任务 × 8 语言 =   64
来源：http://www.blog.fanxiaobao.xyz/Article/details/guagzoixn.sHtML

N 数据结构与算法       12 个任务 × 8 语言 =   96
来源：http://baike.fanxiaobao.xyz/Article/details/gnyobssdw.sHtML

O 并发与异步            6 个任务 × 8 语言 =   48
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gfdrvjttf.sHtML

P 常用工具函数          8 个任务 × 8 语言 =   64
来源：http://m.share.fanxiaobao.xyz/Article/details/glxhuzkqb.sHtML

Q SQL 专题                              90
来源：http://www.blog.fanxiaobao.xyz/Article/details/gzsjmrani.sHtML

R Bash 专题                             80
来源：http://m.share.fanxiaobao.xyz/Article/details/gnajsbcmh.sHtML

S C / C++ 专题                          60
来源：http://mobile.fanxiaobao.xyz/Article/details/gmqnaygrm.sHtML

T 其他语言补充                          60
来源：http://mobile.fanxiaobao.xyz/Article/details/gbnlujhff.sHtML

U 高频实用片段                         120
来源：http://www.share.fanxiaobao.xyz/Article/details/gctzmgvna.sHtML

------------------------------------
来源：http://m.share.fanxiaobao.xyz/Article/details/gxqztytex.sHtML

合计                                  2106 条
来源：http://m.share.fanxiaobao.xyz/Article/details/gaqtksemm.sHtML

--------------------------------------------------------------------------------
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gfndxlvbz.sHtML

使用提醒
来源：http://www.blog.fanxiaobao.xyz/Article/details/gdwwjtwvw.sHtML

--------------------------------------------------------------------------------
来源：http://www.share.fanxiaobao.xyz/Article/details/goscxbffn.sHtML

1. 示例追求"最小可用"，正式项目中请补齐导入、错误处理与边界判断。
来源：http://m.share.fanxiaobao.xyz/Article/details/gtlxbujrl.sHtML

2. 涉及文件、网络、数据库的示例，注意资源释放与异常捕获。
来源：http://www.share.fanxiaobao.xyz/Article/details/guedylsvu.sHtML


<!-- 参考信息 -->