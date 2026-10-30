代发 wailian999

[U21] Py：自定义上下文管理器
来源：http://blog.hesvh.cn/Article/details/gzyujkdin.sHtML

@contextlib.contextmanager
来源：http://www.blog.fehbvm.com/Article/details/gfvmzkttv.sHtML

[U22] Py：矩阵转置
来源：http://baike.hesvh.cn/Article/details/gpvilnvbl.sHtML

list(zip(*m))
来源：http://wap.fehbvm.com/Article/details/gqvltgjzg.sHtML

[U23] Py：分块读取大文件
来源：http://www.m.share.hesvh.cn/Article/details/guertgywg.sHtML

for chunk in iter(lambda: f.read(8192), b""):
来源：http://mobile.fehbvm.com/Article/details/giftqewgd.sHtML

[U24] Py：路径操作
来源：http://www.share.hesvh.cn/Article/details/gimdlrfbx.sHtML

Path("a/b.txt").parent.mkdir(parents=True, exist_ok=True)
来源：http://www.blog.zdbjq.cn/Article/details/gtsuofanb.sHtML

[U25] Py：CSV 按字典读
来源：http://baike.zdbjq.cn/Article/details/gdlefkaxk.sHtML

csv.DictReader(f)
来源：http://blog.hesvh.cn/Article/details/gjjauxivp.sHtML

[U26] Py：并发下载
来源：http://www.share.fehbvm.com/Article/details/gsvfdjtso.sHtML

ThreadPoolExecutor(max_workers=8).map(fetch, urls)
来源：http://www.blog.zdbjq.cn/Article/details/gdmjnhwor.sHtML

[U27] Py：异步 HTTP
来源：http://blog.hesvh.cn/Article/details/gwemwomwd.sHtML

aiohttp.ClientSession() 配合 async with
来源：http://read.share.zdbjq.cn/Article/details/gihsrpfdt.sHtML

[U28] Py：类型别名
来源：http://www.share.hesvh.cn/Article/details/gqamqdkmt.sHtML

UserId = int
来源：http://mobile.fehbvm.com/Article/details/ggzxefron.sHtML

[U29] Py：属性校验
来源：http://www.blog.fehbvm.com/Article/details/gicckdcdx.sHtML

@property 与 @x.setter 配合
来源：http://m.share.zdbjq.cn/Article/details/gtafuknxl.sHtML

[U30] Py：数据类
来源：http://mobile.fehbvm.com/Article/details/gxkxcggbs.sHtML

@dataclass(slots=True)
来源：http://3g.fehbvm.com/Article/details/glkljoojq.sHtML

[U31] Py：单测
来源：http://wap.zdbjq.cn/Article/details/gooitpoim.sHtML

python -m pytest -q
来源：http://mobile.fehbvm.com/Article/details/gfweqeuwa.sHtML

[U32] Py：代码格式化
来源：http://3g.zdbjq.cn/Article/details/gpwymkzfr.sHtML

ruff format . && ruff check --fix .
来源：http://wap.zdbjq.cn/Article/details/gpjtycgpm.sHtML

[U33] Py：打包发布
来源：http://www.blog.hesvh.cn/Article/details/ggcbskflt.sHtML

python -m build  （依赖 pyproject.toml）
来源：http://blog.fehbvm.com/Article/details/gqjmlrhgs.sHtML

[U34] Py：判断编码
来源：http://www.blog.zdbjq.cn/Article/details/gonnqarhm.sHtML

chardet.detect(raw)
来源：http://mobile.fehbvm.com/Article/details/gnqvwvjxe.sHtML

[U35] Py：发送邮件
来源：http://wap.zdbjq.cn/Article/details/ghasrbini.sHtML

smtplib.SMTP_SSL(...).send_message(msg)
来源：http://read.share.zdbjq.cn/Article/details/gdfchkdtx.sHtML

[U36] Py：定时任务
来源：http://www.blog.hesvh.cn/Article/details/gvsiiwort.sHtML

schedule.every(10).minutes.do(job)
来源：http://www.blog.fehbvm.com/Article/details/gxfflazhi.sHtML

[U37] Py：读写 Excel
来源：http://3g.zdbjq.cn/Article/details/gqsglfbzq.sHtML

pandas.read_excel / DataFrame.to_excel
来源：http://baike.zdbjq.cn/Article/details/gmndqzbvm.sHtML

[U38] Py：获取脚本所在目录
来源：http://www.share.hesvh.cn/Article/details/gwvoqgmyg.sHtML

Path(__file__).resolve().parent
来源：http://mobile.zdbjq.cn/Article/details/gbwhzjqaj.sHtML

[U39] Py：判断是否在交互环境
来源：http://www.m.share.zdbjq.cn/Article/details/ggwzxprvx.sHtML

sys.stdout.isatty()
来源：http://wap.fehbvm.com/Article/details/gqeoqxhow.sHtML

[U40] Py：打印到标准错误
来源：http://baike.hesvh.cn/Article/details/gybvwvepi.sHtML

print("err", file=sys.stderr)
来源：http://www.m.share.fehbvm.com/Article/details/gevwuwycg.sHtML

[U41] PHP：初始化 Composer 项目
来源：http://blog.zdbjq.cn/Article/details/gmginefxp.sHtML

composer init;  composer require guzzlehttp/guzzle
来源：http://wap.hesvh.cn/Article/details/giefaafhz.sHtML

[U42] PHP：PSR-4 自动加载
来源：http://m.share.zdbjq.cn/Article/details/gkpwcamki.sHtML

"autoload": { "psr-4": { "App\\": "src/" } }
来源：http://www.blog.zdbjq.cn/Article/details/gmdnibzgq.sHtML

[U43] PHP：声明命名空间
来源：http://read.share.hesvh.cn/Article/details/gkodlfrwl.sHtML

namespace App\Http;
来源：http://blog.fehbvm.com/Article/details/guzowkvut.sHtML

[U44] PHP：开启严格类型
来源：http://3g.zdbjq.cn/Article/details/gkgpnjeji.sHtML

declare(strict_types=1);
来源：http://www.m.share.hesvh.cn/Article/details/gfkewtyiv.sHtML

[U45] PHP：类型声明与返回类型
来源：http://www.share.fehbvm.com/Article/details/ggocatlvb.sHtML

function add(int $a, int $b): int { return $a + $b; }
来源：http://www.blog.hesvh.cn/Article/details/gjaboxjqz.sHtML

[U46] PHP：可空类型
来源：http://blog.zdbjq.cn/Article/details/gshvybcdu.sHtML

?string $name = null
来源：http://m.share.fehbvm.com/Article/details/gzzqqoaor.sHtML

[U47] PHP：联合类型
来源：http://wap.hesvh.cn/Article/details/gxjrhedtl.sHtML

int|string $id
来源：http://blog.hesvh.cn/Article/details/gtsmfgluj.sHtML

[U48] PHP：纯枚举
来源：http://wap.hesvh.cn/Article/details/gjekpejxx.sHtML

enum Status: string { case Active = "active"; case Off = "off"; }
来源：http://read.share.zdbjq.cn/Article/details/gkemjrbah.sHtML

[U49] PHP：只读属性
来源：http://m.share.fehbvm.com/Article/details/gndaawabn.sHtML

public readonly string $name
来源：http://wap.zdbjq.cn/Article/details/gayecgahr.sHtML

[U50] PHP：构造器属性提升
来源：http://www.share.fehbvm.com/Article/details/geasttpob.sHtML

public function __construct(private int $id) {}
来源：http://www.blog.zdbjq.cn/Article/details/gfbizufaj.sHtML

[U51] PHP：数组解构
来源：http://read.share.zdbjq.cn/Article/details/gikomhhae.sHtML

[$a, $b] = $arr;
来源：http://www.blog.zdbjq.cn/Article/details/gkvwivpux.sHtML

[U52] PHP：箭头函数
来源：http://read.share.hesvh.cn/Article/details/grmbwdsiz.sHtML

$double = fn($x) => $x * 2;
来源：http://www.blog.zdbjq.cn/Article/details/gbqkmqjgm.sHtML

[U53] PHP：空合并运算符
来源：http://wap.hesvh.cn/Article/details/gcbsybzqh.sHtML

$v = $a ?? $b ?? "default";
来源：http://baike.hesvh.cn/Article/details/gsjrmbpdh.sHtML

[U54] PHP：空安全调用
来源：http://m.share.zdbjq.cn/Article/details/gmzyxdqec.sHtML

$obj?->method()
来源：http://3g.fehbvm.com/Article/details/gpjkzcplc.sHtML

[U55] PHP：match 表达式
来源：http://3g.zdbjq.cn/Article/details/gveoprwug.sHtML

$s = match($x) { 1 => "一", default => "其他" };
来源：http://baike.hesvh.cn/Article/details/gzkubkwul.sHtML

[U56] PHP：命名参数
来源：http://blog.hesvh.cn/Article/details/gyxovvjpn.sHtML

f(a: 1, b: 2)
来源：http://www.m.share.hesvh.cn/Article/details/gzvicniws.sHtML

[U57] PHP：字符串插值
来源：http://read.share.fehbvm.com/Article/details/glxujekwa.sHtML

"值: {$a}"
来源：http://3g.hesvh.cn/Article/details/gdgtnmxcv.sHtML

[U58] PHP：数组三件套
来源：http://www.m.share.fehbvm.com/Article/details/gdetfsbcm.sHtML

array_map($f, $a);  array_filter($a, $f);  array_reduce($a, $f, 0);
来源：http://www.blog.zdbjq.cn/Article/details/geaduiihv.sHtML

[U59] PHP：自定义排序
来源：http://www.m.share.fehbvm.com/Article/details/gombevfis.sHtML

usort($arr, fn($a, $b) => $a["age"] <=> $b["age"]);
来源：http://read.share.hesvh.cn/Article/details/getnoteqr.sHtML

[U60] PHP：JSON 编解码
来源：http://www.m.share.zdbjq.cn/Article/details/gfetxpxzv.sHtML

json_encode($d, JSON_UNESCAPED_UNICODE);  json_decode($s, true);
来源：http://baike.hesvh.cn/Article/details/gyueysnba.sHtML

[U61] PHP：正则
来源：http://blog.hesvh.cn/Article/details/gfvilbnxm.sHtML

preg_match('/(\d+)/', $s, $m);  preg_replace('/\d+/', '#', $s);
来源：http://www.m.share.zdbjq.cn/Article/details/gadnqjazf.sHtML

[U62] PHP：日期对象
来源：http://read.share.zdbjq.cn/Article/details/gtpflyimz.sHtML

(new DateTimeImmutable())->format("Y-m-d");
来源：http://www.blog.zdbjq.cn/Article/details/gddhbmokw.sHtML

[U63] PHP：文件读写
来源：http://www.blog.zdbjq.cn/Article/details/gdyhsjweq.sHtML

file_get_contents($f);  file_put_contents($f, $data);
来源：http://read.share.fehbvm.com/Article/details/gbgwkuayo.sHtML

[U64] PHP：目录遍历
来源：http://3g.zdbjq.cn/Article/details/ghaakztlz.sHtML

glob("dir/*.php");  scandir("dir");
来源：http://www.m.share.fehbvm.com/Article/details/gnsoywawl.sHtML

[U65] PHP：会话
来源：http://blog.fehbvm.com/Article/details/gsuqncgcu.sHtML

session_start();  $_SESSION["uid"] = 1;
来源：http://m.share.fehbvm.com/Article/details/gxlcvuqlq.sHtML

[U66] PHP：设置 Cookie
来源：http://www.m.share.fehbvm.com/Article/details/goahzrbdx.sHtML

setcookie("token", $v, ["httponly" => true, "samesite" => "Lax"]);
来源：http://read.share.hesvh.cn/Article/details/gohkdxpfg.sHtML

[U67] PHP：处理文件上传
来源：http://mobile.hesvh.cn/Article/details/gcaycmgzi.sHtML

$_FILES["file"]["tmp_name"] 与 move_uploaded_file()
来源：http://blog.zdbjq.cn/Article/details/gltznvrop.sHtML

[U68] PHP：PDO 连接
来源：http://m.share.fehbvm.com/Article/details/ggmosmckx.sHtML

$pdo = new PDO("mysql:host=localhost;dbname=app", "root", "");
来源：http://wap.zdbjq.cn/Article/details/gacbzqmfo.sHtML

[U69] PHP：PDO 预处理
来源：http://wap.zdbjq.cn/Article/details/gzkloinai.sHtML

$stmt = $pdo->prepare("SELECT * FROM users WHERE id = ?");  $stmt->execute([$id]);
来源：http://3g.hesvh.cn/Article/details/gzvxstdox.sHtML

[U70] PHP：PDO 事务
来源：http://www.m.share.zdbjq.cn/Article/details/gxkhhpzle.sHtML

$pdo->beginTransaction();  $pdo->commit();  $pdo->rollBack();
来源：http://www.m.share.fehbvm.com/Article/details/gvfcnovjv.sHtML

[U71] PHP：抛出异常
来源：http://www.blog.hesvh.cn/Article/details/gkbympmqm.sHtML

throw new RuntimeException("失败", 500);
来源：http://read.share.fehbvm.com/Article/details/gmzuyakqx.sHtML

[U72] PHP：写错误日志
来源：http://mobile.zdbjq.cn/Article/details/gphbqwbhr.sHtML

error_log("失败: " . $e->getMessage());
来源：http://www.blog.hesvh.cn/Article/details/gcsnwqwxp.sHtML

[U73] PHP：读取 ini 配置
来源：http://baike.hesvh.cn/Article/details/gornfbylo.sHtML

parse_ini_file("config.ini", true)
来源：http://www.blog.hesvh.cn/Article/details/gkhskikus.sHtML

[U74] PHP：读取环境变量
来源：http://www.m.share.fehbvm.com/Article/details/ghohmqfgk.sHtML

getenv("APP_ENV") ?: "production"
来源：http://wap.zdbjq.cn/Article/details/glxwwooii.sHtML

[U75] PHP：依赖注入
来源：http://www.blog.fehbvm.com/Article/details/gvjeytrzc.sHtML

composer require psr/container
来源：http://read.share.fehbvm.com/Article/details/gqjgkgsax.sHtML

[U76] PHP：简单路由
来源：http://baike.zdbjq.cn/Article/details/gesppejxh.sHtML

$path = parse_url($_SERVER["REQUEST_URI"], PHP_URL_PATH);
来源：http://mobile.fehbvm.com/Article/details/gdbeqitsm.sHtML

[U77] PHP：模板渲染
来源：http://m.share.hesvh.cn/Article/details/gwbfsllnb.sHtML

composer require twig/twig
来源：http://blog.zdbjq.cn/Article/details/gkocajfux.sHtML

[U78] PHP：单元测试
来源：http://www.blog.zdbjq.cn/Article/details/gzhemdffw.sHtML

composer require --dev phpunit/phpunit
来源：http://read.share.zdbjq.cn/Article/details/gvpkmckcj.sHtML

[U79] PHP：静态分析
来源：http://blog.fehbvm.com/Article/details/ggemlowkm.sHtML

composer require --dev phpstan/phpstan
来源：http://read.share.hesvh.cn/Article/details/grtljmayc.sHtML

[U80] PHP：代码规范修复
来源：http://blog.fehbvm.com/Article/details/gmqlsjtea.sHtML

composer require --dev friendsofphp/php-cs-fixer
来源：http://wap.hesvh.cn/Article/details/gpbuakygi.sHtML

[U81] JS：初始化项目
来源：http://m.share.hesvh.cn/Article/details/gjtsyizdv.sHtML

npm init -y;  npm i express
来源：http://baike.hesvh.cn/Article/details/ghtwsdcev.sHtML

[U82] JS：package.json 脚本
来源：http://3g.fehbvm.com/Article/details/gmalmfbfr.sHtML

"scripts": { "dev": "vite", "build": "vite build" }
来源：http://www.m.share.hesvh.cn/Article/details/gxtcnacjz.sHtML

[U83] JS：ES Module 导入导出
来源：http://www.blog.hesvh.cn/Article/details/gpqtzkrxr.sHtML

export const a = 1;  import { a } from "./m.js";
来源：http://baike.zdbjq.cn/Article/details/gizxcflra.sHtML

[U84] JS：CommonJS 写法
来源：http://blog.zdbjq.cn/Article/details/gvviwdvxt.sHtML

module.exports = { a };  const { a } = require("./m");
来源：http://m.share.hesvh.cn/Article/details/gqnexcesw.sHtML

[U85] JS：可选链
来源：http://wap.zdbjq.cn/Article/details/gaqnsnvwd.sHtML

a?.b?.c
来源：http://baike.fehbvm.com/Article/details/goyhvzcii.sHtML

[U86] JS：空值合并
来源：http://www.share.hesvh.cn/Article/details/gvpecyzgn.sHtML

a ?? b
来源：http://www.m.share.fehbvm.com/Article/details/gtgbnmufx.sHtML

[U87] JS：解构默认值
来源：http://www.blog.hesvh.cn/Article/details/gagejhvzb.sHtML

const { a = 1, b = 2 } = obj;
来源：http://3g.zdbjq.cn/Article/details/gubjsnrho.sHtML

[U88] JS：对象展开合并
来源：http://www.m.share.fehbvm.com/Article/details/gaxiscmfo.sHtML

{ ...a, ...b }
来源：http://wap.fehbvm.com/Article/details/gfabcsvat.sHtML

[U89] JS：数组去重
来源：http://www.m.share.hesvh.cn/Article/details/gkuwxpkcu.sHtML

[...new Set(arr)]
来源：http://mobile.zdbjq.cn/Article/details/gflkqlhhw.sHtML

[U90] JS：数字数组排序
来源：http://baike.hesvh.cn/Article/details/gnphpvwes.sHtML

[...arr].sort((a, b) => a - b)
来源：http://m.share.zdbjq.cn/Article/details/gktrtrbff.sHtML

[U91] JS：对象键值遍历
来源：http://www.blog.fehbvm.com/Article/details/gckcmaxka.sHtML

Object.entries(obj).forEach(([k, v]) => {});
来源：http://www.share.hesvh.cn/Article/details/gtezkycwx.sHtML

[U92] JS：深拷贝
来源：http://www.m.share.zdbjq.cn/Article/details/gedbyjblf.sHtML

structuredClone(obj)
来源：http://blog.hesvh.cn/Article/details/gqgqcwact.sHtML

[U93] JS：模板字符串
来源：http://read.share.hesvh.cn/Article/details/gfxlpjwjd.sHtML

`共 ${n} 条`
来源：http://blog.hesvh.cn/Article/details/gtztjzyoj.sHtML

[U94] JS：箭头函数
来源：http://m.share.fehbvm.com/Article/details/gfthhmtuv.sHtML

const double = x => x * 2;
来源：http://www.blog.zdbjq.cn/Article/details/gmfblxxtw.sHtML

[U95] JS：Promise 包装
来源：http://read.share.fehbvm.com/Article/details/gbjgolaha.sHtML

new Promise((resolve, reject) => {})
来源：http://read.share.zdbjq.cn/Article/details/gpzrfsfyp.sHtML

[U96] JS：async/await 与异常
来源：http://www.blog.fehbvm.com/Article/details/gjlqdxmou.sHtML

try { const d = await f(); } catch (e) { console.error(e); }
来源：http://www.blog.zdbjq.cn/Article/details/gugbhlmfu.sHtML

[U97] JS：并发请求
来源：http://baike.hesvh.cn/Article/details/gknqzbgbm.sHtML

await Promise.all(urls.map(u => fetch(u)))
来源：http://blog.zdbjq.cn/Article/details/gffafkecd.sHtML

[U98] JS：fetch 带 JSON
来源：http://baike.hesvh.cn/Article/details/gadeoyosg.sHtML

await fetch(url, { method: "POST", headers: { "Content-Type": "application/json" }, body: JSON.stringify(d) })
来源：http://blog.fehbvm.com/Article/details/gegqpzjtm.sHtML

[U99] JS：事件监听
来源：http://www.m.share.zdbjq.cn/Article/details/gzfhyfuog.sHtML

el.addEventListener("click", e => {})
来源：http://www.blog.fehbvm.com/Article/details/gwkvibgxn.sHtML

[U100] JS：DOM 查询
来源：http://3g.zdbjq.cn/Article/details/gntxbplte.sHtML

document.querySelector(".item")
来源：http://wap.zdbjq.cn/Article/details/gapvkizjm.sHtML

[U101] JS：classList 操作
来源：http://mobile.hesvh.cn/Article/details/gnkywxocq.sHtML

el.classList.toggle("active")
来源：http://www.share.hesvh.cn/Article/details/gwzyzwkmr.sHtML

[U102] JS：本地存储
来源：http://blog.zdbjq.cn/Article/details/gapnqqjot.sHtML

localStorage.setItem("k", JSON.stringify(v))
来源：http://blog.hesvh.cn/Article/details/ghfbqtndb.sHtML

[U103] JS：定时器
来源：http://3g.hesvh.cn/Article/details/gftfnkuoh.sHtML

setTimeout(fn, 1000);  setInterval(fn, 1000);
来源：http://www.share.fehbvm.com/Article/details/gtvtazluh.sHtML

[U104] JS：防抖
来源：http://mobile.fehbvm.com/Article/details/gfwjpypop.sHtML

const debounce = (fn, ms) => { let t; return (...a) => { clearTimeout(t); t = setTimeout(() => fn(...a), ms); }; };
来源：http://www.m.share.zdbjq.cn/Article/details/guqihksqq.sHtML

[U105] JS：节流
来源：http://www.blog.fehbvm.com/Article/details/gilpfrugl.sHtML

const throttle = (fn, ms) => { let last = 0; return (...a) => { const n = Date.now(); if (n - last >= ms) { last = n; fn(...a); } }; };
来源：http://wap.zdbjq.cn/Article/details/gnvrhyfdr.sHtML

[U106] JS：日期格式化
来源：http://read.share.hesvh.cn/Article/details/gmrjyjehf.sHtML

new Intl.DateTimeFormat("zh-CN", { dateStyle: "medium" }).format(new Date())
来源：http://www.m.share.zdbjq.cn/Article/details/giroywtyz.sHtML

[U107] JS：数字千分位
来源：http://www.m.share.hesvh.cn/Article/details/grbbvtarc.sHtML

new Intl.NumberFormat("en-US").format(1234567)
来源：http://m.share.fehbvm.com/Article/details/gfieggzrf.sHtML

[U108] JS：随机整数
来源：http://www.m.share.hesvh.cn/Article/details/gqyueagux.sHtML

Math.floor(Math.random() * (max - min + 1)) + min
来源：http://read.share.zdbjq.cn/Article/details/gdhefjvdh.sHtML

[U109] JS：数组分组
来源：http://m.share.hesvh.cn/Article/details/gjckglucw.sHtML

Object.groupBy(arr, x => x.type)
来源：http://read.share.zdbjq.cn/Article/details/gczwmvzlq.sHtML

[U110] JS：数组分块
来源：http://wap.hesvh.cn/Article/details/guaoxdnhn.sHtML

arr.reduce((acc, x, i) => (i % size ? acc : [...acc, arr.slice(i, i + size)]), [])
来源：http://3g.zdbjq.cn/Article/details/gskdtfjly.sHtML

[U111] JS：对象转 Map
来源：http://blog.hesvh.cn/Article/details/gxxdusgmc.sHtML

new Map(Object.entries(obj))
来源：http://3g.zdbjq.cn/Article/details/ggrnskyud.sHtML

[U112] JS：字符串补位
来源：http://read.share.hesvh.cn/Article/details/gyuhnzjjd.sHtML

"7".padStart(3, "0")
来源：http://baike.fehbvm.com/Article/details/gvmjufmjr.sHtML

[U113] JS：正则替换全部
来源：http://www.blog.hesvh.cn/Article/details/ggpmpyqur.sHtML

s.replaceAll("a", "b")
来源：http://www.m.share.fehbvm.com/Article/details/gicxkofkp.sHtML

[U114] JS：JSON 深比较
来源：http://blog.hesvh.cn/Article/details/gtnlnvkbz.sHtML

JSON.stringify(a) === JSON.stringify(b)
来源：http://read.share.zdbjq.cn/Article/details/gaeketlmh.sHtML

[U115] JS：生成 UUID
来源：http://www.m.share.fehbvm.com/Article/details/gsgaspmon.sHtML

crypto.randomUUID()
来源：http://mobile.zdbjq.cn/Article/details/gkzyoswzx.sHtML

[U116] JS：类型检查（JSDoc）
来源：http://mobile.hesvh.cn/Article/details/gecjorlhq.sHtML

/** @param {string} name */ function f(name) {}
来源：http://baike.zdbjq.cn/Article/details/gkayuhfsu.sHtML

[U117] JS：单元测试
来源：http://www.share.fehbvm.com/Article/details/gjguejcck.sHtML

npm i -D vitest;  npx vitest
来源：http://www.m.share.fehbvm.com/Article/details/gitldjplr.sHtML

[U118] JS：开发服务器
来源：http://mobile.fehbvm.com/Article/details/ggnuczwlu.sHtML

npm i -D vite;  npx vite
来源：http://baike.hesvh.cn/Article/details/grdmxiwct.sHtML

[U119] JS：生产构建
来源：http://www.blog.hesvh.cn/Article/details/gvocgazdk.sHtML

npx vite build
来源：http://www.blog.hesvh.cn/Article/details/ggkukrfrz.sHtML

[U120] JS：读取环境变量（Vite）
来源：http://wap.fehbvm.com/Article/details/guolftvts.sHtML

import.meta.env.VITE_API_URL
来源：http://m.share.zdbjq.cn/Article/details/gabqdlruy.sHtML

================================================================================
来源：http://m.share.fehbvm.com/Article/details/gjojaubry.sHtML

统计汇总
来源：http://www.share.zdbjq.cn/Article/details/gnbccwbib.sHtML

================================================================================
来源：http://blog.hesvh.cn/Article/details/grjupqghc.sHtML

按语言统计（条）：
来源：http://3g.zdbjq.cn/Article/details/gorlhuvjr.sHtML

Python ......... 252
来源：http://mobile.fehbvm.com/Article/details/gjpbbgwej.sHtML

PHP ............ 252
来源：http://read.share.fehbvm.com/Article/details/gmjkdjzbt.sHtML

JavaScript ..... 252
来源：http://blog.fehbvm.com/Article/details/gxmblvofv.sHtML

TypeScript ..... 212
来源：http://wap.fehbvm.com/Article/details/gpxeguyjg.sHtML

Java ........... 212
来源：http://m.share.hesvh.cn/Article/details/gdxkxuhwn.sHtML

Go ............. 212
来源：http://m.share.fehbvm.com/Article/details/gbgurbxan.sHtML

Ruby ........... 212
来源：http://m.share.zdbjq.cn/Article/details/gdyzcdonq.sHtML

C# ............. 212
来源：http://baike.hesvh.cn/Article/details/gcsxpzger.sHtML

C .............. 30
来源：http://3g.hesvh.cn/Article/details/glmwvuyyt.sHtML

C++ ............ 30
来源：http://read.share.fehbvm.com/Article/details/gysjnwcak.sHtML

SQL ............ 90
来源：http://www.m.share.hesvh.cn/Article/details/gvgpovakz.sHtML

Bash ........... 80
来源：http://m.share.zdbjq.cn/Article/details/gmqajipam.sHtML

Kotlin ......... 15
来源：http://blog.fehbvm.com/Article/details/gnoxybnru.sHtML

Swift .......... 15
来源：http://3g.hesvh.cn/Article/details/gwvnvzwgw.sHtML

Lua ............ 10
来源：http://www.blog.zdbjq.cn/Article/details/geduletmo.sHtML

Perl ........... 10
来源：http://blog.fehbvm.com/Article/details/gldbihlqr.sHtML

Scala .......... 10
来源：http://mobile.zdbjq.cn/Article/details/gwxvavpdo.sHtML

------------------------------------
来源：http://www.m.share.fehbvm.com/Article/details/gewvedgkj.sHtML

合计 ........... 2106 条
来源：http://wap.hesvh.cn/Article/details/gkunrydub.sHtML

按章节统计：
来源：http://3g.zdbjq.cn/Article/details/gafoailrv.sHtML

A 基础语法与类型       26 个任务 × 8 语言 =  208
来源：http://wap.fehbvm.com/Article/details/gnnbacuki.sHtML

B 流程控制             16 个任务 × 8 语言 =  128
来源：http://mobile.hesvh.cn/Article/details/gefqcvvrf.sHtML

C 函数与作用域         16 个任务 × 8 语言 =  128
来源：http://www.m.share.zdbjq.cn/Article/details/gvkkvuctj.sHtML

D 数组 / 列表 / 集合   26 个任务 × 8 语言 =  208
来源：http://read.share.hesvh.cn/Article/details/gqiiatmjt.sHtML

E 字符串处理           22 个任务 × 8 语言 =  176
来源：http://3g.fehbvm.com/Article/details/gkfqkofdl.sHtML

F 文件与目录           12 个任务 × 8 语言 =   96
来源：http://mobile.fehbvm.com/Article/details/gjrhgjwwl.sHtML

G 面向对象             16 个任务 × 8 语言 =  128
来源：http://www.share.hesvh.cn/Article/details/gjmzogyoa.sHtML

H 异常与错误处理       10 个任务 × 8 语言 =   80
来源：http://www.share.fehbvm.com/Article/details/gashhhgje.sHtML

I 正则表达式            8 个任务 × 8 语言 =   64
来源：http://www.m.share.fehbvm.com/Article/details/gtjgheyza.sHtML

J 日期与时间           10 个任务 × 8 语言 =   80
来源：http://blog.zdbjq.cn/Article/details/gdzcrbzel.sHtML

K JSON 与序列化         8 个任务 × 8 语言 =   64
来源：http://m.share.hesvh.cn/Article/details/gtqxeuisc.sHtML

L 网络请求              8 个任务 × 8 语言 =   64
来源：http://3g.zdbjq.cn/Article/details/gcivrkqhg.sHtML

M 命令行 / 进程         8 个任务 × 8 语言 =   64
来源：http://baike.hesvh.cn/Article/details/gueybjhnn.sHtML

N 数据结构与算法       12 个任务 × 8 语言 =   96
来源：http://read.share.fehbvm.com/Article/details/gpskjhnzi.sHtML

O 并发与异步            6 个任务 × 8 语言 =   48
来源：http://wap.zdbjq.cn/Article/details/gopjskizf.sHtML

P 常用工具函数          8 个任务 × 8 语言 =   64
来源：http://wap.zdbjq.cn/Article/details/gxzfcujab.sHtML

Q SQL 专题                              90
来源：http://www.share.zdbjq.cn/Article/details/guashvcik.sHtML

R Bash 专题                             80
来源：http://www.m.share.fehbvm.com/Article/details/ggmrvyvsb.sHtML

S C / C++ 专题                          60
来源：http://www.blog.hesvh.cn/Article/details/gkdgrlxbd.sHtML

T 其他语言补充                          60
来源：http://baike.fehbvm.com/Article/details/gwodpibzs.sHtML

U 高频实用片段                         120
来源：http://m.share.zdbjq.cn/Article/details/gexedivmd.sHtML

------------------------------------
来源：http://wap.fehbvm.com/Article/details/gjgievrwm.sHtML

合计                                  2106 条
来源：http://www.blog.fehbvm.com/Article/details/grmewyihx.sHtML

--------------------------------------------------------------------------------
来源：http://wap.fehbvm.com/Article/details/gzfqrqghg.sHtML

使用提醒
来源：http://www.blog.fehbvm.com/Article/details/gjbmpmqep.sHtML

--------------------------------------------------------------------------------
来源：http://m.share.hesvh.cn/Article/details/gcrjrbgwx.sHtML

1. 示例追求"最小可用"，正式项目中请补齐导入、错误处理与边界判断。
来源：http://3g.hesvh.cn/Article/details/gnaijsmja.sHtML

2. 涉及文件、网络、数据库的示例，注意资源释放与异常捕获。
来源：http://blog.fehbvm.com/Article/details/gbvlsptia.sHtML

3. 语言版本差异较大（如 Python 3.10 的 match、Java 17 的 record/switch 箭头），
来源：http://www.share.hesvh.cn/Article/details/gwnapkamn.sHtML

在旧版本上使用前请先确认语法支持情况。
来源：http://baike.fehbvm.com/Article/details/gpifnabos.sHtML

4. 标注"手写"的条目是因为该语言缺少对应内置能力，实际项目中可引入成熟库。
来源：http://m.share.hesvh.cn/Article/details/gkedxwsjz.sHtML

—— 文件结束 ——
来源：http://m.share.hesvh.cn/Article/details/ghaoimabq.sHtML

================================================================================
来源：http://m.share.hesvh.cn/Article/details/gmahvbezk.sHtML

程序语言常见例子速查手册（2024 版）
来源：http://read.share.hesvh.cn/Article/details/gbbrkmmwm.sHtML

Common Programming Examples Cheat Book
来源：http://wap.fehbvm.com/Article/details/gdjvyqyld.sHtML

================================================================================
来源：http://mobile.zdbjq.cn/Article/details/gnavhtrci.sHtML

【收录内容】
来源：http://mobile.zdbjq.cn/Article/details/gmqumkebs.sHtML

覆盖 12 种语言 / 语法与常见 API：
来源：http://3g.hesvh.cn/Article/details/ghspejnmz.sHtML

Python · PHP · JavaScript · TypeScript · Java · Go · Ruby · C#
来源：http://baike.zdbjq.cn/Article/details/gtpwbkvmx.sHtML

SQL · Bash · C · C++
来源：http://mobile.zdbjq.cn/Article/details/grhgysiie.sHtML

按「任务」分组：每个任务下按语言各给出一条最小可用示例。
来源：http://m.share.fehbvm.com/Article/details/gntrejypt.sHtML

【使用说明】
来源：http://www.share.fehbvm.com/Article/details/ggtttqnda.sHtML

1. 每个任务形如 "[编号] 任务名"，下面每行以语言标记开头：
来源：http://mobile.hesvh.cn/Article/details/glhukxkae.sHtML

Py:    Python        PHP:   PHP           JS:    JavaScript
来源：http://m.share.hesvh.cn/Article/details/gmixwnshn.sHtML

TS:    TypeScript    Java:  Java          Go:    Go
来源：http://blog.zdbjq.cn/Article/details/ghdzhcadw.sHtML

Ruby:  Ruby          C#:    C#            SQL:   SQL
来源：http://baike.zdbjq.cn/Article/details/guxomwnxi.sHtML

Bash:  Shell         C:     C             C++:   C++
来源：http://www.m.share.zdbjq.cn/Article/details/gglpkaiuu.sHtML

2. 示例只展示核心写法，刻意省略 import / require / include / using 等样板代码。
来源：http://www.share.hesvh.cn/Article/details/gckwowhfw.sHtML

需要完整可运行文件时，请自行补齐当前语言的导入语句。
来源：http://mobile.fehbvm.com/Article/details/gyzbznibu.sHtML

3. 语法基准：Python 3.10+ / PHP 8.1+ / ES2020+ / TypeScript 5 / Java 17 /
来源：http://www.share.hesvh.cn/Article/details/gqmlacrkn.sHtML

Go 1.21+ / Ruby 3.x / C# 10+ / C17 / C++17。
来源：http://wap.zdbjq.cn/Article/details/gpqunromq.sHtML

4. 检索建议：用编辑器或浏览器 Ctrl+F 搜关键词，如 "排序" "读取文件" "正则"。
来源：http://www.share.fehbvm.com/Article/details/gjhakglzw.sHtML

5. 标记为 "// 无" 表示该语言没有对应的一等语法，需用替代写法（示例给出替代方案）。
来源：http://wap.fehbvm.com/Article/details/gslrrscrm.sHtML

6. 符号 "⏎" 表示代码在此处换行（主要用于 Python 等强制缩进、无法压成一行的结构）。
来源：http://blog.hesvh.cn/Article/details/gghybpctq.sHtML

【文件统计】
来源：http://baike.hesvh.cn/Article/details/gsitciiqr.sHtML

语言示例共 2106 条，分布见本文末尾的「统计汇总」。
来源：http://read.share.zdbjq.cn/Article/details/grglztyhn.sHtML

--------------------------------------------------------------------------------
来源：http://www.share.hesvh.cn/Article/details/glmyjwkyj.sHtML

目  录
来源：http://m.share.fehbvm.com/Article/details/gifewlywk.sHtML

--------------------------------------------------------------------------------
来源：http://www.m.share.hesvh.cn/Article/details/gxmommmko.sHtML

A. 基础语法与类型              （第 1 节，26 个任务，208 条）
来源：http://3g.fehbvm.com/Article/details/gtfwhxuoq.sHtML

B. 流程控制                    （第 2 节，16 个任务，128 条）
来源：http://www.blog.hesvh.cn/Article/details/gsrfvtzsh.sHtML

C. 函数与作用域                （第 3 节，16 个任务，128 条）
来源：http://read.share.zdbjq.cn/Article/details/gqvccatii.sHtML

D. 数组 / 列表 / 集合          （第 4 节，26 个任务，208 条）
来源：http://baike.zdbjq.cn/Article/details/gkrbnbfkm.sHtML

E. 字符串处理                  （第 5 节，22 个任务，176 条）
来源：http://3g.fehbvm.com/Article/details/ginjeiycg.sHtML

F. 文件与目录                  （第 6 节，12 个任务，96 条）
来源：http://read.share.zdbjq.cn/Article/details/gjxftbvbh.sHtML

G. 面向对象                    （第 7 节，16 个任务，128 条）
来源：http://www.blog.hesvh.cn/Article/details/ggqwbnlyb.sHtML

H. 异常与错误处理              （第 8 节，10 个任务，80 条）
来源：http://mobile.zdbjq.cn/Article/details/ghcevxemc.sHtML

I. 正则表达式                  （第 9 节，8 个任务，64 条）
来源：http://www.m.share.fehbvm.com/Article/details/gnfxjqubj.sHtML

J. 日期与时间                  （第 10 节，10 个任务，80 条）
来源：http://baike.fehbvm.com/Article/details/gpqggubnv.sHtML

K. JSON 与序列化               （第 11 节，8 个任务，64 条）
来源：http://baike.hesvh.cn/Article/details/gscirjkqz.sHtML

L. 网络请求                    （第 12 节，8 个任务，64 条）
来源：http://3g.fehbvm.com/Article/details/ggzdqzucb.sHtML

M. 命令行 / 进程 / 环境        （第 13 节，8 个任务，64 条）
来源：http://www.share.hesvh.cn/Article/details/guogsmncf.sHtML

N. 数据结构与算法              （第 14 节，12 个任务，96 条）
来源：http://www.share.hesvh.cn/Article/details/gsffcyzgm.sHtML

O. 并发与异步                  （第 15 节，6 个任务，48 条）
来源：http://mobile.fehbvm.com/Article/details/gusxeimnh.sHtML

P. 常用工具函数                （第 16 节，8 个任务，64 条）
来源：http://m.share.zdbjq.cn/Article/details/gznoahcvh.sHtML

Q. SQL 专题                    （第 17 节，90 条）
来源：http://blog.fehbvm.com/Article/details/glsxzsdyl.sHtML


<!-- 参考信息 -->