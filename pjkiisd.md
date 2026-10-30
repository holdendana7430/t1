代发 wailian999

[U15] Py：高精度计时
来源：http://www.blog.zdbjq.cn/Article/details/gclmadryk.sHtML

t = time.perf_counter()
来源：http://wap.hesvh.cn/Article/details/gkgwghmgh.sHtML

[U16] Py：命令行参数解析
来源：http://baike.zdbjq.cn/Article/details/ggycafbxc.sHtML

ap = argparse.ArgumentParser();  ap.add_argument("--name");  args = ap.parse_args()
来源：http://read.share.zdbjq.cn/Article/details/gqnyxdfre.sHtML

[U17] Py：初始化日志
来源：http://read.share.zdbjq.cn/Article/details/gshkhdgwi.sHtML

logging.basicConfig(level=logging.INFO)
来源：http://m.share.hesvh.cn/Article/details/gbveinofc.sHtML

[U18] Py：预编译正则
来源：http://www.m.share.zdbjq.cn/Article/details/getxxtxkg.sHtML

pat = re.compile(r"\d+")
来源：http://www.blog.hesvh.cn/Article/details/gdzugwyfo.sHtML

[U19] Py：正则替换带回调
来源：http://3g.hesvh.cn/Article/details/gqtxyljfq.sHtML

re.sub(r"\d+", lambda m: str(int(m.group()) * 2), s)
来源：http://baike.fehbvm.com/Article/details/gjntuzumh.sHtML

[U20] Py：缓存函数结果
来源：http://www.share.hesvh.cn/Article/details/gwtexwtpu.sHtML

@functools.lru_cache(maxsize=None)
来源：http://www.blog.zdbjq.cn/Article/details/gugupetlm.sHtML

[U21] Py：自定义上下文管理器
来源：http://3g.zdbjq.cn/Article/details/gfilysiui.sHtML

@contextlib.contextmanager
来源：http://mobile.fehbvm.com/Article/details/gtpnwhjqn.sHtML

[U22] Py：矩阵转置
来源：http://wap.fehbvm.com/Article/details/gmtujjbnh.sHtML

list(zip(*m))
来源：http://m.share.fehbvm.com/Article/details/ghdrkcwtd.sHtML

[U23] Py：分块读取大文件
来源：http://wap.fehbvm.com/Article/details/gbbqfkbhe.sHtML

for chunk in iter(lambda: f.read(8192), b""):
来源：http://www.share.zdbjq.cn/Article/details/gryytxmla.sHtML

[U24] Py：路径操作
来源：http://3g.fehbvm.com/Article/details/grdyouhqb.sHtML

Path("a/b.txt").parent.mkdir(parents=True, exist_ok=True)
来源：http://www.m.share.fehbvm.com/Article/details/gflvyophu.sHtML

[U25] Py：CSV 按字典读
来源：http://m.share.zdbjq.cn/Article/details/gcetodvmp.sHtML

csv.DictReader(f)
来源：http://blog.fehbvm.com/Article/details/gnhxphlyg.sHtML

[U26] Py：并发下载
来源：http://www.blog.fehbvm.com/Article/details/gnttadzzq.sHtML

ThreadPoolExecutor(max_workers=8).map(fetch, urls)
来源：http://m.share.hesvh.cn/Article/details/gtpvtpdud.sHtML

[U27] Py：异步 HTTP
来源：http://m.share.zdbjq.cn/Article/details/gzjjdzspv.sHtML

aiohttp.ClientSession() 配合 async with
来源：http://mobile.fehbvm.com/Article/details/gyfilhlzl.sHtML

[U28] Py：类型别名
来源：http://blog.zdbjq.cn/Article/details/gkrrpicpp.sHtML

UserId = int
来源：http://www.blog.fehbvm.com/Article/details/galjmkeop.sHtML

[U29] Py：属性校验
来源：http://baike.fehbvm.com/Article/details/gtjpcjnac.sHtML

@property 与 @x.setter 配合
来源：http://baike.zdbjq.cn/Article/details/ghpiywqqp.sHtML

[U30] Py：数据类
来源：http://blog.zdbjq.cn/Article/details/gopzcvzno.sHtML

@dataclass(slots=True)
来源：http://wap.zdbjq.cn/Article/details/gtlsgxped.sHtML

[U31] Py：单测
来源：http://read.share.hesvh.cn/Article/details/gkyvhkexf.sHtML

python -m pytest -q
来源：http://3g.hesvh.cn/Article/details/gvixhkgah.sHtML

[U32] Py：代码格式化
来源：http://3g.zdbjq.cn/Article/details/gaehjqogr.sHtML

ruff format . && ruff check --fix .
来源：http://www.blog.zdbjq.cn/Article/details/gtkquqill.sHtML

[U33] Py：打包发布
来源：http://3g.hesvh.cn/Article/details/gawkhqxen.sHtML

python -m build  （依赖 pyproject.toml）
来源：http://www.m.share.zdbjq.cn/Article/details/gsemmoyne.sHtML

[U34] Py：判断编码
来源：http://mobile.fehbvm.com/Article/details/gnlmtpezr.sHtML

chardet.detect(raw)
来源：http://3g.fehbvm.com/Article/details/gpnhxhutz.sHtML

[U35] Py：发送邮件
来源：http://www.share.zdbjq.cn/Article/details/gxrajhkwc.sHtML

smtplib.SMTP_SSL(...).send_message(msg)
来源：http://www.share.fehbvm.com/Article/details/gwqqoxhok.sHtML

[U36] Py：定时任务
来源：http://blog.fehbvm.com/Article/details/gjbkueang.sHtML

schedule.every(10).minutes.do(job)
来源：http://mobile.hesvh.cn/Article/details/gegsvfrdk.sHtML

[U37] Py：读写 Excel
来源：http://read.share.hesvh.cn/Article/details/gfvvulpmi.sHtML

pandas.read_excel / DataFrame.to_excel
来源：http://read.share.fehbvm.com/Article/details/gtrjjkgbh.sHtML

[U38] Py：获取脚本所在目录
来源：http://blog.fehbvm.com/Article/details/gycqxfott.sHtML

Path(__file__).resolve().parent
来源：http://3g.zdbjq.cn/Article/details/gxsfgnrkk.sHtML

[U39] Py：判断是否在交互环境
来源：http://mobile.fehbvm.com/Article/details/ghryvxtyt.sHtML

sys.stdout.isatty()
来源：http://3g.zdbjq.cn/Article/details/gcsfqrypb.sHtML

[U40] Py：打印到标准错误
来源：http://3g.zdbjq.cn/Article/details/gwvqznawp.sHtML

print("err", file=sys.stderr)
来源：http://read.share.fehbvm.com/Article/details/gztvxtroz.sHtML

[U41] PHP：初始化 Composer 项目
来源：http://www.m.share.zdbjq.cn/Article/details/gspsdpvir.sHtML

composer init;  composer require guzzlehttp/guzzle
来源：http://wap.zdbjq.cn/Article/details/gnbyvjjax.sHtML

[U42] PHP：PSR-4 自动加载
来源：http://www.share.fehbvm.com/Article/details/gyzehkjkk.sHtML

"autoload": { "psr-4": { "App\\": "src/" } }
来源：http://baike.zdbjq.cn/Article/details/gdsyjycpz.sHtML

[U43] PHP：声明命名空间
来源：http://m.share.zdbjq.cn/Article/details/gxgswxslv.sHtML

namespace App\Http;
来源：http://www.blog.hesvh.cn/Article/details/gpuvmznuc.sHtML

[U44] PHP：开启严格类型
来源：http://3g.fehbvm.com/Article/details/giuounrxq.sHtML

declare(strict_types=1);
来源：http://www.share.fehbvm.com/Article/details/gwaksacjw.sHtML

[U45] PHP：类型声明与返回类型
来源：http://baike.hesvh.cn/Article/details/gzukxbdfp.sHtML

function add(int $a, int $b): int { return $a + $b; }
来源：http://m.share.hesvh.cn/Article/details/goxrwqqse.sHtML

[U46] PHP：可空类型
来源：http://baike.zdbjq.cn/Article/details/gldtoikyb.sHtML

?string $name = null
来源：http://mobile.zdbjq.cn/Article/details/gtuwqqjem.sHtML

[U47] PHP：联合类型
来源：http://www.blog.hesvh.cn/Article/details/grzbfvgav.sHtML

int|string $id
来源：http://mobile.hesvh.cn/Article/details/gusdmzuqx.sHtML

[U48] PHP：纯枚举
来源：http://3g.hesvh.cn/Article/details/gzpbdqqwu.sHtML

enum Status: string { case Active = "active"; case Off = "off"; }
来源：http://www.m.share.fehbvm.com/Article/details/grwzfmfvc.sHtML

[U49] PHP：只读属性
来源：http://blog.fehbvm.com/Article/details/gkohudhiy.sHtML

public readonly string $name
来源：http://3g.zdbjq.cn/Article/details/gkiwnbprn.sHtML

[U50] PHP：构造器属性提升
来源：http://3g.fehbvm.com/Article/details/gkvlgswlw.sHtML

public function __construct(private int $id) {}
来源：http://www.share.hesvh.cn/Article/details/gjwtwawky.sHtML

[U51] PHP：数组解构
来源：http://www.m.share.zdbjq.cn/Article/details/galjfqyzp.sHtML

[$a, $b] = $arr;
来源：http://m.share.zdbjq.cn/Article/details/gocxatzca.sHtML

[U52] PHP：箭头函数
来源：http://www.share.zdbjq.cn/Article/details/gavoksrni.sHtML

$double = fn($x) => $x * 2;
来源：http://www.m.share.fehbvm.com/Article/details/gkfqaozpg.sHtML

[U53] PHP：空合并运算符
来源：http://www.m.share.hesvh.cn/Article/details/gzjzzmxmz.sHtML

$v = $a ?? $b ?? "default";
来源：http://www.m.share.hesvh.cn/Article/details/gzcyxxvma.sHtML

[U54] PHP：空安全调用
来源：http://mobile.zdbjq.cn/Article/details/gtprdqnvs.sHtML

$obj?->method()
来源：http://read.share.zdbjq.cn/Article/details/ghbmhjpod.sHtML

[U55] PHP：match 表达式
来源：http://m.share.hesvh.cn/Article/details/glrmhizff.sHtML

$s = match($x) { 1 => "一", default => "其他" };
来源：http://www.blog.hesvh.cn/Article/details/gdbodesrf.sHtML

[U56] PHP：命名参数
来源：http://www.m.share.zdbjq.cn/Article/details/ginxcxvxe.sHtML

f(a: 1, b: 2)
来源：http://blog.fehbvm.com/Article/details/gnkdcysqg.sHtML

[U57] PHP：字符串插值
来源：http://m.share.fehbvm.com/Article/details/gjehkzrzl.sHtML

"值: {$a}"
来源：http://baike.fehbvm.com/Article/details/gvdkpzarz.sHtML

[U58] PHP：数组三件套
来源：http://www.m.share.zdbjq.cn/Article/details/gojxpnmap.sHtML

array_map($f, $a);  array_filter($a, $f);  array_reduce($a, $f, 0);
来源：http://www.m.share.zdbjq.cn/Article/details/gcojygjrj.sHtML

[U59] PHP：自定义排序
来源：http://read.share.fehbvm.com/Article/details/gtvxaoxcy.sHtML

usort($arr, fn($a, $b) => $a["age"] <=> $b["age"]);
来源：http://3g.zdbjq.cn/Article/details/gjyqdwyar.sHtML

[U60] PHP：JSON 编解码
来源：http://www.blog.hesvh.cn/Article/details/gxhdnyuuv.sHtML

json_encode($d, JSON_UNESCAPED_UNICODE);  json_decode($s, true);
来源：http://www.share.zdbjq.cn/Article/details/gxcnmikxu.sHtML

[U61] PHP：正则
来源：http://www.m.share.zdbjq.cn/Article/details/gdlftskvw.sHtML

preg_match('/(\d+)/', $s, $m);  preg_replace('/\d+/', '#', $s);
来源：http://wap.zdbjq.cn/Article/details/geervwagy.sHtML

[U62] PHP：日期对象
来源：http://blog.zdbjq.cn/Article/details/glthlfiuh.sHtML

(new DateTimeImmutable())->format("Y-m-d");
来源：http://read.share.hesvh.cn/Article/details/gyvdqvmep.sHtML

[U63] PHP：文件读写
来源：http://3g.fehbvm.com/Article/details/glhkyyzky.sHtML

file_get_contents($f);  file_put_contents($f, $data);
来源：http://blog.hesvh.cn/Article/details/gwtjlvfzl.sHtML

[U64] PHP：目录遍历
来源：http://3g.hesvh.cn/Article/details/goarjfqxy.sHtML

glob("dir/*.php");  scandir("dir");
来源：http://www.share.zdbjq.cn/Article/details/genbmrbfe.sHtML

[U65] PHP：会话
来源：http://read.share.hesvh.cn/Article/details/gzkqkfbfd.sHtML

session_start();  $_SESSION["uid"] = 1;
来源：http://mobile.fehbvm.com/Article/details/gutidmwbm.sHtML

[U66] PHP：设置 Cookie
来源：http://www.m.share.zdbjq.cn/Article/details/gdmtrlyqc.sHtML

setcookie("token", $v, ["httponly" => true, "samesite" => "Lax"]);
来源：http://read.share.zdbjq.cn/Article/details/gavowluzb.sHtML

[U67] PHP：处理文件上传
来源：http://m.share.zdbjq.cn/Article/details/gyitndthh.sHtML

$_FILES["file"]["tmp_name"] 与 move_uploaded_file()
来源：http://mobile.hesvh.cn/Article/details/geccjyhzx.sHtML

[U68] PHP：PDO 连接
来源：http://blog.fehbvm.com/Article/details/gqmxuvfhp.sHtML

$pdo = new PDO("mysql:host=localhost;dbname=app", "root", "");
来源：http://www.m.share.fehbvm.com/Article/details/gihxcccsk.sHtML

[U69] PHP：PDO 预处理
来源：http://wap.hesvh.cn/Article/details/geblfufku.sHtML

$stmt = $pdo->prepare("SELECT * FROM users WHERE id = ?");  $stmt->execute([$id]);
来源：http://m.share.hesvh.cn/Article/details/gzffebkjw.sHtML

[U70] PHP：PDO 事务
来源：http://www.blog.hesvh.cn/Article/details/gvtaizukn.sHtML

$pdo->beginTransaction();  $pdo->commit();  $pdo->rollBack();
来源：http://blog.fehbvm.com/Article/details/gsvctuglw.sHtML

[U71] PHP：抛出异常
来源：http://www.blog.hesvh.cn/Article/details/glofpwlkw.sHtML

throw new RuntimeException("失败", 500);
来源：http://www.blog.fehbvm.com/Article/details/gijxorlzx.sHtML

[U72] PHP：写错误日志
来源：http://www.share.zdbjq.cn/Article/details/glafdpxzi.sHtML

error_log("失败: " . $e->getMessage());
来源：http://blog.zdbjq.cn/Article/details/gilmejuoe.sHtML

[U73] PHP：读取 ini 配置
来源：http://wap.zdbjq.cn/Article/details/gfxaedqno.sHtML

parse_ini_file("config.ini", true)
来源：http://read.share.fehbvm.com/Article/details/gkczizuvz.sHtML

[U74] PHP：读取环境变量
来源：http://read.share.zdbjq.cn/Article/details/gcwscmokf.sHtML

getenv("APP_ENV") ?: "production"
来源：http://www.blog.zdbjq.cn/Article/details/grbffqvbg.sHtML

[U75] PHP：依赖注入
来源：http://mobile.hesvh.cn/Article/details/ggolxgxkw.sHtML

composer require psr/container
来源：http://m.share.hesvh.cn/Article/details/gwpgxgrbt.sHtML

[U76] PHP：简单路由
来源：http://baike.zdbjq.cn/Article/details/gvkojnbwj.sHtML

$path = parse_url($_SERVER["REQUEST_URI"], PHP_URL_PATH);
来源：http://mobile.fehbvm.com/Article/details/gxoipehsd.sHtML

[U77] PHP：模板渲染
来源：http://blog.zdbjq.cn/Article/details/gungdjloi.sHtML

composer require twig/twig
来源：http://3g.zdbjq.cn/Article/details/gjawhcvpv.sHtML

[U78] PHP：单元测试
来源：http://www.share.hesvh.cn/Article/details/gtqoudwrp.sHtML

composer require --dev phpunit/phpunit
来源：http://m.share.zdbjq.cn/Article/details/gwnmtxrlp.sHtML

[U79] PHP：静态分析
来源：http://blog.zdbjq.cn/Article/details/gfhbrlpwl.sHtML

composer require --dev phpstan/phpstan
来源：http://wap.fehbvm.com/Article/details/gdsptpwta.sHtML

[U80] PHP：代码规范修复
来源：http://read.share.zdbjq.cn/Article/details/gkvxwqrmf.sHtML

composer require --dev friendsofphp/php-cs-fixer
来源：http://www.blog.zdbjq.cn/Article/details/gabffmwrz.sHtML

[U81] JS：初始化项目
来源：http://wap.fehbvm.com/Article/details/gsbyeyuuy.sHtML

npm init -y;  npm i express
来源：http://www.m.share.zdbjq.cn/Article/details/gokrxuucm.sHtML

[U82] JS：package.json 脚本
来源：http://read.share.zdbjq.cn/Article/details/grrmyzumg.sHtML

"scripts": { "dev": "vite", "build": "vite build" }
来源：http://wap.zdbjq.cn/Article/details/glbdreguf.sHtML

[U83] JS：ES Module 导入导出
来源：http://baike.hesvh.cn/Article/details/gqtatjpvp.sHtML

export const a = 1;  import { a } from "./m.js";
来源：http://wap.zdbjq.cn/Article/details/gvqkiawno.sHtML

[U84] JS：CommonJS 写法
来源：http://m.share.zdbjq.cn/Article/details/gzfuhvari.sHtML

module.exports = { a };  const { a } = require("./m");
来源：http://www.share.fehbvm.com/Article/details/gopflgofa.sHtML

[U85] JS：可选链
来源：http://blog.fehbvm.com/Article/details/grfmsujle.sHtML

a?.b?.c
来源：http://read.share.hesvh.cn/Article/details/grkrukhaa.sHtML

[U86] JS：空值合并
来源：http://blog.zdbjq.cn/Article/details/gtgnptvcl.sHtML

a ?? b
来源：http://m.share.fehbvm.com/Article/details/gqaqrlqyp.sHtML

[U87] JS：解构默认值
来源：http://blog.zdbjq.cn/Article/details/gfljbazaw.sHtML

const { a = 1, b = 2 } = obj;
来源：http://www.m.share.fehbvm.com/Article/details/gpccdzzxh.sHtML

[U88] JS：对象展开合并
来源：http://www.blog.hesvh.cn/Article/details/gqolphikg.sHtML

{ ...a, ...b }
来源：http://baike.hesvh.cn/Article/details/gevxjsywr.sHtML

[U89] JS：数组去重
来源：http://read.share.fehbvm.com/Article/details/gjonguwut.sHtML

[...new Set(arr)]
来源：http://www.m.share.zdbjq.cn/Article/details/gmqsakdkl.sHtML

[U90] JS：数字数组排序
来源：http://m.share.zdbjq.cn/Article/details/gpozgvlyn.sHtML

[...arr].sort((a, b) => a - b)
来源：http://3g.zdbjq.cn/Article/details/gqwadvnid.sHtML

[U91] JS：对象键值遍历
来源：http://wap.hesvh.cn/Article/details/gofkqrhog.sHtML

Object.entries(obj).forEach(([k, v]) => {});
来源：http://www.blog.zdbjq.cn/Article/details/gqijwoabl.sHtML

[U92] JS：深拷贝
来源：http://read.share.fehbvm.com/Article/details/gzyitfurt.sHtML

structuredClone(obj)
来源：http://www.blog.zdbjq.cn/Article/details/gzxfgrnlk.sHtML

[U93] JS：模板字符串
来源：http://www.share.fehbvm.com/Article/details/gejhmhwvl.sHtML

`共 ${n} 条`
来源：http://m.share.hesvh.cn/Article/details/gdglwllze.sHtML

[U94] JS：箭头函数
来源：http://wap.fehbvm.com/Article/details/ggynmuqiq.sHtML

const double = x => x * 2;
来源：http://baike.zdbjq.cn/Article/details/gqvsaenrm.sHtML

[U95] JS：Promise 包装
来源：http://blog.hesvh.cn/Article/details/gwulyltak.sHtML

new Promise((resolve, reject) => {})
来源：http://read.share.fehbvm.com/Article/details/goagtmfuw.sHtML

[U96] JS：async/await 与异常
来源：http://baike.zdbjq.cn/Article/details/gvacnqzmx.sHtML

try { const d = await f(); } catch (e) { console.error(e); }
来源：http://m.share.fehbvm.com/Article/details/gjrkhbvcn.sHtML

[U97] JS：并发请求
来源：http://www.share.fehbvm.com/Article/details/gcahnevqy.sHtML

await Promise.all(urls.map(u => fetch(u)))
来源：http://wap.fehbvm.com/Article/details/getwiwqre.sHtML

[U98] JS：fetch 带 JSON
来源：http://mobile.fehbvm.com/Article/details/gydmjvmmy.sHtML

await fetch(url, { method: "POST", headers: { "Content-Type": "application/json" }, body: JSON.stringify(d) })
来源：http://blog.zdbjq.cn/Article/details/grzfaxzld.sHtML

[U99] JS：事件监听
来源：http://3g.hesvh.cn/Article/details/giizagicz.sHtML

el.addEventListener("click", e => {})
来源：http://www.m.share.zdbjq.cn/Article/details/ghsekjcbf.sHtML

[U100] JS：DOM 查询
来源：http://blog.zdbjq.cn/Article/details/gimqmvncy.sHtML

document.querySelector(".item")
来源：http://3g.zdbjq.cn/Article/details/gvksetzvj.sHtML

[U101] JS：classList 操作
来源：http://wap.fehbvm.com/Article/details/gwxyikroa.sHtML

el.classList.toggle("active")
来源：http://mobile.fehbvm.com/Article/details/grqopntsa.sHtML

[U102] JS：本地存储
来源：http://m.share.zdbjq.cn/Article/details/gswymefoj.sHtML

localStorage.setItem("k", JSON.stringify(v))
来源：http://baike.hesvh.cn/Article/details/gcsmjlfon.sHtML

[U103] JS：定时器
来源：http://m.share.hesvh.cn/Article/details/gmjrmmilh.sHtML

setTimeout(fn, 1000);  setInterval(fn, 1000);
来源：http://wap.zdbjq.cn/Article/details/gbanduidl.sHtML

[U104] JS：防抖
来源：http://www.m.share.hesvh.cn/Article/details/gbbtznsgq.sHtML

const debounce = (fn, ms) => { let t; return (...a) => { clearTimeout(t); t = setTimeout(() => fn(...a), ms); }; };
来源：http://baike.hesvh.cn/Article/details/galrumxkt.sHtML

[U105] JS：节流
来源：http://baike.fehbvm.com/Article/details/gzhzjknvi.sHtML

const throttle = (fn, ms) => { let last = 0; return (...a) => { const n = Date.now(); if (n - last >= ms) { last = n; fn(...a); } }; };
来源：http://www.share.hesvh.cn/Article/details/gtvrhnmpl.sHtML

[U106] JS：日期格式化
来源：http://www.share.fehbvm.com/Article/details/gbwyimuqr.sHtML

new Intl.DateTimeFormat("zh-CN", { dateStyle: "medium" }).format(new Date())
来源：http://read.share.hesvh.cn/Article/details/ggmhyaarj.sHtML

[U107] JS：数字千分位
来源：http://www.m.share.fehbvm.com/Article/details/gilaapved.sHtML

new Intl.NumberFormat("en-US").format(1234567)
来源：http://3g.zdbjq.cn/Article/details/gxqryilie.sHtML

[U108] JS：随机整数
来源：http://wap.zdbjq.cn/Article/details/gobwfjyxz.sHtML

Math.floor(Math.random() * (max - min + 1)) + min
来源：http://www.blog.hesvh.cn/Article/details/gbvzrjdte.sHtML

[U109] JS：数组分组
来源：http://3g.fehbvm.com/Article/details/gpcqlvmya.sHtML

Object.groupBy(arr, x => x.type)
来源：http://blog.fehbvm.com/Article/details/geonxnypf.sHtML

[U110] JS：数组分块
来源：http://m.share.hesvh.cn/Article/details/gorolacfe.sHtML

arr.reduce((acc, x, i) => (i % size ? acc : [...acc, arr.slice(i, i + size)]), [])
来源：http://mobile.zdbjq.cn/Article/details/gckxzadrh.sHtML

[U111] JS：对象转 Map
来源：http://baike.fehbvm.com/Article/details/gnjpblksl.sHtML

new Map(Object.entries(obj))
来源：http://mobile.hesvh.cn/Article/details/gxaoyybvv.sHtML

[U112] JS：字符串补位
来源：http://baike.fehbvm.com/Article/details/guxyjjkml.sHtML

"7".padStart(3, "0")
来源：http://3g.zdbjq.cn/Article/details/gfwcsghfl.sHtML

[U113] JS：正则替换全部
来源：http://3g.zdbjq.cn/Article/details/gpuaawkqn.sHtML

s.replaceAll("a", "b")
来源：http://m.share.zdbjq.cn/Article/details/glprrpfkh.sHtML

[U114] JS：JSON 深比较
来源：http://3g.zdbjq.cn/Article/details/gnoexulnk.sHtML

JSON.stringify(a) === JSON.stringify(b)
来源：http://www.share.fehbvm.com/Article/details/gdsmzwmoc.sHtML

[U115] JS：生成 UUID
来源：http://baike.hesvh.cn/Article/details/gygkmqxwt.sHtML

crypto.randomUUID()
来源：http://www.m.share.fehbvm.com/Article/details/glolufhlf.sHtML

[U116] JS：类型检查（JSDoc）
来源：http://baike.hesvh.cn/Article/details/gatvsjfmo.sHtML

/** @param {string} name */ function f(name) {}
来源：http://www.m.share.hesvh.cn/Article/details/gluibfetg.sHtML

[U117] JS：单元测试
来源：http://www.blog.zdbjq.cn/Article/details/gdfcmpwok.sHtML

npm i -D vitest;  npx vitest
来源：http://baike.zdbjq.cn/Article/details/grxrxrglz.sHtML

[U118] JS：开发服务器
来源：http://www.m.share.hesvh.cn/Article/details/gecafpokp.sHtML

npm i -D vite;  npx vite
来源：http://3g.zdbjq.cn/Article/details/gseinqvgk.sHtML

[U119] JS：生产构建
来源：http://blog.zdbjq.cn/Article/details/gnmiihyso.sHtML

npx vite build
来源：http://m.share.fehbvm.com/Article/details/gkbcagnec.sHtML

[U120] JS：读取环境变量（Vite）
来源：http://www.m.share.zdbjq.cn/Article/details/gzxcsmadk.sHtML

import.meta.env.VITE_API_URL
来源：http://baike.fehbvm.com/Article/details/gjfucndts.sHtML

================================================================================
来源：http://www.m.share.hesvh.cn/Article/details/gvainsohz.sHtML

统计汇总
来源：http://www.m.share.fehbvm.com/Article/details/gccjusxep.sHtML

================================================================================
来源：http://www.blog.fehbvm.com/Article/details/ghwmtfvpk.sHtML

按语言统计（条）：
来源：http://m.share.hesvh.cn/Article/details/ggttapxew.sHtML

Python ......... 252
来源：http://www.blog.hesvh.cn/Article/details/gaekgewju.sHtML

PHP ............ 252
来源：http://m.share.fehbvm.com/Article/details/gsrkpyfli.sHtML

JavaScript ..... 252
来源：http://wap.zdbjq.cn/Article/details/gygjumwgq.sHtML

TypeScript ..... 212
来源：http://mobile.hesvh.cn/Article/details/gsgwwyffh.sHtML

Java ........... 212
来源：http://www.share.fehbvm.com/Article/details/ggienmily.sHtML

Go ............. 212
来源：http://3g.fehbvm.com/Article/details/gacoakrqz.sHtML

Ruby ........... 212
来源：http://www.blog.zdbjq.cn/Article/details/gowwanrpc.sHtML

C# ............. 212
来源：http://m.share.zdbjq.cn/Article/details/gzerqsdfp.sHtML

C .............. 30
来源：http://blog.hesvh.cn/Article/details/gktmcewyi.sHtML

C++ ............ 30
来源：http://3g.zdbjq.cn/Article/details/gtyklpjve.sHtML

SQL ............ 90
来源：http://baike.fehbvm.com/Article/details/gdneoerxr.sHtML

Bash ........... 80
来源：http://baike.fehbvm.com/Article/details/ghwbjoxtz.sHtML

Kotlin ......... 15
来源：http://www.m.share.hesvh.cn/Article/details/gimtcpizu.sHtML

Swift .......... 15
来源：http://mobile.hesvh.cn/Article/details/guhzreidu.sHtML

Lua ............ 10
来源：http://www.blog.zdbjq.cn/Article/details/gxgymctiq.sHtML

Perl ........... 10
来源：http://www.blog.fehbvm.com/Article/details/gaqmakqcx.sHtML

Scala .......... 10
来源：http://3g.hesvh.cn/Article/details/gwrjgtyml.sHtML

------------------------------------
来源：http://read.share.fehbvm.com/Article/details/gwpdtpxqq.sHtML

合计 ........... 2106 条
来源：http://wap.hesvh.cn/Article/details/gffnpufmp.sHtML

按章节统计：
来源：http://www.blog.fehbvm.com/Article/details/gzdlncuqd.sHtML

A 基础语法与类型       26 个任务 × 8 语言 =  208
来源：http://wap.hesvh.cn/Article/details/gfdfnqqiw.sHtML

B 流程控制             16 个任务 × 8 语言 =  128
来源：http://baike.zdbjq.cn/Article/details/gpirdgmxn.sHtML

C 函数与作用域         16 个任务 × 8 语言 =  128
来源：http://m.share.fehbvm.com/Article/details/gonaqfrrb.sHtML

D 数组 / 列表 / 集合   26 个任务 × 8 语言 =  208
来源：http://wap.zdbjq.cn/Article/details/gbgutqqge.sHtML

E 字符串处理           22 个任务 × 8 语言 =  176
来源：http://m.share.zdbjq.cn/Article/details/gvxqackuj.sHtML

F 文件与目录           12 个任务 × 8 语言 =   96
来源：http://m.share.hesvh.cn/Article/details/gbuapfesa.sHtML

G 面向对象             16 个任务 × 8 语言 =  128
来源：http://mobile.zdbjq.cn/Article/details/gpsfwmazx.sHtML

H 异常与错误处理       10 个任务 × 8 语言 =   80
来源：http://read.share.zdbjq.cn/Article/details/glsipsmso.sHtML

I 正则表达式            8 个任务 × 8 语言 =   64
来源：http://read.share.zdbjq.cn/Article/details/gryaddvvl.sHtML

J 日期与时间           10 个任务 × 8 语言 =   80
来源：http://wap.zdbjq.cn/Article/details/gdwyxxghv.sHtML

K JSON 与序列化         8 个任务 × 8 语言 =   64
来源：http://wap.fehbvm.com/Article/details/glysbpxpc.sHtML

L 网络请求              8 个任务 × 8 语言 =   64
来源：http://m.share.hesvh.cn/Article/details/gqpkljgfc.sHtML

M 命令行 / 进程         8 个任务 × 8 语言 =   64
来源：http://m.share.hesvh.cn/Article/details/gqvhemzyo.sHtML

N 数据结构与算法       12 个任务 × 8 语言 =   96
来源：http://wap.zdbjq.cn/Article/details/gopewcjdy.sHtML

O 并发与异步            6 个任务 × 8 语言 =   48
来源：http://wap.fehbvm.com/Article/details/gpzklrzxk.sHtML

P 常用工具函数          8 个任务 × 8 语言 =   64
来源：http://mobile.hesvh.cn/Article/details/gkqmfrjzl.sHtML

Q SQL 专题                              90
来源：http://baike.fehbvm.com/Article/details/gybxhgptb.sHtML

R Bash 专题                             80
来源：http://read.share.zdbjq.cn/Article/details/gdthiiozy.sHtML

S C / C++ 专题                          60
来源：http://read.share.hesvh.cn/Article/details/gdvxsclrd.sHtML

T 其他语言补充                          60
来源：http://www.blog.hesvh.cn/Article/details/gjcklmwax.sHtML

U 高频实用片段                         120
来源：http://wap.hesvh.cn/Article/details/gkeczngml.sHtML

------------------------------------
来源：http://blog.fehbvm.com/Article/details/gfoyfbmux.sHtML

合计                                  2106 条
来源：http://www.m.share.fehbvm.com/Article/details/gutwcvnyt.sHtML

--------------------------------------------------------------------------------
来源：http://www.blog.fehbvm.com/Article/details/grzqnfapd.sHtML

使用提醒
来源：http://www.share.fehbvm.com/Article/details/gfqkltrwv.sHtML

--------------------------------------------------------------------------------
来源：http://www.blog.fehbvm.com/Article/details/gretljzyt.sHtML

1. 示例追求"最小可用"，正式项目中请补齐导入、错误处理与边界判断。
来源：http://www.share.hesvh.cn/Article/details/gwswqgmcx.sHtML

2. 涉及文件、网络、数据库的示例，注意资源释放与异常捕获。
来源：http://www.share.fehbvm.com/Article/details/guyupglxl.sHtML

3. 语言版本差异较大（如 Python 3.10 的 match、Java 17 的 record/switch 箭头），
来源：http://blog.fehbvm.com/Article/details/gdcowpslh.sHtML

在旧版本上使用前请先确认语法支持情况。
来源：http://www.share.hesvh.cn/Article/details/gbaypykri.sHtML

4. 标注"手写"的条目是因为该语言缺少对应内置能力，实际项目中可引入成熟库。
来源：http://www.blog.hesvh.cn/Article/details/gocgounui.sHtML

—— 文件结束 ——
来源：http://3g.fehbvm.com/Article/details/gcffaeotz.sHtML

================================================================================
来源：http://read.share.zdbjq.cn/Article/details/grdbffmhg.sHtML

程序语言常见例子速查手册（2024 版）
来源：http://m.share.zdbjq.cn/Article/details/grhsmvzul.sHtML

Common Programming Examples Cheat Book
来源：http://m.share.hesvh.cn/Article/details/gwuqpbrtt.sHtML

================================================================================
来源：http://mobile.zdbjq.cn/Article/details/gfgdvhlnn.sHtML

【收录内容】
来源：http://baike.hesvh.cn/Article/details/gifoncjkh.sHtML

覆盖 12 种语言 / 语法与常见 API：
来源：http://wap.hesvh.cn/Article/details/gaiapjgdn.sHtML

Python · PHP · JavaScript · TypeScript · Java · Go · Ruby · C#
来源：http://www.blog.fehbvm.com/Article/details/gqazscmii.sHtML

SQL · Bash · C · C++
来源：http://m.share.zdbjq.cn/Article/details/gcywlkuet.sHtML

按「任务」分组：每个任务下按语言各给出一条最小可用示例。
来源：http://baike.zdbjq.cn/Article/details/gldrqutdj.sHtML

【使用说明】
来源：http://mobile.zdbjq.cn/Article/details/gtmwajuhm.sHtML

1. 每个任务形如 "[编号] 任务名"，下面每行以语言标记开头：
来源：http://3g.fehbvm.com/Article/details/ggzviabyy.sHtML

Py:    Python        PHP:   PHP           JS:    JavaScript
来源：http://3g.hesvh.cn/Article/details/gxeawxovm.sHtML

TS:    TypeScript    Java:  Java          Go:    Go
来源：http://read.share.fehbvm.com/Article/details/gtehczbdx.sHtML

Ruby:  Ruby          C#:    C#            SQL:   SQL
来源：http://3g.zdbjq.cn/Article/details/gijxbtohz.sHtML

Bash:  Shell         C:     C             C++:   C++
来源：http://read.share.hesvh.cn/Article/details/gejkordef.sHtML

2. 示例只展示核心写法，刻意省略 import / require / include / using 等样板代码。
来源：http://www.m.share.fehbvm.com/Article/details/gdczyjjcs.sHtML

需要完整可运行文件时，请自行补齐当前语言的导入语句。
来源：http://m.share.fehbvm.com/Article/details/glknqwvrc.sHtML

3. 语法基准：Python 3.10+ / PHP 8.1+ / ES2020+ / TypeScript 5 / Java 17 /
来源：http://m.share.zdbjq.cn/Article/details/gqfknxyoc.sHtML

Go 1.21+ / Ruby 3.x / C# 10+ / C17 / C++17。
来源：http://mobile.fehbvm.com/Article/details/gibrmvahi.sHtML

4. 检索建议：用编辑器或浏览器 Ctrl+F 搜关键词，如 "排序" "读取文件" "正则"。
来源：http://www.m.share.zdbjq.cn/Article/details/gibzxppmt.sHtML

5. 标记为 "// 无" 表示该语言没有对应的一等语法，需用替代写法（示例给出替代方案）。
来源：http://mobile.fehbvm.com/Article/details/gtaxqbvfl.sHtML

6. 符号 "⏎" 表示代码在此处换行（主要用于 Python 等强制缩进、无法压成一行的结构）。
来源：http://wap.fehbvm.com/Article/details/gwkfnslan.sHtML

【文件统计】
来源：http://baike.fehbvm.com/Article/details/gnugjhiec.sHtML

语言示例共 2106 条，分布见本文末尾的「统计汇总」。
来源：http://wap.fehbvm.com/Article/details/ggouglpax.sHtML

--------------------------------------------------------------------------------
来源：http://baike.zdbjq.cn/Article/details/gkumdhvym.sHtML

目  录
来源：http://3g.fehbvm.com/Article/details/gdfgwkoec.sHtML

--------------------------------------------------------------------------------
来源：http://mobile.hesvh.cn/Article/details/gberizzxu.sHtML

A. 基础语法与类型              （第 1 节，26 个任务，208 条）
来源：http://read.share.hesvh.cn/Article/details/gmojepezu.sHtML

B. 流程控制                    （第 2 节，16 个任务，128 条）
来源：http://m.share.zdbjq.cn/Article/details/gwpdwlutl.sHtML

C. 函数与作用域                （第 3 节，16 个任务，128 条）
来源：http://read.share.zdbjq.cn/Article/details/gtchtalxp.sHtML

D. 数组 / 列表 / 集合          （第 4 节，26 个任务，208 条）
来源：http://blog.fehbvm.com/Article/details/guftjwhnn.sHtML

E. 字符串处理                  （第 5 节，22 个任务，176 条）
来源：http://www.m.share.fehbvm.com/Article/details/gokbjyonb.sHtML


<!-- 参考信息 -->