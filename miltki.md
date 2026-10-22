代发 wailian999

[U25] Py：CSV 按字典读
来源：http://www.52xcode.cn/Article/details/gt2vymykfgh.html

csv.DictReader(f)
来源：http://www.ydjk.org.cn/Article/details/gt2thzsfxew.html

[U26] Py：并发下载
来源：http://www.ydjk.org.cn/Article/details/gt2jwvwevfj.html

ThreadPoolExecutor(max_workers=8).map(fetch, urls)
来源：http://www.52xcode.cn/Article/details/gt2iyuwxhzv.html

[U27] Py：异步 HTTP
来源：http://www.52xcode.cn/Article/details/gt2xefozrwx.html

aiohttp.ClientSession() 配合 async with
来源：http://www.ydjk.org.cn/Article/details/gt2sosfwhjg.html

[U28] Py：类型别名
来源：http://www.52xcode.cn/Article/details/gt2evodmdmc.html

UserId = int
来源：http://www.ydjk.org.cn/Article/details/gt2pffrrqyv.html

[U29] Py：属性校验
来源：http://www.52xcode.cn/Article/details/gt2fawtbvpm.html

@property 与 @x.setter 配合
来源：http://www.ydjk.org.cn/Article/details/gt2bpxqlokc.html

[U30] Py：数据类
来源：http://www.52xcode.cn/Article/details/gt2fwogstom.html

@dataclass(slots=True)
来源：http://www.ydjk.org.cn/Article/details/gt2hupwfrrf.html

[U31] Py：单测
来源：http://www.52xcode.cn/Article/details/gt2ffbqlamz.html

python -m pytest -q
来源：http://www.ydjk.org.cn/Article/details/gt2oskdrscy.html

[U32] Py：代码格式化
来源：http://www.ydjk.org.cn/Article/details/gt2qleeqnpv.html

ruff format . && ruff check --fix .
来源：http://www.ydjk.org.cn/Article/details/gt2wolrnord.html

[U33] Py：打包发布
来源：http://www.ydjk.org.cn/Article/details/gt2iewrpdlb.html

python -m build  （依赖 pyproject.toml）
来源：http://www.ydjk.org.cn/Article/details/gt2zinsxrqb.html

[U34] Py：判断编码
来源：http://www.52xcode.cn/Article/details/gt2yglufjmr.html

chardet.detect(raw)
来源：http://www.ydjk.org.cn/Article/details/gt2murbczht.html

[U35] Py：发送邮件
来源：http://www.ydjk.org.cn/Article/details/gt2vkmoaytl.html

smtplib.SMTP_SSL(...).send_message(msg)
来源：http://www.ydjk.org.cn/Article/details/gt2wjdvfpqp.html

[U36] Py：定时任务
来源：http://www.ydjk.org.cn/Article/details/gt2qmqxqrzx.html

schedule.every(10).minutes.do(job)
来源：http://www.52xcode.cn/Article/details/gt2olygeneo.html

[U37] Py：读写 Excel
来源：http://www.52xcode.cn/Article/details/gt2ccgbmrgt.html

pandas.read_excel / DataFrame.to_excel
来源：http://www.52xcode.cn/Article/details/gt2nckhhrmk.html

[U38] Py：获取脚本所在目录
来源：http://www.ydjk.org.cn/Article/details/gt2smhhlfpz.html

Path(__file__).resolve().parent
来源：http://www.ydjk.org.cn/Article/details/gt2zwlsieof.html

[U39] Py：判断是否在交互环境
来源：http://www.52xcode.cn/Article/details/gt2wsridaxn.html

sys.stdout.isatty()
来源：http://www.52xcode.cn/Article/details/gt2hzejplhx.html

[U40] Py：打印到标准错误
来源：http://www.52xcode.cn/Article/details/gt2spkhwuub.html

print("err", file=sys.stderr)
来源：http://www.ydjk.org.cn/Article/details/gt2saggvdpx.html

[U41] PHP：初始化 Composer 项目
来源：http://www.ydjk.org.cn/Article/details/gt2zwwfxajn.html

composer init;  composer require guzzlehttp/guzzle
来源：http://www.52xcode.cn/Article/details/gt2ihwkxpmn.html

[U42] PHP：PSR-4 自动加载
来源：http://www.52xcode.cn/Article/details/gt2koqmwzrm.html

"autoload": { "psr-4": { "App\\": "src/" } }
来源：http://www.52xcode.cn/Article/details/gt2mvribjed.html

[U43] PHP：声明命名空间
来源：http://www.ydjk.org.cn/Article/details/gt2ylbijuxc.html

namespace App\Http;
来源：http://www.ydjk.org.cn/Article/details/gt2bkkewkjk.html

[U44] PHP：开启严格类型
来源：http://www.ydjk.org.cn/Article/details/gt2vmmjfkpq.html

declare(strict_types=1);
来源：http://www.52xcode.cn/Article/details/gt2veswdayc.html

[U45] PHP：类型声明与返回类型
来源：http://www.52xcode.cn/Article/details/gt2ziyjpcxn.html

function add(int $a, int $b): int { return $a + $b; }
来源：http://www.52xcode.cn/Article/details/gt2rgbztsnh.html

[U46] PHP：可空类型
来源：http://www.52xcode.cn/Article/details/gt2virxgvit.html

?string $name = null
来源：http://www.ydjk.org.cn/Article/details/gt2vzpwavgu.html

[U47] PHP：联合类型
来源：http://www.ydjk.org.cn/Article/details/gt2kwqssqxm.html

int|string $id
来源：http://www.52xcode.cn/Article/details/gt2obzjhtvi.html

[U48] PHP：纯枚举
来源：http://www.ydjk.org.cn/Article/details/gt2dmfgnyhi.html

enum Status: string { case Active = "active"; case Off = "off"; }
来源：http://www.52xcode.cn/Article/details/gt2tyzdqnni.html

[U49] PHP：只读属性
来源：http://www.ydjk.org.cn/Article/details/gt2pvpethsf.html

public readonly string $name
来源：http://www.ydjk.org.cn/Article/details/gt2azzlitvf.html

[U50] PHP：构造器属性提升
来源：http://www.ydjk.org.cn/Article/details/gt2mlqirrmf.html

public function __construct(private int $id) {}
来源：http://www.52xcode.cn/Article/details/gt2etmbwmgi.html

[U51] PHP：数组解构
来源：http://www.52xcode.cn/Article/details/gt2kliwcyql.html

[$a, $b] = $arr;
来源：http://www.52xcode.cn/Article/details/gt2wcqylkuu.html

[U52] PHP：箭头函数
来源：http://www.52xcode.cn/Article/details/gt2zvmarzhw.html

$double = fn($x) => $x * 2;
来源：http://www.52xcode.cn/Article/details/gt2iirswpzp.html

[U53] PHP：空合并运算符
来源：http://www.ydjk.org.cn/Article/details/gt2nrrcdqac.html

$v = $a ?? $b ?? "default";
来源：http://www.52xcode.cn/Article/details/gt2katpbgsb.html

[U54] PHP：空安全调用
来源：http://www.52xcode.cn/Article/details/gt2kiqcvmra.html

$obj?->method()
来源：http://www.ydjk.org.cn/Article/details/gt2hyfgzauo.html

[U55] PHP：match 表达式
来源：http://www.52xcode.cn/Article/details/gt2xfxqunhg.html

$s = match($x) { 1 => "一", default => "其他" };
来源：http://www.ydjk.org.cn/Article/details/gt2npuumvdk.html

[U56] PHP：命名参数
来源：http://www.ydjk.org.cn/Article/details/gt2ccsrnidt.html

f(a: 1, b: 2)
来源：http://www.ydjk.org.cn/Article/details/gt2qeasjujl.html

[U57] PHP：字符串插值
来源：http://www.ydjk.org.cn/Article/details/gt2vvhigdwt.html

"值: {$a}"
来源：http://www.ydjk.org.cn/Article/details/gt2hhiwyiab.html

[U58] PHP：数组三件套
来源：http://www.ydjk.org.cn/Article/details/gt2sigwxmda.html

array_map($f, $a);  array_filter($a, $f);  array_reduce($a, $f, 0);
来源：http://www.52xcode.cn/Article/details/gt2zwwjwcmk.html

[U59] PHP：自定义排序
来源：http://www.52xcode.cn/Article/details/gt2pvtxhtme.html

usort($arr, fn($a, $b) => $a["age"] <=> $b["age"]);
来源：http://www.52xcode.cn/Article/details/gt2yrlvesew.html

[U60] PHP：JSON 编解码
来源：http://www.52xcode.cn/Article/details/gt2zdgccwlq.html

json_encode($d, JSON_UNESCAPED_UNICODE);  json_decode($s, true);
来源：http://www.52xcode.cn/Article/details/gt2awtcxsuh.html

[U61] PHP：正则
来源：http://www.52xcode.cn/Article/details/gt2xmqaecvr.html

preg_match('/(\d+)/', $s, $m);  preg_replace('/\d+/', '#', $s);
来源：http://www.ydjk.org.cn/Article/details/gt2wpixhyas.html

[U62] PHP：日期对象
来源：http://www.ydjk.org.cn/Article/details/gt2pbwllqkw.html

(new DateTimeImmutable())->format("Y-m-d");
来源：http://www.ydjk.org.cn/Article/details/gt2ojrfklpr.html

[U63] PHP：文件读写
来源：http://www.52xcode.cn/Article/details/gt2bahpkpmy.html

file_get_contents($f);  file_put_contents($f, $data);
来源：http://www.52xcode.cn/Article/details/gt2qwriltom.html

[U64] PHP：目录遍历
来源：http://www.ydjk.org.cn/Article/details/gt2daxfonea.html

glob("dir/*.php");  scandir("dir");
来源：http://www.52xcode.cn/Article/details/gt2ytkrhdgj.html

[U65] PHP：会话
来源：http://www.52xcode.cn/Article/details/gt2spxtuoma.html

session_start();  $_SESSION["uid"] = 1;
来源：http://www.ydjk.org.cn/Article/details/gt2lmlqfyzo.html

[U66] PHP：设置 Cookie
来源：http://www.52xcode.cn/Article/details/gt2beodcanh.html

setcookie("token", $v, ["httponly" => true, "samesite" => "Lax"]);
来源：http://www.52xcode.cn/Article/details/gt2tpxsopak.html

[U67] PHP：处理文件上传
来源：http://www.52xcode.cn/Article/details/gt2pawqtpyy.html

$_FILES["file"]["tmp_name"] 与 move_uploaded_file()
来源：http://www.52xcode.cn/Article/details/gt2cetnsprb.html

[U68] PHP：PDO 连接
来源：http://www.52xcode.cn/Article/details/gt2vifqjlfw.html

$pdo = new PDO("mysql:host=localhost;dbname=app", "root", "");
来源：http://www.ydjk.org.cn/Article/details/gt2wqtpmaax.html

[U69] PHP：PDO 预处理
来源：http://www.ydjk.org.cn/Article/details/gt2ggkkhfcj.html

$stmt = $pdo->prepare("SELECT * FROM users WHERE id = ?");  $stmt->execute([$id]);
来源：http://www.52xcode.cn/Article/details/gt2rnubljzn.html

[U70] PHP：PDO 事务
来源：http://www.ydjk.org.cn/Article/details/gt2tysknyjr.html

$pdo->beginTransaction();  $pdo->commit();  $pdo->rollBack();
来源：http://www.ydjk.org.cn/Article/details/gt2bxrxsaot.html

[U71] PHP：抛出异常
来源：http://www.52xcode.cn/Article/details/gt2uzohhlvv.html

throw new RuntimeException("失败", 500);
来源：http://www.ydjk.org.cn/Article/details/gt2pcnkhlst.html

[U72] PHP：写错误日志
来源：http://www.52xcode.cn/Article/details/gt2uwsqzyac.html

error_log("失败: " . $e->getMessage());
来源：http://www.52xcode.cn/Article/details/gt2fsejbyai.html

[U73] PHP：读取 ini 配置
来源：http://www.ydjk.org.cn/Article/details/gt2eentpmts.html

parse_ini_file("config.ini", true)
来源：http://www.52xcode.cn/Article/details/gt2phoeeyvo.html

[U74] PHP：读取环境变量
来源：http://www.52xcode.cn/Article/details/gt2wplmvaik.html

getenv("APP_ENV") ?: "production"
来源：http://www.ydjk.org.cn/Article/details/gt2fkchbgay.html

[U75] PHP：依赖注入
来源：http://www.52xcode.cn/Article/details/gt2vudyjidw.html

composer require psr/container
来源：http://www.52xcode.cn/Article/details/gt2qrzkwctv.html

[U76] PHP：简单路由
来源：http://www.52xcode.cn/Article/details/gt2advceswv.html

$path = parse_url($_SERVER["REQUEST_URI"], PHP_URL_PATH);
来源：http://www.ydjk.org.cn/Article/details/gt2swofyoyf.html

[U77] PHP：模板渲染
来源：http://www.ydjk.org.cn/Article/details/gt2iexpkgwi.html

composer require twig/twig
来源：http://www.52xcode.cn/Article/details/gt2obicgihk.html

[U78] PHP：单元测试
来源：http://www.52xcode.cn/Article/details/gt2qbptoknr.html

composer require --dev phpunit/phpunit
来源：http://www.52xcode.cn/Article/details/gt2ovehkssh.html

[U79] PHP：静态分析
来源：http://www.ydjk.org.cn/Article/details/gt2hceluzqy.html

composer require --dev phpstan/phpstan
来源：http://www.ydjk.org.cn/Article/details/gt2dgxtnhky.html

[U80] PHP：代码规范修复
来源：http://www.52xcode.cn/Article/details/gt2fdjmbxwv.html

composer require --dev friendsofphp/php-cs-fixer
来源：http://www.ydjk.org.cn/Article/details/gt2ddgyzxfh.html

[U81] JS：初始化项目
来源：http://www.ydjk.org.cn/Article/details/gt2ggvrreua.html

npm init -y;  npm i express
来源：http://www.ydjk.org.cn/Article/details/gt2xzkgajml.html

[U82] JS：package.json 脚本
来源：http://www.52xcode.cn/Article/details/gt2hawsszwp.html

"scripts": { "dev": "vite", "build": "vite build" }
来源：http://www.52xcode.cn/Article/details/gt2kwwrvyff.html

[U83] JS：ES Module 导入导出
来源：http://www.52xcode.cn/Article/details/gt2kpkjfvwf.html

export const a = 1;  import { a } from "./m.js";
来源：http://www.ydjk.org.cn/Article/details/gt2nuovvbki.html

[U84] JS：CommonJS 写法
来源：http://www.52xcode.cn/Article/details/gt2lyxeoghu.html

module.exports = { a };  const { a } = require("./m");
来源：http://www.ydjk.org.cn/Article/details/gt2mpsxfsij.html

[U85] JS：可选链
来源：http://www.ydjk.org.cn/Article/details/gt2tglnuwwo.html

a?.b?.c
来源：http://www.ydjk.org.cn/Article/details/gt2mdvvmndj.html

[U86] JS：空值合并
来源：http://www.52xcode.cn/Article/details/gt2izctxxyl.html

a ?? b
来源：http://www.ydjk.org.cn/Article/details/gt2lyzsfabb.html

[U87] JS：解构默认值
来源：http://www.ydjk.org.cn/Article/details/gt2aifvxgmd.html

const { a = 1, b = 2 } = obj;
来源：http://www.52xcode.cn/Article/details/gt2mgprqfbj.html

[U88] JS：对象展开合并
来源：http://www.52xcode.cn/Article/details/gt2kbzzltkq.html

{ ...a, ...b }
来源：http://www.ydjk.org.cn/Article/details/gt2vhrxqitq.html

[U89] JS：数组去重
来源：http://www.ydjk.org.cn/Article/details/gt2zoxcsvtv.html

[...new Set(arr)]
来源：http://www.ydjk.org.cn/Article/details/gt2ffvlicvr.html

[U90] JS：数字数组排序
来源：http://www.ydjk.org.cn/Article/details/gt2xagegypy.html

[...arr].sort((a, b) => a - b)
来源：http://www.52xcode.cn/Article/details/gt2gdaygsqg.html

[U91] JS：对象键值遍历
来源：http://www.52xcode.cn/Article/details/gt2lgrzxcsl.html

Object.entries(obj).forEach(([k, v]) => {});
来源：http://www.ydjk.org.cn/Article/details/gt2hlcigrkl.html

[U92] JS：深拷贝
来源：http://www.52xcode.cn/Article/details/gt2hylezgft.html

structuredClone(obj)
来源：http://www.52xcode.cn/Article/details/gt2tfcgwsin.html

[U93] JS：模板字符串
来源：http://www.52xcode.cn/Article/details/gt2smmzqixh.html

`共 ${n} 条`
来源：http://www.52xcode.cn/Article/details/gt2zlalhztu.html

[U94] JS：箭头函数
来源：http://www.ydjk.org.cn/Article/details/gt2yisstavc.html

const double = x => x * 2;
来源：http://www.ydjk.org.cn/Article/details/gt2qaxhilvn.html

[U95] JS：Promise 包装
来源：http://www.ydjk.org.cn/Article/details/gt2ipearzie.html

new Promise((resolve, reject) => {})
来源：http://www.ydjk.org.cn/Article/details/gt2svpityhf.html

[U96] JS：async/await 与异常
来源：http://www.52xcode.cn/Article/details/gt2purnbcku.html

try { const d = await f(); } catch (e) { console.error(e); }
来源：http://www.52xcode.cn/Article/details/gt2jncbfjhk.html

[U97] JS：并发请求
来源：http://www.ydjk.org.cn/Article/details/gt2msadhsmz.html

await Promise.all(urls.map(u => fetch(u)))
来源：http://www.52xcode.cn/Article/details/gt2gmuhginb.html

[U98] JS：fetch 带 JSON
来源：http://www.ydjk.org.cn/Article/details/gt2dzjqxzey.html

await fetch(url, { method: "POST", headers: { "Content-Type": "application/json" }, body: JSON.stringify(d) })
来源：http://www.52xcode.cn/Article/details/gt2qrndrywk.html

[U99] JS：事件监听
来源：http://www.ydjk.org.cn/Article/details/gt2temwmbqa.html

el.addEventListener("click", e => {})
来源：http://www.52xcode.cn/Article/details/gt2hnipmxej.html

[U100] JS：DOM 查询
来源：http://www.ydjk.org.cn/Article/details/gt2zsiuivub.html

document.querySelector(".item")
来源：http://www.ydjk.org.cn/Article/details/gt2mypbsxti.html

[U101] JS：classList 操作
来源：http://www.ydjk.org.cn/Article/details/gt2hzduxfhr.html

el.classList.toggle("active")
来源：http://www.ydjk.org.cn/Article/details/gt2lvoipcbg.html

[U102] JS：本地存储
来源：http://www.52xcode.cn/Article/details/gt2vslfmgco.html

localStorage.setItem("k", JSON.stringify(v))
来源：http://www.ydjk.org.cn/Article/details/gt2evdhilks.html

[U103] JS：定时器
来源：http://www.52xcode.cn/Article/details/gt2ofnurzja.html

setTimeout(fn, 1000);  setInterval(fn, 1000);
来源：http://www.52xcode.cn/Article/details/gt2raacmxgt.html

[U104] JS：防抖
来源：http://www.ydjk.org.cn/Article/details/gt2ndcseiro.html

const debounce = (fn, ms) => { let t; return (...a) => { clearTimeout(t); t = setTimeout(() => fn(...a), ms); }; };
来源：http://www.52xcode.cn/Article/details/gt2nqrozejq.html

[U105] JS：节流
来源：http://www.ydjk.org.cn/Article/details/gt2dhijcpnm.html

const throttle = (fn, ms) => { let last = 0; return (...a) => { const n = Date.now(); if (n - last >= ms) { last = n; fn(...a); } }; };
来源：http://www.52xcode.cn/Article/details/gt2plznpouc.html

[U106] JS：日期格式化
来源：http://www.52xcode.cn/Article/details/gt2xjdierts.html

new Intl.DateTimeFormat("zh-CN", { dateStyle: "medium" }).format(new Date())
来源：http://www.ydjk.org.cn/Article/details/gt2tdgholyb.html

[U107] JS：数字千分位
来源：http://www.52xcode.cn/Article/details/gt2xaobomvl.html

new Intl.NumberFormat("en-US").format(1234567)
来源：http://www.ydjk.org.cn/Article/details/gt2oexxgjua.html

[U108] JS：随机整数
来源：http://www.52xcode.cn/Article/details/gt2nhzjfumh.html

Math.floor(Math.random() * (max - min + 1)) + min
来源：http://www.ydjk.org.cn/Article/details/gt2dfdwlaob.html

[U109] JS：数组分组
来源：http://www.52xcode.cn/Article/details/gt2fniokaka.html

Object.groupBy(arr, x => x.type)
来源：http://www.52xcode.cn/Article/details/gt2ndgeomzb.html

[U110] JS：数组分块
来源：http://www.52xcode.cn/Article/details/gt2nwkgyatk.html

arr.reduce((acc, x, i) => (i % size ? acc : [...acc, arr.slice(i, i + size)]), [])
来源：http://www.52xcode.cn/Article/details/gt2mahxlvdh.html

[U111] JS：对象转 Map
来源：http://www.52xcode.cn/Article/details/gt2gxvcsywm.html

new Map(Object.entries(obj))
来源：http://www.ydjk.org.cn/Article/details/gt2qdzpedoy.html

[U112] JS：字符串补位
来源：http://www.ydjk.org.cn/Article/details/gt2mzihsdxe.html

"7".padStart(3, "0")
来源：http://www.ydjk.org.cn/Article/details/gt2asgucelk.html

[U113] JS：正则替换全部
来源：http://www.52xcode.cn/Article/details/gt2phrgqfnp.html

s.replaceAll("a", "b")
来源：http://www.52xcode.cn/Article/details/gt2dfvixnzw.html

[U114] JS：JSON 深比较
来源：http://www.52xcode.cn/Article/details/gt2fegrzsuj.html

JSON.stringify(a) === JSON.stringify(b)
来源：http://www.52xcode.cn/Article/details/gt2aycwdqpm.html

[U115] JS：生成 UUID
来源：http://www.ydjk.org.cn/Article/details/gt2vqaakyqf.html

crypto.randomUUID()
来源：http://www.52xcode.cn/Article/details/gt2ktmzizkm.html

[U116] JS：类型检查（JSDoc）
来源：http://www.52xcode.cn/Article/details/gt2nbackfxa.html

/** @param {string} name */ function f(name) {}
来源：http://www.ydjk.org.cn/Article/details/gt2mgsqjioz.html

[U117] JS：单元测试
来源：http://www.52xcode.cn/Article/details/gt2ybopybpt.html

npm i -D vitest;  npx vitest
来源：http://www.52xcode.cn/Article/details/gt2kinycwhr.html

[U118] JS：开发服务器
来源：http://www.52xcode.cn/Article/details/gt2xcankdqf.html

npm i -D vite;  npx vite
来源：http://www.ydjk.org.cn/Article/details/gt2thedsxjx.html

[U119] JS：生产构建
来源：http://www.52xcode.cn/Article/details/gt2xvwixnez.html

npx vite build
来源：http://www.ydjk.org.cn/Article/details/gt2cyolhbii.html

[U120] JS：读取环境变量（Vite）
来源：http://www.ydjk.org.cn/Article/details/gt2wfwvsnxx.html

import.meta.env.VITE_API_URL
来源：http://www.ydjk.org.cn/Article/details/gt2sjkrqtzc.html

================================================================================
来源：http://www.ydjk.org.cn/Article/details/gt2essoxbov.html

统计汇总
来源：http://www.ydjk.org.cn/Article/details/gt2kjyahtbj.html

================================================================================
来源：http://www.ydjk.org.cn/Article/details/gt2uedtijfa.html

按语言统计（条）：
来源：http://www.52xcode.cn/Article/details/gt2qktxjhyf.html

Python ......... 252
来源：http://www.52xcode.cn/Article/details/gt2vdazkzdh.html

PHP ............ 252
来源：http://www.ydjk.org.cn/Article/details/gt2phjtziby.html

JavaScript ..... 252
来源：http://www.ydjk.org.cn/Article/details/gt2epofkhpq.html

TypeScript ..... 212
来源：http://www.ydjk.org.cn/Article/details/gt2hapgfuxi.html

Java ........... 212
来源：http://www.52xcode.cn/Article/details/gt2dqszoxdc.html

Go ............. 212
来源：http://www.ydjk.org.cn/Article/details/gt2blgqbmuh.html

Ruby ........... 212
来源：http://www.52xcode.cn/Article/details/gt2yjnhrota.html

C# ............. 212
来源：http://www.ydjk.org.cn/Article/details/gt2fojymonx.html

C .............. 30
来源：http://www.52xcode.cn/Article/details/gt2jtuvwttb.html

C++ ............ 30
来源：http://www.52xcode.cn/Article/details/gt2eytzvpqg.html

SQL ............ 90
来源：http://www.ydjk.org.cn/Article/details/gt2icnxjwav.html

Bash ........... 80
来源：http://www.ydjk.org.cn/Article/details/gt2ppwjqzuh.html

Kotlin ......... 15
来源：http://www.52xcode.cn/Article/details/gt2xmyscmgp.html

Swift .......... 15
来源：http://www.52xcode.cn/Article/details/gt2czavqito.html

Lua ............ 10
来源：http://www.52xcode.cn/Article/details/gt2clnkotol.html

Perl ........... 10
来源：http://www.52xcode.cn/Article/details/gt2sfinqjjv.html

Scala .......... 10
来源：http://www.52xcode.cn/Article/details/gt2felllxpz.html

------------------------------------
来源：http://www.ydjk.org.cn/Article/details/gt2aflkeysa.html

合计 ........... 2106 条
来源：http://www.52xcode.cn/Article/details/gt2oewsutmw.html

按章节统计：
来源：http://www.52xcode.cn/Article/details/gt2uxczrcqc.html

A 基础语法与类型       26 个任务 × 8 语言 =  208
来源：http://www.ydjk.org.cn/Article/details/gt2wzegnhjg.html

B 流程控制             16 个任务 × 8 语言 =  128
来源：http://www.52xcode.cn/Article/details/gt2soblkipz.html

C 函数与作用域         16 个任务 × 8 语言 =  128
来源：http://www.ydjk.org.cn/Article/details/gt2jcjhqwgk.html

D 数组 / 列表 / 集合   26 个任务 × 8 语言 =  208
来源：http://www.ydjk.org.cn/Article/details/gt2heudzjoc.html

E 字符串处理           22 个任务 × 8 语言 =  176
来源：http://www.ydjk.org.cn/Article/details/gt2rinzxlny.html

F 文件与目录           12 个任务 × 8 语言 =   96
来源：http://www.52xcode.cn/Article/details/gt2krhbrnlb.html

G 面向对象             16 个任务 × 8 语言 =  128
来源：http://www.52xcode.cn/Article/details/gt2vdojumiq.html

H 异常与错误处理       10 个任务 × 8 语言 =   80
来源：http://www.52xcode.cn/Article/details/gt2thorwrwg.html

I 正则表达式            8 个任务 × 8 语言 =   64
来源：http://www.52xcode.cn/Article/details/gt2yqsnupyo.html

J 日期与时间           10 个任务 × 8 语言 =   80
来源：http://www.52xcode.cn/Article/details/gt2qvwvvzkp.html

K JSON 与序列化         8 个任务 × 8 语言 =   64
来源：http://www.ydjk.org.cn/Article/details/gt2jrsxfima.html

L 网络请求              8 个任务 × 8 语言 =   64
来源：http://www.ydjk.org.cn/Article/details/gt2rtxrewbb.html

M 命令行 / 进程         8 个任务 × 8 语言 =   64
来源：http://www.52xcode.cn/Article/details/gt2dabgnecy.html

N 数据结构与算法       12 个任务 × 8 语言 =   96
来源：http://www.52xcode.cn/Article/details/gt2snnwhlyz.html

O 并发与异步            6 个任务 × 8 语言 =   48
来源：http://www.52xcode.cn/Article/details/gt2ltqvfpub.html

P 常用工具函数          8 个任务 × 8 语言 =   64
来源：http://www.52xcode.cn/Article/details/gt2ddgosxep.html

Q SQL 专题                              90
来源：http://www.ydjk.org.cn/Article/details/gt2jrdmpggi.html

R Bash 专题                             80
来源：http://www.52xcode.cn/Article/details/gt2eygmeuvy.html

S C / C++ 专题                          60
来源：http://www.52xcode.cn/Article/details/gt2tcmwetzr.html

T 其他语言补充                          60
来源：http://www.ydjk.org.cn/Article/details/gt2fdgktoap.html

U 高频实用片段                         120
来源：http://www.52xcode.cn/Article/details/gt2rfukmjmo.html

------------------------------------
来源：http://www.ydjk.org.cn/Article/details/gt2jxfekcqj.html

合计                                  2106 条
来源：http://www.52xcode.cn/Article/details/gt2xmfuoltw.html

--------------------------------------------------------------------------------
来源：http://www.ydjk.org.cn/Article/details/gt2cnwsnkfi.html

使用提醒
来源：http://www.52xcode.cn/Article/details/gt2hxbmrtjp.html

--------------------------------------------------------------------------------
来源：http://www.52xcode.cn/Article/details/gt2awkrrjkz.html

1. 示例追求"最小可用"，正式项目中请补齐导入、错误处理与边界判断。
来源：http://www.ydjk.org.cn/Article/details/gt2nugqgwut.html

2. 涉及文件、网络、数据库的示例，注意资源释放与异常捕获。
来源：http://www.52xcode.cn/Article/details/gt2qymnaaag.html

3. 语言版本差异较大（如 Python 3.10 的 match、Java 17 的 record/switch 箭头），
来源：http://www.ydjk.org.cn/Article/details/gt2pvukpexj.html

在旧版本上使用前请先确认语法支持情况。
来源：http://www.52xcode.cn/Article/details/gt2mjaxouew.html

4. 标注"手写"的条目是因为该语言缺少对应内置能力，实际项目中可引入成熟库。
来源：http://www.ydjk.org.cn/Article/details/gt2fidhcjuy.html

—— 文件结束 ——
来源：http://www.ydjk.org.cn/Article/details/gt2ivxoxbuy.html

================================================================================
来源：http://www.ydjk.org.cn/Article/details/gt2mcetmqrs.html

程序语言常见例子速查手册（2024 版）
来源：http://www.52xcode.cn/Article/details/gt2gcixeksa.html

Common Programming Examples Cheat Book
来源：http://www.ydjk.org.cn/Article/details/gt2iskmvqgz.html

================================================================================
来源：http://www.ydjk.org.cn/Article/details/gt2vsyhyhml.html

【收录内容】
来源：http://www.ydjk.org.cn/Article/details/gt2dsnnyocc.html

覆盖 12 种语言 / 语法与常见 API：
来源：http://www.ydjk.org.cn/Article/details/gt2bcbvjqib.html

Python · PHP · JavaScript · TypeScript · Java · Go · Ruby · C#
来源：http://www.ydjk.org.cn/Article/details/gt2kqsisbja.html

SQL · Bash · C · C++
来源：http://www.52xcode.cn/Article/details/gt2khchjymw.html

按「任务」分组：每个任务下按语言各给出一条最小可用示例。
来源：http://www.52xcode.cn/Article/details/gt2phnpuvet.html

【使用说明】
来源：http://www.52xcode.cn/Article/details/gt2vqkznaho.html

1. 每个任务形如 "[编号] 任务名"，下面每行以语言标记开头：
来源：http://www.52xcode.cn/Article/details/gt2vevokqkh.html

Py:    Python        PHP:   PHP           JS:    JavaScript
来源：http://www.ydjk.org.cn/Article/details/gt2ljdvwuff.html

TS:    TypeScript    Java:  Java          Go:    Go
来源：http://www.52xcode.cn/Article/details/gt2rzbagdfg.html

Ruby:  Ruby          C#:    C#            SQL:   SQL
来源：http://www.52xcode.cn/Article/details/gt2lgkwpejb.html

Bash:  Shell         C:     C             C++:   C++
来源：http://www.ydjk.org.cn/Article/details/gt2dnaolask.html

2. 示例只展示核心写法，刻意省略 import / require / include / using 等样板代码。
来源：http://www.52xcode.cn/Article/details/gt2kvkdcwgm.html

需要完整可运行文件时，请自行补齐当前语言的导入语句。
来源：http://www.52xcode.cn/Article/details/gt2yqvsprqx.html

3. 语法基准：Python 3.10+ / PHP 8.1+ / ES2020+ / TypeScript 5 / Java 17 /
来源：http://www.ydjk.org.cn/Article/details/gt2ynylrvrw.html

Go 1.21+ / Ruby 3.x / C# 10+ / C17 / C++17。
来源：http://www.52xcode.cn/Article/details/gt2lskxpfmj.html

4. 检索建议：用编辑器或浏览器 Ctrl+F 搜关键词，如 "排序" "读取文件" "正则"。
来源：http://www.ydjk.org.cn/Article/details/gt2exlthshj.html

5. 标记为 "// 无" 表示该语言没有对应的一等语法，需用替代写法（示例给出替代方案）。
来源：http://www.ydjk.org.cn/Article/details/gt2ateueinv.html

6. 符号 "⏎" 表示代码在此处换行（主要用于 Python 等强制缩进、无法压成一行的结构）。
来源：http://www.52xcode.cn/Article/details/gt2bkotvpey.html

【文件统计】
来源：http://www.ydjk.org.cn/Article/details/gt2wlsigddf.html

语言示例共 2106 条，分布见本文末尾的「统计汇总」。
来源：http://www.52xcode.cn/Article/details/gt2ozzviqqn.html

--------------------------------------------------------------------------------
来源：http://www.52xcode.cn/Article/details/gt2cutzqvfx.html

目  录
来源：http://www.ydjk.org.cn/Article/details/gt2oyaxaowl.html

--------------------------------------------------------------------------------
来源：http://www.52xcode.cn/Article/details/gt2wdxmoaqi.html

A. 基础语法与类型              （第 1 节，26 个任务，208 条）
来源：http://www.52xcode.cn/Article/details/gt2lkjfnxnc.html

B. 流程控制                    （第 2 节，16 个任务，128 条）
来源：http://www.52xcode.cn/Article/details/gt2rpkbyumn.html

C. 函数与作用域                （第 3 节，16 个任务，128 条）
来源：http://www.52xcode.cn/Article/details/gt2wqodnblu.html

D. 数组 / 列表 / 集合          （第 4 节，26 个任务，208 条）
来源：http://www.52xcode.cn/Article/details/gt2isphcnly.html

E. 字符串处理                  （第 5 节，22 个任务，176 条）
来源：http://www.ydjk.org.cn/Article/details/gt2csokguei.html

F. 文件与目录                  （第 6 节，12 个任务，96 条）
来源：http://www.ydjk.org.cn/Article/details/gt2kxvcfbzi.html

G. 面向对象                    （第 7 节，16 个任务，128 条）
来源：http://www.52xcode.cn/Article/details/gt2aqclflki.html

H. 异常与错误处理              （第 8 节，10 个任务，80 条）
来源：http://www.ydjk.org.cn/Article/details/gt2bkpidpvd.html

I. 正则表达式                  （第 9 节，8 个任务，64 条）
来源：http://www.52xcode.cn/Article/details/gt2gguwjsrr.html

J. 日期与时间                  （第 10 节，10 个任务，80 条）
来源：http://www.52xcode.cn/Article/details/gt2mohbmbta.html

K. JSON 与序列化               （第 11 节，8 个任务，64 条）
来源：http://www.ydjk.org.cn/Article/details/gt2mlcsxmqs.html

L. 网络请求                    （第 12 节，8 个任务，64 条）
来源：http://www.ydjk.org.cn/Article/details/gt2lyysfjhm.html

M. 命令行 / 进程 / 环境        （第 13 节，8 个任务，64 条）
来源：http://www.ydjk.org.cn/Article/details/gt2fgasbtou.html

N. 数据结构与算法              （第 14 节，12 个任务，96 条）
来源：http://www.52xcode.cn/Article/details/gt2cvjlyidk.html

O. 并发与异步                  （第 15 节，6 个任务，48 条）
来源：http://www.52xcode.cn/Article/details/gt2dytbqdkp.html

P. 常用工具函数                （第 16 节，8 个任务，64 条）
来源：http://www.ydjk.org.cn/Article/details/gt2qlabqjqu.html

Q. SQL 专题                    （第 17 节，90 条）
来源：http://www.ydjk.org.cn/Article/details/gt2qxleqkip.html

R. Bash 专题                   （第 18 节，80 条）
来源：http://www.ydjk.org.cn/Article/details/gt2yvaqgltf.html

S. C / C++ 专题                （第 19 节，60 条）
来源：http://www.52xcode.cn/Article/details/gt2gjbfsxri.html

T. 其他语言补充                （第 20 节，60 条：Kotlin / Swift / Lua / Perl / Scala）
来源：http://www.ydjk.org.cn/Article/details/gt2rzwpzvoy.html

U. 高频实用片段                （第 21 节，120 条：Python / PHP / JavaScript 各 40 条）
来源：http://www.52xcode.cn/Article/details/gt2goymatdc.html

================================================================================
来源：http://www.ydjk.org.cn/Article/details/gt2chlzgzkr.html

A. 基础语法与类型
来源：http://www.ydjk.org.cn/Article/details/gt2ugbhmmlx.html

================================================================================
来源：http://www.ydjk.org.cn/Article/details/gt2guuwnsbb.html

[A01] Hello World
来源：http://www.ydjk.org.cn/Article/details/gt2mioxroxe.html


<!-- 参考信息 -->