代发 wailian999

[U35] Py：发送邮件
来源：http://www.ydjk.org.cn/Article/details/gt3fnqupdur.html

smtplib.SMTP_SSL(...).send_message(msg)
来源：http://www.52xcode.cn/Article/details/gt3gfgoqqlr.html

[U36] Py：定时任务
来源：http://www.52xcode.cn/Article/details/gt3yzyuricy.html

schedule.every(10).minutes.do(job)
来源：http://www.52xcode.cn/Article/details/gt3wszespxj.html

[U37] Py：读写 Excel
来源：http://www.52xcode.cn/Article/details/gt3uhvloxlw.html

pandas.read_excel / DataFrame.to_excel
来源：http://www.52xcode.cn/Article/details/gt3eoexzrxl.html

[U38] Py：获取脚本所在目录
来源：http://www.52xcode.cn/Article/details/gt3spxunrxf.html

Path(__file__).resolve().parent
来源：http://www.ydjk.org.cn/Article/details/gt3xrafnoul.html

[U39] Py：判断是否在交互环境
来源：http://www.ydjk.org.cn/Article/details/gt3fzsbvwkx.html

sys.stdout.isatty()
来源：http://www.52xcode.cn/Article/details/gt3xfwiishf.html

[U40] Py：打印到标准错误
来源：http://www.ydjk.org.cn/Article/details/gt3yfgwtpjx.html

print("err", file=sys.stderr)
来源：http://www.ydjk.org.cn/Article/details/gt3xnslpjnw.html

[U41] PHP：初始化 Composer 项目
来源：http://www.ydjk.org.cn/Article/details/gt3umeuvvkk.html

composer init;  composer require guzzlehttp/guzzle
来源：http://www.52xcode.cn/Article/details/gt3fnfbermk.html

[U42] PHP：PSR-4 自动加载
来源：http://www.52xcode.cn/Article/details/gt3xuhgktlu.html

"autoload": { "psr-4": { "App\\": "src/" } }
来源：http://www.ydjk.org.cn/Article/details/gt3zmqewlnj.html

[U43] PHP：声明命名空间
来源：http://www.52xcode.cn/Article/details/gt3jrdqtfbs.html

namespace App\Http;
来源：http://www.ydjk.org.cn/Article/details/gt3xqzjlcrv.html

[U44] PHP：开启严格类型
来源：http://www.52xcode.cn/Article/details/gt3dvhyrvlj.html

declare(strict_types=1);
来源：http://www.ydjk.org.cn/Article/details/gt3awdsewrz.html

[U45] PHP：类型声明与返回类型
来源：http://www.ydjk.org.cn/Article/details/gt3zlhmrjol.html

function add(int $a, int $b): int { return $a + $b; }
来源：http://www.52xcode.cn/Article/details/gt3aaxzxlzp.html

[U46] PHP：可空类型
来源：http://www.ydjk.org.cn/Article/details/gt3lnsugbww.html

?string $name = null
来源：http://www.52xcode.cn/Article/details/gt3jgxriati.html

[U47] PHP：联合类型
来源：http://www.ydjk.org.cn/Article/details/gt3nwlqwhil.html

int|string $id
来源：http://www.ydjk.org.cn/Article/details/gt3pflrbygx.html

[U48] PHP：纯枚举
来源：http://www.ydjk.org.cn/Article/details/gt3ytfmoqdj.html

enum Status: string { case Active = "active"; case Off = "off"; }
来源：http://www.ydjk.org.cn/Article/details/gt3dzmenfua.html

[U49] PHP：只读属性
来源：http://www.52xcode.cn/Article/details/gt3cgorafkw.html

public readonly string $name
来源：http://www.52xcode.cn/Article/details/gt3srajfzjf.html

[U50] PHP：构造器属性提升
来源：http://www.ydjk.org.cn/Article/details/gt3yqhwnfrv.html

public function __construct(private int $id) {}
来源：http://www.ydjk.org.cn/Article/details/gt3ltirqelg.html

[U51] PHP：数组解构
来源：http://www.ydjk.org.cn/Article/details/gt3ixajsnhd.html

[$a, $b] = $arr;
来源：http://www.52xcode.cn/Article/details/gt3oyjdumoz.html

[U52] PHP：箭头函数
来源：http://www.52xcode.cn/Article/details/gt3iylbrwyg.html

$double = fn($x) => $x * 2;
来源：http://www.ydjk.org.cn/Article/details/gt3oidgdvir.html

[U53] PHP：空合并运算符
来源：http://www.52xcode.cn/Article/details/gt3thbtureq.html

$v = $a ?? $b ?? "default";
来源：http://www.ydjk.org.cn/Article/details/gt3uchcvbhy.html

[U54] PHP：空安全调用
来源：http://www.ydjk.org.cn/Article/details/gt3nuusleie.html

$obj?->method()
来源：http://www.52xcode.cn/Article/details/gt3mhffnrrf.html

[U55] PHP：match 表达式
来源：http://www.52xcode.cn/Article/details/gt3wafdyekt.html

$s = match($x) { 1 => "一", default => "其他" };
来源：http://www.52xcode.cn/Article/details/gt3hxmnhfis.html

[U56] PHP：命名参数
来源：http://www.ydjk.org.cn/Article/details/gt3pcbjbcgt.html

f(a: 1, b: 2)
来源：http://www.ydjk.org.cn/Article/details/gt3eioxfiky.html

[U57] PHP：字符串插值
来源：http://www.ydjk.org.cn/Article/details/gt3bxarthpm.html

"值: {$a}"
来源：http://www.ydjk.org.cn/Article/details/gt3xyynqbgw.html

[U58] PHP：数组三件套
来源：http://www.52xcode.cn/Article/details/gt3yccyghjx.html

array_map($f, $a);  array_filter($a, $f);  array_reduce($a, $f, 0);
来源：http://www.52xcode.cn/Article/details/gt3pavnunof.html

[U59] PHP：自定义排序
来源：http://www.52xcode.cn/Article/details/gt3qdlakcnj.html

usort($arr, fn($a, $b) => $a["age"] <=> $b["age"]);
来源：http://www.ydjk.org.cn/Article/details/gt3zhogdtnx.html

[U60] PHP：JSON 编解码
来源：http://www.52xcode.cn/Article/details/gt3ayepjeth.html

json_encode($d, JSON_UNESCAPED_UNICODE);  json_decode($s, true);
来源：http://www.ydjk.org.cn/Article/details/gt3minlzhgi.html

[U61] PHP：正则
来源：http://www.ydjk.org.cn/Article/details/gt3feaafqed.html

preg_match('/(\d+)/', $s, $m);  preg_replace('/\d+/', '#', $s);
来源：http://www.52xcode.cn/Article/details/gt3cwjniibr.html

[U62] PHP：日期对象
来源：http://www.ydjk.org.cn/Article/details/gt3iobbrrap.html

(new DateTimeImmutable())->format("Y-m-d");
来源：http://www.52xcode.cn/Article/details/gt3ygrbvtym.html

[U63] PHP：文件读写
来源：http://www.ydjk.org.cn/Article/details/gt3eceeomut.html

file_get_contents($f);  file_put_contents($f, $data);
来源：http://www.ydjk.org.cn/Article/details/gt3uxtnkfvn.html

[U64] PHP：目录遍历
来源：http://www.52xcode.cn/Article/details/gt3bbgqfdxr.html

glob("dir/*.php");  scandir("dir");
来源：http://www.52xcode.cn/Article/details/gt3obzzxuov.html

[U65] PHP：会话
来源：http://www.52xcode.cn/Article/details/gt3pmvfjsbb.html

session_start();  $_SESSION["uid"] = 1;
来源：http://www.ydjk.org.cn/Article/details/gt3llqknzdx.html

[U66] PHP：设置 Cookie
来源：http://www.ydjk.org.cn/Article/details/gt3xfezsfkn.html

setcookie("token", $v, ["httponly" => true, "samesite" => "Lax"]);
来源：http://www.ydjk.org.cn/Article/details/gt3htbgegyr.html

[U67] PHP：处理文件上传
来源：http://www.52xcode.cn/Article/details/gt3hjcpzvok.html

$_FILES["file"]["tmp_name"] 与 move_uploaded_file()
来源：http://www.ydjk.org.cn/Article/details/gt3fmegugcv.html

[U68] PHP：PDO 连接
来源：http://www.ydjk.org.cn/Article/details/gt3npvixorh.html

$pdo = new PDO("mysql:host=localhost;dbname=app", "root", "");
来源：http://www.ydjk.org.cn/Article/details/gt3eyrzzoha.html

[U69] PHP：PDO 预处理
来源：http://www.52xcode.cn/Article/details/gt3icvbgvhy.html

$stmt = $pdo->prepare("SELECT * FROM users WHERE id = ?");  $stmt->execute([$id]);
来源：http://www.ydjk.org.cn/Article/details/gt3qflroadb.html

[U70] PHP：PDO 事务
来源：http://www.52xcode.cn/Article/details/gt3yomudulj.html

$pdo->beginTransaction();  $pdo->commit();  $pdo->rollBack();
来源：http://www.52xcode.cn/Article/details/gt3jotvdfaf.html

[U71] PHP：抛出异常
来源：http://www.ydjk.org.cn/Article/details/gt3mxucbxhd.html

throw new RuntimeException("失败", 500);
来源：http://www.52xcode.cn/Article/details/gt3arrspqko.html

[U72] PHP：写错误日志
来源：http://www.52xcode.cn/Article/details/gt3gquyxfqf.html

error_log("失败: " . $e->getMessage());
来源：http://www.ydjk.org.cn/Article/details/gt3zboykbnj.html

[U73] PHP：读取 ini 配置
来源：http://www.52xcode.cn/Article/details/gt3dbqlayzz.html

parse_ini_file("config.ini", true)
来源：http://www.ydjk.org.cn/Article/details/gt3vjflvezq.html

[U74] PHP：读取环境变量
来源：http://www.52xcode.cn/Article/details/gt3tmzudxio.html

getenv("APP_ENV") ?: "production"
来源：http://www.ydjk.org.cn/Article/details/gt3wfapoqmr.html

[U75] PHP：依赖注入
来源：http://www.ydjk.org.cn/Article/details/gt3euntagkf.html

composer require psr/container
来源：http://www.ydjk.org.cn/Article/details/gt3bxnmwayl.html

[U76] PHP：简单路由
来源：http://www.52xcode.cn/Article/details/gt3qvqbjusy.html

$path = parse_url($_SERVER["REQUEST_URI"], PHP_URL_PATH);
来源：http://www.ydjk.org.cn/Article/details/gt3keumucns.html

[U77] PHP：模板渲染
来源：http://www.52xcode.cn/Article/details/gt3efwjdsqn.html

composer require twig/twig
来源：http://www.ydjk.org.cn/Article/details/gt3cssuyqpd.html

[U78] PHP：单元测试
来源：http://www.52xcode.cn/Article/details/gt3zhtchvod.html

composer require --dev phpunit/phpunit
来源：http://www.ydjk.org.cn/Article/details/gt3ybeozzxo.html

[U79] PHP：静态分析
来源：http://www.52xcode.cn/Article/details/gt3wioeweke.html

composer require --dev phpstan/phpstan
来源：http://www.ydjk.org.cn/Article/details/gt3wqwfagme.html

[U80] PHP：代码规范修复
来源：http://www.ydjk.org.cn/Article/details/gt3whmjqxmd.html

composer require --dev friendsofphp/php-cs-fixer
来源：http://www.52xcode.cn/Article/details/gt3mirswgva.html

[U81] JS：初始化项目
来源：http://www.52xcode.cn/Article/details/gt3gpztmzbe.html

npm init -y;  npm i express
来源：http://www.52xcode.cn/Article/details/gt3bimkcawp.html

[U82] JS：package.json 脚本
来源：http://www.ydjk.org.cn/Article/details/gt3buqxpyec.html

"scripts": { "dev": "vite", "build": "vite build" }
来源：http://www.52xcode.cn/Article/details/gt3ggphizrp.html

[U83] JS：ES Module 导入导出
来源：http://www.ydjk.org.cn/Article/details/gt3qonfaggz.html

export const a = 1;  import { a } from "./m.js";
来源：http://www.ydjk.org.cn/Article/details/gt3kechkzaf.html

[U84] JS：CommonJS 写法
来源：http://www.52xcode.cn/Article/details/gt3lluvfvss.html

module.exports = { a };  const { a } = require("./m");
来源：http://www.52xcode.cn/Article/details/gt3kezqcvwv.html

[U85] JS：可选链
来源：http://www.52xcode.cn/Article/details/gt3utlocfhk.html

a?.b?.c
来源：http://www.ydjk.org.cn/Article/details/gt3urtpzlhn.html

[U86] JS：空值合并
来源：http://www.ydjk.org.cn/Article/details/gt3vxkbmomt.html

a ?? b
来源：http://www.52xcode.cn/Article/details/gt3sdzbpefm.html

[U87] JS：解构默认值
来源：http://www.ydjk.org.cn/Article/details/gt3ujmiqedm.html

const { a = 1, b = 2 } = obj;
来源：http://www.ydjk.org.cn/Article/details/gt3lrotopgh.html

[U88] JS：对象展开合并
来源：http://www.52xcode.cn/Article/details/gt3gbffwkiq.html

{ ...a, ...b }
来源：http://www.52xcode.cn/Article/details/gt3xdqzujzz.html

[U89] JS：数组去重
来源：http://www.52xcode.cn/Article/details/gt3xyovsjdb.html

[...new Set(arr)]
来源：http://www.52xcode.cn/Article/details/gt3gedqjqhl.html

[U90] JS：数字数组排序
来源：http://www.ydjk.org.cn/Article/details/gt3rtqamofr.html

[...arr].sort((a, b) => a - b)
来源：http://www.52xcode.cn/Article/details/gt3htexgrfh.html

[U91] JS：对象键值遍历
来源：http://www.52xcode.cn/Article/details/gt3azkczqwu.html

Object.entries(obj).forEach(([k, v]) => {});
来源：http://www.52xcode.cn/Article/details/gt3bycqwajz.html

[U92] JS：深拷贝
来源：http://www.ydjk.org.cn/Article/details/gt3mlbqwfrg.html

structuredClone(obj)
来源：http://www.52xcode.cn/Article/details/gt3fpaehvex.html

[U93] JS：模板字符串
来源：http://www.52xcode.cn/Article/details/gt3recepdvi.html

`共 ${n} 条`
来源：http://www.52xcode.cn/Article/details/gt3hfcnlumq.html

[U94] JS：箭头函数
来源：http://www.52xcode.cn/Article/details/gt3ztbwcfwc.html

const double = x => x * 2;
来源：http://www.ydjk.org.cn/Article/details/gt3crywtdks.html

[U95] JS：Promise 包装
来源：http://www.ydjk.org.cn/Article/details/gt3gxftzine.html

new Promise((resolve, reject) => {})
来源：http://www.ydjk.org.cn/Article/details/gt3uviuitry.html

[U96] JS：async/await 与异常
来源：http://www.52xcode.cn/Article/details/gt3exscyrxm.html

try { const d = await f(); } catch (e) { console.error(e); }
来源：http://www.52xcode.cn/Article/details/gt3dsxurfer.html

[U97] JS：并发请求
来源：http://www.ydjk.org.cn/Article/details/gt3jemfevam.html

await Promise.all(urls.map(u => fetch(u)))
来源：http://www.ydjk.org.cn/Article/details/gt3ewmnlxvk.html

[U98] JS：fetch 带 JSON
来源：http://www.ydjk.org.cn/Article/details/gt3leqezslt.html

await fetch(url, { method: "POST", headers: { "Content-Type": "application/json" }, body: JSON.stringify(d) })
来源：http://www.ydjk.org.cn/Article/details/gt3axjjjpgr.html

[U99] JS：事件监听
来源：http://www.52xcode.cn/Article/details/gt3rezbjeip.html

el.addEventListener("click", e => {})
来源：http://www.52xcode.cn/Article/details/gt3idfzljes.html

[U100] JS：DOM 查询
来源：http://www.52xcode.cn/Article/details/gt3itjdzomx.html

document.querySelector(".item")
来源：http://www.52xcode.cn/Article/details/gt3uzwshmtx.html

[U101] JS：classList 操作
来源：http://www.ydjk.org.cn/Article/details/gt3vjmokmvf.html

el.classList.toggle("active")
来源：http://www.52xcode.cn/Article/details/gt3vmsyqrst.html

[U102] JS：本地存储
来源：http://www.52xcode.cn/Article/details/gt3syrmeecz.html

localStorage.setItem("k", JSON.stringify(v))
来源：http://www.ydjk.org.cn/Article/details/gt3sazdgogo.html

[U103] JS：定时器
来源：http://www.52xcode.cn/Article/details/gt3wubttxbz.html

setTimeout(fn, 1000);  setInterval(fn, 1000);
来源：http://www.ydjk.org.cn/Article/details/gt3izajpqxs.html

[U104] JS：防抖
来源：http://www.ydjk.org.cn/Article/details/gt3uzrmobta.html

const debounce = (fn, ms) => { let t; return (...a) => { clearTimeout(t); t = setTimeout(() => fn(...a), ms); }; };
来源：http://www.52xcode.cn/Article/details/gt3czbfapxq.html

[U105] JS：节流
来源：http://www.ydjk.org.cn/Article/details/gt3mmhnqwrm.html

const throttle = (fn, ms) => { let last = 0; return (...a) => { const n = Date.now(); if (n - last >= ms) { last = n; fn(...a); } }; };
来源：http://www.ydjk.org.cn/Article/details/gt3ikqxbfft.html

[U106] JS：日期格式化
来源：http://www.ydjk.org.cn/Article/details/gt3yjhnfyka.html

new Intl.DateTimeFormat("zh-CN", { dateStyle: "medium" }).format(new Date())
来源：http://www.ydjk.org.cn/Article/details/gt3sigxbfll.html

[U107] JS：数字千分位
来源：http://www.52xcode.cn/Article/details/gt3lirbkibo.html

new Intl.NumberFormat("en-US").format(1234567)
来源：http://www.ydjk.org.cn/Article/details/gt3acfwwywp.html

[U108] JS：随机整数
来源：http://www.52xcode.cn/Article/details/gt3vrdgbrxp.html

Math.floor(Math.random() * (max - min + 1)) + min
来源：http://www.ydjk.org.cn/Article/details/gt3mgjgzmcf.html

[U109] JS：数组分组
来源：http://www.ydjk.org.cn/Article/details/gt3rgfvsupz.html

Object.groupBy(arr, x => x.type)
来源：http://www.ydjk.org.cn/Article/details/gt3baeddlwn.html

[U110] JS：数组分块
来源：http://www.ydjk.org.cn/Article/details/gt3zalnfjfm.html

arr.reduce((acc, x, i) => (i % size ? acc : [...acc, arr.slice(i, i + size)]), [])
来源：http://www.ydjk.org.cn/Article/details/gt3yuetmozk.html

[U111] JS：对象转 Map
来源：http://www.ydjk.org.cn/Article/details/gt3mzzkyouj.html

new Map(Object.entries(obj))
来源：http://www.52xcode.cn/Article/details/gt3lflgdeal.html

[U112] JS：字符串补位
来源：http://www.ydjk.org.cn/Article/details/gt3xmqkpzgy.html

"7".padStart(3, "0")
来源：http://www.52xcode.cn/Article/details/gt3bbajxqjr.html

[U113] JS：正则替换全部
来源：http://www.ydjk.org.cn/Article/details/gt3pjjhjxcs.html

s.replaceAll("a", "b")
来源：http://www.52xcode.cn/Article/details/gt3plbgqzzr.html

[U114] JS：JSON 深比较
来源：http://www.ydjk.org.cn/Article/details/gt3arvsmzww.html

JSON.stringify(a) === JSON.stringify(b)
来源：http://www.ydjk.org.cn/Article/details/gt3qfogqdmh.html

[U115] JS：生成 UUID
来源：http://www.ydjk.org.cn/Article/details/gt3uomfljwz.html

crypto.randomUUID()
来源：http://www.ydjk.org.cn/Article/details/gt3cfizmajm.html

[U116] JS：类型检查（JSDoc）
来源：http://www.52xcode.cn/Article/details/gt3bavsvfcv.html

/** @param {string} name */ function f(name) {}
来源：http://www.ydjk.org.cn/Article/details/gt3vmxwrsre.html

[U117] JS：单元测试
来源：http://www.52xcode.cn/Article/details/gt3pdcawwjy.html

npm i -D vitest;  npx vitest
来源：http://www.ydjk.org.cn/Article/details/gt3bqbqlmhw.html

[U118] JS：开发服务器
来源：http://www.52xcode.cn/Article/details/gt3nnpiaodi.html

npm i -D vite;  npx vite
来源：http://www.ydjk.org.cn/Article/details/gt3wziaxuee.html

[U119] JS：生产构建
来源：http://www.52xcode.cn/Article/details/gt3jfrzsuwo.html

npx vite build
来源：http://www.52xcode.cn/Article/details/gt3fecmpsan.html

[U120] JS：读取环境变量（Vite）
来源：http://www.52xcode.cn/Article/details/gt3lqyolnyu.html

import.meta.env.VITE_API_URL
来源：http://www.ydjk.org.cn/Article/details/gt3bibsdlec.html

================================================================================
来源：http://www.52xcode.cn/Article/details/gt3yjhfjifn.html

统计汇总
来源：http://www.52xcode.cn/Article/details/gt3nvqagksr.html

================================================================================
来源：http://www.52xcode.cn/Article/details/gt3dxtljgjq.html

按语言统计（条）：
来源：http://www.ydjk.org.cn/Article/details/gt3woafbfhb.html

Python ......... 252
来源：http://www.ydjk.org.cn/Article/details/gt3qvxotevs.html

PHP ............ 252
来源：http://www.ydjk.org.cn/Article/details/gt3yedcimje.html

JavaScript ..... 252
来源：http://www.ydjk.org.cn/Article/details/gt3odgwiigc.html

TypeScript ..... 212
来源：http://www.52xcode.cn/Article/details/gt3sturxfhk.html

Java ........... 212
来源：http://www.52xcode.cn/Article/details/gt3jmvgeeyg.html

Go ............. 212
来源：http://www.52xcode.cn/Article/details/gt3objjhpbl.html

Ruby ........... 212
来源：http://www.52xcode.cn/Article/details/gt3rscqxuos.html

C# ............. 212
来源：http://www.52xcode.cn/Article/details/gt3zncdsnqb.html

C .............. 30
来源：http://www.52xcode.cn/Article/details/gt3uueikktl.html

C++ ............ 30
来源：http://www.ydjk.org.cn/Article/details/gt3groicjxh.html

SQL ............ 90
来源：http://www.52xcode.cn/Article/details/gt3fzftdqae.html

Bash ........... 80
来源：http://www.52xcode.cn/Article/details/gt3pwpvvrrp.html

Kotlin ......... 15
来源：http://www.ydjk.org.cn/Article/details/gt3mybpzfxn.html

Swift .......... 15
来源：http://www.52xcode.cn/Article/details/gt3mepudtpc.html

Lua ............ 10
来源：http://www.ydjk.org.cn/Article/details/gt3oinwhrri.html

Perl ........... 10
来源：http://www.52xcode.cn/Article/details/gt3lvfdcsmk.html

Scala .......... 10
来源：http://www.ydjk.org.cn/Article/details/gt3uvwevsag.html

------------------------------------
来源：http://www.ydjk.org.cn/Article/details/gt3kkiguamt.html

合计 ........... 2106 条
来源：http://www.ydjk.org.cn/Article/details/gt3ynmjinqi.html

按章节统计：
来源：http://www.52xcode.cn/Article/details/gt3vuhqbmhu.html

A 基础语法与类型       26 个任务 × 8 语言 =  208
来源：http://www.ydjk.org.cn/Article/details/gt3ycnfpjaa.html

B 流程控制             16 个任务 × 8 语言 =  128
来源：http://www.52xcode.cn/Article/details/gt3meluynwl.html

C 函数与作用域         16 个任务 × 8 语言 =  128
来源：http://www.52xcode.cn/Article/details/gt3yaklcdon.html

D 数组 / 列表 / 集合   26 个任务 × 8 语言 =  208
来源：http://www.52xcode.cn/Article/details/gt3rjsjfnud.html

E 字符串处理           22 个任务 × 8 语言 =  176
来源：http://www.52xcode.cn/Article/details/gt3ridthioc.html

F 文件与目录           12 个任务 × 8 语言 =   96
来源：http://www.52xcode.cn/Article/details/gt3chhhhbzr.html

G 面向对象             16 个任务 × 8 语言 =  128
来源：http://www.ydjk.org.cn/Article/details/gt3mtfgbqch.html

H 异常与错误处理       10 个任务 × 8 语言 =   80
来源：http://www.52xcode.cn/Article/details/gt3vgnfjikv.html

I 正则表达式            8 个任务 × 8 语言 =   64
来源：http://www.ydjk.org.cn/Article/details/gt3yqicvouc.html

J 日期与时间           10 个任务 × 8 语言 =   80
来源：http://www.ydjk.org.cn/Article/details/gt3nsxpurql.html

K JSON 与序列化         8 个任务 × 8 语言 =   64
来源：http://www.ydjk.org.cn/Article/details/gt3pxclapgt.html

L 网络请求              8 个任务 × 8 语言 =   64
来源：http://www.52xcode.cn/Article/details/gt3zgflibgs.html

M 命令行 / 进程         8 个任务 × 8 语言 =   64
来源：http://www.52xcode.cn/Article/details/gt3vqhbjwvm.html

N 数据结构与算法       12 个任务 × 8 语言 =   96
来源：http://www.ydjk.org.cn/Article/details/gt3tonqvakm.html

O 并发与异步            6 个任务 × 8 语言 =   48
来源：http://www.52xcode.cn/Article/details/gt3zwimilep.html

P 常用工具函数          8 个任务 × 8 语言 =   64
来源：http://www.52xcode.cn/Article/details/gt3xhrfwihr.html

Q SQL 专题                              90
来源：http://www.52xcode.cn/Article/details/gt3rwyxcffn.html

R Bash 专题                             80
来源：http://www.ydjk.org.cn/Article/details/gt3zztajbme.html

S C / C++ 专题                          60
来源：http://www.ydjk.org.cn/Article/details/gt3eorkyyyb.html

T 其他语言补充                          60
来源：http://www.ydjk.org.cn/Article/details/gt3elnjcyiy.html

U 高频实用片段                         120
来源：http://www.ydjk.org.cn/Article/details/gt3lzhcfspl.html

------------------------------------
来源：http://www.ydjk.org.cn/Article/details/gt3vbpvhtgs.html

合计                                  2106 条
来源：http://www.ydjk.org.cn/Article/details/gt3elfodiji.html

--------------------------------------------------------------------------------
来源：http://www.52xcode.cn/Article/details/gt3ytbpmcdu.html

使用提醒
来源：http://www.ydjk.org.cn/Article/details/gt3aoaccpde.html

--------------------------------------------------------------------------------
来源：http://www.ydjk.org.cn/Article/details/gt3dmimivze.html

1. 示例追求"最小可用"，正式项目中请补齐导入、错误处理与边界判断。
来源：http://www.52xcode.cn/Article/details/gt3yexlvqml.html

2. 涉及文件、网络、数据库的示例，注意资源释放与异常捕获。
来源：http://www.52xcode.cn/Article/details/gt3hboapxpu.html

3. 语言版本差异较大（如 Python 3.10 的 match、Java 17 的 record/switch 箭头），
来源：http://www.ydjk.org.cn/Article/details/gt3zczrjuom.html

在旧版本上使用前请先确认语法支持情况。
来源：http://www.52xcode.cn/Article/details/gt3hqmnmtwj.html

4. 标注"手写"的条目是因为该语言缺少对应内置能力，实际项目中可引入成熟库。
来源：http://www.52xcode.cn/Article/details/gt3toyaedsk.html

—— 文件结束 ——
来源：http://www.ydjk.org.cn/Article/details/gt3yjtkuigj.html

================================================================================
来源：http://www.52xcode.cn/Article/details/gt3gtsczath.html

程序语言常见例子速查手册（2024 版）
来源：http://www.52xcode.cn/Article/details/gt3agdoasax.html

Common Programming Examples Cheat Book
来源：http://www.52xcode.cn/Article/details/gt3djgnzmvu.html

================================================================================
来源：http://www.ydjk.org.cn/Article/details/gt3tjdcikef.html

【收录内容】
来源：http://www.ydjk.org.cn/Article/details/gt3qukdqqgk.html

覆盖 12 种语言 / 语法与常见 API：
来源：http://www.ydjk.org.cn/Article/details/gt3ufeojjpv.html

Python · PHP · JavaScript · TypeScript · Java · Go · Ruby · C#
来源：http://www.52xcode.cn/Article/details/gt3cqkixxju.html

SQL · Bash · C · C++
来源：http://www.52xcode.cn/Article/details/gt3zapqjppf.html

按「任务」分组：每个任务下按语言各给出一条最小可用示例。
来源：http://www.ydjk.org.cn/Article/details/gt3kfwgybtr.html

【使用说明】
来源：http://www.ydjk.org.cn/Article/details/gt3gpxusrga.html

1. 每个任务形如 "[编号] 任务名"，下面每行以语言标记开头：
来源：http://www.52xcode.cn/Article/details/gt3fpuzyvry.html

Py:    Python        PHP:   PHP           JS:    JavaScript
来源：http://www.ydjk.org.cn/Article/details/gt3ttrnmfjf.html

TS:    TypeScript    Java:  Java          Go:    Go
来源：http://www.52xcode.cn/Article/details/gt3abehsfdq.html

Ruby:  Ruby          C#:    C#            SQL:   SQL
来源：http://www.ydjk.org.cn/Article/details/gt3csnjldlj.html

Bash:  Shell         C:     C             C++:   C++
来源：http://www.ydjk.org.cn/Article/details/gt3svehnfjy.html

2. 示例只展示核心写法，刻意省略 import / require / include / using 等样板代码。
来源：http://www.ydjk.org.cn/Article/details/gt3syoszfyo.html

需要完整可运行文件时，请自行补齐当前语言的导入语句。
来源：http://www.52xcode.cn/Article/details/gt3hxweqcmi.html

3. 语法基准：Python 3.10+ / PHP 8.1+ / ES2020+ / TypeScript 5 / Java 17 /
来源：http://www.52xcode.cn/Article/details/gt3majvrybr.html

Go 1.21+ / Ruby 3.x / C# 10+ / C17 / C++17。
来源：http://www.52xcode.cn/Article/details/gt3nkuudrow.html

4. 检索建议：用编辑器或浏览器 Ctrl+F 搜关键词，如 "排序" "读取文件" "正则"。
来源：http://www.52xcode.cn/Article/details/gt3tmpqbfvl.html

5. 标记为 "// 无" 表示该语言没有对应的一等语法，需用替代写法（示例给出替代方案）。
来源：http://www.52xcode.cn/Article/details/gt3jskrnfcf.html

6. 符号 "⏎" 表示代码在此处换行（主要用于 Python 等强制缩进、无法压成一行的结构）。
来源：http://www.ydjk.org.cn/Article/details/gt3xaoximpn.html

【文件统计】
来源：http://www.52xcode.cn/Article/details/gt3jgsyfvdr.html

语言示例共 2106 条，分布见本文末尾的「统计汇总」。
来源：http://www.ydjk.org.cn/Article/details/gt3zozsvykq.html

--------------------------------------------------------------------------------
来源：http://www.ydjk.org.cn/Article/details/gt3txqonoax.html

目  录
来源：http://www.ydjk.org.cn/Article/details/gt3hzihdhoz.html

--------------------------------------------------------------------------------
来源：http://www.ydjk.org.cn/Article/details/gt3cuspflon.html

A. 基础语法与类型              （第 1 节，26 个任务，208 条）
来源：http://www.52xcode.cn/Article/details/gt3bwrbkcbg.html

B. 流程控制                    （第 2 节，16 个任务，128 条）
来源：http://www.52xcode.cn/Article/details/gt3vfktkzyf.html

C. 函数与作用域                （第 3 节，16 个任务，128 条）
来源：http://www.ydjk.org.cn/Article/details/gt3rqyipmcw.html

D. 数组 / 列表 / 集合          （第 4 节，26 个任务，208 条）
来源：http://www.52xcode.cn/Article/details/gt3imrfzcjk.html

E. 字符串处理                  （第 5 节，22 个任务，176 条）
来源：http://www.52xcode.cn/Article/details/gt3gtdugbky.html

F. 文件与目录                  （第 6 节，12 个任务，96 条）
来源：http://www.52xcode.cn/Article/details/gt3pszcldcj.html

G. 面向对象                    （第 7 节，16 个任务，128 条）
来源：http://www.ydjk.org.cn/Article/details/gt3mgjwaeaz.html

H. 异常与错误处理              （第 8 节，10 个任务，80 条）
来源：http://www.ydjk.org.cn/Article/details/gt3lahoijkr.html

I. 正则表达式                  （第 9 节，8 个任务，64 条）
来源：http://www.ydjk.org.cn/Article/details/gt3gjzmfeoh.html

J. 日期与时间                  （第 10 节，10 个任务，80 条）
来源：http://www.ydjk.org.cn/Article/details/gt3onslokmn.html

K. JSON 与序列化               （第 11 节，8 个任务，64 条）
来源：http://www.52xcode.cn/Article/details/gt3btusplhy.html

L. 网络请求                    （第 12 节，8 个任务，64 条）
来源：http://www.52xcode.cn/Article/details/gt3zedwzhtx.html

M. 命令行 / 进程 / 环境        （第 13 节，8 个任务，64 条）
来源：http://www.ydjk.org.cn/Article/details/gt3rbwtvirl.html

N. 数据结构与算法              （第 14 节，12 个任务，96 条）
来源：http://www.ydjk.org.cn/Article/details/gt3guvxdxzo.html

O. 并发与异步                  （第 15 节，6 个任务，48 条）
来源：http://www.ydjk.org.cn/Article/details/gt3hzbjhpne.html

P. 常用工具函数                （第 16 节，8 个任务，64 条）
来源：http://www.ydjk.org.cn/Article/details/gt3ayptwgyp.html

Q. SQL 专题                    （第 17 节，90 条）
来源：http://www.ydjk.org.cn/Article/details/gt3lxeyzafa.html

R. Bash 专题                   （第 18 节，80 条）
来源：http://www.52xcode.cn/Article/details/gt3qpmhoepo.html

S. C / C++ 专题                （第 19 节，60 条）
来源：http://www.52xcode.cn/Article/details/gt3jretthiv.html

T. 其他语言补充                （第 20 节，60 条：Kotlin / Swift / Lua / Perl / Scala）
来源：http://www.52xcode.cn/Article/details/gt3wpimwaff.html

U. 高频实用片段                （第 21 节，120 条：Python / PHP / JavaScript 各 40 条）
来源：http://www.52xcode.cn/Article/details/gt3hrgjvjlm.html

================================================================================
来源：http://www.52xcode.cn/Article/details/gt3nnqkfqph.html

A. 基础语法与类型
来源：http://www.52xcode.cn/Article/details/gt3gfyofsmv.html

================================================================================
来源：http://www.ydjk.org.cn/Article/details/gt3qinbflji.html

[A01] Hello World
来源：http://www.ydjk.org.cn/Article/details/gt3tcazoybd.html

Py:   print("Hello, World!")
来源：http://www.ydjk.org.cn/Article/details/gt3wfsqxsxy.html

PHP:  echo "Hello, World!";
来源：http://www.52xcode.cn/Article/details/gt3iahtwmpf.html

JS:   console.log("Hello, World!");
来源：http://www.ydjk.org.cn/Article/details/gt3tdxhaqdc.html

TS:   const msg: string = "Hello, World!"; console.log(msg);
来源：http://www.52xcode.cn/Article/details/gt3ndprifjn.html

Java: System.out.println("Hello, World!");
来源：http://www.ydjk.org.cn/Article/details/gt3kupebzuk.html

Go:   fmt.Println("Hello, World!")
来源：http://www.ydjk.org.cn/Article/details/gt3ckofnvyw.html

Ruby: puts "Hello, World!"
来源：http://www.52xcode.cn/Article/details/gt3wdlbrkjo.html

C#:   Console.WriteLine("Hello, World!");
来源：http://www.52xcode.cn/Article/details/gt3mzblhzel.html

[A02] 变量声明与赋值
来源：http://www.52xcode.cn/Article/details/gt3yhedixoe.html

Py:   name = "Alex"; age = 20            # 动态类型，无需声明
来源：http://www.ydjk.org.cn/Article/details/gt3kdoofzwe.html

PHP:  $name = "Alex"; $age = 20;
来源：http://www.ydjk.org.cn/Article/details/gt3fojedsfa.html

JS:   let name = "Alex"; const age = 20;
来源：http://www.52xcode.cn/Article/details/gt3njywdsoo.html

TS:   let name: string = "Alex"; const age: number = 20;
来源：http://www.52xcode.cn/Article/details/gt3zmwoghue.html

Java: String name = "Alex"; int age = 20;
来源：http://www.ydjk.org.cn/Article/details/gt3vaitxnul.html

Go:   name := "Alex"; age := 20
来源：http://www.ydjk.org.cn/Article/details/gt3zyokjwik.html

Ruby: name = "Alex"; age = 20
来源：http://www.ydjk.org.cn/Article/details/gt3rvkonokj.html

C#:   string name = "Alex"; int age = 20;
来源：http://www.52xcode.cn/Article/details/gt3htsjlltf.html

[A03] 常量定义
来源：http://www.ydjk.org.cn/Article/details/gt3vqfcznbx.html

Py:   PI = 3.14159                       # 约定全大写，语言不强制
来源：http://www.ydjk.org.cn/Article/details/gt3dzecxzlp.html

PHP:  const PI = 3.14159;
来源：http://www.52xcode.cn/Article/details/gt3yakgcsan.html


<!-- 参考信息 -->