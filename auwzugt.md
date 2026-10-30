代发 wailian999

[U19] Py：正则替换带回调
来源：http://www.blog.hesvh.cn/Article/details/gdhsrkcrj.sHtML

re.sub(r"\d+", lambda m: str(int(m.group()) * 2), s)
来源：http://baike.zdbjq.cn/Article/details/gxwbrjpou.sHtML

[U20] Py：缓存函数结果
来源：http://www.share.zdbjq.cn/Article/details/gpjwamlwn.sHtML

@functools.lru_cache(maxsize=None)
来源：http://baike.zdbjq.cn/Article/details/givljumsv.sHtML

[U21] Py：自定义上下文管理器
来源：http://wap.zdbjq.cn/Article/details/gvnsvogxu.sHtML

@contextlib.contextmanager
来源：http://www.m.share.zdbjq.cn/Article/details/gcaicmhzi.sHtML

[U22] Py：矩阵转置
来源：http://wap.hesvh.cn/Article/details/gpikcqniz.sHtML

list(zip(*m))
来源：http://baike.hesvh.cn/Article/details/giumtqtpw.sHtML

[U23] Py：分块读取大文件
来源：http://baike.fehbvm.com/Article/details/gvfnqfwfn.sHtML

for chunk in iter(lambda: f.read(8192), b""):
来源：http://baike.fehbvm.com/Article/details/gvavovhbn.sHtML

[U24] Py：路径操作
来源：http://3g.hesvh.cn/Article/details/gwsqkujpf.sHtML

Path("a/b.txt").parent.mkdir(parents=True, exist_ok=True)
来源：http://www.m.share.hesvh.cn/Article/details/glykbzsez.sHtML

[U25] Py：CSV 按字典读
来源：http://blog.zdbjq.cn/Article/details/gbdfqnpgw.sHtML

csv.DictReader(f)
来源：http://blog.zdbjq.cn/Article/details/gkzhjfznn.sHtML

[U26] Py：并发下载
来源：http://blog.zdbjq.cn/Article/details/glmgblexl.sHtML

ThreadPoolExecutor(max_workers=8).map(fetch, urls)
来源：http://www.m.share.fehbvm.com/Article/details/gmazjlykp.sHtML

[U27] Py：异步 HTTP
来源：http://mobile.zdbjq.cn/Article/details/gkkpzyzdb.sHtML

aiohttp.ClientSession() 配合 async with
来源：http://mobile.zdbjq.cn/Article/details/glfjgzihg.sHtML

[U28] Py：类型别名
来源：http://mobile.hesvh.cn/Article/details/gaztmaqvo.sHtML

UserId = int
来源：http://baike.hesvh.cn/Article/details/gbvqmtnrp.sHtML

[U29] Py：属性校验
来源：http://mobile.fehbvm.com/Article/details/goebvlxwu.sHtML

@property 与 @x.setter 配合
来源：http://wap.fehbvm.com/Article/details/gvpbhfedr.sHtML

[U30] Py：数据类
来源：http://www.blog.fehbvm.com/Article/details/gvoqoqwuc.sHtML

@dataclass(slots=True)
来源：http://www.share.zdbjq.cn/Article/details/ghsmkvpjh.sHtML

[U31] Py：单测
来源：http://read.share.zdbjq.cn/Article/details/gpjdeleoc.sHtML

python -m pytest -q
来源：http://blog.fehbvm.com/Article/details/gsvavbqim.sHtML

[U32] Py：代码格式化
来源：http://www.blog.zdbjq.cn/Article/details/glvcjrjsd.sHtML

ruff format . && ruff check --fix .
来源：http://read.share.hesvh.cn/Article/details/ggwbxzlwz.sHtML

[U33] Py：打包发布
来源：http://3g.fehbvm.com/Article/details/glzgjcvlb.sHtML

python -m build  （依赖 pyproject.toml）
来源：http://www.m.share.fehbvm.com/Article/details/gciosdqcd.sHtML

[U34] Py：判断编码
来源：http://read.share.fehbvm.com/Article/details/grphzegir.sHtML

chardet.detect(raw)
来源：http://blog.zdbjq.cn/Article/details/gtofmgtcv.sHtML

[U35] Py：发送邮件
来源：http://m.share.zdbjq.cn/Article/details/gcrepwvok.sHtML

smtplib.SMTP_SSL(...).send_message(msg)
来源：http://www.share.hesvh.cn/Article/details/grfrvhfka.sHtML

[U36] Py：定时任务
来源：http://wap.zdbjq.cn/Article/details/gwazrqnny.sHtML

schedule.every(10).minutes.do(job)
来源：http://read.share.fehbvm.com/Article/details/gbaaesvuy.sHtML

[U37] Py：读写 Excel
来源：http://www.blog.fehbvm.com/Article/details/ggxegikiz.sHtML

pandas.read_excel / DataFrame.to_excel
来源：http://baike.zdbjq.cn/Article/details/grqygxgha.sHtML

[U38] Py：获取脚本所在目录
来源：http://www.share.hesvh.cn/Article/details/gmzujizis.sHtML

Path(__file__).resolve().parent
来源：http://www.m.share.fehbvm.com/Article/details/gulxkrqwi.sHtML

[U39] Py：判断是否在交互环境
来源：http://3g.zdbjq.cn/Article/details/guuvegwgn.sHtML

sys.stdout.isatty()
来源：http://m.share.fehbvm.com/Article/details/grzzypbrd.sHtML

[U40] Py：打印到标准错误
来源：http://www.share.hesvh.cn/Article/details/gzuimoepl.sHtML

print("err", file=sys.stderr)
来源：http://www.blog.zdbjq.cn/Article/details/gtdceryfi.sHtML

[U41] PHP：初始化 Composer 项目
来源：http://3g.hesvh.cn/Article/details/gxfolkxjq.sHtML

composer init;  composer require guzzlehttp/guzzle
来源：http://mobile.hesvh.cn/Article/details/geasnhaph.sHtML

[U42] PHP：PSR-4 自动加载
来源：http://blog.fehbvm.com/Article/details/gpklrerqk.sHtML

"autoload": { "psr-4": { "App\\": "src/" } }
来源：http://3g.fehbvm.com/Article/details/gbnviuyag.sHtML

[U43] PHP：声明命名空间
来源：http://www.share.fehbvm.com/Article/details/gxfuhgona.sHtML

namespace App\Http;
来源：http://read.share.fehbvm.com/Article/details/gnkmgqaah.sHtML

[U44] PHP：开启严格类型
来源：http://3g.hesvh.cn/Article/details/gfvpyfrda.sHtML

declare(strict_types=1);
来源：http://mobile.fehbvm.com/Article/details/genyivqir.sHtML

[U45] PHP：类型声明与返回类型
来源：http://baike.fehbvm.com/Article/details/gkftbwxni.sHtML

function add(int $a, int $b): int { return $a + $b; }
来源：http://www.m.share.fehbvm.com/Article/details/ggerleubg.sHtML

[U46] PHP：可空类型
来源：http://www.blog.fehbvm.com/Article/details/gomqprxvl.sHtML

?string $name = null
来源：http://m.share.fehbvm.com/Article/details/gvqxcyqok.sHtML

[U47] PHP：联合类型
来源：http://blog.zdbjq.cn/Article/details/gswcacssf.sHtML

int|string $id
来源：http://3g.hesvh.cn/Article/details/gwnnlyvxd.sHtML

[U48] PHP：纯枚举
来源：http://mobile.hesvh.cn/Article/details/gubqcrzyo.sHtML

enum Status: string { case Active = "active"; case Off = "off"; }
来源：http://www.m.share.hesvh.cn/Article/details/gllhgnysq.sHtML

[U49] PHP：只读属性
来源：http://www.blog.zdbjq.cn/Article/details/gqvyelqcq.sHtML

public readonly string $name
来源：http://www.share.fehbvm.com/Article/details/gfipifgom.sHtML

[U50] PHP：构造器属性提升
来源：http://mobile.hesvh.cn/Article/details/gbqgxixqu.sHtML

public function __construct(private int $id) {}
来源：http://baike.fehbvm.com/Article/details/gakvhsuyj.sHtML

[U51] PHP：数组解构
来源：http://read.share.zdbjq.cn/Article/details/gidpievki.sHtML

[$a, $b] = $arr;
来源：http://baike.fehbvm.com/Article/details/ggxejayge.sHtML

[U52] PHP：箭头函数
来源：http://wap.fehbvm.com/Article/details/gaovkcnth.sHtML

$double = fn($x) => $x * 2;
来源：http://3g.hesvh.cn/Article/details/gvrossqur.sHtML

[U53] PHP：空合并运算符
来源：http://read.share.hesvh.cn/Article/details/gzwivsesy.sHtML

$v = $a ?? $b ?? "default";
来源：http://blog.zdbjq.cn/Article/details/gtwadmcmb.sHtML

[U54] PHP：空安全调用
来源：http://mobile.hesvh.cn/Article/details/gnicfxhzb.sHtML

$obj?->method()
来源：http://mobile.fehbvm.com/Article/details/gretwtcdq.sHtML

[U55] PHP：match 表达式
来源：http://3g.zdbjq.cn/Article/details/guoxlmxqg.sHtML

$s = match($x) { 1 => "一", default => "其他" };
来源：http://baike.fehbvm.com/Article/details/gserlwpji.sHtML

[U56] PHP：命名参数
来源：http://www.share.hesvh.cn/Article/details/gvrpptkwf.sHtML

f(a: 1, b: 2)
来源：http://wap.hesvh.cn/Article/details/grpgfwvsi.sHtML

[U57] PHP：字符串插值
来源：http://www.m.share.fehbvm.com/Article/details/grfcbfxvz.sHtML

"值: {$a}"
来源：http://www.m.share.hesvh.cn/Article/details/gpxyusmti.sHtML

[U58] PHP：数组三件套
来源：http://www.blog.zdbjq.cn/Article/details/galdznmom.sHtML

array_map($f, $a);  array_filter($a, $f);  array_reduce($a, $f, 0);
来源：http://3g.hesvh.cn/Article/details/gttjwpoey.sHtML

[U59] PHP：自定义排序
来源：http://baike.zdbjq.cn/Article/details/gmcjkhihj.sHtML

usort($arr, fn($a, $b) => $a["age"] <=> $b["age"]);
来源：http://www.share.hesvh.cn/Article/details/gypijrkzk.sHtML

[U60] PHP：JSON 编解码
来源：http://www.share.zdbjq.cn/Article/details/gsbqsqhgy.sHtML

json_encode($d, JSON_UNESCAPED_UNICODE);  json_decode($s, true);
来源：http://wap.fehbvm.com/Article/details/gipcnrczi.sHtML

[U61] PHP：正则
来源：http://3g.zdbjq.cn/Article/details/gsojhilhs.sHtML

preg_match('/(\d+)/', $s, $m);  preg_replace('/\d+/', '#', $s);
来源：http://blog.zdbjq.cn/Article/details/grkukkmpz.sHtML

[U62] PHP：日期对象
来源：http://blog.hesvh.cn/Article/details/ghtmssbjd.sHtML

(new DateTimeImmutable())->format("Y-m-d");
来源：http://wap.zdbjq.cn/Article/details/gdezumznt.sHtML

[U63] PHP：文件读写
来源：http://read.share.hesvh.cn/Article/details/govwneayj.sHtML

file_get_contents($f);  file_put_contents($f, $data);
来源：http://read.share.hesvh.cn/Article/details/gxqkypctu.sHtML

[U64] PHP：目录遍历
来源：http://www.share.fehbvm.com/Article/details/gdinwejao.sHtML

glob("dir/*.php");  scandir("dir");
来源：http://www.blog.fehbvm.com/Article/details/gubmvdbtj.sHtML

[U65] PHP：会话
来源：http://3g.zdbjq.cn/Article/details/glmhbdggk.sHtML

session_start();  $_SESSION["uid"] = 1;
来源：http://read.share.hesvh.cn/Article/details/ghrvrmvvq.sHtML

[U66] PHP：设置 Cookie
来源：http://www.share.hesvh.cn/Article/details/gernonxad.sHtML

setcookie("token", $v, ["httponly" => true, "samesite" => "Lax"]);
来源：http://baike.hesvh.cn/Article/details/gvoaqidjk.sHtML

[U67] PHP：处理文件上传
来源：http://www.blog.fehbvm.com/Article/details/gcjktmczm.sHtML

$_FILES["file"]["tmp_name"] 与 move_uploaded_file()
来源：http://www.blog.fehbvm.com/Article/details/gcwddigrz.sHtML

[U68] PHP：PDO 连接
来源：http://3g.fehbvm.com/Article/details/gzelkubyy.sHtML

$pdo = new PDO("mysql:host=localhost;dbname=app", "root", "");
来源：http://blog.fehbvm.com/Article/details/gqakqwajo.sHtML

[U69] PHP：PDO 预处理
来源：http://wap.hesvh.cn/Article/details/gvdlktoij.sHtML

$stmt = $pdo->prepare("SELECT * FROM users WHERE id = ?");  $stmt->execute([$id]);
来源：http://wap.fehbvm.com/Article/details/gfheygjdv.sHtML

[U70] PHP：PDO 事务
来源：http://read.share.zdbjq.cn/Article/details/gihfigvti.sHtML

$pdo->beginTransaction();  $pdo->commit();  $pdo->rollBack();
来源：http://mobile.fehbvm.com/Article/details/gqruwyola.sHtML

[U71] PHP：抛出异常
来源：http://www.m.share.zdbjq.cn/Article/details/gacpzsctq.sHtML

throw new RuntimeException("失败", 500);
来源：http://baike.hesvh.cn/Article/details/gpbrilhds.sHtML

[U72] PHP：写错误日志
来源：http://baike.fehbvm.com/Article/details/gbrgcrcze.sHtML

error_log("失败: " . $e->getMessage());
来源：http://3g.hesvh.cn/Article/details/gbeuisnbk.sHtML

[U73] PHP：读取 ini 配置
来源：http://read.share.fehbvm.com/Article/details/gilxeydcg.sHtML

parse_ini_file("config.ini", true)
来源：http://www.share.fehbvm.com/Article/details/gczehqvxj.sHtML

[U74] PHP：读取环境变量
来源：http://m.share.zdbjq.cn/Article/details/gkzhfudlb.sHtML

getenv("APP_ENV") ?: "production"
来源：http://www.m.share.zdbjq.cn/Article/details/gjfjxnfrz.sHtML

[U75] PHP：依赖注入
来源：http://m.share.hesvh.cn/Article/details/ghruspdjc.sHtML

composer require psr/container
来源：http://mobile.hesvh.cn/Article/details/gmnebtfvm.sHtML

[U76] PHP：简单路由
来源：http://read.share.fehbvm.com/Article/details/gscvycbxg.sHtML

$path = parse_url($_SERVER["REQUEST_URI"], PHP_URL_PATH);
来源：http://3g.fehbvm.com/Article/details/gsctrvcas.sHtML

[U77] PHP：模板渲染
来源：http://mobile.fehbvm.com/Article/details/gbmuwrvbj.sHtML

composer require twig/twig
来源：http://www.share.hesvh.cn/Article/details/gtxnixxrv.sHtML

[U78] PHP：单元测试
来源：http://m.share.zdbjq.cn/Article/details/gfzusdsho.sHtML

composer require --dev phpunit/phpunit
来源：http://www.share.zdbjq.cn/Article/details/gwlwxjfeq.sHtML

[U79] PHP：静态分析
来源：http://baike.zdbjq.cn/Article/details/ggyonytsa.sHtML

composer require --dev phpstan/phpstan
来源：http://wap.hesvh.cn/Article/details/gopsvpuur.sHtML

[U80] PHP：代码规范修复
来源：http://www.share.fehbvm.com/Article/details/geqkyfred.sHtML

composer require --dev friendsofphp/php-cs-fixer
来源：http://www.m.share.fehbvm.com/Article/details/gyomrlphz.sHtML

[U81] JS：初始化项目
来源：http://blog.hesvh.cn/Article/details/gmymstwhb.sHtML

npm init -y;  npm i express
来源：http://baike.hesvh.cn/Article/details/gonddjwkf.sHtML

[U82] JS：package.json 脚本
来源：http://3g.zdbjq.cn/Article/details/gjmldvuza.sHtML

"scripts": { "dev": "vite", "build": "vite build" }
来源：http://www.m.share.hesvh.cn/Article/details/gdvnvyehg.sHtML

[U83] JS：ES Module 导入导出
来源：http://read.share.hesvh.cn/Article/details/gthxtbpvb.sHtML

export const a = 1;  import { a } from "./m.js";
来源：http://mobile.fehbvm.com/Article/details/gmzaoyqrd.sHtML

[U84] JS：CommonJS 写法
来源：http://m.share.zdbjq.cn/Article/details/gwgeajorn.sHtML

module.exports = { a };  const { a } = require("./m");
来源：http://m.share.hesvh.cn/Article/details/gtimicbdu.sHtML

[U85] JS：可选链
来源：http://read.share.fehbvm.com/Article/details/gjbelhnld.sHtML

a?.b?.c
来源：http://www.share.hesvh.cn/Article/details/gahrejyoh.sHtML

[U86] JS：空值合并
来源：http://baike.zdbjq.cn/Article/details/glbzrvdnt.sHtML

a ?? b
来源：http://wap.hesvh.cn/Article/details/gxetoleos.sHtML

[U87] JS：解构默认值
来源：http://wap.fehbvm.com/Article/details/gnxosefgh.sHtML

const { a = 1, b = 2 } = obj;
来源：http://mobile.hesvh.cn/Article/details/gebhpcmzu.sHtML

[U88] JS：对象展开合并
来源：http://read.share.hesvh.cn/Article/details/grzapcvrb.sHtML

{ ...a, ...b }
来源：http://wap.fehbvm.com/Article/details/gheeccssb.sHtML

[U89] JS：数组去重
来源：http://baike.hesvh.cn/Article/details/gklwsstgf.sHtML

[...new Set(arr)]
来源：http://baike.fehbvm.com/Article/details/gylpuarpn.sHtML

[U90] JS：数字数组排序
来源：http://3g.fehbvm.com/Article/details/gdnolfmre.sHtML

[...arr].sort((a, b) => a - b)
来源：http://www.m.share.hesvh.cn/Article/details/gqmvegunq.sHtML

[U91] JS：对象键值遍历
来源：http://read.share.zdbjq.cn/Article/details/gvwgixcyy.sHtML

Object.entries(obj).forEach(([k, v]) => {});
来源：http://3g.zdbjq.cn/Article/details/gdtsymzds.sHtML

[U92] JS：深拷贝
来源：http://mobile.zdbjq.cn/Article/details/gzzyxyjiu.sHtML

structuredClone(obj)
来源：http://mobile.fehbvm.com/Article/details/gzdkwqowq.sHtML

[U93] JS：模板字符串
来源：http://www.blog.zdbjq.cn/Article/details/gmfsujosh.sHtML

`共 ${n} 条`
来源：http://www.share.hesvh.cn/Article/details/gfrtulvch.sHtML

[U94] JS：箭头函数
来源：http://www.share.zdbjq.cn/Article/details/gkoetdxrh.sHtML

const double = x => x * 2;
来源：http://wap.fehbvm.com/Article/details/ggknqtsvk.sHtML

[U95] JS：Promise 包装
来源：http://3g.hesvh.cn/Article/details/gmyyhduij.sHtML

new Promise((resolve, reject) => {})
来源：http://baike.fehbvm.com/Article/details/gcyxbrkzs.sHtML

[U96] JS：async/await 与异常
来源：http://wap.fehbvm.com/Article/details/gvhhmltvc.sHtML

try { const d = await f(); } catch (e) { console.error(e); }
来源：http://blog.zdbjq.cn/Article/details/gduisilwl.sHtML

[U97] JS：并发请求
来源：http://read.share.fehbvm.com/Article/details/ghbfnstpl.sHtML

await Promise.all(urls.map(u => fetch(u)))
来源：http://mobile.zdbjq.cn/Article/details/gtmgpygrd.sHtML

[U98] JS：fetch 带 JSON
来源：http://3g.fehbvm.com/Article/details/gvhxcyden.sHtML

await fetch(url, { method: "POST", headers: { "Content-Type": "application/json" }, body: JSON.stringify(d) })
来源：http://www.m.share.hesvh.cn/Article/details/gdfrtedld.sHtML

[U99] JS：事件监听
来源：http://www.share.zdbjq.cn/Article/details/glvkiubgq.sHtML

el.addEventListener("click", e => {})
来源：http://www.m.share.hesvh.cn/Article/details/gbptkxann.sHtML

[U100] JS：DOM 查询
来源：http://www.share.hesvh.cn/Article/details/getrwdsqn.sHtML

document.querySelector(".item")
来源：http://m.share.zdbjq.cn/Article/details/ggrrxldrq.sHtML

[U101] JS：classList 操作
来源：http://wap.hesvh.cn/Article/details/gwbrubccj.sHtML

el.classList.toggle("active")
来源：http://blog.zdbjq.cn/Article/details/gigdgvrsl.sHtML

[U102] JS：本地存储
来源：http://baike.zdbjq.cn/Article/details/gdejylsha.sHtML

localStorage.setItem("k", JSON.stringify(v))
来源：http://read.share.zdbjq.cn/Article/details/gqcqseoqv.sHtML

[U103] JS：定时器
来源：http://m.share.hesvh.cn/Article/details/giluohvzg.sHtML

setTimeout(fn, 1000);  setInterval(fn, 1000);
来源：http://read.share.fehbvm.com/Article/details/gmadweeju.sHtML

[U104] JS：防抖
来源：http://wap.fehbvm.com/Article/details/gmblmugdm.sHtML

const debounce = (fn, ms) => { let t; return (...a) => { clearTimeout(t); t = setTimeout(() => fn(...a), ms); }; };
来源：http://www.share.hesvh.cn/Article/details/gdeauinxy.sHtML

[U105] JS：节流
来源：http://3g.zdbjq.cn/Article/details/gypqvzggw.sHtML

const throttle = (fn, ms) => { let last = 0; return (...a) => { const n = Date.now(); if (n - last >= ms) { last = n; fn(...a); } }; };
来源：http://mobile.hesvh.cn/Article/details/giiulrrnw.sHtML

[U106] JS：日期格式化
来源：http://m.share.fehbvm.com/Article/details/glstqgkhf.sHtML

new Intl.DateTimeFormat("zh-CN", { dateStyle: "medium" }).format(new Date())
来源：http://wap.hesvh.cn/Article/details/gocsircmq.sHtML

[U107] JS：数字千分位
来源：http://mobile.fehbvm.com/Article/details/gzayxjtjt.sHtML

new Intl.NumberFormat("en-US").format(1234567)
来源：http://blog.hesvh.cn/Article/details/gptdtpbke.sHtML

[U108] JS：随机整数
来源：http://www.blog.zdbjq.cn/Article/details/gczbwojpe.sHtML

Math.floor(Math.random() * (max - min + 1)) + min
来源：http://wap.zdbjq.cn/Article/details/gooucqbuz.sHtML

[U109] JS：数组分组
来源：http://blog.hesvh.cn/Article/details/gzuymzjua.sHtML

Object.groupBy(arr, x => x.type)
来源：http://read.share.hesvh.cn/Article/details/gmzrhbzac.sHtML

[U110] JS：数组分块
来源：http://3g.zdbjq.cn/Article/details/gtqzrutce.sHtML

arr.reduce((acc, x, i) => (i % size ? acc : [...acc, arr.slice(i, i + size)]), [])
来源：http://www.blog.zdbjq.cn/Article/details/ghqksnigs.sHtML

[U111] JS：对象转 Map
来源：http://wap.fehbvm.com/Article/details/gtbkfdxep.sHtML

new Map(Object.entries(obj))
来源：http://www.blog.fehbvm.com/Article/details/gzqnxslye.sHtML

[U112] JS：字符串补位
来源：http://wap.zdbjq.cn/Article/details/gmwxcptsj.sHtML

"7".padStart(3, "0")
来源：http://read.share.hesvh.cn/Article/details/gitxubfgn.sHtML

[U113] JS：正则替换全部
来源：http://www.share.hesvh.cn/Article/details/gramsylgt.sHtML

s.replaceAll("a", "b")
来源：http://mobile.zdbjq.cn/Article/details/gwnhuxxzv.sHtML

[U114] JS：JSON 深比较
来源：http://www.blog.fehbvm.com/Article/details/genvsdiws.sHtML

JSON.stringify(a) === JSON.stringify(b)
来源：http://www.blog.hesvh.cn/Article/details/gzgdbtcfq.sHtML

[U115] JS：生成 UUID
来源：http://www.blog.hesvh.cn/Article/details/gorwqxdqv.sHtML

crypto.randomUUID()
来源：http://www.m.share.fehbvm.com/Article/details/gbcnxlibr.sHtML

[U116] JS：类型检查（JSDoc）
来源：http://www.blog.hesvh.cn/Article/details/griktvggd.sHtML

/** @param {string} name */ function f(name) {}
来源：http://m.share.zdbjq.cn/Article/details/gmjsimxgk.sHtML

[U117] JS：单元测试
来源：http://read.share.hesvh.cn/Article/details/gyxmxzdet.sHtML

npm i -D vitest;  npx vitest
来源：http://read.share.zdbjq.cn/Article/details/gobuqnfbm.sHtML

[U118] JS：开发服务器
来源：http://m.share.hesvh.cn/Article/details/gkazesxnx.sHtML

npm i -D vite;  npx vite
来源：http://blog.zdbjq.cn/Article/details/gpwzpfmks.sHtML

[U119] JS：生产构建
来源：http://3g.hesvh.cn/Article/details/gikphpckg.sHtML

npx vite build
来源：http://mobile.zdbjq.cn/Article/details/gjoutjvfb.sHtML

[U120] JS：读取环境变量（Vite）
来源：http://www.share.fehbvm.com/Article/details/gvbvrzaad.sHtML

import.meta.env.VITE_API_URL
来源：http://m.share.hesvh.cn/Article/details/gnybnnzrn.sHtML

================================================================================
来源：http://www.blog.fehbvm.com/Article/details/gpisflloe.sHtML

统计汇总
来源：http://www.m.share.hesvh.cn/Article/details/geiewlmyu.sHtML

================================================================================
来源：http://mobile.fehbvm.com/Article/details/gjejynloq.sHtML

按语言统计（条）：
来源：http://www.share.zdbjq.cn/Article/details/givmbzdaz.sHtML

Python ......... 252
来源：http://www.blog.hesvh.cn/Article/details/gpjowzydz.sHtML

PHP ............ 252
来源：http://www.share.zdbjq.cn/Article/details/ghmsrhcjv.sHtML

JavaScript ..... 252
来源：http://www.m.share.fehbvm.com/Article/details/gxmllqfvp.sHtML

TypeScript ..... 212
来源：http://read.share.hesvh.cn/Article/details/glrzaydqs.sHtML

Java ........... 212
来源：http://baike.hesvh.cn/Article/details/gojnajctg.sHtML

Go ............. 212
来源：http://www.m.share.zdbjq.cn/Article/details/gxaacunkm.sHtML

Ruby ........... 212
来源：http://www.share.zdbjq.cn/Article/details/ggjgedlgt.sHtML

C# ............. 212
来源：http://mobile.fehbvm.com/Article/details/gcwdmwckz.sHtML

C .............. 30
来源：http://www.share.fehbvm.com/Article/details/gjfktmwqj.sHtML

C++ ............ 30
来源：http://mobile.zdbjq.cn/Article/details/gluscufyf.sHtML

SQL ............ 90
来源：http://mobile.hesvh.cn/Article/details/gufwougtv.sHtML

Bash ........... 80
来源：http://read.share.hesvh.cn/Article/details/ghqsqbxbz.sHtML

Kotlin ......... 15
来源：http://www.share.zdbjq.cn/Article/details/ghkeirpwv.sHtML

Swift .......... 15
来源：http://www.share.hesvh.cn/Article/details/gabofkijb.sHtML

Lua ............ 10
来源：http://read.share.hesvh.cn/Article/details/gacoltiui.sHtML

Perl ........... 10
来源：http://3g.hesvh.cn/Article/details/gabjzznxd.sHtML

Scala .......... 10
来源：http://www.share.hesvh.cn/Article/details/gxpkkxqkb.sHtML

------------------------------------
来源：http://wap.hesvh.cn/Article/details/gaylapgdl.sHtML

合计 ........... 2106 条
来源：http://mobile.hesvh.cn/Article/details/ghdnlzyrb.sHtML

按章节统计：
来源：http://m.share.zdbjq.cn/Article/details/gfmzsemoy.sHtML

A 基础语法与类型       26 个任务 × 8 语言 =  208
来源：http://www.share.fehbvm.com/Article/details/gyqvkuyeu.sHtML

B 流程控制             16 个任务 × 8 语言 =  128
来源：http://blog.hesvh.cn/Article/details/ghdiipqgb.sHtML

C 函数与作用域         16 个任务 × 8 语言 =  128
来源：http://www.blog.zdbjq.cn/Article/details/gjdkgtaxr.sHtML

D 数组 / 列表 / 集合   26 个任务 × 8 语言 =  208
来源：http://www.m.share.hesvh.cn/Article/details/gdthopvvp.sHtML

E 字符串处理           22 个任务 × 8 语言 =  176
来源：http://www.share.hesvh.cn/Article/details/gjotzockz.sHtML

F 文件与目录           12 个任务 × 8 语言 =   96
来源：http://read.share.hesvh.cn/Article/details/gxfkbpbue.sHtML

G 面向对象             16 个任务 × 8 语言 =  128
来源：http://www.share.fehbvm.com/Article/details/gibjkencq.sHtML

H 异常与错误处理       10 个任务 × 8 语言 =   80
来源：http://www.blog.zdbjq.cn/Article/details/gvvhjjbzm.sHtML

I 正则表达式            8 个任务 × 8 语言 =   64
来源：http://m.share.zdbjq.cn/Article/details/groqeqgkl.sHtML

J 日期与时间           10 个任务 × 8 语言 =   80
来源：http://read.share.fehbvm.com/Article/details/gjigimfwa.sHtML

K JSON 与序列化         8 个任务 × 8 语言 =   64
来源：http://www.blog.hesvh.cn/Article/details/grafrtzph.sHtML

L 网络请求              8 个任务 × 8 语言 =   64
来源：http://www.blog.zdbjq.cn/Article/details/gjjlewzqk.sHtML

M 命令行 / 进程         8 个任务 × 8 语言 =   64
来源：http://baike.fehbvm.com/Article/details/gypvyirdf.sHtML

N 数据结构与算法       12 个任务 × 8 语言 =   96
来源：http://m.share.zdbjq.cn/Article/details/gcqqhzkeo.sHtML

O 并发与异步            6 个任务 × 8 语言 =   48
来源：http://blog.zdbjq.cn/Article/details/gjzdixgad.sHtML

P 常用工具函数          8 个任务 × 8 语言 =   64
来源：http://read.share.fehbvm.com/Article/details/gcqbczsxq.sHtML

Q SQL 专题                              90
来源：http://www.blog.hesvh.cn/Article/details/gbnobzgwr.sHtML

R Bash 专题                             80
来源：http://www.blog.hesvh.cn/Article/details/gunyczytd.sHtML

S C / C++ 专题                          60
来源：http://3g.zdbjq.cn/Article/details/gfmswuwlj.sHtML

T 其他语言补充                          60
来源：http://3g.fehbvm.com/Article/details/gclkxlsad.sHtML

U 高频实用片段                         120
来源：http://3g.fehbvm.com/Article/details/gxzkccdsw.sHtML

------------------------------------
来源：http://mobile.hesvh.cn/Article/details/gwcmrxcre.sHtML

合计                                  2106 条
来源：http://www.m.share.hesvh.cn/Article/details/gbzupkcfx.sHtML

--------------------------------------------------------------------------------
来源：http://www.share.fehbvm.com/Article/details/gmotzhizj.sHtML

使用提醒
来源：http://read.share.hesvh.cn/Article/details/gofthojyy.sHtML

--------------------------------------------------------------------------------
来源：http://www.share.hesvh.cn/Article/details/gpecvjozn.sHtML

1. 示例追求"最小可用"，正式项目中请补齐导入、错误处理与边界判断。
来源：http://read.share.zdbjq.cn/Article/details/gzpzcqvyh.sHtML

2. 涉及文件、网络、数据库的示例，注意资源释放与异常捕获。
来源：http://m.share.fehbvm.com/Article/details/ghlfdbodh.sHtML

3. 语言版本差异较大（如 Python 3.10 的 match、Java 17 的 record/switch 箭头），
来源：http://mobile.zdbjq.cn/Article/details/gvikcuwzo.sHtML

在旧版本上使用前请先确认语法支持情况。
来源：http://www.m.share.zdbjq.cn/Article/details/gsfneqbbr.sHtML

4. 标注"手写"的条目是因为该语言缺少对应内置能力，实际项目中可引入成熟库。
来源：http://www.share.hesvh.cn/Article/details/gbblkptar.sHtML

—— 文件结束 ——
来源：http://read.share.zdbjq.cn/Article/details/gdzzrpgpg.sHtML

================================================================================
来源：http://blog.zdbjq.cn/Article/details/gpcafhlpy.sHtML

程序语言常见例子速查手册（2024 版）
来源：http://mobile.hesvh.cn/Article/details/gnocojbkt.sHtML

Common Programming Examples Cheat Book
来源：http://baike.hesvh.cn/Article/details/gslonxktg.sHtML

================================================================================
来源：http://baike.hesvh.cn/Article/details/gljpskzkb.sHtML

【收录内容】
来源：http://www.blog.hesvh.cn/Article/details/gbjhtgvqs.sHtML

覆盖 12 种语言 / 语法与常见 API：
来源：http://www.m.share.hesvh.cn/Article/details/gzaspurzq.sHtML

Python · PHP · JavaScript · TypeScript · Java · Go · Ruby · C#
来源：http://www.share.fehbvm.com/Article/details/gufrdtrzq.sHtML

SQL · Bash · C · C++
来源：http://blog.hesvh.cn/Article/details/gdgpnchou.sHtML

按「任务」分组：每个任务下按语言各给出一条最小可用示例。
来源：http://baike.zdbjq.cn/Article/details/gqpmojfip.sHtML

【使用说明】
来源：http://www.share.fehbvm.com/Article/details/gbvxnvggb.sHtML

1. 每个任务形如 "[编号] 任务名"，下面每行以语言标记开头：
来源：http://3g.hesvh.cn/Article/details/gblclrkgw.sHtML

Py:    Python        PHP:   PHP           JS:    JavaScript
来源：http://www.share.hesvh.cn/Article/details/gnlznminy.sHtML

TS:    TypeScript    Java:  Java          Go:    Go
来源：http://www.share.hesvh.cn/Article/details/guikoyxll.sHtML

Ruby:  Ruby          C#:    C#            SQL:   SQL
来源：http://blog.hesvh.cn/Article/details/gcxidrvho.sHtML

Bash:  Shell         C:     C             C++:   C++
来源：http://read.share.fehbvm.com/Article/details/gmohjwkld.sHtML

2. 示例只展示核心写法，刻意省略 import / require / include / using 等样板代码。
来源：http://mobile.zdbjq.cn/Article/details/gombzflzo.sHtML

需要完整可运行文件时，请自行补齐当前语言的导入语句。
来源：http://www.share.zdbjq.cn/Article/details/grnvhaexy.sHtML

3. 语法基准：Python 3.10+ / PHP 8.1+ / ES2020+ / TypeScript 5 / Java 17 /
来源：http://3g.zdbjq.cn/Article/details/gbllghskt.sHtML

Go 1.21+ / Ruby 3.x / C# 10+ / C17 / C++17。
来源：http://m.share.zdbjq.cn/Article/details/gaqlqpleq.sHtML

4. 检索建议：用编辑器或浏览器 Ctrl+F 搜关键词，如 "排序" "读取文件" "正则"。
来源：http://www.share.hesvh.cn/Article/details/gzzggneaf.sHtML

5. 标记为 "// 无" 表示该语言没有对应的一等语法，需用替代写法（示例给出替代方案）。
来源：http://blog.fehbvm.com/Article/details/gtgbsippo.sHtML

6. 符号 "⏎" 表示代码在此处换行（主要用于 Python 等强制缩进、无法压成一行的结构）。
来源：http://blog.zdbjq.cn/Article/details/gvymukovh.sHtML

【文件统计】
来源：http://wap.hesvh.cn/Article/details/grfpvpxyq.sHtML

语言示例共 2106 条，分布见本文末尾的「统计汇总」。
来源：http://wap.zdbjq.cn/Article/details/gjsffybok.sHtML

--------------------------------------------------------------------------------
来源：http://mobile.hesvh.cn/Article/details/ghuflfjrq.sHtML

目  录
来源：http://m.share.hesvh.cn/Article/details/gbfonxzrj.sHtML

--------------------------------------------------------------------------------
来源：http://m.share.zdbjq.cn/Article/details/gdennvpqh.sHtML

A. 基础语法与类型              （第 1 节，26 个任务，208 条）
来源：http://blog.zdbjq.cn/Article/details/gfofepbci.sHtML

B. 流程控制                    （第 2 节，16 个任务，128 条）
来源：http://m.share.hesvh.cn/Article/details/grjsswpid.sHtML

C. 函数与作用域                （第 3 节，16 个任务，128 条）
来源：http://read.share.fehbvm.com/Article/details/golspdqnc.sHtML

D. 数组 / 列表 / 集合          （第 4 节，26 个任务，208 条）
来源：http://wap.hesvh.cn/Article/details/glpkdumrs.sHtML

E. 字符串处理                  （第 5 节，22 个任务，176 条）
来源：http://www.share.fehbvm.com/Article/details/gjxptirlf.sHtML

F. 文件与目录                  （第 6 节，12 个任务，96 条）
来源：http://m.share.fehbvm.com/Article/details/glghqvnmm.sHtML

G. 面向对象                    （第 7 节，16 个任务，128 条）
来源：http://www.share.hesvh.cn/Article/details/gwgqrayho.sHtML

H. 异常与错误处理              （第 8 节，10 个任务，80 条）
来源：http://www.m.share.fehbvm.com/Article/details/gkkwttilh.sHtML

I. 正则表达式                  （第 9 节，8 个任务，64 条）
来源：http://www.m.share.hesvh.cn/Article/details/gyfhbonaf.sHtML

J. 日期与时间                  （第 10 节，10 个任务，80 条）
来源：http://3g.zdbjq.cn/Article/details/glsmnljuv.sHtML

K. JSON 与序列化               （第 11 节，8 个任务，64 条）
来源：http://www.m.share.hesvh.cn/Article/details/gelxawrqb.sHtML

L. 网络请求                    （第 12 节，8 个任务，64 条）
来源：http://www.blog.zdbjq.cn/Article/details/gqwumppnv.sHtML

M. 命令行 / 进程 / 环境        （第 13 节，8 个任务，64 条）
来源：http://baike.zdbjq.cn/Article/details/ghczniaci.sHtML


<!-- 参考信息 -->