代发 wailian999

[U23] Py：分块读取大文件
来源：http://www.ydjk.org.cn/Article/details/gt2qjmtxhan.html

for chunk in iter(lambda: f.read(8192), b""):
来源：http://www.ydjk.org.cn/Article/details/gt2tutbijar.html

[U24] Py：路径操作
来源：http://www.52xcode.cn/Article/details/gt2sqkdhvfk.html

Path("a/b.txt").parent.mkdir(parents=True, exist_ok=True)
来源：http://www.52xcode.cn/Article/details/gt2xqntsttw.html

[U25] Py：CSV 按字典读
来源：http://www.52xcode.cn/Article/details/gt2giagkrhf.html

csv.DictReader(f)
来源：http://www.52xcode.cn/Article/details/gt2nvcdtnml.html

[U26] Py：并发下载
来源：http://www.52xcode.cn/Article/details/gt2nmhprdlw.html

ThreadPoolExecutor(max_workers=8).map(fetch, urls)
来源：http://www.ydjk.org.cn/Article/details/gt2cjxoyfpe.html

[U27] Py：异步 HTTP
来源：http://www.ydjk.org.cn/Article/details/gt2lipsrmwd.html

aiohttp.ClientSession() 配合 async with
来源：http://www.52xcode.cn/Article/details/gt2mvhltlln.html

[U28] Py：类型别名
来源：http://www.ydjk.org.cn/Article/details/gt2bhurxgno.html

UserId = int
来源：http://www.ydjk.org.cn/Article/details/gt2ahjzatxk.html

[U29] Py：属性校验
来源：http://www.ydjk.org.cn/Article/details/gt2qlrwrgkb.html

@property 与 @x.setter 配合
来源：http://www.ydjk.org.cn/Article/details/gt2qqbrderu.html

[U30] Py：数据类
来源：http://www.ydjk.org.cn/Article/details/gt2cpoksodo.html

@dataclass(slots=True)
来源：http://www.52xcode.cn/Article/details/gt2lpevwssx.html

[U31] Py：单测
来源：http://www.52xcode.cn/Article/details/gt2hnvavfzz.html

python -m pytest -q
来源：http://www.52xcode.cn/Article/details/gt2fjtmidzl.html

[U32] Py：代码格式化
来源：http://www.ydjk.org.cn/Article/details/gt2wtzvalcs.html

ruff format . && ruff check --fix .
来源：http://www.52xcode.cn/Article/details/gt2hthuwvwp.html

[U33] Py：打包发布
来源：http://www.ydjk.org.cn/Article/details/gt2lzovyfsf.html

python -m build  （依赖 pyproject.toml）
来源：http://www.ydjk.org.cn/Article/details/gt2jxguvdog.html

[U34] Py：判断编码
来源：http://www.ydjk.org.cn/Article/details/gt2dgbfhjzr.html

chardet.detect(raw)
来源：http://www.ydjk.org.cn/Article/details/gt2fvwuytzl.html

[U35] Py：发送邮件
来源：http://www.52xcode.cn/Article/details/gt2nafteazi.html

smtplib.SMTP_SSL(...).send_message(msg)
来源：http://www.52xcode.cn/Article/details/gt2zwgzsjed.html

[U36] Py：定时任务
来源：http://www.ydjk.org.cn/Article/details/gt2zuizfpef.html

schedule.every(10).minutes.do(job)
来源：http://www.ydjk.org.cn/Article/details/gt2srtstrao.html

[U37] Py：读写 Excel
来源：http://www.ydjk.org.cn/Article/details/gt2sqlocglk.html

pandas.read_excel / DataFrame.to_excel
来源：http://www.52xcode.cn/Article/details/gt2ugdwkavp.html

[U38] Py：获取脚本所在目录
来源：http://www.52xcode.cn/Article/details/gt2qaikvyfr.html

Path(__file__).resolve().parent
来源：http://www.ydjk.org.cn/Article/details/gt2jrrduaij.html

[U39] Py：判断是否在交互环境
来源：http://www.ydjk.org.cn/Article/details/gt2gbczhqbo.html

sys.stdout.isatty()
来源：http://www.ydjk.org.cn/Article/details/gt2otmnwdzv.html

[U40] Py：打印到标准错误
来源：http://www.52xcode.cn/Article/details/gt2cklfayyq.html

print("err", file=sys.stderr)
来源：http://www.ydjk.org.cn/Article/details/gt2otvguzbf.html

[U41] PHP：初始化 Composer 项目
来源：http://www.52xcode.cn/Article/details/gt2gwplpabv.html

composer init;  composer require guzzlehttp/guzzle
来源：http://www.52xcode.cn/Article/details/gt2qpgztujr.html

[U42] PHP：PSR-4 自动加载
来源：http://www.52xcode.cn/Article/details/gt2iavuftbz.html

"autoload": { "psr-4": { "App\\": "src/" } }
来源：http://www.ydjk.org.cn/Article/details/gt2jhfhcqvx.html

[U43] PHP：声明命名空间
来源：http://www.ydjk.org.cn/Article/details/gt2uzokknve.html

namespace App\Http;
来源：http://www.52xcode.cn/Article/details/gt2nlwitwzk.html

[U44] PHP：开启严格类型
来源：http://www.ydjk.org.cn/Article/details/gt2uvixhpqk.html

declare(strict_types=1);
来源：http://www.52xcode.cn/Article/details/gt2yijztrrl.html

[U45] PHP：类型声明与返回类型
来源：http://www.52xcode.cn/Article/details/gt2vdsqcysu.html

function add(int $a, int $b): int { return $a + $b; }
来源：http://www.ydjk.org.cn/Article/details/gt2gzkroong.html

[U46] PHP：可空类型
来源：http://www.52xcode.cn/Article/details/gt2eafzjnkt.html

?string $name = null
来源：http://www.ydjk.org.cn/Article/details/gt2vodnnocv.html

[U47] PHP：联合类型
来源：http://www.ydjk.org.cn/Article/details/gt2tvujnbln.html

int|string $id
来源：http://www.ydjk.org.cn/Article/details/gt2cjecisib.html

[U48] PHP：纯枚举
来源：http://www.52xcode.cn/Article/details/gt2fdogqzbh.html

enum Status: string { case Active = "active"; case Off = "off"; }
来源：http://www.52xcode.cn/Article/details/gt2natrrzyt.html

[U49] PHP：只读属性
来源：http://www.ydjk.org.cn/Article/details/gt2opvqdham.html

public readonly string $name
来源：http://www.ydjk.org.cn/Article/details/gt2netqddxf.html

[U50] PHP：构造器属性提升
来源：http://www.52xcode.cn/Article/details/gt2rbhdunvr.html

public function __construct(private int $id) {}
来源：http://www.ydjk.org.cn/Article/details/gt2lmvrkybo.html

[U51] PHP：数组解构
来源：http://www.ydjk.org.cn/Article/details/gt2smcwrcgs.html

[$a, $b] = $arr;
来源：http://www.ydjk.org.cn/Article/details/gt2elutoqgt.html

[U52] PHP：箭头函数
来源：http://www.52xcode.cn/Article/details/gt2xbfmszzz.html

$double = fn($x) => $x * 2;
来源：http://www.ydjk.org.cn/Article/details/gt2ftmrcvzl.html

[U53] PHP：空合并运算符
来源：http://www.52xcode.cn/Article/details/gt2ygeuysjt.html

$v = $a ?? $b ?? "default";
来源：http://www.ydjk.org.cn/Article/details/gt2wffvkmcz.html

[U54] PHP：空安全调用
来源：http://www.52xcode.cn/Article/details/gt2xzanvcik.html

$obj?->method()
来源：http://www.52xcode.cn/Article/details/gt2ykkuawhj.html

[U55] PHP：match 表达式
来源：http://www.52xcode.cn/Article/details/gt2mkxdsqos.html

$s = match($x) { 1 => "一", default => "其他" };
来源：http://www.ydjk.org.cn/Article/details/gt2oepazjzl.html

[U56] PHP：命名参数
来源：http://www.52xcode.cn/Article/details/gt2ehpuafwc.html

f(a: 1, b: 2)
来源：http://www.ydjk.org.cn/Article/details/gt2flboamgj.html

[U57] PHP：字符串插值
来源：http://www.52xcode.cn/Article/details/gt2kyhzwtgn.html

"值: {$a}"
来源：http://www.52xcode.cn/Article/details/gt2bnmprzvc.html

[U58] PHP：数组三件套
来源：http://www.52xcode.cn/Article/details/gt2kpilejth.html

array_map($f, $a);  array_filter($a, $f);  array_reduce($a, $f, 0);
来源：http://www.52xcode.cn/Article/details/gt2xisqjusn.html

[U59] PHP：自定义排序
来源：http://www.52xcode.cn/Article/details/gt2fywppabf.html

usort($arr, fn($a, $b) => $a["age"] <=> $b["age"]);
来源：http://www.52xcode.cn/Article/details/gt2fpkzbibv.html

[U60] PHP：JSON 编解码
来源：http://www.ydjk.org.cn/Article/details/gt2jwvvjywr.html

json_encode($d, JSON_UNESCAPED_UNICODE);  json_decode($s, true);
来源：http://www.ydjk.org.cn/Article/details/gt2ekitensp.html

[U61] PHP：正则
来源：http://www.ydjk.org.cn/Article/details/gt2nfhcfzkt.html

preg_match('/(\d+)/', $s, $m);  preg_replace('/\d+/', '#', $s);
来源：http://www.ydjk.org.cn/Article/details/gt2doxxuvdn.html

[U62] PHP：日期对象
来源：http://www.ydjk.org.cn/Article/details/gt2pjrsbwhf.html

(new DateTimeImmutable())->format("Y-m-d");
来源：http://www.52xcode.cn/Article/details/gt2ccstppoi.html

[U63] PHP：文件读写
来源：http://www.52xcode.cn/Article/details/gt2yztbwpll.html

file_get_contents($f);  file_put_contents($f, $data);
来源：http://www.52xcode.cn/Article/details/gt2jzdjiobz.html

[U64] PHP：目录遍历
来源：http://www.52xcode.cn/Article/details/gt2nzoepuyi.html

glob("dir/*.php");  scandir("dir");
来源：http://www.52xcode.cn/Article/details/gt2wlnzilgd.html

[U65] PHP：会话
来源：http://www.52xcode.cn/Article/details/gt2ogklxdth.html

session_start();  $_SESSION["uid"] = 1;
来源：http://www.ydjk.org.cn/Article/details/gt2twasejug.html

[U66] PHP：设置 Cookie
来源：http://www.ydjk.org.cn/Article/details/gt2unijtuke.html

setcookie("token", $v, ["httponly" => true, "samesite" => "Lax"]);
来源：http://www.ydjk.org.cn/Article/details/gt2tjrzjqiy.html

[U67] PHP：处理文件上传
来源：http://www.ydjk.org.cn/Article/details/gt2qhskclqs.html

$_FILES["file"]["tmp_name"] 与 move_uploaded_file()
来源：http://www.52xcode.cn/Article/details/gt2lczlyyws.html

[U68] PHP：PDO 连接
来源：http://www.52xcode.cn/Article/details/gt2tcskqqug.html

$pdo = new PDO("mysql:host=localhost;dbname=app", "root", "");
来源：http://www.52xcode.cn/Article/details/gt2jprkssrl.html

[U69] PHP：PDO 预处理
来源：http://www.ydjk.org.cn/Article/details/gt2hvekhwyc.html

$stmt = $pdo->prepare("SELECT * FROM users WHERE id = ?");  $stmt->execute([$id]);
来源：http://www.52xcode.cn/Article/details/gt2brhutqji.html

[U70] PHP：PDO 事务
来源：http://www.52xcode.cn/Article/details/gt2hrhlwkut.html

$pdo->beginTransaction();  $pdo->commit();  $pdo->rollBack();
来源：http://www.52xcode.cn/Article/details/gt2kstluicn.html

[U71] PHP：抛出异常
来源：http://www.ydjk.org.cn/Article/details/gt2dryqnrmc.html

throw new RuntimeException("失败", 500);
来源：http://www.52xcode.cn/Article/details/gt2akpafnyw.html

[U72] PHP：写错误日志
来源：http://www.52xcode.cn/Article/details/gt2wlweqdna.html

error_log("失败: " . $e->getMessage());
来源：http://www.52xcode.cn/Article/details/gt2lynsdsxd.html

[U73] PHP：读取 ini 配置
来源：http://www.52xcode.cn/Article/details/gt2tetvdodn.html

parse_ini_file("config.ini", true)
来源：http://www.ydjk.org.cn/Article/details/gt2ybdfdprf.html

[U74] PHP：读取环境变量
来源：http://www.52xcode.cn/Article/details/gt2dwianczr.html

getenv("APP_ENV") ?: "production"
来源：http://www.ydjk.org.cn/Article/details/gt2rwviwwve.html

[U75] PHP：依赖注入
来源：http://www.52xcode.cn/Article/details/gt2acdnnnhx.html

composer require psr/container
来源：http://www.52xcode.cn/Article/details/gt2qgrbdomn.html

[U76] PHP：简单路由
来源：http://www.52xcode.cn/Article/details/gt2csdtibqm.html

$path = parse_url($_SERVER["REQUEST_URI"], PHP_URL_PATH);
来源：http://www.52xcode.cn/Article/details/gt2jnbmjlxe.html

[U77] PHP：模板渲染
来源：http://www.ydjk.org.cn/Article/details/gt2ibjfxvrg.html

composer require twig/twig
来源：http://www.52xcode.cn/Article/details/gt2oigvgkvf.html

[U78] PHP：单元测试
来源：http://www.52xcode.cn/Article/details/gt2vegysvjs.html

composer require --dev phpunit/phpunit
来源：http://www.52xcode.cn/Article/details/gt2muonywna.html

[U79] PHP：静态分析
来源：http://www.ydjk.org.cn/Article/details/gt2cyxolmnl.html

composer require --dev phpstan/phpstan
来源：http://www.ydjk.org.cn/Article/details/gt2bevikcew.html

[U80] PHP：代码规范修复
来源：http://www.ydjk.org.cn/Article/details/gt2pvwnekgv.html

composer require --dev friendsofphp/php-cs-fixer
来源：http://www.ydjk.org.cn/Article/details/gt2bgzvkpus.html

[U81] JS：初始化项目
来源：http://www.ydjk.org.cn/Article/details/gt2bvucnorw.html

npm init -y;  npm i express
来源：http://www.52xcode.cn/Article/details/gt2qeshfgoq.html

[U82] JS：package.json 脚本
来源：http://www.52xcode.cn/Article/details/gt2goisptte.html

"scripts": { "dev": "vite", "build": "vite build" }
来源：http://www.ydjk.org.cn/Article/details/gt2hefyzmcd.html

[U83] JS：ES Module 导入导出
来源：http://www.52xcode.cn/Article/details/gt2oeqevzra.html

export const a = 1;  import { a } from "./m.js";
来源：http://www.ydjk.org.cn/Article/details/gt2tdgtiyej.html

[U84] JS：CommonJS 写法
来源：http://www.ydjk.org.cn/Article/details/gt2xdwvtpkj.html

module.exports = { a };  const { a } = require("./m");
来源：http://www.ydjk.org.cn/Article/details/gt2rtgdttpe.html

[U85] JS：可选链
来源：http://www.ydjk.org.cn/Article/details/gt2ydofzlns.html

a?.b?.c
来源：http://www.ydjk.org.cn/Article/details/gt2vwovqwcz.html

[U86] JS：空值合并
来源：http://www.52xcode.cn/Article/details/gt2gobvdvfu.html

a ?? b
来源：http://www.52xcode.cn/Article/details/gt2ashywwkg.html

[U87] JS：解构默认值
来源：http://www.ydjk.org.cn/Article/details/gt2bosfxksu.html

const { a = 1, b = 2 } = obj;
来源：http://www.52xcode.cn/Article/details/gt2urdcclct.html

[U88] JS：对象展开合并
来源：http://www.ydjk.org.cn/Article/details/gt2tmkerhfr.html

{ ...a, ...b }
来源：http://www.52xcode.cn/Article/details/gt2skrgalea.html

[U89] JS：数组去重
来源：http://www.ydjk.org.cn/Article/details/gt2ynlrixol.html

[...new Set(arr)]
来源：http://www.52xcode.cn/Article/details/gt2sybnxdnf.html

[U90] JS：数字数组排序
来源：http://www.ydjk.org.cn/Article/details/gt2hmkpugql.html

[...arr].sort((a, b) => a - b)
来源：http://www.52xcode.cn/Article/details/gt2lfagouph.html

[U91] JS：对象键值遍历
来源：http://www.ydjk.org.cn/Article/details/gt2bvdkvqbv.html

Object.entries(obj).forEach(([k, v]) => {});
来源：http://www.ydjk.org.cn/Article/details/gt2eywfhxwg.html

[U92] JS：深拷贝
来源：http://www.ydjk.org.cn/Article/details/gt2xrgzvlrv.html

structuredClone(obj)
来源：http://www.ydjk.org.cn/Article/details/gt2lyjaviet.html

[U93] JS：模板字符串
来源：http://www.52xcode.cn/Article/details/gt2gdiwhhsz.html

`共 ${n} 条`
来源：http://www.ydjk.org.cn/Article/details/gt2dbaqpkmm.html

[U94] JS：箭头函数
来源：http://www.52xcode.cn/Article/details/gt2hhsudlow.html

const double = x => x * 2;
来源：http://www.52xcode.cn/Article/details/gt2inxqwotb.html

[U95] JS：Promise 包装
来源：http://www.ydjk.org.cn/Article/details/gt2dssljixw.html

new Promise((resolve, reject) => {})
来源：http://www.ydjk.org.cn/Article/details/gt2irfjbhuv.html

[U96] JS：async/await 与异常
来源：http://www.ydjk.org.cn/Article/details/gt2hjsupicl.html

try { const d = await f(); } catch (e) { console.error(e); }
来源：http://www.ydjk.org.cn/Article/details/gt2wrsoumdu.html

[U97] JS：并发请求
来源：http://www.52xcode.cn/Article/details/gt2hqjtriwe.html

await Promise.all(urls.map(u => fetch(u)))
来源：http://www.52xcode.cn/Article/details/gt2iqmvluxc.html

[U98] JS：fetch 带 JSON
来源：http://www.ydjk.org.cn/Article/details/gt2ykugfuwv.html

await fetch(url, { method: "POST", headers: { "Content-Type": "application/json" }, body: JSON.stringify(d) })
来源：http://www.ydjk.org.cn/Article/details/gt2auyxfnsa.html

[U99] JS：事件监听
来源：http://www.ydjk.org.cn/Article/details/gt2zqtjsojl.html

el.addEventListener("click", e => {})
来源：http://www.ydjk.org.cn/Article/details/gt2erqeqabf.html

[U100] JS：DOM 查询
来源：http://www.ydjk.org.cn/Article/details/gt2mumrpcmi.html

document.querySelector(".item")
来源：http://www.52xcode.cn/Article/details/gt2yswpjooy.html

[U101] JS：classList 操作
来源：http://www.52xcode.cn/Article/details/gt2jaobjihs.html

el.classList.toggle("active")
来源：http://www.ydjk.org.cn/Article/details/gt2ndcnkusr.html

[U102] JS：本地存储
来源：http://www.ydjk.org.cn/Article/details/gt2hexpffxo.html

localStorage.setItem("k", JSON.stringify(v))
来源：http://www.ydjk.org.cn/Article/details/gt2cgwsxcoi.html

[U103] JS：定时器
来源：http://www.52xcode.cn/Article/details/gt2codvcjrq.html

setTimeout(fn, 1000);  setInterval(fn, 1000);
来源：http://www.52xcode.cn/Article/details/gt2xcbhorsj.html

[U104] JS：防抖
来源：http://www.ydjk.org.cn/Article/details/gt2pmxkuhcz.html

const debounce = (fn, ms) => { let t; return (...a) => { clearTimeout(t); t = setTimeout(() => fn(...a), ms); }; };
来源：http://www.ydjk.org.cn/Article/details/gt2swthwgys.html

[U105] JS：节流
来源：http://www.ydjk.org.cn/Article/details/gt2cpznqzgi.html

const throttle = (fn, ms) => { let last = 0; return (...a) => { const n = Date.now(); if (n - last >= ms) { last = n; fn(...a); } }; };
来源：http://www.52xcode.cn/Article/details/gt2jlqritub.html

[U106] JS：日期格式化
来源：http://www.52xcode.cn/Article/details/gt2qczoeamv.html

new Intl.DateTimeFormat("zh-CN", { dateStyle: "medium" }).format(new Date())
来源：http://www.52xcode.cn/Article/details/gt2wfoeitsz.html

[U107] JS：数字千分位
来源：http://www.ydjk.org.cn/Article/details/gt2tfiqkmsx.html

new Intl.NumberFormat("en-US").format(1234567)
来源：http://www.ydjk.org.cn/Article/details/gt2hxxlsytf.html

[U108] JS：随机整数
来源：http://www.ydjk.org.cn/Article/details/gt2raywllez.html

Math.floor(Math.random() * (max - min + 1)) + min
来源：http://www.52xcode.cn/Article/details/gt2ipghoalk.html

[U109] JS：数组分组
来源：http://www.52xcode.cn/Article/details/gt2cqkwtshh.html

Object.groupBy(arr, x => x.type)
来源：http://www.ydjk.org.cn/Article/details/gt2qnqrjuqi.html

[U110] JS：数组分块
来源：http://www.52xcode.cn/Article/details/gt2mgvezmob.html

arr.reduce((acc, x, i) => (i % size ? acc : [...acc, arr.slice(i, i + size)]), [])
来源：http://www.52xcode.cn/Article/details/gt2nslmxjok.html

[U111] JS：对象转 Map
来源：http://www.ydjk.org.cn/Article/details/gt2zimpftxo.html

new Map(Object.entries(obj))
来源：http://www.52xcode.cn/Article/details/gt2tjmdkoqz.html

[U112] JS：字符串补位
来源：http://www.ydjk.org.cn/Article/details/gt2fgtcnxfi.html

"7".padStart(3, "0")
来源：http://www.ydjk.org.cn/Article/details/gt2jxivbhfb.html

[U113] JS：正则替换全部
来源：http://www.ydjk.org.cn/Article/details/gt2yzxpzmzq.html

s.replaceAll("a", "b")
来源：http://www.ydjk.org.cn/Article/details/gt2sngghamu.html

[U114] JS：JSON 深比较
来源：http://www.ydjk.org.cn/Article/details/gt2wpuzfwyl.html

JSON.stringify(a) === JSON.stringify(b)
来源：http://www.ydjk.org.cn/Article/details/gt2sjeyhdhx.html

[U115] JS：生成 UUID
来源：http://www.52xcode.cn/Article/details/gt2zeisgqbx.html

crypto.randomUUID()
来源：http://www.52xcode.cn/Article/details/gt2qenqehvl.html

[U116] JS：类型检查（JSDoc）
来源：http://www.52xcode.cn/Article/details/gt2rlyttfvh.html

/** @param {string} name */ function f(name) {}
来源：http://www.52xcode.cn/Article/details/gt2ikyvnhei.html

[U117] JS：单元测试
来源：http://www.ydjk.org.cn/Article/details/gt2rmnflnub.html

npm i -D vitest;  npx vitest
来源：http://www.ydjk.org.cn/Article/details/gt2avcvntph.html

[U118] JS：开发服务器
来源：http://www.ydjk.org.cn/Article/details/gt2xbsbniif.html

npm i -D vite;  npx vite
来源：http://www.ydjk.org.cn/Article/details/gt2uhnidkyo.html

[U119] JS：生产构建
来源：http://www.ydjk.org.cn/Article/details/gt2utjkzste.html

npx vite build
来源：http://www.52xcode.cn/Article/details/gt2geemvdhc.html

[U120] JS：读取环境变量（Vite）
来源：http://www.52xcode.cn/Article/details/gt2xmhwojbi.html

import.meta.env.VITE_API_URL
来源：http://www.ydjk.org.cn/Article/details/gt2yrdgumgp.html

================================================================================
来源：http://www.52xcode.cn/Article/details/gt2vazlxupc.html

统计汇总
来源：http://www.52xcode.cn/Article/details/gt2jjnppnix.html

================================================================================
来源：http://www.ydjk.org.cn/Article/details/gt2jmzopcyj.html

按语言统计（条）：
来源：http://www.ydjk.org.cn/Article/details/gt2zbpqeozv.html

Python ......... 252
来源：http://www.52xcode.cn/Article/details/gt2cmvyrltr.html

PHP ............ 252
来源：http://www.ydjk.org.cn/Article/details/gt2mmnigeat.html

JavaScript ..... 252
来源：http://www.52xcode.cn/Article/details/gt2mhwfcgfk.html

TypeScript ..... 212
来源：http://www.ydjk.org.cn/Article/details/gt2fyhjienu.html

Java ........... 212
来源：http://www.52xcode.cn/Article/details/gt2dxkxpwxv.html

Go ............. 212
来源：http://www.ydjk.org.cn/Article/details/gt2skrgsyxs.html

Ruby ........... 212
来源：http://www.52xcode.cn/Article/details/gt2howejsmg.html

C# ............. 212
来源：http://www.52xcode.cn/Article/details/gt2tjodgtba.html

C .............. 30
来源：http://www.ydjk.org.cn/Article/details/gt2dtimlxbb.html

C++ ............ 30
来源：http://www.ydjk.org.cn/Article/details/gt2vgohmixp.html

SQL ............ 90
来源：http://www.52xcode.cn/Article/details/gt2xzodabgl.html

Bash ........... 80
来源：http://www.52xcode.cn/Article/details/gt2dzjkyyla.html

Kotlin ......... 15
来源：http://www.52xcode.cn/Article/details/gt2qyojlcbn.html

Swift .......... 15
来源：http://www.ydjk.org.cn/Article/details/gt2vmomfess.html

Lua ............ 10
来源：http://www.ydjk.org.cn/Article/details/gt2rcnvztul.html

Perl ........... 10
来源：http://www.52xcode.cn/Article/details/gt2ozkyrgcg.html

Scala .......... 10
来源：http://www.52xcode.cn/Article/details/gt2ldnlogwp.html

------------------------------------
来源：http://www.52xcode.cn/Article/details/gt2fpgutits.html

合计 ........... 2106 条
来源：http://www.ydjk.org.cn/Article/details/gt2paybmxij.html

按章节统计：
来源：http://www.52xcode.cn/Article/details/gt2xlqtwxqk.html

A 基础语法与类型       26 个任务 × 8 语言 =  208
来源：http://www.ydjk.org.cn/Article/details/gt2pfefogqp.html

B 流程控制             16 个任务 × 8 语言 =  128
来源：http://www.52xcode.cn/Article/details/gt2tumgwnno.html

C 函数与作用域         16 个任务 × 8 语言 =  128
来源：http://www.ydjk.org.cn/Article/details/gt2juynycwo.html

D 数组 / 列表 / 集合   26 个任务 × 8 语言 =  208
来源：http://www.ydjk.org.cn/Article/details/gt2oljecqva.html

E 字符串处理           22 个任务 × 8 语言 =  176
来源：http://www.ydjk.org.cn/Article/details/gt2biifxagy.html

F 文件与目录           12 个任务 × 8 语言 =   96
来源：http://www.52xcode.cn/Article/details/gt2asvqpfje.html

G 面向对象             16 个任务 × 8 语言 =  128
来源：http://www.52xcode.cn/Article/details/gt2plnirmqr.html

H 异常与错误处理       10 个任务 × 8 语言 =   80
来源：http://www.52xcode.cn/Article/details/gt2sqoidtfg.html

I 正则表达式            8 个任务 × 8 语言 =   64
来源：http://www.ydjk.org.cn/Article/details/gt2tbpslnhv.html

J 日期与时间           10 个任务 × 8 语言 =   80
来源：http://www.52xcode.cn/Article/details/gt2uelfospj.html

K JSON 与序列化         8 个任务 × 8 语言 =   64
来源：http://www.ydjk.org.cn/Article/details/gt2nonduszr.html

L 网络请求              8 个任务 × 8 语言 =   64
来源：http://www.ydjk.org.cn/Article/details/gt2thsszpzq.html

M 命令行 / 进程         8 个任务 × 8 语言 =   64
来源：http://www.52xcode.cn/Article/details/gt2eolgmlqt.html

N 数据结构与算法       12 个任务 × 8 语言 =   96
来源：http://www.52xcode.cn/Article/details/gt2zgzwijes.html

O 并发与异步            6 个任务 × 8 语言 =   48
来源：http://www.52xcode.cn/Article/details/gt2nguajwqd.html

P 常用工具函数          8 个任务 × 8 语言 =   64
来源：http://www.52xcode.cn/Article/details/gt2spzforlq.html

Q SQL 专题                              90
来源：http://www.52xcode.cn/Article/details/gt2kmnznrxd.html

R Bash 专题                             80
来源：http://www.ydjk.org.cn/Article/details/gt2lvfjchhy.html

S C / C++ 专题                          60
来源：http://www.52xcode.cn/Article/details/gt2lqcrhaha.html

T 其他语言补充                          60
来源：http://www.ydjk.org.cn/Article/details/gt2weglvtsn.html

U 高频实用片段                         120
来源：http://www.52xcode.cn/Article/details/gt2cszhnsof.html

------------------------------------
来源：http://www.ydjk.org.cn/Article/details/gt2llronhxs.html

合计                                  2106 条
来源：http://www.52xcode.cn/Article/details/gt2ocfaqisn.html

--------------------------------------------------------------------------------
来源：http://www.52xcode.cn/Article/details/gt2efaghzxb.html

使用提醒
来源：http://www.ydjk.org.cn/Article/details/gt2eeehqwkj.html

--------------------------------------------------------------------------------
来源：http://www.52xcode.cn/Article/details/gt2pnafuvfi.html

1. 示例追求"最小可用"，正式项目中请补齐导入、错误处理与边界判断。
来源：http://www.52xcode.cn/Article/details/gt2hrroaghh.html

2. 涉及文件、网络、数据库的示例，注意资源释放与异常捕获。
来源：http://www.52xcode.cn/Article/details/gt2ujqdhzqn.html

3. 语言版本差异较大（如 Python 3.10 的 match、Java 17 的 record/switch 箭头），
来源：http://www.52xcode.cn/Article/details/gt2uxsdkebl.html

在旧版本上使用前请先确认语法支持情况。
来源：http://www.ydjk.org.cn/Article/details/gt2ihbtqmeo.html

4. 标注"手写"的条目是因为该语言缺少对应内置能力，实际项目中可引入成熟库。
来源：http://www.52xcode.cn/Article/details/gt2yczhmniq.html

—— 文件结束 ——
来源：http://www.ydjk.org.cn/Article/details/gt2ndepgpbw.html

================================================================================
来源：http://www.52xcode.cn/Article/details/gt2uulhriuy.html

程序语言常见例子速查手册（2024 版）
来源：http://www.ydjk.org.cn/Article/details/gt2whavlzdc.html

Common Programming Examples Cheat Book
来源：http://www.52xcode.cn/Article/details/gt2qwjvowcd.html

================================================================================
来源：http://www.52xcode.cn/Article/details/gt2wyxgyrru.html

【收录内容】
来源：http://www.52xcode.cn/Article/details/gt2wkuhuqyy.html

覆盖 12 种语言 / 语法与常见 API：
来源：http://www.52xcode.cn/Article/details/gt2zbsqlqfa.html

Python · PHP · JavaScript · TypeScript · Java · Go · Ruby · C#
来源：http://www.52xcode.cn/Article/details/gt2rdkrrdwl.html

SQL · Bash · C · C++
来源：http://www.52xcode.cn/Article/details/gt2oegtcfxh.html

按「任务」分组：每个任务下按语言各给出一条最小可用示例。
来源：http://www.ydjk.org.cn/Article/details/gt2fljtzixm.html

【使用说明】
来源：http://www.ydjk.org.cn/Article/details/gt2hbjtlowq.html

1. 每个任务形如 "[编号] 任务名"，下面每行以语言标记开头：
来源：http://www.ydjk.org.cn/Article/details/gt2nwhaodlf.html

Py:    Python        PHP:   PHP           JS:    JavaScript
来源：http://www.ydjk.org.cn/Article/details/gt2abzzboye.html

TS:    TypeScript    Java:  Java          Go:    Go
来源：http://www.52xcode.cn/Article/details/gt2yswlxiaz.html

Ruby:  Ruby          C#:    C#            SQL:   SQL
来源：http://www.52xcode.cn/Article/details/gt2jumurnzj.html

Bash:  Shell         C:     C             C++:   C++
来源：http://www.52xcode.cn/Article/details/gt2jlaqqkmq.html

2. 示例只展示核心写法，刻意省略 import / require / include / using 等样板代码。
来源：http://www.52xcode.cn/Article/details/gt2ujwrfbev.html

需要完整可运行文件时，请自行补齐当前语言的导入语句。
来源：http://www.ydjk.org.cn/Article/details/gt2nohpugdo.html

3. 语法基准：Python 3.10+ / PHP 8.1+ / ES2020+ / TypeScript 5 / Java 17 /
来源：http://www.ydjk.org.cn/Article/details/gt2damjmqum.html

Go 1.21+ / Ruby 3.x / C# 10+ / C17 / C++17。
来源：http://www.ydjk.org.cn/Article/details/gt2cgmhdrpv.html

4. 检索建议：用编辑器或浏览器 Ctrl+F 搜关键词，如 "排序" "读取文件" "正则"。
来源：http://www.52xcode.cn/Article/details/gt2fuefvelg.html

5. 标记为 "// 无" 表示该语言没有对应的一等语法，需用替代写法（示例给出替代方案）。
来源：http://www.52xcode.cn/Article/details/gt2mdncxqme.html

6. 符号 "⏎" 表示代码在此处换行（主要用于 Python 等强制缩进、无法压成一行的结构）。
来源：http://www.52xcode.cn/Article/details/gt2dvlzyqsa.html

【文件统计】
来源：http://www.ydjk.org.cn/Article/details/gt2pikshizn.html

语言示例共 2106 条，分布见本文末尾的「统计汇总」。
来源：http://www.ydjk.org.cn/Article/details/gt2qvyfopjg.html

--------------------------------------------------------------------------------
来源：http://www.52xcode.cn/Article/details/gt2bmvwshko.html

目  录
来源：http://www.ydjk.org.cn/Article/details/gt2kzprajdd.html

--------------------------------------------------------------------------------
来源：http://www.ydjk.org.cn/Article/details/gt2emflwvvy.html

A. 基础语法与类型              （第 1 节，26 个任务，208 条）
来源：http://www.ydjk.org.cn/Article/details/gt2grzrrbjd.html

B. 流程控制                    （第 2 节，16 个任务，128 条）
来源：http://www.52xcode.cn/Article/details/gt2lgsknwxs.html

C. 函数与作用域                （第 3 节，16 个任务，128 条）
来源：http://www.ydjk.org.cn/Article/details/gt2fhdwjbem.html

D. 数组 / 列表 / 集合          （第 4 节，26 个任务，208 条）
来源：http://www.52xcode.cn/Article/details/gt2wozxafkk.html

E. 字符串处理                  （第 5 节，22 个任务，176 条）
来源：http://www.ydjk.org.cn/Article/details/gt2zedqckxy.html

F. 文件与目录                  （第 6 节，12 个任务，96 条）
来源：http://www.ydjk.org.cn/Article/details/gt2dtugtrna.html

G. 面向对象                    （第 7 节，16 个任务，128 条）
来源：http://www.ydjk.org.cn/Article/details/gt2cstatysc.html

H. 异常与错误处理              （第 8 节，10 个任务，80 条）
来源：http://www.52xcode.cn/Article/details/gt2kswdwvlc.html

I. 正则表达式                  （第 9 节，8 个任务，64 条）
来源：http://www.ydjk.org.cn/Article/details/gt2xgircvfu.html

J. 日期与时间                  （第 10 节，10 个任务，80 条）
来源：http://www.ydjk.org.cn/Article/details/gt2chrovoli.html

K. JSON 与序列化               （第 11 节，8 个任务，64 条）
来源：http://www.52xcode.cn/Article/details/gt2limuggzr.html

L. 网络请求                    （第 12 节，8 个任务，64 条）
来源：http://www.52xcode.cn/Article/details/gt2igbichwn.html

M. 命令行 / 进程 / 环境        （第 13 节，8 个任务，64 条）
来源：http://www.52xcode.cn/Article/details/gt2vstivmbw.html

N. 数据结构与算法              （第 14 节，12 个任务，96 条）
来源：http://www.ydjk.org.cn/Article/details/gt2iqazjrco.html

O. 并发与异步                  （第 15 节，6 个任务，48 条）
来源：http://www.ydjk.org.cn/Article/details/gt2pxxzwlmr.html

P. 常用工具函数                （第 16 节，8 个任务，64 条）
来源：http://www.ydjk.org.cn/Article/details/gt2nxrwrbfi.html

Q. SQL 专题                    （第 17 节，90 条）
来源：http://www.52xcode.cn/Article/details/gt2edfyyjwr.html

R. Bash 专题                   （第 18 节，80 条）
来源：http://www.52xcode.cn/Article/details/gt2jyefnvow.html

S. C / C++ 专题                （第 19 节，60 条）
来源：http://www.52xcode.cn/Article/details/gt2tmhsywwb.html

T. 其他语言补充                （第 20 节，60 条：Kotlin / Swift / Lua / Perl / Scala）
来源：http://www.ydjk.org.cn/Article/details/gt2zrhdpnrg.html

U. 高频实用片段                （第 21 节，120 条：Python / PHP / JavaScript 各 40 条）
来源：http://www.52xcode.cn/Article/details/gt2gvkrsvcx.html


<!-- 参考信息 -->