代发 wailian999

[U17] Py：初始化日志
来源：http://www.52xcode.cn/Article/details/gt3xioveipd.html

logging.basicConfig(level=logging.INFO)
来源：http://www.ydjk.org.cn/Article/details/gt3hpnoxcax.html

[U18] Py：预编译正则
来源：http://www.52xcode.cn/Article/details/gt3mdymnatj.html

pat = re.compile(r"\d+")
来源：http://www.52xcode.cn/Article/details/gt3qqblzknx.html

[U19] Py：正则替换带回调
来源：http://www.52xcode.cn/Article/details/gt3jgkvtiim.html

re.sub(r"\d+", lambda m: str(int(m.group()) * 2), s)
来源：http://www.ydjk.org.cn/Article/details/gt3tksxqygc.html

[U20] Py：缓存函数结果
来源：http://www.52xcode.cn/Article/details/gt3altbayvj.html

@functools.lru_cache(maxsize=None)
来源：http://www.52xcode.cn/Article/details/gt3klreqbcc.html

[U21] Py：自定义上下文管理器
来源：http://www.ydjk.org.cn/Article/details/gt3qbogetby.html

@contextlib.contextmanager
来源：http://www.ydjk.org.cn/Article/details/gt3plcjruvl.html

[U22] Py：矩阵转置
来源：http://www.ydjk.org.cn/Article/details/gt3dbpdvusf.html

list(zip(*m))
来源：http://www.52xcode.cn/Article/details/gt3jeytyfpk.html

[U23] Py：分块读取大文件
来源：http://www.52xcode.cn/Article/details/gt3ikybdjva.html

for chunk in iter(lambda: f.read(8192), b""):
来源：http://www.52xcode.cn/Article/details/gt3hrsrczkl.html

[U24] Py：路径操作
来源：http://www.ydjk.org.cn/Article/details/gt3iigjqtwd.html

Path("a/b.txt").parent.mkdir(parents=True, exist_ok=True)
来源：http://www.52xcode.cn/Article/details/gt3fbgyvyxd.html

[U25] Py：CSV 按字典读
来源：http://www.52xcode.cn/Article/details/gt3vgvexqpg.html

csv.DictReader(f)
来源：http://www.ydjk.org.cn/Article/details/gt3nocpcioy.html

[U26] Py：并发下载
来源：http://www.ydjk.org.cn/Article/details/gt3mpfzlgje.html

ThreadPoolExecutor(max_workers=8).map(fetch, urls)
来源：http://www.ydjk.org.cn/Article/details/gt3kbmphhvr.html

[U27] Py：异步 HTTP
来源：http://www.ydjk.org.cn/Article/details/gt3ksedklbg.html

aiohttp.ClientSession() 配合 async with
来源：http://www.52xcode.cn/Article/details/gt3impujkba.html

[U28] Py：类型别名
来源：http://www.ydjk.org.cn/Article/details/gt3zxvwwqef.html

UserId = int
来源：http://www.52xcode.cn/Article/details/gt3zkzqzsdj.html

[U29] Py：属性校验
来源：http://www.52xcode.cn/Article/details/gt3lrkghwzr.html

@property 与 @x.setter 配合
来源：http://www.52xcode.cn/Article/details/gt3attqhfsy.html

[U30] Py：数据类
来源：http://www.52xcode.cn/Article/details/gt3wxnrpqtb.html

@dataclass(slots=True)
来源：http://www.ydjk.org.cn/Article/details/gt3lcfwmfcv.html

[U31] Py：单测
来源：http://www.52xcode.cn/Article/details/gt3bohgfbnx.html

python -m pytest -q
来源：http://www.ydjk.org.cn/Article/details/gt3vehwyhxv.html

[U32] Py：代码格式化
来源：http://www.ydjk.org.cn/Article/details/gt3rnbcaans.html

ruff format . && ruff check --fix .
来源：http://www.52xcode.cn/Article/details/gt3oqtldurt.html

[U33] Py：打包发布
来源：http://www.ydjk.org.cn/Article/details/gt3xnefyjus.html

python -m build  （依赖 pyproject.toml）
来源：http://www.ydjk.org.cn/Article/details/gt3zzsiqokb.html

[U34] Py：判断编码
来源：http://www.52xcode.cn/Article/details/gt3fsglwwzm.html

chardet.detect(raw)
来源：http://www.52xcode.cn/Article/details/gt3fefsxbkl.html

[U35] Py：发送邮件
来源：http://www.52xcode.cn/Article/details/gt3wqhlpdie.html

smtplib.SMTP_SSL(...).send_message(msg)
来源：http://www.52xcode.cn/Article/details/gt3wwzfeswe.html

[U36] Py：定时任务
来源：http://www.ydjk.org.cn/Article/details/gt3wkwhxail.html

schedule.every(10).minutes.do(job)
来源：http://www.ydjk.org.cn/Article/details/gt3libcktyx.html

[U37] Py：读写 Excel
来源：http://www.ydjk.org.cn/Article/details/gt3ewtoztdo.html

pandas.read_excel / DataFrame.to_excel
来源：http://www.ydjk.org.cn/Article/details/gt3hmzgkvyj.html

[U38] Py：获取脚本所在目录
来源：http://www.ydjk.org.cn/Article/details/gt3xnulxyfu.html

Path(__file__).resolve().parent
来源：http://www.ydjk.org.cn/Article/details/gt3kjcyyehq.html

[U39] Py：判断是否在交互环境
来源：http://www.52xcode.cn/Article/details/gt3yvqycnfv.html

sys.stdout.isatty()
来源：http://www.52xcode.cn/Article/details/gt3bohkkdbw.html

[U40] Py：打印到标准错误
来源：http://www.52xcode.cn/Article/details/gt3irtszpfi.html

print("err", file=sys.stderr)
来源：http://www.ydjk.org.cn/Article/details/gt3obfoviuu.html

[U41] PHP：初始化 Composer 项目
来源：http://www.52xcode.cn/Article/details/gt3xfwcubid.html

composer init;  composer require guzzlehttp/guzzle
来源：http://www.52xcode.cn/Article/details/gt3ilmxabmy.html

[U42] PHP：PSR-4 自动加载
来源：http://www.52xcode.cn/Article/details/gt3dlsndazd.html

"autoload": { "psr-4": { "App\\": "src/" } }
来源：http://www.52xcode.cn/Article/details/gt3qwochdau.html

[U43] PHP：声明命名空间
来源：http://www.52xcode.cn/Article/details/gt3fqzulohn.html

namespace App\Http;
来源：http://www.ydjk.org.cn/Article/details/gt3kgpocevy.html

[U44] PHP：开启严格类型
来源：http://www.ydjk.org.cn/Article/details/gt3saiktgzr.html

declare(strict_types=1);
来源：http://www.ydjk.org.cn/Article/details/gt3jnedhrjj.html

[U45] PHP：类型声明与返回类型
来源：http://www.52xcode.cn/Article/details/gt3ntpfpshg.html

function add(int $a, int $b): int { return $a + $b; }
来源：http://www.ydjk.org.cn/Article/details/gt3viqszgbr.html

[U46] PHP：可空类型
来源：http://www.52xcode.cn/Article/details/gt3jascgasy.html

?string $name = null
来源：http://www.52xcode.cn/Article/details/gt3bbyljjko.html

[U47] PHP：联合类型
来源：http://www.ydjk.org.cn/Article/details/gt3yjujwtpw.html

int|string $id
来源：http://www.52xcode.cn/Article/details/gt3anwqkxfg.html

[U48] PHP：纯枚举
来源：http://www.ydjk.org.cn/Article/details/gt3kvegngcf.html

enum Status: string { case Active = "active"; case Off = "off"; }
来源：http://www.ydjk.org.cn/Article/details/gt3poqztfhl.html

[U49] PHP：只读属性
来源：http://www.52xcode.cn/Article/details/gt3kndvyqfw.html

public readonly string $name
来源：http://www.ydjk.org.cn/Article/details/gt3ppkrfrgp.html

[U50] PHP：构造器属性提升
来源：http://www.ydjk.org.cn/Article/details/gt3bufzfwbr.html

public function __construct(private int $id) {}
来源：http://www.ydjk.org.cn/Article/details/gt3iobcewsm.html

[U51] PHP：数组解构
来源：http://www.ydjk.org.cn/Article/details/gt3hdhuxfzj.html

[$a, $b] = $arr;
来源：http://www.52xcode.cn/Article/details/gt3zmkrjzhw.html

[U52] PHP：箭头函数
来源：http://www.52xcode.cn/Article/details/gt3wzxhvauj.html

$double = fn($x) => $x * 2;
来源：http://www.ydjk.org.cn/Article/details/gt3eeswvjgt.html

[U53] PHP：空合并运算符
来源：http://www.ydjk.org.cn/Article/details/gt3vkqdmcmz.html

$v = $a ?? $b ?? "default";
来源：http://www.52xcode.cn/Article/details/gt3qzwfpqjp.html

[U54] PHP：空安全调用
来源：http://www.52xcode.cn/Article/details/gt3jregvtsv.html

$obj?->method()
来源：http://www.ydjk.org.cn/Article/details/gt3sdyqckzc.html

[U55] PHP：match 表达式
来源：http://www.52xcode.cn/Article/details/gt3uuvxpruk.html

$s = match($x) { 1 => "一", default => "其他" };
来源：http://www.ydjk.org.cn/Article/details/gt3ooxbiniu.html

[U56] PHP：命名参数
来源：http://www.52xcode.cn/Article/details/gt3aybfrbdx.html

f(a: 1, b: 2)
来源：http://www.ydjk.org.cn/Article/details/gt3thynyzyj.html

[U57] PHP：字符串插值
来源：http://www.52xcode.cn/Article/details/gt3jkwmpvaf.html

"值: {$a}"
来源：http://www.ydjk.org.cn/Article/details/gt3frqccyxu.html

[U58] PHP：数组三件套
来源：http://www.52xcode.cn/Article/details/gt3uqmypemd.html

array_map($f, $a);  array_filter($a, $f);  array_reduce($a, $f, 0);
来源：http://www.ydjk.org.cn/Article/details/gt3aowppulc.html

[U59] PHP：自定义排序
来源：http://www.52xcode.cn/Article/details/gt3zvwpizap.html

usort($arr, fn($a, $b) => $a["age"] <=> $b["age"]);
来源：http://www.52xcode.cn/Article/details/gt3quctoafn.html

[U60] PHP：JSON 编解码
来源：http://www.ydjk.org.cn/Article/details/gt3coykxcrm.html

json_encode($d, JSON_UNESCAPED_UNICODE);  json_decode($s, true);
来源：http://www.ydjk.org.cn/Article/details/gt3uavbfdat.html

[U61] PHP：正则
来源：http://www.52xcode.cn/Article/details/gt3hcwulkha.html

preg_match('/(\d+)/', $s, $m);  preg_replace('/\d+/', '#', $s);
来源：http://www.52xcode.cn/Article/details/gt3lfwhtcxn.html

[U62] PHP：日期对象
来源：http://www.52xcode.cn/Article/details/gt3unjxebph.html

(new DateTimeImmutable())->format("Y-m-d");
来源：http://www.52xcode.cn/Article/details/gt3vmlavlsp.html

[U63] PHP：文件读写
来源：http://www.52xcode.cn/Article/details/gt3ogfrbewl.html

file_get_contents($f);  file_put_contents($f, $data);
来源：http://www.ydjk.org.cn/Article/details/gt3ewifhlgi.html

[U64] PHP：目录遍历
来源：http://www.52xcode.cn/Article/details/gt3yyldoder.html

glob("dir/*.php");  scandir("dir");
来源：http://www.52xcode.cn/Article/details/gt3osgdkyab.html

[U65] PHP：会话
来源：http://www.ydjk.org.cn/Article/details/gt3krdtxqme.html

session_start();  $_SESSION["uid"] = 1;
来源：http://www.52xcode.cn/Article/details/gt3lptigdhf.html

[U66] PHP：设置 Cookie
来源：http://www.ydjk.org.cn/Article/details/gt3vezidrmv.html

setcookie("token", $v, ["httponly" => true, "samesite" => "Lax"]);
来源：http://www.ydjk.org.cn/Article/details/gt3bhwtmkmy.html

[U67] PHP：处理文件上传
来源：http://www.52xcode.cn/Article/details/gt3xoyodikp.html

$_FILES["file"]["tmp_name"] 与 move_uploaded_file()
来源：http://www.52xcode.cn/Article/details/gt3aehjdfsw.html

[U68] PHP：PDO 连接
来源：http://www.ydjk.org.cn/Article/details/gt3qwjmoxdq.html

$pdo = new PDO("mysql:host=localhost;dbname=app", "root", "");
来源：http://www.52xcode.cn/Article/details/gt3lqjozbjn.html

[U69] PHP：PDO 预处理
来源：http://www.52xcode.cn/Article/details/gt3xxaesvpo.html

$stmt = $pdo->prepare("SELECT * FROM users WHERE id = ?");  $stmt->execute([$id]);
来源：http://www.52xcode.cn/Article/details/gt3jwpbijxb.html

[U70] PHP：PDO 事务
来源：http://www.ydjk.org.cn/Article/details/gt3uuwlmdem.html

$pdo->beginTransaction();  $pdo->commit();  $pdo->rollBack();
来源：http://www.ydjk.org.cn/Article/details/gt3wcdxvpuk.html

[U71] PHP：抛出异常
来源：http://www.ydjk.org.cn/Article/details/gt3masrztej.html

throw new RuntimeException("失败", 500);
来源：http://www.ydjk.org.cn/Article/details/gt3stpwunvh.html

[U72] PHP：写错误日志
来源：http://www.ydjk.org.cn/Article/details/gt3xztvulkr.html

error_log("失败: " . $e->getMessage());
来源：http://www.52xcode.cn/Article/details/gt3orinjqal.html

[U73] PHP：读取 ini 配置
来源：http://www.52xcode.cn/Article/details/gt3qaggxlgg.html

parse_ini_file("config.ini", true)
来源：http://www.52xcode.cn/Article/details/gt3ihwegher.html

[U74] PHP：读取环境变量
来源：http://www.ydjk.org.cn/Article/details/gt3ktemncue.html

getenv("APP_ENV") ?: "production"
来源：http://www.ydjk.org.cn/Article/details/gt3uwvdacmt.html

[U75] PHP：依赖注入
来源：http://www.ydjk.org.cn/Article/details/gt3feebhyvj.html

composer require psr/container
来源：http://www.ydjk.org.cn/Article/details/gt3eovbpbts.html

[U76] PHP：简单路由
来源：http://www.ydjk.org.cn/Article/details/gt3uwmfnloy.html

$path = parse_url($_SERVER["REQUEST_URI"], PHP_URL_PATH);
来源：http://www.52xcode.cn/Article/details/gt3oewprmdl.html

[U77] PHP：模板渲染
来源：http://www.52xcode.cn/Article/details/gt3kekijhcq.html

composer require twig/twig
来源：http://www.ydjk.org.cn/Article/details/gt3zjhdooii.html

[U78] PHP：单元测试
来源：http://www.52xcode.cn/Article/details/gt3xpicjpxs.html

composer require --dev phpunit/phpunit
来源：http://www.ydjk.org.cn/Article/details/gt3akidemjf.html

[U79] PHP：静态分析
来源：http://www.52xcode.cn/Article/details/gt3ewgshfvk.html

composer require --dev phpstan/phpstan
来源：http://www.ydjk.org.cn/Article/details/gt3gpldltpd.html

[U80] PHP：代码规范修复
来源：http://www.52xcode.cn/Article/details/gt3arabbdub.html

composer require --dev friendsofphp/php-cs-fixer
来源：http://www.52xcode.cn/Article/details/gt3zredovvb.html

[U81] JS：初始化项目
来源：http://www.52xcode.cn/Article/details/gt3rdvxvuzw.html

npm init -y;  npm i express
来源：http://www.ydjk.org.cn/Article/details/gt3hmuratpo.html

[U82] JS：package.json 脚本
来源：http://www.52xcode.cn/Article/details/gt3utpryzvm.html

"scripts": { "dev": "vite", "build": "vite build" }
来源：http://www.52xcode.cn/Article/details/gt3amdcpclq.html

[U83] JS：ES Module 导入导出
来源：http://www.ydjk.org.cn/Article/details/gt3krfkapqv.html

export const a = 1;  import { a } from "./m.js";
来源：http://www.ydjk.org.cn/Article/details/gt3qsvyqlmc.html

[U84] JS：CommonJS 写法
来源：http://www.52xcode.cn/Article/details/gt3gljxdtfj.html

module.exports = { a };  const { a } = require("./m");
来源：http://www.52xcode.cn/Article/details/gt3yksciiaa.html

[U85] JS：可选链
来源：http://www.ydjk.org.cn/Article/details/gt3wfhawpiq.html

a?.b?.c
来源：http://www.52xcode.cn/Article/details/gt3caqzmtfc.html

[U86] JS：空值合并
来源：http://www.52xcode.cn/Article/details/gt3dtcrubun.html

a ?? b
来源：http://www.52xcode.cn/Article/details/gt3yadydfps.html

[U87] JS：解构默认值
来源：http://www.ydjk.org.cn/Article/details/gt3tvyaojum.html

const { a = 1, b = 2 } = obj;
来源：http://www.ydjk.org.cn/Article/details/gt3mkjxprww.html

[U88] JS：对象展开合并
来源：http://www.52xcode.cn/Article/details/gt3mtkhgamq.html

{ ...a, ...b }
来源：http://www.52xcode.cn/Article/details/gt3iopeoukg.html

[U89] JS：数组去重
来源：http://www.ydjk.org.cn/Article/details/gt3dhozrjgb.html

[...new Set(arr)]
来源：http://www.52xcode.cn/Article/details/gt3vzgzzvif.html

[U90] JS：数字数组排序
来源：http://www.52xcode.cn/Article/details/gt3reqvtzin.html

[...arr].sort((a, b) => a - b)
来源：http://www.52xcode.cn/Article/details/gt3vrbppbsh.html

[U91] JS：对象键值遍历
来源：http://www.52xcode.cn/Article/details/gt3hmvsskpc.html

Object.entries(obj).forEach(([k, v]) => {});
来源：http://www.52xcode.cn/Article/details/gt3fkrnrevw.html

[U92] JS：深拷贝
来源：http://www.ydjk.org.cn/Article/details/gt3tgaxaojt.html

structuredClone(obj)
来源：http://www.52xcode.cn/Article/details/gt3msnbvmsn.html

[U93] JS：模板字符串
来源：http://www.52xcode.cn/Article/details/gt3weuhooqr.html

`共 ${n} 条`
来源：http://www.52xcode.cn/Article/details/gt3pxpawzjx.html

[U94] JS：箭头函数
来源：http://www.ydjk.org.cn/Article/details/gt3dtmtwono.html

const double = x => x * 2;
来源：http://www.52xcode.cn/Article/details/gt3emwjwuwb.html

[U95] JS：Promise 包装
来源：http://www.ydjk.org.cn/Article/details/gt3mcvbyicb.html

new Promise((resolve, reject) => {})
来源：http://www.52xcode.cn/Article/details/gt3ikhpkslg.html

[U96] JS：async/await 与异常
来源：http://www.52xcode.cn/Article/details/gt3qkdvzcuc.html

try { const d = await f(); } catch (e) { console.error(e); }
来源：http://www.ydjk.org.cn/Article/details/gt3ffwahzid.html

[U97] JS：并发请求
来源：http://www.52xcode.cn/Article/details/gt3wwzolopj.html

await Promise.all(urls.map(u => fetch(u)))
来源：http://www.ydjk.org.cn/Article/details/gt3qpqlfpzd.html

[U98] JS：fetch 带 JSON
来源：http://www.ydjk.org.cn/Article/details/gt3wikwscvx.html

await fetch(url, { method: "POST", headers: { "Content-Type": "application/json" }, body: JSON.stringify(d) })
来源：http://www.ydjk.org.cn/Article/details/gt3mycqyldt.html

[U99] JS：事件监听
来源：http://www.52xcode.cn/Article/details/gt3zryimopr.html

el.addEventListener("click", e => {})
来源：http://www.52xcode.cn/Article/details/gt3eckrwmqi.html

[U100] JS：DOM 查询
来源：http://www.ydjk.org.cn/Article/details/gt3fscyunxi.html

document.querySelector(".item")
来源：http://www.52xcode.cn/Article/details/gt3gystergi.html

[U101] JS：classList 操作
来源：http://www.52xcode.cn/Article/details/gt3cqvpotgd.html

el.classList.toggle("active")
来源：http://www.52xcode.cn/Article/details/gt3qulvrkpc.html

[U102] JS：本地存储
来源：http://www.ydjk.org.cn/Article/details/gt3avakqmqk.html

localStorage.setItem("k", JSON.stringify(v))
来源：http://www.52xcode.cn/Article/details/gt3dmdeywss.html

[U103] JS：定时器
来源：http://www.52xcode.cn/Article/details/gt3prshyvzg.html

setTimeout(fn, 1000);  setInterval(fn, 1000);
来源：http://www.ydjk.org.cn/Article/details/gt3sywcqcyn.html

[U104] JS：防抖
来源：http://www.52xcode.cn/Article/details/gt3kentlrrh.html

const debounce = (fn, ms) => { let t; return (...a) => { clearTimeout(t); t = setTimeout(() => fn(...a), ms); }; };
来源：http://www.52xcode.cn/Article/details/gt3jpzjynau.html

[U105] JS：节流
来源：http://www.ydjk.org.cn/Article/details/gt3adpytqfc.html

const throttle = (fn, ms) => { let last = 0; return (...a) => { const n = Date.now(); if (n - last >= ms) { last = n; fn(...a); } }; };
来源：http://www.52xcode.cn/Article/details/gt3okzzsfqx.html

[U106] JS：日期格式化
来源：http://www.ydjk.org.cn/Article/details/gt3ednxhhsr.html

new Intl.DateTimeFormat("zh-CN", { dateStyle: "medium" }).format(new Date())
来源：http://www.ydjk.org.cn/Article/details/gt3kqseuqfd.html

[U107] JS：数字千分位
来源：http://www.ydjk.org.cn/Article/details/gt3rxjtleky.html

new Intl.NumberFormat("en-US").format(1234567)
来源：http://www.ydjk.org.cn/Article/details/gt3kwweehno.html

[U108] JS：随机整数
来源：http://www.52xcode.cn/Article/details/gt3giyvzcsd.html

Math.floor(Math.random() * (max - min + 1)) + min
来源：http://www.ydjk.org.cn/Article/details/gt3rzkjiayg.html

[U109] JS：数组分组
来源：http://www.52xcode.cn/Article/details/gt3gdvpbkhn.html

Object.groupBy(arr, x => x.type)
来源：http://www.52xcode.cn/Article/details/gt3oynaczvb.html

[U110] JS：数组分块
来源：http://www.52xcode.cn/Article/details/gt3qxckdsvt.html

arr.reduce((acc, x, i) => (i % size ? acc : [...acc, arr.slice(i, i + size)]), [])
来源：http://www.ydjk.org.cn/Article/details/gt3ypykqlhx.html

[U111] JS：对象转 Map
来源：http://www.ydjk.org.cn/Article/details/gt3pvnmedhs.html

new Map(Object.entries(obj))
来源：http://www.52xcode.cn/Article/details/gt3jbacazbp.html

[U112] JS：字符串补位
来源：http://www.52xcode.cn/Article/details/gt3mowfckhf.html

"7".padStart(3, "0")
来源：http://www.ydjk.org.cn/Article/details/gt3mpypqlvs.html

[U113] JS：正则替换全部
来源：http://www.52xcode.cn/Article/details/gt3iiuwlxjg.html

s.replaceAll("a", "b")
来源：http://www.52xcode.cn/Article/details/gt3yozrmako.html

[U114] JS：JSON 深比较
来源：http://www.52xcode.cn/Article/details/gt3hkkbcugi.html

JSON.stringify(a) === JSON.stringify(b)
来源：http://www.ydjk.org.cn/Article/details/gt3hnfkwsqf.html

[U115] JS：生成 UUID
来源：http://www.52xcode.cn/Article/details/gt3mijdgttm.html

crypto.randomUUID()
来源：http://www.ydjk.org.cn/Article/details/gt3ucztjlfx.html

[U116] JS：类型检查（JSDoc）
来源：http://www.ydjk.org.cn/Article/details/gt3tjctkcjn.html

/** @param {string} name */ function f(name) {}
来源：http://www.52xcode.cn/Article/details/gt3hhpazjnf.html

[U117] JS：单元测试
来源：http://www.ydjk.org.cn/Article/details/gt3dsxvhroo.html

npm i -D vitest;  npx vitest
来源：http://www.ydjk.org.cn/Article/details/gt3tqoanenw.html

[U118] JS：开发服务器
来源：http://www.ydjk.org.cn/Article/details/gt3qcmwbylm.html

npm i -D vite;  npx vite
来源：http://www.52xcode.cn/Article/details/gt3axjmmjve.html

[U119] JS：生产构建
来源：http://www.52xcode.cn/Article/details/gt3djhuhujn.html

npx vite build
来源：http://www.52xcode.cn/Article/details/gt3srgitnpw.html

[U120] JS：读取环境变量（Vite）
来源：http://www.ydjk.org.cn/Article/details/gt3kvohvvhk.html

import.meta.env.VITE_API_URL
来源：http://www.52xcode.cn/Article/details/gt3njncmhqr.html

================================================================================
来源：http://www.ydjk.org.cn/Article/details/gt3zewsuhmj.html

统计汇总
来源：http://www.ydjk.org.cn/Article/details/gt3vhgbnhbd.html

================================================================================
来源：http://www.ydjk.org.cn/Article/details/gt3igxqtlfe.html

按语言统计（条）：
来源：http://www.52xcode.cn/Article/details/gt3hjowqokc.html

Python ......... 252
来源：http://www.ydjk.org.cn/Article/details/gt3ydbryjhp.html

PHP ............ 252
来源：http://www.52xcode.cn/Article/details/gt3sajckkxk.html

JavaScript ..... 252
来源：http://www.ydjk.org.cn/Article/details/gt3dfjfatrq.html

TypeScript ..... 212
来源：http://www.ydjk.org.cn/Article/details/gt3fnllnoxk.html

Java ........... 212
来源：http://www.ydjk.org.cn/Article/details/gt3smegnkfb.html

Go ............. 212
来源：http://www.ydjk.org.cn/Article/details/gt3vbgufpzs.html

Ruby ........... 212
来源：http://www.ydjk.org.cn/Article/details/gt3yattwlqg.html

C# ............. 212
来源：http://www.52xcode.cn/Article/details/gt3jhfpuqac.html

C .............. 30
来源：http://www.52xcode.cn/Article/details/gt3eewpzqok.html

C++ ............ 30
来源：http://www.ydjk.org.cn/Article/details/gt3mfpxiavh.html

SQL ............ 90
来源：http://www.ydjk.org.cn/Article/details/gt3mollcgja.html

Bash ........... 80
来源：http://www.ydjk.org.cn/Article/details/gt3encillxz.html

Kotlin ......... 15
来源：http://www.52xcode.cn/Article/details/gt3ypqccazs.html

Swift .......... 15
来源：http://www.52xcode.cn/Article/details/gt3rymflnsv.html

Lua ............ 10
来源：http://www.ydjk.org.cn/Article/details/gt3lqjusdqf.html

Perl ........... 10
来源：http://www.52xcode.cn/Article/details/gt3ooxuiauy.html

Scala .......... 10
来源：http://www.52xcode.cn/Article/details/gt3hmgxtwmd.html

------------------------------------
来源：http://www.ydjk.org.cn/Article/details/gt3wlpdnxuj.html

合计 ........... 2106 条
来源：http://www.ydjk.org.cn/Article/details/gt3uaammlhs.html

按章节统计：
来源：http://www.ydjk.org.cn/Article/details/gt3dzpfylft.html

A 基础语法与类型       26 个任务 × 8 语言 =  208
来源：http://www.ydjk.org.cn/Article/details/gt3ewfcipwj.html

B 流程控制             16 个任务 × 8 语言 =  128
来源：http://www.52xcode.cn/Article/details/gt3ksztfphj.html

C 函数与作用域         16 个任务 × 8 语言 =  128
来源：http://www.ydjk.org.cn/Article/details/gt3nbvlohvw.html

D 数组 / 列表 / 集合   26 个任务 × 8 语言 =  208
来源：http://www.52xcode.cn/Article/details/gt3rrabyoec.html

E 字符串处理           22 个任务 × 8 语言 =  176
来源：http://www.52xcode.cn/Article/details/gt3eobeqbqq.html

F 文件与目录           12 个任务 × 8 语言 =   96
来源：http://www.ydjk.org.cn/Article/details/gt3yihvoobx.html

G 面向对象             16 个任务 × 8 语言 =  128
来源：http://www.ydjk.org.cn/Article/details/gt3imimpwds.html

H 异常与错误处理       10 个任务 × 8 语言 =   80
来源：http://www.ydjk.org.cn/Article/details/gt3owvrxzod.html

I 正则表达式            8 个任务 × 8 语言 =   64
来源：http://www.52xcode.cn/Article/details/gt3woywdwuw.html

J 日期与时间           10 个任务 × 8 语言 =   80
来源：http://www.52xcode.cn/Article/details/gt3bjovivfq.html

K JSON 与序列化         8 个任务 × 8 语言 =   64
来源：http://www.52xcode.cn/Article/details/gt3vdbnabwx.html

L 网络请求              8 个任务 × 8 语言 =   64
来源：http://www.52xcode.cn/Article/details/gt3gnqtavib.html

M 命令行 / 进程         8 个任务 × 8 语言 =   64
来源：http://www.ydjk.org.cn/Article/details/gt3uwxvvbuu.html

N 数据结构与算法       12 个任务 × 8 语言 =   96
来源：http://www.52xcode.cn/Article/details/gt3rusytjfr.html

O 并发与异步            6 个任务 × 8 语言 =   48
来源：http://www.52xcode.cn/Article/details/gt3nkbearnb.html

P 常用工具函数          8 个任务 × 8 语言 =   64
来源：http://www.52xcode.cn/Article/details/gt3hnoftoga.html

Q SQL 专题                              90
来源：http://www.52xcode.cn/Article/details/gt3dtpxwtmu.html

R Bash 专题                             80
来源：http://www.ydjk.org.cn/Article/details/gt3fbrqmajz.html

S C / C++ 专题                          60
来源：http://www.52xcode.cn/Article/details/gt3znypvtau.html

T 其他语言补充                          60
来源：http://www.52xcode.cn/Article/details/gt3ccnufdos.html

U 高频实用片段                         120
来源：http://www.52xcode.cn/Article/details/gt3dtnoiqff.html

------------------------------------
来源：http://www.ydjk.org.cn/Article/details/gt3sptqttnd.html

合计                                  2106 条
来源：http://www.ydjk.org.cn/Article/details/gt3bbzewshd.html

--------------------------------------------------------------------------------
来源：http://www.52xcode.cn/Article/details/gt3qzggiesn.html

使用提醒
来源：http://www.ydjk.org.cn/Article/details/gt3ujgxnama.html

--------------------------------------------------------------------------------
来源：http://www.52xcode.cn/Article/details/gt3gqyysous.html

1. 示例追求"最小可用"，正式项目中请补齐导入、错误处理与边界判断。
来源：http://www.ydjk.org.cn/Article/details/gt3ikqxtykd.html

2. 涉及文件、网络、数据库的示例，注意资源释放与异常捕获。
来源：http://www.52xcode.cn/Article/details/gt3gnxyappe.html

3. 语言版本差异较大（如 Python 3.10 的 match、Java 17 的 record/switch 箭头），
来源：http://www.ydjk.org.cn/Article/details/gt3vpieeipl.html

在旧版本上使用前请先确认语法支持情况。
来源：http://www.52xcode.cn/Article/details/gt3tsrmoimh.html

4. 标注"手写"的条目是因为该语言缺少对应内置能力，实际项目中可引入成熟库。
来源：http://www.ydjk.org.cn/Article/details/gt3yxaoousg.html

—— 文件结束 ——
来源：http://www.ydjk.org.cn/Article/details/gt3oirfwcek.html

================================================================================
来源：http://www.ydjk.org.cn/Article/details/gt3wqhfkfgo.html

程序语言常见例子速查手册（2024 版）
来源：http://www.52xcode.cn/Article/details/gt3tmnhagaa.html

Common Programming Examples Cheat Book
来源：http://www.ydjk.org.cn/Article/details/gt3txkublen.html

================================================================================
来源：http://www.52xcode.cn/Article/details/gt3kyvnorru.html

【收录内容】
来源：http://www.52xcode.cn/Article/details/gt3faurchpu.html

覆盖 12 种语言 / 语法与常见 API：
来源：http://www.52xcode.cn/Article/details/gt3vttczvho.html

Python · PHP · JavaScript · TypeScript · Java · Go · Ruby · C#
来源：http://www.52xcode.cn/Article/details/gt3sieyjpsn.html

SQL · Bash · C · C++
来源：http://www.52xcode.cn/Article/details/gt3sawewpfw.html

按「任务」分组：每个任务下按语言各给出一条最小可用示例。
来源：http://www.ydjk.org.cn/Article/details/gt3zojepmbn.html

【使用说明】
来源：http://www.ydjk.org.cn/Article/details/gt3qeawchcy.html

1. 每个任务形如 "[编号] 任务名"，下面每行以语言标记开头：
来源：http://www.ydjk.org.cn/Article/details/gt3uingruko.html

Py:    Python        PHP:   PHP           JS:    JavaScript
来源：http://www.52xcode.cn/Article/details/gt3hxeqvdie.html

TS:    TypeScript    Java:  Java          Go:    Go
来源：http://www.52xcode.cn/Article/details/gt3chubxxrb.html

Ruby:  Ruby          C#:    C#            SQL:   SQL
来源：http://www.52xcode.cn/Article/details/gt3mvizqidk.html

Bash:  Shell         C:     C             C++:   C++
来源：http://www.ydjk.org.cn/Article/details/gt3qsuiarho.html

2. 示例只展示核心写法，刻意省略 import / require / include / using 等样板代码。
来源：http://www.ydjk.org.cn/Article/details/gt3efnfowva.html

需要完整可运行文件时，请自行补齐当前语言的导入语句。
来源：http://www.ydjk.org.cn/Article/details/gt3elpyumqq.html

3. 语法基准：Python 3.10+ / PHP 8.1+ / ES2020+ / TypeScript 5 / Java 17 /
来源：http://www.52xcode.cn/Article/details/gt3xsbhrvrk.html

Go 1.21+ / Ruby 3.x / C# 10+ / C17 / C++17。
来源：http://www.52xcode.cn/Article/details/gt3terlixzr.html

4. 检索建议：用编辑器或浏览器 Ctrl+F 搜关键词，如 "排序" "读取文件" "正则"。
来源：http://www.ydjk.org.cn/Article/details/gt3wwteyjtz.html

5. 标记为 "// 无" 表示该语言没有对应的一等语法，需用替代写法（示例给出替代方案）。
来源：http://www.ydjk.org.cn/Article/details/gt3twxrmgka.html

6. 符号 "⏎" 表示代码在此处换行（主要用于 Python 等强制缩进、无法压成一行的结构）。
来源：http://www.52xcode.cn/Article/details/gt3tvneyejy.html

【文件统计】
来源：http://www.52xcode.cn/Article/details/gt3yaqiyzhn.html

语言示例共 2106 条，分布见本文末尾的「统计汇总」。
来源：http://www.ydjk.org.cn/Article/details/gt3sewgkgrc.html

--------------------------------------------------------------------------------
来源：http://www.ydjk.org.cn/Article/details/gt3uwemyxfd.html

目  录
来源：http://www.ydjk.org.cn/Article/details/gt3ufhuiawk.html

--------------------------------------------------------------------------------
来源：http://www.ydjk.org.cn/Article/details/gt3jtubcwbw.html

A. 基础语法与类型              （第 1 节，26 个任务，208 条）
来源：http://www.ydjk.org.cn/Article/details/gt3cfrvnmgi.html

B. 流程控制                    （第 2 节，16 个任务，128 条）
来源：http://www.ydjk.org.cn/Article/details/gt3zlsapyak.html

C. 函数与作用域                （第 3 节，16 个任务，128 条）
来源：http://www.ydjk.org.cn/Article/details/gt3acmzqqso.html

D. 数组 / 列表 / 集合          （第 4 节，26 个任务，208 条）
来源：http://www.ydjk.org.cn/Article/details/gt3zpinwvat.html

E. 字符串处理                  （第 5 节，22 个任务，176 条）
来源：http://www.52xcode.cn/Article/details/gt3fhqyslxt.html

F. 文件与目录                  （第 6 节，12 个任务，96 条）
来源：http://www.ydjk.org.cn/Article/details/gt3aqyfzeua.html

G. 面向对象                    （第 7 节，16 个任务，128 条）
来源：http://www.52xcode.cn/Article/details/gt3ywdiylsc.html

H. 异常与错误处理              （第 8 节，10 个任务，80 条）
来源：http://www.ydjk.org.cn/Article/details/gt3jwpktqai.html

I. 正则表达式                  （第 9 节，8 个任务，64 条）
来源：http://www.52xcode.cn/Article/details/gt3fvbqcxza.html


<!-- 参考信息 -->