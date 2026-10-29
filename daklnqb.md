代发 wailian999

[U19] Py：正则替换带回调
来源：http://3g.fehbvm.com/Article/details/guktyhfcc.sHtML

re.sub(r"\d+", lambda m: str(int(m.group()) * 2), s)
来源：http://read.share.hesvh.cn/Article/details/gkoonlzzp.sHtML

[U20] Py：缓存函数结果
来源：http://www.blog.hesvh.cn/Article/details/gcylbxqwl.sHtML

@functools.lru_cache(maxsize=None)
来源：http://m.share.hesvh.cn/Article/details/gwahlqxfy.sHtML

[U21] Py：自定义上下文管理器
来源：http://baike.fehbvm.com/Article/details/ggkmloreg.sHtML

@contextlib.contextmanager
来源：http://www.m.share.fehbvm.com/Article/details/gnnwznreb.sHtML

[U22] Py：矩阵转置
来源：http://read.share.zdbjq.cn/Article/details/gjplwniqb.sHtML

list(zip(*m))
来源：http://baike.zdbjq.cn/Article/details/gprseaxrr.sHtML

[U23] Py：分块读取大文件
来源：http://blog.zdbjq.cn/Article/details/gdubzoqmj.sHtML

for chunk in iter(lambda: f.read(8192), b""):
来源：http://blog.fehbvm.com/Article/details/gzloqlhla.sHtML

[U24] Py：路径操作
来源：http://wap.hesvh.cn/Article/details/gmjnebscr.sHtML

Path("a/b.txt").parent.mkdir(parents=True, exist_ok=True)
来源：http://www.m.share.fehbvm.com/Article/details/gvniqduec.sHtML

[U25] Py：CSV 按字典读
来源：http://www.m.share.zdbjq.cn/Article/details/glbfihbbe.sHtML

csv.DictReader(f)
来源：http://blog.hesvh.cn/Article/details/giqsavtje.sHtML

[U26] Py：并发下载
来源：http://www.blog.zdbjq.cn/Article/details/gryefgawk.sHtML

ThreadPoolExecutor(max_workers=8).map(fetch, urls)
来源：http://baike.hesvh.cn/Article/details/gerwatqdp.sHtML

[U27] Py：异步 HTTP
来源：http://wap.fehbvm.com/Article/details/gnovifkzv.sHtML

aiohttp.ClientSession() 配合 async with
来源：http://www.blog.hesvh.cn/Article/details/gkqjfmahr.sHtML

[U28] Py：类型别名
来源：http://www.share.hesvh.cn/Article/details/gjgwtyzqq.sHtML

UserId = int
来源：http://mobile.hesvh.cn/Article/details/gllyvdmkn.sHtML

[U29] Py：属性校验
来源：http://blog.zdbjq.cn/Article/details/gkukiyvzf.sHtML

@property 与 @x.setter 配合
来源：http://mobile.fehbvm.com/Article/details/gtoiaeuhq.sHtML

[U30] Py：数据类
来源：http://wap.zdbjq.cn/Article/details/ghyrshqmv.sHtML

@dataclass(slots=True)
来源：http://www.share.zdbjq.cn/Article/details/gfvzbkuqc.sHtML

[U31] Py：单测
来源：http://www.share.zdbjq.cn/Article/details/gofqmrmbu.sHtML

python -m pytest -q
来源：http://3g.hesvh.cn/Article/details/gsglmqivx.sHtML

[U32] Py：代码格式化
来源：http://read.share.fehbvm.com/Article/details/gotdarcic.sHtML

ruff format . && ruff check --fix .
来源：http://3g.zdbjq.cn/Article/details/gxaehmtjd.sHtML

[U33] Py：打包发布
来源：http://m.share.fehbvm.com/Article/details/gaadcxygw.sHtML

python -m build  （依赖 pyproject.toml）
来源：http://www.share.zdbjq.cn/Article/details/gsqxptgao.sHtML

[U34] Py：判断编码
来源：http://www.share.hesvh.cn/Article/details/gznlhgfns.sHtML

chardet.detect(raw)
来源：http://www.m.share.hesvh.cn/Article/details/gnjnfflre.sHtML

[U35] Py：发送邮件
来源：http://mobile.hesvh.cn/Article/details/gtekjnkkt.sHtML

smtplib.SMTP_SSL(...).send_message(msg)
来源：http://www.m.share.zdbjq.cn/Article/details/gwhvfkghx.sHtML

[U36] Py：定时任务
来源：http://baike.fehbvm.com/Article/details/gjfinhjka.sHtML

schedule.every(10).minutes.do(job)
来源：http://www.blog.hesvh.cn/Article/details/gqdlglbnu.sHtML

[U37] Py：读写 Excel
来源：http://blog.fehbvm.com/Article/details/gxfbmcxal.sHtML

pandas.read_excel / DataFrame.to_excel
来源：http://baike.fehbvm.com/Article/details/gqlszqwcf.sHtML

[U38] Py：获取脚本所在目录
来源：http://blog.hesvh.cn/Article/details/gngmcsios.sHtML

Path(__file__).resolve().parent
来源：http://www.m.share.zdbjq.cn/Article/details/gkliiealp.sHtML

[U39] Py：判断是否在交互环境
来源：http://baike.hesvh.cn/Article/details/gvtsokdws.sHtML

sys.stdout.isatty()
来源：http://www.m.share.zdbjq.cn/Article/details/gahjubyvk.sHtML

[U40] Py：打印到标准错误
来源：http://wap.zdbjq.cn/Article/details/gveedlzbe.sHtML

print("err", file=sys.stderr)
来源：http://www.blog.hesvh.cn/Article/details/gyrwlwslc.sHtML

[U41] PHP：初始化 Composer 项目
来源：http://3g.zdbjq.cn/Article/details/gjtwvbmhz.sHtML

composer init;  composer require guzzlehttp/guzzle
来源：http://mobile.zdbjq.cn/Article/details/gepxguhsc.sHtML

[U42] PHP：PSR-4 自动加载
来源：http://blog.zdbjq.cn/Article/details/gqvcetoif.sHtML

"autoload": { "psr-4": { "App\\": "src/" } }
来源：http://mobile.hesvh.cn/Article/details/glzzjbylh.sHtML

[U43] PHP：声明命名空间
来源：http://baike.hesvh.cn/Article/details/gvvhfwcxp.sHtML

namespace App\Http;
来源：http://www.m.share.fehbvm.com/Article/details/gyhhmyira.sHtML

[U44] PHP：开启严格类型
来源：http://www.blog.hesvh.cn/Article/details/gduaknmzm.sHtML

declare(strict_types=1);
来源：http://mobile.hesvh.cn/Article/details/gpqxiyhxl.sHtML

[U45] PHP：类型声明与返回类型
来源：http://blog.zdbjq.cn/Article/details/gutkayhay.sHtML

function add(int $a, int $b): int { return $a + $b; }
来源：http://3g.zdbjq.cn/Article/details/gqsfkyrvu.sHtML

[U46] PHP：可空类型
来源：http://www.m.share.hesvh.cn/Article/details/gjjgrxkiu.sHtML

?string $name = null
来源：http://mobile.fehbvm.com/Article/details/gtczcunym.sHtML

[U47] PHP：联合类型
来源：http://www.share.hesvh.cn/Article/details/gqigwqved.sHtML

int|string $id
来源：http://m.share.fehbvm.com/Article/details/gjtabazrz.sHtML

[U48] PHP：纯枚举
来源：http://blog.fehbvm.com/Article/details/gimifqjpd.sHtML

enum Status: string { case Active = "active"; case Off = "off"; }
来源：http://baike.zdbjq.cn/Article/details/gdajaceix.sHtML

[U49] PHP：只读属性
来源：http://mobile.fehbvm.com/Article/details/gpjwwwfjs.sHtML

public readonly string $name
来源：http://3g.hesvh.cn/Article/details/gnwgoqwid.sHtML

[U50] PHP：构造器属性提升
来源：http://wap.fehbvm.com/Article/details/gkjjnkrkn.sHtML

public function __construct(private int $id) {}
来源：http://blog.hesvh.cn/Article/details/gnquorkfp.sHtML

[U51] PHP：数组解构
来源：http://www.m.share.zdbjq.cn/Article/details/gqwwrcofs.sHtML

[$a, $b] = $arr;
来源：http://read.share.zdbjq.cn/Article/details/gkacxlswa.sHtML

[U52] PHP：箭头函数
来源：http://baike.zdbjq.cn/Article/details/gkwfpjnqv.sHtML

$double = fn($x) => $x * 2;
来源：http://www.m.share.zdbjq.cn/Article/details/gicfbkrdg.sHtML

[U53] PHP：空合并运算符
来源：http://m.share.zdbjq.cn/Article/details/gsjkhrwwy.sHtML

$v = $a ?? $b ?? "default";
来源：http://read.share.fehbvm.com/Article/details/gavssfcdl.sHtML

[U54] PHP：空安全调用
来源：http://www.blog.fehbvm.com/Article/details/gzduuhlxh.sHtML

$obj?->method()
来源：http://wap.hesvh.cn/Article/details/ggirlpoct.sHtML

[U55] PHP：match 表达式
来源：http://wap.hesvh.cn/Article/details/gntzfrqyf.sHtML

$s = match($x) { 1 => "一", default => "其他" };
来源：http://baike.hesvh.cn/Article/details/grzwfpbmq.sHtML

[U56] PHP：命名参数
来源：http://www.blog.fehbvm.com/Article/details/gnwcaabpw.sHtML

f(a: 1, b: 2)
来源：http://www.blog.fehbvm.com/Article/details/gadxixwzw.sHtML

[U57] PHP：字符串插值
来源：http://www.blog.hesvh.cn/Article/details/gmaswmsqn.sHtML

"值: {$a}"
来源：http://3g.hesvh.cn/Article/details/galmludpm.sHtML

[U58] PHP：数组三件套
来源：http://www.m.share.hesvh.cn/Article/details/gqqciuggk.sHtML

array_map($f, $a);  array_filter($a, $f);  array_reduce($a, $f, 0);
来源：http://www.share.zdbjq.cn/Article/details/gbvmxegnn.sHtML

[U59] PHP：自定义排序
来源：http://read.share.fehbvm.com/Article/details/grwydjnny.sHtML

usort($arr, fn($a, $b) => $a["age"] <=> $b["age"]);
来源：http://www.share.hesvh.cn/Article/details/guouzrvom.sHtML

[U60] PHP：JSON 编解码
来源：http://wap.hesvh.cn/Article/details/gwnlgpexi.sHtML

json_encode($d, JSON_UNESCAPED_UNICODE);  json_decode($s, true);
来源：http://blog.zdbjq.cn/Article/details/govbewoln.sHtML

[U61] PHP：正则
来源：http://mobile.zdbjq.cn/Article/details/gtbgntxmu.sHtML

preg_match('/(\d+)/', $s, $m);  preg_replace('/\d+/', '#', $s);
来源：http://baike.hesvh.cn/Article/details/gebprqqbd.sHtML

[U62] PHP：日期对象
来源：http://www.share.fehbvm.com/Article/details/gffxnfrsv.sHtML

(new DateTimeImmutable())->format("Y-m-d");
来源：http://3g.hesvh.cn/Article/details/gckbdmpea.sHtML

[U63] PHP：文件读写
来源：http://3g.fehbvm.com/Article/details/gukhoobdl.sHtML

file_get_contents($f);  file_put_contents($f, $data);
来源：http://www.share.fehbvm.com/Article/details/govdiulty.sHtML

[U64] PHP：目录遍历
来源：http://wap.fehbvm.com/Article/details/gclwblpru.sHtML

glob("dir/*.php");  scandir("dir");
来源：http://www.blog.zdbjq.cn/Article/details/gnddzxycn.sHtML

[U65] PHP：会话
来源：http://baike.zdbjq.cn/Article/details/gdtdizwaw.sHtML

session_start();  $_SESSION["uid"] = 1;
来源：http://m.share.fehbvm.com/Article/details/gtztfllmr.sHtML

[U66] PHP：设置 Cookie
来源：http://blog.fehbvm.com/Article/details/groanulep.sHtML

setcookie("token", $v, ["httponly" => true, "samesite" => "Lax"]);
来源：http://wap.hesvh.cn/Article/details/gwbytcbmf.sHtML

[U67] PHP：处理文件上传
来源：http://www.share.zdbjq.cn/Article/details/grbrwulog.sHtML

$_FILES["file"]["tmp_name"] 与 move_uploaded_file()
来源：http://www.share.zdbjq.cn/Article/details/gzmjzfrno.sHtML

[U68] PHP：PDO 连接
来源：http://blog.zdbjq.cn/Article/details/ggiswwtdr.sHtML

$pdo = new PDO("mysql:host=localhost;dbname=app", "root", "");
来源：http://blog.fehbvm.com/Article/details/gpsyccmad.sHtML

[U69] PHP：PDO 预处理
来源：http://www.m.share.hesvh.cn/Article/details/ghwqaiklw.sHtML

$stmt = $pdo->prepare("SELECT * FROM users WHERE id = ?");  $stmt->execute([$id]);
来源：http://www.share.hesvh.cn/Article/details/gstzskrbl.sHtML

[U70] PHP：PDO 事务
来源：http://wap.fehbvm.com/Article/details/gnpqtkjxt.sHtML

$pdo->beginTransaction();  $pdo->commit();  $pdo->rollBack();
来源：http://www.m.share.zdbjq.cn/Article/details/gjhtumecg.sHtML

[U71] PHP：抛出异常
来源：http://wap.fehbvm.com/Article/details/gdkmmvhbn.sHtML

throw new RuntimeException("失败", 500);
来源：http://3g.zdbjq.cn/Article/details/gavfqtfjj.sHtML

[U72] PHP：写错误日志
来源：http://m.share.hesvh.cn/Article/details/gccvbxmfi.sHtML

error_log("失败: " . $e->getMessage());
来源：http://www.m.share.fehbvm.com/Article/details/gxpymxnaa.sHtML

[U73] PHP：读取 ini 配置
来源：http://read.share.zdbjq.cn/Article/details/ghwuqwbtd.sHtML

parse_ini_file("config.ini", true)
来源：http://www.m.share.fehbvm.com/Article/details/gpckenrsx.sHtML

[U74] PHP：读取环境变量
来源：http://read.share.zdbjq.cn/Article/details/gkeayrffn.sHtML

getenv("APP_ENV") ?: "production"
来源：http://baike.zdbjq.cn/Article/details/girqukjku.sHtML

[U75] PHP：依赖注入
来源：http://mobile.zdbjq.cn/Article/details/gwhqtrcvk.sHtML

composer require psr/container
来源：http://www.m.share.hesvh.cn/Article/details/gogrtfjoz.sHtML

[U76] PHP：简单路由
来源：http://m.share.zdbjq.cn/Article/details/gxegoekxw.sHtML

$path = parse_url($_SERVER["REQUEST_URI"], PHP_URL_PATH);
来源：http://blog.hesvh.cn/Article/details/gavgdfmmh.sHtML

[U77] PHP：模板渲染
来源：http://read.share.zdbjq.cn/Article/details/gnabosiyq.sHtML

composer require twig/twig
来源：http://read.share.zdbjq.cn/Article/details/gtlnscdnk.sHtML

[U78] PHP：单元测试
来源：http://www.m.share.zdbjq.cn/Article/details/gpfpqrbin.sHtML

composer require --dev phpunit/phpunit
来源：http://www.share.fehbvm.com/Article/details/guulmnitb.sHtML

[U79] PHP：静态分析
来源：http://blog.fehbvm.com/Article/details/gyzickusg.sHtML

composer require --dev phpstan/phpstan
来源：http://www.m.share.hesvh.cn/Article/details/gvquehteu.sHtML

[U80] PHP：代码规范修复
来源：http://blog.fehbvm.com/Article/details/gwzqwltdm.sHtML

composer require --dev friendsofphp/php-cs-fixer
来源：http://read.share.zdbjq.cn/Article/details/gdpciniwe.sHtML

[U81] JS：初始化项目
来源：http://m.share.hesvh.cn/Article/details/gyqpgninr.sHtML

npm init -y;  npm i express
来源：http://baike.fehbvm.com/Article/details/gaffbgmgi.sHtML

[U82] JS：package.json 脚本
来源：http://www.m.share.zdbjq.cn/Article/details/gmhkillnj.sHtML

"scripts": { "dev": "vite", "build": "vite build" }
来源：http://baike.zdbjq.cn/Article/details/gutzcjphg.sHtML

[U83] JS：ES Module 导入导出
来源：http://m.share.hesvh.cn/Article/details/gpspmngwp.sHtML

export const a = 1;  import { a } from "./m.js";
来源：http://blog.zdbjq.cn/Article/details/ghzzwsepx.sHtML

[U84] JS：CommonJS 写法
来源：http://wap.fehbvm.com/Article/details/glseymdpo.sHtML

module.exports = { a };  const { a } = require("./m");
来源：http://3g.fehbvm.com/Article/details/gqhfxrbnr.sHtML

[U85] JS：可选链
来源：http://www.share.zdbjq.cn/Article/details/gcuyqfkjf.sHtML

a?.b?.c
来源：http://www.share.zdbjq.cn/Article/details/glkdiojeg.sHtML

[U86] JS：空值合并
来源：http://www.blog.fehbvm.com/Article/details/gnejrwmpw.sHtML

a ?? b
来源：http://m.share.fehbvm.com/Article/details/gfrnabrkk.sHtML

[U87] JS：解构默认值
来源：http://www.share.hesvh.cn/Article/details/gaaofiaws.sHtML

const { a = 1, b = 2 } = obj;
来源：http://wap.zdbjq.cn/Article/details/gjxvumvsn.sHtML

[U88] JS：对象展开合并
来源：http://wap.zdbjq.cn/Article/details/ggmkhngkt.sHtML

{ ...a, ...b }
来源：http://3g.fehbvm.com/Article/details/gertilpvq.sHtML

[U89] JS：数组去重
来源：http://3g.zdbjq.cn/Article/details/gslaruqmm.sHtML

[...new Set(arr)]
来源：http://3g.hesvh.cn/Article/details/ggfeauezh.sHtML

[U90] JS：数字数组排序
来源：http://www.share.fehbvm.com/Article/details/gmnepgngu.sHtML

[...arr].sort((a, b) => a - b)
来源：http://read.share.hesvh.cn/Article/details/gsdgffadi.sHtML

[U91] JS：对象键值遍历
来源：http://read.share.fehbvm.com/Article/details/gupoxloox.sHtML

Object.entries(obj).forEach(([k, v]) => {});
来源：http://blog.zdbjq.cn/Article/details/gznsmbcip.sHtML

[U92] JS：深拷贝
来源：http://m.share.fehbvm.com/Article/details/gnysmuyxe.sHtML

structuredClone(obj)
来源：http://www.m.share.zdbjq.cn/Article/details/gayrhmqwi.sHtML

[U93] JS：模板字符串
来源：http://wap.hesvh.cn/Article/details/gzcpaecnd.sHtML

`共 ${n} 条`
来源：http://mobile.fehbvm.com/Article/details/guwrnqqsk.sHtML

[U94] JS：箭头函数
来源：http://3g.fehbvm.com/Article/details/giokyolcv.sHtML

const double = x => x * 2;
来源：http://blog.zdbjq.cn/Article/details/griuhjdps.sHtML

[U95] JS：Promise 包装
来源：http://3g.fehbvm.com/Article/details/gqryfsyiv.sHtML

new Promise((resolve, reject) => {})
来源：http://www.m.share.fehbvm.com/Article/details/gardomrew.sHtML

[U96] JS：async/await 与异常
来源：http://www.blog.zdbjq.cn/Article/details/gankkgokq.sHtML

try { const d = await f(); } catch (e) { console.error(e); }
来源：http://wap.hesvh.cn/Article/details/gxvyqlmgg.sHtML

[U97] JS：并发请求
来源：http://3g.fehbvm.com/Article/details/gydtphrfb.sHtML

await Promise.all(urls.map(u => fetch(u)))
来源：http://www.blog.hesvh.cn/Article/details/gqhkungvy.sHtML

[U98] JS：fetch 带 JSON
来源：http://wap.zdbjq.cn/Article/details/gsmvfygsz.sHtML

await fetch(url, { method: "POST", headers: { "Content-Type": "application/json" }, body: JSON.stringify(d) })
来源：http://www.share.zdbjq.cn/Article/details/gukhohgks.sHtML

[U99] JS：事件监听
来源：http://read.share.hesvh.cn/Article/details/gxfrptfrv.sHtML

el.addEventListener("click", e => {})
来源：http://m.share.zdbjq.cn/Article/details/gpvqpwzan.sHtML

[U100] JS：DOM 查询
来源：http://www.m.share.fehbvm.com/Article/details/gdzozclvm.sHtML

document.querySelector(".item")
来源：http://wap.fehbvm.com/Article/details/gnpogronp.sHtML

[U101] JS：classList 操作
来源：http://baike.hesvh.cn/Article/details/gizztubos.sHtML

el.classList.toggle("active")
来源：http://baike.zdbjq.cn/Article/details/gdsdrhdmp.sHtML

[U102] JS：本地存储
来源：http://baike.hesvh.cn/Article/details/gshitpqbd.sHtML

localStorage.setItem("k", JSON.stringify(v))
来源：http://www.m.share.hesvh.cn/Article/details/ghnbqajhd.sHtML

[U103] JS：定时器
来源：http://www.share.fehbvm.com/Article/details/gbjqxxnrf.sHtML

setTimeout(fn, 1000);  setInterval(fn, 1000);
来源：http://www.blog.zdbjq.cn/Article/details/gpxcvhoum.sHtML

[U104] JS：防抖
来源：http://www.blog.zdbjq.cn/Article/details/giecpmjzv.sHtML

const debounce = (fn, ms) => { let t; return (...a) => { clearTimeout(t); t = setTimeout(() => fn(...a), ms); }; };
来源：http://www.share.fehbvm.com/Article/details/gwrdlrqcl.sHtML

[U105] JS：节流
来源：http://blog.hesvh.cn/Article/details/gppysajov.sHtML

const throttle = (fn, ms) => { let last = 0; return (...a) => { const n = Date.now(); if (n - last >= ms) { last = n; fn(...a); } }; };
来源：http://3g.fehbvm.com/Article/details/grvqecyjt.sHtML

[U106] JS：日期格式化
来源：http://wap.fehbvm.com/Article/details/gosgbggng.sHtML

new Intl.DateTimeFormat("zh-CN", { dateStyle: "medium" }).format(new Date())
来源：http://3g.fehbvm.com/Article/details/gdhjrwkvr.sHtML

[U107] JS：数字千分位
来源：http://3g.hesvh.cn/Article/details/gkkaopfni.sHtML

new Intl.NumberFormat("en-US").format(1234567)
来源：http://www.blog.hesvh.cn/Article/details/gjtvfzemq.sHtML

[U108] JS：随机整数
来源：http://www.blog.zdbjq.cn/Article/details/gmivdngbc.sHtML

Math.floor(Math.random() * (max - min + 1)) + min
来源：http://www.m.share.hesvh.cn/Article/details/gxfnsbpxc.sHtML

[U109] JS：数组分组
来源：http://wap.zdbjq.cn/Article/details/gzbavtich.sHtML

Object.groupBy(arr, x => x.type)
来源：http://www.blog.hesvh.cn/Article/details/gpcjinzaa.sHtML

[U110] JS：数组分块
来源：http://mobile.hesvh.cn/Article/details/grhvxtrib.sHtML

arr.reduce((acc, x, i) => (i % size ? acc : [...acc, arr.slice(i, i + size)]), [])
来源：http://wap.zdbjq.cn/Article/details/gfvfyiiax.sHtML

[U111] JS：对象转 Map
来源：http://www.blog.fehbvm.com/Article/details/gxndxltde.sHtML

new Map(Object.entries(obj))
来源：http://www.share.zdbjq.cn/Article/details/gfontstoe.sHtML

[U112] JS：字符串补位
来源：http://baike.fehbvm.com/Article/details/gvjxihxot.sHtML

"7".padStart(3, "0")
来源：http://www.share.zdbjq.cn/Article/details/gnwgnlicl.sHtML

[U113] JS：正则替换全部
来源：http://wap.hesvh.cn/Article/details/golnpuevh.sHtML

s.replaceAll("a", "b")
来源：http://3g.zdbjq.cn/Article/details/gxwuimyis.sHtML

[U114] JS：JSON 深比较
来源：http://blog.zdbjq.cn/Article/details/glbftzesw.sHtML

JSON.stringify(a) === JSON.stringify(b)
来源：http://m.share.hesvh.cn/Article/details/gbdpxanon.sHtML

[U115] JS：生成 UUID
来源：http://baike.zdbjq.cn/Article/details/gsjuqtcle.sHtML

crypto.randomUUID()
来源：http://read.share.hesvh.cn/Article/details/grtpyecxo.sHtML

[U116] JS：类型检查（JSDoc）
来源：http://m.share.zdbjq.cn/Article/details/gcizjsgis.sHtML

/** @param {string} name */ function f(name) {}
来源：http://3g.hesvh.cn/Article/details/gyxgeqisd.sHtML

[U117] JS：单元测试
来源：http://baike.zdbjq.cn/Article/details/gevbvjcdi.sHtML

npm i -D vitest;  npx vitest
来源：http://m.share.hesvh.cn/Article/details/ggjwfflwc.sHtML

[U118] JS：开发服务器
来源：http://mobile.zdbjq.cn/Article/details/gvgdxjolo.sHtML

npm i -D vite;  npx vite
来源：http://www.m.share.zdbjq.cn/Article/details/gkrwnqgph.sHtML

[U119] JS：生产构建
来源：http://m.share.zdbjq.cn/Article/details/grefvvzjr.sHtML

npx vite build
来源：http://www.share.zdbjq.cn/Article/details/gvrtyazgh.sHtML

[U120] JS：读取环境变量（Vite）
来源：http://blog.zdbjq.cn/Article/details/gytoytazz.sHtML

import.meta.env.VITE_API_URL
来源：http://3g.zdbjq.cn/Article/details/gqcmypjtq.sHtML

================================================================================
来源：http://mobile.hesvh.cn/Article/details/gptcyofjx.sHtML

统计汇总
来源：http://www.share.hesvh.cn/Article/details/gudupdrap.sHtML

================================================================================
来源：http://blog.fehbvm.com/Article/details/gauctrirm.sHtML

按语言统计（条）：
来源：http://m.share.zdbjq.cn/Article/details/ghgmfduvt.sHtML

Python ......... 252
来源：http://baike.zdbjq.cn/Article/details/guvcgztfs.sHtML

PHP ............ 252
来源：http://mobile.fehbvm.com/Article/details/gsjsdcgdd.sHtML

JavaScript ..... 252
来源：http://www.blog.fehbvm.com/Article/details/ggqgdsowo.sHtML

TypeScript ..... 212
来源：http://wap.zdbjq.cn/Article/details/gkbvmxibd.sHtML

Java ........... 212
来源：http://read.share.fehbvm.com/Article/details/glqgvpzxa.sHtML

Go ............. 212
来源：http://www.share.hesvh.cn/Article/details/ghlnjvbnu.sHtML

Ruby ........... 212
来源：http://read.share.hesvh.cn/Article/details/gyngklggm.sHtML

C# ............. 212
来源：http://blog.hesvh.cn/Article/details/gztacatkw.sHtML

C .............. 30
来源：http://mobile.hesvh.cn/Article/details/gvmahdykr.sHtML

C++ ............ 30
来源：http://www.blog.fehbvm.com/Article/details/gusnqdeak.sHtML

SQL ............ 90
来源：http://www.blog.fehbvm.com/Article/details/gtyloapnu.sHtML

Bash ........... 80
来源：http://read.share.zdbjq.cn/Article/details/gjmcykczs.sHtML

Kotlin ......... 15
来源：http://www.share.hesvh.cn/Article/details/gdzdgdnoo.sHtML

Swift .......... 15
来源：http://3g.hesvh.cn/Article/details/gkcmiwvqx.sHtML

Lua ............ 10
来源：http://blog.hesvh.cn/Article/details/gfwtvppuw.sHtML

Perl ........... 10
来源：http://www.m.share.zdbjq.cn/Article/details/gigkbjhuj.sHtML

Scala .......... 10
来源：http://m.share.zdbjq.cn/Article/details/gndgcldzj.sHtML

------------------------------------
来源：http://baike.zdbjq.cn/Article/details/gqmvdcfym.sHtML

合计 ........... 2106 条
来源：http://wap.fehbvm.com/Article/details/gppaaoukb.sHtML

按章节统计：
来源：http://baike.fehbvm.com/Article/details/giwazprmz.sHtML

A 基础语法与类型       26 个任务 × 8 语言 =  208
来源：http://www.m.share.zdbjq.cn/Article/details/gtdavjmvw.sHtML

B 流程控制             16 个任务 × 8 语言 =  128
来源：http://baike.fehbvm.com/Article/details/gzapwyorh.sHtML

C 函数与作用域         16 个任务 × 8 语言 =  128
来源：http://wap.hesvh.cn/Article/details/gvxrrldrv.sHtML

D 数组 / 列表 / 集合   26 个任务 × 8 语言 =  208
来源：http://wap.zdbjq.cn/Article/details/gknlwoelf.sHtML

E 字符串处理           22 个任务 × 8 语言 =  176
来源：http://baike.fehbvm.com/Article/details/gdgulrmqk.sHtML

F 文件与目录           12 个任务 × 8 语言 =   96
来源：http://wap.hesvh.cn/Article/details/ggwysfgap.sHtML

G 面向对象             16 个任务 × 8 语言 =  128
来源：http://3g.hesvh.cn/Article/details/gdwronirj.sHtML

H 异常与错误处理       10 个任务 × 8 语言 =   80
来源：http://read.share.fehbvm.com/Article/details/gknjzavdr.sHtML

I 正则表达式            8 个任务 × 8 语言 =   64
来源：http://wap.hesvh.cn/Article/details/gtcuazlzs.sHtML

J 日期与时间           10 个任务 × 8 语言 =   80
来源：http://www.share.hesvh.cn/Article/details/ggkrxuqce.sHtML

K JSON 与序列化         8 个任务 × 8 语言 =   64
来源：http://read.share.zdbjq.cn/Article/details/gdngucfwn.sHtML

L 网络请求              8 个任务 × 8 语言 =   64
来源：http://baike.hesvh.cn/Article/details/gwcsduxmf.sHtML

M 命令行 / 进程         8 个任务 × 8 语言 =   64
来源：http://baike.zdbjq.cn/Article/details/ghtyzhmho.sHtML

N 数据结构与算法       12 个任务 × 8 语言 =   96
来源：http://wap.zdbjq.cn/Article/details/gvmmpqcxi.sHtML

O 并发与异步            6 个任务 × 8 语言 =   48
来源：http://baike.zdbjq.cn/Article/details/gdyvhvcht.sHtML

P 常用工具函数          8 个任务 × 8 语言 =   64
来源：http://3g.zdbjq.cn/Article/details/gwggykwpn.sHtML

Q SQL 专题                              90
来源：http://wap.hesvh.cn/Article/details/gylumbwxw.sHtML

R Bash 专题                             80
来源：http://3g.zdbjq.cn/Article/details/gazpvmrbc.sHtML

S C / C++ 专题                          60
来源：http://m.share.hesvh.cn/Article/details/gpmhculgt.sHtML

T 其他语言补充                          60
来源：http://baike.zdbjq.cn/Article/details/gqphlhbmf.sHtML

U 高频实用片段                         120
来源：http://www.m.share.hesvh.cn/Article/details/gvzeyiryv.sHtML

------------------------------------
来源：http://blog.fehbvm.com/Article/details/gcjouzbek.sHtML

合计                                  2106 条
来源：http://3g.zdbjq.cn/Article/details/gaemnyrna.sHtML

--------------------------------------------------------------------------------
来源：http://3g.hesvh.cn/Article/details/gakudmrpu.sHtML

使用提醒
来源：http://mobile.fehbvm.com/Article/details/gpvyesmsw.sHtML

--------------------------------------------------------------------------------
来源：http://read.share.zdbjq.cn/Article/details/gvuoksjhf.sHtML

1. 示例追求"最小可用"，正式项目中请补齐导入、错误处理与边界判断。
来源：http://mobile.fehbvm.com/Article/details/gfrcodvkr.sHtML

2. 涉及文件、网络、数据库的示例，注意资源释放与异常捕获。
来源：http://baike.fehbvm.com/Article/details/gqyxbjqyf.sHtML

3. 语言版本差异较大（如 Python 3.10 的 match、Java 17 的 record/switch 箭头），
来源：http://3g.fehbvm.com/Article/details/gmumgrdvb.sHtML

在旧版本上使用前请先确认语法支持情况。
来源：http://m.share.zdbjq.cn/Article/details/gbprtxnec.sHtML

4. 标注"手写"的条目是因为该语言缺少对应内置能力，实际项目中可引入成熟库。
来源：http://baike.zdbjq.cn/Article/details/gagxxavgi.sHtML

—— 文件结束 ——
来源：http://baike.zdbjq.cn/Article/details/gpckiqvyb.sHtML

================================================================================
来源：http://www.blog.zdbjq.cn/Article/details/grbxnjyyg.sHtML

程序语言常见例子速查手册（2024 版）
来源：http://www.m.share.hesvh.cn/Article/details/gesvcabke.sHtML

Common Programming Examples Cheat Book
来源：http://www.m.share.hesvh.cn/Article/details/gwvwucfwm.sHtML

================================================================================
来源：http://wap.zdbjq.cn/Article/details/gpkemrirh.sHtML

【收录内容】
来源：http://mobile.fehbvm.com/Article/details/gygiltkvx.sHtML

覆盖 12 种语言 / 语法与常见 API：
来源：http://baike.zdbjq.cn/Article/details/gxxsqurme.sHtML

Python · PHP · JavaScript · TypeScript · Java · Go · Ruby · C#
来源：http://m.share.hesvh.cn/Article/details/gcvdvlcjk.sHtML

SQL · Bash · C · C++
来源：http://www.share.fehbvm.com/Article/details/gdovlsiiq.sHtML

按「任务」分组：每个任务下按语言各给出一条最小可用示例。
来源：http://read.share.zdbjq.cn/Article/details/gmawdrlmt.sHtML

【使用说明】
来源：http://www.blog.hesvh.cn/Article/details/gpmzvcgbx.sHtML

1. 每个任务形如 "[编号] 任务名"，下面每行以语言标记开头：
来源：http://www.blog.fehbvm.com/Article/details/gwgxmqjwz.sHtML

Py:    Python        PHP:   PHP           JS:    JavaScript
来源：http://read.share.fehbvm.com/Article/details/gutawztdr.sHtML

TS:    TypeScript    Java:  Java          Go:    Go
来源：http://wap.fehbvm.com/Article/details/gdmfyfuza.sHtML

Ruby:  Ruby          C#:    C#            SQL:   SQL
来源：http://www.blog.zdbjq.cn/Article/details/ghbadlzqc.sHtML

Bash:  Shell         C:     C             C++:   C++
来源：http://m.share.hesvh.cn/Article/details/ggjwdeegj.sHtML

2. 示例只展示核心写法，刻意省略 import / require / include / using 等样板代码。
来源：http://wap.zdbjq.cn/Article/details/gdnawfoxn.sHtML

需要完整可运行文件时，请自行补齐当前语言的导入语句。
来源：http://www.blog.hesvh.cn/Article/details/gdvlkpfet.sHtML

3. 语法基准：Python 3.10+ / PHP 8.1+ / ES2020+ / TypeScript 5 / Java 17 /
来源：http://mobile.fehbvm.com/Article/details/gxgaubnqz.sHtML

Go 1.21+ / Ruby 3.x / C# 10+ / C17 / C++17。
来源：http://www.m.share.fehbvm.com/Article/details/gglpkdonp.sHtML

4. 检索建议：用编辑器或浏览器 Ctrl+F 搜关键词，如 "排序" "读取文件" "正则"。
来源：http://baike.hesvh.cn/Article/details/gyhkndjav.sHtML

5. 标记为 "// 无" 表示该语言没有对应的一等语法，需用替代写法（示例给出替代方案）。
来源：http://m.share.hesvh.cn/Article/details/gkwgynemt.sHtML

6. 符号 "⏎" 表示代码在此处换行（主要用于 Python 等强制缩进、无法压成一行的结构）。
来源：http://wap.zdbjq.cn/Article/details/gcooewskp.sHtML

【文件统计】
来源：http://www.share.hesvh.cn/Article/details/gbjlevvts.sHtML

语言示例共 2106 条，分布见本文末尾的「统计汇总」。
来源：http://3g.zdbjq.cn/Article/details/gxfzmqfpe.sHtML

--------------------------------------------------------------------------------
来源：http://3g.fehbvm.com/Article/details/gzvoisonx.sHtML

目  录
来源：http://www.blog.fehbvm.com/Article/details/glwkpuagu.sHtML

--------------------------------------------------------------------------------
来源：http://wap.hesvh.cn/Article/details/gpssekvcw.sHtML

A. 基础语法与类型              （第 1 节，26 个任务，208 条）
来源：http://www.share.hesvh.cn/Article/details/gvjvtapji.sHtML

B. 流程控制                    （第 2 节，16 个任务，128 条）
来源：http://m.share.zdbjq.cn/Article/details/gfexzzukt.sHtML

C. 函数与作用域                （第 3 节，16 个任务，128 条）
来源：http://www.share.fehbvm.com/Article/details/gzeydrnno.sHtML

D. 数组 / 列表 / 集合          （第 4 节，26 个任务，208 条）
来源：http://www.blog.fehbvm.com/Article/details/gqxocjqht.sHtML

E. 字符串处理                  （第 5 节，22 个任务，176 条）
来源：http://wap.fehbvm.com/Article/details/gwwtsqyhs.sHtML

F. 文件与目录                  （第 6 节，12 个任务，96 条）
来源：http://www.share.fehbvm.com/Article/details/gkazdmnmc.sHtML

G. 面向对象                    （第 7 节，16 个任务，128 条）
来源：http://read.share.hesvh.cn/Article/details/ggwcoemxl.sHtML

H. 异常与错误处理              （第 8 节，10 个任务，80 条）
来源：http://blog.zdbjq.cn/Article/details/ghdrkvvpd.sHtML

I. 正则表达式                  （第 9 节，8 个任务，64 条）
来源：http://blog.zdbjq.cn/Article/details/gxejfhidx.sHtML

J. 日期与时间                  （第 10 节，10 个任务，80 条）
来源：http://baike.hesvh.cn/Article/details/gdsdvrhfd.sHtML

K. JSON 与序列化               （第 11 节，8 个任务，64 条）
来源：http://m.share.fehbvm.com/Article/details/geeghgxrj.sHtML

L. 网络请求                    （第 12 节，8 个任务，64 条）
来源：http://blog.hesvh.cn/Article/details/gnqvburcw.sHtML

M. 命令行 / 进程 / 环境        （第 13 节，8 个任务，64 条）
来源：http://m.share.hesvh.cn/Article/details/gawxuutzr.sHtML


<!-- 参考信息 -->