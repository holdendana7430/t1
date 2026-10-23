代发 wailian999

[U21] Py：自定义上下文管理器
来源：http://www.52xcode.cn/Article/details/gt3mlrxyzlf.html

@contextlib.contextmanager
来源：http://www.ydjk.org.cn/Article/details/gt3dmgnucsd.html

[U22] Py：矩阵转置
来源：http://www.ydjk.org.cn/Article/details/gt3rpvfdzfb.html

list(zip(*m))
来源：http://www.52xcode.cn/Article/details/gt3yagcgtga.html

[U23] Py：分块读取大文件
来源：http://www.ydjk.org.cn/Article/details/gt3dpzlmdos.html

for chunk in iter(lambda: f.read(8192), b""):
来源：http://www.52xcode.cn/Article/details/gt3cvuqotlk.html

[U24] Py：路径操作
来源：http://www.52xcode.cn/Article/details/gt3txprhrod.html

Path("a/b.txt").parent.mkdir(parents=True, exist_ok=True)
来源：http://www.ydjk.org.cn/Article/details/gt3lyjjjpam.html

[U25] Py：CSV 按字典读
来源：http://www.ydjk.org.cn/Article/details/gt3kxaeogtt.html

csv.DictReader(f)
来源：http://www.52xcode.cn/Article/details/gt3zymzqerc.html

[U26] Py：并发下载
来源：http://www.ydjk.org.cn/Article/details/gt3kfuudcbj.html

ThreadPoolExecutor(max_workers=8).map(fetch, urls)
来源：http://www.52xcode.cn/Article/details/gt3izvoljmk.html

[U27] Py：异步 HTTP
来源：http://www.ydjk.org.cn/Article/details/gt3uzakvyjs.html

aiohttp.ClientSession() 配合 async with
来源：http://www.52xcode.cn/Article/details/gt3ybtltxnu.html

[U28] Py：类型别名
来源：http://www.52xcode.cn/Article/details/gt3ybxwfauf.html

UserId = int
来源：http://www.ydjk.org.cn/Article/details/gt3ckkwvbti.html

[U29] Py：属性校验
来源：http://www.52xcode.cn/Article/details/gt3vbeynmex.html

@property 与 @x.setter 配合
来源：http://www.52xcode.cn/Article/details/gt3cnamvrik.html

[U30] Py：数据类
来源：http://www.ydjk.org.cn/Article/details/gt3izwttwiq.html

@dataclass(slots=True)
来源：http://www.ydjk.org.cn/Article/details/gt3qteiegwx.html

[U31] Py：单测
来源：http://www.52xcode.cn/Article/details/gt3fmkwcobx.html

python -m pytest -q
来源：http://www.52xcode.cn/Article/details/gt3gacupzba.html

[U32] Py：代码格式化
来源：http://www.ydjk.org.cn/Article/details/gt3pjveimtw.html

ruff format . && ruff check --fix .
来源：http://www.ydjk.org.cn/Article/details/gt3jesfmsxq.html

[U33] Py：打包发布
来源：http://www.ydjk.org.cn/Article/details/gt3pyherlzs.html

python -m build  （依赖 pyproject.toml）
来源：http://www.52xcode.cn/Article/details/gt3kkydkocu.html

[U34] Py：判断编码
来源：http://www.52xcode.cn/Article/details/gt3ygdqullj.html

chardet.detect(raw)
来源：http://www.ydjk.org.cn/Article/details/gt3vqvxcnks.html

[U35] Py：发送邮件
来源：http://www.52xcode.cn/Article/details/gt3sxwyjony.html

smtplib.SMTP_SSL(...).send_message(msg)
来源：http://www.ydjk.org.cn/Article/details/gt3kgtkwsoi.html

[U36] Py：定时任务
来源：http://www.52xcode.cn/Article/details/gt3wgqoipdf.html

schedule.every(10).minutes.do(job)
来源：http://www.52xcode.cn/Article/details/gt3vvyajzzh.html

[U37] Py：读写 Excel
来源：http://www.52xcode.cn/Article/details/gt3qyxjawfh.html

pandas.read_excel / DataFrame.to_excel
来源：http://www.ydjk.org.cn/Article/details/gt3hrybngdp.html

[U38] Py：获取脚本所在目录
来源：http://www.52xcode.cn/Article/details/gt3gnjvswwj.html

Path(__file__).resolve().parent
来源：http://www.ydjk.org.cn/Article/details/gt3fshprkkh.html

[U39] Py：判断是否在交互环境
来源：http://www.ydjk.org.cn/Article/details/gt3ltypwobb.html

sys.stdout.isatty()
来源：http://www.52xcode.cn/Article/details/gt3meqgvlez.html

[U40] Py：打印到标准错误
来源：http://www.ydjk.org.cn/Article/details/gt3pfnkmgvl.html

print("err", file=sys.stderr)
来源：http://www.ydjk.org.cn/Article/details/gt3tuxarzuk.html

[U41] PHP：初始化 Composer 项目
来源：http://www.ydjk.org.cn/Article/details/gt3almgzxiv.html

composer init;  composer require guzzlehttp/guzzle
来源：http://www.52xcode.cn/Article/details/gt3bfcneskd.html

[U42] PHP：PSR-4 自动加载
来源：http://www.ydjk.org.cn/Article/details/gt3uuvhvbng.html

"autoload": { "psr-4": { "App\\": "src/" } }
来源：http://www.ydjk.org.cn/Article/details/gt3yyszovkd.html

[U43] PHP：声明命名空间
来源：http://www.ydjk.org.cn/Article/details/gt3esngcfum.html

namespace App\Http;
来源：http://www.ydjk.org.cn/Article/details/gt3gvvxbwlp.html

[U44] PHP：开启严格类型
来源：http://www.ydjk.org.cn/Article/details/gt3kqmngkqw.html

declare(strict_types=1);
来源：http://www.52xcode.cn/Article/details/gt3jddmltwi.html

[U45] PHP：类型声明与返回类型
来源：http://www.ydjk.org.cn/Article/details/gt3styegcqu.html

function add(int $a, int $b): int { return $a + $b; }
来源：http://www.52xcode.cn/Article/details/gt3otdknxls.html

[U46] PHP：可空类型
来源：http://www.ydjk.org.cn/Article/details/gt3cvmsqswe.html

?string $name = null
来源：http://www.ydjk.org.cn/Article/details/gt3lngmkpjf.html

[U47] PHP：联合类型
来源：http://www.52xcode.cn/Article/details/gt3zbbfddvr.html

int|string $id
来源：http://www.52xcode.cn/Article/details/gt3vaaemhpo.html

[U48] PHP：纯枚举
来源：http://www.52xcode.cn/Article/details/gt3pleczdea.html

enum Status: string { case Active = "active"; case Off = "off"; }
来源：http://www.ydjk.org.cn/Article/details/gt3asanwybg.html

[U49] PHP：只读属性
来源：http://www.52xcode.cn/Article/details/gt3emgsleqk.html

public readonly string $name
来源：http://www.ydjk.org.cn/Article/details/gt3fzseqzjz.html

[U50] PHP：构造器属性提升
来源：http://www.52xcode.cn/Article/details/gt3oxaollla.html

public function __construct(private int $id) {}
来源：http://www.ydjk.org.cn/Article/details/gt3msxywuhi.html

[U51] PHP：数组解构
来源：http://www.ydjk.org.cn/Article/details/gt3bsqdtovx.html

[$a, $b] = $arr;
来源：http://www.ydjk.org.cn/Article/details/gt3cgccwvwn.html

[U52] PHP：箭头函数
来源：http://www.52xcode.cn/Article/details/gt3arqstpsg.html

$double = fn($x) => $x * 2;
来源：http://www.52xcode.cn/Article/details/gt3stbobdmq.html

[U53] PHP：空合并运算符
来源：http://www.52xcode.cn/Article/details/gt3lhwyrttj.html

$v = $a ?? $b ?? "default";
来源：http://www.52xcode.cn/Article/details/gt3lxjvrdks.html

[U54] PHP：空安全调用
来源：http://www.ydjk.org.cn/Article/details/gt3nqnlfpqk.html

$obj?->method()
来源：http://www.52xcode.cn/Article/details/gt3soxwhrek.html

[U55] PHP：match 表达式
来源：http://www.52xcode.cn/Article/details/gt3jubqpufi.html

$s = match($x) { 1 => "一", default => "其他" };
来源：http://www.ydjk.org.cn/Article/details/gt3rsubcxwp.html

[U56] PHP：命名参数
来源：http://www.52xcode.cn/Article/details/gt3nagixxcm.html

f(a: 1, b: 2)
来源：http://www.ydjk.org.cn/Article/details/gt3hkekaefb.html

[U57] PHP：字符串插值
来源：http://www.ydjk.org.cn/Article/details/gt3nzadpeiz.html

"值: {$a}"
来源：http://www.52xcode.cn/Article/details/gt3ijlugnaw.html

[U58] PHP：数组三件套
来源：http://www.ydjk.org.cn/Article/details/gt3bxthftjq.html

array_map($f, $a);  array_filter($a, $f);  array_reduce($a, $f, 0);
来源：http://www.52xcode.cn/Article/details/gt3rblutaqh.html

[U59] PHP：自定义排序
来源：http://www.ydjk.org.cn/Article/details/gt3ldfnsucx.html

usort($arr, fn($a, $b) => $a["age"] <=> $b["age"]);
来源：http://www.ydjk.org.cn/Article/details/gt3qcvtditl.html

[U60] PHP：JSON 编解码
来源：http://www.52xcode.cn/Article/details/gt3jlzrmpxi.html

json_encode($d, JSON_UNESCAPED_UNICODE);  json_decode($s, true);
来源：http://www.ydjk.org.cn/Article/details/gt3psknllne.html

[U61] PHP：正则
来源：http://www.ydjk.org.cn/Article/details/gt3azoqaggn.html

preg_match('/(\d+)/', $s, $m);  preg_replace('/\d+/', '#', $s);
来源：http://www.52xcode.cn/Article/details/gt3suiwhrru.html

[U62] PHP：日期对象
来源：http://www.ydjk.org.cn/Article/details/gt3pttszyes.html

(new DateTimeImmutable())->format("Y-m-d");
来源：http://www.ydjk.org.cn/Article/details/gt3jeoqppen.html

[U63] PHP：文件读写
来源：http://www.ydjk.org.cn/Article/details/gt3hsokzjmh.html

file_get_contents($f);  file_put_contents($f, $data);
来源：http://www.52xcode.cn/Article/details/gt3rjlsnjdz.html

[U64] PHP：目录遍历
来源：http://www.52xcode.cn/Article/details/gt3gltfyxoa.html

glob("dir/*.php");  scandir("dir");
来源：http://www.ydjk.org.cn/Article/details/gt3fuhurrej.html

[U65] PHP：会话
来源：http://www.52xcode.cn/Article/details/gt3lvrmhzoi.html

session_start();  $_SESSION["uid"] = 1;
来源：http://www.52xcode.cn/Article/details/gt3vjvlsage.html

[U66] PHP：设置 Cookie
来源：http://www.ydjk.org.cn/Article/details/gt3cxwstvyn.html

setcookie("token", $v, ["httponly" => true, "samesite" => "Lax"]);
来源：http://www.ydjk.org.cn/Article/details/gt3vazuvopl.html

[U67] PHP：处理文件上传
来源：http://www.ydjk.org.cn/Article/details/gt3pgjiptfj.html

$_FILES["file"]["tmp_name"] 与 move_uploaded_file()
来源：http://www.ydjk.org.cn/Article/details/gt3vzcurtft.html

[U68] PHP：PDO 连接
来源：http://www.52xcode.cn/Article/details/gt3cajfqrda.html

$pdo = new PDO("mysql:host=localhost;dbname=app", "root", "");
来源：http://www.ydjk.org.cn/Article/details/gt3ldubincs.html

[U69] PHP：PDO 预处理
来源：http://www.52xcode.cn/Article/details/gt3yfaizrag.html

$stmt = $pdo->prepare("SELECT * FROM users WHERE id = ?");  $stmt->execute([$id]);
来源：http://www.ydjk.org.cn/Article/details/gt3ndvgcvtw.html

[U70] PHP：PDO 事务
来源：http://www.ydjk.org.cn/Article/details/gt3oksqykjq.html

$pdo->beginTransaction();  $pdo->commit();  $pdo->rollBack();
来源：http://www.52xcode.cn/Article/details/gt3ywhtuolp.html

[U71] PHP：抛出异常
来源：http://www.52xcode.cn/Article/details/gt3lpvtkmth.html

throw new RuntimeException("失败", 500);
来源：http://www.52xcode.cn/Article/details/gt3qdxxaprr.html

[U72] PHP：写错误日志
来源：http://www.52xcode.cn/Article/details/gt3sygkvotk.html

error_log("失败: " . $e->getMessage());
来源：http://www.52xcode.cn/Article/details/gt3mvhbxvoi.html

[U73] PHP：读取 ini 配置
来源：http://www.ydjk.org.cn/Article/details/gt3zjxkrylv.html

parse_ini_file("config.ini", true)
来源：http://www.52xcode.cn/Article/details/gt3rdsrxvnr.html

[U74] PHP：读取环境变量
来源：http://www.52xcode.cn/Article/details/gt3pvprizhu.html

getenv("APP_ENV") ?: "production"
来源：http://www.52xcode.cn/Article/details/gt3qtystxcf.html

[U75] PHP：依赖注入
来源：http://www.52xcode.cn/Article/details/gt3oxmvecfu.html

composer require psr/container
来源：http://www.ydjk.org.cn/Article/details/gt3blnnaciq.html

[U76] PHP：简单路由
来源：http://www.ydjk.org.cn/Article/details/gt3kioxwiyx.html

$path = parse_url($_SERVER["REQUEST_URI"], PHP_URL_PATH);
来源：http://www.ydjk.org.cn/Article/details/gt3sadmrhzo.html

[U77] PHP：模板渲染
来源：http://www.ydjk.org.cn/Article/details/gt3uldlqbyc.html

composer require twig/twig
来源：http://www.52xcode.cn/Article/details/gt3tbnezvzs.html

[U78] PHP：单元测试
来源：http://www.ydjk.org.cn/Article/details/gt3foluiiif.html

composer require --dev phpunit/phpunit
来源：http://www.ydjk.org.cn/Article/details/gt3vltccapa.html

[U79] PHP：静态分析
来源：http://www.52xcode.cn/Article/details/gt3ipdbdogc.html

composer require --dev phpstan/phpstan
来源：http://www.52xcode.cn/Article/details/gt3xthomycs.html

[U80] PHP：代码规范修复
来源：http://www.ydjk.org.cn/Article/details/gt3znfzoiwe.html

composer require --dev friendsofphp/php-cs-fixer
来源：http://www.52xcode.cn/Article/details/gt3woeuenmc.html

[U81] JS：初始化项目
来源：http://www.ydjk.org.cn/Article/details/gt3ulkasgvm.html

npm init -y;  npm i express
来源：http://www.ydjk.org.cn/Article/details/gt3aopskctf.html

[U82] JS：package.json 脚本
来源：http://www.52xcode.cn/Article/details/gt3ocpwjozz.html

"scripts": { "dev": "vite", "build": "vite build" }
来源：http://www.52xcode.cn/Article/details/gt3atupmqnm.html

[U83] JS：ES Module 导入导出
来源：http://www.52xcode.cn/Article/details/gt3hqibchua.html

export const a = 1;  import { a } from "./m.js";
来源：http://www.ydjk.org.cn/Article/details/gt3qjnmxnyo.html

[U84] JS：CommonJS 写法
来源：http://www.52xcode.cn/Article/details/gt3sehtxady.html

module.exports = { a };  const { a } = require("./m");
来源：http://www.52xcode.cn/Article/details/gt3manvduxn.html

[U85] JS：可选链
来源：http://www.ydjk.org.cn/Article/details/gt3oszmjmqu.html

a?.b?.c
来源：http://www.52xcode.cn/Article/details/gt3hzdffgfd.html

[U86] JS：空值合并
来源：http://www.ydjk.org.cn/Article/details/gt3ymnotboq.html

a ?? b
来源：http://www.52xcode.cn/Article/details/gt3ghxhgaqf.html

[U87] JS：解构默认值
来源：http://www.52xcode.cn/Article/details/gt3suaanyna.html

const { a = 1, b = 2 } = obj;
来源：http://www.52xcode.cn/Article/details/gt3vnhyafjt.html

[U88] JS：对象展开合并
来源：http://www.ydjk.org.cn/Article/details/gt3buxgzhoy.html

{ ...a, ...b }
来源：http://www.52xcode.cn/Article/details/gt3zwchrefi.html

[U89] JS：数组去重
来源：http://www.52xcode.cn/Article/details/gt3vjzcipom.html

[...new Set(arr)]
来源：http://www.ydjk.org.cn/Article/details/gt3yutubrsb.html

[U90] JS：数字数组排序
来源：http://www.52xcode.cn/Article/details/gt3zoikrjto.html

[...arr].sort((a, b) => a - b)
来源：http://www.52xcode.cn/Article/details/gt3sxwnwwdp.html

[U91] JS：对象键值遍历
来源：http://www.ydjk.org.cn/Article/details/gt3gumpgeip.html

Object.entries(obj).forEach(([k, v]) => {});
来源：http://www.52xcode.cn/Article/details/gt3pxachlui.html

[U92] JS：深拷贝
来源：http://www.ydjk.org.cn/Article/details/gt3pyvozvtj.html

structuredClone(obj)
来源：http://www.52xcode.cn/Article/details/gt3xszqvmjj.html

[U93] JS：模板字符串
来源：http://www.52xcode.cn/Article/details/gt3mcwiufnv.html

`共 ${n} 条`
来源：http://www.52xcode.cn/Article/details/gt3zguasibb.html

[U94] JS：箭头函数
来源：http://www.52xcode.cn/Article/details/gt3xauqwqqn.html

const double = x => x * 2;
来源：http://www.52xcode.cn/Article/details/gt3fkoahaxn.html

[U95] JS：Promise 包装
来源：http://www.ydjk.org.cn/Article/details/gt3etmrisyi.html

new Promise((resolve, reject) => {})
来源：http://www.52xcode.cn/Article/details/gt3lcfdfglx.html

[U96] JS：async/await 与异常
来源：http://www.ydjk.org.cn/Article/details/gt3zvojurtf.html

try { const d = await f(); } catch (e) { console.error(e); }
来源：http://www.52xcode.cn/Article/details/gt3hucjprbz.html

[U97] JS：并发请求
来源：http://www.52xcode.cn/Article/details/gt3negezknx.html

await Promise.all(urls.map(u => fetch(u)))
来源：http://www.ydjk.org.cn/Article/details/gt3whaxjgui.html

[U98] JS：fetch 带 JSON
来源：http://www.ydjk.org.cn/Article/details/gt3qqsjtzeh.html

await fetch(url, { method: "POST", headers: { "Content-Type": "application/json" }, body: JSON.stringify(d) })
来源：http://www.ydjk.org.cn/Article/details/gt3yanhlpre.html

[U99] JS：事件监听
来源：http://www.ydjk.org.cn/Article/details/gt3ixfddkwm.html

el.addEventListener("click", e => {})
来源：http://www.52xcode.cn/Article/details/gt3mdxawwvw.html

[U100] JS：DOM 查询
来源：http://www.ydjk.org.cn/Article/details/gt3nfjkdzpl.html

document.querySelector(".item")
来源：http://www.ydjk.org.cn/Article/details/gt3lnpuvfzr.html

[U101] JS：classList 操作
来源：http://www.52xcode.cn/Article/details/gt3jfewcexl.html

el.classList.toggle("active")
来源：http://www.ydjk.org.cn/Article/details/gt3uiwwleav.html

[U102] JS：本地存储
来源：http://www.52xcode.cn/Article/details/gt3xmgcpegd.html

localStorage.setItem("k", JSON.stringify(v))
来源：http://www.52xcode.cn/Article/details/gt3ckfnieku.html

[U103] JS：定时器
来源：http://www.ydjk.org.cn/Article/details/gt3zkiiranm.html

setTimeout(fn, 1000);  setInterval(fn, 1000);
来源：http://www.52xcode.cn/Article/details/gt3jdfuvmhs.html

[U104] JS：防抖
来源：http://www.52xcode.cn/Article/details/gt3paueakzx.html

const debounce = (fn, ms) => { let t; return (...a) => { clearTimeout(t); t = setTimeout(() => fn(...a), ms); }; };
来源：http://www.52xcode.cn/Article/details/gt3pjoatdbs.html

[U105] JS：节流
来源：http://www.ydjk.org.cn/Article/details/gt3agasxkqc.html

const throttle = (fn, ms) => { let last = 0; return (...a) => { const n = Date.now(); if (n - last >= ms) { last = n; fn(...a); } }; };
来源：http://www.ydjk.org.cn/Article/details/gt3cqojdclc.html

[U106] JS：日期格式化
来源：http://www.ydjk.org.cn/Article/details/gt3kqsdzrlx.html

new Intl.DateTimeFormat("zh-CN", { dateStyle: "medium" }).format(new Date())
来源：http://www.ydjk.org.cn/Article/details/gt3lsdlgufk.html

[U107] JS：数字千分位
来源：http://www.ydjk.org.cn/Article/details/gt3ppnpgvva.html

new Intl.NumberFormat("en-US").format(1234567)
来源：http://www.52xcode.cn/Article/details/gt3hykoikxw.html

[U108] JS：随机整数
来源：http://www.ydjk.org.cn/Article/details/gt3refduepl.html

Math.floor(Math.random() * (max - min + 1)) + min
来源：http://www.52xcode.cn/Article/details/gt3fvhlxgna.html

[U109] JS：数组分组
来源：http://www.ydjk.org.cn/Article/details/gt3zdtootog.html

Object.groupBy(arr, x => x.type)
来源：http://www.ydjk.org.cn/Article/details/gt3ecypuxdf.html

[U110] JS：数组分块
来源：http://www.52xcode.cn/Article/details/gt3preipfxc.html

arr.reduce((acc, x, i) => (i % size ? acc : [...acc, arr.slice(i, i + size)]), [])
来源：http://www.ydjk.org.cn/Article/details/gt3wivbtybk.html

[U111] JS：对象转 Map
来源：http://www.52xcode.cn/Article/details/gt3mbcdqzmc.html

new Map(Object.entries(obj))
来源：http://www.52xcode.cn/Article/details/gt3ozdqthcu.html

[U112] JS：字符串补位
来源：http://www.ydjk.org.cn/Article/details/gt3mnfvcljc.html

"7".padStart(3, "0")
来源：http://www.ydjk.org.cn/Article/details/gt3skuawkkd.html

[U113] JS：正则替换全部
来源：http://www.ydjk.org.cn/Article/details/gt3mdyofzmx.html

s.replaceAll("a", "b")
来源：http://www.ydjk.org.cn/Article/details/gt3xoqinwqb.html

[U114] JS：JSON 深比较
来源：http://www.ydjk.org.cn/Article/details/gt3nzwzwrid.html

JSON.stringify(a) === JSON.stringify(b)
来源：http://www.ydjk.org.cn/Article/details/gt3wgcjkkja.html

[U115] JS：生成 UUID
来源：http://www.52xcode.cn/Article/details/gt3gklzclvt.html

crypto.randomUUID()
来源：http://www.ydjk.org.cn/Article/details/gt3ivsftses.html

[U116] JS：类型检查（JSDoc）
来源：http://www.ydjk.org.cn/Article/details/gt3cbuzdpko.html

/** @param {string} name */ function f(name) {}
来源：http://www.52xcode.cn/Article/details/gt3wkcareer.html

[U117] JS：单元测试
来源：http://www.52xcode.cn/Article/details/gt3btmruqmv.html

npm i -D vitest;  npx vitest
来源：http://www.52xcode.cn/Article/details/gt3yzzzdwje.html

[U118] JS：开发服务器
来源：http://www.52xcode.cn/Article/details/gt3rnuauwjs.html

npm i -D vite;  npx vite
来源：http://www.ydjk.org.cn/Article/details/gt3blnxwrod.html

[U119] JS：生产构建
来源：http://www.52xcode.cn/Article/details/gt3dpzbsusw.html

npx vite build
来源：http://www.ydjk.org.cn/Article/details/gt3rwpwjzyf.html

[U120] JS：读取环境变量（Vite）
来源：http://www.52xcode.cn/Article/details/gt3xjnijgau.html

import.meta.env.VITE_API_URL
来源：http://www.ydjk.org.cn/Article/details/gt3wigxywmd.html

================================================================================
来源：http://www.ydjk.org.cn/Article/details/gt3bssvokpc.html

统计汇总
来源：http://www.52xcode.cn/Article/details/gt3tfkmgmkt.html

================================================================================
来源：http://www.ydjk.org.cn/Article/details/gt3bikbwqlj.html

按语言统计（条）：
来源：http://www.ydjk.org.cn/Article/details/gt3yvoigzcr.html

Python ......... 252
来源：http://www.ydjk.org.cn/Article/details/gt3kjqmvudb.html

PHP ............ 252
来源：http://www.52xcode.cn/Article/details/gt3gtvjidvu.html

JavaScript ..... 252
来源：http://www.52xcode.cn/Article/details/gt3fnihywvk.html

TypeScript ..... 212
来源：http://www.ydjk.org.cn/Article/details/gt3hxvmrqqb.html

Java ........... 212
来源：http://www.ydjk.org.cn/Article/details/gt3ptkisgov.html

Go ............. 212
来源：http://www.52xcode.cn/Article/details/gt3phpollot.html

Ruby ........... 212
来源：http://www.52xcode.cn/Article/details/gt3sqdloubn.html

C# ............. 212
来源：http://www.52xcode.cn/Article/details/gt3afclbqzg.html

C .............. 30
来源：http://www.ydjk.org.cn/Article/details/gt3lcigwkjt.html

C++ ............ 30
来源：http://www.ydjk.org.cn/Article/details/gt3bceoreqd.html

SQL ............ 90
来源：http://www.52xcode.cn/Article/details/gt3lhkyuueb.html

Bash ........... 80
来源：http://www.ydjk.org.cn/Article/details/gt3kjdifhez.html

Kotlin ......... 15
来源：http://www.ydjk.org.cn/Article/details/gt3cybesbem.html

Swift .......... 15
来源：http://www.52xcode.cn/Article/details/gt3dyddwlsa.html

Lua ............ 10
来源：http://www.52xcode.cn/Article/details/gt3dwxnmhqf.html

Perl ........... 10
来源：http://www.52xcode.cn/Article/details/gt3iestqnia.html

Scala .......... 10
来源：http://www.52xcode.cn/Article/details/gt3shggzhfx.html

------------------------------------
来源：http://www.ydjk.org.cn/Article/details/gt3swcfejow.html

合计 ........... 2106 条
来源：http://www.52xcode.cn/Article/details/gt3bfslyehj.html

按章节统计：
来源：http://www.52xcode.cn/Article/details/gt3jbwgtdtx.html

A 基础语法与类型       26 个任务 × 8 语言 =  208
来源：http://www.ydjk.org.cn/Article/details/gt3agncnjor.html

B 流程控制             16 个任务 × 8 语言 =  128
来源：http://www.52xcode.cn/Article/details/gt3srmejwuj.html

C 函数与作用域         16 个任务 × 8 语言 =  128
来源：http://www.ydjk.org.cn/Article/details/gt3epvyuurv.html

D 数组 / 列表 / 集合   26 个任务 × 8 语言 =  208
来源：http://www.ydjk.org.cn/Article/details/gt3cbcpmmqn.html

E 字符串处理           22 个任务 × 8 语言 =  176
来源：http://www.ydjk.org.cn/Article/details/gt3dwgntqfl.html

F 文件与目录           12 个任务 × 8 语言 =   96
来源：http://www.52xcode.cn/Article/details/gt3qoehugmz.html

G 面向对象             16 个任务 × 8 语言 =  128
来源：http://www.ydjk.org.cn/Article/details/gt3wpdadvsn.html

H 异常与错误处理       10 个任务 × 8 语言 =   80
来源：http://www.52xcode.cn/Article/details/gt3jmrtvjut.html

I 正则表达式            8 个任务 × 8 语言 =   64
来源：http://www.ydjk.org.cn/Article/details/gt3todlyhxv.html

J 日期与时间           10 个任务 × 8 语言 =   80
来源：http://www.ydjk.org.cn/Article/details/gt3mwsoiqtc.html

K JSON 与序列化         8 个任务 × 8 语言 =   64
来源：http://www.ydjk.org.cn/Article/details/gt3jipyeqgf.html

L 网络请求              8 个任务 × 8 语言 =   64
来源：http://www.52xcode.cn/Article/details/gt3mckayxdb.html

M 命令行 / 进程         8 个任务 × 8 语言 =   64
来源：http://www.52xcode.cn/Article/details/gt3aldvaqwn.html

N 数据结构与算法       12 个任务 × 8 语言 =   96
来源：http://www.52xcode.cn/Article/details/gt3ubyxhmzr.html

O 并发与异步            6 个任务 × 8 语言 =   48
来源：http://www.52xcode.cn/Article/details/gt3ipfbvdye.html

P 常用工具函数          8 个任务 × 8 语言 =   64
来源：http://www.ydjk.org.cn/Article/details/gt3rzrdsyil.html

Q SQL 专题                              90
来源：http://www.52xcode.cn/Article/details/gt3webhjnjs.html

R Bash 专题                             80
来源：http://www.ydjk.org.cn/Article/details/gt3frtlwsco.html

S C / C++ 专题                          60
来源：http://www.52xcode.cn/Article/details/gt3roiisoyu.html

T 其他语言补充                          60
来源：http://www.52xcode.cn/Article/details/gt3npaxjntc.html

U 高频实用片段                         120
来源：http://www.ydjk.org.cn/Article/details/gt3cperlbvq.html

------------------------------------
来源：http://www.52xcode.cn/Article/details/gt3equoiraq.html

合计                                  2106 条
来源：http://www.ydjk.org.cn/Article/details/gt3evogrlch.html

--------------------------------------------------------------------------------
来源：http://www.52xcode.cn/Article/details/gt3csixjcjw.html

使用提醒
来源：http://www.ydjk.org.cn/Article/details/gt3uanovxtk.html

--------------------------------------------------------------------------------
来源：http://www.ydjk.org.cn/Article/details/gt3lhfaiiia.html

1. 示例追求"最小可用"，正式项目中请补齐导入、错误处理与边界判断。
来源：http://www.52xcode.cn/Article/details/gt3hqrdbtcx.html

2. 涉及文件、网络、数据库的示例，注意资源释放与异常捕获。
来源：http://www.ydjk.org.cn/Article/details/gt3whqypkgk.html

3. 语言版本差异较大（如 Python 3.10 的 match、Java 17 的 record/switch 箭头），
来源：http://www.ydjk.org.cn/Article/details/gt3vygexvnl.html

在旧版本上使用前请先确认语法支持情况。
来源：http://www.52xcode.cn/Article/details/gt3zfbpjqta.html

4. 标注"手写"的条目是因为该语言缺少对应内置能力，实际项目中可引入成熟库。
来源：http://www.ydjk.org.cn/Article/details/gt3qcxcthyq.html

—— 文件结束 ——
来源：http://www.52xcode.cn/Article/details/gt3vmctrhls.html

================================================================================
来源：http://www.ydjk.org.cn/Article/details/gt3yaeayybz.html

程序语言常见例子速查手册（2024 版）
来源：http://www.ydjk.org.cn/Article/details/gt3chugalka.html

Common Programming Examples Cheat Book
来源：http://www.ydjk.org.cn/Article/details/gt3uitmnwms.html

================================================================================
来源：http://www.52xcode.cn/Article/details/gt3auxgtchz.html

【收录内容】
来源：http://www.ydjk.org.cn/Article/details/gt3soyzragn.html

覆盖 12 种语言 / 语法与常见 API：
来源：http://www.52xcode.cn/Article/details/gt3ksnfoxef.html

Python · PHP · JavaScript · TypeScript · Java · Go · Ruby · C#
来源：http://www.ydjk.org.cn/Article/details/gt3wmhwmhzl.html

SQL · Bash · C · C++
来源：http://www.52xcode.cn/Article/details/gt3gsuxfxcy.html

按「任务」分组：每个任务下按语言各给出一条最小可用示例。
来源：http://www.ydjk.org.cn/Article/details/gt3wytpneuf.html

【使用说明】
来源：http://www.ydjk.org.cn/Article/details/gt3czmvgesm.html

1. 每个任务形如 "[编号] 任务名"，下面每行以语言标记开头：
来源：http://www.ydjk.org.cn/Article/details/gt3vijbjgru.html

Py:    Python        PHP:   PHP           JS:    JavaScript
来源：http://www.ydjk.org.cn/Article/details/gt3ntcrhcwl.html

TS:    TypeScript    Java:  Java          Go:    Go
来源：http://www.52xcode.cn/Article/details/gt3edzbovmo.html

Ruby:  Ruby          C#:    C#            SQL:   SQL
来源：http://www.52xcode.cn/Article/details/gt3yfvpqkiw.html

Bash:  Shell         C:     C             C++:   C++
来源：http://www.ydjk.org.cn/Article/details/gt3fzilouzs.html

2. 示例只展示核心写法，刻意省略 import / require / include / using 等样板代码。
来源：http://www.52xcode.cn/Article/details/gt3dyjqcbho.html

需要完整可运行文件时，请自行补齐当前语言的导入语句。
来源：http://www.ydjk.org.cn/Article/details/gt3uygzpred.html

3. 语法基准：Python 3.10+ / PHP 8.1+ / ES2020+ / TypeScript 5 / Java 17 /
来源：http://www.ydjk.org.cn/Article/details/gt3idnzeubm.html

Go 1.21+ / Ruby 3.x / C# 10+ / C17 / C++17。
来源：http://www.52xcode.cn/Article/details/gt3xqahspzo.html

4. 检索建议：用编辑器或浏览器 Ctrl+F 搜关键词，如 "排序" "读取文件" "正则"。
来源：http://www.ydjk.org.cn/Article/details/gt3syaorzau.html

5. 标记为 "// 无" 表示该语言没有对应的一等语法，需用替代写法（示例给出替代方案）。
来源：http://www.ydjk.org.cn/Article/details/gt3cnigwztz.html

6. 符号 "⏎" 表示代码在此处换行（主要用于 Python 等强制缩进、无法压成一行的结构）。
来源：http://www.52xcode.cn/Article/details/gt3tlvefvvn.html

【文件统计】
来源：http://www.52xcode.cn/Article/details/gt3usesbwbg.html

语言示例共 2106 条，分布见本文末尾的「统计汇总」。
来源：http://www.52xcode.cn/Article/details/gt3jxewpohx.html

--------------------------------------------------------------------------------
来源：http://www.52xcode.cn/Article/details/gt3xevmibzo.html

目  录
来源：http://www.52xcode.cn/Article/details/gt3ayvtuuym.html

--------------------------------------------------------------------------------
来源：http://www.ydjk.org.cn/Article/details/gt3gojgvhzy.html

A. 基础语法与类型              （第 1 节，26 个任务，208 条）
来源：http://www.ydjk.org.cn/Article/details/gt3gatfwzou.html

B. 流程控制                    （第 2 节，16 个任务，128 条）
来源：http://www.ydjk.org.cn/Article/details/gt3kkopoorp.html

C. 函数与作用域                （第 3 节，16 个任务，128 条）
来源：http://www.ydjk.org.cn/Article/details/gt3izitwgqd.html

D. 数组 / 列表 / 集合          （第 4 节，26 个任务，208 条）
来源：http://www.52xcode.cn/Article/details/gt3dytpuczb.html

E. 字符串处理                  （第 5 节，22 个任务，176 条）
来源：http://www.ydjk.org.cn/Article/details/gt3niuutsgh.html

F. 文件与目录                  （第 6 节，12 个任务，96 条）
来源：http://www.52xcode.cn/Article/details/gt3wzwzwwcr.html

G. 面向对象                    （第 7 节，16 个任务，128 条）
来源：http://www.ydjk.org.cn/Article/details/gt3utbsfzyn.html

H. 异常与错误处理              （第 8 节，10 个任务，80 条）
来源：http://www.52xcode.cn/Article/details/gt3ercgdkia.html

I. 正则表达式                  （第 9 节，8 个任务，64 条）
来源：http://www.ydjk.org.cn/Article/details/gt3thlvvpyz.html

J. 日期与时间                  （第 10 节，10 个任务，80 条）
来源：http://www.52xcode.cn/Article/details/gt3dzafwskh.html

K. JSON 与序列化               （第 11 节，8 个任务，64 条）
来源：http://www.ydjk.org.cn/Article/details/gt3dllcknvk.html

L. 网络请求                    （第 12 节，8 个任务，64 条）
来源：http://www.ydjk.org.cn/Article/details/gt3zmjfltsa.html

M. 命令行 / 进程 / 环境        （第 13 节，8 个任务，64 条）
来源：http://www.ydjk.org.cn/Article/details/gt3zlrsupak.html

N. 数据结构与算法              （第 14 节，12 个任务，96 条）
来源：http://www.ydjk.org.cn/Article/details/gt3zwsazqip.html

O. 并发与异步                  （第 15 节，6 个任务，48 条）
来源：http://www.52xcode.cn/Article/details/gt3vixaffqf.html

P. 常用工具函数                （第 16 节，8 个任务，64 条）
来源：http://www.52xcode.cn/Article/details/gt3bvyavzcx.html

Q. SQL 专题                    （第 17 节，90 条）
来源：http://www.ydjk.org.cn/Article/details/gt3ksuqjpnl.html


<!-- 参考信息 -->