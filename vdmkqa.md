代发 wailian999

[U35] Py：发送邮件
来源：http://www.ydjk.org.cn/Article/details/gt3kgaeefbe.html

smtplib.SMTP_SSL(...).send_message(msg)
来源：http://www.52xcode.cn/Article/details/gt3zxfzftmn.html

[U36] Py：定时任务
来源：http://www.52xcode.cn/Article/details/gt3ktmhdriv.html

schedule.every(10).minutes.do(job)
来源：http://www.52xcode.cn/Article/details/gt3ypfrpjdx.html

[U37] Py：读写 Excel
来源：http://www.ydjk.org.cn/Article/details/gt3euftthkx.html

pandas.read_excel / DataFrame.to_excel
来源：http://www.52xcode.cn/Article/details/gt3ankjwges.html

[U38] Py：获取脚本所在目录
来源：http://www.52xcode.cn/Article/details/gt3nsgjlgol.html

Path(__file__).resolve().parent
来源：http://www.ydjk.org.cn/Article/details/gt3evrwgrqz.html

[U39] Py：判断是否在交互环境
来源：http://www.ydjk.org.cn/Article/details/gt3asbqixxl.html

sys.stdout.isatty()
来源：http://www.52xcode.cn/Article/details/gt3lokmkfae.html

[U40] Py：打印到标准错误
来源：http://www.52xcode.cn/Article/details/gt3bezzpovc.html

print("err", file=sys.stderr)
来源：http://www.52xcode.cn/Article/details/gt3mtoltxyo.html

[U41] PHP：初始化 Composer 项目
来源：http://www.ydjk.org.cn/Article/details/gt3yadoehvf.html

composer init;  composer require guzzlehttp/guzzle
来源：http://www.ydjk.org.cn/Article/details/gt3qnpzhgwo.html

[U42] PHP：PSR-4 自动加载
来源：http://www.52xcode.cn/Article/details/gt3oeabnkbh.html

"autoload": { "psr-4": { "App\\": "src/" } }
来源：http://www.ydjk.org.cn/Article/details/gt3oqvbtkqc.html

[U43] PHP：声明命名空间
来源：http://www.52xcode.cn/Article/details/gt3dngslmbb.html

namespace App\Http;
来源：http://www.52xcode.cn/Article/details/gt3suxlafex.html

[U44] PHP：开启严格类型
来源：http://www.ydjk.org.cn/Article/details/gt3csrqboin.html

declare(strict_types=1);
来源：http://www.ydjk.org.cn/Article/details/gt3dqsyqbtl.html

[U45] PHP：类型声明与返回类型
来源：http://www.52xcode.cn/Article/details/gt3wtjbarvu.html

function add(int $a, int $b): int { return $a + $b; }
来源：http://www.52xcode.cn/Article/details/gt3tzvjgnlj.html

[U46] PHP：可空类型
来源：http://www.52xcode.cn/Article/details/gt3zjfnfbfh.html

?string $name = null
来源：http://www.52xcode.cn/Article/details/gt3hzgmpqcw.html

[U47] PHP：联合类型
来源：http://www.ydjk.org.cn/Article/details/gt3uacjuluq.html

int|string $id
来源：http://www.52xcode.cn/Article/details/gt3rtnzbkoi.html

[U48] PHP：纯枚举
来源：http://www.52xcode.cn/Article/details/gt3wikhnckl.html

enum Status: string { case Active = "active"; case Off = "off"; }
来源：http://www.ydjk.org.cn/Article/details/gt3yyldqcox.html

[U49] PHP：只读属性
来源：http://www.ydjk.org.cn/Article/details/gt3xyjuvuwl.html

public readonly string $name
来源：http://www.52xcode.cn/Article/details/gt3rttnnsip.html

[U50] PHP：构造器属性提升
来源：http://www.52xcode.cn/Article/details/gt3kuyslqmt.html

public function __construct(private int $id) {}
来源：http://www.52xcode.cn/Article/details/gt3kktophty.html

[U51] PHP：数组解构
来源：http://www.ydjk.org.cn/Article/details/gt3dznyfxvj.html

[$a, $b] = $arr;
来源：http://www.ydjk.org.cn/Article/details/gt3lywgieoe.html

[U52] PHP：箭头函数
来源：http://www.52xcode.cn/Article/details/gt3lkyvherr.html

$double = fn($x) => $x * 2;
来源：http://www.ydjk.org.cn/Article/details/gt3irctxlnh.html

[U53] PHP：空合并运算符
来源：http://www.52xcode.cn/Article/details/gt3jsthooco.html

$v = $a ?? $b ?? "default";
来源：http://www.ydjk.org.cn/Article/details/gt3pizruapn.html

[U54] PHP：空安全调用
来源：http://www.ydjk.org.cn/Article/details/gt3owkuccpw.html

$obj?->method()
来源：http://www.ydjk.org.cn/Article/details/gt3cquafmpt.html

[U55] PHP：match 表达式
来源：http://www.52xcode.cn/Article/details/gt3cgrfmyku.html

$s = match($x) { 1 => "一", default => "其他" };
来源：http://www.ydjk.org.cn/Article/details/gt3fycusgbs.html

[U56] PHP：命名参数
来源：http://www.52xcode.cn/Article/details/gt3mdzgjsce.html

f(a: 1, b: 2)
来源：http://www.52xcode.cn/Article/details/gt3mpeackqd.html

[U57] PHP：字符串插值
来源：http://www.ydjk.org.cn/Article/details/gt3idirpfxq.html

"值: {$a}"
来源：http://www.52xcode.cn/Article/details/gt3uukwsuox.html

[U58] PHP：数组三件套
来源：http://www.ydjk.org.cn/Article/details/gt3eyyrbjiq.html

array_map($f, $a);  array_filter($a, $f);  array_reduce($a, $f, 0);
来源：http://www.ydjk.org.cn/Article/details/gt3zdlapjhb.html

[U59] PHP：自定义排序
来源：http://www.ydjk.org.cn/Article/details/gt3qmsrkyhk.html

usort($arr, fn($a, $b) => $a["age"] <=> $b["age"]);
来源：http://www.ydjk.org.cn/Article/details/gt3pxhdwkfq.html

[U60] PHP：JSON 编解码
来源：http://www.52xcode.cn/Article/details/gt3mcqtqpkw.html

json_encode($d, JSON_UNESCAPED_UNICODE);  json_decode($s, true);
来源：http://www.ydjk.org.cn/Article/details/gt3zvehwnby.html

[U61] PHP：正则
来源：http://www.ydjk.org.cn/Article/details/gt3ybbfkbio.html

preg_match('/(\d+)/', $s, $m);  preg_replace('/\d+/', '#', $s);
来源：http://www.52xcode.cn/Article/details/gt3wyqlklhj.html

[U62] PHP：日期对象
来源：http://www.ydjk.org.cn/Article/details/gt3jerfrbbz.html

(new DateTimeImmutable())->format("Y-m-d");
来源：http://www.ydjk.org.cn/Article/details/gt3snkmhmfy.html

[U63] PHP：文件读写
来源：http://www.ydjk.org.cn/Article/details/gt3vrofzlyc.html

file_get_contents($f);  file_put_contents($f, $data);
来源：http://www.52xcode.cn/Article/details/gt3mtpcynej.html

[U64] PHP：目录遍历
来源：http://www.ydjk.org.cn/Article/details/gt3xrcowprx.html

glob("dir/*.php");  scandir("dir");
来源：http://www.52xcode.cn/Article/details/gt3ysdsrknw.html

[U65] PHP：会话
来源：http://www.ydjk.org.cn/Article/details/gt3lkngvqjk.html

session_start();  $_SESSION["uid"] = 1;
来源：http://www.52xcode.cn/Article/details/gt3dpeffcii.html

[U66] PHP：设置 Cookie
来源：http://www.ydjk.org.cn/Article/details/gt3gizkwhxk.html

setcookie("token", $v, ["httponly" => true, "samesite" => "Lax"]);
来源：http://www.ydjk.org.cn/Article/details/gt3otiqzzan.html

[U67] PHP：处理文件上传
来源：http://www.52xcode.cn/Article/details/gt3pdjgvdto.html

$_FILES["file"]["tmp_name"] 与 move_uploaded_file()
来源：http://www.52xcode.cn/Article/details/gt3qjcemjbf.html

[U68] PHP：PDO 连接
来源：http://www.ydjk.org.cn/Article/details/gt3jtcgcmap.html

$pdo = new PDO("mysql:host=localhost;dbname=app", "root", "");
来源：http://www.52xcode.cn/Article/details/gt3rtebevsm.html

[U69] PHP：PDO 预处理
来源：http://www.52xcode.cn/Article/details/gt3nitdxsnx.html

$stmt = $pdo->prepare("SELECT * FROM users WHERE id = ?");  $stmt->execute([$id]);
来源：http://www.52xcode.cn/Article/details/gt3dvwjcowm.html

[U70] PHP：PDO 事务
来源：http://www.52xcode.cn/Article/details/gt3uzhckwbr.html

$pdo->beginTransaction();  $pdo->commit();  $pdo->rollBack();
来源：http://www.52xcode.cn/Article/details/gt3pipagfeg.html

[U71] PHP：抛出异常
来源：http://www.ydjk.org.cn/Article/details/gt3odujpoey.html

throw new RuntimeException("失败", 500);
来源：http://www.52xcode.cn/Article/details/gt3uifhknfj.html

[U72] PHP：写错误日志
来源：http://www.52xcode.cn/Article/details/gt3iefnvdiw.html

error_log("失败: " . $e->getMessage());
来源：http://www.52xcode.cn/Article/details/gt3nahgxbep.html

[U73] PHP：读取 ini 配置
来源：http://www.ydjk.org.cn/Article/details/gt3xududamc.html

parse_ini_file("config.ini", true)
来源：http://www.52xcode.cn/Article/details/gt3ypunuwqk.html

[U74] PHP：读取环境变量
来源：http://www.ydjk.org.cn/Article/details/gt3klxilnnw.html

getenv("APP_ENV") ?: "production"
来源：http://www.52xcode.cn/Article/details/gt3umkkbsvs.html

[U75] PHP：依赖注入
来源：http://www.ydjk.org.cn/Article/details/gt3inktcpui.html

composer require psr/container
来源：http://www.52xcode.cn/Article/details/gt3uyympfxl.html

[U76] PHP：简单路由
来源：http://www.52xcode.cn/Article/details/gt3qycboipw.html

$path = parse_url($_SERVER["REQUEST_URI"], PHP_URL_PATH);
来源：http://www.ydjk.org.cn/Article/details/gt3dzfkqdkm.html

[U77] PHP：模板渲染
来源：http://www.ydjk.org.cn/Article/details/gt3abtrgcpa.html

composer require twig/twig
来源：http://www.52xcode.cn/Article/details/gt3putrowav.html

[U78] PHP：单元测试
来源：http://www.52xcode.cn/Article/details/gt3repingnz.html

composer require --dev phpunit/phpunit
来源：http://www.ydjk.org.cn/Article/details/gt3ggdjrewh.html

[U79] PHP：静态分析
来源：http://www.ydjk.org.cn/Article/details/gt3kujqwflc.html

composer require --dev phpstan/phpstan
来源：http://www.ydjk.org.cn/Article/details/gt3jwnvyusr.html

[U80] PHP：代码规范修复
来源：http://www.ydjk.org.cn/Article/details/gt3twswolha.html

composer require --dev friendsofphp/php-cs-fixer
来源：http://www.ydjk.org.cn/Article/details/gt3epblvolo.html

[U81] JS：初始化项目
来源：http://www.52xcode.cn/Article/details/gt3dgnptwej.html

npm init -y;  npm i express
来源：http://www.ydjk.org.cn/Article/details/gt3zsiuoctw.html

[U82] JS：package.json 脚本
来源：http://www.ydjk.org.cn/Article/details/gt3yjjghupm.html

"scripts": { "dev": "vite", "build": "vite build" }
来源：http://www.52xcode.cn/Article/details/gt3sdpnuchl.html

[U83] JS：ES Module 导入导出
来源：http://www.52xcode.cn/Article/details/gt3acnutjxk.html

export const a = 1;  import { a } from "./m.js";
来源：http://www.52xcode.cn/Article/details/gt3phwosxxc.html

[U84] JS：CommonJS 写法
来源：http://www.52xcode.cn/Article/details/gt3mxxteilr.html

module.exports = { a };  const { a } = require("./m");
来源：http://www.ydjk.org.cn/Article/details/gt3qtebzkaz.html

[U85] JS：可选链
来源：http://www.52xcode.cn/Article/details/gt3ouhmntpn.html

a?.b?.c
来源：http://www.ydjk.org.cn/Article/details/gt3emuobcfg.html

[U86] JS：空值合并
来源：http://www.ydjk.org.cn/Article/details/gt3chclyvmf.html

a ?? b
来源：http://www.ydjk.org.cn/Article/details/gt3lxrjvvls.html

[U87] JS：解构默认值
来源：http://www.52xcode.cn/Article/details/gt3vblvrapu.html

const { a = 1, b = 2 } = obj;
来源：http://www.ydjk.org.cn/Article/details/gt3dclzbhkb.html

[U88] JS：对象展开合并
来源：http://www.52xcode.cn/Article/details/gt3pnxfebrn.html

{ ...a, ...b }
来源：http://www.52xcode.cn/Article/details/gt3bqvthuly.html

[U89] JS：数组去重
来源：http://www.ydjk.org.cn/Article/details/gt3mkwbajky.html

[...new Set(arr)]
来源：http://www.ydjk.org.cn/Article/details/gt3ssxkbpti.html

[U90] JS：数字数组排序
来源：http://www.ydjk.org.cn/Article/details/gt3likixcgd.html

[...arr].sort((a, b) => a - b)
来源：http://www.52xcode.cn/Article/details/gt3rdqahoxn.html

[U91] JS：对象键值遍历
来源：http://www.ydjk.org.cn/Article/details/gt3jgcbwktj.html

Object.entries(obj).forEach(([k, v]) => {});
来源：http://www.ydjk.org.cn/Article/details/gt3ynzoiyde.html

[U92] JS：深拷贝
来源：http://www.52xcode.cn/Article/details/gt3ryviwzms.html

structuredClone(obj)
来源：http://www.ydjk.org.cn/Article/details/gt3ccaexnzo.html

[U93] JS：模板字符串
来源：http://www.52xcode.cn/Article/details/gt3ojiqjwhk.html

`共 ${n} 条`
来源：http://www.ydjk.org.cn/Article/details/gt3ebjkvuul.html

[U94] JS：箭头函数
来源：http://www.52xcode.cn/Article/details/gt3zwmyykpn.html

const double = x => x * 2;
来源：http://www.ydjk.org.cn/Article/details/gt3wredxqhw.html

[U95] JS：Promise 包装
来源：http://www.52xcode.cn/Article/details/gt3okoxtryo.html

new Promise((resolve, reject) => {})
来源：http://www.ydjk.org.cn/Article/details/gt3ezmwppwh.html

[U96] JS：async/await 与异常
来源：http://www.52xcode.cn/Article/details/gt3pjedleyt.html

try { const d = await f(); } catch (e) { console.error(e); }
来源：http://www.52xcode.cn/Article/details/gt3ioiayujc.html

[U97] JS：并发请求
来源：http://www.52xcode.cn/Article/details/gt3cahkqyfr.html

await Promise.all(urls.map(u => fetch(u)))
来源：http://www.ydjk.org.cn/Article/details/gt3gcggddql.html

[U98] JS：fetch 带 JSON
来源：http://www.ydjk.org.cn/Article/details/gt3wjgswhqh.html

await fetch(url, { method: "POST", headers: { "Content-Type": "application/json" }, body: JSON.stringify(d) })
来源：http://www.52xcode.cn/Article/details/gt3unxymljz.html

[U99] JS：事件监听
来源：http://www.52xcode.cn/Article/details/gt3dmmzexnr.html

el.addEventListener("click", e => {})
来源：http://www.ydjk.org.cn/Article/details/gt3oquxagqe.html

[U100] JS：DOM 查询
来源：http://www.ydjk.org.cn/Article/details/gt3zoaosrlo.html

document.querySelector(".item")
来源：http://www.52xcode.cn/Article/details/gt3rotekegs.html

[U101] JS：classList 操作
来源：http://www.52xcode.cn/Article/details/gt3pjtjgkqp.html

el.classList.toggle("active")
来源：http://www.ydjk.org.cn/Article/details/gt3iahgtumt.html

[U102] JS：本地存储
来源：http://www.ydjk.org.cn/Article/details/gt3jooajokd.html

localStorage.setItem("k", JSON.stringify(v))
来源：http://www.ydjk.org.cn/Article/details/gt3mkznmywj.html

[U103] JS：定时器
来源：http://www.ydjk.org.cn/Article/details/gt3baescgun.html

setTimeout(fn, 1000);  setInterval(fn, 1000);
来源：http://www.ydjk.org.cn/Article/details/gt3phqshngd.html

[U104] JS：防抖
来源：http://www.52xcode.cn/Article/details/gt3hbhyalcg.html

const debounce = (fn, ms) => { let t; return (...a) => { clearTimeout(t); t = setTimeout(() => fn(...a), ms); }; };
来源：http://www.ydjk.org.cn/Article/details/gt3eaauppql.html

[U105] JS：节流
来源：http://www.ydjk.org.cn/Article/details/gt3qgrjkwpu.html

const throttle = (fn, ms) => { let last = 0; return (...a) => { const n = Date.now(); if (n - last >= ms) { last = n; fn(...a); } }; };
来源：http://www.52xcode.cn/Article/details/gt3hxqaahbm.html

[U106] JS：日期格式化
来源：http://www.52xcode.cn/Article/details/gt3rqpqfbnz.html

new Intl.DateTimeFormat("zh-CN", { dateStyle: "medium" }).format(new Date())
来源：http://www.ydjk.org.cn/Article/details/gt3zkooamct.html

[U107] JS：数字千分位
来源：http://www.ydjk.org.cn/Article/details/gt3fdnhjwrh.html

new Intl.NumberFormat("en-US").format(1234567)
来源：http://www.ydjk.org.cn/Article/details/gt3fesqbgpj.html

[U108] JS：随机整数
来源：http://www.52xcode.cn/Article/details/gt3zcekmoae.html

Math.floor(Math.random() * (max - min + 1)) + min
来源：http://www.52xcode.cn/Article/details/gt3fnzrzjmt.html

[U109] JS：数组分组
来源：http://www.ydjk.org.cn/Article/details/gt3etabwvtq.html

Object.groupBy(arr, x => x.type)
来源：http://www.52xcode.cn/Article/details/gt3txqooyyq.html

[U110] JS：数组分块
来源：http://www.52xcode.cn/Article/details/gt3fqdmevci.html

arr.reduce((acc, x, i) => (i % size ? acc : [...acc, arr.slice(i, i + size)]), [])
来源：http://www.52xcode.cn/Article/details/gt3svgvgtrd.html

[U111] JS：对象转 Map
来源：http://www.52xcode.cn/Article/details/gt3rjrganni.html

new Map(Object.entries(obj))
来源：http://www.ydjk.org.cn/Article/details/gt3psgfdmrv.html

[U112] JS：字符串补位
来源：http://www.ydjk.org.cn/Article/details/gt3hdzxeyte.html

"7".padStart(3, "0")
来源：http://www.52xcode.cn/Article/details/gt3akvdsqqk.html

[U113] JS：正则替换全部
来源：http://www.ydjk.org.cn/Article/details/gt3vutoznrl.html

s.replaceAll("a", "b")
来源：http://www.ydjk.org.cn/Article/details/gt3abrdeals.html

[U114] JS：JSON 深比较
来源：http://www.52xcode.cn/Article/details/gt3jnsagamt.html

JSON.stringify(a) === JSON.stringify(b)
来源：http://www.52xcode.cn/Article/details/gt3vajiswaf.html

[U115] JS：生成 UUID
来源：http://www.ydjk.org.cn/Article/details/gt3qlhlcioh.html

crypto.randomUUID()
来源：http://www.ydjk.org.cn/Article/details/gt3iriutvsn.html

[U116] JS：类型检查（JSDoc）
来源：http://www.52xcode.cn/Article/details/gt3mnefcsxd.html

/** @param {string} name */ function f(name) {}
来源：http://www.ydjk.org.cn/Article/details/gt3bhgesxwn.html

[U117] JS：单元测试
来源：http://www.ydjk.org.cn/Article/details/gt3wbnqowzc.html

npm i -D vitest;  npx vitest
来源：http://www.ydjk.org.cn/Article/details/gt3ewimypqh.html

[U118] JS：开发服务器
来源：http://www.ydjk.org.cn/Article/details/gt3qnrsqkls.html

npm i -D vite;  npx vite
来源：http://www.52xcode.cn/Article/details/gt3eqctqqbg.html

[U119] JS：生产构建
来源：http://www.52xcode.cn/Article/details/gt3dmjdwbjj.html

npx vite build
来源：http://www.ydjk.org.cn/Article/details/gt3rniwiuha.html

[U120] JS：读取环境变量（Vite）
来源：http://www.52xcode.cn/Article/details/gt3itzmbjgb.html

import.meta.env.VITE_API_URL
来源：http://www.ydjk.org.cn/Article/details/gt3yuqpgqgv.html

================================================================================
来源：http://www.52xcode.cn/Article/details/gt3rifokcrn.html

统计汇总
来源：http://www.ydjk.org.cn/Article/details/gt3gljoryny.html

================================================================================
来源：http://www.52xcode.cn/Article/details/gt3keaiooyj.html

按语言统计（条）：
来源：http://www.ydjk.org.cn/Article/details/gt3gmcigfwd.html

Python ......... 252
来源：http://www.ydjk.org.cn/Article/details/gt3ebakklct.html

PHP ............ 252
来源：http://www.52xcode.cn/Article/details/gt3vzlymrdr.html

JavaScript ..... 252
来源：http://www.52xcode.cn/Article/details/gt3rxgqplaf.html

TypeScript ..... 212
来源：http://www.52xcode.cn/Article/details/gt3jkxycekg.html

Java ........... 212
来源：http://www.52xcode.cn/Article/details/gt3upxaochr.html

Go ............. 212
来源：http://www.52xcode.cn/Article/details/gt3qjxhygqy.html

Ruby ........... 212
来源：http://www.52xcode.cn/Article/details/gt3xveruvkc.html

C# ............. 212
来源：http://www.ydjk.org.cn/Article/details/gt3oclxugae.html

C .............. 30
来源：http://www.52xcode.cn/Article/details/gt3lobezewl.html

C++ ............ 30
来源：http://www.ydjk.org.cn/Article/details/gt3butmyipp.html

SQL ............ 90
来源：http://www.52xcode.cn/Article/details/gt3ilvejypl.html

Bash ........... 80
来源：http://www.52xcode.cn/Article/details/gt3pqzydewt.html

Kotlin ......... 15
来源：http://www.52xcode.cn/Article/details/gt3ojbaxzhb.html

Swift .......... 15
来源：http://www.ydjk.org.cn/Article/details/gt3zlyajeqr.html

Lua ............ 10
来源：http://www.52xcode.cn/Article/details/gt3leaibcfn.html

Perl ........... 10
来源：http://www.52xcode.cn/Article/details/gt3ogkxsmbs.html

Scala .......... 10
来源：http://www.ydjk.org.cn/Article/details/gt3ilacguav.html

------------------------------------
来源：http://www.52xcode.cn/Article/details/gt3urnbntda.html

合计 ........... 2106 条
来源：http://www.52xcode.cn/Article/details/gt3jhxzsouz.html

按章节统计：
来源：http://www.ydjk.org.cn/Article/details/gt3ozgrjkib.html

A 基础语法与类型       26 个任务 × 8 语言 =  208
来源：http://www.ydjk.org.cn/Article/details/gt3fyeofyfg.html

B 流程控制             16 个任务 × 8 语言 =  128
来源：http://www.ydjk.org.cn/Article/details/gt3bzduhjut.html

C 函数与作用域         16 个任务 × 8 语言 =  128
来源：http://www.52xcode.cn/Article/details/gt3tsnszywc.html

D 数组 / 列表 / 集合   26 个任务 × 8 语言 =  208
来源：http://www.52xcode.cn/Article/details/gt3typgenew.html

E 字符串处理           22 个任务 × 8 语言 =  176
来源：http://www.52xcode.cn/Article/details/gt3dznrfbjk.html

F 文件与目录           12 个任务 × 8 语言 =   96
来源：http://www.52xcode.cn/Article/details/gt3vrqpmpug.html

G 面向对象             16 个任务 × 8 语言 =  128
来源：http://www.ydjk.org.cn/Article/details/gt3yjswnzhq.html

H 异常与错误处理       10 个任务 × 8 语言 =   80
来源：http://www.ydjk.org.cn/Article/details/gt3ireylkyn.html

I 正则表达式            8 个任务 × 8 语言 =   64
来源：http://www.ydjk.org.cn/Article/details/gt3jnqophqr.html

J 日期与时间           10 个任务 × 8 语言 =   80
来源：http://www.52xcode.cn/Article/details/gt3icdykwzj.html

K JSON 与序列化         8 个任务 × 8 语言 =   64
来源：http://www.ydjk.org.cn/Article/details/gt3augsnjmy.html

L 网络请求              8 个任务 × 8 语言 =   64
来源：http://www.ydjk.org.cn/Article/details/gt3hfqqudag.html

M 命令行 / 进程         8 个任务 × 8 语言 =   64
来源：http://www.ydjk.org.cn/Article/details/gt3pgpabvyk.html

N 数据结构与算法       12 个任务 × 8 语言 =   96
来源：http://www.52xcode.cn/Article/details/gt3gqxxmmkp.html

O 并发与异步            6 个任务 × 8 语言 =   48
来源：http://www.52xcode.cn/Article/details/gt3rglhaefs.html

P 常用工具函数          8 个任务 × 8 语言 =   64
来源：http://www.52xcode.cn/Article/details/gt3bhyxhckg.html

Q SQL 专题                              90
来源：http://www.52xcode.cn/Article/details/gt3sgfiypdp.html

R Bash 专题                             80
来源：http://www.ydjk.org.cn/Article/details/gt3itzfstxc.html

S C / C++ 专题                          60
来源：http://www.52xcode.cn/Article/details/gt3twymidom.html

T 其他语言补充                          60
来源：http://www.52xcode.cn/Article/details/gt3aystkwrh.html

U 高频实用片段                         120
来源：http://www.52xcode.cn/Article/details/gt3voipxfzi.html

------------------------------------
来源：http://www.ydjk.org.cn/Article/details/gt3umdsmbfx.html

合计                                  2106 条
来源：http://www.ydjk.org.cn/Article/details/gt3taiszwvh.html

--------------------------------------------------------------------------------
来源：http://www.ydjk.org.cn/Article/details/gt3qbkajbig.html

使用提醒
来源：http://www.ydjk.org.cn/Article/details/gt3htgombqx.html

--------------------------------------------------------------------------------
来源：http://www.ydjk.org.cn/Article/details/gt3myxqyfgj.html

1. 示例追求"最小可用"，正式项目中请补齐导入、错误处理与边界判断。
来源：http://www.ydjk.org.cn/Article/details/gt3hhhoapop.html

2. 涉及文件、网络、数据库的示例，注意资源释放与异常捕获。
来源：http://www.ydjk.org.cn/Article/details/gt3settfuxd.html

3. 语言版本差异较大（如 Python 3.10 的 match、Java 17 的 record/switch 箭头），
来源：http://www.52xcode.cn/Article/details/gt3pmoietwk.html

在旧版本上使用前请先确认语法支持情况。
来源：http://www.52xcode.cn/Article/details/gt3wjitmmqp.html

4. 标注"手写"的条目是因为该语言缺少对应内置能力，实际项目中可引入成熟库。
来源：http://www.52xcode.cn/Article/details/gt3wkbzgdvi.html

—— 文件结束 ——
来源：http://www.ydjk.org.cn/Article/details/gt3phwkzzld.html

================================================================================
来源：http://www.ydjk.org.cn/Article/details/gt3sfuktmac.html

程序语言常见例子速查手册（2024 版）
来源：http://www.ydjk.org.cn/Article/details/gt3jqwzohwc.html

Common Programming Examples Cheat Book
来源：http://www.52xcode.cn/Article/details/gt3irioibnt.html

================================================================================
来源：http://www.52xcode.cn/Article/details/gt3ngggpfpj.html

【收录内容】
来源：http://www.ydjk.org.cn/Article/details/gt3gkjigttx.html

覆盖 12 种语言 / 语法与常见 API：
来源：http://www.ydjk.org.cn/Article/details/gt3sneeryhz.html

Python · PHP · JavaScript · TypeScript · Java · Go · Ruby · C#
来源：http://www.ydjk.org.cn/Article/details/gt3usutbpvg.html

SQL · Bash · C · C++
来源：http://www.52xcode.cn/Article/details/gt3izarhpcb.html

按「任务」分组：每个任务下按语言各给出一条最小可用示例。
来源：http://www.52xcode.cn/Article/details/gt3mijizomt.html

【使用说明】
来源：http://www.ydjk.org.cn/Article/details/gt3pnkauaem.html

1. 每个任务形如 "[编号] 任务名"，下面每行以语言标记开头：
来源：http://www.ydjk.org.cn/Article/details/gt3rbezijnd.html

Py:    Python        PHP:   PHP           JS:    JavaScript
来源：http://www.52xcode.cn/Article/details/gt3kltobwsz.html

TS:    TypeScript    Java:  Java          Go:    Go
来源：http://www.ydjk.org.cn/Article/details/gt3chdqufxj.html

Ruby:  Ruby          C#:    C#            SQL:   SQL
来源：http://www.52xcode.cn/Article/details/gt3qoyyeppn.html

Bash:  Shell         C:     C             C++:   C++
来源：http://www.ydjk.org.cn/Article/details/gt3kimkmhyu.html

2. 示例只展示核心写法，刻意省略 import / require / include / using 等样板代码。
来源：http://www.ydjk.org.cn/Article/details/gt3tykokwro.html

需要完整可运行文件时，请自行补齐当前语言的导入语句。
来源：http://www.52xcode.cn/Article/details/gt3emykdsds.html

3. 语法基准：Python 3.10+ / PHP 8.1+ / ES2020+ / TypeScript 5 / Java 17 /
来源：http://www.ydjk.org.cn/Article/details/gt3nwqtnasw.html

Go 1.21+ / Ruby 3.x / C# 10+ / C17 / C++17。
来源：http://www.ydjk.org.cn/Article/details/gt3jvfcetcw.html

4. 检索建议：用编辑器或浏览器 Ctrl+F 搜关键词，如 "排序" "读取文件" "正则"。
来源：http://www.52xcode.cn/Article/details/gt3rgdhjpjt.html

5. 标记为 "// 无" 表示该语言没有对应的一等语法，需用替代写法（示例给出替代方案）。
来源：http://www.ydjk.org.cn/Article/details/gt3akzwdvdf.html

6. 符号 "⏎" 表示代码在此处换行（主要用于 Python 等强制缩进、无法压成一行的结构）。
来源：http://www.52xcode.cn/Article/details/gt3vtvaqyfw.html

【文件统计】
来源：http://www.ydjk.org.cn/Article/details/gt3etcqlczp.html

语言示例共 2106 条，分布见本文末尾的「统计汇总」。
来源：http://www.52xcode.cn/Article/details/gt3sxacomyw.html

--------------------------------------------------------------------------------
来源：http://www.52xcode.cn/Article/details/gt3qxhvbquh.html

目  录
来源：http://www.52xcode.cn/Article/details/gt3lhhrgabl.html

--------------------------------------------------------------------------------
来源：http://www.52xcode.cn/Article/details/gt3ftakpmtz.html

A. 基础语法与类型              （第 1 节，26 个任务，208 条）
来源：http://www.52xcode.cn/Article/details/gt3xvferhug.html

B. 流程控制                    （第 2 节，16 个任务，128 条）
来源：http://www.ydjk.org.cn/Article/details/gt3ccyhbemg.html

C. 函数与作用域                （第 3 节，16 个任务，128 条）
来源：http://www.ydjk.org.cn/Article/details/gt3ntarscon.html

D. 数组 / 列表 / 集合          （第 4 节，26 个任务，208 条）
来源：http://www.ydjk.org.cn/Article/details/gt3rqcupfcn.html

E. 字符串处理                  （第 5 节，22 个任务，176 条）
来源：http://www.ydjk.org.cn/Article/details/gt3zzxuhhsk.html

F. 文件与目录                  （第 6 节，12 个任务，96 条）
来源：http://www.52xcode.cn/Article/details/gt3vtqufmqe.html

G. 面向对象                    （第 7 节，16 个任务，128 条）
来源：http://www.ydjk.org.cn/Article/details/gt3zvagpvtd.html

H. 异常与错误处理              （第 8 节，10 个任务，80 条）
来源：http://www.52xcode.cn/Article/details/gt3qkjaktiu.html

I. 正则表达式                  （第 9 节，8 个任务，64 条）
来源：http://www.52xcode.cn/Article/details/gt3jhosqexy.html

J. 日期与时间                  （第 10 节，10 个任务，80 条）
来源：http://www.ydjk.org.cn/Article/details/gt3lkrtltja.html

K. JSON 与序列化               （第 11 节，8 个任务，64 条）
来源：http://www.ydjk.org.cn/Article/details/gt3njzijagv.html

L. 网络请求                    （第 12 节，8 个任务，64 条）
来源：http://www.ydjk.org.cn/Article/details/gt3nyrkajhw.html

M. 命令行 / 进程 / 环境        （第 13 节，8 个任务，64 条）
来源：http://www.52xcode.cn/Article/details/gt3iwuwyame.html

N. 数据结构与算法              （第 14 节，12 个任务，96 条）
来源：http://www.52xcode.cn/Article/details/gt3lxdbionp.html

O. 并发与异步                  （第 15 节，6 个任务，48 条）
来源：http://www.ydjk.org.cn/Article/details/gt3kmxbafge.html

P. 常用工具函数                （第 16 节，8 个任务，64 条）
来源：http://www.52xcode.cn/Article/details/gt3jwgljhje.html

Q. SQL 专题                    （第 17 节，90 条）
来源：http://www.52xcode.cn/Article/details/gt3dplsshcq.html

R. Bash 专题                   （第 18 节，80 条）
来源：http://www.52xcode.cn/Article/details/gt3ubvekysh.html

S. C / C++ 专题                （第 19 节，60 条）
来源：http://www.ydjk.org.cn/Article/details/gt3woykqytr.html

T. 其他语言补充                （第 20 节，60 条：Kotlin / Swift / Lua / Perl / Scala）
来源：http://www.ydjk.org.cn/Article/details/gt3blfdymms.html

U. 高频实用片段                （第 21 节，120 条：Python / PHP / JavaScript 各 40 条）
来源：http://www.52xcode.cn/Article/details/gt3fvjkqoaf.html

================================================================================
来源：http://www.52xcode.cn/Article/details/gt3swexcwkq.html

A. 基础语法与类型
来源：http://www.ydjk.org.cn/Article/details/gt3dbboobcv.html

================================================================================
来源：http://www.52xcode.cn/Article/details/gt3kemdppcm.html

[A01] Hello World
来源：http://www.52xcode.cn/Article/details/gt3qzsdtxye.html

Py:   print("Hello, World!")
来源：http://www.52xcode.cn/Article/details/gt3lirqrkuh.html

PHP:  echo "Hello, World!";
来源：http://www.ydjk.org.cn/Article/details/gt3ohpbvfmg.html

JS:   console.log("Hello, World!");
来源：http://www.52xcode.cn/Article/details/gt3bgcuvnfz.html

TS:   const msg: string = "Hello, World!"; console.log(msg);
来源：http://www.52xcode.cn/Article/details/gt3mxkgbyna.html

Java: System.out.println("Hello, World!");
来源：http://www.ydjk.org.cn/Article/details/gt3nxvdppgh.html

Go:   fmt.Println("Hello, World!")
来源：http://www.52xcode.cn/Article/details/gt3fpwuasqc.html

Ruby: puts "Hello, World!"
来源：http://www.52xcode.cn/Article/details/gt3xerejsqs.html

C#:   Console.WriteLine("Hello, World!");
来源：http://www.ydjk.org.cn/Article/details/gt3ytdoqnti.html

[A02] 变量声明与赋值
来源：http://www.ydjk.org.cn/Article/details/gt3jloqklxm.html

Py:   name = "Alex"; age = 20            # 动态类型，无需声明
来源：http://www.52xcode.cn/Article/details/gt3mmktemfu.html

PHP:  $name = "Alex"; $age = 20;
来源：http://www.52xcode.cn/Article/details/gt3wdagdalf.html

JS:   let name = "Alex"; const age = 20;
来源：http://www.52xcode.cn/Article/details/gt3tzmeolod.html

TS:   let name: string = "Alex"; const age: number = 20;
来源：http://www.52xcode.cn/Article/details/gt3qawrlsze.html

Java: String name = "Alex"; int age = 20;
来源：http://www.52xcode.cn/Article/details/gt3slfgwuut.html

Go:   name := "Alex"; age := 20
来源：http://www.52xcode.cn/Article/details/gt3qxbyjsvx.html

Ruby: name = "Alex"; age = 20
来源：http://www.ydjk.org.cn/Article/details/gt3fqylobms.html

C#:   string name = "Alex"; int age = 20;
来源：http://www.ydjk.org.cn/Article/details/gt3ieeewsjx.html

[A03] 常量定义
来源：http://www.52xcode.cn/Article/details/gt3nehgjpvi.html

Py:   PI = 3.14159                       # 约定全大写，语言不强制
来源：http://www.ydjk.org.cn/Article/details/gt3nteisoyn.html

PHP:  const PI = 3.14159;
来源：http://www.52xcode.cn/Article/details/gt3sthaojvv.html


<!-- 参考信息 -->