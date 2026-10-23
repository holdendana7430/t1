代发 wailian999

[U21] Py：自定义上下文管理器
来源：http://www.ydjk.org.cn/Article/details/gt3abynfcnl.html

@contextlib.contextmanager
来源：http://www.ydjk.org.cn/Article/details/gt3ythtwxse.html

[U22] Py：矩阵转置
来源：http://www.ydjk.org.cn/Article/details/gt3siihnrcv.html

list(zip(*m))
来源：http://www.ydjk.org.cn/Article/details/gt3mqfdguyi.html

[U23] Py：分块读取大文件
来源：http://www.ydjk.org.cn/Article/details/gt3sxyedxyn.html

for chunk in iter(lambda: f.read(8192), b""):
来源：http://www.52xcode.cn/Article/details/gt3kfwrujob.html

[U24] Py：路径操作
来源：http://www.52xcode.cn/Article/details/gt3fttpzhwu.html

Path("a/b.txt").parent.mkdir(parents=True, exist_ok=True)
来源：http://www.52xcode.cn/Article/details/gt3mpblmcqp.html

[U25] Py：CSV 按字典读
来源：http://www.52xcode.cn/Article/details/gt3rzntdrev.html

csv.DictReader(f)
来源：http://www.52xcode.cn/Article/details/gt3tzmbktto.html

[U26] Py：并发下载
来源：http://www.52xcode.cn/Article/details/gt3fawltyol.html

ThreadPoolExecutor(max_workers=8).map(fetch, urls)
来源：http://www.ydjk.org.cn/Article/details/gt3xmnkbunc.html

[U27] Py：异步 HTTP
来源：http://www.ydjk.org.cn/Article/details/gt3wnmfjfzp.html

aiohttp.ClientSession() 配合 async with
来源：http://www.52xcode.cn/Article/details/gt3vauofgsz.html

[U28] Py：类型别名
来源：http://www.52xcode.cn/Article/details/gt3xaxmxvxm.html

UserId = int
来源：http://www.52xcode.cn/Article/details/gt3bqojplzh.html

[U29] Py：属性校验
来源：http://www.52xcode.cn/Article/details/gt3kygfwpjp.html

@property 与 @x.setter 配合
来源：http://www.ydjk.org.cn/Article/details/gt3evvtfixz.html

[U30] Py：数据类
来源：http://www.52xcode.cn/Article/details/gt3ybbgvymx.html

@dataclass(slots=True)
来源：http://www.ydjk.org.cn/Article/details/gt3rvaovbgn.html

[U31] Py：单测
来源：http://www.52xcode.cn/Article/details/gt3uqsksjrh.html

python -m pytest -q
来源：http://www.ydjk.org.cn/Article/details/gt3uencmdmf.html

[U32] Py：代码格式化
来源：http://www.52xcode.cn/Article/details/gt3dtxcwewf.html

ruff format . && ruff check --fix .
来源：http://www.ydjk.org.cn/Article/details/gt3lmbflktw.html

[U33] Py：打包发布
来源：http://www.ydjk.org.cn/Article/details/gt3lvgpejmk.html

python -m build  （依赖 pyproject.toml）
来源：http://www.52xcode.cn/Article/details/gt3hvyrykny.html

[U34] Py：判断编码
来源：http://www.52xcode.cn/Article/details/gt3sdikixcd.html

chardet.detect(raw)
来源：http://www.52xcode.cn/Article/details/gt3aliqkqhs.html

[U35] Py：发送邮件
来源：http://www.52xcode.cn/Article/details/gt3bhcylscf.html

smtplib.SMTP_SSL(...).send_message(msg)
来源：http://www.52xcode.cn/Article/details/gt3mqwbzhhl.html

[U36] Py：定时任务
来源：http://www.ydjk.org.cn/Article/details/gt3cnkhnrdl.html

schedule.every(10).minutes.do(job)
来源：http://www.ydjk.org.cn/Article/details/gt3koggrqxy.html

[U37] Py：读写 Excel
来源：http://www.52xcode.cn/Article/details/gt3lhncabgk.html

pandas.read_excel / DataFrame.to_excel
来源：http://www.ydjk.org.cn/Article/details/gt3gxnulfnb.html

[U38] Py：获取脚本所在目录
来源：http://www.ydjk.org.cn/Article/details/gt3alcnlgvy.html

Path(__file__).resolve().parent
来源：http://www.52xcode.cn/Article/details/gt3bkeyorgs.html

[U39] Py：判断是否在交互环境
来源：http://www.52xcode.cn/Article/details/gt3gggqvntg.html

sys.stdout.isatty()
来源：http://www.ydjk.org.cn/Article/details/gt3neijawvs.html

[U40] Py：打印到标准错误
来源：http://www.52xcode.cn/Article/details/gt3ayfuueft.html

print("err", file=sys.stderr)
来源：http://www.52xcode.cn/Article/details/gt3zhflwfyl.html

[U41] PHP：初始化 Composer 项目
来源：http://www.ydjk.org.cn/Article/details/gt3dbjkaznk.html

composer init;  composer require guzzlehttp/guzzle
来源：http://www.ydjk.org.cn/Article/details/gt3pvrtdnmv.html

[U42] PHP：PSR-4 自动加载
来源：http://www.52xcode.cn/Article/details/gt3ipnpkrdz.html

"autoload": { "psr-4": { "App\\": "src/" } }
来源：http://www.ydjk.org.cn/Article/details/gt3gqpdoeen.html

[U43] PHP：声明命名空间
来源：http://www.ydjk.org.cn/Article/details/gt3ihuxojeh.html

namespace App\Http;
来源：http://www.52xcode.cn/Article/details/gt3olusfvri.html

[U44] PHP：开启严格类型
来源：http://www.ydjk.org.cn/Article/details/gt3yshdzacq.html

declare(strict_types=1);
来源：http://www.52xcode.cn/Article/details/gt3awfztfxx.html

[U45] PHP：类型声明与返回类型
来源：http://www.52xcode.cn/Article/details/gt3xwhgtknc.html

function add(int $a, int $b): int { return $a + $b; }
来源：http://www.52xcode.cn/Article/details/gt3ezsvbfpd.html

[U46] PHP：可空类型
来源：http://www.ydjk.org.cn/Article/details/gt3gsytzcpq.html

?string $name = null
来源：http://www.ydjk.org.cn/Article/details/gt3qyazsufq.html

[U47] PHP：联合类型
来源：http://www.ydjk.org.cn/Article/details/gt3juputlqq.html

int|string $id
来源：http://www.52xcode.cn/Article/details/gt3zjyaamge.html

[U48] PHP：纯枚举
来源：http://www.ydjk.org.cn/Article/details/gt3yhnnazcf.html

enum Status: string { case Active = "active"; case Off = "off"; }
来源：http://www.ydjk.org.cn/Article/details/gt3jgwlxcop.html

[U49] PHP：只读属性
来源：http://www.ydjk.org.cn/Article/details/gt3rnvuexss.html

public readonly string $name
来源：http://www.52xcode.cn/Article/details/gt3osbezkvd.html

[U50] PHP：构造器属性提升
来源：http://www.ydjk.org.cn/Article/details/gt3gccqseki.html

public function __construct(private int $id) {}
来源：http://www.ydjk.org.cn/Article/details/gt3dimtskpq.html

[U51] PHP：数组解构
来源：http://www.ydjk.org.cn/Article/details/gt3ymejslvz.html

[$a, $b] = $arr;
来源：http://www.52xcode.cn/Article/details/gt3azjvdkba.html

[U52] PHP：箭头函数
来源：http://www.ydjk.org.cn/Article/details/gt3wnrzzvwm.html

$double = fn($x) => $x * 2;
来源：http://www.52xcode.cn/Article/details/gt3mqfqdmih.html

[U53] PHP：空合并运算符
来源：http://www.ydjk.org.cn/Article/details/gt3yfwlstvz.html

$v = $a ?? $b ?? "default";
来源：http://www.ydjk.org.cn/Article/details/gt3phkyiiyt.html

[U54] PHP：空安全调用
来源：http://www.52xcode.cn/Article/details/gt3xgzkcgxf.html

$obj?->method()
来源：http://www.52xcode.cn/Article/details/gt3flzijzpk.html

[U55] PHP：match 表达式
来源：http://www.ydjk.org.cn/Article/details/gt3aetjczxv.html

$s = match($x) { 1 => "一", default => "其他" };
来源：http://www.52xcode.cn/Article/details/gt3pdmlheob.html

[U56] PHP：命名参数
来源：http://www.ydjk.org.cn/Article/details/gt3qfxivgva.html

f(a: 1, b: 2)
来源：http://www.ydjk.org.cn/Article/details/gt3eniqcczp.html

[U57] PHP：字符串插值
来源：http://www.ydjk.org.cn/Article/details/gt3tcbcjsdm.html

"值: {$a}"
来源：http://www.ydjk.org.cn/Article/details/gt3uhvspymr.html

[U58] PHP：数组三件套
来源：http://www.ydjk.org.cn/Article/details/gt3xoqxvoaf.html

array_map($f, $a);  array_filter($a, $f);  array_reduce($a, $f, 0);
来源：http://www.52xcode.cn/Article/details/gt3sskjmjwp.html

[U59] PHP：自定义排序
来源：http://www.ydjk.org.cn/Article/details/gt3cgicdriy.html

usort($arr, fn($a, $b) => $a["age"] <=> $b["age"]);
来源：http://www.52xcode.cn/Article/details/gt3mupnucjl.html

[U60] PHP：JSON 编解码
来源：http://www.52xcode.cn/Article/details/gt3felxeuhw.html

json_encode($d, JSON_UNESCAPED_UNICODE);  json_decode($s, true);
来源：http://www.52xcode.cn/Article/details/gt3glitjirb.html

[U61] PHP：正则
来源：http://www.ydjk.org.cn/Article/details/gt3gnbpegge.html

preg_match('/(\d+)/', $s, $m);  preg_replace('/\d+/', '#', $s);
来源：http://www.52xcode.cn/Article/details/gt3glpyfnvo.html

[U62] PHP：日期对象
来源：http://www.ydjk.org.cn/Article/details/gt3ssambejb.html

(new DateTimeImmutable())->format("Y-m-d");
来源：http://www.ydjk.org.cn/Article/details/gt3wjgbgxmh.html

[U63] PHP：文件读写
来源：http://www.52xcode.cn/Article/details/gt3eqwjeqvt.html

file_get_contents($f);  file_put_contents($f, $data);
来源：http://www.ydjk.org.cn/Article/details/gt3umyhbcrl.html

[U64] PHP：目录遍历
来源：http://www.ydjk.org.cn/Article/details/gt3gjpgupzo.html

glob("dir/*.php");  scandir("dir");
来源：http://www.ydjk.org.cn/Article/details/gt3hzsvfyry.html

[U65] PHP：会话
来源：http://www.52xcode.cn/Article/details/gt3dknosqul.html

session_start();  $_SESSION["uid"] = 1;
来源：http://www.ydjk.org.cn/Article/details/gt3qnfofega.html

[U66] PHP：设置 Cookie
来源：http://www.52xcode.cn/Article/details/gt3wcolguma.html

setcookie("token", $v, ["httponly" => true, "samesite" => "Lax"]);
来源：http://www.52xcode.cn/Article/details/gt3uquujrrk.html

[U67] PHP：处理文件上传
来源：http://www.52xcode.cn/Article/details/gt3naizzbni.html

$_FILES["file"]["tmp_name"] 与 move_uploaded_file()
来源：http://www.ydjk.org.cn/Article/details/gt3vodiatin.html

[U68] PHP：PDO 连接
来源：http://www.ydjk.org.cn/Article/details/gt3mcdspqam.html

$pdo = new PDO("mysql:host=localhost;dbname=app", "root", "");
来源：http://www.52xcode.cn/Article/details/gt3tutxqtgp.html

[U69] PHP：PDO 预处理
来源：http://www.52xcode.cn/Article/details/gt3rayozmxs.html

$stmt = $pdo->prepare("SELECT * FROM users WHERE id = ?");  $stmt->execute([$id]);
来源：http://www.ydjk.org.cn/Article/details/gt3oedgtejb.html

[U70] PHP：PDO 事务
来源：http://www.ydjk.org.cn/Article/details/gt3domnlwdb.html

$pdo->beginTransaction();  $pdo->commit();  $pdo->rollBack();
来源：http://www.ydjk.org.cn/Article/details/gt3btkpautd.html

[U71] PHP：抛出异常
来源：http://www.52xcode.cn/Article/details/gt3reuqmfmh.html

throw new RuntimeException("失败", 500);
来源：http://www.ydjk.org.cn/Article/details/gt3mhmjhxcm.html

[U72] PHP：写错误日志
来源：http://www.ydjk.org.cn/Article/details/gt3rxzcgbra.html

error_log("失败: " . $e->getMessage());
来源：http://www.ydjk.org.cn/Article/details/gt3mogtmvlr.html

[U73] PHP：读取 ini 配置
来源：http://www.52xcode.cn/Article/details/gt3zrywgwdi.html

parse_ini_file("config.ini", true)
来源：http://www.52xcode.cn/Article/details/gt3qdbbvbag.html

[U74] PHP：读取环境变量
来源：http://www.ydjk.org.cn/Article/details/gt3hoddsoca.html

getenv("APP_ENV") ?: "production"
来源：http://www.ydjk.org.cn/Article/details/gt3zjrxacjg.html

[U75] PHP：依赖注入
来源：http://www.ydjk.org.cn/Article/details/gt3apciwiks.html

composer require psr/container
来源：http://www.52xcode.cn/Article/details/gt3chwdvcuh.html

[U76] PHP：简单路由
来源：http://www.52xcode.cn/Article/details/gt3injvivbc.html

$path = parse_url($_SERVER["REQUEST_URI"], PHP_URL_PATH);
来源：http://www.ydjk.org.cn/Article/details/gt3ivzlouwz.html

[U77] PHP：模板渲染
来源：http://www.52xcode.cn/Article/details/gt3avkmdmqc.html

composer require twig/twig
来源：http://www.52xcode.cn/Article/details/gt3onoedhhw.html

[U78] PHP：单元测试
来源：http://www.52xcode.cn/Article/details/gt3epmvscdf.html

composer require --dev phpunit/phpunit
来源：http://www.ydjk.org.cn/Article/details/gt3fanrcapu.html

[U79] PHP：静态分析
来源：http://www.ydjk.org.cn/Article/details/gt3pderdcxc.html

composer require --dev phpstan/phpstan
来源：http://www.ydjk.org.cn/Article/details/gt3tznnjxzi.html

[U80] PHP：代码规范修复
来源：http://www.52xcode.cn/Article/details/gt3tbnqqydc.html

composer require --dev friendsofphp/php-cs-fixer
来源：http://www.ydjk.org.cn/Article/details/gt3zfumtzel.html

[U81] JS：初始化项目
来源：http://www.52xcode.cn/Article/details/gt3ifansauc.html

npm init -y;  npm i express
来源：http://www.ydjk.org.cn/Article/details/gt3eenfohqx.html

[U82] JS：package.json 脚本
来源：http://www.52xcode.cn/Article/details/gt3seolbebs.html

"scripts": { "dev": "vite", "build": "vite build" }
来源：http://www.52xcode.cn/Article/details/gt3vnmxefws.html

[U83] JS：ES Module 导入导出
来源：http://www.ydjk.org.cn/Article/details/gt3vrbuneyi.html

export const a = 1;  import { a } from "./m.js";
来源：http://www.52xcode.cn/Article/details/gt3yivlkxwv.html

[U84] JS：CommonJS 写法
来源：http://www.52xcode.cn/Article/details/gt3ikwdczbu.html

module.exports = { a };  const { a } = require("./m");
来源：http://www.52xcode.cn/Article/details/gt3pfzbnkdc.html

[U85] JS：可选链
来源：http://www.ydjk.org.cn/Article/details/gt3yycawkci.html

a?.b?.c
来源：http://www.ydjk.org.cn/Article/details/gt3tiktijnd.html

[U86] JS：空值合并
来源：http://www.52xcode.cn/Article/details/gt3qvsclneg.html

a ?? b
来源：http://www.52xcode.cn/Article/details/gt3pvuaupal.html

[U87] JS：解构默认值
来源：http://www.ydjk.org.cn/Article/details/gt3euegqfvl.html

const { a = 1, b = 2 } = obj;
来源：http://www.ydjk.org.cn/Article/details/gt3xntucnac.html

[U88] JS：对象展开合并
来源：http://www.ydjk.org.cn/Article/details/gt3hhvdpcwd.html

{ ...a, ...b }
来源：http://www.52xcode.cn/Article/details/gt3fiabflix.html

[U89] JS：数组去重
来源：http://www.52xcode.cn/Article/details/gt3qmwjxrxm.html

[...new Set(arr)]
来源：http://www.ydjk.org.cn/Article/details/gt3uzwanzxn.html

[U90] JS：数字数组排序
来源：http://www.52xcode.cn/Article/details/gt3xkpooedx.html

[...arr].sort((a, b) => a - b)
来源：http://www.52xcode.cn/Article/details/gt3xburvkfk.html

[U91] JS：对象键值遍历
来源：http://www.52xcode.cn/Article/details/gt3gjzfhzcg.html

Object.entries(obj).forEach(([k, v]) => {});
来源：http://www.ydjk.org.cn/Article/details/gt3mcpkmbdw.html

[U92] JS：深拷贝
来源：http://www.52xcode.cn/Article/details/gt3tdsyijxc.html

structuredClone(obj)
来源：http://www.ydjk.org.cn/Article/details/gt3ieqbbmuo.html

[U93] JS：模板字符串
来源：http://www.ydjk.org.cn/Article/details/gt3foueunsf.html

`共 ${n} 条`
来源：http://www.52xcode.cn/Article/details/gt3wwttxrxa.html

[U94] JS：箭头函数
来源：http://www.ydjk.org.cn/Article/details/gt3jjmrewwz.html

const double = x => x * 2;
来源：http://www.ydjk.org.cn/Article/details/gt3liokumfm.html

[U95] JS：Promise 包装
来源：http://www.ydjk.org.cn/Article/details/gt3zetkqsuu.html

new Promise((resolve, reject) => {})
来源：http://www.52xcode.cn/Article/details/gt3vtgrogtr.html

[U96] JS：async/await 与异常
来源：http://www.52xcode.cn/Article/details/gt3xwivpsxf.html

try { const d = await f(); } catch (e) { console.error(e); }
来源：http://www.52xcode.cn/Article/details/gt3jcejxjgq.html

[U97] JS：并发请求
来源：http://www.52xcode.cn/Article/details/gt3nnqngefc.html

await Promise.all(urls.map(u => fetch(u)))
来源：http://www.52xcode.cn/Article/details/gt3pknfiute.html

[U98] JS：fetch 带 JSON
来源：http://www.ydjk.org.cn/Article/details/gt3jynnikht.html

await fetch(url, { method: "POST", headers: { "Content-Type": "application/json" }, body: JSON.stringify(d) })
来源：http://www.ydjk.org.cn/Article/details/gt3jrukuspg.html

[U99] JS：事件监听
来源：http://www.52xcode.cn/Article/details/gt3ywuosxog.html

el.addEventListener("click", e => {})
来源：http://www.ydjk.org.cn/Article/details/gt3pijjaijg.html

[U100] JS：DOM 查询
来源：http://www.52xcode.cn/Article/details/gt3olcshzwr.html

document.querySelector(".item")
来源：http://www.ydjk.org.cn/Article/details/gt3sagfixbx.html

[U101] JS：classList 操作
来源：http://www.52xcode.cn/Article/details/gt3rejyisem.html

el.classList.toggle("active")
来源：http://www.ydjk.org.cn/Article/details/gt3pfocuxci.html

[U102] JS：本地存储
来源：http://www.ydjk.org.cn/Article/details/gt3vlsrxlrh.html

localStorage.setItem("k", JSON.stringify(v))
来源：http://www.52xcode.cn/Article/details/gt3jzscbpty.html

[U103] JS：定时器
来源：http://www.52xcode.cn/Article/details/gt3emfbjyvr.html

setTimeout(fn, 1000);  setInterval(fn, 1000);
来源：http://www.ydjk.org.cn/Article/details/gt3atkqxzir.html

[U104] JS：防抖
来源：http://www.52xcode.cn/Article/details/gt3hzcalapa.html

const debounce = (fn, ms) => { let t; return (...a) => { clearTimeout(t); t = setTimeout(() => fn(...a), ms); }; };
来源：http://www.52xcode.cn/Article/details/gt3cwxcgcgc.html

[U105] JS：节流
来源：http://www.52xcode.cn/Article/details/gt3eyqezthv.html

const throttle = (fn, ms) => { let last = 0; return (...a) => { const n = Date.now(); if (n - last >= ms) { last = n; fn(...a); } }; };
来源：http://www.52xcode.cn/Article/details/gt3duxegorw.html

[U106] JS：日期格式化
来源：http://www.52xcode.cn/Article/details/gt3ktrbfbjf.html

new Intl.DateTimeFormat("zh-CN", { dateStyle: "medium" }).format(new Date())
来源：http://www.ydjk.org.cn/Article/details/gt3ogysagwv.html

[U107] JS：数字千分位
来源：http://www.ydjk.org.cn/Article/details/gt3ujhrehjt.html

new Intl.NumberFormat("en-US").format(1234567)
来源：http://www.52xcode.cn/Article/details/gt3wfkruzyo.html

[U108] JS：随机整数
来源：http://www.ydjk.org.cn/Article/details/gt3fewjylmq.html

Math.floor(Math.random() * (max - min + 1)) + min
来源：http://www.52xcode.cn/Article/details/gt3cqdsflax.html

[U109] JS：数组分组
来源：http://www.52xcode.cn/Article/details/gt3mnncxnmu.html

Object.groupBy(arr, x => x.type)
来源：http://www.52xcode.cn/Article/details/gt3ropmnukl.html

[U110] JS：数组分块
来源：http://www.52xcode.cn/Article/details/gt3bxcxmola.html

arr.reduce((acc, x, i) => (i % size ? acc : [...acc, arr.slice(i, i + size)]), [])
来源：http://www.ydjk.org.cn/Article/details/gt3agaioolj.html

[U111] JS：对象转 Map
来源：http://www.ydjk.org.cn/Article/details/gt3spkxyykp.html

new Map(Object.entries(obj))
来源：http://www.52xcode.cn/Article/details/gt3ssciwonx.html

[U112] JS：字符串补位
来源：http://www.52xcode.cn/Article/details/gt3ulbhckzw.html

"7".padStart(3, "0")
来源：http://www.52xcode.cn/Article/details/gt3beztmgmm.html

[U113] JS：正则替换全部
来源：http://www.ydjk.org.cn/Article/details/gt3mxgpohfc.html

s.replaceAll("a", "b")
来源：http://www.ydjk.org.cn/Article/details/gt3wkazlhnk.html

[U114] JS：JSON 深比较
来源：http://www.52xcode.cn/Article/details/gt3ouxjhxqd.html

JSON.stringify(a) === JSON.stringify(b)
来源：http://www.ydjk.org.cn/Article/details/gt3pdcpzwrv.html

[U115] JS：生成 UUID
来源：http://www.ydjk.org.cn/Article/details/gt3nadwbevs.html

crypto.randomUUID()
来源：http://www.ydjk.org.cn/Article/details/gt3kprsuowm.html

[U116] JS：类型检查（JSDoc）
来源：http://www.52xcode.cn/Article/details/gt3vuoivxex.html

/** @param {string} name */ function f(name) {}
来源：http://www.52xcode.cn/Article/details/gt3sdcsmpfg.html

[U117] JS：单元测试
来源：http://www.52xcode.cn/Article/details/gt3ezmvaywi.html

npm i -D vitest;  npx vitest
来源：http://www.52xcode.cn/Article/details/gt3urlnjfxn.html

[U118] JS：开发服务器
来源：http://www.52xcode.cn/Article/details/gt3kyuvveyh.html

npm i -D vite;  npx vite
来源：http://www.52xcode.cn/Article/details/gt3ngvsqdgs.html

[U119] JS：生产构建
来源：http://www.52xcode.cn/Article/details/gt3golcbgek.html

npx vite build
来源：http://www.ydjk.org.cn/Article/details/gt3lnputkmi.html

[U120] JS：读取环境变量（Vite）
来源：http://www.ydjk.org.cn/Article/details/gt3opoxzrjp.html

import.meta.env.VITE_API_URL
来源：http://www.52xcode.cn/Article/details/gt3obvfwsph.html

================================================================================
来源：http://www.52xcode.cn/Article/details/gt3ydwqewsy.html

统计汇总
来源：http://www.ydjk.org.cn/Article/details/gt3ppuzgzgf.html

================================================================================
来源：http://www.52xcode.cn/Article/details/gt3xpbojthy.html

按语言统计（条）：
来源：http://www.ydjk.org.cn/Article/details/gt3pewmqcgr.html

Python ......... 252
来源：http://www.52xcode.cn/Article/details/gt3dkrxocsw.html

PHP ............ 252
来源：http://www.ydjk.org.cn/Article/details/gt3wrlezpqc.html

JavaScript ..... 252
来源：http://www.52xcode.cn/Article/details/gt3rwbpgtiy.html

TypeScript ..... 212
来源：http://www.ydjk.org.cn/Article/details/gt3riyjgjuu.html

Java ........... 212
来源：http://www.ydjk.org.cn/Article/details/gt3cesjzpkf.html

Go ............. 212
来源：http://www.52xcode.cn/Article/details/gt3cjkpeagc.html

Ruby ........... 212
来源：http://www.52xcode.cn/Article/details/gt3lcwuifmo.html

C# ............. 212
来源：http://www.52xcode.cn/Article/details/gt3fvseksvg.html

C .............. 30
来源：http://www.ydjk.org.cn/Article/details/gt3wzwfmesj.html

C++ ............ 30
来源：http://www.ydjk.org.cn/Article/details/gt3aakfbddg.html

SQL ............ 90
来源：http://www.52xcode.cn/Article/details/gt3pwoczmwl.html

Bash ........... 80
来源：http://www.ydjk.org.cn/Article/details/gt3xfbdxqdy.html

Kotlin ......... 15
来源：http://www.ydjk.org.cn/Article/details/gt3ttwgtewp.html

Swift .......... 15
来源：http://www.ydjk.org.cn/Article/details/gt3imexuvwg.html

Lua ............ 10
来源：http://www.52xcode.cn/Article/details/gt3aolfrhtr.html

Perl ........... 10
来源：http://www.52xcode.cn/Article/details/gt3ntdrnjmm.html

Scala .......... 10
来源：http://www.ydjk.org.cn/Article/details/gt3gsfeftla.html

------------------------------------
来源：http://www.52xcode.cn/Article/details/gt3oiajvhuv.html

合计 ........... 2106 条
来源：http://www.52xcode.cn/Article/details/gt3kiamertk.html

按章节统计：
来源：http://www.52xcode.cn/Article/details/gt3gjzsihom.html

A 基础语法与类型       26 个任务 × 8 语言 =  208
来源：http://www.ydjk.org.cn/Article/details/gt3yzvdkedq.html

B 流程控制             16 个任务 × 8 语言 =  128
来源：http://www.52xcode.cn/Article/details/gt3qscalugg.html

C 函数与作用域         16 个任务 × 8 语言 =  128
来源：http://www.ydjk.org.cn/Article/details/gt3cofbxzsz.html

D 数组 / 列表 / 集合   26 个任务 × 8 语言 =  208
来源：http://www.ydjk.org.cn/Article/details/gt3ffjcntiq.html

E 字符串处理           22 个任务 × 8 语言 =  176
来源：http://www.52xcode.cn/Article/details/gt3omnvyaiw.html

F 文件与目录           12 个任务 × 8 语言 =   96
来源：http://www.ydjk.org.cn/Article/details/gt3hfbyhifg.html

G 面向对象             16 个任务 × 8 语言 =  128
来源：http://www.ydjk.org.cn/Article/details/gt3jojaaagt.html

H 异常与错误处理       10 个任务 × 8 语言 =   80
来源：http://www.ydjk.org.cn/Article/details/gt3vctqigjb.html

I 正则表达式            8 个任务 × 8 语言 =   64
来源：http://www.ydjk.org.cn/Article/details/gt3zvrdcxbm.html

J 日期与时间           10 个任务 × 8 语言 =   80
来源：http://www.52xcode.cn/Article/details/gt3drhnzyqq.html

K JSON 与序列化         8 个任务 × 8 语言 =   64
来源：http://www.ydjk.org.cn/Article/details/gt3srmixwnz.html

L 网络请求              8 个任务 × 8 语言 =   64
来源：http://www.52xcode.cn/Article/details/gt3unndyhhi.html

M 命令行 / 进程         8 个任务 × 8 语言 =   64
来源：http://www.ydjk.org.cn/Article/details/gt3swnxoeyo.html

N 数据结构与算法       12 个任务 × 8 语言 =   96
来源：http://www.ydjk.org.cn/Article/details/gt3kwaatfnq.html

O 并发与异步            6 个任务 × 8 语言 =   48
来源：http://www.52xcode.cn/Article/details/gt3igxdneuk.html

P 常用工具函数          8 个任务 × 8 语言 =   64
来源：http://www.ydjk.org.cn/Article/details/gt3izquwhwi.html

Q SQL 专题                              90
来源：http://www.ydjk.org.cn/Article/details/gt3sgcdebzp.html

R Bash 专题                             80
来源：http://www.ydjk.org.cn/Article/details/gt3bmqqencb.html

S C / C++ 专题                          60
来源：http://www.ydjk.org.cn/Article/details/gt3vsicwevo.html

T 其他语言补充                          60
来源：http://www.52xcode.cn/Article/details/gt3pixnvoox.html

U 高频实用片段                         120
来源：http://www.52xcode.cn/Article/details/gt3jlohumew.html

------------------------------------
来源：http://www.52xcode.cn/Article/details/gt3ycweqjjv.html

合计                                  2106 条
来源：http://www.ydjk.org.cn/Article/details/gt3zaewkurz.html

--------------------------------------------------------------------------------
来源：http://www.52xcode.cn/Article/details/gt3dmkzknde.html

使用提醒
来源：http://www.52xcode.cn/Article/details/gt3cdfcbuwh.html

--------------------------------------------------------------------------------
来源：http://www.52xcode.cn/Article/details/gt3tsubvuss.html

1. 示例追求"最小可用"，正式项目中请补齐导入、错误处理与边界判断。
来源：http://www.ydjk.org.cn/Article/details/gt3mpledyly.html

2. 涉及文件、网络、数据库的示例，注意资源释放与异常捕获。
来源：http://www.ydjk.org.cn/Article/details/gt3sgmkibyf.html

3. 语言版本差异较大（如 Python 3.10 的 match、Java 17 的 record/switch 箭头），
来源：http://www.ydjk.org.cn/Article/details/gt3txwjjzrw.html

在旧版本上使用前请先确认语法支持情况。
来源：http://www.ydjk.org.cn/Article/details/gt3jrevjlbp.html

4. 标注"手写"的条目是因为该语言缺少对应内置能力，实际项目中可引入成熟库。
来源：http://www.52xcode.cn/Article/details/gt3wqnkwofi.html

—— 文件结束 ——
来源：http://www.52xcode.cn/Article/details/gt3yopqgfhn.html

================================================================================
来源：http://www.ydjk.org.cn/Article/details/gt3txiesnur.html

程序语言常见例子速查手册（2024 版）
来源：http://www.ydjk.org.cn/Article/details/gt3qnmrqudb.html

Common Programming Examples Cheat Book
来源：http://www.ydjk.org.cn/Article/details/gt3tnedexzo.html

================================================================================
来源：http://www.ydjk.org.cn/Article/details/gt3ckpuzzhx.html

【收录内容】
来源：http://www.52xcode.cn/Article/details/gt3ytzfuclp.html

覆盖 12 种语言 / 语法与常见 API：
来源：http://www.52xcode.cn/Article/details/gt3lascjpvd.html

Python · PHP · JavaScript · TypeScript · Java · Go · Ruby · C#
来源：http://www.52xcode.cn/Article/details/gt3qajbchcy.html

SQL · Bash · C · C++
来源：http://www.52xcode.cn/Article/details/gt3zwlliikv.html

按「任务」分组：每个任务下按语言各给出一条最小可用示例。
来源：http://www.ydjk.org.cn/Article/details/gt3jeyueero.html

【使用说明】
来源：http://www.ydjk.org.cn/Article/details/gt3tuiykifj.html

1. 每个任务形如 "[编号] 任务名"，下面每行以语言标记开头：
来源：http://www.52xcode.cn/Article/details/gt3ufetnhjm.html

Py:    Python        PHP:   PHP           JS:    JavaScript
来源：http://www.ydjk.org.cn/Article/details/gt3johijxxa.html

TS:    TypeScript    Java:  Java          Go:    Go
来源：http://www.ydjk.org.cn/Article/details/gt3kwjixyqx.html

Ruby:  Ruby          C#:    C#            SQL:   SQL
来源：http://www.ydjk.org.cn/Article/details/gt3mqndrnqe.html

Bash:  Shell         C:     C             C++:   C++
来源：http://www.52xcode.cn/Article/details/gt3xvdvtlke.html

2. 示例只展示核心写法，刻意省略 import / require / include / using 等样板代码。
来源：http://www.ydjk.org.cn/Article/details/gt3tcsvaltm.html

需要完整可运行文件时，请自行补齐当前语言的导入语句。
来源：http://www.52xcode.cn/Article/details/gt3norolxjv.html

3. 语法基准：Python 3.10+ / PHP 8.1+ / ES2020+ / TypeScript 5 / Java 17 /
来源：http://www.52xcode.cn/Article/details/gt3kcjokwsm.html

Go 1.21+ / Ruby 3.x / C# 10+ / C17 / C++17。
来源：http://www.52xcode.cn/Article/details/gt3zujmuqci.html

4. 检索建议：用编辑器或浏览器 Ctrl+F 搜关键词，如 "排序" "读取文件" "正则"。
来源：http://www.52xcode.cn/Article/details/gt3ewenwtgo.html

5. 标记为 "// 无" 表示该语言没有对应的一等语法，需用替代写法（示例给出替代方案）。
来源：http://www.52xcode.cn/Article/details/gt3lwrytudx.html

6. 符号 "⏎" 表示代码在此处换行（主要用于 Python 等强制缩进、无法压成一行的结构）。
来源：http://www.ydjk.org.cn/Article/details/gt3birxxlhl.html

【文件统计】
来源：http://www.ydjk.org.cn/Article/details/gt3prcdqqiz.html

语言示例共 2106 条，分布见本文末尾的「统计汇总」。
来源：http://www.52xcode.cn/Article/details/gt3hvdefghg.html

--------------------------------------------------------------------------------
来源：http://www.52xcode.cn/Article/details/gt3rotkzmzb.html

目  录
来源：http://www.ydjk.org.cn/Article/details/gt3xxnjbcik.html

--------------------------------------------------------------------------------
来源：http://www.ydjk.org.cn/Article/details/gt3aaqfhahy.html

A. 基础语法与类型              （第 1 节，26 个任务，208 条）
来源：http://www.ydjk.org.cn/Article/details/gt3rqfgcvby.html

B. 流程控制                    （第 2 节，16 个任务，128 条）
来源：http://www.ydjk.org.cn/Article/details/gt3zndxwltq.html

C. 函数与作用域                （第 3 节，16 个任务，128 条）
来源：http://www.ydjk.org.cn/Article/details/gt3wqwtjhgh.html

D. 数组 / 列表 / 集合          （第 4 节，26 个任务，208 条）
来源：http://www.ydjk.org.cn/Article/details/gt3qjsqcefy.html

E. 字符串处理                  （第 5 节，22 个任务，176 条）
来源：http://www.52xcode.cn/Article/details/gt3zpiejzlj.html

F. 文件与目录                  （第 6 节，12 个任务，96 条）
来源：http://www.52xcode.cn/Article/details/gt3hyymmuez.html

G. 面向对象                    （第 7 节，16 个任务，128 条）
来源：http://www.52xcode.cn/Article/details/gt3dffaiyrs.html

H. 异常与错误处理              （第 8 节，10 个任务，80 条）
来源：http://www.ydjk.org.cn/Article/details/gt3cjfqgdhc.html

I. 正则表达式                  （第 9 节，8 个任务，64 条）
来源：http://www.ydjk.org.cn/Article/details/gt3uiuxongq.html

J. 日期与时间                  （第 10 节，10 个任务，80 条）
来源：http://www.52xcode.cn/Article/details/gt3riizutuz.html

K. JSON 与序列化               （第 11 节，8 个任务，64 条）
来源：http://www.ydjk.org.cn/Article/details/gt3rtdjodcr.html

L. 网络请求                    （第 12 节，8 个任务，64 条）
来源：http://www.ydjk.org.cn/Article/details/gt3dkhddqeg.html

M. 命令行 / 进程 / 环境        （第 13 节，8 个任务，64 条）
来源：http://www.52xcode.cn/Article/details/gt3cljyrwfm.html

N. 数据结构与算法              （第 14 节，12 个任务，96 条）
来源：http://www.52xcode.cn/Article/details/gt3medlenew.html

O. 并发与异步                  （第 15 节，6 个任务，48 条）
来源：http://www.52xcode.cn/Article/details/gt3jtjlrrln.html

P. 常用工具函数                （第 16 节，8 个任务，64 条）
来源：http://www.52xcode.cn/Article/details/gt3abmzsaxs.html

Q. SQL 专题                    （第 17 节，90 条）
来源：http://www.52xcode.cn/Article/details/gt3xgfbpnfs.html


<!-- 参考信息 -->