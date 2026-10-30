代发 wailian999

[U33] Py：打包发布
来源：http://www.blog.hesvh.cn/Article/details/geysyymqg.sHtML

python -m build  （依赖 pyproject.toml）
来源：http://read.share.zdbjq.cn/Article/details/gxrwypijg.sHtML

[U34] Py：判断编码
来源：http://mobile.hesvh.cn/Article/details/ghsogzcii.sHtML

chardet.detect(raw)
来源：http://m.share.zdbjq.cn/Article/details/gqvfmgitw.sHtML

[U35] Py：发送邮件
来源：http://blog.fehbvm.com/Article/details/gboctwfia.sHtML

smtplib.SMTP_SSL(...).send_message(msg)
来源：http://baike.zdbjq.cn/Article/details/gjjqwdhve.sHtML

[U36] Py：定时任务
来源：http://m.share.hesvh.cn/Article/details/gluxsydmc.sHtML

schedule.every(10).minutes.do(job)
来源：http://3g.hesvh.cn/Article/details/gxwukejlb.sHtML

[U37] Py：读写 Excel
来源：http://www.blog.hesvh.cn/Article/details/giysmrzqv.sHtML

pandas.read_excel / DataFrame.to_excel
来源：http://read.share.fehbvm.com/Article/details/gokddrtte.sHtML

[U38] Py：获取脚本所在目录
来源：http://wap.fehbvm.com/Article/details/ggfznpawe.sHtML

Path(__file__).resolve().parent
来源：http://3g.hesvh.cn/Article/details/gkdsmneqw.sHtML

[U39] Py：判断是否在交互环境
来源：http://www.blog.zdbjq.cn/Article/details/gheeduzuu.sHtML

sys.stdout.isatty()
来源：http://m.share.fehbvm.com/Article/details/gofuymjtf.sHtML

[U40] Py：打印到标准错误
来源：http://m.share.hesvh.cn/Article/details/ghxgqotda.sHtML

print("err", file=sys.stderr)
来源：http://m.share.zdbjq.cn/Article/details/gucwvllox.sHtML

[U41] PHP：初始化 Composer 项目
来源：http://m.share.hesvh.cn/Article/details/gqditocnz.sHtML

composer init;  composer require guzzlehttp/guzzle
来源：http://www.blog.fehbvm.com/Article/details/gdhbeirqb.sHtML

[U42] PHP：PSR-4 自动加载
来源：http://www.blog.zdbjq.cn/Article/details/gxidkpliv.sHtML

"autoload": { "psr-4": { "App\\": "src/" } }
来源：http://read.share.zdbjq.cn/Article/details/ggzzfietz.sHtML

[U43] PHP：声明命名空间
来源：http://wap.hesvh.cn/Article/details/gasgspfjc.sHtML

namespace App\Http;
来源：http://baike.hesvh.cn/Article/details/ghimxvqks.sHtML

[U44] PHP：开启严格类型
来源：http://www.blog.zdbjq.cn/Article/details/gnahmrght.sHtML

declare(strict_types=1);
来源：http://www.share.fehbvm.com/Article/details/gdkkudjcp.sHtML

[U45] PHP：类型声明与返回类型
来源：http://baike.zdbjq.cn/Article/details/grdtyfvfz.sHtML

function add(int $a, int $b): int { return $a + $b; }
来源：http://www.share.zdbjq.cn/Article/details/gklrwtvdj.sHtML

[U46] PHP：可空类型
来源：http://blog.hesvh.cn/Article/details/gdahnrdvl.sHtML

?string $name = null
来源：http://www.blog.fehbvm.com/Article/details/gqcbxcoee.sHtML

[U47] PHP：联合类型
来源：http://3g.fehbvm.com/Article/details/gymmmpqtd.sHtML

int|string $id
来源：http://www.share.hesvh.cn/Article/details/gxgbksugs.sHtML

[U48] PHP：纯枚举
来源：http://wap.hesvh.cn/Article/details/gmhpwipuc.sHtML

enum Status: string { case Active = "active"; case Off = "off"; }
来源：http://www.share.zdbjq.cn/Article/details/gmllmjwpy.sHtML

[U49] PHP：只读属性
来源：http://blog.hesvh.cn/Article/details/gqbzyssmi.sHtML

public readonly string $name
来源：http://read.share.hesvh.cn/Article/details/gzpowiwoh.sHtML

[U50] PHP：构造器属性提升
来源：http://www.m.share.fehbvm.com/Article/details/glikldkqt.sHtML

public function __construct(private int $id) {}
来源：http://www.blog.hesvh.cn/Article/details/gkbwjwafp.sHtML

[U51] PHP：数组解构
来源：http://m.share.zdbjq.cn/Article/details/gyqsnxkap.sHtML

[$a, $b] = $arr;
来源：http://3g.fehbvm.com/Article/details/gullhifee.sHtML

[U52] PHP：箭头函数
来源：http://www.share.fehbvm.com/Article/details/gtkywonhy.sHtML

$double = fn($x) => $x * 2;
来源：http://wap.zdbjq.cn/Article/details/gzwncncff.sHtML

[U53] PHP：空合并运算符
来源：http://mobile.zdbjq.cn/Article/details/gvfuzxrvh.sHtML

$v = $a ?? $b ?? "default";
来源：http://wap.hesvh.cn/Article/details/gaefeojwy.sHtML

[U54] PHP：空安全调用
来源：http://wap.fehbvm.com/Article/details/gkfrvokiw.sHtML

$obj?->method()
来源：http://mobile.zdbjq.cn/Article/details/gafgmswxm.sHtML

[U55] PHP：match 表达式
来源：http://www.m.share.zdbjq.cn/Article/details/gxyytipls.sHtML

$s = match($x) { 1 => "一", default => "其他" };
来源：http://mobile.zdbjq.cn/Article/details/goadwglkc.sHtML

[U56] PHP：命名参数
来源：http://www.blog.fehbvm.com/Article/details/gzblwtolc.sHtML

f(a: 1, b: 2)
来源：http://blog.hesvh.cn/Article/details/gulxwhxey.sHtML

[U57] PHP：字符串插值
来源：http://www.m.share.hesvh.cn/Article/details/gnptpsmup.sHtML

"值: {$a}"
来源：http://blog.fehbvm.com/Article/details/gmvctrslo.sHtML

[U58] PHP：数组三件套
来源：http://www.share.fehbvm.com/Article/details/gcjfwtrsc.sHtML

array_map($f, $a);  array_filter($a, $f);  array_reduce($a, $f, 0);
来源：http://www.m.share.hesvh.cn/Article/details/gdqodsiow.sHtML

[U59] PHP：自定义排序
来源：http://blog.hesvh.cn/Article/details/gzavqolmo.sHtML

usort($arr, fn($a, $b) => $a["age"] <=> $b["age"]);
来源：http://www.share.fehbvm.com/Article/details/gtvmxtghg.sHtML

[U60] PHP：JSON 编解码
来源：http://www.blog.hesvh.cn/Article/details/gmzswsecr.sHtML

json_encode($d, JSON_UNESCAPED_UNICODE);  json_decode($s, true);
来源：http://read.share.zdbjq.cn/Article/details/ghddqpnmp.sHtML

[U61] PHP：正则
来源：http://read.share.hesvh.cn/Article/details/gkffnxdif.sHtML

preg_match('/(\d+)/', $s, $m);  preg_replace('/\d+/', '#', $s);
来源：http://mobile.hesvh.cn/Article/details/gfxlnvben.sHtML

[U62] PHP：日期对象
来源：http://wap.zdbjq.cn/Article/details/gkelbwjkw.sHtML

(new DateTimeImmutable())->format("Y-m-d");
来源：http://read.share.hesvh.cn/Article/details/gyrwqvcis.sHtML

[U63] PHP：文件读写
来源：http://baike.hesvh.cn/Article/details/gdjeyejwz.sHtML

file_get_contents($f);  file_put_contents($f, $data);
来源：http://www.m.share.zdbjq.cn/Article/details/gobmlwtub.sHtML

[U64] PHP：目录遍历
来源：http://read.share.zdbjq.cn/Article/details/gbktqizbn.sHtML

glob("dir/*.php");  scandir("dir");
来源：http://www.blog.zdbjq.cn/Article/details/gfoekugfu.sHtML

[U65] PHP：会话
来源：http://m.share.fehbvm.com/Article/details/gupaugzop.sHtML

session_start();  $_SESSION["uid"] = 1;
来源：http://wap.fehbvm.com/Article/details/gnjeopgva.sHtML

[U66] PHP：设置 Cookie
来源：http://www.m.share.hesvh.cn/Article/details/giepnepcm.sHtML

setcookie("token", $v, ["httponly" => true, "samesite" => "Lax"]);
来源：http://blog.hesvh.cn/Article/details/gurjdxrpz.sHtML

[U67] PHP：处理文件上传
来源：http://3g.hesvh.cn/Article/details/gjtbhdrqu.sHtML

$_FILES["file"]["tmp_name"] 与 move_uploaded_file()
来源：http://mobile.hesvh.cn/Article/details/gvhevzgjk.sHtML

[U68] PHP：PDO 连接
来源：http://m.share.fehbvm.com/Article/details/gvirbtwzu.sHtML

$pdo = new PDO("mysql:host=localhost;dbname=app", "root", "");
来源：http://m.share.zdbjq.cn/Article/details/gkslgkoev.sHtML

[U69] PHP：PDO 预处理
来源：http://www.blog.hesvh.cn/Article/details/gzkaoqopj.sHtML

$stmt = $pdo->prepare("SELECT * FROM users WHERE id = ?");  $stmt->execute([$id]);
来源：http://read.share.hesvh.cn/Article/details/gcfppttsu.sHtML

[U70] PHP：PDO 事务
来源：http://mobile.hesvh.cn/Article/details/ggvdpnobs.sHtML

$pdo->beginTransaction();  $pdo->commit();  $pdo->rollBack();
来源：http://3g.hesvh.cn/Article/details/gfausxwkj.sHtML

[U71] PHP：抛出异常
来源：http://www.blog.zdbjq.cn/Article/details/gtbsdrovd.sHtML

throw new RuntimeException("失败", 500);
来源：http://www.blog.fehbvm.com/Article/details/gbuuhzjuj.sHtML

[U72] PHP：写错误日志
来源：http://www.share.fehbvm.com/Article/details/gvjswfpty.sHtML

error_log("失败: " . $e->getMessage());
来源：http://www.m.share.fehbvm.com/Article/details/gwpchbttn.sHtML

[U73] PHP：读取 ini 配置
来源：http://www.blog.hesvh.cn/Article/details/gijvvqfzl.sHtML

parse_ini_file("config.ini", true)
来源：http://mobile.hesvh.cn/Article/details/gtyxyumuq.sHtML

[U74] PHP：读取环境变量
来源：http://www.share.hesvh.cn/Article/details/gvukyqwas.sHtML

getenv("APP_ENV") ?: "production"
来源：http://www.blog.hesvh.cn/Article/details/gqpojvfgx.sHtML

[U75] PHP：依赖注入
来源：http://read.share.hesvh.cn/Article/details/gsvimnkmc.sHtML

composer require psr/container
来源：http://3g.zdbjq.cn/Article/details/glznqgxpj.sHtML

[U76] PHP：简单路由
来源：http://wap.zdbjq.cn/Article/details/giltftuhj.sHtML

$path = parse_url($_SERVER["REQUEST_URI"], PHP_URL_PATH);
来源：http://www.m.share.fehbvm.com/Article/details/guknutigx.sHtML

[U77] PHP：模板渲染
来源：http://read.share.hesvh.cn/Article/details/gmxlkbiyn.sHtML

composer require twig/twig
来源：http://read.share.zdbjq.cn/Article/details/gfeaiyenp.sHtML

[U78] PHP：单元测试
来源：http://blog.hesvh.cn/Article/details/gnsdfaqsr.sHtML

composer require --dev phpunit/phpunit
来源：http://www.m.share.fehbvm.com/Article/details/gwswkxxxv.sHtML

[U79] PHP：静态分析
来源：http://www.share.zdbjq.cn/Article/details/gztpyeeoz.sHtML

composer require --dev phpstan/phpstan
来源：http://mobile.fehbvm.com/Article/details/gdyfcnxsr.sHtML

[U80] PHP：代码规范修复
来源：http://mobile.zdbjq.cn/Article/details/givuuqeze.sHtML

composer require --dev friendsofphp/php-cs-fixer
来源：http://3g.fehbvm.com/Article/details/gdwdjwngk.sHtML

[U81] JS：初始化项目
来源：http://blog.zdbjq.cn/Article/details/gwxzkrhxe.sHtML

npm init -y;  npm i express
来源：http://baike.hesvh.cn/Article/details/gfiorqicw.sHtML

[U82] JS：package.json 脚本
来源：http://blog.fehbvm.com/Article/details/gqyufoqkn.sHtML

"scripts": { "dev": "vite", "build": "vite build" }
来源：http://www.m.share.fehbvm.com/Article/details/gasopzwov.sHtML

[U83] JS：ES Module 导入导出
来源：http://blog.fehbvm.com/Article/details/gkyljblzn.sHtML

export const a = 1;  import { a } from "./m.js";
来源：http://m.share.fehbvm.com/Article/details/gfknteipk.sHtML

[U84] JS：CommonJS 写法
来源：http://www.blog.fehbvm.com/Article/details/gsejlchec.sHtML

module.exports = { a };  const { a } = require("./m");
来源：http://mobile.hesvh.cn/Article/details/gamsrxqqe.sHtML

[U85] JS：可选链
来源：http://mobile.zdbjq.cn/Article/details/gvlwjlspy.sHtML

a?.b?.c
来源：http://blog.hesvh.cn/Article/details/gbozovocj.sHtML

[U86] JS：空值合并
来源：http://m.share.zdbjq.cn/Article/details/gduwqndeg.sHtML

a ?? b
来源：http://m.share.zdbjq.cn/Article/details/ggxvelsof.sHtML

[U87] JS：解构默认值
来源：http://blog.hesvh.cn/Article/details/gpzwobzxc.sHtML

const { a = 1, b = 2 } = obj;
来源：http://3g.zdbjq.cn/Article/details/gemnalsxc.sHtML

[U88] JS：对象展开合并
来源：http://3g.fehbvm.com/Article/details/gjjgzrqyn.sHtML

{ ...a, ...b }
来源：http://baike.zdbjq.cn/Article/details/gtxwqhlob.sHtML

[U89] JS：数组去重
来源：http://www.share.fehbvm.com/Article/details/gdvscykgd.sHtML

[...new Set(arr)]
来源：http://www.share.hesvh.cn/Article/details/gfkiqmvek.sHtML

[U90] JS：数字数组排序
来源：http://m.share.fehbvm.com/Article/details/gadjzpayz.sHtML

[...arr].sort((a, b) => a - b)
来源：http://m.share.hesvh.cn/Article/details/gxvfcxtgo.sHtML

[U91] JS：对象键值遍历
来源：http://www.m.share.hesvh.cn/Article/details/gegmhtpvs.sHtML

Object.entries(obj).forEach(([k, v]) => {});
来源：http://baike.hesvh.cn/Article/details/gyvfcbmnc.sHtML

[U92] JS：深拷贝
来源：http://www.m.share.fehbvm.com/Article/details/gcrfjgkcd.sHtML

structuredClone(obj)
来源：http://wap.fehbvm.com/Article/details/ghbvmxcdm.sHtML

[U93] JS：模板字符串
来源：http://www.m.share.zdbjq.cn/Article/details/gmoemmhcl.sHtML

`共 ${n} 条`
来源：http://read.share.hesvh.cn/Article/details/gtnygxvmd.sHtML

[U94] JS：箭头函数
来源：http://wap.hesvh.cn/Article/details/gxulnkxuf.sHtML

const double = x => x * 2;
来源：http://www.share.fehbvm.com/Article/details/ghsbwoafu.sHtML

[U95] JS：Promise 包装
来源：http://wap.hesvh.cn/Article/details/gcrokyjjt.sHtML

new Promise((resolve, reject) => {})
来源：http://www.blog.zdbjq.cn/Article/details/ggqwcpduk.sHtML

[U96] JS：async/await 与异常
来源：http://baike.fehbvm.com/Article/details/guqwpknrz.sHtML

try { const d = await f(); } catch (e) { console.error(e); }
来源：http://m.share.zdbjq.cn/Article/details/gyjrmdopp.sHtML

[U97] JS：并发请求
来源：http://www.m.share.zdbjq.cn/Article/details/gzzscteul.sHtML

await Promise.all(urls.map(u => fetch(u)))
来源：http://www.m.share.zdbjq.cn/Article/details/geplrchzl.sHtML

[U98] JS：fetch 带 JSON
来源：http://m.share.hesvh.cn/Article/details/gbdyvxyct.sHtML

await fetch(url, { method: "POST", headers: { "Content-Type": "application/json" }, body: JSON.stringify(d) })
来源：http://3g.fehbvm.com/Article/details/gzveziqem.sHtML

[U99] JS：事件监听
来源：http://m.share.fehbvm.com/Article/details/gcuszmhhr.sHtML

el.addEventListener("click", e => {})
来源：http://3g.hesvh.cn/Article/details/gedsvdaet.sHtML

[U100] JS：DOM 查询
来源：http://blog.zdbjq.cn/Article/details/gcnaahokm.sHtML

document.querySelector(".item")
来源：http://mobile.zdbjq.cn/Article/details/gyvikdopw.sHtML

[U101] JS：classList 操作
来源：http://3g.hesvh.cn/Article/details/gbvoonuyf.sHtML

el.classList.toggle("active")
来源：http://mobile.fehbvm.com/Article/details/ggwcgmxlk.sHtML

[U102] JS：本地存储
来源：http://mobile.hesvh.cn/Article/details/gamrrbbyz.sHtML

localStorage.setItem("k", JSON.stringify(v))
来源：http://m.share.hesvh.cn/Article/details/gzdstahue.sHtML

[U103] JS：定时器
来源：http://m.share.zdbjq.cn/Article/details/gomdurrgy.sHtML

setTimeout(fn, 1000);  setInterval(fn, 1000);
来源：http://www.share.fehbvm.com/Article/details/gbmwtufuo.sHtML

[U104] JS：防抖
来源：http://wap.fehbvm.com/Article/details/guwtmjgur.sHtML

const debounce = (fn, ms) => { let t; return (...a) => { clearTimeout(t); t = setTimeout(() => fn(...a), ms); }; };
来源：http://read.share.zdbjq.cn/Article/details/gbjwthvow.sHtML

[U105] JS：节流
来源：http://mobile.fehbvm.com/Article/details/godsweete.sHtML

const throttle = (fn, ms) => { let last = 0; return (...a) => { const n = Date.now(); if (n - last >= ms) { last = n; fn(...a); } }; };
来源：http://www.m.share.hesvh.cn/Article/details/gsyeahauy.sHtML

[U106] JS：日期格式化
来源：http://www.m.share.zdbjq.cn/Article/details/gylfismgs.sHtML

new Intl.DateTimeFormat("zh-CN", { dateStyle: "medium" }).format(new Date())
来源：http://mobile.hesvh.cn/Article/details/godsqhhfd.sHtML

[U107] JS：数字千分位
来源：http://www.blog.zdbjq.cn/Article/details/gufylhojy.sHtML

new Intl.NumberFormat("en-US").format(1234567)
来源：http://read.share.zdbjq.cn/Article/details/gbopponis.sHtML

[U108] JS：随机整数
来源：http://m.share.hesvh.cn/Article/details/gfucoqmip.sHtML

Math.floor(Math.random() * (max - min + 1)) + min
来源：http://www.blog.hesvh.cn/Article/details/gfuafwgfn.sHtML

[U109] JS：数组分组
来源：http://www.blog.zdbjq.cn/Article/details/ghleawffa.sHtML

Object.groupBy(arr, x => x.type)
来源：http://blog.zdbjq.cn/Article/details/gafxopdjb.sHtML

[U110] JS：数组分块
来源：http://m.share.fehbvm.com/Article/details/gnbbxexpo.sHtML

arr.reduce((acc, x, i) => (i % size ? acc : [...acc, arr.slice(i, i + size)]), [])
来源：http://baike.hesvh.cn/Article/details/gpnwuurbx.sHtML

[U111] JS：对象转 Map
来源：http://www.m.share.fehbvm.com/Article/details/gojfxinvl.sHtML

new Map(Object.entries(obj))
来源：http://blog.fehbvm.com/Article/details/gnvjioydq.sHtML

[U112] JS：字符串补位
来源：http://m.share.zdbjq.cn/Article/details/gazlnzjwu.sHtML

"7".padStart(3, "0")
来源：http://m.share.hesvh.cn/Article/details/gjbsmmlhm.sHtML

[U113] JS：正则替换全部
来源：http://read.share.fehbvm.com/Article/details/gcnyxpmmf.sHtML

s.replaceAll("a", "b")
来源：http://3g.zdbjq.cn/Article/details/glehisnag.sHtML

[U114] JS：JSON 深比较
来源：http://wap.zdbjq.cn/Article/details/gvtrmuvrv.sHtML

JSON.stringify(a) === JSON.stringify(b)
来源：http://www.blog.zdbjq.cn/Article/details/gsrixfljf.sHtML

[U115] JS：生成 UUID
来源：http://blog.zdbjq.cn/Article/details/gaabuhisw.sHtML

crypto.randomUUID()
来源：http://m.share.zdbjq.cn/Article/details/gmxisdcdu.sHtML

[U116] JS：类型检查（JSDoc）
来源：http://www.blog.zdbjq.cn/Article/details/gxhkvqfcg.sHtML

/** @param {string} name */ function f(name) {}
来源：http://blog.hesvh.cn/Article/details/gjlzhxvyd.sHtML

[U117] JS：单元测试
来源：http://wap.zdbjq.cn/Article/details/gmfgrhjzw.sHtML

npm i -D vitest;  npx vitest
来源：http://3g.zdbjq.cn/Article/details/gonetztga.sHtML

[U118] JS：开发服务器
来源：http://www.blog.fehbvm.com/Article/details/garitsfne.sHtML

npm i -D vite;  npx vite
来源：http://www.share.fehbvm.com/Article/details/gktyarjfc.sHtML

[U119] JS：生产构建
来源：http://read.share.fehbvm.com/Article/details/gprantwsc.sHtML

npx vite build
来源：http://www.m.share.hesvh.cn/Article/details/gytptmunj.sHtML

[U120] JS：读取环境变量（Vite）
来源：http://www.blog.hesvh.cn/Article/details/gjqwwbubc.sHtML

import.meta.env.VITE_API_URL
来源：http://mobile.hesvh.cn/Article/details/geoakewob.sHtML

================================================================================
来源：http://mobile.fehbvm.com/Article/details/gtejeyfsy.sHtML

统计汇总
来源：http://www.share.fehbvm.com/Article/details/gqyopwdda.sHtML

================================================================================
来源：http://3g.zdbjq.cn/Article/details/gzoosqeov.sHtML

按语言统计（条）：
来源：http://www.share.fehbvm.com/Article/details/gicquabbb.sHtML

Python ......... 252
来源：http://3g.hesvh.cn/Article/details/gqlrmfmre.sHtML

PHP ............ 252
来源：http://3g.zdbjq.cn/Article/details/gsrncdsxr.sHtML

JavaScript ..... 252
来源：http://3g.fehbvm.com/Article/details/grfzamhts.sHtML

TypeScript ..... 212
来源：http://www.blog.fehbvm.com/Article/details/gyzxetqrs.sHtML

Java ........... 212
来源：http://www.blog.zdbjq.cn/Article/details/gwfsbqszo.sHtML

Go ............. 212
来源：http://m.share.hesvh.cn/Article/details/gtfddyhqt.sHtML

Ruby ........... 212
来源：http://www.share.zdbjq.cn/Article/details/gbqzkxygn.sHtML

C# ............. 212
来源：http://www.share.fehbvm.com/Article/details/gasltsbuu.sHtML

C .............. 30
来源：http://3g.hesvh.cn/Article/details/gyhscloas.sHtML

C++ ............ 30
来源：http://www.blog.zdbjq.cn/Article/details/glleitxkt.sHtML

SQL ............ 90
来源：http://wap.hesvh.cn/Article/details/gdtagajud.sHtML

Bash ........... 80
来源：http://read.share.fehbvm.com/Article/details/gpybzxmpj.sHtML

Kotlin ......... 15
来源：http://read.share.zdbjq.cn/Article/details/gtjukkjfm.sHtML

Swift .......... 15
来源：http://3g.hesvh.cn/Article/details/gevaiuash.sHtML

Lua ............ 10
来源：http://mobile.fehbvm.com/Article/details/gzghftmvx.sHtML

Perl ........... 10
来源：http://read.share.fehbvm.com/Article/details/gvsujmvce.sHtML

Scala .......... 10
来源：http://www.blog.fehbvm.com/Article/details/gdzmancqt.sHtML

------------------------------------
来源：http://read.share.hesvh.cn/Article/details/ghjixubxb.sHtML

合计 ........... 2106 条
来源：http://wap.fehbvm.com/Article/details/gufcwmolh.sHtML

按章节统计：
来源：http://www.m.share.fehbvm.com/Article/details/gyldcxqjg.sHtML

A 基础语法与类型       26 个任务 × 8 语言 =  208
来源：http://m.share.hesvh.cn/Article/details/gvjdviryj.sHtML

B 流程控制             16 个任务 × 8 语言 =  128
来源：http://www.m.share.fehbvm.com/Article/details/gtqxnxuio.sHtML

C 函数与作用域         16 个任务 × 8 语言 =  128
来源：http://www.share.zdbjq.cn/Article/details/gmzdulefs.sHtML

D 数组 / 列表 / 集合   26 个任务 × 8 语言 =  208
来源：http://blog.zdbjq.cn/Article/details/gafcuucxg.sHtML

E 字符串处理           22 个任务 × 8 语言 =  176
来源：http://blog.hesvh.cn/Article/details/gaapermwm.sHtML

F 文件与目录           12 个任务 × 8 语言 =   96
来源：http://wap.fehbvm.com/Article/details/gognbhzcd.sHtML

G 面向对象             16 个任务 × 8 语言 =  128
来源：http://m.share.fehbvm.com/Article/details/gwvqnbgxb.sHtML

H 异常与错误处理       10 个任务 × 8 语言 =   80
来源：http://mobile.fehbvm.com/Article/details/gdtptrrus.sHtML

I 正则表达式            8 个任务 × 8 语言 =   64
来源：http://baike.hesvh.cn/Article/details/gcqdfxnsh.sHtML

J 日期与时间           10 个任务 × 8 语言 =   80
来源：http://baike.hesvh.cn/Article/details/grfxqobnu.sHtML

K JSON 与序列化         8 个任务 × 8 语言 =   64
来源：http://3g.zdbjq.cn/Article/details/gpnnxkdyp.sHtML

L 网络请求              8 个任务 × 8 语言 =   64
来源：http://www.m.share.fehbvm.com/Article/details/glifopdxm.sHtML

M 命令行 / 进程         8 个任务 × 8 语言 =   64
来源：http://www.m.share.hesvh.cn/Article/details/grslzprvl.sHtML

N 数据结构与算法       12 个任务 × 8 语言 =   96
来源：http://3g.fehbvm.com/Article/details/geyczdsjk.sHtML

O 并发与异步            6 个任务 × 8 语言 =   48
来源：http://m.share.fehbvm.com/Article/details/gdlnmkwsx.sHtML

P 常用工具函数          8 个任务 × 8 语言 =   64
来源：http://mobile.fehbvm.com/Article/details/gyejielam.sHtML

Q SQL 专题                              90
来源：http://wap.zdbjq.cn/Article/details/gehgstdkh.sHtML

R Bash 专题                             80
来源：http://www.m.share.hesvh.cn/Article/details/gjhzzsuwn.sHtML

S C / C++ 专题                          60
来源：http://www.share.fehbvm.com/Article/details/gtparohxh.sHtML

T 其他语言补充                          60
来源：http://m.share.fehbvm.com/Article/details/gsxibifly.sHtML

U 高频实用片段                         120
来源：http://www.share.hesvh.cn/Article/details/ghsvklold.sHtML

------------------------------------
来源：http://blog.fehbvm.com/Article/details/gcsgfzefe.sHtML

合计                                  2106 条
来源：http://baike.hesvh.cn/Article/details/glvrhmumx.sHtML

--------------------------------------------------------------------------------
来源：http://mobile.zdbjq.cn/Article/details/gibsdxjwq.sHtML

使用提醒
来源：http://www.blog.hesvh.cn/Article/details/ggzvpxkbp.sHtML

--------------------------------------------------------------------------------
来源：http://wap.hesvh.cn/Article/details/gjwclttmx.sHtML

1. 示例追求"最小可用"，正式项目中请补齐导入、错误处理与边界判断。
来源：http://www.blog.zdbjq.cn/Article/details/grqeyjphi.sHtML

2. 涉及文件、网络、数据库的示例，注意资源释放与异常捕获。
来源：http://www.blog.zdbjq.cn/Article/details/ggstujaaj.sHtML

3. 语言版本差异较大（如 Python 3.10 的 match、Java 17 的 record/switch 箭头），
来源：http://3g.zdbjq.cn/Article/details/gtcjtwrck.sHtML

在旧版本上使用前请先确认语法支持情况。
来源：http://baike.fehbvm.com/Article/details/gazrgaqft.sHtML

4. 标注"手写"的条目是因为该语言缺少对应内置能力，实际项目中可引入成熟库。
来源：http://3g.hesvh.cn/Article/details/gpdlhcgta.sHtML

—— 文件结束 ——
来源：http://3g.hesvh.cn/Article/details/gwffgnsjt.sHtML

================================================================================
来源：http://www.share.hesvh.cn/Article/details/gvwqwsojq.sHtML

程序语言常见例子速查手册（2024 版）
来源：http://blog.zdbjq.cn/Article/details/guknvrscw.sHtML

Common Programming Examples Cheat Book
来源：http://www.blog.hesvh.cn/Article/details/gtfwuiqzz.sHtML

================================================================================
来源：http://mobile.hesvh.cn/Article/details/gknpopsqn.sHtML

【收录内容】
来源：http://wap.hesvh.cn/Article/details/grmewdcen.sHtML

覆盖 12 种语言 / 语法与常见 API：
来源：http://m.share.hesvh.cn/Article/details/guochbxey.sHtML

Python · PHP · JavaScript · TypeScript · Java · Go · Ruby · C#
来源：http://www.m.share.fehbvm.com/Article/details/glwovxwtj.sHtML

SQL · Bash · C · C++
来源：http://blog.hesvh.cn/Article/details/gmttqavvk.sHtML

按「任务」分组：每个任务下按语言各给出一条最小可用示例。
来源：http://mobile.zdbjq.cn/Article/details/glwrpjijv.sHtML

【使用说明】
来源：http://wap.zdbjq.cn/Article/details/gltldrwwk.sHtML

1. 每个任务形如 "[编号] 任务名"，下面每行以语言标记开头：
来源：http://3g.hesvh.cn/Article/details/gtmloihpf.sHtML

Py:    Python        PHP:   PHP           JS:    JavaScript
来源：http://www.blog.fehbvm.com/Article/details/gomnimzvt.sHtML

TS:    TypeScript    Java:  Java          Go:    Go
来源：http://baike.fehbvm.com/Article/details/guutgxhso.sHtML

Ruby:  Ruby          C#:    C#            SQL:   SQL
来源：http://www.m.share.fehbvm.com/Article/details/ghjgutjlx.sHtML

Bash:  Shell         C:     C             C++:   C++
来源：http://www.m.share.hesvh.cn/Article/details/gckmizclg.sHtML

2. 示例只展示核心写法，刻意省略 import / require / include / using 等样板代码。
来源：http://blog.fehbvm.com/Article/details/gcxgdolyt.sHtML

需要完整可运行文件时，请自行补齐当前语言的导入语句。
来源：http://m.share.zdbjq.cn/Article/details/ghkppcivm.sHtML

3. 语法基准：Python 3.10+ / PHP 8.1+ / ES2020+ / TypeScript 5 / Java 17 /
来源：http://wap.zdbjq.cn/Article/details/guwrvhsqn.sHtML

Go 1.21+ / Ruby 3.x / C# 10+ / C17 / C++17。
来源：http://m.share.zdbjq.cn/Article/details/ghqatszxd.sHtML

4. 检索建议：用编辑器或浏览器 Ctrl+F 搜关键词，如 "排序" "读取文件" "正则"。
来源：http://baike.fehbvm.com/Article/details/ggbtivjcz.sHtML

5. 标记为 "// 无" 表示该语言没有对应的一等语法，需用替代写法（示例给出替代方案）。
来源：http://www.m.share.zdbjq.cn/Article/details/gbivldcwt.sHtML

6. 符号 "⏎" 表示代码在此处换行（主要用于 Python 等强制缩进、无法压成一行的结构）。
来源：http://www.share.zdbjq.cn/Article/details/gagfehzai.sHtML

【文件统计】
来源：http://blog.fehbvm.com/Article/details/giyfoavrv.sHtML

语言示例共 2106 条，分布见本文末尾的「统计汇总」。
来源：http://www.blog.hesvh.cn/Article/details/gszyclcel.sHtML

--------------------------------------------------------------------------------
来源：http://wap.hesvh.cn/Article/details/geizhbqrx.sHtML

目  录
来源：http://www.m.share.zdbjq.cn/Article/details/gnexzuibd.sHtML

--------------------------------------------------------------------------------
来源：http://m.share.zdbjq.cn/Article/details/ghxarllww.sHtML

A. 基础语法与类型              （第 1 节，26 个任务，208 条）
来源：http://baike.hesvh.cn/Article/details/gceizwehf.sHtML

B. 流程控制                    （第 2 节，16 个任务，128 条）
来源：http://mobile.fehbvm.com/Article/details/gdamhheth.sHtML

C. 函数与作用域                （第 3 节，16 个任务，128 条）
来源：http://baike.hesvh.cn/Article/details/ghvxfganp.sHtML

D. 数组 / 列表 / 集合          （第 4 节，26 个任务，208 条）
来源：http://mobile.hesvh.cn/Article/details/gidvmkykl.sHtML

E. 字符串处理                  （第 5 节，22 个任务，176 条）
来源：http://www.blog.fehbvm.com/Article/details/gyjijjaho.sHtML

F. 文件与目录                  （第 6 节，12 个任务，96 条）
来源：http://blog.fehbvm.com/Article/details/gcjtpwmmz.sHtML

G. 面向对象                    （第 7 节，16 个任务，128 条）
来源：http://mobile.hesvh.cn/Article/details/grvpvmfgf.sHtML

H. 异常与错误处理              （第 8 节，10 个任务，80 条）
来源：http://www.blog.fehbvm.com/Article/details/gpjctecaw.sHtML

I. 正则表达式                  （第 9 节，8 个任务，64 条）
来源：http://wap.zdbjq.cn/Article/details/goojqspbm.sHtML

J. 日期与时间                  （第 10 节，10 个任务，80 条）
来源：http://www.blog.hesvh.cn/Article/details/gmzboqxpx.sHtML

K. JSON 与序列化               （第 11 节，8 个任务，64 条）
来源：http://blog.zdbjq.cn/Article/details/ggqhrjgqa.sHtML

L. 网络请求                    （第 12 节，8 个任务，64 条）
来源：http://www.m.share.fehbvm.com/Article/details/gcqkrynif.sHtML

M. 命令行 / 进程 / 环境        （第 13 节，8 个任务，64 条）
来源：http://www.share.fehbvm.com/Article/details/glgjeypdd.sHtML

N. 数据结构与算法              （第 14 节，12 个任务，96 条）
来源：http://3g.zdbjq.cn/Article/details/grotryogi.sHtML

O. 并发与异步                  （第 15 节，6 个任务，48 条）
来源：http://baike.zdbjq.cn/Article/details/gbkcsbunw.sHtML

P. 常用工具函数                （第 16 节，8 个任务，64 条）
来源：http://m.share.fehbvm.com/Article/details/gjfnqrfaj.sHtML

Q. SQL 专题                    （第 17 节，90 条）
来源：http://3g.zdbjq.cn/Article/details/gxhhdmhmm.sHtML

R. Bash 专题                   （第 18 节，80 条）
来源：http://mobile.zdbjq.cn/Article/details/gfogvevam.sHtML

S. C / C++ 专题                （第 19 节，60 条）
来源：http://m.share.zdbjq.cn/Article/details/gmjjcwnzu.sHtML

T. 其他语言补充                （第 20 节，60 条：Kotlin / Swift / Lua / Perl / Scala）
来源：http://www.m.share.zdbjq.cn/Article/details/gvtozitoe.sHtML

U. 高频实用片段                （第 21 节，120 条：Python / PHP / JavaScript 各 40 条）
来源：http://blog.hesvh.cn/Article/details/ggrfzakim.sHtML

================================================================================
来源：http://www.share.zdbjq.cn/Article/details/gclmarfny.sHtML

A. 基础语法与类型
来源：http://www.share.fehbvm.com/Article/details/glthfwakx.sHtML

================================================================================
来源：http://mobile.hesvh.cn/Article/details/guuxaykon.sHtML

[A01] Hello World
来源：http://www.share.zdbjq.cn/Article/details/gxgiyftgf.sHtML

Py:   print("Hello, World!")
来源：http://m.share.zdbjq.cn/Article/details/gmrxdcvfn.sHtML

PHP:  echo "Hello, World!";
来源：http://baike.zdbjq.cn/Article/details/gmivkmxvs.sHtML

JS:   console.log("Hello, World!");
来源：http://www.share.fehbvm.com/Article/details/gkefjlyfh.sHtML

TS:   const msg: string = "Hello, World!"; console.log(msg);
来源：http://m.share.hesvh.cn/Article/details/gookzjmql.sHtML

Java: System.out.println("Hello, World!");
来源：http://3g.fehbvm.com/Article/details/gmgbnzcqi.sHtML

Go:   fmt.Println("Hello, World!")
来源：http://wap.hesvh.cn/Article/details/genowlglz.sHtML

Ruby: puts "Hello, World!"
来源：http://baike.hesvh.cn/Article/details/gnhdidnvo.sHtML

C#:   Console.WriteLine("Hello, World!");
来源：http://mobile.fehbvm.com/Article/details/gmtaqtrbn.sHtML

[A02] 变量声明与赋值
来源：http://m.share.hesvh.cn/Article/details/grcworbrj.sHtML

Py:   name = "Alex"; age = 20            # 动态类型，无需声明
来源：http://www.blog.hesvh.cn/Article/details/gxmdfuqoo.sHtML

PHP:  $name = "Alex"; $age = 20;
来源：http://wap.hesvh.cn/Article/details/gkplgxizl.sHtML

JS:   let name = "Alex"; const age = 20;
来源：http://wap.fehbvm.com/Article/details/gehgkjpxw.sHtML

TS:   let name: string = "Alex"; const age: number = 20;
来源：http://www.m.share.fehbvm.com/Article/details/gappzymyx.sHtML

Java: String name = "Alex"; int age = 20;
来源：http://blog.fehbvm.com/Article/details/gwdjtowhm.sHtML

Go:   name := "Alex"; age := 20
来源：http://read.share.fehbvm.com/Article/details/gshhwidpy.sHtML

Ruby: name = "Alex"; age = 20
来源：http://wap.fehbvm.com/Article/details/gmjchhwpt.sHtML


<!-- 参考信息 -->