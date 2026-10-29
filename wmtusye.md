代发 wailian999

[U15] Py：高精度计时
来源：http://www.blog.zdbjq.cn/Article/details/gwuffilpc.sHtML

t = time.perf_counter()
来源：http://m.share.hesvh.cn/Article/details/ggcwciwzq.sHtML

[U16] Py：命令行参数解析
来源：http://3g.hesvh.cn/Article/details/gqmjoguer.sHtML

ap = argparse.ArgumentParser();  ap.add_argument("--name");  args = ap.parse_args()
来源：http://www.m.share.hesvh.cn/Article/details/goinbaogw.sHtML

[U17] Py：初始化日志
来源：http://m.share.hesvh.cn/Article/details/gebzbnaxn.sHtML

logging.basicConfig(level=logging.INFO)
来源：http://m.share.fehbvm.com/Article/details/gyecwvuwf.sHtML

[U18] Py：预编译正则
来源：http://www.blog.hesvh.cn/Article/details/gqlvpzuct.sHtML

pat = re.compile(r"\d+")
来源：http://blog.hesvh.cn/Article/details/goaxdlrgj.sHtML

[U19] Py：正则替换带回调
来源：http://read.share.hesvh.cn/Article/details/gtqodsctf.sHtML

re.sub(r"\d+", lambda m: str(int(m.group()) * 2), s)
来源：http://read.share.fehbvm.com/Article/details/gybgujwyn.sHtML

[U20] Py：缓存函数结果
来源：http://blog.hesvh.cn/Article/details/gmwcjklvp.sHtML

@functools.lru_cache(maxsize=None)
来源：http://www.share.fehbvm.com/Article/details/grcubztom.sHtML

[U21] Py：自定义上下文管理器
来源：http://3g.fehbvm.com/Article/details/ggyrrzufq.sHtML

@contextlib.contextmanager
来源：http://blog.fehbvm.com/Article/details/geujpzjra.sHtML

[U22] Py：矩阵转置
来源：http://wap.hesvh.cn/Article/details/girfwfyqg.sHtML

list(zip(*m))
来源：http://mobile.fehbvm.com/Article/details/geydewuxc.sHtML

[U23] Py：分块读取大文件
来源：http://wap.hesvh.cn/Article/details/ghdvmcljh.sHtML

for chunk in iter(lambda: f.read(8192), b""):
来源：http://baike.fehbvm.com/Article/details/gsxgsmmrl.sHtML

[U24] Py：路径操作
来源：http://3g.fehbvm.com/Article/details/gcidzhjmi.sHtML

Path("a/b.txt").parent.mkdir(parents=True, exist_ok=True)
来源：http://wap.zdbjq.cn/Article/details/gnwkztykp.sHtML

[U25] Py：CSV 按字典读
来源：http://www.m.share.fehbvm.com/Article/details/gbomzukxu.sHtML

csv.DictReader(f)
来源：http://baike.fehbvm.com/Article/details/ggmywsbqb.sHtML

[U26] Py：并发下载
来源：http://mobile.hesvh.cn/Article/details/gnfaxlpyh.sHtML

ThreadPoolExecutor(max_workers=8).map(fetch, urls)
来源：http://www.m.share.zdbjq.cn/Article/details/gtukjbpyd.sHtML

[U27] Py：异步 HTTP
来源：http://baike.fehbvm.com/Article/details/gjyafpylr.sHtML

aiohttp.ClientSession() 配合 async with
来源：http://www.m.share.hesvh.cn/Article/details/ggtcjwxxq.sHtML

[U28] Py：类型别名
来源：http://3g.hesvh.cn/Article/details/gtwyycadl.sHtML

UserId = int
来源：http://baike.zdbjq.cn/Article/details/gmbgvufij.sHtML

[U29] Py：属性校验
来源：http://3g.zdbjq.cn/Article/details/gptjhnsuw.sHtML

@property 与 @x.setter 配合
来源：http://mobile.zdbjq.cn/Article/details/guckwomcw.sHtML

[U30] Py：数据类
来源：http://m.share.hesvh.cn/Article/details/gwtlqtsoz.sHtML

@dataclass(slots=True)
来源：http://www.blog.fehbvm.com/Article/details/guuxsxthq.sHtML

[U31] Py：单测
来源：http://mobile.zdbjq.cn/Article/details/gsxflnuji.sHtML

python -m pytest -q
来源：http://read.share.zdbjq.cn/Article/details/gmislqjel.sHtML

[U32] Py：代码格式化
来源：http://wap.zdbjq.cn/Article/details/gydfawgcm.sHtML

ruff format . && ruff check --fix .
来源：http://wap.hesvh.cn/Article/details/gfuvmxusn.sHtML

[U33] Py：打包发布
来源：http://mobile.fehbvm.com/Article/details/gqhhsodxk.sHtML

python -m build  （依赖 pyproject.toml）
来源：http://www.m.share.hesvh.cn/Article/details/gdveysjgz.sHtML

[U34] Py：判断编码
来源：http://www.blog.hesvh.cn/Article/details/gzwvdtubz.sHtML

chardet.detect(raw)
来源：http://m.share.hesvh.cn/Article/details/gwqvrghrc.sHtML

[U35] Py：发送邮件
来源：http://blog.zdbjq.cn/Article/details/gcjdgarhg.sHtML

smtplib.SMTP_SSL(...).send_message(msg)
来源：http://mobile.zdbjq.cn/Article/details/gnzltdwvc.sHtML

[U36] Py：定时任务
来源：http://www.blog.zdbjq.cn/Article/details/gjyrulrvz.sHtML

schedule.every(10).minutes.do(job)
来源：http://blog.zdbjq.cn/Article/details/grbkgygkx.sHtML

[U37] Py：读写 Excel
来源：http://mobile.zdbjq.cn/Article/details/girypcazc.sHtML

pandas.read_excel / DataFrame.to_excel
来源：http://www.blog.zdbjq.cn/Article/details/gfxojkwst.sHtML

[U38] Py：获取脚本所在目录
来源：http://m.share.fehbvm.com/Article/details/gvlhhsvby.sHtML

Path(__file__).resolve().parent
来源：http://www.share.zdbjq.cn/Article/details/gagyjbomh.sHtML

[U39] Py：判断是否在交互环境
来源：http://wap.zdbjq.cn/Article/details/gvdbjwlge.sHtML

sys.stdout.isatty()
来源：http://3g.fehbvm.com/Article/details/gqtvspfqz.sHtML

[U40] Py：打印到标准错误
来源：http://blog.fehbvm.com/Article/details/gqljnqhdt.sHtML

print("err", file=sys.stderr)
来源：http://blog.zdbjq.cn/Article/details/gcsnqjamm.sHtML

[U41] PHP：初始化 Composer 项目
来源：http://wap.zdbjq.cn/Article/details/gejrcrigy.sHtML

composer init;  composer require guzzlehttp/guzzle
来源：http://www.m.share.fehbvm.com/Article/details/ghascwrtj.sHtML

[U42] PHP：PSR-4 自动加载
来源：http://read.share.fehbvm.com/Article/details/gghppmlvm.sHtML

"autoload": { "psr-4": { "App\\": "src/" } }
来源：http://www.blog.hesvh.cn/Article/details/gpklvjhkz.sHtML

[U43] PHP：声明命名空间
来源：http://www.share.hesvh.cn/Article/details/gzsycupnl.sHtML

namespace App\Http;
来源：http://baike.zdbjq.cn/Article/details/gunonupul.sHtML

[U44] PHP：开启严格类型
来源：http://mobile.hesvh.cn/Article/details/gzlsmcqwa.sHtML

declare(strict_types=1);
来源：http://3g.hesvh.cn/Article/details/grvlhfvct.sHtML

[U45] PHP：类型声明与返回类型
来源：http://m.share.hesvh.cn/Article/details/glgvcyqcs.sHtML

function add(int $a, int $b): int { return $a + $b; }
来源：http://wap.fehbvm.com/Article/details/gqpyebkug.sHtML

[U46] PHP：可空类型
来源：http://baike.zdbjq.cn/Article/details/gzitqxzds.sHtML

?string $name = null
来源：http://read.share.hesvh.cn/Article/details/gkcdjusev.sHtML

[U47] PHP：联合类型
来源：http://www.blog.hesvh.cn/Article/details/gnuvhxdsc.sHtML

int|string $id
来源：http://baike.hesvh.cn/Article/details/ggzqbhtee.sHtML

[U48] PHP：纯枚举
来源：http://www.m.share.fehbvm.com/Article/details/gaxamgkjv.sHtML

enum Status: string { case Active = "active"; case Off = "off"; }
来源：http://3g.hesvh.cn/Article/details/gnqoclbky.sHtML

[U49] PHP：只读属性
来源：http://blog.hesvh.cn/Article/details/gybirseml.sHtML

public readonly string $name
来源：http://www.share.fehbvm.com/Article/details/gukrtcjzd.sHtML

[U50] PHP：构造器属性提升
来源：http://m.share.hesvh.cn/Article/details/gzfiwosjm.sHtML

public function __construct(private int $id) {}
来源：http://m.share.fehbvm.com/Article/details/gmpzvabnt.sHtML

[U51] PHP：数组解构
来源：http://mobile.fehbvm.com/Article/details/glfkipein.sHtML

[$a, $b] = $arr;
来源：http://baike.hesvh.cn/Article/details/gilaxaaee.sHtML

[U52] PHP：箭头函数
来源：http://read.share.fehbvm.com/Article/details/gcnuihjyt.sHtML

$double = fn($x) => $x * 2;
来源：http://m.share.zdbjq.cn/Article/details/gfhijgaek.sHtML

[U53] PHP：空合并运算符
来源：http://www.share.fehbvm.com/Article/details/gfngimlwx.sHtML

$v = $a ?? $b ?? "default";
来源：http://wap.hesvh.cn/Article/details/gasattjmb.sHtML

[U54] PHP：空安全调用
来源：http://blog.hesvh.cn/Article/details/gvsuwhsjk.sHtML

$obj?->method()
来源：http://www.share.fehbvm.com/Article/details/gsdfldedw.sHtML

[U55] PHP：match 表达式
来源：http://www.blog.fehbvm.com/Article/details/gykksybpl.sHtML

$s = match($x) { 1 => "一", default => "其他" };
来源：http://read.share.zdbjq.cn/Article/details/ghrunkvye.sHtML

[U56] PHP：命名参数
来源：http://www.share.hesvh.cn/Article/details/glrsqgmmp.sHtML

f(a: 1, b: 2)
来源：http://read.share.hesvh.cn/Article/details/gahykjpnm.sHtML

[U57] PHP：字符串插值
来源：http://m.share.hesvh.cn/Article/details/gtyknxqxv.sHtML

"值: {$a}"
来源：http://baike.hesvh.cn/Article/details/gwiojiaei.sHtML

[U58] PHP：数组三件套
来源：http://mobile.zdbjq.cn/Article/details/gfuucisyt.sHtML

array_map($f, $a);  array_filter($a, $f);  array_reduce($a, $f, 0);
来源：http://wap.fehbvm.com/Article/details/gnutexkez.sHtML

[U59] PHP：自定义排序
来源：http://read.share.fehbvm.com/Article/details/gaywjgfeo.sHtML

usort($arr, fn($a, $b) => $a["age"] <=> $b["age"]);
来源：http://blog.hesvh.cn/Article/details/gdayybgpt.sHtML

[U60] PHP：JSON 编解码
来源：http://mobile.hesvh.cn/Article/details/gifqnnlkz.sHtML

json_encode($d, JSON_UNESCAPED_UNICODE);  json_decode($s, true);
来源：http://wap.fehbvm.com/Article/details/gfvxqxrub.sHtML

[U61] PHP：正则
来源：http://www.blog.zdbjq.cn/Article/details/gkhdswhmz.sHtML

preg_match('/(\d+)/', $s, $m);  preg_replace('/\d+/', '#', $s);
来源：http://read.share.fehbvm.com/Article/details/gezyylkrf.sHtML

[U62] PHP：日期对象
来源：http://www.share.zdbjq.cn/Article/details/gvkrsmovf.sHtML

(new DateTimeImmutable())->format("Y-m-d");
来源：http://blog.zdbjq.cn/Article/details/gcdbdlbhv.sHtML

[U63] PHP：文件读写
来源：http://baike.zdbjq.cn/Article/details/gknreisas.sHtML

file_get_contents($f);  file_put_contents($f, $data);
来源：http://3g.hesvh.cn/Article/details/gwurauvna.sHtML

[U64] PHP：目录遍历
来源：http://mobile.fehbvm.com/Article/details/gxsgmrhtk.sHtML

glob("dir/*.php");  scandir("dir");
来源：http://www.m.share.fehbvm.com/Article/details/gbnwwoapw.sHtML

[U65] PHP：会话
来源：http://wap.hesvh.cn/Article/details/gywcdedqk.sHtML

session_start();  $_SESSION["uid"] = 1;
来源：http://3g.zdbjq.cn/Article/details/gcsordeve.sHtML

[U66] PHP：设置 Cookie
来源：http://m.share.zdbjq.cn/Article/details/geyzjainq.sHtML

setcookie("token", $v, ["httponly" => true, "samesite" => "Lax"]);
来源：http://baike.hesvh.cn/Article/details/gcedyhbdt.sHtML

[U67] PHP：处理文件上传
来源：http://read.share.fehbvm.com/Article/details/gszwycgxf.sHtML

$_FILES["file"]["tmp_name"] 与 move_uploaded_file()
来源：http://www.share.zdbjq.cn/Article/details/gfijumhkf.sHtML

[U68] PHP：PDO 连接
来源：http://mobile.hesvh.cn/Article/details/gwnltegxc.sHtML

$pdo = new PDO("mysql:host=localhost;dbname=app", "root", "");
来源：http://blog.fehbvm.com/Article/details/gqjzyyplf.sHtML

[U69] PHP：PDO 预处理
来源：http://blog.zdbjq.cn/Article/details/glztgrlpm.sHtML

$stmt = $pdo->prepare("SELECT * FROM users WHERE id = ?");  $stmt->execute([$id]);
来源：http://www.m.share.zdbjq.cn/Article/details/guytzibca.sHtML

[U70] PHP：PDO 事务
来源：http://www.blog.hesvh.cn/Article/details/gqvxsirfj.sHtML

$pdo->beginTransaction();  $pdo->commit();  $pdo->rollBack();
来源：http://www.share.fehbvm.com/Article/details/glbdvamul.sHtML

[U71] PHP：抛出异常
来源：http://mobile.zdbjq.cn/Article/details/gllzbunxk.sHtML

throw new RuntimeException("失败", 500);
来源：http://baike.zdbjq.cn/Article/details/gevykxish.sHtML

[U72] PHP：写错误日志
来源：http://baike.fehbvm.com/Article/details/gydybvlis.sHtML

error_log("失败: " . $e->getMessage());
来源：http://blog.zdbjq.cn/Article/details/gphlpscjw.sHtML

[U73] PHP：读取 ini 配置
来源：http://3g.zdbjq.cn/Article/details/gjcwbldig.sHtML

parse_ini_file("config.ini", true)
来源：http://www.share.fehbvm.com/Article/details/gmvpvxjjm.sHtML

[U74] PHP：读取环境变量
来源：http://baike.fehbvm.com/Article/details/grbhtkyth.sHtML

getenv("APP_ENV") ?: "production"
来源：http://read.share.fehbvm.com/Article/details/gbeyanicm.sHtML

[U75] PHP：依赖注入
来源：http://read.share.fehbvm.com/Article/details/gdavbyhbs.sHtML

composer require psr/container
来源：http://baike.fehbvm.com/Article/details/gttopvspx.sHtML

[U76] PHP：简单路由
来源：http://blog.zdbjq.cn/Article/details/gcvmcxwch.sHtML

$path = parse_url($_SERVER["REQUEST_URI"], PHP_URL_PATH);
来源：http://www.m.share.zdbjq.cn/Article/details/gnhsijtpr.sHtML

[U77] PHP：模板渲染
来源：http://3g.hesvh.cn/Article/details/gqejenbhp.sHtML

composer require twig/twig
来源：http://www.blog.hesvh.cn/Article/details/guwriisdb.sHtML

[U78] PHP：单元测试
来源：http://www.m.share.zdbjq.cn/Article/details/glhjjluvg.sHtML

composer require --dev phpunit/phpunit
来源：http://www.blog.zdbjq.cn/Article/details/gjyackvum.sHtML

[U79] PHP：静态分析
来源：http://baike.zdbjq.cn/Article/details/gyxkjbshh.sHtML

composer require --dev phpstan/phpstan
来源：http://www.blog.fehbvm.com/Article/details/gmrypzfqn.sHtML

[U80] PHP：代码规范修复
来源：http://mobile.fehbvm.com/Article/details/gvtvjvixp.sHtML

composer require --dev friendsofphp/php-cs-fixer
来源：http://mobile.zdbjq.cn/Article/details/gfbxnblax.sHtML

[U81] JS：初始化项目
来源：http://www.share.zdbjq.cn/Article/details/gwlrmqygf.sHtML

npm init -y;  npm i express
来源：http://baike.fehbvm.com/Article/details/gpxngskod.sHtML

[U82] JS：package.json 脚本
来源：http://www.m.share.hesvh.cn/Article/details/gcuqajugp.sHtML

"scripts": { "dev": "vite", "build": "vite build" }
来源：http://read.share.hesvh.cn/Article/details/gsnslmkbh.sHtML

[U83] JS：ES Module 导入导出
来源：http://www.share.zdbjq.cn/Article/details/gjwvogeyo.sHtML

export const a = 1;  import { a } from "./m.js";
来源：http://wap.fehbvm.com/Article/details/gephjhcsu.sHtML

[U84] JS：CommonJS 写法
来源：http://www.blog.hesvh.cn/Article/details/gaakpsetu.sHtML

module.exports = { a };  const { a } = require("./m");
来源：http://blog.zdbjq.cn/Article/details/gzdwmmdeg.sHtML

[U85] JS：可选链
来源：http://baike.hesvh.cn/Article/details/gjzcaqlpp.sHtML

a?.b?.c
来源：http://baike.zdbjq.cn/Article/details/gdslymijz.sHtML

[U86] JS：空值合并
来源：http://mobile.zdbjq.cn/Article/details/gvgkrwrvy.sHtML

a ?? b
来源：http://mobile.hesvh.cn/Article/details/gefuretck.sHtML

[U87] JS：解构默认值
来源：http://baike.fehbvm.com/Article/details/gmfhpyqif.sHtML

const { a = 1, b = 2 } = obj;
来源：http://www.share.fehbvm.com/Article/details/gbginltir.sHtML

[U88] JS：对象展开合并
来源：http://read.share.zdbjq.cn/Article/details/gxwehqsxt.sHtML

{ ...a, ...b }
来源：http://www.m.share.hesvh.cn/Article/details/gnxqnyhcu.sHtML

[U89] JS：数组去重
来源：http://mobile.zdbjq.cn/Article/details/gkmgfholh.sHtML

[...new Set(arr)]
来源：http://wap.zdbjq.cn/Article/details/glqueztii.sHtML

[U90] JS：数字数组排序
来源：http://www.blog.fehbvm.com/Article/details/gmteioktg.sHtML

[...arr].sort((a, b) => a - b)
来源：http://www.m.share.hesvh.cn/Article/details/gffvuxnqm.sHtML

[U91] JS：对象键值遍历
来源：http://3g.fehbvm.com/Article/details/giwbyxigo.sHtML

Object.entries(obj).forEach(([k, v]) => {});
来源：http://m.share.hesvh.cn/Article/details/gaprvcaql.sHtML

[U92] JS：深拷贝
来源：http://blog.hesvh.cn/Article/details/gsskzurmg.sHtML

structuredClone(obj)
来源：http://baike.fehbvm.com/Article/details/gyttdwipn.sHtML

[U93] JS：模板字符串
来源：http://mobile.zdbjq.cn/Article/details/gzmkdvojb.sHtML

`共 ${n} 条`
来源：http://3g.zdbjq.cn/Article/details/ghpafanel.sHtML

[U94] JS：箭头函数
来源：http://mobile.hesvh.cn/Article/details/gygpsgxva.sHtML

const double = x => x * 2;
来源：http://baike.zdbjq.cn/Article/details/gvxworufz.sHtML

[U95] JS：Promise 包装
来源：http://www.share.zdbjq.cn/Article/details/guatgpjeu.sHtML

new Promise((resolve, reject) => {})
来源：http://blog.hesvh.cn/Article/details/gfaeoyadr.sHtML

[U96] JS：async/await 与异常
来源：http://m.share.zdbjq.cn/Article/details/grtysnhxg.sHtML

try { const d = await f(); } catch (e) { console.error(e); }
来源：http://m.share.fehbvm.com/Article/details/gddjabwvu.sHtML

[U97] JS：并发请求
来源：http://m.share.zdbjq.cn/Article/details/gxzrecevh.sHtML

await Promise.all(urls.map(u => fetch(u)))
来源：http://baike.hesvh.cn/Article/details/guthkxodq.sHtML

[U98] JS：fetch 带 JSON
来源：http://3g.fehbvm.com/Article/details/ggsbgdkqm.sHtML

await fetch(url, { method: "POST", headers: { "Content-Type": "application/json" }, body: JSON.stringify(d) })
来源：http://read.share.fehbvm.com/Article/details/grhkommjs.sHtML

[U99] JS：事件监听
来源：http://blog.zdbjq.cn/Article/details/goxmmabzs.sHtML

el.addEventListener("click", e => {})
来源：http://baike.fehbvm.com/Article/details/gltsuqmgu.sHtML

[U100] JS：DOM 查询
来源：http://wap.zdbjq.cn/Article/details/ghefgyary.sHtML

document.querySelector(".item")
来源：http://m.share.hesvh.cn/Article/details/gnqdpsivh.sHtML

[U101] JS：classList 操作
来源：http://www.m.share.fehbvm.com/Article/details/gxxpwbzbi.sHtML

el.classList.toggle("active")
来源：http://wap.zdbjq.cn/Article/details/gdidzyrra.sHtML

[U102] JS：本地存储
来源：http://baike.zdbjq.cn/Article/details/gowkdjfyz.sHtML

localStorage.setItem("k", JSON.stringify(v))
来源：http://wap.zdbjq.cn/Article/details/gkwrjwczv.sHtML

[U103] JS：定时器
来源：http://mobile.fehbvm.com/Article/details/guexkwcrv.sHtML

setTimeout(fn, 1000);  setInterval(fn, 1000);
来源：http://mobile.fehbvm.com/Article/details/ggsxkefgw.sHtML

[U104] JS：防抖
来源：http://www.share.hesvh.cn/Article/details/gfrwaggwt.sHtML

const debounce = (fn, ms) => { let t; return (...a) => { clearTimeout(t); t = setTimeout(() => fn(...a), ms); }; };
来源：http://wap.zdbjq.cn/Article/details/gkwwltbzq.sHtML

[U105] JS：节流
来源：http://baike.zdbjq.cn/Article/details/ghjaocutq.sHtML

const throttle = (fn, ms) => { let last = 0; return (...a) => { const n = Date.now(); if (n - last >= ms) { last = n; fn(...a); } }; };
来源：http://www.blog.hesvh.cn/Article/details/gfqrtngnh.sHtML

[U106] JS：日期格式化
来源：http://read.share.zdbjq.cn/Article/details/gicqahnts.sHtML

new Intl.DateTimeFormat("zh-CN", { dateStyle: "medium" }).format(new Date())
来源：http://www.m.share.zdbjq.cn/Article/details/gdwgmswlp.sHtML

[U107] JS：数字千分位
来源：http://3g.hesvh.cn/Article/details/gvfkkxnel.sHtML

new Intl.NumberFormat("en-US").format(1234567)
来源：http://wap.zdbjq.cn/Article/details/gplnagafq.sHtML

[U108] JS：随机整数
来源：http://wap.zdbjq.cn/Article/details/gydwkufyd.sHtML

Math.floor(Math.random() * (max - min + 1)) + min
来源：http://mobile.zdbjq.cn/Article/details/gekcqmmxi.sHtML

[U109] JS：数组分组
来源：http://3g.hesvh.cn/Article/details/gjbfigxoy.sHtML

Object.groupBy(arr, x => x.type)
来源：http://mobile.hesvh.cn/Article/details/gfxryvkho.sHtML

[U110] JS：数组分块
来源：http://www.share.fehbvm.com/Article/details/gxvkwglge.sHtML

arr.reduce((acc, x, i) => (i % size ? acc : [...acc, arr.slice(i, i + size)]), [])
来源：http://baike.zdbjq.cn/Article/details/gbxbhapfy.sHtML

[U111] JS：对象转 Map
来源：http://www.blog.hesvh.cn/Article/details/goffrgilu.sHtML

new Map(Object.entries(obj))
来源：http://blog.hesvh.cn/Article/details/gzehuptnp.sHtML

[U112] JS：字符串补位
来源：http://wap.zdbjq.cn/Article/details/gkhzudtbq.sHtML

"7".padStart(3, "0")
来源：http://baike.hesvh.cn/Article/details/ggejmwvtd.sHtML

[U113] JS：正则替换全部
来源：http://read.share.zdbjq.cn/Article/details/gyvziznvs.sHtML

s.replaceAll("a", "b")
来源：http://wap.zdbjq.cn/Article/details/gnqkmfwnf.sHtML

[U114] JS：JSON 深比较
来源：http://www.blog.zdbjq.cn/Article/details/grvbkuwul.sHtML

JSON.stringify(a) === JSON.stringify(b)
来源：http://www.blog.fehbvm.com/Article/details/gqvumkfgl.sHtML

[U115] JS：生成 UUID
来源：http://www.share.zdbjq.cn/Article/details/gtaekcvfh.sHtML

crypto.randomUUID()
来源：http://m.share.fehbvm.com/Article/details/gnkkurpja.sHtML

[U116] JS：类型检查（JSDoc）
来源：http://www.share.fehbvm.com/Article/details/grbadecnr.sHtML

/** @param {string} name */ function f(name) {}
来源：http://blog.fehbvm.com/Article/details/ggtwaxjja.sHtML

[U117] JS：单元测试
来源：http://m.share.hesvh.cn/Article/details/gfhbekqps.sHtML

npm i -D vitest;  npx vitest
来源：http://www.share.fehbvm.com/Article/details/gdwlezcqw.sHtML

[U118] JS：开发服务器
来源：http://m.share.fehbvm.com/Article/details/gapatkqug.sHtML

npm i -D vite;  npx vite
来源：http://m.share.hesvh.cn/Article/details/grrkxrnkf.sHtML

[U119] JS：生产构建
来源：http://www.share.hesvh.cn/Article/details/gnehfggap.sHtML

npx vite build
来源：http://m.share.zdbjq.cn/Article/details/gvmioohtw.sHtML

[U120] JS：读取环境变量（Vite）
来源：http://blog.fehbvm.com/Article/details/gytruktmb.sHtML

import.meta.env.VITE_API_URL
来源：http://wap.hesvh.cn/Article/details/gfnsmcdgm.sHtML

================================================================================
来源：http://blog.fehbvm.com/Article/details/guqlnendv.sHtML

统计汇总
来源：http://read.share.hesvh.cn/Article/details/gugagfiyq.sHtML

================================================================================
来源：http://m.share.fehbvm.com/Article/details/gdmvohuyy.sHtML

按语言统计（条）：
来源：http://www.share.zdbjq.cn/Article/details/gvgiisosi.sHtML

Python ......... 252
来源：http://baike.zdbjq.cn/Article/details/gmbtogdsb.sHtML

PHP ............ 252
来源：http://read.share.fehbvm.com/Article/details/ginjovwfj.sHtML

JavaScript ..... 252
来源：http://baike.hesvh.cn/Article/details/gvrjlfqzj.sHtML

TypeScript ..... 212
来源：http://m.share.zdbjq.cn/Article/details/gjzrezwpv.sHtML

Java ........... 212
来源：http://3g.fehbvm.com/Article/details/gnpcrgtva.sHtML

Go ............. 212
来源：http://m.share.zdbjq.cn/Article/details/gbjcleyyl.sHtML

Ruby ........... 212
来源：http://www.blog.hesvh.cn/Article/details/gznodfjue.sHtML

C# ............. 212
来源：http://www.blog.zdbjq.cn/Article/details/gjicxwjav.sHtML

C .............. 30
来源：http://blog.zdbjq.cn/Article/details/gytetfmej.sHtML

C++ ............ 30
来源：http://3g.fehbvm.com/Article/details/gngntbflw.sHtML

SQL ............ 90
来源：http://blog.hesvh.cn/Article/details/guejiqtjn.sHtML

Bash ........... 80
来源：http://www.blog.zdbjq.cn/Article/details/giplhrhao.sHtML

Kotlin ......... 15
来源：http://m.share.fehbvm.com/Article/details/gdkbqltyl.sHtML

Swift .......... 15
来源：http://wap.zdbjq.cn/Article/details/gdvaznfxl.sHtML

Lua ............ 10
来源：http://blog.zdbjq.cn/Article/details/gpnittgfc.sHtML

Perl ........... 10
来源：http://www.m.share.zdbjq.cn/Article/details/ggogvvgox.sHtML

Scala .......... 10
来源：http://m.share.zdbjq.cn/Article/details/godpnewbe.sHtML

------------------------------------
来源：http://3g.fehbvm.com/Article/details/gamhbruyu.sHtML

合计 ........... 2106 条
来源：http://mobile.hesvh.cn/Article/details/gmrfrkqzs.sHtML

按章节统计：
来源：http://www.m.share.hesvh.cn/Article/details/guzzfqquo.sHtML

A 基础语法与类型       26 个任务 × 8 语言 =  208
来源：http://www.blog.hesvh.cn/Article/details/gakjzipeh.sHtML

B 流程控制             16 个任务 × 8 语言 =  128
来源：http://m.share.fehbvm.com/Article/details/gyzxmzmvp.sHtML

C 函数与作用域         16 个任务 × 8 语言 =  128
来源：http://baike.fehbvm.com/Article/details/ggwwirwal.sHtML

D 数组 / 列表 / 集合   26 个任务 × 8 语言 =  208
来源：http://baike.zdbjq.cn/Article/details/gjhvhmgpt.sHtML

E 字符串处理           22 个任务 × 8 语言 =  176
来源：http://m.share.hesvh.cn/Article/details/glbljqqpi.sHtML

F 文件与目录           12 个任务 × 8 语言 =   96
来源：http://www.m.share.zdbjq.cn/Article/details/gezntfkrp.sHtML

G 面向对象             16 个任务 × 8 语言 =  128
来源：http://read.share.fehbvm.com/Article/details/glbbjbtep.sHtML

H 异常与错误处理       10 个任务 × 8 语言 =   80
来源：http://www.blog.fehbvm.com/Article/details/gezrshwep.sHtML

I 正则表达式            8 个任务 × 8 语言 =   64
来源：http://wap.hesvh.cn/Article/details/gbslbsbjx.sHtML

J 日期与时间           10 个任务 × 8 语言 =   80
来源：http://www.share.zdbjq.cn/Article/details/gotcqsmgr.sHtML

K JSON 与序列化         8 个任务 × 8 语言 =   64
来源：http://wap.fehbvm.com/Article/details/gznubydvz.sHtML

L 网络请求              8 个任务 × 8 语言 =   64
来源：http://m.share.zdbjq.cn/Article/details/gstohjhbr.sHtML

M 命令行 / 进程         8 个任务 × 8 语言 =   64
来源：http://www.share.zdbjq.cn/Article/details/giucajhva.sHtML

N 数据结构与算法       12 个任务 × 8 语言 =   96
来源：http://www.share.fehbvm.com/Article/details/gbfvxmnmy.sHtML

O 并发与异步            6 个任务 × 8 语言 =   48
来源：http://www.m.share.fehbvm.com/Article/details/gbjpgmxxb.sHtML

P 常用工具函数          8 个任务 × 8 语言 =   64
来源：http://m.share.zdbjq.cn/Article/details/gkxuhmybq.sHtML

Q SQL 专题                              90
来源：http://baike.zdbjq.cn/Article/details/gpfrwmqgv.sHtML

R Bash 专题                             80
来源：http://www.blog.zdbjq.cn/Article/details/gawgpzmzc.sHtML

S C / C++ 专题                          60
来源：http://www.blog.zdbjq.cn/Article/details/gftltzfyo.sHtML

T 其他语言补充                          60
来源：http://www.share.fehbvm.com/Article/details/geuaxswzj.sHtML

U 高频实用片段                         120
来源：http://wap.zdbjq.cn/Article/details/gagxtltok.sHtML

------------------------------------
来源：http://www.share.zdbjq.cn/Article/details/gktrjbkmh.sHtML

合计                                  2106 条
来源：http://wap.fehbvm.com/Article/details/gzrcgtrla.sHtML

--------------------------------------------------------------------------------
来源：http://www.share.zdbjq.cn/Article/details/gqhwgxtpd.sHtML

使用提醒
来源：http://blog.fehbvm.com/Article/details/gqdkbjsvv.sHtML

--------------------------------------------------------------------------------
来源：http://wap.zdbjq.cn/Article/details/gkgzuxeee.sHtML

1. 示例追求"最小可用"，正式项目中请补齐导入、错误处理与边界判断。
来源：http://www.blog.zdbjq.cn/Article/details/grpxdwboa.sHtML

2. 涉及文件、网络、数据库的示例，注意资源释放与异常捕获。
来源：http://www.blog.zdbjq.cn/Article/details/gefxqlaxh.sHtML

3. 语言版本差异较大（如 Python 3.10 的 match、Java 17 的 record/switch 箭头），
来源：http://mobile.fehbvm.com/Article/details/gttcezojf.sHtML

在旧版本上使用前请先确认语法支持情况。
来源：http://mobile.zdbjq.cn/Article/details/gwxuptprx.sHtML

4. 标注"手写"的条目是因为该语言缺少对应内置能力，实际项目中可引入成熟库。
来源：http://read.share.fehbvm.com/Article/details/gmbenfehh.sHtML

—— 文件结束 ——
来源：http://3g.hesvh.cn/Article/details/glcpwseaj.sHtML

================================================================================
来源：http://blog.fehbvm.com/Article/details/glholkifc.sHtML

程序语言常见例子速查手册（2024 版）
来源：http://read.share.fehbvm.com/Article/details/gzgiruibw.sHtML

Common Programming Examples Cheat Book
来源：http://www.m.share.hesvh.cn/Article/details/ghdtfvysh.sHtML

================================================================================
来源：http://www.blog.zdbjq.cn/Article/details/grihljade.sHtML

【收录内容】
来源：http://www.m.share.hesvh.cn/Article/details/gffqeafuy.sHtML

覆盖 12 种语言 / 语法与常见 API：
来源：http://blog.zdbjq.cn/Article/details/gkbhdajwx.sHtML

Python · PHP · JavaScript · TypeScript · Java · Go · Ruby · C#
来源：http://wap.zdbjq.cn/Article/details/gsgdiivey.sHtML

SQL · Bash · C · C++
来源：http://www.blog.zdbjq.cn/Article/details/gqnfllkpd.sHtML

按「任务」分组：每个任务下按语言各给出一条最小可用示例。
来源：http://www.blog.zdbjq.cn/Article/details/gaawucgsq.sHtML

【使用说明】
来源：http://blog.hesvh.cn/Article/details/gagsiogte.sHtML

1. 每个任务形如 "[编号] 任务名"，下面每行以语言标记开头：
来源：http://blog.fehbvm.com/Article/details/gzzslgykl.sHtML

Py:    Python        PHP:   PHP           JS:    JavaScript
来源：http://baike.hesvh.cn/Article/details/gkamezwvb.sHtML

TS:    TypeScript    Java:  Java          Go:    Go
来源：http://baike.zdbjq.cn/Article/details/garyidcxs.sHtML

Ruby:  Ruby          C#:    C#            SQL:   SQL
来源：http://www.m.share.zdbjq.cn/Article/details/gygixzlze.sHtML

Bash:  Shell         C:     C             C++:   C++
来源：http://www.blog.hesvh.cn/Article/details/grqsmusqj.sHtML

2. 示例只展示核心写法，刻意省略 import / require / include / using 等样板代码。
来源：http://www.share.zdbjq.cn/Article/details/gmvqbmpvl.sHtML

需要完整可运行文件时，请自行补齐当前语言的导入语句。
来源：http://www.m.share.fehbvm.com/Article/details/gojjjzkyn.sHtML

3. 语法基准：Python 3.10+ / PHP 8.1+ / ES2020+ / TypeScript 5 / Java 17 /
来源：http://www.m.share.hesvh.cn/Article/details/gwjlhseze.sHtML

Go 1.21+ / Ruby 3.x / C# 10+ / C17 / C++17。
来源：http://www.blog.zdbjq.cn/Article/details/gxgyczlvh.sHtML

4. 检索建议：用编辑器或浏览器 Ctrl+F 搜关键词，如 "排序" "读取文件" "正则"。
来源：http://baike.fehbvm.com/Article/details/gesaxsqub.sHtML

5. 标记为 "// 无" 表示该语言没有对应的一等语法，需用替代写法（示例给出替代方案）。
来源：http://www.blog.zdbjq.cn/Article/details/ggxfqzlzx.sHtML

6. 符号 "⏎" 表示代码在此处换行（主要用于 Python 等强制缩进、无法压成一行的结构）。
来源：http://3g.fehbvm.com/Article/details/grbgxrxds.sHtML

【文件统计】
来源：http://wap.hesvh.cn/Article/details/gqkbziqsv.sHtML

语言示例共 2106 条，分布见本文末尾的「统计汇总」。
来源：http://blog.fehbvm.com/Article/details/giagiyhns.sHtML

--------------------------------------------------------------------------------
来源：http://www.blog.zdbjq.cn/Article/details/gjgnyydeq.sHtML

目  录
来源：http://www.share.fehbvm.com/Article/details/gvfbbksnb.sHtML

--------------------------------------------------------------------------------
来源：http://www.share.hesvh.cn/Article/details/gerdhbhha.sHtML

A. 基础语法与类型              （第 1 节，26 个任务，208 条）
来源：http://www.m.share.fehbvm.com/Article/details/gfcfbearr.sHtML

B. 流程控制                    （第 2 节，16 个任务，128 条）
来源：http://m.share.hesvh.cn/Article/details/gfepplbrg.sHtML

C. 函数与作用域                （第 3 节，16 个任务，128 条）
来源：http://www.m.share.hesvh.cn/Article/details/ghiokirud.sHtML

D. 数组 / 列表 / 集合          （第 4 节，26 个任务，208 条）
来源：http://wap.fehbvm.com/Article/details/gjhqezpjl.sHtML

E. 字符串处理                  （第 5 节，22 个任务，176 条）
来源：http://wap.fehbvm.com/Article/details/gywuknxul.sHtML


<!-- 参考信息 -->