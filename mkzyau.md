代发 wailian999

[U17] Py：初始化日志
来源：http://www.ydjk.org.cn/Article/details/gt2hhiubxie.html

logging.basicConfig(level=logging.INFO)
来源：http://www.ydjk.org.cn/Article/details/gt2ajbfjckk.html

[U18] Py：预编译正则
来源：http://www.ydjk.org.cn/Article/details/gt2wkdteveb.html

pat = re.compile(r"\d+")
来源：http://www.ydjk.org.cn/Article/details/gt2tkrhhbdk.html

[U19] Py：正则替换带回调
来源：http://www.ydjk.org.cn/Article/details/gt2spzzqcya.html

re.sub(r"\d+", lambda m: str(int(m.group()) * 2), s)
来源：http://www.ydjk.org.cn/Article/details/gt2nsjojumm.html

[U20] Py：缓存函数结果
来源：http://www.ydjk.org.cn/Article/details/gt2btvazdpf.html

@functools.lru_cache(maxsize=None)
来源：http://www.ydjk.org.cn/Article/details/gt2khjxnzpc.html

[U21] Py：自定义上下文管理器
来源：http://www.52xcode.cn/Article/details/gt2yxdeqiis.html

@contextlib.contextmanager
来源：http://www.52xcode.cn/Article/details/gt2xmrihfql.html

[U22] Py：矩阵转置
来源：http://www.52xcode.cn/Article/details/gt2zwuexyex.html

list(zip(*m))
来源：http://www.ydjk.org.cn/Article/details/gt2lbystxir.html

[U23] Py：分块读取大文件
来源：http://www.ydjk.org.cn/Article/details/gt2degejffu.html

for chunk in iter(lambda: f.read(8192), b""):
来源：http://www.ydjk.org.cn/Article/details/gt2jrcpyppq.html

[U24] Py：路径操作
来源：http://www.ydjk.org.cn/Article/details/gt2yymnxdop.html

Path("a/b.txt").parent.mkdir(parents=True, exist_ok=True)
来源：http://www.52xcode.cn/Article/details/gt2tqekxege.html

[U25] Py：CSV 按字典读
来源：http://www.52xcode.cn/Article/details/gt2dgpzghwg.html

csv.DictReader(f)
来源：http://www.52xcode.cn/Article/details/gt2mudfkdbg.html

[U26] Py：并发下载
来源：http://www.ydjk.org.cn/Article/details/gt2nnkzwgfo.html

ThreadPoolExecutor(max_workers=8).map(fetch, urls)
来源：http://www.ydjk.org.cn/Article/details/gt2jhqukauh.html

[U27] Py：异步 HTTP
来源：http://www.ydjk.org.cn/Article/details/gt2yavcnqlo.html

aiohttp.ClientSession() 配合 async with
来源：http://www.ydjk.org.cn/Article/details/gt2zkzpzkah.html

[U28] Py：类型别名
来源：http://www.ydjk.org.cn/Article/details/gt2wipcbkts.html

UserId = int
来源：http://www.ydjk.org.cn/Article/details/gt2mmlhpddi.html

[U29] Py：属性校验
来源：http://www.52xcode.cn/Article/details/gt2xzcnzsze.html

@property 与 @x.setter 配合
来源：http://www.52xcode.cn/Article/details/gt2gwyljeus.html

[U30] Py：数据类
来源：http://www.ydjk.org.cn/Article/details/gt2oywnglzw.html

@dataclass(slots=True)
来源：http://www.ydjk.org.cn/Article/details/gt2vsvouvss.html

[U31] Py：单测
来源：http://www.ydjk.org.cn/Article/details/gt2xpaynjsh.html

python -m pytest -q
来源：http://www.ydjk.org.cn/Article/details/gt2prhmhqra.html

[U32] Py：代码格式化
来源：http://www.ydjk.org.cn/Article/details/gt2orwoacvd.html

ruff format . && ruff check --fix .
来源：http://www.52xcode.cn/Article/details/gt2zwsjuztw.html

[U33] Py：打包发布
来源：http://www.52xcode.cn/Article/details/gt2bwmnmypw.html

python -m build  （依赖 pyproject.toml）
来源：http://www.ydjk.org.cn/Article/details/gt2aegynmzr.html

[U34] Py：判断编码
来源：http://www.ydjk.org.cn/Article/details/gt2mzcipiwu.html

chardet.detect(raw)
来源：http://www.52xcode.cn/Article/details/gt2prvuugnz.html

[U35] Py：发送邮件
来源：http://www.52xcode.cn/Article/details/gt2woiovthc.html

smtplib.SMTP_SSL(...).send_message(msg)
来源：http://www.52xcode.cn/Article/details/gt2dowuaiye.html

[U36] Py：定时任务
来源：http://www.ydjk.org.cn/Article/details/gt2jaxdzlfs.html

schedule.every(10).minutes.do(job)
来源：http://www.ydjk.org.cn/Article/details/gt2btiqtqmq.html

[U37] Py：读写 Excel
来源：http://www.ydjk.org.cn/Article/details/gt2dqmmcvkm.html

pandas.read_excel / DataFrame.to_excel
来源：http://www.ydjk.org.cn/Article/details/gt2plifrsry.html

[U38] Py：获取脚本所在目录
来源：http://www.ydjk.org.cn/Article/details/gt2dzwahzkv.html

Path(__file__).resolve().parent
来源：http://www.52xcode.cn/Article/details/gt2wezrnzxc.html

[U39] Py：判断是否在交互环境
来源：http://www.52xcode.cn/Article/details/gt2xarexmnk.html

sys.stdout.isatty()
来源：http://www.ydjk.org.cn/Article/details/gt2prapdibb.html

[U40] Py：打印到标准错误
来源：http://www.ydjk.org.cn/Article/details/gt2txfhirjb.html

print("err", file=sys.stderr)
来源：http://www.52xcode.cn/Article/details/gt2lwjkkxix.html

[U41] PHP：初始化 Composer 项目
来源：http://www.ydjk.org.cn/Article/details/gt2gebshhkb.html

composer init;  composer require guzzlehttp/guzzle
来源：http://www.ydjk.org.cn/Article/details/gt2rpgldcuc.html

[U42] PHP：PSR-4 自动加载
来源：http://www.52xcode.cn/Article/details/gt2vpzhlfdc.html

"autoload": { "psr-4": { "App\\": "src/" } }
来源：http://www.ydjk.org.cn/Article/details/gt2qariqhqr.html

[U43] PHP：声明命名空间
来源：http://www.52xcode.cn/Article/details/gt2pbrungle.html

namespace App\Http;
来源：http://www.52xcode.cn/Article/details/gt2awhbmbah.html

[U44] PHP：开启严格类型
来源：http://www.52xcode.cn/Article/details/gt2ukahhtwi.html

declare(strict_types=1);
来源：http://www.52xcode.cn/Article/details/gt2ughxftoj.html

[U45] PHP：类型声明与返回类型
来源：http://www.ydjk.org.cn/Article/details/gt2tfzxrbey.html

function add(int $a, int $b): int { return $a + $b; }
来源：http://www.52xcode.cn/Article/details/gt2plcouplu.html

[U46] PHP：可空类型
来源：http://www.52xcode.cn/Article/details/gt2fbjcmbam.html

?string $name = null
来源：http://www.52xcode.cn/Article/details/gt2vevtyaws.html

[U47] PHP：联合类型
来源：http://www.52xcode.cn/Article/details/gt2ihaqdmfn.html

int|string $id
来源：http://www.52xcode.cn/Article/details/gt2mubotsia.html

[U48] PHP：纯枚举
来源：http://www.ydjk.org.cn/Article/details/gt2frqxguiu.html

enum Status: string { case Active = "active"; case Off = "off"; }
来源：http://www.52xcode.cn/Article/details/gt2vpgueffp.html

[U49] PHP：只读属性
来源：http://www.52xcode.cn/Article/details/gt2wbauagav.html

public readonly string $name
来源：http://www.52xcode.cn/Article/details/gt2ybgfkhbc.html

[U50] PHP：构造器属性提升
来源：http://www.52xcode.cn/Article/details/gt2pcdtguyn.html

public function __construct(private int $id) {}
来源：http://www.52xcode.cn/Article/details/gt2vcidlxbe.html

[U51] PHP：数组解构
来源：http://www.ydjk.org.cn/Article/details/gt2npammlww.html

[$a, $b] = $arr;
来源：http://www.52xcode.cn/Article/details/gt2jxwxbwxl.html

[U52] PHP：箭头函数
来源：http://www.52xcode.cn/Article/details/gt2csvewpxc.html

$double = fn($x) => $x * 2;
来源：http://www.52xcode.cn/Article/details/gt2rpohhesg.html

[U53] PHP：空合并运算符
来源：http://www.ydjk.org.cn/Article/details/gt2xfjpqvoe.html

$v = $a ?? $b ?? "default";
来源：http://www.ydjk.org.cn/Article/details/gt2jikvwjwn.html

[U54] PHP：空安全调用
来源：http://www.ydjk.org.cn/Article/details/gt2nviixrbw.html

$obj?->method()
来源：http://www.52xcode.cn/Article/details/gt2tbjnqmcp.html

[U55] PHP：match 表达式
来源：http://www.52xcode.cn/Article/details/gt2duhltbqp.html

$s = match($x) { 1 => "一", default => "其他" };
来源：http://www.ydjk.org.cn/Article/details/gt2mjtivtoj.html

[U56] PHP：命名参数
来源：http://www.52xcode.cn/Article/details/gt2hraatfga.html

f(a: 1, b: 2)
来源：http://www.52xcode.cn/Article/details/gt2lkayjhxc.html

[U57] PHP：字符串插值
来源：http://www.52xcode.cn/Article/details/gt2gdcaskdf.html

"值: {$a}"
来源：http://www.52xcode.cn/Article/details/gt2avobrjhq.html

[U58] PHP：数组三件套
来源：http://www.ydjk.org.cn/Article/details/gt2ngmjkoku.html

array_map($f, $a);  array_filter($a, $f);  array_reduce($a, $f, 0);
来源：http://www.52xcode.cn/Article/details/gt2cuitmych.html

[U59] PHP：自定义排序
来源：http://www.ydjk.org.cn/Article/details/gt2zfozqqrb.html

usort($arr, fn($a, $b) => $a["age"] <=> $b["age"]);
来源：http://www.52xcode.cn/Article/details/gt2zagifabl.html

[U60] PHP：JSON 编解码
来源：http://www.52xcode.cn/Article/details/gt2zzlvxzam.html

json_encode($d, JSON_UNESCAPED_UNICODE);  json_decode($s, true);
来源：http://www.ydjk.org.cn/Article/details/gt2oguvzsxm.html

[U61] PHP：正则
来源：http://www.ydjk.org.cn/Article/details/gt2trigggex.html

preg_match('/(\d+)/', $s, $m);  preg_replace('/\d+/', '#', $s);
来源：http://www.52xcode.cn/Article/details/gt2jpkzcrgn.html

[U62] PHP：日期对象
来源：http://www.ydjk.org.cn/Article/details/gt2ipyytzcr.html

(new DateTimeImmutable())->format("Y-m-d");
来源：http://www.52xcode.cn/Article/details/gt2okwkxady.html

[U63] PHP：文件读写
来源：http://www.ydjk.org.cn/Article/details/gt2kuxugeal.html

file_get_contents($f);  file_put_contents($f, $data);
来源：http://www.52xcode.cn/Article/details/gt2rtjjelzs.html

[U64] PHP：目录遍历
来源：http://www.52xcode.cn/Article/details/gt2dvqnqeaa.html

glob("dir/*.php");  scandir("dir");
来源：http://www.ydjk.org.cn/Article/details/gt2uanoynyr.html

[U65] PHP：会话
来源：http://www.52xcode.cn/Article/details/gt2woxjtrqd.html

session_start();  $_SESSION["uid"] = 1;
来源：http://www.52xcode.cn/Article/details/gt2gdxvoaya.html

[U66] PHP：设置 Cookie
来源：http://www.52xcode.cn/Article/details/gt2wphkvqxa.html

setcookie("token", $v, ["httponly" => true, "samesite" => "Lax"]);
来源：http://www.ydjk.org.cn/Article/details/gt2octfewvo.html

[U67] PHP：处理文件上传
来源：http://www.ydjk.org.cn/Article/details/gt2obluikhg.html

$_FILES["file"]["tmp_name"] 与 move_uploaded_file()
来源：http://www.52xcode.cn/Article/details/gt2wzxgtkgb.html

[U68] PHP：PDO 连接
来源：http://www.52xcode.cn/Article/details/gt2ppsjffqk.html

$pdo = new PDO("mysql:host=localhost;dbname=app", "root", "");
来源：http://www.52xcode.cn/Article/details/gt2tthdxojz.html

[U69] PHP：PDO 预处理
来源：http://www.ydjk.org.cn/Article/details/gt2cgskleex.html

$stmt = $pdo->prepare("SELECT * FROM users WHERE id = ?");  $stmt->execute([$id]);
来源：http://www.52xcode.cn/Article/details/gt2pklrhduf.html

[U70] PHP：PDO 事务
来源：http://www.ydjk.org.cn/Article/details/gt2ensluymm.html

$pdo->beginTransaction();  $pdo->commit();  $pdo->rollBack();
来源：http://www.52xcode.cn/Article/details/gt2mrwhzbwz.html

[U71] PHP：抛出异常
来源：http://www.ydjk.org.cn/Article/details/gt2unhuznvn.html

throw new RuntimeException("失败", 500);
来源：http://www.ydjk.org.cn/Article/details/gt2icuyjxan.html

[U72] PHP：写错误日志
来源：http://www.52xcode.cn/Article/details/gt2adbgomxd.html

error_log("失败: " . $e->getMessage());
来源：http://www.52xcode.cn/Article/details/gt2hhtkbqte.html

[U73] PHP：读取 ini 配置
来源：http://www.ydjk.org.cn/Article/details/gt2qjjygoac.html

parse_ini_file("config.ini", true)
来源：http://www.52xcode.cn/Article/details/gt2wkgttkbe.html

[U74] PHP：读取环境变量
来源：http://www.ydjk.org.cn/Article/details/gt2ahxonrnq.html

getenv("APP_ENV") ?: "production"
来源：http://www.52xcode.cn/Article/details/gt2uvjokwtz.html

[U75] PHP：依赖注入
来源：http://www.52xcode.cn/Article/details/gt2vfhxthxy.html

composer require psr/container
来源：http://www.ydjk.org.cn/Article/details/gt2kkwacmwu.html

[U76] PHP：简单路由
来源：http://www.ydjk.org.cn/Article/details/gt2mscxuiou.html

$path = parse_url($_SERVER["REQUEST_URI"], PHP_URL_PATH);
来源：http://www.ydjk.org.cn/Article/details/gt2ibxkfzzj.html

[U77] PHP：模板渲染
来源：http://www.52xcode.cn/Article/details/gt2fysmakst.html

composer require twig/twig
来源：http://www.ydjk.org.cn/Article/details/gt2hfkmrwov.html

[U78] PHP：单元测试
来源：http://www.52xcode.cn/Article/details/gt2vdhqbdbb.html

composer require --dev phpunit/phpunit
来源：http://www.ydjk.org.cn/Article/details/gt2cpblypmh.html

[U79] PHP：静态分析
来源：http://www.52xcode.cn/Article/details/gt2dgogfkje.html

composer require --dev phpstan/phpstan
来源：http://www.52xcode.cn/Article/details/gt2kmawcbzs.html

[U80] PHP：代码规范修复
来源：http://www.ydjk.org.cn/Article/details/gt2sroikfbc.html

composer require --dev friendsofphp/php-cs-fixer
来源：http://www.ydjk.org.cn/Article/details/gt2iaoxjgkz.html

[U81] JS：初始化项目
来源：http://www.52xcode.cn/Article/details/gt2kntqtixm.html

npm init -y;  npm i express
来源：http://www.52xcode.cn/Article/details/gt2uueelzkt.html

[U82] JS：package.json 脚本
来源：http://www.ydjk.org.cn/Article/details/gt2hnzzioqk.html

"scripts": { "dev": "vite", "build": "vite build" }
来源：http://www.ydjk.org.cn/Article/details/gt2cvskabks.html

[U83] JS：ES Module 导入导出
来源：http://www.ydjk.org.cn/Article/details/gt2selbufyr.html

export const a = 1;  import { a } from "./m.js";
来源：http://www.52xcode.cn/Article/details/gt2ysveffdj.html

[U84] JS：CommonJS 写法
来源：http://www.52xcode.cn/Article/details/gt2vdkjqvmw.html

module.exports = { a };  const { a } = require("./m");
来源：http://www.ydjk.org.cn/Article/details/gt2pbrluece.html

[U85] JS：可选链
来源：http://www.ydjk.org.cn/Article/details/gt2nbakskdz.html

a?.b?.c
来源：http://www.52xcode.cn/Article/details/gt2ixfdqtwj.html

[U86] JS：空值合并
来源：http://www.ydjk.org.cn/Article/details/gt2yyilpglv.html

a ?? b
来源：http://www.52xcode.cn/Article/details/gt2mplqniea.html

[U87] JS：解构默认值
来源：http://www.ydjk.org.cn/Article/details/gt2vdgebrrs.html

const { a = 1, b = 2 } = obj;
来源：http://www.52xcode.cn/Article/details/gt2mtjzndaa.html

[U88] JS：对象展开合并
来源：http://www.ydjk.org.cn/Article/details/gt2zopddard.html

{ ...a, ...b }
来源：http://www.52xcode.cn/Article/details/gt2gahuqnyt.html

[U89] JS：数组去重
来源：http://www.ydjk.org.cn/Article/details/gt2fxmvbutk.html

[...new Set(arr)]
来源：http://www.52xcode.cn/Article/details/gt2hkgvgsjr.html

[U90] JS：数字数组排序
来源：http://www.ydjk.org.cn/Article/details/gt2isiogqlm.html

[...arr].sort((a, b) => a - b)
来源：http://www.ydjk.org.cn/Article/details/gt2xheemayn.html

[U91] JS：对象键值遍历
来源：http://www.ydjk.org.cn/Article/details/gt2zmjghqer.html

Object.entries(obj).forEach(([k, v]) => {});
来源：http://www.52xcode.cn/Article/details/gt2lfaywqlk.html

[U92] JS：深拷贝
来源：http://www.52xcode.cn/Article/details/gt2zpvzfccl.html

structuredClone(obj)
来源：http://www.ydjk.org.cn/Article/details/gt2prptluea.html

[U93] JS：模板字符串
来源：http://www.ydjk.org.cn/Article/details/gt2jquocorj.html

`共 ${n} 条`
来源：http://www.52xcode.cn/Article/details/gt2rvkbaeap.html

[U94] JS：箭头函数
来源：http://www.52xcode.cn/Article/details/gt2hokmypqb.html

const double = x => x * 2;
来源：http://www.52xcode.cn/Article/details/gt2iqyrcgzv.html

[U95] JS：Promise 包装
来源：http://www.ydjk.org.cn/Article/details/gt2covnzbih.html

new Promise((resolve, reject) => {})
来源：http://www.52xcode.cn/Article/details/gt2wlugdwep.html

[U96] JS：async/await 与异常
来源：http://www.ydjk.org.cn/Article/details/gt2ehnkcspx.html

try { const d = await f(); } catch (e) { console.error(e); }
来源：http://www.ydjk.org.cn/Article/details/gt2tmrjjkcu.html

[U97] JS：并发请求
来源：http://www.ydjk.org.cn/Article/details/gt2ipkbginy.html

await Promise.all(urls.map(u => fetch(u)))
来源：http://www.ydjk.org.cn/Article/details/gt2unkobvxk.html

[U98] JS：fetch 带 JSON
来源：http://www.52xcode.cn/Article/details/gt2orguymoz.html

await fetch(url, { method: "POST", headers: { "Content-Type": "application/json" }, body: JSON.stringify(d) })
来源：http://www.ydjk.org.cn/Article/details/gt2otulkmiu.html

[U99] JS：事件监听
来源：http://www.52xcode.cn/Article/details/gt2wjguecvs.html

el.addEventListener("click", e => {})
来源：http://www.52xcode.cn/Article/details/gt2byulufyv.html

[U100] JS：DOM 查询
来源：http://www.ydjk.org.cn/Article/details/gt2xukjndgw.html

document.querySelector(".item")
来源：http://www.ydjk.org.cn/Article/details/gt2ujibtxdx.html

[U101] JS：classList 操作
来源：http://www.ydjk.org.cn/Article/details/gt2gekdthfc.html

el.classList.toggle("active")
来源：http://www.52xcode.cn/Article/details/gt2gvyxioir.html

[U102] JS：本地存储
来源：http://www.ydjk.org.cn/Article/details/gt2ywpyrwcj.html

localStorage.setItem("k", JSON.stringify(v))
来源：http://www.ydjk.org.cn/Article/details/gt2tqjakxoq.html

[U103] JS：定时器
来源：http://www.ydjk.org.cn/Article/details/gt2mqdiamfq.html

setTimeout(fn, 1000);  setInterval(fn, 1000);
来源：http://www.52xcode.cn/Article/details/gt2nzsuehob.html

[U104] JS：防抖
来源：http://www.ydjk.org.cn/Article/details/gt2eoveswul.html

const debounce = (fn, ms) => { let t; return (...a) => { clearTimeout(t); t = setTimeout(() => fn(...a), ms); }; };
来源：http://www.ydjk.org.cn/Article/details/gt2xhuzyawz.html

[U105] JS：节流
来源：http://www.52xcode.cn/Article/details/gt2uysfuxag.html

const throttle = (fn, ms) => { let last = 0; return (...a) => { const n = Date.now(); if (n - last >= ms) { last = n; fn(...a); } }; };
来源：http://www.ydjk.org.cn/Article/details/gt2cppphecg.html

[U106] JS：日期格式化
来源：http://www.ydjk.org.cn/Article/details/gt2intbmdpq.html

new Intl.DateTimeFormat("zh-CN", { dateStyle: "medium" }).format(new Date())
来源：http://www.ydjk.org.cn/Article/details/gt2qmhtwbcx.html

[U107] JS：数字千分位
来源：http://www.ydjk.org.cn/Article/details/gt2jfozumxd.html

new Intl.NumberFormat("en-US").format(1234567)
来源：http://www.ydjk.org.cn/Article/details/gt2tcnnwnul.html

[U108] JS：随机整数
来源：http://www.52xcode.cn/Article/details/gt2mnyxhdmm.html

Math.floor(Math.random() * (max - min + 1)) + min
来源：http://www.ydjk.org.cn/Article/details/gt2awmnwrfi.html

[U109] JS：数组分组
来源：http://www.52xcode.cn/Article/details/gt2nnmfckxk.html

Object.groupBy(arr, x => x.type)
来源：http://www.52xcode.cn/Article/details/gt2zkwmywrh.html

[U110] JS：数组分块
来源：http://www.ydjk.org.cn/Article/details/gt2flaxextb.html

arr.reduce((acc, x, i) => (i % size ? acc : [...acc, arr.slice(i, i + size)]), [])
来源：http://www.ydjk.org.cn/Article/details/gt2ifmeydze.html

[U111] JS：对象转 Map
来源：http://www.ydjk.org.cn/Article/details/gt2pbihfauu.html

new Map(Object.entries(obj))
来源：http://www.52xcode.cn/Article/details/gt2humckzzu.html

[U112] JS：字符串补位
来源：http://www.52xcode.cn/Article/details/gt2itxrbvjf.html

"7".padStart(3, "0")
来源：http://www.52xcode.cn/Article/details/gt2jcksvnfg.html

[U113] JS：正则替换全部
来源：http://www.52xcode.cn/Article/details/gt2emaedzcg.html

s.replaceAll("a", "b")
来源：http://www.52xcode.cn/Article/details/gt2ibodduyd.html

[U114] JS：JSON 深比较
来源：http://www.52xcode.cn/Article/details/gt2nqdkmuwa.html

JSON.stringify(a) === JSON.stringify(b)
来源：http://www.ydjk.org.cn/Article/details/gt2qrcvoouw.html

[U115] JS：生成 UUID
来源：http://www.ydjk.org.cn/Article/details/gt2urphxoif.html

crypto.randomUUID()
来源：http://www.52xcode.cn/Article/details/gt2yaqqrglt.html

[U116] JS：类型检查（JSDoc）
来源：http://www.ydjk.org.cn/Article/details/gt2sqbectkb.html

/** @param {string} name */ function f(name) {}
来源：http://www.ydjk.org.cn/Article/details/gt2wzxsrrjl.html

[U117] JS：单元测试
来源：http://www.ydjk.org.cn/Article/details/gt2kxiatogw.html

npm i -D vitest;  npx vitest
来源：http://www.ydjk.org.cn/Article/details/gt2utvmsqfg.html

[U118] JS：开发服务器
来源：http://www.ydjk.org.cn/Article/details/gt2wvwjddus.html

npm i -D vite;  npx vite
来源：http://www.ydjk.org.cn/Article/details/gt2lvbhpuqg.html

[U119] JS：生产构建
来源：http://www.52xcode.cn/Article/details/gt2zszjczzl.html

npx vite build
来源：http://www.52xcode.cn/Article/details/gt2eltndtnb.html

[U120] JS：读取环境变量（Vite）
来源：http://www.ydjk.org.cn/Article/details/gt2kpvdvupz.html

import.meta.env.VITE_API_URL
来源：http://www.52xcode.cn/Article/details/gt2numdykuh.html

================================================================================
来源：http://www.ydjk.org.cn/Article/details/gt2apsyomxs.html

统计汇总
来源：http://www.52xcode.cn/Article/details/gt2tocacqhd.html

================================================================================
来源：http://www.ydjk.org.cn/Article/details/gt2yxyjhbor.html

按语言统计（条）：
来源：http://www.ydjk.org.cn/Article/details/gt2bvwxgjgk.html

Python ......... 252
来源：http://www.52xcode.cn/Article/details/gt2wbnezsop.html

PHP ............ 252
来源：http://www.52xcode.cn/Article/details/gt2nlcritlf.html

JavaScript ..... 252
来源：http://www.52xcode.cn/Article/details/gt2ywakybqp.html

TypeScript ..... 212
来源：http://www.ydjk.org.cn/Article/details/gt2zurdrfrx.html

Java ........... 212
来源：http://www.52xcode.cn/Article/details/gt2ydkhqlbz.html

Go ............. 212
来源：http://www.52xcode.cn/Article/details/gt2tizsvagi.html

Ruby ........... 212
来源：http://www.52xcode.cn/Article/details/gt2fwtigvgl.html

C# ............. 212
来源：http://www.ydjk.org.cn/Article/details/gt2jikvsknl.html

C .............. 30
来源：http://www.52xcode.cn/Article/details/gt2oqnuvuaq.html

C++ ............ 30
来源：http://www.ydjk.org.cn/Article/details/gt2mwbgjorh.html

SQL ............ 90
来源：http://www.52xcode.cn/Article/details/gt2jurwqyqf.html

Bash ........... 80
来源：http://www.ydjk.org.cn/Article/details/gt2exqqkvff.html

Kotlin ......... 15
来源：http://www.ydjk.org.cn/Article/details/gt2twylyxol.html

Swift .......... 15
来源：http://www.52xcode.cn/Article/details/gt2sjmciqet.html

Lua ............ 10
来源：http://www.ydjk.org.cn/Article/details/gt2izcbmpga.html

Perl ........... 10
来源：http://www.ydjk.org.cn/Article/details/gt2wyrtlbrw.html

Scala .......... 10
来源：http://www.ydjk.org.cn/Article/details/gt2nfkptlny.html

------------------------------------
来源：http://www.52xcode.cn/Article/details/gt2bmmovkpu.html

合计 ........... 2106 条
来源：http://www.52xcode.cn/Article/details/gt2vnakyhpc.html

按章节统计：
来源：http://www.ydjk.org.cn/Article/details/gt2xwjorqzs.html

A 基础语法与类型       26 个任务 × 8 语言 =  208
来源：http://www.ydjk.org.cn/Article/details/gt2vrvvlbwo.html

B 流程控制             16 个任务 × 8 语言 =  128
来源：http://www.52xcode.cn/Article/details/gt2kzebjihx.html

C 函数与作用域         16 个任务 × 8 语言 =  128
来源：http://www.52xcode.cn/Article/details/gt2tsssihdt.html

D 数组 / 列表 / 集合   26 个任务 × 8 语言 =  208
来源：http://www.ydjk.org.cn/Article/details/gt2zjhijycw.html

E 字符串处理           22 个任务 × 8 语言 =  176
来源：http://www.ydjk.org.cn/Article/details/gt2bfztalee.html

F 文件与目录           12 个任务 × 8 语言 =   96
来源：http://www.ydjk.org.cn/Article/details/gt2qlveqmra.html

G 面向对象             16 个任务 × 8 语言 =  128
来源：http://www.ydjk.org.cn/Article/details/gt2apudpqvq.html

H 异常与错误处理       10 个任务 × 8 语言 =   80
来源：http://www.52xcode.cn/Article/details/gt2bzfbwnsj.html

I 正则表达式            8 个任务 × 8 语言 =   64
来源：http://www.ydjk.org.cn/Article/details/gt2lablxhwl.html

J 日期与时间           10 个任务 × 8 语言 =   80
来源：http://www.52xcode.cn/Article/details/gt2uigcfroa.html

K JSON 与序列化         8 个任务 × 8 语言 =   64
来源：http://www.52xcode.cn/Article/details/gt2xpehkfii.html

L 网络请求              8 个任务 × 8 语言 =   64
来源：http://www.ydjk.org.cn/Article/details/gt2gjpqkybb.html

M 命令行 / 进程         8 个任务 × 8 语言 =   64
来源：http://www.ydjk.org.cn/Article/details/gt2oqzuxiaw.html

N 数据结构与算法       12 个任务 × 8 语言 =   96
来源：http://www.52xcode.cn/Article/details/gt2rqjcicor.html

O 并发与异步            6 个任务 × 8 语言 =   48
来源：http://www.52xcode.cn/Article/details/gt2zoeypaic.html

P 常用工具函数          8 个任务 × 8 语言 =   64
来源：http://www.ydjk.org.cn/Article/details/gt2obnankuq.html

Q SQL 专题                              90
来源：http://www.ydjk.org.cn/Article/details/gt2fnvhekyl.html

R Bash 专题                             80
来源：http://www.52xcode.cn/Article/details/gt2xjnbalco.html

S C / C++ 专题                          60
来源：http://www.ydjk.org.cn/Article/details/gt2hobllbue.html

T 其他语言补充                          60
来源：http://www.ydjk.org.cn/Article/details/gt2ovirwhvm.html

U 高频实用片段                         120
来源：http://www.52xcode.cn/Article/details/gt2eeujcmsq.html

------------------------------------
来源：http://www.52xcode.cn/Article/details/gt2vevogyjj.html

合计                                  2106 条
来源：http://www.52xcode.cn/Article/details/gt2zyyurncz.html

--------------------------------------------------------------------------------
来源：http://www.ydjk.org.cn/Article/details/gt2ukoytnzr.html

使用提醒
来源：http://www.52xcode.cn/Article/details/gt2eqbecatw.html

--------------------------------------------------------------------------------
来源：http://www.ydjk.org.cn/Article/details/gt2pgibuomi.html

1. 示例追求"最小可用"，正式项目中请补齐导入、错误处理与边界判断。
来源：http://www.52xcode.cn/Article/details/gt2xesayjid.html

2. 涉及文件、网络、数据库的示例，注意资源释放与异常捕获。
来源：http://www.ydjk.org.cn/Article/details/gt2bebuiofo.html

3. 语言版本差异较大（如 Python 3.10 的 match、Java 17 的 record/switch 箭头），
来源：http://www.ydjk.org.cn/Article/details/gt2buaruwgg.html

在旧版本上使用前请先确认语法支持情况。
来源：http://www.ydjk.org.cn/Article/details/gt2bjrjofzc.html

4. 标注"手写"的条目是因为该语言缺少对应内置能力，实际项目中可引入成熟库。
来源：http://www.ydjk.org.cn/Article/details/gt2qpukfqiv.html

—— 文件结束 ——
来源：http://www.52xcode.cn/Article/details/gt2icfmlbav.html

================================================================================
来源：http://www.ydjk.org.cn/Article/details/gt2objmlilx.html

程序语言常见例子速查手册（2024 版）
来源：http://www.52xcode.cn/Article/details/gt2cvxghpot.html

Common Programming Examples Cheat Book
来源：http://www.ydjk.org.cn/Article/details/gt2ggstpcje.html

================================================================================
来源：http://www.52xcode.cn/Article/details/gt2hpzmmfvu.html

【收录内容】
来源：http://www.ydjk.org.cn/Article/details/gt2pwhfzufp.html

覆盖 12 种语言 / 语法与常见 API：
来源：http://www.52xcode.cn/Article/details/gt2dayhwsxk.html

Python · PHP · JavaScript · TypeScript · Java · Go · Ruby · C#
来源：http://www.ydjk.org.cn/Article/details/gt2sqguyaxk.html

SQL · Bash · C · C++
来源：http://www.52xcode.cn/Article/details/gt2ujhphnzm.html

按「任务」分组：每个任务下按语言各给出一条最小可用示例。
来源：http://www.52xcode.cn/Article/details/gt2fhvezvvs.html

【使用说明】
来源：http://www.ydjk.org.cn/Article/details/gt2ghdrwqei.html

1. 每个任务形如 "[编号] 任务名"，下面每行以语言标记开头：
来源：http://www.52xcode.cn/Article/details/gt2rcasxahb.html

Py:    Python        PHP:   PHP           JS:    JavaScript
来源：http://www.ydjk.org.cn/Article/details/gt2xvyfcaks.html

TS:    TypeScript    Java:  Java          Go:    Go
来源：http://www.ydjk.org.cn/Article/details/gt2hptpcsto.html

Ruby:  Ruby          C#:    C#            SQL:   SQL
来源：http://www.52xcode.cn/Article/details/gt2lxkemhcd.html

Bash:  Shell         C:     C             C++:   C++
来源：http://www.52xcode.cn/Article/details/gt2eswhkpwx.html

2. 示例只展示核心写法，刻意省略 import / require / include / using 等样板代码。
来源：http://www.ydjk.org.cn/Article/details/gt2xybuvaom.html

需要完整可运行文件时，请自行补齐当前语言的导入语句。
来源：http://www.52xcode.cn/Article/details/gt2ldmxhfrx.html

3. 语法基准：Python 3.10+ / PHP 8.1+ / ES2020+ / TypeScript 5 / Java 17 /
来源：http://www.52xcode.cn/Article/details/gt2bwcebbie.html

Go 1.21+ / Ruby 3.x / C# 10+ / C17 / C++17。
来源：http://www.ydjk.org.cn/Article/details/gt2elooxwmx.html

4. 检索建议：用编辑器或浏览器 Ctrl+F 搜关键词，如 "排序" "读取文件" "正则"。
来源：http://www.52xcode.cn/Article/details/gt2pgcyzgbi.html

5. 标记为 "// 无" 表示该语言没有对应的一等语法，需用替代写法（示例给出替代方案）。
来源：http://www.52xcode.cn/Article/details/gt2ywebgyjj.html

6. 符号 "⏎" 表示代码在此处换行（主要用于 Python 等强制缩进、无法压成一行的结构）。
来源：http://www.52xcode.cn/Article/details/gt2ljgcfihz.html

【文件统计】
来源：http://www.52xcode.cn/Article/details/gt2mrlefuwh.html

语言示例共 2106 条，分布见本文末尾的「统计汇总」。
来源：http://www.ydjk.org.cn/Article/details/gt2qoyckoei.html

--------------------------------------------------------------------------------
来源：http://www.ydjk.org.cn/Article/details/gt2wjjjuuud.html

目  录
来源：http://www.52xcode.cn/Article/details/gt2kpeqlmah.html

--------------------------------------------------------------------------------
来源：http://www.ydjk.org.cn/Article/details/gt2sviobdce.html

A. 基础语法与类型              （第 1 节，26 个任务，208 条）
来源：http://www.52xcode.cn/Article/details/gt2nwlqujwt.html

B. 流程控制                    （第 2 节，16 个任务，128 条）
来源：http://www.ydjk.org.cn/Article/details/gt2cdaehldq.html

C. 函数与作用域                （第 3 节，16 个任务，128 条）
来源：http://www.52xcode.cn/Article/details/gt2mvzngwmz.html

D. 数组 / 列表 / 集合          （第 4 节，26 个任务，208 条）
来源：http://www.ydjk.org.cn/Article/details/gt2vqibxsqz.html

E. 字符串处理                  （第 5 节，22 个任务，176 条）
来源：http://www.ydjk.org.cn/Article/details/gt2isjzuqfn.html

F. 文件与目录                  （第 6 节，12 个任务，96 条）
来源：http://www.ydjk.org.cn/Article/details/gt2lngsxidl.html

G. 面向对象                    （第 7 节，16 个任务，128 条）
来源：http://www.ydjk.org.cn/Article/details/gt2xutloclp.html

H. 异常与错误处理              （第 8 节，10 个任务，80 条）
来源：http://www.ydjk.org.cn/Article/details/gt2rgmkoxcg.html

I. 正则表达式                  （第 9 节，8 个任务，64 条）
来源：http://www.52xcode.cn/Article/details/gt2duvamnir.html


<!-- 参考信息 -->