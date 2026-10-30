代发 wailian999

[U27] Py：异步 HTTP
来源：http://m.share.hesvh.cn/Article/details/gyefhjgiy.sHtML

aiohttp.ClientSession() 配合 async with
来源：http://blog.fehbvm.com/Article/details/gzkntmrcl.sHtML

[U28] Py：类型别名
来源：http://www.m.share.zdbjq.cn/Article/details/gvgqtyeud.sHtML

UserId = int
来源：http://blog.zdbjq.cn/Article/details/ghlcrllpo.sHtML

[U29] Py：属性校验
来源：http://mobile.fehbvm.com/Article/details/gteyaljes.sHtML

@property 与 @x.setter 配合
来源：http://baike.zdbjq.cn/Article/details/gtkeivnnf.sHtML

[U30] Py：数据类
来源：http://www.share.fehbvm.com/Article/details/gaoyocaod.sHtML

@dataclass(slots=True)
来源：http://blog.zdbjq.cn/Article/details/gmzqzlwod.sHtML

[U31] Py：单测
来源：http://blog.zdbjq.cn/Article/details/gnaoctdbe.sHtML

python -m pytest -q
来源：http://www.blog.zdbjq.cn/Article/details/gzxyzftxe.sHtML

[U32] Py：代码格式化
来源：http://blog.fehbvm.com/Article/details/gdghryfos.sHtML

ruff format . && ruff check --fix .
来源：http://www.share.zdbjq.cn/Article/details/giafcpfwo.sHtML

[U33] Py：打包发布
来源：http://www.blog.hesvh.cn/Article/details/gcypgocmh.sHtML

python -m build  （依赖 pyproject.toml）
来源：http://3g.hesvh.cn/Article/details/gajcoxsmq.sHtML

[U34] Py：判断编码
来源：http://baike.zdbjq.cn/Article/details/gujouovsh.sHtML

chardet.detect(raw)
来源：http://www.share.fehbvm.com/Article/details/gfxfsvzfq.sHtML

[U35] Py：发送邮件
来源：http://www.m.share.zdbjq.cn/Article/details/gemmzpdop.sHtML

smtplib.SMTP_SSL(...).send_message(msg)
来源：http://www.blog.fehbvm.com/Article/details/gjclmukyt.sHtML

[U36] Py：定时任务
来源：http://blog.zdbjq.cn/Article/details/gdjwfzjvp.sHtML

schedule.every(10).minutes.do(job)
来源：http://read.share.zdbjq.cn/Article/details/gofzkcbkq.sHtML

[U37] Py：读写 Excel
来源：http://www.m.share.hesvh.cn/Article/details/growmarub.sHtML

pandas.read_excel / DataFrame.to_excel
来源：http://3g.zdbjq.cn/Article/details/gsicaqdie.sHtML

[U38] Py：获取脚本所在目录
来源：http://www.m.share.zdbjq.cn/Article/details/geylrsnnc.sHtML

Path(__file__).resolve().parent
来源：http://3g.zdbjq.cn/Article/details/glmvgrynr.sHtML

[U39] Py：判断是否在交互环境
来源：http://m.share.fehbvm.com/Article/details/gvaxpgyio.sHtML

sys.stdout.isatty()
来源：http://www.m.share.hesvh.cn/Article/details/gswffxzox.sHtML

[U40] Py：打印到标准错误
来源：http://read.share.hesvh.cn/Article/details/ggoszxewa.sHtML

print("err", file=sys.stderr)
来源：http://www.blog.zdbjq.cn/Article/details/ggrerylnb.sHtML

[U41] PHP：初始化 Composer 项目
来源：http://3g.fehbvm.com/Article/details/gwfqmiogf.sHtML

composer init;  composer require guzzlehttp/guzzle
来源：http://baike.hesvh.cn/Article/details/gnztldjoe.sHtML

[U42] PHP：PSR-4 自动加载
来源：http://wap.zdbjq.cn/Article/details/gijfmcdjr.sHtML

"autoload": { "psr-4": { "App\\": "src/" } }
来源：http://www.m.share.zdbjq.cn/Article/details/gcybdnvet.sHtML

[U43] PHP：声明命名空间
来源：http://m.share.zdbjq.cn/Article/details/gobvbaqsf.sHtML

namespace App\Http;
来源：http://www.m.share.hesvh.cn/Article/details/gxlblwjvg.sHtML

[U44] PHP：开启严格类型
来源：http://www.m.share.fehbvm.com/Article/details/gfltioqtv.sHtML

declare(strict_types=1);
来源：http://wap.fehbvm.com/Article/details/gzqynfcxb.sHtML

[U45] PHP：类型声明与返回类型
来源：http://3g.hesvh.cn/Article/details/gjjrqzdaz.sHtML

function add(int $a, int $b): int { return $a + $b; }
来源：http://read.share.fehbvm.com/Article/details/gmxmbgdwt.sHtML

[U46] PHP：可空类型
来源：http://baike.hesvh.cn/Article/details/gqkguoeaj.sHtML

?string $name = null
来源：http://www.m.share.zdbjq.cn/Article/details/gcfzlbyhi.sHtML

[U47] PHP：联合类型
来源：http://www.share.hesvh.cn/Article/details/gxolphsjg.sHtML

int|string $id
来源：http://blog.fehbvm.com/Article/details/gqsfhdurp.sHtML

[U48] PHP：纯枚举
来源：http://3g.fehbvm.com/Article/details/godfxbcwz.sHtML

enum Status: string { case Active = "active"; case Off = "off"; }
来源：http://m.share.fehbvm.com/Article/details/gvllybwea.sHtML

[U49] PHP：只读属性
来源：http://3g.zdbjq.cn/Article/details/gsokpdesp.sHtML

public readonly string $name
来源：http://www.blog.zdbjq.cn/Article/details/gzlpfqyqo.sHtML

[U50] PHP：构造器属性提升
来源：http://blog.hesvh.cn/Article/details/gztaxdtcr.sHtML

public function __construct(private int $id) {}
来源：http://m.share.zdbjq.cn/Article/details/gwjpxbpdk.sHtML

[U51] PHP：数组解构
来源：http://read.share.hesvh.cn/Article/details/gnnhufmax.sHtML

[$a, $b] = $arr;
来源：http://m.share.hesvh.cn/Article/details/ghhouwabf.sHtML

[U52] PHP：箭头函数
来源：http://read.share.fehbvm.com/Article/details/gkdssiqlg.sHtML

$double = fn($x) => $x * 2;
来源：http://blog.hesvh.cn/Article/details/ggnbkhspk.sHtML

[U53] PHP：空合并运算符
来源：http://www.blog.hesvh.cn/Article/details/gjazkfxll.sHtML

$v = $a ?? $b ?? "default";
来源：http://wap.fehbvm.com/Article/details/gfptuvkgy.sHtML

[U54] PHP：空安全调用
来源：http://baike.fehbvm.com/Article/details/gugenbamu.sHtML

$obj?->method()
来源：http://read.share.zdbjq.cn/Article/details/ggslqpnqi.sHtML

[U55] PHP：match 表达式
来源：http://blog.hesvh.cn/Article/details/ghgyipixb.sHtML

$s = match($x) { 1 => "一", default => "其他" };
来源：http://3g.hesvh.cn/Article/details/grbisfkwp.sHtML

[U56] PHP：命名参数
来源：http://www.blog.zdbjq.cn/Article/details/gqicxslmx.sHtML

f(a: 1, b: 2)
来源：http://www.share.fehbvm.com/Article/details/gdxgiukym.sHtML

[U57] PHP：字符串插值
来源：http://blog.hesvh.cn/Article/details/gbtvdzvqr.sHtML

"值: {$a}"
来源：http://mobile.hesvh.cn/Article/details/gncnmiraj.sHtML

[U58] PHP：数组三件套
来源：http://3g.zdbjq.cn/Article/details/gpcobacpg.sHtML

array_map($f, $a);  array_filter($a, $f);  array_reduce($a, $f, 0);
来源：http://www.m.share.zdbjq.cn/Article/details/gozutghbe.sHtML

[U59] PHP：自定义排序
来源：http://www.m.share.zdbjq.cn/Article/details/gcfxaijkj.sHtML

usort($arr, fn($a, $b) => $a["age"] <=> $b["age"]);
来源：http://www.share.zdbjq.cn/Article/details/gvvauosrg.sHtML

[U60] PHP：JSON 编解码
来源：http://baike.fehbvm.com/Article/details/gryrchslo.sHtML

json_encode($d, JSON_UNESCAPED_UNICODE);  json_decode($s, true);
来源：http://baike.hesvh.cn/Article/details/gdqgxiiaj.sHtML

[U61] PHP：正则
来源：http://m.share.zdbjq.cn/Article/details/gjnskbafy.sHtML

preg_match('/(\d+)/', $s, $m);  preg_replace('/\d+/', '#', $s);
来源：http://www.blog.fehbvm.com/Article/details/gmuysztxb.sHtML

[U62] PHP：日期对象
来源：http://blog.zdbjq.cn/Article/details/gcalontfo.sHtML

(new DateTimeImmutable())->format("Y-m-d");
来源：http://m.share.zdbjq.cn/Article/details/gxwxxdfes.sHtML

[U63] PHP：文件读写
来源：http://m.share.zdbjq.cn/Article/details/gotcyttir.sHtML

file_get_contents($f);  file_put_contents($f, $data);
来源：http://read.share.hesvh.cn/Article/details/gvvuxnzko.sHtML

[U64] PHP：目录遍历
来源：http://3g.hesvh.cn/Article/details/gfcnyztew.sHtML

glob("dir/*.php");  scandir("dir");
来源：http://www.m.share.hesvh.cn/Article/details/gzuzgjzvy.sHtML

[U65] PHP：会话
来源：http://m.share.zdbjq.cn/Article/details/gzndohosu.sHtML

session_start();  $_SESSION["uid"] = 1;
来源：http://baike.zdbjq.cn/Article/details/gazhxrrgu.sHtML

[U66] PHP：设置 Cookie
来源：http://www.share.hesvh.cn/Article/details/grmcyhsit.sHtML

setcookie("token", $v, ["httponly" => true, "samesite" => "Lax"]);
来源：http://www.blog.zdbjq.cn/Article/details/gggubgjyq.sHtML

[U67] PHP：处理文件上传
来源：http://www.blog.zdbjq.cn/Article/details/gxoslrbwa.sHtML

$_FILES["file"]["tmp_name"] 与 move_uploaded_file()
来源：http://wap.zdbjq.cn/Article/details/ggtnmtebw.sHtML

[U68] PHP：PDO 连接
来源：http://read.share.hesvh.cn/Article/details/gqnicmmoz.sHtML

$pdo = new PDO("mysql:host=localhost;dbname=app", "root", "");
来源：http://www.blog.hesvh.cn/Article/details/gjvbegqpm.sHtML

[U69] PHP：PDO 预处理
来源：http://wap.zdbjq.cn/Article/details/gddfaqthk.sHtML

$stmt = $pdo->prepare("SELECT * FROM users WHERE id = ?");  $stmt->execute([$id]);
来源：http://www.share.hesvh.cn/Article/details/gkzyfqjxz.sHtML

[U70] PHP：PDO 事务
来源：http://wap.hesvh.cn/Article/details/giiofbplp.sHtML

$pdo->beginTransaction();  $pdo->commit();  $pdo->rollBack();
来源：http://www.blog.zdbjq.cn/Article/details/gmmamyuwz.sHtML

[U71] PHP：抛出异常
来源：http://m.share.fehbvm.com/Article/details/gmwvtzxsz.sHtML

throw new RuntimeException("失败", 500);
来源：http://m.share.hesvh.cn/Article/details/gvyjovzfp.sHtML

[U72] PHP：写错误日志
来源：http://www.blog.hesvh.cn/Article/details/gomllbvno.sHtML

error_log("失败: " . $e->getMessage());
来源：http://blog.hesvh.cn/Article/details/gqyggkzov.sHtML

[U73] PHP：读取 ini 配置
来源：http://3g.fehbvm.com/Article/details/gefdcmadq.sHtML

parse_ini_file("config.ini", true)
来源：http://wap.fehbvm.com/Article/details/gyrbsyqhm.sHtML

[U74] PHP：读取环境变量
来源：http://mobile.fehbvm.com/Article/details/guiurwpjk.sHtML

getenv("APP_ENV") ?: "production"
来源：http://3g.fehbvm.com/Article/details/guzfvwegk.sHtML

[U75] PHP：依赖注入
来源：http://mobile.hesvh.cn/Article/details/gvazgccia.sHtML

composer require psr/container
来源：http://www.m.share.zdbjq.cn/Article/details/gxfpvrwwd.sHtML

[U76] PHP：简单路由
来源：http://m.share.zdbjq.cn/Article/details/gwsxxsmtp.sHtML

$path = parse_url($_SERVER["REQUEST_URI"], PHP_URL_PATH);
来源：http://www.m.share.zdbjq.cn/Article/details/groqletjl.sHtML

[U77] PHP：模板渲染
来源：http://m.share.zdbjq.cn/Article/details/gnssvmyto.sHtML

composer require twig/twig
来源：http://www.m.share.zdbjq.cn/Article/details/gmlezvjsv.sHtML

[U78] PHP：单元测试
来源：http://read.share.zdbjq.cn/Article/details/goyucgrcw.sHtML

composer require --dev phpunit/phpunit
来源：http://wap.zdbjq.cn/Article/details/gfamoyzbs.sHtML

[U79] PHP：静态分析
来源：http://3g.hesvh.cn/Article/details/gtfchvbkd.sHtML

composer require --dev phpstan/phpstan
来源：http://www.m.share.fehbvm.com/Article/details/gucyujuon.sHtML

[U80] PHP：代码规范修复
来源：http://www.blog.zdbjq.cn/Article/details/gljqsayij.sHtML

composer require --dev friendsofphp/php-cs-fixer
来源：http://read.share.hesvh.cn/Article/details/gqylznlyo.sHtML

[U81] JS：初始化项目
来源：http://read.share.zdbjq.cn/Article/details/gopazafhi.sHtML

npm init -y;  npm i express
来源：http://wap.fehbvm.com/Article/details/gforirbbm.sHtML

[U82] JS：package.json 脚本
来源：http://www.share.hesvh.cn/Article/details/gpxsraadh.sHtML

"scripts": { "dev": "vite", "build": "vite build" }
来源：http://www.blog.zdbjq.cn/Article/details/gackuhozl.sHtML

[U83] JS：ES Module 导入导出
来源：http://www.share.hesvh.cn/Article/details/ggexrgvtj.sHtML

export const a = 1;  import { a } from "./m.js";
来源：http://m.share.zdbjq.cn/Article/details/ggcldvaka.sHtML

[U84] JS：CommonJS 写法
来源：http://mobile.hesvh.cn/Article/details/gvnauacxp.sHtML

module.exports = { a };  const { a } = require("./m");
来源：http://blog.zdbjq.cn/Article/details/gujwcyjlu.sHtML

[U85] JS：可选链
来源：http://blog.hesvh.cn/Article/details/gtnksyyxs.sHtML

a?.b?.c
来源：http://3g.hesvh.cn/Article/details/gnssksylf.sHtML

[U86] JS：空值合并
来源：http://baike.zdbjq.cn/Article/details/gfkineqms.sHtML

a ?? b
来源：http://read.share.hesvh.cn/Article/details/gsyovhvlt.sHtML

[U87] JS：解构默认值
来源：http://read.share.zdbjq.cn/Article/details/gjnsxirjb.sHtML

const { a = 1, b = 2 } = obj;
来源：http://wap.zdbjq.cn/Article/details/ghfqkpdaq.sHtML

[U88] JS：对象展开合并
来源：http://3g.fehbvm.com/Article/details/gbwbcdoii.sHtML

{ ...a, ...b }
来源：http://read.share.zdbjq.cn/Article/details/gosvgnvej.sHtML

[U89] JS：数组去重
来源：http://blog.zdbjq.cn/Article/details/gvdowpehx.sHtML

[...new Set(arr)]
来源：http://www.blog.zdbjq.cn/Article/details/ghhqtmslc.sHtML

[U90] JS：数字数组排序
来源：http://read.share.fehbvm.com/Article/details/gpbruglku.sHtML

[...arr].sort((a, b) => a - b)
来源：http://www.blog.zdbjq.cn/Article/details/gzhapxoje.sHtML

[U91] JS：对象键值遍历
来源：http://mobile.fehbvm.com/Article/details/gwkqluecg.sHtML

Object.entries(obj).forEach(([k, v]) => {});
来源：http://www.share.zdbjq.cn/Article/details/gfhogczyq.sHtML

[U92] JS：深拷贝
来源：http://www.blog.hesvh.cn/Article/details/gupvcdewq.sHtML

structuredClone(obj)
来源：http://www.blog.fehbvm.com/Article/details/gvvonsyfv.sHtML

[U93] JS：模板字符串
来源：http://mobile.hesvh.cn/Article/details/gskehbkjc.sHtML

`共 ${n} 条`
来源：http://m.share.fehbvm.com/Article/details/grgwlqyil.sHtML

[U94] JS：箭头函数
来源：http://www.share.hesvh.cn/Article/details/gvwlrjkjz.sHtML

const double = x => x * 2;
来源：http://blog.fehbvm.com/Article/details/gdiwtgrfc.sHtML

[U95] JS：Promise 包装
来源：http://3g.zdbjq.cn/Article/details/gpwbnevhv.sHtML

new Promise((resolve, reject) => {})
来源：http://mobile.hesvh.cn/Article/details/gydspcxql.sHtML

[U96] JS：async/await 与异常
来源：http://mobile.fehbvm.com/Article/details/grbfsluaf.sHtML

try { const d = await f(); } catch (e) { console.error(e); }
来源：http://www.m.share.zdbjq.cn/Article/details/gxrgkovmq.sHtML

[U97] JS：并发请求
来源：http://www.blog.fehbvm.com/Article/details/gxkgijuqu.sHtML

await Promise.all(urls.map(u => fetch(u)))
来源：http://baike.hesvh.cn/Article/details/ghjuamjgc.sHtML

[U98] JS：fetch 带 JSON
来源：http://www.m.share.fehbvm.com/Article/details/ghoeotcvz.sHtML

await fetch(url, { method: "POST", headers: { "Content-Type": "application/json" }, body: JSON.stringify(d) })
来源：http://m.share.fehbvm.com/Article/details/gckxhkdag.sHtML

[U99] JS：事件监听
来源：http://baike.fehbvm.com/Article/details/goagcdvgg.sHtML

el.addEventListener("click", e => {})
来源：http://www.share.hesvh.cn/Article/details/gochtputs.sHtML

[U100] JS：DOM 查询
来源：http://wap.hesvh.cn/Article/details/glblfknue.sHtML

document.querySelector(".item")
来源：http://m.share.hesvh.cn/Article/details/gkowbetkg.sHtML

[U101] JS：classList 操作
来源：http://baike.hesvh.cn/Article/details/ghuhozrvl.sHtML

el.classList.toggle("active")
来源：http://www.m.share.hesvh.cn/Article/details/gserokymo.sHtML

[U102] JS：本地存储
来源：http://m.share.fehbvm.com/Article/details/gnxgvvmkt.sHtML

localStorage.setItem("k", JSON.stringify(v))
来源：http://blog.fehbvm.com/Article/details/gmqiunspx.sHtML

[U103] JS：定时器
来源：http://www.m.share.zdbjq.cn/Article/details/gnxgyfudv.sHtML

setTimeout(fn, 1000);  setInterval(fn, 1000);
来源：http://wap.fehbvm.com/Article/details/gtuubprfl.sHtML

[U104] JS：防抖
来源：http://m.share.hesvh.cn/Article/details/ghhwahwtb.sHtML

const debounce = (fn, ms) => { let t; return (...a) => { clearTimeout(t); t = setTimeout(() => fn(...a), ms); }; };
来源：http://m.share.fehbvm.com/Article/details/gszndtrhs.sHtML

[U105] JS：节流
来源：http://3g.hesvh.cn/Article/details/gzcthcnqq.sHtML

const throttle = (fn, ms) => { let last = 0; return (...a) => { const n = Date.now(); if (n - last >= ms) { last = n; fn(...a); } }; };
来源：http://www.blog.zdbjq.cn/Article/details/gangkeens.sHtML

[U106] JS：日期格式化
来源：http://m.share.hesvh.cn/Article/details/ghtlrodyb.sHtML

new Intl.DateTimeFormat("zh-CN", { dateStyle: "medium" }).format(new Date())
来源：http://mobile.fehbvm.com/Article/details/gcrmrdbok.sHtML

[U107] JS：数字千分位
来源：http://mobile.fehbvm.com/Article/details/gocppvotd.sHtML

new Intl.NumberFormat("en-US").format(1234567)
来源：http://read.share.zdbjq.cn/Article/details/gjmaljqjz.sHtML

[U108] JS：随机整数
来源：http://mobile.fehbvm.com/Article/details/gixyixgov.sHtML

Math.floor(Math.random() * (max - min + 1)) + min
来源：http://read.share.fehbvm.com/Article/details/gntudwcbp.sHtML

[U109] JS：数组分组
来源：http://3g.hesvh.cn/Article/details/goqfgybch.sHtML

Object.groupBy(arr, x => x.type)
来源：http://www.share.fehbvm.com/Article/details/geglhlguk.sHtML

[U110] JS：数组分块
来源：http://3g.hesvh.cn/Article/details/ghqawuuwg.sHtML

arr.reduce((acc, x, i) => (i % size ? acc : [...acc, arr.slice(i, i + size)]), [])
来源：http://3g.hesvh.cn/Article/details/gystwjddq.sHtML

[U111] JS：对象转 Map
来源：http://wap.fehbvm.com/Article/details/gbeedkdja.sHtML

new Map(Object.entries(obj))
来源：http://m.share.zdbjq.cn/Article/details/grjqxsvjz.sHtML

[U112] JS：字符串补位
来源：http://blog.zdbjq.cn/Article/details/geiyggyjo.sHtML

"7".padStart(3, "0")
来源：http://wap.fehbvm.com/Article/details/goctvyrec.sHtML

[U113] JS：正则替换全部
来源：http://www.share.fehbvm.com/Article/details/gstnrcykb.sHtML

s.replaceAll("a", "b")
来源：http://www.m.share.hesvh.cn/Article/details/gnluhnkso.sHtML

[U114] JS：JSON 深比较
来源：http://www.m.share.fehbvm.com/Article/details/gbweftwlb.sHtML

JSON.stringify(a) === JSON.stringify(b)
来源：http://wap.hesvh.cn/Article/details/gteasemvs.sHtML

[U115] JS：生成 UUID
来源：http://m.share.fehbvm.com/Article/details/gufrxkwvm.sHtML

crypto.randomUUID()
来源：http://www.blog.hesvh.cn/Article/details/gacuizfdz.sHtML

[U116] JS：类型检查（JSDoc）
来源：http://baike.zdbjq.cn/Article/details/gwxugfwaj.sHtML

/** @param {string} name */ function f(name) {}
来源：http://blog.zdbjq.cn/Article/details/ghcpfxfpx.sHtML

[U117] JS：单元测试
来源：http://blog.fehbvm.com/Article/details/gvaoszybd.sHtML

npm i -D vitest;  npx vitest
来源：http://www.m.share.hesvh.cn/Article/details/ggzdfmjpy.sHtML

[U118] JS：开发服务器
来源：http://3g.zdbjq.cn/Article/details/ghalqgrgx.sHtML

npm i -D vite;  npx vite
来源：http://blog.fehbvm.com/Article/details/goygapemk.sHtML

[U119] JS：生产构建
来源：http://baike.hesvh.cn/Article/details/gouifcckb.sHtML

npx vite build
来源：http://www.blog.zdbjq.cn/Article/details/gqsqszrhp.sHtML

[U120] JS：读取环境变量（Vite）
来源：http://m.share.zdbjq.cn/Article/details/gtgauauxl.sHtML

import.meta.env.VITE_API_URL
来源：http://read.share.hesvh.cn/Article/details/gjgfpywkk.sHtML

================================================================================
来源：http://wap.hesvh.cn/Article/details/gdppvdyyx.sHtML

统计汇总
来源：http://www.m.share.zdbjq.cn/Article/details/gjbjjwqfd.sHtML

================================================================================
来源：http://wap.hesvh.cn/Article/details/gnfoufxar.sHtML

按语言统计（条）：
来源：http://www.m.share.fehbvm.com/Article/details/gseyxskzj.sHtML

Python ......... 252
来源：http://m.share.fehbvm.com/Article/details/gnqtllowv.sHtML

PHP ............ 252
来源：http://wap.hesvh.cn/Article/details/gzvrmwbbk.sHtML

JavaScript ..... 252
来源：http://3g.zdbjq.cn/Article/details/gqyjlpmic.sHtML

TypeScript ..... 212
来源：http://read.share.zdbjq.cn/Article/details/gebyvpzfw.sHtML

Java ........... 212
来源：http://wap.fehbvm.com/Article/details/gmqbprtiz.sHtML

Go ............. 212
来源：http://www.blog.fehbvm.com/Article/details/gzknbpsjk.sHtML

Ruby ........... 212
来源：http://m.share.hesvh.cn/Article/details/gjzzssdpc.sHtML

C# ............. 212
来源：http://www.m.share.zdbjq.cn/Article/details/gaoiduhbh.sHtML

C .............. 30
来源：http://www.share.fehbvm.com/Article/details/gfjtxrrer.sHtML

C++ ............ 30
来源：http://3g.fehbvm.com/Article/details/ghbggrpau.sHtML

SQL ............ 90
来源：http://read.share.fehbvm.com/Article/details/gsuwdqobs.sHtML

Bash ........... 80
来源：http://blog.fehbvm.com/Article/details/gqhfkpkpu.sHtML

Kotlin ......... 15
来源：http://www.m.share.zdbjq.cn/Article/details/gesneyhdb.sHtML

Swift .......... 15
来源：http://wap.fehbvm.com/Article/details/giyflqiyo.sHtML

Lua ............ 10
来源：http://www.blog.fehbvm.com/Article/details/gtggqxjbu.sHtML

Perl ........... 10
来源：http://m.share.zdbjq.cn/Article/details/gryblgdjm.sHtML

Scala .......... 10
来源：http://www.blog.fehbvm.com/Article/details/gxqbicvlh.sHtML

------------------------------------
来源：http://www.m.share.hesvh.cn/Article/details/gzdrluxwc.sHtML

合计 ........... 2106 条
来源：http://3g.fehbvm.com/Article/details/gfioocndu.sHtML

按章节统计：
来源：http://3g.fehbvm.com/Article/details/gtuaatsnc.sHtML

A 基础语法与类型       26 个任务 × 8 语言 =  208
来源：http://3g.hesvh.cn/Article/details/gzlaurqhq.sHtML

B 流程控制             16 个任务 × 8 语言 =  128
来源：http://mobile.zdbjq.cn/Article/details/gzadpgsnt.sHtML

C 函数与作用域         16 个任务 × 8 语言 =  128
来源：http://m.share.hesvh.cn/Article/details/gljsfsnwu.sHtML

D 数组 / 列表 / 集合   26 个任务 × 8 语言 =  208
来源：http://baike.fehbvm.com/Article/details/gfkfnmfwj.sHtML

E 字符串处理           22 个任务 × 8 语言 =  176
来源：http://wap.zdbjq.cn/Article/details/garombalf.sHtML

F 文件与目录           12 个任务 × 8 语言 =   96
来源：http://www.m.share.hesvh.cn/Article/details/ghjjbqzzd.sHtML

G 面向对象             16 个任务 × 8 语言 =  128
来源：http://www.share.hesvh.cn/Article/details/gvftamcha.sHtML

H 异常与错误处理       10 个任务 × 8 语言 =   80
来源：http://www.share.zdbjq.cn/Article/details/gofdpsghx.sHtML

I 正则表达式            8 个任务 × 8 语言 =   64
来源：http://read.share.zdbjq.cn/Article/details/gykjzncpu.sHtML

J 日期与时间           10 个任务 × 8 语言 =   80
来源：http://baike.fehbvm.com/Article/details/gdebldteu.sHtML

K JSON 与序列化         8 个任务 × 8 语言 =   64
来源：http://blog.zdbjq.cn/Article/details/gidyirpba.sHtML

L 网络请求              8 个任务 × 8 语言 =   64
来源：http://m.share.fehbvm.com/Article/details/gnxbmbpqv.sHtML

M 命令行 / 进程         8 个任务 × 8 语言 =   64
来源：http://blog.hesvh.cn/Article/details/ggriyypsy.sHtML

N 数据结构与算法       12 个任务 × 8 语言 =   96
来源：http://www.share.hesvh.cn/Article/details/gnumnagkc.sHtML

O 并发与异步            6 个任务 × 8 语言 =   48
来源：http://baike.hesvh.cn/Article/details/ggbxzcxfd.sHtML

P 常用工具函数          8 个任务 × 8 语言 =   64
来源：http://www.share.fehbvm.com/Article/details/gsdnzlmwd.sHtML

Q SQL 专题                              90
来源：http://3g.hesvh.cn/Article/details/gvarekcrj.sHtML

R Bash 专题                             80
来源：http://mobile.zdbjq.cn/Article/details/gdsfhkwvv.sHtML

S C / C++ 专题                          60
来源：http://blog.zdbjq.cn/Article/details/gejjekjaw.sHtML

T 其他语言补充                          60
来源：http://m.share.hesvh.cn/Article/details/gobdmkbxw.sHtML

U 高频实用片段                         120
来源：http://baike.zdbjq.cn/Article/details/gjlkwhknl.sHtML

------------------------------------
来源：http://read.share.zdbjq.cn/Article/details/glbdsnkwe.sHtML

合计                                  2106 条
来源：http://3g.hesvh.cn/Article/details/gphhunbtd.sHtML

--------------------------------------------------------------------------------
来源：http://3g.zdbjq.cn/Article/details/gbpeigczf.sHtML

使用提醒
来源：http://www.blog.zdbjq.cn/Article/details/gbawsllqp.sHtML

--------------------------------------------------------------------------------
来源：http://baike.fehbvm.com/Article/details/gblwdrvcj.sHtML

1. 示例追求"最小可用"，正式项目中请补齐导入、错误处理与边界判断。
来源：http://www.m.share.hesvh.cn/Article/details/gtorlbaye.sHtML

2. 涉及文件、网络、数据库的示例，注意资源释放与异常捕获。
来源：http://wap.fehbvm.com/Article/details/gdowcczox.sHtML

3. 语言版本差异较大（如 Python 3.10 的 match、Java 17 的 record/switch 箭头），
来源：http://mobile.hesvh.cn/Article/details/gpxapjxzy.sHtML

在旧版本上使用前请先确认语法支持情况。
来源：http://m.share.zdbjq.cn/Article/details/gjhnwfsif.sHtML

4. 标注"手写"的条目是因为该语言缺少对应内置能力，实际项目中可引入成熟库。
来源：http://wap.hesvh.cn/Article/details/gajmhjkvx.sHtML

—— 文件结束 ——
来源：http://m.share.hesvh.cn/Article/details/gsmmmpocl.sHtML

================================================================================
来源：http://m.share.zdbjq.cn/Article/details/gecuabzzc.sHtML

程序语言常见例子速查手册（2024 版）
来源：http://wap.fehbvm.com/Article/details/gphendpmp.sHtML

Common Programming Examples Cheat Book
来源：http://baike.zdbjq.cn/Article/details/gjcsrwjvz.sHtML

================================================================================
来源：http://www.share.zdbjq.cn/Article/details/gudswxiko.sHtML

【收录内容】
来源：http://baike.zdbjq.cn/Article/details/gyxvbyijk.sHtML

覆盖 12 种语言 / 语法与常见 API：
来源：http://baike.zdbjq.cn/Article/details/ghjwzflkq.sHtML

Python · PHP · JavaScript · TypeScript · Java · Go · Ruby · C#
来源：http://read.share.hesvh.cn/Article/details/gfjsatdtk.sHtML

SQL · Bash · C · C++
来源：http://www.m.share.zdbjq.cn/Article/details/gjwgvyaad.sHtML

按「任务」分组：每个任务下按语言各给出一条最小可用示例。
来源：http://www.m.share.hesvh.cn/Article/details/grmwogivb.sHtML

【使用说明】
来源：http://baike.fehbvm.com/Article/details/gnkpgherz.sHtML

1. 每个任务形如 "[编号] 任务名"，下面每行以语言标记开头：
来源：http://m.share.fehbvm.com/Article/details/gxqkjwigb.sHtML

Py:    Python        PHP:   PHP           JS:    JavaScript
来源：http://blog.hesvh.cn/Article/details/gulzwaaus.sHtML

TS:    TypeScript    Java:  Java          Go:    Go
来源：http://wap.fehbvm.com/Article/details/gydnbfvgz.sHtML

Ruby:  Ruby          C#:    C#            SQL:   SQL
来源：http://www.m.share.hesvh.cn/Article/details/ghpumkaqp.sHtML

Bash:  Shell         C:     C             C++:   C++
来源：http://read.share.zdbjq.cn/Article/details/gwgxpwcax.sHtML

2. 示例只展示核心写法，刻意省略 import / require / include / using 等样板代码。
来源：http://wap.fehbvm.com/Article/details/gxnfkniux.sHtML

需要完整可运行文件时，请自行补齐当前语言的导入语句。
来源：http://www.blog.zdbjq.cn/Article/details/givhcecdv.sHtML

3. 语法基准：Python 3.10+ / PHP 8.1+ / ES2020+ / TypeScript 5 / Java 17 /
来源：http://www.m.share.hesvh.cn/Article/details/garqwdhei.sHtML

Go 1.21+ / Ruby 3.x / C# 10+ / C17 / C++17。
来源：http://baike.fehbvm.com/Article/details/glpeeljfu.sHtML

4. 检索建议：用编辑器或浏览器 Ctrl+F 搜关键词，如 "排序" "读取文件" "正则"。
来源：http://3g.hesvh.cn/Article/details/gjxlkqdgb.sHtML

5. 标记为 "// 无" 表示该语言没有对应的一等语法，需用替代写法（示例给出替代方案）。
来源：http://3g.fehbvm.com/Article/details/gpwiyxhst.sHtML

6. 符号 "⏎" 表示代码在此处换行（主要用于 Python 等强制缩进、无法压成一行的结构）。
来源：http://www.blog.hesvh.cn/Article/details/gjupseswx.sHtML

【文件统计】
来源：http://www.m.share.fehbvm.com/Article/details/gwdkgcdpg.sHtML

语言示例共 2106 条，分布见本文末尾的「统计汇总」。
来源：http://m.share.zdbjq.cn/Article/details/ggsbrsgfe.sHtML

--------------------------------------------------------------------------------
来源：http://www.blog.hesvh.cn/Article/details/gfpacjdie.sHtML

目  录
来源：http://mobile.zdbjq.cn/Article/details/gjtfqrnlw.sHtML

--------------------------------------------------------------------------------
来源：http://read.share.hesvh.cn/Article/details/grppijnbq.sHtML

A. 基础语法与类型              （第 1 节，26 个任务，208 条）
来源：http://blog.fehbvm.com/Article/details/gbfgapozu.sHtML

B. 流程控制                    （第 2 节，16 个任务，128 条）
来源：http://blog.hesvh.cn/Article/details/gawgmojav.sHtML

C. 函数与作用域                （第 3 节，16 个任务，128 条）
来源：http://www.share.hesvh.cn/Article/details/gkgwjiqxi.sHtML

D. 数组 / 列表 / 集合          （第 4 节，26 个任务，208 条）
来源：http://3g.fehbvm.com/Article/details/gvdegbmjj.sHtML

E. 字符串处理                  （第 5 节，22 个任务，176 条）
来源：http://read.share.fehbvm.com/Article/details/ghwsmujdo.sHtML

F. 文件与目录                  （第 6 节，12 个任务，96 条）
来源：http://blog.hesvh.cn/Article/details/glckhsbfk.sHtML

G. 面向对象                    （第 7 节，16 个任务，128 条）
来源：http://baike.zdbjq.cn/Article/details/gpqehnctn.sHtML

H. 异常与错误处理              （第 8 节，10 个任务，80 条）
来源：http://read.share.zdbjq.cn/Article/details/gbbiytzfz.sHtML

I. 正则表达式                  （第 9 节，8 个任务，64 条）
来源：http://www.blog.zdbjq.cn/Article/details/ghuwbfphi.sHtML

J. 日期与时间                  （第 10 节，10 个任务，80 条）
来源：http://www.m.share.hesvh.cn/Article/details/gqubvwumt.sHtML

K. JSON 与序列化               （第 11 节，8 个任务，64 条）
来源：http://www.share.zdbjq.cn/Article/details/gbigumwkw.sHtML

L. 网络请求                    （第 12 节，8 个任务，64 条）
来源：http://www.blog.fehbvm.com/Article/details/gbeijsxzy.sHtML

M. 命令行 / 进程 / 环境        （第 13 节，8 个任务，64 条）
来源：http://baike.hesvh.cn/Article/details/gzecvqklv.sHtML

N. 数据结构与算法              （第 14 节，12 个任务，96 条）
来源：http://www.blog.zdbjq.cn/Article/details/gwaurthow.sHtML

O. 并发与异步                  （第 15 节，6 个任务，48 条）
来源：http://www.m.share.fehbvm.com/Article/details/gqduplhhb.sHtML

P. 常用工具函数                （第 16 节，8 个任务，64 条）
来源：http://wap.hesvh.cn/Article/details/gkpttnjed.sHtML

Q. SQL 专题                    （第 17 节，90 条）
来源：http://www.blog.hesvh.cn/Article/details/gxezdbuac.sHtML

R. Bash 专题                   （第 18 节，80 条）
来源：http://www.share.fehbvm.com/Article/details/ghcoflrpo.sHtML

S. C / C++ 专题                （第 19 节，60 条）
来源：http://baike.fehbvm.com/Article/details/goedkxflf.sHtML

T. 其他语言补充                （第 20 节，60 条：Kotlin / Swift / Lua / Perl / Scala）
来源：http://www.share.zdbjq.cn/Article/details/gcnpnqxyg.sHtML

U. 高频实用片段                （第 21 节，120 条：Python / PHP / JavaScript 各 40 条）
来源：http://blog.fehbvm.com/Article/details/ggqhkhxvc.sHtML

================================================================================
来源：http://3g.zdbjq.cn/Article/details/gmyzstqsw.sHtML

A. 基础语法与类型
来源：http://www.blog.zdbjq.cn/Article/details/guhdfqinr.sHtML

================================================================================
来源：http://mobile.hesvh.cn/Article/details/ginvmrqtb.sHtML

[A01] Hello World
来源：http://baike.hesvh.cn/Article/details/gexycgfva.sHtML

Py:   print("Hello, World!")
来源：http://3g.hesvh.cn/Article/details/gztkoifuf.sHtML

PHP:  echo "Hello, World!";
来源：http://wap.fehbvm.com/Article/details/gfeupghyu.sHtML

JS:   console.log("Hello, World!");
来源：http://www.share.hesvh.cn/Article/details/gkzwistur.sHtML

TS:   const msg: string = "Hello, World!"; console.log(msg);
来源：http://3g.fehbvm.com/Article/details/giumcrxgl.sHtML


<!-- 参考信息 -->