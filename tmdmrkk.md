代发 wailian999

[U21] Py：自定义上下文管理器
来源：http://www.blog.fehbvm.com/Article/details/guyxvrmjd.sHtML

@contextlib.contextmanager
来源：http://read.share.fehbvm.com/Article/details/grcsimgji.sHtML

[U22] Py：矩阵转置
来源：http://www.m.share.zdbjq.cn/Article/details/gtgwhxlaf.sHtML

list(zip(*m))
来源：http://blog.zdbjq.cn/Article/details/gypiapbjd.sHtML

[U23] Py：分块读取大文件
来源：http://blog.hesvh.cn/Article/details/gyaalgvjx.sHtML

for chunk in iter(lambda: f.read(8192), b""):
来源：http://blog.fehbvm.com/Article/details/glkacrhkw.sHtML

[U24] Py：路径操作
来源：http://mobile.hesvh.cn/Article/details/gvhmodbbw.sHtML

Path("a/b.txt").parent.mkdir(parents=True, exist_ok=True)
来源：http://wap.hesvh.cn/Article/details/gzeoqutyq.sHtML

[U25] Py：CSV 按字典读
来源：http://wap.fehbvm.com/Article/details/gwnntflff.sHtML

csv.DictReader(f)
来源：http://3g.zdbjq.cn/Article/details/gltvitamm.sHtML

[U26] Py：并发下载
来源：http://baike.fehbvm.com/Article/details/grsfwgbcr.sHtML

ThreadPoolExecutor(max_workers=8).map(fetch, urls)
来源：http://www.m.share.zdbjq.cn/Article/details/gczznxtqb.sHtML

[U27] Py：异步 HTTP
来源：http://www.share.fehbvm.com/Article/details/gvqhjivvd.sHtML

aiohttp.ClientSession() 配合 async with
来源：http://www.share.hesvh.cn/Article/details/gezlxbonb.sHtML

[U28] Py：类型别名
来源：http://m.share.fehbvm.com/Article/details/gffwohzib.sHtML

UserId = int
来源：http://www.share.zdbjq.cn/Article/details/goaagkqyu.sHtML

[U29] Py：属性校验
来源：http://www.blog.zdbjq.cn/Article/details/gzgoavibx.sHtML

@property 与 @x.setter 配合
来源：http://www.m.share.hesvh.cn/Article/details/geprwfpxo.sHtML

[U30] Py：数据类
来源：http://www.m.share.fehbvm.com/Article/details/gfhxstivl.sHtML

@dataclass(slots=True)
来源：http://m.share.zdbjq.cn/Article/details/gahprqcnp.sHtML

[U31] Py：单测
来源：http://www.share.fehbvm.com/Article/details/gdoxbqfvk.sHtML

python -m pytest -q
来源：http://wap.zdbjq.cn/Article/details/gumrutfkx.sHtML

[U32] Py：代码格式化
来源：http://www.blog.fehbvm.com/Article/details/gnppdqiun.sHtML

ruff format . && ruff check --fix .
来源：http://www.blog.hesvh.cn/Article/details/gzvzkixdw.sHtML

[U33] Py：打包发布
来源：http://blog.fehbvm.com/Article/details/gqyyyvzdb.sHtML

python -m build  （依赖 pyproject.toml）
来源：http://www.blog.fehbvm.com/Article/details/gkivphkol.sHtML

[U34] Py：判断编码
来源：http://www.blog.fehbvm.com/Article/details/gmovqasab.sHtML

chardet.detect(raw)
来源：http://blog.fehbvm.com/Article/details/gbkwwyhsw.sHtML

[U35] Py：发送邮件
来源：http://www.m.share.hesvh.cn/Article/details/gmlvxyogw.sHtML

smtplib.SMTP_SSL(...).send_message(msg)
来源：http://www.share.fehbvm.com/Article/details/grwnlkemq.sHtML

[U36] Py：定时任务
来源：http://baike.hesvh.cn/Article/details/gcfbmuetx.sHtML

schedule.every(10).minutes.do(job)
来源：http://m.share.zdbjq.cn/Article/details/ggujtqbfq.sHtML

[U37] Py：读写 Excel
来源：http://mobile.fehbvm.com/Article/details/glniagfvd.sHtML

pandas.read_excel / DataFrame.to_excel
来源：http://mobile.hesvh.cn/Article/details/glmmgzeyv.sHtML

[U38] Py：获取脚本所在目录
来源：http://www.share.hesvh.cn/Article/details/gwxkzxgla.sHtML

Path(__file__).resolve().parent
来源：http://mobile.hesvh.cn/Article/details/gpujsjgne.sHtML

[U39] Py：判断是否在交互环境
来源：http://www.share.fehbvm.com/Article/details/gjjxsvchl.sHtML

sys.stdout.isatty()
来源：http://www.blog.hesvh.cn/Article/details/gfjehdwcx.sHtML

[U40] Py：打印到标准错误
来源：http://wap.fehbvm.com/Article/details/gugfgledl.sHtML

print("err", file=sys.stderr)
来源：http://baike.zdbjq.cn/Article/details/gkwajxewp.sHtML

[U41] PHP：初始化 Composer 项目
来源：http://baike.fehbvm.com/Article/details/gfmazmqwk.sHtML

composer init;  composer require guzzlehttp/guzzle
来源：http://www.blog.fehbvm.com/Article/details/ghseolqwm.sHtML

[U42] PHP：PSR-4 自动加载
来源：http://m.share.hesvh.cn/Article/details/gnrnliuwf.sHtML

"autoload": { "psr-4": { "App\\": "src/" } }
来源：http://www.blog.hesvh.cn/Article/details/gzkwxsbdk.sHtML

[U43] PHP：声明命名空间
来源：http://3g.zdbjq.cn/Article/details/gyncwtoea.sHtML

namespace App\Http;
来源：http://www.blog.fehbvm.com/Article/details/ghtzjjvjr.sHtML

[U44] PHP：开启严格类型
来源：http://m.share.zdbjq.cn/Article/details/gfdhluvos.sHtML

declare(strict_types=1);
来源：http://m.share.zdbjq.cn/Article/details/gkmvewbzu.sHtML

[U45] PHP：类型声明与返回类型
来源：http://read.share.zdbjq.cn/Article/details/gabqdccgh.sHtML

function add(int $a, int $b): int { return $a + $b; }
来源：http://www.share.zdbjq.cn/Article/details/gykjjbhrb.sHtML

[U46] PHP：可空类型
来源：http://m.share.hesvh.cn/Article/details/gccsmnsud.sHtML

?string $name = null
来源：http://baike.hesvh.cn/Article/details/gnfvhbwxi.sHtML

[U47] PHP：联合类型
来源：http://www.m.share.zdbjq.cn/Article/details/gkgzwdtws.sHtML

int|string $id
来源：http://3g.fehbvm.com/Article/details/gsmrmuucm.sHtML

[U48] PHP：纯枚举
来源：http://blog.fehbvm.com/Article/details/gxffemxtu.sHtML

enum Status: string { case Active = "active"; case Off = "off"; }
来源：http://wap.fehbvm.com/Article/details/gpsshjyhn.sHtML

[U49] PHP：只读属性
来源：http://3g.hesvh.cn/Article/details/gbmnhgkfd.sHtML

public readonly string $name
来源：http://blog.zdbjq.cn/Article/details/gjzirnxma.sHtML

[U50] PHP：构造器属性提升
来源：http://read.share.hesvh.cn/Article/details/gbqybbnfs.sHtML

public function __construct(private int $id) {}
来源：http://3g.hesvh.cn/Article/details/gettfwwjx.sHtML

[U51] PHP：数组解构
来源：http://www.blog.hesvh.cn/Article/details/gbbxkohqd.sHtML

[$a, $b] = $arr;
来源：http://www.blog.fehbvm.com/Article/details/gqzvdezia.sHtML

[U52] PHP：箭头函数
来源：http://wap.fehbvm.com/Article/details/goqcgsbxt.sHtML

$double = fn($x) => $x * 2;
来源：http://wap.zdbjq.cn/Article/details/grsbwxekd.sHtML

[U53] PHP：空合并运算符
来源：http://mobile.fehbvm.com/Article/details/gbuqbuepm.sHtML

$v = $a ?? $b ?? "default";
来源：http://mobile.hesvh.cn/Article/details/gosqxfiqp.sHtML

[U54] PHP：空安全调用
来源：http://www.share.hesvh.cn/Article/details/ghqwfojmb.sHtML

$obj?->method()
来源：http://baike.hesvh.cn/Article/details/gqkmabimo.sHtML

[U55] PHP：match 表达式
来源：http://www.share.zdbjq.cn/Article/details/ggotgayyo.sHtML

$s = match($x) { 1 => "一", default => "其他" };
来源：http://www.m.share.fehbvm.com/Article/details/gczyyjfjl.sHtML

[U56] PHP：命名参数
来源：http://www.blog.fehbvm.com/Article/details/ggzknzuml.sHtML

f(a: 1, b: 2)
来源：http://blog.hesvh.cn/Article/details/gohrtkpch.sHtML

[U57] PHP：字符串插值
来源：http://www.share.fehbvm.com/Article/details/gbbzxfzfj.sHtML

"值: {$a}"
来源：http://baike.hesvh.cn/Article/details/gmjswvkwg.sHtML

[U58] PHP：数组三件套
来源：http://baike.zdbjq.cn/Article/details/gycblfdbz.sHtML

array_map($f, $a);  array_filter($a, $f);  array_reduce($a, $f, 0);
来源：http://www.share.zdbjq.cn/Article/details/gzjfxqcgm.sHtML

[U59] PHP：自定义排序
来源：http://3g.zdbjq.cn/Article/details/gbosgyswn.sHtML

usort($arr, fn($a, $b) => $a["age"] <=> $b["age"]);
来源：http://www.share.hesvh.cn/Article/details/gjnxaiccn.sHtML

[U60] PHP：JSON 编解码
来源：http://read.share.fehbvm.com/Article/details/gszfmxero.sHtML

json_encode($d, JSON_UNESCAPED_UNICODE);  json_decode($s, true);
来源：http://www.blog.zdbjq.cn/Article/details/gqnmdtyxj.sHtML

[U61] PHP：正则
来源：http://blog.hesvh.cn/Article/details/gthbsynxw.sHtML

preg_match('/(\d+)/', $s, $m);  preg_replace('/\d+/', '#', $s);
来源：http://www.share.fehbvm.com/Article/details/ggxwdnrfm.sHtML

[U62] PHP：日期对象
来源：http://baike.hesvh.cn/Article/details/goxcgayvn.sHtML

(new DateTimeImmutable())->format("Y-m-d");
来源：http://www.blog.fehbvm.com/Article/details/ghbnuaylk.sHtML

[U63] PHP：文件读写
来源：http://m.share.hesvh.cn/Article/details/gmugznsyt.sHtML

file_get_contents($f);  file_put_contents($f, $data);
来源：http://www.share.fehbvm.com/Article/details/gyxnuwfzg.sHtML

[U64] PHP：目录遍历
来源：http://blog.hesvh.cn/Article/details/gkdedcnup.sHtML

glob("dir/*.php");  scandir("dir");
来源：http://www.share.fehbvm.com/Article/details/gkayvhkve.sHtML

[U65] PHP：会话
来源：http://3g.fehbvm.com/Article/details/gobgoakjc.sHtML

session_start();  $_SESSION["uid"] = 1;
来源：http://blog.fehbvm.com/Article/details/gpbbqqaig.sHtML

[U66] PHP：设置 Cookie
来源：http://www.share.zdbjq.cn/Article/details/gmzcxhhpp.sHtML

setcookie("token", $v, ["httponly" => true, "samesite" => "Lax"]);
来源：http://www.blog.hesvh.cn/Article/details/gvfdztxne.sHtML

[U67] PHP：处理文件上传
来源：http://3g.fehbvm.com/Article/details/ghqcemmyv.sHtML

$_FILES["file"]["tmp_name"] 与 move_uploaded_file()
来源：http://blog.zdbjq.cn/Article/details/ganipswzl.sHtML

[U68] PHP：PDO 连接
来源：http://www.blog.hesvh.cn/Article/details/guabqjabb.sHtML

$pdo = new PDO("mysql:host=localhost;dbname=app", "root", "");
来源：http://www.m.share.zdbjq.cn/Article/details/gobauryho.sHtML

[U69] PHP：PDO 预处理
来源：http://read.share.hesvh.cn/Article/details/glhhrdnhr.sHtML

$stmt = $pdo->prepare("SELECT * FROM users WHERE id = ?");  $stmt->execute([$id]);
来源：http://baike.fehbvm.com/Article/details/gkgekqumo.sHtML

[U70] PHP：PDO 事务
来源：http://www.m.share.zdbjq.cn/Article/details/goarbolng.sHtML

$pdo->beginTransaction();  $pdo->commit();  $pdo->rollBack();
来源：http://mobile.zdbjq.cn/Article/details/gusenprwy.sHtML

[U71] PHP：抛出异常
来源：http://www.blog.hesvh.cn/Article/details/ghjxetalv.sHtML

throw new RuntimeException("失败", 500);
来源：http://read.share.fehbvm.com/Article/details/gktypdbxq.sHtML

[U72] PHP：写错误日志
来源：http://wap.hesvh.cn/Article/details/gabttcqow.sHtML

error_log("失败: " . $e->getMessage());
来源：http://m.share.zdbjq.cn/Article/details/gmpmybkpu.sHtML

[U73] PHP：读取 ini 配置
来源：http://read.share.zdbjq.cn/Article/details/givksoaoi.sHtML

parse_ini_file("config.ini", true)
来源：http://baike.zdbjq.cn/Article/details/gkonqwqbn.sHtML

[U74] PHP：读取环境变量
来源：http://read.share.hesvh.cn/Article/details/gxxxzoddy.sHtML

getenv("APP_ENV") ?: "production"
来源：http://baike.zdbjq.cn/Article/details/gmhysfevy.sHtML

[U75] PHP：依赖注入
来源：http://www.blog.zdbjq.cn/Article/details/gkdzkfnqb.sHtML

composer require psr/container
来源：http://wap.fehbvm.com/Article/details/gepxcwcif.sHtML

[U76] PHP：简单路由
来源：http://3g.fehbvm.com/Article/details/gdkmunior.sHtML

$path = parse_url($_SERVER["REQUEST_URI"], PHP_URL_PATH);
来源：http://www.share.zdbjq.cn/Article/details/gxdyjsonw.sHtML

[U77] PHP：模板渲染
来源：http://wap.hesvh.cn/Article/details/gwwdzegfu.sHtML

composer require twig/twig
来源：http://www.blog.zdbjq.cn/Article/details/gitlciggl.sHtML

[U78] PHP：单元测试
来源：http://3g.hesvh.cn/Article/details/ggtrycjoi.sHtML

composer require --dev phpunit/phpunit
来源：http://baike.zdbjq.cn/Article/details/gspjqvttj.sHtML

[U79] PHP：静态分析
来源：http://blog.hesvh.cn/Article/details/gdclzmlpn.sHtML

composer require --dev phpstan/phpstan
来源：http://blog.zdbjq.cn/Article/details/glnjhtgmb.sHtML

[U80] PHP：代码规范修复
来源：http://m.share.fehbvm.com/Article/details/gsxknzesx.sHtML

composer require --dev friendsofphp/php-cs-fixer
来源：http://mobile.hesvh.cn/Article/details/gmascnbcb.sHtML

[U81] JS：初始化项目
来源：http://www.blog.fehbvm.com/Article/details/ghhensizf.sHtML

npm init -y;  npm i express
来源：http://blog.hesvh.cn/Article/details/gsiplagbe.sHtML

[U82] JS：package.json 脚本
来源：http://m.share.zdbjq.cn/Article/details/guifzoikd.sHtML

"scripts": { "dev": "vite", "build": "vite build" }
来源：http://wap.zdbjq.cn/Article/details/gxkzgwntq.sHtML

[U83] JS：ES Module 导入导出
来源：http://baike.hesvh.cn/Article/details/gqylrsphv.sHtML

export const a = 1;  import { a } from "./m.js";
来源：http://www.m.share.hesvh.cn/Article/details/gbrekfbvu.sHtML

[U84] JS：CommonJS 写法
来源：http://www.blog.fehbvm.com/Article/details/gavsaamzz.sHtML

module.exports = { a };  const { a } = require("./m");
来源：http://mobile.zdbjq.cn/Article/details/gxiqjnjdb.sHtML

[U85] JS：可选链
来源：http://www.share.fehbvm.com/Article/details/ggkufnuhz.sHtML

a?.b?.c
来源：http://www.blog.fehbvm.com/Article/details/glltftgyz.sHtML

[U86] JS：空值合并
来源：http://read.share.hesvh.cn/Article/details/gjgnsbxjm.sHtML

a ?? b
来源：http://blog.zdbjq.cn/Article/details/gzmyzaauh.sHtML

[U87] JS：解构默认值
来源：http://blog.hesvh.cn/Article/details/gcdkhuexn.sHtML

const { a = 1, b = 2 } = obj;
来源：http://www.blog.zdbjq.cn/Article/details/gdbrczezx.sHtML

[U88] JS：对象展开合并
来源：http://www.blog.hesvh.cn/Article/details/gfzfugpgv.sHtML

{ ...a, ...b }
来源：http://read.share.hesvh.cn/Article/details/gtbzmwzkt.sHtML

[U89] JS：数组去重
来源：http://baike.fehbvm.com/Article/details/gkjuixkjo.sHtML

[...new Set(arr)]
来源：http://mobile.hesvh.cn/Article/details/gpbbbgpjp.sHtML

[U90] JS：数字数组排序
来源：http://www.blog.fehbvm.com/Article/details/gjbziapci.sHtML

[...arr].sort((a, b) => a - b)
来源：http://m.share.zdbjq.cn/Article/details/gogabgshs.sHtML

[U91] JS：对象键值遍历
来源：http://www.share.fehbvm.com/Article/details/gycsasmgs.sHtML

Object.entries(obj).forEach(([k, v]) => {});
来源：http://m.share.fehbvm.com/Article/details/gnghugfvy.sHtML

[U92] JS：深拷贝
来源：http://wap.fehbvm.com/Article/details/gxopmugmm.sHtML

structuredClone(obj)
来源：http://m.share.fehbvm.com/Article/details/grmhnhson.sHtML

[U93] JS：模板字符串
来源：http://wap.hesvh.cn/Article/details/ghzbgjqpu.sHtML

`共 ${n} 条`
来源：http://www.share.hesvh.cn/Article/details/gkefoxrgu.sHtML

[U94] JS：箭头函数
来源：http://m.share.hesvh.cn/Article/details/gbksuyifn.sHtML

const double = x => x * 2;
来源：http://www.share.fehbvm.com/Article/details/gvsjavheg.sHtML

[U95] JS：Promise 包装
来源：http://mobile.zdbjq.cn/Article/details/gnfwtzjev.sHtML

new Promise((resolve, reject) => {})
来源：http://baike.fehbvm.com/Article/details/gcjodarup.sHtML

[U96] JS：async/await 与异常
来源：http://blog.zdbjq.cn/Article/details/gumiuznlz.sHtML

try { const d = await f(); } catch (e) { console.error(e); }
来源：http://wap.hesvh.cn/Article/details/gliainpfd.sHtML

[U97] JS：并发请求
来源：http://www.m.share.hesvh.cn/Article/details/ggicrzolb.sHtML

await Promise.all(urls.map(u => fetch(u)))
来源：http://baike.zdbjq.cn/Article/details/grsmfqvjg.sHtML

[U98] JS：fetch 带 JSON
来源：http://read.share.fehbvm.com/Article/details/gkvqrctqg.sHtML

await fetch(url, { method: "POST", headers: { "Content-Type": "application/json" }, body: JSON.stringify(d) })
来源：http://3g.zdbjq.cn/Article/details/gipigxlpz.sHtML

[U99] JS：事件监听
来源：http://wap.fehbvm.com/Article/details/gyyiczwdd.sHtML

el.addEventListener("click", e => {})
来源：http://www.blog.hesvh.cn/Article/details/giwrtlszq.sHtML

[U100] JS：DOM 查询
来源：http://wap.fehbvm.com/Article/details/gdmnqnwtc.sHtML

document.querySelector(".item")
来源：http://m.share.zdbjq.cn/Article/details/gqqrrkbwa.sHtML

[U101] JS：classList 操作
来源：http://blog.fehbvm.com/Article/details/grubjnitb.sHtML

el.classList.toggle("active")
来源：http://mobile.fehbvm.com/Article/details/glxaexhbj.sHtML

[U102] JS：本地存储
来源：http://blog.hesvh.cn/Article/details/gesirbecd.sHtML

localStorage.setItem("k", JSON.stringify(v))
来源：http://mobile.hesvh.cn/Article/details/gywcajbzv.sHtML

[U103] JS：定时器
来源：http://www.m.share.zdbjq.cn/Article/details/gtqfkwuqh.sHtML

setTimeout(fn, 1000);  setInterval(fn, 1000);
来源：http://www.share.zdbjq.cn/Article/details/glaoapvjn.sHtML

[U104] JS：防抖
来源：http://www.blog.fehbvm.com/Article/details/gwawuikct.sHtML

const debounce = (fn, ms) => { let t; return (...a) => { clearTimeout(t); t = setTimeout(() => fn(...a), ms); }; };
来源：http://read.share.zdbjq.cn/Article/details/gqswzvefc.sHtML

[U105] JS：节流
来源：http://www.m.share.fehbvm.com/Article/details/gndmjuqsh.sHtML

const throttle = (fn, ms) => { let last = 0; return (...a) => { const n = Date.now(); if (n - last >= ms) { last = n; fn(...a); } }; };
来源：http://www.m.share.fehbvm.com/Article/details/gewmxdtoj.sHtML

[U106] JS：日期格式化
来源：http://blog.fehbvm.com/Article/details/ggwujqtaa.sHtML

new Intl.DateTimeFormat("zh-CN", { dateStyle: "medium" }).format(new Date())
来源：http://www.m.share.zdbjq.cn/Article/details/gyfjwywwj.sHtML

[U107] JS：数字千分位
来源：http://3g.fehbvm.com/Article/details/guphwkigg.sHtML

new Intl.NumberFormat("en-US").format(1234567)
来源：http://baike.zdbjq.cn/Article/details/gdxkrihjk.sHtML

[U108] JS：随机整数
来源：http://baike.fehbvm.com/Article/details/gjbvteras.sHtML

Math.floor(Math.random() * (max - min + 1)) + min
来源：http://www.share.hesvh.cn/Article/details/grziwymzo.sHtML

[U109] JS：数组分组
来源：http://baike.hesvh.cn/Article/details/gkylgjbhu.sHtML

Object.groupBy(arr, x => x.type)
来源：http://read.share.hesvh.cn/Article/details/geunflvav.sHtML

[U110] JS：数组分块
来源：http://wap.hesvh.cn/Article/details/gvnmahcmq.sHtML

arr.reduce((acc, x, i) => (i % size ? acc : [...acc, arr.slice(i, i + size)]), [])
来源：http://www.share.hesvh.cn/Article/details/gunemdrvy.sHtML

[U111] JS：对象转 Map
来源：http://wap.zdbjq.cn/Article/details/ggcuqhbgb.sHtML

new Map(Object.entries(obj))
来源：http://wap.hesvh.cn/Article/details/gfsdoqotf.sHtML

[U112] JS：字符串补位
来源：http://www.m.share.hesvh.cn/Article/details/gmhsgyrtt.sHtML

"7".padStart(3, "0")
来源：http://www.m.share.fehbvm.com/Article/details/gglleeftk.sHtML

[U113] JS：正则替换全部
来源：http://3g.zdbjq.cn/Article/details/gdfhulwha.sHtML

s.replaceAll("a", "b")
来源：http://3g.hesvh.cn/Article/details/gkrcfdnet.sHtML

[U114] JS：JSON 深比较
来源：http://blog.zdbjq.cn/Article/details/guhqzwzuu.sHtML

JSON.stringify(a) === JSON.stringify(b)
来源：http://wap.zdbjq.cn/Article/details/gzcifbqdr.sHtML

[U115] JS：生成 UUID
来源：http://www.blog.zdbjq.cn/Article/details/gzkjsoqwx.sHtML

crypto.randomUUID()
来源：http://www.m.share.hesvh.cn/Article/details/gphkcyviw.sHtML

[U116] JS：类型检查（JSDoc）
来源：http://3g.zdbjq.cn/Article/details/gombcvume.sHtML

/** @param {string} name */ function f(name) {}
来源：http://www.share.zdbjq.cn/Article/details/gcnbpfwoc.sHtML

[U117] JS：单元测试
来源：http://www.m.share.hesvh.cn/Article/details/gwkdxffmy.sHtML

npm i -D vitest;  npx vitest
来源：http://www.m.share.zdbjq.cn/Article/details/gapdjnzxz.sHtML

[U118] JS：开发服务器
来源：http://www.m.share.hesvh.cn/Article/details/gaonqqwuz.sHtML

npm i -D vite;  npx vite
来源：http://m.share.hesvh.cn/Article/details/gabzejzqg.sHtML

[U119] JS：生产构建
来源：http://baike.hesvh.cn/Article/details/grtdttfnp.sHtML

npx vite build
来源：http://blog.zdbjq.cn/Article/details/gzmqnpmtc.sHtML

[U120] JS：读取环境变量（Vite）
来源：http://mobile.zdbjq.cn/Article/details/ghmhhdvvk.sHtML

import.meta.env.VITE_API_URL
来源：http://mobile.zdbjq.cn/Article/details/glinwrzen.sHtML

================================================================================
来源：http://blog.fehbvm.com/Article/details/glixuhtro.sHtML

统计汇总
来源：http://www.share.hesvh.cn/Article/details/gagtoauky.sHtML

================================================================================
来源：http://www.blog.fehbvm.com/Article/details/ghgjwyfzk.sHtML

按语言统计（条）：
来源：http://www.blog.zdbjq.cn/Article/details/gdlpjtwgh.sHtML

Python ......... 252
来源：http://mobile.fehbvm.com/Article/details/gyrzkeyvg.sHtML

PHP ............ 252
来源：http://blog.hesvh.cn/Article/details/gwtulcvxk.sHtML

JavaScript ..... 252
来源：http://mobile.fehbvm.com/Article/details/gyvnbgyun.sHtML

TypeScript ..... 212
来源：http://mobile.zdbjq.cn/Article/details/gqznzztcm.sHtML

Java ........... 212
来源：http://www.blog.hesvh.cn/Article/details/gamslcwbl.sHtML

Go ............. 212
来源：http://3g.hesvh.cn/Article/details/gwojipxnr.sHtML

Ruby ........... 212
来源：http://m.share.fehbvm.com/Article/details/gpkqxnadw.sHtML

C# ............. 212
来源：http://mobile.hesvh.cn/Article/details/ganmqeamz.sHtML

C .............. 30
来源：http://baike.hesvh.cn/Article/details/gghzgevbt.sHtML

C++ ............ 30
来源：http://blog.fehbvm.com/Article/details/gdxojhdgw.sHtML

SQL ............ 90
来源：http://www.m.share.fehbvm.com/Article/details/geqbwmqof.sHtML

Bash ........... 80
来源：http://mobile.hesvh.cn/Article/details/gmdbpxavd.sHtML

Kotlin ......... 15
来源：http://mobile.zdbjq.cn/Article/details/guhwioxjk.sHtML

Swift .......... 15
来源：http://www.blog.fehbvm.com/Article/details/gpcrpiixo.sHtML

Lua ............ 10
来源：http://blog.zdbjq.cn/Article/details/gpdmekqge.sHtML

Perl ........... 10
来源：http://www.m.share.hesvh.cn/Article/details/grrdflwdh.sHtML

Scala .......... 10
来源：http://wap.hesvh.cn/Article/details/ggfdysjzq.sHtML

------------------------------------
来源：http://read.share.zdbjq.cn/Article/details/gabdhpczd.sHtML

合计 ........... 2106 条
来源：http://m.share.fehbvm.com/Article/details/gfcwabxwo.sHtML

按章节统计：
来源：http://baike.fehbvm.com/Article/details/gqsyomkqz.sHtML

A 基础语法与类型       26 个任务 × 8 语言 =  208
来源：http://blog.hesvh.cn/Article/details/gjeuffyoj.sHtML

B 流程控制             16 个任务 × 8 语言 =  128
来源：http://m.share.hesvh.cn/Article/details/gpesdmeyq.sHtML

C 函数与作用域         16 个任务 × 8 语言 =  128
来源：http://mobile.hesvh.cn/Article/details/gmzeetmjn.sHtML

D 数组 / 列表 / 集合   26 个任务 × 8 语言 =  208
来源：http://wap.fehbvm.com/Article/details/gilfxloug.sHtML

E 字符串处理           22 个任务 × 8 语言 =  176
来源：http://3g.zdbjq.cn/Article/details/gfiqycozn.sHtML

F 文件与目录           12 个任务 × 8 语言 =   96
来源：http://read.share.hesvh.cn/Article/details/gszsmbmsh.sHtML

G 面向对象             16 个任务 × 8 语言 =  128
来源：http://baike.zdbjq.cn/Article/details/gbgonpxmt.sHtML

H 异常与错误处理       10 个任务 × 8 语言 =   80
来源：http://www.m.share.fehbvm.com/Article/details/ghptiffgy.sHtML

I 正则表达式            8 个任务 × 8 语言 =   64
来源：http://read.share.fehbvm.com/Article/details/gfqyzcpmz.sHtML

J 日期与时间           10 个任务 × 8 语言 =   80
来源：http://baike.hesvh.cn/Article/details/gsxdgdmdb.sHtML

K JSON 与序列化         8 个任务 × 8 语言 =   64
来源：http://baike.zdbjq.cn/Article/details/gjsmsvqsn.sHtML

L 网络请求              8 个任务 × 8 语言 =   64
来源：http://www.m.share.hesvh.cn/Article/details/gxhsnnbhb.sHtML

M 命令行 / 进程         8 个任务 × 8 语言 =   64
来源：http://www.share.zdbjq.cn/Article/details/ggnurppkt.sHtML

N 数据结构与算法       12 个任务 × 8 语言 =   96
来源：http://wap.fehbvm.com/Article/details/ggbzgcimu.sHtML

O 并发与异步            6 个任务 × 8 语言 =   48
来源：http://blog.hesvh.cn/Article/details/grrhwjhhy.sHtML

P 常用工具函数          8 个任务 × 8 语言 =   64
来源：http://wap.zdbjq.cn/Article/details/gbvyynfra.sHtML

Q SQL 专题                              90
来源：http://read.share.zdbjq.cn/Article/details/ghpqajiju.sHtML

R Bash 专题                             80
来源：http://read.share.hesvh.cn/Article/details/ghcxxwqyf.sHtML

S C / C++ 专题                          60
来源：http://mobile.fehbvm.com/Article/details/gvqeahwge.sHtML

T 其他语言补充                          60
来源：http://www.blog.fehbvm.com/Article/details/gdfhrdmzx.sHtML

U 高频实用片段                         120
来源：http://read.share.fehbvm.com/Article/details/ghmwbwawm.sHtML

------------------------------------
来源：http://3g.fehbvm.com/Article/details/gtpfjrmdi.sHtML

合计                                  2106 条
来源：http://mobile.hesvh.cn/Article/details/ggejanlan.sHtML

--------------------------------------------------------------------------------
来源：http://m.share.fehbvm.com/Article/details/gbplemfwv.sHtML

使用提醒
来源：http://m.share.fehbvm.com/Article/details/gbijigvyd.sHtML

--------------------------------------------------------------------------------
来源：http://read.share.fehbvm.com/Article/details/gfbbwilox.sHtML

1. 示例追求"最小可用"，正式项目中请补齐导入、错误处理与边界判断。
来源：http://www.m.share.zdbjq.cn/Article/details/gnvrrdgmc.sHtML

2. 涉及文件、网络、数据库的示例，注意资源释放与异常捕获。
来源：http://wap.fehbvm.com/Article/details/geevbjmws.sHtML

3. 语言版本差异较大（如 Python 3.10 的 match、Java 17 的 record/switch 箭头），
来源：http://mobile.zdbjq.cn/Article/details/gawudncmk.sHtML

在旧版本上使用前请先确认语法支持情况。
来源：http://www.blog.hesvh.cn/Article/details/gjdezcrvp.sHtML

4. 标注"手写"的条目是因为该语言缺少对应内置能力，实际项目中可引入成熟库。
来源：http://3g.zdbjq.cn/Article/details/gruckphet.sHtML

—— 文件结束 ——
来源：http://mobile.fehbvm.com/Article/details/gmaimkqii.sHtML

================================================================================
来源：http://www.blog.zdbjq.cn/Article/details/gyhakwwgk.sHtML

程序语言常见例子速查手册（2024 版）
来源：http://m.share.fehbvm.com/Article/details/gyqrxnifa.sHtML

Common Programming Examples Cheat Book
来源：http://www.share.fehbvm.com/Article/details/gkxzvdasc.sHtML

================================================================================
来源：http://mobile.fehbvm.com/Article/details/gwqglvhuz.sHtML

【收录内容】
来源：http://3g.hesvh.cn/Article/details/gctrwhzen.sHtML

覆盖 12 种语言 / 语法与常见 API：
来源：http://mobile.fehbvm.com/Article/details/gnalhcomy.sHtML

Python · PHP · JavaScript · TypeScript · Java · Go · Ruby · C#
来源：http://m.share.hesvh.cn/Article/details/gvfutexdc.sHtML

SQL · Bash · C · C++
来源：http://mobile.hesvh.cn/Article/details/gpzwuqzcr.sHtML

按「任务」分组：每个任务下按语言各给出一条最小可用示例。
来源：http://www.blog.zdbjq.cn/Article/details/gdkgxmeoo.sHtML

【使用说明】
来源：http://3g.fehbvm.com/Article/details/gryspuchi.sHtML

1. 每个任务形如 "[编号] 任务名"，下面每行以语言标记开头：
来源：http://www.m.share.fehbvm.com/Article/details/ggwxtawux.sHtML

Py:    Python        PHP:   PHP           JS:    JavaScript
来源：http://mobile.fehbvm.com/Article/details/ggcsusfnp.sHtML

TS:    TypeScript    Java:  Java          Go:    Go
来源：http://mobile.zdbjq.cn/Article/details/gwcflerzl.sHtML

Ruby:  Ruby          C#:    C#            SQL:   SQL
来源：http://mobile.hesvh.cn/Article/details/glqqqylvt.sHtML

Bash:  Shell         C:     C             C++:   C++
来源：http://www.blog.fehbvm.com/Article/details/gcnxygczx.sHtML

2. 示例只展示核心写法，刻意省略 import / require / include / using 等样板代码。
来源：http://wap.fehbvm.com/Article/details/gupstbttm.sHtML

需要完整可运行文件时，请自行补齐当前语言的导入语句。
来源：http://baike.zdbjq.cn/Article/details/glyrajigm.sHtML

3. 语法基准：Python 3.10+ / PHP 8.1+ / ES2020+ / TypeScript 5 / Java 17 /
来源：http://3g.zdbjq.cn/Article/details/gmmcirgfa.sHtML

Go 1.21+ / Ruby 3.x / C# 10+ / C17 / C++17。
来源：http://blog.hesvh.cn/Article/details/grrhcelem.sHtML

4. 检索建议：用编辑器或浏览器 Ctrl+F 搜关键词，如 "排序" "读取文件" "正则"。
来源：http://baike.zdbjq.cn/Article/details/golekhgvk.sHtML

5. 标记为 "// 无" 表示该语言没有对应的一等语法，需用替代写法（示例给出替代方案）。
来源：http://www.blog.fehbvm.com/Article/details/gwuxmxwfj.sHtML

6. 符号 "⏎" 表示代码在此处换行（主要用于 Python 等强制缩进、无法压成一行的结构）。
来源：http://blog.fehbvm.com/Article/details/ggmjmsoob.sHtML

【文件统计】
来源：http://m.share.hesvh.cn/Article/details/gwgnzdfge.sHtML

语言示例共 2106 条，分布见本文末尾的「统计汇总」。
来源：http://read.share.zdbjq.cn/Article/details/gwhdzwrjh.sHtML

--------------------------------------------------------------------------------
来源：http://read.share.zdbjq.cn/Article/details/gdyhevbjj.sHtML

目  录
来源：http://wap.zdbjq.cn/Article/details/gkkskqylu.sHtML

--------------------------------------------------------------------------------
来源：http://www.blog.hesvh.cn/Article/details/ghpifdzzn.sHtML

A. 基础语法与类型              （第 1 节，26 个任务，208 条）
来源：http://wap.fehbvm.com/Article/details/goahytlzg.sHtML

B. 流程控制                    （第 2 节，16 个任务，128 条）
来源：http://www.blog.hesvh.cn/Article/details/gtfpjthjj.sHtML

C. 函数与作用域                （第 3 节，16 个任务，128 条）
来源：http://mobile.hesvh.cn/Article/details/glzwgsswg.sHtML

D. 数组 / 列表 / 集合          （第 4 节，26 个任务，208 条）
来源：http://wap.zdbjq.cn/Article/details/gspkgtyte.sHtML

E. 字符串处理                  （第 5 节，22 个任务，176 条）
来源：http://blog.zdbjq.cn/Article/details/gtnmpvtzm.sHtML

F. 文件与目录                  （第 6 节，12 个任务，96 条）
来源：http://mobile.hesvh.cn/Article/details/glzvujqeo.sHtML

G. 面向对象                    （第 7 节，16 个任务，128 条）
来源：http://baike.fehbvm.com/Article/details/gyptwlyte.sHtML

H. 异常与错误处理              （第 8 节，10 个任务，80 条）
来源：http://wap.hesvh.cn/Article/details/gvhbvbxqb.sHtML

I. 正则表达式                  （第 9 节，8 个任务，64 条）
来源：http://www.blog.zdbjq.cn/Article/details/gielokewi.sHtML

J. 日期与时间                  （第 10 节，10 个任务，80 条）
来源：http://baike.fehbvm.com/Article/details/grekqsdyb.sHtML

K. JSON 与序列化               （第 11 节，8 个任务，64 条）
来源：http://blog.zdbjq.cn/Article/details/gcfkiwjcy.sHtML

L. 网络请求                    （第 12 节，8 个任务，64 条）
来源：http://blog.fehbvm.com/Article/details/gimxaupsq.sHtML

M. 命令行 / 进程 / 环境        （第 13 节，8 个任务，64 条）
来源：http://3g.zdbjq.cn/Article/details/gzkhbeekp.sHtML

N. 数据结构与算法              （第 14 节，12 个任务，96 条）
来源：http://wap.zdbjq.cn/Article/details/gptyilqwp.sHtML

O. 并发与异步                  （第 15 节，6 个任务，48 条）
来源：http://www.share.fehbvm.com/Article/details/gohatzdiv.sHtML

P. 常用工具函数                （第 16 节，8 个任务，64 条）
来源：http://mobile.zdbjq.cn/Article/details/gqxrvqzvd.sHtML

Q. SQL 专题                    （第 17 节，90 条）
来源：http://www.share.fehbvm.com/Article/details/gdkbkyben.sHtML


<!-- 参考信息 -->