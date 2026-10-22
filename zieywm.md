代发 wailian999

[U35] Py：发送邮件
来源：http://www.ydjk.org.cn/Article/details/gt2zvksgusj.html

smtplib.SMTP_SSL(...).send_message(msg)
来源：http://www.ydjk.org.cn/Article/details/gt2cwqtcegg.html

[U36] Py：定时任务
来源：http://www.ydjk.org.cn/Article/details/gt2xwnekbaq.html

schedule.every(10).minutes.do(job)
来源：http://www.ydjk.org.cn/Article/details/gt2qfvjpstg.html

[U37] Py：读写 Excel
来源：http://www.52xcode.cn/Article/details/gt2hzzpdqjv.html

pandas.read_excel / DataFrame.to_excel
来源：http://www.52xcode.cn/Article/details/gt2afftjzqj.html

[U38] Py：获取脚本所在目录
来源：http://www.52xcode.cn/Article/details/gt2sohrmymp.html

Path(__file__).resolve().parent
来源：http://www.ydjk.org.cn/Article/details/gt2wvhfdshu.html

[U39] Py：判断是否在交互环境
来源：http://www.52xcode.cn/Article/details/gt2zdtcyjhx.html

sys.stdout.isatty()
来源：http://www.52xcode.cn/Article/details/gt2hyhrgulb.html

[U40] Py：打印到标准错误
来源：http://www.52xcode.cn/Article/details/gt2wzanhnrt.html

print("err", file=sys.stderr)
来源：http://www.52xcode.cn/Article/details/gt2xdcppnze.html

[U41] PHP：初始化 Composer 项目
来源：http://www.52xcode.cn/Article/details/gt2pjcjiujx.html

composer init;  composer require guzzlehttp/guzzle
来源：http://www.52xcode.cn/Article/details/gt2ancqacjg.html

[U42] PHP：PSR-4 自动加载
来源：http://www.ydjk.org.cn/Article/details/gt2vlyqvpiu.html

"autoload": { "psr-4": { "App\\": "src/" } }
来源：http://www.52xcode.cn/Article/details/gt2rjgmxjfi.html

[U43] PHP：声明命名空间
来源：http://www.52xcode.cn/Article/details/gt2aikewbsm.html

namespace App\Http;
来源：http://www.ydjk.org.cn/Article/details/gt2cardghmt.html

[U44] PHP：开启严格类型
来源：http://www.52xcode.cn/Article/details/gt2yhkcqffm.html

declare(strict_types=1);
来源：http://www.52xcode.cn/Article/details/gt2pollaqha.html

[U45] PHP：类型声明与返回类型
来源：http://www.52xcode.cn/Article/details/gt2ztugdqxv.html

function add(int $a, int $b): int { return $a + $b; }
来源：http://www.52xcode.cn/Article/details/gt2bhhjrpfo.html

[U46] PHP：可空类型
来源：http://www.ydjk.org.cn/Article/details/gt2ogzgobez.html

?string $name = null
来源：http://www.ydjk.org.cn/Article/details/gt2qaprsbef.html

[U47] PHP：联合类型
来源：http://www.ydjk.org.cn/Article/details/gt2esgweczp.html

int|string $id
来源：http://www.52xcode.cn/Article/details/gt2ucbilxtd.html

[U48] PHP：纯枚举
来源：http://www.ydjk.org.cn/Article/details/gt2lvgvotkx.html

enum Status: string { case Active = "active"; case Off = "off"; }
来源：http://www.52xcode.cn/Article/details/gt2lvxjuhgh.html

[U49] PHP：只读属性
来源：http://www.ydjk.org.cn/Article/details/gt2cksnqdnq.html

public readonly string $name
来源：http://www.ydjk.org.cn/Article/details/gt2uofufgtt.html

[U50] PHP：构造器属性提升
来源：http://www.ydjk.org.cn/Article/details/gt2vrfnoqsb.html

public function __construct(private int $id) {}
来源：http://www.ydjk.org.cn/Article/details/gt2zewuwvlm.html

[U51] PHP：数组解构
来源：http://www.ydjk.org.cn/Article/details/gt2srsyzozs.html

[$a, $b] = $arr;
来源：http://www.52xcode.cn/Article/details/gt2kphnowtr.html

[U52] PHP：箭头函数
来源：http://www.52xcode.cn/Article/details/gt2lafhbewz.html

$double = fn($x) => $x * 2;
来源：http://www.ydjk.org.cn/Article/details/gt2chdcznwe.html

[U53] PHP：空合并运算符
来源：http://www.52xcode.cn/Article/details/gt2bwrhwwpu.html

$v = $a ?? $b ?? "default";
来源：http://www.ydjk.org.cn/Article/details/gt2rjldeosi.html

[U54] PHP：空安全调用
来源：http://www.52xcode.cn/Article/details/gt2ksnwitkv.html

$obj?->method()
来源：http://www.52xcode.cn/Article/details/gt2vukojjxr.html

[U55] PHP：match 表达式
来源：http://www.52xcode.cn/Article/details/gt2gswyiupa.html

$s = match($x) { 1 => "一", default => "其他" };
来源：http://www.ydjk.org.cn/Article/details/gt2namxxbyk.html

[U56] PHP：命名参数
来源：http://www.ydjk.org.cn/Article/details/gt2fczvqnkg.html

f(a: 1, b: 2)
来源：http://www.ydjk.org.cn/Article/details/gt2owzoyhkb.html

[U57] PHP：字符串插值
来源：http://www.ydjk.org.cn/Article/details/gt2biazpjul.html

"值: {$a}"
来源：http://www.ydjk.org.cn/Article/details/gt2fwlzodro.html

[U58] PHP：数组三件套
来源：http://www.52xcode.cn/Article/details/gt2spvbdetl.html

array_map($f, $a);  array_filter($a, $f);  array_reduce($a, $f, 0);
来源：http://www.ydjk.org.cn/Article/details/gt2mcpdgygw.html

[U59] PHP：自定义排序
来源：http://www.ydjk.org.cn/Article/details/gt2azicscxh.html

usort($arr, fn($a, $b) => $a["age"] <=> $b["age"]);
来源：http://www.ydjk.org.cn/Article/details/gt2jngbwamn.html

[U60] PHP：JSON 编解码
来源：http://www.ydjk.org.cn/Article/details/gt2tggqjbxk.html

json_encode($d, JSON_UNESCAPED_UNICODE);  json_decode($s, true);
来源：http://www.52xcode.cn/Article/details/gt2qrqhwmcx.html

[U61] PHP：正则
来源：http://www.52xcode.cn/Article/details/gt2oarsveyd.html

preg_match('/(\d+)/', $s, $m);  preg_replace('/\d+/', '#', $s);
来源：http://www.ydjk.org.cn/Article/details/gt2pcmumukm.html

[U62] PHP：日期对象
来源：http://www.52xcode.cn/Article/details/gt2fhwtjdll.html

(new DateTimeImmutable())->format("Y-m-d");
来源：http://www.52xcode.cn/Article/details/gt2wbmndcsr.html

[U63] PHP：文件读写
来源：http://www.52xcode.cn/Article/details/gt2hbkyjlek.html

file_get_contents($f);  file_put_contents($f, $data);
来源：http://www.52xcode.cn/Article/details/gt2wulfvwom.html

[U64] PHP：目录遍历
来源：http://www.ydjk.org.cn/Article/details/gt2nthizcag.html

glob("dir/*.php");  scandir("dir");
来源：http://www.52xcode.cn/Article/details/gt2zgvpncpx.html

[U65] PHP：会话
来源：http://www.52xcode.cn/Article/details/gt2ewpxuunh.html

session_start();  $_SESSION["uid"] = 1;
来源：http://www.52xcode.cn/Article/details/gt2ojuicqwm.html

[U66] PHP：设置 Cookie
来源：http://www.ydjk.org.cn/Article/details/gt2wactqlfb.html

setcookie("token", $v, ["httponly" => true, "samesite" => "Lax"]);
来源：http://www.ydjk.org.cn/Article/details/gt2kxgytyvw.html

[U67] PHP：处理文件上传
来源：http://www.52xcode.cn/Article/details/gt2usebcxpo.html

$_FILES["file"]["tmp_name"] 与 move_uploaded_file()
来源：http://www.52xcode.cn/Article/details/gt2jopsicjn.html

[U68] PHP：PDO 连接
来源：http://www.52xcode.cn/Article/details/gt2qpzfqnrq.html

$pdo = new PDO("mysql:host=localhost;dbname=app", "root", "");
来源：http://www.52xcode.cn/Article/details/gt2mvbovrol.html

[U69] PHP：PDO 预处理
来源：http://www.ydjk.org.cn/Article/details/gt2mlzxkamn.html

$stmt = $pdo->prepare("SELECT * FROM users WHERE id = ?");  $stmt->execute([$id]);
来源：http://www.ydjk.org.cn/Article/details/gt2gtehudox.html

[U70] PHP：PDO 事务
来源：http://www.52xcode.cn/Article/details/gt2tnctqcpy.html

$pdo->beginTransaction();  $pdo->commit();  $pdo->rollBack();
来源：http://www.ydjk.org.cn/Article/details/gt2gunzrvnk.html

[U71] PHP：抛出异常
来源：http://www.ydjk.org.cn/Article/details/gt2xfeaniuz.html

throw new RuntimeException("失败", 500);
来源：http://www.52xcode.cn/Article/details/gt2iogodxmm.html

[U72] PHP：写错误日志
来源：http://www.ydjk.org.cn/Article/details/gt2erlkgtis.html

error_log("失败: " . $e->getMessage());
来源：http://www.ydjk.org.cn/Article/details/gt2xcwiknii.html

[U73] PHP：读取 ini 配置
来源：http://www.52xcode.cn/Article/details/gt2npysycnt.html

parse_ini_file("config.ini", true)
来源：http://www.52xcode.cn/Article/details/gt2ogoxesug.html

[U74] PHP：读取环境变量
来源：http://www.52xcode.cn/Article/details/gt2riccaeun.html

getenv("APP_ENV") ?: "production"
来源：http://www.52xcode.cn/Article/details/gt2furmhzbp.html

[U75] PHP：依赖注入
来源：http://www.52xcode.cn/Article/details/gt2jxpxwvhc.html

composer require psr/container
来源：http://www.ydjk.org.cn/Article/details/gt2nuvtemkq.html

[U76] PHP：简单路由
来源：http://www.52xcode.cn/Article/details/gt2chokihbt.html

$path = parse_url($_SERVER["REQUEST_URI"], PHP_URL_PATH);
来源：http://www.ydjk.org.cn/Article/details/gt2fbzhgegb.html

[U77] PHP：模板渲染
来源：http://www.52xcode.cn/Article/details/gt2jgxmvosh.html

composer require twig/twig
来源：http://www.52xcode.cn/Article/details/gt2aeagbcpx.html

[U78] PHP：单元测试
来源：http://www.52xcode.cn/Article/details/gt2qsgdwnrd.html

composer require --dev phpunit/phpunit
来源：http://www.ydjk.org.cn/Article/details/gt2gfsgavha.html

[U79] PHP：静态分析
来源：http://www.52xcode.cn/Article/details/gt2wseilghr.html

composer require --dev phpstan/phpstan
来源：http://www.52xcode.cn/Article/details/gt2vdmmgxwo.html

[U80] PHP：代码规范修复
来源：http://www.52xcode.cn/Article/details/gt2xjyrurcp.html

composer require --dev friendsofphp/php-cs-fixer
来源：http://www.ydjk.org.cn/Article/details/gt2cecqqoef.html

[U81] JS：初始化项目
来源：http://www.ydjk.org.cn/Article/details/gt2xxfefppy.html

npm init -y;  npm i express
来源：http://www.52xcode.cn/Article/details/gt2ebppezkc.html

[U82] JS：package.json 脚本
来源：http://www.52xcode.cn/Article/details/gt2pcgomrea.html

"scripts": { "dev": "vite", "build": "vite build" }
来源：http://www.52xcode.cn/Article/details/gt2mdgmgqlg.html

[U83] JS：ES Module 导入导出
来源：http://www.52xcode.cn/Article/details/gt2ibfsiukm.html

export const a = 1;  import { a } from "./m.js";
来源：http://www.ydjk.org.cn/Article/details/gt2avdncmbw.html

[U84] JS：CommonJS 写法
来源：http://www.ydjk.org.cn/Article/details/gt2fqmvrlfv.html

module.exports = { a };  const { a } = require("./m");
来源：http://www.52xcode.cn/Article/details/gt2ztwdjavv.html

[U85] JS：可选链
来源：http://www.ydjk.org.cn/Article/details/gt2zcxkbtcv.html

a?.b?.c
来源：http://www.ydjk.org.cn/Article/details/gt2dscmpdfp.html

[U86] JS：空值合并
来源：http://www.52xcode.cn/Article/details/gt2vyvezazs.html

a ?? b
来源：http://www.52xcode.cn/Article/details/gt2dnvxsnwc.html

[U87] JS：解构默认值
来源：http://www.ydjk.org.cn/Article/details/gt2ujastage.html

const { a = 1, b = 2 } = obj;
来源：http://www.52xcode.cn/Article/details/gt2awflajre.html

[U88] JS：对象展开合并
来源：http://www.ydjk.org.cn/Article/details/gt2tcysaxof.html

{ ...a, ...b }
来源：http://www.52xcode.cn/Article/details/gt2elqrvpmb.html

[U89] JS：数组去重
来源：http://www.ydjk.org.cn/Article/details/gt2njdtsjcl.html

[...new Set(arr)]
来源：http://www.52xcode.cn/Article/details/gt2vhbaqcmb.html

[U90] JS：数字数组排序
来源：http://www.52xcode.cn/Article/details/gt2zkaxtzgc.html

[...arr].sort((a, b) => a - b)
来源：http://www.52xcode.cn/Article/details/gt2bhyugcbl.html

[U91] JS：对象键值遍历
来源：http://www.52xcode.cn/Article/details/gt2xdpmcbyj.html

Object.entries(obj).forEach(([k, v]) => {});
来源：http://www.ydjk.org.cn/Article/details/gt2buldgqvd.html

[U92] JS：深拷贝
来源：http://www.ydjk.org.cn/Article/details/gt2jwzxkyfu.html

structuredClone(obj)
来源：http://www.ydjk.org.cn/Article/details/gt2vtxfjgqf.html

[U93] JS：模板字符串
来源：http://www.ydjk.org.cn/Article/details/gt2dllamcgv.html

`共 ${n} 条`
来源：http://www.52xcode.cn/Article/details/gt2pibizxeo.html

[U94] JS：箭头函数
来源：http://www.ydjk.org.cn/Article/details/gt2eycqtydv.html

const double = x => x * 2;
来源：http://www.52xcode.cn/Article/details/gt2awkmeqpf.html

[U95] JS：Promise 包装
来源：http://www.ydjk.org.cn/Article/details/gt2rkgwisdp.html

new Promise((resolve, reject) => {})
来源：http://www.52xcode.cn/Article/details/gt2imtvfitj.html

[U96] JS：async/await 与异常
来源：http://www.ydjk.org.cn/Article/details/gt2obbajyxu.html

try { const d = await f(); } catch (e) { console.error(e); }
来源：http://www.ydjk.org.cn/Article/details/gt2lkxspzys.html

[U97] JS：并发请求
来源：http://www.ydjk.org.cn/Article/details/gt2wxkseilw.html

await Promise.all(urls.map(u => fetch(u)))
来源：http://www.ydjk.org.cn/Article/details/gt2wqxqbomx.html

[U98] JS：fetch 带 JSON
来源：http://www.52xcode.cn/Article/details/gt2reiyzhui.html

await fetch(url, { method: "POST", headers: { "Content-Type": "application/json" }, body: JSON.stringify(d) })
来源：http://www.ydjk.org.cn/Article/details/gt2gbucvnyb.html

[U99] JS：事件监听
来源：http://www.ydjk.org.cn/Article/details/gt2esbcgeek.html

el.addEventListener("click", e => {})
来源：http://www.ydjk.org.cn/Article/details/gt2gncdtmen.html

[U100] JS：DOM 查询
来源：http://www.52xcode.cn/Article/details/gt2arezktdg.html

document.querySelector(".item")
来源：http://www.52xcode.cn/Article/details/gt2blbhhjlk.html

[U101] JS：classList 操作
来源：http://www.ydjk.org.cn/Article/details/gt2pqmistig.html

el.classList.toggle("active")
来源：http://www.ydjk.org.cn/Article/details/gt2rikkqpih.html

[U102] JS：本地存储
来源：http://www.52xcode.cn/Article/details/gt2pgxlddzs.html

localStorage.setItem("k", JSON.stringify(v))
来源：http://www.ydjk.org.cn/Article/details/gt2aasanksy.html

[U103] JS：定时器
来源：http://www.ydjk.org.cn/Article/details/gt2wnitcirp.html

setTimeout(fn, 1000);  setInterval(fn, 1000);
来源：http://www.52xcode.cn/Article/details/gt2wvpicqzm.html

[U104] JS：防抖
来源：http://www.52xcode.cn/Article/details/gt2xhbcjidl.html

const debounce = (fn, ms) => { let t; return (...a) => { clearTimeout(t); t = setTimeout(() => fn(...a), ms); }; };
来源：http://www.52xcode.cn/Article/details/gt2xixkllkx.html

[U105] JS：节流
来源：http://www.ydjk.org.cn/Article/details/gt2aewvnzco.html

const throttle = (fn, ms) => { let last = 0; return (...a) => { const n = Date.now(); if (n - last >= ms) { last = n; fn(...a); } }; };
来源：http://www.ydjk.org.cn/Article/details/gt2kkrgaque.html

[U106] JS：日期格式化
来源：http://www.52xcode.cn/Article/details/gt2ygqvvmtn.html

new Intl.DateTimeFormat("zh-CN", { dateStyle: "medium" }).format(new Date())
来源：http://www.ydjk.org.cn/Article/details/gt2wvxqkrxf.html

[U107] JS：数字千分位
来源：http://www.52xcode.cn/Article/details/gt2vhlmdvxu.html

new Intl.NumberFormat("en-US").format(1234567)
来源：http://www.52xcode.cn/Article/details/gt2iwnddqlr.html

[U108] JS：随机整数
来源：http://www.ydjk.org.cn/Article/details/gt2onxbgjuy.html

Math.floor(Math.random() * (max - min + 1)) + min
来源：http://www.ydjk.org.cn/Article/details/gt2eqytqxwp.html

[U109] JS：数组分组
来源：http://www.52xcode.cn/Article/details/gt2uggtxscy.html

Object.groupBy(arr, x => x.type)
来源：http://www.ydjk.org.cn/Article/details/gt2gxiwocsj.html

[U110] JS：数组分块
来源：http://www.ydjk.org.cn/Article/details/gt2slpkzvfe.html

arr.reduce((acc, x, i) => (i % size ? acc : [...acc, arr.slice(i, i + size)]), [])
来源：http://www.ydjk.org.cn/Article/details/gt2snnvmsbe.html

[U111] JS：对象转 Map
来源：http://www.ydjk.org.cn/Article/details/gt2ccnblpao.html

new Map(Object.entries(obj))
来源：http://www.ydjk.org.cn/Article/details/gt2vjvhqnyi.html

[U112] JS：字符串补位
来源：http://www.ydjk.org.cn/Article/details/gt2fcmueioj.html

"7".padStart(3, "0")
来源：http://www.52xcode.cn/Article/details/gt2eierrubi.html

[U113] JS：正则替换全部
来源：http://www.52xcode.cn/Article/details/gt2trwjhhyh.html

s.replaceAll("a", "b")
来源：http://www.ydjk.org.cn/Article/details/gt2mcixcovx.html

[U114] JS：JSON 深比较
来源：http://www.52xcode.cn/Article/details/gt2ccimfghi.html

JSON.stringify(a) === JSON.stringify(b)
来源：http://www.ydjk.org.cn/Article/details/gt2wdzcuqmf.html

[U115] JS：生成 UUID
来源：http://www.52xcode.cn/Article/details/gt2dfzuekmx.html

crypto.randomUUID()
来源：http://www.52xcode.cn/Article/details/gt2zjhrblgd.html

[U116] JS：类型检查（JSDoc）
来源：http://www.52xcode.cn/Article/details/gt2nwyyinvh.html

/** @param {string} name */ function f(name) {}
来源：http://www.52xcode.cn/Article/details/gt2ykvsoihh.html

[U117] JS：单元测试
来源：http://www.52xcode.cn/Article/details/gt2kotqhwbl.html

npm i -D vitest;  npx vitest
来源：http://www.52xcode.cn/Article/details/gt2pvfjibkb.html

[U118] JS：开发服务器
来源：http://www.52xcode.cn/Article/details/gt2iwlbckkd.html

npm i -D vite;  npx vite
来源：http://www.ydjk.org.cn/Article/details/gt2wjfosmcc.html

[U119] JS：生产构建
来源：http://www.52xcode.cn/Article/details/gt2fbtbjysi.html

npx vite build
来源：http://www.52xcode.cn/Article/details/gt2anctvqls.html

[U120] JS：读取环境变量（Vite）
来源：http://www.ydjk.org.cn/Article/details/gt2biedhhcy.html

import.meta.env.VITE_API_URL
来源：http://www.52xcode.cn/Article/details/gt2tehluqbg.html

================================================================================
来源：http://www.52xcode.cn/Article/details/gt2ukybjdgy.html

统计汇总
来源：http://www.ydjk.org.cn/Article/details/gt2rffuazgx.html

================================================================================
来源：http://www.ydjk.org.cn/Article/details/gt2amnekwmd.html

按语言统计（条）：
来源：http://www.ydjk.org.cn/Article/details/gt2qxrmrhra.html

Python ......... 252
来源：http://www.ydjk.org.cn/Article/details/gt2arlxrdho.html

PHP ............ 252
来源：http://www.52xcode.cn/Article/details/gt2umsohlcu.html

JavaScript ..... 252
来源：http://www.ydjk.org.cn/Article/details/gt2zacfcybz.html

TypeScript ..... 212
来源：http://www.ydjk.org.cn/Article/details/gt2zflbhszm.html

Java ........... 212
来源：http://www.ydjk.org.cn/Article/details/gt2bdakufxv.html

Go ............. 212
来源：http://www.ydjk.org.cn/Article/details/gt2sircraxj.html

Ruby ........... 212
来源：http://www.ydjk.org.cn/Article/details/gt2xyybnsqa.html

C# ............. 212
来源：http://www.ydjk.org.cn/Article/details/gt2ztoqbtxo.html

C .............. 30
来源：http://www.52xcode.cn/Article/details/gt2lanhavds.html

C++ ............ 30
来源：http://www.ydjk.org.cn/Article/details/gt2igeusdhx.html

SQL ............ 90
来源：http://www.ydjk.org.cn/Article/details/gt2uovdyaai.html

Bash ........... 80
来源：http://www.ydjk.org.cn/Article/details/gt2fmqgtlyw.html

Kotlin ......... 15
来源：http://www.ydjk.org.cn/Article/details/gt2nfcupifi.html

Swift .......... 15
来源：http://www.52xcode.cn/Article/details/gt2jicnmgbv.html

Lua ............ 10
来源：http://www.52xcode.cn/Article/details/gt2cinuwady.html

Perl ........... 10
来源：http://www.52xcode.cn/Article/details/gt2nnwfbsge.html

Scala .......... 10
来源：http://www.ydjk.org.cn/Article/details/gt2vwdzpgbn.html

------------------------------------
来源：http://www.ydjk.org.cn/Article/details/gt2scepelxp.html

合计 ........... 2106 条
来源：http://www.52xcode.cn/Article/details/gt2mnaaouds.html

按章节统计：
来源：http://www.ydjk.org.cn/Article/details/gt2tjsqfhgu.html

A 基础语法与类型       26 个任务 × 8 语言 =  208
来源：http://www.52xcode.cn/Article/details/gt2bwsacqzl.html

B 流程控制             16 个任务 × 8 语言 =  128
来源：http://www.52xcode.cn/Article/details/gt2gkziykue.html

C 函数与作用域         16 个任务 × 8 语言 =  128
来源：http://www.ydjk.org.cn/Article/details/gt2fidbksmk.html

D 数组 / 列表 / 集合   26 个任务 × 8 语言 =  208
来源：http://www.ydjk.org.cn/Article/details/gt2fxvrhxmh.html

E 字符串处理           22 个任务 × 8 语言 =  176
来源：http://www.52xcode.cn/Article/details/gt2uhjabvke.html

F 文件与目录           12 个任务 × 8 语言 =   96
来源：http://www.ydjk.org.cn/Article/details/gt2jgnssqvz.html

G 面向对象             16 个任务 × 8 语言 =  128
来源：http://www.ydjk.org.cn/Article/details/gt2ojqaiwcw.html

H 异常与错误处理       10 个任务 × 8 语言 =   80
来源：http://www.52xcode.cn/Article/details/gt2hajfsyxt.html

I 正则表达式            8 个任务 × 8 语言 =   64
来源：http://www.52xcode.cn/Article/details/gt2gqsmazsg.html

J 日期与时间           10 个任务 × 8 语言 =   80
来源：http://www.ydjk.org.cn/Article/details/gt2fuixrjhm.html

K JSON 与序列化         8 个任务 × 8 语言 =   64
来源：http://www.ydjk.org.cn/Article/details/gt2ncnzoowl.html

L 网络请求              8 个任务 × 8 语言 =   64
来源：http://www.52xcode.cn/Article/details/gt2pejzysiv.html

M 命令行 / 进程         8 个任务 × 8 语言 =   64
来源：http://www.52xcode.cn/Article/details/gt2hezrdndk.html

N 数据结构与算法       12 个任务 × 8 语言 =   96
来源：http://www.ydjk.org.cn/Article/details/gt2wxdnukry.html

O 并发与异步            6 个任务 × 8 语言 =   48
来源：http://www.ydjk.org.cn/Article/details/gt2ecjcmapi.html

P 常用工具函数          8 个任务 × 8 语言 =   64
来源：http://www.52xcode.cn/Article/details/gt2rtedcezq.html

Q SQL 专题                              90
来源：http://www.ydjk.org.cn/Article/details/gt2rpgkfwlu.html

R Bash 专题                             80
来源：http://www.ydjk.org.cn/Article/details/gt2mddlnmat.html

S C / C++ 专题                          60
来源：http://www.52xcode.cn/Article/details/gt2uptthvyw.html

T 其他语言补充                          60
来源：http://www.52xcode.cn/Article/details/gt2mwfurvug.html

U 高频实用片段                         120
来源：http://www.ydjk.org.cn/Article/details/gt2ypbgpgyc.html

------------------------------------
来源：http://www.ydjk.org.cn/Article/details/gt2aweiwtzv.html

合计                                  2106 条
来源：http://www.52xcode.cn/Article/details/gt2pudfusqb.html

--------------------------------------------------------------------------------
来源：http://www.ydjk.org.cn/Article/details/gt2ygoucfuq.html

使用提醒
来源：http://www.52xcode.cn/Article/details/gt2kzfcrwch.html

--------------------------------------------------------------------------------
来源：http://www.ydjk.org.cn/Article/details/gt2ywvriked.html

1. 示例追求"最小可用"，正式项目中请补齐导入、错误处理与边界判断。
来源：http://www.ydjk.org.cn/Article/details/gt2fjjibkwa.html

2. 涉及文件、网络、数据库的示例，注意资源释放与异常捕获。
来源：http://www.ydjk.org.cn/Article/details/gt2rqgvcxut.html

3. 语言版本差异较大（如 Python 3.10 的 match、Java 17 的 record/switch 箭头），
来源：http://www.ydjk.org.cn/Article/details/gt2nqllnier.html

在旧版本上使用前请先确认语法支持情况。
来源：http://www.52xcode.cn/Article/details/gt2onjufsef.html

4. 标注"手写"的条目是因为该语言缺少对应内置能力，实际项目中可引入成熟库。
来源：http://www.52xcode.cn/Article/details/gt2rgzazkuu.html

—— 文件结束 ——
来源：http://www.ydjk.org.cn/Article/details/gt2hhpamjbx.html

================================================================================
来源：http://www.52xcode.cn/Article/details/gt2eycimnua.html

程序语言常见例子速查手册（2024 版）
来源：http://www.52xcode.cn/Article/details/gt2uvlkjjny.html

Common Programming Examples Cheat Book
来源：http://www.52xcode.cn/Article/details/gt2trbvzdva.html

================================================================================
来源：http://www.ydjk.org.cn/Article/details/gt2iaykgjab.html

【收录内容】
来源：http://www.52xcode.cn/Article/details/gt2cypueedo.html

覆盖 12 种语言 / 语法与常见 API：
来源：http://www.52xcode.cn/Article/details/gt2jjfudcss.html

Python · PHP · JavaScript · TypeScript · Java · Go · Ruby · C#
来源：http://www.52xcode.cn/Article/details/gt2wbifyrof.html

SQL · Bash · C · C++
来源：http://www.52xcode.cn/Article/details/gt2iatrahye.html

按「任务」分组：每个任务下按语言各给出一条最小可用示例。
来源：http://www.52xcode.cn/Article/details/gt2uiyyydsu.html

【使用说明】
来源：http://www.52xcode.cn/Article/details/gt2ppvhjrgf.html

1. 每个任务形如 "[编号] 任务名"，下面每行以语言标记开头：
来源：http://www.ydjk.org.cn/Article/details/gt2cgizdkkr.html

Py:    Python        PHP:   PHP           JS:    JavaScript
来源：http://www.52xcode.cn/Article/details/gt2srqtbnex.html

TS:    TypeScript    Java:  Java          Go:    Go
来源：http://www.ydjk.org.cn/Article/details/gt2pypxrsgh.html

Ruby:  Ruby          C#:    C#            SQL:   SQL
来源：http://www.ydjk.org.cn/Article/details/gt2ezwheesr.html

Bash:  Shell         C:     C             C++:   C++
来源：http://www.52xcode.cn/Article/details/gt2godhiakp.html

2. 示例只展示核心写法，刻意省略 import / require / include / using 等样板代码。
来源：http://www.ydjk.org.cn/Article/details/gt2tgykjmdn.html

需要完整可运行文件时，请自行补齐当前语言的导入语句。
来源：http://www.ydjk.org.cn/Article/details/gt2mrskinha.html

3. 语法基准：Python 3.10+ / PHP 8.1+ / ES2020+ / TypeScript 5 / Java 17 /
来源：http://www.52xcode.cn/Article/details/gt2zbrdexzw.html

Go 1.21+ / Ruby 3.x / C# 10+ / C17 / C++17。
来源：http://www.ydjk.org.cn/Article/details/gt2xwlhvrdg.html

4. 检索建议：用编辑器或浏览器 Ctrl+F 搜关键词，如 "排序" "读取文件" "正则"。
来源：http://www.ydjk.org.cn/Article/details/gt2phcukslw.html

5. 标记为 "// 无" 表示该语言没有对应的一等语法，需用替代写法（示例给出替代方案）。
来源：http://www.52xcode.cn/Article/details/gt2ywbztfxo.html

6. 符号 "⏎" 表示代码在此处换行（主要用于 Python 等强制缩进、无法压成一行的结构）。
来源：http://www.ydjk.org.cn/Article/details/gt2dqbomwyx.html

【文件统计】
来源：http://www.52xcode.cn/Article/details/gt2jmbvitca.html

语言示例共 2106 条，分布见本文末尾的「统计汇总」。
来源：http://www.52xcode.cn/Article/details/gt2cdsftcty.html

--------------------------------------------------------------------------------
来源：http://www.52xcode.cn/Article/details/gt2wekorkjv.html

目  录
来源：http://www.ydjk.org.cn/Article/details/gt2stwgqter.html

--------------------------------------------------------------------------------
来源：http://www.52xcode.cn/Article/details/gt2mpfomnek.html

A. 基础语法与类型              （第 1 节，26 个任务，208 条）
来源：http://www.ydjk.org.cn/Article/details/gt2sedokhmq.html

B. 流程控制                    （第 2 节，16 个任务，128 条）
来源：http://www.ydjk.org.cn/Article/details/gt2dzrwlhar.html

C. 函数与作用域                （第 3 节，16 个任务，128 条）
来源：http://www.ydjk.org.cn/Article/details/gt2oqeqgaql.html

D. 数组 / 列表 / 集合          （第 4 节，26 个任务，208 条）
来源：http://www.52xcode.cn/Article/details/gt2omnmqevh.html

E. 字符串处理                  （第 5 节，22 个任务，176 条）
来源：http://www.52xcode.cn/Article/details/gt2nspoelua.html

F. 文件与目录                  （第 6 节，12 个任务，96 条）
来源：http://www.ydjk.org.cn/Article/details/gt2zmbsfxya.html

G. 面向对象                    （第 7 节，16 个任务，128 条）
来源：http://www.52xcode.cn/Article/details/gt2rbjnweqk.html

H. 异常与错误处理              （第 8 节，10 个任务，80 条）
来源：http://www.52xcode.cn/Article/details/gt2xehegjvj.html

I. 正则表达式                  （第 9 节，8 个任务，64 条）
来源：http://www.52xcode.cn/Article/details/gt2yhcepqpm.html

J. 日期与时间                  （第 10 节，10 个任务，80 条）
来源：http://www.ydjk.org.cn/Article/details/gt2rwuddsqq.html

K. JSON 与序列化               （第 11 节，8 个任务，64 条）
来源：http://www.ydjk.org.cn/Article/details/gt2lvvgjrdb.html

L. 网络请求                    （第 12 节，8 个任务，64 条）
来源：http://www.ydjk.org.cn/Article/details/gt2gbwfkrem.html

M. 命令行 / 进程 / 环境        （第 13 节，8 个任务，64 条）
来源：http://www.ydjk.org.cn/Article/details/gt2opcxhhxt.html

N. 数据结构与算法              （第 14 节，12 个任务，96 条）
来源：http://www.ydjk.org.cn/Article/details/gt2gyfgmzwl.html

O. 并发与异步                  （第 15 节，6 个任务，48 条）
来源：http://www.52xcode.cn/Article/details/gt2cvzftdnk.html

P. 常用工具函数                （第 16 节，8 个任务，64 条）
来源：http://www.52xcode.cn/Article/details/gt2xdrigyni.html

Q. SQL 专题                    （第 17 节，90 条）
来源：http://www.ydjk.org.cn/Article/details/gt2pvsvzrxw.html

R. Bash 专题                   （第 18 节，80 条）
来源：http://www.ydjk.org.cn/Article/details/gt2sbiheuze.html

S. C / C++ 专题                （第 19 节，60 条）
来源：http://www.ydjk.org.cn/Article/details/gt2yqdhgxtz.html

T. 其他语言补充                （第 20 节，60 条：Kotlin / Swift / Lua / Perl / Scala）
来源：http://www.52xcode.cn/Article/details/gt2noxmhluk.html

U. 高频实用片段                （第 21 节，120 条：Python / PHP / JavaScript 各 40 条）
来源：http://www.52xcode.cn/Article/details/gt2sugizsky.html

================================================================================
来源：http://www.52xcode.cn/Article/details/gt2ysobopvu.html

A. 基础语法与类型
来源：http://www.ydjk.org.cn/Article/details/gt2dgatbvxf.html

================================================================================
来源：http://www.ydjk.org.cn/Article/details/gt2wthkylcv.html

[A01] Hello World
来源：http://www.ydjk.org.cn/Article/details/gt2rrsjmjjz.html

Py:   print("Hello, World!")
来源：http://www.ydjk.org.cn/Article/details/gt2gviafqcs.html

PHP:  echo "Hello, World!";
来源：http://www.52xcode.cn/Article/details/gt2kldtkvou.html

JS:   console.log("Hello, World!");
来源：http://www.52xcode.cn/Article/details/gt2uwzxrfgr.html

TS:   const msg: string = "Hello, World!"; console.log(msg);
来源：http://www.52xcode.cn/Article/details/gt2avfzanyz.html

Java: System.out.println("Hello, World!");
来源：http://www.ydjk.org.cn/Article/details/gt2ecgjfqtc.html

Go:   fmt.Println("Hello, World!")
来源：http://www.52xcode.cn/Article/details/gt2aupcxwka.html

Ruby: puts "Hello, World!"
来源：http://www.52xcode.cn/Article/details/gt2rfowmokr.html

C#:   Console.WriteLine("Hello, World!");
来源：http://www.52xcode.cn/Article/details/gt2benwrnfp.html

[A02] 变量声明与赋值
来源：http://www.52xcode.cn/Article/details/gt2mqjaumoo.html

Py:   name = "Alex"; age = 20            # 动态类型，无需声明
来源：http://www.52xcode.cn/Article/details/gt2qobtmcua.html

PHP:  $name = "Alex"; $age = 20;
来源：http://www.ydjk.org.cn/Article/details/gt2rjwnvmyp.html

JS:   let name = "Alex"; const age = 20;
来源：http://www.ydjk.org.cn/Article/details/gt2jykhevbp.html

TS:   let name: string = "Alex"; const age: number = 20;
来源：http://www.52xcode.cn/Article/details/gt2mjlvrkmf.html

Java: String name = "Alex"; int age = 20;
来源：http://www.52xcode.cn/Article/details/gt2xyxihjmw.html

Go:   name := "Alex"; age := 20
来源：http://www.ydjk.org.cn/Article/details/gt2rrbknwej.html

Ruby: name = "Alex"; age = 20
来源：http://www.ydjk.org.cn/Article/details/gt2dbpeayjl.html

C#:   string name = "Alex"; int age = 20;
来源：http://www.52xcode.cn/Article/details/gt2litacovi.html

[A03] 常量定义
来源：http://www.ydjk.org.cn/Article/details/gt2ljsahgiz.html

Py:   PI = 3.14159                       # 约定全大写，语言不强制
来源：http://www.52xcode.cn/Article/details/gt2yymmlunw.html

PHP:  const PI = 3.14159;
来源：http://www.52xcode.cn/Article/details/gt2jmyvhgoo.html


<!-- 参考信息 -->