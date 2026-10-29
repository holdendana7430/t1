代发 wailian999

[U19] Py：正则替换带回调
来源：http://baike.hesvh.cn/Article/details/ghpqejjoy.sHtML

re.sub(r"\d+", lambda m: str(int(m.group()) * 2), s)
来源：http://www.m.share.fehbvm.com/Article/details/guaigynqk.sHtML

[U20] Py：缓存函数结果
来源：http://read.share.fehbvm.com/Article/details/gzrhgksjj.sHtML

@functools.lru_cache(maxsize=None)
来源：http://www.blog.zdbjq.cn/Article/details/gcdsbbrix.sHtML

[U21] Py：自定义上下文管理器
来源：http://3g.zdbjq.cn/Article/details/gjjujwhlm.sHtML

@contextlib.contextmanager
来源：http://read.share.zdbjq.cn/Article/details/guvndadnf.sHtML

[U22] Py：矩阵转置
来源：http://m.share.fehbvm.com/Article/details/gprqxdrcl.sHtML

list(zip(*m))
来源：http://blog.fehbvm.com/Article/details/gpwwihdbo.sHtML

[U23] Py：分块读取大文件
来源：http://3g.fehbvm.com/Article/details/gugakzrse.sHtML

for chunk in iter(lambda: f.read(8192), b""):
来源：http://m.share.fehbvm.com/Article/details/gzutvvyhj.sHtML

[U24] Py：路径操作
来源：http://www.share.hesvh.cn/Article/details/gemwknlxo.sHtML

Path("a/b.txt").parent.mkdir(parents=True, exist_ok=True)
来源：http://wap.hesvh.cn/Article/details/gxwaxuzzn.sHtML

[U25] Py：CSV 按字典读
来源：http://www.blog.hesvh.cn/Article/details/ghvwcdvdq.sHtML

csv.DictReader(f)
来源：http://blog.fehbvm.com/Article/details/glwwzvgiq.sHtML

[U26] Py：并发下载
来源：http://3g.fehbvm.com/Article/details/ghtdtrsvh.sHtML

ThreadPoolExecutor(max_workers=8).map(fetch, urls)
来源：http://baike.fehbvm.com/Article/details/gtgygpbql.sHtML

[U27] Py：异步 HTTP
来源：http://www.blog.fehbvm.com/Article/details/geihlswsn.sHtML

aiohttp.ClientSession() 配合 async with
来源：http://www.m.share.hesvh.cn/Article/details/gzbxipbae.sHtML

[U28] Py：类型别名
来源：http://www.blog.hesvh.cn/Article/details/ggfkrazja.sHtML

UserId = int
来源：http://www.share.hesvh.cn/Article/details/gdkabwpyc.sHtML

[U29] Py：属性校验
来源：http://3g.hesvh.cn/Article/details/ghizjgglx.sHtML

@property 与 @x.setter 配合
来源：http://baike.hesvh.cn/Article/details/gzcugooqg.sHtML

[U30] Py：数据类
来源：http://www.blog.hesvh.cn/Article/details/gtqeboyti.sHtML

@dataclass(slots=True)
来源：http://www.m.share.hesvh.cn/Article/details/gibkqtyza.sHtML

[U31] Py：单测
来源：http://www.blog.zdbjq.cn/Article/details/gjeylcoll.sHtML

python -m pytest -q
来源：http://read.share.fehbvm.com/Article/details/gkjtuxeyv.sHtML

[U32] Py：代码格式化
来源：http://www.m.share.zdbjq.cn/Article/details/gcazzwqvv.sHtML

ruff format . && ruff check --fix .
来源：http://mobile.fehbvm.com/Article/details/granxbueu.sHtML

[U33] Py：打包发布
来源：http://blog.hesvh.cn/Article/details/gqfrnehvg.sHtML

python -m build  （依赖 pyproject.toml）
来源：http://blog.zdbjq.cn/Article/details/gyzwccycm.sHtML

[U34] Py：判断编码
来源：http://blog.fehbvm.com/Article/details/gscguhbtg.sHtML

chardet.detect(raw)
来源：http://wap.hesvh.cn/Article/details/gtyvedrdd.sHtML

[U35] Py：发送邮件
来源：http://read.share.hesvh.cn/Article/details/grabuoveh.sHtML

smtplib.SMTP_SSL(...).send_message(msg)
来源：http://blog.hesvh.cn/Article/details/gwrvgfxtx.sHtML

[U36] Py：定时任务
来源：http://3g.hesvh.cn/Article/details/gbqcpfbth.sHtML

schedule.every(10).minutes.do(job)
来源：http://blog.zdbjq.cn/Article/details/gytkidvdv.sHtML

[U37] Py：读写 Excel
来源：http://read.share.fehbvm.com/Article/details/gcfubqutz.sHtML

pandas.read_excel / DataFrame.to_excel
来源：http://read.share.hesvh.cn/Article/details/gtlmvjzhn.sHtML

[U38] Py：获取脚本所在目录
来源：http://www.blog.zdbjq.cn/Article/details/ghfbmcglt.sHtML

Path(__file__).resolve().parent
来源：http://www.m.share.hesvh.cn/Article/details/gusetxxbf.sHtML

[U39] Py：判断是否在交互环境
来源：http://3g.fehbvm.com/Article/details/ghhipjojq.sHtML

sys.stdout.isatty()
来源：http://mobile.hesvh.cn/Article/details/gdvbbttwq.sHtML

[U40] Py：打印到标准错误
来源：http://m.share.fehbvm.com/Article/details/gkrooxdrr.sHtML

print("err", file=sys.stderr)
来源：http://3g.zdbjq.cn/Article/details/gyhktuspq.sHtML

[U41] PHP：初始化 Composer 项目
来源：http://read.share.hesvh.cn/Article/details/gikqbseju.sHtML

composer init;  composer require guzzlehttp/guzzle
来源：http://www.blog.fehbvm.com/Article/details/guaflrwsg.sHtML

[U42] PHP：PSR-4 自动加载
来源：http://read.share.fehbvm.com/Article/details/ghigywuxu.sHtML

"autoload": { "psr-4": { "App\\": "src/" } }
来源：http://wap.fehbvm.com/Article/details/gixtusefv.sHtML

[U43] PHP：声明命名空间
来源：http://www.m.share.zdbjq.cn/Article/details/gvrwrnchv.sHtML

namespace App\Http;
来源：http://m.share.fehbvm.com/Article/details/gwjftspid.sHtML

[U44] PHP：开启严格类型
来源：http://www.m.share.fehbvm.com/Article/details/getzyxgjp.sHtML

declare(strict_types=1);
来源：http://www.m.share.hesvh.cn/Article/details/gtkwikcpu.sHtML

[U45] PHP：类型声明与返回类型
来源：http://mobile.fehbvm.com/Article/details/gfrlbhoaa.sHtML

function add(int $a, int $b): int { return $a + $b; }
来源：http://mobile.hesvh.cn/Article/details/ghjkesaaf.sHtML

[U46] PHP：可空类型
来源：http://wap.zdbjq.cn/Article/details/gmnbhpshy.sHtML

?string $name = null
来源：http://www.m.share.hesvh.cn/Article/details/gxsapzmdw.sHtML

[U47] PHP：联合类型
来源：http://baike.zdbjq.cn/Article/details/gaggefcmb.sHtML

int|string $id
来源：http://www.share.hesvh.cn/Article/details/gjpvtwwza.sHtML

[U48] PHP：纯枚举
来源：http://wap.hesvh.cn/Article/details/glztmqout.sHtML

enum Status: string { case Active = "active"; case Off = "off"; }
来源：http://3g.hesvh.cn/Article/details/gdwaukqiu.sHtML

[U49] PHP：只读属性
来源：http://3g.zdbjq.cn/Article/details/gpzfpahtj.sHtML

public readonly string $name
来源：http://www.share.zdbjq.cn/Article/details/gxgpkutqy.sHtML

[U50] PHP：构造器属性提升
来源：http://blog.hesvh.cn/Article/details/gmucrszgl.sHtML

public function __construct(private int $id) {}
来源：http://www.blog.fehbvm.com/Article/details/ghxtcvqdz.sHtML

[U51] PHP：数组解构
来源：http://wap.zdbjq.cn/Article/details/gjfludjuw.sHtML

[$a, $b] = $arr;
来源：http://3g.zdbjq.cn/Article/details/gghjxmukg.sHtML

[U52] PHP：箭头函数
来源：http://mobile.zdbjq.cn/Article/details/gqwzddmsh.sHtML

$double = fn($x) => $x * 2;
来源：http://www.m.share.fehbvm.com/Article/details/gbxztsbfl.sHtML

[U53] PHP：空合并运算符
来源：http://baike.hesvh.cn/Article/details/gylkmwixp.sHtML

$v = $a ?? $b ?? "default";
来源：http://blog.hesvh.cn/Article/details/gdgrlehxm.sHtML

[U54] PHP：空安全调用
来源：http://wap.fehbvm.com/Article/details/gylfjshfd.sHtML

$obj?->method()
来源：http://mobile.hesvh.cn/Article/details/gpefatjii.sHtML

[U55] PHP：match 表达式
来源：http://www.blog.zdbjq.cn/Article/details/gziutqbny.sHtML

$s = match($x) { 1 => "一", default => "其他" };
来源：http://www.m.share.zdbjq.cn/Article/details/gqxsuicxm.sHtML

[U56] PHP：命名参数
来源：http://mobile.hesvh.cn/Article/details/gdkxajatd.sHtML

f(a: 1, b: 2)
来源：http://mobile.fehbvm.com/Article/details/gnqzrasgn.sHtML

[U57] PHP：字符串插值
来源：http://m.share.fehbvm.com/Article/details/gbkjpssdz.sHtML

"值: {$a}"
来源：http://m.share.fehbvm.com/Article/details/gexecygar.sHtML

[U58] PHP：数组三件套
来源：http://wap.zdbjq.cn/Article/details/gyhxuwhfd.sHtML

array_map($f, $a);  array_filter($a, $f);  array_reduce($a, $f, 0);
来源：http://www.blog.zdbjq.cn/Article/details/gamlycszp.sHtML

[U59] PHP：自定义排序
来源：http://www.share.hesvh.cn/Article/details/gargdzwdf.sHtML

usort($arr, fn($a, $b) => $a["age"] <=> $b["age"]);
来源：http://wap.fehbvm.com/Article/details/gtpcfsuss.sHtML

[U60] PHP：JSON 编解码
来源：http://www.m.share.fehbvm.com/Article/details/ggilreeul.sHtML

json_encode($d, JSON_UNESCAPED_UNICODE);  json_decode($s, true);
来源：http://blog.fehbvm.com/Article/details/gywuibcrw.sHtML

[U61] PHP：正则
来源：http://m.share.fehbvm.com/Article/details/gajkbnanl.sHtML

preg_match('/(\d+)/', $s, $m);  preg_replace('/\d+/', '#', $s);
来源：http://mobile.zdbjq.cn/Article/details/gonukpvig.sHtML

[U62] PHP：日期对象
来源：http://blog.zdbjq.cn/Article/details/gufnradfz.sHtML

(new DateTimeImmutable())->format("Y-m-d");
来源：http://baike.hesvh.cn/Article/details/gcpbydtwl.sHtML

[U63] PHP：文件读写
来源：http://3g.fehbvm.com/Article/details/gzyhytnrf.sHtML

file_get_contents($f);  file_put_contents($f, $data);
来源：http://3g.hesvh.cn/Article/details/guwokofoz.sHtML

[U64] PHP：目录遍历
来源：http://www.share.hesvh.cn/Article/details/gbqijnppd.sHtML

glob("dir/*.php");  scandir("dir");
来源：http://baike.zdbjq.cn/Article/details/gmljqtxvz.sHtML

[U65] PHP：会话
来源：http://blog.fehbvm.com/Article/details/gtxmqship.sHtML

session_start();  $_SESSION["uid"] = 1;
来源：http://read.share.hesvh.cn/Article/details/gstxhzsik.sHtML

[U66] PHP：设置 Cookie
来源：http://www.share.fehbvm.com/Article/details/gfhipzkfs.sHtML

setcookie("token", $v, ["httponly" => true, "samesite" => "Lax"]);
来源：http://blog.fehbvm.com/Article/details/goygqhhwc.sHtML

[U67] PHP：处理文件上传
来源：http://baike.hesvh.cn/Article/details/gyxvkaaeb.sHtML

$_FILES["file"]["tmp_name"] 与 move_uploaded_file()
来源：http://read.share.zdbjq.cn/Article/details/ghyhouuxc.sHtML

[U68] PHP：PDO 连接
来源：http://baike.hesvh.cn/Article/details/gypmsskqc.sHtML

$pdo = new PDO("mysql:host=localhost;dbname=app", "root", "");
来源：http://baike.fehbvm.com/Article/details/gcmijmkgv.sHtML

[U69] PHP：PDO 预处理
来源：http://www.m.share.fehbvm.com/Article/details/gdppmgvkb.sHtML

$stmt = $pdo->prepare("SELECT * FROM users WHERE id = ?");  $stmt->execute([$id]);
来源：http://m.share.zdbjq.cn/Article/details/gockhvzuv.sHtML

[U70] PHP：PDO 事务
来源：http://mobile.fehbvm.com/Article/details/gzqqfxryx.sHtML

$pdo->beginTransaction();  $pdo->commit();  $pdo->rollBack();
来源：http://3g.fehbvm.com/Article/details/gpcdtbspg.sHtML

[U71] PHP：抛出异常
来源：http://baike.hesvh.cn/Article/details/gchxkramz.sHtML

throw new RuntimeException("失败", 500);
来源：http://wap.hesvh.cn/Article/details/gsbtlkmzm.sHtML

[U72] PHP：写错误日志
来源：http://baike.hesvh.cn/Article/details/gewyzmolm.sHtML

error_log("失败: " . $e->getMessage());
来源：http://m.share.zdbjq.cn/Article/details/gvaoxxswr.sHtML

[U73] PHP：读取 ini 配置
来源：http://3g.zdbjq.cn/Article/details/gmzpaaypp.sHtML

parse_ini_file("config.ini", true)
来源：http://read.share.fehbvm.com/Article/details/gzbbmnxgn.sHtML

[U74] PHP：读取环境变量
来源：http://mobile.hesvh.cn/Article/details/gamsczifp.sHtML

getenv("APP_ENV") ?: "production"
来源：http://3g.hesvh.cn/Article/details/gzgtrzrdx.sHtML

[U75] PHP：依赖注入
来源：http://baike.zdbjq.cn/Article/details/gqmmemtpd.sHtML

composer require psr/container
来源：http://blog.zdbjq.cn/Article/details/gpbgckxki.sHtML

[U76] PHP：简单路由
来源：http://read.share.hesvh.cn/Article/details/ghtilyzmg.sHtML

$path = parse_url($_SERVER["REQUEST_URI"], PHP_URL_PATH);
来源：http://3g.zdbjq.cn/Article/details/gjedvfwxp.sHtML

[U77] PHP：模板渲染
来源：http://m.share.hesvh.cn/Article/details/gcmkjoara.sHtML

composer require twig/twig
来源：http://wap.hesvh.cn/Article/details/gcuiqpowg.sHtML

[U78] PHP：单元测试
来源：http://blog.hesvh.cn/Article/details/gtjcsbthz.sHtML

composer require --dev phpunit/phpunit
来源：http://www.m.share.hesvh.cn/Article/details/gmpgrofbi.sHtML

[U79] PHP：静态分析
来源：http://www.m.share.zdbjq.cn/Article/details/gezbxzbrf.sHtML

composer require --dev phpstan/phpstan
来源：http://3g.zdbjq.cn/Article/details/gcrvzmlcw.sHtML

[U80] PHP：代码规范修复
来源：http://mobile.zdbjq.cn/Article/details/gvfprtihz.sHtML

composer require --dev friendsofphp/php-cs-fixer
来源：http://www.share.fehbvm.com/Article/details/gzrkfiadm.sHtML

[U81] JS：初始化项目
来源：http://3g.hesvh.cn/Article/details/gbegnrwek.sHtML

npm init -y;  npm i express
来源：http://blog.zdbjq.cn/Article/details/gxorpyoqn.sHtML

[U82] JS：package.json 脚本
来源：http://m.share.zdbjq.cn/Article/details/gwzqevlgi.sHtML

"scripts": { "dev": "vite", "build": "vite build" }
来源：http://blog.zdbjq.cn/Article/details/gpbteimsm.sHtML

[U83] JS：ES Module 导入导出
来源：http://wap.zdbjq.cn/Article/details/gxovfegll.sHtML

export const a = 1;  import { a } from "./m.js";
来源：http://m.share.hesvh.cn/Article/details/gwmffpcep.sHtML

[U84] JS：CommonJS 写法
来源：http://read.share.hesvh.cn/Article/details/gnatujgjk.sHtML

module.exports = { a };  const { a } = require("./m");
来源：http://wap.fehbvm.com/Article/details/gclmzactk.sHtML

[U85] JS：可选链
来源：http://www.m.share.fehbvm.com/Article/details/gcqcgwhbp.sHtML

a?.b?.c
来源：http://www.blog.zdbjq.cn/Article/details/gofjcznle.sHtML

[U86] JS：空值合并
来源：http://www.blog.zdbjq.cn/Article/details/gusughvre.sHtML

a ?? b
来源：http://m.share.zdbjq.cn/Article/details/grmmawjpn.sHtML

[U87] JS：解构默认值
来源：http://blog.fehbvm.com/Article/details/ggelibsko.sHtML

const { a = 1, b = 2 } = obj;
来源：http://wap.zdbjq.cn/Article/details/gxvqdhuhv.sHtML

[U88] JS：对象展开合并
来源：http://blog.zdbjq.cn/Article/details/gffbfbuxl.sHtML

{ ...a, ...b }
来源：http://baike.zdbjq.cn/Article/details/gzlmnsbgk.sHtML

[U89] JS：数组去重
来源：http://wap.fehbvm.com/Article/details/goczcxnym.sHtML

[...new Set(arr)]
来源：http://read.share.zdbjq.cn/Article/details/gobfbykaf.sHtML

[U90] JS：数字数组排序
来源：http://www.m.share.fehbvm.com/Article/details/gdxwmiude.sHtML

[...arr].sort((a, b) => a - b)
来源：http://wap.zdbjq.cn/Article/details/gmiommcgx.sHtML

[U91] JS：对象键值遍历
来源：http://wap.zdbjq.cn/Article/details/gnbrgjuti.sHtML

Object.entries(obj).forEach(([k, v]) => {});
来源：http://www.m.share.zdbjq.cn/Article/details/gfhxftdtt.sHtML

[U92] JS：深拷贝
来源：http://www.m.share.zdbjq.cn/Article/details/gepfexmmy.sHtML

structuredClone(obj)
来源：http://3g.hesvh.cn/Article/details/gfusnwumy.sHtML

[U93] JS：模板字符串
来源：http://baike.zdbjq.cn/Article/details/gftdsdujq.sHtML

`共 ${n} 条`
来源：http://mobile.fehbvm.com/Article/details/gulljyrwe.sHtML

[U94] JS：箭头函数
来源：http://m.share.zdbjq.cn/Article/details/glgfvvdek.sHtML

const double = x => x * 2;
来源：http://read.share.fehbvm.com/Article/details/gxxbqtqow.sHtML

[U95] JS：Promise 包装
来源：http://www.blog.fehbvm.com/Article/details/gvydffvkr.sHtML

new Promise((resolve, reject) => {})
来源：http://3g.zdbjq.cn/Article/details/gqsppfrfk.sHtML

[U96] JS：async/await 与异常
来源：http://baike.fehbvm.com/Article/details/goukbbezu.sHtML

try { const d = await f(); } catch (e) { console.error(e); }
来源：http://read.share.hesvh.cn/Article/details/ghzpmxqko.sHtML

[U97] JS：并发请求
来源：http://m.share.zdbjq.cn/Article/details/gpoitboke.sHtML

await Promise.all(urls.map(u => fetch(u)))
来源：http://m.share.fehbvm.com/Article/details/gbbaqnumm.sHtML

[U98] JS：fetch 带 JSON
来源：http://mobile.hesvh.cn/Article/details/glkvrxmfl.sHtML

await fetch(url, { method: "POST", headers: { "Content-Type": "application/json" }, body: JSON.stringify(d) })
来源：http://wap.fehbvm.com/Article/details/gguvobnxr.sHtML

[U99] JS：事件监听
来源：http://www.m.share.zdbjq.cn/Article/details/gjhohgswr.sHtML

el.addEventListener("click", e => {})
来源：http://wap.fehbvm.com/Article/details/gosmeiitt.sHtML

[U100] JS：DOM 查询
来源：http://blog.zdbjq.cn/Article/details/gwmdupxqj.sHtML

document.querySelector(".item")
来源：http://blog.hesvh.cn/Article/details/gfmwjnqom.sHtML

[U101] JS：classList 操作
来源：http://m.share.fehbvm.com/Article/details/gggzoowwc.sHtML

el.classList.toggle("active")
来源：http://read.share.zdbjq.cn/Article/details/gipbxvzdi.sHtML

[U102] JS：本地存储
来源：http://baike.zdbjq.cn/Article/details/gioxcubxw.sHtML

localStorage.setItem("k", JSON.stringify(v))
来源：http://3g.hesvh.cn/Article/details/gqcyyecga.sHtML

[U103] JS：定时器
来源：http://baike.zdbjq.cn/Article/details/gzoedomma.sHtML

setTimeout(fn, 1000);  setInterval(fn, 1000);
来源：http://www.blog.fehbvm.com/Article/details/gaijsfwnz.sHtML

[U104] JS：防抖
来源：http://www.m.share.fehbvm.com/Article/details/gimxzbsaa.sHtML

const debounce = (fn, ms) => { let t; return (...a) => { clearTimeout(t); t = setTimeout(() => fn(...a), ms); }; };
来源：http://m.share.fehbvm.com/Article/details/gsbmdotfy.sHtML

[U105] JS：节流
来源：http://m.share.hesvh.cn/Article/details/gwjkyqcej.sHtML

const throttle = (fn, ms) => { let last = 0; return (...a) => { const n = Date.now(); if (n - last >= ms) { last = n; fn(...a); } }; };
来源：http://baike.fehbvm.com/Article/details/ghyulnywv.sHtML

[U106] JS：日期格式化
来源：http://baike.hesvh.cn/Article/details/gqakyssga.sHtML

new Intl.DateTimeFormat("zh-CN", { dateStyle: "medium" }).format(new Date())
来源：http://mobile.hesvh.cn/Article/details/gnxuwmbyw.sHtML

[U107] JS：数字千分位
来源：http://baike.fehbvm.com/Article/details/gnzlqqzes.sHtML

new Intl.NumberFormat("en-US").format(1234567)
来源：http://mobile.fehbvm.com/Article/details/gwaymbdgv.sHtML

[U108] JS：随机整数
来源：http://m.share.fehbvm.com/Article/details/gfaxjnkwk.sHtML

Math.floor(Math.random() * (max - min + 1)) + min
来源：http://3g.hesvh.cn/Article/details/gshnocksv.sHtML

[U109] JS：数组分组
来源：http://wap.hesvh.cn/Article/details/gwrqkoggq.sHtML

Object.groupBy(arr, x => x.type)
来源：http://read.share.zdbjq.cn/Article/details/gvdecgsmh.sHtML

[U110] JS：数组分块
来源：http://www.m.share.fehbvm.com/Article/details/gnbuvxpjx.sHtML

arr.reduce((acc, x, i) => (i % size ? acc : [...acc, arr.slice(i, i + size)]), [])
来源：http://www.blog.fehbvm.com/Article/details/gizchnslv.sHtML

[U111] JS：对象转 Map
来源：http://blog.fehbvm.com/Article/details/guxwllths.sHtML

new Map(Object.entries(obj))
来源：http://baike.zdbjq.cn/Article/details/ggeewaeft.sHtML

[U112] JS：字符串补位
来源：http://wap.hesvh.cn/Article/details/gjklmddzo.sHtML

"7".padStart(3, "0")
来源：http://www.m.share.zdbjq.cn/Article/details/goghmzwan.sHtML

[U113] JS：正则替换全部
来源：http://www.m.share.hesvh.cn/Article/details/gmgmolfxf.sHtML

s.replaceAll("a", "b")
来源：http://www.blog.hesvh.cn/Article/details/gtyfurmpj.sHtML

[U114] JS：JSON 深比较
来源：http://m.share.zdbjq.cn/Article/details/gzxuxjtzc.sHtML

JSON.stringify(a) === JSON.stringify(b)
来源：http://baike.zdbjq.cn/Article/details/gkhwalqqa.sHtML

[U115] JS：生成 UUID
来源：http://blog.zdbjq.cn/Article/details/gozonqtya.sHtML

crypto.randomUUID()
来源：http://baike.fehbvm.com/Article/details/geaevsbiu.sHtML

[U116] JS：类型检查（JSDoc）
来源：http://baike.fehbvm.com/Article/details/gecjmrzhy.sHtML

/** @param {string} name */ function f(name) {}
来源：http://www.share.zdbjq.cn/Article/details/gfvzixtnd.sHtML

[U117] JS：单元测试
来源：http://read.share.zdbjq.cn/Article/details/gokfydtfd.sHtML

npm i -D vitest;  npx vitest
来源：http://wap.zdbjq.cn/Article/details/genreyqts.sHtML

[U118] JS：开发服务器
来源：http://mobile.hesvh.cn/Article/details/gnunfrfwv.sHtML

npm i -D vite;  npx vite
来源：http://wap.zdbjq.cn/Article/details/gijqvkbps.sHtML

[U119] JS：生产构建
来源：http://www.m.share.hesvh.cn/Article/details/gazbpiblb.sHtML

npx vite build
来源：http://read.share.hesvh.cn/Article/details/gpxdxodob.sHtML

[U120] JS：读取环境变量（Vite）
来源：http://www.blog.hesvh.cn/Article/details/ggsubiklq.sHtML

import.meta.env.VITE_API_URL
来源：http://blog.hesvh.cn/Article/details/gdxexvewt.sHtML

================================================================================
来源：http://blog.fehbvm.com/Article/details/gygkfmrda.sHtML

统计汇总
来源：http://baike.zdbjq.cn/Article/details/gygagpwwx.sHtML

================================================================================
来源：http://wap.hesvh.cn/Article/details/gncjafssu.sHtML

按语言统计（条）：
来源：http://m.share.hesvh.cn/Article/details/gkggmedbl.sHtML

Python ......... 252
来源：http://3g.fehbvm.com/Article/details/gaecfpoet.sHtML

PHP ............ 252
来源：http://www.m.share.fehbvm.com/Article/details/gyarlurob.sHtML

JavaScript ..... 252
来源：http://baike.zdbjq.cn/Article/details/gckltnbry.sHtML

TypeScript ..... 212
来源：http://m.share.zdbjq.cn/Article/details/gtvqncpid.sHtML

Java ........... 212
来源：http://read.share.zdbjq.cn/Article/details/gclmdetqv.sHtML

Go ............. 212
来源：http://mobile.fehbvm.com/Article/details/glwfcnxaq.sHtML

Ruby ........... 212
来源：http://read.share.fehbvm.com/Article/details/gioartrbq.sHtML

C# ............. 212
来源：http://mobile.fehbvm.com/Article/details/godgebtrk.sHtML

C .............. 30
来源：http://mobile.zdbjq.cn/Article/details/gyhzqvclf.sHtML

C++ ............ 30
来源：http://read.share.zdbjq.cn/Article/details/gmzuwehwg.sHtML

SQL ............ 90
来源：http://read.share.zdbjq.cn/Article/details/gfvgavjkn.sHtML

Bash ........... 80
来源：http://www.blog.hesvh.cn/Article/details/gwbmqvzhj.sHtML

Kotlin ......... 15
来源：http://blog.zdbjq.cn/Article/details/gomqvqaet.sHtML

Swift .......... 15
来源：http://mobile.hesvh.cn/Article/details/grvyzqbna.sHtML

Lua ............ 10
来源：http://www.m.share.hesvh.cn/Article/details/giifgvpyp.sHtML

Perl ........... 10
来源：http://www.m.share.fehbvm.com/Article/details/gpfawuzqy.sHtML

Scala .......... 10
来源：http://www.share.fehbvm.com/Article/details/gpibpczpj.sHtML

------------------------------------
来源：http://www.blog.hesvh.cn/Article/details/gygkbzkqt.sHtML

合计 ........... 2106 条
来源：http://blog.hesvh.cn/Article/details/gbsplphsv.sHtML

按章节统计：
来源：http://www.share.zdbjq.cn/Article/details/gwtdrgcji.sHtML

A 基础语法与类型       26 个任务 × 8 语言 =  208
来源：http://www.blog.hesvh.cn/Article/details/gptblovva.sHtML

B 流程控制             16 个任务 × 8 语言 =  128
来源：http://mobile.fehbvm.com/Article/details/gtrqeqxfn.sHtML

C 函数与作用域         16 个任务 × 8 语言 =  128
来源：http://www.m.share.hesvh.cn/Article/details/gerrfmkmf.sHtML

D 数组 / 列表 / 集合   26 个任务 × 8 语言 =  208
来源：http://wap.fehbvm.com/Article/details/gbfnxgczh.sHtML

E 字符串处理           22 个任务 × 8 语言 =  176
来源：http://read.share.hesvh.cn/Article/details/gpwgrckit.sHtML

F 文件与目录           12 个任务 × 8 语言 =   96
来源：http://wap.fehbvm.com/Article/details/gtklplfbw.sHtML

G 面向对象             16 个任务 × 8 语言 =  128
来源：http://blog.zdbjq.cn/Article/details/gehtjgxuk.sHtML

H 异常与错误处理       10 个任务 × 8 语言 =   80
来源：http://www.share.fehbvm.com/Article/details/gegfxnhgy.sHtML

I 正则表达式            8 个任务 × 8 语言 =   64
来源：http://m.share.hesvh.cn/Article/details/glpjmyfqq.sHtML

J 日期与时间           10 个任务 × 8 语言 =   80
来源：http://www.m.share.zdbjq.cn/Article/details/glxgjmpdc.sHtML

K JSON 与序列化         8 个任务 × 8 语言 =   64
来源：http://read.share.fehbvm.com/Article/details/gtmxmpivo.sHtML

L 网络请求              8 个任务 × 8 语言 =   64
来源：http://3g.zdbjq.cn/Article/details/gblzmssdm.sHtML

M 命令行 / 进程         8 个任务 × 8 语言 =   64
来源：http://www.m.share.fehbvm.com/Article/details/gbymnazkn.sHtML

N 数据结构与算法       12 个任务 × 8 语言 =   96
来源：http://blog.fehbvm.com/Article/details/gdvulczdz.sHtML

O 并发与异步            6 个任务 × 8 语言 =   48
来源：http://wap.zdbjq.cn/Article/details/gkongzdga.sHtML

P 常用工具函数          8 个任务 × 8 语言 =   64
来源：http://baike.zdbjq.cn/Article/details/gsgpzqawz.sHtML

Q SQL 专题                              90
来源：http://3g.zdbjq.cn/Article/details/gzgzjtnec.sHtML

R Bash 专题                             80
来源：http://www.m.share.fehbvm.com/Article/details/gufzzicsz.sHtML

S C / C++ 专题                          60
来源：http://baike.fehbvm.com/Article/details/guuuskyjw.sHtML

T 其他语言补充                          60
来源：http://mobile.hesvh.cn/Article/details/gkxulukui.sHtML

U 高频实用片段                         120
来源：http://www.blog.hesvh.cn/Article/details/ggymhyfiy.sHtML

------------------------------------
来源：http://www.share.fehbvm.com/Article/details/gaykowsnj.sHtML

合计                                  2106 条
来源：http://blog.fehbvm.com/Article/details/gfalcmrhq.sHtML

--------------------------------------------------------------------------------
来源：http://mobile.fehbvm.com/Article/details/gdznwqesy.sHtML

使用提醒
来源：http://mobile.fehbvm.com/Article/details/girsrgzeu.sHtML

--------------------------------------------------------------------------------
来源：http://read.share.hesvh.cn/Article/details/gnxttqdls.sHtML

1. 示例追求"最小可用"，正式项目中请补齐导入、错误处理与边界判断。
来源：http://baike.fehbvm.com/Article/details/govlkoltj.sHtML

2. 涉及文件、网络、数据库的示例，注意资源释放与异常捕获。
来源：http://wap.fehbvm.com/Article/details/gcyzbvfdg.sHtML

3. 语言版本差异较大（如 Python 3.10 的 match、Java 17 的 record/switch 箭头），
来源：http://wap.fehbvm.com/Article/details/gamnsquzs.sHtML

在旧版本上使用前请先确认语法支持情况。
来源：http://read.share.fehbvm.com/Article/details/gedmowvmg.sHtML

4. 标注"手写"的条目是因为该语言缺少对应内置能力，实际项目中可引入成熟库。
来源：http://www.blog.zdbjq.cn/Article/details/glrdpcomf.sHtML

—— 文件结束 ——
来源：http://www.share.fehbvm.com/Article/details/glokkfmpu.sHtML

================================================================================
来源：http://www.share.hesvh.cn/Article/details/goovajcmd.sHtML

程序语言常见例子速查手册（2024 版）
来源：http://wap.fehbvm.com/Article/details/gshihifsy.sHtML

Common Programming Examples Cheat Book
来源：http://www.share.zdbjq.cn/Article/details/grughuqrt.sHtML

================================================================================
来源：http://wap.hesvh.cn/Article/details/gxiptveyl.sHtML

【收录内容】
来源：http://blog.fehbvm.com/Article/details/gnikmubsm.sHtML

覆盖 12 种语言 / 语法与常见 API：
来源：http://blog.fehbvm.com/Article/details/gufmyydwz.sHtML

Python · PHP · JavaScript · TypeScript · Java · Go · Ruby · C#
来源：http://read.share.fehbvm.com/Article/details/grumzsrru.sHtML

SQL · Bash · C · C++
来源：http://baike.hesvh.cn/Article/details/gegvlpplb.sHtML

按「任务」分组：每个任务下按语言各给出一条最小可用示例。
来源：http://baike.zdbjq.cn/Article/details/gfolporle.sHtML

【使用说明】
来源：http://baike.hesvh.cn/Article/details/gustcptqc.sHtML

1. 每个任务形如 "[编号] 任务名"，下面每行以语言标记开头：
来源：http://read.share.zdbjq.cn/Article/details/gzcttprry.sHtML

Py:    Python        PHP:   PHP           JS:    JavaScript
来源：http://www.blog.hesvh.cn/Article/details/gepfwmpmw.sHtML

TS:    TypeScript    Java:  Java          Go:    Go
来源：http://read.share.fehbvm.com/Article/details/gvbpbpuxv.sHtML

Ruby:  Ruby          C#:    C#            SQL:   SQL
来源：http://read.share.hesvh.cn/Article/details/gmvyackwr.sHtML

Bash:  Shell         C:     C             C++:   C++
来源：http://www.blog.fehbvm.com/Article/details/gdufzkgpk.sHtML

2. 示例只展示核心写法，刻意省略 import / require / include / using 等样板代码。
来源：http://m.share.fehbvm.com/Article/details/gxbuejpzr.sHtML

需要完整可运行文件时，请自行补齐当前语言的导入语句。
来源：http://3g.hesvh.cn/Article/details/gaeaoztvs.sHtML

3. 语法基准：Python 3.10+ / PHP 8.1+ / ES2020+ / TypeScript 5 / Java 17 /
来源：http://m.share.hesvh.cn/Article/details/gkhwhkprp.sHtML

Go 1.21+ / Ruby 3.x / C# 10+ / C17 / C++17。
来源：http://read.share.zdbjq.cn/Article/details/gvpyrelcg.sHtML

4. 检索建议：用编辑器或浏览器 Ctrl+F 搜关键词，如 "排序" "读取文件" "正则"。
来源：http://baike.zdbjq.cn/Article/details/gzvhpkhps.sHtML

5. 标记为 "// 无" 表示该语言没有对应的一等语法，需用替代写法（示例给出替代方案）。
来源：http://read.share.fehbvm.com/Article/details/gzfpssklm.sHtML

6. 符号 "⏎" 表示代码在此处换行（主要用于 Python 等强制缩进、无法压成一行的结构）。
来源：http://blog.hesvh.cn/Article/details/gauopddvd.sHtML

【文件统计】
来源：http://www.blog.zdbjq.cn/Article/details/gyxycbguu.sHtML

语言示例共 2106 条，分布见本文末尾的「统计汇总」。
来源：http://blog.hesvh.cn/Article/details/gmwsjfobh.sHtML

--------------------------------------------------------------------------------
来源：http://www.share.fehbvm.com/Article/details/guxqlnowt.sHtML

目  录
来源：http://baike.fehbvm.com/Article/details/guchgqkxz.sHtML

--------------------------------------------------------------------------------
来源：http://www.share.fehbvm.com/Article/details/gsmwjdwjb.sHtML

A. 基础语法与类型              （第 1 节，26 个任务，208 条）
来源：http://www.blog.zdbjq.cn/Article/details/gnnrmkinz.sHtML

B. 流程控制                    （第 2 节，16 个任务，128 条）
来源：http://www.m.share.hesvh.cn/Article/details/ggoekonbk.sHtML

C. 函数与作用域                （第 3 节，16 个任务，128 条）
来源：http://baike.fehbvm.com/Article/details/gxgkjxjrc.sHtML

D. 数组 / 列表 / 集合          （第 4 节，26 个任务，208 条）
来源：http://mobile.fehbvm.com/Article/details/gwgnxfcqo.sHtML

E. 字符串处理                  （第 5 节，22 个任务，176 条）
来源：http://m.share.hesvh.cn/Article/details/gqvraqoqo.sHtML

F. 文件与目录                  （第 6 节，12 个任务，96 条）
来源：http://3g.hesvh.cn/Article/details/gtgyucnsn.sHtML

G. 面向对象                    （第 7 节，16 个任务，128 条）
来源：http://www.m.share.fehbvm.com/Article/details/ghfbkrzgq.sHtML

H. 异常与错误处理              （第 8 节，10 个任务，80 条）
来源：http://www.m.share.zdbjq.cn/Article/details/gzaroxuge.sHtML

I. 正则表达式                  （第 9 节，8 个任务，64 条）
来源：http://blog.hesvh.cn/Article/details/gfrnxtqju.sHtML

J. 日期与时间                  （第 10 节，10 个任务，80 条）
来源：http://3g.zdbjq.cn/Article/details/gjgomfqzk.sHtML

K. JSON 与序列化               （第 11 节，8 个任务，64 条）
来源：http://www.share.hesvh.cn/Article/details/gmboawmrw.sHtML

L. 网络请求                    （第 12 节，8 个任务，64 条）
来源：http://www.share.hesvh.cn/Article/details/gvmjqrqyz.sHtML

M. 命令行 / 进程 / 环境        （第 13 节，8 个任务，64 条）
来源：http://m.share.fehbvm.com/Article/details/ghhkxbdmo.sHtML


<!-- 参考信息 -->