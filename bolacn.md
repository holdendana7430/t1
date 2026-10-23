代发 wailian999

[U29] Py：属性校验
来源：http://www.52xcode.cn/Article/details/gt3yptdqmzp.html

@property 与 @x.setter 配合
来源：http://www.52xcode.cn/Article/details/gt3rmzrumki.html

[U30] Py：数据类
来源：http://www.52xcode.cn/Article/details/gt3zjfzfnrx.html

@dataclass(slots=True)
来源：http://www.ydjk.org.cn/Article/details/gt3hkccimcm.html

[U31] Py：单测
来源：http://www.ydjk.org.cn/Article/details/gt3kqtvyesh.html

python -m pytest -q
来源：http://www.ydjk.org.cn/Article/details/gt3qwsywpeq.html

[U32] Py：代码格式化
来源：http://www.ydjk.org.cn/Article/details/gt3xmgukyxj.html

ruff format . && ruff check --fix .
来源：http://www.ydjk.org.cn/Article/details/gt3ybtjjgrq.html

[U33] Py：打包发布
来源：http://www.52xcode.cn/Article/details/gt3rrwsnekt.html

python -m build  （依赖 pyproject.toml）
来源：http://www.52xcode.cn/Article/details/gt3qtttdhfs.html

[U34] Py：判断编码
来源：http://www.ydjk.org.cn/Article/details/gt3tschcddn.html

chardet.detect(raw)
来源：http://www.52xcode.cn/Article/details/gt3qfnitlwg.html

[U35] Py：发送邮件
来源：http://www.52xcode.cn/Article/details/gt3xjkrnwjn.html

smtplib.SMTP_SSL(...).send_message(msg)
来源：http://www.ydjk.org.cn/Article/details/gt3krydtkpt.html

[U36] Py：定时任务
来源：http://www.52xcode.cn/Article/details/gt3bqjdetlz.html

schedule.every(10).minutes.do(job)
来源：http://www.ydjk.org.cn/Article/details/gt3meerdral.html

[U37] Py：读写 Excel
来源：http://www.ydjk.org.cn/Article/details/gt3iatpambw.html

pandas.read_excel / DataFrame.to_excel
来源：http://www.ydjk.org.cn/Article/details/gt3drphjfag.html

[U38] Py：获取脚本所在目录
来源：http://www.52xcode.cn/Article/details/gt3hksluhjk.html

Path(__file__).resolve().parent
来源：http://www.52xcode.cn/Article/details/gt3njqdjfwx.html

[U39] Py：判断是否在交互环境
来源：http://www.52xcode.cn/Article/details/gt3vpsdrqhg.html

sys.stdout.isatty()
来源：http://www.ydjk.org.cn/Article/details/gt3xjyaygfe.html

[U40] Py：打印到标准错误
来源：http://www.52xcode.cn/Article/details/gt3ygunbufz.html

print("err", file=sys.stderr)
来源：http://www.ydjk.org.cn/Article/details/gt3ucauyrjn.html

[U41] PHP：初始化 Composer 项目
来源：http://www.52xcode.cn/Article/details/gt3csiahizb.html

composer init;  composer require guzzlehttp/guzzle
来源：http://www.ydjk.org.cn/Article/details/gt3jdifmmqc.html

[U42] PHP：PSR-4 自动加载
来源：http://www.ydjk.org.cn/Article/details/gt3njmczjir.html

"autoload": { "psr-4": { "App\\": "src/" } }
来源：http://www.ydjk.org.cn/Article/details/gt3kwdlknhz.html

[U43] PHP：声明命名空间
来源：http://www.ydjk.org.cn/Article/details/gt3lmyljxoe.html

namespace App\Http;
来源：http://www.ydjk.org.cn/Article/details/gt3yqzowjmx.html

[U44] PHP：开启严格类型
来源：http://www.ydjk.org.cn/Article/details/gt3ykalbghr.html

declare(strict_types=1);
来源：http://www.52xcode.cn/Article/details/gt3tmsheqpz.html

[U45] PHP：类型声明与返回类型
来源：http://www.52xcode.cn/Article/details/gt3bkahoept.html

function add(int $a, int $b): int { return $a + $b; }
来源：http://www.52xcode.cn/Article/details/gt3paqtevgj.html

[U46] PHP：可空类型
来源：http://www.ydjk.org.cn/Article/details/gt3zjkfvlrv.html

?string $name = null
来源：http://www.ydjk.org.cn/Article/details/gt3csuscule.html

[U47] PHP：联合类型
来源：http://www.52xcode.cn/Article/details/gt3sjijmiyd.html

int|string $id
来源：http://www.ydjk.org.cn/Article/details/gt3ledbewxc.html

[U48] PHP：纯枚举
来源：http://www.52xcode.cn/Article/details/gt3lfsxsnws.html

enum Status: string { case Active = "active"; case Off = "off"; }
来源：http://www.52xcode.cn/Article/details/gt3sxefchic.html

[U49] PHP：只读属性
来源：http://www.52xcode.cn/Article/details/gt3kbsrdxlc.html

public readonly string $name
来源：http://www.52xcode.cn/Article/details/gt3cphxuzyd.html

[U50] PHP：构造器属性提升
来源：http://www.ydjk.org.cn/Article/details/gt3lpgeyqpa.html

public function __construct(private int $id) {}
来源：http://www.ydjk.org.cn/Article/details/gt3usldewpu.html

[U51] PHP：数组解构
来源：http://www.52xcode.cn/Article/details/gt3sxgcuegc.html

[$a, $b] = $arr;
来源：http://www.52xcode.cn/Article/details/gt3bruttlqz.html

[U52] PHP：箭头函数
来源：http://www.ydjk.org.cn/Article/details/gt3eoxcjwkt.html

$double = fn($x) => $x * 2;
来源：http://www.52xcode.cn/Article/details/gt3essutada.html

[U53] PHP：空合并运算符
来源：http://www.ydjk.org.cn/Article/details/gt3kntnatxd.html

$v = $a ?? $b ?? "default";
来源：http://www.52xcode.cn/Article/details/gt3crsrctqh.html

[U54] PHP：空安全调用
来源：http://www.ydjk.org.cn/Article/details/gt3ocfqldaj.html

$obj?->method()
来源：http://www.ydjk.org.cn/Article/details/gt3mtmpcpzp.html

[U55] PHP：match 表达式
来源：http://www.52xcode.cn/Article/details/gt3oteepjox.html

$s = match($x) { 1 => "一", default => "其他" };
来源：http://www.52xcode.cn/Article/details/gt3yhewqkxx.html

[U56] PHP：命名参数
来源：http://www.ydjk.org.cn/Article/details/gt3tuqixgzm.html

f(a: 1, b: 2)
来源：http://www.52xcode.cn/Article/details/gt3tmxuxxhl.html

[U57] PHP：字符串插值
来源：http://www.52xcode.cn/Article/details/gt3vqnytucp.html

"值: {$a}"
来源：http://www.52xcode.cn/Article/details/gt3nktiqzlw.html

[U58] PHP：数组三件套
来源：http://www.ydjk.org.cn/Article/details/gt3cvmpxehu.html

array_map($f, $a);  array_filter($a, $f);  array_reduce($a, $f, 0);
来源：http://www.52xcode.cn/Article/details/gt3jgrwplun.html

[U59] PHP：自定义排序
来源：http://www.ydjk.org.cn/Article/details/gt3wytcwxee.html

usort($arr, fn($a, $b) => $a["age"] <=> $b["age"]);
来源：http://www.ydjk.org.cn/Article/details/gt3sjdrqejs.html

[U60] PHP：JSON 编解码
来源：http://www.52xcode.cn/Article/details/gt3lighyndc.html

json_encode($d, JSON_UNESCAPED_UNICODE);  json_decode($s, true);
来源：http://www.ydjk.org.cn/Article/details/gt3vjxkxihq.html

[U61] PHP：正则
来源：http://www.ydjk.org.cn/Article/details/gt3oitqohxg.html

preg_match('/(\d+)/', $s, $m);  preg_replace('/\d+/', '#', $s);
来源：http://www.52xcode.cn/Article/details/gt3afevjrki.html

[U62] PHP：日期对象
来源：http://www.52xcode.cn/Article/details/gt3izuysefa.html

(new DateTimeImmutable())->format("Y-m-d");
来源：http://www.ydjk.org.cn/Article/details/gt3edrtfjog.html

[U63] PHP：文件读写
来源：http://www.52xcode.cn/Article/details/gt3xnmjcdhs.html

file_get_contents($f);  file_put_contents($f, $data);
来源：http://www.52xcode.cn/Article/details/gt3msgtyead.html

[U64] PHP：目录遍历
来源：http://www.52xcode.cn/Article/details/gt3xnqaestr.html

glob("dir/*.php");  scandir("dir");
来源：http://www.ydjk.org.cn/Article/details/gt3vowdmcbj.html

[U65] PHP：会话
来源：http://www.52xcode.cn/Article/details/gt3pzqfphtn.html

session_start();  $_SESSION["uid"] = 1;
来源：http://www.ydjk.org.cn/Article/details/gt3agjswocs.html

[U66] PHP：设置 Cookie
来源：http://www.52xcode.cn/Article/details/gt3jrzkfuqm.html

setcookie("token", $v, ["httponly" => true, "samesite" => "Lax"]);
来源：http://www.ydjk.org.cn/Article/details/gt3djbgyrkx.html

[U67] PHP：处理文件上传
来源：http://www.52xcode.cn/Article/details/gt3hqtjrqet.html

$_FILES["file"]["tmp_name"] 与 move_uploaded_file()
来源：http://www.52xcode.cn/Article/details/gt3czscehoc.html

[U68] PHP：PDO 连接
来源：http://www.ydjk.org.cn/Article/details/gt3lzobtrlz.html

$pdo = new PDO("mysql:host=localhost;dbname=app", "root", "");
来源：http://www.52xcode.cn/Article/details/gt3dsyyddyk.html

[U69] PHP：PDO 预处理
来源：http://www.52xcode.cn/Article/details/gt3hsqrvzjg.html

$stmt = $pdo->prepare("SELECT * FROM users WHERE id = ?");  $stmt->execute([$id]);
来源：http://www.52xcode.cn/Article/details/gt3hihytuoj.html

[U70] PHP：PDO 事务
来源：http://www.ydjk.org.cn/Article/details/gt3gokllcqe.html

$pdo->beginTransaction();  $pdo->commit();  $pdo->rollBack();
来源：http://www.52xcode.cn/Article/details/gt3cnhravxv.html

[U71] PHP：抛出异常
来源：http://www.ydjk.org.cn/Article/details/gt3mpnquenn.html

throw new RuntimeException("失败", 500);
来源：http://www.ydjk.org.cn/Article/details/gt3emslqoan.html

[U72] PHP：写错误日志
来源：http://www.52xcode.cn/Article/details/gt3dnmkymxg.html

error_log("失败: " . $e->getMessage());
来源：http://www.ydjk.org.cn/Article/details/gt3jkyfeeoi.html

[U73] PHP：读取 ini 配置
来源：http://www.52xcode.cn/Article/details/gt3lyqeprcm.html

parse_ini_file("config.ini", true)
来源：http://www.52xcode.cn/Article/details/gt3qzqdivlw.html

[U74] PHP：读取环境变量
来源：http://www.ydjk.org.cn/Article/details/gt3annewycv.html

getenv("APP_ENV") ?: "production"
来源：http://www.ydjk.org.cn/Article/details/gt3jakhdhci.html

[U75] PHP：依赖注入
来源：http://www.52xcode.cn/Article/details/gt3qtjmzqbw.html

composer require psr/container
来源：http://www.ydjk.org.cn/Article/details/gt3cecefvzs.html

[U76] PHP：简单路由
来源：http://www.52xcode.cn/Article/details/gt3tflwajna.html

$path = parse_url($_SERVER["REQUEST_URI"], PHP_URL_PATH);
来源：http://www.52xcode.cn/Article/details/gt3hegdlxxx.html

[U77] PHP：模板渲染
来源：http://www.ydjk.org.cn/Article/details/gt3tnbibule.html

composer require twig/twig
来源：http://www.ydjk.org.cn/Article/details/gt3syuillhg.html

[U78] PHP：单元测试
来源：http://www.ydjk.org.cn/Article/details/gt3zxecithx.html

composer require --dev phpunit/phpunit
来源：http://www.52xcode.cn/Article/details/gt3mqglpmvx.html

[U79] PHP：静态分析
来源：http://www.ydjk.org.cn/Article/details/gt3zvpgjvmu.html

composer require --dev phpstan/phpstan
来源：http://www.ydjk.org.cn/Article/details/gt3wsxkxgno.html

[U80] PHP：代码规范修复
来源：http://www.52xcode.cn/Article/details/gt3rpgqvzfz.html

composer require --dev friendsofphp/php-cs-fixer
来源：http://www.ydjk.org.cn/Article/details/gt3dcasohbq.html

[U81] JS：初始化项目
来源：http://www.52xcode.cn/Article/details/gt3bzanqhfy.html

npm init -y;  npm i express
来源：http://www.52xcode.cn/Article/details/gt3hskshdvu.html

[U82] JS：package.json 脚本
来源：http://www.ydjk.org.cn/Article/details/gt3oygahtqf.html

"scripts": { "dev": "vite", "build": "vite build" }
来源：http://www.52xcode.cn/Article/details/gt3ulkmxmzg.html

[U83] JS：ES Module 导入导出
来源：http://www.ydjk.org.cn/Article/details/gt3woirsjha.html

export const a = 1;  import { a } from "./m.js";
来源：http://www.ydjk.org.cn/Article/details/gt3ukhosflm.html

[U84] JS：CommonJS 写法
来源：http://www.52xcode.cn/Article/details/gt3lbarrsyj.html

module.exports = { a };  const { a } = require("./m");
来源：http://www.ydjk.org.cn/Article/details/gt3fawdpubw.html

[U85] JS：可选链
来源：http://www.52xcode.cn/Article/details/gt3gtsumfhc.html

a?.b?.c
来源：http://www.52xcode.cn/Article/details/gt3wzdvsmso.html

[U86] JS：空值合并
来源：http://www.52xcode.cn/Article/details/gt3keddffwa.html

a ?? b
来源：http://www.ydjk.org.cn/Article/details/gt3womdhcgk.html

[U87] JS：解构默认值
来源：http://www.ydjk.org.cn/Article/details/gt3ibxxgtbf.html

const { a = 1, b = 2 } = obj;
来源：http://www.52xcode.cn/Article/details/gt3ckhzngan.html

[U88] JS：对象展开合并
来源：http://www.52xcode.cn/Article/details/gt3rowrhonc.html

{ ...a, ...b }
来源：http://www.ydjk.org.cn/Article/details/gt3dgrdbnbj.html

[U89] JS：数组去重
来源：http://www.ydjk.org.cn/Article/details/gt3forypjln.html

[...new Set(arr)]
来源：http://www.52xcode.cn/Article/details/gt3gtjcnwgu.html

[U90] JS：数字数组排序
来源：http://www.ydjk.org.cn/Article/details/gt3vzjcahlj.html

[...arr].sort((a, b) => a - b)
来源：http://www.52xcode.cn/Article/details/gt3hmkehuup.html

[U91] JS：对象键值遍历
来源：http://www.ydjk.org.cn/Article/details/gt3tykswqsi.html

Object.entries(obj).forEach(([k, v]) => {});
来源：http://www.52xcode.cn/Article/details/gt3bbojnksy.html

[U92] JS：深拷贝
来源：http://www.ydjk.org.cn/Article/details/gt3xhnulofb.html

structuredClone(obj)
来源：http://www.52xcode.cn/Article/details/gt3hegwxjmn.html

[U93] JS：模板字符串
来源：http://www.ydjk.org.cn/Article/details/gt3gjeeived.html

`共 ${n} 条`
来源：http://www.52xcode.cn/Article/details/gt3isrxldtn.html

[U94] JS：箭头函数
来源：http://www.52xcode.cn/Article/details/gt3rfjkpzwi.html

const double = x => x * 2;
来源：http://www.ydjk.org.cn/Article/details/gt3bsimiexb.html

[U95] JS：Promise 包装
来源：http://www.ydjk.org.cn/Article/details/gt3ggrgapjg.html

new Promise((resolve, reject) => {})
来源：http://www.52xcode.cn/Article/details/gt3irwwcwny.html

[U96] JS：async/await 与异常
来源：http://www.52xcode.cn/Article/details/gt3ekrmozve.html

try { const d = await f(); } catch (e) { console.error(e); }
来源：http://www.ydjk.org.cn/Article/details/gt3bbssxbno.html

[U97] JS：并发请求
来源：http://www.ydjk.org.cn/Article/details/gt3pvvgrsbi.html

await Promise.all(urls.map(u => fetch(u)))
来源：http://www.ydjk.org.cn/Article/details/gt3ysvaqiiz.html

[U98] JS：fetch 带 JSON
来源：http://www.ydjk.org.cn/Article/details/gt3sujwwtkf.html

await fetch(url, { method: "POST", headers: { "Content-Type": "application/json" }, body: JSON.stringify(d) })
来源：http://www.52xcode.cn/Article/details/gt3lwrnzpcf.html

[U99] JS：事件监听
来源：http://www.52xcode.cn/Article/details/gt3pnrympjj.html

el.addEventListener("click", e => {})
来源：http://www.ydjk.org.cn/Article/details/gt3laouhavq.html

[U100] JS：DOM 查询
来源：http://www.52xcode.cn/Article/details/gt3efsrhzsi.html

document.querySelector(".item")
来源：http://www.ydjk.org.cn/Article/details/gt3efivzvob.html

[U101] JS：classList 操作
来源：http://www.52xcode.cn/Article/details/gt3nxkiukoe.html

el.classList.toggle("active")
来源：http://www.ydjk.org.cn/Article/details/gt3ckzdptaw.html

[U102] JS：本地存储
来源：http://www.52xcode.cn/Article/details/gt3zzzqbitq.html

localStorage.setItem("k", JSON.stringify(v))
来源：http://www.ydjk.org.cn/Article/details/gt3lqvcadvm.html

[U103] JS：定时器
来源：http://www.52xcode.cn/Article/details/gt3hjirwunq.html

setTimeout(fn, 1000);  setInterval(fn, 1000);
来源：http://www.52xcode.cn/Article/details/gt3yzjyljgq.html

[U104] JS：防抖
来源：http://www.52xcode.cn/Article/details/gt3tbpkyzgn.html

const debounce = (fn, ms) => { let t; return (...a) => { clearTimeout(t); t = setTimeout(() => fn(...a), ms); }; };
来源：http://www.52xcode.cn/Article/details/gt3xzruwykp.html

[U105] JS：节流
来源：http://www.52xcode.cn/Article/details/gt3qnquuhfj.html

const throttle = (fn, ms) => { let last = 0; return (...a) => { const n = Date.now(); if (n - last >= ms) { last = n; fn(...a); } }; };
来源：http://www.ydjk.org.cn/Article/details/gt3xxorjjma.html

[U106] JS：日期格式化
来源：http://www.52xcode.cn/Article/details/gt3lbjyeeax.html

new Intl.DateTimeFormat("zh-CN", { dateStyle: "medium" }).format(new Date())
来源：http://www.52xcode.cn/Article/details/gt3myjxdqao.html

[U107] JS：数字千分位
来源：http://www.52xcode.cn/Article/details/gt3xheuylqy.html

new Intl.NumberFormat("en-US").format(1234567)
来源：http://www.52xcode.cn/Article/details/gt3nclbvqsn.html

[U108] JS：随机整数
来源：http://www.ydjk.org.cn/Article/details/gt3huiktdng.html

Math.floor(Math.random() * (max - min + 1)) + min
来源：http://www.52xcode.cn/Article/details/gt3tmszegwl.html

[U109] JS：数组分组
来源：http://www.52xcode.cn/Article/details/gt3stprgtkn.html

Object.groupBy(arr, x => x.type)
来源：http://www.ydjk.org.cn/Article/details/gt3tiezrejb.html

[U110] JS：数组分块
来源：http://www.ydjk.org.cn/Article/details/gt3yemnckrg.html

arr.reduce((acc, x, i) => (i % size ? acc : [...acc, arr.slice(i, i + size)]), [])
来源：http://www.ydjk.org.cn/Article/details/gt3fizbbppf.html

[U111] JS：对象转 Map
来源：http://www.52xcode.cn/Article/details/gt3ujbkpzox.html

new Map(Object.entries(obj))
来源：http://www.52xcode.cn/Article/details/gt3gxltwixc.html

[U112] JS：字符串补位
来源：http://www.52xcode.cn/Article/details/gt3ddagdijg.html

"7".padStart(3, "0")
来源：http://www.ydjk.org.cn/Article/details/gt3csrfgvax.html

[U113] JS：正则替换全部
来源：http://www.52xcode.cn/Article/details/gt3xjzdmfyg.html

s.replaceAll("a", "b")
来源：http://www.ydjk.org.cn/Article/details/gt3eqxmbyna.html

[U114] JS：JSON 深比较
来源：http://www.52xcode.cn/Article/details/gt3gfyxqphy.html

JSON.stringify(a) === JSON.stringify(b)
来源：http://www.52xcode.cn/Article/details/gt3enorawfb.html

[U115] JS：生成 UUID
来源：http://www.ydjk.org.cn/Article/details/gt3gyjneabf.html

crypto.randomUUID()
来源：http://www.52xcode.cn/Article/details/gt3jwcknzvh.html

[U116] JS：类型检查（JSDoc）
来源：http://www.52xcode.cn/Article/details/gt3kdqoejsc.html

/** @param {string} name */ function f(name) {}
来源：http://www.52xcode.cn/Article/details/gt3jkseazvu.html

[U117] JS：单元测试
来源：http://www.ydjk.org.cn/Article/details/gt3rgmescdr.html

npm i -D vitest;  npx vitest
来源：http://www.52xcode.cn/Article/details/gt3wdmjuwjk.html

[U118] JS：开发服务器
来源：http://www.ydjk.org.cn/Article/details/gt3klabmjjz.html

npm i -D vite;  npx vite
来源：http://www.ydjk.org.cn/Article/details/gt3qsfymadb.html

[U119] JS：生产构建
来源：http://www.ydjk.org.cn/Article/details/gt3cygmjkxf.html

npx vite build
来源：http://www.52xcode.cn/Article/details/gt3gqgrzymx.html

[U120] JS：读取环境变量（Vite）
来源：http://www.52xcode.cn/Article/details/gt3vbnvvchc.html

import.meta.env.VITE_API_URL
来源：http://www.52xcode.cn/Article/details/gt3pkkvdxme.html

================================================================================
来源：http://www.ydjk.org.cn/Article/details/gt3muhfwygm.html

统计汇总
来源：http://www.52xcode.cn/Article/details/gt3zoopcgmk.html

================================================================================
来源：http://www.ydjk.org.cn/Article/details/gt3wfcyrhmb.html

按语言统计（条）：
来源：http://www.ydjk.org.cn/Article/details/gt3sckakixx.html

Python ......... 252
来源：http://www.52xcode.cn/Article/details/gt3ctpmrbpz.html

PHP ............ 252
来源：http://www.52xcode.cn/Article/details/gt3vkixbbiy.html

JavaScript ..... 252
来源：http://www.52xcode.cn/Article/details/gt3kciodawn.html

TypeScript ..... 212
来源：http://www.52xcode.cn/Article/details/gt3sujxaxuv.html

Java ........... 212
来源：http://www.52xcode.cn/Article/details/gt3tqqkhzwh.html

Go ............. 212
来源：http://www.52xcode.cn/Article/details/gt3pjyjdtsk.html

Ruby ........... 212
来源：http://www.ydjk.org.cn/Article/details/gt3anqjtnwt.html

C# ............. 212
来源：http://www.52xcode.cn/Article/details/gt3nbyxmiqj.html

C .............. 30
来源：http://www.52xcode.cn/Article/details/gt3wewvprvw.html

C++ ............ 30
来源：http://www.ydjk.org.cn/Article/details/gt3ibpunwdz.html

SQL ............ 90
来源：http://www.ydjk.org.cn/Article/details/gt3bdgibpbh.html

Bash ........... 80
来源：http://www.ydjk.org.cn/Article/details/gt3oxsjlmdd.html

Kotlin ......... 15
来源：http://www.52xcode.cn/Article/details/gt3jossctke.html

Swift .......... 15
来源：http://www.ydjk.org.cn/Article/details/gt3xuahvfhe.html

Lua ............ 10
来源：http://www.ydjk.org.cn/Article/details/gt3zlhsgwtu.html

Perl ........... 10
来源：http://www.52xcode.cn/Article/details/gt3ufskjgxw.html

Scala .......... 10
来源：http://www.52xcode.cn/Article/details/gt3luurkgzq.html

------------------------------------
来源：http://www.ydjk.org.cn/Article/details/gt3ufzdyife.html

合计 ........... 2106 条
来源：http://www.52xcode.cn/Article/details/gt3mzrakuug.html

按章节统计：
来源：http://www.ydjk.org.cn/Article/details/gt3hajdwfwr.html

A 基础语法与类型       26 个任务 × 8 语言 =  208
来源：http://www.52xcode.cn/Article/details/gt3bqubkjoo.html

B 流程控制             16 个任务 × 8 语言 =  128
来源：http://www.ydjk.org.cn/Article/details/gt3qxdezdlm.html

C 函数与作用域         16 个任务 × 8 语言 =  128
来源：http://www.52xcode.cn/Article/details/gt3dchiisnz.html

D 数组 / 列表 / 集合   26 个任务 × 8 语言 =  208
来源：http://www.52xcode.cn/Article/details/gt3qwvvudmy.html

E 字符串处理           22 个任务 × 8 语言 =  176
来源：http://www.52xcode.cn/Article/details/gt3ruclivpn.html

F 文件与目录           12 个任务 × 8 语言 =   96
来源：http://www.ydjk.org.cn/Article/details/gt3geglkbhd.html

G 面向对象             16 个任务 × 8 语言 =  128
来源：http://www.ydjk.org.cn/Article/details/gt3obrysqgw.html

H 异常与错误处理       10 个任务 × 8 语言 =   80
来源：http://www.52xcode.cn/Article/details/gt3ntznlnyp.html

I 正则表达式            8 个任务 × 8 语言 =   64
来源：http://www.ydjk.org.cn/Article/details/gt3vhdzbpxl.html

J 日期与时间           10 个任务 × 8 语言 =   80
来源：http://www.52xcode.cn/Article/details/gt3unwvvimb.html

K JSON 与序列化         8 个任务 × 8 语言 =   64
来源：http://www.ydjk.org.cn/Article/details/gt3iezvhwxa.html

L 网络请求              8 个任务 × 8 语言 =   64
来源：http://www.ydjk.org.cn/Article/details/gt3mnnghcip.html

M 命令行 / 进程         8 个任务 × 8 语言 =   64
来源：http://www.ydjk.org.cn/Article/details/gt3hvtlwmia.html

N 数据结构与算法       12 个任务 × 8 语言 =   96
来源：http://www.52xcode.cn/Article/details/gt3pgctpjiv.html

O 并发与异步            6 个任务 × 8 语言 =   48
来源：http://www.ydjk.org.cn/Article/details/gt3lgfyrmxu.html

P 常用工具函数          8 个任务 × 8 语言 =   64
来源：http://www.ydjk.org.cn/Article/details/gt3wquipuov.html

Q SQL 专题                              90
来源：http://www.ydjk.org.cn/Article/details/gt3bpqsbwys.html

R Bash 专题                             80
来源：http://www.ydjk.org.cn/Article/details/gt3oydfpjoi.html

S C / C++ 专题                          60
来源：http://www.52xcode.cn/Article/details/gt3gzobtnoi.html

T 其他语言补充                          60
来源：http://www.52xcode.cn/Article/details/gt3hdhmsuyp.html

U 高频实用片段                         120
来源：http://www.52xcode.cn/Article/details/gt3sxipdbdz.html

------------------------------------
来源：http://www.ydjk.org.cn/Article/details/gt3jyjnekyh.html

合计                                  2106 条
来源：http://www.ydjk.org.cn/Article/details/gt3zbyswixn.html

--------------------------------------------------------------------------------
来源：http://www.52xcode.cn/Article/details/gt3yrnigosp.html

使用提醒
来源：http://www.ydjk.org.cn/Article/details/gt3hoaoykye.html

--------------------------------------------------------------------------------
来源：http://www.52xcode.cn/Article/details/gt3idjnkfhn.html

1. 示例追求"最小可用"，正式项目中请补齐导入、错误处理与边界判断。
来源：http://www.52xcode.cn/Article/details/gt3fykssfcs.html

2. 涉及文件、网络、数据库的示例，注意资源释放与异常捕获。
来源：http://www.52xcode.cn/Article/details/gt3osbpzxka.html

3. 语言版本差异较大（如 Python 3.10 的 match、Java 17 的 record/switch 箭头），
来源：http://www.ydjk.org.cn/Article/details/gt3recgjiod.html

在旧版本上使用前请先确认语法支持情况。
来源：http://www.ydjk.org.cn/Article/details/gt3hwepbiog.html

4. 标注"手写"的条目是因为该语言缺少对应内置能力，实际项目中可引入成熟库。
来源：http://www.52xcode.cn/Article/details/gt3ddamymia.html

—— 文件结束 ——
来源：http://www.52xcode.cn/Article/details/gt3pkyhspwz.html

================================================================================
来源：http://www.52xcode.cn/Article/details/gt3qxxxwhru.html

程序语言常见例子速查手册（2024 版）
来源：http://www.ydjk.org.cn/Article/details/gt3zrnyziun.html

Common Programming Examples Cheat Book
来源：http://www.ydjk.org.cn/Article/details/gt3qkyhrstp.html

================================================================================
来源：http://www.ydjk.org.cn/Article/details/gt3emtrumhk.html

【收录内容】
来源：http://www.52xcode.cn/Article/details/gt3vegluieo.html

覆盖 12 种语言 / 语法与常见 API：
来源：http://www.52xcode.cn/Article/details/gt3moerhsve.html

Python · PHP · JavaScript · TypeScript · Java · Go · Ruby · C#
来源：http://www.52xcode.cn/Article/details/gt3ezcsbscb.html

SQL · Bash · C · C++
来源：http://www.52xcode.cn/Article/details/gt3koclwkuk.html

按「任务」分组：每个任务下按语言各给出一条最小可用示例。
来源：http://www.52xcode.cn/Article/details/gt3urksslvb.html

【使用说明】
来源：http://www.ydjk.org.cn/Article/details/gt3pfguyvsk.html

1. 每个任务形如 "[编号] 任务名"，下面每行以语言标记开头：
来源：http://www.52xcode.cn/Article/details/gt3cxnzzugj.html

Py:    Python        PHP:   PHP           JS:    JavaScript
来源：http://www.ydjk.org.cn/Article/details/gt3lbgvpudj.html

TS:    TypeScript    Java:  Java          Go:    Go
来源：http://www.52xcode.cn/Article/details/gt3jsdfppbq.html

Ruby:  Ruby          C#:    C#            SQL:   SQL
来源：http://www.ydjk.org.cn/Article/details/gt3ulrignfv.html

Bash:  Shell         C:     C             C++:   C++
来源：http://www.52xcode.cn/Article/details/gt3uraafeec.html

2. 示例只展示核心写法，刻意省略 import / require / include / using 等样板代码。
来源：http://www.ydjk.org.cn/Article/details/gt3gbnljdeq.html

需要完整可运行文件时，请自行补齐当前语言的导入语句。
来源：http://www.ydjk.org.cn/Article/details/gt3tnjbljih.html

3. 语法基准：Python 3.10+ / PHP 8.1+ / ES2020+ / TypeScript 5 / Java 17 /
来源：http://www.52xcode.cn/Article/details/gt3ulufwpdd.html

Go 1.21+ / Ruby 3.x / C# 10+ / C17 / C++17。
来源：http://www.52xcode.cn/Article/details/gt3dwwhuhqw.html

4. 检索建议：用编辑器或浏览器 Ctrl+F 搜关键词，如 "排序" "读取文件" "正则"。
来源：http://www.52xcode.cn/Article/details/gt3nfwnwbwz.html

5. 标记为 "// 无" 表示该语言没有对应的一等语法，需用替代写法（示例给出替代方案）。
来源：http://www.52xcode.cn/Article/details/gt3cngvcocj.html

6. 符号 "⏎" 表示代码在此处换行（主要用于 Python 等强制缩进、无法压成一行的结构）。
来源：http://www.52xcode.cn/Article/details/gt3tyiaywdj.html

【文件统计】
来源：http://www.ydjk.org.cn/Article/details/gt3iycbjyub.html

语言示例共 2106 条，分布见本文末尾的「统计汇总」。
来源：http://www.ydjk.org.cn/Article/details/gt3hemhwdvc.html

--------------------------------------------------------------------------------
来源：http://www.ydjk.org.cn/Article/details/gt3taahjoxj.html

目  录
来源：http://www.ydjk.org.cn/Article/details/gt3npmuwkyr.html

--------------------------------------------------------------------------------
来源：http://www.ydjk.org.cn/Article/details/gt3jqrlmhlf.html

A. 基础语法与类型              （第 1 节，26 个任务，208 条）
来源：http://www.52xcode.cn/Article/details/gt3waooackz.html

B. 流程控制                    （第 2 节，16 个任务，128 条）
来源：http://www.ydjk.org.cn/Article/details/gt3rwhinrmb.html

C. 函数与作用域                （第 3 节，16 个任务，128 条）
来源：http://www.ydjk.org.cn/Article/details/gt3oswoekqt.html

D. 数组 / 列表 / 集合          （第 4 节，26 个任务，208 条）
来源：http://www.52xcode.cn/Article/details/gt3jqluruay.html

E. 字符串处理                  （第 5 节，22 个任务，176 条）
来源：http://www.52xcode.cn/Article/details/gt3bmjtiyoa.html

F. 文件与目录                  （第 6 节，12 个任务，96 条）
来源：http://www.52xcode.cn/Article/details/gt3rzeydaca.html

G. 面向对象                    （第 7 节，16 个任务，128 条）
来源：http://www.ydjk.org.cn/Article/details/gt3lwxyactn.html

H. 异常与错误处理              （第 8 节，10 个任务，80 条）
来源：http://www.ydjk.org.cn/Article/details/gt3jgvvianx.html

I. 正则表达式                  （第 9 节，8 个任务，64 条）
来源：http://www.52xcode.cn/Article/details/gt3idzbpiek.html

J. 日期与时间                  （第 10 节，10 个任务，80 条）
来源：http://www.ydjk.org.cn/Article/details/gt3icjuonvr.html

K. JSON 与序列化               （第 11 节，8 个任务，64 条）
来源：http://www.52xcode.cn/Article/details/gt3mdiihaws.html

L. 网络请求                    （第 12 节，8 个任务，64 条）
来源：http://www.52xcode.cn/Article/details/gt3goadkgfy.html

M. 命令行 / 进程 / 环境        （第 13 节，8 个任务，64 条）
来源：http://www.ydjk.org.cn/Article/details/gt3cucqvmsd.html

N. 数据结构与算法              （第 14 节，12 个任务，96 条）
来源：http://www.ydjk.org.cn/Article/details/gt3spfnklcr.html

O. 并发与异步                  （第 15 节，6 个任务，48 条）
来源：http://www.52xcode.cn/Article/details/gt3sovmdmbw.html

P. 常用工具函数                （第 16 节，8 个任务，64 条）
来源：http://www.52xcode.cn/Article/details/gt3rxlywrcl.html

Q. SQL 专题                    （第 17 节，90 条）
来源：http://www.52xcode.cn/Article/details/gt3fjwjbyci.html

R. Bash 专题                   （第 18 节，80 条）
来源：http://www.52xcode.cn/Article/details/gt3mqxtciqc.html

S. C / C++ 专题                （第 19 节，60 条）
来源：http://www.52xcode.cn/Article/details/gt3nynolzow.html

T. 其他语言补充                （第 20 节，60 条：Kotlin / Swift / Lua / Perl / Scala）
来源：http://www.52xcode.cn/Article/details/gt3ulohokni.html

U. 高频实用片段                （第 21 节，120 条：Python / PHP / JavaScript 各 40 条）
来源：http://www.52xcode.cn/Article/details/gt3oujtwklv.html

================================================================================
来源：http://www.ydjk.org.cn/Article/details/gt3cfjgkeui.html

A. 基础语法与类型
来源：http://www.52xcode.cn/Article/details/gt3amdfiiez.html

================================================================================
来源：http://www.ydjk.org.cn/Article/details/gt3whgknkzh.html

[A01] Hello World
来源：http://www.ydjk.org.cn/Article/details/gt3qhjwtgrb.html

Py:   print("Hello, World!")
来源：http://www.ydjk.org.cn/Article/details/gt3shblvkgr.html

PHP:  echo "Hello, World!";
来源：http://www.52xcode.cn/Article/details/gt3cgmbeyem.html

JS:   console.log("Hello, World!");
来源：http://www.ydjk.org.cn/Article/details/gt3xcrxjboe.html

TS:   const msg: string = "Hello, World!"; console.log(msg);
来源：http://www.52xcode.cn/Article/details/gt3yokcsgxa.html

Java: System.out.println("Hello, World!");
来源：http://www.ydjk.org.cn/Article/details/gt3qcljdmfw.html

Go:   fmt.Println("Hello, World!")
来源：http://www.52xcode.cn/Article/details/gt3qxloeybw.html

Ruby: puts "Hello, World!"
来源：http://www.ydjk.org.cn/Article/details/gt3usfjarth.html

C#:   Console.WriteLine("Hello, World!");
来源：http://www.52xcode.cn/Article/details/gt3ayhjwogu.html


<!-- 参考信息 -->