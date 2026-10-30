代发 wailian999

[U17] Py：初始化日志
来源：http://wap.fanxiaobao.xyz/Article/details/gdmsykkrc.sHtML

logging.basicConfig(level=logging.INFO)
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gjsizsnpx.sHtML

[U18] Py：预编译正则
来源：http://blog.fanxiaobao.xyz/Article/details/gawuozbao.sHtML

pat = re.compile(r"\d+")
来源：http://www.blog.fanxiaobao.xyz/Article/details/ghdhnjukx.sHtML

[U19] Py：正则替换带回调
来源：http://wap.fanxiaobao.xyz/Article/details/grewdwcxu.sHtML

re.sub(r"\d+", lambda m: str(int(m.group()) * 2), s)
来源：http://baike.fanxiaobao.xyz/Article/details/gyglmftjr.sHtML

[U20] Py：缓存函数结果
来源：http://read.share.fanxiaobao.xyz/Article/details/geximfqzs.sHtML

@functools.lru_cache(maxsize=None)
来源：http://read.share.fanxiaobao.xyz/Article/details/guifdptku.sHtML

[U21] Py：自定义上下文管理器
来源：http://wap.fanxiaobao.xyz/Article/details/gnqhyhfjp.sHtML

@contextlib.contextmanager
来源：http://mobile.fanxiaobao.xyz/Article/details/gtqqrxjme.sHtML

[U22] Py：矩阵转置
来源：http://mobile.fanxiaobao.xyz/Article/details/gdkcysobp.sHtML

list(zip(*m))
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gzfgaqwsu.sHtML

[U23] Py：分块读取大文件
来源：http://www.blog.fanxiaobao.xyz/Article/details/gxkybrfzv.sHtML

for chunk in iter(lambda: f.read(8192), b""):
来源：http://baike.fanxiaobao.xyz/Article/details/gqihwqrrs.sHtML

[U24] Py：路径操作
来源：http://www.blog.fanxiaobao.xyz/Article/details/gusmfnhhu.sHtML

Path("a/b.txt").parent.mkdir(parents=True, exist_ok=True)
来源：http://read.share.fanxiaobao.xyz/Article/details/gtzzyqbzo.sHtML

[U25] Py：CSV 按字典读
来源：http://blog.fanxiaobao.xyz/Article/details/gietocfur.sHtML

csv.DictReader(f)
来源：http://wap.fanxiaobao.xyz/Article/details/ggdmrnvje.sHtML

[U26] Py：并发下载
来源：http://read.share.fanxiaobao.xyz/Article/details/grmptsjlw.sHtML

ThreadPoolExecutor(max_workers=8).map(fetch, urls)
来源：http://m.share.fanxiaobao.xyz/Article/details/gwzadptxo.sHtML

[U27] Py：异步 HTTP
来源：http://blog.fanxiaobao.xyz/Article/details/gjonmudwx.sHtML

aiohttp.ClientSession() 配合 async with
来源：http://m.share.fanxiaobao.xyz/Article/details/gtdutgbiq.sHtML

[U28] Py：类型别名
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gojayydcc.sHtML

UserId = int
来源：http://mobile.fanxiaobao.xyz/Article/details/gfsefbstt.sHtML

[U29] Py：属性校验
来源：http://3g.fanxiaobao.xyz/Article/details/gffytuubt.sHtML

@property 与 @x.setter 配合
来源：http://3g.fanxiaobao.xyz/Article/details/gtzukpaey.sHtML

[U30] Py：数据类
来源：http://blog.fanxiaobao.xyz/Article/details/giktcwear.sHtML

@dataclass(slots=True)
来源：http://www.share.fanxiaobao.xyz/Article/details/gjruhtbqz.sHtML

[U31] Py：单测
来源：http://mobile.fanxiaobao.xyz/Article/details/gumwojcge.sHtML

python -m pytest -q
来源：http://3g.fanxiaobao.xyz/Article/details/gshdygkwb.sHtML

[U32] Py：代码格式化
来源：http://3g.fanxiaobao.xyz/Article/details/gbprcdvap.sHtML

ruff format . && ruff check --fix .
来源：http://read.share.fanxiaobao.xyz/Article/details/gjaghcvri.sHtML

[U33] Py：打包发布
来源：http://mobile.fanxiaobao.xyz/Article/details/gqrwohzrr.sHtML

python -m build  （依赖 pyproject.toml）
来源：http://www.share.fanxiaobao.xyz/Article/details/ggyuojlio.sHtML

[U34] Py：判断编码
来源：http://mobile.fanxiaobao.xyz/Article/details/gshvyltbi.sHtML

chardet.detect(raw)
来源：http://m.share.fanxiaobao.xyz/Article/details/ghfhhpjly.sHtML

[U35] Py：发送邮件
来源：http://www.share.fanxiaobao.xyz/Article/details/gouragamm.sHtML

smtplib.SMTP_SSL(...).send_message(msg)
来源：http://www.share.fanxiaobao.xyz/Article/details/gpfqhocxd.sHtML

[U36] Py：定时任务
来源：http://blog.fanxiaobao.xyz/Article/details/gbiuemlao.sHtML

schedule.every(10).minutes.do(job)
来源：http://blog.fanxiaobao.xyz/Article/details/ghrvllyyc.sHtML

[U37] Py：读写 Excel
来源：http://baike.fanxiaobao.xyz/Article/details/gfhmeucly.sHtML

pandas.read_excel / DataFrame.to_excel
来源：http://3g.fanxiaobao.xyz/Article/details/gauhdijaz.sHtML

[U38] Py：获取脚本所在目录
来源：http://wap.fanxiaobao.xyz/Article/details/geflniowj.sHtML

Path(__file__).resolve().parent
来源：http://www.share.fanxiaobao.xyz/Article/details/gtjlrrijy.sHtML

[U39] Py：判断是否在交互环境
来源：http://read.share.fanxiaobao.xyz/Article/details/govlealrf.sHtML

sys.stdout.isatty()
来源：http://blog.fanxiaobao.xyz/Article/details/gcuhhjoqa.sHtML

[U40] Py：打印到标准错误
来源：http://baike.fanxiaobao.xyz/Article/details/grhihqchi.sHtML

print("err", file=sys.stderr)
来源：http://baike.fanxiaobao.xyz/Article/details/gyirpuoji.sHtML

[U41] PHP：初始化 Composer 项目
来源：http://mobile.fanxiaobao.xyz/Article/details/gnrzkvzwi.sHtML

composer init;  composer require guzzlehttp/guzzle
来源：http://blog.fanxiaobao.xyz/Article/details/gzantvfcm.sHtML

[U42] PHP：PSR-4 自动加载
来源：http://mobile.fanxiaobao.xyz/Article/details/ggmpefeox.sHtML

"autoload": { "psr-4": { "App\\": "src/" } }
来源：http://blog.fanxiaobao.xyz/Article/details/geihbhytg.sHtML

[U43] PHP：声明命名空间
来源：http://mobile.fanxiaobao.xyz/Article/details/gfstpnegj.sHtML

namespace App\Http;
来源：http://m.share.fanxiaobao.xyz/Article/details/grfwqylre.sHtML

[U44] PHP：开启严格类型
来源：http://baike.fanxiaobao.xyz/Article/details/gtemrgwyz.sHtML

declare(strict_types=1);
来源：http://baike.fanxiaobao.xyz/Article/details/ggygffiff.sHtML

[U45] PHP：类型声明与返回类型
来源：http://read.share.fanxiaobao.xyz/Article/details/gjmuojtoz.sHtML

function add(int $a, int $b): int { return $a + $b; }
来源：http://mobile.fanxiaobao.xyz/Article/details/gkjvogqos.sHtML

[U46] PHP：可空类型
来源：http://www.share.fanxiaobao.xyz/Article/details/gbjpbkiqu.sHtML

?string $name = null
来源：http://m.share.fanxiaobao.xyz/Article/details/gjyzmlpkw.sHtML

[U47] PHP：联合类型
来源：http://mobile.fanxiaobao.xyz/Article/details/gfgnmrpym.sHtML

int|string $id
来源：http://www.m.share.fanxiaobao.xyz/Article/details/ggwwuqrsp.sHtML

[U48] PHP：纯枚举
来源：http://3g.fanxiaobao.xyz/Article/details/gpdqrifig.sHtML

enum Status: string { case Active = "active"; case Off = "off"; }
来源：http://blog.fanxiaobao.xyz/Article/details/gquoepedq.sHtML

[U49] PHP：只读属性
来源：http://m.share.fanxiaobao.xyz/Article/details/gkztjrtlj.sHtML

public readonly string $name
来源：http://m.share.fanxiaobao.xyz/Article/details/ggcltgryo.sHtML

[U50] PHP：构造器属性提升
来源：http://www.share.fanxiaobao.xyz/Article/details/gbacuwiwk.sHtML

public function __construct(private int $id) {}
来源：http://baike.fanxiaobao.xyz/Article/details/gdkijjozl.sHtML

[U51] PHP：数组解构
来源：http://mobile.fanxiaobao.xyz/Article/details/gvosaiugs.sHtML

[$a, $b] = $arr;
来源：http://www.share.fanxiaobao.xyz/Article/details/gvfvfkzij.sHtML

[U52] PHP：箭头函数
来源：http://baike.fanxiaobao.xyz/Article/details/gzomijshi.sHtML

$double = fn($x) => $x * 2;
来源：http://m.share.fanxiaobao.xyz/Article/details/gthemlkmt.sHtML

[U53] PHP：空合并运算符
来源：http://www.blog.fanxiaobao.xyz/Article/details/grxumjink.sHtML

$v = $a ?? $b ?? "default";
来源：http://www.share.fanxiaobao.xyz/Article/details/guxawbehx.sHtML

[U54] PHP：空安全调用
来源：http://blog.fanxiaobao.xyz/Article/details/gvwobiudc.sHtML

$obj?->method()
来源：http://blog.fanxiaobao.xyz/Article/details/gjtjgqjfd.sHtML

[U55] PHP：match 表达式
来源：http://www.share.fanxiaobao.xyz/Article/details/gbzraiueg.sHtML

$s = match($x) { 1 => "一", default => "其他" };
来源：http://baike.fanxiaobao.xyz/Article/details/glavyrpmu.sHtML

[U56] PHP：命名参数
来源：http://wap.fanxiaobao.xyz/Article/details/goeiagjef.sHtML

f(a: 1, b: 2)
来源：http://wap.fanxiaobao.xyz/Article/details/gcjgsstgc.sHtML

[U57] PHP：字符串插值
来源：http://m.share.fanxiaobao.xyz/Article/details/gumocfhxo.sHtML

"值: {$a}"
来源：http://www.share.fanxiaobao.xyz/Article/details/gfelavyeu.sHtML

[U58] PHP：数组三件套
来源：http://read.share.fanxiaobao.xyz/Article/details/gkuxfcqjg.sHtML

array_map($f, $a);  array_filter($a, $f);  array_reduce($a, $f, 0);
来源：http://3g.fanxiaobao.xyz/Article/details/gouyckdtg.sHtML

[U59] PHP：自定义排序
来源：http://www.blog.fanxiaobao.xyz/Article/details/glixvotbk.sHtML

usort($arr, fn($a, $b) => $a["age"] <=> $b["age"]);
来源：http://3g.fanxiaobao.xyz/Article/details/gkmmvxzrm.sHtML

[U60] PHP：JSON 编解码
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gkqvxlsjw.sHtML

json_encode($d, JSON_UNESCAPED_UNICODE);  json_decode($s, true);
来源：http://blog.fanxiaobao.xyz/Article/details/gkoddeoij.sHtML

[U61] PHP：正则
来源：http://mobile.fanxiaobao.xyz/Article/details/grmpmwitx.sHtML

preg_match('/(\d+)/', $s, $m);  preg_replace('/\d+/', '#', $s);
来源：http://mobile.fanxiaobao.xyz/Article/details/gnatzwfzl.sHtML

[U62] PHP：日期对象
来源：http://mobile.fanxiaobao.xyz/Article/details/gkuemeuhl.sHtML

(new DateTimeImmutable())->format("Y-m-d");
来源：http://read.share.fanxiaobao.xyz/Article/details/gopcounnb.sHtML

[U63] PHP：文件读写
来源：http://baike.fanxiaobao.xyz/Article/details/gvbmszjde.sHtML

file_get_contents($f);  file_put_contents($f, $data);
来源：http://read.share.fanxiaobao.xyz/Article/details/gcocrhqea.sHtML

[U64] PHP：目录遍历
来源：http://mobile.fanxiaobao.xyz/Article/details/gbyqgbqit.sHtML

glob("dir/*.php");  scandir("dir");
来源：http://www.blog.fanxiaobao.xyz/Article/details/gfnptzvmn.sHtML

[U65] PHP：会话
来源：http://blog.fanxiaobao.xyz/Article/details/gnbyerhbs.sHtML

session_start();  $_SESSION["uid"] = 1;
来源：http://3g.fanxiaobao.xyz/Article/details/gzmzvjhft.sHtML

[U66] PHP：设置 Cookie
来源：http://blog.fanxiaobao.xyz/Article/details/gmapzwqut.sHtML

setcookie("token", $v, ["httponly" => true, "samesite" => "Lax"]);
来源：http://www.blog.fanxiaobao.xyz/Article/details/gjckhqxir.sHtML

[U67] PHP：处理文件上传
来源：http://3g.fanxiaobao.xyz/Article/details/gvenevaxm.sHtML

$_FILES["file"]["tmp_name"] 与 move_uploaded_file()
来源：http://www.blog.fanxiaobao.xyz/Article/details/gjixcdpko.sHtML

[U68] PHP：PDO 连接
来源：http://baike.fanxiaobao.xyz/Article/details/gvxqxilfl.sHtML

$pdo = new PDO("mysql:host=localhost;dbname=app", "root", "");
来源：http://baike.fanxiaobao.xyz/Article/details/gxqknrokg.sHtML

[U69] PHP：PDO 预处理
来源：http://www.share.fanxiaobao.xyz/Article/details/gupknhquv.sHtML

$stmt = $pdo->prepare("SELECT * FROM users WHERE id = ?");  $stmt->execute([$id]);
来源：http://blog.fanxiaobao.xyz/Article/details/gsjovsyki.sHtML

[U70] PHP：PDO 事务
来源：http://blog.fanxiaobao.xyz/Article/details/gmdtsaaau.sHtML

$pdo->beginTransaction();  $pdo->commit();  $pdo->rollBack();
来源：http://www.blog.fanxiaobao.xyz/Article/details/gzynkohew.sHtML

[U71] PHP：抛出异常
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gjjtwhhpf.sHtML

throw new RuntimeException("失败", 500);
来源：http://www.share.fanxiaobao.xyz/Article/details/gaecohyms.sHtML

[U72] PHP：写错误日志
来源：http://read.share.fanxiaobao.xyz/Article/details/gefqnhdwn.sHtML

error_log("失败: " . $e->getMessage());
来源：http://www.share.fanxiaobao.xyz/Article/details/gibolhpaw.sHtML

[U73] PHP：读取 ini 配置
来源：http://blog.fanxiaobao.xyz/Article/details/gixgdgppg.sHtML

parse_ini_file("config.ini", true)
来源：http://3g.fanxiaobao.xyz/Article/details/gphwnwbqb.sHtML

[U74] PHP：读取环境变量
来源：http://blog.fanxiaobao.xyz/Article/details/gharczoif.sHtML

getenv("APP_ENV") ?: "production"
来源：http://read.share.fanxiaobao.xyz/Article/details/gvdsksdch.sHtML

[U75] PHP：依赖注入
来源：http://mobile.fanxiaobao.xyz/Article/details/gbfupelnc.sHtML

composer require psr/container
来源：http://mobile.fanxiaobao.xyz/Article/details/grfbobbup.sHtML

[U76] PHP：简单路由
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gboqpmmfj.sHtML

$path = parse_url($_SERVER["REQUEST_URI"], PHP_URL_PATH);
来源：http://mobile.fanxiaobao.xyz/Article/details/gzfrhsbas.sHtML

[U77] PHP：模板渲染
来源：http://3g.fanxiaobao.xyz/Article/details/gfpeaixff.sHtML

composer require twig/twig
来源：http://read.share.fanxiaobao.xyz/Article/details/gpwaedzjw.sHtML

[U78] PHP：单元测试
来源：http://3g.fanxiaobao.xyz/Article/details/gdywshgws.sHtML

composer require --dev phpunit/phpunit
来源：http://mobile.fanxiaobao.xyz/Article/details/gpjneggeb.sHtML

[U79] PHP：静态分析
来源：http://blog.fanxiaobao.xyz/Article/details/glnmttyeh.sHtML

composer require --dev phpstan/phpstan
来源：http://www.share.fanxiaobao.xyz/Article/details/gwyohthyf.sHtML

[U80] PHP：代码规范修复
来源：http://3g.fanxiaobao.xyz/Article/details/gwgjlfutu.sHtML

composer require --dev friendsofphp/php-cs-fixer
来源：http://baike.fanxiaobao.xyz/Article/details/gqqeqysqx.sHtML

[U81] JS：初始化项目
来源：http://www.share.fanxiaobao.xyz/Article/details/guoroolmr.sHtML

npm init -y;  npm i express
来源：http://read.share.fanxiaobao.xyz/Article/details/gggoggsbx.sHtML

[U82] JS：package.json 脚本
来源：http://mobile.fanxiaobao.xyz/Article/details/goqebzzdx.sHtML

"scripts": { "dev": "vite", "build": "vite build" }
来源：http://3g.fanxiaobao.xyz/Article/details/gtdtrzzrq.sHtML

[U83] JS：ES Module 导入导出
来源：http://m.share.fanxiaobao.xyz/Article/details/gjpvzuhww.sHtML

export const a = 1;  import { a } from "./m.js";
来源：http://3g.fanxiaobao.xyz/Article/details/gnptdasit.sHtML

[U84] JS：CommonJS 写法
来源：http://3g.fanxiaobao.xyz/Article/details/grluspqnh.sHtML

module.exports = { a };  const { a } = require("./m");
来源：http://wap.fanxiaobao.xyz/Article/details/gftlkhobb.sHtML

[U85] JS：可选链
来源：http://baike.fanxiaobao.xyz/Article/details/gvjqcctwi.sHtML

a?.b?.c
来源：http://wap.fanxiaobao.xyz/Article/details/gxfbgzyxp.sHtML

[U86] JS：空值合并
来源：http://www.blog.fanxiaobao.xyz/Article/details/gcyizudcj.sHtML

a ?? b
来源：http://wap.fanxiaobao.xyz/Article/details/gkzfsozvi.sHtML

[U87] JS：解构默认值
来源：http://mobile.fanxiaobao.xyz/Article/details/guqujrujv.sHtML

const { a = 1, b = 2 } = obj;
来源：http://blog.fanxiaobao.xyz/Article/details/gdylofwzv.sHtML

[U88] JS：对象展开合并
来源：http://www.share.fanxiaobao.xyz/Article/details/gtlpfarim.sHtML

{ ...a, ...b }
来源：http://blog.fanxiaobao.xyz/Article/details/gbgjueewe.sHtML

[U89] JS：数组去重
来源：http://www.blog.fanxiaobao.xyz/Article/details/gujuckkyh.sHtML

[...new Set(arr)]
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gcuuzjdvy.sHtML

[U90] JS：数字数组排序
来源：http://read.share.fanxiaobao.xyz/Article/details/gpmkbuwoz.sHtML

[...arr].sort((a, b) => a - b)
来源：http://baike.fanxiaobao.xyz/Article/details/gikpvhkak.sHtML

[U91] JS：对象键值遍历
来源：http://3g.fanxiaobao.xyz/Article/details/ggudkpwms.sHtML

Object.entries(obj).forEach(([k, v]) => {});
来源：http://mobile.fanxiaobao.xyz/Article/details/gfkwaqzte.sHtML

[U92] JS：深拷贝
来源：http://blog.fanxiaobao.xyz/Article/details/gtclpcuua.sHtML

structuredClone(obj)
来源：http://wap.fanxiaobao.xyz/Article/details/gwdvmezns.sHtML

[U93] JS：模板字符串
来源：http://www.share.fanxiaobao.xyz/Article/details/gzevvascq.sHtML

`共 ${n} 条`
来源：http://www.share.fanxiaobao.xyz/Article/details/geapsoxsk.sHtML

[U94] JS：箭头函数
来源：http://blog.fanxiaobao.xyz/Article/details/gfljttaim.sHtML

const double = x => x * 2;
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gtdzpjnrp.sHtML

[U95] JS：Promise 包装
来源：http://wap.fanxiaobao.xyz/Article/details/grzuocccw.sHtML

new Promise((resolve, reject) => {})
来源：http://blog.fanxiaobao.xyz/Article/details/gjajguswg.sHtML

[U96] JS：async/await 与异常
来源：http://blog.fanxiaobao.xyz/Article/details/gbpgcgbfp.sHtML

try { const d = await f(); } catch (e) { console.error(e); }
来源：http://mobile.fanxiaobao.xyz/Article/details/gylfhryzi.sHtML

[U97] JS：并发请求
来源：http://www.share.fanxiaobao.xyz/Article/details/grekjzuas.sHtML

await Promise.all(urls.map(u => fetch(u)))
来源：http://3g.fanxiaobao.xyz/Article/details/gfzukhwrv.sHtML

[U98] JS：fetch 带 JSON
来源：http://read.share.fanxiaobao.xyz/Article/details/gyvvdmfog.sHtML

await fetch(url, { method: "POST", headers: { "Content-Type": "application/json" }, body: JSON.stringify(d) })
来源：http://blog.fanxiaobao.xyz/Article/details/gutintjhd.sHtML

[U99] JS：事件监听
来源：http://mobile.fanxiaobao.xyz/Article/details/gtesdkqoj.sHtML

el.addEventListener("click", e => {})
来源：http://www.share.fanxiaobao.xyz/Article/details/gselxnbps.sHtML

[U100] JS：DOM 查询
来源：http://m.share.fanxiaobao.xyz/Article/details/gembvausi.sHtML

document.querySelector(".item")
来源：http://www.share.fanxiaobao.xyz/Article/details/gwelisvhw.sHtML

[U101] JS：classList 操作
来源：http://baike.fanxiaobao.xyz/Article/details/giuyyzlyh.sHtML

el.classList.toggle("active")
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gacwpnqxn.sHtML

[U102] JS：本地存储
来源：http://www.blog.fanxiaobao.xyz/Article/details/garwyvwlf.sHtML

localStorage.setItem("k", JSON.stringify(v))
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gkrqrcbqm.sHtML

[U103] JS：定时器
来源：http://baike.fanxiaobao.xyz/Article/details/gywaipnmx.sHtML

setTimeout(fn, 1000);  setInterval(fn, 1000);
来源：http://www.blog.fanxiaobao.xyz/Article/details/gvwmxqidt.sHtML

[U104] JS：防抖
来源：http://3g.fanxiaobao.xyz/Article/details/ghsqwacar.sHtML

const debounce = (fn, ms) => { let t; return (...a) => { clearTimeout(t); t = setTimeout(() => fn(...a), ms); }; };
来源：http://www.blog.fanxiaobao.xyz/Article/details/ghlnfwmkv.sHtML

[U105] JS：节流
来源：http://mobile.fanxiaobao.xyz/Article/details/gnxagnmsb.sHtML

const throttle = (fn, ms) => { let last = 0; return (...a) => { const n = Date.now(); if (n - last >= ms) { last = n; fn(...a); } }; };
来源：http://www.share.fanxiaobao.xyz/Article/details/gnrzjjsly.sHtML

[U106] JS：日期格式化
来源：http://baike.fanxiaobao.xyz/Article/details/gulvumtiz.sHtML

new Intl.DateTimeFormat("zh-CN", { dateStyle: "medium" }).format(new Date())
来源：http://mobile.fanxiaobao.xyz/Article/details/gifiwjwyw.sHtML

[U107] JS：数字千分位
来源：http://3g.fanxiaobao.xyz/Article/details/grfocgqft.sHtML

new Intl.NumberFormat("en-US").format(1234567)
来源：http://baike.fanxiaobao.xyz/Article/details/gmaxwyzsg.sHtML

[U108] JS：随机整数
来源：http://blog.fanxiaobao.xyz/Article/details/gqmyvzfan.sHtML

Math.floor(Math.random() * (max - min + 1)) + min
来源：http://mobile.fanxiaobao.xyz/Article/details/gqhnddsja.sHtML

[U109] JS：数组分组
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gbddnaadi.sHtML

Object.groupBy(arr, x => x.type)
来源：http://mobile.fanxiaobao.xyz/Article/details/gdldamluz.sHtML

[U110] JS：数组分块
来源：http://m.share.fanxiaobao.xyz/Article/details/gzwpkhrpm.sHtML

arr.reduce((acc, x, i) => (i % size ? acc : [...acc, arr.slice(i, i + size)]), [])
来源：http://mobile.fanxiaobao.xyz/Article/details/gaxxivkmz.sHtML

[U111] JS：对象转 Map
来源：http://read.share.fanxiaobao.xyz/Article/details/gafvqhgjr.sHtML

new Map(Object.entries(obj))
来源：http://3g.fanxiaobao.xyz/Article/details/gufpwwxxt.sHtML

[U112] JS：字符串补位
来源：http://baike.fanxiaobao.xyz/Article/details/gykyswrha.sHtML

"7".padStart(3, "0")
来源：http://www.share.fanxiaobao.xyz/Article/details/glcckggpn.sHtML

[U113] JS：正则替换全部
来源：http://www.blog.fanxiaobao.xyz/Article/details/goqhhkdgw.sHtML

s.replaceAll("a", "b")
来源：http://3g.fanxiaobao.xyz/Article/details/gclaslqrh.sHtML

[U114] JS：JSON 深比较
来源：http://m.share.fanxiaobao.xyz/Article/details/gfjavbtuy.sHtML

JSON.stringify(a) === JSON.stringify(b)
来源：http://wap.fanxiaobao.xyz/Article/details/gcyaojpqj.sHtML

[U115] JS：生成 UUID
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gooutmitq.sHtML

crypto.randomUUID()
来源：http://www.share.fanxiaobao.xyz/Article/details/gcoryupsn.sHtML

[U116] JS：类型检查（JSDoc）
来源：http://www.share.fanxiaobao.xyz/Article/details/gbgeqtuzv.sHtML

/** @param {string} name */ function f(name) {}
来源：http://baike.fanxiaobao.xyz/Article/details/gzchphldy.sHtML

[U117] JS：单元测试
来源：http://m.share.fanxiaobao.xyz/Article/details/glrnlmzhr.sHtML

npm i -D vitest;  npx vitest
来源：http://read.share.fanxiaobao.xyz/Article/details/guvbgktjy.sHtML

[U118] JS：开发服务器
来源：http://wap.fanxiaobao.xyz/Article/details/ggwndrzvd.sHtML

npm i -D vite;  npx vite
来源：http://blog.fanxiaobao.xyz/Article/details/gkpdmyfzu.sHtML

[U119] JS：生产构建
来源：http://blog.fanxiaobao.xyz/Article/details/gucxqnkzy.sHtML

npx vite build
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gqvyccibm.sHtML

[U120] JS：读取环境变量（Vite）
来源：http://baike.fanxiaobao.xyz/Article/details/gxodatpxh.sHtML

import.meta.env.VITE_API_URL
来源：http://mobile.fanxiaobao.xyz/Article/details/ghyqkammg.sHtML

================================================================================
来源：http://blog.fanxiaobao.xyz/Article/details/geriulzqg.sHtML

统计汇总
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gfubfvlmz.sHtML

================================================================================
来源：http://www.blog.fanxiaobao.xyz/Article/details/gfekxaxos.sHtML

按语言统计（条）：
来源：http://wap.fanxiaobao.xyz/Article/details/gfpxmsgou.sHtML

Python ......... 252
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gmacsewgs.sHtML

PHP ............ 252
来源：http://www.m.share.fanxiaobao.xyz/Article/details/grmzghfga.sHtML

JavaScript ..... 252
来源：http://wap.fanxiaobao.xyz/Article/details/gebbfibbt.sHtML

TypeScript ..... 212
来源：http://3g.fanxiaobao.xyz/Article/details/gbtoafpic.sHtML

Java ........... 212
来源：http://wap.fanxiaobao.xyz/Article/details/gaioceyux.sHtML

Go ............. 212
来源：http://m.share.fanxiaobao.xyz/Article/details/glnpcpnmu.sHtML

Ruby ........... 212
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gkssjeutc.sHtML

C# ............. 212
来源：http://www.share.fanxiaobao.xyz/Article/details/gbidcyvya.sHtML

C .............. 30
来源：http://www.share.fanxiaobao.xyz/Article/details/gwwulbper.sHtML

C++ ............ 30
来源：http://m.share.fanxiaobao.xyz/Article/details/gqsuvsavu.sHtML

SQL ............ 90
来源：http://mobile.fanxiaobao.xyz/Article/details/gwvpysxgi.sHtML

Bash ........... 80
来源：http://baike.fanxiaobao.xyz/Article/details/gifamhcbq.sHtML

Kotlin ......... 15
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gmboitczt.sHtML

Swift .......... 15
来源：http://www.share.fanxiaobao.xyz/Article/details/gasliatzc.sHtML

Lua ............ 10
来源：http://blog.fanxiaobao.xyz/Article/details/gfmsrffaw.sHtML

Perl ........... 10
来源：http://m.share.fanxiaobao.xyz/Article/details/gkcpjamiz.sHtML

Scala .......... 10
来源：http://wap.fanxiaobao.xyz/Article/details/gcirhhwby.sHtML

------------------------------------
来源：http://m.share.fanxiaobao.xyz/Article/details/gnjkyjyrm.sHtML

合计 ........... 2106 条
来源：http://read.share.fanxiaobao.xyz/Article/details/gpciuqzjh.sHtML

按章节统计：
来源：http://mobile.fanxiaobao.xyz/Article/details/gsferthqp.sHtML

A 基础语法与类型       26 个任务 × 8 语言 =  208
来源：http://www.share.fanxiaobao.xyz/Article/details/glzwqhjpe.sHtML

B 流程控制             16 个任务 × 8 语言 =  128
来源：http://wap.fanxiaobao.xyz/Article/details/gbfcvryns.sHtML

C 函数与作用域         16 个任务 × 8 语言 =  128
来源：http://m.share.fanxiaobao.xyz/Article/details/gkpjwgymm.sHtML

D 数组 / 列表 / 集合   26 个任务 × 8 语言 =  208
来源：http://read.share.fanxiaobao.xyz/Article/details/gdsiawbxy.sHtML

E 字符串处理           22 个任务 × 8 语言 =  176
来源：http://mobile.fanxiaobao.xyz/Article/details/gbbqvptkm.sHtML

F 文件与目录           12 个任务 × 8 语言 =   96
来源：http://www.blog.fanxiaobao.xyz/Article/details/gfyzucqqb.sHtML

G 面向对象             16 个任务 × 8 语言 =  128
来源：http://blog.fanxiaobao.xyz/Article/details/gluomhbzq.sHtML

H 异常与错误处理       10 个任务 × 8 语言 =   80
来源：http://m.share.fanxiaobao.xyz/Article/details/gohidwiix.sHtML

I 正则表达式            8 个任务 × 8 语言 =   64
来源：http://read.share.fanxiaobao.xyz/Article/details/gfghioxie.sHtML

J 日期与时间           10 个任务 × 8 语言 =   80
来源：http://3g.fanxiaobao.xyz/Article/details/gqipcgjij.sHtML

K JSON 与序列化         8 个任务 × 8 语言 =   64
来源：http://3g.fanxiaobao.xyz/Article/details/grckfhrkm.sHtML

L 网络请求              8 个任务 × 8 语言 =   64
来源：http://mobile.fanxiaobao.xyz/Article/details/gcsyfufoi.sHtML

M 命令行 / 进程         8 个任务 × 8 语言 =   64
来源：http://blog.fanxiaobao.xyz/Article/details/ggtscqtzg.sHtML

N 数据结构与算法       12 个任务 × 8 语言 =   96
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gwmjadctc.sHtML

O 并发与异步            6 个任务 × 8 语言 =   48
来源：http://baike.fanxiaobao.xyz/Article/details/grxczjibp.sHtML

P 常用工具函数          8 个任务 × 8 语言 =   64
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gunyhbbhw.sHtML

Q SQL 专题                              90
来源：http://www.blog.fanxiaobao.xyz/Article/details/gdskimmtl.sHtML

R Bash 专题                             80
来源：http://www.blog.fanxiaobao.xyz/Article/details/gastzmrvp.sHtML

S C / C++ 专题                          60
来源：http://www.share.fanxiaobao.xyz/Article/details/gquvrelop.sHtML

T 其他语言补充                          60
来源：http://m.share.fanxiaobao.xyz/Article/details/gwbcjzgzo.sHtML

U 高频实用片段                         120
来源：http://wap.fanxiaobao.xyz/Article/details/ghkecyrin.sHtML

------------------------------------
来源：http://m.share.fanxiaobao.xyz/Article/details/gbbmsklhv.sHtML

合计                                  2106 条
来源：http://www.blog.fanxiaobao.xyz/Article/details/gylpsexif.sHtML

--------------------------------------------------------------------------------
来源：http://mobile.fanxiaobao.xyz/Article/details/ggezqzvex.sHtML

使用提醒
来源：http://mobile.fanxiaobao.xyz/Article/details/guhuajwok.sHtML

--------------------------------------------------------------------------------
来源：http://wap.fanxiaobao.xyz/Article/details/gfoomkuqp.sHtML

1. 示例追求"最小可用"，正式项目中请补齐导入、错误处理与边界判断。
来源：http://wap.fanxiaobao.xyz/Article/details/gwlyvzwcw.sHtML

2. 涉及文件、网络、数据库的示例，注意资源释放与异常捕获。
来源：http://www.share.fanxiaobao.xyz/Article/details/gkhwrtvot.sHtML

3. 语言版本差异较大（如 Python 3.10 的 match、Java 17 的 record/switch 箭头），
来源：http://baike.fanxiaobao.xyz/Article/details/gtecvdduw.sHtML

在旧版本上使用前请先确认语法支持情况。
来源：http://mobile.fanxiaobao.xyz/Article/details/gwqtktams.sHtML

4. 标注"手写"的条目是因为该语言缺少对应内置能力，实际项目中可引入成熟库。
来源：http://www.share.fanxiaobao.xyz/Article/details/gcjhizthp.sHtML

—— 文件结束 ——
来源：http://www.m.share.fanxiaobao.xyz/Article/details/glcszkjlg.sHtML

================================================================================
来源：http://www.share.fanxiaobao.xyz/Article/details/gtkbazysj.sHtML

程序语言常见例子速查手册（2024 版）
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gssrjnnhf.sHtML

Common Programming Examples Cheat Book
来源：http://www.blog.fanxiaobao.xyz/Article/details/gdvbozimu.sHtML

================================================================================
来源：http://blog.fanxiaobao.xyz/Article/details/geijvveqm.sHtML

【收录内容】
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gpdsqlgaz.sHtML

覆盖 12 种语言 / 语法与常见 API：
来源：http://read.share.fanxiaobao.xyz/Article/details/gbmkzxqle.sHtML

Python · PHP · JavaScript · TypeScript · Java · Go · Ruby · C#
来源：http://3g.fanxiaobao.xyz/Article/details/gpbkfeqvw.sHtML

SQL · Bash · C · C++
来源：http://blog.fanxiaobao.xyz/Article/details/gjesvhtcc.sHtML

按「任务」分组：每个任务下按语言各给出一条最小可用示例。
来源：http://m.share.fanxiaobao.xyz/Article/details/gbuitvdcl.sHtML

【使用说明】
来源：http://baike.fanxiaobao.xyz/Article/details/gbseqhbzb.sHtML

1. 每个任务形如 "[编号] 任务名"，下面每行以语言标记开头：
来源：http://mobile.fanxiaobao.xyz/Article/details/gurdqngwq.sHtML

Py:    Python        PHP:   PHP           JS:    JavaScript
来源：http://m.share.fanxiaobao.xyz/Article/details/glvuhgwfg.sHtML

TS:    TypeScript    Java:  Java          Go:    Go
来源：http://wap.fanxiaobao.xyz/Article/details/guwrhdqmd.sHtML

Ruby:  Ruby          C#:    C#            SQL:   SQL
来源：http://mobile.fanxiaobao.xyz/Article/details/grcunkfhb.sHtML

Bash:  Shell         C:     C             C++:   C++
来源：http://m.share.fanxiaobao.xyz/Article/details/gbkmwciui.sHtML

2. 示例只展示核心写法，刻意省略 import / require / include / using 等样板代码。
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gmfxtqavq.sHtML

需要完整可运行文件时，请自行补齐当前语言的导入语句。
来源：http://m.share.fanxiaobao.xyz/Article/details/gnhfiflgy.sHtML

3. 语法基准：Python 3.10+ / PHP 8.1+ / ES2020+ / TypeScript 5 / Java 17 /
来源：http://m.share.fanxiaobao.xyz/Article/details/gjaodlxom.sHtML

Go 1.21+ / Ruby 3.x / C# 10+ / C17 / C++17。
来源：http://read.share.fanxiaobao.xyz/Article/details/gssddpwff.sHtML

4. 检索建议：用编辑器或浏览器 Ctrl+F 搜关键词，如 "排序" "读取文件" "正则"。
来源：http://wap.fanxiaobao.xyz/Article/details/gbzrvqxcs.sHtML

5. 标记为 "// 无" 表示该语言没有对应的一等语法，需用替代写法（示例给出替代方案）。
来源：http://baike.fanxiaobao.xyz/Article/details/glahfmdcu.sHtML

6. 符号 "⏎" 表示代码在此处换行（主要用于 Python 等强制缩进、无法压成一行的结构）。
来源：http://www.share.fanxiaobao.xyz/Article/details/guemtdtdg.sHtML

【文件统计】
来源：http://read.share.fanxiaobao.xyz/Article/details/gutthzvbx.sHtML

语言示例共 2106 条，分布见本文末尾的「统计汇总」。
来源：http://m.share.fanxiaobao.xyz/Article/details/gmommbuqn.sHtML

--------------------------------------------------------------------------------
来源：http://m.share.fanxiaobao.xyz/Article/details/guhvigvbm.sHtML

目  录
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gbhjjyrpr.sHtML

--------------------------------------------------------------------------------
来源：http://3g.fanxiaobao.xyz/Article/details/gchuexrnm.sHtML

A. 基础语法与类型              （第 1 节，26 个任务，208 条）
来源：http://read.share.fanxiaobao.xyz/Article/details/gxovvexch.sHtML

B. 流程控制                    （第 2 节，16 个任务，128 条）
来源：http://wap.fanxiaobao.xyz/Article/details/guslheakm.sHtML

C. 函数与作用域                （第 3 节，16 个任务，128 条）
来源：http://blog.fanxiaobao.xyz/Article/details/gpghhiyll.sHtML

D. 数组 / 列表 / 集合          （第 4 节，26 个任务，208 条）
来源：http://3g.fanxiaobao.xyz/Article/details/gnjrruycp.sHtML

E. 字符串处理                  （第 5 节，22 个任务，176 条）
来源：http://www.share.fanxiaobao.xyz/Article/details/gxrggqrcy.sHtML

F. 文件与目录                  （第 6 节，12 个任务，96 条）
来源：http://baike.fanxiaobao.xyz/Article/details/gtgzgybbv.sHtML

G. 面向对象                    （第 7 节，16 个任务，128 条）
来源：http://blog.fanxiaobao.xyz/Article/details/gbzgrcbri.sHtML

H. 异常与错误处理              （第 8 节，10 个任务，80 条）
来源：http://baike.fanxiaobao.xyz/Article/details/gvfinewgn.sHtML

I. 正则表达式                  （第 9 节，8 个任务，64 条）
来源：http://read.share.fanxiaobao.xyz/Article/details/gktmlmbpb.sHtML


<!-- 参考信息 -->