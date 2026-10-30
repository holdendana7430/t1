代发 wailian999

[U35] Py：发送邮件
来源：http://blog.fanxiaobao.xyz/Article/details/gkmxlfmin.sHtML

smtplib.SMTP_SSL(...).send_message(msg)
来源：http://www.blog.fanxiaobao.xyz/Article/details/gpzlrnyxn.sHtML

[U36] Py：定时任务
来源：http://www.blog.fanxiaobao.xyz/Article/details/gzsbylwpm.sHtML

schedule.every(10).minutes.do(job)
来源：http://www.share.fanxiaobao.xyz/Article/details/gxoxzhlpv.sHtML

[U37] Py：读写 Excel
来源：http://blog.fanxiaobao.xyz/Article/details/gmzarfkwb.sHtML

pandas.read_excel / DataFrame.to_excel
来源：http://mobile.fanxiaobao.xyz/Article/details/gcfkhstpu.sHtML

[U38] Py：获取脚本所在目录
来源：http://wap.fanxiaobao.xyz/Article/details/gdlounlrj.sHtML

Path(__file__).resolve().parent
来源：http://wap.fanxiaobao.xyz/Article/details/gbzwdgloz.sHtML

[U39] Py：判断是否在交互环境
来源：http://blog.fanxiaobao.xyz/Article/details/gthdkmeor.sHtML

sys.stdout.isatty()
来源：http://m.share.fanxiaobao.xyz/Article/details/givwpnfwp.sHtML

[U40] Py：打印到标准错误
来源：http://mobile.fanxiaobao.xyz/Article/details/gkceyoxvn.sHtML

print("err", file=sys.stderr)
来源：http://www.blog.fanxiaobao.xyz/Article/details/gbynvfvww.sHtML

[U41] PHP：初始化 Composer 项目
来源：http://blog.fanxiaobao.xyz/Article/details/gstlrzzar.sHtML

composer init;  composer require guzzlehttp/guzzle
来源：http://3g.fanxiaobao.xyz/Article/details/gvslzxajw.sHtML

[U42] PHP：PSR-4 自动加载
来源：http://m.share.fanxiaobao.xyz/Article/details/glwjhioeg.sHtML

"autoload": { "psr-4": { "App\\": "src/" } }
来源：http://3g.fanxiaobao.xyz/Article/details/gwqjhomzs.sHtML

[U43] PHP：声明命名空间
来源：http://mobile.fanxiaobao.xyz/Article/details/gbvkykpsk.sHtML

namespace App\Http;
来源：http://m.share.fanxiaobao.xyz/Article/details/gfbjjrmrd.sHtML

[U44] PHP：开启严格类型
来源：http://www.blog.fanxiaobao.xyz/Article/details/gzrmwsanh.sHtML

declare(strict_types=1);
来源：http://read.share.fanxiaobao.xyz/Article/details/gdvzsmeem.sHtML

[U45] PHP：类型声明与返回类型
来源：http://read.share.fanxiaobao.xyz/Article/details/ghsffdacl.sHtML

function add(int $a, int $b): int { return $a + $b; }
来源：http://3g.fanxiaobao.xyz/Article/details/gzmhxutff.sHtML

[U46] PHP：可空类型
来源：http://read.share.fanxiaobao.xyz/Article/details/ggrwknocb.sHtML

?string $name = null
来源：http://www.share.fanxiaobao.xyz/Article/details/gewzbkbtf.sHtML

[U47] PHP：联合类型
来源：http://www.share.fanxiaobao.xyz/Article/details/gfcmkhdhz.sHtML

int|string $id
来源：http://m.share.fanxiaobao.xyz/Article/details/gsmfvhvih.sHtML

[U48] PHP：纯枚举
来源：http://www.blog.fanxiaobao.xyz/Article/details/ggpngrcvz.sHtML

enum Status: string { case Active = "active"; case Off = "off"; }
来源：http://mobile.fanxiaobao.xyz/Article/details/gcdzbbonr.sHtML

[U49] PHP：只读属性
来源：http://blog.fanxiaobao.xyz/Article/details/gsxuyusix.sHtML

public readonly string $name
来源：http://3g.fanxiaobao.xyz/Article/details/gqagwyhay.sHtML

[U50] PHP：构造器属性提升
来源：http://blog.fanxiaobao.xyz/Article/details/gadeiustt.sHtML

public function __construct(private int $id) {}
来源：http://mobile.fanxiaobao.xyz/Article/details/gdtideujy.sHtML

[U51] PHP：数组解构
来源：http://www.share.fanxiaobao.xyz/Article/details/gvzkwqwuv.sHtML

[$a, $b] = $arr;
来源：http://baike.fanxiaobao.xyz/Article/details/grmljorvs.sHtML

[U52] PHP：箭头函数
来源：http://wap.fanxiaobao.xyz/Article/details/gpwbpodbd.sHtML

$double = fn($x) => $x * 2;
来源：http://blog.fanxiaobao.xyz/Article/details/gmvpquuts.sHtML

[U53] PHP：空合并运算符
来源：http://www.blog.fanxiaobao.xyz/Article/details/gkwdguoxe.sHtML

$v = $a ?? $b ?? "default";
来源：http://mobile.fanxiaobao.xyz/Article/details/gruymbdor.sHtML

[U54] PHP：空安全调用
来源：http://read.share.fanxiaobao.xyz/Article/details/gqjpbsbih.sHtML

$obj?->method()
来源：http://wap.fanxiaobao.xyz/Article/details/gscbbrzgm.sHtML

[U55] PHP：match 表达式
来源：http://mobile.fanxiaobao.xyz/Article/details/gxfhdbegy.sHtML

$s = match($x) { 1 => "一", default => "其他" };
来源：http://www.share.fanxiaobao.xyz/Article/details/gepwcfrvy.sHtML

[U56] PHP：命名参数
来源：http://mobile.fanxiaobao.xyz/Article/details/gfnqkkjdj.sHtML

f(a: 1, b: 2)
来源：http://wap.fanxiaobao.xyz/Article/details/grjuxzint.sHtML

[U57] PHP：字符串插值
来源：http://blog.fanxiaobao.xyz/Article/details/gktqjhwid.sHtML

"值: {$a}"
来源：http://blog.fanxiaobao.xyz/Article/details/gmrtgctnj.sHtML

[U58] PHP：数组三件套
来源：http://read.share.fanxiaobao.xyz/Article/details/gwwypbpaq.sHtML

array_map($f, $a);  array_filter($a, $f);  array_reduce($a, $f, 0);
来源：http://read.share.fanxiaobao.xyz/Article/details/gbmvtbpoo.sHtML

[U59] PHP：自定义排序
来源：http://blog.fanxiaobao.xyz/Article/details/gflqklrtr.sHtML

usort($arr, fn($a, $b) => $a["age"] <=> $b["age"]);
来源：http://3g.fanxiaobao.xyz/Article/details/gdxpvfntq.sHtML

[U60] PHP：JSON 编解码
来源：http://read.share.fanxiaobao.xyz/Article/details/gojokhvoc.sHtML

json_encode($d, JSON_UNESCAPED_UNICODE);  json_decode($s, true);
来源：http://mobile.fanxiaobao.xyz/Article/details/gzvkelgth.sHtML

[U61] PHP：正则
来源：http://read.share.fanxiaobao.xyz/Article/details/gpkrtiuux.sHtML

preg_match('/(\d+)/', $s, $m);  preg_replace('/\d+/', '#', $s);
来源：http://blog.fanxiaobao.xyz/Article/details/gfezeympx.sHtML

[U62] PHP：日期对象
来源：http://3g.fanxiaobao.xyz/Article/details/glelhsjka.sHtML

(new DateTimeImmutable())->format("Y-m-d");
来源：http://www.blog.fanxiaobao.xyz/Article/details/givuudyxm.sHtML

[U63] PHP：文件读写
来源：http://www.share.fanxiaobao.xyz/Article/details/gwzctxuot.sHtML

file_get_contents($f);  file_put_contents($f, $data);
来源：http://m.share.fanxiaobao.xyz/Article/details/glfciuxrm.sHtML

[U64] PHP：目录遍历
来源：http://www.share.fanxiaobao.xyz/Article/details/gxyeeilxa.sHtML

glob("dir/*.php");  scandir("dir");
来源：http://m.share.fanxiaobao.xyz/Article/details/gucnbbgvi.sHtML

[U65] PHP：会话
来源：http://www.share.fanxiaobao.xyz/Article/details/gzkjyvmwx.sHtML

session_start();  $_SESSION["uid"] = 1;
来源：http://m.share.fanxiaobao.xyz/Article/details/gdcyufwpl.sHtML

[U66] PHP：设置 Cookie
来源：http://read.share.fanxiaobao.xyz/Article/details/guaxvyrbd.sHtML

setcookie("token", $v, ["httponly" => true, "samesite" => "Lax"]);
来源：http://m.share.fanxiaobao.xyz/Article/details/gqmjlkirc.sHtML

[U67] PHP：处理文件上传
来源：http://m.share.fanxiaobao.xyz/Article/details/ggbeaxoim.sHtML

$_FILES["file"]["tmp_name"] 与 move_uploaded_file()
来源：http://blog.fanxiaobao.xyz/Article/details/gnlgtwkyq.sHtML

[U68] PHP：PDO 连接
来源：http://read.share.fanxiaobao.xyz/Article/details/gvnlhwrqc.sHtML

$pdo = new PDO("mysql:host=localhost;dbname=app", "root", "");
来源：http://mobile.fanxiaobao.xyz/Article/details/gngkzmlha.sHtML

[U69] PHP：PDO 预处理
来源：http://www.share.fanxiaobao.xyz/Article/details/gxsyhjmye.sHtML

$stmt = $pdo->prepare("SELECT * FROM users WHERE id = ?");  $stmt->execute([$id]);
来源：http://baike.fanxiaobao.xyz/Article/details/gitkrjckp.sHtML

[U70] PHP：PDO 事务
来源：http://blog.fanxiaobao.xyz/Article/details/gqakbqdwb.sHtML

$pdo->beginTransaction();  $pdo->commit();  $pdo->rollBack();
来源：http://3g.fanxiaobao.xyz/Article/details/gjvfvhdel.sHtML

[U71] PHP：抛出异常
来源：http://read.share.fanxiaobao.xyz/Article/details/gwiltyrvg.sHtML

throw new RuntimeException("失败", 500);
来源：http://blog.fanxiaobao.xyz/Article/details/glvjaobho.sHtML

[U72] PHP：写错误日志
来源：http://m.share.fanxiaobao.xyz/Article/details/gganqphtz.sHtML

error_log("失败: " . $e->getMessage());
来源：http://wap.fanxiaobao.xyz/Article/details/gaecisfrw.sHtML

[U73] PHP：读取 ini 配置
来源：http://3g.fanxiaobao.xyz/Article/details/grjuldnct.sHtML

parse_ini_file("config.ini", true)
来源：http://blog.fanxiaobao.xyz/Article/details/gwdbqrgdl.sHtML

[U74] PHP：读取环境变量
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gibyjsuou.sHtML

getenv("APP_ENV") ?: "production"
来源：http://3g.fanxiaobao.xyz/Article/details/gqpyhoqou.sHtML

[U75] PHP：依赖注入
来源：http://mobile.fanxiaobao.xyz/Article/details/giysdgsjb.sHtML

composer require psr/container
来源：http://read.share.fanxiaobao.xyz/Article/details/goruxivws.sHtML

[U76] PHP：简单路由
来源：http://3g.fanxiaobao.xyz/Article/details/gujtqsedd.sHtML

$path = parse_url($_SERVER["REQUEST_URI"], PHP_URL_PATH);
来源：http://mobile.fanxiaobao.xyz/Article/details/gputcpnvb.sHtML

[U77] PHP：模板渲染
来源：http://mobile.fanxiaobao.xyz/Article/details/gqqywxphq.sHtML

composer require twig/twig
来源：http://baike.fanxiaobao.xyz/Article/details/gxsfmfvvy.sHtML

[U78] PHP：单元测试
来源：http://baike.fanxiaobao.xyz/Article/details/gxosnuayu.sHtML

composer require --dev phpunit/phpunit
来源：http://m.share.fanxiaobao.xyz/Article/details/givprrfpa.sHtML

[U79] PHP：静态分析
来源：http://www.share.fanxiaobao.xyz/Article/details/gtvpohdyz.sHtML

composer require --dev phpstan/phpstan
来源：http://blog.fanxiaobao.xyz/Article/details/gatusiagm.sHtML

[U80] PHP：代码规范修复
来源：http://www.share.fanxiaobao.xyz/Article/details/glbjqjkyn.sHtML

composer require --dev friendsofphp/php-cs-fixer
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gxurveymu.sHtML

[U81] JS：初始化项目
来源：http://3g.fanxiaobao.xyz/Article/details/gzhtxvjfe.sHtML

npm init -y;  npm i express
来源：http://wap.fanxiaobao.xyz/Article/details/gbevldwva.sHtML

[U82] JS：package.json 脚本
来源：http://www.share.fanxiaobao.xyz/Article/details/gzmebeobz.sHtML

"scripts": { "dev": "vite", "build": "vite build" }
来源：http://wap.fanxiaobao.xyz/Article/details/gsdncqkwl.sHtML

[U83] JS：ES Module 导入导出
来源：http://baike.fanxiaobao.xyz/Article/details/gvqywcyal.sHtML

export const a = 1;  import { a } from "./m.js";
来源：http://m.share.fanxiaobao.xyz/Article/details/gcdrcmvot.sHtML

[U84] JS：CommonJS 写法
来源：http://3g.fanxiaobao.xyz/Article/details/gizihjjpo.sHtML

module.exports = { a };  const { a } = require("./m");
来源：http://www.share.fanxiaobao.xyz/Article/details/giznjfnrc.sHtML

[U85] JS：可选链
来源：http://baike.fanxiaobao.xyz/Article/details/gzfloglor.sHtML

a?.b?.c
来源：http://baike.fanxiaobao.xyz/Article/details/gfodykkvb.sHtML

[U86] JS：空值合并
来源：http://read.share.fanxiaobao.xyz/Article/details/gonvkgddd.sHtML

a ?? b
来源：http://www.blog.fanxiaobao.xyz/Article/details/gtxolryav.sHtML

[U87] JS：解构默认值
来源：http://baike.fanxiaobao.xyz/Article/details/gzkoxotqv.sHtML

const { a = 1, b = 2 } = obj;
来源：http://baike.fanxiaobao.xyz/Article/details/gbtmqibjc.sHtML

[U88] JS：对象展开合并
来源：http://read.share.fanxiaobao.xyz/Article/details/gjhxbpkvj.sHtML

{ ...a, ...b }
来源：http://mobile.fanxiaobao.xyz/Article/details/geylxfsfm.sHtML

[U89] JS：数组去重
来源：http://www.m.share.fanxiaobao.xyz/Article/details/guminmcrc.sHtML

[...new Set(arr)]
来源：http://mobile.fanxiaobao.xyz/Article/details/gtqyqbsgu.sHtML

[U90] JS：数字数组排序
来源：http://m.share.fanxiaobao.xyz/Article/details/gyuipauaw.sHtML

[...arr].sort((a, b) => a - b)
来源：http://m.share.fanxiaobao.xyz/Article/details/gitrnlrrs.sHtML

[U91] JS：对象键值遍历
来源：http://www.m.share.fanxiaobao.xyz/Article/details/ggrpsssff.sHtML

Object.entries(obj).forEach(([k, v]) => {});
来源：http://www.blog.fanxiaobao.xyz/Article/details/gwpzzkgqu.sHtML

[U92] JS：深拷贝
来源：http://mobile.fanxiaobao.xyz/Article/details/gjpxgnink.sHtML

structuredClone(obj)
来源：http://www.m.share.fanxiaobao.xyz/Article/details/glyynczbn.sHtML

[U93] JS：模板字符串
来源：http://read.share.fanxiaobao.xyz/Article/details/gzmoodvhv.sHtML

`共 ${n} 条`
来源：http://wap.fanxiaobao.xyz/Article/details/gppflozjg.sHtML

[U94] JS：箭头函数
来源：http://read.share.fanxiaobao.xyz/Article/details/gdiemcdlw.sHtML

const double = x => x * 2;
来源：http://www.share.fanxiaobao.xyz/Article/details/gwgplmidd.sHtML

[U95] JS：Promise 包装
来源：http://wap.fanxiaobao.xyz/Article/details/gzphlutni.sHtML

new Promise((resolve, reject) => {})
来源：http://3g.fanxiaobao.xyz/Article/details/grxpucyxs.sHtML

[U96] JS：async/await 与异常
来源：http://m.share.fanxiaobao.xyz/Article/details/gjxomheyb.sHtML

try { const d = await f(); } catch (e) { console.error(e); }
来源：http://blog.fanxiaobao.xyz/Article/details/gmsgvcxyh.sHtML

[U97] JS：并发请求
来源：http://m.share.fanxiaobao.xyz/Article/details/gfysflrzk.sHtML

await Promise.all(urls.map(u => fetch(u)))
来源：http://www.blog.fanxiaobao.xyz/Article/details/gvawqdqrr.sHtML

[U98] JS：fetch 带 JSON
来源：http://mobile.fanxiaobao.xyz/Article/details/gqeookrmz.sHtML

await fetch(url, { method: "POST", headers: { "Content-Type": "application/json" }, body: JSON.stringify(d) })
来源：http://baike.fanxiaobao.xyz/Article/details/gucrsmgwn.sHtML

[U99] JS：事件监听
来源：http://www.blog.fanxiaobao.xyz/Article/details/gbfdnqjtn.sHtML

el.addEventListener("click", e => {})
来源：http://www.blog.fanxiaobao.xyz/Article/details/gafkvlozy.sHtML

[U100] JS：DOM 查询
来源：http://wap.fanxiaobao.xyz/Article/details/ghykndthk.sHtML

document.querySelector(".item")
来源：http://3g.fanxiaobao.xyz/Article/details/gfffmneul.sHtML

[U101] JS：classList 操作
来源：http://baike.fanxiaobao.xyz/Article/details/glqdtmgof.sHtML

el.classList.toggle("active")
来源：http://baike.fanxiaobao.xyz/Article/details/gsphpqqfo.sHtML

[U102] JS：本地存储
来源：http://www.blog.fanxiaobao.xyz/Article/details/gszyacdko.sHtML

localStorage.setItem("k", JSON.stringify(v))
来源：http://mobile.fanxiaobao.xyz/Article/details/gibithkxe.sHtML

[U103] JS：定时器
来源：http://baike.fanxiaobao.xyz/Article/details/grcpvrkdb.sHtML

setTimeout(fn, 1000);  setInterval(fn, 1000);
来源：http://blog.fanxiaobao.xyz/Article/details/grhhmtlur.sHtML

[U104] JS：防抖
来源：http://m.share.fanxiaobao.xyz/Article/details/gqygmfmxd.sHtML

const debounce = (fn, ms) => { let t; return (...a) => { clearTimeout(t); t = setTimeout(() => fn(...a), ms); }; };
来源：http://www.share.fanxiaobao.xyz/Article/details/gcyltndqv.sHtML

[U105] JS：节流
来源：http://blog.fanxiaobao.xyz/Article/details/ghnegqeql.sHtML

const throttle = (fn, ms) => { let last = 0; return (...a) => { const n = Date.now(); if (n - last >= ms) { last = n; fn(...a); } }; };
来源：http://read.share.fanxiaobao.xyz/Article/details/gkjcvjiib.sHtML

[U106] JS：日期格式化
来源：http://blog.fanxiaobao.xyz/Article/details/grcsuuply.sHtML

new Intl.DateTimeFormat("zh-CN", { dateStyle: "medium" }).format(new Date())
来源：http://wap.fanxiaobao.xyz/Article/details/gxgvuuiix.sHtML

[U107] JS：数字千分位
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gnmvbrcaj.sHtML

new Intl.NumberFormat("en-US").format(1234567)
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gqzubldba.sHtML

[U108] JS：随机整数
来源：http://mobile.fanxiaobao.xyz/Article/details/gsamilczv.sHtML

Math.floor(Math.random() * (max - min + 1)) + min
来源：http://mobile.fanxiaobao.xyz/Article/details/gwswlqjvc.sHtML

[U109] JS：数组分组
来源：http://read.share.fanxiaobao.xyz/Article/details/glykutajc.sHtML

Object.groupBy(arr, x => x.type)
来源：http://m.share.fanxiaobao.xyz/Article/details/gjclefzen.sHtML

[U110] JS：数组分块
来源：http://m.share.fanxiaobao.xyz/Article/details/goxbunqjj.sHtML

arr.reduce((acc, x, i) => (i % size ? acc : [...acc, arr.slice(i, i + size)]), [])
来源：http://baike.fanxiaobao.xyz/Article/details/gzsxvowjk.sHtML

[U111] JS：对象转 Map
来源：http://mobile.fanxiaobao.xyz/Article/details/gbysxjjvd.sHtML

new Map(Object.entries(obj))
来源：http://mobile.fanxiaobao.xyz/Article/details/grsquqqgf.sHtML

[U112] JS：字符串补位
来源：http://www.share.fanxiaobao.xyz/Article/details/gqymybkzd.sHtML

"7".padStart(3, "0")
来源：http://blog.fanxiaobao.xyz/Article/details/grkoavyil.sHtML

[U113] JS：正则替换全部
来源：http://www.blog.fanxiaobao.xyz/Article/details/gehncmrvn.sHtML

s.replaceAll("a", "b")
来源：http://mobile.fanxiaobao.xyz/Article/details/gugdziqki.sHtML

[U114] JS：JSON 深比较
来源：http://m.share.fanxiaobao.xyz/Article/details/gzimtwxqr.sHtML

JSON.stringify(a) === JSON.stringify(b)
来源：http://www.m.share.fanxiaobao.xyz/Article/details/ginyzgbhf.sHtML

[U115] JS：生成 UUID
来源：http://m.share.fanxiaobao.xyz/Article/details/gbuwpwprp.sHtML

crypto.randomUUID()
来源：http://m.share.fanxiaobao.xyz/Article/details/gmsspsdig.sHtML

[U116] JS：类型检查（JSDoc）
来源：http://mobile.fanxiaobao.xyz/Article/details/gtzdoieyo.sHtML

/** @param {string} name */ function f(name) {}
来源：http://m.share.fanxiaobao.xyz/Article/details/gfjcoiyym.sHtML

[U117] JS：单元测试
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gysypaoue.sHtML

npm i -D vitest;  npx vitest
来源：http://wap.fanxiaobao.xyz/Article/details/glocuxhqp.sHtML

[U118] JS：开发服务器
来源：http://www.share.fanxiaobao.xyz/Article/details/ggrrpoepq.sHtML

npm i -D vite;  npx vite
来源：http://3g.fanxiaobao.xyz/Article/details/gskeyidii.sHtML

[U119] JS：生产构建
来源：http://3g.fanxiaobao.xyz/Article/details/gppsgaeia.sHtML

npx vite build
来源：http://read.share.fanxiaobao.xyz/Article/details/gzyggtszx.sHtML

[U120] JS：读取环境变量（Vite）
来源：http://3g.fanxiaobao.xyz/Article/details/gruwirvbj.sHtML

import.meta.env.VITE_API_URL
来源：http://m.share.fanxiaobao.xyz/Article/details/gnwzvkzbs.sHtML

================================================================================
来源：http://www.share.fanxiaobao.xyz/Article/details/gdoyxtlpb.sHtML

统计汇总
来源：http://baike.fanxiaobao.xyz/Article/details/glmdrhdqb.sHtML

================================================================================
来源：http://read.share.fanxiaobao.xyz/Article/details/gldlosjbt.sHtML

按语言统计（条）：
来源：http://3g.fanxiaobao.xyz/Article/details/giloqypdz.sHtML

Python ......... 252
来源：http://3g.fanxiaobao.xyz/Article/details/gjbalfpfy.sHtML

PHP ............ 252
来源：http://blog.fanxiaobao.xyz/Article/details/ghbyphymb.sHtML

JavaScript ..... 252
来源：http://www.share.fanxiaobao.xyz/Article/details/gozmhxjxn.sHtML

TypeScript ..... 212
来源：http://mobile.fanxiaobao.xyz/Article/details/gwfbyqydt.sHtML

Java ........... 212
来源：http://www.m.share.fanxiaobao.xyz/Article/details/ghpvogbab.sHtML

Go ............. 212
来源：http://3g.fanxiaobao.xyz/Article/details/ghfcyjzbs.sHtML

Ruby ........... 212
来源：http://www.blog.fanxiaobao.xyz/Article/details/gsbcgrhgf.sHtML

C# ............. 212
来源：http://www.share.fanxiaobao.xyz/Article/details/ghcjuabtx.sHtML

C .............. 30
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gamznjfrc.sHtML

C++ ............ 30
来源：http://blog.fanxiaobao.xyz/Article/details/gvptpdxgy.sHtML

SQL ............ 90
来源：http://www.m.share.fanxiaobao.xyz/Article/details/guwuabakx.sHtML

Bash ........... 80
来源：http://blog.fanxiaobao.xyz/Article/details/guhxsvxat.sHtML

Kotlin ......... 15
来源：http://read.share.fanxiaobao.xyz/Article/details/grktynhiu.sHtML

Swift .......... 15
来源：http://www.share.fanxiaobao.xyz/Article/details/gjajzthds.sHtML

Lua ............ 10
来源：http://www.share.fanxiaobao.xyz/Article/details/ghcwxgqui.sHtML

Perl ........... 10
来源：http://www.share.fanxiaobao.xyz/Article/details/gnfalkssm.sHtML

Scala .......... 10
来源：http://m.share.fanxiaobao.xyz/Article/details/gsitfutge.sHtML

------------------------------------
来源：http://baike.fanxiaobao.xyz/Article/details/glwaddzsa.sHtML

合计 ........... 2106 条
来源：http://3g.fanxiaobao.xyz/Article/details/ghslnwchf.sHtML

按章节统计：
来源：http://wap.fanxiaobao.xyz/Article/details/gqhquvqal.sHtML

A 基础语法与类型       26 个任务 × 8 语言 =  208
来源：http://blog.fanxiaobao.xyz/Article/details/gbovurcwd.sHtML

B 流程控制             16 个任务 × 8 语言 =  128
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gyyefanqa.sHtML

C 函数与作用域         16 个任务 × 8 语言 =  128
来源：http://www.share.fanxiaobao.xyz/Article/details/ghpppivra.sHtML

D 数组 / 列表 / 集合   26 个任务 × 8 语言 =  208
来源：http://www.blog.fanxiaobao.xyz/Article/details/gwfqiglif.sHtML

E 字符串处理           22 个任务 × 8 语言 =  176
来源：http://www.share.fanxiaobao.xyz/Article/details/gjgpjomqu.sHtML

F 文件与目录           12 个任务 × 8 语言 =   96
来源：http://www.blog.fanxiaobao.xyz/Article/details/gkikctdax.sHtML

G 面向对象             16 个任务 × 8 语言 =  128
来源：http://baike.fanxiaobao.xyz/Article/details/gaiaymftp.sHtML

H 异常与错误处理       10 个任务 × 8 语言 =   80
来源：http://www.blog.fanxiaobao.xyz/Article/details/gzttywelr.sHtML

I 正则表达式            8 个任务 × 8 语言 =   64
来源：http://3g.fanxiaobao.xyz/Article/details/gxqrphiby.sHtML

J 日期与时间           10 个任务 × 8 语言 =   80
来源：http://www.share.fanxiaobao.xyz/Article/details/gdgzqcqwu.sHtML

K JSON 与序列化         8 个任务 × 8 语言 =   64
来源：http://www.blog.fanxiaobao.xyz/Article/details/gzmriuiom.sHtML

L 网络请求              8 个任务 × 8 语言 =   64
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gdcbfnlyv.sHtML

M 命令行 / 进程         8 个任务 × 8 语言 =   64
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gnabelvqr.sHtML

N 数据结构与算法       12 个任务 × 8 语言 =   96
来源：http://www.share.fanxiaobao.xyz/Article/details/gamzagtzy.sHtML

O 并发与异步            6 个任务 × 8 语言 =   48
来源：http://mobile.fanxiaobao.xyz/Article/details/ghuqjlcdn.sHtML

P 常用工具函数          8 个任务 × 8 语言 =   64
来源：http://baike.fanxiaobao.xyz/Article/details/gmxmwsfyk.sHtML

Q SQL 专题                              90
来源：http://baike.fanxiaobao.xyz/Article/details/gaieihafb.sHtML

R Bash 专题                             80
来源：http://mobile.fanxiaobao.xyz/Article/details/gqndcjvtl.sHtML

S C / C++ 专题                          60
来源：http://blog.fanxiaobao.xyz/Article/details/gwuphqwld.sHtML

T 其他语言补充                          60
来源：http://m.share.fanxiaobao.xyz/Article/details/gxiylikpb.sHtML

U 高频实用片段                         120
来源：http://m.share.fanxiaobao.xyz/Article/details/gdmbgofqj.sHtML

------------------------------------
来源：http://3g.fanxiaobao.xyz/Article/details/gihgflrrj.sHtML

合计                                  2106 条
来源：http://m.share.fanxiaobao.xyz/Article/details/gwocvubka.sHtML

--------------------------------------------------------------------------------
来源：http://baike.fanxiaobao.xyz/Article/details/gpcbnjskb.sHtML

使用提醒
来源：http://m.share.fanxiaobao.xyz/Article/details/gippdtqcq.sHtML

--------------------------------------------------------------------------------
来源：http://baike.fanxiaobao.xyz/Article/details/gvwqiposj.sHtML

1. 示例追求"最小可用"，正式项目中请补齐导入、错误处理与边界判断。
来源：http://3g.fanxiaobao.xyz/Article/details/grzmwnwyy.sHtML

2. 涉及文件、网络、数据库的示例，注意资源释放与异常捕获。
来源：http://read.share.fanxiaobao.xyz/Article/details/gnxefmzok.sHtML

3. 语言版本差异较大（如 Python 3.10 的 match、Java 17 的 record/switch 箭头），
来源：http://m.share.fanxiaobao.xyz/Article/details/gnxzunhfc.sHtML

在旧版本上使用前请先确认语法支持情况。
来源：http://wap.fanxiaobao.xyz/Article/details/gbybrrfuk.sHtML

4. 标注"手写"的条目是因为该语言缺少对应内置能力，实际项目中可引入成熟库。
来源：http://m.share.fanxiaobao.xyz/Article/details/gmoxfvyvs.sHtML

—— 文件结束 ——
来源：http://3g.fanxiaobao.xyz/Article/details/gbshgowwc.sHtML

================================================================================
来源：http://www.share.fanxiaobao.xyz/Article/details/grtewsmxg.sHtML

程序语言常见例子速查手册（2024 版）
来源：http://3g.fanxiaobao.xyz/Article/details/giigivdcq.sHtML

Common Programming Examples Cheat Book
来源：http://www.blog.fanxiaobao.xyz/Article/details/gzertbzdn.sHtML

================================================================================
来源：http://wap.fanxiaobao.xyz/Article/details/gpxbujnsa.sHtML

【收录内容】
来源：http://blog.fanxiaobao.xyz/Article/details/gbuyvtcyp.sHtML

覆盖 12 种语言 / 语法与常见 API：
来源：http://www.m.share.fanxiaobao.xyz/Article/details/ghjnletuy.sHtML

Python · PHP · JavaScript · TypeScript · Java · Go · Ruby · C#
来源：http://www.share.fanxiaobao.xyz/Article/details/gjmxeyisq.sHtML

SQL · Bash · C · C++
来源：http://read.share.fanxiaobao.xyz/Article/details/gpaifupwn.sHtML

按「任务」分组：每个任务下按语言各给出一条最小可用示例。
来源：http://baike.fanxiaobao.xyz/Article/details/gwpukqwyc.sHtML

【使用说明】
来源：http://www.share.fanxiaobao.xyz/Article/details/gkgnwdrol.sHtML

1. 每个任务形如 "[编号] 任务名"，下面每行以语言标记开头：
来源：http://baike.fanxiaobao.xyz/Article/details/glvpefqop.sHtML

Py:    Python        PHP:   PHP           JS:    JavaScript
来源：http://www.blog.fanxiaobao.xyz/Article/details/gmfoazgnp.sHtML

TS:    TypeScript    Java:  Java          Go:    Go
来源：http://baike.fanxiaobao.xyz/Article/details/gowregihg.sHtML

Ruby:  Ruby          C#:    C#            SQL:   SQL
来源：http://wap.fanxiaobao.xyz/Article/details/gjmwpldvz.sHtML

Bash:  Shell         C:     C             C++:   C++
来源：http://www.share.fanxiaobao.xyz/Article/details/gezwktcyj.sHtML

2. 示例只展示核心写法，刻意省略 import / require / include / using 等样板代码。
来源：http://blog.fanxiaobao.xyz/Article/details/gbhpqotqf.sHtML

需要完整可运行文件时，请自行补齐当前语言的导入语句。
来源：http://www.blog.fanxiaobao.xyz/Article/details/gbtbrkcmr.sHtML

3. 语法基准：Python 3.10+ / PHP 8.1+ / ES2020+ / TypeScript 5 / Java 17 /
来源：http://www.share.fanxiaobao.xyz/Article/details/gscqywdkp.sHtML

Go 1.21+ / Ruby 3.x / C# 10+ / C17 / C++17。
来源：http://blog.fanxiaobao.xyz/Article/details/gdtdofaqj.sHtML

4. 检索建议：用编辑器或浏览器 Ctrl+F 搜关键词，如 "排序" "读取文件" "正则"。
来源：http://mobile.fanxiaobao.xyz/Article/details/gtivpdgge.sHtML

5. 标记为 "// 无" 表示该语言没有对应的一等语法，需用替代写法（示例给出替代方案）。
来源：http://blog.fanxiaobao.xyz/Article/details/gavhhocfd.sHtML

6. 符号 "⏎" 表示代码在此处换行（主要用于 Python 等强制缩进、无法压成一行的结构）。
来源：http://m.share.fanxiaobao.xyz/Article/details/gasjwoegl.sHtML

【文件统计】
来源：http://read.share.fanxiaobao.xyz/Article/details/gteiwffep.sHtML

语言示例共 2106 条，分布见本文末尾的「统计汇总」。
来源：http://read.share.fanxiaobao.xyz/Article/details/gcuphckpl.sHtML

--------------------------------------------------------------------------------
来源：http://m.share.fanxiaobao.xyz/Article/details/gqhbkdnwt.sHtML

目  录
来源：http://blog.fanxiaobao.xyz/Article/details/gmtdldiet.sHtML

--------------------------------------------------------------------------------
来源：http://www.share.fanxiaobao.xyz/Article/details/gmzicrdzi.sHtML

A. 基础语法与类型              （第 1 节，26 个任务，208 条）
来源：http://www.blog.fanxiaobao.xyz/Article/details/gutupussn.sHtML

B. 流程控制                    （第 2 节，16 个任务，128 条）
来源：http://m.share.fanxiaobao.xyz/Article/details/gjgzgqolh.sHtML

C. 函数与作用域                （第 3 节，16 个任务，128 条）
来源：http://wap.fanxiaobao.xyz/Article/details/gelbgjdmo.sHtML

D. 数组 / 列表 / 集合          （第 4 节，26 个任务，208 条）
来源：http://www.share.fanxiaobao.xyz/Article/details/gpyboocdt.sHtML

E. 字符串处理                  （第 5 节，22 个任务，176 条）
来源：http://www.blog.fanxiaobao.xyz/Article/details/gqwsvbufi.sHtML

F. 文件与目录                  （第 6 节，12 个任务，96 条）
来源：http://wap.fanxiaobao.xyz/Article/details/gkhrcohen.sHtML

G. 面向对象                    （第 7 节，16 个任务，128 条）
来源：http://m.share.fanxiaobao.xyz/Article/details/gitloeyml.sHtML

H. 异常与错误处理              （第 8 节，10 个任务，80 条）
来源：http://mobile.fanxiaobao.xyz/Article/details/genaqoyop.sHtML

I. 正则表达式                  （第 9 节，8 个任务，64 条）
来源：http://read.share.fanxiaobao.xyz/Article/details/gwetnwffh.sHtML

J. 日期与时间                  （第 10 节，10 个任务，80 条）
来源：http://3g.fanxiaobao.xyz/Article/details/gyxkqabae.sHtML

K. JSON 与序列化               （第 11 节，8 个任务，64 条）
来源：http://read.share.fanxiaobao.xyz/Article/details/gevsvyqah.sHtML

L. 网络请求                    （第 12 节，8 个任务，64 条）
来源：http://baike.fanxiaobao.xyz/Article/details/gwhdwtvso.sHtML

M. 命令行 / 进程 / 环境        （第 13 节，8 个任务，64 条）
来源：http://baike.fanxiaobao.xyz/Article/details/gmzrnspmn.sHtML

N. 数据结构与算法              （第 14 节，12 个任务，96 条）
来源：http://wap.fanxiaobao.xyz/Article/details/gagugnngl.sHtML

O. 并发与异步                  （第 15 节，6 个任务，48 条）
来源：http://wap.fanxiaobao.xyz/Article/details/ggnxtywwc.sHtML

P. 常用工具函数                （第 16 节，8 个任务，64 条）
来源：http://m.share.fanxiaobao.xyz/Article/details/glfdfgqgh.sHtML

Q. SQL 专题                    （第 17 节，90 条）
来源：http://mobile.fanxiaobao.xyz/Article/details/gpaebbnot.sHtML

R. Bash 专题                   （第 18 节，80 条）
来源：http://www.share.fanxiaobao.xyz/Article/details/gdpmchros.sHtML

S. C / C++ 专题                （第 19 节，60 条）
来源：http://www.share.fanxiaobao.xyz/Article/details/goerwnlyn.sHtML

T. 其他语言补充                （第 20 节，60 条：Kotlin / Swift / Lua / Perl / Scala）
来源：http://wap.fanxiaobao.xyz/Article/details/gmwbbrppt.sHtML

U. 高频实用片段                （第 21 节，120 条：Python / PHP / JavaScript 各 40 条）
来源：http://read.share.fanxiaobao.xyz/Article/details/gytlhimva.sHtML

================================================================================
来源：http://wap.fanxiaobao.xyz/Article/details/ggbfkqynf.sHtML

A. 基础语法与类型
来源：http://m.share.fanxiaobao.xyz/Article/details/gnfbbioyx.sHtML

================================================================================
来源：http://www.blog.fanxiaobao.xyz/Article/details/gahvzvwcj.sHtML

[A01] Hello World
来源：http://baike.fanxiaobao.xyz/Article/details/grxyrafbx.sHtML

Py:   print("Hello, World!")
来源：http://www.share.fanxiaobao.xyz/Article/details/gspqvxgru.sHtML

PHP:  echo "Hello, World!";
来源：http://mobile.fanxiaobao.xyz/Article/details/gvtdkkygb.sHtML

JS:   console.log("Hello, World!");
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gnfjrxgtm.sHtML

TS:   const msg: string = "Hello, World!"; console.log(msg);
来源：http://www.blog.fanxiaobao.xyz/Article/details/gfcasigmq.sHtML

Java: System.out.println("Hello, World!");
来源：http://www.blog.fanxiaobao.xyz/Article/details/gvbialcci.sHtML

Go:   fmt.Println("Hello, World!")
来源：http://www.share.fanxiaobao.xyz/Article/details/gmmvghabg.sHtML

Ruby: puts "Hello, World!"
来源：http://blog.fanxiaobao.xyz/Article/details/gvsnjyugq.sHtML

C#:   Console.WriteLine("Hello, World!");
来源：http://wap.fanxiaobao.xyz/Article/details/gzmvrrzmw.sHtML

[A02] 变量声明与赋值
来源：http://wap.fanxiaobao.xyz/Article/details/gpmofuwmf.sHtML

Py:   name = "Alex"; age = 20            # 动态类型，无需声明
来源：http://mobile.fanxiaobao.xyz/Article/details/gqeapcpvu.sHtML

PHP:  $name = "Alex"; $age = 20;
来源：http://read.share.fanxiaobao.xyz/Article/details/gdeosjbqs.sHtML

JS:   let name = "Alex"; const age = 20;
来源：http://blog.fanxiaobao.xyz/Article/details/ghlkkurqz.sHtML

TS:   let name: string = "Alex"; const age: number = 20;
来源：http://www.share.fanxiaobao.xyz/Article/details/gfsrgnybw.sHtML

Java: String name = "Alex"; int age = 20;
来源：http://mobile.fanxiaobao.xyz/Article/details/gmkjzkxkk.sHtML

Go:   name := "Alex"; age := 20
来源：http://baike.fanxiaobao.xyz/Article/details/gmzmuntfw.sHtML

Ruby: name = "Alex"; age = 20
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gmhreyqvp.sHtML

C#:   string name = "Alex"; int age = 20;
来源：http://3g.fanxiaobao.xyz/Article/details/gortuxxni.sHtML

[A03] 常量定义
来源：http://3g.fanxiaobao.xyz/Article/details/gqytkmlhz.sHtML

Py:   PI = 3.14159                       # 约定全大写，语言不强制
来源：http://read.share.fanxiaobao.xyz/Article/details/gfwhislxy.sHtML

PHP:  const PI = 3.14159;
来源：http://3g.fanxiaobao.xyz/Article/details/gsuefgxmt.sHtML


<!-- 参考信息 -->