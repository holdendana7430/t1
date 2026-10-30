代发 wailian999

[U13] Py：固定长度队列
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gfeuytvis.sHtML

deque(maxlen=10)
来源：http://m.share.fanxiaobao.xyz/Article/details/gdcsnlapb.sHtML

[U14] Py：分组收集到列表
来源：http://blog.fanxiaobao.xyz/Article/details/ghzfjgeko.sHtML

defaultdict(list)
来源：http://baike.fanxiaobao.xyz/Article/details/gcprisypb.sHtML

[U15] Py：高精度计时
来源：http://blog.fanxiaobao.xyz/Article/details/gyicyjehz.sHtML

t = time.perf_counter()
来源：http://3g.fanxiaobao.xyz/Article/details/ggahjnvoo.sHtML

[U16] Py：命令行参数解析
来源：http://blog.fanxiaobao.xyz/Article/details/gluzdoadd.sHtML

ap = argparse.ArgumentParser();  ap.add_argument("--name");  args = ap.parse_args()
来源：http://www.share.fanxiaobao.xyz/Article/details/gxpchfvxt.sHtML

[U17] Py：初始化日志
来源：http://baike.fanxiaobao.xyz/Article/details/gntfwasul.sHtML

logging.basicConfig(level=logging.INFO)
来源：http://mobile.fanxiaobao.xyz/Article/details/gfzksaksx.sHtML

[U18] Py：预编译正则
来源：http://www.share.fanxiaobao.xyz/Article/details/gqwrzzpur.sHtML

pat = re.compile(r"\d+")
来源：http://mobile.fanxiaobao.xyz/Article/details/gsajivusi.sHtML

[U19] Py：正则替换带回调
来源：http://mobile.fanxiaobao.xyz/Article/details/gfynslfpv.sHtML

re.sub(r"\d+", lambda m: str(int(m.group()) * 2), s)
来源：http://www.share.fanxiaobao.xyz/Article/details/gdkhyygod.sHtML

[U20] Py：缓存函数结果
来源：http://www.share.fanxiaobao.xyz/Article/details/gkoywjgrr.sHtML

@functools.lru_cache(maxsize=None)
来源：http://www.share.fanxiaobao.xyz/Article/details/geptgpoji.sHtML

[U21] Py：自定义上下文管理器
来源：http://wap.fanxiaobao.xyz/Article/details/gjmentfav.sHtML

@contextlib.contextmanager
来源：http://www.blog.fanxiaobao.xyz/Article/details/gozsmjdyb.sHtML

[U22] Py：矩阵转置
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gkdbtffrp.sHtML

list(zip(*m))
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gaojekprl.sHtML

[U23] Py：分块读取大文件
来源：http://read.share.fanxiaobao.xyz/Article/details/gxrviggik.sHtML

for chunk in iter(lambda: f.read(8192), b""):
来源：http://www.blog.fanxiaobao.xyz/Article/details/ghlhpyhiv.sHtML

[U24] Py：路径操作
来源：http://mobile.fanxiaobao.xyz/Article/details/gheleobik.sHtML

Path("a/b.txt").parent.mkdir(parents=True, exist_ok=True)
来源：http://www.blog.fanxiaobao.xyz/Article/details/gwquiiohv.sHtML

[U25] Py：CSV 按字典读
来源：http://mobile.fanxiaobao.xyz/Article/details/gjvfvdfht.sHtML

csv.DictReader(f)
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gxqdjwkfp.sHtML

[U26] Py：并发下载
来源：http://www.m.share.fanxiaobao.xyz/Article/details/geswzmjnb.sHtML

ThreadPoolExecutor(max_workers=8).map(fetch, urls)
来源：http://baike.fanxiaobao.xyz/Article/details/grfmzrlcb.sHtML

[U27] Py：异步 HTTP
来源：http://baike.fanxiaobao.xyz/Article/details/grkrmrksg.sHtML

aiohttp.ClientSession() 配合 async with
来源：http://www.share.fanxiaobao.xyz/Article/details/gnuygzjwj.sHtML

[U28] Py：类型别名
来源：http://baike.fanxiaobao.xyz/Article/details/gbjxsqlyq.sHtML

UserId = int
来源：http://mobile.fanxiaobao.xyz/Article/details/goccmlocl.sHtML

[U29] Py：属性校验
来源：http://3g.fanxiaobao.xyz/Article/details/gloffgdih.sHtML

@property 与 @x.setter 配合
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gzklnkclz.sHtML

[U30] Py：数据类
来源：http://baike.fanxiaobao.xyz/Article/details/gzxfupyzi.sHtML

@dataclass(slots=True)
来源：http://wap.fanxiaobao.xyz/Article/details/gfvuvdimx.sHtML

[U31] Py：单测
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gtijllmzk.sHtML

python -m pytest -q
来源：http://blog.fanxiaobao.xyz/Article/details/glpjxrymf.sHtML

[U32] Py：代码格式化
来源：http://read.share.fanxiaobao.xyz/Article/details/gikidsxqj.sHtML

ruff format . && ruff check --fix .
来源：http://read.share.fanxiaobao.xyz/Article/details/glcuxjdgp.sHtML

[U33] Py：打包发布
来源：http://m.share.fanxiaobao.xyz/Article/details/gziuciwag.sHtML

python -m build  （依赖 pyproject.toml）
来源：http://www.blog.fanxiaobao.xyz/Article/details/gdulqewkn.sHtML

[U34] Py：判断编码
来源：http://blog.fanxiaobao.xyz/Article/details/gsjdtrgfk.sHtML

chardet.detect(raw)
来源：http://www.blog.fanxiaobao.xyz/Article/details/gihuofwpl.sHtML

[U35] Py：发送邮件
来源：http://blog.fanxiaobao.xyz/Article/details/gvehfgmpt.sHtML

smtplib.SMTP_SSL(...).send_message(msg)
来源：http://www.share.fanxiaobao.xyz/Article/details/gowpaujwi.sHtML

[U36] Py：定时任务
来源：http://read.share.fanxiaobao.xyz/Article/details/gsuobbdcy.sHtML

schedule.every(10).minutes.do(job)
来源：http://www.blog.fanxiaobao.xyz/Article/details/ggbsueezs.sHtML

[U37] Py：读写 Excel
来源：http://mobile.fanxiaobao.xyz/Article/details/gbheubtnp.sHtML

pandas.read_excel / DataFrame.to_excel
来源：http://www.share.fanxiaobao.xyz/Article/details/ghxubodmr.sHtML

[U38] Py：获取脚本所在目录
来源：http://wap.fanxiaobao.xyz/Article/details/gqokhhodm.sHtML

Path(__file__).resolve().parent
来源：http://mobile.fanxiaobao.xyz/Article/details/ghucjwqke.sHtML

[U39] Py：判断是否在交互环境
来源：http://www.blog.fanxiaobao.xyz/Article/details/gfdfxtvci.sHtML

sys.stdout.isatty()
来源：http://3g.fanxiaobao.xyz/Article/details/gxdvsdiqc.sHtML

[U40] Py：打印到标准错误
来源：http://baike.fanxiaobao.xyz/Article/details/gatrspbfn.sHtML

print("err", file=sys.stderr)
来源：http://m.share.fanxiaobao.xyz/Article/details/ggztxwkmv.sHtML

[U41] PHP：初始化 Composer 项目
来源：http://www.share.fanxiaobao.xyz/Article/details/gwvwcssyr.sHtML

composer init;  composer require guzzlehttp/guzzle
来源：http://m.share.fanxiaobao.xyz/Article/details/gncjmwagj.sHtML

[U42] PHP：PSR-4 自动加载
来源：http://mobile.fanxiaobao.xyz/Article/details/gjxdsudhe.sHtML

"autoload": { "psr-4": { "App\\": "src/" } }
来源：http://3g.fanxiaobao.xyz/Article/details/gavydmnxm.sHtML

[U43] PHP：声明命名空间
来源：http://www.blog.fanxiaobao.xyz/Article/details/godmomyzf.sHtML

namespace App\Http;
来源：http://3g.fanxiaobao.xyz/Article/details/ghtpdmnbx.sHtML

[U44] PHP：开启严格类型
来源：http://wap.fanxiaobao.xyz/Article/details/gatkacsob.sHtML

declare(strict_types=1);
来源：http://www.blog.fanxiaobao.xyz/Article/details/gjxfyxudh.sHtML

[U45] PHP：类型声明与返回类型
来源：http://baike.fanxiaobao.xyz/Article/details/ghvopfszf.sHtML

function add(int $a, int $b): int { return $a + $b; }
来源：http://m.share.fanxiaobao.xyz/Article/details/gahejcgtr.sHtML

[U46] PHP：可空类型
来源：http://m.share.fanxiaobao.xyz/Article/details/giibiirsz.sHtML

?string $name = null
来源：http://baike.fanxiaobao.xyz/Article/details/gynyzqmkh.sHtML

[U47] PHP：联合类型
来源：http://read.share.fanxiaobao.xyz/Article/details/ggeeagyac.sHtML

int|string $id
来源：http://read.share.fanxiaobao.xyz/Article/details/golbfrwfi.sHtML

[U48] PHP：纯枚举
来源：http://blog.fanxiaobao.xyz/Article/details/gnhiewnqh.sHtML

enum Status: string { case Active = "active"; case Off = "off"; }
来源：http://www.blog.fanxiaobao.xyz/Article/details/grqbclesc.sHtML

[U49] PHP：只读属性
来源：http://read.share.fanxiaobao.xyz/Article/details/gpmusbccr.sHtML

public readonly string $name
来源：http://wap.fanxiaobao.xyz/Article/details/gaxymcsuu.sHtML

[U50] PHP：构造器属性提升
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gyyahedrd.sHtML

public function __construct(private int $id) {}
来源：http://www.blog.fanxiaobao.xyz/Article/details/gaqwbjgre.sHtML

[U51] PHP：数组解构
来源：http://wap.fanxiaobao.xyz/Article/details/ghmoeowea.sHtML

[$a, $b] = $arr;
来源：http://blog.fanxiaobao.xyz/Article/details/goecjvyqp.sHtML

[U52] PHP：箭头函数
来源：http://mobile.fanxiaobao.xyz/Article/details/gyzgdpuib.sHtML

$double = fn($x) => $x * 2;
来源：http://wap.fanxiaobao.xyz/Article/details/gsspswbbr.sHtML

[U53] PHP：空合并运算符
来源：http://baike.fanxiaobao.xyz/Article/details/gvuymajga.sHtML

$v = $a ?? $b ?? "default";
来源：http://baike.fanxiaobao.xyz/Article/details/gqesimabf.sHtML

[U54] PHP：空安全调用
来源：http://baike.fanxiaobao.xyz/Article/details/gfjyqpjyd.sHtML

$obj?->method()
来源：http://m.share.fanxiaobao.xyz/Article/details/gipjdbxfo.sHtML

[U55] PHP：match 表达式
来源：http://www.m.share.fanxiaobao.xyz/Article/details/griqesfka.sHtML

$s = match($x) { 1 => "一", default => "其他" };
来源：http://m.share.fanxiaobao.xyz/Article/details/gbhzfybzf.sHtML

[U56] PHP：命名参数
来源：http://mobile.fanxiaobao.xyz/Article/details/gknlqgbuq.sHtML

f(a: 1, b: 2)
来源：http://read.share.fanxiaobao.xyz/Article/details/ggevvhsai.sHtML

[U57] PHP：字符串插值
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gwacnijxv.sHtML

"值: {$a}"
来源：http://mobile.fanxiaobao.xyz/Article/details/grckisbdx.sHtML

[U58] PHP：数组三件套
来源：http://blog.fanxiaobao.xyz/Article/details/guozjcnvo.sHtML

array_map($f, $a);  array_filter($a, $f);  array_reduce($a, $f, 0);
来源：http://wap.fanxiaobao.xyz/Article/details/gnyjwmuel.sHtML

[U59] PHP：自定义排序
来源：http://read.share.fanxiaobao.xyz/Article/details/ghizmygiz.sHtML

usort($arr, fn($a, $b) => $a["age"] <=> $b["age"]);
来源：http://www.m.share.fanxiaobao.xyz/Article/details/guevlchbe.sHtML

[U60] PHP：JSON 编解码
来源：http://wap.fanxiaobao.xyz/Article/details/gfpapmuoi.sHtML

json_encode($d, JSON_UNESCAPED_UNICODE);  json_decode($s, true);
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gzwxnwtou.sHtML

[U61] PHP：正则
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gqtgivnnn.sHtML

preg_match('/(\d+)/', $s, $m);  preg_replace('/\d+/', '#', $s);
来源：http://wap.fanxiaobao.xyz/Article/details/gsefnqhod.sHtML

[U62] PHP：日期对象
来源：http://m.share.fanxiaobao.xyz/Article/details/gyziaiuhu.sHtML

(new DateTimeImmutable())->format("Y-m-d");
来源：http://baike.fanxiaobao.xyz/Article/details/gqpjanhbr.sHtML

[U63] PHP：文件读写
来源：http://wap.fanxiaobao.xyz/Article/details/gwtvemiwr.sHtML

file_get_contents($f);  file_put_contents($f, $data);
来源：http://mobile.fanxiaobao.xyz/Article/details/gavijmobj.sHtML

[U64] PHP：目录遍历
来源：http://3g.fanxiaobao.xyz/Article/details/gqoevuyfu.sHtML

glob("dir/*.php");  scandir("dir");
来源：http://wap.fanxiaobao.xyz/Article/details/gzozjwdma.sHtML

[U65] PHP：会话
来源：http://mobile.fanxiaobao.xyz/Article/details/gdxzstshe.sHtML

session_start();  $_SESSION["uid"] = 1;
来源：http://blog.fanxiaobao.xyz/Article/details/gndgamvil.sHtML

[U66] PHP：设置 Cookie
来源：http://www.share.fanxiaobao.xyz/Article/details/gqsukqtgw.sHtML

setcookie("token", $v, ["httponly" => true, "samesite" => "Lax"]);
来源：http://3g.fanxiaobao.xyz/Article/details/gttzpsgbo.sHtML

[U67] PHP：处理文件上传
来源：http://www.m.share.fanxiaobao.xyz/Article/details/ghjoteddc.sHtML

$_FILES["file"]["tmp_name"] 与 move_uploaded_file()
来源：http://wap.fanxiaobao.xyz/Article/details/gjhsigcyz.sHtML

[U68] PHP：PDO 连接
来源：http://baike.fanxiaobao.xyz/Article/details/glpckepkz.sHtML

$pdo = new PDO("mysql:host=localhost;dbname=app", "root", "");
来源：http://www.share.fanxiaobao.xyz/Article/details/gntmldrrb.sHtML

[U69] PHP：PDO 预处理
来源：http://blog.fanxiaobao.xyz/Article/details/gxzruvkpp.sHtML

$stmt = $pdo->prepare("SELECT * FROM users WHERE id = ?");  $stmt->execute([$id]);
来源：http://mobile.fanxiaobao.xyz/Article/details/gxoszvfoz.sHtML

[U70] PHP：PDO 事务
来源：http://m.share.fanxiaobao.xyz/Article/details/gpclfdffk.sHtML

$pdo->beginTransaction();  $pdo->commit();  $pdo->rollBack();
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gweieptsr.sHtML

[U71] PHP：抛出异常
来源：http://3g.fanxiaobao.xyz/Article/details/gptciiryo.sHtML

throw new RuntimeException("失败", 500);
来源：http://blog.fanxiaobao.xyz/Article/details/gsanwajhg.sHtML

[U72] PHP：写错误日志
来源：http://3g.fanxiaobao.xyz/Article/details/gitjojfrj.sHtML

error_log("失败: " . $e->getMessage());
来源：http://m.share.fanxiaobao.xyz/Article/details/gfjpdkjcr.sHtML

[U73] PHP：读取 ini 配置
来源：http://www.blog.fanxiaobao.xyz/Article/details/gfhvriwta.sHtML

parse_ini_file("config.ini", true)
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gumvgmzbx.sHtML

[U74] PHP：读取环境变量
来源：http://3g.fanxiaobao.xyz/Article/details/gjmexzkfs.sHtML

getenv("APP_ENV") ?: "production"
来源：http://3g.fanxiaobao.xyz/Article/details/gbficjrnb.sHtML

[U75] PHP：依赖注入
来源：http://www.blog.fanxiaobao.xyz/Article/details/gvtgaqofz.sHtML

composer require psr/container
来源：http://m.share.fanxiaobao.xyz/Article/details/gvhgjhzue.sHtML

[U76] PHP：简单路由
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gjwqlckxz.sHtML

$path = parse_url($_SERVER["REQUEST_URI"], PHP_URL_PATH);
来源：http://read.share.fanxiaobao.xyz/Article/details/gghmxoode.sHtML

[U77] PHP：模板渲染
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gdtksgfoe.sHtML

composer require twig/twig
来源：http://www.share.fanxiaobao.xyz/Article/details/gnmjgcqpa.sHtML

[U78] PHP：单元测试
来源：http://mobile.fanxiaobao.xyz/Article/details/gmhhezgtr.sHtML

composer require --dev phpunit/phpunit
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gctzevptk.sHtML

[U79] PHP：静态分析
来源：http://blog.fanxiaobao.xyz/Article/details/gkkddetot.sHtML

composer require --dev phpstan/phpstan
来源：http://www.blog.fanxiaobao.xyz/Article/details/gagbzbtwa.sHtML

[U80] PHP：代码规范修复
来源：http://m.share.fanxiaobao.xyz/Article/details/gfzfrebel.sHtML

composer require --dev friendsofphp/php-cs-fixer
来源：http://read.share.fanxiaobao.xyz/Article/details/ginkkrtno.sHtML

[U81] JS：初始化项目
来源：http://baike.fanxiaobao.xyz/Article/details/gvgwoccmg.sHtML

npm init -y;  npm i express
来源：http://3g.fanxiaobao.xyz/Article/details/gcywbwbzx.sHtML

[U82] JS：package.json 脚本
来源：http://blog.fanxiaobao.xyz/Article/details/grhrngyja.sHtML

"scripts": { "dev": "vite", "build": "vite build" }
来源：http://m.share.fanxiaobao.xyz/Article/details/gczfjkluy.sHtML

[U83] JS：ES Module 导入导出
来源：http://read.share.fanxiaobao.xyz/Article/details/gszqsqpoe.sHtML

export const a = 1;  import { a } from "./m.js";
来源：http://mobile.fanxiaobao.xyz/Article/details/gwnwqgayd.sHtML

[U84] JS：CommonJS 写法
来源：http://wap.fanxiaobao.xyz/Article/details/gizrvifen.sHtML

module.exports = { a };  const { a } = require("./m");
来源：http://www.blog.fanxiaobao.xyz/Article/details/gwqceeejo.sHtML

[U85] JS：可选链
来源：http://www.share.fanxiaobao.xyz/Article/details/gfujrtxjh.sHtML

a?.b?.c
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gfjkhhvfn.sHtML

[U86] JS：空值合并
来源：http://m.share.fanxiaobao.xyz/Article/details/gcyefyaps.sHtML

a ?? b
来源：http://www.share.fanxiaobao.xyz/Article/details/gmtemwjrv.sHtML

[U87] JS：解构默认值
来源：http://www.blog.fanxiaobao.xyz/Article/details/gqitwovko.sHtML

const { a = 1, b = 2 } = obj;
来源：http://www.blog.fanxiaobao.xyz/Article/details/gijfjlgry.sHtML

[U88] JS：对象展开合并
来源：http://www.blog.fanxiaobao.xyz/Article/details/gaqgfjtlb.sHtML

{ ...a, ...b }
来源：http://blog.fanxiaobao.xyz/Article/details/gzysasnoe.sHtML

[U89] JS：数组去重
来源：http://mobile.fanxiaobao.xyz/Article/details/gzwpoefno.sHtML

[...new Set(arr)]
来源：http://blog.fanxiaobao.xyz/Article/details/gloynypex.sHtML

[U90] JS：数字数组排序
来源：http://m.share.fanxiaobao.xyz/Article/details/gwxoymmlz.sHtML

[...arr].sort((a, b) => a - b)
来源：http://mobile.fanxiaobao.xyz/Article/details/gtkdpojtq.sHtML

[U91] JS：对象键值遍历
来源：http://m.share.fanxiaobao.xyz/Article/details/gagaxzonu.sHtML

Object.entries(obj).forEach(([k, v]) => {});
来源：http://read.share.fanxiaobao.xyz/Article/details/gyvkwtpbw.sHtML

[U92] JS：深拷贝
来源：http://3g.fanxiaobao.xyz/Article/details/gcaawqjgc.sHtML

structuredClone(obj)
来源：http://3g.fanxiaobao.xyz/Article/details/gtpishqco.sHtML

[U93] JS：模板字符串
来源：http://blog.fanxiaobao.xyz/Article/details/gygfftyoc.sHtML

`共 ${n} 条`
来源：http://mobile.fanxiaobao.xyz/Article/details/grznpxosa.sHtML

[U94] JS：箭头函数
来源：http://baike.fanxiaobao.xyz/Article/details/gtgimwyim.sHtML

const double = x => x * 2;
来源：http://www.m.share.fanxiaobao.xyz/Article/details/ggrdxcjdp.sHtML

[U95] JS：Promise 包装
来源：http://blog.fanxiaobao.xyz/Article/details/gnuphhont.sHtML

new Promise((resolve, reject) => {})
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gebaihkgc.sHtML

[U96] JS：async/await 与异常
来源：http://m.share.fanxiaobao.xyz/Article/details/gjgkcziid.sHtML

try { const d = await f(); } catch (e) { console.error(e); }
来源：http://www.share.fanxiaobao.xyz/Article/details/gmhqtmhpj.sHtML

[U97] JS：并发请求
来源：http://blog.fanxiaobao.xyz/Article/details/gpkjetcoj.sHtML

await Promise.all(urls.map(u => fetch(u)))
来源：http://baike.fanxiaobao.xyz/Article/details/gjvjvcnqi.sHtML

[U98] JS：fetch 带 JSON
来源：http://wap.fanxiaobao.xyz/Article/details/gislikqmg.sHtML

await fetch(url, { method: "POST", headers: { "Content-Type": "application/json" }, body: JSON.stringify(d) })
来源：http://blog.fanxiaobao.xyz/Article/details/glxtygvcc.sHtML

[U99] JS：事件监听
来源：http://3g.fanxiaobao.xyz/Article/details/gzdllkajb.sHtML

el.addEventListener("click", e => {})
来源：http://blog.fanxiaobao.xyz/Article/details/genpasovr.sHtML

[U100] JS：DOM 查询
来源：http://read.share.fanxiaobao.xyz/Article/details/gizvjmcby.sHtML

document.querySelector(".item")
来源：http://wap.fanxiaobao.xyz/Article/details/gyuyqnsad.sHtML

[U101] JS：classList 操作
来源：http://www.blog.fanxiaobao.xyz/Article/details/gjivizarj.sHtML

el.classList.toggle("active")
来源：http://www.blog.fanxiaobao.xyz/Article/details/gdspxmgnm.sHtML

[U102] JS：本地存储
来源：http://blog.fanxiaobao.xyz/Article/details/gneealolr.sHtML

localStorage.setItem("k", JSON.stringify(v))
来源：http://m.share.fanxiaobao.xyz/Article/details/gwlqnvykc.sHtML

[U103] JS：定时器
来源：http://baike.fanxiaobao.xyz/Article/details/gvgsqbhzb.sHtML

setTimeout(fn, 1000);  setInterval(fn, 1000);
来源：http://m.share.fanxiaobao.xyz/Article/details/gbwjsahlu.sHtML

[U104] JS：防抖
来源：http://baike.fanxiaobao.xyz/Article/details/gizttopnq.sHtML

const debounce = (fn, ms) => { let t; return (...a) => { clearTimeout(t); t = setTimeout(() => fn(...a), ms); }; };
来源：http://m.share.fanxiaobao.xyz/Article/details/gkqdblsot.sHtML

[U105] JS：节流
来源：http://m.share.fanxiaobao.xyz/Article/details/gzbgerhfd.sHtML

const throttle = (fn, ms) => { let last = 0; return (...a) => { const n = Date.now(); if (n - last >= ms) { last = n; fn(...a); } }; };
来源：http://read.share.fanxiaobao.xyz/Article/details/govufvpil.sHtML

[U106] JS：日期格式化
来源：http://read.share.fanxiaobao.xyz/Article/details/gaahjslwe.sHtML

new Intl.DateTimeFormat("zh-CN", { dateStyle: "medium" }).format(new Date())
来源：http://m.share.fanxiaobao.xyz/Article/details/gdiwsfhkb.sHtML

[U107] JS：数字千分位
来源：http://wap.fanxiaobao.xyz/Article/details/gswhsvbws.sHtML

new Intl.NumberFormat("en-US").format(1234567)
来源：http://www.m.share.fanxiaobao.xyz/Article/details/glwjsonfv.sHtML

[U108] JS：随机整数
来源：http://3g.fanxiaobao.xyz/Article/details/gmnwrtznx.sHtML

Math.floor(Math.random() * (max - min + 1)) + min
来源：http://baike.fanxiaobao.xyz/Article/details/gespifcsy.sHtML

[U109] JS：数组分组
来源：http://mobile.fanxiaobao.xyz/Article/details/gyowavnyt.sHtML

Object.groupBy(arr, x => x.type)
来源：http://3g.fanxiaobao.xyz/Article/details/gonhcvvsh.sHtML

[U110] JS：数组分块
来源：http://www.share.fanxiaobao.xyz/Article/details/gkufxauyi.sHtML

arr.reduce((acc, x, i) => (i % size ? acc : [...acc, arr.slice(i, i + size)]), [])
来源：http://read.share.fanxiaobao.xyz/Article/details/gfnsaeyjc.sHtML

[U111] JS：对象转 Map
来源：http://m.share.fanxiaobao.xyz/Article/details/gxjygdroi.sHtML

new Map(Object.entries(obj))
来源：http://m.share.fanxiaobao.xyz/Article/details/gwthpapvc.sHtML

[U112] JS：字符串补位
来源：http://blog.fanxiaobao.xyz/Article/details/gnvkuseqt.sHtML

"7".padStart(3, "0")
来源：http://3g.fanxiaobao.xyz/Article/details/gyxotunqw.sHtML

[U113] JS：正则替换全部
来源：http://read.share.fanxiaobao.xyz/Article/details/gwomnowoc.sHtML

s.replaceAll("a", "b")
来源：http://www.blog.fanxiaobao.xyz/Article/details/gangwlttm.sHtML

[U114] JS：JSON 深比较
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gukofrsxn.sHtML

JSON.stringify(a) === JSON.stringify(b)
来源：http://3g.fanxiaobao.xyz/Article/details/gfcqsdwsi.sHtML

[U115] JS：生成 UUID
来源：http://www.blog.fanxiaobao.xyz/Article/details/gleivvuvc.sHtML

crypto.randomUUID()
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gzrvjnyif.sHtML

[U116] JS：类型检查（JSDoc）
来源：http://read.share.fanxiaobao.xyz/Article/details/gyvotmphp.sHtML

/** @param {string} name */ function f(name) {}
来源：http://3g.fanxiaobao.xyz/Article/details/gymuztjuu.sHtML

[U117] JS：单元测试
来源：http://baike.fanxiaobao.xyz/Article/details/gizymtvlq.sHtML

npm i -D vitest;  npx vitest
来源：http://www.share.fanxiaobao.xyz/Article/details/gmvbpfdln.sHtML

[U118] JS：开发服务器
来源：http://read.share.fanxiaobao.xyz/Article/details/gufbhxrlo.sHtML

npm i -D vite;  npx vite
来源：http://mobile.fanxiaobao.xyz/Article/details/gmpmyuyqm.sHtML

[U119] JS：生产构建
来源：http://wap.fanxiaobao.xyz/Article/details/gkajpkmkc.sHtML

npx vite build
来源：http://www.blog.fanxiaobao.xyz/Article/details/ggazirrvq.sHtML

[U120] JS：读取环境变量（Vite）
来源：http://mobile.fanxiaobao.xyz/Article/details/gfvydcvzi.sHtML

import.meta.env.VITE_API_URL
来源：http://wap.fanxiaobao.xyz/Article/details/gkrlhjtkw.sHtML

================================================================================
来源：http://www.share.fanxiaobao.xyz/Article/details/gsnjdcsso.sHtML

统计汇总
来源：http://www.share.fanxiaobao.xyz/Article/details/gorgojoby.sHtML

================================================================================
来源：http://mobile.fanxiaobao.xyz/Article/details/gvuskvyxq.sHtML

按语言统计（条）：
来源：http://www.blog.fanxiaobao.xyz/Article/details/gxgdurror.sHtML

Python ......... 252
来源：http://www.share.fanxiaobao.xyz/Article/details/gsdgsbree.sHtML

PHP ............ 252
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gzqnzsdbx.sHtML

JavaScript ..... 252
来源：http://wap.fanxiaobao.xyz/Article/details/gqbuugkip.sHtML

TypeScript ..... 212
来源：http://blog.fanxiaobao.xyz/Article/details/gkliphjrx.sHtML

Java ........... 212
来源：http://3g.fanxiaobao.xyz/Article/details/glryzokmu.sHtML

Go ............. 212
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gsllhpzfa.sHtML

Ruby ........... 212
来源：http://baike.fanxiaobao.xyz/Article/details/gsubpxkdb.sHtML

C# ............. 212
来源：http://www.blog.fanxiaobao.xyz/Article/details/gkxrocnfz.sHtML

C .............. 30
来源：http://mobile.fanxiaobao.xyz/Article/details/gjyxzzrjm.sHtML

C++ ............ 30
来源：http://mobile.fanxiaobao.xyz/Article/details/gnwqlmqfl.sHtML

SQL ............ 90
来源：http://mobile.fanxiaobao.xyz/Article/details/gczfzkewz.sHtML

Bash ........... 80
来源：http://baike.fanxiaobao.xyz/Article/details/gqodrmruy.sHtML

Kotlin ......... 15
来源：http://www.share.fanxiaobao.xyz/Article/details/gxnbcbbso.sHtML

Swift .......... 15
来源：http://wap.fanxiaobao.xyz/Article/details/geyjbbdon.sHtML

Lua ............ 10
来源：http://read.share.fanxiaobao.xyz/Article/details/gvldnyhfg.sHtML

Perl ........... 10
来源：http://3g.fanxiaobao.xyz/Article/details/gxgjbyrxn.sHtML

Scala .......... 10
来源：http://3g.fanxiaobao.xyz/Article/details/gfzoleqvk.sHtML

------------------------------------
来源：http://3g.fanxiaobao.xyz/Article/details/gtdmqblgg.sHtML

合计 ........... 2106 条
来源：http://mobile.fanxiaobao.xyz/Article/details/gqzfbowlo.sHtML

按章节统计：
来源：http://mobile.fanxiaobao.xyz/Article/details/gzfbttdkh.sHtML

A 基础语法与类型       26 个任务 × 8 语言 =  208
来源：http://baike.fanxiaobao.xyz/Article/details/godmeisrd.sHtML

B 流程控制             16 个任务 × 8 语言 =  128
来源：http://m.share.fanxiaobao.xyz/Article/details/giioroikz.sHtML

C 函数与作用域         16 个任务 × 8 语言 =  128
来源：http://m.share.fanxiaobao.xyz/Article/details/gzlhqrqdi.sHtML

D 数组 / 列表 / 集合   26 个任务 × 8 语言 =  208
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gehoxnzrm.sHtML

E 字符串处理           22 个任务 × 8 语言 =  176
来源：http://baike.fanxiaobao.xyz/Article/details/gsdknjwdz.sHtML

F 文件与目录           12 个任务 × 8 语言 =   96
来源：http://baike.fanxiaobao.xyz/Article/details/gckhyvbpx.sHtML

G 面向对象             16 个任务 × 8 语言 =  128
来源：http://wap.fanxiaobao.xyz/Article/details/gsytgkhkf.sHtML

H 异常与错误处理       10 个任务 × 8 语言 =   80
来源：http://www.share.fanxiaobao.xyz/Article/details/gacnvxzpd.sHtML

I 正则表达式            8 个任务 × 8 语言 =   64
来源：http://read.share.fanxiaobao.xyz/Article/details/gdyndzztm.sHtML

J 日期与时间           10 个任务 × 8 语言 =   80
来源：http://wap.fanxiaobao.xyz/Article/details/gkszenvgx.sHtML

K JSON 与序列化         8 个任务 × 8 语言 =   64
来源：http://3g.fanxiaobao.xyz/Article/details/gnabddxys.sHtML

L 网络请求              8 个任务 × 8 语言 =   64
来源：http://blog.fanxiaobao.xyz/Article/details/gszgkuwzp.sHtML

M 命令行 / 进程         8 个任务 × 8 语言 =   64
来源：http://read.share.fanxiaobao.xyz/Article/details/gtpcmmkrh.sHtML

N 数据结构与算法       12 个任务 × 8 语言 =   96
来源：http://mobile.fanxiaobao.xyz/Article/details/gaeascoki.sHtML

O 并发与异步            6 个任务 × 8 语言 =   48
来源：http://3g.fanxiaobao.xyz/Article/details/gsbuxqhaa.sHtML

P 常用工具函数          8 个任务 × 8 语言 =   64
来源：http://wap.fanxiaobao.xyz/Article/details/gsayuepmt.sHtML

Q SQL 专题                              90
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gbxoxxjrb.sHtML

R Bash 专题                             80
来源：http://mobile.fanxiaobao.xyz/Article/details/gogjlxdpo.sHtML

S C / C++ 专题                          60
来源：http://blog.fanxiaobao.xyz/Article/details/gxyldwsmg.sHtML

T 其他语言补充                          60
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gdxueyxca.sHtML

U 高频实用片段                         120
来源：http://mobile.fanxiaobao.xyz/Article/details/giszkatxc.sHtML

------------------------------------
来源：http://blog.fanxiaobao.xyz/Article/details/gpstrjspz.sHtML

合计                                  2106 条
来源：http://www.blog.fanxiaobao.xyz/Article/details/gwnonddbe.sHtML

--------------------------------------------------------------------------------
来源：http://wap.fanxiaobao.xyz/Article/details/gniapxtgd.sHtML

使用提醒
来源：http://wap.fanxiaobao.xyz/Article/details/gydqdjvvl.sHtML

--------------------------------------------------------------------------------
来源：http://read.share.fanxiaobao.xyz/Article/details/gpouacstj.sHtML

1. 示例追求"最小可用"，正式项目中请补齐导入、错误处理与边界判断。
来源：http://www.m.share.fanxiaobao.xyz/Article/details/glppbqsdo.sHtML

2. 涉及文件、网络、数据库的示例，注意资源释放与异常捕获。
来源：http://blog.fanxiaobao.xyz/Article/details/gkbbmopye.sHtML

3. 语言版本差异较大（如 Python 3.10 的 match、Java 17 的 record/switch 箭头），
来源：http://m.share.fanxiaobao.xyz/Article/details/gynclnmmg.sHtML

在旧版本上使用前请先确认语法支持情况。
来源：http://baike.fanxiaobao.xyz/Article/details/ggpbqiugh.sHtML

4. 标注"手写"的条目是因为该语言缺少对应内置能力，实际项目中可引入成熟库。
来源：http://www.m.share.fanxiaobao.xyz/Article/details/ghcdpdyow.sHtML

—— 文件结束 ——
来源：http://3g.fanxiaobao.xyz/Article/details/gvhkclqxa.sHtML

================================================================================
来源：http://read.share.fanxiaobao.xyz/Article/details/gculdeujs.sHtML

程序语言常见例子速查手册（2024 版）
来源：http://m.share.fanxiaobao.xyz/Article/details/gvfrweskx.sHtML

Common Programming Examples Cheat Book
来源：http://baike.fanxiaobao.xyz/Article/details/gixqydhmf.sHtML

================================================================================
来源：http://www.m.share.fanxiaobao.xyz/Article/details/ginbpnwdy.sHtML

【收录内容】
来源：http://blog.fanxiaobao.xyz/Article/details/gkwaezodb.sHtML

覆盖 12 种语言 / 语法与常见 API：
来源：http://mobile.fanxiaobao.xyz/Article/details/gulkefxzf.sHtML

Python · PHP · JavaScript · TypeScript · Java · Go · Ruby · C#
来源：http://www.m.share.fanxiaobao.xyz/Article/details/ghlqovieb.sHtML

SQL · Bash · C · C++
来源：http://www.blog.fanxiaobao.xyz/Article/details/gemrcrwrg.sHtML

按「任务」分组：每个任务下按语言各给出一条最小可用示例。
来源：http://www.share.fanxiaobao.xyz/Article/details/grkygdehp.sHtML

【使用说明】
来源：http://3g.fanxiaobao.xyz/Article/details/gwulvjezb.sHtML

1. 每个任务形如 "[编号] 任务名"，下面每行以语言标记开头：
来源：http://read.share.fanxiaobao.xyz/Article/details/gyxdknyhf.sHtML

Py:    Python        PHP:   PHP           JS:    JavaScript
来源：http://blog.fanxiaobao.xyz/Article/details/gplgmvpro.sHtML

TS:    TypeScript    Java:  Java          Go:    Go
来源：http://wap.fanxiaobao.xyz/Article/details/gbuaytvmn.sHtML

Ruby:  Ruby          C#:    C#            SQL:   SQL
来源：http://www.share.fanxiaobao.xyz/Article/details/gdugowewb.sHtML

Bash:  Shell         C:     C             C++:   C++
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gqyakrpyt.sHtML

2. 示例只展示核心写法，刻意省略 import / require / include / using 等样板代码。
来源：http://3g.fanxiaobao.xyz/Article/details/gvdkjiebb.sHtML

需要完整可运行文件时，请自行补齐当前语言的导入语句。
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gchghtqzm.sHtML

3. 语法基准：Python 3.10+ / PHP 8.1+ / ES2020+ / TypeScript 5 / Java 17 /
来源：http://m.share.fanxiaobao.xyz/Article/details/gwntooepd.sHtML

Go 1.21+ / Ruby 3.x / C# 10+ / C17 / C++17。
来源：http://mobile.fanxiaobao.xyz/Article/details/gqxnutvjd.sHtML

4. 检索建议：用编辑器或浏览器 Ctrl+F 搜关键词，如 "排序" "读取文件" "正则"。
来源：http://mobile.fanxiaobao.xyz/Article/details/ghnifmsrm.sHtML

5. 标记为 "// 无" 表示该语言没有对应的一等语法，需用替代写法（示例给出替代方案）。
来源：http://3g.fanxiaobao.xyz/Article/details/gsghsgjdn.sHtML

6. 符号 "⏎" 表示代码在此处换行（主要用于 Python 等强制缩进、无法压成一行的结构）。
来源：http://www.share.fanxiaobao.xyz/Article/details/gxsgrkmgu.sHtML

【文件统计】
来源：http://www.share.fanxiaobao.xyz/Article/details/gfwwaokah.sHtML

语言示例共 2106 条，分布见本文末尾的「统计汇总」。
来源：http://mobile.fanxiaobao.xyz/Article/details/gvxkocugw.sHtML

--------------------------------------------------------------------------------
来源：http://www.blog.fanxiaobao.xyz/Article/details/gbsgxyezu.sHtML

目  录
来源：http://www.blog.fanxiaobao.xyz/Article/details/gwzyngwbs.sHtML

--------------------------------------------------------------------------------
来源：http://read.share.fanxiaobao.xyz/Article/details/gtwjyarhp.sHtML

A. 基础语法与类型              （第 1 节，26 个任务，208 条）
来源：http://3g.fanxiaobao.xyz/Article/details/guqkcoqhy.sHtML


<!-- 参考信息 -->