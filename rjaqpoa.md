代发 wailian999

[U15] Py：高精度计时
来源：http://baike.fehbvm.com/Article/details/gihtycmgh.sHtML

t = time.perf_counter()
来源：http://www.blog.hesvh.cn/Article/details/guztcxhtk.sHtML

[U16] Py：命令行参数解析
来源：http://baike.fehbvm.com/Article/details/govnoqqsu.sHtML

ap = argparse.ArgumentParser();  ap.add_argument("--name");  args = ap.parse_args()
来源：http://3g.hesvh.cn/Article/details/grhjrfajd.sHtML

[U17] Py：初始化日志
来源：http://blog.fehbvm.com/Article/details/gcbeldjrz.sHtML

logging.basicConfig(level=logging.INFO)
来源：http://baike.hesvh.cn/Article/details/gvtksomzt.sHtML

[U18] Py：预编译正则
来源：http://wap.zdbjq.cn/Article/details/gkdyhlvoh.sHtML

pat = re.compile(r"\d+")
来源：http://blog.zdbjq.cn/Article/details/godkftzsw.sHtML

[U19] Py：正则替换带回调
来源：http://3g.zdbjq.cn/Article/details/glarjmlni.sHtML

re.sub(r"\d+", lambda m: str(int(m.group()) * 2), s)
来源：http://read.share.zdbjq.cn/Article/details/glijlrqan.sHtML

[U20] Py：缓存函数结果
来源：http://wap.fehbvm.com/Article/details/gvidlwqpm.sHtML

@functools.lru_cache(maxsize=None)
来源：http://www.share.fehbvm.com/Article/details/gxdzznmay.sHtML

[U21] Py：自定义上下文管理器
来源：http://3g.fehbvm.com/Article/details/gpakwadrr.sHtML

@contextlib.contextmanager
来源：http://wap.hesvh.cn/Article/details/gobhkfhqj.sHtML

[U22] Py：矩阵转置
来源：http://mobile.fehbvm.com/Article/details/gaxwxrnag.sHtML

list(zip(*m))
来源：http://blog.fehbvm.com/Article/details/gxigynxmx.sHtML

[U23] Py：分块读取大文件
来源：http://www.m.share.fehbvm.com/Article/details/gbbgkbgpg.sHtML

for chunk in iter(lambda: f.read(8192), b""):
来源：http://mobile.fehbvm.com/Article/details/gufdzdfwn.sHtML

[U24] Py：路径操作
来源：http://www.blog.hesvh.cn/Article/details/gbqzxcxkq.sHtML

Path("a/b.txt").parent.mkdir(parents=True, exist_ok=True)
来源：http://read.share.fehbvm.com/Article/details/ghfqvvqmi.sHtML

[U25] Py：CSV 按字典读
来源：http://www.m.share.zdbjq.cn/Article/details/ghwhllvzy.sHtML

csv.DictReader(f)
来源：http://mobile.fehbvm.com/Article/details/gegmatnnp.sHtML

[U26] Py：并发下载
来源：http://read.share.hesvh.cn/Article/details/gyesxexqz.sHtML

ThreadPoolExecutor(max_workers=8).map(fetch, urls)
来源：http://www.blog.fehbvm.com/Article/details/gwbamkwvf.sHtML

[U27] Py：异步 HTTP
来源：http://m.share.hesvh.cn/Article/details/gnsrruhyv.sHtML

aiohttp.ClientSession() 配合 async with
来源：http://blog.hesvh.cn/Article/details/gvqbeuynv.sHtML

[U28] Py：类型别名
来源：http://read.share.zdbjq.cn/Article/details/gnngszbpw.sHtML

UserId = int
来源：http://www.blog.fehbvm.com/Article/details/gdmnfbpck.sHtML

[U29] Py：属性校验
来源：http://read.share.hesvh.cn/Article/details/gbydtyarl.sHtML

@property 与 @x.setter 配合
来源：http://baike.hesvh.cn/Article/details/gtqcblggv.sHtML

[U30] Py：数据类
来源：http://www.share.hesvh.cn/Article/details/gxsfqhlay.sHtML

@dataclass(slots=True)
来源：http://mobile.zdbjq.cn/Article/details/gwscfklpl.sHtML

[U31] Py：单测
来源：http://www.share.fehbvm.com/Article/details/gkxdcmbpb.sHtML

python -m pytest -q
来源：http://www.share.hesvh.cn/Article/details/gvwxsqvzm.sHtML

[U32] Py：代码格式化
来源：http://read.share.zdbjq.cn/Article/details/geayxroqr.sHtML

ruff format . && ruff check --fix .
来源：http://m.share.hesvh.cn/Article/details/gzzscfjtv.sHtML

[U33] Py：打包发布
来源：http://read.share.fehbvm.com/Article/details/glbqozxbw.sHtML

python -m build  （依赖 pyproject.toml）
来源：http://www.blog.hesvh.cn/Article/details/gpuxwhokz.sHtML

[U34] Py：判断编码
来源：http://baike.hesvh.cn/Article/details/grmkqxiaa.sHtML

chardet.detect(raw)
来源：http://wap.fehbvm.com/Article/details/gbrpcizwl.sHtML

[U35] Py：发送邮件
来源：http://3g.hesvh.cn/Article/details/ghabytafv.sHtML

smtplib.SMTP_SSL(...).send_message(msg)
来源：http://wap.hesvh.cn/Article/details/ghtanfhwv.sHtML

[U36] Py：定时任务
来源：http://www.m.share.hesvh.cn/Article/details/gdpkpifcf.sHtML

schedule.every(10).minutes.do(job)
来源：http://blog.fehbvm.com/Article/details/ggyhosunt.sHtML

[U37] Py：读写 Excel
来源：http://baike.zdbjq.cn/Article/details/gsvmbrysn.sHtML

pandas.read_excel / DataFrame.to_excel
来源：http://3g.hesvh.cn/Article/details/gkbheztvr.sHtML

[U38] Py：获取脚本所在目录
来源：http://3g.zdbjq.cn/Article/details/gszsxluzo.sHtML

Path(__file__).resolve().parent
来源：http://3g.hesvh.cn/Article/details/gvoxduinx.sHtML

[U39] Py：判断是否在交互环境
来源：http://www.share.hesvh.cn/Article/details/gyakbhdlc.sHtML

sys.stdout.isatty()
来源：http://www.share.zdbjq.cn/Article/details/gqplldvup.sHtML

[U40] Py：打印到标准错误
来源：http://read.share.zdbjq.cn/Article/details/gqntoqobz.sHtML

print("err", file=sys.stderr)
来源：http://www.m.share.fehbvm.com/Article/details/gupifjdrq.sHtML

[U41] PHP：初始化 Composer 项目
来源：http://blog.zdbjq.cn/Article/details/gefuwuxha.sHtML

composer init;  composer require guzzlehttp/guzzle
来源：http://3g.fehbvm.com/Article/details/gvnfczzpa.sHtML

[U42] PHP：PSR-4 自动加载
来源：http://3g.hesvh.cn/Article/details/grthidnfy.sHtML

"autoload": { "psr-4": { "App\\": "src/" } }
来源：http://m.share.hesvh.cn/Article/details/gikqegwai.sHtML

[U43] PHP：声明命名空间
来源：http://www.share.zdbjq.cn/Article/details/gdujppzjk.sHtML

namespace App\Http;
来源：http://wap.fehbvm.com/Article/details/gzozuytsu.sHtML

[U44] PHP：开启严格类型
来源：http://read.share.fehbvm.com/Article/details/gvnmwjzrt.sHtML

declare(strict_types=1);
来源：http://baike.fehbvm.com/Article/details/ghxzueoit.sHtML

[U45] PHP：类型声明与返回类型
来源：http://3g.zdbjq.cn/Article/details/ggykuwsir.sHtML

function add(int $a, int $b): int { return $a + $b; }
来源：http://www.m.share.hesvh.cn/Article/details/goqaqtgfi.sHtML

[U46] PHP：可空类型
来源：http://wap.hesvh.cn/Article/details/gimggonhk.sHtML

?string $name = null
来源：http://www.m.share.fehbvm.com/Article/details/glyneagug.sHtML

[U47] PHP：联合类型
来源：http://read.share.fehbvm.com/Article/details/gxkylukwa.sHtML

int|string $id
来源：http://read.share.fehbvm.com/Article/details/gjjsecwdf.sHtML

[U48] PHP：纯枚举
来源：http://baike.zdbjq.cn/Article/details/gluivgkal.sHtML

enum Status: string { case Active = "active"; case Off = "off"; }
来源：http://www.share.zdbjq.cn/Article/details/gwrpmqeuf.sHtML

[U49] PHP：只读属性
来源：http://wap.zdbjq.cn/Article/details/gcpuuhamd.sHtML

public readonly string $name
来源：http://read.share.hesvh.cn/Article/details/ggzlgozqo.sHtML

[U50] PHP：构造器属性提升
来源：http://3g.zdbjq.cn/Article/details/ghsyjosnz.sHtML

public function __construct(private int $id) {}
来源：http://baike.hesvh.cn/Article/details/gxeazgtph.sHtML

[U51] PHP：数组解构
来源：http://www.m.share.fehbvm.com/Article/details/gyaucfewm.sHtML

[$a, $b] = $arr;
来源：http://mobile.hesvh.cn/Article/details/gmruirxkk.sHtML

[U52] PHP：箭头函数
来源：http://mobile.fehbvm.com/Article/details/glhuhgjax.sHtML

$double = fn($x) => $x * 2;
来源：http://3g.hesvh.cn/Article/details/gouwgsgbe.sHtML

[U53] PHP：空合并运算符
来源：http://m.share.fehbvm.com/Article/details/gihegrbhp.sHtML

$v = $a ?? $b ?? "default";
来源：http://3g.zdbjq.cn/Article/details/gtecpqxvm.sHtML

[U54] PHP：空安全调用
来源：http://www.share.fehbvm.com/Article/details/gpsgoffsp.sHtML

$obj?->method()
来源：http://www.share.hesvh.cn/Article/details/gtokwkhch.sHtML

[U55] PHP：match 表达式
来源：http://www.share.zdbjq.cn/Article/details/getxuhugu.sHtML

$s = match($x) { 1 => "一", default => "其他" };
来源：http://read.share.fehbvm.com/Article/details/gptcfewcc.sHtML

[U56] PHP：命名参数
来源：http://read.share.fehbvm.com/Article/details/gasibtkbb.sHtML

f(a: 1, b: 2)
来源：http://m.share.hesvh.cn/Article/details/gaaexdpar.sHtML

[U57] PHP：字符串插值
来源：http://www.share.fehbvm.com/Article/details/gbapyjewi.sHtML

"值: {$a}"
来源：http://www.m.share.zdbjq.cn/Article/details/gbbprzqwz.sHtML

[U58] PHP：数组三件套
来源：http://www.m.share.zdbjq.cn/Article/details/gndtiydwj.sHtML

array_map($f, $a);  array_filter($a, $f);  array_reduce($a, $f, 0);
来源：http://blog.fehbvm.com/Article/details/gneeggfdt.sHtML

[U59] PHP：自定义排序
来源：http://blog.zdbjq.cn/Article/details/gwfsjzpgv.sHtML

usort($arr, fn($a, $b) => $a["age"] <=> $b["age"]);
来源：http://www.share.hesvh.cn/Article/details/gqxaynhua.sHtML

[U60] PHP：JSON 编解码
来源：http://wap.hesvh.cn/Article/details/gazfhavib.sHtML

json_encode($d, JSON_UNESCAPED_UNICODE);  json_decode($s, true);
来源：http://www.blog.hesvh.cn/Article/details/gkgrbcvon.sHtML

[U61] PHP：正则
来源：http://www.m.share.hesvh.cn/Article/details/gegwcwxng.sHtML

preg_match('/(\d+)/', $s, $m);  preg_replace('/\d+/', '#', $s);
来源：http://blog.hesvh.cn/Article/details/gilphihhd.sHtML

[U62] PHP：日期对象
来源：http://mobile.zdbjq.cn/Article/details/gsozdnrjp.sHtML

(new DateTimeImmutable())->format("Y-m-d");
来源：http://3g.zdbjq.cn/Article/details/gmahxtuhg.sHtML

[U63] PHP：文件读写
来源：http://mobile.fehbvm.com/Article/details/gwsatblbi.sHtML

file_get_contents($f);  file_put_contents($f, $data);
来源：http://m.share.zdbjq.cn/Article/details/gejddtexo.sHtML

[U64] PHP：目录遍历
来源：http://www.m.share.hesvh.cn/Article/details/glonypagt.sHtML

glob("dir/*.php");  scandir("dir");
来源：http://m.share.hesvh.cn/Article/details/gqriroxit.sHtML

[U65] PHP：会话
来源：http://www.m.share.zdbjq.cn/Article/details/gwbpjemmr.sHtML

session_start();  $_SESSION["uid"] = 1;
来源：http://read.share.hesvh.cn/Article/details/galbswgob.sHtML

[U66] PHP：设置 Cookie
来源：http://mobile.hesvh.cn/Article/details/gbrsiyxmc.sHtML

setcookie("token", $v, ["httponly" => true, "samesite" => "Lax"]);
来源：http://3g.hesvh.cn/Article/details/gipvoevwo.sHtML

[U67] PHP：处理文件上传
来源：http://baike.hesvh.cn/Article/details/govzqhiwu.sHtML

$_FILES["file"]["tmp_name"] 与 move_uploaded_file()
来源：http://read.share.fehbvm.com/Article/details/ggryhgcaf.sHtML

[U68] PHP：PDO 连接
来源：http://3g.fehbvm.com/Article/details/glqpvszjz.sHtML

$pdo = new PDO("mysql:host=localhost;dbname=app", "root", "");
来源：http://www.blog.zdbjq.cn/Article/details/grxsmetgv.sHtML

[U69] PHP：PDO 预处理
来源：http://3g.zdbjq.cn/Article/details/gsazryxpe.sHtML

$stmt = $pdo->prepare("SELECT * FROM users WHERE id = ?");  $stmt->execute([$id]);
来源：http://read.share.fehbvm.com/Article/details/gsylanlep.sHtML

[U70] PHP：PDO 事务
来源：http://3g.fehbvm.com/Article/details/gmpyrwtok.sHtML

$pdo->beginTransaction();  $pdo->commit();  $pdo->rollBack();
来源：http://mobile.fehbvm.com/Article/details/gkinlbakp.sHtML

[U71] PHP：抛出异常
来源：http://wap.hesvh.cn/Article/details/gxfcskiep.sHtML

throw new RuntimeException("失败", 500);
来源：http://3g.fehbvm.com/Article/details/gpaurvmnd.sHtML

[U72] PHP：写错误日志
来源：http://read.share.fehbvm.com/Article/details/ghdaiagwx.sHtML

error_log("失败: " . $e->getMessage());
来源：http://wap.zdbjq.cn/Article/details/gpuqovsun.sHtML

[U73] PHP：读取 ini 配置
来源：http://www.blog.fehbvm.com/Article/details/gxasjnwah.sHtML

parse_ini_file("config.ini", true)
来源：http://www.blog.hesvh.cn/Article/details/goyjwiqva.sHtML

[U74] PHP：读取环境变量
来源：http://3g.hesvh.cn/Article/details/gxoxdijxa.sHtML

getenv("APP_ENV") ?: "production"
来源：http://m.share.zdbjq.cn/Article/details/gzkumzgar.sHtML

[U75] PHP：依赖注入
来源：http://mobile.fehbvm.com/Article/details/gygoopkuh.sHtML

composer require psr/container
来源：http://3g.zdbjq.cn/Article/details/gqfietvow.sHtML

[U76] PHP：简单路由
来源：http://www.share.zdbjq.cn/Article/details/gberncvmd.sHtML

$path = parse_url($_SERVER["REQUEST_URI"], PHP_URL_PATH);
来源：http://read.share.fehbvm.com/Article/details/gverhazlt.sHtML

[U77] PHP：模板渲染
来源：http://mobile.fehbvm.com/Article/details/gwbnquapb.sHtML

composer require twig/twig
来源：http://mobile.hesvh.cn/Article/details/gvocnsmdn.sHtML

[U78] PHP：单元测试
来源：http://www.blog.zdbjq.cn/Article/details/gfbhsdyxw.sHtML

composer require --dev phpunit/phpunit
来源：http://www.blog.zdbjq.cn/Article/details/grcvcqpxs.sHtML

[U79] PHP：静态分析
来源：http://www.blog.zdbjq.cn/Article/details/gupblycvu.sHtML

composer require --dev phpstan/phpstan
来源：http://www.blog.hesvh.cn/Article/details/gnjxnorvf.sHtML

[U80] PHP：代码规范修复
来源：http://baike.zdbjq.cn/Article/details/gquqqncjb.sHtML

composer require --dev friendsofphp/php-cs-fixer
来源：http://3g.hesvh.cn/Article/details/gaskfuyju.sHtML

[U81] JS：初始化项目
来源：http://baike.fehbvm.com/Article/details/gidqqnghu.sHtML

npm init -y;  npm i express
来源：http://wap.fehbvm.com/Article/details/gadbzwsfh.sHtML

[U82] JS：package.json 脚本
来源：http://read.share.zdbjq.cn/Article/details/gsqmdsqhn.sHtML

"scripts": { "dev": "vite", "build": "vite build" }
来源：http://read.share.fehbvm.com/Article/details/gwkgztfhs.sHtML

[U83] JS：ES Module 导入导出
来源：http://mobile.zdbjq.cn/Article/details/gtoszkbnp.sHtML

export const a = 1;  import { a } from "./m.js";
来源：http://www.m.share.zdbjq.cn/Article/details/ggbzdledf.sHtML

[U84] JS：CommonJS 写法
来源：http://wap.hesvh.cn/Article/details/gzimqopjd.sHtML

module.exports = { a };  const { a } = require("./m");
来源：http://blog.fehbvm.com/Article/details/ggusbakas.sHtML

[U85] JS：可选链
来源：http://www.blog.zdbjq.cn/Article/details/gdxrgunqd.sHtML

a?.b?.c
来源：http://www.blog.fehbvm.com/Article/details/gequotpdc.sHtML

[U86] JS：空值合并
来源：http://read.share.fehbvm.com/Article/details/grmpmwtca.sHtML

a ?? b
来源：http://www.share.fehbvm.com/Article/details/gtbuqpodc.sHtML

[U87] JS：解构默认值
来源：http://m.share.zdbjq.cn/Article/details/grvfzzvhg.sHtML

const { a = 1, b = 2 } = obj;
来源：http://3g.zdbjq.cn/Article/details/gytizvwyq.sHtML

[U88] JS：对象展开合并
来源：http://baike.fehbvm.com/Article/details/gduvhdteu.sHtML

{ ...a, ...b }
来源：http://www.m.share.hesvh.cn/Article/details/gwnukhjrm.sHtML

[U89] JS：数组去重
来源：http://mobile.zdbjq.cn/Article/details/gdtceuwff.sHtML

[...new Set(arr)]
来源：http://www.blog.fehbvm.com/Article/details/gzfurqajm.sHtML

[U90] JS：数字数组排序
来源：http://wap.zdbjq.cn/Article/details/gdebwfwmk.sHtML

[...arr].sort((a, b) => a - b)
来源：http://wap.fehbvm.com/Article/details/gugyodioe.sHtML

[U91] JS：对象键值遍历
来源：http://www.share.hesvh.cn/Article/details/geplpwkun.sHtML

Object.entries(obj).forEach(([k, v]) => {});
来源：http://blog.hesvh.cn/Article/details/gotoujdzn.sHtML

[U92] JS：深拷贝
来源：http://blog.fehbvm.com/Article/details/gpjoovhfi.sHtML

structuredClone(obj)
来源：http://3g.fehbvm.com/Article/details/gggwjojza.sHtML

[U93] JS：模板字符串
来源：http://read.share.zdbjq.cn/Article/details/gspjbzdhn.sHtML

`共 ${n} 条`
来源：http://m.share.fehbvm.com/Article/details/gzpadkgkz.sHtML

[U94] JS：箭头函数
来源：http://blog.hesvh.cn/Article/details/gsuydhbwd.sHtML

const double = x => x * 2;
来源：http://wap.zdbjq.cn/Article/details/gmtinoioy.sHtML

[U95] JS：Promise 包装
来源：http://mobile.fehbvm.com/Article/details/ggfojcfwb.sHtML

new Promise((resolve, reject) => {})
来源：http://www.share.hesvh.cn/Article/details/gcweaiigx.sHtML

[U96] JS：async/await 与异常
来源：http://3g.hesvh.cn/Article/details/gvjzkonla.sHtML

try { const d = await f(); } catch (e) { console.error(e); }
来源：http://read.share.zdbjq.cn/Article/details/gfjlwmulw.sHtML

[U97] JS：并发请求
来源：http://mobile.fehbvm.com/Article/details/goifwsrtt.sHtML

await Promise.all(urls.map(u => fetch(u)))
来源：http://wap.hesvh.cn/Article/details/gqcbaeiqr.sHtML

[U98] JS：fetch 带 JSON
来源：http://read.share.zdbjq.cn/Article/details/gtlvzbawy.sHtML

await fetch(url, { method: "POST", headers: { "Content-Type": "application/json" }, body: JSON.stringify(d) })
来源：http://3g.fehbvm.com/Article/details/gjfdvshlh.sHtML

[U99] JS：事件监听
来源：http://baike.hesvh.cn/Article/details/gzoimhefa.sHtML

el.addEventListener("click", e => {})
来源：http://blog.fehbvm.com/Article/details/gxgkpjgyb.sHtML

[U100] JS：DOM 查询
来源：http://read.share.hesvh.cn/Article/details/gvfxcdmlk.sHtML

document.querySelector(".item")
来源：http://www.share.hesvh.cn/Article/details/gyukjiujg.sHtML

[U101] JS：classList 操作
来源：http://www.blog.zdbjq.cn/Article/details/gzoucuswa.sHtML

el.classList.toggle("active")
来源：http://3g.zdbjq.cn/Article/details/goynrwgny.sHtML

[U102] JS：本地存储
来源：http://mobile.zdbjq.cn/Article/details/gcnudoxym.sHtML

localStorage.setItem("k", JSON.stringify(v))
来源：http://www.share.hesvh.cn/Article/details/gehbqvcrb.sHtML

[U103] JS：定时器
来源：http://baike.fehbvm.com/Article/details/gdxuisrrd.sHtML

setTimeout(fn, 1000);  setInterval(fn, 1000);
来源：http://m.share.hesvh.cn/Article/details/ghjyncqau.sHtML

[U104] JS：防抖
来源：http://read.share.fehbvm.com/Article/details/ghdebrpsp.sHtML

const debounce = (fn, ms) => { let t; return (...a) => { clearTimeout(t); t = setTimeout(() => fn(...a), ms); }; };
来源：http://m.share.zdbjq.cn/Article/details/gmimxbgrk.sHtML

[U105] JS：节流
来源：http://m.share.zdbjq.cn/Article/details/glbnfinmw.sHtML

const throttle = (fn, ms) => { let last = 0; return (...a) => { const n = Date.now(); if (n - last >= ms) { last = n; fn(...a); } }; };
来源：http://baike.fehbvm.com/Article/details/goeflfqul.sHtML

[U106] JS：日期格式化
来源：http://www.share.zdbjq.cn/Article/details/gjinnrvmp.sHtML

new Intl.DateTimeFormat("zh-CN", { dateStyle: "medium" }).format(new Date())
来源：http://m.share.hesvh.cn/Article/details/gqqbjtivl.sHtML

[U107] JS：数字千分位
来源：http://wap.fehbvm.com/Article/details/gtlryddsv.sHtML

new Intl.NumberFormat("en-US").format(1234567)
来源：http://www.share.fehbvm.com/Article/details/gwzqajsdv.sHtML

[U108] JS：随机整数
来源：http://www.m.share.hesvh.cn/Article/details/gxlnicwnk.sHtML

Math.floor(Math.random() * (max - min + 1)) + min
来源：http://www.m.share.zdbjq.cn/Article/details/ghdekfiwh.sHtML

[U109] JS：数组分组
来源：http://blog.fehbvm.com/Article/details/gpeemwiqs.sHtML

Object.groupBy(arr, x => x.type)
来源：http://blog.fehbvm.com/Article/details/gbwxbkuho.sHtML

[U110] JS：数组分块
来源：http://mobile.hesvh.cn/Article/details/gqalljeej.sHtML

arr.reduce((acc, x, i) => (i % size ? acc : [...acc, arr.slice(i, i + size)]), [])
来源：http://mobile.zdbjq.cn/Article/details/gyncheisg.sHtML

[U111] JS：对象转 Map
来源：http://read.share.hesvh.cn/Article/details/gloxsejhx.sHtML

new Map(Object.entries(obj))
来源：http://read.share.hesvh.cn/Article/details/gcshaerbr.sHtML

[U112] JS：字符串补位
来源：http://www.m.share.zdbjq.cn/Article/details/grkkffito.sHtML

"7".padStart(3, "0")
来源：http://3g.zdbjq.cn/Article/details/ggjrneaaz.sHtML

[U113] JS：正则替换全部
来源：http://mobile.zdbjq.cn/Article/details/gsswnmadl.sHtML

s.replaceAll("a", "b")
来源：http://blog.fehbvm.com/Article/details/glegznzde.sHtML

[U114] JS：JSON 深比较
来源：http://read.share.zdbjq.cn/Article/details/gidwquxio.sHtML

JSON.stringify(a) === JSON.stringify(b)
来源：http://blog.hesvh.cn/Article/details/gewwmvjdj.sHtML

[U115] JS：生成 UUID
来源：http://3g.hesvh.cn/Article/details/ghcidqexz.sHtML

crypto.randomUUID()
来源：http://m.share.zdbjq.cn/Article/details/gffowefda.sHtML

[U116] JS：类型检查（JSDoc）
来源：http://mobile.fehbvm.com/Article/details/gvjkyttvh.sHtML

/** @param {string} name */ function f(name) {}
来源：http://read.share.fehbvm.com/Article/details/gdufhnsef.sHtML

[U117] JS：单元测试
来源：http://www.share.fehbvm.com/Article/details/gxdbeaptl.sHtML

npm i -D vitest;  npx vitest
来源：http://www.m.share.zdbjq.cn/Article/details/gscuhouko.sHtML

[U118] JS：开发服务器
来源：http://www.m.share.zdbjq.cn/Article/details/gffqdoynt.sHtML

npm i -D vite;  npx vite
来源：http://read.share.zdbjq.cn/Article/details/gyfsdqahi.sHtML

[U119] JS：生产构建
来源：http://wap.zdbjq.cn/Article/details/gvcejaqyp.sHtML

npx vite build
来源：http://www.blog.fehbvm.com/Article/details/gmybdtdnn.sHtML

[U120] JS：读取环境变量（Vite）
来源：http://baike.fehbvm.com/Article/details/gdphkhiql.sHtML

import.meta.env.VITE_API_URL
来源：http://www.m.share.fehbvm.com/Article/details/ggfxpldpy.sHtML

================================================================================
来源：http://mobile.fehbvm.com/Article/details/gbhablmgr.sHtML

统计汇总
来源：http://baike.zdbjq.cn/Article/details/gdpiprtry.sHtML

================================================================================
来源：http://baike.hesvh.cn/Article/details/gjkcbndbl.sHtML

按语言统计（条）：
来源：http://www.share.fehbvm.com/Article/details/gorshnpak.sHtML

Python ......... 252
来源：http://www.blog.fehbvm.com/Article/details/gceudhzwq.sHtML

PHP ............ 252
来源：http://www.blog.hesvh.cn/Article/details/gzwglzdzj.sHtML

JavaScript ..... 252
来源：http://baike.fehbvm.com/Article/details/gewyjrwjk.sHtML

TypeScript ..... 212
来源：http://m.share.fehbvm.com/Article/details/gzjkkrdnm.sHtML

Java ........... 212
来源：http://www.blog.zdbjq.cn/Article/details/gskyuylfi.sHtML

Go ............. 212
来源：http://www.m.share.zdbjq.cn/Article/details/gkqzwcuji.sHtML

Ruby ........... 212
来源：http://wap.hesvh.cn/Article/details/gnkktumoq.sHtML

C# ............. 212
来源：http://3g.fehbvm.com/Article/details/gkgowlsbi.sHtML

C .............. 30
来源：http://www.share.hesvh.cn/Article/details/giqkxvlvw.sHtML

C++ ............ 30
来源：http://wap.zdbjq.cn/Article/details/gdtpbzdsd.sHtML

SQL ............ 90
来源：http://www.m.share.hesvh.cn/Article/details/gzrzbpzfm.sHtML

Bash ........... 80
来源：http://read.share.zdbjq.cn/Article/details/gkigojoeh.sHtML

Kotlin ......... 15
来源：http://mobile.fehbvm.com/Article/details/goskuhouv.sHtML

Swift .......... 15
来源：http://wap.hesvh.cn/Article/details/ggdahfjww.sHtML

Lua ............ 10
来源：http://read.share.zdbjq.cn/Article/details/gvkhtvmnf.sHtML

Perl ........... 10
来源：http://www.m.share.fehbvm.com/Article/details/ghydpljpt.sHtML

Scala .......... 10
来源：http://m.share.zdbjq.cn/Article/details/gugzpcruv.sHtML

------------------------------------
来源：http://3g.zdbjq.cn/Article/details/gzcphbdnc.sHtML

合计 ........... 2106 条
来源：http://www.blog.fehbvm.com/Article/details/gulhwvggf.sHtML

按章节统计：
来源：http://wap.zdbjq.cn/Article/details/gbnijlbaq.sHtML

A 基础语法与类型       26 个任务 × 8 语言 =  208
来源：http://www.blog.hesvh.cn/Article/details/gltmfltje.sHtML

B 流程控制             16 个任务 × 8 语言 =  128
来源：http://mobile.hesvh.cn/Article/details/gegmoeqvh.sHtML

C 函数与作用域         16 个任务 × 8 语言 =  128
来源：http://baike.fehbvm.com/Article/details/ggpsopmvp.sHtML

D 数组 / 列表 / 集合   26 个任务 × 8 语言 =  208
来源：http://www.m.share.hesvh.cn/Article/details/gxpyaufdj.sHtML

E 字符串处理           22 个任务 × 8 语言 =  176
来源：http://blog.fehbvm.com/Article/details/gmmqtgxoa.sHtML

F 文件与目录           12 个任务 × 8 语言 =   96
来源：http://baike.zdbjq.cn/Article/details/gabejfmxe.sHtML

G 面向对象             16 个任务 × 8 语言 =  128
来源：http://mobile.zdbjq.cn/Article/details/gnsvlgiio.sHtML

H 异常与错误处理       10 个任务 × 8 语言 =   80
来源：http://blog.hesvh.cn/Article/details/gahloqmpq.sHtML

I 正则表达式            8 个任务 × 8 语言 =   64
来源：http://www.m.share.fehbvm.com/Article/details/gqxrputsm.sHtML

J 日期与时间           10 个任务 × 8 语言 =   80
来源：http://wap.zdbjq.cn/Article/details/gtanqslfn.sHtML

K JSON 与序列化         8 个任务 × 8 语言 =   64
来源：http://3g.zdbjq.cn/Article/details/grfnvpsfc.sHtML

L 网络请求              8 个任务 × 8 语言 =   64
来源：http://blog.fehbvm.com/Article/details/ghwymqdzr.sHtML

M 命令行 / 进程         8 个任务 × 8 语言 =   64
来源：http://baike.fehbvm.com/Article/details/gpbwhjkdv.sHtML

N 数据结构与算法       12 个任务 × 8 语言 =   96
来源：http://wap.hesvh.cn/Article/details/gxyjuasfm.sHtML

O 并发与异步            6 个任务 × 8 语言 =   48
来源：http://baike.hesvh.cn/Article/details/gcmpxsuoh.sHtML

P 常用工具函数          8 个任务 × 8 语言 =   64
来源：http://blog.hesvh.cn/Article/details/gkuclzqtq.sHtML

Q SQL 专题                              90
来源：http://mobile.zdbjq.cn/Article/details/gyjdtcqfv.sHtML

R Bash 专题                             80
来源：http://www.blog.hesvh.cn/Article/details/grlyqhdet.sHtML

S C / C++ 专题                          60
来源：http://m.share.zdbjq.cn/Article/details/gemojgyfw.sHtML

T 其他语言补充                          60
来源：http://baike.zdbjq.cn/Article/details/gtifckqqy.sHtML

U 高频实用片段                         120
来源：http://blog.hesvh.cn/Article/details/gvlayuxyq.sHtML

------------------------------------
来源：http://www.blog.zdbjq.cn/Article/details/grzoyedae.sHtML

合计                                  2106 条
来源：http://baike.fehbvm.com/Article/details/grpprkfdk.sHtML

--------------------------------------------------------------------------------
来源：http://www.blog.hesvh.cn/Article/details/gedelqean.sHtML

使用提醒
来源：http://mobile.zdbjq.cn/Article/details/gtxyevrow.sHtML

--------------------------------------------------------------------------------
来源：http://www.blog.hesvh.cn/Article/details/ghltmzhuu.sHtML

1. 示例追求"最小可用"，正式项目中请补齐导入、错误处理与边界判断。
来源：http://baike.fehbvm.com/Article/details/gsjrlgiuw.sHtML

2. 涉及文件、网络、数据库的示例，注意资源释放与异常捕获。
来源：http://wap.hesvh.cn/Article/details/ghoqfmmfq.sHtML

3. 语言版本差异较大（如 Python 3.10 的 match、Java 17 的 record/switch 箭头），
来源：http://mobile.zdbjq.cn/Article/details/gvlampoex.sHtML

在旧版本上使用前请先确认语法支持情况。
来源：http://m.share.zdbjq.cn/Article/details/greqikvyx.sHtML

4. 标注"手写"的条目是因为该语言缺少对应内置能力，实际项目中可引入成熟库。
来源：http://www.m.share.fehbvm.com/Article/details/gkydnyhej.sHtML

—— 文件结束 ——
来源：http://www.share.hesvh.cn/Article/details/gezwdcxxf.sHtML

================================================================================
来源：http://blog.zdbjq.cn/Article/details/gsmwlcrwl.sHtML

程序语言常见例子速查手册（2024 版）
来源：http://blog.zdbjq.cn/Article/details/gqvyaknns.sHtML

Common Programming Examples Cheat Book
来源：http://read.share.fehbvm.com/Article/details/gubupexwy.sHtML

================================================================================
来源：http://m.share.fehbvm.com/Article/details/ghkfyxymr.sHtML

【收录内容】
来源：http://3g.hesvh.cn/Article/details/gosrcqsan.sHtML

覆盖 12 种语言 / 语法与常见 API：
来源：http://baike.fehbvm.com/Article/details/gsnhyzpqd.sHtML

Python · PHP · JavaScript · TypeScript · Java · Go · Ruby · C#
来源：http://www.m.share.hesvh.cn/Article/details/gaouyalxq.sHtML

SQL · Bash · C · C++
来源：http://3g.fehbvm.com/Article/details/gxereacir.sHtML

按「任务」分组：每个任务下按语言各给出一条最小可用示例。
来源：http://m.share.zdbjq.cn/Article/details/gaddiqyvm.sHtML

【使用说明】
来源：http://wap.hesvh.cn/Article/details/gmqhxszlq.sHtML

1. 每个任务形如 "[编号] 任务名"，下面每行以语言标记开头：
来源：http://mobile.hesvh.cn/Article/details/gfoytrmiu.sHtML

Py:    Python        PHP:   PHP           JS:    JavaScript
来源：http://wap.fehbvm.com/Article/details/gvbmteykd.sHtML

TS:    TypeScript    Java:  Java          Go:    Go
来源：http://read.share.hesvh.cn/Article/details/gjslythez.sHtML

Ruby:  Ruby          C#:    C#            SQL:   SQL
来源：http://www.blog.hesvh.cn/Article/details/ghohoyqix.sHtML

Bash:  Shell         C:     C             C++:   C++
来源：http://m.share.zdbjq.cn/Article/details/gtpnpecxr.sHtML

2. 示例只展示核心写法，刻意省略 import / require / include / using 等样板代码。
来源：http://blog.fehbvm.com/Article/details/gmzmdcqpj.sHtML

需要完整可运行文件时，请自行补齐当前语言的导入语句。
来源：http://m.share.hesvh.cn/Article/details/gimsdjvkf.sHtML

3. 语法基准：Python 3.10+ / PHP 8.1+ / ES2020+ / TypeScript 5 / Java 17 /
来源：http://3g.zdbjq.cn/Article/details/gghtgajzj.sHtML

Go 1.21+ / Ruby 3.x / C# 10+ / C17 / C++17。
来源：http://www.share.zdbjq.cn/Article/details/gpuglpdsw.sHtML

4. 检索建议：用编辑器或浏览器 Ctrl+F 搜关键词，如 "排序" "读取文件" "正则"。
来源：http://3g.zdbjq.cn/Article/details/gvjoocave.sHtML

5. 标记为 "// 无" 表示该语言没有对应的一等语法，需用替代写法（示例给出替代方案）。
来源：http://www.blog.hesvh.cn/Article/details/gfxitzhhy.sHtML

6. 符号 "⏎" 表示代码在此处换行（主要用于 Python 等强制缩进、无法压成一行的结构）。
来源：http://www.blog.fehbvm.com/Article/details/gdopocfdh.sHtML

【文件统计】
来源：http://read.share.hesvh.cn/Article/details/ghowubifn.sHtML

语言示例共 2106 条，分布见本文末尾的「统计汇总」。
来源：http://wap.zdbjq.cn/Article/details/gqtmspfvp.sHtML

--------------------------------------------------------------------------------
来源：http://wap.zdbjq.cn/Article/details/grbrhoqkw.sHtML

目  录
来源：http://read.share.zdbjq.cn/Article/details/guvsmxymx.sHtML

--------------------------------------------------------------------------------
来源：http://read.share.fehbvm.com/Article/details/gcykbmbpp.sHtML

A. 基础语法与类型              （第 1 节，26 个任务，208 条）
来源：http://www.blog.zdbjq.cn/Article/details/gzehkdqow.sHtML

B. 流程控制                    （第 2 节，16 个任务，128 条）
来源：http://baike.zdbjq.cn/Article/details/gxsizsqks.sHtML

C. 函数与作用域                （第 3 节，16 个任务，128 条）
来源：http://baike.hesvh.cn/Article/details/gslujhyhn.sHtML

D. 数组 / 列表 / 集合          （第 4 节，26 个任务，208 条）
来源：http://baike.fehbvm.com/Article/details/gxgxtqwfi.sHtML

E. 字符串处理                  （第 5 节，22 个任务，176 条）
来源：http://www.share.zdbjq.cn/Article/details/gcmkaplms.sHtML


<!-- 参考信息 -->