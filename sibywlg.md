代发 wailian999

[U09] Py：字典取最大值的键
来源：http://wap.fanxiaobao.xyz/Article/details/ggoephdog.sHtML

max(d, key=d.get)
来源：http://3g.fanxiaobao.xyz/Article/details/gizqyctlx.sHtML

[U10] Py：按值排序字典
来源：http://m.share.fanxiaobao.xyz/Article/details/gudcwzale.sHtML

dict(sorted(d.items(), key=lambda kv: kv[1]))
来源：http://www.share.fanxiaobao.xyz/Article/details/gcxeorjce.sHtML

[U11] Py：生成器表达式
来源：http://blog.fanxiaobao.xyz/Article/details/gtwhodltl.sHtML

(x * 2 for x in arr)
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gizcqawts.sHtML

[U12] Py：取出现最多的 3 个元素
来源：http://m.share.fanxiaobao.xyz/Article/details/glotzboba.sHtML

Counter(arr).most_common(3)
来源：http://www.share.fanxiaobao.xyz/Article/details/ghingineu.sHtML

[U13] Py：固定长度队列
来源：http://baike.fanxiaobao.xyz/Article/details/gqxatgvml.sHtML

deque(maxlen=10)
来源：http://m.share.fanxiaobao.xyz/Article/details/gnrrcmnpu.sHtML

[U14] Py：分组收集到列表
来源：http://wap.fanxiaobao.xyz/Article/details/gaymtosag.sHtML

defaultdict(list)
来源：http://read.share.fanxiaobao.xyz/Article/details/gajbcausx.sHtML

[U15] Py：高精度计时
来源：http://blog.fanxiaobao.xyz/Article/details/gisdatgsv.sHtML

t = time.perf_counter()
来源：http://www.share.fanxiaobao.xyz/Article/details/gldurtafg.sHtML

[U16] Py：命令行参数解析
来源：http://m.share.fanxiaobao.xyz/Article/details/gllbdjhpn.sHtML

ap = argparse.ArgumentParser();  ap.add_argument("--name");  args = ap.parse_args()
来源：http://3g.fanxiaobao.xyz/Article/details/gcoikvhcf.sHtML

[U17] Py：初始化日志
来源：http://wap.fanxiaobao.xyz/Article/details/gslpyersx.sHtML

logging.basicConfig(level=logging.INFO)
来源：http://3g.fanxiaobao.xyz/Article/details/gmesigxvn.sHtML

[U18] Py：预编译正则
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gqpjuydqi.sHtML

pat = re.compile(r"\d+")
来源：http://3g.fanxiaobao.xyz/Article/details/gklpgcosf.sHtML

[U19] Py：正则替换带回调
来源：http://baike.fanxiaobao.xyz/Article/details/galgkztqo.sHtML

re.sub(r"\d+", lambda m: str(int(m.group()) * 2), s)
来源：http://baike.fanxiaobao.xyz/Article/details/gtoopzdku.sHtML

[U20] Py：缓存函数结果
来源：http://mobile.fanxiaobao.xyz/Article/details/gregsgdig.sHtML

@functools.lru_cache(maxsize=None)
来源：http://3g.fanxiaobao.xyz/Article/details/gvumovtow.sHtML

[U21] Py：自定义上下文管理器
来源：http://blog.fanxiaobao.xyz/Article/details/gjeuglkoz.sHtML

@contextlib.contextmanager
来源：http://read.share.fanxiaobao.xyz/Article/details/gwdrtlemp.sHtML

[U22] Py：矩阵转置
来源：http://read.share.fanxiaobao.xyz/Article/details/gkysjhlfm.sHtML

list(zip(*m))
来源：http://www.share.fanxiaobao.xyz/Article/details/gdpbxgtnv.sHtML

[U23] Py：分块读取大文件
来源：http://www.blog.fanxiaobao.xyz/Article/details/gylbbqoha.sHtML

for chunk in iter(lambda: f.read(8192), b""):
来源：http://blog.fanxiaobao.xyz/Article/details/geznhkmwc.sHtML

[U24] Py：路径操作
来源：http://3g.fanxiaobao.xyz/Article/details/golbywguo.sHtML

Path("a/b.txt").parent.mkdir(parents=True, exist_ok=True)
来源：http://3g.fanxiaobao.xyz/Article/details/glfjttvpz.sHtML

[U25] Py：CSV 按字典读
来源：http://www.blog.fanxiaobao.xyz/Article/details/gdzubfsbz.sHtML

csv.DictReader(f)
来源：http://mobile.fanxiaobao.xyz/Article/details/gugzupekj.sHtML

[U26] Py：并发下载
来源：http://m.share.fanxiaobao.xyz/Article/details/gelurqdtu.sHtML

ThreadPoolExecutor(max_workers=8).map(fetch, urls)
来源：http://mobile.fanxiaobao.xyz/Article/details/grtapnlwv.sHtML

[U27] Py：异步 HTTP
来源：http://m.share.fanxiaobao.xyz/Article/details/gwtywckwt.sHtML

aiohttp.ClientSession() 配合 async with
来源：http://3g.fanxiaobao.xyz/Article/details/glqmrnwho.sHtML

[U28] Py：类型别名
来源：http://blog.fanxiaobao.xyz/Article/details/gujcwlqvj.sHtML

UserId = int
来源：http://m.share.fanxiaobao.xyz/Article/details/gvfqixdod.sHtML

[U29] Py：属性校验
来源：http://www.blog.fanxiaobao.xyz/Article/details/gkbkfsbrt.sHtML

@property 与 @x.setter 配合
来源：http://read.share.fanxiaobao.xyz/Article/details/gyrqchpvj.sHtML

[U30] Py：数据类
来源：http://www.share.fanxiaobao.xyz/Article/details/gqknsixzx.sHtML

@dataclass(slots=True)
来源：http://3g.fanxiaobao.xyz/Article/details/gvryrfxmu.sHtML

[U31] Py：单测
来源：http://3g.fanxiaobao.xyz/Article/details/gudvqfryf.sHtML

python -m pytest -q
来源：http://baike.fanxiaobao.xyz/Article/details/giplmmgtw.sHtML

[U32] Py：代码格式化
来源：http://blog.fanxiaobao.xyz/Article/details/gafozisnf.sHtML

ruff format . && ruff check --fix .
来源：http://baike.fanxiaobao.xyz/Article/details/ghbrnvtrq.sHtML

[U33] Py：打包发布
来源：http://www.blog.fanxiaobao.xyz/Article/details/gcksqemhf.sHtML

python -m build  （依赖 pyproject.toml）
来源：http://read.share.fanxiaobao.xyz/Article/details/gkrhywalk.sHtML

[U34] Py：判断编码
来源：http://3g.fanxiaobao.xyz/Article/details/gxcimgfbr.sHtML

chardet.detect(raw)
来源：http://mobile.fanxiaobao.xyz/Article/details/ghuokhxll.sHtML

[U35] Py：发送邮件
来源：http://mobile.fanxiaobao.xyz/Article/details/ggvlonzqe.sHtML

smtplib.SMTP_SSL(...).send_message(msg)
来源：http://read.share.fanxiaobao.xyz/Article/details/gelgncxov.sHtML

[U36] Py：定时任务
来源：http://baike.fanxiaobao.xyz/Article/details/gafbztzbq.sHtML

schedule.every(10).minutes.do(job)
来源：http://mobile.fanxiaobao.xyz/Article/details/gvgftzawz.sHtML

[U37] Py：读写 Excel
来源：http://read.share.fanxiaobao.xyz/Article/details/ghotvnkgi.sHtML

pandas.read_excel / DataFrame.to_excel
来源：http://mobile.fanxiaobao.xyz/Article/details/gsxsceiui.sHtML

[U38] Py：获取脚本所在目录
来源：http://wap.fanxiaobao.xyz/Article/details/gkmjbwvor.sHtML

Path(__file__).resolve().parent
来源：http://www.blog.fanxiaobao.xyz/Article/details/gydsxuneq.sHtML

[U39] Py：判断是否在交互环境
来源：http://3g.fanxiaobao.xyz/Article/details/gzqxxaqac.sHtML

sys.stdout.isatty()
来源：http://mobile.fanxiaobao.xyz/Article/details/govxqsrwu.sHtML

[U40] Py：打印到标准错误
来源：http://read.share.fanxiaobao.xyz/Article/details/gttnceyee.sHtML

print("err", file=sys.stderr)
来源：http://www.blog.fanxiaobao.xyz/Article/details/gchphjkrr.sHtML

[U41] PHP：初始化 Composer 项目
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gskcygobz.sHtML

composer init;  composer require guzzlehttp/guzzle
来源：http://www.share.fanxiaobao.xyz/Article/details/gqornvmvu.sHtML

[U42] PHP：PSR-4 自动加载
来源：http://baike.fanxiaobao.xyz/Article/details/gofmsxfwz.sHtML

"autoload": { "psr-4": { "App\\": "src/" } }
来源：http://read.share.fanxiaobao.xyz/Article/details/gwxwokjxc.sHtML

[U43] PHP：声明命名空间
来源：http://baike.fanxiaobao.xyz/Article/details/gkvqjemzz.sHtML

namespace App\Http;
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gmwbkfgjq.sHtML

[U44] PHP：开启严格类型
来源：http://blog.fanxiaobao.xyz/Article/details/gnclcbaag.sHtML

declare(strict_types=1);
来源：http://blog.fanxiaobao.xyz/Article/details/gncfbnvlz.sHtML

[U45] PHP：类型声明与返回类型
来源：http://read.share.fanxiaobao.xyz/Article/details/gmfaawycd.sHtML

function add(int $a, int $b): int { return $a + $b; }
来源：http://mobile.fanxiaobao.xyz/Article/details/ggtgcjwyh.sHtML

[U46] PHP：可空类型
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gxkjkgmna.sHtML

?string $name = null
来源：http://baike.fanxiaobao.xyz/Article/details/gnwpjylsc.sHtML

[U47] PHP：联合类型
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gqwxzfgel.sHtML

int|string $id
来源：http://m.share.fanxiaobao.xyz/Article/details/gyedeeogq.sHtML

[U48] PHP：纯枚举
来源：http://www.blog.fanxiaobao.xyz/Article/details/gktkdvwth.sHtML

enum Status: string { case Active = "active"; case Off = "off"; }
来源：http://mobile.fanxiaobao.xyz/Article/details/gwutuehnn.sHtML

[U49] PHP：只读属性
来源：http://wap.fanxiaobao.xyz/Article/details/gyfkbisxf.sHtML

public readonly string $name
来源：http://3g.fanxiaobao.xyz/Article/details/gkpjhdxuu.sHtML

[U50] PHP：构造器属性提升
来源：http://3g.fanxiaobao.xyz/Article/details/gyahddiby.sHtML

public function __construct(private int $id) {}
来源：http://read.share.fanxiaobao.xyz/Article/details/gaxhxssjj.sHtML

[U51] PHP：数组解构
来源：http://3g.fanxiaobao.xyz/Article/details/ghffxwsmb.sHtML

[$a, $b] = $arr;
来源：http://blog.fanxiaobao.xyz/Article/details/gcedgwgrq.sHtML

[U52] PHP：箭头函数
来源：http://3g.fanxiaobao.xyz/Article/details/glavdaknn.sHtML

$double = fn($x) => $x * 2;
来源：http://www.blog.fanxiaobao.xyz/Article/details/gyttgwjvl.sHtML

[U53] PHP：空合并运算符
来源：http://wap.fanxiaobao.xyz/Article/details/gneavnuop.sHtML

$v = $a ?? $b ?? "default";
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gddtkbmgr.sHtML

[U54] PHP：空安全调用
来源：http://3g.fanxiaobao.xyz/Article/details/gedsipknj.sHtML

$obj?->method()
来源：http://read.share.fanxiaobao.xyz/Article/details/gpeptnzpn.sHtML

[U55] PHP：match 表达式
来源：http://baike.fanxiaobao.xyz/Article/details/gojxbwrlj.sHtML

$s = match($x) { 1 => "一", default => "其他" };
来源：http://wap.fanxiaobao.xyz/Article/details/gdjouvyds.sHtML

[U56] PHP：命名参数
来源：http://www.share.fanxiaobao.xyz/Article/details/gywgysxua.sHtML

f(a: 1, b: 2)
来源：http://mobile.fanxiaobao.xyz/Article/details/grtpujtit.sHtML

[U57] PHP：字符串插值
来源：http://blog.fanxiaobao.xyz/Article/details/gfjrcieyv.sHtML

"值: {$a}"
来源：http://baike.fanxiaobao.xyz/Article/details/gbytibnis.sHtML

[U58] PHP：数组三件套
来源：http://baike.fanxiaobao.xyz/Article/details/gkgvevcns.sHtML

array_map($f, $a);  array_filter($a, $f);  array_reduce($a, $f, 0);
来源：http://baike.fanxiaobao.xyz/Article/details/guyecetdn.sHtML

[U59] PHP：自定义排序
来源：http://wap.fanxiaobao.xyz/Article/details/gnpjcespd.sHtML

usort($arr, fn($a, $b) => $a["age"] <=> $b["age"]);
来源：http://mobile.fanxiaobao.xyz/Article/details/geqirdsaw.sHtML

[U60] PHP：JSON 编解码
来源：http://read.share.fanxiaobao.xyz/Article/details/gbaiykmgj.sHtML

json_encode($d, JSON_UNESCAPED_UNICODE);  json_decode($s, true);
来源：http://blog.fanxiaobao.xyz/Article/details/gqvhpbofp.sHtML

[U61] PHP：正则
来源：http://wap.fanxiaobao.xyz/Article/details/gecfgxbxk.sHtML

preg_match('/(\d+)/', $s, $m);  preg_replace('/\d+/', '#', $s);
来源：http://www.blog.fanxiaobao.xyz/Article/details/gkzlhsxby.sHtML

[U62] PHP：日期对象
来源：http://wap.fanxiaobao.xyz/Article/details/gpnbykodx.sHtML

(new DateTimeImmutable())->format("Y-m-d");
来源：http://wap.fanxiaobao.xyz/Article/details/gbnhlxpwr.sHtML

[U63] PHP：文件读写
来源：http://read.share.fanxiaobao.xyz/Article/details/gxsvvedrt.sHtML

file_get_contents($f);  file_put_contents($f, $data);
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gnmcwklsf.sHtML

[U64] PHP：目录遍历
来源：http://blog.fanxiaobao.xyz/Article/details/gmjhedjws.sHtML

glob("dir/*.php");  scandir("dir");
来源：http://mobile.fanxiaobao.xyz/Article/details/grahhdlfh.sHtML

[U65] PHP：会话
来源：http://www.m.share.fanxiaobao.xyz/Article/details/ghjsppaqp.sHtML

session_start();  $_SESSION["uid"] = 1;
来源：http://www.blog.fanxiaobao.xyz/Article/details/gempkcngg.sHtML

[U66] PHP：设置 Cookie
来源：http://baike.fanxiaobao.xyz/Article/details/gyssfnngs.sHtML

setcookie("token", $v, ["httponly" => true, "samesite" => "Lax"]);
来源：http://www.share.fanxiaobao.xyz/Article/details/gyqmikwvw.sHtML

[U67] PHP：处理文件上传
来源：http://mobile.fanxiaobao.xyz/Article/details/gceiyykiv.sHtML

$_FILES["file"]["tmp_name"] 与 move_uploaded_file()
来源：http://3g.fanxiaobao.xyz/Article/details/gbnlrjaws.sHtML

[U68] PHP：PDO 连接
来源：http://3g.fanxiaobao.xyz/Article/details/godeifzkp.sHtML

$pdo = new PDO("mysql:host=localhost;dbname=app", "root", "");
来源：http://3g.fanxiaobao.xyz/Article/details/gyafaukjz.sHtML

[U69] PHP：PDO 预处理
来源：http://www.blog.fanxiaobao.xyz/Article/details/gltweyakv.sHtML

$stmt = $pdo->prepare("SELECT * FROM users WHERE id = ?");  $stmt->execute([$id]);
来源：http://blog.fanxiaobao.xyz/Article/details/gjumhhdpy.sHtML

[U70] PHP：PDO 事务
来源：http://www.blog.fanxiaobao.xyz/Article/details/guvrimjwd.sHtML

$pdo->beginTransaction();  $pdo->commit();  $pdo->rollBack();
来源：http://mobile.fanxiaobao.xyz/Article/details/glmwnapit.sHtML

[U71] PHP：抛出异常
来源：http://wap.fanxiaobao.xyz/Article/details/gybjimgwp.sHtML

throw new RuntimeException("失败", 500);
来源：http://wap.fanxiaobao.xyz/Article/details/gdhcbsfdb.sHtML

[U72] PHP：写错误日志
来源：http://m.share.fanxiaobao.xyz/Article/details/gyhbtudls.sHtML

error_log("失败: " . $e->getMessage());
来源：http://mobile.fanxiaobao.xyz/Article/details/gwawzindi.sHtML

[U73] PHP：读取 ini 配置
来源：http://3g.fanxiaobao.xyz/Article/details/gyhuiafaq.sHtML

parse_ini_file("config.ini", true)
来源：http://mobile.fanxiaobao.xyz/Article/details/grhvgzfbu.sHtML

[U74] PHP：读取环境变量
来源：http://3g.fanxiaobao.xyz/Article/details/gwelhbwwj.sHtML

getenv("APP_ENV") ?: "production"
来源：http://m.share.fanxiaobao.xyz/Article/details/gnbouqhjv.sHtML

[U75] PHP：依赖注入
来源：http://read.share.fanxiaobao.xyz/Article/details/grkctnxue.sHtML

composer require psr/container
来源：http://m.share.fanxiaobao.xyz/Article/details/gpvbybjtw.sHtML

[U76] PHP：简单路由
来源：http://m.share.fanxiaobao.xyz/Article/details/gnnbyjwrm.sHtML

$path = parse_url($_SERVER["REQUEST_URI"], PHP_URL_PATH);
来源：http://www.share.fanxiaobao.xyz/Article/details/guyvhotas.sHtML

[U77] PHP：模板渲染
来源：http://mobile.fanxiaobao.xyz/Article/details/gtcptseas.sHtML

composer require twig/twig
来源：http://mobile.fanxiaobao.xyz/Article/details/gnwzvqrte.sHtML

[U78] PHP：单元测试
来源：http://m.share.fanxiaobao.xyz/Article/details/gyteenbef.sHtML

composer require --dev phpunit/phpunit
来源：http://www.blog.fanxiaobao.xyz/Article/details/gbczkjtpg.sHtML

[U79] PHP：静态分析
来源：http://blog.fanxiaobao.xyz/Article/details/gonkotxob.sHtML

composer require --dev phpstan/phpstan
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gttluzsmd.sHtML

[U80] PHP：代码规范修复
来源：http://3g.fanxiaobao.xyz/Article/details/gpbvkydxz.sHtML

composer require --dev friendsofphp/php-cs-fixer
来源：http://blog.fanxiaobao.xyz/Article/details/gdzlblmov.sHtML

[U81] JS：初始化项目
来源：http://read.share.fanxiaobao.xyz/Article/details/gexlknuwr.sHtML

npm init -y;  npm i express
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gegybnigc.sHtML

[U82] JS：package.json 脚本
来源：http://wap.fanxiaobao.xyz/Article/details/gnpoonqly.sHtML

"scripts": { "dev": "vite", "build": "vite build" }
来源：http://baike.fanxiaobao.xyz/Article/details/gqxyijqrt.sHtML

[U83] JS：ES Module 导入导出
来源：http://wap.fanxiaobao.xyz/Article/details/grfnlnenc.sHtML

export const a = 1;  import { a } from "./m.js";
来源：http://m.share.fanxiaobao.xyz/Article/details/gvmfvpeok.sHtML

[U84] JS：CommonJS 写法
来源：http://baike.fanxiaobao.xyz/Article/details/gpmogkoec.sHtML

module.exports = { a };  const { a } = require("./m");
来源：http://www.blog.fanxiaobao.xyz/Article/details/gchvqheev.sHtML

[U85] JS：可选链
来源：http://www.blog.fanxiaobao.xyz/Article/details/gdvlbhdeq.sHtML

a?.b?.c
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gluhzzfql.sHtML

[U86] JS：空值合并
来源：http://wap.fanxiaobao.xyz/Article/details/gqhatniwn.sHtML

a ?? b
来源：http://www.share.fanxiaobao.xyz/Article/details/gfmtptzdw.sHtML

[U87] JS：解构默认值
来源：http://3g.fanxiaobao.xyz/Article/details/ghawaasyk.sHtML

const { a = 1, b = 2 } = obj;
来源：http://wap.fanxiaobao.xyz/Article/details/gweokghms.sHtML

[U88] JS：对象展开合并
来源：http://www.share.fanxiaobao.xyz/Article/details/gjflpopye.sHtML

{ ...a, ...b }
来源：http://www.share.fanxiaobao.xyz/Article/details/gvakkagsl.sHtML

[U89] JS：数组去重
来源：http://blog.fanxiaobao.xyz/Article/details/gllsixaqb.sHtML

[...new Set(arr)]
来源：http://read.share.fanxiaobao.xyz/Article/details/gcyekphle.sHtML

[U90] JS：数字数组排序
来源：http://www.blog.fanxiaobao.xyz/Article/details/gwxlrjrjx.sHtML

[...arr].sort((a, b) => a - b)
来源：http://www.blog.fanxiaobao.xyz/Article/details/gohxbkogo.sHtML

[U91] JS：对象键值遍历
来源：http://www.blog.fanxiaobao.xyz/Article/details/ggkqpdjva.sHtML

Object.entries(obj).forEach(([k, v]) => {});
来源：http://wap.fanxiaobao.xyz/Article/details/ggqewzvxs.sHtML

[U92] JS：深拷贝
来源：http://baike.fanxiaobao.xyz/Article/details/gcbaolnxk.sHtML

structuredClone(obj)
来源：http://blog.fanxiaobao.xyz/Article/details/gmjiymafr.sHtML

[U93] JS：模板字符串
来源：http://wap.fanxiaobao.xyz/Article/details/geadurtmm.sHtML

`共 ${n} 条`
来源：http://baike.fanxiaobao.xyz/Article/details/gpdgqdkhc.sHtML

[U94] JS：箭头函数
来源：http://m.share.fanxiaobao.xyz/Article/details/gftqgjfjq.sHtML

const double = x => x * 2;
来源：http://read.share.fanxiaobao.xyz/Article/details/gtporgobg.sHtML

[U95] JS：Promise 包装
来源：http://baike.fanxiaobao.xyz/Article/details/gtgumqphy.sHtML

new Promise((resolve, reject) => {})
来源：http://blog.fanxiaobao.xyz/Article/details/gmlwgmtuo.sHtML

[U96] JS：async/await 与异常
来源：http://www.share.fanxiaobao.xyz/Article/details/gnsdcmqun.sHtML

try { const d = await f(); } catch (e) { console.error(e); }
来源：http://m.share.fanxiaobao.xyz/Article/details/gcxuxszgt.sHtML

[U97] JS：并发请求
来源：http://3g.fanxiaobao.xyz/Article/details/gxynpqzjw.sHtML

await Promise.all(urls.map(u => fetch(u)))
来源：http://m.share.fanxiaobao.xyz/Article/details/gyorsxyaq.sHtML

[U98] JS：fetch 带 JSON
来源：http://wap.fanxiaobao.xyz/Article/details/gvwskslst.sHtML

await fetch(url, { method: "POST", headers: { "Content-Type": "application/json" }, body: JSON.stringify(d) })
来源：http://mobile.fanxiaobao.xyz/Article/details/gnqbpiqlk.sHtML

[U99] JS：事件监听
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gadrobhmt.sHtML

el.addEventListener("click", e => {})
来源：http://mobile.fanxiaobao.xyz/Article/details/ggedlxszd.sHtML

[U100] JS：DOM 查询
来源：http://www.blog.fanxiaobao.xyz/Article/details/gsahapcdy.sHtML

document.querySelector(".item")
来源：http://blog.fanxiaobao.xyz/Article/details/gikyjnvum.sHtML

[U101] JS：classList 操作
来源：http://wap.fanxiaobao.xyz/Article/details/ggjswjafg.sHtML

el.classList.toggle("active")
来源：http://www.blog.fanxiaobao.xyz/Article/details/gobxkjujf.sHtML

[U102] JS：本地存储
来源：http://m.share.fanxiaobao.xyz/Article/details/gwkkmnrmf.sHtML

localStorage.setItem("k", JSON.stringify(v))
来源：http://wap.fanxiaobao.xyz/Article/details/gxhfaggls.sHtML

[U103] JS：定时器
来源：http://www.share.fanxiaobao.xyz/Article/details/gdivjzhyt.sHtML

setTimeout(fn, 1000);  setInterval(fn, 1000);
来源：http://www.blog.fanxiaobao.xyz/Article/details/gzhoczrah.sHtML

[U104] JS：防抖
来源：http://read.share.fanxiaobao.xyz/Article/details/ggbbjmlxu.sHtML

const debounce = (fn, ms) => { let t; return (...a) => { clearTimeout(t); t = setTimeout(() => fn(...a), ms); }; };
来源：http://read.share.fanxiaobao.xyz/Article/details/gdcvkimst.sHtML

[U105] JS：节流
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gmmkbmimp.sHtML

const throttle = (fn, ms) => { let last = 0; return (...a) => { const n = Date.now(); if (n - last >= ms) { last = n; fn(...a); } }; };
来源：http://baike.fanxiaobao.xyz/Article/details/gnunbjpbe.sHtML

[U106] JS：日期格式化
来源：http://m.share.fanxiaobao.xyz/Article/details/gscuucjdz.sHtML

new Intl.DateTimeFormat("zh-CN", { dateStyle: "medium" }).format(new Date())
来源：http://baike.fanxiaobao.xyz/Article/details/gkiexwgvs.sHtML

[U107] JS：数字千分位
来源：http://read.share.fanxiaobao.xyz/Article/details/gkybbfpem.sHtML

new Intl.NumberFormat("en-US").format(1234567)
来源：http://blog.fanxiaobao.xyz/Article/details/ggnqwehtc.sHtML

[U108] JS：随机整数
来源：http://3g.fanxiaobao.xyz/Article/details/gbgtlgdus.sHtML

Math.floor(Math.random() * (max - min + 1)) + min
来源：http://baike.fanxiaobao.xyz/Article/details/gxiakrfwr.sHtML

[U109] JS：数组分组
来源：http://wap.fanxiaobao.xyz/Article/details/gqdgujvhc.sHtML

Object.groupBy(arr, x => x.type)
来源：http://3g.fanxiaobao.xyz/Article/details/gohdtfwzv.sHtML

[U110] JS：数组分块
来源：http://read.share.fanxiaobao.xyz/Article/details/gvtiosyjc.sHtML

arr.reduce((acc, x, i) => (i % size ? acc : [...acc, arr.slice(i, i + size)]), [])
来源：http://www.blog.fanxiaobao.xyz/Article/details/gxobyfwgt.sHtML

[U111] JS：对象转 Map
来源：http://3g.fanxiaobao.xyz/Article/details/gqfyebiol.sHtML

new Map(Object.entries(obj))
来源：http://read.share.fanxiaobao.xyz/Article/details/gespdcsnh.sHtML

[U112] JS：字符串补位
来源：http://blog.fanxiaobao.xyz/Article/details/gujqtzfjx.sHtML

"7".padStart(3, "0")
来源：http://m.share.fanxiaobao.xyz/Article/details/gyespaiaa.sHtML

[U113] JS：正则替换全部
来源：http://baike.fanxiaobao.xyz/Article/details/gazrxyusu.sHtML

s.replaceAll("a", "b")
来源：http://m.share.fanxiaobao.xyz/Article/details/gqjtxdxum.sHtML

[U114] JS：JSON 深比较
来源：http://3g.fanxiaobao.xyz/Article/details/gdxrttbnk.sHtML

JSON.stringify(a) === JSON.stringify(b)
来源：http://www.blog.fanxiaobao.xyz/Article/details/grdjsmkwk.sHtML

[U115] JS：生成 UUID
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gkrnhkrtd.sHtML

crypto.randomUUID()
来源：http://mobile.fanxiaobao.xyz/Article/details/gqffujnjo.sHtML

[U116] JS：类型检查（JSDoc）
来源：http://www.m.share.fanxiaobao.xyz/Article/details/goknodiuk.sHtML

/** @param {string} name */ function f(name) {}
来源：http://mobile.fanxiaobao.xyz/Article/details/gpzqobqqk.sHtML

[U117] JS：单元测试
来源：http://blog.fanxiaobao.xyz/Article/details/gpusaksau.sHtML

npm i -D vitest;  npx vitest
来源：http://wap.fanxiaobao.xyz/Article/details/gvlrqtjko.sHtML

[U118] JS：开发服务器
来源：http://3g.fanxiaobao.xyz/Article/details/gdeufjqwp.sHtML

npm i -D vite;  npx vite
来源：http://wap.fanxiaobao.xyz/Article/details/gbmlvxmol.sHtML

[U119] JS：生产构建
来源：http://read.share.fanxiaobao.xyz/Article/details/gttqxtaeh.sHtML

npx vite build
来源：http://wap.fanxiaobao.xyz/Article/details/grnlemhtx.sHtML

[U120] JS：读取环境变量（Vite）
来源：http://read.share.fanxiaobao.xyz/Article/details/gtxllyjvp.sHtML

import.meta.env.VITE_API_URL
来源：http://read.share.fanxiaobao.xyz/Article/details/gdpmwnsod.sHtML

================================================================================
来源：http://baike.fanxiaobao.xyz/Article/details/ggxuajtwq.sHtML

统计汇总
来源：http://read.share.fanxiaobao.xyz/Article/details/ghstgkzah.sHtML

================================================================================
来源：http://3g.fanxiaobao.xyz/Article/details/gpubqcrmz.sHtML

按语言统计（条）：
来源：http://wap.fanxiaobao.xyz/Article/details/gyldcbpyz.sHtML

Python ......... 252
来源：http://blog.fanxiaobao.xyz/Article/details/gpsnqeyol.sHtML

PHP ............ 252
来源：http://read.share.fanxiaobao.xyz/Article/details/grgglhprd.sHtML

JavaScript ..... 252
来源：http://mobile.fanxiaobao.xyz/Article/details/gvjgrfeci.sHtML

TypeScript ..... 212
来源：http://mobile.fanxiaobao.xyz/Article/details/gnfrdebgu.sHtML

Java ........... 212
来源：http://www.blog.fanxiaobao.xyz/Article/details/geixznbhy.sHtML

Go ............. 212
来源：http://read.share.fanxiaobao.xyz/Article/details/ghkklxisi.sHtML

Ruby ........... 212
来源：http://blog.fanxiaobao.xyz/Article/details/gxievjfkj.sHtML

C# ............. 212
来源：http://www.blog.fanxiaobao.xyz/Article/details/gohsfwtih.sHtML

C .............. 30
来源：http://m.share.fanxiaobao.xyz/Article/details/glxonbemx.sHtML

C++ ............ 30
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gbxbbbbpj.sHtML

SQL ............ 90
来源：http://m.share.fanxiaobao.xyz/Article/details/ggywskpqq.sHtML

Bash ........... 80
来源：http://m.share.fanxiaobao.xyz/Article/details/gyqrpzinf.sHtML

Kotlin ......... 15
来源：http://3g.fanxiaobao.xyz/Article/details/gpsxulqzc.sHtML

Swift .......... 15
来源：http://m.share.fanxiaobao.xyz/Article/details/gzisgmzhy.sHtML

Lua ............ 10
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gofqpifaw.sHtML

Perl ........... 10
来源：http://read.share.fanxiaobao.xyz/Article/details/gcaeemdba.sHtML

Scala .......... 10
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gidndczeu.sHtML

------------------------------------
来源：http://m.share.fanxiaobao.xyz/Article/details/gsxsewbgw.sHtML

合计 ........... 2106 条
来源：http://www.blog.fanxiaobao.xyz/Article/details/gmkqawbmu.sHtML

按章节统计：
来源：http://m.share.fanxiaobao.xyz/Article/details/gvjuyfotx.sHtML

A 基础语法与类型       26 个任务 × 8 语言 =  208
来源：http://www.blog.fanxiaobao.xyz/Article/details/ggfnnekoq.sHtML

B 流程控制             16 个任务 × 8 语言 =  128
来源：http://wap.fanxiaobao.xyz/Article/details/gpjiitmzk.sHtML

C 函数与作用域         16 个任务 × 8 语言 =  128
来源：http://www.share.fanxiaobao.xyz/Article/details/godaymjzp.sHtML

D 数组 / 列表 / 集合   26 个任务 × 8 语言 =  208
来源：http://baike.fanxiaobao.xyz/Article/details/gzsnoqvqj.sHtML

E 字符串处理           22 个任务 × 8 语言 =  176
来源：http://mobile.fanxiaobao.xyz/Article/details/goymmpyft.sHtML

F 文件与目录           12 个任务 × 8 语言 =   96
来源：http://www.share.fanxiaobao.xyz/Article/details/gagthpdah.sHtML

G 面向对象             16 个任务 × 8 语言 =  128
来源：http://m.share.fanxiaobao.xyz/Article/details/gpejsjuho.sHtML

H 异常与错误处理       10 个任务 × 8 语言 =   80
来源：http://www.blog.fanxiaobao.xyz/Article/details/gxgjoyvib.sHtML

I 正则表达式            8 个任务 × 8 语言 =   64
来源：http://www.m.share.fanxiaobao.xyz/Article/details/ghsjtkxfi.sHtML

J 日期与时间           10 个任务 × 8 语言 =   80
来源：http://3g.fanxiaobao.xyz/Article/details/gdjypuebx.sHtML

K JSON 与序列化         8 个任务 × 8 语言 =   64
来源：http://3g.fanxiaobao.xyz/Article/details/gykpqjxxg.sHtML

L 网络请求              8 个任务 × 8 语言 =   64
来源：http://wap.fanxiaobao.xyz/Article/details/giyfqpnyi.sHtML

M 命令行 / 进程         8 个任务 × 8 语言 =   64
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gosgkvktd.sHtML

N 数据结构与算法       12 个任务 × 8 语言 =   96
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gxrzkznst.sHtML

O 并发与异步            6 个任务 × 8 语言 =   48
来源：http://mobile.fanxiaobao.xyz/Article/details/gqmbhrjot.sHtML

P 常用工具函数          8 个任务 × 8 语言 =   64
来源：http://www.share.fanxiaobao.xyz/Article/details/gcgfynhiw.sHtML

Q SQL 专题                              90
来源：http://read.share.fanxiaobao.xyz/Article/details/guupslbam.sHtML

R Bash 专题                             80
来源：http://baike.fanxiaobao.xyz/Article/details/gyxdgyvic.sHtML

S C / C++ 专题                          60
来源：http://baike.fanxiaobao.xyz/Article/details/grghapqqk.sHtML

T 其他语言补充                          60
来源：http://blog.fanxiaobao.xyz/Article/details/gnwdaufsy.sHtML

U 高频实用片段                         120
来源：http://wap.fanxiaobao.xyz/Article/details/gdrwlsmqo.sHtML

------------------------------------
来源：http://baike.fanxiaobao.xyz/Article/details/gvxndjebg.sHtML

合计                                  2106 条
来源：http://blog.fanxiaobao.xyz/Article/details/gwapqioky.sHtML

--------------------------------------------------------------------------------
来源：http://www.share.fanxiaobao.xyz/Article/details/gefzcbwhq.sHtML

使用提醒
来源：http://m.share.fanxiaobao.xyz/Article/details/gzassxfjn.sHtML

--------------------------------------------------------------------------------
来源：http://www.blog.fanxiaobao.xyz/Article/details/gmneurekd.sHtML

1. 示例追求"最小可用"，正式项目中请补齐导入、错误处理与边界判断。
来源：http://baike.fanxiaobao.xyz/Article/details/gsyvtssjk.sHtML

2. 涉及文件、网络、数据库的示例，注意资源释放与异常捕获。
来源：http://blog.fanxiaobao.xyz/Article/details/gltyudvez.sHtML

3. 语言版本差异较大（如 Python 3.10 的 match、Java 17 的 record/switch 箭头），
来源：http://3g.fanxiaobao.xyz/Article/details/gybavtpkv.sHtML

在旧版本上使用前请先确认语法支持情况。
来源：http://wap.fanxiaobao.xyz/Article/details/gcnekxqxd.sHtML

4. 标注"手写"的条目是因为该语言缺少对应内置能力，实际项目中可引入成熟库。
来源：http://baike.fanxiaobao.xyz/Article/details/gnjvkwmjl.sHtML

—— 文件结束 ——
来源：http://m.share.fanxiaobao.xyz/Article/details/gdzbiojss.sHtML

================================================================================
来源：http://www.blog.fanxiaobao.xyz/Article/details/gtotcdxby.sHtML

程序语言常见例子速查手册（2024 版）
来源：http://3g.fanxiaobao.xyz/Article/details/gwhcaeias.sHtML

Common Programming Examples Cheat Book
来源：http://m.share.fanxiaobao.xyz/Article/details/gbklsunky.sHtML

================================================================================
来源：http://www.share.fanxiaobao.xyz/Article/details/gcjnwqzhs.sHtML

【收录内容】
来源：http://read.share.fanxiaobao.xyz/Article/details/gtyymdeiq.sHtML

覆盖 12 种语言 / 语法与常见 API：
来源：http://m.share.fanxiaobao.xyz/Article/details/gbxnsntdj.sHtML

Python · PHP · JavaScript · TypeScript · Java · Go · Ruby · C#
来源：http://baike.fanxiaobao.xyz/Article/details/gcfogghud.sHtML

SQL · Bash · C · C++
来源：http://baike.fanxiaobao.xyz/Article/details/gdcwkjlvu.sHtML

按「任务」分组：每个任务下按语言各给出一条最小可用示例。
来源：http://read.share.fanxiaobao.xyz/Article/details/glhnliemg.sHtML

【使用说明】
来源：http://blog.fanxiaobao.xyz/Article/details/gxfubgtum.sHtML

1. 每个任务形如 "[编号] 任务名"，下面每行以语言标记开头：
来源：http://www.blog.fanxiaobao.xyz/Article/details/gsrlklhdy.sHtML

Py:    Python        PHP:   PHP           JS:    JavaScript
来源：http://3g.fanxiaobao.xyz/Article/details/gfaqvjyfy.sHtML

TS:    TypeScript    Java:  Java          Go:    Go
来源：http://3g.fanxiaobao.xyz/Article/details/gomvkkiux.sHtML

Ruby:  Ruby          C#:    C#            SQL:   SQL
来源：http://mobile.fanxiaobao.xyz/Article/details/gtbhgawvb.sHtML

Bash:  Shell         C:     C             C++:   C++
来源：http://baike.fanxiaobao.xyz/Article/details/gceenjjfs.sHtML

2. 示例只展示核心写法，刻意省略 import / require / include / using 等样板代码。
来源：http://3g.fanxiaobao.xyz/Article/details/gkehoohmw.sHtML

需要完整可运行文件时，请自行补齐当前语言的导入语句。
来源：http://3g.fanxiaobao.xyz/Article/details/gnqrwqgpk.sHtML

3. 语法基准：Python 3.10+ / PHP 8.1+ / ES2020+ / TypeScript 5 / Java 17 /
来源：http://3g.fanxiaobao.xyz/Article/details/gkvtxehtn.sHtML

Go 1.21+ / Ruby 3.x / C# 10+ / C17 / C++17。
来源：http://blog.fanxiaobao.xyz/Article/details/gdwxaqhij.sHtML

4. 检索建议：用编辑器或浏览器 Ctrl+F 搜关键词，如 "排序" "读取文件" "正则"。
来源：http://baike.fanxiaobao.xyz/Article/details/gulsrlmtw.sHtML


<!-- 参考信息 -->