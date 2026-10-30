代发 wailian999

[U15] Py：高精度计时
来源：http://www.share.fanxiaobao.xyz/Article/details/godaqksym.sHtML

t = time.perf_counter()
来源：http://www.share.fanxiaobao.xyz/Article/details/gnaezdwxb.sHtML

[U16] Py：命令行参数解析
来源：http://m.share.fanxiaobao.xyz/Article/details/gvhxutwmx.sHtML

ap = argparse.ArgumentParser();  ap.add_argument("--name");  args = ap.parse_args()
来源：http://baike.fanxiaobao.xyz/Article/details/gjosoxusx.sHtML

[U17] Py：初始化日志
来源：http://www.share.fanxiaobao.xyz/Article/details/gdtrphipq.sHtML

logging.basicConfig(level=logging.INFO)
来源：http://m.share.fanxiaobao.xyz/Article/details/gbtcgusrt.sHtML

[U18] Py：预编译正则
来源：http://wap.fanxiaobao.xyz/Article/details/gvxrutfje.sHtML

pat = re.compile(r"\d+")
来源：http://3g.fanxiaobao.xyz/Article/details/geofvyrdn.sHtML

[U19] Py：正则替换带回调
来源：http://www.share.fanxiaobao.xyz/Article/details/gojvxbeqf.sHtML

re.sub(r"\d+", lambda m: str(int(m.group()) * 2), s)
来源：http://baike.fanxiaobao.xyz/Article/details/grpwxjkzb.sHtML

[U20] Py：缓存函数结果
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gtjgageei.sHtML

@functools.lru_cache(maxsize=None)
来源：http://baike.fanxiaobao.xyz/Article/details/gmmgwcfmr.sHtML

[U21] Py：自定义上下文管理器
来源：http://read.share.fanxiaobao.xyz/Article/details/gkhjavkmu.sHtML

@contextlib.contextmanager
来源：http://www.m.share.fanxiaobao.xyz/Article/details/guffrasgf.sHtML

[U22] Py：矩阵转置
来源：http://m.share.fanxiaobao.xyz/Article/details/gzamccevs.sHtML

list(zip(*m))
来源：http://blog.fanxiaobao.xyz/Article/details/glcfwiwqb.sHtML

[U23] Py：分块读取大文件
来源：http://m.share.fanxiaobao.xyz/Article/details/gzujctznl.sHtML

for chunk in iter(lambda: f.read(8192), b""):
来源：http://wap.fanxiaobao.xyz/Article/details/gsggupocb.sHtML

[U24] Py：路径操作
来源：http://mobile.fanxiaobao.xyz/Article/details/gxhumttru.sHtML

Path("a/b.txt").parent.mkdir(parents=True, exist_ok=True)
来源：http://wap.fanxiaobao.xyz/Article/details/ggohrjuyv.sHtML

[U25] Py：CSV 按字典读
来源：http://baike.fanxiaobao.xyz/Article/details/gjcilkzws.sHtML

csv.DictReader(f)
来源：http://read.share.fanxiaobao.xyz/Article/details/gbbqarhnn.sHtML

[U26] Py：并发下载
来源：http://read.share.fanxiaobao.xyz/Article/details/gwtaybleq.sHtML

ThreadPoolExecutor(max_workers=8).map(fetch, urls)
来源：http://mobile.fanxiaobao.xyz/Article/details/glayzjjme.sHtML

[U27] Py：异步 HTTP
来源：http://baike.fanxiaobao.xyz/Article/details/grrxgnhnd.sHtML

aiohttp.ClientSession() 配合 async with
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gtdhkusiv.sHtML

[U28] Py：类型别名
来源：http://read.share.fanxiaobao.xyz/Article/details/gtzdevuza.sHtML

UserId = int
来源：http://m.share.fanxiaobao.xyz/Article/details/gtgvpavyx.sHtML

[U29] Py：属性校验
来源：http://mobile.fanxiaobao.xyz/Article/details/ggzvzcggi.sHtML

@property 与 @x.setter 配合
来源：http://baike.fanxiaobao.xyz/Article/details/gvjvallfh.sHtML

[U30] Py：数据类
来源：http://m.share.fanxiaobao.xyz/Article/details/gijvjlfyr.sHtML

@dataclass(slots=True)
来源：http://read.share.fanxiaobao.xyz/Article/details/gevxfykxk.sHtML

[U31] Py：单测
来源：http://m.share.fanxiaobao.xyz/Article/details/giduenscb.sHtML

python -m pytest -q
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gedbwdrdb.sHtML

[U32] Py：代码格式化
来源：http://baike.fanxiaobao.xyz/Article/details/gqfkcqztw.sHtML

ruff format . && ruff check --fix .
来源：http://3g.fanxiaobao.xyz/Article/details/gomimlkoc.sHtML

[U33] Py：打包发布
来源：http://www.share.fanxiaobao.xyz/Article/details/grnnmifbx.sHtML

python -m build  （依赖 pyproject.toml）
来源：http://3g.fanxiaobao.xyz/Article/details/girksdjqi.sHtML

[U34] Py：判断编码
来源：http://blog.fanxiaobao.xyz/Article/details/glqlbvzmy.sHtML

chardet.detect(raw)
来源：http://www.share.fanxiaobao.xyz/Article/details/gyknazota.sHtML

[U35] Py：发送邮件
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gifxezesw.sHtML

smtplib.SMTP_SSL(...).send_message(msg)
来源：http://mobile.fanxiaobao.xyz/Article/details/gxhewxmud.sHtML

[U36] Py：定时任务
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gqkrzdupq.sHtML

schedule.every(10).minutes.do(job)
来源：http://3g.fanxiaobao.xyz/Article/details/ghdmrhpnv.sHtML

[U37] Py：读写 Excel
来源：http://3g.fanxiaobao.xyz/Article/details/gmpisbmab.sHtML

pandas.read_excel / DataFrame.to_excel
来源：http://baike.fanxiaobao.xyz/Article/details/gazplhxbk.sHtML

[U38] Py：获取脚本所在目录
来源：http://mobile.fanxiaobao.xyz/Article/details/gzsymnxym.sHtML

Path(__file__).resolve().parent
来源：http://3g.fanxiaobao.xyz/Article/details/gqlkkgixv.sHtML

[U39] Py：判断是否在交互环境
来源：http://3g.fanxiaobao.xyz/Article/details/gbttkfjto.sHtML

sys.stdout.isatty()
来源：http://read.share.fanxiaobao.xyz/Article/details/gvvuhrzps.sHtML

[U40] Py：打印到标准错误
来源：http://www.blog.fanxiaobao.xyz/Article/details/gbxxqvsyb.sHtML

print("err", file=sys.stderr)
来源：http://wap.fanxiaobao.xyz/Article/details/gqankojld.sHtML

[U41] PHP：初始化 Composer 项目
来源：http://www.share.fanxiaobao.xyz/Article/details/gnzbjogjg.sHtML

composer init;  composer require guzzlehttp/guzzle
来源：http://mobile.fanxiaobao.xyz/Article/details/gwzcpsnei.sHtML

[U42] PHP：PSR-4 自动加载
来源：http://baike.fanxiaobao.xyz/Article/details/gnfyrjulh.sHtML

"autoload": { "psr-4": { "App\\": "src/" } }
来源：http://www.blog.fanxiaobao.xyz/Article/details/gcqrruxpn.sHtML

[U43] PHP：声明命名空间
来源：http://3g.fanxiaobao.xyz/Article/details/gqbqldgtf.sHtML

namespace App\Http;
来源：http://wap.fanxiaobao.xyz/Article/details/ghucgicsp.sHtML

[U44] PHP：开启严格类型
来源：http://blog.fanxiaobao.xyz/Article/details/gqzpduest.sHtML

declare(strict_types=1);
来源：http://mobile.fanxiaobao.xyz/Article/details/ghcdofhuk.sHtML

[U45] PHP：类型声明与返回类型
来源：http://blog.fanxiaobao.xyz/Article/details/gjxjtzcmk.sHtML

function add(int $a, int $b): int { return $a + $b; }
来源：http://wap.fanxiaobao.xyz/Article/details/gcvtkwvhb.sHtML

[U46] PHP：可空类型
来源：http://m.share.fanxiaobao.xyz/Article/details/glztweznw.sHtML

?string $name = null
来源：http://m.share.fanxiaobao.xyz/Article/details/gwlpxyhnx.sHtML

[U47] PHP：联合类型
来源：http://mobile.fanxiaobao.xyz/Article/details/ghyjwglgf.sHtML

int|string $id
来源：http://www.share.fanxiaobao.xyz/Article/details/gefksczgb.sHtML

[U48] PHP：纯枚举
来源：http://wap.fanxiaobao.xyz/Article/details/gyyfwmrwf.sHtML

enum Status: string { case Active = "active"; case Off = "off"; }
来源：http://www.blog.fanxiaobao.xyz/Article/details/gbdlcjois.sHtML

[U49] PHP：只读属性
来源：http://www.share.fanxiaobao.xyz/Article/details/gabuofcjx.sHtML

public readonly string $name
来源：http://3g.fanxiaobao.xyz/Article/details/ghepbetlo.sHtML

[U50] PHP：构造器属性提升
来源：http://mobile.fanxiaobao.xyz/Article/details/glqpwocmf.sHtML

public function __construct(private int $id) {}
来源：http://blog.fanxiaobao.xyz/Article/details/gvpwtduio.sHtML

[U51] PHP：数组解构
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gfvesohqh.sHtML

[$a, $b] = $arr;
来源：http://read.share.fanxiaobao.xyz/Article/details/geixiyfzl.sHtML

[U52] PHP：箭头函数
来源：http://baike.fanxiaobao.xyz/Article/details/gzhudvroz.sHtML

$double = fn($x) => $x * 2;
来源：http://www.m.share.fanxiaobao.xyz/Article/details/ggjkqvkdh.sHtML

[U53] PHP：空合并运算符
来源：http://m.share.fanxiaobao.xyz/Article/details/gteykhkqn.sHtML

$v = $a ?? $b ?? "default";
来源：http://read.share.fanxiaobao.xyz/Article/details/goytmfzjs.sHtML

[U54] PHP：空安全调用
来源：http://www.share.fanxiaobao.xyz/Article/details/gcdyabrns.sHtML

$obj?->method()
来源：http://blog.fanxiaobao.xyz/Article/details/gtrsbttog.sHtML

[U55] PHP：match 表达式
来源：http://blog.fanxiaobao.xyz/Article/details/gqocemloq.sHtML

$s = match($x) { 1 => "一", default => "其他" };
来源：http://baike.fanxiaobao.xyz/Article/details/ggbuudehw.sHtML

[U56] PHP：命名参数
来源：http://baike.fanxiaobao.xyz/Article/details/gtzqukwry.sHtML

f(a: 1, b: 2)
来源：http://www.share.fanxiaobao.xyz/Article/details/geczaaawv.sHtML

[U57] PHP：字符串插值
来源：http://blog.fanxiaobao.xyz/Article/details/gbsdvzwmo.sHtML

"值: {$a}"
来源：http://read.share.fanxiaobao.xyz/Article/details/getkduhxx.sHtML

[U58] PHP：数组三件套
来源：http://baike.fanxiaobao.xyz/Article/details/gprscezry.sHtML

array_map($f, $a);  array_filter($a, $f);  array_reduce($a, $f, 0);
来源：http://blog.fanxiaobao.xyz/Article/details/gsnstimhm.sHtML

[U59] PHP：自定义排序
来源：http://www.share.fanxiaobao.xyz/Article/details/gjvgiikzn.sHtML

usort($arr, fn($a, $b) => $a["age"] <=> $b["age"]);
来源：http://wap.fanxiaobao.xyz/Article/details/gpkahquuy.sHtML

[U60] PHP：JSON 编解码
来源：http://www.share.fanxiaobao.xyz/Article/details/grlnqlntr.sHtML

json_encode($d, JSON_UNESCAPED_UNICODE);  json_decode($s, true);
来源：http://www.share.fanxiaobao.xyz/Article/details/gcrrpjlkj.sHtML

[U61] PHP：正则
来源：http://www.blog.fanxiaobao.xyz/Article/details/glgvrcvxb.sHtML

preg_match('/(\d+)/', $s, $m);  preg_replace('/\d+/', '#', $s);
来源：http://mobile.fanxiaobao.xyz/Article/details/gehjxuega.sHtML

[U62] PHP：日期对象
来源：http://3g.fanxiaobao.xyz/Article/details/gyaktfkyf.sHtML

(new DateTimeImmutable())->format("Y-m-d");
来源：http://mobile.fanxiaobao.xyz/Article/details/gvbhhsxen.sHtML

[U63] PHP：文件读写
来源：http://baike.fanxiaobao.xyz/Article/details/ghkxzufob.sHtML

file_get_contents($f);  file_put_contents($f, $data);
来源：http://www.share.fanxiaobao.xyz/Article/details/gdphemcvy.sHtML

[U64] PHP：目录遍历
来源：http://m.share.fanxiaobao.xyz/Article/details/gdscotfro.sHtML

glob("dir/*.php");  scandir("dir");
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gdqhmsozl.sHtML

[U65] PHP：会话
来源：http://3g.fanxiaobao.xyz/Article/details/gqgmvcxft.sHtML

session_start();  $_SESSION["uid"] = 1;
来源：http://www.share.fanxiaobao.xyz/Article/details/gbxtnulik.sHtML

[U66] PHP：设置 Cookie
来源：http://m.share.fanxiaobao.xyz/Article/details/gjwoizpoh.sHtML

setcookie("token", $v, ["httponly" => true, "samesite" => "Lax"]);
来源：http://read.share.fanxiaobao.xyz/Article/details/ghrguqabo.sHtML

[U67] PHP：处理文件上传
来源：http://blog.fanxiaobao.xyz/Article/details/gffahcdzb.sHtML

$_FILES["file"]["tmp_name"] 与 move_uploaded_file()
来源：http://3g.fanxiaobao.xyz/Article/details/gmukgwrlm.sHtML

[U68] PHP：PDO 连接
来源：http://3g.fanxiaobao.xyz/Article/details/gznmxiyni.sHtML

$pdo = new PDO("mysql:host=localhost;dbname=app", "root", "");
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gfwrjeptc.sHtML

[U69] PHP：PDO 预处理
来源：http://mobile.fanxiaobao.xyz/Article/details/gyldsbtbj.sHtML

$stmt = $pdo->prepare("SELECT * FROM users WHERE id = ?");  $stmt->execute([$id]);
来源：http://3g.fanxiaobao.xyz/Article/details/gljihocjq.sHtML

[U70] PHP：PDO 事务
来源：http://www.blog.fanxiaobao.xyz/Article/details/gnuxyeoaw.sHtML

$pdo->beginTransaction();  $pdo->commit();  $pdo->rollBack();
来源：http://wap.fanxiaobao.xyz/Article/details/gnnxdphtg.sHtML

[U71] PHP：抛出异常
来源：http://www.blog.fanxiaobao.xyz/Article/details/gdvnuafxi.sHtML

throw new RuntimeException("失败", 500);
来源：http://www.blog.fanxiaobao.xyz/Article/details/gwiuouyni.sHtML

[U72] PHP：写错误日志
来源：http://mobile.fanxiaobao.xyz/Article/details/gvibbnohu.sHtML

error_log("失败: " . $e->getMessage());
来源：http://wap.fanxiaobao.xyz/Article/details/gdhprxcbi.sHtML

[U73] PHP：读取 ini 配置
来源：http://baike.fanxiaobao.xyz/Article/details/grjsgwzsa.sHtML

parse_ini_file("config.ini", true)
来源：http://m.share.fanxiaobao.xyz/Article/details/gezvgeffl.sHtML

[U74] PHP：读取环境变量
来源：http://3g.fanxiaobao.xyz/Article/details/gxapsdecw.sHtML

getenv("APP_ENV") ?: "production"
来源：http://wap.fanxiaobao.xyz/Article/details/getteebpw.sHtML

[U75] PHP：依赖注入
来源：http://www.share.fanxiaobao.xyz/Article/details/gtrvzshgl.sHtML

composer require psr/container
来源：http://baike.fanxiaobao.xyz/Article/details/glmjvwnek.sHtML

[U76] PHP：简单路由
来源：http://blog.fanxiaobao.xyz/Article/details/ggcxgpbou.sHtML

$path = parse_url($_SERVER["REQUEST_URI"], PHP_URL_PATH);
来源：http://wap.fanxiaobao.xyz/Article/details/gdjnklyjz.sHtML

[U77] PHP：模板渲染
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gqcpjlugb.sHtML

composer require twig/twig
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gpvdysrbl.sHtML

[U78] PHP：单元测试
来源：http://3g.fanxiaobao.xyz/Article/details/gtukyaqbg.sHtML

composer require --dev phpunit/phpunit
来源：http://m.share.fanxiaobao.xyz/Article/details/gbjptwhmr.sHtML

[U79] PHP：静态分析
来源：http://m.share.fanxiaobao.xyz/Article/details/gzxfgpguo.sHtML

composer require --dev phpstan/phpstan
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gantprdza.sHtML

[U80] PHP：代码规范修复
来源：http://read.share.fanxiaobao.xyz/Article/details/gwpecihof.sHtML

composer require --dev friendsofphp/php-cs-fixer
来源：http://mobile.fanxiaobao.xyz/Article/details/gocdzpwih.sHtML

[U81] JS：初始化项目
来源：http://www.blog.fanxiaobao.xyz/Article/details/gqllaviql.sHtML

npm init -y;  npm i express
来源：http://read.share.fanxiaobao.xyz/Article/details/gzgrfaemc.sHtML

[U82] JS：package.json 脚本
来源：http://www.blog.fanxiaobao.xyz/Article/details/gslljdbay.sHtML

"scripts": { "dev": "vite", "build": "vite build" }
来源：http://www.blog.fanxiaobao.xyz/Article/details/gkoxpkslw.sHtML

[U83] JS：ES Module 导入导出
来源：http://m.share.fanxiaobao.xyz/Article/details/gsetyvxgt.sHtML

export const a = 1;  import { a } from "./m.js";
来源：http://www.blog.fanxiaobao.xyz/Article/details/gtdjunxub.sHtML

[U84] JS：CommonJS 写法
来源：http://m.share.fanxiaobao.xyz/Article/details/gumuzukzi.sHtML

module.exports = { a };  const { a } = require("./m");
来源：http://www.share.fanxiaobao.xyz/Article/details/gvpdhedkg.sHtML

[U85] JS：可选链
来源：http://www.share.fanxiaobao.xyz/Article/details/gtoikjbzi.sHtML

a?.b?.c
来源：http://wap.fanxiaobao.xyz/Article/details/gtnrqjxyo.sHtML

[U86] JS：空值合并
来源：http://wap.fanxiaobao.xyz/Article/details/gausasgih.sHtML

a ?? b
来源：http://m.share.fanxiaobao.xyz/Article/details/guwdjikgk.sHtML

[U87] JS：解构默认值
来源：http://www.share.fanxiaobao.xyz/Article/details/ghmjtyqoz.sHtML

const { a = 1, b = 2 } = obj;
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gcyztyybj.sHtML

[U88] JS：对象展开合并
来源：http://blog.fanxiaobao.xyz/Article/details/gscfwqocx.sHtML

{ ...a, ...b }
来源：http://mobile.fanxiaobao.xyz/Article/details/gspefyujl.sHtML

[U89] JS：数组去重
来源：http://blog.fanxiaobao.xyz/Article/details/gnyymuidi.sHtML

[...new Set(arr)]
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gfzjjmirb.sHtML

[U90] JS：数字数组排序
来源：http://wap.fanxiaobao.xyz/Article/details/gyqelyhma.sHtML

[...arr].sort((a, b) => a - b)
来源：http://baike.fanxiaobao.xyz/Article/details/gjnjwxggw.sHtML

[U91] JS：对象键值遍历
来源：http://www.share.fanxiaobao.xyz/Article/details/gsuxisvfo.sHtML

Object.entries(obj).forEach(([k, v]) => {});
来源：http://mobile.fanxiaobao.xyz/Article/details/glmpiqmcm.sHtML

[U92] JS：深拷贝
来源：http://www.m.share.fanxiaobao.xyz/Article/details/goxcbgmpk.sHtML

structuredClone(obj)
来源：http://www.blog.fanxiaobao.xyz/Article/details/gipibiryn.sHtML

[U93] JS：模板字符串
来源：http://read.share.fanxiaobao.xyz/Article/details/gmyjgjkhc.sHtML

`共 ${n} 条`
来源：http://www.share.fanxiaobao.xyz/Article/details/guhpnspli.sHtML

[U94] JS：箭头函数
来源：http://blog.fanxiaobao.xyz/Article/details/ggznyridm.sHtML

const double = x => x * 2;
来源：http://baike.fanxiaobao.xyz/Article/details/gsdvsafbs.sHtML

[U95] JS：Promise 包装
来源：http://baike.fanxiaobao.xyz/Article/details/gxbirwsum.sHtML

new Promise((resolve, reject) => {})
来源：http://wap.fanxiaobao.xyz/Article/details/gzhigaxzp.sHtML

[U96] JS：async/await 与异常
来源：http://mobile.fanxiaobao.xyz/Article/details/gfxbvwvnr.sHtML

try { const d = await f(); } catch (e) { console.error(e); }
来源：http://wap.fanxiaobao.xyz/Article/details/gvrxzxhzw.sHtML

[U97] JS：并发请求
来源：http://www.share.fanxiaobao.xyz/Article/details/gjjfetjff.sHtML

await Promise.all(urls.map(u => fetch(u)))
来源：http://wap.fanxiaobao.xyz/Article/details/gyyvqkfyr.sHtML

[U98] JS：fetch 带 JSON
来源：http://3g.fanxiaobao.xyz/Article/details/grnkxbymf.sHtML

await fetch(url, { method: "POST", headers: { "Content-Type": "application/json" }, body: JSON.stringify(d) })
来源：http://wap.fanxiaobao.xyz/Article/details/gpsdylqti.sHtML

[U99] JS：事件监听
来源：http://www.share.fanxiaobao.xyz/Article/details/gwzsngikl.sHtML

el.addEventListener("click", e => {})
来源：http://3g.fanxiaobao.xyz/Article/details/gtpcfdfmp.sHtML

[U100] JS：DOM 查询
来源：http://www.blog.fanxiaobao.xyz/Article/details/gvhexbalf.sHtML

document.querySelector(".item")
来源：http://baike.fanxiaobao.xyz/Article/details/gubamztlw.sHtML

[U101] JS：classList 操作
来源：http://mobile.fanxiaobao.xyz/Article/details/gbtuflzhj.sHtML

el.classList.toggle("active")
来源：http://read.share.fanxiaobao.xyz/Article/details/gphnorvhu.sHtML

[U102] JS：本地存储
来源：http://read.share.fanxiaobao.xyz/Article/details/gyjwidrih.sHtML

localStorage.setItem("k", JSON.stringify(v))
来源：http://wap.fanxiaobao.xyz/Article/details/gkikyluxu.sHtML

[U103] JS：定时器
来源：http://read.share.fanxiaobao.xyz/Article/details/ghnursigf.sHtML

setTimeout(fn, 1000);  setInterval(fn, 1000);
来源：http://www.share.fanxiaobao.xyz/Article/details/ggtqpllnn.sHtML

[U104] JS：防抖
来源：http://read.share.fanxiaobao.xyz/Article/details/ganyfpfoo.sHtML

const debounce = (fn, ms) => { let t; return (...a) => { clearTimeout(t); t = setTimeout(() => fn(...a), ms); }; };
来源：http://blog.fanxiaobao.xyz/Article/details/gtvphciup.sHtML

[U105] JS：节流
来源：http://www.share.fanxiaobao.xyz/Article/details/gynivqrxo.sHtML

const throttle = (fn, ms) => { let last = 0; return (...a) => { const n = Date.now(); if (n - last >= ms) { last = n; fn(...a); } }; };
来源：http://www.share.fanxiaobao.xyz/Article/details/gwstkmdbl.sHtML

[U106] JS：日期格式化
来源：http://blog.fanxiaobao.xyz/Article/details/gyoizboiz.sHtML

new Intl.DateTimeFormat("zh-CN", { dateStyle: "medium" }).format(new Date())
来源：http://read.share.fanxiaobao.xyz/Article/details/gpywksyye.sHtML

[U107] JS：数字千分位
来源：http://wap.fanxiaobao.xyz/Article/details/gxlsyckkp.sHtML

new Intl.NumberFormat("en-US").format(1234567)
来源：http://m.share.fanxiaobao.xyz/Article/details/gxvitxwfa.sHtML

[U108] JS：随机整数
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gnerhyxgm.sHtML

Math.floor(Math.random() * (max - min + 1)) + min
来源：http://www.share.fanxiaobao.xyz/Article/details/gpbsuugdq.sHtML

[U109] JS：数组分组
来源：http://www.share.fanxiaobao.xyz/Article/details/glkpxzejl.sHtML

Object.groupBy(arr, x => x.type)
来源：http://blog.fanxiaobao.xyz/Article/details/gtzgkpayc.sHtML

[U110] JS：数组分块
来源：http://www.share.fanxiaobao.xyz/Article/details/ghqzusyzz.sHtML

arr.reduce((acc, x, i) => (i % size ? acc : [...acc, arr.slice(i, i + size)]), [])
来源：http://3g.fanxiaobao.xyz/Article/details/gxhwodhur.sHtML

[U111] JS：对象转 Map
来源：http://read.share.fanxiaobao.xyz/Article/details/gnmvseghk.sHtML

new Map(Object.entries(obj))
来源：http://read.share.fanxiaobao.xyz/Article/details/gppctiakq.sHtML

[U112] JS：字符串补位
来源：http://m.share.fanxiaobao.xyz/Article/details/gqyegnxjp.sHtML

"7".padStart(3, "0")
来源：http://www.blog.fanxiaobao.xyz/Article/details/gqbraajde.sHtML

[U113] JS：正则替换全部
来源：http://www.blog.fanxiaobao.xyz/Article/details/gqbrynqeg.sHtML

s.replaceAll("a", "b")
来源：http://blog.fanxiaobao.xyz/Article/details/gvlnpgxkq.sHtML

[U114] JS：JSON 深比较
来源：http://www.blog.fanxiaobao.xyz/Article/details/ghikiztzc.sHtML

JSON.stringify(a) === JSON.stringify(b)
来源：http://m.share.fanxiaobao.xyz/Article/details/gvmasggdd.sHtML

[U115] JS：生成 UUID
来源：http://read.share.fanxiaobao.xyz/Article/details/gziscmaqv.sHtML

crypto.randomUUID()
来源：http://read.share.fanxiaobao.xyz/Article/details/gtlhqcnzg.sHtML

[U116] JS：类型检查（JSDoc）
来源：http://baike.fanxiaobao.xyz/Article/details/gdnbkyvwh.sHtML

/** @param {string} name */ function f(name) {}
来源：http://www.share.fanxiaobao.xyz/Article/details/goepischo.sHtML

[U117] JS：单元测试
来源：http://3g.fanxiaobao.xyz/Article/details/godpqulyz.sHtML

npm i -D vitest;  npx vitest
来源：http://blog.fanxiaobao.xyz/Article/details/goqskczvt.sHtML

[U118] JS：开发服务器
来源：http://baike.fanxiaobao.xyz/Article/details/gitarpptt.sHtML

npm i -D vite;  npx vite
来源：http://www.blog.fanxiaobao.xyz/Article/details/gzqsoixta.sHtML

[U119] JS：生产构建
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gtggyvfoo.sHtML

npx vite build
来源：http://www.share.fanxiaobao.xyz/Article/details/gpzhpyfud.sHtML

[U120] JS：读取环境变量（Vite）
来源：http://www.share.fanxiaobao.xyz/Article/details/gxjssxyxk.sHtML

import.meta.env.VITE_API_URL
来源：http://wap.fanxiaobao.xyz/Article/details/gyqdijjmn.sHtML

================================================================================
来源：http://wap.fanxiaobao.xyz/Article/details/gteaoybrv.sHtML

统计汇总
来源：http://blog.fanxiaobao.xyz/Article/details/gkkkxgumr.sHtML

================================================================================
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gyxpivapt.sHtML

按语言统计（条）：
来源：http://3g.fanxiaobao.xyz/Article/details/gjolgtkyu.sHtML

Python ......... 252
来源：http://www.share.fanxiaobao.xyz/Article/details/gwzzkbcyx.sHtML

PHP ............ 252
来源：http://mobile.fanxiaobao.xyz/Article/details/gxewozvok.sHtML

JavaScript ..... 252
来源：http://www.blog.fanxiaobao.xyz/Article/details/ghzcjowep.sHtML

TypeScript ..... 212
来源：http://mobile.fanxiaobao.xyz/Article/details/gsexbavkf.sHtML

Java ........... 212
来源：http://blog.fanxiaobao.xyz/Article/details/gbhgiotdm.sHtML

Go ............. 212
来源：http://3g.fanxiaobao.xyz/Article/details/gcomutqpz.sHtML

Ruby ........... 212
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gidinfxof.sHtML

C# ............. 212
来源：http://wap.fanxiaobao.xyz/Article/details/gnokxypvl.sHtML

C .............. 30
来源：http://www.blog.fanxiaobao.xyz/Article/details/godscbdcv.sHtML

C++ ............ 30
来源：http://read.share.fanxiaobao.xyz/Article/details/gwhhnzarz.sHtML

SQL ............ 90
来源：http://www.share.fanxiaobao.xyz/Article/details/goehimdkb.sHtML

Bash ........... 80
来源：http://baike.fanxiaobao.xyz/Article/details/gdduqarzw.sHtML

Kotlin ......... 15
来源：http://baike.fanxiaobao.xyz/Article/details/ggjtbhflg.sHtML

Swift .......... 15
来源：http://baike.fanxiaobao.xyz/Article/details/gsulmcwgr.sHtML

Lua ............ 10
来源：http://www.share.fanxiaobao.xyz/Article/details/gpdobreos.sHtML

Perl ........... 10
来源：http://mobile.fanxiaobao.xyz/Article/details/gnnitjhbd.sHtML

Scala .......... 10
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gwdxjbpin.sHtML

------------------------------------
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gmvpxlpuv.sHtML

合计 ........... 2106 条
来源：http://wap.fanxiaobao.xyz/Article/details/ggwfjaxsb.sHtML

按章节统计：
来源：http://baike.fanxiaobao.xyz/Article/details/gorohbidq.sHtML

A 基础语法与类型       26 个任务 × 8 语言 =  208
来源：http://baike.fanxiaobao.xyz/Article/details/gtrwgaelv.sHtML

B 流程控制             16 个任务 × 8 语言 =  128
来源：http://mobile.fanxiaobao.xyz/Article/details/gwttqzebf.sHtML

C 函数与作用域         16 个任务 × 8 语言 =  128
来源：http://m.share.fanxiaobao.xyz/Article/details/gzdmmkzof.sHtML

D 数组 / 列表 / 集合   26 个任务 × 8 语言 =  208
来源：http://blog.fanxiaobao.xyz/Article/details/guifitbdd.sHtML

E 字符串处理           22 个任务 × 8 语言 =  176
来源：http://mobile.fanxiaobao.xyz/Article/details/gzrecdzbw.sHtML

F 文件与目录           12 个任务 × 8 语言 =   96
来源：http://3g.fanxiaobao.xyz/Article/details/gjsafoiir.sHtML

G 面向对象             16 个任务 × 8 语言 =  128
来源：http://baike.fanxiaobao.xyz/Article/details/gafeubcci.sHtML

H 异常与错误处理       10 个任务 × 8 语言 =   80
来源：http://read.share.fanxiaobao.xyz/Article/details/gtchsvvxh.sHtML

I 正则表达式            8 个任务 × 8 语言 =   64
来源：http://www.blog.fanxiaobao.xyz/Article/details/gomiyadon.sHtML

J 日期与时间           10 个任务 × 8 语言 =   80
来源：http://baike.fanxiaobao.xyz/Article/details/gixvmbehm.sHtML

K JSON 与序列化         8 个任务 × 8 语言 =   64
来源：http://wap.fanxiaobao.xyz/Article/details/gukdkxypt.sHtML

L 网络请求              8 个任务 × 8 语言 =   64
来源：http://read.share.fanxiaobao.xyz/Article/details/gfhqghnko.sHtML

M 命令行 / 进程         8 个任务 × 8 语言 =   64
来源：http://m.share.fanxiaobao.xyz/Article/details/gjyxyhclc.sHtML

N 数据结构与算法       12 个任务 × 8 语言 =   96
来源：http://mobile.fanxiaobao.xyz/Article/details/gerafzikr.sHtML

O 并发与异步            6 个任务 × 8 语言 =   48
来源：http://www.share.fanxiaobao.xyz/Article/details/gjwawwaro.sHtML

P 常用工具函数          8 个任务 × 8 语言 =   64
来源：http://3g.fanxiaobao.xyz/Article/details/gikmainma.sHtML

Q SQL 专题                              90
来源：http://baike.fanxiaobao.xyz/Article/details/gzjmexvid.sHtML

R Bash 专题                             80
来源：http://3g.fanxiaobao.xyz/Article/details/gsjepzylc.sHtML

S C / C++ 专题                          60
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gnfczzejn.sHtML

T 其他语言补充                          60
来源：http://blog.fanxiaobao.xyz/Article/details/glgzpleoe.sHtML

U 高频实用片段                         120
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gxecklptc.sHtML

------------------------------------
来源：http://read.share.fanxiaobao.xyz/Article/details/gqvygnbbr.sHtML

合计                                  2106 条
来源：http://www.blog.fanxiaobao.xyz/Article/details/gayiqplsh.sHtML

--------------------------------------------------------------------------------
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gbcizscss.sHtML

使用提醒
来源：http://read.share.fanxiaobao.xyz/Article/details/glhqwnjct.sHtML

--------------------------------------------------------------------------------
来源：http://www.blog.fanxiaobao.xyz/Article/details/ggxakuffa.sHtML

1. 示例追求"最小可用"，正式项目中请补齐导入、错误处理与边界判断。
来源：http://wap.fanxiaobao.xyz/Article/details/gfxfkxhhg.sHtML

2. 涉及文件、网络、数据库的示例，注意资源释放与异常捕获。
来源：http://www.blog.fanxiaobao.xyz/Article/details/gvyhqyhcc.sHtML

3. 语言版本差异较大（如 Python 3.10 的 match、Java 17 的 record/switch 箭头），
来源：http://blog.fanxiaobao.xyz/Article/details/gxzojkrfm.sHtML

在旧版本上使用前请先确认语法支持情况。
来源：http://www.share.fanxiaobao.xyz/Article/details/gwqqzblgd.sHtML

4. 标注"手写"的条目是因为该语言缺少对应内置能力，实际项目中可引入成熟库。
来源：http://www.share.fanxiaobao.xyz/Article/details/gdvnbcyic.sHtML

—— 文件结束 ——
来源：http://www.blog.fanxiaobao.xyz/Article/details/gluwbvnia.sHtML

================================================================================
来源：http://3g.fanxiaobao.xyz/Article/details/gnoumtlgh.sHtML

程序语言常见例子速查手册（2024 版）
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gaoxnpfnx.sHtML

Common Programming Examples Cheat Book
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gpswnfxcz.sHtML

================================================================================
来源：http://m.share.fanxiaobao.xyz/Article/details/gjfezzlrr.sHtML

【收录内容】
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gmycdkyst.sHtML

覆盖 12 种语言 / 语法与常见 API：
来源：http://www.share.fanxiaobao.xyz/Article/details/gdmtbazky.sHtML

Python · PHP · JavaScript · TypeScript · Java · Go · Ruby · C#
来源：http://mobile.fanxiaobao.xyz/Article/details/gojsdliiu.sHtML

SQL · Bash · C · C++
来源：http://www.blog.fanxiaobao.xyz/Article/details/gndlhazni.sHtML

按「任务」分组：每个任务下按语言各给出一条最小可用示例。
来源：http://www.share.fanxiaobao.xyz/Article/details/gurbzmxvo.sHtML

【使用说明】
来源：http://www.share.fanxiaobao.xyz/Article/details/gycvoycgx.sHtML

1. 每个任务形如 "[编号] 任务名"，下面每行以语言标记开头：
来源：http://m.share.fanxiaobao.xyz/Article/details/gphejaddm.sHtML

Py:    Python        PHP:   PHP           JS:    JavaScript
来源：http://www.blog.fanxiaobao.xyz/Article/details/gtwldbmnf.sHtML

TS:    TypeScript    Java:  Java          Go:    Go
来源：http://mobile.fanxiaobao.xyz/Article/details/gvstxohrq.sHtML

Ruby:  Ruby          C#:    C#            SQL:   SQL
来源：http://baike.fanxiaobao.xyz/Article/details/gouspjxkq.sHtML

Bash:  Shell         C:     C             C++:   C++
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gamikcayz.sHtML

2. 示例只展示核心写法，刻意省略 import / require / include / using 等样板代码。
来源：http://m.share.fanxiaobao.xyz/Article/details/gmvllgcvs.sHtML

需要完整可运行文件时，请自行补齐当前语言的导入语句。
来源：http://www.blog.fanxiaobao.xyz/Article/details/gfaforojs.sHtML

3. 语法基准：Python 3.10+ / PHP 8.1+ / ES2020+ / TypeScript 5 / Java 17 /
来源：http://read.share.fanxiaobao.xyz/Article/details/gwpwkzdgp.sHtML

Go 1.21+ / Ruby 3.x / C# 10+ / C17 / C++17。
来源：http://3g.fanxiaobao.xyz/Article/details/giljrfikm.sHtML

4. 检索建议：用编辑器或浏览器 Ctrl+F 搜关键词，如 "排序" "读取文件" "正则"。
来源：http://mobile.fanxiaobao.xyz/Article/details/gzntfmgek.sHtML

5. 标记为 "// 无" 表示该语言没有对应的一等语法，需用替代写法（示例给出替代方案）。
来源：http://mobile.fanxiaobao.xyz/Article/details/ggfaqcltj.sHtML

6. 符号 "⏎" 表示代码在此处换行（主要用于 Python 等强制缩进、无法压成一行的结构）。
来源：http://wap.fanxiaobao.xyz/Article/details/gxventzak.sHtML

【文件统计】
来源：http://3g.fanxiaobao.xyz/Article/details/gwkjjxqdh.sHtML

语言示例共 2106 条，分布见本文末尾的「统计汇总」。
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gpiqcrpgj.sHtML

--------------------------------------------------------------------------------
来源：http://www.blog.fanxiaobao.xyz/Article/details/gvccpfwny.sHtML

目  录
来源：http://www.blog.fanxiaobao.xyz/Article/details/gejrisoxv.sHtML

--------------------------------------------------------------------------------
来源：http://m.share.fanxiaobao.xyz/Article/details/geffvpuqu.sHtML

A. 基础语法与类型              （第 1 节，26 个任务，208 条）
来源：http://wap.fanxiaobao.xyz/Article/details/grnykifeg.sHtML

B. 流程控制                    （第 2 节，16 个任务，128 条）
来源：http://mobile.fanxiaobao.xyz/Article/details/gnyiodfll.sHtML

C. 函数与作用域                （第 3 节，16 个任务，128 条）
来源：http://wap.fanxiaobao.xyz/Article/details/gsqpiwouc.sHtML

D. 数组 / 列表 / 集合          （第 4 节，26 个任务，208 条）
来源：http://read.share.fanxiaobao.xyz/Article/details/gyosismnq.sHtML

E. 字符串处理                  （第 5 节，22 个任务，176 条）
来源：http://www.blog.fanxiaobao.xyz/Article/details/gcvyiphcm.sHtML


<!-- 参考信息 -->