代发 wailian999

[U17] Py：初始化日志
来源：http://wap.fanxiaobao.xyz/Article/details/gqcseqann.sHtML

logging.basicConfig(level=logging.INFO)
来源：http://wap.fanxiaobao.xyz/Article/details/gzoqrfggn.sHtML

[U18] Py：预编译正则
来源：http://m.share.fanxiaobao.xyz/Article/details/gubpxkskk.sHtML

pat = re.compile(r"\d+")
来源：http://m.share.fanxiaobao.xyz/Article/details/gsgxrdrsw.sHtML

[U19] Py：正则替换带回调
来源：http://wap.fanxiaobao.xyz/Article/details/gauzroumd.sHtML

re.sub(r"\d+", lambda m: str(int(m.group()) * 2), s)
来源：http://www.blog.fanxiaobao.xyz/Article/details/gtogjjqms.sHtML

[U20] Py：缓存函数结果
来源：http://www.blog.fanxiaobao.xyz/Article/details/gozwopmtm.sHtML

@functools.lru_cache(maxsize=None)
来源：http://read.share.fanxiaobao.xyz/Article/details/gfeontihj.sHtML

[U21] Py：自定义上下文管理器
来源：http://www.blog.fanxiaobao.xyz/Article/details/gobdsfnwy.sHtML

@contextlib.contextmanager
来源：http://baike.fanxiaobao.xyz/Article/details/gvgrvxpgp.sHtML

[U22] Py：矩阵转置
来源：http://mobile.fanxiaobao.xyz/Article/details/gkpdfbujc.sHtML

list(zip(*m))
来源：http://blog.fanxiaobao.xyz/Article/details/gmbitqmam.sHtML

[U23] Py：分块读取大文件
来源：http://m.share.fanxiaobao.xyz/Article/details/gjgoprnht.sHtML

for chunk in iter(lambda: f.read(8192), b""):
来源：http://m.share.fanxiaobao.xyz/Article/details/gdedrfihj.sHtML

[U24] Py：路径操作
来源：http://www.blog.fanxiaobao.xyz/Article/details/gleswvgvn.sHtML

Path("a/b.txt").parent.mkdir(parents=True, exist_ok=True)
来源：http://read.share.fanxiaobao.xyz/Article/details/gkgzycewg.sHtML

[U25] Py：CSV 按字典读
来源：http://blog.fanxiaobao.xyz/Article/details/gagwzxcnq.sHtML

csv.DictReader(f)
来源：http://mobile.fanxiaobao.xyz/Article/details/gdbyhmljw.sHtML

[U26] Py：并发下载
来源：http://3g.fanxiaobao.xyz/Article/details/gjrotzpwu.sHtML

ThreadPoolExecutor(max_workers=8).map(fetch, urls)
来源：http://wap.fanxiaobao.xyz/Article/details/geygwwxyj.sHtML

[U27] Py：异步 HTTP
来源：http://m.share.fanxiaobao.xyz/Article/details/gjunslxtw.sHtML

aiohttp.ClientSession() 配合 async with
来源：http://blog.fanxiaobao.xyz/Article/details/gbxqcjyuv.sHtML

[U28] Py：类型别名
来源：http://baike.fanxiaobao.xyz/Article/details/gpcazvzph.sHtML

UserId = int
来源：http://baike.fanxiaobao.xyz/Article/details/gkncqgxsq.sHtML

[U29] Py：属性校验
来源：http://m.share.fanxiaobao.xyz/Article/details/gnoshaywj.sHtML

@property 与 @x.setter 配合
来源：http://read.share.fanxiaobao.xyz/Article/details/gcaczduyn.sHtML

[U30] Py：数据类
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gcmyuwxlr.sHtML

@dataclass(slots=True)
来源：http://www.share.fanxiaobao.xyz/Article/details/gnqbvvcer.sHtML

[U31] Py：单测
来源：http://3g.fanxiaobao.xyz/Article/details/gzpuvsibs.sHtML

python -m pytest -q
来源：http://www.blog.fanxiaobao.xyz/Article/details/ginvswbif.sHtML

[U32] Py：代码格式化
来源：http://mobile.fanxiaobao.xyz/Article/details/gqxexrssp.sHtML

ruff format . && ruff check --fix .
来源：http://3g.fanxiaobao.xyz/Article/details/gznusmnkw.sHtML

[U33] Py：打包发布
来源：http://mobile.fanxiaobao.xyz/Article/details/gdxliqyoh.sHtML

python -m build  （依赖 pyproject.toml）
来源：http://3g.fanxiaobao.xyz/Article/details/grwvjchxg.sHtML

[U34] Py：判断编码
来源：http://3g.fanxiaobao.xyz/Article/details/gmwdacbkb.sHtML

chardet.detect(raw)
来源：http://baike.fanxiaobao.xyz/Article/details/ggrdrdrkz.sHtML

[U35] Py：发送邮件
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gftlqdomn.sHtML

smtplib.SMTP_SSL(...).send_message(msg)
来源：http://3g.fanxiaobao.xyz/Article/details/gqnrjcxfl.sHtML

[U36] Py：定时任务
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gjofglpen.sHtML

schedule.every(10).minutes.do(job)
来源：http://mobile.fanxiaobao.xyz/Article/details/gwvvxrbey.sHtML

[U37] Py：读写 Excel
来源：http://www.blog.fanxiaobao.xyz/Article/details/gwvzisfli.sHtML

pandas.read_excel / DataFrame.to_excel
来源：http://m.share.fanxiaobao.xyz/Article/details/gqtqmgusg.sHtML

[U38] Py：获取脚本所在目录
来源：http://blog.fanxiaobao.xyz/Article/details/gvcmmfufx.sHtML

Path(__file__).resolve().parent
来源：http://read.share.fanxiaobao.xyz/Article/details/gwxsdedfr.sHtML

[U39] Py：判断是否在交互环境
来源：http://m.share.fanxiaobao.xyz/Article/details/gnimiangh.sHtML

sys.stdout.isatty()
来源：http://baike.fanxiaobao.xyz/Article/details/gcmxyveyi.sHtML

[U40] Py：打印到标准错误
来源：http://www.m.share.fanxiaobao.xyz/Article/details/guxpgdwfx.sHtML

print("err", file=sys.stderr)
来源：http://mobile.fanxiaobao.xyz/Article/details/golwyahet.sHtML

[U41] PHP：初始化 Composer 项目
来源：http://wap.fanxiaobao.xyz/Article/details/gsrqhuyyh.sHtML

composer init;  composer require guzzlehttp/guzzle
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gcceqjxvv.sHtML

[U42] PHP：PSR-4 自动加载
来源：http://mobile.fanxiaobao.xyz/Article/details/gyjyloyde.sHtML

"autoload": { "psr-4": { "App\\": "src/" } }
来源：http://blog.fanxiaobao.xyz/Article/details/gqqooqfth.sHtML

[U43] PHP：声明命名空间
来源：http://www.blog.fanxiaobao.xyz/Article/details/gghxezdpn.sHtML

namespace App\Http;
来源：http://mobile.fanxiaobao.xyz/Article/details/gadcczrkc.sHtML

[U44] PHP：开启严格类型
来源：http://read.share.fanxiaobao.xyz/Article/details/gmcqmeubg.sHtML

declare(strict_types=1);
来源：http://www.share.fanxiaobao.xyz/Article/details/ggzrstcyg.sHtML

[U45] PHP：类型声明与返回类型
来源：http://read.share.fanxiaobao.xyz/Article/details/gdnwwykzg.sHtML

function add(int $a, int $b): int { return $a + $b; }
来源：http://www.share.fanxiaobao.xyz/Article/details/gbjqfxlze.sHtML

[U46] PHP：可空类型
来源：http://www.blog.fanxiaobao.xyz/Article/details/ggfruawvq.sHtML

?string $name = null
来源：http://baike.fanxiaobao.xyz/Article/details/gcxbjmdwb.sHtML

[U47] PHP：联合类型
来源：http://read.share.fanxiaobao.xyz/Article/details/grbdvrlsu.sHtML

int|string $id
来源：http://baike.fanxiaobao.xyz/Article/details/gmoscowjf.sHtML

[U48] PHP：纯枚举
来源：http://wap.fanxiaobao.xyz/Article/details/gzdwqgrax.sHtML

enum Status: string { case Active = "active"; case Off = "off"; }
来源：http://www.m.share.fanxiaobao.xyz/Article/details/ggclrzcsn.sHtML

[U49] PHP：只读属性
来源：http://www.share.fanxiaobao.xyz/Article/details/gjnrfpsja.sHtML

public readonly string $name
来源：http://www.blog.fanxiaobao.xyz/Article/details/gzfqjgeaf.sHtML

[U50] PHP：构造器属性提升
来源：http://m.share.fanxiaobao.xyz/Article/details/gzmdfkynm.sHtML

public function __construct(private int $id) {}
来源：http://wap.fanxiaobao.xyz/Article/details/guxmwhery.sHtML

[U51] PHP：数组解构
来源：http://baike.fanxiaobao.xyz/Article/details/golqxqpbn.sHtML

[$a, $b] = $arr;
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gsywqidse.sHtML

[U52] PHP：箭头函数
来源：http://blog.fanxiaobao.xyz/Article/details/gfgkkuksd.sHtML

$double = fn($x) => $x * 2;
来源：http://www.share.fanxiaobao.xyz/Article/details/gdpgprbjn.sHtML

[U53] PHP：空合并运算符
来源：http://m.share.fanxiaobao.xyz/Article/details/gqeomlioy.sHtML

$v = $a ?? $b ?? "default";
来源：http://m.share.fanxiaobao.xyz/Article/details/gknmfsqnl.sHtML

[U54] PHP：空安全调用
来源：http://www.blog.fanxiaobao.xyz/Article/details/glhlzbcnf.sHtML

$obj?->method()
来源：http://3g.fanxiaobao.xyz/Article/details/gvkhgxbbh.sHtML

[U55] PHP：match 表达式
来源：http://baike.fanxiaobao.xyz/Article/details/ggigvygol.sHtML

$s = match($x) { 1 => "一", default => "其他" };
来源：http://mobile.fanxiaobao.xyz/Article/details/gjqtgtzfc.sHtML

[U56] PHP：命名参数
来源：http://blog.fanxiaobao.xyz/Article/details/gtgeutldo.sHtML

f(a: 1, b: 2)
来源：http://www.blog.fanxiaobao.xyz/Article/details/gzmitlvkr.sHtML

[U57] PHP：字符串插值
来源：http://blog.fanxiaobao.xyz/Article/details/gwrnsbtza.sHtML

"值: {$a}"
来源：http://mobile.fanxiaobao.xyz/Article/details/gzyjfsxre.sHtML

[U58] PHP：数组三件套
来源：http://blog.fanxiaobao.xyz/Article/details/gwqplqiui.sHtML

array_map($f, $a);  array_filter($a, $f);  array_reduce($a, $f, 0);
来源：http://www.blog.fanxiaobao.xyz/Article/details/gwnbsdddb.sHtML

[U59] PHP：自定义排序
来源：http://baike.fanxiaobao.xyz/Article/details/gddhgmbgx.sHtML

usort($arr, fn($a, $b) => $a["age"] <=> $b["age"]);
来源：http://blog.fanxiaobao.xyz/Article/details/gakanelct.sHtML

[U60] PHP：JSON 编解码
来源：http://mobile.fanxiaobao.xyz/Article/details/giusoidnd.sHtML

json_encode($d, JSON_UNESCAPED_UNICODE);  json_decode($s, true);
来源：http://www.share.fanxiaobao.xyz/Article/details/ggoxmwnck.sHtML

[U61] PHP：正则
来源：http://baike.fanxiaobao.xyz/Article/details/gvsdzacjo.sHtML

preg_match('/(\d+)/', $s, $m);  preg_replace('/\d+/', '#', $s);
来源：http://read.share.fanxiaobao.xyz/Article/details/gyeazgnff.sHtML

[U62] PHP：日期对象
来源：http://mobile.fanxiaobao.xyz/Article/details/gofeaeycz.sHtML

(new DateTimeImmutable())->format("Y-m-d");
来源：http://read.share.fanxiaobao.xyz/Article/details/gcffaqodt.sHtML

[U63] PHP：文件读写
来源：http://baike.fanxiaobao.xyz/Article/details/gfqdhkimi.sHtML

file_get_contents($f);  file_put_contents($f, $data);
来源：http://www.share.fanxiaobao.xyz/Article/details/gdqkgiuxe.sHtML

[U64] PHP：目录遍历
来源：http://m.share.fanxiaobao.xyz/Article/details/gdqqlyruc.sHtML

glob("dir/*.php");  scandir("dir");
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gehiipukw.sHtML

[U65] PHP：会话
来源：http://m.share.fanxiaobao.xyz/Article/details/gfodtwzww.sHtML

session_start();  $_SESSION["uid"] = 1;
来源：http://www.blog.fanxiaobao.xyz/Article/details/gehsmwlbj.sHtML

[U66] PHP：设置 Cookie
来源：http://baike.fanxiaobao.xyz/Article/details/gzbxoxsmz.sHtML

setcookie("token", $v, ["httponly" => true, "samesite" => "Lax"]);
来源：http://m.share.fanxiaobao.xyz/Article/details/gmwgvtcvh.sHtML

[U67] PHP：处理文件上传
来源：http://read.share.fanxiaobao.xyz/Article/details/gzznwuaot.sHtML

$_FILES["file"]["tmp_name"] 与 move_uploaded_file()
来源：http://www.blog.fanxiaobao.xyz/Article/details/gkbzhgoil.sHtML

[U68] PHP：PDO 连接
来源：http://baike.fanxiaobao.xyz/Article/details/gjhskakmr.sHtML

$pdo = new PDO("mysql:host=localhost;dbname=app", "root", "");
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gfrepijsv.sHtML

[U69] PHP：PDO 预处理
来源：http://www.blog.fanxiaobao.xyz/Article/details/gjliugrce.sHtML

$stmt = $pdo->prepare("SELECT * FROM users WHERE id = ?");  $stmt->execute([$id]);
来源：http://mobile.fanxiaobao.xyz/Article/details/gpzegcmuv.sHtML

[U70] PHP：PDO 事务
来源：http://www.share.fanxiaobao.xyz/Article/details/gkjgfiypd.sHtML

$pdo->beginTransaction();  $pdo->commit();  $pdo->rollBack();
来源：http://www.blog.fanxiaobao.xyz/Article/details/grhvaiapg.sHtML

[U71] PHP：抛出异常
来源：http://3g.fanxiaobao.xyz/Article/details/gjvkadnky.sHtML

throw new RuntimeException("失败", 500);
来源：http://www.share.fanxiaobao.xyz/Article/details/gvcpfhuei.sHtML

[U72] PHP：写错误日志
来源：http://blog.fanxiaobao.xyz/Article/details/gvhtoatqr.sHtML

error_log("失败: " . $e->getMessage());
来源：http://mobile.fanxiaobao.xyz/Article/details/glqeshrit.sHtML

[U73] PHP：读取 ini 配置
来源：http://www.share.fanxiaobao.xyz/Article/details/gcroumjoh.sHtML

parse_ini_file("config.ini", true)
来源：http://www.share.fanxiaobao.xyz/Article/details/gijwmaevd.sHtML

[U74] PHP：读取环境变量
来源：http://baike.fanxiaobao.xyz/Article/details/gowbntwzu.sHtML

getenv("APP_ENV") ?: "production"
来源：http://www.share.fanxiaobao.xyz/Article/details/gpqsxudpl.sHtML

[U75] PHP：依赖注入
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gzwalxtyj.sHtML

composer require psr/container
来源：http://blog.fanxiaobao.xyz/Article/details/gezoxclyg.sHtML

[U76] PHP：简单路由
来源：http://baike.fanxiaobao.xyz/Article/details/gjulavmno.sHtML

$path = parse_url($_SERVER["REQUEST_URI"], PHP_URL_PATH);
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gyitkmddj.sHtML

[U77] PHP：模板渲染
来源：http://www.share.fanxiaobao.xyz/Article/details/gequoijud.sHtML

composer require twig/twig
来源：http://wap.fanxiaobao.xyz/Article/details/gamiqhuki.sHtML

[U78] PHP：单元测试
来源：http://3g.fanxiaobao.xyz/Article/details/gatgpzsqj.sHtML

composer require --dev phpunit/phpunit
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gmiksglgf.sHtML

[U79] PHP：静态分析
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gnfwnwmgg.sHtML

composer require --dev phpstan/phpstan
来源：http://www.share.fanxiaobao.xyz/Article/details/gmqwmuhih.sHtML

[U80] PHP：代码规范修复
来源：http://baike.fanxiaobao.xyz/Article/details/gatbtuyvs.sHtML

composer require --dev friendsofphp/php-cs-fixer
来源：http://mobile.fanxiaobao.xyz/Article/details/gjcwtocbk.sHtML

[U81] JS：初始化项目
来源：http://mobile.fanxiaobao.xyz/Article/details/guthyfuam.sHtML

npm init -y;  npm i express
来源：http://blog.fanxiaobao.xyz/Article/details/gemirobqk.sHtML

[U82] JS：package.json 脚本
来源：http://baike.fanxiaobao.xyz/Article/details/gfcqcqykg.sHtML

"scripts": { "dev": "vite", "build": "vite build" }
来源：http://read.share.fanxiaobao.xyz/Article/details/gtrabvbhm.sHtML

[U83] JS：ES Module 导入导出
来源：http://wap.fanxiaobao.xyz/Article/details/gzdutysvi.sHtML

export const a = 1;  import { a } from "./m.js";
来源：http://m.share.fanxiaobao.xyz/Article/details/gpxncldxo.sHtML

[U84] JS：CommonJS 写法
来源：http://wap.fanxiaobao.xyz/Article/details/gnzqnqrne.sHtML

module.exports = { a };  const { a } = require("./m");
来源：http://mobile.fanxiaobao.xyz/Article/details/gaawsobpe.sHtML

[U85] JS：可选链
来源：http://3g.fanxiaobao.xyz/Article/details/gozturieg.sHtML

a?.b?.c
来源：http://read.share.fanxiaobao.xyz/Article/details/gsbghejpu.sHtML

[U86] JS：空值合并
来源：http://baike.fanxiaobao.xyz/Article/details/gtljmawle.sHtML

a ?? b
来源：http://wap.fanxiaobao.xyz/Article/details/gzzeskjwn.sHtML

[U87] JS：解构默认值
来源：http://www.blog.fanxiaobao.xyz/Article/details/guxukcbfj.sHtML

const { a = 1, b = 2 } = obj;
来源：http://3g.fanxiaobao.xyz/Article/details/gumzewyug.sHtML

[U88] JS：对象展开合并
来源：http://3g.fanxiaobao.xyz/Article/details/gmqzvukgq.sHtML

{ ...a, ...b }
来源：http://mobile.fanxiaobao.xyz/Article/details/gdubpppzj.sHtML

[U89] JS：数组去重
来源：http://www.share.fanxiaobao.xyz/Article/details/gdddggbdg.sHtML

[...new Set(arr)]
来源：http://baike.fanxiaobao.xyz/Article/details/gizkoyzjc.sHtML

[U90] JS：数字数组排序
来源：http://mobile.fanxiaobao.xyz/Article/details/gwnazctsn.sHtML

[...arr].sort((a, b) => a - b)
来源：http://3g.fanxiaobao.xyz/Article/details/gncljxwyz.sHtML

[U91] JS：对象键值遍历
来源：http://m.share.fanxiaobao.xyz/Article/details/gqhrjtujb.sHtML

Object.entries(obj).forEach(([k, v]) => {});
来源：http://www.blog.fanxiaobao.xyz/Article/details/ghglmqrji.sHtML

[U92] JS：深拷贝
来源：http://baike.fanxiaobao.xyz/Article/details/gnpxxgsih.sHtML

structuredClone(obj)
来源：http://mobile.fanxiaobao.xyz/Article/details/gufjvlpex.sHtML

[U93] JS：模板字符串
来源：http://m.share.fanxiaobao.xyz/Article/details/gsvwygnaf.sHtML

`共 ${n} 条`
来源：http://read.share.fanxiaobao.xyz/Article/details/ggbuxksqa.sHtML

[U94] JS：箭头函数
来源：http://m.share.fanxiaobao.xyz/Article/details/gahqspkqn.sHtML

const double = x => x * 2;
来源：http://blog.fanxiaobao.xyz/Article/details/gbfqepukf.sHtML

[U95] JS：Promise 包装
来源：http://www.blog.fanxiaobao.xyz/Article/details/gjpjjrnjp.sHtML

new Promise((resolve, reject) => {})
来源：http://mobile.fanxiaobao.xyz/Article/details/gmfcshesa.sHtML

[U96] JS：async/await 与异常
来源：http://baike.fanxiaobao.xyz/Article/details/gvwnfthpr.sHtML

try { const d = await f(); } catch (e) { console.error(e); }
来源：http://blog.fanxiaobao.xyz/Article/details/gztsqedsg.sHtML

[U97] JS：并发请求
来源：http://baike.fanxiaobao.xyz/Article/details/grbdcoxgz.sHtML

await Promise.all(urls.map(u => fetch(u)))
来源：http://blog.fanxiaobao.xyz/Article/details/gvsgrgarh.sHtML

[U98] JS：fetch 带 JSON
来源：http://blog.fanxiaobao.xyz/Article/details/genxlkmxp.sHtML

await fetch(url, { method: "POST", headers: { "Content-Type": "application/json" }, body: JSON.stringify(d) })
来源：http://3g.fanxiaobao.xyz/Article/details/glkpkijtd.sHtML

[U99] JS：事件监听
来源：http://wap.fanxiaobao.xyz/Article/details/gheldxbiy.sHtML

el.addEventListener("click", e => {})
来源：http://mobile.fanxiaobao.xyz/Article/details/goitbegtp.sHtML

[U100] JS：DOM 查询
来源：http://blog.fanxiaobao.xyz/Article/details/giuhwjpnw.sHtML

document.querySelector(".item")
来源：http://www.share.fanxiaobao.xyz/Article/details/greivahoj.sHtML

[U101] JS：classList 操作
来源：http://3g.fanxiaobao.xyz/Article/details/geedjygad.sHtML

el.classList.toggle("active")
来源：http://mobile.fanxiaobao.xyz/Article/details/gikyqqlhd.sHtML

[U102] JS：本地存储
来源：http://blog.fanxiaobao.xyz/Article/details/gkvmlwair.sHtML

localStorage.setItem("k", JSON.stringify(v))
来源：http://read.share.fanxiaobao.xyz/Article/details/gckmhroda.sHtML

[U103] JS：定时器
来源：http://m.share.fanxiaobao.xyz/Article/details/gtqfsvzlq.sHtML

setTimeout(fn, 1000);  setInterval(fn, 1000);
来源：http://mobile.fanxiaobao.xyz/Article/details/gyyyzqwbb.sHtML

[U104] JS：防抖
来源：http://baike.fanxiaobao.xyz/Article/details/gpdympipt.sHtML

const debounce = (fn, ms) => { let t; return (...a) => { clearTimeout(t); t = setTimeout(() => fn(...a), ms); }; };
来源：http://blog.fanxiaobao.xyz/Article/details/glwunxunk.sHtML

[U105] JS：节流
来源：http://blog.fanxiaobao.xyz/Article/details/gegcqqsmg.sHtML

const throttle = (fn, ms) => { let last = 0; return (...a) => { const n = Date.now(); if (n - last >= ms) { last = n; fn(...a); } }; };
来源：http://wap.fanxiaobao.xyz/Article/details/gyxptzlmg.sHtML

[U106] JS：日期格式化
来源：http://mobile.fanxiaobao.xyz/Article/details/glfbuizxk.sHtML

new Intl.DateTimeFormat("zh-CN", { dateStyle: "medium" }).format(new Date())
来源：http://mobile.fanxiaobao.xyz/Article/details/gpltlztau.sHtML

[U107] JS：数字千分位
来源：http://www.share.fanxiaobao.xyz/Article/details/gbonfuypr.sHtML

new Intl.NumberFormat("en-US").format(1234567)
来源：http://m.share.fanxiaobao.xyz/Article/details/gvbdfrwwe.sHtML

[U108] JS：随机整数
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gzrawvzbw.sHtML

Math.floor(Math.random() * (max - min + 1)) + min
来源：http://blog.fanxiaobao.xyz/Article/details/gonfgzdny.sHtML

[U109] JS：数组分组
来源：http://baike.fanxiaobao.xyz/Article/details/gdqumwfrz.sHtML

Object.groupBy(arr, x => x.type)
来源：http://www.blog.fanxiaobao.xyz/Article/details/gxacusvcc.sHtML

[U110] JS：数组分块
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gksinpmpx.sHtML

arr.reduce((acc, x, i) => (i % size ? acc : [...acc, arr.slice(i, i + size)]), [])
来源：http://www.share.fanxiaobao.xyz/Article/details/ggjwlamif.sHtML

[U111] JS：对象转 Map
来源：http://www.blog.fanxiaobao.xyz/Article/details/gcyeztuci.sHtML

new Map(Object.entries(obj))
来源：http://read.share.fanxiaobao.xyz/Article/details/guckjxenv.sHtML

[U112] JS：字符串补位
来源：http://read.share.fanxiaobao.xyz/Article/details/gniivwbvv.sHtML

"7".padStart(3, "0")
来源：http://www.blog.fanxiaobao.xyz/Article/details/gkmynaetc.sHtML

[U113] JS：正则替换全部
来源：http://baike.fanxiaobao.xyz/Article/details/gcdnovpoy.sHtML

s.replaceAll("a", "b")
来源：http://3g.fanxiaobao.xyz/Article/details/gsdygxhsm.sHtML

[U114] JS：JSON 深比较
来源：http://www.blog.fanxiaobao.xyz/Article/details/gwwarqynm.sHtML

JSON.stringify(a) === JSON.stringify(b)
来源：http://mobile.fanxiaobao.xyz/Article/details/grxuvsokq.sHtML

[U115] JS：生成 UUID
来源：http://mobile.fanxiaobao.xyz/Article/details/gzkjqrskn.sHtML

crypto.randomUUID()
来源：http://blog.fanxiaobao.xyz/Article/details/gycwjuipu.sHtML

[U116] JS：类型检查（JSDoc）
来源：http://www.blog.fanxiaobao.xyz/Article/details/gfcymbace.sHtML

/** @param {string} name */ function f(name) {}
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gnytpjxez.sHtML

[U117] JS：单元测试
来源：http://3g.fanxiaobao.xyz/Article/details/gkugufkoi.sHtML

npm i -D vitest;  npx vitest
来源：http://baike.fanxiaobao.xyz/Article/details/gofcidffj.sHtML

[U118] JS：开发服务器
来源：http://www.share.fanxiaobao.xyz/Article/details/guepfmwmr.sHtML

npm i -D vite;  npx vite
来源：http://wap.fanxiaobao.xyz/Article/details/gcgqqnktk.sHtML

[U119] JS：生产构建
来源：http://m.share.fanxiaobao.xyz/Article/details/gstuptubz.sHtML

npx vite build
来源：http://www.blog.fanxiaobao.xyz/Article/details/gnqtmuhnx.sHtML

[U120] JS：读取环境变量（Vite）
来源：http://baike.fanxiaobao.xyz/Article/details/gvbassuwu.sHtML

import.meta.env.VITE_API_URL
来源：http://3g.fanxiaobao.xyz/Article/details/gdomzrinl.sHtML

================================================================================
来源：http://read.share.fanxiaobao.xyz/Article/details/gxmkcceas.sHtML

统计汇总
来源：http://www.share.fanxiaobao.xyz/Article/details/gftsseuro.sHtML

================================================================================
来源：http://baike.fanxiaobao.xyz/Article/details/gxcuaydbx.sHtML

按语言统计（条）：
来源：http://baike.fanxiaobao.xyz/Article/details/gkoynmglw.sHtML

Python ......... 252
来源：http://www.blog.fanxiaobao.xyz/Article/details/gzublohhn.sHtML

PHP ............ 252
来源：http://www.blog.fanxiaobao.xyz/Article/details/gwfnmarwu.sHtML

JavaScript ..... 252
来源：http://www.blog.fanxiaobao.xyz/Article/details/gagcsfeys.sHtML

TypeScript ..... 212
来源：http://baike.fanxiaobao.xyz/Article/details/gvdkahvfr.sHtML

Java ........... 212
来源：http://read.share.fanxiaobao.xyz/Article/details/grbvrvnyb.sHtML

Go ............. 212
来源：http://blog.fanxiaobao.xyz/Article/details/ggyggszxt.sHtML

Ruby ........... 212
来源：http://3g.fanxiaobao.xyz/Article/details/gcjcctqjv.sHtML

C# ............. 212
来源：http://baike.fanxiaobao.xyz/Article/details/gbjxzazey.sHtML

C .............. 30
来源：http://m.share.fanxiaobao.xyz/Article/details/gvsdsptuv.sHtML

C++ ............ 30
来源：http://m.share.fanxiaobao.xyz/Article/details/gubdqezbc.sHtML

SQL ............ 90
来源：http://www.m.share.fanxiaobao.xyz/Article/details/geoszhilh.sHtML

Bash ........... 80
来源：http://baike.fanxiaobao.xyz/Article/details/gdidtosaw.sHtML

Kotlin ......... 15
来源：http://read.share.fanxiaobao.xyz/Article/details/ggcnoplji.sHtML

Swift .......... 15
来源：http://blog.fanxiaobao.xyz/Article/details/gtjnxpczo.sHtML

Lua ............ 10
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gugjlyapv.sHtML

Perl ........... 10
来源：http://read.share.fanxiaobao.xyz/Article/details/gcgybctks.sHtML

Scala .......... 10
来源：http://blog.fanxiaobao.xyz/Article/details/gazlnyhnp.sHtML

------------------------------------
来源：http://blog.fanxiaobao.xyz/Article/details/gdgnvmatb.sHtML

合计 ........... 2106 条
来源：http://3g.fanxiaobao.xyz/Article/details/gdayocrqj.sHtML

按章节统计：
来源：http://read.share.fanxiaobao.xyz/Article/details/gsgyrzhnz.sHtML

A 基础语法与类型       26 个任务 × 8 语言 =  208
来源：http://read.share.fanxiaobao.xyz/Article/details/gxtqowknz.sHtML

B 流程控制             16 个任务 × 8 语言 =  128
来源：http://wap.fanxiaobao.xyz/Article/details/gyyxsnvov.sHtML

C 函数与作用域         16 个任务 × 8 语言 =  128
来源：http://blog.fanxiaobao.xyz/Article/details/gochjdegl.sHtML

D 数组 / 列表 / 集合   26 个任务 × 8 语言 =  208
来源：http://www.blog.fanxiaobao.xyz/Article/details/gotdlfeqy.sHtML

E 字符串处理           22 个任务 × 8 语言 =  176
来源：http://baike.fanxiaobao.xyz/Article/details/gqzvbmprd.sHtML

F 文件与目录           12 个任务 × 8 语言 =   96
来源：http://baike.fanxiaobao.xyz/Article/details/gnfdfmazq.sHtML

G 面向对象             16 个任务 × 8 语言 =  128
来源：http://wap.fanxiaobao.xyz/Article/details/glrlmdqsm.sHtML

H 异常与错误处理       10 个任务 × 8 语言 =   80
来源：http://www.share.fanxiaobao.xyz/Article/details/gysxmlyoo.sHtML

I 正则表达式            8 个任务 × 8 语言 =   64
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gjjtolnhz.sHtML

J 日期与时间           10 个任务 × 8 语言 =   80
来源：http://www.share.fanxiaobao.xyz/Article/details/gbksdqnbz.sHtML

K JSON 与序列化         8 个任务 × 8 语言 =   64
来源：http://read.share.fanxiaobao.xyz/Article/details/gdzvdlymj.sHtML

L 网络请求              8 个任务 × 8 语言 =   64
来源：http://mobile.fanxiaobao.xyz/Article/details/gbmutmdbd.sHtML

M 命令行 / 进程         8 个任务 × 8 语言 =   64
来源：http://baike.fanxiaobao.xyz/Article/details/gibljcuyt.sHtML

N 数据结构与算法       12 个任务 × 8 语言 =   96
来源：http://baike.fanxiaobao.xyz/Article/details/gutejurum.sHtML

O 并发与异步            6 个任务 × 8 语言 =   48
来源：http://3g.fanxiaobao.xyz/Article/details/gvgekwfmq.sHtML

P 常用工具函数          8 个任务 × 8 语言 =   64
来源：http://m.share.fanxiaobao.xyz/Article/details/gbnypncle.sHtML

Q SQL 专题                              90
来源：http://read.share.fanxiaobao.xyz/Article/details/gcaqjxlcg.sHtML

R Bash 专题                             80
来源：http://read.share.fanxiaobao.xyz/Article/details/gjwuybeha.sHtML

S C / C++ 专题                          60
来源：http://www.blog.fanxiaobao.xyz/Article/details/gurxnexvo.sHtML

T 其他语言补充                          60
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gpuvnwscl.sHtML

U 高频实用片段                         120
来源：http://wap.fanxiaobao.xyz/Article/details/gpcanjljt.sHtML

------------------------------------
来源：http://baike.fanxiaobao.xyz/Article/details/gqjfdahzg.sHtML

合计                                  2106 条
来源：http://baike.fanxiaobao.xyz/Article/details/gndbcnmgg.sHtML

--------------------------------------------------------------------------------
来源：http://blog.fanxiaobao.xyz/Article/details/gpzpshviv.sHtML

使用提醒
来源：http://3g.fanxiaobao.xyz/Article/details/gkrilcdoi.sHtML

--------------------------------------------------------------------------------
来源：http://mobile.fanxiaobao.xyz/Article/details/gksqwixkd.sHtML

1. 示例追求"最小可用"，正式项目中请补齐导入、错误处理与边界判断。
来源：http://baike.fanxiaobao.xyz/Article/details/glysagins.sHtML

2. 涉及文件、网络、数据库的示例，注意资源释放与异常捕获。
来源：http://www.blog.fanxiaobao.xyz/Article/details/gzjtwuviu.sHtML

3. 语言版本差异较大（如 Python 3.10 的 match、Java 17 的 record/switch 箭头），
来源：http://read.share.fanxiaobao.xyz/Article/details/gzonjjhng.sHtML

在旧版本上使用前请先确认语法支持情况。
来源：http://wap.fanxiaobao.xyz/Article/details/gcannsgof.sHtML

4. 标注"手写"的条目是因为该语言缺少对应内置能力，实际项目中可引入成熟库。
来源：http://mobile.fanxiaobao.xyz/Article/details/gajesgbsj.sHtML

—— 文件结束 ——
来源：http://read.share.fanxiaobao.xyz/Article/details/gkvbuxugq.sHtML

================================================================================
来源：http://www.share.fanxiaobao.xyz/Article/details/guvhcnbom.sHtML

程序语言常见例子速查手册（2024 版）
来源：http://www.blog.fanxiaobao.xyz/Article/details/gzexfskvl.sHtML

Common Programming Examples Cheat Book
来源：http://www.blog.fanxiaobao.xyz/Article/details/grtphwycg.sHtML

================================================================================
来源：http://read.share.fanxiaobao.xyz/Article/details/gwygemqsw.sHtML

【收录内容】
来源：http://blog.fanxiaobao.xyz/Article/details/gbbgruoql.sHtML

覆盖 12 种语言 / 语法与常见 API：
来源：http://www.share.fanxiaobao.xyz/Article/details/griaultpm.sHtML

Python · PHP · JavaScript · TypeScript · Java · Go · Ruby · C#
来源：http://www.share.fanxiaobao.xyz/Article/details/gdsgqignq.sHtML

SQL · Bash · C · C++
来源：http://www.m.share.fanxiaobao.xyz/Article/details/ggroqxjwh.sHtML

按「任务」分组：每个任务下按语言各给出一条最小可用示例。
来源：http://www.blog.fanxiaobao.xyz/Article/details/gynkdlwvv.sHtML

【使用说明】
来源：http://baike.fanxiaobao.xyz/Article/details/gnunnzyvv.sHtML

1. 每个任务形如 "[编号] 任务名"，下面每行以语言标记开头：
来源：http://3g.fanxiaobao.xyz/Article/details/gxffggyia.sHtML

Py:    Python        PHP:   PHP           JS:    JavaScript
来源：http://www.share.fanxiaobao.xyz/Article/details/gbfgyktup.sHtML

TS:    TypeScript    Java:  Java          Go:    Go
来源：http://m.share.fanxiaobao.xyz/Article/details/gdybmyfka.sHtML

Ruby:  Ruby          C#:    C#            SQL:   SQL
来源：http://mobile.fanxiaobao.xyz/Article/details/gxrwnvkub.sHtML

Bash:  Shell         C:     C             C++:   C++
来源：http://read.share.fanxiaobao.xyz/Article/details/gxntkylnf.sHtML

2. 示例只展示核心写法，刻意省略 import / require / include / using 等样板代码。
来源：http://read.share.fanxiaobao.xyz/Article/details/gngdcmtcc.sHtML

需要完整可运行文件时，请自行补齐当前语言的导入语句。
来源：http://3g.fanxiaobao.xyz/Article/details/gnpymmysb.sHtML

3. 语法基准：Python 3.10+ / PHP 8.1+ / ES2020+ / TypeScript 5 / Java 17 /
来源：http://wap.fanxiaobao.xyz/Article/details/gdbcasxfq.sHtML

Go 1.21+ / Ruby 3.x / C# 10+ / C17 / C++17。
来源：http://www.blog.fanxiaobao.xyz/Article/details/gmkxweowr.sHtML

4. 检索建议：用编辑器或浏览器 Ctrl+F 搜关键词，如 "排序" "读取文件" "正则"。
来源：http://m.share.fanxiaobao.xyz/Article/details/gfclqjoiu.sHtML

5. 标记为 "// 无" 表示该语言没有对应的一等语法，需用替代写法（示例给出替代方案）。
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gpdwcrjik.sHtML

6. 符号 "⏎" 表示代码在此处换行（主要用于 Python 等强制缩进、无法压成一行的结构）。
来源：http://blog.fanxiaobao.xyz/Article/details/ghflitvwu.sHtML

【文件统计】
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gpkonmrmb.sHtML

语言示例共 2106 条，分布见本文末尾的「统计汇总」。
来源：http://blog.fanxiaobao.xyz/Article/details/gfvzvqqyl.sHtML

--------------------------------------------------------------------------------
来源：http://3g.fanxiaobao.xyz/Article/details/gdepnojox.sHtML

目  录
来源：http://baike.fanxiaobao.xyz/Article/details/gawqmlafo.sHtML

--------------------------------------------------------------------------------
来源：http://mobile.fanxiaobao.xyz/Article/details/gvjqevkpd.sHtML

A. 基础语法与类型              （第 1 节，26 个任务，208 条）
来源：http://baike.fanxiaobao.xyz/Article/details/gxevfjdgi.sHtML

B. 流程控制                    （第 2 节，16 个任务，128 条）
来源：http://3g.fanxiaobao.xyz/Article/details/gdnhrjrhb.sHtML

C. 函数与作用域                （第 3 节，16 个任务，128 条）
来源：http://m.share.fanxiaobao.xyz/Article/details/gieqijzcc.sHtML

D. 数组 / 列表 / 集合          （第 4 节，26 个任务，208 条）
来源：http://3g.fanxiaobao.xyz/Article/details/guvhkyfln.sHtML

E. 字符串处理                  （第 5 节，22 个任务，176 条）
来源：http://wap.fanxiaobao.xyz/Article/details/grnoxosux.sHtML

F. 文件与目录                  （第 6 节，12 个任务，96 条）
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gowmlrfoj.sHtML

G. 面向对象                    （第 7 节，16 个任务，128 条）
来源：http://m.share.fanxiaobao.xyz/Article/details/gvzpauhag.sHtML

H. 异常与错误处理              （第 8 节，10 个任务，80 条）
来源：http://read.share.fanxiaobao.xyz/Article/details/gyxgyjyij.sHtML

I. 正则表达式                  （第 9 节，8 个任务，64 条）
来源：http://baike.fanxiaobao.xyz/Article/details/gssznexqm.sHtML


<!-- 参考信息 -->