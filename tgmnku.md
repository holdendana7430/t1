代发 wailian999

[U31] Py：单测
来源：http://www.ydjk.org.cn/Article/details/gt3eyylrvgr.html

python -m pytest -q
来源：http://www.ydjk.org.cn/Article/details/gt3zzxejyil.html

[U32] Py：代码格式化
来源：http://www.52xcode.cn/Article/details/gt3egmdaria.html

ruff format . && ruff check --fix .
来源：http://www.52xcode.cn/Article/details/gt3apjxvrdn.html

[U33] Py：打包发布
来源：http://www.52xcode.cn/Article/details/gt3ipjauafj.html

python -m build  （依赖 pyproject.toml）
来源：http://www.ydjk.org.cn/Article/details/gt3qcdehqgg.html

[U34] Py：判断编码
来源：http://www.52xcode.cn/Article/details/gt3klezyddm.html

chardet.detect(raw)
来源：http://www.ydjk.org.cn/Article/details/gt3elcjvkkt.html

[U35] Py：发送邮件
来源：http://www.ydjk.org.cn/Article/details/gt3bbdbifsy.html

smtplib.SMTP_SSL(...).send_message(msg)
来源：http://www.ydjk.org.cn/Article/details/gt3hucltyzm.html

[U36] Py：定时任务
来源：http://www.ydjk.org.cn/Article/details/gt3nuugwvwi.html

schedule.every(10).minutes.do(job)
来源：http://www.52xcode.cn/Article/details/gt3omoqtzna.html

[U37] Py：读写 Excel
来源：http://www.52xcode.cn/Article/details/gt3bbwizuwj.html

pandas.read_excel / DataFrame.to_excel
来源：http://www.ydjk.org.cn/Article/details/gt3xbtozwau.html

[U38] Py：获取脚本所在目录
来源：http://www.52xcode.cn/Article/details/gt3iwzmarlt.html

Path(__file__).resolve().parent
来源：http://www.ydjk.org.cn/Article/details/gt3nszlmkqq.html

[U39] Py：判断是否在交互环境
来源：http://www.52xcode.cn/Article/details/gt3ivyrzfsp.html

sys.stdout.isatty()
来源：http://www.52xcode.cn/Article/details/gt3biomhkkh.html

[U40] Py：打印到标准错误
来源：http://www.ydjk.org.cn/Article/details/gt3xtbximgt.html

print("err", file=sys.stderr)
来源：http://www.52xcode.cn/Article/details/gt3aejmacuc.html

[U41] PHP：初始化 Composer 项目
来源：http://www.ydjk.org.cn/Article/details/gt3fwtooegq.html

composer init;  composer require guzzlehttp/guzzle
来源：http://www.52xcode.cn/Article/details/gt3qcriruhf.html

[U42] PHP：PSR-4 自动加载
来源：http://www.ydjk.org.cn/Article/details/gt3pkouqprp.html

"autoload": { "psr-4": { "App\\": "src/" } }
来源：http://www.52xcode.cn/Article/details/gt3duselack.html

[U43] PHP：声明命名空间
来源：http://www.ydjk.org.cn/Article/details/gt3quqmpiex.html

namespace App\Http;
来源：http://www.52xcode.cn/Article/details/gt3kbnwcyii.html

[U44] PHP：开启严格类型
来源：http://www.ydjk.org.cn/Article/details/gt3zwgrncht.html

declare(strict_types=1);
来源：http://www.ydjk.org.cn/Article/details/gt3ozcxtvwd.html

[U45] PHP：类型声明与返回类型
来源：http://www.52xcode.cn/Article/details/gt3qnkanpeg.html

function add(int $a, int $b): int { return $a + $b; }
来源：http://www.52xcode.cn/Article/details/gt3jqqhdjzm.html

[U46] PHP：可空类型
来源：http://www.ydjk.org.cn/Article/details/gt3eqqnhcup.html

?string $name = null
来源：http://www.ydjk.org.cn/Article/details/gt3qpfptglv.html

[U47] PHP：联合类型
来源：http://www.52xcode.cn/Article/details/gt3tgoituid.html

int|string $id
来源：http://www.ydjk.org.cn/Article/details/gt3eljrcdbq.html

[U48] PHP：纯枚举
来源：http://www.ydjk.org.cn/Article/details/gt3tedignix.html

enum Status: string { case Active = "active"; case Off = "off"; }
来源：http://www.52xcode.cn/Article/details/gt3upmryilu.html

[U49] PHP：只读属性
来源：http://www.ydjk.org.cn/Article/details/gt3zxudfdjj.html

public readonly string $name
来源：http://www.52xcode.cn/Article/details/gt3ctpzdqkj.html

[U50] PHP：构造器属性提升
来源：http://www.ydjk.org.cn/Article/details/gt3ptrxdhmg.html

public function __construct(private int $id) {}
来源：http://www.52xcode.cn/Article/details/gt3shhrzagy.html

[U51] PHP：数组解构
来源：http://www.ydjk.org.cn/Article/details/gt3voajbuif.html

[$a, $b] = $arr;
来源：http://www.52xcode.cn/Article/details/gt3ydpobicd.html

[U52] PHP：箭头函数
来源：http://www.ydjk.org.cn/Article/details/gt3bovjvpql.html

$double = fn($x) => $x * 2;
来源：http://www.ydjk.org.cn/Article/details/gt3rbiyuokz.html

[U53] PHP：空合并运算符
来源：http://www.52xcode.cn/Article/details/gt3chizekdr.html

$v = $a ?? $b ?? "default";
来源：http://www.ydjk.org.cn/Article/details/gt3avwbfxyr.html

[U54] PHP：空安全调用
来源：http://www.52xcode.cn/Article/details/gt3uoakjbya.html

$obj?->method()
来源：http://www.ydjk.org.cn/Article/details/gt3oskiblub.html

[U55] PHP：match 表达式
来源：http://www.52xcode.cn/Article/details/gt3vrgerwqo.html

$s = match($x) { 1 => "一", default => "其他" };
来源：http://www.52xcode.cn/Article/details/gt3etpgiwke.html

[U56] PHP：命名参数
来源：http://www.ydjk.org.cn/Article/details/gt3awceiqrx.html

f(a: 1, b: 2)
来源：http://www.ydjk.org.cn/Article/details/gt3iffrbqju.html

[U57] PHP：字符串插值
来源：http://www.52xcode.cn/Article/details/gt3xicwpxnb.html

"值: {$a}"
来源：http://www.ydjk.org.cn/Article/details/gt3swamazct.html

[U58] PHP：数组三件套
来源：http://www.ydjk.org.cn/Article/details/gt3otutlrse.html

array_map($f, $a);  array_filter($a, $f);  array_reduce($a, $f, 0);
来源：http://www.52xcode.cn/Article/details/gt3ymhjhtxr.html

[U59] PHP：自定义排序
来源：http://www.52xcode.cn/Article/details/gt3cnvutmis.html

usort($arr, fn($a, $b) => $a["age"] <=> $b["age"]);
来源：http://www.52xcode.cn/Article/details/gt3fgytytza.html

[U60] PHP：JSON 编解码
来源：http://www.52xcode.cn/Article/details/gt3ctvamghc.html

json_encode($d, JSON_UNESCAPED_UNICODE);  json_decode($s, true);
来源：http://www.52xcode.cn/Article/details/gt3vxehiyrr.html

[U61] PHP：正则
来源：http://www.ydjk.org.cn/Article/details/gt3jzdhqaor.html

preg_match('/(\d+)/', $s, $m);  preg_replace('/\d+/', '#', $s);
来源：http://www.52xcode.cn/Article/details/gt3bdkguurh.html

[U62] PHP：日期对象
来源：http://www.ydjk.org.cn/Article/details/gt3jbmycknq.html

(new DateTimeImmutable())->format("Y-m-d");
来源：http://www.52xcode.cn/Article/details/gt3rvihqxde.html

[U63] PHP：文件读写
来源：http://www.52xcode.cn/Article/details/gt3xqqaxhir.html

file_get_contents($f);  file_put_contents($f, $data);
来源：http://www.ydjk.org.cn/Article/details/gt3teqvnpqo.html

[U64] PHP：目录遍历
来源：http://www.52xcode.cn/Article/details/gt3azyqkcfm.html

glob("dir/*.php");  scandir("dir");
来源：http://www.ydjk.org.cn/Article/details/gt3zdgdqpqr.html

[U65] PHP：会话
来源：http://www.ydjk.org.cn/Article/details/gt3sinckcjp.html

session_start();  $_SESSION["uid"] = 1;
来源：http://www.ydjk.org.cn/Article/details/gt3coihhfze.html

[U66] PHP：设置 Cookie
来源：http://www.ydjk.org.cn/Article/details/gt3mihacdcj.html

setcookie("token", $v, ["httponly" => true, "samesite" => "Lax"]);
来源：http://www.ydjk.org.cn/Article/details/gt3cylwaekd.html

[U67] PHP：处理文件上传
来源：http://www.52xcode.cn/Article/details/gt3tlnwhzzk.html

$_FILES["file"]["tmp_name"] 与 move_uploaded_file()
来源：http://www.ydjk.org.cn/Article/details/gt3yiumscsh.html

[U68] PHP：PDO 连接
来源：http://www.52xcode.cn/Article/details/gt3ildmqsoe.html

$pdo = new PDO("mysql:host=localhost;dbname=app", "root", "");
来源：http://www.52xcode.cn/Article/details/gt3mnwarydg.html

[U69] PHP：PDO 预处理
来源：http://www.52xcode.cn/Article/details/gt3ibjbzius.html

$stmt = $pdo->prepare("SELECT * FROM users WHERE id = ?");  $stmt->execute([$id]);
来源：http://www.52xcode.cn/Article/details/gt3jsaesdmb.html

[U70] PHP：PDO 事务
来源：http://www.ydjk.org.cn/Article/details/gt3icofwyfr.html

$pdo->beginTransaction();  $pdo->commit();  $pdo->rollBack();
来源：http://www.52xcode.cn/Article/details/gt3bqnclzxd.html

[U71] PHP：抛出异常
来源：http://www.52xcode.cn/Article/details/gt3zsmwymku.html

throw new RuntimeException("失败", 500);
来源：http://www.52xcode.cn/Article/details/gt3ksguyexa.html

[U72] PHP：写错误日志
来源：http://www.52xcode.cn/Article/details/gt3sdnprfcc.html

error_log("失败: " . $e->getMessage());
来源：http://www.ydjk.org.cn/Article/details/gt3vznbwvgd.html

[U73] PHP：读取 ini 配置
来源：http://www.ydjk.org.cn/Article/details/gt3ynkmqrga.html

parse_ini_file("config.ini", true)
来源：http://www.ydjk.org.cn/Article/details/gt3ostcatei.html

[U74] PHP：读取环境变量
来源：http://www.52xcode.cn/Article/details/gt3uvqwilyl.html

getenv("APP_ENV") ?: "production"
来源：http://www.ydjk.org.cn/Article/details/gt3wldfytfr.html

[U75] PHP：依赖注入
来源：http://www.ydjk.org.cn/Article/details/gt3mctvrscp.html

composer require psr/container
来源：http://www.52xcode.cn/Article/details/gt3qwqciboa.html

[U76] PHP：简单路由
来源：http://www.52xcode.cn/Article/details/gt3kccyqqqc.html

$path = parse_url($_SERVER["REQUEST_URI"], PHP_URL_PATH);
来源：http://www.ydjk.org.cn/Article/details/gt3faosgzhr.html

[U77] PHP：模板渲染
来源：http://www.52xcode.cn/Article/details/gt3uokrniox.html

composer require twig/twig
来源：http://www.ydjk.org.cn/Article/details/gt3khobdnwi.html

[U78] PHP：单元测试
来源：http://www.52xcode.cn/Article/details/gt3ztultkum.html

composer require --dev phpunit/phpunit
来源：http://www.52xcode.cn/Article/details/gt3pctrsoga.html

[U79] PHP：静态分析
来源：http://www.ydjk.org.cn/Article/details/gt3eicsovtv.html

composer require --dev phpstan/phpstan
来源：http://www.ydjk.org.cn/Article/details/gt3hgamrpjc.html

[U80] PHP：代码规范修复
来源：http://www.ydjk.org.cn/Article/details/gt3eulcgzjb.html

composer require --dev friendsofphp/php-cs-fixer
来源：http://www.ydjk.org.cn/Article/details/gt3fnmzzapj.html

[U81] JS：初始化项目
来源：http://www.52xcode.cn/Article/details/gt3chyhzcsa.html

npm init -y;  npm i express
来源：http://www.52xcode.cn/Article/details/gt3vgigdrng.html

[U82] JS：package.json 脚本
来源：http://www.ydjk.org.cn/Article/details/gt3jfhezpke.html

"scripts": { "dev": "vite", "build": "vite build" }
来源：http://www.52xcode.cn/Article/details/gt3jmkdzdto.html

[U83] JS：ES Module 导入导出
来源：http://www.52xcode.cn/Article/details/gt3glasqjyt.html

export const a = 1;  import { a } from "./m.js";
来源：http://www.ydjk.org.cn/Article/details/gt3plmhtazx.html

[U84] JS：CommonJS 写法
来源：http://www.52xcode.cn/Article/details/gt3mtmrmcmm.html

module.exports = { a };  const { a } = require("./m");
来源：http://www.ydjk.org.cn/Article/details/gt3eqeqkvmm.html

[U85] JS：可选链
来源：http://www.ydjk.org.cn/Article/details/gt3byjkwwqt.html

a?.b?.c
来源：http://www.ydjk.org.cn/Article/details/gt3mfccznsk.html

[U86] JS：空值合并
来源：http://www.52xcode.cn/Article/details/gt3lexjcknq.html

a ?? b
来源：http://www.ydjk.org.cn/Article/details/gt3zzuugmzr.html

[U87] JS：解构默认值
来源：http://www.52xcode.cn/Article/details/gt3zorzydxl.html

const { a = 1, b = 2 } = obj;
来源：http://www.52xcode.cn/Article/details/gt3pyxsrnbq.html

[U88] JS：对象展开合并
来源：http://www.ydjk.org.cn/Article/details/gt3tohlopwp.html

{ ...a, ...b }
来源：http://www.52xcode.cn/Article/details/gt3zquihtpa.html

[U89] JS：数组去重
来源：http://www.ydjk.org.cn/Article/details/gt3ifzspwza.html

[...new Set(arr)]
来源：http://www.52xcode.cn/Article/details/gt3hliqplwb.html

[U90] JS：数字数组排序
来源：http://www.52xcode.cn/Article/details/gt3zshbqvaz.html

[...arr].sort((a, b) => a - b)
来源：http://www.52xcode.cn/Article/details/gt3uyudgnqp.html

[U91] JS：对象键值遍历
来源：http://www.ydjk.org.cn/Article/details/gt3ofkenzzo.html

Object.entries(obj).forEach(([k, v]) => {});
来源：http://www.52xcode.cn/Article/details/gt3xunaoyxc.html

[U92] JS：深拷贝
来源：http://www.52xcode.cn/Article/details/gt3jgnxlmry.html

structuredClone(obj)
来源：http://www.ydjk.org.cn/Article/details/gt3yengjuot.html

[U93] JS：模板字符串
来源：http://www.ydjk.org.cn/Article/details/gt3bxltalys.html

`共 ${n} 条`
来源：http://www.ydjk.org.cn/Article/details/gt3wghepyle.html

[U94] JS：箭头函数
来源：http://www.ydjk.org.cn/Article/details/gt3zeacwfso.html

const double = x => x * 2;
来源：http://www.ydjk.org.cn/Article/details/gt3canjejmm.html

[U95] JS：Promise 包装
来源：http://www.52xcode.cn/Article/details/gt3sbdbfhrg.html

new Promise((resolve, reject) => {})
来源：http://www.52xcode.cn/Article/details/gt3illkugpb.html

[U96] JS：async/await 与异常
来源：http://www.52xcode.cn/Article/details/gt3mlrsmkfo.html

try { const d = await f(); } catch (e) { console.error(e); }
来源：http://www.52xcode.cn/Article/details/gt3htamxiir.html

[U97] JS：并发请求
来源：http://www.ydjk.org.cn/Article/details/gt3dbxaatvj.html

await Promise.all(urls.map(u => fetch(u)))
来源：http://www.ydjk.org.cn/Article/details/gt3lxfonsnd.html

[U98] JS：fetch 带 JSON
来源：http://www.52xcode.cn/Article/details/gt3skiftdvb.html

await fetch(url, { method: "POST", headers: { "Content-Type": "application/json" }, body: JSON.stringify(d) })
来源：http://www.ydjk.org.cn/Article/details/gt3kldtjwza.html

[U99] JS：事件监听
来源：http://www.52xcode.cn/Article/details/gt3wijyyior.html

el.addEventListener("click", e => {})
来源：http://www.52xcode.cn/Article/details/gt3ufixngte.html

[U100] JS：DOM 查询
来源：http://www.ydjk.org.cn/Article/details/gt3bgiwrzzf.html

document.querySelector(".item")
来源：http://www.ydjk.org.cn/Article/details/gt3jevwgzhl.html

[U101] JS：classList 操作
来源：http://www.52xcode.cn/Article/details/gt3faqhkiny.html

el.classList.toggle("active")
来源：http://www.52xcode.cn/Article/details/gt3gnnmbfqu.html

[U102] JS：本地存储
来源：http://www.52xcode.cn/Article/details/gt3jjdznqjb.html

localStorage.setItem("k", JSON.stringify(v))
来源：http://www.ydjk.org.cn/Article/details/gt3vawkfocc.html

[U103] JS：定时器
来源：http://www.ydjk.org.cn/Article/details/gt3lvhpejxf.html

setTimeout(fn, 1000);  setInterval(fn, 1000);
来源：http://www.52xcode.cn/Article/details/gt3dxogcacx.html

[U104] JS：防抖
来源：http://www.ydjk.org.cn/Article/details/gt3wjzgzcuq.html

const debounce = (fn, ms) => { let t; return (...a) => { clearTimeout(t); t = setTimeout(() => fn(...a), ms); }; };
来源：http://www.52xcode.cn/Article/details/gt3tozukses.html

[U105] JS：节流
来源：http://www.52xcode.cn/Article/details/gt3izwltcke.html

const throttle = (fn, ms) => { let last = 0; return (...a) => { const n = Date.now(); if (n - last >= ms) { last = n; fn(...a); } }; };
来源：http://www.ydjk.org.cn/Article/details/gt3ejxkovps.html

[U106] JS：日期格式化
来源：http://www.52xcode.cn/Article/details/gt3daxfqdkq.html

new Intl.DateTimeFormat("zh-CN", { dateStyle: "medium" }).format(new Date())
来源：http://www.52xcode.cn/Article/details/gt3flwsshfg.html

[U107] JS：数字千分位
来源：http://www.ydjk.org.cn/Article/details/gt3raoqyqia.html

new Intl.NumberFormat("en-US").format(1234567)
来源：http://www.ydjk.org.cn/Article/details/gt3izdxdnwx.html

[U108] JS：随机整数
来源：http://www.52xcode.cn/Article/details/gt3zfysyrug.html

Math.floor(Math.random() * (max - min + 1)) + min
来源：http://www.52xcode.cn/Article/details/gt3mfaqtuco.html

[U109] JS：数组分组
来源：http://www.ydjk.org.cn/Article/details/gt3ycwuuiaf.html

Object.groupBy(arr, x => x.type)
来源：http://www.ydjk.org.cn/Article/details/gt3axwzdbca.html

[U110] JS：数组分块
来源：http://www.ydjk.org.cn/Article/details/gt3cfcqoqla.html

arr.reduce((acc, x, i) => (i % size ? acc : [...acc, arr.slice(i, i + size)]), [])
来源：http://www.ydjk.org.cn/Article/details/gt3ozbxckpz.html

[U111] JS：对象转 Map
来源：http://www.52xcode.cn/Article/details/gt3ttghrnqk.html

new Map(Object.entries(obj))
来源：http://www.ydjk.org.cn/Article/details/gt3dfenpbfy.html

[U112] JS：字符串补位
来源：http://www.52xcode.cn/Article/details/gt3srjjeinr.html

"7".padStart(3, "0")
来源：http://www.52xcode.cn/Article/details/gt3mlqyivtm.html

[U113] JS：正则替换全部
来源：http://www.ydjk.org.cn/Article/details/gt3riytckkw.html

s.replaceAll("a", "b")
来源：http://www.ydjk.org.cn/Article/details/gt3xftfbvar.html

[U114] JS：JSON 深比较
来源：http://www.ydjk.org.cn/Article/details/gt3lhlstwcv.html

JSON.stringify(a) === JSON.stringify(b)
来源：http://www.ydjk.org.cn/Article/details/gt3vfywosif.html

[U115] JS：生成 UUID
来源：http://www.52xcode.cn/Article/details/gt3aamnupym.html

crypto.randomUUID()
来源：http://www.52xcode.cn/Article/details/gt3qnjiqghv.html

[U116] JS：类型检查（JSDoc）
来源：http://www.52xcode.cn/Article/details/gt3bqlpomsq.html

/** @param {string} name */ function f(name) {}
来源：http://www.52xcode.cn/Article/details/gt3hhsuxdql.html

[U117] JS：单元测试
来源：http://www.52xcode.cn/Article/details/gt3eiuqmsjf.html

npm i -D vitest;  npx vitest
来源：http://www.52xcode.cn/Article/details/gt3zpxkuukz.html

[U118] JS：开发服务器
来源：http://www.ydjk.org.cn/Article/details/gt3irklqsld.html

npm i -D vite;  npx vite
来源：http://www.52xcode.cn/Article/details/gt3ooldukry.html

[U119] JS：生产构建
来源：http://www.ydjk.org.cn/Article/details/gt3wapckwud.html

npx vite build
来源：http://www.52xcode.cn/Article/details/gt3ganjojyx.html

[U120] JS：读取环境变量（Vite）
来源：http://www.ydjk.org.cn/Article/details/gt3ydfjirou.html

import.meta.env.VITE_API_URL
来源：http://www.52xcode.cn/Article/details/gt3wenbaoar.html

================================================================================
来源：http://www.ydjk.org.cn/Article/details/gt3keoovuvy.html

统计汇总
来源：http://www.ydjk.org.cn/Article/details/gt3wahxqixr.html

================================================================================
来源：http://www.52xcode.cn/Article/details/gt3jkiuiseh.html

按语言统计（条）：
来源：http://www.ydjk.org.cn/Article/details/gt3vbzyntxr.html

Python ......... 252
来源：http://www.52xcode.cn/Article/details/gt3yskfywuh.html

PHP ............ 252
来源：http://www.ydjk.org.cn/Article/details/gt3rpytapxc.html

JavaScript ..... 252
来源：http://www.52xcode.cn/Article/details/gt3twlxqxau.html

TypeScript ..... 212
来源：http://www.52xcode.cn/Article/details/gt3jsyrvepg.html

Java ........... 212
来源：http://www.52xcode.cn/Article/details/gt3eqgpgjbt.html

Go ............. 212
来源：http://www.ydjk.org.cn/Article/details/gt3eywddmxg.html

Ruby ........... 212
来源：http://www.52xcode.cn/Article/details/gt3pmkqmzca.html

C# ............. 212
来源：http://www.ydjk.org.cn/Article/details/gt3zfwyfxjx.html

C .............. 30
来源：http://www.ydjk.org.cn/Article/details/gt3pgtqpnmn.html

C++ ............ 30
来源：http://www.52xcode.cn/Article/details/gt3iuutbhbg.html

SQL ............ 90
来源：http://www.ydjk.org.cn/Article/details/gt3hxkbbywp.html

Bash ........... 80
来源：http://www.ydjk.org.cn/Article/details/gt3nliksxgt.html

Kotlin ......... 15
来源：http://www.ydjk.org.cn/Article/details/gt3iuzxqvip.html

Swift .......... 15
来源：http://www.52xcode.cn/Article/details/gt3glgrfeea.html

Lua ............ 10
来源：http://www.ydjk.org.cn/Article/details/gt3moijrgbm.html

Perl ........... 10
来源：http://www.52xcode.cn/Article/details/gt3rdsgtpxg.html

Scala .......... 10
来源：http://www.ydjk.org.cn/Article/details/gt3lzzmasfn.html

------------------------------------
来源：http://www.ydjk.org.cn/Article/details/gt3yqiwywjt.html

合计 ........... 2106 条
来源：http://www.52xcode.cn/Article/details/gt3afaocooj.html

按章节统计：
来源：http://www.ydjk.org.cn/Article/details/gt3uoqfqlcd.html

A 基础语法与类型       26 个任务 × 8 语言 =  208
来源：http://www.ydjk.org.cn/Article/details/gt3pwncmcfn.html

B 流程控制             16 个任务 × 8 语言 =  128
来源：http://www.ydjk.org.cn/Article/details/gt3cgiwnjgm.html

C 函数与作用域         16 个任务 × 8 语言 =  128
来源：http://www.ydjk.org.cn/Article/details/gt3nsglbrkx.html

D 数组 / 列表 / 集合   26 个任务 × 8 语言 =  208
来源：http://www.52xcode.cn/Article/details/gt3oqincfca.html

E 字符串处理           22 个任务 × 8 语言 =  176
来源：http://www.52xcode.cn/Article/details/gt3wegilbdq.html

F 文件与目录           12 个任务 × 8 语言 =   96
来源：http://www.ydjk.org.cn/Article/details/gt3bbyrkanq.html

G 面向对象             16 个任务 × 8 语言 =  128
来源：http://www.ydjk.org.cn/Article/details/gt3ltfhppbn.html

H 异常与错误处理       10 个任务 × 8 语言 =   80
来源：http://www.ydjk.org.cn/Article/details/gt3nrrrxjsg.html

I 正则表达式            8 个任务 × 8 语言 =   64
来源：http://www.52xcode.cn/Article/details/gt3pztezyaq.html

J 日期与时间           10 个任务 × 8 语言 =   80
来源：http://www.52xcode.cn/Article/details/gt3ehezyqlb.html

K JSON 与序列化         8 个任务 × 8 语言 =   64
来源：http://www.52xcode.cn/Article/details/gt3eyihcjta.html

L 网络请求              8 个任务 × 8 语言 =   64
来源：http://www.52xcode.cn/Article/details/gt3ihjtsuuh.html

M 命令行 / 进程         8 个任务 × 8 语言 =   64
来源：http://www.52xcode.cn/Article/details/gt3nevxyjar.html

N 数据结构与算法       12 个任务 × 8 语言 =   96
来源：http://www.ydjk.org.cn/Article/details/gt3tgbsfqja.html

O 并发与异步            6 个任务 × 8 语言 =   48
来源：http://www.ydjk.org.cn/Article/details/gt3ycmlchah.html

P 常用工具函数          8 个任务 × 8 语言 =   64
来源：http://www.52xcode.cn/Article/details/gt3qpajxfms.html

Q SQL 专题                              90
来源：http://www.ydjk.org.cn/Article/details/gt3hnfwphxm.html

R Bash 专题                             80
来源：http://www.52xcode.cn/Article/details/gt3bxehulzf.html

S C / C++ 专题                          60
来源：http://www.52xcode.cn/Article/details/gt3nvzyajdx.html

T 其他语言补充                          60
来源：http://www.52xcode.cn/Article/details/gt3czoiifnn.html

U 高频实用片段                         120
来源：http://www.ydjk.org.cn/Article/details/gt3zcqgaowr.html

------------------------------------
来源：http://www.52xcode.cn/Article/details/gt3btwzyxax.html

合计                                  2106 条
来源：http://www.ydjk.org.cn/Article/details/gt3dftcivdv.html

--------------------------------------------------------------------------------
来源：http://www.52xcode.cn/Article/details/gt3snotapoe.html

使用提醒
来源：http://www.52xcode.cn/Article/details/gt3nvepdoac.html

--------------------------------------------------------------------------------
来源：http://www.ydjk.org.cn/Article/details/gt3eveilqco.html

1. 示例追求"最小可用"，正式项目中请补齐导入、错误处理与边界判断。
来源：http://www.ydjk.org.cn/Article/details/gt3nxpwkyff.html

2. 涉及文件、网络、数据库的示例，注意资源释放与异常捕获。
来源：http://www.52xcode.cn/Article/details/gt3nhmohxuf.html

3. 语言版本差异较大（如 Python 3.10 的 match、Java 17 的 record/switch 箭头），
来源：http://www.52xcode.cn/Article/details/gt3oxdrmeao.html

在旧版本上使用前请先确认语法支持情况。
来源：http://www.52xcode.cn/Article/details/gt3jazqlyym.html

4. 标注"手写"的条目是因为该语言缺少对应内置能力，实际项目中可引入成熟库。
来源：http://www.ydjk.org.cn/Article/details/gt3jjgrbfhi.html

—— 文件结束 ——
来源：http://www.52xcode.cn/Article/details/gt3vpucfczw.html

================================================================================
来源：http://www.ydjk.org.cn/Article/details/gt3mxvddvzm.html

程序语言常见例子速查手册（2024 版）
来源：http://www.ydjk.org.cn/Article/details/gt3jiqvhllw.html

Common Programming Examples Cheat Book
来源：http://www.52xcode.cn/Article/details/gt3mpdwdgkx.html

================================================================================
来源：http://www.52xcode.cn/Article/details/gt3cjjisblo.html

【收录内容】
来源：http://www.52xcode.cn/Article/details/gt3gpbwggyp.html

覆盖 12 种语言 / 语法与常见 API：
来源：http://www.52xcode.cn/Article/details/gt3kagqvelp.html

Python · PHP · JavaScript · TypeScript · Java · Go · Ruby · C#
来源：http://www.ydjk.org.cn/Article/details/gt3mlboocli.html

SQL · Bash · C · C++
来源：http://www.ydjk.org.cn/Article/details/gt3bmnsypjb.html

按「任务」分组：每个任务下按语言各给出一条最小可用示例。
来源：http://www.ydjk.org.cn/Article/details/gt3yjzwtrqs.html

【使用说明】
来源：http://www.52xcode.cn/Article/details/gt3eslzizob.html

1. 每个任务形如 "[编号] 任务名"，下面每行以语言标记开头：
来源：http://www.52xcode.cn/Article/details/gt3dpdykghi.html

Py:    Python        PHP:   PHP           JS:    JavaScript
来源：http://www.52xcode.cn/Article/details/gt3wjdzfjbi.html

TS:    TypeScript    Java:  Java          Go:    Go
来源：http://www.52xcode.cn/Article/details/gt3zgmxmyfy.html

Ruby:  Ruby          C#:    C#            SQL:   SQL
来源：http://www.52xcode.cn/Article/details/gt3qhbspyyr.html

Bash:  Shell         C:     C             C++:   C++
来源：http://www.ydjk.org.cn/Article/details/gt3gbgtvxpp.html

2. 示例只展示核心写法，刻意省略 import / require / include / using 等样板代码。
来源：http://www.52xcode.cn/Article/details/gt3vqnwiyaj.html

需要完整可运行文件时，请自行补齐当前语言的导入语句。
来源：http://www.52xcode.cn/Article/details/gt3ujzkvckh.html

3. 语法基准：Python 3.10+ / PHP 8.1+ / ES2020+ / TypeScript 5 / Java 17 /
来源：http://www.52xcode.cn/Article/details/gt3ftmyqhwa.html

Go 1.21+ / Ruby 3.x / C# 10+ / C17 / C++17。
来源：http://www.ydjk.org.cn/Article/details/gt3fnmluwrr.html

4. 检索建议：用编辑器或浏览器 Ctrl+F 搜关键词，如 "排序" "读取文件" "正则"。
来源：http://www.ydjk.org.cn/Article/details/gt3phzgwhnk.html

5. 标记为 "// 无" 表示该语言没有对应的一等语法，需用替代写法（示例给出替代方案）。
来源：http://www.52xcode.cn/Article/details/gt3fgdpmhcq.html

6. 符号 "⏎" 表示代码在此处换行（主要用于 Python 等强制缩进、无法压成一行的结构）。
来源：http://www.52xcode.cn/Article/details/gt3sanxssqr.html

【文件统计】
来源：http://www.ydjk.org.cn/Article/details/gt3cfdqcfym.html

语言示例共 2106 条，分布见本文末尾的「统计汇总」。
来源：http://www.52xcode.cn/Article/details/gt3gzdpjlin.html

--------------------------------------------------------------------------------
来源：http://www.ydjk.org.cn/Article/details/gt3hlboqnjo.html

目  录
来源：http://www.52xcode.cn/Article/details/gt3jfawnwqc.html

--------------------------------------------------------------------------------
来源：http://www.52xcode.cn/Article/details/gt3gbochmad.html

A. 基础语法与类型              （第 1 节，26 个任务，208 条）
来源：http://www.ydjk.org.cn/Article/details/gt3unqoojrw.html

B. 流程控制                    （第 2 节，16 个任务，128 条）
来源：http://www.ydjk.org.cn/Article/details/gt3oqajmlel.html

C. 函数与作用域                （第 3 节，16 个任务，128 条）
来源：http://www.52xcode.cn/Article/details/gt3doapcphm.html

D. 数组 / 列表 / 集合          （第 4 节，26 个任务，208 条）
来源：http://www.ydjk.org.cn/Article/details/gt3avqtiaqz.html

E. 字符串处理                  （第 5 节，22 个任务，176 条）
来源：http://www.ydjk.org.cn/Article/details/gt3ecoquivt.html

F. 文件与目录                  （第 6 节，12 个任务，96 条）
来源：http://www.52xcode.cn/Article/details/gt3pqpmijvf.html

G. 面向对象                    （第 7 节，16 个任务，128 条）
来源：http://www.ydjk.org.cn/Article/details/gt3fapaumaw.html

H. 异常与错误处理              （第 8 节，10 个任务，80 条）
来源：http://www.ydjk.org.cn/Article/details/gt3durpawpy.html

I. 正则表达式                  （第 9 节，8 个任务，64 条）
来源：http://www.52xcode.cn/Article/details/gt3meystpka.html

J. 日期与时间                  （第 10 节，10 个任务，80 条）
来源：http://www.52xcode.cn/Article/details/gt3dtgnaetg.html

K. JSON 与序列化               （第 11 节，8 个任务，64 条）
来源：http://www.ydjk.org.cn/Article/details/gt3zpochofj.html

L. 网络请求                    （第 12 节，8 个任务，64 条）
来源：http://www.ydjk.org.cn/Article/details/gt3ruomnqbt.html

M. 命令行 / 进程 / 环境        （第 13 节，8 个任务，64 条）
来源：http://www.ydjk.org.cn/Article/details/gt3hwrjzoqs.html

N. 数据结构与算法              （第 14 节，12 个任务，96 条）
来源：http://www.52xcode.cn/Article/details/gt3eetadzed.html

O. 并发与异步                  （第 15 节，6 个任务，48 条）
来源：http://www.52xcode.cn/Article/details/gt3edschxfc.html

P. 常用工具函数                （第 16 节，8 个任务，64 条）
来源：http://www.52xcode.cn/Article/details/gt3muedxbsj.html

Q. SQL 专题                    （第 17 节，90 条）
来源：http://www.52xcode.cn/Article/details/gt3bcppteme.html

R. Bash 专题                   （第 18 节，80 条）
来源：http://www.ydjk.org.cn/Article/details/gt3zxlygkho.html

S. C / C++ 专题                （第 19 节，60 条）
来源：http://www.52xcode.cn/Article/details/gt3ciirdjkc.html

T. 其他语言补充                （第 20 节，60 条：Kotlin / Swift / Lua / Perl / Scala）
来源：http://www.52xcode.cn/Article/details/gt3nhmaduze.html

U. 高频实用片段                （第 21 节，120 条：Python / PHP / JavaScript 各 40 条）
来源：http://www.ydjk.org.cn/Article/details/gt3jxijfkft.html

================================================================================
来源：http://www.ydjk.org.cn/Article/details/gt3azyobzez.html

A. 基础语法与类型
来源：http://www.52xcode.cn/Article/details/gt3yvtfkvib.html

================================================================================
来源：http://www.ydjk.org.cn/Article/details/gt3pnkcpiem.html

[A01] Hello World
来源：http://www.52xcode.cn/Article/details/gt3qwwdemsv.html

Py:   print("Hello, World!")
来源：http://www.ydjk.org.cn/Article/details/gt3ehhjiufx.html

PHP:  echo "Hello, World!";
来源：http://www.52xcode.cn/Article/details/gt3foprheei.html

JS:   console.log("Hello, World!");
来源：http://www.52xcode.cn/Article/details/gt3gjwbicvq.html

TS:   const msg: string = "Hello, World!"; console.log(msg);
来源：http://www.52xcode.cn/Article/details/gt3rgkfncru.html

Java: System.out.println("Hello, World!");
来源：http://www.ydjk.org.cn/Article/details/gt3icxnrapq.html

Go:   fmt.Println("Hello, World!")
来源：http://www.ydjk.org.cn/Article/details/gt3ooeseozk.html

Ruby: puts "Hello, World!"
来源：http://www.ydjk.org.cn/Article/details/gt3ydlqydir.html

C#:   Console.WriteLine("Hello, World!");
来源：http://www.52xcode.cn/Article/details/gt3oxoajibq.html

[A02] 变量声明与赋值
来源：http://www.52xcode.cn/Article/details/gt3jnoimeyw.html

Py:   name = "Alex"; age = 20            # 动态类型，无需声明
来源：http://www.ydjk.org.cn/Article/details/gt3fjodsvtq.html

PHP:  $name = "Alex"; $age = 20;
来源：http://www.ydjk.org.cn/Article/details/gt3sheqkdmn.html

JS:   let name = "Alex"; const age = 20;
来源：http://www.ydjk.org.cn/Article/details/gt3evdmheij.html


<!-- 参考信息 -->