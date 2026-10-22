代发 wailian999

[U25] Py：CSV 按字典读
来源：http://www.ydjk.org.cn/Article/details/gt2dyexjxda.html

csv.DictReader(f)
来源：http://www.ydjk.org.cn/Article/details/gt2khelggzp.html

[U26] Py：并发下载
来源：http://www.ydjk.org.cn/Article/details/gt2hybigfdt.html

ThreadPoolExecutor(max_workers=8).map(fetch, urls)
来源：http://www.52xcode.cn/Article/details/gt2odrhsmge.html

[U27] Py：异步 HTTP
来源：http://www.ydjk.org.cn/Article/details/gt2jvtdbmyt.html

aiohttp.ClientSession() 配合 async with
来源：http://www.ydjk.org.cn/Article/details/gt2kofseluc.html

[U28] Py：类型别名
来源：http://www.52xcode.cn/Article/details/gt2egxaqdsd.html

UserId = int
来源：http://www.52xcode.cn/Article/details/gt2sxbahwyc.html

[U29] Py：属性校验
来源：http://www.52xcode.cn/Article/details/gt2hmeuvtye.html

@property 与 @x.setter 配合
来源：http://www.ydjk.org.cn/Article/details/gt2rrpyqbuj.html

[U30] Py：数据类
来源：http://www.52xcode.cn/Article/details/gt2ciopjctc.html

@dataclass(slots=True)
来源：http://www.52xcode.cn/Article/details/gt2gnnxieil.html

[U31] Py：单测
来源：http://www.52xcode.cn/Article/details/gt2tdjlvyjg.html

python -m pytest -q
来源：http://www.ydjk.org.cn/Article/details/gt2rmhsqbnq.html

[U32] Py：代码格式化
来源：http://www.52xcode.cn/Article/details/gt2invzuznl.html

ruff format . && ruff check --fix .
来源：http://www.ydjk.org.cn/Article/details/gt2eygsstqk.html

[U33] Py：打包发布
来源：http://www.ydjk.org.cn/Article/details/gt2zaqubhrr.html

python -m build  （依赖 pyproject.toml）
来源：http://www.52xcode.cn/Article/details/gt2cxoorezv.html

[U34] Py：判断编码
来源：http://www.52xcode.cn/Article/details/gt2xaqnoxra.html

chardet.detect(raw)
来源：http://www.ydjk.org.cn/Article/details/gt2tgjqgdwd.html

[U35] Py：发送邮件
来源：http://www.52xcode.cn/Article/details/gt2yqxhxtxo.html

smtplib.SMTP_SSL(...).send_message(msg)
来源：http://www.52xcode.cn/Article/details/gt2breelepq.html

[U36] Py：定时任务
来源：http://www.ydjk.org.cn/Article/details/gt2zdniaten.html

schedule.every(10).minutes.do(job)
来源：http://www.52xcode.cn/Article/details/gt2hrwgxbji.html

[U37] Py：读写 Excel
来源：http://www.52xcode.cn/Article/details/gt2hscnupzm.html

pandas.read_excel / DataFrame.to_excel
来源：http://www.52xcode.cn/Article/details/gt2mmvqnvkm.html

[U38] Py：获取脚本所在目录
来源：http://www.ydjk.org.cn/Article/details/gt2zaomozpp.html

Path(__file__).resolve().parent
来源：http://www.52xcode.cn/Article/details/gt2dzashbyo.html

[U39] Py：判断是否在交互环境
来源：http://www.52xcode.cn/Article/details/gt2bqtztqvd.html

sys.stdout.isatty()
来源：http://www.52xcode.cn/Article/details/gt2ulobmeob.html

[U40] Py：打印到标准错误
来源：http://www.ydjk.org.cn/Article/details/gt2uqkjbqtn.html

print("err", file=sys.stderr)
来源：http://www.ydjk.org.cn/Article/details/gt2usnpzfml.html

[U41] PHP：初始化 Composer 项目
来源：http://www.ydjk.org.cn/Article/details/gt2psvvasbn.html

composer init;  composer require guzzlehttp/guzzle
来源：http://www.52xcode.cn/Article/details/gt2yemstdtr.html

[U42] PHP：PSR-4 自动加载
来源：http://www.52xcode.cn/Article/details/gt2nhxgfbkl.html

"autoload": { "psr-4": { "App\\": "src/" } }
来源：http://www.ydjk.org.cn/Article/details/gt2cijqnsrl.html

[U43] PHP：声明命名空间
来源：http://www.52xcode.cn/Article/details/gt2kzcmmawx.html

namespace App\Http;
来源：http://www.ydjk.org.cn/Article/details/gt2uxxpiqmd.html

[U44] PHP：开启严格类型
来源：http://www.ydjk.org.cn/Article/details/gt2jhcpbixx.html

declare(strict_types=1);
来源：http://www.ydjk.org.cn/Article/details/gt2jxhsnjoc.html

[U45] PHP：类型声明与返回类型
来源：http://www.52xcode.cn/Article/details/gt2nzcjrqbn.html

function add(int $a, int $b): int { return $a + $b; }
来源：http://www.ydjk.org.cn/Article/details/gt2iwzbunlb.html

[U46] PHP：可空类型
来源：http://www.ydjk.org.cn/Article/details/gt2hsenjbpb.html

?string $name = null
来源：http://www.52xcode.cn/Article/details/gt2kbfhwkho.html

[U47] PHP：联合类型
来源：http://www.ydjk.org.cn/Article/details/gt2vgszskmd.html

int|string $id
来源：http://www.ydjk.org.cn/Article/details/gt2hgcwthbd.html

[U48] PHP：纯枚举
来源：http://www.52xcode.cn/Article/details/gt2rnksefhf.html

enum Status: string { case Active = "active"; case Off = "off"; }
来源：http://www.ydjk.org.cn/Article/details/gt2wrupsnkh.html

[U49] PHP：只读属性
来源：http://www.52xcode.cn/Article/details/gt2lzqegeqp.html

public readonly string $name
来源：http://www.52xcode.cn/Article/details/gt2uvibetko.html

[U50] PHP：构造器属性提升
来源：http://www.ydjk.org.cn/Article/details/gt2snzzkclh.html

public function __construct(private int $id) {}
来源：http://www.52xcode.cn/Article/details/gt2hfqckhwz.html

[U51] PHP：数组解构
来源：http://www.52xcode.cn/Article/details/gt2owszzjza.html

[$a, $b] = $arr;
来源：http://www.52xcode.cn/Article/details/gt2dzlmdgdo.html

[U52] PHP：箭头函数
来源：http://www.52xcode.cn/Article/details/gt2izitfwzt.html

$double = fn($x) => $x * 2;
来源：http://www.52xcode.cn/Article/details/gt2csvgwzsa.html

[U53] PHP：空合并运算符
来源：http://www.ydjk.org.cn/Article/details/gt2cflwqgnu.html

$v = $a ?? $b ?? "default";
来源：http://www.ydjk.org.cn/Article/details/gt2eqlwcysc.html

[U54] PHP：空安全调用
来源：http://www.52xcode.cn/Article/details/gt2dzlfocyk.html

$obj?->method()
来源：http://www.ydjk.org.cn/Article/details/gt2rjkngvtq.html

[U55] PHP：match 表达式
来源：http://www.ydjk.org.cn/Article/details/gt2ohhbgsgq.html

$s = match($x) { 1 => "一", default => "其他" };
来源：http://www.52xcode.cn/Article/details/gt2bmufahgj.html

[U56] PHP：命名参数
来源：http://www.52xcode.cn/Article/details/gt2ryndvmcx.html

f(a: 1, b: 2)
来源：http://www.ydjk.org.cn/Article/details/gt2jgkxmoiy.html

[U57] PHP：字符串插值
来源：http://www.ydjk.org.cn/Article/details/gt2hpwcmcju.html

"值: {$a}"
来源：http://www.52xcode.cn/Article/details/gt2pqtambum.html

[U58] PHP：数组三件套
来源：http://www.52xcode.cn/Article/details/gt2toobqvev.html

array_map($f, $a);  array_filter($a, $f);  array_reduce($a, $f, 0);
来源：http://www.ydjk.org.cn/Article/details/gt2jrumqgtm.html

[U59] PHP：自定义排序
来源：http://www.ydjk.org.cn/Article/details/gt2ebgfppzh.html

usort($arr, fn($a, $b) => $a["age"] <=> $b["age"]);
来源：http://www.ydjk.org.cn/Article/details/gt2twyvdizv.html

[U60] PHP：JSON 编解码
来源：http://www.52xcode.cn/Article/details/gt2twcavpys.html

json_encode($d, JSON_UNESCAPED_UNICODE);  json_decode($s, true);
来源：http://www.52xcode.cn/Article/details/gt2mgzdnjin.html

[U61] PHP：正则
来源：http://www.ydjk.org.cn/Article/details/gt2ulrprrtx.html

preg_match('/(\d+)/', $s, $m);  preg_replace('/\d+/', '#', $s);
来源：http://www.ydjk.org.cn/Article/details/gt2vfavhurt.html

[U62] PHP：日期对象
来源：http://www.52xcode.cn/Article/details/gt2ifutyhrs.html

(new DateTimeImmutable())->format("Y-m-d");
来源：http://www.52xcode.cn/Article/details/gt2tuorgary.html

[U63] PHP：文件读写
来源：http://www.52xcode.cn/Article/details/gt2haekzuxj.html

file_get_contents($f);  file_put_contents($f, $data);
来源：http://www.52xcode.cn/Article/details/gt2xrspinsz.html

[U64] PHP：目录遍历
来源：http://www.52xcode.cn/Article/details/gt2mmqbonwa.html

glob("dir/*.php");  scandir("dir");
来源：http://www.52xcode.cn/Article/details/gt2ynzsckyl.html

[U65] PHP：会话
来源：http://www.52xcode.cn/Article/details/gt2cqciagng.html

session_start();  $_SESSION["uid"] = 1;
来源：http://www.52xcode.cn/Article/details/gt2bnpfsvfz.html

[U66] PHP：设置 Cookie
来源：http://www.ydjk.org.cn/Article/details/gt2prwsanfu.html

setcookie("token", $v, ["httponly" => true, "samesite" => "Lax"]);
来源：http://www.ydjk.org.cn/Article/details/gt2dxdqvana.html

[U67] PHP：处理文件上传
来源：http://www.ydjk.org.cn/Article/details/gt2htonapxq.html

$_FILES["file"]["tmp_name"] 与 move_uploaded_file()
来源：http://www.52xcode.cn/Article/details/gt2rnhkkdtb.html

[U68] PHP：PDO 连接
来源：http://www.52xcode.cn/Article/details/gt2krhzhegr.html

$pdo = new PDO("mysql:host=localhost;dbname=app", "root", "");
来源：http://www.ydjk.org.cn/Article/details/gt2jhxfgbsa.html

[U69] PHP：PDO 预处理
来源：http://www.52xcode.cn/Article/details/gt2iigwcada.html

$stmt = $pdo->prepare("SELECT * FROM users WHERE id = ?");  $stmt->execute([$id]);
来源：http://www.52xcode.cn/Article/details/gt2kocskmrr.html

[U70] PHP：PDO 事务
来源：http://www.52xcode.cn/Article/details/gt2kssgxbin.html

$pdo->beginTransaction();  $pdo->commit();  $pdo->rollBack();
来源：http://www.52xcode.cn/Article/details/gt2faiplafm.html

[U71] PHP：抛出异常
来源：http://www.52xcode.cn/Article/details/gt2rbunwxsb.html

throw new RuntimeException("失败", 500);
来源：http://www.52xcode.cn/Article/details/gt2yjqxzrzw.html

[U72] PHP：写错误日志
来源：http://www.52xcode.cn/Article/details/gt2lnocudmd.html

error_log("失败: " . $e->getMessage());
来源：http://www.52xcode.cn/Article/details/gt2faacfraa.html

[U73] PHP：读取 ini 配置
来源：http://www.ydjk.org.cn/Article/details/gt2qhacjxis.html

parse_ini_file("config.ini", true)
来源：http://www.52xcode.cn/Article/details/gt2gprenels.html

[U74] PHP：读取环境变量
来源：http://www.52xcode.cn/Article/details/gt2flmbaolf.html

getenv("APP_ENV") ?: "production"
来源：http://www.ydjk.org.cn/Article/details/gt2lohldmgv.html

[U75] PHP：依赖注入
来源：http://www.ydjk.org.cn/Article/details/gt2cdnknkna.html

composer require psr/container
来源：http://www.ydjk.org.cn/Article/details/gt2kckixzhm.html

[U76] PHP：简单路由
来源：http://www.52xcode.cn/Article/details/gt2nwhckfgn.html

$path = parse_url($_SERVER["REQUEST_URI"], PHP_URL_PATH);
来源：http://www.ydjk.org.cn/Article/details/gt2mkinsrbk.html

[U77] PHP：模板渲染
来源：http://www.52xcode.cn/Article/details/gt2boczhadd.html

composer require twig/twig
来源：http://www.ydjk.org.cn/Article/details/gt2cjnzlyqf.html

[U78] PHP：单元测试
来源：http://www.52xcode.cn/Article/details/gt2zyvkismg.html

composer require --dev phpunit/phpunit
来源：http://www.ydjk.org.cn/Article/details/gt2ugwyoomx.html

[U79] PHP：静态分析
来源：http://www.52xcode.cn/Article/details/gt2hxlppcxh.html

composer require --dev phpstan/phpstan
来源：http://www.52xcode.cn/Article/details/gt2sltrklnp.html

[U80] PHP：代码规范修复
来源：http://www.52xcode.cn/Article/details/gt2xpjtpekb.html

composer require --dev friendsofphp/php-cs-fixer
来源：http://www.ydjk.org.cn/Article/details/gt2xrlblhxd.html

[U81] JS：初始化项目
来源：http://www.ydjk.org.cn/Article/details/gt2roosmeti.html

npm init -y;  npm i express
来源：http://www.52xcode.cn/Article/details/gt2ebfrzjgp.html

[U82] JS：package.json 脚本
来源：http://www.52xcode.cn/Article/details/gt2hswmsfob.html

"scripts": { "dev": "vite", "build": "vite build" }
来源：http://www.ydjk.org.cn/Article/details/gt2jbynmbsd.html

[U83] JS：ES Module 导入导出
来源：http://www.ydjk.org.cn/Article/details/gt2nzmrmksx.html

export const a = 1;  import { a } from "./m.js";
来源：http://www.52xcode.cn/Article/details/gt2buaftoxt.html

[U84] JS：CommonJS 写法
来源：http://www.ydjk.org.cn/Article/details/gt2vaigygkh.html

module.exports = { a };  const { a } = require("./m");
来源：http://www.ydjk.org.cn/Article/details/gt2odshrstq.html

[U85] JS：可选链
来源：http://www.ydjk.org.cn/Article/details/gt2gppetazu.html

a?.b?.c
来源：http://www.ydjk.org.cn/Article/details/gt2srgretug.html

[U86] JS：空值合并
来源：http://www.52xcode.cn/Article/details/gt2phmpfbra.html

a ?? b
来源：http://www.52xcode.cn/Article/details/gt2npccqdqe.html

[U87] JS：解构默认值
来源：http://www.ydjk.org.cn/Article/details/gt2qwfbhqts.html

const { a = 1, b = 2 } = obj;
来源：http://www.ydjk.org.cn/Article/details/gt2sgvctthr.html

[U88] JS：对象展开合并
来源：http://www.ydjk.org.cn/Article/details/gt2qaxfevkw.html

{ ...a, ...b }
来源：http://www.52xcode.cn/Article/details/gt2gsgzxzyn.html

[U89] JS：数组去重
来源：http://www.ydjk.org.cn/Article/details/gt2vtmvaekb.html

[...new Set(arr)]
来源：http://www.ydjk.org.cn/Article/details/gt2nqgervps.html

[U90] JS：数字数组排序
来源：http://www.ydjk.org.cn/Article/details/gt2dgbbkdar.html

[...arr].sort((a, b) => a - b)
来源：http://www.52xcode.cn/Article/details/gt2kxebtzpb.html

[U91] JS：对象键值遍历
来源：http://www.52xcode.cn/Article/details/gt2shjfiusv.html

Object.entries(obj).forEach(([k, v]) => {});
来源：http://www.ydjk.org.cn/Article/details/gt2palpuwwz.html

[U92] JS：深拷贝
来源：http://www.52xcode.cn/Article/details/gt2iofystkx.html

structuredClone(obj)
来源：http://www.ydjk.org.cn/Article/details/gt2mgfgfcyw.html

[U93] JS：模板字符串
来源：http://www.ydjk.org.cn/Article/details/gt2atconmvr.html

`共 ${n} 条`
来源：http://www.52xcode.cn/Article/details/gt2tevxebzp.html

[U94] JS：箭头函数
来源：http://www.ydjk.org.cn/Article/details/gt2lzixenug.html

const double = x => x * 2;
来源：http://www.52xcode.cn/Article/details/gt2aawytiog.html

[U95] JS：Promise 包装
来源：http://www.ydjk.org.cn/Article/details/gt2yaicvgik.html

new Promise((resolve, reject) => {})
来源：http://www.52xcode.cn/Article/details/gt2vsdxegms.html

[U96] JS：async/await 与异常
来源：http://www.52xcode.cn/Article/details/gt2cbukrkid.html

try { const d = await f(); } catch (e) { console.error(e); }
来源：http://www.52xcode.cn/Article/details/gt2jlknokbk.html

[U97] JS：并发请求
来源：http://www.52xcode.cn/Article/details/gt2nmfozmym.html

await Promise.all(urls.map(u => fetch(u)))
来源：http://www.ydjk.org.cn/Article/details/gt2ovyhnkmg.html

[U98] JS：fetch 带 JSON
来源：http://www.52xcode.cn/Article/details/gt2qtrcvpcw.html

await fetch(url, { method: "POST", headers: { "Content-Type": "application/json" }, body: JSON.stringify(d) })
来源：http://www.52xcode.cn/Article/details/gt2vnupzmoc.html

[U99] JS：事件监听
来源：http://www.ydjk.org.cn/Article/details/gt2tiaeorik.html

el.addEventListener("click", e => {})
来源：http://www.52xcode.cn/Article/details/gt2gbvudsub.html

[U100] JS：DOM 查询
来源：http://www.ydjk.org.cn/Article/details/gt2unjhprss.html

document.querySelector(".item")
来源：http://www.52xcode.cn/Article/details/gt2focfllbn.html

[U101] JS：classList 操作
来源：http://www.52xcode.cn/Article/details/gt2voinvdyb.html

el.classList.toggle("active")
来源：http://www.52xcode.cn/Article/details/gt2ivqcwpge.html

[U102] JS：本地存储
来源：http://www.52xcode.cn/Article/details/gt2hhrslpcv.html

localStorage.setItem("k", JSON.stringify(v))
来源：http://www.ydjk.org.cn/Article/details/gt2jnbmunkj.html

[U103] JS：定时器
来源：http://www.ydjk.org.cn/Article/details/gt2bsqszxbe.html

setTimeout(fn, 1000);  setInterval(fn, 1000);
来源：http://www.52xcode.cn/Article/details/gt2gjvwefja.html

[U104] JS：防抖
来源：http://www.ydjk.org.cn/Article/details/gt2iidatats.html

const debounce = (fn, ms) => { let t; return (...a) => { clearTimeout(t); t = setTimeout(() => fn(...a), ms); }; };
来源：http://www.ydjk.org.cn/Article/details/gt2xxgdtfag.html

[U105] JS：节流
来源：http://www.52xcode.cn/Article/details/gt2yqntrusw.html

const throttle = (fn, ms) => { let last = 0; return (...a) => { const n = Date.now(); if (n - last >= ms) { last = n; fn(...a); } }; };
来源：http://www.ydjk.org.cn/Article/details/gt2rwrfsces.html

[U106] JS：日期格式化
来源：http://www.ydjk.org.cn/Article/details/gt2uqxjvcou.html

new Intl.DateTimeFormat("zh-CN", { dateStyle: "medium" }).format(new Date())
来源：http://www.ydjk.org.cn/Article/details/gt2psvfrxaz.html

[U107] JS：数字千分位
来源：http://www.ydjk.org.cn/Article/details/gt2pldqjubs.html

new Intl.NumberFormat("en-US").format(1234567)
来源：http://www.52xcode.cn/Article/details/gt2rjfqpduo.html

[U108] JS：随机整数
来源：http://www.ydjk.org.cn/Article/details/gt2wfhmrgav.html

Math.floor(Math.random() * (max - min + 1)) + min
来源：http://www.52xcode.cn/Article/details/gt2xfxcfcjb.html

[U109] JS：数组分组
来源：http://www.ydjk.org.cn/Article/details/gt2fgpkptzr.html

Object.groupBy(arr, x => x.type)
来源：http://www.ydjk.org.cn/Article/details/gt2nyoywsso.html

[U110] JS：数组分块
来源：http://www.ydjk.org.cn/Article/details/gt2yjpmksgl.html

arr.reduce((acc, x, i) => (i % size ? acc : [...acc, arr.slice(i, i + size)]), [])
来源：http://www.ydjk.org.cn/Article/details/gt2cvjjwoah.html

[U111] JS：对象转 Map
来源：http://www.ydjk.org.cn/Article/details/gt2jsqgnhyb.html

new Map(Object.entries(obj))
来源：http://www.ydjk.org.cn/Article/details/gt2znellqbx.html

[U112] JS：字符串补位
来源：http://www.ydjk.org.cn/Article/details/gt2tueascxi.html

"7".padStart(3, "0")
来源：http://www.52xcode.cn/Article/details/gt2cnlcwnbl.html

[U113] JS：正则替换全部
来源：http://www.52xcode.cn/Article/details/gt2smezclkv.html

s.replaceAll("a", "b")
来源：http://www.52xcode.cn/Article/details/gt2avdgkirp.html

[U114] JS：JSON 深比较
来源：http://www.ydjk.org.cn/Article/details/gt2rjsxxwpd.html

JSON.stringify(a) === JSON.stringify(b)
来源：http://www.ydjk.org.cn/Article/details/gt2bgflkyok.html

[U115] JS：生成 UUID
来源：http://www.ydjk.org.cn/Article/details/gt2lxwsaiuk.html

crypto.randomUUID()
来源：http://www.52xcode.cn/Article/details/gt2wrwirxut.html

[U116] JS：类型检查（JSDoc）
来源：http://www.ydjk.org.cn/Article/details/gt2buugccvh.html

/** @param {string} name */ function f(name) {}
来源：http://www.ydjk.org.cn/Article/details/gt2jyvsijyq.html

[U117] JS：单元测试
来源：http://www.ydjk.org.cn/Article/details/gt2owguszqo.html

npm i -D vitest;  npx vitest
来源：http://www.ydjk.org.cn/Article/details/gt2flnsotew.html

[U118] JS：开发服务器
来源：http://www.ydjk.org.cn/Article/details/gt2nelacqqj.html

npm i -D vite;  npx vite
来源：http://www.52xcode.cn/Article/details/gt2voxjupqh.html

[U119] JS：生产构建
来源：http://www.52xcode.cn/Article/details/gt2cjlvxbkw.html

npx vite build
来源：http://www.ydjk.org.cn/Article/details/gt2ehfihyyq.html

[U120] JS：读取环境变量（Vite）
来源：http://www.52xcode.cn/Article/details/gt2egdbtoaw.html

import.meta.env.VITE_API_URL
来源：http://www.52xcode.cn/Article/details/gt2ubehpsod.html

================================================================================
来源：http://www.52xcode.cn/Article/details/gt2kwtrgljh.html

统计汇总
来源：http://www.ydjk.org.cn/Article/details/gt2lthigzif.html

================================================================================
来源：http://www.52xcode.cn/Article/details/gt2nbypcdzy.html

按语言统计（条）：
来源：http://www.ydjk.org.cn/Article/details/gt2uqrlfcth.html

Python ......... 252
来源：http://www.52xcode.cn/Article/details/gt2bijbvjfe.html

PHP ............ 252
来源：http://www.52xcode.cn/Article/details/gt2lxgwadvx.html

JavaScript ..... 252
来源：http://www.52xcode.cn/Article/details/gt2xzobxkrb.html

TypeScript ..... 212
来源：http://www.52xcode.cn/Article/details/gt2kivsymsy.html

Java ........... 212
来源：http://www.52xcode.cn/Article/details/gt2keezorbo.html

Go ............. 212
来源：http://www.52xcode.cn/Article/details/gt2lfzcsvun.html

Ruby ........... 212
来源：http://www.52xcode.cn/Article/details/gt2funuxsjv.html

C# ............. 212
来源：http://www.52xcode.cn/Article/details/gt2uehxvaqz.html

C .............. 30
来源：http://www.ydjk.org.cn/Article/details/gt2gmrzgbnk.html

C++ ............ 30
来源：http://www.ydjk.org.cn/Article/details/gt2dibmimxr.html

SQL ............ 90
来源：http://www.ydjk.org.cn/Article/details/gt2tdwpdpwa.html

Bash ........... 80
来源：http://www.ydjk.org.cn/Article/details/gt2zisxdagi.html

Kotlin ......... 15
来源：http://www.ydjk.org.cn/Article/details/gt2rixcrpjt.html

Swift .......... 15
来源：http://www.ydjk.org.cn/Article/details/gt2ukxjtzai.html

Lua ............ 10
来源：http://www.52xcode.cn/Article/details/gt2iznlczmp.html

Perl ........... 10
来源：http://www.52xcode.cn/Article/details/gt2fxvmoopb.html

Scala .......... 10
来源：http://www.ydjk.org.cn/Article/details/gt2eokzzmiz.html

------------------------------------
来源：http://www.52xcode.cn/Article/details/gt2lmmidvpc.html

合计 ........... 2106 条
来源：http://www.ydjk.org.cn/Article/details/gt2awmhseyk.html

按章节统计：
来源：http://www.ydjk.org.cn/Article/details/gt2botbxrqb.html

A 基础语法与类型       26 个任务 × 8 语言 =  208
来源：http://www.ydjk.org.cn/Article/details/gt2gbryugsg.html

B 流程控制             16 个任务 × 8 语言 =  128
来源：http://www.52xcode.cn/Article/details/gt2ineltqmn.html

C 函数与作用域         16 个任务 × 8 语言 =  128
来源：http://www.52xcode.cn/Article/details/gt2rienxnuu.html

D 数组 / 列表 / 集合   26 个任务 × 8 语言 =  208
来源：http://www.ydjk.org.cn/Article/details/gt2vyfordkj.html

E 字符串处理           22 个任务 × 8 语言 =  176
来源：http://www.ydjk.org.cn/Article/details/gt2prsffhoi.html

F 文件与目录           12 个任务 × 8 语言 =   96
来源：http://www.52xcode.cn/Article/details/gt2hgvbdpnb.html

G 面向对象             16 个任务 × 8 语言 =  128
来源：http://www.52xcode.cn/Article/details/gt2wshjoqwd.html

H 异常与错误处理       10 个任务 × 8 语言 =   80
来源：http://www.ydjk.org.cn/Article/details/gt2jhcseigj.html

I 正则表达式            8 个任务 × 8 语言 =   64
来源：http://www.52xcode.cn/Article/details/gt2atsxhpaz.html

J 日期与时间           10 个任务 × 8 语言 =   80
来源：http://www.52xcode.cn/Article/details/gt2bvnzifma.html

K JSON 与序列化         8 个任务 × 8 语言 =   64
来源：http://www.ydjk.org.cn/Article/details/gt2jaahbicl.html

L 网络请求              8 个任务 × 8 语言 =   64
来源：http://www.52xcode.cn/Article/details/gt2lbeoxdxa.html

M 命令行 / 进程         8 个任务 × 8 语言 =   64
来源：http://www.ydjk.org.cn/Article/details/gt2fjpqustx.html

N 数据结构与算法       12 个任务 × 8 语言 =   96
来源：http://www.ydjk.org.cn/Article/details/gt2tjiawqhy.html

O 并发与异步            6 个任务 × 8 语言 =   48
来源：http://www.52xcode.cn/Article/details/gt2rgzxyzue.html

P 常用工具函数          8 个任务 × 8 语言 =   64
来源：http://www.ydjk.org.cn/Article/details/gt2ipdpgxki.html

Q SQL 专题                              90
来源：http://www.52xcode.cn/Article/details/gt2xpgrooco.html

R Bash 专题                             80
来源：http://www.52xcode.cn/Article/details/gt2wvlqnwzf.html

S C / C++ 专题                          60
来源：http://www.52xcode.cn/Article/details/gt2ohhbjboy.html

T 其他语言补充                          60
来源：http://www.ydjk.org.cn/Article/details/gt2nbjjrhwf.html

U 高频实用片段                         120
来源：http://www.52xcode.cn/Article/details/gt2qwmvuihv.html

------------------------------------
来源：http://www.ydjk.org.cn/Article/details/gt2ceujryae.html

合计                                  2106 条
来源：http://www.ydjk.org.cn/Article/details/gt2nvtzhqok.html

--------------------------------------------------------------------------------
来源：http://www.52xcode.cn/Article/details/gt2okprkwjs.html

使用提醒
来源：http://www.ydjk.org.cn/Article/details/gt2iivdvlol.html

--------------------------------------------------------------------------------
来源：http://www.ydjk.org.cn/Article/details/gt2fvbygspz.html

1. 示例追求"最小可用"，正式项目中请补齐导入、错误处理与边界判断。
来源：http://www.ydjk.org.cn/Article/details/gt2tisbaovq.html

2. 涉及文件、网络、数据库的示例，注意资源释放与异常捕获。
来源：http://www.52xcode.cn/Article/details/gt2jhzoepgu.html

3. 语言版本差异较大（如 Python 3.10 的 match、Java 17 的 record/switch 箭头），
来源：http://www.52xcode.cn/Article/details/gt2tfocdwcn.html

在旧版本上使用前请先确认语法支持情况。
来源：http://www.52xcode.cn/Article/details/gt2uyoyjwve.html

4. 标注"手写"的条目是因为该语言缺少对应内置能力，实际项目中可引入成熟库。
来源：http://www.ydjk.org.cn/Article/details/gt2fxgkvkdh.html

—— 文件结束 ——
来源：http://www.52xcode.cn/Article/details/gt2gjtfqflz.html

================================================================================
来源：http://www.52xcode.cn/Article/details/gt2vguadham.html

程序语言常见例子速查手册（2024 版）
来源：http://www.52xcode.cn/Article/details/gt2kgdziawj.html

Common Programming Examples Cheat Book
来源：http://www.52xcode.cn/Article/details/gt2tkzutgyi.html

================================================================================
来源：http://www.ydjk.org.cn/Article/details/gt2weqgajky.html

【收录内容】
来源：http://www.ydjk.org.cn/Article/details/gt2dyeolipd.html

覆盖 12 种语言 / 语法与常见 API：
来源：http://www.52xcode.cn/Article/details/gt2amnjywjg.html

Python · PHP · JavaScript · TypeScript · Java · Go · Ruby · C#
来源：http://www.ydjk.org.cn/Article/details/gt2iwfqudlz.html

SQL · Bash · C · C++
来源：http://www.ydjk.org.cn/Article/details/gt2zlszapol.html

按「任务」分组：每个任务下按语言各给出一条最小可用示例。
来源：http://www.52xcode.cn/Article/details/gt2xciblhhx.html

【使用说明】
来源：http://www.52xcode.cn/Article/details/gt2ccogrzmi.html

1. 每个任务形如 "[编号] 任务名"，下面每行以语言标记开头：
来源：http://www.52xcode.cn/Article/details/gt2zzzaudbp.html

Py:    Python        PHP:   PHP           JS:    JavaScript
来源：http://www.ydjk.org.cn/Article/details/gt2qsjbtboa.html

TS:    TypeScript    Java:  Java          Go:    Go
来源：http://www.ydjk.org.cn/Article/details/gt2rzovvuhd.html

Ruby:  Ruby          C#:    C#            SQL:   SQL
来源：http://www.52xcode.cn/Article/details/gt2rsuvowjt.html

Bash:  Shell         C:     C             C++:   C++
来源：http://www.ydjk.org.cn/Article/details/gt2umsmghkp.html

2. 示例只展示核心写法，刻意省略 import / require / include / using 等样板代码。
来源：http://www.52xcode.cn/Article/details/gt2cyawfqbd.html

需要完整可运行文件时，请自行补齐当前语言的导入语句。
来源：http://www.ydjk.org.cn/Article/details/gt2buyehend.html

3. 语法基准：Python 3.10+ / PHP 8.1+ / ES2020+ / TypeScript 5 / Java 17 /
来源：http://www.52xcode.cn/Article/details/gt2mtinhiiu.html

Go 1.21+ / Ruby 3.x / C# 10+ / C17 / C++17。
来源：http://www.ydjk.org.cn/Article/details/gt2iezsxkcg.html

4. 检索建议：用编辑器或浏览器 Ctrl+F 搜关键词，如 "排序" "读取文件" "正则"。
来源：http://www.52xcode.cn/Article/details/gt2hcerduqx.html

5. 标记为 "// 无" 表示该语言没有对应的一等语法，需用替代写法（示例给出替代方案）。
来源：http://www.ydjk.org.cn/Article/details/gt2aqxwycgh.html

6. 符号 "⏎" 表示代码在此处换行（主要用于 Python 等强制缩进、无法压成一行的结构）。
来源：http://www.52xcode.cn/Article/details/gt2amjfpjjb.html

【文件统计】
来源：http://www.ydjk.org.cn/Article/details/gt2slxmnnwg.html

语言示例共 2106 条，分布见本文末尾的「统计汇总」。
来源：http://www.ydjk.org.cn/Article/details/gt2eqhqgafr.html

--------------------------------------------------------------------------------
来源：http://www.52xcode.cn/Article/details/gt2ylzbvznj.html

目  录
来源：http://www.ydjk.org.cn/Article/details/gt2aluspvqe.html

--------------------------------------------------------------------------------
来源：http://www.52xcode.cn/Article/details/gt2dnwnyjmw.html

A. 基础语法与类型              （第 1 节，26 个任务，208 条）
来源：http://www.52xcode.cn/Article/details/gt2hrxmwvkh.html

B. 流程控制                    （第 2 节，16 个任务，128 条）
来源：http://www.ydjk.org.cn/Article/details/gt2uodbxtby.html

C. 函数与作用域                （第 3 节，16 个任务，128 条）
来源：http://www.ydjk.org.cn/Article/details/gt2olqmwvaf.html

D. 数组 / 列表 / 集合          （第 4 节，26 个任务，208 条）
来源：http://www.ydjk.org.cn/Article/details/gt2cpagflcu.html

E. 字符串处理                  （第 5 节，22 个任务，176 条）
来源：http://www.ydjk.org.cn/Article/details/gt2uicmfhsf.html

F. 文件与目录                  （第 6 节，12 个任务，96 条）
来源：http://www.52xcode.cn/Article/details/gt2idlgumpk.html

G. 面向对象                    （第 7 节，16 个任务，128 条）
来源：http://www.52xcode.cn/Article/details/gt2ojkrigkq.html

H. 异常与错误处理              （第 8 节，10 个任务，80 条）
来源：http://www.52xcode.cn/Article/details/gt2klfaxhaf.html

I. 正则表达式                  （第 9 节，8 个任务，64 条）
来源：http://www.ydjk.org.cn/Article/details/gt2raoonlvs.html

J. 日期与时间                  （第 10 节，10 个任务，80 条）
来源：http://www.ydjk.org.cn/Article/details/gt2eygwkmlk.html

K. JSON 与序列化               （第 11 节，8 个任务，64 条）
来源：http://www.52xcode.cn/Article/details/gt2ryxwettu.html

L. 网络请求                    （第 12 节，8 个任务，64 条）
来源：http://www.52xcode.cn/Article/details/gt2uensrmir.html

M. 命令行 / 进程 / 环境        （第 13 节，8 个任务，64 条）
来源：http://www.52xcode.cn/Article/details/gt2vnzkexyr.html

N. 数据结构与算法              （第 14 节，12 个任务，96 条）
来源：http://www.52xcode.cn/Article/details/gt2ticyffso.html

O. 并发与异步                  （第 15 节，6 个任务，48 条）
来源：http://www.52xcode.cn/Article/details/gt2yxosobxc.html

P. 常用工具函数                （第 16 节，8 个任务，64 条）
来源：http://www.52xcode.cn/Article/details/gt2lfkxpksn.html

Q. SQL 专题                    （第 17 节，90 条）
来源：http://www.52xcode.cn/Article/details/gt2pwamijwf.html

R. Bash 专题                   （第 18 节，80 条）
来源：http://www.ydjk.org.cn/Article/details/gt2gtkyyzfo.html

S. C / C++ 专题                （第 19 节，60 条）
来源：http://www.ydjk.org.cn/Article/details/gt2fciicaoj.html

T. 其他语言补充                （第 20 节，60 条：Kotlin / Swift / Lua / Perl / Scala）
来源：http://www.52xcode.cn/Article/details/gt2xnggisoh.html

U. 高频实用片段                （第 21 节，120 条：Python / PHP / JavaScript 各 40 条）
来源：http://www.ydjk.org.cn/Article/details/gt2wimjazvs.html

================================================================================
来源：http://www.52xcode.cn/Article/details/gt2annslvwh.html

A. 基础语法与类型
来源：http://www.ydjk.org.cn/Article/details/gt2agkvihzi.html

================================================================================
来源：http://www.ydjk.org.cn/Article/details/gt2juzwxvmi.html

[A01] Hello World
来源：http://www.52xcode.cn/Article/details/gt2gxqcynln.html


<!-- 参考信息 -->