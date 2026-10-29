代发 wailian999

[U33] Py：打包发布
来源：http://www.share.zdbjq.cn/Article/details/gmnakevbx.sHtML

python -m build  （依赖 pyproject.toml）
来源：http://m.share.hesvh.cn/Article/details/gcaicwabo.sHtML

[U34] Py：判断编码
来源：http://www.share.hesvh.cn/Article/details/gpjpyyepo.sHtML

chardet.detect(raw)
来源：http://wap.zdbjq.cn/Article/details/ghgvfrbvm.sHtML

[U35] Py：发送邮件
来源：http://mobile.zdbjq.cn/Article/details/gfjoprphw.sHtML

smtplib.SMTP_SSL(...).send_message(msg)
来源：http://baike.fehbvm.com/Article/details/glvvxriei.sHtML

[U36] Py：定时任务
来源：http://baike.zdbjq.cn/Article/details/ggurwpynt.sHtML

schedule.every(10).minutes.do(job)
来源：http://read.share.hesvh.cn/Article/details/gxkwhlefs.sHtML

[U37] Py：读写 Excel
来源：http://www.blog.zdbjq.cn/Article/details/gxfzqcvbd.sHtML

pandas.read_excel / DataFrame.to_excel
来源：http://mobile.fehbvm.com/Article/details/goupsnwcj.sHtML

[U38] Py：获取脚本所在目录
来源：http://www.m.share.zdbjq.cn/Article/details/gcchtybep.sHtML

Path(__file__).resolve().parent
来源：http://www.m.share.hesvh.cn/Article/details/godcfzuwy.sHtML

[U39] Py：判断是否在交互环境
来源：http://baike.zdbjq.cn/Article/details/giqnkjdiq.sHtML

sys.stdout.isatty()
来源：http://3g.zdbjq.cn/Article/details/glzqkdbup.sHtML

[U40] Py：打印到标准错误
来源：http://read.share.zdbjq.cn/Article/details/gkwgbtpof.sHtML

print("err", file=sys.stderr)
来源：http://www.m.share.zdbjq.cn/Article/details/gxxdtkcli.sHtML

[U41] PHP：初始化 Composer 项目
来源：http://mobile.zdbjq.cn/Article/details/gijxnlolg.sHtML

composer init;  composer require guzzlehttp/guzzle
来源：http://3g.zdbjq.cn/Article/details/gkvbqbtez.sHtML

[U42] PHP：PSR-4 自动加载
来源：http://www.m.share.fehbvm.com/Article/details/gylgjjcqn.sHtML

"autoload": { "psr-4": { "App\\": "src/" } }
来源：http://3g.fehbvm.com/Article/details/gnxfhvwqe.sHtML

[U43] PHP：声明命名空间
来源：http://baike.zdbjq.cn/Article/details/gundedbjn.sHtML

namespace App\Http;
来源：http://www.share.fehbvm.com/Article/details/gskdejsfy.sHtML

[U44] PHP：开启严格类型
来源：http://wap.hesvh.cn/Article/details/gvdbmwcfy.sHtML

declare(strict_types=1);
来源：http://wap.fehbvm.com/Article/details/gvybpprky.sHtML

[U45] PHP：类型声明与返回类型
来源：http://blog.zdbjq.cn/Article/details/gynwdrmhm.sHtML

function add(int $a, int $b): int { return $a + $b; }
来源：http://read.share.hesvh.cn/Article/details/gthyiaigd.sHtML

[U46] PHP：可空类型
来源：http://3g.zdbjq.cn/Article/details/gikghpyvh.sHtML

?string $name = null
来源：http://www.share.zdbjq.cn/Article/details/ghgypdnms.sHtML

[U47] PHP：联合类型
来源：http://www.m.share.hesvh.cn/Article/details/gtkwwdnzu.sHtML

int|string $id
来源：http://m.share.hesvh.cn/Article/details/gjpdppsoq.sHtML

[U48] PHP：纯枚举
来源：http://m.share.hesvh.cn/Article/details/gtvvzaifm.sHtML

enum Status: string { case Active = "active"; case Off = "off"; }
来源：http://wap.fehbvm.com/Article/details/gvlnltstw.sHtML

[U49] PHP：只读属性
来源：http://www.blog.zdbjq.cn/Article/details/gvqdrcyia.sHtML

public readonly string $name
来源：http://3g.hesvh.cn/Article/details/gtmmubzdp.sHtML

[U50] PHP：构造器属性提升
来源：http://mobile.hesvh.cn/Article/details/gyahkhoim.sHtML

public function __construct(private int $id) {}
来源：http://read.share.fehbvm.com/Article/details/gdnbafibe.sHtML

[U51] PHP：数组解构
来源：http://www.blog.zdbjq.cn/Article/details/gioflpqfu.sHtML

[$a, $b] = $arr;
来源：http://www.m.share.hesvh.cn/Article/details/gdlqwvhmq.sHtML

[U52] PHP：箭头函数
来源：http://www.share.fehbvm.com/Article/details/gfmcfkbmu.sHtML

$double = fn($x) => $x * 2;
来源：http://read.share.zdbjq.cn/Article/details/gkiiuynuc.sHtML

[U53] PHP：空合并运算符
来源：http://wap.fehbvm.com/Article/details/gneegatln.sHtML

$v = $a ?? $b ?? "default";
来源：http://blog.zdbjq.cn/Article/details/gkmbytptn.sHtML

[U54] PHP：空安全调用
来源：http://www.m.share.hesvh.cn/Article/details/gnzfngzns.sHtML

$obj?->method()
来源：http://www.share.hesvh.cn/Article/details/gcwjvtnsh.sHtML

[U55] PHP：match 表达式
来源：http://www.blog.zdbjq.cn/Article/details/giaxqdwrh.sHtML

$s = match($x) { 1 => "一", default => "其他" };
来源：http://www.m.share.hesvh.cn/Article/details/gpygbedmj.sHtML

[U56] PHP：命名参数
来源：http://www.blog.fehbvm.com/Article/details/gkveiljlr.sHtML

f(a: 1, b: 2)
来源：http://www.m.share.hesvh.cn/Article/details/gzlxgxyyn.sHtML

[U57] PHP：字符串插值
来源：http://www.blog.hesvh.cn/Article/details/gsflkhcrc.sHtML

"值: {$a}"
来源：http://baike.zdbjq.cn/Article/details/gftsavwdu.sHtML

[U58] PHP：数组三件套
来源：http://www.share.zdbjq.cn/Article/details/gdxtwqvbi.sHtML

array_map($f, $a);  array_filter($a, $f);  array_reduce($a, $f, 0);
来源：http://www.share.fehbvm.com/Article/details/geqgoxgyl.sHtML

[U59] PHP：自定义排序
来源：http://www.blog.hesvh.cn/Article/details/gqbcdjtxg.sHtML

usort($arr, fn($a, $b) => $a["age"] <=> $b["age"]);
来源：http://blog.hesvh.cn/Article/details/ggjssaabt.sHtML

[U60] PHP：JSON 编解码
来源：http://www.share.zdbjq.cn/Article/details/grzeryanv.sHtML

json_encode($d, JSON_UNESCAPED_UNICODE);  json_decode($s, true);
来源：http://www.m.share.hesvh.cn/Article/details/glrdeuysy.sHtML

[U61] PHP：正则
来源：http://wap.hesvh.cn/Article/details/gjhhbztwq.sHtML

preg_match('/(\d+)/', $s, $m);  preg_replace('/\d+/', '#', $s);
来源：http://wap.fehbvm.com/Article/details/gxupfioug.sHtML

[U62] PHP：日期对象
来源：http://wap.zdbjq.cn/Article/details/gtngtnfcw.sHtML

(new DateTimeImmutable())->format("Y-m-d");
来源：http://www.m.share.fehbvm.com/Article/details/gtbiwoehx.sHtML

[U63] PHP：文件读写
来源：http://baike.zdbjq.cn/Article/details/gvnkcythh.sHtML

file_get_contents($f);  file_put_contents($f, $data);
来源：http://read.share.zdbjq.cn/Article/details/guebljmtq.sHtML

[U64] PHP：目录遍历
来源：http://www.m.share.hesvh.cn/Article/details/gmuzvpaio.sHtML

glob("dir/*.php");  scandir("dir");
来源：http://mobile.hesvh.cn/Article/details/gpqyjbgog.sHtML

[U65] PHP：会话
来源：http://3g.fehbvm.com/Article/details/gjqmqkwpw.sHtML

session_start();  $_SESSION["uid"] = 1;
来源：http://m.share.hesvh.cn/Article/details/guvbgugdi.sHtML

[U66] PHP：设置 Cookie
来源：http://wap.hesvh.cn/Article/details/gkhbafqar.sHtML

setcookie("token", $v, ["httponly" => true, "samesite" => "Lax"]);
来源：http://blog.hesvh.cn/Article/details/gqmoynsmx.sHtML

[U67] PHP：处理文件上传
来源：http://wap.hesvh.cn/Article/details/gwtscrlmx.sHtML

$_FILES["file"]["tmp_name"] 与 move_uploaded_file()
来源：http://www.share.hesvh.cn/Article/details/gvjqjtwux.sHtML

[U68] PHP：PDO 连接
来源：http://www.m.share.fehbvm.com/Article/details/gdwmutgxe.sHtML

$pdo = new PDO("mysql:host=localhost;dbname=app", "root", "");
来源：http://read.share.zdbjq.cn/Article/details/grnqsjfak.sHtML

[U69] PHP：PDO 预处理
来源：http://3g.fehbvm.com/Article/details/gsgwayfxp.sHtML

$stmt = $pdo->prepare("SELECT * FROM users WHERE id = ?");  $stmt->execute([$id]);
来源：http://mobile.fehbvm.com/Article/details/ganbcwkty.sHtML

[U70] PHP：PDO 事务
来源：http://mobile.hesvh.cn/Article/details/gtnzljlnh.sHtML

$pdo->beginTransaction();  $pdo->commit();  $pdo->rollBack();
来源：http://3g.zdbjq.cn/Article/details/gysyjgsyl.sHtML

[U71] PHP：抛出异常
来源：http://blog.fehbvm.com/Article/details/gftjtynrl.sHtML

throw new RuntimeException("失败", 500);
来源：http://baike.zdbjq.cn/Article/details/gvrqstntc.sHtML

[U72] PHP：写错误日志
来源：http://www.share.zdbjq.cn/Article/details/gmzqaktft.sHtML

error_log("失败: " . $e->getMessage());
来源：http://read.share.zdbjq.cn/Article/details/glnubxtmv.sHtML

[U73] PHP：读取 ini 配置
来源：http://read.share.hesvh.cn/Article/details/gixqwyoro.sHtML

parse_ini_file("config.ini", true)
来源：http://www.blog.hesvh.cn/Article/details/gdbwxmfnl.sHtML

[U74] PHP：读取环境变量
来源：http://blog.hesvh.cn/Article/details/gqoagmgpz.sHtML

getenv("APP_ENV") ?: "production"
来源：http://wap.hesvh.cn/Article/details/gdpgacwaq.sHtML

[U75] PHP：依赖注入
来源：http://www.blog.fehbvm.com/Article/details/gubrterxf.sHtML

composer require psr/container
来源：http://m.share.hesvh.cn/Article/details/gymdtwmkf.sHtML

[U76] PHP：简单路由
来源：http://baike.fehbvm.com/Article/details/giuafhteb.sHtML

$path = parse_url($_SERVER["REQUEST_URI"], PHP_URL_PATH);
来源：http://blog.fehbvm.com/Article/details/grntomijd.sHtML

[U77] PHP：模板渲染
来源：http://mobile.zdbjq.cn/Article/details/ggblotnka.sHtML

composer require twig/twig
来源：http://blog.zdbjq.cn/Article/details/gkgivldlb.sHtML

[U78] PHP：单元测试
来源：http://baike.zdbjq.cn/Article/details/gadvzomxl.sHtML

composer require --dev phpunit/phpunit
来源：http://www.m.share.fehbvm.com/Article/details/gajqjitoi.sHtML

[U79] PHP：静态分析
来源：http://www.share.hesvh.cn/Article/details/gfkealzvt.sHtML

composer require --dev phpstan/phpstan
来源：http://wap.hesvh.cn/Article/details/glphnimuw.sHtML

[U80] PHP：代码规范修复
来源：http://www.blog.hesvh.cn/Article/details/gvyrzfaxr.sHtML

composer require --dev friendsofphp/php-cs-fixer
来源：http://www.m.share.hesvh.cn/Article/details/gporsrhia.sHtML

[U81] JS：初始化项目
来源：http://baike.hesvh.cn/Article/details/gcpzxqyfp.sHtML

npm init -y;  npm i express
来源：http://mobile.fehbvm.com/Article/details/guahqqpps.sHtML

[U82] JS：package.json 脚本
来源：http://www.share.fehbvm.com/Article/details/gghyahhtg.sHtML

"scripts": { "dev": "vite", "build": "vite build" }
来源：http://baike.fehbvm.com/Article/details/grffrskll.sHtML

[U83] JS：ES Module 导入导出
来源：http://3g.hesvh.cn/Article/details/gdqfwhgph.sHtML

export const a = 1;  import { a } from "./m.js";
来源：http://wap.fehbvm.com/Article/details/gffzvkftf.sHtML

[U84] JS：CommonJS 写法
来源：http://3g.hesvh.cn/Article/details/gwckccbvz.sHtML

module.exports = { a };  const { a } = require("./m");
来源：http://baike.hesvh.cn/Article/details/gmbdfpeod.sHtML

[U85] JS：可选链
来源：http://www.m.share.fehbvm.com/Article/details/gpviaifoa.sHtML

a?.b?.c
来源：http://read.share.hesvh.cn/Article/details/getaeyyiu.sHtML

[U86] JS：空值合并
来源：http://wap.zdbjq.cn/Article/details/gmuwlgcgp.sHtML

a ?? b
来源：http://3g.fehbvm.com/Article/details/ggkbwteed.sHtML

[U87] JS：解构默认值
来源：http://www.blog.zdbjq.cn/Article/details/gxkooopfn.sHtML

const { a = 1, b = 2 } = obj;
来源：http://m.share.hesvh.cn/Article/details/gvwxvvplv.sHtML

[U88] JS：对象展开合并
来源：http://www.share.hesvh.cn/Article/details/grzdycbcq.sHtML

{ ...a, ...b }
来源：http://www.blog.zdbjq.cn/Article/details/gbrwfzvyp.sHtML

[U89] JS：数组去重
来源：http://www.share.hesvh.cn/Article/details/gklbbxmjr.sHtML

[...new Set(arr)]
来源：http://www.share.fehbvm.com/Article/details/gfhlskmub.sHtML

[U90] JS：数字数组排序
来源：http://wap.zdbjq.cn/Article/details/gdddldvdm.sHtML

[...arr].sort((a, b) => a - b)
来源：http://m.share.fehbvm.com/Article/details/gtjnzhall.sHtML

[U91] JS：对象键值遍历
来源：http://baike.hesvh.cn/Article/details/gukahmuda.sHtML

Object.entries(obj).forEach(([k, v]) => {});
来源：http://wap.fehbvm.com/Article/details/gffdlfaur.sHtML

[U92] JS：深拷贝
来源：http://wap.zdbjq.cn/Article/details/grtylagtv.sHtML

structuredClone(obj)
来源：http://baike.zdbjq.cn/Article/details/gfevrpbir.sHtML

[U93] JS：模板字符串
来源：http://www.m.share.fehbvm.com/Article/details/gwrrlqxsw.sHtML

`共 ${n} 条`
来源：http://mobile.zdbjq.cn/Article/details/gpjefqygj.sHtML

[U94] JS：箭头函数
来源：http://baike.hesvh.cn/Article/details/gnxcouhnb.sHtML

const double = x => x * 2;
来源：http://3g.fehbvm.com/Article/details/gsrgtjklm.sHtML

[U95] JS：Promise 包装
来源：http://m.share.fehbvm.com/Article/details/gujrndimy.sHtML

new Promise((resolve, reject) => {})
来源：http://www.blog.zdbjq.cn/Article/details/gnibqigtq.sHtML

[U96] JS：async/await 与异常
来源：http://read.share.zdbjq.cn/Article/details/gbjjjfhfg.sHtML

try { const d = await f(); } catch (e) { console.error(e); }
来源：http://www.blog.fehbvm.com/Article/details/gczqwllyj.sHtML

[U97] JS：并发请求
来源：http://wap.hesvh.cn/Article/details/gsxlkhjzu.sHtML

await Promise.all(urls.map(u => fetch(u)))
来源：http://mobile.zdbjq.cn/Article/details/gqcxjluew.sHtML

[U98] JS：fetch 带 JSON
来源：http://m.share.zdbjq.cn/Article/details/godtnejwr.sHtML

await fetch(url, { method: "POST", headers: { "Content-Type": "application/json" }, body: JSON.stringify(d) })
来源：http://blog.zdbjq.cn/Article/details/gmfjgajnx.sHtML

[U99] JS：事件监听
来源：http://read.share.zdbjq.cn/Article/details/gyuuowbcw.sHtML

el.addEventListener("click", e => {})
来源：http://mobile.hesvh.cn/Article/details/gtfqheltu.sHtML

[U100] JS：DOM 查询
来源：http://baike.zdbjq.cn/Article/details/gxwottxcw.sHtML

document.querySelector(".item")
来源：http://www.m.share.zdbjq.cn/Article/details/gmnwrxosb.sHtML

[U101] JS：classList 操作
来源：http://www.share.zdbjq.cn/Article/details/gqzlqcibo.sHtML

el.classList.toggle("active")
来源：http://www.m.share.fehbvm.com/Article/details/gpjaisixm.sHtML

[U102] JS：本地存储
来源：http://m.share.zdbjq.cn/Article/details/gmrfrhbhj.sHtML

localStorage.setItem("k", JSON.stringify(v))
来源：http://wap.hesvh.cn/Article/details/gbbhwmbha.sHtML

[U103] JS：定时器
来源：http://www.blog.zdbjq.cn/Article/details/gcsrsaikz.sHtML

setTimeout(fn, 1000);  setInterval(fn, 1000);
来源：http://blog.hesvh.cn/Article/details/gfcvhydmg.sHtML

[U104] JS：防抖
来源：http://baike.zdbjq.cn/Article/details/ghyfphsas.sHtML

const debounce = (fn, ms) => { let t; return (...a) => { clearTimeout(t); t = setTimeout(() => fn(...a), ms); }; };
来源：http://read.share.zdbjq.cn/Article/details/gcpnkuvuf.sHtML

[U105] JS：节流
来源：http://3g.zdbjq.cn/Article/details/ghpvkuivc.sHtML

const throttle = (fn, ms) => { let last = 0; return (...a) => { const n = Date.now(); if (n - last >= ms) { last = n; fn(...a); } }; };
来源：http://www.blog.hesvh.cn/Article/details/gmrfnasld.sHtML

[U106] JS：日期格式化
来源：http://wap.zdbjq.cn/Article/details/gurrjevqp.sHtML

new Intl.DateTimeFormat("zh-CN", { dateStyle: "medium" }).format(new Date())
来源：http://www.share.hesvh.cn/Article/details/grleqrgrq.sHtML

[U107] JS：数字千分位
来源：http://www.blog.hesvh.cn/Article/details/gftmvazrv.sHtML

new Intl.NumberFormat("en-US").format(1234567)
来源：http://3g.zdbjq.cn/Article/details/gkfzvehsc.sHtML

[U108] JS：随机整数
来源：http://www.m.share.zdbjq.cn/Article/details/gdigguxtj.sHtML

Math.floor(Math.random() * (max - min + 1)) + min
来源：http://www.blog.hesvh.cn/Article/details/gnkynknpy.sHtML

[U109] JS：数组分组
来源：http://blog.hesvh.cn/Article/details/gswjvmbgv.sHtML

Object.groupBy(arr, x => x.type)
来源：http://baike.fehbvm.com/Article/details/gbjbuksqp.sHtML

[U110] JS：数组分块
来源：http://baike.zdbjq.cn/Article/details/gtpuamcrz.sHtML

arr.reduce((acc, x, i) => (i % size ? acc : [...acc, arr.slice(i, i + size)]), [])
来源：http://3g.hesvh.cn/Article/details/gtcswcbzo.sHtML

[U111] JS：对象转 Map
来源：http://www.m.share.fehbvm.com/Article/details/girlveafp.sHtML

new Map(Object.entries(obj))
来源：http://mobile.zdbjq.cn/Article/details/gitmemobe.sHtML

[U112] JS：字符串补位
来源：http://mobile.hesvh.cn/Article/details/gelaryhpi.sHtML

"7".padStart(3, "0")
来源：http://blog.fehbvm.com/Article/details/guhjwjtsp.sHtML

[U113] JS：正则替换全部
来源：http://mobile.fehbvm.com/Article/details/gmrgmpshq.sHtML

s.replaceAll("a", "b")
来源：http://read.share.zdbjq.cn/Article/details/girgrngfy.sHtML

[U114] JS：JSON 深比较
来源：http://3g.fehbvm.com/Article/details/gmhhrfqnz.sHtML

JSON.stringify(a) === JSON.stringify(b)
来源：http://3g.fehbvm.com/Article/details/gvyfatycf.sHtML

[U115] JS：生成 UUID
来源：http://3g.fehbvm.com/Article/details/gtwcdgxlw.sHtML

crypto.randomUUID()
来源：http://m.share.fehbvm.com/Article/details/gcvxcmlvu.sHtML

[U116] JS：类型检查（JSDoc）
来源：http://www.blog.fehbvm.com/Article/details/goucixldy.sHtML

/** @param {string} name */ function f(name) {}
来源：http://m.share.hesvh.cn/Article/details/gqkohvvqf.sHtML

[U117] JS：单元测试
来源：http://read.share.fehbvm.com/Article/details/ghaknihim.sHtML

npm i -D vitest;  npx vitest
来源：http://baike.hesvh.cn/Article/details/gefhrrvef.sHtML

[U118] JS：开发服务器
来源：http://www.m.share.hesvh.cn/Article/details/gjpuqzstu.sHtML

npm i -D vite;  npx vite
来源：http://m.share.hesvh.cn/Article/details/gxfouzuma.sHtML

[U119] JS：生产构建
来源：http://www.m.share.fehbvm.com/Article/details/gduhfphsv.sHtML

npx vite build
来源：http://www.blog.zdbjq.cn/Article/details/gmvgnjckd.sHtML

[U120] JS：读取环境变量（Vite）
来源：http://blog.hesvh.cn/Article/details/gloewpwdv.sHtML

import.meta.env.VITE_API_URL
来源：http://baike.zdbjq.cn/Article/details/gjjguevbz.sHtML

================================================================================
来源：http://www.blog.fehbvm.com/Article/details/grktoupfo.sHtML

统计汇总
来源：http://3g.zdbjq.cn/Article/details/gwtjybdqe.sHtML

================================================================================
来源：http://m.share.hesvh.cn/Article/details/gmhtbufdf.sHtML

按语言统计（条）：
来源：http://m.share.hesvh.cn/Article/details/gmsorpebj.sHtML

Python ......... 252
来源：http://www.m.share.hesvh.cn/Article/details/gdppcyomg.sHtML

PHP ............ 252
来源：http://m.share.hesvh.cn/Article/details/gdvrdjwqd.sHtML

JavaScript ..... 252
来源：http://baike.hesvh.cn/Article/details/gfsvbrhss.sHtML

TypeScript ..... 212
来源：http://m.share.fehbvm.com/Article/details/gekltbpes.sHtML

Java ........... 212
来源：http://m.share.hesvh.cn/Article/details/gfjlmclds.sHtML

Go ............. 212
来源：http://baike.hesvh.cn/Article/details/goclxohhs.sHtML

Ruby ........... 212
来源：http://m.share.hesvh.cn/Article/details/giuucvekd.sHtML

C# ............. 212
来源：http://blog.fehbvm.com/Article/details/gzspvpkji.sHtML

C .............. 30
来源：http://www.share.fehbvm.com/Article/details/gkxwkvfqt.sHtML

C++ ............ 30
来源：http://baike.fehbvm.com/Article/details/gxcxvfbvb.sHtML

SQL ............ 90
来源：http://www.m.share.hesvh.cn/Article/details/gripkkvjh.sHtML

Bash ........... 80
来源：http://wap.hesvh.cn/Article/details/gvrrtkhti.sHtML

Kotlin ......... 15
来源：http://read.share.zdbjq.cn/Article/details/gcaeayrbl.sHtML

Swift .......... 15
来源：http://read.share.zdbjq.cn/Article/details/gomffvvdj.sHtML

Lua ............ 10
来源：http://wap.hesvh.cn/Article/details/gapsonqas.sHtML

Perl ........... 10
来源：http://baike.fehbvm.com/Article/details/guauatpuo.sHtML

Scala .......... 10
来源：http://wap.hesvh.cn/Article/details/gwckkvofy.sHtML

------------------------------------
来源：http://m.share.hesvh.cn/Article/details/ggafsmjms.sHtML

合计 ........... 2106 条
来源：http://blog.fehbvm.com/Article/details/glekryqmu.sHtML

按章节统计：
来源：http://read.share.hesvh.cn/Article/details/giauiqbgc.sHtML

A 基础语法与类型       26 个任务 × 8 语言 =  208
来源：http://www.share.hesvh.cn/Article/details/gzyzjrbfv.sHtML

B 流程控制             16 个任务 × 8 语言 =  128
来源：http://blog.zdbjq.cn/Article/details/gqprkbrdd.sHtML

C 函数与作用域         16 个任务 × 8 语言 =  128
来源：http://read.share.fehbvm.com/Article/details/gdykhfoyq.sHtML

D 数组 / 列表 / 集合   26 个任务 × 8 语言 =  208
来源：http://wap.zdbjq.cn/Article/details/gceamrnie.sHtML

E 字符串处理           22 个任务 × 8 语言 =  176
来源：http://m.share.zdbjq.cn/Article/details/ghvjdodfz.sHtML

F 文件与目录           12 个任务 × 8 语言 =   96
来源：http://mobile.fehbvm.com/Article/details/gkucdrevo.sHtML

G 面向对象             16 个任务 × 8 语言 =  128
来源：http://baike.zdbjq.cn/Article/details/gltyplgdc.sHtML

H 异常与错误处理       10 个任务 × 8 语言 =   80
来源：http://blog.hesvh.cn/Article/details/ggvczpfml.sHtML

I 正则表达式            8 个任务 × 8 语言 =   64
来源：http://baike.fehbvm.com/Article/details/gjpzbhayw.sHtML

J 日期与时间           10 个任务 × 8 语言 =   80
来源：http://blog.zdbjq.cn/Article/details/gojrklpds.sHtML

K JSON 与序列化         8 个任务 × 8 语言 =   64
来源：http://3g.hesvh.cn/Article/details/ggunfgapy.sHtML

L 网络请求              8 个任务 × 8 语言 =   64
来源：http://read.share.fehbvm.com/Article/details/gcmngnano.sHtML

M 命令行 / 进程         8 个任务 × 8 语言 =   64
来源：http://read.share.hesvh.cn/Article/details/gjupbzjkt.sHtML

N 数据结构与算法       12 个任务 × 8 语言 =   96
来源：http://www.m.share.hesvh.cn/Article/details/gnsyqedrr.sHtML

O 并发与异步            6 个任务 × 8 语言 =   48
来源：http://wap.hesvh.cn/Article/details/gfngorwwf.sHtML

P 常用工具函数          8 个任务 × 8 语言 =   64
来源：http://baike.zdbjq.cn/Article/details/gazyxozat.sHtML

Q SQL 专题                              90
来源：http://m.share.fehbvm.com/Article/details/ggpsjhgqg.sHtML

R Bash 专题                             80
来源：http://www.m.share.zdbjq.cn/Article/details/gwkgzynbj.sHtML

S C / C++ 专题                          60
来源：http://mobile.zdbjq.cn/Article/details/gxnsqwkgw.sHtML

T 其他语言补充                          60
来源：http://3g.fehbvm.com/Article/details/gajsvunwz.sHtML

U 高频实用片段                         120
来源：http://www.m.share.fehbvm.com/Article/details/gqirjeqds.sHtML

------------------------------------
来源：http://baike.zdbjq.cn/Article/details/gbdttaish.sHtML

合计                                  2106 条
来源：http://3g.zdbjq.cn/Article/details/gqudijtmg.sHtML

--------------------------------------------------------------------------------
来源：http://wap.zdbjq.cn/Article/details/gndmywgdg.sHtML

使用提醒
来源：http://blog.fehbvm.com/Article/details/gilbiyedt.sHtML

--------------------------------------------------------------------------------
来源：http://baike.zdbjq.cn/Article/details/gzxboulhs.sHtML

1. 示例追求"最小可用"，正式项目中请补齐导入、错误处理与边界判断。
来源：http://blog.fehbvm.com/Article/details/gvqpjatmh.sHtML

2. 涉及文件、网络、数据库的示例，注意资源释放与异常捕获。
来源：http://3g.hesvh.cn/Article/details/gisxxixey.sHtML

3. 语言版本差异较大（如 Python 3.10 的 match、Java 17 的 record/switch 箭头），
来源：http://wap.hesvh.cn/Article/details/ggunkgffu.sHtML

在旧版本上使用前请先确认语法支持情况。
来源：http://www.m.share.hesvh.cn/Article/details/gzacmxgcn.sHtML

4. 标注"手写"的条目是因为该语言缺少对应内置能力，实际项目中可引入成熟库。
来源：http://read.share.zdbjq.cn/Article/details/grvwlrhms.sHtML

—— 文件结束 ——
来源：http://m.share.fehbvm.com/Article/details/gwrfljmgt.sHtML

================================================================================
来源：http://mobile.hesvh.cn/Article/details/glowwiwpg.sHtML

程序语言常见例子速查手册（2024 版）
来源：http://m.share.zdbjq.cn/Article/details/grdpxgura.sHtML

Common Programming Examples Cheat Book
来源：http://www.share.hesvh.cn/Article/details/giletusve.sHtML

================================================================================
来源：http://m.share.zdbjq.cn/Article/details/gvovtkmos.sHtML

【收录内容】
来源：http://m.share.zdbjq.cn/Article/details/ggkyuvvdm.sHtML

覆盖 12 种语言 / 语法与常见 API：
来源：http://read.share.fehbvm.com/Article/details/ggukpnlkr.sHtML

Python · PHP · JavaScript · TypeScript · Java · Go · Ruby · C#
来源：http://www.m.share.fehbvm.com/Article/details/gjrthbgey.sHtML

SQL · Bash · C · C++
来源：http://blog.fehbvm.com/Article/details/gfteugrwu.sHtML

按「任务」分组：每个任务下按语言各给出一条最小可用示例。
来源：http://www.m.share.fehbvm.com/Article/details/ghaoicifa.sHtML

【使用说明】
来源：http://www.share.fehbvm.com/Article/details/glfhmthrh.sHtML

1. 每个任务形如 "[编号] 任务名"，下面每行以语言标记开头：
来源：http://mobile.zdbjq.cn/Article/details/gxtbpkhik.sHtML

Py:    Python        PHP:   PHP           JS:    JavaScript
来源：http://m.share.fehbvm.com/Article/details/gfmhmmvxu.sHtML

TS:    TypeScript    Java:  Java          Go:    Go
来源：http://m.share.fehbvm.com/Article/details/guudkbawd.sHtML

Ruby:  Ruby          C#:    C#            SQL:   SQL
来源：http://3g.fehbvm.com/Article/details/gmyeksuik.sHtML

Bash:  Shell         C:     C             C++:   C++
来源：http://wap.fehbvm.com/Article/details/goraaxise.sHtML

2. 示例只展示核心写法，刻意省略 import / require / include / using 等样板代码。
来源：http://baike.zdbjq.cn/Article/details/gxbixjzup.sHtML

需要完整可运行文件时，请自行补齐当前语言的导入语句。
来源：http://blog.fehbvm.com/Article/details/gwxtxzgwv.sHtML

3. 语法基准：Python 3.10+ / PHP 8.1+ / ES2020+ / TypeScript 5 / Java 17 /
来源：http://blog.hesvh.cn/Article/details/gibsraube.sHtML

Go 1.21+ / Ruby 3.x / C# 10+ / C17 / C++17。
来源：http://www.m.share.zdbjq.cn/Article/details/gsebzkcmo.sHtML

4. 检索建议：用编辑器或浏览器 Ctrl+F 搜关键词，如 "排序" "读取文件" "正则"。
来源：http://3g.zdbjq.cn/Article/details/gnttrkmum.sHtML

5. 标记为 "// 无" 表示该语言没有对应的一等语法，需用替代写法（示例给出替代方案）。
来源：http://www.share.hesvh.cn/Article/details/gppmpquyf.sHtML

6. 符号 "⏎" 表示代码在此处换行（主要用于 Python 等强制缩进、无法压成一行的结构）。
来源：http://mobile.zdbjq.cn/Article/details/gqzrtqqtl.sHtML

【文件统计】
来源：http://www.share.fehbvm.com/Article/details/ghhkwlbpq.sHtML

语言示例共 2106 条，分布见本文末尾的「统计汇总」。
来源：http://3g.hesvh.cn/Article/details/gpkyriudi.sHtML

--------------------------------------------------------------------------------
来源：http://www.blog.fehbvm.com/Article/details/gypfkyhuw.sHtML

目  录
来源：http://www.blog.hesvh.cn/Article/details/greskvfhe.sHtML

--------------------------------------------------------------------------------
来源：http://www.blog.fehbvm.com/Article/details/grrdxsuvn.sHtML

A. 基础语法与类型              （第 1 节，26 个任务，208 条）
来源：http://wap.fehbvm.com/Article/details/gxvtuqpcj.sHtML

B. 流程控制                    （第 2 节，16 个任务，128 条）
来源：http://m.share.zdbjq.cn/Article/details/ghqscjrnu.sHtML

C. 函数与作用域                （第 3 节，16 个任务，128 条）
来源：http://blog.zdbjq.cn/Article/details/giwxwiwxs.sHtML

D. 数组 / 列表 / 集合          （第 4 节，26 个任务，208 条）
来源：http://mobile.zdbjq.cn/Article/details/gcvdewzai.sHtML

E. 字符串处理                  （第 5 节，22 个任务，176 条）
来源：http://baike.fehbvm.com/Article/details/gqgjacfqs.sHtML

F. 文件与目录                  （第 6 节，12 个任务，96 条）
来源：http://www.blog.hesvh.cn/Article/details/gzzvczysi.sHtML

G. 面向对象                    （第 7 节，16 个任务，128 条）
来源：http://mobile.zdbjq.cn/Article/details/gnsaqciec.sHtML

H. 异常与错误处理              （第 8 节，10 个任务，80 条）
来源：http://read.share.fehbvm.com/Article/details/gckdxshgr.sHtML

I. 正则表达式                  （第 9 节，8 个任务，64 条）
来源：http://read.share.zdbjq.cn/Article/details/gitubmdyh.sHtML

J. 日期与时间                  （第 10 节，10 个任务，80 条）
来源：http://3g.fehbvm.com/Article/details/gkzpxuxdv.sHtML

K. JSON 与序列化               （第 11 节，8 个任务，64 条）
来源：http://read.share.fehbvm.com/Article/details/gyxshzdom.sHtML

L. 网络请求                    （第 12 节，8 个任务，64 条）
来源：http://www.share.hesvh.cn/Article/details/gbiuynnos.sHtML

M. 命令行 / 进程 / 环境        （第 13 节，8 个任务，64 条）
来源：http://www.blog.fehbvm.com/Article/details/gwgwtaxth.sHtML

N. 数据结构与算法              （第 14 节，12 个任务，96 条）
来源：http://wap.hesvh.cn/Article/details/gdkgwkjfd.sHtML

O. 并发与异步                  （第 15 节，6 个任务，48 条）
来源：http://mobile.fehbvm.com/Article/details/gpomwdlqg.sHtML

P. 常用工具函数                （第 16 节，8 个任务，64 条）
来源：http://www.share.zdbjq.cn/Article/details/ggnidoekl.sHtML

Q. SQL 专题                    （第 17 节，90 条）
来源：http://read.share.fehbvm.com/Article/details/genvixvdo.sHtML

R. Bash 专题                   （第 18 节，80 条）
来源：http://3g.hesvh.cn/Article/details/gensxctvm.sHtML

S. C / C++ 专题                （第 19 节，60 条）
来源：http://www.share.zdbjq.cn/Article/details/guiaaiqcq.sHtML

T. 其他语言补充                （第 20 节，60 条：Kotlin / Swift / Lua / Perl / Scala）
来源：http://baike.fehbvm.com/Article/details/gburtzlcb.sHtML

U. 高频实用片段                （第 21 节，120 条：Python / PHP / JavaScript 各 40 条）
来源：http://read.share.zdbjq.cn/Article/details/gmkfnpmnu.sHtML

================================================================================
来源：http://baike.fehbvm.com/Article/details/ghtqynqho.sHtML

A. 基础语法与类型
来源：http://read.share.hesvh.cn/Article/details/gsikczrhu.sHtML

================================================================================
来源：http://read.share.hesvh.cn/Article/details/gpzbgdjkd.sHtML

[A01] Hello World
来源：http://baike.hesvh.cn/Article/details/gfeapxrro.sHtML

Py:   print("Hello, World!")
来源：http://baike.hesvh.cn/Article/details/goyoikzch.sHtML

PHP:  echo "Hello, World!";
来源：http://read.share.fehbvm.com/Article/details/gjkxvkibu.sHtML

JS:   console.log("Hello, World!");
来源：http://mobile.zdbjq.cn/Article/details/ggibwkqbr.sHtML

TS:   const msg: string = "Hello, World!"; console.log(msg);
来源：http://baike.fehbvm.com/Article/details/gsggvlkli.sHtML

Java: System.out.println("Hello, World!");
来源：http://baike.fehbvm.com/Article/details/gtdavutyh.sHtML

Go:   fmt.Println("Hello, World!")
来源：http://blog.fehbvm.com/Article/details/gfmqrrzkt.sHtML

Ruby: puts "Hello, World!"
来源：http://www.blog.zdbjq.cn/Article/details/gdlaiobtx.sHtML

C#:   Console.WriteLine("Hello, World!");
来源：http://wap.fehbvm.com/Article/details/gbdxksxue.sHtML

[A02] 变量声明与赋值
来源：http://wap.fehbvm.com/Article/details/gomowwfij.sHtML

Py:   name = "Alex"; age = 20            # 动态类型，无需声明
来源：http://mobile.fehbvm.com/Article/details/gzaplbpzg.sHtML

PHP:  $name = "Alex"; $age = 20;
来源：http://www.m.share.zdbjq.cn/Article/details/gqgvrdcps.sHtML

JS:   let name = "Alex"; const age = 20;
来源：http://blog.hesvh.cn/Article/details/gdjahukfy.sHtML

TS:   let name: string = "Alex"; const age: number = 20;
来源：http://m.share.fehbvm.com/Article/details/gfdxmpzgj.sHtML

Java: String name = "Alex"; int age = 20;
来源：http://blog.fehbvm.com/Article/details/gkbnemqpx.sHtML

Go:   name := "Alex"; age := 20
来源：http://baike.zdbjq.cn/Article/details/gytjgmyrd.sHtML

Ruby: name = "Alex"; age = 20
来源：http://read.share.fehbvm.com/Article/details/gysyqajal.sHtML


<!-- 参考信息 -->