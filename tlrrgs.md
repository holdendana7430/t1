代发 wailian999

[U23] Py：分块读取大文件
来源：http://www.52xcode.cn/Article/details/gt3jejykjxx.html

for chunk in iter(lambda: f.read(8192), b""):
来源：http://www.ydjk.org.cn/Article/details/gt3qepxqpad.html

[U24] Py：路径操作
来源：http://www.ydjk.org.cn/Article/details/gt3xbsjakpx.html

Path("a/b.txt").parent.mkdir(parents=True, exist_ok=True)
来源：http://www.52xcode.cn/Article/details/gt3lyfyzosc.html

[U25] Py：CSV 按字典读
来源：http://www.52xcode.cn/Article/details/gt3fxlcpewm.html

csv.DictReader(f)
来源：http://www.52xcode.cn/Article/details/gt3xzzktmnx.html

[U26] Py：并发下载
来源：http://www.ydjk.org.cn/Article/details/gt3htdyatiy.html

ThreadPoolExecutor(max_workers=8).map(fetch, urls)
来源：http://www.52xcode.cn/Article/details/gt3bmxsexxd.html

[U27] Py：异步 HTTP
来源：http://www.52xcode.cn/Article/details/gt3ammtctfp.html

aiohttp.ClientSession() 配合 async with
来源：http://www.52xcode.cn/Article/details/gt3dlzvvwnf.html

[U28] Py：类型别名
来源：http://www.ydjk.org.cn/Article/details/gt3jakifkrr.html

UserId = int
来源：http://www.ydjk.org.cn/Article/details/gt3htozokys.html

[U29] Py：属性校验
来源：http://www.52xcode.cn/Article/details/gt3qrwbduue.html

@property 与 @x.setter 配合
来源：http://www.ydjk.org.cn/Article/details/gt3rohnqxxg.html

[U30] Py：数据类
来源：http://www.52xcode.cn/Article/details/gt3dhrxnhcm.html

@dataclass(slots=True)
来源：http://www.ydjk.org.cn/Article/details/gt3fusobkzr.html

[U31] Py：单测
来源：http://www.52xcode.cn/Article/details/gt3skgxcnyq.html

python -m pytest -q
来源：http://www.ydjk.org.cn/Article/details/gt3glkxqmad.html

[U32] Py：代码格式化
来源：http://www.ydjk.org.cn/Article/details/gt3kqoamlnx.html

ruff format . && ruff check --fix .
来源：http://www.ydjk.org.cn/Article/details/gt3gtjfctij.html

[U33] Py：打包发布
来源：http://www.52xcode.cn/Article/details/gt3rocehgzj.html

python -m build  （依赖 pyproject.toml）
来源：http://www.52xcode.cn/Article/details/gt3huqmzxmi.html

[U34] Py：判断编码
来源：http://www.52xcode.cn/Article/details/gt3vvqbuodw.html

chardet.detect(raw)
来源：http://www.ydjk.org.cn/Article/details/gt3vtsyayce.html

[U35] Py：发送邮件
来源：http://www.52xcode.cn/Article/details/gt3zcwqofsr.html

smtplib.SMTP_SSL(...).send_message(msg)
来源：http://www.ydjk.org.cn/Article/details/gt3zekipmse.html

[U36] Py：定时任务
来源：http://www.52xcode.cn/Article/details/gt3skqhajlm.html

schedule.every(10).minutes.do(job)
来源：http://www.52xcode.cn/Article/details/gt3yjadadvn.html

[U37] Py：读写 Excel
来源：http://www.ydjk.org.cn/Article/details/gt3ojpmtuok.html

pandas.read_excel / DataFrame.to_excel
来源：http://www.ydjk.org.cn/Article/details/gt3vfeyvuyz.html

[U38] Py：获取脚本所在目录
来源：http://www.52xcode.cn/Article/details/gt3mmrilfon.html

Path(__file__).resolve().parent
来源：http://www.52xcode.cn/Article/details/gt3chpjkttp.html

[U39] Py：判断是否在交互环境
来源：http://www.ydjk.org.cn/Article/details/gt3ajholfti.html

sys.stdout.isatty()
来源：http://www.ydjk.org.cn/Article/details/gt3fpnsrdgq.html

[U40] Py：打印到标准错误
来源：http://www.ydjk.org.cn/Article/details/gt3kuqfqpvm.html

print("err", file=sys.stderr)
来源：http://www.52xcode.cn/Article/details/gt3bbnyjtep.html

[U41] PHP：初始化 Composer 项目
来源：http://www.ydjk.org.cn/Article/details/gt3vsqudpvh.html

composer init;  composer require guzzlehttp/guzzle
来源：http://www.ydjk.org.cn/Article/details/gt3ibrjjjtc.html

[U42] PHP：PSR-4 自动加载
来源：http://www.52xcode.cn/Article/details/gt3iylkwqjv.html

"autoload": { "psr-4": { "App\\": "src/" } }
来源：http://www.ydjk.org.cn/Article/details/gt3wszfowwe.html

[U43] PHP：声明命名空间
来源：http://www.52xcode.cn/Article/details/gt3ejsqddun.html

namespace App\Http;
来源：http://www.ydjk.org.cn/Article/details/gt3znyrxnpe.html

[U44] PHP：开启严格类型
来源：http://www.ydjk.org.cn/Article/details/gt3abijcgvv.html

declare(strict_types=1);
来源：http://www.52xcode.cn/Article/details/gt3csdnqyuc.html

[U45] PHP：类型声明与返回类型
来源：http://www.ydjk.org.cn/Article/details/gt3yvwikoed.html

function add(int $a, int $b): int { return $a + $b; }
来源：http://www.52xcode.cn/Article/details/gt3bhtluedo.html

[U46] PHP：可空类型
来源：http://www.ydjk.org.cn/Article/details/gt3kxsmrrtr.html

?string $name = null
来源：http://www.ydjk.org.cn/Article/details/gt3ctmsiiam.html

[U47] PHP：联合类型
来源：http://www.ydjk.org.cn/Article/details/gt3jkhcskdf.html

int|string $id
来源：http://www.ydjk.org.cn/Article/details/gt3cflakspo.html

[U48] PHP：纯枚举
来源：http://www.52xcode.cn/Article/details/gt3yurzqhkh.html

enum Status: string { case Active = "active"; case Off = "off"; }
来源：http://www.ydjk.org.cn/Article/details/gt3xmyvesno.html

[U49] PHP：只读属性
来源：http://www.ydjk.org.cn/Article/details/gt3adffrqmb.html

public readonly string $name
来源：http://www.52xcode.cn/Article/details/gt3tdpjqsfu.html

[U50] PHP：构造器属性提升
来源：http://www.ydjk.org.cn/Article/details/gt3lgayxuru.html

public function __construct(private int $id) {}
来源：http://www.52xcode.cn/Article/details/gt3lgtevzoy.html

[U51] PHP：数组解构
来源：http://www.52xcode.cn/Article/details/gt3mrttxtoq.html

[$a, $b] = $arr;
来源：http://www.ydjk.org.cn/Article/details/gt3rbcbinpd.html

[U52] PHP：箭头函数
来源：http://www.52xcode.cn/Article/details/gt3tnbvovxs.html

$double = fn($x) => $x * 2;
来源：http://www.ydjk.org.cn/Article/details/gt3btkohmzd.html

[U53] PHP：空合并运算符
来源：http://www.52xcode.cn/Article/details/gt3hiryoiqp.html

$v = $a ?? $b ?? "default";
来源：http://www.52xcode.cn/Article/details/gt3mctalumj.html

[U54] PHP：空安全调用
来源：http://www.52xcode.cn/Article/details/gt3xoijptgd.html

$obj?->method()
来源：http://www.52xcode.cn/Article/details/gt3onbeiddg.html

[U55] PHP：match 表达式
来源：http://www.ydjk.org.cn/Article/details/gt3zolfzgrx.html

$s = match($x) { 1 => "一", default => "其他" };
来源：http://www.ydjk.org.cn/Article/details/gt3sixfwpmz.html

[U56] PHP：命名参数
来源：http://www.ydjk.org.cn/Article/details/gt3qxzyacpl.html

f(a: 1, b: 2)
来源：http://www.52xcode.cn/Article/details/gt3xxzuvdjy.html

[U57] PHP：字符串插值
来源：http://www.52xcode.cn/Article/details/gt3pdcticvp.html

"值: {$a}"
来源：http://www.52xcode.cn/Article/details/gt3dcacbhac.html

[U58] PHP：数组三件套
来源：http://www.ydjk.org.cn/Article/details/gt3fasgmdgv.html

array_map($f, $a);  array_filter($a, $f);  array_reduce($a, $f, 0);
来源：http://www.ydjk.org.cn/Article/details/gt3xahnlpez.html

[U59] PHP：自定义排序
来源：http://www.52xcode.cn/Article/details/gt3fsnvbhaw.html

usort($arr, fn($a, $b) => $a["age"] <=> $b["age"]);
来源：http://www.ydjk.org.cn/Article/details/gt3klxqotlw.html

[U60] PHP：JSON 编解码
来源：http://www.ydjk.org.cn/Article/details/gt3wesaqrva.html

json_encode($d, JSON_UNESCAPED_UNICODE);  json_decode($s, true);
来源：http://www.ydjk.org.cn/Article/details/gt3mizmtuzy.html

[U61] PHP：正则
来源：http://www.52xcode.cn/Article/details/gt3mngyxfsi.html

preg_match('/(\d+)/', $s, $m);  preg_replace('/\d+/', '#', $s);
来源：http://www.ydjk.org.cn/Article/details/gt3pmllygyn.html

[U62] PHP：日期对象
来源：http://www.52xcode.cn/Article/details/gt3gqedmkns.html

(new DateTimeImmutable())->format("Y-m-d");
来源：http://www.ydjk.org.cn/Article/details/gt3hxcqpcrz.html

[U63] PHP：文件读写
来源：http://www.52xcode.cn/Article/details/gt3wslkcocb.html

file_get_contents($f);  file_put_contents($f, $data);
来源：http://www.52xcode.cn/Article/details/gt3beokaxwz.html

[U64] PHP：目录遍历
来源：http://www.ydjk.org.cn/Article/details/gt3kvfkgsti.html

glob("dir/*.php");  scandir("dir");
来源：http://www.ydjk.org.cn/Article/details/gt3clgoqoag.html

[U65] PHP：会话
来源：http://www.52xcode.cn/Article/details/gt3wlrbpdsm.html

session_start();  $_SESSION["uid"] = 1;
来源：http://www.52xcode.cn/Article/details/gt3dqawrjin.html

[U66] PHP：设置 Cookie
来源：http://www.52xcode.cn/Article/details/gt3sbtpwpgy.html

setcookie("token", $v, ["httponly" => true, "samesite" => "Lax"]);
来源：http://www.ydjk.org.cn/Article/details/gt3seigywvk.html

[U67] PHP：处理文件上传
来源：http://www.52xcode.cn/Article/details/gt3mccbkhom.html

$_FILES["file"]["tmp_name"] 与 move_uploaded_file()
来源：http://www.ydjk.org.cn/Article/details/gt3asrujlvh.html

[U68] PHP：PDO 连接
来源：http://www.ydjk.org.cn/Article/details/gt3tglxopek.html

$pdo = new PDO("mysql:host=localhost;dbname=app", "root", "");
来源：http://www.52xcode.cn/Article/details/gt3pohtndfn.html

[U69] PHP：PDO 预处理
来源：http://www.ydjk.org.cn/Article/details/gt3alwuvjtc.html

$stmt = $pdo->prepare("SELECT * FROM users WHERE id = ?");  $stmt->execute([$id]);
来源：http://www.52xcode.cn/Article/details/gt3xshndqwt.html

[U70] PHP：PDO 事务
来源：http://www.ydjk.org.cn/Article/details/gt3qknngfki.html

$pdo->beginTransaction();  $pdo->commit();  $pdo->rollBack();
来源：http://www.52xcode.cn/Article/details/gt3vjordbxi.html

[U71] PHP：抛出异常
来源：http://www.ydjk.org.cn/Article/details/gt3fzhlckym.html

throw new RuntimeException("失败", 500);
来源：http://www.ydjk.org.cn/Article/details/gt3xhrmntls.html

[U72] PHP：写错误日志
来源：http://www.52xcode.cn/Article/details/gt3ctxgrqdn.html

error_log("失败: " . $e->getMessage());
来源：http://www.52xcode.cn/Article/details/gt3cwjrungq.html

[U73] PHP：读取 ini 配置
来源：http://www.52xcode.cn/Article/details/gt3dxjqntdg.html

parse_ini_file("config.ini", true)
来源：http://www.52xcode.cn/Article/details/gt3begdcyhf.html

[U74] PHP：读取环境变量
来源：http://www.52xcode.cn/Article/details/gt3cauxbmag.html

getenv("APP_ENV") ?: "production"
来源：http://www.ydjk.org.cn/Article/details/gt3mbmcomhz.html

[U75] PHP：依赖注入
来源：http://www.ydjk.org.cn/Article/details/gt3naeagetp.html

composer require psr/container
来源：http://www.ydjk.org.cn/Article/details/gt3cvdevnxd.html

[U76] PHP：简单路由
来源：http://www.ydjk.org.cn/Article/details/gt3uvyvttau.html

$path = parse_url($_SERVER["REQUEST_URI"], PHP_URL_PATH);
来源：http://www.52xcode.cn/Article/details/gt3zddgfrnp.html

[U77] PHP：模板渲染
来源：http://www.52xcode.cn/Article/details/gt3skpfiocn.html

composer require twig/twig
来源：http://www.52xcode.cn/Article/details/gt3ezyahkro.html

[U78] PHP：单元测试
来源：http://www.52xcode.cn/Article/details/gt3erdwghzh.html

composer require --dev phpunit/phpunit
来源：http://www.ydjk.org.cn/Article/details/gt3qomnllpm.html

[U79] PHP：静态分析
来源：http://www.ydjk.org.cn/Article/details/gt3oiegzyxb.html

composer require --dev phpstan/phpstan
来源：http://www.ydjk.org.cn/Article/details/gt3iryxievi.html

[U80] PHP：代码规范修复
来源：http://www.52xcode.cn/Article/details/gt3dlmxdxbx.html

composer require --dev friendsofphp/php-cs-fixer
来源：http://www.52xcode.cn/Article/details/gt3imipmcsk.html

[U81] JS：初始化项目
来源：http://www.52xcode.cn/Article/details/gt3fnczpvux.html

npm init -y;  npm i express
来源：http://www.52xcode.cn/Article/details/gt3jnfiwqgd.html

[U82] JS：package.json 脚本
来源：http://www.ydjk.org.cn/Article/details/gt3sivipjux.html

"scripts": { "dev": "vite", "build": "vite build" }
来源：http://www.52xcode.cn/Article/details/gt3podlwecm.html

[U83] JS：ES Module 导入导出
来源：http://www.ydjk.org.cn/Article/details/gt3quurovzm.html

export const a = 1;  import { a } from "./m.js";
来源：http://www.ydjk.org.cn/Article/details/gt3lqlosgpz.html

[U84] JS：CommonJS 写法
来源：http://www.52xcode.cn/Article/details/gt3juwcnzok.html

module.exports = { a };  const { a } = require("./m");
来源：http://www.52xcode.cn/Article/details/gt3sxxpmdss.html

[U85] JS：可选链
来源：http://www.ydjk.org.cn/Article/details/gt3nmbnqmyu.html

a?.b?.c
来源：http://www.ydjk.org.cn/Article/details/gt3lbfzskpa.html

[U86] JS：空值合并
来源：http://www.52xcode.cn/Article/details/gt3adeuwokm.html

a ?? b
来源：http://www.ydjk.org.cn/Article/details/gt3wlmvzbpp.html

[U87] JS：解构默认值
来源：http://www.52xcode.cn/Article/details/gt3dwxgpwop.html

const { a = 1, b = 2 } = obj;
来源：http://www.52xcode.cn/Article/details/gt3jtaiafoo.html

[U88] JS：对象展开合并
来源：http://www.52xcode.cn/Article/details/gt3hrdcngjm.html

{ ...a, ...b }
来源：http://www.ydjk.org.cn/Article/details/gt3zqpkknit.html

[U89] JS：数组去重
来源：http://www.52xcode.cn/Article/details/gt3xsynhoyo.html

[...new Set(arr)]
来源：http://www.ydjk.org.cn/Article/details/gt3qfsgcmsz.html

[U90] JS：数字数组排序
来源：http://www.52xcode.cn/Article/details/gt3vwkrcwcs.html

[...arr].sort((a, b) => a - b)
来源：http://www.52xcode.cn/Article/details/gt3rxreegvu.html

[U91] JS：对象键值遍历
来源：http://www.52xcode.cn/Article/details/gt3djbegtvc.html

Object.entries(obj).forEach(([k, v]) => {});
来源：http://www.52xcode.cn/Article/details/gt3nmyjkkpc.html

[U92] JS：深拷贝
来源：http://www.52xcode.cn/Article/details/gt3flidxwdh.html

structuredClone(obj)
来源：http://www.52xcode.cn/Article/details/gt3pimajkxw.html

[U93] JS：模板字符串
来源：http://www.ydjk.org.cn/Article/details/gt3ueocxvis.html

`共 ${n} 条`
来源：http://www.52xcode.cn/Article/details/gt3jfjytmvi.html

[U94] JS：箭头函数
来源：http://www.52xcode.cn/Article/details/gt3ezrjoaol.html

const double = x => x * 2;
来源：http://www.ydjk.org.cn/Article/details/gt3dkgcyuig.html

[U95] JS：Promise 包装
来源：http://www.ydjk.org.cn/Article/details/gt3lqqkmhgx.html

new Promise((resolve, reject) => {})
来源：http://www.ydjk.org.cn/Article/details/gt3clnzixvr.html

[U96] JS：async/await 与异常
来源：http://www.ydjk.org.cn/Article/details/gt3qimpdrlv.html

try { const d = await f(); } catch (e) { console.error(e); }
来源：http://www.ydjk.org.cn/Article/details/gt3ktoaxdeq.html

[U97] JS：并发请求
来源：http://www.52xcode.cn/Article/details/gt3aygjjcdf.html

await Promise.all(urls.map(u => fetch(u)))
来源：http://www.52xcode.cn/Article/details/gt3yvfejgwc.html

[U98] JS：fetch 带 JSON
来源：http://www.ydjk.org.cn/Article/details/gt3euhmqwvk.html

await fetch(url, { method: "POST", headers: { "Content-Type": "application/json" }, body: JSON.stringify(d) })
来源：http://www.ydjk.org.cn/Article/details/gt3axrplayo.html

[U99] JS：事件监听
来源：http://www.52xcode.cn/Article/details/gt3inihesax.html

el.addEventListener("click", e => {})
来源：http://www.ydjk.org.cn/Article/details/gt3ptgimcqp.html

[U100] JS：DOM 查询
来源：http://www.52xcode.cn/Article/details/gt3jrxxbpxq.html

document.querySelector(".item")
来源：http://www.52xcode.cn/Article/details/gt3ptqvcmew.html

[U101] JS：classList 操作
来源：http://www.52xcode.cn/Article/details/gt3dvimwfpo.html

el.classList.toggle("active")
来源：http://www.52xcode.cn/Article/details/gt3cwugnvwt.html

[U102] JS：本地存储
来源：http://www.ydjk.org.cn/Article/details/gt3obzesgmd.html

localStorage.setItem("k", JSON.stringify(v))
来源：http://www.ydjk.org.cn/Article/details/gt3fzhsprqv.html

[U103] JS：定时器
来源：http://www.52xcode.cn/Article/details/gt3hvlkhles.html

setTimeout(fn, 1000);  setInterval(fn, 1000);
来源：http://www.52xcode.cn/Article/details/gt3ajhwpapc.html

[U104] JS：防抖
来源：http://www.52xcode.cn/Article/details/gt3oinuxvon.html

const debounce = (fn, ms) => { let t; return (...a) => { clearTimeout(t); t = setTimeout(() => fn(...a), ms); }; };
来源：http://www.52xcode.cn/Article/details/gt3eviwkgyw.html

[U105] JS：节流
来源：http://www.ydjk.org.cn/Article/details/gt3qgvzjbmd.html

const throttle = (fn, ms) => { let last = 0; return (...a) => { const n = Date.now(); if (n - last >= ms) { last = n; fn(...a); } }; };
来源：http://www.ydjk.org.cn/Article/details/gt3mwgbdlhx.html

[U106] JS：日期格式化
来源：http://www.52xcode.cn/Article/details/gt3uqtxbneh.html

new Intl.DateTimeFormat("zh-CN", { dateStyle: "medium" }).format(new Date())
来源：http://www.ydjk.org.cn/Article/details/gt3lvcegtiv.html

[U107] JS：数字千分位
来源：http://www.52xcode.cn/Article/details/gt3jvntsicy.html

new Intl.NumberFormat("en-US").format(1234567)
来源：http://www.ydjk.org.cn/Article/details/gt3onmhgnpg.html

[U108] JS：随机整数
来源：http://www.ydjk.org.cn/Article/details/gt3wukywpav.html

Math.floor(Math.random() * (max - min + 1)) + min
来源：http://www.ydjk.org.cn/Article/details/gt3zwtrahts.html

[U109] JS：数组分组
来源：http://www.52xcode.cn/Article/details/gt3svuznxxt.html

Object.groupBy(arr, x => x.type)
来源：http://www.ydjk.org.cn/Article/details/gt3xmrpehbo.html

[U110] JS：数组分块
来源：http://www.52xcode.cn/Article/details/gt3iahotzly.html

arr.reduce((acc, x, i) => (i % size ? acc : [...acc, arr.slice(i, i + size)]), [])
来源：http://www.ydjk.org.cn/Article/details/gt3trfkdkjw.html

[U111] JS：对象转 Map
来源：http://www.ydjk.org.cn/Article/details/gt3kzgwqugj.html

new Map(Object.entries(obj))
来源：http://www.52xcode.cn/Article/details/gt3doisvfix.html

[U112] JS：字符串补位
来源：http://www.52xcode.cn/Article/details/gt3kthgpvpp.html

"7".padStart(3, "0")
来源：http://www.ydjk.org.cn/Article/details/gt3neamabxu.html

[U113] JS：正则替换全部
来源：http://www.ydjk.org.cn/Article/details/gt3wotxwwoa.html

s.replaceAll("a", "b")
来源：http://www.52xcode.cn/Article/details/gt3kgrkpuie.html

[U114] JS：JSON 深比较
来源：http://www.52xcode.cn/Article/details/gt3pvrlbmqg.html

JSON.stringify(a) === JSON.stringify(b)
来源：http://www.ydjk.org.cn/Article/details/gt3vzsmkwuw.html

[U115] JS：生成 UUID
来源：http://www.52xcode.cn/Article/details/gt3rovfetjb.html

crypto.randomUUID()
来源：http://www.ydjk.org.cn/Article/details/gt3cbjpmehn.html

[U116] JS：类型检查（JSDoc）
来源：http://www.52xcode.cn/Article/details/gt3exptmuev.html

/** @param {string} name */ function f(name) {}
来源：http://www.52xcode.cn/Article/details/gt3nbppkpng.html

[U117] JS：单元测试
来源：http://www.52xcode.cn/Article/details/gt3iigojvju.html

npm i -D vitest;  npx vitest
来源：http://www.52xcode.cn/Article/details/gt3lsjxkunr.html

[U118] JS：开发服务器
来源：http://www.52xcode.cn/Article/details/gt3gythotxx.html

npm i -D vite;  npx vite
来源：http://www.52xcode.cn/Article/details/gt3gkefkidi.html

[U119] JS：生产构建
来源：http://www.52xcode.cn/Article/details/gt3nahqiqlt.html

npx vite build
来源：http://www.ydjk.org.cn/Article/details/gt3bzvmymux.html

[U120] JS：读取环境变量（Vite）
来源：http://www.ydjk.org.cn/Article/details/gt3cmhooefn.html

import.meta.env.VITE_API_URL
来源：http://www.ydjk.org.cn/Article/details/gt3wujyioez.html

================================================================================
来源：http://www.52xcode.cn/Article/details/gt3yvshsslh.html

统计汇总
来源：http://www.ydjk.org.cn/Article/details/gt3rmkojlct.html

================================================================================
来源：http://www.ydjk.org.cn/Article/details/gt3ptjobojh.html

按语言统计（条）：
来源：http://www.52xcode.cn/Article/details/gt3cfnmpycg.html

Python ......... 252
来源：http://www.ydjk.org.cn/Article/details/gt3oewqeoin.html

PHP ............ 252
来源：http://www.52xcode.cn/Article/details/gt3fkjqyilk.html

JavaScript ..... 252
来源：http://www.ydjk.org.cn/Article/details/gt3pefyahli.html

TypeScript ..... 212
来源：http://www.52xcode.cn/Article/details/gt3opnnaark.html

Java ........... 212
来源：http://www.52xcode.cn/Article/details/gt3fsffjefp.html

Go ............. 212
来源：http://www.ydjk.org.cn/Article/details/gt3gwbvyavg.html

Ruby ........... 212
来源：http://www.ydjk.org.cn/Article/details/gt3fvbmycjn.html

C# ............. 212
来源：http://www.52xcode.cn/Article/details/gt3zzxxinan.html

C .............. 30
来源：http://www.ydjk.org.cn/Article/details/gt3wcorotte.html

C++ ............ 30
来源：http://www.52xcode.cn/Article/details/gt3nkrgwase.html

SQL ............ 90
来源：http://www.ydjk.org.cn/Article/details/gt3fdrghrjy.html

Bash ........... 80
来源：http://www.ydjk.org.cn/Article/details/gt3kkmawezc.html

Kotlin ......... 15
来源：http://www.52xcode.cn/Article/details/gt3aztohofm.html

Swift .......... 15
来源：http://www.ydjk.org.cn/Article/details/gt3sqidmzuh.html

Lua ............ 10
来源：http://www.ydjk.org.cn/Article/details/gt3nxnqaozg.html

Perl ........... 10
来源：http://www.52xcode.cn/Article/details/gt3pczuncsu.html

Scala .......... 10
来源：http://www.ydjk.org.cn/Article/details/gt3ybuzkyhk.html

------------------------------------
来源：http://www.ydjk.org.cn/Article/details/gt3vttggnyl.html

合计 ........... 2106 条
来源：http://www.52xcode.cn/Article/details/gt3ikelfohb.html

按章节统计：
来源：http://www.ydjk.org.cn/Article/details/gt3obeebpns.html

A 基础语法与类型       26 个任务 × 8 语言 =  208
来源：http://www.52xcode.cn/Article/details/gt3todbvisa.html

B 流程控制             16 个任务 × 8 语言 =  128
来源：http://www.52xcode.cn/Article/details/gt3wwdwtdhc.html

C 函数与作用域         16 个任务 × 8 语言 =  128
来源：http://www.52xcode.cn/Article/details/gt3tmfrpczs.html

D 数组 / 列表 / 集合   26 个任务 × 8 语言 =  208
来源：http://www.ydjk.org.cn/Article/details/gt3agokrxjs.html

E 字符串处理           22 个任务 × 8 语言 =  176
来源：http://www.52xcode.cn/Article/details/gt3imurlnqy.html

F 文件与目录           12 个任务 × 8 语言 =   96
来源：http://www.52xcode.cn/Article/details/gt3fxwoavht.html

G 面向对象             16 个任务 × 8 语言 =  128
来源：http://www.52xcode.cn/Article/details/gt3zcqcgynd.html

H 异常与错误处理       10 个任务 × 8 语言 =   80
来源：http://www.ydjk.org.cn/Article/details/gt3dhbfyqyz.html

I 正则表达式            8 个任务 × 8 语言 =   64
来源：http://www.ydjk.org.cn/Article/details/gt3wwjwfmdf.html

J 日期与时间           10 个任务 × 8 语言 =   80
来源：http://www.ydjk.org.cn/Article/details/gt3ijdfeclo.html

K JSON 与序列化         8 个任务 × 8 语言 =   64
来源：http://www.ydjk.org.cn/Article/details/gt3uvuknarj.html

L 网络请求              8 个任务 × 8 语言 =   64
来源：http://www.ydjk.org.cn/Article/details/gt3zawfidar.html

M 命令行 / 进程         8 个任务 × 8 语言 =   64
来源：http://www.52xcode.cn/Article/details/gt3odqmqcbv.html

N 数据结构与算法       12 个任务 × 8 语言 =   96
来源：http://www.52xcode.cn/Article/details/gt3bhjbmurw.html

O 并发与异步            6 个任务 × 8 语言 =   48
来源：http://www.52xcode.cn/Article/details/gt3jghupmyu.html

P 常用工具函数          8 个任务 × 8 语言 =   64
来源：http://www.ydjk.org.cn/Article/details/gt3zqnywwau.html

Q SQL 专题                              90
来源：http://www.52xcode.cn/Article/details/gt3dtkydksl.html

R Bash 专题                             80
来源：http://www.52xcode.cn/Article/details/gt3auxntewg.html

S C / C++ 专题                          60
来源：http://www.52xcode.cn/Article/details/gt3rtlbpqxp.html

T 其他语言补充                          60
来源：http://www.52xcode.cn/Article/details/gt3vlyciofa.html

U 高频实用片段                         120
来源：http://www.ydjk.org.cn/Article/details/gt3dedbznjh.html

------------------------------------
来源：http://www.ydjk.org.cn/Article/details/gt3vflzobmw.html

合计                                  2106 条
来源：http://www.52xcode.cn/Article/details/gt3uxbjcdvu.html

--------------------------------------------------------------------------------
来源：http://www.ydjk.org.cn/Article/details/gt3jjeuxuor.html

使用提醒
来源：http://www.ydjk.org.cn/Article/details/gt3lmrwprjj.html

--------------------------------------------------------------------------------
来源：http://www.52xcode.cn/Article/details/gt3qunjehsj.html

1. 示例追求"最小可用"，正式项目中请补齐导入、错误处理与边界判断。
来源：http://www.52xcode.cn/Article/details/gt3bgyvjvrr.html

2. 涉及文件、网络、数据库的示例，注意资源释放与异常捕获。
来源：http://www.ydjk.org.cn/Article/details/gt3cvhpstha.html

3. 语言版本差异较大（如 Python 3.10 的 match、Java 17 的 record/switch 箭头），
来源：http://www.52xcode.cn/Article/details/gt3uurtntwv.html

在旧版本上使用前请先确认语法支持情况。
来源：http://www.52xcode.cn/Article/details/gt3uvzcogvs.html

4. 标注"手写"的条目是因为该语言缺少对应内置能力，实际项目中可引入成熟库。
来源：http://www.52xcode.cn/Article/details/gt3mytilwtt.html

—— 文件结束 ——
来源：http://www.52xcode.cn/Article/details/gt3bezfwxme.html

================================================================================
来源：http://www.ydjk.org.cn/Article/details/gt3ybprwwdn.html

程序语言常见例子速查手册（2024 版）
来源：http://www.52xcode.cn/Article/details/gt3dxebcmhh.html

Common Programming Examples Cheat Book
来源：http://www.52xcode.cn/Article/details/gt3gxwhtshw.html

================================================================================
来源：http://www.ydjk.org.cn/Article/details/gt3mdyvsqcn.html

【收录内容】
来源：http://www.52xcode.cn/Article/details/gt3wckpewep.html

覆盖 12 种语言 / 语法与常见 API：
来源：http://www.ydjk.org.cn/Article/details/gt3sayicubw.html

Python · PHP · JavaScript · TypeScript · Java · Go · Ruby · C#
来源：http://www.52xcode.cn/Article/details/gt3mreszsxw.html

SQL · Bash · C · C++
来源：http://www.ydjk.org.cn/Article/details/gt3fxyhumfa.html

按「任务」分组：每个任务下按语言各给出一条最小可用示例。
来源：http://www.52xcode.cn/Article/details/gt3esxsvucv.html

【使用说明】
来源：http://www.ydjk.org.cn/Article/details/gt3glkbklrl.html

1. 每个任务形如 "[编号] 任务名"，下面每行以语言标记开头：
来源：http://www.52xcode.cn/Article/details/gt3chwgwztt.html

Py:    Python        PHP:   PHP           JS:    JavaScript
来源：http://www.ydjk.org.cn/Article/details/gt3wdidkgmh.html

TS:    TypeScript    Java:  Java          Go:    Go
来源：http://www.52xcode.cn/Article/details/gt3pcdjrzft.html

Ruby:  Ruby          C#:    C#            SQL:   SQL
来源：http://www.52xcode.cn/Article/details/gt3pkcxtqio.html

Bash:  Shell         C:     C             C++:   C++
来源：http://www.ydjk.org.cn/Article/details/gt3qwneykdc.html

2. 示例只展示核心写法，刻意省略 import / require / include / using 等样板代码。
来源：http://www.ydjk.org.cn/Article/details/gt3vkttbmui.html

需要完整可运行文件时，请自行补齐当前语言的导入语句。
来源：http://www.52xcode.cn/Article/details/gt3zuttqoxx.html

3. 语法基准：Python 3.10+ / PHP 8.1+ / ES2020+ / TypeScript 5 / Java 17 /
来源：http://www.ydjk.org.cn/Article/details/gt3flnfxpzf.html

Go 1.21+ / Ruby 3.x / C# 10+ / C17 / C++17。
来源：http://www.52xcode.cn/Article/details/gt3kcxbqugg.html

4. 检索建议：用编辑器或浏览器 Ctrl+F 搜关键词，如 "排序" "读取文件" "正则"。
来源：http://www.ydjk.org.cn/Article/details/gt3sqdzjmdy.html

5. 标记为 "// 无" 表示该语言没有对应的一等语法，需用替代写法（示例给出替代方案）。
来源：http://www.52xcode.cn/Article/details/gt3mofodcws.html

6. 符号 "⏎" 表示代码在此处换行（主要用于 Python 等强制缩进、无法压成一行的结构）。
来源：http://www.52xcode.cn/Article/details/gt3zrtjcmvt.html

【文件统计】
来源：http://www.ydjk.org.cn/Article/details/gt3xnbvogsl.html

语言示例共 2106 条，分布见本文末尾的「统计汇总」。
来源：http://www.52xcode.cn/Article/details/gt3mhworrwn.html

--------------------------------------------------------------------------------
来源：http://www.ydjk.org.cn/Article/details/gt3cjgvdgec.html

目  录
来源：http://www.52xcode.cn/Article/details/gt3zdrewzmf.html

--------------------------------------------------------------------------------
来源：http://www.ydjk.org.cn/Article/details/gt3eqblrmki.html

A. 基础语法与类型              （第 1 节，26 个任务，208 条）
来源：http://www.52xcode.cn/Article/details/gt3djkuxlso.html

B. 流程控制                    （第 2 节，16 个任务，128 条）
来源：http://www.ydjk.org.cn/Article/details/gt3hsvnmxme.html

C. 函数与作用域                （第 3 节，16 个任务，128 条）
来源：http://www.52xcode.cn/Article/details/gt3zcucdyhe.html

D. 数组 / 列表 / 集合          （第 4 节，26 个任务，208 条）
来源：http://www.52xcode.cn/Article/details/gt3xbapiuax.html

E. 字符串处理                  （第 5 节，22 个任务，176 条）
来源：http://www.52xcode.cn/Article/details/gt3wdtcclhy.html

F. 文件与目录                  （第 6 节，12 个任务，96 条）
来源：http://www.52xcode.cn/Article/details/gt3funqwkmi.html

G. 面向对象                    （第 7 节，16 个任务，128 条）
来源：http://www.ydjk.org.cn/Article/details/gt3pxrvhwie.html

H. 异常与错误处理              （第 8 节，10 个任务，80 条）
来源：http://www.52xcode.cn/Article/details/gt3mdcbzbfk.html

I. 正则表达式                  （第 9 节，8 个任务，64 条）
来源：http://www.ydjk.org.cn/Article/details/gt3olgxjdhs.html

J. 日期与时间                  （第 10 节，10 个任务，80 条）
来源：http://www.52xcode.cn/Article/details/gt3omrzxxqp.html

K. JSON 与序列化               （第 11 节，8 个任务，64 条）
来源：http://www.52xcode.cn/Article/details/gt3wyksjjom.html

L. 网络请求                    （第 12 节，8 个任务，64 条）
来源：http://www.ydjk.org.cn/Article/details/gt3grscddux.html

M. 命令行 / 进程 / 环境        （第 13 节，8 个任务，64 条）
来源：http://www.ydjk.org.cn/Article/details/gt3rqposvoe.html

N. 数据结构与算法              （第 14 节，12 个任务，96 条）
来源：http://www.52xcode.cn/Article/details/gt3uhrveahl.html

O. 并发与异步                  （第 15 节，6 个任务，48 条）
来源：http://www.ydjk.org.cn/Article/details/gt3xdsmzkcp.html

P. 常用工具函数                （第 16 节，8 个任务，64 条）
来源：http://www.52xcode.cn/Article/details/gt3fbtscnja.html

Q. SQL 专题                    （第 17 节，90 条）
来源：http://www.ydjk.org.cn/Article/details/gt3awttdezs.html

R. Bash 专题                   （第 18 节，80 条）
来源：http://www.52xcode.cn/Article/details/gt3imqxfhah.html

S. C / C++ 专题                （第 19 节，60 条）
来源：http://www.52xcode.cn/Article/details/gt3wneoaqpq.html

T. 其他语言补充                （第 20 节，60 条：Kotlin / Swift / Lua / Perl / Scala）
来源：http://www.52xcode.cn/Article/details/gt3ickjbbxz.html

U. 高频实用片段                （第 21 节，120 条：Python / PHP / JavaScript 各 40 条）
来源：http://www.ydjk.org.cn/Article/details/gt3jmqqtrrm.html


<!-- 参考信息 -->