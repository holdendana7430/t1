代发 wailian999

[U19] Py：正则替换带回调
来源：http://www.m.share.hesvh.cn/Article/details/glmvrhuko.sHtML

re.sub(r"\d+", lambda m: str(int(m.group()) * 2), s)
来源：http://3g.fehbvm.com/Article/details/ggnhcpdlz.sHtML

[U20] Py：缓存函数结果
来源：http://mobile.fehbvm.com/Article/details/glovvbsah.sHtML

@functools.lru_cache(maxsize=None)
来源：http://wap.hesvh.cn/Article/details/gapnpmqze.sHtML

[U21] Py：自定义上下文管理器
来源：http://baike.fehbvm.com/Article/details/gyxzoaymp.sHtML

@contextlib.contextmanager
来源：http://www.m.share.hesvh.cn/Article/details/gvmoyqbnv.sHtML

[U22] Py：矩阵转置
来源：http://3g.hesvh.cn/Article/details/gcfrbocvh.sHtML

list(zip(*m))
来源：http://3g.fehbvm.com/Article/details/gufzmfgwb.sHtML

[U23] Py：分块读取大文件
来源：http://mobile.hesvh.cn/Article/details/grvddwmxe.sHtML

for chunk in iter(lambda: f.read(8192), b""):
来源：http://3g.zdbjq.cn/Article/details/galooxdqy.sHtML

[U24] Py：路径操作
来源：http://3g.hesvh.cn/Article/details/gbzgeaddx.sHtML

Path("a/b.txt").parent.mkdir(parents=True, exist_ok=True)
来源：http://baike.hesvh.cn/Article/details/gkllhllhi.sHtML

[U25] Py：CSV 按字典读
来源：http://blog.hesvh.cn/Article/details/gfpfwuqvq.sHtML

csv.DictReader(f)
来源：http://m.share.hesvh.cn/Article/details/gazzukigk.sHtML

[U26] Py：并发下载
来源：http://www.blog.zdbjq.cn/Article/details/ghwdvavxs.sHtML

ThreadPoolExecutor(max_workers=8).map(fetch, urls)
来源：http://mobile.fehbvm.com/Article/details/gtedvurhj.sHtML

[U27] Py：异步 HTTP
来源：http://baike.hesvh.cn/Article/details/gkfobbkur.sHtML

aiohttp.ClientSession() 配合 async with
来源：http://www.share.hesvh.cn/Article/details/gbsodxfkk.sHtML

[U28] Py：类型别名
来源：http://www.share.zdbjq.cn/Article/details/gkbklxmms.sHtML

UserId = int
来源：http://wap.fehbvm.com/Article/details/glbgfwiky.sHtML

[U29] Py：属性校验
来源：http://mobile.fehbvm.com/Article/details/goukdchvp.sHtML

@property 与 @x.setter 配合
来源：http://www.m.share.hesvh.cn/Article/details/glgvcbgtm.sHtML

[U30] Py：数据类
来源：http://3g.fehbvm.com/Article/details/gvtkpjgli.sHtML

@dataclass(slots=True)
来源：http://baike.fehbvm.com/Article/details/gzrzlbyit.sHtML

[U31] Py：单测
来源：http://www.share.zdbjq.cn/Article/details/geqnaqlsi.sHtML

python -m pytest -q
来源：http://read.share.zdbjq.cn/Article/details/gzxiguptd.sHtML

[U32] Py：代码格式化
来源：http://3g.zdbjq.cn/Article/details/gxuffaqmm.sHtML

ruff format . && ruff check --fix .
来源：http://read.share.fehbvm.com/Article/details/gthitewip.sHtML

[U33] Py：打包发布
来源：http://read.share.fehbvm.com/Article/details/grnxolhar.sHtML

python -m build  （依赖 pyproject.toml）
来源：http://www.share.hesvh.cn/Article/details/goyqbkrbh.sHtML

[U34] Py：判断编码
来源：http://m.share.zdbjq.cn/Article/details/gbcsdskas.sHtML

chardet.detect(raw)
来源：http://www.share.fehbvm.com/Article/details/gnclxhcgq.sHtML

[U35] Py：发送邮件
来源：http://wap.hesvh.cn/Article/details/gtopfmjqf.sHtML

smtplib.SMTP_SSL(...).send_message(msg)
来源：http://www.share.hesvh.cn/Article/details/guahoyihs.sHtML

[U36] Py：定时任务
来源：http://blog.zdbjq.cn/Article/details/gyyvhuvvi.sHtML

schedule.every(10).minutes.do(job)
来源：http://www.blog.hesvh.cn/Article/details/gmbqtjrhh.sHtML

[U37] Py：读写 Excel
来源：http://mobile.hesvh.cn/Article/details/gfzaxildb.sHtML

pandas.read_excel / DataFrame.to_excel
来源：http://mobile.hesvh.cn/Article/details/gnbzryjhd.sHtML

[U38] Py：获取脚本所在目录
来源：http://m.share.fehbvm.com/Article/details/gznxwcrnb.sHtML

Path(__file__).resolve().parent
来源：http://mobile.fehbvm.com/Article/details/gdqoqefhq.sHtML

[U39] Py：判断是否在交互环境
来源：http://blog.zdbjq.cn/Article/details/gcojiwwgh.sHtML

sys.stdout.isatty()
来源：http://mobile.zdbjq.cn/Article/details/gurgwuudp.sHtML

[U40] Py：打印到标准错误
来源：http://www.m.share.hesvh.cn/Article/details/gjlszqgga.sHtML

print("err", file=sys.stderr)
来源：http://baike.fehbvm.com/Article/details/glrdhqinw.sHtML

[U41] PHP：初始化 Composer 项目
来源：http://read.share.zdbjq.cn/Article/details/gsdvwbqmf.sHtML

composer init;  composer require guzzlehttp/guzzle
来源：http://baike.hesvh.cn/Article/details/gtouhxwca.sHtML

[U42] PHP：PSR-4 自动加载
来源：http://3g.fehbvm.com/Article/details/gnsnxlotq.sHtML

"autoload": { "psr-4": { "App\\": "src/" } }
来源：http://mobile.zdbjq.cn/Article/details/gohkmbvcj.sHtML

[U43] PHP：声明命名空间
来源：http://baike.zdbjq.cn/Article/details/gojkwmpbl.sHtML

namespace App\Http;
来源：http://www.m.share.zdbjq.cn/Article/details/gpvsjagcv.sHtML

[U44] PHP：开启严格类型
来源：http://baike.fehbvm.com/Article/details/gjkmieuhk.sHtML

declare(strict_types=1);
来源：http://mobile.hesvh.cn/Article/details/ghsuldher.sHtML

[U45] PHP：类型声明与返回类型
来源：http://3g.hesvh.cn/Article/details/glymecpuj.sHtML

function add(int $a, int $b): int { return $a + $b; }
来源：http://blog.hesvh.cn/Article/details/gtrecblxh.sHtML

[U46] PHP：可空类型
来源：http://baike.zdbjq.cn/Article/details/grlsvxiyo.sHtML

?string $name = null
来源：http://blog.hesvh.cn/Article/details/gdloppzmt.sHtML

[U47] PHP：联合类型
来源：http://mobile.zdbjq.cn/Article/details/gwkzqdxsl.sHtML

int|string $id
来源：http://3g.hesvh.cn/Article/details/ghztgtgvk.sHtML

[U48] PHP：纯枚举
来源：http://m.share.hesvh.cn/Article/details/glseffwsu.sHtML

enum Status: string { case Active = "active"; case Off = "off"; }
来源：http://www.blog.zdbjq.cn/Article/details/gzshymraj.sHtML

[U49] PHP：只读属性
来源：http://read.share.zdbjq.cn/Article/details/glulhnddx.sHtML

public readonly string $name
来源：http://baike.hesvh.cn/Article/details/gyjtsibwt.sHtML

[U50] PHP：构造器属性提升
来源：http://read.share.hesvh.cn/Article/details/gtcoarbcu.sHtML

public function __construct(private int $id) {}
来源：http://3g.fehbvm.com/Article/details/gcqbtfspr.sHtML

[U51] PHP：数组解构
来源：http://www.share.hesvh.cn/Article/details/ghwrfqcsm.sHtML

[$a, $b] = $arr;
来源：http://3g.zdbjq.cn/Article/details/gshjcxhkp.sHtML

[U52] PHP：箭头函数
来源：http://www.m.share.zdbjq.cn/Article/details/gvtoorzme.sHtML

$double = fn($x) => $x * 2;
来源：http://mobile.zdbjq.cn/Article/details/guoolekpc.sHtML

[U53] PHP：空合并运算符
来源：http://m.share.zdbjq.cn/Article/details/gbrkigxdn.sHtML

$v = $a ?? $b ?? "default";
来源：http://wap.hesvh.cn/Article/details/gzvjdmdyf.sHtML

[U54] PHP：空安全调用
来源：http://baike.fehbvm.com/Article/details/gqdshcceq.sHtML

$obj?->method()
来源：http://www.share.fehbvm.com/Article/details/gkblbijua.sHtML

[U55] PHP：match 表达式
来源：http://baike.hesvh.cn/Article/details/gfrfabuxk.sHtML

$s = match($x) { 1 => "一", default => "其他" };
来源：http://wap.fehbvm.com/Article/details/gitalezsh.sHtML

[U56] PHP：命名参数
来源：http://read.share.hesvh.cn/Article/details/gxrbbtkgz.sHtML

f(a: 1, b: 2)
来源：http://www.blog.fehbvm.com/Article/details/gtwzgmycw.sHtML

[U57] PHP：字符串插值
来源：http://m.share.fehbvm.com/Article/details/gvsutrdle.sHtML

"值: {$a}"
来源：http://3g.hesvh.cn/Article/details/gfxuqcvug.sHtML

[U58] PHP：数组三件套
来源：http://blog.fehbvm.com/Article/details/gebbjaqrf.sHtML

array_map($f, $a);  array_filter($a, $f);  array_reduce($a, $f, 0);
来源：http://read.share.hesvh.cn/Article/details/gbuqgtqkx.sHtML

[U59] PHP：自定义排序
来源：http://blog.fehbvm.com/Article/details/ginnurkej.sHtML

usort($arr, fn($a, $b) => $a["age"] <=> $b["age"]);
来源：http://www.share.zdbjq.cn/Article/details/gxovzepzs.sHtML

[U60] PHP：JSON 编解码
来源：http://blog.fehbvm.com/Article/details/gyinfnawg.sHtML

json_encode($d, JSON_UNESCAPED_UNICODE);  json_decode($s, true);
来源：http://www.blog.zdbjq.cn/Article/details/gehlmixfl.sHtML

[U61] PHP：正则
来源：http://m.share.fehbvm.com/Article/details/giwyrggss.sHtML

preg_match('/(\d+)/', $s, $m);  preg_replace('/\d+/', '#', $s);
来源：http://wap.fehbvm.com/Article/details/ghjoqcszv.sHtML

[U62] PHP：日期对象
来源：http://blog.hesvh.cn/Article/details/gtzmxylbw.sHtML

(new DateTimeImmutable())->format("Y-m-d");
来源：http://wap.hesvh.cn/Article/details/gumomrbyp.sHtML

[U63] PHP：文件读写
来源：http://baike.fehbvm.com/Article/details/gonndpwfs.sHtML

file_get_contents($f);  file_put_contents($f, $data);
来源：http://3g.fehbvm.com/Article/details/guitahkpr.sHtML

[U64] PHP：目录遍历
来源：http://www.share.fehbvm.com/Article/details/ginifaeth.sHtML

glob("dir/*.php");  scandir("dir");
来源：http://mobile.zdbjq.cn/Article/details/gbncctnft.sHtML

[U65] PHP：会话
来源：http://www.blog.fehbvm.com/Article/details/gdbrxpafi.sHtML

session_start();  $_SESSION["uid"] = 1;
来源：http://wap.fehbvm.com/Article/details/gbiazrdcv.sHtML

[U66] PHP：设置 Cookie
来源：http://3g.fehbvm.com/Article/details/guebhmbqb.sHtML

setcookie("token", $v, ["httponly" => true, "samesite" => "Lax"]);
来源：http://3g.zdbjq.cn/Article/details/gehsffrug.sHtML

[U67] PHP：处理文件上传
来源：http://wap.hesvh.cn/Article/details/grtvdiejr.sHtML

$_FILES["file"]["tmp_name"] 与 move_uploaded_file()
来源：http://blog.fehbvm.com/Article/details/gwtbpnuqa.sHtML

[U68] PHP：PDO 连接
来源：http://www.blog.fehbvm.com/Article/details/gjbrrbppg.sHtML

$pdo = new PDO("mysql:host=localhost;dbname=app", "root", "");
来源：http://blog.zdbjq.cn/Article/details/gtljnitpk.sHtML

[U69] PHP：PDO 预处理
来源：http://3g.fehbvm.com/Article/details/giwybzdzo.sHtML

$stmt = $pdo->prepare("SELECT * FROM users WHERE id = ?");  $stmt->execute([$id]);
来源：http://blog.fehbvm.com/Article/details/gijyloaux.sHtML

[U70] PHP：PDO 事务
来源：http://www.m.share.zdbjq.cn/Article/details/gjcabwniw.sHtML

$pdo->beginTransaction();  $pdo->commit();  $pdo->rollBack();
来源：http://mobile.zdbjq.cn/Article/details/gkbsnlcdh.sHtML

[U71] PHP：抛出异常
来源：http://www.share.hesvh.cn/Article/details/ggaplwsby.sHtML

throw new RuntimeException("失败", 500);
来源：http://blog.zdbjq.cn/Article/details/gtufqsney.sHtML

[U72] PHP：写错误日志
来源：http://mobile.fehbvm.com/Article/details/gayziwtdn.sHtML

error_log("失败: " . $e->getMessage());
来源：http://blog.hesvh.cn/Article/details/goehbovrp.sHtML

[U73] PHP：读取 ini 配置
来源：http://baike.fehbvm.com/Article/details/gwuueonqk.sHtML

parse_ini_file("config.ini", true)
来源：http://www.blog.zdbjq.cn/Article/details/gxdcxbecc.sHtML

[U74] PHP：读取环境变量
来源：http://m.share.fehbvm.com/Article/details/grpgvusma.sHtML

getenv("APP_ENV") ?: "production"
来源：http://read.share.hesvh.cn/Article/details/gzhjpfazl.sHtML

[U75] PHP：依赖注入
来源：http://m.share.hesvh.cn/Article/details/gxdmywgaa.sHtML

composer require psr/container
来源：http://www.share.hesvh.cn/Article/details/gxzkvwdgp.sHtML

[U76] PHP：简单路由
来源：http://m.share.fehbvm.com/Article/details/grqxjdcrj.sHtML

$path = parse_url($_SERVER["REQUEST_URI"], PHP_URL_PATH);
来源：http://mobile.hesvh.cn/Article/details/gkukhmpse.sHtML

[U77] PHP：模板渲染
来源：http://baike.fehbvm.com/Article/details/gelrnfedf.sHtML

composer require twig/twig
来源：http://www.m.share.zdbjq.cn/Article/details/gzqxazbzg.sHtML

[U78] PHP：单元测试
来源：http://blog.zdbjq.cn/Article/details/gvmpkvwlk.sHtML

composer require --dev phpunit/phpunit
来源：http://m.share.hesvh.cn/Article/details/ggfflfscy.sHtML

[U79] PHP：静态分析
来源：http://read.share.fehbvm.com/Article/details/gsrudeqzo.sHtML

composer require --dev phpstan/phpstan
来源：http://www.share.hesvh.cn/Article/details/gzgxzwmpz.sHtML

[U80] PHP：代码规范修复
来源：http://3g.fehbvm.com/Article/details/gwgwmvudf.sHtML

composer require --dev friendsofphp/php-cs-fixer
来源：http://www.m.share.hesvh.cn/Article/details/gebvbcbqu.sHtML

[U81] JS：初始化项目
来源：http://www.blog.hesvh.cn/Article/details/gdqemcdex.sHtML

npm init -y;  npm i express
来源：http://wap.hesvh.cn/Article/details/gptxutdzc.sHtML

[U82] JS：package.json 脚本
来源：http://read.share.fehbvm.com/Article/details/gyqrosewd.sHtML

"scripts": { "dev": "vite", "build": "vite build" }
来源：http://baike.fehbvm.com/Article/details/gxrxnunxy.sHtML

[U83] JS：ES Module 导入导出
来源：http://www.blog.zdbjq.cn/Article/details/gqmcbrebx.sHtML

export const a = 1;  import { a } from "./m.js";
来源：http://www.blog.hesvh.cn/Article/details/gvvrvblbd.sHtML

[U84] JS：CommonJS 写法
来源：http://www.m.share.hesvh.cn/Article/details/gidypzrmn.sHtML

module.exports = { a };  const { a } = require("./m");
来源：http://3g.hesvh.cn/Article/details/gsaawrafz.sHtML

[U85] JS：可选链
来源：http://www.share.hesvh.cn/Article/details/gdlpxnvvr.sHtML

a?.b?.c
来源：http://www.m.share.fehbvm.com/Article/details/gjwhlabmo.sHtML

[U86] JS：空值合并
来源：http://www.m.share.zdbjq.cn/Article/details/gshgkpdka.sHtML

a ?? b
来源：http://wap.fehbvm.com/Article/details/gavxsvayn.sHtML

[U87] JS：解构默认值
来源：http://www.m.share.fehbvm.com/Article/details/gmgglbrtn.sHtML

const { a = 1, b = 2 } = obj;
来源：http://www.share.hesvh.cn/Article/details/gumdveayq.sHtML

[U88] JS：对象展开合并
来源：http://3g.zdbjq.cn/Article/details/gkijnhouh.sHtML

{ ...a, ...b }
来源：http://mobile.fehbvm.com/Article/details/geeawzfie.sHtML

[U89] JS：数组去重
来源：http://3g.zdbjq.cn/Article/details/gbqwjrnyj.sHtML

[...new Set(arr)]
来源：http://m.share.hesvh.cn/Article/details/glynbklrd.sHtML

[U90] JS：数字数组排序
来源：http://read.share.zdbjq.cn/Article/details/gcxfhnxzk.sHtML

[...arr].sort((a, b) => a - b)
来源：http://www.blog.zdbjq.cn/Article/details/gozsovrze.sHtML

[U91] JS：对象键值遍历
来源：http://3g.hesvh.cn/Article/details/gyuvqsmew.sHtML

Object.entries(obj).forEach(([k, v]) => {});
来源：http://baike.fehbvm.com/Article/details/gppyjsnvo.sHtML

[U92] JS：深拷贝
来源：http://www.blog.hesvh.cn/Article/details/ggippwkbi.sHtML

structuredClone(obj)
来源：http://www.m.share.fehbvm.com/Article/details/gtfwqclms.sHtML

[U93] JS：模板字符串
来源：http://m.share.hesvh.cn/Article/details/gvmmvwies.sHtML

`共 ${n} 条`
来源：http://wap.fehbvm.com/Article/details/ghgjgkuxb.sHtML

[U94] JS：箭头函数
来源：http://mobile.zdbjq.cn/Article/details/gkhksfidg.sHtML

const double = x => x * 2;
来源：http://www.m.share.fehbvm.com/Article/details/gyxxgobek.sHtML

[U95] JS：Promise 包装
来源：http://www.m.share.fehbvm.com/Article/details/gixuhpqqa.sHtML

new Promise((resolve, reject) => {})
来源：http://www.share.fehbvm.com/Article/details/gchhhusgv.sHtML

[U96] JS：async/await 与异常
来源：http://www.share.hesvh.cn/Article/details/gxiuhpcnx.sHtML

try { const d = await f(); } catch (e) { console.error(e); }
来源：http://blog.hesvh.cn/Article/details/gxjfndnvl.sHtML

[U97] JS：并发请求
来源：http://m.share.hesvh.cn/Article/details/gamgiasjg.sHtML

await Promise.all(urls.map(u => fetch(u)))
来源：http://read.share.fehbvm.com/Article/details/ggxkaiodw.sHtML

[U98] JS：fetch 带 JSON
来源：http://www.blog.fehbvm.com/Article/details/gllmlpipq.sHtML

await fetch(url, { method: "POST", headers: { "Content-Type": "application/json" }, body: JSON.stringify(d) })
来源：http://baike.hesvh.cn/Article/details/gzjglxvbk.sHtML

[U99] JS：事件监听
来源：http://mobile.fehbvm.com/Article/details/gkxtpoeti.sHtML

el.addEventListener("click", e => {})
来源：http://www.blog.fehbvm.com/Article/details/gniutzulk.sHtML

[U100] JS：DOM 查询
来源：http://www.share.zdbjq.cn/Article/details/gzwqxigyf.sHtML

document.querySelector(".item")
来源：http://m.share.hesvh.cn/Article/details/gaixrvqmm.sHtML

[U101] JS：classList 操作
来源：http://baike.fehbvm.com/Article/details/gqrzwvhwv.sHtML

el.classList.toggle("active")
来源：http://www.m.share.fehbvm.com/Article/details/gabtjybwy.sHtML

[U102] JS：本地存储
来源：http://blog.hesvh.cn/Article/details/gtjykzttw.sHtML

localStorage.setItem("k", JSON.stringify(v))
来源：http://read.share.zdbjq.cn/Article/details/gycfjdvmy.sHtML

[U103] JS：定时器
来源：http://mobile.fehbvm.com/Article/details/gdclhghpv.sHtML

setTimeout(fn, 1000);  setInterval(fn, 1000);
来源：http://www.blog.fehbvm.com/Article/details/gdcdnfcof.sHtML

[U104] JS：防抖
来源：http://baike.hesvh.cn/Article/details/ghljadesh.sHtML

const debounce = (fn, ms) => { let t; return (...a) => { clearTimeout(t); t = setTimeout(() => fn(...a), ms); }; };
来源：http://3g.zdbjq.cn/Article/details/gzfzvypyc.sHtML

[U105] JS：节流
来源：http://mobile.hesvh.cn/Article/details/gvqsjyxzl.sHtML

const throttle = (fn, ms) => { let last = 0; return (...a) => { const n = Date.now(); if (n - last >= ms) { last = n; fn(...a); } }; };
来源：http://wap.fehbvm.com/Article/details/gbvkovovy.sHtML

[U106] JS：日期格式化
来源：http://read.share.fehbvm.com/Article/details/gonkykydm.sHtML

new Intl.DateTimeFormat("zh-CN", { dateStyle: "medium" }).format(new Date())
来源：http://wap.zdbjq.cn/Article/details/gatwjtsxu.sHtML

[U107] JS：数字千分位
来源：http://baike.zdbjq.cn/Article/details/gctuavrqa.sHtML

new Intl.NumberFormat("en-US").format(1234567)
来源：http://blog.zdbjq.cn/Article/details/gvitwxmld.sHtML

[U108] JS：随机整数
来源：http://blog.fehbvm.com/Article/details/gocjgruae.sHtML

Math.floor(Math.random() * (max - min + 1)) + min
来源：http://baike.hesvh.cn/Article/details/gtuszqlko.sHtML

[U109] JS：数组分组
来源：http://blog.zdbjq.cn/Article/details/gxmsvujbh.sHtML

Object.groupBy(arr, x => x.type)
来源：http://read.share.fehbvm.com/Article/details/gmqdlfrvi.sHtML

[U110] JS：数组分块
来源：http://3g.hesvh.cn/Article/details/ghrgdxlsu.sHtML

arr.reduce((acc, x, i) => (i % size ? acc : [...acc, arr.slice(i, i + size)]), [])
来源：http://read.share.hesvh.cn/Article/details/gxzjzuboz.sHtML

[U111] JS：对象转 Map
来源：http://m.share.hesvh.cn/Article/details/ghpumjljs.sHtML

new Map(Object.entries(obj))
来源：http://3g.hesvh.cn/Article/details/gohrcukea.sHtML

[U112] JS：字符串补位
来源：http://3g.fehbvm.com/Article/details/gcpsabeuh.sHtML

"7".padStart(3, "0")
来源：http://blog.hesvh.cn/Article/details/gaqfvsgvk.sHtML

[U113] JS：正则替换全部
来源：http://blog.hesvh.cn/Article/details/gmfetuixe.sHtML

s.replaceAll("a", "b")
来源：http://3g.hesvh.cn/Article/details/golzvinhd.sHtML

[U114] JS：JSON 深比较
来源：http://blog.hesvh.cn/Article/details/gbwmyfteb.sHtML

JSON.stringify(a) === JSON.stringify(b)
来源：http://m.share.zdbjq.cn/Article/details/gayqxnyiu.sHtML

[U115] JS：生成 UUID
来源：http://www.blog.fehbvm.com/Article/details/gshehamkg.sHtML

crypto.randomUUID()
来源：http://m.share.fehbvm.com/Article/details/ghporwzyv.sHtML

[U116] JS：类型检查（JSDoc）
来源：http://mobile.hesvh.cn/Article/details/gzunvxvfu.sHtML

/** @param {string} name */ function f(name) {}
来源：http://blog.zdbjq.cn/Article/details/giogswptp.sHtML

[U117] JS：单元测试
来源：http://read.share.fehbvm.com/Article/details/gfmabimlh.sHtML

npm i -D vitest;  npx vitest
来源：http://www.share.zdbjq.cn/Article/details/gtadfobjg.sHtML

[U118] JS：开发服务器
来源：http://m.share.zdbjq.cn/Article/details/geocwzxzy.sHtML

npm i -D vite;  npx vite
来源：http://wap.fehbvm.com/Article/details/gkewqorlq.sHtML

[U119] JS：生产构建
来源：http://www.blog.fehbvm.com/Article/details/gimdclhyb.sHtML

npx vite build
来源：http://www.share.hesvh.cn/Article/details/gsxigwrcp.sHtML

[U120] JS：读取环境变量（Vite）
来源：http://www.blog.fehbvm.com/Article/details/ghxblizrt.sHtML

import.meta.env.VITE_API_URL
来源：http://wap.zdbjq.cn/Article/details/gzojjycaq.sHtML

================================================================================
来源：http://wap.hesvh.cn/Article/details/gtvkigqhc.sHtML

统计汇总
来源：http://3g.hesvh.cn/Article/details/gyzfoxham.sHtML

================================================================================
来源：http://m.share.hesvh.cn/Article/details/gyclxxoye.sHtML

按语言统计（条）：
来源：http://3g.fehbvm.com/Article/details/gbdkhbiyb.sHtML

Python ......... 252
来源：http://www.blog.zdbjq.cn/Article/details/gjuoihtjd.sHtML

PHP ............ 252
来源：http://www.m.share.hesvh.cn/Article/details/gafzaduuq.sHtML

JavaScript ..... 252
来源：http://m.share.hesvh.cn/Article/details/gepgskzws.sHtML

TypeScript ..... 212
来源：http://m.share.zdbjq.cn/Article/details/glalkhlvl.sHtML

Java ........... 212
来源：http://www.m.share.fehbvm.com/Article/details/ghalojieq.sHtML

Go ............. 212
来源：http://read.share.fehbvm.com/Article/details/gbamaeloh.sHtML

Ruby ........... 212
来源：http://read.share.fehbvm.com/Article/details/grpdhoyck.sHtML

C# ............. 212
来源：http://m.share.zdbjq.cn/Article/details/gmjsxqbwb.sHtML

C .............. 30
来源：http://mobile.fehbvm.com/Article/details/gexockybu.sHtML

C++ ............ 30
来源：http://blog.hesvh.cn/Article/details/gpefidbih.sHtML

SQL ............ 90
来源：http://www.m.share.hesvh.cn/Article/details/gkbmxgbxt.sHtML

Bash ........... 80
来源：http://wap.fehbvm.com/Article/details/gphuecjkb.sHtML

Kotlin ......... 15
来源：http://www.blog.zdbjq.cn/Article/details/gneysenpy.sHtML

Swift .......... 15
来源：http://3g.fehbvm.com/Article/details/gaywtgnxt.sHtML

Lua ............ 10
来源：http://m.share.hesvh.cn/Article/details/gjhqtfgsj.sHtML

Perl ........... 10
来源：http://www.m.share.hesvh.cn/Article/details/gnhwaankm.sHtML

Scala .......... 10
来源：http://mobile.zdbjq.cn/Article/details/ggzzhoozk.sHtML

------------------------------------
来源：http://www.m.share.hesvh.cn/Article/details/gyjthjhey.sHtML

合计 ........... 2106 条
来源：http://baike.fehbvm.com/Article/details/gdegfmqvn.sHtML

按章节统计：
来源：http://baike.fehbvm.com/Article/details/ghpliyzpr.sHtML

A 基础语法与类型       26 个任务 × 8 语言 =  208
来源：http://mobile.fehbvm.com/Article/details/geshwpqnj.sHtML

B 流程控制             16 个任务 × 8 语言 =  128
来源：http://wap.zdbjq.cn/Article/details/gkvjcatem.sHtML

C 函数与作用域         16 个任务 × 8 语言 =  128
来源：http://blog.zdbjq.cn/Article/details/gbeyjbxlq.sHtML

D 数组 / 列表 / 集合   26 个任务 × 8 语言 =  208
来源：http://mobile.hesvh.cn/Article/details/gxtheegcy.sHtML

E 字符串处理           22 个任务 × 8 语言 =  176
来源：http://www.share.fehbvm.com/Article/details/gnysyfnrf.sHtML

F 文件与目录           12 个任务 × 8 语言 =   96
来源：http://3g.hesvh.cn/Article/details/gadlqftti.sHtML

G 面向对象             16 个任务 × 8 语言 =  128
来源：http://wap.fehbvm.com/Article/details/gqrrgjpyy.sHtML

H 异常与错误处理       10 个任务 × 8 语言 =   80
来源：http://www.blog.hesvh.cn/Article/details/gppdkykei.sHtML

I 正则表达式            8 个任务 × 8 语言 =   64
来源：http://mobile.zdbjq.cn/Article/details/gvucnwged.sHtML

J 日期与时间           10 个任务 × 8 语言 =   80
来源：http://3g.zdbjq.cn/Article/details/gsevioniw.sHtML

K JSON 与序列化         8 个任务 × 8 语言 =   64
来源：http://baike.fehbvm.com/Article/details/gttguatlf.sHtML

L 网络请求              8 个任务 × 8 语言 =   64
来源：http://read.share.hesvh.cn/Article/details/girmswvxe.sHtML

M 命令行 / 进程         8 个任务 × 8 语言 =   64
来源：http://wap.fehbvm.com/Article/details/gpuwnvrox.sHtML

N 数据结构与算法       12 个任务 × 8 语言 =   96
来源：http://wap.fehbvm.com/Article/details/gpgjazshe.sHtML

O 并发与异步            6 个任务 × 8 语言 =   48
来源：http://mobile.fehbvm.com/Article/details/gjgtakesl.sHtML

P 常用工具函数          8 个任务 × 8 语言 =   64
来源：http://blog.zdbjq.cn/Article/details/gqjlohylf.sHtML

Q SQL 专题                              90
来源：http://mobile.fehbvm.com/Article/details/gbkcpiepb.sHtML

R Bash 专题                             80
来源：http://mobile.fehbvm.com/Article/details/gmwzhmtle.sHtML

S C / C++ 专题                          60
来源：http://www.share.fehbvm.com/Article/details/gzwtnyoex.sHtML

T 其他语言补充                          60
来源：http://wap.fehbvm.com/Article/details/goluprlqy.sHtML

U 高频实用片段                         120
来源：http://m.share.hesvh.cn/Article/details/givambjfu.sHtML

------------------------------------
来源：http://www.m.share.zdbjq.cn/Article/details/gsthkgiyl.sHtML

合计                                  2106 条
来源：http://mobile.fehbvm.com/Article/details/gfdgpgkou.sHtML

--------------------------------------------------------------------------------
来源：http://blog.zdbjq.cn/Article/details/gruhawpmt.sHtML

使用提醒
来源：http://blog.hesvh.cn/Article/details/gasibmcli.sHtML

--------------------------------------------------------------------------------
来源：http://3g.hesvh.cn/Article/details/gvtvjpgba.sHtML

1. 示例追求"最小可用"，正式项目中请补齐导入、错误处理与边界判断。
来源：http://www.share.fehbvm.com/Article/details/gzzvikppc.sHtML

2. 涉及文件、网络、数据库的示例，注意资源释放与异常捕获。
来源：http://3g.hesvh.cn/Article/details/gdelnctdk.sHtML

3. 语言版本差异较大（如 Python 3.10 的 match、Java 17 的 record/switch 箭头），
来源：http://3g.fehbvm.com/Article/details/ghpijdkfw.sHtML

在旧版本上使用前请先确认语法支持情况。
来源：http://read.share.fehbvm.com/Article/details/gysahksvu.sHtML

4. 标注"手写"的条目是因为该语言缺少对应内置能力，实际项目中可引入成熟库。
来源：http://blog.zdbjq.cn/Article/details/gdpgccakd.sHtML

—— 文件结束 ——
来源：http://blog.hesvh.cn/Article/details/gjmmngjrh.sHtML

================================================================================
来源：http://mobile.hesvh.cn/Article/details/glqdltxcs.sHtML

程序语言常见例子速查手册（2024 版）
来源：http://baike.zdbjq.cn/Article/details/grfzbsvtm.sHtML

Common Programming Examples Cheat Book
来源：http://www.m.share.fehbvm.com/Article/details/gdzmpaeub.sHtML

================================================================================
来源：http://3g.fehbvm.com/Article/details/gcslmxyyi.sHtML

【收录内容】
来源：http://m.share.zdbjq.cn/Article/details/gtmbhhwgx.sHtML

覆盖 12 种语言 / 语法与常见 API：
来源：http://blog.hesvh.cn/Article/details/gmixwwglv.sHtML

Python · PHP · JavaScript · TypeScript · Java · Go · Ruby · C#
来源：http://read.share.fehbvm.com/Article/details/ggbrqtyfp.sHtML

SQL · Bash · C · C++
来源：http://wap.fehbvm.com/Article/details/ggpwfcrio.sHtML

按「任务」分组：每个任务下按语言各给出一条最小可用示例。
来源：http://www.m.share.hesvh.cn/Article/details/gnnrsarnx.sHtML

【使用说明】
来源：http://www.share.hesvh.cn/Article/details/gcuedaqkz.sHtML

1. 每个任务形如 "[编号] 任务名"，下面每行以语言标记开头：
来源：http://m.share.fehbvm.com/Article/details/gawhqvdli.sHtML

Py:    Python        PHP:   PHP           JS:    JavaScript
来源：http://www.m.share.hesvh.cn/Article/details/gzaudkdwd.sHtML

TS:    TypeScript    Java:  Java          Go:    Go
来源：http://www.share.zdbjq.cn/Article/details/gnapnjgjv.sHtML

Ruby:  Ruby          C#:    C#            SQL:   SQL
来源：http://www.m.share.hesvh.cn/Article/details/gfpxlvwgm.sHtML

Bash:  Shell         C:     C             C++:   C++
来源：http://baike.zdbjq.cn/Article/details/gfmjlzmrb.sHtML

2. 示例只展示核心写法，刻意省略 import / require / include / using 等样板代码。
来源：http://m.share.fehbvm.com/Article/details/ghmslcqgf.sHtML

需要完整可运行文件时，请自行补齐当前语言的导入语句。
来源：http://read.share.zdbjq.cn/Article/details/gmropslxk.sHtML

3. 语法基准：Python 3.10+ / PHP 8.1+ / ES2020+ / TypeScript 5 / Java 17 /
来源：http://www.m.share.fehbvm.com/Article/details/gassoigcf.sHtML

Go 1.21+ / Ruby 3.x / C# 10+ / C17 / C++17。
来源：http://mobile.zdbjq.cn/Article/details/gqsiinvak.sHtML

4. 检索建议：用编辑器或浏览器 Ctrl+F 搜关键词，如 "排序" "读取文件" "正则"。
来源：http://www.blog.zdbjq.cn/Article/details/gldjohfjp.sHtML

5. 标记为 "// 无" 表示该语言没有对应的一等语法，需用替代写法（示例给出替代方案）。
来源：http://blog.fehbvm.com/Article/details/gyhgmcdmb.sHtML

6. 符号 "⏎" 表示代码在此处换行（主要用于 Python 等强制缩进、无法压成一行的结构）。
来源：http://wap.fehbvm.com/Article/details/gpvqqiywo.sHtML

【文件统计】
来源：http://wap.fehbvm.com/Article/details/gvisbdxvh.sHtML

语言示例共 2106 条，分布见本文末尾的「统计汇总」。
来源：http://m.share.fehbvm.com/Article/details/gzptafojo.sHtML

--------------------------------------------------------------------------------
来源：http://www.m.share.hesvh.cn/Article/details/glyasxyod.sHtML

目  录
来源：http://baike.fehbvm.com/Article/details/gcqpkpghj.sHtML

--------------------------------------------------------------------------------
来源：http://m.share.hesvh.cn/Article/details/gmaoqdmua.sHtML

A. 基础语法与类型              （第 1 节，26 个任务，208 条）
来源：http://read.share.hesvh.cn/Article/details/grukmloth.sHtML

B. 流程控制                    （第 2 节，16 个任务，128 条）
来源：http://m.share.zdbjq.cn/Article/details/geggcbdfg.sHtML

C. 函数与作用域                （第 3 节，16 个任务，128 条）
来源：http://read.share.fehbvm.com/Article/details/gmtgbpjwt.sHtML

D. 数组 / 列表 / 集合          （第 4 节，26 个任务，208 条）
来源：http://baike.fehbvm.com/Article/details/gagdzeubu.sHtML

E. 字符串处理                  （第 5 节，22 个任务，176 条）
来源：http://3g.fehbvm.com/Article/details/gjohfelcj.sHtML

F. 文件与目录                  （第 6 节，12 个任务，96 条）
来源：http://m.share.hesvh.cn/Article/details/gvsgynrdc.sHtML

G. 面向对象                    （第 7 节，16 个任务，128 条）
来源：http://blog.fehbvm.com/Article/details/gmdsjlxuf.sHtML

H. 异常与错误处理              （第 8 节，10 个任务，80 条）
来源：http://www.share.hesvh.cn/Article/details/ggaqdxtdh.sHtML

I. 正则表达式                  （第 9 节，8 个任务，64 条）
来源：http://m.share.fehbvm.com/Article/details/gogttzxlt.sHtML

J. 日期与时间                  （第 10 节，10 个任务，80 条）
来源：http://blog.hesvh.cn/Article/details/gpwnqrmek.sHtML

K. JSON 与序列化               （第 11 节，8 个任务，64 条）
来源：http://wap.fehbvm.com/Article/details/gghzmfpsx.sHtML

L. 网络请求                    （第 12 节，8 个任务，64 条）
来源：http://m.share.zdbjq.cn/Article/details/gmqqissgc.sHtML

M. 命令行 / 进程 / 环境        （第 13 节，8 个任务，64 条）
来源：http://www.share.fehbvm.com/Article/details/gumxlhlwn.sHtML


<!-- 参考信息 -->