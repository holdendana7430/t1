代发 wailian999

[U17] Py：初始化日志
来源：http://blog.fanxiaobao.xyz/Article/details/gwerhuaei.sHtML

logging.basicConfig(level=logging.INFO)
来源：http://3g.fanxiaobao.xyz/Article/details/gqkmbpqbd.sHtML

[U18] Py：预编译正则
来源：http://3g.fanxiaobao.xyz/Article/details/ggjoqcetx.sHtML

pat = re.compile(r"\d+")
来源：http://blog.fanxiaobao.xyz/Article/details/ggypmtubc.sHtML

[U19] Py：正则替换带回调
来源：http://www.share.fanxiaobao.xyz/Article/details/gkuyfahbo.sHtML

re.sub(r"\d+", lambda m: str(int(m.group()) * 2), s)
来源：http://www.share.fanxiaobao.xyz/Article/details/gpgvbheni.sHtML

[U20] Py：缓存函数结果
来源：http://www.share.fanxiaobao.xyz/Article/details/gvesdsmft.sHtML

@functools.lru_cache(maxsize=None)
来源：http://3g.fanxiaobao.xyz/Article/details/gvwtbwmyl.sHtML

[U21] Py：自定义上下文管理器
来源：http://www.share.fanxiaobao.xyz/Article/details/gtgebdmhx.sHtML

@contextlib.contextmanager
来源：http://3g.fanxiaobao.xyz/Article/details/gtazygmab.sHtML

[U22] Py：矩阵转置
来源：http://www.share.fanxiaobao.xyz/Article/details/glnlyrbpd.sHtML

list(zip(*m))
来源：http://wap.fanxiaobao.xyz/Article/details/grsinhbtv.sHtML

[U23] Py：分块读取大文件
来源：http://m.share.fanxiaobao.xyz/Article/details/gbggnchox.sHtML

for chunk in iter(lambda: f.read(8192), b""):
来源：http://3g.fanxiaobao.xyz/Article/details/ggmprotxq.sHtML

[U24] Py：路径操作
来源：http://m.share.fanxiaobao.xyz/Article/details/gohirqbdi.sHtML

Path("a/b.txt").parent.mkdir(parents=True, exist_ok=True)
来源：http://baike.fanxiaobao.xyz/Article/details/gettutniu.sHtML

[U25] Py：CSV 按字典读
来源：http://www.m.share.fanxiaobao.xyz/Article/details/ggokwcchj.sHtML

csv.DictReader(f)
来源：http://wap.fanxiaobao.xyz/Article/details/gteazsmxq.sHtML

[U26] Py：并发下载
来源：http://baike.fanxiaobao.xyz/Article/details/ggtrcjfcf.sHtML

ThreadPoolExecutor(max_workers=8).map(fetch, urls)
来源：http://read.share.fanxiaobao.xyz/Article/details/glghmbmey.sHtML

[U27] Py：异步 HTTP
来源：http://mobile.fanxiaobao.xyz/Article/details/gcbusaepz.sHtML

aiohttp.ClientSession() 配合 async with
来源：http://m.share.fanxiaobao.xyz/Article/details/gfysnxqyp.sHtML

[U28] Py：类型别名
来源：http://blog.fanxiaobao.xyz/Article/details/gadofabsn.sHtML

UserId = int
来源：http://m.share.fanxiaobao.xyz/Article/details/gucaxupcg.sHtML

[U29] Py：属性校验
来源：http://wap.fanxiaobao.xyz/Article/details/gvoaydchn.sHtML

@property 与 @x.setter 配合
来源：http://baike.fanxiaobao.xyz/Article/details/grdinxeob.sHtML

[U30] Py：数据类
来源：http://mobile.fanxiaobao.xyz/Article/details/gntraravv.sHtML

@dataclass(slots=True)
来源：http://blog.fanxiaobao.xyz/Article/details/gnbgnltyq.sHtML

[U31] Py：单测
来源：http://www.m.share.fanxiaobao.xyz/Article/details/grhawysnp.sHtML

python -m pytest -q
来源：http://mobile.fanxiaobao.xyz/Article/details/giaalrobg.sHtML

[U32] Py：代码格式化
来源：http://m.share.fanxiaobao.xyz/Article/details/guyrafxda.sHtML

ruff format . && ruff check --fix .
来源：http://www.m.share.fanxiaobao.xyz/Article/details/ghkslijcu.sHtML

[U33] Py：打包发布
来源：http://baike.fanxiaobao.xyz/Article/details/gscxpgobv.sHtML

python -m build  （依赖 pyproject.toml）
来源：http://3g.fanxiaobao.xyz/Article/details/gsaqlibyj.sHtML

[U34] Py：判断编码
来源：http://www.blog.fanxiaobao.xyz/Article/details/glfkrrhzx.sHtML

chardet.detect(raw)
来源：http://www.m.share.fanxiaobao.xyz/Article/details/glrafxdim.sHtML

[U35] Py：发送邮件
来源：http://www.share.fanxiaobao.xyz/Article/details/gosxqcnnx.sHtML

smtplib.SMTP_SSL(...).send_message(msg)
来源：http://mobile.fanxiaobao.xyz/Article/details/ggvndgsfw.sHtML

[U36] Py：定时任务
来源：http://baike.fanxiaobao.xyz/Article/details/gacdydzih.sHtML

schedule.every(10).minutes.do(job)
来源：http://wap.fanxiaobao.xyz/Article/details/gaiexelha.sHtML

[U37] Py：读写 Excel
来源：http://www.share.fanxiaobao.xyz/Article/details/gmvwynfhj.sHtML

pandas.read_excel / DataFrame.to_excel
来源：http://mobile.fanxiaobao.xyz/Article/details/gbajeoxgj.sHtML

[U38] Py：获取脚本所在目录
来源：http://wap.fanxiaobao.xyz/Article/details/gjsqtymmz.sHtML

Path(__file__).resolve().parent
来源：http://www.blog.fanxiaobao.xyz/Article/details/gsgjxpirc.sHtML

[U39] Py：判断是否在交互环境
来源：http://3g.fanxiaobao.xyz/Article/details/gvjxhuopc.sHtML

sys.stdout.isatty()
来源：http://mobile.fanxiaobao.xyz/Article/details/gxunxaciu.sHtML

[U40] Py：打印到标准错误
来源：http://www.m.share.fanxiaobao.xyz/Article/details/goojrljsf.sHtML

print("err", file=sys.stderr)
来源：http://read.share.fanxiaobao.xyz/Article/details/ginwjbmjl.sHtML

[U41] PHP：初始化 Composer 项目
来源：http://www.blog.fanxiaobao.xyz/Article/details/grvzusgfm.sHtML

composer init;  composer require guzzlehttp/guzzle
来源：http://3g.fanxiaobao.xyz/Article/details/gwuhrhmol.sHtML

[U42] PHP：PSR-4 自动加载
来源：http://m.share.fanxiaobao.xyz/Article/details/gklsogfea.sHtML

"autoload": { "psr-4": { "App\\": "src/" } }
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gfbaqwhxy.sHtML

[U43] PHP：声明命名空间
来源：http://read.share.fanxiaobao.xyz/Article/details/ggpuyzace.sHtML

namespace App\Http;
来源：http://mobile.fanxiaobao.xyz/Article/details/gowvlsuyy.sHtML

[U44] PHP：开启严格类型
来源：http://www.m.share.fanxiaobao.xyz/Article/details/grgcmknem.sHtML

declare(strict_types=1);
来源：http://m.share.fanxiaobao.xyz/Article/details/giglbunpd.sHtML

[U45] PHP：类型声明与返回类型
来源：http://blog.fanxiaobao.xyz/Article/details/gctsjrxow.sHtML

function add(int $a, int $b): int { return $a + $b; }
来源：http://read.share.fanxiaobao.xyz/Article/details/gvbbyqddn.sHtML

[U46] PHP：可空类型
来源：http://mobile.fanxiaobao.xyz/Article/details/gkyvrfbpc.sHtML

?string $name = null
来源：http://blog.fanxiaobao.xyz/Article/details/grnravzbr.sHtML

[U47] PHP：联合类型
来源：http://m.share.fanxiaobao.xyz/Article/details/gsjvdugbo.sHtML

int|string $id
来源：http://3g.fanxiaobao.xyz/Article/details/gfaumlzxs.sHtML

[U48] PHP：纯枚举
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gugidhgry.sHtML

enum Status: string { case Active = "active"; case Off = "off"; }
来源：http://www.blog.fanxiaobao.xyz/Article/details/gnadtumvu.sHtML

[U49] PHP：只读属性
来源：http://blog.fanxiaobao.xyz/Article/details/gcsguemsr.sHtML

public readonly string $name
来源：http://baike.fanxiaobao.xyz/Article/details/gizdrnkzo.sHtML

[U50] PHP：构造器属性提升
来源：http://www.blog.fanxiaobao.xyz/Article/details/grnhkpsmf.sHtML

public function __construct(private int $id) {}
来源：http://baike.fanxiaobao.xyz/Article/details/gqiuoqtxg.sHtML

[U51] PHP：数组解构
来源：http://baike.fanxiaobao.xyz/Article/details/geqwhbnbl.sHtML

[$a, $b] = $arr;
来源：http://3g.fanxiaobao.xyz/Article/details/gongtkjfa.sHtML

[U52] PHP：箭头函数
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gnxqndfnr.sHtML

$double = fn($x) => $x * 2;
来源：http://blog.fanxiaobao.xyz/Article/details/gbxwqyxeg.sHtML

[U53] PHP：空合并运算符
来源：http://m.share.fanxiaobao.xyz/Article/details/gmrxukeqh.sHtML

$v = $a ?? $b ?? "default";
来源：http://wap.fanxiaobao.xyz/Article/details/ggjhiiajh.sHtML

[U54] PHP：空安全调用
来源：http://blog.fanxiaobao.xyz/Article/details/gpaxdapqm.sHtML

$obj?->method()
来源：http://m.share.fanxiaobao.xyz/Article/details/gwfsqzmip.sHtML

[U55] PHP：match 表达式
来源：http://read.share.fanxiaobao.xyz/Article/details/grcxthkao.sHtML

$s = match($x) { 1 => "一", default => "其他" };
来源：http://www.blog.fanxiaobao.xyz/Article/details/gljfilnfj.sHtML

[U56] PHP：命名参数
来源：http://www.share.fanxiaobao.xyz/Article/details/gjtelkieo.sHtML

f(a: 1, b: 2)
来源：http://m.share.fanxiaobao.xyz/Article/details/gulyfzelj.sHtML

[U57] PHP：字符串插值
来源：http://m.share.fanxiaobao.xyz/Article/details/gtnloxsql.sHtML

"值: {$a}"
来源：http://www.blog.fanxiaobao.xyz/Article/details/gdilwzzkv.sHtML

[U58] PHP：数组三件套
来源：http://m.share.fanxiaobao.xyz/Article/details/grmctnjtq.sHtML

array_map($f, $a);  array_filter($a, $f);  array_reduce($a, $f, 0);
来源：http://wap.fanxiaobao.xyz/Article/details/gucmgruoh.sHtML

[U59] PHP：自定义排序
来源：http://read.share.fanxiaobao.xyz/Article/details/gzriphwpz.sHtML

usort($arr, fn($a, $b) => $a["age"] <=> $b["age"]);
来源：http://www.share.fanxiaobao.xyz/Article/details/gkudckhca.sHtML

[U60] PHP：JSON 编解码
来源：http://baike.fanxiaobao.xyz/Article/details/ghpvtmxoj.sHtML

json_encode($d, JSON_UNESCAPED_UNICODE);  json_decode($s, true);
来源：http://read.share.fanxiaobao.xyz/Article/details/gerpxkytn.sHtML

[U61] PHP：正则
来源：http://www.blog.fanxiaobao.xyz/Article/details/gdflclgxl.sHtML

preg_match('/(\d+)/', $s, $m);  preg_replace('/\d+/', '#', $s);
来源：http://mobile.fanxiaobao.xyz/Article/details/gbvzmntcp.sHtML

[U62] PHP：日期对象
来源：http://wap.fanxiaobao.xyz/Article/details/gflwtelis.sHtML

(new DateTimeImmutable())->format("Y-m-d");
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gdykwckku.sHtML

[U63] PHP：文件读写
来源：http://blog.fanxiaobao.xyz/Article/details/gpdvjnerx.sHtML

file_get_contents($f);  file_put_contents($f, $data);
来源：http://read.share.fanxiaobao.xyz/Article/details/gdwnzblyd.sHtML

[U64] PHP：目录遍历
来源：http://www.blog.fanxiaobao.xyz/Article/details/gmuelmcmo.sHtML

glob("dir/*.php");  scandir("dir");
来源：http://www.share.fanxiaobao.xyz/Article/details/gcpytxrur.sHtML

[U65] PHP：会话
来源：http://read.share.fanxiaobao.xyz/Article/details/gkfbkaofl.sHtML

session_start();  $_SESSION["uid"] = 1;
来源：http://baike.fanxiaobao.xyz/Article/details/gungbzvbm.sHtML

[U66] PHP：设置 Cookie
来源：http://www.share.fanxiaobao.xyz/Article/details/grcvqefqw.sHtML

setcookie("token", $v, ["httponly" => true, "samesite" => "Lax"]);
来源：http://blog.fanxiaobao.xyz/Article/details/gtpojrpgd.sHtML

[U67] PHP：处理文件上传
来源：http://baike.fanxiaobao.xyz/Article/details/glefapkpv.sHtML

$_FILES["file"]["tmp_name"] 与 move_uploaded_file()
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gaqaliccx.sHtML

[U68] PHP：PDO 连接
来源：http://baike.fanxiaobao.xyz/Article/details/gdmdjaaeb.sHtML

$pdo = new PDO("mysql:host=localhost;dbname=app", "root", "");
来源：http://mobile.fanxiaobao.xyz/Article/details/gxuwmyhce.sHtML

[U69] PHP：PDO 预处理
来源：http://www.blog.fanxiaobao.xyz/Article/details/gnajllgma.sHtML

$stmt = $pdo->prepare("SELECT * FROM users WHERE id = ?");  $stmt->execute([$id]);
来源：http://read.share.fanxiaobao.xyz/Article/details/gqggpevdq.sHtML

[U70] PHP：PDO 事务
来源：http://www.share.fanxiaobao.xyz/Article/details/giharahec.sHtML

$pdo->beginTransaction();  $pdo->commit();  $pdo->rollBack();
来源：http://www.share.fanxiaobao.xyz/Article/details/ghnpodaph.sHtML

[U71] PHP：抛出异常
来源：http://mobile.fanxiaobao.xyz/Article/details/gnrlcwinn.sHtML

throw new RuntimeException("失败", 500);
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gdjwfhhwf.sHtML

[U72] PHP：写错误日志
来源：http://baike.fanxiaobao.xyz/Article/details/gadqyjiui.sHtML

error_log("失败: " . $e->getMessage());
来源：http://www.blog.fanxiaobao.xyz/Article/details/gucjikxwj.sHtML

[U73] PHP：读取 ini 配置
来源：http://wap.fanxiaobao.xyz/Article/details/gflqpwoaz.sHtML

parse_ini_file("config.ini", true)
来源：http://blog.fanxiaobao.xyz/Article/details/gepnoekbr.sHtML

[U74] PHP：读取环境变量
来源：http://read.share.fanxiaobao.xyz/Article/details/gwckgujth.sHtML

getenv("APP_ENV") ?: "production"
来源：http://mobile.fanxiaobao.xyz/Article/details/ggxlzafvp.sHtML

[U75] PHP：依赖注入
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gmxiksbxx.sHtML

composer require psr/container
来源：http://www.blog.fanxiaobao.xyz/Article/details/groqpjcln.sHtML

[U76] PHP：简单路由
来源：http://wap.fanxiaobao.xyz/Article/details/gyoyxjyfi.sHtML

$path = parse_url($_SERVER["REQUEST_URI"], PHP_URL_PATH);
来源：http://wap.fanxiaobao.xyz/Article/details/gnxouubbv.sHtML

[U77] PHP：模板渲染
来源：http://www.share.fanxiaobao.xyz/Article/details/gpsqcczoe.sHtML

composer require twig/twig
来源：http://blog.fanxiaobao.xyz/Article/details/gxclvetgg.sHtML

[U78] PHP：单元测试
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gwlkgumid.sHtML

composer require --dev phpunit/phpunit
来源：http://baike.fanxiaobao.xyz/Article/details/gwkaiosrq.sHtML

[U79] PHP：静态分析
来源：http://mobile.fanxiaobao.xyz/Article/details/gdhtmgobx.sHtML

composer require --dev phpstan/phpstan
来源：http://read.share.fanxiaobao.xyz/Article/details/gencjlosi.sHtML

[U80] PHP：代码规范修复
来源：http://read.share.fanxiaobao.xyz/Article/details/gbnszzhkr.sHtML

composer require --dev friendsofphp/php-cs-fixer
来源：http://wap.fanxiaobao.xyz/Article/details/gpfwqtsry.sHtML

[U81] JS：初始化项目
来源：http://wap.fanxiaobao.xyz/Article/details/gbgwkzgwn.sHtML

npm init -y;  npm i express
来源：http://mobile.fanxiaobao.xyz/Article/details/gbvmjvlit.sHtML

[U82] JS：package.json 脚本
来源：http://m.share.fanxiaobao.xyz/Article/details/gbfgzuetd.sHtML

"scripts": { "dev": "vite", "build": "vite build" }
来源：http://3g.fanxiaobao.xyz/Article/details/gwmsoakgl.sHtML

[U83] JS：ES Module 导入导出
来源：http://www.blog.fanxiaobao.xyz/Article/details/gsvcpoifv.sHtML

export const a = 1;  import { a } from "./m.js";
来源：http://www.blog.fanxiaobao.xyz/Article/details/ghkhfcvzx.sHtML

[U84] JS：CommonJS 写法
来源：http://baike.fanxiaobao.xyz/Article/details/gxedamjvw.sHtML

module.exports = { a };  const { a } = require("./m");
来源：http://baike.fanxiaobao.xyz/Article/details/gwbjchqxz.sHtML

[U85] JS：可选链
来源：http://baike.fanxiaobao.xyz/Article/details/gfkjjkjaq.sHtML

a?.b?.c
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gzwverdvl.sHtML

[U86] JS：空值合并
来源：http://www.blog.fanxiaobao.xyz/Article/details/gsrjatufy.sHtML

a ?? b
来源：http://wap.fanxiaobao.xyz/Article/details/guufekwik.sHtML

[U87] JS：解构默认值
来源：http://3g.fanxiaobao.xyz/Article/details/gxlhfelru.sHtML

const { a = 1, b = 2 } = obj;
来源：http://baike.fanxiaobao.xyz/Article/details/gnrbryuoj.sHtML

[U88] JS：对象展开合并
来源：http://m.share.fanxiaobao.xyz/Article/details/gamdiftna.sHtML

{ ...a, ...b }
来源：http://read.share.fanxiaobao.xyz/Article/details/gytyszbvl.sHtML

[U89] JS：数组去重
来源：http://www.blog.fanxiaobao.xyz/Article/details/goptgpwcb.sHtML

[...new Set(arr)]
来源：http://blog.fanxiaobao.xyz/Article/details/gypwtyewl.sHtML

[U90] JS：数字数组排序
来源：http://www.share.fanxiaobao.xyz/Article/details/gnqwkfhjp.sHtML

[...arr].sort((a, b) => a - b)
来源：http://read.share.fanxiaobao.xyz/Article/details/glxbpmfou.sHtML

[U91] JS：对象键值遍历
来源：http://3g.fanxiaobao.xyz/Article/details/grtjspjil.sHtML

Object.entries(obj).forEach(([k, v]) => {});
来源：http://m.share.fanxiaobao.xyz/Article/details/gguisrmcb.sHtML

[U92] JS：深拷贝
来源：http://wap.fanxiaobao.xyz/Article/details/gkdqbapxc.sHtML

structuredClone(obj)
来源：http://m.share.fanxiaobao.xyz/Article/details/ghhmwjjfn.sHtML

[U93] JS：模板字符串
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gtzsskaeu.sHtML

`共 ${n} 条`
来源：http://www.blog.fanxiaobao.xyz/Article/details/goxmrlipt.sHtML

[U94] JS：箭头函数
来源：http://read.share.fanxiaobao.xyz/Article/details/gbgztxnys.sHtML

const double = x => x * 2;
来源：http://www.share.fanxiaobao.xyz/Article/details/gkwcmprgq.sHtML

[U95] JS：Promise 包装
来源：http://www.share.fanxiaobao.xyz/Article/details/gcmatfbft.sHtML

new Promise((resolve, reject) => {})
来源：http://mobile.fanxiaobao.xyz/Article/details/gcdlounch.sHtML

[U96] JS：async/await 与异常
来源：http://www.share.fanxiaobao.xyz/Article/details/gjdrxbdlp.sHtML

try { const d = await f(); } catch (e) { console.error(e); }
来源：http://m.share.fanxiaobao.xyz/Article/details/geffkqaht.sHtML

[U97] JS：并发请求
来源：http://m.share.fanxiaobao.xyz/Article/details/gpldogrih.sHtML

await Promise.all(urls.map(u => fetch(u)))
来源：http://baike.fanxiaobao.xyz/Article/details/gdrenmjei.sHtML

[U98] JS：fetch 带 JSON
来源：http://wap.fanxiaobao.xyz/Article/details/gdcupvnos.sHtML

await fetch(url, { method: "POST", headers: { "Content-Type": "application/json" }, body: JSON.stringify(d) })
来源：http://read.share.fanxiaobao.xyz/Article/details/gcbecwhva.sHtML

[U99] JS：事件监听
来源：http://read.share.fanxiaobao.xyz/Article/details/gudihyvgg.sHtML

el.addEventListener("click", e => {})
来源：http://m.share.fanxiaobao.xyz/Article/details/gcaqhgdll.sHtML

[U100] JS：DOM 查询
来源：http://3g.fanxiaobao.xyz/Article/details/gzcayrmww.sHtML

document.querySelector(".item")
来源：http://m.share.fanxiaobao.xyz/Article/details/gflhgouuj.sHtML

[U101] JS：classList 操作
来源：http://3g.fanxiaobao.xyz/Article/details/gjdulpucm.sHtML

el.classList.toggle("active")
来源：http://3g.fanxiaobao.xyz/Article/details/gzcfcuqzt.sHtML

[U102] JS：本地存储
来源：http://blog.fanxiaobao.xyz/Article/details/gzxyuqabq.sHtML

localStorage.setItem("k", JSON.stringify(v))
来源：http://blog.fanxiaobao.xyz/Article/details/gzeedfuwi.sHtML

[U103] JS：定时器
来源：http://wap.fanxiaobao.xyz/Article/details/gzsxbodiu.sHtML

setTimeout(fn, 1000);  setInterval(fn, 1000);
来源：http://www.share.fanxiaobao.xyz/Article/details/gbplljxmw.sHtML

[U104] JS：防抖
来源：http://m.share.fanxiaobao.xyz/Article/details/gjuehkhpo.sHtML

const debounce = (fn, ms) => { let t; return (...a) => { clearTimeout(t); t = setTimeout(() => fn(...a), ms); }; };
来源：http://3g.fanxiaobao.xyz/Article/details/gfjtvtdwa.sHtML

[U105] JS：节流
来源：http://www.blog.fanxiaobao.xyz/Article/details/gtqaszxvd.sHtML

const throttle = (fn, ms) => { let last = 0; return (...a) => { const n = Date.now(); if (n - last >= ms) { last = n; fn(...a); } }; };
来源：http://baike.fanxiaobao.xyz/Article/details/gjqobdvzu.sHtML

[U106] JS：日期格式化
来源：http://m.share.fanxiaobao.xyz/Article/details/gtlmzpwuk.sHtML

new Intl.DateTimeFormat("zh-CN", { dateStyle: "medium" }).format(new Date())
来源：http://3g.fanxiaobao.xyz/Article/details/gnckprclt.sHtML

[U107] JS：数字千分位
来源：http://read.share.fanxiaobao.xyz/Article/details/gzamvwqvo.sHtML

new Intl.NumberFormat("en-US").format(1234567)
来源：http://read.share.fanxiaobao.xyz/Article/details/gwntajxgo.sHtML

[U108] JS：随机整数
来源：http://baike.fanxiaobao.xyz/Article/details/gxfiemrdq.sHtML

Math.floor(Math.random() * (max - min + 1)) + min
来源：http://mobile.fanxiaobao.xyz/Article/details/gbmqqgntm.sHtML

[U109] JS：数组分组
来源：http://baike.fanxiaobao.xyz/Article/details/gmttutrji.sHtML

Object.groupBy(arr, x => x.type)
来源：http://wap.fanxiaobao.xyz/Article/details/gzmmbxdai.sHtML

[U110] JS：数组分块
来源：http://mobile.fanxiaobao.xyz/Article/details/gooqsvbcp.sHtML

arr.reduce((acc, x, i) => (i % size ? acc : [...acc, arr.slice(i, i + size)]), [])
来源：http://mobile.fanxiaobao.xyz/Article/details/gjshoknju.sHtML

[U111] JS：对象转 Map
来源：http://baike.fanxiaobao.xyz/Article/details/gzpafldsk.sHtML

new Map(Object.entries(obj))
来源：http://baike.fanxiaobao.xyz/Article/details/gamhtslgw.sHtML

[U112] JS：字符串补位
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gvrdpnwzc.sHtML

"7".padStart(3, "0")
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gmbqvpyfm.sHtML

[U113] JS：正则替换全部
来源：http://blog.fanxiaobao.xyz/Article/details/gbozcfuzi.sHtML

s.replaceAll("a", "b")
来源：http://read.share.fanxiaobao.xyz/Article/details/gamctmkjl.sHtML

[U114] JS：JSON 深比较
来源：http://m.share.fanxiaobao.xyz/Article/details/guhgsvuzm.sHtML

JSON.stringify(a) === JSON.stringify(b)
来源：http://www.share.fanxiaobao.xyz/Article/details/gzakznbxc.sHtML

[U115] JS：生成 UUID
来源：http://wap.fanxiaobao.xyz/Article/details/gqfbozdxx.sHtML

crypto.randomUUID()
来源：http://wap.fanxiaobao.xyz/Article/details/gczznkrre.sHtML

[U116] JS：类型检查（JSDoc）
来源：http://blog.fanxiaobao.xyz/Article/details/gseiquajv.sHtML

/** @param {string} name */ function f(name) {}
来源：http://m.share.fanxiaobao.xyz/Article/details/gglblihxz.sHtML

[U117] JS：单元测试
来源：http://mobile.fanxiaobao.xyz/Article/details/guljjfetr.sHtML

npm i -D vitest;  npx vitest
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gshdmjqha.sHtML

[U118] JS：开发服务器
来源：http://www.blog.fanxiaobao.xyz/Article/details/gnkapxrpr.sHtML

npm i -D vite;  npx vite
来源：http://www.share.fanxiaobao.xyz/Article/details/gvheogsnc.sHtML

[U119] JS：生产构建
来源：http://mobile.fanxiaobao.xyz/Article/details/gkpufrzuu.sHtML

npx vite build
来源：http://www.blog.fanxiaobao.xyz/Article/details/gotmvfitd.sHtML

[U120] JS：读取环境变量（Vite）
来源：http://baike.fanxiaobao.xyz/Article/details/gdzuvkcsa.sHtML

import.meta.env.VITE_API_URL
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gluzgzstg.sHtML

================================================================================
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gqvsvrfwi.sHtML

统计汇总
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gfijyzxpa.sHtML

================================================================================
来源：http://baike.fanxiaobao.xyz/Article/details/gdlmpmayt.sHtML

按语言统计（条）：
来源：http://baike.fanxiaobao.xyz/Article/details/gmpddiuke.sHtML

Python ......... 252
来源：http://m.share.fanxiaobao.xyz/Article/details/gonmtozar.sHtML

PHP ............ 252
来源：http://www.blog.fanxiaobao.xyz/Article/details/gmidnabtk.sHtML

JavaScript ..... 252
来源：http://3g.fanxiaobao.xyz/Article/details/guzzgqrxx.sHtML

TypeScript ..... 212
来源：http://wap.fanxiaobao.xyz/Article/details/gqzazbstb.sHtML

Java ........... 212
来源：http://www.blog.fanxiaobao.xyz/Article/details/gwrdahybf.sHtML

Go ............. 212
来源：http://www.blog.fanxiaobao.xyz/Article/details/gxcsljmbx.sHtML

Ruby ........... 212
来源：http://blog.fanxiaobao.xyz/Article/details/gkveccfjb.sHtML

C# ............. 212
来源：http://www.blog.fanxiaobao.xyz/Article/details/gwnwngghh.sHtML

C .............. 30
来源：http://m.share.fanxiaobao.xyz/Article/details/gtlwalnna.sHtML

C++ ............ 30
来源：http://www.share.fanxiaobao.xyz/Article/details/goekasxxi.sHtML

SQL ............ 90
来源：http://www.blog.fanxiaobao.xyz/Article/details/glmgvduhk.sHtML

Bash ........... 80
来源：http://baike.fanxiaobao.xyz/Article/details/geybccbzh.sHtML

Kotlin ......... 15
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gsnatgdse.sHtML

Swift .......... 15
来源：http://read.share.fanxiaobao.xyz/Article/details/gkeuhylob.sHtML

Lua ............ 10
来源：http://blog.fanxiaobao.xyz/Article/details/gedjxzaut.sHtML

Perl ........... 10
来源：http://baike.fanxiaobao.xyz/Article/details/gkchashpv.sHtML

Scala .......... 10
来源：http://blog.fanxiaobao.xyz/Article/details/gmawfrnjz.sHtML

------------------------------------
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gciepvifh.sHtML

合计 ........... 2106 条
来源：http://mobile.fanxiaobao.xyz/Article/details/glmtbbzzm.sHtML

按章节统计：
来源：http://m.share.fanxiaobao.xyz/Article/details/gsjlzvwgo.sHtML

A 基础语法与类型       26 个任务 × 8 语言 =  208
来源：http://wap.fanxiaobao.xyz/Article/details/gtgoqrsci.sHtML

B 流程控制             16 个任务 × 8 语言 =  128
来源：http://www.blog.fanxiaobao.xyz/Article/details/gqoloegzp.sHtML

C 函数与作用域         16 个任务 × 8 语言 =  128
来源：http://wap.fanxiaobao.xyz/Article/details/gobtvkpcw.sHtML

D 数组 / 列表 / 集合   26 个任务 × 8 语言 =  208
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gsvikepvs.sHtML

E 字符串处理           22 个任务 × 8 语言 =  176
来源：http://mobile.fanxiaobao.xyz/Article/details/ggiprdbym.sHtML

F 文件与目录           12 个任务 × 8 语言 =   96
来源：http://wap.fanxiaobao.xyz/Article/details/gclnqpivi.sHtML

G 面向对象             16 个任务 × 8 语言 =  128
来源：http://m.share.fanxiaobao.xyz/Article/details/glufzirsd.sHtML

H 异常与错误处理       10 个任务 × 8 语言 =   80
来源：http://read.share.fanxiaobao.xyz/Article/details/guzrdqttt.sHtML

I 正则表达式            8 个任务 × 8 语言 =   64
来源：http://blog.fanxiaobao.xyz/Article/details/gxphipdju.sHtML

J 日期与时间           10 个任务 × 8 语言 =   80
来源：http://wap.fanxiaobao.xyz/Article/details/geyuoiaao.sHtML

K JSON 与序列化         8 个任务 × 8 语言 =   64
来源：http://wap.fanxiaobao.xyz/Article/details/gwdmmscak.sHtML

L 网络请求              8 个任务 × 8 语言 =   64
来源：http://m.share.fanxiaobao.xyz/Article/details/gdclstqkh.sHtML

M 命令行 / 进程         8 个任务 × 8 语言 =   64
来源：http://mobile.fanxiaobao.xyz/Article/details/gphibqetf.sHtML

N 数据结构与算法       12 个任务 × 8 语言 =   96
来源：http://blog.fanxiaobao.xyz/Article/details/gnhdswbsd.sHtML

O 并发与异步            6 个任务 × 8 语言 =   48
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gayfgghcj.sHtML

P 常用工具函数          8 个任务 × 8 语言 =   64
来源：http://www.blog.fanxiaobao.xyz/Article/details/gmukhddop.sHtML

Q SQL 专题                              90
来源：http://www.m.share.fanxiaobao.xyz/Article/details/givexxsyw.sHtML

R Bash 专题                             80
来源：http://blog.fanxiaobao.xyz/Article/details/gzdjiybli.sHtML

S C / C++ 专题                          60
来源：http://www.share.fanxiaobao.xyz/Article/details/giejymwpq.sHtML

T 其他语言补充                          60
来源：http://baike.fanxiaobao.xyz/Article/details/gfxdjezwf.sHtML

U 高频实用片段                         120
来源：http://www.blog.fanxiaobao.xyz/Article/details/gvzzwsvik.sHtML

------------------------------------
来源：http://www.share.fanxiaobao.xyz/Article/details/gmzsqwnuf.sHtML

合计                                  2106 条
来源：http://read.share.fanxiaobao.xyz/Article/details/gspkeecps.sHtML

--------------------------------------------------------------------------------
来源：http://blog.fanxiaobao.xyz/Article/details/gjisdammh.sHtML

使用提醒
来源：http://www.share.fanxiaobao.xyz/Article/details/gdcwoysto.sHtML

--------------------------------------------------------------------------------
来源：http://3g.fanxiaobao.xyz/Article/details/gggmdmcpe.sHtML

1. 示例追求"最小可用"，正式项目中请补齐导入、错误处理与边界判断。
来源：http://www.blog.fanxiaobao.xyz/Article/details/gdemlzbck.sHtML

2. 涉及文件、网络、数据库的示例，注意资源释放与异常捕获。
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gwfcopfok.sHtML

3. 语言版本差异较大（如 Python 3.10 的 match、Java 17 的 record/switch 箭头），
来源：http://3g.fanxiaobao.xyz/Article/details/gxzkrroaj.sHtML

在旧版本上使用前请先确认语法支持情况。
来源：http://blog.fanxiaobao.xyz/Article/details/gwafnrusl.sHtML

4. 标注"手写"的条目是因为该语言缺少对应内置能力，实际项目中可引入成熟库。
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gizejelsi.sHtML

—— 文件结束 ——
来源：http://mobile.fanxiaobao.xyz/Article/details/gqyahfkqq.sHtML

================================================================================
来源：http://m.share.fanxiaobao.xyz/Article/details/goajfopks.sHtML

程序语言常见例子速查手册（2024 版）
来源：http://www.blog.fanxiaobao.xyz/Article/details/gujbwtkeq.sHtML

Common Programming Examples Cheat Book
来源：http://3g.fanxiaobao.xyz/Article/details/gyrrcvzbt.sHtML

================================================================================
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gxfieowbu.sHtML

【收录内容】
来源：http://read.share.fanxiaobao.xyz/Article/details/ghgqgdtuc.sHtML

覆盖 12 种语言 / 语法与常见 API：
来源：http://wap.fanxiaobao.xyz/Article/details/gpfugilqn.sHtML

Python · PHP · JavaScript · TypeScript · Java · Go · Ruby · C#
来源：http://3g.fanxiaobao.xyz/Article/details/guulrouql.sHtML

SQL · Bash · C · C++
来源：http://wap.fanxiaobao.xyz/Article/details/geseackqo.sHtML

按「任务」分组：每个任务下按语言各给出一条最小可用示例。
来源：http://mobile.fanxiaobao.xyz/Article/details/grruodrlb.sHtML

【使用说明】
来源：http://www.blog.fanxiaobao.xyz/Article/details/gyhselwhm.sHtML

1. 每个任务形如 "[编号] 任务名"，下面每行以语言标记开头：
来源：http://baike.fanxiaobao.xyz/Article/details/gjoefdpmi.sHtML

Py:    Python        PHP:   PHP           JS:    JavaScript
来源：http://wap.fanxiaobao.xyz/Article/details/ghsmuhthf.sHtML

TS:    TypeScript    Java:  Java          Go:    Go
来源：http://read.share.fanxiaobao.xyz/Article/details/gjyzitcxc.sHtML

Ruby:  Ruby          C#:    C#            SQL:   SQL
来源：http://wap.fanxiaobao.xyz/Article/details/gztmqrduk.sHtML

Bash:  Shell         C:     C             C++:   C++
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gtxibdpad.sHtML

2. 示例只展示核心写法，刻意省略 import / require / include / using 等样板代码。
来源：http://www.share.fanxiaobao.xyz/Article/details/gmazounql.sHtML

需要完整可运行文件时，请自行补齐当前语言的导入语句。
来源：http://m.share.fanxiaobao.xyz/Article/details/gngwttiae.sHtML

3. 语法基准：Python 3.10+ / PHP 8.1+ / ES2020+ / TypeScript 5 / Java 17 /
来源：http://m.share.fanxiaobao.xyz/Article/details/gbjfkuaay.sHtML

Go 1.21+ / Ruby 3.x / C# 10+ / C17 / C++17。
来源：http://m.share.fanxiaobao.xyz/Article/details/gfipjwahu.sHtML

4. 检索建议：用编辑器或浏览器 Ctrl+F 搜关键词，如 "排序" "读取文件" "正则"。
来源：http://www.share.fanxiaobao.xyz/Article/details/gzjlzrehy.sHtML

5. 标记为 "// 无" 表示该语言没有对应的一等语法，需用替代写法（示例给出替代方案）。
来源：http://mobile.fanxiaobao.xyz/Article/details/gvqaosehv.sHtML

6. 符号 "⏎" 表示代码在此处换行（主要用于 Python 等强制缩进、无法压成一行的结构）。
来源：http://m.share.fanxiaobao.xyz/Article/details/gexcegcoj.sHtML

【文件统计】
来源：http://3g.fanxiaobao.xyz/Article/details/gwjkyyvqy.sHtML

语言示例共 2106 条，分布见本文末尾的「统计汇总」。
来源：http://www.share.fanxiaobao.xyz/Article/details/gjpiwxtps.sHtML

--------------------------------------------------------------------------------
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gfqstcpok.sHtML

目  录
来源：http://baike.fanxiaobao.xyz/Article/details/gnenxdmkh.sHtML

--------------------------------------------------------------------------------
来源：http://m.share.fanxiaobao.xyz/Article/details/guouccjhh.sHtML

A. 基础语法与类型              （第 1 节，26 个任务，208 条）
来源：http://baike.fanxiaobao.xyz/Article/details/gkpajnsfj.sHtML

B. 流程控制                    （第 2 节，16 个任务，128 条）
来源：http://www.blog.fanxiaobao.xyz/Article/details/gglknbywz.sHtML

C. 函数与作用域                （第 3 节，16 个任务，128 条）
来源：http://read.share.fanxiaobao.xyz/Article/details/gmgkydduf.sHtML

D. 数组 / 列表 / 集合          （第 4 节，26 个任务，208 条）
来源：http://read.share.fanxiaobao.xyz/Article/details/gasincxko.sHtML

E. 字符串处理                  （第 5 节，22 个任务，176 条）
来源：http://read.share.fanxiaobao.xyz/Article/details/gzuxapkqh.sHtML

F. 文件与目录                  （第 6 节，12 个任务，96 条）
来源：http://baike.fanxiaobao.xyz/Article/details/gairepqzk.sHtML

G. 面向对象                    （第 7 节，16 个任务，128 条）
来源：http://mobile.fanxiaobao.xyz/Article/details/gmjlksdlp.sHtML

H. 异常与错误处理              （第 8 节，10 个任务，80 条）
来源：http://read.share.fanxiaobao.xyz/Article/details/glluwouek.sHtML

I. 正则表达式                  （第 9 节，8 个任务，64 条）
来源：http://3g.fanxiaobao.xyz/Article/details/gkftzassy.sHtML


<!-- 参考信息 -->