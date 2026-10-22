代发 wailian999

[U19] Py：正则替换带回调
来源：http://www.52xcode.cn/Article/details/gt2lxgqbyio.html

re.sub(r"\d+", lambda m: str(int(m.group()) * 2), s)
来源：http://www.52xcode.cn/Article/details/gt2oxeehfhk.html

[U20] Py：缓存函数结果
来源：http://www.52xcode.cn/Article/details/gt2naityiyk.html

@functools.lru_cache(maxsize=None)
来源：http://www.52xcode.cn/Article/details/gt2qvgbuqcd.html

[U21] Py：自定义上下文管理器
来源：http://www.ydjk.org.cn/Article/details/gt2fnfjrahr.html

@contextlib.contextmanager
来源：http://www.ydjk.org.cn/Article/details/gt2qqvvmumj.html

[U22] Py：矩阵转置
来源：http://www.52xcode.cn/Article/details/gt2zqevneuj.html

list(zip(*m))
来源：http://www.52xcode.cn/Article/details/gt2xvqqnapt.html

[U23] Py：分块读取大文件
来源：http://www.ydjk.org.cn/Article/details/gt2tbrooenm.html

for chunk in iter(lambda: f.read(8192), b""):
来源：http://www.52xcode.cn/Article/details/gt2yjbxebrq.html

[U24] Py：路径操作
来源：http://www.ydjk.org.cn/Article/details/gt2qlqdsrqr.html

Path("a/b.txt").parent.mkdir(parents=True, exist_ok=True)
来源：http://www.52xcode.cn/Article/details/gt2roczlugl.html

[U25] Py：CSV 按字典读
来源：http://www.ydjk.org.cn/Article/details/gt2dkqhdjqh.html

csv.DictReader(f)
来源：http://www.52xcode.cn/Article/details/gt2xtfqrmjr.html

[U26] Py：并发下载
来源：http://www.ydjk.org.cn/Article/details/gt2aydlgfrp.html

ThreadPoolExecutor(max_workers=8).map(fetch, urls)
来源：http://www.52xcode.cn/Article/details/gt2ayidnnmr.html

[U27] Py：异步 HTTP
来源：http://www.ydjk.org.cn/Article/details/gt2pwnwyaqi.html

aiohttp.ClientSession() 配合 async with
来源：http://www.52xcode.cn/Article/details/gt2leyldnko.html

[U28] Py：类型别名
来源：http://www.ydjk.org.cn/Article/details/gt2nwqyoxed.html

UserId = int
来源：http://www.52xcode.cn/Article/details/gt2dyaertfw.html

[U29] Py：属性校验
来源：http://www.ydjk.org.cn/Article/details/gt2kfyydnsc.html

@property 与 @x.setter 配合
来源：http://www.ydjk.org.cn/Article/details/gt2kreovevf.html

[U30] Py：数据类
来源：http://www.52xcode.cn/Article/details/gt2ninmrvsq.html

@dataclass(slots=True)
来源：http://www.52xcode.cn/Article/details/gt2ibyrkbin.html

[U31] Py：单测
来源：http://www.ydjk.org.cn/Article/details/gt2msmnmxqv.html

python -m pytest -q
来源：http://www.ydjk.org.cn/Article/details/gt2oxqyingi.html

[U32] Py：代码格式化
来源：http://www.ydjk.org.cn/Article/details/gt2puwbacaa.html

ruff format . && ruff check --fix .
来源：http://www.52xcode.cn/Article/details/gt2bttqkurl.html

[U33] Py：打包发布
来源：http://www.ydjk.org.cn/Article/details/gt2usushyru.html

python -m build  （依赖 pyproject.toml）
来源：http://www.ydjk.org.cn/Article/details/gt2rsvwkghw.html

[U34] Py：判断编码
来源：http://www.52xcode.cn/Article/details/gt2kxfnqero.html

chardet.detect(raw)
来源：http://www.ydjk.org.cn/Article/details/gt2spoxxcnt.html

[U35] Py：发送邮件
来源：http://www.ydjk.org.cn/Article/details/gt2pgwwtczy.html

smtplib.SMTP_SSL(...).send_message(msg)
来源：http://www.52xcode.cn/Article/details/gt2rnxyehpf.html

[U36] Py：定时任务
来源：http://www.52xcode.cn/Article/details/gt2veuakach.html

schedule.every(10).minutes.do(job)
来源：http://www.52xcode.cn/Article/details/gt2pjcwfqml.html

[U37] Py：读写 Excel
来源：http://www.52xcode.cn/Article/details/gt2frxmkwxf.html

pandas.read_excel / DataFrame.to_excel
来源：http://www.52xcode.cn/Article/details/gt2wvmmbiii.html

[U38] Py：获取脚本所在目录
来源：http://www.52xcode.cn/Article/details/gt2jlbuvozk.html

Path(__file__).resolve().parent
来源：http://www.52xcode.cn/Article/details/gt2itnvtzut.html

[U39] Py：判断是否在交互环境
来源：http://www.ydjk.org.cn/Article/details/gt2cmluubqt.html

sys.stdout.isatty()
来源：http://www.ydjk.org.cn/Article/details/gt2oydsslap.html

[U40] Py：打印到标准错误
来源：http://www.ydjk.org.cn/Article/details/gt2gqdrfzsm.html

print("err", file=sys.stderr)
来源：http://www.52xcode.cn/Article/details/gt2oahavlkn.html

[U41] PHP：初始化 Composer 项目
来源：http://www.52xcode.cn/Article/details/gt2vkbfgvxl.html

composer init;  composer require guzzlehttp/guzzle
来源：http://www.ydjk.org.cn/Article/details/gt2enawveju.html

[U42] PHP：PSR-4 自动加载
来源：http://www.ydjk.org.cn/Article/details/gt2yhezbzth.html

"autoload": { "psr-4": { "App\\": "src/" } }
来源：http://www.52xcode.cn/Article/details/gt2xyynfyds.html

[U43] PHP：声明命名空间
来源：http://www.52xcode.cn/Article/details/gt2cdwafumc.html

namespace App\Http;
来源：http://www.ydjk.org.cn/Article/details/gt2vxugyucb.html

[U44] PHP：开启严格类型
来源：http://www.ydjk.org.cn/Article/details/gt2vwemxjas.html

declare(strict_types=1);
来源：http://www.ydjk.org.cn/Article/details/gt2farqcgnp.html

[U45] PHP：类型声明与返回类型
来源：http://www.ydjk.org.cn/Article/details/gt2nmewbkck.html

function add(int $a, int $b): int { return $a + $b; }
来源：http://www.ydjk.org.cn/Article/details/gt2lubovguu.html

[U46] PHP：可空类型
来源：http://www.ydjk.org.cn/Article/details/gt2cqayjvte.html

?string $name = null
来源：http://www.52xcode.cn/Article/details/gt2eltpmini.html

[U47] PHP：联合类型
来源：http://www.52xcode.cn/Article/details/gt2apqplfzz.html

int|string $id
来源：http://www.52xcode.cn/Article/details/gt2nukqxwaa.html

[U48] PHP：纯枚举
来源：http://www.52xcode.cn/Article/details/gt2fnskcwcp.html

enum Status: string { case Active = "active"; case Off = "off"; }
来源：http://www.ydjk.org.cn/Article/details/gt2paxcckib.html

[U49] PHP：只读属性
来源：http://www.ydjk.org.cn/Article/details/gt2netwynnn.html

public readonly string $name
来源：http://www.ydjk.org.cn/Article/details/gt2wkugihty.html

[U50] PHP：构造器属性提升
来源：http://www.52xcode.cn/Article/details/gt2fymvrydt.html

public function __construct(private int $id) {}
来源：http://www.52xcode.cn/Article/details/gt2ipjijwgq.html

[U51] PHP：数组解构
来源：http://www.ydjk.org.cn/Article/details/gt2vhisikdq.html

[$a, $b] = $arr;
来源：http://www.ydjk.org.cn/Article/details/gt2wbfiofeg.html

[U52] PHP：箭头函数
来源：http://www.52xcode.cn/Article/details/gt2sdqjksom.html

$double = fn($x) => $x * 2;
来源：http://www.52xcode.cn/Article/details/gt2bpgkownw.html

[U53] PHP：空合并运算符
来源：http://www.ydjk.org.cn/Article/details/gt2igbxpgxv.html

$v = $a ?? $b ?? "default";
来源：http://www.52xcode.cn/Article/details/gt2lsiuzhhx.html

[U54] PHP：空安全调用
来源：http://www.52xcode.cn/Article/details/gt2uxkdkmio.html

$obj?->method()
来源：http://www.52xcode.cn/Article/details/gt2bdpajhra.html

[U55] PHP：match 表达式
来源：http://www.ydjk.org.cn/Article/details/gt2zoxrzwpc.html

$s = match($x) { 1 => "一", default => "其他" };
来源：http://www.52xcode.cn/Article/details/gt2etxeaphz.html

[U56] PHP：命名参数
来源：http://www.52xcode.cn/Article/details/gt2oveawjwz.html

f(a: 1, b: 2)
来源：http://www.ydjk.org.cn/Article/details/gt2bcegmuru.html

[U57] PHP：字符串插值
来源：http://www.52xcode.cn/Article/details/gt2hehajlmb.html

"值: {$a}"
来源：http://www.52xcode.cn/Article/details/gt2lrwrbkxx.html

[U58] PHP：数组三件套
来源：http://www.ydjk.org.cn/Article/details/gt2wxaotrvo.html

array_map($f, $a);  array_filter($a, $f);  array_reduce($a, $f, 0);
来源：http://www.52xcode.cn/Article/details/gt2mhbdogid.html

[U59] PHP：自定义排序
来源：http://www.ydjk.org.cn/Article/details/gt2ukbtnhbr.html

usort($arr, fn($a, $b) => $a["age"] <=> $b["age"]);
来源：http://www.ydjk.org.cn/Article/details/gt2ymowryyn.html

[U60] PHP：JSON 编解码
来源：http://www.52xcode.cn/Article/details/gt2memgyfso.html

json_encode($d, JSON_UNESCAPED_UNICODE);  json_decode($s, true);
来源：http://www.52xcode.cn/Article/details/gt2dpcbbxed.html

[U61] PHP：正则
来源：http://www.52xcode.cn/Article/details/gt2nmzwxwpp.html

preg_match('/(\d+)/', $s, $m);  preg_replace('/\d+/', '#', $s);
来源：http://www.52xcode.cn/Article/details/gt2fbxnbyld.html

[U62] PHP：日期对象
来源：http://www.ydjk.org.cn/Article/details/gt2suboqyky.html

(new DateTimeImmutable())->format("Y-m-d");
来源：http://www.ydjk.org.cn/Article/details/gt2jkxjfvmf.html

[U63] PHP：文件读写
来源：http://www.52xcode.cn/Article/details/gt2fedkxkoz.html

file_get_contents($f);  file_put_contents($f, $data);
来源：http://www.52xcode.cn/Article/details/gt2rtklopmm.html

[U64] PHP：目录遍历
来源：http://www.52xcode.cn/Article/details/gt2umpdbdhl.html

glob("dir/*.php");  scandir("dir");
来源：http://www.ydjk.org.cn/Article/details/gt2ofhakmwb.html

[U65] PHP：会话
来源：http://www.ydjk.org.cn/Article/details/gt2easpjesh.html

session_start();  $_SESSION["uid"] = 1;
来源：http://www.52xcode.cn/Article/details/gt2qwvxdhsk.html

[U66] PHP：设置 Cookie
来源：http://www.52xcode.cn/Article/details/gt2qhwwblbl.html

setcookie("token", $v, ["httponly" => true, "samesite" => "Lax"]);
来源：http://www.ydjk.org.cn/Article/details/gt2tcitxygd.html

[U67] PHP：处理文件上传
来源：http://www.52xcode.cn/Article/details/gt2lweyvvzv.html

$_FILES["file"]["tmp_name"] 与 move_uploaded_file()
来源：http://www.ydjk.org.cn/Article/details/gt2ujmxmpum.html

[U68] PHP：PDO 连接
来源：http://www.52xcode.cn/Article/details/gt2mxglnsrc.html

$pdo = new PDO("mysql:host=localhost;dbname=app", "root", "");
来源：http://www.52xcode.cn/Article/details/gt2ttdqjaff.html

[U69] PHP：PDO 预处理
来源：http://www.ydjk.org.cn/Article/details/gt2wfgqhkip.html

$stmt = $pdo->prepare("SELECT * FROM users WHERE id = ?");  $stmt->execute([$id]);
来源：http://www.52xcode.cn/Article/details/gt2jieesrkt.html

[U70] PHP：PDO 事务
来源：http://www.52xcode.cn/Article/details/gt2illwafot.html

$pdo->beginTransaction();  $pdo->commit();  $pdo->rollBack();
来源：http://www.ydjk.org.cn/Article/details/gt2heowhpnr.html

[U71] PHP：抛出异常
来源：http://www.ydjk.org.cn/Article/details/gt2xwxnycie.html

throw new RuntimeException("失败", 500);
来源：http://www.52xcode.cn/Article/details/gt2lqneptqu.html

[U72] PHP：写错误日志
来源：http://www.52xcode.cn/Article/details/gt2lvwzxjrk.html

error_log("失败: " . $e->getMessage());
来源：http://www.52xcode.cn/Article/details/gt2pmpbwjnp.html

[U73] PHP：读取 ini 配置
来源：http://www.ydjk.org.cn/Article/details/gt2nvhyszij.html

parse_ini_file("config.ini", true)
来源：http://www.52xcode.cn/Article/details/gt2envqqrub.html

[U74] PHP：读取环境变量
来源：http://www.ydjk.org.cn/Article/details/gt2snpbdgct.html

getenv("APP_ENV") ?: "production"
来源：http://www.52xcode.cn/Article/details/gt2kcwaqbeb.html

[U75] PHP：依赖注入
来源：http://www.ydjk.org.cn/Article/details/gt2esmaxtws.html

composer require psr/container
来源：http://www.ydjk.org.cn/Article/details/gt2bjxmffqf.html

[U76] PHP：简单路由
来源：http://www.52xcode.cn/Article/details/gt2jbqhdfzz.html

$path = parse_url($_SERVER["REQUEST_URI"], PHP_URL_PATH);
来源：http://www.ydjk.org.cn/Article/details/gt2molwtwff.html

[U77] PHP：模板渲染
来源：http://www.52xcode.cn/Article/details/gt2bmgkgemn.html

composer require twig/twig
来源：http://www.52xcode.cn/Article/details/gt2ieldndcr.html

[U78] PHP：单元测试
来源：http://www.52xcode.cn/Article/details/gt2geotpieu.html

composer require --dev phpunit/phpunit
来源：http://www.52xcode.cn/Article/details/gt2lieymsvk.html

[U79] PHP：静态分析
来源：http://www.52xcode.cn/Article/details/gt2bqlvpdyd.html

composer require --dev phpstan/phpstan
来源：http://www.ydjk.org.cn/Article/details/gt2ausxujdr.html

[U80] PHP：代码规范修复
来源：http://www.52xcode.cn/Article/details/gt2phjxegsm.html

composer require --dev friendsofphp/php-cs-fixer
来源：http://www.ydjk.org.cn/Article/details/gt2rfmrptqr.html

[U81] JS：初始化项目
来源：http://www.ydjk.org.cn/Article/details/gt2wsayhjkj.html

npm init -y;  npm i express
来源：http://www.ydjk.org.cn/Article/details/gt2lysotrlz.html

[U82] JS：package.json 脚本
来源：http://www.52xcode.cn/Article/details/gt2qvnjdwsi.html

"scripts": { "dev": "vite", "build": "vite build" }
来源：http://www.52xcode.cn/Article/details/gt2eewvzjzx.html

[U83] JS：ES Module 导入导出
来源：http://www.ydjk.org.cn/Article/details/gt2htzbqeer.html

export const a = 1;  import { a } from "./m.js";
来源：http://www.ydjk.org.cn/Article/details/gt2whheuxno.html

[U84] JS：CommonJS 写法
来源：http://www.52xcode.cn/Article/details/gt2lwahsiwn.html

module.exports = { a };  const { a } = require("./m");
来源：http://www.ydjk.org.cn/Article/details/gt2erbwjupp.html

[U85] JS：可选链
来源：http://www.ydjk.org.cn/Article/details/gt2furxpafm.html

a?.b?.c
来源：http://www.52xcode.cn/Article/details/gt2qdoecukq.html

[U86] JS：空值合并
来源：http://www.52xcode.cn/Article/details/gt2rnuqlplw.html

a ?? b
来源：http://www.ydjk.org.cn/Article/details/gt2tocqexdl.html

[U87] JS：解构默认值
来源：http://www.52xcode.cn/Article/details/gt2xyabynml.html

const { a = 1, b = 2 } = obj;
来源：http://www.52xcode.cn/Article/details/gt2vusrukvr.html

[U88] JS：对象展开合并
来源：http://www.ydjk.org.cn/Article/details/gt2iqmwjdhz.html

{ ...a, ...b }
来源：http://www.ydjk.org.cn/Article/details/gt2knsnidic.html

[U89] JS：数组去重
来源：http://www.52xcode.cn/Article/details/gt2bewsnlsm.html

[...new Set(arr)]
来源：http://www.ydjk.org.cn/Article/details/gt2amdogzaa.html

[U90] JS：数字数组排序
来源：http://www.52xcode.cn/Article/details/gt2xpzlindc.html

[...arr].sort((a, b) => a - b)
来源：http://www.52xcode.cn/Article/details/gt2uanzbwjj.html

[U91] JS：对象键值遍历
来源：http://www.ydjk.org.cn/Article/details/gt2vllyqtln.html

Object.entries(obj).forEach(([k, v]) => {});
来源：http://www.ydjk.org.cn/Article/details/gt2cgbrzara.html

[U92] JS：深拷贝
来源：http://www.ydjk.org.cn/Article/details/gt2ghheueuf.html

structuredClone(obj)
来源：http://www.ydjk.org.cn/Article/details/gt2twgtkqpw.html

[U93] JS：模板字符串
来源：http://www.52xcode.cn/Article/details/gt2mpyxoebe.html

`共 ${n} 条`
来源：http://www.ydjk.org.cn/Article/details/gt2aykoqnwb.html

[U94] JS：箭头函数
来源：http://www.ydjk.org.cn/Article/details/gt2sswewzqp.html

const double = x => x * 2;
来源：http://www.52xcode.cn/Article/details/gt2sxhejjna.html

[U95] JS：Promise 包装
来源：http://www.52xcode.cn/Article/details/gt2wdilgihm.html

new Promise((resolve, reject) => {})
来源：http://www.52xcode.cn/Article/details/gt2jiekehvg.html

[U96] JS：async/await 与异常
来源：http://www.ydjk.org.cn/Article/details/gt2mnzlyuaw.html

try { const d = await f(); } catch (e) { console.error(e); }
来源：http://www.52xcode.cn/Article/details/gt2cxsnqhku.html

[U97] JS：并发请求
来源：http://www.52xcode.cn/Article/details/gt2ywxbnysl.html

await Promise.all(urls.map(u => fetch(u)))
来源：http://www.ydjk.org.cn/Article/details/gt2vksqtorv.html

[U98] JS：fetch 带 JSON
来源：http://www.ydjk.org.cn/Article/details/gt2atoktclp.html

await fetch(url, { method: "POST", headers: { "Content-Type": "application/json" }, body: JSON.stringify(d) })
来源：http://www.ydjk.org.cn/Article/details/gt2vngcdsnl.html

[U99] JS：事件监听
来源：http://www.ydjk.org.cn/Article/details/gt2gflxqaqm.html

el.addEventListener("click", e => {})
来源：http://www.52xcode.cn/Article/details/gt2fndjdylm.html

[U100] JS：DOM 查询
来源：http://www.52xcode.cn/Article/details/gt2zdgfmouz.html

document.querySelector(".item")
来源：http://www.ydjk.org.cn/Article/details/gt2bhzldgnj.html

[U101] JS：classList 操作
来源：http://www.52xcode.cn/Article/details/gt2yowouvhr.html

el.classList.toggle("active")
来源：http://www.52xcode.cn/Article/details/gt2rjzsnmou.html

[U102] JS：本地存储
来源：http://www.52xcode.cn/Article/details/gt2mwqyocnv.html

localStorage.setItem("k", JSON.stringify(v))
来源：http://www.52xcode.cn/Article/details/gt2jrbrrybk.html

[U103] JS：定时器
来源：http://www.ydjk.org.cn/Article/details/gt2mkuynmqu.html

setTimeout(fn, 1000);  setInterval(fn, 1000);
来源：http://www.52xcode.cn/Article/details/gt2rgngztch.html

[U104] JS：防抖
来源：http://www.ydjk.org.cn/Article/details/gt2lhmujyii.html

const debounce = (fn, ms) => { let t; return (...a) => { clearTimeout(t); t = setTimeout(() => fn(...a), ms); }; };
来源：http://www.52xcode.cn/Article/details/gt2xtkcywzi.html

[U105] JS：节流
来源：http://www.52xcode.cn/Article/details/gt2fmxpavun.html

const throttle = (fn, ms) => { let last = 0; return (...a) => { const n = Date.now(); if (n - last >= ms) { last = n; fn(...a); } }; };
来源：http://www.52xcode.cn/Article/details/gt2zscklxih.html

[U106] JS：日期格式化
来源：http://www.52xcode.cn/Article/details/gt2lopozzhp.html

new Intl.DateTimeFormat("zh-CN", { dateStyle: "medium" }).format(new Date())
来源：http://www.52xcode.cn/Article/details/gt2xcdowwav.html

[U107] JS：数字千分位
来源：http://www.52xcode.cn/Article/details/gt2ewkajpwd.html

new Intl.NumberFormat("en-US").format(1234567)
来源：http://www.52xcode.cn/Article/details/gt2skafdivs.html

[U108] JS：随机整数
来源：http://www.ydjk.org.cn/Article/details/gt2sjhyzcxd.html

Math.floor(Math.random() * (max - min + 1)) + min
来源：http://www.ydjk.org.cn/Article/details/gt2jraovhcs.html

[U109] JS：数组分组
来源：http://www.ydjk.org.cn/Article/details/gt2jfozlwpn.html

Object.groupBy(arr, x => x.type)
来源：http://www.ydjk.org.cn/Article/details/gt2exqtbkqd.html

[U110] JS：数组分块
来源：http://www.52xcode.cn/Article/details/gt2wcoixbth.html

arr.reduce((acc, x, i) => (i % size ? acc : [...acc, arr.slice(i, i + size)]), [])
来源：http://www.ydjk.org.cn/Article/details/gt2opwnwjdq.html

[U111] JS：对象转 Map
来源：http://www.52xcode.cn/Article/details/gt2oflsinjm.html

new Map(Object.entries(obj))
来源：http://www.ydjk.org.cn/Article/details/gt2noqtvjgj.html

[U112] JS：字符串补位
来源：http://www.ydjk.org.cn/Article/details/gt2iumkucss.html

"7".padStart(3, "0")
来源：http://www.ydjk.org.cn/Article/details/gt2mdpevsfg.html

[U113] JS：正则替换全部
来源：http://www.ydjk.org.cn/Article/details/gt2vnvnpdxj.html

s.replaceAll("a", "b")
来源：http://www.52xcode.cn/Article/details/gt2pcibnapx.html

[U114] JS：JSON 深比较
来源：http://www.52xcode.cn/Article/details/gt2jwsgtsah.html

JSON.stringify(a) === JSON.stringify(b)
来源：http://www.52xcode.cn/Article/details/gt2vlaqwlhb.html

[U115] JS：生成 UUID
来源：http://www.ydjk.org.cn/Article/details/gt2uviwomcy.html

crypto.randomUUID()
来源：http://www.ydjk.org.cn/Article/details/gt2gwrbvlpd.html

[U116] JS：类型检查（JSDoc）
来源：http://www.52xcode.cn/Article/details/gt2wbsqcnen.html

/** @param {string} name */ function f(name) {}
来源：http://www.ydjk.org.cn/Article/details/gt2pvkagcbl.html

[U117] JS：单元测试
来源：http://www.ydjk.org.cn/Article/details/gt2dbkqxhnh.html

npm i -D vitest;  npx vitest
来源：http://www.ydjk.org.cn/Article/details/gt2byuppmps.html

[U118] JS：开发服务器
来源：http://www.52xcode.cn/Article/details/gt2dwgcpuvd.html

npm i -D vite;  npx vite
来源：http://www.52xcode.cn/Article/details/gt2baqvqymv.html

[U119] JS：生产构建
来源：http://www.52xcode.cn/Article/details/gt2bxhoavjg.html

npx vite build
来源：http://www.ydjk.org.cn/Article/details/gt2oayeeoaz.html

[U120] JS：读取环境变量（Vite）
来源：http://www.52xcode.cn/Article/details/gt2vnnelwls.html

import.meta.env.VITE_API_URL
来源：http://www.ydjk.org.cn/Article/details/gt2saocaitw.html

================================================================================
来源：http://www.ydjk.org.cn/Article/details/gt2pwhwnpbh.html

统计汇总
来源：http://www.52xcode.cn/Article/details/gt2ebdeyczq.html

================================================================================
来源：http://www.52xcode.cn/Article/details/gt2jsuyenbp.html

按语言统计（条）：
来源：http://www.52xcode.cn/Article/details/gt2wzqykzin.html

Python ......... 252
来源：http://www.ydjk.org.cn/Article/details/gt2quvlqyrp.html

PHP ............ 252
来源：http://www.52xcode.cn/Article/details/gt2syymrsuj.html

JavaScript ..... 252
来源：http://www.ydjk.org.cn/Article/details/gt2hgurbjpd.html

TypeScript ..... 212
来源：http://www.52xcode.cn/Article/details/gt2wirqahox.html

Java ........... 212
来源：http://www.ydjk.org.cn/Article/details/gt2diozjdvo.html

Go ............. 212
来源：http://www.52xcode.cn/Article/details/gt2hvaxtxym.html

Ruby ........... 212
来源：http://www.52xcode.cn/Article/details/gt2rbkgbiio.html

C# ............. 212
来源：http://www.52xcode.cn/Article/details/gt2lgkzhyxa.html

C .............. 30
来源：http://www.ydjk.org.cn/Article/details/gt2ysqnjnby.html

C++ ............ 30
来源：http://www.ydjk.org.cn/Article/details/gt2fladattu.html

SQL ............ 90
来源：http://www.ydjk.org.cn/Article/details/gt2pbrteffj.html

Bash ........... 80
来源：http://www.ydjk.org.cn/Article/details/gt2feqbqubt.html

Kotlin ......... 15
来源：http://www.52xcode.cn/Article/details/gt2byejowxz.html

Swift .......... 15
来源：http://www.ydjk.org.cn/Article/details/gt2xszwsuff.html

Lua ............ 10
来源：http://www.52xcode.cn/Article/details/gt2dkicndvm.html

Perl ........... 10
来源：http://www.52xcode.cn/Article/details/gt2ouiljkia.html

Scala .......... 10
来源：http://www.ydjk.org.cn/Article/details/gt2rusaecxb.html

------------------------------------
来源：http://www.ydjk.org.cn/Article/details/gt2ipzlaavt.html

合计 ........... 2106 条
来源：http://www.ydjk.org.cn/Article/details/gt2uzekoled.html

按章节统计：
来源：http://www.52xcode.cn/Article/details/gt2tqjjgffd.html

A 基础语法与类型       26 个任务 × 8 语言 =  208
来源：http://www.ydjk.org.cn/Article/details/gt2dfyjndpf.html

B 流程控制             16 个任务 × 8 语言 =  128
来源：http://www.ydjk.org.cn/Article/details/gt2zbxcacdx.html

C 函数与作用域         16 个任务 × 8 语言 =  128
来源：http://www.ydjk.org.cn/Article/details/gt2ezcwikmf.html

D 数组 / 列表 / 集合   26 个任务 × 8 语言 =  208
来源：http://www.ydjk.org.cn/Article/details/gt2ifbpzpux.html

E 字符串处理           22 个任务 × 8 语言 =  176
来源：http://www.ydjk.org.cn/Article/details/gt2zrcyyruf.html

F 文件与目录           12 个任务 × 8 语言 =   96
来源：http://www.ydjk.org.cn/Article/details/gt2avtharxd.html

G 面向对象             16 个任务 × 8 语言 =  128
来源：http://www.52xcode.cn/Article/details/gt2syqcfzhj.html

H 异常与错误处理       10 个任务 × 8 语言 =   80
来源：http://www.ydjk.org.cn/Article/details/gt2xglthjfr.html

I 正则表达式            8 个任务 × 8 语言 =   64
来源：http://www.ydjk.org.cn/Article/details/gt2fvecoiyi.html

J 日期与时间           10 个任务 × 8 语言 =   80
来源：http://www.52xcode.cn/Article/details/gt2ytrbdpbj.html

K JSON 与序列化         8 个任务 × 8 语言 =   64
来源：http://www.ydjk.org.cn/Article/details/gt2fvvpimot.html

L 网络请求              8 个任务 × 8 语言 =   64
来源：http://www.52xcode.cn/Article/details/gt2rdvmxwga.html

M 命令行 / 进程         8 个任务 × 8 语言 =   64
来源：http://www.52xcode.cn/Article/details/gt2gpljwslo.html

N 数据结构与算法       12 个任务 × 8 语言 =   96
来源：http://www.52xcode.cn/Article/details/gt2ejlggyen.html

O 并发与异步            6 个任务 × 8 语言 =   48
来源：http://www.52xcode.cn/Article/details/gt2gzscdbtq.html

P 常用工具函数          8 个任务 × 8 语言 =   64
来源：http://www.52xcode.cn/Article/details/gt2caiieica.html

Q SQL 专题                              90
来源：http://www.ydjk.org.cn/Article/details/gt2vluyfjgz.html

R Bash 专题                             80
来源：http://www.52xcode.cn/Article/details/gt2kckltdrk.html

S C / C++ 专题                          60
来源：http://www.ydjk.org.cn/Article/details/gt2anrmburr.html

T 其他语言补充                          60
来源：http://www.52xcode.cn/Article/details/gt2zlcdknfq.html

U 高频实用片段                         120
来源：http://www.52xcode.cn/Article/details/gt2bmqjyuye.html

------------------------------------
来源：http://www.52xcode.cn/Article/details/gt2qfwbluvh.html

合计                                  2106 条
来源：http://www.52xcode.cn/Article/details/gt2uvlfrugj.html

--------------------------------------------------------------------------------
来源：http://www.52xcode.cn/Article/details/gt2ozrimmwn.html

使用提醒
来源：http://www.52xcode.cn/Article/details/gt2qtuaeevb.html

--------------------------------------------------------------------------------
来源：http://www.ydjk.org.cn/Article/details/gt2tkedfise.html

1. 示例追求"最小可用"，正式项目中请补齐导入、错误处理与边界判断。
来源：http://www.52xcode.cn/Article/details/gt2muwvwazn.html

2. 涉及文件、网络、数据库的示例，注意资源释放与异常捕获。
来源：http://www.52xcode.cn/Article/details/gt2llqlipjq.html

3. 语言版本差异较大（如 Python 3.10 的 match、Java 17 的 record/switch 箭头），
来源：http://www.ydjk.org.cn/Article/details/gt2zwsxvprq.html

在旧版本上使用前请先确认语法支持情况。
来源：http://www.52xcode.cn/Article/details/gt2fbnvhbvk.html

4. 标注"手写"的条目是因为该语言缺少对应内置能力，实际项目中可引入成熟库。
来源：http://www.52xcode.cn/Article/details/gt2zcxpstxe.html

—— 文件结束 ——
来源：http://www.52xcode.cn/Article/details/gt2wvbcaaxz.html

================================================================================
来源：http://www.ydjk.org.cn/Article/details/gt2cexkbcat.html

程序语言常见例子速查手册（2024 版）
来源：http://www.ydjk.org.cn/Article/details/gt2vespzbqp.html

Common Programming Examples Cheat Book
来源：http://www.52xcode.cn/Article/details/gt2xgaxgwzg.html

================================================================================
来源：http://www.52xcode.cn/Article/details/gt2fatbsvtp.html

【收录内容】
来源：http://www.ydjk.org.cn/Article/details/gt2whknuvgo.html

覆盖 12 种语言 / 语法与常见 API：
来源：http://www.52xcode.cn/Article/details/gt2uuhlvysh.html

Python · PHP · JavaScript · TypeScript · Java · Go · Ruby · C#
来源：http://www.52xcode.cn/Article/details/gt2hwjifeyy.html

SQL · Bash · C · C++
来源：http://www.52xcode.cn/Article/details/gt2zldcbwgi.html

按「任务」分组：每个任务下按语言各给出一条最小可用示例。
来源：http://www.ydjk.org.cn/Article/details/gt2ayclfwkd.html

【使用说明】
来源：http://www.52xcode.cn/Article/details/gt2lpywlvay.html

1. 每个任务形如 "[编号] 任务名"，下面每行以语言标记开头：
来源：http://www.ydjk.org.cn/Article/details/gt2sauznbmt.html

Py:    Python        PHP:   PHP           JS:    JavaScript
来源：http://www.52xcode.cn/Article/details/gt2viyuvdlo.html

TS:    TypeScript    Java:  Java          Go:    Go
来源：http://www.52xcode.cn/Article/details/gt2hylhpisl.html

Ruby:  Ruby          C#:    C#            SQL:   SQL
来源：http://www.52xcode.cn/Article/details/gt2rlsaerzh.html

Bash:  Shell         C:     C             C++:   C++
来源：http://www.52xcode.cn/Article/details/gt2uyarowyr.html

2. 示例只展示核心写法，刻意省略 import / require / include / using 等样板代码。
来源：http://www.ydjk.org.cn/Article/details/gt2eodtpmps.html

需要完整可运行文件时，请自行补齐当前语言的导入语句。
来源：http://www.ydjk.org.cn/Article/details/gt2dvfduwgw.html

3. 语法基准：Python 3.10+ / PHP 8.1+ / ES2020+ / TypeScript 5 / Java 17 /
来源：http://www.52xcode.cn/Article/details/gt2bmowagrf.html

Go 1.21+ / Ruby 3.x / C# 10+ / C17 / C++17。
来源：http://www.ydjk.org.cn/Article/details/gt2odfiised.html

4. 检索建议：用编辑器或浏览器 Ctrl+F 搜关键词，如 "排序" "读取文件" "正则"。
来源：http://www.52xcode.cn/Article/details/gt2sixzzypw.html

5. 标记为 "// 无" 表示该语言没有对应的一等语法，需用替代写法（示例给出替代方案）。
来源：http://www.ydjk.org.cn/Article/details/gt2ffwdipee.html

6. 符号 "⏎" 表示代码在此处换行（主要用于 Python 等强制缩进、无法压成一行的结构）。
来源：http://www.52xcode.cn/Article/details/gt2rgfhfexr.html

【文件统计】
来源：http://www.52xcode.cn/Article/details/gt2lghxjamt.html

语言示例共 2106 条，分布见本文末尾的「统计汇总」。
来源：http://www.ydjk.org.cn/Article/details/gt2vpmldkjo.html

--------------------------------------------------------------------------------
来源：http://www.ydjk.org.cn/Article/details/gt2vzwfwphm.html

目  录
来源：http://www.ydjk.org.cn/Article/details/gt2fvdfqcvl.html

--------------------------------------------------------------------------------
来源：http://www.52xcode.cn/Article/details/gt2bmczdzes.html

A. 基础语法与类型              （第 1 节，26 个任务，208 条）
来源：http://www.52xcode.cn/Article/details/gt2vmtxvqpy.html

B. 流程控制                    （第 2 节，16 个任务，128 条）
来源：http://www.52xcode.cn/Article/details/gt2utcuxlua.html

C. 函数与作用域                （第 3 节，16 个任务，128 条）
来源：http://www.52xcode.cn/Article/details/gt2sbxywgpy.html

D. 数组 / 列表 / 集合          （第 4 节，26 个任务，208 条）
来源：http://www.ydjk.org.cn/Article/details/gt2shlxdcgl.html

E. 字符串处理                  （第 5 节，22 个任务，176 条）
来源：http://www.ydjk.org.cn/Article/details/gt2szisxrox.html

F. 文件与目录                  （第 6 节，12 个任务，96 条）
来源：http://www.ydjk.org.cn/Article/details/gt2jfcydpdm.html

G. 面向对象                    （第 7 节，16 个任务，128 条）
来源：http://www.ydjk.org.cn/Article/details/gt2oiatgxmp.html

H. 异常与错误处理              （第 8 节，10 个任务，80 条）
来源：http://www.ydjk.org.cn/Article/details/gt2lfpprbhg.html

I. 正则表达式                  （第 9 节，8 个任务，64 条）
来源：http://www.52xcode.cn/Article/details/gt2ctzlcspp.html

J. 日期与时间                  （第 10 节，10 个任务，80 条）
来源：http://www.ydjk.org.cn/Article/details/gt2cereihjo.html

K. JSON 与序列化               （第 11 节，8 个任务，64 条）
来源：http://www.ydjk.org.cn/Article/details/gt2fczsoiqo.html

L. 网络请求                    （第 12 节，8 个任务，64 条）
来源：http://www.ydjk.org.cn/Article/details/gt2kgtpqoiu.html

M. 命令行 / 进程 / 环境        （第 13 节，8 个任务，64 条）
来源：http://www.52xcode.cn/Article/details/gt2akaoyceq.html


<!-- 参考信息 -->