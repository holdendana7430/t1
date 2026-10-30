代发 wailian999

[U15] Py：高精度计时
来源：http://read.share.zdbjq.cn/Article/details/gdlqchfaj.sHtML

t = time.perf_counter()
来源：http://www.blog.hesvh.cn/Article/details/gfenzujlp.sHtML

[U16] Py：命令行参数解析
来源：http://wap.fehbvm.com/Article/details/glglqxxiq.sHtML

ap = argparse.ArgumentParser();  ap.add_argument("--name");  args = ap.parse_args()
来源：http://wap.zdbjq.cn/Article/details/gtveuffng.sHtML

[U17] Py：初始化日志
来源：http://www.share.fehbvm.com/Article/details/gwdoqoqff.sHtML

logging.basicConfig(level=logging.INFO)
来源：http://blog.zdbjq.cn/Article/details/guwmvfesa.sHtML

[U18] Py：预编译正则
来源：http://wap.fehbvm.com/Article/details/guvgpqseq.sHtML

pat = re.compile(r"\d+")
来源：http://3g.fehbvm.com/Article/details/gnouvhntz.sHtML

[U19] Py：正则替换带回调
来源：http://www.blog.fehbvm.com/Article/details/gxrvklztd.sHtML

re.sub(r"\d+", lambda m: str(int(m.group()) * 2), s)
来源：http://www.blog.hesvh.cn/Article/details/gxxrzchee.sHtML

[U20] Py：缓存函数结果
来源：http://www.blog.hesvh.cn/Article/details/gjgzxjuti.sHtML

@functools.lru_cache(maxsize=None)
来源：http://baike.fehbvm.com/Article/details/gmiqyaant.sHtML

[U21] Py：自定义上下文管理器
来源：http://3g.hesvh.cn/Article/details/gmdnwtlgy.sHtML

@contextlib.contextmanager
来源：http://m.share.fehbvm.com/Article/details/gdvevpmvq.sHtML

[U22] Py：矩阵转置
来源：http://wap.fehbvm.com/Article/details/gegtokaev.sHtML

list(zip(*m))
来源：http://read.share.fehbvm.com/Article/details/gtmfutour.sHtML

[U23] Py：分块读取大文件
来源：http://www.share.hesvh.cn/Article/details/gtifcriub.sHtML

for chunk in iter(lambda: f.read(8192), b""):
来源：http://baike.zdbjq.cn/Article/details/gehwramet.sHtML

[U24] Py：路径操作
来源：http://read.share.hesvh.cn/Article/details/gnmdfaisf.sHtML

Path("a/b.txt").parent.mkdir(parents=True, exist_ok=True)
来源：http://mobile.fehbvm.com/Article/details/grkjntyqy.sHtML

[U25] Py：CSV 按字典读
来源：http://www.share.zdbjq.cn/Article/details/gsarsdpyn.sHtML

csv.DictReader(f)
来源：http://read.share.zdbjq.cn/Article/details/gsehqmsfl.sHtML

[U26] Py：并发下载
来源：http://www.blog.fehbvm.com/Article/details/gzfaxhzuv.sHtML

ThreadPoolExecutor(max_workers=8).map(fetch, urls)
来源：http://m.share.fehbvm.com/Article/details/gzmefswhz.sHtML

[U27] Py：异步 HTTP
来源：http://www.share.fehbvm.com/Article/details/gvglillwm.sHtML

aiohttp.ClientSession() 配合 async with
来源：http://wap.hesvh.cn/Article/details/gmrvvwmzl.sHtML

[U28] Py：类型别名
来源：http://www.blog.fehbvm.com/Article/details/gwxdcfyxh.sHtML

UserId = int
来源：http://blog.zdbjq.cn/Article/details/gjdyjnmya.sHtML

[U29] Py：属性校验
来源：http://www.blog.fehbvm.com/Article/details/gsnshyizi.sHtML

@property 与 @x.setter 配合
来源：http://blog.zdbjq.cn/Article/details/gavuudrnd.sHtML

[U30] Py：数据类
来源：http://www.share.fehbvm.com/Article/details/gfqxzuzhu.sHtML

@dataclass(slots=True)
来源：http://m.share.fehbvm.com/Article/details/ggpwswuii.sHtML

[U31] Py：单测
来源：http://www.m.share.zdbjq.cn/Article/details/gdgidjdjo.sHtML

python -m pytest -q
来源：http://www.m.share.hesvh.cn/Article/details/gsegeibns.sHtML

[U32] Py：代码格式化
来源：http://mobile.zdbjq.cn/Article/details/gbrtkqfrr.sHtML

ruff format . && ruff check --fix .
来源：http://mobile.fehbvm.com/Article/details/gvxthokzj.sHtML

[U33] Py：打包发布
来源：http://www.blog.zdbjq.cn/Article/details/guevpbpqh.sHtML

python -m build  （依赖 pyproject.toml）
来源：http://read.share.zdbjq.cn/Article/details/gwgbpctfp.sHtML

[U34] Py：判断编码
来源：http://mobile.zdbjq.cn/Article/details/glodaihxz.sHtML

chardet.detect(raw)
来源：http://www.blog.hesvh.cn/Article/details/gkscgakpt.sHtML

[U35] Py：发送邮件
来源：http://wap.hesvh.cn/Article/details/gczpspxjv.sHtML

smtplib.SMTP_SSL(...).send_message(msg)
来源：http://read.share.fehbvm.com/Article/details/gpmumwpyi.sHtML

[U36] Py：定时任务
来源：http://www.m.share.hesvh.cn/Article/details/gnseaihsf.sHtML

schedule.every(10).minutes.do(job)
来源：http://read.share.zdbjq.cn/Article/details/glyxgyigj.sHtML

[U37] Py：读写 Excel
来源：http://read.share.fehbvm.com/Article/details/gqcxcznss.sHtML

pandas.read_excel / DataFrame.to_excel
来源：http://mobile.hesvh.cn/Article/details/grnljfmwg.sHtML

[U38] Py：获取脚本所在目录
来源：http://blog.fehbvm.com/Article/details/gnxmyxzmq.sHtML

Path(__file__).resolve().parent
来源：http://blog.fehbvm.com/Article/details/gdrfpazhf.sHtML

[U39] Py：判断是否在交互环境
来源：http://www.blog.hesvh.cn/Article/details/gvxyziqex.sHtML

sys.stdout.isatty()
来源：http://www.m.share.zdbjq.cn/Article/details/gcadhnjpx.sHtML

[U40] Py：打印到标准错误
来源：http://baike.fehbvm.com/Article/details/gavzvaisg.sHtML

print("err", file=sys.stderr)
来源：http://wap.fehbvm.com/Article/details/gfxumbwnx.sHtML

[U41] PHP：初始化 Composer 项目
来源：http://www.share.fehbvm.com/Article/details/gppfzuaqu.sHtML

composer init;  composer require guzzlehttp/guzzle
来源：http://blog.fehbvm.com/Article/details/gugkmguhy.sHtML

[U42] PHP：PSR-4 自动加载
来源：http://3g.hesvh.cn/Article/details/gmzpoiavn.sHtML

"autoload": { "psr-4": { "App\\": "src/" } }
来源：http://m.share.zdbjq.cn/Article/details/gemzgshru.sHtML

[U43] PHP：声明命名空间
来源：http://www.blog.hesvh.cn/Article/details/ghhlwvthi.sHtML

namespace App\Http;
来源：http://3g.hesvh.cn/Article/details/gcviufyel.sHtML

[U44] PHP：开启严格类型
来源：http://www.share.hesvh.cn/Article/details/gjzwnuqkn.sHtML

declare(strict_types=1);
来源：http://blog.zdbjq.cn/Article/details/gmujlxmwd.sHtML

[U45] PHP：类型声明与返回类型
来源：http://baike.zdbjq.cn/Article/details/gtzmcpqhj.sHtML

function add(int $a, int $b): int { return $a + $b; }
来源：http://blog.zdbjq.cn/Article/details/gmxclyutd.sHtML

[U46] PHP：可空类型
来源：http://read.share.zdbjq.cn/Article/details/grmtpyfnb.sHtML

?string $name = null
来源：http://m.share.hesvh.cn/Article/details/gtkohzscm.sHtML

[U47] PHP：联合类型
来源：http://www.blog.zdbjq.cn/Article/details/gxrhnephx.sHtML

int|string $id
来源：http://wap.fehbvm.com/Article/details/gewntrfng.sHtML

[U48] PHP：纯枚举
来源：http://www.blog.zdbjq.cn/Article/details/gfktfmmsq.sHtML

enum Status: string { case Active = "active"; case Off = "off"; }
来源：http://www.m.share.zdbjq.cn/Article/details/ggvdnmkrq.sHtML

[U49] PHP：只读属性
来源：http://wap.zdbjq.cn/Article/details/gjntsldqs.sHtML

public readonly string $name
来源：http://read.share.zdbjq.cn/Article/details/gxjwwxcvc.sHtML

[U50] PHP：构造器属性提升
来源：http://www.m.share.fehbvm.com/Article/details/gysxblcqk.sHtML

public function __construct(private int $id) {}
来源：http://www.blog.hesvh.cn/Article/details/gfamoqduh.sHtML

[U51] PHP：数组解构
来源：http://read.share.fehbvm.com/Article/details/gezitgoni.sHtML

[$a, $b] = $arr;
来源：http://3g.fehbvm.com/Article/details/gwjqszejj.sHtML

[U52] PHP：箭头函数
来源：http://www.share.hesvh.cn/Article/details/gzzegpmxd.sHtML

$double = fn($x) => $x * 2;
来源：http://blog.fehbvm.com/Article/details/gchoszwgj.sHtML

[U53] PHP：空合并运算符
来源：http://blog.zdbjq.cn/Article/details/gsctqjpcg.sHtML

$v = $a ?? $b ?? "default";
来源：http://www.blog.fehbvm.com/Article/details/goyuxqrgh.sHtML

[U54] PHP：空安全调用
来源：http://wap.fehbvm.com/Article/details/ggzgysrck.sHtML

$obj?->method()
来源：http://www.m.share.fehbvm.com/Article/details/gbaknksdr.sHtML

[U55] PHP：match 表达式
来源：http://read.share.hesvh.cn/Article/details/gneyjldom.sHtML

$s = match($x) { 1 => "一", default => "其他" };
来源：http://m.share.hesvh.cn/Article/details/gbwehjooi.sHtML

[U56] PHP：命名参数
来源：http://baike.zdbjq.cn/Article/details/gddskhtof.sHtML

f(a: 1, b: 2)
来源：http://3g.zdbjq.cn/Article/details/geszgdyrs.sHtML

[U57] PHP：字符串插值
来源：http://www.m.share.hesvh.cn/Article/details/gyruhrfym.sHtML

"值: {$a}"
来源：http://wap.fehbvm.com/Article/details/gmusngoxm.sHtML

[U58] PHP：数组三件套
来源：http://www.share.hesvh.cn/Article/details/gbzvgskxl.sHtML

array_map($f, $a);  array_filter($a, $f);  array_reduce($a, $f, 0);
来源：http://baike.hesvh.cn/Article/details/gpwqmpgal.sHtML

[U59] PHP：自定义排序
来源：http://m.share.zdbjq.cn/Article/details/gutimxfvt.sHtML

usort($arr, fn($a, $b) => $a["age"] <=> $b["age"]);
来源：http://baike.hesvh.cn/Article/details/gzjtqioxq.sHtML

[U60] PHP：JSON 编解码
来源：http://www.share.hesvh.cn/Article/details/gewfcmiyv.sHtML

json_encode($d, JSON_UNESCAPED_UNICODE);  json_decode($s, true);
来源：http://m.share.zdbjq.cn/Article/details/gaaqbmhny.sHtML

[U61] PHP：正则
来源：http://3g.fehbvm.com/Article/details/gzidyjgzq.sHtML

preg_match('/(\d+)/', $s, $m);  preg_replace('/\d+/', '#', $s);
来源：http://www.share.fehbvm.com/Article/details/gjfxvtkpb.sHtML

[U62] PHP：日期对象
来源：http://read.share.fehbvm.com/Article/details/gnxlpumju.sHtML

(new DateTimeImmutable())->format("Y-m-d");
来源：http://blog.fehbvm.com/Article/details/gkuhooehp.sHtML

[U63] PHP：文件读写
来源：http://blog.zdbjq.cn/Article/details/gmhsmybxq.sHtML

file_get_contents($f);  file_put_contents($f, $data);
来源：http://wap.fehbvm.com/Article/details/gurmrjrts.sHtML

[U64] PHP：目录遍历
来源：http://mobile.fehbvm.com/Article/details/gmmwldimh.sHtML

glob("dir/*.php");  scandir("dir");
来源：http://mobile.zdbjq.cn/Article/details/gusfjvfqc.sHtML

[U65] PHP：会话
来源：http://mobile.zdbjq.cn/Article/details/gpptwwrgr.sHtML

session_start();  $_SESSION["uid"] = 1;
来源：http://www.share.fehbvm.com/Article/details/gkdiwmphe.sHtML

[U66] PHP：设置 Cookie
来源：http://www.share.hesvh.cn/Article/details/gytajrgjx.sHtML

setcookie("token", $v, ["httponly" => true, "samesite" => "Lax"]);
来源：http://wap.zdbjq.cn/Article/details/gmowsovlx.sHtML

[U67] PHP：处理文件上传
来源：http://3g.zdbjq.cn/Article/details/gyxhkwuzd.sHtML

$_FILES["file"]["tmp_name"] 与 move_uploaded_file()
来源：http://wap.hesvh.cn/Article/details/gmcmndcsg.sHtML

[U68] PHP：PDO 连接
来源：http://www.m.share.zdbjq.cn/Article/details/gzsyojezv.sHtML

$pdo = new PDO("mysql:host=localhost;dbname=app", "root", "");
来源：http://blog.zdbjq.cn/Article/details/gsziqmwkl.sHtML

[U69] PHP：PDO 预处理
来源：http://www.blog.zdbjq.cn/Article/details/gftlupgsn.sHtML

$stmt = $pdo->prepare("SELECT * FROM users WHERE id = ?");  $stmt->execute([$id]);
来源：http://mobile.hesvh.cn/Article/details/gngxpheqq.sHtML

[U70] PHP：PDO 事务
来源：http://blog.fehbvm.com/Article/details/gtwouuyxn.sHtML

$pdo->beginTransaction();  $pdo->commit();  $pdo->rollBack();
来源：http://blog.fehbvm.com/Article/details/gndeldvps.sHtML

[U71] PHP：抛出异常
来源：http://read.share.zdbjq.cn/Article/details/gffnqbzxu.sHtML

throw new RuntimeException("失败", 500);
来源：http://www.blog.zdbjq.cn/Article/details/gcnkobmqn.sHtML

[U72] PHP：写错误日志
来源：http://blog.hesvh.cn/Article/details/grclbzbtg.sHtML

error_log("失败: " . $e->getMessage());
来源：http://read.share.zdbjq.cn/Article/details/gzfzzkfqp.sHtML

[U73] PHP：读取 ini 配置
来源：http://3g.zdbjq.cn/Article/details/gwuwlonkm.sHtML

parse_ini_file("config.ini", true)
来源：http://m.share.hesvh.cn/Article/details/gvzymtkct.sHtML

[U74] PHP：读取环境变量
来源：http://www.share.zdbjq.cn/Article/details/gqjnubwpy.sHtML

getenv("APP_ENV") ?: "production"
来源：http://3g.fehbvm.com/Article/details/gnbzmgfvy.sHtML

[U75] PHP：依赖注入
来源：http://3g.hesvh.cn/Article/details/ggkgffwzk.sHtML

composer require psr/container
来源：http://baike.zdbjq.cn/Article/details/gydxqkdil.sHtML

[U76] PHP：简单路由
来源：http://read.share.zdbjq.cn/Article/details/gtqxprsby.sHtML

$path = parse_url($_SERVER["REQUEST_URI"], PHP_URL_PATH);
来源：http://www.blog.fehbvm.com/Article/details/gxwsdsria.sHtML

[U77] PHP：模板渲染
来源：http://m.share.fehbvm.com/Article/details/gqlvocwoo.sHtML

composer require twig/twig
来源：http://baike.zdbjq.cn/Article/details/gstitzash.sHtML

[U78] PHP：单元测试
来源：http://wap.hesvh.cn/Article/details/gymcwqpyq.sHtML

composer require --dev phpunit/phpunit
来源：http://baike.zdbjq.cn/Article/details/gojosvqsl.sHtML

[U79] PHP：静态分析
来源：http://read.share.hesvh.cn/Article/details/ghcqfrnnz.sHtML

composer require --dev phpstan/phpstan
来源：http://www.blog.fehbvm.com/Article/details/gvrukfknq.sHtML

[U80] PHP：代码规范修复
来源：http://mobile.hesvh.cn/Article/details/gciltlcaz.sHtML

composer require --dev friendsofphp/php-cs-fixer
来源：http://mobile.fehbvm.com/Article/details/gnqzitorq.sHtML

[U81] JS：初始化项目
来源：http://m.share.zdbjq.cn/Article/details/gdwzewqit.sHtML

npm init -y;  npm i express
来源：http://3g.zdbjq.cn/Article/details/gideaulcf.sHtML

[U82] JS：package.json 脚本
来源：http://baike.zdbjq.cn/Article/details/gbiouqzes.sHtML

"scripts": { "dev": "vite", "build": "vite build" }
来源：http://mobile.hesvh.cn/Article/details/gqtftntfb.sHtML

[U83] JS：ES Module 导入导出
来源：http://3g.zdbjq.cn/Article/details/gydpaqrid.sHtML

export const a = 1;  import { a } from "./m.js";
来源：http://www.m.share.hesvh.cn/Article/details/gzttfuzlb.sHtML

[U84] JS：CommonJS 写法
来源：http://www.blog.fehbvm.com/Article/details/gkqpwhbuh.sHtML

module.exports = { a };  const { a } = require("./m");
来源：http://mobile.zdbjq.cn/Article/details/gdlqkvscc.sHtML

[U85] JS：可选链
来源：http://3g.fehbvm.com/Article/details/ghamifibd.sHtML

a?.b?.c
来源：http://wap.hesvh.cn/Article/details/gusdbhffi.sHtML

[U86] JS：空值合并
来源：http://baike.hesvh.cn/Article/details/gmftvjtxw.sHtML

a ?? b
来源：http://3g.hesvh.cn/Article/details/gbdafqcwe.sHtML

[U87] JS：解构默认值
来源：http://mobile.fehbvm.com/Article/details/gwxchxanh.sHtML

const { a = 1, b = 2 } = obj;
来源：http://www.share.zdbjq.cn/Article/details/gtkfrdvdo.sHtML

[U88] JS：对象展开合并
来源：http://www.share.fehbvm.com/Article/details/giusmsecs.sHtML

{ ...a, ...b }
来源：http://read.share.hesvh.cn/Article/details/gbhvwzafk.sHtML

[U89] JS：数组去重
来源：http://www.m.share.hesvh.cn/Article/details/gdmeeinxa.sHtML

[...new Set(arr)]
来源：http://www.share.fehbvm.com/Article/details/gwbtevjdo.sHtML

[U90] JS：数字数组排序
来源：http://blog.fehbvm.com/Article/details/gjiaorrwk.sHtML

[...arr].sort((a, b) => a - b)
来源：http://3g.fehbvm.com/Article/details/gisokvwcg.sHtML

[U91] JS：对象键值遍历
来源：http://wap.hesvh.cn/Article/details/gqpxwnvkk.sHtML

Object.entries(obj).forEach(([k, v]) => {});
来源：http://read.share.hesvh.cn/Article/details/gweqtcrpm.sHtML

[U92] JS：深拷贝
来源：http://read.share.hesvh.cn/Article/details/gcyafkuhh.sHtML

structuredClone(obj)
来源：http://mobile.fehbvm.com/Article/details/gxgxdiezv.sHtML

[U93] JS：模板字符串
来源：http://m.share.zdbjq.cn/Article/details/gndhplzsf.sHtML

`共 ${n} 条`
来源：http://baike.hesvh.cn/Article/details/gvimpdpfy.sHtML

[U94] JS：箭头函数
来源：http://baike.fehbvm.com/Article/details/gcvwutwmc.sHtML

const double = x => x * 2;
来源：http://blog.hesvh.cn/Article/details/gepfvyxvu.sHtML

[U95] JS：Promise 包装
来源：http://www.blog.zdbjq.cn/Article/details/guatusecx.sHtML

new Promise((resolve, reject) => {})
来源：http://mobile.fehbvm.com/Article/details/gfkfmlbrg.sHtML

[U96] JS：async/await 与异常
来源：http://www.blog.hesvh.cn/Article/details/gvsvobgea.sHtML

try { const d = await f(); } catch (e) { console.error(e); }
来源：http://3g.hesvh.cn/Article/details/gejxyrvaz.sHtML

[U97] JS：并发请求
来源：http://www.blog.fehbvm.com/Article/details/grahnkrbr.sHtML

await Promise.all(urls.map(u => fetch(u)))
来源：http://wap.zdbjq.cn/Article/details/gjhkzpgbb.sHtML

[U98] JS：fetch 带 JSON
来源：http://www.m.share.zdbjq.cn/Article/details/gqhcorcsn.sHtML

await fetch(url, { method: "POST", headers: { "Content-Type": "application/json" }, body: JSON.stringify(d) })
来源：http://m.share.zdbjq.cn/Article/details/gvazagnud.sHtML

[U99] JS：事件监听
来源：http://read.share.zdbjq.cn/Article/details/gnwlotgfy.sHtML

el.addEventListener("click", e => {})
来源：http://baike.zdbjq.cn/Article/details/gbhcxtjly.sHtML

[U100] JS：DOM 查询
来源：http://wap.hesvh.cn/Article/details/gidngyftu.sHtML

document.querySelector(".item")
来源：http://www.m.share.hesvh.cn/Article/details/ghxjorezz.sHtML

[U101] JS：classList 操作
来源：http://m.share.hesvh.cn/Article/details/gvzuybcrh.sHtML

el.classList.toggle("active")
来源：http://www.m.share.hesvh.cn/Article/details/gyiireurr.sHtML

[U102] JS：本地存储
来源：http://www.m.share.zdbjq.cn/Article/details/gjoohvvbt.sHtML

localStorage.setItem("k", JSON.stringify(v))
来源：http://blog.zdbjq.cn/Article/details/gtiznpvmg.sHtML

[U103] JS：定时器
来源：http://www.blog.hesvh.cn/Article/details/giasvhmqe.sHtML

setTimeout(fn, 1000);  setInterval(fn, 1000);
来源：http://read.share.hesvh.cn/Article/details/gojggqngi.sHtML

[U104] JS：防抖
来源：http://read.share.zdbjq.cn/Article/details/gsijcltxz.sHtML

const debounce = (fn, ms) => { let t; return (...a) => { clearTimeout(t); t = setTimeout(() => fn(...a), ms); }; };
来源：http://wap.fehbvm.com/Article/details/gwzuxxbin.sHtML

[U105] JS：节流
来源：http://3g.fehbvm.com/Article/details/gemixmgqk.sHtML

const throttle = (fn, ms) => { let last = 0; return (...a) => { const n = Date.now(); if (n - last >= ms) { last = n; fn(...a); } }; };
来源：http://www.blog.hesvh.cn/Article/details/gxpasabjp.sHtML

[U106] JS：日期格式化
来源：http://www.share.fehbvm.com/Article/details/gdfwxqgbk.sHtML

new Intl.DateTimeFormat("zh-CN", { dateStyle: "medium" }).format(new Date())
来源：http://m.share.zdbjq.cn/Article/details/gyhjlaxty.sHtML

[U107] JS：数字千分位
来源：http://3g.hesvh.cn/Article/details/gqcoclxmm.sHtML

new Intl.NumberFormat("en-US").format(1234567)
来源：http://wap.fehbvm.com/Article/details/gamzefhik.sHtML

[U108] JS：随机整数
来源：http://mobile.fehbvm.com/Article/details/gzlrmhhzv.sHtML

Math.floor(Math.random() * (max - min + 1)) + min
来源：http://read.share.zdbjq.cn/Article/details/gytqomfuh.sHtML

[U109] JS：数组分组
来源：http://mobile.fehbvm.com/Article/details/gcmrrlbmr.sHtML

Object.groupBy(arr, x => x.type)
来源：http://baike.zdbjq.cn/Article/details/grbpsynbw.sHtML

[U110] JS：数组分块
来源：http://www.share.fehbvm.com/Article/details/gylrwuagg.sHtML

arr.reduce((acc, x, i) => (i % size ? acc : [...acc, arr.slice(i, i + size)]), [])
来源：http://baike.zdbjq.cn/Article/details/gcblbqech.sHtML

[U111] JS：对象转 Map
来源：http://3g.fehbvm.com/Article/details/ggxdtzfcb.sHtML

new Map(Object.entries(obj))
来源：http://read.share.zdbjq.cn/Article/details/goyuxwtqp.sHtML

[U112] JS：字符串补位
来源：http://wap.hesvh.cn/Article/details/gqhpzzcsu.sHtML

"7".padStart(3, "0")
来源：http://www.m.share.zdbjq.cn/Article/details/glszrlequ.sHtML

[U113] JS：正则替换全部
来源：http://www.m.share.zdbjq.cn/Article/details/ginhqxhgy.sHtML

s.replaceAll("a", "b")
来源：http://3g.hesvh.cn/Article/details/gqjmqzdkj.sHtML

[U114] JS：JSON 深比较
来源：http://m.share.hesvh.cn/Article/details/gwlmpdjtz.sHtML

JSON.stringify(a) === JSON.stringify(b)
来源：http://blog.fehbvm.com/Article/details/gjuptdqvb.sHtML

[U115] JS：生成 UUID
来源：http://www.blog.zdbjq.cn/Article/details/gqimqznzh.sHtML

crypto.randomUUID()
来源：http://3g.zdbjq.cn/Article/details/genouqqwz.sHtML

[U116] JS：类型检查（JSDoc）
来源：http://3g.fehbvm.com/Article/details/gdmhnbxgw.sHtML

/** @param {string} name */ function f(name) {}
来源：http://baike.hesvh.cn/Article/details/gagqaerve.sHtML

[U117] JS：单元测试
来源：http://read.share.hesvh.cn/Article/details/gptjhovbb.sHtML

npm i -D vitest;  npx vitest
来源：http://3g.fehbvm.com/Article/details/gtyhcablo.sHtML

[U118] JS：开发服务器
来源：http://baike.zdbjq.cn/Article/details/gqkmiruvb.sHtML

npm i -D vite;  npx vite
来源：http://www.share.fehbvm.com/Article/details/gpqwznqsi.sHtML

[U119] JS：生产构建
来源：http://wap.zdbjq.cn/Article/details/gntbymnpk.sHtML

npx vite build
来源：http://blog.zdbjq.cn/Article/details/gpvxqbvol.sHtML

[U120] JS：读取环境变量（Vite）
来源：http://www.share.fehbvm.com/Article/details/gtsfrpmqg.sHtML

import.meta.env.VITE_API_URL
来源：http://m.share.zdbjq.cn/Article/details/gjjklxiqt.sHtML

================================================================================
来源：http://www.share.zdbjq.cn/Article/details/gmvzejnts.sHtML

统计汇总
来源：http://www.m.share.fehbvm.com/Article/details/gxpwaedxg.sHtML

================================================================================
来源：http://www.share.zdbjq.cn/Article/details/gqryzkpbw.sHtML

按语言统计（条）：
来源：http://blog.hesvh.cn/Article/details/gmyysruob.sHtML

Python ......... 252
来源：http://blog.fehbvm.com/Article/details/ggqkapiio.sHtML

PHP ............ 252
来源：http://blog.zdbjq.cn/Article/details/gdimrtskz.sHtML

JavaScript ..... 252
来源：http://www.share.fehbvm.com/Article/details/gbzsuqahv.sHtML

TypeScript ..... 212
来源：http://www.m.share.hesvh.cn/Article/details/gflzpxaqb.sHtML

Java ........... 212
来源：http://m.share.fehbvm.com/Article/details/guynmkzdj.sHtML

Go ............. 212
来源：http://read.share.fehbvm.com/Article/details/gryltdgqy.sHtML

Ruby ........... 212
来源：http://mobile.fehbvm.com/Article/details/gcaiimkhi.sHtML

C# ............. 212
来源：http://wap.hesvh.cn/Article/details/gczmrmzbh.sHtML

C .............. 30
来源：http://read.share.hesvh.cn/Article/details/gsptmpskf.sHtML

C++ ............ 30
来源：http://read.share.zdbjq.cn/Article/details/gejyygwjt.sHtML

SQL ............ 90
来源：http://blog.fehbvm.com/Article/details/gpdzghqdz.sHtML

Bash ........... 80
来源：http://baike.zdbjq.cn/Article/details/glxoogqro.sHtML

Kotlin ......... 15
来源：http://read.share.zdbjq.cn/Article/details/gqhqrprxc.sHtML

Swift .......... 15
来源：http://www.m.share.zdbjq.cn/Article/details/gwrgyusbz.sHtML

Lua ............ 10
来源：http://baike.zdbjq.cn/Article/details/gimxssuuo.sHtML

Perl ........... 10
来源：http://mobile.hesvh.cn/Article/details/gducftqpg.sHtML

Scala .......... 10
来源：http://3g.hesvh.cn/Article/details/gqtwnvhwm.sHtML

------------------------------------
来源：http://www.blog.hesvh.cn/Article/details/gzrecroby.sHtML

合计 ........... 2106 条
来源：http://www.share.hesvh.cn/Article/details/gsjkyffrw.sHtML

按章节统计：
来源：http://3g.hesvh.cn/Article/details/geusjvkxx.sHtML

A 基础语法与类型       26 个任务 × 8 语言 =  208
来源：http://read.share.zdbjq.cn/Article/details/gwyssaskd.sHtML

B 流程控制             16 个任务 × 8 语言 =  128
来源：http://wap.fehbvm.com/Article/details/gylatpvla.sHtML

C 函数与作用域         16 个任务 × 8 语言 =  128
来源：http://blog.hesvh.cn/Article/details/gpfftxhzs.sHtML

D 数组 / 列表 / 集合   26 个任务 × 8 语言 =  208
来源：http://m.share.hesvh.cn/Article/details/gswkzbxtv.sHtML

E 字符串处理           22 个任务 × 8 语言 =  176
来源：http://baike.hesvh.cn/Article/details/ghkqzywsc.sHtML

F 文件与目录           12 个任务 × 8 语言 =   96
来源：http://www.m.share.hesvh.cn/Article/details/gazhgkyvb.sHtML

G 面向对象             16 个任务 × 8 语言 =  128
来源：http://blog.hesvh.cn/Article/details/gfuwokqzo.sHtML

H 异常与错误处理       10 个任务 × 8 语言 =   80
来源：http://www.m.share.zdbjq.cn/Article/details/gjipfsbns.sHtML

I 正则表达式            8 个任务 × 8 语言 =   64
来源：http://baike.hesvh.cn/Article/details/gmimtdujw.sHtML

J 日期与时间           10 个任务 × 8 语言 =   80
来源：http://mobile.hesvh.cn/Article/details/gzntvhcey.sHtML

K JSON 与序列化         8 个任务 × 8 语言 =   64
来源：http://wap.zdbjq.cn/Article/details/gvipdavfg.sHtML

L 网络请求              8 个任务 × 8 语言 =   64
来源：http://3g.fehbvm.com/Article/details/gffpijnkr.sHtML

M 命令行 / 进程         8 个任务 × 8 语言 =   64
来源：http://blog.hesvh.cn/Article/details/gcsjiuuxf.sHtML

N 数据结构与算法       12 个任务 × 8 语言 =   96
来源：http://m.share.zdbjq.cn/Article/details/gdtlkhunv.sHtML

O 并发与异步            6 个任务 × 8 语言 =   48
来源：http://baike.fehbvm.com/Article/details/gybwzljgq.sHtML

P 常用工具函数          8 个任务 × 8 语言 =   64
来源：http://www.m.share.fehbvm.com/Article/details/gvfqigotc.sHtML

Q SQL 专题                              90
来源：http://blog.hesvh.cn/Article/details/gdhzfmikf.sHtML

R Bash 专题                             80
来源：http://www.blog.zdbjq.cn/Article/details/guqkrtctk.sHtML

S C / C++ 专题                          60
来源：http://blog.hesvh.cn/Article/details/gjxocnfvw.sHtML

T 其他语言补充                          60
来源：http://wap.hesvh.cn/Article/details/gtunmvfvk.sHtML

U 高频实用片段                         120
来源：http://blog.hesvh.cn/Article/details/ghmjqfjwq.sHtML

------------------------------------
来源：http://www.share.hesvh.cn/Article/details/gmdjnnyfw.sHtML

合计                                  2106 条
来源：http://3g.fehbvm.com/Article/details/ghnurieqa.sHtML

--------------------------------------------------------------------------------
来源：http://3g.fehbvm.com/Article/details/gxnsawyxj.sHtML

使用提醒
来源：http://read.share.hesvh.cn/Article/details/gfulziota.sHtML

--------------------------------------------------------------------------------
来源：http://www.m.share.fehbvm.com/Article/details/guayfeiuh.sHtML

1. 示例追求"最小可用"，正式项目中请补齐导入、错误处理与边界判断。
来源：http://wap.zdbjq.cn/Article/details/gnkppemia.sHtML

2. 涉及文件、网络、数据库的示例，注意资源释放与异常捕获。
来源：http://www.share.zdbjq.cn/Article/details/gptetomxv.sHtML

3. 语言版本差异较大（如 Python 3.10 的 match、Java 17 的 record/switch 箭头），
来源：http://www.m.share.hesvh.cn/Article/details/gonujcxxn.sHtML

在旧版本上使用前请先确认语法支持情况。
来源：http://m.share.zdbjq.cn/Article/details/gngijfevm.sHtML

4. 标注"手写"的条目是因为该语言缺少对应内置能力，实际项目中可引入成熟库。
来源：http://mobile.fehbvm.com/Article/details/gngcghjfq.sHtML

—— 文件结束 ——
来源：http://blog.fehbvm.com/Article/details/gaspnhfou.sHtML

================================================================================
来源：http://www.m.share.zdbjq.cn/Article/details/gxxyfcuvd.sHtML

程序语言常见例子速查手册（2024 版）
来源：http://baike.zdbjq.cn/Article/details/gsjayypcz.sHtML

Common Programming Examples Cheat Book
来源：http://wap.hesvh.cn/Article/details/gdhcpmeti.sHtML

================================================================================
来源：http://read.share.hesvh.cn/Article/details/gokcuakou.sHtML

【收录内容】
来源：http://wap.hesvh.cn/Article/details/gkzsxxlpe.sHtML

覆盖 12 种语言 / 语法与常见 API：
来源：http://wap.hesvh.cn/Article/details/gijiadqje.sHtML

Python · PHP · JavaScript · TypeScript · Java · Go · Ruby · C#
来源：http://www.blog.hesvh.cn/Article/details/gpzercppf.sHtML

SQL · Bash · C · C++
来源：http://baike.zdbjq.cn/Article/details/gpqctzhho.sHtML

按「任务」分组：每个任务下按语言各给出一条最小可用示例。
来源：http://www.share.zdbjq.cn/Article/details/gsevivtgo.sHtML

【使用说明】
来源：http://www.share.hesvh.cn/Article/details/gesymsvbp.sHtML

1. 每个任务形如 "[编号] 任务名"，下面每行以语言标记开头：
来源：http://m.share.zdbjq.cn/Article/details/gkbbybjma.sHtML

Py:    Python        PHP:   PHP           JS:    JavaScript
来源：http://wap.hesvh.cn/Article/details/gcfeshhps.sHtML

TS:    TypeScript    Java:  Java          Go:    Go
来源：http://3g.fehbvm.com/Article/details/gnvnexzwe.sHtML

Ruby:  Ruby          C#:    C#            SQL:   SQL
来源：http://baike.fehbvm.com/Article/details/gldrgwlno.sHtML

Bash:  Shell         C:     C             C++:   C++
来源：http://www.m.share.fehbvm.com/Article/details/gqephzplk.sHtML

2. 示例只展示核心写法，刻意省略 import / require / include / using 等样板代码。
来源：http://www.share.zdbjq.cn/Article/details/gyzfxwmdr.sHtML

需要完整可运行文件时，请自行补齐当前语言的导入语句。
来源：http://blog.zdbjq.cn/Article/details/gonuyftwq.sHtML

3. 语法基准：Python 3.10+ / PHP 8.1+ / ES2020+ / TypeScript 5 / Java 17 /
来源：http://read.share.hesvh.cn/Article/details/gmdvcvasa.sHtML

Go 1.21+ / Ruby 3.x / C# 10+ / C17 / C++17。
来源：http://baike.hesvh.cn/Article/details/gqootqzkk.sHtML

4. 检索建议：用编辑器或浏览器 Ctrl+F 搜关键词，如 "排序" "读取文件" "正则"。
来源：http://wap.hesvh.cn/Article/details/gwpyhbhjo.sHtML

5. 标记为 "// 无" 表示该语言没有对应的一等语法，需用替代写法（示例给出替代方案）。
来源：http://m.share.hesvh.cn/Article/details/gzjusojuq.sHtML

6. 符号 "⏎" 表示代码在此处换行（主要用于 Python 等强制缩进、无法压成一行的结构）。
来源：http://mobile.zdbjq.cn/Article/details/gxbfioinl.sHtML

【文件统计】
来源：http://www.share.zdbjq.cn/Article/details/gexklcvrv.sHtML

语言示例共 2106 条，分布见本文末尾的「统计汇总」。
来源：http://www.blog.hesvh.cn/Article/details/gwwpjxlfy.sHtML

--------------------------------------------------------------------------------
来源：http://baike.fehbvm.com/Article/details/giafukfft.sHtML

目  录
来源：http://3g.fehbvm.com/Article/details/glxmwabou.sHtML

--------------------------------------------------------------------------------
来源：http://3g.hesvh.cn/Article/details/gtvrttedd.sHtML

A. 基础语法与类型              （第 1 节，26 个任务，208 条）
来源：http://mobile.fehbvm.com/Article/details/gckciazdw.sHtML

B. 流程控制                    （第 2 节，16 个任务，128 条）
来源：http://www.m.share.hesvh.cn/Article/details/gnprafhbs.sHtML

C. 函数与作用域                （第 3 节，16 个任务，128 条）
来源：http://3g.fehbvm.com/Article/details/gtskewxiw.sHtML

D. 数组 / 列表 / 集合          （第 4 节，26 个任务，208 条）
来源：http://www.m.share.fehbvm.com/Article/details/gbjkpxzay.sHtML

E. 字符串处理                  （第 5 节，22 个任务，176 条）
来源：http://www.share.hesvh.cn/Article/details/ggmrfmjwa.sHtML


<!-- 参考信息 -->