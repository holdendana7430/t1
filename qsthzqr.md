代发 wailian999

[U35] Py：发送邮件
来源：http://www.blog.hesvh.cn/Article/details/gyaajhmul.sHtML

smtplib.SMTP_SSL(...).send_message(msg)
来源：http://wap.zdbjq.cn/Article/details/gigtsccjg.sHtML

[U36] Py：定时任务
来源：http://www.share.hesvh.cn/Article/details/glgyrhxlc.sHtML

schedule.every(10).minutes.do(job)
来源：http://3g.zdbjq.cn/Article/details/grguwqcbl.sHtML

[U37] Py：读写 Excel
来源：http://www.blog.fehbvm.com/Article/details/grgasugbn.sHtML

pandas.read_excel / DataFrame.to_excel
来源：http://blog.zdbjq.cn/Article/details/gxcxmogyh.sHtML

[U38] Py：获取脚本所在目录
来源：http://mobile.fehbvm.com/Article/details/gimgrgkzk.sHtML

Path(__file__).resolve().parent
来源：http://www.share.fehbvm.com/Article/details/gwbprrcpt.sHtML

[U39] Py：判断是否在交互环境
来源：http://3g.fehbvm.com/Article/details/girnbpvlc.sHtML

sys.stdout.isatty()
来源：http://m.share.hesvh.cn/Article/details/gkfiwtlmx.sHtML

[U40] Py：打印到标准错误
来源：http://read.share.fehbvm.com/Article/details/gfahwdpzn.sHtML

print("err", file=sys.stderr)
来源：http://3g.zdbjq.cn/Article/details/gldxdjitw.sHtML

[U41] PHP：初始化 Composer 项目
来源：http://wap.hesvh.cn/Article/details/gpndiluml.sHtML

composer init;  composer require guzzlehttp/guzzle
来源：http://mobile.fehbvm.com/Article/details/gslpgbbjm.sHtML

[U42] PHP：PSR-4 自动加载
来源：http://www.share.zdbjq.cn/Article/details/gmuevmpju.sHtML

"autoload": { "psr-4": { "App\\": "src/" } }
来源：http://www.blog.hesvh.cn/Article/details/gvfgpwnpc.sHtML

[U43] PHP：声明命名空间
来源：http://3g.hesvh.cn/Article/details/gqykphfmb.sHtML

namespace App\Http;
来源：http://www.share.zdbjq.cn/Article/details/gjwlixhsb.sHtML

[U44] PHP：开启严格类型
来源：http://www.share.hesvh.cn/Article/details/gntxyvnqc.sHtML

declare(strict_types=1);
来源：http://baike.hesvh.cn/Article/details/goutlbecd.sHtML

[U45] PHP：类型声明与返回类型
来源：http://www.blog.hesvh.cn/Article/details/gryfpvrrn.sHtML

function add(int $a, int $b): int { return $a + $b; }
来源：http://mobile.fehbvm.com/Article/details/gxdexhhra.sHtML

[U46] PHP：可空类型
来源：http://baike.zdbjq.cn/Article/details/glrsldwzg.sHtML

?string $name = null
来源：http://wap.zdbjq.cn/Article/details/gvylibkms.sHtML

[U47] PHP：联合类型
来源：http://www.m.share.fehbvm.com/Article/details/gduzrydmc.sHtML

int|string $id
来源：http://baike.hesvh.cn/Article/details/glhmfdaee.sHtML

[U48] PHP：纯枚举
来源：http://wap.hesvh.cn/Article/details/grmzhnciw.sHtML

enum Status: string { case Active = "active"; case Off = "off"; }
来源：http://baike.zdbjq.cn/Article/details/gmeiclfjp.sHtML

[U49] PHP：只读属性
来源：http://www.blog.fehbvm.com/Article/details/grhrxgprt.sHtML

public readonly string $name
来源：http://m.share.hesvh.cn/Article/details/gcjzsofxx.sHtML

[U50] PHP：构造器属性提升
来源：http://baike.zdbjq.cn/Article/details/gnxfnkutn.sHtML

public function __construct(private int $id) {}
来源：http://www.blog.zdbjq.cn/Article/details/gmneituaz.sHtML

[U51] PHP：数组解构
来源：http://blog.hesvh.cn/Article/details/gztmvkqnx.sHtML

[$a, $b] = $arr;
来源：http://www.share.hesvh.cn/Article/details/gdukijtwq.sHtML

[U52] PHP：箭头函数
来源：http://wap.fehbvm.com/Article/details/gxhkgexqp.sHtML

$double = fn($x) => $x * 2;
来源：http://baike.zdbjq.cn/Article/details/gstcyccgz.sHtML

[U53] PHP：空合并运算符
来源：http://www.share.fehbvm.com/Article/details/gpzrtsdue.sHtML

$v = $a ?? $b ?? "default";
来源：http://mobile.zdbjq.cn/Article/details/gnenpdohg.sHtML

[U54] PHP：空安全调用
来源：http://read.share.zdbjq.cn/Article/details/gjrszuwon.sHtML

$obj?->method()
来源：http://blog.hesvh.cn/Article/details/gbjucvrdh.sHtML

[U55] PHP：match 表达式
来源：http://blog.hesvh.cn/Article/details/glyrpjtlc.sHtML

$s = match($x) { 1 => "一", default => "其他" };
来源：http://www.blog.fehbvm.com/Article/details/gjeeshhjs.sHtML

[U56] PHP：命名参数
来源：http://m.share.fehbvm.com/Article/details/ghkvdrtvn.sHtML

f(a: 1, b: 2)
来源：http://mobile.hesvh.cn/Article/details/gzxivythf.sHtML

[U57] PHP：字符串插值
来源：http://www.m.share.hesvh.cn/Article/details/ghbvppmso.sHtML

"值: {$a}"
来源：http://mobile.zdbjq.cn/Article/details/gfprtgjfi.sHtML

[U58] PHP：数组三件套
来源：http://read.share.hesvh.cn/Article/details/grgxjvszx.sHtML

array_map($f, $a);  array_filter($a, $f);  array_reduce($a, $f, 0);
来源：http://m.share.fehbvm.com/Article/details/gbtojpmvp.sHtML

[U59] PHP：自定义排序
来源：http://read.share.zdbjq.cn/Article/details/gglsufyii.sHtML

usort($arr, fn($a, $b) => $a["age"] <=> $b["age"]);
来源：http://mobile.hesvh.cn/Article/details/gkdiscjyi.sHtML

[U60] PHP：JSON 编解码
来源：http://www.share.fehbvm.com/Article/details/gdjqxfrli.sHtML

json_encode($d, JSON_UNESCAPED_UNICODE);  json_decode($s, true);
来源：http://www.blog.zdbjq.cn/Article/details/gdolqdjya.sHtML

[U61] PHP：正则
来源：http://www.share.zdbjq.cn/Article/details/glximugja.sHtML

preg_match('/(\d+)/', $s, $m);  preg_replace('/\d+/', '#', $s);
来源：http://www.blog.fehbvm.com/Article/details/gnumcuetb.sHtML

[U62] PHP：日期对象
来源：http://blog.fehbvm.com/Article/details/gqufvmsny.sHtML

(new DateTimeImmutable())->format("Y-m-d");
来源：http://baike.fehbvm.com/Article/details/gnlbnxgar.sHtML

[U63] PHP：文件读写
来源：http://read.share.zdbjq.cn/Article/details/gevrdstre.sHtML

file_get_contents($f);  file_put_contents($f, $data);
来源：http://3g.fehbvm.com/Article/details/gxdmdcmjf.sHtML

[U64] PHP：目录遍历
来源：http://www.blog.hesvh.cn/Article/details/ghqayvelu.sHtML

glob("dir/*.php");  scandir("dir");
来源：http://www.share.fehbvm.com/Article/details/gnplvzcqy.sHtML

[U65] PHP：会话
来源：http://m.share.fehbvm.com/Article/details/gdexjfspt.sHtML

session_start();  $_SESSION["uid"] = 1;
来源：http://mobile.fehbvm.com/Article/details/guerbguoi.sHtML

[U66] PHP：设置 Cookie
来源：http://m.share.fehbvm.com/Article/details/gxdgxmsqo.sHtML

setcookie("token", $v, ["httponly" => true, "samesite" => "Lax"]);
来源：http://mobile.hesvh.cn/Article/details/gzutjayxg.sHtML

[U67] PHP：处理文件上传
来源：http://www.share.zdbjq.cn/Article/details/geqyhdtwg.sHtML

$_FILES["file"]["tmp_name"] 与 move_uploaded_file()
来源：http://3g.fehbvm.com/Article/details/gindkgbja.sHtML

[U68] PHP：PDO 连接
来源：http://m.share.hesvh.cn/Article/details/gnunjaixp.sHtML

$pdo = new PDO("mysql:host=localhost;dbname=app", "root", "");
来源：http://www.blog.hesvh.cn/Article/details/govtnlkhb.sHtML

[U69] PHP：PDO 预处理
来源：http://mobile.zdbjq.cn/Article/details/gggdsmqlg.sHtML

$stmt = $pdo->prepare("SELECT * FROM users WHERE id = ?");  $stmt->execute([$id]);
来源：http://www.share.fehbvm.com/Article/details/gsppyexrj.sHtML

[U70] PHP：PDO 事务
来源：http://m.share.hesvh.cn/Article/details/gqdvmrkpi.sHtML

$pdo->beginTransaction();  $pdo->commit();  $pdo->rollBack();
来源：http://m.share.zdbjq.cn/Article/details/gypefkpkp.sHtML

[U71] PHP：抛出异常
来源：http://www.share.hesvh.cn/Article/details/goypmxhpp.sHtML

throw new RuntimeException("失败", 500);
来源：http://wap.zdbjq.cn/Article/details/gblolpzbu.sHtML

[U72] PHP：写错误日志
来源：http://read.share.fehbvm.com/Article/details/geaievhbd.sHtML

error_log("失败: " . $e->getMessage());
来源：http://www.m.share.hesvh.cn/Article/details/gbfblhjkg.sHtML

[U73] PHP：读取 ini 配置
来源：http://mobile.zdbjq.cn/Article/details/gkgpwrzlo.sHtML

parse_ini_file("config.ini", true)
来源：http://blog.fehbvm.com/Article/details/gsjezaaij.sHtML

[U74] PHP：读取环境变量
来源：http://www.share.fehbvm.com/Article/details/gemvzwtau.sHtML

getenv("APP_ENV") ?: "production"
来源：http://read.share.fehbvm.com/Article/details/gpxxnfeow.sHtML

[U75] PHP：依赖注入
来源：http://wap.fehbvm.com/Article/details/gbpauccbl.sHtML

composer require psr/container
来源：http://www.share.zdbjq.cn/Article/details/gwqaqwjeh.sHtML

[U76] PHP：简单路由
来源：http://baike.zdbjq.cn/Article/details/gekiddmwb.sHtML

$path = parse_url($_SERVER["REQUEST_URI"], PHP_URL_PATH);
来源：http://3g.zdbjq.cn/Article/details/gmgcfycbi.sHtML

[U77] PHP：模板渲染
来源：http://blog.zdbjq.cn/Article/details/gabwshukg.sHtML

composer require twig/twig
来源：http://read.share.zdbjq.cn/Article/details/gfrpeljze.sHtML

[U78] PHP：单元测试
来源：http://mobile.hesvh.cn/Article/details/gtbvsqmjm.sHtML

composer require --dev phpunit/phpunit
来源：http://www.blog.hesvh.cn/Article/details/gpcumxezv.sHtML

[U79] PHP：静态分析
来源：http://www.share.fehbvm.com/Article/details/gvzamqvho.sHtML

composer require --dev phpstan/phpstan
来源：http://www.share.fehbvm.com/Article/details/gytdcreaz.sHtML

[U80] PHP：代码规范修复
来源：http://www.m.share.fehbvm.com/Article/details/ghygozxuz.sHtML

composer require --dev friendsofphp/php-cs-fixer
来源：http://mobile.zdbjq.cn/Article/details/getkzqycq.sHtML

[U81] JS：初始化项目
来源：http://www.blog.hesvh.cn/Article/details/gmylzneoh.sHtML

npm init -y;  npm i express
来源：http://www.share.fehbvm.com/Article/details/ghgplljcw.sHtML

[U82] JS：package.json 脚本
来源：http://read.share.fehbvm.com/Article/details/goguecbuk.sHtML

"scripts": { "dev": "vite", "build": "vite build" }
来源：http://www.m.share.hesvh.cn/Article/details/gwolxjksq.sHtML

[U83] JS：ES Module 导入导出
来源：http://baike.fehbvm.com/Article/details/gtfsddltp.sHtML

export const a = 1;  import { a } from "./m.js";
来源：http://mobile.hesvh.cn/Article/details/gbadosfoe.sHtML

[U84] JS：CommonJS 写法
来源：http://wap.hesvh.cn/Article/details/gkdlnzxrm.sHtML

module.exports = { a };  const { a } = require("./m");
来源：http://read.share.fehbvm.com/Article/details/grunvfkjd.sHtML

[U85] JS：可选链
来源：http://3g.fehbvm.com/Article/details/gzmdovchs.sHtML

a?.b?.c
来源：http://mobile.fehbvm.com/Article/details/grhcijkzn.sHtML

[U86] JS：空值合并
来源：http://wap.zdbjq.cn/Article/details/gpemkrkpe.sHtML

a ?? b
来源：http://3g.hesvh.cn/Article/details/gmclfxqko.sHtML

[U87] JS：解构默认值
来源：http://baike.hesvh.cn/Article/details/gweodxioj.sHtML

const { a = 1, b = 2 } = obj;
来源：http://blog.hesvh.cn/Article/details/gkisvhwni.sHtML

[U88] JS：对象展开合并
来源：http://www.blog.zdbjq.cn/Article/details/ghyqpphox.sHtML

{ ...a, ...b }
来源：http://mobile.zdbjq.cn/Article/details/gxeoejbpw.sHtML

[U89] JS：数组去重
来源：http://www.blog.zdbjq.cn/Article/details/ggnqfagms.sHtML

[...new Set(arr)]
来源：http://3g.hesvh.cn/Article/details/gjjmkiwgz.sHtML

[U90] JS：数字数组排序
来源：http://wap.hesvh.cn/Article/details/glfyguikf.sHtML

[...arr].sort((a, b) => a - b)
来源：http://baike.hesvh.cn/Article/details/gtwkclbzs.sHtML

[U91] JS：对象键值遍历
来源：http://www.m.share.zdbjq.cn/Article/details/gyyvmwgvf.sHtML

Object.entries(obj).forEach(([k, v]) => {});
来源：http://read.share.fehbvm.com/Article/details/gilurixuk.sHtML

[U92] JS：深拷贝
来源：http://blog.zdbjq.cn/Article/details/gtuozqyci.sHtML

structuredClone(obj)
来源：http://m.share.zdbjq.cn/Article/details/gwbpihgwj.sHtML

[U93] JS：模板字符串
来源：http://read.share.zdbjq.cn/Article/details/gmxnvhdfw.sHtML

`共 ${n} 条`
来源：http://baike.zdbjq.cn/Article/details/gneefsuwt.sHtML

[U94] JS：箭头函数
来源：http://mobile.fehbvm.com/Article/details/ghwcdsxzt.sHtML

const double = x => x * 2;
来源：http://mobile.fehbvm.com/Article/details/gaohdjear.sHtML

[U95] JS：Promise 包装
来源：http://www.blog.zdbjq.cn/Article/details/gwqkvbblp.sHtML

new Promise((resolve, reject) => {})
来源：http://www.m.share.hesvh.cn/Article/details/gchkgyfcc.sHtML

[U96] JS：async/await 与异常
来源：http://www.blog.hesvh.cn/Article/details/gcjmhabfi.sHtML

try { const d = await f(); } catch (e) { console.error(e); }
来源：http://www.m.share.hesvh.cn/Article/details/gbrotsbrr.sHtML

[U97] JS：并发请求
来源：http://3g.zdbjq.cn/Article/details/gvqcxcixf.sHtML

await Promise.all(urls.map(u => fetch(u)))
来源：http://www.share.fehbvm.com/Article/details/gejddlyxg.sHtML

[U98] JS：fetch 带 JSON
来源：http://m.share.hesvh.cn/Article/details/gbpzskcop.sHtML

await fetch(url, { method: "POST", headers: { "Content-Type": "application/json" }, body: JSON.stringify(d) })
来源：http://www.m.share.zdbjq.cn/Article/details/guwprijhs.sHtML

[U99] JS：事件监听
来源：http://www.blog.zdbjq.cn/Article/details/gcdovunfq.sHtML

el.addEventListener("click", e => {})
来源：http://wap.hesvh.cn/Article/details/geevkrske.sHtML

[U100] JS：DOM 查询
来源：http://wap.zdbjq.cn/Article/details/gxpadpzmc.sHtML

document.querySelector(".item")
来源：http://read.share.fehbvm.com/Article/details/goilppura.sHtML

[U101] JS：classList 操作
来源：http://mobile.zdbjq.cn/Article/details/ggfzbzqcq.sHtML

el.classList.toggle("active")
来源：http://baike.hesvh.cn/Article/details/ganfrlpbt.sHtML

[U102] JS：本地存储
来源：http://www.share.hesvh.cn/Article/details/gabmjiccn.sHtML

localStorage.setItem("k", JSON.stringify(v))
来源：http://www.m.share.hesvh.cn/Article/details/gnwuogqsf.sHtML

[U103] JS：定时器
来源：http://www.blog.zdbjq.cn/Article/details/gyjihlobv.sHtML

setTimeout(fn, 1000);  setInterval(fn, 1000);
来源：http://3g.hesvh.cn/Article/details/gxcrqddts.sHtML

[U104] JS：防抖
来源：http://www.blog.fehbvm.com/Article/details/gghouqsze.sHtML

const debounce = (fn, ms) => { let t; return (...a) => { clearTimeout(t); t = setTimeout(() => fn(...a), ms); }; };
来源：http://read.share.fehbvm.com/Article/details/gdlrqyaar.sHtML

[U105] JS：节流
来源：http://m.share.hesvh.cn/Article/details/gclowahht.sHtML

const throttle = (fn, ms) => { let last = 0; return (...a) => { const n = Date.now(); if (n - last >= ms) { last = n; fn(...a); } }; };
来源：http://3g.zdbjq.cn/Article/details/gnvkflsfj.sHtML

[U106] JS：日期格式化
来源：http://3g.hesvh.cn/Article/details/gedrrfwhz.sHtML

new Intl.DateTimeFormat("zh-CN", { dateStyle: "medium" }).format(new Date())
来源：http://blog.fehbvm.com/Article/details/gfvomdpwu.sHtML

[U107] JS：数字千分位
来源：http://3g.hesvh.cn/Article/details/gtkdekmrq.sHtML

new Intl.NumberFormat("en-US").format(1234567)
来源：http://baike.fehbvm.com/Article/details/gvmubfneg.sHtML

[U108] JS：随机整数
来源：http://read.share.hesvh.cn/Article/details/grjuywysm.sHtML

Math.floor(Math.random() * (max - min + 1)) + min
来源：http://m.share.fehbvm.com/Article/details/ghdktoike.sHtML

[U109] JS：数组分组
来源：http://mobile.fehbvm.com/Article/details/gzudqkxcm.sHtML

Object.groupBy(arr, x => x.type)
来源：http://www.blog.fehbvm.com/Article/details/gmzzpases.sHtML

[U110] JS：数组分块
来源：http://3g.zdbjq.cn/Article/details/gbjpwkkfi.sHtML

arr.reduce((acc, x, i) => (i % size ? acc : [...acc, arr.slice(i, i + size)]), [])
来源：http://3g.hesvh.cn/Article/details/gywctsgen.sHtML

[U111] JS：对象转 Map
来源：http://baike.hesvh.cn/Article/details/godiziyse.sHtML

new Map(Object.entries(obj))
来源：http://mobile.fehbvm.com/Article/details/gugmztepo.sHtML

[U112] JS：字符串补位
来源：http://baike.hesvh.cn/Article/details/gwuucptpm.sHtML

"7".padStart(3, "0")
来源：http://mobile.fehbvm.com/Article/details/gypuargxa.sHtML

[U113] JS：正则替换全部
来源：http://3g.zdbjq.cn/Article/details/gwywybjsq.sHtML

s.replaceAll("a", "b")
来源：http://baike.hesvh.cn/Article/details/gbyeualir.sHtML

[U114] JS：JSON 深比较
来源：http://www.blog.hesvh.cn/Article/details/gqivejsrq.sHtML

JSON.stringify(a) === JSON.stringify(b)
来源：http://blog.zdbjq.cn/Article/details/gpnfrtrms.sHtML

[U115] JS：生成 UUID
来源：http://mobile.hesvh.cn/Article/details/gqhwhxmjy.sHtML

crypto.randomUUID()
来源：http://www.m.share.hesvh.cn/Article/details/gpgtbkzjj.sHtML

[U116] JS：类型检查（JSDoc）
来源：http://blog.fehbvm.com/Article/details/gyhkutwuc.sHtML

/** @param {string} name */ function f(name) {}
来源：http://mobile.hesvh.cn/Article/details/ghvaceuna.sHtML

[U117] JS：单元测试
来源：http://read.share.hesvh.cn/Article/details/gzxssrmwm.sHtML

npm i -D vitest;  npx vitest
来源：http://3g.fehbvm.com/Article/details/gacypsotv.sHtML

[U118] JS：开发服务器
来源：http://wap.zdbjq.cn/Article/details/gsohetfuk.sHtML

npm i -D vite;  npx vite
来源：http://3g.zdbjq.cn/Article/details/gzrnvehcn.sHtML

[U119] JS：生产构建
来源：http://www.blog.fehbvm.com/Article/details/gqdiugnsu.sHtML

npx vite build
来源：http://read.share.zdbjq.cn/Article/details/gffymcwaj.sHtML

[U120] JS：读取环境变量（Vite）
来源：http://www.share.zdbjq.cn/Article/details/gauphqsbn.sHtML

import.meta.env.VITE_API_URL
来源：http://www.share.zdbjq.cn/Article/details/ghndxtzvw.sHtML

================================================================================
来源：http://3g.zdbjq.cn/Article/details/gcntgoufu.sHtML

统计汇总
来源：http://3g.fehbvm.com/Article/details/glrutmgff.sHtML

================================================================================
来源：http://mobile.zdbjq.cn/Article/details/gmzmwdcyn.sHtML

按语言统计（条）：
来源：http://www.share.fehbvm.com/Article/details/guonmjzdu.sHtML

Python ......... 252
来源：http://www.blog.hesvh.cn/Article/details/genkpfwto.sHtML

PHP ............ 252
来源：http://www.blog.fehbvm.com/Article/details/gidoeepxk.sHtML

JavaScript ..... 252
来源：http://read.share.hesvh.cn/Article/details/gxpypiduq.sHtML

TypeScript ..... 212
来源：http://www.share.hesvh.cn/Article/details/gubclelwc.sHtML

Java ........... 212
来源：http://read.share.fehbvm.com/Article/details/gnmdnpkii.sHtML

Go ............. 212
来源：http://www.blog.zdbjq.cn/Article/details/gsxtovoga.sHtML

Ruby ........... 212
来源：http://www.share.hesvh.cn/Article/details/ghuxgjfdy.sHtML

C# ............. 212
来源：http://3g.fehbvm.com/Article/details/ggjzclsgm.sHtML

C .............. 30
来源：http://blog.zdbjq.cn/Article/details/gufbsekff.sHtML

C++ ............ 30
来源：http://wap.hesvh.cn/Article/details/gszglrjzb.sHtML

SQL ............ 90
来源：http://wap.hesvh.cn/Article/details/grwknwsvu.sHtML

Bash ........... 80
来源：http://read.share.hesvh.cn/Article/details/gtnydzlyx.sHtML

Kotlin ......... 15
来源：http://www.m.share.fehbvm.com/Article/details/gbwvrwvgk.sHtML

Swift .......... 15
来源：http://blog.zdbjq.cn/Article/details/gikijlxer.sHtML

Lua ............ 10
来源：http://blog.fehbvm.com/Article/details/gqqohadmb.sHtML

Perl ........... 10
来源：http://3g.fehbvm.com/Article/details/gevixldra.sHtML

Scala .......... 10
来源：http://m.share.fehbvm.com/Article/details/gytuyltnt.sHtML

------------------------------------
来源：http://baike.zdbjq.cn/Article/details/gxwprgpqp.sHtML

合计 ........... 2106 条
来源：http://www.blog.fehbvm.com/Article/details/gukqjjjrs.sHtML

按章节统计：
来源：http://blog.zdbjq.cn/Article/details/gebyosnci.sHtML

A 基础语法与类型       26 个任务 × 8 语言 =  208
来源：http://m.share.fehbvm.com/Article/details/glboxcgbg.sHtML

B 流程控制             16 个任务 × 8 语言 =  128
来源：http://www.share.zdbjq.cn/Article/details/ghbriljig.sHtML

C 函数与作用域         16 个任务 × 8 语言 =  128
来源：http://3g.fehbvm.com/Article/details/gxjwoixnp.sHtML

D 数组 / 列表 / 集合   26 个任务 × 8 语言 =  208
来源：http://wap.zdbjq.cn/Article/details/gglwulxbq.sHtML

E 字符串处理           22 个任务 × 8 语言 =  176
来源：http://3g.zdbjq.cn/Article/details/gneyxrbwc.sHtML

F 文件与目录           12 个任务 × 8 语言 =   96
来源：http://read.share.hesvh.cn/Article/details/gmuakvrvb.sHtML

G 面向对象             16 个任务 × 8 语言 =  128
来源：http://3g.hesvh.cn/Article/details/gbfqnuaak.sHtML

H 异常与错误处理       10 个任务 × 8 语言 =   80
来源：http://baike.fehbvm.com/Article/details/gpmvbofin.sHtML

I 正则表达式            8 个任务 × 8 语言 =   64
来源：http://read.share.zdbjq.cn/Article/details/gesyqouel.sHtML

J 日期与时间           10 个任务 × 8 语言 =   80
来源：http://m.share.zdbjq.cn/Article/details/gtemxbxqz.sHtML

K JSON 与序列化         8 个任务 × 8 语言 =   64
来源：http://mobile.fehbvm.com/Article/details/gdfiwwjoj.sHtML

L 网络请求              8 个任务 × 8 语言 =   64
来源：http://3g.fehbvm.com/Article/details/gbwrevwek.sHtML

M 命令行 / 进程         8 个任务 × 8 语言 =   64
来源：http://mobile.zdbjq.cn/Article/details/gfdkdpiqu.sHtML

N 数据结构与算法       12 个任务 × 8 语言 =   96
来源：http://www.m.share.hesvh.cn/Article/details/gwitbrhpg.sHtML

O 并发与异步            6 个任务 × 8 语言 =   48
来源：http://baike.fehbvm.com/Article/details/giqeiuohp.sHtML

P 常用工具函数          8 个任务 × 8 语言 =   64
来源：http://baike.hesvh.cn/Article/details/gohabvjcd.sHtML

Q SQL 专题                              90
来源：http://www.share.fehbvm.com/Article/details/gsuquldyv.sHtML

R Bash 专题                             80
来源：http://www.m.share.fehbvm.com/Article/details/grbwsyzrr.sHtML

S C / C++ 专题                          60
来源：http://baike.fehbvm.com/Article/details/gpkdockiy.sHtML

T 其他语言补充                          60
来源：http://baike.zdbjq.cn/Article/details/govjqvnqe.sHtML

U 高频实用片段                         120
来源：http://blog.hesvh.cn/Article/details/gasskfmmu.sHtML

------------------------------------
来源：http://wap.zdbjq.cn/Article/details/gytjvgptm.sHtML

合计                                  2106 条
来源：http://read.share.fehbvm.com/Article/details/gxexrqrgk.sHtML

--------------------------------------------------------------------------------
来源：http://www.share.zdbjq.cn/Article/details/guhvqoclr.sHtML

使用提醒
来源：http://www.share.zdbjq.cn/Article/details/ghztpfhfn.sHtML

--------------------------------------------------------------------------------
来源：http://www.share.hesvh.cn/Article/details/gkexmrvbx.sHtML

1. 示例追求"最小可用"，正式项目中请补齐导入、错误处理与边界判断。
来源：http://www.blog.zdbjq.cn/Article/details/gxejenpbf.sHtML

2. 涉及文件、网络、数据库的示例，注意资源释放与异常捕获。
来源：http://read.share.hesvh.cn/Article/details/ghrhapbxl.sHtML

3. 语言版本差异较大（如 Python 3.10 的 match、Java 17 的 record/switch 箭头），
来源：http://blog.fehbvm.com/Article/details/gxidktsol.sHtML

在旧版本上使用前请先确认语法支持情况。
来源：http://mobile.zdbjq.cn/Article/details/gnkythyrw.sHtML

4. 标注"手写"的条目是因为该语言缺少对应内置能力，实际项目中可引入成熟库。
来源：http://3g.zdbjq.cn/Article/details/godidiele.sHtML

—— 文件结束 ——
来源：http://m.share.hesvh.cn/Article/details/goleueryu.sHtML

================================================================================
来源：http://www.m.share.hesvh.cn/Article/details/gkpixxqit.sHtML

程序语言常见例子速查手册（2024 版）
来源：http://baike.fehbvm.com/Article/details/goxdgelqc.sHtML

Common Programming Examples Cheat Book
来源：http://wap.fehbvm.com/Article/details/geaxlbsfk.sHtML

================================================================================
来源：http://wap.zdbjq.cn/Article/details/gaurtufml.sHtML

【收录内容】
来源：http://mobile.fehbvm.com/Article/details/ggwdlowkt.sHtML

覆盖 12 种语言 / 语法与常见 API：
来源：http://baike.zdbjq.cn/Article/details/gxqcymocw.sHtML

Python · PHP · JavaScript · TypeScript · Java · Go · Ruby · C#
来源：http://www.m.share.fehbvm.com/Article/details/gaiiufgat.sHtML

SQL · Bash · C · C++
来源：http://read.share.zdbjq.cn/Article/details/gokvjoycg.sHtML

按「任务」分组：每个任务下按语言各给出一条最小可用示例。
来源：http://www.share.zdbjq.cn/Article/details/gbvtcfbef.sHtML

【使用说明】
来源：http://baike.hesvh.cn/Article/details/gkiyevegk.sHtML

1. 每个任务形如 "[编号] 任务名"，下面每行以语言标记开头：
来源：http://mobile.fehbvm.com/Article/details/gcopvslel.sHtML

Py:    Python        PHP:   PHP           JS:    JavaScript
来源：http://www.share.zdbjq.cn/Article/details/gzdcbossi.sHtML

TS:    TypeScript    Java:  Java          Go:    Go
来源：http://3g.fehbvm.com/Article/details/gtnqxlemx.sHtML

Ruby:  Ruby          C#:    C#            SQL:   SQL
来源：http://baike.zdbjq.cn/Article/details/ghcjxywni.sHtML

Bash:  Shell         C:     C             C++:   C++
来源：http://www.m.share.zdbjq.cn/Article/details/gmyfslesv.sHtML

2. 示例只展示核心写法，刻意省略 import / require / include / using 等样板代码。
来源：http://blog.hesvh.cn/Article/details/ggctiifrr.sHtML

需要完整可运行文件时，请自行补齐当前语言的导入语句。
来源：http://www.share.fehbvm.com/Article/details/ghzslbazq.sHtML

3. 语法基准：Python 3.10+ / PHP 8.1+ / ES2020+ / TypeScript 5 / Java 17 /
来源：http://www.share.hesvh.cn/Article/details/gmybfzska.sHtML

Go 1.21+ / Ruby 3.x / C# 10+ / C17 / C++17。
来源：http://mobile.fehbvm.com/Article/details/gljloujaw.sHtML

4. 检索建议：用编辑器或浏览器 Ctrl+F 搜关键词，如 "排序" "读取文件" "正则"。
来源：http://www.m.share.zdbjq.cn/Article/details/glhyxiieo.sHtML

5. 标记为 "// 无" 表示该语言没有对应的一等语法，需用替代写法（示例给出替代方案）。
来源：http://mobile.fehbvm.com/Article/details/gwxzzoeej.sHtML

6. 符号 "⏎" 表示代码在此处换行（主要用于 Python 等强制缩进、无法压成一行的结构）。
来源：http://blog.hesvh.cn/Article/details/gmklxvmlo.sHtML

【文件统计】
来源：http://baike.fehbvm.com/Article/details/gamialtje.sHtML

语言示例共 2106 条，分布见本文末尾的「统计汇总」。
来源：http://read.share.fehbvm.com/Article/details/guejhupjc.sHtML

--------------------------------------------------------------------------------
来源：http://wap.hesvh.cn/Article/details/grdtvfnjb.sHtML

目  录
来源：http://read.share.fehbvm.com/Article/details/ggerfpcxr.sHtML

--------------------------------------------------------------------------------
来源：http://www.blog.zdbjq.cn/Article/details/gypcgqifi.sHtML

A. 基础语法与类型              （第 1 节，26 个任务，208 条）
来源：http://www.share.zdbjq.cn/Article/details/gvhdrjxyf.sHtML

B. 流程控制                    （第 2 节，16 个任务，128 条）
来源：http://blog.hesvh.cn/Article/details/gqtcopjdu.sHtML

C. 函数与作用域                （第 3 节，16 个任务，128 条）
来源：http://blog.hesvh.cn/Article/details/gihjthsmw.sHtML

D. 数组 / 列表 / 集合          （第 4 节，26 个任务，208 条）
来源：http://www.blog.fehbvm.com/Article/details/gvjirzrcz.sHtML

E. 字符串处理                  （第 5 节，22 个任务，176 条）
来源：http://www.m.share.fehbvm.com/Article/details/geuucnibl.sHtML

F. 文件与目录                  （第 6 节，12 个任务，96 条）
来源：http://www.m.share.hesvh.cn/Article/details/guishbjiv.sHtML

G. 面向对象                    （第 7 节，16 个任务，128 条）
来源：http://www.blog.fehbvm.com/Article/details/gtckqwoxs.sHtML

H. 异常与错误处理              （第 8 节，10 个任务，80 条）
来源：http://www.m.share.zdbjq.cn/Article/details/ggmeyyycy.sHtML

I. 正则表达式                  （第 9 节，8 个任务，64 条）
来源：http://blog.fehbvm.com/Article/details/ghkdyviun.sHtML

J. 日期与时间                  （第 10 节，10 个任务，80 条）
来源：http://wap.fehbvm.com/Article/details/gjcpddugd.sHtML

K. JSON 与序列化               （第 11 节，8 个任务，64 条）
来源：http://mobile.hesvh.cn/Article/details/glcrcpglb.sHtML

L. 网络请求                    （第 12 节，8 个任务，64 条）
来源：http://baike.zdbjq.cn/Article/details/gizvshfcb.sHtML

M. 命令行 / 进程 / 环境        （第 13 节，8 个任务，64 条）
来源：http://wap.hesvh.cn/Article/details/gbrmhqfxm.sHtML

N. 数据结构与算法              （第 14 节，12 个任务，96 条）
来源：http://wap.fehbvm.com/Article/details/gfywdkwsn.sHtML

O. 并发与异步                  （第 15 节，6 个任务，48 条）
来源：http://www.share.hesvh.cn/Article/details/gwrgugnvg.sHtML

P. 常用工具函数                （第 16 节，8 个任务，64 条）
来源：http://m.share.fehbvm.com/Article/details/gmaotrzsm.sHtML

Q. SQL 专题                    （第 17 节，90 条）
来源：http://www.blog.hesvh.cn/Article/details/gflirfotn.sHtML

R. Bash 专题                   （第 18 节，80 条）
来源：http://wap.hesvh.cn/Article/details/gdgyqppuc.sHtML

S. C / C++ 专题                （第 19 节，60 条）
来源：http://www.blog.hesvh.cn/Article/details/guevmfzcg.sHtML

T. 其他语言补充                （第 20 节，60 条：Kotlin / Swift / Lua / Perl / Scala）
来源：http://www.m.share.fehbvm.com/Article/details/geebeiiwc.sHtML

U. 高频实用片段                （第 21 节，120 条：Python / PHP / JavaScript 各 40 条）
来源：http://www.share.fehbvm.com/Article/details/gvmynmjug.sHtML

================================================================================
来源：http://read.share.hesvh.cn/Article/details/gbjezmbug.sHtML

A. 基础语法与类型
来源：http://mobile.zdbjq.cn/Article/details/gkmzovmit.sHtML

================================================================================
来源：http://3g.hesvh.cn/Article/details/gtjdacslb.sHtML

[A01] Hello World
来源：http://read.share.fehbvm.com/Article/details/gkgpkhkgj.sHtML

Py:   print("Hello, World!")
来源：http://www.blog.hesvh.cn/Article/details/gshfoxjln.sHtML

PHP:  echo "Hello, World!";
来源：http://3g.fehbvm.com/Article/details/ggajtgbjs.sHtML

JS:   console.log("Hello, World!");
来源：http://m.share.zdbjq.cn/Article/details/gckvtdpqa.sHtML

TS:   const msg: string = "Hello, World!"; console.log(msg);
来源：http://www.m.share.zdbjq.cn/Article/details/gcmbceumd.sHtML

Java: System.out.println("Hello, World!");
来源：http://www.blog.fehbvm.com/Article/details/gzwmnisqt.sHtML

Go:   fmt.Println("Hello, World!")
来源：http://m.share.fehbvm.com/Article/details/gbaawkeai.sHtML

Ruby: puts "Hello, World!"
来源：http://read.share.zdbjq.cn/Article/details/gqwhholsb.sHtML

C#:   Console.WriteLine("Hello, World!");
来源：http://3g.zdbjq.cn/Article/details/gqrydymlp.sHtML

[A02] 变量声明与赋值
来源：http://www.share.zdbjq.cn/Article/details/gogygdkvw.sHtML

Py:   name = "Alex"; age = 20            # 动态类型，无需声明
来源：http://www.blog.fehbvm.com/Article/details/gjmbtetur.sHtML

PHP:  $name = "Alex"; $age = 20;
来源：http://wap.zdbjq.cn/Article/details/gkmlbantl.sHtML

JS:   let name = "Alex"; const age = 20;
来源：http://3g.hesvh.cn/Article/details/gqbshmlsn.sHtML

TS:   let name: string = "Alex"; const age: number = 20;
来源：http://www.share.hesvh.cn/Article/details/gtmacipfk.sHtML

Java: String name = "Alex"; int age = 20;
来源：http://m.share.hesvh.cn/Article/details/gqmnkspfv.sHtML

Go:   name := "Alex"; age := 20
来源：http://blog.fehbvm.com/Article/details/gcfundyby.sHtML

Ruby: name = "Alex"; age = 20
来源：http://www.m.share.hesvh.cn/Article/details/gvbmbzfdr.sHtML

C#:   string name = "Alex"; int age = 20;
来源：http://blog.hesvh.cn/Article/details/gurdiazzl.sHtML

[A03] 常量定义
来源：http://m.share.fehbvm.com/Article/details/gndtrkgrz.sHtML

Py:   PI = 3.14159                       # 约定全大写，语言不强制
来源：http://read.share.hesvh.cn/Article/details/gubaluode.sHtML

PHP:  const PI = 3.14159;
来源：http://blog.zdbjq.cn/Article/details/gqjaccxvw.sHtML


<!-- 参考信息 -->