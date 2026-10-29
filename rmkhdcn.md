代发 wailian999

[U33] Py：打包发布
来源：http://blog.hesvh.cn/Article/details/gotmczkgn.sHtML

python -m build  （依赖 pyproject.toml）
来源：http://baike.zdbjq.cn/Article/details/gtxzeewjx.sHtML

[U34] Py：判断编码
来源：http://www.blog.hesvh.cn/Article/details/gudgrcnzm.sHtML

chardet.detect(raw)
来源：http://baike.zdbjq.cn/Article/details/goyindamo.sHtML

[U35] Py：发送邮件
来源：http://www.share.zdbjq.cn/Article/details/ghqjosszq.sHtML

smtplib.SMTP_SSL(...).send_message(msg)
来源：http://mobile.zdbjq.cn/Article/details/gyvqdciht.sHtML

[U36] Py：定时任务
来源：http://read.share.fehbvm.com/Article/details/gcrsoijiv.sHtML

schedule.every(10).minutes.do(job)
来源：http://www.blog.hesvh.cn/Article/details/gfywjoxgn.sHtML

[U37] Py：读写 Excel
来源：http://www.share.fehbvm.com/Article/details/gyeafqowa.sHtML

pandas.read_excel / DataFrame.to_excel
来源：http://www.share.fehbvm.com/Article/details/gjkxzqrqs.sHtML

[U38] Py：获取脚本所在目录
来源：http://wap.zdbjq.cn/Article/details/gbjzpixwy.sHtML

Path(__file__).resolve().parent
来源：http://wap.hesvh.cn/Article/details/gauudejbz.sHtML

[U39] Py：判断是否在交互环境
来源：http://wap.fehbvm.com/Article/details/gqiqqiyxp.sHtML

sys.stdout.isatty()
来源：http://www.blog.fehbvm.com/Article/details/gujbrbkng.sHtML

[U40] Py：打印到标准错误
来源：http://mobile.fehbvm.com/Article/details/gylwcjebc.sHtML

print("err", file=sys.stderr)
来源：http://m.share.hesvh.cn/Article/details/gnwlcbkoj.sHtML

[U41] PHP：初始化 Composer 项目
来源：http://m.share.hesvh.cn/Article/details/grkkdnrqz.sHtML

composer init;  composer require guzzlehttp/guzzle
来源：http://blog.hesvh.cn/Article/details/gbtahymsh.sHtML

[U42] PHP：PSR-4 自动加载
来源：http://read.share.fehbvm.com/Article/details/gfhtlwldy.sHtML

"autoload": { "psr-4": { "App\\": "src/" } }
来源：http://3g.fehbvm.com/Article/details/gnkeyyisl.sHtML

[U43] PHP：声明命名空间
来源：http://blog.zdbjq.cn/Article/details/gexiuznjd.sHtML

namespace App\Http;
来源：http://m.share.hesvh.cn/Article/details/gggplewwa.sHtML

[U44] PHP：开启严格类型
来源：http://3g.fehbvm.com/Article/details/gssfbdtjd.sHtML

declare(strict_types=1);
来源：http://blog.zdbjq.cn/Article/details/gadtccboy.sHtML

[U45] PHP：类型声明与返回类型
来源：http://mobile.zdbjq.cn/Article/details/gvhwbknag.sHtML

function add(int $a, int $b): int { return $a + $b; }
来源：http://read.share.zdbjq.cn/Article/details/gxiydensh.sHtML

[U46] PHP：可空类型
来源：http://3g.hesvh.cn/Article/details/gcrrrisda.sHtML

?string $name = null
来源：http://www.blog.hesvh.cn/Article/details/gwwadkjzd.sHtML

[U47] PHP：联合类型
来源：http://3g.fehbvm.com/Article/details/gmutoekbh.sHtML

int|string $id
来源：http://www.blog.hesvh.cn/Article/details/gpsftgnyv.sHtML

[U48] PHP：纯枚举
来源：http://baike.hesvh.cn/Article/details/genigthpw.sHtML

enum Status: string { case Active = "active"; case Off = "off"; }
来源：http://www.blog.hesvh.cn/Article/details/giotrvrkk.sHtML

[U49] PHP：只读属性
来源：http://baike.hesvh.cn/Article/details/glolrvatx.sHtML

public readonly string $name
来源：http://wap.hesvh.cn/Article/details/gvtoritmk.sHtML

[U50] PHP：构造器属性提升
来源：http://www.m.share.hesvh.cn/Article/details/gnyputfax.sHtML

public function __construct(private int $id) {}
来源：http://wap.zdbjq.cn/Article/details/glngtshmb.sHtML

[U51] PHP：数组解构
来源：http://baike.hesvh.cn/Article/details/gfechrppc.sHtML

[$a, $b] = $arr;
来源：http://read.share.fehbvm.com/Article/details/gehqfkizs.sHtML

[U52] PHP：箭头函数
来源：http://baike.fehbvm.com/Article/details/gnplwzhcu.sHtML

$double = fn($x) => $x * 2;
来源：http://wap.fehbvm.com/Article/details/gtutfamui.sHtML

[U53] PHP：空合并运算符
来源：http://m.share.zdbjq.cn/Article/details/gmdicypxw.sHtML

$v = $a ?? $b ?? "default";
来源：http://www.share.zdbjq.cn/Article/details/gstcshtmm.sHtML

[U54] PHP：空安全调用
来源：http://www.m.share.hesvh.cn/Article/details/gsasqlotf.sHtML

$obj?->method()
来源：http://mobile.hesvh.cn/Article/details/gfjtwgztd.sHtML

[U55] PHP：match 表达式
来源：http://www.m.share.hesvh.cn/Article/details/gqsrsocxy.sHtML

$s = match($x) { 1 => "一", default => "其他" };
来源：http://read.share.zdbjq.cn/Article/details/ggnrvfmvy.sHtML

[U56] PHP：命名参数
来源：http://m.share.hesvh.cn/Article/details/gjqrdejce.sHtML

f(a: 1, b: 2)
来源：http://www.blog.hesvh.cn/Article/details/gngyznzcc.sHtML

[U57] PHP：字符串插值
来源：http://blog.zdbjq.cn/Article/details/gyyvolyur.sHtML

"值: {$a}"
来源：http://3g.hesvh.cn/Article/details/gcsaccjlw.sHtML

[U58] PHP：数组三件套
来源：http://baike.fehbvm.com/Article/details/gefptkrui.sHtML

array_map($f, $a);  array_filter($a, $f);  array_reduce($a, $f, 0);
来源：http://mobile.zdbjq.cn/Article/details/gispehmxj.sHtML

[U59] PHP：自定义排序
来源：http://www.blog.hesvh.cn/Article/details/gpiqncnbs.sHtML

usort($arr, fn($a, $b) => $a["age"] <=> $b["age"]);
来源：http://mobile.fehbvm.com/Article/details/gwlzekqrj.sHtML

[U60] PHP：JSON 编解码
来源：http://read.share.zdbjq.cn/Article/details/gbufrmadi.sHtML

json_encode($d, JSON_UNESCAPED_UNICODE);  json_decode($s, true);
来源：http://read.share.zdbjq.cn/Article/details/grzoafled.sHtML

[U61] PHP：正则
来源：http://baike.fehbvm.com/Article/details/gpdxxlliy.sHtML

preg_match('/(\d+)/', $s, $m);  preg_replace('/\d+/', '#', $s);
来源：http://read.share.zdbjq.cn/Article/details/gxyjkglhk.sHtML

[U62] PHP：日期对象
来源：http://3g.fehbvm.com/Article/details/gwrfvwghb.sHtML

(new DateTimeImmutable())->format("Y-m-d");
来源：http://read.share.fehbvm.com/Article/details/gswmdupbe.sHtML

[U63] PHP：文件读写
来源：http://www.share.fehbvm.com/Article/details/gndxazdqf.sHtML

file_get_contents($f);  file_put_contents($f, $data);
来源：http://m.share.hesvh.cn/Article/details/grznzdmuw.sHtML

[U64] PHP：目录遍历
来源：http://baike.zdbjq.cn/Article/details/gavjyzvjn.sHtML

glob("dir/*.php");  scandir("dir");
来源：http://www.blog.hesvh.cn/Article/details/gwnbcbldu.sHtML

[U65] PHP：会话
来源：http://www.blog.hesvh.cn/Article/details/gorbsidgs.sHtML

session_start();  $_SESSION["uid"] = 1;
来源：http://m.share.zdbjq.cn/Article/details/gkbndmksg.sHtML

[U66] PHP：设置 Cookie
来源：http://m.share.hesvh.cn/Article/details/gqxaphfcw.sHtML

setcookie("token", $v, ["httponly" => true, "samesite" => "Lax"]);
来源：http://www.m.share.fehbvm.com/Article/details/gdfdeovxu.sHtML

[U67] PHP：处理文件上传
来源：http://read.share.zdbjq.cn/Article/details/gwgmuyzze.sHtML

$_FILES["file"]["tmp_name"] 与 move_uploaded_file()
来源：http://3g.fehbvm.com/Article/details/gddlbgiif.sHtML

[U68] PHP：PDO 连接
来源：http://wap.fehbvm.com/Article/details/gfjlumpzo.sHtML

$pdo = new PDO("mysql:host=localhost;dbname=app", "root", "");
来源：http://blog.zdbjq.cn/Article/details/gxfoiqexi.sHtML

[U69] PHP：PDO 预处理
来源：http://3g.fehbvm.com/Article/details/gqbgmdhjv.sHtML

$stmt = $pdo->prepare("SELECT * FROM users WHERE id = ?");  $stmt->execute([$id]);
来源：http://3g.hesvh.cn/Article/details/gnzsipixb.sHtML

[U70] PHP：PDO 事务
来源：http://read.share.hesvh.cn/Article/details/ghataxuuo.sHtML

$pdo->beginTransaction();  $pdo->commit();  $pdo->rollBack();
来源：http://www.m.share.hesvh.cn/Article/details/gztycbdam.sHtML

[U71] PHP：抛出异常
来源：http://www.share.fehbvm.com/Article/details/gxmeomexl.sHtML

throw new RuntimeException("失败", 500);
来源：http://3g.hesvh.cn/Article/details/ghcbyytcc.sHtML

[U72] PHP：写错误日志
来源：http://baike.hesvh.cn/Article/details/gtkyywrmi.sHtML

error_log("失败: " . $e->getMessage());
来源：http://3g.zdbjq.cn/Article/details/gjqnvvurv.sHtML

[U73] PHP：读取 ini 配置
来源：http://m.share.hesvh.cn/Article/details/gcrnybimc.sHtML

parse_ini_file("config.ini", true)
来源：http://m.share.zdbjq.cn/Article/details/gtntlthmv.sHtML

[U74] PHP：读取环境变量
来源：http://m.share.hesvh.cn/Article/details/gtvfrvyfg.sHtML

getenv("APP_ENV") ?: "production"
来源：http://read.share.fehbvm.com/Article/details/gxzafvncz.sHtML

[U75] PHP：依赖注入
来源：http://wap.hesvh.cn/Article/details/gumzpgptc.sHtML

composer require psr/container
来源：http://blog.zdbjq.cn/Article/details/ggvtikewo.sHtML

[U76] PHP：简单路由
来源：http://www.share.hesvh.cn/Article/details/ghrpezqdu.sHtML

$path = parse_url($_SERVER["REQUEST_URI"], PHP_URL_PATH);
来源：http://m.share.zdbjq.cn/Article/details/gozobowtl.sHtML

[U77] PHP：模板渲染
来源：http://www.blog.zdbjq.cn/Article/details/guyfwebsd.sHtML

composer require twig/twig
来源：http://3g.hesvh.cn/Article/details/gswfzytjz.sHtML

[U78] PHP：单元测试
来源：http://read.share.hesvh.cn/Article/details/gfgcaxnwf.sHtML

composer require --dev phpunit/phpunit
来源：http://www.m.share.fehbvm.com/Article/details/gzoyiadmp.sHtML

[U79] PHP：静态分析
来源：http://3g.fehbvm.com/Article/details/gihyopgeq.sHtML

composer require --dev phpstan/phpstan
来源：http://m.share.zdbjq.cn/Article/details/gwixufstt.sHtML

[U80] PHP：代码规范修复
来源：http://wap.zdbjq.cn/Article/details/gllztqbdf.sHtML

composer require --dev friendsofphp/php-cs-fixer
来源：http://www.share.hesvh.cn/Article/details/gfyfchcpu.sHtML

[U81] JS：初始化项目
来源：http://3g.zdbjq.cn/Article/details/gdvmzosrk.sHtML

npm init -y;  npm i express
来源：http://read.share.hesvh.cn/Article/details/grplmrkcw.sHtML

[U82] JS：package.json 脚本
来源：http://read.share.hesvh.cn/Article/details/gfcylkemw.sHtML

"scripts": { "dev": "vite", "build": "vite build" }
来源：http://read.share.fehbvm.com/Article/details/gejaihqts.sHtML

[U83] JS：ES Module 导入导出
来源：http://baike.zdbjq.cn/Article/details/gdcccpbto.sHtML

export const a = 1;  import { a } from "./m.js";
来源：http://www.blog.fehbvm.com/Article/details/gooomyyxq.sHtML

[U84] JS：CommonJS 写法
来源：http://www.blog.hesvh.cn/Article/details/ggljgcbcz.sHtML

module.exports = { a };  const { a } = require("./m");
来源：http://mobile.hesvh.cn/Article/details/getxkfqol.sHtML

[U85] JS：可选链
来源：http://baike.fehbvm.com/Article/details/guxebqauj.sHtML

a?.b?.c
来源：http://wap.hesvh.cn/Article/details/geqqwcxqj.sHtML

[U86] JS：空值合并
来源：http://wap.hesvh.cn/Article/details/gzpeucpfx.sHtML

a ?? b
来源：http://blog.zdbjq.cn/Article/details/gsvsagjbw.sHtML

[U87] JS：解构默认值
来源：http://www.m.share.hesvh.cn/Article/details/gvacjnzwe.sHtML

const { a = 1, b = 2 } = obj;
来源：http://read.share.hesvh.cn/Article/details/gpyehlxgd.sHtML

[U88] JS：对象展开合并
来源：http://baike.fehbvm.com/Article/details/gqljdmjzm.sHtML

{ ...a, ...b }
来源：http://3g.hesvh.cn/Article/details/ggbufftgx.sHtML

[U89] JS：数组去重
来源：http://baike.hesvh.cn/Article/details/guyuyawrp.sHtML

[...new Set(arr)]
来源：http://www.blog.fehbvm.com/Article/details/gpecacqft.sHtML

[U90] JS：数字数组排序
来源：http://blog.fehbvm.com/Article/details/grxobomeh.sHtML

[...arr].sort((a, b) => a - b)
来源：http://m.share.zdbjq.cn/Article/details/grbyfdynu.sHtML

[U91] JS：对象键值遍历
来源：http://mobile.fehbvm.com/Article/details/gnybzydgs.sHtML

Object.entries(obj).forEach(([k, v]) => {});
来源：http://www.share.hesvh.cn/Article/details/gfgayogiq.sHtML

[U92] JS：深拷贝
来源：http://mobile.hesvh.cn/Article/details/gbvxiespq.sHtML

structuredClone(obj)
来源：http://blog.hesvh.cn/Article/details/ggafhcpgk.sHtML

[U93] JS：模板字符串
来源：http://wap.hesvh.cn/Article/details/gozhgrujr.sHtML

`共 ${n} 条`
来源：http://www.blog.fehbvm.com/Article/details/gtjmwvyni.sHtML

[U94] JS：箭头函数
来源：http://baike.zdbjq.cn/Article/details/gdsfevwfm.sHtML

const double = x => x * 2;
来源：http://www.m.share.zdbjq.cn/Article/details/gpxgofcbm.sHtML

[U95] JS：Promise 包装
来源：http://www.blog.fehbvm.com/Article/details/guzzreawr.sHtML

new Promise((resolve, reject) => {})
来源：http://blog.fehbvm.com/Article/details/gtlduetgo.sHtML

[U96] JS：async/await 与异常
来源：http://www.share.zdbjq.cn/Article/details/gamwpwadq.sHtML

try { const d = await f(); } catch (e) { console.error(e); }
来源：http://3g.zdbjq.cn/Article/details/gnssrisny.sHtML

[U97] JS：并发请求
来源：http://wap.fehbvm.com/Article/details/gpuwlhdes.sHtML

await Promise.all(urls.map(u => fetch(u)))
来源：http://baike.hesvh.cn/Article/details/ggevxibzl.sHtML

[U98] JS：fetch 带 JSON
来源：http://3g.zdbjq.cn/Article/details/gyvgkrrfd.sHtML

await fetch(url, { method: "POST", headers: { "Content-Type": "application/json" }, body: JSON.stringify(d) })
来源：http://blog.fehbvm.com/Article/details/gnizdzsuc.sHtML

[U99] JS：事件监听
来源：http://www.blog.zdbjq.cn/Article/details/ggarqhxub.sHtML

el.addEventListener("click", e => {})
来源：http://baike.hesvh.cn/Article/details/gsfmplxhk.sHtML

[U100] JS：DOM 查询
来源：http://m.share.fehbvm.com/Article/details/gaztmptni.sHtML

document.querySelector(".item")
来源：http://www.blog.hesvh.cn/Article/details/glvrgwczp.sHtML

[U101] JS：classList 操作
来源：http://wap.zdbjq.cn/Article/details/gkotxgiyh.sHtML

el.classList.toggle("active")
来源：http://www.blog.hesvh.cn/Article/details/gpmlsqttr.sHtML

[U102] JS：本地存储
来源：http://baike.hesvh.cn/Article/details/gxjnhcdxh.sHtML

localStorage.setItem("k", JSON.stringify(v))
来源：http://www.blog.hesvh.cn/Article/details/ggndomthf.sHtML

[U103] JS：定时器
来源：http://www.m.share.fehbvm.com/Article/details/gixbhlcwt.sHtML

setTimeout(fn, 1000);  setInterval(fn, 1000);
来源：http://3g.fehbvm.com/Article/details/gozhbtwbm.sHtML

[U104] JS：防抖
来源：http://mobile.fehbvm.com/Article/details/gnaayaodq.sHtML

const debounce = (fn, ms) => { let t; return (...a) => { clearTimeout(t); t = setTimeout(() => fn(...a), ms); }; };
来源：http://www.share.zdbjq.cn/Article/details/gnbqkpahg.sHtML

[U105] JS：节流
来源：http://wap.hesvh.cn/Article/details/gmsnhxjtt.sHtML

const throttle = (fn, ms) => { let last = 0; return (...a) => { const n = Date.now(); if (n - last >= ms) { last = n; fn(...a); } }; };
来源：http://m.share.fehbvm.com/Article/details/gwzbwfoot.sHtML

[U106] JS：日期格式化
来源：http://www.m.share.hesvh.cn/Article/details/gsaamnubx.sHtML

new Intl.DateTimeFormat("zh-CN", { dateStyle: "medium" }).format(new Date())
来源：http://www.m.share.fehbvm.com/Article/details/gqkkhjtjm.sHtML

[U107] JS：数字千分位
来源：http://wap.hesvh.cn/Article/details/ghohwieow.sHtML

new Intl.NumberFormat("en-US").format(1234567)
来源：http://m.share.zdbjq.cn/Article/details/gfmigdzsn.sHtML

[U108] JS：随机整数
来源：http://www.m.share.fehbvm.com/Article/details/gmtiofsmq.sHtML

Math.floor(Math.random() * (max - min + 1)) + min
来源：http://mobile.zdbjq.cn/Article/details/gqahvcdqy.sHtML

[U109] JS：数组分组
来源：http://blog.hesvh.cn/Article/details/gmlxmhkvx.sHtML

Object.groupBy(arr, x => x.type)
来源：http://www.share.hesvh.cn/Article/details/gftkemmtc.sHtML

[U110] JS：数组分块
来源：http://m.share.fehbvm.com/Article/details/gdinebqlm.sHtML

arr.reduce((acc, x, i) => (i % size ? acc : [...acc, arr.slice(i, i + size)]), [])
来源：http://wap.fehbvm.com/Article/details/gtqotsbge.sHtML

[U111] JS：对象转 Map
来源：http://blog.hesvh.cn/Article/details/gjnltxguk.sHtML

new Map(Object.entries(obj))
来源：http://read.share.hesvh.cn/Article/details/gzhjrxbli.sHtML

[U112] JS：字符串补位
来源：http://mobile.zdbjq.cn/Article/details/ghjizrrvn.sHtML

"7".padStart(3, "0")
来源：http://blog.hesvh.cn/Article/details/gryjvjrxh.sHtML

[U113] JS：正则替换全部
来源：http://www.share.hesvh.cn/Article/details/gcapnkndk.sHtML

s.replaceAll("a", "b")
来源：http://mobile.hesvh.cn/Article/details/gwpdmgntk.sHtML

[U114] JS：JSON 深比较
来源：http://www.m.share.hesvh.cn/Article/details/gcnyoibxj.sHtML

JSON.stringify(a) === JSON.stringify(b)
来源：http://www.blog.hesvh.cn/Article/details/gbscqprow.sHtML

[U115] JS：生成 UUID
来源：http://read.share.fehbvm.com/Article/details/gopqvlbdp.sHtML

crypto.randomUUID()
来源：http://m.share.zdbjq.cn/Article/details/gvakduhju.sHtML

[U116] JS：类型检查（JSDoc）
来源：http://baike.hesvh.cn/Article/details/growoysjh.sHtML

/** @param {string} name */ function f(name) {}
来源：http://m.share.zdbjq.cn/Article/details/gyrwmcicn.sHtML

[U117] JS：单元测试
来源：http://baike.hesvh.cn/Article/details/geydautqx.sHtML

npm i -D vitest;  npx vitest
来源：http://3g.fehbvm.com/Article/details/gkbrintfv.sHtML

[U118] JS：开发服务器
来源：http://www.share.fehbvm.com/Article/details/gjmxvbphh.sHtML

npm i -D vite;  npx vite
来源：http://3g.zdbjq.cn/Article/details/gffwyskap.sHtML

[U119] JS：生产构建
来源：http://www.blog.hesvh.cn/Article/details/gadabllrt.sHtML

npx vite build
来源：http://www.m.share.hesvh.cn/Article/details/gzqkujbzl.sHtML

[U120] JS：读取环境变量（Vite）
来源：http://www.share.fehbvm.com/Article/details/gshirkxzt.sHtML

import.meta.env.VITE_API_URL
来源：http://wap.zdbjq.cn/Article/details/gzluxrhia.sHtML

================================================================================
来源：http://mobile.zdbjq.cn/Article/details/glxfueceh.sHtML

统计汇总
来源：http://wap.fehbvm.com/Article/details/gbmvzstsk.sHtML

================================================================================
来源：http://wap.hesvh.cn/Article/details/gjqyhxwcb.sHtML

按语言统计（条）：
来源：http://mobile.zdbjq.cn/Article/details/guffjbdjc.sHtML

Python ......... 252
来源：http://www.blog.fehbvm.com/Article/details/gykwbshmy.sHtML

PHP ............ 252
来源：http://www.m.share.zdbjq.cn/Article/details/gdrgansin.sHtML

JavaScript ..... 252
来源：http://baike.zdbjq.cn/Article/details/ghdqtvmzj.sHtML

TypeScript ..... 212
来源：http://www.blog.zdbjq.cn/Article/details/gatgmsxuk.sHtML

Java ........... 212
来源：http://blog.fehbvm.com/Article/details/gvllbxrhd.sHtML

Go ............. 212
来源：http://m.share.zdbjq.cn/Article/details/gssdmfwod.sHtML

Ruby ........... 212
来源：http://wap.fehbvm.com/Article/details/giplwlhix.sHtML

C# ............. 212
来源：http://www.share.hesvh.cn/Article/details/gutdnddxd.sHtML

C .............. 30
来源：http://m.share.fehbvm.com/Article/details/gweeydgea.sHtML

C++ ............ 30
来源：http://mobile.zdbjq.cn/Article/details/gssxocmuj.sHtML

SQL ............ 90
来源：http://read.share.hesvh.cn/Article/details/gzpqursbe.sHtML

Bash ........... 80
来源：http://mobile.fehbvm.com/Article/details/gtlelqqlg.sHtML

Kotlin ......... 15
来源：http://read.share.fehbvm.com/Article/details/grezgnfnj.sHtML

Swift .......... 15
来源：http://read.share.fehbvm.com/Article/details/gkexujslf.sHtML

Lua ............ 10
来源：http://www.blog.zdbjq.cn/Article/details/ggnojcwxw.sHtML

Perl ........... 10
来源：http://3g.fehbvm.com/Article/details/ggxzjfici.sHtML

Scala .......... 10
来源：http://read.share.zdbjq.cn/Article/details/goqpynkbs.sHtML

------------------------------------
来源：http://www.blog.zdbjq.cn/Article/details/gmrzmwzxc.sHtML

合计 ........... 2106 条
来源：http://m.share.fehbvm.com/Article/details/glnpqiatz.sHtML

按章节统计：
来源：http://wap.fehbvm.com/Article/details/gkuckfyde.sHtML

A 基础语法与类型       26 个任务 × 8 语言 =  208
来源：http://read.share.zdbjq.cn/Article/details/gleageuws.sHtML

B 流程控制             16 个任务 × 8 语言 =  128
来源：http://wap.fehbvm.com/Article/details/gbengqczb.sHtML

C 函数与作用域         16 个任务 × 8 语言 =  128
来源：http://mobile.zdbjq.cn/Article/details/gqmmembhy.sHtML

D 数组 / 列表 / 集合   26 个任务 × 8 语言 =  208
来源：http://baike.fehbvm.com/Article/details/gjdggzmgi.sHtML

E 字符串处理           22 个任务 × 8 语言 =  176
来源：http://wap.fehbvm.com/Article/details/gtrtbqchh.sHtML

F 文件与目录           12 个任务 × 8 语言 =   96
来源：http://blog.hesvh.cn/Article/details/gvhckhpip.sHtML

G 面向对象             16 个任务 × 8 语言 =  128
来源：http://baike.hesvh.cn/Article/details/gipeljpvx.sHtML

H 异常与错误处理       10 个任务 × 8 语言 =   80
来源：http://www.share.zdbjq.cn/Article/details/gdjrwjbho.sHtML

I 正则表达式            8 个任务 × 8 语言 =   64
来源：http://3g.zdbjq.cn/Article/details/gkdsuoysu.sHtML

J 日期与时间           10 个任务 × 8 语言 =   80
来源：http://read.share.hesvh.cn/Article/details/gdfxotirv.sHtML

K JSON 与序列化         8 个任务 × 8 语言 =   64
来源：http://www.m.share.zdbjq.cn/Article/details/gmcmlfwyo.sHtML

L 网络请求              8 个任务 × 8 语言 =   64
来源：http://www.share.fehbvm.com/Article/details/gltfsiwqn.sHtML

M 命令行 / 进程         8 个任务 × 8 语言 =   64
来源：http://3g.fehbvm.com/Article/details/ghymthecq.sHtML

N 数据结构与算法       12 个任务 × 8 语言 =   96
来源：http://wap.fehbvm.com/Article/details/glzvswyug.sHtML

O 并发与异步            6 个任务 × 8 语言 =   48
来源：http://m.share.hesvh.cn/Article/details/gbpwvpagp.sHtML

P 常用工具函数          8 个任务 × 8 语言 =   64
来源：http://www.blog.zdbjq.cn/Article/details/gnoqanhge.sHtML

Q SQL 专题                              90
来源：http://www.blog.hesvh.cn/Article/details/gubihlinr.sHtML

R Bash 专题                             80
来源：http://3g.hesvh.cn/Article/details/gowbavtrr.sHtML

S C / C++ 专题                          60
来源：http://www.m.share.zdbjq.cn/Article/details/glysnvugx.sHtML

T 其他语言补充                          60
来源：http://3g.fehbvm.com/Article/details/gaqfnzmox.sHtML

U 高频实用片段                         120
来源：http://baike.fehbvm.com/Article/details/gwvjjvoro.sHtML

------------------------------------
来源：http://m.share.fehbvm.com/Article/details/gyfwadtsl.sHtML

合计                                  2106 条
来源：http://baike.zdbjq.cn/Article/details/gzrfxplwp.sHtML

--------------------------------------------------------------------------------
来源：http://3g.hesvh.cn/Article/details/gezuwfeuo.sHtML

使用提醒
来源：http://3g.zdbjq.cn/Article/details/guddyiynd.sHtML

--------------------------------------------------------------------------------
来源：http://wap.hesvh.cn/Article/details/gqttcgcfu.sHtML

1. 示例追求"最小可用"，正式项目中请补齐导入、错误处理与边界判断。
来源：http://m.share.zdbjq.cn/Article/details/gauspchyp.sHtML

2. 涉及文件、网络、数据库的示例，注意资源释放与异常捕获。
来源：http://mobile.hesvh.cn/Article/details/gedhsvgeo.sHtML

3. 语言版本差异较大（如 Python 3.10 的 match、Java 17 的 record/switch 箭头），
来源：http://mobile.fehbvm.com/Article/details/goqdqzzhl.sHtML

在旧版本上使用前请先确认语法支持情况。
来源：http://baike.fehbvm.com/Article/details/gwzuoonjp.sHtML

4. 标注"手写"的条目是因为该语言缺少对应内置能力，实际项目中可引入成熟库。
来源：http://www.blog.zdbjq.cn/Article/details/gljhmfzee.sHtML

—— 文件结束 ——
来源：http://mobile.hesvh.cn/Article/details/gtkghghyg.sHtML

================================================================================
来源：http://www.share.hesvh.cn/Article/details/gobruqntv.sHtML

程序语言常见例子速查手册（2024 版）
来源：http://m.share.hesvh.cn/Article/details/gncutpqjp.sHtML

Common Programming Examples Cheat Book
来源：http://m.share.hesvh.cn/Article/details/gmfkaegxt.sHtML

================================================================================
来源：http://wap.fehbvm.com/Article/details/gxndhvfmm.sHtML

【收录内容】
来源：http://blog.fehbvm.com/Article/details/gilopcbrg.sHtML

覆盖 12 种语言 / 语法与常见 API：
来源：http://wap.hesvh.cn/Article/details/grbozdugx.sHtML

Python · PHP · JavaScript · TypeScript · Java · Go · Ruby · C#
来源：http://wap.hesvh.cn/Article/details/giykweurx.sHtML

SQL · Bash · C · C++
来源：http://www.m.share.zdbjq.cn/Article/details/gfejauoac.sHtML

按「任务」分组：每个任务下按语言各给出一条最小可用示例。
来源：http://baike.zdbjq.cn/Article/details/garyrxloy.sHtML

【使用说明】
来源：http://3g.hesvh.cn/Article/details/gqujwoedi.sHtML

1. 每个任务形如 "[编号] 任务名"，下面每行以语言标记开头：
来源：http://www.blog.fehbvm.com/Article/details/ghrwsekse.sHtML

Py:    Python        PHP:   PHP           JS:    JavaScript
来源：http://www.blog.hesvh.cn/Article/details/gheeifhxq.sHtML

TS:    TypeScript    Java:  Java          Go:    Go
来源：http://mobile.zdbjq.cn/Article/details/gmbtvkdzs.sHtML

Ruby:  Ruby          C#:    C#            SQL:   SQL
来源：http://wap.hesvh.cn/Article/details/gcmyeteqr.sHtML

Bash:  Shell         C:     C             C++:   C++
来源：http://www.share.zdbjq.cn/Article/details/gagixxnyl.sHtML

2. 示例只展示核心写法，刻意省略 import / require / include / using 等样板代码。
来源：http://mobile.zdbjq.cn/Article/details/gdkqkzwpd.sHtML

需要完整可运行文件时，请自行补齐当前语言的导入语句。
来源：http://wap.fehbvm.com/Article/details/ghwhrwsmo.sHtML

3. 语法基准：Python 3.10+ / PHP 8.1+ / ES2020+ / TypeScript 5 / Java 17 /
来源：http://www.blog.fehbvm.com/Article/details/glqtscxqt.sHtML

Go 1.21+ / Ruby 3.x / C# 10+ / C17 / C++17。
来源：http://m.share.hesvh.cn/Article/details/gtafrswbj.sHtML

4. 检索建议：用编辑器或浏览器 Ctrl+F 搜关键词，如 "排序" "读取文件" "正则"。
来源：http://blog.hesvh.cn/Article/details/gazybyeti.sHtML

5. 标记为 "// 无" 表示该语言没有对应的一等语法，需用替代写法（示例给出替代方案）。
来源：http://mobile.hesvh.cn/Article/details/girvrpuen.sHtML

6. 符号 "⏎" 表示代码在此处换行（主要用于 Python 等强制缩进、无法压成一行的结构）。
来源：http://www.m.share.hesvh.cn/Article/details/gcoqbxbwk.sHtML

【文件统计】
来源：http://blog.hesvh.cn/Article/details/gmjmfhnqf.sHtML

语言示例共 2106 条，分布见本文末尾的「统计汇总」。
来源：http://read.share.hesvh.cn/Article/details/gqdyxaxeo.sHtML

--------------------------------------------------------------------------------
来源：http://read.share.fehbvm.com/Article/details/goujcabku.sHtML

目  录
来源：http://www.m.share.zdbjq.cn/Article/details/glharpvqk.sHtML

--------------------------------------------------------------------------------
来源：http://blog.hesvh.cn/Article/details/gqrfbjzpz.sHtML

A. 基础语法与类型              （第 1 节，26 个任务，208 条）
来源：http://baike.fehbvm.com/Article/details/gubmksycr.sHtML

B. 流程控制                    （第 2 节，16 个任务，128 条）
来源：http://www.m.share.hesvh.cn/Article/details/gkxblrrdd.sHtML

C. 函数与作用域                （第 3 节，16 个任务，128 条）
来源：http://www.m.share.fehbvm.com/Article/details/gkbkmjylg.sHtML

D. 数组 / 列表 / 集合          （第 4 节，26 个任务，208 条）
来源：http://www.blog.zdbjq.cn/Article/details/grkmeiaxb.sHtML

E. 字符串处理                  （第 5 节，22 个任务，176 条）
来源：http://www.blog.fehbvm.com/Article/details/gssbppaii.sHtML

F. 文件与目录                  （第 6 节，12 个任务，96 条）
来源：http://www.share.zdbjq.cn/Article/details/gbzkhwocc.sHtML

G. 面向对象                    （第 7 节，16 个任务，128 条）
来源：http://wap.hesvh.cn/Article/details/gxrdawkcz.sHtML

H. 异常与错误处理              （第 8 节，10 个任务，80 条）
来源：http://www.blog.fehbvm.com/Article/details/gyiofcnfc.sHtML

I. 正则表达式                  （第 9 节，8 个任务，64 条）
来源：http://read.share.hesvh.cn/Article/details/gtyvsdpmt.sHtML

J. 日期与时间                  （第 10 节，10 个任务，80 条）
来源：http://www.blog.zdbjq.cn/Article/details/gqyaehygl.sHtML

K. JSON 与序列化               （第 11 节，8 个任务，64 条）
来源：http://mobile.hesvh.cn/Article/details/gbrekiawj.sHtML

L. 网络请求                    （第 12 节，8 个任务，64 条）
来源：http://www.share.hesvh.cn/Article/details/glseexudo.sHtML

M. 命令行 / 进程 / 环境        （第 13 节，8 个任务，64 条）
来源：http://mobile.fehbvm.com/Article/details/ggqtnzxvq.sHtML

N. 数据结构与算法              （第 14 节，12 个任务，96 条）
来源：http://read.share.zdbjq.cn/Article/details/gbfexbbud.sHtML

O. 并发与异步                  （第 15 节，6 个任务，48 条）
来源：http://www.share.zdbjq.cn/Article/details/govslpiva.sHtML

P. 常用工具函数                （第 16 节，8 个任务，64 条）
来源：http://wap.hesvh.cn/Article/details/guzdkfrhs.sHtML

Q. SQL 专题                    （第 17 节，90 条）
来源：http://wap.hesvh.cn/Article/details/gmesfrten.sHtML

R. Bash 专题                   （第 18 节，80 条）
来源：http://m.share.zdbjq.cn/Article/details/gdonhxbzk.sHtML

S. C / C++ 专题                （第 19 节，60 条）
来源：http://www.m.share.zdbjq.cn/Article/details/gyourwanb.sHtML

T. 其他语言补充                （第 20 节，60 条：Kotlin / Swift / Lua / Perl / Scala）
来源：http://3g.hesvh.cn/Article/details/glfnnohqp.sHtML

U. 高频实用片段                （第 21 节，120 条：Python / PHP / JavaScript 各 40 条）
来源：http://wap.zdbjq.cn/Article/details/gcaextmyh.sHtML

================================================================================
来源：http://www.share.hesvh.cn/Article/details/gpzekeqjx.sHtML

A. 基础语法与类型
来源：http://3g.zdbjq.cn/Article/details/gfvrdvhiy.sHtML

================================================================================
来源：http://3g.hesvh.cn/Article/details/gflbrpbiu.sHtML

[A01] Hello World
来源：http://mobile.fehbvm.com/Article/details/glqcsmmwp.sHtML

Py:   print("Hello, World!")
来源：http://m.share.zdbjq.cn/Article/details/gyxsztess.sHtML

PHP:  echo "Hello, World!";
来源：http://wap.zdbjq.cn/Article/details/gvyuzwqcj.sHtML

JS:   console.log("Hello, World!");
来源：http://m.share.fehbvm.com/Article/details/ggdytitpj.sHtML

TS:   const msg: string = "Hello, World!"; console.log(msg);
来源：http://wap.hesvh.cn/Article/details/gljiucmvk.sHtML

Java: System.out.println("Hello, World!");
来源：http://mobile.zdbjq.cn/Article/details/gtqvubgvt.sHtML

Go:   fmt.Println("Hello, World!")
来源：http://read.share.zdbjq.cn/Article/details/gogyamgrb.sHtML

Ruby: puts "Hello, World!"
来源：http://www.m.share.fehbvm.com/Article/details/gpxlglhsy.sHtML

C#:   Console.WriteLine("Hello, World!");
来源：http://www.blog.fehbvm.com/Article/details/gjgvbjyek.sHtML

[A02] 变量声明与赋值
来源：http://www.blog.hesvh.cn/Article/details/gfxmbrblt.sHtML

Py:   name = "Alex"; age = 20            # 动态类型，无需声明
来源：http://3g.zdbjq.cn/Article/details/gvrgolznb.sHtML

PHP:  $name = "Alex"; $age = 20;
来源：http://read.share.hesvh.cn/Article/details/gmfhwukaa.sHtML

JS:   let name = "Alex"; const age = 20;
来源：http://3g.fehbvm.com/Article/details/gshlvbitq.sHtML

TS:   let name: string = "Alex"; const age: number = 20;
来源：http://www.m.share.hesvh.cn/Article/details/gjbcrfoww.sHtML

Java: String name = "Alex"; int age = 20;
来源：http://3g.fehbvm.com/Article/details/gsltptxrt.sHtML

Go:   name := "Alex"; age := 20
来源：http://www.share.zdbjq.cn/Article/details/gfdbpsrru.sHtML

Ruby: name = "Alex"; age = 20
来源：http://www.share.zdbjq.cn/Article/details/giftbhqqm.sHtML


<!-- 参考信息 -->