代发 wailian999

def add(a: Int, b: Int): Int = a + b
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gwmnioudg.sHtML

[T59] Scala：循环
来源：http://3g.fanxiaobao.xyz/Article/details/gfgletxfx.sHtML

for (i <- 1 to 10) println(i)
来源：http://blog.fanxiaobao.xyz/Article/details/gsbplvech.sHtML

[T60] Scala：折叠
来源：http://wap.fanxiaobao.xyz/Article/details/goptscyqy.sHtML

List(1, 2, 3).foldLeft(0)(_ + _)
来源：http://wap.fanxiaobao.xyz/Article/details/gdesymvtn.sHtML

================================================================================
来源：http://www.share.fanxiaobao.xyz/Article/details/ggoeepgni.sHtML

U. 高频实用片段（Python / PHP / JavaScript 各 40 条）
来源：http://3g.fanxiaobao.xyz/Article/details/ggtwoqunb.sHtML

================================================================================
来源：http://3g.fanxiaobao.xyz/Article/details/gwauywcpl.sHtML

[U01] Py：创建虚拟环境
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gevvwrqmg.sHtML

python -m venv .venv && source .venv/bin/activate
来源：http://read.share.fanxiaobao.xyz/Article/details/gxvumlmpl.sHtML

[U02] Py：导出 / 安装依赖
来源：http://baike.fanxiaobao.xyz/Article/details/gohgjzvie.sHtML

pip freeze > requirements.txt;  pip install -r requirements.txt
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gqoqjecni.sHtML

[U03] Py：加载 .env 配置
来源：http://mobile.fanxiaobao.xyz/Article/details/gvgothqjg.sHtML

from dotenv import load_dotenv; load_dotenv()
来源：http://baike.fanxiaobao.xyz/Article/details/gselqkppa.sHtML

[U04] Py：变量调试打印
来源：http://baike.fanxiaobao.xyz/Article/details/gkejpcdyl.sHtML

print(f"{x=}")            # 输出 x=值，Python 3.8+
来源：http://mobile.fanxiaobao.xyz/Article/details/gjvsymcjn.sHtML

[U05] Py：列表去重且保序
来源：http://read.share.fanxiaobao.xyz/Article/details/glipcoyir.sHtML

list(dict.fromkeys(arr))
来源：http://read.share.fanxiaobao.xyz/Article/details/gtqjozhbs.sHtML

[U06] Py：合并两个字典
来源：http://blog.fanxiaobao.xyz/Article/details/gimkfxbzv.sHtML

{**a, **b}
来源：http://mobile.fanxiaobao.xyz/Article/details/gmphnhoev.sHtML

[U07] Py：反转字典键值
来源：http://blog.fanxiaobao.xyz/Article/details/gcnzjfvlh.sHtML

{v: k for k, v in d.items()}
来源：http://blog.fanxiaobao.xyz/Article/details/gikokwhdt.sHtML

[U08] Py：展平二维列表
来源：http://www.m.share.fanxiaobao.xyz/Article/details/glfmbbgms.sHtML

[y for x in nested for y in x]
来源：http://m.share.fanxiaobao.xyz/Article/details/gvlflwaij.sHtML

[U09] Py：字典取最大值的键
来源：http://m.share.fanxiaobao.xyz/Article/details/gkuowbepa.sHtML

max(d, key=d.get)
来源：http://www.blog.fanxiaobao.xyz/Article/details/grdeskjbv.sHtML

[U10] Py：按值排序字典
来源：http://3g.fanxiaobao.xyz/Article/details/gjoxntujt.sHtML

dict(sorted(d.items(), key=lambda kv: kv[1]))
来源：http://www.share.fanxiaobao.xyz/Article/details/gqluctvwk.sHtML

[U11] Py：生成器表达式
来源：http://m.share.fanxiaobao.xyz/Article/details/gbfdolahc.sHtML

(x * 2 for x in arr)
来源：http://blog.fanxiaobao.xyz/Article/details/goqibtsmh.sHtML

[U12] Py：取出现最多的 3 个元素
来源：http://www.blog.fanxiaobao.xyz/Article/details/gugkddsux.sHtML

Counter(arr).most_common(3)
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gqtzayacf.sHtML

[U13] Py：固定长度队列
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gnqqbuwnl.sHtML

deque(maxlen=10)
来源：http://mobile.fanxiaobao.xyz/Article/details/giqggxcbk.sHtML

[U14] Py：分组收集到列表
来源：http://wap.fanxiaobao.xyz/Article/details/gacmwivdc.sHtML

defaultdict(list)
来源：http://blog.fanxiaobao.xyz/Article/details/gqbhzgmeg.sHtML

[U15] Py：高精度计时
来源：http://www.blog.fanxiaobao.xyz/Article/details/gqbjuuebk.sHtML

t = time.perf_counter()
来源：http://www.blog.fanxiaobao.xyz/Article/details/gypovumvn.sHtML

[U16] Py：命令行参数解析
来源：http://wap.fanxiaobao.xyz/Article/details/gdbzrzikr.sHtML

ap = argparse.ArgumentParser();  ap.add_argument("--name");  args = ap.parse_args()
来源：http://baike.fanxiaobao.xyz/Article/details/gijxtxqql.sHtML

[U17] Py：初始化日志
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gcuyfebkb.sHtML

logging.basicConfig(level=logging.INFO)
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gvprkxqpj.sHtML

[U18] Py：预编译正则
来源：http://baike.fanxiaobao.xyz/Article/details/guwcijztq.sHtML

pat = re.compile(r"\d+")
来源：http://mobile.fanxiaobao.xyz/Article/details/gkftzhlhg.sHtML

[U19] Py：正则替换带回调
来源：http://www.m.share.fanxiaobao.xyz/Article/details/ghkncwtkh.sHtML

re.sub(r"\d+", lambda m: str(int(m.group()) * 2), s)
来源：http://www.blog.fanxiaobao.xyz/Article/details/gmbqitjdw.sHtML

[U20] Py：缓存函数结果
来源：http://www.share.fanxiaobao.xyz/Article/details/gugcytbqi.sHtML

@functools.lru_cache(maxsize=None)
来源：http://m.share.fanxiaobao.xyz/Article/details/gftuurtvq.sHtML

[U21] Py：自定义上下文管理器
来源：http://m.share.fanxiaobao.xyz/Article/details/gjvvfenrv.sHtML

@contextlib.contextmanager
来源：http://www.blog.fanxiaobao.xyz/Article/details/girjwhwqc.sHtML

[U22] Py：矩阵转置
来源：http://mobile.fanxiaobao.xyz/Article/details/gnjijacce.sHtML

list(zip(*m))
来源：http://m.share.fanxiaobao.xyz/Article/details/gxifxmkfg.sHtML

[U23] Py：分块读取大文件
来源：http://3g.fanxiaobao.xyz/Article/details/gehybsqxs.sHtML

for chunk in iter(lambda: f.read(8192), b""):
来源：http://www.share.fanxiaobao.xyz/Article/details/gmqsggbah.sHtML

[U24] Py：路径操作
来源：http://mobile.fanxiaobao.xyz/Article/details/gkqpxojuu.sHtML

Path("a/b.txt").parent.mkdir(parents=True, exist_ok=True)
来源：http://www.blog.fanxiaobao.xyz/Article/details/gnxxpmcsu.sHtML

[U25] Py：CSV 按字典读
来源：http://baike.fanxiaobao.xyz/Article/details/guzlaxsrk.sHtML

csv.DictReader(f)
来源：http://m.share.fanxiaobao.xyz/Article/details/giibvxpxv.sHtML

[U26] Py：并发下载
来源：http://blog.fanxiaobao.xyz/Article/details/gwgsoxmhn.sHtML

ThreadPoolExecutor(max_workers=8).map(fetch, urls)
来源：http://www.blog.fanxiaobao.xyz/Article/details/gzvfibkhk.sHtML

[U27] Py：异步 HTTP
来源：http://blog.fanxiaobao.xyz/Article/details/gukkzcweq.sHtML

aiohttp.ClientSession() 配合 async with
来源：http://www.blog.fanxiaobao.xyz/Article/details/gjiwienao.sHtML

[U28] Py：类型别名
来源：http://blog.fanxiaobao.xyz/Article/details/gplyzwcid.sHtML

UserId = int
来源：http://wap.fanxiaobao.xyz/Article/details/gpfpwmemx.sHtML

[U29] Py：属性校验
来源：http://blog.fanxiaobao.xyz/Article/details/gjenhmzkg.sHtML

@property 与 @x.setter 配合
来源：http://www.blog.fanxiaobao.xyz/Article/details/gqjsrlixf.sHtML

[U30] Py：数据类
来源：http://www.blog.fanxiaobao.xyz/Article/details/glrbzbxuy.sHtML

@dataclass(slots=True)
来源：http://m.share.fanxiaobao.xyz/Article/details/gauvmpwpz.sHtML

[U31] Py：单测
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gcvyplhob.sHtML

python -m pytest -q
来源：http://m.share.fanxiaobao.xyz/Article/details/gqqjahdef.sHtML

[U32] Py：代码格式化
来源：http://blog.fanxiaobao.xyz/Article/details/gdmpsmnrd.sHtML

ruff format . && ruff check --fix .
来源：http://blog.fanxiaobao.xyz/Article/details/grenicikr.sHtML

[U33] Py：打包发布
来源：http://read.share.fanxiaobao.xyz/Article/details/gfwpilfem.sHtML

python -m build  （依赖 pyproject.toml）
来源：http://3g.fanxiaobao.xyz/Article/details/geeukumma.sHtML

[U34] Py：判断编码
来源：http://www.blog.fanxiaobao.xyz/Article/details/guilusunq.sHtML

chardet.detect(raw)
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gkmdygwbv.sHtML

[U35] Py：发送邮件
来源：http://www.share.fanxiaobao.xyz/Article/details/gpeftijcs.sHtML

smtplib.SMTP_SSL(...).send_message(msg)
来源：http://www.share.fanxiaobao.xyz/Article/details/gbnxlhfoi.sHtML

[U36] Py：定时任务
来源：http://blog.fanxiaobao.xyz/Article/details/gdlomcnuf.sHtML

schedule.every(10).minutes.do(job)
来源：http://3g.fanxiaobao.xyz/Article/details/gyzkfxyzv.sHtML

[U37] Py：读写 Excel
来源：http://blog.fanxiaobao.xyz/Article/details/gxcphzfjw.sHtML

pandas.read_excel / DataFrame.to_excel
来源：http://m.share.fanxiaobao.xyz/Article/details/gwkpojlrh.sHtML

[U38] Py：获取脚本所在目录
来源：http://wap.fanxiaobao.xyz/Article/details/gbvkkacpz.sHtML

Path(__file__).resolve().parent
来源：http://read.share.fanxiaobao.xyz/Article/details/gfxzaevkr.sHtML

[U39] Py：判断是否在交互环境
来源：http://www.m.share.fanxiaobao.xyz/Article/details/guxiamujl.sHtML

sys.stdout.isatty()
来源：http://www.blog.fanxiaobao.xyz/Article/details/gfiwnepok.sHtML

[U40] Py：打印到标准错误
来源：http://m.share.fanxiaobao.xyz/Article/details/gtseqvjut.sHtML

print("err", file=sys.stderr)
来源：http://mobile.fanxiaobao.xyz/Article/details/ghckaocqv.sHtML

[U41] PHP：初始化 Composer 项目
来源：http://m.share.fanxiaobao.xyz/Article/details/gzoujflkf.sHtML

composer init;  composer require guzzlehttp/guzzle
来源：http://baike.fanxiaobao.xyz/Article/details/gtcgwtvua.sHtML

[U42] PHP：PSR-4 自动加载
来源：http://baike.fanxiaobao.xyz/Article/details/gpveajwwu.sHtML

"autoload": { "psr-4": { "App\\": "src/" } }
来源：http://3g.fanxiaobao.xyz/Article/details/ggcvzstjs.sHtML

[U43] PHP：声明命名空间
来源：http://read.share.fanxiaobao.xyz/Article/details/gnoechsom.sHtML

namespace App\Http;
来源：http://mobile.fanxiaobao.xyz/Article/details/gvxyxfrwu.sHtML

[U44] PHP：开启严格类型
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gujgnwycb.sHtML

declare(strict_types=1);
来源：http://read.share.fanxiaobao.xyz/Article/details/gfgvmpbvc.sHtML

[U45] PHP：类型声明与返回类型
来源：http://3g.fanxiaobao.xyz/Article/details/gyxjzdtrn.sHtML

function add(int $a, int $b): int { return $a + $b; }
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gujmhcwbh.sHtML

[U46] PHP：可空类型
来源：http://blog.fanxiaobao.xyz/Article/details/gcpvudmam.sHtML

?string $name = null
来源：http://3g.fanxiaobao.xyz/Article/details/grqerehuy.sHtML

[U47] PHP：联合类型
来源：http://3g.fanxiaobao.xyz/Article/details/glbrgsrlf.sHtML

int|string $id
来源：http://www.blog.fanxiaobao.xyz/Article/details/geoevmzgy.sHtML

[U48] PHP：纯枚举
来源：http://www.share.fanxiaobao.xyz/Article/details/gbzlfjjpi.sHtML

enum Status: string { case Active = "active"; case Off = "off"; }
来源：http://baike.fanxiaobao.xyz/Article/details/ggtcgkpck.sHtML

[U49] PHP：只读属性
来源：http://wap.fanxiaobao.xyz/Article/details/grfmdgcoz.sHtML

public readonly string $name
来源：http://wap.fanxiaobao.xyz/Article/details/gkuulmopo.sHtML

[U50] PHP：构造器属性提升
来源：http://m.share.fanxiaobao.xyz/Article/details/gffmoqwpd.sHtML

public function __construct(private int $id) {}
来源：http://wap.fanxiaobao.xyz/Article/details/gxmjwnese.sHtML

[U51] PHP：数组解构
来源：http://read.share.fanxiaobao.xyz/Article/details/gammsrazd.sHtML

[$a, $b] = $arr;
来源：http://mobile.fanxiaobao.xyz/Article/details/gshvjqjyg.sHtML

[U52] PHP：箭头函数
来源：http://blog.fanxiaobao.xyz/Article/details/gfsrbnftv.sHtML

$double = fn($x) => $x * 2;
来源：http://wap.fanxiaobao.xyz/Article/details/ghcvqnlzr.sHtML

[U53] PHP：空合并运算符
来源：http://www.share.fanxiaobao.xyz/Article/details/gtzzmeofp.sHtML

$v = $a ?? $b ?? "default";
来源：http://www.blog.fanxiaobao.xyz/Article/details/gkfzctiqm.sHtML

[U54] PHP：空安全调用
来源：http://wap.fanxiaobao.xyz/Article/details/gumdjxgfq.sHtML

$obj?->method()
来源：http://baike.fanxiaobao.xyz/Article/details/gvxmeqcww.sHtML

[U55] PHP：match 表达式
来源：http://blog.fanxiaobao.xyz/Article/details/gfbfssjfa.sHtML

$s = match($x) { 1 => "一", default => "其他" };
来源：http://m.share.fanxiaobao.xyz/Article/details/gofqovbrq.sHtML

[U56] PHP：命名参数
来源：http://read.share.fanxiaobao.xyz/Article/details/gxfjjawbl.sHtML

f(a: 1, b: 2)
来源：http://3g.fanxiaobao.xyz/Article/details/gghdwgyep.sHtML

[U57] PHP：字符串插值
来源：http://www.blog.fanxiaobao.xyz/Article/details/gcjyifdpo.sHtML

"值: {$a}"
来源：http://3g.fanxiaobao.xyz/Article/details/gsiqcirju.sHtML

[U58] PHP：数组三件套
来源：http://mobile.fanxiaobao.xyz/Article/details/grsipgipo.sHtML

array_map($f, $a);  array_filter($a, $f);  array_reduce($a, $f, 0);
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gacqdjvdk.sHtML

[U59] PHP：自定义排序
来源：http://blog.fanxiaobao.xyz/Article/details/gyagkxpac.sHtML

usort($arr, fn($a, $b) => $a["age"] <=> $b["age"]);
来源：http://www.blog.fanxiaobao.xyz/Article/details/gnumegfeo.sHtML

[U60] PHP：JSON 编解码
来源：http://www.blog.fanxiaobao.xyz/Article/details/gsgfipixe.sHtML

json_encode($d, JSON_UNESCAPED_UNICODE);  json_decode($s, true);
来源：http://m.share.fanxiaobao.xyz/Article/details/gspqcplvn.sHtML

[U61] PHP：正则
来源：http://wap.fanxiaobao.xyz/Article/details/gdstzduvq.sHtML

preg_match('/(\d+)/', $s, $m);  preg_replace('/\d+/', '#', $s);
来源：http://m.share.fanxiaobao.xyz/Article/details/gskhwcvlc.sHtML

[U62] PHP：日期对象
来源：http://baike.fanxiaobao.xyz/Article/details/gxyuvavmx.sHtML

(new DateTimeImmutable())->format("Y-m-d");
来源：http://3g.fanxiaobao.xyz/Article/details/gputkfbes.sHtML

[U63] PHP：文件读写
来源：http://m.share.fanxiaobao.xyz/Article/details/gdhgesiqz.sHtML

file_get_contents($f);  file_put_contents($f, $data);
来源：http://read.share.fanxiaobao.xyz/Article/details/grgjraedu.sHtML

[U64] PHP：目录遍历
来源：http://read.share.fanxiaobao.xyz/Article/details/gcvnvsalg.sHtML

glob("dir/*.php");  scandir("dir");
来源：http://mobile.fanxiaobao.xyz/Article/details/gmyjcbdxx.sHtML

[U65] PHP：会话
来源：http://www.share.fanxiaobao.xyz/Article/details/gcphglewm.sHtML

session_start();  $_SESSION["uid"] = 1;
来源：http://m.share.fanxiaobao.xyz/Article/details/gvbcpyoyu.sHtML

[U66] PHP：设置 Cookie
来源：http://3g.fanxiaobao.xyz/Article/details/gumnfnfrl.sHtML

setcookie("token", $v, ["httponly" => true, "samesite" => "Lax"]);
来源：http://www.share.fanxiaobao.xyz/Article/details/gemaacjuj.sHtML

[U67] PHP：处理文件上传
来源：http://read.share.fanxiaobao.xyz/Article/details/gmnkolmoo.sHtML

$_FILES["file"]["tmp_name"] 与 move_uploaded_file()
来源：http://baike.fanxiaobao.xyz/Article/details/gegedjhkr.sHtML

[U68] PHP：PDO 连接
来源：http://blog.fanxiaobao.xyz/Article/details/gjhgkzreb.sHtML

$pdo = new PDO("mysql:host=localhost;dbname=app", "root", "");
来源：http://read.share.fanxiaobao.xyz/Article/details/gzlrvfmtd.sHtML

[U69] PHP：PDO 预处理
来源：http://baike.fanxiaobao.xyz/Article/details/geraddtam.sHtML

$stmt = $pdo->prepare("SELECT * FROM users WHERE id = ?");  $stmt->execute([$id]);
来源：http://wap.fanxiaobao.xyz/Article/details/gvcxxghev.sHtML

[U70] PHP：PDO 事务
来源：http://www.blog.fanxiaobao.xyz/Article/details/gutrdfhso.sHtML

$pdo->beginTransaction();  $pdo->commit();  $pdo->rollBack();
来源：http://m.share.fanxiaobao.xyz/Article/details/gvdrottoj.sHtML

[U71] PHP：抛出异常
来源：http://blog.fanxiaobao.xyz/Article/details/gtxmbsbhl.sHtML

throw new RuntimeException("失败", 500);
来源：http://3g.fanxiaobao.xyz/Article/details/glvgzlqmw.sHtML

[U72] PHP：写错误日志
来源：http://wap.fanxiaobao.xyz/Article/details/gkawgolqj.sHtML

error_log("失败: " . $e->getMessage());
来源：http://read.share.fanxiaobao.xyz/Article/details/ghntmuwwz.sHtML

[U73] PHP：读取 ini 配置
来源：http://wap.fanxiaobao.xyz/Article/details/gmopksuhn.sHtML

parse_ini_file("config.ini", true)
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gvtwfekuf.sHtML

[U74] PHP：读取环境变量
来源：http://www.share.fanxiaobao.xyz/Article/details/ggcuedvvk.sHtML

getenv("APP_ENV") ?: "production"
来源：http://blog.fanxiaobao.xyz/Article/details/gqqamzndt.sHtML

[U75] PHP：依赖注入
来源：http://read.share.fanxiaobao.xyz/Article/details/gunlwracw.sHtML

composer require psr/container
来源：http://baike.fanxiaobao.xyz/Article/details/glpwwgfub.sHtML

[U76] PHP：简单路由
来源：http://m.share.fanxiaobao.xyz/Article/details/gwttcburx.sHtML

$path = parse_url($_SERVER["REQUEST_URI"], PHP_URL_PATH);
来源：http://www.blog.fanxiaobao.xyz/Article/details/gtzoupbch.sHtML

[U77] PHP：模板渲染
来源：http://mobile.fanxiaobao.xyz/Article/details/gghfxplnp.sHtML

composer require twig/twig
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gqrdbcgit.sHtML

[U78] PHP：单元测试
来源：http://www.blog.fanxiaobao.xyz/Article/details/gbvgssgbc.sHtML

composer require --dev phpunit/phpunit
来源：http://baike.fanxiaobao.xyz/Article/details/ggcwhazqx.sHtML

[U79] PHP：静态分析
来源：http://mobile.fanxiaobao.xyz/Article/details/gohjqlyrg.sHtML

composer require --dev phpstan/phpstan
来源：http://wap.fanxiaobao.xyz/Article/details/gmcxandge.sHtML

[U80] PHP：代码规范修复
来源：http://3g.fanxiaobao.xyz/Article/details/gzqetwgdr.sHtML

composer require --dev friendsofphp/php-cs-fixer
来源：http://www.blog.fanxiaobao.xyz/Article/details/gcumcnnca.sHtML

[U81] JS：初始化项目
来源：http://blog.fanxiaobao.xyz/Article/details/guzmvjyiz.sHtML

npm init -y;  npm i express
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gmltptsml.sHtML

[U82] JS：package.json 脚本
来源：http://baike.fanxiaobao.xyz/Article/details/gmcuswuxv.sHtML

"scripts": { "dev": "vite", "build": "vite build" }
来源：http://m.share.fanxiaobao.xyz/Article/details/gpdffkclv.sHtML

[U83] JS：ES Module 导入导出
来源：http://www.blog.fanxiaobao.xyz/Article/details/gudurlutl.sHtML

export const a = 1;  import { a } from "./m.js";
来源：http://read.share.fanxiaobao.xyz/Article/details/gixkzxzbf.sHtML

[U84] JS：CommonJS 写法
来源：http://mobile.fanxiaobao.xyz/Article/details/ggfwnuyiz.sHtML

module.exports = { a };  const { a } = require("./m");
来源：http://mobile.fanxiaobao.xyz/Article/details/gylgjqurw.sHtML

[U85] JS：可选链
来源：http://3g.fanxiaobao.xyz/Article/details/gtgnsdzqk.sHtML

a?.b?.c
来源：http://3g.fanxiaobao.xyz/Article/details/gkzeybbzy.sHtML

[U86] JS：空值合并
来源：http://mobile.fanxiaobao.xyz/Article/details/gjmxoadro.sHtML

a ?? b
来源：http://wap.fanxiaobao.xyz/Article/details/gehgdlxwp.sHtML

[U87] JS：解构默认值
来源：http://3g.fanxiaobao.xyz/Article/details/gfwaavaet.sHtML

const { a = 1, b = 2 } = obj;
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gqaupoedr.sHtML

[U88] JS：对象展开合并
来源：http://baike.fanxiaobao.xyz/Article/details/ghgxskwrk.sHtML

{ ...a, ...b }
来源：http://read.share.fanxiaobao.xyz/Article/details/gyfvvgpij.sHtML

[U89] JS：数组去重
来源：http://m.share.fanxiaobao.xyz/Article/details/gsuuzrjxx.sHtML

[...new Set(arr)]
来源：http://m.share.fanxiaobao.xyz/Article/details/ggarthala.sHtML

[U90] JS：数字数组排序
来源：http://mobile.fanxiaobao.xyz/Article/details/gxjzlgjyp.sHtML

[...arr].sort((a, b) => a - b)
来源：http://m.share.fanxiaobao.xyz/Article/details/gqxosuvqm.sHtML

[U91] JS：对象键值遍历
来源：http://m.share.fanxiaobao.xyz/Article/details/gaugmuuks.sHtML

Object.entries(obj).forEach(([k, v]) => {});
来源：http://3g.fanxiaobao.xyz/Article/details/giwqckqvs.sHtML

[U92] JS：深拷贝
来源：http://baike.fanxiaobao.xyz/Article/details/ghxvigptv.sHtML

structuredClone(obj)
来源：http://baike.fanxiaobao.xyz/Article/details/gdmdhtksv.sHtML

[U93] JS：模板字符串
来源：http://mobile.fanxiaobao.xyz/Article/details/gsstpcmxu.sHtML

`共 ${n} 条`
来源：http://blog.fanxiaobao.xyz/Article/details/gtvwbeuqo.sHtML

[U94] JS：箭头函数
来源：http://www.blog.fanxiaobao.xyz/Article/details/gwvjqkisp.sHtML

const double = x => x * 2;
来源：http://wap.fanxiaobao.xyz/Article/details/gejzavzoi.sHtML

[U95] JS：Promise 包装
来源：http://m.share.fanxiaobao.xyz/Article/details/gifkkfpge.sHtML

new Promise((resolve, reject) => {})
来源：http://read.share.fanxiaobao.xyz/Article/details/gsaxbqych.sHtML

[U96] JS：async/await 与异常
来源：http://www.blog.fanxiaobao.xyz/Article/details/gabsyjqvw.sHtML

try { const d = await f(); } catch (e) { console.error(e); }
来源：http://read.share.fanxiaobao.xyz/Article/details/guqogqatv.sHtML

[U97] JS：并发请求
来源：http://read.share.fanxiaobao.xyz/Article/details/gbdgejhqo.sHtML

await Promise.all(urls.map(u => fetch(u)))
来源：http://mobile.fanxiaobao.xyz/Article/details/gvnwytulh.sHtML

[U98] JS：fetch 带 JSON
来源：http://www.blog.fanxiaobao.xyz/Article/details/gjahriash.sHtML

await fetch(url, { method: "POST", headers: { "Content-Type": "application/json" }, body: JSON.stringify(d) })
来源：http://www.share.fanxiaobao.xyz/Article/details/gxafuplfi.sHtML

[U99] JS：事件监听
来源：http://read.share.fanxiaobao.xyz/Article/details/gjqkqynal.sHtML

el.addEventListener("click", e => {})
来源：http://blog.fanxiaobao.xyz/Article/details/grigknslo.sHtML

[U100] JS：DOM 查询
来源：http://read.share.fanxiaobao.xyz/Article/details/gzeffayig.sHtML

document.querySelector(".item")
来源：http://wap.fanxiaobao.xyz/Article/details/gzfrldcsk.sHtML

[U101] JS：classList 操作
来源：http://blog.fanxiaobao.xyz/Article/details/gjvqvkvdt.sHtML

el.classList.toggle("active")
来源：http://mobile.fanxiaobao.xyz/Article/details/gfdhalhvy.sHtML

[U102] JS：本地存储
来源：http://m.share.fanxiaobao.xyz/Article/details/gpzzawuvc.sHtML

localStorage.setItem("k", JSON.stringify(v))
来源：http://baike.fanxiaobao.xyz/Article/details/getxpuszj.sHtML

[U103] JS：定时器
来源：http://www.share.fanxiaobao.xyz/Article/details/gznzkhmbq.sHtML

setTimeout(fn, 1000);  setInterval(fn, 1000);
来源：http://read.share.fanxiaobao.xyz/Article/details/gmdhwrzbo.sHtML

[U104] JS：防抖
来源：http://read.share.fanxiaobao.xyz/Article/details/gtkfumeqz.sHtML

const debounce = (fn, ms) => { let t; return (...a) => { clearTimeout(t); t = setTimeout(() => fn(...a), ms); }; };
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gmhsjdoik.sHtML

[U105] JS：节流
来源：http://mobile.fanxiaobao.xyz/Article/details/guocufxyd.sHtML

const throttle = (fn, ms) => { let last = 0; return (...a) => { const n = Date.now(); if (n - last >= ms) { last = n; fn(...a); } }; };
来源：http://blog.fanxiaobao.xyz/Article/details/gtscejufi.sHtML

[U106] JS：日期格式化
来源：http://3g.fanxiaobao.xyz/Article/details/gvgegsvsp.sHtML

new Intl.DateTimeFormat("zh-CN", { dateStyle: "medium" }).format(new Date())
来源：http://blog.fanxiaobao.xyz/Article/details/guypdpual.sHtML

[U107] JS：数字千分位
来源：http://baike.fanxiaobao.xyz/Article/details/ggsdiuawq.sHtML

new Intl.NumberFormat("en-US").format(1234567)
来源：http://m.share.fanxiaobao.xyz/Article/details/gxppzbysl.sHtML

[U108] JS：随机整数
来源：http://read.share.fanxiaobao.xyz/Article/details/gjnvgsyoi.sHtML

Math.floor(Math.random() * (max - min + 1)) + min
来源：http://wap.fanxiaobao.xyz/Article/details/gdmlauxgm.sHtML

[U109] JS：数组分组
来源：http://blog.fanxiaobao.xyz/Article/details/ghmluheny.sHtML

Object.groupBy(arr, x => x.type)
来源：http://m.share.fanxiaobao.xyz/Article/details/gnowdgjzc.sHtML

[U110] JS：数组分块
来源：http://baike.fanxiaobao.xyz/Article/details/grkcgfcte.sHtML

arr.reduce((acc, x, i) => (i % size ? acc : [...acc, arr.slice(i, i + size)]), [])
来源：http://baike.fanxiaobao.xyz/Article/details/giafxwnyx.sHtML

[U111] JS：对象转 Map
来源：http://m.share.fanxiaobao.xyz/Article/details/gbpflexpm.sHtML

new Map(Object.entries(obj))
来源：http://www.share.fanxiaobao.xyz/Article/details/gevjtjcvl.sHtML

[U112] JS：字符串补位
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gspliykzt.sHtML

"7".padStart(3, "0")
来源：http://www.share.fanxiaobao.xyz/Article/details/gzhxmkamu.sHtML

[U113] JS：正则替换全部
来源：http://blog.fanxiaobao.xyz/Article/details/grwffkzci.sHtML

s.replaceAll("a", "b")
来源：http://m.share.fanxiaobao.xyz/Article/details/gwzpuuonf.sHtML

[U114] JS：JSON 深比较
来源：http://www.share.fanxiaobao.xyz/Article/details/gzgiafhyn.sHtML

JSON.stringify(a) === JSON.stringify(b)
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gejmqyolq.sHtML

[U115] JS：生成 UUID
来源：http://blog.fanxiaobao.xyz/Article/details/gegrsiids.sHtML

crypto.randomUUID()
来源：http://read.share.fanxiaobao.xyz/Article/details/gangiutua.sHtML

[U116] JS：类型检查（JSDoc）
来源：http://wap.fanxiaobao.xyz/Article/details/gnizefzie.sHtML

/** @param {string} name */ function f(name) {}
来源：http://www.blog.fanxiaobao.xyz/Article/details/gwifvquwy.sHtML

[U117] JS：单元测试
来源：http://m.share.fanxiaobao.xyz/Article/details/geqlodmde.sHtML

npm i -D vitest;  npx vitest
来源：http://www.blog.fanxiaobao.xyz/Article/details/gsxyvlpdu.sHtML

[U118] JS：开发服务器
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gofplbmta.sHtML

npm i -D vite;  npx vite
来源：http://www.share.fanxiaobao.xyz/Article/details/gttimiuli.sHtML

[U119] JS：生产构建
来源：http://www.m.share.fanxiaobao.xyz/Article/details/grtxvylht.sHtML

npx vite build
来源：http://wap.fanxiaobao.xyz/Article/details/gaysldkwq.sHtML

[U120] JS：读取环境变量（Vite）
来源：http://www.blog.fanxiaobao.xyz/Article/details/ghmayldii.sHtML

import.meta.env.VITE_API_URL
来源：http://read.share.fanxiaobao.xyz/Article/details/gickqhgkh.sHtML

================================================================================
来源：http://wap.fanxiaobao.xyz/Article/details/gygpfcjsb.sHtML

统计汇总
来源：http://wap.fanxiaobao.xyz/Article/details/gvbzoexij.sHtML

================================================================================
来源：http://blog.fanxiaobao.xyz/Article/details/guhlrdtuh.sHtML

按语言统计（条）：
来源：http://baike.fanxiaobao.xyz/Article/details/gzthfgaiu.sHtML

Python ......... 252
来源：http://www.share.fanxiaobao.xyz/Article/details/gehnrpmau.sHtML

PHP ............ 252
来源：http://baike.fanxiaobao.xyz/Article/details/gwyjzezyt.sHtML

JavaScript ..... 252
来源：http://www.m.share.fanxiaobao.xyz/Article/details/glfyfdtrn.sHtML

TypeScript ..... 212
来源：http://3g.fanxiaobao.xyz/Article/details/gthlljkfm.sHtML

Java ........... 212
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gztfdspax.sHtML

Go ............. 212
来源：http://baike.fanxiaobao.xyz/Article/details/ggnpbhyoa.sHtML

Ruby ........... 212
来源：http://wap.fanxiaobao.xyz/Article/details/gpihprsjy.sHtML

C# ............. 212
来源：http://mobile.fanxiaobao.xyz/Article/details/gisiarzrw.sHtML

C .............. 30
来源：http://wap.fanxiaobao.xyz/Article/details/gtarmrezc.sHtML

C++ ............ 30
来源：http://baike.fanxiaobao.xyz/Article/details/gtforfiod.sHtML

SQL ............ 90
来源：http://www.blog.fanxiaobao.xyz/Article/details/gtlwiryga.sHtML

Bash ........... 80
来源：http://read.share.fanxiaobao.xyz/Article/details/gbcapshei.sHtML

Kotlin ......... 15
来源：http://mobile.fanxiaobao.xyz/Article/details/gpcyglxeu.sHtML

Swift .......... 15
来源：http://wap.fanxiaobao.xyz/Article/details/gtvyzhpdx.sHtML

Lua ............ 10
来源：http://www.share.fanxiaobao.xyz/Article/details/getiyzzjg.sHtML

Perl ........... 10
来源：http://3g.fanxiaobao.xyz/Article/details/gmalpuzxr.sHtML

Scala .......... 10
来源：http://www.blog.fanxiaobao.xyz/Article/details/gqqkmxcxk.sHtML

------------------------------------
来源：http://read.share.fanxiaobao.xyz/Article/details/gkfqgpnim.sHtML

合计 ........... 2106 条
来源：http://blog.fanxiaobao.xyz/Article/details/grtvyuqxd.sHtML

按章节统计：
来源：http://blog.fanxiaobao.xyz/Article/details/grtqgzvqr.sHtML

A 基础语法与类型       26 个任务 × 8 语言 =  208
来源：http://mobile.fanxiaobao.xyz/Article/details/gxfatwaek.sHtML

B 流程控制             16 个任务 × 8 语言 =  128
来源：http://read.share.fanxiaobao.xyz/Article/details/gzljbyalj.sHtML

C 函数与作用域         16 个任务 × 8 语言 =  128
来源：http://mobile.fanxiaobao.xyz/Article/details/gbdhdtecg.sHtML

D 数组 / 列表 / 集合   26 个任务 × 8 语言 =  208
来源：http://www.share.fanxiaobao.xyz/Article/details/gogmfhjlj.sHtML

E 字符串处理           22 个任务 × 8 语言 =  176
来源：http://www.share.fanxiaobao.xyz/Article/details/gnsntvgtr.sHtML

F 文件与目录           12 个任务 × 8 语言 =   96
来源：http://m.share.fanxiaobao.xyz/Article/details/gmzzgpdwy.sHtML

G 面向对象             16 个任务 × 8 语言 =  128
来源：http://read.share.fanxiaobao.xyz/Article/details/gqvqswotw.sHtML

H 异常与错误处理       10 个任务 × 8 语言 =   80
来源：http://www.blog.fanxiaobao.xyz/Article/details/goshybmjf.sHtML

I 正则表达式            8 个任务 × 8 语言 =   64
来源：http://3g.fanxiaobao.xyz/Article/details/gyraxtmwf.sHtML

J 日期与时间           10 个任务 × 8 语言 =   80
来源：http://baike.fanxiaobao.xyz/Article/details/gqhgeirai.sHtML

K JSON 与序列化         8 个任务 × 8 语言 =   64
来源：http://blog.fanxiaobao.xyz/Article/details/grxjttlob.sHtML

L 网络请求              8 个任务 × 8 语言 =   64
来源：http://www.m.share.fanxiaobao.xyz/Article/details/glzyuexqz.sHtML

M 命令行 / 进程         8 个任务 × 8 语言 =   64
来源：http://m.share.fanxiaobao.xyz/Article/details/ggtlmycew.sHtML

N 数据结构与算法       12 个任务 × 8 语言 =   96
来源：http://m.share.fanxiaobao.xyz/Article/details/gmeqpdbur.sHtML

O 并发与异步            6 个任务 × 8 语言 =   48
来源：http://wap.fanxiaobao.xyz/Article/details/gxehtvpsi.sHtML

P 常用工具函数          8 个任务 × 8 语言 =   64
来源：http://m.share.fanxiaobao.xyz/Article/details/gjnascbpr.sHtML

Q SQL 专题                              90
来源：http://www.blog.fanxiaobao.xyz/Article/details/grlmgyjfv.sHtML

R Bash 专题                             80
来源：http://baike.fanxiaobao.xyz/Article/details/gewbtrwop.sHtML

S C / C++ 专题                          60
来源：http://blog.fanxiaobao.xyz/Article/details/ghsxfzsfx.sHtML

T 其他语言补充                          60
来源：http://read.share.fanxiaobao.xyz/Article/details/gtqiyeprc.sHtML

U 高频实用片段                         120
来源：http://3g.fanxiaobao.xyz/Article/details/gphegfeqy.sHtML

------------------------------------
来源：http://wap.fanxiaobao.xyz/Article/details/gfhfcorqj.sHtML

合计                                  2106 条
来源：http://www.blog.fanxiaobao.xyz/Article/details/gkrdzsgjc.sHtML

--------------------------------------------------------------------------------
来源：http://www.blog.fanxiaobao.xyz/Article/details/gkvskcktl.sHtML

使用提醒
来源：http://m.share.fanxiaobao.xyz/Article/details/gmsaymnoy.sHtML

--------------------------------------------------------------------------------
来源：http://mobile.fanxiaobao.xyz/Article/details/gruytbctz.sHtML

1. 示例追求"最小可用"，正式项目中请补齐导入、错误处理与边界判断。
来源：http://baike.fanxiaobao.xyz/Article/details/grlwqcbob.sHtML

2. 涉及文件、网络、数据库的示例，注意资源释放与异常捕获。
来源：http://wap.fanxiaobao.xyz/Article/details/gfmikcaoc.sHtML


<!-- 参考信息 -->