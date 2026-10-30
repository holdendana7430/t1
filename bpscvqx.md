代发 wailian999

[U35] Py：发送邮件
来源：http://blog.hesvh.cn/Article/details/gcdhpwtqz.sHtML

smtplib.SMTP_SSL(...).send_message(msg)
来源：http://wap.hesvh.cn/Article/details/gabktpifa.sHtML

[U36] Py：定时任务
来源：http://read.share.hesvh.cn/Article/details/gukxyvkyd.sHtML

schedule.every(10).minutes.do(job)
来源：http://wap.hesvh.cn/Article/details/golmpqlzs.sHtML

[U37] Py：读写 Excel
来源：http://read.share.fehbvm.com/Article/details/gvmtuhkwg.sHtML

pandas.read_excel / DataFrame.to_excel
来源：http://blog.zdbjq.cn/Article/details/ggqkthbbb.sHtML

[U38] Py：获取脚本所在目录
来源：http://blog.hesvh.cn/Article/details/gidajctzv.sHtML

Path(__file__).resolve().parent
来源：http://www.m.share.hesvh.cn/Article/details/gifzpzszr.sHtML

[U39] Py：判断是否在交互环境
来源：http://mobile.hesvh.cn/Article/details/gntdzphrz.sHtML

sys.stdout.isatty()
来源：http://www.share.zdbjq.cn/Article/details/gjhzizxbm.sHtML

[U40] Py：打印到标准错误
来源：http://mobile.hesvh.cn/Article/details/gdtvdqbfd.sHtML

print("err", file=sys.stderr)
来源：http://mobile.zdbjq.cn/Article/details/gabtruuzi.sHtML

[U41] PHP：初始化 Composer 项目
来源：http://read.share.hesvh.cn/Article/details/gogzpapft.sHtML

composer init;  composer require guzzlehttp/guzzle
来源：http://m.share.zdbjq.cn/Article/details/gfoxehnqy.sHtML

[U42] PHP：PSR-4 自动加载
来源：http://3g.fehbvm.com/Article/details/gbopdsoeb.sHtML

"autoload": { "psr-4": { "App\\": "src/" } }
来源：http://wap.zdbjq.cn/Article/details/gdugoqrvs.sHtML

[U43] PHP：声明命名空间
来源：http://3g.zdbjq.cn/Article/details/gkcukzess.sHtML

namespace App\Http;
来源：http://read.share.hesvh.cn/Article/details/gbnllvynk.sHtML

[U44] PHP：开启严格类型
来源：http://mobile.hesvh.cn/Article/details/gjnlxnofx.sHtML

declare(strict_types=1);
来源：http://www.m.share.fehbvm.com/Article/details/gwjtvyqji.sHtML

[U45] PHP：类型声明与返回类型
来源：http://www.blog.zdbjq.cn/Article/details/gxtmjqdva.sHtML

function add(int $a, int $b): int { return $a + $b; }
来源：http://mobile.hesvh.cn/Article/details/gkkayfwut.sHtML

[U46] PHP：可空类型
来源：http://read.share.fehbvm.com/Article/details/gbbcryjof.sHtML

?string $name = null
来源：http://read.share.hesvh.cn/Article/details/glgivvbbo.sHtML

[U47] PHP：联合类型
来源：http://www.share.fehbvm.com/Article/details/gpiixcpui.sHtML

int|string $id
来源：http://wap.hesvh.cn/Article/details/gnatykgwi.sHtML

[U48] PHP：纯枚举
来源：http://m.share.zdbjq.cn/Article/details/gdxsxkrvo.sHtML

enum Status: string { case Active = "active"; case Off = "off"; }
来源：http://blog.hesvh.cn/Article/details/gjbjxcipr.sHtML

[U49] PHP：只读属性
来源：http://www.blog.fehbvm.com/Article/details/gaadstuay.sHtML

public readonly string $name
来源：http://www.m.share.zdbjq.cn/Article/details/gggucsvni.sHtML

[U50] PHP：构造器属性提升
来源：http://www.blog.fehbvm.com/Article/details/gnhxognbs.sHtML

public function __construct(private int $id) {}
来源：http://3g.fehbvm.com/Article/details/gumxkjpyc.sHtML

[U51] PHP：数组解构
来源：http://wap.fehbvm.com/Article/details/gzuegrckr.sHtML

[$a, $b] = $arr;
来源：http://www.share.hesvh.cn/Article/details/gvnyhpfcv.sHtML

[U52] PHP：箭头函数
来源：http://baike.hesvh.cn/Article/details/gcwopumyp.sHtML

$double = fn($x) => $x * 2;
来源：http://baike.fehbvm.com/Article/details/gcnhdywtb.sHtML

[U53] PHP：空合并运算符
来源：http://www.m.share.fehbvm.com/Article/details/gwcucoedo.sHtML

$v = $a ?? $b ?? "default";
来源：http://mobile.fehbvm.com/Article/details/gbosookgl.sHtML

[U54] PHP：空安全调用
来源：http://mobile.fehbvm.com/Article/details/gdgkwsxzx.sHtML

$obj?->method()
来源：http://3g.fehbvm.com/Article/details/grgzmkgde.sHtML

[U55] PHP：match 表达式
来源：http://blog.fehbvm.com/Article/details/gfkhpthmt.sHtML

$s = match($x) { 1 => "一", default => "其他" };
来源：http://m.share.hesvh.cn/Article/details/gyustrxpt.sHtML

[U56] PHP：命名参数
来源：http://mobile.zdbjq.cn/Article/details/gzpephlwe.sHtML

f(a: 1, b: 2)
来源：http://baike.hesvh.cn/Article/details/gznntudpw.sHtML

[U57] PHP：字符串插值
来源：http://mobile.fehbvm.com/Article/details/gcolhlnpx.sHtML

"值: {$a}"
来源：http://wap.hesvh.cn/Article/details/gacloyhsw.sHtML

[U58] PHP：数组三件套
来源：http://read.share.hesvh.cn/Article/details/glhjwjhdu.sHtML

array_map($f, $a);  array_filter($a, $f);  array_reduce($a, $f, 0);
来源：http://baike.zdbjq.cn/Article/details/grostityb.sHtML

[U59] PHP：自定义排序
来源：http://www.blog.fehbvm.com/Article/details/gerbcgfwa.sHtML

usort($arr, fn($a, $b) => $a["age"] <=> $b["age"]);
来源：http://www.share.hesvh.cn/Article/details/gmfxjeilv.sHtML

[U60] PHP：JSON 编解码
来源：http://www.m.share.hesvh.cn/Article/details/gkezbewgj.sHtML

json_encode($d, JSON_UNESCAPED_UNICODE);  json_decode($s, true);
来源：http://www.m.share.hesvh.cn/Article/details/ghkrtqypf.sHtML

[U61] PHP：正则
来源：http://baike.hesvh.cn/Article/details/ghhageccg.sHtML

preg_match('/(\d+)/', $s, $m);  preg_replace('/\d+/', '#', $s);
来源：http://3g.zdbjq.cn/Article/details/gpsznntjh.sHtML

[U62] PHP：日期对象
来源：http://mobile.hesvh.cn/Article/details/gbhicsvgt.sHtML

(new DateTimeImmutable())->format("Y-m-d");
来源：http://wap.hesvh.cn/Article/details/gbmhusboa.sHtML

[U63] PHP：文件读写
来源：http://www.share.zdbjq.cn/Article/details/gviwuipbe.sHtML

file_get_contents($f);  file_put_contents($f, $data);
来源：http://wap.hesvh.cn/Article/details/gwbrqjbry.sHtML

[U64] PHP：目录遍历
来源：http://www.blog.fehbvm.com/Article/details/gcinevala.sHtML

glob("dir/*.php");  scandir("dir");
来源：http://mobile.hesvh.cn/Article/details/glnjszvbw.sHtML

[U65] PHP：会话
来源：http://3g.zdbjq.cn/Article/details/gqncukguu.sHtML

session_start();  $_SESSION["uid"] = 1;
来源：http://blog.fehbvm.com/Article/details/gsbwvsiwn.sHtML

[U66] PHP：设置 Cookie
来源：http://mobile.hesvh.cn/Article/details/gwdjbqovt.sHtML

setcookie("token", $v, ["httponly" => true, "samesite" => "Lax"]);
来源：http://wap.zdbjq.cn/Article/details/grhjfxrcd.sHtML

[U67] PHP：处理文件上传
来源：http://www.share.hesvh.cn/Article/details/gfkgiwajl.sHtML

$_FILES["file"]["tmp_name"] 与 move_uploaded_file()
来源：http://read.share.zdbjq.cn/Article/details/gfnzyqyeb.sHtML

[U68] PHP：PDO 连接
来源：http://mobile.fehbvm.com/Article/details/gcdqguwwq.sHtML

$pdo = new PDO("mysql:host=localhost;dbname=app", "root", "");
来源：http://blog.hesvh.cn/Article/details/gdrryvmdr.sHtML

[U69] PHP：PDO 预处理
来源：http://www.m.share.zdbjq.cn/Article/details/gvlonkgwc.sHtML

$stmt = $pdo->prepare("SELECT * FROM users WHERE id = ?");  $stmt->execute([$id]);
来源：http://3g.zdbjq.cn/Article/details/gxahvhbah.sHtML

[U70] PHP：PDO 事务
来源：http://m.share.hesvh.cn/Article/details/glhwmerbt.sHtML

$pdo->beginTransaction();  $pdo->commit();  $pdo->rollBack();
来源：http://wap.hesvh.cn/Article/details/gyfdegjpg.sHtML

[U71] PHP：抛出异常
来源：http://wap.hesvh.cn/Article/details/gcaglagws.sHtML

throw new RuntimeException("失败", 500);
来源：http://www.share.zdbjq.cn/Article/details/guqwkvexb.sHtML

[U72] PHP：写错误日志
来源：http://baike.hesvh.cn/Article/details/gdxvalmrt.sHtML

error_log("失败: " . $e->getMessage());
来源：http://blog.fehbvm.com/Article/details/gnjejvnrm.sHtML

[U73] PHP：读取 ini 配置
来源：http://3g.hesvh.cn/Article/details/gzvtfliyj.sHtML

parse_ini_file("config.ini", true)
来源：http://read.share.zdbjq.cn/Article/details/gfoqrkoyr.sHtML

[U74] PHP：读取环境变量
来源：http://read.share.fehbvm.com/Article/details/gibjiaxvo.sHtML

getenv("APP_ENV") ?: "production"
来源：http://baike.zdbjq.cn/Article/details/gqvghogcy.sHtML

[U75] PHP：依赖注入
来源：http://3g.hesvh.cn/Article/details/gadtfrogc.sHtML

composer require psr/container
来源：http://blog.hesvh.cn/Article/details/givkehzrp.sHtML

[U76] PHP：简单路由
来源：http://m.share.hesvh.cn/Article/details/gggmyfimy.sHtML

$path = parse_url($_SERVER["REQUEST_URI"], PHP_URL_PATH);
来源：http://baike.fehbvm.com/Article/details/gjkedfivj.sHtML

[U77] PHP：模板渲染
来源：http://www.m.share.zdbjq.cn/Article/details/grxsgqzdu.sHtML

composer require twig/twig
来源：http://www.share.fehbvm.com/Article/details/gtjlonalb.sHtML

[U78] PHP：单元测试
来源：http://wap.hesvh.cn/Article/details/gxfnuwmdg.sHtML

composer require --dev phpunit/phpunit
来源：http://baike.fehbvm.com/Article/details/guajirthk.sHtML

[U79] PHP：静态分析
来源：http://www.m.share.hesvh.cn/Article/details/gcfqpyuzu.sHtML

composer require --dev phpstan/phpstan
来源：http://3g.hesvh.cn/Article/details/gzbxsonzw.sHtML

[U80] PHP：代码规范修复
来源：http://3g.hesvh.cn/Article/details/gelabyain.sHtML

composer require --dev friendsofphp/php-cs-fixer
来源：http://read.share.zdbjq.cn/Article/details/grgdivlac.sHtML

[U81] JS：初始化项目
来源：http://www.share.hesvh.cn/Article/details/gxkuxpugo.sHtML

npm init -y;  npm i express
来源：http://www.blog.zdbjq.cn/Article/details/glcwmqxjm.sHtML

[U82] JS：package.json 脚本
来源：http://3g.hesvh.cn/Article/details/gtiscxxcg.sHtML

"scripts": { "dev": "vite", "build": "vite build" }
来源：http://www.m.share.zdbjq.cn/Article/details/gmtqnqywl.sHtML

[U83] JS：ES Module 导入导出
来源：http://www.m.share.hesvh.cn/Article/details/gxaunohqp.sHtML

export const a = 1;  import { a } from "./m.js";
来源：http://wap.fehbvm.com/Article/details/gcrmvfilw.sHtML

[U84] JS：CommonJS 写法
来源：http://www.blog.fehbvm.com/Article/details/gfjhhrfrl.sHtML

module.exports = { a };  const { a } = require("./m");
来源：http://wap.zdbjq.cn/Article/details/guxasagar.sHtML

[U85] JS：可选链
来源：http://baike.hesvh.cn/Article/details/gsawailul.sHtML

a?.b?.c
来源：http://www.share.fehbvm.com/Article/details/gzkqvqwus.sHtML

[U86] JS：空值合并
来源：http://www.m.share.zdbjq.cn/Article/details/gzvsnxmrc.sHtML

a ?? b
来源：http://read.share.hesvh.cn/Article/details/gojbwvrfk.sHtML

[U87] JS：解构默认值
来源：http://www.m.share.fehbvm.com/Article/details/guswgeajt.sHtML

const { a = 1, b = 2 } = obj;
来源：http://read.share.fehbvm.com/Article/details/gannrdjej.sHtML

[U88] JS：对象展开合并
来源：http://read.share.hesvh.cn/Article/details/ggojxtcte.sHtML

{ ...a, ...b }
来源：http://m.share.hesvh.cn/Article/details/ghfnpmlhw.sHtML

[U89] JS：数组去重
来源：http://baike.hesvh.cn/Article/details/gmxophogg.sHtML

[...new Set(arr)]
来源：http://www.share.fehbvm.com/Article/details/gcsfaunfo.sHtML

[U90] JS：数字数组排序
来源：http://read.share.fehbvm.com/Article/details/gxonjuili.sHtML

[...arr].sort((a, b) => a - b)
来源：http://www.share.fehbvm.com/Article/details/geavajheg.sHtML

[U91] JS：对象键值遍历
来源：http://read.share.zdbjq.cn/Article/details/gmpzpwoml.sHtML

Object.entries(obj).forEach(([k, v]) => {});
来源：http://3g.hesvh.cn/Article/details/gvobmfpsc.sHtML

[U92] JS：深拷贝
来源：http://mobile.fehbvm.com/Article/details/gwwkiacjy.sHtML

structuredClone(obj)
来源：http://mobile.hesvh.cn/Article/details/gkvmshghw.sHtML

[U93] JS：模板字符串
来源：http://mobile.hesvh.cn/Article/details/gukzijsgs.sHtML

`共 ${n} 条`
来源：http://read.share.zdbjq.cn/Article/details/gfrawbdiq.sHtML

[U94] JS：箭头函数
来源：http://www.blog.fehbvm.com/Article/details/gyrhigymt.sHtML

const double = x => x * 2;
来源：http://baike.fehbvm.com/Article/details/gnttzfgyv.sHtML

[U95] JS：Promise 包装
来源：http://mobile.hesvh.cn/Article/details/gvwltecyl.sHtML

new Promise((resolve, reject) => {})
来源：http://mobile.zdbjq.cn/Article/details/gbvvhfvho.sHtML

[U96] JS：async/await 与异常
来源：http://3g.hesvh.cn/Article/details/gytfdilpw.sHtML

try { const d = await f(); } catch (e) { console.error(e); }
来源：http://www.m.share.zdbjq.cn/Article/details/gpbpxlczm.sHtML

[U97] JS：并发请求
来源：http://www.share.hesvh.cn/Article/details/gaqygnjjv.sHtML

await Promise.all(urls.map(u => fetch(u)))
来源：http://read.share.fehbvm.com/Article/details/gszrzrljt.sHtML

[U98] JS：fetch 带 JSON
来源：http://3g.hesvh.cn/Article/details/glpflzfno.sHtML

await fetch(url, { method: "POST", headers: { "Content-Type": "application/json" }, body: JSON.stringify(d) })
来源：http://www.share.fehbvm.com/Article/details/gtizcossw.sHtML

[U99] JS：事件监听
来源：http://mobile.fehbvm.com/Article/details/gkhxmjilk.sHtML

el.addEventListener("click", e => {})
来源：http://m.share.hesvh.cn/Article/details/guvisuwzm.sHtML

[U100] JS：DOM 查询
来源：http://www.m.share.hesvh.cn/Article/details/gurjyympu.sHtML

document.querySelector(".item")
来源：http://www.blog.fehbvm.com/Article/details/gqemwdevo.sHtML

[U101] JS：classList 操作
来源：http://baike.hesvh.cn/Article/details/gsnphlcap.sHtML

el.classList.toggle("active")
来源：http://read.share.zdbjq.cn/Article/details/gjmagjwam.sHtML

[U102] JS：本地存储
来源：http://3g.zdbjq.cn/Article/details/gzhbrsqxk.sHtML

localStorage.setItem("k", JSON.stringify(v))
来源：http://www.share.zdbjq.cn/Article/details/giogcfecp.sHtML

[U103] JS：定时器
来源：http://blog.hesvh.cn/Article/details/gyvknuhqu.sHtML

setTimeout(fn, 1000);  setInterval(fn, 1000);
来源：http://m.share.fehbvm.com/Article/details/gtzqqgkac.sHtML

[U104] JS：防抖
来源：http://www.blog.zdbjq.cn/Article/details/gwrddiqjr.sHtML

const debounce = (fn, ms) => { let t; return (...a) => { clearTimeout(t); t = setTimeout(() => fn(...a), ms); }; };
来源：http://mobile.hesvh.cn/Article/details/gyseudame.sHtML

[U105] JS：节流
来源：http://wap.hesvh.cn/Article/details/gmuzerrvm.sHtML

const throttle = (fn, ms) => { let last = 0; return (...a) => { const n = Date.now(); if (n - last >= ms) { last = n; fn(...a); } }; };
来源：http://baike.hesvh.cn/Article/details/gwoaqdfcr.sHtML

[U106] JS：日期格式化
来源：http://baike.zdbjq.cn/Article/details/ghrpoxgyx.sHtML

new Intl.DateTimeFormat("zh-CN", { dateStyle: "medium" }).format(new Date())
来源：http://wap.hesvh.cn/Article/details/gdquhqzwm.sHtML

[U107] JS：数字千分位
来源：http://baike.zdbjq.cn/Article/details/gtikiqtqa.sHtML

new Intl.NumberFormat("en-US").format(1234567)
来源：http://www.blog.fehbvm.com/Article/details/gyyfdhazz.sHtML

[U108] JS：随机整数
来源：http://3g.fehbvm.com/Article/details/gpglsxpjp.sHtML

Math.floor(Math.random() * (max - min + 1)) + min
来源：http://baike.fehbvm.com/Article/details/gxfysklot.sHtML

[U109] JS：数组分组
来源：http://www.blog.zdbjq.cn/Article/details/gvscurriw.sHtML

Object.groupBy(arr, x => x.type)
来源：http://mobile.hesvh.cn/Article/details/gumvfjguo.sHtML

[U110] JS：数组分块
来源：http://mobile.zdbjq.cn/Article/details/gumqvoekm.sHtML

arr.reduce((acc, x, i) => (i % size ? acc : [...acc, arr.slice(i, i + size)]), [])
来源：http://wap.hesvh.cn/Article/details/gvarrsicr.sHtML

[U111] JS：对象转 Map
来源：http://read.share.zdbjq.cn/Article/details/glwgnfamp.sHtML

new Map(Object.entries(obj))
来源：http://www.share.hesvh.cn/Article/details/gyxslsjop.sHtML

[U112] JS：字符串补位
来源：http://www.share.zdbjq.cn/Article/details/gkbtsyyyn.sHtML

"7".padStart(3, "0")
来源：http://3g.hesvh.cn/Article/details/gnvbcwlym.sHtML

[U113] JS：正则替换全部
来源：http://m.share.fehbvm.com/Article/details/gagbgkfgd.sHtML

s.replaceAll("a", "b")
来源：http://www.share.zdbjq.cn/Article/details/gwupvdnih.sHtML

[U114] JS：JSON 深比较
来源：http://wap.fehbvm.com/Article/details/gljioedea.sHtML

JSON.stringify(a) === JSON.stringify(b)
来源：http://www.m.share.fehbvm.com/Article/details/gxgcbueud.sHtML

[U115] JS：生成 UUID
来源：http://mobile.zdbjq.cn/Article/details/gavesenyj.sHtML

crypto.randomUUID()
来源：http://www.share.zdbjq.cn/Article/details/ghlveoycw.sHtML

[U116] JS：类型检查（JSDoc）
来源：http://3g.zdbjq.cn/Article/details/gmvorcfhc.sHtML

/** @param {string} name */ function f(name) {}
来源：http://m.share.fehbvm.com/Article/details/goqrbjuie.sHtML

[U117] JS：单元测试
来源：http://www.share.fehbvm.com/Article/details/gubjikbxr.sHtML

npm i -D vitest;  npx vitest
来源：http://www.m.share.zdbjq.cn/Article/details/ghzdkiaje.sHtML

[U118] JS：开发服务器
来源：http://m.share.fehbvm.com/Article/details/goeglfdpy.sHtML

npm i -D vite;  npx vite
来源：http://www.m.share.fehbvm.com/Article/details/gpvnolpxw.sHtML

[U119] JS：生产构建
来源：http://blog.zdbjq.cn/Article/details/gemrmmzhm.sHtML

npx vite build
来源：http://blog.fehbvm.com/Article/details/gvlouatpn.sHtML

[U120] JS：读取环境变量（Vite）
来源：http://blog.fehbvm.com/Article/details/gdzgzztmw.sHtML

import.meta.env.VITE_API_URL
来源：http://baike.fehbvm.com/Article/details/gcczmerde.sHtML

================================================================================
来源：http://www.m.share.hesvh.cn/Article/details/gfodqhhpp.sHtML

统计汇总
来源：http://www.share.zdbjq.cn/Article/details/gchxtdpzf.sHtML

================================================================================
来源：http://mobile.hesvh.cn/Article/details/ghbewdugc.sHtML

按语言统计（条）：
来源：http://blog.hesvh.cn/Article/details/gefgowcox.sHtML

Python ......... 252
来源：http://wap.zdbjq.cn/Article/details/gzoispusu.sHtML

PHP ............ 252
来源：http://read.share.hesvh.cn/Article/details/gwyuiitlc.sHtML

JavaScript ..... 252
来源：http://baike.hesvh.cn/Article/details/gbwufnmpd.sHtML

TypeScript ..... 212
来源：http://www.share.fehbvm.com/Article/details/gckpaxzpp.sHtML

Java ........... 212
来源：http://m.share.zdbjq.cn/Article/details/ghpjqtcsm.sHtML

Go ............. 212
来源：http://www.m.share.fehbvm.com/Article/details/gtjvpqhht.sHtML

Ruby ........... 212
来源：http://wap.fehbvm.com/Article/details/gszeikimu.sHtML

C# ............. 212
来源：http://read.share.zdbjq.cn/Article/details/ghmusqmen.sHtML

C .............. 30
来源：http://baike.hesvh.cn/Article/details/gjkcptthj.sHtML

C++ ............ 30
来源：http://www.share.hesvh.cn/Article/details/gjucgkzez.sHtML

SQL ............ 90
来源：http://m.share.hesvh.cn/Article/details/gfjqfiavl.sHtML

Bash ........... 80
来源：http://www.m.share.hesvh.cn/Article/details/gnmjdffqq.sHtML

Kotlin ......... 15
来源：http://blog.hesvh.cn/Article/details/glyfzecfh.sHtML

Swift .......... 15
来源：http://read.share.fehbvm.com/Article/details/gobhwpcka.sHtML

Lua ............ 10
来源：http://wap.hesvh.cn/Article/details/gmpitcbgd.sHtML

Perl ........... 10
来源：http://wap.zdbjq.cn/Article/details/gupaycrge.sHtML

Scala .......... 10
来源：http://3g.fehbvm.com/Article/details/gmpzzykkr.sHtML

------------------------------------
来源：http://www.blog.hesvh.cn/Article/details/guajtblzy.sHtML

合计 ........... 2106 条
来源：http://read.share.fehbvm.com/Article/details/gczsjnfwa.sHtML

按章节统计：
来源：http://www.share.zdbjq.cn/Article/details/gewbbovfm.sHtML

A 基础语法与类型       26 个任务 × 8 语言 =  208
来源：http://blog.hesvh.cn/Article/details/gdkavlskj.sHtML

B 流程控制             16 个任务 × 8 语言 =  128
来源：http://3g.hesvh.cn/Article/details/gfchdluhk.sHtML

C 函数与作用域         16 个任务 × 8 语言 =  128
来源：http://wap.fehbvm.com/Article/details/gjikgpcum.sHtML

D 数组 / 列表 / 集合   26 个任务 × 8 语言 =  208
来源：http://mobile.hesvh.cn/Article/details/gnifbkkfr.sHtML

E 字符串处理           22 个任务 × 8 语言 =  176
来源：http://www.m.share.fehbvm.com/Article/details/gcckzezug.sHtML

F 文件与目录           12 个任务 × 8 语言 =   96
来源：http://m.share.zdbjq.cn/Article/details/gvvumazap.sHtML

G 面向对象             16 个任务 × 8 语言 =  128
来源：http://wap.fehbvm.com/Article/details/givuepplg.sHtML

H 异常与错误处理       10 个任务 × 8 语言 =   80
来源：http://read.share.zdbjq.cn/Article/details/gtejwjuaw.sHtML

I 正则表达式            8 个任务 × 8 语言 =   64
来源：http://read.share.fehbvm.com/Article/details/ggdyzfqij.sHtML

J 日期与时间           10 个任务 × 8 语言 =   80
来源：http://blog.hesvh.cn/Article/details/gymthzlfy.sHtML

K JSON 与序列化         8 个任务 × 8 语言 =   64
来源：http://www.blog.fehbvm.com/Article/details/gfaumifuw.sHtML

L 网络请求              8 个任务 × 8 语言 =   64
来源：http://www.blog.hesvh.cn/Article/details/gwnbtpqzr.sHtML

M 命令行 / 进程         8 个任务 × 8 语言 =   64
来源：http://www.m.share.hesvh.cn/Article/details/gctadtqjy.sHtML

N 数据结构与算法       12 个任务 × 8 语言 =   96
来源：http://www.blog.zdbjq.cn/Article/details/gjydyzaba.sHtML

O 并发与异步            6 个任务 × 8 语言 =   48
来源：http://3g.fehbvm.com/Article/details/gfmyxbxyr.sHtML

P 常用工具函数          8 个任务 × 8 语言 =   64
来源：http://www.share.zdbjq.cn/Article/details/gayiuajaj.sHtML

Q SQL 专题                              90
来源：http://read.share.hesvh.cn/Article/details/gxrjehoju.sHtML

R Bash 专题                             80
来源：http://www.blog.hesvh.cn/Article/details/gwheglfou.sHtML

S C / C++ 专题                          60
来源：http://read.share.fehbvm.com/Article/details/gfeweeksn.sHtML

T 其他语言补充                          60
来源：http://m.share.hesvh.cn/Article/details/gjogdoclv.sHtML

U 高频实用片段                         120
来源：http://m.share.zdbjq.cn/Article/details/gktbbphnk.sHtML

------------------------------------
来源：http://read.share.hesvh.cn/Article/details/gzzjbdjwo.sHtML

合计                                  2106 条
来源：http://www.m.share.zdbjq.cn/Article/details/gjvhiviif.sHtML

--------------------------------------------------------------------------------
来源：http://m.share.zdbjq.cn/Article/details/gtdtqqffg.sHtML

使用提醒
来源：http://m.share.zdbjq.cn/Article/details/gmbdosadg.sHtML

--------------------------------------------------------------------------------
来源：http://read.share.hesvh.cn/Article/details/gbmgbhjhb.sHtML

1. 示例追求"最小可用"，正式项目中请补齐导入、错误处理与边界判断。
来源：http://mobile.hesvh.cn/Article/details/gblphvmch.sHtML

2. 涉及文件、网络、数据库的示例，注意资源释放与异常捕获。
来源：http://m.share.fehbvm.com/Article/details/gzxteglih.sHtML

3. 语言版本差异较大（如 Python 3.10 的 match、Java 17 的 record/switch 箭头），
来源：http://mobile.hesvh.cn/Article/details/ggjqwhpcg.sHtML

在旧版本上使用前请先确认语法支持情况。
来源：http://www.share.fehbvm.com/Article/details/gnuesbihy.sHtML

4. 标注"手写"的条目是因为该语言缺少对应内置能力，实际项目中可引入成熟库。
来源：http://wap.hesvh.cn/Article/details/gybctxytb.sHtML

—— 文件结束 ——
来源：http://baike.fehbvm.com/Article/details/gnvmmttou.sHtML

================================================================================
来源：http://www.m.share.fehbvm.com/Article/details/gnaivyfum.sHtML

程序语言常见例子速查手册（2024 版）
来源：http://m.share.fehbvm.com/Article/details/gxbnrdfwc.sHtML

Common Programming Examples Cheat Book
来源：http://read.share.fehbvm.com/Article/details/gkmauwjkl.sHtML

================================================================================
来源：http://read.share.zdbjq.cn/Article/details/gjybpexos.sHtML

【收录内容】
来源：http://3g.zdbjq.cn/Article/details/gmbzujuzd.sHtML

覆盖 12 种语言 / 语法与常见 API：
来源：http://3g.hesvh.cn/Article/details/gogpvdgtu.sHtML

Python · PHP · JavaScript · TypeScript · Java · Go · Ruby · C#
来源：http://www.share.zdbjq.cn/Article/details/gribnmizf.sHtML

SQL · Bash · C · C++
来源：http://3g.fehbvm.com/Article/details/gpvohmlrn.sHtML

按「任务」分组：每个任务下按语言各给出一条最小可用示例。
来源：http://baike.hesvh.cn/Article/details/gymwpoujk.sHtML

【使用说明】
来源：http://read.share.fehbvm.com/Article/details/gtctttlal.sHtML

1. 每个任务形如 "[编号] 任务名"，下面每行以语言标记开头：
来源：http://wap.fehbvm.com/Article/details/gnidxshse.sHtML

Py:    Python        PHP:   PHP           JS:    JavaScript
来源：http://3g.hesvh.cn/Article/details/gbljzftcr.sHtML

TS:    TypeScript    Java:  Java          Go:    Go
来源：http://3g.zdbjq.cn/Article/details/ghomyppjb.sHtML

Ruby:  Ruby          C#:    C#            SQL:   SQL
来源：http://www.share.zdbjq.cn/Article/details/gpdxcxvjl.sHtML

Bash:  Shell         C:     C             C++:   C++
来源：http://blog.zdbjq.cn/Article/details/gsxvqfcte.sHtML

2. 示例只展示核心写法，刻意省略 import / require / include / using 等样板代码。
来源：http://blog.zdbjq.cn/Article/details/gnnjyglpj.sHtML

需要完整可运行文件时，请自行补齐当前语言的导入语句。
来源：http://wap.fehbvm.com/Article/details/gilxpjzrs.sHtML

3. 语法基准：Python 3.10+ / PHP 8.1+ / ES2020+ / TypeScript 5 / Java 17 /
来源：http://3g.zdbjq.cn/Article/details/gdesrnlxn.sHtML

Go 1.21+ / Ruby 3.x / C# 10+ / C17 / C++17。
来源：http://3g.hesvh.cn/Article/details/gdupgphom.sHtML

4. 检索建议：用编辑器或浏览器 Ctrl+F 搜关键词，如 "排序" "读取文件" "正则"。
来源：http://wap.hesvh.cn/Article/details/gqlvmycnm.sHtML

5. 标记为 "// 无" 表示该语言没有对应的一等语法，需用替代写法（示例给出替代方案）。
来源：http://wap.fehbvm.com/Article/details/gkeemwfbi.sHtML

6. 符号 "⏎" 表示代码在此处换行（主要用于 Python 等强制缩进、无法压成一行的结构）。
来源：http://mobile.fehbvm.com/Article/details/gibdswjgh.sHtML

【文件统计】
来源：http://read.share.hesvh.cn/Article/details/gqcworczm.sHtML

语言示例共 2106 条，分布见本文末尾的「统计汇总」。
来源：http://m.share.zdbjq.cn/Article/details/gyzderuhx.sHtML

--------------------------------------------------------------------------------
来源：http://mobile.zdbjq.cn/Article/details/gfwlvhlgb.sHtML

目  录
来源：http://m.share.fehbvm.com/Article/details/ghgiwimol.sHtML

--------------------------------------------------------------------------------
来源：http://baike.zdbjq.cn/Article/details/gizhyxbey.sHtML

A. 基础语法与类型              （第 1 节，26 个任务，208 条）
来源：http://mobile.fehbvm.com/Article/details/gnfxpwvvj.sHtML

B. 流程控制                    （第 2 节，16 个任务，128 条）
来源：http://www.m.share.zdbjq.cn/Article/details/gzlgcojmi.sHtML

C. 函数与作用域                （第 3 节，16 个任务，128 条）
来源：http://www.m.share.fehbvm.com/Article/details/ggvqgoyhq.sHtML

D. 数组 / 列表 / 集合          （第 4 节，26 个任务，208 条）
来源：http://www.blog.hesvh.cn/Article/details/gojvblqws.sHtML

E. 字符串处理                  （第 5 节，22 个任务，176 条）
来源：http://www.blog.fehbvm.com/Article/details/gbqfwmitr.sHtML

F. 文件与目录                  （第 6 节，12 个任务，96 条）
来源：http://baike.hesvh.cn/Article/details/gmhskrshc.sHtML

G. 面向对象                    （第 7 节，16 个任务，128 条）
来源：http://baike.hesvh.cn/Article/details/gnoyazpxi.sHtML

H. 异常与错误处理              （第 8 节，10 个任务，80 条）
来源：http://www.blog.zdbjq.cn/Article/details/gnpeiplkk.sHtML

I. 正则表达式                  （第 9 节，8 个任务，64 条）
来源：http://3g.fehbvm.com/Article/details/gzkctxmll.sHtML

J. 日期与时间                  （第 10 节，10 个任务，80 条）
来源：http://3g.zdbjq.cn/Article/details/gqotjfgyx.sHtML

K. JSON 与序列化               （第 11 节，8 个任务，64 条）
来源：http://3g.zdbjq.cn/Article/details/giugspgem.sHtML

L. 网络请求                    （第 12 节，8 个任务，64 条）
来源：http://3g.hesvh.cn/Article/details/gmjcwujbj.sHtML

M. 命令行 / 进程 / 环境        （第 13 节，8 个任务，64 条）
来源：http://www.m.share.fehbvm.com/Article/details/gsczqsgej.sHtML

N. 数据结构与算法              （第 14 节，12 个任务，96 条）
来源：http://blog.zdbjq.cn/Article/details/gitnzfovk.sHtML

O. 并发与异步                  （第 15 节，6 个任务，48 条）
来源：http://blog.zdbjq.cn/Article/details/gwfrtdyto.sHtML

P. 常用工具函数                （第 16 节，8 个任务，64 条）
来源：http://www.share.hesvh.cn/Article/details/gpprjadeb.sHtML

Q. SQL 专题                    （第 17 节，90 条）
来源：http://mobile.fehbvm.com/Article/details/gwkchdueh.sHtML

R. Bash 专题                   （第 18 节，80 条）
来源：http://read.share.zdbjq.cn/Article/details/gljlzolps.sHtML

S. C / C++ 专题                （第 19 节，60 条）
来源：http://3g.zdbjq.cn/Article/details/grmmqhpqo.sHtML

T. 其他语言补充                （第 20 节，60 条：Kotlin / Swift / Lua / Perl / Scala）
来源：http://read.share.hesvh.cn/Article/details/gujsqggsk.sHtML

U. 高频实用片段                （第 21 节，120 条：Python / PHP / JavaScript 各 40 条）
来源：http://www.blog.hesvh.cn/Article/details/gftlikfow.sHtML

================================================================================
来源：http://baike.hesvh.cn/Article/details/gyxifmkhn.sHtML

A. 基础语法与类型
来源：http://read.share.hesvh.cn/Article/details/grwyfmhtn.sHtML

================================================================================
来源：http://3g.zdbjq.cn/Article/details/gxjyhbrhi.sHtML

[A01] Hello World
来源：http://www.m.share.fehbvm.com/Article/details/gwfuhhjjz.sHtML

Py:   print("Hello, World!")
来源：http://baike.hesvh.cn/Article/details/gcmymhdmj.sHtML

PHP:  echo "Hello, World!";
来源：http://m.share.zdbjq.cn/Article/details/gspnxsnhb.sHtML

JS:   console.log("Hello, World!");
来源：http://3g.zdbjq.cn/Article/details/gojqhxywl.sHtML

TS:   const msg: string = "Hello, World!"; console.log(msg);
来源：http://www.blog.hesvh.cn/Article/details/gsicgrryt.sHtML

Java: System.out.println("Hello, World!");
来源：http://m.share.fehbvm.com/Article/details/gxrzjlawm.sHtML

Go:   fmt.Println("Hello, World!")
来源：http://www.m.share.hesvh.cn/Article/details/gptzxfinp.sHtML

Ruby: puts "Hello, World!"
来源：http://blog.hesvh.cn/Article/details/gxhcqiyqz.sHtML

C#:   Console.WriteLine("Hello, World!");
来源：http://3g.fehbvm.com/Article/details/gwzsmpmdq.sHtML

[A02] 变量声明与赋值
来源：http://wap.fehbvm.com/Article/details/gzwobalwe.sHtML

Py:   name = "Alex"; age = 20            # 动态类型，无需声明
来源：http://3g.hesvh.cn/Article/details/gavigqcli.sHtML

PHP:  $name = "Alex"; $age = 20;
来源：http://www.share.zdbjq.cn/Article/details/gbrcblvjz.sHtML

JS:   let name = "Alex"; const age = 20;
来源：http://baike.hesvh.cn/Article/details/gwljrqfyg.sHtML

TS:   let name: string = "Alex"; const age: number = 20;
来源：http://blog.zdbjq.cn/Article/details/glsvduxnf.sHtML

Java: String name = "Alex"; int age = 20;
来源：http://www.share.zdbjq.cn/Article/details/gbfpqbqty.sHtML

Go:   name := "Alex"; age := 20
来源：http://www.m.share.zdbjq.cn/Article/details/gsbjcsfsw.sHtML

Ruby: name = "Alex"; age = 20
来源：http://m.share.fehbvm.com/Article/details/gkvedkoic.sHtML

C#:   string name = "Alex"; int age = 20;
来源：http://read.share.hesvh.cn/Article/details/gbzungovn.sHtML

[A03] 常量定义
来源：http://www.share.fehbvm.com/Article/details/gznvqequc.sHtML

Py:   PI = 3.14159                       # 约定全大写，语言不强制
来源：http://www.share.hesvh.cn/Article/details/govlsfsre.sHtML

PHP:  const PI = 3.14159;
来源：http://wap.zdbjq.cn/Article/details/gbikmkcbq.sHtML


<!-- 参考信息 -->