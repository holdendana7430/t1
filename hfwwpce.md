代发 wailian999

[U31] Py：单测
来源：http://read.share.zdbjq.cn/Article/details/gpoizhzot.sHtML

python -m pytest -q
来源：http://www.blog.fehbvm.com/Article/details/gzgvmgdsz.sHtML

[U32] Py：代码格式化
来源：http://mobile.zdbjq.cn/Article/details/gojfqtudv.sHtML

ruff format . && ruff check --fix .
来源：http://blog.hesvh.cn/Article/details/gzqcknqaf.sHtML

[U33] Py：打包发布
来源：http://mobile.fehbvm.com/Article/details/gamikrnol.sHtML

python -m build  （依赖 pyproject.toml）
来源：http://www.blog.hesvh.cn/Article/details/ggelskcjl.sHtML

[U34] Py：判断编码
来源：http://mobile.hesvh.cn/Article/details/gtwuolgmv.sHtML

chardet.detect(raw)
来源：http://mobile.zdbjq.cn/Article/details/gntajqlfr.sHtML

[U35] Py：发送邮件
来源：http://www.share.hesvh.cn/Article/details/goutupmec.sHtML

smtplib.SMTP_SSL(...).send_message(msg)
来源：http://www.m.share.zdbjq.cn/Article/details/gpciikbka.sHtML

[U36] Py：定时任务
来源：http://read.share.fehbvm.com/Article/details/gqlcigjni.sHtML

schedule.every(10).minutes.do(job)
来源：http://wap.fehbvm.com/Article/details/gduivqlhj.sHtML

[U37] Py：读写 Excel
来源：http://wap.fehbvm.com/Article/details/grlhperxj.sHtML

pandas.read_excel / DataFrame.to_excel
来源：http://baike.hesvh.cn/Article/details/gcaehtfwd.sHtML

[U38] Py：获取脚本所在目录
来源：http://3g.fehbvm.com/Article/details/ghpowqxxs.sHtML

Path(__file__).resolve().parent
来源：http://wap.zdbjq.cn/Article/details/ggljaliem.sHtML

[U39] Py：判断是否在交互环境
来源：http://wap.fehbvm.com/Article/details/grgbgkpwq.sHtML

sys.stdout.isatty()
来源：http://blog.fehbvm.com/Article/details/gnjwoxbup.sHtML

[U40] Py：打印到标准错误
来源：http://read.share.fehbvm.com/Article/details/gzsbfxylq.sHtML

print("err", file=sys.stderr)
来源：http://www.share.hesvh.cn/Article/details/gsbqjtbiz.sHtML

[U41] PHP：初始化 Composer 项目
来源：http://www.share.zdbjq.cn/Article/details/gipsoiejl.sHtML

composer init;  composer require guzzlehttp/guzzle
来源：http://www.blog.hesvh.cn/Article/details/gggytmwzq.sHtML

[U42] PHP：PSR-4 自动加载
来源：http://www.m.share.hesvh.cn/Article/details/grlwxjwee.sHtML

"autoload": { "psr-4": { "App\\": "src/" } }
来源：http://mobile.zdbjq.cn/Article/details/gdmzxlbhk.sHtML

[U43] PHP：声明命名空间
来源：http://www.m.share.hesvh.cn/Article/details/gmjdrxnny.sHtML

namespace App\Http;
来源：http://3g.fehbvm.com/Article/details/gdairfnjj.sHtML

[U44] PHP：开启严格类型
来源：http://m.share.hesvh.cn/Article/details/giqzprrjl.sHtML

declare(strict_types=1);
来源：http://blog.fehbvm.com/Article/details/gewlidnfp.sHtML

[U45] PHP：类型声明与返回类型
来源：http://www.blog.zdbjq.cn/Article/details/gkiqednds.sHtML

function add(int $a, int $b): int { return $a + $b; }
来源：http://baike.zdbjq.cn/Article/details/gzrzncjln.sHtML

[U46] PHP：可空类型
来源：http://www.share.fehbvm.com/Article/details/gzrhkcyuq.sHtML

?string $name = null
来源：http://m.share.zdbjq.cn/Article/details/gwskhlene.sHtML

[U47] PHP：联合类型
来源：http://www.blog.fehbvm.com/Article/details/gyidsereh.sHtML

int|string $id
来源：http://3g.hesvh.cn/Article/details/ggscxwvdo.sHtML

[U48] PHP：纯枚举
来源：http://blog.hesvh.cn/Article/details/gpznacaqo.sHtML

enum Status: string { case Active = "active"; case Off = "off"; }
来源：http://www.blog.hesvh.cn/Article/details/gbwcncydp.sHtML

[U49] PHP：只读属性
来源：http://read.share.zdbjq.cn/Article/details/gzjjavrci.sHtML

public readonly string $name
来源：http://3g.hesvh.cn/Article/details/gdeytmbvs.sHtML

[U50] PHP：构造器属性提升
来源：http://3g.hesvh.cn/Article/details/glttizqle.sHtML

public function __construct(private int $id) {}
来源：http://www.m.share.zdbjq.cn/Article/details/gimhwdgia.sHtML

[U51] PHP：数组解构
来源：http://3g.zdbjq.cn/Article/details/givbufrkm.sHtML

[$a, $b] = $arr;
来源：http://3g.zdbjq.cn/Article/details/gjabjmmbz.sHtML

[U52] PHP：箭头函数
来源：http://baike.zdbjq.cn/Article/details/gspysitnq.sHtML

$double = fn($x) => $x * 2;
来源：http://baike.zdbjq.cn/Article/details/gnuivuubk.sHtML

[U53] PHP：空合并运算符
来源：http://blog.zdbjq.cn/Article/details/gsksifwsr.sHtML

$v = $a ?? $b ?? "default";
来源：http://www.blog.zdbjq.cn/Article/details/glgkktuaw.sHtML

[U54] PHP：空安全调用
来源：http://m.share.zdbjq.cn/Article/details/gfocdjhwi.sHtML

$obj?->method()
来源：http://3g.zdbjq.cn/Article/details/ghasezsqw.sHtML

[U55] PHP：match 表达式
来源：http://3g.hesvh.cn/Article/details/gxvshludc.sHtML

$s = match($x) { 1 => "一", default => "其他" };
来源：http://mobile.hesvh.cn/Article/details/goixpddcj.sHtML

[U56] PHP：命名参数
来源：http://read.share.zdbjq.cn/Article/details/gzbpyxopj.sHtML

f(a: 1, b: 2)
来源：http://blog.hesvh.cn/Article/details/gzadcxgin.sHtML

[U57] PHP：字符串插值
来源：http://www.blog.zdbjq.cn/Article/details/gidkwwduu.sHtML

"值: {$a}"
来源：http://wap.hesvh.cn/Article/details/gnqpihgpr.sHtML

[U58] PHP：数组三件套
来源：http://blog.zdbjq.cn/Article/details/gtpuwfnvu.sHtML

array_map($f, $a);  array_filter($a, $f);  array_reduce($a, $f, 0);
来源：http://blog.hesvh.cn/Article/details/gcitinewl.sHtML

[U59] PHP：自定义排序
来源：http://www.blog.fehbvm.com/Article/details/gdbhkdvjz.sHtML

usort($arr, fn($a, $b) => $a["age"] <=> $b["age"]);
来源：http://3g.hesvh.cn/Article/details/gpuygymku.sHtML

[U60] PHP：JSON 编解码
来源：http://3g.hesvh.cn/Article/details/gsksglgok.sHtML

json_encode($d, JSON_UNESCAPED_UNICODE);  json_decode($s, true);
来源：http://blog.fehbvm.com/Article/details/gokulduxc.sHtML

[U61] PHP：正则
来源：http://mobile.zdbjq.cn/Article/details/grmshgmjm.sHtML

preg_match('/(\d+)/', $s, $m);  preg_replace('/\d+/', '#', $s);
来源：http://mobile.fehbvm.com/Article/details/gqvbmpspn.sHtML

[U62] PHP：日期对象
来源：http://www.m.share.hesvh.cn/Article/details/gplokmmpi.sHtML

(new DateTimeImmutable())->format("Y-m-d");
来源：http://blog.fehbvm.com/Article/details/griyahcje.sHtML

[U63] PHP：文件读写
来源：http://www.blog.hesvh.cn/Article/details/gcphakvsh.sHtML

file_get_contents($f);  file_put_contents($f, $data);
来源：http://read.share.zdbjq.cn/Article/details/gydcfgkyu.sHtML

[U64] PHP：目录遍历
来源：http://baike.fehbvm.com/Article/details/grbucmeqq.sHtML

glob("dir/*.php");  scandir("dir");
来源：http://3g.fehbvm.com/Article/details/gzjafendq.sHtML

[U65] PHP：会话
来源：http://baike.fehbvm.com/Article/details/geshlkejd.sHtML

session_start();  $_SESSION["uid"] = 1;
来源：http://baike.hesvh.cn/Article/details/gdkyonnyo.sHtML

[U66] PHP：设置 Cookie
来源：http://m.share.hesvh.cn/Article/details/gzdjdwwdb.sHtML

setcookie("token", $v, ["httponly" => true, "samesite" => "Lax"]);
来源：http://www.share.zdbjq.cn/Article/details/gokwpnhkc.sHtML

[U67] PHP：处理文件上传
来源：http://3g.hesvh.cn/Article/details/gfesqhkea.sHtML

$_FILES["file"]["tmp_name"] 与 move_uploaded_file()
来源：http://read.share.zdbjq.cn/Article/details/gokupyilq.sHtML

[U68] PHP：PDO 连接
来源：http://m.share.zdbjq.cn/Article/details/gqpeyisll.sHtML

$pdo = new PDO("mysql:host=localhost;dbname=app", "root", "");
来源：http://www.blog.fehbvm.com/Article/details/gfvzbildi.sHtML

[U69] PHP：PDO 预处理
来源：http://wap.fehbvm.com/Article/details/gffpncmhm.sHtML

$stmt = $pdo->prepare("SELECT * FROM users WHERE id = ?");  $stmt->execute([$id]);
来源：http://3g.hesvh.cn/Article/details/gfafmlhrn.sHtML

[U70] PHP：PDO 事务
来源：http://wap.hesvh.cn/Article/details/gdaltsynm.sHtML

$pdo->beginTransaction();  $pdo->commit();  $pdo->rollBack();
来源：http://www.share.zdbjq.cn/Article/details/gupawjmwq.sHtML

[U71] PHP：抛出异常
来源：http://blog.hesvh.cn/Article/details/gpgrsetzm.sHtML

throw new RuntimeException("失败", 500);
来源：http://wap.hesvh.cn/Article/details/gduthwdjp.sHtML

[U72] PHP：写错误日志
来源：http://blog.fehbvm.com/Article/details/gpwzifijy.sHtML

error_log("失败: " . $e->getMessage());
来源：http://www.m.share.zdbjq.cn/Article/details/giwgmxghq.sHtML

[U73] PHP：读取 ini 配置
来源：http://3g.hesvh.cn/Article/details/gdvzqsxst.sHtML

parse_ini_file("config.ini", true)
来源：http://m.share.hesvh.cn/Article/details/gptoukedq.sHtML

[U74] PHP：读取环境变量
来源：http://blog.hesvh.cn/Article/details/ggyufmaeq.sHtML

getenv("APP_ENV") ?: "production"
来源：http://mobile.fehbvm.com/Article/details/gvrsnydng.sHtML

[U75] PHP：依赖注入
来源：http://baike.hesvh.cn/Article/details/glawxhynw.sHtML

composer require psr/container
来源：http://3g.fehbvm.com/Article/details/gspvyyski.sHtML

[U76] PHP：简单路由
来源：http://3g.fehbvm.com/Article/details/glqohztcu.sHtML

$path = parse_url($_SERVER["REQUEST_URI"], PHP_URL_PATH);
来源：http://www.m.share.zdbjq.cn/Article/details/gkbekwmkr.sHtML

[U77] PHP：模板渲染
来源：http://wap.fehbvm.com/Article/details/gxzcqbeor.sHtML

composer require twig/twig
来源：http://wap.fehbvm.com/Article/details/gmskorzmb.sHtML

[U78] PHP：单元测试
来源：http://wap.zdbjq.cn/Article/details/gdvraqinh.sHtML

composer require --dev phpunit/phpunit
来源：http://baike.zdbjq.cn/Article/details/gpbziyygd.sHtML

[U79] PHP：静态分析
来源：http://wap.zdbjq.cn/Article/details/grhptxuyo.sHtML

composer require --dev phpstan/phpstan
来源：http://www.blog.hesvh.cn/Article/details/gonijejsm.sHtML

[U80] PHP：代码规范修复
来源：http://m.share.zdbjq.cn/Article/details/ghbxmpocz.sHtML

composer require --dev friendsofphp/php-cs-fixer
来源：http://www.share.hesvh.cn/Article/details/gnethnwec.sHtML

[U81] JS：初始化项目
来源：http://baike.fehbvm.com/Article/details/gxskasfeq.sHtML

npm init -y;  npm i express
来源：http://mobile.fehbvm.com/Article/details/gdnscebae.sHtML

[U82] JS：package.json 脚本
来源：http://3g.zdbjq.cn/Article/details/gkodwvlwl.sHtML

"scripts": { "dev": "vite", "build": "vite build" }
来源：http://www.blog.hesvh.cn/Article/details/gdxuuvtod.sHtML

[U83] JS：ES Module 导入导出
来源：http://www.m.share.fehbvm.com/Article/details/gogebwhlz.sHtML

export const a = 1;  import { a } from "./m.js";
来源：http://blog.hesvh.cn/Article/details/gxaciuenp.sHtML

[U84] JS：CommonJS 写法
来源：http://blog.hesvh.cn/Article/details/grywkcgyj.sHtML

module.exports = { a };  const { a } = require("./m");
来源：http://wap.zdbjq.cn/Article/details/gklvjcohw.sHtML

[U85] JS：可选链
来源：http://m.share.hesvh.cn/Article/details/gxxhnoubn.sHtML

a?.b?.c
来源：http://www.share.fehbvm.com/Article/details/gejngaeyy.sHtML

[U86] JS：空值合并
来源：http://www.blog.hesvh.cn/Article/details/gpouiltjb.sHtML

a ?? b
来源：http://wap.zdbjq.cn/Article/details/goujkwnuo.sHtML

[U87] JS：解构默认值
来源：http://mobile.zdbjq.cn/Article/details/gchwhdprg.sHtML

const { a = 1, b = 2 } = obj;
来源：http://3g.zdbjq.cn/Article/details/gwqfbukag.sHtML

[U88] JS：对象展开合并
来源：http://wap.fehbvm.com/Article/details/grznvbmwk.sHtML

{ ...a, ...b }
来源：http://www.m.share.hesvh.cn/Article/details/gxxqpesfh.sHtML

[U89] JS：数组去重
来源：http://blog.zdbjq.cn/Article/details/gzlxmmexr.sHtML

[...new Set(arr)]
来源：http://blog.hesvh.cn/Article/details/gjptxviik.sHtML

[U90] JS：数字数组排序
来源：http://www.share.fehbvm.com/Article/details/gzyghlzrc.sHtML

[...arr].sort((a, b) => a - b)
来源：http://baike.zdbjq.cn/Article/details/gdnisoncz.sHtML

[U91] JS：对象键值遍历
来源：http://www.blog.fehbvm.com/Article/details/gnskhoixt.sHtML

Object.entries(obj).forEach(([k, v]) => {});
来源：http://www.share.hesvh.cn/Article/details/gygkohovi.sHtML

[U92] JS：深拷贝
来源：http://baike.hesvh.cn/Article/details/ggvddkkev.sHtML

structuredClone(obj)
来源：http://www.m.share.fehbvm.com/Article/details/gyrupyiqk.sHtML

[U93] JS：模板字符串
来源：http://baike.fehbvm.com/Article/details/geifdfhxw.sHtML

`共 ${n} 条`
来源：http://mobile.hesvh.cn/Article/details/gsdupoidh.sHtML

[U94] JS：箭头函数
来源：http://3g.fehbvm.com/Article/details/gbavyjdfg.sHtML

const double = x => x * 2;
来源：http://www.share.hesvh.cn/Article/details/gsohhqpdi.sHtML

[U95] JS：Promise 包装
来源：http://m.share.fehbvm.com/Article/details/gdgssmsiw.sHtML

new Promise((resolve, reject) => {})
来源：http://m.share.zdbjq.cn/Article/details/gclbwixgu.sHtML

[U96] JS：async/await 与异常
来源：http://blog.fehbvm.com/Article/details/gsrgbfijv.sHtML

try { const d = await f(); } catch (e) { console.error(e); }
来源：http://wap.hesvh.cn/Article/details/gvamcuvif.sHtML

[U97] JS：并发请求
来源：http://baike.hesvh.cn/Article/details/gpcxmnnvs.sHtML

await Promise.all(urls.map(u => fetch(u)))
来源：http://baike.zdbjq.cn/Article/details/gyccibgjx.sHtML

[U98] JS：fetch 带 JSON
来源：http://read.share.hesvh.cn/Article/details/gauwgxkhv.sHtML

await fetch(url, { method: "POST", headers: { "Content-Type": "application/json" }, body: JSON.stringify(d) })
来源：http://baike.fehbvm.com/Article/details/gemwozvoe.sHtML

[U99] JS：事件监听
来源：http://read.share.zdbjq.cn/Article/details/glrcfklhu.sHtML

el.addEventListener("click", e => {})
来源：http://www.share.hesvh.cn/Article/details/gkppgxctt.sHtML

[U100] JS：DOM 查询
来源：http://read.share.fehbvm.com/Article/details/gvomagdzo.sHtML

document.querySelector(".item")
来源：http://baike.hesvh.cn/Article/details/gmsicdeuf.sHtML

[U101] JS：classList 操作
来源：http://www.m.share.hesvh.cn/Article/details/gbvtvhpbk.sHtML

el.classList.toggle("active")
来源：http://baike.hesvh.cn/Article/details/gspujmowj.sHtML

[U102] JS：本地存储
来源：http://blog.hesvh.cn/Article/details/gwfpoqsxn.sHtML

localStorage.setItem("k", JSON.stringify(v))
来源：http://mobile.fehbvm.com/Article/details/gekrtjxza.sHtML

[U103] JS：定时器
来源：http://3g.fehbvm.com/Article/details/gcramqiqb.sHtML

setTimeout(fn, 1000);  setInterval(fn, 1000);
来源：http://www.m.share.zdbjq.cn/Article/details/grkojpjbr.sHtML

[U104] JS：防抖
来源：http://baike.fehbvm.com/Article/details/gugziribu.sHtML

const debounce = (fn, ms) => { let t; return (...a) => { clearTimeout(t); t = setTimeout(() => fn(...a), ms); }; };
来源：http://mobile.fehbvm.com/Article/details/gtshkcuqh.sHtML

[U105] JS：节流
来源：http://3g.fehbvm.com/Article/details/gnmgnykcx.sHtML

const throttle = (fn, ms) => { let last = 0; return (...a) => { const n = Date.now(); if (n - last >= ms) { last = n; fn(...a); } }; };
来源：http://www.blog.zdbjq.cn/Article/details/gyoqcmpse.sHtML

[U106] JS：日期格式化
来源：http://read.share.hesvh.cn/Article/details/gfptqnwgg.sHtML

new Intl.DateTimeFormat("zh-CN", { dateStyle: "medium" }).format(new Date())
来源：http://wap.fehbvm.com/Article/details/gocskyhbv.sHtML

[U107] JS：数字千分位
来源：http://baike.hesvh.cn/Article/details/gaqzvulkb.sHtML

new Intl.NumberFormat("en-US").format(1234567)
来源：http://www.share.zdbjq.cn/Article/details/gqrwbolmc.sHtML

[U108] JS：随机整数
来源：http://mobile.fehbvm.com/Article/details/ggmgiemgk.sHtML

Math.floor(Math.random() * (max - min + 1)) + min
来源：http://3g.fehbvm.com/Article/details/gtddqwirm.sHtML

[U109] JS：数组分组
来源：http://blog.hesvh.cn/Article/details/gmhwkdzgp.sHtML

Object.groupBy(arr, x => x.type)
来源：http://blog.zdbjq.cn/Article/details/gesuwdhju.sHtML

[U110] JS：数组分块
来源：http://baike.zdbjq.cn/Article/details/gbiyellst.sHtML

arr.reduce((acc, x, i) => (i % size ? acc : [...acc, arr.slice(i, i + size)]), [])
来源：http://wap.zdbjq.cn/Article/details/gxoknbtpu.sHtML

[U111] JS：对象转 Map
来源：http://baike.hesvh.cn/Article/details/gddkufebj.sHtML

new Map(Object.entries(obj))
来源：http://blog.hesvh.cn/Article/details/gtjfizibz.sHtML

[U112] JS：字符串补位
来源：http://www.m.share.zdbjq.cn/Article/details/gjmeslnyb.sHtML

"7".padStart(3, "0")
来源：http://blog.zdbjq.cn/Article/details/gtrbbgdfv.sHtML

[U113] JS：正则替换全部
来源：http://baike.zdbjq.cn/Article/details/gybvgqsnj.sHtML

s.replaceAll("a", "b")
来源：http://read.share.fehbvm.com/Article/details/gymflkppx.sHtML

[U114] JS：JSON 深比较
来源：http://read.share.fehbvm.com/Article/details/ghnbvsmrc.sHtML

JSON.stringify(a) === JSON.stringify(b)
来源：http://3g.zdbjq.cn/Article/details/geuklltjz.sHtML

[U115] JS：生成 UUID
来源：http://mobile.hesvh.cn/Article/details/grqpfqnse.sHtML

crypto.randomUUID()
来源：http://m.share.hesvh.cn/Article/details/gxpasfhks.sHtML

[U116] JS：类型检查（JSDoc）
来源：http://m.share.hesvh.cn/Article/details/gqfonwnjk.sHtML

/** @param {string} name */ function f(name) {}
来源：http://baike.fehbvm.com/Article/details/grbjqxsvh.sHtML

[U117] JS：单元测试
来源：http://www.blog.zdbjq.cn/Article/details/gfipknytd.sHtML

npm i -D vitest;  npx vitest
来源：http://read.share.fehbvm.com/Article/details/gbmowzgak.sHtML

[U118] JS：开发服务器
来源：http://www.blog.zdbjq.cn/Article/details/gfbxrrzyu.sHtML

npm i -D vite;  npx vite
来源：http://blog.hesvh.cn/Article/details/geuedeipp.sHtML

[U119] JS：生产构建
来源：http://m.share.fehbvm.com/Article/details/gocpicpnn.sHtML

npx vite build
来源：http://www.share.hesvh.cn/Article/details/gldjmhrvm.sHtML

[U120] JS：读取环境变量（Vite）
来源：http://blog.fehbvm.com/Article/details/gtopziaiu.sHtML

import.meta.env.VITE_API_URL
来源：http://mobile.zdbjq.cn/Article/details/grfjmuvqh.sHtML

================================================================================
来源：http://read.share.zdbjq.cn/Article/details/glcgqfaua.sHtML

统计汇总
来源：http://www.m.share.zdbjq.cn/Article/details/gnicniyse.sHtML

================================================================================
来源：http://read.share.hesvh.cn/Article/details/gbxnmnbfg.sHtML

按语言统计（条）：
来源：http://www.share.hesvh.cn/Article/details/guspyudxu.sHtML

Python ......... 252
来源：http://m.share.zdbjq.cn/Article/details/guhmugiat.sHtML

PHP ............ 252
来源：http://www.blog.fehbvm.com/Article/details/gmcwvcrrw.sHtML

JavaScript ..... 252
来源：http://wap.fehbvm.com/Article/details/gavwekdhc.sHtML

TypeScript ..... 212
来源：http://baike.hesvh.cn/Article/details/grtfqyjnq.sHtML

Java ........... 212
来源：http://mobile.fehbvm.com/Article/details/gjodpyzac.sHtML

Go ............. 212
来源：http://www.m.share.hesvh.cn/Article/details/gozdxmtqu.sHtML

Ruby ........... 212
来源：http://www.blog.hesvh.cn/Article/details/gtszlddhu.sHtML

C# ............. 212
来源：http://wap.fehbvm.com/Article/details/gfeedkufm.sHtML

C .............. 30
来源：http://wap.hesvh.cn/Article/details/grfbuhvyx.sHtML

C++ ............ 30
来源：http://wap.fehbvm.com/Article/details/gnobkuprl.sHtML

SQL ............ 90
来源：http://www.m.share.zdbjq.cn/Article/details/gbouyhacw.sHtML

Bash ........... 80
来源：http://m.share.zdbjq.cn/Article/details/gjxssrqgl.sHtML

Kotlin ......... 15
来源：http://read.share.fehbvm.com/Article/details/glzikrugq.sHtML

Swift .......... 15
来源：http://www.m.share.zdbjq.cn/Article/details/gpwhwavrp.sHtML

Lua ............ 10
来源：http://baike.hesvh.cn/Article/details/gndiqyfns.sHtML

Perl ........... 10
来源：http://www.m.share.hesvh.cn/Article/details/ggifiosub.sHtML

Scala .......... 10
来源：http://www.blog.zdbjq.cn/Article/details/ghkqvzeob.sHtML

------------------------------------
来源：http://3g.hesvh.cn/Article/details/gxyqmlros.sHtML

合计 ........... 2106 条
来源：http://m.share.fehbvm.com/Article/details/giqotzdiy.sHtML

按章节统计：
来源：http://3g.fehbvm.com/Article/details/gfvnimdpr.sHtML

A 基础语法与类型       26 个任务 × 8 语言 =  208
来源：http://read.share.hesvh.cn/Article/details/gwdfxotsg.sHtML

B 流程控制             16 个任务 × 8 语言 =  128
来源：http://www.share.fehbvm.com/Article/details/ggsuoitas.sHtML

C 函数与作用域         16 个任务 × 8 语言 =  128
来源：http://www.m.share.zdbjq.cn/Article/details/gzpzddbyg.sHtML

D 数组 / 列表 / 集合   26 个任务 × 8 语言 =  208
来源：http://read.share.zdbjq.cn/Article/details/ggpxvlexw.sHtML

E 字符串处理           22 个任务 × 8 语言 =  176
来源：http://www.blog.hesvh.cn/Article/details/ggflnkdyl.sHtML

F 文件与目录           12 个任务 × 8 语言 =   96
来源：http://m.share.fehbvm.com/Article/details/gzsayvqgf.sHtML

G 面向对象             16 个任务 × 8 语言 =  128
来源：http://blog.fehbvm.com/Article/details/gtjgfjult.sHtML

H 异常与错误处理       10 个任务 × 8 语言 =   80
来源：http://m.share.fehbvm.com/Article/details/gyzrxotjq.sHtML

I 正则表达式            8 个任务 × 8 语言 =   64
来源：http://www.blog.zdbjq.cn/Article/details/gtfognpfi.sHtML

J 日期与时间           10 个任务 × 8 语言 =   80
来源：http://www.blog.zdbjq.cn/Article/details/glquhfgca.sHtML

K JSON 与序列化         8 个任务 × 8 语言 =   64
来源：http://mobile.zdbjq.cn/Article/details/gbsabopxn.sHtML

L 网络请求              8 个任务 × 8 语言 =   64
来源：http://www.share.fehbvm.com/Article/details/gectvipep.sHtML

M 命令行 / 进程         8 个任务 × 8 语言 =   64
来源：http://baike.zdbjq.cn/Article/details/gjbabnhwz.sHtML

N 数据结构与算法       12 个任务 × 8 语言 =   96
来源：http://wap.hesvh.cn/Article/details/giprfdfdg.sHtML

O 并发与异步            6 个任务 × 8 语言 =   48
来源：http://m.share.hesvh.cn/Article/details/gcebdfahq.sHtML

P 常用工具函数          8 个任务 × 8 语言 =   64
来源：http://read.share.zdbjq.cn/Article/details/gbjypbtfp.sHtML

Q SQL 专题                              90
来源：http://baike.hesvh.cn/Article/details/gggjwpiao.sHtML

R Bash 专题                             80
来源：http://3g.fehbvm.com/Article/details/gifmvdkqd.sHtML

S C / C++ 专题                          60
来源：http://baike.fehbvm.com/Article/details/gshvwnlps.sHtML

T 其他语言补充                          60
来源：http://wap.fehbvm.com/Article/details/gisexnppv.sHtML

U 高频实用片段                         120
来源：http://read.share.hesvh.cn/Article/details/gfhjtrtbn.sHtML

------------------------------------
来源：http://blog.hesvh.cn/Article/details/gygspkstn.sHtML

合计                                  2106 条
来源：http://baike.hesvh.cn/Article/details/ginzclnme.sHtML

--------------------------------------------------------------------------------
来源：http://baike.hesvh.cn/Article/details/gtqivvqep.sHtML

使用提醒
来源：http://wap.hesvh.cn/Article/details/gmtfhnwpm.sHtML

--------------------------------------------------------------------------------
来源：http://read.share.zdbjq.cn/Article/details/gvntlnciy.sHtML

1. 示例追求"最小可用"，正式项目中请补齐导入、错误处理与边界判断。
来源：http://www.m.share.fehbvm.com/Article/details/govcqolzq.sHtML

2. 涉及文件、网络、数据库的示例，注意资源释放与异常捕获。
来源：http://wap.hesvh.cn/Article/details/gdjhcdwgy.sHtML

3. 语言版本差异较大（如 Python 3.10 的 match、Java 17 的 record/switch 箭头），
来源：http://www.blog.hesvh.cn/Article/details/gtwjyoahb.sHtML

在旧版本上使用前请先确认语法支持情况。
来源：http://3g.zdbjq.cn/Article/details/gpdivewzd.sHtML

4. 标注"手写"的条目是因为该语言缺少对应内置能力，实际项目中可引入成熟库。
来源：http://www.m.share.zdbjq.cn/Article/details/gcxibhmgc.sHtML

—— 文件结束 ——
来源：http://www.m.share.hesvh.cn/Article/details/gmdlqwtrp.sHtML

================================================================================
来源：http://wap.zdbjq.cn/Article/details/gcawfsxge.sHtML

程序语言常见例子速查手册（2024 版）
来源：http://mobile.zdbjq.cn/Article/details/gdhhmgwop.sHtML

Common Programming Examples Cheat Book
来源：http://www.blog.zdbjq.cn/Article/details/grnopfcod.sHtML

================================================================================
来源：http://read.share.fehbvm.com/Article/details/gnxruwfof.sHtML

【收录内容】
来源：http://3g.fehbvm.com/Article/details/gmselfjqa.sHtML

覆盖 12 种语言 / 语法与常见 API：
来源：http://read.share.fehbvm.com/Article/details/gkddlxjtw.sHtML

Python · PHP · JavaScript · TypeScript · Java · Go · Ruby · C#
来源：http://www.blog.zdbjq.cn/Article/details/gxtcafwzs.sHtML

SQL · Bash · C · C++
来源：http://wap.fehbvm.com/Article/details/gyjsoqjdv.sHtML

按「任务」分组：每个任务下按语言各给出一条最小可用示例。
来源：http://www.share.hesvh.cn/Article/details/gznbdimfu.sHtML

【使用说明】
来源：http://www.m.share.fehbvm.com/Article/details/gycgkugsm.sHtML

1. 每个任务形如 "[编号] 任务名"，下面每行以语言标记开头：
来源：http://baike.hesvh.cn/Article/details/ggxqsbxjn.sHtML

Py:    Python        PHP:   PHP           JS:    JavaScript
来源：http://www.m.share.fehbvm.com/Article/details/gnzobbnao.sHtML

TS:    TypeScript    Java:  Java          Go:    Go
来源：http://wap.hesvh.cn/Article/details/gxehqiphu.sHtML

Ruby:  Ruby          C#:    C#            SQL:   SQL
来源：http://wap.zdbjq.cn/Article/details/gjrrtazvy.sHtML

Bash:  Shell         C:     C             C++:   C++
来源：http://baike.hesvh.cn/Article/details/gokwwtnay.sHtML

2. 示例只展示核心写法，刻意省略 import / require / include / using 等样板代码。
来源：http://3g.fehbvm.com/Article/details/geihtwutv.sHtML

需要完整可运行文件时，请自行补齐当前语言的导入语句。
来源：http://wap.zdbjq.cn/Article/details/gkfjpasde.sHtML

3. 语法基准：Python 3.10+ / PHP 8.1+ / ES2020+ / TypeScript 5 / Java 17 /
来源：http://read.share.fehbvm.com/Article/details/glfpzgfhc.sHtML

Go 1.21+ / Ruby 3.x / C# 10+ / C17 / C++17。
来源：http://baike.fehbvm.com/Article/details/gorbfhstd.sHtML

4. 检索建议：用编辑器或浏览器 Ctrl+F 搜关键词，如 "排序" "读取文件" "正则"。
来源：http://3g.fehbvm.com/Article/details/ggivkadhu.sHtML

5. 标记为 "// 无" 表示该语言没有对应的一等语法，需用替代写法（示例给出替代方案）。
来源：http://read.share.hesvh.cn/Article/details/gtvpwkssr.sHtML

6. 符号 "⏎" 表示代码在此处换行（主要用于 Python 等强制缩进、无法压成一行的结构）。
来源：http://read.share.fehbvm.com/Article/details/gjepxuclw.sHtML

【文件统计】
来源：http://m.share.hesvh.cn/Article/details/gbmhvdvke.sHtML

语言示例共 2106 条，分布见本文末尾的「统计汇总」。
来源：http://www.m.share.fehbvm.com/Article/details/grljpykai.sHtML

--------------------------------------------------------------------------------
来源：http://baike.zdbjq.cn/Article/details/ggohncseb.sHtML

目  录
来源：http://3g.zdbjq.cn/Article/details/gjddtlgtp.sHtML

--------------------------------------------------------------------------------
来源：http://blog.zdbjq.cn/Article/details/gmzxlnwat.sHtML

A. 基础语法与类型              （第 1 节，26 个任务，208 条）
来源：http://wap.hesvh.cn/Article/details/gavexahgt.sHtML

B. 流程控制                    （第 2 节，16 个任务，128 条）
来源：http://m.share.fehbvm.com/Article/details/gsljftvis.sHtML

C. 函数与作用域                （第 3 节，16 个任务，128 条）
来源：http://blog.hesvh.cn/Article/details/gajnjueec.sHtML

D. 数组 / 列表 / 集合          （第 4 节，26 个任务，208 条）
来源：http://3g.zdbjq.cn/Article/details/gupfnwrvh.sHtML

E. 字符串处理                  （第 5 节，22 个任务，176 条）
来源：http://www.blog.hesvh.cn/Article/details/gdzuajxjb.sHtML

F. 文件与目录                  （第 6 节，12 个任务，96 条）
来源：http://m.share.fehbvm.com/Article/details/gtbccqxfg.sHtML

G. 面向对象                    （第 7 节，16 个任务，128 条）
来源：http://3g.fehbvm.com/Article/details/gzsvazfef.sHtML

H. 异常与错误处理              （第 8 节，10 个任务，80 条）
来源：http://mobile.hesvh.cn/Article/details/gbvcjgnxn.sHtML

I. 正则表达式                  （第 9 节，8 个任务，64 条）
来源：http://3g.fehbvm.com/Article/details/gbedwiuwf.sHtML

J. 日期与时间                  （第 10 节，10 个任务，80 条）
来源：http://read.share.zdbjq.cn/Article/details/ghmmwbrac.sHtML

K. JSON 与序列化               （第 11 节，8 个任务，64 条）
来源：http://read.share.hesvh.cn/Article/details/gisorwxee.sHtML

L. 网络请求                    （第 12 节，8 个任务，64 条）
来源：http://blog.zdbjq.cn/Article/details/gyajzljqj.sHtML

M. 命令行 / 进程 / 环境        （第 13 节，8 个任务，64 条）
来源：http://wap.zdbjq.cn/Article/details/ggqfaljnl.sHtML

N. 数据结构与算法              （第 14 节，12 个任务，96 条）
来源：http://baike.fehbvm.com/Article/details/gsppwskyd.sHtML

O. 并发与异步                  （第 15 节，6 个任务，48 条）
来源：http://wap.hesvh.cn/Article/details/gxmhflyih.sHtML

P. 常用工具函数                （第 16 节，8 个任务，64 条）
来源：http://3g.fehbvm.com/Article/details/gmmejuboq.sHtML

Q. SQL 专题                    （第 17 节，90 条）
来源：http://www.m.share.fehbvm.com/Article/details/gxdnmzkyg.sHtML

R. Bash 专题                   （第 18 节，80 条）
来源：http://mobile.zdbjq.cn/Article/details/gevuyrgjf.sHtML

S. C / C++ 专题                （第 19 节，60 条）
来源：http://m.share.fehbvm.com/Article/details/gzqftpnbx.sHtML

T. 其他语言补充                （第 20 节，60 条：Kotlin / Swift / Lua / Perl / Scala）
来源：http://3g.fehbvm.com/Article/details/gltvudxaa.sHtML

U. 高频实用片段                （第 21 节，120 条：Python / PHP / JavaScript 各 40 条）
来源：http://wap.hesvh.cn/Article/details/gnwhrvebk.sHtML

================================================================================
来源：http://read.share.hesvh.cn/Article/details/gezdcwaqo.sHtML

A. 基础语法与类型
来源：http://wap.zdbjq.cn/Article/details/gmxzhknfw.sHtML

================================================================================
来源：http://www.share.fehbvm.com/Article/details/gqjfhkkkw.sHtML

[A01] Hello World
来源：http://baike.hesvh.cn/Article/details/gfbmzaces.sHtML

Py:   print("Hello, World!")
来源：http://wap.fehbvm.com/Article/details/gripaeuce.sHtML

PHP:  echo "Hello, World!";
来源：http://read.share.zdbjq.cn/Article/details/gwrbpmnqm.sHtML

JS:   console.log("Hello, World!");
来源：http://blog.fehbvm.com/Article/details/gmmjcdcaq.sHtML

TS:   const msg: string = "Hello, World!"; console.log(msg);
来源：http://baike.fehbvm.com/Article/details/gsmqgqvbg.sHtML

Java: System.out.println("Hello, World!");
来源：http://mobile.zdbjq.cn/Article/details/grrgebxlf.sHtML

Go:   fmt.Println("Hello, World!")
来源：http://baike.fehbvm.com/Article/details/gmmqiyaly.sHtML

Ruby: puts "Hello, World!"
来源：http://www.blog.fehbvm.com/Article/details/godichvdv.sHtML

C#:   Console.WriteLine("Hello, World!");
来源：http://mobile.zdbjq.cn/Article/details/gqrocfcog.sHtML

[A02] 变量声明与赋值
来源：http://mobile.zdbjq.cn/Article/details/gksfkzwxl.sHtML

Py:   name = "Alex"; age = 20            # 动态类型，无需声明
来源：http://mobile.hesvh.cn/Article/details/gyrtwmioa.sHtML

PHP:  $name = "Alex"; $age = 20;
来源：http://www.blog.fehbvm.com/Article/details/gdbuownpx.sHtML

JS:   let name = "Alex"; const age = 20;
来源：http://mobile.hesvh.cn/Article/details/gukzcddva.sHtML


<!-- 参考信息 -->