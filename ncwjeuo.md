代发 wailian999

[U27] Py：异步 HTTP
来源：http://baike.zdbjq.cn/Article/details/gnilbodlx.sHtML

aiohttp.ClientSession() 配合 async with
来源：http://baike.hesvh.cn/Article/details/gknrziwpl.sHtML

[U28] Py：类型别名
来源：http://baike.fehbvm.com/Article/details/ghkndecag.sHtML

UserId = int
来源：http://mobile.fehbvm.com/Article/details/gcudiwebf.sHtML

[U29] Py：属性校验
来源：http://mobile.hesvh.cn/Article/details/gkcurhwaw.sHtML

@property 与 @x.setter 配合
来源：http://www.m.share.zdbjq.cn/Article/details/gidiolwqu.sHtML

[U30] Py：数据类
来源：http://wap.hesvh.cn/Article/details/gblyopurz.sHtML

@dataclass(slots=True)
来源：http://3g.zdbjq.cn/Article/details/gvtzovrhf.sHtML

[U31] Py：单测
来源：http://baike.hesvh.cn/Article/details/gbnlyysfl.sHtML

python -m pytest -q
来源：http://baike.fehbvm.com/Article/details/glwuuegos.sHtML

[U32] Py：代码格式化
来源：http://blog.fehbvm.com/Article/details/gdwnedico.sHtML

ruff format . && ruff check --fix .
来源：http://www.share.hesvh.cn/Article/details/gojkjfijr.sHtML

[U33] Py：打包发布
来源：http://3g.hesvh.cn/Article/details/gtheoecib.sHtML

python -m build  （依赖 pyproject.toml）
来源：http://www.blog.hesvh.cn/Article/details/gcefmvkkk.sHtML

[U34] Py：判断编码
来源：http://mobile.hesvh.cn/Article/details/gtdciklga.sHtML

chardet.detect(raw)
来源：http://m.share.hesvh.cn/Article/details/grycyujtw.sHtML

[U35] Py：发送邮件
来源：http://www.share.hesvh.cn/Article/details/gpsjvgtzr.sHtML

smtplib.SMTP_SSL(...).send_message(msg)
来源：http://www.m.share.fehbvm.com/Article/details/gmqeuhicy.sHtML

[U36] Py：定时任务
来源：http://www.share.hesvh.cn/Article/details/gcuhuejgt.sHtML

schedule.every(10).minutes.do(job)
来源：http://www.blog.fehbvm.com/Article/details/gekeaagfe.sHtML

[U37] Py：读写 Excel
来源：http://www.m.share.fehbvm.com/Article/details/gljedcawn.sHtML

pandas.read_excel / DataFrame.to_excel
来源：http://www.blog.zdbjq.cn/Article/details/ggmnhzohk.sHtML

[U38] Py：获取脚本所在目录
来源：http://wap.zdbjq.cn/Article/details/gqhfkwzok.sHtML

Path(__file__).resolve().parent
来源：http://3g.fehbvm.com/Article/details/gqnmkcrio.sHtML

[U39] Py：判断是否在交互环境
来源：http://mobile.zdbjq.cn/Article/details/gjompqlie.sHtML

sys.stdout.isatty()
来源：http://baike.fehbvm.com/Article/details/gdcaxtnjs.sHtML

[U40] Py：打印到标准错误
来源：http://wap.zdbjq.cn/Article/details/gcdkrkwhu.sHtML

print("err", file=sys.stderr)
来源：http://3g.zdbjq.cn/Article/details/gfpbphrex.sHtML

[U41] PHP：初始化 Composer 项目
来源：http://blog.hesvh.cn/Article/details/gnapjadop.sHtML

composer init;  composer require guzzlehttp/guzzle
来源：http://wap.fehbvm.com/Article/details/golhilpxe.sHtML

[U42] PHP：PSR-4 自动加载
来源：http://blog.zdbjq.cn/Article/details/gnbnhossd.sHtML

"autoload": { "psr-4": { "App\\": "src/" } }
来源：http://www.m.share.zdbjq.cn/Article/details/ggdtebrkh.sHtML

[U43] PHP：声明命名空间
来源：http://3g.hesvh.cn/Article/details/gvgiyadkg.sHtML

namespace App\Http;
来源：http://www.blog.zdbjq.cn/Article/details/gcbqrlmzf.sHtML

[U44] PHP：开启严格类型
来源：http://blog.fehbvm.com/Article/details/gzpbnkrcm.sHtML

declare(strict_types=1);
来源：http://m.share.zdbjq.cn/Article/details/gxgkuyktl.sHtML

[U45] PHP：类型声明与返回类型
来源：http://3g.zdbjq.cn/Article/details/gkilapkuo.sHtML

function add(int $a, int $b): int { return $a + $b; }
来源：http://read.share.hesvh.cn/Article/details/gphtwoshh.sHtML

[U46] PHP：可空类型
来源：http://www.blog.hesvh.cn/Article/details/gjfxvfovr.sHtML

?string $name = null
来源：http://www.blog.zdbjq.cn/Article/details/gjubxrhnh.sHtML

[U47] PHP：联合类型
来源：http://blog.zdbjq.cn/Article/details/gpalvnqbc.sHtML

int|string $id
来源：http://mobile.fehbvm.com/Article/details/ghdfarxgb.sHtML

[U48] PHP：纯枚举
来源：http://www.m.share.fehbvm.com/Article/details/gjpygnbkf.sHtML

enum Status: string { case Active = "active"; case Off = "off"; }
来源：http://www.blog.fehbvm.com/Article/details/gefxvonxj.sHtML

[U49] PHP：只读属性
来源：http://blog.fehbvm.com/Article/details/gjoexpvzv.sHtML

public readonly string $name
来源：http://3g.zdbjq.cn/Article/details/gsryxhjra.sHtML

[U50] PHP：构造器属性提升
来源：http://read.share.hesvh.cn/Article/details/gmnkoyptt.sHtML

public function __construct(private int $id) {}
来源：http://m.share.hesvh.cn/Article/details/gyghfqiua.sHtML

[U51] PHP：数组解构
来源：http://wap.hesvh.cn/Article/details/gpwvlrlmt.sHtML

[$a, $b] = $arr;
来源：http://www.share.fehbvm.com/Article/details/gzjbxvtci.sHtML

[U52] PHP：箭头函数
来源：http://3g.fehbvm.com/Article/details/gnssirftg.sHtML

$double = fn($x) => $x * 2;
来源：http://mobile.zdbjq.cn/Article/details/gmilrbzvv.sHtML

[U53] PHP：空合并运算符
来源：http://mobile.zdbjq.cn/Article/details/ghdjsvwue.sHtML

$v = $a ?? $b ?? "default";
来源：http://3g.zdbjq.cn/Article/details/geuwxeosk.sHtML

[U54] PHP：空安全调用
来源：http://www.blog.fehbvm.com/Article/details/gjwbyrvos.sHtML

$obj?->method()
来源：http://wap.zdbjq.cn/Article/details/gpqdrzlly.sHtML

[U55] PHP：match 表达式
来源：http://wap.fehbvm.com/Article/details/gbbekndhj.sHtML

$s = match($x) { 1 => "一", default => "其他" };
来源：http://3g.hesvh.cn/Article/details/gcaitohmm.sHtML

[U56] PHP：命名参数
来源：http://www.share.fehbvm.com/Article/details/gcsukhlgi.sHtML

f(a: 1, b: 2)
来源：http://3g.hesvh.cn/Article/details/gfupnckrz.sHtML

[U57] PHP：字符串插值
来源：http://baike.hesvh.cn/Article/details/gcuexmlrf.sHtML

"值: {$a}"
来源：http://3g.zdbjq.cn/Article/details/gaftvrgsu.sHtML

[U58] PHP：数组三件套
来源：http://www.m.share.zdbjq.cn/Article/details/gacvkobov.sHtML

array_map($f, $a);  array_filter($a, $f);  array_reduce($a, $f, 0);
来源：http://www.m.share.zdbjq.cn/Article/details/germubtmu.sHtML

[U59] PHP：自定义排序
来源：http://www.share.fehbvm.com/Article/details/gdexxvssb.sHtML

usort($arr, fn($a, $b) => $a["age"] <=> $b["age"]);
来源：http://mobile.hesvh.cn/Article/details/gkitbjbfl.sHtML

[U60] PHP：JSON 编解码
来源：http://baike.zdbjq.cn/Article/details/gtlgslmfg.sHtML

json_encode($d, JSON_UNESCAPED_UNICODE);  json_decode($s, true);
来源：http://mobile.fehbvm.com/Article/details/gnkdnwags.sHtML

[U61] PHP：正则
来源：http://read.share.hesvh.cn/Article/details/guazdurrt.sHtML

preg_match('/(\d+)/', $s, $m);  preg_replace('/\d+/', '#', $s);
来源：http://mobile.fehbvm.com/Article/details/glfwgvzmc.sHtML

[U62] PHP：日期对象
来源：http://baike.fehbvm.com/Article/details/gdcntyyln.sHtML

(new DateTimeImmutable())->format("Y-m-d");
来源：http://www.blog.zdbjq.cn/Article/details/gmsqaslhb.sHtML

[U63] PHP：文件读写
来源：http://www.share.hesvh.cn/Article/details/gucgyenlt.sHtML

file_get_contents($f);  file_put_contents($f, $data);
来源：http://baike.fehbvm.com/Article/details/ghpkfoxkr.sHtML

[U64] PHP：目录遍历
来源：http://www.share.zdbjq.cn/Article/details/gdhdoygwu.sHtML

glob("dir/*.php");  scandir("dir");
来源：http://blog.hesvh.cn/Article/details/guwhdzmnw.sHtML

[U65] PHP：会话
来源：http://3g.hesvh.cn/Article/details/gloukfawu.sHtML

session_start();  $_SESSION["uid"] = 1;
来源：http://mobile.zdbjq.cn/Article/details/ghtwsgjkp.sHtML

[U66] PHP：设置 Cookie
来源：http://m.share.hesvh.cn/Article/details/gsiwvhizz.sHtML

setcookie("token", $v, ["httponly" => true, "samesite" => "Lax"]);
来源：http://www.share.zdbjq.cn/Article/details/gyupioxgz.sHtML

[U67] PHP：处理文件上传
来源：http://read.share.zdbjq.cn/Article/details/gashqqkta.sHtML

$_FILES["file"]["tmp_name"] 与 move_uploaded_file()
来源：http://www.m.share.hesvh.cn/Article/details/goqvdxjya.sHtML

[U68] PHP：PDO 连接
来源：http://mobile.hesvh.cn/Article/details/gvpimqezv.sHtML

$pdo = new PDO("mysql:host=localhost;dbname=app", "root", "");
来源：http://m.share.hesvh.cn/Article/details/gsztehlcw.sHtML

[U69] PHP：PDO 预处理
来源：http://3g.hesvh.cn/Article/details/gcfdltbdo.sHtML

$stmt = $pdo->prepare("SELECT * FROM users WHERE id = ?");  $stmt->execute([$id]);
来源：http://baike.hesvh.cn/Article/details/gduaannrw.sHtML

[U70] PHP：PDO 事务
来源：http://mobile.hesvh.cn/Article/details/glfdlkdfy.sHtML

$pdo->beginTransaction();  $pdo->commit();  $pdo->rollBack();
来源：http://m.share.zdbjq.cn/Article/details/gmvpnaeyu.sHtML

[U71] PHP：抛出异常
来源：http://www.share.fehbvm.com/Article/details/ggpjqzpjt.sHtML

throw new RuntimeException("失败", 500);
来源：http://wap.zdbjq.cn/Article/details/gvgtffyfc.sHtML

[U72] PHP：写错误日志
来源：http://baike.hesvh.cn/Article/details/gsohfmqxx.sHtML

error_log("失败: " . $e->getMessage());
来源：http://3g.hesvh.cn/Article/details/gkssubrgh.sHtML

[U73] PHP：读取 ini 配置
来源：http://www.m.share.zdbjq.cn/Article/details/gagzqcyxd.sHtML

parse_ini_file("config.ini", true)
来源：http://www.blog.fehbvm.com/Article/details/gjxtzswkj.sHtML

[U74] PHP：读取环境变量
来源：http://blog.hesvh.cn/Article/details/grresvfxl.sHtML

getenv("APP_ENV") ?: "production"
来源：http://www.blog.hesvh.cn/Article/details/gaqzbtxpn.sHtML

[U75] PHP：依赖注入
来源：http://read.share.zdbjq.cn/Article/details/gzjiubmlt.sHtML

composer require psr/container
来源：http://mobile.zdbjq.cn/Article/details/gwogqvcpr.sHtML

[U76] PHP：简单路由
来源：http://baike.hesvh.cn/Article/details/gponrbusi.sHtML

$path = parse_url($_SERVER["REQUEST_URI"], PHP_URL_PATH);
来源：http://www.m.share.zdbjq.cn/Article/details/grwjekutb.sHtML

[U77] PHP：模板渲染
来源：http://read.share.zdbjq.cn/Article/details/govgyeabb.sHtML

composer require twig/twig
来源：http://m.share.hesvh.cn/Article/details/gijllrsvm.sHtML

[U78] PHP：单元测试
来源：http://3g.zdbjq.cn/Article/details/gxurkhoiw.sHtML

composer require --dev phpunit/phpunit
来源：http://3g.hesvh.cn/Article/details/gewndzmmr.sHtML

[U79] PHP：静态分析
来源：http://m.share.zdbjq.cn/Article/details/gdbkjywzk.sHtML

composer require --dev phpstan/phpstan
来源：http://3g.fehbvm.com/Article/details/gbcmpjxdr.sHtML

[U80] PHP：代码规范修复
来源：http://www.share.fehbvm.com/Article/details/gpysruhja.sHtML

composer require --dev friendsofphp/php-cs-fixer
来源：http://m.share.fehbvm.com/Article/details/gxtdklpky.sHtML

[U81] JS：初始化项目
来源：http://wap.zdbjq.cn/Article/details/gphgisgoz.sHtML

npm init -y;  npm i express
来源：http://mobile.zdbjq.cn/Article/details/gnpzdhspu.sHtML

[U82] JS：package.json 脚本
来源：http://baike.hesvh.cn/Article/details/gzutbebot.sHtML

"scripts": { "dev": "vite", "build": "vite build" }
来源：http://baike.fehbvm.com/Article/details/gegzrsssy.sHtML

[U83] JS：ES Module 导入导出
来源：http://3g.fehbvm.com/Article/details/gaqkuunza.sHtML

export const a = 1;  import { a } from "./m.js";
来源：http://3g.fehbvm.com/Article/details/gosekuvrh.sHtML

[U84] JS：CommonJS 写法
来源：http://m.share.zdbjq.cn/Article/details/guizimfqj.sHtML

module.exports = { a };  const { a } = require("./m");
来源：http://www.blog.zdbjq.cn/Article/details/gnquahdcd.sHtML

[U85] JS：可选链
来源：http://baike.hesvh.cn/Article/details/gqlmtykcw.sHtML

a?.b?.c
来源：http://www.m.share.hesvh.cn/Article/details/gcrvhiivs.sHtML

[U86] JS：空值合并
来源：http://wap.hesvh.cn/Article/details/gfvqnnpub.sHtML

a ?? b
来源：http://baike.hesvh.cn/Article/details/gixmsxohe.sHtML

[U87] JS：解构默认值
来源：http://www.m.share.zdbjq.cn/Article/details/gfwffnnhi.sHtML

const { a = 1, b = 2 } = obj;
来源：http://mobile.fehbvm.com/Article/details/glltpcgbr.sHtML

[U88] JS：对象展开合并
来源：http://wap.hesvh.cn/Article/details/gejntxcys.sHtML

{ ...a, ...b }
来源：http://www.blog.zdbjq.cn/Article/details/ggbrxhgjp.sHtML

[U89] JS：数组去重
来源：http://mobile.hesvh.cn/Article/details/gcbgxqabc.sHtML

[...new Set(arr)]
来源：http://mobile.zdbjq.cn/Article/details/guzhpyigv.sHtML

[U90] JS：数字数组排序
来源：http://wap.fehbvm.com/Article/details/gecokztam.sHtML

[...arr].sort((a, b) => a - b)
来源：http://wap.fehbvm.com/Article/details/guncklszw.sHtML

[U91] JS：对象键值遍历
来源：http://blog.fehbvm.com/Article/details/gfcvgaxym.sHtML

Object.entries(obj).forEach(([k, v]) => {});
来源：http://wap.hesvh.cn/Article/details/gtwawqvnu.sHtML

[U92] JS：深拷贝
来源：http://blog.hesvh.cn/Article/details/gtxripegz.sHtML

structuredClone(obj)
来源：http://3g.zdbjq.cn/Article/details/gtshussnp.sHtML

[U93] JS：模板字符串
来源：http://www.m.share.fehbvm.com/Article/details/ggrquwpnb.sHtML

`共 ${n} 条`
来源：http://read.share.zdbjq.cn/Article/details/gvorfvgfi.sHtML

[U94] JS：箭头函数
来源：http://www.blog.zdbjq.cn/Article/details/gizlsnltb.sHtML

const double = x => x * 2;
来源：http://www.m.share.zdbjq.cn/Article/details/gpaclkrmo.sHtML

[U95] JS：Promise 包装
来源：http://mobile.fehbvm.com/Article/details/grauvjmpm.sHtML

new Promise((resolve, reject) => {})
来源：http://blog.hesvh.cn/Article/details/goevddfxx.sHtML

[U96] JS：async/await 与异常
来源：http://baike.fehbvm.com/Article/details/gcctjcrqi.sHtML

try { const d = await f(); } catch (e) { console.error(e); }
来源：http://baike.fehbvm.com/Article/details/gymwvtucx.sHtML

[U97] JS：并发请求
来源：http://www.blog.zdbjq.cn/Article/details/gispofgji.sHtML

await Promise.all(urls.map(u => fetch(u)))
来源：http://wap.fehbvm.com/Article/details/gjqyoibva.sHtML

[U98] JS：fetch 带 JSON
来源：http://wap.fehbvm.com/Article/details/gycbhojlr.sHtML

await fetch(url, { method: "POST", headers: { "Content-Type": "application/json" }, body: JSON.stringify(d) })
来源：http://blog.hesvh.cn/Article/details/gkozffrju.sHtML

[U99] JS：事件监听
来源：http://read.share.hesvh.cn/Article/details/guejxncid.sHtML

el.addEventListener("click", e => {})
来源：http://www.m.share.fehbvm.com/Article/details/gmqqfcsah.sHtML

[U100] JS：DOM 查询
来源：http://m.share.fehbvm.com/Article/details/glwejqlda.sHtML

document.querySelector(".item")
来源：http://blog.fehbvm.com/Article/details/gkzaewwcc.sHtML

[U101] JS：classList 操作
来源：http://mobile.zdbjq.cn/Article/details/guwqmpunt.sHtML

el.classList.toggle("active")
来源：http://www.m.share.hesvh.cn/Article/details/gmcsipetv.sHtML

[U102] JS：本地存储
来源：http://blog.hesvh.cn/Article/details/gczkaiaoh.sHtML

localStorage.setItem("k", JSON.stringify(v))
来源：http://3g.fehbvm.com/Article/details/gvfrtwxad.sHtML

[U103] JS：定时器
来源：http://www.m.share.fehbvm.com/Article/details/grlaunyra.sHtML

setTimeout(fn, 1000);  setInterval(fn, 1000);
来源：http://wap.zdbjq.cn/Article/details/gorolcfaw.sHtML

[U104] JS：防抖
来源：http://www.blog.hesvh.cn/Article/details/gijlwmiax.sHtML

const debounce = (fn, ms) => { let t; return (...a) => { clearTimeout(t); t = setTimeout(() => fn(...a), ms); }; };
来源：http://blog.hesvh.cn/Article/details/gjaohgaer.sHtML

[U105] JS：节流
来源：http://www.m.share.hesvh.cn/Article/details/gdhhzilii.sHtML

const throttle = (fn, ms) => { let last = 0; return (...a) => { const n = Date.now(); if (n - last >= ms) { last = n; fn(...a); } }; };
来源：http://www.m.share.fehbvm.com/Article/details/gqmcfnpti.sHtML

[U106] JS：日期格式化
来源：http://3g.fehbvm.com/Article/details/gkvszwmpf.sHtML

new Intl.DateTimeFormat("zh-CN", { dateStyle: "medium" }).format(new Date())
来源：http://m.share.hesvh.cn/Article/details/gvkylgyua.sHtML

[U107] JS：数字千分位
来源：http://blog.fehbvm.com/Article/details/ggutmbiul.sHtML

new Intl.NumberFormat("en-US").format(1234567)
来源：http://www.blog.hesvh.cn/Article/details/glamjvefk.sHtML

[U108] JS：随机整数
来源：http://baike.fehbvm.com/Article/details/gsdeytlzw.sHtML

Math.floor(Math.random() * (max - min + 1)) + min
来源：http://read.share.fehbvm.com/Article/details/gwzrtmfpb.sHtML

[U109] JS：数组分组
来源：http://m.share.zdbjq.cn/Article/details/gwtbgblsj.sHtML

Object.groupBy(arr, x => x.type)
来源：http://baike.hesvh.cn/Article/details/gvbnkhdab.sHtML

[U110] JS：数组分块
来源：http://wap.zdbjq.cn/Article/details/gmfprimtb.sHtML

arr.reduce((acc, x, i) => (i % size ? acc : [...acc, arr.slice(i, i + size)]), [])
来源：http://baike.zdbjq.cn/Article/details/gylpkrkqo.sHtML

[U111] JS：对象转 Map
来源：http://mobile.fehbvm.com/Article/details/glduqjkck.sHtML

new Map(Object.entries(obj))
来源：http://mobile.hesvh.cn/Article/details/gkkbuazaj.sHtML

[U112] JS：字符串补位
来源：http://read.share.fehbvm.com/Article/details/gkjgivqnw.sHtML

"7".padStart(3, "0")
来源：http://m.share.zdbjq.cn/Article/details/gkkghdqke.sHtML

[U113] JS：正则替换全部
来源：http://www.blog.fehbvm.com/Article/details/gqzuhfqxm.sHtML

s.replaceAll("a", "b")
来源：http://www.blog.hesvh.cn/Article/details/gtkhtwwca.sHtML

[U114] JS：JSON 深比较
来源：http://www.blog.zdbjq.cn/Article/details/gzselkgqo.sHtML

JSON.stringify(a) === JSON.stringify(b)
来源：http://3g.fehbvm.com/Article/details/gdzrwmtqb.sHtML

[U115] JS：生成 UUID
来源：http://3g.fehbvm.com/Article/details/gtulgphou.sHtML

crypto.randomUUID()
来源：http://blog.zdbjq.cn/Article/details/gqjwsylzy.sHtML

[U116] JS：类型检查（JSDoc）
来源：http://m.share.zdbjq.cn/Article/details/gbasjcvzo.sHtML

/** @param {string} name */ function f(name) {}
来源：http://blog.hesvh.cn/Article/details/gdecxlmta.sHtML

[U117] JS：单元测试
来源：http://m.share.zdbjq.cn/Article/details/gtchlisyd.sHtML

npm i -D vitest;  npx vitest
来源：http://www.share.zdbjq.cn/Article/details/grgbqbbcj.sHtML

[U118] JS：开发服务器
来源：http://blog.zdbjq.cn/Article/details/geepqweck.sHtML

npm i -D vite;  npx vite
来源：http://m.share.fehbvm.com/Article/details/gwvmzhvav.sHtML

[U119] JS：生产构建
来源：http://mobile.hesvh.cn/Article/details/ggkzczqkb.sHtML

npx vite build
来源：http://wap.zdbjq.cn/Article/details/gdxfkjzis.sHtML

[U120] JS：读取环境变量（Vite）
来源：http://www.blog.fehbvm.com/Article/details/gquditlyo.sHtML

import.meta.env.VITE_API_URL
来源：http://www.share.fehbvm.com/Article/details/gdvxjksvd.sHtML

================================================================================
来源：http://mobile.zdbjq.cn/Article/details/gulvtwhuq.sHtML

统计汇总
来源：http://m.share.hesvh.cn/Article/details/glbufzgyg.sHtML

================================================================================
来源：http://baike.zdbjq.cn/Article/details/gpgajskgt.sHtML

按语言统计（条）：
来源：http://3g.fehbvm.com/Article/details/gdygcaoir.sHtML

Python ......... 252
来源：http://mobile.zdbjq.cn/Article/details/gosbvprma.sHtML

PHP ............ 252
来源：http://wap.fehbvm.com/Article/details/gzatuhvsj.sHtML

JavaScript ..... 252
来源：http://baike.zdbjq.cn/Article/details/gorgkehom.sHtML

TypeScript ..... 212
来源：http://3g.fehbvm.com/Article/details/gvlntwvnv.sHtML

Java ........... 212
来源：http://www.m.share.hesvh.cn/Article/details/gwqrdwnlq.sHtML

Go ............. 212
来源：http://www.share.fehbvm.com/Article/details/guwmaunvn.sHtML

Ruby ........... 212
来源：http://www.share.zdbjq.cn/Article/details/gwaagrmiz.sHtML

C# ............. 212
来源：http://mobile.hesvh.cn/Article/details/gugzjgkbb.sHtML

C .............. 30
来源：http://www.blog.fehbvm.com/Article/details/gzexqakhm.sHtML

C++ ............ 30
来源：http://mobile.zdbjq.cn/Article/details/gfqointln.sHtML

SQL ............ 90
来源：http://m.share.hesvh.cn/Article/details/gpnrrfygj.sHtML

Bash ........... 80
来源：http://mobile.zdbjq.cn/Article/details/gjrcybvkf.sHtML

Kotlin ......... 15
来源：http://www.m.share.zdbjq.cn/Article/details/gxanoedvo.sHtML

Swift .......... 15
来源：http://www.share.hesvh.cn/Article/details/gcpgddvru.sHtML

Lua ............ 10
来源：http://m.share.hesvh.cn/Article/details/gamwdtget.sHtML

Perl ........... 10
来源：http://www.blog.zdbjq.cn/Article/details/goearvage.sHtML

Scala .......... 10
来源：http://baike.zdbjq.cn/Article/details/gdzkjqmsi.sHtML

------------------------------------
来源：http://3g.zdbjq.cn/Article/details/grvyotkrz.sHtML

合计 ........... 2106 条
来源：http://www.share.zdbjq.cn/Article/details/goiiehzge.sHtML

按章节统计：
来源：http://baike.fehbvm.com/Article/details/gsnhguwfj.sHtML

A 基础语法与类型       26 个任务 × 8 语言 =  208
来源：http://read.share.fehbvm.com/Article/details/gipfexwsh.sHtML

B 流程控制             16 个任务 × 8 语言 =  128
来源：http://www.share.zdbjq.cn/Article/details/geqxmkigl.sHtML

C 函数与作用域         16 个任务 × 8 语言 =  128
来源：http://m.share.hesvh.cn/Article/details/gzsbceapm.sHtML

D 数组 / 列表 / 集合   26 个任务 × 8 语言 =  208
来源：http://m.share.fehbvm.com/Article/details/gbqoznbyx.sHtML

E 字符串处理           22 个任务 × 8 语言 =  176
来源：http://mobile.zdbjq.cn/Article/details/gcwforeyh.sHtML

F 文件与目录           12 个任务 × 8 语言 =   96
来源：http://www.share.fehbvm.com/Article/details/gphlulrno.sHtML

G 面向对象             16 个任务 × 8 语言 =  128
来源：http://www.blog.hesvh.cn/Article/details/gujwreglh.sHtML

H 异常与错误处理       10 个任务 × 8 语言 =   80
来源：http://3g.hesvh.cn/Article/details/gswivwfcm.sHtML

I 正则表达式            8 个任务 × 8 语言 =   64
来源：http://mobile.zdbjq.cn/Article/details/gnefwiksl.sHtML

J 日期与时间           10 个任务 × 8 语言 =   80
来源：http://baike.fehbvm.com/Article/details/gplalgucf.sHtML

K JSON 与序列化         8 个任务 × 8 语言 =   64
来源：http://baike.fehbvm.com/Article/details/gvwkhyjmx.sHtML

L 网络请求              8 个任务 × 8 语言 =   64
来源：http://read.share.zdbjq.cn/Article/details/gecwmlugk.sHtML

M 命令行 / 进程         8 个任务 × 8 语言 =   64
来源：http://mobile.zdbjq.cn/Article/details/gywkskynw.sHtML

N 数据结构与算法       12 个任务 × 8 语言 =   96
来源：http://www.share.zdbjq.cn/Article/details/gsasmblni.sHtML

O 并发与异步            6 个任务 × 8 语言 =   48
来源：http://www.share.fehbvm.com/Article/details/grbxkhgcl.sHtML

P 常用工具函数          8 个任务 × 8 语言 =   64
来源：http://blog.hesvh.cn/Article/details/gaqqivydf.sHtML

Q SQL 专题                              90
来源：http://m.share.fehbvm.com/Article/details/glsxsadap.sHtML

R Bash 专题                             80
来源：http://baike.fehbvm.com/Article/details/gslmyyumb.sHtML

S C / C++ 专题                          60
来源：http://www.m.share.zdbjq.cn/Article/details/grwpsjkbe.sHtML

T 其他语言补充                          60
来源：http://blog.hesvh.cn/Article/details/gymfvfxhk.sHtML

U 高频实用片段                         120
来源：http://mobile.zdbjq.cn/Article/details/gqurlbirw.sHtML

------------------------------------
来源：http://www.blog.fehbvm.com/Article/details/gxylgiedj.sHtML

合计                                  2106 条
来源：http://mobile.fehbvm.com/Article/details/ggcljxgjt.sHtML

--------------------------------------------------------------------------------
来源：http://read.share.fehbvm.com/Article/details/gtwaxvvsi.sHtML

使用提醒
来源：http://www.m.share.fehbvm.com/Article/details/ggyakujks.sHtML

--------------------------------------------------------------------------------
来源：http://www.blog.fehbvm.com/Article/details/gmrrsrwtp.sHtML

1. 示例追求"最小可用"，正式项目中请补齐导入、错误处理与边界判断。
来源：http://www.blog.hesvh.cn/Article/details/gdgksdlyl.sHtML

2. 涉及文件、网络、数据库的示例，注意资源释放与异常捕获。
来源：http://www.share.hesvh.cn/Article/details/gxwyroxzq.sHtML

3. 语言版本差异较大（如 Python 3.10 的 match、Java 17 的 record/switch 箭头），
来源：http://baike.zdbjq.cn/Article/details/gxabuzbrb.sHtML

在旧版本上使用前请先确认语法支持情况。
来源：http://mobile.fehbvm.com/Article/details/gubtlcfaj.sHtML

4. 标注"手写"的条目是因为该语言缺少对应内置能力，实际项目中可引入成熟库。
来源：http://3g.hesvh.cn/Article/details/gehfbejyb.sHtML

—— 文件结束 ——
来源：http://www.blog.hesvh.cn/Article/details/gjzxauiri.sHtML

================================================================================
来源：http://read.share.zdbjq.cn/Article/details/gihjsvers.sHtML

程序语言常见例子速查手册（2024 版）
来源：http://www.blog.zdbjq.cn/Article/details/gkzxilcjf.sHtML

Common Programming Examples Cheat Book
来源：http://www.blog.zdbjq.cn/Article/details/gcrhdhzss.sHtML

================================================================================
来源：http://read.share.hesvh.cn/Article/details/gwifiiywr.sHtML

【收录内容】
来源：http://3g.fehbvm.com/Article/details/giajyrodi.sHtML

覆盖 12 种语言 / 语法与常见 API：
来源：http://www.blog.fehbvm.com/Article/details/gxewknyrq.sHtML

Python · PHP · JavaScript · TypeScript · Java · Go · Ruby · C#
来源：http://www.m.share.zdbjq.cn/Article/details/gcgwujuyw.sHtML

SQL · Bash · C · C++
来源：http://www.share.hesvh.cn/Article/details/ggsalgpzl.sHtML

按「任务」分组：每个任务下按语言各给出一条最小可用示例。
来源：http://www.share.zdbjq.cn/Article/details/gwbjzzjjp.sHtML

【使用说明】
来源：http://www.m.share.hesvh.cn/Article/details/gvlwqfmpl.sHtML

1. 每个任务形如 "[编号] 任务名"，下面每行以语言标记开头：
来源：http://blog.zdbjq.cn/Article/details/gadublmfi.sHtML

Py:    Python        PHP:   PHP           JS:    JavaScript
来源：http://www.blog.hesvh.cn/Article/details/gorpubyac.sHtML

TS:    TypeScript    Java:  Java          Go:    Go
来源：http://read.share.zdbjq.cn/Article/details/gavenwtqm.sHtML

Ruby:  Ruby          C#:    C#            SQL:   SQL
来源：http://blog.hesvh.cn/Article/details/gwbgerqnm.sHtML

Bash:  Shell         C:     C             C++:   C++
来源：http://www.m.share.zdbjq.cn/Article/details/goyvfuazh.sHtML

2. 示例只展示核心写法，刻意省略 import / require / include / using 等样板代码。
来源：http://read.share.fehbvm.com/Article/details/gtnprmfxl.sHtML

需要完整可运行文件时，请自行补齐当前语言的导入语句。
来源：http://read.share.zdbjq.cn/Article/details/gjkniabqk.sHtML

3. 语法基准：Python 3.10+ / PHP 8.1+ / ES2020+ / TypeScript 5 / Java 17 /
来源：http://baike.hesvh.cn/Article/details/gjgxrcscv.sHtML

Go 1.21+ / Ruby 3.x / C# 10+ / C17 / C++17。
来源：http://www.m.share.zdbjq.cn/Article/details/gefxydeej.sHtML

4. 检索建议：用编辑器或浏览器 Ctrl+F 搜关键词，如 "排序" "读取文件" "正则"。
来源：http://wap.fehbvm.com/Article/details/gkxhirmvx.sHtML

5. 标记为 "// 无" 表示该语言没有对应的一等语法，需用替代写法（示例给出替代方案）。
来源：http://m.share.hesvh.cn/Article/details/gsakpnkdx.sHtML

6. 符号 "⏎" 表示代码在此处换行（主要用于 Python 等强制缩进、无法压成一行的结构）。
来源：http://3g.zdbjq.cn/Article/details/gppapdpzh.sHtML

【文件统计】
来源：http://wap.fehbvm.com/Article/details/gvgkptowz.sHtML

语言示例共 2106 条，分布见本文末尾的「统计汇总」。
来源：http://read.share.fehbvm.com/Article/details/gtjtbhzpo.sHtML

--------------------------------------------------------------------------------
来源：http://read.share.hesvh.cn/Article/details/gvsyetkwx.sHtML

目  录
来源：http://read.share.zdbjq.cn/Article/details/gyaqgeusb.sHtML

--------------------------------------------------------------------------------
来源：http://m.share.hesvh.cn/Article/details/gnpjcklwe.sHtML

A. 基础语法与类型              （第 1 节，26 个任务，208 条）
来源：http://www.m.share.zdbjq.cn/Article/details/gsuxkfztm.sHtML

B. 流程控制                    （第 2 节，16 个任务，128 条）
来源：http://www.share.fehbvm.com/Article/details/gzukytnpu.sHtML

C. 函数与作用域                （第 3 节，16 个任务，128 条）
来源：http://read.share.zdbjq.cn/Article/details/gtakkvqvy.sHtML

D. 数组 / 列表 / 集合          （第 4 节，26 个任务，208 条）
来源：http://3g.fehbvm.com/Article/details/gnyzhnrwd.sHtML

E. 字符串处理                  （第 5 节，22 个任务，176 条）
来源：http://3g.zdbjq.cn/Article/details/gcrmdkpam.sHtML

F. 文件与目录                  （第 6 节，12 个任务，96 条）
来源：http://www.share.zdbjq.cn/Article/details/gclsjqtfs.sHtML

G. 面向对象                    （第 7 节，16 个任务，128 条）
来源：http://blog.hesvh.cn/Article/details/gwsoqlpnp.sHtML

H. 异常与错误处理              （第 8 节，10 个任务，80 条）
来源：http://wap.hesvh.cn/Article/details/ghdiieavz.sHtML

I. 正则表达式                  （第 9 节，8 个任务，64 条）
来源：http://www.share.hesvh.cn/Article/details/gjspbjbrg.sHtML

J. 日期与时间                  （第 10 节，10 个任务，80 条）
来源：http://mobile.fehbvm.com/Article/details/gklzdhmld.sHtML

K. JSON 与序列化               （第 11 节，8 个任务，64 条）
来源：http://wap.hesvh.cn/Article/details/grojyndvd.sHtML

L. 网络请求                    （第 12 节，8 个任务，64 条）
来源：http://3g.zdbjq.cn/Article/details/gkqcudlqn.sHtML

M. 命令行 / 进程 / 环境        （第 13 节，8 个任务，64 条）
来源：http://www.share.hesvh.cn/Article/details/gacsemodr.sHtML

N. 数据结构与算法              （第 14 节，12 个任务，96 条）
来源：http://www.blog.zdbjq.cn/Article/details/ggstijnmm.sHtML

O. 并发与异步                  （第 15 节，6 个任务，48 条）
来源：http://mobile.zdbjq.cn/Article/details/gieqlummu.sHtML

P. 常用工具函数                （第 16 节，8 个任务，64 条）
来源：http://wap.zdbjq.cn/Article/details/gigfganic.sHtML

Q. SQL 专题                    （第 17 节，90 条）
来源：http://m.share.hesvh.cn/Article/details/gagmorskm.sHtML

R. Bash 专题                   （第 18 节，80 条）
来源：http://mobile.hesvh.cn/Article/details/gkgvoknop.sHtML

S. C / C++ 专题                （第 19 节，60 条）
来源：http://baike.hesvh.cn/Article/details/gurcfnvlb.sHtML

T. 其他语言补充                （第 20 节，60 条：Kotlin / Swift / Lua / Perl / Scala）
来源：http://blog.fehbvm.com/Article/details/gphvgiewp.sHtML

U. 高频实用片段                （第 21 节，120 条：Python / PHP / JavaScript 各 40 条）
来源：http://3g.fehbvm.com/Article/details/gijrqvwho.sHtML

================================================================================
来源：http://www.blog.zdbjq.cn/Article/details/glasxmhwo.sHtML

A. 基础语法与类型
来源：http://www.blog.hesvh.cn/Article/details/ggpvuvqod.sHtML

================================================================================
来源：http://blog.hesvh.cn/Article/details/gummjmraa.sHtML

[A01] Hello World
来源：http://www.blog.zdbjq.cn/Article/details/gtjckfupj.sHtML

Py:   print("Hello, World!")
来源：http://www.share.fehbvm.com/Article/details/gzvbuqudv.sHtML

PHP:  echo "Hello, World!";
来源：http://blog.hesvh.cn/Article/details/gmabrxxdf.sHtML

JS:   console.log("Hello, World!");
来源：http://www.share.zdbjq.cn/Article/details/gyubdgtrg.sHtML

TS:   const msg: string = "Hello, World!"; console.log(msg);
来源：http://blog.zdbjq.cn/Article/details/gnbdmhauk.sHtML


<!-- 参考信息 -->