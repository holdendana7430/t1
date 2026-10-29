代发 wailian999

[U31] Py：单测
来源：http://m.share.hesvh.cn/Article/details/gkmzwiyiz.sHtML

python -m pytest -q
来源：http://baike.fehbvm.com/Article/details/gwbgyzctm.sHtML

[U32] Py：代码格式化
来源：http://3g.zdbjq.cn/Article/details/glfcncmfc.sHtML

ruff format . && ruff check --fix .
来源：http://www.share.fehbvm.com/Article/details/golqyhxqx.sHtML

[U33] Py：打包发布
来源：http://3g.zdbjq.cn/Article/details/gowatcngh.sHtML

python -m build  （依赖 pyproject.toml）
来源：http://3g.hesvh.cn/Article/details/gfbhdpfhd.sHtML

[U34] Py：判断编码
来源：http://baike.zdbjq.cn/Article/details/gqnsuxzyo.sHtML

chardet.detect(raw)
来源：http://m.share.hesvh.cn/Article/details/gizarebix.sHtML

[U35] Py：发送邮件
来源：http://www.blog.hesvh.cn/Article/details/gasdhpcap.sHtML

smtplib.SMTP_SSL(...).send_message(msg)
来源：http://wap.fehbvm.com/Article/details/grwasukcl.sHtML

[U36] Py：定时任务
来源：http://blog.zdbjq.cn/Article/details/gdirgzfwb.sHtML

schedule.every(10).minutes.do(job)
来源：http://3g.hesvh.cn/Article/details/ggygklena.sHtML

[U37] Py：读写 Excel
来源：http://www.blog.fehbvm.com/Article/details/gprvabrax.sHtML

pandas.read_excel / DataFrame.to_excel
来源：http://baike.zdbjq.cn/Article/details/grxwsfqkg.sHtML

[U38] Py：获取脚本所在目录
来源：http://read.share.fehbvm.com/Article/details/gxhiqgpbh.sHtML

Path(__file__).resolve().parent
来源：http://baike.zdbjq.cn/Article/details/gqmijgaif.sHtML

[U39] Py：判断是否在交互环境
来源：http://www.blog.hesvh.cn/Article/details/gjoqakyho.sHtML

sys.stdout.isatty()
来源：http://www.blog.hesvh.cn/Article/details/gxofcfnrt.sHtML

[U40] Py：打印到标准错误
来源：http://m.share.fehbvm.com/Article/details/glwhciyvl.sHtML

print("err", file=sys.stderr)
来源：http://baike.zdbjq.cn/Article/details/grclzruad.sHtML

[U41] PHP：初始化 Composer 项目
来源：http://blog.zdbjq.cn/Article/details/gxmyqjhqg.sHtML

composer init;  composer require guzzlehttp/guzzle
来源：http://wap.hesvh.cn/Article/details/ghpkpcpri.sHtML

[U42] PHP：PSR-4 自动加载
来源：http://m.share.fehbvm.com/Article/details/gyaurglie.sHtML

"autoload": { "psr-4": { "App\\": "src/" } }
来源：http://wap.zdbjq.cn/Article/details/gnnviryej.sHtML

[U43] PHP：声明命名空间
来源：http://www.m.share.hesvh.cn/Article/details/goewxxirn.sHtML

namespace App\Http;
来源：http://mobile.zdbjq.cn/Article/details/gmhrvschk.sHtML

[U44] PHP：开启严格类型
来源：http://www.blog.zdbjq.cn/Article/details/gjdmpkkpv.sHtML

declare(strict_types=1);
来源：http://wap.fehbvm.com/Article/details/gnhzowlwg.sHtML

[U45] PHP：类型声明与返回类型
来源：http://m.share.hesvh.cn/Article/details/guiqghgcw.sHtML

function add(int $a, int $b): int { return $a + $b; }
来源：http://3g.hesvh.cn/Article/details/gyntixyty.sHtML

[U46] PHP：可空类型
来源：http://www.m.share.hesvh.cn/Article/details/ghzswpmxl.sHtML

?string $name = null
来源：http://www.blog.zdbjq.cn/Article/details/gsrztokia.sHtML

[U47] PHP：联合类型
来源：http://mobile.fehbvm.com/Article/details/gynuusaaa.sHtML

int|string $id
来源：http://wap.zdbjq.cn/Article/details/gcochbagp.sHtML

[U48] PHP：纯枚举
来源：http://www.m.share.zdbjq.cn/Article/details/gzemcgjri.sHtML

enum Status: string { case Active = "active"; case Off = "off"; }
来源：http://www.m.share.hesvh.cn/Article/details/gjqytziak.sHtML

[U49] PHP：只读属性
来源：http://mobile.zdbjq.cn/Article/details/gczmsskkr.sHtML

public readonly string $name
来源：http://wap.fehbvm.com/Article/details/gudhcnnpe.sHtML

[U50] PHP：构造器属性提升
来源：http://blog.fehbvm.com/Article/details/gsijprzjh.sHtML

public function __construct(private int $id) {}
来源：http://read.share.fehbvm.com/Article/details/glogqiisy.sHtML

[U51] PHP：数组解构
来源：http://mobile.hesvh.cn/Article/details/gutmxxuut.sHtML

[$a, $b] = $arr;
来源：http://wap.fehbvm.com/Article/details/grqnijuux.sHtML

[U52] PHP：箭头函数
来源：http://blog.zdbjq.cn/Article/details/gmorfnkag.sHtML

$double = fn($x) => $x * 2;
来源：http://blog.zdbjq.cn/Article/details/gjozklgbi.sHtML

[U53] PHP：空合并运算符
来源：http://www.m.share.fehbvm.com/Article/details/gfbpsisxm.sHtML

$v = $a ?? $b ?? "default";
来源：http://www.share.zdbjq.cn/Article/details/gkzdwrbdd.sHtML

[U54] PHP：空安全调用
来源：http://www.share.zdbjq.cn/Article/details/gfqukyjkh.sHtML

$obj?->method()
来源：http://www.blog.fehbvm.com/Article/details/grxocjzuq.sHtML

[U55] PHP：match 表达式
来源：http://www.m.share.zdbjq.cn/Article/details/gicnohmkh.sHtML

$s = match($x) { 1 => "一", default => "其他" };
来源：http://m.share.zdbjq.cn/Article/details/givdfjvrr.sHtML

[U56] PHP：命名参数
来源：http://3g.zdbjq.cn/Article/details/gmykrmivf.sHtML

f(a: 1, b: 2)
来源：http://read.share.zdbjq.cn/Article/details/gtmjkrkkj.sHtML

[U57] PHP：字符串插值
来源：http://wap.fehbvm.com/Article/details/gcmjlqhrp.sHtML

"值: {$a}"
来源：http://read.share.zdbjq.cn/Article/details/gpoctusou.sHtML

[U58] PHP：数组三件套
来源：http://m.share.zdbjq.cn/Article/details/gexviiekd.sHtML

array_map($f, $a);  array_filter($a, $f);  array_reduce($a, $f, 0);
来源：http://www.share.hesvh.cn/Article/details/gfsxqvtub.sHtML

[U59] PHP：自定义排序
来源：http://3g.zdbjq.cn/Article/details/gzmmzvvvq.sHtML

usort($arr, fn($a, $b) => $a["age"] <=> $b["age"]);
来源：http://wap.zdbjq.cn/Article/details/gdfoqhovn.sHtML

[U60] PHP：JSON 编解码
来源：http://3g.zdbjq.cn/Article/details/gvcqufsju.sHtML

json_encode($d, JSON_UNESCAPED_UNICODE);  json_decode($s, true);
来源：http://mobile.hesvh.cn/Article/details/gldiqydud.sHtML

[U61] PHP：正则
来源：http://m.share.fehbvm.com/Article/details/gzdskvvqp.sHtML

preg_match('/(\d+)/', $s, $m);  preg_replace('/\d+/', '#', $s);
来源：http://mobile.fehbvm.com/Article/details/gtohhuoiu.sHtML

[U62] PHP：日期对象
来源：http://wap.zdbjq.cn/Article/details/gcbpnpnux.sHtML

(new DateTimeImmutable())->format("Y-m-d");
来源：http://wap.fehbvm.com/Article/details/grrekitfd.sHtML

[U63] PHP：文件读写
来源：http://wap.hesvh.cn/Article/details/gcehwwkfm.sHtML

file_get_contents($f);  file_put_contents($f, $data);
来源：http://wap.fehbvm.com/Article/details/gylmctqna.sHtML

[U64] PHP：目录遍历
来源：http://blog.zdbjq.cn/Article/details/gpjcxzyoo.sHtML

glob("dir/*.php");  scandir("dir");
来源：http://read.share.fehbvm.com/Article/details/gmypdezjg.sHtML

[U65] PHP：会话
来源：http://www.share.zdbjq.cn/Article/details/gocuhppcw.sHtML

session_start();  $_SESSION["uid"] = 1;
来源：http://read.share.hesvh.cn/Article/details/gztvijkpo.sHtML

[U66] PHP：设置 Cookie
来源：http://m.share.hesvh.cn/Article/details/gtzpckskd.sHtML

setcookie("token", $v, ["httponly" => true, "samesite" => "Lax"]);
来源：http://3g.fehbvm.com/Article/details/gsahvrofn.sHtML

[U67] PHP：处理文件上传
来源：http://3g.zdbjq.cn/Article/details/gcohdgbfg.sHtML

$_FILES["file"]["tmp_name"] 与 move_uploaded_file()
来源：http://m.share.zdbjq.cn/Article/details/gwrqwletu.sHtML

[U68] PHP：PDO 连接
来源：http://baike.fehbvm.com/Article/details/gyajvpckn.sHtML

$pdo = new PDO("mysql:host=localhost;dbname=app", "root", "");
来源：http://blog.fehbvm.com/Article/details/gxrrjhqik.sHtML

[U69] PHP：PDO 预处理
来源：http://www.share.fehbvm.com/Article/details/gugkgayxt.sHtML

$stmt = $pdo->prepare("SELECT * FROM users WHERE id = ?");  $stmt->execute([$id]);
来源：http://read.share.hesvh.cn/Article/details/gzslpisrw.sHtML

[U70] PHP：PDO 事务
来源：http://www.blog.hesvh.cn/Article/details/gcnlhjmgd.sHtML

$pdo->beginTransaction();  $pdo->commit();  $pdo->rollBack();
来源：http://mobile.fehbvm.com/Article/details/gonvqdsgd.sHtML

[U71] PHP：抛出异常
来源：http://www.m.share.zdbjq.cn/Article/details/gtldsluas.sHtML

throw new RuntimeException("失败", 500);
来源：http://baike.zdbjq.cn/Article/details/gjvesumce.sHtML

[U72] PHP：写错误日志
来源：http://blog.zdbjq.cn/Article/details/glpijxigk.sHtML

error_log("失败: " . $e->getMessage());
来源：http://mobile.fehbvm.com/Article/details/gssjswoqh.sHtML

[U73] PHP：读取 ini 配置
来源：http://www.blog.hesvh.cn/Article/details/gmnetxjwr.sHtML

parse_ini_file("config.ini", true)
来源：http://wap.zdbjq.cn/Article/details/gsnxhktau.sHtML

[U74] PHP：读取环境变量
来源：http://3g.fehbvm.com/Article/details/gsbbsujpr.sHtML

getenv("APP_ENV") ?: "production"
来源：http://3g.hesvh.cn/Article/details/gmmifvnaw.sHtML

[U75] PHP：依赖注入
来源：http://wap.hesvh.cn/Article/details/gewreoyum.sHtML

composer require psr/container
来源：http://baike.hesvh.cn/Article/details/gohnwkigy.sHtML

[U76] PHP：简单路由
来源：http://blog.zdbjq.cn/Article/details/grwnyfpfi.sHtML

$path = parse_url($_SERVER["REQUEST_URI"], PHP_URL_PATH);
来源：http://wap.fehbvm.com/Article/details/gqcnaroag.sHtML

[U77] PHP：模板渲染
来源：http://wap.fehbvm.com/Article/details/gnygcmnur.sHtML

composer require twig/twig
来源：http://www.share.hesvh.cn/Article/details/goyoovwym.sHtML

[U78] PHP：单元测试
来源：http://wap.hesvh.cn/Article/details/ggqblwyms.sHtML

composer require --dev phpunit/phpunit
来源：http://mobile.hesvh.cn/Article/details/gqsoomeui.sHtML

[U79] PHP：静态分析
来源：http://read.share.zdbjq.cn/Article/details/gssehtxzp.sHtML

composer require --dev phpstan/phpstan
来源：http://www.m.share.zdbjq.cn/Article/details/gxolshywk.sHtML

[U80] PHP：代码规范修复
来源：http://wap.fehbvm.com/Article/details/ghmmlyimd.sHtML

composer require --dev friendsofphp/php-cs-fixer
来源：http://read.share.zdbjq.cn/Article/details/gyfdponns.sHtML

[U81] JS：初始化项目
来源：http://3g.zdbjq.cn/Article/details/gnxasxkbs.sHtML

npm init -y;  npm i express
来源：http://wap.hesvh.cn/Article/details/gszswwbzf.sHtML

[U82] JS：package.json 脚本
来源：http://www.m.share.zdbjq.cn/Article/details/gdwisdmyr.sHtML

"scripts": { "dev": "vite", "build": "vite build" }
来源：http://3g.fehbvm.com/Article/details/gmptzzxrz.sHtML

[U83] JS：ES Module 导入导出
来源：http://www.share.hesvh.cn/Article/details/gjnkifcdd.sHtML

export const a = 1;  import { a } from "./m.js";
来源：http://www.share.zdbjq.cn/Article/details/gvuueglsy.sHtML

[U84] JS：CommonJS 写法
来源：http://3g.fehbvm.com/Article/details/gmiydnlte.sHtML

module.exports = { a };  const { a } = require("./m");
来源：http://blog.hesvh.cn/Article/details/gbxsfgqui.sHtML

[U85] JS：可选链
来源：http://baike.hesvh.cn/Article/details/gkqvghyjv.sHtML

a?.b?.c
来源：http://www.m.share.zdbjq.cn/Article/details/gkhhmjink.sHtML

[U86] JS：空值合并
来源：http://mobile.fehbvm.com/Article/details/gmndexswr.sHtML

a ?? b
来源：http://wap.fehbvm.com/Article/details/guyqhgrjp.sHtML

[U87] JS：解构默认值
来源：http://blog.zdbjq.cn/Article/details/gsugiqrmd.sHtML

const { a = 1, b = 2 } = obj;
来源：http://read.share.hesvh.cn/Article/details/ggklrnedo.sHtML

[U88] JS：对象展开合并
来源：http://mobile.fehbvm.com/Article/details/gsfgvvwcf.sHtML

{ ...a, ...b }
来源：http://www.m.share.fehbvm.com/Article/details/garprnqul.sHtML

[U89] JS：数组去重
来源：http://blog.fehbvm.com/Article/details/gayfbtexm.sHtML

[...new Set(arr)]
来源：http://www.m.share.fehbvm.com/Article/details/gqwkjmcpv.sHtML

[U90] JS：数字数组排序
来源：http://blog.zdbjq.cn/Article/details/gvriymiyr.sHtML

[...arr].sort((a, b) => a - b)
来源：http://mobile.zdbjq.cn/Article/details/gdtddppsx.sHtML

[U91] JS：对象键值遍历
来源：http://blog.hesvh.cn/Article/details/gfgafrkct.sHtML

Object.entries(obj).forEach(([k, v]) => {});
来源：http://www.blog.zdbjq.cn/Article/details/gtvkqezui.sHtML

[U92] JS：深拷贝
来源：http://m.share.fehbvm.com/Article/details/giwwrmjyq.sHtML

structuredClone(obj)
来源：http://blog.zdbjq.cn/Article/details/gvtkphgux.sHtML

[U93] JS：模板字符串
来源：http://www.blog.hesvh.cn/Article/details/gjiviccyg.sHtML

`共 ${n} 条`
来源：http://3g.hesvh.cn/Article/details/gxxghygmw.sHtML

[U94] JS：箭头函数
来源：http://3g.hesvh.cn/Article/details/gfivnpphc.sHtML

const double = x => x * 2;
来源：http://m.share.fehbvm.com/Article/details/gyukfakjv.sHtML

[U95] JS：Promise 包装
来源：http://m.share.zdbjq.cn/Article/details/gtclduies.sHtML

new Promise((resolve, reject) => {})
来源：http://3g.hesvh.cn/Article/details/ghdohupyg.sHtML

[U96] JS：async/await 与异常
来源：http://www.blog.zdbjq.cn/Article/details/ggwxkznxf.sHtML

try { const d = await f(); } catch (e) { console.error(e); }
来源：http://mobile.fehbvm.com/Article/details/gtdozzrqs.sHtML

[U97] JS：并发请求
来源：http://read.share.zdbjq.cn/Article/details/gtmdijzol.sHtML

await Promise.all(urls.map(u => fetch(u)))
来源：http://wap.zdbjq.cn/Article/details/gxivcwgrr.sHtML

[U98] JS：fetch 带 JSON
来源：http://wap.zdbjq.cn/Article/details/gssqapzdf.sHtML

await fetch(url, { method: "POST", headers: { "Content-Type": "application/json" }, body: JSON.stringify(d) })
来源：http://baike.hesvh.cn/Article/details/gqrmmeyre.sHtML

[U99] JS：事件监听
来源：http://blog.zdbjq.cn/Article/details/gsgmugqjx.sHtML

el.addEventListener("click", e => {})
来源：http://3g.fehbvm.com/Article/details/gishmwpik.sHtML

[U100] JS：DOM 查询
来源：http://baike.zdbjq.cn/Article/details/gseabahug.sHtML

document.querySelector(".item")
来源：http://read.share.hesvh.cn/Article/details/gbbowrrmz.sHtML

[U101] JS：classList 操作
来源：http://blog.zdbjq.cn/Article/details/gpspytfvd.sHtML

el.classList.toggle("active")
来源：http://read.share.fehbvm.com/Article/details/gpwvhpoib.sHtML

[U102] JS：本地存储
来源：http://www.m.share.hesvh.cn/Article/details/gggwzrlcf.sHtML

localStorage.setItem("k", JSON.stringify(v))
来源：http://wap.hesvh.cn/Article/details/gohuegflt.sHtML

[U103] JS：定时器
来源：http://mobile.hesvh.cn/Article/details/gybhjmeel.sHtML

setTimeout(fn, 1000);  setInterval(fn, 1000);
来源：http://3g.fehbvm.com/Article/details/grobvudvw.sHtML

[U104] JS：防抖
来源：http://www.share.fehbvm.com/Article/details/gtpkgrnsy.sHtML

const debounce = (fn, ms) => { let t; return (...a) => { clearTimeout(t); t = setTimeout(() => fn(...a), ms); }; };
来源：http://m.share.fehbvm.com/Article/details/ggqyupddr.sHtML

[U105] JS：节流
来源：http://read.share.zdbjq.cn/Article/details/gblgiipsv.sHtML

const throttle = (fn, ms) => { let last = 0; return (...a) => { const n = Date.now(); if (n - last >= ms) { last = n; fn(...a); } }; };
来源：http://www.share.fehbvm.com/Article/details/gmwhbktft.sHtML

[U106] JS：日期格式化
来源：http://www.m.share.zdbjq.cn/Article/details/gbymlaxgd.sHtML

new Intl.DateTimeFormat("zh-CN", { dateStyle: "medium" }).format(new Date())
来源：http://mobile.hesvh.cn/Article/details/gkatmwxdz.sHtML

[U107] JS：数字千分位
来源：http://wap.zdbjq.cn/Article/details/gvrxcmtwq.sHtML

new Intl.NumberFormat("en-US").format(1234567)
来源：http://m.share.hesvh.cn/Article/details/gusiiwowk.sHtML

[U108] JS：随机整数
来源：http://baike.fehbvm.com/Article/details/gvpnjbpfn.sHtML

Math.floor(Math.random() * (max - min + 1)) + min
来源：http://www.blog.hesvh.cn/Article/details/goitgwmfx.sHtML

[U109] JS：数组分组
来源：http://www.share.zdbjq.cn/Article/details/gtfraooyl.sHtML

Object.groupBy(arr, x => x.type)
来源：http://m.share.hesvh.cn/Article/details/gggikkypk.sHtML

[U110] JS：数组分块
来源：http://www.m.share.hesvh.cn/Article/details/gsykfssbe.sHtML

arr.reduce((acc, x, i) => (i % size ? acc : [...acc, arr.slice(i, i + size)]), [])
来源：http://www.blog.fehbvm.com/Article/details/gcgkpgsll.sHtML

[U111] JS：对象转 Map
来源：http://m.share.zdbjq.cn/Article/details/gnalvglzd.sHtML

new Map(Object.entries(obj))
来源：http://mobile.zdbjq.cn/Article/details/glyqmouuy.sHtML

[U112] JS：字符串补位
来源：http://baike.fehbvm.com/Article/details/glgseduul.sHtML

"7".padStart(3, "0")
来源：http://m.share.fehbvm.com/Article/details/gnuqkxtvo.sHtML

[U113] JS：正则替换全部
来源：http://m.share.fehbvm.com/Article/details/guwuxqvgt.sHtML

s.replaceAll("a", "b")
来源：http://3g.hesvh.cn/Article/details/ghdrxejkq.sHtML

[U114] JS：JSON 深比较
来源：http://wap.fehbvm.com/Article/details/gnacrpiem.sHtML

JSON.stringify(a) === JSON.stringify(b)
来源：http://www.m.share.hesvh.cn/Article/details/gymtzcymx.sHtML

[U115] JS：生成 UUID
来源：http://mobile.zdbjq.cn/Article/details/gsveprbps.sHtML

crypto.randomUUID()
来源：http://www.blog.hesvh.cn/Article/details/gkuncoryf.sHtML

[U116] JS：类型检查（JSDoc）
来源：http://wap.fehbvm.com/Article/details/gaokmrkdp.sHtML

/** @param {string} name */ function f(name) {}
来源：http://read.share.zdbjq.cn/Article/details/grakkslan.sHtML

[U117] JS：单元测试
来源：http://3g.fehbvm.com/Article/details/gfncnefix.sHtML

npm i -D vitest;  npx vitest
来源：http://www.m.share.hesvh.cn/Article/details/goqmqjlae.sHtML

[U118] JS：开发服务器
来源：http://blog.fehbvm.com/Article/details/gzilxbuxz.sHtML

npm i -D vite;  npx vite
来源：http://read.share.hesvh.cn/Article/details/ggvhsuqdx.sHtML

[U119] JS：生产构建
来源：http://baike.fehbvm.com/Article/details/giatfzzgy.sHtML

npx vite build
来源：http://www.m.share.hesvh.cn/Article/details/gimodeogg.sHtML

[U120] JS：读取环境变量（Vite）
来源：http://baike.hesvh.cn/Article/details/gjzmapdwd.sHtML

import.meta.env.VITE_API_URL
来源：http://m.share.fehbvm.com/Article/details/gmykkqspb.sHtML

================================================================================
来源：http://www.m.share.hesvh.cn/Article/details/gvpkhnluy.sHtML

统计汇总
来源：http://3g.fehbvm.com/Article/details/gqlxfrrek.sHtML

================================================================================
来源：http://m.share.hesvh.cn/Article/details/gigwiitse.sHtML

按语言统计（条）：
来源：http://www.blog.hesvh.cn/Article/details/gpoebmdpt.sHtML

Python ......... 252
来源：http://read.share.hesvh.cn/Article/details/gqlpoebhh.sHtML

PHP ............ 252
来源：http://read.share.fehbvm.com/Article/details/gsidflcpn.sHtML

JavaScript ..... 252
来源：http://blog.fehbvm.com/Article/details/glwtpzvlf.sHtML

TypeScript ..... 212
来源：http://www.share.hesvh.cn/Article/details/gydrppkpr.sHtML

Java ........... 212
来源：http://3g.fehbvm.com/Article/details/gtsobwdhy.sHtML

Go ............. 212
来源：http://3g.zdbjq.cn/Article/details/ggwoxfixp.sHtML

Ruby ........... 212
来源：http://wap.fehbvm.com/Article/details/gsecqkghx.sHtML

C# ............. 212
来源：http://www.blog.fehbvm.com/Article/details/gctdsyitu.sHtML

C .............. 30
来源：http://blog.fehbvm.com/Article/details/gishcxcqa.sHtML

C++ ............ 30
来源：http://wap.fehbvm.com/Article/details/gdblmhmrv.sHtML

SQL ............ 90
来源：http://www.blog.zdbjq.cn/Article/details/gctedqcgg.sHtML

Bash ........... 80
来源：http://blog.fehbvm.com/Article/details/gwwhazclo.sHtML

Kotlin ......... 15
来源：http://www.m.share.zdbjq.cn/Article/details/ghzkemrxu.sHtML

Swift .......... 15
来源：http://mobile.hesvh.cn/Article/details/gkatkbboo.sHtML

Lua ............ 10
来源：http://mobile.hesvh.cn/Article/details/gdeiggidr.sHtML

Perl ........... 10
来源：http://www.share.hesvh.cn/Article/details/gakmweqka.sHtML

Scala .......... 10
来源：http://read.share.hesvh.cn/Article/details/gsieygist.sHtML

------------------------------------
来源：http://wap.hesvh.cn/Article/details/gfqrftutz.sHtML

合计 ........... 2106 条
来源：http://baike.hesvh.cn/Article/details/gdxvsazub.sHtML

按章节统计：
来源：http://3g.fehbvm.com/Article/details/godtnfvvp.sHtML

A 基础语法与类型       26 个任务 × 8 语言 =  208
来源：http://m.share.fehbvm.com/Article/details/gbrufapcy.sHtML

B 流程控制             16 个任务 × 8 语言 =  128
来源：http://wap.hesvh.cn/Article/details/gaekldigl.sHtML

C 函数与作用域         16 个任务 × 8 语言 =  128
来源：http://mobile.zdbjq.cn/Article/details/gxbchafiz.sHtML

D 数组 / 列表 / 集合   26 个任务 × 8 语言 =  208
来源：http://www.share.zdbjq.cn/Article/details/glzuvyqyo.sHtML

E 字符串处理           22 个任务 × 8 语言 =  176
来源：http://wap.fehbvm.com/Article/details/gogvbporj.sHtML

F 文件与目录           12 个任务 × 8 语言 =   96
来源：http://blog.hesvh.cn/Article/details/gfkkocqmx.sHtML

G 面向对象             16 个任务 × 8 语言 =  128
来源：http://read.share.hesvh.cn/Article/details/gyymdwdux.sHtML

H 异常与错误处理       10 个任务 × 8 语言 =   80
来源：http://wap.fehbvm.com/Article/details/gyldmuhxa.sHtML

I 正则表达式            8 个任务 × 8 语言 =   64
来源：http://www.blog.zdbjq.cn/Article/details/gszkrsdwz.sHtML

J 日期与时间           10 个任务 × 8 语言 =   80
来源：http://mobile.zdbjq.cn/Article/details/grhlmmxrz.sHtML

K JSON 与序列化         8 个任务 × 8 语言 =   64
来源：http://m.share.zdbjq.cn/Article/details/ggayebccg.sHtML

L 网络请求              8 个任务 × 8 语言 =   64
来源：http://www.blog.fehbvm.com/Article/details/gtmahitvl.sHtML

M 命令行 / 进程         8 个任务 × 8 语言 =   64
来源：http://blog.fehbvm.com/Article/details/gmyhwjduy.sHtML

N 数据结构与算法       12 个任务 × 8 语言 =   96
来源：http://www.blog.hesvh.cn/Article/details/ggwnlbrgr.sHtML

O 并发与异步            6 个任务 × 8 语言 =   48
来源：http://m.share.fehbvm.com/Article/details/gmrlqjpvi.sHtML

P 常用工具函数          8 个任务 × 8 语言 =   64
来源：http://read.share.fehbvm.com/Article/details/gnzbllkyx.sHtML

Q SQL 专题                              90
来源：http://www.m.share.zdbjq.cn/Article/details/gggcikzpe.sHtML

R Bash 专题                             80
来源：http://www.blog.zdbjq.cn/Article/details/guypylhvu.sHtML

S C / C++ 专题                          60
来源：http://www.share.hesvh.cn/Article/details/gitsscudd.sHtML

T 其他语言补充                          60
来源：http://blog.fehbvm.com/Article/details/gngwcufiu.sHtML

U 高频实用片段                         120
来源：http://www.blog.hesvh.cn/Article/details/gijnhzmim.sHtML

------------------------------------
来源：http://www.blog.zdbjq.cn/Article/details/gydklqrpg.sHtML

合计                                  2106 条
来源：http://m.share.hesvh.cn/Article/details/gjsfepwyp.sHtML

--------------------------------------------------------------------------------
来源：http://m.share.hesvh.cn/Article/details/gsbtdjkiu.sHtML

使用提醒
来源：http://m.share.hesvh.cn/Article/details/gdrzgsjgu.sHtML

--------------------------------------------------------------------------------
来源：http://blog.fehbvm.com/Article/details/glslspmeh.sHtML

1. 示例追求"最小可用"，正式项目中请补齐导入、错误处理与边界判断。
来源：http://www.blog.hesvh.cn/Article/details/gijrfrdvi.sHtML

2. 涉及文件、网络、数据库的示例，注意资源释放与异常捕获。
来源：http://www.blog.fehbvm.com/Article/details/gwledrael.sHtML

3. 语言版本差异较大（如 Python 3.10 的 match、Java 17 的 record/switch 箭头），
来源：http://baike.hesvh.cn/Article/details/gtsfgpury.sHtML

在旧版本上使用前请先确认语法支持情况。
来源：http://www.m.share.fehbvm.com/Article/details/geonipmre.sHtML

4. 标注"手写"的条目是因为该语言缺少对应内置能力，实际项目中可引入成熟库。
来源：http://wap.hesvh.cn/Article/details/ghczbvowm.sHtML

—— 文件结束 ——
来源：http://mobile.fehbvm.com/Article/details/gldtzgrpi.sHtML

================================================================================
来源：http://blog.zdbjq.cn/Article/details/gxzyawtzm.sHtML

程序语言常见例子速查手册（2024 版）
来源：http://mobile.hesvh.cn/Article/details/gmudwlbyj.sHtML

Common Programming Examples Cheat Book
来源：http://m.share.zdbjq.cn/Article/details/gidzqyybl.sHtML

================================================================================
来源：http://read.share.zdbjq.cn/Article/details/gxmgfwway.sHtML

【收录内容】
来源：http://blog.fehbvm.com/Article/details/gxfztbmkx.sHtML

覆盖 12 种语言 / 语法与常见 API：
来源：http://baike.fehbvm.com/Article/details/gjyisvput.sHtML

Python · PHP · JavaScript · TypeScript · Java · Go · Ruby · C#
来源：http://baike.hesvh.cn/Article/details/gbsryftrv.sHtML

SQL · Bash · C · C++
来源：http://read.share.zdbjq.cn/Article/details/gbtlcdohy.sHtML

按「任务」分组：每个任务下按语言各给出一条最小可用示例。
来源：http://mobile.fehbvm.com/Article/details/goksemomc.sHtML

【使用说明】
来源：http://read.share.fehbvm.com/Article/details/gsksdwcps.sHtML

1. 每个任务形如 "[编号] 任务名"，下面每行以语言标记开头：
来源：http://mobile.zdbjq.cn/Article/details/gupbzwjfz.sHtML

Py:    Python        PHP:   PHP           JS:    JavaScript
来源：http://m.share.hesvh.cn/Article/details/gdanzynkb.sHtML

TS:    TypeScript    Java:  Java          Go:    Go
来源：http://www.blog.fehbvm.com/Article/details/gzcfypghl.sHtML

Ruby:  Ruby          C#:    C#            SQL:   SQL
来源：http://3g.fehbvm.com/Article/details/grkgwjmss.sHtML

Bash:  Shell         C:     C             C++:   C++
来源：http://www.share.hesvh.cn/Article/details/guhhpuykp.sHtML

2. 示例只展示核心写法，刻意省略 import / require / include / using 等样板代码。
来源：http://blog.fehbvm.com/Article/details/gdpzuxkjp.sHtML

需要完整可运行文件时，请自行补齐当前语言的导入语句。
来源：http://www.blog.zdbjq.cn/Article/details/gtooyfbtp.sHtML

3. 语法基准：Python 3.10+ / PHP 8.1+ / ES2020+ / TypeScript 5 / Java 17 /
来源：http://mobile.fehbvm.com/Article/details/gxhpisejw.sHtML

Go 1.21+ / Ruby 3.x / C# 10+ / C17 / C++17。
来源：http://3g.fehbvm.com/Article/details/ggdcvutjd.sHtML

4. 检索建议：用编辑器或浏览器 Ctrl+F 搜关键词，如 "排序" "读取文件" "正则"。
来源：http://baike.hesvh.cn/Article/details/gqpntjacb.sHtML

5. 标记为 "// 无" 表示该语言没有对应的一等语法，需用替代写法（示例给出替代方案）。
来源：http://3g.zdbjq.cn/Article/details/gjszsvfvo.sHtML

6. 符号 "⏎" 表示代码在此处换行（主要用于 Python 等强制缩进、无法压成一行的结构）。
来源：http://read.share.hesvh.cn/Article/details/gwzvlfung.sHtML

【文件统计】
来源：http://blog.fehbvm.com/Article/details/grgqcseod.sHtML

语言示例共 2106 条，分布见本文末尾的「统计汇总」。
来源：http://blog.fehbvm.com/Article/details/gzaphuxcf.sHtML

--------------------------------------------------------------------------------
来源：http://m.share.fehbvm.com/Article/details/gxertvhel.sHtML

目  录
来源：http://baike.fehbvm.com/Article/details/glktwcvyz.sHtML

--------------------------------------------------------------------------------
来源：http://baike.fehbvm.com/Article/details/ggtqcddhu.sHtML

A. 基础语法与类型              （第 1 节，26 个任务，208 条）
来源：http://www.blog.fehbvm.com/Article/details/gawkrudfo.sHtML

B. 流程控制                    （第 2 节，16 个任务，128 条）
来源：http://3g.hesvh.cn/Article/details/gjljjmexj.sHtML

C. 函数与作用域                （第 3 节，16 个任务，128 条）
来源：http://3g.hesvh.cn/Article/details/gqvlhyygl.sHtML

D. 数组 / 列表 / 集合          （第 4 节，26 个任务，208 条）
来源：http://www.share.fehbvm.com/Article/details/gywckktah.sHtML

E. 字符串处理                  （第 5 节，22 个任务，176 条）
来源：http://baike.zdbjq.cn/Article/details/gmnwefjdn.sHtML

F. 文件与目录                  （第 6 节，12 个任务，96 条）
来源：http://www.m.share.fehbvm.com/Article/details/gxhhrgxnk.sHtML

G. 面向对象                    （第 7 节，16 个任务，128 条）
来源：http://www.blog.zdbjq.cn/Article/details/gsaqiiffe.sHtML

H. 异常与错误处理              （第 8 节，10 个任务，80 条）
来源：http://blog.fehbvm.com/Article/details/godpyplbw.sHtML

I. 正则表达式                  （第 9 节，8 个任务，64 条）
来源：http://www.share.hesvh.cn/Article/details/gllunjpee.sHtML

J. 日期与时间                  （第 10 节，10 个任务，80 条）
来源：http://www.blog.fehbvm.com/Article/details/gnustghaz.sHtML

K. JSON 与序列化               （第 11 节，8 个任务，64 条）
来源：http://m.share.zdbjq.cn/Article/details/gibkgdhfw.sHtML

L. 网络请求                    （第 12 节，8 个任务，64 条）
来源：http://m.share.hesvh.cn/Article/details/gprlteckv.sHtML

M. 命令行 / 进程 / 环境        （第 13 节，8 个任务，64 条）
来源：http://blog.hesvh.cn/Article/details/gwyhfhqsr.sHtML

N. 数据结构与算法              （第 14 节，12 个任务，96 条）
来源：http://wap.zdbjq.cn/Article/details/gqeumsjur.sHtML

O. 并发与异步                  （第 15 节，6 个任务，48 条）
来源：http://www.blog.hesvh.cn/Article/details/gsiqtsxwa.sHtML

P. 常用工具函数                （第 16 节，8 个任务，64 条）
来源：http://blog.fehbvm.com/Article/details/gzobmqvqt.sHtML

Q. SQL 专题                    （第 17 节，90 条）
来源：http://3g.fehbvm.com/Article/details/gbtofijpb.sHtML

R. Bash 专题                   （第 18 节，80 条）
来源：http://baike.fehbvm.com/Article/details/gchjluzvy.sHtML

S. C / C++ 专题                （第 19 节，60 条）
来源：http://m.share.hesvh.cn/Article/details/gbizlffhl.sHtML

T. 其他语言补充                （第 20 节，60 条：Kotlin / Swift / Lua / Perl / Scala）
来源：http://www.blog.zdbjq.cn/Article/details/garvlumro.sHtML

U. 高频实用片段                （第 21 节，120 条：Python / PHP / JavaScript 各 40 条）
来源：http://read.share.fehbvm.com/Article/details/gtioomqlc.sHtML

================================================================================
来源：http://blog.hesvh.cn/Article/details/gqywlooxj.sHtML

A. 基础语法与类型
来源：http://www.blog.zdbjq.cn/Article/details/guyrcrcug.sHtML

================================================================================
来源：http://3g.zdbjq.cn/Article/details/gllvxsfdc.sHtML

[A01] Hello World
来源：http://wap.zdbjq.cn/Article/details/gdsjaebyi.sHtML

Py:   print("Hello, World!")
来源：http://read.share.zdbjq.cn/Article/details/gighjvsot.sHtML

PHP:  echo "Hello, World!";
来源：http://www.m.share.hesvh.cn/Article/details/gtvaqujne.sHtML

JS:   console.log("Hello, World!");
来源：http://wap.hesvh.cn/Article/details/gqyeivngl.sHtML

TS:   const msg: string = "Hello, World!"; console.log(msg);
来源：http://m.share.hesvh.cn/Article/details/gjzawrsmr.sHtML

Java: System.out.println("Hello, World!");
来源：http://www.share.hesvh.cn/Article/details/gdwacipmn.sHtML

Go:   fmt.Println("Hello, World!")
来源：http://blog.hesvh.cn/Article/details/gwxlkloue.sHtML

Ruby: puts "Hello, World!"
来源：http://www.share.hesvh.cn/Article/details/gdowyxigw.sHtML

C#:   Console.WriteLine("Hello, World!");
来源：http://www.m.share.hesvh.cn/Article/details/gtkflrtrr.sHtML

[A02] 变量声明与赋值
来源：http://baike.zdbjq.cn/Article/details/gzzfsucug.sHtML

Py:   name = "Alex"; age = 20            # 动态类型，无需声明
来源：http://www.share.hesvh.cn/Article/details/gutkmilqz.sHtML

PHP:  $name = "Alex"; $age = 20;
来源：http://blog.fehbvm.com/Article/details/glmutdxef.sHtML

JS:   let name = "Alex"; const age = 20;
来源：http://m.share.hesvh.cn/Article/details/gfppkzvsk.sHtML


<!-- 参考信息 -->