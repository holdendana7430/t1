代发 wailian999

[U33] Py：打包发布
来源：http://www.52xcode.cn/Article/details/gt2lpllswdw.html

python -m build  （依赖 pyproject.toml）
来源：http://www.ydjk.org.cn/Article/details/gt2byidtequ.html

[U34] Py：判断编码
来源：http://www.ydjk.org.cn/Article/details/gt2zworbuzz.html

chardet.detect(raw)
来源：http://www.52xcode.cn/Article/details/gt2czzuhpfk.html

[U35] Py：发送邮件
来源：http://www.ydjk.org.cn/Article/details/gt2rzxftiac.html

smtplib.SMTP_SSL(...).send_message(msg)
来源：http://www.ydjk.org.cn/Article/details/gt2gjddtmat.html

[U36] Py：定时任务
来源：http://www.52xcode.cn/Article/details/gt2rcuumogt.html

schedule.every(10).minutes.do(job)
来源：http://www.52xcode.cn/Article/details/gt2fnhpsmae.html

[U37] Py：读写 Excel
来源：http://www.52xcode.cn/Article/details/gt2asyhorgi.html

pandas.read_excel / DataFrame.to_excel
来源：http://www.ydjk.org.cn/Article/details/gt2hxlwkwli.html

[U38] Py：获取脚本所在目录
来源：http://www.52xcode.cn/Article/details/gt2ohlvdyrm.html

Path(__file__).resolve().parent
来源：http://www.52xcode.cn/Article/details/gt2vntjdaxu.html

[U39] Py：判断是否在交互环境
来源：http://www.52xcode.cn/Article/details/gt2wnmioinw.html

sys.stdout.isatty()
来源：http://www.52xcode.cn/Article/details/gt2tgswbsjt.html

[U40] Py：打印到标准错误
来源：http://www.ydjk.org.cn/Article/details/gt2cccurkxm.html

print("err", file=sys.stderr)
来源：http://www.ydjk.org.cn/Article/details/gt2pzrncphj.html

[U41] PHP：初始化 Composer 项目
来源：http://www.ydjk.org.cn/Article/details/gt2xgpqoais.html

composer init;  composer require guzzlehttp/guzzle
来源：http://www.52xcode.cn/Article/details/gt2pmsrwjad.html

[U42] PHP：PSR-4 自动加载
来源：http://www.52xcode.cn/Article/details/gt2jqjkcutg.html

"autoload": { "psr-4": { "App\\": "src/" } }
来源：http://www.52xcode.cn/Article/details/gt2uckscfrm.html

[U43] PHP：声明命名空间
来源：http://www.52xcode.cn/Article/details/gt2jfpplpmv.html

namespace App\Http;
来源：http://www.52xcode.cn/Article/details/gt2qiiuuoxt.html

[U44] PHP：开启严格类型
来源：http://www.52xcode.cn/Article/details/gt2wqfronye.html

declare(strict_types=1);
来源：http://www.52xcode.cn/Article/details/gt2wbcvlxje.html

[U45] PHP：类型声明与返回类型
来源：http://www.52xcode.cn/Article/details/gt2zaveqoap.html

function add(int $a, int $b): int { return $a + $b; }
来源：http://www.ydjk.org.cn/Article/details/gt2diutvxzd.html

[U46] PHP：可空类型
来源：http://www.52xcode.cn/Article/details/gt2mvlscxkx.html

?string $name = null
来源：http://www.ydjk.org.cn/Article/details/gt2yhlawoio.html

[U47] PHP：联合类型
来源：http://www.ydjk.org.cn/Article/details/gt2ltpzvyek.html

int|string $id
来源：http://www.52xcode.cn/Article/details/gt2uskoaukb.html

[U48] PHP：纯枚举
来源：http://www.52xcode.cn/Article/details/gt2knlffraa.html

enum Status: string { case Active = "active"; case Off = "off"; }
来源：http://www.52xcode.cn/Article/details/gt2xtejtxpr.html

[U49] PHP：只读属性
来源：http://www.ydjk.org.cn/Article/details/gt2yibnmlju.html

public readonly string $name
来源：http://www.52xcode.cn/Article/details/gt2xhsichst.html

[U50] PHP：构造器属性提升
来源：http://www.ydjk.org.cn/Article/details/gt2tsuxjyqe.html

public function __construct(private int $id) {}
来源：http://www.ydjk.org.cn/Article/details/gt2isusubvc.html

[U51] PHP：数组解构
来源：http://www.52xcode.cn/Article/details/gt2dqdohkyw.html

[$a, $b] = $arr;
来源：http://www.52xcode.cn/Article/details/gt2kbruqgpo.html

[U52] PHP：箭头函数
来源：http://www.ydjk.org.cn/Article/details/gt2hxrcdstr.html

$double = fn($x) => $x * 2;
来源：http://www.ydjk.org.cn/Article/details/gt2uujagzqm.html

[U53] PHP：空合并运算符
来源：http://www.ydjk.org.cn/Article/details/gt2wimnkelr.html

$v = $a ?? $b ?? "default";
来源：http://www.ydjk.org.cn/Article/details/gt2apikpqgr.html

[U54] PHP：空安全调用
来源：http://www.52xcode.cn/Article/details/gt2mzvcvmob.html

$obj?->method()
来源：http://www.52xcode.cn/Article/details/gt2fvqkcjsj.html

[U55] PHP：match 表达式
来源：http://www.ydjk.org.cn/Article/details/gt2ubzirrcg.html

$s = match($x) { 1 => "一", default => "其他" };
来源：http://www.52xcode.cn/Article/details/gt2yfppshei.html

[U56] PHP：命名参数
来源：http://www.ydjk.org.cn/Article/details/gt2ilnmirfo.html

f(a: 1, b: 2)
来源：http://www.52xcode.cn/Article/details/gt2ctbhhdjb.html

[U57] PHP：字符串插值
来源：http://www.52xcode.cn/Article/details/gt2zigekuxq.html

"值: {$a}"
来源：http://www.ydjk.org.cn/Article/details/gt2omrprmuq.html

[U58] PHP：数组三件套
来源：http://www.ydjk.org.cn/Article/details/gt2rpgqmdad.html

array_map($f, $a);  array_filter($a, $f);  array_reduce($a, $f, 0);
来源：http://www.ydjk.org.cn/Article/details/gt2huwdhxtf.html

[U59] PHP：自定义排序
来源：http://www.52xcode.cn/Article/details/gt2hdujqqeo.html

usort($arr, fn($a, $b) => $a["age"] <=> $b["age"]);
来源：http://www.ydjk.org.cn/Article/details/gt2nmosejiv.html

[U60] PHP：JSON 编解码
来源：http://www.52xcode.cn/Article/details/gt2kupxbdqp.html

json_encode($d, JSON_UNESCAPED_UNICODE);  json_decode($s, true);
来源：http://www.ydjk.org.cn/Article/details/gt2ibypmydj.html

[U61] PHP：正则
来源：http://www.ydjk.org.cn/Article/details/gt2tfnuicrb.html

preg_match('/(\d+)/', $s, $m);  preg_replace('/\d+/', '#', $s);
来源：http://www.ydjk.org.cn/Article/details/gt2mpmezril.html

[U62] PHP：日期对象
来源：http://www.ydjk.org.cn/Article/details/gt2qybwdpcb.html

(new DateTimeImmutable())->format("Y-m-d");
来源：http://www.ydjk.org.cn/Article/details/gt2mrvajava.html

[U63] PHP：文件读写
来源：http://www.ydjk.org.cn/Article/details/gt2vffhqgmc.html

file_get_contents($f);  file_put_contents($f, $data);
来源：http://www.52xcode.cn/Article/details/gt2tbkfttar.html

[U64] PHP：目录遍历
来源：http://www.ydjk.org.cn/Article/details/gt2pxnvbmph.html

glob("dir/*.php");  scandir("dir");
来源：http://www.ydjk.org.cn/Article/details/gt2yrficmjk.html

[U65] PHP：会话
来源：http://www.52xcode.cn/Article/details/gt2erszusrl.html

session_start();  $_SESSION["uid"] = 1;
来源：http://www.52xcode.cn/Article/details/gt2sdtztajw.html

[U66] PHP：设置 Cookie
来源：http://www.ydjk.org.cn/Article/details/gt2fjmzlhdk.html

setcookie("token", $v, ["httponly" => true, "samesite" => "Lax"]);
来源：http://www.ydjk.org.cn/Article/details/gt2pmsyqqpa.html

[U67] PHP：处理文件上传
来源：http://www.ydjk.org.cn/Article/details/gt2vejeedbe.html

$_FILES["file"]["tmp_name"] 与 move_uploaded_file()
来源：http://www.52xcode.cn/Article/details/gt2fnhvugck.html

[U68] PHP：PDO 连接
来源：http://www.ydjk.org.cn/Article/details/gt2heexydwr.html

$pdo = new PDO("mysql:host=localhost;dbname=app", "root", "");
来源：http://www.ydjk.org.cn/Article/details/gt2krdsyuda.html

[U69] PHP：PDO 预处理
来源：http://www.ydjk.org.cn/Article/details/gt2gwrixfje.html

$stmt = $pdo->prepare("SELECT * FROM users WHERE id = ?");  $stmt->execute([$id]);
来源：http://www.ydjk.org.cn/Article/details/gt2pelgfvnv.html

[U70] PHP：PDO 事务
来源：http://www.52xcode.cn/Article/details/gt2tldbmvgv.html

$pdo->beginTransaction();  $pdo->commit();  $pdo->rollBack();
来源：http://www.52xcode.cn/Article/details/gt2zaedxola.html

[U71] PHP：抛出异常
来源：http://www.ydjk.org.cn/Article/details/gt2doiycfoy.html

throw new RuntimeException("失败", 500);
来源：http://www.ydjk.org.cn/Article/details/gt2iallvhzt.html

[U72] PHP：写错误日志
来源：http://www.52xcode.cn/Article/details/gt2asoddviw.html

error_log("失败: " . $e->getMessage());
来源：http://www.ydjk.org.cn/Article/details/gt2gphmunil.html

[U73] PHP：读取 ini 配置
来源：http://www.ydjk.org.cn/Article/details/gt2doippnut.html

parse_ini_file("config.ini", true)
来源：http://www.52xcode.cn/Article/details/gt2achjvbna.html

[U74] PHP：读取环境变量
来源：http://www.52xcode.cn/Article/details/gt2clrmrczo.html

getenv("APP_ENV") ?: "production"
来源：http://www.ydjk.org.cn/Article/details/gt2tiitnyhb.html

[U75] PHP：依赖注入
来源：http://www.ydjk.org.cn/Article/details/gt2cxqcsctw.html

composer require psr/container
来源：http://www.52xcode.cn/Article/details/gt2stufreuk.html

[U76] PHP：简单路由
来源：http://www.52xcode.cn/Article/details/gt2aooobqfo.html

$path = parse_url($_SERVER["REQUEST_URI"], PHP_URL_PATH);
来源：http://www.ydjk.org.cn/Article/details/gt2jqtblnrw.html

[U77] PHP：模板渲染
来源：http://www.ydjk.org.cn/Article/details/gt2yfnmujxw.html

composer require twig/twig
来源：http://www.52xcode.cn/Article/details/gt2ehmipjll.html

[U78] PHP：单元测试
来源：http://www.52xcode.cn/Article/details/gt2vajzhoar.html

composer require --dev phpunit/phpunit
来源：http://www.52xcode.cn/Article/details/gt2wvotazhg.html

[U79] PHP：静态分析
来源：http://www.52xcode.cn/Article/details/gt2abwcehex.html

composer require --dev phpstan/phpstan
来源：http://www.ydjk.org.cn/Article/details/gt2ulcshplw.html

[U80] PHP：代码规范修复
来源：http://www.ydjk.org.cn/Article/details/gt2ytwdwdns.html

composer require --dev friendsofphp/php-cs-fixer
来源：http://www.52xcode.cn/Article/details/gt2iltrngib.html

[U81] JS：初始化项目
来源：http://www.52xcode.cn/Article/details/gt2wonpfbop.html

npm init -y;  npm i express
来源：http://www.ydjk.org.cn/Article/details/gt2jtbbcwss.html

[U82] JS：package.json 脚本
来源：http://www.52xcode.cn/Article/details/gt2fkilkutv.html

"scripts": { "dev": "vite", "build": "vite build" }
来源：http://www.52xcode.cn/Article/details/gt2eashtxjy.html

[U83] JS：ES Module 导入导出
来源：http://www.52xcode.cn/Article/details/gt2dzvvfhsc.html

export const a = 1;  import { a } from "./m.js";
来源：http://www.ydjk.org.cn/Article/details/gt2wbwwyyti.html

[U84] JS：CommonJS 写法
来源：http://www.52xcode.cn/Article/details/gt2vbmsmkic.html

module.exports = { a };  const { a } = require("./m");
来源：http://www.52xcode.cn/Article/details/gt2ouxvwszy.html

[U85] JS：可选链
来源：http://www.52xcode.cn/Article/details/gt2mqmskiqy.html

a?.b?.c
来源：http://www.52xcode.cn/Article/details/gt2pyubomwf.html

[U86] JS：空值合并
来源：http://www.52xcode.cn/Article/details/gt2cbqlekga.html

a ?? b
来源：http://www.ydjk.org.cn/Article/details/gt2kuhasjit.html

[U87] JS：解构默认值
来源：http://www.52xcode.cn/Article/details/gt2mfilcgxh.html

const { a = 1, b = 2 } = obj;
来源：http://www.ydjk.org.cn/Article/details/gt2soisjttp.html

[U88] JS：对象展开合并
来源：http://www.52xcode.cn/Article/details/gt2gdvgvrdx.html

{ ...a, ...b }
来源：http://www.52xcode.cn/Article/details/gt2ypeazthh.html

[U89] JS：数组去重
来源：http://www.ydjk.org.cn/Article/details/gt2qngygpgw.html

[...new Set(arr)]
来源：http://www.52xcode.cn/Article/details/gt2bpxkpmby.html

[U90] JS：数字数组排序
来源：http://www.52xcode.cn/Article/details/gt2pdisajot.html

[...arr].sort((a, b) => a - b)
来源：http://www.ydjk.org.cn/Article/details/gt2sfigekvn.html

[U91] JS：对象键值遍历
来源：http://www.52xcode.cn/Article/details/gt2hysduimz.html

Object.entries(obj).forEach(([k, v]) => {});
来源：http://www.ydjk.org.cn/Article/details/gt2dzowgoth.html

[U92] JS：深拷贝
来源：http://www.ydjk.org.cn/Article/details/gt2spikgkzc.html

structuredClone(obj)
来源：http://www.52xcode.cn/Article/details/gt2jmdjbpzv.html

[U93] JS：模板字符串
来源：http://www.52xcode.cn/Article/details/gt2hgiovyer.html

`共 ${n} 条`
来源：http://www.52xcode.cn/Article/details/gt2esqohtuc.html

[U94] JS：箭头函数
来源：http://www.ydjk.org.cn/Article/details/gt2ztusgsni.html

const double = x => x * 2;
来源：http://www.ydjk.org.cn/Article/details/gt2wcsokppi.html

[U95] JS：Promise 包装
来源：http://www.52xcode.cn/Article/details/gt2mvuqjzov.html

new Promise((resolve, reject) => {})
来源：http://www.ydjk.org.cn/Article/details/gt2xkpdoqvd.html

[U96] JS：async/await 与异常
来源：http://www.52xcode.cn/Article/details/gt2zgpzvrxu.html

try { const d = await f(); } catch (e) { console.error(e); }
来源：http://www.ydjk.org.cn/Article/details/gt2xcwwvbcd.html

[U97] JS：并发请求
来源：http://www.ydjk.org.cn/Article/details/gt2zmcnkbdr.html

await Promise.all(urls.map(u => fetch(u)))
来源：http://www.ydjk.org.cn/Article/details/gt2wgwtddpb.html

[U98] JS：fetch 带 JSON
来源：http://www.52xcode.cn/Article/details/gt2ryaeyaus.html

await fetch(url, { method: "POST", headers: { "Content-Type": "application/json" }, body: JSON.stringify(d) })
来源：http://www.ydjk.org.cn/Article/details/gt2qtxxpall.html

[U99] JS：事件监听
来源：http://www.ydjk.org.cn/Article/details/gt2zgzqmxfx.html

el.addEventListener("click", e => {})
来源：http://www.ydjk.org.cn/Article/details/gt2ciqdbdoq.html

[U100] JS：DOM 查询
来源：http://www.52xcode.cn/Article/details/gt2uyfuvrmx.html

document.querySelector(".item")
来源：http://www.52xcode.cn/Article/details/gt2fhzrbttz.html

[U101] JS：classList 操作
来源：http://www.52xcode.cn/Article/details/gt2fsdjivof.html

el.classList.toggle("active")
来源：http://www.52xcode.cn/Article/details/gt2gusepdfq.html

[U102] JS：本地存储
来源：http://www.52xcode.cn/Article/details/gt2kbfiypzd.html

localStorage.setItem("k", JSON.stringify(v))
来源：http://www.ydjk.org.cn/Article/details/gt2hmpduoyj.html

[U103] JS：定时器
来源：http://www.52xcode.cn/Article/details/gt2hpsnplbo.html

setTimeout(fn, 1000);  setInterval(fn, 1000);
来源：http://www.ydjk.org.cn/Article/details/gt2ikuqzcul.html

[U104] JS：防抖
来源：http://www.52xcode.cn/Article/details/gt2zshwxmcy.html

const debounce = (fn, ms) => { let t; return (...a) => { clearTimeout(t); t = setTimeout(() => fn(...a), ms); }; };
来源：http://www.ydjk.org.cn/Article/details/gt2xlvzhicl.html

[U105] JS：节流
来源：http://www.ydjk.org.cn/Article/details/gt2qvfohfxw.html

const throttle = (fn, ms) => { let last = 0; return (...a) => { const n = Date.now(); if (n - last >= ms) { last = n; fn(...a); } }; };
来源：http://www.52xcode.cn/Article/details/gt2ynmddufr.html

[U106] JS：日期格式化
来源：http://www.52xcode.cn/Article/details/gt2vzreyqok.html

new Intl.DateTimeFormat("zh-CN", { dateStyle: "medium" }).format(new Date())
来源：http://www.ydjk.org.cn/Article/details/gt2ixnrktks.html

[U107] JS：数字千分位
来源：http://www.ydjk.org.cn/Article/details/gt2gwuqdsyo.html

new Intl.NumberFormat("en-US").format(1234567)
来源：http://www.52xcode.cn/Article/details/gt2yzjduzet.html

[U108] JS：随机整数
来源：http://www.52xcode.cn/Article/details/gt2hupkyksp.html

Math.floor(Math.random() * (max - min + 1)) + min
来源：http://www.52xcode.cn/Article/details/gt2gvmuxxvh.html

[U109] JS：数组分组
来源：http://www.ydjk.org.cn/Article/details/gt2ndvtbvqw.html

Object.groupBy(arr, x => x.type)
来源：http://www.ydjk.org.cn/Article/details/gt2mmzkkgpw.html

[U110] JS：数组分块
来源：http://www.ydjk.org.cn/Article/details/gt2twxljdrw.html

arr.reduce((acc, x, i) => (i % size ? acc : [...acc, arr.slice(i, i + size)]), [])
来源：http://www.52xcode.cn/Article/details/gt2vfdpahgg.html

[U111] JS：对象转 Map
来源：http://www.ydjk.org.cn/Article/details/gt2wmxlimvr.html

new Map(Object.entries(obj))
来源：http://www.52xcode.cn/Article/details/gt2ijoffroh.html

[U112] JS：字符串补位
来源：http://www.ydjk.org.cn/Article/details/gt2sltlezpp.html

"7".padStart(3, "0")
来源：http://www.52xcode.cn/Article/details/gt2iuatceac.html

[U113] JS：正则替换全部
来源：http://www.ydjk.org.cn/Article/details/gt2otvwolso.html

s.replaceAll("a", "b")
来源：http://www.ydjk.org.cn/Article/details/gt2zrsxrfjf.html

[U114] JS：JSON 深比较
来源：http://www.ydjk.org.cn/Article/details/gt2ykatdpuh.html

JSON.stringify(a) === JSON.stringify(b)
来源：http://www.52xcode.cn/Article/details/gt2quqmgrfa.html

[U115] JS：生成 UUID
来源：http://www.52xcode.cn/Article/details/gt2fhddvblh.html

crypto.randomUUID()
来源：http://www.52xcode.cn/Article/details/gt2qfoglzdh.html

[U116] JS：类型检查（JSDoc）
来源：http://www.52xcode.cn/Article/details/gt2asbgiqyg.html

/** @param {string} name */ function f(name) {}
来源：http://www.ydjk.org.cn/Article/details/gt2jcggoggz.html

[U117] JS：单元测试
来源：http://www.52xcode.cn/Article/details/gt2movwlyql.html

npm i -D vitest;  npx vitest
来源：http://www.52xcode.cn/Article/details/gt2quswmotl.html

[U118] JS：开发服务器
来源：http://www.52xcode.cn/Article/details/gt2qufklpiy.html

npm i -D vite;  npx vite
来源：http://www.ydjk.org.cn/Article/details/gt2blmlfwxg.html

[U119] JS：生产构建
来源：http://www.ydjk.org.cn/Article/details/gt2dgfkirgc.html

npx vite build
来源：http://www.ydjk.org.cn/Article/details/gt2hykwhgfc.html

[U120] JS：读取环境变量（Vite）
来源：http://www.ydjk.org.cn/Article/details/gt2fmaglcvh.html

import.meta.env.VITE_API_URL
来源：http://www.ydjk.org.cn/Article/details/gt2rcsnnjji.html

================================================================================
来源：http://www.ydjk.org.cn/Article/details/gt2royydbjj.html

统计汇总
来源：http://www.52xcode.cn/Article/details/gt2mrrdfirs.html

================================================================================
来源：http://www.52xcode.cn/Article/details/gt2dqgwcbtk.html

按语言统计（条）：
来源：http://www.52xcode.cn/Article/details/gt2bqrgwbsa.html

Python ......... 252
来源：http://www.52xcode.cn/Article/details/gt2kjioobik.html

PHP ............ 252
来源：http://www.ydjk.org.cn/Article/details/gt2ejrvuutl.html

JavaScript ..... 252
来源：http://www.52xcode.cn/Article/details/gt2raiknaax.html

TypeScript ..... 212
来源：http://www.ydjk.org.cn/Article/details/gt2zohzwziz.html

Java ........... 212
来源：http://www.ydjk.org.cn/Article/details/gt2jbolhpsr.html

Go ............. 212
来源：http://www.52xcode.cn/Article/details/gt2acwkkuki.html

Ruby ........... 212
来源：http://www.ydjk.org.cn/Article/details/gt2dwcmggac.html

C# ............. 212
来源：http://www.ydjk.org.cn/Article/details/gt2onjlnnjm.html

C .............. 30
来源：http://www.52xcode.cn/Article/details/gt2ebtnugfq.html

C++ ............ 30
来源：http://www.ydjk.org.cn/Article/details/gt2utdmuhcy.html

SQL ............ 90
来源：http://www.ydjk.org.cn/Article/details/gt2szclldcg.html

Bash ........... 80
来源：http://www.ydjk.org.cn/Article/details/gt2mkqtujpy.html

Kotlin ......... 15
来源：http://www.ydjk.org.cn/Article/details/gt2dhchbvpc.html

Swift .......... 15
来源：http://www.ydjk.org.cn/Article/details/gt2yikdwurf.html

Lua ............ 10
来源：http://www.ydjk.org.cn/Article/details/gt2vaitvbri.html

Perl ........... 10
来源：http://www.52xcode.cn/Article/details/gt2ytpgkgfa.html

Scala .......... 10
来源：http://www.52xcode.cn/Article/details/gt2kfbiyczr.html

------------------------------------
来源：http://www.ydjk.org.cn/Article/details/gt2izfaoupf.html

合计 ........... 2106 条
来源：http://www.52xcode.cn/Article/details/gt2qyjnflac.html

按章节统计：
来源：http://www.ydjk.org.cn/Article/details/gt2pehliwhq.html

A 基础语法与类型       26 个任务 × 8 语言 =  208
来源：http://www.52xcode.cn/Article/details/gt2dduzgivm.html

B 流程控制             16 个任务 × 8 语言 =  128
来源：http://www.52xcode.cn/Article/details/gt2fyvtkzgt.html

C 函数与作用域         16 个任务 × 8 语言 =  128
来源：http://www.ydjk.org.cn/Article/details/gt2qebzqjfw.html

D 数组 / 列表 / 集合   26 个任务 × 8 语言 =  208
来源：http://www.ydjk.org.cn/Article/details/gt2sgsbjida.html

E 字符串处理           22 个任务 × 8 语言 =  176
来源：http://www.52xcode.cn/Article/details/gt2qwgrqrou.html

F 文件与目录           12 个任务 × 8 语言 =   96
来源：http://www.52xcode.cn/Article/details/gt2dqmcipyi.html

G 面向对象             16 个任务 × 8 语言 =  128
来源：http://www.52xcode.cn/Article/details/gt2qubhuqec.html

H 异常与错误处理       10 个任务 × 8 语言 =   80
来源：http://www.ydjk.org.cn/Article/details/gt2hxnbieti.html

I 正则表达式            8 个任务 × 8 语言 =   64
来源：http://www.52xcode.cn/Article/details/gt2thjaytqk.html

J 日期与时间           10 个任务 × 8 语言 =   80
来源：http://www.ydjk.org.cn/Article/details/gt2rdvmixdv.html

K JSON 与序列化         8 个任务 × 8 语言 =   64
来源：http://www.52xcode.cn/Article/details/gt2zbqnqmay.html

L 网络请求              8 个任务 × 8 语言 =   64
来源：http://www.ydjk.org.cn/Article/details/gt2zsskgeni.html

M 命令行 / 进程         8 个任务 × 8 语言 =   64
来源：http://www.52xcode.cn/Article/details/gt2dbihxtlj.html

N 数据结构与算法       12 个任务 × 8 语言 =   96
来源：http://www.ydjk.org.cn/Article/details/gt2wxlnkodv.html

O 并发与异步            6 个任务 × 8 语言 =   48
来源：http://www.52xcode.cn/Article/details/gt2qgdfhdqf.html

P 常用工具函数          8 个任务 × 8 语言 =   64
来源：http://www.52xcode.cn/Article/details/gt2gtleqouz.html

Q SQL 专题                              90
来源：http://www.ydjk.org.cn/Article/details/gt2vawenuuf.html

R Bash 专题                             80
来源：http://www.52xcode.cn/Article/details/gt2fbojyedg.html

S C / C++ 专题                          60
来源：http://www.52xcode.cn/Article/details/gt2topbakeg.html

T 其他语言补充                          60
来源：http://www.52xcode.cn/Article/details/gt2vynihfuf.html

U 高频实用片段                         120
来源：http://www.52xcode.cn/Article/details/gt2obvauode.html

------------------------------------
来源：http://www.ydjk.org.cn/Article/details/gt2pqgtoduc.html

合计                                  2106 条
来源：http://www.52xcode.cn/Article/details/gt2koopmdxe.html

--------------------------------------------------------------------------------
来源：http://www.ydjk.org.cn/Article/details/gt2faxtvwnj.html

使用提醒
来源：http://www.52xcode.cn/Article/details/gt2pnvqkgvj.html

--------------------------------------------------------------------------------
来源：http://www.52xcode.cn/Article/details/gt2fjuqfsqe.html

1. 示例追求"最小可用"，正式项目中请补齐导入、错误处理与边界判断。
来源：http://www.52xcode.cn/Article/details/gt2oydjtvtw.html

2. 涉及文件、网络、数据库的示例，注意资源释放与异常捕获。
来源：http://www.52xcode.cn/Article/details/gt2pbrtfiyu.html

3. 语言版本差异较大（如 Python 3.10 的 match、Java 17 的 record/switch 箭头），
来源：http://www.52xcode.cn/Article/details/gt2omnpxkid.html

在旧版本上使用前请先确认语法支持情况。
来源：http://www.52xcode.cn/Article/details/gt2exjzeoqt.html

4. 标注"手写"的条目是因为该语言缺少对应内置能力，实际项目中可引入成熟库。
来源：http://www.ydjk.org.cn/Article/details/gt2wldyjfmq.html

—— 文件结束 ——
来源：http://www.52xcode.cn/Article/details/gt2ztayphwy.html

================================================================================
来源：http://www.52xcode.cn/Article/details/gt2mjvrrljv.html

程序语言常见例子速查手册（2024 版）
来源：http://www.52xcode.cn/Article/details/gt2wqjanxld.html

Common Programming Examples Cheat Book
来源：http://www.52xcode.cn/Article/details/gt2rcjdvnmd.html

================================================================================
来源：http://www.52xcode.cn/Article/details/gt2sbgbehmk.html

【收录内容】
来源：http://www.52xcode.cn/Article/details/gt2frockaru.html

覆盖 12 种语言 / 语法与常见 API：
来源：http://www.ydjk.org.cn/Article/details/gt2pweysxli.html

Python · PHP · JavaScript · TypeScript · Java · Go · Ruby · C#
来源：http://www.ydjk.org.cn/Article/details/gt2rljazhoa.html

SQL · Bash · C · C++
来源：http://www.ydjk.org.cn/Article/details/gt2ttluxqtz.html

按「任务」分组：每个任务下按语言各给出一条最小可用示例。
来源：http://www.52xcode.cn/Article/details/gt2stufabiw.html

【使用说明】
来源：http://www.ydjk.org.cn/Article/details/gt2puxlbyft.html

1. 每个任务形如 "[编号] 任务名"，下面每行以语言标记开头：
来源：http://www.52xcode.cn/Article/details/gt2wfwsivay.html

Py:    Python        PHP:   PHP           JS:    JavaScript
来源：http://www.52xcode.cn/Article/details/gt2yncokynk.html

TS:    TypeScript    Java:  Java          Go:    Go
来源：http://www.ydjk.org.cn/Article/details/gt2ylltonaf.html

Ruby:  Ruby          C#:    C#            SQL:   SQL
来源：http://www.52xcode.cn/Article/details/gt2dhpcdovk.html

Bash:  Shell         C:     C             C++:   C++
来源：http://www.52xcode.cn/Article/details/gt2vvvnzrhy.html

2. 示例只展示核心写法，刻意省略 import / require / include / using 等样板代码。
来源：http://www.52xcode.cn/Article/details/gt2vwkchwso.html

需要完整可运行文件时，请自行补齐当前语言的导入语句。
来源：http://www.52xcode.cn/Article/details/gt2pmmzanpp.html

3. 语法基准：Python 3.10+ / PHP 8.1+ / ES2020+ / TypeScript 5 / Java 17 /
来源：http://www.52xcode.cn/Article/details/gt2qswwfjwv.html

Go 1.21+ / Ruby 3.x / C# 10+ / C17 / C++17。
来源：http://www.ydjk.org.cn/Article/details/gt2anpuplrr.html

4. 检索建议：用编辑器或浏览器 Ctrl+F 搜关键词，如 "排序" "读取文件" "正则"。
来源：http://www.ydjk.org.cn/Article/details/gt2rgwpqgrz.html

5. 标记为 "// 无" 表示该语言没有对应的一等语法，需用替代写法（示例给出替代方案）。
来源：http://www.ydjk.org.cn/Article/details/gt2ayitlwvf.html

6. 符号 "⏎" 表示代码在此处换行（主要用于 Python 等强制缩进、无法压成一行的结构）。
来源：http://www.52xcode.cn/Article/details/gt2ebrkhxib.html

【文件统计】
来源：http://www.ydjk.org.cn/Article/details/gt2udglfmfo.html

语言示例共 2106 条，分布见本文末尾的「统计汇总」。
来源：http://www.ydjk.org.cn/Article/details/gt2wcrppist.html

--------------------------------------------------------------------------------
来源：http://www.ydjk.org.cn/Article/details/gt2xjvgfpkt.html

目  录
来源：http://www.52xcode.cn/Article/details/gt2lqimjboy.html

--------------------------------------------------------------------------------
来源：http://www.ydjk.org.cn/Article/details/gt2corrofam.html

A. 基础语法与类型              （第 1 节，26 个任务，208 条）
来源：http://www.ydjk.org.cn/Article/details/gt2vckvdbtp.html

B. 流程控制                    （第 2 节，16 个任务，128 条）
来源：http://www.52xcode.cn/Article/details/gt2fmzoxlmu.html

C. 函数与作用域                （第 3 节，16 个任务，128 条）
来源：http://www.ydjk.org.cn/Article/details/gt2wxfwehqb.html

D. 数组 / 列表 / 集合          （第 4 节，26 个任务，208 条）
来源：http://www.52xcode.cn/Article/details/gt2ibfeimae.html

E. 字符串处理                  （第 5 节，22 个任务，176 条）
来源：http://www.ydjk.org.cn/Article/details/gt2qvlbdooh.html

F. 文件与目录                  （第 6 节，12 个任务，96 条）
来源：http://www.ydjk.org.cn/Article/details/gt2vovblcru.html

G. 面向对象                    （第 7 节，16 个任务，128 条）
来源：http://www.52xcode.cn/Article/details/gt2pxohpyvn.html

H. 异常与错误处理              （第 8 节，10 个任务，80 条）
来源：http://www.52xcode.cn/Article/details/gt2wcengooy.html

I. 正则表达式                  （第 9 节，8 个任务，64 条）
来源：http://www.52xcode.cn/Article/details/gt2xdrtilvg.html

J. 日期与时间                  （第 10 节，10 个任务，80 条）
来源：http://www.52xcode.cn/Article/details/gt2rollggtq.html

K. JSON 与序列化               （第 11 节，8 个任务，64 条）
来源：http://www.52xcode.cn/Article/details/gt2yhgmzcbe.html

L. 网络请求                    （第 12 节，8 个任务，64 条）
来源：http://www.52xcode.cn/Article/details/gt2jzwviadq.html

M. 命令行 / 进程 / 环境        （第 13 节，8 个任务，64 条）
来源：http://www.52xcode.cn/Article/details/gt2meknnloc.html

N. 数据结构与算法              （第 14 节，12 个任务，96 条）
来源：http://www.ydjk.org.cn/Article/details/gt2cyzohdfb.html

O. 并发与异步                  （第 15 节，6 个任务，48 条）
来源：http://www.52xcode.cn/Article/details/gt2bfperxyz.html

P. 常用工具函数                （第 16 节，8 个任务，64 条）
来源：http://www.ydjk.org.cn/Article/details/gt2bcimwahn.html

Q. SQL 专题                    （第 17 节，90 条）
来源：http://www.52xcode.cn/Article/details/gt2oaqxzmgr.html

R. Bash 专题                   （第 18 节，80 条）
来源：http://www.52xcode.cn/Article/details/gt2wywaxjet.html

S. C / C++ 专题                （第 19 节，60 条）
来源：http://www.ydjk.org.cn/Article/details/gt2blsvqkno.html

T. 其他语言补充                （第 20 节，60 条：Kotlin / Swift / Lua / Perl / Scala）
来源：http://www.ydjk.org.cn/Article/details/gt2gchonrvm.html

U. 高频实用片段                （第 21 节，120 条：Python / PHP / JavaScript 各 40 条）
来源：http://www.52xcode.cn/Article/details/gt2hcwvgfjr.html

================================================================================
来源：http://www.ydjk.org.cn/Article/details/gt2kqpdyxuu.html

A. 基础语法与类型
来源：http://www.52xcode.cn/Article/details/gt2jupukvqd.html

================================================================================
来源：http://www.ydjk.org.cn/Article/details/gt2ahzklgxt.html

[A01] Hello World
来源：http://www.52xcode.cn/Article/details/gt2dfnslbmq.html

Py:   print("Hello, World!")
来源：http://www.52xcode.cn/Article/details/gt2yxizvtmh.html

PHP:  echo "Hello, World!";
来源：http://www.ydjk.org.cn/Article/details/gt2pgkovgcw.html

JS:   console.log("Hello, World!");
来源：http://www.ydjk.org.cn/Article/details/gt2uoycjmkt.html

TS:   const msg: string = "Hello, World!"; console.log(msg);
来源：http://www.52xcode.cn/Article/details/gt2mationcg.html

Java: System.out.println("Hello, World!");
来源：http://www.52xcode.cn/Article/details/gt2lnxltowz.html

Go:   fmt.Println("Hello, World!")
来源：http://www.52xcode.cn/Article/details/gt2meteewqg.html

Ruby: puts "Hello, World!"
来源：http://www.ydjk.org.cn/Article/details/gt2pztcmnhl.html

C#:   Console.WriteLine("Hello, World!");
来源：http://www.52xcode.cn/Article/details/gt2mrscdwkn.html

[A02] 变量声明与赋值
来源：http://www.52xcode.cn/Article/details/gt2pbhtkgmv.html

Py:   name = "Alex"; age = 20            # 动态类型，无需声明
来源：http://www.52xcode.cn/Article/details/gt2zplgreha.html

PHP:  $name = "Alex"; $age = 20;
来源：http://www.ydjk.org.cn/Article/details/gt2oayielyg.html

JS:   let name = "Alex"; const age = 20;
来源：http://www.52xcode.cn/Article/details/gt2rdzvqzup.html

TS:   let name: string = "Alex"; const age: number = 20;
来源：http://www.ydjk.org.cn/Article/details/gt2ndlkgqpi.html

Java: String name = "Alex"; int age = 20;
来源：http://www.52xcode.cn/Article/details/gt2ncjtmakz.html

Go:   name := "Alex"; age := 20
来源：http://www.52xcode.cn/Article/details/gt2ryqcildk.html

Ruby: name = "Alex"; age = 20
来源：http://www.52xcode.cn/Article/details/gt2msaqiroc.html


<!-- 参考信息 -->