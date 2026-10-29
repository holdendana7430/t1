代发 wailian999

[U29] Py：属性校验
来源：http://3g.hesvh.cn/Article/details/gtinpyshx.sHtML

@property 与 @x.setter 配合
来源：http://www.m.share.fehbvm.com/Article/details/goftvudyi.sHtML

[U30] Py：数据类
来源：http://www.blog.zdbjq.cn/Article/details/gzmygsnkx.sHtML

@dataclass(slots=True)
来源：http://blog.fehbvm.com/Article/details/gvawmcywk.sHtML

[U31] Py：单测
来源：http://wap.hesvh.cn/Article/details/ggzgflzte.sHtML

python -m pytest -q
来源：http://m.share.hesvh.cn/Article/details/gmbcsqfll.sHtML

[U32] Py：代码格式化
来源：http://3g.hesvh.cn/Article/details/ghrfijysd.sHtML

ruff format . && ruff check --fix .
来源：http://wap.zdbjq.cn/Article/details/gszkwzaag.sHtML

[U33] Py：打包发布
来源：http://www.m.share.fehbvm.com/Article/details/gjpdalnrh.sHtML

python -m build  （依赖 pyproject.toml）
来源：http://blog.zdbjq.cn/Article/details/gffkgcpyw.sHtML

[U34] Py：判断编码
来源：http://3g.hesvh.cn/Article/details/gukwkeigj.sHtML

chardet.detect(raw)
来源：http://blog.fehbvm.com/Article/details/ggptrtbdu.sHtML

[U35] Py：发送邮件
来源：http://www.blog.fehbvm.com/Article/details/giblmouxy.sHtML

smtplib.SMTP_SSL(...).send_message(msg)
来源：http://3g.fehbvm.com/Article/details/gxjovnzom.sHtML

[U36] Py：定时任务
来源：http://m.share.hesvh.cn/Article/details/gfgltcftn.sHtML

schedule.every(10).minutes.do(job)
来源：http://www.share.zdbjq.cn/Article/details/gwtdzgjzr.sHtML

[U37] Py：读写 Excel
来源：http://wap.hesvh.cn/Article/details/gxoiyzfrz.sHtML

pandas.read_excel / DataFrame.to_excel
来源：http://www.blog.zdbjq.cn/Article/details/gxnimrtzg.sHtML

[U38] Py：获取脚本所在目录
来源：http://baike.zdbjq.cn/Article/details/guholerfg.sHtML

Path(__file__).resolve().parent
来源：http://www.m.share.zdbjq.cn/Article/details/gcfhxcfha.sHtML

[U39] Py：判断是否在交互环境
来源：http://mobile.fehbvm.com/Article/details/gedyojjvn.sHtML

sys.stdout.isatty()
来源：http://m.share.fehbvm.com/Article/details/gvymygknq.sHtML

[U40] Py：打印到标准错误
来源：http://www.m.share.zdbjq.cn/Article/details/gegsghbrd.sHtML

print("err", file=sys.stderr)
来源：http://mobile.zdbjq.cn/Article/details/gjrbuoimv.sHtML

[U41] PHP：初始化 Composer 项目
来源：http://www.share.zdbjq.cn/Article/details/gkohedtte.sHtML

composer init;  composer require guzzlehttp/guzzle
来源：http://www.m.share.hesvh.cn/Article/details/gufiyskjk.sHtML

[U42] PHP：PSR-4 自动加载
来源：http://m.share.hesvh.cn/Article/details/gkofeeqdm.sHtML

"autoload": { "psr-4": { "App\\": "src/" } }
来源：http://m.share.hesvh.cn/Article/details/gacgltfbs.sHtML

[U43] PHP：声明命名空间
来源：http://m.share.hesvh.cn/Article/details/gdlfgndke.sHtML

namespace App\Http;
来源：http://m.share.zdbjq.cn/Article/details/gbbhumhhc.sHtML

[U44] PHP：开启严格类型
来源：http://www.blog.zdbjq.cn/Article/details/gsoyfrexy.sHtML

declare(strict_types=1);
来源：http://www.share.zdbjq.cn/Article/details/gjaskzhlw.sHtML

[U45] PHP：类型声明与返回类型
来源：http://baike.hesvh.cn/Article/details/gkzgdatwy.sHtML

function add(int $a, int $b): int { return $a + $b; }
来源：http://3g.hesvh.cn/Article/details/gfeqlttyk.sHtML

[U46] PHP：可空类型
来源：http://baike.zdbjq.cn/Article/details/gqqftmqlj.sHtML

?string $name = null
来源：http://baike.zdbjq.cn/Article/details/gajhycdug.sHtML

[U47] PHP：联合类型
来源：http://www.blog.zdbjq.cn/Article/details/gxztvlwpa.sHtML

int|string $id
来源：http://baike.fehbvm.com/Article/details/gowfjjetz.sHtML

[U48] PHP：纯枚举
来源：http://baike.zdbjq.cn/Article/details/glttrvkkj.sHtML

enum Status: string { case Active = "active"; case Off = "off"; }
来源：http://mobile.zdbjq.cn/Article/details/gbnfzbybf.sHtML

[U49] PHP：只读属性
来源：http://www.blog.hesvh.cn/Article/details/gwhsinszp.sHtML

public readonly string $name
来源：http://www.blog.hesvh.cn/Article/details/gqnshoahn.sHtML

[U50] PHP：构造器属性提升
来源：http://3g.zdbjq.cn/Article/details/ghgxwsurg.sHtML

public function __construct(private int $id) {}
来源：http://read.share.hesvh.cn/Article/details/gxojiporx.sHtML

[U51] PHP：数组解构
来源：http://wap.zdbjq.cn/Article/details/gxrllxssq.sHtML

[$a, $b] = $arr;
来源：http://blog.fehbvm.com/Article/details/gstgbceju.sHtML

[U52] PHP：箭头函数
来源：http://3g.fehbvm.com/Article/details/gqghthmhf.sHtML

$double = fn($x) => $x * 2;
来源：http://www.m.share.hesvh.cn/Article/details/gpdhojxip.sHtML

[U53] PHP：空合并运算符
来源：http://www.blog.zdbjq.cn/Article/details/gftgzmqom.sHtML

$v = $a ?? $b ?? "default";
来源：http://read.share.fehbvm.com/Article/details/geittgiwl.sHtML

[U54] PHP：空安全调用
来源：http://baike.hesvh.cn/Article/details/getcntadp.sHtML

$obj?->method()
来源：http://baike.zdbjq.cn/Article/details/gzbbbmyfw.sHtML

[U55] PHP：match 表达式
来源：http://3g.zdbjq.cn/Article/details/goixwyqhn.sHtML

$s = match($x) { 1 => "一", default => "其他" };
来源：http://wap.hesvh.cn/Article/details/gthuazesk.sHtML

[U56] PHP：命名参数
来源：http://www.blog.hesvh.cn/Article/details/gybgoljqx.sHtML

f(a: 1, b: 2)
来源：http://read.share.fehbvm.com/Article/details/gdheuoebe.sHtML

[U57] PHP：字符串插值
来源：http://www.m.share.fehbvm.com/Article/details/gngryltda.sHtML

"值: {$a}"
来源：http://www.share.zdbjq.cn/Article/details/ghadasuuv.sHtML

[U58] PHP：数组三件套
来源：http://wap.fehbvm.com/Article/details/glqpkbsfb.sHtML

array_map($f, $a);  array_filter($a, $f);  array_reduce($a, $f, 0);
来源：http://www.share.hesvh.cn/Article/details/gcqalvfie.sHtML

[U59] PHP：自定义排序
来源：http://blog.fehbvm.com/Article/details/gqmjytwsq.sHtML

usort($arr, fn($a, $b) => $a["age"] <=> $b["age"]);
来源：http://blog.hesvh.cn/Article/details/ghrsefmme.sHtML

[U60] PHP：JSON 编解码
来源：http://m.share.zdbjq.cn/Article/details/gtoemjcdd.sHtML

json_encode($d, JSON_UNESCAPED_UNICODE);  json_decode($s, true);
来源：http://www.share.hesvh.cn/Article/details/girricums.sHtML

[U61] PHP：正则
来源：http://www.share.hesvh.cn/Article/details/goppucpco.sHtML

preg_match('/(\d+)/', $s, $m);  preg_replace('/\d+/', '#', $s);
来源：http://www.m.share.fehbvm.com/Article/details/gsifurisu.sHtML

[U62] PHP：日期对象
来源：http://www.blog.fehbvm.com/Article/details/glctdfqzx.sHtML

(new DateTimeImmutable())->format("Y-m-d");
来源：http://wap.fehbvm.com/Article/details/ghlzgppwz.sHtML

[U63] PHP：文件读写
来源：http://www.m.share.zdbjq.cn/Article/details/gmwtslsci.sHtML

file_get_contents($f);  file_put_contents($f, $data);
来源：http://m.share.fehbvm.com/Article/details/gtnmaekss.sHtML

[U64] PHP：目录遍历
来源：http://www.m.share.hesvh.cn/Article/details/gmrkcrpos.sHtML

glob("dir/*.php");  scandir("dir");
来源：http://www.blog.zdbjq.cn/Article/details/gcshnwfww.sHtML

[U65] PHP：会话
来源：http://wap.zdbjq.cn/Article/details/gzmzmstjp.sHtML

session_start();  $_SESSION["uid"] = 1;
来源：http://3g.fehbvm.com/Article/details/goizmnoss.sHtML

[U66] PHP：设置 Cookie
来源：http://baike.zdbjq.cn/Article/details/ghotpoykb.sHtML

setcookie("token", $v, ["httponly" => true, "samesite" => "Lax"]);
来源：http://baike.fehbvm.com/Article/details/gykteolrm.sHtML

[U67] PHP：处理文件上传
来源：http://wap.hesvh.cn/Article/details/gxpbxtdhv.sHtML

$_FILES["file"]["tmp_name"] 与 move_uploaded_file()
来源：http://3g.fehbvm.com/Article/details/gehurxbth.sHtML

[U68] PHP：PDO 连接
来源：http://read.share.hesvh.cn/Article/details/grricaiyp.sHtML

$pdo = new PDO("mysql:host=localhost;dbname=app", "root", "");
来源：http://www.share.hesvh.cn/Article/details/ghzepgqiz.sHtML

[U69] PHP：PDO 预处理
来源：http://www.blog.fehbvm.com/Article/details/grevxjyjb.sHtML

$stmt = $pdo->prepare("SELECT * FROM users WHERE id = ?");  $stmt->execute([$id]);
来源：http://www.share.fehbvm.com/Article/details/gpkwyutbo.sHtML

[U70] PHP：PDO 事务
来源：http://www.blog.hesvh.cn/Article/details/gxqygwgcp.sHtML

$pdo->beginTransaction();  $pdo->commit();  $pdo->rollBack();
来源：http://mobile.hesvh.cn/Article/details/giooixwlf.sHtML

[U71] PHP：抛出异常
来源：http://www.blog.fehbvm.com/Article/details/gnugmqphk.sHtML

throw new RuntimeException("失败", 500);
来源：http://www.m.share.hesvh.cn/Article/details/gcsdqlkgb.sHtML

[U72] PHP：写错误日志
来源：http://blog.hesvh.cn/Article/details/ggywponbl.sHtML

error_log("失败: " . $e->getMessage());
来源：http://wap.hesvh.cn/Article/details/gkrgdqhge.sHtML

[U73] PHP：读取 ini 配置
来源：http://wap.hesvh.cn/Article/details/gyyuhrqjx.sHtML

parse_ini_file("config.ini", true)
来源：http://www.share.fehbvm.com/Article/details/gkhlzjesp.sHtML

[U74] PHP：读取环境变量
来源：http://3g.hesvh.cn/Article/details/gffwbvhbp.sHtML

getenv("APP_ENV") ?: "production"
来源：http://www.blog.hesvh.cn/Article/details/gumwkutwj.sHtML

[U75] PHP：依赖注入
来源：http://www.m.share.fehbvm.com/Article/details/gzlvwrrzh.sHtML

composer require psr/container
来源：http://www.share.fehbvm.com/Article/details/gejrqpxfi.sHtML

[U76] PHP：简单路由
来源：http://www.blog.fehbvm.com/Article/details/gcvkmqgcy.sHtML

$path = parse_url($_SERVER["REQUEST_URI"], PHP_URL_PATH);
来源：http://blog.hesvh.cn/Article/details/gfstzbhsy.sHtML

[U77] PHP：模板渲染
来源：http://www.share.zdbjq.cn/Article/details/gyaydiuqy.sHtML

composer require twig/twig
来源：http://m.share.fehbvm.com/Article/details/gebilsxgg.sHtML

[U78] PHP：单元测试
来源：http://read.share.zdbjq.cn/Article/details/gosnadvqr.sHtML

composer require --dev phpunit/phpunit
来源：http://mobile.hesvh.cn/Article/details/gxclfssbc.sHtML

[U79] PHP：静态分析
来源：http://wap.zdbjq.cn/Article/details/gzvzzprqw.sHtML

composer require --dev phpstan/phpstan
来源：http://wap.zdbjq.cn/Article/details/grxyhrogf.sHtML

[U80] PHP：代码规范修复
来源：http://m.share.fehbvm.com/Article/details/gtximsxhk.sHtML

composer require --dev friendsofphp/php-cs-fixer
来源：http://blog.zdbjq.cn/Article/details/gvuypmooz.sHtML

[U81] JS：初始化项目
来源：http://3g.fehbvm.com/Article/details/gzlhvljor.sHtML

npm init -y;  npm i express
来源：http://mobile.fehbvm.com/Article/details/gybmjuhhd.sHtML

[U82] JS：package.json 脚本
来源：http://mobile.fehbvm.com/Article/details/gqwnocdzv.sHtML

"scripts": { "dev": "vite", "build": "vite build" }
来源：http://mobile.hesvh.cn/Article/details/gwcnjvsoe.sHtML

[U83] JS：ES Module 导入导出
来源：http://blog.hesvh.cn/Article/details/gbnzthkvl.sHtML

export const a = 1;  import { a } from "./m.js";
来源：http://www.blog.hesvh.cn/Article/details/gfrtspflt.sHtML

[U84] JS：CommonJS 写法
来源：http://www.blog.hesvh.cn/Article/details/gynqrmntc.sHtML

module.exports = { a };  const { a } = require("./m");
来源：http://wap.fehbvm.com/Article/details/gvxtcsgyz.sHtML

[U85] JS：可选链
来源：http://www.blog.zdbjq.cn/Article/details/gnseaaxif.sHtML

a?.b?.c
来源：http://3g.fehbvm.com/Article/details/gixfszcob.sHtML

[U86] JS：空值合并
来源：http://www.m.share.hesvh.cn/Article/details/gwjpvguys.sHtML

a ?? b
来源：http://www.share.zdbjq.cn/Article/details/glhstgfdk.sHtML

[U87] JS：解构默认值
来源：http://3g.hesvh.cn/Article/details/gqjxkxshz.sHtML

const { a = 1, b = 2 } = obj;
来源：http://m.share.fehbvm.com/Article/details/gwmxezynf.sHtML

[U88] JS：对象展开合并
来源：http://m.share.fehbvm.com/Article/details/gajysafeq.sHtML

{ ...a, ...b }
来源：http://www.m.share.hesvh.cn/Article/details/gdqdupqnl.sHtML

[U89] JS：数组去重
来源：http://baike.hesvh.cn/Article/details/gskmxjtzk.sHtML

[...new Set(arr)]
来源：http://read.share.zdbjq.cn/Article/details/gzqsdldtp.sHtML

[U90] JS：数字数组排序
来源：http://mobile.zdbjq.cn/Article/details/gtnxksztk.sHtML

[...arr].sort((a, b) => a - b)
来源：http://baike.fehbvm.com/Article/details/gubiitxit.sHtML

[U91] JS：对象键值遍历
来源：http://mobile.hesvh.cn/Article/details/gjjuqtihe.sHtML

Object.entries(obj).forEach(([k, v]) => {});
来源：http://www.blog.fehbvm.com/Article/details/gooyvbzrp.sHtML

[U92] JS：深拷贝
来源：http://mobile.zdbjq.cn/Article/details/gmkisityc.sHtML

structuredClone(obj)
来源：http://wap.fehbvm.com/Article/details/gxfrgbduu.sHtML

[U93] JS：模板字符串
来源：http://www.m.share.fehbvm.com/Article/details/gzfndsdhr.sHtML

`共 ${n} 条`
来源：http://www.m.share.fehbvm.com/Article/details/gythxgycq.sHtML

[U94] JS：箭头函数
来源：http://blog.fehbvm.com/Article/details/gnqumasjb.sHtML

const double = x => x * 2;
来源：http://3g.fehbvm.com/Article/details/gtfdzuobd.sHtML

[U95] JS：Promise 包装
来源：http://baike.fehbvm.com/Article/details/gpathgmji.sHtML

new Promise((resolve, reject) => {})
来源：http://baike.zdbjq.cn/Article/details/gmqxbfqsr.sHtML

[U96] JS：async/await 与异常
来源：http://www.m.share.fehbvm.com/Article/details/gmpfoullu.sHtML

try { const d = await f(); } catch (e) { console.error(e); }
来源：http://read.share.hesvh.cn/Article/details/gbsfqlzmt.sHtML

[U97] JS：并发请求
来源：http://wap.fehbvm.com/Article/details/gpkgsneex.sHtML

await Promise.all(urls.map(u => fetch(u)))
来源：http://mobile.hesvh.cn/Article/details/gbezbjhxj.sHtML

[U98] JS：fetch 带 JSON
来源：http://baike.fehbvm.com/Article/details/gxnpksoiw.sHtML

await fetch(url, { method: "POST", headers: { "Content-Type": "application/json" }, body: JSON.stringify(d) })
来源：http://wap.hesvh.cn/Article/details/gvteyzwsp.sHtML

[U99] JS：事件监听
来源：http://www.m.share.hesvh.cn/Article/details/grvkvaota.sHtML

el.addEventListener("click", e => {})
来源：http://read.share.zdbjq.cn/Article/details/ggyikpboi.sHtML

[U100] JS：DOM 查询
来源：http://blog.zdbjq.cn/Article/details/gcbshrvrj.sHtML

document.querySelector(".item")
来源：http://blog.zdbjq.cn/Article/details/glwpmaplc.sHtML

[U101] JS：classList 操作
来源：http://www.blog.fehbvm.com/Article/details/gtknnikqd.sHtML

el.classList.toggle("active")
来源：http://baike.fehbvm.com/Article/details/gzsqxfgek.sHtML

[U102] JS：本地存储
来源：http://baike.fehbvm.com/Article/details/gnaguphtv.sHtML

localStorage.setItem("k", JSON.stringify(v))
来源：http://www.blog.zdbjq.cn/Article/details/ggusmyggl.sHtML

[U103] JS：定时器
来源：http://3g.hesvh.cn/Article/details/ggsgtinhn.sHtML

setTimeout(fn, 1000);  setInterval(fn, 1000);
来源：http://www.m.share.zdbjq.cn/Article/details/goriviwit.sHtML

[U104] JS：防抖
来源：http://www.blog.hesvh.cn/Article/details/giwiwduxj.sHtML

const debounce = (fn, ms) => { let t; return (...a) => { clearTimeout(t); t = setTimeout(() => fn(...a), ms); }; };
来源：http://www.m.share.zdbjq.cn/Article/details/ghukpxezf.sHtML

[U105] JS：节流
来源：http://3g.hesvh.cn/Article/details/gdpeepsgh.sHtML

const throttle = (fn, ms) => { let last = 0; return (...a) => { const n = Date.now(); if (n - last >= ms) { last = n; fn(...a); } }; };
来源：http://m.share.zdbjq.cn/Article/details/gwjyxbjpx.sHtML

[U106] JS：日期格式化
来源：http://baike.fehbvm.com/Article/details/ghzwudfku.sHtML

new Intl.DateTimeFormat("zh-CN", { dateStyle: "medium" }).format(new Date())
来源：http://baike.zdbjq.cn/Article/details/gfphvuxgk.sHtML

[U107] JS：数字千分位
来源：http://read.share.hesvh.cn/Article/details/gsmudhstt.sHtML

new Intl.NumberFormat("en-US").format(1234567)
来源：http://m.share.hesvh.cn/Article/details/gfcezypvf.sHtML

[U108] JS：随机整数
来源：http://blog.zdbjq.cn/Article/details/gczpwvafb.sHtML

Math.floor(Math.random() * (max - min + 1)) + min
来源：http://3g.zdbjq.cn/Article/details/guuthqwku.sHtML

[U109] JS：数组分组
来源：http://www.blog.fehbvm.com/Article/details/gijpfqftu.sHtML

Object.groupBy(arr, x => x.type)
来源：http://blog.fehbvm.com/Article/details/gcqikqipz.sHtML

[U110] JS：数组分块
来源：http://3g.zdbjq.cn/Article/details/gbvhcfoiq.sHtML

arr.reduce((acc, x, i) => (i % size ? acc : [...acc, arr.slice(i, i + size)]), [])
来源：http://www.blog.hesvh.cn/Article/details/groiqkhzq.sHtML

[U111] JS：对象转 Map
来源：http://baike.zdbjq.cn/Article/details/gldcmfaqj.sHtML

new Map(Object.entries(obj))
来源：http://3g.hesvh.cn/Article/details/gfkgdxohz.sHtML

[U112] JS：字符串补位
来源：http://www.share.hesvh.cn/Article/details/ginztugwq.sHtML

"7".padStart(3, "0")
来源：http://wap.zdbjq.cn/Article/details/glnokqmvh.sHtML

[U113] JS：正则替换全部
来源：http://3g.hesvh.cn/Article/details/gmfyalpcj.sHtML

s.replaceAll("a", "b")
来源：http://m.share.zdbjq.cn/Article/details/glafuweht.sHtML

[U114] JS：JSON 深比较
来源：http://blog.fehbvm.com/Article/details/ggojolakr.sHtML

JSON.stringify(a) === JSON.stringify(b)
来源：http://www.m.share.hesvh.cn/Article/details/ggtywahaw.sHtML

[U115] JS：生成 UUID
来源：http://mobile.hesvh.cn/Article/details/glfagcnag.sHtML

crypto.randomUUID()
来源：http://read.share.fehbvm.com/Article/details/gmnkfictf.sHtML

[U116] JS：类型检查（JSDoc）
来源：http://3g.zdbjq.cn/Article/details/gtxxxqcrk.sHtML

/** @param {string} name */ function f(name) {}
来源：http://www.m.share.fehbvm.com/Article/details/gjnjomupm.sHtML

[U117] JS：单元测试
来源：http://www.blog.hesvh.cn/Article/details/gjloaunou.sHtML

npm i -D vitest;  npx vitest
来源：http://www.m.share.fehbvm.com/Article/details/gdgkldghi.sHtML

[U118] JS：开发服务器
来源：http://3g.fehbvm.com/Article/details/gnjysbvvu.sHtML

npm i -D vite;  npx vite
来源：http://www.m.share.hesvh.cn/Article/details/gdwvsixby.sHtML

[U119] JS：生产构建
来源：http://3g.fehbvm.com/Article/details/giqufycjn.sHtML

npx vite build
来源：http://read.share.hesvh.cn/Article/details/gguvtvfvo.sHtML

[U120] JS：读取环境变量（Vite）
来源：http://m.share.fehbvm.com/Article/details/gfoxznvkz.sHtML

import.meta.env.VITE_API_URL
来源：http://baike.fehbvm.com/Article/details/gkdblqjbu.sHtML

================================================================================
来源：http://3g.hesvh.cn/Article/details/gorkmdlgl.sHtML

统计汇总
来源：http://www.m.share.zdbjq.cn/Article/details/gbwpvglhr.sHtML

================================================================================
来源：http://baike.fehbvm.com/Article/details/gmgbxiibn.sHtML

按语言统计（条）：
来源：http://www.m.share.zdbjq.cn/Article/details/guldteczh.sHtML

Python ......... 252
来源：http://baike.zdbjq.cn/Article/details/gqzhieubs.sHtML

PHP ............ 252
来源：http://www.share.hesvh.cn/Article/details/gfztlejot.sHtML

JavaScript ..... 252
来源：http://www.share.fehbvm.com/Article/details/ghwwokmia.sHtML

TypeScript ..... 212
来源：http://mobile.fehbvm.com/Article/details/ggtfxmink.sHtML

Java ........... 212
来源：http://blog.zdbjq.cn/Article/details/gsgmduauw.sHtML

Go ............. 212
来源：http://blog.zdbjq.cn/Article/details/gtgeapenm.sHtML

Ruby ........... 212
来源：http://m.share.zdbjq.cn/Article/details/galnsjcal.sHtML

C# ............. 212
来源：http://wap.zdbjq.cn/Article/details/guqbtnnqd.sHtML

C .............. 30
来源：http://m.share.fehbvm.com/Article/details/grszpaukr.sHtML

C++ ............ 30
来源：http://blog.zdbjq.cn/Article/details/gbirppmhx.sHtML

SQL ............ 90
来源：http://blog.hesvh.cn/Article/details/gzkvwktxj.sHtML

Bash ........... 80
来源：http://read.share.fehbvm.com/Article/details/gdmbicvcy.sHtML

Kotlin ......... 15
来源：http://mobile.zdbjq.cn/Article/details/goerbwxsj.sHtML

Swift .......... 15
来源：http://blog.fehbvm.com/Article/details/glhmzgbiv.sHtML

Lua ............ 10
来源：http://m.share.zdbjq.cn/Article/details/gtsasoksr.sHtML

Perl ........... 10
来源：http://m.share.fehbvm.com/Article/details/gvbgqhvep.sHtML

Scala .......... 10
来源：http://www.m.share.fehbvm.com/Article/details/gxxdcsmbk.sHtML

------------------------------------
来源：http://m.share.zdbjq.cn/Article/details/ggngqchqx.sHtML

合计 ........... 2106 条
来源：http://wap.fehbvm.com/Article/details/gtzijsxtb.sHtML

按章节统计：
来源：http://baike.hesvh.cn/Article/details/gyyjbcwfj.sHtML

A 基础语法与类型       26 个任务 × 8 语言 =  208
来源：http://www.share.zdbjq.cn/Article/details/gmxjsmkrn.sHtML

B 流程控制             16 个任务 × 8 语言 =  128
来源：http://www.share.fehbvm.com/Article/details/gcgqnagjl.sHtML

C 函数与作用域         16 个任务 × 8 语言 =  128
来源：http://read.share.fehbvm.com/Article/details/gabshluyg.sHtML

D 数组 / 列表 / 集合   26 个任务 × 8 语言 =  208
来源：http://mobile.hesvh.cn/Article/details/gusklxdbg.sHtML

E 字符串处理           22 个任务 × 8 语言 =  176
来源：http://www.m.share.fehbvm.com/Article/details/ggfeivmqf.sHtML

F 文件与目录           12 个任务 × 8 语言 =   96
来源：http://3g.hesvh.cn/Article/details/gfozpmqzb.sHtML

G 面向对象             16 个任务 × 8 语言 =  128
来源：http://www.blog.fehbvm.com/Article/details/gqupmtpmm.sHtML

H 异常与错误处理       10 个任务 × 8 语言 =   80
来源：http://wap.fehbvm.com/Article/details/gczenrexx.sHtML

I 正则表达式            8 个任务 × 8 语言 =   64
来源：http://blog.hesvh.cn/Article/details/giyepvatt.sHtML

J 日期与时间           10 个任务 × 8 语言 =   80
来源：http://read.share.hesvh.cn/Article/details/gaehgzacx.sHtML

K JSON 与序列化         8 个任务 × 8 语言 =   64
来源：http://www.m.share.hesvh.cn/Article/details/gxaixfcsv.sHtML

L 网络请求              8 个任务 × 8 语言 =   64
来源：http://www.blog.zdbjq.cn/Article/details/gscwozatl.sHtML

M 命令行 / 进程         8 个任务 × 8 语言 =   64
来源：http://3g.fehbvm.com/Article/details/ghucnamje.sHtML

N 数据结构与算法       12 个任务 × 8 语言 =   96
来源：http://www.m.share.hesvh.cn/Article/details/gcwlhypou.sHtML

O 并发与异步            6 个任务 × 8 语言 =   48
来源：http://m.share.fehbvm.com/Article/details/gwkurtvav.sHtML

P 常用工具函数          8 个任务 × 8 语言 =   64
来源：http://3g.hesvh.cn/Article/details/gafluohju.sHtML

Q SQL 专题                              90
来源：http://www.blog.zdbjq.cn/Article/details/gkvjclasv.sHtML

R Bash 专题                             80
来源：http://wap.fehbvm.com/Article/details/gfnmiwcsn.sHtML

S C / C++ 专题                          60
来源：http://www.share.hesvh.cn/Article/details/gbbonutcr.sHtML

T 其他语言补充                          60
来源：http://mobile.fehbvm.com/Article/details/gnhfactwn.sHtML

U 高频实用片段                         120
来源：http://m.share.hesvh.cn/Article/details/ggyvoaywi.sHtML

------------------------------------
来源：http://www.blog.fehbvm.com/Article/details/gnkngtuay.sHtML

合计                                  2106 条
来源：http://www.m.share.hesvh.cn/Article/details/gwyeftffr.sHtML

--------------------------------------------------------------------------------
来源：http://www.blog.hesvh.cn/Article/details/gbfubvsky.sHtML

使用提醒
来源：http://www.m.share.hesvh.cn/Article/details/gsfxydcxp.sHtML

--------------------------------------------------------------------------------
来源：http://www.m.share.zdbjq.cn/Article/details/geogncihi.sHtML

1. 示例追求"最小可用"，正式项目中请补齐导入、错误处理与边界判断。
来源：http://3g.fehbvm.com/Article/details/gvcdjjgvt.sHtML

2. 涉及文件、网络、数据库的示例，注意资源释放与异常捕获。
来源：http://3g.hesvh.cn/Article/details/gmvdxpcpy.sHtML

3. 语言版本差异较大（如 Python 3.10 的 match、Java 17 的 record/switch 箭头），
来源：http://wap.fehbvm.com/Article/details/gnupyygle.sHtML

在旧版本上使用前请先确认语法支持情况。
来源：http://www.share.hesvh.cn/Article/details/gqdbdtnag.sHtML

4. 标注"手写"的条目是因为该语言缺少对应内置能力，实际项目中可引入成熟库。
来源：http://blog.hesvh.cn/Article/details/gxfopipbp.sHtML

—— 文件结束 ——
来源：http://read.share.zdbjq.cn/Article/details/getxdjmbm.sHtML

================================================================================
来源：http://www.m.share.hesvh.cn/Article/details/gacbmobly.sHtML

程序语言常见例子速查手册（2024 版）
来源：http://www.share.zdbjq.cn/Article/details/gdiywxzlm.sHtML

Common Programming Examples Cheat Book
来源：http://wap.zdbjq.cn/Article/details/geyyywhxw.sHtML

================================================================================
来源：http://blog.hesvh.cn/Article/details/gqxnquscn.sHtML

【收录内容】
来源：http://www.share.fehbvm.com/Article/details/glbmywrqo.sHtML

覆盖 12 种语言 / 语法与常见 API：
来源：http://www.share.hesvh.cn/Article/details/gbierzbwc.sHtML

Python · PHP · JavaScript · TypeScript · Java · Go · Ruby · C#
来源：http://www.share.zdbjq.cn/Article/details/gewliksqm.sHtML

SQL · Bash · C · C++
来源：http://3g.zdbjq.cn/Article/details/giglavcip.sHtML

按「任务」分组：每个任务下按语言各给出一条最小可用示例。
来源：http://mobile.zdbjq.cn/Article/details/gjtaawtvo.sHtML

【使用说明】
来源：http://blog.hesvh.cn/Article/details/gcbnqkaiy.sHtML

1. 每个任务形如 "[编号] 任务名"，下面每行以语言标记开头：
来源：http://m.share.fehbvm.com/Article/details/griissrxl.sHtML

Py:    Python        PHP:   PHP           JS:    JavaScript
来源：http://www.share.hesvh.cn/Article/details/gyopgyiet.sHtML

TS:    TypeScript    Java:  Java          Go:    Go
来源：http://www.share.fehbvm.com/Article/details/gpjwlmdqz.sHtML

Ruby:  Ruby          C#:    C#            SQL:   SQL
来源：http://www.m.share.fehbvm.com/Article/details/gxvocyzgx.sHtML

Bash:  Shell         C:     C             C++:   C++
来源：http://www.m.share.fehbvm.com/Article/details/gdomfxrcs.sHtML

2. 示例只展示核心写法，刻意省略 import / require / include / using 等样板代码。
来源：http://baike.hesvh.cn/Article/details/gdqkjypzz.sHtML

需要完整可运行文件时，请自行补齐当前语言的导入语句。
来源：http://www.share.fehbvm.com/Article/details/gzbscwwpz.sHtML

3. 语法基准：Python 3.10+ / PHP 8.1+ / ES2020+ / TypeScript 5 / Java 17 /
来源：http://wap.hesvh.cn/Article/details/gbckknqqc.sHtML

Go 1.21+ / Ruby 3.x / C# 10+ / C17 / C++17。
来源：http://www.share.hesvh.cn/Article/details/gbysgkrgr.sHtML

4. 检索建议：用编辑器或浏览器 Ctrl+F 搜关键词，如 "排序" "读取文件" "正则"。
来源：http://www.share.fehbvm.com/Article/details/gaylhbpjk.sHtML

5. 标记为 "// 无" 表示该语言没有对应的一等语法，需用替代写法（示例给出替代方案）。
来源：http://3g.zdbjq.cn/Article/details/gazqfedpl.sHtML

6. 符号 "⏎" 表示代码在此处换行（主要用于 Python 等强制缩进、无法压成一行的结构）。
来源：http://blog.zdbjq.cn/Article/details/goxpntxuv.sHtML

【文件统计】
来源：http://read.share.zdbjq.cn/Article/details/gcfycwcsq.sHtML

语言示例共 2106 条，分布见本文末尾的「统计汇总」。
来源：http://m.share.hesvh.cn/Article/details/gscjvuexc.sHtML

--------------------------------------------------------------------------------
来源：http://www.share.hesvh.cn/Article/details/gboyhidcl.sHtML

目  录
来源：http://wap.hesvh.cn/Article/details/gxbsxfqmq.sHtML

--------------------------------------------------------------------------------
来源：http://mobile.hesvh.cn/Article/details/gdhznyhxy.sHtML

A. 基础语法与类型              （第 1 节，26 个任务，208 条）
来源：http://mobile.hesvh.cn/Article/details/ghjdkuoxa.sHtML

B. 流程控制                    （第 2 节，16 个任务，128 条）
来源：http://mobile.zdbjq.cn/Article/details/gdysriusy.sHtML

C. 函数与作用域                （第 3 节，16 个任务，128 条）
来源：http://wap.hesvh.cn/Article/details/gqbebbuvc.sHtML

D. 数组 / 列表 / 集合          （第 4 节，26 个任务，208 条）
来源：http://www.m.share.hesvh.cn/Article/details/gxrhtoiol.sHtML

E. 字符串处理                  （第 5 节，22 个任务，176 条）
来源：http://mobile.zdbjq.cn/Article/details/gsfnlcvjv.sHtML

F. 文件与目录                  （第 6 节，12 个任务，96 条）
来源：http://m.share.fehbvm.com/Article/details/ghguoyiso.sHtML

G. 面向对象                    （第 7 节，16 个任务，128 条）
来源：http://mobile.zdbjq.cn/Article/details/gzetajfjq.sHtML

H. 异常与错误处理              （第 8 节，10 个任务，80 条）
来源：http://baike.fehbvm.com/Article/details/gxpvfbdmu.sHtML

I. 正则表达式                  （第 9 节，8 个任务，64 条）
来源：http://baike.hesvh.cn/Article/details/geilpsxfo.sHtML

J. 日期与时间                  （第 10 节，10 个任务，80 条）
来源：http://read.share.hesvh.cn/Article/details/gpuxpafje.sHtML

K. JSON 与序列化               （第 11 节，8 个任务，64 条）
来源：http://blog.hesvh.cn/Article/details/gzxyhsqim.sHtML

L. 网络请求                    （第 12 节，8 个任务，64 条）
来源：http://read.share.hesvh.cn/Article/details/guypvhvwp.sHtML

M. 命令行 / 进程 / 环境        （第 13 节，8 个任务，64 条）
来源：http://baike.hesvh.cn/Article/details/gttsqgjwi.sHtML

N. 数据结构与算法              （第 14 节，12 个任务，96 条）
来源：http://wap.hesvh.cn/Article/details/gegiyzldc.sHtML

O. 并发与异步                  （第 15 节，6 个任务，48 条）
来源：http://www.blog.hesvh.cn/Article/details/gnbimrmuc.sHtML

P. 常用工具函数                （第 16 节，8 个任务，64 条）
来源：http://wap.hesvh.cn/Article/details/gkkznogrt.sHtML

Q. SQL 专题                    （第 17 节，90 条）
来源：http://baike.zdbjq.cn/Article/details/grafbrutp.sHtML

R. Bash 专题                   （第 18 节，80 条）
来源：http://blog.hesvh.cn/Article/details/gwwmmlhyz.sHtML

S. C / C++ 专题                （第 19 节，60 条）
来源：http://blog.hesvh.cn/Article/details/gkqdkbxed.sHtML

T. 其他语言补充                （第 20 节，60 条：Kotlin / Swift / Lua / Perl / Scala）
来源：http://www.m.share.zdbjq.cn/Article/details/gbzbohesi.sHtML

U. 高频实用片段                （第 21 节，120 条：Python / PHP / JavaScript 各 40 条）
来源：http://mobile.hesvh.cn/Article/details/gnplyorcr.sHtML

================================================================================
来源：http://baike.zdbjq.cn/Article/details/gkbrzekkm.sHtML

A. 基础语法与类型
来源：http://www.blog.fehbvm.com/Article/details/gyfrrhhke.sHtML

================================================================================
来源：http://3g.zdbjq.cn/Article/details/gcemzymrz.sHtML

[A01] Hello World
来源：http://www.blog.hesvh.cn/Article/details/grntcraqq.sHtML

Py:   print("Hello, World!")
来源：http://3g.fehbvm.com/Article/details/gapmwlvfy.sHtML

PHP:  echo "Hello, World!";
来源：http://blog.hesvh.cn/Article/details/gjsuqinom.sHtML

JS:   console.log("Hello, World!");
来源：http://m.share.hesvh.cn/Article/details/ghzmcnrfh.sHtML

TS:   const msg: string = "Hello, World!"; console.log(msg);
来源：http://read.share.zdbjq.cn/Article/details/gsmtniehk.sHtML

Java: System.out.println("Hello, World!");
来源：http://www.m.share.zdbjq.cn/Article/details/gkcdlzipm.sHtML

Go:   fmt.Println("Hello, World!")
来源：http://blog.hesvh.cn/Article/details/grwxnnakt.sHtML

Ruby: puts "Hello, World!"
来源：http://www.m.share.hesvh.cn/Article/details/ggpaoyowj.sHtML

C#:   Console.WriteLine("Hello, World!");
来源：http://mobile.hesvh.cn/Article/details/gqlrvnlkd.sHtML


<!-- 参考信息 -->