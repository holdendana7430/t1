代发 wailian999

[U31] Py：单测
来源：http://www.52xcode.cn/Article/details/gt3nytqgwke.html

python -m pytest -q
来源：http://www.ydjk.org.cn/Article/details/gt3fvkzrtfd.html

[U32] Py：代码格式化
来源：http://www.52xcode.cn/Article/details/gt3kuhfekcb.html

ruff format . && ruff check --fix .
来源：http://www.ydjk.org.cn/Article/details/gt3pvxytqld.html

[U33] Py：打包发布
来源：http://www.ydjk.org.cn/Article/details/gt3siengjwt.html

python -m build  （依赖 pyproject.toml）
来源：http://www.52xcode.cn/Article/details/gt3wiemmrtb.html

[U34] Py：判断编码
来源：http://www.52xcode.cn/Article/details/gt3zlezjpii.html

chardet.detect(raw)
来源：http://www.ydjk.org.cn/Article/details/gt3uptmeeic.html

[U35] Py：发送邮件
来源：http://www.ydjk.org.cn/Article/details/gt3wulzhlub.html

smtplib.SMTP_SSL(...).send_message(msg)
来源：http://www.52xcode.cn/Article/details/gt3cufikxmj.html

[U36] Py：定时任务
来源：http://www.52xcode.cn/Article/details/gt3nlbutpcf.html

schedule.every(10).minutes.do(job)
来源：http://www.ydjk.org.cn/Article/details/gt3apuifbob.html

[U37] Py：读写 Excel
来源：http://www.ydjk.org.cn/Article/details/gt3bpdnhxoc.html

pandas.read_excel / DataFrame.to_excel
来源：http://www.52xcode.cn/Article/details/gt3raveoofe.html

[U38] Py：获取脚本所在目录
来源：http://www.ydjk.org.cn/Article/details/gt3nkpmkaaa.html

Path(__file__).resolve().parent
来源：http://www.ydjk.org.cn/Article/details/gt3xaukyips.html

[U39] Py：判断是否在交互环境
来源：http://www.ydjk.org.cn/Article/details/gt3wmaxqmne.html

sys.stdout.isatty()
来源：http://www.52xcode.cn/Article/details/gt3wbcojkxu.html

[U40] Py：打印到标准错误
来源：http://www.ydjk.org.cn/Article/details/gt3andjrlxi.html

print("err", file=sys.stderr)
来源：http://www.ydjk.org.cn/Article/details/gt3cfdmkruz.html

[U41] PHP：初始化 Composer 项目
来源：http://www.ydjk.org.cn/Article/details/gt3qmksdbri.html

composer init;  composer require guzzlehttp/guzzle
来源：http://www.52xcode.cn/Article/details/gt3rmvarzfz.html

[U42] PHP：PSR-4 自动加载
来源：http://www.ydjk.org.cn/Article/details/gt3htmgjzgb.html

"autoload": { "psr-4": { "App\\": "src/" } }
来源：http://www.ydjk.org.cn/Article/details/gt3fzjdnjag.html

[U43] PHP：声明命名空间
来源：http://www.52xcode.cn/Article/details/gt3zuegemvp.html

namespace App\Http;
来源：http://www.52xcode.cn/Article/details/gt3llzbdhvo.html

[U44] PHP：开启严格类型
来源：http://www.ydjk.org.cn/Article/details/gt3enrvxhvq.html

declare(strict_types=1);
来源：http://www.52xcode.cn/Article/details/gt3xstweind.html

[U45] PHP：类型声明与返回类型
来源：http://www.52xcode.cn/Article/details/gt3fcswhznu.html

function add(int $a, int $b): int { return $a + $b; }
来源：http://www.ydjk.org.cn/Article/details/gt3azoztbqv.html

[U46] PHP：可空类型
来源：http://www.52xcode.cn/Article/details/gt3xcczimdx.html

?string $name = null
来源：http://www.ydjk.org.cn/Article/details/gt3elppeeis.html

[U47] PHP：联合类型
来源：http://www.ydjk.org.cn/Article/details/gt3ejhamktm.html

int|string $id
来源：http://www.ydjk.org.cn/Article/details/gt3njimdokx.html

[U48] PHP：纯枚举
来源：http://www.52xcode.cn/Article/details/gt3isuuvtcz.html

enum Status: string { case Active = "active"; case Off = "off"; }
来源：http://www.52xcode.cn/Article/details/gt3plmyfmwz.html

[U49] PHP：只读属性
来源：http://www.ydjk.org.cn/Article/details/gt3cnjhablz.html

public readonly string $name
来源：http://www.ydjk.org.cn/Article/details/gt3eqeyzkjc.html

[U50] PHP：构造器属性提升
来源：http://www.52xcode.cn/Article/details/gt3fxskyyhz.html

public function __construct(private int $id) {}
来源：http://www.ydjk.org.cn/Article/details/gt3lyorlpmf.html

[U51] PHP：数组解构
来源：http://www.ydjk.org.cn/Article/details/gt3syctcgjm.html

[$a, $b] = $arr;
来源：http://www.ydjk.org.cn/Article/details/gt3zmhhvvru.html

[U52] PHP：箭头函数
来源：http://www.52xcode.cn/Article/details/gt3bbhubxzw.html

$double = fn($x) => $x * 2;
来源：http://www.ydjk.org.cn/Article/details/gt3inlwfgnd.html

[U53] PHP：空合并运算符
来源：http://www.52xcode.cn/Article/details/gt3iplcbzvl.html

$v = $a ?? $b ?? "default";
来源：http://www.ydjk.org.cn/Article/details/gt3dxyvaaaq.html

[U54] PHP：空安全调用
来源：http://www.52xcode.cn/Article/details/gt3artuadcf.html

$obj?->method()
来源：http://www.ydjk.org.cn/Article/details/gt3doqdkgdv.html

[U55] PHP：match 表达式
来源：http://www.52xcode.cn/Article/details/gt3ajuquveb.html

$s = match($x) { 1 => "一", default => "其他" };
来源：http://www.ydjk.org.cn/Article/details/gt3raznflww.html

[U56] PHP：命名参数
来源：http://www.ydjk.org.cn/Article/details/gt3bjwayqcn.html

f(a: 1, b: 2)
来源：http://www.ydjk.org.cn/Article/details/gt3jbsckicz.html

[U57] PHP：字符串插值
来源：http://www.52xcode.cn/Article/details/gt3fpcvxknv.html

"值: {$a}"
来源：http://www.52xcode.cn/Article/details/gt3vjikoixo.html

[U58] PHP：数组三件套
来源：http://www.ydjk.org.cn/Article/details/gt3cyrdueoo.html

array_map($f, $a);  array_filter($a, $f);  array_reduce($a, $f, 0);
来源：http://www.52xcode.cn/Article/details/gt3kzwrywpu.html

[U59] PHP：自定义排序
来源：http://www.ydjk.org.cn/Article/details/gt3dnicrtuw.html

usort($arr, fn($a, $b) => $a["age"] <=> $b["age"]);
来源：http://www.52xcode.cn/Article/details/gt3afsfsipu.html

[U60] PHP：JSON 编解码
来源：http://www.ydjk.org.cn/Article/details/gt3qyohtxsl.html

json_encode($d, JSON_UNESCAPED_UNICODE);  json_decode($s, true);
来源：http://www.ydjk.org.cn/Article/details/gt3gtqyoxgv.html

[U61] PHP：正则
来源：http://www.ydjk.org.cn/Article/details/gt3inzfxvcs.html

preg_match('/(\d+)/', $s, $m);  preg_replace('/\d+/', '#', $s);
来源：http://www.ydjk.org.cn/Article/details/gt3zgzywrtf.html

[U62] PHP：日期对象
来源：http://www.52xcode.cn/Article/details/gt3whaszokx.html

(new DateTimeImmutable())->format("Y-m-d");
来源：http://www.ydjk.org.cn/Article/details/gt3xsosixjk.html

[U63] PHP：文件读写
来源：http://www.ydjk.org.cn/Article/details/gt3lumgpopz.html

file_get_contents($f);  file_put_contents($f, $data);
来源：http://www.52xcode.cn/Article/details/gt3wnbicjtw.html

[U64] PHP：目录遍历
来源：http://www.ydjk.org.cn/Article/details/gt3rftqxtbl.html

glob("dir/*.php");  scandir("dir");
来源：http://www.52xcode.cn/Article/details/gt3wiwhzyfz.html

[U65] PHP：会话
来源：http://www.52xcode.cn/Article/details/gt3xyxxgfdq.html

session_start();  $_SESSION["uid"] = 1;
来源：http://www.52xcode.cn/Article/details/gt3evmiruso.html

[U66] PHP：设置 Cookie
来源：http://www.ydjk.org.cn/Article/details/gt3muudzfic.html

setcookie("token", $v, ["httponly" => true, "samesite" => "Lax"]);
来源：http://www.52xcode.cn/Article/details/gt3sddxygfk.html

[U67] PHP：处理文件上传
来源：http://www.52xcode.cn/Article/details/gt3ixlxbnwm.html

$_FILES["file"]["tmp_name"] 与 move_uploaded_file()
来源：http://www.ydjk.org.cn/Article/details/gt3yhidjkph.html

[U68] PHP：PDO 连接
来源：http://www.ydjk.org.cn/Article/details/gt3ujofngpc.html

$pdo = new PDO("mysql:host=localhost;dbname=app", "root", "");
来源：http://www.ydjk.org.cn/Article/details/gt3cluvzeee.html

[U69] PHP：PDO 预处理
来源：http://www.52xcode.cn/Article/details/gt3woftlnio.html

$stmt = $pdo->prepare("SELECT * FROM users WHERE id = ?");  $stmt->execute([$id]);
来源：http://www.52xcode.cn/Article/details/gt3ndrimada.html

[U70] PHP：PDO 事务
来源：http://www.ydjk.org.cn/Article/details/gt3rkjmdpli.html

$pdo->beginTransaction();  $pdo->commit();  $pdo->rollBack();
来源：http://www.52xcode.cn/Article/details/gt3uiwvbhyo.html

[U71] PHP：抛出异常
来源：http://www.52xcode.cn/Article/details/gt3sjacwkqj.html

throw new RuntimeException("失败", 500);
来源：http://www.52xcode.cn/Article/details/gt3gpivnpoo.html

[U72] PHP：写错误日志
来源：http://www.52xcode.cn/Article/details/gt3jbkumgse.html

error_log("失败: " . $e->getMessage());
来源：http://www.52xcode.cn/Article/details/gt3eunfpohi.html

[U73] PHP：读取 ini 配置
来源：http://www.52xcode.cn/Article/details/gt3qblrhdux.html

parse_ini_file("config.ini", true)
来源：http://www.52xcode.cn/Article/details/gt3frpuxfzh.html

[U74] PHP：读取环境变量
来源：http://www.ydjk.org.cn/Article/details/gt3gfguhzio.html

getenv("APP_ENV") ?: "production"
来源：http://www.ydjk.org.cn/Article/details/gt3cjmsbqzq.html

[U75] PHP：依赖注入
来源：http://www.ydjk.org.cn/Article/details/gt3wavwmtqc.html

composer require psr/container
来源：http://www.ydjk.org.cn/Article/details/gt3cloceqgs.html

[U76] PHP：简单路由
来源：http://www.52xcode.cn/Article/details/gt3apqyqyxi.html

$path = parse_url($_SERVER["REQUEST_URI"], PHP_URL_PATH);
来源：http://www.ydjk.org.cn/Article/details/gt3msibtyzb.html

[U77] PHP：模板渲染
来源：http://www.ydjk.org.cn/Article/details/gt3gofdpuxn.html

composer require twig/twig
来源：http://www.52xcode.cn/Article/details/gt3uselvhxv.html

[U78] PHP：单元测试
来源：http://www.52xcode.cn/Article/details/gt3fkbbdpdw.html

composer require --dev phpunit/phpunit
来源：http://www.52xcode.cn/Article/details/gt3qpwxntol.html

[U79] PHP：静态分析
来源：http://www.ydjk.org.cn/Article/details/gt3eqxccvvx.html

composer require --dev phpstan/phpstan
来源：http://www.52xcode.cn/Article/details/gt3fjycvrdm.html

[U80] PHP：代码规范修复
来源：http://www.52xcode.cn/Article/details/gt3dilubxhq.html

composer require --dev friendsofphp/php-cs-fixer
来源：http://www.52xcode.cn/Article/details/gt3xbxrkmgw.html

[U81] JS：初始化项目
来源：http://www.52xcode.cn/Article/details/gt3hnnjctyp.html

npm init -y;  npm i express
来源：http://www.ydjk.org.cn/Article/details/gt3mxqlkjzy.html

[U82] JS：package.json 脚本
来源：http://www.ydjk.org.cn/Article/details/gt3ulvlikcv.html

"scripts": { "dev": "vite", "build": "vite build" }
来源：http://www.52xcode.cn/Article/details/gt3imqwywyl.html

[U83] JS：ES Module 导入导出
来源：http://www.ydjk.org.cn/Article/details/gt3blrmvkyb.html

export const a = 1;  import { a } from "./m.js";
来源：http://www.ydjk.org.cn/Article/details/gt3xskipqsm.html

[U84] JS：CommonJS 写法
来源：http://www.52xcode.cn/Article/details/gt3tardpplu.html

module.exports = { a };  const { a } = require("./m");
来源：http://www.ydjk.org.cn/Article/details/gt3gtfwlspv.html

[U85] JS：可选链
来源：http://www.ydjk.org.cn/Article/details/gt3cjerghhj.html

a?.b?.c
来源：http://www.52xcode.cn/Article/details/gt3pludwdtu.html

[U86] JS：空值合并
来源：http://www.52xcode.cn/Article/details/gt3gxsojkjp.html

a ?? b
来源：http://www.ydjk.org.cn/Article/details/gt3estryece.html

[U87] JS：解构默认值
来源：http://www.ydjk.org.cn/Article/details/gt3jfqbnrtr.html

const { a = 1, b = 2 } = obj;
来源：http://www.52xcode.cn/Article/details/gt3qctnppjw.html

[U88] JS：对象展开合并
来源：http://www.ydjk.org.cn/Article/details/gt3yksgiuod.html

{ ...a, ...b }
来源：http://www.52xcode.cn/Article/details/gt3xnaiyaak.html

[U89] JS：数组去重
来源：http://www.ydjk.org.cn/Article/details/gt3jkpaarhr.html

[...new Set(arr)]
来源：http://www.52xcode.cn/Article/details/gt3naytthoo.html

[U90] JS：数字数组排序
来源：http://www.52xcode.cn/Article/details/gt3enphdhqs.html

[...arr].sort((a, b) => a - b)
来源：http://www.ydjk.org.cn/Article/details/gt3wgykwqzt.html

[U91] JS：对象键值遍历
来源：http://www.ydjk.org.cn/Article/details/gt3pfqwwlft.html

Object.entries(obj).forEach(([k, v]) => {});
来源：http://www.ydjk.org.cn/Article/details/gt3kmjjtthe.html

[U92] JS：深拷贝
来源：http://www.52xcode.cn/Article/details/gt3wghhcpct.html

structuredClone(obj)
来源：http://www.ydjk.org.cn/Article/details/gt3szczglkd.html

[U93] JS：模板字符串
来源：http://www.52xcode.cn/Article/details/gt3uphprskj.html

`共 ${n} 条`
来源：http://www.52xcode.cn/Article/details/gt3gqjgczuy.html

[U94] JS：箭头函数
来源：http://www.ydjk.org.cn/Article/details/gt3umjofojx.html

const double = x => x * 2;
来源：http://www.52xcode.cn/Article/details/gt3ozvisbwn.html

[U95] JS：Promise 包装
来源：http://www.ydjk.org.cn/Article/details/gt3xgnwezzh.html

new Promise((resolve, reject) => {})
来源：http://www.ydjk.org.cn/Article/details/gt3papgfisq.html

[U96] JS：async/await 与异常
来源：http://www.52xcode.cn/Article/details/gt3tnyiifos.html

try { const d = await f(); } catch (e) { console.error(e); }
来源：http://www.ydjk.org.cn/Article/details/gt3umlulqbs.html

[U97] JS：并发请求
来源：http://www.52xcode.cn/Article/details/gt3ouulrmda.html

await Promise.all(urls.map(u => fetch(u)))
来源：http://www.52xcode.cn/Article/details/gt3xefrqppk.html

[U98] JS：fetch 带 JSON
来源：http://www.52xcode.cn/Article/details/gt3pwnrglcf.html

await fetch(url, { method: "POST", headers: { "Content-Type": "application/json" }, body: JSON.stringify(d) })
来源：http://www.ydjk.org.cn/Article/details/gt3zsjpordh.html

[U99] JS：事件监听
来源：http://www.ydjk.org.cn/Article/details/gt3gdtzlygv.html

el.addEventListener("click", e => {})
来源：http://www.52xcode.cn/Article/details/gt3plbrodzr.html

[U100] JS：DOM 查询
来源：http://www.ydjk.org.cn/Article/details/gt3effauvea.html

document.querySelector(".item")
来源：http://www.52xcode.cn/Article/details/gt3kcdzmkju.html

[U101] JS：classList 操作
来源：http://www.52xcode.cn/Article/details/gt3egroygpb.html

el.classList.toggle("active")
来源：http://www.52xcode.cn/Article/details/gt3puotywbl.html

[U102] JS：本地存储
来源：http://www.ydjk.org.cn/Article/details/gt3mqbocjby.html

localStorage.setItem("k", JSON.stringify(v))
来源：http://www.ydjk.org.cn/Article/details/gt3cjzevaom.html

[U103] JS：定时器
来源：http://www.ydjk.org.cn/Article/details/gt3bhwooizo.html

setTimeout(fn, 1000);  setInterval(fn, 1000);
来源：http://www.ydjk.org.cn/Article/details/gt3kajlboou.html

[U104] JS：防抖
来源：http://www.52xcode.cn/Article/details/gt3oanchcgu.html

const debounce = (fn, ms) => { let t; return (...a) => { clearTimeout(t); t = setTimeout(() => fn(...a), ms); }; };
来源：http://www.ydjk.org.cn/Article/details/gt3ujkterat.html

[U105] JS：节流
来源：http://www.ydjk.org.cn/Article/details/gt3mqushphr.html

const throttle = (fn, ms) => { let last = 0; return (...a) => { const n = Date.now(); if (n - last >= ms) { last = n; fn(...a); } }; };
来源：http://www.52xcode.cn/Article/details/gt3bogcoeeh.html

[U106] JS：日期格式化
来源：http://www.ydjk.org.cn/Article/details/gt3hfggujev.html

new Intl.DateTimeFormat("zh-CN", { dateStyle: "medium" }).format(new Date())
来源：http://www.52xcode.cn/Article/details/gt3evbhjiaq.html

[U107] JS：数字千分位
来源：http://www.52xcode.cn/Article/details/gt3wackqbzw.html

new Intl.NumberFormat("en-US").format(1234567)
来源：http://www.52xcode.cn/Article/details/gt3mlitljqx.html

[U108] JS：随机整数
来源：http://www.52xcode.cn/Article/details/gt3frbaqnnk.html

Math.floor(Math.random() * (max - min + 1)) + min
来源：http://www.ydjk.org.cn/Article/details/gt3fxljhmpu.html

[U109] JS：数组分组
来源：http://www.52xcode.cn/Article/details/gt3rjdeanvm.html

Object.groupBy(arr, x => x.type)
来源：http://www.ydjk.org.cn/Article/details/gt3hltlbhsq.html

[U110] JS：数组分块
来源：http://www.52xcode.cn/Article/details/gt3vntxqjmh.html

arr.reduce((acc, x, i) => (i % size ? acc : [...acc, arr.slice(i, i + size)]), [])
来源：http://www.52xcode.cn/Article/details/gt3vnbxgtky.html

[U111] JS：对象转 Map
来源：http://www.52xcode.cn/Article/details/gt3lpymsgvy.html

new Map(Object.entries(obj))
来源：http://www.ydjk.org.cn/Article/details/gt3npljpopj.html

[U112] JS：字符串补位
来源：http://www.52xcode.cn/Article/details/gt3wdumxvwq.html

"7".padStart(3, "0")
来源：http://www.52xcode.cn/Article/details/gt3fwbkvzey.html

[U113] JS：正则替换全部
来源：http://www.ydjk.org.cn/Article/details/gt3mvwizssj.html

s.replaceAll("a", "b")
来源：http://www.ydjk.org.cn/Article/details/gt3kslajywm.html

[U114] JS：JSON 深比较
来源：http://www.52xcode.cn/Article/details/gt3rokxojoq.html

JSON.stringify(a) === JSON.stringify(b)
来源：http://www.ydjk.org.cn/Article/details/gt3jjfyulaq.html

[U115] JS：生成 UUID
来源：http://www.ydjk.org.cn/Article/details/gt3yjkuuesa.html

crypto.randomUUID()
来源：http://www.52xcode.cn/Article/details/gt3hrsneies.html

[U116] JS：类型检查（JSDoc）
来源：http://www.52xcode.cn/Article/details/gt3pwtbvhbo.html

/** @param {string} name */ function f(name) {}
来源：http://www.ydjk.org.cn/Article/details/gt3shzeolfp.html

[U117] JS：单元测试
来源：http://www.ydjk.org.cn/Article/details/gt3sjnepffo.html

npm i -D vitest;  npx vitest
来源：http://www.52xcode.cn/Article/details/gt3oefnzdlw.html

[U118] JS：开发服务器
来源：http://www.52xcode.cn/Article/details/gt3xpsiukwq.html

npm i -D vite;  npx vite
来源：http://www.52xcode.cn/Article/details/gt3awmwqcyn.html

[U119] JS：生产构建
来源：http://www.52xcode.cn/Article/details/gt3tppvmaqj.html

npx vite build
来源：http://www.52xcode.cn/Article/details/gt3fcimiwgu.html

[U120] JS：读取环境变量（Vite）
来源：http://www.52xcode.cn/Article/details/gt3jbbugrpi.html

import.meta.env.VITE_API_URL
来源：http://www.52xcode.cn/Article/details/gt3rjltglii.html

================================================================================
来源：http://www.52xcode.cn/Article/details/gt3sirdvwkv.html

统计汇总
来源：http://www.52xcode.cn/Article/details/gt3oscpvbec.html

================================================================================
来源：http://www.52xcode.cn/Article/details/gt3gjgvakcm.html

按语言统计（条）：
来源：http://www.52xcode.cn/Article/details/gt3ufyyqexx.html

Python ......... 252
来源：http://www.52xcode.cn/Article/details/gt3kpstvkqr.html

PHP ............ 252
来源：http://www.ydjk.org.cn/Article/details/gt3qaxptpio.html

JavaScript ..... 252
来源：http://www.ydjk.org.cn/Article/details/gt3byiixvqd.html

TypeScript ..... 212
来源：http://www.52xcode.cn/Article/details/gt3lgngpdhu.html

Java ........... 212
来源：http://www.52xcode.cn/Article/details/gt3pedpsofx.html

Go ............. 212
来源：http://www.ydjk.org.cn/Article/details/gt3zgabtaes.html

Ruby ........... 212
来源：http://www.ydjk.org.cn/Article/details/gt3mjwiiugi.html

C# ............. 212
来源：http://www.ydjk.org.cn/Article/details/gt3kqyejuwq.html

C .............. 30
来源：http://www.52xcode.cn/Article/details/gt3jusxordc.html

C++ ............ 30
来源：http://www.52xcode.cn/Article/details/gt3obertxzz.html

SQL ............ 90
来源：http://www.52xcode.cn/Article/details/gt3keukmkmy.html

Bash ........... 80
来源：http://www.ydjk.org.cn/Article/details/gt3qwqbfrhl.html

Kotlin ......... 15
来源：http://www.52xcode.cn/Article/details/gt3kerviooz.html

Swift .......... 15
来源：http://www.52xcode.cn/Article/details/gt3hatmprvj.html

Lua ............ 10
来源：http://www.52xcode.cn/Article/details/gt3pyvdqufe.html

Perl ........... 10
来源：http://www.52xcode.cn/Article/details/gt3gkndhcqy.html

Scala .......... 10
来源：http://www.ydjk.org.cn/Article/details/gt3kknpadex.html

------------------------------------
来源：http://www.ydjk.org.cn/Article/details/gt3rrbklccz.html

合计 ........... 2106 条
来源：http://www.ydjk.org.cn/Article/details/gt3jkyaqywq.html

按章节统计：
来源：http://www.52xcode.cn/Article/details/gt3vmrlixir.html

A 基础语法与类型       26 个任务 × 8 语言 =  208
来源：http://www.52xcode.cn/Article/details/gt3fnsqijur.html

B 流程控制             16 个任务 × 8 语言 =  128
来源：http://www.52xcode.cn/Article/details/gt3cahaxjyw.html

C 函数与作用域         16 个任务 × 8 语言 =  128
来源：http://www.52xcode.cn/Article/details/gt3uecebyfs.html

D 数组 / 列表 / 集合   26 个任务 × 8 语言 =  208
来源：http://www.52xcode.cn/Article/details/gt3ytvhqlij.html

E 字符串处理           22 个任务 × 8 语言 =  176
来源：http://www.52xcode.cn/Article/details/gt3oziczbjb.html

F 文件与目录           12 个任务 × 8 语言 =   96
来源：http://www.52xcode.cn/Article/details/gt3lwdpillg.html

G 面向对象             16 个任务 × 8 语言 =  128
来源：http://www.ydjk.org.cn/Article/details/gt3abmknkwg.html

H 异常与错误处理       10 个任务 × 8 语言 =   80
来源：http://www.52xcode.cn/Article/details/gt3onjrpkqk.html

I 正则表达式            8 个任务 × 8 语言 =   64
来源：http://www.52xcode.cn/Article/details/gt3nhglyuja.html

J 日期与时间           10 个任务 × 8 语言 =   80
来源：http://www.ydjk.org.cn/Article/details/gt3azrovwnb.html

K JSON 与序列化         8 个任务 × 8 语言 =   64
来源：http://www.52xcode.cn/Article/details/gt3zeiafvwh.html

L 网络请求              8 个任务 × 8 语言 =   64
来源：http://www.52xcode.cn/Article/details/gt3kaqajraj.html

M 命令行 / 进程         8 个任务 × 8 语言 =   64
来源：http://www.ydjk.org.cn/Article/details/gt3zirwjdlr.html

N 数据结构与算法       12 个任务 × 8 语言 =   96
来源：http://www.ydjk.org.cn/Article/details/gt3htrbsrjk.html

O 并发与异步            6 个任务 × 8 语言 =   48
来源：http://www.ydjk.org.cn/Article/details/gt3lwoqdqdz.html

P 常用工具函数          8 个任务 × 8 语言 =   64
来源：http://www.52xcode.cn/Article/details/gt3jehknwpk.html

Q SQL 专题                              90
来源：http://www.52xcode.cn/Article/details/gt3sfidhhlr.html

R Bash 专题                             80
来源：http://www.52xcode.cn/Article/details/gt3iovioezi.html

S C / C++ 专题                          60
来源：http://www.52xcode.cn/Article/details/gt3vsexgkye.html

T 其他语言补充                          60
来源：http://www.52xcode.cn/Article/details/gt3jekesbew.html

U 高频实用片段                         120
来源：http://www.52xcode.cn/Article/details/gt3nktlntib.html

------------------------------------
来源：http://www.52xcode.cn/Article/details/gt3mqkxfiao.html

合计                                  2106 条
来源：http://www.ydjk.org.cn/Article/details/gt3lsfkvkqi.html

--------------------------------------------------------------------------------
来源：http://www.ydjk.org.cn/Article/details/gt3emohighb.html

使用提醒
来源：http://www.52xcode.cn/Article/details/gt3quafxqii.html

--------------------------------------------------------------------------------
来源：http://www.ydjk.org.cn/Article/details/gt3xhsfkqxj.html

1. 示例追求"最小可用"，正式项目中请补齐导入、错误处理与边界判断。
来源：http://www.ydjk.org.cn/Article/details/gt3vrkdaoqv.html

2. 涉及文件、网络、数据库的示例，注意资源释放与异常捕获。
来源：http://www.52xcode.cn/Article/details/gt3gmjfdjyk.html

3. 语言版本差异较大（如 Python 3.10 的 match、Java 17 的 record/switch 箭头），
来源：http://www.52xcode.cn/Article/details/gt3njdvprtl.html

在旧版本上使用前请先确认语法支持情况。
来源：http://www.ydjk.org.cn/Article/details/gt3xsnniewk.html

4. 标注"手写"的条目是因为该语言缺少对应内置能力，实际项目中可引入成熟库。
来源：http://www.52xcode.cn/Article/details/gt3vqsvsjlw.html

—— 文件结束 ——
来源：http://www.52xcode.cn/Article/details/gt3bbqfjlrr.html

================================================================================
来源：http://www.ydjk.org.cn/Article/details/gt3wzbsdizq.html

程序语言常见例子速查手册（2024 版）
来源：http://www.52xcode.cn/Article/details/gt3vvmbpdev.html

Common Programming Examples Cheat Book
来源：http://www.52xcode.cn/Article/details/gt3cugyoayv.html

================================================================================
来源：http://www.52xcode.cn/Article/details/gt3zduhswzb.html

【收录内容】
来源：http://www.52xcode.cn/Article/details/gt3aqhrdaiq.html

覆盖 12 种语言 / 语法与常见 API：
来源：http://www.52xcode.cn/Article/details/gt3kscqnbyv.html

Python · PHP · JavaScript · TypeScript · Java · Go · Ruby · C#
来源：http://www.ydjk.org.cn/Article/details/gt3ujyukjrt.html

SQL · Bash · C · C++
来源：http://www.ydjk.org.cn/Article/details/gt3xmixlbvi.html

按「任务」分组：每个任务下按语言各给出一条最小可用示例。
来源：http://www.52xcode.cn/Article/details/gt3vhpdfrqr.html

【使用说明】
来源：http://www.52xcode.cn/Article/details/gt3cfrwuycy.html

1. 每个任务形如 "[编号] 任务名"，下面每行以语言标记开头：
来源：http://www.ydjk.org.cn/Article/details/gt3chiecoop.html

Py:    Python        PHP:   PHP           JS:    JavaScript
来源：http://www.52xcode.cn/Article/details/gt3tujkvmjt.html

TS:    TypeScript    Java:  Java          Go:    Go
来源：http://www.52xcode.cn/Article/details/gt3kvjvdhvd.html

Ruby:  Ruby          C#:    C#            SQL:   SQL
来源：http://www.52xcode.cn/Article/details/gt3mpggxppw.html

Bash:  Shell         C:     C             C++:   C++
来源：http://www.52xcode.cn/Article/details/gt3gpjlodmt.html

2. 示例只展示核心写法，刻意省略 import / require / include / using 等样板代码。
来源：http://www.52xcode.cn/Article/details/gt3bncjwsmn.html

需要完整可运行文件时，请自行补齐当前语言的导入语句。
来源：http://www.52xcode.cn/Article/details/gt3nvyqxnec.html

3. 语法基准：Python 3.10+ / PHP 8.1+ / ES2020+ / TypeScript 5 / Java 17 /
来源：http://www.ydjk.org.cn/Article/details/gt3cowwnfff.html

Go 1.21+ / Ruby 3.x / C# 10+ / C17 / C++17。
来源：http://www.ydjk.org.cn/Article/details/gt3afwbianq.html

4. 检索建议：用编辑器或浏览器 Ctrl+F 搜关键词，如 "排序" "读取文件" "正则"。
来源：http://www.ydjk.org.cn/Article/details/gt3rdskuvbx.html

5. 标记为 "// 无" 表示该语言没有对应的一等语法，需用替代写法（示例给出替代方案）。
来源：http://www.ydjk.org.cn/Article/details/gt3dmbdnuer.html

6. 符号 "⏎" 表示代码在此处换行（主要用于 Python 等强制缩进、无法压成一行的结构）。
来源：http://www.52xcode.cn/Article/details/gt3wvxbpvgh.html

【文件统计】
来源：http://www.ydjk.org.cn/Article/details/gt3yczqynjp.html

语言示例共 2106 条，分布见本文末尾的「统计汇总」。
来源：http://www.52xcode.cn/Article/details/gt3zykkhlti.html

--------------------------------------------------------------------------------
来源：http://www.ydjk.org.cn/Article/details/gt3ogtacsno.html

目  录
来源：http://www.ydjk.org.cn/Article/details/gt3icxjnriv.html

--------------------------------------------------------------------------------
来源：http://www.ydjk.org.cn/Article/details/gt3dgeiezlm.html

A. 基础语法与类型              （第 1 节，26 个任务，208 条）
来源：http://www.52xcode.cn/Article/details/gt3nqnbmtim.html

B. 流程控制                    （第 2 节，16 个任务，128 条）
来源：http://www.ydjk.org.cn/Article/details/gt3oayjilxp.html

C. 函数与作用域                （第 3 节，16 个任务，128 条）
来源：http://www.52xcode.cn/Article/details/gt3ieqoeaut.html

D. 数组 / 列表 / 集合          （第 4 节，26 个任务，208 条）
来源：http://www.52xcode.cn/Article/details/gt3betgahwu.html

E. 字符串处理                  （第 5 节，22 个任务，176 条）
来源：http://www.ydjk.org.cn/Article/details/gt3fkvondrh.html

F. 文件与目录                  （第 6 节，12 个任务，96 条）
来源：http://www.ydjk.org.cn/Article/details/gt3mazdgjwv.html

G. 面向对象                    （第 7 节，16 个任务，128 条）
来源：http://www.52xcode.cn/Article/details/gt3aohvljdx.html

H. 异常与错误处理              （第 8 节，10 个任务，80 条）
来源：http://www.ydjk.org.cn/Article/details/gt3qulsgyfg.html

I. 正则表达式                  （第 9 节，8 个任务，64 条）
来源：http://www.52xcode.cn/Article/details/gt3ebijjhwg.html

J. 日期与时间                  （第 10 节，10 个任务，80 条）
来源：http://www.52xcode.cn/Article/details/gt3jlxlkuap.html

K. JSON 与序列化               （第 11 节，8 个任务，64 条）
来源：http://www.ydjk.org.cn/Article/details/gt3xpxlozoa.html

L. 网络请求                    （第 12 节，8 个任务，64 条）
来源：http://www.52xcode.cn/Article/details/gt3snoquciq.html

M. 命令行 / 进程 / 环境        （第 13 节，8 个任务，64 条）
来源：http://www.52xcode.cn/Article/details/gt3mxnoqceq.html

N. 数据结构与算法              （第 14 节，12 个任务，96 条）
来源：http://www.52xcode.cn/Article/details/gt3bwmjowey.html

O. 并发与异步                  （第 15 节，6 个任务，48 条）
来源：http://www.52xcode.cn/Article/details/gt3bedyprlk.html

P. 常用工具函数                （第 16 节，8 个任务，64 条）
来源：http://www.52xcode.cn/Article/details/gt3eotoqwsz.html

Q. SQL 专题                    （第 17 节，90 条）
来源：http://www.52xcode.cn/Article/details/gt3ejfmutdv.html

R. Bash 专题                   （第 18 节，80 条）
来源：http://www.ydjk.org.cn/Article/details/gt3zxyslcxg.html

S. C / C++ 专题                （第 19 节，60 条）
来源：http://www.52xcode.cn/Article/details/gt3wivppvdp.html

T. 其他语言补充                （第 20 节，60 条：Kotlin / Swift / Lua / Perl / Scala）
来源：http://www.ydjk.org.cn/Article/details/gt3kcxqfeot.html

U. 高频实用片段                （第 21 节，120 条：Python / PHP / JavaScript 各 40 条）
来源：http://www.52xcode.cn/Article/details/gt3oljmmoif.html

================================================================================
来源：http://www.ydjk.org.cn/Article/details/gt3ttxjrdcp.html

A. 基础语法与类型
来源：http://www.ydjk.org.cn/Article/details/gt3gmymgnqu.html

================================================================================
来源：http://www.ydjk.org.cn/Article/details/gt3vbvdktls.html

[A01] Hello World
来源：http://www.52xcode.cn/Article/details/gt3imyggmch.html

Py:   print("Hello, World!")
来源：http://www.52xcode.cn/Article/details/gt3iepprfmp.html

PHP:  echo "Hello, World!";
来源：http://www.52xcode.cn/Article/details/gt3dgibosdi.html

JS:   console.log("Hello, World!");
来源：http://www.52xcode.cn/Article/details/gt3pblwkymo.html

TS:   const msg: string = "Hello, World!"; console.log(msg);
来源：http://www.52xcode.cn/Article/details/gt3nacnpllx.html

Java: System.out.println("Hello, World!");
来源：http://www.ydjk.org.cn/Article/details/gt3uzznbxrt.html

Go:   fmt.Println("Hello, World!")
来源：http://www.ydjk.org.cn/Article/details/gt3krgfzkce.html

Ruby: puts "Hello, World!"
来源：http://www.52xcode.cn/Article/details/gt3jigoszkz.html

C#:   Console.WriteLine("Hello, World!");
来源：http://www.52xcode.cn/Article/details/gt3gypfptst.html

[A02] 变量声明与赋值
来源：http://www.52xcode.cn/Article/details/gt3slznnhmp.html

Py:   name = "Alex"; age = 20            # 动态类型，无需声明
来源：http://www.52xcode.cn/Article/details/gt3dfsocxoq.html

PHP:  $name = "Alex"; $age = 20;
来源：http://www.52xcode.cn/Article/details/gt3qxwvbydf.html

JS:   let name = "Alex"; const age = 20;
来源：http://www.52xcode.cn/Article/details/gt3vdikvpmm.html


<!-- 参考信息 -->