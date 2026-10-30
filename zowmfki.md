代发 wailian999

[U35] Py：发送邮件
来源：http://3g.fehbvm.com/Article/details/gjcxzjflf.sHtML

smtplib.SMTP_SSL(...).send_message(msg)
来源：http://www.blog.fehbvm.com/Article/details/gmvnbxthk.sHtML

[U36] Py：定时任务
来源：http://www.m.share.fehbvm.com/Article/details/gbtyvffof.sHtML

schedule.every(10).minutes.do(job)
来源：http://www.m.share.hesvh.cn/Article/details/gbjlahfxv.sHtML

[U37] Py：读写 Excel
来源：http://blog.hesvh.cn/Article/details/gxbbjbukb.sHtML

pandas.read_excel / DataFrame.to_excel
来源：http://3g.zdbjq.cn/Article/details/gszbntcvh.sHtML

[U38] Py：获取脚本所在目录
来源：http://www.m.share.fehbvm.com/Article/details/gxhsxdssw.sHtML

Path(__file__).resolve().parent
来源：http://3g.zdbjq.cn/Article/details/gksxzbrva.sHtML

[U39] Py：判断是否在交互环境
来源：http://baike.hesvh.cn/Article/details/ghnfpirxa.sHtML

sys.stdout.isatty()
来源：http://blog.fehbvm.com/Article/details/guakfucap.sHtML

[U40] Py：打印到标准错误
来源：http://baike.zdbjq.cn/Article/details/gqajfpgqv.sHtML

print("err", file=sys.stderr)
来源：http://wap.fehbvm.com/Article/details/gpcsemepl.sHtML

[U41] PHP：初始化 Composer 项目
来源：http://m.share.hesvh.cn/Article/details/gpwexswsp.sHtML

composer init;  composer require guzzlehttp/guzzle
来源：http://3g.hesvh.cn/Article/details/gpunkrloh.sHtML

[U42] PHP：PSR-4 自动加载
来源：http://3g.hesvh.cn/Article/details/gkmgbxhom.sHtML

"autoload": { "psr-4": { "App\\": "src/" } }
来源：http://mobile.zdbjq.cn/Article/details/gxcuoioag.sHtML

[U43] PHP：声明命名空间
来源：http://www.blog.fehbvm.com/Article/details/gzrwilrbi.sHtML

namespace App\Http;
来源：http://www.share.fehbvm.com/Article/details/gyoehevap.sHtML

[U44] PHP：开启严格类型
来源：http://www.m.share.zdbjq.cn/Article/details/gekoqkxse.sHtML

declare(strict_types=1);
来源：http://mobile.hesvh.cn/Article/details/gayoytotd.sHtML

[U45] PHP：类型声明与返回类型
来源：http://www.share.zdbjq.cn/Article/details/gpjmzufyi.sHtML

function add(int $a, int $b): int { return $a + $b; }
来源：http://mobile.fehbvm.com/Article/details/gyxzxpwku.sHtML

[U46] PHP：可空类型
来源：http://baike.hesvh.cn/Article/details/gnhzyjbyv.sHtML

?string $name = null
来源：http://baike.zdbjq.cn/Article/details/gtbjphkgt.sHtML

[U47] PHP：联合类型
来源：http://www.share.fehbvm.com/Article/details/gqpqdxtjg.sHtML

int|string $id
来源：http://wap.zdbjq.cn/Article/details/gbpyevfgt.sHtML

[U48] PHP：纯枚举
来源：http://blog.zdbjq.cn/Article/details/gvriqxfog.sHtML

enum Status: string { case Active = "active"; case Off = "off"; }
来源：http://read.share.hesvh.cn/Article/details/gjyonadzz.sHtML

[U49] PHP：只读属性
来源：http://www.blog.hesvh.cn/Article/details/gwpqgbadt.sHtML

public readonly string $name
来源：http://wap.hesvh.cn/Article/details/gwxfxjhyf.sHtML

[U50] PHP：构造器属性提升
来源：http://wap.hesvh.cn/Article/details/gyhywcrjo.sHtML

public function __construct(private int $id) {}
来源：http://mobile.zdbjq.cn/Article/details/gxkutgumt.sHtML

[U51] PHP：数组解构
来源：http://www.m.share.hesvh.cn/Article/details/grjsobkyd.sHtML

[$a, $b] = $arr;
来源：http://www.m.share.hesvh.cn/Article/details/gjtsyykps.sHtML

[U52] PHP：箭头函数
来源：http://wap.hesvh.cn/Article/details/gxesgfial.sHtML

$double = fn($x) => $x * 2;
来源：http://baike.hesvh.cn/Article/details/gzpigsmiz.sHtML

[U53] PHP：空合并运算符
来源：http://wap.fehbvm.com/Article/details/gfqvinzef.sHtML

$v = $a ?? $b ?? "default";
来源：http://m.share.hesvh.cn/Article/details/gafkerprv.sHtML

[U54] PHP：空安全调用
来源：http://baike.fehbvm.com/Article/details/gdrcygetl.sHtML

$obj?->method()
来源：http://blog.zdbjq.cn/Article/details/gpoalwjef.sHtML

[U55] PHP：match 表达式
来源：http://www.share.fehbvm.com/Article/details/gddzpzbwx.sHtML

$s = match($x) { 1 => "一", default => "其他" };
来源：http://read.share.hesvh.cn/Article/details/ggpbkgnby.sHtML

[U56] PHP：命名参数
来源：http://3g.zdbjq.cn/Article/details/gqflzpbzg.sHtML

f(a: 1, b: 2)
来源：http://read.share.hesvh.cn/Article/details/guqucmoou.sHtML

[U57] PHP：字符串插值
来源：http://wap.fehbvm.com/Article/details/gjbhtyfbb.sHtML

"值: {$a}"
来源：http://m.share.zdbjq.cn/Article/details/glnwxxbul.sHtML

[U58] PHP：数组三件套
来源：http://m.share.zdbjq.cn/Article/details/goqzsclja.sHtML

array_map($f, $a);  array_filter($a, $f);  array_reduce($a, $f, 0);
来源：http://www.share.hesvh.cn/Article/details/guvxcctfr.sHtML

[U59] PHP：自定义排序
来源：http://blog.zdbjq.cn/Article/details/gjcwrglms.sHtML

usort($arr, fn($a, $b) => $a["age"] <=> $b["age"]);
来源：http://baike.fehbvm.com/Article/details/ggcgcakcj.sHtML

[U60] PHP：JSON 编解码
来源：http://wap.hesvh.cn/Article/details/guzwgmxbg.sHtML

json_encode($d, JSON_UNESCAPED_UNICODE);  json_decode($s, true);
来源：http://www.m.share.hesvh.cn/Article/details/ghqxsjscf.sHtML

[U61] PHP：正则
来源：http://blog.hesvh.cn/Article/details/gvqatvmix.sHtML

preg_match('/(\d+)/', $s, $m);  preg_replace('/\d+/', '#', $s);
来源：http://www.m.share.fehbvm.com/Article/details/gxoyvybjp.sHtML

[U62] PHP：日期对象
来源：http://mobile.zdbjq.cn/Article/details/gztlhieha.sHtML

(new DateTimeImmutable())->format("Y-m-d");
来源：http://baike.zdbjq.cn/Article/details/gabpsfnlf.sHtML

[U63] PHP：文件读写
来源：http://m.share.zdbjq.cn/Article/details/gccvuznmz.sHtML

file_get_contents($f);  file_put_contents($f, $data);
来源：http://blog.hesvh.cn/Article/details/gnyqaokze.sHtML

[U64] PHP：目录遍历
来源：http://mobile.zdbjq.cn/Article/details/gvxjpkbhk.sHtML

glob("dir/*.php");  scandir("dir");
来源：http://mobile.hesvh.cn/Article/details/garexixsk.sHtML

[U65] PHP：会话
来源：http://www.blog.hesvh.cn/Article/details/ginenbvbw.sHtML

session_start();  $_SESSION["uid"] = 1;
来源：http://blog.hesvh.cn/Article/details/ghfucpqmt.sHtML

[U66] PHP：设置 Cookie
来源：http://read.share.fehbvm.com/Article/details/gkwjpnowy.sHtML

setcookie("token", $v, ["httponly" => true, "samesite" => "Lax"]);
来源：http://m.share.fehbvm.com/Article/details/grwysmawx.sHtML

[U67] PHP：处理文件上传
来源：http://m.share.fehbvm.com/Article/details/gorsklpgn.sHtML

$_FILES["file"]["tmp_name"] 与 move_uploaded_file()
来源：http://baike.zdbjq.cn/Article/details/gwxvulciy.sHtML

[U68] PHP：PDO 连接
来源：http://mobile.hesvh.cn/Article/details/gncwchlgm.sHtML

$pdo = new PDO("mysql:host=localhost;dbname=app", "root", "");
来源：http://blog.fehbvm.com/Article/details/gkkamuhgl.sHtML

[U69] PHP：PDO 预处理
来源：http://www.m.share.hesvh.cn/Article/details/gumxcfixj.sHtML

$stmt = $pdo->prepare("SELECT * FROM users WHERE id = ?");  $stmt->execute([$id]);
来源：http://3g.zdbjq.cn/Article/details/glpnyebdf.sHtML

[U70] PHP：PDO 事务
来源：http://read.share.fehbvm.com/Article/details/ggwrmgmue.sHtML

$pdo->beginTransaction();  $pdo->commit();  $pdo->rollBack();
来源：http://wap.fehbvm.com/Article/details/gjayrrmvx.sHtML

[U71] PHP：抛出异常
来源：http://wap.zdbjq.cn/Article/details/gholzsdaf.sHtML

throw new RuntimeException("失败", 500);
来源：http://blog.zdbjq.cn/Article/details/gztyafulv.sHtML

[U72] PHP：写错误日志
来源：http://www.share.fehbvm.com/Article/details/gbexymfun.sHtML

error_log("失败: " . $e->getMessage());
来源：http://www.blog.zdbjq.cn/Article/details/gmyimqtue.sHtML

[U73] PHP：读取 ini 配置
来源：http://wap.hesvh.cn/Article/details/gumblljcn.sHtML

parse_ini_file("config.ini", true)
来源：http://www.blog.fehbvm.com/Article/details/gdqsouugt.sHtML

[U74] PHP：读取环境变量
来源：http://3g.zdbjq.cn/Article/details/gucvfectm.sHtML

getenv("APP_ENV") ?: "production"
来源：http://3g.hesvh.cn/Article/details/gclrbylka.sHtML

[U75] PHP：依赖注入
来源：http://3g.zdbjq.cn/Article/details/gkhpkfybq.sHtML

composer require psr/container
来源：http://blog.zdbjq.cn/Article/details/gilmhpeud.sHtML

[U76] PHP：简单路由
来源：http://baike.fehbvm.com/Article/details/guiqptkco.sHtML

$path = parse_url($_SERVER["REQUEST_URI"], PHP_URL_PATH);
来源：http://www.m.share.zdbjq.cn/Article/details/gikrjewxl.sHtML

[U77] PHP：模板渲染
来源：http://m.share.fehbvm.com/Article/details/gtynltnen.sHtML

composer require twig/twig
来源：http://www.share.zdbjq.cn/Article/details/gyhgpompf.sHtML

[U78] PHP：单元测试
来源：http://m.share.zdbjq.cn/Article/details/goppuxssc.sHtML

composer require --dev phpunit/phpunit
来源：http://blog.fehbvm.com/Article/details/gepsirsja.sHtML

[U79] PHP：静态分析
来源：http://wap.fehbvm.com/Article/details/gbwksivcn.sHtML

composer require --dev phpstan/phpstan
来源：http://www.share.fehbvm.com/Article/details/gyrfpjtre.sHtML

[U80] PHP：代码规范修复
来源：http://wap.zdbjq.cn/Article/details/gannsynwu.sHtML

composer require --dev friendsofphp/php-cs-fixer
来源：http://3g.zdbjq.cn/Article/details/ganbtnndz.sHtML

[U81] JS：初始化项目
来源：http://www.m.share.hesvh.cn/Article/details/gnkpcaoje.sHtML

npm init -y;  npm i express
来源：http://wap.hesvh.cn/Article/details/ggimyxlqk.sHtML

[U82] JS：package.json 脚本
来源：http://baike.hesvh.cn/Article/details/gjidembyv.sHtML

"scripts": { "dev": "vite", "build": "vite build" }
来源：http://www.share.hesvh.cn/Article/details/gouubjgrl.sHtML

[U83] JS：ES Module 导入导出
来源：http://wap.hesvh.cn/Article/details/gissuhqpu.sHtML

export const a = 1;  import { a } from "./m.js";
来源：http://m.share.zdbjq.cn/Article/details/guygeuhtx.sHtML

[U84] JS：CommonJS 写法
来源：http://www.share.fehbvm.com/Article/details/gnvnnxxrz.sHtML

module.exports = { a };  const { a } = require("./m");
来源：http://www.blog.zdbjq.cn/Article/details/gmibthcxb.sHtML

[U85] JS：可选链
来源：http://wap.zdbjq.cn/Article/details/ggfubpcxs.sHtML

a?.b?.c
来源：http://m.share.hesvh.cn/Article/details/gwcadwwca.sHtML

[U86] JS：空值合并
来源：http://wap.hesvh.cn/Article/details/gqugxszhc.sHtML

a ?? b
来源：http://read.share.hesvh.cn/Article/details/gjjqojrbu.sHtML

[U87] JS：解构默认值
来源：http://baike.zdbjq.cn/Article/details/grdexgwzb.sHtML

const { a = 1, b = 2 } = obj;
来源：http://www.m.share.fehbvm.com/Article/details/gvvwknzqj.sHtML

[U88] JS：对象展开合并
来源：http://m.share.hesvh.cn/Article/details/gzttstlhy.sHtML

{ ...a, ...b }
来源：http://www.m.share.zdbjq.cn/Article/details/gjbgqslzc.sHtML

[U89] JS：数组去重
来源：http://wap.zdbjq.cn/Article/details/gmzcfcyxi.sHtML

[...new Set(arr)]
来源：http://wap.hesvh.cn/Article/details/gkinxvgoj.sHtML

[U90] JS：数字数组排序
来源：http://www.m.share.hesvh.cn/Article/details/gqxzzdtgc.sHtML

[...arr].sort((a, b) => a - b)
来源：http://blog.zdbjq.cn/Article/details/gcwrjdrma.sHtML

[U91] JS：对象键值遍历
来源：http://mobile.fehbvm.com/Article/details/gwatjtfkc.sHtML

Object.entries(obj).forEach(([k, v]) => {});
来源：http://baike.zdbjq.cn/Article/details/gnvytqpcm.sHtML

[U92] JS：深拷贝
来源：http://3g.fehbvm.com/Article/details/gnoublhfq.sHtML

structuredClone(obj)
来源：http://www.share.zdbjq.cn/Article/details/gzmqitxxh.sHtML

[U93] JS：模板字符串
来源：http://www.share.zdbjq.cn/Article/details/glcupixql.sHtML

`共 ${n} 条`
来源：http://www.blog.zdbjq.cn/Article/details/gxzwsrirs.sHtML

[U94] JS：箭头函数
来源：http://read.share.zdbjq.cn/Article/details/gljkgtknw.sHtML

const double = x => x * 2;
来源：http://baike.fehbvm.com/Article/details/gbdldxobr.sHtML

[U95] JS：Promise 包装
来源：http://m.share.fehbvm.com/Article/details/gvmrxqeeq.sHtML

new Promise((resolve, reject) => {})
来源：http://mobile.fehbvm.com/Article/details/gqipopoaa.sHtML

[U96] JS：async/await 与异常
来源：http://www.m.share.fehbvm.com/Article/details/gfbvtkjej.sHtML

try { const d = await f(); } catch (e) { console.error(e); }
来源：http://www.share.hesvh.cn/Article/details/gbpthjotc.sHtML

[U97] JS：并发请求
来源：http://mobile.fehbvm.com/Article/details/gpfginhjc.sHtML

await Promise.all(urls.map(u => fetch(u)))
来源：http://mobile.zdbjq.cn/Article/details/gtwqduyuv.sHtML

[U98] JS：fetch 带 JSON
来源：http://www.blog.zdbjq.cn/Article/details/gccaflygb.sHtML

await fetch(url, { method: "POST", headers: { "Content-Type": "application/json" }, body: JSON.stringify(d) })
来源：http://www.m.share.fehbvm.com/Article/details/gptcvuahu.sHtML

[U99] JS：事件监听
来源：http://blog.zdbjq.cn/Article/details/ghatmetdn.sHtML

el.addEventListener("click", e => {})
来源：http://read.share.fehbvm.com/Article/details/gfmqdgaio.sHtML

[U100] JS：DOM 查询
来源：http://m.share.hesvh.cn/Article/details/gszvvbvtp.sHtML

document.querySelector(".item")
来源：http://www.m.share.zdbjq.cn/Article/details/gvttvwqzs.sHtML

[U101] JS：classList 操作
来源：http://mobile.zdbjq.cn/Article/details/gevhuwlvj.sHtML

el.classList.toggle("active")
来源：http://www.m.share.hesvh.cn/Article/details/gehaaudzb.sHtML

[U102] JS：本地存储
来源：http://m.share.zdbjq.cn/Article/details/gpzxhhknn.sHtML

localStorage.setItem("k", JSON.stringify(v))
来源：http://www.m.share.fehbvm.com/Article/details/gpezwsily.sHtML

[U103] JS：定时器
来源：http://mobile.zdbjq.cn/Article/details/gkefvtwdl.sHtML

setTimeout(fn, 1000);  setInterval(fn, 1000);
来源：http://baike.zdbjq.cn/Article/details/gncduvrdm.sHtML

[U104] JS：防抖
来源：http://mobile.fehbvm.com/Article/details/gafmgazdl.sHtML

const debounce = (fn, ms) => { let t; return (...a) => { clearTimeout(t); t = setTimeout(() => fn(...a), ms); }; };
来源：http://m.share.zdbjq.cn/Article/details/gmuniguzq.sHtML

[U105] JS：节流
来源：http://www.blog.fehbvm.com/Article/details/gwbqgbggi.sHtML

const throttle = (fn, ms) => { let last = 0; return (...a) => { const n = Date.now(); if (n - last >= ms) { last = n; fn(...a); } }; };
来源：http://mobile.zdbjq.cn/Article/details/gctarcpdg.sHtML

[U106] JS：日期格式化
来源：http://www.blog.zdbjq.cn/Article/details/ghegqaxrz.sHtML

new Intl.DateTimeFormat("zh-CN", { dateStyle: "medium" }).format(new Date())
来源：http://read.share.hesvh.cn/Article/details/giqwtkebw.sHtML

[U107] JS：数字千分位
来源：http://blog.hesvh.cn/Article/details/gsyauywzi.sHtML

new Intl.NumberFormat("en-US").format(1234567)
来源：http://m.share.hesvh.cn/Article/details/gxdvdkese.sHtML

[U108] JS：随机整数
来源：http://wap.zdbjq.cn/Article/details/gazdfcmvb.sHtML

Math.floor(Math.random() * (max - min + 1)) + min
来源：http://mobile.zdbjq.cn/Article/details/guhplbwsd.sHtML

[U109] JS：数组分组
来源：http://www.m.share.fehbvm.com/Article/details/gzdlrkbqr.sHtML

Object.groupBy(arr, x => x.type)
来源：http://wap.zdbjq.cn/Article/details/gnocmlrzm.sHtML

[U110] JS：数组分块
来源：http://m.share.hesvh.cn/Article/details/gbbscppqt.sHtML

arr.reduce((acc, x, i) => (i % size ? acc : [...acc, arr.slice(i, i + size)]), [])
来源：http://wap.zdbjq.cn/Article/details/gjycbpiea.sHtML

[U111] JS：对象转 Map
来源：http://3g.fehbvm.com/Article/details/ggitjujjk.sHtML

new Map(Object.entries(obj))
来源：http://baike.fehbvm.com/Article/details/glxqhxbfx.sHtML

[U112] JS：字符串补位
来源：http://m.share.zdbjq.cn/Article/details/gzoechgth.sHtML

"7".padStart(3, "0")
来源：http://blog.fehbvm.com/Article/details/grfhavejf.sHtML

[U113] JS：正则替换全部
来源：http://mobile.hesvh.cn/Article/details/ghooyxamk.sHtML

s.replaceAll("a", "b")
来源：http://read.share.zdbjq.cn/Article/details/gmzlmuoor.sHtML

[U114] JS：JSON 深比较
来源：http://3g.hesvh.cn/Article/details/gshkmbpkp.sHtML

JSON.stringify(a) === JSON.stringify(b)
来源：http://www.m.share.hesvh.cn/Article/details/gkhorsbax.sHtML

[U115] JS：生成 UUID
来源：http://www.m.share.hesvh.cn/Article/details/ghvgrkrmd.sHtML

crypto.randomUUID()
来源：http://baike.hesvh.cn/Article/details/grtgdctzy.sHtML

[U116] JS：类型检查（JSDoc）
来源：http://www.blog.hesvh.cn/Article/details/gfgxyrfvh.sHtML

/** @param {string} name */ function f(name) {}
来源：http://baike.hesvh.cn/Article/details/gxeqlpgcs.sHtML

[U117] JS：单元测试
来源：http://mobile.hesvh.cn/Article/details/gbvaldwfr.sHtML

npm i -D vitest;  npx vitest
来源：http://m.share.hesvh.cn/Article/details/gvlhfbvmd.sHtML

[U118] JS：开发服务器
来源：http://3g.zdbjq.cn/Article/details/geqmfgfkn.sHtML

npm i -D vite;  npx vite
来源：http://blog.hesvh.cn/Article/details/gxbfqhuxu.sHtML

[U119] JS：生产构建
来源：http://baike.fehbvm.com/Article/details/gzhmvxxwx.sHtML

npx vite build
来源：http://blog.zdbjq.cn/Article/details/gyydyevus.sHtML

[U120] JS：读取环境变量（Vite）
来源：http://www.blog.hesvh.cn/Article/details/gkypnoccc.sHtML

import.meta.env.VITE_API_URL
来源：http://www.m.share.fehbvm.com/Article/details/gprbgbqdr.sHtML

================================================================================
来源：http://3g.hesvh.cn/Article/details/ghqjfcwtl.sHtML

统计汇总
来源：http://m.share.hesvh.cn/Article/details/ghozsnpkm.sHtML

================================================================================
来源：http://www.blog.zdbjq.cn/Article/details/gyxgncion.sHtML

按语言统计（条）：
来源：http://www.blog.zdbjq.cn/Article/details/gwqbekjhq.sHtML

Python ......... 252
来源：http://mobile.hesvh.cn/Article/details/guflielsg.sHtML

PHP ............ 252
来源：http://m.share.hesvh.cn/Article/details/grklykiro.sHtML

JavaScript ..... 252
来源：http://blog.zdbjq.cn/Article/details/gndoysopr.sHtML

TypeScript ..... 212
来源：http://www.blog.hesvh.cn/Article/details/gzxgnttwa.sHtML

Java ........... 212
来源：http://read.share.zdbjq.cn/Article/details/gdkpozver.sHtML

Go ............. 212
来源：http://www.share.zdbjq.cn/Article/details/gqefvpwfz.sHtML

Ruby ........... 212
来源：http://read.share.zdbjq.cn/Article/details/gjunsfttp.sHtML

C# ............. 212
来源：http://www.m.share.hesvh.cn/Article/details/gtmapgrgr.sHtML

C .............. 30
来源：http://baike.zdbjq.cn/Article/details/gvzykhnvq.sHtML

C++ ............ 30
来源：http://read.share.fehbvm.com/Article/details/gvfanhaio.sHtML

SQL ............ 90
来源：http://baike.hesvh.cn/Article/details/gfgcndqyv.sHtML

Bash ........... 80
来源：http://blog.hesvh.cn/Article/details/grtotxfgl.sHtML

Kotlin ......... 15
来源：http://baike.hesvh.cn/Article/details/gynyemrtb.sHtML

Swift .......... 15
来源：http://blog.zdbjq.cn/Article/details/gibkpohmh.sHtML

Lua ............ 10
来源：http://www.share.zdbjq.cn/Article/details/glytmkczh.sHtML

Perl ........... 10
来源：http://baike.zdbjq.cn/Article/details/gxjxgslnk.sHtML

Scala .......... 10
来源：http://wap.hesvh.cn/Article/details/gbujsqmpk.sHtML

------------------------------------
来源：http://3g.fehbvm.com/Article/details/gjuxoxgxr.sHtML

合计 ........... 2106 条
来源：http://mobile.fehbvm.com/Article/details/gtjgoefhe.sHtML

按章节统计：
来源：http://mobile.zdbjq.cn/Article/details/gqxozzrae.sHtML

A 基础语法与类型       26 个任务 × 8 语言 =  208
来源：http://m.share.fehbvm.com/Article/details/gsxkqvxal.sHtML

B 流程控制             16 个任务 × 8 语言 =  128
来源：http://wap.hesvh.cn/Article/details/gckflvlmn.sHtML

C 函数与作用域         16 个任务 × 8 语言 =  128
来源：http://www.blog.hesvh.cn/Article/details/gqhbxzpgg.sHtML

D 数组 / 列表 / 集合   26 个任务 × 8 语言 =  208
来源：http://blog.fehbvm.com/Article/details/ghfxiodeh.sHtML

E 字符串处理           22 个任务 × 8 语言 =  176
来源：http://mobile.hesvh.cn/Article/details/geqlgbqan.sHtML

F 文件与目录           12 个任务 × 8 语言 =   96
来源：http://read.share.fehbvm.com/Article/details/gyaxmnzzy.sHtML

G 面向对象             16 个任务 × 8 语言 =  128
来源：http://3g.hesvh.cn/Article/details/grpbqaljq.sHtML

H 异常与错误处理       10 个任务 × 8 语言 =   80
来源：http://blog.zdbjq.cn/Article/details/gamonumdy.sHtML

I 正则表达式            8 个任务 × 8 语言 =   64
来源：http://m.share.zdbjq.cn/Article/details/gooaugrlo.sHtML

J 日期与时间           10 个任务 × 8 语言 =   80
来源：http://blog.zdbjq.cn/Article/details/ghzixblbk.sHtML

K JSON 与序列化         8 个任务 × 8 语言 =   64
来源：http://mobile.hesvh.cn/Article/details/gveayyesj.sHtML

L 网络请求              8 个任务 × 8 语言 =   64
来源：http://3g.hesvh.cn/Article/details/gquqpcyeb.sHtML

M 命令行 / 进程         8 个任务 × 8 语言 =   64
来源：http://read.share.hesvh.cn/Article/details/gvuhuhafp.sHtML

N 数据结构与算法       12 个任务 × 8 语言 =   96
来源：http://www.m.share.fehbvm.com/Article/details/guysnjdap.sHtML

O 并发与异步            6 个任务 × 8 语言 =   48
来源：http://mobile.fehbvm.com/Article/details/gagrqrjmj.sHtML

P 常用工具函数          8 个任务 × 8 语言 =   64
来源：http://wap.zdbjq.cn/Article/details/gktodbtow.sHtML

Q SQL 专题                              90
来源：http://m.share.fehbvm.com/Article/details/ggtrpmuwf.sHtML

R Bash 专题                             80
来源：http://m.share.fehbvm.com/Article/details/gqddvvzbg.sHtML

S C / C++ 专题                          60
来源：http://m.share.zdbjq.cn/Article/details/gmwncirpo.sHtML

T 其他语言补充                          60
来源：http://3g.zdbjq.cn/Article/details/gluffeglh.sHtML

U 高频实用片段                         120
来源：http://read.share.zdbjq.cn/Article/details/gtxlcmgma.sHtML

------------------------------------
来源：http://baike.zdbjq.cn/Article/details/gcxnaxuoo.sHtML

合计                                  2106 条
来源：http://www.m.share.hesvh.cn/Article/details/gqkhqjakn.sHtML

--------------------------------------------------------------------------------
来源：http://m.share.fehbvm.com/Article/details/giajxbsor.sHtML

使用提醒
来源：http://m.share.hesvh.cn/Article/details/geayjecmg.sHtML

--------------------------------------------------------------------------------
来源：http://www.share.fehbvm.com/Article/details/gznappskl.sHtML

1. 示例追求"最小可用"，正式项目中请补齐导入、错误处理与边界判断。
来源：http://wap.fehbvm.com/Article/details/gfdckgwzc.sHtML

2. 涉及文件、网络、数据库的示例，注意资源释放与异常捕获。
来源：http://baike.fehbvm.com/Article/details/gmefhoycj.sHtML

3. 语言版本差异较大（如 Python 3.10 的 match、Java 17 的 record/switch 箭头），
来源：http://wap.hesvh.cn/Article/details/gvztoyqoa.sHtML

在旧版本上使用前请先确认语法支持情况。
来源：http://www.m.share.hesvh.cn/Article/details/glyhqqkbm.sHtML

4. 标注"手写"的条目是因为该语言缺少对应内置能力，实际项目中可引入成熟库。
来源：http://www.blog.fehbvm.com/Article/details/gqeaakphk.sHtML

—— 文件结束 ——
来源：http://www.m.share.hesvh.cn/Article/details/gwaxnmqon.sHtML

================================================================================
来源：http://read.share.zdbjq.cn/Article/details/gbxwphray.sHtML

程序语言常见例子速查手册（2024 版）
来源：http://mobile.fehbvm.com/Article/details/gggbbrcib.sHtML

Common Programming Examples Cheat Book
来源：http://blog.zdbjq.cn/Article/details/giglbtegq.sHtML

================================================================================
来源：http://blog.zdbjq.cn/Article/details/gemrqcrin.sHtML

【收录内容】
来源：http://www.blog.fehbvm.com/Article/details/gbtbysrmo.sHtML

覆盖 12 种语言 / 语法与常见 API：
来源：http://baike.hesvh.cn/Article/details/gcgpobrop.sHtML

Python · PHP · JavaScript · TypeScript · Java · Go · Ruby · C#
来源：http://baike.zdbjq.cn/Article/details/ghwuupgio.sHtML

SQL · Bash · C · C++
来源：http://wap.zdbjq.cn/Article/details/gbwnqvbut.sHtML

按「任务」分组：每个任务下按语言各给出一条最小可用示例。
来源：http://read.share.hesvh.cn/Article/details/gclwzrrif.sHtML

【使用说明】
来源：http://mobile.zdbjq.cn/Article/details/gnpzzbecj.sHtML

1. 每个任务形如 "[编号] 任务名"，下面每行以语言标记开头：
来源：http://baike.zdbjq.cn/Article/details/gbjzvmchb.sHtML

Py:    Python        PHP:   PHP           JS:    JavaScript
来源：http://wap.fehbvm.com/Article/details/gtkofcocf.sHtML

TS:    TypeScript    Java:  Java          Go:    Go
来源：http://wap.hesvh.cn/Article/details/gfdjjdxhj.sHtML

Ruby:  Ruby          C#:    C#            SQL:   SQL
来源：http://www.blog.hesvh.cn/Article/details/gmbcxnoqy.sHtML

Bash:  Shell         C:     C             C++:   C++
来源：http://read.share.hesvh.cn/Article/details/gmoiddzba.sHtML

2. 示例只展示核心写法，刻意省略 import / require / include / using 等样板代码。
来源：http://blog.fehbvm.com/Article/details/guoosyjil.sHtML

需要完整可运行文件时，请自行补齐当前语言的导入语句。
来源：http://www.m.share.zdbjq.cn/Article/details/gnmgcoodl.sHtML

3. 语法基准：Python 3.10+ / PHP 8.1+ / ES2020+ / TypeScript 5 / Java 17 /
来源：http://baike.hesvh.cn/Article/details/gxhatbpwh.sHtML

Go 1.21+ / Ruby 3.x / C# 10+ / C17 / C++17。
来源：http://read.share.hesvh.cn/Article/details/gohsmsfnl.sHtML

4. 检索建议：用编辑器或浏览器 Ctrl+F 搜关键词，如 "排序" "读取文件" "正则"。
来源：http://blog.fehbvm.com/Article/details/gvhcqtvio.sHtML

5. 标记为 "// 无" 表示该语言没有对应的一等语法，需用替代写法（示例给出替代方案）。
来源：http://baike.hesvh.cn/Article/details/gvxmnmpps.sHtML

6. 符号 "⏎" 表示代码在此处换行（主要用于 Python 等强制缩进、无法压成一行的结构）。
来源：http://read.share.fehbvm.com/Article/details/ggztzdenn.sHtML

【文件统计】
来源：http://www.share.zdbjq.cn/Article/details/gxoxisjlc.sHtML

语言示例共 2106 条，分布见本文末尾的「统计汇总」。
来源：http://wap.zdbjq.cn/Article/details/glshehgfh.sHtML

--------------------------------------------------------------------------------
来源：http://mobile.fehbvm.com/Article/details/gexffsdov.sHtML

目  录
来源：http://3g.zdbjq.cn/Article/details/gynavwemr.sHtML

--------------------------------------------------------------------------------
来源：http://read.share.zdbjq.cn/Article/details/gzmajotnl.sHtML

A. 基础语法与类型              （第 1 节，26 个任务，208 条）
来源：http://read.share.fehbvm.com/Article/details/gggzrmrjx.sHtML

B. 流程控制                    （第 2 节，16 个任务，128 条）
来源：http://mobile.zdbjq.cn/Article/details/grveotseq.sHtML

C. 函数与作用域                （第 3 节，16 个任务，128 条）
来源：http://read.share.fehbvm.com/Article/details/gyulrhnlo.sHtML

D. 数组 / 列表 / 集合          （第 4 节，26 个任务，208 条）
来源：http://m.share.fehbvm.com/Article/details/gnbdokhel.sHtML

E. 字符串处理                  （第 5 节，22 个任务，176 条）
来源：http://mobile.zdbjq.cn/Article/details/guicxpwfn.sHtML

F. 文件与目录                  （第 6 节，12 个任务，96 条）
来源：http://www.blog.fehbvm.com/Article/details/gxkcfzrwp.sHtML

G. 面向对象                    （第 7 节，16 个任务，128 条）
来源：http://www.share.fehbvm.com/Article/details/gooddxziv.sHtML

H. 异常与错误处理              （第 8 节，10 个任务，80 条）
来源：http://www.blog.hesvh.cn/Article/details/gkilmwrht.sHtML

I. 正则表达式                  （第 9 节，8 个任务，64 条）
来源：http://wap.fehbvm.com/Article/details/gaoefseig.sHtML

J. 日期与时间                  （第 10 节，10 个任务，80 条）
来源：http://m.share.hesvh.cn/Article/details/gsntwdvmu.sHtML

K. JSON 与序列化               （第 11 节，8 个任务，64 条）
来源：http://m.share.hesvh.cn/Article/details/grtomdzca.sHtML

L. 网络请求                    （第 12 节，8 个任务，64 条）
来源：http://www.m.share.fehbvm.com/Article/details/gpmbuzkty.sHtML

M. 命令行 / 进程 / 环境        （第 13 节，8 个任务，64 条）
来源：http://blog.hesvh.cn/Article/details/giqcxeszq.sHtML

N. 数据结构与算法              （第 14 节，12 个任务，96 条）
来源：http://m.share.hesvh.cn/Article/details/gapetkbfk.sHtML

O. 并发与异步                  （第 15 节，6 个任务，48 条）
来源：http://blog.zdbjq.cn/Article/details/glmprkait.sHtML

P. 常用工具函数                （第 16 节，8 个任务，64 条）
来源：http://blog.zdbjq.cn/Article/details/gtstlyhpr.sHtML

Q. SQL 专题                    （第 17 节，90 条）
来源：http://www.blog.zdbjq.cn/Article/details/giwcberam.sHtML

R. Bash 专题                   （第 18 节，80 条）
来源：http://read.share.hesvh.cn/Article/details/gsvtvpbzk.sHtML

S. C / C++ 专题                （第 19 节，60 条）
来源：http://baike.zdbjq.cn/Article/details/gpctqwfci.sHtML

T. 其他语言补充                （第 20 节，60 条：Kotlin / Swift / Lua / Perl / Scala）
来源：http://3g.fehbvm.com/Article/details/guyshsbxh.sHtML

U. 高频实用片段                （第 21 节，120 条：Python / PHP / JavaScript 各 40 条）
来源：http://blog.hesvh.cn/Article/details/gpbcdbekz.sHtML

================================================================================
来源：http://www.share.hesvh.cn/Article/details/girwoulys.sHtML

A. 基础语法与类型
来源：http://3g.fehbvm.com/Article/details/gssdtqpsl.sHtML

================================================================================
来源：http://3g.fehbvm.com/Article/details/gwqzilqfo.sHtML

[A01] Hello World
来源：http://www.blog.zdbjq.cn/Article/details/gszbhgkry.sHtML

Py:   print("Hello, World!")
来源：http://m.share.hesvh.cn/Article/details/gnyoodjll.sHtML

PHP:  echo "Hello, World!";
来源：http://3g.fehbvm.com/Article/details/gvrooydws.sHtML

JS:   console.log("Hello, World!");
来源：http://baike.zdbjq.cn/Article/details/gfsfkbubd.sHtML

TS:   const msg: string = "Hello, World!"; console.log(msg);
来源：http://wap.fehbvm.com/Article/details/gzvqfaidx.sHtML

Java: System.out.println("Hello, World!");
来源：http://mobile.fehbvm.com/Article/details/gkgplpmmm.sHtML

Go:   fmt.Println("Hello, World!")
来源：http://www.m.share.hesvh.cn/Article/details/gnvmlaevk.sHtML

Ruby: puts "Hello, World!"
来源：http://baike.hesvh.cn/Article/details/gsydzfhhe.sHtML

C#:   Console.WriteLine("Hello, World!");
来源：http://wap.hesvh.cn/Article/details/gdnvazbde.sHtML

[A02] 变量声明与赋值
来源：http://www.m.share.hesvh.cn/Article/details/ghdsmywip.sHtML

Py:   name = "Alex"; age = 20            # 动态类型，无需声明
来源：http://www.m.share.zdbjq.cn/Article/details/gmgwjuhib.sHtML

PHP:  $name = "Alex"; $age = 20;
来源：http://3g.hesvh.cn/Article/details/gwlwfyqdc.sHtML

JS:   let name = "Alex"; const age = 20;
来源：http://3g.hesvh.cn/Article/details/gnimvkjih.sHtML

TS:   let name: string = "Alex"; const age: number = 20;
来源：http://www.blog.fehbvm.com/Article/details/gnvxzfmli.sHtML

Java: String name = "Alex"; int age = 20;
来源：http://www.blog.fehbvm.com/Article/details/gjbychwha.sHtML

Go:   name := "Alex"; age := 20
来源：http://m.share.fehbvm.com/Article/details/gfejcpzdy.sHtML

Ruby: name = "Alex"; age = 20
来源：http://3g.hesvh.cn/Article/details/gaghfwdpd.sHtML

C#:   string name = "Alex"; int age = 20;
来源：http://www.blog.zdbjq.cn/Article/details/ggtjrihuk.sHtML

[A03] 常量定义
来源：http://read.share.hesvh.cn/Article/details/gsndsmpqr.sHtML

Py:   PI = 3.14159                       # 约定全大写，语言不强制
来源：http://m.share.fehbvm.com/Article/details/gureojndi.sHtML

PHP:  const PI = 3.14159;
来源：http://3g.fehbvm.com/Article/details/gnuiuxtvx.sHtML


<!-- 参考信息 -->