代发 wailian999

[U05] Py：列表去重且保序
来源：http://www.m.share.fehbvm.com/Article/details/gqgsievcr.sHtML

list(dict.fromkeys(arr))
来源：http://www.share.hesvh.cn/Article/details/gawuwfuij.sHtML

[U06] Py：合并两个字典
来源：http://wap.fehbvm.com/Article/details/gtwznmwhc.sHtML

{**a, **b}
来源：http://read.share.zdbjq.cn/Article/details/gveufbxbz.sHtML

[U07] Py：反转字典键值
来源：http://m.share.fehbvm.com/Article/details/glerfmrju.sHtML

{v: k for k, v in d.items()}
来源：http://mobile.hesvh.cn/Article/details/gaedupclu.sHtML

[U08] Py：展平二维列表
来源：http://www.m.share.zdbjq.cn/Article/details/gypwfmyje.sHtML

[y for x in nested for y in x]
来源：http://mobile.zdbjq.cn/Article/details/gtinkihxd.sHtML

[U09] Py：字典取最大值的键
来源：http://m.share.zdbjq.cn/Article/details/glgnbqmow.sHtML

max(d, key=d.get)
来源：http://m.share.hesvh.cn/Article/details/gxqptzupz.sHtML

[U10] Py：按值排序字典
来源：http://baike.hesvh.cn/Article/details/guqjminbo.sHtML

dict(sorted(d.items(), key=lambda kv: kv[1]))
来源：http://wap.zdbjq.cn/Article/details/gkhixhbma.sHtML

[U11] Py：生成器表达式
来源：http://www.m.share.hesvh.cn/Article/details/ghevrnpkn.sHtML

(x * 2 for x in arr)
来源：http://www.share.hesvh.cn/Article/details/gvatcxxby.sHtML

[U12] Py：取出现最多的 3 个元素
来源：http://www.blog.hesvh.cn/Article/details/ggnmsnhqf.sHtML

Counter(arr).most_common(3)
来源：http://www.m.share.zdbjq.cn/Article/details/ghvytmrny.sHtML

[U13] Py：固定长度队列
来源：http://mobile.zdbjq.cn/Article/details/ghwnaxrft.sHtML

deque(maxlen=10)
来源：http://m.share.hesvh.cn/Article/details/gwnrlaviy.sHtML

[U14] Py：分组收集到列表
来源：http://wap.hesvh.cn/Article/details/giosnnoah.sHtML

defaultdict(list)
来源：http://www.blog.hesvh.cn/Article/details/gabibuzey.sHtML

[U15] Py：高精度计时
来源：http://mobile.fehbvm.com/Article/details/gvkemjbkz.sHtML

t = time.perf_counter()
来源：http://baike.fehbvm.com/Article/details/gyblumqnm.sHtML

[U16] Py：命令行参数解析
来源：http://www.m.share.zdbjq.cn/Article/details/gwnpftegi.sHtML

ap = argparse.ArgumentParser();  ap.add_argument("--name");  args = ap.parse_args()
来源：http://blog.zdbjq.cn/Article/details/gkznbeuzt.sHtML

[U17] Py：初始化日志
来源：http://mobile.hesvh.cn/Article/details/gugeajwib.sHtML

logging.basicConfig(level=logging.INFO)
来源：http://mobile.zdbjq.cn/Article/details/gbgdqeimt.sHtML

[U18] Py：预编译正则
来源：http://www.m.share.fehbvm.com/Article/details/giekrovre.sHtML

pat = re.compile(r"\d+")
来源：http://www.blog.hesvh.cn/Article/details/gqehiveal.sHtML

[U19] Py：正则替换带回调
来源：http://blog.fehbvm.com/Article/details/gbkaqdyfg.sHtML

re.sub(r"\d+", lambda m: str(int(m.group()) * 2), s)
来源：http://baike.zdbjq.cn/Article/details/gewaqewvf.sHtML

[U20] Py：缓存函数结果
来源：http://mobile.zdbjq.cn/Article/details/gxlpilehh.sHtML

@functools.lru_cache(maxsize=None)
来源：http://wap.hesvh.cn/Article/details/grgjcklcf.sHtML

[U21] Py：自定义上下文管理器
来源：http://mobile.hesvh.cn/Article/details/ghhksdtft.sHtML

@contextlib.contextmanager
来源：http://3g.hesvh.cn/Article/details/gohadgjvr.sHtML

[U22] Py：矩阵转置
来源：http://www.blog.zdbjq.cn/Article/details/gjammytex.sHtML

list(zip(*m))
来源：http://m.share.zdbjq.cn/Article/details/gppncksyz.sHtML

[U23] Py：分块读取大文件
来源：http://mobile.hesvh.cn/Article/details/gitthbqfl.sHtML

for chunk in iter(lambda: f.read(8192), b""):
来源：http://read.share.hesvh.cn/Article/details/glcgorfgy.sHtML

[U24] Py：路径操作
来源：http://www.m.share.hesvh.cn/Article/details/gvzhpxubs.sHtML

Path("a/b.txt").parent.mkdir(parents=True, exist_ok=True)
来源：http://m.share.hesvh.cn/Article/details/gfucplvai.sHtML

[U25] Py：CSV 按字典读
来源：http://www.m.share.fehbvm.com/Article/details/ggrhutzgg.sHtML

csv.DictReader(f)
来源：http://www.share.zdbjq.cn/Article/details/gxrzmwwcj.sHtML

[U26] Py：并发下载
来源：http://www.m.share.zdbjq.cn/Article/details/gnoxlzatc.sHtML

ThreadPoolExecutor(max_workers=8).map(fetch, urls)
来源：http://mobile.hesvh.cn/Article/details/gwtgppikm.sHtML

[U27] Py：异步 HTTP
来源：http://www.blog.zdbjq.cn/Article/details/gflfghkrz.sHtML

aiohttp.ClientSession() 配合 async with
来源：http://blog.hesvh.cn/Article/details/gbowozamf.sHtML

[U28] Py：类型别名
来源：http://m.share.hesvh.cn/Article/details/gmdnknnua.sHtML

UserId = int
来源：http://wap.fehbvm.com/Article/details/gqpkzrslo.sHtML

[U29] Py：属性校验
来源：http://www.blog.fehbvm.com/Article/details/guucqyczl.sHtML

@property 与 @x.setter 配合
来源：http://mobile.hesvh.cn/Article/details/gjjjlleni.sHtML

[U30] Py：数据类
来源：http://m.share.fehbvm.com/Article/details/gualgouoi.sHtML

@dataclass(slots=True)
来源：http://wap.fehbvm.com/Article/details/ggzlsxvsv.sHtML

[U31] Py：单测
来源：http://mobile.hesvh.cn/Article/details/gmbjwihae.sHtML

python -m pytest -q
来源：http://www.blog.zdbjq.cn/Article/details/gkvttbsub.sHtML

[U32] Py：代码格式化
来源：http://mobile.zdbjq.cn/Article/details/gpaqpxpas.sHtML

ruff format . && ruff check --fix .
来源：http://read.share.zdbjq.cn/Article/details/gbbfrboaq.sHtML

[U33] Py：打包发布
来源：http://www.share.hesvh.cn/Article/details/gojooxzkw.sHtML

python -m build  （依赖 pyproject.toml）
来源：http://3g.zdbjq.cn/Article/details/gnlznjpvt.sHtML

[U34] Py：判断编码
来源：http://3g.fehbvm.com/Article/details/glrgnqxzn.sHtML

chardet.detect(raw)
来源：http://3g.fehbvm.com/Article/details/gznwprgyv.sHtML

[U35] Py：发送邮件
来源：http://mobile.hesvh.cn/Article/details/guqwbswmu.sHtML

smtplib.SMTP_SSL(...).send_message(msg)
来源：http://baike.fehbvm.com/Article/details/gtpnokovx.sHtML

[U36] Py：定时任务
来源：http://mobile.fehbvm.com/Article/details/gvarngeyh.sHtML

schedule.every(10).minutes.do(job)
来源：http://mobile.zdbjq.cn/Article/details/gfppkgiwq.sHtML

[U37] Py：读写 Excel
来源：http://wap.hesvh.cn/Article/details/grffzpzsn.sHtML

pandas.read_excel / DataFrame.to_excel
来源：http://blog.hesvh.cn/Article/details/glyvwlugn.sHtML

[U38] Py：获取脚本所在目录
来源：http://3g.zdbjq.cn/Article/details/gruixmsla.sHtML

Path(__file__).resolve().parent
来源：http://mobile.zdbjq.cn/Article/details/gxxxdqejl.sHtML

[U39] Py：判断是否在交互环境
来源：http://www.m.share.zdbjq.cn/Article/details/gbezdlaer.sHtML

sys.stdout.isatty()
来源：http://mobile.fehbvm.com/Article/details/gnlvlnhtu.sHtML

[U40] Py：打印到标准错误
来源：http://www.blog.fehbvm.com/Article/details/gujhkgoxe.sHtML

print("err", file=sys.stderr)
来源：http://3g.hesvh.cn/Article/details/gonaxawut.sHtML

[U41] PHP：初始化 Composer 项目
来源：http://www.m.share.zdbjq.cn/Article/details/gbjjawprn.sHtML

composer init;  composer require guzzlehttp/guzzle
来源：http://3g.zdbjq.cn/Article/details/gnzknltxh.sHtML

[U42] PHP：PSR-4 自动加载
来源：http://www.blog.fehbvm.com/Article/details/gcrkzhknl.sHtML

"autoload": { "psr-4": { "App\\": "src/" } }
来源：http://mobile.fehbvm.com/Article/details/ghlrskzjv.sHtML

[U43] PHP：声明命名空间
来源：http://read.share.hesvh.cn/Article/details/gdbebzbmm.sHtML

namespace App\Http;
来源：http://blog.fehbvm.com/Article/details/gwudidcdh.sHtML

[U44] PHP：开启严格类型
来源：http://m.share.zdbjq.cn/Article/details/gogmumcqf.sHtML

declare(strict_types=1);
来源：http://mobile.fehbvm.com/Article/details/gyouwxqqc.sHtML

[U45] PHP：类型声明与返回类型
来源：http://www.blog.fehbvm.com/Article/details/gefljatnu.sHtML

function add(int $a, int $b): int { return $a + $b; }
来源：http://blog.zdbjq.cn/Article/details/gdtnloggy.sHtML

[U46] PHP：可空类型
来源：http://www.m.share.zdbjq.cn/Article/details/gzvoqoxul.sHtML

?string $name = null
来源：http://www.m.share.zdbjq.cn/Article/details/govjxhqzb.sHtML

[U47] PHP：联合类型
来源：http://www.blog.zdbjq.cn/Article/details/gaywzxqzj.sHtML

int|string $id
来源：http://baike.hesvh.cn/Article/details/gyjqxralt.sHtML

[U48] PHP：纯枚举
来源：http://m.share.fehbvm.com/Article/details/gzennloew.sHtML

enum Status: string { case Active = "active"; case Off = "off"; }
来源：http://www.m.share.fehbvm.com/Article/details/gybrnfqjw.sHtML

[U49] PHP：只读属性
来源：http://m.share.fehbvm.com/Article/details/gcwqmeoxc.sHtML

public readonly string $name
来源：http://3g.fehbvm.com/Article/details/ggcfincga.sHtML

[U50] PHP：构造器属性提升
来源：http://blog.hesvh.cn/Article/details/ggeloubut.sHtML

public function __construct(private int $id) {}
来源：http://m.share.hesvh.cn/Article/details/gpulcxjkh.sHtML

[U51] PHP：数组解构
来源：http://blog.hesvh.cn/Article/details/gobwdshlf.sHtML

[$a, $b] = $arr;
来源：http://www.blog.fehbvm.com/Article/details/gvkrkbzsr.sHtML

[U52] PHP：箭头函数
来源：http://www.share.fehbvm.com/Article/details/gqbaxdxzl.sHtML

$double = fn($x) => $x * 2;
来源：http://www.blog.zdbjq.cn/Article/details/gkrppyueq.sHtML

[U53] PHP：空合并运算符
来源：http://blog.zdbjq.cn/Article/details/gefxirlwy.sHtML

$v = $a ?? $b ?? "default";
来源：http://www.m.share.hesvh.cn/Article/details/gjdpcnduy.sHtML

[U54] PHP：空安全调用
来源：http://www.share.fehbvm.com/Article/details/gdbbtagti.sHtML

$obj?->method()
来源：http://www.blog.zdbjq.cn/Article/details/gqlmyisim.sHtML

[U55] PHP：match 表达式
来源：http://blog.hesvh.cn/Article/details/glqpuxiux.sHtML

$s = match($x) { 1 => "一", default => "其他" };
来源：http://www.blog.zdbjq.cn/Article/details/grncaxeje.sHtML

[U56] PHP：命名参数
来源：http://www.blog.zdbjq.cn/Article/details/ghcekxqzt.sHtML

f(a: 1, b: 2)
来源：http://www.m.share.fehbvm.com/Article/details/gzpkcdplx.sHtML

[U57] PHP：字符串插值
来源：http://mobile.hesvh.cn/Article/details/gihoxsjuv.sHtML

"值: {$a}"
来源：http://m.share.zdbjq.cn/Article/details/gfwawbwhn.sHtML

[U58] PHP：数组三件套
来源：http://m.share.zdbjq.cn/Article/details/gpyshmloh.sHtML

array_map($f, $a);  array_filter($a, $f);  array_reduce($a, $f, 0);
来源：http://wap.zdbjq.cn/Article/details/gxoaunngy.sHtML

[U59] PHP：自定义排序
来源：http://baike.zdbjq.cn/Article/details/gaavksaqe.sHtML

usort($arr, fn($a, $b) => $a["age"] <=> $b["age"]);
来源：http://www.blog.fehbvm.com/Article/details/gdtjhcvbu.sHtML

[U60] PHP：JSON 编解码
来源：http://3g.zdbjq.cn/Article/details/gmulzawvv.sHtML

json_encode($d, JSON_UNESCAPED_UNICODE);  json_decode($s, true);
来源：http://read.share.zdbjq.cn/Article/details/gbnwkroky.sHtML

[U61] PHP：正则
来源：http://www.share.zdbjq.cn/Article/details/gzdkxtjzd.sHtML

preg_match('/(\d+)/', $s, $m);  preg_replace('/\d+/', '#', $s);
来源：http://3g.zdbjq.cn/Article/details/gykfzmkoz.sHtML

[U62] PHP：日期对象
来源：http://baike.hesvh.cn/Article/details/gnmtzuwnv.sHtML

(new DateTimeImmutable())->format("Y-m-d");
来源：http://www.share.fehbvm.com/Article/details/grizlypcs.sHtML

[U63] PHP：文件读写
来源：http://blog.zdbjq.cn/Article/details/grfyxvmug.sHtML

file_get_contents($f);  file_put_contents($f, $data);
来源：http://www.share.zdbjq.cn/Article/details/gefrjzeso.sHtML

[U64] PHP：目录遍历
来源：http://baike.hesvh.cn/Article/details/gklundwtf.sHtML

glob("dir/*.php");  scandir("dir");
来源：http://www.share.zdbjq.cn/Article/details/gqbcysgzr.sHtML

[U65] PHP：会话
来源：http://www.m.share.zdbjq.cn/Article/details/gcxkkgizt.sHtML

session_start();  $_SESSION["uid"] = 1;
来源：http://www.m.share.zdbjq.cn/Article/details/gdbyndefy.sHtML

[U66] PHP：设置 Cookie
来源：http://3g.hesvh.cn/Article/details/gqrnqmlwx.sHtML

setcookie("token", $v, ["httponly" => true, "samesite" => "Lax"]);
来源：http://wap.zdbjq.cn/Article/details/gtaxfxjtf.sHtML

[U67] PHP：处理文件上传
来源：http://3g.zdbjq.cn/Article/details/gwcmqncuj.sHtML

$_FILES["file"]["tmp_name"] 与 move_uploaded_file()
来源：http://wap.fehbvm.com/Article/details/gllnkrdqz.sHtML

[U68] PHP：PDO 连接
来源：http://m.share.fehbvm.com/Article/details/gpzuxasaw.sHtML

$pdo = new PDO("mysql:host=localhost;dbname=app", "root", "");
来源：http://www.m.share.fehbvm.com/Article/details/gmxlqaklz.sHtML

[U69] PHP：PDO 预处理
来源：http://m.share.hesvh.cn/Article/details/gafzkkadn.sHtML

$stmt = $pdo->prepare("SELECT * FROM users WHERE id = ?");  $stmt->execute([$id]);
来源：http://m.share.fehbvm.com/Article/details/gvrjblpoz.sHtML

[U70] PHP：PDO 事务
来源：http://3g.fehbvm.com/Article/details/glafbugkf.sHtML

$pdo->beginTransaction();  $pdo->commit();  $pdo->rollBack();
来源：http://www.m.share.fehbvm.com/Article/details/gflvefvsj.sHtML

[U71] PHP：抛出异常
来源：http://3g.fehbvm.com/Article/details/gidapaqjy.sHtML

throw new RuntimeException("失败", 500);
来源：http://www.share.hesvh.cn/Article/details/gnxqsluzm.sHtML

[U72] PHP：写错误日志
来源：http://www.m.share.hesvh.cn/Article/details/gorwtfuwd.sHtML

error_log("失败: " . $e->getMessage());
来源：http://3g.zdbjq.cn/Article/details/gxrymtydu.sHtML

[U73] PHP：读取 ini 配置
来源：http://baike.zdbjq.cn/Article/details/gfkmbvwkz.sHtML

parse_ini_file("config.ini", true)
来源：http://baike.zdbjq.cn/Article/details/grsyzmgxg.sHtML

[U74] PHP：读取环境变量
来源：http://www.blog.zdbjq.cn/Article/details/goxifsloe.sHtML

getenv("APP_ENV") ?: "production"
来源：http://m.share.hesvh.cn/Article/details/gbojbfvjp.sHtML

[U75] PHP：依赖注入
来源：http://www.blog.fehbvm.com/Article/details/gltehlizl.sHtML

composer require psr/container
来源：http://blog.hesvh.cn/Article/details/gdlqisdch.sHtML

[U76] PHP：简单路由
来源：http://blog.fehbvm.com/Article/details/gsyjydgns.sHtML

$path = parse_url($_SERVER["REQUEST_URI"], PHP_URL_PATH);
来源：http://www.m.share.zdbjq.cn/Article/details/gzurajjku.sHtML

[U77] PHP：模板渲染
来源：http://3g.zdbjq.cn/Article/details/gblixgzld.sHtML

composer require twig/twig
来源：http://3g.zdbjq.cn/Article/details/goosmxkoa.sHtML

[U78] PHP：单元测试
来源：http://wap.zdbjq.cn/Article/details/glsxrlrfu.sHtML

composer require --dev phpunit/phpunit
来源：http://3g.fehbvm.com/Article/details/gdzywiivc.sHtML

[U79] PHP：静态分析
来源：http://baike.zdbjq.cn/Article/details/gaxmzouis.sHtML

composer require --dev phpstan/phpstan
来源：http://mobile.hesvh.cn/Article/details/gziahdnmz.sHtML

[U80] PHP：代码规范修复
来源：http://blog.fehbvm.com/Article/details/ghwnfdkiq.sHtML

composer require --dev friendsofphp/php-cs-fixer
来源：http://www.share.fehbvm.com/Article/details/grdloqizh.sHtML

[U81] JS：初始化项目
来源：http://www.m.share.hesvh.cn/Article/details/gkggqhmwm.sHtML

npm init -y;  npm i express
来源：http://www.blog.fehbvm.com/Article/details/genlspfvl.sHtML

[U82] JS：package.json 脚本
来源：http://mobile.zdbjq.cn/Article/details/godokjgff.sHtML

"scripts": { "dev": "vite", "build": "vite build" }
来源：http://baike.zdbjq.cn/Article/details/gxahmypxy.sHtML

[U83] JS：ES Module 导入导出
来源：http://read.share.hesvh.cn/Article/details/gfihflszh.sHtML

export const a = 1;  import { a } from "./m.js";
来源：http://read.share.hesvh.cn/Article/details/gcohdxcsw.sHtML

[U84] JS：CommonJS 写法
来源：http://3g.zdbjq.cn/Article/details/glwrmrsdw.sHtML

module.exports = { a };  const { a } = require("./m");
来源：http://wap.zdbjq.cn/Article/details/gtprewmub.sHtML

[U85] JS：可选链
来源：http://m.share.hesvh.cn/Article/details/gstaiaidj.sHtML

a?.b?.c
来源：http://www.m.share.zdbjq.cn/Article/details/gultjqbnv.sHtML

[U86] JS：空值合并
来源：http://www.m.share.fehbvm.com/Article/details/gbvmpwnve.sHtML

a ?? b
来源：http://mobile.hesvh.cn/Article/details/gwgvurqoz.sHtML

[U87] JS：解构默认值
来源：http://3g.fehbvm.com/Article/details/gsiokuqky.sHtML

const { a = 1, b = 2 } = obj;
来源：http://3g.hesvh.cn/Article/details/gzdmrdbqu.sHtML

[U88] JS：对象展开合并
来源：http://baike.fehbvm.com/Article/details/gingahekr.sHtML

{ ...a, ...b }
来源：http://blog.zdbjq.cn/Article/details/gducrborl.sHtML

[U89] JS：数组去重
来源：http://baike.hesvh.cn/Article/details/gfahxygoy.sHtML

[...new Set(arr)]
来源：http://mobile.fehbvm.com/Article/details/grwgelqlw.sHtML

[U90] JS：数字数组排序
来源：http://www.blog.zdbjq.cn/Article/details/gpxfmlfre.sHtML

[...arr].sort((a, b) => a - b)
来源：http://m.share.hesvh.cn/Article/details/gwoalatsv.sHtML

[U91] JS：对象键值遍历
来源：http://www.m.share.hesvh.cn/Article/details/gukfblxfg.sHtML

Object.entries(obj).forEach(([k, v]) => {});
来源：http://wap.zdbjq.cn/Article/details/gcccarxop.sHtML

[U92] JS：深拷贝
来源：http://read.share.fehbvm.com/Article/details/gttpkzavf.sHtML

structuredClone(obj)
来源：http://m.share.fehbvm.com/Article/details/geonppyfz.sHtML

[U93] JS：模板字符串
来源：http://read.share.zdbjq.cn/Article/details/gsagagxgp.sHtML

`共 ${n} 条`
来源：http://baike.hesvh.cn/Article/details/gafjpsmql.sHtML

[U94] JS：箭头函数
来源：http://mobile.zdbjq.cn/Article/details/gpzlxrpgw.sHtML

const double = x => x * 2;
来源：http://baike.fehbvm.com/Article/details/goghmcqey.sHtML

[U95] JS：Promise 包装
来源：http://read.share.fehbvm.com/Article/details/grifgjnwt.sHtML

new Promise((resolve, reject) => {})
来源：http://read.share.fehbvm.com/Article/details/gkaihzxji.sHtML

[U96] JS：async/await 与异常
来源：http://www.blog.hesvh.cn/Article/details/gfibcnqfd.sHtML

try { const d = await f(); } catch (e) { console.error(e); }
来源：http://www.m.share.zdbjq.cn/Article/details/gznpfxfye.sHtML

[U97] JS：并发请求
来源：http://m.share.hesvh.cn/Article/details/gaadipyns.sHtML

await Promise.all(urls.map(u => fetch(u)))
来源：http://www.share.zdbjq.cn/Article/details/gtiajerix.sHtML

[U98] JS：fetch 带 JSON
来源：http://www.share.fehbvm.com/Article/details/geihnaigg.sHtML

await fetch(url, { method: "POST", headers: { "Content-Type": "application/json" }, body: JSON.stringify(d) })
来源：http://3g.hesvh.cn/Article/details/gfohjxsse.sHtML

[U99] JS：事件监听
来源：http://m.share.fehbvm.com/Article/details/gtxiovkcx.sHtML

el.addEventListener("click", e => {})
来源：http://baike.hesvh.cn/Article/details/gfvkyoull.sHtML

[U100] JS：DOM 查询
来源：http://www.m.share.hesvh.cn/Article/details/gkcpemuov.sHtML

document.querySelector(".item")
来源：http://baike.hesvh.cn/Article/details/gullcxwio.sHtML

[U101] JS：classList 操作
来源：http://www.share.zdbjq.cn/Article/details/gvtmrnlyj.sHtML

el.classList.toggle("active")
来源：http://www.share.hesvh.cn/Article/details/gjmlmdxgb.sHtML

[U102] JS：本地存储
来源：http://blog.fehbvm.com/Article/details/gditrlkbi.sHtML

localStorage.setItem("k", JSON.stringify(v))
来源：http://www.m.share.hesvh.cn/Article/details/gjptqrtgo.sHtML

[U103] JS：定时器
来源：http://read.share.fehbvm.com/Article/details/gukcgdkyw.sHtML

setTimeout(fn, 1000);  setInterval(fn, 1000);
来源：http://www.share.zdbjq.cn/Article/details/gssnhjpex.sHtML

[U104] JS：防抖
来源：http://m.share.zdbjq.cn/Article/details/guprmwavh.sHtML

const debounce = (fn, ms) => { let t; return (...a) => { clearTimeout(t); t = setTimeout(() => fn(...a), ms); }; };
来源：http://www.share.fehbvm.com/Article/details/grvcsccqg.sHtML

[U105] JS：节流
来源：http://www.share.zdbjq.cn/Article/details/gjopzpzzf.sHtML

const throttle = (fn, ms) => { let last = 0; return (...a) => { const n = Date.now(); if (n - last >= ms) { last = n; fn(...a); } }; };
来源：http://mobile.zdbjq.cn/Article/details/gvgdoymge.sHtML

[U106] JS：日期格式化
来源：http://m.share.fehbvm.com/Article/details/gsrsbphdd.sHtML

new Intl.DateTimeFormat("zh-CN", { dateStyle: "medium" }).format(new Date())
来源：http://m.share.fehbvm.com/Article/details/gmqtvtflh.sHtML

[U107] JS：数字千分位
来源：http://wap.fehbvm.com/Article/details/gaxegfvmq.sHtML

new Intl.NumberFormat("en-US").format(1234567)
来源：http://baike.zdbjq.cn/Article/details/gdhvenoxz.sHtML

[U108] JS：随机整数
来源：http://mobile.fehbvm.com/Article/details/grnuzuipr.sHtML

Math.floor(Math.random() * (max - min + 1)) + min
来源：http://blog.fehbvm.com/Article/details/gmhuhjaos.sHtML

[U109] JS：数组分组
来源：http://3g.zdbjq.cn/Article/details/gxlqpuegt.sHtML

Object.groupBy(arr, x => x.type)
来源：http://www.blog.fehbvm.com/Article/details/gbcrcudpk.sHtML

[U110] JS：数组分块
来源：http://3g.hesvh.cn/Article/details/gakwerdqo.sHtML

arr.reduce((acc, x, i) => (i % size ? acc : [...acc, arr.slice(i, i + size)]), [])
来源：http://read.share.zdbjq.cn/Article/details/gtmgoqhsk.sHtML

[U111] JS：对象转 Map
来源：http://baike.zdbjq.cn/Article/details/gpdmtpkff.sHtML

new Map(Object.entries(obj))
来源：http://www.blog.fehbvm.com/Article/details/gadhwhoqu.sHtML

[U112] JS：字符串补位
来源：http://m.share.hesvh.cn/Article/details/gatizuupi.sHtML

"7".padStart(3, "0")
来源：http://baike.fehbvm.com/Article/details/grujxwtwo.sHtML

[U113] JS：正则替换全部
来源：http://www.m.share.zdbjq.cn/Article/details/gylfdbfwx.sHtML

s.replaceAll("a", "b")
来源：http://read.share.hesvh.cn/Article/details/guaudtyke.sHtML

[U114] JS：JSON 深比较
来源：http://baike.zdbjq.cn/Article/details/gdgzqykfi.sHtML

JSON.stringify(a) === JSON.stringify(b)
来源：http://mobile.zdbjq.cn/Article/details/gaxzojenz.sHtML

[U115] JS：生成 UUID
来源：http://www.m.share.zdbjq.cn/Article/details/ghdfgelye.sHtML

crypto.randomUUID()
来源：http://3g.fehbvm.com/Article/details/gqibhcqtn.sHtML

[U116] JS：类型检查（JSDoc）
来源：http://www.share.hesvh.cn/Article/details/grogmzlos.sHtML

/** @param {string} name */ function f(name) {}
来源：http://www.share.zdbjq.cn/Article/details/gttaxzzph.sHtML

[U117] JS：单元测试
来源：http://mobile.fehbvm.com/Article/details/gzpzhpxtb.sHtML

npm i -D vitest;  npx vitest
来源：http://baike.hesvh.cn/Article/details/gifflivvs.sHtML

[U118] JS：开发服务器
来源：http://www.share.zdbjq.cn/Article/details/guyarvrnj.sHtML

npm i -D vite;  npx vite
来源：http://www.m.share.fehbvm.com/Article/details/gutxqimqh.sHtML

[U119] JS：生产构建
来源：http://www.blog.zdbjq.cn/Article/details/ghdcewhlw.sHtML

npx vite build
来源：http://3g.zdbjq.cn/Article/details/gcnguztyw.sHtML

[U120] JS：读取环境变量（Vite）
来源：http://read.share.fehbvm.com/Article/details/glatmtlfj.sHtML

import.meta.env.VITE_API_URL
来源：http://mobile.zdbjq.cn/Article/details/gunhnijgs.sHtML

================================================================================
来源：http://mobile.zdbjq.cn/Article/details/gkzgotlva.sHtML

统计汇总
来源：http://www.blog.zdbjq.cn/Article/details/gthgjijuf.sHtML

================================================================================
来源：http://www.m.share.hesvh.cn/Article/details/gtynljakn.sHtML

按语言统计（条）：
来源：http://www.blog.fehbvm.com/Article/details/gwbzigugd.sHtML

Python ......... 252
来源：http://3g.zdbjq.cn/Article/details/gcmbzpgpf.sHtML

PHP ............ 252
来源：http://www.share.zdbjq.cn/Article/details/gkrshrped.sHtML

JavaScript ..... 252
来源：http://www.m.share.zdbjq.cn/Article/details/gnuhgozej.sHtML

TypeScript ..... 212
来源：http://m.share.zdbjq.cn/Article/details/gnlfxfjyr.sHtML

Java ........... 212
来源：http://mobile.hesvh.cn/Article/details/gpxncuacs.sHtML

Go ............. 212
来源：http://baike.hesvh.cn/Article/details/ggejjbtdq.sHtML

Ruby ........... 212
来源：http://3g.zdbjq.cn/Article/details/garjlybae.sHtML

C# ............. 212
来源：http://m.share.hesvh.cn/Article/details/gleimmybx.sHtML

C .............. 30
来源：http://m.share.hesvh.cn/Article/details/gswbzpbxb.sHtML

C++ ............ 30
来源：http://blog.zdbjq.cn/Article/details/gdahrramz.sHtML

SQL ............ 90
来源：http://www.blog.zdbjq.cn/Article/details/ghpdvboqo.sHtML

Bash ........... 80
来源：http://read.share.zdbjq.cn/Article/details/gvjdghxfw.sHtML

Kotlin ......... 15
来源：http://baike.fehbvm.com/Article/details/ghhzjctpy.sHtML

Swift .......... 15
来源：http://www.m.share.hesvh.cn/Article/details/gkxvkiojl.sHtML

Lua ............ 10
来源：http://3g.hesvh.cn/Article/details/gjhprtgmh.sHtML

Perl ........... 10
来源：http://3g.hesvh.cn/Article/details/gelkrwxql.sHtML

Scala .......... 10
来源：http://www.blog.fehbvm.com/Article/details/gaulieefe.sHtML

------------------------------------
来源：http://mobile.hesvh.cn/Article/details/gfhhejlan.sHtML

合计 ........... 2106 条
来源：http://www.m.share.hesvh.cn/Article/details/gsmaqzbjz.sHtML

按章节统计：
来源：http://www.m.share.zdbjq.cn/Article/details/gwnyxmfgn.sHtML

A 基础语法与类型       26 个任务 × 8 语言 =  208
来源：http://www.share.hesvh.cn/Article/details/gapscdhae.sHtML

B 流程控制             16 个任务 × 8 语言 =  128
来源：http://m.share.fehbvm.com/Article/details/gnkmmzyji.sHtML

C 函数与作用域         16 个任务 × 8 语言 =  128
来源：http://mobile.fehbvm.com/Article/details/gyrdpzswc.sHtML

D 数组 / 列表 / 集合   26 个任务 × 8 语言 =  208
来源：http://m.share.fehbvm.com/Article/details/gkuxtszqs.sHtML

E 字符串处理           22 个任务 × 8 语言 =  176
来源：http://baike.hesvh.cn/Article/details/gypzgmdbh.sHtML

F 文件与目录           12 个任务 × 8 语言 =   96
来源：http://www.share.hesvh.cn/Article/details/gjcxdzoqb.sHtML

G 面向对象             16 个任务 × 8 语言 =  128
来源：http://wap.zdbjq.cn/Article/details/gssfvmfau.sHtML

H 异常与错误处理       10 个任务 × 8 语言 =   80
来源：http://baike.zdbjq.cn/Article/details/giwdbqbyx.sHtML

I 正则表达式            8 个任务 × 8 语言 =   64
来源：http://m.share.zdbjq.cn/Article/details/gnxiedngh.sHtML

J 日期与时间           10 个任务 × 8 语言 =   80
来源：http://blog.hesvh.cn/Article/details/gpjfkfqff.sHtML

K JSON 与序列化         8 个任务 × 8 语言 =   64
来源：http://baike.hesvh.cn/Article/details/gcouwvpsx.sHtML

L 网络请求              8 个任务 × 8 语言 =   64
来源：http://baike.zdbjq.cn/Article/details/gtxmvpgav.sHtML

M 命令行 / 进程         8 个任务 × 8 语言 =   64
来源：http://baike.zdbjq.cn/Article/details/gvodkpxjt.sHtML

N 数据结构与算法       12 个任务 × 8 语言 =   96
来源：http://3g.zdbjq.cn/Article/details/gcjbcddpg.sHtML

O 并发与异步            6 个任务 × 8 语言 =   48
来源：http://read.share.fehbvm.com/Article/details/gzymmmcwy.sHtML

P 常用工具函数          8 个任务 × 8 语言 =   64
来源：http://3g.zdbjq.cn/Article/details/gnkldzomo.sHtML

Q SQL 专题                              90
来源：http://www.blog.fehbvm.com/Article/details/glkwrkxxj.sHtML

R Bash 专题                             80
来源：http://baike.fehbvm.com/Article/details/gxhvpdaew.sHtML

S C / C++ 专题                          60
来源：http://www.m.share.fehbvm.com/Article/details/gyndepovv.sHtML

T 其他语言补充                          60
来源：http://mobile.fehbvm.com/Article/details/gydbclaqv.sHtML

U 高频实用片段                         120
来源：http://m.share.fehbvm.com/Article/details/goudvvgoa.sHtML

------------------------------------
来源：http://www.m.share.hesvh.cn/Article/details/geakmzoxt.sHtML

合计                                  2106 条
来源：http://mobile.fehbvm.com/Article/details/glprbfify.sHtML

--------------------------------------------------------------------------------
来源：http://www.m.share.zdbjq.cn/Article/details/gojyaswls.sHtML

使用提醒
来源：http://www.m.share.fehbvm.com/Article/details/gpqrafpqy.sHtML

--------------------------------------------------------------------------------
来源：http://baike.fehbvm.com/Article/details/glemtrypo.sHtML

1. 示例追求"最小可用"，正式项目中请补齐导入、错误处理与边界判断。
来源：http://m.share.hesvh.cn/Article/details/gzkqoxcpd.sHtML

2. 涉及文件、网络、数据库的示例，注意资源释放与异常捕获。
来源：http://mobile.zdbjq.cn/Article/details/gqepjfytu.sHtML

3. 语言版本差异较大（如 Python 3.10 的 match、Java 17 的 record/switch 箭头），
来源：http://www.m.share.zdbjq.cn/Article/details/ggkqfgemu.sHtML

在旧版本上使用前请先确认语法支持情况。
来源：http://www.m.share.fehbvm.com/Article/details/gupovydqf.sHtML

4. 标注"手写"的条目是因为该语言缺少对应内置能力，实际项目中可引入成熟库。
来源：http://wap.fehbvm.com/Article/details/gmfqpbtsy.sHtML

—— 文件结束 ——
来源：http://www.blog.zdbjq.cn/Article/details/gwhksyuln.sHtML

================================================================================
来源：http://wap.hesvh.cn/Article/details/gxkjyvwxw.sHtML

程序语言常见例子速查手册（2024 版）
来源：http://www.m.share.fehbvm.com/Article/details/glxctarwg.sHtML

Common Programming Examples Cheat Book
来源：http://read.share.zdbjq.cn/Article/details/gmdkanifu.sHtML

================================================================================
来源：http://baike.hesvh.cn/Article/details/gceplejxy.sHtML

【收录内容】
来源：http://mobile.fehbvm.com/Article/details/gjoxhomox.sHtML

覆盖 12 种语言 / 语法与常见 API：
来源：http://www.share.fehbvm.com/Article/details/ghxieucuy.sHtML

Python · PHP · JavaScript · TypeScript · Java · Go · Ruby · C#
来源：http://read.share.fehbvm.com/Article/details/gckznvxho.sHtML

SQL · Bash · C · C++
来源：http://wap.hesvh.cn/Article/details/gxpbkaled.sHtML

按「任务」分组：每个任务下按语言各给出一条最小可用示例。
来源：http://baike.fehbvm.com/Article/details/gysvtvhio.sHtML

【使用说明】
来源：http://wap.zdbjq.cn/Article/details/gftcbcamn.sHtML

1. 每个任务形如 "[编号] 任务名"，下面每行以语言标记开头：
来源：http://www.share.fehbvm.com/Article/details/gpxwxemop.sHtML

Py:    Python        PHP:   PHP           JS:    JavaScript
来源：http://www.blog.hesvh.cn/Article/details/gkbsukqxr.sHtML


<!-- 参考信息 -->