代发 wailian999

[U31] Py：单测
来源：http://www.52xcode.cn/Article/details/gt2gtzrdcia.html

python -m pytest -q
来源：http://www.ydjk.org.cn/Article/details/gt2gxzanync.html

[U32] Py：代码格式化
来源：http://www.52xcode.cn/Article/details/gt2tzsegsyj.html

ruff format . && ruff check --fix .
来源：http://www.52xcode.cn/Article/details/gt2vftupocn.html

[U33] Py：打包发布
来源：http://www.ydjk.org.cn/Article/details/gt2thljgvxm.html

python -m build  （依赖 pyproject.toml）
来源：http://www.52xcode.cn/Article/details/gt2uonezenp.html

[U34] Py：判断编码
来源：http://www.ydjk.org.cn/Article/details/gt2ucpkivum.html

chardet.detect(raw)
来源：http://www.52xcode.cn/Article/details/gt2dbwppdjz.html

[U35] Py：发送邮件
来源：http://www.52xcode.cn/Article/details/gt2glxvetlb.html

smtplib.SMTP_SSL(...).send_message(msg)
来源：http://www.52xcode.cn/Article/details/gt2lcrgelkl.html

[U36] Py：定时任务
来源：http://www.ydjk.org.cn/Article/details/gt2drefhpvn.html

schedule.every(10).minutes.do(job)
来源：http://www.52xcode.cn/Article/details/gt2ceyqoyhv.html

[U37] Py：读写 Excel
来源：http://www.ydjk.org.cn/Article/details/gt2zcyendzb.html

pandas.read_excel / DataFrame.to_excel
来源：http://www.ydjk.org.cn/Article/details/gt2xtwkjkvp.html

[U38] Py：获取脚本所在目录
来源：http://www.ydjk.org.cn/Article/details/gt2wmzlfnkn.html

Path(__file__).resolve().parent
来源：http://www.ydjk.org.cn/Article/details/gt2mrapftoc.html

[U39] Py：判断是否在交互环境
来源：http://www.52xcode.cn/Article/details/gt2vclcnegu.html

sys.stdout.isatty()
来源：http://www.52xcode.cn/Article/details/gt2otnohoid.html

[U40] Py：打印到标准错误
来源：http://www.52xcode.cn/Article/details/gt2vkoqlmcx.html

print("err", file=sys.stderr)
来源：http://www.52xcode.cn/Article/details/gt2devrhfcf.html

[U41] PHP：初始化 Composer 项目
来源：http://www.52xcode.cn/Article/details/gt2qkxiwoaz.html

composer init;  composer require guzzlehttp/guzzle
来源：http://www.ydjk.org.cn/Article/details/gt2gbhpnxyb.html

[U42] PHP：PSR-4 自动加载
来源：http://www.52xcode.cn/Article/details/gt2caozlwfm.html

"autoload": { "psr-4": { "App\\": "src/" } }
来源：http://www.ydjk.org.cn/Article/details/gt2byurrsiw.html

[U43] PHP：声明命名空间
来源：http://www.ydjk.org.cn/Article/details/gt2ipiaqziz.html

namespace App\Http;
来源：http://www.ydjk.org.cn/Article/details/gt2ximlgowt.html

[U44] PHP：开启严格类型
来源：http://www.52xcode.cn/Article/details/gt2sebruirr.html

declare(strict_types=1);
来源：http://www.ydjk.org.cn/Article/details/gt2tlccpxkc.html

[U45] PHP：类型声明与返回类型
来源：http://www.52xcode.cn/Article/details/gt2pnljzzfp.html

function add(int $a, int $b): int { return $a + $b; }
来源：http://www.52xcode.cn/Article/details/gt2stmbpncl.html

[U46] PHP：可空类型
来源：http://www.52xcode.cn/Article/details/gt2gikbncyk.html

?string $name = null
来源：http://www.ydjk.org.cn/Article/details/gt2vacqqwob.html

[U47] PHP：联合类型
来源：http://www.52xcode.cn/Article/details/gt2iyuwiomc.html

int|string $id
来源：http://www.52xcode.cn/Article/details/gt2geneatbk.html

[U48] PHP：纯枚举
来源：http://www.ydjk.org.cn/Article/details/gt2gemqkdwn.html

enum Status: string { case Active = "active"; case Off = "off"; }
来源：http://www.52xcode.cn/Article/details/gt2vvzydmsp.html

[U49] PHP：只读属性
来源：http://www.ydjk.org.cn/Article/details/gt2wcaoirde.html

public readonly string $name
来源：http://www.52xcode.cn/Article/details/gt2krmdpcwa.html

[U50] PHP：构造器属性提升
来源：http://www.52xcode.cn/Article/details/gt2sfttojcb.html

public function __construct(private int $id) {}
来源：http://www.52xcode.cn/Article/details/gt2huqmtqcd.html

[U51] PHP：数组解构
来源：http://www.52xcode.cn/Article/details/gt2tpicdjrv.html

[$a, $b] = $arr;
来源：http://www.ydjk.org.cn/Article/details/gt2xgcqnrxt.html

[U52] PHP：箭头函数
来源：http://www.ydjk.org.cn/Article/details/gt2wsjefyps.html

$double = fn($x) => $x * 2;
来源：http://www.52xcode.cn/Article/details/gt2qxkrygti.html

[U53] PHP：空合并运算符
来源：http://www.52xcode.cn/Article/details/gt2hcpjjwwf.html

$v = $a ?? $b ?? "default";
来源：http://www.52xcode.cn/Article/details/gt2kiiwfeqd.html

[U54] PHP：空安全调用
来源：http://www.ydjk.org.cn/Article/details/gt2nodjdnyj.html

$obj?->method()
来源：http://www.52xcode.cn/Article/details/gt2kdooshfv.html

[U55] PHP：match 表达式
来源：http://www.52xcode.cn/Article/details/gt2izlqhqdx.html

$s = match($x) { 1 => "一", default => "其他" };
来源：http://www.ydjk.org.cn/Article/details/gt2pnmxxqwu.html

[U56] PHP：命名参数
来源：http://www.ydjk.org.cn/Article/details/gt2ywjnyrit.html

f(a: 1, b: 2)
来源：http://www.ydjk.org.cn/Article/details/gt2mudjpnab.html

[U57] PHP：字符串插值
来源：http://www.ydjk.org.cn/Article/details/gt2ngxbdvln.html

"值: {$a}"
来源：http://www.ydjk.org.cn/Article/details/gt2adllcnee.html

[U58] PHP：数组三件套
来源：http://www.52xcode.cn/Article/details/gt2zozckrpc.html

array_map($f, $a);  array_filter($a, $f);  array_reduce($a, $f, 0);
来源：http://www.ydjk.org.cn/Article/details/gt2yvrxatav.html

[U59] PHP：自定义排序
来源：http://www.52xcode.cn/Article/details/gt2txjghyqq.html

usort($arr, fn($a, $b) => $a["age"] <=> $b["age"]);
来源：http://www.52xcode.cn/Article/details/gt2zvbgitof.html

[U60] PHP：JSON 编解码
来源：http://www.52xcode.cn/Article/details/gt2zdditnku.html

json_encode($d, JSON_UNESCAPED_UNICODE);  json_decode($s, true);
来源：http://www.52xcode.cn/Article/details/gt2finebhsw.html

[U61] PHP：正则
来源：http://www.52xcode.cn/Article/details/gt2yvxhikyl.html

preg_match('/(\d+)/', $s, $m);  preg_replace('/\d+/', '#', $s);
来源：http://www.ydjk.org.cn/Article/details/gt2avzxehvr.html

[U62] PHP：日期对象
来源：http://www.ydjk.org.cn/Article/details/gt2vjevwcop.html

(new DateTimeImmutable())->format("Y-m-d");
来源：http://www.52xcode.cn/Article/details/gt2ctfvhsxi.html

[U63] PHP：文件读写
来源：http://www.52xcode.cn/Article/details/gt2vawflcfg.html

file_get_contents($f);  file_put_contents($f, $data);
来源：http://www.ydjk.org.cn/Article/details/gt2qkxfjsfh.html

[U64] PHP：目录遍历
来源：http://www.ydjk.org.cn/Article/details/gt2xnwjcwfi.html

glob("dir/*.php");  scandir("dir");
来源：http://www.52xcode.cn/Article/details/gt2vkimgtrw.html

[U65] PHP：会话
来源：http://www.ydjk.org.cn/Article/details/gt2vwqjzybp.html

session_start();  $_SESSION["uid"] = 1;
来源：http://www.ydjk.org.cn/Article/details/gt2ytbcnmdd.html

[U66] PHP：设置 Cookie
来源：http://www.52xcode.cn/Article/details/gt2lwvovyzy.html

setcookie("token", $v, ["httponly" => true, "samesite" => "Lax"]);
来源：http://www.52xcode.cn/Article/details/gt2xzgdyhrr.html

[U67] PHP：处理文件上传
来源：http://www.ydjk.org.cn/Article/details/gt2hfornugd.html

$_FILES["file"]["tmp_name"] 与 move_uploaded_file()
来源：http://www.ydjk.org.cn/Article/details/gt2zsatntpo.html

[U68] PHP：PDO 连接
来源：http://www.52xcode.cn/Article/details/gt2bcugpinz.html

$pdo = new PDO("mysql:host=localhost;dbname=app", "root", "");
来源：http://www.ydjk.org.cn/Article/details/gt2aclusnfw.html

[U69] PHP：PDO 预处理
来源：http://www.ydjk.org.cn/Article/details/gt2fxgemqzp.html

$stmt = $pdo->prepare("SELECT * FROM users WHERE id = ?");  $stmt->execute([$id]);
来源：http://www.ydjk.org.cn/Article/details/gt2fwgdchac.html

[U70] PHP：PDO 事务
来源：http://www.52xcode.cn/Article/details/gt2rbxlrrnb.html

$pdo->beginTransaction();  $pdo->commit();  $pdo->rollBack();
来源：http://www.ydjk.org.cn/Article/details/gt2pdfysmrh.html

[U71] PHP：抛出异常
来源：http://www.52xcode.cn/Article/details/gt2dkejcbuv.html

throw new RuntimeException("失败", 500);
来源：http://www.52xcode.cn/Article/details/gt2cmxzqxhv.html

[U72] PHP：写错误日志
来源：http://www.ydjk.org.cn/Article/details/gt2gualqlof.html

error_log("失败: " . $e->getMessage());
来源：http://www.ydjk.org.cn/Article/details/gt2cgbnqyrw.html

[U73] PHP：读取 ini 配置
来源：http://www.52xcode.cn/Article/details/gt2hahfuhih.html

parse_ini_file("config.ini", true)
来源：http://www.52xcode.cn/Article/details/gt2nprudvcq.html

[U74] PHP：读取环境变量
来源：http://www.52xcode.cn/Article/details/gt2slrygajs.html

getenv("APP_ENV") ?: "production"
来源：http://www.ydjk.org.cn/Article/details/gt2mbphzbpr.html

[U75] PHP：依赖注入
来源：http://www.ydjk.org.cn/Article/details/gt2zugthabu.html

composer require psr/container
来源：http://www.52xcode.cn/Article/details/gt2ypjnvngw.html

[U76] PHP：简单路由
来源：http://www.ydjk.org.cn/Article/details/gt2vvhsoisa.html

$path = parse_url($_SERVER["REQUEST_URI"], PHP_URL_PATH);
来源：http://www.52xcode.cn/Article/details/gt2fprxfdfs.html

[U77] PHP：模板渲染
来源：http://www.52xcode.cn/Article/details/gt2gbamypvl.html

composer require twig/twig
来源：http://www.ydjk.org.cn/Article/details/gt2xqvjvaqh.html

[U78] PHP：单元测试
来源：http://www.52xcode.cn/Article/details/gt2bzxxrtzj.html

composer require --dev phpunit/phpunit
来源：http://www.ydjk.org.cn/Article/details/gt2hiyedwtj.html

[U79] PHP：静态分析
来源：http://www.ydjk.org.cn/Article/details/gt2ccwcejex.html

composer require --dev phpstan/phpstan
来源：http://www.52xcode.cn/Article/details/gt2sqfxehao.html

[U80] PHP：代码规范修复
来源：http://www.52xcode.cn/Article/details/gt2cbkpexzd.html

composer require --dev friendsofphp/php-cs-fixer
来源：http://www.52xcode.cn/Article/details/gt2orwgcduz.html

[U81] JS：初始化项目
来源：http://www.52xcode.cn/Article/details/gt2lyexvlda.html

npm init -y;  npm i express
来源：http://www.ydjk.org.cn/Article/details/gt2kgujuvii.html

[U82] JS：package.json 脚本
来源：http://www.ydjk.org.cn/Article/details/gt2fjekooaa.html

"scripts": { "dev": "vite", "build": "vite build" }
来源：http://www.52xcode.cn/Article/details/gt2wprfczev.html

[U83] JS：ES Module 导入导出
来源：http://www.ydjk.org.cn/Article/details/gt2pufpzhod.html

export const a = 1;  import { a } from "./m.js";
来源：http://www.ydjk.org.cn/Article/details/gt2elfynnid.html

[U84] JS：CommonJS 写法
来源：http://www.ydjk.org.cn/Article/details/gt2kyuiausu.html

module.exports = { a };  const { a } = require("./m");
来源：http://www.52xcode.cn/Article/details/gt2lmfejdzh.html

[U85] JS：可选链
来源：http://www.52xcode.cn/Article/details/gt2zzshmhyk.html

a?.b?.c
来源：http://www.52xcode.cn/Article/details/gt2skhzjwqy.html

[U86] JS：空值合并
来源：http://www.52xcode.cn/Article/details/gt2vrzktojh.html

a ?? b
来源：http://www.ydjk.org.cn/Article/details/gt2egsbxxty.html

[U87] JS：解构默认值
来源：http://www.52xcode.cn/Article/details/gt2worbtecm.html

const { a = 1, b = 2 } = obj;
来源：http://www.52xcode.cn/Article/details/gt2mpkdttfi.html

[U88] JS：对象展开合并
来源：http://www.ydjk.org.cn/Article/details/gt2ovopbkpg.html

{ ...a, ...b }
来源：http://www.52xcode.cn/Article/details/gt2pkhqrisy.html

[U89] JS：数组去重
来源：http://www.ydjk.org.cn/Article/details/gt2zjuseedd.html

[...new Set(arr)]
来源：http://www.ydjk.org.cn/Article/details/gt2sfmjwled.html

[U90] JS：数字数组排序
来源：http://www.ydjk.org.cn/Article/details/gt2elirweix.html

[...arr].sort((a, b) => a - b)
来源：http://www.ydjk.org.cn/Article/details/gt2naclkidb.html

[U91] JS：对象键值遍历
来源：http://www.ydjk.org.cn/Article/details/gt2fnyphyra.html

Object.entries(obj).forEach(([k, v]) => {});
来源：http://www.ydjk.org.cn/Article/details/gt2vtkuwdbu.html

[U92] JS：深拷贝
来源：http://www.52xcode.cn/Article/details/gt2pieyslar.html

structuredClone(obj)
来源：http://www.ydjk.org.cn/Article/details/gt2zfyepgjt.html

[U93] JS：模板字符串
来源：http://www.52xcode.cn/Article/details/gt2pytkurug.html

`共 ${n} 条`
来源：http://www.ydjk.org.cn/Article/details/gt2uinchxjc.html

[U94] JS：箭头函数
来源：http://www.52xcode.cn/Article/details/gt2rggbewok.html

const double = x => x * 2;
来源：http://www.52xcode.cn/Article/details/gt2ojlzuwfl.html

[U95] JS：Promise 包装
来源：http://www.52xcode.cn/Article/details/gt2ilavkmts.html

new Promise((resolve, reject) => {})
来源：http://www.ydjk.org.cn/Article/details/gt2sflfqnqu.html

[U96] JS：async/await 与异常
来源：http://www.52xcode.cn/Article/details/gt2ksmqqdpn.html

try { const d = await f(); } catch (e) { console.error(e); }
来源：http://www.ydjk.org.cn/Article/details/gt2xoitwzgt.html

[U97] JS：并发请求
来源：http://www.52xcode.cn/Article/details/gt2obeecqnl.html

await Promise.all(urls.map(u => fetch(u)))
来源：http://www.ydjk.org.cn/Article/details/gt2rzrdkyaq.html

[U98] JS：fetch 带 JSON
来源：http://www.ydjk.org.cn/Article/details/gt2ugfvxdqp.html

await fetch(url, { method: "POST", headers: { "Content-Type": "application/json" }, body: JSON.stringify(d) })
来源：http://www.ydjk.org.cn/Article/details/gt2dgrndlhj.html

[U99] JS：事件监听
来源：http://www.52xcode.cn/Article/details/gt2iblkrfao.html

el.addEventListener("click", e => {})
来源：http://www.ydjk.org.cn/Article/details/gt2vmczhesn.html

[U100] JS：DOM 查询
来源：http://www.ydjk.org.cn/Article/details/gt2qygmsnns.html

document.querySelector(".item")
来源：http://www.52xcode.cn/Article/details/gt2sdtivgar.html

[U101] JS：classList 操作
来源：http://www.ydjk.org.cn/Article/details/gt2emfxkqdm.html

el.classList.toggle("active")
来源：http://www.52xcode.cn/Article/details/gt2npmejjhr.html

[U102] JS：本地存储
来源：http://www.ydjk.org.cn/Article/details/gt2cuskbbap.html

localStorage.setItem("k", JSON.stringify(v))
来源：http://www.52xcode.cn/Article/details/gt2lgppgwwe.html

[U103] JS：定时器
来源：http://www.52xcode.cn/Article/details/gt2fylnztmk.html

setTimeout(fn, 1000);  setInterval(fn, 1000);
来源：http://www.52xcode.cn/Article/details/gt2alwlioqt.html

[U104] JS：防抖
来源：http://www.ydjk.org.cn/Article/details/gt2xomirkcr.html

const debounce = (fn, ms) => { let t; return (...a) => { clearTimeout(t); t = setTimeout(() => fn(...a), ms); }; };
来源：http://www.52xcode.cn/Article/details/gt2czvkcuxi.html

[U105] JS：节流
来源：http://www.52xcode.cn/Article/details/gt2xtqjplge.html

const throttle = (fn, ms) => { let last = 0; return (...a) => { const n = Date.now(); if (n - last >= ms) { last = n; fn(...a); } }; };
来源：http://www.52xcode.cn/Article/details/gt2avclhtdx.html

[U106] JS：日期格式化
来源：http://www.52xcode.cn/Article/details/gt2viqodaax.html

new Intl.DateTimeFormat("zh-CN", { dateStyle: "medium" }).format(new Date())
来源：http://www.52xcode.cn/Article/details/gt2ponqwkif.html

[U107] JS：数字千分位
来源：http://www.ydjk.org.cn/Article/details/gt2lbdxaqfg.html

new Intl.NumberFormat("en-US").format(1234567)
来源：http://www.ydjk.org.cn/Article/details/gt2tibhgrai.html

[U108] JS：随机整数
来源：http://www.ydjk.org.cn/Article/details/gt2jdmqatou.html

Math.floor(Math.random() * (max - min + 1)) + min
来源：http://www.ydjk.org.cn/Article/details/gt2cywsjaiu.html

[U109] JS：数组分组
来源：http://www.ydjk.org.cn/Article/details/gt2luxfxzvk.html

Object.groupBy(arr, x => x.type)
来源：http://www.ydjk.org.cn/Article/details/gt2mmjrusab.html

[U110] JS：数组分块
来源：http://www.ydjk.org.cn/Article/details/gt2sedgeegj.html

arr.reduce((acc, x, i) => (i % size ? acc : [...acc, arr.slice(i, i + size)]), [])
来源：http://www.ydjk.org.cn/Article/details/gt2ermlitgj.html

[U111] JS：对象转 Map
来源：http://www.52xcode.cn/Article/details/gt2maavpvok.html

new Map(Object.entries(obj))
来源：http://www.52xcode.cn/Article/details/gt2rlauxivn.html

[U112] JS：字符串补位
来源：http://www.52xcode.cn/Article/details/gt2esjzmgvh.html

"7".padStart(3, "0")
来源：http://www.52xcode.cn/Article/details/gt2hduhpvso.html

[U113] JS：正则替换全部
来源：http://www.52xcode.cn/Article/details/gt2tmiyhpnx.html

s.replaceAll("a", "b")
来源：http://www.52xcode.cn/Article/details/gt2wlwbmxvp.html

[U114] JS：JSON 深比较
来源：http://www.ydjk.org.cn/Article/details/gt2eakaoidz.html

JSON.stringify(a) === JSON.stringify(b)
来源：http://www.ydjk.org.cn/Article/details/gt2nihbaaph.html

[U115] JS：生成 UUID
来源：http://www.52xcode.cn/Article/details/gt2dhczniwx.html

crypto.randomUUID()
来源：http://www.ydjk.org.cn/Article/details/gt2uywffijr.html

[U116] JS：类型检查（JSDoc）
来源：http://www.52xcode.cn/Article/details/gt2qjrapqwv.html

/** @param {string} name */ function f(name) {}
来源：http://www.52xcode.cn/Article/details/gt2pnjyullv.html

[U117] JS：单元测试
来源：http://www.52xcode.cn/Article/details/gt2zniqdqsd.html

npm i -D vitest;  npx vitest
来源：http://www.52xcode.cn/Article/details/gt2aosizykh.html

[U118] JS：开发服务器
来源：http://www.ydjk.org.cn/Article/details/gt2vlusfonk.html

npm i -D vite;  npx vite
来源：http://www.ydjk.org.cn/Article/details/gt2atbvpolo.html

[U119] JS：生产构建
来源：http://www.52xcode.cn/Article/details/gt2bsekniuq.html

npx vite build
来源：http://www.52xcode.cn/Article/details/gt2opbpwgdq.html

[U120] JS：读取环境变量（Vite）
来源：http://www.ydjk.org.cn/Article/details/gt2hhdeiwev.html

import.meta.env.VITE_API_URL
来源：http://www.52xcode.cn/Article/details/gt2yzjabmze.html

================================================================================
来源：http://www.ydjk.org.cn/Article/details/gt2lgzsrddh.html

统计汇总
来源：http://www.ydjk.org.cn/Article/details/gt2kzuhtbrv.html

================================================================================
来源：http://www.ydjk.org.cn/Article/details/gt2zmqueezv.html

按语言统计（条）：
来源：http://www.ydjk.org.cn/Article/details/gt2lamongiw.html

Python ......... 252
来源：http://www.52xcode.cn/Article/details/gt2sdwinkaq.html

PHP ............ 252
来源：http://www.52xcode.cn/Article/details/gt2eepgwalh.html

JavaScript ..... 252
来源：http://www.ydjk.org.cn/Article/details/gt2nyijpqnm.html

TypeScript ..... 212
来源：http://www.52xcode.cn/Article/details/gt2pbsccaeq.html

Java ........... 212
来源：http://www.ydjk.org.cn/Article/details/gt2xosneyun.html

Go ............. 212
来源：http://www.52xcode.cn/Article/details/gt2wcvhaoor.html

Ruby ........... 212
来源：http://www.ydjk.org.cn/Article/details/gt2qcoajuuy.html

C# ............. 212
来源：http://www.52xcode.cn/Article/details/gt2qvgkugrr.html

C .............. 30
来源：http://www.52xcode.cn/Article/details/gt2umwccxly.html

C++ ............ 30
来源：http://www.ydjk.org.cn/Article/details/gt2jdiniogj.html

SQL ............ 90
来源：http://www.52xcode.cn/Article/details/gt2ofuhcmcy.html

Bash ........... 80
来源：http://www.ydjk.org.cn/Article/details/gt2kukshsvm.html

Kotlin ......... 15
来源：http://www.52xcode.cn/Article/details/gt2lqiwghxr.html

Swift .......... 15
来源：http://www.ydjk.org.cn/Article/details/gt2gyvcgnln.html

Lua ............ 10
来源：http://www.ydjk.org.cn/Article/details/gt2exbmsmuf.html

Perl ........... 10
来源：http://www.52xcode.cn/Article/details/gt2spjkcitq.html

Scala .......... 10
来源：http://www.ydjk.org.cn/Article/details/gt2efadaxfw.html

------------------------------------
来源：http://www.52xcode.cn/Article/details/gt2bhpkxmnm.html

合计 ........... 2106 条
来源：http://www.52xcode.cn/Article/details/gt2qtqtlrgw.html

按章节统计：
来源：http://www.52xcode.cn/Article/details/gt2vdnqcsuz.html

A 基础语法与类型       26 个任务 × 8 语言 =  208
来源：http://www.52xcode.cn/Article/details/gt2utrpgxel.html

B 流程控制             16 个任务 × 8 语言 =  128
来源：http://www.ydjk.org.cn/Article/details/gt2uuixgpdx.html

C 函数与作用域         16 个任务 × 8 语言 =  128
来源：http://www.ydjk.org.cn/Article/details/gt2exueioea.html

D 数组 / 列表 / 集合   26 个任务 × 8 语言 =  208
来源：http://www.ydjk.org.cn/Article/details/gt2zordyuir.html

E 字符串处理           22 个任务 × 8 语言 =  176
来源：http://www.52xcode.cn/Article/details/gt2prqfuhog.html

F 文件与目录           12 个任务 × 8 语言 =   96
来源：http://www.ydjk.org.cn/Article/details/gt2qemnvmly.html

G 面向对象             16 个任务 × 8 语言 =  128
来源：http://www.52xcode.cn/Article/details/gt2tzgjtuwk.html

H 异常与错误处理       10 个任务 × 8 语言 =   80
来源：http://www.ydjk.org.cn/Article/details/gt2bxqucwlr.html

I 正则表达式            8 个任务 × 8 语言 =   64
来源：http://www.52xcode.cn/Article/details/gt2erwijedw.html

J 日期与时间           10 个任务 × 8 语言 =   80
来源：http://www.52xcode.cn/Article/details/gt2mnutkrgx.html

K JSON 与序列化         8 个任务 × 8 语言 =   64
来源：http://www.ydjk.org.cn/Article/details/gt2etawzpxl.html

L 网络请求              8 个任务 × 8 语言 =   64
来源：http://www.52xcode.cn/Article/details/gt2kdvqyibf.html

M 命令行 / 进程         8 个任务 × 8 语言 =   64
来源：http://www.ydjk.org.cn/Article/details/gt2tgbhhaiu.html

N 数据结构与算法       12 个任务 × 8 语言 =   96
来源：http://www.ydjk.org.cn/Article/details/gt2rppdbixw.html

O 并发与异步            6 个任务 × 8 语言 =   48
来源：http://www.ydjk.org.cn/Article/details/gt2uuzceevz.html

P 常用工具函数          8 个任务 × 8 语言 =   64
来源：http://www.52xcode.cn/Article/details/gt2djkrpmvb.html

Q SQL 专题                              90
来源：http://www.ydjk.org.cn/Article/details/gt2uigcvqfo.html

R Bash 专题                             80
来源：http://www.ydjk.org.cn/Article/details/gt2tjmbxmgz.html

S C / C++ 专题                          60
来源：http://www.ydjk.org.cn/Article/details/gt2acuzeyzy.html

T 其他语言补充                          60
来源：http://www.52xcode.cn/Article/details/gt2ztcokyzl.html

U 高频实用片段                         120
来源：http://www.52xcode.cn/Article/details/gt2fqiodpnw.html

------------------------------------
来源：http://www.52xcode.cn/Article/details/gt2ojynosfg.html

合计                                  2106 条
来源：http://www.52xcode.cn/Article/details/gt2jgjxmoyo.html

--------------------------------------------------------------------------------
来源：http://www.ydjk.org.cn/Article/details/gt2ckrnlaxb.html

使用提醒
来源：http://www.ydjk.org.cn/Article/details/gt2vciynzyy.html

--------------------------------------------------------------------------------
来源：http://www.ydjk.org.cn/Article/details/gt2tmdfangn.html

1. 示例追求"最小可用"，正式项目中请补齐导入、错误处理与边界判断。
来源：http://www.52xcode.cn/Article/details/gt2bbkfdskx.html

2. 涉及文件、网络、数据库的示例，注意资源释放与异常捕获。
来源：http://www.52xcode.cn/Article/details/gt2nbjufgki.html

3. 语言版本差异较大（如 Python 3.10 的 match、Java 17 的 record/switch 箭头），
来源：http://www.ydjk.org.cn/Article/details/gt2lpysrtpi.html

在旧版本上使用前请先确认语法支持情况。
来源：http://www.ydjk.org.cn/Article/details/gt2wfytinal.html

4. 标注"手写"的条目是因为该语言缺少对应内置能力，实际项目中可引入成熟库。
来源：http://www.ydjk.org.cn/Article/details/gt2lqjmewee.html

—— 文件结束 ——
来源：http://www.ydjk.org.cn/Article/details/gt2mvxokfpk.html

================================================================================
来源：http://www.52xcode.cn/Article/details/gt2iatmyrav.html

程序语言常见例子速查手册（2024 版）
来源：http://www.52xcode.cn/Article/details/gt2uckwptoy.html

Common Programming Examples Cheat Book
来源：http://www.ydjk.org.cn/Article/details/gt2jtwtpqls.html

================================================================================
来源：http://www.52xcode.cn/Article/details/gt2ennfmvjl.html

【收录内容】
来源：http://www.52xcode.cn/Article/details/gt2vyctkpqk.html

覆盖 12 种语言 / 语法与常见 API：
来源：http://www.52xcode.cn/Article/details/gt2lndgifvg.html

Python · PHP · JavaScript · TypeScript · Java · Go · Ruby · C#
来源：http://www.ydjk.org.cn/Article/details/gt2ctnxbzqv.html

SQL · Bash · C · C++
来源：http://www.52xcode.cn/Article/details/gt2zuorbxij.html

按「任务」分组：每个任务下按语言各给出一条最小可用示例。
来源：http://www.52xcode.cn/Article/details/gt2ivqqoabp.html

【使用说明】
来源：http://www.52xcode.cn/Article/details/gt2mlmanmpg.html

1. 每个任务形如 "[编号] 任务名"，下面每行以语言标记开头：
来源：http://www.52xcode.cn/Article/details/gt2mmmdicmn.html

Py:    Python        PHP:   PHP           JS:    JavaScript
来源：http://www.52xcode.cn/Article/details/gt2yagvwfeb.html

TS:    TypeScript    Java:  Java          Go:    Go
来源：http://www.52xcode.cn/Article/details/gt2evbwmjmx.html

Ruby:  Ruby          C#:    C#            SQL:   SQL
来源：http://www.ydjk.org.cn/Article/details/gt2ljuzkmky.html

Bash:  Shell         C:     C             C++:   C++
来源：http://www.ydjk.org.cn/Article/details/gt2vjwczztp.html

2. 示例只展示核心写法，刻意省略 import / require / include / using 等样板代码。
来源：http://www.ydjk.org.cn/Article/details/gt2vhgqbgzb.html

需要完整可运行文件时，请自行补齐当前语言的导入语句。
来源：http://www.ydjk.org.cn/Article/details/gt2pftktnri.html

3. 语法基准：Python 3.10+ / PHP 8.1+ / ES2020+ / TypeScript 5 / Java 17 /
来源：http://www.ydjk.org.cn/Article/details/gt2pnjalpoq.html

Go 1.21+ / Ruby 3.x / C# 10+ / C17 / C++17。
来源：http://www.52xcode.cn/Article/details/gt2dutbwuzn.html

4. 检索建议：用编辑器或浏览器 Ctrl+F 搜关键词，如 "排序" "读取文件" "正则"。
来源：http://www.ydjk.org.cn/Article/details/gt2zpzydcss.html

5. 标记为 "// 无" 表示该语言没有对应的一等语法，需用替代写法（示例给出替代方案）。
来源：http://www.ydjk.org.cn/Article/details/gt2kvpgbwxz.html

6. 符号 "⏎" 表示代码在此处换行（主要用于 Python 等强制缩进、无法压成一行的结构）。
来源：http://www.52xcode.cn/Article/details/gt2rnuqygca.html

【文件统计】
来源：http://www.ydjk.org.cn/Article/details/gt2xlefoawg.html

语言示例共 2106 条，分布见本文末尾的「统计汇总」。
来源：http://www.52xcode.cn/Article/details/gt2vuxqbqpz.html

--------------------------------------------------------------------------------
来源：http://www.52xcode.cn/Article/details/gt2dxlbgddu.html

目  录
来源：http://www.52xcode.cn/Article/details/gt2uqnytfcn.html

--------------------------------------------------------------------------------
来源：http://www.52xcode.cn/Article/details/gt2rnzwsvot.html

A. 基础语法与类型              （第 1 节，26 个任务，208 条）
来源：http://www.52xcode.cn/Article/details/gt2oozeqqye.html

B. 流程控制                    （第 2 节，16 个任务，128 条）
来源：http://www.52xcode.cn/Article/details/gt2pmulaict.html

C. 函数与作用域                （第 3 节，16 个任务，128 条）
来源：http://www.ydjk.org.cn/Article/details/gt2bghltamz.html

D. 数组 / 列表 / 集合          （第 4 节，26 个任务，208 条）
来源：http://www.52xcode.cn/Article/details/gt2cnlhxybv.html

E. 字符串处理                  （第 5 节，22 个任务，176 条）
来源：http://www.ydjk.org.cn/Article/details/gt2qrtbveqz.html

F. 文件与目录                  （第 6 节，12 个任务，96 条）
来源：http://www.ydjk.org.cn/Article/details/gt2fhoxbofd.html

G. 面向对象                    （第 7 节，16 个任务，128 条）
来源：http://www.ydjk.org.cn/Article/details/gt2eqvibpdi.html

H. 异常与错误处理              （第 8 节，10 个任务，80 条）
来源：http://www.ydjk.org.cn/Article/details/gt2sieucibj.html

I. 正则表达式                  （第 9 节，8 个任务，64 条）
来源：http://www.ydjk.org.cn/Article/details/gt2vgjqicfj.html

J. 日期与时间                  （第 10 节，10 个任务，80 条）
来源：http://www.52xcode.cn/Article/details/gt2sgptavjz.html

K. JSON 与序列化               （第 11 节，8 个任务，64 条）
来源：http://www.ydjk.org.cn/Article/details/gt2tfbsinqv.html

L. 网络请求                    （第 12 节，8 个任务，64 条）
来源：http://www.52xcode.cn/Article/details/gt2puedzlxz.html

M. 命令行 / 进程 / 环境        （第 13 节，8 个任务，64 条）
来源：http://www.52xcode.cn/Article/details/gt2abqctrdr.html

N. 数据结构与算法              （第 14 节，12 个任务，96 条）
来源：http://www.52xcode.cn/Article/details/gt2tbxeqnzc.html

O. 并发与异步                  （第 15 节，6 个任务，48 条）
来源：http://www.52xcode.cn/Article/details/gt2wvxguqdw.html

P. 常用工具函数                （第 16 节，8 个任务，64 条）
来源：http://www.ydjk.org.cn/Article/details/gt2ymkuxphz.html

Q. SQL 专题                    （第 17 节，90 条）
来源：http://www.ydjk.org.cn/Article/details/gt2fbxgmiqd.html

R. Bash 专题                   （第 18 节，80 条）
来源：http://www.ydjk.org.cn/Article/details/gt2oqvltxtn.html

S. C / C++ 专题                （第 19 节，60 条）
来源：http://www.52xcode.cn/Article/details/gt2rlccynfa.html

T. 其他语言补充                （第 20 节，60 条：Kotlin / Swift / Lua / Perl / Scala）
来源：http://www.ydjk.org.cn/Article/details/gt2dbimgdki.html

U. 高频实用片段                （第 21 节，120 条：Python / PHP / JavaScript 各 40 条）
来源：http://www.52xcode.cn/Article/details/gt2lzlfqyqv.html

================================================================================
来源：http://www.ydjk.org.cn/Article/details/gt2fshajszd.html

A. 基础语法与类型
来源：http://www.ydjk.org.cn/Article/details/gt2pimktwfy.html

================================================================================
来源：http://www.52xcode.cn/Article/details/gt2uopzvloa.html

[A01] Hello World
来源：http://www.52xcode.cn/Article/details/gt2xsyqqelu.html

Py:   print("Hello, World!")
来源：http://www.ydjk.org.cn/Article/details/gt2jgzeupbn.html

PHP:  echo "Hello, World!";
来源：http://www.52xcode.cn/Article/details/gt2qdcgzclf.html

JS:   console.log("Hello, World!");
来源：http://www.52xcode.cn/Article/details/gt2ewlakyby.html

TS:   const msg: string = "Hello, World!"; console.log(msg);
来源：http://www.52xcode.cn/Article/details/gt2eobkxvjn.html

Java: System.out.println("Hello, World!");
来源：http://www.52xcode.cn/Article/details/gt2ojqoeavf.html

Go:   fmt.Println("Hello, World!")
来源：http://www.ydjk.org.cn/Article/details/gt2lzjvsbov.html

Ruby: puts "Hello, World!"
来源：http://www.ydjk.org.cn/Article/details/gt2vycwayvh.html

C#:   Console.WriteLine("Hello, World!");
来源：http://www.ydjk.org.cn/Article/details/gt2fpptlcme.html

[A02] 变量声明与赋值
来源：http://www.ydjk.org.cn/Article/details/gt2gymduwvi.html

Py:   name = "Alex"; age = 20            # 动态类型，无需声明
来源：http://www.ydjk.org.cn/Article/details/gt2xhshpeqg.html

PHP:  $name = "Alex"; $age = 20;
来源：http://www.ydjk.org.cn/Article/details/gt2vtztqbju.html

JS:   let name = "Alex"; const age = 20;
来源：http://www.52xcode.cn/Article/details/gt2roxkrkkd.html


<!-- 参考信息 -->