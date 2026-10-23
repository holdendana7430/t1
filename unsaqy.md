代发 wailian999

[U31] Py：单测
来源：http://www.52xcode.cn/Article/details/gt3xmvkkekj.html

python -m pytest -q
来源：http://www.ydjk.org.cn/Article/details/gt3ceeldhin.html

[U32] Py：代码格式化
来源：http://www.52xcode.cn/Article/details/gt3vsqkvhft.html

ruff format . && ruff check --fix .
来源：http://www.ydjk.org.cn/Article/details/gt3oxsqwchu.html

[U33] Py：打包发布
来源：http://www.52xcode.cn/Article/details/gt3hrqrlycb.html

python -m build  （依赖 pyproject.toml）
来源：http://www.52xcode.cn/Article/details/gt3koogjlvr.html

[U34] Py：判断编码
来源：http://www.ydjk.org.cn/Article/details/gt3cjdcyjza.html

chardet.detect(raw)
来源：http://www.52xcode.cn/Article/details/gt3txezwwuv.html

[U35] Py：发送邮件
来源：http://www.ydjk.org.cn/Article/details/gt3frdbrnst.html

smtplib.SMTP_SSL(...).send_message(msg)
来源：http://www.ydjk.org.cn/Article/details/gt3aewnwhum.html

[U36] Py：定时任务
来源：http://www.52xcode.cn/Article/details/gt3lkvedbxj.html

schedule.every(10).minutes.do(job)
来源：http://www.ydjk.org.cn/Article/details/gt3uaqcmevc.html

[U37] Py：读写 Excel
来源：http://www.52xcode.cn/Article/details/gt3npuweomu.html

pandas.read_excel / DataFrame.to_excel
来源：http://www.ydjk.org.cn/Article/details/gt3ivrvkhpy.html

[U38] Py：获取脚本所在目录
来源：http://www.52xcode.cn/Article/details/gt3zmwuokep.html

Path(__file__).resolve().parent
来源：http://www.ydjk.org.cn/Article/details/gt3fohofvyi.html

[U39] Py：判断是否在交互环境
来源：http://www.52xcode.cn/Article/details/gt3yckapjmb.html

sys.stdout.isatty()
来源：http://www.52xcode.cn/Article/details/gt3gdvuyslj.html

[U40] Py：打印到标准错误
来源：http://www.ydjk.org.cn/Article/details/gt3clnzscwh.html

print("err", file=sys.stderr)
来源：http://www.ydjk.org.cn/Article/details/gt3hxexmhlr.html

[U41] PHP：初始化 Composer 项目
来源：http://www.ydjk.org.cn/Article/details/gt3wazmxdds.html

composer init;  composer require guzzlehttp/guzzle
来源：http://www.52xcode.cn/Article/details/gt3srmhoymi.html

[U42] PHP：PSR-4 自动加载
来源：http://www.52xcode.cn/Article/details/gt3ibjmkwxp.html

"autoload": { "psr-4": { "App\\": "src/" } }
来源：http://www.ydjk.org.cn/Article/details/gt3aryvgplv.html

[U43] PHP：声明命名空间
来源：http://www.52xcode.cn/Article/details/gt3iqorukkf.html

namespace App\Http;
来源：http://www.ydjk.org.cn/Article/details/gt3jvsfcmif.html

[U44] PHP：开启严格类型
来源：http://www.52xcode.cn/Article/details/gt3xkiykuzz.html

declare(strict_types=1);
来源：http://www.52xcode.cn/Article/details/gt3xaulbkgh.html

[U45] PHP：类型声明与返回类型
来源：http://www.ydjk.org.cn/Article/details/gt3pvfpdxoo.html

function add(int $a, int $b): int { return $a + $b; }
来源：http://www.52xcode.cn/Article/details/gt3ufqstwot.html

[U46] PHP：可空类型
来源：http://www.ydjk.org.cn/Article/details/gt3qetmlvmc.html

?string $name = null
来源：http://www.ydjk.org.cn/Article/details/gt3zeainapj.html

[U47] PHP：联合类型
来源：http://www.52xcode.cn/Article/details/gt3icnngqxi.html

int|string $id
来源：http://www.52xcode.cn/Article/details/gt3bbxgyohd.html

[U48] PHP：纯枚举
来源：http://www.52xcode.cn/Article/details/gt3giekhlue.html

enum Status: string { case Active = "active"; case Off = "off"; }
来源：http://www.52xcode.cn/Article/details/gt3sphseaut.html

[U49] PHP：只读属性
来源：http://www.52xcode.cn/Article/details/gt3rxsxgqej.html

public readonly string $name
来源：http://www.ydjk.org.cn/Article/details/gt3ldbhesfm.html

[U50] PHP：构造器属性提升
来源：http://www.52xcode.cn/Article/details/gt3zuccvmvm.html

public function __construct(private int $id) {}
来源：http://www.52xcode.cn/Article/details/gt3gircjjqm.html

[U51] PHP：数组解构
来源：http://www.52xcode.cn/Article/details/gt3lrbsikve.html

[$a, $b] = $arr;
来源：http://www.52xcode.cn/Article/details/gt3qrjhwrfz.html

[U52] PHP：箭头函数
来源：http://www.ydjk.org.cn/Article/details/gt3jbwofqhy.html

$double = fn($x) => $x * 2;
来源：http://www.52xcode.cn/Article/details/gt3teetzjek.html

[U53] PHP：空合并运算符
来源：http://www.52xcode.cn/Article/details/gt3prjuesec.html

$v = $a ?? $b ?? "default";
来源：http://www.ydjk.org.cn/Article/details/gt3wyyfqqpb.html

[U54] PHP：空安全调用
来源：http://www.52xcode.cn/Article/details/gt3ypidzprx.html

$obj?->method()
来源：http://www.ydjk.org.cn/Article/details/gt3djizhsvk.html

[U55] PHP：match 表达式
来源：http://www.ydjk.org.cn/Article/details/gt3jodnjpcw.html

$s = match($x) { 1 => "一", default => "其他" };
来源：http://www.ydjk.org.cn/Article/details/gt3bsuvndjo.html

[U56] PHP：命名参数
来源：http://www.ydjk.org.cn/Article/details/gt3mzxuhkxu.html

f(a: 1, b: 2)
来源：http://www.ydjk.org.cn/Article/details/gt3napdozrm.html

[U57] PHP：字符串插值
来源：http://www.52xcode.cn/Article/details/gt3ltlqktbs.html

"值: {$a}"
来源：http://www.52xcode.cn/Article/details/gt3gfsbikrd.html

[U58] PHP：数组三件套
来源：http://www.52xcode.cn/Article/details/gt3aeuntqam.html

array_map($f, $a);  array_filter($a, $f);  array_reduce($a, $f, 0);
来源：http://www.52xcode.cn/Article/details/gt3gmaiodkv.html

[U59] PHP：自定义排序
来源：http://www.ydjk.org.cn/Article/details/gt3nviowbhd.html

usort($arr, fn($a, $b) => $a["age"] <=> $b["age"]);
来源：http://www.ydjk.org.cn/Article/details/gt3wrabitjl.html

[U60] PHP：JSON 编解码
来源：http://www.52xcode.cn/Article/details/gt3ewnkexgo.html

json_encode($d, JSON_UNESCAPED_UNICODE);  json_decode($s, true);
来源：http://www.ydjk.org.cn/Article/details/gt3yzjxzawg.html

[U61] PHP：正则
来源：http://www.ydjk.org.cn/Article/details/gt3dfvcmimt.html

preg_match('/(\d+)/', $s, $m);  preg_replace('/\d+/', '#', $s);
来源：http://www.52xcode.cn/Article/details/gt3xlwmebpk.html

[U62] PHP：日期对象
来源：http://www.52xcode.cn/Article/details/gt3feetffdk.html

(new DateTimeImmutable())->format("Y-m-d");
来源：http://www.ydjk.org.cn/Article/details/gt3ojptznrn.html

[U63] PHP：文件读写
来源：http://www.ydjk.org.cn/Article/details/gt3esixcpja.html

file_get_contents($f);  file_put_contents($f, $data);
来源：http://www.52xcode.cn/Article/details/gt3xsivmoxb.html

[U64] PHP：目录遍历
来源：http://www.52xcode.cn/Article/details/gt3jasusiif.html

glob("dir/*.php");  scandir("dir");
来源：http://www.ydjk.org.cn/Article/details/gt3edcmxhly.html

[U65] PHP：会话
来源：http://www.ydjk.org.cn/Article/details/gt3wtjiehhj.html

session_start();  $_SESSION["uid"] = 1;
来源：http://www.ydjk.org.cn/Article/details/gt3liivxhfy.html

[U66] PHP：设置 Cookie
来源：http://www.52xcode.cn/Article/details/gt3jemgyzny.html

setcookie("token", $v, ["httponly" => true, "samesite" => "Lax"]);
来源：http://www.ydjk.org.cn/Article/details/gt3ucwqqtnq.html

[U67] PHP：处理文件上传
来源：http://www.ydjk.org.cn/Article/details/gt3apncdami.html

$_FILES["file"]["tmp_name"] 与 move_uploaded_file()
来源：http://www.ydjk.org.cn/Article/details/gt3ndtoeeeh.html

[U68] PHP：PDO 连接
来源：http://www.52xcode.cn/Article/details/gt3ljtvycvr.html

$pdo = new PDO("mysql:host=localhost;dbname=app", "root", "");
来源：http://www.ydjk.org.cn/Article/details/gt3eopsxyab.html

[U69] PHP：PDO 预处理
来源：http://www.ydjk.org.cn/Article/details/gt3txybuung.html

$stmt = $pdo->prepare("SELECT * FROM users WHERE id = ?");  $stmt->execute([$id]);
来源：http://www.ydjk.org.cn/Article/details/gt3knbeidng.html

[U70] PHP：PDO 事务
来源：http://www.52xcode.cn/Article/details/gt3xszustaa.html

$pdo->beginTransaction();  $pdo->commit();  $pdo->rollBack();
来源：http://www.52xcode.cn/Article/details/gt3ljscigkp.html

[U71] PHP：抛出异常
来源：http://www.ydjk.org.cn/Article/details/gt3sbpjpikp.html

throw new RuntimeException("失败", 500);
来源：http://www.52xcode.cn/Article/details/gt3chdxpjtm.html

[U72] PHP：写错误日志
来源：http://www.ydjk.org.cn/Article/details/gt3hylnutdi.html

error_log("失败: " . $e->getMessage());
来源：http://www.52xcode.cn/Article/details/gt3ojftvnnz.html

[U73] PHP：读取 ini 配置
来源：http://www.ydjk.org.cn/Article/details/gt3pkvcjeri.html

parse_ini_file("config.ini", true)
来源：http://www.ydjk.org.cn/Article/details/gt3ibvdogbp.html

[U74] PHP：读取环境变量
来源：http://www.ydjk.org.cn/Article/details/gt3sbiojdgw.html

getenv("APP_ENV") ?: "production"
来源：http://www.ydjk.org.cn/Article/details/gt3diyhfkwq.html

[U75] PHP：依赖注入
来源：http://www.ydjk.org.cn/Article/details/gt3hstlmmfx.html

composer require psr/container
来源：http://www.52xcode.cn/Article/details/gt3ridhyboy.html

[U76] PHP：简单路由
来源：http://www.ydjk.org.cn/Article/details/gt3yxlqerwt.html

$path = parse_url($_SERVER["REQUEST_URI"], PHP_URL_PATH);
来源：http://www.ydjk.org.cn/Article/details/gt3puvorwgp.html

[U77] PHP：模板渲染
来源：http://www.52xcode.cn/Article/details/gt3tbzxvcgz.html

composer require twig/twig
来源：http://www.ydjk.org.cn/Article/details/gt3vkwdijzb.html

[U78] PHP：单元测试
来源：http://www.ydjk.org.cn/Article/details/gt3cedlozmi.html

composer require --dev phpunit/phpunit
来源：http://www.ydjk.org.cn/Article/details/gt3chxkwhet.html

[U79] PHP：静态分析
来源：http://www.52xcode.cn/Article/details/gt3xiwhpwfq.html

composer require --dev phpstan/phpstan
来源：http://www.52xcode.cn/Article/details/gt3ocfjgntu.html

[U80] PHP：代码规范修复
来源：http://www.52xcode.cn/Article/details/gt3wmpfjctq.html

composer require --dev friendsofphp/php-cs-fixer
来源：http://www.ydjk.org.cn/Article/details/gt3amjzikdf.html

[U81] JS：初始化项目
来源：http://www.52xcode.cn/Article/details/gt3gghzqqcw.html

npm init -y;  npm i express
来源：http://www.52xcode.cn/Article/details/gt3uvgxqwmh.html

[U82] JS：package.json 脚本
来源：http://www.52xcode.cn/Article/details/gt3xugzhhnu.html

"scripts": { "dev": "vite", "build": "vite build" }
来源：http://www.ydjk.org.cn/Article/details/gt3kljwbgfo.html

[U83] JS：ES Module 导入导出
来源：http://www.52xcode.cn/Article/details/gt3wvzdtknf.html

export const a = 1;  import { a } from "./m.js";
来源：http://www.ydjk.org.cn/Article/details/gt3zmpmgtyr.html

[U84] JS：CommonJS 写法
来源：http://www.52xcode.cn/Article/details/gt3ejxooqhy.html

module.exports = { a };  const { a } = require("./m");
来源：http://www.ydjk.org.cn/Article/details/gt3nnintuzr.html

[U85] JS：可选链
来源：http://www.52xcode.cn/Article/details/gt3qylrebyq.html

a?.b?.c
来源：http://www.52xcode.cn/Article/details/gt3octfumpc.html

[U86] JS：空值合并
来源：http://www.ydjk.org.cn/Article/details/gt3vbrokqpu.html

a ?? b
来源：http://www.52xcode.cn/Article/details/gt3hbjgadwo.html

[U87] JS：解构默认值
来源：http://www.52xcode.cn/Article/details/gt3lprndtta.html

const { a = 1, b = 2 } = obj;
来源：http://www.52xcode.cn/Article/details/gt3vttjwcmx.html

[U88] JS：对象展开合并
来源：http://www.52xcode.cn/Article/details/gt3sydnffsl.html

{ ...a, ...b }
来源：http://www.ydjk.org.cn/Article/details/gt3cujuxfvi.html

[U89] JS：数组去重
来源：http://www.ydjk.org.cn/Article/details/gt3qrqwxqnp.html

[...new Set(arr)]
来源：http://www.ydjk.org.cn/Article/details/gt3xoradbxq.html

[U90] JS：数字数组排序
来源：http://www.52xcode.cn/Article/details/gt3esjngcpa.html

[...arr].sort((a, b) => a - b)
来源：http://www.ydjk.org.cn/Article/details/gt3pitjblyh.html

[U91] JS：对象键值遍历
来源：http://www.52xcode.cn/Article/details/gt3sjchavvu.html

Object.entries(obj).forEach(([k, v]) => {});
来源：http://www.52xcode.cn/Article/details/gt3eulyxygg.html

[U92] JS：深拷贝
来源：http://www.ydjk.org.cn/Article/details/gt3sjrgkvuk.html

structuredClone(obj)
来源：http://www.ydjk.org.cn/Article/details/gt3yaygborh.html

[U93] JS：模板字符串
来源：http://www.52xcode.cn/Article/details/gt3actcgbke.html

`共 ${n} 条`
来源：http://www.ydjk.org.cn/Article/details/gt3hxjjjvcg.html

[U94] JS：箭头函数
来源：http://www.52xcode.cn/Article/details/gt3ilesnbox.html

const double = x => x * 2;
来源：http://www.52xcode.cn/Article/details/gt3wtlxcqkl.html

[U95] JS：Promise 包装
来源：http://www.52xcode.cn/Article/details/gt3wvrkocyq.html

new Promise((resolve, reject) => {})
来源：http://www.ydjk.org.cn/Article/details/gt3gyzfqfay.html

[U96] JS：async/await 与异常
来源：http://www.52xcode.cn/Article/details/gt3tubrzhde.html

try { const d = await f(); } catch (e) { console.error(e); }
来源：http://www.ydjk.org.cn/Article/details/gt3ngntvmrz.html

[U97] JS：并发请求
来源：http://www.52xcode.cn/Article/details/gt3cgtisqdv.html

await Promise.all(urls.map(u => fetch(u)))
来源：http://www.ydjk.org.cn/Article/details/gt3xycstnwl.html

[U98] JS：fetch 带 JSON
来源：http://www.ydjk.org.cn/Article/details/gt3ysnctkzk.html

await fetch(url, { method: "POST", headers: { "Content-Type": "application/json" }, body: JSON.stringify(d) })
来源：http://www.52xcode.cn/Article/details/gt3yeqgzewr.html

[U99] JS：事件监听
来源：http://www.ydjk.org.cn/Article/details/gt3uizrlclo.html

el.addEventListener("click", e => {})
来源：http://www.52xcode.cn/Article/details/gt3zykdssfw.html

[U100] JS：DOM 查询
来源：http://www.52xcode.cn/Article/details/gt3rpaotpev.html

document.querySelector(".item")
来源：http://www.52xcode.cn/Article/details/gt3cieyrmyd.html

[U101] JS：classList 操作
来源：http://www.ydjk.org.cn/Article/details/gt3ougdccgc.html

el.classList.toggle("active")
来源：http://www.ydjk.org.cn/Article/details/gt3taqwrdwp.html

[U102] JS：本地存储
来源：http://www.ydjk.org.cn/Article/details/gt3yetvexnx.html

localStorage.setItem("k", JSON.stringify(v))
来源：http://www.ydjk.org.cn/Article/details/gt3fdflefga.html

[U103] JS：定时器
来源：http://www.ydjk.org.cn/Article/details/gt3azfgwmxf.html

setTimeout(fn, 1000);  setInterval(fn, 1000);
来源：http://www.52xcode.cn/Article/details/gt3dqxakkye.html

[U104] JS：防抖
来源：http://www.ydjk.org.cn/Article/details/gt3yldlyria.html

const debounce = (fn, ms) => { let t; return (...a) => { clearTimeout(t); t = setTimeout(() => fn(...a), ms); }; };
来源：http://www.ydjk.org.cn/Article/details/gt3ydpenprx.html

[U105] JS：节流
来源：http://www.ydjk.org.cn/Article/details/gt3zfxyyxrt.html

const throttle = (fn, ms) => { let last = 0; return (...a) => { const n = Date.now(); if (n - last >= ms) { last = n; fn(...a); } }; };
来源：http://www.ydjk.org.cn/Article/details/gt3haisggzg.html

[U106] JS：日期格式化
来源：http://www.ydjk.org.cn/Article/details/gt3pcmkbodx.html

new Intl.DateTimeFormat("zh-CN", { dateStyle: "medium" }).format(new Date())
来源：http://www.ydjk.org.cn/Article/details/gt3uusnfegz.html

[U107] JS：数字千分位
来源：http://www.ydjk.org.cn/Article/details/gt3mxruwaac.html

new Intl.NumberFormat("en-US").format(1234567)
来源：http://www.ydjk.org.cn/Article/details/gt3gxyhvola.html

[U108] JS：随机整数
来源：http://www.ydjk.org.cn/Article/details/gt3sbhcaebt.html

Math.floor(Math.random() * (max - min + 1)) + min
来源：http://www.52xcode.cn/Article/details/gt3iyotqztr.html

[U109] JS：数组分组
来源：http://www.ydjk.org.cn/Article/details/gt3dwdyadnh.html

Object.groupBy(arr, x => x.type)
来源：http://www.ydjk.org.cn/Article/details/gt3xckklaye.html

[U110] JS：数组分块
来源：http://www.ydjk.org.cn/Article/details/gt3qmkrvrzp.html

arr.reduce((acc, x, i) => (i % size ? acc : [...acc, arr.slice(i, i + size)]), [])
来源：http://www.ydjk.org.cn/Article/details/gt3lysiwgiq.html

[U111] JS：对象转 Map
来源：http://www.52xcode.cn/Article/details/gt3rtugjoyx.html

new Map(Object.entries(obj))
来源：http://www.ydjk.org.cn/Article/details/gt3zmmbzvcm.html

[U112] JS：字符串补位
来源：http://www.52xcode.cn/Article/details/gt3wdigdfev.html

"7".padStart(3, "0")
来源：http://www.ydjk.org.cn/Article/details/gt3zzccnoqf.html

[U113] JS：正则替换全部
来源：http://www.ydjk.org.cn/Article/details/gt3egjpjoiy.html

s.replaceAll("a", "b")
来源：http://www.52xcode.cn/Article/details/gt3lglzgxta.html

[U114] JS：JSON 深比较
来源：http://www.ydjk.org.cn/Article/details/gt3stxxwglq.html

JSON.stringify(a) === JSON.stringify(b)
来源：http://www.52xcode.cn/Article/details/gt3yfaeadjc.html

[U115] JS：生成 UUID
来源：http://www.52xcode.cn/Article/details/gt3bymfyfvk.html

crypto.randomUUID()
来源：http://www.ydjk.org.cn/Article/details/gt3pcxbsqel.html

[U116] JS：类型检查（JSDoc）
来源：http://www.ydjk.org.cn/Article/details/gt3xhhcwrvh.html

/** @param {string} name */ function f(name) {}
来源：http://www.52xcode.cn/Article/details/gt3fzsnrtqg.html

[U117] JS：单元测试
来源：http://www.ydjk.org.cn/Article/details/gt3kglrnowx.html

npm i -D vitest;  npx vitest
来源：http://www.52xcode.cn/Article/details/gt3sbxqwmdd.html

[U118] JS：开发服务器
来源：http://www.52xcode.cn/Article/details/gt3vrymyiag.html

npm i -D vite;  npx vite
来源：http://www.52xcode.cn/Article/details/gt3ysefsjer.html

[U119] JS：生产构建
来源：http://www.ydjk.org.cn/Article/details/gt3bhwaxwao.html

npx vite build
来源：http://www.ydjk.org.cn/Article/details/gt3aeinftnt.html

[U120] JS：读取环境变量（Vite）
来源：http://www.52xcode.cn/Article/details/gt3bnftxbor.html

import.meta.env.VITE_API_URL
来源：http://www.ydjk.org.cn/Article/details/gt3yfkzskcz.html

================================================================================
来源：http://www.ydjk.org.cn/Article/details/gt3ykbmoqdn.html

统计汇总
来源：http://www.52xcode.cn/Article/details/gt3iybvvwwi.html

================================================================================
来源：http://www.52xcode.cn/Article/details/gt3bfcqhbie.html

按语言统计（条）：
来源：http://www.ydjk.org.cn/Article/details/gt3qohrftbs.html

Python ......... 252
来源：http://www.ydjk.org.cn/Article/details/gt3rpzekxuh.html

PHP ............ 252
来源：http://www.ydjk.org.cn/Article/details/gt3xwaoxols.html

JavaScript ..... 252
来源：http://www.ydjk.org.cn/Article/details/gt3klsrjglz.html

TypeScript ..... 212
来源：http://www.52xcode.cn/Article/details/gt3xsevrijx.html

Java ........... 212
来源：http://www.ydjk.org.cn/Article/details/gt3jnaayeuj.html

Go ............. 212
来源：http://www.ydjk.org.cn/Article/details/gt3ibpyojbi.html

Ruby ........... 212
来源：http://www.ydjk.org.cn/Article/details/gt3aalenhce.html

C# ............. 212
来源：http://www.52xcode.cn/Article/details/gt3gklzlmsw.html

C .............. 30
来源：http://www.ydjk.org.cn/Article/details/gt3dsuhocfr.html

C++ ............ 30
来源：http://www.52xcode.cn/Article/details/gt3qkpsyzuu.html

SQL ............ 90
来源：http://www.52xcode.cn/Article/details/gt3knpwuaax.html

Bash ........... 80
来源：http://www.52xcode.cn/Article/details/gt3bhhvhgsu.html

Kotlin ......... 15
来源：http://www.52xcode.cn/Article/details/gt3bgxiyjct.html

Swift .......... 15
来源：http://www.ydjk.org.cn/Article/details/gt3ysiiwnen.html

Lua ............ 10
来源：http://www.ydjk.org.cn/Article/details/gt3ysilvamh.html

Perl ........... 10
来源：http://www.52xcode.cn/Article/details/gt3wbswxjyq.html

Scala .......... 10
来源：http://www.52xcode.cn/Article/details/gt3djulshnn.html

------------------------------------
来源：http://www.ydjk.org.cn/Article/details/gt3uthfqkqr.html

合计 ........... 2106 条
来源：http://www.52xcode.cn/Article/details/gt3ymzxcusb.html

按章节统计：
来源：http://www.52xcode.cn/Article/details/gt3regrawck.html

A 基础语法与类型       26 个任务 × 8 语言 =  208
来源：http://www.ydjk.org.cn/Article/details/gt3hgherrsp.html

B 流程控制             16 个任务 × 8 语言 =  128
来源：http://www.52xcode.cn/Article/details/gt3twdjnnik.html

C 函数与作用域         16 个任务 × 8 语言 =  128
来源：http://www.52xcode.cn/Article/details/gt3xgqwfnne.html

D 数组 / 列表 / 集合   26 个任务 × 8 语言 =  208
来源：http://www.ydjk.org.cn/Article/details/gt3yctsduie.html

E 字符串处理           22 个任务 × 8 语言 =  176
来源：http://www.ydjk.org.cn/Article/details/gt3jajatwpz.html

F 文件与目录           12 个任务 × 8 语言 =   96
来源：http://www.ydjk.org.cn/Article/details/gt3hwtnmtuk.html

G 面向对象             16 个任务 × 8 语言 =  128
来源：http://www.52xcode.cn/Article/details/gt3hjullrru.html

H 异常与错误处理       10 个任务 × 8 语言 =   80
来源：http://www.52xcode.cn/Article/details/gt3dwolqdkk.html

I 正则表达式            8 个任务 × 8 语言 =   64
来源：http://www.ydjk.org.cn/Article/details/gt3iogwoemt.html

J 日期与时间           10 个任务 × 8 语言 =   80
来源：http://www.52xcode.cn/Article/details/gt3zinmrnjn.html

K JSON 与序列化         8 个任务 × 8 语言 =   64
来源：http://www.52xcode.cn/Article/details/gt3ibpecyby.html

L 网络请求              8 个任务 × 8 语言 =   64
来源：http://www.52xcode.cn/Article/details/gt3soyigxrd.html

M 命令行 / 进程         8 个任务 × 8 语言 =   64
来源：http://www.ydjk.org.cn/Article/details/gt3sobrgdcn.html

N 数据结构与算法       12 个任务 × 8 语言 =   96
来源：http://www.ydjk.org.cn/Article/details/gt3qnzbsgup.html

O 并发与异步            6 个任务 × 8 语言 =   48
来源：http://www.ydjk.org.cn/Article/details/gt3ephxprac.html

P 常用工具函数          8 个任务 × 8 语言 =   64
来源：http://www.ydjk.org.cn/Article/details/gt3lcxxswpq.html

Q SQL 专题                              90
来源：http://www.ydjk.org.cn/Article/details/gt3bqdrqted.html

R Bash 专题                             80
来源：http://www.ydjk.org.cn/Article/details/gt3jivpcawi.html

S C / C++ 专题                          60
来源：http://www.ydjk.org.cn/Article/details/gt3gysbdxgd.html

T 其他语言补充                          60
来源：http://www.ydjk.org.cn/Article/details/gt3rderzmtq.html

U 高频实用片段                         120
来源：http://www.52xcode.cn/Article/details/gt3axbxfydv.html

------------------------------------
来源：http://www.52xcode.cn/Article/details/gt3zpuhyioe.html

合计                                  2106 条
来源：http://www.52xcode.cn/Article/details/gt3pkrijkit.html

--------------------------------------------------------------------------------
来源：http://www.52xcode.cn/Article/details/gt3qutskhwa.html

使用提醒
来源：http://www.52xcode.cn/Article/details/gt3pcbahmnc.html

--------------------------------------------------------------------------------
来源：http://www.ydjk.org.cn/Article/details/gt3nfiuipdg.html

1. 示例追求"最小可用"，正式项目中请补齐导入、错误处理与边界判断。
来源：http://www.52xcode.cn/Article/details/gt3xqitshhv.html

2. 涉及文件、网络、数据库的示例，注意资源释放与异常捕获。
来源：http://www.52xcode.cn/Article/details/gt3ajnkxoil.html

3. 语言版本差异较大（如 Python 3.10 的 match、Java 17 的 record/switch 箭头），
来源：http://www.ydjk.org.cn/Article/details/gt3gehbsdmh.html

在旧版本上使用前请先确认语法支持情况。
来源：http://www.ydjk.org.cn/Article/details/gt3ovdxdmpy.html

4. 标注"手写"的条目是因为该语言缺少对应内置能力，实际项目中可引入成熟库。
来源：http://www.ydjk.org.cn/Article/details/gt3sfopjipu.html

—— 文件结束 ——
来源：http://www.52xcode.cn/Article/details/gt3npqdjaxq.html

================================================================================
来源：http://www.ydjk.org.cn/Article/details/gt3ldmukwxn.html

程序语言常见例子速查手册（2024 版）
来源：http://www.ydjk.org.cn/Article/details/gt3pipynewm.html

Common Programming Examples Cheat Book
来源：http://www.52xcode.cn/Article/details/gt3bhfbxuir.html

================================================================================
来源：http://www.52xcode.cn/Article/details/gt3yeywnwmw.html

【收录内容】
来源：http://www.ydjk.org.cn/Article/details/gt3esbkjihx.html

覆盖 12 种语言 / 语法与常见 API：
来源：http://www.52xcode.cn/Article/details/gt3rvobqjxd.html

Python · PHP · JavaScript · TypeScript · Java · Go · Ruby · C#
来源：http://www.52xcode.cn/Article/details/gt3qufripkw.html

SQL · Bash · C · C++
来源：http://www.ydjk.org.cn/Article/details/gt3uhnnzrha.html

按「任务」分组：每个任务下按语言各给出一条最小可用示例。
来源：http://www.ydjk.org.cn/Article/details/gt3ykykldzp.html

【使用说明】
来源：http://www.ydjk.org.cn/Article/details/gt3vleoafuu.html

1. 每个任务形如 "[编号] 任务名"，下面每行以语言标记开头：
来源：http://www.52xcode.cn/Article/details/gt3uujusycr.html

Py:    Python        PHP:   PHP           JS:    JavaScript
来源：http://www.52xcode.cn/Article/details/gt3ljghisit.html

TS:    TypeScript    Java:  Java          Go:    Go
来源：http://www.52xcode.cn/Article/details/gt3erpgqrlq.html

Ruby:  Ruby          C#:    C#            SQL:   SQL
来源：http://www.ydjk.org.cn/Article/details/gt3kvxsjkhd.html

Bash:  Shell         C:     C             C++:   C++
来源：http://www.52xcode.cn/Article/details/gt3dgjldeui.html

2. 示例只展示核心写法，刻意省略 import / require / include / using 等样板代码。
来源：http://www.ydjk.org.cn/Article/details/gt3yrrzueyr.html

需要完整可运行文件时，请自行补齐当前语言的导入语句。
来源：http://www.52xcode.cn/Article/details/gt3hybbvegf.html

3. 语法基准：Python 3.10+ / PHP 8.1+ / ES2020+ / TypeScript 5 / Java 17 /
来源：http://www.52xcode.cn/Article/details/gt3kderzaqx.html

Go 1.21+ / Ruby 3.x / C# 10+ / C17 / C++17。
来源：http://www.52xcode.cn/Article/details/gt3ldktlphc.html

4. 检索建议：用编辑器或浏览器 Ctrl+F 搜关键词，如 "排序" "读取文件" "正则"。
来源：http://www.ydjk.org.cn/Article/details/gt3tddqlmkk.html

5. 标记为 "// 无" 表示该语言没有对应的一等语法，需用替代写法（示例给出替代方案）。
来源：http://www.ydjk.org.cn/Article/details/gt3vhktdhqn.html

6. 符号 "⏎" 表示代码在此处换行（主要用于 Python 等强制缩进、无法压成一行的结构）。
来源：http://www.ydjk.org.cn/Article/details/gt3pqrrzlvl.html

【文件统计】
来源：http://www.52xcode.cn/Article/details/gt3ikvwelmx.html

语言示例共 2106 条，分布见本文末尾的「统计汇总」。
来源：http://www.52xcode.cn/Article/details/gt3poeygqno.html

--------------------------------------------------------------------------------
来源：http://www.52xcode.cn/Article/details/gt3vxbqanss.html

目  录
来源：http://www.52xcode.cn/Article/details/gt3hvpncrla.html

--------------------------------------------------------------------------------
来源：http://www.52xcode.cn/Article/details/gt3uxnnfngt.html

A. 基础语法与类型              （第 1 节，26 个任务，208 条）
来源：http://www.ydjk.org.cn/Article/details/gt3zuhzzwmy.html

B. 流程控制                    （第 2 节，16 个任务，128 条）
来源：http://www.ydjk.org.cn/Article/details/gt3qfinvooc.html

C. 函数与作用域                （第 3 节，16 个任务，128 条）
来源：http://www.52xcode.cn/Article/details/gt3uxgtcejk.html

D. 数组 / 列表 / 集合          （第 4 节，26 个任务，208 条）
来源：http://www.ydjk.org.cn/Article/details/gt3xmumgcfk.html

E. 字符串处理                  （第 5 节，22 个任务，176 条）
来源：http://www.ydjk.org.cn/Article/details/gt3wzlumezb.html

F. 文件与目录                  （第 6 节，12 个任务，96 条）
来源：http://www.52xcode.cn/Article/details/gt3egpzigfy.html

G. 面向对象                    （第 7 节，16 个任务，128 条）
来源：http://www.52xcode.cn/Article/details/gt3uljhhkxx.html

H. 异常与错误处理              （第 8 节，10 个任务，80 条）
来源：http://www.ydjk.org.cn/Article/details/gt3zmtapfjd.html

I. 正则表达式                  （第 9 节，8 个任务，64 条）
来源：http://www.ydjk.org.cn/Article/details/gt3bnuaowig.html

J. 日期与时间                  （第 10 节，10 个任务，80 条）
来源：http://www.52xcode.cn/Article/details/gt3oceldrhg.html

K. JSON 与序列化               （第 11 节，8 个任务，64 条）
来源：http://www.52xcode.cn/Article/details/gt3xhszggfd.html

L. 网络请求                    （第 12 节，8 个任务，64 条）
来源：http://www.ydjk.org.cn/Article/details/gt3lvbegoyy.html

M. 命令行 / 进程 / 环境        （第 13 节，8 个任务，64 条）
来源：http://www.52xcode.cn/Article/details/gt3jnoikdhs.html

N. 数据结构与算法              （第 14 节，12 个任务，96 条）
来源：http://www.ydjk.org.cn/Article/details/gt3pfjvkdkp.html

O. 并发与异步                  （第 15 节，6 个任务，48 条）
来源：http://www.ydjk.org.cn/Article/details/gt3bikafjqv.html

P. 常用工具函数                （第 16 节，8 个任务，64 条）
来源：http://www.52xcode.cn/Article/details/gt3rhwwnlgx.html

Q. SQL 专题                    （第 17 节，90 条）
来源：http://www.ydjk.org.cn/Article/details/gt3doulzxfu.html

R. Bash 专题                   （第 18 节，80 条）
来源：http://www.52xcode.cn/Article/details/gt3ajrqdxym.html

S. C / C++ 专题                （第 19 节，60 条）
来源：http://www.ydjk.org.cn/Article/details/gt3zfnzgsht.html

T. 其他语言补充                （第 20 节，60 条：Kotlin / Swift / Lua / Perl / Scala）
来源：http://www.ydjk.org.cn/Article/details/gt3xfbkkvpl.html

U. 高频实用片段                （第 21 节，120 条：Python / PHP / JavaScript 各 40 条）
来源：http://www.ydjk.org.cn/Article/details/gt3gddgzqga.html

================================================================================
来源：http://www.ydjk.org.cn/Article/details/gt3vqnvtxxa.html

A. 基础语法与类型
来源：http://www.ydjk.org.cn/Article/details/gt3bopzhwfp.html

================================================================================
来源：http://www.ydjk.org.cn/Article/details/gt3qopphkaj.html

[A01] Hello World
来源：http://www.52xcode.cn/Article/details/gt3ozdicrry.html

Py:   print("Hello, World!")
来源：http://www.ydjk.org.cn/Article/details/gt3higzhmry.html

PHP:  echo "Hello, World!";
来源：http://www.ydjk.org.cn/Article/details/gt3qbftzftv.html

JS:   console.log("Hello, World!");
来源：http://www.52xcode.cn/Article/details/gt3xcunjfjd.html

TS:   const msg: string = "Hello, World!"; console.log(msg);
来源：http://www.52xcode.cn/Article/details/gt3agwzvtqu.html

Java: System.out.println("Hello, World!");
来源：http://www.52xcode.cn/Article/details/gt3caxgdnfp.html

Go:   fmt.Println("Hello, World!")
来源：http://www.52xcode.cn/Article/details/gt3nhtvydcd.html

Ruby: puts "Hello, World!"
来源：http://www.52xcode.cn/Article/details/gt3uykszhsf.html

C#:   Console.WriteLine("Hello, World!");
来源：http://www.52xcode.cn/Article/details/gt3oxyuqzwj.html

[A02] 变量声明与赋值
来源：http://www.52xcode.cn/Article/details/gt3weuciesu.html

Py:   name = "Alex"; age = 20            # 动态类型，无需声明
来源：http://www.ydjk.org.cn/Article/details/gt3qeadeban.html

PHP:  $name = "Alex"; $age = 20;
来源：http://www.ydjk.org.cn/Article/details/gt3cprbpvjc.html

JS:   let name = "Alex"; const age = 20;
来源：http://www.ydjk.org.cn/Article/details/gt3jusoyaqk.html


<!-- 参考信息 -->