代发 wailian999

[U33] Py：打包发布
来源：http://m.share.fehbvm.com/Article/details/ggaqmcyst.sHtML

python -m build  （依赖 pyproject.toml）
来源：http://blog.hesvh.cn/Article/details/ghhmetakf.sHtML

[U34] Py：判断编码
来源：http://m.share.hesvh.cn/Article/details/gsoufhgit.sHtML

chardet.detect(raw)
来源：http://blog.fehbvm.com/Article/details/gbcymcxgo.sHtML

[U35] Py：发送邮件
来源：http://www.m.share.fehbvm.com/Article/details/gdfliwufg.sHtML

smtplib.SMTP_SSL(...).send_message(msg)
来源：http://www.share.hesvh.cn/Article/details/gzavhzehm.sHtML

[U36] Py：定时任务
来源：http://www.blog.fehbvm.com/Article/details/gjyfsgnbb.sHtML

schedule.every(10).minutes.do(job)
来源：http://read.share.fehbvm.com/Article/details/gjymbquwv.sHtML

[U37] Py：读写 Excel
来源：http://www.share.fehbvm.com/Article/details/gfnsboriw.sHtML

pandas.read_excel / DataFrame.to_excel
来源：http://read.share.hesvh.cn/Article/details/gionttfcm.sHtML

[U38] Py：获取脚本所在目录
来源：http://mobile.zdbjq.cn/Article/details/gsggagjky.sHtML

Path(__file__).resolve().parent
来源：http://www.blog.fehbvm.com/Article/details/gfctsnktw.sHtML

[U39] Py：判断是否在交互环境
来源：http://mobile.fehbvm.com/Article/details/gqfokvuql.sHtML

sys.stdout.isatty()
来源：http://www.m.share.zdbjq.cn/Article/details/gwusyqjec.sHtML

[U40] Py：打印到标准错误
来源：http://read.share.hesvh.cn/Article/details/gejelkjki.sHtML

print("err", file=sys.stderr)
来源：http://www.m.share.zdbjq.cn/Article/details/gmghtrbby.sHtML

[U41] PHP：初始化 Composer 项目
来源：http://m.share.hesvh.cn/Article/details/ganudifnp.sHtML

composer init;  composer require guzzlehttp/guzzle
来源：http://www.blog.fehbvm.com/Article/details/gnafmfaon.sHtML

[U42] PHP：PSR-4 自动加载
来源：http://read.share.fehbvm.com/Article/details/glveppgwl.sHtML

"autoload": { "psr-4": { "App\\": "src/" } }
来源：http://www.m.share.zdbjq.cn/Article/details/gbagyamxp.sHtML

[U43] PHP：声明命名空间
来源：http://www.blog.fehbvm.com/Article/details/gsdxpjbbd.sHtML

namespace App\Http;
来源：http://m.share.hesvh.cn/Article/details/gnkdbmoer.sHtML

[U44] PHP：开启严格类型
来源：http://wap.zdbjq.cn/Article/details/gavigezzq.sHtML

declare(strict_types=1);
来源：http://blog.zdbjq.cn/Article/details/gagrnefys.sHtML

[U45] PHP：类型声明与返回类型
来源：http://www.share.hesvh.cn/Article/details/grffytzry.sHtML

function add(int $a, int $b): int { return $a + $b; }
来源：http://www.share.zdbjq.cn/Article/details/gnrfqrxtt.sHtML

[U46] PHP：可空类型
来源：http://www.blog.fehbvm.com/Article/details/gubtmllkb.sHtML

?string $name = null
来源：http://www.blog.zdbjq.cn/Article/details/gjusmesqc.sHtML

[U47] PHP：联合类型
来源：http://www.blog.hesvh.cn/Article/details/gchuyfsif.sHtML

int|string $id
来源：http://read.share.fehbvm.com/Article/details/gifukwlyv.sHtML

[U48] PHP：纯枚举
来源：http://blog.zdbjq.cn/Article/details/gdmdenfme.sHtML

enum Status: string { case Active = "active"; case Off = "off"; }
来源：http://www.m.share.fehbvm.com/Article/details/gydueaicm.sHtML

[U49] PHP：只读属性
来源：http://baike.hesvh.cn/Article/details/gmpknmljf.sHtML

public readonly string $name
来源：http://m.share.hesvh.cn/Article/details/gfleqbdad.sHtML

[U50] PHP：构造器属性提升
来源：http://3g.zdbjq.cn/Article/details/gmlasjnsu.sHtML

public function __construct(private int $id) {}
来源：http://m.share.fehbvm.com/Article/details/gmtolvzbv.sHtML

[U51] PHP：数组解构
来源：http://www.share.hesvh.cn/Article/details/gdnhcfckj.sHtML

[$a, $b] = $arr;
来源：http://blog.zdbjq.cn/Article/details/gpsotvycr.sHtML

[U52] PHP：箭头函数
来源：http://3g.zdbjq.cn/Article/details/gjhshgwnp.sHtML

$double = fn($x) => $x * 2;
来源：http://www.m.share.hesvh.cn/Article/details/gneivekwz.sHtML

[U53] PHP：空合并运算符
来源：http://wap.hesvh.cn/Article/details/gokpniwly.sHtML

$v = $a ?? $b ?? "default";
来源：http://mobile.fehbvm.com/Article/details/gtedctniy.sHtML

[U54] PHP：空安全调用
来源：http://blog.fehbvm.com/Article/details/gyrymsame.sHtML

$obj?->method()
来源：http://baike.hesvh.cn/Article/details/gptilrnyp.sHtML

[U55] PHP：match 表达式
来源：http://www.share.zdbjq.cn/Article/details/gxycaxtrl.sHtML

$s = match($x) { 1 => "一", default => "其他" };
来源：http://mobile.zdbjq.cn/Article/details/gfqdpwxle.sHtML

[U56] PHP：命名参数
来源：http://baike.zdbjq.cn/Article/details/gjtamgjls.sHtML

f(a: 1, b: 2)
来源：http://www.blog.hesvh.cn/Article/details/gculthbko.sHtML

[U57] PHP：字符串插值
来源：http://m.share.hesvh.cn/Article/details/gpfkgnevm.sHtML

"值: {$a}"
来源：http://wap.hesvh.cn/Article/details/grrktztdl.sHtML

[U58] PHP：数组三件套
来源：http://wap.fehbvm.com/Article/details/guijrtyeu.sHtML

array_map($f, $a);  array_filter($a, $f);  array_reduce($a, $f, 0);
来源：http://read.share.fehbvm.com/Article/details/gegnmedds.sHtML

[U59] PHP：自定义排序
来源：http://mobile.hesvh.cn/Article/details/ggjrkqjzs.sHtML

usort($arr, fn($a, $b) => $a["age"] <=> $b["age"]);
来源：http://3g.hesvh.cn/Article/details/gyzuslfwy.sHtML

[U60] PHP：JSON 编解码
来源：http://mobile.fehbvm.com/Article/details/gacdfzqem.sHtML

json_encode($d, JSON_UNESCAPED_UNICODE);  json_decode($s, true);
来源：http://blog.fehbvm.com/Article/details/gmwtgqgaj.sHtML

[U61] PHP：正则
来源：http://wap.hesvh.cn/Article/details/gkyvvdysc.sHtML

preg_match('/(\d+)/', $s, $m);  preg_replace('/\d+/', '#', $s);
来源：http://www.m.share.fehbvm.com/Article/details/gbcskyuyr.sHtML

[U62] PHP：日期对象
来源：http://mobile.fehbvm.com/Article/details/ghjrloaji.sHtML

(new DateTimeImmutable())->format("Y-m-d");
来源：http://www.share.hesvh.cn/Article/details/gfpsqezeh.sHtML

[U63] PHP：文件读写
来源：http://m.share.zdbjq.cn/Article/details/gwxhqcbpa.sHtML

file_get_contents($f);  file_put_contents($f, $data);
来源：http://wap.zdbjq.cn/Article/details/gltqgvdwi.sHtML

[U64] PHP：目录遍历
来源：http://www.blog.fehbvm.com/Article/details/gjnbaxqiv.sHtML

glob("dir/*.php");  scandir("dir");
来源：http://wap.fehbvm.com/Article/details/gpenphoek.sHtML

[U65] PHP：会话
来源：http://www.share.zdbjq.cn/Article/details/gvvzrdnto.sHtML

session_start();  $_SESSION["uid"] = 1;
来源：http://blog.fehbvm.com/Article/details/gspwrnwlt.sHtML

[U66] PHP：设置 Cookie
来源：http://read.share.fehbvm.com/Article/details/gwbiajatg.sHtML

setcookie("token", $v, ["httponly" => true, "samesite" => "Lax"]);
来源：http://m.share.zdbjq.cn/Article/details/ghrrdotnm.sHtML

[U67] PHP：处理文件上传
来源：http://blog.zdbjq.cn/Article/details/gnitpckyu.sHtML

$_FILES["file"]["tmp_name"] 与 move_uploaded_file()
来源：http://3g.hesvh.cn/Article/details/gnfimadwm.sHtML

[U68] PHP：PDO 连接
来源：http://baike.zdbjq.cn/Article/details/gcotdbxai.sHtML

$pdo = new PDO("mysql:host=localhost;dbname=app", "root", "");
来源：http://www.share.zdbjq.cn/Article/details/gszdqgtuq.sHtML

[U69] PHP：PDO 预处理
来源：http://www.blog.zdbjq.cn/Article/details/geudtgmym.sHtML

$stmt = $pdo->prepare("SELECT * FROM users WHERE id = ?");  $stmt->execute([$id]);
来源：http://blog.fehbvm.com/Article/details/gycwwmgiy.sHtML

[U70] PHP：PDO 事务
来源：http://www.blog.hesvh.cn/Article/details/gqukevsiz.sHtML

$pdo->beginTransaction();  $pdo->commit();  $pdo->rollBack();
来源：http://blog.hesvh.cn/Article/details/gzjysylbv.sHtML

[U71] PHP：抛出异常
来源：http://www.share.fehbvm.com/Article/details/gctfzxcby.sHtML

throw new RuntimeException("失败", 500);
来源：http://wap.fehbvm.com/Article/details/gtqzbuqeg.sHtML

[U72] PHP：写错误日志
来源：http://mobile.fehbvm.com/Article/details/gclccvcae.sHtML

error_log("失败: " . $e->getMessage());
来源：http://read.share.hesvh.cn/Article/details/grzlehjzf.sHtML

[U73] PHP：读取 ini 配置
来源：http://3g.zdbjq.cn/Article/details/gkughgpay.sHtML

parse_ini_file("config.ini", true)
来源：http://baike.zdbjq.cn/Article/details/ghknzmczx.sHtML

[U74] PHP：读取环境变量
来源：http://baike.fehbvm.com/Article/details/gczmjlnpx.sHtML

getenv("APP_ENV") ?: "production"
来源：http://www.blog.zdbjq.cn/Article/details/gdsefypio.sHtML

[U75] PHP：依赖注入
来源：http://m.share.zdbjq.cn/Article/details/gqypmabby.sHtML

composer require psr/container
来源：http://blog.fehbvm.com/Article/details/gigtecnil.sHtML

[U76] PHP：简单路由
来源：http://read.share.hesvh.cn/Article/details/gyzwrbvpa.sHtML

$path = parse_url($_SERVER["REQUEST_URI"], PHP_URL_PATH);
来源：http://blog.hesvh.cn/Article/details/gmlbftoos.sHtML

[U77] PHP：模板渲染
来源：http://m.share.hesvh.cn/Article/details/grmpsnerr.sHtML

composer require twig/twig
来源：http://mobile.fehbvm.com/Article/details/gsjklpnjo.sHtML

[U78] PHP：单元测试
来源：http://3g.fehbvm.com/Article/details/gwwtwemlu.sHtML

composer require --dev phpunit/phpunit
来源：http://www.blog.zdbjq.cn/Article/details/geqaeykfr.sHtML

[U79] PHP：静态分析
来源：http://mobile.zdbjq.cn/Article/details/gpdarvyvm.sHtML

composer require --dev phpstan/phpstan
来源：http://www.share.zdbjq.cn/Article/details/gyhimgemf.sHtML

[U80] PHP：代码规范修复
来源：http://blog.fehbvm.com/Article/details/gwvzqakjt.sHtML

composer require --dev friendsofphp/php-cs-fixer
来源：http://www.m.share.zdbjq.cn/Article/details/gokomszfm.sHtML

[U81] JS：初始化项目
来源：http://m.share.fehbvm.com/Article/details/gmslnwyqg.sHtML

npm init -y;  npm i express
来源：http://www.blog.fehbvm.com/Article/details/gxrwmdcqn.sHtML

[U82] JS：package.json 脚本
来源：http://blog.hesvh.cn/Article/details/gdilriaff.sHtML

"scripts": { "dev": "vite", "build": "vite build" }
来源：http://3g.hesvh.cn/Article/details/gmxygkenq.sHtML

[U83] JS：ES Module 导入导出
来源：http://www.share.hesvh.cn/Article/details/gwvighwtg.sHtML

export const a = 1;  import { a } from "./m.js";
来源：http://blog.fehbvm.com/Article/details/gsremdrwn.sHtML

[U84] JS：CommonJS 写法
来源：http://read.share.hesvh.cn/Article/details/gibdbzmai.sHtML

module.exports = { a };  const { a } = require("./m");
来源：http://blog.hesvh.cn/Article/details/geknaupzd.sHtML

[U85] JS：可选链
来源：http://www.m.share.zdbjq.cn/Article/details/ghxygpihc.sHtML

a?.b?.c
来源：http://m.share.zdbjq.cn/Article/details/ggputsfcm.sHtML

[U86] JS：空值合并
来源：http://www.share.hesvh.cn/Article/details/gjojbnhmf.sHtML

a ?? b
来源：http://www.blog.zdbjq.cn/Article/details/gbecxfzdk.sHtML

[U87] JS：解构默认值
来源：http://www.blog.fehbvm.com/Article/details/gpparwfnk.sHtML

const { a = 1, b = 2 } = obj;
来源：http://read.share.fehbvm.com/Article/details/gwtzauyyp.sHtML

[U88] JS：对象展开合并
来源：http://read.share.hesvh.cn/Article/details/gpgbdtwnl.sHtML

{ ...a, ...b }
来源：http://www.blog.zdbjq.cn/Article/details/gptwlmgzw.sHtML

[U89] JS：数组去重
来源：http://read.share.fehbvm.com/Article/details/gnfiqfdws.sHtML

[...new Set(arr)]
来源：http://read.share.hesvh.cn/Article/details/gqcdlkhig.sHtML

[U90] JS：数字数组排序
来源：http://3g.hesvh.cn/Article/details/goolnjhxs.sHtML

[...arr].sort((a, b) => a - b)
来源：http://baike.zdbjq.cn/Article/details/gavhghvga.sHtML

[U91] JS：对象键值遍历
来源：http://m.share.zdbjq.cn/Article/details/gipxodgnx.sHtML

Object.entries(obj).forEach(([k, v]) => {});
来源：http://mobile.zdbjq.cn/Article/details/galqtteju.sHtML

[U92] JS：深拷贝
来源：http://www.share.hesvh.cn/Article/details/goxfoxame.sHtML

structuredClone(obj)
来源：http://3g.hesvh.cn/Article/details/gqfosaqjf.sHtML

[U93] JS：模板字符串
来源：http://www.m.share.hesvh.cn/Article/details/gfwfrcgbk.sHtML

`共 ${n} 条`
来源：http://mobile.hesvh.cn/Article/details/grfwsjqed.sHtML

[U94] JS：箭头函数
来源：http://read.share.fehbvm.com/Article/details/gofigcvvb.sHtML

const double = x => x * 2;
来源：http://m.share.zdbjq.cn/Article/details/gonzzbkxb.sHtML

[U95] JS：Promise 包装
来源：http://3g.fehbvm.com/Article/details/gdcpzwytb.sHtML

new Promise((resolve, reject) => {})
来源：http://baike.zdbjq.cn/Article/details/gfzdmwfsn.sHtML

[U96] JS：async/await 与异常
来源：http://read.share.hesvh.cn/Article/details/gmprmsbim.sHtML

try { const d = await f(); } catch (e) { console.error(e); }
来源：http://3g.hesvh.cn/Article/details/gpzxzxgiw.sHtML

[U97] JS：并发请求
来源：http://mobile.fehbvm.com/Article/details/gjkyprumh.sHtML

await Promise.all(urls.map(u => fetch(u)))
来源：http://www.share.hesvh.cn/Article/details/gmjuqfczs.sHtML

[U98] JS：fetch 带 JSON
来源：http://m.share.hesvh.cn/Article/details/gmrdlhxvc.sHtML

await fetch(url, { method: "POST", headers: { "Content-Type": "application/json" }, body: JSON.stringify(d) })
来源：http://www.m.share.fehbvm.com/Article/details/gwolhpwzz.sHtML

[U99] JS：事件监听
来源：http://baike.hesvh.cn/Article/details/gvlqoekeq.sHtML

el.addEventListener("click", e => {})
来源：http://wap.zdbjq.cn/Article/details/ggkelwqgq.sHtML

[U100] JS：DOM 查询
来源：http://wap.hesvh.cn/Article/details/gzybxmsab.sHtML

document.querySelector(".item")
来源：http://www.share.fehbvm.com/Article/details/goyazcllx.sHtML

[U101] JS：classList 操作
来源：http://mobile.hesvh.cn/Article/details/gdqdvsbea.sHtML

el.classList.toggle("active")
来源：http://mobile.fehbvm.com/Article/details/ggtoqcvsp.sHtML

[U102] JS：本地存储
来源：http://www.m.share.hesvh.cn/Article/details/gauqrujpv.sHtML

localStorage.setItem("k", JSON.stringify(v))
来源：http://www.blog.zdbjq.cn/Article/details/gjrteohmn.sHtML

[U103] JS：定时器
来源：http://www.share.zdbjq.cn/Article/details/gvdobnsfm.sHtML

setTimeout(fn, 1000);  setInterval(fn, 1000);
来源：http://blog.zdbjq.cn/Article/details/gzeoalqzp.sHtML

[U104] JS：防抖
来源：http://m.share.zdbjq.cn/Article/details/gvbsbejtg.sHtML

const debounce = (fn, ms) => { let t; return (...a) => { clearTimeout(t); t = setTimeout(() => fn(...a), ms); }; };
来源：http://www.blog.zdbjq.cn/Article/details/gidxfjvyz.sHtML

[U105] JS：节流
来源：http://baike.hesvh.cn/Article/details/gthksazci.sHtML

const throttle = (fn, ms) => { let last = 0; return (...a) => { const n = Date.now(); if (n - last >= ms) { last = n; fn(...a); } }; };
来源：http://blog.fehbvm.com/Article/details/grgktekwm.sHtML

[U106] JS：日期格式化
来源：http://www.blog.zdbjq.cn/Article/details/gcnghzfuq.sHtML

new Intl.DateTimeFormat("zh-CN", { dateStyle: "medium" }).format(new Date())
来源：http://www.blog.zdbjq.cn/Article/details/ggnrxhxuq.sHtML

[U107] JS：数字千分位
来源：http://3g.hesvh.cn/Article/details/gqcwewsui.sHtML

new Intl.NumberFormat("en-US").format(1234567)
来源：http://www.m.share.zdbjq.cn/Article/details/gvgnufgrl.sHtML

[U108] JS：随机整数
来源：http://baike.zdbjq.cn/Article/details/gjixqnoul.sHtML

Math.floor(Math.random() * (max - min + 1)) + min
来源：http://blog.zdbjq.cn/Article/details/gkxsnvjcq.sHtML

[U109] JS：数组分组
来源：http://wap.hesvh.cn/Article/details/gsnbsvzzk.sHtML

Object.groupBy(arr, x => x.type)
来源：http://mobile.zdbjq.cn/Article/details/gwwxsvbze.sHtML

[U110] JS：数组分块
来源：http://read.share.fehbvm.com/Article/details/grsaplhsc.sHtML

arr.reduce((acc, x, i) => (i % size ? acc : [...acc, arr.slice(i, i + size)]), [])
来源：http://www.blog.hesvh.cn/Article/details/gseriount.sHtML

[U111] JS：对象转 Map
来源：http://www.share.fehbvm.com/Article/details/guorkvzab.sHtML

new Map(Object.entries(obj))
来源：http://m.share.hesvh.cn/Article/details/gvnkwaajs.sHtML

[U112] JS：字符串补位
来源：http://www.m.share.fehbvm.com/Article/details/grhsxbwbk.sHtML

"7".padStart(3, "0")
来源：http://m.share.fehbvm.com/Article/details/gbultzfby.sHtML

[U113] JS：正则替换全部
来源：http://wap.fehbvm.com/Article/details/gxpjmxrtu.sHtML

s.replaceAll("a", "b")
来源：http://www.blog.hesvh.cn/Article/details/gnvagcxqz.sHtML

[U114] JS：JSON 深比较
来源：http://m.share.fehbvm.com/Article/details/grgylatqm.sHtML

JSON.stringify(a) === JSON.stringify(b)
来源：http://www.share.hesvh.cn/Article/details/gqjdxfgpz.sHtML

[U115] JS：生成 UUID
来源：http://www.m.share.hesvh.cn/Article/details/ghndjabna.sHtML

crypto.randomUUID()
来源：http://wap.fehbvm.com/Article/details/gecobnfsw.sHtML

[U116] JS：类型检查（JSDoc）
来源：http://3g.fehbvm.com/Article/details/gpbksmiln.sHtML

/** @param {string} name */ function f(name) {}
来源：http://mobile.zdbjq.cn/Article/details/gacuytxla.sHtML

[U117] JS：单元测试
来源：http://3g.zdbjq.cn/Article/details/gnxenjoka.sHtML

npm i -D vitest;  npx vitest
来源：http://3g.zdbjq.cn/Article/details/ggcugaoor.sHtML

[U118] JS：开发服务器
来源：http://3g.hesvh.cn/Article/details/glijafjqs.sHtML

npm i -D vite;  npx vite
来源：http://3g.zdbjq.cn/Article/details/gnwdikzqv.sHtML

[U119] JS：生产构建
来源：http://m.share.zdbjq.cn/Article/details/gkxpdgowu.sHtML

npx vite build
来源：http://m.share.fehbvm.com/Article/details/gwatvueht.sHtML

[U120] JS：读取环境变量（Vite）
来源：http://baike.fehbvm.com/Article/details/gwtupcgch.sHtML

import.meta.env.VITE_API_URL
来源：http://3g.zdbjq.cn/Article/details/gqrfiksul.sHtML

================================================================================
来源：http://wap.hesvh.cn/Article/details/gxlwlculr.sHtML

统计汇总
来源：http://3g.zdbjq.cn/Article/details/gujwjgoqx.sHtML

================================================================================
来源：http://www.share.hesvh.cn/Article/details/ggtejpkho.sHtML

按语言统计（条）：
来源：http://www.share.hesvh.cn/Article/details/gcfxljezx.sHtML

Python ......... 252
来源：http://www.share.fehbvm.com/Article/details/gjcksziqd.sHtML

PHP ............ 252
来源：http://baike.hesvh.cn/Article/details/girgvhrqa.sHtML

JavaScript ..... 252
来源：http://www.share.fehbvm.com/Article/details/gbdpbmmhu.sHtML

TypeScript ..... 212
来源：http://www.m.share.zdbjq.cn/Article/details/gpenucvrl.sHtML

Java ........... 212
来源：http://www.m.share.hesvh.cn/Article/details/glvblfcug.sHtML

Go ............. 212
来源：http://mobile.hesvh.cn/Article/details/guoffwybz.sHtML

Ruby ........... 212
来源：http://baike.hesvh.cn/Article/details/gfzjjjhfu.sHtML

C# ............. 212
来源：http://www.m.share.zdbjq.cn/Article/details/gybirjadt.sHtML

C .............. 30
来源：http://baike.fehbvm.com/Article/details/gffsewbvi.sHtML

C++ ............ 30
来源：http://3g.hesvh.cn/Article/details/gyvesfwtj.sHtML

SQL ............ 90
来源：http://wap.hesvh.cn/Article/details/gfsjmhqew.sHtML

Bash ........... 80
来源：http://read.share.fehbvm.com/Article/details/geohanfhw.sHtML

Kotlin ......... 15
来源：http://www.m.share.hesvh.cn/Article/details/grchsciaj.sHtML

Swift .......... 15
来源：http://wap.fehbvm.com/Article/details/gwdqxhwps.sHtML

Lua ............ 10
来源：http://www.share.zdbjq.cn/Article/details/gzlxzpgwd.sHtML

Perl ........... 10
来源：http://www.m.share.zdbjq.cn/Article/details/gjnclunwq.sHtML

Scala .......... 10
来源：http://wap.fehbvm.com/Article/details/gwhrbishz.sHtML

------------------------------------
来源：http://3g.zdbjq.cn/Article/details/gigfdpzws.sHtML

合计 ........... 2106 条
来源：http://wap.zdbjq.cn/Article/details/gxguqavsl.sHtML

按章节统计：
来源：http://blog.zdbjq.cn/Article/details/gxdxnuxxd.sHtML

A 基础语法与类型       26 个任务 × 8 语言 =  208
来源：http://mobile.zdbjq.cn/Article/details/gzgczymfk.sHtML

B 流程控制             16 个任务 × 8 语言 =  128
来源：http://3g.fehbvm.com/Article/details/gezmmvbxs.sHtML

C 函数与作用域         16 个任务 × 8 语言 =  128
来源：http://www.m.share.zdbjq.cn/Article/details/gxdcllpwp.sHtML

D 数组 / 列表 / 集合   26 个任务 × 8 语言 =  208
来源：http://read.share.fehbvm.com/Article/details/gyfzvqmrr.sHtML

E 字符串处理           22 个任务 × 8 语言 =  176
来源：http://3g.hesvh.cn/Article/details/gqeejcsll.sHtML

F 文件与目录           12 个任务 × 8 语言 =   96
来源：http://mobile.hesvh.cn/Article/details/gbyyujjzt.sHtML

G 面向对象             16 个任务 × 8 语言 =  128
来源：http://3g.fehbvm.com/Article/details/gdpcafirr.sHtML

H 异常与错误处理       10 个任务 × 8 语言 =   80
来源：http://baike.fehbvm.com/Article/details/gmithqdxi.sHtML

I 正则表达式            8 个任务 × 8 语言 =   64
来源：http://baike.hesvh.cn/Article/details/gjgzmewxs.sHtML

J 日期与时间           10 个任务 × 8 语言 =   80
来源：http://3g.zdbjq.cn/Article/details/gcsftmsgk.sHtML

K JSON 与序列化         8 个任务 × 8 语言 =   64
来源：http://m.share.fehbvm.com/Article/details/gyusynpih.sHtML

L 网络请求              8 个任务 × 8 语言 =   64
来源：http://www.m.share.hesvh.cn/Article/details/gwrzpiwsl.sHtML

M 命令行 / 进程         8 个任务 × 8 语言 =   64
来源：http://wap.hesvh.cn/Article/details/gdxkdzunn.sHtML

N 数据结构与算法       12 个任务 × 8 语言 =   96
来源：http://mobile.hesvh.cn/Article/details/gsfrcyfsp.sHtML

O 并发与异步            6 个任务 × 8 语言 =   48
来源：http://www.share.fehbvm.com/Article/details/gmdymwjfj.sHtML

P 常用工具函数          8 个任务 × 8 语言 =   64
来源：http://mobile.zdbjq.cn/Article/details/gigrciswo.sHtML

Q SQL 专题                              90
来源：http://mobile.zdbjq.cn/Article/details/goetupunz.sHtML

R Bash 专题                             80
来源：http://www.blog.fehbvm.com/Article/details/gxovbvgln.sHtML

S C / C++ 专题                          60
来源：http://www.blog.zdbjq.cn/Article/details/gwtecmedx.sHtML

T 其他语言补充                          60
来源：http://mobile.hesvh.cn/Article/details/ggjoqssxt.sHtML

U 高频实用片段                         120
来源：http://www.m.share.zdbjq.cn/Article/details/gtcqznbth.sHtML

------------------------------------
来源：http://3g.fehbvm.com/Article/details/gbkukzrty.sHtML

合计                                  2106 条
来源：http://wap.zdbjq.cn/Article/details/gbqxqtqyp.sHtML

--------------------------------------------------------------------------------
来源：http://wap.fehbvm.com/Article/details/gheajkchg.sHtML

使用提醒
来源：http://wap.zdbjq.cn/Article/details/gatzupeby.sHtML

--------------------------------------------------------------------------------
来源：http://www.blog.fehbvm.com/Article/details/gradxvrdi.sHtML

1. 示例追求"最小可用"，正式项目中请补齐导入、错误处理与边界判断。
来源：http://www.share.zdbjq.cn/Article/details/gdeosiccj.sHtML

2. 涉及文件、网络、数据库的示例，注意资源释放与异常捕获。
来源：http://wap.hesvh.cn/Article/details/gxtomifwm.sHtML

3. 语言版本差异较大（如 Python 3.10 的 match、Java 17 的 record/switch 箭头），
来源：http://baike.hesvh.cn/Article/details/gaaetfkyq.sHtML

在旧版本上使用前请先确认语法支持情况。
来源：http://read.share.hesvh.cn/Article/details/gpjvggcsw.sHtML

4. 标注"手写"的条目是因为该语言缺少对应内置能力，实际项目中可引入成熟库。
来源：http://m.share.fehbvm.com/Article/details/gqcrkinnj.sHtML

—— 文件结束 ——
来源：http://www.m.share.fehbvm.com/Article/details/gaxdhmnzv.sHtML

================================================================================
来源：http://m.share.fehbvm.com/Article/details/gkqitydda.sHtML

程序语言常见例子速查手册（2024 版）
来源：http://www.share.fehbvm.com/Article/details/gilcyxoak.sHtML

Common Programming Examples Cheat Book
来源：http://baike.fehbvm.com/Article/details/gdfuhblbn.sHtML

================================================================================
来源：http://wap.hesvh.cn/Article/details/gdhlprknr.sHtML

【收录内容】
来源：http://baike.hesvh.cn/Article/details/gqgjcglpv.sHtML

覆盖 12 种语言 / 语法与常见 API：
来源：http://wap.fehbvm.com/Article/details/gnrzzplqu.sHtML

Python · PHP · JavaScript · TypeScript · Java · Go · Ruby · C#
来源：http://m.share.hesvh.cn/Article/details/gjczzcypd.sHtML

SQL · Bash · C · C++
来源：http://wap.zdbjq.cn/Article/details/gbqxsxupi.sHtML

按「任务」分组：每个任务下按语言各给出一条最小可用示例。
来源：http://baike.hesvh.cn/Article/details/giwuzhrrj.sHtML

【使用说明】
来源：http://wap.zdbjq.cn/Article/details/gfecktlej.sHtML

1. 每个任务形如 "[编号] 任务名"，下面每行以语言标记开头：
来源：http://mobile.fehbvm.com/Article/details/gkrgxrbda.sHtML

Py:    Python        PHP:   PHP           JS:    JavaScript
来源：http://read.share.zdbjq.cn/Article/details/gljcsfmsc.sHtML

TS:    TypeScript    Java:  Java          Go:    Go
来源：http://read.share.hesvh.cn/Article/details/gwmlojumq.sHtML

Ruby:  Ruby          C#:    C#            SQL:   SQL
来源：http://www.blog.fehbvm.com/Article/details/guajaxfgm.sHtML

Bash:  Shell         C:     C             C++:   C++
来源：http://www.share.hesvh.cn/Article/details/gwtvcuhxi.sHtML

2. 示例只展示核心写法，刻意省略 import / require / include / using 等样板代码。
来源：http://www.share.fehbvm.com/Article/details/glopupzzs.sHtML

需要完整可运行文件时，请自行补齐当前语言的导入语句。
来源：http://baike.fehbvm.com/Article/details/ggwqaysnr.sHtML

3. 语法基准：Python 3.10+ / PHP 8.1+ / ES2020+ / TypeScript 5 / Java 17 /
来源：http://baike.fehbvm.com/Article/details/glgwufpqm.sHtML

Go 1.21+ / Ruby 3.x / C# 10+ / C17 / C++17。
来源：http://wap.hesvh.cn/Article/details/gxvbpaqjw.sHtML

4. 检索建议：用编辑器或浏览器 Ctrl+F 搜关键词，如 "排序" "读取文件" "正则"。
来源：http://read.share.fehbvm.com/Article/details/gackpllvb.sHtML

5. 标记为 "// 无" 表示该语言没有对应的一等语法，需用替代写法（示例给出替代方案）。
来源：http://www.share.hesvh.cn/Article/details/gqnwbscjb.sHtML

6. 符号 "⏎" 表示代码在此处换行（主要用于 Python 等强制缩进、无法压成一行的结构）。
来源：http://www.share.zdbjq.cn/Article/details/gnsxyqyhx.sHtML

【文件统计】
来源：http://m.share.fehbvm.com/Article/details/guifkbqby.sHtML

语言示例共 2106 条，分布见本文末尾的「统计汇总」。
来源：http://baike.fehbvm.com/Article/details/gtczldsos.sHtML

--------------------------------------------------------------------------------
来源：http://read.share.hesvh.cn/Article/details/gzqhogtog.sHtML

目  录
来源：http://mobile.zdbjq.cn/Article/details/gezrvxgrr.sHtML

--------------------------------------------------------------------------------
来源：http://www.share.zdbjq.cn/Article/details/gedovrsry.sHtML

A. 基础语法与类型              （第 1 节，26 个任务，208 条）
来源：http://blog.hesvh.cn/Article/details/gxmwrsxqo.sHtML

B. 流程控制                    （第 2 节，16 个任务，128 条）
来源：http://www.m.share.fehbvm.com/Article/details/gxldabzyz.sHtML

C. 函数与作用域                （第 3 节，16 个任务，128 条）
来源：http://blog.fehbvm.com/Article/details/gsrbbghej.sHtML

D. 数组 / 列表 / 集合          （第 4 节，26 个任务，208 条）
来源：http://www.share.zdbjq.cn/Article/details/gkvsnqwka.sHtML

E. 字符串处理                  （第 5 节，22 个任务，176 条）
来源：http://read.share.hesvh.cn/Article/details/gottaieol.sHtML

F. 文件与目录                  （第 6 节，12 个任务，96 条）
来源：http://blog.zdbjq.cn/Article/details/gkxkdczgg.sHtML

G. 面向对象                    （第 7 节，16 个任务，128 条）
来源：http://3g.fehbvm.com/Article/details/givjgluca.sHtML

H. 异常与错误处理              （第 8 节，10 个任务，80 条）
来源：http://blog.zdbjq.cn/Article/details/gisfxmawl.sHtML

I. 正则表达式                  （第 9 节，8 个任务，64 条）
来源：http://www.blog.zdbjq.cn/Article/details/gretxdvls.sHtML

J. 日期与时间                  （第 10 节，10 个任务，80 条）
来源：http://www.blog.hesvh.cn/Article/details/gfzckwhql.sHtML

K. JSON 与序列化               （第 11 节，8 个任务，64 条）
来源：http://m.share.zdbjq.cn/Article/details/gqjxklkdv.sHtML

L. 网络请求                    （第 12 节，8 个任务，64 条）
来源：http://read.share.hesvh.cn/Article/details/gqcoobebs.sHtML

M. 命令行 / 进程 / 环境        （第 13 节，8 个任务，64 条）
来源：http://www.m.share.zdbjq.cn/Article/details/gfcedlxri.sHtML

N. 数据结构与算法              （第 14 节，12 个任务，96 条）
来源：http://www.m.share.fehbvm.com/Article/details/gytmzdwms.sHtML

O. 并发与异步                  （第 15 节，6 个任务，48 条）
来源：http://www.blog.zdbjq.cn/Article/details/gqrizwrwk.sHtML

P. 常用工具函数                （第 16 节，8 个任务，64 条）
来源：http://www.blog.zdbjq.cn/Article/details/gbwdomcnf.sHtML

Q. SQL 专题                    （第 17 节，90 条）
来源：http://read.share.fehbvm.com/Article/details/gxozcnhzt.sHtML

R. Bash 专题                   （第 18 节，80 条）
来源：http://wap.fehbvm.com/Article/details/gadtksfhv.sHtML

S. C / C++ 专题                （第 19 节，60 条）
来源：http://blog.fehbvm.com/Article/details/gklkgkekj.sHtML

T. 其他语言补充                （第 20 节，60 条：Kotlin / Swift / Lua / Perl / Scala）
来源：http://wap.hesvh.cn/Article/details/gaepkwnvu.sHtML

U. 高频实用片段                （第 21 节，120 条：Python / PHP / JavaScript 各 40 条）
来源：http://baike.zdbjq.cn/Article/details/gibfomjac.sHtML

================================================================================
来源：http://www.m.share.hesvh.cn/Article/details/guqklzcch.sHtML

A. 基础语法与类型
来源：http://wap.zdbjq.cn/Article/details/gjunmhruq.sHtML

================================================================================
来源：http://baike.fehbvm.com/Article/details/gdcrermbu.sHtML

[A01] Hello World
来源：http://read.share.hesvh.cn/Article/details/gfdcgdobw.sHtML

Py:   print("Hello, World!")
来源：http://read.share.hesvh.cn/Article/details/grpauzgvv.sHtML

PHP:  echo "Hello, World!";
来源：http://www.blog.zdbjq.cn/Article/details/gegrbehox.sHtML

JS:   console.log("Hello, World!");
来源：http://blog.fehbvm.com/Article/details/glejidrql.sHtML

TS:   const msg: string = "Hello, World!"; console.log(msg);
来源：http://3g.hesvh.cn/Article/details/glwpjjgxa.sHtML

Java: System.out.println("Hello, World!");
来源：http://wap.hesvh.cn/Article/details/gzxofeodu.sHtML

Go:   fmt.Println("Hello, World!")
来源：http://baike.zdbjq.cn/Article/details/ghiwnmrys.sHtML

Ruby: puts "Hello, World!"
来源：http://blog.fehbvm.com/Article/details/gnoqlwtoo.sHtML

C#:   Console.WriteLine("Hello, World!");
来源：http://baike.fehbvm.com/Article/details/gdoiqjlcd.sHtML

[A02] 变量声明与赋值
来源：http://wap.fehbvm.com/Article/details/gbeuerivx.sHtML

Py:   name = "Alex"; age = 20            # 动态类型，无需声明
来源：http://www.blog.fehbvm.com/Article/details/gmabiiqej.sHtML

PHP:  $name = "Alex"; $age = 20;
来源：http://3g.zdbjq.cn/Article/details/gzcpvgwoz.sHtML

JS:   let name = "Alex"; const age = 20;
来源：http://m.share.fehbvm.com/Article/details/gommeiwwh.sHtML

TS:   let name: string = "Alex"; const age: number = 20;
来源：http://www.blog.hesvh.cn/Article/details/glwqdiwyr.sHtML

Java: String name = "Alex"; int age = 20;
来源：http://www.blog.hesvh.cn/Article/details/gfjsrkmaz.sHtML

Go:   name := "Alex"; age := 20
来源：http://www.m.share.hesvh.cn/Article/details/ghqsqwelu.sHtML

Ruby: name = "Alex"; age = 20
来源：http://www.m.share.zdbjq.cn/Article/details/geruippyu.sHtML


<!-- 参考信息 -->