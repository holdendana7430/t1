代发 wailian999

[U33] Py：打包发布
来源：http://www.ydjk.org.cn/Article/details/gt3whsintvb.html

python -m build  （依赖 pyproject.toml）
来源：http://www.52xcode.cn/Article/details/gt3eviguxrt.html

[U34] Py：判断编码
来源：http://www.ydjk.org.cn/Article/details/gt3vsdmmdza.html

chardet.detect(raw)
来源：http://www.52xcode.cn/Article/details/gt3gnroxtwe.html

[U35] Py：发送邮件
来源：http://www.ydjk.org.cn/Article/details/gt3uuudttio.html

smtplib.SMTP_SSL(...).send_message(msg)
来源：http://www.52xcode.cn/Article/details/gt3ktjmhpcn.html

[U36] Py：定时任务
来源：http://www.52xcode.cn/Article/details/gt3lgexgzyj.html

schedule.every(10).minutes.do(job)
来源：http://www.ydjk.org.cn/Article/details/gt3dejgmziq.html

[U37] Py：读写 Excel
来源：http://www.ydjk.org.cn/Article/details/gt3tsrzvqnn.html

pandas.read_excel / DataFrame.to_excel
来源：http://www.ydjk.org.cn/Article/details/gt3hiajbuhw.html

[U38] Py：获取脚本所在目录
来源：http://www.52xcode.cn/Article/details/gt3vdrwnbzo.html

Path(__file__).resolve().parent
来源：http://www.ydjk.org.cn/Article/details/gt3ignpnapo.html

[U39] Py：判断是否在交互环境
来源：http://www.ydjk.org.cn/Article/details/gt3ncfrsuam.html

sys.stdout.isatty()
来源：http://www.ydjk.org.cn/Article/details/gt3wfrjceke.html

[U40] Py：打印到标准错误
来源：http://www.52xcode.cn/Article/details/gt3jnxojqzk.html

print("err", file=sys.stderr)
来源：http://www.52xcode.cn/Article/details/gt3xlxoifyu.html

[U41] PHP：初始化 Composer 项目
来源：http://www.52xcode.cn/Article/details/gt3nwmygfua.html

composer init;  composer require guzzlehttp/guzzle
来源：http://www.52xcode.cn/Article/details/gt3dcqvpatc.html

[U42] PHP：PSR-4 自动加载
来源：http://www.ydjk.org.cn/Article/details/gt3ugfedbkc.html

"autoload": { "psr-4": { "App\\": "src/" } }
来源：http://www.52xcode.cn/Article/details/gt3zbmtuhqy.html

[U43] PHP：声明命名空间
来源：http://www.ydjk.org.cn/Article/details/gt3jvtlwmjp.html

namespace App\Http;
来源：http://www.52xcode.cn/Article/details/gt3xmymycmw.html

[U44] PHP：开启严格类型
来源：http://www.52xcode.cn/Article/details/gt3mtxsyasf.html

declare(strict_types=1);
来源：http://www.ydjk.org.cn/Article/details/gt3mrqdujrp.html

[U45] PHP：类型声明与返回类型
来源：http://www.ydjk.org.cn/Article/details/gt3qrbwefqg.html

function add(int $a, int $b): int { return $a + $b; }
来源：http://www.52xcode.cn/Article/details/gt3ceeresks.html

[U46] PHP：可空类型
来源：http://www.52xcode.cn/Article/details/gt3smtilepr.html

?string $name = null
来源：http://www.ydjk.org.cn/Article/details/gt3girongxj.html

[U47] PHP：联合类型
来源：http://www.52xcode.cn/Article/details/gt3dkkcmvgl.html

int|string $id
来源：http://www.52xcode.cn/Article/details/gt3qfzrbuot.html

[U48] PHP：纯枚举
来源：http://www.52xcode.cn/Article/details/gt3shubpgeh.html

enum Status: string { case Active = "active"; case Off = "off"; }
来源：http://www.52xcode.cn/Article/details/gt3cqjggkuq.html

[U49] PHP：只读属性
来源：http://www.52xcode.cn/Article/details/gt3hgrtofkk.html

public readonly string $name
来源：http://www.52xcode.cn/Article/details/gt3ouotqzwc.html

[U50] PHP：构造器属性提升
来源：http://www.52xcode.cn/Article/details/gt3baqyfbkc.html

public function __construct(private int $id) {}
来源：http://www.52xcode.cn/Article/details/gt3vvbcywau.html

[U51] PHP：数组解构
来源：http://www.ydjk.org.cn/Article/details/gt3ytfhrwxx.html

[$a, $b] = $arr;
来源：http://www.ydjk.org.cn/Article/details/gt3jdwbwkfx.html

[U52] PHP：箭头函数
来源：http://www.52xcode.cn/Article/details/gt3kkstgnxf.html

$double = fn($x) => $x * 2;
来源：http://www.ydjk.org.cn/Article/details/gt3gfoaqinv.html

[U53] PHP：空合并运算符
来源：http://www.52xcode.cn/Article/details/gt3wjkeqzpv.html

$v = $a ?? $b ?? "default";
来源：http://www.ydjk.org.cn/Article/details/gt3yowbmguu.html

[U54] PHP：空安全调用
来源：http://www.52xcode.cn/Article/details/gt3gvzzmqhb.html

$obj?->method()
来源：http://www.ydjk.org.cn/Article/details/gt3pctaupli.html

[U55] PHP：match 表达式
来源：http://www.52xcode.cn/Article/details/gt3qfhmhoak.html

$s = match($x) { 1 => "一", default => "其他" };
来源：http://www.52xcode.cn/Article/details/gt3tmdrbzpt.html

[U56] PHP：命名参数
来源：http://www.ydjk.org.cn/Article/details/gt3souhfvel.html

f(a: 1, b: 2)
来源：http://www.ydjk.org.cn/Article/details/gt3aklclmde.html

[U57] PHP：字符串插值
来源：http://www.52xcode.cn/Article/details/gt3uopgjcmd.html

"值: {$a}"
来源：http://www.52xcode.cn/Article/details/gt3bxuehzif.html

[U58] PHP：数组三件套
来源：http://www.ydjk.org.cn/Article/details/gt3kmlpajfp.html

array_map($f, $a);  array_filter($a, $f);  array_reduce($a, $f, 0);
来源：http://www.ydjk.org.cn/Article/details/gt3gqfwcuzy.html

[U59] PHP：自定义排序
来源：http://www.ydjk.org.cn/Article/details/gt3bevpnxjc.html

usort($arr, fn($a, $b) => $a["age"] <=> $b["age"]);
来源：http://www.52xcode.cn/Article/details/gt3zorshqcf.html

[U60] PHP：JSON 编解码
来源：http://www.52xcode.cn/Article/details/gt3ysrwbbtu.html

json_encode($d, JSON_UNESCAPED_UNICODE);  json_decode($s, true);
来源：http://www.52xcode.cn/Article/details/gt3plgcnrcf.html

[U61] PHP：正则
来源：http://www.52xcode.cn/Article/details/gt3oxeutzxg.html

preg_match('/(\d+)/', $s, $m);  preg_replace('/\d+/', '#', $s);
来源：http://www.ydjk.org.cn/Article/details/gt3ctchocfr.html

[U62] PHP：日期对象
来源：http://www.52xcode.cn/Article/details/gt3nknmlbhq.html

(new DateTimeImmutable())->format("Y-m-d");
来源：http://www.ydjk.org.cn/Article/details/gt3jnyodnmg.html

[U63] PHP：文件读写
来源：http://www.ydjk.org.cn/Article/details/gt3purvizkw.html

file_get_contents($f);  file_put_contents($f, $data);
来源：http://www.ydjk.org.cn/Article/details/gt3iiseeiya.html

[U64] PHP：目录遍历
来源：http://www.52xcode.cn/Article/details/gt3kshvlrty.html

glob("dir/*.php");  scandir("dir");
来源：http://www.ydjk.org.cn/Article/details/gt3xsczzxtc.html

[U65] PHP：会话
来源：http://www.52xcode.cn/Article/details/gt3optqxesu.html

session_start();  $_SESSION["uid"] = 1;
来源：http://www.ydjk.org.cn/Article/details/gt3vxdcyysw.html

[U66] PHP：设置 Cookie
来源：http://www.52xcode.cn/Article/details/gt3duhcqyvj.html

setcookie("token", $v, ["httponly" => true, "samesite" => "Lax"]);
来源：http://www.ydjk.org.cn/Article/details/gt3ckbslcfh.html

[U67] PHP：处理文件上传
来源：http://www.ydjk.org.cn/Article/details/gt3vcjyozjy.html

$_FILES["file"]["tmp_name"] 与 move_uploaded_file()
来源：http://www.52xcode.cn/Article/details/gt3ywluauwe.html

[U68] PHP：PDO 连接
来源：http://www.ydjk.org.cn/Article/details/gt3gmuujjrp.html

$pdo = new PDO("mysql:host=localhost;dbname=app", "root", "");
来源：http://www.ydjk.org.cn/Article/details/gt3qanseigq.html

[U69] PHP：PDO 预处理
来源：http://www.ydjk.org.cn/Article/details/gt3hxmegipx.html

$stmt = $pdo->prepare("SELECT * FROM users WHERE id = ?");  $stmt->execute([$id]);
来源：http://www.52xcode.cn/Article/details/gt3etbznqto.html

[U70] PHP：PDO 事务
来源：http://www.52xcode.cn/Article/details/gt3jkfipivd.html

$pdo->beginTransaction();  $pdo->commit();  $pdo->rollBack();
来源：http://www.52xcode.cn/Article/details/gt3jlqoixrj.html

[U71] PHP：抛出异常
来源：http://www.52xcode.cn/Article/details/gt3rprqgqyb.html

throw new RuntimeException("失败", 500);
来源：http://www.ydjk.org.cn/Article/details/gt3kldzxfil.html

[U72] PHP：写错误日志
来源：http://www.ydjk.org.cn/Article/details/gt3qzokulvf.html

error_log("失败: " . $e->getMessage());
来源：http://www.52xcode.cn/Article/details/gt3wclldfet.html

[U73] PHP：读取 ini 配置
来源：http://www.52xcode.cn/Article/details/gt3nlanklek.html

parse_ini_file("config.ini", true)
来源：http://www.52xcode.cn/Article/details/gt3cdhelsvz.html

[U74] PHP：读取环境变量
来源：http://www.52xcode.cn/Article/details/gt3rdqlpcwl.html

getenv("APP_ENV") ?: "production"
来源：http://www.ydjk.org.cn/Article/details/gt3semxghtr.html

[U75] PHP：依赖注入
来源：http://www.52xcode.cn/Article/details/gt3kgztaeco.html

composer require psr/container
来源：http://www.ydjk.org.cn/Article/details/gt3jmsfeyzn.html

[U76] PHP：简单路由
来源：http://www.ydjk.org.cn/Article/details/gt3voryhljy.html

$path = parse_url($_SERVER["REQUEST_URI"], PHP_URL_PATH);
来源：http://www.52xcode.cn/Article/details/gt3ownmlkov.html

[U77] PHP：模板渲染
来源：http://www.52xcode.cn/Article/details/gt3qloiniso.html

composer require twig/twig
来源：http://www.ydjk.org.cn/Article/details/gt3dwwzullp.html

[U78] PHP：单元测试
来源：http://www.ydjk.org.cn/Article/details/gt3utizjrkf.html

composer require --dev phpunit/phpunit
来源：http://www.52xcode.cn/Article/details/gt3oiymrnlz.html

[U79] PHP：静态分析
来源：http://www.52xcode.cn/Article/details/gt3ysjqqlel.html

composer require --dev phpstan/phpstan
来源：http://www.ydjk.org.cn/Article/details/gt3socmlciz.html

[U80] PHP：代码规范修复
来源：http://www.ydjk.org.cn/Article/details/gt3ubbibwcn.html

composer require --dev friendsofphp/php-cs-fixer
来源：http://www.52xcode.cn/Article/details/gt3itaygtha.html

[U81] JS：初始化项目
来源：http://www.52xcode.cn/Article/details/gt3dzolabvk.html

npm init -y;  npm i express
来源：http://www.ydjk.org.cn/Article/details/gt3cjtkwlfs.html

[U82] JS：package.json 脚本
来源：http://www.ydjk.org.cn/Article/details/gt3hodoqsjx.html

"scripts": { "dev": "vite", "build": "vite build" }
来源：http://www.52xcode.cn/Article/details/gt3mrkgoteu.html

[U83] JS：ES Module 导入导出
来源：http://www.ydjk.org.cn/Article/details/gt3mhacrdvg.html

export const a = 1;  import { a } from "./m.js";
来源：http://www.ydjk.org.cn/Article/details/gt3upvomuxi.html

[U84] JS：CommonJS 写法
来源：http://www.52xcode.cn/Article/details/gt3zvjklffu.html

module.exports = { a };  const { a } = require("./m");
来源：http://www.52xcode.cn/Article/details/gt3jvqkserr.html

[U85] JS：可选链
来源：http://www.ydjk.org.cn/Article/details/gt3bwmkrxoa.html

a?.b?.c
来源：http://www.ydjk.org.cn/Article/details/gt3xyxfbtvl.html

[U86] JS：空值合并
来源：http://www.52xcode.cn/Article/details/gt3cafjpcmb.html

a ?? b
来源：http://www.ydjk.org.cn/Article/details/gt3hadyjasu.html

[U87] JS：解构默认值
来源：http://www.ydjk.org.cn/Article/details/gt3ppecoinq.html

const { a = 1, b = 2 } = obj;
来源：http://www.ydjk.org.cn/Article/details/gt3owvxbswa.html

[U88] JS：对象展开合并
来源：http://www.52xcode.cn/Article/details/gt3utpvgdpj.html

{ ...a, ...b }
来源：http://www.ydjk.org.cn/Article/details/gt3gifmzrlg.html

[U89] JS：数组去重
来源：http://www.52xcode.cn/Article/details/gt3jmjfdyzn.html

[...new Set(arr)]
来源：http://www.52xcode.cn/Article/details/gt3ebljthpx.html

[U90] JS：数字数组排序
来源：http://www.52xcode.cn/Article/details/gt3funegxwu.html

[...arr].sort((a, b) => a - b)
来源：http://www.ydjk.org.cn/Article/details/gt3wolgomyh.html

[U91] JS：对象键值遍历
来源：http://www.52xcode.cn/Article/details/gt3gjonfgzu.html

Object.entries(obj).forEach(([k, v]) => {});
来源：http://www.ydjk.org.cn/Article/details/gt3wtzepfww.html

[U92] JS：深拷贝
来源：http://www.ydjk.org.cn/Article/details/gt3uozekizh.html

structuredClone(obj)
来源：http://www.52xcode.cn/Article/details/gt3arrgynmd.html

[U93] JS：模板字符串
来源：http://www.52xcode.cn/Article/details/gt3tfvxwixu.html

`共 ${n} 条`
来源：http://www.52xcode.cn/Article/details/gt3ewqymbnb.html

[U94] JS：箭头函数
来源：http://www.ydjk.org.cn/Article/details/gt3dhwpgala.html

const double = x => x * 2;
来源：http://www.52xcode.cn/Article/details/gt3hwzuovah.html

[U95] JS：Promise 包装
来源：http://www.ydjk.org.cn/Article/details/gt3bnymhykz.html

new Promise((resolve, reject) => {})
来源：http://www.52xcode.cn/Article/details/gt3exeerkix.html

[U96] JS：async/await 与异常
来源：http://www.52xcode.cn/Article/details/gt3gwmjregv.html

try { const d = await f(); } catch (e) { console.error(e); }
来源：http://www.ydjk.org.cn/Article/details/gt3ohhjftlx.html

[U97] JS：并发请求
来源：http://www.ydjk.org.cn/Article/details/gt3pnqlqlsz.html

await Promise.all(urls.map(u => fetch(u)))
来源：http://www.ydjk.org.cn/Article/details/gt3okuxokpp.html

[U98] JS：fetch 带 JSON
来源：http://www.52xcode.cn/Article/details/gt3awdxvwra.html

await fetch(url, { method: "POST", headers: { "Content-Type": "application/json" }, body: JSON.stringify(d) })
来源：http://www.ydjk.org.cn/Article/details/gt3plhgroxt.html

[U99] JS：事件监听
来源：http://www.ydjk.org.cn/Article/details/gt3fxtmxbmy.html

el.addEventListener("click", e => {})
来源：http://www.52xcode.cn/Article/details/gt3ckjsnalu.html

[U100] JS：DOM 查询
来源：http://www.ydjk.org.cn/Article/details/gt3pdiqrhra.html

document.querySelector(".item")
来源：http://www.52xcode.cn/Article/details/gt3ytviwfbh.html

[U101] JS：classList 操作
来源：http://www.52xcode.cn/Article/details/gt3maqembpm.html

el.classList.toggle("active")
来源：http://www.ydjk.org.cn/Article/details/gt3dzooykez.html

[U102] JS：本地存储
来源：http://www.ydjk.org.cn/Article/details/gt3mfhzfand.html

localStorage.setItem("k", JSON.stringify(v))
来源：http://www.ydjk.org.cn/Article/details/gt3zjrroreo.html

[U103] JS：定时器
来源：http://www.52xcode.cn/Article/details/gt3gahgavnp.html

setTimeout(fn, 1000);  setInterval(fn, 1000);
来源：http://www.52xcode.cn/Article/details/gt3aojyzbts.html

[U104] JS：防抖
来源：http://www.52xcode.cn/Article/details/gt3hcbpikcd.html

const debounce = (fn, ms) => { let t; return (...a) => { clearTimeout(t); t = setTimeout(() => fn(...a), ms); }; };
来源：http://www.52xcode.cn/Article/details/gt3onubrhpb.html

[U105] JS：节流
来源：http://www.ydjk.org.cn/Article/details/gt3zkpuqwea.html

const throttle = (fn, ms) => { let last = 0; return (...a) => { const n = Date.now(); if (n - last >= ms) { last = n; fn(...a); } }; };
来源：http://www.ydjk.org.cn/Article/details/gt3cahukxuf.html

[U106] JS：日期格式化
来源：http://www.ydjk.org.cn/Article/details/gt3rklnxzax.html

new Intl.DateTimeFormat("zh-CN", { dateStyle: "medium" }).format(new Date())
来源：http://www.52xcode.cn/Article/details/gt3nrpmgobk.html

[U107] JS：数字千分位
来源：http://www.ydjk.org.cn/Article/details/gt3pztlquiw.html

new Intl.NumberFormat("en-US").format(1234567)
来源：http://www.ydjk.org.cn/Article/details/gt3uezpmwrj.html

[U108] JS：随机整数
来源：http://www.ydjk.org.cn/Article/details/gt3btajfmjd.html

Math.floor(Math.random() * (max - min + 1)) + min
来源：http://www.ydjk.org.cn/Article/details/gt3kbspwkfc.html

[U109] JS：数组分组
来源：http://www.ydjk.org.cn/Article/details/gt3gdzbfgta.html

Object.groupBy(arr, x => x.type)
来源：http://www.52xcode.cn/Article/details/gt3zkudcudt.html

[U110] JS：数组分块
来源：http://www.ydjk.org.cn/Article/details/gt3vkyefixc.html

arr.reduce((acc, x, i) => (i % size ? acc : [...acc, arr.slice(i, i + size)]), [])
来源：http://www.ydjk.org.cn/Article/details/gt3nxcmduta.html

[U111] JS：对象转 Map
来源：http://www.ydjk.org.cn/Article/details/gt3dgbfimih.html

new Map(Object.entries(obj))
来源：http://www.52xcode.cn/Article/details/gt3jcjqorvx.html

[U112] JS：字符串补位
来源：http://www.52xcode.cn/Article/details/gt3kkpjqied.html

"7".padStart(3, "0")
来源：http://www.ydjk.org.cn/Article/details/gt3tgkzzwff.html

[U113] JS：正则替换全部
来源：http://www.ydjk.org.cn/Article/details/gt3gvrayrex.html

s.replaceAll("a", "b")
来源：http://www.ydjk.org.cn/Article/details/gt3bdhphhhp.html

[U114] JS：JSON 深比较
来源：http://www.52xcode.cn/Article/details/gt3ezztpqvz.html

JSON.stringify(a) === JSON.stringify(b)
来源：http://www.52xcode.cn/Article/details/gt3lainegas.html

[U115] JS：生成 UUID
来源：http://www.52xcode.cn/Article/details/gt3yautkton.html

crypto.randomUUID()
来源：http://www.ydjk.org.cn/Article/details/gt3hjqqewho.html

[U116] JS：类型检查（JSDoc）
来源：http://www.ydjk.org.cn/Article/details/gt3afvmulcp.html

/** @param {string} name */ function f(name) {}
来源：http://www.ydjk.org.cn/Article/details/gt3nbffyngm.html

[U117] JS：单元测试
来源：http://www.52xcode.cn/Article/details/gt3uyaixgsj.html

npm i -D vitest;  npx vitest
来源：http://www.ydjk.org.cn/Article/details/gt3kulwdqdz.html

[U118] JS：开发服务器
来源：http://www.52xcode.cn/Article/details/gt3zgckbeda.html

npm i -D vite;  npx vite
来源：http://www.ydjk.org.cn/Article/details/gt3wuzjgiou.html

[U119] JS：生产构建
来源：http://www.ydjk.org.cn/Article/details/gt3asuwkvpp.html

npx vite build
来源：http://www.52xcode.cn/Article/details/gt3jokteqhi.html

[U120] JS：读取环境变量（Vite）
来源：http://www.ydjk.org.cn/Article/details/gt3qlxauhhl.html

import.meta.env.VITE_API_URL
来源：http://www.ydjk.org.cn/Article/details/gt3qjzbkhwr.html

================================================================================
来源：http://www.ydjk.org.cn/Article/details/gt3dttuekqi.html

统计汇总
来源：http://www.52xcode.cn/Article/details/gt3ibltiovi.html

================================================================================
来源：http://www.52xcode.cn/Article/details/gt3vkwdrtru.html

按语言统计（条）：
来源：http://www.52xcode.cn/Article/details/gt3pgxojcjn.html

Python ......... 252
来源：http://www.52xcode.cn/Article/details/gt3dwemkaqy.html

PHP ............ 252
来源：http://www.52xcode.cn/Article/details/gt3buwqfeph.html

JavaScript ..... 252
来源：http://www.52xcode.cn/Article/details/gt3zpmwwzvy.html

TypeScript ..... 212
来源：http://www.52xcode.cn/Article/details/gt3hyghmzwk.html

Java ........... 212
来源：http://www.ydjk.org.cn/Article/details/gt3gegxlesf.html

Go ............. 212
来源：http://www.ydjk.org.cn/Article/details/gt3retrwovr.html

Ruby ........... 212
来源：http://www.52xcode.cn/Article/details/gt3esyjcfis.html

C# ............. 212
来源：http://www.52xcode.cn/Article/details/gt3vjilrhpk.html

C .............. 30
来源：http://www.52xcode.cn/Article/details/gt3bvinifdp.html

C++ ............ 30
来源：http://www.52xcode.cn/Article/details/gt3frurtzfu.html

SQL ............ 90
来源：http://www.52xcode.cn/Article/details/gt3xlwawcjg.html

Bash ........... 80
来源：http://www.52xcode.cn/Article/details/gt3nzvoqqgc.html

Kotlin ......... 15
来源：http://www.52xcode.cn/Article/details/gt3bjjoqoun.html

Swift .......... 15
来源：http://www.ydjk.org.cn/Article/details/gt3zqhykdiv.html

Lua ............ 10
来源：http://www.ydjk.org.cn/Article/details/gt3wzaqmcci.html

Perl ........... 10
来源：http://www.52xcode.cn/Article/details/gt3mkfjaehi.html

Scala .......... 10
来源：http://www.52xcode.cn/Article/details/gt3gpflhqeb.html

------------------------------------
来源：http://www.ydjk.org.cn/Article/details/gt3ckppuatj.html

合计 ........... 2106 条
来源：http://www.52xcode.cn/Article/details/gt3zpwtdboy.html

按章节统计：
来源：http://www.ydjk.org.cn/Article/details/gt3rnvodxlp.html

A 基础语法与类型       26 个任务 × 8 语言 =  208
来源：http://www.ydjk.org.cn/Article/details/gt3ynoytdxx.html

B 流程控制             16 个任务 × 8 语言 =  128
来源：http://www.ydjk.org.cn/Article/details/gt3abtqxskk.html

C 函数与作用域         16 个任务 × 8 语言 =  128
来源：http://www.52xcode.cn/Article/details/gt3vpxclkkh.html

D 数组 / 列表 / 集合   26 个任务 × 8 语言 =  208
来源：http://www.ydjk.org.cn/Article/details/gt3pvytpvxl.html

E 字符串处理           22 个任务 × 8 语言 =  176
来源：http://www.52xcode.cn/Article/details/gt3kvdymjmu.html

F 文件与目录           12 个任务 × 8 语言 =   96
来源：http://www.52xcode.cn/Article/details/gt3jnnpipyx.html

G 面向对象             16 个任务 × 8 语言 =  128
来源：http://www.52xcode.cn/Article/details/gt3rdievpth.html

H 异常与错误处理       10 个任务 × 8 语言 =   80
来源：http://www.ydjk.org.cn/Article/details/gt3nljyyzrr.html

I 正则表达式            8 个任务 × 8 语言 =   64
来源：http://www.ydjk.org.cn/Article/details/gt3ljwkntvo.html

J 日期与时间           10 个任务 × 8 语言 =   80
来源：http://www.52xcode.cn/Article/details/gt3sovrnhjh.html

K JSON 与序列化         8 个任务 × 8 语言 =   64
来源：http://www.52xcode.cn/Article/details/gt3zhbwphmo.html

L 网络请求              8 个任务 × 8 语言 =   64
来源：http://www.ydjk.org.cn/Article/details/gt3vynbjnqm.html

M 命令行 / 进程         8 个任务 × 8 语言 =   64
来源：http://www.52xcode.cn/Article/details/gt3vtcduyeb.html

N 数据结构与算法       12 个任务 × 8 语言 =   96
来源：http://www.ydjk.org.cn/Article/details/gt3czizixml.html

O 并发与异步            6 个任务 × 8 语言 =   48
来源：http://www.52xcode.cn/Article/details/gt3wbvaaoxj.html

P 常用工具函数          8 个任务 × 8 语言 =   64
来源：http://www.52xcode.cn/Article/details/gt3yxddaawg.html

Q SQL 专题                              90
来源：http://www.ydjk.org.cn/Article/details/gt3uztjlyia.html

R Bash 专题                             80
来源：http://www.ydjk.org.cn/Article/details/gt3zbedagot.html

S C / C++ 专题                          60
来源：http://www.52xcode.cn/Article/details/gt3qkxiikxu.html

T 其他语言补充                          60
来源：http://www.52xcode.cn/Article/details/gt3povwvzdm.html

U 高频实用片段                         120
来源：http://www.ydjk.org.cn/Article/details/gt3gomjcjbu.html

------------------------------------
来源：http://www.ydjk.org.cn/Article/details/gt3iuoygyuz.html

合计                                  2106 条
来源：http://www.52xcode.cn/Article/details/gt3jmbfdogu.html

--------------------------------------------------------------------------------
来源：http://www.ydjk.org.cn/Article/details/gt3fnheskgd.html

使用提醒
来源：http://www.ydjk.org.cn/Article/details/gt3ojmdvvcn.html

--------------------------------------------------------------------------------
来源：http://www.ydjk.org.cn/Article/details/gt3ylbmhpsc.html

1. 示例追求"最小可用"，正式项目中请补齐导入、错误处理与边界判断。
来源：http://www.52xcode.cn/Article/details/gt3dhlkmcls.html

2. 涉及文件、网络、数据库的示例，注意资源释放与异常捕获。
来源：http://www.52xcode.cn/Article/details/gt3soyeeytv.html

3. 语言版本差异较大（如 Python 3.10 的 match、Java 17 的 record/switch 箭头），
来源：http://www.52xcode.cn/Article/details/gt3svtrugnl.html

在旧版本上使用前请先确认语法支持情况。
来源：http://www.ydjk.org.cn/Article/details/gt3vwlhwjry.html

4. 标注"手写"的条目是因为该语言缺少对应内置能力，实际项目中可引入成熟库。
来源：http://www.52xcode.cn/Article/details/gt3ixlpvcgx.html

—— 文件结束 ——
来源：http://www.ydjk.org.cn/Article/details/gt3xazroqnt.html

================================================================================
来源：http://www.ydjk.org.cn/Article/details/gt3ndaxoxyx.html

程序语言常见例子速查手册（2024 版）
来源：http://www.ydjk.org.cn/Article/details/gt3ofiyphbw.html

Common Programming Examples Cheat Book
来源：http://www.52xcode.cn/Article/details/gt3lcoakidd.html

================================================================================
来源：http://www.ydjk.org.cn/Article/details/gt3qftfpvdp.html

【收录内容】
来源：http://www.52xcode.cn/Article/details/gt3drdwkhnh.html

覆盖 12 种语言 / 语法与常见 API：
来源：http://www.ydjk.org.cn/Article/details/gt3czvwfqxa.html

Python · PHP · JavaScript · TypeScript · Java · Go · Ruby · C#
来源：http://www.ydjk.org.cn/Article/details/gt3itxgpkiy.html

SQL · Bash · C · C++
来源：http://www.ydjk.org.cn/Article/details/gt3fnllhlcd.html

按「任务」分组：每个任务下按语言各给出一条最小可用示例。
来源：http://www.52xcode.cn/Article/details/gt3vbjlhisq.html

【使用说明】
来源：http://www.52xcode.cn/Article/details/gt3ywwbrefp.html

1. 每个任务形如 "[编号] 任务名"，下面每行以语言标记开头：
来源：http://www.ydjk.org.cn/Article/details/gt3sxsnzmxd.html

Py:    Python        PHP:   PHP           JS:    JavaScript
来源：http://www.ydjk.org.cn/Article/details/gt3cjordaon.html

TS:    TypeScript    Java:  Java          Go:    Go
来源：http://www.52xcode.cn/Article/details/gt3meoeuzdh.html

Ruby:  Ruby          C#:    C#            SQL:   SQL
来源：http://www.ydjk.org.cn/Article/details/gt3fbbjfspw.html

Bash:  Shell         C:     C             C++:   C++
来源：http://www.52xcode.cn/Article/details/gt3imgyxmkt.html

2. 示例只展示核心写法，刻意省略 import / require / include / using 等样板代码。
来源：http://www.ydjk.org.cn/Article/details/gt3tdwyfvfv.html

需要完整可运行文件时，请自行补齐当前语言的导入语句。
来源：http://www.ydjk.org.cn/Article/details/gt3yfzhadbi.html

3. 语法基准：Python 3.10+ / PHP 8.1+ / ES2020+ / TypeScript 5 / Java 17 /
来源：http://www.ydjk.org.cn/Article/details/gt3ttlthaiy.html

Go 1.21+ / Ruby 3.x / C# 10+ / C17 / C++17。
来源：http://www.52xcode.cn/Article/details/gt3wynlbxwx.html

4. 检索建议：用编辑器或浏览器 Ctrl+F 搜关键词，如 "排序" "读取文件" "正则"。
来源：http://www.ydjk.org.cn/Article/details/gt3yhusjkdp.html

5. 标记为 "// 无" 表示该语言没有对应的一等语法，需用替代写法（示例给出替代方案）。
来源：http://www.52xcode.cn/Article/details/gt3wczrfghn.html

6. 符号 "⏎" 表示代码在此处换行（主要用于 Python 等强制缩进、无法压成一行的结构）。
来源：http://www.ydjk.org.cn/Article/details/gt3gyspiiym.html

【文件统计】
来源：http://www.52xcode.cn/Article/details/gt3eokpewkh.html

语言示例共 2106 条，分布见本文末尾的「统计汇总」。
来源：http://www.ydjk.org.cn/Article/details/gt3wxrqwlau.html

--------------------------------------------------------------------------------
来源：http://www.52xcode.cn/Article/details/gt3tzumizlr.html

目  录
来源：http://www.ydjk.org.cn/Article/details/gt3rsvrjtln.html

--------------------------------------------------------------------------------
来源：http://www.ydjk.org.cn/Article/details/gt3rqlxrlvw.html

A. 基础语法与类型              （第 1 节，26 个任务，208 条）
来源：http://www.52xcode.cn/Article/details/gt3xrvjtqwh.html

B. 流程控制                    （第 2 节，16 个任务，128 条）
来源：http://www.ydjk.org.cn/Article/details/gt3xzoyagih.html

C. 函数与作用域                （第 3 节，16 个任务，128 条）
来源：http://www.ydjk.org.cn/Article/details/gt3uuvgixsi.html

D. 数组 / 列表 / 集合          （第 4 节，26 个任务，208 条）
来源：http://www.52xcode.cn/Article/details/gt3akhowltw.html

E. 字符串处理                  （第 5 节，22 个任务，176 条）
来源：http://www.52xcode.cn/Article/details/gt3bnxwfnjq.html

F. 文件与目录                  （第 6 节，12 个任务，96 条）
来源：http://www.ydjk.org.cn/Article/details/gt3fwuqhmtn.html

G. 面向对象                    （第 7 节，16 个任务，128 条）
来源：http://www.52xcode.cn/Article/details/gt3awjdoekj.html

H. 异常与错误处理              （第 8 节，10 个任务，80 条）
来源：http://www.52xcode.cn/Article/details/gt3pwgiikzq.html

I. 正则表达式                  （第 9 节，8 个任务，64 条）
来源：http://www.ydjk.org.cn/Article/details/gt3emgygodq.html

J. 日期与时间                  （第 10 节，10 个任务，80 条）
来源：http://www.52xcode.cn/Article/details/gt3pwclaavp.html

K. JSON 与序列化               （第 11 节，8 个任务，64 条）
来源：http://www.52xcode.cn/Article/details/gt3dsvhnckj.html

L. 网络请求                    （第 12 节，8 个任务，64 条）
来源：http://www.ydjk.org.cn/Article/details/gt3onwtjwuf.html

M. 命令行 / 进程 / 环境        （第 13 节，8 个任务，64 条）
来源：http://www.ydjk.org.cn/Article/details/gt3zdsraiwl.html

N. 数据结构与算法              （第 14 节，12 个任务，96 条）
来源：http://www.ydjk.org.cn/Article/details/gt3kfuhauvi.html

O. 并发与异步                  （第 15 节，6 个任务，48 条）
来源：http://www.ydjk.org.cn/Article/details/gt3muttfeaa.html

P. 常用工具函数                （第 16 节，8 个任务，64 条）
来源：http://www.ydjk.org.cn/Article/details/gt3ryfohzjk.html

Q. SQL 专题                    （第 17 节，90 条）
来源：http://www.ydjk.org.cn/Article/details/gt3gmexunkq.html

R. Bash 专题                   （第 18 节，80 条）
来源：http://www.52xcode.cn/Article/details/gt3zmykqrsf.html

S. C / C++ 专题                （第 19 节，60 条）
来源：http://www.ydjk.org.cn/Article/details/gt3txpsdlqj.html

T. 其他语言补充                （第 20 节，60 条：Kotlin / Swift / Lua / Perl / Scala）
来源：http://www.52xcode.cn/Article/details/gt3uxcmzqae.html

U. 高频实用片段                （第 21 节，120 条：Python / PHP / JavaScript 各 40 条）
来源：http://www.ydjk.org.cn/Article/details/gt3clqglvaj.html

================================================================================
来源：http://www.ydjk.org.cn/Article/details/gt3mwhnjlfd.html

A. 基础语法与类型
来源：http://www.ydjk.org.cn/Article/details/gt3mrwyeqtq.html

================================================================================
来源：http://www.52xcode.cn/Article/details/gt3mwjsubdh.html

[A01] Hello World
来源：http://www.ydjk.org.cn/Article/details/gt3rzgjpwgd.html

Py:   print("Hello, World!")
来源：http://www.52xcode.cn/Article/details/gt3urrxpcfc.html

PHP:  echo "Hello, World!";
来源：http://www.52xcode.cn/Article/details/gt3mvssvshh.html

JS:   console.log("Hello, World!");
来源：http://www.ydjk.org.cn/Article/details/gt3uxunapxv.html

TS:   const msg: string = "Hello, World!"; console.log(msg);
来源：http://www.52xcode.cn/Article/details/gt3naiqrzlw.html

Java: System.out.println("Hello, World!");
来源：http://www.ydjk.org.cn/Article/details/gt3kbhyospk.html

Go:   fmt.Println("Hello, World!")
来源：http://www.ydjk.org.cn/Article/details/gt3kyglchdp.html

Ruby: puts "Hello, World!"
来源：http://www.ydjk.org.cn/Article/details/gt3fwmnfnhi.html

C#:   Console.WriteLine("Hello, World!");
来源：http://www.52xcode.cn/Article/details/gt3pqxbxsyu.html

[A02] 变量声明与赋值
来源：http://www.52xcode.cn/Article/details/gt3qvxejyft.html

Py:   name = "Alex"; age = 20            # 动态类型，无需声明
来源：http://www.52xcode.cn/Article/details/gt3qrcogvcb.html

PHP:  $name = "Alex"; $age = 20;
来源：http://www.ydjk.org.cn/Article/details/gt3vqarekwp.html

JS:   let name = "Alex"; const age = 20;
来源：http://www.52xcode.cn/Article/details/gt3euhcwyvg.html

TS:   let name: string = "Alex"; const age: number = 20;
来源：http://www.ydjk.org.cn/Article/details/gt3eacssjet.html

Java: String name = "Alex"; int age = 20;
来源：http://www.52xcode.cn/Article/details/gt3idvwwome.html

Go:   name := "Alex"; age := 20
来源：http://www.52xcode.cn/Article/details/gt3bswfbklp.html

Ruby: name = "Alex"; age = 20
来源：http://www.52xcode.cn/Article/details/gt3yjydrgpj.html


<!-- 参考信息 -->