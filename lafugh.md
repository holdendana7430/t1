代发 wailian999

[U35] Py：发送邮件
来源：http://www.ydjk.org.cn/Article/details/gt3stttnzms.html

smtplib.SMTP_SSL(...).send_message(msg)
来源：http://www.ydjk.org.cn/Article/details/gt3suecormh.html

[U36] Py：定时任务
来源：http://www.52xcode.cn/Article/details/gt3jbrnujeg.html

schedule.every(10).minutes.do(job)
来源：http://www.52xcode.cn/Article/details/gt3scluglrn.html

[U37] Py：读写 Excel
来源：http://www.ydjk.org.cn/Article/details/gt3admfthbo.html

pandas.read_excel / DataFrame.to_excel
来源：http://www.ydjk.org.cn/Article/details/gt3uqjneysj.html

[U38] Py：获取脚本所在目录
来源：http://www.52xcode.cn/Article/details/gt3sqivqoix.html

Path(__file__).resolve().parent
来源：http://www.ydjk.org.cn/Article/details/gt3figpsimf.html

[U39] Py：判断是否在交互环境
来源：http://www.52xcode.cn/Article/details/gt3htcfmsnw.html

sys.stdout.isatty()
来源：http://www.52xcode.cn/Article/details/gt3juflyamu.html

[U40] Py：打印到标准错误
来源：http://www.ydjk.org.cn/Article/details/gt3uldxkmuq.html

print("err", file=sys.stderr)
来源：http://www.ydjk.org.cn/Article/details/gt3amewdymj.html

[U41] PHP：初始化 Composer 项目
来源：http://www.ydjk.org.cn/Article/details/gt3vanlxavs.html

composer init;  composer require guzzlehttp/guzzle
来源：http://www.52xcode.cn/Article/details/gt3pusoioim.html

[U42] PHP：PSR-4 自动加载
来源：http://www.52xcode.cn/Article/details/gt3rmezybuu.html

"autoload": { "psr-4": { "App\\": "src/" } }
来源：http://www.52xcode.cn/Article/details/gt3okyoymnw.html

[U43] PHP：声明命名空间
来源：http://www.52xcode.cn/Article/details/gt3vxdhteeh.html

namespace App\Http;
来源：http://www.52xcode.cn/Article/details/gt3yaaqcdeg.html

[U44] PHP：开启严格类型
来源：http://www.ydjk.org.cn/Article/details/gt3vriinkik.html

declare(strict_types=1);
来源：http://www.ydjk.org.cn/Article/details/gt3htgqxwbt.html

[U45] PHP：类型声明与返回类型
来源：http://www.ydjk.org.cn/Article/details/gt3bivheebq.html

function add(int $a, int $b): int { return $a + $b; }
来源：http://www.ydjk.org.cn/Article/details/gt3wbfanill.html

[U46] PHP：可空类型
来源：http://www.52xcode.cn/Article/details/gt3pfzwopjv.html

?string $name = null
来源：http://www.52xcode.cn/Article/details/gt3fkhrknew.html

[U47] PHP：联合类型
来源：http://www.52xcode.cn/Article/details/gt3vfdcakhv.html

int|string $id
来源：http://www.ydjk.org.cn/Article/details/gt3tqoworix.html

[U48] PHP：纯枚举
来源：http://www.ydjk.org.cn/Article/details/gt3ymmtonyr.html

enum Status: string { case Active = "active"; case Off = "off"; }
来源：http://www.ydjk.org.cn/Article/details/gt3hbybtaqj.html

[U49] PHP：只读属性
来源：http://www.52xcode.cn/Article/details/gt3hceibquy.html

public readonly string $name
来源：http://www.ydjk.org.cn/Article/details/gt3axyugxuo.html

[U50] PHP：构造器属性提升
来源：http://www.ydjk.org.cn/Article/details/gt3tgpperhm.html

public function __construct(private int $id) {}
来源：http://www.ydjk.org.cn/Article/details/gt3dkjrkisn.html

[U51] PHP：数组解构
来源：http://www.ydjk.org.cn/Article/details/gt3bfldxlvs.html

[$a, $b] = $arr;
来源：http://www.52xcode.cn/Article/details/gt3juoaueho.html

[U52] PHP：箭头函数
来源：http://www.ydjk.org.cn/Article/details/gt3zhfsgtzg.html

$double = fn($x) => $x * 2;
来源：http://www.52xcode.cn/Article/details/gt3bnqvybde.html

[U53] PHP：空合并运算符
来源：http://www.52xcode.cn/Article/details/gt3eotglyog.html

$v = $a ?? $b ?? "default";
来源：http://www.ydjk.org.cn/Article/details/gt3ksktnzkx.html

[U54] PHP：空安全调用
来源：http://www.ydjk.org.cn/Article/details/gt3xrdoswfm.html

$obj?->method()
来源：http://www.ydjk.org.cn/Article/details/gt3igqpvkks.html

[U55] PHP：match 表达式
来源：http://www.52xcode.cn/Article/details/gt3eqlxtxse.html

$s = match($x) { 1 => "一", default => "其他" };
来源：http://www.52xcode.cn/Article/details/gt3uxubsura.html

[U56] PHP：命名参数
来源：http://www.52xcode.cn/Article/details/gt3lgoaeqic.html

f(a: 1, b: 2)
来源：http://www.ydjk.org.cn/Article/details/gt3jsjccpei.html

[U57] PHP：字符串插值
来源：http://www.52xcode.cn/Article/details/gt3nsetwitt.html

"值: {$a}"
来源：http://www.52xcode.cn/Article/details/gt3quabgflf.html

[U58] PHP：数组三件套
来源：http://www.ydjk.org.cn/Article/details/gt3yixbhadt.html

array_map($f, $a);  array_filter($a, $f);  array_reduce($a, $f, 0);
来源：http://www.52xcode.cn/Article/details/gt3kqtunxkb.html

[U59] PHP：自定义排序
来源：http://www.ydjk.org.cn/Article/details/gt3upucvaxh.html

usort($arr, fn($a, $b) => $a["age"] <=> $b["age"]);
来源：http://www.ydjk.org.cn/Article/details/gt3wbzfpquq.html

[U60] PHP：JSON 编解码
来源：http://www.52xcode.cn/Article/details/gt3kcqbgoih.html

json_encode($d, JSON_UNESCAPED_UNICODE);  json_decode($s, true);
来源：http://www.ydjk.org.cn/Article/details/gt3obvsoyik.html

[U61] PHP：正则
来源：http://www.52xcode.cn/Article/details/gt3obfhqzuw.html

preg_match('/(\d+)/', $s, $m);  preg_replace('/\d+/', '#', $s);
来源：http://www.ydjk.org.cn/Article/details/gt3lduenfwd.html

[U62] PHP：日期对象
来源：http://www.ydjk.org.cn/Article/details/gt3flqmhqri.html

(new DateTimeImmutable())->format("Y-m-d");
来源：http://www.ydjk.org.cn/Article/details/gt3bijuwqme.html

[U63] PHP：文件读写
来源：http://www.52xcode.cn/Article/details/gt3jfhrvdrm.html

file_get_contents($f);  file_put_contents($f, $data);
来源：http://www.ydjk.org.cn/Article/details/gt3fkqejenq.html

[U64] PHP：目录遍历
来源：http://www.52xcode.cn/Article/details/gt3hyfoqvhw.html

glob("dir/*.php");  scandir("dir");
来源：http://www.ydjk.org.cn/Article/details/gt3rnhyzhwn.html

[U65] PHP：会话
来源：http://www.ydjk.org.cn/Article/details/gt3hhvggbbv.html

session_start();  $_SESSION["uid"] = 1;
来源：http://www.ydjk.org.cn/Article/details/gt3pqfqawsj.html

[U66] PHP：设置 Cookie
来源：http://www.52xcode.cn/Article/details/gt3xlsykfxc.html

setcookie("token", $v, ["httponly" => true, "samesite" => "Lax"]);
来源：http://www.52xcode.cn/Article/details/gt3sbkxmmwu.html

[U67] PHP：处理文件上传
来源：http://www.ydjk.org.cn/Article/details/gt3qmncsihk.html

$_FILES["file"]["tmp_name"] 与 move_uploaded_file()
来源：http://www.52xcode.cn/Article/details/gt3rhjukqxp.html

[U68] PHP：PDO 连接
来源：http://www.ydjk.org.cn/Article/details/gt3lebgdoye.html

$pdo = new PDO("mysql:host=localhost;dbname=app", "root", "");
来源：http://www.52xcode.cn/Article/details/gt3obqwnqak.html

[U69] PHP：PDO 预处理
来源：http://www.52xcode.cn/Article/details/gt3gbgjwczc.html

$stmt = $pdo->prepare("SELECT * FROM users WHERE id = ?");  $stmt->execute([$id]);
来源：http://www.ydjk.org.cn/Article/details/gt3nxjpvrgr.html

[U70] PHP：PDO 事务
来源：http://www.52xcode.cn/Article/details/gt3mjlwgcri.html

$pdo->beginTransaction();  $pdo->commit();  $pdo->rollBack();
来源：http://www.52xcode.cn/Article/details/gt3sttzmcpl.html

[U71] PHP：抛出异常
来源：http://www.ydjk.org.cn/Article/details/gt3muwhdips.html

throw new RuntimeException("失败", 500);
来源：http://www.52xcode.cn/Article/details/gt3vooqzbmc.html

[U72] PHP：写错误日志
来源：http://www.ydjk.org.cn/Article/details/gt3lhznczmy.html

error_log("失败: " . $e->getMessage());
来源：http://www.ydjk.org.cn/Article/details/gt3apkjltnt.html

[U73] PHP：读取 ini 配置
来源：http://www.52xcode.cn/Article/details/gt3aopdwkpb.html

parse_ini_file("config.ini", true)
来源：http://www.ydjk.org.cn/Article/details/gt3wznxtjru.html

[U74] PHP：读取环境变量
来源：http://www.52xcode.cn/Article/details/gt3xemudjfa.html

getenv("APP_ENV") ?: "production"
来源：http://www.52xcode.cn/Article/details/gt3kylvawld.html

[U75] PHP：依赖注入
来源：http://www.52xcode.cn/Article/details/gt3tqmeyuxi.html

composer require psr/container
来源：http://www.ydjk.org.cn/Article/details/gt3lzwppadt.html

[U76] PHP：简单路由
来源：http://www.ydjk.org.cn/Article/details/gt3kxidluuy.html

$path = parse_url($_SERVER["REQUEST_URI"], PHP_URL_PATH);
来源：http://www.52xcode.cn/Article/details/gt3mhkqrezk.html

[U77] PHP：模板渲染
来源：http://www.52xcode.cn/Article/details/gt3qwcfisrk.html

composer require twig/twig
来源：http://www.52xcode.cn/Article/details/gt3uulorqwx.html

[U78] PHP：单元测试
来源：http://www.ydjk.org.cn/Article/details/gt3itlgfsyc.html

composer require --dev phpunit/phpunit
来源：http://www.52xcode.cn/Article/details/gt3lfluisoo.html

[U79] PHP：静态分析
来源：http://www.52xcode.cn/Article/details/gt3ogdqvllq.html

composer require --dev phpstan/phpstan
来源：http://www.52xcode.cn/Article/details/gt3iojngpzb.html

[U80] PHP：代码规范修复
来源：http://www.ydjk.org.cn/Article/details/gt3blnctkix.html

composer require --dev friendsofphp/php-cs-fixer
来源：http://www.ydjk.org.cn/Article/details/gt3xakqvaal.html

[U81] JS：初始化项目
来源：http://www.ydjk.org.cn/Article/details/gt3hcykvjpk.html

npm init -y;  npm i express
来源：http://www.ydjk.org.cn/Article/details/gt3miligkby.html

[U82] JS：package.json 脚本
来源：http://www.ydjk.org.cn/Article/details/gt3ylfpqugz.html

"scripts": { "dev": "vite", "build": "vite build" }
来源：http://www.ydjk.org.cn/Article/details/gt3mptnngni.html

[U83] JS：ES Module 导入导出
来源：http://www.52xcode.cn/Article/details/gt3riukmjzs.html

export const a = 1;  import { a } from "./m.js";
来源：http://www.ydjk.org.cn/Article/details/gt3kcnqtfbz.html

[U84] JS：CommonJS 写法
来源：http://www.52xcode.cn/Article/details/gt3atrtgfpb.html

module.exports = { a };  const { a } = require("./m");
来源：http://www.ydjk.org.cn/Article/details/gt3maslmfnm.html

[U85] JS：可选链
来源：http://www.ydjk.org.cn/Article/details/gt3zqqieurk.html

a?.b?.c
来源：http://www.ydjk.org.cn/Article/details/gt3vfsnfouo.html

[U86] JS：空值合并
来源：http://www.ydjk.org.cn/Article/details/gt3lptigrwa.html

a ?? b
来源：http://www.ydjk.org.cn/Article/details/gt3saacodlu.html

[U87] JS：解构默认值
来源：http://www.52xcode.cn/Article/details/gt3teaxmfil.html

const { a = 1, b = 2 } = obj;
来源：http://www.52xcode.cn/Article/details/gt3fixrdqoz.html

[U88] JS：对象展开合并
来源：http://www.ydjk.org.cn/Article/details/gt3ehybntnu.html

{ ...a, ...b }
来源：http://www.52xcode.cn/Article/details/gt3cepofthk.html

[U89] JS：数组去重
来源：http://www.52xcode.cn/Article/details/gt3pqetcixz.html

[...new Set(arr)]
来源：http://www.ydjk.org.cn/Article/details/gt3whwmyifa.html

[U90] JS：数字数组排序
来源：http://www.ydjk.org.cn/Article/details/gt3crycnseu.html

[...arr].sort((a, b) => a - b)
来源：http://www.52xcode.cn/Article/details/gt3tawombtd.html

[U91] JS：对象键值遍历
来源：http://www.ydjk.org.cn/Article/details/gt3bgnovhes.html

Object.entries(obj).forEach(([k, v]) => {});
来源：http://www.52xcode.cn/Article/details/gt3ihqzzdvn.html

[U92] JS：深拷贝
来源：http://www.52xcode.cn/Article/details/gt3svykwgqy.html

structuredClone(obj)
来源：http://www.52xcode.cn/Article/details/gt3tiatajde.html

[U93] JS：模板字符串
来源：http://www.52xcode.cn/Article/details/gt3dcocqrzy.html

`共 ${n} 条`
来源：http://www.ydjk.org.cn/Article/details/gt3zumztagp.html

[U94] JS：箭头函数
来源：http://www.52xcode.cn/Article/details/gt3atsjdlma.html

const double = x => x * 2;
来源：http://www.52xcode.cn/Article/details/gt3dhgkgbar.html

[U95] JS：Promise 包装
来源：http://www.ydjk.org.cn/Article/details/gt3vlnwitbu.html

new Promise((resolve, reject) => {})
来源：http://www.52xcode.cn/Article/details/gt3dtonqsij.html

[U96] JS：async/await 与异常
来源：http://www.ydjk.org.cn/Article/details/gt3yfuauxhn.html

try { const d = await f(); } catch (e) { console.error(e); }
来源：http://www.ydjk.org.cn/Article/details/gt3lnlhsmus.html

[U97] JS：并发请求
来源：http://www.52xcode.cn/Article/details/gt3byogvkro.html

await Promise.all(urls.map(u => fetch(u)))
来源：http://www.ydjk.org.cn/Article/details/gt3dphmhcbk.html

[U98] JS：fetch 带 JSON
来源：http://www.ydjk.org.cn/Article/details/gt3qavrmasj.html

await fetch(url, { method: "POST", headers: { "Content-Type": "application/json" }, body: JSON.stringify(d) })
来源：http://www.52xcode.cn/Article/details/gt3bkdqwwwv.html

[U99] JS：事件监听
来源：http://www.ydjk.org.cn/Article/details/gt3lyzqnghr.html

el.addEventListener("click", e => {})
来源：http://www.ydjk.org.cn/Article/details/gt3issulqok.html

[U100] JS：DOM 查询
来源：http://www.52xcode.cn/Article/details/gt3uekvasbq.html

document.querySelector(".item")
来源：http://www.52xcode.cn/Article/details/gt3szhdfhys.html

[U101] JS：classList 操作
来源：http://www.52xcode.cn/Article/details/gt3hldefyeh.html

el.classList.toggle("active")
来源：http://www.52xcode.cn/Article/details/gt3stygoeln.html

[U102] JS：本地存储
来源：http://www.52xcode.cn/Article/details/gt3ulpobmrk.html

localStorage.setItem("k", JSON.stringify(v))
来源：http://www.ydjk.org.cn/Article/details/gt3yvnuvual.html

[U103] JS：定时器
来源：http://www.52xcode.cn/Article/details/gt3wxjsmtze.html

setTimeout(fn, 1000);  setInterval(fn, 1000);
来源：http://www.ydjk.org.cn/Article/details/gt3wlvvuyyq.html

[U104] JS：防抖
来源：http://www.ydjk.org.cn/Article/details/gt3rxuzuzcl.html

const debounce = (fn, ms) => { let t; return (...a) => { clearTimeout(t); t = setTimeout(() => fn(...a), ms); }; };
来源：http://www.ydjk.org.cn/Article/details/gt3wkvbecyp.html

[U105] JS：节流
来源：http://www.ydjk.org.cn/Article/details/gt3lycoanhk.html

const throttle = (fn, ms) => { let last = 0; return (...a) => { const n = Date.now(); if (n - last >= ms) { last = n; fn(...a); } }; };
来源：http://www.ydjk.org.cn/Article/details/gt3agmdapuu.html

[U106] JS：日期格式化
来源：http://www.ydjk.org.cn/Article/details/gt3nnsavexv.html

new Intl.DateTimeFormat("zh-CN", { dateStyle: "medium" }).format(new Date())
来源：http://www.ydjk.org.cn/Article/details/gt3xhkgcoyf.html

[U107] JS：数字千分位
来源：http://www.ydjk.org.cn/Article/details/gt3hnlshzpb.html

new Intl.NumberFormat("en-US").format(1234567)
来源：http://www.ydjk.org.cn/Article/details/gt3tpwhgkei.html

[U108] JS：随机整数
来源：http://www.ydjk.org.cn/Article/details/gt3imrorojp.html

Math.floor(Math.random() * (max - min + 1)) + min
来源：http://www.ydjk.org.cn/Article/details/gt3cbxzmshl.html

[U109] JS：数组分组
来源：http://www.52xcode.cn/Article/details/gt3hqkeaznr.html

Object.groupBy(arr, x => x.type)
来源：http://www.52xcode.cn/Article/details/gt3hjeystyi.html

[U110] JS：数组分块
来源：http://www.ydjk.org.cn/Article/details/gt3vszkxobm.html

arr.reduce((acc, x, i) => (i % size ? acc : [...acc, arr.slice(i, i + size)]), [])
来源：http://www.52xcode.cn/Article/details/gt3uxygseiu.html

[U111] JS：对象转 Map
来源：http://www.ydjk.org.cn/Article/details/gt3tskashuz.html

new Map(Object.entries(obj))
来源：http://www.52xcode.cn/Article/details/gt3agleubtw.html

[U112] JS：字符串补位
来源：http://www.ydjk.org.cn/Article/details/gt3jqequmjw.html

"7".padStart(3, "0")
来源：http://www.52xcode.cn/Article/details/gt3fjqlzqiq.html

[U113] JS：正则替换全部
来源：http://www.ydjk.org.cn/Article/details/gt3sfzjijif.html

s.replaceAll("a", "b")
来源：http://www.ydjk.org.cn/Article/details/gt3psjntxuo.html

[U114] JS：JSON 深比较
来源：http://www.ydjk.org.cn/Article/details/gt3xlrsrxqp.html

JSON.stringify(a) === JSON.stringify(b)
来源：http://www.52xcode.cn/Article/details/gt3sxdrukyu.html

[U115] JS：生成 UUID
来源：http://www.52xcode.cn/Article/details/gt3rstgfguo.html

crypto.randomUUID()
来源：http://www.ydjk.org.cn/Article/details/gt3cgnjfira.html

[U116] JS：类型检查（JSDoc）
来源：http://www.ydjk.org.cn/Article/details/gt3hlajxxax.html

/** @param {string} name */ function f(name) {}
来源：http://www.ydjk.org.cn/Article/details/gt3akkktgar.html

[U117] JS：单元测试
来源：http://www.52xcode.cn/Article/details/gt3dzpdkior.html

npm i -D vitest;  npx vitest
来源：http://www.ydjk.org.cn/Article/details/gt3xdqevquk.html

[U118] JS：开发服务器
来源：http://www.ydjk.org.cn/Article/details/gt3cneokdmk.html

npm i -D vite;  npx vite
来源：http://www.52xcode.cn/Article/details/gt3mtjfareo.html

[U119] JS：生产构建
来源：http://www.52xcode.cn/Article/details/gt3icqmzoxm.html

npx vite build
来源：http://www.52xcode.cn/Article/details/gt3centofwl.html

[U120] JS：读取环境变量（Vite）
来源：http://www.ydjk.org.cn/Article/details/gt3nmmwiwgz.html

import.meta.env.VITE_API_URL
来源：http://www.ydjk.org.cn/Article/details/gt3vudbpjvq.html

================================================================================
来源：http://www.52xcode.cn/Article/details/gt3qmdctnxb.html

统计汇总
来源：http://www.52xcode.cn/Article/details/gt3ulfgxlga.html

================================================================================
来源：http://www.ydjk.org.cn/Article/details/gt3krfundzq.html

按语言统计（条）：
来源：http://www.52xcode.cn/Article/details/gt3kogxmdtm.html

Python ......... 252
来源：http://www.52xcode.cn/Article/details/gt3mvcnlhyc.html

PHP ............ 252
来源：http://www.ydjk.org.cn/Article/details/gt3byuerzzo.html

JavaScript ..... 252
来源：http://www.52xcode.cn/Article/details/gt3dnqwbaqe.html

TypeScript ..... 212
来源：http://www.ydjk.org.cn/Article/details/gt3hymfjbnk.html

Java ........... 212
来源：http://www.ydjk.org.cn/Article/details/gt3eenbtjnk.html

Go ............. 212
来源：http://www.ydjk.org.cn/Article/details/gt3pmrragej.html

Ruby ........... 212
来源：http://www.52xcode.cn/Article/details/gt3vmbgafsi.html

C# ............. 212
来源：http://www.ydjk.org.cn/Article/details/gt3nosttsnt.html

C .............. 30
来源：http://www.52xcode.cn/Article/details/gt3dhshzfzj.html

C++ ............ 30
来源：http://www.52xcode.cn/Article/details/gt3kvrncmts.html

SQL ............ 90
来源：http://www.52xcode.cn/Article/details/gt3jubdypwf.html

Bash ........... 80
来源：http://www.ydjk.org.cn/Article/details/gt3btzeujne.html

Kotlin ......... 15
来源：http://www.ydjk.org.cn/Article/details/gt3afarenyb.html

Swift .......... 15
来源：http://www.52xcode.cn/Article/details/gt3gfntxskv.html

Lua ............ 10
来源：http://www.52xcode.cn/Article/details/gt3cvvhzdhk.html

Perl ........... 10
来源：http://www.52xcode.cn/Article/details/gt3xyfuxtts.html

Scala .......... 10
来源：http://www.52xcode.cn/Article/details/gt3sbxvdnbq.html

------------------------------------
来源：http://www.ydjk.org.cn/Article/details/gt3nffhoxue.html

合计 ........... 2106 条
来源：http://www.ydjk.org.cn/Article/details/gt3gmrukohm.html

按章节统计：
来源：http://www.ydjk.org.cn/Article/details/gt3jvruchws.html

A 基础语法与类型       26 个任务 × 8 语言 =  208
来源：http://www.52xcode.cn/Article/details/gt3zdoueyfn.html

B 流程控制             16 个任务 × 8 语言 =  128
来源：http://www.52xcode.cn/Article/details/gt3wstxxmxd.html

C 函数与作用域         16 个任务 × 8 语言 =  128
来源：http://www.52xcode.cn/Article/details/gt3nulwrrgi.html

D 数组 / 列表 / 集合   26 个任务 × 8 语言 =  208
来源：http://www.52xcode.cn/Article/details/gt3bxtspvzb.html

E 字符串处理           22 个任务 × 8 语言 =  176
来源：http://www.ydjk.org.cn/Article/details/gt3onncpxyc.html

F 文件与目录           12 个任务 × 8 语言 =   96
来源：http://www.ydjk.org.cn/Article/details/gt3xeawnxja.html

G 面向对象             16 个任务 × 8 语言 =  128
来源：http://www.ydjk.org.cn/Article/details/gt3wetrszts.html

H 异常与错误处理       10 个任务 × 8 语言 =   80
来源：http://www.52xcode.cn/Article/details/gt3vlsnojdn.html

I 正则表达式            8 个任务 × 8 语言 =   64
来源：http://www.52xcode.cn/Article/details/gt3hvqfqoxa.html

J 日期与时间           10 个任务 × 8 语言 =   80
来源：http://www.ydjk.org.cn/Article/details/gt3vibryojj.html

K JSON 与序列化         8 个任务 × 8 语言 =   64
来源：http://www.ydjk.org.cn/Article/details/gt3jhxofycb.html

L 网络请求              8 个任务 × 8 语言 =   64
来源：http://www.ydjk.org.cn/Article/details/gt3fpzizxsw.html

M 命令行 / 进程         8 个任务 × 8 语言 =   64
来源：http://www.52xcode.cn/Article/details/gt3qmsemoqb.html

N 数据结构与算法       12 个任务 × 8 语言 =   96
来源：http://www.ydjk.org.cn/Article/details/gt3eulnmazx.html

O 并发与异步            6 个任务 × 8 语言 =   48
来源：http://www.52xcode.cn/Article/details/gt3mqljjljn.html

P 常用工具函数          8 个任务 × 8 语言 =   64
来源：http://www.ydjk.org.cn/Article/details/gt3smcqnmke.html

Q SQL 专题                              90
来源：http://www.ydjk.org.cn/Article/details/gt3bmztrwno.html

R Bash 专题                             80
来源：http://www.ydjk.org.cn/Article/details/gt3aroymimn.html

S C / C++ 专题                          60
来源：http://www.52xcode.cn/Article/details/gt3hhyzcihq.html

T 其他语言补充                          60
来源：http://www.52xcode.cn/Article/details/gt3jppdmokz.html

U 高频实用片段                         120
来源：http://www.ydjk.org.cn/Article/details/gt3xapztufb.html

------------------------------------
来源：http://www.ydjk.org.cn/Article/details/gt3roahbulq.html

合计                                  2106 条
来源：http://www.52xcode.cn/Article/details/gt3sadeatvv.html

--------------------------------------------------------------------------------
来源：http://www.52xcode.cn/Article/details/gt3ctspsmee.html

使用提醒
来源：http://www.ydjk.org.cn/Article/details/gt3mqakhzls.html

--------------------------------------------------------------------------------
来源：http://www.ydjk.org.cn/Article/details/gt3pccijjfr.html

1. 示例追求"最小可用"，正式项目中请补齐导入、错误处理与边界判断。
来源：http://www.ydjk.org.cn/Article/details/gt3rbxtegpn.html

2. 涉及文件、网络、数据库的示例，注意资源释放与异常捕获。
来源：http://www.52xcode.cn/Article/details/gt3avyllkfc.html

3. 语言版本差异较大（如 Python 3.10 的 match、Java 17 的 record/switch 箭头），
来源：http://www.52xcode.cn/Article/details/gt3mycpwloe.html

在旧版本上使用前请先确认语法支持情况。
来源：http://www.52xcode.cn/Article/details/gt3mvdgyole.html

4. 标注"手写"的条目是因为该语言缺少对应内置能力，实际项目中可引入成熟库。
来源：http://www.ydjk.org.cn/Article/details/gt3arbvross.html

—— 文件结束 ——
来源：http://www.52xcode.cn/Article/details/gt3ezqnjall.html

================================================================================
来源：http://www.ydjk.org.cn/Article/details/gt3rrmnqwlo.html

程序语言常见例子速查手册（2024 版）
来源：http://www.52xcode.cn/Article/details/gt3pknkmfmn.html

Common Programming Examples Cheat Book
来源：http://www.ydjk.org.cn/Article/details/gt3mddehznx.html

================================================================================
来源：http://www.ydjk.org.cn/Article/details/gt3ixmokksf.html

【收录内容】
来源：http://www.ydjk.org.cn/Article/details/gt3gthmaoqq.html

覆盖 12 种语言 / 语法与常见 API：
来源：http://www.ydjk.org.cn/Article/details/gt3qneuihpj.html

Python · PHP · JavaScript · TypeScript · Java · Go · Ruby · C#
来源：http://www.ydjk.org.cn/Article/details/gt3mapwivor.html

SQL · Bash · C · C++
来源：http://www.ydjk.org.cn/Article/details/gt3omxcgduy.html

按「任务」分组：每个任务下按语言各给出一条最小可用示例。
来源：http://www.52xcode.cn/Article/details/gt3qdegvsyv.html

【使用说明】
来源：http://www.52xcode.cn/Article/details/gt3boovnskm.html

1. 每个任务形如 "[编号] 任务名"，下面每行以语言标记开头：
来源：http://www.52xcode.cn/Article/details/gt3eovolsef.html

Py:    Python        PHP:   PHP           JS:    JavaScript
来源：http://www.ydjk.org.cn/Article/details/gt3vpdpzlyh.html

TS:    TypeScript    Java:  Java          Go:    Go
来源：http://www.ydjk.org.cn/Article/details/gt3tawzcrel.html

Ruby:  Ruby          C#:    C#            SQL:   SQL
来源：http://www.52xcode.cn/Article/details/gt3yuayuwlh.html

Bash:  Shell         C:     C             C++:   C++
来源：http://www.ydjk.org.cn/Article/details/gt3lrqgpkpp.html

2. 示例只展示核心写法，刻意省略 import / require / include / using 等样板代码。
来源：http://www.ydjk.org.cn/Article/details/gt3ofmhxezc.html

需要完整可运行文件时，请自行补齐当前语言的导入语句。
来源：http://www.ydjk.org.cn/Article/details/gt3bpkhirdz.html

3. 语法基准：Python 3.10+ / PHP 8.1+ / ES2020+ / TypeScript 5 / Java 17 /
来源：http://www.ydjk.org.cn/Article/details/gt3boicklga.html

Go 1.21+ / Ruby 3.x / C# 10+ / C17 / C++17。
来源：http://www.52xcode.cn/Article/details/gt3xnmrydka.html

4. 检索建议：用编辑器或浏览器 Ctrl+F 搜关键词，如 "排序" "读取文件" "正则"。
来源：http://www.ydjk.org.cn/Article/details/gt3xzpzgdmn.html

5. 标记为 "// 无" 表示该语言没有对应的一等语法，需用替代写法（示例给出替代方案）。
来源：http://www.52xcode.cn/Article/details/gt3bxgtspxk.html

6. 符号 "⏎" 表示代码在此处换行（主要用于 Python 等强制缩进、无法压成一行的结构）。
来源：http://www.ydjk.org.cn/Article/details/gt3obajxfvn.html

【文件统计】
来源：http://www.52xcode.cn/Article/details/gt3dbkqffwl.html

语言示例共 2106 条，分布见本文末尾的「统计汇总」。
来源：http://www.ydjk.org.cn/Article/details/gt3wyclydsi.html

--------------------------------------------------------------------------------
来源：http://www.52xcode.cn/Article/details/gt3tonqsdkq.html

目  录
来源：http://www.ydjk.org.cn/Article/details/gt3kwxdwgcg.html

--------------------------------------------------------------------------------
来源：http://www.ydjk.org.cn/Article/details/gt3nvgkuiyd.html

A. 基础语法与类型              （第 1 节，26 个任务，208 条）
来源：http://www.ydjk.org.cn/Article/details/gt3oslawqwg.html

B. 流程控制                    （第 2 节，16 个任务，128 条）
来源：http://www.ydjk.org.cn/Article/details/gt3xkilqycy.html

C. 函数与作用域                （第 3 节，16 个任务，128 条）
来源：http://www.ydjk.org.cn/Article/details/gt3xhsredwg.html

D. 数组 / 列表 / 集合          （第 4 节，26 个任务，208 条）
来源：http://www.52xcode.cn/Article/details/gt3glauvefu.html

E. 字符串处理                  （第 5 节，22 个任务，176 条）
来源：http://www.52xcode.cn/Article/details/gt3yyuvhkud.html

F. 文件与目录                  （第 6 节，12 个任务，96 条）
来源：http://www.ydjk.org.cn/Article/details/gt3etjjdihs.html

G. 面向对象                    （第 7 节，16 个任务，128 条）
来源：http://www.52xcode.cn/Article/details/gt3hvtbdzfa.html

H. 异常与错误处理              （第 8 节，10 个任务，80 条）
来源：http://www.52xcode.cn/Article/details/gt3iitlzddt.html

I. 正则表达式                  （第 9 节，8 个任务，64 条）
来源：http://www.ydjk.org.cn/Article/details/gt3ewxytiyw.html

J. 日期与时间                  （第 10 节，10 个任务，80 条）
来源：http://www.ydjk.org.cn/Article/details/gt3bxxsmgdt.html

K. JSON 与序列化               （第 11 节，8 个任务，64 条）
来源：http://www.ydjk.org.cn/Article/details/gt3ycgwltsr.html

L. 网络请求                    （第 12 节，8 个任务，64 条）
来源：http://www.ydjk.org.cn/Article/details/gt3ufdfkvmm.html

M. 命令行 / 进程 / 环境        （第 13 节，8 个任务，64 条）
来源：http://www.52xcode.cn/Article/details/gt3voycrmnm.html

N. 数据结构与算法              （第 14 节，12 个任务，96 条）
来源：http://www.ydjk.org.cn/Article/details/gt3lvcxgyin.html

O. 并发与异步                  （第 15 节，6 个任务，48 条）
来源：http://www.52xcode.cn/Article/details/gt3oudliwlw.html

P. 常用工具函数                （第 16 节，8 个任务，64 条）
来源：http://www.52xcode.cn/Article/details/gt3beinbkod.html

Q. SQL 专题                    （第 17 节，90 条）
来源：http://www.ydjk.org.cn/Article/details/gt3fpvimtpg.html

R. Bash 专题                   （第 18 节，80 条）
来源：http://www.52xcode.cn/Article/details/gt3chkrjirk.html

S. C / C++ 专题                （第 19 节，60 条）
来源：http://www.52xcode.cn/Article/details/gt3wvnzaopw.html

T. 其他语言补充                （第 20 节，60 条：Kotlin / Swift / Lua / Perl / Scala）
来源：http://www.ydjk.org.cn/Article/details/gt3irljujcq.html

U. 高频实用片段                （第 21 节，120 条：Python / PHP / JavaScript 各 40 条）
来源：http://www.ydjk.org.cn/Article/details/gt3zwxskbpm.html

================================================================================
来源：http://www.ydjk.org.cn/Article/details/gt3kmztxoby.html

A. 基础语法与类型
来源：http://www.ydjk.org.cn/Article/details/gt3hcaormid.html

================================================================================
来源：http://www.ydjk.org.cn/Article/details/gt3jihumkyf.html

[A01] Hello World
来源：http://www.52xcode.cn/Article/details/gt3pfgjvpix.html

Py:   print("Hello, World!")
来源：http://www.ydjk.org.cn/Article/details/gt3nlvkbbzv.html

PHP:  echo "Hello, World!";
来源：http://www.52xcode.cn/Article/details/gt3chldqigc.html

JS:   console.log("Hello, World!");
来源：http://www.ydjk.org.cn/Article/details/gt3qirplqod.html

TS:   const msg: string = "Hello, World!"; console.log(msg);
来源：http://www.ydjk.org.cn/Article/details/gt3hvylcwnw.html

Java: System.out.println("Hello, World!");
来源：http://www.ydjk.org.cn/Article/details/gt3lhmiyrpy.html

Go:   fmt.Println("Hello, World!")
来源：http://www.ydjk.org.cn/Article/details/gt3xfvxizid.html

Ruby: puts "Hello, World!"
来源：http://www.ydjk.org.cn/Article/details/gt3kownpvls.html

C#:   Console.WriteLine("Hello, World!");
来源：http://www.52xcode.cn/Article/details/gt3nawbssia.html

[A02] 变量声明与赋值
来源：http://www.ydjk.org.cn/Article/details/gt3dqvsnkir.html

Py:   name = "Alex"; age = 20            # 动态类型，无需声明
来源：http://www.52xcode.cn/Article/details/gt3fnhmvnye.html

PHP:  $name = "Alex"; $age = 20;
来源：http://www.52xcode.cn/Article/details/gt3abeythvr.html

JS:   let name = "Alex"; const age = 20;
来源：http://www.ydjk.org.cn/Article/details/gt3hahseoqa.html

TS:   let name: string = "Alex"; const age: number = 20;
来源：http://www.ydjk.org.cn/Article/details/gt3gfllapxe.html

Java: String name = "Alex"; int age = 20;
来源：http://www.52xcode.cn/Article/details/gt3jvkzwjcg.html

Go:   name := "Alex"; age := 20
来源：http://www.52xcode.cn/Article/details/gt3zqfrjpsf.html

Ruby: name = "Alex"; age = 20
来源：http://www.52xcode.cn/Article/details/gt3jfnvzfqx.html

C#:   string name = "Alex"; int age = 20;
来源：http://www.52xcode.cn/Article/details/gt3zyxcacxj.html

[A03] 常量定义
来源：http://www.52xcode.cn/Article/details/gt3qzhcdrfb.html

Py:   PI = 3.14159                       # 约定全大写，语言不强制
来源：http://www.ydjk.org.cn/Article/details/gt3wesluiuz.html

PHP:  const PI = 3.14159;
来源：http://www.ydjk.org.cn/Article/details/gt3dszsoxig.html


<!-- 参考信息 -->