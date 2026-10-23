代发 wailian999

[U21] Py：自定义上下文管理器
来源：http://www.ydjk.org.cn/Article/details/gt3trytswjy.html

@contextlib.contextmanager
来源：http://www.ydjk.org.cn/Article/details/gt3huavnhlg.html

[U22] Py：矩阵转置
来源：http://www.ydjk.org.cn/Article/details/gt3usbjkqdo.html

list(zip(*m))
来源：http://www.ydjk.org.cn/Article/details/gt3cflsossv.html

[U23] Py：分块读取大文件
来源：http://www.ydjk.org.cn/Article/details/gt3ykyvirur.html

for chunk in iter(lambda: f.read(8192), b""):
来源：http://www.52xcode.cn/Article/details/gt3ebxsnvoe.html

[U24] Py：路径操作
来源：http://www.52xcode.cn/Article/details/gt3ebsfevki.html

Path("a/b.txt").parent.mkdir(parents=True, exist_ok=True)
来源：http://www.52xcode.cn/Article/details/gt3aapfnuqo.html

[U25] Py：CSV 按字典读
来源：http://www.ydjk.org.cn/Article/details/gt3dtgstzaz.html

csv.DictReader(f)
来源：http://www.52xcode.cn/Article/details/gt3ggpwbxmr.html

[U26] Py：并发下载
来源：http://www.52xcode.cn/Article/details/gt3abzszqsy.html

ThreadPoolExecutor(max_workers=8).map(fetch, urls)
来源：http://www.ydjk.org.cn/Article/details/gt3kdoxtudj.html

[U27] Py：异步 HTTP
来源：http://www.52xcode.cn/Article/details/gt3whmphvgi.html

aiohttp.ClientSession() 配合 async with
来源：http://www.ydjk.org.cn/Article/details/gt3gvkanygx.html

[U28] Py：类型别名
来源：http://www.ydjk.org.cn/Article/details/gt3uooaniyg.html

UserId = int
来源：http://www.52xcode.cn/Article/details/gt3teakxvif.html

[U29] Py：属性校验
来源：http://www.52xcode.cn/Article/details/gt3stkgzyav.html

@property 与 @x.setter 配合
来源：http://www.ydjk.org.cn/Article/details/gt3epdirjke.html

[U30] Py：数据类
来源：http://www.ydjk.org.cn/Article/details/gt3oisdidcx.html

@dataclass(slots=True)
来源：http://www.ydjk.org.cn/Article/details/gt3kdawnrrw.html

[U31] Py：单测
来源：http://www.ydjk.org.cn/Article/details/gt3tjziwrzi.html

python -m pytest -q
来源：http://www.ydjk.org.cn/Article/details/gt3lsjivqoq.html

[U32] Py：代码格式化
来源：http://www.52xcode.cn/Article/details/gt3pvqtonbl.html

ruff format . && ruff check --fix .
来源：http://www.ydjk.org.cn/Article/details/gt3elzoiigy.html

[U33] Py：打包发布
来源：http://www.ydjk.org.cn/Article/details/gt3ndcmircf.html

python -m build  （依赖 pyproject.toml）
来源：http://www.52xcode.cn/Article/details/gt3hixonxcm.html

[U34] Py：判断编码
来源：http://www.52xcode.cn/Article/details/gt3kinierqv.html

chardet.detect(raw)
来源：http://www.52xcode.cn/Article/details/gt3javvekol.html

[U35] Py：发送邮件
来源：http://www.52xcode.cn/Article/details/gt3aoxesqfh.html

smtplib.SMTP_SSL(...).send_message(msg)
来源：http://www.52xcode.cn/Article/details/gt3arglwzra.html

[U36] Py：定时任务
来源：http://www.52xcode.cn/Article/details/gt3hdpnmpqr.html

schedule.every(10).minutes.do(job)
来源：http://www.52xcode.cn/Article/details/gt3nwrkwwjc.html

[U37] Py：读写 Excel
来源：http://www.ydjk.org.cn/Article/details/gt3nzfbnyau.html

pandas.read_excel / DataFrame.to_excel
来源：http://www.ydjk.org.cn/Article/details/gt3dxghvxdw.html

[U38] Py：获取脚本所在目录
来源：http://www.ydjk.org.cn/Article/details/gt3ejpejeyh.html

Path(__file__).resolve().parent
来源：http://www.ydjk.org.cn/Article/details/gt3gtikphws.html

[U39] Py：判断是否在交互环境
来源：http://www.ydjk.org.cn/Article/details/gt3bfpxbmrk.html

sys.stdout.isatty()
来源：http://www.52xcode.cn/Article/details/gt3ivtvcobc.html

[U40] Py：打印到标准错误
来源：http://www.52xcode.cn/Article/details/gt3iyhrpbnv.html

print("err", file=sys.stderr)
来源：http://www.52xcode.cn/Article/details/gt3fmhxzgnh.html

[U41] PHP：初始化 Composer 项目
来源：http://www.52xcode.cn/Article/details/gt3qbryjwda.html

composer init;  composer require guzzlehttp/guzzle
来源：http://www.52xcode.cn/Article/details/gt3qgxesyww.html

[U42] PHP：PSR-4 自动加载
来源：http://www.ydjk.org.cn/Article/details/gt3jetydgka.html

"autoload": { "psr-4": { "App\\": "src/" } }
来源：http://www.52xcode.cn/Article/details/gt3zstlazhe.html

[U43] PHP：声明命名空间
来源：http://www.ydjk.org.cn/Article/details/gt3rcyhdgmq.html

namespace App\Http;
来源：http://www.ydjk.org.cn/Article/details/gt3ifgrcxtv.html

[U44] PHP：开启严格类型
来源：http://www.52xcode.cn/Article/details/gt3psrvlavl.html

declare(strict_types=1);
来源：http://www.52xcode.cn/Article/details/gt3uzfnixkx.html

[U45] PHP：类型声明与返回类型
来源：http://www.ydjk.org.cn/Article/details/gt3zgaxalkc.html

function add(int $a, int $b): int { return $a + $b; }
来源：http://www.52xcode.cn/Article/details/gt3bzlkqfgf.html

[U46] PHP：可空类型
来源：http://www.52xcode.cn/Article/details/gt3rkcfmufy.html

?string $name = null
来源：http://www.ydjk.org.cn/Article/details/gt3ifqvndkv.html

[U47] PHP：联合类型
来源：http://www.ydjk.org.cn/Article/details/gt3xqnwrnbh.html

int|string $id
来源：http://www.52xcode.cn/Article/details/gt3vhulkeha.html

[U48] PHP：纯枚举
来源：http://www.ydjk.org.cn/Article/details/gt3mgdaavvu.html

enum Status: string { case Active = "active"; case Off = "off"; }
来源：http://www.ydjk.org.cn/Article/details/gt3wdbcmdiq.html

[U49] PHP：只读属性
来源：http://www.52xcode.cn/Article/details/gt3gebljqjk.html

public readonly string $name
来源：http://www.52xcode.cn/Article/details/gt3vbyewkmn.html

[U50] PHP：构造器属性提升
来源：http://www.52xcode.cn/Article/details/gt3yahvpstv.html

public function __construct(private int $id) {}
来源：http://www.52xcode.cn/Article/details/gt3zvazhxmu.html

[U51] PHP：数组解构
来源：http://www.52xcode.cn/Article/details/gt3zrtnsxdv.html

[$a, $b] = $arr;
来源：http://www.52xcode.cn/Article/details/gt3qsfppcud.html

[U52] PHP：箭头函数
来源：http://www.52xcode.cn/Article/details/gt3faywiuqk.html

$double = fn($x) => $x * 2;
来源：http://www.ydjk.org.cn/Article/details/gt3hphnjceo.html

[U53] PHP：空合并运算符
来源：http://www.ydjk.org.cn/Article/details/gt3vghotfym.html

$v = $a ?? $b ?? "default";
来源：http://www.52xcode.cn/Article/details/gt3qrwzxfcf.html

[U54] PHP：空安全调用
来源：http://www.ydjk.org.cn/Article/details/gt3uiigdgwo.html

$obj?->method()
来源：http://www.ydjk.org.cn/Article/details/gt3ekrztktj.html

[U55] PHP：match 表达式
来源：http://www.52xcode.cn/Article/details/gt3nfrukjnl.html

$s = match($x) { 1 => "一", default => "其他" };
来源：http://www.ydjk.org.cn/Article/details/gt3jsfesxex.html

[U56] PHP：命名参数
来源：http://www.52xcode.cn/Article/details/gt3lcvrsvjo.html

f(a: 1, b: 2)
来源：http://www.ydjk.org.cn/Article/details/gt3usphzyrw.html

[U57] PHP：字符串插值
来源：http://www.52xcode.cn/Article/details/gt3eqmfqwpi.html

"值: {$a}"
来源：http://www.ydjk.org.cn/Article/details/gt3xypptwdy.html

[U58] PHP：数组三件套
来源：http://www.52xcode.cn/Article/details/gt3kehydcnv.html

array_map($f, $a);  array_filter($a, $f);  array_reduce($a, $f, 0);
来源：http://www.ydjk.org.cn/Article/details/gt3srjqeeio.html

[U59] PHP：自定义排序
来源：http://www.ydjk.org.cn/Article/details/gt3pcpdfula.html

usort($arr, fn($a, $b) => $a["age"] <=> $b["age"]);
来源：http://www.52xcode.cn/Article/details/gt3lbqmvywd.html

[U60] PHP：JSON 编解码
来源：http://www.ydjk.org.cn/Article/details/gt3lkaeiyxq.html

json_encode($d, JSON_UNESCAPED_UNICODE);  json_decode($s, true);
来源：http://www.52xcode.cn/Article/details/gt3czvrfqmm.html

[U61] PHP：正则
来源：http://www.52xcode.cn/Article/details/gt3laovwxkv.html

preg_match('/(\d+)/', $s, $m);  preg_replace('/\d+/', '#', $s);
来源：http://www.52xcode.cn/Article/details/gt3iwkllvyj.html

[U62] PHP：日期对象
来源：http://www.52xcode.cn/Article/details/gt3oamctdfn.html

(new DateTimeImmutable())->format("Y-m-d");
来源：http://www.ydjk.org.cn/Article/details/gt3egvqiwpc.html

[U63] PHP：文件读写
来源：http://www.ydjk.org.cn/Article/details/gt3clfnikhn.html

file_get_contents($f);  file_put_contents($f, $data);
来源：http://www.ydjk.org.cn/Article/details/gt3jhsezhrn.html

[U64] PHP：目录遍历
来源：http://www.ydjk.org.cn/Article/details/gt3ijxpmbtf.html

glob("dir/*.php");  scandir("dir");
来源：http://www.ydjk.org.cn/Article/details/gt3yoxvjhcw.html

[U65] PHP：会话
来源：http://www.ydjk.org.cn/Article/details/gt3vxdqugfu.html

session_start();  $_SESSION["uid"] = 1;
来源：http://www.ydjk.org.cn/Article/details/gt3mjliaroh.html

[U66] PHP：设置 Cookie
来源：http://www.ydjk.org.cn/Article/details/gt3ufihxehv.html

setcookie("token", $v, ["httponly" => true, "samesite" => "Lax"]);
来源：http://www.52xcode.cn/Article/details/gt3urtnjhxq.html

[U67] PHP：处理文件上传
来源：http://www.52xcode.cn/Article/details/gt3yzhnvcfz.html

$_FILES["file"]["tmp_name"] 与 move_uploaded_file()
来源：http://www.ydjk.org.cn/Article/details/gt3essbtwhq.html

[U68] PHP：PDO 连接
来源：http://www.52xcode.cn/Article/details/gt3iwlxslwm.html

$pdo = new PDO("mysql:host=localhost;dbname=app", "root", "");
来源：http://www.ydjk.org.cn/Article/details/gt3igadxhtn.html

[U69] PHP：PDO 预处理
来源：http://www.ydjk.org.cn/Article/details/gt3exxjcybr.html

$stmt = $pdo->prepare("SELECT * FROM users WHERE id = ?");  $stmt->execute([$id]);
来源：http://www.ydjk.org.cn/Article/details/gt3mowprkbp.html

[U70] PHP：PDO 事务
来源：http://www.ydjk.org.cn/Article/details/gt3hmzaouvk.html

$pdo->beginTransaction();  $pdo->commit();  $pdo->rollBack();
来源：http://www.ydjk.org.cn/Article/details/gt3maxiyujx.html

[U71] PHP：抛出异常
来源：http://www.52xcode.cn/Article/details/gt3kkwpykpg.html

throw new RuntimeException("失败", 500);
来源：http://www.52xcode.cn/Article/details/gt3fjbtuxjp.html

[U72] PHP：写错误日志
来源：http://www.52xcode.cn/Article/details/gt3hyqninsz.html

error_log("失败: " . $e->getMessage());
来源：http://www.ydjk.org.cn/Article/details/gt3egkuospj.html

[U73] PHP：读取 ini 配置
来源：http://www.52xcode.cn/Article/details/gt3nkzozuth.html

parse_ini_file("config.ini", true)
来源：http://www.52xcode.cn/Article/details/gt3lttwldfy.html

[U74] PHP：读取环境变量
来源：http://www.ydjk.org.cn/Article/details/gt3gnzgazqy.html

getenv("APP_ENV") ?: "production"
来源：http://www.52xcode.cn/Article/details/gt3shedvhqq.html

[U75] PHP：依赖注入
来源：http://www.ydjk.org.cn/Article/details/gt3joxycgxp.html

composer require psr/container
来源：http://www.ydjk.org.cn/Article/details/gt3plvtljge.html

[U76] PHP：简单路由
来源：http://www.52xcode.cn/Article/details/gt3rtsnhcay.html

$path = parse_url($_SERVER["REQUEST_URI"], PHP_URL_PATH);
来源：http://www.52xcode.cn/Article/details/gt3dxplgspn.html

[U77] PHP：模板渲染
来源：http://www.ydjk.org.cn/Article/details/gt3plonaghb.html

composer require twig/twig
来源：http://www.ydjk.org.cn/Article/details/gt3hppddlne.html

[U78] PHP：单元测试
来源：http://www.ydjk.org.cn/Article/details/gt3ezarcgsn.html

composer require --dev phpunit/phpunit
来源：http://www.52xcode.cn/Article/details/gt3ulldjmqn.html

[U79] PHP：静态分析
来源：http://www.52xcode.cn/Article/details/gt3szjfbbpd.html

composer require --dev phpstan/phpstan
来源：http://www.ydjk.org.cn/Article/details/gt3rhnajhfe.html

[U80] PHP：代码规范修复
来源：http://www.ydjk.org.cn/Article/details/gt3tsfootmx.html

composer require --dev friendsofphp/php-cs-fixer
来源：http://www.52xcode.cn/Article/details/gt3cikajoqh.html

[U81] JS：初始化项目
来源：http://www.ydjk.org.cn/Article/details/gt3jectxeqk.html

npm init -y;  npm i express
来源：http://www.52xcode.cn/Article/details/gt3xpiojhiv.html

[U82] JS：package.json 脚本
来源：http://www.ydjk.org.cn/Article/details/gt3argizthr.html

"scripts": { "dev": "vite", "build": "vite build" }
来源：http://www.ydjk.org.cn/Article/details/gt3jgwczvlb.html

[U83] JS：ES Module 导入导出
来源：http://www.ydjk.org.cn/Article/details/gt3ahgoeixj.html

export const a = 1;  import { a } from "./m.js";
来源：http://www.ydjk.org.cn/Article/details/gt3ntucyini.html

[U84] JS：CommonJS 写法
来源：http://www.52xcode.cn/Article/details/gt3hrybsgot.html

module.exports = { a };  const { a } = require("./m");
来源：http://www.52xcode.cn/Article/details/gt3tyesizht.html

[U85] JS：可选链
来源：http://www.52xcode.cn/Article/details/gt3oywecyro.html

a?.b?.c
来源：http://www.52xcode.cn/Article/details/gt3htqpjchm.html

[U86] JS：空值合并
来源：http://www.ydjk.org.cn/Article/details/gt3oruingvi.html

a ?? b
来源：http://www.ydjk.org.cn/Article/details/gt3wgwjdocf.html

[U87] JS：解构默认值
来源：http://www.ydjk.org.cn/Article/details/gt3qtdpplnk.html

const { a = 1, b = 2 } = obj;
来源：http://www.ydjk.org.cn/Article/details/gt3ldvrfpqp.html

[U88] JS：对象展开合并
来源：http://www.52xcode.cn/Article/details/gt3utotfshw.html

{ ...a, ...b }
来源：http://www.52xcode.cn/Article/details/gt3twmnbuof.html

[U89] JS：数组去重
来源：http://www.ydjk.org.cn/Article/details/gt3rhrxkahk.html

[...new Set(arr)]
来源：http://www.ydjk.org.cn/Article/details/gt3fxekjjgw.html

[U90] JS：数字数组排序
来源：http://www.ydjk.org.cn/Article/details/gt3jomaiqey.html

[...arr].sort((a, b) => a - b)
来源：http://www.52xcode.cn/Article/details/gt3bfkeazmb.html

[U91] JS：对象键值遍历
来源：http://www.52xcode.cn/Article/details/gt3wqdegzze.html

Object.entries(obj).forEach(([k, v]) => {});
来源：http://www.ydjk.org.cn/Article/details/gt3gsuxviqa.html

[U92] JS：深拷贝
来源：http://www.ydjk.org.cn/Article/details/gt3kzlblqvk.html

structuredClone(obj)
来源：http://www.ydjk.org.cn/Article/details/gt3rmtbndjy.html

[U93] JS：模板字符串
来源：http://www.ydjk.org.cn/Article/details/gt3nufvaqqu.html

`共 ${n} 条`
来源：http://www.ydjk.org.cn/Article/details/gt3zrfvharw.html

[U94] JS：箭头函数
来源：http://www.52xcode.cn/Article/details/gt3dweilrcq.html

const double = x => x * 2;
来源：http://www.52xcode.cn/Article/details/gt3whrwedrc.html

[U95] JS：Promise 包装
来源：http://www.52xcode.cn/Article/details/gt3tdqftusk.html

new Promise((resolve, reject) => {})
来源：http://www.ydjk.org.cn/Article/details/gt3qttivxle.html

[U96] JS：async/await 与异常
来源：http://www.ydjk.org.cn/Article/details/gt3soesdutf.html

try { const d = await f(); } catch (e) { console.error(e); }
来源：http://www.ydjk.org.cn/Article/details/gt3jgokerap.html

[U97] JS：并发请求
来源：http://www.52xcode.cn/Article/details/gt3weviaaia.html

await Promise.all(urls.map(u => fetch(u)))
来源：http://www.52xcode.cn/Article/details/gt3tbyvhdpl.html

[U98] JS：fetch 带 JSON
来源：http://www.52xcode.cn/Article/details/gt3roafinot.html

await fetch(url, { method: "POST", headers: { "Content-Type": "application/json" }, body: JSON.stringify(d) })
来源：http://www.ydjk.org.cn/Article/details/gt3yevagvxx.html

[U99] JS：事件监听
来源：http://www.52xcode.cn/Article/details/gt3pnawxtjw.html

el.addEventListener("click", e => {})
来源：http://www.52xcode.cn/Article/details/gt3yfroblsg.html

[U100] JS：DOM 查询
来源：http://www.ydjk.org.cn/Article/details/gt3gupcqwdg.html

document.querySelector(".item")
来源：http://www.ydjk.org.cn/Article/details/gt3pypkxdij.html

[U101] JS：classList 操作
来源：http://www.ydjk.org.cn/Article/details/gt3plvcnfal.html

el.classList.toggle("active")
来源：http://www.ydjk.org.cn/Article/details/gt3nkbomnfm.html

[U102] JS：本地存储
来源：http://www.ydjk.org.cn/Article/details/gt3bxsrvxti.html

localStorage.setItem("k", JSON.stringify(v))
来源：http://www.52xcode.cn/Article/details/gt3vmprzrqh.html

[U103] JS：定时器
来源：http://www.52xcode.cn/Article/details/gt3qihqgeud.html

setTimeout(fn, 1000);  setInterval(fn, 1000);
来源：http://www.ydjk.org.cn/Article/details/gt3hgnbtmov.html

[U104] JS：防抖
来源：http://www.52xcode.cn/Article/details/gt3kxjwfvwp.html

const debounce = (fn, ms) => { let t; return (...a) => { clearTimeout(t); t = setTimeout(() => fn(...a), ms); }; };
来源：http://www.52xcode.cn/Article/details/gt3ufevheyg.html

[U105] JS：节流
来源：http://www.ydjk.org.cn/Article/details/gt3xelfpvin.html

const throttle = (fn, ms) => { let last = 0; return (...a) => { const n = Date.now(); if (n - last >= ms) { last = n; fn(...a); } }; };
来源：http://www.ydjk.org.cn/Article/details/gt3jojnmejo.html

[U106] JS：日期格式化
来源：http://www.ydjk.org.cn/Article/details/gt3xymcsmtu.html

new Intl.DateTimeFormat("zh-CN", { dateStyle: "medium" }).format(new Date())
来源：http://www.ydjk.org.cn/Article/details/gt3iagmuiox.html

[U107] JS：数字千分位
来源：http://www.52xcode.cn/Article/details/gt3zbehudbp.html

new Intl.NumberFormat("en-US").format(1234567)
来源：http://www.ydjk.org.cn/Article/details/gt3ggbwndgj.html

[U108] JS：随机整数
来源：http://www.ydjk.org.cn/Article/details/gt3unuochwu.html

Math.floor(Math.random() * (max - min + 1)) + min
来源：http://www.ydjk.org.cn/Article/details/gt3slyembhh.html

[U109] JS：数组分组
来源：http://www.52xcode.cn/Article/details/gt3twgnzfmh.html

Object.groupBy(arr, x => x.type)
来源：http://www.52xcode.cn/Article/details/gt3avzofpoc.html

[U110] JS：数组分块
来源：http://www.ydjk.org.cn/Article/details/gt3zrxqfpwb.html

arr.reduce((acc, x, i) => (i % size ? acc : [...acc, arr.slice(i, i + size)]), [])
来源：http://www.52xcode.cn/Article/details/gt3iexxgsxw.html

[U111] JS：对象转 Map
来源：http://www.ydjk.org.cn/Article/details/gt3zxcqjbtz.html

new Map(Object.entries(obj))
来源：http://www.52xcode.cn/Article/details/gt3jxjkgllg.html

[U112] JS：字符串补位
来源：http://www.ydjk.org.cn/Article/details/gt3lsexnfyo.html

"7".padStart(3, "0")
来源：http://www.52xcode.cn/Article/details/gt3smgiieph.html

[U113] JS：正则替换全部
来源：http://www.52xcode.cn/Article/details/gt3rllwuzcl.html

s.replaceAll("a", "b")
来源：http://www.52xcode.cn/Article/details/gt3gnpppygy.html

[U114] JS：JSON 深比较
来源：http://www.52xcode.cn/Article/details/gt3sxiefuon.html

JSON.stringify(a) === JSON.stringify(b)
来源：http://www.ydjk.org.cn/Article/details/gt3huucrbyt.html

[U115] JS：生成 UUID
来源：http://www.ydjk.org.cn/Article/details/gt3mysqvzjw.html

crypto.randomUUID()
来源：http://www.ydjk.org.cn/Article/details/gt3oheimrkw.html

[U116] JS：类型检查（JSDoc）
来源：http://www.ydjk.org.cn/Article/details/gt3nvuoelnz.html

/** @param {string} name */ function f(name) {}
来源：http://www.ydjk.org.cn/Article/details/gt3enepekpe.html

[U117] JS：单元测试
来源：http://www.ydjk.org.cn/Article/details/gt3lsdfhesr.html

npm i -D vitest;  npx vitest
来源：http://www.52xcode.cn/Article/details/gt3hrbslnap.html

[U118] JS：开发服务器
来源：http://www.52xcode.cn/Article/details/gt3hpzkkcpl.html

npm i -D vite;  npx vite
来源：http://www.ydjk.org.cn/Article/details/gt3pkorekck.html

[U119] JS：生产构建
来源：http://www.ydjk.org.cn/Article/details/gt3sdszwguo.html

npx vite build
来源：http://www.ydjk.org.cn/Article/details/gt3mtowgkec.html

[U120] JS：读取环境变量（Vite）
来源：http://www.ydjk.org.cn/Article/details/gt3fasaectx.html

import.meta.env.VITE_API_URL
来源：http://www.ydjk.org.cn/Article/details/gt3wzgnswex.html

================================================================================
来源：http://www.ydjk.org.cn/Article/details/gt3byaecnnm.html

统计汇总
来源：http://www.ydjk.org.cn/Article/details/gt3nkmfolgc.html

================================================================================
来源：http://www.ydjk.org.cn/Article/details/gt3ntltpmut.html

按语言统计（条）：
来源：http://www.52xcode.cn/Article/details/gt3nmtpaizf.html

Python ......... 252
来源：http://www.ydjk.org.cn/Article/details/gt3ipkpmqdt.html

PHP ............ 252
来源：http://www.52xcode.cn/Article/details/gt3rztjfezl.html

JavaScript ..... 252
来源：http://www.52xcode.cn/Article/details/gt3eimkpduv.html

TypeScript ..... 212
来源：http://www.52xcode.cn/Article/details/gt3ippoulax.html

Java ........... 212
来源：http://www.52xcode.cn/Article/details/gt3gbjhmnqn.html

Go ............. 212
来源：http://www.52xcode.cn/Article/details/gt3hedbmvnw.html

Ruby ........... 212
来源：http://www.52xcode.cn/Article/details/gt3yfipyzxb.html

C# ............. 212
来源：http://www.ydjk.org.cn/Article/details/gt3bnyocvzz.html

C .............. 30
来源：http://www.52xcode.cn/Article/details/gt3qdwpcznh.html

C++ ............ 30
来源：http://www.ydjk.org.cn/Article/details/gt3hzocobbe.html

SQL ............ 90
来源：http://www.ydjk.org.cn/Article/details/gt3rexdjiru.html

Bash ........... 80
来源：http://www.ydjk.org.cn/Article/details/gt3apbaucby.html

Kotlin ......... 15
来源：http://www.52xcode.cn/Article/details/gt3ulxalgbv.html

Swift .......... 15
来源：http://www.52xcode.cn/Article/details/gt3vyloudud.html

Lua ............ 10
来源：http://www.52xcode.cn/Article/details/gt3dddglipg.html

Perl ........... 10
来源：http://www.52xcode.cn/Article/details/gt3etibaesx.html

Scala .......... 10
来源：http://www.52xcode.cn/Article/details/gt3spdgcqbb.html

------------------------------------
来源：http://www.52xcode.cn/Article/details/gt3dwhyllov.html

合计 ........... 2106 条
来源：http://www.ydjk.org.cn/Article/details/gt3tsdxjrfz.html

按章节统计：
来源：http://www.52xcode.cn/Article/details/gt3howffdlq.html

A 基础语法与类型       26 个任务 × 8 语言 =  208
来源：http://www.ydjk.org.cn/Article/details/gt3kftnzmro.html

B 流程控制             16 个任务 × 8 语言 =  128
来源：http://www.ydjk.org.cn/Article/details/gt3obvffjqa.html

C 函数与作用域         16 个任务 × 8 语言 =  128
来源：http://www.52xcode.cn/Article/details/gt3exrhujcg.html

D 数组 / 列表 / 集合   26 个任务 × 8 语言 =  208
来源：http://www.52xcode.cn/Article/details/gt3xhyanjhm.html

E 字符串处理           22 个任务 × 8 语言 =  176
来源：http://www.52xcode.cn/Article/details/gt3gyyxrzzh.html

F 文件与目录           12 个任务 × 8 语言 =   96
来源：http://www.52xcode.cn/Article/details/gt3nevavscw.html

G 面向对象             16 个任务 × 8 语言 =  128
来源：http://www.ydjk.org.cn/Article/details/gt3nczmkudd.html

H 异常与错误处理       10 个任务 × 8 语言 =   80
来源：http://www.ydjk.org.cn/Article/details/gt3uaxrfmit.html

I 正则表达式            8 个任务 × 8 语言 =   64
来源：http://www.52xcode.cn/Article/details/gt3tvbfxuvt.html

J 日期与时间           10 个任务 × 8 语言 =   80
来源：http://www.52xcode.cn/Article/details/gt3mkryaezl.html

K JSON 与序列化         8 个任务 × 8 语言 =   64
来源：http://www.ydjk.org.cn/Article/details/gt3kyvxxmvb.html

L 网络请求              8 个任务 × 8 语言 =   64
来源：http://www.ydjk.org.cn/Article/details/gt3osbsxtfu.html

M 命令行 / 进程         8 个任务 × 8 语言 =   64
来源：http://www.52xcode.cn/Article/details/gt3wpuebotl.html

N 数据结构与算法       12 个任务 × 8 语言 =   96
来源：http://www.52xcode.cn/Article/details/gt3bypppqgn.html

O 并发与异步            6 个任务 × 8 语言 =   48
来源：http://www.52xcode.cn/Article/details/gt3cemcetwy.html

P 常用工具函数          8 个任务 × 8 语言 =   64
来源：http://www.52xcode.cn/Article/details/gt3rnusgxja.html

Q SQL 专题                              90
来源：http://www.ydjk.org.cn/Article/details/gt3jldgizvw.html

R Bash 专题                             80
来源：http://www.52xcode.cn/Article/details/gt3sgezonbv.html

S C / C++ 专题                          60
来源：http://www.52xcode.cn/Article/details/gt3hrfybqhp.html

T 其他语言补充                          60
来源：http://www.ydjk.org.cn/Article/details/gt3clbztfhf.html

U 高频实用片段                         120
来源：http://www.ydjk.org.cn/Article/details/gt3zmgnazdt.html

------------------------------------
来源：http://www.ydjk.org.cn/Article/details/gt3rbjqdgru.html

合计                                  2106 条
来源：http://www.52xcode.cn/Article/details/gt3gknobvlx.html

--------------------------------------------------------------------------------
来源：http://www.ydjk.org.cn/Article/details/gt3wecfqkzc.html

使用提醒
来源：http://www.ydjk.org.cn/Article/details/gt3taptzrdn.html

--------------------------------------------------------------------------------
来源：http://www.52xcode.cn/Article/details/gt3kcloyjdd.html

1. 示例追求"最小可用"，正式项目中请补齐导入、错误处理与边界判断。
来源：http://www.52xcode.cn/Article/details/gt3gbkinhmn.html

2. 涉及文件、网络、数据库的示例，注意资源释放与异常捕获。
来源：http://www.ydjk.org.cn/Article/details/gt3rrsitxmw.html

3. 语言版本差异较大（如 Python 3.10 的 match、Java 17 的 record/switch 箭头），
来源：http://www.ydjk.org.cn/Article/details/gt3mrdxosbo.html

在旧版本上使用前请先确认语法支持情况。
来源：http://www.ydjk.org.cn/Article/details/gt3ovunpmvs.html

4. 标注"手写"的条目是因为该语言缺少对应内置能力，实际项目中可引入成熟库。
来源：http://www.ydjk.org.cn/Article/details/gt3utfsgrht.html

—— 文件结束 ——
来源：http://www.ydjk.org.cn/Article/details/gt3ijnnrrmd.html

================================================================================
来源：http://www.52xcode.cn/Article/details/gt3osunutvg.html

程序语言常见例子速查手册（2024 版）
来源：http://www.ydjk.org.cn/Article/details/gt3bwlgglbz.html

Common Programming Examples Cheat Book
来源：http://www.52xcode.cn/Article/details/gt3lwangtly.html

================================================================================
来源：http://www.ydjk.org.cn/Article/details/gt3wbpzwaqp.html

【收录内容】
来源：http://www.52xcode.cn/Article/details/gt3xdonpnox.html

覆盖 12 种语言 / 语法与常见 API：
来源：http://www.52xcode.cn/Article/details/gt3kowrjinh.html

Python · PHP · JavaScript · TypeScript · Java · Go · Ruby · C#
来源：http://www.52xcode.cn/Article/details/gt3zruzcxyg.html

SQL · Bash · C · C++
来源：http://www.ydjk.org.cn/Article/details/gt3wacxpobi.html

按「任务」分组：每个任务下按语言各给出一条最小可用示例。
来源：http://www.ydjk.org.cn/Article/details/gt3urhwbvuw.html

【使用说明】
来源：http://www.52xcode.cn/Article/details/gt3qeywjmjv.html

1. 每个任务形如 "[编号] 任务名"，下面每行以语言标记开头：
来源：http://www.ydjk.org.cn/Article/details/gt3byiylabw.html

Py:    Python        PHP:   PHP           JS:    JavaScript
来源：http://www.ydjk.org.cn/Article/details/gt3ulycstbu.html

TS:    TypeScript    Java:  Java          Go:    Go
来源：http://www.ydjk.org.cn/Article/details/gt3rrpqevou.html

Ruby:  Ruby          C#:    C#            SQL:   SQL
来源：http://www.52xcode.cn/Article/details/gt3tjinecay.html

Bash:  Shell         C:     C             C++:   C++
来源：http://www.52xcode.cn/Article/details/gt3tziiklix.html

2. 示例只展示核心写法，刻意省略 import / require / include / using 等样板代码。
来源：http://www.52xcode.cn/Article/details/gt3stmxriip.html

需要完整可运行文件时，请自行补齐当前语言的导入语句。
来源：http://www.52xcode.cn/Article/details/gt3jtmpedcw.html

3. 语法基准：Python 3.10+ / PHP 8.1+ / ES2020+ / TypeScript 5 / Java 17 /
来源：http://www.ydjk.org.cn/Article/details/gt3wyunblww.html

Go 1.21+ / Ruby 3.x / C# 10+ / C17 / C++17。
来源：http://www.ydjk.org.cn/Article/details/gt3ljuwmwhz.html

4. 检索建议：用编辑器或浏览器 Ctrl+F 搜关键词，如 "排序" "读取文件" "正则"。
来源：http://www.52xcode.cn/Article/details/gt3glrzziml.html

5. 标记为 "// 无" 表示该语言没有对应的一等语法，需用替代写法（示例给出替代方案）。
来源：http://www.52xcode.cn/Article/details/gt3luanifmm.html

6. 符号 "⏎" 表示代码在此处换行（主要用于 Python 等强制缩进、无法压成一行的结构）。
来源：http://www.52xcode.cn/Article/details/gt3bbqnuztc.html

【文件统计】
来源：http://www.ydjk.org.cn/Article/details/gt3lijjbttw.html

语言示例共 2106 条，分布见本文末尾的「统计汇总」。
来源：http://www.52xcode.cn/Article/details/gt3hmpbsslo.html

--------------------------------------------------------------------------------
来源：http://www.ydjk.org.cn/Article/details/gt3bidnaysv.html

目  录
来源：http://www.ydjk.org.cn/Article/details/gt3qouylvxl.html

--------------------------------------------------------------------------------
来源：http://www.52xcode.cn/Article/details/gt3ciheavru.html

A. 基础语法与类型              （第 1 节，26 个任务，208 条）
来源：http://www.52xcode.cn/Article/details/gt3capebmik.html

B. 流程控制                    （第 2 节，16 个任务，128 条）
来源：http://www.ydjk.org.cn/Article/details/gt3omqjylix.html

C. 函数与作用域                （第 3 节，16 个任务，128 条）
来源：http://www.52xcode.cn/Article/details/gt3vxdpwgxz.html

D. 数组 / 列表 / 集合          （第 4 节，26 个任务，208 条）
来源：http://www.52xcode.cn/Article/details/gt3hxauusgz.html

E. 字符串处理                  （第 5 节，22 个任务，176 条）
来源：http://www.ydjk.org.cn/Article/details/gt3ncfedlut.html

F. 文件与目录                  （第 6 节，12 个任务，96 条）
来源：http://www.ydjk.org.cn/Article/details/gt3fkabmsjs.html

G. 面向对象                    （第 7 节，16 个任务，128 条）
来源：http://www.ydjk.org.cn/Article/details/gt3cwefikvg.html

H. 异常与错误处理              （第 8 节，10 个任务，80 条）
来源：http://www.ydjk.org.cn/Article/details/gt3elhnooiy.html

I. 正则表达式                  （第 9 节，8 个任务，64 条）
来源：http://www.ydjk.org.cn/Article/details/gt3ikqsqrkj.html

J. 日期与时间                  （第 10 节，10 个任务，80 条）
来源：http://www.ydjk.org.cn/Article/details/gt3majoexeb.html

K. JSON 与序列化               （第 11 节，8 个任务，64 条）
来源：http://www.ydjk.org.cn/Article/details/gt3ccvochdp.html

L. 网络请求                    （第 12 节，8 个任务，64 条）
来源：http://www.ydjk.org.cn/Article/details/gt3joxckmpt.html

M. 命令行 / 进程 / 环境        （第 13 节，8 个任务，64 条）
来源：http://www.ydjk.org.cn/Article/details/gt3hraxhkze.html

N. 数据结构与算法              （第 14 节，12 个任务，96 条）
来源：http://www.52xcode.cn/Article/details/gt3zcntdewl.html

O. 并发与异步                  （第 15 节，6 个任务，48 条）
来源：http://www.ydjk.org.cn/Article/details/gt3prpdlfgu.html

P. 常用工具函数                （第 16 节，8 个任务，64 条）
来源：http://www.ydjk.org.cn/Article/details/gt3vtlpkllw.html

Q. SQL 专题                    （第 17 节，90 条）
来源：http://www.52xcode.cn/Article/details/gt3dxilomsp.html


<!-- 参考信息 -->