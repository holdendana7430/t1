代发 wailian999

[U39] Py：判断是否在交互环境
来源：http://blog.zdbjq.cn/Article/details/gocfmnxug.sHtML

sys.stdout.isatty()
来源：http://3g.zdbjq.cn/Article/details/ggxzsdfrm.sHtML

[U40] Py：打印到标准错误
来源：http://read.share.hesvh.cn/Article/details/gcmrvaafr.sHtML

print("err", file=sys.stderr)
来源：http://blog.hesvh.cn/Article/details/gxlslfxok.sHtML

[U41] PHP：初始化 Composer 项目
来源：http://3g.fehbvm.com/Article/details/gfvtculns.sHtML

composer init;  composer require guzzlehttp/guzzle
来源：http://www.share.fehbvm.com/Article/details/gthlfcdhv.sHtML

[U42] PHP：PSR-4 自动加载
来源：http://wap.fehbvm.com/Article/details/ggbxltaye.sHtML

"autoload": { "psr-4": { "App\\": "src/" } }
来源：http://www.m.share.zdbjq.cn/Article/details/gybzgyblk.sHtML

[U43] PHP：声明命名空间
来源：http://www.m.share.zdbjq.cn/Article/details/grbvgnald.sHtML

namespace App\Http;
来源：http://mobile.zdbjq.cn/Article/details/gjkiqeusz.sHtML

[U44] PHP：开启严格类型
来源：http://m.share.zdbjq.cn/Article/details/gpuqtnidl.sHtML

declare(strict_types=1);
来源：http://mobile.hesvh.cn/Article/details/ghssfsofi.sHtML

[U45] PHP：类型声明与返回类型
来源：http://m.share.zdbjq.cn/Article/details/gibfsudqx.sHtML

function add(int $a, int $b): int { return $a + $b; }
来源：http://mobile.zdbjq.cn/Article/details/gblrrmefp.sHtML

[U46] PHP：可空类型
来源：http://baike.fehbvm.com/Article/details/glsaeulty.sHtML

?string $name = null
来源：http://m.share.fehbvm.com/Article/details/glizdfnsn.sHtML

[U47] PHP：联合类型
来源：http://wap.zdbjq.cn/Article/details/gndwhxpjx.sHtML

int|string $id
来源：http://wap.hesvh.cn/Article/details/gekrjswgy.sHtML

[U48] PHP：纯枚举
来源：http://wap.zdbjq.cn/Article/details/gtysruddx.sHtML

enum Status: string { case Active = "active"; case Off = "off"; }
来源：http://www.share.hesvh.cn/Article/details/givsrjqvk.sHtML

[U49] PHP：只读属性
来源：http://mobile.fehbvm.com/Article/details/gyffpkcyx.sHtML

public readonly string $name
来源：http://www.share.fehbvm.com/Article/details/gagowuyqd.sHtML

[U50] PHP：构造器属性提升
来源：http://read.share.zdbjq.cn/Article/details/gftchsyud.sHtML

public function __construct(private int $id) {}
来源：http://baike.fehbvm.com/Article/details/ghcadvqib.sHtML

[U51] PHP：数组解构
来源：http://www.m.share.fehbvm.com/Article/details/glyfoidcr.sHtML

[$a, $b] = $arr;
来源：http://www.share.zdbjq.cn/Article/details/gihlyujpj.sHtML

[U52] PHP：箭头函数
来源：http://read.share.zdbjq.cn/Article/details/ggvsfrzli.sHtML

$double = fn($x) => $x * 2;
来源：http://www.share.zdbjq.cn/Article/details/gtkgfjpii.sHtML

[U53] PHP：空合并运算符
来源：http://blog.hesvh.cn/Article/details/gmyviejxc.sHtML

$v = $a ?? $b ?? "default";
来源：http://baike.hesvh.cn/Article/details/gzsaaliiz.sHtML

[U54] PHP：空安全调用
来源：http://read.share.hesvh.cn/Article/details/gjtpfzhin.sHtML

$obj?->method()
来源：http://m.share.hesvh.cn/Article/details/gjokeiogg.sHtML

[U55] PHP：match 表达式
来源：http://www.blog.hesvh.cn/Article/details/gandlbava.sHtML

$s = match($x) { 1 => "一", default => "其他" };
来源：http://wap.hesvh.cn/Article/details/giugsoxmx.sHtML

[U56] PHP：命名参数
来源：http://www.m.share.zdbjq.cn/Article/details/gmzlktprk.sHtML

f(a: 1, b: 2)
来源：http://blog.hesvh.cn/Article/details/gtelvreep.sHtML

[U57] PHP：字符串插值
来源：http://www.share.zdbjq.cn/Article/details/gfxzexmaf.sHtML

"值: {$a}"
来源：http://www.share.zdbjq.cn/Article/details/gcyuokqla.sHtML

[U58] PHP：数组三件套
来源：http://wap.hesvh.cn/Article/details/gxsnwwiwo.sHtML

array_map($f, $a);  array_filter($a, $f);  array_reduce($a, $f, 0);
来源：http://m.share.zdbjq.cn/Article/details/gxncmsbhu.sHtML

[U59] PHP：自定义排序
来源：http://blog.hesvh.cn/Article/details/gkuojvlxt.sHtML

usort($arr, fn($a, $b) => $a["age"] <=> $b["age"]);
来源：http://m.share.fehbvm.com/Article/details/gqsinrrjx.sHtML

[U60] PHP：JSON 编解码
来源：http://m.share.hesvh.cn/Article/details/gmpluagku.sHtML

json_encode($d, JSON_UNESCAPED_UNICODE);  json_decode($s, true);
来源：http://www.share.hesvh.cn/Article/details/gcyxnwgms.sHtML

[U61] PHP：正则
来源：http://baike.hesvh.cn/Article/details/gpwbrynbp.sHtML

preg_match('/(\d+)/', $s, $m);  preg_replace('/\d+/', '#', $s);
来源：http://3g.hesvh.cn/Article/details/glsxyzgii.sHtML

[U62] PHP：日期对象
来源：http://mobile.hesvh.cn/Article/details/gcquhjyye.sHtML

(new DateTimeImmutable())->format("Y-m-d");
来源：http://www.m.share.zdbjq.cn/Article/details/gujlkpawt.sHtML

[U63] PHP：文件读写
来源：http://wap.zdbjq.cn/Article/details/gvpwceagd.sHtML

file_get_contents($f);  file_put_contents($f, $data);
来源：http://3g.fehbvm.com/Article/details/gqewwwiaf.sHtML

[U64] PHP：目录遍历
来源：http://www.share.hesvh.cn/Article/details/gvtefpwuv.sHtML

glob("dir/*.php");  scandir("dir");
来源：http://mobile.zdbjq.cn/Article/details/gseiqbyjg.sHtML

[U65] PHP：会话
来源：http://3g.fehbvm.com/Article/details/gsoltcjyd.sHtML

session_start();  $_SESSION["uid"] = 1;
来源：http://read.share.hesvh.cn/Article/details/gyqujszar.sHtML

[U66] PHP：设置 Cookie
来源：http://m.share.zdbjq.cn/Article/details/gcluykewr.sHtML

setcookie("token", $v, ["httponly" => true, "samesite" => "Lax"]);
来源：http://blog.fehbvm.com/Article/details/gnhuuupqi.sHtML

[U67] PHP：处理文件上传
来源：http://www.blog.hesvh.cn/Article/details/glpiwcngm.sHtML

$_FILES["file"]["tmp_name"] 与 move_uploaded_file()
来源：http://blog.zdbjq.cn/Article/details/gwajjdxat.sHtML

[U68] PHP：PDO 连接
来源：http://blog.fehbvm.com/Article/details/glmizrkfj.sHtML

$pdo = new PDO("mysql:host=localhost;dbname=app", "root", "");
来源：http://www.share.fehbvm.com/Article/details/gvalsyqyo.sHtML

[U69] PHP：PDO 预处理
来源：http://www.share.fehbvm.com/Article/details/gevvxhkgb.sHtML

$stmt = $pdo->prepare("SELECT * FROM users WHERE id = ?");  $stmt->execute([$id]);
来源：http://baike.zdbjq.cn/Article/details/gmuhgddrb.sHtML

[U70] PHP：PDO 事务
来源：http://read.share.hesvh.cn/Article/details/glfccsjbn.sHtML

$pdo->beginTransaction();  $pdo->commit();  $pdo->rollBack();
来源：http://www.blog.zdbjq.cn/Article/details/gpytcpbzd.sHtML

[U71] PHP：抛出异常
来源：http://www.blog.fehbvm.com/Article/details/gmzknqdib.sHtML

throw new RuntimeException("失败", 500);
来源：http://blog.hesvh.cn/Article/details/gsviihedp.sHtML

[U72] PHP：写错误日志
来源：http://baike.fehbvm.com/Article/details/geooowpwn.sHtML

error_log("失败: " . $e->getMessage());
来源：http://read.share.fehbvm.com/Article/details/gjfrgdtgc.sHtML

[U73] PHP：读取 ini 配置
来源：http://read.share.fehbvm.com/Article/details/gmmztxstz.sHtML

parse_ini_file("config.ini", true)
来源：http://www.m.share.fehbvm.com/Article/details/gjwwvixka.sHtML

[U74] PHP：读取环境变量
来源：http://blog.fehbvm.com/Article/details/gyvbvoqlo.sHtML

getenv("APP_ENV") ?: "production"
来源：http://mobile.hesvh.cn/Article/details/gxvhesoti.sHtML

[U75] PHP：依赖注入
来源：http://mobile.hesvh.cn/Article/details/gmtlzxgfw.sHtML

composer require psr/container
来源：http://read.share.hesvh.cn/Article/details/gzssjdtvi.sHtML

[U76] PHP：简单路由
来源：http://read.share.hesvh.cn/Article/details/ggpjshuht.sHtML

$path = parse_url($_SERVER["REQUEST_URI"], PHP_URL_PATH);
来源：http://m.share.fehbvm.com/Article/details/gqoarceja.sHtML

[U77] PHP：模板渲染
来源：http://blog.hesvh.cn/Article/details/grqgcopew.sHtML

composer require twig/twig
来源：http://read.share.hesvh.cn/Article/details/gngjkzkmh.sHtML

[U78] PHP：单元测试
来源：http://www.blog.hesvh.cn/Article/details/gdyeontit.sHtML

composer require --dev phpunit/phpunit
来源：http://3g.hesvh.cn/Article/details/gxztmzrfe.sHtML

[U79] PHP：静态分析
来源：http://www.blog.zdbjq.cn/Article/details/gkfmaqmfz.sHtML

composer require --dev phpstan/phpstan
来源：http://mobile.hesvh.cn/Article/details/gtuiejohr.sHtML

[U80] PHP：代码规范修复
来源：http://www.blog.zdbjq.cn/Article/details/gmlyyuzbh.sHtML

composer require --dev friendsofphp/php-cs-fixer
来源：http://www.m.share.fehbvm.com/Article/details/ggscndnai.sHtML

[U81] JS：初始化项目
来源：http://baike.hesvh.cn/Article/details/gpmuqzbjj.sHtML

npm init -y;  npm i express
来源：http://read.share.hesvh.cn/Article/details/gsbybmhgp.sHtML

[U82] JS：package.json 脚本
来源：http://m.share.hesvh.cn/Article/details/gqppvudqf.sHtML

"scripts": { "dev": "vite", "build": "vite build" }
来源：http://www.share.zdbjq.cn/Article/details/gizipeoxu.sHtML

[U83] JS：ES Module 导入导出
来源：http://blog.zdbjq.cn/Article/details/gmpghpimk.sHtML

export const a = 1;  import { a } from "./m.js";
来源：http://wap.fehbvm.com/Article/details/gkmixpgqy.sHtML

[U84] JS：CommonJS 写法
来源：http://www.m.share.zdbjq.cn/Article/details/ghcbtcooz.sHtML

module.exports = { a };  const { a } = require("./m");
来源：http://mobile.zdbjq.cn/Article/details/gouxrustl.sHtML

[U85] JS：可选链
来源：http://www.blog.hesvh.cn/Article/details/gheyztowr.sHtML

a?.b?.c
来源：http://www.blog.hesvh.cn/Article/details/garcxfncs.sHtML

[U86] JS：空值合并
来源：http://m.share.fehbvm.com/Article/details/glykrjmow.sHtML

a ?? b
来源：http://blog.hesvh.cn/Article/details/gfjptqimq.sHtML

[U87] JS：解构默认值
来源：http://www.blog.fehbvm.com/Article/details/gaevunbhy.sHtML

const { a = 1, b = 2 } = obj;
来源：http://mobile.hesvh.cn/Article/details/gstulqphx.sHtML

[U88] JS：对象展开合并
来源：http://mobile.hesvh.cn/Article/details/gilkpyzzq.sHtML

{ ...a, ...b }
来源：http://baike.hesvh.cn/Article/details/ggcxihloz.sHtML

[U89] JS：数组去重
来源：http://www.share.fehbvm.com/Article/details/gcogfbdzs.sHtML

[...new Set(arr)]
来源：http://www.share.fehbvm.com/Article/details/gevvotcco.sHtML

[U90] JS：数字数组排序
来源：http://www.share.zdbjq.cn/Article/details/gibnzxffi.sHtML

[...arr].sort((a, b) => a - b)
来源：http://blog.hesvh.cn/Article/details/gclcsiiea.sHtML

[U91] JS：对象键值遍历
来源：http://m.share.zdbjq.cn/Article/details/giyhltibh.sHtML

Object.entries(obj).forEach(([k, v]) => {});
来源：http://blog.zdbjq.cn/Article/details/gpbetryam.sHtML

[U92] JS：深拷贝
来源：http://baike.hesvh.cn/Article/details/gaiumqcxx.sHtML

structuredClone(obj)
来源：http://3g.hesvh.cn/Article/details/gywdbniuq.sHtML

[U93] JS：模板字符串
来源：http://baike.hesvh.cn/Article/details/gfptjripe.sHtML

`共 ${n} 条`
来源：http://baike.fehbvm.com/Article/details/gamfcytji.sHtML

[U94] JS：箭头函数
来源：http://3g.fehbvm.com/Article/details/gkaiidqzf.sHtML

const double = x => x * 2;
来源：http://www.blog.fehbvm.com/Article/details/gnhsomxjg.sHtML

[U95] JS：Promise 包装
来源：http://mobile.fehbvm.com/Article/details/gnygsugdw.sHtML

new Promise((resolve, reject) => {})
来源：http://www.blog.hesvh.cn/Article/details/gzkcpfdof.sHtML

[U96] JS：async/await 与异常
来源：http://m.share.hesvh.cn/Article/details/gpdazyali.sHtML

try { const d = await f(); } catch (e) { console.error(e); }
来源：http://m.share.hesvh.cn/Article/details/gohwxvozg.sHtML

[U97] JS：并发请求
来源：http://mobile.hesvh.cn/Article/details/gcbqllpvg.sHtML

await Promise.all(urls.map(u => fetch(u)))
来源：http://mobile.fehbvm.com/Article/details/gtowzkwli.sHtML

[U98] JS：fetch 带 JSON
来源：http://wap.zdbjq.cn/Article/details/gmmtkwwjc.sHtML

await fetch(url, { method: "POST", headers: { "Content-Type": "application/json" }, body: JSON.stringify(d) })
来源：http://3g.fehbvm.com/Article/details/gvdwufviu.sHtML

[U99] JS：事件监听
来源：http://wap.fehbvm.com/Article/details/gaxrhbpbz.sHtML

el.addEventListener("click", e => {})
来源：http://3g.fehbvm.com/Article/details/gkfezrcog.sHtML

[U100] JS：DOM 查询
来源：http://mobile.hesvh.cn/Article/details/gdhjgvczf.sHtML

document.querySelector(".item")
来源：http://baike.hesvh.cn/Article/details/gnkmmwglj.sHtML

[U101] JS：classList 操作
来源：http://www.blog.fehbvm.com/Article/details/guklbwtir.sHtML

el.classList.toggle("active")
来源：http://www.blog.hesvh.cn/Article/details/gjotzvrex.sHtML

[U102] JS：本地存储
来源：http://m.share.zdbjq.cn/Article/details/gczyhcdkc.sHtML

localStorage.setItem("k", JSON.stringify(v))
来源：http://blog.hesvh.cn/Article/details/gdtwlmtdz.sHtML

[U103] JS：定时器
来源：http://read.share.fehbvm.com/Article/details/gwwroucyg.sHtML

setTimeout(fn, 1000);  setInterval(fn, 1000);
来源：http://read.share.zdbjq.cn/Article/details/gubrzqtzj.sHtML

[U104] JS：防抖
来源：http://mobile.fehbvm.com/Article/details/gnulzfvvj.sHtML

const debounce = (fn, ms) => { let t; return (...a) => { clearTimeout(t); t = setTimeout(() => fn(...a), ms); }; };
来源：http://www.blog.fehbvm.com/Article/details/gtcexfszy.sHtML

[U105] JS：节流
来源：http://read.share.zdbjq.cn/Article/details/gbqzuyzuf.sHtML

const throttle = (fn, ms) => { let last = 0; return (...a) => { const n = Date.now(); if (n - last >= ms) { last = n; fn(...a); } }; };
来源：http://m.share.hesvh.cn/Article/details/glfntelws.sHtML

[U106] JS：日期格式化
来源：http://read.share.hesvh.cn/Article/details/gxaqfehzg.sHtML

new Intl.DateTimeFormat("zh-CN", { dateStyle: "medium" }).format(new Date())
来源：http://3g.fehbvm.com/Article/details/gbxsqtemb.sHtML

[U107] JS：数字千分位
来源：http://m.share.fehbvm.com/Article/details/gnmqfdrlc.sHtML

new Intl.NumberFormat("en-US").format(1234567)
来源：http://mobile.fehbvm.com/Article/details/gvbcimkso.sHtML

[U108] JS：随机整数
来源：http://mobile.hesvh.cn/Article/details/glwcwcltz.sHtML

Math.floor(Math.random() * (max - min + 1)) + min
来源：http://read.share.zdbjq.cn/Article/details/ghvcldfyk.sHtML

[U109] JS：数组分组
来源：http://www.m.share.fehbvm.com/Article/details/gdbnwzbch.sHtML

Object.groupBy(arr, x => x.type)
来源：http://m.share.hesvh.cn/Article/details/gjfblpodk.sHtML

[U110] JS：数组分块
来源：http://read.share.fehbvm.com/Article/details/gjmxbcerz.sHtML

arr.reduce((acc, x, i) => (i % size ? acc : [...acc, arr.slice(i, i + size)]), [])
来源：http://read.share.zdbjq.cn/Article/details/gmvhljnaz.sHtML

[U111] JS：对象转 Map
来源：http://www.m.share.fehbvm.com/Article/details/gdbkssaju.sHtML

new Map(Object.entries(obj))
来源：http://m.share.zdbjq.cn/Article/details/gxehfwbam.sHtML

[U112] JS：字符串补位
来源：http://3g.fehbvm.com/Article/details/ggnlmxbmr.sHtML

"7".padStart(3, "0")
来源：http://3g.fehbvm.com/Article/details/goithsmtd.sHtML

[U113] JS：正则替换全部
来源：http://wap.hesvh.cn/Article/details/glwtdlumh.sHtML

s.replaceAll("a", "b")
来源：http://www.blog.hesvh.cn/Article/details/gntyuswjd.sHtML

[U114] JS：JSON 深比较
来源：http://baike.hesvh.cn/Article/details/ggituqdki.sHtML

JSON.stringify(a) === JSON.stringify(b)
来源：http://www.blog.fehbvm.com/Article/details/gyplfxjov.sHtML

[U115] JS：生成 UUID
来源：http://mobile.fehbvm.com/Article/details/gbjqprkqv.sHtML

crypto.randomUUID()
来源：http://mobile.fehbvm.com/Article/details/gfrkswxwa.sHtML

[U116] JS：类型检查（JSDoc）
来源：http://3g.hesvh.cn/Article/details/grrccsfne.sHtML

/** @param {string} name */ function f(name) {}
来源：http://www.m.share.fehbvm.com/Article/details/gtcftkkte.sHtML

[U117] JS：单元测试
来源：http://www.m.share.fehbvm.com/Article/details/gvuhvpgbu.sHtML

npm i -D vitest;  npx vitest
来源：http://blog.fehbvm.com/Article/details/gmdejfzbx.sHtML

[U118] JS：开发服务器
来源：http://www.blog.zdbjq.cn/Article/details/gjglbkgps.sHtML

npm i -D vite;  npx vite
来源：http://mobile.fehbvm.com/Article/details/gojyzgnwz.sHtML

[U119] JS：生产构建
来源：http://m.share.hesvh.cn/Article/details/ggvvvbtyy.sHtML

npx vite build
来源：http://www.share.hesvh.cn/Article/details/glnzwxmpy.sHtML

[U120] JS：读取环境变量（Vite）
来源：http://mobile.zdbjq.cn/Article/details/gamyacizz.sHtML

import.meta.env.VITE_API_URL
来源：http://m.share.hesvh.cn/Article/details/gdrpohuzz.sHtML

================================================================================
来源：http://wap.fehbvm.com/Article/details/gemtyhlev.sHtML

统计汇总
来源：http://mobile.hesvh.cn/Article/details/gbrymroyp.sHtML

================================================================================
来源：http://m.share.fehbvm.com/Article/details/gqyekmatm.sHtML

按语言统计（条）：
来源：http://www.m.share.hesvh.cn/Article/details/gvphqtqnk.sHtML

Python ......... 252
来源：http://3g.zdbjq.cn/Article/details/gcqgznjve.sHtML

PHP ............ 252
来源：http://www.blog.hesvh.cn/Article/details/gxlibpmlc.sHtML

JavaScript ..... 252
来源：http://mobile.fehbvm.com/Article/details/gcpbxuxty.sHtML

TypeScript ..... 212
来源：http://read.share.fehbvm.com/Article/details/ggxrvqoax.sHtML

Java ........... 212
来源：http://mobile.zdbjq.cn/Article/details/gkhandjpo.sHtML

Go ............. 212
来源：http://www.share.zdbjq.cn/Article/details/gfjkxaaco.sHtML

Ruby ........... 212
来源：http://www.share.hesvh.cn/Article/details/gozkygpjn.sHtML

C# ............. 212
来源：http://blog.fehbvm.com/Article/details/gwdbtnens.sHtML

C .............. 30
来源：http://www.m.share.hesvh.cn/Article/details/glbhapppi.sHtML

C++ ............ 30
来源：http://3g.hesvh.cn/Article/details/gwilgosce.sHtML

SQL ............ 90
来源：http://wap.hesvh.cn/Article/details/gtokymmwi.sHtML

Bash ........... 80
来源：http://3g.hesvh.cn/Article/details/gkrysvvgr.sHtML

Kotlin ......... 15
来源：http://3g.hesvh.cn/Article/details/gwehhyqbe.sHtML

Swift .......... 15
来源：http://m.share.zdbjq.cn/Article/details/gvfuqhzde.sHtML

Lua ............ 10
来源：http://read.share.fehbvm.com/Article/details/ghygkpebv.sHtML

Perl ........... 10
来源：http://read.share.fehbvm.com/Article/details/gmvqjgiel.sHtML

Scala .......... 10
来源：http://mobile.fehbvm.com/Article/details/gelsrfipj.sHtML

------------------------------------
来源：http://baike.zdbjq.cn/Article/details/ggtzyevwp.sHtML

合计 ........... 2106 条
来源：http://baike.zdbjq.cn/Article/details/gejetgpqy.sHtML

按章节统计：
来源：http://mobile.zdbjq.cn/Article/details/gmmgwihgo.sHtML

A 基础语法与类型       26 个任务 × 8 语言 =  208
来源：http://baike.zdbjq.cn/Article/details/gdmfaozmt.sHtML

B 流程控制             16 个任务 × 8 语言 =  128
来源：http://3g.fehbvm.com/Article/details/gkdiiwgid.sHtML

C 函数与作用域         16 个任务 × 8 语言 =  128
来源：http://www.blog.hesvh.cn/Article/details/gsjealfds.sHtML

D 数组 / 列表 / 集合   26 个任务 × 8 语言 =  208
来源：http://www.m.share.hesvh.cn/Article/details/gcbuzewea.sHtML

E 字符串处理           22 个任务 × 8 语言 =  176
来源：http://3g.zdbjq.cn/Article/details/gpaebsqxv.sHtML

F 文件与目录           12 个任务 × 8 语言 =   96
来源：http://m.share.fehbvm.com/Article/details/gzwkfwzpd.sHtML

G 面向对象             16 个任务 × 8 语言 =  128
来源：http://read.share.hesvh.cn/Article/details/gvdurkeap.sHtML

H 异常与错误处理       10 个任务 × 8 语言 =   80
来源：http://www.share.zdbjq.cn/Article/details/gyhlwdesq.sHtML

I 正则表达式            8 个任务 × 8 语言 =   64
来源：http://mobile.fehbvm.com/Article/details/gtlipszqb.sHtML

J 日期与时间           10 个任务 × 8 语言 =   80
来源：http://mobile.fehbvm.com/Article/details/gzkvkcode.sHtML

K JSON 与序列化         8 个任务 × 8 语言 =   64
来源：http://3g.fehbvm.com/Article/details/gaevovssi.sHtML

L 网络请求              8 个任务 × 8 语言 =   64
来源：http://read.share.zdbjq.cn/Article/details/gvralwyvq.sHtML

M 命令行 / 进程         8 个任务 × 8 语言 =   64
来源：http://mobile.fehbvm.com/Article/details/gtqekmlrs.sHtML

N 数据结构与算法       12 个任务 × 8 语言 =   96
来源：http://m.share.hesvh.cn/Article/details/gpmbibqes.sHtML

O 并发与异步            6 个任务 × 8 语言 =   48
来源：http://blog.fehbvm.com/Article/details/gpgvhwanr.sHtML

P 常用工具函数          8 个任务 × 8 语言 =   64
来源：http://m.share.hesvh.cn/Article/details/getienlke.sHtML

Q SQL 专题                              90
来源：http://www.share.fehbvm.com/Article/details/gfiqdvtdh.sHtML

R Bash 专题                             80
来源：http://www.share.fehbvm.com/Article/details/gmjazbfta.sHtML

S C / C++ 专题                          60
来源：http://www.m.share.fehbvm.com/Article/details/gljeqeckv.sHtML

T 其他语言补充                          60
来源：http://blog.fehbvm.com/Article/details/gnpbmgmeo.sHtML

U 高频实用片段                         120
来源：http://mobile.fehbvm.com/Article/details/gapmmrdzd.sHtML

------------------------------------
来源：http://baike.fehbvm.com/Article/details/ggrldsijx.sHtML

合计                                  2106 条
来源：http://blog.zdbjq.cn/Article/details/gjftnlupj.sHtML

--------------------------------------------------------------------------------
来源：http://read.share.hesvh.cn/Article/details/gktljlkfx.sHtML

使用提醒
来源：http://www.m.share.zdbjq.cn/Article/details/gmxvmjbbh.sHtML

--------------------------------------------------------------------------------
来源：http://3g.fehbvm.com/Article/details/gznneyxgf.sHtML

1. 示例追求"最小可用"，正式项目中请补齐导入、错误处理与边界判断。
来源：http://baike.hesvh.cn/Article/details/gofkwjbgi.sHtML

2. 涉及文件、网络、数据库的示例，注意资源释放与异常捕获。
来源：http://read.share.zdbjq.cn/Article/details/gatnsspjp.sHtML

3. 语言版本差异较大（如 Python 3.10 的 match、Java 17 的 record/switch 箭头），
来源：http://www.m.share.hesvh.cn/Article/details/glhnvhata.sHtML

在旧版本上使用前请先确认语法支持情况。
来源：http://wap.hesvh.cn/Article/details/gzctryzyy.sHtML

4. 标注"手写"的条目是因为该语言缺少对应内置能力，实际项目中可引入成熟库。
来源：http://m.share.zdbjq.cn/Article/details/gwcweryye.sHtML

—— 文件结束 ——
来源：http://blog.zdbjq.cn/Article/details/ggcejvaao.sHtML

================================================================================
来源：http://m.share.zdbjq.cn/Article/details/ganckmtol.sHtML

程序语言常见例子速查手册（2024 版）
来源：http://www.share.hesvh.cn/Article/details/gyysjjpbi.sHtML

Common Programming Examples Cheat Book
来源：http://3g.fehbvm.com/Article/details/gspdxodlp.sHtML

================================================================================
来源：http://baike.zdbjq.cn/Article/details/gsjzhphmw.sHtML

【收录内容】
来源：http://www.blog.fehbvm.com/Article/details/gypfdddex.sHtML

覆盖 12 种语言 / 语法与常见 API：
来源：http://3g.fehbvm.com/Article/details/gfbidduoe.sHtML

Python · PHP · JavaScript · TypeScript · Java · Go · Ruby · C#
来源：http://baike.hesvh.cn/Article/details/ghwudopyk.sHtML

SQL · Bash · C · C++
来源：http://m.share.fehbvm.com/Article/details/gwloztxnu.sHtML

按「任务」分组：每个任务下按语言各给出一条最小可用示例。
来源：http://blog.zdbjq.cn/Article/details/gqnzymoog.sHtML

【使用说明】
来源：http://www.share.hesvh.cn/Article/details/gilbhhgmu.sHtML

1. 每个任务形如 "[编号] 任务名"，下面每行以语言标记开头：
来源：http://baike.zdbjq.cn/Article/details/gzaxwmrwp.sHtML

Py:    Python        PHP:   PHP           JS:    JavaScript
来源：http://www.share.zdbjq.cn/Article/details/gbronhcag.sHtML

TS:    TypeScript    Java:  Java          Go:    Go
来源：http://mobile.hesvh.cn/Article/details/gzngkgeze.sHtML

Ruby:  Ruby          C#:    C#            SQL:   SQL
来源：http://baike.fehbvm.com/Article/details/ghtmnpoyk.sHtML

Bash:  Shell         C:     C             C++:   C++
来源：http://blog.zdbjq.cn/Article/details/gdmbssgko.sHtML

2. 示例只展示核心写法，刻意省略 import / require / include / using 等样板代码。
来源：http://mobile.fehbvm.com/Article/details/gngiuqdyu.sHtML

需要完整可运行文件时，请自行补齐当前语言的导入语句。
来源：http://read.share.fehbvm.com/Article/details/gvcquywde.sHtML

3. 语法基准：Python 3.10+ / PHP 8.1+ / ES2020+ / TypeScript 5 / Java 17 /
来源：http://m.share.zdbjq.cn/Article/details/gwujhbesd.sHtML

Go 1.21+ / Ruby 3.x / C# 10+ / C17 / C++17。
来源：http://read.share.zdbjq.cn/Article/details/gallpcwbi.sHtML

4. 检索建议：用编辑器或浏览器 Ctrl+F 搜关键词，如 "排序" "读取文件" "正则"。
来源：http://www.blog.fehbvm.com/Article/details/gunldtduj.sHtML

5. 标记为 "// 无" 表示该语言没有对应的一等语法，需用替代写法（示例给出替代方案）。
来源：http://mobile.zdbjq.cn/Article/details/ggnbjxhbv.sHtML

6. 符号 "⏎" 表示代码在此处换行（主要用于 Python 等强制缩进、无法压成一行的结构）。
来源：http://www.m.share.fehbvm.com/Article/details/grkemidll.sHtML

【文件统计】
来源：http://wap.fehbvm.com/Article/details/ggfiahupo.sHtML

语言示例共 2106 条，分布见本文末尾的「统计汇总」。
来源：http://3g.zdbjq.cn/Article/details/gocmfgaew.sHtML

--------------------------------------------------------------------------------
来源：http://www.m.share.fehbvm.com/Article/details/gqgldygrh.sHtML

目  录
来源：http://wap.hesvh.cn/Article/details/gyzwlmirn.sHtML

--------------------------------------------------------------------------------
来源：http://www.m.share.zdbjq.cn/Article/details/gbeyvwdci.sHtML

A. 基础语法与类型              （第 1 节，26 个任务，208 条）
来源：http://wap.zdbjq.cn/Article/details/gksuhlwlr.sHtML

B. 流程控制                    （第 2 节，16 个任务，128 条）
来源：http://mobile.hesvh.cn/Article/details/gnnsnhblv.sHtML

C. 函数与作用域                （第 3 节，16 个任务，128 条）
来源：http://www.blog.zdbjq.cn/Article/details/gmbuxqdym.sHtML

D. 数组 / 列表 / 集合          （第 4 节，26 个任务，208 条）
来源：http://baike.hesvh.cn/Article/details/ghprbdaqb.sHtML

E. 字符串处理                  （第 5 节，22 个任务，176 条）
来源：http://baike.zdbjq.cn/Article/details/ghulzrijm.sHtML

F. 文件与目录                  （第 6 节，12 个任务，96 条）
来源：http://www.blog.zdbjq.cn/Article/details/gagcomdij.sHtML

G. 面向对象                    （第 7 节，16 个任务，128 条）
来源：http://mobile.fehbvm.com/Article/details/ghxxsyoyc.sHtML

H. 异常与错误处理              （第 8 节，10 个任务，80 条）
来源：http://www.m.share.fehbvm.com/Article/details/gwiissvxg.sHtML

I. 正则表达式                  （第 9 节，8 个任务，64 条）
来源：http://mobile.fehbvm.com/Article/details/gaoarxvkp.sHtML

J. 日期与时间                  （第 10 节，10 个任务，80 条）
来源：http://blog.zdbjq.cn/Article/details/glryefjov.sHtML

K. JSON 与序列化               （第 11 节，8 个任务，64 条）
来源：http://3g.fehbvm.com/Article/details/gkukbzkqp.sHtML

L. 网络请求                    （第 12 节，8 个任务，64 条）
来源：http://www.share.zdbjq.cn/Article/details/glkctwqyf.sHtML

M. 命令行 / 进程 / 环境        （第 13 节，8 个任务，64 条）
来源：http://wap.fehbvm.com/Article/details/ganghkgtb.sHtML

N. 数据结构与算法              （第 14 节，12 个任务，96 条）
来源：http://www.share.fehbvm.com/Article/details/gbgcyanmm.sHtML

O. 并发与异步                  （第 15 节，6 个任务，48 条）
来源：http://mobile.fehbvm.com/Article/details/gpjaqmyfe.sHtML

P. 常用工具函数                （第 16 节，8 个任务，64 条）
来源：http://www.m.share.hesvh.cn/Article/details/ggiklyrsj.sHtML

Q. SQL 专题                    （第 17 节，90 条）
来源：http://blog.fehbvm.com/Article/details/gbfuxdoxj.sHtML

R. Bash 专题                   （第 18 节，80 条）
来源：http://www.m.share.zdbjq.cn/Article/details/gjvxdkrdw.sHtML

S. C / C++ 专题                （第 19 节，60 条）
来源：http://read.share.zdbjq.cn/Article/details/giymqroeq.sHtML

T. 其他语言补充                （第 20 节，60 条：Kotlin / Swift / Lua / Perl / Scala）
来源：http://mobile.zdbjq.cn/Article/details/gaqkfvlyn.sHtML

U. 高频实用片段                （第 21 节，120 条：Python / PHP / JavaScript 各 40 条）
来源：http://www.blog.fehbvm.com/Article/details/gdsczirnt.sHtML

================================================================================
来源：http://read.share.hesvh.cn/Article/details/gnrkbtyml.sHtML

A. 基础语法与类型
来源：http://blog.hesvh.cn/Article/details/goepiabhg.sHtML

================================================================================
来源：http://www.m.share.hesvh.cn/Article/details/gheuadlqf.sHtML

[A01] Hello World
来源：http://mobile.zdbjq.cn/Article/details/grjqmutuq.sHtML

Py:   print("Hello, World!")
来源：http://read.share.fehbvm.com/Article/details/gnpudkfez.sHtML

PHP:  echo "Hello, World!";
来源：http://3g.fehbvm.com/Article/details/gudzteduf.sHtML

JS:   console.log("Hello, World!");
来源：http://blog.zdbjq.cn/Article/details/ggjijhkkx.sHtML

TS:   const msg: string = "Hello, World!"; console.log(msg);
来源：http://blog.zdbjq.cn/Article/details/gnsmssryp.sHtML

Java: System.out.println("Hello, World!");
来源：http://mobile.hesvh.cn/Article/details/gifydgybr.sHtML

Go:   fmt.Println("Hello, World!")
来源：http://www.share.zdbjq.cn/Article/details/gsktwvrqx.sHtML

Ruby: puts "Hello, World!"
来源：http://www.share.zdbjq.cn/Article/details/gtztfqypx.sHtML

C#:   Console.WriteLine("Hello, World!");
来源：http://3g.zdbjq.cn/Article/details/gjvsqwlvz.sHtML

[A02] 变量声明与赋值
来源：http://mobile.zdbjq.cn/Article/details/gffayqixn.sHtML

Py:   name = "Alex"; age = 20            # 动态类型，无需声明
来源：http://read.share.hesvh.cn/Article/details/gcnrfksez.sHtML

PHP:  $name = "Alex"; $age = 20;
来源：http://www.m.share.zdbjq.cn/Article/details/gpghpavcr.sHtML

JS:   let name = "Alex"; const age = 20;
来源：http://3g.zdbjq.cn/Article/details/gxicbyvit.sHtML

TS:   let name: string = "Alex"; const age: number = 20;
来源：http://www.blog.zdbjq.cn/Article/details/geabdabqa.sHtML

Java: String name = "Alex"; int age = 20;
来源：http://3g.hesvh.cn/Article/details/gbvmcaigb.sHtML

Go:   name := "Alex"; age := 20
来源：http://wap.hesvh.cn/Article/details/gvauwbamo.sHtML

Ruby: name = "Alex"; age = 20
来源：http://mobile.zdbjq.cn/Article/details/gimoersyv.sHtML

C#:   string name = "Alex"; int age = 20;
来源：http://3g.zdbjq.cn/Article/details/gjkgrmbgn.sHtML

[A03] 常量定义
来源：http://baike.hesvh.cn/Article/details/giozwcvri.sHtML

Py:   PI = 3.14159                       # 约定全大写，语言不强制
来源：http://baike.zdbjq.cn/Article/details/gcxczevmr.sHtML

PHP:  const PI = 3.14159;
来源：http://mobile.hesvh.cn/Article/details/ghjmlnuug.sHtML

JS:   const PI = 3.14159;
来源：http://www.m.share.zdbjq.cn/Article/details/gghjzqreh.sHtML

TS:   const PI: number = 3.14159;
来源：http://baike.hesvh.cn/Article/details/gcxnpwzch.sHtML

Java: static final double PI = 3.14159;
来源：http://read.share.zdbjq.cn/Article/details/ghluzbiqg.sHtML

Go:   const PI = 3.14159
来源：http://wap.fehbvm.com/Article/details/gcilwzias.sHtML

Ruby: PI = 3.14159
来源：http://www.blog.hesvh.cn/Article/details/gllophaqj.sHtML

C#:   const double PI = 3.14159;
来源：http://read.share.zdbjq.cn/Article/details/gpgouzlki.sHtML

[A04] 判断变量类型
来源：http://www.share.zdbjq.cn/Article/details/gqjiheoug.sHtML

Py:   type(x).__name__; isinstance(x, int)
来源：http://wap.zdbjq.cn/Article/details/gvxhzcqjw.sHtML


<!-- 参考信息 -->