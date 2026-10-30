代发 wailian999

[U31] Py：单测
来源：http://3g.zdbjq.cn/Article/details/gxktngafc.sHtML

python -m pytest -q
来源：http://www.m.share.zdbjq.cn/Article/details/gwyanmjlr.sHtML

[U32] Py：代码格式化
来源：http://blog.fehbvm.com/Article/details/gkgrdvqrx.sHtML

ruff format . && ruff check --fix .
来源：http://wap.hesvh.cn/Article/details/glewlwyxc.sHtML

[U33] Py：打包发布
来源：http://m.share.zdbjq.cn/Article/details/gykqvfssf.sHtML

python -m build  （依赖 pyproject.toml）
来源：http://baike.fehbvm.com/Article/details/gebwmqeku.sHtML

[U34] Py：判断编码
来源：http://wap.hesvh.cn/Article/details/ggvmzvkyz.sHtML

chardet.detect(raw)
来源：http://www.blog.fehbvm.com/Article/details/ggexarejo.sHtML

[U35] Py：发送邮件
来源：http://www.blog.zdbjq.cn/Article/details/gjjispubh.sHtML

smtplib.SMTP_SSL(...).send_message(msg)
来源：http://www.blog.fehbvm.com/Article/details/gjsqacdqf.sHtML

[U36] Py：定时任务
来源：http://www.m.share.fehbvm.com/Article/details/gdckjtehb.sHtML

schedule.every(10).minutes.do(job)
来源：http://www.blog.hesvh.cn/Article/details/gcbhquace.sHtML

[U37] Py：读写 Excel
来源：http://www.share.zdbjq.cn/Article/details/gohvvinzo.sHtML

pandas.read_excel / DataFrame.to_excel
来源：http://3g.fehbvm.com/Article/details/gydkrqorj.sHtML

[U38] Py：获取脚本所在目录
来源：http://read.share.hesvh.cn/Article/details/gksesklbt.sHtML

Path(__file__).resolve().parent
来源：http://blog.fehbvm.com/Article/details/gjbztbepi.sHtML

[U39] Py：判断是否在交互环境
来源：http://www.blog.hesvh.cn/Article/details/gdczxfegh.sHtML

sys.stdout.isatty()
来源：http://www.m.share.fehbvm.com/Article/details/gktfhpltr.sHtML

[U40] Py：打印到标准错误
来源：http://m.share.hesvh.cn/Article/details/gnbyklfwm.sHtML

print("err", file=sys.stderr)
来源：http://read.share.zdbjq.cn/Article/details/gfsffwubp.sHtML

[U41] PHP：初始化 Composer 项目
来源：http://3g.fehbvm.com/Article/details/gcxlfxava.sHtML

composer init;  composer require guzzlehttp/guzzle
来源：http://www.blog.hesvh.cn/Article/details/gudeaukbh.sHtML

[U42] PHP：PSR-4 自动加载
来源：http://blog.zdbjq.cn/Article/details/gkcnykwww.sHtML

"autoload": { "psr-4": { "App\\": "src/" } }
来源：http://blog.zdbjq.cn/Article/details/glpwpshho.sHtML

[U43] PHP：声明命名空间
来源：http://baike.zdbjq.cn/Article/details/gdhgffqfg.sHtML

namespace App\Http;
来源：http://mobile.hesvh.cn/Article/details/gofvguyxi.sHtML

[U44] PHP：开启严格类型
来源：http://www.blog.hesvh.cn/Article/details/ggschsflp.sHtML

declare(strict_types=1);
来源：http://baike.zdbjq.cn/Article/details/gtdmamzvf.sHtML

[U45] PHP：类型声明与返回类型
来源：http://read.share.fehbvm.com/Article/details/gzngxagwj.sHtML

function add(int $a, int $b): int { return $a + $b; }
来源：http://read.share.fehbvm.com/Article/details/gjelhihgs.sHtML

[U46] PHP：可空类型
来源：http://m.share.hesvh.cn/Article/details/gzecwwzgr.sHtML

?string $name = null
来源：http://read.share.fehbvm.com/Article/details/gggjlnfhg.sHtML

[U47] PHP：联合类型
来源：http://www.share.zdbjq.cn/Article/details/gpczgoqjl.sHtML

int|string $id
来源：http://www.blog.fehbvm.com/Article/details/gkhisobeg.sHtML

[U48] PHP：纯枚举
来源：http://mobile.fehbvm.com/Article/details/gncbcreng.sHtML

enum Status: string { case Active = "active"; case Off = "off"; }
来源：http://www.share.fehbvm.com/Article/details/gdcbgkgqb.sHtML

[U49] PHP：只读属性
来源：http://3g.hesvh.cn/Article/details/gqwnnsdvr.sHtML

public readonly string $name
来源：http://blog.fehbvm.com/Article/details/gcbdopttm.sHtML

[U50] PHP：构造器属性提升
来源：http://m.share.zdbjq.cn/Article/details/gfygzwmzg.sHtML

public function __construct(private int $id) {}
来源：http://blog.fehbvm.com/Article/details/gkkldksye.sHtML

[U51] PHP：数组解构
来源：http://m.share.zdbjq.cn/Article/details/gnonyyzmt.sHtML

[$a, $b] = $arr;
来源：http://www.blog.zdbjq.cn/Article/details/gbsipcwvl.sHtML

[U52] PHP：箭头函数
来源：http://wap.hesvh.cn/Article/details/gazkccxxk.sHtML

$double = fn($x) => $x * 2;
来源：http://mobile.zdbjq.cn/Article/details/gotbsjqjt.sHtML

[U53] PHP：空合并运算符
来源：http://www.m.share.hesvh.cn/Article/details/gpxpdseev.sHtML

$v = $a ?? $b ?? "default";
来源：http://baike.hesvh.cn/Article/details/ggamughps.sHtML

[U54] PHP：空安全调用
来源：http://3g.fehbvm.com/Article/details/ghudcucfx.sHtML

$obj?->method()
来源：http://mobile.hesvh.cn/Article/details/gcydncykr.sHtML

[U55] PHP：match 表达式
来源：http://wap.fehbvm.com/Article/details/gqooalxpw.sHtML

$s = match($x) { 1 => "一", default => "其他" };
来源：http://www.blog.hesvh.cn/Article/details/grfqwwlin.sHtML

[U56] PHP：命名参数
来源：http://www.share.hesvh.cn/Article/details/gsqscujho.sHtML

f(a: 1, b: 2)
来源：http://www.share.fehbvm.com/Article/details/gecfrpsua.sHtML

[U57] PHP：字符串插值
来源：http://www.m.share.zdbjq.cn/Article/details/gzifaupty.sHtML

"值: {$a}"
来源：http://mobile.hesvh.cn/Article/details/ghstkdvrv.sHtML

[U58] PHP：数组三件套
来源：http://www.share.zdbjq.cn/Article/details/gosofigsx.sHtML

array_map($f, $a);  array_filter($a, $f);  array_reduce($a, $f, 0);
来源：http://read.share.fehbvm.com/Article/details/gpbrthjdo.sHtML

[U59] PHP：自定义排序
来源：http://baike.fehbvm.com/Article/details/grkryvryi.sHtML

usort($arr, fn($a, $b) => $a["age"] <=> $b["age"]);
来源：http://www.m.share.hesvh.cn/Article/details/gdqqqkisr.sHtML

[U60] PHP：JSON 编解码
来源：http://www.share.fehbvm.com/Article/details/gsunnxnnh.sHtML

json_encode($d, JSON_UNESCAPED_UNICODE);  json_decode($s, true);
来源：http://www.blog.fehbvm.com/Article/details/gkoqltjlc.sHtML

[U61] PHP：正则
来源：http://blog.zdbjq.cn/Article/details/gzncyeaez.sHtML

preg_match('/(\d+)/', $s, $m);  preg_replace('/\d+/', '#', $s);
来源：http://3g.zdbjq.cn/Article/details/gnzzuqjja.sHtML

[U62] PHP：日期对象
来源：http://read.share.fehbvm.com/Article/details/ggeeddrgi.sHtML

(new DateTimeImmutable())->format("Y-m-d");
来源：http://mobile.zdbjq.cn/Article/details/gsykydjww.sHtML

[U63] PHP：文件读写
来源：http://mobile.fehbvm.com/Article/details/gjqwbagnw.sHtML

file_get_contents($f);  file_put_contents($f, $data);
来源：http://www.blog.hesvh.cn/Article/details/gphaicgey.sHtML

[U64] PHP：目录遍历
来源：http://mobile.zdbjq.cn/Article/details/gvhnsveye.sHtML

glob("dir/*.php");  scandir("dir");
来源：http://baike.zdbjq.cn/Article/details/gfucjwcdd.sHtML

[U65] PHP：会话
来源：http://baike.zdbjq.cn/Article/details/gyriavoco.sHtML

session_start();  $_SESSION["uid"] = 1;
来源：http://www.share.zdbjq.cn/Article/details/gmpxkwljb.sHtML

[U66] PHP：设置 Cookie
来源：http://www.m.share.hesvh.cn/Article/details/gzzbjxfvb.sHtML

setcookie("token", $v, ["httponly" => true, "samesite" => "Lax"]);
来源：http://blog.zdbjq.cn/Article/details/gyipolehx.sHtML

[U67] PHP：处理文件上传
来源：http://baike.fehbvm.com/Article/details/gasuognuj.sHtML

$_FILES["file"]["tmp_name"] 与 move_uploaded_file()
来源：http://wap.hesvh.cn/Article/details/gfhkqkyxw.sHtML

[U68] PHP：PDO 连接
来源：http://www.blog.zdbjq.cn/Article/details/gentczepr.sHtML

$pdo = new PDO("mysql:host=localhost;dbname=app", "root", "");
来源：http://www.blog.zdbjq.cn/Article/details/glqxztgwj.sHtML

[U69] PHP：PDO 预处理
来源：http://3g.hesvh.cn/Article/details/godnxbhlx.sHtML

$stmt = $pdo->prepare("SELECT * FROM users WHERE id = ?");  $stmt->execute([$id]);
来源：http://3g.hesvh.cn/Article/details/gfaovjowi.sHtML

[U70] PHP：PDO 事务
来源：http://read.share.zdbjq.cn/Article/details/gyxgyacyv.sHtML

$pdo->beginTransaction();  $pdo->commit();  $pdo->rollBack();
来源：http://mobile.zdbjq.cn/Article/details/gqrdmzbul.sHtML

[U71] PHP：抛出异常
来源：http://www.share.fehbvm.com/Article/details/gklmtsqmy.sHtML

throw new RuntimeException("失败", 500);
来源：http://baike.hesvh.cn/Article/details/gmnfaxysi.sHtML

[U72] PHP：写错误日志
来源：http://baike.zdbjq.cn/Article/details/gioesfjxc.sHtML

error_log("失败: " . $e->getMessage());
来源：http://read.share.fehbvm.com/Article/details/gozwmmxvl.sHtML

[U73] PHP：读取 ini 配置
来源：http://3g.zdbjq.cn/Article/details/gpxczkiql.sHtML

parse_ini_file("config.ini", true)
来源：http://m.share.fehbvm.com/Article/details/gjpvuihsy.sHtML

[U74] PHP：读取环境变量
来源：http://wap.fehbvm.com/Article/details/gdzdhngjs.sHtML

getenv("APP_ENV") ?: "production"
来源：http://3g.zdbjq.cn/Article/details/gwcucdxps.sHtML

[U75] PHP：依赖注入
来源：http://mobile.zdbjq.cn/Article/details/gqjqobnlz.sHtML

composer require psr/container
来源：http://read.share.hesvh.cn/Article/details/gylkvybjf.sHtML

[U76] PHP：简单路由
来源：http://baike.zdbjq.cn/Article/details/grjyvepkl.sHtML

$path = parse_url($_SERVER["REQUEST_URI"], PHP_URL_PATH);
来源：http://mobile.hesvh.cn/Article/details/gqazakxfs.sHtML

[U77] PHP：模板渲染
来源：http://www.m.share.zdbjq.cn/Article/details/ghtxglfiq.sHtML

composer require twig/twig
来源：http://www.m.share.fehbvm.com/Article/details/gugkodtyw.sHtML

[U78] PHP：单元测试
来源：http://blog.hesvh.cn/Article/details/gwbhtqkmn.sHtML

composer require --dev phpunit/phpunit
来源：http://m.share.fehbvm.com/Article/details/gitumevnh.sHtML

[U79] PHP：静态分析
来源：http://baike.hesvh.cn/Article/details/gwtvwhqtk.sHtML

composer require --dev phpstan/phpstan
来源：http://blog.fehbvm.com/Article/details/gfoogeuah.sHtML

[U80] PHP：代码规范修复
来源：http://3g.fehbvm.com/Article/details/ghorgakhe.sHtML

composer require --dev friendsofphp/php-cs-fixer
来源：http://mobile.hesvh.cn/Article/details/gmyudlzdm.sHtML

[U81] JS：初始化项目
来源：http://www.blog.hesvh.cn/Article/details/gjsvtyaev.sHtML

npm init -y;  npm i express
来源：http://wap.zdbjq.cn/Article/details/gyjqzfuwj.sHtML

[U82] JS：package.json 脚本
来源：http://read.share.zdbjq.cn/Article/details/gqizcfyzt.sHtML

"scripts": { "dev": "vite", "build": "vite build" }
来源：http://3g.hesvh.cn/Article/details/grvmziyzx.sHtML

[U83] JS：ES Module 导入导出
来源：http://m.share.fehbvm.com/Article/details/gatgsjmrz.sHtML

export const a = 1;  import { a } from "./m.js";
来源：http://wap.hesvh.cn/Article/details/giycycysz.sHtML

[U84] JS：CommonJS 写法
来源：http://baike.fehbvm.com/Article/details/glticnfhj.sHtML

module.exports = { a };  const { a } = require("./m");
来源：http://wap.fehbvm.com/Article/details/gspwtbulh.sHtML

[U85] JS：可选链
来源：http://blog.zdbjq.cn/Article/details/gatphousm.sHtML

a?.b?.c
来源：http://read.share.zdbjq.cn/Article/details/gjzcxsslt.sHtML

[U86] JS：空值合并
来源：http://read.share.hesvh.cn/Article/details/gpcjftkdz.sHtML

a ?? b
来源：http://mobile.fehbvm.com/Article/details/gdnvvkqdl.sHtML

[U87] JS：解构默认值
来源：http://blog.fehbvm.com/Article/details/gwufgunfa.sHtML

const { a = 1, b = 2 } = obj;
来源：http://read.share.hesvh.cn/Article/details/gejxcaxym.sHtML

[U88] JS：对象展开合并
来源：http://blog.hesvh.cn/Article/details/gosvejuwg.sHtML

{ ...a, ...b }
来源：http://www.blog.hesvh.cn/Article/details/gwaasilgf.sHtML

[U89] JS：数组去重
来源：http://www.m.share.hesvh.cn/Article/details/guqzjhiqy.sHtML

[...new Set(arr)]
来源：http://3g.hesvh.cn/Article/details/ghiyanwns.sHtML

[U90] JS：数字数组排序
来源：http://blog.fehbvm.com/Article/details/gonfrczuy.sHtML

[...arr].sort((a, b) => a - b)
来源：http://m.share.hesvh.cn/Article/details/gutrctlct.sHtML

[U91] JS：对象键值遍历
来源：http://baike.fehbvm.com/Article/details/gwpackxxi.sHtML

Object.entries(obj).forEach(([k, v]) => {});
来源：http://3g.fehbvm.com/Article/details/gordniwaf.sHtML

[U92] JS：深拷贝
来源：http://3g.fehbvm.com/Article/details/grkyxxebn.sHtML

structuredClone(obj)
来源：http://mobile.hesvh.cn/Article/details/gtnjiefoc.sHtML

[U93] JS：模板字符串
来源：http://www.share.fehbvm.com/Article/details/gswudjhcj.sHtML

`共 ${n} 条`
来源：http://baike.zdbjq.cn/Article/details/gublvrbma.sHtML

[U94] JS：箭头函数
来源：http://www.blog.zdbjq.cn/Article/details/gyhapazby.sHtML

const double = x => x * 2;
来源：http://www.m.share.zdbjq.cn/Article/details/glofyjhow.sHtML

[U95] JS：Promise 包装
来源：http://baike.zdbjq.cn/Article/details/gbcabajfu.sHtML

new Promise((resolve, reject) => {})
来源：http://www.m.share.fehbvm.com/Article/details/gldhwswgq.sHtML

[U96] JS：async/await 与异常
来源：http://www.blog.zdbjq.cn/Article/details/glnkqnfmh.sHtML

try { const d = await f(); } catch (e) { console.error(e); }
来源：http://blog.fehbvm.com/Article/details/guvaeahoz.sHtML

[U97] JS：并发请求
来源：http://mobile.hesvh.cn/Article/details/gpfskrsql.sHtML

await Promise.all(urls.map(u => fetch(u)))
来源：http://www.m.share.zdbjq.cn/Article/details/gqpyzltea.sHtML

[U98] JS：fetch 带 JSON
来源：http://mobile.fehbvm.com/Article/details/gjnxgezuz.sHtML

await fetch(url, { method: "POST", headers: { "Content-Type": "application/json" }, body: JSON.stringify(d) })
来源：http://mobile.fehbvm.com/Article/details/gqmydhgjs.sHtML

[U99] JS：事件监听
来源：http://mobile.fehbvm.com/Article/details/gqxzhtksr.sHtML

el.addEventListener("click", e => {})
来源：http://www.m.share.fehbvm.com/Article/details/gbgmfopyc.sHtML

[U100] JS：DOM 查询
来源：http://baike.fehbvm.com/Article/details/gwqurmcni.sHtML

document.querySelector(".item")
来源：http://blog.fehbvm.com/Article/details/geygvvjqh.sHtML

[U101] JS：classList 操作
来源：http://m.share.fehbvm.com/Article/details/gftldmyae.sHtML

el.classList.toggle("active")
来源：http://www.share.zdbjq.cn/Article/details/glbyqnekd.sHtML

[U102] JS：本地存储
来源：http://read.share.zdbjq.cn/Article/details/gpluwiuhs.sHtML

localStorage.setItem("k", JSON.stringify(v))
来源：http://www.m.share.hesvh.cn/Article/details/gervcujrl.sHtML

[U103] JS：定时器
来源：http://www.share.zdbjq.cn/Article/details/gqjquwbao.sHtML

setTimeout(fn, 1000);  setInterval(fn, 1000);
来源：http://www.share.fehbvm.com/Article/details/gxlwodpie.sHtML

[U104] JS：防抖
来源：http://www.share.fehbvm.com/Article/details/gawniszfp.sHtML

const debounce = (fn, ms) => { let t; return (...a) => { clearTimeout(t); t = setTimeout(() => fn(...a), ms); }; };
来源：http://baike.hesvh.cn/Article/details/gdfjowyly.sHtML

[U105] JS：节流
来源：http://www.blog.fehbvm.com/Article/details/gdayzfjaa.sHtML

const throttle = (fn, ms) => { let last = 0; return (...a) => { const n = Date.now(); if (n - last >= ms) { last = n; fn(...a); } }; };
来源：http://3g.fehbvm.com/Article/details/gctpauieo.sHtML

[U106] JS：日期格式化
来源：http://mobile.hesvh.cn/Article/details/gqteorkrg.sHtML

new Intl.DateTimeFormat("zh-CN", { dateStyle: "medium" }).format(new Date())
来源：http://www.share.zdbjq.cn/Article/details/gkbbqmdiq.sHtML

[U107] JS：数字千分位
来源：http://3g.hesvh.cn/Article/details/gugbexokw.sHtML

new Intl.NumberFormat("en-US").format(1234567)
来源：http://m.share.fehbvm.com/Article/details/ggjoqmdcg.sHtML

[U108] JS：随机整数
来源：http://www.blog.hesvh.cn/Article/details/gsfgpmtug.sHtML

Math.floor(Math.random() * (max - min + 1)) + min
来源：http://www.share.fehbvm.com/Article/details/gksdxcejo.sHtML

[U109] JS：数组分组
来源：http://mobile.hesvh.cn/Article/details/gqbexkbcw.sHtML

Object.groupBy(arr, x => x.type)
来源：http://m.share.fehbvm.com/Article/details/gjehehsav.sHtML

[U110] JS：数组分块
来源：http://wap.fehbvm.com/Article/details/gitawtpij.sHtML

arr.reduce((acc, x, i) => (i % size ? acc : [...acc, arr.slice(i, i + size)]), [])
来源：http://baike.fehbvm.com/Article/details/gjuczjnus.sHtML

[U111] JS：对象转 Map
来源：http://www.m.share.fehbvm.com/Article/details/gehbfgzgy.sHtML

new Map(Object.entries(obj))
来源：http://www.share.zdbjq.cn/Article/details/grtazcjvh.sHtML

[U112] JS：字符串补位
来源：http://3g.zdbjq.cn/Article/details/glaehckrp.sHtML

"7".padStart(3, "0")
来源：http://mobile.zdbjq.cn/Article/details/glkdumtiw.sHtML

[U113] JS：正则替换全部
来源：http://read.share.fehbvm.com/Article/details/gkqjwklyp.sHtML

s.replaceAll("a", "b")
来源：http://wap.zdbjq.cn/Article/details/gqmtvovww.sHtML

[U114] JS：JSON 深比较
来源：http://wap.hesvh.cn/Article/details/gxhjvflmw.sHtML

JSON.stringify(a) === JSON.stringify(b)
来源：http://read.share.zdbjq.cn/Article/details/gbwcwrrpy.sHtML

[U115] JS：生成 UUID
来源：http://baike.zdbjq.cn/Article/details/gduluhfuz.sHtML

crypto.randomUUID()
来源：http://www.blog.hesvh.cn/Article/details/gpekoqfip.sHtML

[U116] JS：类型检查（JSDoc）
来源：http://www.blog.zdbjq.cn/Article/details/gxpnoebos.sHtML

/** @param {string} name */ function f(name) {}
来源：http://baike.hesvh.cn/Article/details/gyndyptms.sHtML

[U117] JS：单元测试
来源：http://read.share.zdbjq.cn/Article/details/gmnbuewex.sHtML

npm i -D vitest;  npx vitest
来源：http://mobile.fehbvm.com/Article/details/gllmfttak.sHtML

[U118] JS：开发服务器
来源：http://baike.hesvh.cn/Article/details/gawvguckk.sHtML

npm i -D vite;  npx vite
来源：http://wap.zdbjq.cn/Article/details/gxzkmncdj.sHtML

[U119] JS：生产构建
来源：http://3g.fehbvm.com/Article/details/gjuosmigj.sHtML

npx vite build
来源：http://read.share.zdbjq.cn/Article/details/gzugqegef.sHtML

[U120] JS：读取环境变量（Vite）
来源：http://3g.zdbjq.cn/Article/details/gtemzrcih.sHtML

import.meta.env.VITE_API_URL
来源：http://mobile.fehbvm.com/Article/details/gpfhmjbum.sHtML

================================================================================
来源：http://blog.hesvh.cn/Article/details/gwhrhzkmr.sHtML

统计汇总
来源：http://www.m.share.zdbjq.cn/Article/details/gptkdbhjr.sHtML

================================================================================
来源：http://www.m.share.hesvh.cn/Article/details/gldpnqely.sHtML

按语言统计（条）：
来源：http://3g.fehbvm.com/Article/details/gclkykvmb.sHtML

Python ......... 252
来源：http://www.share.hesvh.cn/Article/details/gcualcbhv.sHtML

PHP ............ 252
来源：http://m.share.hesvh.cn/Article/details/geuppsqth.sHtML

JavaScript ..... 252
来源：http://www.m.share.fehbvm.com/Article/details/gtpqpguzy.sHtML

TypeScript ..... 212
来源：http://baike.zdbjq.cn/Article/details/gknffhqqo.sHtML

Java ........... 212
来源：http://m.share.zdbjq.cn/Article/details/grtehniya.sHtML

Go ............. 212
来源：http://m.share.fehbvm.com/Article/details/ghguibavq.sHtML

Ruby ........... 212
来源：http://mobile.hesvh.cn/Article/details/ggygqmudp.sHtML

C# ............. 212
来源：http://www.m.share.zdbjq.cn/Article/details/gzgbeynax.sHtML

C .............. 30
来源：http://wap.hesvh.cn/Article/details/gktzymzkv.sHtML

C++ ............ 30
来源：http://www.share.fehbvm.com/Article/details/gzvdzyplm.sHtML

SQL ............ 90
来源：http://blog.fehbvm.com/Article/details/gyedgdhum.sHtML

Bash ........... 80
来源：http://www.m.share.fehbvm.com/Article/details/ganettzfy.sHtML

Kotlin ......... 15
来源：http://3g.hesvh.cn/Article/details/glkuueeah.sHtML

Swift .......... 15
来源：http://wap.hesvh.cn/Article/details/gtuyxaabh.sHtML

Lua ............ 10
来源：http://read.share.zdbjq.cn/Article/details/gahpwfsqu.sHtML

Perl ........... 10
来源：http://3g.zdbjq.cn/Article/details/gginjmjbs.sHtML

Scala .......... 10
来源：http://read.share.zdbjq.cn/Article/details/gohrfhuhk.sHtML

------------------------------------
来源：http://blog.hesvh.cn/Article/details/grulimlsc.sHtML

合计 ........... 2106 条
来源：http://wap.zdbjq.cn/Article/details/gtpbnysub.sHtML

按章节统计：
来源：http://blog.fehbvm.com/Article/details/gkhfvrrxa.sHtML

A 基础语法与类型       26 个任务 × 8 语言 =  208
来源：http://read.share.hesvh.cn/Article/details/gldcerqxt.sHtML

B 流程控制             16 个任务 × 8 语言 =  128
来源：http://www.share.fehbvm.com/Article/details/gvulnodsm.sHtML

C 函数与作用域         16 个任务 × 8 语言 =  128
来源：http://blog.fehbvm.com/Article/details/gakapfxuj.sHtML

D 数组 / 列表 / 集合   26 个任务 × 8 语言 =  208
来源：http://baike.hesvh.cn/Article/details/gpwhaxklc.sHtML

E 字符串处理           22 个任务 × 8 语言 =  176
来源：http://m.share.fehbvm.com/Article/details/gwvwmwfvj.sHtML

F 文件与目录           12 个任务 × 8 语言 =   96
来源：http://read.share.zdbjq.cn/Article/details/gzrxlscrx.sHtML

G 面向对象             16 个任务 × 8 语言 =  128
来源：http://mobile.fehbvm.com/Article/details/gvjumobab.sHtML

H 异常与错误处理       10 个任务 × 8 语言 =   80
来源：http://baike.hesvh.cn/Article/details/gogizqxli.sHtML

I 正则表达式            8 个任务 × 8 语言 =   64
来源：http://3g.fehbvm.com/Article/details/gmhuqybve.sHtML

J 日期与时间           10 个任务 × 8 语言 =   80
来源：http://wap.hesvh.cn/Article/details/gjexevqru.sHtML

K JSON 与序列化         8 个任务 × 8 语言 =   64
来源：http://3g.fehbvm.com/Article/details/glblzfkcs.sHtML

L 网络请求              8 个任务 × 8 语言 =   64
来源：http://www.blog.hesvh.cn/Article/details/gamcjvrpd.sHtML

M 命令行 / 进程         8 个任务 × 8 语言 =   64
来源：http://www.blog.zdbjq.cn/Article/details/gbbyywdez.sHtML

N 数据结构与算法       12 个任务 × 8 语言 =   96
来源：http://blog.zdbjq.cn/Article/details/gvvjallfc.sHtML

O 并发与异步            6 个任务 × 8 语言 =   48
来源：http://read.share.hesvh.cn/Article/details/gixqtoyuj.sHtML

P 常用工具函数          8 个任务 × 8 语言 =   64
来源：http://read.share.fehbvm.com/Article/details/gonjbvgrd.sHtML

Q SQL 专题                              90
来源：http://www.blog.fehbvm.com/Article/details/gufyiabta.sHtML

R Bash 专题                             80
来源：http://3g.zdbjq.cn/Article/details/gpwpqqkei.sHtML

S C / C++ 专题                          60
来源：http://mobile.zdbjq.cn/Article/details/grlivzxfp.sHtML

T 其他语言补充                          60
来源：http://wap.zdbjq.cn/Article/details/gwnexxsgo.sHtML

U 高频实用片段                         120
来源：http://mobile.zdbjq.cn/Article/details/gudaojqrt.sHtML

------------------------------------
来源：http://baike.fehbvm.com/Article/details/gwydihqyp.sHtML

合计                                  2106 条
来源：http://m.share.hesvh.cn/Article/details/gmxjxeili.sHtML

--------------------------------------------------------------------------------
来源：http://3g.zdbjq.cn/Article/details/gdakofgmd.sHtML

使用提醒
来源：http://baike.zdbjq.cn/Article/details/gopkbgoib.sHtML

--------------------------------------------------------------------------------
来源：http://www.share.hesvh.cn/Article/details/gleympkzx.sHtML

1. 示例追求"最小可用"，正式项目中请补齐导入、错误处理与边界判断。
来源：http://3g.fehbvm.com/Article/details/gliugcrth.sHtML

2. 涉及文件、网络、数据库的示例，注意资源释放与异常捕获。
来源：http://read.share.hesvh.cn/Article/details/gnbqkwafh.sHtML

3. 语言版本差异较大（如 Python 3.10 的 match、Java 17 的 record/switch 箭头），
来源：http://3g.hesvh.cn/Article/details/gultixezr.sHtML

在旧版本上使用前请先确认语法支持情况。
来源：http://www.share.hesvh.cn/Article/details/ggaajnveb.sHtML

4. 标注"手写"的条目是因为该语言缺少对应内置能力，实际项目中可引入成熟库。
来源：http://m.share.zdbjq.cn/Article/details/gxxiwanlo.sHtML

—— 文件结束 ——
来源：http://wap.zdbjq.cn/Article/details/gdmqhkujd.sHtML

================================================================================
来源：http://mobile.fehbvm.com/Article/details/gpupfjiel.sHtML

程序语言常见例子速查手册（2024 版）
来源：http://3g.zdbjq.cn/Article/details/ghvahuvtj.sHtML

Common Programming Examples Cheat Book
来源：http://read.share.hesvh.cn/Article/details/gyfxconal.sHtML

================================================================================
来源：http://wap.hesvh.cn/Article/details/gyvigxrvp.sHtML

【收录内容】
来源：http://blog.hesvh.cn/Article/details/gedsnurxp.sHtML

覆盖 12 种语言 / 语法与常见 API：
来源：http://blog.zdbjq.cn/Article/details/gzycbevnz.sHtML

Python · PHP · JavaScript · TypeScript · Java · Go · Ruby · C#
来源：http://www.blog.zdbjq.cn/Article/details/gvyszmywf.sHtML

SQL · Bash · C · C++
来源：http://baike.hesvh.cn/Article/details/gktplyckp.sHtML

按「任务」分组：每个任务下按语言各给出一条最小可用示例。
来源：http://wap.fehbvm.com/Article/details/gtirvkmcn.sHtML

【使用说明】
来源：http://www.blog.hesvh.cn/Article/details/gciqmycpr.sHtML

1. 每个任务形如 "[编号] 任务名"，下面每行以语言标记开头：
来源：http://www.share.fehbvm.com/Article/details/gelnguebl.sHtML

Py:    Python        PHP:   PHP           JS:    JavaScript
来源：http://3g.hesvh.cn/Article/details/galvnbdap.sHtML

TS:    TypeScript    Java:  Java          Go:    Go
来源：http://wap.hesvh.cn/Article/details/ggziyvzuf.sHtML

Ruby:  Ruby          C#:    C#            SQL:   SQL
来源：http://3g.fehbvm.com/Article/details/ghfuzsgmi.sHtML

Bash:  Shell         C:     C             C++:   C++
来源：http://3g.hesvh.cn/Article/details/gglhirlhk.sHtML

2. 示例只展示核心写法，刻意省略 import / require / include / using 等样板代码。
来源：http://m.share.hesvh.cn/Article/details/ghfbcqroe.sHtML

需要完整可运行文件时，请自行补齐当前语言的导入语句。
来源：http://mobile.zdbjq.cn/Article/details/gurhxnbdc.sHtML

3. 语法基准：Python 3.10+ / PHP 8.1+ / ES2020+ / TypeScript 5 / Java 17 /
来源：http://3g.fehbvm.com/Article/details/gjkylwyhb.sHtML

Go 1.21+ / Ruby 3.x / C# 10+ / C17 / C++17。
来源：http://www.m.share.zdbjq.cn/Article/details/gmleeeqzq.sHtML

4. 检索建议：用编辑器或浏览器 Ctrl+F 搜关键词，如 "排序" "读取文件" "正则"。
来源：http://baike.hesvh.cn/Article/details/gfginmbyp.sHtML

5. 标记为 "// 无" 表示该语言没有对应的一等语法，需用替代写法（示例给出替代方案）。
来源：http://blog.zdbjq.cn/Article/details/gmcebhkcy.sHtML

6. 符号 "⏎" 表示代码在此处换行（主要用于 Python 等强制缩进、无法压成一行的结构）。
来源：http://www.m.share.fehbvm.com/Article/details/gzaihebgi.sHtML

【文件统计】
来源：http://3g.zdbjq.cn/Article/details/gpmefzqxv.sHtML

语言示例共 2106 条，分布见本文末尾的「统计汇总」。
来源：http://read.share.fehbvm.com/Article/details/gwdsexuzi.sHtML

--------------------------------------------------------------------------------
来源：http://wap.fehbvm.com/Article/details/gxtvmurns.sHtML

目  录
来源：http://www.m.share.hesvh.cn/Article/details/gdjfjxlhz.sHtML

--------------------------------------------------------------------------------
来源：http://www.m.share.hesvh.cn/Article/details/gohhykzgu.sHtML

A. 基础语法与类型              （第 1 节，26 个任务，208 条）
来源：http://3g.fehbvm.com/Article/details/gnbgriyym.sHtML

B. 流程控制                    （第 2 节，16 个任务，128 条）
来源：http://www.blog.zdbjq.cn/Article/details/goxlvmzqc.sHtML

C. 函数与作用域                （第 3 节，16 个任务，128 条）
来源：http://wap.hesvh.cn/Article/details/getnmxcys.sHtML

D. 数组 / 列表 / 集合          （第 4 节，26 个任务，208 条）
来源：http://blog.hesvh.cn/Article/details/gnzydxmgh.sHtML

E. 字符串处理                  （第 5 节，22 个任务，176 条）
来源：http://3g.fehbvm.com/Article/details/gsoehwvxr.sHtML

F. 文件与目录                  （第 6 节，12 个任务，96 条）
来源：http://baike.fehbvm.com/Article/details/gxkyglgsh.sHtML

G. 面向对象                    （第 7 节，16 个任务，128 条）
来源：http://read.share.fehbvm.com/Article/details/ggijdjeyi.sHtML

H. 异常与错误处理              （第 8 节，10 个任务，80 条）
来源：http://m.share.zdbjq.cn/Article/details/giugeyycb.sHtML

I. 正则表达式                  （第 9 节，8 个任务，64 条）
来源：http://www.share.fehbvm.com/Article/details/gjgorahvq.sHtML

J. 日期与时间                  （第 10 节，10 个任务，80 条）
来源：http://3g.fehbvm.com/Article/details/gppsimasv.sHtML

K. JSON 与序列化               （第 11 节，8 个任务，64 条）
来源：http://mobile.fehbvm.com/Article/details/gvrtrpvwa.sHtML

L. 网络请求                    （第 12 节，8 个任务，64 条）
来源：http://www.blog.hesvh.cn/Article/details/ghwimmqdw.sHtML

M. 命令行 / 进程 / 环境        （第 13 节，8 个任务，64 条）
来源：http://mobile.zdbjq.cn/Article/details/gnvrpfjhj.sHtML

N. 数据结构与算法              （第 14 节，12 个任务，96 条）
来源：http://www.blog.fehbvm.com/Article/details/gtjvcyxbb.sHtML

O. 并发与异步                  （第 15 节，6 个任务，48 条）
来源：http://www.m.share.zdbjq.cn/Article/details/gpxrnzzky.sHtML

P. 常用工具函数                （第 16 节，8 个任务，64 条）
来源：http://3g.fehbvm.com/Article/details/gmygfvgos.sHtML

Q. SQL 专题                    （第 17 节，90 条）
来源：http://read.share.zdbjq.cn/Article/details/geyjggfpv.sHtML

R. Bash 专题                   （第 18 节，80 条）
来源：http://blog.fehbvm.com/Article/details/gbdhaekga.sHtML

S. C / C++ 专题                （第 19 节，60 条）
来源：http://www.m.share.fehbvm.com/Article/details/gugtkxpcf.sHtML

T. 其他语言补充                （第 20 节，60 条：Kotlin / Swift / Lua / Perl / Scala）
来源：http://wap.fehbvm.com/Article/details/gncpicrht.sHtML

U. 高频实用片段                （第 21 节，120 条：Python / PHP / JavaScript 各 40 条）
来源：http://read.share.zdbjq.cn/Article/details/gqldjxlee.sHtML

================================================================================
来源：http://blog.fehbvm.com/Article/details/gggokhdde.sHtML

A. 基础语法与类型
来源：http://www.share.zdbjq.cn/Article/details/gsmcjewof.sHtML

================================================================================
来源：http://read.share.zdbjq.cn/Article/details/gxicmfwwz.sHtML

[A01] Hello World
来源：http://3g.fehbvm.com/Article/details/gqmisqseq.sHtML

Py:   print("Hello, World!")
来源：http://www.share.zdbjq.cn/Article/details/gsrpaprka.sHtML

PHP:  echo "Hello, World!";
来源：http://m.share.fehbvm.com/Article/details/ghzgkbnuo.sHtML

JS:   console.log("Hello, World!");
来源：http://wap.hesvh.cn/Article/details/gkmqvdkyp.sHtML

TS:   const msg: string = "Hello, World!"; console.log(msg);
来源：http://baike.zdbjq.cn/Article/details/gwzyjicpc.sHtML

Java: System.out.println("Hello, World!");
来源：http://wap.zdbjq.cn/Article/details/gwysvqwxy.sHtML

Go:   fmt.Println("Hello, World!")
来源：http://3g.hesvh.cn/Article/details/gaepglpqb.sHtML

Ruby: puts "Hello, World!"
来源：http://blog.hesvh.cn/Article/details/gnqiamies.sHtML

C#:   Console.WriteLine("Hello, World!");
来源：http://3g.hesvh.cn/Article/details/gdxfabgbl.sHtML

[A02] 变量声明与赋值
来源：http://m.share.fehbvm.com/Article/details/gbourvxxo.sHtML

Py:   name = "Alex"; age = 20            # 动态类型，无需声明
来源：http://blog.hesvh.cn/Article/details/gurwlnils.sHtML

PHP:  $name = "Alex"; $age = 20;
来源：http://www.m.share.zdbjq.cn/Article/details/glspaugct.sHtML

JS:   let name = "Alex"; const age = 20;
来源：http://3g.zdbjq.cn/Article/details/gnvjiralx.sHtML


<!-- 参考信息 -->