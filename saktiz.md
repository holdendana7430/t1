代发 wailian999

[U33] Py：打包发布
来源：http://www.52xcode.cn/Article/details/gt3tvgvgwrt.html

python -m build  （依赖 pyproject.toml）
来源：http://www.ydjk.org.cn/Article/details/gt3xbyffvqo.html

[U34] Py：判断编码
来源：http://www.52xcode.cn/Article/details/gt3bkwxzdsr.html

chardet.detect(raw)
来源：http://www.52xcode.cn/Article/details/gt3xigbjilk.html

[U35] Py：发送邮件
来源：http://www.52xcode.cn/Article/details/gt3ztorhgmi.html

smtplib.SMTP_SSL(...).send_message(msg)
来源：http://www.ydjk.org.cn/Article/details/gt3tjslsgil.html

[U36] Py：定时任务
来源：http://www.52xcode.cn/Article/details/gt3xjmtgcnh.html

schedule.every(10).minutes.do(job)
来源：http://www.ydjk.org.cn/Article/details/gt3qppttpqm.html

[U37] Py：读写 Excel
来源：http://www.52xcode.cn/Article/details/gt3xczgecus.html

pandas.read_excel / DataFrame.to_excel
来源：http://www.52xcode.cn/Article/details/gt3odeijcfm.html

[U38] Py：获取脚本所在目录
来源：http://www.52xcode.cn/Article/details/gt3cfvflrex.html

Path(__file__).resolve().parent
来源：http://www.ydjk.org.cn/Article/details/gt3dxgjvhtb.html

[U39] Py：判断是否在交互环境
来源：http://www.ydjk.org.cn/Article/details/gt3uniwlqgx.html

sys.stdout.isatty()
来源：http://www.52xcode.cn/Article/details/gt3pprfwlnf.html

[U40] Py：打印到标准错误
来源：http://www.52xcode.cn/Article/details/gt3fsiwgmjr.html

print("err", file=sys.stderr)
来源：http://www.ydjk.org.cn/Article/details/gt3sjxlghuc.html

[U41] PHP：初始化 Composer 项目
来源：http://www.ydjk.org.cn/Article/details/gt3qqxalxgk.html

composer init;  composer require guzzlehttp/guzzle
来源：http://www.52xcode.cn/Article/details/gt3taxeuxkx.html

[U42] PHP：PSR-4 自动加载
来源：http://www.52xcode.cn/Article/details/gt3qfsvzhsq.html

"autoload": { "psr-4": { "App\\": "src/" } }
来源：http://www.ydjk.org.cn/Article/details/gt3ngtlkrre.html

[U43] PHP：声明命名空间
来源：http://www.52xcode.cn/Article/details/gt3amnzcubs.html

namespace App\Http;
来源：http://www.52xcode.cn/Article/details/gt3wutvaxni.html

[U44] PHP：开启严格类型
来源：http://www.ydjk.org.cn/Article/details/gt3kyhznqqs.html

declare(strict_types=1);
来源：http://www.ydjk.org.cn/Article/details/gt3cuwvatct.html

[U45] PHP：类型声明与返回类型
来源：http://www.52xcode.cn/Article/details/gt3phbqisag.html

function add(int $a, int $b): int { return $a + $b; }
来源：http://www.52xcode.cn/Article/details/gt3zeynunts.html

[U46] PHP：可空类型
来源：http://www.52xcode.cn/Article/details/gt3blskjarm.html

?string $name = null
来源：http://www.ydjk.org.cn/Article/details/gt3noepefse.html

[U47] PHP：联合类型
来源：http://www.52xcode.cn/Article/details/gt3eodnskhg.html

int|string $id
来源：http://www.ydjk.org.cn/Article/details/gt3ragpggiy.html

[U48] PHP：纯枚举
来源：http://www.52xcode.cn/Article/details/gt3bqquvpza.html

enum Status: string { case Active = "active"; case Off = "off"; }
来源：http://www.52xcode.cn/Article/details/gt3yqknewdf.html

[U49] PHP：只读属性
来源：http://www.ydjk.org.cn/Article/details/gt3ntxtjrpb.html

public readonly string $name
来源：http://www.52xcode.cn/Article/details/gt3pjilskaw.html

[U50] PHP：构造器属性提升
来源：http://www.52xcode.cn/Article/details/gt3gpvaxlki.html

public function __construct(private int $id) {}
来源：http://www.52xcode.cn/Article/details/gt3awkqkadh.html

[U51] PHP：数组解构
来源：http://www.ydjk.org.cn/Article/details/gt3idpcmzof.html

[$a, $b] = $arr;
来源：http://www.ydjk.org.cn/Article/details/gt3zpkjoguo.html

[U52] PHP：箭头函数
来源：http://www.52xcode.cn/Article/details/gt3bypzqhqu.html

$double = fn($x) => $x * 2;
来源：http://www.ydjk.org.cn/Article/details/gt3ujryhecr.html

[U53] PHP：空合并运算符
来源：http://www.52xcode.cn/Article/details/gt3eabidtgc.html

$v = $a ?? $b ?? "default";
来源：http://www.52xcode.cn/Article/details/gt3nyubnhia.html

[U54] PHP：空安全调用
来源：http://www.ydjk.org.cn/Article/details/gt3wnlvnvkm.html

$obj?->method()
来源：http://www.ydjk.org.cn/Article/details/gt3gdjzvdtk.html

[U55] PHP：match 表达式
来源：http://www.ydjk.org.cn/Article/details/gt3zmtqsepk.html

$s = match($x) { 1 => "一", default => "其他" };
来源：http://www.52xcode.cn/Article/details/gt3xwlslmnd.html

[U56] PHP：命名参数
来源：http://www.52xcode.cn/Article/details/gt3morokxhf.html

f(a: 1, b: 2)
来源：http://www.52xcode.cn/Article/details/gt3gbtyoexx.html

[U57] PHP：字符串插值
来源：http://www.52xcode.cn/Article/details/gt3sbrogcqr.html

"值: {$a}"
来源：http://www.ydjk.org.cn/Article/details/gt3kvaesxwe.html

[U58] PHP：数组三件套
来源：http://www.52xcode.cn/Article/details/gt3ycuwnhdj.html

array_map($f, $a);  array_filter($a, $f);  array_reduce($a, $f, 0);
来源：http://www.52xcode.cn/Article/details/gt3apdqfsxr.html

[U59] PHP：自定义排序
来源：http://www.ydjk.org.cn/Article/details/gt3esotquix.html

usort($arr, fn($a, $b) => $a["age"] <=> $b["age"]);
来源：http://www.52xcode.cn/Article/details/gt3pstatcbp.html

[U60] PHP：JSON 编解码
来源：http://www.52xcode.cn/Article/details/gt3mmbfgkwb.html

json_encode($d, JSON_UNESCAPED_UNICODE);  json_decode($s, true);
来源：http://www.ydjk.org.cn/Article/details/gt3vdhrnsjz.html

[U61] PHP：正则
来源：http://www.ydjk.org.cn/Article/details/gt3qqtixqna.html

preg_match('/(\d+)/', $s, $m);  preg_replace('/\d+/', '#', $s);
来源：http://www.ydjk.org.cn/Article/details/gt3cmexfrvg.html

[U62] PHP：日期对象
来源：http://www.ydjk.org.cn/Article/details/gt3qtfcovfo.html

(new DateTimeImmutable())->format("Y-m-d");
来源：http://www.ydjk.org.cn/Article/details/gt3rbargdvm.html

[U63] PHP：文件读写
来源：http://www.52xcode.cn/Article/details/gt3jmlccbdu.html

file_get_contents($f);  file_put_contents($f, $data);
来源：http://www.52xcode.cn/Article/details/gt3chyfnqxv.html

[U64] PHP：目录遍历
来源：http://www.52xcode.cn/Article/details/gt3yhuekorn.html

glob("dir/*.php");  scandir("dir");
来源：http://www.ydjk.org.cn/Article/details/gt3bceumtbb.html

[U65] PHP：会话
来源：http://www.ydjk.org.cn/Article/details/gt3sfzbxvyd.html

session_start();  $_SESSION["uid"] = 1;
来源：http://www.ydjk.org.cn/Article/details/gt3dfvzkcnk.html

[U66] PHP：设置 Cookie
来源：http://www.52xcode.cn/Article/details/gt3hskjpzin.html

setcookie("token", $v, ["httponly" => true, "samesite" => "Lax"]);
来源：http://www.ydjk.org.cn/Article/details/gt3zacdesjr.html

[U67] PHP：处理文件上传
来源：http://www.52xcode.cn/Article/details/gt3ejzwhieh.html

$_FILES["file"]["tmp_name"] 与 move_uploaded_file()
来源：http://www.ydjk.org.cn/Article/details/gt3oxcfbwtp.html

[U68] PHP：PDO 连接
来源：http://www.52xcode.cn/Article/details/gt3whiytjol.html

$pdo = new PDO("mysql:host=localhost;dbname=app", "root", "");
来源：http://www.ydjk.org.cn/Article/details/gt3tlflspuo.html

[U69] PHP：PDO 预处理
来源：http://www.ydjk.org.cn/Article/details/gt3lcfvkdmh.html

$stmt = $pdo->prepare("SELECT * FROM users WHERE id = ?");  $stmt->execute([$id]);
来源：http://www.52xcode.cn/Article/details/gt3patsxufo.html

[U70] PHP：PDO 事务
来源：http://www.ydjk.org.cn/Article/details/gt3omdirfwq.html

$pdo->beginTransaction();  $pdo->commit();  $pdo->rollBack();
来源：http://www.52xcode.cn/Article/details/gt3uyqbjvxu.html

[U71] PHP：抛出异常
来源：http://www.ydjk.org.cn/Article/details/gt3qyicckjw.html

throw new RuntimeException("失败", 500);
来源：http://www.52xcode.cn/Article/details/gt3pbxakcpj.html

[U72] PHP：写错误日志
来源：http://www.ydjk.org.cn/Article/details/gt3pqrrouby.html

error_log("失败: " . $e->getMessage());
来源：http://www.52xcode.cn/Article/details/gt3xzquglkc.html

[U73] PHP：读取 ini 配置
来源：http://www.52xcode.cn/Article/details/gt3goicujwd.html

parse_ini_file("config.ini", true)
来源：http://www.ydjk.org.cn/Article/details/gt3xdzvkjbs.html

[U74] PHP：读取环境变量
来源：http://www.ydjk.org.cn/Article/details/gt3eydiohwe.html

getenv("APP_ENV") ?: "production"
来源：http://www.52xcode.cn/Article/details/gt3ncpldvts.html

[U75] PHP：依赖注入
来源：http://www.ydjk.org.cn/Article/details/gt3ovvlmltw.html

composer require psr/container
来源：http://www.52xcode.cn/Article/details/gt3jlwizyrg.html

[U76] PHP：简单路由
来源：http://www.52xcode.cn/Article/details/gt3tssjjyga.html

$path = parse_url($_SERVER["REQUEST_URI"], PHP_URL_PATH);
来源：http://www.52xcode.cn/Article/details/gt3dlwmofwy.html

[U77] PHP：模板渲染
来源：http://www.52xcode.cn/Article/details/gt3zfrxkfsw.html

composer require twig/twig
来源：http://www.ydjk.org.cn/Article/details/gt3kmqskovf.html

[U78] PHP：单元测试
来源：http://www.ydjk.org.cn/Article/details/gt3teilyzsq.html

composer require --dev phpunit/phpunit
来源：http://www.ydjk.org.cn/Article/details/gt3enrpppwz.html

[U79] PHP：静态分析
来源：http://www.ydjk.org.cn/Article/details/gt3ruewqrlf.html

composer require --dev phpstan/phpstan
来源：http://www.52xcode.cn/Article/details/gt3cfevsgdf.html

[U80] PHP：代码规范修复
来源：http://www.52xcode.cn/Article/details/gt3lbfgrjgm.html

composer require --dev friendsofphp/php-cs-fixer
来源：http://www.ydjk.org.cn/Article/details/gt3vouhzgqo.html

[U81] JS：初始化项目
来源：http://www.52xcode.cn/Article/details/gt3nmztlbzn.html

npm init -y;  npm i express
来源：http://www.ydjk.org.cn/Article/details/gt3ybviyfyx.html

[U82] JS：package.json 脚本
来源：http://www.ydjk.org.cn/Article/details/gt3dqfbuclg.html

"scripts": { "dev": "vite", "build": "vite build" }
来源：http://www.ydjk.org.cn/Article/details/gt3pxhvzsfs.html

[U83] JS：ES Module 导入导出
来源：http://www.52xcode.cn/Article/details/gt3eavsihig.html

export const a = 1;  import { a } from "./m.js";
来源：http://www.ydjk.org.cn/Article/details/gt3eclqkgef.html

[U84] JS：CommonJS 写法
来源：http://www.ydjk.org.cn/Article/details/gt3xjycjmrz.html

module.exports = { a };  const { a } = require("./m");
来源：http://www.52xcode.cn/Article/details/gt3egryeokc.html

[U85] JS：可选链
来源：http://www.ydjk.org.cn/Article/details/gt3zlnhutnw.html

a?.b?.c
来源：http://www.ydjk.org.cn/Article/details/gt3hvgpthrz.html

[U86] JS：空值合并
来源：http://www.ydjk.org.cn/Article/details/gt3rbbuvvif.html

a ?? b
来源：http://www.ydjk.org.cn/Article/details/gt3fykdjvwq.html

[U87] JS：解构默认值
来源：http://www.ydjk.org.cn/Article/details/gt3oqjylfcy.html

const { a = 1, b = 2 } = obj;
来源：http://www.ydjk.org.cn/Article/details/gt3znljipah.html

[U88] JS：对象展开合并
来源：http://www.52xcode.cn/Article/details/gt3coltvune.html

{ ...a, ...b }
来源：http://www.ydjk.org.cn/Article/details/gt3hhmhriur.html

[U89] JS：数组去重
来源：http://www.ydjk.org.cn/Article/details/gt3repsghxv.html

[...new Set(arr)]
来源：http://www.52xcode.cn/Article/details/gt3fjmyopum.html

[U90] JS：数字数组排序
来源：http://www.ydjk.org.cn/Article/details/gt3xblfjxic.html

[...arr].sort((a, b) => a - b)
来源：http://www.ydjk.org.cn/Article/details/gt3ewogoaow.html

[U91] JS：对象键值遍历
来源：http://www.52xcode.cn/Article/details/gt3ctpbhyxs.html

Object.entries(obj).forEach(([k, v]) => {});
来源：http://www.52xcode.cn/Article/details/gt3wxcpqrsj.html

[U92] JS：深拷贝
来源：http://www.52xcode.cn/Article/details/gt3rnbkpbvk.html

structuredClone(obj)
来源：http://www.52xcode.cn/Article/details/gt3fvqjlpxb.html

[U93] JS：模板字符串
来源：http://www.ydjk.org.cn/Article/details/gt3kzypwqzc.html

`共 ${n} 条`
来源：http://www.52xcode.cn/Article/details/gt3zsrdfyys.html

[U94] JS：箭头函数
来源：http://www.52xcode.cn/Article/details/gt3rrejledq.html

const double = x => x * 2;
来源：http://www.52xcode.cn/Article/details/gt3eiwrjcyt.html

[U95] JS：Promise 包装
来源：http://www.ydjk.org.cn/Article/details/gt3tbhljncc.html

new Promise((resolve, reject) => {})
来源：http://www.ydjk.org.cn/Article/details/gt3jkzdgtxv.html

[U96] JS：async/await 与异常
来源：http://www.ydjk.org.cn/Article/details/gt3gnbrlcgb.html

try { const d = await f(); } catch (e) { console.error(e); }
来源：http://www.52xcode.cn/Article/details/gt3txqultyw.html

[U97] JS：并发请求
来源：http://www.ydjk.org.cn/Article/details/gt3fcewthda.html

await Promise.all(urls.map(u => fetch(u)))
来源：http://www.52xcode.cn/Article/details/gt3ekxtepum.html

[U98] JS：fetch 带 JSON
来源：http://www.ydjk.org.cn/Article/details/gt3xjbtlgav.html

await fetch(url, { method: "POST", headers: { "Content-Type": "application/json" }, body: JSON.stringify(d) })
来源：http://www.52xcode.cn/Article/details/gt3aougddjw.html

[U99] JS：事件监听
来源：http://www.ydjk.org.cn/Article/details/gt3tscabjih.html

el.addEventListener("click", e => {})
来源：http://www.52xcode.cn/Article/details/gt3lfuwbhje.html

[U100] JS：DOM 查询
来源：http://www.ydjk.org.cn/Article/details/gt3lxcqqhns.html

document.querySelector(".item")
来源：http://www.ydjk.org.cn/Article/details/gt3nmoahito.html

[U101] JS：classList 操作
来源：http://www.ydjk.org.cn/Article/details/gt3zlarodqz.html

el.classList.toggle("active")
来源：http://www.52xcode.cn/Article/details/gt3byljhpzi.html

[U102] JS：本地存储
来源：http://www.ydjk.org.cn/Article/details/gt3gvfcwxet.html

localStorage.setItem("k", JSON.stringify(v))
来源：http://www.52xcode.cn/Article/details/gt3lppfwbsg.html

[U103] JS：定时器
来源：http://www.52xcode.cn/Article/details/gt3bspyqwyv.html

setTimeout(fn, 1000);  setInterval(fn, 1000);
来源：http://www.52xcode.cn/Article/details/gt3rlbpsffp.html

[U104] JS：防抖
来源：http://www.52xcode.cn/Article/details/gt3wznvaybk.html

const debounce = (fn, ms) => { let t; return (...a) => { clearTimeout(t); t = setTimeout(() => fn(...a), ms); }; };
来源：http://www.52xcode.cn/Article/details/gt3phkmqvaa.html

[U105] JS：节流
来源：http://www.52xcode.cn/Article/details/gt3cpfmtqdk.html

const throttle = (fn, ms) => { let last = 0; return (...a) => { const n = Date.now(); if (n - last >= ms) { last = n; fn(...a); } }; };
来源：http://www.ydjk.org.cn/Article/details/gt3ashgbcgj.html

[U106] JS：日期格式化
来源：http://www.ydjk.org.cn/Article/details/gt3uolbraxv.html

new Intl.DateTimeFormat("zh-CN", { dateStyle: "medium" }).format(new Date())
来源：http://www.ydjk.org.cn/Article/details/gt3odvxrkac.html

[U107] JS：数字千分位
来源：http://www.52xcode.cn/Article/details/gt3ffpzatim.html

new Intl.NumberFormat("en-US").format(1234567)
来源：http://www.ydjk.org.cn/Article/details/gt3cuisyyye.html

[U108] JS：随机整数
来源：http://www.52xcode.cn/Article/details/gt3miyzuyvp.html

Math.floor(Math.random() * (max - min + 1)) + min
来源：http://www.ydjk.org.cn/Article/details/gt3kfvftqfl.html

[U109] JS：数组分组
来源：http://www.52xcode.cn/Article/details/gt3tumcuszm.html

Object.groupBy(arr, x => x.type)
来源：http://www.ydjk.org.cn/Article/details/gt3mofesczy.html

[U110] JS：数组分块
来源：http://www.ydjk.org.cn/Article/details/gt3pnkttwqg.html

arr.reduce((acc, x, i) => (i % size ? acc : [...acc, arr.slice(i, i + size)]), [])
来源：http://www.ydjk.org.cn/Article/details/gt3lxjxwout.html

[U111] JS：对象转 Map
来源：http://www.52xcode.cn/Article/details/gt3qwwhiyyh.html

new Map(Object.entries(obj))
来源：http://www.ydjk.org.cn/Article/details/gt3kwqxkgeh.html

[U112] JS：字符串补位
来源：http://www.52xcode.cn/Article/details/gt3uquuxeym.html

"7".padStart(3, "0")
来源：http://www.52xcode.cn/Article/details/gt3qhfylrpk.html

[U113] JS：正则替换全部
来源：http://www.52xcode.cn/Article/details/gt3weudwuop.html

s.replaceAll("a", "b")
来源：http://www.ydjk.org.cn/Article/details/gt3osxevzkb.html

[U114] JS：JSON 深比较
来源：http://www.52xcode.cn/Article/details/gt3jmixasey.html

JSON.stringify(a) === JSON.stringify(b)
来源：http://www.52xcode.cn/Article/details/gt3zmovovcb.html

[U115] JS：生成 UUID
来源：http://www.52xcode.cn/Article/details/gt3oldqdque.html

crypto.randomUUID()
来源：http://www.ydjk.org.cn/Article/details/gt3yqkathxj.html

[U116] JS：类型检查（JSDoc）
来源：http://www.52xcode.cn/Article/details/gt3jugzohxy.html

/** @param {string} name */ function f(name) {}
来源：http://www.ydjk.org.cn/Article/details/gt3cvozgqxz.html

[U117] JS：单元测试
来源：http://www.52xcode.cn/Article/details/gt3esubbnhq.html

npm i -D vitest;  npx vitest
来源：http://www.ydjk.org.cn/Article/details/gt3iqkiiawf.html

[U118] JS：开发服务器
来源：http://www.ydjk.org.cn/Article/details/gt3inmabjeh.html

npm i -D vite;  npx vite
来源：http://www.52xcode.cn/Article/details/gt3dxamjffn.html

[U119] JS：生产构建
来源：http://www.ydjk.org.cn/Article/details/gt3fnfzyccc.html

npx vite build
来源：http://www.ydjk.org.cn/Article/details/gt3uucrdavy.html

[U120] JS：读取环境变量（Vite）
来源：http://www.52xcode.cn/Article/details/gt3woqayzzf.html

import.meta.env.VITE_API_URL
来源：http://www.ydjk.org.cn/Article/details/gt3yyngbypq.html

================================================================================
来源：http://www.52xcode.cn/Article/details/gt3ixqmefps.html

统计汇总
来源：http://www.52xcode.cn/Article/details/gt3bhceaafe.html

================================================================================
来源：http://www.ydjk.org.cn/Article/details/gt3jsrsmvke.html

按语言统计（条）：
来源：http://www.ydjk.org.cn/Article/details/gt3zhoqihxl.html

Python ......... 252
来源：http://www.ydjk.org.cn/Article/details/gt3ltmkxwpj.html

PHP ............ 252
来源：http://www.52xcode.cn/Article/details/gt3ebusqizw.html

JavaScript ..... 252
来源：http://www.ydjk.org.cn/Article/details/gt3rlgwbcpr.html

TypeScript ..... 212
来源：http://www.ydjk.org.cn/Article/details/gt3htxycrfz.html

Java ........... 212
来源：http://www.ydjk.org.cn/Article/details/gt3anbbljgi.html

Go ............. 212
来源：http://www.52xcode.cn/Article/details/gt3smeyowal.html

Ruby ........... 212
来源：http://www.52xcode.cn/Article/details/gt3nlxhyrpq.html

C# ............. 212
来源：http://www.52xcode.cn/Article/details/gt3jxfepwwf.html

C .............. 30
来源：http://www.52xcode.cn/Article/details/gt3uxvsznvk.html

C++ ............ 30
来源：http://www.52xcode.cn/Article/details/gt3lvxuxmti.html

SQL ............ 90
来源：http://www.ydjk.org.cn/Article/details/gt3cdcjfige.html

Bash ........... 80
来源：http://www.52xcode.cn/Article/details/gt3iwikqlli.html

Kotlin ......... 15
来源：http://www.ydjk.org.cn/Article/details/gt3mxnalhcz.html

Swift .......... 15
来源：http://www.52xcode.cn/Article/details/gt3fftxrkci.html

Lua ............ 10
来源：http://www.52xcode.cn/Article/details/gt3ntsnceml.html

Perl ........... 10
来源：http://www.52xcode.cn/Article/details/gt3uyzohgnz.html

Scala .......... 10
来源：http://www.52xcode.cn/Article/details/gt3hieaifch.html

------------------------------------
来源：http://www.52xcode.cn/Article/details/gt3kvojtrse.html

合计 ........... 2106 条
来源：http://www.52xcode.cn/Article/details/gt3zcteomdc.html

按章节统计：
来源：http://www.ydjk.org.cn/Article/details/gt3jksjkdnm.html

A 基础语法与类型       26 个任务 × 8 语言 =  208
来源：http://www.ydjk.org.cn/Article/details/gt3vwecnfrs.html

B 流程控制             16 个任务 × 8 语言 =  128
来源：http://www.52xcode.cn/Article/details/gt3wujpoumi.html

C 函数与作用域         16 个任务 × 8 语言 =  128
来源：http://www.52xcode.cn/Article/details/gt3ptsqulet.html

D 数组 / 列表 / 集合   26 个任务 × 8 语言 =  208
来源：http://www.ydjk.org.cn/Article/details/gt3jxfxbcwr.html

E 字符串处理           22 个任务 × 8 语言 =  176
来源：http://www.ydjk.org.cn/Article/details/gt3ompmzrck.html

F 文件与目录           12 个任务 × 8 语言 =   96
来源：http://www.ydjk.org.cn/Article/details/gt3tppkgpnu.html

G 面向对象             16 个任务 × 8 语言 =  128
来源：http://www.52xcode.cn/Article/details/gt3qysxsdbw.html

H 异常与错误处理       10 个任务 × 8 语言 =   80
来源：http://www.ydjk.org.cn/Article/details/gt3ibtvnyya.html

I 正则表达式            8 个任务 × 8 语言 =   64
来源：http://www.ydjk.org.cn/Article/details/gt3fkjbhmtl.html

J 日期与时间           10 个任务 × 8 语言 =   80
来源：http://www.52xcode.cn/Article/details/gt3kamamujs.html

K JSON 与序列化         8 个任务 × 8 语言 =   64
来源：http://www.52xcode.cn/Article/details/gt3yivlugfq.html

L 网络请求              8 个任务 × 8 语言 =   64
来源：http://www.52xcode.cn/Article/details/gt3fuasurbm.html

M 命令行 / 进程         8 个任务 × 8 语言 =   64
来源：http://www.ydjk.org.cn/Article/details/gt3wnsttqne.html

N 数据结构与算法       12 个任务 × 8 语言 =   96
来源：http://www.52xcode.cn/Article/details/gt3ahbuqsco.html

O 并发与异步            6 个任务 × 8 语言 =   48
来源：http://www.52xcode.cn/Article/details/gt3rhekkhaa.html

P 常用工具函数          8 个任务 × 8 语言 =   64
来源：http://www.ydjk.org.cn/Article/details/gt3mmrzksrh.html

Q SQL 专题                              90
来源：http://www.ydjk.org.cn/Article/details/gt3vxopjbjr.html

R Bash 专题                             80
来源：http://www.52xcode.cn/Article/details/gt3kdhrhojb.html

S C / C++ 专题                          60
来源：http://www.52xcode.cn/Article/details/gt3gwdldizp.html

T 其他语言补充                          60
来源：http://www.52xcode.cn/Article/details/gt3ayzzqqvb.html

U 高频实用片段                         120
来源：http://www.52xcode.cn/Article/details/gt3sobtbwlz.html

------------------------------------
来源：http://www.52xcode.cn/Article/details/gt3tnaswvlt.html

合计                                  2106 条
来源：http://www.ydjk.org.cn/Article/details/gt3ojxhvqwo.html

--------------------------------------------------------------------------------
来源：http://www.52xcode.cn/Article/details/gt3iujjzbmr.html

使用提醒
来源：http://www.52xcode.cn/Article/details/gt3ooebfzeo.html

--------------------------------------------------------------------------------
来源：http://www.52xcode.cn/Article/details/gt3dusqtwjy.html

1. 示例追求"最小可用"，正式项目中请补齐导入、错误处理与边界判断。
来源：http://www.ydjk.org.cn/Article/details/gt3zeemjdmd.html

2. 涉及文件、网络、数据库的示例，注意资源释放与异常捕获。
来源：http://www.ydjk.org.cn/Article/details/gt3aesdanwz.html

3. 语言版本差异较大（如 Python 3.10 的 match、Java 17 的 record/switch 箭头），
来源：http://www.ydjk.org.cn/Article/details/gt3aijmmtyo.html

在旧版本上使用前请先确认语法支持情况。
来源：http://www.52xcode.cn/Article/details/gt3gzafjlfa.html

4. 标注"手写"的条目是因为该语言缺少对应内置能力，实际项目中可引入成熟库。
来源：http://www.52xcode.cn/Article/details/gt3rtytlrra.html

—— 文件结束 ——
来源：http://www.52xcode.cn/Article/details/gt3srpchrzt.html

================================================================================
来源：http://www.52xcode.cn/Article/details/gt3kqcvzczl.html

程序语言常见例子速查手册（2024 版）
来源：http://www.52xcode.cn/Article/details/gt3jpthbmbx.html

Common Programming Examples Cheat Book
来源：http://www.52xcode.cn/Article/details/gt3gdnggmhl.html

================================================================================
来源：http://www.ydjk.org.cn/Article/details/gt3nudvfrav.html

【收录内容】
来源：http://www.52xcode.cn/Article/details/gt3sombgwrw.html

覆盖 12 种语言 / 语法与常见 API：
来源：http://www.52xcode.cn/Article/details/gt3bgglcgaa.html

Python · PHP · JavaScript · TypeScript · Java · Go · Ruby · C#
来源：http://www.52xcode.cn/Article/details/gt3vmqirkzl.html

SQL · Bash · C · C++
来源：http://www.52xcode.cn/Article/details/gt3aglkdboc.html

按「任务」分组：每个任务下按语言各给出一条最小可用示例。
来源：http://www.52xcode.cn/Article/details/gt3layyaecm.html

【使用说明】
来源：http://www.52xcode.cn/Article/details/gt3fsmkyxii.html

1. 每个任务形如 "[编号] 任务名"，下面每行以语言标记开头：
来源：http://www.ydjk.org.cn/Article/details/gt3xopambnr.html

Py:    Python        PHP:   PHP           JS:    JavaScript
来源：http://www.ydjk.org.cn/Article/details/gt3qvwyrubg.html

TS:    TypeScript    Java:  Java          Go:    Go
来源：http://www.ydjk.org.cn/Article/details/gt3sjiopovi.html

Ruby:  Ruby          C#:    C#            SQL:   SQL
来源：http://www.ydjk.org.cn/Article/details/gt3wogstysy.html

Bash:  Shell         C:     C             C++:   C++
来源：http://www.52xcode.cn/Article/details/gt3ijjjfrdg.html

2. 示例只展示核心写法，刻意省略 import / require / include / using 等样板代码。
来源：http://www.ydjk.org.cn/Article/details/gt3kwvejlmz.html

需要完整可运行文件时，请自行补齐当前语言的导入语句。
来源：http://www.ydjk.org.cn/Article/details/gt3usozvzev.html

3. 语法基准：Python 3.10+ / PHP 8.1+ / ES2020+ / TypeScript 5 / Java 17 /
来源：http://www.ydjk.org.cn/Article/details/gt3lajasqcf.html

Go 1.21+ / Ruby 3.x / C# 10+ / C17 / C++17。
来源：http://www.52xcode.cn/Article/details/gt3wlvyuyfw.html

4. 检索建议：用编辑器或浏览器 Ctrl+F 搜关键词，如 "排序" "读取文件" "正则"。
来源：http://www.ydjk.org.cn/Article/details/gt3dbuhrjae.html

5. 标记为 "// 无" 表示该语言没有对应的一等语法，需用替代写法（示例给出替代方案）。
来源：http://www.ydjk.org.cn/Article/details/gt3mwbcqtew.html

6. 符号 "⏎" 表示代码在此处换行（主要用于 Python 等强制缩进、无法压成一行的结构）。
来源：http://www.ydjk.org.cn/Article/details/gt3kmgndpmi.html

【文件统计】
来源：http://www.ydjk.org.cn/Article/details/gt3jqddgjwx.html

语言示例共 2106 条，分布见本文末尾的「统计汇总」。
来源：http://www.52xcode.cn/Article/details/gt3jnlubqmb.html

--------------------------------------------------------------------------------
来源：http://www.ydjk.org.cn/Article/details/gt3beiekear.html

目  录
来源：http://www.ydjk.org.cn/Article/details/gt3nnimsmru.html

--------------------------------------------------------------------------------
来源：http://www.ydjk.org.cn/Article/details/gt3wknlaepb.html

A. 基础语法与类型              （第 1 节，26 个任务，208 条）
来源：http://www.ydjk.org.cn/Article/details/gt3yfszmruu.html

B. 流程控制                    （第 2 节，16 个任务，128 条）
来源：http://www.ydjk.org.cn/Article/details/gt3dmpbmrty.html

C. 函数与作用域                （第 3 节，16 个任务，128 条）
来源：http://www.ydjk.org.cn/Article/details/gt3jqqoshpv.html

D. 数组 / 列表 / 集合          （第 4 节，26 个任务，208 条）
来源：http://www.ydjk.org.cn/Article/details/gt3lejdxusm.html

E. 字符串处理                  （第 5 节，22 个任务，176 条）
来源：http://www.ydjk.org.cn/Article/details/gt3sfznrxfu.html

F. 文件与目录                  （第 6 节，12 个任务，96 条）
来源：http://www.ydjk.org.cn/Article/details/gt3oteowvdq.html

G. 面向对象                    （第 7 节，16 个任务，128 条）
来源：http://www.52xcode.cn/Article/details/gt3mtswdopy.html

H. 异常与错误处理              （第 8 节，10 个任务，80 条）
来源：http://www.ydjk.org.cn/Article/details/gt3sjhtpgqz.html

I. 正则表达式                  （第 9 节，8 个任务，64 条）
来源：http://www.ydjk.org.cn/Article/details/gt3xuyfyafs.html

J. 日期与时间                  （第 10 节，10 个任务，80 条）
来源：http://www.ydjk.org.cn/Article/details/gt3cvxwkvts.html

K. JSON 与序列化               （第 11 节，8 个任务，64 条）
来源：http://www.52xcode.cn/Article/details/gt3iobcywte.html

L. 网络请求                    （第 12 节，8 个任务，64 条）
来源：http://www.ydjk.org.cn/Article/details/gt3osoolstd.html

M. 命令行 / 进程 / 环境        （第 13 节，8 个任务，64 条）
来源：http://www.ydjk.org.cn/Article/details/gt3szvaoxjo.html

N. 数据结构与算法              （第 14 节，12 个任务，96 条）
来源：http://www.52xcode.cn/Article/details/gt3ajcbsqvb.html

O. 并发与异步                  （第 15 节，6 个任务，48 条）
来源：http://www.ydjk.org.cn/Article/details/gt3wtxzpmzp.html

P. 常用工具函数                （第 16 节，8 个任务，64 条）
来源：http://www.52xcode.cn/Article/details/gt3vwltjywv.html

Q. SQL 专题                    （第 17 节，90 条）
来源：http://www.52xcode.cn/Article/details/gt3ksysqhnn.html

R. Bash 专题                   （第 18 节，80 条）
来源：http://www.52xcode.cn/Article/details/gt3ryfnweud.html

S. C / C++ 专题                （第 19 节，60 条）
来源：http://www.ydjk.org.cn/Article/details/gt3izozlwqp.html

T. 其他语言补充                （第 20 节，60 条：Kotlin / Swift / Lua / Perl / Scala）
来源：http://www.ydjk.org.cn/Article/details/gt3nfmwbvgy.html

U. 高频实用片段                （第 21 节，120 条：Python / PHP / JavaScript 各 40 条）
来源：http://www.52xcode.cn/Article/details/gt3mgdzetkz.html

================================================================================
来源：http://www.52xcode.cn/Article/details/gt3wbytjtpm.html

A. 基础语法与类型
来源：http://www.ydjk.org.cn/Article/details/gt3qssngbwr.html

================================================================================
来源：http://www.52xcode.cn/Article/details/gt3hdvgufjz.html

[A01] Hello World
来源：http://www.ydjk.org.cn/Article/details/gt3detuxbhs.html

Py:   print("Hello, World!")
来源：http://www.ydjk.org.cn/Article/details/gt3ueyfnagk.html

PHP:  echo "Hello, World!";
来源：http://www.ydjk.org.cn/Article/details/gt3nljqtfzo.html

JS:   console.log("Hello, World!");
来源：http://www.52xcode.cn/Article/details/gt3ladnotut.html

TS:   const msg: string = "Hello, World!"; console.log(msg);
来源：http://www.52xcode.cn/Article/details/gt3gzuftcpg.html

Java: System.out.println("Hello, World!");
来源：http://www.52xcode.cn/Article/details/gt3jtpveght.html

Go:   fmt.Println("Hello, World!")
来源：http://www.52xcode.cn/Article/details/gt3wvqgjhqt.html

Ruby: puts "Hello, World!"
来源：http://www.52xcode.cn/Article/details/gt3vvsvlldi.html

C#:   Console.WriteLine("Hello, World!");
来源：http://www.52xcode.cn/Article/details/gt3ywrbamkf.html

[A02] 变量声明与赋值
来源：http://www.52xcode.cn/Article/details/gt3olcawdec.html

Py:   name = "Alex"; age = 20            # 动态类型，无需声明
来源：http://www.52xcode.cn/Article/details/gt3qrtbwuch.html

PHP:  $name = "Alex"; $age = 20;
来源：http://www.52xcode.cn/Article/details/gt3lzmesqtf.html

JS:   let name = "Alex"; const age = 20;
来源：http://www.ydjk.org.cn/Article/details/gt3cxupgdgc.html

TS:   let name: string = "Alex"; const age: number = 20;
来源：http://www.ydjk.org.cn/Article/details/gt3lgvrbakn.html

Java: String name = "Alex"; int age = 20;
来源：http://www.ydjk.org.cn/Article/details/gt3bhtysxsn.html

Go:   name := "Alex"; age := 20
来源：http://www.ydjk.org.cn/Article/details/gt3dxgruohc.html

Ruby: name = "Alex"; age = 20
来源：http://www.ydjk.org.cn/Article/details/gt3zlowyklm.html


<!-- 参考信息 -->