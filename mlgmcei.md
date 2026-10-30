代发 wailian999

[U21] Py：自定义上下文管理器
来源：http://blog.hesvh.cn/Article/details/gliaifadz.sHtML

@contextlib.contextmanager
来源：http://www.m.share.hesvh.cn/Article/details/gpwxumqqy.sHtML

[U22] Py：矩阵转置
来源：http://wap.zdbjq.cn/Article/details/gxzpisjre.sHtML

list(zip(*m))
来源：http://mobile.zdbjq.cn/Article/details/gwbxisiky.sHtML

[U23] Py：分块读取大文件
来源：http://www.m.share.fehbvm.com/Article/details/gaojelsde.sHtML

for chunk in iter(lambda: f.read(8192), b""):
来源：http://read.share.fehbvm.com/Article/details/geylgepjz.sHtML

[U24] Py：路径操作
来源：http://www.blog.hesvh.cn/Article/details/grkydxddg.sHtML

Path("a/b.txt").parent.mkdir(parents=True, exist_ok=True)
来源：http://mobile.hesvh.cn/Article/details/gqxtcxsot.sHtML

[U25] Py：CSV 按字典读
来源：http://read.share.fehbvm.com/Article/details/gziwrwrhr.sHtML

csv.DictReader(f)
来源：http://read.share.hesvh.cn/Article/details/gkafgzvfn.sHtML

[U26] Py：并发下载
来源：http://www.blog.hesvh.cn/Article/details/ghcqttwge.sHtML

ThreadPoolExecutor(max_workers=8).map(fetch, urls)
来源：http://baike.hesvh.cn/Article/details/gwoqogupg.sHtML

[U27] Py：异步 HTTP
来源：http://m.share.zdbjq.cn/Article/details/giibdfopz.sHtML

aiohttp.ClientSession() 配合 async with
来源：http://blog.hesvh.cn/Article/details/gkdsxkvkj.sHtML

[U28] Py：类型别名
来源：http://www.m.share.fehbvm.com/Article/details/ghxxjmdbj.sHtML

UserId = int
来源：http://www.blog.fehbvm.com/Article/details/gcnsqsojz.sHtML

[U29] Py：属性校验
来源：http://wap.zdbjq.cn/Article/details/ghxkwzusl.sHtML

@property 与 @x.setter 配合
来源：http://www.blog.zdbjq.cn/Article/details/golubrmyq.sHtML

[U30] Py：数据类
来源：http://blog.fehbvm.com/Article/details/geykizsdz.sHtML

@dataclass(slots=True)
来源：http://wap.fehbvm.com/Article/details/gbaisjyys.sHtML

[U31] Py：单测
来源：http://wap.hesvh.cn/Article/details/ghajokvvy.sHtML

python -m pytest -q
来源：http://baike.zdbjq.cn/Article/details/gcmrsslzm.sHtML

[U32] Py：代码格式化
来源：http://mobile.fehbvm.com/Article/details/glnmwrezh.sHtML

ruff format . && ruff check --fix .
来源：http://3g.zdbjq.cn/Article/details/gbbodsuha.sHtML

[U33] Py：打包发布
来源：http://m.share.zdbjq.cn/Article/details/gnsddrfom.sHtML

python -m build  （依赖 pyproject.toml）
来源：http://m.share.fehbvm.com/Article/details/gtjxekawq.sHtML

[U34] Py：判断编码
来源：http://read.share.hesvh.cn/Article/details/gubddcuaf.sHtML

chardet.detect(raw)
来源：http://blog.hesvh.cn/Article/details/glgvzmodp.sHtML

[U35] Py：发送邮件
来源：http://www.share.zdbjq.cn/Article/details/gbvlvnkuc.sHtML

smtplib.SMTP_SSL(...).send_message(msg)
来源：http://wap.zdbjq.cn/Article/details/gncuajuik.sHtML

[U36] Py：定时任务
来源：http://mobile.fehbvm.com/Article/details/gkqagstgu.sHtML

schedule.every(10).minutes.do(job)
来源：http://www.share.fehbvm.com/Article/details/gziawcbwa.sHtML

[U37] Py：读写 Excel
来源：http://www.blog.zdbjq.cn/Article/details/gteefhnfv.sHtML

pandas.read_excel / DataFrame.to_excel
来源：http://www.blog.fehbvm.com/Article/details/gdavwalgt.sHtML

[U38] Py：获取脚本所在目录
来源：http://3g.fehbvm.com/Article/details/gsdxofcyv.sHtML

Path(__file__).resolve().parent
来源：http://baike.zdbjq.cn/Article/details/gdiewiool.sHtML

[U39] Py：判断是否在交互环境
来源：http://blog.hesvh.cn/Article/details/gxzaewsnp.sHtML

sys.stdout.isatty()
来源：http://m.share.hesvh.cn/Article/details/gnwlvyebd.sHtML

[U40] Py：打印到标准错误
来源：http://blog.zdbjq.cn/Article/details/gnjbwyqup.sHtML

print("err", file=sys.stderr)
来源：http://www.share.zdbjq.cn/Article/details/gwpjxxnai.sHtML

[U41] PHP：初始化 Composer 项目
来源：http://baike.fehbvm.com/Article/details/gnlwpyalt.sHtML

composer init;  composer require guzzlehttp/guzzle
来源：http://mobile.fehbvm.com/Article/details/galqqyfdk.sHtML

[U42] PHP：PSR-4 自动加载
来源：http://www.blog.hesvh.cn/Article/details/guljwcaxn.sHtML

"autoload": { "psr-4": { "App\\": "src/" } }
来源：http://read.share.hesvh.cn/Article/details/gaetkcnno.sHtML

[U43] PHP：声明命名空间
来源：http://mobile.fehbvm.com/Article/details/gflmjbase.sHtML

namespace App\Http;
来源：http://blog.hesvh.cn/Article/details/gklvvxmca.sHtML

[U44] PHP：开启严格类型
来源：http://www.blog.hesvh.cn/Article/details/gusclxoiq.sHtML

declare(strict_types=1);
来源：http://read.share.hesvh.cn/Article/details/gsxbelyky.sHtML

[U45] PHP：类型声明与返回类型
来源：http://www.blog.hesvh.cn/Article/details/gpctuwibu.sHtML

function add(int $a, int $b): int { return $a + $b; }
来源：http://mobile.hesvh.cn/Article/details/gieuvnawr.sHtML

[U46] PHP：可空类型
来源：http://m.share.fehbvm.com/Article/details/gpatzsvkj.sHtML

?string $name = null
来源：http://m.share.zdbjq.cn/Article/details/gsnlixibl.sHtML

[U47] PHP：联合类型
来源：http://www.blog.zdbjq.cn/Article/details/gvvogtvbv.sHtML

int|string $id
来源：http://mobile.fehbvm.com/Article/details/gmmkocffx.sHtML

[U48] PHP：纯枚举
来源：http://blog.zdbjq.cn/Article/details/gfnzgjifo.sHtML

enum Status: string { case Active = "active"; case Off = "off"; }
来源：http://3g.fehbvm.com/Article/details/gjbscrhey.sHtML

[U49] PHP：只读属性
来源：http://3g.hesvh.cn/Article/details/gmkzdexqo.sHtML

public readonly string $name
来源：http://blog.fehbvm.com/Article/details/gjrtymlnt.sHtML

[U50] PHP：构造器属性提升
来源：http://www.m.share.zdbjq.cn/Article/details/gqjyybwep.sHtML

public function __construct(private int $id) {}
来源：http://mobile.hesvh.cn/Article/details/gtczujxne.sHtML

[U51] PHP：数组解构
来源：http://mobile.hesvh.cn/Article/details/gtvmbufmg.sHtML

[$a, $b] = $arr;
来源：http://www.blog.zdbjq.cn/Article/details/gfittvhrm.sHtML

[U52] PHP：箭头函数
来源：http://wap.hesvh.cn/Article/details/gwtmixpqg.sHtML

$double = fn($x) => $x * 2;
来源：http://3g.hesvh.cn/Article/details/gmxtodcin.sHtML

[U53] PHP：空合并运算符
来源：http://mobile.zdbjq.cn/Article/details/gcxcbaqtf.sHtML

$v = $a ?? $b ?? "default";
来源：http://3g.zdbjq.cn/Article/details/gmujoayft.sHtML

[U54] PHP：空安全调用
来源：http://mobile.fehbvm.com/Article/details/gfzhgutez.sHtML

$obj?->method()
来源：http://www.share.zdbjq.cn/Article/details/gvucaxcsu.sHtML

[U55] PHP：match 表达式
来源：http://mobile.fehbvm.com/Article/details/guugufvud.sHtML

$s = match($x) { 1 => "一", default => "其他" };
来源：http://mobile.fehbvm.com/Article/details/glldmdfpt.sHtML

[U56] PHP：命名参数
来源：http://www.share.zdbjq.cn/Article/details/geymjijtr.sHtML

f(a: 1, b: 2)
来源：http://www.m.share.fehbvm.com/Article/details/geyqelajx.sHtML

[U57] PHP：字符串插值
来源：http://blog.fehbvm.com/Article/details/gfjotermo.sHtML

"值: {$a}"
来源：http://www.blog.hesvh.cn/Article/details/gicawjwme.sHtML

[U58] PHP：数组三件套
来源：http://blog.hesvh.cn/Article/details/gzmdrfjoa.sHtML

array_map($f, $a);  array_filter($a, $f);  array_reduce($a, $f, 0);
来源：http://blog.fehbvm.com/Article/details/gdmzfcgio.sHtML

[U59] PHP：自定义排序
来源：http://www.blog.hesvh.cn/Article/details/gdbqvgpdc.sHtML

usort($arr, fn($a, $b) => $a["age"] <=> $b["age"]);
来源：http://wap.zdbjq.cn/Article/details/gkvscgojl.sHtML

[U60] PHP：JSON 编解码
来源：http://baike.fehbvm.com/Article/details/gnmjtlgcs.sHtML

json_encode($d, JSON_UNESCAPED_UNICODE);  json_decode($s, true);
来源：http://mobile.fehbvm.com/Article/details/ggcotxlok.sHtML

[U61] PHP：正则
来源：http://www.share.hesvh.cn/Article/details/gqafljbzo.sHtML

preg_match('/(\d+)/', $s, $m);  preg_replace('/\d+/', '#', $s);
来源：http://mobile.fehbvm.com/Article/details/gggssbgmr.sHtML

[U62] PHP：日期对象
来源：http://read.share.hesvh.cn/Article/details/gnktkldna.sHtML

(new DateTimeImmutable())->format("Y-m-d");
来源：http://wap.zdbjq.cn/Article/details/gljtwvods.sHtML

[U63] PHP：文件读写
来源：http://mobile.zdbjq.cn/Article/details/gtpawknxw.sHtML

file_get_contents($f);  file_put_contents($f, $data);
来源：http://www.share.hesvh.cn/Article/details/gtrqjtlfo.sHtML

[U64] PHP：目录遍历
来源：http://baike.zdbjq.cn/Article/details/guevjcmhb.sHtML

glob("dir/*.php");  scandir("dir");
来源：http://baike.fehbvm.com/Article/details/gytvwajxh.sHtML

[U65] PHP：会话
来源：http://baike.zdbjq.cn/Article/details/gegaebbcy.sHtML

session_start();  $_SESSION["uid"] = 1;
来源：http://www.share.zdbjq.cn/Article/details/gvolqbdoi.sHtML

[U66] PHP：设置 Cookie
来源：http://www.m.share.hesvh.cn/Article/details/gzfgdiqjz.sHtML

setcookie("token", $v, ["httponly" => true, "samesite" => "Lax"]);
来源：http://www.m.share.fehbvm.com/Article/details/guijaikzf.sHtML

[U67] PHP：处理文件上传
来源：http://baike.fehbvm.com/Article/details/gwojerttq.sHtML

$_FILES["file"]["tmp_name"] 与 move_uploaded_file()
来源：http://www.blog.zdbjq.cn/Article/details/gufiavsrl.sHtML

[U68] PHP：PDO 连接
来源：http://www.m.share.zdbjq.cn/Article/details/gqixjgzmr.sHtML

$pdo = new PDO("mysql:host=localhost;dbname=app", "root", "");
来源：http://read.share.hesvh.cn/Article/details/gbyulvzpm.sHtML

[U69] PHP：PDO 预处理
来源：http://www.blog.hesvh.cn/Article/details/gfvkzfplj.sHtML

$stmt = $pdo->prepare("SELECT * FROM users WHERE id = ?");  $stmt->execute([$id]);
来源：http://m.share.fehbvm.com/Article/details/gtzpbhrwz.sHtML

[U70] PHP：PDO 事务
来源：http://3g.fehbvm.com/Article/details/gzgrohide.sHtML

$pdo->beginTransaction();  $pdo->commit();  $pdo->rollBack();
来源：http://mobile.fehbvm.com/Article/details/gdutzmzmt.sHtML

[U71] PHP：抛出异常
来源：http://www.blog.hesvh.cn/Article/details/gdehahaud.sHtML

throw new RuntimeException("失败", 500);
来源：http://read.share.fehbvm.com/Article/details/glzvxmbst.sHtML

[U72] PHP：写错误日志
来源：http://blog.hesvh.cn/Article/details/geczpnogi.sHtML

error_log("失败: " . $e->getMessage());
来源：http://blog.fehbvm.com/Article/details/gtevbtjkc.sHtML

[U73] PHP：读取 ini 配置
来源：http://blog.hesvh.cn/Article/details/ggvdbfssd.sHtML

parse_ini_file("config.ini", true)
来源：http://read.share.zdbjq.cn/Article/details/ghvraplvc.sHtML

[U74] PHP：读取环境变量
来源：http://3g.fehbvm.com/Article/details/gmqcqjkjs.sHtML

getenv("APP_ENV") ?: "production"
来源：http://3g.fehbvm.com/Article/details/gbgmpfjvz.sHtML

[U75] PHP：依赖注入
来源：http://baike.zdbjq.cn/Article/details/gusnafmfo.sHtML

composer require psr/container
来源：http://wap.fehbvm.com/Article/details/gcziusiqt.sHtML

[U76] PHP：简单路由
来源：http://3g.fehbvm.com/Article/details/gcamfljmk.sHtML

$path = parse_url($_SERVER["REQUEST_URI"], PHP_URL_PATH);
来源：http://mobile.zdbjq.cn/Article/details/gxoealdjd.sHtML

[U77] PHP：模板渲染
来源：http://www.blog.hesvh.cn/Article/details/gqymppekj.sHtML

composer require twig/twig
来源：http://3g.fehbvm.com/Article/details/gwffgoqov.sHtML

[U78] PHP：单元测试
来源：http://www.blog.zdbjq.cn/Article/details/gmwrldlnu.sHtML

composer require --dev phpunit/phpunit
来源：http://blog.hesvh.cn/Article/details/gdivqvpao.sHtML

[U79] PHP：静态分析
来源：http://3g.zdbjq.cn/Article/details/gycddvrry.sHtML

composer require --dev phpstan/phpstan
来源：http://read.share.zdbjq.cn/Article/details/ghjabkkyg.sHtML

[U80] PHP：代码规范修复
来源：http://blog.zdbjq.cn/Article/details/ghuxujefw.sHtML

composer require --dev friendsofphp/php-cs-fixer
来源：http://3g.fehbvm.com/Article/details/gmewovczz.sHtML

[U81] JS：初始化项目
来源：http://baike.hesvh.cn/Article/details/gzrlrpdnp.sHtML

npm init -y;  npm i express
来源：http://www.blog.zdbjq.cn/Article/details/gujisyhfv.sHtML

[U82] JS：package.json 脚本
来源：http://www.share.fehbvm.com/Article/details/gjeeqjhwg.sHtML

"scripts": { "dev": "vite", "build": "vite build" }
来源：http://www.blog.hesvh.cn/Article/details/gyftnxacv.sHtML

[U83] JS：ES Module 导入导出
来源：http://www.m.share.fehbvm.com/Article/details/ggwdrvsxe.sHtML

export const a = 1;  import { a } from "./m.js";
来源：http://www.m.share.zdbjq.cn/Article/details/gagevfqmn.sHtML

[U84] JS：CommonJS 写法
来源：http://blog.hesvh.cn/Article/details/ggllaxedg.sHtML

module.exports = { a };  const { a } = require("./m");
来源：http://m.share.hesvh.cn/Article/details/ghynwcveg.sHtML

[U85] JS：可选链
来源：http://read.share.zdbjq.cn/Article/details/goixxgutg.sHtML

a?.b?.c
来源：http://baike.fehbvm.com/Article/details/ghjfdvzgo.sHtML

[U86] JS：空值合并
来源：http://3g.fehbvm.com/Article/details/getaqxxsa.sHtML

a ?? b
来源：http://3g.zdbjq.cn/Article/details/gagwrwmmd.sHtML

[U87] JS：解构默认值
来源：http://www.m.share.hesvh.cn/Article/details/glfnlmloj.sHtML

const { a = 1, b = 2 } = obj;
来源：http://mobile.fehbvm.com/Article/details/gyxaoujws.sHtML

[U88] JS：对象展开合并
来源：http://read.share.fehbvm.com/Article/details/glslcdsij.sHtML

{ ...a, ...b }
来源：http://m.share.zdbjq.cn/Article/details/giulzdedz.sHtML

[U89] JS：数组去重
来源：http://3g.zdbjq.cn/Article/details/gtumlboua.sHtML

[...new Set(arr)]
来源：http://wap.zdbjq.cn/Article/details/ghorngvmn.sHtML

[U90] JS：数字数组排序
来源：http://3g.zdbjq.cn/Article/details/gnodzfvsw.sHtML

[...arr].sort((a, b) => a - b)
来源：http://www.m.share.zdbjq.cn/Article/details/gmxuzkizz.sHtML

[U91] JS：对象键值遍历
来源：http://baike.fehbvm.com/Article/details/gjrmmadsy.sHtML

Object.entries(obj).forEach(([k, v]) => {});
来源：http://mobile.fehbvm.com/Article/details/gwgympojk.sHtML

[U92] JS：深拷贝
来源：http://wap.zdbjq.cn/Article/details/gjlfbtoro.sHtML

structuredClone(obj)
来源：http://wap.zdbjq.cn/Article/details/gfjotgirr.sHtML

[U93] JS：模板字符串
来源：http://m.share.hesvh.cn/Article/details/gyahcuxpt.sHtML

`共 ${n} 条`
来源：http://read.share.fehbvm.com/Article/details/gukuoskcj.sHtML

[U94] JS：箭头函数
来源：http://www.share.fehbvm.com/Article/details/gafhthoho.sHtML

const double = x => x * 2;
来源：http://www.share.zdbjq.cn/Article/details/gganhqlbh.sHtML

[U95] JS：Promise 包装
来源：http://3g.fehbvm.com/Article/details/gdlcgozqw.sHtML

new Promise((resolve, reject) => {})
来源：http://wap.hesvh.cn/Article/details/gcbcmcgts.sHtML

[U96] JS：async/await 与异常
来源：http://read.share.zdbjq.cn/Article/details/gekwsgood.sHtML

try { const d = await f(); } catch (e) { console.error(e); }
来源：http://www.m.share.fehbvm.com/Article/details/gekvcfjaa.sHtML

[U97] JS：并发请求
来源：http://wap.fehbvm.com/Article/details/gqtyfbtsi.sHtML

await Promise.all(urls.map(u => fetch(u)))
来源：http://www.m.share.zdbjq.cn/Article/details/gfzizcdgn.sHtML

[U98] JS：fetch 带 JSON
来源：http://blog.zdbjq.cn/Article/details/ggolmmrgb.sHtML

await fetch(url, { method: "POST", headers: { "Content-Type": "application/json" }, body: JSON.stringify(d) })
来源：http://wap.hesvh.cn/Article/details/gczlbwigt.sHtML

[U99] JS：事件监听
来源：http://www.share.fehbvm.com/Article/details/gtmgacbpz.sHtML

el.addEventListener("click", e => {})
来源：http://read.share.hesvh.cn/Article/details/gwajuvdnu.sHtML

[U100] JS：DOM 查询
来源：http://wap.zdbjq.cn/Article/details/guuppfsgu.sHtML

document.querySelector(".item")
来源：http://www.blog.zdbjq.cn/Article/details/gmbvbzgfr.sHtML

[U101] JS：classList 操作
来源：http://www.share.hesvh.cn/Article/details/gboelhnrf.sHtML

el.classList.toggle("active")
来源：http://www.m.share.zdbjq.cn/Article/details/gmdxzkbqg.sHtML

[U102] JS：本地存储
来源：http://www.m.share.zdbjq.cn/Article/details/gztjamhgq.sHtML

localStorage.setItem("k", JSON.stringify(v))
来源：http://wap.fehbvm.com/Article/details/gssqcsxel.sHtML

[U103] JS：定时器
来源：http://m.share.fehbvm.com/Article/details/gnoikkckp.sHtML

setTimeout(fn, 1000);  setInterval(fn, 1000);
来源：http://www.blog.fehbvm.com/Article/details/gwfvpywnp.sHtML

[U104] JS：防抖
来源：http://3g.hesvh.cn/Article/details/gldkehlcj.sHtML

const debounce = (fn, ms) => { let t; return (...a) => { clearTimeout(t); t = setTimeout(() => fn(...a), ms); }; };
来源：http://read.share.hesvh.cn/Article/details/gtlswxzps.sHtML

[U105] JS：节流
来源：http://blog.zdbjq.cn/Article/details/gbeoqwhdr.sHtML

const throttle = (fn, ms) => { let last = 0; return (...a) => { const n = Date.now(); if (n - last >= ms) { last = n; fn(...a); } }; };
来源：http://www.blog.hesvh.cn/Article/details/golrzlhct.sHtML

[U106] JS：日期格式化
来源：http://m.share.zdbjq.cn/Article/details/gdurlvtpf.sHtML

new Intl.DateTimeFormat("zh-CN", { dateStyle: "medium" }).format(new Date())
来源：http://blog.hesvh.cn/Article/details/gayqrdnpm.sHtML

[U107] JS：数字千分位
来源：http://wap.zdbjq.cn/Article/details/gqsqslvuz.sHtML

new Intl.NumberFormat("en-US").format(1234567)
来源：http://www.m.share.hesvh.cn/Article/details/gansrafoy.sHtML

[U108] JS：随机整数
来源：http://read.share.zdbjq.cn/Article/details/ggblmvqnm.sHtML

Math.floor(Math.random() * (max - min + 1)) + min
来源：http://baike.fehbvm.com/Article/details/gfmrlhaap.sHtML

[U109] JS：数组分组
来源：http://m.share.hesvh.cn/Article/details/grxgcloce.sHtML

Object.groupBy(arr, x => x.type)
来源：http://blog.hesvh.cn/Article/details/gifcijmdm.sHtML

[U110] JS：数组分块
来源：http://baike.zdbjq.cn/Article/details/gncnkrczh.sHtML

arr.reduce((acc, x, i) => (i % size ? acc : [...acc, arr.slice(i, i + size)]), [])
来源：http://blog.hesvh.cn/Article/details/goouzgqdr.sHtML

[U111] JS：对象转 Map
来源：http://www.share.zdbjq.cn/Article/details/ghrtvtnzh.sHtML

new Map(Object.entries(obj))
来源：http://3g.zdbjq.cn/Article/details/gjhsbjgsk.sHtML

[U112] JS：字符串补位
来源：http://blog.zdbjq.cn/Article/details/getacodwc.sHtML

"7".padStart(3, "0")
来源：http://m.share.fehbvm.com/Article/details/gpwejmxcq.sHtML

[U113] JS：正则替换全部
来源：http://www.blog.hesvh.cn/Article/details/gdrcdlqfw.sHtML

s.replaceAll("a", "b")
来源：http://m.share.zdbjq.cn/Article/details/gqujuexax.sHtML

[U114] JS：JSON 深比较
来源：http://mobile.zdbjq.cn/Article/details/ghvlxeltw.sHtML

JSON.stringify(a) === JSON.stringify(b)
来源：http://3g.zdbjq.cn/Article/details/gwqdpmfyc.sHtML

[U115] JS：生成 UUID
来源：http://baike.fehbvm.com/Article/details/gguqpzzin.sHtML

crypto.randomUUID()
来源：http://www.blog.fehbvm.com/Article/details/geptbxxny.sHtML

[U116] JS：类型检查（JSDoc）
来源：http://3g.hesvh.cn/Article/details/gtlflyumw.sHtML

/** @param {string} name */ function f(name) {}
来源：http://blog.hesvh.cn/Article/details/gmhjwnvuu.sHtML

[U117] JS：单元测试
来源：http://wap.fehbvm.com/Article/details/gzvrmyqgg.sHtML

npm i -D vitest;  npx vitest
来源：http://www.m.share.hesvh.cn/Article/details/gozkzqdtl.sHtML

[U118] JS：开发服务器
来源：http://wap.fehbvm.com/Article/details/gzxwibejw.sHtML

npm i -D vite;  npx vite
来源：http://read.share.zdbjq.cn/Article/details/ghywttknm.sHtML

[U119] JS：生产构建
来源：http://m.share.hesvh.cn/Article/details/gvkdbaxni.sHtML

npx vite build
来源：http://blog.zdbjq.cn/Article/details/gayymuhrg.sHtML

[U120] JS：读取环境变量（Vite）
来源：http://mobile.hesvh.cn/Article/details/gijbxdtua.sHtML

import.meta.env.VITE_API_URL
来源：http://baike.zdbjq.cn/Article/details/gghrqgqri.sHtML

================================================================================
来源：http://www.share.zdbjq.cn/Article/details/gbsgmztal.sHtML

统计汇总
来源：http://3g.hesvh.cn/Article/details/grnbirsqj.sHtML

================================================================================
来源：http://mobile.zdbjq.cn/Article/details/gdbrdkico.sHtML

按语言统计（条）：
来源：http://read.share.fehbvm.com/Article/details/gmrubfewd.sHtML

Python ......... 252
来源：http://3g.hesvh.cn/Article/details/gvbnffuuc.sHtML

PHP ............ 252
来源：http://wap.hesvh.cn/Article/details/gqbfkydhe.sHtML

JavaScript ..... 252
来源：http://blog.fehbvm.com/Article/details/gfdvpmijd.sHtML

TypeScript ..... 212
来源：http://www.share.hesvh.cn/Article/details/gihkwyxmq.sHtML

Java ........... 212
来源：http://www.blog.fehbvm.com/Article/details/gtjbfjboy.sHtML

Go ............. 212
来源：http://3g.fehbvm.com/Article/details/gscjpugdu.sHtML

Ruby ........... 212
来源：http://3g.fehbvm.com/Article/details/gelmhbvyn.sHtML

C# ............. 212
来源：http://m.share.zdbjq.cn/Article/details/gekrhryzs.sHtML

C .............. 30
来源：http://www.share.zdbjq.cn/Article/details/gzpikkanb.sHtML

C++ ............ 30
来源：http://blog.fehbvm.com/Article/details/gifpphivn.sHtML

SQL ............ 90
来源：http://m.share.hesvh.cn/Article/details/gsrbezbvi.sHtML

Bash ........... 80
来源：http://baike.fehbvm.com/Article/details/gvrwxszrx.sHtML

Kotlin ......... 15
来源：http://m.share.zdbjq.cn/Article/details/gcqfrzdwo.sHtML

Swift .......... 15
来源：http://3g.fehbvm.com/Article/details/gdffeekya.sHtML

Lua ............ 10
来源：http://blog.hesvh.cn/Article/details/ghnestqmk.sHtML

Perl ........... 10
来源：http://www.share.hesvh.cn/Article/details/gezopwnev.sHtML

Scala .......... 10
来源：http://baike.hesvh.cn/Article/details/gjmdqnuak.sHtML

------------------------------------
来源：http://3g.fehbvm.com/Article/details/glwnrcdkg.sHtML

合计 ........... 2106 条
来源：http://www.blog.hesvh.cn/Article/details/gqyuiichc.sHtML

按章节统计：
来源：http://www.blog.zdbjq.cn/Article/details/gfgmfqdxf.sHtML

A 基础语法与类型       26 个任务 × 8 语言 =  208
来源：http://mobile.hesvh.cn/Article/details/glsqeipfz.sHtML

B 流程控制             16 个任务 × 8 语言 =  128
来源：http://www.m.share.hesvh.cn/Article/details/gzqywtngo.sHtML

C 函数与作用域         16 个任务 × 8 语言 =  128
来源：http://mobile.zdbjq.cn/Article/details/ghzttuopx.sHtML

D 数组 / 列表 / 集合   26 个任务 × 8 语言 =  208
来源：http://www.blog.zdbjq.cn/Article/details/gqdgllndw.sHtML

E 字符串处理           22 个任务 × 8 语言 =  176
来源：http://3g.zdbjq.cn/Article/details/gpezxeofm.sHtML

F 文件与目录           12 个任务 × 8 语言 =   96
来源：http://wap.hesvh.cn/Article/details/gvwzuyykt.sHtML

G 面向对象             16 个任务 × 8 语言 =  128
来源：http://www.share.fehbvm.com/Article/details/gojbpdpae.sHtML

H 异常与错误处理       10 个任务 × 8 语言 =   80
来源：http://read.share.zdbjq.cn/Article/details/gywzxkpej.sHtML

I 正则表达式            8 个任务 × 8 语言 =   64
来源：http://m.share.fehbvm.com/Article/details/gzlczwhis.sHtML

J 日期与时间           10 个任务 × 8 语言 =   80
来源：http://3g.fehbvm.com/Article/details/gevmtqjli.sHtML

K JSON 与序列化         8 个任务 × 8 语言 =   64
来源：http://m.share.fehbvm.com/Article/details/ghdviuqtu.sHtML

L 网络请求              8 个任务 × 8 语言 =   64
来源：http://blog.zdbjq.cn/Article/details/ggifbouyq.sHtML

M 命令行 / 进程         8 个任务 × 8 语言 =   64
来源：http://mobile.zdbjq.cn/Article/details/guiymqamg.sHtML

N 数据结构与算法       12 个任务 × 8 语言 =   96
来源：http://www.m.share.fehbvm.com/Article/details/ggjldkrgz.sHtML

O 并发与异步            6 个任务 × 8 语言 =   48
来源：http://wap.hesvh.cn/Article/details/gqebquwcm.sHtML

P 常用工具函数          8 个任务 × 8 语言 =   64
来源：http://read.share.fehbvm.com/Article/details/gdfbwstnc.sHtML

Q SQL 专题                              90
来源：http://baike.hesvh.cn/Article/details/grtbdtjuw.sHtML

R Bash 专题                             80
来源：http://www.blog.zdbjq.cn/Article/details/ggwbbysts.sHtML

S C / C++ 专题                          60
来源：http://m.share.hesvh.cn/Article/details/gvnjcvftl.sHtML

T 其他语言补充                          60
来源：http://www.blog.zdbjq.cn/Article/details/ggbnedbyt.sHtML

U 高频实用片段                         120
来源：http://m.share.zdbjq.cn/Article/details/gniypjcaj.sHtML

------------------------------------
来源：http://read.share.fehbvm.com/Article/details/gfhwsqybx.sHtML

合计                                  2106 条
来源：http://3g.fehbvm.com/Article/details/gzahkchxv.sHtML

--------------------------------------------------------------------------------
来源：http://baike.zdbjq.cn/Article/details/gunoauyke.sHtML

使用提醒
来源：http://read.share.fehbvm.com/Article/details/gipcxmmmi.sHtML

--------------------------------------------------------------------------------
来源：http://www.blog.fehbvm.com/Article/details/grwvbzlpa.sHtML

1. 示例追求"最小可用"，正式项目中请补齐导入、错误处理与边界判断。
来源：http://wap.hesvh.cn/Article/details/gvtryfvmn.sHtML

2. 涉及文件、网络、数据库的示例，注意资源释放与异常捕获。
来源：http://3g.zdbjq.cn/Article/details/gcpbyugoo.sHtML

3. 语言版本差异较大（如 Python 3.10 的 match、Java 17 的 record/switch 箭头），
来源：http://www.m.share.fehbvm.com/Article/details/gxreetghg.sHtML

在旧版本上使用前请先确认语法支持情况。
来源：http://www.blog.zdbjq.cn/Article/details/gbrryjpmb.sHtML

4. 标注"手写"的条目是因为该语言缺少对应内置能力，实际项目中可引入成熟库。
来源：http://m.share.hesvh.cn/Article/details/gzcljuuex.sHtML

—— 文件结束 ——
来源：http://blog.fehbvm.com/Article/details/gsykjxikc.sHtML

================================================================================
来源：http://blog.hesvh.cn/Article/details/gtifacean.sHtML

程序语言常见例子速查手册（2024 版）
来源：http://www.blog.hesvh.cn/Article/details/gxqftvyzm.sHtML

Common Programming Examples Cheat Book
来源：http://baike.zdbjq.cn/Article/details/gdtempyuo.sHtML

================================================================================
来源：http://blog.zdbjq.cn/Article/details/gypjglisw.sHtML

【收录内容】
来源：http://www.m.share.hesvh.cn/Article/details/gespakwdy.sHtML

覆盖 12 种语言 / 语法与常见 API：
来源：http://www.blog.fehbvm.com/Article/details/giyosyovg.sHtML

Python · PHP · JavaScript · TypeScript · Java · Go · Ruby · C#
来源：http://baike.hesvh.cn/Article/details/gjrdzyink.sHtML

SQL · Bash · C · C++
来源：http://wap.zdbjq.cn/Article/details/ggywxjptn.sHtML

按「任务」分组：每个任务下按语言各给出一条最小可用示例。
来源：http://mobile.hesvh.cn/Article/details/gnilqvxcb.sHtML

【使用说明】
来源：http://www.m.share.fehbvm.com/Article/details/gqljpczfg.sHtML

1. 每个任务形如 "[编号] 任务名"，下面每行以语言标记开头：
来源：http://www.blog.zdbjq.cn/Article/details/gwuhdxabh.sHtML

Py:    Python        PHP:   PHP           JS:    JavaScript
来源：http://wap.fehbvm.com/Article/details/gemmqirns.sHtML

TS:    TypeScript    Java:  Java          Go:    Go
来源：http://m.share.fehbvm.com/Article/details/ggvcjnqna.sHtML

Ruby:  Ruby          C#:    C#            SQL:   SQL
来源：http://blog.zdbjq.cn/Article/details/gnveyczdi.sHtML

Bash:  Shell         C:     C             C++:   C++
来源：http://3g.zdbjq.cn/Article/details/gbupczscb.sHtML

2. 示例只展示核心写法，刻意省略 import / require / include / using 等样板代码。
来源：http://m.share.zdbjq.cn/Article/details/gafzdgrch.sHtML

需要完整可运行文件时，请自行补齐当前语言的导入语句。
来源：http://3g.zdbjq.cn/Article/details/gqemcgadd.sHtML

3. 语法基准：Python 3.10+ / PHP 8.1+ / ES2020+ / TypeScript 5 / Java 17 /
来源：http://3g.zdbjq.cn/Article/details/gavosbfiz.sHtML

Go 1.21+ / Ruby 3.x / C# 10+ / C17 / C++17。
来源：http://www.share.hesvh.cn/Article/details/gnorhwpgz.sHtML

4. 检索建议：用编辑器或浏览器 Ctrl+F 搜关键词，如 "排序" "读取文件" "正则"。
来源：http://read.share.fehbvm.com/Article/details/gfnjuebwr.sHtML

5. 标记为 "// 无" 表示该语言没有对应的一等语法，需用替代写法（示例给出替代方案）。
来源：http://www.m.share.zdbjq.cn/Article/details/gblkxzngg.sHtML

6. 符号 "⏎" 表示代码在此处换行（主要用于 Python 等强制缩进、无法压成一行的结构）。
来源：http://read.share.zdbjq.cn/Article/details/gdlejjfsd.sHtML

【文件统计】
来源：http://wap.hesvh.cn/Article/details/gtkfneeih.sHtML

语言示例共 2106 条，分布见本文末尾的「统计汇总」。
来源：http://blog.hesvh.cn/Article/details/gcxbpkjwj.sHtML

--------------------------------------------------------------------------------
来源：http://3g.zdbjq.cn/Article/details/ggpwspwrh.sHtML

目  录
来源：http://www.m.share.fehbvm.com/Article/details/gbeojiwxg.sHtML

--------------------------------------------------------------------------------
来源：http://www.share.hesvh.cn/Article/details/gnoekkxgk.sHtML

A. 基础语法与类型              （第 1 节，26 个任务，208 条）
来源：http://mobile.fehbvm.com/Article/details/gfvuluoqv.sHtML

B. 流程控制                    （第 2 节，16 个任务，128 条）
来源：http://mobile.zdbjq.cn/Article/details/gwolvdvpy.sHtML

C. 函数与作用域                （第 3 节，16 个任务，128 条）
来源：http://blog.hesvh.cn/Article/details/gxmktzple.sHtML

D. 数组 / 列表 / 集合          （第 4 节，26 个任务，208 条）
来源：http://mobile.hesvh.cn/Article/details/gslossriv.sHtML

E. 字符串处理                  （第 5 节，22 个任务，176 条）
来源：http://m.share.fehbvm.com/Article/details/gjgofbyll.sHtML

F. 文件与目录                  （第 6 节，12 个任务，96 条）
来源：http://www.share.zdbjq.cn/Article/details/gszcdxkgo.sHtML

G. 面向对象                    （第 7 节，16 个任务，128 条）
来源：http://3g.zdbjq.cn/Article/details/gtmhfidwd.sHtML

H. 异常与错误处理              （第 8 节，10 个任务，80 条）
来源：http://mobile.fehbvm.com/Article/details/gldialzdq.sHtML

I. 正则表达式                  （第 9 节，8 个任务，64 条）
来源：http://read.share.hesvh.cn/Article/details/gaxspdrqz.sHtML

J. 日期与时间                  （第 10 节，10 个任务，80 条）
来源：http://baike.hesvh.cn/Article/details/gahnnqpca.sHtML

K. JSON 与序列化               （第 11 节，8 个任务，64 条）
来源：http://wap.hesvh.cn/Article/details/gpapvmwud.sHtML

L. 网络请求                    （第 12 节，8 个任务，64 条）
来源：http://3g.zdbjq.cn/Article/details/gnalrvvtt.sHtML

M. 命令行 / 进程 / 环境        （第 13 节，8 个任务，64 条）
来源：http://wap.zdbjq.cn/Article/details/gcqifnibn.sHtML

N. 数据结构与算法              （第 14 节，12 个任务，96 条）
来源：http://www.m.share.fehbvm.com/Article/details/gqulcykcy.sHtML

O. 并发与异步                  （第 15 节，6 个任务，48 条）
来源：http://wap.zdbjq.cn/Article/details/gzsijkjdh.sHtML

P. 常用工具函数                （第 16 节，8 个任务，64 条）
来源：http://baike.zdbjq.cn/Article/details/geuuxbhwp.sHtML

Q. SQL 专题                    （第 17 节，90 条）
来源：http://www.share.fehbvm.com/Article/details/gixfjfctr.sHtML


<!-- 参考信息 -->