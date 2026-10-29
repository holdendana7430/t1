代发 wailian999

[U21] Py：自定义上下文管理器
来源：http://wap.zdbjq.cn/Article/details/gondqwqfd.sHtML

@contextlib.contextmanager
来源：http://blog.fehbvm.com/Article/details/glpihtsps.sHtML

[U22] Py：矩阵转置
来源：http://read.share.fehbvm.com/Article/details/gdqukveip.sHtML

list(zip(*m))
来源：http://www.share.hesvh.cn/Article/details/gcqnnrwip.sHtML

[U23] Py：分块读取大文件
来源：http://baike.fehbvm.com/Article/details/gbbigzbzj.sHtML

for chunk in iter(lambda: f.read(8192), b""):
来源：http://3g.fehbvm.com/Article/details/geescjuir.sHtML

[U24] Py：路径操作
来源：http://blog.fehbvm.com/Article/details/grflfsryz.sHtML

Path("a/b.txt").parent.mkdir(parents=True, exist_ok=True)
来源：http://blog.fehbvm.com/Article/details/gcikzryoj.sHtML

[U25] Py：CSV 按字典读
来源：http://www.blog.zdbjq.cn/Article/details/gobhbvqqa.sHtML

csv.DictReader(f)
来源：http://mobile.hesvh.cn/Article/details/gnuthejed.sHtML

[U26] Py：并发下载
来源：http://www.blog.hesvh.cn/Article/details/gpchqzfij.sHtML

ThreadPoolExecutor(max_workers=8).map(fetch, urls)
来源：http://m.share.zdbjq.cn/Article/details/guljipzbh.sHtML

[U27] Py：异步 HTTP
来源：http://m.share.zdbjq.cn/Article/details/gkqmktyiy.sHtML

aiohttp.ClientSession() 配合 async with
来源：http://read.share.zdbjq.cn/Article/details/gjqtlxbdg.sHtML

[U28] Py：类型别名
来源：http://www.blog.fehbvm.com/Article/details/gzjldubms.sHtML

UserId = int
来源：http://www.share.fehbvm.com/Article/details/gtjznrmtw.sHtML

[U29] Py：属性校验
来源：http://baike.zdbjq.cn/Article/details/gxrhvcogh.sHtML

@property 与 @x.setter 配合
来源：http://mobile.fehbvm.com/Article/details/gxgmglksm.sHtML

[U30] Py：数据类
来源：http://www.share.hesvh.cn/Article/details/gqicblklg.sHtML

@dataclass(slots=True)
来源：http://www.share.hesvh.cn/Article/details/gguvrosyi.sHtML

[U31] Py：单测
来源：http://read.share.fehbvm.com/Article/details/gtrttyogr.sHtML

python -m pytest -q
来源：http://wap.zdbjq.cn/Article/details/gdtyuaktt.sHtML

[U32] Py：代码格式化
来源：http://mobile.zdbjq.cn/Article/details/ghfmtjdmy.sHtML

ruff format . && ruff check --fix .
来源：http://baike.zdbjq.cn/Article/details/gejsugtiw.sHtML

[U33] Py：打包发布
来源：http://m.share.hesvh.cn/Article/details/gmgqtaahm.sHtML

python -m build  （依赖 pyproject.toml）
来源：http://3g.hesvh.cn/Article/details/gkaaydlnk.sHtML

[U34] Py：判断编码
来源：http://www.blog.zdbjq.cn/Article/details/gnyktwlij.sHtML

chardet.detect(raw)
来源：http://www.blog.fehbvm.com/Article/details/ggvyapgxw.sHtML

[U35] Py：发送邮件
来源：http://read.share.zdbjq.cn/Article/details/goupfcwci.sHtML

smtplib.SMTP_SSL(...).send_message(msg)
来源：http://wap.fehbvm.com/Article/details/gjrjfwwyz.sHtML

[U36] Py：定时任务
来源：http://read.share.zdbjq.cn/Article/details/gvwvtdmul.sHtML

schedule.every(10).minutes.do(job)
来源：http://read.share.zdbjq.cn/Article/details/gocugfrnd.sHtML

[U37] Py：读写 Excel
来源：http://mobile.zdbjq.cn/Article/details/garxfuirc.sHtML

pandas.read_excel / DataFrame.to_excel
来源：http://m.share.fehbvm.com/Article/details/gxeemjhul.sHtML

[U38] Py：获取脚本所在目录
来源：http://3g.hesvh.cn/Article/details/gyfbkwmyn.sHtML

Path(__file__).resolve().parent
来源：http://3g.fehbvm.com/Article/details/gjgfatkil.sHtML

[U39] Py：判断是否在交互环境
来源：http://blog.hesvh.cn/Article/details/gqpqgnudo.sHtML

sys.stdout.isatty()
来源：http://baike.hesvh.cn/Article/details/gcojethue.sHtML

[U40] Py：打印到标准错误
来源：http://3g.fehbvm.com/Article/details/gdaouryrs.sHtML

print("err", file=sys.stderr)
来源：http://mobile.fehbvm.com/Article/details/gpqxmwezq.sHtML

[U41] PHP：初始化 Composer 项目
来源：http://m.share.zdbjq.cn/Article/details/gedlhyhqr.sHtML

composer init;  composer require guzzlehttp/guzzle
来源：http://blog.hesvh.cn/Article/details/ggbwznysd.sHtML

[U42] PHP：PSR-4 自动加载
来源：http://www.blog.fehbvm.com/Article/details/gifisguqv.sHtML

"autoload": { "psr-4": { "App\\": "src/" } }
来源：http://blog.fehbvm.com/Article/details/gbrkfikzv.sHtML

[U43] PHP：声明命名空间
来源：http://blog.fehbvm.com/Article/details/gwcldqnxs.sHtML

namespace App\Http;
来源：http://m.share.zdbjq.cn/Article/details/gwezmnbbf.sHtML

[U44] PHP：开启严格类型
来源：http://read.share.zdbjq.cn/Article/details/gamjkwqac.sHtML

declare(strict_types=1);
来源：http://www.m.share.hesvh.cn/Article/details/gqhwvkmnw.sHtML

[U45] PHP：类型声明与返回类型
来源：http://m.share.hesvh.cn/Article/details/gnwojtrxb.sHtML

function add(int $a, int $b): int { return $a + $b; }
来源：http://3g.hesvh.cn/Article/details/gxxuobdab.sHtML

[U46] PHP：可空类型
来源：http://www.share.zdbjq.cn/Article/details/gnbooyjsm.sHtML

?string $name = null
来源：http://www.m.share.fehbvm.com/Article/details/gmglutzir.sHtML

[U47] PHP：联合类型
来源：http://wap.zdbjq.cn/Article/details/ghmhkpzrh.sHtML

int|string $id
来源：http://blog.hesvh.cn/Article/details/gthugmezf.sHtML

[U48] PHP：纯枚举
来源：http://read.share.hesvh.cn/Article/details/gwbvfcqzn.sHtML

enum Status: string { case Active = "active"; case Off = "off"; }
来源：http://baike.fehbvm.com/Article/details/ggauqcpgj.sHtML

[U49] PHP：只读属性
来源：http://blog.fehbvm.com/Article/details/gojpmtsxc.sHtML

public readonly string $name
来源：http://mobile.fehbvm.com/Article/details/ghrpyjidu.sHtML

[U50] PHP：构造器属性提升
来源：http://m.share.zdbjq.cn/Article/details/gtnbnasqf.sHtML

public function __construct(private int $id) {}
来源：http://blog.fehbvm.com/Article/details/gjyzqiwnv.sHtML

[U51] PHP：数组解构
来源：http://blog.zdbjq.cn/Article/details/gssygtduq.sHtML

[$a, $b] = $arr;
来源：http://wap.zdbjq.cn/Article/details/gactvjajw.sHtML

[U52] PHP：箭头函数
来源：http://www.m.share.hesvh.cn/Article/details/givaghjzg.sHtML

$double = fn($x) => $x * 2;
来源：http://baike.fehbvm.com/Article/details/gtvmvzicg.sHtML

[U53] PHP：空合并运算符
来源：http://3g.fehbvm.com/Article/details/gxzvqyhlu.sHtML

$v = $a ?? $b ?? "default";
来源：http://wap.zdbjq.cn/Article/details/gyiauxbse.sHtML

[U54] PHP：空安全调用
来源：http://blog.zdbjq.cn/Article/details/gvaqjlxpg.sHtML

$obj?->method()
来源：http://www.m.share.fehbvm.com/Article/details/gvrlpjsfy.sHtML

[U55] PHP：match 表达式
来源：http://www.blog.zdbjq.cn/Article/details/gfbbegtla.sHtML

$s = match($x) { 1 => "一", default => "其他" };
来源：http://wap.hesvh.cn/Article/details/gltzrxxjk.sHtML

[U56] PHP：命名参数
来源：http://www.share.hesvh.cn/Article/details/glhvhmbmb.sHtML

f(a: 1, b: 2)
来源：http://www.share.fehbvm.com/Article/details/gqadmbkuz.sHtML

[U57] PHP：字符串插值
来源：http://www.m.share.hesvh.cn/Article/details/glyokqpqh.sHtML

"值: {$a}"
来源：http://read.share.hesvh.cn/Article/details/gnheoodoc.sHtML

[U58] PHP：数组三件套
来源：http://www.share.zdbjq.cn/Article/details/gozwwnilr.sHtML

array_map($f, $a);  array_filter($a, $f);  array_reduce($a, $f, 0);
来源：http://wap.hesvh.cn/Article/details/gqlzdbsde.sHtML

[U59] PHP：自定义排序
来源：http://www.share.fehbvm.com/Article/details/gpfbnldsh.sHtML

usort($arr, fn($a, $b) => $a["age"] <=> $b["age"]);
来源：http://3g.zdbjq.cn/Article/details/gabyyyxzk.sHtML

[U60] PHP：JSON 编解码
来源：http://www.blog.hesvh.cn/Article/details/giwqgcsme.sHtML

json_encode($d, JSON_UNESCAPED_UNICODE);  json_decode($s, true);
来源：http://mobile.fehbvm.com/Article/details/gyzvjtzso.sHtML

[U61] PHP：正则
来源：http://baike.hesvh.cn/Article/details/gthzoataa.sHtML

preg_match('/(\d+)/', $s, $m);  preg_replace('/\d+/', '#', $s);
来源：http://blog.hesvh.cn/Article/details/gezrnazrw.sHtML

[U62] PHP：日期对象
来源：http://wap.zdbjq.cn/Article/details/gljracfri.sHtML

(new DateTimeImmutable())->format("Y-m-d");
来源：http://www.m.share.fehbvm.com/Article/details/gphiahond.sHtML

[U63] PHP：文件读写
来源：http://blog.fehbvm.com/Article/details/gyvsievom.sHtML

file_get_contents($f);  file_put_contents($f, $data);
来源：http://www.blog.hesvh.cn/Article/details/giqpwqpuo.sHtML

[U64] PHP：目录遍历
来源：http://wap.zdbjq.cn/Article/details/grsrzjihs.sHtML

glob("dir/*.php");  scandir("dir");
来源：http://m.share.hesvh.cn/Article/details/gjbstadfg.sHtML

[U65] PHP：会话
来源：http://m.share.fehbvm.com/Article/details/gosxvkcbs.sHtML

session_start();  $_SESSION["uid"] = 1;
来源：http://www.m.share.fehbvm.com/Article/details/gfjhuzuqt.sHtML

[U66] PHP：设置 Cookie
来源：http://3g.hesvh.cn/Article/details/glzlnoceg.sHtML

setcookie("token", $v, ["httponly" => true, "samesite" => "Lax"]);
来源：http://www.m.share.hesvh.cn/Article/details/gfruwrmfb.sHtML

[U67] PHP：处理文件上传
来源：http://m.share.hesvh.cn/Article/details/gnblvujcv.sHtML

$_FILES["file"]["tmp_name"] 与 move_uploaded_file()
来源：http://mobile.fehbvm.com/Article/details/gcdeaflxj.sHtML

[U68] PHP：PDO 连接
来源：http://mobile.hesvh.cn/Article/details/gmuglyoxg.sHtML

$pdo = new PDO("mysql:host=localhost;dbname=app", "root", "");
来源：http://m.share.fehbvm.com/Article/details/gfbhegghr.sHtML

[U69] PHP：PDO 预处理
来源：http://baike.fehbvm.com/Article/details/gfwwshbdx.sHtML

$stmt = $pdo->prepare("SELECT * FROM users WHERE id = ?");  $stmt->execute([$id]);
来源：http://baike.hesvh.cn/Article/details/gsqkqtbii.sHtML

[U70] PHP：PDO 事务
来源：http://blog.hesvh.cn/Article/details/gocinlmph.sHtML

$pdo->beginTransaction();  $pdo->commit();  $pdo->rollBack();
来源：http://3g.fehbvm.com/Article/details/gzteaskwi.sHtML

[U71] PHP：抛出异常
来源：http://3g.hesvh.cn/Article/details/gnoyumeds.sHtML

throw new RuntimeException("失败", 500);
来源：http://www.blog.hesvh.cn/Article/details/gzaegbkfx.sHtML

[U72] PHP：写错误日志
来源：http://www.blog.fehbvm.com/Article/details/glilfbiby.sHtML

error_log("失败: " . $e->getMessage());
来源：http://blog.zdbjq.cn/Article/details/ggcwfkpcj.sHtML

[U73] PHP：读取 ini 配置
来源：http://wap.fehbvm.com/Article/details/gnbybqcku.sHtML

parse_ini_file("config.ini", true)
来源：http://m.share.hesvh.cn/Article/details/gblznwiqk.sHtML

[U74] PHP：读取环境变量
来源：http://wap.fehbvm.com/Article/details/gfzoskbln.sHtML

getenv("APP_ENV") ?: "production"
来源：http://www.share.hesvh.cn/Article/details/gvzqtgoeq.sHtML

[U75] PHP：依赖注入
来源：http://baike.zdbjq.cn/Article/details/gveqogegw.sHtML

composer require psr/container
来源：http://baike.zdbjq.cn/Article/details/glcmslaeq.sHtML

[U76] PHP：简单路由
来源：http://www.share.hesvh.cn/Article/details/gpsqrfnqh.sHtML

$path = parse_url($_SERVER["REQUEST_URI"], PHP_URL_PATH);
来源：http://mobile.hesvh.cn/Article/details/gtjjvhhli.sHtML

[U77] PHP：模板渲染
来源：http://www.m.share.zdbjq.cn/Article/details/gofdwovfa.sHtML

composer require twig/twig
来源：http://wap.fehbvm.com/Article/details/gajglpjyf.sHtML

[U78] PHP：单元测试
来源：http://www.m.share.fehbvm.com/Article/details/ghmcpqkuq.sHtML

composer require --dev phpunit/phpunit
来源：http://blog.fehbvm.com/Article/details/gpfudasab.sHtML

[U79] PHP：静态分析
来源：http://www.blog.hesvh.cn/Article/details/gyyyvclgm.sHtML

composer require --dev phpstan/phpstan
来源：http://baike.fehbvm.com/Article/details/gmqkzaxgw.sHtML

[U80] PHP：代码规范修复
来源：http://wap.zdbjq.cn/Article/details/giumaykve.sHtML

composer require --dev friendsofphp/php-cs-fixer
来源：http://www.m.share.fehbvm.com/Article/details/gprlaczae.sHtML

[U81] JS：初始化项目
来源：http://blog.fehbvm.com/Article/details/gzxpgftol.sHtML

npm init -y;  npm i express
来源：http://read.share.hesvh.cn/Article/details/girzojwlr.sHtML

[U82] JS：package.json 脚本
来源：http://baike.fehbvm.com/Article/details/gnhdpxvbr.sHtML

"scripts": { "dev": "vite", "build": "vite build" }
来源：http://m.share.hesvh.cn/Article/details/gtndizfsm.sHtML

[U83] JS：ES Module 导入导出
来源：http://blog.fehbvm.com/Article/details/gjalbreyg.sHtML

export const a = 1;  import { a } from "./m.js";
来源：http://www.share.fehbvm.com/Article/details/gyqqxvekh.sHtML

[U84] JS：CommonJS 写法
来源：http://www.share.hesvh.cn/Article/details/ggqimvhzq.sHtML

module.exports = { a };  const { a } = require("./m");
来源：http://blog.zdbjq.cn/Article/details/gtyvithyh.sHtML

[U85] JS：可选链
来源：http://baike.zdbjq.cn/Article/details/gillhutye.sHtML

a?.b?.c
来源：http://www.blog.fehbvm.com/Article/details/gelvsmelu.sHtML

[U86] JS：空值合并
来源：http://www.m.share.fehbvm.com/Article/details/gsdjmdlee.sHtML

a ?? b
来源：http://blog.zdbjq.cn/Article/details/gfbajnjcn.sHtML

[U87] JS：解构默认值
来源：http://www.m.share.zdbjq.cn/Article/details/gigszytlz.sHtML

const { a = 1, b = 2 } = obj;
来源：http://www.m.share.zdbjq.cn/Article/details/gdskfpdak.sHtML

[U88] JS：对象展开合并
来源：http://baike.fehbvm.com/Article/details/gybjhxaog.sHtML

{ ...a, ...b }
来源：http://3g.hesvh.cn/Article/details/gdmffslcd.sHtML

[U89] JS：数组去重
来源：http://www.blog.fehbvm.com/Article/details/gvhionkpq.sHtML

[...new Set(arr)]
来源：http://www.blog.hesvh.cn/Article/details/gfwkpmdlc.sHtML

[U90] JS：数字数组排序
来源：http://read.share.zdbjq.cn/Article/details/ggpwqjveh.sHtML

[...arr].sort((a, b) => a - b)
来源：http://wap.zdbjq.cn/Article/details/gpdppgval.sHtML

[U91] JS：对象键值遍历
来源：http://3g.zdbjq.cn/Article/details/gxgiyqeva.sHtML

Object.entries(obj).forEach(([k, v]) => {});
来源：http://blog.zdbjq.cn/Article/details/gsegiimim.sHtML

[U92] JS：深拷贝
来源：http://3g.hesvh.cn/Article/details/grspxsefv.sHtML

structuredClone(obj)
来源：http://m.share.fehbvm.com/Article/details/gjlyttsyd.sHtML

[U93] JS：模板字符串
来源：http://blog.hesvh.cn/Article/details/gwuhvfgze.sHtML

`共 ${n} 条`
来源：http://read.share.hesvh.cn/Article/details/goohcjuoz.sHtML

[U94] JS：箭头函数
来源：http://www.share.zdbjq.cn/Article/details/gyhqfwvhr.sHtML

const double = x => x * 2;
来源：http://m.share.zdbjq.cn/Article/details/gmeiaxqbd.sHtML

[U95] JS：Promise 包装
来源：http://3g.zdbjq.cn/Article/details/gbufwsitu.sHtML

new Promise((resolve, reject) => {})
来源：http://baike.hesvh.cn/Article/details/gsdumspar.sHtML

[U96] JS：async/await 与异常
来源：http://m.share.fehbvm.com/Article/details/govkndexk.sHtML

try { const d = await f(); } catch (e) { console.error(e); }
来源：http://read.share.fehbvm.com/Article/details/ghasgdlzo.sHtML

[U97] JS：并发请求
来源：http://www.m.share.zdbjq.cn/Article/details/ggisljchx.sHtML

await Promise.all(urls.map(u => fetch(u)))
来源：http://baike.fehbvm.com/Article/details/gyaexassr.sHtML

[U98] JS：fetch 带 JSON
来源：http://3g.fehbvm.com/Article/details/geqnvwqzv.sHtML

await fetch(url, { method: "POST", headers: { "Content-Type": "application/json" }, body: JSON.stringify(d) })
来源：http://baike.zdbjq.cn/Article/details/gipykdkto.sHtML

[U99] JS：事件监听
来源：http://www.share.fehbvm.com/Article/details/gxaukhsic.sHtML

el.addEventListener("click", e => {})
来源：http://www.blog.hesvh.cn/Article/details/gsczzgxyv.sHtML

[U100] JS：DOM 查询
来源：http://www.blog.zdbjq.cn/Article/details/gpwxukryw.sHtML

document.querySelector(".item")
来源：http://www.blog.zdbjq.cn/Article/details/gfoedvnrg.sHtML

[U101] JS：classList 操作
来源：http://wap.fehbvm.com/Article/details/gzbwruqzo.sHtML

el.classList.toggle("active")
来源：http://baike.zdbjq.cn/Article/details/gncowvcnz.sHtML

[U102] JS：本地存储
来源：http://www.blog.fehbvm.com/Article/details/geaohswwz.sHtML

localStorage.setItem("k", JSON.stringify(v))
来源：http://m.share.hesvh.cn/Article/details/gvaezrziy.sHtML

[U103] JS：定时器
来源：http://www.m.share.hesvh.cn/Article/details/ginfhwqdl.sHtML

setTimeout(fn, 1000);  setInterval(fn, 1000);
来源：http://3g.fehbvm.com/Article/details/gabldammo.sHtML

[U104] JS：防抖
来源：http://read.share.hesvh.cn/Article/details/gaatqakrm.sHtML

const debounce = (fn, ms) => { let t; return (...a) => { clearTimeout(t); t = setTimeout(() => fn(...a), ms); }; };
来源：http://www.share.hesvh.cn/Article/details/gwyfhouag.sHtML

[U105] JS：节流
来源：http://www.m.share.fehbvm.com/Article/details/gdwzewyys.sHtML

const throttle = (fn, ms) => { let last = 0; return (...a) => { const n = Date.now(); if (n - last >= ms) { last = n; fn(...a); } }; };
来源：http://m.share.fehbvm.com/Article/details/gbazcgovb.sHtML

[U106] JS：日期格式化
来源：http://m.share.fehbvm.com/Article/details/gdkqkrfqt.sHtML

new Intl.DateTimeFormat("zh-CN", { dateStyle: "medium" }).format(new Date())
来源：http://3g.zdbjq.cn/Article/details/gfrwqihou.sHtML

[U107] JS：数字千分位
来源：http://blog.zdbjq.cn/Article/details/gndnehxiz.sHtML

new Intl.NumberFormat("en-US").format(1234567)
来源：http://mobile.fehbvm.com/Article/details/gziluqqel.sHtML

[U108] JS：随机整数
来源：http://mobile.zdbjq.cn/Article/details/gdlydbdnm.sHtML

Math.floor(Math.random() * (max - min + 1)) + min
来源：http://mobile.zdbjq.cn/Article/details/gophudcnb.sHtML

[U109] JS：数组分组
来源：http://www.m.share.hesvh.cn/Article/details/gacwusgwg.sHtML

Object.groupBy(arr, x => x.type)
来源：http://baike.zdbjq.cn/Article/details/geykhxkvj.sHtML

[U110] JS：数组分块
来源：http://read.share.zdbjq.cn/Article/details/gsdngmiog.sHtML

arr.reduce((acc, x, i) => (i % size ? acc : [...acc, arr.slice(i, i + size)]), [])
来源：http://www.share.hesvh.cn/Article/details/gmdswufoe.sHtML

[U111] JS：对象转 Map
来源：http://read.share.hesvh.cn/Article/details/gosnlwycy.sHtML

new Map(Object.entries(obj))
来源：http://wap.fehbvm.com/Article/details/gjhbnzzcr.sHtML

[U112] JS：字符串补位
来源：http://m.share.fehbvm.com/Article/details/grihwjlll.sHtML

"7".padStart(3, "0")
来源：http://www.m.share.zdbjq.cn/Article/details/gpkavtfau.sHtML

[U113] JS：正则替换全部
来源：http://baike.zdbjq.cn/Article/details/gvtxnjjun.sHtML

s.replaceAll("a", "b")
来源：http://baike.hesvh.cn/Article/details/gmmgfbsug.sHtML

[U114] JS：JSON 深比较
来源：http://wap.fehbvm.com/Article/details/gokrxbbqc.sHtML

JSON.stringify(a) === JSON.stringify(b)
来源：http://www.share.hesvh.cn/Article/details/gjxgzjpdz.sHtML

[U115] JS：生成 UUID
来源：http://mobile.hesvh.cn/Article/details/gbfmccbax.sHtML

crypto.randomUUID()
来源：http://www.m.share.hesvh.cn/Article/details/glqfrrqlm.sHtML

[U116] JS：类型检查（JSDoc）
来源：http://mobile.fehbvm.com/Article/details/gjfvbfehg.sHtML

/** @param {string} name */ function f(name) {}
来源：http://wap.fehbvm.com/Article/details/gmmpneasj.sHtML

[U117] JS：单元测试
来源：http://baike.zdbjq.cn/Article/details/gtjtsacav.sHtML

npm i -D vitest;  npx vitest
来源：http://www.blog.zdbjq.cn/Article/details/gppurrbrt.sHtML

[U118] JS：开发服务器
来源：http://wap.zdbjq.cn/Article/details/gujcpmkdz.sHtML

npm i -D vite;  npx vite
来源：http://3g.zdbjq.cn/Article/details/gdqgkzieb.sHtML

[U119] JS：生产构建
来源：http://3g.zdbjq.cn/Article/details/gvzcmvmpc.sHtML

npx vite build
来源：http://3g.hesvh.cn/Article/details/gjxedxzwt.sHtML

[U120] JS：读取环境变量（Vite）
来源：http://www.share.hesvh.cn/Article/details/gnbwwmmhx.sHtML

import.meta.env.VITE_API_URL
来源：http://baike.zdbjq.cn/Article/details/gytohehah.sHtML

================================================================================
来源：http://www.m.share.fehbvm.com/Article/details/gearmtrzd.sHtML

统计汇总
来源：http://www.blog.hesvh.cn/Article/details/genmfrzlm.sHtML

================================================================================
来源：http://m.share.fehbvm.com/Article/details/gpjkjquif.sHtML

按语言统计（条）：
来源：http://blog.hesvh.cn/Article/details/goriryubw.sHtML

Python ......... 252
来源：http://m.share.hesvh.cn/Article/details/guuqaujza.sHtML

PHP ............ 252
来源：http://baike.fehbvm.com/Article/details/givyqqvrz.sHtML

JavaScript ..... 252
来源：http://www.m.share.hesvh.cn/Article/details/ggifsdwge.sHtML

TypeScript ..... 212
来源：http://www.blog.hesvh.cn/Article/details/gxfzpgslf.sHtML

Java ........... 212
来源：http://mobile.zdbjq.cn/Article/details/gbvtbtupd.sHtML

Go ............. 212
来源：http://www.blog.fehbvm.com/Article/details/gdmcbtdvt.sHtML

Ruby ........... 212
来源：http://www.m.share.fehbvm.com/Article/details/gnahydbve.sHtML

C# ............. 212
来源：http://blog.zdbjq.cn/Article/details/gesqikxwr.sHtML

C .............. 30
来源：http://www.share.hesvh.cn/Article/details/gjqizotlj.sHtML

C++ ............ 30
来源：http://mobile.zdbjq.cn/Article/details/ggdspving.sHtML

SQL ............ 90
来源：http://wap.zdbjq.cn/Article/details/gozgyfznq.sHtML

Bash ........... 80
来源：http://blog.fehbvm.com/Article/details/guiguyevr.sHtML

Kotlin ......... 15
来源：http://wap.zdbjq.cn/Article/details/gipgkcogw.sHtML

Swift .......... 15
来源：http://m.share.hesvh.cn/Article/details/guhgbiddj.sHtML

Lua ............ 10
来源：http://mobile.fehbvm.com/Article/details/gvkidyyms.sHtML

Perl ........... 10
来源：http://m.share.zdbjq.cn/Article/details/ghtxellno.sHtML

Scala .......... 10
来源：http://3g.zdbjq.cn/Article/details/gilvrvkzh.sHtML

------------------------------------
来源：http://3g.fehbvm.com/Article/details/gohjugpvw.sHtML

合计 ........... 2106 条
来源：http://www.m.share.zdbjq.cn/Article/details/gfdzdciuz.sHtML

按章节统计：
来源：http://wap.hesvh.cn/Article/details/gyayplgui.sHtML

A 基础语法与类型       26 个任务 × 8 语言 =  208
来源：http://read.share.hesvh.cn/Article/details/grukussne.sHtML

B 流程控制             16 个任务 × 8 语言 =  128
来源：http://3g.zdbjq.cn/Article/details/gornhhbzt.sHtML

C 函数与作用域         16 个任务 × 8 语言 =  128
来源：http://3g.fehbvm.com/Article/details/geqidwldu.sHtML

D 数组 / 列表 / 集合   26 个任务 × 8 语言 =  208
来源：http://blog.hesvh.cn/Article/details/gystnejne.sHtML

E 字符串处理           22 个任务 × 8 语言 =  176
来源：http://www.share.zdbjq.cn/Article/details/gzwkawtiw.sHtML

F 文件与目录           12 个任务 × 8 语言 =   96
来源：http://www.blog.zdbjq.cn/Article/details/gfencrpua.sHtML

G 面向对象             16 个任务 × 8 语言 =  128
来源：http://baike.zdbjq.cn/Article/details/gxgkgvhxj.sHtML

H 异常与错误处理       10 个任务 × 8 语言 =   80
来源：http://www.share.hesvh.cn/Article/details/gilrkpvgg.sHtML

I 正则表达式            8 个任务 × 8 语言 =   64
来源：http://3g.hesvh.cn/Article/details/guptxcbqv.sHtML

J 日期与时间           10 个任务 × 8 语言 =   80
来源：http://www.m.share.hesvh.cn/Article/details/ghyqqciwx.sHtML

K JSON 与序列化         8 个任务 × 8 语言 =   64
来源：http://wap.zdbjq.cn/Article/details/gevnchnim.sHtML

L 网络请求              8 个任务 × 8 语言 =   64
来源：http://read.share.zdbjq.cn/Article/details/gyiohkrmu.sHtML

M 命令行 / 进程         8 个任务 × 8 语言 =   64
来源：http://www.blog.zdbjq.cn/Article/details/gdbvqhvra.sHtML

N 数据结构与算法       12 个任务 × 8 语言 =   96
来源：http://baike.fehbvm.com/Article/details/gymfrjnof.sHtML

O 并发与异步            6 个任务 × 8 语言 =   48
来源：http://3g.hesvh.cn/Article/details/gvhsoovix.sHtML

P 常用工具函数          8 个任务 × 8 语言 =   64
来源：http://www.blog.hesvh.cn/Article/details/gaiglekpa.sHtML

Q SQL 专题                              90
来源：http://wap.hesvh.cn/Article/details/gjnekdlib.sHtML

R Bash 专题                             80
来源：http://blog.zdbjq.cn/Article/details/gqanncivl.sHtML

S C / C++ 专题                          60
来源：http://www.share.zdbjq.cn/Article/details/gyvdwlhxk.sHtML

T 其他语言补充                          60
来源：http://www.m.share.zdbjq.cn/Article/details/gekrgbspn.sHtML

U 高频实用片段                         120
来源：http://m.share.hesvh.cn/Article/details/gqlgnbfxs.sHtML

------------------------------------
来源：http://wap.fehbvm.com/Article/details/gurvobfhk.sHtML

合计                                  2106 条
来源：http://blog.zdbjq.cn/Article/details/gafdcdmka.sHtML

--------------------------------------------------------------------------------
来源：http://baike.zdbjq.cn/Article/details/geiscjvrz.sHtML

使用提醒
来源：http://3g.zdbjq.cn/Article/details/gpiwymaup.sHtML

--------------------------------------------------------------------------------
来源：http://baike.hesvh.cn/Article/details/gfpomosct.sHtML

1. 示例追求"最小可用"，正式项目中请补齐导入、错误处理与边界判断。
来源：http://www.blog.hesvh.cn/Article/details/gdjbwuzwi.sHtML

2. 涉及文件、网络、数据库的示例，注意资源释放与异常捕获。
来源：http://3g.fehbvm.com/Article/details/gouggtmdi.sHtML

3. 语言版本差异较大（如 Python 3.10 的 match、Java 17 的 record/switch 箭头），
来源：http://blog.fehbvm.com/Article/details/gjiprcxzo.sHtML

在旧版本上使用前请先确认语法支持情况。
来源：http://baike.fehbvm.com/Article/details/gauzqyqmc.sHtML

4. 标注"手写"的条目是因为该语言缺少对应内置能力，实际项目中可引入成熟库。
来源：http://wap.hesvh.cn/Article/details/gewauxkhd.sHtML

—— 文件结束 ——
来源：http://wap.fehbvm.com/Article/details/gdhemrhqf.sHtML

================================================================================
来源：http://wap.fehbvm.com/Article/details/gfpsgczhy.sHtML

程序语言常见例子速查手册（2024 版）
来源：http://www.share.zdbjq.cn/Article/details/gokmibkcl.sHtML

Common Programming Examples Cheat Book
来源：http://read.share.hesvh.cn/Article/details/gtcujwxru.sHtML

================================================================================
来源：http://3g.zdbjq.cn/Article/details/gfqrfcxtm.sHtML

【收录内容】
来源：http://mobile.hesvh.cn/Article/details/grmrlcvxk.sHtML

覆盖 12 种语言 / 语法与常见 API：
来源：http://m.share.hesvh.cn/Article/details/gwesolekk.sHtML

Python · PHP · JavaScript · TypeScript · Java · Go · Ruby · C#
来源：http://blog.hesvh.cn/Article/details/gugclamjg.sHtML

SQL · Bash · C · C++
来源：http://mobile.zdbjq.cn/Article/details/ghwdjulyf.sHtML

按「任务」分组：每个任务下按语言各给出一条最小可用示例。
来源：http://www.blog.fehbvm.com/Article/details/gvdybjxlf.sHtML

【使用说明】
来源：http://www.blog.hesvh.cn/Article/details/gygfmuzma.sHtML

1. 每个任务形如 "[编号] 任务名"，下面每行以语言标记开头：
来源：http://read.share.zdbjq.cn/Article/details/gluieeohn.sHtML

Py:    Python        PHP:   PHP           JS:    JavaScript
来源：http://www.share.zdbjq.cn/Article/details/gbvztrwfs.sHtML

TS:    TypeScript    Java:  Java          Go:    Go
来源：http://www.blog.hesvh.cn/Article/details/gtenxzsxu.sHtML

Ruby:  Ruby          C#:    C#            SQL:   SQL
来源：http://baike.zdbjq.cn/Article/details/gharqbfqi.sHtML

Bash:  Shell         C:     C             C++:   C++
来源：http://3g.hesvh.cn/Article/details/gisgxdqym.sHtML

2. 示例只展示核心写法，刻意省略 import / require / include / using 等样板代码。
来源：http://3g.zdbjq.cn/Article/details/gbghnsqgj.sHtML

需要完整可运行文件时，请自行补齐当前语言的导入语句。
来源：http://mobile.hesvh.cn/Article/details/geackzpuz.sHtML

3. 语法基准：Python 3.10+ / PHP 8.1+ / ES2020+ / TypeScript 5 / Java 17 /
来源：http://www.share.zdbjq.cn/Article/details/gidjjqwtk.sHtML

Go 1.21+ / Ruby 3.x / C# 10+ / C17 / C++17。
来源：http://blog.fehbvm.com/Article/details/gqkkgkbnx.sHtML

4. 检索建议：用编辑器或浏览器 Ctrl+F 搜关键词，如 "排序" "读取文件" "正则"。
来源：http://www.blog.fehbvm.com/Article/details/gkglirtyk.sHtML

5. 标记为 "// 无" 表示该语言没有对应的一等语法，需用替代写法（示例给出替代方案）。
来源：http://www.share.fehbvm.com/Article/details/gpkjrarrf.sHtML

6. 符号 "⏎" 表示代码在此处换行（主要用于 Python 等强制缩进、无法压成一行的结构）。
来源：http://read.share.zdbjq.cn/Article/details/ghzxpzycy.sHtML

【文件统计】
来源：http://baike.zdbjq.cn/Article/details/gajioflqx.sHtML

语言示例共 2106 条，分布见本文末尾的「统计汇总」。
来源：http://baike.fehbvm.com/Article/details/grbuozlee.sHtML

--------------------------------------------------------------------------------
来源：http://www.blog.zdbjq.cn/Article/details/ginsufxvy.sHtML

目  录
来源：http://baike.zdbjq.cn/Article/details/gaskcqgkl.sHtML

--------------------------------------------------------------------------------
来源：http://wap.fehbvm.com/Article/details/gebivsvxg.sHtML

A. 基础语法与类型              （第 1 节，26 个任务，208 条）
来源：http://www.blog.fehbvm.com/Article/details/glhkoznqg.sHtML

B. 流程控制                    （第 2 节，16 个任务，128 条）
来源：http://3g.fehbvm.com/Article/details/gjzzmfxzy.sHtML

C. 函数与作用域                （第 3 节，16 个任务，128 条）
来源：http://wap.hesvh.cn/Article/details/gusoeedfu.sHtML

D. 数组 / 列表 / 集合          （第 4 节，26 个任务，208 条）
来源：http://3g.zdbjq.cn/Article/details/gvvibkxqn.sHtML

E. 字符串处理                  （第 5 节，22 个任务，176 条）
来源：http://www.m.share.zdbjq.cn/Article/details/glcadlwmc.sHtML

F. 文件与目录                  （第 6 节，12 个任务，96 条）
来源：http://baike.fehbvm.com/Article/details/gadejomkb.sHtML

G. 面向对象                    （第 7 节，16 个任务，128 条）
来源：http://3g.fehbvm.com/Article/details/gplxneubx.sHtML

H. 异常与错误处理              （第 8 节，10 个任务，80 条）
来源：http://mobile.hesvh.cn/Article/details/gvxnrbydc.sHtML

I. 正则表达式                  （第 9 节，8 个任务，64 条）
来源：http://wap.hesvh.cn/Article/details/gfszhdxhf.sHtML

J. 日期与时间                  （第 10 节，10 个任务，80 条）
来源：http://www.m.share.fehbvm.com/Article/details/glgpdkuah.sHtML

K. JSON 与序列化               （第 11 节，8 个任务，64 条）
来源：http://baike.hesvh.cn/Article/details/gzaadpjaj.sHtML

L. 网络请求                    （第 12 节，8 个任务，64 条）
来源：http://www.blog.hesvh.cn/Article/details/gyqwgriis.sHtML

M. 命令行 / 进程 / 环境        （第 13 节，8 个任务，64 条）
来源：http://www.m.share.fehbvm.com/Article/details/gsvakbfgw.sHtML

N. 数据结构与算法              （第 14 节，12 个任务，96 条）
来源：http://www.share.zdbjq.cn/Article/details/gwtyafizj.sHtML

O. 并发与异步                  （第 15 节，6 个任务，48 条）
来源：http://www.blog.zdbjq.cn/Article/details/gvlpfxdsr.sHtML

P. 常用工具函数                （第 16 节，8 个任务，64 条）
来源：http://www.share.fehbvm.com/Article/details/gupsbtqmy.sHtML

Q. SQL 专题                    （第 17 节，90 条）
来源：http://www.blog.zdbjq.cn/Article/details/gnjfldarp.sHtML


<!-- 参考信息 -->