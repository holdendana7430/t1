代发 wailian999

[U15] Py：高精度计时
来源：http://3g.zdbjq.cn/Article/details/gifglgtjv.sHtML

t = time.perf_counter()
来源：http://www.share.zdbjq.cn/Article/details/gosymlpdk.sHtML

[U16] Py：命令行参数解析
来源：http://read.share.hesvh.cn/Article/details/gzgvrrmcl.sHtML

ap = argparse.ArgumentParser();  ap.add_argument("--name");  args = ap.parse_args()
来源：http://www.blog.hesvh.cn/Article/details/gpbzegrjk.sHtML

[U17] Py：初始化日志
来源：http://www.share.zdbjq.cn/Article/details/ghjxgeaqk.sHtML

logging.basicConfig(level=logging.INFO)
来源：http://www.blog.zdbjq.cn/Article/details/ggbtquiai.sHtML

[U18] Py：预编译正则
来源：http://read.share.hesvh.cn/Article/details/gdbhiwhzx.sHtML

pat = re.compile(r"\d+")
来源：http://www.m.share.fehbvm.com/Article/details/gemeuxjns.sHtML

[U19] Py：正则替换带回调
来源：http://baike.fehbvm.com/Article/details/gxuinnoge.sHtML

re.sub(r"\d+", lambda m: str(int(m.group()) * 2), s)
来源：http://www.blog.fehbvm.com/Article/details/gneanqatu.sHtML

[U20] Py：缓存函数结果
来源：http://www.blog.fehbvm.com/Article/details/gsjyumakv.sHtML

@functools.lru_cache(maxsize=None)
来源：http://www.share.fehbvm.com/Article/details/gznyxzjki.sHtML

[U21] Py：自定义上下文管理器
来源：http://blog.zdbjq.cn/Article/details/giyuzjcem.sHtML

@contextlib.contextmanager
来源：http://read.share.hesvh.cn/Article/details/ghpuoesvh.sHtML

[U22] Py：矩阵转置
来源：http://read.share.fehbvm.com/Article/details/gkhppmhzk.sHtML

list(zip(*m))
来源：http://www.m.share.zdbjq.cn/Article/details/gnytnrtwq.sHtML

[U23] Py：分块读取大文件
来源：http://3g.fehbvm.com/Article/details/gahmbzzyb.sHtML

for chunk in iter(lambda: f.read(8192), b""):
来源：http://www.blog.hesvh.cn/Article/details/gjjbbqwip.sHtML

[U24] Py：路径操作
来源：http://baike.zdbjq.cn/Article/details/ghzhsglac.sHtML

Path("a/b.txt").parent.mkdir(parents=True, exist_ok=True)
来源：http://3g.fehbvm.com/Article/details/gwjlctfdx.sHtML

[U25] Py：CSV 按字典读
来源：http://wap.fehbvm.com/Article/details/ghxddhfss.sHtML

csv.DictReader(f)
来源：http://mobile.zdbjq.cn/Article/details/gwveuhmes.sHtML

[U26] Py：并发下载
来源：http://www.m.share.hesvh.cn/Article/details/guvyhpwwe.sHtML

ThreadPoolExecutor(max_workers=8).map(fetch, urls)
来源：http://www.m.share.hesvh.cn/Article/details/grqcwxmxq.sHtML

[U27] Py：异步 HTTP
来源：http://wap.hesvh.cn/Article/details/grdtbsiie.sHtML

aiohttp.ClientSession() 配合 async with
来源：http://www.m.share.hesvh.cn/Article/details/gxlsoarhn.sHtML

[U28] Py：类型别名
来源：http://m.share.hesvh.cn/Article/details/gvpmxqpdv.sHtML

UserId = int
来源：http://baike.fehbvm.com/Article/details/gqqiufgyv.sHtML

[U29] Py：属性校验
来源：http://www.m.share.zdbjq.cn/Article/details/gbcgpkdfw.sHtML

@property 与 @x.setter 配合
来源：http://m.share.fehbvm.com/Article/details/gstksicwt.sHtML

[U30] Py：数据类
来源：http://blog.fehbvm.com/Article/details/gprwcrdxh.sHtML

@dataclass(slots=True)
来源：http://baike.fehbvm.com/Article/details/grmlrgvpa.sHtML

[U31] Py：单测
来源：http://www.blog.fehbvm.com/Article/details/gjqvfbwcw.sHtML

python -m pytest -q
来源：http://blog.fehbvm.com/Article/details/gbtwcurvd.sHtML

[U32] Py：代码格式化
来源：http://wap.hesvh.cn/Article/details/gtzkprylq.sHtML

ruff format . && ruff check --fix .
来源：http://read.share.hesvh.cn/Article/details/gelfmngzt.sHtML

[U33] Py：打包发布
来源：http://blog.hesvh.cn/Article/details/gtgunqxui.sHtML

python -m build  （依赖 pyproject.toml）
来源：http://www.m.share.fehbvm.com/Article/details/gnwtfeqjk.sHtML

[U34] Py：判断编码
来源：http://blog.fehbvm.com/Article/details/gyuqezuxi.sHtML

chardet.detect(raw)
来源：http://baike.hesvh.cn/Article/details/gwyqkqmsz.sHtML

[U35] Py：发送邮件
来源：http://blog.zdbjq.cn/Article/details/gaesmlgpr.sHtML

smtplib.SMTP_SSL(...).send_message(msg)
来源：http://read.share.hesvh.cn/Article/details/guagemdmj.sHtML

[U36] Py：定时任务
来源：http://3g.fehbvm.com/Article/details/gyaitatxw.sHtML

schedule.every(10).minutes.do(job)
来源：http://www.share.zdbjq.cn/Article/details/gvkbvvzdg.sHtML

[U37] Py：读写 Excel
来源：http://www.m.share.fehbvm.com/Article/details/gkvrxpzqc.sHtML

pandas.read_excel / DataFrame.to_excel
来源：http://mobile.fehbvm.com/Article/details/geedzlprq.sHtML

[U38] Py：获取脚本所在目录
来源：http://m.share.zdbjq.cn/Article/details/gmcomtdma.sHtML

Path(__file__).resolve().parent
来源：http://mobile.zdbjq.cn/Article/details/genyesonj.sHtML

[U39] Py：判断是否在交互环境
来源：http://wap.zdbjq.cn/Article/details/gwndmtsfj.sHtML

sys.stdout.isatty()
来源：http://m.share.zdbjq.cn/Article/details/ghjlcuhap.sHtML

[U40] Py：打印到标准错误
来源：http://www.m.share.zdbjq.cn/Article/details/ggxowbnyg.sHtML

print("err", file=sys.stderr)
来源：http://baike.zdbjq.cn/Article/details/gynoutgtb.sHtML

[U41] PHP：初始化 Composer 项目
来源：http://www.share.zdbjq.cn/Article/details/ghppzgypw.sHtML

composer init;  composer require guzzlehttp/guzzle
来源：http://blog.fehbvm.com/Article/details/gzupeksrw.sHtML

[U42] PHP：PSR-4 自动加载
来源：http://blog.zdbjq.cn/Article/details/geeyhksqj.sHtML

"autoload": { "psr-4": { "App\\": "src/" } }
来源：http://baike.fehbvm.com/Article/details/gdlyyptxl.sHtML

[U43] PHP：声明命名空间
来源：http://www.m.share.fehbvm.com/Article/details/gmwhlqbkb.sHtML

namespace App\Http;
来源：http://mobile.zdbjq.cn/Article/details/ghfvedaex.sHtML

[U44] PHP：开启严格类型
来源：http://baike.fehbvm.com/Article/details/gbpftcsls.sHtML

declare(strict_types=1);
来源：http://mobile.hesvh.cn/Article/details/ggnykrhgh.sHtML

[U45] PHP：类型声明与返回类型
来源：http://www.blog.zdbjq.cn/Article/details/grelmxhys.sHtML

function add(int $a, int $b): int { return $a + $b; }
来源：http://3g.zdbjq.cn/Article/details/gwfsojbui.sHtML

[U46] PHP：可空类型
来源：http://m.share.fehbvm.com/Article/details/gmercbreq.sHtML

?string $name = null
来源：http://m.share.zdbjq.cn/Article/details/gngfbbgzk.sHtML

[U47] PHP：联合类型
来源：http://3g.hesvh.cn/Article/details/gpiqtowjh.sHtML

int|string $id
来源：http://blog.hesvh.cn/Article/details/gfqgxooth.sHtML

[U48] PHP：纯枚举
来源：http://www.blog.fehbvm.com/Article/details/gujloqxix.sHtML

enum Status: string { case Active = "active"; case Off = "off"; }
来源：http://3g.fehbvm.com/Article/details/gomlubstz.sHtML

[U49] PHP：只读属性
来源：http://mobile.zdbjq.cn/Article/details/gixbopouv.sHtML

public readonly string $name
来源：http://m.share.zdbjq.cn/Article/details/gfcmlthcu.sHtML

[U50] PHP：构造器属性提升
来源：http://baike.hesvh.cn/Article/details/guqtfuqpd.sHtML

public function __construct(private int $id) {}
来源：http://wap.hesvh.cn/Article/details/gqhucipqz.sHtML

[U51] PHP：数组解构
来源：http://m.share.fehbvm.com/Article/details/gdgowgesw.sHtML

[$a, $b] = $arr;
来源：http://wap.hesvh.cn/Article/details/gfjspvpcm.sHtML

[U52] PHP：箭头函数
来源：http://mobile.zdbjq.cn/Article/details/gnaxdxbqn.sHtML

$double = fn($x) => $x * 2;
来源：http://read.share.zdbjq.cn/Article/details/gpgzelxid.sHtML

[U53] PHP：空合并运算符
来源：http://www.blog.zdbjq.cn/Article/details/gpaszcice.sHtML

$v = $a ?? $b ?? "default";
来源：http://www.blog.fehbvm.com/Article/details/gtkogkvvm.sHtML

[U54] PHP：空安全调用
来源：http://wap.fehbvm.com/Article/details/gctikcuhb.sHtML

$obj?->method()
来源：http://m.share.zdbjq.cn/Article/details/gazfmpbvv.sHtML

[U55] PHP：match 表达式
来源：http://baike.fehbvm.com/Article/details/gpekjlsax.sHtML

$s = match($x) { 1 => "一", default => "其他" };
来源：http://baike.zdbjq.cn/Article/details/gnrumwjdt.sHtML

[U56] PHP：命名参数
来源：http://read.share.zdbjq.cn/Article/details/groovlqkp.sHtML

f(a: 1, b: 2)
来源：http://www.m.share.zdbjq.cn/Article/details/gtzrhxnik.sHtML

[U57] PHP：字符串插值
来源：http://read.share.hesvh.cn/Article/details/gnnvytbwc.sHtML

"值: {$a}"
来源：http://www.m.share.zdbjq.cn/Article/details/gjjowyxcn.sHtML

[U58] PHP：数组三件套
来源：http://m.share.zdbjq.cn/Article/details/gkzbqlvbf.sHtML

array_map($f, $a);  array_filter($a, $f);  array_reduce($a, $f, 0);
来源：http://www.blog.fehbvm.com/Article/details/gvgkyqxjh.sHtML

[U59] PHP：自定义排序
来源：http://read.share.hesvh.cn/Article/details/gpierwogu.sHtML

usort($arr, fn($a, $b) => $a["age"] <=> $b["age"]);
来源：http://www.m.share.zdbjq.cn/Article/details/grojwuewh.sHtML

[U60] PHP：JSON 编解码
来源：http://mobile.fehbvm.com/Article/details/gqcwyrbpq.sHtML

json_encode($d, JSON_UNESCAPED_UNICODE);  json_decode($s, true);
来源：http://www.share.fehbvm.com/Article/details/gzgrxflkj.sHtML

[U61] PHP：正则
来源：http://m.share.hesvh.cn/Article/details/gnyvehdxo.sHtML

preg_match('/(\d+)/', $s, $m);  preg_replace('/\d+/', '#', $s);
来源：http://www.blog.zdbjq.cn/Article/details/gidtyxnch.sHtML

[U62] PHP：日期对象
来源：http://www.blog.hesvh.cn/Article/details/gzeziruor.sHtML

(new DateTimeImmutable())->format("Y-m-d");
来源：http://wap.zdbjq.cn/Article/details/gjtppavfg.sHtML

[U63] PHP：文件读写
来源：http://www.m.share.hesvh.cn/Article/details/gghsccgre.sHtML

file_get_contents($f);  file_put_contents($f, $data);
来源：http://3g.fehbvm.com/Article/details/gvcudqgpo.sHtML

[U64] PHP：目录遍历
来源：http://wap.fehbvm.com/Article/details/gfkalhtqb.sHtML

glob("dir/*.php");  scandir("dir");
来源：http://www.m.share.hesvh.cn/Article/details/golbsegzf.sHtML

[U65] PHP：会话
来源：http://wap.zdbjq.cn/Article/details/gdjsdimjl.sHtML

session_start();  $_SESSION["uid"] = 1;
来源：http://baike.zdbjq.cn/Article/details/grghiipuo.sHtML

[U66] PHP：设置 Cookie
来源：http://read.share.zdbjq.cn/Article/details/gwfsdqpxe.sHtML

setcookie("token", $v, ["httponly" => true, "samesite" => "Lax"]);
来源：http://baike.zdbjq.cn/Article/details/gmnttzedh.sHtML

[U67] PHP：处理文件上传
来源：http://baike.zdbjq.cn/Article/details/gizdnudiq.sHtML

$_FILES["file"]["tmp_name"] 与 move_uploaded_file()
来源：http://www.share.fehbvm.com/Article/details/gowsdqofa.sHtML

[U68] PHP：PDO 连接
来源：http://baike.hesvh.cn/Article/details/gixzutcjc.sHtML

$pdo = new PDO("mysql:host=localhost;dbname=app", "root", "");
来源：http://wap.hesvh.cn/Article/details/godpjuxgl.sHtML

[U69] PHP：PDO 预处理
来源：http://read.share.zdbjq.cn/Article/details/ghdhhpqgi.sHtML

$stmt = $pdo->prepare("SELECT * FROM users WHERE id = ?");  $stmt->execute([$id]);
来源：http://m.share.fehbvm.com/Article/details/gsnruowgz.sHtML

[U70] PHP：PDO 事务
来源：http://blog.zdbjq.cn/Article/details/gsxmjqwao.sHtML

$pdo->beginTransaction();  $pdo->commit();  $pdo->rollBack();
来源：http://m.share.fehbvm.com/Article/details/gnwmlybgg.sHtML

[U71] PHP：抛出异常
来源：http://blog.hesvh.cn/Article/details/ggvnxrzad.sHtML

throw new RuntimeException("失败", 500);
来源：http://baike.hesvh.cn/Article/details/gdxcjdzbj.sHtML

[U72] PHP：写错误日志
来源：http://www.m.share.zdbjq.cn/Article/details/gaxoabelf.sHtML

error_log("失败: " . $e->getMessage());
来源：http://mobile.zdbjq.cn/Article/details/gukgehupq.sHtML

[U73] PHP：读取 ini 配置
来源：http://blog.hesvh.cn/Article/details/gcmdzkjhw.sHtML

parse_ini_file("config.ini", true)
来源：http://wap.hesvh.cn/Article/details/gnaokmavx.sHtML

[U74] PHP：读取环境变量
来源：http://www.share.fehbvm.com/Article/details/gnreqpkkd.sHtML

getenv("APP_ENV") ?: "production"
来源：http://www.m.share.hesvh.cn/Article/details/gcczvtfju.sHtML

[U75] PHP：依赖注入
来源：http://m.share.hesvh.cn/Article/details/gcevsmvml.sHtML

composer require psr/container
来源：http://wap.hesvh.cn/Article/details/gltyalbho.sHtML

[U76] PHP：简单路由
来源：http://baike.fehbvm.com/Article/details/ghirlvnen.sHtML

$path = parse_url($_SERVER["REQUEST_URI"], PHP_URL_PATH);
来源：http://www.m.share.zdbjq.cn/Article/details/gtjnfjnib.sHtML

[U77] PHP：模板渲染
来源：http://www.blog.fehbvm.com/Article/details/gkkvxhvav.sHtML

composer require twig/twig
来源：http://mobile.zdbjq.cn/Article/details/grylaykfe.sHtML

[U78] PHP：单元测试
来源：http://3g.hesvh.cn/Article/details/gsghcrqkv.sHtML

composer require --dev phpunit/phpunit
来源：http://mobile.fehbvm.com/Article/details/gbzaidliq.sHtML

[U79] PHP：静态分析
来源：http://wap.zdbjq.cn/Article/details/gdmguchqo.sHtML

composer require --dev phpstan/phpstan
来源：http://3g.zdbjq.cn/Article/details/gfbqubhmg.sHtML

[U80] PHP：代码规范修复
来源：http://m.share.zdbjq.cn/Article/details/gurvudeyg.sHtML

composer require --dev friendsofphp/php-cs-fixer
来源：http://www.m.share.zdbjq.cn/Article/details/gsrscqiwk.sHtML

[U81] JS：初始化项目
来源：http://www.m.share.zdbjq.cn/Article/details/giaznutwn.sHtML

npm init -y;  npm i express
来源：http://read.share.hesvh.cn/Article/details/glhzerhgb.sHtML

[U82] JS：package.json 脚本
来源：http://m.share.zdbjq.cn/Article/details/grqkdzhmg.sHtML

"scripts": { "dev": "vite", "build": "vite build" }
来源：http://wap.fehbvm.com/Article/details/guyyxmvqv.sHtML

[U83] JS：ES Module 导入导出
来源：http://read.share.fehbvm.com/Article/details/gnylgwpza.sHtML

export const a = 1;  import { a } from "./m.js";
来源：http://m.share.fehbvm.com/Article/details/gsgmlikdl.sHtML

[U84] JS：CommonJS 写法
来源：http://mobile.zdbjq.cn/Article/details/gzopqrfso.sHtML

module.exports = { a };  const { a } = require("./m");
来源：http://blog.fehbvm.com/Article/details/gfwhkrqmb.sHtML

[U85] JS：可选链
来源：http://read.share.zdbjq.cn/Article/details/gnjtirhxq.sHtML

a?.b?.c
来源：http://blog.zdbjq.cn/Article/details/gmknmtaou.sHtML

[U86] JS：空值合并
来源：http://baike.fehbvm.com/Article/details/gvgbsgevq.sHtML

a ?? b
来源：http://www.share.hesvh.cn/Article/details/gkceqzkne.sHtML

[U87] JS：解构默认值
来源：http://m.share.zdbjq.cn/Article/details/gkspfvmyn.sHtML

const { a = 1, b = 2 } = obj;
来源：http://read.share.fehbvm.com/Article/details/guvgzdelj.sHtML

[U88] JS：对象展开合并
来源：http://www.m.share.fehbvm.com/Article/details/gxcmxtcpk.sHtML

{ ...a, ...b }
来源：http://m.share.fehbvm.com/Article/details/glqafyeoz.sHtML

[U89] JS：数组去重
来源：http://wap.hesvh.cn/Article/details/gyreyxejr.sHtML

[...new Set(arr)]
来源：http://3g.fehbvm.com/Article/details/gecnfaofv.sHtML

[U90] JS：数字数组排序
来源：http://www.share.hesvh.cn/Article/details/gvgamxwgz.sHtML

[...arr].sort((a, b) => a - b)
来源：http://blog.zdbjq.cn/Article/details/giorasqlg.sHtML

[U91] JS：对象键值遍历
来源：http://www.share.zdbjq.cn/Article/details/gskyserpi.sHtML

Object.entries(obj).forEach(([k, v]) => {});
来源：http://baike.fehbvm.com/Article/details/gkoedkood.sHtML

[U92] JS：深拷贝
来源：http://baike.fehbvm.com/Article/details/gjqyisvwg.sHtML

structuredClone(obj)
来源：http://www.blog.hesvh.cn/Article/details/ggkxfdppx.sHtML

[U93] JS：模板字符串
来源：http://read.share.fehbvm.com/Article/details/gatywrhom.sHtML

`共 ${n} 条`
来源：http://mobile.hesvh.cn/Article/details/gtzfdtdmh.sHtML

[U94] JS：箭头函数
来源：http://read.share.hesvh.cn/Article/details/geouvamjx.sHtML

const double = x => x * 2;
来源：http://read.share.hesvh.cn/Article/details/gcdskcnka.sHtML

[U95] JS：Promise 包装
来源：http://3g.zdbjq.cn/Article/details/grdoifntx.sHtML

new Promise((resolve, reject) => {})
来源：http://www.share.fehbvm.com/Article/details/gjwgrpyjg.sHtML

[U96] JS：async/await 与异常
来源：http://www.share.fehbvm.com/Article/details/gtnlibigt.sHtML

try { const d = await f(); } catch (e) { console.error(e); }
来源：http://m.share.fehbvm.com/Article/details/gicjxuugs.sHtML

[U97] JS：并发请求
来源：http://blog.fehbvm.com/Article/details/gzsiyyyhi.sHtML

await Promise.all(urls.map(u => fetch(u)))
来源：http://www.m.share.fehbvm.com/Article/details/gkckgrcgu.sHtML

[U98] JS：fetch 带 JSON
来源：http://m.share.fehbvm.com/Article/details/gogfmjgkc.sHtML

await fetch(url, { method: "POST", headers: { "Content-Type": "application/json" }, body: JSON.stringify(d) })
来源：http://m.share.hesvh.cn/Article/details/gqvoyoxam.sHtML

[U99] JS：事件监听
来源：http://read.share.fehbvm.com/Article/details/gqhpkjlfi.sHtML

el.addEventListener("click", e => {})
来源：http://baike.zdbjq.cn/Article/details/gaqqcsxea.sHtML

[U100] JS：DOM 查询
来源：http://blog.zdbjq.cn/Article/details/gpzsyxtsw.sHtML

document.querySelector(".item")
来源：http://read.share.zdbjq.cn/Article/details/ghhwjonma.sHtML

[U101] JS：classList 操作
来源：http://m.share.fehbvm.com/Article/details/gwqayxbjw.sHtML

el.classList.toggle("active")
来源：http://m.share.zdbjq.cn/Article/details/griwhoprq.sHtML

[U102] JS：本地存储
来源：http://3g.fehbvm.com/Article/details/gqtetuiyo.sHtML

localStorage.setItem("k", JSON.stringify(v))
来源：http://www.m.share.zdbjq.cn/Article/details/gawyxqlkz.sHtML

[U103] JS：定时器
来源：http://read.share.hesvh.cn/Article/details/gqzdevbbd.sHtML

setTimeout(fn, 1000);  setInterval(fn, 1000);
来源：http://wap.hesvh.cn/Article/details/gjluorymz.sHtML

[U104] JS：防抖
来源：http://baike.zdbjq.cn/Article/details/gohndjmgv.sHtML

const debounce = (fn, ms) => { let t; return (...a) => { clearTimeout(t); t = setTimeout(() => fn(...a), ms); }; };
来源：http://blog.zdbjq.cn/Article/details/gyhxumzta.sHtML

[U105] JS：节流
来源：http://m.share.fehbvm.com/Article/details/gvdrucmbn.sHtML

const throttle = (fn, ms) => { let last = 0; return (...a) => { const n = Date.now(); if (n - last >= ms) { last = n; fn(...a); } }; };
来源：http://m.share.hesvh.cn/Article/details/gfipmcalu.sHtML

[U106] JS：日期格式化
来源：http://blog.zdbjq.cn/Article/details/gaacajoxs.sHtML

new Intl.DateTimeFormat("zh-CN", { dateStyle: "medium" }).format(new Date())
来源：http://blog.fehbvm.com/Article/details/guzgobtoh.sHtML

[U107] JS：数字千分位
来源：http://m.share.fehbvm.com/Article/details/ggkzwbfpc.sHtML

new Intl.NumberFormat("en-US").format(1234567)
来源：http://wap.zdbjq.cn/Article/details/grykidivo.sHtML

[U108] JS：随机整数
来源：http://m.share.zdbjq.cn/Article/details/gmkzmvcjd.sHtML

Math.floor(Math.random() * (max - min + 1)) + min
来源：http://3g.zdbjq.cn/Article/details/grbvzciep.sHtML

[U109] JS：数组分组
来源：http://m.share.fehbvm.com/Article/details/gxbnghveu.sHtML

Object.groupBy(arr, x => x.type)
来源：http://blog.hesvh.cn/Article/details/gyuizrwpb.sHtML

[U110] JS：数组分块
来源：http://blog.fehbvm.com/Article/details/gtvnxncax.sHtML

arr.reduce((acc, x, i) => (i % size ? acc : [...acc, arr.slice(i, i + size)]), [])
来源：http://3g.hesvh.cn/Article/details/gjezvbczd.sHtML

[U111] JS：对象转 Map
来源：http://baike.zdbjq.cn/Article/details/gvafxkdbz.sHtML

new Map(Object.entries(obj))
来源：http://www.share.zdbjq.cn/Article/details/gwxwwhflr.sHtML

[U112] JS：字符串补位
来源：http://baike.fehbvm.com/Article/details/gzjfulttn.sHtML

"7".padStart(3, "0")
来源：http://baike.hesvh.cn/Article/details/guewuudlm.sHtML

[U113] JS：正则替换全部
来源：http://www.blog.zdbjq.cn/Article/details/gizmgmqry.sHtML

s.replaceAll("a", "b")
来源：http://read.share.fehbvm.com/Article/details/gfvenjfrw.sHtML

[U114] JS：JSON 深比较
来源：http://www.share.hesvh.cn/Article/details/gdpkfwisv.sHtML

JSON.stringify(a) === JSON.stringify(b)
来源：http://read.share.fehbvm.com/Article/details/gnsuzrnty.sHtML

[U115] JS：生成 UUID
来源：http://blog.hesvh.cn/Article/details/gygdxeiph.sHtML

crypto.randomUUID()
来源：http://baike.zdbjq.cn/Article/details/gbxusyifp.sHtML

[U116] JS：类型检查（JSDoc）
来源：http://wap.hesvh.cn/Article/details/gsyavhvmp.sHtML

/** @param {string} name */ function f(name) {}
来源：http://www.share.fehbvm.com/Article/details/grfetgghd.sHtML

[U117] JS：单元测试
来源：http://read.share.zdbjq.cn/Article/details/gbmkluwrd.sHtML

npm i -D vitest;  npx vitest
来源：http://www.blog.zdbjq.cn/Article/details/glhuecsql.sHtML

[U118] JS：开发服务器
来源：http://blog.fehbvm.com/Article/details/guhgbldci.sHtML

npm i -D vite;  npx vite
来源：http://www.blog.hesvh.cn/Article/details/gbzbwcxnn.sHtML

[U119] JS：生产构建
来源：http://wap.hesvh.cn/Article/details/glaqfyakj.sHtML

npx vite build
来源：http://3g.hesvh.cn/Article/details/gjqatdpiq.sHtML

[U120] JS：读取环境变量（Vite）
来源：http://baike.zdbjq.cn/Article/details/gnwfcyapz.sHtML

import.meta.env.VITE_API_URL
来源：http://wap.fehbvm.com/Article/details/gwkcvtbru.sHtML

================================================================================
来源：http://mobile.zdbjq.cn/Article/details/gmrzjvhaf.sHtML

统计汇总
来源：http://3g.zdbjq.cn/Article/details/golatdzrs.sHtML

================================================================================
来源：http://wap.zdbjq.cn/Article/details/gbwwkpunr.sHtML

按语言统计（条）：
来源：http://www.blog.hesvh.cn/Article/details/gdozezjph.sHtML

Python ......... 252
来源：http://baike.fehbvm.com/Article/details/gpwwukgpi.sHtML

PHP ............ 252
来源：http://blog.hesvh.cn/Article/details/groqzkqkc.sHtML

JavaScript ..... 252
来源：http://www.share.fehbvm.com/Article/details/gcuwtolfw.sHtML

TypeScript ..... 212
来源：http://blog.fehbvm.com/Article/details/gryhwcjou.sHtML

Java ........... 212
来源：http://3g.fehbvm.com/Article/details/gfdvfufxt.sHtML

Go ............. 212
来源：http://blog.hesvh.cn/Article/details/gpjztzjzi.sHtML

Ruby ........... 212
来源：http://m.share.fehbvm.com/Article/details/gbtscqvmd.sHtML

C# ............. 212
来源：http://blog.zdbjq.cn/Article/details/gbjcseeei.sHtML

C .............. 30
来源：http://3g.hesvh.cn/Article/details/gqstmfeca.sHtML

C++ ............ 30
来源：http://www.m.share.zdbjq.cn/Article/details/gfhlaedog.sHtML

SQL ............ 90
来源：http://baike.zdbjq.cn/Article/details/gidwnbkme.sHtML

Bash ........... 80
来源：http://www.share.hesvh.cn/Article/details/gqotwhcmb.sHtML

Kotlin ......... 15
来源：http://baike.zdbjq.cn/Article/details/gchhaolwd.sHtML

Swift .......... 15
来源：http://baike.hesvh.cn/Article/details/gajupbcfq.sHtML

Lua ............ 10
来源：http://baike.zdbjq.cn/Article/details/getowascy.sHtML

Perl ........... 10
来源：http://www.blog.fehbvm.com/Article/details/gnlvwhwwl.sHtML

Scala .......... 10
来源：http://www.m.share.zdbjq.cn/Article/details/gdkbkvknt.sHtML

------------------------------------
来源：http://mobile.hesvh.cn/Article/details/gozvtfuwz.sHtML

合计 ........... 2106 条
来源：http://read.share.zdbjq.cn/Article/details/gpomwvubh.sHtML

按章节统计：
来源：http://m.share.zdbjq.cn/Article/details/gsbfskohv.sHtML

A 基础语法与类型       26 个任务 × 8 语言 =  208
来源：http://read.share.zdbjq.cn/Article/details/gysxqnwaq.sHtML

B 流程控制             16 个任务 × 8 语言 =  128
来源：http://read.share.hesvh.cn/Article/details/gwqyjudit.sHtML

C 函数与作用域         16 个任务 × 8 语言 =  128
来源：http://3g.zdbjq.cn/Article/details/gtqfmpvqg.sHtML

D 数组 / 列表 / 集合   26 个任务 × 8 语言 =  208
来源：http://mobile.hesvh.cn/Article/details/geklimoeh.sHtML

E 字符串处理           22 个任务 × 8 语言 =  176
来源：http://read.share.hesvh.cn/Article/details/gfrkudwef.sHtML

F 文件与目录           12 个任务 × 8 语言 =   96
来源：http://m.share.fehbvm.com/Article/details/guskwziys.sHtML

G 面向对象             16 个任务 × 8 语言 =  128
来源：http://blog.zdbjq.cn/Article/details/gndjxzlvx.sHtML

H 异常与错误处理       10 个任务 × 8 语言 =   80
来源：http://read.share.hesvh.cn/Article/details/gzektkeks.sHtML

I 正则表达式            8 个任务 × 8 语言 =   64
来源：http://wap.zdbjq.cn/Article/details/guxxtspsq.sHtML

J 日期与时间           10 个任务 × 8 语言 =   80
来源：http://baike.fehbvm.com/Article/details/gsnrayhil.sHtML

K JSON 与序列化         8 个任务 × 8 语言 =   64
来源：http://baike.zdbjq.cn/Article/details/guqkhgmqg.sHtML

L 网络请求              8 个任务 × 8 语言 =   64
来源：http://www.blog.hesvh.cn/Article/details/gbrxnqxft.sHtML

M 命令行 / 进程         8 个任务 × 8 语言 =   64
来源：http://wap.hesvh.cn/Article/details/gzrpwlteo.sHtML

N 数据结构与算法       12 个任务 × 8 语言 =   96
来源：http://m.share.zdbjq.cn/Article/details/gapkxusyv.sHtML

O 并发与异步            6 个任务 × 8 语言 =   48
来源：http://www.share.zdbjq.cn/Article/details/gnzlmgqll.sHtML

P 常用工具函数          8 个任务 × 8 语言 =   64
来源：http://read.share.fehbvm.com/Article/details/gqqhubuce.sHtML

Q SQL 专题                              90
来源：http://wap.hesvh.cn/Article/details/gssndtffa.sHtML

R Bash 专题                             80
来源：http://mobile.zdbjq.cn/Article/details/gnllgzgyl.sHtML

S C / C++ 专题                          60
来源：http://m.share.fehbvm.com/Article/details/gejsivtkc.sHtML

T 其他语言补充                          60
来源：http://mobile.fehbvm.com/Article/details/grajwkkqg.sHtML

U 高频实用片段                         120
来源：http://read.share.zdbjq.cn/Article/details/gsbzhrqcr.sHtML

------------------------------------
来源：http://www.m.share.zdbjq.cn/Article/details/gxljlrodl.sHtML

合计                                  2106 条
来源：http://www.m.share.hesvh.cn/Article/details/gjnovrkxe.sHtML

--------------------------------------------------------------------------------
来源：http://m.share.fehbvm.com/Article/details/gymzvneub.sHtML

使用提醒
来源：http://read.share.zdbjq.cn/Article/details/goilyvjih.sHtML

--------------------------------------------------------------------------------
来源：http://m.share.hesvh.cn/Article/details/gfygkraxq.sHtML

1. 示例追求"最小可用"，正式项目中请补齐导入、错误处理与边界判断。
来源：http://www.blog.zdbjq.cn/Article/details/gxxacnmzh.sHtML

2. 涉及文件、网络、数据库的示例，注意资源释放与异常捕获。
来源：http://baike.hesvh.cn/Article/details/gtivoonpo.sHtML

3. 语言版本差异较大（如 Python 3.10 的 match、Java 17 的 record/switch 箭头），
来源：http://3g.zdbjq.cn/Article/details/gnirvoqzg.sHtML

在旧版本上使用前请先确认语法支持情况。
来源：http://www.share.zdbjq.cn/Article/details/gasujnteu.sHtML

4. 标注"手写"的条目是因为该语言缺少对应内置能力，实际项目中可引入成熟库。
来源：http://www.blog.zdbjq.cn/Article/details/gkhfltvyx.sHtML

—— 文件结束 ——
来源：http://m.share.zdbjq.cn/Article/details/gepljejen.sHtML

================================================================================
来源：http://www.share.fehbvm.com/Article/details/gpgwzlnvs.sHtML

程序语言常见例子速查手册（2024 版）
来源：http://www.blog.hesvh.cn/Article/details/gxqyhtyxp.sHtML

Common Programming Examples Cheat Book
来源：http://3g.fehbvm.com/Article/details/galiraxya.sHtML

================================================================================
来源：http://www.m.share.fehbvm.com/Article/details/gsyrccvcp.sHtML

【收录内容】
来源：http://wap.hesvh.cn/Article/details/goijcynyp.sHtML

覆盖 12 种语言 / 语法与常见 API：
来源：http://www.m.share.fehbvm.com/Article/details/gxqhpmruo.sHtML

Python · PHP · JavaScript · TypeScript · Java · Go · Ruby · C#
来源：http://www.blog.fehbvm.com/Article/details/gjthxoyye.sHtML

SQL · Bash · C · C++
来源：http://3g.fehbvm.com/Article/details/gxnxpwvyl.sHtML

按「任务」分组：每个任务下按语言各给出一条最小可用示例。
来源：http://m.share.fehbvm.com/Article/details/gqbpuldzq.sHtML

【使用说明】
来源：http://www.blog.zdbjq.cn/Article/details/giobtjfqo.sHtML

1. 每个任务形如 "[编号] 任务名"，下面每行以语言标记开头：
来源：http://www.share.hesvh.cn/Article/details/gymluruvx.sHtML

Py:    Python        PHP:   PHP           JS:    JavaScript
来源：http://www.m.share.hesvh.cn/Article/details/gjywcrnst.sHtML

TS:    TypeScript    Java:  Java          Go:    Go
来源：http://www.m.share.hesvh.cn/Article/details/grhzcmeer.sHtML

Ruby:  Ruby          C#:    C#            SQL:   SQL
来源：http://blog.fehbvm.com/Article/details/ghacldthm.sHtML

Bash:  Shell         C:     C             C++:   C++
来源：http://baike.hesvh.cn/Article/details/gdlnnfodn.sHtML

2. 示例只展示核心写法，刻意省略 import / require / include / using 等样板代码。
来源：http://m.share.zdbjq.cn/Article/details/gwbybiwpw.sHtML

需要完整可运行文件时，请自行补齐当前语言的导入语句。
来源：http://m.share.hesvh.cn/Article/details/gczpdviop.sHtML

3. 语法基准：Python 3.10+ / PHP 8.1+ / ES2020+ / TypeScript 5 / Java 17 /
来源：http://baike.zdbjq.cn/Article/details/gccapnnsc.sHtML

Go 1.21+ / Ruby 3.x / C# 10+ / C17 / C++17。
来源：http://wap.hesvh.cn/Article/details/goablcpib.sHtML

4. 检索建议：用编辑器或浏览器 Ctrl+F 搜关键词，如 "排序" "读取文件" "正则"。
来源：http://m.share.fehbvm.com/Article/details/gnilshpeg.sHtML

5. 标记为 "// 无" 表示该语言没有对应的一等语法，需用替代写法（示例给出替代方案）。
来源：http://baike.fehbvm.com/Article/details/gzouggohm.sHtML

6. 符号 "⏎" 表示代码在此处换行（主要用于 Python 等强制缩进、无法压成一行的结构）。
来源：http://3g.zdbjq.cn/Article/details/ghmkcrxuq.sHtML

【文件统计】
来源：http://www.blog.fehbvm.com/Article/details/gxwhwhffa.sHtML

语言示例共 2106 条，分布见本文末尾的「统计汇总」。
来源：http://read.share.zdbjq.cn/Article/details/gjjoyhgbc.sHtML

--------------------------------------------------------------------------------
来源：http://baike.fehbvm.com/Article/details/gazoradat.sHtML

目  录
来源：http://3g.hesvh.cn/Article/details/guwfmqktm.sHtML

--------------------------------------------------------------------------------
来源：http://wap.zdbjq.cn/Article/details/gifjhjozj.sHtML

A. 基础语法与类型              （第 1 节，26 个任务，208 条）
来源：http://baike.hesvh.cn/Article/details/grkcbiwgt.sHtML

B. 流程控制                    （第 2 节，16 个任务，128 条）
来源：http://3g.hesvh.cn/Article/details/gxuqybrns.sHtML

C. 函数与作用域                （第 3 节，16 个任务，128 条）
来源：http://www.blog.hesvh.cn/Article/details/gvvxwqghm.sHtML

D. 数组 / 列表 / 集合          （第 4 节，26 个任务，208 条）
来源：http://wap.hesvh.cn/Article/details/gakvhzvpa.sHtML

E. 字符串处理                  （第 5 节，22 个任务，176 条）
来源：http://blog.fehbvm.com/Article/details/gfusanmdu.sHtML


<!-- 参考信息 -->