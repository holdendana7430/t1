代发 wailian999

[U19] Py：正则替换带回调
来源：http://www.ydjk.org.cn/Article/details/gt2lhjgkyne.html

re.sub(r"\d+", lambda m: str(int(m.group()) * 2), s)
来源：http://www.52xcode.cn/Article/details/gt2fyfipnxi.html

[U20] Py：缓存函数结果
来源：http://www.ydjk.org.cn/Article/details/gt2qkqwqfzd.html

@functools.lru_cache(maxsize=None)
来源：http://www.52xcode.cn/Article/details/gt2oivgotvy.html

[U21] Py：自定义上下文管理器
来源：http://www.52xcode.cn/Article/details/gt2yxhkxojt.html

@contextlib.contextmanager
来源：http://www.52xcode.cn/Article/details/gt2axlgemzq.html

[U22] Py：矩阵转置
来源：http://www.52xcode.cn/Article/details/gt2dxduaonj.html

list(zip(*m))
来源：http://www.52xcode.cn/Article/details/gt2bznfiamn.html

[U23] Py：分块读取大文件
来源：http://www.ydjk.org.cn/Article/details/gt2ulmmscwl.html

for chunk in iter(lambda: f.read(8192), b""):
来源：http://www.ydjk.org.cn/Article/details/gt2jhedivny.html

[U24] Py：路径操作
来源：http://www.ydjk.org.cn/Article/details/gt2fsebsllp.html

Path("a/b.txt").parent.mkdir(parents=True, exist_ok=True)
来源：http://www.52xcode.cn/Article/details/gt2fzwnwiro.html

[U25] Py：CSV 按字典读
来源：http://www.ydjk.org.cn/Article/details/gt2txkbjyjg.html

csv.DictReader(f)
来源：http://www.ydjk.org.cn/Article/details/gt2lfqhhuwr.html

[U26] Py：并发下载
来源：http://www.52xcode.cn/Article/details/gt2ufubcvmy.html

ThreadPoolExecutor(max_workers=8).map(fetch, urls)
来源：http://www.ydjk.org.cn/Article/details/gt2cqmfwuzs.html

[U27] Py：异步 HTTP
来源：http://www.52xcode.cn/Article/details/gt2zcvhvnkr.html

aiohttp.ClientSession() 配合 async with
来源：http://www.ydjk.org.cn/Article/details/gt2vcjpsykx.html

[U28] Py：类型别名
来源：http://www.52xcode.cn/Article/details/gt2xfrehqrt.html

UserId = int
来源：http://www.52xcode.cn/Article/details/gt2hqidxtml.html

[U29] Py：属性校验
来源：http://www.ydjk.org.cn/Article/details/gt2rqpxyash.html

@property 与 @x.setter 配合
来源：http://www.ydjk.org.cn/Article/details/gt2acioxnfm.html

[U30] Py：数据类
来源：http://www.52xcode.cn/Article/details/gt2jjnirzgd.html

@dataclass(slots=True)
来源：http://www.ydjk.org.cn/Article/details/gt2zkpnfadv.html

[U31] Py：单测
来源：http://www.52xcode.cn/Article/details/gt2hlndlolg.html

python -m pytest -q
来源：http://www.52xcode.cn/Article/details/gt2sjjykrpa.html

[U32] Py：代码格式化
来源：http://www.52xcode.cn/Article/details/gt2itmnmztn.html

ruff format . && ruff check --fix .
来源：http://www.52xcode.cn/Article/details/gt2lfzifibe.html

[U33] Py：打包发布
来源：http://www.52xcode.cn/Article/details/gt2nferuvtr.html

python -m build  （依赖 pyproject.toml）
来源：http://www.52xcode.cn/Article/details/gt2yuoylewe.html

[U34] Py：判断编码
来源：http://www.52xcode.cn/Article/details/gt2oxlmeahd.html

chardet.detect(raw)
来源：http://www.52xcode.cn/Article/details/gt2qbmifisa.html

[U35] Py：发送邮件
来源：http://www.52xcode.cn/Article/details/gt2tymgrpub.html

smtplib.SMTP_SSL(...).send_message(msg)
来源：http://www.52xcode.cn/Article/details/gt2ruupmxes.html

[U36] Py：定时任务
来源：http://www.52xcode.cn/Article/details/gt2zakejaal.html

schedule.every(10).minutes.do(job)
来源：http://www.52xcode.cn/Article/details/gt2ggzszzzi.html

[U37] Py：读写 Excel
来源：http://www.52xcode.cn/Article/details/gt2awiqufbf.html

pandas.read_excel / DataFrame.to_excel
来源：http://www.52xcode.cn/Article/details/gt2gqpgojuq.html

[U38] Py：获取脚本所在目录
来源：http://www.52xcode.cn/Article/details/gt2pakczify.html

Path(__file__).resolve().parent
来源：http://www.52xcode.cn/Article/details/gt2biuweptr.html

[U39] Py：判断是否在交互环境
来源：http://www.52xcode.cn/Article/details/gt2bkkqxzeq.html

sys.stdout.isatty()
来源：http://www.ydjk.org.cn/Article/details/gt2cyxcwjdt.html

[U40] Py：打印到标准错误
来源：http://www.ydjk.org.cn/Article/details/gt2zhlamcxa.html

print("err", file=sys.stderr)
来源：http://www.52xcode.cn/Article/details/gt2yetivoqj.html

[U41] PHP：初始化 Composer 项目
来源：http://www.52xcode.cn/Article/details/gt2cdyhvsoo.html

composer init;  composer require guzzlehttp/guzzle
来源：http://www.ydjk.org.cn/Article/details/gt2rnlhrxpp.html

[U42] PHP：PSR-4 自动加载
来源：http://www.ydjk.org.cn/Article/details/gt2mmhehezc.html

"autoload": { "psr-4": { "App\\": "src/" } }
来源：http://www.52xcode.cn/Article/details/gt2rpgpclqo.html

[U43] PHP：声明命名空间
来源：http://www.ydjk.org.cn/Article/details/gt2roqtbhdh.html

namespace App\Http;
来源：http://www.52xcode.cn/Article/details/gt2axrphgyc.html

[U44] PHP：开启严格类型
来源：http://www.ydjk.org.cn/Article/details/gt2nypegiyw.html

declare(strict_types=1);
来源：http://www.ydjk.org.cn/Article/details/gt2julobgkk.html

[U45] PHP：类型声明与返回类型
来源：http://www.52xcode.cn/Article/details/gt2nnrejtjc.html

function add(int $a, int $b): int { return $a + $b; }
来源：http://www.ydjk.org.cn/Article/details/gt2lbdrvusj.html

[U46] PHP：可空类型
来源：http://www.52xcode.cn/Article/details/gt2mckqamzz.html

?string $name = null
来源：http://www.ydjk.org.cn/Article/details/gt2ccogbvik.html

[U47] PHP：联合类型
来源：http://www.ydjk.org.cn/Article/details/gt2wirwdpwj.html

int|string $id
来源：http://www.ydjk.org.cn/Article/details/gt2lgqqgihl.html

[U48] PHP：纯枚举
来源：http://www.52xcode.cn/Article/details/gt2vwxkqwld.html

enum Status: string { case Active = "active"; case Off = "off"; }
来源：http://www.ydjk.org.cn/Article/details/gt2oagvrity.html

[U49] PHP：只读属性
来源：http://www.ydjk.org.cn/Article/details/gt2neoiwmfc.html

public readonly string $name
来源：http://www.52xcode.cn/Article/details/gt2rjakicmn.html

[U50] PHP：构造器属性提升
来源：http://www.52xcode.cn/Article/details/gt2mdgvobkx.html

public function __construct(private int $id) {}
来源：http://www.ydjk.org.cn/Article/details/gt2gcfvderd.html

[U51] PHP：数组解构
来源：http://www.ydjk.org.cn/Article/details/gt2wlwzylto.html

[$a, $b] = $arr;
来源：http://www.52xcode.cn/Article/details/gt2vtwmvwoj.html

[U52] PHP：箭头函数
来源：http://www.52xcode.cn/Article/details/gt2qesozwmx.html

$double = fn($x) => $x * 2;
来源：http://www.52xcode.cn/Article/details/gt2chanzvno.html

[U53] PHP：空合并运算符
来源：http://www.52xcode.cn/Article/details/gt2vuvywtvs.html

$v = $a ?? $b ?? "default";
来源：http://www.ydjk.org.cn/Article/details/gt2ywahgcbr.html

[U54] PHP：空安全调用
来源：http://www.ydjk.org.cn/Article/details/gt2kahjsvzd.html

$obj?->method()
来源：http://www.52xcode.cn/Article/details/gt2imqzlzbw.html

[U55] PHP：match 表达式
来源：http://www.52xcode.cn/Article/details/gt2zqgzvaiv.html

$s = match($x) { 1 => "一", default => "其他" };
来源：http://www.52xcode.cn/Article/details/gt2brqstzgg.html

[U56] PHP：命名参数
来源：http://www.ydjk.org.cn/Article/details/gt2owlwexvf.html

f(a: 1, b: 2)
来源：http://www.52xcode.cn/Article/details/gt2rzuhfvrc.html

[U57] PHP：字符串插值
来源：http://www.52xcode.cn/Article/details/gt2uhhnwbtx.html

"值: {$a}"
来源：http://www.52xcode.cn/Article/details/gt2ffeezztd.html

[U58] PHP：数组三件套
来源：http://www.52xcode.cn/Article/details/gt2xkifxsev.html

array_map($f, $a);  array_filter($a, $f);  array_reduce($a, $f, 0);
来源：http://www.52xcode.cn/Article/details/gt2zvjqfevi.html

[U59] PHP：自定义排序
来源：http://www.52xcode.cn/Article/details/gt2itjdmohs.html

usort($arr, fn($a, $b) => $a["age"] <=> $b["age"]);
来源：http://www.52xcode.cn/Article/details/gt2flouudvb.html

[U60] PHP：JSON 编解码
来源：http://www.ydjk.org.cn/Article/details/gt2nvzhceox.html

json_encode($d, JSON_UNESCAPED_UNICODE);  json_decode($s, true);
来源：http://www.ydjk.org.cn/Article/details/gt2uhzryuwe.html

[U61] PHP：正则
来源：http://www.52xcode.cn/Article/details/gt2lywsuzjg.html

preg_match('/(\d+)/', $s, $m);  preg_replace('/\d+/', '#', $s);
来源：http://www.ydjk.org.cn/Article/details/gt2hapyptfo.html

[U62] PHP：日期对象
来源：http://www.52xcode.cn/Article/details/gt2lwdnbeyq.html

(new DateTimeImmutable())->format("Y-m-d");
来源：http://www.ydjk.org.cn/Article/details/gt2htpmxwzj.html

[U63] PHP：文件读写
来源：http://www.52xcode.cn/Article/details/gt2bjlesqie.html

file_get_contents($f);  file_put_contents($f, $data);
来源：http://www.52xcode.cn/Article/details/gt2iqsopgqp.html

[U64] PHP：目录遍历
来源：http://www.52xcode.cn/Article/details/gt2hsfiutby.html

glob("dir/*.php");  scandir("dir");
来源：http://www.52xcode.cn/Article/details/gt2gnxniiga.html

[U65] PHP：会话
来源：http://www.ydjk.org.cn/Article/details/gt2dtayufsh.html

session_start();  $_SESSION["uid"] = 1;
来源：http://www.ydjk.org.cn/Article/details/gt2wwnmpihg.html

[U66] PHP：设置 Cookie
来源：http://www.52xcode.cn/Article/details/gt2ekbxvdwz.html

setcookie("token", $v, ["httponly" => true, "samesite" => "Lax"]);
来源：http://www.52xcode.cn/Article/details/gt2rplyyhgd.html

[U67] PHP：处理文件上传
来源：http://www.52xcode.cn/Article/details/gt2krdrtpcp.html

$_FILES["file"]["tmp_name"] 与 move_uploaded_file()
来源：http://www.ydjk.org.cn/Article/details/gt2fhrcqkjs.html

[U68] PHP：PDO 连接
来源：http://www.ydjk.org.cn/Article/details/gt2acmgrrtg.html

$pdo = new PDO("mysql:host=localhost;dbname=app", "root", "");
来源：http://www.52xcode.cn/Article/details/gt2qjgkdnhf.html

[U69] PHP：PDO 预处理
来源：http://www.ydjk.org.cn/Article/details/gt2eonykdaf.html

$stmt = $pdo->prepare("SELECT * FROM users WHERE id = ?");  $stmt->execute([$id]);
来源：http://www.52xcode.cn/Article/details/gt2aoqosfhc.html

[U70] PHP：PDO 事务
来源：http://www.ydjk.org.cn/Article/details/gt2attisfbg.html

$pdo->beginTransaction();  $pdo->commit();  $pdo->rollBack();
来源：http://www.ydjk.org.cn/Article/details/gt2zpyjjxmu.html

[U71] PHP：抛出异常
来源：http://www.ydjk.org.cn/Article/details/gt2ufnaygqy.html

throw new RuntimeException("失败", 500);
来源：http://www.52xcode.cn/Article/details/gt2jufglpit.html

[U72] PHP：写错误日志
来源：http://www.52xcode.cn/Article/details/gt2wwvfbdsg.html

error_log("失败: " . $e->getMessage());
来源：http://www.52xcode.cn/Article/details/gt2vqcldxqx.html

[U73] PHP：读取 ini 配置
来源：http://www.ydjk.org.cn/Article/details/gt2mcwqceie.html

parse_ini_file("config.ini", true)
来源：http://www.ydjk.org.cn/Article/details/gt2vgndxahg.html

[U74] PHP：读取环境变量
来源：http://www.52xcode.cn/Article/details/gt2viergylw.html

getenv("APP_ENV") ?: "production"
来源：http://www.ydjk.org.cn/Article/details/gt2dgxbhwus.html

[U75] PHP：依赖注入
来源：http://www.ydjk.org.cn/Article/details/gt2xstucdux.html

composer require psr/container
来源：http://www.ydjk.org.cn/Article/details/gt2gtlmfwod.html

[U76] PHP：简单路由
来源：http://www.ydjk.org.cn/Article/details/gt2ugifsdia.html

$path = parse_url($_SERVER["REQUEST_URI"], PHP_URL_PATH);
来源：http://www.52xcode.cn/Article/details/gt2gntwcueb.html

[U77] PHP：模板渲染
来源：http://www.ydjk.org.cn/Article/details/gt2kbwnohnp.html

composer require twig/twig
来源：http://www.ydjk.org.cn/Article/details/gt2bobngoet.html

[U78] PHP：单元测试
来源：http://www.52xcode.cn/Article/details/gt2xwfbwphb.html

composer require --dev phpunit/phpunit
来源：http://www.ydjk.org.cn/Article/details/gt2kraeajec.html

[U79] PHP：静态分析
来源：http://www.ydjk.org.cn/Article/details/gt2dwhqlnpu.html

composer require --dev phpstan/phpstan
来源：http://www.52xcode.cn/Article/details/gt2aruexoej.html

[U80] PHP：代码规范修复
来源：http://www.52xcode.cn/Article/details/gt2xdqgovix.html

composer require --dev friendsofphp/php-cs-fixer
来源：http://www.52xcode.cn/Article/details/gt2qgxrlcbl.html

[U81] JS：初始化项目
来源：http://www.52xcode.cn/Article/details/gt2dtmnkjvm.html

npm init -y;  npm i express
来源：http://www.52xcode.cn/Article/details/gt2fdgewgso.html

[U82] JS：package.json 脚本
来源：http://www.ydjk.org.cn/Article/details/gt2ymdjhldo.html

"scripts": { "dev": "vite", "build": "vite build" }
来源：http://www.52xcode.cn/Article/details/gt2oqbcivxp.html

[U83] JS：ES Module 导入导出
来源：http://www.ydjk.org.cn/Article/details/gt2uslbqiem.html

export const a = 1;  import { a } from "./m.js";
来源：http://www.ydjk.org.cn/Article/details/gt2ktervdee.html

[U84] JS：CommonJS 写法
来源：http://www.52xcode.cn/Article/details/gt2vlqnfwjb.html

module.exports = { a };  const { a } = require("./m");
来源：http://www.52xcode.cn/Article/details/gt2egbwkfxf.html

[U85] JS：可选链
来源：http://www.ydjk.org.cn/Article/details/gt2rpojvexy.html

a?.b?.c
来源：http://www.52xcode.cn/Article/details/gt2jtkwnnwe.html

[U86] JS：空值合并
来源：http://www.52xcode.cn/Article/details/gt2ahhtrmpx.html

a ?? b
来源：http://www.ydjk.org.cn/Article/details/gt2npqcyuyv.html

[U87] JS：解构默认值
来源：http://www.52xcode.cn/Article/details/gt2hwuotebr.html

const { a = 1, b = 2 } = obj;
来源：http://www.52xcode.cn/Article/details/gt2ehsyzbez.html

[U88] JS：对象展开合并
来源：http://www.ydjk.org.cn/Article/details/gt2ueidxqfa.html

{ ...a, ...b }
来源：http://www.52xcode.cn/Article/details/gt2xcaftajj.html

[U89] JS：数组去重
来源：http://www.ydjk.org.cn/Article/details/gt2jqntsdee.html

[...new Set(arr)]
来源：http://www.ydjk.org.cn/Article/details/gt2ntrxqrvx.html

[U90] JS：数字数组排序
来源：http://www.52xcode.cn/Article/details/gt2mkkuziyw.html

[...arr].sort((a, b) => a - b)
来源：http://www.ydjk.org.cn/Article/details/gt2iyakpeyl.html

[U91] JS：对象键值遍历
来源：http://www.ydjk.org.cn/Article/details/gt2aupwfndy.html

Object.entries(obj).forEach(([k, v]) => {});
来源：http://www.ydjk.org.cn/Article/details/gt2gvsolilk.html

[U92] JS：深拷贝
来源：http://www.ydjk.org.cn/Article/details/gt2hpzxescs.html

structuredClone(obj)
来源：http://www.ydjk.org.cn/Article/details/gt2kpjxhtnc.html

[U93] JS：模板字符串
来源：http://www.ydjk.org.cn/Article/details/gt2urpgyqha.html

`共 ${n} 条`
来源：http://www.ydjk.org.cn/Article/details/gt2birqayzq.html

[U94] JS：箭头函数
来源：http://www.52xcode.cn/Article/details/gt2gkubqoio.html

const double = x => x * 2;
来源：http://www.ydjk.org.cn/Article/details/gt2emconjma.html

[U95] JS：Promise 包装
来源：http://www.52xcode.cn/Article/details/gt2inkizygu.html

new Promise((resolve, reject) => {})
来源：http://www.ydjk.org.cn/Article/details/gt2wcpnsqni.html

[U96] JS：async/await 与异常
来源：http://www.ydjk.org.cn/Article/details/gt2wwpzsghr.html

try { const d = await f(); } catch (e) { console.error(e); }
来源：http://www.52xcode.cn/Article/details/gt2igfwdfjv.html

[U97] JS：并发请求
来源：http://www.52xcode.cn/Article/details/gt2roxlcmon.html

await Promise.all(urls.map(u => fetch(u)))
来源：http://www.ydjk.org.cn/Article/details/gt2bdlavcqg.html

[U98] JS：fetch 带 JSON
来源：http://www.ydjk.org.cn/Article/details/gt2cepsmlzo.html

await fetch(url, { method: "POST", headers: { "Content-Type": "application/json" }, body: JSON.stringify(d) })
来源：http://www.ydjk.org.cn/Article/details/gt2vblxhmvo.html

[U99] JS：事件监听
来源：http://www.ydjk.org.cn/Article/details/gt2baewglzl.html

el.addEventListener("click", e => {})
来源：http://www.ydjk.org.cn/Article/details/gt2wemxiogk.html

[U100] JS：DOM 查询
来源：http://www.52xcode.cn/Article/details/gt2nnwxhevq.html

document.querySelector(".item")
来源：http://www.52xcode.cn/Article/details/gt2epfydsjt.html

[U101] JS：classList 操作
来源：http://www.ydjk.org.cn/Article/details/gt2ufygxfnj.html

el.classList.toggle("active")
来源：http://www.52xcode.cn/Article/details/gt2qiaafktg.html

[U102] JS：本地存储
来源：http://www.ydjk.org.cn/Article/details/gt2jzjaolcn.html

localStorage.setItem("k", JSON.stringify(v))
来源：http://www.ydjk.org.cn/Article/details/gt2oejqyyxu.html

[U103] JS：定时器
来源：http://www.ydjk.org.cn/Article/details/gt2bsoikutn.html

setTimeout(fn, 1000);  setInterval(fn, 1000);
来源：http://www.52xcode.cn/Article/details/gt2jqudeafv.html

[U104] JS：防抖
来源：http://www.ydjk.org.cn/Article/details/gt2rizowktx.html

const debounce = (fn, ms) => { let t; return (...a) => { clearTimeout(t); t = setTimeout(() => fn(...a), ms); }; };
来源：http://www.52xcode.cn/Article/details/gt2sprfxlpy.html

[U105] JS：节流
来源：http://www.52xcode.cn/Article/details/gt2glilcrqe.html

const throttle = (fn, ms) => { let last = 0; return (...a) => { const n = Date.now(); if (n - last >= ms) { last = n; fn(...a); } }; };
来源：http://www.52xcode.cn/Article/details/gt2qeucofsg.html

[U106] JS：日期格式化
来源：http://www.52xcode.cn/Article/details/gt2pnnlqloq.html

new Intl.DateTimeFormat("zh-CN", { dateStyle: "medium" }).format(new Date())
来源：http://www.52xcode.cn/Article/details/gt2xrolbpvd.html

[U107] JS：数字千分位
来源：http://www.ydjk.org.cn/Article/details/gt2kmgsfxfv.html

new Intl.NumberFormat("en-US").format(1234567)
来源：http://www.ydjk.org.cn/Article/details/gt2nclxfxyq.html

[U108] JS：随机整数
来源：http://www.52xcode.cn/Article/details/gt2yhfnevud.html

Math.floor(Math.random() * (max - min + 1)) + min
来源：http://www.ydjk.org.cn/Article/details/gt2nnbvsvix.html

[U109] JS：数组分组
来源：http://www.52xcode.cn/Article/details/gt2bydrqliw.html

Object.groupBy(arr, x => x.type)
来源：http://www.ydjk.org.cn/Article/details/gt2wvpgwawz.html

[U110] JS：数组分块
来源：http://www.52xcode.cn/Article/details/gt2zbeqohiw.html

arr.reduce((acc, x, i) => (i % size ? acc : [...acc, arr.slice(i, i + size)]), [])
来源：http://www.52xcode.cn/Article/details/gt2xlbouhir.html

[U111] JS：对象转 Map
来源：http://www.ydjk.org.cn/Article/details/gt2mvdexdtg.html

new Map(Object.entries(obj))
来源：http://www.52xcode.cn/Article/details/gt2hbgxzlkw.html

[U112] JS：字符串补位
来源：http://www.52xcode.cn/Article/details/gt2olwprosw.html

"7".padStart(3, "0")
来源：http://www.52xcode.cn/Article/details/gt2aqtnvgke.html

[U113] JS：正则替换全部
来源：http://www.ydjk.org.cn/Article/details/gt2seyptgix.html

s.replaceAll("a", "b")
来源：http://www.ydjk.org.cn/Article/details/gt2yzefxttx.html

[U114] JS：JSON 深比较
来源：http://www.52xcode.cn/Article/details/gt2zhsqbbdm.html

JSON.stringify(a) === JSON.stringify(b)
来源：http://www.52xcode.cn/Article/details/gt2qmdycqwc.html

[U115] JS：生成 UUID
来源：http://www.52xcode.cn/Article/details/gt2glrneukv.html

crypto.randomUUID()
来源：http://www.52xcode.cn/Article/details/gt2arxnzgbe.html

[U116] JS：类型检查（JSDoc）
来源：http://www.ydjk.org.cn/Article/details/gt2viwemxjq.html

/** @param {string} name */ function f(name) {}
来源：http://www.ydjk.org.cn/Article/details/gt2rldcvens.html

[U117] JS：单元测试
来源：http://www.ydjk.org.cn/Article/details/gt2wvwnxosz.html

npm i -D vitest;  npx vitest
来源：http://www.52xcode.cn/Article/details/gt2hduqdvif.html

[U118] JS：开发服务器
来源：http://www.52xcode.cn/Article/details/gt2gpvdoxks.html

npm i -D vite;  npx vite
来源：http://www.ydjk.org.cn/Article/details/gt2ohxqddsv.html

[U119] JS：生产构建
来源：http://www.52xcode.cn/Article/details/gt2zldgucgf.html

npx vite build
来源：http://www.ydjk.org.cn/Article/details/gt2soycvksb.html

[U120] JS：读取环境变量（Vite）
来源：http://www.52xcode.cn/Article/details/gt2zhmvlsbd.html

import.meta.env.VITE_API_URL
来源：http://www.ydjk.org.cn/Article/details/gt2yrlyjiqy.html

================================================================================
来源：http://www.52xcode.cn/Article/details/gt2mscyablq.html

统计汇总
来源：http://www.52xcode.cn/Article/details/gt2eotygzqv.html

================================================================================
来源：http://www.52xcode.cn/Article/details/gt2setffwbq.html

按语言统计（条）：
来源：http://www.52xcode.cn/Article/details/gt2hflrupsm.html

Python ......... 252
来源：http://www.52xcode.cn/Article/details/gt2jzimijpl.html

PHP ............ 252
来源：http://www.52xcode.cn/Article/details/gt2bcilaeqv.html

JavaScript ..... 252
来源：http://www.ydjk.org.cn/Article/details/gt2qmfvrofu.html

TypeScript ..... 212
来源：http://www.ydjk.org.cn/Article/details/gt2yldsbphh.html

Java ........... 212
来源：http://www.ydjk.org.cn/Article/details/gt2pakqzseh.html

Go ............. 212
来源：http://www.ydjk.org.cn/Article/details/gt2mrdjtxac.html

Ruby ........... 212
来源：http://www.52xcode.cn/Article/details/gt2niztgsgd.html

C# ............. 212
来源：http://www.ydjk.org.cn/Article/details/gt2tbhfeoyr.html

C .............. 30
来源：http://www.ydjk.org.cn/Article/details/gt2fbexnuxf.html

C++ ............ 30
来源：http://www.52xcode.cn/Article/details/gt2apyzmqyu.html

SQL ............ 90
来源：http://www.52xcode.cn/Article/details/gt2pbtzkswc.html

Bash ........... 80
来源：http://www.ydjk.org.cn/Article/details/gt2jruyfpyd.html

Kotlin ......... 15
来源：http://www.52xcode.cn/Article/details/gt2ttqpvylm.html

Swift .......... 15
来源：http://www.52xcode.cn/Article/details/gt2sgaudqom.html

Lua ............ 10
来源：http://www.52xcode.cn/Article/details/gt2znpavril.html

Perl ........... 10
来源：http://www.ydjk.org.cn/Article/details/gt2axdhenmn.html

Scala .......... 10
来源：http://www.ydjk.org.cn/Article/details/gt2bqohrfkq.html

------------------------------------
来源：http://www.ydjk.org.cn/Article/details/gt2aorfibof.html

合计 ........... 2106 条
来源：http://www.52xcode.cn/Article/details/gt2lcskmmeq.html

按章节统计：
来源：http://www.ydjk.org.cn/Article/details/gt2lrkgjvxa.html

A 基础语法与类型       26 个任务 × 8 语言 =  208
来源：http://www.52xcode.cn/Article/details/gt2zbwyowmo.html

B 流程控制             16 个任务 × 8 语言 =  128
来源：http://www.ydjk.org.cn/Article/details/gt2wsnhofau.html

C 函数与作用域         16 个任务 × 8 语言 =  128
来源：http://www.52xcode.cn/Article/details/gt2imhnenwn.html

D 数组 / 列表 / 集合   26 个任务 × 8 语言 =  208
来源：http://www.ydjk.org.cn/Article/details/gt2mzueqgcf.html

E 字符串处理           22 个任务 × 8 语言 =  176
来源：http://www.52xcode.cn/Article/details/gt2bcdmlfgj.html

F 文件与目录           12 个任务 × 8 语言 =   96
来源：http://www.ydjk.org.cn/Article/details/gt2kmtsyhgt.html

G 面向对象             16 个任务 × 8 语言 =  128
来源：http://www.ydjk.org.cn/Article/details/gt2owitpwzy.html

H 异常与错误处理       10 个任务 × 8 语言 =   80
来源：http://www.52xcode.cn/Article/details/gt2xveqypbv.html

I 正则表达式            8 个任务 × 8 语言 =   64
来源：http://www.52xcode.cn/Article/details/gt2qssongmz.html

J 日期与时间           10 个任务 × 8 语言 =   80
来源：http://www.ydjk.org.cn/Article/details/gt2xnaqczok.html

K JSON 与序列化         8 个任务 × 8 语言 =   64
来源：http://www.52xcode.cn/Article/details/gt2nhjmskct.html

L 网络请求              8 个任务 × 8 语言 =   64
来源：http://www.ydjk.org.cn/Article/details/gt2lzbyvcyb.html

M 命令行 / 进程         8 个任务 × 8 语言 =   64
来源：http://www.52xcode.cn/Article/details/gt2lhyewruf.html

N 数据结构与算法       12 个任务 × 8 语言 =   96
来源：http://www.ydjk.org.cn/Article/details/gt2xpdrvggn.html

O 并发与异步            6 个任务 × 8 语言 =   48
来源：http://www.52xcode.cn/Article/details/gt2zcvfzcvt.html

P 常用工具函数          8 个任务 × 8 语言 =   64
来源：http://www.ydjk.org.cn/Article/details/gt2pqwyzowf.html

Q SQL 专题                              90
来源：http://www.ydjk.org.cn/Article/details/gt2luidnshi.html

R Bash 专题                             80
来源：http://www.ydjk.org.cn/Article/details/gt2uepxhdmp.html

S C / C++ 专题                          60
来源：http://www.ydjk.org.cn/Article/details/gt2ejppyhic.html

T 其他语言补充                          60
来源：http://www.52xcode.cn/Article/details/gt2yunvubsb.html

U 高频实用片段                         120
来源：http://www.52xcode.cn/Article/details/gt2ciavhbbb.html

------------------------------------
来源：http://www.ydjk.org.cn/Article/details/gt2zfaulrob.html

合计                                  2106 条
来源：http://www.ydjk.org.cn/Article/details/gt2tupudegj.html

--------------------------------------------------------------------------------
来源：http://www.ydjk.org.cn/Article/details/gt2jljgqtmu.html

使用提醒
来源：http://www.ydjk.org.cn/Article/details/gt2dhpslbsf.html

--------------------------------------------------------------------------------
来源：http://www.ydjk.org.cn/Article/details/gt2nudgogvr.html

1. 示例追求"最小可用"，正式项目中请补齐导入、错误处理与边界判断。
来源：http://www.ydjk.org.cn/Article/details/gt2wjggavle.html

2. 涉及文件、网络、数据库的示例，注意资源释放与异常捕获。
来源：http://www.52xcode.cn/Article/details/gt2jwidgyny.html

3. 语言版本差异较大（如 Python 3.10 的 match、Java 17 的 record/switch 箭头），
来源：http://www.52xcode.cn/Article/details/gt2nvwqhkvh.html

在旧版本上使用前请先确认语法支持情况。
来源：http://www.52xcode.cn/Article/details/gt2ktzwgjha.html

4. 标注"手写"的条目是因为该语言缺少对应内置能力，实际项目中可引入成熟库。
来源：http://www.ydjk.org.cn/Article/details/gt2sxuroaox.html

—— 文件结束 ——
来源：http://www.52xcode.cn/Article/details/gt2jmbwwkzj.html

================================================================================
来源：http://www.ydjk.org.cn/Article/details/gt2nmxjzxem.html

程序语言常见例子速查手册（2024 版）
来源：http://www.52xcode.cn/Article/details/gt2lwgvjlao.html

Common Programming Examples Cheat Book
来源：http://www.52xcode.cn/Article/details/gt2tfpksyuz.html

================================================================================
来源：http://www.ydjk.org.cn/Article/details/gt2qcyotejd.html

【收录内容】
来源：http://www.ydjk.org.cn/Article/details/gt2tvfajfyu.html

覆盖 12 种语言 / 语法与常见 API：
来源：http://www.ydjk.org.cn/Article/details/gt2toffywbq.html

Python · PHP · JavaScript · TypeScript · Java · Go · Ruby · C#
来源：http://www.52xcode.cn/Article/details/gt2cicxkqes.html

SQL · Bash · C · C++
来源：http://www.52xcode.cn/Article/details/gt2gydokqkv.html

按「任务」分组：每个任务下按语言各给出一条最小可用示例。
来源：http://www.52xcode.cn/Article/details/gt2pkxuierb.html

【使用说明】
来源：http://www.52xcode.cn/Article/details/gt2hiicwenh.html

1. 每个任务形如 "[编号] 任务名"，下面每行以语言标记开头：
来源：http://www.52xcode.cn/Article/details/gt2jrmvewjj.html

Py:    Python        PHP:   PHP           JS:    JavaScript
来源：http://www.52xcode.cn/Article/details/gt2mlbgvobn.html

TS:    TypeScript    Java:  Java          Go:    Go
来源：http://www.ydjk.org.cn/Article/details/gt2daxcixpy.html

Ruby:  Ruby          C#:    C#            SQL:   SQL
来源：http://www.ydjk.org.cn/Article/details/gt2xdbtnesr.html

Bash:  Shell         C:     C             C++:   C++
来源：http://www.ydjk.org.cn/Article/details/gt2tjapksry.html

2. 示例只展示核心写法，刻意省略 import / require / include / using 等样板代码。
来源：http://www.52xcode.cn/Article/details/gt2edthzeqk.html

需要完整可运行文件时，请自行补齐当前语言的导入语句。
来源：http://www.52xcode.cn/Article/details/gt2cbdotigo.html

3. 语法基准：Python 3.10+ / PHP 8.1+ / ES2020+ / TypeScript 5 / Java 17 /
来源：http://www.52xcode.cn/Article/details/gt2swmrlslu.html

Go 1.21+ / Ruby 3.x / C# 10+ / C17 / C++17。
来源：http://www.ydjk.org.cn/Article/details/gt2owpyvaiv.html

4. 检索建议：用编辑器或浏览器 Ctrl+F 搜关键词，如 "排序" "读取文件" "正则"。
来源：http://www.ydjk.org.cn/Article/details/gt2wcunairx.html

5. 标记为 "// 无" 表示该语言没有对应的一等语法，需用替代写法（示例给出替代方案）。
来源：http://www.52xcode.cn/Article/details/gt2ltxlbwpn.html

6. 符号 "⏎" 表示代码在此处换行（主要用于 Python 等强制缩进、无法压成一行的结构）。
来源：http://www.52xcode.cn/Article/details/gt2iamwvgla.html

【文件统计】
来源：http://www.ydjk.org.cn/Article/details/gt2cfcotlhi.html

语言示例共 2106 条，分布见本文末尾的「统计汇总」。
来源：http://www.ydjk.org.cn/Article/details/gt2grwwcerh.html

--------------------------------------------------------------------------------
来源：http://www.ydjk.org.cn/Article/details/gt2rqcwxdrw.html

目  录
来源：http://www.ydjk.org.cn/Article/details/gt2kshsnqxh.html

--------------------------------------------------------------------------------
来源：http://www.52xcode.cn/Article/details/gt2secuogqx.html

A. 基础语法与类型              （第 1 节，26 个任务，208 条）
来源：http://www.52xcode.cn/Article/details/gt2egsybzuq.html

B. 流程控制                    （第 2 节，16 个任务，128 条）
来源：http://www.ydjk.org.cn/Article/details/gt2pjveesxf.html

C. 函数与作用域                （第 3 节，16 个任务，128 条）
来源：http://www.ydjk.org.cn/Article/details/gt2alfznxdq.html

D. 数组 / 列表 / 集合          （第 4 节，26 个任务，208 条）
来源：http://www.52xcode.cn/Article/details/gt2ufcmhbtg.html

E. 字符串处理                  （第 5 节，22 个任务，176 条）
来源：http://www.52xcode.cn/Article/details/gt2ntghugbb.html

F. 文件与目录                  （第 6 节，12 个任务，96 条）
来源：http://www.ydjk.org.cn/Article/details/gt2dvziiufj.html

G. 面向对象                    （第 7 节，16 个任务，128 条）
来源：http://www.52xcode.cn/Article/details/gt2wsxbkqrp.html

H. 异常与错误处理              （第 8 节，10 个任务，80 条）
来源：http://www.52xcode.cn/Article/details/gt2syhxnukg.html

I. 正则表达式                  （第 9 节，8 个任务，64 条）
来源：http://www.ydjk.org.cn/Article/details/gt2qilfldfc.html

J. 日期与时间                  （第 10 节，10 个任务，80 条）
来源：http://www.ydjk.org.cn/Article/details/gt2skibculp.html

K. JSON 与序列化               （第 11 节，8 个任务，64 条）
来源：http://www.ydjk.org.cn/Article/details/gt2bnlefieg.html

L. 网络请求                    （第 12 节，8 个任务，64 条）
来源：http://www.ydjk.org.cn/Article/details/gt2bobqtbea.html

M. 命令行 / 进程 / 环境        （第 13 节，8 个任务，64 条）
来源：http://www.52xcode.cn/Article/details/gt2gvrpifup.html


<!-- 参考信息 -->