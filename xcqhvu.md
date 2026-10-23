代发 wailian999

[U21] Py：自定义上下文管理器
来源：http://www.52xcode.cn/Article/details/gt3tdhjlqmt.html

@contextlib.contextmanager
来源：http://www.52xcode.cn/Article/details/gt3kdakgjfb.html

[U22] Py：矩阵转置
来源：http://www.ydjk.org.cn/Article/details/gt3iyqbizkh.html

list(zip(*m))
来源：http://www.ydjk.org.cn/Article/details/gt3jbicgwnp.html

[U23] Py：分块读取大文件
来源：http://www.ydjk.org.cn/Article/details/gt3ptwtmduh.html

for chunk in iter(lambda: f.read(8192), b""):
来源：http://www.ydjk.org.cn/Article/details/gt3cqovntnr.html

[U24] Py：路径操作
来源：http://www.52xcode.cn/Article/details/gt3sstjjkua.html

Path("a/b.txt").parent.mkdir(parents=True, exist_ok=True)
来源：http://www.52xcode.cn/Article/details/gt3rotryaxh.html

[U25] Py：CSV 按字典读
来源：http://www.ydjk.org.cn/Article/details/gt3rekqijdh.html

csv.DictReader(f)
来源：http://www.52xcode.cn/Article/details/gt3dstttgho.html

[U26] Py：并发下载
来源：http://www.ydjk.org.cn/Article/details/gt3etnmcakr.html

ThreadPoolExecutor(max_workers=8).map(fetch, urls)
来源：http://www.ydjk.org.cn/Article/details/gt3cjnykuyf.html

[U27] Py：异步 HTTP
来源：http://www.52xcode.cn/Article/details/gt3ddqezcti.html

aiohttp.ClientSession() 配合 async with
来源：http://www.ydjk.org.cn/Article/details/gt3ylugcfum.html

[U28] Py：类型别名
来源：http://www.52xcode.cn/Article/details/gt3ofgnjlks.html

UserId = int
来源：http://www.52xcode.cn/Article/details/gt3mebaucot.html

[U29] Py：属性校验
来源：http://www.52xcode.cn/Article/details/gt3nbmjqiyv.html

@property 与 @x.setter 配合
来源：http://www.ydjk.org.cn/Article/details/gt3agsgsesq.html

[U30] Py：数据类
来源：http://www.ydjk.org.cn/Article/details/gt3okzetsmg.html

@dataclass(slots=True)
来源：http://www.ydjk.org.cn/Article/details/gt3cihcnejm.html

[U31] Py：单测
来源：http://www.ydjk.org.cn/Article/details/gt3nqrphaqd.html

python -m pytest -q
来源：http://www.ydjk.org.cn/Article/details/gt3ukyxbpua.html

[U32] Py：代码格式化
来源：http://www.ydjk.org.cn/Article/details/gt3rqiabhsx.html

ruff format . && ruff check --fix .
来源：http://www.52xcode.cn/Article/details/gt3eezqngev.html

[U33] Py：打包发布
来源：http://www.52xcode.cn/Article/details/gt3uysksmvc.html

python -m build  （依赖 pyproject.toml）
来源：http://www.52xcode.cn/Article/details/gt3duxotqlk.html

[U34] Py：判断编码
来源：http://www.52xcode.cn/Article/details/gt3kptbpzey.html

chardet.detect(raw)
来源：http://www.52xcode.cn/Article/details/gt3mhwnqfgs.html

[U35] Py：发送邮件
来源：http://www.52xcode.cn/Article/details/gt3itiztkba.html

smtplib.SMTP_SSL(...).send_message(msg)
来源：http://www.52xcode.cn/Article/details/gt3ejahshhm.html

[U36] Py：定时任务
来源：http://www.52xcode.cn/Article/details/gt3wafvskbx.html

schedule.every(10).minutes.do(job)
来源：http://www.52xcode.cn/Article/details/gt3kmuwftzm.html

[U37] Py：读写 Excel
来源：http://www.52xcode.cn/Article/details/gt3ujdsgbyj.html

pandas.read_excel / DataFrame.to_excel
来源：http://www.ydjk.org.cn/Article/details/gt3mzjknall.html

[U38] Py：获取脚本所在目录
来源：http://www.52xcode.cn/Article/details/gt3cmzrocba.html

Path(__file__).resolve().parent
来源：http://www.52xcode.cn/Article/details/gt3ouwaconi.html

[U39] Py：判断是否在交互环境
来源：http://www.52xcode.cn/Article/details/gt3uxljxaze.html

sys.stdout.isatty()
来源：http://www.52xcode.cn/Article/details/gt3rcydgwjb.html

[U40] Py：打印到标准错误
来源：http://www.52xcode.cn/Article/details/gt3cxovjguv.html

print("err", file=sys.stderr)
来源：http://www.ydjk.org.cn/Article/details/gt3nvrjfolt.html

[U41] PHP：初始化 Composer 项目
来源：http://www.52xcode.cn/Article/details/gt3cefhapiw.html

composer init;  composer require guzzlehttp/guzzle
来源：http://www.52xcode.cn/Article/details/gt3wpbrixnp.html

[U42] PHP：PSR-4 自动加载
来源：http://www.52xcode.cn/Article/details/gt3qjuutogx.html

"autoload": { "psr-4": { "App\\": "src/" } }
来源：http://www.ydjk.org.cn/Article/details/gt3ohfaicdx.html

[U43] PHP：声明命名空间
来源：http://www.ydjk.org.cn/Article/details/gt3nlwwipyh.html

namespace App\Http;
来源：http://www.52xcode.cn/Article/details/gt3zwgbrbrw.html

[U44] PHP：开启严格类型
来源：http://www.52xcode.cn/Article/details/gt3ctrmroqn.html

declare(strict_types=1);
来源：http://www.52xcode.cn/Article/details/gt3awraqtgv.html

[U45] PHP：类型声明与返回类型
来源：http://www.52xcode.cn/Article/details/gt3drowyouy.html

function add(int $a, int $b): int { return $a + $b; }
来源：http://www.ydjk.org.cn/Article/details/gt3xbgjhvrv.html

[U46] PHP：可空类型
来源：http://www.52xcode.cn/Article/details/gt3mcazqxkb.html

?string $name = null
来源：http://www.ydjk.org.cn/Article/details/gt3bhmrnfel.html

[U47] PHP：联合类型
来源：http://www.52xcode.cn/Article/details/gt3qmuleryj.html

int|string $id
来源：http://www.52xcode.cn/Article/details/gt3qcxddzzp.html

[U48] PHP：纯枚举
来源：http://www.52xcode.cn/Article/details/gt3lfitdrst.html

enum Status: string { case Active = "active"; case Off = "off"; }
来源：http://www.52xcode.cn/Article/details/gt3pnvtoaga.html

[U49] PHP：只读属性
来源：http://www.52xcode.cn/Article/details/gt3utonrpie.html

public readonly string $name
来源：http://www.52xcode.cn/Article/details/gt3kjuovvcd.html

[U50] PHP：构造器属性提升
来源：http://www.ydjk.org.cn/Article/details/gt3qolulgps.html

public function __construct(private int $id) {}
来源：http://www.ydjk.org.cn/Article/details/gt3hlhducxq.html

[U51] PHP：数组解构
来源：http://www.52xcode.cn/Article/details/gt3rxftqwwn.html

[$a, $b] = $arr;
来源：http://www.52xcode.cn/Article/details/gt3kucqbdbb.html

[U52] PHP：箭头函数
来源：http://www.52xcode.cn/Article/details/gt3nozeeffs.html

$double = fn($x) => $x * 2;
来源：http://www.52xcode.cn/Article/details/gt3whnfpsqk.html

[U53] PHP：空合并运算符
来源：http://www.52xcode.cn/Article/details/gt3fiuhisxn.html

$v = $a ?? $b ?? "default";
来源：http://www.52xcode.cn/Article/details/gt3kbhpsmbu.html

[U54] PHP：空安全调用
来源：http://www.ydjk.org.cn/Article/details/gt3qvycdlqb.html

$obj?->method()
来源：http://www.ydjk.org.cn/Article/details/gt3iyhdysxq.html

[U55] PHP：match 表达式
来源：http://www.ydjk.org.cn/Article/details/gt3cdrsvqgg.html

$s = match($x) { 1 => "一", default => "其他" };
来源：http://www.52xcode.cn/Article/details/gt3dnjglgsq.html

[U56] PHP：命名参数
来源：http://www.52xcode.cn/Article/details/gt3qhsetlae.html

f(a: 1, b: 2)
来源：http://www.52xcode.cn/Article/details/gt3oqwixaof.html

[U57] PHP：字符串插值
来源：http://www.ydjk.org.cn/Article/details/gt3vjpyvifa.html

"值: {$a}"
来源：http://www.52xcode.cn/Article/details/gt3gxdswpma.html

[U58] PHP：数组三件套
来源：http://www.52xcode.cn/Article/details/gt3xqvzwujj.html

array_map($f, $a);  array_filter($a, $f);  array_reduce($a, $f, 0);
来源：http://www.ydjk.org.cn/Article/details/gt3idrjueoi.html

[U59] PHP：自定义排序
来源：http://www.52xcode.cn/Article/details/gt3serbmvhf.html

usort($arr, fn($a, $b) => $a["age"] <=> $b["age"]);
来源：http://www.ydjk.org.cn/Article/details/gt3mkzwcpvo.html

[U60] PHP：JSON 编解码
来源：http://www.52xcode.cn/Article/details/gt3cnifsrqz.html

json_encode($d, JSON_UNESCAPED_UNICODE);  json_decode($s, true);
来源：http://www.ydjk.org.cn/Article/details/gt3njqvjytg.html

[U61] PHP：正则
来源：http://www.ydjk.org.cn/Article/details/gt3fqgytgys.html

preg_match('/(\d+)/', $s, $m);  preg_replace('/\d+/', '#', $s);
来源：http://www.52xcode.cn/Article/details/gt3toujqtvk.html

[U62] PHP：日期对象
来源：http://www.52xcode.cn/Article/details/gt3rvbbmnju.html

(new DateTimeImmutable())->format("Y-m-d");
来源：http://www.ydjk.org.cn/Article/details/gt3ypqgqyib.html

[U63] PHP：文件读写
来源：http://www.ydjk.org.cn/Article/details/gt3rxykanjd.html

file_get_contents($f);  file_put_contents($f, $data);
来源：http://www.52xcode.cn/Article/details/gt3hfgpzeei.html

[U64] PHP：目录遍历
来源：http://www.52xcode.cn/Article/details/gt3vavryiba.html

glob("dir/*.php");  scandir("dir");
来源：http://www.ydjk.org.cn/Article/details/gt3ovsqztln.html

[U65] PHP：会话
来源：http://www.ydjk.org.cn/Article/details/gt3zthpehft.html

session_start();  $_SESSION["uid"] = 1;
来源：http://www.52xcode.cn/Article/details/gt3tkutpyav.html

[U66] PHP：设置 Cookie
来源：http://www.ydjk.org.cn/Article/details/gt3kjfauvzr.html

setcookie("token", $v, ["httponly" => true, "samesite" => "Lax"]);
来源：http://www.ydjk.org.cn/Article/details/gt3moncywjx.html

[U67] PHP：处理文件上传
来源：http://www.ydjk.org.cn/Article/details/gt3dssiaoud.html

$_FILES["file"]["tmp_name"] 与 move_uploaded_file()
来源：http://www.ydjk.org.cn/Article/details/gt3pnfguahf.html

[U68] PHP：PDO 连接
来源：http://www.ydjk.org.cn/Article/details/gt3zlomeoss.html

$pdo = new PDO("mysql:host=localhost;dbname=app", "root", "");
来源：http://www.ydjk.org.cn/Article/details/gt3bieoicwv.html

[U69] PHP：PDO 预处理
来源：http://www.ydjk.org.cn/Article/details/gt3xvgnwofl.html

$stmt = $pdo->prepare("SELECT * FROM users WHERE id = ?");  $stmt->execute([$id]);
来源：http://www.ydjk.org.cn/Article/details/gt3hygmxtty.html

[U70] PHP：PDO 事务
来源：http://www.ydjk.org.cn/Article/details/gt3zzbjspdg.html

$pdo->beginTransaction();  $pdo->commit();  $pdo->rollBack();
来源：http://www.52xcode.cn/Article/details/gt3ywctanbk.html

[U71] PHP：抛出异常
来源：http://www.ydjk.org.cn/Article/details/gt3hpwkvvjj.html

throw new RuntimeException("失败", 500);
来源：http://www.52xcode.cn/Article/details/gt3oovdxvme.html

[U72] PHP：写错误日志
来源：http://www.52xcode.cn/Article/details/gt3hkstbdhh.html

error_log("失败: " . $e->getMessage());
来源：http://www.ydjk.org.cn/Article/details/gt3pqyhrxpq.html

[U73] PHP：读取 ini 配置
来源：http://www.ydjk.org.cn/Article/details/gt3zhrnutva.html

parse_ini_file("config.ini", true)
来源：http://www.52xcode.cn/Article/details/gt3ypwcyjas.html

[U74] PHP：读取环境变量
来源：http://www.52xcode.cn/Article/details/gt3kpkxydnx.html

getenv("APP_ENV") ?: "production"
来源：http://www.52xcode.cn/Article/details/gt3ninorfmw.html

[U75] PHP：依赖注入
来源：http://www.52xcode.cn/Article/details/gt3hcoohtjb.html

composer require psr/container
来源：http://www.ydjk.org.cn/Article/details/gt3btveoodd.html

[U76] PHP：简单路由
来源：http://www.52xcode.cn/Article/details/gt3cvpsgaue.html

$path = parse_url($_SERVER["REQUEST_URI"], PHP_URL_PATH);
来源：http://www.52xcode.cn/Article/details/gt3hqxsfkyl.html

[U77] PHP：模板渲染
来源：http://www.ydjk.org.cn/Article/details/gt3wmoivlgs.html

composer require twig/twig
来源：http://www.52xcode.cn/Article/details/gt3baxmgwmd.html

[U78] PHP：单元测试
来源：http://www.ydjk.org.cn/Article/details/gt3pzyjyltk.html

composer require --dev phpunit/phpunit
来源：http://www.ydjk.org.cn/Article/details/gt3mndulwga.html

[U79] PHP：静态分析
来源：http://www.ydjk.org.cn/Article/details/gt3rivfwrpx.html

composer require --dev phpstan/phpstan
来源：http://www.52xcode.cn/Article/details/gt3wuqcyaoe.html

[U80] PHP：代码规范修复
来源：http://www.52xcode.cn/Article/details/gt3wizbbyjw.html

composer require --dev friendsofphp/php-cs-fixer
来源：http://www.52xcode.cn/Article/details/gt3vjtnpokv.html

[U81] JS：初始化项目
来源：http://www.52xcode.cn/Article/details/gt3nwkgcqph.html

npm init -y;  npm i express
来源：http://www.ydjk.org.cn/Article/details/gt3fdkqbqmh.html

[U82] JS：package.json 脚本
来源：http://www.52xcode.cn/Article/details/gt3zmtmtoyp.html

"scripts": { "dev": "vite", "build": "vite build" }
来源：http://www.ydjk.org.cn/Article/details/gt3kyadrtph.html

[U83] JS：ES Module 导入导出
来源：http://www.52xcode.cn/Article/details/gt3mhpmibaw.html

export const a = 1;  import { a } from "./m.js";
来源：http://www.52xcode.cn/Article/details/gt3npvhtnum.html

[U84] JS：CommonJS 写法
来源：http://www.52xcode.cn/Article/details/gt3lpvlcczv.html

module.exports = { a };  const { a } = require("./m");
来源：http://www.ydjk.org.cn/Article/details/gt3eldtdgko.html

[U85] JS：可选链
来源：http://www.52xcode.cn/Article/details/gt3grohayyh.html

a?.b?.c
来源：http://www.ydjk.org.cn/Article/details/gt3oyhylisv.html

[U86] JS：空值合并
来源：http://www.ydjk.org.cn/Article/details/gt3qjckwdeq.html

a ?? b
来源：http://www.52xcode.cn/Article/details/gt3hypvdwef.html

[U87] JS：解构默认值
来源：http://www.52xcode.cn/Article/details/gt3lbsloywt.html

const { a = 1, b = 2 } = obj;
来源：http://www.ydjk.org.cn/Article/details/gt3vpvwfwle.html

[U88] JS：对象展开合并
来源：http://www.ydjk.org.cn/Article/details/gt3kcjqbzki.html

{ ...a, ...b }
来源：http://www.52xcode.cn/Article/details/gt3hmtehukd.html

[U89] JS：数组去重
来源：http://www.ydjk.org.cn/Article/details/gt3wvfovyth.html

[...new Set(arr)]
来源：http://www.ydjk.org.cn/Article/details/gt3lluydhsq.html

[U90] JS：数字数组排序
来源：http://www.52xcode.cn/Article/details/gt3bhwafuqq.html

[...arr].sort((a, b) => a - b)
来源：http://www.ydjk.org.cn/Article/details/gt3odonwilu.html

[U91] JS：对象键值遍历
来源：http://www.ydjk.org.cn/Article/details/gt3bduhgdln.html

Object.entries(obj).forEach(([k, v]) => {});
来源：http://www.52xcode.cn/Article/details/gt3vitqdjml.html

[U92] JS：深拷贝
来源：http://www.ydjk.org.cn/Article/details/gt3zgtbnqdt.html

structuredClone(obj)
来源：http://www.ydjk.org.cn/Article/details/gt3btktujvc.html

[U93] JS：模板字符串
来源：http://www.ydjk.org.cn/Article/details/gt3liwnfhtr.html

`共 ${n} 条`
来源：http://www.ydjk.org.cn/Article/details/gt3fytgqasy.html

[U94] JS：箭头函数
来源：http://www.ydjk.org.cn/Article/details/gt3ajduidde.html

const double = x => x * 2;
来源：http://www.ydjk.org.cn/Article/details/gt3egjzrznu.html

[U95] JS：Promise 包装
来源：http://www.ydjk.org.cn/Article/details/gt3qowyazho.html

new Promise((resolve, reject) => {})
来源：http://www.ydjk.org.cn/Article/details/gt3bocwrgmc.html

[U96] JS：async/await 与异常
来源：http://www.ydjk.org.cn/Article/details/gt3tzxjbegf.html

try { const d = await f(); } catch (e) { console.error(e); }
来源：http://www.ydjk.org.cn/Article/details/gt3vnuilmwx.html

[U97] JS：并发请求
来源：http://www.52xcode.cn/Article/details/gt3fadjbdho.html

await Promise.all(urls.map(u => fetch(u)))
来源：http://www.52xcode.cn/Article/details/gt3jyopuetd.html

[U98] JS：fetch 带 JSON
来源：http://www.ydjk.org.cn/Article/details/gt3rcclgeva.html

await fetch(url, { method: "POST", headers: { "Content-Type": "application/json" }, body: JSON.stringify(d) })
来源：http://www.ydjk.org.cn/Article/details/gt3oeppwiza.html

[U99] JS：事件监听
来源：http://www.52xcode.cn/Article/details/gt3qcnilvgo.html

el.addEventListener("click", e => {})
来源：http://www.52xcode.cn/Article/details/gt3lzikkrii.html

[U100] JS：DOM 查询
来源：http://www.ydjk.org.cn/Article/details/gt3jgkthhsl.html

document.querySelector(".item")
来源：http://www.ydjk.org.cn/Article/details/gt3wbpkrvaj.html

[U101] JS：classList 操作
来源：http://www.52xcode.cn/Article/details/gt3inmozyzg.html

el.classList.toggle("active")
来源：http://www.ydjk.org.cn/Article/details/gt3vstcbtjn.html

[U102] JS：本地存储
来源：http://www.52xcode.cn/Article/details/gt3kcwgkido.html

localStorage.setItem("k", JSON.stringify(v))
来源：http://www.ydjk.org.cn/Article/details/gt3zerbscoc.html

[U103] JS：定时器
来源：http://www.ydjk.org.cn/Article/details/gt3gdrlddks.html

setTimeout(fn, 1000);  setInterval(fn, 1000);
来源：http://www.52xcode.cn/Article/details/gt3cnukgnhj.html

[U104] JS：防抖
来源：http://www.ydjk.org.cn/Article/details/gt3ksweetkm.html

const debounce = (fn, ms) => { let t; return (...a) => { clearTimeout(t); t = setTimeout(() => fn(...a), ms); }; };
来源：http://www.ydjk.org.cn/Article/details/gt3igypddmf.html

[U105] JS：节流
来源：http://www.ydjk.org.cn/Article/details/gt3pjytlmzh.html

const throttle = (fn, ms) => { let last = 0; return (...a) => { const n = Date.now(); if (n - last >= ms) { last = n; fn(...a); } }; };
来源：http://www.ydjk.org.cn/Article/details/gt3miolvvps.html

[U106] JS：日期格式化
来源：http://www.ydjk.org.cn/Article/details/gt3ofurvnoo.html

new Intl.DateTimeFormat("zh-CN", { dateStyle: "medium" }).format(new Date())
来源：http://www.ydjk.org.cn/Article/details/gt3rpcxufbp.html

[U107] JS：数字千分位
来源：http://www.ydjk.org.cn/Article/details/gt3szskcser.html

new Intl.NumberFormat("en-US").format(1234567)
来源：http://www.52xcode.cn/Article/details/gt3tzqovxjd.html

[U108] JS：随机整数
来源：http://www.ydjk.org.cn/Article/details/gt3hmxslsbm.html

Math.floor(Math.random() * (max - min + 1)) + min
来源：http://www.ydjk.org.cn/Article/details/gt3dwmhzhwv.html

[U109] JS：数组分组
来源：http://www.ydjk.org.cn/Article/details/gt3ccywoqys.html

Object.groupBy(arr, x => x.type)
来源：http://www.ydjk.org.cn/Article/details/gt3nprobuen.html

[U110] JS：数组分块
来源：http://www.ydjk.org.cn/Article/details/gt3hhhscwft.html

arr.reduce((acc, x, i) => (i % size ? acc : [...acc, arr.slice(i, i + size)]), [])
来源：http://www.ydjk.org.cn/Article/details/gt3yehhovlw.html

[U111] JS：对象转 Map
来源：http://www.52xcode.cn/Article/details/gt3fnvrtoun.html

new Map(Object.entries(obj))
来源：http://www.52xcode.cn/Article/details/gt3qmjsoxje.html

[U112] JS：字符串补位
来源：http://www.ydjk.org.cn/Article/details/gt3okdnkped.html

"7".padStart(3, "0")
来源：http://www.ydjk.org.cn/Article/details/gt3rpawjlnp.html

[U113] JS：正则替换全部
来源：http://www.52xcode.cn/Article/details/gt3wzlcrume.html

s.replaceAll("a", "b")
来源：http://www.52xcode.cn/Article/details/gt3sgbmxomj.html

[U114] JS：JSON 深比较
来源：http://www.ydjk.org.cn/Article/details/gt3ukknhgcv.html

JSON.stringify(a) === JSON.stringify(b)
来源：http://www.ydjk.org.cn/Article/details/gt3ysfscvmc.html

[U115] JS：生成 UUID
来源：http://www.ydjk.org.cn/Article/details/gt3porrmucr.html

crypto.randomUUID()
来源：http://www.ydjk.org.cn/Article/details/gt3mcvqrqvx.html

[U116] JS：类型检查（JSDoc）
来源：http://www.52xcode.cn/Article/details/gt3pcbcwwom.html

/** @param {string} name */ function f(name) {}
来源：http://www.ydjk.org.cn/Article/details/gt3mxaljxao.html

[U117] JS：单元测试
来源：http://www.52xcode.cn/Article/details/gt3nbinqnxu.html

npm i -D vitest;  npx vitest
来源：http://www.52xcode.cn/Article/details/gt3uvxfksfp.html

[U118] JS：开发服务器
来源：http://www.ydjk.org.cn/Article/details/gt3gvuoegzq.html

npm i -D vite;  npx vite
来源：http://www.52xcode.cn/Article/details/gt3rxgaalsj.html

[U119] JS：生产构建
来源：http://www.ydjk.org.cn/Article/details/gt3lamqzwfb.html

npx vite build
来源：http://www.ydjk.org.cn/Article/details/gt3cffbfyvm.html

[U120] JS：读取环境变量（Vite）
来源：http://www.52xcode.cn/Article/details/gt3xpmewway.html

import.meta.env.VITE_API_URL
来源：http://www.52xcode.cn/Article/details/gt3kyqcwktd.html

================================================================================
来源：http://www.ydjk.org.cn/Article/details/gt3ztnvfoke.html

统计汇总
来源：http://www.52xcode.cn/Article/details/gt3plhlpocm.html

================================================================================
来源：http://www.ydjk.org.cn/Article/details/gt3ptkdeemm.html

按语言统计（条）：
来源：http://www.52xcode.cn/Article/details/gt3kegmeyzn.html

Python ......... 252
来源：http://www.52xcode.cn/Article/details/gt3yfjtxobo.html

PHP ............ 252
来源：http://www.ydjk.org.cn/Article/details/gt3brswyyfr.html

JavaScript ..... 252
来源：http://www.52xcode.cn/Article/details/gt3opjbyvdd.html

TypeScript ..... 212
来源：http://www.52xcode.cn/Article/details/gt3lxjpmlup.html

Java ........... 212
来源：http://www.52xcode.cn/Article/details/gt3kvwzvbhe.html

Go ............. 212
来源：http://www.52xcode.cn/Article/details/gt3gfvpxqac.html

Ruby ........... 212
来源：http://www.52xcode.cn/Article/details/gt3jozralen.html

C# ............. 212
来源：http://www.ydjk.org.cn/Article/details/gt3zzedkewg.html

C .............. 30
来源：http://www.52xcode.cn/Article/details/gt3tfywmzqf.html

C++ ............ 30
来源：http://www.52xcode.cn/Article/details/gt3tlivghxw.html

SQL ............ 90
来源：http://www.52xcode.cn/Article/details/gt3hayoehfm.html

Bash ........... 80
来源：http://www.52xcode.cn/Article/details/gt3ptqpzzgj.html

Kotlin ......... 15
来源：http://www.ydjk.org.cn/Article/details/gt3ltyncvog.html

Swift .......... 15
来源：http://www.ydjk.org.cn/Article/details/gt3ckzojijp.html

Lua ............ 10
来源：http://www.52xcode.cn/Article/details/gt3dlfjshol.html

Perl ........... 10
来源：http://www.52xcode.cn/Article/details/gt3sjjoahiw.html

Scala .......... 10
来源：http://www.52xcode.cn/Article/details/gt3xpkwdtev.html

------------------------------------
来源：http://www.52xcode.cn/Article/details/gt3gzhttdwv.html

合计 ........... 2106 条
来源：http://www.52xcode.cn/Article/details/gt3zlsafqxg.html

按章节统计：
来源：http://www.ydjk.org.cn/Article/details/gt3yrwtlipb.html

A 基础语法与类型       26 个任务 × 8 语言 =  208
来源：http://www.52xcode.cn/Article/details/gt3yedgvmnl.html

B 流程控制             16 个任务 × 8 语言 =  128
来源：http://www.ydjk.org.cn/Article/details/gt3cjkmzbov.html

C 函数与作用域         16 个任务 × 8 语言 =  128
来源：http://www.52xcode.cn/Article/details/gt3jhpaqgin.html

D 数组 / 列表 / 集合   26 个任务 × 8 语言 =  208
来源：http://www.ydjk.org.cn/Article/details/gt3qdiqydlo.html

E 字符串处理           22 个任务 × 8 语言 =  176
来源：http://www.52xcode.cn/Article/details/gt3wjrssrha.html

F 文件与目录           12 个任务 × 8 语言 =   96
来源：http://www.52xcode.cn/Article/details/gt3gycpbxdi.html

G 面向对象             16 个任务 × 8 语言 =  128
来源：http://www.52xcode.cn/Article/details/gt3bqrphyxb.html

H 异常与错误处理       10 个任务 × 8 语言 =   80
来源：http://www.ydjk.org.cn/Article/details/gt3xvyfzijb.html

I 正则表达式            8 个任务 × 8 语言 =   64
来源：http://www.ydjk.org.cn/Article/details/gt3orbrxmhf.html

J 日期与时间           10 个任务 × 8 语言 =   80
来源：http://www.52xcode.cn/Article/details/gt3ofjrdwzp.html

K JSON 与序列化         8 个任务 × 8 语言 =   64
来源：http://www.52xcode.cn/Article/details/gt3ryeredie.html

L 网络请求              8 个任务 × 8 语言 =   64
来源：http://www.ydjk.org.cn/Article/details/gt3loayaojo.html

M 命令行 / 进程         8 个任务 × 8 语言 =   64
来源：http://www.52xcode.cn/Article/details/gt3rvjfaidk.html

N 数据结构与算法       12 个任务 × 8 语言 =   96
来源：http://www.52xcode.cn/Article/details/gt3xdnvxhag.html

O 并发与异步            6 个任务 × 8 语言 =   48
来源：http://www.ydjk.org.cn/Article/details/gt3stbnmmuh.html

P 常用工具函数          8 个任务 × 8 语言 =   64
来源：http://www.52xcode.cn/Article/details/gt3jyphrwvl.html

Q SQL 专题                              90
来源：http://www.52xcode.cn/Article/details/gt3cxviivfm.html

R Bash 专题                             80
来源：http://www.ydjk.org.cn/Article/details/gt3jnzqkzwa.html

S C / C++ 专题                          60
来源：http://www.52xcode.cn/Article/details/gt3wjvsbajq.html

T 其他语言补充                          60
来源：http://www.ydjk.org.cn/Article/details/gt3siytjfuu.html

U 高频实用片段                         120
来源：http://www.ydjk.org.cn/Article/details/gt3bnalhsew.html

------------------------------------
来源：http://www.ydjk.org.cn/Article/details/gt3qqykbnhi.html

合计                                  2106 条
来源：http://www.52xcode.cn/Article/details/gt3eelsaifi.html

--------------------------------------------------------------------------------
来源：http://www.52xcode.cn/Article/details/gt3ubafwlzv.html

使用提醒
来源：http://www.ydjk.org.cn/Article/details/gt3hhdypkgd.html

--------------------------------------------------------------------------------
来源：http://www.ydjk.org.cn/Article/details/gt3glrqbmpt.html

1. 示例追求"最小可用"，正式项目中请补齐导入、错误处理与边界判断。
来源：http://www.52xcode.cn/Article/details/gt3jsbsjzlu.html

2. 涉及文件、网络、数据库的示例，注意资源释放与异常捕获。
来源：http://www.ydjk.org.cn/Article/details/gt3fdkkaeuh.html

3. 语言版本差异较大（如 Python 3.10 的 match、Java 17 的 record/switch 箭头），
来源：http://www.52xcode.cn/Article/details/gt3lgrypdih.html

在旧版本上使用前请先确认语法支持情况。
来源：http://www.ydjk.org.cn/Article/details/gt3jongsuna.html

4. 标注"手写"的条目是因为该语言缺少对应内置能力，实际项目中可引入成熟库。
来源：http://www.ydjk.org.cn/Article/details/gt3zxvgbjeh.html

—— 文件结束 ——
来源：http://www.ydjk.org.cn/Article/details/gt3fklaxugi.html

================================================================================
来源：http://www.ydjk.org.cn/Article/details/gt3cwccyzbk.html

程序语言常见例子速查手册（2024 版）
来源：http://www.ydjk.org.cn/Article/details/gt3urcwizze.html

Common Programming Examples Cheat Book
来源：http://www.ydjk.org.cn/Article/details/gt3ojybrbkq.html

================================================================================
来源：http://www.ydjk.org.cn/Article/details/gt3ttrruhqz.html

【收录内容】
来源：http://www.52xcode.cn/Article/details/gt3mrnjzxpu.html

覆盖 12 种语言 / 语法与常见 API：
来源：http://www.52xcode.cn/Article/details/gt3tkdurpox.html

Python · PHP · JavaScript · TypeScript · Java · Go · Ruby · C#
来源：http://www.ydjk.org.cn/Article/details/gt3hrtgdejb.html

SQL · Bash · C · C++
来源：http://www.ydjk.org.cn/Article/details/gt3vxzojuui.html

按「任务」分组：每个任务下按语言各给出一条最小可用示例。
来源：http://www.52xcode.cn/Article/details/gt3ssmbugiw.html

【使用说明】
来源：http://www.52xcode.cn/Article/details/gt3gqefpizl.html

1. 每个任务形如 "[编号] 任务名"，下面每行以语言标记开头：
来源：http://www.ydjk.org.cn/Article/details/gt3vwcpuzti.html

Py:    Python        PHP:   PHP           JS:    JavaScript
来源：http://www.52xcode.cn/Article/details/gt3zjmecgep.html

TS:    TypeScript    Java:  Java          Go:    Go
来源：http://www.ydjk.org.cn/Article/details/gt3jblfozcb.html

Ruby:  Ruby          C#:    C#            SQL:   SQL
来源：http://www.ydjk.org.cn/Article/details/gt3sdqooxrq.html

Bash:  Shell         C:     C             C++:   C++
来源：http://www.ydjk.org.cn/Article/details/gt3frkenmgw.html

2. 示例只展示核心写法，刻意省略 import / require / include / using 等样板代码。
来源：http://www.ydjk.org.cn/Article/details/gt3rtwbeiun.html

需要完整可运行文件时，请自行补齐当前语言的导入语句。
来源：http://www.52xcode.cn/Article/details/gt3qkvotaef.html

3. 语法基准：Python 3.10+ / PHP 8.1+ / ES2020+ / TypeScript 5 / Java 17 /
来源：http://www.ydjk.org.cn/Article/details/gt3swfvoxep.html

Go 1.21+ / Ruby 3.x / C# 10+ / C17 / C++17。
来源：http://www.52xcode.cn/Article/details/gt3wjszeqng.html

4. 检索建议：用编辑器或浏览器 Ctrl+F 搜关键词，如 "排序" "读取文件" "正则"。
来源：http://www.ydjk.org.cn/Article/details/gt3yxvaxftj.html

5. 标记为 "// 无" 表示该语言没有对应的一等语法，需用替代写法（示例给出替代方案）。
来源：http://www.ydjk.org.cn/Article/details/gt3klmrhmbs.html

6. 符号 "⏎" 表示代码在此处换行（主要用于 Python 等强制缩进、无法压成一行的结构）。
来源：http://www.52xcode.cn/Article/details/gt3gbswhpqj.html

【文件统计】
来源：http://www.52xcode.cn/Article/details/gt3kgaqfuhm.html

语言示例共 2106 条，分布见本文末尾的「统计汇总」。
来源：http://www.52xcode.cn/Article/details/gt3fmlomuws.html

--------------------------------------------------------------------------------
来源：http://www.52xcode.cn/Article/details/gt3dypmfltv.html

目  录
来源：http://www.52xcode.cn/Article/details/gt3senvjmnz.html

--------------------------------------------------------------------------------
来源：http://www.ydjk.org.cn/Article/details/gt3yxjbiasg.html

A. 基础语法与类型              （第 1 节，26 个任务，208 条）
来源：http://www.52xcode.cn/Article/details/gt3exozohap.html

B. 流程控制                    （第 2 节，16 个任务，128 条）
来源：http://www.52xcode.cn/Article/details/gt3pygihkbe.html

C. 函数与作用域                （第 3 节，16 个任务，128 条）
来源：http://www.ydjk.org.cn/Article/details/gt3unhmfiqr.html

D. 数组 / 列表 / 集合          （第 4 节，26 个任务，208 条）
来源：http://www.ydjk.org.cn/Article/details/gt3mciekxcp.html

E. 字符串处理                  （第 5 节，22 个任务，176 条）
来源：http://www.ydjk.org.cn/Article/details/gt3cvmikouf.html

F. 文件与目录                  （第 6 节，12 个任务，96 条）
来源：http://www.52xcode.cn/Article/details/gt3kozpnkgd.html

G. 面向对象                    （第 7 节，16 个任务，128 条）
来源：http://www.ydjk.org.cn/Article/details/gt3xlyaibtz.html

H. 异常与错误处理              （第 8 节，10 个任务，80 条）
来源：http://www.ydjk.org.cn/Article/details/gt3dsspcpvd.html

I. 正则表达式                  （第 9 节，8 个任务，64 条）
来源：http://www.ydjk.org.cn/Article/details/gt3qugyghwa.html

J. 日期与时间                  （第 10 节，10 个任务，80 条）
来源：http://www.ydjk.org.cn/Article/details/gt3joqnpzca.html

K. JSON 与序列化               （第 11 节，8 个任务，64 条）
来源：http://www.52xcode.cn/Article/details/gt3janblrhs.html

L. 网络请求                    （第 12 节，8 个任务，64 条）
来源：http://www.ydjk.org.cn/Article/details/gt3radxnegm.html

M. 命令行 / 进程 / 环境        （第 13 节，8 个任务，64 条）
来源：http://www.ydjk.org.cn/Article/details/gt3bswxkgjz.html

N. 数据结构与算法              （第 14 节，12 个任务，96 条）
来源：http://www.52xcode.cn/Article/details/gt3rfobgsbc.html

O. 并发与异步                  （第 15 节，6 个任务，48 条）
来源：http://www.ydjk.org.cn/Article/details/gt3gcnywidm.html

P. 常用工具函数                （第 16 节，8 个任务，64 条）
来源：http://www.52xcode.cn/Article/details/gt3kxjzinyw.html

Q. SQL 专题                    （第 17 节，90 条）
来源：http://www.ydjk.org.cn/Article/details/gt3nkwhpbhw.html


<!-- 参考信息 -->