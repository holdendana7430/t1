代发 wailian999

[U35] Py：发送邮件
来源：http://read.share.hesvh.cn/Article/details/gkaeqwpgx.sHtML

smtplib.SMTP_SSL(...).send_message(msg)
来源：http://3g.hesvh.cn/Article/details/gcjoltcih.sHtML

[U36] Py：定时任务
来源：http://baike.fehbvm.com/Article/details/gusmpzubs.sHtML

schedule.every(10).minutes.do(job)
来源：http://www.share.fehbvm.com/Article/details/gwzruveww.sHtML

[U37] Py：读写 Excel
来源：http://baike.fehbvm.com/Article/details/grkpykzrj.sHtML

pandas.read_excel / DataFrame.to_excel
来源：http://wap.fehbvm.com/Article/details/gidwvvntx.sHtML

[U38] Py：获取脚本所在目录
来源：http://blog.hesvh.cn/Article/details/gievpmyyd.sHtML

Path(__file__).resolve().parent
来源：http://mobile.zdbjq.cn/Article/details/gsuthipnz.sHtML

[U39] Py：判断是否在交互环境
来源：http://mobile.zdbjq.cn/Article/details/gpviiyxqy.sHtML

sys.stdout.isatty()
来源：http://mobile.zdbjq.cn/Article/details/gylxeclyd.sHtML

[U40] Py：打印到标准错误
来源：http://www.blog.hesvh.cn/Article/details/ghdwzpvux.sHtML

print("err", file=sys.stderr)
来源：http://3g.zdbjq.cn/Article/details/gcbpksugl.sHtML

[U41] PHP：初始化 Composer 项目
来源：http://blog.hesvh.cn/Article/details/gbvqshhbk.sHtML

composer init;  composer require guzzlehttp/guzzle
来源：http://mobile.fehbvm.com/Article/details/gotorclkb.sHtML

[U42] PHP：PSR-4 自动加载
来源：http://www.blog.zdbjq.cn/Article/details/gmgliqjqd.sHtML

"autoload": { "psr-4": { "App\\": "src/" } }
来源：http://3g.hesvh.cn/Article/details/gikxleyos.sHtML

[U43] PHP：声明命名空间
来源：http://wap.hesvh.cn/Article/details/gvcgezkll.sHtML

namespace App\Http;
来源：http://blog.fehbvm.com/Article/details/gmuixxxfn.sHtML

[U44] PHP：开启严格类型
来源：http://blog.zdbjq.cn/Article/details/gewaiihts.sHtML

declare(strict_types=1);
来源：http://www.share.fehbvm.com/Article/details/gqxeesbkn.sHtML

[U45] PHP：类型声明与返回类型
来源：http://baike.hesvh.cn/Article/details/gepznwkyl.sHtML

function add(int $a, int $b): int { return $a + $b; }
来源：http://wap.fehbvm.com/Article/details/gpramzoyp.sHtML

[U46] PHP：可空类型
来源：http://read.share.zdbjq.cn/Article/details/gbcfeuhkk.sHtML

?string $name = null
来源：http://3g.hesvh.cn/Article/details/gjqlbylxh.sHtML

[U47] PHP：联合类型
来源：http://baike.zdbjq.cn/Article/details/ghsnuuysf.sHtML

int|string $id
来源：http://m.share.fehbvm.com/Article/details/ghsaujnea.sHtML

[U48] PHP：纯枚举
来源：http://m.share.zdbjq.cn/Article/details/glikuikdz.sHtML

enum Status: string { case Active = "active"; case Off = "off"; }
来源：http://www.share.fehbvm.com/Article/details/gjxbxgcmf.sHtML

[U49] PHP：只读属性
来源：http://www.blog.hesvh.cn/Article/details/gowrvxryw.sHtML

public readonly string $name
来源：http://m.share.zdbjq.cn/Article/details/gsbtgbcdm.sHtML

[U50] PHP：构造器属性提升
来源：http://wap.fehbvm.com/Article/details/gvrwhdwyq.sHtML

public function __construct(private int $id) {}
来源：http://www.blog.fehbvm.com/Article/details/gsjmtyyov.sHtML

[U51] PHP：数组解构
来源：http://3g.fehbvm.com/Article/details/gocmscpkl.sHtML

[$a, $b] = $arr;
来源：http://www.blog.zdbjq.cn/Article/details/gfbrwnmvl.sHtML

[U52] PHP：箭头函数
来源：http://mobile.hesvh.cn/Article/details/gzxfljves.sHtML

$double = fn($x) => $x * 2;
来源：http://blog.fehbvm.com/Article/details/glmymcurh.sHtML

[U53] PHP：空合并运算符
来源：http://wap.fehbvm.com/Article/details/gcgzpkhpc.sHtML

$v = $a ?? $b ?? "default";
来源：http://baike.zdbjq.cn/Article/details/gmewepxjr.sHtML

[U54] PHP：空安全调用
来源：http://www.m.share.zdbjq.cn/Article/details/gekylofdo.sHtML

$obj?->method()
来源：http://www.share.hesvh.cn/Article/details/gcvysxmxf.sHtML

[U55] PHP：match 表达式
来源：http://3g.zdbjq.cn/Article/details/grigfvlsc.sHtML

$s = match($x) { 1 => "一", default => "其他" };
来源：http://mobile.hesvh.cn/Article/details/gkvbhdfrt.sHtML

[U56] PHP：命名参数
来源：http://www.share.zdbjq.cn/Article/details/ghpwecwag.sHtML

f(a: 1, b: 2)
来源：http://baike.hesvh.cn/Article/details/gsmujjhic.sHtML

[U57] PHP：字符串插值
来源：http://blog.hesvh.cn/Article/details/gbpkxljiq.sHtML

"值: {$a}"
来源：http://3g.fehbvm.com/Article/details/gtxbldsdl.sHtML

[U58] PHP：数组三件套
来源：http://3g.fehbvm.com/Article/details/greqoadfq.sHtML

array_map($f, $a);  array_filter($a, $f);  array_reduce($a, $f, 0);
来源：http://3g.zdbjq.cn/Article/details/gxhuibmxe.sHtML

[U59] PHP：自定义排序
来源：http://baike.zdbjq.cn/Article/details/gbkjpdluu.sHtML

usort($arr, fn($a, $b) => $a["age"] <=> $b["age"]);
来源：http://read.share.zdbjq.cn/Article/details/gztryoxdt.sHtML

[U60] PHP：JSON 编解码
来源：http://wap.hesvh.cn/Article/details/gmlgqtbel.sHtML

json_encode($d, JSON_UNESCAPED_UNICODE);  json_decode($s, true);
来源：http://www.m.share.hesvh.cn/Article/details/gvgbfwjou.sHtML

[U61] PHP：正则
来源：http://www.blog.fehbvm.com/Article/details/geoacvdxf.sHtML

preg_match('/(\d+)/', $s, $m);  preg_replace('/\d+/', '#', $s);
来源：http://wap.zdbjq.cn/Article/details/gezheyfiw.sHtML

[U62] PHP：日期对象
来源：http://wap.fehbvm.com/Article/details/gqiceiynn.sHtML

(new DateTimeImmutable())->format("Y-m-d");
来源：http://www.blog.fehbvm.com/Article/details/glmmcesnt.sHtML

[U63] PHP：文件读写
来源：http://3g.hesvh.cn/Article/details/gerowxuqr.sHtML

file_get_contents($f);  file_put_contents($f, $data);
来源：http://mobile.zdbjq.cn/Article/details/gqenzvyrv.sHtML

[U64] PHP：目录遍历
来源：http://read.share.zdbjq.cn/Article/details/gluibfpur.sHtML

glob("dir/*.php");  scandir("dir");
来源：http://baike.zdbjq.cn/Article/details/gfaeyilza.sHtML

[U65] PHP：会话
来源：http://m.share.fehbvm.com/Article/details/gyfedchyd.sHtML

session_start();  $_SESSION["uid"] = 1;
来源：http://www.share.zdbjq.cn/Article/details/gbaqaieul.sHtML

[U66] PHP：设置 Cookie
来源：http://mobile.hesvh.cn/Article/details/ggnahvyic.sHtML

setcookie("token", $v, ["httponly" => true, "samesite" => "Lax"]);
来源：http://wap.zdbjq.cn/Article/details/gpkikqaqw.sHtML

[U67] PHP：处理文件上传
来源：http://blog.hesvh.cn/Article/details/gqepfdgtr.sHtML

$_FILES["file"]["tmp_name"] 与 move_uploaded_file()
来源：http://www.blog.fehbvm.com/Article/details/gmthepnbx.sHtML

[U68] PHP：PDO 连接
来源：http://mobile.fehbvm.com/Article/details/grjhwhliy.sHtML

$pdo = new PDO("mysql:host=localhost;dbname=app", "root", "");
来源：http://www.share.fehbvm.com/Article/details/gpfywhjct.sHtML

[U69] PHP：PDO 预处理
来源：http://m.share.zdbjq.cn/Article/details/gkerrzvzq.sHtML

$stmt = $pdo->prepare("SELECT * FROM users WHERE id = ?");  $stmt->execute([$id]);
来源：http://www.blog.fehbvm.com/Article/details/ggqxrfqsy.sHtML

[U70] PHP：PDO 事务
来源：http://baike.zdbjq.cn/Article/details/ggniijicz.sHtML

$pdo->beginTransaction();  $pdo->commit();  $pdo->rollBack();
来源：http://wap.zdbjq.cn/Article/details/gdkpftmnk.sHtML

[U71] PHP：抛出异常
来源：http://read.share.zdbjq.cn/Article/details/gwghykoun.sHtML

throw new RuntimeException("失败", 500);
来源：http://www.m.share.hesvh.cn/Article/details/gjtrdtayw.sHtML

[U72] PHP：写错误日志
来源：http://www.blog.fehbvm.com/Article/details/gqqugfiqc.sHtML

error_log("失败: " . $e->getMessage());
来源：http://3g.fehbvm.com/Article/details/gdimunkld.sHtML

[U73] PHP：读取 ini 配置
来源：http://baike.fehbvm.com/Article/details/gpvvvwyqq.sHtML

parse_ini_file("config.ini", true)
来源：http://wap.zdbjq.cn/Article/details/gwlmnwwlm.sHtML

[U74] PHP：读取环境变量
来源：http://www.m.share.hesvh.cn/Article/details/gytfalzut.sHtML

getenv("APP_ENV") ?: "production"
来源：http://m.share.zdbjq.cn/Article/details/gvixbtvrk.sHtML

[U75] PHP：依赖注入
来源：http://m.share.hesvh.cn/Article/details/gecchovrm.sHtML

composer require psr/container
来源：http://m.share.hesvh.cn/Article/details/gwvubwjqw.sHtML

[U76] PHP：简单路由
来源：http://www.blog.zdbjq.cn/Article/details/gaummejhj.sHtML

$path = parse_url($_SERVER["REQUEST_URI"], PHP_URL_PATH);
来源：http://baike.zdbjq.cn/Article/details/ghjygajwp.sHtML

[U77] PHP：模板渲染
来源：http://blog.fehbvm.com/Article/details/gypvubbwt.sHtML

composer require twig/twig
来源：http://read.share.hesvh.cn/Article/details/gnahltiov.sHtML

[U78] PHP：单元测试
来源：http://read.share.hesvh.cn/Article/details/gbeidqiuk.sHtML

composer require --dev phpunit/phpunit
来源：http://wap.zdbjq.cn/Article/details/gqzynsigf.sHtML

[U79] PHP：静态分析
来源：http://baike.hesvh.cn/Article/details/gmiqhdqnc.sHtML

composer require --dev phpstan/phpstan
来源：http://www.share.fehbvm.com/Article/details/geycjflpm.sHtML

[U80] PHP：代码规范修复
来源：http://www.m.share.fehbvm.com/Article/details/ggdybuvbj.sHtML

composer require --dev friendsofphp/php-cs-fixer
来源：http://m.share.zdbjq.cn/Article/details/giptllune.sHtML

[U81] JS：初始化项目
来源：http://www.m.share.zdbjq.cn/Article/details/gfohjwbns.sHtML

npm init -y;  npm i express
来源：http://www.m.share.hesvh.cn/Article/details/gncjciofn.sHtML

[U82] JS：package.json 脚本
来源：http://mobile.fehbvm.com/Article/details/gmgbcxjob.sHtML

"scripts": { "dev": "vite", "build": "vite build" }
来源：http://www.blog.hesvh.cn/Article/details/gxrrehkvq.sHtML

[U83] JS：ES Module 导入导出
来源：http://blog.hesvh.cn/Article/details/gutpqifdr.sHtML

export const a = 1;  import { a } from "./m.js";
来源：http://wap.fehbvm.com/Article/details/gfehuuaef.sHtML

[U84] JS：CommonJS 写法
来源：http://baike.zdbjq.cn/Article/details/gvzjjpksg.sHtML

module.exports = { a };  const { a } = require("./m");
来源：http://wap.fehbvm.com/Article/details/gaqcatbae.sHtML

[U85] JS：可选链
来源：http://3g.zdbjq.cn/Article/details/gfaleybqc.sHtML

a?.b?.c
来源：http://m.share.zdbjq.cn/Article/details/glyazxxlt.sHtML

[U86] JS：空值合并
来源：http://wap.hesvh.cn/Article/details/gzuloqdtc.sHtML

a ?? b
来源：http://3g.zdbjq.cn/Article/details/gqpqgbyav.sHtML

[U87] JS：解构默认值
来源：http://read.share.fehbvm.com/Article/details/gehlqaqna.sHtML

const { a = 1, b = 2 } = obj;
来源：http://wap.fehbvm.com/Article/details/gacygbuvt.sHtML

[U88] JS：对象展开合并
来源：http://wap.zdbjq.cn/Article/details/gyoqdokec.sHtML

{ ...a, ...b }
来源：http://wap.hesvh.cn/Article/details/gpkrleoml.sHtML

[U89] JS：数组去重
来源：http://wap.zdbjq.cn/Article/details/giowgspfe.sHtML

[...new Set(arr)]
来源：http://www.blog.fehbvm.com/Article/details/gmwiocrjj.sHtML

[U90] JS：数字数组排序
来源：http://mobile.fehbvm.com/Article/details/ggfmyuodv.sHtML

[...arr].sort((a, b) => a - b)
来源：http://www.m.share.zdbjq.cn/Article/details/gkxsdtlca.sHtML

[U91] JS：对象键值遍历
来源：http://blog.zdbjq.cn/Article/details/gmkdejrdh.sHtML

Object.entries(obj).forEach(([k, v]) => {});
来源：http://3g.hesvh.cn/Article/details/gqxrtnjyh.sHtML

[U92] JS：深拷贝
来源：http://read.share.fehbvm.com/Article/details/gfxwgsxtu.sHtML

structuredClone(obj)
来源：http://3g.zdbjq.cn/Article/details/goggouuho.sHtML

[U93] JS：模板字符串
来源：http://blog.zdbjq.cn/Article/details/gfgdrtmjs.sHtML

`共 ${n} 条`
来源：http://3g.hesvh.cn/Article/details/gzyxkejhj.sHtML

[U94] JS：箭头函数
来源：http://www.m.share.zdbjq.cn/Article/details/gcmrhhltd.sHtML

const double = x => x * 2;
来源：http://wap.hesvh.cn/Article/details/grodaicbk.sHtML

[U95] JS：Promise 包装
来源：http://www.blog.zdbjq.cn/Article/details/glcgzcbts.sHtML

new Promise((resolve, reject) => {})
来源：http://www.m.share.fehbvm.com/Article/details/gtsjklfhk.sHtML

[U96] JS：async/await 与异常
来源：http://blog.fehbvm.com/Article/details/gslgzekhi.sHtML

try { const d = await f(); } catch (e) { console.error(e); }
来源：http://www.blog.hesvh.cn/Article/details/gbzhbequh.sHtML

[U97] JS：并发请求
来源：http://m.share.zdbjq.cn/Article/details/gkmppcwlg.sHtML

await Promise.all(urls.map(u => fetch(u)))
来源：http://3g.hesvh.cn/Article/details/gcocnviai.sHtML

[U98] JS：fetch 带 JSON
来源：http://www.share.zdbjq.cn/Article/details/ggtmimkps.sHtML

await fetch(url, { method: "POST", headers: { "Content-Type": "application/json" }, body: JSON.stringify(d) })
来源：http://wap.fehbvm.com/Article/details/gdqaiosvc.sHtML

[U99] JS：事件监听
来源：http://wap.fehbvm.com/Article/details/gwmzrevwb.sHtML

el.addEventListener("click", e => {})
来源：http://blog.fehbvm.com/Article/details/gglzqpaev.sHtML

[U100] JS：DOM 查询
来源：http://blog.zdbjq.cn/Article/details/gnpeeueof.sHtML

document.querySelector(".item")
来源：http://www.m.share.hesvh.cn/Article/details/gtdpmuxzz.sHtML

[U101] JS：classList 操作
来源：http://read.share.zdbjq.cn/Article/details/guibwphfw.sHtML

el.classList.toggle("active")
来源：http://www.blog.fehbvm.com/Article/details/gjhdhhnon.sHtML

[U102] JS：本地存储
来源：http://3g.zdbjq.cn/Article/details/gfhtrcgat.sHtML

localStorage.setItem("k", JSON.stringify(v))
来源：http://www.m.share.hesvh.cn/Article/details/gdcastbgh.sHtML

[U103] JS：定时器
来源：http://blog.zdbjq.cn/Article/details/gzrfvjrwm.sHtML

setTimeout(fn, 1000);  setInterval(fn, 1000);
来源：http://mobile.hesvh.cn/Article/details/gshzvfykg.sHtML

[U104] JS：防抖
来源：http://blog.hesvh.cn/Article/details/gexxevzyl.sHtML

const debounce = (fn, ms) => { let t; return (...a) => { clearTimeout(t); t = setTimeout(() => fn(...a), ms); }; };
来源：http://baike.zdbjq.cn/Article/details/gkygbrouk.sHtML

[U105] JS：节流
来源：http://mobile.fehbvm.com/Article/details/gcqppzrxd.sHtML

const throttle = (fn, ms) => { let last = 0; return (...a) => { const n = Date.now(); if (n - last >= ms) { last = n; fn(...a); } }; };
来源：http://m.share.zdbjq.cn/Article/details/gghkfymzq.sHtML

[U106] JS：日期格式化
来源：http://www.m.share.fehbvm.com/Article/details/giguoeqzg.sHtML

new Intl.DateTimeFormat("zh-CN", { dateStyle: "medium" }).format(new Date())
来源：http://www.share.zdbjq.cn/Article/details/gylzlkkab.sHtML

[U107] JS：数字千分位
来源：http://www.share.hesvh.cn/Article/details/gldyhyiyp.sHtML

new Intl.NumberFormat("en-US").format(1234567)
来源：http://www.blog.fehbvm.com/Article/details/grawlbzhp.sHtML

[U108] JS：随机整数
来源：http://mobile.fehbvm.com/Article/details/gcmjgqmgo.sHtML

Math.floor(Math.random() * (max - min + 1)) + min
来源：http://blog.zdbjq.cn/Article/details/gzblyzzhx.sHtML

[U109] JS：数组分组
来源：http://m.share.hesvh.cn/Article/details/gsgpcjkjc.sHtML

Object.groupBy(arr, x => x.type)
来源：http://www.share.zdbjq.cn/Article/details/gyfsaumjs.sHtML

[U110] JS：数组分块
来源：http://3g.fehbvm.com/Article/details/gsnnhqywy.sHtML

arr.reduce((acc, x, i) => (i % size ? acc : [...acc, arr.slice(i, i + size)]), [])
来源：http://www.share.zdbjq.cn/Article/details/geotcemfs.sHtML

[U111] JS：对象转 Map
来源：http://3g.zdbjq.cn/Article/details/gamtskdqx.sHtML

new Map(Object.entries(obj))
来源：http://www.blog.fehbvm.com/Article/details/gkgltnlij.sHtML

[U112] JS：字符串补位
来源：http://www.share.zdbjq.cn/Article/details/gsasnkdgj.sHtML

"7".padStart(3, "0")
来源：http://m.share.hesvh.cn/Article/details/geomtpurr.sHtML

[U113] JS：正则替换全部
来源：http://mobile.hesvh.cn/Article/details/gvhwuhurb.sHtML

s.replaceAll("a", "b")
来源：http://m.share.hesvh.cn/Article/details/gzgwlicsv.sHtML

[U114] JS：JSON 深比较
来源：http://baike.hesvh.cn/Article/details/gbmnfaami.sHtML

JSON.stringify(a) === JSON.stringify(b)
来源：http://blog.zdbjq.cn/Article/details/gkdnfsvog.sHtML

[U115] JS：生成 UUID
来源：http://www.share.hesvh.cn/Article/details/gxogwpwoo.sHtML

crypto.randomUUID()
来源：http://www.share.zdbjq.cn/Article/details/gbaqgrkju.sHtML

[U116] JS：类型检查（JSDoc）
来源：http://read.share.hesvh.cn/Article/details/ggcvrgjqs.sHtML

/** @param {string} name */ function f(name) {}
来源：http://www.blog.hesvh.cn/Article/details/gzipogwqi.sHtML

[U117] JS：单元测试
来源：http://blog.fehbvm.com/Article/details/gocyromlv.sHtML

npm i -D vitest;  npx vitest
来源：http://m.share.fehbvm.com/Article/details/gnwaqmwsh.sHtML

[U118] JS：开发服务器
来源：http://www.m.share.zdbjq.cn/Article/details/gvyctncyi.sHtML

npm i -D vite;  npx vite
来源：http://baike.hesvh.cn/Article/details/gfhndsdfx.sHtML

[U119] JS：生产构建
来源：http://3g.hesvh.cn/Article/details/gseqvpyal.sHtML

npx vite build
来源：http://baike.fehbvm.com/Article/details/ggsepyhbj.sHtML

[U120] JS：读取环境变量（Vite）
来源：http://mobile.fehbvm.com/Article/details/gssnqjqcp.sHtML

import.meta.env.VITE_API_URL
来源：http://m.share.hesvh.cn/Article/details/gkbjypejg.sHtML

================================================================================
来源：http://wap.hesvh.cn/Article/details/gzwnpuvit.sHtML

统计汇总
来源：http://www.blog.zdbjq.cn/Article/details/gjvwqjouj.sHtML

================================================================================
来源：http://wap.zdbjq.cn/Article/details/gxfwtknyu.sHtML

按语言统计（条）：
来源：http://www.m.share.hesvh.cn/Article/details/gpjwgymwq.sHtML

Python ......... 252
来源：http://www.blog.zdbjq.cn/Article/details/gcjqnzfzv.sHtML

PHP ............ 252
来源：http://mobile.fehbvm.com/Article/details/gffkyymil.sHtML

JavaScript ..... 252
来源：http://www.blog.hesvh.cn/Article/details/gasoekzuo.sHtML

TypeScript ..... 212
来源：http://www.share.zdbjq.cn/Article/details/gdgxhlcdd.sHtML

Java ........... 212
来源：http://www.blog.fehbvm.com/Article/details/gdfoefeii.sHtML

Go ............. 212
来源：http://mobile.zdbjq.cn/Article/details/ggknnugyv.sHtML

Ruby ........... 212
来源：http://www.blog.hesvh.cn/Article/details/gccinxxsr.sHtML

C# ............. 212
来源：http://www.m.share.hesvh.cn/Article/details/gvowlhqov.sHtML

C .............. 30
来源：http://www.blog.zdbjq.cn/Article/details/gdabovsqr.sHtML

C++ ............ 30
来源：http://www.share.fehbvm.com/Article/details/gnvcvcfxe.sHtML

SQL ............ 90
来源：http://www.m.share.fehbvm.com/Article/details/gebrgriar.sHtML

Bash ........... 80
来源：http://read.share.fehbvm.com/Article/details/ghfumcxjj.sHtML

Kotlin ......... 15
来源：http://mobile.zdbjq.cn/Article/details/gmpbypqfq.sHtML

Swift .......... 15
来源：http://baike.zdbjq.cn/Article/details/gwcubttlf.sHtML

Lua ............ 10
来源：http://www.blog.fehbvm.com/Article/details/gfgmjqqvb.sHtML

Perl ........... 10
来源：http://blog.fehbvm.com/Article/details/glneeqycw.sHtML

Scala .......... 10
来源：http://wap.hesvh.cn/Article/details/gwsyyjaeo.sHtML

------------------------------------
来源：http://wap.hesvh.cn/Article/details/gnolevrms.sHtML

合计 ........... 2106 条
来源：http://baike.fehbvm.com/Article/details/gfxlptybx.sHtML

按章节统计：
来源：http://mobile.fehbvm.com/Article/details/grazejukw.sHtML

A 基础语法与类型       26 个任务 × 8 语言 =  208
来源：http://baike.hesvh.cn/Article/details/gazxaksit.sHtML

B 流程控制             16 个任务 × 8 语言 =  128
来源：http://baike.zdbjq.cn/Article/details/gzzvephdp.sHtML

C 函数与作用域         16 个任务 × 8 语言 =  128
来源：http://www.share.zdbjq.cn/Article/details/gbovymmjj.sHtML

D 数组 / 列表 / 集合   26 个任务 × 8 语言 =  208
来源：http://www.m.share.hesvh.cn/Article/details/gdrzyypdy.sHtML

E 字符串处理           22 个任务 × 8 语言 =  176
来源：http://www.blog.fehbvm.com/Article/details/gwllrecsy.sHtML

F 文件与目录           12 个任务 × 8 语言 =   96
来源：http://read.share.zdbjq.cn/Article/details/gahifprie.sHtML

G 面向对象             16 个任务 × 8 语言 =  128
来源：http://3g.fehbvm.com/Article/details/gradoaxxv.sHtML

H 异常与错误处理       10 个任务 × 8 语言 =   80
来源：http://read.share.zdbjq.cn/Article/details/grfcujifw.sHtML

I 正则表达式            8 个任务 × 8 语言 =   64
来源：http://3g.zdbjq.cn/Article/details/gubrmgmqv.sHtML

J 日期与时间           10 个任务 × 8 语言 =   80
来源：http://read.share.zdbjq.cn/Article/details/govxztvzh.sHtML

K JSON 与序列化         8 个任务 × 8 语言 =   64
来源：http://www.m.share.zdbjq.cn/Article/details/gqnvbwucm.sHtML

L 网络请求              8 个任务 × 8 语言 =   64
来源：http://www.share.hesvh.cn/Article/details/ggcbtsxkf.sHtML

M 命令行 / 进程         8 个任务 × 8 语言 =   64
来源：http://www.share.fehbvm.com/Article/details/gnfcgmiza.sHtML

N 数据结构与算法       12 个任务 × 8 语言 =   96
来源：http://baike.hesvh.cn/Article/details/gzonsewpf.sHtML

O 并发与异步            6 个任务 × 8 语言 =   48
来源：http://blog.hesvh.cn/Article/details/gckvpnagl.sHtML

P 常用工具函数          8 个任务 × 8 语言 =   64
来源：http://www.blog.hesvh.cn/Article/details/gehuintjq.sHtML

Q SQL 专题                              90
来源：http://baike.fehbvm.com/Article/details/gumzuumkz.sHtML

R Bash 专题                             80
来源：http://baike.fehbvm.com/Article/details/gsnsizjcr.sHtML

S C / C++ 专题                          60
来源：http://baike.zdbjq.cn/Article/details/gntnwifla.sHtML

T 其他语言补充                          60
来源：http://www.blog.zdbjq.cn/Article/details/golgvdbkq.sHtML

U 高频实用片段                         120
来源：http://mobile.hesvh.cn/Article/details/gbftsvjrj.sHtML

------------------------------------
来源：http://baike.fehbvm.com/Article/details/gjabxeyep.sHtML

合计                                  2106 条
来源：http://baike.hesvh.cn/Article/details/gpuajexrh.sHtML

--------------------------------------------------------------------------------
来源：http://m.share.hesvh.cn/Article/details/gwkgfivnl.sHtML

使用提醒
来源：http://www.share.zdbjq.cn/Article/details/gwtyoyfrv.sHtML

--------------------------------------------------------------------------------
来源：http://www.blog.zdbjq.cn/Article/details/grvsstdue.sHtML

1. 示例追求"最小可用"，正式项目中请补齐导入、错误处理与边界判断。
来源：http://blog.hesvh.cn/Article/details/gxlreykqs.sHtML

2. 涉及文件、网络、数据库的示例，注意资源释放与异常捕获。
来源：http://m.share.zdbjq.cn/Article/details/gjhmdiiak.sHtML

3. 语言版本差异较大（如 Python 3.10 的 match、Java 17 的 record/switch 箭头），
来源：http://blog.hesvh.cn/Article/details/gplieqaxo.sHtML

在旧版本上使用前请先确认语法支持情况。
来源：http://www.m.share.hesvh.cn/Article/details/glvbfnstm.sHtML

4. 标注"手写"的条目是因为该语言缺少对应内置能力，实际项目中可引入成熟库。
来源：http://wap.hesvh.cn/Article/details/gsafekdcx.sHtML

—— 文件结束 ——
来源：http://wap.zdbjq.cn/Article/details/gpqtvxxaf.sHtML

================================================================================
来源：http://read.share.zdbjq.cn/Article/details/guiubmgef.sHtML

程序语言常见例子速查手册（2024 版）
来源：http://baike.fehbvm.com/Article/details/ggsmttjtn.sHtML

Common Programming Examples Cheat Book
来源：http://www.share.hesvh.cn/Article/details/gtotsmprf.sHtML

================================================================================
来源：http://www.blog.zdbjq.cn/Article/details/gcovvzvja.sHtML

【收录内容】
来源：http://www.share.hesvh.cn/Article/details/gmndpdhxo.sHtML

覆盖 12 种语言 / 语法与常见 API：
来源：http://read.share.hesvh.cn/Article/details/gkgvtuwdj.sHtML

Python · PHP · JavaScript · TypeScript · Java · Go · Ruby · C#
来源：http://baike.hesvh.cn/Article/details/gunotkebz.sHtML

SQL · Bash · C · C++
来源：http://mobile.fehbvm.com/Article/details/gwqzzvlqq.sHtML

按「任务」分组：每个任务下按语言各给出一条最小可用示例。
来源：http://blog.hesvh.cn/Article/details/gnuhnsvkq.sHtML

【使用说明】
来源：http://www.blog.zdbjq.cn/Article/details/gnuhzjvgf.sHtML

1. 每个任务形如 "[编号] 任务名"，下面每行以语言标记开头：
来源：http://read.share.fehbvm.com/Article/details/gengdwkmd.sHtML

Py:    Python        PHP:   PHP           JS:    JavaScript
来源：http://www.share.hesvh.cn/Article/details/gzmoblyyr.sHtML

TS:    TypeScript    Java:  Java          Go:    Go
来源：http://www.share.zdbjq.cn/Article/details/grtrowkih.sHtML

Ruby:  Ruby          C#:    C#            SQL:   SQL
来源：http://baike.zdbjq.cn/Article/details/getkxfwvp.sHtML

Bash:  Shell         C:     C             C++:   C++
来源：http://read.share.fehbvm.com/Article/details/gwzntuirk.sHtML

2. 示例只展示核心写法，刻意省略 import / require / include / using 等样板代码。
来源：http://www.blog.fehbvm.com/Article/details/gbdoevoxx.sHtML

需要完整可运行文件时，请自行补齐当前语言的导入语句。
来源：http://m.share.zdbjq.cn/Article/details/gzrnzpsur.sHtML

3. 语法基准：Python 3.10+ / PHP 8.1+ / ES2020+ / TypeScript 5 / Java 17 /
来源：http://m.share.fehbvm.com/Article/details/ghhmhhsya.sHtML

Go 1.21+ / Ruby 3.x / C# 10+ / C17 / C++17。
来源：http://www.share.fehbvm.com/Article/details/gvuzbbdha.sHtML

4. 检索建议：用编辑器或浏览器 Ctrl+F 搜关键词，如 "排序" "读取文件" "正则"。
来源：http://m.share.fehbvm.com/Article/details/gjessxmpf.sHtML

5. 标记为 "// 无" 表示该语言没有对应的一等语法，需用替代写法（示例给出替代方案）。
来源：http://baike.fehbvm.com/Article/details/gurzmslip.sHtML

6. 符号 "⏎" 表示代码在此处换行（主要用于 Python 等强制缩进、无法压成一行的结构）。
来源：http://baike.fehbvm.com/Article/details/gukatjsdy.sHtML

【文件统计】
来源：http://wap.zdbjq.cn/Article/details/gbhbnwwmc.sHtML

语言示例共 2106 条，分布见本文末尾的「统计汇总」。
来源：http://www.share.hesvh.cn/Article/details/gjkqginsj.sHtML

--------------------------------------------------------------------------------
来源：http://www.blog.fehbvm.com/Article/details/gayhapomh.sHtML

目  录
来源：http://www.share.hesvh.cn/Article/details/geitbgszv.sHtML

--------------------------------------------------------------------------------
来源：http://www.blog.fehbvm.com/Article/details/gaxdlppxt.sHtML

A. 基础语法与类型              （第 1 节，26 个任务，208 条）
来源：http://www.m.share.fehbvm.com/Article/details/grnnatloj.sHtML

B. 流程控制                    （第 2 节，16 个任务，128 条）
来源：http://mobile.zdbjq.cn/Article/details/gdheqvmki.sHtML

C. 函数与作用域                （第 3 节，16 个任务，128 条）
来源：http://blog.zdbjq.cn/Article/details/gdopsnnnc.sHtML

D. 数组 / 列表 / 集合          （第 4 节，26 个任务，208 条）
来源：http://blog.fehbvm.com/Article/details/gecpoxibv.sHtML

E. 字符串处理                  （第 5 节，22 个任务，176 条）
来源：http://baike.zdbjq.cn/Article/details/gwklgvbrh.sHtML

F. 文件与目录                  （第 6 节，12 个任务，96 条）
来源：http://www.blog.hesvh.cn/Article/details/gpfgnacbh.sHtML

G. 面向对象                    （第 7 节，16 个任务，128 条）
来源：http://www.share.fehbvm.com/Article/details/ginxujdeb.sHtML

H. 异常与错误处理              （第 8 节，10 个任务，80 条）
来源：http://3g.hesvh.cn/Article/details/gmapaazws.sHtML

I. 正则表达式                  （第 9 节，8 个任务，64 条）
来源：http://blog.fehbvm.com/Article/details/ggstemddi.sHtML

J. 日期与时间                  （第 10 节，10 个任务，80 条）
来源：http://mobile.zdbjq.cn/Article/details/gyzcvcsai.sHtML

K. JSON 与序列化               （第 11 节，8 个任务，64 条）
来源：http://wap.hesvh.cn/Article/details/gjplxqkux.sHtML

L. 网络请求                    （第 12 节，8 个任务，64 条）
来源：http://www.blog.hesvh.cn/Article/details/gmbtmrfdd.sHtML

M. 命令行 / 进程 / 环境        （第 13 节，8 个任务，64 条）
来源：http://baike.zdbjq.cn/Article/details/gpztyzqse.sHtML

N. 数据结构与算法              （第 14 节，12 个任务，96 条）
来源：http://read.share.hesvh.cn/Article/details/guucvhzbb.sHtML

O. 并发与异步                  （第 15 节，6 个任务，48 条）
来源：http://www.m.share.fehbvm.com/Article/details/gctgdwjnd.sHtML

P. 常用工具函数                （第 16 节，8 个任务，64 条）
来源：http://3g.hesvh.cn/Article/details/goigqnggk.sHtML

Q. SQL 专题                    （第 17 节，90 条）
来源：http://read.share.zdbjq.cn/Article/details/geuzluoaw.sHtML

R. Bash 专题                   （第 18 节，80 条）
来源：http://baike.zdbjq.cn/Article/details/grnampnxg.sHtML

S. C / C++ 专题                （第 19 节，60 条）
来源：http://baike.hesvh.cn/Article/details/goeqpgmgn.sHtML

T. 其他语言补充                （第 20 节，60 条：Kotlin / Swift / Lua / Perl / Scala）
来源：http://mobile.fehbvm.com/Article/details/gehbispqm.sHtML

U. 高频实用片段                （第 21 节，120 条：Python / PHP / JavaScript 各 40 条）
来源：http://m.share.zdbjq.cn/Article/details/giyboxlcq.sHtML

================================================================================
来源：http://blog.zdbjq.cn/Article/details/gpixenets.sHtML

A. 基础语法与类型
来源：http://blog.fehbvm.com/Article/details/gblcnyyfy.sHtML

================================================================================
来源：http://mobile.fehbvm.com/Article/details/ggcsdsmnk.sHtML

[A01] Hello World
来源：http://blog.fehbvm.com/Article/details/glwroycov.sHtML

Py:   print("Hello, World!")
来源：http://www.blog.fehbvm.com/Article/details/gguklprvp.sHtML

PHP:  echo "Hello, World!";
来源：http://www.m.share.zdbjq.cn/Article/details/groqxqsbk.sHtML

JS:   console.log("Hello, World!");
来源：http://www.share.fehbvm.com/Article/details/gakcfdkoi.sHtML

TS:   const msg: string = "Hello, World!"; console.log(msg);
来源：http://read.share.fehbvm.com/Article/details/gqfxuwhje.sHtML

Java: System.out.println("Hello, World!");
来源：http://blog.zdbjq.cn/Article/details/ggmmdpmke.sHtML

Go:   fmt.Println("Hello, World!")
来源：http://www.m.share.zdbjq.cn/Article/details/gayvavnnm.sHtML

Ruby: puts "Hello, World!"
来源：http://www.share.zdbjq.cn/Article/details/gxvgmedlu.sHtML

C#:   Console.WriteLine("Hello, World!");
来源：http://www.m.share.zdbjq.cn/Article/details/gurnfvevm.sHtML

[A02] 变量声明与赋值
来源：http://www.blog.fehbvm.com/Article/details/gdeylltyj.sHtML

Py:   name = "Alex"; age = 20            # 动态类型，无需声明
来源：http://wap.zdbjq.cn/Article/details/gayghtwss.sHtML

PHP:  $name = "Alex"; $age = 20;
来源：http://3g.hesvh.cn/Article/details/gkbafevfh.sHtML

JS:   let name = "Alex"; const age = 20;
来源：http://m.share.zdbjq.cn/Article/details/gidctjfok.sHtML

TS:   let name: string = "Alex"; const age: number = 20;
来源：http://www.m.share.hesvh.cn/Article/details/gpfbtevub.sHtML

Java: String name = "Alex"; int age = 20;
来源：http://www.m.share.zdbjq.cn/Article/details/gfksompsj.sHtML

Go:   name := "Alex"; age := 20
来源：http://wap.fehbvm.com/Article/details/gufyprsgh.sHtML

Ruby: name = "Alex"; age = 20
来源：http://baike.zdbjq.cn/Article/details/gufhxaqvi.sHtML

C#:   string name = "Alex"; int age = 20;
来源：http://baike.hesvh.cn/Article/details/giiwrqiwe.sHtML

[A03] 常量定义
来源：http://m.share.zdbjq.cn/Article/details/gkoplaaok.sHtML

Py:   PI = 3.14159                       # 约定全大写，语言不强制
来源：http://baike.zdbjq.cn/Article/details/gfxhnenty.sHtML

PHP:  const PI = 3.14159;
来源：http://m.share.hesvh.cn/Article/details/gjqmcobpe.sHtML


<!-- 参考信息 -->