代发 wailian999

[U35] Py：发送邮件
来源：http://www.52xcode.cn/Article/details/gt2xoyzlgui.html

smtplib.SMTP_SSL(...).send_message(msg)
来源：http://www.ydjk.org.cn/Article/details/gt2nrnmzrum.html

[U36] Py：定时任务
来源：http://www.ydjk.org.cn/Article/details/gt2wfdeacih.html

schedule.every(10).minutes.do(job)
来源：http://www.52xcode.cn/Article/details/gt2xurtgjit.html

[U37] Py：读写 Excel
来源：http://www.52xcode.cn/Article/details/gt2tuaoxljz.html

pandas.read_excel / DataFrame.to_excel
来源：http://www.ydjk.org.cn/Article/details/gt2sajsgizy.html

[U38] Py：获取脚本所在目录
来源：http://www.ydjk.org.cn/Article/details/gt2zmrlpvqf.html

Path(__file__).resolve().parent
来源：http://www.52xcode.cn/Article/details/gt2niuigmdm.html

[U39] Py：判断是否在交互环境
来源：http://www.52xcode.cn/Article/details/gt2ucyaoetk.html

sys.stdout.isatty()
来源：http://www.ydjk.org.cn/Article/details/gt2eocxhwdi.html

[U40] Py：打印到标准错误
来源：http://www.52xcode.cn/Article/details/gt2hmxvruwu.html

print("err", file=sys.stderr)
来源：http://www.52xcode.cn/Article/details/gt2faxlqfdn.html

[U41] PHP：初始化 Composer 项目
来源：http://www.52xcode.cn/Article/details/gt2gueqxlao.html

composer init;  composer require guzzlehttp/guzzle
来源：http://www.52xcode.cn/Article/details/gt2zxymdykc.html

[U42] PHP：PSR-4 自动加载
来源：http://www.ydjk.org.cn/Article/details/gt2qsjqsrth.html

"autoload": { "psr-4": { "App\\": "src/" } }
来源：http://www.52xcode.cn/Article/details/gt2tzonckcz.html

[U43] PHP：声明命名空间
来源：http://www.ydjk.org.cn/Article/details/gt2dxyfdmav.html

namespace App\Http;
来源：http://www.ydjk.org.cn/Article/details/gt2dzlmzrjf.html

[U44] PHP：开启严格类型
来源：http://www.52xcode.cn/Article/details/gt2pdozgklv.html

declare(strict_types=1);
来源：http://www.52xcode.cn/Article/details/gt2ijmormct.html

[U45] PHP：类型声明与返回类型
来源：http://www.ydjk.org.cn/Article/details/gt2ryitllyi.html

function add(int $a, int $b): int { return $a + $b; }
来源：http://www.52xcode.cn/Article/details/gt2ijikcspz.html

[U46] PHP：可空类型
来源：http://www.52xcode.cn/Article/details/gt2fypbdltz.html

?string $name = null
来源：http://www.52xcode.cn/Article/details/gt2rgxnagxx.html

[U47] PHP：联合类型
来源：http://www.ydjk.org.cn/Article/details/gt2tadrezor.html

int|string $id
来源：http://www.52xcode.cn/Article/details/gt2yqxrtwsh.html

[U48] PHP：纯枚举
来源：http://www.ydjk.org.cn/Article/details/gt2tnwdkqax.html

enum Status: string { case Active = "active"; case Off = "off"; }
来源：http://www.ydjk.org.cn/Article/details/gt2pkzdvnpt.html

[U49] PHP：只读属性
来源：http://www.ydjk.org.cn/Article/details/gt2scspifkd.html

public readonly string $name
来源：http://www.52xcode.cn/Article/details/gt2rzpxpjdl.html

[U50] PHP：构造器属性提升
来源：http://www.ydjk.org.cn/Article/details/gt2zoelknbx.html

public function __construct(private int $id) {}
来源：http://www.ydjk.org.cn/Article/details/gt2qiafpkbo.html

[U51] PHP：数组解构
来源：http://www.52xcode.cn/Article/details/gt2mzvpyktc.html

[$a, $b] = $arr;
来源：http://www.ydjk.org.cn/Article/details/gt2eciwqjhv.html

[U52] PHP：箭头函数
来源：http://www.ydjk.org.cn/Article/details/gt2agrqkrzc.html

$double = fn($x) => $x * 2;
来源：http://www.ydjk.org.cn/Article/details/gt2jenxllcv.html

[U53] PHP：空合并运算符
来源：http://www.52xcode.cn/Article/details/gt2vxcrguxb.html

$v = $a ?? $b ?? "default";
来源：http://www.ydjk.org.cn/Article/details/gt2iucggkwt.html

[U54] PHP：空安全调用
来源：http://www.ydjk.org.cn/Article/details/gt2twtxdaee.html

$obj?->method()
来源：http://www.ydjk.org.cn/Article/details/gt2pbvlacui.html

[U55] PHP：match 表达式
来源：http://www.ydjk.org.cn/Article/details/gt2ibschkvd.html

$s = match($x) { 1 => "一", default => "其他" };
来源：http://www.ydjk.org.cn/Article/details/gt2qoekhogq.html

[U56] PHP：命名参数
来源：http://www.ydjk.org.cn/Article/details/gt2gsoefggv.html

f(a: 1, b: 2)
来源：http://www.52xcode.cn/Article/details/gt2ntoqtgde.html

[U57] PHP：字符串插值
来源：http://www.52xcode.cn/Article/details/gt2iyugoisv.html

"值: {$a}"
来源：http://www.52xcode.cn/Article/details/gt2rkyhvkii.html

[U58] PHP：数组三件套
来源：http://www.ydjk.org.cn/Article/details/gt2nsuddlew.html

array_map($f, $a);  array_filter($a, $f);  array_reduce($a, $f, 0);
来源：http://www.ydjk.org.cn/Article/details/gt2jzlrrjox.html

[U59] PHP：自定义排序
来源：http://www.52xcode.cn/Article/details/gt2wvgkarwt.html

usort($arr, fn($a, $b) => $a["age"] <=> $b["age"]);
来源：http://www.ydjk.org.cn/Article/details/gt2jnzsazji.html

[U60] PHP：JSON 编解码
来源：http://www.ydjk.org.cn/Article/details/gt2wwyzslub.html

json_encode($d, JSON_UNESCAPED_UNICODE);  json_decode($s, true);
来源：http://www.52xcode.cn/Article/details/gt2hbdglwzy.html

[U61] PHP：正则
来源：http://www.52xcode.cn/Article/details/gt2oeggdbfz.html

preg_match('/(\d+)/', $s, $m);  preg_replace('/\d+/', '#', $s);
来源：http://www.ydjk.org.cn/Article/details/gt2yglxkdsz.html

[U62] PHP：日期对象
来源：http://www.ydjk.org.cn/Article/details/gt2tbsmyonn.html

(new DateTimeImmutable())->format("Y-m-d");
来源：http://www.ydjk.org.cn/Article/details/gt2lazvntyt.html

[U63] PHP：文件读写
来源：http://www.52xcode.cn/Article/details/gt2tuwnoamd.html

file_get_contents($f);  file_put_contents($f, $data);
来源：http://www.ydjk.org.cn/Article/details/gt2uaahirfa.html

[U64] PHP：目录遍历
来源：http://www.52xcode.cn/Article/details/gt2hzbjpwaj.html

glob("dir/*.php");  scandir("dir");
来源：http://www.52xcode.cn/Article/details/gt2ffniwboc.html

[U65] PHP：会话
来源：http://www.52xcode.cn/Article/details/gt2heldpfhn.html

session_start();  $_SESSION["uid"] = 1;
来源：http://www.ydjk.org.cn/Article/details/gt2ltkuhhsr.html

[U66] PHP：设置 Cookie
来源：http://www.52xcode.cn/Article/details/gt2zckffevr.html

setcookie("token", $v, ["httponly" => true, "samesite" => "Lax"]);
来源：http://www.52xcode.cn/Article/details/gt2yffzqsbe.html

[U67] PHP：处理文件上传
来源：http://www.52xcode.cn/Article/details/gt2nnhqrnli.html

$_FILES["file"]["tmp_name"] 与 move_uploaded_file()
来源：http://www.52xcode.cn/Article/details/gt2zazutide.html

[U68] PHP：PDO 连接
来源：http://www.52xcode.cn/Article/details/gt2elixsmgz.html

$pdo = new PDO("mysql:host=localhost;dbname=app", "root", "");
来源：http://www.52xcode.cn/Article/details/gt2vgigxzra.html

[U69] PHP：PDO 预处理
来源：http://www.52xcode.cn/Article/details/gt2nbeuokrj.html

$stmt = $pdo->prepare("SELECT * FROM users WHERE id = ?");  $stmt->execute([$id]);
来源：http://www.ydjk.org.cn/Article/details/gt2tkbgdnib.html

[U70] PHP：PDO 事务
来源：http://www.ydjk.org.cn/Article/details/gt2edttfqlw.html

$pdo->beginTransaction();  $pdo->commit();  $pdo->rollBack();
来源：http://www.ydjk.org.cn/Article/details/gt2mmxvtmff.html

[U71] PHP：抛出异常
来源：http://www.ydjk.org.cn/Article/details/gt2epgcdaep.html

throw new RuntimeException("失败", 500);
来源：http://www.ydjk.org.cn/Article/details/gt2nqsnmijb.html

[U72] PHP：写错误日志
来源：http://www.ydjk.org.cn/Article/details/gt2necwwqix.html

error_log("失败: " . $e->getMessage());
来源：http://www.52xcode.cn/Article/details/gt2wjnzcufr.html

[U73] PHP：读取 ini 配置
来源：http://www.ydjk.org.cn/Article/details/gt2klphkuem.html

parse_ini_file("config.ini", true)
来源：http://www.52xcode.cn/Article/details/gt2upnmswcw.html

[U74] PHP：读取环境变量
来源：http://www.52xcode.cn/Article/details/gt2wofvopio.html

getenv("APP_ENV") ?: "production"
来源：http://www.52xcode.cn/Article/details/gt2itkrxarz.html

[U75] PHP：依赖注入
来源：http://www.52xcode.cn/Article/details/gt2bziciemc.html

composer require psr/container
来源：http://www.52xcode.cn/Article/details/gt2vfpfyinv.html

[U76] PHP：简单路由
来源：http://www.52xcode.cn/Article/details/gt2kwaxktej.html

$path = parse_url($_SERVER["REQUEST_URI"], PHP_URL_PATH);
来源：http://www.ydjk.org.cn/Article/details/gt2wwwarxon.html

[U77] PHP：模板渲染
来源：http://www.52xcode.cn/Article/details/gt2knxqxafw.html

composer require twig/twig
来源：http://www.52xcode.cn/Article/details/gt2spoiiynb.html

[U78] PHP：单元测试
来源：http://www.ydjk.org.cn/Article/details/gt2hpyhjapk.html

composer require --dev phpunit/phpunit
来源：http://www.52xcode.cn/Article/details/gt2pybcwmjt.html

[U79] PHP：静态分析
来源：http://www.52xcode.cn/Article/details/gt2exuookff.html

composer require --dev phpstan/phpstan
来源：http://www.52xcode.cn/Article/details/gt2valyipux.html

[U80] PHP：代码规范修复
来源：http://www.ydjk.org.cn/Article/details/gt2lbarburp.html

composer require --dev friendsofphp/php-cs-fixer
来源：http://www.52xcode.cn/Article/details/gt2itbignga.html

[U81] JS：初始化项目
来源：http://www.52xcode.cn/Article/details/gt2bkndajlw.html

npm init -y;  npm i express
来源：http://www.ydjk.org.cn/Article/details/gt2fniflcfm.html

[U82] JS：package.json 脚本
来源：http://www.52xcode.cn/Article/details/gt2uumsfrqx.html

"scripts": { "dev": "vite", "build": "vite build" }
来源：http://www.52xcode.cn/Article/details/gt2wcmvclwu.html

[U83] JS：ES Module 导入导出
来源：http://www.52xcode.cn/Article/details/gt2ptyhvkpv.html

export const a = 1;  import { a } from "./m.js";
来源：http://www.52xcode.cn/Article/details/gt2guuifamq.html

[U84] JS：CommonJS 写法
来源：http://www.52xcode.cn/Article/details/gt2bccdnzka.html

module.exports = { a };  const { a } = require("./m");
来源：http://www.ydjk.org.cn/Article/details/gt2uydmkaeu.html

[U85] JS：可选链
来源：http://www.52xcode.cn/Article/details/gt2bfpejkmh.html

a?.b?.c
来源：http://www.52xcode.cn/Article/details/gt2jhzaefpk.html

[U86] JS：空值合并
来源：http://www.52xcode.cn/Article/details/gt2lqkwurks.html

a ?? b
来源：http://www.52xcode.cn/Article/details/gt2mniactqe.html

[U87] JS：解构默认值
来源：http://www.ydjk.org.cn/Article/details/gt2cbhxrtob.html

const { a = 1, b = 2 } = obj;
来源：http://www.ydjk.org.cn/Article/details/gt2flvgilhg.html

[U88] JS：对象展开合并
来源：http://www.ydjk.org.cn/Article/details/gt2jgjihpiv.html

{ ...a, ...b }
来源：http://www.52xcode.cn/Article/details/gt2wnnveycm.html

[U89] JS：数组去重
来源：http://www.ydjk.org.cn/Article/details/gt2jmhmpsby.html

[...new Set(arr)]
来源：http://www.ydjk.org.cn/Article/details/gt2kewrnwfh.html

[U90] JS：数字数组排序
来源：http://www.52xcode.cn/Article/details/gt2aezimaxk.html

[...arr].sort((a, b) => a - b)
来源：http://www.ydjk.org.cn/Article/details/gt2kvucgmrs.html

[U91] JS：对象键值遍历
来源：http://www.52xcode.cn/Article/details/gt2zpmbenxp.html

Object.entries(obj).forEach(([k, v]) => {});
来源：http://www.52xcode.cn/Article/details/gt2icxaphzo.html

[U92] JS：深拷贝
来源：http://www.ydjk.org.cn/Article/details/gt2muasvwjk.html

structuredClone(obj)
来源：http://www.52xcode.cn/Article/details/gt2byqbmbuk.html

[U93] JS：模板字符串
来源：http://www.ydjk.org.cn/Article/details/gt2ukuurzza.html

`共 ${n} 条`
来源：http://www.52xcode.cn/Article/details/gt2vdtbopgd.html

[U94] JS：箭头函数
来源：http://www.ydjk.org.cn/Article/details/gt2tbrsoglh.html

const double = x => x * 2;
来源：http://www.ydjk.org.cn/Article/details/gt2juslazqj.html

[U95] JS：Promise 包装
来源：http://www.ydjk.org.cn/Article/details/gt2fudnjjmk.html

new Promise((resolve, reject) => {})
来源：http://www.ydjk.org.cn/Article/details/gt2hubtsfbd.html

[U96] JS：async/await 与异常
来源：http://www.ydjk.org.cn/Article/details/gt2szwajfoj.html

try { const d = await f(); } catch (e) { console.error(e); }
来源：http://www.52xcode.cn/Article/details/gt2nywxehzf.html

[U97] JS：并发请求
来源：http://www.ydjk.org.cn/Article/details/gt2vkyyonml.html

await Promise.all(urls.map(u => fetch(u)))
来源：http://www.52xcode.cn/Article/details/gt2ulrmonka.html

[U98] JS：fetch 带 JSON
来源：http://www.52xcode.cn/Article/details/gt2spuzrjid.html

await fetch(url, { method: "POST", headers: { "Content-Type": "application/json" }, body: JSON.stringify(d) })
来源：http://www.ydjk.org.cn/Article/details/gt2rhvlhusk.html

[U99] JS：事件监听
来源：http://www.ydjk.org.cn/Article/details/gt2hcszykht.html

el.addEventListener("click", e => {})
来源：http://www.ydjk.org.cn/Article/details/gt2hrvgboju.html

[U100] JS：DOM 查询
来源：http://www.ydjk.org.cn/Article/details/gt2tjdsssze.html

document.querySelector(".item")
来源：http://www.52xcode.cn/Article/details/gt2basymwef.html

[U101] JS：classList 操作
来源：http://www.ydjk.org.cn/Article/details/gt2zuoymkaf.html

el.classList.toggle("active")
来源：http://www.ydjk.org.cn/Article/details/gt2lbaualqb.html

[U102] JS：本地存储
来源：http://www.52xcode.cn/Article/details/gt2omxcdzdk.html

localStorage.setItem("k", JSON.stringify(v))
来源：http://www.ydjk.org.cn/Article/details/gt2dcdirkbe.html

[U103] JS：定时器
来源：http://www.ydjk.org.cn/Article/details/gt2nkmgfsxi.html

setTimeout(fn, 1000);  setInterval(fn, 1000);
来源：http://www.52xcode.cn/Article/details/gt2qiijrvdq.html

[U104] JS：防抖
来源：http://www.52xcode.cn/Article/details/gt2axthjowy.html

const debounce = (fn, ms) => { let t; return (...a) => { clearTimeout(t); t = setTimeout(() => fn(...a), ms); }; };
来源：http://www.ydjk.org.cn/Article/details/gt2vmqjorsz.html

[U105] JS：节流
来源：http://www.ydjk.org.cn/Article/details/gt2obikbaqm.html

const throttle = (fn, ms) => { let last = 0; return (...a) => { const n = Date.now(); if (n - last >= ms) { last = n; fn(...a); } }; };
来源：http://www.ydjk.org.cn/Article/details/gt2lcrxhluw.html

[U106] JS：日期格式化
来源：http://www.ydjk.org.cn/Article/details/gt2suthwgja.html

new Intl.DateTimeFormat("zh-CN", { dateStyle: "medium" }).format(new Date())
来源：http://www.ydjk.org.cn/Article/details/gt2kzgrdskz.html

[U107] JS：数字千分位
来源：http://www.ydjk.org.cn/Article/details/gt2zxyesrwj.html

new Intl.NumberFormat("en-US").format(1234567)
来源：http://www.52xcode.cn/Article/details/gt2aijptaru.html

[U108] JS：随机整数
来源：http://www.52xcode.cn/Article/details/gt2qidrkrvr.html

Math.floor(Math.random() * (max - min + 1)) + min
来源：http://www.ydjk.org.cn/Article/details/gt2wlommyvj.html

[U109] JS：数组分组
来源：http://www.52xcode.cn/Article/details/gt2juvxdbec.html

Object.groupBy(arr, x => x.type)
来源：http://www.52xcode.cn/Article/details/gt2lzmauafk.html

[U110] JS：数组分块
来源：http://www.ydjk.org.cn/Article/details/gt2cfehcyke.html

arr.reduce((acc, x, i) => (i % size ? acc : [...acc, arr.slice(i, i + size)]), [])
来源：http://www.ydjk.org.cn/Article/details/gt2rjiuyxbk.html

[U111] JS：对象转 Map
来源：http://www.52xcode.cn/Article/details/gt2wsbnojny.html

new Map(Object.entries(obj))
来源：http://www.ydjk.org.cn/Article/details/gt2rbmzmlif.html

[U112] JS：字符串补位
来源：http://www.52xcode.cn/Article/details/gt2kbnqhdzx.html

"7".padStart(3, "0")
来源：http://www.ydjk.org.cn/Article/details/gt2vmwfkgjo.html

[U113] JS：正则替换全部
来源：http://www.52xcode.cn/Article/details/gt2hpisvgvo.html

s.replaceAll("a", "b")
来源：http://www.52xcode.cn/Article/details/gt2txrpykbx.html

[U114] JS：JSON 深比较
来源：http://www.52xcode.cn/Article/details/gt2gvfygqwf.html

JSON.stringify(a) === JSON.stringify(b)
来源：http://www.52xcode.cn/Article/details/gt2vcrvdpkk.html

[U115] JS：生成 UUID
来源：http://www.ydjk.org.cn/Article/details/gt2wlwsbdcy.html

crypto.randomUUID()
来源：http://www.ydjk.org.cn/Article/details/gt2evujnggs.html

[U116] JS：类型检查（JSDoc）
来源：http://www.52xcode.cn/Article/details/gt2csucrbuo.html

/** @param {string} name */ function f(name) {}
来源：http://www.ydjk.org.cn/Article/details/gt2ujyrejvy.html

[U117] JS：单元测试
来源：http://www.ydjk.org.cn/Article/details/gt2nvcygctv.html

npm i -D vitest;  npx vitest
来源：http://www.52xcode.cn/Article/details/gt2ccmdymht.html

[U118] JS：开发服务器
来源：http://www.ydjk.org.cn/Article/details/gt2fkqkxhie.html

npm i -D vite;  npx vite
来源：http://www.52xcode.cn/Article/details/gt2eebtqitp.html

[U119] JS：生产构建
来源：http://www.52xcode.cn/Article/details/gt2ijsebzet.html

npx vite build
来源：http://www.52xcode.cn/Article/details/gt2mmpzbrmw.html

[U120] JS：读取环境变量（Vite）
来源：http://www.52xcode.cn/Article/details/gt2yieicief.html

import.meta.env.VITE_API_URL
来源：http://www.52xcode.cn/Article/details/gt2fwpreaqj.html

================================================================================
来源：http://www.ydjk.org.cn/Article/details/gt2bfbahrzh.html

统计汇总
来源：http://www.52xcode.cn/Article/details/gt2fnpczuzm.html

================================================================================
来源：http://www.52xcode.cn/Article/details/gt2bkboqmuq.html

按语言统计（条）：
来源：http://www.52xcode.cn/Article/details/gt2mjewkpka.html

Python ......... 252
来源：http://www.52xcode.cn/Article/details/gt2ivdddaom.html

PHP ............ 252
来源：http://www.52xcode.cn/Article/details/gt2lafcjdyh.html

JavaScript ..... 252
来源：http://www.ydjk.org.cn/Article/details/gt2hxfillcv.html

TypeScript ..... 212
来源：http://www.52xcode.cn/Article/details/gt2qdivwwaa.html

Java ........... 212
来源：http://www.52xcode.cn/Article/details/gt2qjwqdtnw.html

Go ............. 212
来源：http://www.ydjk.org.cn/Article/details/gt2mocupllb.html

Ruby ........... 212
来源：http://www.52xcode.cn/Article/details/gt2uxrycbkt.html

C# ............. 212
来源：http://www.52xcode.cn/Article/details/gt2isivybfx.html

C .............. 30
来源：http://www.ydjk.org.cn/Article/details/gt2fsjtljhf.html

C++ ............ 30
来源：http://www.52xcode.cn/Article/details/gt2qhhzokni.html

SQL ............ 90
来源：http://www.ydjk.org.cn/Article/details/gt2ncumqdcb.html

Bash ........... 80
来源：http://www.52xcode.cn/Article/details/gt2oxvjhhih.html

Kotlin ......... 15
来源：http://www.52xcode.cn/Article/details/gt2lyovpcvq.html

Swift .......... 15
来源：http://www.52xcode.cn/Article/details/gt2jpnshewb.html

Lua ............ 10
来源：http://www.52xcode.cn/Article/details/gt2vmumuyne.html

Perl ........... 10
来源：http://www.ydjk.org.cn/Article/details/gt2kvudnqei.html

Scala .......... 10
来源：http://www.ydjk.org.cn/Article/details/gt2rfidzawl.html

------------------------------------
来源：http://www.ydjk.org.cn/Article/details/gt2rejvlyxs.html

合计 ........... 2106 条
来源：http://www.52xcode.cn/Article/details/gt2nzefjzrt.html

按章节统计：
来源：http://www.ydjk.org.cn/Article/details/gt2spszbtqh.html

A 基础语法与类型       26 个任务 × 8 语言 =  208
来源：http://www.52xcode.cn/Article/details/gt2gzfwzvbc.html

B 流程控制             16 个任务 × 8 语言 =  128
来源：http://www.ydjk.org.cn/Article/details/gt2ocgrseju.html

C 函数与作用域         16 个任务 × 8 语言 =  128
来源：http://www.ydjk.org.cn/Article/details/gt2mxpqigoh.html

D 数组 / 列表 / 集合   26 个任务 × 8 语言 =  208
来源：http://www.ydjk.org.cn/Article/details/gt2lqnzpnxk.html

E 字符串处理           22 个任务 × 8 语言 =  176
来源：http://www.52xcode.cn/Article/details/gt2yabbxzaq.html

F 文件与目录           12 个任务 × 8 语言 =   96
来源：http://www.52xcode.cn/Article/details/gt2zlekaqlz.html

G 面向对象             16 个任务 × 8 语言 =  128
来源：http://www.ydjk.org.cn/Article/details/gt2hhegkecr.html

H 异常与错误处理       10 个任务 × 8 语言 =   80
来源：http://www.ydjk.org.cn/Article/details/gt2jmdyedla.html

I 正则表达式            8 个任务 × 8 语言 =   64
来源：http://www.ydjk.org.cn/Article/details/gt2zmopyqnc.html

J 日期与时间           10 个任务 × 8 语言 =   80
来源：http://www.52xcode.cn/Article/details/gt2kndsyvxw.html

K JSON 与序列化         8 个任务 × 8 语言 =   64
来源：http://www.52xcode.cn/Article/details/gt2wvsyijzg.html

L 网络请求              8 个任务 × 8 语言 =   64
来源：http://www.ydjk.org.cn/Article/details/gt2tokxfejv.html

M 命令行 / 进程         8 个任务 × 8 语言 =   64
来源：http://www.52xcode.cn/Article/details/gt2kflbprvl.html

N 数据结构与算法       12 个任务 × 8 语言 =   96
来源：http://www.52xcode.cn/Article/details/gt2gheudkbt.html

O 并发与异步            6 个任务 × 8 语言 =   48
来源：http://www.ydjk.org.cn/Article/details/gt2bvxcrvxf.html

P 常用工具函数          8 个任务 × 8 语言 =   64
来源：http://www.ydjk.org.cn/Article/details/gt2ybarogrk.html

Q SQL 专题                              90
来源：http://www.ydjk.org.cn/Article/details/gt2yiucftba.html

R Bash 专题                             80
来源：http://www.ydjk.org.cn/Article/details/gt2pzcuycov.html

S C / C++ 专题                          60
来源：http://www.52xcode.cn/Article/details/gt2ltfpgtdy.html

T 其他语言补充                          60
来源：http://www.52xcode.cn/Article/details/gt2mazuqhgw.html

U 高频实用片段                         120
来源：http://www.52xcode.cn/Article/details/gt2doypdubl.html

------------------------------------
来源：http://www.52xcode.cn/Article/details/gt2tctqtrka.html

合计                                  2106 条
来源：http://www.52xcode.cn/Article/details/gt2vrcjaxsv.html

--------------------------------------------------------------------------------
来源：http://www.52xcode.cn/Article/details/gt2wfkfigqx.html

使用提醒
来源：http://www.ydjk.org.cn/Article/details/gt2ubaundof.html

--------------------------------------------------------------------------------
来源：http://www.ydjk.org.cn/Article/details/gt2oucxyghl.html

1. 示例追求"最小可用"，正式项目中请补齐导入、错误处理与边界判断。
来源：http://www.ydjk.org.cn/Article/details/gt2nbvytpxx.html

2. 涉及文件、网络、数据库的示例，注意资源释放与异常捕获。
来源：http://www.52xcode.cn/Article/details/gt2qcenshji.html

3. 语言版本差异较大（如 Python 3.10 的 match、Java 17 的 record/switch 箭头），
来源：http://www.ydjk.org.cn/Article/details/gt2ygigbnei.html

在旧版本上使用前请先确认语法支持情况。
来源：http://www.52xcode.cn/Article/details/gt2nddeaeii.html

4. 标注"手写"的条目是因为该语言缺少对应内置能力，实际项目中可引入成熟库。
来源：http://www.52xcode.cn/Article/details/gt2ctoihzla.html

—— 文件结束 ——
来源：http://www.52xcode.cn/Article/details/gt2iswrdzqc.html

================================================================================
来源：http://www.52xcode.cn/Article/details/gt2jnszukid.html

程序语言常见例子速查手册（2024 版）
来源：http://www.ydjk.org.cn/Article/details/gt2cjfavebo.html

Common Programming Examples Cheat Book
来源：http://www.ydjk.org.cn/Article/details/gt2medpazpc.html

================================================================================
来源：http://www.ydjk.org.cn/Article/details/gt2rxprathw.html

【收录内容】
来源：http://www.52xcode.cn/Article/details/gt2niylukkb.html

覆盖 12 种语言 / 语法与常见 API：
来源：http://www.ydjk.org.cn/Article/details/gt2qiuhqbae.html

Python · PHP · JavaScript · TypeScript · Java · Go · Ruby · C#
来源：http://www.52xcode.cn/Article/details/gt2ypjiityu.html

SQL · Bash · C · C++
来源：http://www.ydjk.org.cn/Article/details/gt2yuaeibii.html

按「任务」分组：每个任务下按语言各给出一条最小可用示例。
来源：http://www.ydjk.org.cn/Article/details/gt2yssggahe.html

【使用说明】
来源：http://www.52xcode.cn/Article/details/gt2fpobdpss.html

1. 每个任务形如 "[编号] 任务名"，下面每行以语言标记开头：
来源：http://www.ydjk.org.cn/Article/details/gt2qbxgelgq.html

Py:    Python        PHP:   PHP           JS:    JavaScript
来源：http://www.ydjk.org.cn/Article/details/gt2rxzbgfxs.html

TS:    TypeScript    Java:  Java          Go:    Go
来源：http://www.ydjk.org.cn/Article/details/gt2tmgbuvib.html

Ruby:  Ruby          C#:    C#            SQL:   SQL
来源：http://www.52xcode.cn/Article/details/gt2jxuxamir.html

Bash:  Shell         C:     C             C++:   C++
来源：http://www.52xcode.cn/Article/details/gt2eqwwgyus.html

2. 示例只展示核心写法，刻意省略 import / require / include / using 等样板代码。
来源：http://www.52xcode.cn/Article/details/gt2jpusvceg.html

需要完整可运行文件时，请自行补齐当前语言的导入语句。
来源：http://www.ydjk.org.cn/Article/details/gt2etbngynq.html

3. 语法基准：Python 3.10+ / PHP 8.1+ / ES2020+ / TypeScript 5 / Java 17 /
来源：http://www.ydjk.org.cn/Article/details/gt2wnrqxhut.html

Go 1.21+ / Ruby 3.x / C# 10+ / C17 / C++17。
来源：http://www.52xcode.cn/Article/details/gt2ohyolhtr.html

4. 检索建议：用编辑器或浏览器 Ctrl+F 搜关键词，如 "排序" "读取文件" "正则"。
来源：http://www.ydjk.org.cn/Article/details/gt2hjuftrwd.html

5. 标记为 "// 无" 表示该语言没有对应的一等语法，需用替代写法（示例给出替代方案）。
来源：http://www.52xcode.cn/Article/details/gt2mereewrl.html

6. 符号 "⏎" 表示代码在此处换行（主要用于 Python 等强制缩进、无法压成一行的结构）。
来源：http://www.52xcode.cn/Article/details/gt2voabltmf.html

【文件统计】
来源：http://www.52xcode.cn/Article/details/gt2nksvccdh.html

语言示例共 2106 条，分布见本文末尾的「统计汇总」。
来源：http://www.52xcode.cn/Article/details/gt2pmczcukl.html

--------------------------------------------------------------------------------
来源：http://www.52xcode.cn/Article/details/gt2srirfrlf.html

目  录
来源：http://www.ydjk.org.cn/Article/details/gt2tiellije.html

--------------------------------------------------------------------------------
来源：http://www.52xcode.cn/Article/details/gt2ddndweeq.html

A. 基础语法与类型              （第 1 节，26 个任务，208 条）
来源：http://www.ydjk.org.cn/Article/details/gt2lkovckkt.html

B. 流程控制                    （第 2 节，16 个任务，128 条）
来源：http://www.52xcode.cn/Article/details/gt2arqbyfzz.html

C. 函数与作用域                （第 3 节，16 个任务，128 条）
来源：http://www.ydjk.org.cn/Article/details/gt2kugvvisq.html

D. 数组 / 列表 / 集合          （第 4 节，26 个任务，208 条）
来源：http://www.ydjk.org.cn/Article/details/gt2wxokgmwx.html

E. 字符串处理                  （第 5 节，22 个任务，176 条）
来源：http://www.52xcode.cn/Article/details/gt2pgewovci.html

F. 文件与目录                  （第 6 节，12 个任务，96 条）
来源：http://www.ydjk.org.cn/Article/details/gt2ysfoteqq.html

G. 面向对象                    （第 7 节，16 个任务，128 条）
来源：http://www.52xcode.cn/Article/details/gt2cnnfeueu.html

H. 异常与错误处理              （第 8 节，10 个任务，80 条）
来源：http://www.52xcode.cn/Article/details/gt2xmckrwjw.html

I. 正则表达式                  （第 9 节，8 个任务，64 条）
来源：http://www.ydjk.org.cn/Article/details/gt2pdgfwghv.html

J. 日期与时间                  （第 10 节，10 个任务，80 条）
来源：http://www.52xcode.cn/Article/details/gt2eoukxbhj.html

K. JSON 与序列化               （第 11 节，8 个任务，64 条）
来源：http://www.52xcode.cn/Article/details/gt2tcxmjwpa.html

L. 网络请求                    （第 12 节，8 个任务，64 条）
来源：http://www.52xcode.cn/Article/details/gt2brkcwhuj.html

M. 命令行 / 进程 / 环境        （第 13 节，8 个任务，64 条）
来源：http://www.ydjk.org.cn/Article/details/gt2vsvohkuc.html

N. 数据结构与算法              （第 14 节，12 个任务，96 条）
来源：http://www.ydjk.org.cn/Article/details/gt2vmqnpykb.html

O. 并发与异步                  （第 15 节，6 个任务，48 条）
来源：http://www.ydjk.org.cn/Article/details/gt2wsylqvsf.html

P. 常用工具函数                （第 16 节，8 个任务，64 条）
来源：http://www.ydjk.org.cn/Article/details/gt2pqtsmemv.html

Q. SQL 专题                    （第 17 节，90 条）
来源：http://www.52xcode.cn/Article/details/gt2lichldhx.html

R. Bash 专题                   （第 18 节，80 条）
来源：http://www.52xcode.cn/Article/details/gt2gdgsmhfo.html

S. C / C++ 专题                （第 19 节，60 条）
来源：http://www.ydjk.org.cn/Article/details/gt2osirvpzh.html

T. 其他语言补充                （第 20 节，60 条：Kotlin / Swift / Lua / Perl / Scala）
来源：http://www.ydjk.org.cn/Article/details/gt2eoazhgbp.html

U. 高频实用片段                （第 21 节，120 条：Python / PHP / JavaScript 各 40 条）
来源：http://www.52xcode.cn/Article/details/gt2svflempv.html

================================================================================
来源：http://www.ydjk.org.cn/Article/details/gt2qjnlzcfh.html

A. 基础语法与类型
来源：http://www.52xcode.cn/Article/details/gt2wfzrlccc.html

================================================================================
来源：http://www.52xcode.cn/Article/details/gt2qwuomnnz.html

[A01] Hello World
来源：http://www.ydjk.org.cn/Article/details/gt2tsejnvmw.html

Py:   print("Hello, World!")
来源：http://www.ydjk.org.cn/Article/details/gt2yhedtqno.html

PHP:  echo "Hello, World!";
来源：http://www.ydjk.org.cn/Article/details/gt2dlzahbiy.html

JS:   console.log("Hello, World!");
来源：http://www.ydjk.org.cn/Article/details/gt2sauvpwbe.html

TS:   const msg: string = "Hello, World!"; console.log(msg);
来源：http://www.52xcode.cn/Article/details/gt2yuztswbs.html

Java: System.out.println("Hello, World!");
来源：http://www.52xcode.cn/Article/details/gt2lrpzltxc.html

Go:   fmt.Println("Hello, World!")
来源：http://www.52xcode.cn/Article/details/gt2gwujnmei.html

Ruby: puts "Hello, World!"
来源：http://www.ydjk.org.cn/Article/details/gt2oolrrmjn.html

C#:   Console.WriteLine("Hello, World!");
来源：http://www.52xcode.cn/Article/details/gt2cwpcpeno.html

[A02] 变量声明与赋值
来源：http://www.ydjk.org.cn/Article/details/gt2ptzmtadm.html

Py:   name = "Alex"; age = 20            # 动态类型，无需声明
来源：http://www.ydjk.org.cn/Article/details/gt2yvvfqarf.html

PHP:  $name = "Alex"; $age = 20;
来源：http://www.52xcode.cn/Article/details/gt2epnfuhqy.html

JS:   let name = "Alex"; const age = 20;
来源：http://www.52xcode.cn/Article/details/gt2zjyucbhn.html

TS:   let name: string = "Alex"; const age: number = 20;
来源：http://www.ydjk.org.cn/Article/details/gt2eloxxswn.html

Java: String name = "Alex"; int age = 20;
来源：http://www.52xcode.cn/Article/details/gt2uqkxmera.html

Go:   name := "Alex"; age := 20
来源：http://www.ydjk.org.cn/Article/details/gt2nkgonfzl.html

Ruby: name = "Alex"; age = 20
来源：http://www.ydjk.org.cn/Article/details/gt2vuywzhni.html

C#:   string name = "Alex"; int age = 20;
来源：http://www.ydjk.org.cn/Article/details/gt2jwbhutcn.html

[A03] 常量定义
来源：http://www.52xcode.cn/Article/details/gt2sxjshxas.html

Py:   PI = 3.14159                       # 约定全大写，语言不强制
来源：http://www.52xcode.cn/Article/details/gt2nrkmbpyp.html

PHP:  const PI = 3.14159;
来源：http://www.52xcode.cn/Article/details/gt2athztrwo.html


<!-- 参考信息 -->