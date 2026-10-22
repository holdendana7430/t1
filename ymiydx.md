代发 wailian999

[U31] Py：单测
来源：http://www.52xcode.cn/Article/details/gt2wtrubood.html

python -m pytest -q
来源：http://www.52xcode.cn/Article/details/gt2xkqwvlfd.html

[U32] Py：代码格式化
来源：http://www.ydjk.org.cn/Article/details/gt2usvrxfsk.html

ruff format . && ruff check --fix .
来源：http://www.ydjk.org.cn/Article/details/gt2zifzsanc.html

[U33] Py：打包发布
来源：http://www.52xcode.cn/Article/details/gt2xgcjsvab.html

python -m build  （依赖 pyproject.toml）
来源：http://www.ydjk.org.cn/Article/details/gt2enucueej.html

[U34] Py：判断编码
来源：http://www.52xcode.cn/Article/details/gt2mpwcpauz.html

chardet.detect(raw)
来源：http://www.ydjk.org.cn/Article/details/gt2lvrrwrei.html

[U35] Py：发送邮件
来源：http://www.52xcode.cn/Article/details/gt2yzvaqfky.html

smtplib.SMTP_SSL(...).send_message(msg)
来源：http://www.52xcode.cn/Article/details/gt2rjxvkjcz.html

[U36] Py：定时任务
来源：http://www.ydjk.org.cn/Article/details/gt2rjazgtqh.html

schedule.every(10).minutes.do(job)
来源：http://www.52xcode.cn/Article/details/gt2fehvzbzg.html

[U37] Py：读写 Excel
来源：http://www.52xcode.cn/Article/details/gt2etxrqoho.html

pandas.read_excel / DataFrame.to_excel
来源：http://www.52xcode.cn/Article/details/gt2dhgfvukt.html

[U38] Py：获取脚本所在目录
来源：http://www.52xcode.cn/Article/details/gt2otkylefr.html

Path(__file__).resolve().parent
来源：http://www.52xcode.cn/Article/details/gt2ouobjtju.html

[U39] Py：判断是否在交互环境
来源：http://www.ydjk.org.cn/Article/details/gt2ctositpd.html

sys.stdout.isatty()
来源：http://www.52xcode.cn/Article/details/gt2owbxbmai.html

[U40] Py：打印到标准错误
来源：http://www.52xcode.cn/Article/details/gt2dkvlvirm.html

print("err", file=sys.stderr)
来源：http://www.ydjk.org.cn/Article/details/gt2emcpkybf.html

[U41] PHP：初始化 Composer 项目
来源：http://www.ydjk.org.cn/Article/details/gt2gsehpqwh.html

composer init;  composer require guzzlehttp/guzzle
来源：http://www.ydjk.org.cn/Article/details/gt2ucgxbjmm.html

[U42] PHP：PSR-4 自动加载
来源：http://www.ydjk.org.cn/Article/details/gt2nyzmoiic.html

"autoload": { "psr-4": { "App\\": "src/" } }
来源：http://www.52xcode.cn/Article/details/gt2xmzbbgnl.html

[U43] PHP：声明命名空间
来源：http://www.52xcode.cn/Article/details/gt2zcflsdun.html

namespace App\Http;
来源：http://www.52xcode.cn/Article/details/gt2vxeblryg.html

[U44] PHP：开启严格类型
来源：http://www.52xcode.cn/Article/details/gt2uapwgchm.html

declare(strict_types=1);
来源：http://www.ydjk.org.cn/Article/details/gt2eqgmrler.html

[U45] PHP：类型声明与返回类型
来源：http://www.ydjk.org.cn/Article/details/gt2pemdamwj.html

function add(int $a, int $b): int { return $a + $b; }
来源：http://www.52xcode.cn/Article/details/gt2wzxvylen.html

[U46] PHP：可空类型
来源：http://www.52xcode.cn/Article/details/gt2xlbhtcqx.html

?string $name = null
来源：http://www.52xcode.cn/Article/details/gt2ntwjdnjr.html

[U47] PHP：联合类型
来源：http://www.ydjk.org.cn/Article/details/gt2wyqmohzg.html

int|string $id
来源：http://www.52xcode.cn/Article/details/gt2sxstsslo.html

[U48] PHP：纯枚举
来源：http://www.ydjk.org.cn/Article/details/gt2btfjukyv.html

enum Status: string { case Active = "active"; case Off = "off"; }
来源：http://www.52xcode.cn/Article/details/gt2pdlerdni.html

[U49] PHP：只读属性
来源：http://www.ydjk.org.cn/Article/details/gt2omvhxpet.html

public readonly string $name
来源：http://www.52xcode.cn/Article/details/gt2irdfurzn.html

[U50] PHP：构造器属性提升
来源：http://www.52xcode.cn/Article/details/gt2cjjvkomq.html

public function __construct(private int $id) {}
来源：http://www.52xcode.cn/Article/details/gt2mdmftzxp.html

[U51] PHP：数组解构
来源：http://www.ydjk.org.cn/Article/details/gt2sqkepcsw.html

[$a, $b] = $arr;
来源：http://www.52xcode.cn/Article/details/gt2bvegqtol.html

[U52] PHP：箭头函数
来源：http://www.ydjk.org.cn/Article/details/gt2nefjrkdp.html

$double = fn($x) => $x * 2;
来源：http://www.ydjk.org.cn/Article/details/gt2entplhmn.html

[U53] PHP：空合并运算符
来源：http://www.52xcode.cn/Article/details/gt2bciavjno.html

$v = $a ?? $b ?? "default";
来源：http://www.52xcode.cn/Article/details/gt2jlgncgip.html

[U54] PHP：空安全调用
来源：http://www.52xcode.cn/Article/details/gt2qvsjisks.html

$obj?->method()
来源：http://www.52xcode.cn/Article/details/gt2xfzstunh.html

[U55] PHP：match 表达式
来源：http://www.52xcode.cn/Article/details/gt2dhjygdjt.html

$s = match($x) { 1 => "一", default => "其他" };
来源：http://www.ydjk.org.cn/Article/details/gt2zkqlzpcy.html

[U56] PHP：命名参数
来源：http://www.52xcode.cn/Article/details/gt2flhakiey.html

f(a: 1, b: 2)
来源：http://www.ydjk.org.cn/Article/details/gt2kwcduqbc.html

[U57] PHP：字符串插值
来源：http://www.52xcode.cn/Article/details/gt2qmikwnxm.html

"值: {$a}"
来源：http://www.52xcode.cn/Article/details/gt2sqhmjbhj.html

[U58] PHP：数组三件套
来源：http://www.52xcode.cn/Article/details/gt2rprrjybg.html

array_map($f, $a);  array_filter($a, $f);  array_reduce($a, $f, 0);
来源：http://www.52xcode.cn/Article/details/gt2rdvevneq.html

[U59] PHP：自定义排序
来源：http://www.52xcode.cn/Article/details/gt2jdkpewnf.html

usort($arr, fn($a, $b) => $a["age"] <=> $b["age"]);
来源：http://www.52xcode.cn/Article/details/gt2jegzvffg.html

[U60] PHP：JSON 编解码
来源：http://www.52xcode.cn/Article/details/gt2cqtkenvr.html

json_encode($d, JSON_UNESCAPED_UNICODE);  json_decode($s, true);
来源：http://www.52xcode.cn/Article/details/gt2hvtrzlvn.html

[U61] PHP：正则
来源：http://www.52xcode.cn/Article/details/gt2yxtvrhou.html

preg_match('/(\d+)/', $s, $m);  preg_replace('/\d+/', '#', $s);
来源：http://www.52xcode.cn/Article/details/gt2evslsqxh.html

[U62] PHP：日期对象
来源：http://www.52xcode.cn/Article/details/gt2ildzadrb.html

(new DateTimeImmutable())->format("Y-m-d");
来源：http://www.ydjk.org.cn/Article/details/gt2bmyxnabz.html

[U63] PHP：文件读写
来源：http://www.52xcode.cn/Article/details/gt2rijxhsne.html

file_get_contents($f);  file_put_contents($f, $data);
来源：http://www.ydjk.org.cn/Article/details/gt2sisurwyz.html

[U64] PHP：目录遍历
来源：http://www.52xcode.cn/Article/details/gt2zyrnmxza.html

glob("dir/*.php");  scandir("dir");
来源：http://www.52xcode.cn/Article/details/gt2amapnlod.html

[U65] PHP：会话
来源：http://www.ydjk.org.cn/Article/details/gt2djsxyyxl.html

session_start();  $_SESSION["uid"] = 1;
来源：http://www.ydjk.org.cn/Article/details/gt2yffzzich.html

[U66] PHP：设置 Cookie
来源：http://www.52xcode.cn/Article/details/gt2qyrafszr.html

setcookie("token", $v, ["httponly" => true, "samesite" => "Lax"]);
来源：http://www.ydjk.org.cn/Article/details/gt2mexiczdq.html

[U67] PHP：处理文件上传
来源：http://www.ydjk.org.cn/Article/details/gt2iltojzhs.html

$_FILES["file"]["tmp_name"] 与 move_uploaded_file()
来源：http://www.ydjk.org.cn/Article/details/gt2gseccplc.html

[U68] PHP：PDO 连接
来源：http://www.ydjk.org.cn/Article/details/gt2eofgolxc.html

$pdo = new PDO("mysql:host=localhost;dbname=app", "root", "");
来源：http://www.52xcode.cn/Article/details/gt2cdvsmfhv.html

[U69] PHP：PDO 预处理
来源：http://www.ydjk.org.cn/Article/details/gt2uernroqs.html

$stmt = $pdo->prepare("SELECT * FROM users WHERE id = ?");  $stmt->execute([$id]);
来源：http://www.ydjk.org.cn/Article/details/gt2gwjpvsaq.html

[U70] PHP：PDO 事务
来源：http://www.52xcode.cn/Article/details/gt2wsoihhrv.html

$pdo->beginTransaction();  $pdo->commit();  $pdo->rollBack();
来源：http://www.52xcode.cn/Article/details/gt2zcuuapmi.html

[U71] PHP：抛出异常
来源：http://www.ydjk.org.cn/Article/details/gt2utagdutb.html

throw new RuntimeException("失败", 500);
来源：http://www.ydjk.org.cn/Article/details/gt2xzhlbqvy.html

[U72] PHP：写错误日志
来源：http://www.ydjk.org.cn/Article/details/gt2hwwnuvej.html

error_log("失败: " . $e->getMessage());
来源：http://www.ydjk.org.cn/Article/details/gt2tmkkvqet.html

[U73] PHP：读取 ini 配置
来源：http://www.ydjk.org.cn/Article/details/gt2isxstsfq.html

parse_ini_file("config.ini", true)
来源：http://www.52xcode.cn/Article/details/gt2dhigftjk.html

[U74] PHP：读取环境变量
来源：http://www.ydjk.org.cn/Article/details/gt2nhjrelic.html

getenv("APP_ENV") ?: "production"
来源：http://www.52xcode.cn/Article/details/gt2hnbowgwo.html

[U75] PHP：依赖注入
来源：http://www.52xcode.cn/Article/details/gt2fkutjofc.html

composer require psr/container
来源：http://www.52xcode.cn/Article/details/gt2fwisdypa.html

[U76] PHP：简单路由
来源：http://www.52xcode.cn/Article/details/gt2pjhnoadt.html

$path = parse_url($_SERVER["REQUEST_URI"], PHP_URL_PATH);
来源：http://www.ydjk.org.cn/Article/details/gt2urnllyxb.html

[U77] PHP：模板渲染
来源：http://www.ydjk.org.cn/Article/details/gt2zuirwzdt.html

composer require twig/twig
来源：http://www.52xcode.cn/Article/details/gt2vmvzmiaj.html

[U78] PHP：单元测试
来源：http://www.ydjk.org.cn/Article/details/gt2flgwwrsq.html

composer require --dev phpunit/phpunit
来源：http://www.52xcode.cn/Article/details/gt2aoutmoyr.html

[U79] PHP：静态分析
来源：http://www.52xcode.cn/Article/details/gt2urhoymga.html

composer require --dev phpstan/phpstan
来源：http://www.52xcode.cn/Article/details/gt2ntvtbqkd.html

[U80] PHP：代码规范修复
来源：http://www.52xcode.cn/Article/details/gt2qdhgmuvo.html

composer require --dev friendsofphp/php-cs-fixer
来源：http://www.52xcode.cn/Article/details/gt2daowyytk.html

[U81] JS：初始化项目
来源：http://www.52xcode.cn/Article/details/gt2pkmteeoy.html

npm init -y;  npm i express
来源：http://www.ydjk.org.cn/Article/details/gt2byjoqjed.html

[U82] JS：package.json 脚本
来源：http://www.52xcode.cn/Article/details/gt2gvbcukww.html

"scripts": { "dev": "vite", "build": "vite build" }
来源：http://www.52xcode.cn/Article/details/gt2ccbwmnkz.html

[U83] JS：ES Module 导入导出
来源：http://www.ydjk.org.cn/Article/details/gt2tqmzhhbx.html

export const a = 1;  import { a } from "./m.js";
来源：http://www.52xcode.cn/Article/details/gt2gjwghpnm.html

[U84] JS：CommonJS 写法
来源：http://www.52xcode.cn/Article/details/gt2mpbjxbjz.html

module.exports = { a };  const { a } = require("./m");
来源：http://www.52xcode.cn/Article/details/gt2ildsdmvz.html

[U85] JS：可选链
来源：http://www.ydjk.org.cn/Article/details/gt2cynbyqme.html

a?.b?.c
来源：http://www.52xcode.cn/Article/details/gt2llrresmf.html

[U86] JS：空值合并
来源：http://www.ydjk.org.cn/Article/details/gt2nqypkiel.html

a ?? b
来源：http://www.52xcode.cn/Article/details/gt2zonjtgef.html

[U87] JS：解构默认值
来源：http://www.52xcode.cn/Article/details/gt2qhwthefu.html

const { a = 1, b = 2 } = obj;
来源：http://www.ydjk.org.cn/Article/details/gt2jkzouhxa.html

[U88] JS：对象展开合并
来源：http://www.52xcode.cn/Article/details/gt2cooowrug.html

{ ...a, ...b }
来源：http://www.ydjk.org.cn/Article/details/gt2acsgovzd.html

[U89] JS：数组去重
来源：http://www.ydjk.org.cn/Article/details/gt2afplcpqt.html

[...new Set(arr)]
来源：http://www.ydjk.org.cn/Article/details/gt2vnhxuysb.html

[U90] JS：数字数组排序
来源：http://www.ydjk.org.cn/Article/details/gt2rlwbrnlh.html

[...arr].sort((a, b) => a - b)
来源：http://www.52xcode.cn/Article/details/gt2jwdbcddy.html

[U91] JS：对象键值遍历
来源：http://www.ydjk.org.cn/Article/details/gt2euyfbcke.html

Object.entries(obj).forEach(([k, v]) => {});
来源：http://www.ydjk.org.cn/Article/details/gt2bazmsscq.html

[U92] JS：深拷贝
来源：http://www.52xcode.cn/Article/details/gt2ocfgbnnw.html

structuredClone(obj)
来源：http://www.ydjk.org.cn/Article/details/gt2egblcvik.html

[U93] JS：模板字符串
来源：http://www.ydjk.org.cn/Article/details/gt2cxqbqveg.html

`共 ${n} 条`
来源：http://www.52xcode.cn/Article/details/gt2xyxsapyp.html

[U94] JS：箭头函数
来源：http://www.ydjk.org.cn/Article/details/gt2zzufwimm.html

const double = x => x * 2;
来源：http://www.ydjk.org.cn/Article/details/gt2uhomdhru.html

[U95] JS：Promise 包装
来源：http://www.52xcode.cn/Article/details/gt2syqbkisy.html

new Promise((resolve, reject) => {})
来源：http://www.52xcode.cn/Article/details/gt2pbvuvaze.html

[U96] JS：async/await 与异常
来源：http://www.ydjk.org.cn/Article/details/gt2wcqevceb.html

try { const d = await f(); } catch (e) { console.error(e); }
来源：http://www.ydjk.org.cn/Article/details/gt2zujnkgvt.html

[U97] JS：并发请求
来源：http://www.52xcode.cn/Article/details/gt2jqwjipdv.html

await Promise.all(urls.map(u => fetch(u)))
来源：http://www.ydjk.org.cn/Article/details/gt2ctqpetdl.html

[U98] JS：fetch 带 JSON
来源：http://www.52xcode.cn/Article/details/gt2osezifjc.html

await fetch(url, { method: "POST", headers: { "Content-Type": "application/json" }, body: JSON.stringify(d) })
来源：http://www.ydjk.org.cn/Article/details/gt2tfqsgvmx.html

[U99] JS：事件监听
来源：http://www.ydjk.org.cn/Article/details/gt2dmjujtcs.html

el.addEventListener("click", e => {})
来源：http://www.ydjk.org.cn/Article/details/gt2ulccbtyx.html

[U100] JS：DOM 查询
来源：http://www.ydjk.org.cn/Article/details/gt2dqqwgubk.html

document.querySelector(".item")
来源：http://www.ydjk.org.cn/Article/details/gt2txabwzql.html

[U101] JS：classList 操作
来源：http://www.52xcode.cn/Article/details/gt2yenlyvzq.html

el.classList.toggle("active")
来源：http://www.52xcode.cn/Article/details/gt2lqydgtmj.html

[U102] JS：本地存储
来源：http://www.ydjk.org.cn/Article/details/gt2toozlmqr.html

localStorage.setItem("k", JSON.stringify(v))
来源：http://www.52xcode.cn/Article/details/gt2vcqxdjjg.html

[U103] JS：定时器
来源：http://www.ydjk.org.cn/Article/details/gt2xhllfejp.html

setTimeout(fn, 1000);  setInterval(fn, 1000);
来源：http://www.52xcode.cn/Article/details/gt2oaxonzft.html

[U104] JS：防抖
来源：http://www.ydjk.org.cn/Article/details/gt2xflyuurv.html

const debounce = (fn, ms) => { let t; return (...a) => { clearTimeout(t); t = setTimeout(() => fn(...a), ms); }; };
来源：http://www.52xcode.cn/Article/details/gt2cbnjdamy.html

[U105] JS：节流
来源：http://www.ydjk.org.cn/Article/details/gt2okxnwcvb.html

const throttle = (fn, ms) => { let last = 0; return (...a) => { const n = Date.now(); if (n - last >= ms) { last = n; fn(...a); } }; };
来源：http://www.52xcode.cn/Article/details/gt2gnasgcjc.html

[U106] JS：日期格式化
来源：http://www.52xcode.cn/Article/details/gt2mnxnhsxs.html

new Intl.DateTimeFormat("zh-CN", { dateStyle: "medium" }).format(new Date())
来源：http://www.52xcode.cn/Article/details/gt2nbcvorvg.html

[U107] JS：数字千分位
来源：http://www.ydjk.org.cn/Article/details/gt2slviockh.html

new Intl.NumberFormat("en-US").format(1234567)
来源：http://www.52xcode.cn/Article/details/gt2fonobhct.html

[U108] JS：随机整数
来源：http://www.ydjk.org.cn/Article/details/gt2cjsknong.html

Math.floor(Math.random() * (max - min + 1)) + min
来源：http://www.ydjk.org.cn/Article/details/gt2jtsowrmb.html

[U109] JS：数组分组
来源：http://www.52xcode.cn/Article/details/gt2dsrtkfbd.html

Object.groupBy(arr, x => x.type)
来源：http://www.ydjk.org.cn/Article/details/gt2zbopnjif.html

[U110] JS：数组分块
来源：http://www.ydjk.org.cn/Article/details/gt2ipeoixrs.html

arr.reduce((acc, x, i) => (i % size ? acc : [...acc, arr.slice(i, i + size)]), [])
来源：http://www.52xcode.cn/Article/details/gt2ucprvoms.html

[U111] JS：对象转 Map
来源：http://www.52xcode.cn/Article/details/gt2brxsgxmo.html

new Map(Object.entries(obj))
来源：http://www.52xcode.cn/Article/details/gt2vcvbctea.html

[U112] JS：字符串补位
来源：http://www.ydjk.org.cn/Article/details/gt2cnhtwjvx.html

"7".padStart(3, "0")
来源：http://www.52xcode.cn/Article/details/gt2xeeflzqp.html

[U113] JS：正则替换全部
来源：http://www.ydjk.org.cn/Article/details/gt2ifiuyitb.html

s.replaceAll("a", "b")
来源：http://www.ydjk.org.cn/Article/details/gt2sdwwnkdh.html

[U114] JS：JSON 深比较
来源：http://www.52xcode.cn/Article/details/gt2cmadgrdm.html

JSON.stringify(a) === JSON.stringify(b)
来源：http://www.ydjk.org.cn/Article/details/gt2sqpwfkvi.html

[U115] JS：生成 UUID
来源：http://www.52xcode.cn/Article/details/gt2xdcycbpd.html

crypto.randomUUID()
来源：http://www.ydjk.org.cn/Article/details/gt2tnxfzxww.html

[U116] JS：类型检查（JSDoc）
来源：http://www.ydjk.org.cn/Article/details/gt2xgodgjmm.html

/** @param {string} name */ function f(name) {}
来源：http://www.ydjk.org.cn/Article/details/gt2csnssvhk.html

[U117] JS：单元测试
来源：http://www.ydjk.org.cn/Article/details/gt2wribeaej.html

npm i -D vitest;  npx vitest
来源：http://www.ydjk.org.cn/Article/details/gt2heahazun.html

[U118] JS：开发服务器
来源：http://www.ydjk.org.cn/Article/details/gt2nbcmrqdv.html

npm i -D vite;  npx vite
来源：http://www.ydjk.org.cn/Article/details/gt2vlplqyri.html

[U119] JS：生产构建
来源：http://www.ydjk.org.cn/Article/details/gt2wjitwaus.html

npx vite build
来源：http://www.52xcode.cn/Article/details/gt2leyouiii.html

[U120] JS：读取环境变量（Vite）
来源：http://www.ydjk.org.cn/Article/details/gt2sqevsogi.html

import.meta.env.VITE_API_URL
来源：http://www.ydjk.org.cn/Article/details/gt2nkngyiib.html

================================================================================
来源：http://www.52xcode.cn/Article/details/gt2eaulnogd.html

统计汇总
来源：http://www.ydjk.org.cn/Article/details/gt2ldzgcjcw.html

================================================================================
来源：http://www.52xcode.cn/Article/details/gt2qxaveepg.html

按语言统计（条）：
来源：http://www.ydjk.org.cn/Article/details/gt2kiylguvu.html

Python ......... 252
来源：http://www.ydjk.org.cn/Article/details/gt2eruharwj.html

PHP ............ 252
来源：http://www.ydjk.org.cn/Article/details/gt2nsncrfoh.html

JavaScript ..... 252
来源：http://www.52xcode.cn/Article/details/gt2kzxtbgsj.html

TypeScript ..... 212
来源：http://www.52xcode.cn/Article/details/gt2dewtwfvd.html

Java ........... 212
来源：http://www.ydjk.org.cn/Article/details/gt2wgduuoqe.html

Go ............. 212
来源：http://www.52xcode.cn/Article/details/gt2fvugnavh.html

Ruby ........... 212
来源：http://www.52xcode.cn/Article/details/gt2jexeiamn.html

C# ............. 212
来源：http://www.ydjk.org.cn/Article/details/gt2oblmscqq.html

C .............. 30
来源：http://www.52xcode.cn/Article/details/gt2wppolqxg.html

C++ ............ 30
来源：http://www.ydjk.org.cn/Article/details/gt2fpmqyyiw.html

SQL ............ 90
来源：http://www.ydjk.org.cn/Article/details/gt2vkafjuua.html

Bash ........... 80
来源：http://www.ydjk.org.cn/Article/details/gt2brotfbuj.html

Kotlin ......... 15
来源：http://www.52xcode.cn/Article/details/gt2uqtxzpla.html

Swift .......... 15
来源：http://www.ydjk.org.cn/Article/details/gt2ozsazgzd.html

Lua ............ 10
来源：http://www.52xcode.cn/Article/details/gt2ousqibei.html

Perl ........... 10
来源：http://www.ydjk.org.cn/Article/details/gt2oavopnri.html

Scala .......... 10
来源：http://www.52xcode.cn/Article/details/gt2abupimip.html

------------------------------------
来源：http://www.ydjk.org.cn/Article/details/gt2hfrvpfxi.html

合计 ........... 2106 条
来源：http://www.52xcode.cn/Article/details/gt2ylidhotl.html

按章节统计：
来源：http://www.ydjk.org.cn/Article/details/gt2seqwkevd.html

A 基础语法与类型       26 个任务 × 8 语言 =  208
来源：http://www.ydjk.org.cn/Article/details/gt2uozkojzm.html

B 流程控制             16 个任务 × 8 语言 =  128
来源：http://www.ydjk.org.cn/Article/details/gt2gytbjurx.html

C 函数与作用域         16 个任务 × 8 语言 =  128
来源：http://www.ydjk.org.cn/Article/details/gt2mpzqhifg.html

D 数组 / 列表 / 集合   26 个任务 × 8 语言 =  208
来源：http://www.ydjk.org.cn/Article/details/gt2zxgcpnsz.html

E 字符串处理           22 个任务 × 8 语言 =  176
来源：http://www.ydjk.org.cn/Article/details/gt2lfkthzre.html

F 文件与目录           12 个任务 × 8 语言 =   96
来源：http://www.52xcode.cn/Article/details/gt2ncpuhxjl.html

G 面向对象             16 个任务 × 8 语言 =  128
来源：http://www.ydjk.org.cn/Article/details/gt2rhvfuqml.html

H 异常与错误处理       10 个任务 × 8 语言 =   80
来源：http://www.52xcode.cn/Article/details/gt2vijlxrue.html

I 正则表达式            8 个任务 × 8 语言 =   64
来源：http://www.ydjk.org.cn/Article/details/gt2guctepiw.html

J 日期与时间           10 个任务 × 8 语言 =   80
来源：http://www.52xcode.cn/Article/details/gt2syxwkppa.html

K JSON 与序列化         8 个任务 × 8 语言 =   64
来源：http://www.ydjk.org.cn/Article/details/gt2eocwtgxv.html

L 网络请求              8 个任务 × 8 语言 =   64
来源：http://www.52xcode.cn/Article/details/gt2rargjpmn.html

M 命令行 / 进程         8 个任务 × 8 语言 =   64
来源：http://www.52xcode.cn/Article/details/gt2hpstgeue.html

N 数据结构与算法       12 个任务 × 8 语言 =   96
来源：http://www.ydjk.org.cn/Article/details/gt2qckcwtsi.html

O 并发与异步            6 个任务 × 8 语言 =   48
来源：http://www.ydjk.org.cn/Article/details/gt2seafirvi.html

P 常用工具函数          8 个任务 × 8 语言 =   64
来源：http://www.52xcode.cn/Article/details/gt2xmvxcpuy.html

Q SQL 专题                              90
来源：http://www.ydjk.org.cn/Article/details/gt2yqrpfffe.html

R Bash 专题                             80
来源：http://www.52xcode.cn/Article/details/gt2uuuxnqep.html

S C / C++ 专题                          60
来源：http://www.ydjk.org.cn/Article/details/gt2kvzmbczm.html

T 其他语言补充                          60
来源：http://www.52xcode.cn/Article/details/gt2eymvmrpu.html

U 高频实用片段                         120
来源：http://www.ydjk.org.cn/Article/details/gt2vlwwpkns.html

------------------------------------
来源：http://www.52xcode.cn/Article/details/gt2agyjsczn.html

合计                                  2106 条
来源：http://www.ydjk.org.cn/Article/details/gt2swmlunwo.html

--------------------------------------------------------------------------------
来源：http://www.ydjk.org.cn/Article/details/gt2aoxnxwww.html

使用提醒
来源：http://www.52xcode.cn/Article/details/gt2tohogftr.html

--------------------------------------------------------------------------------
来源：http://www.52xcode.cn/Article/details/gt2fufrymxq.html

1. 示例追求"最小可用"，正式项目中请补齐导入、错误处理与边界判断。
来源：http://www.ydjk.org.cn/Article/details/gt2kkqrlfen.html

2. 涉及文件、网络、数据库的示例，注意资源释放与异常捕获。
来源：http://www.52xcode.cn/Article/details/gt2pyojcclu.html

3. 语言版本差异较大（如 Python 3.10 的 match、Java 17 的 record/switch 箭头），
来源：http://www.ydjk.org.cn/Article/details/gt2rowhkhyd.html

在旧版本上使用前请先确认语法支持情况。
来源：http://www.ydjk.org.cn/Article/details/gt2hnutcfrc.html

4. 标注"手写"的条目是因为该语言缺少对应内置能力，实际项目中可引入成熟库。
来源：http://www.ydjk.org.cn/Article/details/gt2xomuxbbq.html

—— 文件结束 ——
来源：http://www.52xcode.cn/Article/details/gt2nkzmgolj.html

================================================================================
来源：http://www.52xcode.cn/Article/details/gt2oxcujiny.html

程序语言常见例子速查手册（2024 版）
来源：http://www.52xcode.cn/Article/details/gt2snbmytyc.html

Common Programming Examples Cheat Book
来源：http://www.52xcode.cn/Article/details/gt2rnyoyous.html

================================================================================
来源：http://www.52xcode.cn/Article/details/gt2uqhhbrej.html

【收录内容】
来源：http://www.ydjk.org.cn/Article/details/gt2esqzzxmt.html

覆盖 12 种语言 / 语法与常见 API：
来源：http://www.ydjk.org.cn/Article/details/gt2cdxvzrhs.html

Python · PHP · JavaScript · TypeScript · Java · Go · Ruby · C#
来源：http://www.52xcode.cn/Article/details/gt2mzxhpvoo.html

SQL · Bash · C · C++
来源：http://www.52xcode.cn/Article/details/gt2jubcpxrr.html

按「任务」分组：每个任务下按语言各给出一条最小可用示例。
来源：http://www.ydjk.org.cn/Article/details/gt2utbidnds.html

【使用说明】
来源：http://www.ydjk.org.cn/Article/details/gt2uyxvlkhk.html

1. 每个任务形如 "[编号] 任务名"，下面每行以语言标记开头：
来源：http://www.ydjk.org.cn/Article/details/gt2bwxphajf.html

Py:    Python        PHP:   PHP           JS:    JavaScript
来源：http://www.ydjk.org.cn/Article/details/gt2xbuvvkdq.html

TS:    TypeScript    Java:  Java          Go:    Go
来源：http://www.ydjk.org.cn/Article/details/gt2jrmnnjtt.html

Ruby:  Ruby          C#:    C#            SQL:   SQL
来源：http://www.ydjk.org.cn/Article/details/gt2vxuiewdf.html

Bash:  Shell         C:     C             C++:   C++
来源：http://www.52xcode.cn/Article/details/gt2mtfgxgzv.html

2. 示例只展示核心写法，刻意省略 import / require / include / using 等样板代码。
来源：http://www.52xcode.cn/Article/details/gt2maazqzzz.html

需要完整可运行文件时，请自行补齐当前语言的导入语句。
来源：http://www.ydjk.org.cn/Article/details/gt2nmbxfrrt.html

3. 语法基准：Python 3.10+ / PHP 8.1+ / ES2020+ / TypeScript 5 / Java 17 /
来源：http://www.52xcode.cn/Article/details/gt2pkjoajig.html

Go 1.21+ / Ruby 3.x / C# 10+ / C17 / C++17。
来源：http://www.ydjk.org.cn/Article/details/gt2phkndzad.html

4. 检索建议：用编辑器或浏览器 Ctrl+F 搜关键词，如 "排序" "读取文件" "正则"。
来源：http://www.ydjk.org.cn/Article/details/gt2ceditfwj.html

5. 标记为 "// 无" 表示该语言没有对应的一等语法，需用替代写法（示例给出替代方案）。
来源：http://www.ydjk.org.cn/Article/details/gt2pehboibc.html

6. 符号 "⏎" 表示代码在此处换行（主要用于 Python 等强制缩进、无法压成一行的结构）。
来源：http://www.ydjk.org.cn/Article/details/gt2qxdadhst.html

【文件统计】
来源：http://www.52xcode.cn/Article/details/gt2ueuuewht.html

语言示例共 2106 条，分布见本文末尾的「统计汇总」。
来源：http://www.52xcode.cn/Article/details/gt2vrlwinjo.html

--------------------------------------------------------------------------------
来源：http://www.52xcode.cn/Article/details/gt2eulkfvug.html

目  录
来源：http://www.ydjk.org.cn/Article/details/gt2esybfpmr.html

--------------------------------------------------------------------------------
来源：http://www.ydjk.org.cn/Article/details/gt2rklidoeb.html

A. 基础语法与类型              （第 1 节，26 个任务，208 条）
来源：http://www.52xcode.cn/Article/details/gt2wwprzdpy.html

B. 流程控制                    （第 2 节，16 个任务，128 条）
来源：http://www.52xcode.cn/Article/details/gt2idschuny.html

C. 函数与作用域                （第 3 节，16 个任务，128 条）
来源：http://www.52xcode.cn/Article/details/gt2jpqnbjax.html

D. 数组 / 列表 / 集合          （第 4 节，26 个任务，208 条）
来源：http://www.52xcode.cn/Article/details/gt2nojdauge.html

E. 字符串处理                  （第 5 节，22 个任务，176 条）
来源：http://www.52xcode.cn/Article/details/gt2zkyibrqt.html

F. 文件与目录                  （第 6 节，12 个任务，96 条）
来源：http://www.52xcode.cn/Article/details/gt2pwomywye.html

G. 面向对象                    （第 7 节，16 个任务，128 条）
来源：http://www.ydjk.org.cn/Article/details/gt2sgmjruzi.html

H. 异常与错误处理              （第 8 节，10 个任务，80 条）
来源：http://www.52xcode.cn/Article/details/gt2gfwayjkg.html

I. 正则表达式                  （第 9 节，8 个任务，64 条）
来源：http://www.52xcode.cn/Article/details/gt2nfinfcin.html

J. 日期与时间                  （第 10 节，10 个任务，80 条）
来源：http://www.ydjk.org.cn/Article/details/gt2jfjohpka.html

K. JSON 与序列化               （第 11 节，8 个任务，64 条）
来源：http://www.ydjk.org.cn/Article/details/gt2olhatjdx.html

L. 网络请求                    （第 12 节，8 个任务，64 条）
来源：http://www.ydjk.org.cn/Article/details/gt2bnpcpsev.html

M. 命令行 / 进程 / 环境        （第 13 节，8 个任务，64 条）
来源：http://www.ydjk.org.cn/Article/details/gt2sktdsfkz.html

N. 数据结构与算法              （第 14 节，12 个任务，96 条）
来源：http://www.52xcode.cn/Article/details/gt2gsnxtnwi.html

O. 并发与异步                  （第 15 节，6 个任务，48 条）
来源：http://www.52xcode.cn/Article/details/gt2isicisoh.html

P. 常用工具函数                （第 16 节，8 个任务，64 条）
来源：http://www.ydjk.org.cn/Article/details/gt2ndktlnhl.html

Q. SQL 专题                    （第 17 节，90 条）
来源：http://www.ydjk.org.cn/Article/details/gt2hairbsnl.html

R. Bash 专题                   （第 18 节，80 条）
来源：http://www.52xcode.cn/Article/details/gt2ozczruzw.html

S. C / C++ 专题                （第 19 节，60 条）
来源：http://www.52xcode.cn/Article/details/gt2pxjthwuq.html

T. 其他语言补充                （第 20 节，60 条：Kotlin / Swift / Lua / Perl / Scala）
来源：http://www.52xcode.cn/Article/details/gt2uzhurkmy.html

U. 高频实用片段                （第 21 节，120 条：Python / PHP / JavaScript 各 40 条）
来源：http://www.52xcode.cn/Article/details/gt2zvfsluqz.html

================================================================================
来源：http://www.52xcode.cn/Article/details/gt2jfmkchcc.html

A. 基础语法与类型
来源：http://www.52xcode.cn/Article/details/gt2htfnoxoi.html

================================================================================
来源：http://www.ydjk.org.cn/Article/details/gt2ysmbypkj.html

[A01] Hello World
来源：http://www.52xcode.cn/Article/details/gt2oppwfqkq.html

Py:   print("Hello, World!")
来源：http://www.ydjk.org.cn/Article/details/gt2suqybstq.html

PHP:  echo "Hello, World!";
来源：http://www.ydjk.org.cn/Article/details/gt2rreanwnt.html

JS:   console.log("Hello, World!");
来源：http://www.ydjk.org.cn/Article/details/gt2ysxglkop.html

TS:   const msg: string = "Hello, World!"; console.log(msg);
来源：http://www.52xcode.cn/Article/details/gt2xxntlcsk.html

Java: System.out.println("Hello, World!");
来源：http://www.52xcode.cn/Article/details/gt2atrxcbjo.html

Go:   fmt.Println("Hello, World!")
来源：http://www.52xcode.cn/Article/details/gt2xzeadyxd.html

Ruby: puts "Hello, World!"
来源：http://www.52xcode.cn/Article/details/gt2afksqfnm.html

C#:   Console.WriteLine("Hello, World!");
来源：http://www.ydjk.org.cn/Article/details/gt2gybcehiq.html

[A02] 变量声明与赋值
来源：http://www.ydjk.org.cn/Article/details/gt2lywooofp.html

Py:   name = "Alex"; age = 20            # 动态类型，无需声明
来源：http://www.52xcode.cn/Article/details/gt2idqcvuyc.html

PHP:  $name = "Alex"; $age = 20;
来源：http://www.ydjk.org.cn/Article/details/gt2yczihibw.html

JS:   let name = "Alex"; const age = 20;
来源：http://www.52xcode.cn/Article/details/gt2zlynbvxl.html


<!-- 参考信息 -->