代发 wailian999

[U33] Py：打包发布
来源：http://www.blog.fanxiaobao.xyz/Article/details/geumdpaun.sHtML

python -m build  （依赖 pyproject.toml）
来源：http://m.share.fanxiaobao.xyz/Article/details/gxvnauqjh.sHtML

[U34] Py：判断编码
来源：http://wap.fanxiaobao.xyz/Article/details/gvtkcttly.sHtML

chardet.detect(raw)
来源：http://baike.fanxiaobao.xyz/Article/details/gmswifuya.sHtML

[U35] Py：发送邮件
来源：http://baike.fanxiaobao.xyz/Article/details/gqmjpbbvx.sHtML

smtplib.SMTP_SSL(...).send_message(msg)
来源：http://wap.fanxiaobao.xyz/Article/details/guxndfluw.sHtML

[U36] Py：定时任务
来源：http://blog.fanxiaobao.xyz/Article/details/gbasyagtm.sHtML

schedule.every(10).minutes.do(job)
来源：http://mobile.fanxiaobao.xyz/Article/details/glmjnxrxc.sHtML

[U37] Py：读写 Excel
来源：http://wap.fanxiaobao.xyz/Article/details/guthtyafb.sHtML

pandas.read_excel / DataFrame.to_excel
来源：http://read.share.fanxiaobao.xyz/Article/details/govmjzmir.sHtML

[U38] Py：获取脚本所在目录
来源：http://3g.fanxiaobao.xyz/Article/details/ggtghhqhw.sHtML

Path(__file__).resolve().parent
来源：http://blog.fanxiaobao.xyz/Article/details/gypfutkrb.sHtML

[U39] Py：判断是否在交互环境
来源：http://wap.fanxiaobao.xyz/Article/details/gyapnwgfq.sHtML

sys.stdout.isatty()
来源：http://www.share.fanxiaobao.xyz/Article/details/gvankbvks.sHtML

[U40] Py：打印到标准错误
来源：http://baike.fanxiaobao.xyz/Article/details/gsehgvhty.sHtML

print("err", file=sys.stderr)
来源：http://www.share.fanxiaobao.xyz/Article/details/gdmhdveip.sHtML

[U41] PHP：初始化 Composer 项目
来源：http://baike.fanxiaobao.xyz/Article/details/gjobxyznh.sHtML

composer init;  composer require guzzlehttp/guzzle
来源：http://m.share.fanxiaobao.xyz/Article/details/gwoqghfyq.sHtML

[U42] PHP：PSR-4 自动加载
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gyzbiqspf.sHtML

"autoload": { "psr-4": { "App\\": "src/" } }
来源：http://www.m.share.fanxiaobao.xyz/Article/details/ghduuqpxy.sHtML

[U43] PHP：声明命名空间
来源：http://www.blog.fanxiaobao.xyz/Article/details/giamaqvlr.sHtML

namespace App\Http;
来源：http://www.share.fanxiaobao.xyz/Article/details/gfdvfdult.sHtML

[U44] PHP：开启严格类型
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gqyqymtfb.sHtML

declare(strict_types=1);
来源：http://wap.fanxiaobao.xyz/Article/details/gfbfvlrvt.sHtML

[U45] PHP：类型声明与返回类型
来源：http://wap.fanxiaobao.xyz/Article/details/gwjmyglfs.sHtML

function add(int $a, int $b): int { return $a + $b; }
来源：http://www.share.fanxiaobao.xyz/Article/details/gmhvjyroi.sHtML

[U46] PHP：可空类型
来源：http://www.blog.fanxiaobao.xyz/Article/details/grajdvtcf.sHtML

?string $name = null
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gmjdugyzd.sHtML

[U47] PHP：联合类型
来源：http://baike.fanxiaobao.xyz/Article/details/gndpeqrzl.sHtML

int|string $id
来源：http://read.share.fanxiaobao.xyz/Article/details/gfllnklli.sHtML

[U48] PHP：纯枚举
来源：http://mobile.fanxiaobao.xyz/Article/details/glwpaichl.sHtML

enum Status: string { case Active = "active"; case Off = "off"; }
来源：http://mobile.fanxiaobao.xyz/Article/details/guijwetop.sHtML

[U49] PHP：只读属性
来源：http://blog.fanxiaobao.xyz/Article/details/gjfwyajpu.sHtML

public readonly string $name
来源：http://m.share.fanxiaobao.xyz/Article/details/gicivvgkk.sHtML

[U50] PHP：构造器属性提升
来源：http://mobile.fanxiaobao.xyz/Article/details/ggznofhfy.sHtML

public function __construct(private int $id) {}
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gvmandplf.sHtML

[U51] PHP：数组解构
来源：http://3g.fanxiaobao.xyz/Article/details/gnedhlkjw.sHtML

[$a, $b] = $arr;
来源：http://baike.fanxiaobao.xyz/Article/details/ghmxojtky.sHtML

[U52] PHP：箭头函数
来源：http://www.blog.fanxiaobao.xyz/Article/details/gmnxclqae.sHtML

$double = fn($x) => $x * 2;
来源：http://m.share.fanxiaobao.xyz/Article/details/gobilvppa.sHtML

[U53] PHP：空合并运算符
来源：http://m.share.fanxiaobao.xyz/Article/details/gyygjhrnw.sHtML

$v = $a ?? $b ?? "default";
来源：http://read.share.fanxiaobao.xyz/Article/details/gnbhenhsc.sHtML

[U54] PHP：空安全调用
来源：http://mobile.fanxiaobao.xyz/Article/details/gwjecynqb.sHtML

$obj?->method()
来源：http://blog.fanxiaobao.xyz/Article/details/gbdsjefjt.sHtML

[U55] PHP：match 表达式
来源：http://3g.fanxiaobao.xyz/Article/details/gvklrgzco.sHtML

$s = match($x) { 1 => "一", default => "其他" };
来源：http://www.share.fanxiaobao.xyz/Article/details/gduzbnbyp.sHtML

[U56] PHP：命名参数
来源：http://www.share.fanxiaobao.xyz/Article/details/gmpranubq.sHtML

f(a: 1, b: 2)
来源：http://www.m.share.fanxiaobao.xyz/Article/details/ggakfblsn.sHtML

[U57] PHP：字符串插值
来源：http://baike.fanxiaobao.xyz/Article/details/gkeihqjmi.sHtML

"值: {$a}"
来源：http://baike.fanxiaobao.xyz/Article/details/gyovhiouu.sHtML

[U58] PHP：数组三件套
来源：http://blog.fanxiaobao.xyz/Article/details/ggkkvrslt.sHtML

array_map($f, $a);  array_filter($a, $f);  array_reduce($a, $f, 0);
来源：http://www.share.fanxiaobao.xyz/Article/details/gtuaimgrc.sHtML

[U59] PHP：自定义排序
来源：http://mobile.fanxiaobao.xyz/Article/details/gphjpagbo.sHtML

usort($arr, fn($a, $b) => $a["age"] <=> $b["age"]);
来源：http://m.share.fanxiaobao.xyz/Article/details/gbhvngnqc.sHtML

[U60] PHP：JSON 编解码
来源：http://www.share.fanxiaobao.xyz/Article/details/gewdggwyj.sHtML

json_encode($d, JSON_UNESCAPED_UNICODE);  json_decode($s, true);
来源：http://3g.fanxiaobao.xyz/Article/details/gdvuibngs.sHtML

[U61] PHP：正则
来源：http://www.blog.fanxiaobao.xyz/Article/details/gtltwzxpt.sHtML

preg_match('/(\d+)/', $s, $m);  preg_replace('/\d+/', '#', $s);
来源：http://mobile.fanxiaobao.xyz/Article/details/gopclqiga.sHtML

[U62] PHP：日期对象
来源：http://read.share.fanxiaobao.xyz/Article/details/ggpvpfflg.sHtML

(new DateTimeImmutable())->format("Y-m-d");
来源：http://3g.fanxiaobao.xyz/Article/details/gfpnfjtmi.sHtML

[U63] PHP：文件读写
来源：http://3g.fanxiaobao.xyz/Article/details/gsiujzjzv.sHtML

file_get_contents($f);  file_put_contents($f, $data);
来源：http://3g.fanxiaobao.xyz/Article/details/gqumddirg.sHtML

[U64] PHP：目录遍历
来源：http://www.blog.fanxiaobao.xyz/Article/details/gkkzjoobj.sHtML

glob("dir/*.php");  scandir("dir");
来源：http://wap.fanxiaobao.xyz/Article/details/guzhahfll.sHtML

[U65] PHP：会话
来源：http://read.share.fanxiaobao.xyz/Article/details/gevekhbou.sHtML

session_start();  $_SESSION["uid"] = 1;
来源：http://mobile.fanxiaobao.xyz/Article/details/gljikccvr.sHtML

[U66] PHP：设置 Cookie
来源：http://read.share.fanxiaobao.xyz/Article/details/gcbcayapt.sHtML

setcookie("token", $v, ["httponly" => true, "samesite" => "Lax"]);
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gfjzvafan.sHtML

[U67] PHP：处理文件上传
来源：http://read.share.fanxiaobao.xyz/Article/details/gbybqrdkw.sHtML

$_FILES["file"]["tmp_name"] 与 move_uploaded_file()
来源：http://mobile.fanxiaobao.xyz/Article/details/gcpzyerfv.sHtML

[U68] PHP：PDO 连接
来源：http://www.share.fanxiaobao.xyz/Article/details/gyxkctalx.sHtML

$pdo = new PDO("mysql:host=localhost;dbname=app", "root", "");
来源：http://wap.fanxiaobao.xyz/Article/details/gqqznhzvr.sHtML

[U69] PHP：PDO 预处理
来源：http://baike.fanxiaobao.xyz/Article/details/gywdswugj.sHtML

$stmt = $pdo->prepare("SELECT * FROM users WHERE id = ?");  $stmt->execute([$id]);
来源：http://m.share.fanxiaobao.xyz/Article/details/gkvxnomuu.sHtML

[U70] PHP：PDO 事务
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gpeqjsugf.sHtML

$pdo->beginTransaction();  $pdo->commit();  $pdo->rollBack();
来源：http://wap.fanxiaobao.xyz/Article/details/gdaibcshb.sHtML

[U71] PHP：抛出异常
来源：http://wap.fanxiaobao.xyz/Article/details/gvuqloipg.sHtML

throw new RuntimeException("失败", 500);
来源：http://read.share.fanxiaobao.xyz/Article/details/ggmgcwanj.sHtML

[U72] PHP：写错误日志
来源：http://baike.fanxiaobao.xyz/Article/details/gfjobjkwe.sHtML

error_log("失败: " . $e->getMessage());
来源：http://www.share.fanxiaobao.xyz/Article/details/gptxrsopu.sHtML

[U73] PHP：读取 ini 配置
来源：http://3g.fanxiaobao.xyz/Article/details/gfmjdznjq.sHtML

parse_ini_file("config.ini", true)
来源：http://baike.fanxiaobao.xyz/Article/details/guqysmdmn.sHtML

[U74] PHP：读取环境变量
来源：http://baike.fanxiaobao.xyz/Article/details/gfdfymxye.sHtML

getenv("APP_ENV") ?: "production"
来源：http://www.share.fanxiaobao.xyz/Article/details/gkvohjjev.sHtML

[U75] PHP：依赖注入
来源：http://www.share.fanxiaobao.xyz/Article/details/gfqtzpmse.sHtML

composer require psr/container
来源：http://m.share.fanxiaobao.xyz/Article/details/gjdhghefl.sHtML

[U76] PHP：简单路由
来源：http://wap.fanxiaobao.xyz/Article/details/gpwbuniah.sHtML

$path = parse_url($_SERVER["REQUEST_URI"], PHP_URL_PATH);
来源：http://mobile.fanxiaobao.xyz/Article/details/gvafsqere.sHtML

[U77] PHP：模板渲染
来源：http://read.share.fanxiaobao.xyz/Article/details/gtnmvpdid.sHtML

composer require twig/twig
来源：http://www.blog.fanxiaobao.xyz/Article/details/gzfkoqyjo.sHtML

[U78] PHP：单元测试
来源：http://read.share.fanxiaobao.xyz/Article/details/gupouhhkg.sHtML

composer require --dev phpunit/phpunit
来源：http://read.share.fanxiaobao.xyz/Article/details/gmqmpoxrx.sHtML

[U79] PHP：静态分析
来源：http://baike.fanxiaobao.xyz/Article/details/glsedqtgi.sHtML

composer require --dev phpstan/phpstan
来源：http://wap.fanxiaobao.xyz/Article/details/gcyxrnfsz.sHtML

[U80] PHP：代码规范修复
来源：http://blog.fanxiaobao.xyz/Article/details/gzrwjbduf.sHtML

composer require --dev friendsofphp/php-cs-fixer
来源：http://blog.fanxiaobao.xyz/Article/details/gidlffbuq.sHtML

[U81] JS：初始化项目
来源：http://www.blog.fanxiaobao.xyz/Article/details/gzjoqrfbo.sHtML

npm init -y;  npm i express
来源：http://m.share.fanxiaobao.xyz/Article/details/glvomahqt.sHtML

[U82] JS：package.json 脚本
来源：http://www.share.fanxiaobao.xyz/Article/details/gzbfbvrvr.sHtML

"scripts": { "dev": "vite", "build": "vite build" }
来源：http://baike.fanxiaobao.xyz/Article/details/gkwldcsmx.sHtML

[U83] JS：ES Module 导入导出
来源：http://read.share.fanxiaobao.xyz/Article/details/gxvctcczw.sHtML

export const a = 1;  import { a } from "./m.js";
来源：http://wap.fanxiaobao.xyz/Article/details/gipyrkdhg.sHtML

[U84] JS：CommonJS 写法
来源：http://3g.fanxiaobao.xyz/Article/details/gxlnwlwls.sHtML

module.exports = { a };  const { a } = require("./m");
来源：http://read.share.fanxiaobao.xyz/Article/details/grlurdgzt.sHtML

[U85] JS：可选链
来源：http://m.share.fanxiaobao.xyz/Article/details/gifhclzcc.sHtML

a?.b?.c
来源：http://3g.fanxiaobao.xyz/Article/details/gwbtkjkgc.sHtML

[U86] JS：空值合并
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gepbmygry.sHtML

a ?? b
来源：http://www.blog.fanxiaobao.xyz/Article/details/gryhyhyxv.sHtML

[U87] JS：解构默认值
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gekdwgcwj.sHtML

const { a = 1, b = 2 } = obj;
来源：http://m.share.fanxiaobao.xyz/Article/details/gcfjwviod.sHtML

[U88] JS：对象展开合并
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gxncgsuza.sHtML

{ ...a, ...b }
来源：http://wap.fanxiaobao.xyz/Article/details/gutzwsqss.sHtML

[U89] JS：数组去重
来源：http://wap.fanxiaobao.xyz/Article/details/gdxwzcxll.sHtML

[...new Set(arr)]
来源：http://baike.fanxiaobao.xyz/Article/details/gmhrmgstv.sHtML

[U90] JS：数字数组排序
来源：http://3g.fanxiaobao.xyz/Article/details/gopkslzcl.sHtML

[...arr].sort((a, b) => a - b)
来源：http://wap.fanxiaobao.xyz/Article/details/giylrcgyy.sHtML

[U91] JS：对象键值遍历
来源：http://3g.fanxiaobao.xyz/Article/details/gyzlaxcky.sHtML

Object.entries(obj).forEach(([k, v]) => {});
来源：http://3g.fanxiaobao.xyz/Article/details/ggpxrdwfi.sHtML

[U92] JS：深拷贝
来源：http://mobile.fanxiaobao.xyz/Article/details/glqaxvhip.sHtML

structuredClone(obj)
来源：http://mobile.fanxiaobao.xyz/Article/details/gdcsydkec.sHtML

[U93] JS：模板字符串
来源：http://baike.fanxiaobao.xyz/Article/details/gegpsvauj.sHtML

`共 ${n} 条`
来源：http://blog.fanxiaobao.xyz/Article/details/giqmwwvlv.sHtML

[U94] JS：箭头函数
来源：http://www.blog.fanxiaobao.xyz/Article/details/gqdsaajnv.sHtML

const double = x => x * 2;
来源：http://blog.fanxiaobao.xyz/Article/details/gcnnvtxfr.sHtML

[U95] JS：Promise 包装
来源：http://mobile.fanxiaobao.xyz/Article/details/gjssbiakr.sHtML

new Promise((resolve, reject) => {})
来源：http://3g.fanxiaobao.xyz/Article/details/gbpzhctty.sHtML

[U96] JS：async/await 与异常
来源：http://baike.fanxiaobao.xyz/Article/details/ggwwbqsgg.sHtML

try { const d = await f(); } catch (e) { console.error(e); }
来源：http://baike.fanxiaobao.xyz/Article/details/gbadeqjzq.sHtML

[U97] JS：并发请求
来源：http://wap.fanxiaobao.xyz/Article/details/gfahesapp.sHtML

await Promise.all(urls.map(u => fetch(u)))
来源：http://www.share.fanxiaobao.xyz/Article/details/gwawdmrdw.sHtML

[U98] JS：fetch 带 JSON
来源：http://www.blog.fanxiaobao.xyz/Article/details/grtsapwxi.sHtML

await fetch(url, { method: "POST", headers: { "Content-Type": "application/json" }, body: JSON.stringify(d) })
来源：http://baike.fanxiaobao.xyz/Article/details/ggfkrsgjo.sHtML

[U99] JS：事件监听
来源：http://www.m.share.fanxiaobao.xyz/Article/details/ginnaephh.sHtML

el.addEventListener("click", e => {})
来源：http://m.share.fanxiaobao.xyz/Article/details/gwmdqqmtu.sHtML

[U100] JS：DOM 查询
来源：http://3g.fanxiaobao.xyz/Article/details/gyzlmfjub.sHtML

document.querySelector(".item")
来源：http://mobile.fanxiaobao.xyz/Article/details/gbvyfmqce.sHtML

[U101] JS：classList 操作
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gtcexyvsz.sHtML

el.classList.toggle("active")
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gbxfngyii.sHtML

[U102] JS：本地存储
来源：http://3g.fanxiaobao.xyz/Article/details/gqujlmqpz.sHtML

localStorage.setItem("k", JSON.stringify(v))
来源：http://mobile.fanxiaobao.xyz/Article/details/ghpskixqs.sHtML

[U103] JS：定时器
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gkuwdxnzg.sHtML

setTimeout(fn, 1000);  setInterval(fn, 1000);
来源：http://mobile.fanxiaobao.xyz/Article/details/girjlndbd.sHtML

[U104] JS：防抖
来源：http://read.share.fanxiaobao.xyz/Article/details/glryaevqt.sHtML

const debounce = (fn, ms) => { let t; return (...a) => { clearTimeout(t); t = setTimeout(() => fn(...a), ms); }; };
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gbmkojjli.sHtML

[U105] JS：节流
来源：http://blog.fanxiaobao.xyz/Article/details/goyhxtgby.sHtML

const throttle = (fn, ms) => { let last = 0; return (...a) => { const n = Date.now(); if (n - last >= ms) { last = n; fn(...a); } }; };
来源：http://read.share.fanxiaobao.xyz/Article/details/gctlqnklu.sHtML

[U106] JS：日期格式化
来源：http://www.share.fanxiaobao.xyz/Article/details/gzydfkrsq.sHtML

new Intl.DateTimeFormat("zh-CN", { dateStyle: "medium" }).format(new Date())
来源：http://baike.fanxiaobao.xyz/Article/details/gzkcsycye.sHtML

[U107] JS：数字千分位
来源：http://wap.fanxiaobao.xyz/Article/details/gumpdnnlx.sHtML

new Intl.NumberFormat("en-US").format(1234567)
来源：http://wap.fanxiaobao.xyz/Article/details/gnjpahfkq.sHtML

[U108] JS：随机整数
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gkggbluuj.sHtML

Math.floor(Math.random() * (max - min + 1)) + min
来源：http://m.share.fanxiaobao.xyz/Article/details/gloervfpv.sHtML

[U109] JS：数组分组
来源：http://wap.fanxiaobao.xyz/Article/details/gigmuddad.sHtML

Object.groupBy(arr, x => x.type)
来源：http://www.blog.fanxiaobao.xyz/Article/details/glqaipogz.sHtML

[U110] JS：数组分块
来源：http://www.share.fanxiaobao.xyz/Article/details/gzpckpetp.sHtML

arr.reduce((acc, x, i) => (i % size ? acc : [...acc, arr.slice(i, i + size)]), [])
来源：http://www.share.fanxiaobao.xyz/Article/details/gutpdhvft.sHtML

[U111] JS：对象转 Map
来源：http://wap.fanxiaobao.xyz/Article/details/gtvonbryb.sHtML

new Map(Object.entries(obj))
来源：http://baike.fanxiaobao.xyz/Article/details/gucykhtim.sHtML

[U112] JS：字符串补位
来源：http://www.share.fanxiaobao.xyz/Article/details/gqzbslxmo.sHtML

"7".padStart(3, "0")
来源：http://www.blog.fanxiaobao.xyz/Article/details/gtjeqxtjf.sHtML

[U113] JS：正则替换全部
来源：http://www.blog.fanxiaobao.xyz/Article/details/gnkmhlxol.sHtML

s.replaceAll("a", "b")
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gafrdyqdl.sHtML

[U114] JS：JSON 深比较
来源：http://m.share.fanxiaobao.xyz/Article/details/gismcevga.sHtML

JSON.stringify(a) === JSON.stringify(b)
来源：http://m.share.fanxiaobao.xyz/Article/details/gxmkkryrr.sHtML

[U115] JS：生成 UUID
来源：http://baike.fanxiaobao.xyz/Article/details/gwqmojepj.sHtML

crypto.randomUUID()
来源：http://blog.fanxiaobao.xyz/Article/details/gsigwcomu.sHtML

[U116] JS：类型检查（JSDoc）
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gldkbjhua.sHtML

/** @param {string} name */ function f(name) {}
来源：http://baike.fanxiaobao.xyz/Article/details/gmdrwsjpq.sHtML

[U117] JS：单元测试
来源：http://read.share.fanxiaobao.xyz/Article/details/glmweghnj.sHtML

npm i -D vitest;  npx vitest
来源：http://read.share.fanxiaobao.xyz/Article/details/gpnighuns.sHtML

[U118] JS：开发服务器
来源：http://blog.fanxiaobao.xyz/Article/details/gtctfsamg.sHtML

npm i -D vite;  npx vite
来源：http://m.share.fanxiaobao.xyz/Article/details/gauyvelnm.sHtML

[U119] JS：生产构建
来源：http://blog.fanxiaobao.xyz/Article/details/griiexjtg.sHtML

npx vite build
来源：http://3g.fanxiaobao.xyz/Article/details/gjjfhljei.sHtML

[U120] JS：读取环境变量（Vite）
来源：http://3g.fanxiaobao.xyz/Article/details/gbxymojgo.sHtML

import.meta.env.VITE_API_URL
来源：http://3g.fanxiaobao.xyz/Article/details/gvcvlxxtn.sHtML

================================================================================
来源：http://www.share.fanxiaobao.xyz/Article/details/gxdyhpbul.sHtML

统计汇总
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gfubakqcp.sHtML

================================================================================
来源：http://mobile.fanxiaobao.xyz/Article/details/gaescglrw.sHtML

按语言统计（条）：
来源：http://blog.fanxiaobao.xyz/Article/details/gcymegqyg.sHtML

Python ......... 252
来源：http://3g.fanxiaobao.xyz/Article/details/gatmmscuw.sHtML

PHP ............ 252
来源：http://blog.fanxiaobao.xyz/Article/details/gwizexxzn.sHtML

JavaScript ..... 252
来源：http://www.blog.fanxiaobao.xyz/Article/details/gikokestc.sHtML

TypeScript ..... 212
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gmfyunhsd.sHtML

Java ........... 212
来源：http://www.blog.fanxiaobao.xyz/Article/details/gzwrlckhk.sHtML

Go ............. 212
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gzytbhpxl.sHtML

Ruby ........... 212
来源：http://www.share.fanxiaobao.xyz/Article/details/gdniirvhf.sHtML

C# ............. 212
来源：http://baike.fanxiaobao.xyz/Article/details/gjnnbkmce.sHtML

C .............. 30
来源：http://mobile.fanxiaobao.xyz/Article/details/gzmuvbppa.sHtML

C++ ............ 30
来源：http://read.share.fanxiaobao.xyz/Article/details/gbtnjbzog.sHtML

SQL ............ 90
来源：http://mobile.fanxiaobao.xyz/Article/details/gfdfkidgl.sHtML

Bash ........... 80
来源：http://www.share.fanxiaobao.xyz/Article/details/ggdgttibt.sHtML

Kotlin ......... 15
来源：http://www.share.fanxiaobao.xyz/Article/details/gebneebof.sHtML

Swift .......... 15
来源：http://wap.fanxiaobao.xyz/Article/details/gkruynfbn.sHtML

Lua ............ 10
来源：http://www.blog.fanxiaobao.xyz/Article/details/gchanleti.sHtML

Perl ........... 10
来源：http://wap.fanxiaobao.xyz/Article/details/gosxpvfkg.sHtML

Scala .......... 10
来源：http://mobile.fanxiaobao.xyz/Article/details/gsckdgqsv.sHtML

------------------------------------
来源：http://www.share.fanxiaobao.xyz/Article/details/ghdyychye.sHtML

合计 ........... 2106 条
来源：http://www.share.fanxiaobao.xyz/Article/details/gxjvllwxh.sHtML

按章节统计：
来源：http://mobile.fanxiaobao.xyz/Article/details/grdlmhrao.sHtML

A 基础语法与类型       26 个任务 × 8 语言 =  208
来源：http://mobile.fanxiaobao.xyz/Article/details/gvgefzohb.sHtML

B 流程控制             16 个任务 × 8 语言 =  128
来源：http://mobile.fanxiaobao.xyz/Article/details/gewbirlcf.sHtML

C 函数与作用域         16 个任务 × 8 语言 =  128
来源：http://www.blog.fanxiaobao.xyz/Article/details/gzrdnggze.sHtML

D 数组 / 列表 / 集合   26 个任务 × 8 语言 =  208
来源：http://blog.fanxiaobao.xyz/Article/details/gfnlydqtj.sHtML

E 字符串处理           22 个任务 × 8 语言 =  176
来源：http://mobile.fanxiaobao.xyz/Article/details/gyxhelytm.sHtML

F 文件与目录           12 个任务 × 8 语言 =   96
来源：http://mobile.fanxiaobao.xyz/Article/details/ghwmzhvmk.sHtML

G 面向对象             16 个任务 × 8 语言 =  128
来源：http://mobile.fanxiaobao.xyz/Article/details/gywguebit.sHtML

H 异常与错误处理       10 个任务 × 8 语言 =   80
来源：http://www.m.share.fanxiaobao.xyz/Article/details/geariixzy.sHtML

I 正则表达式            8 个任务 × 8 语言 =   64
来源：http://m.share.fanxiaobao.xyz/Article/details/gtpfvpxvq.sHtML

J 日期与时间           10 个任务 × 8 语言 =   80
来源：http://wap.fanxiaobao.xyz/Article/details/gjvvzknlj.sHtML

K JSON 与序列化         8 个任务 × 8 语言 =   64
来源：http://baike.fanxiaobao.xyz/Article/details/gfsvvjyzz.sHtML

L 网络请求              8 个任务 × 8 语言 =   64
来源：http://www.blog.fanxiaobao.xyz/Article/details/ghxgtbjaa.sHtML

M 命令行 / 进程         8 个任务 × 8 语言 =   64
来源：http://www.share.fanxiaobao.xyz/Article/details/goqwkhitq.sHtML

N 数据结构与算法       12 个任务 × 8 语言 =   96
来源：http://wap.fanxiaobao.xyz/Article/details/girwfuxzr.sHtML

O 并发与异步            6 个任务 × 8 语言 =   48
来源：http://blog.fanxiaobao.xyz/Article/details/gyqudvlui.sHtML

P 常用工具函数          8 个任务 × 8 语言 =   64
来源：http://www.blog.fanxiaobao.xyz/Article/details/gtmpebeno.sHtML

Q SQL 专题                              90
来源：http://mobile.fanxiaobao.xyz/Article/details/gzgtkitzy.sHtML

R Bash 专题                             80
来源：http://www.share.fanxiaobao.xyz/Article/details/gmjrxgsgj.sHtML

S C / C++ 专题                          60
来源：http://blog.fanxiaobao.xyz/Article/details/gabihpwvq.sHtML

T 其他语言补充                          60
来源：http://www.share.fanxiaobao.xyz/Article/details/gcihgvhvq.sHtML

U 高频实用片段                         120
来源：http://read.share.fanxiaobao.xyz/Article/details/geyjsxial.sHtML

------------------------------------
来源：http://wap.fanxiaobao.xyz/Article/details/gqdkjzbqq.sHtML

合计                                  2106 条
来源：http://baike.fanxiaobao.xyz/Article/details/gfdcvhesp.sHtML

--------------------------------------------------------------------------------
来源：http://www.blog.fanxiaobao.xyz/Article/details/gzdcwgbbu.sHtML

使用提醒
来源：http://m.share.fanxiaobao.xyz/Article/details/gyqvlkcqn.sHtML

--------------------------------------------------------------------------------
来源：http://3g.fanxiaobao.xyz/Article/details/gnyioccoy.sHtML

1. 示例追求"最小可用"，正式项目中请补齐导入、错误处理与边界判断。
来源：http://m.share.fanxiaobao.xyz/Article/details/gxmzsciev.sHtML

2. 涉及文件、网络、数据库的示例，注意资源释放与异常捕获。
来源：http://read.share.fanxiaobao.xyz/Article/details/gtgyjzksx.sHtML

3. 语言版本差异较大（如 Python 3.10 的 match、Java 17 的 record/switch 箭头），
来源：http://mobile.fanxiaobao.xyz/Article/details/gslvpezjn.sHtML

在旧版本上使用前请先确认语法支持情况。
来源：http://wap.fanxiaobao.xyz/Article/details/grqpvftim.sHtML

4. 标注"手写"的条目是因为该语言缺少对应内置能力，实际项目中可引入成熟库。
来源：http://baike.fanxiaobao.xyz/Article/details/gmqfbcjrr.sHtML

—— 文件结束 ——
来源：http://baike.fanxiaobao.xyz/Article/details/gasideihk.sHtML

================================================================================
来源：http://wap.fanxiaobao.xyz/Article/details/gzpevyjny.sHtML

程序语言常见例子速查手册（2024 版）
来源：http://read.share.fanxiaobao.xyz/Article/details/gujwymvsd.sHtML

Common Programming Examples Cheat Book
来源：http://wap.fanxiaobao.xyz/Article/details/gbdvlwxgz.sHtML

================================================================================
来源：http://baike.fanxiaobao.xyz/Article/details/gnhfrwgss.sHtML

【收录内容】
来源：http://www.blog.fanxiaobao.xyz/Article/details/genzlrrkb.sHtML

覆盖 12 种语言 / 语法与常见 API：
来源：http://read.share.fanxiaobao.xyz/Article/details/gwkwuestn.sHtML

Python · PHP · JavaScript · TypeScript · Java · Go · Ruby · C#
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gsdvhbujg.sHtML

SQL · Bash · C · C++
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gtlyqdami.sHtML

按「任务」分组：每个任务下按语言各给出一条最小可用示例。
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gyvzrvjcd.sHtML

【使用说明】
来源：http://mobile.fanxiaobao.xyz/Article/details/gymwainyk.sHtML

1. 每个任务形如 "[编号] 任务名"，下面每行以语言标记开头：
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gdfiuvdnm.sHtML

Py:    Python        PHP:   PHP           JS:    JavaScript
来源：http://www.blog.fanxiaobao.xyz/Article/details/gmkqindid.sHtML

TS:    TypeScript    Java:  Java          Go:    Go
来源：http://blog.fanxiaobao.xyz/Article/details/gnboffung.sHtML

Ruby:  Ruby          C#:    C#            SQL:   SQL
来源：http://wap.fanxiaobao.xyz/Article/details/grekaeplu.sHtML

Bash:  Shell         C:     C             C++:   C++
来源：http://www.share.fanxiaobao.xyz/Article/details/gdzezarmj.sHtML

2. 示例只展示核心写法，刻意省略 import / require / include / using 等样板代码。
来源：http://mobile.fanxiaobao.xyz/Article/details/gtlzabgum.sHtML

需要完整可运行文件时，请自行补齐当前语言的导入语句。
来源：http://3g.fanxiaobao.xyz/Article/details/gtjwehzhj.sHtML

3. 语法基准：Python 3.10+ / PHP 8.1+ / ES2020+ / TypeScript 5 / Java 17 /
来源：http://read.share.fanxiaobao.xyz/Article/details/gfnemrdnl.sHtML

Go 1.21+ / Ruby 3.x / C# 10+ / C17 / C++17。
来源：http://www.blog.fanxiaobao.xyz/Article/details/gqjtvojbg.sHtML

4. 检索建议：用编辑器或浏览器 Ctrl+F 搜关键词，如 "排序" "读取文件" "正则"。
来源：http://3g.fanxiaobao.xyz/Article/details/gbrxwaeaq.sHtML

5. 标记为 "// 无" 表示该语言没有对应的一等语法，需用替代写法（示例给出替代方案）。
来源：http://www.share.fanxiaobao.xyz/Article/details/ghcgraycb.sHtML

6. 符号 "⏎" 表示代码在此处换行（主要用于 Python 等强制缩进、无法压成一行的结构）。
来源：http://blog.fanxiaobao.xyz/Article/details/gbffbttkw.sHtML

【文件统计】
来源：http://www.share.fanxiaobao.xyz/Article/details/gtlecunjx.sHtML

语言示例共 2106 条，分布见本文末尾的「统计汇总」。
来源：http://m.share.fanxiaobao.xyz/Article/details/gjbomqivn.sHtML

--------------------------------------------------------------------------------
来源：http://www.share.fanxiaobao.xyz/Article/details/gmojgeniq.sHtML

目  录
来源：http://wap.fanxiaobao.xyz/Article/details/gxohqiwcz.sHtML

--------------------------------------------------------------------------------
来源：http://mobile.fanxiaobao.xyz/Article/details/gbpzqqnwf.sHtML

A. 基础语法与类型              （第 1 节，26 个任务，208 条）
来源：http://www.blog.fanxiaobao.xyz/Article/details/gtqtoveez.sHtML

B. 流程控制                    （第 2 节，16 个任务，128 条）
来源：http://mobile.fanxiaobao.xyz/Article/details/gmcwicoex.sHtML

C. 函数与作用域                （第 3 节，16 个任务，128 条）
来源：http://blog.fanxiaobao.xyz/Article/details/gtwuljczv.sHtML

D. 数组 / 列表 / 集合          （第 4 节，26 个任务，208 条）
来源：http://mobile.fanxiaobao.xyz/Article/details/gersezwxw.sHtML

E. 字符串处理                  （第 5 节，22 个任务，176 条）
来源：http://mobile.fanxiaobao.xyz/Article/details/gvzbppzlf.sHtML

F. 文件与目录                  （第 6 节，12 个任务，96 条）
来源：http://baike.fanxiaobao.xyz/Article/details/gobioypgv.sHtML

G. 面向对象                    （第 7 节，16 个任务，128 条）
来源：http://www.blog.fanxiaobao.xyz/Article/details/gwilrdmlv.sHtML

H. 异常与错误处理              （第 8 节，10 个任务，80 条）
来源：http://www.blog.fanxiaobao.xyz/Article/details/gsblamlzy.sHtML

I. 正则表达式                  （第 9 节，8 个任务，64 条）
来源：http://m.share.fanxiaobao.xyz/Article/details/ggyiyzryp.sHtML

J. 日期与时间                  （第 10 节，10 个任务，80 条）
来源：http://www.share.fanxiaobao.xyz/Article/details/gdgwzvhag.sHtML

K. JSON 与序列化               （第 11 节，8 个任务，64 条）
来源：http://baike.fanxiaobao.xyz/Article/details/ggkydofam.sHtML

L. 网络请求                    （第 12 节，8 个任务，64 条）
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gtuhaeqkf.sHtML

M. 命令行 / 进程 / 环境        （第 13 节，8 个任务，64 条）
来源：http://m.share.fanxiaobao.xyz/Article/details/ggjynudzk.sHtML

N. 数据结构与算法              （第 14 节，12 个任务，96 条）
来源：http://m.share.fanxiaobao.xyz/Article/details/glpgcipwn.sHtML

O. 并发与异步                  （第 15 节，6 个任务，48 条）
来源：http://3g.fanxiaobao.xyz/Article/details/gbrdsnbro.sHtML

P. 常用工具函数                （第 16 节，8 个任务，64 条）
来源：http://wap.fanxiaobao.xyz/Article/details/ggrrnzpgz.sHtML

Q. SQL 专题                    （第 17 节，90 条）
来源：http://m.share.fanxiaobao.xyz/Article/details/gkclqyomm.sHtML

R. Bash 专题                   （第 18 节，80 条）
来源：http://baike.fanxiaobao.xyz/Article/details/gvvngazdf.sHtML

S. C / C++ 专题                （第 19 节，60 条）
来源：http://www.m.share.fanxiaobao.xyz/Article/details/ggbzzvnvp.sHtML

T. 其他语言补充                （第 20 节，60 条：Kotlin / Swift / Lua / Perl / Scala）
来源：http://m.share.fanxiaobao.xyz/Article/details/gzlptcrqv.sHtML

U. 高频实用片段                （第 21 节，120 条：Python / PHP / JavaScript 各 40 条）
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gqnzpgtas.sHtML

================================================================================
来源：http://m.share.fanxiaobao.xyz/Article/details/gytgbwcap.sHtML

A. 基础语法与类型
来源：http://baike.fanxiaobao.xyz/Article/details/gspvtemoz.sHtML

================================================================================
来源：http://3g.fanxiaobao.xyz/Article/details/glnpvlakh.sHtML

[A01] Hello World
来源：http://blog.fanxiaobao.xyz/Article/details/ghzcluklu.sHtML

Py:   print("Hello, World!")
来源：http://baike.fanxiaobao.xyz/Article/details/geysqpkyq.sHtML

PHP:  echo "Hello, World!";
来源：http://blog.fanxiaobao.xyz/Article/details/gxyavkgdy.sHtML

JS:   console.log("Hello, World!");
来源：http://m.share.fanxiaobao.xyz/Article/details/gxewvdqrh.sHtML

TS:   const msg: string = "Hello, World!"; console.log(msg);
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gnddwnash.sHtML

Java: System.out.println("Hello, World!");
来源：http://www.share.fanxiaobao.xyz/Article/details/gpcqibjsx.sHtML

Go:   fmt.Println("Hello, World!")
来源：http://m.share.fanxiaobao.xyz/Article/details/gbguwxycn.sHtML

Ruby: puts "Hello, World!"
来源：http://www.m.share.fanxiaobao.xyz/Article/details/goxnzrfrc.sHtML

C#:   Console.WriteLine("Hello, World!");
来源：http://wap.fanxiaobao.xyz/Article/details/ggriwoxpr.sHtML

[A02] 变量声明与赋值
来源：http://www.share.fanxiaobao.xyz/Article/details/gipepretf.sHtML

Py:   name = "Alex"; age = 20            # 动态类型，无需声明
来源：http://www.share.fanxiaobao.xyz/Article/details/glmbxchvj.sHtML

PHP:  $name = "Alex"; $age = 20;
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gyxrtyegy.sHtML

JS:   let name = "Alex"; const age = 20;
来源：http://3g.fanxiaobao.xyz/Article/details/gbjebhmpe.sHtML

TS:   let name: string = "Alex"; const age: number = 20;
来源：http://wap.fanxiaobao.xyz/Article/details/gvqbuwpnb.sHtML

Java: String name = "Alex"; int age = 20;
来源：http://wap.fanxiaobao.xyz/Article/details/gzejrjgpt.sHtML

Go:   name := "Alex"; age := 20
来源：http://www.share.fanxiaobao.xyz/Article/details/galcrdeji.sHtML

Ruby: name = "Alex"; age = 20
来源：http://read.share.fanxiaobao.xyz/Article/details/gtzmrjgqn.sHtML


<!-- 参考信息 -->