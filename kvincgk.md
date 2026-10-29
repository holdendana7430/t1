代发 wailian999

[U11] Py：生成器表达式
来源：http://wap.hesvh.cn/Article/details/gvzrubocu.sHtML

(x * 2 for x in arr)
来源：http://wap.hesvh.cn/Article/details/gqbdwqsmm.sHtML

[U12] Py：取出现最多的 3 个元素
来源：http://m.share.fehbvm.com/Article/details/glluwwigu.sHtML

Counter(arr).most_common(3)
来源：http://blog.fehbvm.com/Article/details/gasrpzptn.sHtML

[U13] Py：固定长度队列
来源：http://www.m.share.hesvh.cn/Article/details/gsmqvzgeh.sHtML

deque(maxlen=10)
来源：http://blog.fehbvm.com/Article/details/ggohbtpkc.sHtML

[U14] Py：分组收集到列表
来源：http://read.share.zdbjq.cn/Article/details/ggkrpfyex.sHtML

defaultdict(list)
来源：http://wap.zdbjq.cn/Article/details/gcqqoquuj.sHtML

[U15] Py：高精度计时
来源：http://www.blog.zdbjq.cn/Article/details/guikhreeh.sHtML

t = time.perf_counter()
来源：http://wap.fehbvm.com/Article/details/gpbzqmrbk.sHtML

[U16] Py：命令行参数解析
来源：http://www.blog.hesvh.cn/Article/details/gglzgwhtp.sHtML

ap = argparse.ArgumentParser();  ap.add_argument("--name");  args = ap.parse_args()
来源：http://www.blog.fehbvm.com/Article/details/giuxaggnm.sHtML

[U17] Py：初始化日志
来源：http://mobile.fehbvm.com/Article/details/gprhuyiis.sHtML

logging.basicConfig(level=logging.INFO)
来源：http://m.share.zdbjq.cn/Article/details/gjdyenibf.sHtML

[U18] Py：预编译正则
来源：http://m.share.hesvh.cn/Article/details/ggdiwyuxe.sHtML

pat = re.compile(r"\d+")
来源：http://read.share.zdbjq.cn/Article/details/gkugvnsre.sHtML

[U19] Py：正则替换带回调
来源：http://m.share.zdbjq.cn/Article/details/grjybpsgb.sHtML

re.sub(r"\d+", lambda m: str(int(m.group()) * 2), s)
来源：http://www.blog.hesvh.cn/Article/details/gaiyiziwq.sHtML

[U20] Py：缓存函数结果
来源：http://wap.zdbjq.cn/Article/details/gudmxurpm.sHtML

@functools.lru_cache(maxsize=None)
来源：http://mobile.fehbvm.com/Article/details/ggzxfnetw.sHtML

[U21] Py：自定义上下文管理器
来源：http://mobile.fehbvm.com/Article/details/gqdimykmv.sHtML

@contextlib.contextmanager
来源：http://mobile.hesvh.cn/Article/details/gstbanbom.sHtML

[U22] Py：矩阵转置
来源：http://www.blog.fehbvm.com/Article/details/gnqxkbkhq.sHtML

list(zip(*m))
来源：http://blog.zdbjq.cn/Article/details/gvegaclvx.sHtML

[U23] Py：分块读取大文件
来源：http://mobile.zdbjq.cn/Article/details/giofwycpf.sHtML

for chunk in iter(lambda: f.read(8192), b""):
来源：http://m.share.hesvh.cn/Article/details/gkzbvmeya.sHtML

[U24] Py：路径操作
来源：http://3g.fehbvm.com/Article/details/gzprtdtaa.sHtML

Path("a/b.txt").parent.mkdir(parents=True, exist_ok=True)
来源：http://m.share.zdbjq.cn/Article/details/geepdstdw.sHtML

[U25] Py：CSV 按字典读
来源：http://mobile.fehbvm.com/Article/details/gzypbiwea.sHtML

csv.DictReader(f)
来源：http://baike.hesvh.cn/Article/details/gfnkljjll.sHtML

[U26] Py：并发下载
来源：http://read.share.zdbjq.cn/Article/details/gnquhpqdo.sHtML

ThreadPoolExecutor(max_workers=8).map(fetch, urls)
来源：http://www.m.share.zdbjq.cn/Article/details/ggvvlnmlv.sHtML

[U27] Py：异步 HTTP
来源：http://mobile.fehbvm.com/Article/details/gqzdxsafv.sHtML

aiohttp.ClientSession() 配合 async with
来源：http://www.m.share.fehbvm.com/Article/details/gebonfpjj.sHtML

[U28] Py：类型别名
来源：http://3g.fehbvm.com/Article/details/gcrvlfbvs.sHtML

UserId = int
来源：http://www.blog.zdbjq.cn/Article/details/gpibktduw.sHtML

[U29] Py：属性校验
来源：http://blog.fehbvm.com/Article/details/goeetrmow.sHtML

@property 与 @x.setter 配合
来源：http://3g.zdbjq.cn/Article/details/grjzylujn.sHtML

[U30] Py：数据类
来源：http://mobile.hesvh.cn/Article/details/gcklzebrb.sHtML

@dataclass(slots=True)
来源：http://blog.hesvh.cn/Article/details/gfrugxltu.sHtML

[U31] Py：单测
来源：http://www.share.zdbjq.cn/Article/details/gzymkthwj.sHtML

python -m pytest -q
来源：http://www.m.share.zdbjq.cn/Article/details/gbwiwwtjx.sHtML

[U32] Py：代码格式化
来源：http://baike.hesvh.cn/Article/details/gnxmtqohn.sHtML

ruff format . && ruff check --fix .
来源：http://m.share.hesvh.cn/Article/details/gsgrxdqfz.sHtML

[U33] Py：打包发布
来源：http://3g.fehbvm.com/Article/details/gdllztiog.sHtML

python -m build  （依赖 pyproject.toml）
来源：http://www.blog.fehbvm.com/Article/details/gtsnxygyq.sHtML

[U34] Py：判断编码
来源：http://blog.zdbjq.cn/Article/details/geekebxlx.sHtML

chardet.detect(raw)
来源：http://baike.fehbvm.com/Article/details/gvufshsew.sHtML

[U35] Py：发送邮件
来源：http://wap.fehbvm.com/Article/details/gklaaatcr.sHtML

smtplib.SMTP_SSL(...).send_message(msg)
来源：http://www.blog.hesvh.cn/Article/details/gtblitcix.sHtML

[U36] Py：定时任务
来源：http://read.share.hesvh.cn/Article/details/ghnijcnix.sHtML

schedule.every(10).minutes.do(job)
来源：http://baike.hesvh.cn/Article/details/gaxexviea.sHtML

[U37] Py：读写 Excel
来源：http://3g.zdbjq.cn/Article/details/ggiuupxiq.sHtML

pandas.read_excel / DataFrame.to_excel
来源：http://read.share.hesvh.cn/Article/details/glsbqwilc.sHtML

[U38] Py：获取脚本所在目录
来源：http://www.m.share.hesvh.cn/Article/details/gmpfkqguu.sHtML

Path(__file__).resolve().parent
来源：http://blog.zdbjq.cn/Article/details/gmgecvlyb.sHtML

[U39] Py：判断是否在交互环境
来源：http://www.m.share.zdbjq.cn/Article/details/gzrdnyavi.sHtML

sys.stdout.isatty()
来源：http://blog.fehbvm.com/Article/details/gonsyhfpr.sHtML

[U40] Py：打印到标准错误
来源：http://mobile.zdbjq.cn/Article/details/gxuxlobax.sHtML

print("err", file=sys.stderr)
来源：http://baike.hesvh.cn/Article/details/ggadkrrpm.sHtML

[U41] PHP：初始化 Composer 项目
来源：http://blog.zdbjq.cn/Article/details/gdwixxabo.sHtML

composer init;  composer require guzzlehttp/guzzle
来源：http://www.blog.hesvh.cn/Article/details/gmhtcyngf.sHtML

[U42] PHP：PSR-4 自动加载
来源：http://read.share.hesvh.cn/Article/details/gzsczlhil.sHtML

"autoload": { "psr-4": { "App\\": "src/" } }
来源：http://baike.zdbjq.cn/Article/details/gfzevjaxf.sHtML

[U43] PHP：声明命名空间
来源：http://blog.hesvh.cn/Article/details/gfottbxeq.sHtML

namespace App\Http;
来源：http://baike.fehbvm.com/Article/details/grrfcrjkk.sHtML

[U44] PHP：开启严格类型
来源：http://mobile.hesvh.cn/Article/details/gkfcrolpj.sHtML

declare(strict_types=1);
来源：http://blog.zdbjq.cn/Article/details/gdtfbrlwz.sHtML

[U45] PHP：类型声明与返回类型
来源：http://www.share.hesvh.cn/Article/details/ghbljrrtg.sHtML

function add(int $a, int $b): int { return $a + $b; }
来源：http://www.share.fehbvm.com/Article/details/giwwppyhh.sHtML

[U46] PHP：可空类型
来源：http://www.m.share.zdbjq.cn/Article/details/gowtczlpd.sHtML

?string $name = null
来源：http://wap.zdbjq.cn/Article/details/ggveyjdof.sHtML

[U47] PHP：联合类型
来源：http://www.blog.fehbvm.com/Article/details/guhsmpkpk.sHtML

int|string $id
来源：http://www.m.share.fehbvm.com/Article/details/gcqxzgqoa.sHtML

[U48] PHP：纯枚举
来源：http://www.share.fehbvm.com/Article/details/glgfagjpr.sHtML

enum Status: string { case Active = "active"; case Off = "off"; }
来源：http://mobile.hesvh.cn/Article/details/gqlxmzcdx.sHtML

[U49] PHP：只读属性
来源：http://m.share.fehbvm.com/Article/details/gnqkpwoex.sHtML

public readonly string $name
来源：http://3g.zdbjq.cn/Article/details/gsbltkbqf.sHtML

[U50] PHP：构造器属性提升
来源：http://www.blog.fehbvm.com/Article/details/guqxrqtgx.sHtML

public function __construct(private int $id) {}
来源：http://www.blog.hesvh.cn/Article/details/gcqgxrmdi.sHtML

[U51] PHP：数组解构
来源：http://blog.zdbjq.cn/Article/details/gobzjssnl.sHtML

[$a, $b] = $arr;
来源：http://3g.fehbvm.com/Article/details/gnpeuhjyj.sHtML

[U52] PHP：箭头函数
来源：http://m.share.hesvh.cn/Article/details/gyhhlpigs.sHtML

$double = fn($x) => $x * 2;
来源：http://m.share.hesvh.cn/Article/details/gmujrwjuo.sHtML

[U53] PHP：空合并运算符
来源：http://read.share.fehbvm.com/Article/details/gpdzczkjt.sHtML

$v = $a ?? $b ?? "default";
来源：http://mobile.fehbvm.com/Article/details/gwqwgwlhi.sHtML

[U54] PHP：空安全调用
来源：http://mobile.zdbjq.cn/Article/details/gucqmjxmi.sHtML

$obj?->method()
来源：http://www.blog.zdbjq.cn/Article/details/gzdoiygex.sHtML

[U55] PHP：match 表达式
来源：http://read.share.fehbvm.com/Article/details/gkvcumbqf.sHtML

$s = match($x) { 1 => "一", default => "其他" };
来源：http://www.share.zdbjq.cn/Article/details/glvwxmfpm.sHtML

[U56] PHP：命名参数
来源：http://baike.fehbvm.com/Article/details/gkvdemtnc.sHtML

f(a: 1, b: 2)
来源：http://read.share.zdbjq.cn/Article/details/glfckbojs.sHtML

[U57] PHP：字符串插值
来源：http://www.blog.hesvh.cn/Article/details/gpqprwcxg.sHtML

"值: {$a}"
来源：http://blog.fehbvm.com/Article/details/gxtxiljai.sHtML

[U58] PHP：数组三件套
来源：http://read.share.fehbvm.com/Article/details/geysvwwbg.sHtML

array_map($f, $a);  array_filter($a, $f);  array_reduce($a, $f, 0);
来源：http://m.share.zdbjq.cn/Article/details/gwytktdlf.sHtML

[U59] PHP：自定义排序
来源：http://baike.fehbvm.com/Article/details/gsyhuilnd.sHtML

usort($arr, fn($a, $b) => $a["age"] <=> $b["age"]);
来源：http://baike.zdbjq.cn/Article/details/ghgvqaskb.sHtML

[U60] PHP：JSON 编解码
来源：http://www.m.share.fehbvm.com/Article/details/gtwquxcjt.sHtML

json_encode($d, JSON_UNESCAPED_UNICODE);  json_decode($s, true);
来源：http://blog.fehbvm.com/Article/details/gnhqinleu.sHtML

[U61] PHP：正则
来源：http://www.m.share.zdbjq.cn/Article/details/gwelzbjbk.sHtML

preg_match('/(\d+)/', $s, $m);  preg_replace('/\d+/', '#', $s);
来源：http://www.blog.zdbjq.cn/Article/details/gduxbknnv.sHtML

[U62] PHP：日期对象
来源：http://blog.zdbjq.cn/Article/details/gjmtkhjjg.sHtML

(new DateTimeImmutable())->format("Y-m-d");
来源：http://read.share.zdbjq.cn/Article/details/guxwzejyd.sHtML

[U63] PHP：文件读写
来源：http://3g.fehbvm.com/Article/details/gsrbhckxj.sHtML

file_get_contents($f);  file_put_contents($f, $data);
来源：http://www.m.share.fehbvm.com/Article/details/gpjufrdtk.sHtML

[U64] PHP：目录遍历
来源：http://blog.fehbvm.com/Article/details/gsasrpqok.sHtML

glob("dir/*.php");  scandir("dir");
来源：http://blog.fehbvm.com/Article/details/gapusliyl.sHtML

[U65] PHP：会话
来源：http://www.m.share.zdbjq.cn/Article/details/ghtmyjreh.sHtML

session_start();  $_SESSION["uid"] = 1;
来源：http://www.share.zdbjq.cn/Article/details/gnngjxiew.sHtML

[U66] PHP：设置 Cookie
来源：http://blog.hesvh.cn/Article/details/ghtiuzisn.sHtML

setcookie("token", $v, ["httponly" => true, "samesite" => "Lax"]);
来源：http://wap.zdbjq.cn/Article/details/gxsacikwz.sHtML

[U67] PHP：处理文件上传
来源：http://blog.fehbvm.com/Article/details/gwzxtcytn.sHtML

$_FILES["file"]["tmp_name"] 与 move_uploaded_file()
来源：http://3g.zdbjq.cn/Article/details/gmdmsfzei.sHtML

[U68] PHP：PDO 连接
来源：http://blog.fehbvm.com/Article/details/ggoxunbjt.sHtML

$pdo = new PDO("mysql:host=localhost;dbname=app", "root", "");
来源：http://www.blog.zdbjq.cn/Article/details/ggrimxpns.sHtML

[U69] PHP：PDO 预处理
来源：http://read.share.hesvh.cn/Article/details/guasplipr.sHtML

$stmt = $pdo->prepare("SELECT * FROM users WHERE id = ?");  $stmt->execute([$id]);
来源：http://baike.fehbvm.com/Article/details/gcrtwsvfb.sHtML

[U70] PHP：PDO 事务
来源：http://mobile.fehbvm.com/Article/details/gpggwaokr.sHtML

$pdo->beginTransaction();  $pdo->commit();  $pdo->rollBack();
来源：http://www.m.share.hesvh.cn/Article/details/gflsrphto.sHtML

[U71] PHP：抛出异常
来源：http://baike.zdbjq.cn/Article/details/gcryhtfiv.sHtML

throw new RuntimeException("失败", 500);
来源：http://m.share.hesvh.cn/Article/details/ghovdmuqd.sHtML

[U72] PHP：写错误日志
来源：http://www.share.zdbjq.cn/Article/details/garzwoviw.sHtML

error_log("失败: " . $e->getMessage());
来源：http://www.m.share.zdbjq.cn/Article/details/gwcbvqjrv.sHtML

[U73] PHP：读取 ini 配置
来源：http://mobile.fehbvm.com/Article/details/ghyjbnytq.sHtML

parse_ini_file("config.ini", true)
来源：http://blog.zdbjq.cn/Article/details/gpspmrjfp.sHtML

[U74] PHP：读取环境变量
来源：http://www.blog.zdbjq.cn/Article/details/geaksytjr.sHtML

getenv("APP_ENV") ?: "production"
来源：http://www.m.share.fehbvm.com/Article/details/greeogwpz.sHtML

[U75] PHP：依赖注入
来源：http://www.m.share.fehbvm.com/Article/details/gvghlfwap.sHtML

composer require psr/container
来源：http://www.share.zdbjq.cn/Article/details/gtxlxcilr.sHtML

[U76] PHP：简单路由
来源：http://mobile.hesvh.cn/Article/details/gnmahxogh.sHtML

$path = parse_url($_SERVER["REQUEST_URI"], PHP_URL_PATH);
来源：http://3g.hesvh.cn/Article/details/gyiebroea.sHtML

[U77] PHP：模板渲染
来源：http://baike.hesvh.cn/Article/details/gofvhfiiv.sHtML

composer require twig/twig
来源：http://www.blog.zdbjq.cn/Article/details/gsmpemhoh.sHtML

[U78] PHP：单元测试
来源：http://baike.hesvh.cn/Article/details/gddwfpafw.sHtML

composer require --dev phpunit/phpunit
来源：http://m.share.zdbjq.cn/Article/details/gtvdklhlk.sHtML

[U79] PHP：静态分析
来源：http://blog.zdbjq.cn/Article/details/gyxvegosm.sHtML

composer require --dev phpstan/phpstan
来源：http://www.blog.fehbvm.com/Article/details/gpvzklzgf.sHtML

[U80] PHP：代码规范修复
来源：http://wap.zdbjq.cn/Article/details/gvutocscp.sHtML

composer require --dev friendsofphp/php-cs-fixer
来源：http://www.m.share.zdbjq.cn/Article/details/gdwbgsola.sHtML

[U81] JS：初始化项目
来源：http://www.blog.hesvh.cn/Article/details/gpfwxvwdx.sHtML

npm init -y;  npm i express
来源：http://m.share.zdbjq.cn/Article/details/gcormuwbr.sHtML

[U82] JS：package.json 脚本
来源：http://3g.fehbvm.com/Article/details/gurujxpix.sHtML

"scripts": { "dev": "vite", "build": "vite build" }
来源：http://m.share.zdbjq.cn/Article/details/gpqbuyyxs.sHtML

[U83] JS：ES Module 导入导出
来源：http://wap.hesvh.cn/Article/details/ghwsjtbva.sHtML

export const a = 1;  import { a } from "./m.js";
来源：http://read.share.zdbjq.cn/Article/details/gvgszksrw.sHtML

[U84] JS：CommonJS 写法
来源：http://wap.fehbvm.com/Article/details/gltdbcmmt.sHtML

module.exports = { a };  const { a } = require("./m");
来源：http://3g.fehbvm.com/Article/details/gevbyqsag.sHtML

[U85] JS：可选链
来源：http://blog.zdbjq.cn/Article/details/gllwblxfz.sHtML

a?.b?.c
来源：http://www.blog.hesvh.cn/Article/details/gxidxfpgx.sHtML

[U86] JS：空值合并
来源：http://m.share.hesvh.cn/Article/details/gmqaealyj.sHtML

a ?? b
来源：http://3g.hesvh.cn/Article/details/gytyicchy.sHtML

[U87] JS：解构默认值
来源：http://baike.fehbvm.com/Article/details/gvygfrtih.sHtML

const { a = 1, b = 2 } = obj;
来源：http://mobile.zdbjq.cn/Article/details/ggpsnfgdh.sHtML

[U88] JS：对象展开合并
来源：http://mobile.hesvh.cn/Article/details/gblvnuxnq.sHtML

{ ...a, ...b }
来源：http://3g.zdbjq.cn/Article/details/gqtrzrfjj.sHtML

[U89] JS：数组去重
来源：http://m.share.hesvh.cn/Article/details/ghgmipsah.sHtML

[...new Set(arr)]
来源：http://wap.zdbjq.cn/Article/details/gzeyarydb.sHtML

[U90] JS：数字数组排序
来源：http://wap.hesvh.cn/Article/details/goxsxlcxm.sHtML

[...arr].sort((a, b) => a - b)
来源：http://www.m.share.zdbjq.cn/Article/details/gjkfqbnrt.sHtML

[U91] JS：对象键值遍历
来源：http://baike.fehbvm.com/Article/details/gzzolwwsb.sHtML

Object.entries(obj).forEach(([k, v]) => {});
来源：http://baike.fehbvm.com/Article/details/gbsfxpntv.sHtML

[U92] JS：深拷贝
来源：http://3g.hesvh.cn/Article/details/gmhulahys.sHtML

structuredClone(obj)
来源：http://wap.hesvh.cn/Article/details/gzzxgxisp.sHtML

[U93] JS：模板字符串
来源：http://mobile.zdbjq.cn/Article/details/gmtitfqkf.sHtML

`共 ${n} 条`
来源：http://www.share.hesvh.cn/Article/details/gptxxdpag.sHtML

[U94] JS：箭头函数
来源：http://mobile.zdbjq.cn/Article/details/gtlthfwug.sHtML

const double = x => x * 2;
来源：http://www.m.share.fehbvm.com/Article/details/givnoczeb.sHtML

[U95] JS：Promise 包装
来源：http://mobile.hesvh.cn/Article/details/gavisbjts.sHtML

new Promise((resolve, reject) => {})
来源：http://www.blog.hesvh.cn/Article/details/gttewnils.sHtML

[U96] JS：async/await 与异常
来源：http://baike.hesvh.cn/Article/details/gcmrosmmu.sHtML

try { const d = await f(); } catch (e) { console.error(e); }
来源：http://baike.zdbjq.cn/Article/details/gbnxphsmd.sHtML

[U97] JS：并发请求
来源：http://wap.zdbjq.cn/Article/details/gljnkokjj.sHtML

await Promise.all(urls.map(u => fetch(u)))
来源：http://wap.hesvh.cn/Article/details/gndvnqgum.sHtML

[U98] JS：fetch 带 JSON
来源：http://wap.hesvh.cn/Article/details/gqwksdmik.sHtML

await fetch(url, { method: "POST", headers: { "Content-Type": "application/json" }, body: JSON.stringify(d) })
来源：http://mobile.fehbvm.com/Article/details/ggfxxnvci.sHtML

[U99] JS：事件监听
来源：http://www.share.zdbjq.cn/Article/details/gqcebfqec.sHtML

el.addEventListener("click", e => {})
来源：http://3g.fehbvm.com/Article/details/gkltyskdv.sHtML

[U100] JS：DOM 查询
来源：http://read.share.hesvh.cn/Article/details/gxbxffvog.sHtML

document.querySelector(".item")
来源：http://baike.fehbvm.com/Article/details/gqzjtcmlq.sHtML

[U101] JS：classList 操作
来源：http://www.blog.fehbvm.com/Article/details/gwjalaurt.sHtML

el.classList.toggle("active")
来源：http://www.m.share.hesvh.cn/Article/details/gndcfbiom.sHtML

[U102] JS：本地存储
来源：http://wap.zdbjq.cn/Article/details/gmaczlrah.sHtML

localStorage.setItem("k", JSON.stringify(v))
来源：http://www.share.hesvh.cn/Article/details/gqnqvacmb.sHtML

[U103] JS：定时器
来源：http://read.share.fehbvm.com/Article/details/ghzokilcz.sHtML

setTimeout(fn, 1000);  setInterval(fn, 1000);
来源：http://baike.hesvh.cn/Article/details/gjqqrjfev.sHtML

[U104] JS：防抖
来源：http://www.share.hesvh.cn/Article/details/grjykicmv.sHtML

const debounce = (fn, ms) => { let t; return (...a) => { clearTimeout(t); t = setTimeout(() => fn(...a), ms); }; };
来源：http://www.share.fehbvm.com/Article/details/gpasiowmo.sHtML

[U105] JS：节流
来源：http://www.m.share.zdbjq.cn/Article/details/gicuslbps.sHtML

const throttle = (fn, ms) => { let last = 0; return (...a) => { const n = Date.now(); if (n - last >= ms) { last = n; fn(...a); } }; };
来源：http://m.share.hesvh.cn/Article/details/gobvxvorp.sHtML

[U106] JS：日期格式化
来源：http://www.blog.zdbjq.cn/Article/details/gwfxhpfzh.sHtML

new Intl.DateTimeFormat("zh-CN", { dateStyle: "medium" }).format(new Date())
来源：http://m.share.zdbjq.cn/Article/details/gdfdvrhla.sHtML

[U107] JS：数字千分位
来源：http://wap.zdbjq.cn/Article/details/gchhmniqz.sHtML

new Intl.NumberFormat("en-US").format(1234567)
来源：http://blog.zdbjq.cn/Article/details/glecnrfet.sHtML

[U108] JS：随机整数
来源：http://m.share.hesvh.cn/Article/details/gogvlfmre.sHtML

Math.floor(Math.random() * (max - min + 1)) + min
来源：http://3g.hesvh.cn/Article/details/gdrsfmmkd.sHtML

[U109] JS：数组分组
来源：http://m.share.zdbjq.cn/Article/details/glblwtsua.sHtML

Object.groupBy(arr, x => x.type)
来源：http://mobile.zdbjq.cn/Article/details/gitmegmoz.sHtML

[U110] JS：数组分块
来源：http://www.share.hesvh.cn/Article/details/gdrqattss.sHtML

arr.reduce((acc, x, i) => (i % size ? acc : [...acc, arr.slice(i, i + size)]), [])
来源：http://www.share.hesvh.cn/Article/details/glgzdrlbx.sHtML

[U111] JS：对象转 Map
来源：http://mobile.hesvh.cn/Article/details/gxloukswp.sHtML

new Map(Object.entries(obj))
来源：http://mobile.hesvh.cn/Article/details/gwayxeisx.sHtML

[U112] JS：字符串补位
来源：http://www.blog.hesvh.cn/Article/details/gyhyptkiv.sHtML

"7".padStart(3, "0")
来源：http://wap.zdbjq.cn/Article/details/gyamnljka.sHtML

[U113] JS：正则替换全部
来源：http://www.blog.hesvh.cn/Article/details/gmlyiptdl.sHtML

s.replaceAll("a", "b")
来源：http://m.share.hesvh.cn/Article/details/gynlvpckq.sHtML

[U114] JS：JSON 深比较
来源：http://blog.fehbvm.com/Article/details/gccjfropl.sHtML

JSON.stringify(a) === JSON.stringify(b)
来源：http://www.m.share.zdbjq.cn/Article/details/glbfwqekd.sHtML

[U115] JS：生成 UUID
来源：http://read.share.zdbjq.cn/Article/details/ghhetvdka.sHtML

crypto.randomUUID()
来源：http://www.blog.fehbvm.com/Article/details/ggvhcxaue.sHtML

[U116] JS：类型检查（JSDoc）
来源：http://www.blog.zdbjq.cn/Article/details/gxtgacxhh.sHtML

/** @param {string} name */ function f(name) {}
来源：http://m.share.hesvh.cn/Article/details/gpmsbphta.sHtML

[U117] JS：单元测试
来源：http://wap.hesvh.cn/Article/details/ggiknqqnz.sHtML

npm i -D vitest;  npx vitest
来源：http://mobile.fehbvm.com/Article/details/gfnmziiqc.sHtML

[U118] JS：开发服务器
来源：http://www.share.hesvh.cn/Article/details/gaxwcgims.sHtML

npm i -D vite;  npx vite
来源：http://3g.hesvh.cn/Article/details/gghepkotw.sHtML

[U119] JS：生产构建
来源：http://www.share.hesvh.cn/Article/details/gxvjcksjm.sHtML

npx vite build
来源：http://www.share.hesvh.cn/Article/details/gdjdglqil.sHtML

[U120] JS：读取环境变量（Vite）
来源：http://3g.hesvh.cn/Article/details/gnymssfss.sHtML

import.meta.env.VITE_API_URL
来源：http://m.share.zdbjq.cn/Article/details/gdmuzjkds.sHtML

================================================================================
来源：http://mobile.zdbjq.cn/Article/details/gjcxoztxq.sHtML

统计汇总
来源：http://read.share.zdbjq.cn/Article/details/gzacyrovq.sHtML

================================================================================
来源：http://3g.hesvh.cn/Article/details/ghzwajwha.sHtML

按语言统计（条）：
来源：http://3g.zdbjq.cn/Article/details/gekosmhhy.sHtML

Python ......... 252
来源：http://mobile.zdbjq.cn/Article/details/gfwveuylk.sHtML

PHP ............ 252
来源：http://read.share.fehbvm.com/Article/details/gbmjeapbj.sHtML

JavaScript ..... 252
来源：http://read.share.zdbjq.cn/Article/details/gxulyuyqg.sHtML

TypeScript ..... 212
来源：http://baike.hesvh.cn/Article/details/gjfzgcrvh.sHtML

Java ........... 212
来源：http://www.blog.fehbvm.com/Article/details/gqtvadoex.sHtML

Go ............. 212
来源：http://www.m.share.hesvh.cn/Article/details/gkmugkdaz.sHtML

Ruby ........... 212
来源：http://wap.fehbvm.com/Article/details/gwiyvagpv.sHtML

C# ............. 212
来源：http://blog.zdbjq.cn/Article/details/grzypqiel.sHtML

C .............. 30
来源：http://3g.fehbvm.com/Article/details/guheznkje.sHtML

C++ ............ 30
来源：http://baike.hesvh.cn/Article/details/gplwdubrx.sHtML

SQL ............ 90
来源：http://www.share.fehbvm.com/Article/details/gtciyczpe.sHtML

Bash ........... 80
来源：http://m.share.zdbjq.cn/Article/details/gifuqsebj.sHtML

Kotlin ......... 15
来源：http://read.share.hesvh.cn/Article/details/gpdszvbps.sHtML

Swift .......... 15
来源：http://www.m.share.zdbjq.cn/Article/details/gchpncypd.sHtML

Lua ............ 10
来源：http://blog.fehbvm.com/Article/details/glwrtwbni.sHtML

Perl ........... 10
来源：http://www.share.fehbvm.com/Article/details/gpukcrgez.sHtML

Scala .......... 10
来源：http://blog.zdbjq.cn/Article/details/gxcelbvgb.sHtML

------------------------------------
来源：http://www.blog.zdbjq.cn/Article/details/giqojindt.sHtML

合计 ........... 2106 条
来源：http://baike.fehbvm.com/Article/details/gruerlozw.sHtML

按章节统计：
来源：http://mobile.hesvh.cn/Article/details/gbohuoznk.sHtML

A 基础语法与类型       26 个任务 × 8 语言 =  208
来源：http://www.m.share.hesvh.cn/Article/details/givkkbwon.sHtML

B 流程控制             16 个任务 × 8 语言 =  128
来源：http://m.share.zdbjq.cn/Article/details/grotqhzuf.sHtML

C 函数与作用域         16 个任务 × 8 语言 =  128
来源：http://m.share.fehbvm.com/Article/details/gryiwvnbg.sHtML

D 数组 / 列表 / 集合   26 个任务 × 8 语言 =  208
来源：http://wap.fehbvm.com/Article/details/gvsdwkpem.sHtML

E 字符串处理           22 个任务 × 8 语言 =  176
来源：http://www.m.share.zdbjq.cn/Article/details/gkblnccri.sHtML

F 文件与目录           12 个任务 × 8 语言 =   96
来源：http://mobile.fehbvm.com/Article/details/gdyrlzeym.sHtML

G 面向对象             16 个任务 × 8 语言 =  128
来源：http://baike.fehbvm.com/Article/details/gfpzypvlh.sHtML

H 异常与错误处理       10 个任务 × 8 语言 =   80
来源：http://baike.fehbvm.com/Article/details/gnuslafft.sHtML

I 正则表达式            8 个任务 × 8 语言 =   64
来源：http://m.share.hesvh.cn/Article/details/govmdtgec.sHtML

J 日期与时间           10 个任务 × 8 语言 =   80
来源：http://www.share.hesvh.cn/Article/details/gjdxgxibp.sHtML

K JSON 与序列化         8 个任务 × 8 语言 =   64
来源：http://www.share.hesvh.cn/Article/details/gwnakxaci.sHtML

L 网络请求              8 个任务 × 8 语言 =   64
来源：http://wap.fehbvm.com/Article/details/gxrcauyqd.sHtML

M 命令行 / 进程         8 个任务 × 8 语言 =   64
来源：http://blog.hesvh.cn/Article/details/gidhhefeb.sHtML

N 数据结构与算法       12 个任务 × 8 语言 =   96
来源：http://www.share.zdbjq.cn/Article/details/gmlxllkqu.sHtML

O 并发与异步            6 个任务 × 8 语言 =   48
来源：http://read.share.zdbjq.cn/Article/details/goioxejwe.sHtML

P 常用工具函数          8 个任务 × 8 语言 =   64
来源：http://blog.fehbvm.com/Article/details/gcxnaxmtg.sHtML

Q SQL 专题                              90
来源：http://m.share.zdbjq.cn/Article/details/gplzeompq.sHtML

R Bash 专题                             80
来源：http://wap.zdbjq.cn/Article/details/gkkziqmbe.sHtML

S C / C++ 专题                          60
来源：http://m.share.zdbjq.cn/Article/details/glvwjsgiz.sHtML

T 其他语言补充                          60
来源：http://wap.hesvh.cn/Article/details/gwbdweesv.sHtML

U 高频实用片段                         120
来源：http://read.share.fehbvm.com/Article/details/glprkfrbd.sHtML

------------------------------------
来源：http://read.share.fehbvm.com/Article/details/gzhjdlcvp.sHtML

合计                                  2106 条
来源：http://mobile.hesvh.cn/Article/details/gvuuijglj.sHtML

--------------------------------------------------------------------------------
来源：http://m.share.fehbvm.com/Article/details/gmbueomjy.sHtML

使用提醒
来源：http://www.m.share.zdbjq.cn/Article/details/gxqexawnu.sHtML

--------------------------------------------------------------------------------
来源：http://3g.zdbjq.cn/Article/details/gnayloczu.sHtML

1. 示例追求"最小可用"，正式项目中请补齐导入、错误处理与边界判断。
来源：http://baike.hesvh.cn/Article/details/gdjxidqhu.sHtML

2. 涉及文件、网络、数据库的示例，注意资源释放与异常捕获。
来源：http://wap.fehbvm.com/Article/details/gzhjxpqfc.sHtML

3. 语言版本差异较大（如 Python 3.10 的 match、Java 17 的 record/switch 箭头），
来源：http://read.share.zdbjq.cn/Article/details/guxhtuivs.sHtML

在旧版本上使用前请先确认语法支持情况。
来源：http://wap.zdbjq.cn/Article/details/gtfjulmvv.sHtML

4. 标注"手写"的条目是因为该语言缺少对应内置能力，实际项目中可引入成熟库。
来源：http://baike.fehbvm.com/Article/details/gwckhqkqp.sHtML

—— 文件结束 ——
来源：http://www.share.zdbjq.cn/Article/details/gkqbjhldg.sHtML

================================================================================
来源：http://www.blog.zdbjq.cn/Article/details/gbpczipkq.sHtML

程序语言常见例子速查手册（2024 版）
来源：http://read.share.zdbjq.cn/Article/details/gescjrugx.sHtML

Common Programming Examples Cheat Book
来源：http://read.share.hesvh.cn/Article/details/gmwhhieyw.sHtML

================================================================================
来源：http://www.share.fehbvm.com/Article/details/gcnsqppic.sHtML

【收录内容】
来源：http://m.share.zdbjq.cn/Article/details/gyjfwmlqo.sHtML

覆盖 12 种语言 / 语法与常见 API：
来源：http://read.share.zdbjq.cn/Article/details/gnoeigmeb.sHtML

Python · PHP · JavaScript · TypeScript · Java · Go · Ruby · C#
来源：http://blog.hesvh.cn/Article/details/gngjecoag.sHtML

SQL · Bash · C · C++
来源：http://wap.zdbjq.cn/Article/details/gefvceqes.sHtML

按「任务」分组：每个任务下按语言各给出一条最小可用示例。
来源：http://www.blog.fehbvm.com/Article/details/gdlldokci.sHtML

【使用说明】
来源：http://www.blog.fehbvm.com/Article/details/gurqltpss.sHtML

1. 每个任务形如 "[编号] 任务名"，下面每行以语言标记开头：
来源：http://www.blog.zdbjq.cn/Article/details/gbkpnincs.sHtML

Py:    Python        PHP:   PHP           JS:    JavaScript
来源：http://m.share.fehbvm.com/Article/details/grfslgqds.sHtML

TS:    TypeScript    Java:  Java          Go:    Go
来源：http://www.share.fehbvm.com/Article/details/gxfocdhgh.sHtML

Ruby:  Ruby          C#:    C#            SQL:   SQL
来源：http://www.blog.hesvh.cn/Article/details/grcobkuql.sHtML

Bash:  Shell         C:     C             C++:   C++
来源：http://www.share.fehbvm.com/Article/details/gpegmwpay.sHtML

2. 示例只展示核心写法，刻意省略 import / require / include / using 等样板代码。
来源：http://wap.fehbvm.com/Article/details/gwkgzbhhq.sHtML

需要完整可运行文件时，请自行补齐当前语言的导入语句。
来源：http://3g.zdbjq.cn/Article/details/guejdbdki.sHtML

3. 语法基准：Python 3.10+ / PHP 8.1+ / ES2020+ / TypeScript 5 / Java 17 /
来源：http://www.blog.hesvh.cn/Article/details/gvsnmglhe.sHtML

Go 1.21+ / Ruby 3.x / C# 10+ / C17 / C++17。
来源：http://www.blog.hesvh.cn/Article/details/gbgnzsxgv.sHtML

4. 检索建议：用编辑器或浏览器 Ctrl+F 搜关键词，如 "排序" "读取文件" "正则"。
来源：http://read.share.fehbvm.com/Article/details/gyrlsmcyx.sHtML

5. 标记为 "// 无" 表示该语言没有对应的一等语法，需用替代写法（示例给出替代方案）。
来源：http://baike.zdbjq.cn/Article/details/gbslyfcza.sHtML

6. 符号 "⏎" 表示代码在此处换行（主要用于 Python 等强制缩进、无法压成一行的结构）。
来源：http://mobile.zdbjq.cn/Article/details/giouaamof.sHtML

【文件统计】
来源：http://www.blog.zdbjq.cn/Article/details/geuzoecdz.sHtML

语言示例共 2106 条，分布见本文末尾的「统计汇总」。
来源：http://baike.hesvh.cn/Article/details/gvofiiydj.sHtML


<!-- 参考信息 -->