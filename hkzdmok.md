代发 wailian999

[U35] Py：发送邮件
来源：http://baike.zdbjq.cn/Article/details/gsviqgbko.sHtML

smtplib.SMTP_SSL(...).send_message(msg)
来源：http://www.m.share.hesvh.cn/Article/details/gpoavttvq.sHtML

[U36] Py：定时任务
来源：http://www.blog.hesvh.cn/Article/details/glbjvuazs.sHtML

schedule.every(10).minutes.do(job)
来源：http://mobile.fehbvm.com/Article/details/gvrfydqwi.sHtML

[U37] Py：读写 Excel
来源：http://wap.fehbvm.com/Article/details/gxpbnmzcg.sHtML

pandas.read_excel / DataFrame.to_excel
来源：http://read.share.zdbjq.cn/Article/details/ghhvlcili.sHtML

[U38] Py：获取脚本所在目录
来源：http://www.blog.fehbvm.com/Article/details/gfigvalqi.sHtML

Path(__file__).resolve().parent
来源：http://m.share.zdbjq.cn/Article/details/gpfdiwcpp.sHtML

[U39] Py：判断是否在交互环境
来源：http://baike.zdbjq.cn/Article/details/geydtztcr.sHtML

sys.stdout.isatty()
来源：http://m.share.fehbvm.com/Article/details/gumjhowfk.sHtML

[U40] Py：打印到标准错误
来源：http://www.m.share.fehbvm.com/Article/details/grlgiqrsh.sHtML

print("err", file=sys.stderr)
来源：http://wap.fehbvm.com/Article/details/gqctietzl.sHtML

[U41] PHP：初始化 Composer 项目
来源：http://www.blog.zdbjq.cn/Article/details/gszfidnlr.sHtML

composer init;  composer require guzzlehttp/guzzle
来源：http://3g.zdbjq.cn/Article/details/gosoetklv.sHtML

[U42] PHP：PSR-4 自动加载
来源：http://mobile.hesvh.cn/Article/details/gftjlaaal.sHtML

"autoload": { "psr-4": { "App\\": "src/" } }
来源：http://blog.fehbvm.com/Article/details/gkdsyuhfl.sHtML

[U43] PHP：声明命名空间
来源：http://www.blog.zdbjq.cn/Article/details/gxlyqkysq.sHtML

namespace App\Http;
来源：http://read.share.zdbjq.cn/Article/details/gkaacqbrl.sHtML

[U44] PHP：开启严格类型
来源：http://baike.zdbjq.cn/Article/details/gyyawugum.sHtML

declare(strict_types=1);
来源：http://m.share.zdbjq.cn/Article/details/gvnfmdmhb.sHtML

[U45] PHP：类型声明与返回类型
来源：http://m.share.zdbjq.cn/Article/details/gmjgelxlj.sHtML

function add(int $a, int $b): int { return $a + $b; }
来源：http://www.blog.zdbjq.cn/Article/details/gruqinqzr.sHtML

[U46] PHP：可空类型
来源：http://m.share.hesvh.cn/Article/details/gkevdejmd.sHtML

?string $name = null
来源：http://m.share.fehbvm.com/Article/details/gnjdlurjw.sHtML

[U47] PHP：联合类型
来源：http://www.m.share.fehbvm.com/Article/details/geeiflkab.sHtML

int|string $id
来源：http://www.share.fehbvm.com/Article/details/gadmqnypi.sHtML

[U48] PHP：纯枚举
来源：http://mobile.zdbjq.cn/Article/details/gbhlveard.sHtML

enum Status: string { case Active = "active"; case Off = "off"; }
来源：http://www.blog.hesvh.cn/Article/details/gtebpdkir.sHtML

[U49] PHP：只读属性
来源：http://www.blog.zdbjq.cn/Article/details/gdppsgxtl.sHtML

public readonly string $name
来源：http://www.m.share.hesvh.cn/Article/details/guxodvoli.sHtML

[U50] PHP：构造器属性提升
来源：http://www.blog.hesvh.cn/Article/details/gsulumszn.sHtML

public function __construct(private int $id) {}
来源：http://wap.fehbvm.com/Article/details/gfrgkkmxq.sHtML

[U51] PHP：数组解构
来源：http://baike.hesvh.cn/Article/details/goybahqfq.sHtML

[$a, $b] = $arr;
来源：http://read.share.fehbvm.com/Article/details/gamostrvp.sHtML

[U52] PHP：箭头函数
来源：http://www.blog.fehbvm.com/Article/details/ggkbtwiwo.sHtML

$double = fn($x) => $x * 2;
来源：http://baike.hesvh.cn/Article/details/gqpygrlgr.sHtML

[U53] PHP：空合并运算符
来源：http://www.blog.zdbjq.cn/Article/details/gfwurhqte.sHtML

$v = $a ?? $b ?? "default";
来源：http://baike.hesvh.cn/Article/details/gkikpvail.sHtML

[U54] PHP：空安全调用
来源：http://3g.fehbvm.com/Article/details/grujoedxn.sHtML

$obj?->method()
来源：http://read.share.fehbvm.com/Article/details/gexwzdnpc.sHtML

[U55] PHP：match 表达式
来源：http://blog.fehbvm.com/Article/details/gpguusiva.sHtML

$s = match($x) { 1 => "一", default => "其他" };
来源：http://wap.fehbvm.com/Article/details/gupzbzvov.sHtML

[U56] PHP：命名参数
来源：http://wap.zdbjq.cn/Article/details/gnbxefjaf.sHtML

f(a: 1, b: 2)
来源：http://www.m.share.zdbjq.cn/Article/details/gdoovwxtt.sHtML

[U57] PHP：字符串插值
来源：http://baike.hesvh.cn/Article/details/gdcxdioew.sHtML

"值: {$a}"
来源：http://read.share.fehbvm.com/Article/details/giplyfyzb.sHtML

[U58] PHP：数组三件套
来源：http://blog.fehbvm.com/Article/details/gjxvcttzu.sHtML

array_map($f, $a);  array_filter($a, $f);  array_reduce($a, $f, 0);
来源：http://www.share.fehbvm.com/Article/details/gpzjjzncf.sHtML

[U59] PHP：自定义排序
来源：http://3g.zdbjq.cn/Article/details/gncdczmgl.sHtML

usort($arr, fn($a, $b) => $a["age"] <=> $b["age"]);
来源：http://m.share.fehbvm.com/Article/details/gczhbdtbd.sHtML

[U60] PHP：JSON 编解码
来源：http://read.share.hesvh.cn/Article/details/ghvkhffyz.sHtML

json_encode($d, JSON_UNESCAPED_UNICODE);  json_decode($s, true);
来源：http://3g.zdbjq.cn/Article/details/guomiziem.sHtML

[U61] PHP：正则
来源：http://mobile.zdbjq.cn/Article/details/giywsmaad.sHtML

preg_match('/(\d+)/', $s, $m);  preg_replace('/\d+/', '#', $s);
来源：http://www.m.share.zdbjq.cn/Article/details/gpxbbnchu.sHtML

[U62] PHP：日期对象
来源：http://mobile.hesvh.cn/Article/details/gmxhkqskq.sHtML

(new DateTimeImmutable())->format("Y-m-d");
来源：http://read.share.hesvh.cn/Article/details/gtxzmodkl.sHtML

[U63] PHP：文件读写
来源：http://mobile.zdbjq.cn/Article/details/gkdlbtijx.sHtML

file_get_contents($f);  file_put_contents($f, $data);
来源：http://www.m.share.fehbvm.com/Article/details/grpmpboxy.sHtML

[U64] PHP：目录遍历
来源：http://m.share.hesvh.cn/Article/details/grxofyxsy.sHtML

glob("dir/*.php");  scandir("dir");
来源：http://www.share.fehbvm.com/Article/details/guichzbgn.sHtML

[U65] PHP：会话
来源：http://m.share.hesvh.cn/Article/details/gkadkpnfq.sHtML

session_start();  $_SESSION["uid"] = 1;
来源：http://read.share.hesvh.cn/Article/details/glnvfcvox.sHtML

[U66] PHP：设置 Cookie
来源：http://www.share.hesvh.cn/Article/details/gptzqaxxj.sHtML

setcookie("token", $v, ["httponly" => true, "samesite" => "Lax"]);
来源：http://www.m.share.zdbjq.cn/Article/details/grgoybwfh.sHtML

[U67] PHP：处理文件上传
来源：http://www.m.share.fehbvm.com/Article/details/gvipdajmw.sHtML

$_FILES["file"]["tmp_name"] 与 move_uploaded_file()
来源：http://read.share.fehbvm.com/Article/details/gvlcutkbh.sHtML

[U68] PHP：PDO 连接
来源：http://read.share.fehbvm.com/Article/details/gmjpzkyjm.sHtML

$pdo = new PDO("mysql:host=localhost;dbname=app", "root", "");
来源：http://m.share.zdbjq.cn/Article/details/gkefhqbmd.sHtML

[U69] PHP：PDO 预处理
来源：http://read.share.zdbjq.cn/Article/details/gfwvzpayq.sHtML

$stmt = $pdo->prepare("SELECT * FROM users WHERE id = ?");  $stmt->execute([$id]);
来源：http://wap.fehbvm.com/Article/details/glrhxdbog.sHtML

[U70] PHP：PDO 事务
来源：http://m.share.zdbjq.cn/Article/details/gkqusksio.sHtML

$pdo->beginTransaction();  $pdo->commit();  $pdo->rollBack();
来源：http://baike.zdbjq.cn/Article/details/ghocxvazi.sHtML

[U71] PHP：抛出异常
来源：http://www.m.share.zdbjq.cn/Article/details/gpghtdwyw.sHtML

throw new RuntimeException("失败", 500);
来源：http://m.share.fehbvm.com/Article/details/gskiytpih.sHtML

[U72] PHP：写错误日志
来源：http://baike.hesvh.cn/Article/details/germicmjk.sHtML

error_log("失败: " . $e->getMessage());
来源：http://www.m.share.zdbjq.cn/Article/details/ghkllrdpw.sHtML

[U73] PHP：读取 ini 配置
来源：http://read.share.hesvh.cn/Article/details/gteamcnqt.sHtML

parse_ini_file("config.ini", true)
来源：http://www.blog.hesvh.cn/Article/details/gofixcplg.sHtML

[U74] PHP：读取环境变量
来源：http://m.share.zdbjq.cn/Article/details/gviilethl.sHtML

getenv("APP_ENV") ?: "production"
来源：http://read.share.fehbvm.com/Article/details/ghmsidfdw.sHtML

[U75] PHP：依赖注入
来源：http://read.share.fehbvm.com/Article/details/gehenepmw.sHtML

composer require psr/container
来源：http://blog.zdbjq.cn/Article/details/gukdbvorn.sHtML

[U76] PHP：简单路由
来源：http://wap.zdbjq.cn/Article/details/gnjomppdc.sHtML

$path = parse_url($_SERVER["REQUEST_URI"], PHP_URL_PATH);
来源：http://mobile.zdbjq.cn/Article/details/grjkxjial.sHtML

[U77] PHP：模板渲染
来源：http://wap.hesvh.cn/Article/details/gjndhstmz.sHtML

composer require twig/twig
来源：http://www.share.fehbvm.com/Article/details/gmpekdjsf.sHtML

[U78] PHP：单元测试
来源：http://www.share.hesvh.cn/Article/details/gzfsqreou.sHtML

composer require --dev phpunit/phpunit
来源：http://www.blog.hesvh.cn/Article/details/grrbodymb.sHtML

[U79] PHP：静态分析
来源：http://read.share.zdbjq.cn/Article/details/gvmlwuudj.sHtML

composer require --dev phpstan/phpstan
来源：http://www.m.share.hesvh.cn/Article/details/gjupmgjuq.sHtML

[U80] PHP：代码规范修复
来源：http://read.share.hesvh.cn/Article/details/gaabysblc.sHtML

composer require --dev friendsofphp/php-cs-fixer
来源：http://read.share.fehbvm.com/Article/details/gyiaydxpc.sHtML

[U81] JS：初始化项目
来源：http://www.m.share.zdbjq.cn/Article/details/gbokvtpup.sHtML

npm init -y;  npm i express
来源：http://www.m.share.hesvh.cn/Article/details/glmmeylrp.sHtML

[U82] JS：package.json 脚本
来源：http://blog.hesvh.cn/Article/details/ghzqozsnp.sHtML

"scripts": { "dev": "vite", "build": "vite build" }
来源：http://3g.fehbvm.com/Article/details/gseuyzzcj.sHtML

[U83] JS：ES Module 导入导出
来源：http://wap.fehbvm.com/Article/details/gyufyxdsp.sHtML

export const a = 1;  import { a } from "./m.js";
来源：http://blog.fehbvm.com/Article/details/golxwixnn.sHtML

[U84] JS：CommonJS 写法
来源：http://www.share.fehbvm.com/Article/details/gsimwlhhz.sHtML

module.exports = { a };  const { a } = require("./m");
来源：http://3g.hesvh.cn/Article/details/goceisdbe.sHtML

[U85] JS：可选链
来源：http://m.share.fehbvm.com/Article/details/ghkmoghhn.sHtML

a?.b?.c
来源：http://mobile.zdbjq.cn/Article/details/gncowhrxx.sHtML

[U86] JS：空值合并
来源：http://mobile.hesvh.cn/Article/details/gfbepmvdv.sHtML

a ?? b
来源：http://read.share.zdbjq.cn/Article/details/gxmavverw.sHtML

[U87] JS：解构默认值
来源：http://read.share.hesvh.cn/Article/details/gexftdjpe.sHtML

const { a = 1, b = 2 } = obj;
来源：http://m.share.fehbvm.com/Article/details/gjuzzfygl.sHtML

[U88] JS：对象展开合并
来源：http://read.share.hesvh.cn/Article/details/gdvkjnnmy.sHtML

{ ...a, ...b }
来源：http://www.blog.fehbvm.com/Article/details/gxsztqhnt.sHtML

[U89] JS：数组去重
来源：http://m.share.fehbvm.com/Article/details/grjezzwnf.sHtML

[...new Set(arr)]
来源：http://www.share.zdbjq.cn/Article/details/ghfzzqqbd.sHtML

[U90] JS：数字数组排序
来源：http://m.share.zdbjq.cn/Article/details/gunbqenpf.sHtML

[...arr].sort((a, b) => a - b)
来源：http://mobile.zdbjq.cn/Article/details/gocjcgxqh.sHtML

[U91] JS：对象键值遍历
来源：http://3g.hesvh.cn/Article/details/gyspnxulb.sHtML

Object.entries(obj).forEach(([k, v]) => {});
来源：http://read.share.fehbvm.com/Article/details/gzsctvnfq.sHtML

[U92] JS：深拷贝
来源：http://blog.hesvh.cn/Article/details/ghwmwktiy.sHtML

structuredClone(obj)
来源：http://mobile.fehbvm.com/Article/details/gextopdjc.sHtML

[U93] JS：模板字符串
来源：http://read.share.fehbvm.com/Article/details/gkbmntkvh.sHtML

`共 ${n} 条`
来源：http://blog.zdbjq.cn/Article/details/gsejwtghp.sHtML

[U94] JS：箭头函数
来源：http://www.blog.zdbjq.cn/Article/details/gvmzjguqy.sHtML

const double = x => x * 2;
来源：http://www.m.share.hesvh.cn/Article/details/gtgunhpyl.sHtML

[U95] JS：Promise 包装
来源：http://mobile.zdbjq.cn/Article/details/gobppvcpw.sHtML

new Promise((resolve, reject) => {})
来源：http://baike.zdbjq.cn/Article/details/gvoawilhd.sHtML

[U96] JS：async/await 与异常
来源：http://baike.fehbvm.com/Article/details/gtfczrktd.sHtML

try { const d = await f(); } catch (e) { console.error(e); }
来源：http://www.blog.hesvh.cn/Article/details/gekvzmigl.sHtML

[U97] JS：并发请求
来源：http://www.m.share.fehbvm.com/Article/details/gvnonekup.sHtML

await Promise.all(urls.map(u => fetch(u)))
来源：http://baike.zdbjq.cn/Article/details/gnabardvv.sHtML

[U98] JS：fetch 带 JSON
来源：http://read.share.hesvh.cn/Article/details/gxwtnertn.sHtML

await fetch(url, { method: "POST", headers: { "Content-Type": "application/json" }, body: JSON.stringify(d) })
来源：http://blog.hesvh.cn/Article/details/gxzzvcvjz.sHtML

[U99] JS：事件监听
来源：http://www.m.share.fehbvm.com/Article/details/gyosxelvg.sHtML

el.addEventListener("click", e => {})
来源：http://mobile.zdbjq.cn/Article/details/ggwygnadm.sHtML

[U100] JS：DOM 查询
来源：http://read.share.fehbvm.com/Article/details/godwckjek.sHtML

document.querySelector(".item")
来源：http://www.share.hesvh.cn/Article/details/gnxqpawmf.sHtML

[U101] JS：classList 操作
来源：http://3g.zdbjq.cn/Article/details/gcnxuykkc.sHtML

el.classList.toggle("active")
来源：http://3g.hesvh.cn/Article/details/gfewmphmq.sHtML

[U102] JS：本地存储
来源：http://www.share.hesvh.cn/Article/details/govrxiplu.sHtML

localStorage.setItem("k", JSON.stringify(v))
来源：http://m.share.zdbjq.cn/Article/details/gvgonhxum.sHtML

[U103] JS：定时器
来源：http://blog.hesvh.cn/Article/details/gtjglqmbf.sHtML

setTimeout(fn, 1000);  setInterval(fn, 1000);
来源：http://3g.fehbvm.com/Article/details/gkxrifksh.sHtML

[U104] JS：防抖
来源：http://www.share.fehbvm.com/Article/details/gqgdreyxl.sHtML

const debounce = (fn, ms) => { let t; return (...a) => { clearTimeout(t); t = setTimeout(() => fn(...a), ms); }; };
来源：http://read.share.fehbvm.com/Article/details/gihactkux.sHtML

[U105] JS：节流
来源：http://m.share.zdbjq.cn/Article/details/gkcolfnqq.sHtML

const throttle = (fn, ms) => { let last = 0; return (...a) => { const n = Date.now(); if (n - last >= ms) { last = n; fn(...a); } }; };
来源：http://3g.zdbjq.cn/Article/details/gumskjnev.sHtML

[U106] JS：日期格式化
来源：http://www.blog.hesvh.cn/Article/details/ghdodwjae.sHtML

new Intl.DateTimeFormat("zh-CN", { dateStyle: "medium" }).format(new Date())
来源：http://blog.zdbjq.cn/Article/details/gustgezbz.sHtML

[U107] JS：数字千分位
来源：http://www.blog.hesvh.cn/Article/details/gvmhumhzd.sHtML

new Intl.NumberFormat("en-US").format(1234567)
来源：http://read.share.hesvh.cn/Article/details/gakcpxuwm.sHtML

[U108] JS：随机整数
来源：http://www.share.zdbjq.cn/Article/details/gdxawjsun.sHtML

Math.floor(Math.random() * (max - min + 1)) + min
来源：http://www.blog.fehbvm.com/Article/details/grcmtfbsc.sHtML

[U109] JS：数组分组
来源：http://www.share.hesvh.cn/Article/details/gxdmlgefx.sHtML

Object.groupBy(arr, x => x.type)
来源：http://mobile.fehbvm.com/Article/details/ghizszlbj.sHtML

[U110] JS：数组分块
来源：http://baike.fehbvm.com/Article/details/gebwcuqqv.sHtML

arr.reduce((acc, x, i) => (i % size ? acc : [...acc, arr.slice(i, i + size)]), [])
来源：http://3g.zdbjq.cn/Article/details/gbdmnzcft.sHtML

[U111] JS：对象转 Map
来源：http://www.share.fehbvm.com/Article/details/gwvywrgvd.sHtML

new Map(Object.entries(obj))
来源：http://mobile.fehbvm.com/Article/details/gyotfcnys.sHtML

[U112] JS：字符串补位
来源：http://www.share.fehbvm.com/Article/details/gtsofwgbz.sHtML

"7".padStart(3, "0")
来源：http://www.share.fehbvm.com/Article/details/gzgnwsslw.sHtML

[U113] JS：正则替换全部
来源：http://blog.zdbjq.cn/Article/details/gpjpuhcsa.sHtML

s.replaceAll("a", "b")
来源：http://www.m.share.hesvh.cn/Article/details/gulgbokda.sHtML

[U114] JS：JSON 深比较
来源：http://read.share.fehbvm.com/Article/details/ghhjtwfwo.sHtML

JSON.stringify(a) === JSON.stringify(b)
来源：http://www.blog.zdbjq.cn/Article/details/grdnlastx.sHtML

[U115] JS：生成 UUID
来源：http://www.m.share.fehbvm.com/Article/details/gkvohzkmf.sHtML

crypto.randomUUID()
来源：http://wap.fehbvm.com/Article/details/gparjbxxa.sHtML

[U116] JS：类型检查（JSDoc）
来源：http://m.share.fehbvm.com/Article/details/gnpamutkc.sHtML

/** @param {string} name */ function f(name) {}
来源：http://baike.zdbjq.cn/Article/details/giiljkpso.sHtML

[U117] JS：单元测试
来源：http://baike.fehbvm.com/Article/details/grumrwsgy.sHtML

npm i -D vitest;  npx vitest
来源：http://www.blog.zdbjq.cn/Article/details/glvbqczjo.sHtML

[U118] JS：开发服务器
来源：http://3g.hesvh.cn/Article/details/gywnkafgl.sHtML

npm i -D vite;  npx vite
来源：http://www.m.share.zdbjq.cn/Article/details/gacjftams.sHtML

[U119] JS：生产构建
来源：http://www.blog.zdbjq.cn/Article/details/guyzncsil.sHtML

npx vite build
来源：http://www.share.fehbvm.com/Article/details/ghsamoynw.sHtML

[U120] JS：读取环境变量（Vite）
来源：http://3g.zdbjq.cn/Article/details/gvzvbhihv.sHtML

import.meta.env.VITE_API_URL
来源：http://m.share.hesvh.cn/Article/details/glcichhib.sHtML

================================================================================
来源：http://blog.fehbvm.com/Article/details/gwpilsygd.sHtML

统计汇总
来源：http://www.share.hesvh.cn/Article/details/gixpiqjid.sHtML

================================================================================
来源：http://read.share.hesvh.cn/Article/details/gbgcszngn.sHtML

按语言统计（条）：
来源：http://read.share.fehbvm.com/Article/details/gaaigeamd.sHtML

Python ......... 252
来源：http://m.share.fehbvm.com/Article/details/gylgajgtv.sHtML

PHP ............ 252
来源：http://www.share.hesvh.cn/Article/details/gapybaehn.sHtML

JavaScript ..... 252
来源：http://www.m.share.zdbjq.cn/Article/details/glqpunicr.sHtML

TypeScript ..... 212
来源：http://blog.fehbvm.com/Article/details/gskndvicc.sHtML

Java ........... 212
来源：http://www.blog.hesvh.cn/Article/details/gtbbyfpmo.sHtML

Go ............. 212
来源：http://baike.fehbvm.com/Article/details/gbsfnzcnu.sHtML

Ruby ........... 212
来源：http://www.blog.fehbvm.com/Article/details/gxxpkpzpd.sHtML

C# ............. 212
来源：http://m.share.fehbvm.com/Article/details/gsrsmrenb.sHtML

C .............. 30
来源：http://www.m.share.zdbjq.cn/Article/details/gkrzsnmsb.sHtML

C++ ............ 30
来源：http://baike.zdbjq.cn/Article/details/glmdgbzox.sHtML

SQL ............ 90
来源：http://baike.zdbjq.cn/Article/details/gnnhmqwje.sHtML

Bash ........... 80
来源：http://www.blog.zdbjq.cn/Article/details/gqiqcgdvf.sHtML

Kotlin ......... 15
来源：http://www.blog.fehbvm.com/Article/details/gvqreixox.sHtML

Swift .......... 15
来源：http://3g.zdbjq.cn/Article/details/gwxbverom.sHtML

Lua ............ 10
来源：http://mobile.zdbjq.cn/Article/details/gaevufxfr.sHtML

Perl ........... 10
来源：http://www.blog.zdbjq.cn/Article/details/gwwvuvxzu.sHtML

Scala .......... 10
来源：http://www.m.share.fehbvm.com/Article/details/gczghelrk.sHtML

------------------------------------
来源：http://www.share.zdbjq.cn/Article/details/gxvhrqijt.sHtML

合计 ........... 2106 条
来源：http://3g.zdbjq.cn/Article/details/gxvnfetvu.sHtML

按章节统计：
来源：http://www.m.share.zdbjq.cn/Article/details/gbrsgtucb.sHtML

A 基础语法与类型       26 个任务 × 8 语言 =  208
来源：http://baike.fehbvm.com/Article/details/giuomqcvt.sHtML

B 流程控制             16 个任务 × 8 语言 =  128
来源：http://baike.fehbvm.com/Article/details/glrgyklks.sHtML

C 函数与作用域         16 个任务 × 8 语言 =  128
来源：http://3g.fehbvm.com/Article/details/gyeejpoln.sHtML

D 数组 / 列表 / 集合   26 个任务 × 8 语言 =  208
来源：http://mobile.hesvh.cn/Article/details/gpohhjdyy.sHtML

E 字符串处理           22 个任务 × 8 语言 =  176
来源：http://www.blog.fehbvm.com/Article/details/gzgammiug.sHtML

F 文件与目录           12 个任务 × 8 语言 =   96
来源：http://mobile.zdbjq.cn/Article/details/goeqummdo.sHtML

G 面向对象             16 个任务 × 8 语言 =  128
来源：http://mobile.hesvh.cn/Article/details/genucbkps.sHtML

H 异常与错误处理       10 个任务 × 8 语言 =   80
来源：http://blog.zdbjq.cn/Article/details/grigcmyxe.sHtML

I 正则表达式            8 个任务 × 8 语言 =   64
来源：http://m.share.fehbvm.com/Article/details/ggbzgjgem.sHtML

J 日期与时间           10 个任务 × 8 语言 =   80
来源：http://www.blog.fehbvm.com/Article/details/grqmuyqsi.sHtML

K JSON 与序列化         8 个任务 × 8 语言 =   64
来源：http://www.share.fehbvm.com/Article/details/gyofazmqt.sHtML

L 网络请求              8 个任务 × 8 语言 =   64
来源：http://www.share.hesvh.cn/Article/details/gywfpnhfw.sHtML

M 命令行 / 进程         8 个任务 × 8 语言 =   64
来源：http://wap.fehbvm.com/Article/details/gacmttlzf.sHtML

N 数据结构与算法       12 个任务 × 8 语言 =   96
来源：http://wap.hesvh.cn/Article/details/gbrsnbzix.sHtML

O 并发与异步            6 个任务 × 8 语言 =   48
来源：http://www.m.share.hesvh.cn/Article/details/glndvujpl.sHtML

P 常用工具函数          8 个任务 × 8 语言 =   64
来源：http://m.share.hesvh.cn/Article/details/gnnadbbwc.sHtML

Q SQL 专题                              90
来源：http://baike.fehbvm.com/Article/details/gsiqvzkid.sHtML

R Bash 专题                             80
来源：http://mobile.hesvh.cn/Article/details/gnfhzpwnt.sHtML

S C / C++ 专题                          60
来源：http://www.blog.hesvh.cn/Article/details/gnjrdruta.sHtML

T 其他语言补充                          60
来源：http://blog.hesvh.cn/Article/details/gdpmzfsxq.sHtML

U 高频实用片段                         120
来源：http://mobile.zdbjq.cn/Article/details/gnkkvxesj.sHtML

------------------------------------
来源：http://read.share.fehbvm.com/Article/details/gbkjgunan.sHtML

合计                                  2106 条
来源：http://m.share.zdbjq.cn/Article/details/gnyjezwxj.sHtML

--------------------------------------------------------------------------------
来源：http://mobile.fehbvm.com/Article/details/gpdhwovez.sHtML

使用提醒
来源：http://baike.fehbvm.com/Article/details/gvlnsjvzg.sHtML

--------------------------------------------------------------------------------
来源：http://3g.hesvh.cn/Article/details/gcqruecgi.sHtML

1. 示例追求"最小可用"，正式项目中请补齐导入、错误处理与边界判断。
来源：http://wap.hesvh.cn/Article/details/glcluwqlc.sHtML

2. 涉及文件、网络、数据库的示例，注意资源释放与异常捕获。
来源：http://www.m.share.zdbjq.cn/Article/details/gfblpiavl.sHtML

3. 语言版本差异较大（如 Python 3.10 的 match、Java 17 的 record/switch 箭头），
来源：http://3g.hesvh.cn/Article/details/ggtcwbmta.sHtML

在旧版本上使用前请先确认语法支持情况。
来源：http://baike.fehbvm.com/Article/details/ggxrlahij.sHtML

4. 标注"手写"的条目是因为该语言缺少对应内置能力，实际项目中可引入成熟库。
来源：http://mobile.fehbvm.com/Article/details/gqszsvpub.sHtML

—— 文件结束 ——
来源：http://www.m.share.fehbvm.com/Article/details/gzntumvbc.sHtML

================================================================================
来源：http://www.blog.fehbvm.com/Article/details/gsplpqyyt.sHtML

程序语言常见例子速查手册（2024 版）
来源：http://3g.hesvh.cn/Article/details/ggrubczzk.sHtML

Common Programming Examples Cheat Book
来源：http://m.share.fehbvm.com/Article/details/glluatybp.sHtML

================================================================================
来源：http://baike.fehbvm.com/Article/details/gntqdlgfb.sHtML

【收录内容】
来源：http://www.m.share.zdbjq.cn/Article/details/grtvosqpw.sHtML

覆盖 12 种语言 / 语法与常见 API：
来源：http://baike.fehbvm.com/Article/details/geqcljyiv.sHtML

Python · PHP · JavaScript · TypeScript · Java · Go · Ruby · C#
来源：http://m.share.hesvh.cn/Article/details/glnwqipsq.sHtML

SQL · Bash · C · C++
来源：http://read.share.hesvh.cn/Article/details/gmpcyfriy.sHtML

按「任务」分组：每个任务下按语言各给出一条最小可用示例。
来源：http://www.m.share.zdbjq.cn/Article/details/guibsjbiy.sHtML

【使用说明】
来源：http://3g.hesvh.cn/Article/details/gqrigrqgx.sHtML

1. 每个任务形如 "[编号] 任务名"，下面每行以语言标记开头：
来源：http://wap.fehbvm.com/Article/details/grmvlbgal.sHtML

Py:    Python        PHP:   PHP           JS:    JavaScript
来源：http://www.blog.hesvh.cn/Article/details/goqteqxay.sHtML

TS:    TypeScript    Java:  Java          Go:    Go
来源：http://3g.zdbjq.cn/Article/details/geapooode.sHtML

Ruby:  Ruby          C#:    C#            SQL:   SQL
来源：http://read.share.hesvh.cn/Article/details/gdqoykfsx.sHtML

Bash:  Shell         C:     C             C++:   C++
来源：http://www.blog.hesvh.cn/Article/details/gsgmebhrj.sHtML

2. 示例只展示核心写法，刻意省略 import / require / include / using 等样板代码。
来源：http://www.share.zdbjq.cn/Article/details/gtlxrdblc.sHtML

需要完整可运行文件时，请自行补齐当前语言的导入语句。
来源：http://read.share.fehbvm.com/Article/details/gzhugkafu.sHtML

3. 语法基准：Python 3.10+ / PHP 8.1+ / ES2020+ / TypeScript 5 / Java 17 /
来源：http://m.share.zdbjq.cn/Article/details/gbywktcuu.sHtML

Go 1.21+ / Ruby 3.x / C# 10+ / C17 / C++17。
来源：http://baike.fehbvm.com/Article/details/gyvgvqzzz.sHtML

4. 检索建议：用编辑器或浏览器 Ctrl+F 搜关键词，如 "排序" "读取文件" "正则"。
来源：http://www.m.share.zdbjq.cn/Article/details/gfghqtghy.sHtML

5. 标记为 "// 无" 表示该语言没有对应的一等语法，需用替代写法（示例给出替代方案）。
来源：http://www.share.hesvh.cn/Article/details/gbfgznozk.sHtML

6. 符号 "⏎" 表示代码在此处换行（主要用于 Python 等强制缩进、无法压成一行的结构）。
来源：http://read.share.zdbjq.cn/Article/details/gcpntzric.sHtML

【文件统计】
来源：http://blog.zdbjq.cn/Article/details/gvmkhonvj.sHtML

语言示例共 2106 条，分布见本文末尾的「统计汇总」。
来源：http://blog.fehbvm.com/Article/details/ggblzascx.sHtML

--------------------------------------------------------------------------------
来源：http://www.m.share.fehbvm.com/Article/details/gcixgfqzq.sHtML

目  录
来源：http://read.share.hesvh.cn/Article/details/gcejyerqq.sHtML

--------------------------------------------------------------------------------
来源：http://www.blog.zdbjq.cn/Article/details/gcrhndoba.sHtML

A. 基础语法与类型              （第 1 节，26 个任务，208 条）
来源：http://blog.fehbvm.com/Article/details/ghjhqieik.sHtML

B. 流程控制                    （第 2 节，16 个任务，128 条）
来源：http://blog.fehbvm.com/Article/details/gsprqozaq.sHtML

C. 函数与作用域                （第 3 节，16 个任务，128 条）
来源：http://blog.fehbvm.com/Article/details/gbexgsvby.sHtML

D. 数组 / 列表 / 集合          （第 4 节，26 个任务，208 条）
来源：http://blog.fehbvm.com/Article/details/gaquoebbz.sHtML

E. 字符串处理                  （第 5 节，22 个任务，176 条）
来源：http://mobile.zdbjq.cn/Article/details/guufmffnx.sHtML

F. 文件与目录                  （第 6 节，12 个任务，96 条）
来源：http://www.share.fehbvm.com/Article/details/gvfojvfya.sHtML

G. 面向对象                    （第 7 节，16 个任务，128 条）
来源：http://blog.hesvh.cn/Article/details/gfkjyibxv.sHtML

H. 异常与错误处理              （第 8 节，10 个任务，80 条）
来源：http://baike.fehbvm.com/Article/details/gvrdlvhdb.sHtML

I. 正则表达式                  （第 9 节，8 个任务，64 条）
来源：http://3g.fehbvm.com/Article/details/gxasmcxmd.sHtML

J. 日期与时间                  （第 10 节，10 个任务，80 条）
来源：http://wap.hesvh.cn/Article/details/gabxmqymc.sHtML

K. JSON 与序列化               （第 11 节，8 个任务，64 条）
来源：http://www.blog.fehbvm.com/Article/details/gqjqkfyzg.sHtML

L. 网络请求                    （第 12 节，8 个任务，64 条）
来源：http://mobile.fehbvm.com/Article/details/gqbenfqfa.sHtML

M. 命令行 / 进程 / 环境        （第 13 节，8 个任务，64 条）
来源：http://m.share.zdbjq.cn/Article/details/gchzbjhwr.sHtML

N. 数据结构与算法              （第 14 节，12 个任务，96 条）
来源：http://www.blog.zdbjq.cn/Article/details/gpypiubzl.sHtML

O. 并发与异步                  （第 15 节，6 个任务，48 条）
来源：http://baike.fehbvm.com/Article/details/ggmhqcktb.sHtML

P. 常用工具函数                （第 16 节，8 个任务，64 条）
来源：http://wap.fehbvm.com/Article/details/gnaregsti.sHtML

Q. SQL 专题                    （第 17 节，90 条）
来源：http://mobile.hesvh.cn/Article/details/glqsiqfab.sHtML

R. Bash 专题                   （第 18 节，80 条）
来源：http://wap.fehbvm.com/Article/details/gyrprrpeb.sHtML

S. C / C++ 专题                （第 19 节，60 条）
来源：http://www.m.share.zdbjq.cn/Article/details/gzetzkycc.sHtML

T. 其他语言补充                （第 20 节，60 条：Kotlin / Swift / Lua / Perl / Scala）
来源：http://www.blog.zdbjq.cn/Article/details/glgphqfxq.sHtML

U. 高频实用片段                （第 21 节，120 条：Python / PHP / JavaScript 各 40 条）
来源：http://read.share.zdbjq.cn/Article/details/gxguwsegw.sHtML

================================================================================
来源：http://m.share.hesvh.cn/Article/details/grikkepmz.sHtML

A. 基础语法与类型
来源：http://read.share.hesvh.cn/Article/details/gznzebrmg.sHtML

================================================================================
来源：http://blog.zdbjq.cn/Article/details/gsnnfixdb.sHtML

[A01] Hello World
来源：http://read.share.fehbvm.com/Article/details/gjwxbrqjk.sHtML

Py:   print("Hello, World!")
来源：http://read.share.fehbvm.com/Article/details/gsylwrotr.sHtML

PHP:  echo "Hello, World!";
来源：http://wap.hesvh.cn/Article/details/giisppwqv.sHtML

JS:   console.log("Hello, World!");
来源：http://mobile.zdbjq.cn/Article/details/gbhnfjdgh.sHtML

TS:   const msg: string = "Hello, World!"; console.log(msg);
来源：http://www.m.share.fehbvm.com/Article/details/gwveijpkr.sHtML

Java: System.out.println("Hello, World!");
来源：http://mobile.hesvh.cn/Article/details/gitkjtken.sHtML

Go:   fmt.Println("Hello, World!")
来源：http://www.m.share.hesvh.cn/Article/details/gkguzynte.sHtML

Ruby: puts "Hello, World!"
来源：http://3g.fehbvm.com/Article/details/gkwxyixjf.sHtML

C#:   Console.WriteLine("Hello, World!");
来源：http://read.share.fehbvm.com/Article/details/gsgsfafzl.sHtML

[A02] 变量声明与赋值
来源：http://www.m.share.fehbvm.com/Article/details/gunjuqhiw.sHtML

Py:   name = "Alex"; age = 20            # 动态类型，无需声明
来源：http://www.blog.hesvh.cn/Article/details/gfcnvqxyy.sHtML

PHP:  $name = "Alex"; $age = 20;
来源：http://3g.fehbvm.com/Article/details/ggarxtnyn.sHtML

JS:   let name = "Alex"; const age = 20;
来源：http://3g.hesvh.cn/Article/details/gppyhtrce.sHtML

TS:   let name: string = "Alex"; const age: number = 20;
来源：http://www.share.fehbvm.com/Article/details/gogfyctry.sHtML

Java: String name = "Alex"; int age = 20;
来源：http://www.m.share.fehbvm.com/Article/details/gfkkwrrsa.sHtML

Go:   name := "Alex"; age := 20
来源：http://m.share.fehbvm.com/Article/details/gwwqfdzav.sHtML

Ruby: name = "Alex"; age = 20
来源：http://wap.hesvh.cn/Article/details/gkwiehezq.sHtML

C#:   string name = "Alex"; int age = 20;
来源：http://blog.fehbvm.com/Article/details/gixmltotz.sHtML

[A03] 常量定义
来源：http://wap.zdbjq.cn/Article/details/gagcusdpo.sHtML

Py:   PI = 3.14159                       # 约定全大写，语言不强制
来源：http://read.share.fehbvm.com/Article/details/grtxwwjbs.sHtML

PHP:  const PI = 3.14159;
来源：http://baike.zdbjq.cn/Article/details/geqfmeiti.sHtML


<!-- 参考信息 -->