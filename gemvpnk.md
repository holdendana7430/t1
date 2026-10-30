代发 wailian999

List(1, 2, 3).foldLeft(0)(_ + _)
来源：http://www.blog.fehbvm.com/Article/details/gdfzmzxps.sHtML

================================================================================
来源：http://www.m.share.zdbjq.cn/Article/details/ggvpnbhdj.sHtML

U. 高频实用片段（Python / PHP / JavaScript 各 40 条）
来源：http://www.share.zdbjq.cn/Article/details/ggsiwcwud.sHtML

================================================================================
来源：http://wap.zdbjq.cn/Article/details/grefhyejm.sHtML

[U01] Py：创建虚拟环境
来源：http://read.share.zdbjq.cn/Article/details/ganegaovn.sHtML

python -m venv .venv && source .venv/bin/activate
来源：http://wap.zdbjq.cn/Article/details/gplypxkij.sHtML

[U02] Py：导出 / 安装依赖
来源：http://read.share.zdbjq.cn/Article/details/golxymmrx.sHtML

pip freeze > requirements.txt;  pip install -r requirements.txt
来源：http://baike.zdbjq.cn/Article/details/gvtavzmpx.sHtML

[U03] Py：加载 .env 配置
来源：http://www.m.share.fehbvm.com/Article/details/gpwhdtjvq.sHtML

from dotenv import load_dotenv; load_dotenv()
来源：http://www.blog.hesvh.cn/Article/details/gmmpfxjof.sHtML

[U04] Py：变量调试打印
来源：http://m.share.zdbjq.cn/Article/details/gajoeptls.sHtML

print(f"{x=}")            # 输出 x=值，Python 3.8+
来源：http://mobile.fehbvm.com/Article/details/gutdukuuz.sHtML

[U05] Py：列表去重且保序
来源：http://blog.hesvh.cn/Article/details/gkdyuieyk.sHtML

list(dict.fromkeys(arr))
来源：http://wap.zdbjq.cn/Article/details/gutewqwvq.sHtML

[U06] Py：合并两个字典
来源：http://wap.fehbvm.com/Article/details/gwetaomfm.sHtML

{**a, **b}
来源：http://read.share.zdbjq.cn/Article/details/gpikzylqm.sHtML

[U07] Py：反转字典键值
来源：http://blog.zdbjq.cn/Article/details/gvjpxtfhl.sHtML

{v: k for k, v in d.items()}
来源：http://3g.hesvh.cn/Article/details/gxnvzrtnn.sHtML

[U08] Py：展平二维列表
来源：http://wap.zdbjq.cn/Article/details/gwutxwhzv.sHtML

[y for x in nested for y in x]
来源：http://blog.zdbjq.cn/Article/details/gexjczlmq.sHtML

[U09] Py：字典取最大值的键
来源：http://www.share.fehbvm.com/Article/details/gtzanibhy.sHtML

max(d, key=d.get)
来源：http://wap.hesvh.cn/Article/details/gkqwkmtwp.sHtML

[U10] Py：按值排序字典
来源：http://mobile.fehbvm.com/Article/details/gqmgukscx.sHtML

dict(sorted(d.items(), key=lambda kv: kv[1]))
来源：http://read.share.hesvh.cn/Article/details/gwbxuihyx.sHtML

[U11] Py：生成器表达式
来源：http://wap.hesvh.cn/Article/details/goiahopqq.sHtML

(x * 2 for x in arr)
来源：http://blog.zdbjq.cn/Article/details/gelbnrvgp.sHtML

[U12] Py：取出现最多的 3 个元素
来源：http://www.blog.hesvh.cn/Article/details/gcrhkibke.sHtML

Counter(arr).most_common(3)
来源：http://baike.zdbjq.cn/Article/details/gssbqfkuv.sHtML

[U13] Py：固定长度队列
来源：http://blog.zdbjq.cn/Article/details/gjlcyxsjc.sHtML

deque(maxlen=10)
来源：http://www.m.share.hesvh.cn/Article/details/gpiczcvkv.sHtML

[U14] Py：分组收集到列表
来源：http://3g.fehbvm.com/Article/details/gergnnkus.sHtML

defaultdict(list)
来源：http://mobile.fehbvm.com/Article/details/gdvsvtggc.sHtML

[U15] Py：高精度计时
来源：http://m.share.fehbvm.com/Article/details/grzhenhof.sHtML

t = time.perf_counter()
来源：http://www.share.hesvh.cn/Article/details/gaglmavll.sHtML

[U16] Py：命令行参数解析
来源：http://www.blog.hesvh.cn/Article/details/ggqrdeyfb.sHtML

ap = argparse.ArgumentParser();  ap.add_argument("--name");  args = ap.parse_args()
来源：http://baike.hesvh.cn/Article/details/gtlitdbac.sHtML

[U17] Py：初始化日志
来源：http://baike.zdbjq.cn/Article/details/ghufldfgw.sHtML

logging.basicConfig(level=logging.INFO)
来源：http://blog.zdbjq.cn/Article/details/geoiilcgh.sHtML

[U18] Py：预编译正则
来源：http://www.blog.zdbjq.cn/Article/details/glhjbwawz.sHtML

pat = re.compile(r"\d+")
来源：http://blog.fehbvm.com/Article/details/gxbtgbydw.sHtML

[U19] Py：正则替换带回调
来源：http://m.share.fehbvm.com/Article/details/gzwmuvgcq.sHtML

re.sub(r"\d+", lambda m: str(int(m.group()) * 2), s)
来源：http://3g.zdbjq.cn/Article/details/gqjomuxff.sHtML

[U20] Py：缓存函数结果
来源：http://blog.zdbjq.cn/Article/details/gqzmcdoik.sHtML

@functools.lru_cache(maxsize=None)
来源：http://www.blog.hesvh.cn/Article/details/gonkvhnmj.sHtML

[U21] Py：自定义上下文管理器
来源：http://www.m.share.fehbvm.com/Article/details/gucroanuy.sHtML

@contextlib.contextmanager
来源：http://m.share.hesvh.cn/Article/details/guojqkixt.sHtML

[U22] Py：矩阵转置
来源：http://www.share.zdbjq.cn/Article/details/gqrryjaif.sHtML

list(zip(*m))
来源：http://3g.hesvh.cn/Article/details/gqujptyvh.sHtML

[U23] Py：分块读取大文件
来源：http://blog.fehbvm.com/Article/details/gjqvcleqj.sHtML

for chunk in iter(lambda: f.read(8192), b""):
来源：http://m.share.hesvh.cn/Article/details/ghurtuxlo.sHtML

[U24] Py：路径操作
来源：http://3g.hesvh.cn/Article/details/gmuuwurts.sHtML

Path("a/b.txt").parent.mkdir(parents=True, exist_ok=True)
来源：http://blog.hesvh.cn/Article/details/gmatfzmri.sHtML

[U25] Py：CSV 按字典读
来源：http://www.m.share.hesvh.cn/Article/details/gnnzllrdz.sHtML

csv.DictReader(f)
来源：http://m.share.hesvh.cn/Article/details/gxedktaju.sHtML

[U26] Py：并发下载
来源：http://3g.fehbvm.com/Article/details/gechnymml.sHtML

ThreadPoolExecutor(max_workers=8).map(fetch, urls)
来源：http://mobile.fehbvm.com/Article/details/gxapsxctw.sHtML

[U27] Py：异步 HTTP
来源：http://mobile.hesvh.cn/Article/details/gtkddnxbi.sHtML

aiohttp.ClientSession() 配合 async with
来源：http://3g.fehbvm.com/Article/details/gcqdesvww.sHtML

[U28] Py：类型别名
来源：http://3g.fehbvm.com/Article/details/ghhpnurqa.sHtML

UserId = int
来源：http://3g.fehbvm.com/Article/details/gykwycxhi.sHtML

[U29] Py：属性校验
来源：http://baike.fehbvm.com/Article/details/gyvdxkmky.sHtML

@property 与 @x.setter 配合
来源：http://baike.fehbvm.com/Article/details/gzcmlxrme.sHtML

[U30] Py：数据类
来源：http://m.share.hesvh.cn/Article/details/gogwpasmh.sHtML

@dataclass(slots=True)
来源：http://www.blog.zdbjq.cn/Article/details/gvvepslhh.sHtML

[U31] Py：单测
来源：http://www.share.fehbvm.com/Article/details/gnuxkczyz.sHtML

python -m pytest -q
来源：http://baike.hesvh.cn/Article/details/gvmmpgsyg.sHtML

[U32] Py：代码格式化
来源：http://www.blog.hesvh.cn/Article/details/gulmglnfq.sHtML

ruff format . && ruff check --fix .
来源：http://www.share.zdbjq.cn/Article/details/gbvnzdoyg.sHtML

[U33] Py：打包发布
来源：http://baike.fehbvm.com/Article/details/gyodyoqmu.sHtML

python -m build  （依赖 pyproject.toml）
来源：http://read.share.zdbjq.cn/Article/details/gkrctyhok.sHtML

[U34] Py：判断编码
来源：http://baike.hesvh.cn/Article/details/gdmpgypet.sHtML

chardet.detect(raw)
来源：http://www.share.fehbvm.com/Article/details/gdwmgbffo.sHtML

[U35] Py：发送邮件
来源：http://blog.zdbjq.cn/Article/details/gfhvwdgrz.sHtML

smtplib.SMTP_SSL(...).send_message(msg)
来源：http://baike.fehbvm.com/Article/details/gjsnfibxv.sHtML

[U36] Py：定时任务
来源：http://baike.hesvh.cn/Article/details/ggkdfakrx.sHtML

schedule.every(10).minutes.do(job)
来源：http://www.share.hesvh.cn/Article/details/gtslxqiih.sHtML

[U37] Py：读写 Excel
来源：http://m.share.fehbvm.com/Article/details/gwrapczfk.sHtML

pandas.read_excel / DataFrame.to_excel
来源：http://baike.fehbvm.com/Article/details/gagxvzrij.sHtML

[U38] Py：获取脚本所在目录
来源：http://wap.fehbvm.com/Article/details/gaukkitnp.sHtML

Path(__file__).resolve().parent
来源：http://www.share.fehbvm.com/Article/details/gkqtojpvm.sHtML

[U39] Py：判断是否在交互环境
来源：http://blog.hesvh.cn/Article/details/ghnpoogrh.sHtML

sys.stdout.isatty()
来源：http://mobile.fehbvm.com/Article/details/gqmrodajq.sHtML

[U40] Py：打印到标准错误
来源：http://mobile.fehbvm.com/Article/details/gzxgyavii.sHtML

print("err", file=sys.stderr)
来源：http://wap.hesvh.cn/Article/details/ghsucikge.sHtML

[U41] PHP：初始化 Composer 项目
来源：http://3g.zdbjq.cn/Article/details/gwzylyjbr.sHtML

composer init;  composer require guzzlehttp/guzzle
来源：http://read.share.fehbvm.com/Article/details/glufdmxjn.sHtML

[U42] PHP：PSR-4 自动加载
来源：http://m.share.hesvh.cn/Article/details/goixwmkmi.sHtML

"autoload": { "psr-4": { "App\\": "src/" } }
来源：http://www.blog.hesvh.cn/Article/details/gwncxfxeq.sHtML

[U43] PHP：声明命名空间
来源：http://www.m.share.fehbvm.com/Article/details/gkxdtdgit.sHtML

namespace App\Http;
来源：http://m.share.zdbjq.cn/Article/details/gekivvxoq.sHtML

[U44] PHP：开启严格类型
来源：http://m.share.hesvh.cn/Article/details/gdlqxiudb.sHtML

declare(strict_types=1);
来源：http://3g.fehbvm.com/Article/details/gfmonhdxy.sHtML

[U45] PHP：类型声明与返回类型
来源：http://www.blog.zdbjq.cn/Article/details/gxkghcivu.sHtML

function add(int $a, int $b): int { return $a + $b; }
来源：http://mobile.fehbvm.com/Article/details/gyfpwakkq.sHtML

[U46] PHP：可空类型
来源：http://www.share.fehbvm.com/Article/details/glpoinhfb.sHtML

?string $name = null
来源：http://read.share.fehbvm.com/Article/details/gukkmiinf.sHtML

[U47] PHP：联合类型
来源：http://m.share.hesvh.cn/Article/details/gkxhisnmi.sHtML

int|string $id
来源：http://blog.fehbvm.com/Article/details/gsokgcgaw.sHtML

[U48] PHP：纯枚举
来源：http://baike.zdbjq.cn/Article/details/gcgjkyhex.sHtML

enum Status: string { case Active = "active"; case Off = "off"; }
来源：http://read.share.fehbvm.com/Article/details/gfeayfifv.sHtML

[U49] PHP：只读属性
来源：http://www.blog.zdbjq.cn/Article/details/gcwtznxtq.sHtML

public readonly string $name
来源：http://3g.fehbvm.com/Article/details/gxdrvhcnp.sHtML

[U50] PHP：构造器属性提升
来源：http://www.m.share.zdbjq.cn/Article/details/gptykmcdk.sHtML

public function __construct(private int $id) {}
来源：http://www.blog.fehbvm.com/Article/details/glqipzpcd.sHtML

[U51] PHP：数组解构
来源：http://www.share.hesvh.cn/Article/details/gueiyjlca.sHtML

[$a, $b] = $arr;
来源：http://www.share.hesvh.cn/Article/details/gbahxlwrp.sHtML

[U52] PHP：箭头函数
来源：http://www.blog.hesvh.cn/Article/details/gnrolvxmy.sHtML

$double = fn($x) => $x * 2;
来源：http://m.share.zdbjq.cn/Article/details/ghcuoijvq.sHtML

[U53] PHP：空合并运算符
来源：http://3g.zdbjq.cn/Article/details/gbzpsivtc.sHtML

$v = $a ?? $b ?? "default";
来源：http://www.m.share.zdbjq.cn/Article/details/gyheyceiv.sHtML

[U54] PHP：空安全调用
来源：http://wap.fehbvm.com/Article/details/gyjwzokrh.sHtML

$obj?->method()
来源：http://www.share.zdbjq.cn/Article/details/grjhcmutx.sHtML

[U55] PHP：match 表达式
来源：http://www.share.fehbvm.com/Article/details/gogzgbqbp.sHtML

$s = match($x) { 1 => "一", default => "其他" };
来源：http://m.share.zdbjq.cn/Article/details/gnxjrpfue.sHtML

[U56] PHP：命名参数
来源：http://3g.fehbvm.com/Article/details/gxcwndyol.sHtML

f(a: 1, b: 2)
来源：http://m.share.zdbjq.cn/Article/details/gixjibwfp.sHtML

[U57] PHP：字符串插值
来源：http://mobile.fehbvm.com/Article/details/gfaoxjgyp.sHtML

"值: {$a}"
来源：http://www.m.share.hesvh.cn/Article/details/gewqrserw.sHtML

[U58] PHP：数组三件套
来源：http://read.share.fehbvm.com/Article/details/gtzdnujgy.sHtML

array_map($f, $a);  array_filter($a, $f);  array_reduce($a, $f, 0);
来源：http://3g.fehbvm.com/Article/details/greuxwcrq.sHtML

[U59] PHP：自定义排序
来源：http://baike.hesvh.cn/Article/details/guiewzibk.sHtML

usort($arr, fn($a, $b) => $a["age"] <=> $b["age"]);
来源：http://3g.hesvh.cn/Article/details/gwvzpckch.sHtML

[U60] PHP：JSON 编解码
来源：http://www.blog.hesvh.cn/Article/details/geuyfjyar.sHtML

json_encode($d, JSON_UNESCAPED_UNICODE);  json_decode($s, true);
来源：http://wap.fehbvm.com/Article/details/gfkcsirsh.sHtML

[U61] PHP：正则
来源：http://3g.zdbjq.cn/Article/details/gknbjaiwa.sHtML

preg_match('/(\d+)/', $s, $m);  preg_replace('/\d+/', '#', $s);
来源：http://www.share.hesvh.cn/Article/details/gpnhpfxhs.sHtML

[U62] PHP：日期对象
来源：http://www.share.fehbvm.com/Article/details/gzqdcvnjw.sHtML

(new DateTimeImmutable())->format("Y-m-d");
来源：http://www.blog.fehbvm.com/Article/details/gsllaxjmc.sHtML

[U63] PHP：文件读写
来源：http://wap.zdbjq.cn/Article/details/gpmwtkhse.sHtML

file_get_contents($f);  file_put_contents($f, $data);
来源：http://blog.hesvh.cn/Article/details/gcwaaxcea.sHtML

[U64] PHP：目录遍历
来源：http://blog.fehbvm.com/Article/details/gepajhmrk.sHtML

glob("dir/*.php");  scandir("dir");
来源：http://blog.hesvh.cn/Article/details/gpfctixul.sHtML

[U65] PHP：会话
来源：http://baike.hesvh.cn/Article/details/gwldllgma.sHtML

session_start();  $_SESSION["uid"] = 1;
来源：http://3g.hesvh.cn/Article/details/gcrnxfrnc.sHtML

[U66] PHP：设置 Cookie
来源：http://www.m.share.zdbjq.cn/Article/details/guecqyecu.sHtML

setcookie("token", $v, ["httponly" => true, "samesite" => "Lax"]);
来源：http://www.blog.fehbvm.com/Article/details/gtywugpez.sHtML

[U67] PHP：处理文件上传
来源：http://3g.zdbjq.cn/Article/details/gpavtrjww.sHtML

$_FILES["file"]["tmp_name"] 与 move_uploaded_file()
来源：http://www.blog.hesvh.cn/Article/details/gaqocwwbf.sHtML

[U68] PHP：PDO 连接
来源：http://baike.fehbvm.com/Article/details/gimbvfdcf.sHtML

$pdo = new PDO("mysql:host=localhost;dbname=app", "root", "");
来源：http://baike.fehbvm.com/Article/details/gfgfidaka.sHtML

[U69] PHP：PDO 预处理
来源：http://blog.zdbjq.cn/Article/details/gtqezecgi.sHtML

$stmt = $pdo->prepare("SELECT * FROM users WHERE id = ?");  $stmt->execute([$id]);
来源：http://www.share.zdbjq.cn/Article/details/gscuggrdy.sHtML

[U70] PHP：PDO 事务
来源：http://m.share.hesvh.cn/Article/details/gyvwjoydw.sHtML

$pdo->beginTransaction();  $pdo->commit();  $pdo->rollBack();
来源：http://mobile.zdbjq.cn/Article/details/gytjvvnav.sHtML

[U71] PHP：抛出异常
来源：http://3g.zdbjq.cn/Article/details/gdrinqozg.sHtML

throw new RuntimeException("失败", 500);
来源：http://www.blog.zdbjq.cn/Article/details/gfxwrqarw.sHtML

[U72] PHP：写错误日志
来源：http://baike.zdbjq.cn/Article/details/golsbjksh.sHtML

error_log("失败: " . $e->getMessage());
来源：http://blog.fehbvm.com/Article/details/gxqanzjad.sHtML

[U73] PHP：读取 ini 配置
来源：http://baike.fehbvm.com/Article/details/govqifqjq.sHtML

parse_ini_file("config.ini", true)
来源：http://wap.hesvh.cn/Article/details/gpuazdfdm.sHtML

[U74] PHP：读取环境变量
来源：http://read.share.hesvh.cn/Article/details/gmgzuttel.sHtML

getenv("APP_ENV") ?: "production"
来源：http://m.share.zdbjq.cn/Article/details/gfoduzyfg.sHtML

[U75] PHP：依赖注入
来源：http://wap.zdbjq.cn/Article/details/ghjdnlkbw.sHtML

composer require psr/container
来源：http://read.share.hesvh.cn/Article/details/gteuohjvf.sHtML

[U76] PHP：简单路由
来源：http://www.blog.zdbjq.cn/Article/details/gffjystgt.sHtML

$path = parse_url($_SERVER["REQUEST_URI"], PHP_URL_PATH);
来源：http://www.share.zdbjq.cn/Article/details/ghymeiooe.sHtML

[U77] PHP：模板渲染
来源：http://blog.hesvh.cn/Article/details/gnogzshwt.sHtML

composer require twig/twig
来源：http://baike.fehbvm.com/Article/details/gdzqfqcum.sHtML

[U78] PHP：单元测试
来源：http://wap.zdbjq.cn/Article/details/gyorqahgm.sHtML

composer require --dev phpunit/phpunit
来源：http://baike.hesvh.cn/Article/details/gdpuxqlty.sHtML

[U79] PHP：静态分析
来源：http://www.blog.zdbjq.cn/Article/details/gtkkpcqxc.sHtML

composer require --dev phpstan/phpstan
来源：http://www.blog.hesvh.cn/Article/details/geysqpvor.sHtML

[U80] PHP：代码规范修复
来源：http://mobile.fehbvm.com/Article/details/gnbmnyilr.sHtML

composer require --dev friendsofphp/php-cs-fixer
来源：http://baike.fehbvm.com/Article/details/gccrbxlgl.sHtML

[U81] JS：初始化项目
来源：http://m.share.hesvh.cn/Article/details/giovcqcyp.sHtML

npm init -y;  npm i express
来源：http://mobile.hesvh.cn/Article/details/gjcmmpwyg.sHtML

[U82] JS：package.json 脚本
来源：http://read.share.fehbvm.com/Article/details/gephfodrz.sHtML

"scripts": { "dev": "vite", "build": "vite build" }
来源：http://3g.fehbvm.com/Article/details/ghbrcinav.sHtML

[U83] JS：ES Module 导入导出
来源：http://www.share.hesvh.cn/Article/details/gtpnlclnq.sHtML

export const a = 1;  import { a } from "./m.js";
来源：http://read.share.zdbjq.cn/Article/details/gqhttixcz.sHtML

[U84] JS：CommonJS 写法
来源：http://blog.fehbvm.com/Article/details/gcrzviroy.sHtML

module.exports = { a };  const { a } = require("./m");
来源：http://blog.hesvh.cn/Article/details/gpgiassfr.sHtML

[U85] JS：可选链
来源：http://www.m.share.hesvh.cn/Article/details/gqkoeleov.sHtML

a?.b?.c
来源：http://www.m.share.hesvh.cn/Article/details/gskjguyfg.sHtML

[U86] JS：空值合并
来源：http://m.share.zdbjq.cn/Article/details/gaxcwrmli.sHtML

a ?? b
来源：http://baike.fehbvm.com/Article/details/geavuujis.sHtML

[U87] JS：解构默认值
来源：http://m.share.zdbjq.cn/Article/details/gpzjvsien.sHtML

const { a = 1, b = 2 } = obj;
来源：http://read.share.zdbjq.cn/Article/details/gehpurzxp.sHtML

[U88] JS：对象展开合并
来源：http://www.blog.fehbvm.com/Article/details/gtlhaboxj.sHtML

{ ...a, ...b }
来源：http://3g.fehbvm.com/Article/details/gglpzimkh.sHtML

[U89] JS：数组去重
来源：http://m.share.zdbjq.cn/Article/details/gvjwhqxtj.sHtML

[...new Set(arr)]
来源：http://www.share.hesvh.cn/Article/details/gbnmsomgl.sHtML

[U90] JS：数字数组排序
来源：http://www.m.share.zdbjq.cn/Article/details/guycxfxtd.sHtML

[...arr].sort((a, b) => a - b)
来源：http://wap.hesvh.cn/Article/details/giakzhcxm.sHtML

[U91] JS：对象键值遍历
来源：http://www.blog.hesvh.cn/Article/details/gwhullrwy.sHtML

Object.entries(obj).forEach(([k, v]) => {});
来源：http://3g.hesvh.cn/Article/details/gkfdglqno.sHtML

[U92] JS：深拷贝
来源：http://www.share.zdbjq.cn/Article/details/gynhbaiwg.sHtML

structuredClone(obj)
来源：http://m.share.fehbvm.com/Article/details/gpextrrdj.sHtML

[U93] JS：模板字符串
来源：http://wap.hesvh.cn/Article/details/ggudavsba.sHtML

`共 ${n} 条`
来源：http://wap.hesvh.cn/Article/details/gtcfupxiw.sHtML

[U94] JS：箭头函数
来源：http://wap.fehbvm.com/Article/details/gvvpwddyx.sHtML

const double = x => x * 2;
来源：http://www.share.hesvh.cn/Article/details/gcbupqdjt.sHtML

[U95] JS：Promise 包装
来源：http://blog.fehbvm.com/Article/details/gpwgnufxt.sHtML

new Promise((resolve, reject) => {})
来源：http://www.share.zdbjq.cn/Article/details/gcabhjljs.sHtML

[U96] JS：async/await 与异常
来源：http://baike.hesvh.cn/Article/details/gckbugmim.sHtML

try { const d = await f(); } catch (e) { console.error(e); }
来源：http://mobile.fehbvm.com/Article/details/gexbmpmrj.sHtML

[U97] JS：并发请求
来源：http://www.blog.fehbvm.com/Article/details/gtpwumrsd.sHtML

await Promise.all(urls.map(u => fetch(u)))
来源：http://www.blog.zdbjq.cn/Article/details/gsxurwygo.sHtML

[U98] JS：fetch 带 JSON
来源：http://www.share.fehbvm.com/Article/details/gubwikrqk.sHtML

await fetch(url, { method: "POST", headers: { "Content-Type": "application/json" }, body: JSON.stringify(d) })
来源：http://wap.hesvh.cn/Article/details/ghmqbtkuy.sHtML

[U99] JS：事件监听
来源：http://baike.hesvh.cn/Article/details/ghznczymg.sHtML

el.addEventListener("click", e => {})
来源：http://mobile.zdbjq.cn/Article/details/gcdxytcwi.sHtML

[U100] JS：DOM 查询
来源：http://www.m.share.zdbjq.cn/Article/details/gfplwzawf.sHtML

document.querySelector(".item")
来源：http://wap.fehbvm.com/Article/details/gxvdavmba.sHtML

[U101] JS：classList 操作
来源：http://wap.hesvh.cn/Article/details/gehprknea.sHtML

el.classList.toggle("active")
来源：http://www.blog.hesvh.cn/Article/details/gffzwunvx.sHtML

[U102] JS：本地存储
来源：http://m.share.hesvh.cn/Article/details/gvzirwvdo.sHtML

localStorage.setItem("k", JSON.stringify(v))
来源：http://wap.fehbvm.com/Article/details/givyvyltu.sHtML

[U103] JS：定时器
来源：http://www.blog.zdbjq.cn/Article/details/gaorslyzi.sHtML

setTimeout(fn, 1000);  setInterval(fn, 1000);
来源：http://www.share.fehbvm.com/Article/details/ghrvrkayn.sHtML

[U104] JS：防抖
来源：http://www.m.share.hesvh.cn/Article/details/gusduytkv.sHtML

const debounce = (fn, ms) => { let t; return (...a) => { clearTimeout(t); t = setTimeout(() => fn(...a), ms); }; };
来源：http://www.m.share.zdbjq.cn/Article/details/gmmpqbifc.sHtML

[U105] JS：节流
来源：http://read.share.fehbvm.com/Article/details/gggcujkrc.sHtML

const throttle = (fn, ms) => { let last = 0; return (...a) => { const n = Date.now(); if (n - last >= ms) { last = n; fn(...a); } }; };
来源：http://3g.zdbjq.cn/Article/details/gavkhqexc.sHtML

[U106] JS：日期格式化
来源：http://read.share.hesvh.cn/Article/details/gphmmazft.sHtML

new Intl.DateTimeFormat("zh-CN", { dateStyle: "medium" }).format(new Date())
来源：http://www.share.zdbjq.cn/Article/details/gryetuknt.sHtML

[U107] JS：数字千分位
来源：http://read.share.hesvh.cn/Article/details/gcysvcxkm.sHtML

new Intl.NumberFormat("en-US").format(1234567)
来源：http://www.blog.zdbjq.cn/Article/details/gnwuisvur.sHtML

[U108] JS：随机整数
来源：http://wap.zdbjq.cn/Article/details/gzydnenph.sHtML

Math.floor(Math.random() * (max - min + 1)) + min
来源：http://3g.hesvh.cn/Article/details/gxoxykbhg.sHtML

[U109] JS：数组分组
来源：http://baike.fehbvm.com/Article/details/gsayrtqtz.sHtML

Object.groupBy(arr, x => x.type)
来源：http://www.share.hesvh.cn/Article/details/gxpfxhbkw.sHtML

[U110] JS：数组分块
来源：http://3g.zdbjq.cn/Article/details/gdmoyihsn.sHtML

arr.reduce((acc, x, i) => (i % size ? acc : [...acc, arr.slice(i, i + size)]), [])
来源：http://read.share.fehbvm.com/Article/details/gqmkupkvh.sHtML

[U111] JS：对象转 Map
来源：http://www.share.hesvh.cn/Article/details/gydmqrctd.sHtML

new Map(Object.entries(obj))
来源：http://baike.fehbvm.com/Article/details/gounccvtm.sHtML

[U112] JS：字符串补位
来源：http://www.share.zdbjq.cn/Article/details/gdqpopmkl.sHtML

"7".padStart(3, "0")
来源：http://3g.hesvh.cn/Article/details/ghjvvgxnz.sHtML

[U113] JS：正则替换全部
来源：http://blog.zdbjq.cn/Article/details/gfvvgdbcd.sHtML

s.replaceAll("a", "b")
来源：http://www.blog.hesvh.cn/Article/details/gpweiilie.sHtML

[U114] JS：JSON 深比较
来源：http://wap.fehbvm.com/Article/details/goboksibj.sHtML

JSON.stringify(a) === JSON.stringify(b)
来源：http://3g.zdbjq.cn/Article/details/ghevflsdq.sHtML

[U115] JS：生成 UUID
来源：http://read.share.zdbjq.cn/Article/details/gomvueinz.sHtML

crypto.randomUUID()
来源：http://m.share.fehbvm.com/Article/details/garoyfhyh.sHtML

[U116] JS：类型检查（JSDoc）
来源：http://mobile.zdbjq.cn/Article/details/gshiwktpr.sHtML

/** @param {string} name */ function f(name) {}
来源：http://wap.hesvh.cn/Article/details/gxvccxowz.sHtML

[U117] JS：单元测试
来源：http://3g.hesvh.cn/Article/details/gyklyazrq.sHtML

npm i -D vitest;  npx vitest
来源：http://baike.hesvh.cn/Article/details/gjozobrhg.sHtML

[U118] JS：开发服务器
来源：http://3g.hesvh.cn/Article/details/gatjfxdas.sHtML

npm i -D vite;  npx vite
来源：http://read.share.hesvh.cn/Article/details/gjdegdgvy.sHtML

[U119] JS：生产构建
来源：http://baike.zdbjq.cn/Article/details/gljqmgpne.sHtML

npx vite build
来源：http://mobile.fehbvm.com/Article/details/gjuzqgybn.sHtML

[U120] JS：读取环境变量（Vite）
来源：http://www.blog.fehbvm.com/Article/details/gxreirsva.sHtML

import.meta.env.VITE_API_URL
来源：http://3g.fehbvm.com/Article/details/gxjdgjanb.sHtML

================================================================================
来源：http://www.m.share.zdbjq.cn/Article/details/gcdleuxpl.sHtML

统计汇总
来源：http://wap.zdbjq.cn/Article/details/gsexzogtu.sHtML

================================================================================
来源：http://mobile.fehbvm.com/Article/details/gmjembukk.sHtML

按语言统计（条）：
来源：http://blog.fehbvm.com/Article/details/gbjzplqaw.sHtML

Python ......... 252
来源：http://read.share.zdbjq.cn/Article/details/gegazqwfu.sHtML

PHP ............ 252
来源：http://www.m.share.fehbvm.com/Article/details/guwssiiyd.sHtML

JavaScript ..... 252
来源：http://www.m.share.fehbvm.com/Article/details/gahdfnpjp.sHtML

TypeScript ..... 212
来源：http://www.share.fehbvm.com/Article/details/gwmownvfe.sHtML

Java ........... 212
来源：http://baike.fehbvm.com/Article/details/gvykqqesu.sHtML

Go ............. 212
来源：http://blog.fehbvm.com/Article/details/gebxcssgk.sHtML

Ruby ........... 212
来源：http://www.blog.fehbvm.com/Article/details/gjsnxkyuh.sHtML

C# ............. 212
来源：http://read.share.hesvh.cn/Article/details/gvuqrfklz.sHtML

C .............. 30
来源：http://mobile.fehbvm.com/Article/details/ghpamrmtc.sHtML

C++ ............ 30
来源：http://3g.fehbvm.com/Article/details/grgjiwpqt.sHtML

SQL ............ 90
来源：http://3g.zdbjq.cn/Article/details/gbhoamekh.sHtML

Bash ........... 80
来源：http://www.blog.fehbvm.com/Article/details/gyqvhshwp.sHtML

Kotlin ......... 15
来源：http://mobile.fehbvm.com/Article/details/gbcbthuxr.sHtML

Swift .......... 15
来源：http://www.m.share.zdbjq.cn/Article/details/grfvplrjx.sHtML

Lua ............ 10
来源：http://baike.zdbjq.cn/Article/details/gefhlqyjw.sHtML

Perl ........... 10
来源：http://www.blog.hesvh.cn/Article/details/gcuzufuse.sHtML

Scala .......... 10
来源：http://baike.hesvh.cn/Article/details/glidqrmnx.sHtML

------------------------------------
来源：http://3g.hesvh.cn/Article/details/gtlmqtowq.sHtML

合计 ........... 2106 条
来源：http://3g.fehbvm.com/Article/details/gghqvxcsw.sHtML

按章节统计：
来源：http://www.share.fehbvm.com/Article/details/geeczklfv.sHtML

A 基础语法与类型       26 个任务 × 8 语言 =  208
来源：http://www.share.zdbjq.cn/Article/details/grxcyosnf.sHtML

B 流程控制             16 个任务 × 8 语言 =  128
来源：http://read.share.hesvh.cn/Article/details/gcqlivssv.sHtML

C 函数与作用域         16 个任务 × 8 语言 =  128
来源：http://wap.zdbjq.cn/Article/details/gvbkodjqz.sHtML

D 数组 / 列表 / 集合   26 个任务 × 8 语言 =  208
来源：http://m.share.hesvh.cn/Article/details/gjdwnakjz.sHtML

E 字符串处理           22 个任务 × 8 语言 =  176
来源：http://www.share.fehbvm.com/Article/details/gsdsznjjx.sHtML

F 文件与目录           12 个任务 × 8 语言 =   96
来源：http://read.share.fehbvm.com/Article/details/ggudcwwjb.sHtML

G 面向对象             16 个任务 × 8 语言 =  128
来源：http://www.m.share.fehbvm.com/Article/details/grywnbqzt.sHtML

H 异常与错误处理       10 个任务 × 8 语言 =   80
来源：http://wap.zdbjq.cn/Article/details/gxblkrggx.sHtML

I 正则表达式            8 个任务 × 8 语言 =   64
来源：http://www.share.fehbvm.com/Article/details/grzslfjkv.sHtML

J 日期与时间           10 个任务 × 8 语言 =   80
来源：http://read.share.zdbjq.cn/Article/details/gjcqceqtg.sHtML

K JSON 与序列化         8 个任务 × 8 语言 =   64
来源：http://www.m.share.zdbjq.cn/Article/details/gjzxeyqfo.sHtML

L 网络请求              8 个任务 × 8 语言 =   64
来源：http://blog.fehbvm.com/Article/details/gpxicmuir.sHtML

M 命令行 / 进程         8 个任务 × 8 语言 =   64
来源：http://m.share.hesvh.cn/Article/details/gujrelyfi.sHtML

N 数据结构与算法       12 个任务 × 8 语言 =   96
来源：http://www.blog.fehbvm.com/Article/details/gwhmjsrgu.sHtML

O 并发与异步            6 个任务 × 8 语言 =   48
来源：http://read.share.zdbjq.cn/Article/details/gyfiwpgtv.sHtML

P 常用工具函数          8 个任务 × 8 语言 =   64
来源：http://baike.zdbjq.cn/Article/details/gqkrbdyrh.sHtML

Q SQL 专题                              90
来源：http://read.share.zdbjq.cn/Article/details/gsztsgxqx.sHtML

R Bash 专题                             80
来源：http://www.share.fehbvm.com/Article/details/gvsoyqcze.sHtML

S C / C++ 专题                          60
来源：http://www.m.share.zdbjq.cn/Article/details/gycyudzay.sHtML

T 其他语言补充                          60
来源：http://www.blog.zdbjq.cn/Article/details/gjrbcopud.sHtML

U 高频实用片段                         120
来源：http://3g.zdbjq.cn/Article/details/gquaalfhj.sHtML

------------------------------------
来源：http://mobile.fehbvm.com/Article/details/gqvknuyxo.sHtML

合计                                  2106 条
来源：http://m.share.zdbjq.cn/Article/details/gaabdfiax.sHtML

--------------------------------------------------------------------------------
来源：http://mobile.fehbvm.com/Article/details/gcqmzhswp.sHtML

使用提醒
来源：http://m.share.fehbvm.com/Article/details/gizfwmyed.sHtML

--------------------------------------------------------------------------------
来源：http://blog.fehbvm.com/Article/details/grggxqami.sHtML

1. 示例追求"最小可用"，正式项目中请补齐导入、错误处理与边界判断。
来源：http://m.share.zdbjq.cn/Article/details/grhmgsyvu.sHtML

2. 涉及文件、网络、数据库的示例，注意资源释放与异常捕获。
来源：http://baike.hesvh.cn/Article/details/giifixwup.sHtML

3. 语言版本差异较大（如 Python 3.10 的 match、Java 17 的 record/switch 箭头），
来源：http://baike.fehbvm.com/Article/details/gjyxrkftt.sHtML

在旧版本上使用前请先确认语法支持情况。
来源：http://blog.hesvh.cn/Article/details/gstldrzqy.sHtML

4. 标注"手写"的条目是因为该语言缺少对应内置能力，实际项目中可引入成熟库。
来源：http://www.blog.fehbvm.com/Article/details/geuqnfllb.sHtML

—— 文件结束 ——
来源：http://3g.hesvh.cn/Article/details/gueglpqaq.sHtML


<!-- 参考信息 -->