代发 wailian999

[U23] Py：分块读取大文件
来源：http://www.share.fanxiaobao.xyz/Article/details/gshpwxyxa.sHtML

for chunk in iter(lambda: f.read(8192), b""):
来源：http://m.share.fanxiaobao.xyz/Article/details/gjxyantpa.sHtML

[U24] Py：路径操作
来源：http://www.share.fanxiaobao.xyz/Article/details/gcohlktyg.sHtML

Path("a/b.txt").parent.mkdir(parents=True, exist_ok=True)
来源：http://read.share.fanxiaobao.xyz/Article/details/gkwofngdb.sHtML

[U25] Py：CSV 按字典读
来源：http://read.share.fanxiaobao.xyz/Article/details/grbykgonq.sHtML

csv.DictReader(f)
来源：http://read.share.fanxiaobao.xyz/Article/details/gefugibfr.sHtML

[U26] Py：并发下载
来源：http://www.blog.fanxiaobao.xyz/Article/details/grktfxsfi.sHtML

ThreadPoolExecutor(max_workers=8).map(fetch, urls)
来源：http://www.share.fanxiaobao.xyz/Article/details/gzeajwvqk.sHtML

[U27] Py：异步 HTTP
来源：http://m.share.fanxiaobao.xyz/Article/details/gpptxfqvq.sHtML

aiohttp.ClientSession() 配合 async with
来源：http://3g.fanxiaobao.xyz/Article/details/goyaamdgh.sHtML

[U28] Py：类型别名
来源：http://3g.fanxiaobao.xyz/Article/details/gvaybinlh.sHtML

UserId = int
来源：http://read.share.fanxiaobao.xyz/Article/details/gjsrvwmde.sHtML

[U29] Py：属性校验
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gubphvppo.sHtML

@property 与 @x.setter 配合
来源：http://blog.fanxiaobao.xyz/Article/details/gblpkcnno.sHtML

[U30] Py：数据类
来源：http://blog.fanxiaobao.xyz/Article/details/gfndbtccy.sHtML

@dataclass(slots=True)
来源：http://blog.fanxiaobao.xyz/Article/details/gboyibkdd.sHtML

[U31] Py：单测
来源：http://www.share.fanxiaobao.xyz/Article/details/gzdtxlplr.sHtML

python -m pytest -q
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gxjzazijl.sHtML

[U32] Py：代码格式化
来源：http://baike.fanxiaobao.xyz/Article/details/gyluaeacs.sHtML

ruff format . && ruff check --fix .
来源：http://mobile.fanxiaobao.xyz/Article/details/guebdonvk.sHtML

[U33] Py：打包发布
来源：http://read.share.fanxiaobao.xyz/Article/details/gfbcdglxk.sHtML

python -m build  （依赖 pyproject.toml）
来源：http://mobile.fanxiaobao.xyz/Article/details/gebfjahkh.sHtML

[U34] Py：判断编码
来源：http://baike.fanxiaobao.xyz/Article/details/grwtqbtrd.sHtML

chardet.detect(raw)
来源：http://www.blog.fanxiaobao.xyz/Article/details/gbcqalgek.sHtML

[U35] Py：发送邮件
来源：http://blog.fanxiaobao.xyz/Article/details/gzfttfxql.sHtML

smtplib.SMTP_SSL(...).send_message(msg)
来源：http://mobile.fanxiaobao.xyz/Article/details/gjyxubukm.sHtML

[U36] Py：定时任务
来源：http://3g.fanxiaobao.xyz/Article/details/gxjhmlplb.sHtML

schedule.every(10).minutes.do(job)
来源：http://mobile.fanxiaobao.xyz/Article/details/gfnzwiqpo.sHtML

[U37] Py：读写 Excel
来源：http://wap.fanxiaobao.xyz/Article/details/gwvtgghqq.sHtML

pandas.read_excel / DataFrame.to_excel
来源：http://www.blog.fanxiaobao.xyz/Article/details/gcjxweqaq.sHtML

[U38] Py：获取脚本所在目录
来源：http://www.share.fanxiaobao.xyz/Article/details/gumcjcymw.sHtML

Path(__file__).resolve().parent
来源：http://m.share.fanxiaobao.xyz/Article/details/ghbbtasny.sHtML

[U39] Py：判断是否在交互环境
来源：http://www.share.fanxiaobao.xyz/Article/details/glumfndwf.sHtML

sys.stdout.isatty()
来源：http://wap.fanxiaobao.xyz/Article/details/ggptpukfm.sHtML

[U40] Py：打印到标准错误
来源：http://m.share.fanxiaobao.xyz/Article/details/gykzaezzi.sHtML

print("err", file=sys.stderr)
来源：http://baike.fanxiaobao.xyz/Article/details/gmizzopfs.sHtML

[U41] PHP：初始化 Composer 项目
来源：http://read.share.fanxiaobao.xyz/Article/details/gtmgkwrdf.sHtML

composer init;  composer require guzzlehttp/guzzle
来源：http://blog.fanxiaobao.xyz/Article/details/gpavhpcfw.sHtML

[U42] PHP：PSR-4 自动加载
来源：http://read.share.fanxiaobao.xyz/Article/details/ggyoclfuz.sHtML

"autoload": { "psr-4": { "App\\": "src/" } }
来源：http://blog.fanxiaobao.xyz/Article/details/gayyimami.sHtML

[U43] PHP：声明命名空间
来源：http://www.blog.fanxiaobao.xyz/Article/details/gndsnhdtj.sHtML

namespace App\Http;
来源：http://mobile.fanxiaobao.xyz/Article/details/goruruaxz.sHtML

[U44] PHP：开启严格类型
来源：http://baike.fanxiaobao.xyz/Article/details/gchnquwtp.sHtML

declare(strict_types=1);
来源：http://read.share.fanxiaobao.xyz/Article/details/gkhccphub.sHtML

[U45] PHP：类型声明与返回类型
来源：http://3g.fanxiaobao.xyz/Article/details/gorjaryyh.sHtML

function add(int $a, int $b): int { return $a + $b; }
来源：http://baike.fanxiaobao.xyz/Article/details/gldtggtxh.sHtML

[U46] PHP：可空类型
来源：http://read.share.fanxiaobao.xyz/Article/details/gaohiuoce.sHtML

?string $name = null
来源：http://www.blog.fanxiaobao.xyz/Article/details/gtfjgrxjb.sHtML

[U47] PHP：联合类型
来源：http://3g.fanxiaobao.xyz/Article/details/gzktfljer.sHtML

int|string $id
来源：http://wap.fanxiaobao.xyz/Article/details/gonvgxnqy.sHtML

[U48] PHP：纯枚举
来源：http://www.m.share.fanxiaobao.xyz/Article/details/grusvgsxt.sHtML

enum Status: string { case Active = "active"; case Off = "off"; }
来源：http://www.m.share.fanxiaobao.xyz/Article/details/ghqntgzxb.sHtML

[U49] PHP：只读属性
来源：http://wap.fanxiaobao.xyz/Article/details/gogojebyn.sHtML

public readonly string $name
来源：http://read.share.fanxiaobao.xyz/Article/details/gzsubawys.sHtML

[U50] PHP：构造器属性提升
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gtafsykte.sHtML

public function __construct(private int $id) {}
来源：http://www.share.fanxiaobao.xyz/Article/details/gwvtqebbo.sHtML

[U51] PHP：数组解构
来源：http://3g.fanxiaobao.xyz/Article/details/glawawjqs.sHtML

[$a, $b] = $arr;
来源：http://wap.fanxiaobao.xyz/Article/details/gijorcmgp.sHtML

[U52] PHP：箭头函数
来源：http://www.share.fanxiaobao.xyz/Article/details/gmmwucyjy.sHtML

$double = fn($x) => $x * 2;
来源：http://wap.fanxiaobao.xyz/Article/details/gtnhnofpc.sHtML

[U53] PHP：空合并运算符
来源：http://read.share.fanxiaobao.xyz/Article/details/glsudxltm.sHtML

$v = $a ?? $b ?? "default";
来源：http://www.share.fanxiaobao.xyz/Article/details/gzuekakxw.sHtML

[U54] PHP：空安全调用
来源：http://www.share.fanxiaobao.xyz/Article/details/gfvsxpyhm.sHtML

$obj?->method()
来源：http://blog.fanxiaobao.xyz/Article/details/gwxlffvws.sHtML

[U55] PHP：match 表达式
来源：http://3g.fanxiaobao.xyz/Article/details/gfqcoxajg.sHtML

$s = match($x) { 1 => "一", default => "其他" };
来源：http://www.blog.fanxiaobao.xyz/Article/details/gdrxotdxs.sHtML

[U56] PHP：命名参数
来源：http://blog.fanxiaobao.xyz/Article/details/gfqezzsnu.sHtML

f(a: 1, b: 2)
来源：http://3g.fanxiaobao.xyz/Article/details/gisdagkvu.sHtML

[U57] PHP：字符串插值
来源：http://www.share.fanxiaobao.xyz/Article/details/gqsmicyhz.sHtML

"值: {$a}"
来源：http://read.share.fanxiaobao.xyz/Article/details/gbgadqyoa.sHtML

[U58] PHP：数组三件套
来源：http://3g.fanxiaobao.xyz/Article/details/gcjjiipqg.sHtML

array_map($f, $a);  array_filter($a, $f);  array_reduce($a, $f, 0);
来源：http://m.share.fanxiaobao.xyz/Article/details/gwjjbhbbt.sHtML

[U59] PHP：自定义排序
来源：http://read.share.fanxiaobao.xyz/Article/details/grjdwelxf.sHtML

usort($arr, fn($a, $b) => $a["age"] <=> $b["age"]);
来源：http://read.share.fanxiaobao.xyz/Article/details/gldiruqei.sHtML

[U60] PHP：JSON 编解码
来源：http://www.share.fanxiaobao.xyz/Article/details/gahnkuluw.sHtML

json_encode($d, JSON_UNESCAPED_UNICODE);  json_decode($s, true);
来源：http://m.share.fanxiaobao.xyz/Article/details/gpoqyuuuw.sHtML

[U61] PHP：正则
来源：http://mobile.fanxiaobao.xyz/Article/details/gwysmnfhr.sHtML

preg_match('/(\d+)/', $s, $m);  preg_replace('/\d+/', '#', $s);
来源：http://wap.fanxiaobao.xyz/Article/details/ggkjkbqvx.sHtML

[U62] PHP：日期对象
来源：http://wap.fanxiaobao.xyz/Article/details/gekgeqyei.sHtML

(new DateTimeImmutable())->format("Y-m-d");
来源：http://www.share.fanxiaobao.xyz/Article/details/graryaqxz.sHtML

[U63] PHP：文件读写
来源：http://baike.fanxiaobao.xyz/Article/details/gtxelowtu.sHtML

file_get_contents($f);  file_put_contents($f, $data);
来源：http://wap.fanxiaobao.xyz/Article/details/grjsbxuvq.sHtML

[U64] PHP：目录遍历
来源：http://blog.fanxiaobao.xyz/Article/details/gxzqdnudr.sHtML

glob("dir/*.php");  scandir("dir");
来源：http://m.share.fanxiaobao.xyz/Article/details/gvsmyplni.sHtML

[U65] PHP：会话
来源：http://www.m.share.fanxiaobao.xyz/Article/details/ggvcrxanr.sHtML

session_start();  $_SESSION["uid"] = 1;
来源：http://baike.fanxiaobao.xyz/Article/details/gorxbuqfo.sHtML

[U66] PHP：设置 Cookie
来源：http://3g.fanxiaobao.xyz/Article/details/gohvshcng.sHtML

setcookie("token", $v, ["httponly" => true, "samesite" => "Lax"]);
来源：http://www.blog.fanxiaobao.xyz/Article/details/ghrukxgtx.sHtML

[U67] PHP：处理文件上传
来源：http://mobile.fanxiaobao.xyz/Article/details/gzfuxnqcr.sHtML

$_FILES["file"]["tmp_name"] 与 move_uploaded_file()
来源：http://m.share.fanxiaobao.xyz/Article/details/gmqljpgxq.sHtML

[U68] PHP：PDO 连接
来源：http://baike.fanxiaobao.xyz/Article/details/gadttxmfd.sHtML

$pdo = new PDO("mysql:host=localhost;dbname=app", "root", "");
来源：http://wap.fanxiaobao.xyz/Article/details/ggjbcozeq.sHtML

[U69] PHP：PDO 预处理
来源：http://m.share.fanxiaobao.xyz/Article/details/gwjbwhjkc.sHtML

$stmt = $pdo->prepare("SELECT * FROM users WHERE id = ?");  $stmt->execute([$id]);
来源：http://blog.fanxiaobao.xyz/Article/details/gdwfoloej.sHtML

[U70] PHP：PDO 事务
来源：http://m.share.fanxiaobao.xyz/Article/details/glfqfjrav.sHtML

$pdo->beginTransaction();  $pdo->commit();  $pdo->rollBack();
来源：http://read.share.fanxiaobao.xyz/Article/details/gdltldmzu.sHtML

[U71] PHP：抛出异常
来源：http://m.share.fanxiaobao.xyz/Article/details/ghzhsisca.sHtML

throw new RuntimeException("失败", 500);
来源：http://mobile.fanxiaobao.xyz/Article/details/glkchnkxo.sHtML

[U72] PHP：写错误日志
来源：http://read.share.fanxiaobao.xyz/Article/details/gekgqcahs.sHtML

error_log("失败: " . $e->getMessage());
来源：http://m.share.fanxiaobao.xyz/Article/details/gwltygchv.sHtML

[U73] PHP：读取 ini 配置
来源：http://www.blog.fanxiaobao.xyz/Article/details/goohqtqmw.sHtML

parse_ini_file("config.ini", true)
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gctkhlzjc.sHtML

[U74] PHP：读取环境变量
来源：http://blog.fanxiaobao.xyz/Article/details/gzemarksn.sHtML

getenv("APP_ENV") ?: "production"
来源：http://baike.fanxiaobao.xyz/Article/details/gthvctsfo.sHtML

[U75] PHP：依赖注入
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gkgbzutkm.sHtML

composer require psr/container
来源：http://www.share.fanxiaobao.xyz/Article/details/gcydabvzm.sHtML

[U76] PHP：简单路由
来源：http://3g.fanxiaobao.xyz/Article/details/gnumrnhan.sHtML

$path = parse_url($_SERVER["REQUEST_URI"], PHP_URL_PATH);
来源：http://www.share.fanxiaobao.xyz/Article/details/gdgobqfqo.sHtML

[U77] PHP：模板渲染
来源：http://www.share.fanxiaobao.xyz/Article/details/gssozkkdt.sHtML

composer require twig/twig
来源：http://blog.fanxiaobao.xyz/Article/details/gmiaxursr.sHtML

[U78] PHP：单元测试
来源：http://www.m.share.fanxiaobao.xyz/Article/details/glbcmxyfy.sHtML

composer require --dev phpunit/phpunit
来源：http://m.share.fanxiaobao.xyz/Article/details/grbjkiypz.sHtML

[U79] PHP：静态分析
来源：http://m.share.fanxiaobao.xyz/Article/details/ghtpiwbfo.sHtML

composer require --dev phpstan/phpstan
来源：http://mobile.fanxiaobao.xyz/Article/details/grypyciqv.sHtML

[U80] PHP：代码规范修复
来源：http://3g.fanxiaobao.xyz/Article/details/gdhtxyzty.sHtML

composer require --dev friendsofphp/php-cs-fixer
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gwtftclkt.sHtML

[U81] JS：初始化项目
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gwqrfsuay.sHtML

npm init -y;  npm i express
来源：http://read.share.fanxiaobao.xyz/Article/details/grjudkipa.sHtML

[U82] JS：package.json 脚本
来源：http://mobile.fanxiaobao.xyz/Article/details/gbpaaxpdw.sHtML

"scripts": { "dev": "vite", "build": "vite build" }
来源：http://m.share.fanxiaobao.xyz/Article/details/gsridtrcc.sHtML

[U83] JS：ES Module 导入导出
来源：http://www.blog.fanxiaobao.xyz/Article/details/gathvbkpw.sHtML

export const a = 1;  import { a } from "./m.js";
来源：http://www.blog.fanxiaobao.xyz/Article/details/gjutfufcj.sHtML

[U84] JS：CommonJS 写法
来源：http://read.share.fanxiaobao.xyz/Article/details/gxucubwiw.sHtML

module.exports = { a };  const { a } = require("./m");
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gthoqhbha.sHtML

[U85] JS：可选链
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gqialpnkb.sHtML

a?.b?.c
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gscrbaqxb.sHtML

[U86] JS：空值合并
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gudlavkex.sHtML

a ?? b
来源：http://baike.fanxiaobao.xyz/Article/details/gfyjyvyrg.sHtML

[U87] JS：解构默认值
来源：http://www.blog.fanxiaobao.xyz/Article/details/gywtbvtxv.sHtML

const { a = 1, b = 2 } = obj;
来源：http://m.share.fanxiaobao.xyz/Article/details/gkxznnvst.sHtML

[U88] JS：对象展开合并
来源：http://baike.fanxiaobao.xyz/Article/details/gncklnacx.sHtML

{ ...a, ...b }
来源：http://3g.fanxiaobao.xyz/Article/details/gbkzvebtw.sHtML

[U89] JS：数组去重
来源：http://www.share.fanxiaobao.xyz/Article/details/girguokjy.sHtML

[...new Set(arr)]
来源：http://baike.fanxiaobao.xyz/Article/details/gvxcdlkai.sHtML

[U90] JS：数字数组排序
来源：http://m.share.fanxiaobao.xyz/Article/details/gpttwojyw.sHtML

[...arr].sort((a, b) => a - b)
来源：http://read.share.fanxiaobao.xyz/Article/details/gwizachwg.sHtML

[U91] JS：对象键值遍历
来源：http://www.blog.fanxiaobao.xyz/Article/details/gsqudvizc.sHtML

Object.entries(obj).forEach(([k, v]) => {});
来源：http://read.share.fanxiaobao.xyz/Article/details/gwtlvrkli.sHtML

[U92] JS：深拷贝
来源：http://m.share.fanxiaobao.xyz/Article/details/gvguhxkyh.sHtML

structuredClone(obj)
来源：http://www.m.share.fanxiaobao.xyz/Article/details/goiralvwx.sHtML

[U93] JS：模板字符串
来源：http://www.blog.fanxiaobao.xyz/Article/details/gyjyovkqj.sHtML

`共 ${n} 条`
来源：http://baike.fanxiaobao.xyz/Article/details/gwfqnxeqz.sHtML

[U94] JS：箭头函数
来源：http://blog.fanxiaobao.xyz/Article/details/gsuerdopv.sHtML

const double = x => x * 2;
来源：http://read.share.fanxiaobao.xyz/Article/details/gceflzxux.sHtML

[U95] JS：Promise 包装
来源：http://www.blog.fanxiaobao.xyz/Article/details/gqmdmjazg.sHtML

new Promise((resolve, reject) => {})
来源：http://blog.fanxiaobao.xyz/Article/details/gfxeshxpu.sHtML

[U96] JS：async/await 与异常
来源：http://baike.fanxiaobao.xyz/Article/details/gtxgfevfp.sHtML

try { const d = await f(); } catch (e) { console.error(e); }
来源：http://wap.fanxiaobao.xyz/Article/details/gtgzslkbw.sHtML

[U97] JS：并发请求
来源：http://wap.fanxiaobao.xyz/Article/details/gibjpqroq.sHtML

await Promise.all(urls.map(u => fetch(u)))
来源：http://wap.fanxiaobao.xyz/Article/details/gxfvdpvqs.sHtML

[U98] JS：fetch 带 JSON
来源：http://read.share.fanxiaobao.xyz/Article/details/gbvacycsj.sHtML

await fetch(url, { method: "POST", headers: { "Content-Type": "application/json" }, body: JSON.stringify(d) })
来源：http://wap.fanxiaobao.xyz/Article/details/gkkxvnpmd.sHtML

[U99] JS：事件监听
来源：http://baike.fanxiaobao.xyz/Article/details/gmbsjbfqf.sHtML

el.addEventListener("click", e => {})
来源：http://blog.fanxiaobao.xyz/Article/details/gxaihgdfq.sHtML

[U100] JS：DOM 查询
来源：http://mobile.fanxiaobao.xyz/Article/details/gobwofiik.sHtML

document.querySelector(".item")
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gummindey.sHtML

[U101] JS：classList 操作
来源：http://wap.fanxiaobao.xyz/Article/details/godwooyeh.sHtML

el.classList.toggle("active")
来源：http://baike.fanxiaobao.xyz/Article/details/ghskdyzaf.sHtML

[U102] JS：本地存储
来源：http://baike.fanxiaobao.xyz/Article/details/gebegarhv.sHtML

localStorage.setItem("k", JSON.stringify(v))
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gfatmpkms.sHtML

[U103] JS：定时器
来源：http://www.share.fanxiaobao.xyz/Article/details/goenagprg.sHtML

setTimeout(fn, 1000);  setInterval(fn, 1000);
来源：http://3g.fanxiaobao.xyz/Article/details/gwsheugoq.sHtML

[U104] JS：防抖
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gennmncsz.sHtML

const debounce = (fn, ms) => { let t; return (...a) => { clearTimeout(t); t = setTimeout(() => fn(...a), ms); }; };
来源：http://m.share.fanxiaobao.xyz/Article/details/gqsfbuudk.sHtML

[U105] JS：节流
来源：http://baike.fanxiaobao.xyz/Article/details/gruerwfpr.sHtML

const throttle = (fn, ms) => { let last = 0; return (...a) => { const n = Date.now(); if (n - last >= ms) { last = n; fn(...a); } }; };
来源：http://www.m.share.fanxiaobao.xyz/Article/details/garmxsoak.sHtML

[U106] JS：日期格式化
来源：http://blog.fanxiaobao.xyz/Article/details/ghhennsez.sHtML

new Intl.DateTimeFormat("zh-CN", { dateStyle: "medium" }).format(new Date())
来源：http://www.m.share.fanxiaobao.xyz/Article/details/ghnnjlovz.sHtML

[U107] JS：数字千分位
来源：http://www.blog.fanxiaobao.xyz/Article/details/gvzooesac.sHtML

new Intl.NumberFormat("en-US").format(1234567)
来源：http://m.share.fanxiaobao.xyz/Article/details/gdgxhgzbg.sHtML

[U108] JS：随机整数
来源：http://read.share.fanxiaobao.xyz/Article/details/gtvzqsmca.sHtML

Math.floor(Math.random() * (max - min + 1)) + min
来源：http://baike.fanxiaobao.xyz/Article/details/gwufqphtj.sHtML

[U109] JS：数组分组
来源：http://mobile.fanxiaobao.xyz/Article/details/gwnmltfal.sHtML

Object.groupBy(arr, x => x.type)
来源：http://mobile.fanxiaobao.xyz/Article/details/gnnypvnvs.sHtML

[U110] JS：数组分块
来源：http://www.share.fanxiaobao.xyz/Article/details/glidlanjm.sHtML

arr.reduce((acc, x, i) => (i % size ? acc : [...acc, arr.slice(i, i + size)]), [])
来源：http://read.share.fanxiaobao.xyz/Article/details/gdkrxvzyk.sHtML

[U111] JS：对象转 Map
来源：http://www.share.fanxiaobao.xyz/Article/details/gxkbbhsyx.sHtML

new Map(Object.entries(obj))
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gtlmgrbqn.sHtML

[U112] JS：字符串补位
来源：http://m.share.fanxiaobao.xyz/Article/details/gjregblzc.sHtML

"7".padStart(3, "0")
来源：http://wap.fanxiaobao.xyz/Article/details/gxzraxqel.sHtML

[U113] JS：正则替换全部
来源：http://blog.fanxiaobao.xyz/Article/details/gxzocmkst.sHtML

s.replaceAll("a", "b")
来源：http://m.share.fanxiaobao.xyz/Article/details/gtmvkubsw.sHtML

[U114] JS：JSON 深比较
来源：http://m.share.fanxiaobao.xyz/Article/details/gvclazsny.sHtML

JSON.stringify(a) === JSON.stringify(b)
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gyfnwdwmb.sHtML

[U115] JS：生成 UUID
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gcgzeuwvq.sHtML

crypto.randomUUID()
来源：http://baike.fanxiaobao.xyz/Article/details/ghllzlacm.sHtML

[U116] JS：类型检查（JSDoc）
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gamoeqwbm.sHtML

/** @param {string} name */ function f(name) {}
来源：http://baike.fanxiaobao.xyz/Article/details/gjgcmwksw.sHtML

[U117] JS：单元测试
来源：http://wap.fanxiaobao.xyz/Article/details/gflixirkn.sHtML

npm i -D vitest;  npx vitest
来源：http://www.share.fanxiaobao.xyz/Article/details/gihwpdbhv.sHtML

[U118] JS：开发服务器
来源：http://mobile.fanxiaobao.xyz/Article/details/gqvbvfelv.sHtML

npm i -D vite;  npx vite
来源：http://www.blog.fanxiaobao.xyz/Article/details/gjdtvmvnf.sHtML

[U119] JS：生产构建
来源：http://read.share.fanxiaobao.xyz/Article/details/gszvbudma.sHtML

npx vite build
来源：http://wap.fanxiaobao.xyz/Article/details/guigwaxba.sHtML

[U120] JS：读取环境变量（Vite）
来源：http://m.share.fanxiaobao.xyz/Article/details/gynaynnsr.sHtML

import.meta.env.VITE_API_URL
来源：http://m.share.fanxiaobao.xyz/Article/details/gghdwethg.sHtML

================================================================================
来源：http://m.share.fanxiaobao.xyz/Article/details/gigmhmqzy.sHtML

统计汇总
来源：http://mobile.fanxiaobao.xyz/Article/details/gymrmhyah.sHtML

================================================================================
来源：http://mobile.fanxiaobao.xyz/Article/details/gpzuhaxnp.sHtML

按语言统计（条）：
来源：http://wap.fanxiaobao.xyz/Article/details/gbivkalzs.sHtML

Python ......... 252
来源：http://m.share.fanxiaobao.xyz/Article/details/gruoebync.sHtML

PHP ............ 252
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gwnhsovmc.sHtML

JavaScript ..... 252
来源：http://www.share.fanxiaobao.xyz/Article/details/gofhcwqry.sHtML

TypeScript ..... 212
来源：http://www.m.share.fanxiaobao.xyz/Article/details/ggpriamwv.sHtML

Java ........... 212
来源：http://www.blog.fanxiaobao.xyz/Article/details/gmubznsnb.sHtML

Go ............. 212
来源：http://m.share.fanxiaobao.xyz/Article/details/gpyvnmupm.sHtML

Ruby ........... 212
来源：http://wap.fanxiaobao.xyz/Article/details/gkcichyjr.sHtML

C# ............. 212
来源：http://www.blog.fanxiaobao.xyz/Article/details/gmoojsikv.sHtML

C .............. 30
来源：http://www.blog.fanxiaobao.xyz/Article/details/gnsenwybc.sHtML

C++ ............ 30
来源：http://www.share.fanxiaobao.xyz/Article/details/gsvdiqgcs.sHtML

SQL ............ 90
来源：http://mobile.fanxiaobao.xyz/Article/details/gzviigkgw.sHtML

Bash ........... 80
来源：http://www.m.share.fanxiaobao.xyz/Article/details/grmqsmivh.sHtML

Kotlin ......... 15
来源：http://baike.fanxiaobao.xyz/Article/details/gcauxotmn.sHtML

Swift .......... 15
来源：http://baike.fanxiaobao.xyz/Article/details/gngzfqvae.sHtML

Lua ............ 10
来源：http://read.share.fanxiaobao.xyz/Article/details/gkvkxlgib.sHtML

Perl ........... 10
来源：http://www.share.fanxiaobao.xyz/Article/details/ggkwnehvq.sHtML

Scala .......... 10
来源：http://baike.fanxiaobao.xyz/Article/details/gtsscccqs.sHtML

------------------------------------
来源：http://baike.fanxiaobao.xyz/Article/details/gulidygow.sHtML

合计 ........... 2106 条
来源：http://www.share.fanxiaobao.xyz/Article/details/gcvplmkgo.sHtML

按章节统计：
来源：http://www.blog.fanxiaobao.xyz/Article/details/gwsrlpcpp.sHtML

A 基础语法与类型       26 个任务 × 8 语言 =  208
来源：http://read.share.fanxiaobao.xyz/Article/details/gskvflquq.sHtML

B 流程控制             16 个任务 × 8 语言 =  128
来源：http://mobile.fanxiaobao.xyz/Article/details/gfzmumdsx.sHtML

C 函数与作用域         16 个任务 × 8 语言 =  128
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gzcqawazu.sHtML

D 数组 / 列表 / 集合   26 个任务 × 8 语言 =  208
来源：http://m.share.fanxiaobao.xyz/Article/details/gtsfukoxi.sHtML

E 字符串处理           22 个任务 × 8 语言 =  176
来源：http://www.share.fanxiaobao.xyz/Article/details/gyodfhmec.sHtML

F 文件与目录           12 个任务 × 8 语言 =   96
来源：http://read.share.fanxiaobao.xyz/Article/details/gqeqbmakd.sHtML

G 面向对象             16 个任务 × 8 语言 =  128
来源：http://blog.fanxiaobao.xyz/Article/details/gotmhqitn.sHtML

H 异常与错误处理       10 个任务 × 8 语言 =   80
来源：http://m.share.fanxiaobao.xyz/Article/details/gmnoypydd.sHtML

I 正则表达式            8 个任务 × 8 语言 =   64
来源：http://mobile.fanxiaobao.xyz/Article/details/glvnjrofv.sHtML

J 日期与时间           10 个任务 × 8 语言 =   80
来源：http://www.share.fanxiaobao.xyz/Article/details/gxxtitkmm.sHtML

K JSON 与序列化         8 个任务 × 8 语言 =   64
来源：http://www.share.fanxiaobao.xyz/Article/details/gbeuwvgjj.sHtML

L 网络请求              8 个任务 × 8 语言 =   64
来源：http://www.share.fanxiaobao.xyz/Article/details/gqdxsdjch.sHtML

M 命令行 / 进程         8 个任务 × 8 语言 =   64
来源：http://read.share.fanxiaobao.xyz/Article/details/gwejbxndd.sHtML

N 数据结构与算法       12 个任务 × 8 语言 =   96
来源：http://m.share.fanxiaobao.xyz/Article/details/gbvhtodoe.sHtML

O 并发与异步            6 个任务 × 8 语言 =   48
来源：http://wap.fanxiaobao.xyz/Article/details/gmcuekctc.sHtML

P 常用工具函数          8 个任务 × 8 语言 =   64
来源：http://mobile.fanxiaobao.xyz/Article/details/gifncfyfr.sHtML

Q SQL 专题                              90
来源：http://www.blog.fanxiaobao.xyz/Article/details/gahzllnsr.sHtML

R Bash 专题                             80
来源：http://read.share.fanxiaobao.xyz/Article/details/glzbkbary.sHtML

S C / C++ 专题                          60
来源：http://www.share.fanxiaobao.xyz/Article/details/goghxoskl.sHtML

T 其他语言补充                          60
来源：http://blog.fanxiaobao.xyz/Article/details/gpmtenfdu.sHtML

U 高频实用片段                         120
来源：http://m.share.fanxiaobao.xyz/Article/details/gqnznkqbq.sHtML

------------------------------------
来源：http://baike.fanxiaobao.xyz/Article/details/gmvlcmzzb.sHtML

合计                                  2106 条
来源：http://read.share.fanxiaobao.xyz/Article/details/gjcdoxitx.sHtML

--------------------------------------------------------------------------------
来源：http://www.share.fanxiaobao.xyz/Article/details/gybxknuzz.sHtML

使用提醒
来源：http://wap.fanxiaobao.xyz/Article/details/gjcerdybj.sHtML

--------------------------------------------------------------------------------
来源：http://wap.fanxiaobao.xyz/Article/details/gaarqhqgq.sHtML

1. 示例追求"最小可用"，正式项目中请补齐导入、错误处理与边界判断。
来源：http://mobile.fanxiaobao.xyz/Article/details/goornsssi.sHtML

2. 涉及文件、网络、数据库的示例，注意资源释放与异常捕获。
来源：http://mobile.fanxiaobao.xyz/Article/details/gesmwauyc.sHtML

3. 语言版本差异较大（如 Python 3.10 的 match、Java 17 的 record/switch 箭头），
来源：http://3g.fanxiaobao.xyz/Article/details/gcienridx.sHtML

在旧版本上使用前请先确认语法支持情况。
来源：http://blog.fanxiaobao.xyz/Article/details/gnkbefmzt.sHtML

4. 标注"手写"的条目是因为该语言缺少对应内置能力，实际项目中可引入成熟库。
来源：http://read.share.fanxiaobao.xyz/Article/details/gbbqhatwd.sHtML

—— 文件结束 ——
来源：http://blog.fanxiaobao.xyz/Article/details/gsykljdve.sHtML

================================================================================
来源：http://read.share.fanxiaobao.xyz/Article/details/gncmfscvg.sHtML

程序语言常见例子速查手册（2024 版）
来源：http://3g.fanxiaobao.xyz/Article/details/gxszhlxeb.sHtML

Common Programming Examples Cheat Book
来源：http://read.share.fanxiaobao.xyz/Article/details/gpugmezhe.sHtML

================================================================================
来源：http://baike.fanxiaobao.xyz/Article/details/gpbzcqhgm.sHtML

【收录内容】
来源：http://blog.fanxiaobao.xyz/Article/details/gevrrmedu.sHtML

覆盖 12 种语言 / 语法与常见 API：
来源：http://www.blog.fanxiaobao.xyz/Article/details/gpkghxndr.sHtML

Python · PHP · JavaScript · TypeScript · Java · Go · Ruby · C#
来源：http://3g.fanxiaobao.xyz/Article/details/gluzvrifk.sHtML

SQL · Bash · C · C++
来源：http://baike.fanxiaobao.xyz/Article/details/gokbhqesz.sHtML

按「任务」分组：每个任务下按语言各给出一条最小可用示例。
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gbskjxqtl.sHtML

【使用说明】
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gkdwcfkah.sHtML

1. 每个任务形如 "[编号] 任务名"，下面每行以语言标记开头：
来源：http://mobile.fanxiaobao.xyz/Article/details/gcemniynv.sHtML

Py:    Python        PHP:   PHP           JS:    JavaScript
来源：http://blog.fanxiaobao.xyz/Article/details/gplqagthb.sHtML

TS:    TypeScript    Java:  Java          Go:    Go
来源：http://read.share.fanxiaobao.xyz/Article/details/gluqasuer.sHtML

Ruby:  Ruby          C#:    C#            SQL:   SQL
来源：http://blog.fanxiaobao.xyz/Article/details/ghacwxgrp.sHtML

Bash:  Shell         C:     C             C++:   C++
来源：http://baike.fanxiaobao.xyz/Article/details/gjenjoxvl.sHtML

2. 示例只展示核心写法，刻意省略 import / require / include / using 等样板代码。
来源：http://baike.fanxiaobao.xyz/Article/details/gebbvzqcb.sHtML

需要完整可运行文件时，请自行补齐当前语言的导入语句。
来源：http://m.share.fanxiaobao.xyz/Article/details/gjudmeank.sHtML

3. 语法基准：Python 3.10+ / PHP 8.1+ / ES2020+ / TypeScript 5 / Java 17 /
来源：http://m.share.fanxiaobao.xyz/Article/details/gdkopiqxx.sHtML

Go 1.21+ / Ruby 3.x / C# 10+ / C17 / C++17。
来源：http://m.share.fanxiaobao.xyz/Article/details/gckypfiaz.sHtML

4. 检索建议：用编辑器或浏览器 Ctrl+F 搜关键词，如 "排序" "读取文件" "正则"。
来源：http://baike.fanxiaobao.xyz/Article/details/gvlxjkgof.sHtML

5. 标记为 "// 无" 表示该语言没有对应的一等语法，需用替代写法（示例给出替代方案）。
来源：http://mobile.fanxiaobao.xyz/Article/details/gmwvhjplz.sHtML

6. 符号 "⏎" 表示代码在此处换行（主要用于 Python 等强制缩进、无法压成一行的结构）。
来源：http://www.share.fanxiaobao.xyz/Article/details/gjwonmuya.sHtML

【文件统计】
来源：http://www.blog.fanxiaobao.xyz/Article/details/gwdlgxdwd.sHtML

语言示例共 2106 条，分布见本文末尾的「统计汇总」。
来源：http://blog.fanxiaobao.xyz/Article/details/gsamvxtjw.sHtML

--------------------------------------------------------------------------------
来源：http://blog.fanxiaobao.xyz/Article/details/guwgmztxv.sHtML

目  录
来源：http://3g.fanxiaobao.xyz/Article/details/gzgcrmxma.sHtML

--------------------------------------------------------------------------------
来源：http://3g.fanxiaobao.xyz/Article/details/gczpwxljw.sHtML

A. 基础语法与类型              （第 1 节，26 个任务，208 条）
来源：http://m.share.fanxiaobao.xyz/Article/details/gxlduxcjo.sHtML

B. 流程控制                    （第 2 节，16 个任务，128 条）
来源：http://baike.fanxiaobao.xyz/Article/details/gstjspnld.sHtML

C. 函数与作用域                （第 3 节，16 个任务，128 条）
来源：http://blog.fanxiaobao.xyz/Article/details/gsmvdtgya.sHtML

D. 数组 / 列表 / 集合          （第 4 节，26 个任务，208 条）
来源：http://m.share.fanxiaobao.xyz/Article/details/gnwqmfozm.sHtML

E. 字符串处理                  （第 5 节，22 个任务，176 条）
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gmagrtkgo.sHtML

F. 文件与目录                  （第 6 节，12 个任务，96 条）
来源：http://mobile.fanxiaobao.xyz/Article/details/gcozikqyi.sHtML

G. 面向对象                    （第 7 节，16 个任务，128 条）
来源：http://www.blog.fanxiaobao.xyz/Article/details/gfvvupunu.sHtML

H. 异常与错误处理              （第 8 节，10 个任务，80 条）
来源：http://blog.fanxiaobao.xyz/Article/details/gnbwmvmjh.sHtML

I. 正则表达式                  （第 9 节，8 个任务，64 条）
来源：http://mobile.fanxiaobao.xyz/Article/details/gpxkpqpup.sHtML

J. 日期与时间                  （第 10 节，10 个任务，80 条）
来源：http://www.blog.fanxiaobao.xyz/Article/details/gvfqcvnyy.sHtML

K. JSON 与序列化               （第 11 节，8 个任务，64 条）
来源：http://wap.fanxiaobao.xyz/Article/details/gxccyvkre.sHtML

L. 网络请求                    （第 12 节，8 个任务，64 条）
来源：http://3g.fanxiaobao.xyz/Article/details/gsixfrzic.sHtML

M. 命令行 / 进程 / 环境        （第 13 节，8 个任务，64 条）
来源：http://mobile.fanxiaobao.xyz/Article/details/glojgwbez.sHtML

N. 数据结构与算法              （第 14 节，12 个任务，96 条）
来源：http://mobile.fanxiaobao.xyz/Article/details/gbcomgrnj.sHtML

O. 并发与异步                  （第 15 节，6 个任务，48 条）
来源：http://www.share.fanxiaobao.xyz/Article/details/gqugylcyx.sHtML

P. 常用工具函数                （第 16 节，8 个任务，64 条）
来源：http://read.share.fanxiaobao.xyz/Article/details/gfpczttae.sHtML

Q. SQL 专题                    （第 17 节，90 条）
来源：http://www.blog.fanxiaobao.xyz/Article/details/gljzmobnk.sHtML

R. Bash 专题                   （第 18 节，80 条）
来源：http://blog.fanxiaobao.xyz/Article/details/gmqndubdl.sHtML

S. C / C++ 专题                （第 19 节，60 条）
来源：http://m.share.fanxiaobao.xyz/Article/details/gfxvcjqas.sHtML

T. 其他语言补充                （第 20 节，60 条：Kotlin / Swift / Lua / Perl / Scala）
来源：http://3g.fanxiaobao.xyz/Article/details/guitqwcdy.sHtML

U. 高频实用片段                （第 21 节，120 条：Python / PHP / JavaScript 各 40 条）
来源：http://mobile.fanxiaobao.xyz/Article/details/gqnajuetg.sHtML


<!-- 参考信息 -->