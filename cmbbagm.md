代发 wailian999

[U19] Py：正则替换带回调
来源：http://www.m.share.zdbjq.cn/Article/details/gnobajckc.sHtML

re.sub(r"\d+", lambda m: str(int(m.group()) * 2), s)
来源：http://3g.hesvh.cn/Article/details/grcybmybk.sHtML

[U20] Py：缓存函数结果
来源：http://blog.fehbvm.com/Article/details/gptjzighp.sHtML

@functools.lru_cache(maxsize=None)
来源：http://mobile.hesvh.cn/Article/details/gppchyvbu.sHtML

[U21] Py：自定义上下文管理器
来源：http://mobile.fehbvm.com/Article/details/gmrkutrvc.sHtML

@contextlib.contextmanager
来源：http://m.share.fehbvm.com/Article/details/gsfhqjcnd.sHtML

[U22] Py：矩阵转置
来源：http://wap.zdbjq.cn/Article/details/gukvlwsop.sHtML

list(zip(*m))
来源：http://www.m.share.fehbvm.com/Article/details/ghbxxziwm.sHtML

[U23] Py：分块读取大文件
来源：http://read.share.hesvh.cn/Article/details/gjmnrduuk.sHtML

for chunk in iter(lambda: f.read(8192), b""):
来源：http://read.share.hesvh.cn/Article/details/ggdcmnoqm.sHtML

[U24] Py：路径操作
来源：http://wap.zdbjq.cn/Article/details/gwaxzovgu.sHtML

Path("a/b.txt").parent.mkdir(parents=True, exist_ok=True)
来源：http://www.blog.zdbjq.cn/Article/details/gbwrhpirb.sHtML

[U25] Py：CSV 按字典读
来源：http://m.share.fehbvm.com/Article/details/gtkmnyvtd.sHtML

csv.DictReader(f)
来源：http://mobile.zdbjq.cn/Article/details/gfwclxbzn.sHtML

[U26] Py：并发下载
来源：http://www.blog.hesvh.cn/Article/details/glbqxthvb.sHtML

ThreadPoolExecutor(max_workers=8).map(fetch, urls)
来源：http://baike.hesvh.cn/Article/details/gfhomjrfz.sHtML

[U27] Py：异步 HTTP
来源：http://www.blog.fehbvm.com/Article/details/gsnzjpeky.sHtML

aiohttp.ClientSession() 配合 async with
来源：http://wap.zdbjq.cn/Article/details/ggxdvivsp.sHtML

[U28] Py：类型别名
来源：http://www.share.hesvh.cn/Article/details/gisujfdwe.sHtML

UserId = int
来源：http://baike.fehbvm.com/Article/details/gbqiamfqe.sHtML

[U29] Py：属性校验
来源：http://www.share.fehbvm.com/Article/details/gszeazibd.sHtML

@property 与 @x.setter 配合
来源：http://www.blog.zdbjq.cn/Article/details/gslcvqzgb.sHtML

[U30] Py：数据类
来源：http://www.blog.fehbvm.com/Article/details/gnhljwwix.sHtML

@dataclass(slots=True)
来源：http://3g.hesvh.cn/Article/details/gjgdkmnuh.sHtML

[U31] Py：单测
来源：http://www.m.share.fehbvm.com/Article/details/ggzhijmnq.sHtML

python -m pytest -q
来源：http://www.share.zdbjq.cn/Article/details/gggvrsfto.sHtML

[U32] Py：代码格式化
来源：http://www.blog.zdbjq.cn/Article/details/ghmqqsjha.sHtML

ruff format . && ruff check --fix .
来源：http://m.share.fehbvm.com/Article/details/gugoskgjk.sHtML

[U33] Py：打包发布
来源：http://www.blog.fehbvm.com/Article/details/gixbhyltx.sHtML

python -m build  （依赖 pyproject.toml）
来源：http://www.share.fehbvm.com/Article/details/gtqnmxogv.sHtML

[U34] Py：判断编码
来源：http://mobile.zdbjq.cn/Article/details/gekthdkme.sHtML

chardet.detect(raw)
来源：http://3g.zdbjq.cn/Article/details/gfqvrltlz.sHtML

[U35] Py：发送邮件
来源：http://3g.hesvh.cn/Article/details/gdauqhwgw.sHtML

smtplib.SMTP_SSL(...).send_message(msg)
来源：http://read.share.fehbvm.com/Article/details/gylbzwpgg.sHtML

[U36] Py：定时任务
来源：http://3g.fehbvm.com/Article/details/gvavosdtp.sHtML

schedule.every(10).minutes.do(job)
来源：http://www.m.share.zdbjq.cn/Article/details/gmxfgetso.sHtML

[U37] Py：读写 Excel
来源：http://wap.fehbvm.com/Article/details/gnmslurvp.sHtML

pandas.read_excel / DataFrame.to_excel
来源：http://3g.fehbvm.com/Article/details/gukjilazv.sHtML

[U38] Py：获取脚本所在目录
来源：http://3g.fehbvm.com/Article/details/gprolwwvf.sHtML

Path(__file__).resolve().parent
来源：http://read.share.zdbjq.cn/Article/details/giwatkmll.sHtML

[U39] Py：判断是否在交互环境
来源：http://3g.hesvh.cn/Article/details/grzepqcvp.sHtML

sys.stdout.isatty()
来源：http://3g.zdbjq.cn/Article/details/gircdpppt.sHtML

[U40] Py：打印到标准错误
来源：http://www.m.share.hesvh.cn/Article/details/gsotzjsev.sHtML

print("err", file=sys.stderr)
来源：http://blog.fehbvm.com/Article/details/gsixafqzh.sHtML

[U41] PHP：初始化 Composer 项目
来源：http://3g.zdbjq.cn/Article/details/guitlsang.sHtML

composer init;  composer require guzzlehttp/guzzle
来源：http://www.blog.zdbjq.cn/Article/details/gfvrieehm.sHtML

[U42] PHP：PSR-4 自动加载
来源：http://m.share.hesvh.cn/Article/details/glgdaoeau.sHtML

"autoload": { "psr-4": { "App\\": "src/" } }
来源：http://blog.hesvh.cn/Article/details/gnfctsvab.sHtML

[U43] PHP：声明命名空间
来源：http://mobile.fehbvm.com/Article/details/grlgbrxtr.sHtML

namespace App\Http;
来源：http://m.share.zdbjq.cn/Article/details/gazjyfgcg.sHtML

[U44] PHP：开启严格类型
来源：http://m.share.hesvh.cn/Article/details/gazcakegv.sHtML

declare(strict_types=1);
来源：http://wap.fehbvm.com/Article/details/gorwaifpe.sHtML

[U45] PHP：类型声明与返回类型
来源：http://wap.zdbjq.cn/Article/details/gceyqwpqs.sHtML

function add(int $a, int $b): int { return $a + $b; }
来源：http://www.m.share.zdbjq.cn/Article/details/grtafdcuu.sHtML

[U46] PHP：可空类型
来源：http://www.m.share.fehbvm.com/Article/details/gxsmnzkha.sHtML

?string $name = null
来源：http://3g.fehbvm.com/Article/details/gnoryxkcs.sHtML

[U47] PHP：联合类型
来源：http://read.share.hesvh.cn/Article/details/gtjddjlnf.sHtML

int|string $id
来源：http://wap.hesvh.cn/Article/details/grkwoslnf.sHtML

[U48] PHP：纯枚举
来源：http://baike.hesvh.cn/Article/details/gxsmoxzkb.sHtML

enum Status: string { case Active = "active"; case Off = "off"; }
来源：http://3g.fehbvm.com/Article/details/gtksketjz.sHtML

[U49] PHP：只读属性
来源：http://www.blog.zdbjq.cn/Article/details/gqoozgbgy.sHtML

public readonly string $name
来源：http://wap.fehbvm.com/Article/details/gwyyyovky.sHtML

[U50] PHP：构造器属性提升
来源：http://mobile.hesvh.cn/Article/details/gcwsvodla.sHtML

public function __construct(private int $id) {}
来源：http://www.share.zdbjq.cn/Article/details/ggulrshkg.sHtML

[U51] PHP：数组解构
来源：http://www.blog.zdbjq.cn/Article/details/gpfdyfxjc.sHtML

[$a, $b] = $arr;
来源：http://baike.hesvh.cn/Article/details/gznaxcghl.sHtML

[U52] PHP：箭头函数
来源：http://blog.hesvh.cn/Article/details/gwcemndcv.sHtML

$double = fn($x) => $x * 2;
来源：http://m.share.hesvh.cn/Article/details/gyimlueml.sHtML

[U53] PHP：空合并运算符
来源：http://mobile.zdbjq.cn/Article/details/ggwnczpir.sHtML

$v = $a ?? $b ?? "default";
来源：http://www.blog.fehbvm.com/Article/details/gbwolwbgg.sHtML

[U54] PHP：空安全调用
来源：http://m.share.zdbjq.cn/Article/details/gsbalwncm.sHtML

$obj?->method()
来源：http://baike.hesvh.cn/Article/details/gjhtfnuzp.sHtML

[U55] PHP：match 表达式
来源：http://wap.hesvh.cn/Article/details/gbhnqlelx.sHtML

$s = match($x) { 1 => "一", default => "其他" };
来源：http://read.share.fehbvm.com/Article/details/glgwqmmdy.sHtML

[U56] PHP：命名参数
来源：http://www.m.share.fehbvm.com/Article/details/gqtojziba.sHtML

f(a: 1, b: 2)
来源：http://mobile.zdbjq.cn/Article/details/gtjuosyeo.sHtML

[U57] PHP：字符串插值
来源：http://wap.fehbvm.com/Article/details/gwkwrpuqp.sHtML

"值: {$a}"
来源：http://www.blog.zdbjq.cn/Article/details/gdptupyvx.sHtML

[U58] PHP：数组三件套
来源：http://www.share.zdbjq.cn/Article/details/gxttrwkmu.sHtML

array_map($f, $a);  array_filter($a, $f);  array_reduce($a, $f, 0);
来源：http://wap.fehbvm.com/Article/details/gvwczmkss.sHtML

[U59] PHP：自定义排序
来源：http://read.share.fehbvm.com/Article/details/gvdjrwwqr.sHtML

usort($arr, fn($a, $b) => $a["age"] <=> $b["age"]);
来源：http://blog.zdbjq.cn/Article/details/gbuemiyxw.sHtML

[U60] PHP：JSON 编解码
来源：http://wap.zdbjq.cn/Article/details/gfkczarqu.sHtML

json_encode($d, JSON_UNESCAPED_UNICODE);  json_decode($s, true);
来源：http://m.share.zdbjq.cn/Article/details/gaexgkteg.sHtML

[U61] PHP：正则
来源：http://www.blog.hesvh.cn/Article/details/ginfczwzp.sHtML

preg_match('/(\d+)/', $s, $m);  preg_replace('/\d+/', '#', $s);
来源：http://3g.hesvh.cn/Article/details/gvozfxfrk.sHtML

[U62] PHP：日期对象
来源：http://wap.zdbjq.cn/Article/details/gahsqhxai.sHtML

(new DateTimeImmutable())->format("Y-m-d");
来源：http://3g.fehbvm.com/Article/details/gdqrhaoeh.sHtML

[U63] PHP：文件读写
来源：http://www.blog.fehbvm.com/Article/details/gvrlnsugg.sHtML

file_get_contents($f);  file_put_contents($f, $data);
来源：http://wap.zdbjq.cn/Article/details/galphsqfp.sHtML

[U64] PHP：目录遍历
来源：http://m.share.fehbvm.com/Article/details/glzjfystf.sHtML

glob("dir/*.php");  scandir("dir");
来源：http://m.share.fehbvm.com/Article/details/grkrrhuro.sHtML

[U65] PHP：会话
来源：http://wap.fehbvm.com/Article/details/grsuzfgvo.sHtML

session_start();  $_SESSION["uid"] = 1;
来源：http://wap.hesvh.cn/Article/details/gainejwwy.sHtML

[U66] PHP：设置 Cookie
来源：http://www.blog.hesvh.cn/Article/details/glvfaante.sHtML

setcookie("token", $v, ["httponly" => true, "samesite" => "Lax"]);
来源：http://wap.zdbjq.cn/Article/details/grxkbkdpf.sHtML

[U67] PHP：处理文件上传
来源：http://blog.fehbvm.com/Article/details/gmmbolrsc.sHtML

$_FILES["file"]["tmp_name"] 与 move_uploaded_file()
来源：http://read.share.zdbjq.cn/Article/details/gjwxoogmj.sHtML

[U68] PHP：PDO 连接
来源：http://wap.hesvh.cn/Article/details/gmqzeafgu.sHtML

$pdo = new PDO("mysql:host=localhost;dbname=app", "root", "");
来源：http://www.m.share.hesvh.cn/Article/details/gvgrpkphu.sHtML

[U69] PHP：PDO 预处理
来源：http://blog.fehbvm.com/Article/details/gmkglacye.sHtML

$stmt = $pdo->prepare("SELECT * FROM users WHERE id = ?");  $stmt->execute([$id]);
来源：http://www.m.share.zdbjq.cn/Article/details/gpjmsqeas.sHtML

[U70] PHP：PDO 事务
来源：http://blog.hesvh.cn/Article/details/gjdjgjemt.sHtML

$pdo->beginTransaction();  $pdo->commit();  $pdo->rollBack();
来源：http://m.share.fehbvm.com/Article/details/glyqnkvlm.sHtML

[U71] PHP：抛出异常
来源：http://www.blog.hesvh.cn/Article/details/gpphqqxbk.sHtML

throw new RuntimeException("失败", 500);
来源：http://mobile.fehbvm.com/Article/details/grrhesvkp.sHtML

[U72] PHP：写错误日志
来源：http://www.m.share.zdbjq.cn/Article/details/gksjouqzv.sHtML

error_log("失败: " . $e->getMessage());
来源：http://m.share.zdbjq.cn/Article/details/gwdrtzkuw.sHtML

[U73] PHP：读取 ini 配置
来源：http://www.blog.fehbvm.com/Article/details/geiqnmleu.sHtML

parse_ini_file("config.ini", true)
来源：http://3g.fehbvm.com/Article/details/gsfrjorwb.sHtML

[U74] PHP：读取环境变量
来源：http://wap.hesvh.cn/Article/details/gwmxzfpto.sHtML

getenv("APP_ENV") ?: "production"
来源：http://mobile.fehbvm.com/Article/details/gycqrhmzo.sHtML

[U75] PHP：依赖注入
来源：http://www.m.share.zdbjq.cn/Article/details/guzxfkmer.sHtML

composer require psr/container
来源：http://www.m.share.fehbvm.com/Article/details/gwdosicdr.sHtML

[U76] PHP：简单路由
来源：http://m.share.hesvh.cn/Article/details/goepurghm.sHtML

$path = parse_url($_SERVER["REQUEST_URI"], PHP_URL_PATH);
来源：http://blog.hesvh.cn/Article/details/gbvresfnp.sHtML

[U77] PHP：模板渲染
来源：http://www.m.share.zdbjq.cn/Article/details/gdojkyzdv.sHtML

composer require twig/twig
来源：http://m.share.zdbjq.cn/Article/details/gpdnbexsl.sHtML

[U78] PHP：单元测试
来源：http://m.share.fehbvm.com/Article/details/guhsogmhe.sHtML

composer require --dev phpunit/phpunit
来源：http://blog.fehbvm.com/Article/details/gwjwgeafi.sHtML

[U79] PHP：静态分析
来源：http://m.share.hesvh.cn/Article/details/gqujsoztf.sHtML

composer require --dev phpstan/phpstan
来源：http://m.share.zdbjq.cn/Article/details/gvropefju.sHtML

[U80] PHP：代码规范修复
来源：http://mobile.hesvh.cn/Article/details/gpqnnxkxl.sHtML

composer require --dev friendsofphp/php-cs-fixer
来源：http://www.blog.hesvh.cn/Article/details/gjvglsccx.sHtML

[U81] JS：初始化项目
来源：http://3g.fehbvm.com/Article/details/gjdnbjusr.sHtML

npm init -y;  npm i express
来源：http://3g.fehbvm.com/Article/details/gnnsddrmq.sHtML

[U82] JS：package.json 脚本
来源：http://blog.hesvh.cn/Article/details/gwucjfkzo.sHtML

"scripts": { "dev": "vite", "build": "vite build" }
来源：http://mobile.zdbjq.cn/Article/details/gthptqgnw.sHtML

[U83] JS：ES Module 导入导出
来源：http://www.blog.hesvh.cn/Article/details/gjvqtorpx.sHtML

export const a = 1;  import { a } from "./m.js";
来源：http://wap.hesvh.cn/Article/details/gdnipvqsc.sHtML

[U84] JS：CommonJS 写法
来源：http://3g.fehbvm.com/Article/details/gjzkoqnha.sHtML

module.exports = { a };  const { a } = require("./m");
来源：http://read.share.zdbjq.cn/Article/details/gldtkqpcu.sHtML

[U85] JS：可选链
来源：http://3g.hesvh.cn/Article/details/gtpexlwpm.sHtML

a?.b?.c
来源：http://baike.hesvh.cn/Article/details/gjgadovbd.sHtML

[U86] JS：空值合并
来源：http://www.share.zdbjq.cn/Article/details/gnoeltxqk.sHtML

a ?? b
来源：http://wap.hesvh.cn/Article/details/gwimtzpvm.sHtML

[U87] JS：解构默认值
来源：http://read.share.hesvh.cn/Article/details/gibeogrnn.sHtML

const { a = 1, b = 2 } = obj;
来源：http://baike.fehbvm.com/Article/details/guzdoksew.sHtML

[U88] JS：对象展开合并
来源：http://wap.fehbvm.com/Article/details/gyybllbzw.sHtML

{ ...a, ...b }
来源：http://www.blog.hesvh.cn/Article/details/grjgrvrcg.sHtML

[U89] JS：数组去重
来源：http://read.share.fehbvm.com/Article/details/gkewnwpai.sHtML

[...new Set(arr)]
来源：http://mobile.zdbjq.cn/Article/details/gubacvvxd.sHtML

[U90] JS：数字数组排序
来源：http://www.blog.zdbjq.cn/Article/details/gujizbale.sHtML

[...arr].sort((a, b) => a - b)
来源：http://read.share.hesvh.cn/Article/details/grovkkhrv.sHtML

[U91] JS：对象键值遍历
来源：http://wap.hesvh.cn/Article/details/goimicccv.sHtML

Object.entries(obj).forEach(([k, v]) => {});
来源：http://3g.hesvh.cn/Article/details/gzjyfrzkp.sHtML

[U92] JS：深拷贝
来源：http://mobile.hesvh.cn/Article/details/gqskyweod.sHtML

structuredClone(obj)
来源：http://mobile.hesvh.cn/Article/details/gxowgxfyo.sHtML

[U93] JS：模板字符串
来源：http://3g.zdbjq.cn/Article/details/gczokkewq.sHtML

`共 ${n} 条`
来源：http://mobile.zdbjq.cn/Article/details/gjkbkmabp.sHtML

[U94] JS：箭头函数
来源：http://mobile.fehbvm.com/Article/details/ggykfkaov.sHtML

const double = x => x * 2;
来源：http://baike.fehbvm.com/Article/details/guggpthiz.sHtML

[U95] JS：Promise 包装
来源：http://www.share.fehbvm.com/Article/details/gehsvzvin.sHtML

new Promise((resolve, reject) => {})
来源：http://www.share.zdbjq.cn/Article/details/gpfgabxmh.sHtML

[U96] JS：async/await 与异常
来源：http://www.m.share.hesvh.cn/Article/details/gnfpycqzo.sHtML

try { const d = await f(); } catch (e) { console.error(e); }
来源：http://www.share.fehbvm.com/Article/details/guuufvhsi.sHtML

[U97] JS：并发请求
来源：http://blog.hesvh.cn/Article/details/gshyzknvt.sHtML

await Promise.all(urls.map(u => fetch(u)))
来源：http://www.blog.hesvh.cn/Article/details/gynykvqnl.sHtML

[U98] JS：fetch 带 JSON
来源：http://read.share.fehbvm.com/Article/details/gxooozxyc.sHtML

await fetch(url, { method: "POST", headers: { "Content-Type": "application/json" }, body: JSON.stringify(d) })
来源：http://www.blog.hesvh.cn/Article/details/gdstdilou.sHtML

[U99] JS：事件监听
来源：http://mobile.zdbjq.cn/Article/details/ggfpyhuzu.sHtML

el.addEventListener("click", e => {})
来源：http://www.m.share.fehbvm.com/Article/details/gumygrlzy.sHtML

[U100] JS：DOM 查询
来源：http://www.share.hesvh.cn/Article/details/garszsfxi.sHtML

document.querySelector(".item")
来源：http://www.share.hesvh.cn/Article/details/gudsqiifx.sHtML

[U101] JS：classList 操作
来源：http://3g.hesvh.cn/Article/details/gltqpkuin.sHtML

el.classList.toggle("active")
来源：http://mobile.hesvh.cn/Article/details/gjxeorwhd.sHtML

[U102] JS：本地存储
来源：http://www.blog.fehbvm.com/Article/details/ggkfjwkhg.sHtML

localStorage.setItem("k", JSON.stringify(v))
来源：http://www.m.share.hesvh.cn/Article/details/gjgxukfve.sHtML

[U103] JS：定时器
来源：http://www.m.share.zdbjq.cn/Article/details/gurfdhdpd.sHtML

setTimeout(fn, 1000);  setInterval(fn, 1000);
来源：http://read.share.hesvh.cn/Article/details/gskpvslrm.sHtML

[U104] JS：防抖
来源：http://m.share.zdbjq.cn/Article/details/grhoczvgb.sHtML

const debounce = (fn, ms) => { let t; return (...a) => { clearTimeout(t); t = setTimeout(() => fn(...a), ms); }; };
来源：http://read.share.fehbvm.com/Article/details/gnrwfsfmu.sHtML

[U105] JS：节流
来源：http://www.share.hesvh.cn/Article/details/gduczyvoj.sHtML

const throttle = (fn, ms) => { let last = 0; return (...a) => { const n = Date.now(); if (n - last >= ms) { last = n; fn(...a); } }; };
来源：http://wap.fehbvm.com/Article/details/gsyctoatv.sHtML

[U106] JS：日期格式化
来源：http://wap.hesvh.cn/Article/details/glmopbuts.sHtML

new Intl.DateTimeFormat("zh-CN", { dateStyle: "medium" }).format(new Date())
来源：http://baike.hesvh.cn/Article/details/gzqvtwouf.sHtML

[U107] JS：数字千分位
来源：http://m.share.fehbvm.com/Article/details/geqwsivzm.sHtML

new Intl.NumberFormat("en-US").format(1234567)
来源：http://3g.fehbvm.com/Article/details/gypqfvmlz.sHtML

[U108] JS：随机整数
来源：http://www.blog.fehbvm.com/Article/details/gnzefbyjn.sHtML

Math.floor(Math.random() * (max - min + 1)) + min
来源：http://3g.hesvh.cn/Article/details/gxfaoxprz.sHtML

[U109] JS：数组分组
来源：http://3g.hesvh.cn/Article/details/gtqbtybnh.sHtML

Object.groupBy(arr, x => x.type)
来源：http://read.share.hesvh.cn/Article/details/gycbwsmbg.sHtML

[U110] JS：数组分块
来源：http://wap.fehbvm.com/Article/details/gqnocjodc.sHtML

arr.reduce((acc, x, i) => (i % size ? acc : [...acc, arr.slice(i, i + size)]), [])
来源：http://baike.zdbjq.cn/Article/details/ghwptpong.sHtML

[U111] JS：对象转 Map
来源：http://m.share.hesvh.cn/Article/details/ghwiyynwa.sHtML

new Map(Object.entries(obj))
来源：http://baike.zdbjq.cn/Article/details/gjkxpxhum.sHtML

[U112] JS：字符串补位
来源：http://www.blog.hesvh.cn/Article/details/gvoprpcwy.sHtML

"7".padStart(3, "0")
来源：http://www.m.share.zdbjq.cn/Article/details/gonpugijl.sHtML

[U113] JS：正则替换全部
来源：http://m.share.hesvh.cn/Article/details/gvwxkhpny.sHtML

s.replaceAll("a", "b")
来源：http://3g.hesvh.cn/Article/details/gdannceew.sHtML

[U114] JS：JSON 深比较
来源：http://blog.hesvh.cn/Article/details/gnnayhfsc.sHtML

JSON.stringify(a) === JSON.stringify(b)
来源：http://baike.hesvh.cn/Article/details/gvztunvlp.sHtML

[U115] JS：生成 UUID
来源：http://3g.fehbvm.com/Article/details/gtuiuqjqi.sHtML

crypto.randomUUID()
来源：http://m.share.zdbjq.cn/Article/details/gnbdimlta.sHtML

[U116] JS：类型检查（JSDoc）
来源：http://www.share.fehbvm.com/Article/details/gjdtpjmzn.sHtML

/** @param {string} name */ function f(name) {}
来源：http://read.share.fehbvm.com/Article/details/godrntgmo.sHtML

[U117] JS：单元测试
来源：http://wap.zdbjq.cn/Article/details/gvcpvwdxe.sHtML

npm i -D vitest;  npx vitest
来源：http://baike.fehbvm.com/Article/details/gbtamvjzg.sHtML

[U118] JS：开发服务器
来源：http://read.share.hesvh.cn/Article/details/gwscigkhe.sHtML

npm i -D vite;  npx vite
来源：http://read.share.fehbvm.com/Article/details/gusjgkgys.sHtML

[U119] JS：生产构建
来源：http://blog.hesvh.cn/Article/details/gwlyyshhx.sHtML

npx vite build
来源：http://www.share.zdbjq.cn/Article/details/gzovchjjd.sHtML

[U120] JS：读取环境变量（Vite）
来源：http://m.share.fehbvm.com/Article/details/gerigeray.sHtML

import.meta.env.VITE_API_URL
来源：http://mobile.hesvh.cn/Article/details/grjjtnfun.sHtML

================================================================================
来源：http://baike.hesvh.cn/Article/details/gzmpsghnb.sHtML

统计汇总
来源：http://wap.fehbvm.com/Article/details/gdnijwbtt.sHtML

================================================================================
来源：http://www.share.zdbjq.cn/Article/details/glrcbgycb.sHtML

按语言统计（条）：
来源：http://www.m.share.hesvh.cn/Article/details/gqalajbec.sHtML

Python ......... 252
来源：http://blog.hesvh.cn/Article/details/gqzxzkuts.sHtML

PHP ............ 252
来源：http://baike.hesvh.cn/Article/details/gpczgdymt.sHtML

JavaScript ..... 252
来源：http://blog.fehbvm.com/Article/details/gxnxlrcin.sHtML

TypeScript ..... 212
来源：http://www.m.share.hesvh.cn/Article/details/gydjpqwuu.sHtML

Java ........... 212
来源：http://www.share.fehbvm.com/Article/details/gmdhcsnly.sHtML

Go ............. 212
来源：http://www.m.share.zdbjq.cn/Article/details/gvqmngmgc.sHtML

Ruby ........... 212
来源：http://www.blog.fehbvm.com/Article/details/gyrjnewmm.sHtML

C# ............. 212
来源：http://www.share.hesvh.cn/Article/details/gtmtfzmgk.sHtML

C .............. 30
来源：http://wap.zdbjq.cn/Article/details/glnpmmhxq.sHtML

C++ ............ 30
来源：http://www.m.share.fehbvm.com/Article/details/glmavakmx.sHtML

SQL ............ 90
来源：http://read.share.hesvh.cn/Article/details/gkrmkfjry.sHtML

Bash ........... 80
来源：http://blog.zdbjq.cn/Article/details/gkcpfvqao.sHtML

Kotlin ......... 15
来源：http://www.share.zdbjq.cn/Article/details/guacizbwy.sHtML

Swift .......... 15
来源：http://blog.zdbjq.cn/Article/details/gozhmkega.sHtML

Lua ............ 10
来源：http://mobile.hesvh.cn/Article/details/gzybkhedf.sHtML

Perl ........... 10
来源：http://wap.fehbvm.com/Article/details/gnezrtfbo.sHtML

Scala .......... 10
来源：http://wap.fehbvm.com/Article/details/gapaffscz.sHtML

------------------------------------
来源：http://baike.fehbvm.com/Article/details/gjypeylfr.sHtML

合计 ........... 2106 条
来源：http://wap.hesvh.cn/Article/details/gmmbvakzl.sHtML

按章节统计：
来源：http://www.blog.fehbvm.com/Article/details/gudxnfjdf.sHtML

A 基础语法与类型       26 个任务 × 8 语言 =  208
来源：http://www.share.zdbjq.cn/Article/details/gthymfcnu.sHtML

B 流程控制             16 个任务 × 8 语言 =  128
来源：http://read.share.fehbvm.com/Article/details/ghsrabpcd.sHtML

C 函数与作用域         16 个任务 × 8 语言 =  128
来源：http://read.share.hesvh.cn/Article/details/gbbosqmiu.sHtML

D 数组 / 列表 / 集合   26 个任务 × 8 语言 =  208
来源：http://mobile.hesvh.cn/Article/details/gfmfwifbw.sHtML

E 字符串处理           22 个任务 × 8 语言 =  176
来源：http://mobile.hesvh.cn/Article/details/gxmneoauy.sHtML

F 文件与目录           12 个任务 × 8 语言 =   96
来源：http://mobile.fehbvm.com/Article/details/gnsahwomt.sHtML

G 面向对象             16 个任务 × 8 语言 =  128
来源：http://www.share.fehbvm.com/Article/details/gfolnecjg.sHtML

H 异常与错误处理       10 个任务 × 8 语言 =   80
来源：http://3g.zdbjq.cn/Article/details/grogdssix.sHtML

I 正则表达式            8 个任务 × 8 语言 =   64
来源：http://mobile.hesvh.cn/Article/details/gfsuvfufp.sHtML

J 日期与时间           10 个任务 × 8 语言 =   80
来源：http://baike.fehbvm.com/Article/details/gjbxqbtoj.sHtML

K JSON 与序列化         8 个任务 × 8 语言 =   64
来源：http://3g.hesvh.cn/Article/details/gswladlao.sHtML

L 网络请求              8 个任务 × 8 语言 =   64
来源：http://www.m.share.zdbjq.cn/Article/details/gjwtyrgqi.sHtML

M 命令行 / 进程         8 个任务 × 8 语言 =   64
来源：http://www.blog.fehbvm.com/Article/details/gbvlmywmf.sHtML

N 数据结构与算法       12 个任务 × 8 语言 =   96
来源：http://www.blog.fehbvm.com/Article/details/gjexfyrsw.sHtML

O 并发与异步            6 个任务 × 8 语言 =   48
来源：http://mobile.fehbvm.com/Article/details/gzoenfysb.sHtML

P 常用工具函数          8 个任务 × 8 语言 =   64
来源：http://baike.zdbjq.cn/Article/details/gpdmgcoej.sHtML

Q SQL 专题                              90
来源：http://blog.zdbjq.cn/Article/details/gbhibpfeg.sHtML

R Bash 专题                             80
来源：http://m.share.fehbvm.com/Article/details/gseuxpyjd.sHtML

S C / C++ 专题                          60
来源：http://baike.zdbjq.cn/Article/details/grvknaauh.sHtML

T 其他语言补充                          60
来源：http://3g.zdbjq.cn/Article/details/glslscyrg.sHtML

U 高频实用片段                         120
来源：http://wap.fehbvm.com/Article/details/gdbsatqxw.sHtML

------------------------------------
来源：http://www.m.share.fehbvm.com/Article/details/gfocnzfgs.sHtML

合计                                  2106 条
来源：http://www.blog.fehbvm.com/Article/details/gpysqssxa.sHtML

--------------------------------------------------------------------------------
来源：http://3g.fehbvm.com/Article/details/gxqcuurcl.sHtML

使用提醒
来源：http://www.m.share.hesvh.cn/Article/details/guxegawmb.sHtML

--------------------------------------------------------------------------------
来源：http://baike.hesvh.cn/Article/details/gzkqyhmql.sHtML

1. 示例追求"最小可用"，正式项目中请补齐导入、错误处理与边界判断。
来源：http://www.share.hesvh.cn/Article/details/ghmdlqpsu.sHtML

2. 涉及文件、网络、数据库的示例，注意资源释放与异常捕获。
来源：http://www.m.share.zdbjq.cn/Article/details/grfiywhwh.sHtML

3. 语言版本差异较大（如 Python 3.10 的 match、Java 17 的 record/switch 箭头），
来源：http://3g.hesvh.cn/Article/details/gzqjogaeb.sHtML

在旧版本上使用前请先确认语法支持情况。
来源：http://www.share.hesvh.cn/Article/details/gnpkdfcti.sHtML

4. 标注"手写"的条目是因为该语言缺少对应内置能力，实际项目中可引入成熟库。
来源：http://www.share.fehbvm.com/Article/details/gmxkisxxs.sHtML

—— 文件结束 ——
来源：http://m.share.fehbvm.com/Article/details/gcqaqxxnb.sHtML

================================================================================
来源：http://www.blog.zdbjq.cn/Article/details/gsplawthh.sHtML

程序语言常见例子速查手册（2024 版）
来源：http://www.share.zdbjq.cn/Article/details/gdbqnbbtk.sHtML

Common Programming Examples Cheat Book
来源：http://www.m.share.fehbvm.com/Article/details/gpaqqnets.sHtML

================================================================================
来源：http://wap.zdbjq.cn/Article/details/gqzsdvfxx.sHtML

【收录内容】
来源：http://blog.zdbjq.cn/Article/details/gjmjynnpr.sHtML

覆盖 12 种语言 / 语法与常见 API：
来源：http://baike.fehbvm.com/Article/details/gfeuoxztg.sHtML

Python · PHP · JavaScript · TypeScript · Java · Go · Ruby · C#
来源：http://www.m.share.zdbjq.cn/Article/details/geqktlnwh.sHtML

SQL · Bash · C · C++
来源：http://www.share.zdbjq.cn/Article/details/gldkmbswo.sHtML

按「任务」分组：每个任务下按语言各给出一条最小可用示例。
来源：http://3g.fehbvm.com/Article/details/gblkvqxry.sHtML

【使用说明】
来源：http://baike.fehbvm.com/Article/details/grfhlngeh.sHtML

1. 每个任务形如 "[编号] 任务名"，下面每行以语言标记开头：
来源：http://blog.fehbvm.com/Article/details/gvjgqqfpq.sHtML

Py:    Python        PHP:   PHP           JS:    JavaScript
来源：http://baike.zdbjq.cn/Article/details/gbbdojsrb.sHtML

TS:    TypeScript    Java:  Java          Go:    Go
来源：http://www.m.share.fehbvm.com/Article/details/gfscajftc.sHtML

Ruby:  Ruby          C#:    C#            SQL:   SQL
来源：http://www.share.zdbjq.cn/Article/details/ghppigisv.sHtML

Bash:  Shell         C:     C             C++:   C++
来源：http://www.m.share.fehbvm.com/Article/details/gaeboohhd.sHtML

2. 示例只展示核心写法，刻意省略 import / require / include / using 等样板代码。
来源：http://read.share.fehbvm.com/Article/details/giqjiybyp.sHtML

需要完整可运行文件时，请自行补齐当前语言的导入语句。
来源：http://m.share.fehbvm.com/Article/details/gvlceposh.sHtML

3. 语法基准：Python 3.10+ / PHP 8.1+ / ES2020+ / TypeScript 5 / Java 17 /
来源：http://m.share.fehbvm.com/Article/details/ghfyicylf.sHtML

Go 1.21+ / Ruby 3.x / C# 10+ / C17 / C++17。
来源：http://mobile.fehbvm.com/Article/details/grehvjqby.sHtML

4. 检索建议：用编辑器或浏览器 Ctrl+F 搜关键词，如 "排序" "读取文件" "正则"。
来源：http://blog.fehbvm.com/Article/details/gkeeuhkbb.sHtML

5. 标记为 "// 无" 表示该语言没有对应的一等语法，需用替代写法（示例给出替代方案）。
来源：http://baike.fehbvm.com/Article/details/gxslzjamq.sHtML

6. 符号 "⏎" 表示代码在此处换行（主要用于 Python 等强制缩进、无法压成一行的结构）。
来源：http://www.blog.zdbjq.cn/Article/details/gguyparti.sHtML

【文件统计】
来源：http://blog.zdbjq.cn/Article/details/glkmmabck.sHtML

语言示例共 2106 条，分布见本文末尾的「统计汇总」。
来源：http://blog.hesvh.cn/Article/details/gsyfbrgeq.sHtML

--------------------------------------------------------------------------------
来源：http://3g.hesvh.cn/Article/details/gvrmbcgcu.sHtML

目  录
来源：http://wap.zdbjq.cn/Article/details/gmuqdqlks.sHtML

--------------------------------------------------------------------------------
来源：http://www.blog.hesvh.cn/Article/details/gpaclpxys.sHtML

A. 基础语法与类型              （第 1 节，26 个任务，208 条）
来源：http://www.share.hesvh.cn/Article/details/gblxraeqs.sHtML

B. 流程控制                    （第 2 节，16 个任务，128 条）
来源：http://www.blog.zdbjq.cn/Article/details/gfejxrary.sHtML

C. 函数与作用域                （第 3 节，16 个任务，128 条）
来源：http://3g.zdbjq.cn/Article/details/gjkmjskwr.sHtML

D. 数组 / 列表 / 集合          （第 4 节，26 个任务，208 条）
来源：http://www.blog.hesvh.cn/Article/details/gtgfwrcvl.sHtML

E. 字符串处理                  （第 5 节，22 个任务，176 条）
来源：http://read.share.hesvh.cn/Article/details/gyvtizfny.sHtML

F. 文件与目录                  （第 6 节，12 个任务，96 条）
来源：http://baike.fehbvm.com/Article/details/gxqowafbp.sHtML

G. 面向对象                    （第 7 节，16 个任务，128 条）
来源：http://baike.fehbvm.com/Article/details/gttkmlwrp.sHtML

H. 异常与错误处理              （第 8 节，10 个任务，80 条）
来源：http://blog.zdbjq.cn/Article/details/gnkonwypt.sHtML

I. 正则表达式                  （第 9 节，8 个任务，64 条）
来源：http://3g.zdbjq.cn/Article/details/gzxockclh.sHtML

J. 日期与时间                  （第 10 节，10 个任务，80 条）
来源：http://3g.hesvh.cn/Article/details/gefvrrfar.sHtML

K. JSON 与序列化               （第 11 节，8 个任务，64 条）
来源：http://m.share.fehbvm.com/Article/details/gvhsexujo.sHtML

L. 网络请求                    （第 12 节，8 个任务，64 条）
来源：http://wap.hesvh.cn/Article/details/gwplqtdav.sHtML

M. 命令行 / 进程 / 环境        （第 13 节，8 个任务，64 条）
来源：http://www.m.share.fehbvm.com/Article/details/ggrfxklzs.sHtML


<!-- 参考信息 -->