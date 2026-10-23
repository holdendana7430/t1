代发 wailian999

[U33] Py：打包发布
来源：http://www.52xcode.cn/Article/details/gt3zsyekahm.html

python -m build  （依赖 pyproject.toml）
来源：http://www.52xcode.cn/Article/details/gt3opbczjrj.html

[U34] Py：判断编码
来源：http://www.52xcode.cn/Article/details/gt3znbptapu.html

chardet.detect(raw)
来源：http://www.52xcode.cn/Article/details/gt3hghlgpfc.html

[U35] Py：发送邮件
来源：http://www.52xcode.cn/Article/details/gt3kpgeueac.html

smtplib.SMTP_SSL(...).send_message(msg)
来源：http://www.52xcode.cn/Article/details/gt3fpqzhrel.html

[U36] Py：定时任务
来源：http://www.ydjk.org.cn/Article/details/gt3kcqwmonh.html

schedule.every(10).minutes.do(job)
来源：http://www.52xcode.cn/Article/details/gt3hglubmaz.html

[U37] Py：读写 Excel
来源：http://www.52xcode.cn/Article/details/gt3nfyhchlo.html

pandas.read_excel / DataFrame.to_excel
来源：http://www.ydjk.org.cn/Article/details/gt3unqyaobj.html

[U38] Py：获取脚本所在目录
来源：http://www.ydjk.org.cn/Article/details/gt3gfjtpovo.html

Path(__file__).resolve().parent
来源：http://www.ydjk.org.cn/Article/details/gt3tupnnzst.html

[U39] Py：判断是否在交互环境
来源：http://www.ydjk.org.cn/Article/details/gt3ltohvcrb.html

sys.stdout.isatty()
来源：http://www.52xcode.cn/Article/details/gt3dfefvxoj.html

[U40] Py：打印到标准错误
来源：http://www.52xcode.cn/Article/details/gt3tcmlarly.html

print("err", file=sys.stderr)
来源：http://www.52xcode.cn/Article/details/gt3avpixuly.html

[U41] PHP：初始化 Composer 项目
来源：http://www.52xcode.cn/Article/details/gt3qabpwmzo.html

composer init;  composer require guzzlehttp/guzzle
来源：http://www.52xcode.cn/Article/details/gt3ktznuqfs.html

[U42] PHP：PSR-4 自动加载
来源：http://www.52xcode.cn/Article/details/gt3xjqdhygc.html

"autoload": { "psr-4": { "App\\": "src/" } }
来源：http://www.ydjk.org.cn/Article/details/gt3olwnypbo.html

[U43] PHP：声明命名空间
来源：http://www.52xcode.cn/Article/details/gt3zinpcmkv.html

namespace App\Http;
来源：http://www.ydjk.org.cn/Article/details/gt3kystvypu.html

[U44] PHP：开启严格类型
来源：http://www.ydjk.org.cn/Article/details/gt3bvjxwyik.html

declare(strict_types=1);
来源：http://www.ydjk.org.cn/Article/details/gt3oxqpujpd.html

[U45] PHP：类型声明与返回类型
来源：http://www.ydjk.org.cn/Article/details/gt3kooajowl.html

function add(int $a, int $b): int { return $a + $b; }
来源：http://www.52xcode.cn/Article/details/gt3vlgxrgza.html

[U46] PHP：可空类型
来源：http://www.52xcode.cn/Article/details/gt3mzpmpfin.html

?string $name = null
来源：http://www.ydjk.org.cn/Article/details/gt3owfpflij.html

[U47] PHP：联合类型
来源：http://www.52xcode.cn/Article/details/gt3tlrqmmsb.html

int|string $id
来源：http://www.ydjk.org.cn/Article/details/gt3plpaxwwi.html

[U48] PHP：纯枚举
来源：http://www.52xcode.cn/Article/details/gt3nuuunnrz.html

enum Status: string { case Active = "active"; case Off = "off"; }
来源：http://www.ydjk.org.cn/Article/details/gt3uijtjazo.html

[U49] PHP：只读属性
来源：http://www.ydjk.org.cn/Article/details/gt3kigqpzdr.html

public readonly string $name
来源：http://www.52xcode.cn/Article/details/gt3bwhfweqa.html

[U50] PHP：构造器属性提升
来源：http://www.ydjk.org.cn/Article/details/gt3vvllmqnt.html

public function __construct(private int $id) {}
来源：http://www.ydjk.org.cn/Article/details/gt3hmyoibwz.html

[U51] PHP：数组解构
来源：http://www.ydjk.org.cn/Article/details/gt3cvyqpqdq.html

[$a, $b] = $arr;
来源：http://www.52xcode.cn/Article/details/gt3cuinxtjs.html

[U52] PHP：箭头函数
来源：http://www.52xcode.cn/Article/details/gt3bnyeifxn.html

$double = fn($x) => $x * 2;
来源：http://www.ydjk.org.cn/Article/details/gt3cchaxxzy.html

[U53] PHP：空合并运算符
来源：http://www.52xcode.cn/Article/details/gt3awpjoabw.html

$v = $a ?? $b ?? "default";
来源：http://www.52xcode.cn/Article/details/gt3unksbxmc.html

[U54] PHP：空安全调用
来源：http://www.ydjk.org.cn/Article/details/gt3ihfepuzs.html

$obj?->method()
来源：http://www.52xcode.cn/Article/details/gt3ffmzitkm.html

[U55] PHP：match 表达式
来源：http://www.52xcode.cn/Article/details/gt3fbcyubeg.html

$s = match($x) { 1 => "一", default => "其他" };
来源：http://www.ydjk.org.cn/Article/details/gt3kynjhmbh.html

[U56] PHP：命名参数
来源：http://www.ydjk.org.cn/Article/details/gt3dnwuyeqr.html

f(a: 1, b: 2)
来源：http://www.ydjk.org.cn/Article/details/gt3pxnvnxdh.html

[U57] PHP：字符串插值
来源：http://www.ydjk.org.cn/Article/details/gt3qzlingvn.html

"值: {$a}"
来源：http://www.52xcode.cn/Article/details/gt3gggubylt.html

[U58] PHP：数组三件套
来源：http://www.52xcode.cn/Article/details/gt3fuiwjgke.html

array_map($f, $a);  array_filter($a, $f);  array_reduce($a, $f, 0);
来源：http://www.52xcode.cn/Article/details/gt3dndujjlg.html

[U59] PHP：自定义排序
来源：http://www.ydjk.org.cn/Article/details/gt3tlzpdtfl.html

usort($arr, fn($a, $b) => $a["age"] <=> $b["age"]);
来源：http://www.52xcode.cn/Article/details/gt3ssokqxrx.html

[U60] PHP：JSON 编解码
来源：http://www.52xcode.cn/Article/details/gt3dbocnmef.html

json_encode($d, JSON_UNESCAPED_UNICODE);  json_decode($s, true);
来源：http://www.52xcode.cn/Article/details/gt3eixqecqp.html

[U61] PHP：正则
来源：http://www.ydjk.org.cn/Article/details/gt3ejcesukk.html

preg_match('/(\d+)/', $s, $m);  preg_replace('/\d+/', '#', $s);
来源：http://www.52xcode.cn/Article/details/gt3ancbeeje.html

[U62] PHP：日期对象
来源：http://www.ydjk.org.cn/Article/details/gt3ntwkjfbt.html

(new DateTimeImmutable())->format("Y-m-d");
来源：http://www.52xcode.cn/Article/details/gt3glshzjqb.html

[U63] PHP：文件读写
来源：http://www.52xcode.cn/Article/details/gt3npmxrltn.html

file_get_contents($f);  file_put_contents($f, $data);
来源：http://www.52xcode.cn/Article/details/gt3jerrygym.html

[U64] PHP：目录遍历
来源：http://www.52xcode.cn/Article/details/gt3xylivujy.html

glob("dir/*.php");  scandir("dir");
来源：http://www.52xcode.cn/Article/details/gt3aepsgyob.html

[U65] PHP：会话
来源：http://www.ydjk.org.cn/Article/details/gt3cigqswmb.html

session_start();  $_SESSION["uid"] = 1;
来源：http://www.52xcode.cn/Article/details/gt3kphcllms.html

[U66] PHP：设置 Cookie
来源：http://www.ydjk.org.cn/Article/details/gt3bfruzdrt.html

setcookie("token", $v, ["httponly" => true, "samesite" => "Lax"]);
来源：http://www.52xcode.cn/Article/details/gt3znmoynej.html

[U67] PHP：处理文件上传
来源：http://www.52xcode.cn/Article/details/gt3kgtzirds.html

$_FILES["file"]["tmp_name"] 与 move_uploaded_file()
来源：http://www.52xcode.cn/Article/details/gt3utdlgtlg.html

[U68] PHP：PDO 连接
来源：http://www.52xcode.cn/Article/details/gt3qpffkzzi.html

$pdo = new PDO("mysql:host=localhost;dbname=app", "root", "");
来源：http://www.ydjk.org.cn/Article/details/gt3anpyxhuw.html

[U69] PHP：PDO 预处理
来源：http://www.ydjk.org.cn/Article/details/gt3izspislh.html

$stmt = $pdo->prepare("SELECT * FROM users WHERE id = ?");  $stmt->execute([$id]);
来源：http://www.52xcode.cn/Article/details/gt3ibapzicf.html

[U70] PHP：PDO 事务
来源：http://www.52xcode.cn/Article/details/gt3vauvdxxr.html

$pdo->beginTransaction();  $pdo->commit();  $pdo->rollBack();
来源：http://www.ydjk.org.cn/Article/details/gt3oxtejuqp.html

[U71] PHP：抛出异常
来源：http://www.ydjk.org.cn/Article/details/gt3mppthxaw.html

throw new RuntimeException("失败", 500);
来源：http://www.ydjk.org.cn/Article/details/gt3dnxgbwsa.html

[U72] PHP：写错误日志
来源：http://www.52xcode.cn/Article/details/gt3qmuvsyvj.html

error_log("失败: " . $e->getMessage());
来源：http://www.52xcode.cn/Article/details/gt3vujyoelw.html

[U73] PHP：读取 ini 配置
来源：http://www.52xcode.cn/Article/details/gt3lqhcrsgs.html

parse_ini_file("config.ini", true)
来源：http://www.52xcode.cn/Article/details/gt3xsvstsfz.html

[U74] PHP：读取环境变量
来源：http://www.ydjk.org.cn/Article/details/gt3eedrinhi.html

getenv("APP_ENV") ?: "production"
来源：http://www.52xcode.cn/Article/details/gt3xpahhhwv.html

[U75] PHP：依赖注入
来源：http://www.52xcode.cn/Article/details/gt3zflstkvv.html

composer require psr/container
来源：http://www.ydjk.org.cn/Article/details/gt3ecsivgyx.html

[U76] PHP：简单路由
来源：http://www.ydjk.org.cn/Article/details/gt3zjczjdap.html

$path = parse_url($_SERVER["REQUEST_URI"], PHP_URL_PATH);
来源：http://www.ydjk.org.cn/Article/details/gt3kmwtzbfe.html

[U77] PHP：模板渲染
来源：http://www.ydjk.org.cn/Article/details/gt3fuisyhqs.html

composer require twig/twig
来源：http://www.52xcode.cn/Article/details/gt3ueuqfqfv.html

[U78] PHP：单元测试
来源：http://www.ydjk.org.cn/Article/details/gt3duoqhbzz.html

composer require --dev phpunit/phpunit
来源：http://www.ydjk.org.cn/Article/details/gt3hpyymufy.html

[U79] PHP：静态分析
来源：http://www.52xcode.cn/Article/details/gt3ovfdwppr.html

composer require --dev phpstan/phpstan
来源：http://www.52xcode.cn/Article/details/gt3jybkrcpt.html

[U80] PHP：代码规范修复
来源：http://www.52xcode.cn/Article/details/gt3xwcunbcd.html

composer require --dev friendsofphp/php-cs-fixer
来源：http://www.52xcode.cn/Article/details/gt3msghakfj.html

[U81] JS：初始化项目
来源：http://www.52xcode.cn/Article/details/gt3sibjmcqz.html

npm init -y;  npm i express
来源：http://www.ydjk.org.cn/Article/details/gt3vlxjyslr.html

[U82] JS：package.json 脚本
来源：http://www.ydjk.org.cn/Article/details/gt3rhjbjaei.html

"scripts": { "dev": "vite", "build": "vite build" }
来源：http://www.ydjk.org.cn/Article/details/gt3oajcklxo.html

[U83] JS：ES Module 导入导出
来源：http://www.ydjk.org.cn/Article/details/gt3cikgqacd.html

export const a = 1;  import { a } from "./m.js";
来源：http://www.ydjk.org.cn/Article/details/gt3cfieuyar.html

[U84] JS：CommonJS 写法
来源：http://www.52xcode.cn/Article/details/gt3zsrejvbm.html

module.exports = { a };  const { a } = require("./m");
来源：http://www.52xcode.cn/Article/details/gt3vtctjjnk.html

[U85] JS：可选链
来源：http://www.ydjk.org.cn/Article/details/gt3bkifozld.html

a?.b?.c
来源：http://www.ydjk.org.cn/Article/details/gt3mcjjuuma.html

[U86] JS：空值合并
来源：http://www.ydjk.org.cn/Article/details/gt3kmzdpuiy.html

a ?? b
来源：http://www.ydjk.org.cn/Article/details/gt3joidfxqw.html

[U87] JS：解构默认值
来源：http://www.52xcode.cn/Article/details/gt3fbibwwez.html

const { a = 1, b = 2 } = obj;
来源：http://www.ydjk.org.cn/Article/details/gt3xvrmutzl.html

[U88] JS：对象展开合并
来源：http://www.52xcode.cn/Article/details/gt3bwxqmirt.html

{ ...a, ...b }
来源：http://www.ydjk.org.cn/Article/details/gt3akvzrtpp.html

[U89] JS：数组去重
来源：http://www.ydjk.org.cn/Article/details/gt3gozilved.html

[...new Set(arr)]
来源：http://www.ydjk.org.cn/Article/details/gt3hweqpdjv.html

[U90] JS：数字数组排序
来源：http://www.ydjk.org.cn/Article/details/gt3gypghnee.html

[...arr].sort((a, b) => a - b)
来源：http://www.52xcode.cn/Article/details/gt3drgiydbu.html

[U91] JS：对象键值遍历
来源：http://www.52xcode.cn/Article/details/gt3lllkbqlj.html

Object.entries(obj).forEach(([k, v]) => {});
来源：http://www.52xcode.cn/Article/details/gt3gutbhfle.html

[U92] JS：深拷贝
来源：http://www.52xcode.cn/Article/details/gt3skgvdaaj.html

structuredClone(obj)
来源：http://www.52xcode.cn/Article/details/gt3dveoycsc.html

[U93] JS：模板字符串
来源：http://www.52xcode.cn/Article/details/gt3pyreqxqy.html

`共 ${n} 条`
来源：http://www.ydjk.org.cn/Article/details/gt3ufytghft.html

[U94] JS：箭头函数
来源：http://www.ydjk.org.cn/Article/details/gt3anfchhgh.html

const double = x => x * 2;
来源：http://www.52xcode.cn/Article/details/gt3mqkowuwr.html

[U95] JS：Promise 包装
来源：http://www.ydjk.org.cn/Article/details/gt3wxaszzqd.html

new Promise((resolve, reject) => {})
来源：http://www.52xcode.cn/Article/details/gt3rlzlpikg.html

[U96] JS：async/await 与异常
来源：http://www.52xcode.cn/Article/details/gt3neyvoczq.html

try { const d = await f(); } catch (e) { console.error(e); }
来源：http://www.52xcode.cn/Article/details/gt3svmgqfyn.html

[U97] JS：并发请求
来源：http://www.ydjk.org.cn/Article/details/gt3swfnedcu.html

await Promise.all(urls.map(u => fetch(u)))
来源：http://www.ydjk.org.cn/Article/details/gt3amnjapwg.html

[U98] JS：fetch 带 JSON
来源：http://www.ydjk.org.cn/Article/details/gt3knvurspk.html

await fetch(url, { method: "POST", headers: { "Content-Type": "application/json" }, body: JSON.stringify(d) })
来源：http://www.ydjk.org.cn/Article/details/gt3epixctga.html

[U99] JS：事件监听
来源：http://www.ydjk.org.cn/Article/details/gt3grvczcyc.html

el.addEventListener("click", e => {})
来源：http://www.52xcode.cn/Article/details/gt3lbbiksxw.html

[U100] JS：DOM 查询
来源：http://www.ydjk.org.cn/Article/details/gt3ilglvdzm.html

document.querySelector(".item")
来源：http://www.52xcode.cn/Article/details/gt3dalewify.html

[U101] JS：classList 操作
来源：http://www.52xcode.cn/Article/details/gt3qexgdzxo.html

el.classList.toggle("active")
来源：http://www.52xcode.cn/Article/details/gt3gtxwaecx.html

[U102] JS：本地存储
来源：http://www.ydjk.org.cn/Article/details/gt3zffbycla.html

localStorage.setItem("k", JSON.stringify(v))
来源：http://www.ydjk.org.cn/Article/details/gt3lbapmrjj.html

[U103] JS：定时器
来源：http://www.52xcode.cn/Article/details/gt3xcvqlajb.html

setTimeout(fn, 1000);  setInterval(fn, 1000);
来源：http://www.ydjk.org.cn/Article/details/gt3dqstlpcf.html

[U104] JS：防抖
来源：http://www.52xcode.cn/Article/details/gt3wcqapksh.html

const debounce = (fn, ms) => { let t; return (...a) => { clearTimeout(t); t = setTimeout(() => fn(...a), ms); }; };
来源：http://www.ydjk.org.cn/Article/details/gt3zgnljkan.html

[U105] JS：节流
来源：http://www.ydjk.org.cn/Article/details/gt3ymyauzhd.html

const throttle = (fn, ms) => { let last = 0; return (...a) => { const n = Date.now(); if (n - last >= ms) { last = n; fn(...a); } }; };
来源：http://www.ydjk.org.cn/Article/details/gt3zufdweve.html

[U106] JS：日期格式化
来源：http://www.52xcode.cn/Article/details/gt3ymlgdwhl.html

new Intl.DateTimeFormat("zh-CN", { dateStyle: "medium" }).format(new Date())
来源：http://www.ydjk.org.cn/Article/details/gt3malepoav.html

[U107] JS：数字千分位
来源：http://www.52xcode.cn/Article/details/gt3uyaarmef.html

new Intl.NumberFormat("en-US").format(1234567)
来源：http://www.ydjk.org.cn/Article/details/gt3nkajxpvs.html

[U108] JS：随机整数
来源：http://www.52xcode.cn/Article/details/gt3pggyujif.html

Math.floor(Math.random() * (max - min + 1)) + min
来源：http://www.52xcode.cn/Article/details/gt3nlbvmwko.html

[U109] JS：数组分组
来源：http://www.52xcode.cn/Article/details/gt3elukhivo.html

Object.groupBy(arr, x => x.type)
来源：http://www.52xcode.cn/Article/details/gt3cynafqpp.html

[U110] JS：数组分块
来源：http://www.ydjk.org.cn/Article/details/gt3xlmeodzc.html

arr.reduce((acc, x, i) => (i % size ? acc : [...acc, arr.slice(i, i + size)]), [])
来源：http://www.ydjk.org.cn/Article/details/gt3ktjgetog.html

[U111] JS：对象转 Map
来源：http://www.ydjk.org.cn/Article/details/gt3kfudhssb.html

new Map(Object.entries(obj))
来源：http://www.52xcode.cn/Article/details/gt3xfhcxfkf.html

[U112] JS：字符串补位
来源：http://www.52xcode.cn/Article/details/gt3drkwipkd.html

"7".padStart(3, "0")
来源：http://www.ydjk.org.cn/Article/details/gt3kjwpemjn.html

[U113] JS：正则替换全部
来源：http://www.ydjk.org.cn/Article/details/gt3kovaxdkt.html

s.replaceAll("a", "b")
来源：http://www.52xcode.cn/Article/details/gt3iglxjzyx.html

[U114] JS：JSON 深比较
来源：http://www.ydjk.org.cn/Article/details/gt3vigswypu.html

JSON.stringify(a) === JSON.stringify(b)
来源：http://www.ydjk.org.cn/Article/details/gt3feevhmie.html

[U115] JS：生成 UUID
来源：http://www.ydjk.org.cn/Article/details/gt3fxxabvau.html

crypto.randomUUID()
来源：http://www.ydjk.org.cn/Article/details/gt3odyggonr.html

[U116] JS：类型检查（JSDoc）
来源：http://www.ydjk.org.cn/Article/details/gt3mxlnqbpr.html

/** @param {string} name */ function f(name) {}
来源：http://www.ydjk.org.cn/Article/details/gt3gejygqpm.html

[U117] JS：单元测试
来源：http://www.ydjk.org.cn/Article/details/gt3qbtvhrmo.html

npm i -D vitest;  npx vitest
来源：http://www.52xcode.cn/Article/details/gt3itutotfa.html

[U118] JS：开发服务器
来源：http://www.ydjk.org.cn/Article/details/gt3nwooxyti.html

npm i -D vite;  npx vite
来源：http://www.52xcode.cn/Article/details/gt3vlkrnvbt.html

[U119] JS：生产构建
来源：http://www.ydjk.org.cn/Article/details/gt3wobwdfrr.html

npx vite build
来源：http://www.52xcode.cn/Article/details/gt3rrlfdemt.html

[U120] JS：读取环境变量（Vite）
来源：http://www.ydjk.org.cn/Article/details/gt3dxopwzrw.html

import.meta.env.VITE_API_URL
来源：http://www.52xcode.cn/Article/details/gt3dzfakrje.html

================================================================================
来源：http://www.52xcode.cn/Article/details/gt3yngzbknt.html

统计汇总
来源：http://www.52xcode.cn/Article/details/gt3sfqtjxzw.html

================================================================================
来源：http://www.52xcode.cn/Article/details/gt3vaxhnfet.html

按语言统计（条）：
来源：http://www.52xcode.cn/Article/details/gt3lvptdbjv.html

Python ......... 252
来源：http://www.ydjk.org.cn/Article/details/gt3tnxiqkfv.html

PHP ............ 252
来源：http://www.52xcode.cn/Article/details/gt3hvgbjlnr.html

JavaScript ..... 252
来源：http://www.52xcode.cn/Article/details/gt3ebjawest.html

TypeScript ..... 212
来源：http://www.ydjk.org.cn/Article/details/gt3sukzodur.html

Java ........... 212
来源：http://www.ydjk.org.cn/Article/details/gt3jhjgdpnz.html

Go ............. 212
来源：http://www.52xcode.cn/Article/details/gt3ytrubjcr.html

Ruby ........... 212
来源：http://www.52xcode.cn/Article/details/gt3oqhltoci.html

C# ............. 212
来源：http://www.ydjk.org.cn/Article/details/gt3yvsdhziv.html

C .............. 30
来源：http://www.52xcode.cn/Article/details/gt3ctpahkcg.html

C++ ............ 30
来源：http://www.ydjk.org.cn/Article/details/gt3dlzcsnlm.html

SQL ............ 90
来源：http://www.52xcode.cn/Article/details/gt3vpzeakvw.html

Bash ........... 80
来源：http://www.ydjk.org.cn/Article/details/gt3lurnnfrs.html

Kotlin ......... 15
来源：http://www.52xcode.cn/Article/details/gt3qofoxczg.html

Swift .......... 15
来源：http://www.52xcode.cn/Article/details/gt3jwadjyht.html

Lua ............ 10
来源：http://www.52xcode.cn/Article/details/gt3hrminhrm.html

Perl ........... 10
来源：http://www.52xcode.cn/Article/details/gt3rismfoiz.html

Scala .......... 10
来源：http://www.ydjk.org.cn/Article/details/gt3ierxyuuf.html

------------------------------------
来源：http://www.ydjk.org.cn/Article/details/gt3yxjhybkb.html

合计 ........... 2106 条
来源：http://www.ydjk.org.cn/Article/details/gt3jfmmvtgw.html

按章节统计：
来源：http://www.52xcode.cn/Article/details/gt3asgstslv.html

A 基础语法与类型       26 个任务 × 8 语言 =  208
来源：http://www.ydjk.org.cn/Article/details/gt3epzbbfnz.html

B 流程控制             16 个任务 × 8 语言 =  128
来源：http://www.ydjk.org.cn/Article/details/gt3mnbpjpvl.html

C 函数与作用域         16 个任务 × 8 语言 =  128
来源：http://www.52xcode.cn/Article/details/gt3hesmwrbt.html

D 数组 / 列表 / 集合   26 个任务 × 8 语言 =  208
来源：http://www.ydjk.org.cn/Article/details/gt3vgjsoynf.html

E 字符串处理           22 个任务 × 8 语言 =  176
来源：http://www.ydjk.org.cn/Article/details/gt3llzxytrh.html

F 文件与目录           12 个任务 × 8 语言 =   96
来源：http://www.52xcode.cn/Article/details/gt3mphgbfka.html

G 面向对象             16 个任务 × 8 语言 =  128
来源：http://www.52xcode.cn/Article/details/gt3hpyzeefl.html

H 异常与错误处理       10 个任务 × 8 语言 =   80
来源：http://www.ydjk.org.cn/Article/details/gt3pumhcxlv.html

I 正则表达式            8 个任务 × 8 语言 =   64
来源：http://www.ydjk.org.cn/Article/details/gt3gabunuuv.html

J 日期与时间           10 个任务 × 8 语言 =   80
来源：http://www.52xcode.cn/Article/details/gt3ayblixli.html

K JSON 与序列化         8 个任务 × 8 语言 =   64
来源：http://www.52xcode.cn/Article/details/gt3pbreharw.html

L 网络请求              8 个任务 × 8 语言 =   64
来源：http://www.52xcode.cn/Article/details/gt3zyeyuclg.html

M 命令行 / 进程         8 个任务 × 8 语言 =   64
来源：http://www.ydjk.org.cn/Article/details/gt3tsaiwesg.html

N 数据结构与算法       12 个任务 × 8 语言 =   96
来源：http://www.ydjk.org.cn/Article/details/gt3eoevyznf.html

O 并发与异步            6 个任务 × 8 语言 =   48
来源：http://www.ydjk.org.cn/Article/details/gt3svlayhud.html

P 常用工具函数          8 个任务 × 8 语言 =   64
来源：http://www.52xcode.cn/Article/details/gt3zjdlxkda.html

Q SQL 专题                              90
来源：http://www.ydjk.org.cn/Article/details/gt3jnfecghc.html

R Bash 专题                             80
来源：http://www.52xcode.cn/Article/details/gt3cnhlljou.html

S C / C++ 专题                          60
来源：http://www.52xcode.cn/Article/details/gt3kjteczjm.html

T 其他语言补充                          60
来源：http://www.52xcode.cn/Article/details/gt3ahmatqft.html

U 高频实用片段                         120
来源：http://www.ydjk.org.cn/Article/details/gt3hxhonhru.html

------------------------------------
来源：http://www.52xcode.cn/Article/details/gt3mdqvwjem.html

合计                                  2106 条
来源：http://www.ydjk.org.cn/Article/details/gt3ebldntjz.html

--------------------------------------------------------------------------------
来源：http://www.ydjk.org.cn/Article/details/gt3wxdoctwu.html

使用提醒
来源：http://www.52xcode.cn/Article/details/gt3mphejgqu.html

--------------------------------------------------------------------------------
来源：http://www.ydjk.org.cn/Article/details/gt3uftmipnu.html

1. 示例追求"最小可用"，正式项目中请补齐导入、错误处理与边界判断。
来源：http://www.52xcode.cn/Article/details/gt3kjzwzstc.html

2. 涉及文件、网络、数据库的示例，注意资源释放与异常捕获。
来源：http://www.52xcode.cn/Article/details/gt3hrabsywo.html

3. 语言版本差异较大（如 Python 3.10 的 match、Java 17 的 record/switch 箭头），
来源：http://www.52xcode.cn/Article/details/gt3vgxmqxkf.html

在旧版本上使用前请先确认语法支持情况。
来源：http://www.ydjk.org.cn/Article/details/gt3etrakkpo.html

4. 标注"手写"的条目是因为该语言缺少对应内置能力，实际项目中可引入成熟库。
来源：http://www.ydjk.org.cn/Article/details/gt3melxkymv.html

—— 文件结束 ——
来源：http://www.ydjk.org.cn/Article/details/gt3wkzwhqsz.html

================================================================================
来源：http://www.ydjk.org.cn/Article/details/gt3bphkkvgx.html

程序语言常见例子速查手册（2024 版）
来源：http://www.ydjk.org.cn/Article/details/gt3gyrurvsq.html

Common Programming Examples Cheat Book
来源：http://www.52xcode.cn/Article/details/gt3rpeefczc.html

================================================================================
来源：http://www.52xcode.cn/Article/details/gt3ysbxkvtf.html

【收录内容】
来源：http://www.52xcode.cn/Article/details/gt3yzlbqcbf.html

覆盖 12 种语言 / 语法与常见 API：
来源：http://www.52xcode.cn/Article/details/gt3gxojpyei.html

Python · PHP · JavaScript · TypeScript · Java · Go · Ruby · C#
来源：http://www.ydjk.org.cn/Article/details/gt3hwzwenzd.html

SQL · Bash · C · C++
来源：http://www.52xcode.cn/Article/details/gt3osarlrng.html

按「任务」分组：每个任务下按语言各给出一条最小可用示例。
来源：http://www.52xcode.cn/Article/details/gt3adnokqtx.html

【使用说明】
来源：http://www.ydjk.org.cn/Article/details/gt3phziryic.html

1. 每个任务形如 "[编号] 任务名"，下面每行以语言标记开头：
来源：http://www.52xcode.cn/Article/details/gt3qbuwwhdw.html

Py:    Python        PHP:   PHP           JS:    JavaScript
来源：http://www.52xcode.cn/Article/details/gt3wfudsfwf.html

TS:    TypeScript    Java:  Java          Go:    Go
来源：http://www.ydjk.org.cn/Article/details/gt3xszvcmrv.html

Ruby:  Ruby          C#:    C#            SQL:   SQL
来源：http://www.ydjk.org.cn/Article/details/gt3kcnvbqcl.html

Bash:  Shell         C:     C             C++:   C++
来源：http://www.ydjk.org.cn/Article/details/gt3aeuzvhls.html

2. 示例只展示核心写法，刻意省略 import / require / include / using 等样板代码。
来源：http://www.52xcode.cn/Article/details/gt3evmfqhlw.html

需要完整可运行文件时，请自行补齐当前语言的导入语句。
来源：http://www.ydjk.org.cn/Article/details/gt3ueyhdupi.html

3. 语法基准：Python 3.10+ / PHP 8.1+ / ES2020+ / TypeScript 5 / Java 17 /
来源：http://www.52xcode.cn/Article/details/gt3vogrnyae.html

Go 1.21+ / Ruby 3.x / C# 10+ / C17 / C++17。
来源：http://www.52xcode.cn/Article/details/gt3exxwwpoe.html

4. 检索建议：用编辑器或浏览器 Ctrl+F 搜关键词，如 "排序" "读取文件" "正则"。
来源：http://www.ydjk.org.cn/Article/details/gt3wuzrxbpw.html

5. 标记为 "// 无" 表示该语言没有对应的一等语法，需用替代写法（示例给出替代方案）。
来源：http://www.ydjk.org.cn/Article/details/gt3pmdltehb.html

6. 符号 "⏎" 表示代码在此处换行（主要用于 Python 等强制缩进、无法压成一行的结构）。
来源：http://www.52xcode.cn/Article/details/gt3dfufccmw.html

【文件统计】
来源：http://www.ydjk.org.cn/Article/details/gt3uieeunfw.html

语言示例共 2106 条，分布见本文末尾的「统计汇总」。
来源：http://www.ydjk.org.cn/Article/details/gt3wtxllslw.html

--------------------------------------------------------------------------------
来源：http://www.ydjk.org.cn/Article/details/gt3qbntymor.html

目  录
来源：http://www.ydjk.org.cn/Article/details/gt3uppfrzmp.html

--------------------------------------------------------------------------------
来源：http://www.52xcode.cn/Article/details/gt3klcolxnh.html

A. 基础语法与类型              （第 1 节，26 个任务，208 条）
来源：http://www.52xcode.cn/Article/details/gt3ylqallyd.html

B. 流程控制                    （第 2 节，16 个任务，128 条）
来源：http://www.52xcode.cn/Article/details/gt3ujmayaac.html

C. 函数与作用域                （第 3 节，16 个任务，128 条）
来源：http://www.ydjk.org.cn/Article/details/gt3isrmebfy.html

D. 数组 / 列表 / 集合          （第 4 节，26 个任务，208 条）
来源：http://www.52xcode.cn/Article/details/gt3dlbkppkv.html

E. 字符串处理                  （第 5 节，22 个任务，176 条）
来源：http://www.52xcode.cn/Article/details/gt3qoogriye.html

F. 文件与目录                  （第 6 节，12 个任务，96 条）
来源：http://www.52xcode.cn/Article/details/gt3tinhpnih.html

G. 面向对象                    （第 7 节，16 个任务，128 条）
来源：http://www.ydjk.org.cn/Article/details/gt3pwxvxkva.html

H. 异常与错误处理              （第 8 节，10 个任务，80 条）
来源：http://www.ydjk.org.cn/Article/details/gt3mtuyhffc.html

I. 正则表达式                  （第 9 节，8 个任务，64 条）
来源：http://www.ydjk.org.cn/Article/details/gt3dvaxkhdt.html

J. 日期与时间                  （第 10 节，10 个任务，80 条）
来源：http://www.ydjk.org.cn/Article/details/gt3gokyzuri.html

K. JSON 与序列化               （第 11 节，8 个任务，64 条）
来源：http://www.ydjk.org.cn/Article/details/gt3gqfzeate.html

L. 网络请求                    （第 12 节，8 个任务，64 条）
来源：http://www.ydjk.org.cn/Article/details/gt3jwmuhraf.html

M. 命令行 / 进程 / 环境        （第 13 节，8 个任务，64 条）
来源：http://www.52xcode.cn/Article/details/gt3xhdwosmj.html

N. 数据结构与算法              （第 14 节，12 个任务，96 条）
来源：http://www.ydjk.org.cn/Article/details/gt3wxpjyuab.html

O. 并发与异步                  （第 15 节，6 个任务，48 条）
来源：http://www.52xcode.cn/Article/details/gt3ivorcyvx.html

P. 常用工具函数                （第 16 节，8 个任务，64 条）
来源：http://www.52xcode.cn/Article/details/gt3ykqszosh.html

Q. SQL 专题                    （第 17 节，90 条）
来源：http://www.ydjk.org.cn/Article/details/gt3qhlrgart.html

R. Bash 专题                   （第 18 节，80 条）
来源：http://www.ydjk.org.cn/Article/details/gt3tsqnorcq.html

S. C / C++ 专题                （第 19 节，60 条）
来源：http://www.52xcode.cn/Article/details/gt3gffaujoh.html

T. 其他语言补充                （第 20 节，60 条：Kotlin / Swift / Lua / Perl / Scala）
来源：http://www.ydjk.org.cn/Article/details/gt3djiyfydn.html

U. 高频实用片段                （第 21 节，120 条：Python / PHP / JavaScript 各 40 条）
来源：http://www.ydjk.org.cn/Article/details/gt3srprftsj.html

================================================================================
来源：http://www.52xcode.cn/Article/details/gt3fknmmeei.html

A. 基础语法与类型
来源：http://www.ydjk.org.cn/Article/details/gt3syyeqvyf.html

================================================================================
来源：http://www.ydjk.org.cn/Article/details/gt3xciehzma.html

[A01] Hello World
来源：http://www.52xcode.cn/Article/details/gt3tktxochz.html

Py:   print("Hello, World!")
来源：http://www.ydjk.org.cn/Article/details/gt3feijenze.html

PHP:  echo "Hello, World!";
来源：http://www.ydjk.org.cn/Article/details/gt3foumtqpe.html

JS:   console.log("Hello, World!");
来源：http://www.52xcode.cn/Article/details/gt3tmhmoqqo.html

TS:   const msg: string = "Hello, World!"; console.log(msg);
来源：http://www.ydjk.org.cn/Article/details/gt3qsoseroq.html

Java: System.out.println("Hello, World!");
来源：http://www.52xcode.cn/Article/details/gt3tdoqogln.html

Go:   fmt.Println("Hello, World!")
来源：http://www.ydjk.org.cn/Article/details/gt3ixgxkyrv.html

Ruby: puts "Hello, World!"
来源：http://www.52xcode.cn/Article/details/gt3dispdkro.html

C#:   Console.WriteLine("Hello, World!");
来源：http://www.52xcode.cn/Article/details/gt3bhzbzlbq.html

[A02] 变量声明与赋值
来源：http://www.52xcode.cn/Article/details/gt3jbqlofhe.html

Py:   name = "Alex"; age = 20            # 动态类型，无需声明
来源：http://www.52xcode.cn/Article/details/gt3fvxexzgs.html

PHP:  $name = "Alex"; $age = 20;
来源：http://www.ydjk.org.cn/Article/details/gt3eqqzmixr.html

JS:   let name = "Alex"; const age = 20;
来源：http://www.52xcode.cn/Article/details/gt3lprbgpmu.html

TS:   let name: string = "Alex"; const age: number = 20;
来源：http://www.52xcode.cn/Article/details/gt3hvqtfnlj.html

Java: String name = "Alex"; int age = 20;
来源：http://www.ydjk.org.cn/Article/details/gt3tziicpsf.html

Go:   name := "Alex"; age := 20
来源：http://www.ydjk.org.cn/Article/details/gt3lfhitojo.html

Ruby: name = "Alex"; age = 20
来源：http://www.52xcode.cn/Article/details/gt3ygahovqb.html


<!-- 参考信息 -->