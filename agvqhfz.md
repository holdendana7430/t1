代发 wailian999

[U35] Py：发送邮件
来源：http://www.share.hesvh.cn/Article/details/giwwtqeam.sHtML

smtplib.SMTP_SSL(...).send_message(msg)
来源：http://wap.hesvh.cn/Article/details/giztlnstn.sHtML

[U36] Py：定时任务
来源：http://baike.fehbvm.com/Article/details/gxefozhlq.sHtML

schedule.every(10).minutes.do(job)
来源：http://baike.zdbjq.cn/Article/details/glofajmtj.sHtML

[U37] Py：读写 Excel
来源：http://mobile.hesvh.cn/Article/details/gfvlgmcxt.sHtML

pandas.read_excel / DataFrame.to_excel
来源：http://www.share.fehbvm.com/Article/details/gjmzqiiyb.sHtML

[U38] Py：获取脚本所在目录
来源：http://3g.zdbjq.cn/Article/details/grdukelus.sHtML

Path(__file__).resolve().parent
来源：http://read.share.zdbjq.cn/Article/details/gkmzjseib.sHtML

[U39] Py：判断是否在交互环境
来源：http://www.blog.zdbjq.cn/Article/details/gaadvvxvi.sHtML

sys.stdout.isatty()
来源：http://www.blog.fehbvm.com/Article/details/gzhauxasr.sHtML

[U40] Py：打印到标准错误
来源：http://www.share.fehbvm.com/Article/details/gzcvvzott.sHtML

print("err", file=sys.stderr)
来源：http://www.m.share.hesvh.cn/Article/details/gxpuzmxru.sHtML

[U41] PHP：初始化 Composer 项目
来源：http://www.share.hesvh.cn/Article/details/gwuyddmrv.sHtML

composer init;  composer require guzzlehttp/guzzle
来源：http://3g.zdbjq.cn/Article/details/gorsdkaiq.sHtML

[U42] PHP：PSR-4 自动加载
来源：http://www.share.fehbvm.com/Article/details/gmbknakqz.sHtML

"autoload": { "psr-4": { "App\\": "src/" } }
来源：http://www.m.share.zdbjq.cn/Article/details/gldpusqvw.sHtML

[U43] PHP：声明命名空间
来源：http://baike.fehbvm.com/Article/details/gdgorbkvu.sHtML

namespace App\Http;
来源：http://mobile.hesvh.cn/Article/details/gexfvyevu.sHtML

[U44] PHP：开启严格类型
来源：http://baike.hesvh.cn/Article/details/grsamfhuv.sHtML

declare(strict_types=1);
来源：http://www.share.zdbjq.cn/Article/details/gxzfvxnub.sHtML

[U45] PHP：类型声明与返回类型
来源：http://blog.fehbvm.com/Article/details/gtxbfyayb.sHtML

function add(int $a, int $b): int { return $a + $b; }
来源：http://www.share.hesvh.cn/Article/details/gcjlwpwxi.sHtML

[U46] PHP：可空类型
来源：http://read.share.zdbjq.cn/Article/details/ghpzbhizd.sHtML

?string $name = null
来源：http://www.blog.hesvh.cn/Article/details/gvywalysn.sHtML

[U47] PHP：联合类型
来源：http://www.share.hesvh.cn/Article/details/gfblqgrlw.sHtML

int|string $id
来源：http://mobile.hesvh.cn/Article/details/gcvsnxslq.sHtML

[U48] PHP：纯枚举
来源：http://www.share.fehbvm.com/Article/details/grbjkbsve.sHtML

enum Status: string { case Active = "active"; case Off = "off"; }
来源：http://m.share.zdbjq.cn/Article/details/gvqdnoram.sHtML

[U49] PHP：只读属性
来源：http://mobile.zdbjq.cn/Article/details/gxkmstkrj.sHtML

public readonly string $name
来源：http://3g.hesvh.cn/Article/details/grpvhjdrg.sHtML

[U50] PHP：构造器属性提升
来源：http://mobile.hesvh.cn/Article/details/grlljguhp.sHtML

public function __construct(private int $id) {}
来源：http://mobile.zdbjq.cn/Article/details/ghdameqro.sHtML

[U51] PHP：数组解构
来源：http://blog.zdbjq.cn/Article/details/gokuqpfpe.sHtML

[$a, $b] = $arr;
来源：http://m.share.zdbjq.cn/Article/details/gswxcyszw.sHtML

[U52] PHP：箭头函数
来源：http://www.m.share.hesvh.cn/Article/details/gcuzornzg.sHtML

$double = fn($x) => $x * 2;
来源：http://www.blog.hesvh.cn/Article/details/gqbpcuwmr.sHtML

[U53] PHP：空合并运算符
来源：http://www.share.zdbjq.cn/Article/details/gnzpoyfdm.sHtML

$v = $a ?? $b ?? "default";
来源：http://wap.fehbvm.com/Article/details/grtluixzt.sHtML

[U54] PHP：空安全调用
来源：http://mobile.zdbjq.cn/Article/details/gktlwcvgm.sHtML

$obj?->method()
来源：http://www.blog.fehbvm.com/Article/details/ghzpwlqjl.sHtML

[U55] PHP：match 表达式
来源：http://www.blog.hesvh.cn/Article/details/gclsrbhdq.sHtML

$s = match($x) { 1 => "一", default => "其他" };
来源：http://mobile.hesvh.cn/Article/details/gdiyjsrop.sHtML

[U56] PHP：命名参数
来源：http://m.share.hesvh.cn/Article/details/gjfexaxbh.sHtML

f(a: 1, b: 2)
来源：http://www.m.share.hesvh.cn/Article/details/gluwdzghr.sHtML

[U57] PHP：字符串插值
来源：http://blog.hesvh.cn/Article/details/gznkgoeia.sHtML

"值: {$a}"
来源：http://blog.hesvh.cn/Article/details/gcismfcjr.sHtML

[U58] PHP：数组三件套
来源：http://mobile.zdbjq.cn/Article/details/ghhdjbcti.sHtML

array_map($f, $a);  array_filter($a, $f);  array_reduce($a, $f, 0);
来源：http://www.m.share.fehbvm.com/Article/details/gndcvzcbb.sHtML

[U59] PHP：自定义排序
来源：http://baike.zdbjq.cn/Article/details/grswgbili.sHtML

usort($arr, fn($a, $b) => $a["age"] <=> $b["age"]);
来源：http://baike.hesvh.cn/Article/details/gohpvwqtf.sHtML

[U60] PHP：JSON 编解码
来源：http://blog.zdbjq.cn/Article/details/gvoiddint.sHtML

json_encode($d, JSON_UNESCAPED_UNICODE);  json_decode($s, true);
来源：http://m.share.hesvh.cn/Article/details/gktxwraci.sHtML

[U61] PHP：正则
来源：http://baike.hesvh.cn/Article/details/gqboqudtm.sHtML

preg_match('/(\d+)/', $s, $m);  preg_replace('/\d+/', '#', $s);
来源：http://blog.hesvh.cn/Article/details/gxrlmyydr.sHtML

[U62] PHP：日期对象
来源：http://wap.hesvh.cn/Article/details/gtsrkvdkp.sHtML

(new DateTimeImmutable())->format("Y-m-d");
来源：http://www.blog.hesvh.cn/Article/details/gonzlkxfx.sHtML

[U63] PHP：文件读写
来源：http://wap.hesvh.cn/Article/details/gorfqhlwo.sHtML

file_get_contents($f);  file_put_contents($f, $data);
来源：http://blog.fehbvm.com/Article/details/gqcgajdea.sHtML

[U64] PHP：目录遍历
来源：http://wap.hesvh.cn/Article/details/gynhxxudi.sHtML

glob("dir/*.php");  scandir("dir");
来源：http://www.m.share.hesvh.cn/Article/details/ghwenenld.sHtML

[U65] PHP：会话
来源：http://mobile.zdbjq.cn/Article/details/gprkljaos.sHtML

session_start();  $_SESSION["uid"] = 1;
来源：http://blog.fehbvm.com/Article/details/guiymmvzv.sHtML

[U66] PHP：设置 Cookie
来源：http://mobile.fehbvm.com/Article/details/giljihqre.sHtML

setcookie("token", $v, ["httponly" => true, "samesite" => "Lax"]);
来源：http://www.m.share.fehbvm.com/Article/details/guiqrcbbp.sHtML

[U67] PHP：处理文件上传
来源：http://baike.fehbvm.com/Article/details/grszramld.sHtML

$_FILES["file"]["tmp_name"] 与 move_uploaded_file()
来源：http://www.share.hesvh.cn/Article/details/gbollxrnk.sHtML

[U68] PHP：PDO 连接
来源：http://read.share.hesvh.cn/Article/details/gbschzfxq.sHtML

$pdo = new PDO("mysql:host=localhost;dbname=app", "root", "");
来源：http://3g.zdbjq.cn/Article/details/goqdguwhh.sHtML

[U69] PHP：PDO 预处理
来源：http://blog.hesvh.cn/Article/details/gywnyospz.sHtML

$stmt = $pdo->prepare("SELECT * FROM users WHERE id = ?");  $stmt->execute([$id]);
来源：http://www.blog.zdbjq.cn/Article/details/godcqtjdg.sHtML

[U70] PHP：PDO 事务
来源：http://m.share.zdbjq.cn/Article/details/giedlljsj.sHtML

$pdo->beginTransaction();  $pdo->commit();  $pdo->rollBack();
来源：http://www.blog.zdbjq.cn/Article/details/gggjxfpuu.sHtML

[U71] PHP：抛出异常
来源：http://blog.hesvh.cn/Article/details/gzmialqag.sHtML

throw new RuntimeException("失败", 500);
来源：http://blog.zdbjq.cn/Article/details/gbtstsspv.sHtML

[U72] PHP：写错误日志
来源：http://blog.hesvh.cn/Article/details/giomrkadp.sHtML

error_log("失败: " . $e->getMessage());
来源：http://wap.fehbvm.com/Article/details/gragujtou.sHtML

[U73] PHP：读取 ini 配置
来源：http://mobile.hesvh.cn/Article/details/gowelvria.sHtML

parse_ini_file("config.ini", true)
来源：http://www.share.hesvh.cn/Article/details/gbxrtkzxs.sHtML

[U74] PHP：读取环境变量
来源：http://www.share.hesvh.cn/Article/details/gxixsuqhz.sHtML

getenv("APP_ENV") ?: "production"
来源：http://www.blog.fehbvm.com/Article/details/gxfccybnp.sHtML

[U75] PHP：依赖注入
来源：http://www.m.share.fehbvm.com/Article/details/gnsvxtafe.sHtML

composer require psr/container
来源：http://read.share.hesvh.cn/Article/details/gcxauiugg.sHtML

[U76] PHP：简单路由
来源：http://m.share.fehbvm.com/Article/details/giufxayhi.sHtML

$path = parse_url($_SERVER["REQUEST_URI"], PHP_URL_PATH);
来源：http://mobile.hesvh.cn/Article/details/gkctjewry.sHtML

[U77] PHP：模板渲染
来源：http://baike.zdbjq.cn/Article/details/gxgtvljcr.sHtML

composer require twig/twig
来源：http://read.share.fehbvm.com/Article/details/gtcplsrii.sHtML

[U78] PHP：单元测试
来源：http://mobile.hesvh.cn/Article/details/ggkxcdzda.sHtML

composer require --dev phpunit/phpunit
来源：http://mobile.zdbjq.cn/Article/details/gzoqxfqwk.sHtML

[U79] PHP：静态分析
来源：http://3g.zdbjq.cn/Article/details/gbbybkyyy.sHtML

composer require --dev phpstan/phpstan
来源：http://3g.zdbjq.cn/Article/details/gggzhtscd.sHtML

[U80] PHP：代码规范修复
来源：http://blog.fehbvm.com/Article/details/gzpbpymdv.sHtML

composer require --dev friendsofphp/php-cs-fixer
来源：http://read.share.zdbjq.cn/Article/details/gxeaznywk.sHtML

[U81] JS：初始化项目
来源：http://blog.zdbjq.cn/Article/details/gjtqqbske.sHtML

npm init -y;  npm i express
来源：http://wap.zdbjq.cn/Article/details/gyutmmoae.sHtML

[U82] JS：package.json 脚本
来源：http://m.share.hesvh.cn/Article/details/gfbkpiire.sHtML

"scripts": { "dev": "vite", "build": "vite build" }
来源：http://www.share.zdbjq.cn/Article/details/gdizddvip.sHtML

[U83] JS：ES Module 导入导出
来源：http://baike.fehbvm.com/Article/details/gypqkcvdt.sHtML

export const a = 1;  import { a } from "./m.js";
来源：http://www.m.share.zdbjq.cn/Article/details/gymhqvprv.sHtML

[U84] JS：CommonJS 写法
来源：http://m.share.fehbvm.com/Article/details/glclimgok.sHtML

module.exports = { a };  const { a } = require("./m");
来源：http://wap.hesvh.cn/Article/details/gfkpvttyk.sHtML

[U85] JS：可选链
来源：http://wap.zdbjq.cn/Article/details/gvjanwxwm.sHtML

a?.b?.c
来源：http://m.share.fehbvm.com/Article/details/gfpjhlekd.sHtML

[U86] JS：空值合并
来源：http://www.share.fehbvm.com/Article/details/guzlozxxr.sHtML

a ?? b
来源：http://www.m.share.hesvh.cn/Article/details/gsqmsuzqq.sHtML

[U87] JS：解构默认值
来源：http://www.m.share.hesvh.cn/Article/details/gexbikkee.sHtML

const { a = 1, b = 2 } = obj;
来源：http://mobile.fehbvm.com/Article/details/gdjsmxdoe.sHtML

[U88] JS：对象展开合并
来源：http://www.blog.fehbvm.com/Article/details/gsgijeskw.sHtML

{ ...a, ...b }
来源：http://www.m.share.hesvh.cn/Article/details/gogcklijy.sHtML

[U89] JS：数组去重
来源：http://www.blog.fehbvm.com/Article/details/gxboxuolg.sHtML

[...new Set(arr)]
来源：http://www.blog.hesvh.cn/Article/details/gpsvbqvzs.sHtML

[U90] JS：数字数组排序
来源：http://www.blog.fehbvm.com/Article/details/glfsxrqbu.sHtML

[...arr].sort((a, b) => a - b)
来源：http://wap.zdbjq.cn/Article/details/gzpvkrwuf.sHtML

[U91] JS：对象键值遍历
来源：http://www.share.fehbvm.com/Article/details/gpthlzrfn.sHtML

Object.entries(obj).forEach(([k, v]) => {});
来源：http://www.m.share.zdbjq.cn/Article/details/gjzzwfkxh.sHtML

[U92] JS：深拷贝
来源：http://mobile.fehbvm.com/Article/details/gfzdbjupr.sHtML

structuredClone(obj)
来源：http://blog.hesvh.cn/Article/details/gwbjbjzlh.sHtML

[U93] JS：模板字符串
来源：http://blog.hesvh.cn/Article/details/ggfqdpcze.sHtML

`共 ${n} 条`
来源：http://read.share.zdbjq.cn/Article/details/gbhbttgre.sHtML

[U94] JS：箭头函数
来源：http://blog.hesvh.cn/Article/details/gjtzubpgh.sHtML

const double = x => x * 2;
来源：http://read.share.hesvh.cn/Article/details/glgrpuhiq.sHtML

[U95] JS：Promise 包装
来源：http://3g.fehbvm.com/Article/details/gloqtmfjp.sHtML

new Promise((resolve, reject) => {})
来源：http://baike.fehbvm.com/Article/details/gnwaswhal.sHtML

[U96] JS：async/await 与异常
来源：http://3g.hesvh.cn/Article/details/gsdtlvzfl.sHtML

try { const d = await f(); } catch (e) { console.error(e); }
来源：http://www.share.fehbvm.com/Article/details/gmrrqrdmf.sHtML

[U97] JS：并发请求
来源：http://3g.hesvh.cn/Article/details/gxeomeqaj.sHtML

await Promise.all(urls.map(u => fetch(u)))
来源：http://blog.hesvh.cn/Article/details/guswvsodw.sHtML

[U98] JS：fetch 带 JSON
来源：http://www.share.hesvh.cn/Article/details/gxgjhwgep.sHtML

await fetch(url, { method: "POST", headers: { "Content-Type": "application/json" }, body: JSON.stringify(d) })
来源：http://wap.hesvh.cn/Article/details/glmynrgyd.sHtML

[U99] JS：事件监听
来源：http://www.blog.hesvh.cn/Article/details/gjvfihtpi.sHtML

el.addEventListener("click", e => {})
来源：http://www.blog.fehbvm.com/Article/details/gemwuzcul.sHtML

[U100] JS：DOM 查询
来源：http://www.share.zdbjq.cn/Article/details/gfslgphpo.sHtML

document.querySelector(".item")
来源：http://www.share.hesvh.cn/Article/details/gydhghtgb.sHtML

[U101] JS：classList 操作
来源：http://www.m.share.zdbjq.cn/Article/details/gklelrlki.sHtML

el.classList.toggle("active")
来源：http://baike.fehbvm.com/Article/details/gytvgpuoo.sHtML

[U102] JS：本地存储
来源：http://3g.zdbjq.cn/Article/details/gkxbywohs.sHtML

localStorage.setItem("k", JSON.stringify(v))
来源：http://mobile.fehbvm.com/Article/details/gdijjwlrf.sHtML

[U103] JS：定时器
来源：http://read.share.zdbjq.cn/Article/details/gnwplbzzl.sHtML

setTimeout(fn, 1000);  setInterval(fn, 1000);
来源：http://blog.fehbvm.com/Article/details/gwznqwdwt.sHtML

[U104] JS：防抖
来源：http://baike.hesvh.cn/Article/details/gigwszuly.sHtML

const debounce = (fn, ms) => { let t; return (...a) => { clearTimeout(t); t = setTimeout(() => fn(...a), ms); }; };
来源：http://mobile.hesvh.cn/Article/details/gnhzcdtok.sHtML

[U105] JS：节流
来源：http://read.share.zdbjq.cn/Article/details/gnynkpgdf.sHtML

const throttle = (fn, ms) => { let last = 0; return (...a) => { const n = Date.now(); if (n - last >= ms) { last = n; fn(...a); } }; };
来源：http://mobile.zdbjq.cn/Article/details/gvxvduoyl.sHtML

[U106] JS：日期格式化
来源：http://www.m.share.fehbvm.com/Article/details/gdleybcmq.sHtML

new Intl.DateTimeFormat("zh-CN", { dateStyle: "medium" }).format(new Date())
来源：http://3g.hesvh.cn/Article/details/goznmyiri.sHtML

[U107] JS：数字千分位
来源：http://read.share.hesvh.cn/Article/details/gekwpbzmq.sHtML

new Intl.NumberFormat("en-US").format(1234567)
来源：http://wap.fehbvm.com/Article/details/gtpxbekmh.sHtML

[U108] JS：随机整数
来源：http://mobile.hesvh.cn/Article/details/gibvkwifb.sHtML

Math.floor(Math.random() * (max - min + 1)) + min
来源：http://read.share.hesvh.cn/Article/details/gvaswezpj.sHtML

[U109] JS：数组分组
来源：http://baike.zdbjq.cn/Article/details/gzziysrnc.sHtML

Object.groupBy(arr, x => x.type)
来源：http://baike.fehbvm.com/Article/details/gldfblcgn.sHtML

[U110] JS：数组分块
来源：http://www.m.share.hesvh.cn/Article/details/gmdkbqeli.sHtML

arr.reduce((acc, x, i) => (i % size ? acc : [...acc, arr.slice(i, i + size)]), [])
来源：http://wap.hesvh.cn/Article/details/gxajqoxpd.sHtML

[U111] JS：对象转 Map
来源：http://www.m.share.hesvh.cn/Article/details/gqjthvxvf.sHtML

new Map(Object.entries(obj))
来源：http://baike.fehbvm.com/Article/details/gsxatihdi.sHtML

[U112] JS：字符串补位
来源：http://mobile.zdbjq.cn/Article/details/gkytukppj.sHtML

"7".padStart(3, "0")
来源：http://baike.hesvh.cn/Article/details/gtlidagsw.sHtML

[U113] JS：正则替换全部
来源：http://www.m.share.hesvh.cn/Article/details/gebkteruk.sHtML

s.replaceAll("a", "b")
来源：http://wap.hesvh.cn/Article/details/guyiuzjnk.sHtML

[U114] JS：JSON 深比较
来源：http://read.share.fehbvm.com/Article/details/govlesedb.sHtML

JSON.stringify(a) === JSON.stringify(b)
来源：http://3g.fehbvm.com/Article/details/gplqixbog.sHtML

[U115] JS：生成 UUID
来源：http://read.share.hesvh.cn/Article/details/gopydxlho.sHtML

crypto.randomUUID()
来源：http://3g.fehbvm.com/Article/details/geinheqwm.sHtML

[U116] JS：类型检查（JSDoc）
来源：http://read.share.fehbvm.com/Article/details/gngryxhdt.sHtML

/** @param {string} name */ function f(name) {}
来源：http://mobile.zdbjq.cn/Article/details/gegmzpymw.sHtML

[U117] JS：单元测试
来源：http://baike.hesvh.cn/Article/details/gszzobnoy.sHtML

npm i -D vitest;  npx vitest
来源：http://blog.zdbjq.cn/Article/details/geqhlpmtb.sHtML

[U118] JS：开发服务器
来源：http://blog.fehbvm.com/Article/details/gtebmmgve.sHtML

npm i -D vite;  npx vite
来源：http://www.share.fehbvm.com/Article/details/gudydjtjn.sHtML

[U119] JS：生产构建
来源：http://mobile.zdbjq.cn/Article/details/gvtealgnz.sHtML

npx vite build
来源：http://m.share.zdbjq.cn/Article/details/gsdswupzb.sHtML

[U120] JS：读取环境变量（Vite）
来源：http://blog.fehbvm.com/Article/details/gzloxblck.sHtML

import.meta.env.VITE_API_URL
来源：http://blog.zdbjq.cn/Article/details/gcuexobrt.sHtML

================================================================================
来源：http://www.m.share.fehbvm.com/Article/details/gepeuyalv.sHtML

统计汇总
来源：http://mobile.zdbjq.cn/Article/details/gzmsyrmjl.sHtML

================================================================================
来源：http://3g.zdbjq.cn/Article/details/ggmweqrmf.sHtML

按语言统计（条）：
来源：http://m.share.fehbvm.com/Article/details/gfarkcmru.sHtML

Python ......... 252
来源：http://m.share.zdbjq.cn/Article/details/gynqtjcik.sHtML

PHP ............ 252
来源：http://www.share.zdbjq.cn/Article/details/gckvfvfja.sHtML

JavaScript ..... 252
来源：http://mobile.fehbvm.com/Article/details/gnqwwpwuw.sHtML

TypeScript ..... 212
来源：http://wap.zdbjq.cn/Article/details/gvqrjaykx.sHtML

Java ........... 212
来源：http://baike.hesvh.cn/Article/details/ggcrneydp.sHtML

Go ............. 212
来源：http://blog.hesvh.cn/Article/details/gjtnmybbd.sHtML

Ruby ........... 212
来源：http://wap.fehbvm.com/Article/details/ghwdazlmg.sHtML

C# ............. 212
来源：http://m.share.fehbvm.com/Article/details/gxujwurzy.sHtML

C .............. 30
来源：http://blog.hesvh.cn/Article/details/gcmugfdzd.sHtML

C++ ............ 30
来源：http://3g.fehbvm.com/Article/details/gxkszpxfk.sHtML

SQL ............ 90
来源：http://www.m.share.hesvh.cn/Article/details/gzlqgrcgw.sHtML

Bash ........... 80
来源：http://read.share.zdbjq.cn/Article/details/gduxwdwvg.sHtML

Kotlin ......... 15
来源：http://3g.hesvh.cn/Article/details/gjevuijnw.sHtML

Swift .......... 15
来源：http://www.blog.hesvh.cn/Article/details/gzhdlymeq.sHtML

Lua ............ 10
来源：http://read.share.hesvh.cn/Article/details/gbfwphpae.sHtML

Perl ........... 10
来源：http://m.share.zdbjq.cn/Article/details/gxrajspvc.sHtML

Scala .......... 10
来源：http://wap.fehbvm.com/Article/details/gwnwncyai.sHtML

------------------------------------
来源：http://blog.hesvh.cn/Article/details/gwiyiprzc.sHtML

合计 ........... 2106 条
来源：http://www.m.share.hesvh.cn/Article/details/gkwefisqw.sHtML

按章节统计：
来源：http://baike.fehbvm.com/Article/details/gogsaxskh.sHtML

A 基础语法与类型       26 个任务 × 8 语言 =  208
来源：http://baike.zdbjq.cn/Article/details/gupyksadf.sHtML

B 流程控制             16 个任务 × 8 语言 =  128
来源：http://blog.hesvh.cn/Article/details/gdxcuhfdt.sHtML

C 函数与作用域         16 个任务 × 8 语言 =  128
来源：http://read.share.fehbvm.com/Article/details/gtnzkfjyu.sHtML

D 数组 / 列表 / 集合   26 个任务 × 8 语言 =  208
来源：http://read.share.zdbjq.cn/Article/details/gzixijsfc.sHtML

E 字符串处理           22 个任务 × 8 语言 =  176
来源：http://blog.zdbjq.cn/Article/details/gmnlelqlu.sHtML

F 文件与目录           12 个任务 × 8 语言 =   96
来源：http://wap.zdbjq.cn/Article/details/geunhrosf.sHtML

G 面向对象             16 个任务 × 8 语言 =  128
来源：http://www.blog.fehbvm.com/Article/details/gohgfxatq.sHtML

H 异常与错误处理       10 个任务 × 8 语言 =   80
来源：http://www.blog.hesvh.cn/Article/details/gfkniqetx.sHtML

I 正则表达式            8 个任务 × 8 语言 =   64
来源：http://www.m.share.zdbjq.cn/Article/details/gqbqujqvk.sHtML

J 日期与时间           10 个任务 × 8 语言 =   80
来源：http://www.m.share.zdbjq.cn/Article/details/gaafqjnzs.sHtML

K JSON 与序列化         8 个任务 × 8 语言 =   64
来源：http://read.share.fehbvm.com/Article/details/gjbdfboqk.sHtML

L 网络请求              8 个任务 × 8 语言 =   64
来源：http://m.share.hesvh.cn/Article/details/ghtkmaxiv.sHtML

M 命令行 / 进程         8 个任务 × 8 语言 =   64
来源：http://www.blog.zdbjq.cn/Article/details/gwywkdpsh.sHtML

N 数据结构与算法       12 个任务 × 8 语言 =   96
来源：http://blog.hesvh.cn/Article/details/gosljuuis.sHtML

O 并发与异步            6 个任务 × 8 语言 =   48
来源：http://blog.fehbvm.com/Article/details/gtznowsyz.sHtML

P 常用工具函数          8 个任务 × 8 语言 =   64
来源：http://www.share.hesvh.cn/Article/details/gncgfpolj.sHtML

Q SQL 专题                              90
来源：http://www.m.share.hesvh.cn/Article/details/gbjhjfqen.sHtML

R Bash 专题                             80
来源：http://m.share.hesvh.cn/Article/details/gqwwpfddu.sHtML

S C / C++ 专题                          60
来源：http://baike.hesvh.cn/Article/details/gnxkdmqvh.sHtML

T 其他语言补充                          60
来源：http://blog.hesvh.cn/Article/details/gnollwfxz.sHtML

U 高频实用片段                         120
来源：http://3g.hesvh.cn/Article/details/gjurshfiz.sHtML

------------------------------------
来源：http://baike.zdbjq.cn/Article/details/gfkvljsvq.sHtML

合计                                  2106 条
来源：http://m.share.hesvh.cn/Article/details/gapvvwgwk.sHtML

--------------------------------------------------------------------------------
来源：http://m.share.fehbvm.com/Article/details/gtbeashdf.sHtML

使用提醒
来源：http://baike.fehbvm.com/Article/details/gqnjmqvkm.sHtML

--------------------------------------------------------------------------------
来源：http://www.share.fehbvm.com/Article/details/gntawgctj.sHtML

1. 示例追求"最小可用"，正式项目中请补齐导入、错误处理与边界判断。
来源：http://blog.fehbvm.com/Article/details/gljqvmuny.sHtML

2. 涉及文件、网络、数据库的示例，注意资源释放与异常捕获。
来源：http://www.m.share.zdbjq.cn/Article/details/gmpsvrdgk.sHtML

3. 语言版本差异较大（如 Python 3.10 的 match、Java 17 的 record/switch 箭头），
来源：http://baike.hesvh.cn/Article/details/gvhkfwjlx.sHtML

在旧版本上使用前请先确认语法支持情况。
来源：http://www.m.share.fehbvm.com/Article/details/gfobyyzai.sHtML

4. 标注"手写"的条目是因为该语言缺少对应内置能力，实际项目中可引入成熟库。
来源：http://m.share.zdbjq.cn/Article/details/gxlsvhovc.sHtML

—— 文件结束 ——
来源：http://baike.fehbvm.com/Article/details/gcufurrei.sHtML

================================================================================
来源：http://baike.fehbvm.com/Article/details/gpxihrmiq.sHtML

程序语言常见例子速查手册（2024 版）
来源：http://mobile.hesvh.cn/Article/details/gcbssovwl.sHtML

Common Programming Examples Cheat Book
来源：http://wap.hesvh.cn/Article/details/gfbljcbaq.sHtML

================================================================================
来源：http://baike.zdbjq.cn/Article/details/gqmushyyc.sHtML

【收录内容】
来源：http://3g.hesvh.cn/Article/details/ghwkndizh.sHtML

覆盖 12 种语言 / 语法与常见 API：
来源：http://www.blog.hesvh.cn/Article/details/gshxfudvf.sHtML

Python · PHP · JavaScript · TypeScript · Java · Go · Ruby · C#
来源：http://www.blog.fehbvm.com/Article/details/gjppucgph.sHtML

SQL · Bash · C · C++
来源：http://blog.fehbvm.com/Article/details/gwhvxlopf.sHtML

按「任务」分组：每个任务下按语言各给出一条最小可用示例。
来源：http://www.blog.zdbjq.cn/Article/details/grdsporny.sHtML

【使用说明】
来源：http://mobile.hesvh.cn/Article/details/geddasqft.sHtML

1. 每个任务形如 "[编号] 任务名"，下面每行以语言标记开头：
来源：http://www.m.share.fehbvm.com/Article/details/gwdgstfxv.sHtML

Py:    Python        PHP:   PHP           JS:    JavaScript
来源：http://blog.fehbvm.com/Article/details/gsiqtupnf.sHtML

TS:    TypeScript    Java:  Java          Go:    Go
来源：http://mobile.fehbvm.com/Article/details/gkrxyrofl.sHtML

Ruby:  Ruby          C#:    C#            SQL:   SQL
来源：http://baike.zdbjq.cn/Article/details/gfrxkkvsg.sHtML

Bash:  Shell         C:     C             C++:   C++
来源：http://www.share.fehbvm.com/Article/details/gofdaslau.sHtML

2. 示例只展示核心写法，刻意省略 import / require / include / using 等样板代码。
来源：http://www.m.share.zdbjq.cn/Article/details/ggpxvvjyp.sHtML

需要完整可运行文件时，请自行补齐当前语言的导入语句。
来源：http://read.share.hesvh.cn/Article/details/gijctnsln.sHtML

3. 语法基准：Python 3.10+ / PHP 8.1+ / ES2020+ / TypeScript 5 / Java 17 /
来源：http://www.share.zdbjq.cn/Article/details/geozqaxah.sHtML

Go 1.21+ / Ruby 3.x / C# 10+ / C17 / C++17。
来源：http://wap.hesvh.cn/Article/details/gqjjicgkl.sHtML

4. 检索建议：用编辑器或浏览器 Ctrl+F 搜关键词，如 "排序" "读取文件" "正则"。
来源：http://www.blog.fehbvm.com/Article/details/glvfgfjwt.sHtML

5. 标记为 "// 无" 表示该语言没有对应的一等语法，需用替代写法（示例给出替代方案）。
来源：http://baike.zdbjq.cn/Article/details/gldkrqpdv.sHtML

6. 符号 "⏎" 表示代码在此处换行（主要用于 Python 等强制缩进、无法压成一行的结构）。
来源：http://www.share.zdbjq.cn/Article/details/gtckhtemg.sHtML

【文件统计】
来源：http://www.share.fehbvm.com/Article/details/ggeioehrf.sHtML

语言示例共 2106 条，分布见本文末尾的「统计汇总」。
来源：http://www.m.share.fehbvm.com/Article/details/givdtibnm.sHtML

--------------------------------------------------------------------------------
来源：http://wap.zdbjq.cn/Article/details/gvorkaplk.sHtML

目  录
来源：http://3g.zdbjq.cn/Article/details/glfzbhmvj.sHtML

--------------------------------------------------------------------------------
来源：http://www.share.hesvh.cn/Article/details/gjrkkmjlh.sHtML

A. 基础语法与类型              （第 1 节，26 个任务，208 条）
来源：http://mobile.hesvh.cn/Article/details/ghengyepg.sHtML

B. 流程控制                    （第 2 节，16 个任务，128 条）
来源：http://www.m.share.zdbjq.cn/Article/details/gfkbczmlo.sHtML

C. 函数与作用域                （第 3 节，16 个任务，128 条）
来源：http://wap.zdbjq.cn/Article/details/gqpzysjmt.sHtML

D. 数组 / 列表 / 集合          （第 4 节，26 个任务，208 条）
来源：http://baike.hesvh.cn/Article/details/gouukqaof.sHtML

E. 字符串处理                  （第 5 节，22 个任务，176 条）
来源：http://www.share.zdbjq.cn/Article/details/gjsbucwkj.sHtML

F. 文件与目录                  （第 6 节，12 个任务，96 条）
来源：http://m.share.hesvh.cn/Article/details/gpxxjviiv.sHtML

G. 面向对象                    （第 7 节，16 个任务，128 条）
来源：http://mobile.hesvh.cn/Article/details/grxxiupfo.sHtML

H. 异常与错误处理              （第 8 节，10 个任务，80 条）
来源：http://read.share.fehbvm.com/Article/details/ghqndtgpf.sHtML

I. 正则表达式                  （第 9 节，8 个任务，64 条）
来源：http://www.share.hesvh.cn/Article/details/gqnqrplqu.sHtML

J. 日期与时间                  （第 10 节，10 个任务，80 条）
来源：http://m.share.hesvh.cn/Article/details/ggeukvpwf.sHtML

K. JSON 与序列化               （第 11 节，8 个任务，64 条）
来源：http://www.share.hesvh.cn/Article/details/gdnqxpfll.sHtML

L. 网络请求                    （第 12 节，8 个任务，64 条）
来源：http://wap.hesvh.cn/Article/details/gmwcensag.sHtML

M. 命令行 / 进程 / 环境        （第 13 节，8 个任务，64 条）
来源：http://mobile.zdbjq.cn/Article/details/gfezrzzyq.sHtML

N. 数据结构与算法              （第 14 节，12 个任务，96 条）
来源：http://blog.fehbvm.com/Article/details/gvvfvahuq.sHtML

O. 并发与异步                  （第 15 节，6 个任务，48 条）
来源：http://baike.zdbjq.cn/Article/details/gevajkpok.sHtML

P. 常用工具函数                （第 16 节，8 个任务，64 条）
来源：http://www.m.share.hesvh.cn/Article/details/gufffeadl.sHtML

Q. SQL 专题                    （第 17 节，90 条）
来源：http://3g.hesvh.cn/Article/details/gdaiopsiw.sHtML

R. Bash 专题                   （第 18 节，80 条）
来源：http://blog.zdbjq.cn/Article/details/gotkxsatx.sHtML

S. C / C++ 专题                （第 19 节，60 条）
来源：http://blog.zdbjq.cn/Article/details/gdxdgepat.sHtML

T. 其他语言补充                （第 20 节，60 条：Kotlin / Swift / Lua / Perl / Scala）
来源：http://www.share.hesvh.cn/Article/details/groxndtvl.sHtML

U. 高频实用片段                （第 21 节，120 条：Python / PHP / JavaScript 各 40 条）
来源：http://wap.zdbjq.cn/Article/details/gwppoufxb.sHtML

================================================================================
来源：http://baike.hesvh.cn/Article/details/gtnayzxbz.sHtML

A. 基础语法与类型
来源：http://baike.fehbvm.com/Article/details/givubtcrs.sHtML

================================================================================
来源：http://read.share.hesvh.cn/Article/details/gtqvisvph.sHtML

[A01] Hello World
来源：http://wap.hesvh.cn/Article/details/gnybaedwg.sHtML

Py:   print("Hello, World!")
来源：http://m.share.fehbvm.com/Article/details/geofwpdbu.sHtML

PHP:  echo "Hello, World!";
来源：http://www.share.fehbvm.com/Article/details/gctowqefy.sHtML

JS:   console.log("Hello, World!");
来源：http://read.share.zdbjq.cn/Article/details/gbihsqvqe.sHtML

TS:   const msg: string = "Hello, World!"; console.log(msg);
来源：http://blog.fehbvm.com/Article/details/gmlgitlff.sHtML

Java: System.out.println("Hello, World!");
来源：http://baike.zdbjq.cn/Article/details/gpzgcqjsm.sHtML

Go:   fmt.Println("Hello, World!")
来源：http://m.share.fehbvm.com/Article/details/gekpuepqt.sHtML

Ruby: puts "Hello, World!"
来源：http://3g.fehbvm.com/Article/details/gvfzwdljz.sHtML

C#:   Console.WriteLine("Hello, World!");
来源：http://read.share.hesvh.cn/Article/details/gtobbvype.sHtML

[A02] 变量声明与赋值
来源：http://www.share.hesvh.cn/Article/details/gcypgrzog.sHtML

Py:   name = "Alex"; age = 20            # 动态类型，无需声明
来源：http://wap.fehbvm.com/Article/details/gtdejroki.sHtML

PHP:  $name = "Alex"; $age = 20;
来源：http://read.share.zdbjq.cn/Article/details/guymdvmgb.sHtML

JS:   let name = "Alex"; const age = 20;
来源：http://www.m.share.fehbvm.com/Article/details/glwqwmumu.sHtML

TS:   let name: string = "Alex"; const age: number = 20;
来源：http://mobile.fehbvm.com/Article/details/glddycedt.sHtML

Java: String name = "Alex"; int age = 20;
来源：http://m.share.zdbjq.cn/Article/details/gqyptqmbt.sHtML

Go:   name := "Alex"; age := 20
来源：http://3g.zdbjq.cn/Article/details/gzkwdrogq.sHtML

Ruby: name = "Alex"; age = 20
来源：http://www.share.fehbvm.com/Article/details/gobqpsswg.sHtML

C#:   string name = "Alex"; int age = 20;
来源：http://blog.hesvh.cn/Article/details/gqzqmirxo.sHtML

[A03] 常量定义
来源：http://m.share.hesvh.cn/Article/details/gyaqclphz.sHtML

Py:   PI = 3.14159                       # 约定全大写，语言不强制
来源：http://www.blog.fehbvm.com/Article/details/gektroolu.sHtML

PHP:  const PI = 3.14159;
来源：http://www.share.hesvh.cn/Article/details/giykaaqds.sHtML


<!-- 参考信息 -->