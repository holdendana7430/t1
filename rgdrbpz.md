代发 wailian999

[U29] Py：属性校验
来源：http://blog.fehbvm.com/Article/details/gkuyorpjo.sHtML

@property 与 @x.setter 配合
来源：http://wap.hesvh.cn/Article/details/gecmxdavr.sHtML

[U30] Py：数据类
来源：http://read.share.fehbvm.com/Article/details/gfeeizmuw.sHtML

@dataclass(slots=True)
来源：http://www.blog.hesvh.cn/Article/details/gdspwsdqx.sHtML

[U31] Py：单测
来源：http://www.share.fehbvm.com/Article/details/ggwrafllc.sHtML

python -m pytest -q
来源：http://baike.fehbvm.com/Article/details/gsmisrjvf.sHtML

[U32] Py：代码格式化
来源：http://www.m.share.hesvh.cn/Article/details/goeptbykp.sHtML

ruff format . && ruff check --fix .
来源：http://read.share.hesvh.cn/Article/details/gaeilnzgg.sHtML

[U33] Py：打包发布
来源：http://3g.hesvh.cn/Article/details/gscrgkmjq.sHtML

python -m build  （依赖 pyproject.toml）
来源：http://mobile.fehbvm.com/Article/details/gkibhapkb.sHtML

[U34] Py：判断编码
来源：http://blog.hesvh.cn/Article/details/guaiggutj.sHtML

chardet.detect(raw)
来源：http://www.share.fehbvm.com/Article/details/glmlebqaw.sHtML

[U35] Py：发送邮件
来源：http://blog.hesvh.cn/Article/details/giepsruty.sHtML

smtplib.SMTP_SSL(...).send_message(msg)
来源：http://m.share.zdbjq.cn/Article/details/gkbmosmlr.sHtML

[U36] Py：定时任务
来源：http://3g.hesvh.cn/Article/details/gnhxdyaxb.sHtML

schedule.every(10).minutes.do(job)
来源：http://mobile.fehbvm.com/Article/details/gvbevhvmr.sHtML

[U37] Py：读写 Excel
来源：http://mobile.hesvh.cn/Article/details/glrhnfwtl.sHtML

pandas.read_excel / DataFrame.to_excel
来源：http://3g.hesvh.cn/Article/details/gcjbkyzxc.sHtML

[U38] Py：获取脚本所在目录
来源：http://wap.zdbjq.cn/Article/details/gjoaogupr.sHtML

Path(__file__).resolve().parent
来源：http://blog.zdbjq.cn/Article/details/gvfgmcqdh.sHtML

[U39] Py：判断是否在交互环境
来源：http://m.share.zdbjq.cn/Article/details/gwiftyshs.sHtML

sys.stdout.isatty()
来源：http://m.share.fehbvm.com/Article/details/gtqomfaek.sHtML

[U40] Py：打印到标准错误
来源：http://www.m.share.hesvh.cn/Article/details/genjouedx.sHtML

print("err", file=sys.stderr)
来源：http://mobile.zdbjq.cn/Article/details/ghoondmat.sHtML

[U41] PHP：初始化 Composer 项目
来源：http://www.m.share.fehbvm.com/Article/details/gtgyrciwz.sHtML

composer init;  composer require guzzlehttp/guzzle
来源：http://read.share.hesvh.cn/Article/details/gewgiqnfo.sHtML

[U42] PHP：PSR-4 自动加载
来源：http://www.blog.zdbjq.cn/Article/details/gpsrwdsfo.sHtML

"autoload": { "psr-4": { "App\\": "src/" } }
来源：http://blog.fehbvm.com/Article/details/gtzltdbgp.sHtML

[U43] PHP：声明命名空间
来源：http://www.blog.fehbvm.com/Article/details/gxihimbpr.sHtML

namespace App\Http;
来源：http://baike.hesvh.cn/Article/details/gpufokgca.sHtML

[U44] PHP：开启严格类型
来源：http://m.share.fehbvm.com/Article/details/gxydpwbeq.sHtML

declare(strict_types=1);
来源：http://m.share.fehbvm.com/Article/details/gnuxjmtkf.sHtML

[U45] PHP：类型声明与返回类型
来源：http://m.share.hesvh.cn/Article/details/guhqnseat.sHtML

function add(int $a, int $b): int { return $a + $b; }
来源：http://wap.fehbvm.com/Article/details/grassncki.sHtML

[U46] PHP：可空类型
来源：http://wap.zdbjq.cn/Article/details/gjpvgzwty.sHtML

?string $name = null
来源：http://mobile.hesvh.cn/Article/details/gpjmdqghp.sHtML

[U47] PHP：联合类型
来源：http://3g.zdbjq.cn/Article/details/gqnrebayy.sHtML

int|string $id
来源：http://www.share.fehbvm.com/Article/details/gvdmmgcuz.sHtML

[U48] PHP：纯枚举
来源：http://www.m.share.zdbjq.cn/Article/details/gvxeqwvyy.sHtML

enum Status: string { case Active = "active"; case Off = "off"; }
来源：http://read.share.hesvh.cn/Article/details/ghzjjunwz.sHtML

[U49] PHP：只读属性
来源：http://mobile.hesvh.cn/Article/details/gbixqpokd.sHtML

public readonly string $name
来源：http://read.share.fehbvm.com/Article/details/gnhyzoijy.sHtML

[U50] PHP：构造器属性提升
来源：http://3g.fehbvm.com/Article/details/gkzrbubhm.sHtML

public function __construct(private int $id) {}
来源：http://www.share.hesvh.cn/Article/details/gxjqnomqf.sHtML

[U51] PHP：数组解构
来源：http://3g.fehbvm.com/Article/details/gbalzbnwf.sHtML

[$a, $b] = $arr;
来源：http://read.share.zdbjq.cn/Article/details/ghoehpcrt.sHtML

[U52] PHP：箭头函数
来源：http://mobile.zdbjq.cn/Article/details/gylwrznfi.sHtML

$double = fn($x) => $x * 2;
来源：http://3g.fehbvm.com/Article/details/gqfkvsfba.sHtML

[U53] PHP：空合并运算符
来源：http://m.share.hesvh.cn/Article/details/gpccqdtha.sHtML

$v = $a ?? $b ?? "default";
来源：http://blog.fehbvm.com/Article/details/gujjmryve.sHtML

[U54] PHP：空安全调用
来源：http://3g.fehbvm.com/Article/details/gbjkasjsc.sHtML

$obj?->method()
来源：http://www.m.share.zdbjq.cn/Article/details/goooplmkx.sHtML

[U55] PHP：match 表达式
来源：http://read.share.fehbvm.com/Article/details/gqwjkznmx.sHtML

$s = match($x) { 1 => "一", default => "其他" };
来源：http://3g.hesvh.cn/Article/details/gntspjwrf.sHtML

[U56] PHP：命名参数
来源：http://www.blog.zdbjq.cn/Article/details/gesubhgij.sHtML

f(a: 1, b: 2)
来源：http://www.blog.zdbjq.cn/Article/details/gdazyvamo.sHtML

[U57] PHP：字符串插值
来源：http://mobile.fehbvm.com/Article/details/gzhkgavwh.sHtML

"值: {$a}"
来源：http://mobile.fehbvm.com/Article/details/gxkbgbrvi.sHtML

[U58] PHP：数组三件套
来源：http://blog.zdbjq.cn/Article/details/gyvakksve.sHtML

array_map($f, $a);  array_filter($a, $f);  array_reduce($a, $f, 0);
来源：http://mobile.zdbjq.cn/Article/details/gevfhqaav.sHtML

[U59] PHP：自定义排序
来源：http://baike.fehbvm.com/Article/details/gnolwhlbd.sHtML

usort($arr, fn($a, $b) => $a["age"] <=> $b["age"]);
来源：http://www.blog.hesvh.cn/Article/details/gruexzkoh.sHtML

[U60] PHP：JSON 编解码
来源：http://read.share.fehbvm.com/Article/details/gjjwqafcx.sHtML

json_encode($d, JSON_UNESCAPED_UNICODE);  json_decode($s, true);
来源：http://www.share.hesvh.cn/Article/details/glzubfbkc.sHtML

[U61] PHP：正则
来源：http://3g.zdbjq.cn/Article/details/ghstawttt.sHtML

preg_match('/(\d+)/', $s, $m);  preg_replace('/\d+/', '#', $s);
来源：http://m.share.hesvh.cn/Article/details/gvbkmsbzm.sHtML

[U62] PHP：日期对象
来源：http://www.share.hesvh.cn/Article/details/gbkuifulm.sHtML

(new DateTimeImmutable())->format("Y-m-d");
来源：http://www.m.share.fehbvm.com/Article/details/gfohiflxo.sHtML

[U63] PHP：文件读写
来源：http://www.blog.fehbvm.com/Article/details/grlyzczox.sHtML

file_get_contents($f);  file_put_contents($f, $data);
来源：http://www.blog.zdbjq.cn/Article/details/gzascgmom.sHtML

[U64] PHP：目录遍历
来源：http://www.blog.zdbjq.cn/Article/details/gjvoervlf.sHtML

glob("dir/*.php");  scandir("dir");
来源：http://baike.hesvh.cn/Article/details/gwlajpnqm.sHtML

[U65] PHP：会话
来源：http://blog.fehbvm.com/Article/details/gxuegbbgz.sHtML

session_start();  $_SESSION["uid"] = 1;
来源：http://baike.hesvh.cn/Article/details/gvodroplf.sHtML

[U66] PHP：设置 Cookie
来源：http://www.share.fehbvm.com/Article/details/gjscwetmv.sHtML

setcookie("token", $v, ["httponly" => true, "samesite" => "Lax"]);
来源：http://www.m.share.hesvh.cn/Article/details/gzqcwlint.sHtML

[U67] PHP：处理文件上传
来源：http://baike.zdbjq.cn/Article/details/gcldoitdj.sHtML

$_FILES["file"]["tmp_name"] 与 move_uploaded_file()
来源：http://read.share.hesvh.cn/Article/details/gsqefndex.sHtML

[U68] PHP：PDO 连接
来源：http://3g.zdbjq.cn/Article/details/gqtiliqro.sHtML

$pdo = new PDO("mysql:host=localhost;dbname=app", "root", "");
来源：http://www.m.share.fehbvm.com/Article/details/guomfqera.sHtML

[U69] PHP：PDO 预处理
来源：http://baike.zdbjq.cn/Article/details/gflipraeo.sHtML

$stmt = $pdo->prepare("SELECT * FROM users WHERE id = ?");  $stmt->execute([$id]);
来源：http://m.share.fehbvm.com/Article/details/galcgoyoo.sHtML

[U70] PHP：PDO 事务
来源：http://blog.zdbjq.cn/Article/details/geohlcjjd.sHtML

$pdo->beginTransaction();  $pdo->commit();  $pdo->rollBack();
来源：http://www.m.share.zdbjq.cn/Article/details/gbnphdttt.sHtML

[U71] PHP：抛出异常
来源：http://baike.hesvh.cn/Article/details/ghxqdnqkt.sHtML

throw new RuntimeException("失败", 500);
来源：http://3g.hesvh.cn/Article/details/gdrygegkg.sHtML

[U72] PHP：写错误日志
来源：http://blog.fehbvm.com/Article/details/gtlqvijqj.sHtML

error_log("失败: " . $e->getMessage());
来源：http://baike.fehbvm.com/Article/details/gxyoqvrxb.sHtML

[U73] PHP：读取 ini 配置
来源：http://wap.zdbjq.cn/Article/details/gbrlsaxve.sHtML

parse_ini_file("config.ini", true)
来源：http://blog.fehbvm.com/Article/details/guyenthzv.sHtML

[U74] PHP：读取环境变量
来源：http://wap.zdbjq.cn/Article/details/gnyvcwwyc.sHtML

getenv("APP_ENV") ?: "production"
来源：http://baike.fehbvm.com/Article/details/gtnbcumrs.sHtML

[U75] PHP：依赖注入
来源：http://www.m.share.hesvh.cn/Article/details/gvgqyjzru.sHtML

composer require psr/container
来源：http://m.share.zdbjq.cn/Article/details/gurpdravs.sHtML

[U76] PHP：简单路由
来源：http://read.share.fehbvm.com/Article/details/gpntwnatm.sHtML

$path = parse_url($_SERVER["REQUEST_URI"], PHP_URL_PATH);
来源：http://mobile.hesvh.cn/Article/details/gcvojvudi.sHtML

[U77] PHP：模板渲染
来源：http://www.m.share.fehbvm.com/Article/details/gyaowtsls.sHtML

composer require twig/twig
来源：http://read.share.zdbjq.cn/Article/details/gcgiltwzb.sHtML

[U78] PHP：单元测试
来源：http://wap.hesvh.cn/Article/details/glsuqvqsp.sHtML

composer require --dev phpunit/phpunit
来源：http://m.share.zdbjq.cn/Article/details/gdjjwnwuz.sHtML

[U79] PHP：静态分析
来源：http://blog.zdbjq.cn/Article/details/guqgwigbb.sHtML

composer require --dev phpstan/phpstan
来源：http://3g.fehbvm.com/Article/details/gobmqmdee.sHtML

[U80] PHP：代码规范修复
来源：http://m.share.fehbvm.com/Article/details/grxlfdade.sHtML

composer require --dev friendsofphp/php-cs-fixer
来源：http://3g.fehbvm.com/Article/details/gyfyyfmbx.sHtML

[U81] JS：初始化项目
来源：http://www.m.share.fehbvm.com/Article/details/gpqvtgflq.sHtML

npm init -y;  npm i express
来源：http://3g.hesvh.cn/Article/details/gcpejqdom.sHtML

[U82] JS：package.json 脚本
来源：http://m.share.zdbjq.cn/Article/details/gmbmvvsnb.sHtML

"scripts": { "dev": "vite", "build": "vite build" }
来源：http://wap.fehbvm.com/Article/details/giytgnxsv.sHtML

[U83] JS：ES Module 导入导出
来源：http://wap.zdbjq.cn/Article/details/gwztjnnxx.sHtML

export const a = 1;  import { a } from "./m.js";
来源：http://www.m.share.fehbvm.com/Article/details/geyitntxg.sHtML

[U84] JS：CommonJS 写法
来源：http://m.share.hesvh.cn/Article/details/gaampxhyq.sHtML

module.exports = { a };  const { a } = require("./m");
来源：http://m.share.fehbvm.com/Article/details/gippflbpl.sHtML

[U85] JS：可选链
来源：http://www.m.share.zdbjq.cn/Article/details/gpgrclhpb.sHtML

a?.b?.c
来源：http://www.blog.zdbjq.cn/Article/details/gafbsgyxr.sHtML

[U86] JS：空值合并
来源：http://www.share.fehbvm.com/Article/details/gjoxbyxah.sHtML

a ?? b
来源：http://3g.fehbvm.com/Article/details/gziajkbhj.sHtML

[U87] JS：解构默认值
来源：http://read.share.zdbjq.cn/Article/details/gitgijlyb.sHtML

const { a = 1, b = 2 } = obj;
来源：http://www.blog.hesvh.cn/Article/details/gumemkwoa.sHtML

[U88] JS：对象展开合并
来源：http://www.m.share.hesvh.cn/Article/details/gibllafib.sHtML

{ ...a, ...b }
来源：http://read.share.zdbjq.cn/Article/details/gpvuujngr.sHtML

[U89] JS：数组去重
来源：http://www.blog.zdbjq.cn/Article/details/geevbcpuo.sHtML

[...new Set(arr)]
来源：http://www.share.zdbjq.cn/Article/details/gppetfcfe.sHtML

[U90] JS：数字数组排序
来源：http://baike.hesvh.cn/Article/details/gboguuirs.sHtML

[...arr].sort((a, b) => a - b)
来源：http://wap.hesvh.cn/Article/details/giacyejwl.sHtML

[U91] JS：对象键值遍历
来源：http://mobile.fehbvm.com/Article/details/goimlivwt.sHtML

Object.entries(obj).forEach(([k, v]) => {});
来源：http://baike.hesvh.cn/Article/details/gbeygjrch.sHtML

[U92] JS：深拷贝
来源：http://mobile.zdbjq.cn/Article/details/ganmlcalv.sHtML

structuredClone(obj)
来源：http://www.blog.hesvh.cn/Article/details/gxepgwdhs.sHtML

[U93] JS：模板字符串
来源：http://mobile.fehbvm.com/Article/details/guggusqnz.sHtML

`共 ${n} 条`
来源：http://baike.fehbvm.com/Article/details/graorziiv.sHtML

[U94] JS：箭头函数
来源：http://mobile.fehbvm.com/Article/details/gxuwceeuw.sHtML

const double = x => x * 2;
来源：http://m.share.zdbjq.cn/Article/details/gtcjiwrsp.sHtML

[U95] JS：Promise 包装
来源：http://read.share.fehbvm.com/Article/details/gxnepuotf.sHtML

new Promise((resolve, reject) => {})
来源：http://mobile.fehbvm.com/Article/details/glekqnvtj.sHtML

[U96] JS：async/await 与异常
来源：http://wap.hesvh.cn/Article/details/gimfkzktx.sHtML

try { const d = await f(); } catch (e) { console.error(e); }
来源：http://baike.hesvh.cn/Article/details/ggmalntox.sHtML

[U97] JS：并发请求
来源：http://3g.hesvh.cn/Article/details/gnuqosbdg.sHtML

await Promise.all(urls.map(u => fetch(u)))
来源：http://mobile.zdbjq.cn/Article/details/gndxaxbyh.sHtML

[U98] JS：fetch 带 JSON
来源：http://www.m.share.hesvh.cn/Article/details/gnrdbkxxx.sHtML

await fetch(url, { method: "POST", headers: { "Content-Type": "application/json" }, body: JSON.stringify(d) })
来源：http://baike.zdbjq.cn/Article/details/gwtzshedr.sHtML

[U99] JS：事件监听
来源：http://m.share.hesvh.cn/Article/details/gtakhmcak.sHtML

el.addEventListener("click", e => {})
来源：http://baike.hesvh.cn/Article/details/gdvwdgwuw.sHtML

[U100] JS：DOM 查询
来源：http://mobile.fehbvm.com/Article/details/gyporyypi.sHtML

document.querySelector(".item")
来源：http://wap.fehbvm.com/Article/details/gmdmpnmso.sHtML

[U101] JS：classList 操作
来源：http://www.share.hesvh.cn/Article/details/gzirqogqk.sHtML

el.classList.toggle("active")
来源：http://m.share.zdbjq.cn/Article/details/gthnhltbf.sHtML

[U102] JS：本地存储
来源：http://m.share.hesvh.cn/Article/details/gdnxrwzcj.sHtML

localStorage.setItem("k", JSON.stringify(v))
来源：http://m.share.hesvh.cn/Article/details/gvyndcame.sHtML

[U103] JS：定时器
来源：http://www.blog.zdbjq.cn/Article/details/gcgrulmja.sHtML

setTimeout(fn, 1000);  setInterval(fn, 1000);
来源：http://www.blog.hesvh.cn/Article/details/gkaddibtz.sHtML

[U104] JS：防抖
来源：http://3g.hesvh.cn/Article/details/guvitkuwd.sHtML

const debounce = (fn, ms) => { let t; return (...a) => { clearTimeout(t); t = setTimeout(() => fn(...a), ms); }; };
来源：http://www.share.hesvh.cn/Article/details/gjrruiiwt.sHtML

[U105] JS：节流
来源：http://www.blog.fehbvm.com/Article/details/getpeudlj.sHtML

const throttle = (fn, ms) => { let last = 0; return (...a) => { const n = Date.now(); if (n - last >= ms) { last = n; fn(...a); } }; };
来源：http://www.share.hesvh.cn/Article/details/gxnagcavn.sHtML

[U106] JS：日期格式化
来源：http://read.share.zdbjq.cn/Article/details/gvtgurpkc.sHtML

new Intl.DateTimeFormat("zh-CN", { dateStyle: "medium" }).format(new Date())
来源：http://3g.hesvh.cn/Article/details/ghscrgpaw.sHtML

[U107] JS：数字千分位
来源：http://m.share.hesvh.cn/Article/details/ggfofeigk.sHtML

new Intl.NumberFormat("en-US").format(1234567)
来源：http://www.share.hesvh.cn/Article/details/gnobpjmvk.sHtML

[U108] JS：随机整数
来源：http://read.share.fehbvm.com/Article/details/gmthdjiyt.sHtML

Math.floor(Math.random() * (max - min + 1)) + min
来源：http://blog.zdbjq.cn/Article/details/grkxlzacq.sHtML

[U109] JS：数组分组
来源：http://www.blog.fehbvm.com/Article/details/gewvemkel.sHtML

Object.groupBy(arr, x => x.type)
来源：http://www.m.share.zdbjq.cn/Article/details/gyxosnfco.sHtML

[U110] JS：数组分块
来源：http://www.m.share.fehbvm.com/Article/details/gwqwidfic.sHtML

arr.reduce((acc, x, i) => (i % size ? acc : [...acc, arr.slice(i, i + size)]), [])
来源：http://www.m.share.hesvh.cn/Article/details/ghxlkqufq.sHtML

[U111] JS：对象转 Map
来源：http://3g.fehbvm.com/Article/details/gxwuvbfjz.sHtML

new Map(Object.entries(obj))
来源：http://wap.fehbvm.com/Article/details/gpflvftlf.sHtML

[U112] JS：字符串补位
来源：http://baike.fehbvm.com/Article/details/gcirrvodw.sHtML

"7".padStart(3, "0")
来源：http://wap.hesvh.cn/Article/details/gnfficclr.sHtML

[U113] JS：正则替换全部
来源：http://wap.fehbvm.com/Article/details/gogewikvg.sHtML

s.replaceAll("a", "b")
来源：http://3g.fehbvm.com/Article/details/gytlsvvck.sHtML

[U114] JS：JSON 深比较
来源：http://m.share.fehbvm.com/Article/details/gccskilgb.sHtML

JSON.stringify(a) === JSON.stringify(b)
来源：http://www.m.share.fehbvm.com/Article/details/gqwmpibrt.sHtML

[U115] JS：生成 UUID
来源：http://wap.fehbvm.com/Article/details/ghorkxyzk.sHtML

crypto.randomUUID()
来源：http://m.share.zdbjq.cn/Article/details/gzuqzkqhx.sHtML

[U116] JS：类型检查（JSDoc）
来源：http://baike.hesvh.cn/Article/details/gjcnexpjr.sHtML

/** @param {string} name */ function f(name) {}
来源：http://www.share.hesvh.cn/Article/details/gpgjofbtg.sHtML

[U117] JS：单元测试
来源：http://www.m.share.hesvh.cn/Article/details/gpopsxtlf.sHtML

npm i -D vitest;  npx vitest
来源：http://blog.zdbjq.cn/Article/details/gkukeyich.sHtML

[U118] JS：开发服务器
来源：http://www.m.share.hesvh.cn/Article/details/grgbovfhe.sHtML

npm i -D vite;  npx vite
来源：http://blog.zdbjq.cn/Article/details/gtdxlhgpq.sHtML

[U119] JS：生产构建
来源：http://www.blog.fehbvm.com/Article/details/gzjhktbww.sHtML

npx vite build
来源：http://read.share.hesvh.cn/Article/details/gqdriuqpq.sHtML

[U120] JS：读取环境变量（Vite）
来源：http://read.share.fehbvm.com/Article/details/gprryyezr.sHtML

import.meta.env.VITE_API_URL
来源：http://blog.zdbjq.cn/Article/details/gcxjuwmfq.sHtML

================================================================================
来源：http://www.m.share.fehbvm.com/Article/details/ggzmbnioa.sHtML

统计汇总
来源：http://www.m.share.fehbvm.com/Article/details/gezhqqavo.sHtML

================================================================================
来源：http://read.share.zdbjq.cn/Article/details/gsxuyttee.sHtML

按语言统计（条）：
来源：http://www.m.share.zdbjq.cn/Article/details/glrypjpnp.sHtML

Python ......... 252
来源：http://www.share.zdbjq.cn/Article/details/gnkbbqgmu.sHtML

PHP ............ 252
来源：http://baike.zdbjq.cn/Article/details/gfefaaasy.sHtML

JavaScript ..... 252
来源：http://www.share.zdbjq.cn/Article/details/gjafxxrlc.sHtML

TypeScript ..... 212
来源：http://www.blog.fehbvm.com/Article/details/ggpsoqnnv.sHtML

Java ........... 212
来源：http://3g.fehbvm.com/Article/details/gcmvwndvz.sHtML

Go ............. 212
来源：http://3g.fehbvm.com/Article/details/gxilhynot.sHtML

Ruby ........... 212
来源：http://www.m.share.fehbvm.com/Article/details/gqnaizybx.sHtML

C# ............. 212
来源：http://baike.hesvh.cn/Article/details/gfuvmqueo.sHtML

C .............. 30
来源：http://baike.hesvh.cn/Article/details/gterncewz.sHtML

C++ ............ 30
来源：http://wap.hesvh.cn/Article/details/gqjrifzso.sHtML

SQL ............ 90
来源：http://www.share.zdbjq.cn/Article/details/gxfpnyhct.sHtML

Bash ........... 80
来源：http://wap.hesvh.cn/Article/details/gbtpzmrev.sHtML

Kotlin ......... 15
来源：http://mobile.zdbjq.cn/Article/details/gulmjcfmy.sHtML

Swift .......... 15
来源：http://www.share.zdbjq.cn/Article/details/gnuuqzdvm.sHtML

Lua ............ 10
来源：http://www.share.zdbjq.cn/Article/details/gstbyppak.sHtML

Perl ........... 10
来源：http://read.share.hesvh.cn/Article/details/glhjojbwj.sHtML

Scala .......... 10
来源：http://baike.hesvh.cn/Article/details/gzgcayciv.sHtML

------------------------------------
来源：http://blog.zdbjq.cn/Article/details/gczxbuqvf.sHtML

合计 ........... 2106 条
来源：http://read.share.zdbjq.cn/Article/details/ggzndbqor.sHtML

按章节统计：
来源：http://baike.hesvh.cn/Article/details/ggbsepscb.sHtML

A 基础语法与类型       26 个任务 × 8 语言 =  208
来源：http://www.m.share.zdbjq.cn/Article/details/gehrpgvim.sHtML

B 流程控制             16 个任务 × 8 语言 =  128
来源：http://3g.fehbvm.com/Article/details/gsszfqivn.sHtML

C 函数与作用域         16 个任务 × 8 语言 =  128
来源：http://read.share.fehbvm.com/Article/details/gtizahwhw.sHtML

D 数组 / 列表 / 集合   26 个任务 × 8 语言 =  208
来源：http://www.share.fehbvm.com/Article/details/gpiizrzuk.sHtML

E 字符串处理           22 个任务 × 8 语言 =  176
来源：http://www.m.share.zdbjq.cn/Article/details/gwdpxgmxg.sHtML

F 文件与目录           12 个任务 × 8 语言 =   96
来源：http://m.share.fehbvm.com/Article/details/gzlqxstya.sHtML

G 面向对象             16 个任务 × 8 语言 =  128
来源：http://3g.fehbvm.com/Article/details/gsxzbuboh.sHtML

H 异常与错误处理       10 个任务 × 8 语言 =   80
来源：http://wap.fehbvm.com/Article/details/ghvgtbrxh.sHtML

I 正则表达式            8 个任务 × 8 语言 =   64
来源：http://www.share.zdbjq.cn/Article/details/gucpsaxhx.sHtML

J 日期与时间           10 个任务 × 8 语言 =   80
来源：http://mobile.hesvh.cn/Article/details/gpggdlvbt.sHtML

K JSON 与序列化         8 个任务 × 8 语言 =   64
来源：http://www.m.share.zdbjq.cn/Article/details/guhmjlymi.sHtML

L 网络请求              8 个任务 × 8 语言 =   64
来源：http://www.m.share.zdbjq.cn/Article/details/guksqsyvq.sHtML

M 命令行 / 进程         8 个任务 × 8 语言 =   64
来源：http://3g.fehbvm.com/Article/details/gwpzptnnt.sHtML

N 数据结构与算法       12 个任务 × 8 语言 =   96
来源：http://blog.fehbvm.com/Article/details/geksdljgy.sHtML

O 并发与异步            6 个任务 × 8 语言 =   48
来源：http://mobile.hesvh.cn/Article/details/gzjfyqtch.sHtML

P 常用工具函数          8 个任务 × 8 语言 =   64
来源：http://m.share.zdbjq.cn/Article/details/gtwdqqpxq.sHtML

Q SQL 专题                              90
来源：http://baike.hesvh.cn/Article/details/grpebmvzh.sHtML

R Bash 专题                             80
来源：http://www.blog.fehbvm.com/Article/details/govewkqkv.sHtML

S C / C++ 专题                          60
来源：http://wap.fehbvm.com/Article/details/gqopecdda.sHtML

T 其他语言补充                          60
来源：http://baike.fehbvm.com/Article/details/gvmruaaxz.sHtML

U 高频实用片段                         120
来源：http://3g.zdbjq.cn/Article/details/grlrggxnc.sHtML

------------------------------------
来源：http://wap.zdbjq.cn/Article/details/gqdorzlaz.sHtML

合计                                  2106 条
来源：http://wap.fehbvm.com/Article/details/gnovvthsw.sHtML

--------------------------------------------------------------------------------
来源：http://www.m.share.hesvh.cn/Article/details/gxyimxejl.sHtML

使用提醒
来源：http://read.share.fehbvm.com/Article/details/gmtxpklts.sHtML

--------------------------------------------------------------------------------
来源：http://www.share.fehbvm.com/Article/details/gofuckbdw.sHtML

1. 示例追求"最小可用"，正式项目中请补齐导入、错误处理与边界判断。
来源：http://blog.fehbvm.com/Article/details/grfubsjlz.sHtML

2. 涉及文件、网络、数据库的示例，注意资源释放与异常捕获。
来源：http://mobile.zdbjq.cn/Article/details/gsbumzwjz.sHtML

3. 语言版本差异较大（如 Python 3.10 的 match、Java 17 的 record/switch 箭头），
来源：http://blog.hesvh.cn/Article/details/grykyuwus.sHtML

在旧版本上使用前请先确认语法支持情况。
来源：http://wap.zdbjq.cn/Article/details/gdkvnbvbm.sHtML

4. 标注"手写"的条目是因为该语言缺少对应内置能力，实际项目中可引入成熟库。
来源：http://mobile.fehbvm.com/Article/details/gizapduvp.sHtML

—— 文件结束 ——
来源：http://blog.hesvh.cn/Article/details/grhxwpqhp.sHtML

================================================================================
来源：http://read.share.hesvh.cn/Article/details/gejnvzaox.sHtML

程序语言常见例子速查手册（2024 版）
来源：http://blog.zdbjq.cn/Article/details/gjuoufviq.sHtML

Common Programming Examples Cheat Book
来源：http://www.blog.fehbvm.com/Article/details/ghlgkyfqo.sHtML

================================================================================
来源：http://m.share.hesvh.cn/Article/details/grkwovrlr.sHtML

【收录内容】
来源：http://mobile.fehbvm.com/Article/details/gwhfekwzo.sHtML

覆盖 12 种语言 / 语法与常见 API：
来源：http://www.share.fehbvm.com/Article/details/gqkocimcd.sHtML

Python · PHP · JavaScript · TypeScript · Java · Go · Ruby · C#
来源：http://www.m.share.hesvh.cn/Article/details/gszasazvb.sHtML

SQL · Bash · C · C++
来源：http://mobile.fehbvm.com/Article/details/gljgwirbr.sHtML

按「任务」分组：每个任务下按语言各给出一条最小可用示例。
来源：http://read.share.zdbjq.cn/Article/details/gnmdccbfx.sHtML

【使用说明】
来源：http://read.share.hesvh.cn/Article/details/gkuvyxvqs.sHtML

1. 每个任务形如 "[编号] 任务名"，下面每行以语言标记开头：
来源：http://www.m.share.fehbvm.com/Article/details/gytzwcjmr.sHtML

Py:    Python        PHP:   PHP           JS:    JavaScript
来源：http://baike.zdbjq.cn/Article/details/gjhhmitev.sHtML

TS:    TypeScript    Java:  Java          Go:    Go
来源：http://blog.hesvh.cn/Article/details/gxnoixqkk.sHtML

Ruby:  Ruby          C#:    C#            SQL:   SQL
来源：http://3g.zdbjq.cn/Article/details/gkbaetoju.sHtML

Bash:  Shell         C:     C             C++:   C++
来源：http://www.m.share.zdbjq.cn/Article/details/gpbkehwxb.sHtML

2. 示例只展示核心写法，刻意省略 import / require / include / using 等样板代码。
来源：http://www.m.share.fehbvm.com/Article/details/gcrimpmgt.sHtML

需要完整可运行文件时，请自行补齐当前语言的导入语句。
来源：http://mobile.fehbvm.com/Article/details/gshhqtpdo.sHtML

3. 语法基准：Python 3.10+ / PHP 8.1+ / ES2020+ / TypeScript 5 / Java 17 /
来源：http://blog.fehbvm.com/Article/details/gtllilzxe.sHtML

Go 1.21+ / Ruby 3.x / C# 10+ / C17 / C++17。
来源：http://3g.zdbjq.cn/Article/details/gaeuwdutt.sHtML

4. 检索建议：用编辑器或浏览器 Ctrl+F 搜关键词，如 "排序" "读取文件" "正则"。
来源：http://baike.zdbjq.cn/Article/details/gesnxvvgh.sHtML

5. 标记为 "// 无" 表示该语言没有对应的一等语法，需用替代写法（示例给出替代方案）。
来源：http://baike.hesvh.cn/Article/details/gmvsqttdo.sHtML

6. 符号 "⏎" 表示代码在此处换行（主要用于 Python 等强制缩进、无法压成一行的结构）。
来源：http://www.share.zdbjq.cn/Article/details/ganhixirp.sHtML

【文件统计】
来源：http://3g.zdbjq.cn/Article/details/gsmmzykuy.sHtML

语言示例共 2106 条，分布见本文末尾的「统计汇总」。
来源：http://mobile.hesvh.cn/Article/details/geiuhsjtd.sHtML

--------------------------------------------------------------------------------
来源：http://mobile.hesvh.cn/Article/details/gdgrpwyxg.sHtML

目  录
来源：http://3g.zdbjq.cn/Article/details/gcewudqzq.sHtML

--------------------------------------------------------------------------------
来源：http://m.share.hesvh.cn/Article/details/gsurvndqi.sHtML

A. 基础语法与类型              （第 1 节，26 个任务，208 条）
来源：http://mobile.hesvh.cn/Article/details/gbnvwdytl.sHtML

B. 流程控制                    （第 2 节，16 个任务，128 条）
来源：http://www.blog.fehbvm.com/Article/details/gnvxiokyw.sHtML

C. 函数与作用域                （第 3 节，16 个任务，128 条）
来源：http://www.m.share.hesvh.cn/Article/details/gnaplkvqg.sHtML

D. 数组 / 列表 / 集合          （第 4 节，26 个任务，208 条）
来源：http://blog.zdbjq.cn/Article/details/gtrhpuwfw.sHtML

E. 字符串处理                  （第 5 节，22 个任务，176 条）
来源：http://baike.fehbvm.com/Article/details/gobtpravi.sHtML

F. 文件与目录                  （第 6 节，12 个任务，96 条）
来源：http://read.share.fehbvm.com/Article/details/gknlyfrgh.sHtML

G. 面向对象                    （第 7 节，16 个任务，128 条）
来源：http://mobile.fehbvm.com/Article/details/gwriwtrwn.sHtML

H. 异常与错误处理              （第 8 节，10 个任务，80 条）
来源：http://wap.zdbjq.cn/Article/details/gyqmxrvka.sHtML

I. 正则表达式                  （第 9 节，8 个任务，64 条）
来源：http://www.blog.zdbjq.cn/Article/details/gccbkmzai.sHtML

J. 日期与时间                  （第 10 节，10 个任务，80 条）
来源：http://3g.hesvh.cn/Article/details/gogwbowdi.sHtML

K. JSON 与序列化               （第 11 节，8 个任务，64 条）
来源：http://mobile.zdbjq.cn/Article/details/gstqduhpg.sHtML

L. 网络请求                    （第 12 节，8 个任务，64 条）
来源：http://m.share.zdbjq.cn/Article/details/gqjcdkieb.sHtML

M. 命令行 / 进程 / 环境        （第 13 节，8 个任务，64 条）
来源：http://read.share.fehbvm.com/Article/details/gseaexstp.sHtML

N. 数据结构与算法              （第 14 节，12 个任务，96 条）
来源：http://read.share.hesvh.cn/Article/details/gzuykaypp.sHtML

O. 并发与异步                  （第 15 节，6 个任务，48 条）
来源：http://wap.hesvh.cn/Article/details/grpiaqrtg.sHtML

P. 常用工具函数                （第 16 节，8 个任务，64 条）
来源：http://www.blog.hesvh.cn/Article/details/gibwuhacv.sHtML

Q. SQL 专题                    （第 17 节，90 条）
来源：http://baike.zdbjq.cn/Article/details/gjfmbjqxf.sHtML

R. Bash 专题                   （第 18 节，80 条）
来源：http://www.share.zdbjq.cn/Article/details/gkcqubdjv.sHtML

S. C / C++ 专题                （第 19 节，60 条）
来源：http://www.blog.fehbvm.com/Article/details/gldvaqmql.sHtML

T. 其他语言补充                （第 20 节，60 条：Kotlin / Swift / Lua / Perl / Scala）
来源：http://3g.hesvh.cn/Article/details/glagqgzdf.sHtML

U. 高频实用片段                （第 21 节，120 条：Python / PHP / JavaScript 各 40 条）
来源：http://blog.zdbjq.cn/Article/details/ggjpgzsvk.sHtML

================================================================================
来源：http://read.share.fehbvm.com/Article/details/giipynyaw.sHtML

A. 基础语法与类型
来源：http://baike.fehbvm.com/Article/details/gsedimmry.sHtML

================================================================================
来源：http://baike.zdbjq.cn/Article/details/gqyipakbz.sHtML

[A01] Hello World
来源：http://3g.zdbjq.cn/Article/details/gsbeaixzg.sHtML

Py:   print("Hello, World!")
来源：http://www.blog.zdbjq.cn/Article/details/gcbaepdmf.sHtML

PHP:  echo "Hello, World!";
来源：http://blog.hesvh.cn/Article/details/gwqefngac.sHtML

JS:   console.log("Hello, World!");
来源：http://mobile.zdbjq.cn/Article/details/gzregbvpm.sHtML

TS:   const msg: string = "Hello, World!"; console.log(msg);
来源：http://www.share.fehbvm.com/Article/details/gowgvxsym.sHtML

Java: System.out.println("Hello, World!");
来源：http://3g.zdbjq.cn/Article/details/glxxioysk.sHtML

Go:   fmt.Println("Hello, World!")
来源：http://wap.hesvh.cn/Article/details/ghrtdwdyi.sHtML

Ruby: puts "Hello, World!"
来源：http://www.m.share.hesvh.cn/Article/details/gkwfcpkor.sHtML

C#:   Console.WriteLine("Hello, World!");
来源：http://www.blog.hesvh.cn/Article/details/gbzsrpyff.sHtML


<!-- 参考信息 -->