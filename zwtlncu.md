代发 wailian999

[U17] Py：初始化日志
来源：http://www.share.hesvh.cn/Article/details/gkwfglvub.sHtML

logging.basicConfig(level=logging.INFO)
来源：http://3g.fehbvm.com/Article/details/gfbdzugmw.sHtML

[U18] Py：预编译正则
来源：http://baike.fehbvm.com/Article/details/gcwkibmti.sHtML

pat = re.compile(r"\d+")
来源：http://blog.zdbjq.cn/Article/details/gukguswll.sHtML

[U19] Py：正则替换带回调
来源：http://www.m.share.zdbjq.cn/Article/details/gtjmmzjke.sHtML

re.sub(r"\d+", lambda m: str(int(m.group()) * 2), s)
来源：http://wap.fehbvm.com/Article/details/gqttqmdbe.sHtML

[U20] Py：缓存函数结果
来源：http://www.share.zdbjq.cn/Article/details/gthypgnop.sHtML

@functools.lru_cache(maxsize=None)
来源：http://m.share.fehbvm.com/Article/details/gprrzdtkq.sHtML

[U21] Py：自定义上下文管理器
来源：http://m.share.hesvh.cn/Article/details/gxcwdmeko.sHtML

@contextlib.contextmanager
来源：http://3g.zdbjq.cn/Article/details/gljjvxhch.sHtML

[U22] Py：矩阵转置
来源：http://blog.zdbjq.cn/Article/details/gimpxzqve.sHtML

list(zip(*m))
来源：http://m.share.hesvh.cn/Article/details/gdytgqhil.sHtML

[U23] Py：分块读取大文件
来源：http://read.share.hesvh.cn/Article/details/gxubmndue.sHtML

for chunk in iter(lambda: f.read(8192), b""):
来源：http://wap.fehbvm.com/Article/details/gurxdhdrn.sHtML

[U24] Py：路径操作
来源：http://www.m.share.zdbjq.cn/Article/details/grazzrqfo.sHtML

Path("a/b.txt").parent.mkdir(parents=True, exist_ok=True)
来源：http://blog.hesvh.cn/Article/details/gjeejjhmf.sHtML

[U25] Py：CSV 按字典读
来源：http://baike.zdbjq.cn/Article/details/gthgdsynn.sHtML

csv.DictReader(f)
来源：http://3g.fehbvm.com/Article/details/gunjhkwnv.sHtML

[U26] Py：并发下载
来源：http://3g.zdbjq.cn/Article/details/gdzlitsbj.sHtML

ThreadPoolExecutor(max_workers=8).map(fetch, urls)
来源：http://baike.hesvh.cn/Article/details/gcqlrjyah.sHtML

[U27] Py：异步 HTTP
来源：http://wap.fehbvm.com/Article/details/gdozhyppg.sHtML

aiohttp.ClientSession() 配合 async with
来源：http://www.m.share.fehbvm.com/Article/details/goxdlshov.sHtML

[U28] Py：类型别名
来源：http://blog.fehbvm.com/Article/details/gbsrcsmmi.sHtML

UserId = int
来源：http://blog.hesvh.cn/Article/details/gjgwrlvao.sHtML

[U29] Py：属性校验
来源：http://read.share.fehbvm.com/Article/details/goerwnyjy.sHtML

@property 与 @x.setter 配合
来源：http://3g.hesvh.cn/Article/details/gnzyijbbq.sHtML

[U30] Py：数据类
来源：http://m.share.zdbjq.cn/Article/details/gskaaolka.sHtML

@dataclass(slots=True)
来源：http://3g.zdbjq.cn/Article/details/gfhseexhw.sHtML

[U31] Py：单测
来源：http://wap.hesvh.cn/Article/details/gbgpbzdzn.sHtML

python -m pytest -q
来源：http://3g.zdbjq.cn/Article/details/gwrytlawb.sHtML

[U32] Py：代码格式化
来源：http://baike.fehbvm.com/Article/details/glkhjxasj.sHtML

ruff format . && ruff check --fix .
来源：http://read.share.hesvh.cn/Article/details/gyyifnujj.sHtML

[U33] Py：打包发布
来源：http://3g.zdbjq.cn/Article/details/gumqtomfw.sHtML

python -m build  （依赖 pyproject.toml）
来源：http://mobile.hesvh.cn/Article/details/gjakhcjxh.sHtML

[U34] Py：判断编码
来源：http://3g.hesvh.cn/Article/details/gablqrdda.sHtML

chardet.detect(raw)
来源：http://3g.zdbjq.cn/Article/details/gisdwflfq.sHtML

[U35] Py：发送邮件
来源：http://baike.fehbvm.com/Article/details/gmfmkyngd.sHtML

smtplib.SMTP_SSL(...).send_message(msg)
来源：http://3g.hesvh.cn/Article/details/garadebkm.sHtML

[U36] Py：定时任务
来源：http://blog.hesvh.cn/Article/details/gppqzulfa.sHtML

schedule.every(10).minutes.do(job)
来源：http://3g.hesvh.cn/Article/details/guejmlvhp.sHtML

[U37] Py：读写 Excel
来源：http://mobile.fehbvm.com/Article/details/gpirbokao.sHtML

pandas.read_excel / DataFrame.to_excel
来源：http://blog.fehbvm.com/Article/details/giamhpuff.sHtML

[U38] Py：获取脚本所在目录
来源：http://3g.hesvh.cn/Article/details/gzzvpqezb.sHtML

Path(__file__).resolve().parent
来源：http://baike.zdbjq.cn/Article/details/ggaoaycrp.sHtML

[U39] Py：判断是否在交互环境
来源：http://3g.zdbjq.cn/Article/details/gxbfedcxd.sHtML

sys.stdout.isatty()
来源：http://mobile.zdbjq.cn/Article/details/ghcbuowkw.sHtML

[U40] Py：打印到标准错误
来源：http://m.share.fehbvm.com/Article/details/gwwyhcuey.sHtML

print("err", file=sys.stderr)
来源：http://www.blog.fehbvm.com/Article/details/gofluwpae.sHtML

[U41] PHP：初始化 Composer 项目
来源：http://mobile.zdbjq.cn/Article/details/gfcmfadma.sHtML

composer init;  composer require guzzlehttp/guzzle
来源：http://baike.zdbjq.cn/Article/details/gsuvmybdo.sHtML

[U42] PHP：PSR-4 自动加载
来源：http://blog.hesvh.cn/Article/details/gjavzkknq.sHtML

"autoload": { "psr-4": { "App\\": "src/" } }
来源：http://wap.fehbvm.com/Article/details/gfvpqqeag.sHtML

[U43] PHP：声明命名空间
来源：http://blog.zdbjq.cn/Article/details/gnuioikhh.sHtML

namespace App\Http;
来源：http://baike.fehbvm.com/Article/details/gypddvkav.sHtML

[U44] PHP：开启严格类型
来源：http://m.share.zdbjq.cn/Article/details/gahhunrmc.sHtML

declare(strict_types=1);
来源：http://baike.hesvh.cn/Article/details/gjnkxexlq.sHtML

[U45] PHP：类型声明与返回类型
来源：http://baike.zdbjq.cn/Article/details/gqbtakeje.sHtML

function add(int $a, int $b): int { return $a + $b; }
来源：http://www.m.share.hesvh.cn/Article/details/grfnmgjts.sHtML

[U46] PHP：可空类型
来源：http://m.share.zdbjq.cn/Article/details/gbixtjmim.sHtML

?string $name = null
来源：http://m.share.fehbvm.com/Article/details/gxotilkwa.sHtML

[U47] PHP：联合类型
来源：http://m.share.zdbjq.cn/Article/details/goryrelbp.sHtML

int|string $id
来源：http://mobile.hesvh.cn/Article/details/glzcpdqgx.sHtML

[U48] PHP：纯枚举
来源：http://mobile.fehbvm.com/Article/details/gkxofdlqx.sHtML

enum Status: string { case Active = "active"; case Off = "off"; }
来源：http://www.m.share.zdbjq.cn/Article/details/gjveegdcx.sHtML

[U49] PHP：只读属性
来源：http://mobile.fehbvm.com/Article/details/gpnnuoedw.sHtML

public readonly string $name
来源：http://wap.zdbjq.cn/Article/details/gcmmyxnfy.sHtML

[U50] PHP：构造器属性提升
来源：http://m.share.fehbvm.com/Article/details/gdnhlqlei.sHtML

public function __construct(private int $id) {}
来源：http://baike.zdbjq.cn/Article/details/gbhwiaqii.sHtML

[U51] PHP：数组解构
来源：http://blog.zdbjq.cn/Article/details/grjbagzcj.sHtML

[$a, $b] = $arr;
来源：http://read.share.hesvh.cn/Article/details/gdrojgcqn.sHtML

[U52] PHP：箭头函数
来源：http://www.blog.hesvh.cn/Article/details/gldpjmvgf.sHtML

$double = fn($x) => $x * 2;
来源：http://m.share.hesvh.cn/Article/details/ghnasfyww.sHtML

[U53] PHP：空合并运算符
来源：http://read.share.fehbvm.com/Article/details/goawcvwuj.sHtML

$v = $a ?? $b ?? "default";
来源：http://blog.zdbjq.cn/Article/details/gmvzcibgb.sHtML

[U54] PHP：空安全调用
来源：http://www.blog.zdbjq.cn/Article/details/gahglflnw.sHtML

$obj?->method()
来源：http://baike.zdbjq.cn/Article/details/gqbruxkdl.sHtML

[U55] PHP：match 表达式
来源：http://3g.hesvh.cn/Article/details/gvcginawl.sHtML

$s = match($x) { 1 => "一", default => "其他" };
来源：http://blog.zdbjq.cn/Article/details/gnejglmgc.sHtML

[U56] PHP：命名参数
来源：http://m.share.zdbjq.cn/Article/details/gbvnqcowj.sHtML

f(a: 1, b: 2)
来源：http://blog.fehbvm.com/Article/details/glqlydtbk.sHtML

[U57] PHP：字符串插值
来源：http://www.m.share.zdbjq.cn/Article/details/ggzgpmpce.sHtML

"值: {$a}"
来源：http://wap.zdbjq.cn/Article/details/guqiamvsu.sHtML

[U58] PHP：数组三件套
来源：http://wap.hesvh.cn/Article/details/gjbsradyc.sHtML

array_map($f, $a);  array_filter($a, $f);  array_reduce($a, $f, 0);
来源：http://m.share.hesvh.cn/Article/details/gnovdytwd.sHtML

[U59] PHP：自定义排序
来源：http://blog.hesvh.cn/Article/details/gkeytcbtx.sHtML

usort($arr, fn($a, $b) => $a["age"] <=> $b["age"]);
来源：http://www.m.share.zdbjq.cn/Article/details/gimkrzdho.sHtML

[U60] PHP：JSON 编解码
来源：http://baike.hesvh.cn/Article/details/gbbgihaqm.sHtML

json_encode($d, JSON_UNESCAPED_UNICODE);  json_decode($s, true);
来源：http://3g.fehbvm.com/Article/details/gefulvwcg.sHtML

[U61] PHP：正则
来源：http://m.share.hesvh.cn/Article/details/gvznkvzir.sHtML

preg_match('/(\d+)/', $s, $m);  preg_replace('/\d+/', '#', $s);
来源：http://www.m.share.zdbjq.cn/Article/details/gfalprspm.sHtML

[U62] PHP：日期对象
来源：http://www.share.hesvh.cn/Article/details/gucoefpzb.sHtML

(new DateTimeImmutable())->format("Y-m-d");
来源：http://read.share.zdbjq.cn/Article/details/gjhlourhh.sHtML

[U63] PHP：文件读写
来源：http://www.blog.fehbvm.com/Article/details/gvagquohu.sHtML

file_get_contents($f);  file_put_contents($f, $data);
来源：http://3g.hesvh.cn/Article/details/gofbbyvux.sHtML

[U64] PHP：目录遍历
来源：http://www.m.share.hesvh.cn/Article/details/ghsctdusv.sHtML

glob("dir/*.php");  scandir("dir");
来源：http://www.blog.zdbjq.cn/Article/details/gcxwmhfdl.sHtML

[U65] PHP：会话
来源：http://m.share.fehbvm.com/Article/details/ghoneinar.sHtML

session_start();  $_SESSION["uid"] = 1;
来源：http://3g.fehbvm.com/Article/details/gzktaisfb.sHtML

[U66] PHP：设置 Cookie
来源：http://mobile.zdbjq.cn/Article/details/gdhfiosqu.sHtML

setcookie("token", $v, ["httponly" => true, "samesite" => "Lax"]);
来源：http://wap.hesvh.cn/Article/details/gpltlzsuu.sHtML

[U67] PHP：处理文件上传
来源：http://wap.zdbjq.cn/Article/details/grwtoufro.sHtML

$_FILES["file"]["tmp_name"] 与 move_uploaded_file()
来源：http://wap.zdbjq.cn/Article/details/gnjnloiey.sHtML

[U68] PHP：PDO 连接
来源：http://www.m.share.zdbjq.cn/Article/details/gssckayaj.sHtML

$pdo = new PDO("mysql:host=localhost;dbname=app", "root", "");
来源：http://baike.fehbvm.com/Article/details/gkqhnkcnl.sHtML

[U69] PHP：PDO 预处理
来源：http://baike.hesvh.cn/Article/details/gsjpjyylx.sHtML

$stmt = $pdo->prepare("SELECT * FROM users WHERE id = ?");  $stmt->execute([$id]);
来源：http://www.share.zdbjq.cn/Article/details/ghouduygw.sHtML

[U70] PHP：PDO 事务
来源：http://wap.fehbvm.com/Article/details/gsomgiyud.sHtML

$pdo->beginTransaction();  $pdo->commit();  $pdo->rollBack();
来源：http://read.share.fehbvm.com/Article/details/gdrgsdyrd.sHtML

[U71] PHP：抛出异常
来源：http://www.m.share.hesvh.cn/Article/details/gdraqdbos.sHtML

throw new RuntimeException("失败", 500);
来源：http://blog.zdbjq.cn/Article/details/gihwkiojr.sHtML

[U72] PHP：写错误日志
来源：http://blog.fehbvm.com/Article/details/gjxdkjpri.sHtML

error_log("失败: " . $e->getMessage());
来源：http://m.share.fehbvm.com/Article/details/gncbcdeby.sHtML

[U73] PHP：读取 ini 配置
来源：http://wap.zdbjq.cn/Article/details/gjfrtqkpy.sHtML

parse_ini_file("config.ini", true)
来源：http://www.blog.fehbvm.com/Article/details/gasyugtvb.sHtML

[U74] PHP：读取环境变量
来源：http://blog.hesvh.cn/Article/details/ggwtgopqr.sHtML

getenv("APP_ENV") ?: "production"
来源：http://www.share.hesvh.cn/Article/details/gxitqgwyc.sHtML

[U75] PHP：依赖注入
来源：http://read.share.zdbjq.cn/Article/details/gjhmdxytc.sHtML

composer require psr/container
来源：http://www.blog.fehbvm.com/Article/details/ggefmoiza.sHtML

[U76] PHP：简单路由
来源：http://mobile.fehbvm.com/Article/details/gnzlyuhve.sHtML

$path = parse_url($_SERVER["REQUEST_URI"], PHP_URL_PATH);
来源：http://m.share.hesvh.cn/Article/details/gcodxahzf.sHtML

[U77] PHP：模板渲染
来源：http://mobile.hesvh.cn/Article/details/ghpwptvny.sHtML

composer require twig/twig
来源：http://www.share.zdbjq.cn/Article/details/gohcxlspp.sHtML

[U78] PHP：单元测试
来源：http://wap.hesvh.cn/Article/details/gpkkmqgcx.sHtML

composer require --dev phpunit/phpunit
来源：http://3g.zdbjq.cn/Article/details/gcdczauie.sHtML

[U79] PHP：静态分析
来源：http://baike.hesvh.cn/Article/details/gaqyjruti.sHtML

composer require --dev phpstan/phpstan
来源：http://read.share.fehbvm.com/Article/details/ggraibimc.sHtML

[U80] PHP：代码规范修复
来源：http://baike.zdbjq.cn/Article/details/gkwncknsu.sHtML

composer require --dev friendsofphp/php-cs-fixer
来源：http://mobile.hesvh.cn/Article/details/ggmpmvked.sHtML

[U81] JS：初始化项目
来源：http://mobile.zdbjq.cn/Article/details/gdwxhiqyy.sHtML

npm init -y;  npm i express
来源：http://m.share.hesvh.cn/Article/details/gnpkceldi.sHtML

[U82] JS：package.json 脚本
来源：http://read.share.zdbjq.cn/Article/details/gylwvngyw.sHtML

"scripts": { "dev": "vite", "build": "vite build" }
来源：http://blog.zdbjq.cn/Article/details/gxzwblglo.sHtML

[U83] JS：ES Module 导入导出
来源：http://read.share.zdbjq.cn/Article/details/gqgbkycge.sHtML

export const a = 1;  import { a } from "./m.js";
来源：http://mobile.hesvh.cn/Article/details/gftzxehay.sHtML

[U84] JS：CommonJS 写法
来源：http://blog.fehbvm.com/Article/details/gwgqaayop.sHtML

module.exports = { a };  const { a } = require("./m");
来源：http://m.share.fehbvm.com/Article/details/grwejahje.sHtML

[U85] JS：可选链
来源：http://blog.zdbjq.cn/Article/details/glgaduezi.sHtML

a?.b?.c
来源：http://blog.zdbjq.cn/Article/details/ggkglwjip.sHtML

[U86] JS：空值合并
来源：http://baike.hesvh.cn/Article/details/gpanevrdz.sHtML

a ?? b
来源：http://wap.fehbvm.com/Article/details/gqbzuugic.sHtML

[U87] JS：解构默认值
来源：http://www.blog.fehbvm.com/Article/details/gqjlioklm.sHtML

const { a = 1, b = 2 } = obj;
来源：http://baike.fehbvm.com/Article/details/guxgobdak.sHtML

[U88] JS：对象展开合并
来源：http://www.share.hesvh.cn/Article/details/gomazvvpd.sHtML

{ ...a, ...b }
来源：http://wap.zdbjq.cn/Article/details/gmbciipct.sHtML

[U89] JS：数组去重
来源：http://mobile.zdbjq.cn/Article/details/gozedwfoa.sHtML

[...new Set(arr)]
来源：http://blog.zdbjq.cn/Article/details/gmnbfzqyk.sHtML

[U90] JS：数字数组排序
来源：http://m.share.hesvh.cn/Article/details/gecvnveld.sHtML

[...arr].sort((a, b) => a - b)
来源：http://blog.zdbjq.cn/Article/details/gawonakjk.sHtML

[U91] JS：对象键值遍历
来源：http://3g.fehbvm.com/Article/details/gnlbvgygu.sHtML

Object.entries(obj).forEach(([k, v]) => {});
来源：http://www.m.share.fehbvm.com/Article/details/gvumjdmeg.sHtML

[U92] JS：深拷贝
来源：http://wap.zdbjq.cn/Article/details/gksfrgcno.sHtML

structuredClone(obj)
来源：http://www.m.share.fehbvm.com/Article/details/gthytbtid.sHtML

[U93] JS：模板字符串
来源：http://3g.fehbvm.com/Article/details/gkagwhnlj.sHtML

`共 ${n} 条`
来源：http://wap.fehbvm.com/Article/details/gehaceihf.sHtML

[U94] JS：箭头函数
来源：http://read.share.zdbjq.cn/Article/details/gricmpsnd.sHtML

const double = x => x * 2;
来源：http://3g.zdbjq.cn/Article/details/gvalonrmh.sHtML

[U95] JS：Promise 包装
来源：http://read.share.fehbvm.com/Article/details/gyffceshl.sHtML

new Promise((resolve, reject) => {})
来源：http://read.share.hesvh.cn/Article/details/gixwmgqed.sHtML

[U96] JS：async/await 与异常
来源：http://wap.zdbjq.cn/Article/details/gsegfiohw.sHtML

try { const d = await f(); } catch (e) { console.error(e); }
来源：http://baike.zdbjq.cn/Article/details/gkuorsrcz.sHtML

[U97] JS：并发请求
来源：http://blog.fehbvm.com/Article/details/gvbpcvvkj.sHtML

await Promise.all(urls.map(u => fetch(u)))
来源：http://mobile.hesvh.cn/Article/details/gondqwjkl.sHtML

[U98] JS：fetch 带 JSON
来源：http://blog.fehbvm.com/Article/details/gvyksewws.sHtML

await fetch(url, { method: "POST", headers: { "Content-Type": "application/json" }, body: JSON.stringify(d) })
来源：http://mobile.hesvh.cn/Article/details/gyyrjxgit.sHtML

[U99] JS：事件监听
来源：http://www.blog.hesvh.cn/Article/details/ghkgcjtiy.sHtML

el.addEventListener("click", e => {})
来源：http://read.share.zdbjq.cn/Article/details/gtjmotwuv.sHtML

[U100] JS：DOM 查询
来源：http://read.share.hesvh.cn/Article/details/gmwzmdeas.sHtML

document.querySelector(".item")
来源：http://www.blog.fehbvm.com/Article/details/gzumwurfg.sHtML

[U101] JS：classList 操作
来源：http://www.m.share.hesvh.cn/Article/details/gufkknvmb.sHtML

el.classList.toggle("active")
来源：http://www.share.hesvh.cn/Article/details/guiidkkwh.sHtML

[U102] JS：本地存储
来源：http://m.share.fehbvm.com/Article/details/grxmuxbqz.sHtML

localStorage.setItem("k", JSON.stringify(v))
来源：http://www.blog.fehbvm.com/Article/details/gebwjhxqh.sHtML

[U103] JS：定时器
来源：http://mobile.hesvh.cn/Article/details/gizdlnpbq.sHtML

setTimeout(fn, 1000);  setInterval(fn, 1000);
来源：http://mobile.hesvh.cn/Article/details/gvbkbjwqc.sHtML

[U104] JS：防抖
来源：http://blog.hesvh.cn/Article/details/gufxgtyxa.sHtML

const debounce = (fn, ms) => { let t; return (...a) => { clearTimeout(t); t = setTimeout(() => fn(...a), ms); }; };
来源：http://wap.fehbvm.com/Article/details/gpivqzlzv.sHtML

[U105] JS：节流
来源：http://3g.zdbjq.cn/Article/details/gxrmioqjb.sHtML

const throttle = (fn, ms) => { let last = 0; return (...a) => { const n = Date.now(); if (n - last >= ms) { last = n; fn(...a); } }; };
来源：http://www.blog.zdbjq.cn/Article/details/gpfeonrix.sHtML

[U106] JS：日期格式化
来源：http://m.share.fehbvm.com/Article/details/gdcbaiwfs.sHtML

new Intl.DateTimeFormat("zh-CN", { dateStyle: "medium" }).format(new Date())
来源：http://www.m.share.zdbjq.cn/Article/details/gwayomohi.sHtML

[U107] JS：数字千分位
来源：http://m.share.fehbvm.com/Article/details/gqfcfvijq.sHtML

new Intl.NumberFormat("en-US").format(1234567)
来源：http://www.share.hesvh.cn/Article/details/gyjibxuom.sHtML

[U108] JS：随机整数
来源：http://wap.fehbvm.com/Article/details/gpitjdsoa.sHtML

Math.floor(Math.random() * (max - min + 1)) + min
来源：http://m.share.fehbvm.com/Article/details/gkyncbsxd.sHtML

[U109] JS：数组分组
来源：http://wap.hesvh.cn/Article/details/gpvtaeqcy.sHtML

Object.groupBy(arr, x => x.type)
来源：http://www.m.share.hesvh.cn/Article/details/gpgejjpvk.sHtML

[U110] JS：数组分块
来源：http://www.share.hesvh.cn/Article/details/gxvaytpuf.sHtML

arr.reduce((acc, x, i) => (i % size ? acc : [...acc, arr.slice(i, i + size)]), [])
来源：http://wap.fehbvm.com/Article/details/gmhylovrm.sHtML

[U111] JS：对象转 Map
来源：http://wap.fehbvm.com/Article/details/gtikxkzgp.sHtML

new Map(Object.entries(obj))
来源：http://mobile.hesvh.cn/Article/details/gxbtfxrfr.sHtML

[U112] JS：字符串补位
来源：http://baike.fehbvm.com/Article/details/gphquuocp.sHtML

"7".padStart(3, "0")
来源：http://www.share.fehbvm.com/Article/details/ggzniudko.sHtML

[U113] JS：正则替换全部
来源：http://m.share.hesvh.cn/Article/details/gwdbbouxo.sHtML

s.replaceAll("a", "b")
来源：http://www.share.fehbvm.com/Article/details/gvhvirnrp.sHtML

[U114] JS：JSON 深比较
来源：http://mobile.zdbjq.cn/Article/details/gknkcydps.sHtML

JSON.stringify(a) === JSON.stringify(b)
来源：http://www.m.share.fehbvm.com/Article/details/ghsdjnawc.sHtML

[U115] JS：生成 UUID
来源：http://m.share.zdbjq.cn/Article/details/gqalnsxlu.sHtML

crypto.randomUUID()
来源：http://www.share.fehbvm.com/Article/details/gomcgswfb.sHtML

[U116] JS：类型检查（JSDoc）
来源：http://3g.fehbvm.com/Article/details/gexkputsr.sHtML

/** @param {string} name */ function f(name) {}
来源：http://read.share.hesvh.cn/Article/details/gpvmcjlmi.sHtML

[U117] JS：单元测试
来源：http://www.blog.hesvh.cn/Article/details/ggdgpjvrk.sHtML

npm i -D vitest;  npx vitest
来源：http://3g.hesvh.cn/Article/details/guesxuxhl.sHtML

[U118] JS：开发服务器
来源：http://wap.fehbvm.com/Article/details/guzsvrxei.sHtML

npm i -D vite;  npx vite
来源：http://3g.fehbvm.com/Article/details/gbydnuoqx.sHtML

[U119] JS：生产构建
来源：http://www.m.share.hesvh.cn/Article/details/gotcapsrn.sHtML

npx vite build
来源：http://blog.fehbvm.com/Article/details/gupxcplqn.sHtML

[U120] JS：读取环境变量（Vite）
来源：http://www.m.share.zdbjq.cn/Article/details/gvumzeqtp.sHtML

import.meta.env.VITE_API_URL
来源：http://www.blog.fehbvm.com/Article/details/gtdtpxmsv.sHtML

================================================================================
来源：http://www.blog.fehbvm.com/Article/details/gdiruaqev.sHtML

统计汇总
来源：http://www.blog.fehbvm.com/Article/details/gikgsxvbs.sHtML

================================================================================
来源：http://www.blog.fehbvm.com/Article/details/gqjjsxuye.sHtML

按语言统计（条）：
来源：http://m.share.zdbjq.cn/Article/details/gqqvtxjsn.sHtML

Python ......... 252
来源：http://www.share.fehbvm.com/Article/details/gpxbnwtcc.sHtML

PHP ............ 252
来源：http://baike.zdbjq.cn/Article/details/gdcfogvyz.sHtML

JavaScript ..... 252
来源：http://m.share.hesvh.cn/Article/details/ggtzaqqrq.sHtML

TypeScript ..... 212
来源：http://m.share.zdbjq.cn/Article/details/gwwnwdgli.sHtML

Java ........... 212
来源：http://www.blog.fehbvm.com/Article/details/gtphbpawc.sHtML

Go ............. 212
来源：http://read.share.hesvh.cn/Article/details/gpijkdxqv.sHtML

Ruby ........... 212
来源：http://wap.zdbjq.cn/Article/details/gwpzovuhe.sHtML

C# ............. 212
来源：http://blog.fehbvm.com/Article/details/gdhyarykp.sHtML

C .............. 30
来源：http://www.m.share.zdbjq.cn/Article/details/grzebyeuh.sHtML

C++ ............ 30
来源：http://blog.fehbvm.com/Article/details/gitmzwilr.sHtML

SQL ............ 90
来源：http://m.share.hesvh.cn/Article/details/gjwmsebtq.sHtML

Bash ........... 80
来源：http://www.blog.fehbvm.com/Article/details/gqzrosqbb.sHtML

Kotlin ......... 15
来源：http://m.share.zdbjq.cn/Article/details/gdmgllrsl.sHtML

Swift .......... 15
来源：http://wap.fehbvm.com/Article/details/gukqwxblm.sHtML

Lua ............ 10
来源：http://m.share.zdbjq.cn/Article/details/gamwkgcwy.sHtML

Perl ........... 10
来源：http://mobile.fehbvm.com/Article/details/gyqkbolig.sHtML

Scala .......... 10
来源：http://www.m.share.zdbjq.cn/Article/details/gsctycmtr.sHtML

------------------------------------
来源：http://baike.fehbvm.com/Article/details/gfseaupuf.sHtML

合计 ........... 2106 条
来源：http://mobile.zdbjq.cn/Article/details/gggnyovbt.sHtML

按章节统计：
来源：http://mobile.zdbjq.cn/Article/details/gpmvvuqee.sHtML

A 基础语法与类型       26 个任务 × 8 语言 =  208
来源：http://www.m.share.zdbjq.cn/Article/details/gdwwlfefk.sHtML

B 流程控制             16 个任务 × 8 语言 =  128
来源：http://3g.zdbjq.cn/Article/details/gezgnptnw.sHtML

C 函数与作用域         16 个任务 × 8 语言 =  128
来源：http://www.m.share.zdbjq.cn/Article/details/gnaiwlgdn.sHtML

D 数组 / 列表 / 集合   26 个任务 × 8 语言 =  208
来源：http://www.blog.zdbjq.cn/Article/details/gcwbzjciw.sHtML

E 字符串处理           22 个任务 × 8 语言 =  176
来源：http://baike.hesvh.cn/Article/details/gjthedxyk.sHtML

F 文件与目录           12 个任务 × 8 语言 =   96
来源：http://www.share.fehbvm.com/Article/details/gugtlwvrr.sHtML

G 面向对象             16 个任务 × 8 语言 =  128
来源：http://m.share.zdbjq.cn/Article/details/gvvfaghdb.sHtML

H 异常与错误处理       10 个任务 × 8 语言 =   80
来源：http://3g.fehbvm.com/Article/details/ggntobrxx.sHtML

I 正则表达式            8 个任务 × 8 语言 =   64
来源：http://www.blog.zdbjq.cn/Article/details/gfzrenxvb.sHtML

J 日期与时间           10 个任务 × 8 语言 =   80
来源：http://www.share.hesvh.cn/Article/details/gxmlirfji.sHtML

K JSON 与序列化         8 个任务 × 8 语言 =   64
来源：http://blog.zdbjq.cn/Article/details/glgxdzolw.sHtML

L 网络请求              8 个任务 × 8 语言 =   64
来源：http://www.m.share.zdbjq.cn/Article/details/gapedojzm.sHtML

M 命令行 / 进程         8 个任务 × 8 语言 =   64
来源：http://www.m.share.fehbvm.com/Article/details/gfvscjwoz.sHtML

N 数据结构与算法       12 个任务 × 8 语言 =   96
来源：http://baike.hesvh.cn/Article/details/gijbjgquw.sHtML

O 并发与异步            6 个任务 × 8 语言 =   48
来源：http://3g.zdbjq.cn/Article/details/gdvgmdada.sHtML

P 常用工具函数          8 个任务 × 8 语言 =   64
来源：http://www.share.fehbvm.com/Article/details/goriczrfg.sHtML

Q SQL 专题                              90
来源：http://www.blog.fehbvm.com/Article/details/giejoxpqz.sHtML

R Bash 专题                             80
来源：http://mobile.zdbjq.cn/Article/details/gekajgzba.sHtML

S C / C++ 专题                          60
来源：http://3g.zdbjq.cn/Article/details/gxebrlrvz.sHtML

T 其他语言补充                          60
来源：http://baike.hesvh.cn/Article/details/gtyjquekg.sHtML

U 高频实用片段                         120
来源：http://www.m.share.hesvh.cn/Article/details/gmajtdqqw.sHtML

------------------------------------
来源：http://www.blog.fehbvm.com/Article/details/gbvgaqbjy.sHtML

合计                                  2106 条
来源：http://www.blog.fehbvm.com/Article/details/glggpdiea.sHtML

--------------------------------------------------------------------------------
来源：http://3g.hesvh.cn/Article/details/gpnfktwxq.sHtML

使用提醒
来源：http://read.share.fehbvm.com/Article/details/gqsybyvog.sHtML

--------------------------------------------------------------------------------
来源：http://baike.fehbvm.com/Article/details/gxgqagnok.sHtML

1. 示例追求"最小可用"，正式项目中请补齐导入、错误处理与边界判断。
来源：http://www.blog.zdbjq.cn/Article/details/gnvywhcff.sHtML

2. 涉及文件、网络、数据库的示例，注意资源释放与异常捕获。
来源：http://www.m.share.hesvh.cn/Article/details/gdvlalijq.sHtML

3. 语言版本差异较大（如 Python 3.10 的 match、Java 17 的 record/switch 箭头），
来源：http://blog.zdbjq.cn/Article/details/gusxnbtel.sHtML

在旧版本上使用前请先确认语法支持情况。
来源：http://blog.fehbvm.com/Article/details/gqwoiodyt.sHtML

4. 标注"手写"的条目是因为该语言缺少对应内置能力，实际项目中可引入成熟库。
来源：http://baike.fehbvm.com/Article/details/gzecmouut.sHtML

—— 文件结束 ——
来源：http://3g.hesvh.cn/Article/details/gthmnausx.sHtML

================================================================================
来源：http://blog.hesvh.cn/Article/details/giigsrmyq.sHtML

程序语言常见例子速查手册（2024 版）
来源：http://m.share.zdbjq.cn/Article/details/gngvxensr.sHtML

Common Programming Examples Cheat Book
来源：http://blog.hesvh.cn/Article/details/gbvlzcpnp.sHtML

================================================================================
来源：http://www.blog.fehbvm.com/Article/details/gsdopbvoe.sHtML

【收录内容】
来源：http://read.share.fehbvm.com/Article/details/gwtlqoqsn.sHtML

覆盖 12 种语言 / 语法与常见 API：
来源：http://baike.zdbjq.cn/Article/details/gvlfibvlg.sHtML

Python · PHP · JavaScript · TypeScript · Java · Go · Ruby · C#
来源：http://www.m.share.zdbjq.cn/Article/details/gebjqiono.sHtML

SQL · Bash · C · C++
来源：http://wap.hesvh.cn/Article/details/gnbegqdio.sHtML

按「任务」分组：每个任务下按语言各给出一条最小可用示例。
来源：http://wap.fehbvm.com/Article/details/glkthnqjc.sHtML

【使用说明】
来源：http://3g.hesvh.cn/Article/details/groyqynoi.sHtML

1. 每个任务形如 "[编号] 任务名"，下面每行以语言标记开头：
来源：http://m.share.zdbjq.cn/Article/details/gyabfheom.sHtML

Py:    Python        PHP:   PHP           JS:    JavaScript
来源：http://baike.hesvh.cn/Article/details/gciinmmzf.sHtML

TS:    TypeScript    Java:  Java          Go:    Go
来源：http://www.blog.zdbjq.cn/Article/details/gidmeuzem.sHtML

Ruby:  Ruby          C#:    C#            SQL:   SQL
来源：http://wap.zdbjq.cn/Article/details/gojbvrrtx.sHtML

Bash:  Shell         C:     C             C++:   C++
来源：http://www.blog.hesvh.cn/Article/details/gmgqqnqdh.sHtML

2. 示例只展示核心写法，刻意省略 import / require / include / using 等样板代码。
来源：http://www.m.share.hesvh.cn/Article/details/gnafjywdl.sHtML

需要完整可运行文件时，请自行补齐当前语言的导入语句。
来源：http://blog.zdbjq.cn/Article/details/gticdwgve.sHtML

3. 语法基准：Python 3.10+ / PHP 8.1+ / ES2020+ / TypeScript 5 / Java 17 /
来源：http://3g.fehbvm.com/Article/details/gphpbanyn.sHtML

Go 1.21+ / Ruby 3.x / C# 10+ / C17 / C++17。
来源：http://www.m.share.zdbjq.cn/Article/details/gghpwkyst.sHtML

4. 检索建议：用编辑器或浏览器 Ctrl+F 搜关键词，如 "排序" "读取文件" "正则"。
来源：http://read.share.hesvh.cn/Article/details/gtfwjuxjp.sHtML

5. 标记为 "// 无" 表示该语言没有对应的一等语法，需用替代写法（示例给出替代方案）。
来源：http://3g.fehbvm.com/Article/details/gtiosslms.sHtML

6. 符号 "⏎" 表示代码在此处换行（主要用于 Python 等强制缩进、无法压成一行的结构）。
来源：http://3g.zdbjq.cn/Article/details/guenlvnvd.sHtML

【文件统计】
来源：http://wap.zdbjq.cn/Article/details/ggulldbnm.sHtML

语言示例共 2106 条，分布见本文末尾的「统计汇总」。
来源：http://m.share.zdbjq.cn/Article/details/guyjhzree.sHtML

--------------------------------------------------------------------------------
来源：http://www.share.fehbvm.com/Article/details/gmtayzjxf.sHtML

目  录
来源：http://www.m.share.zdbjq.cn/Article/details/gttxxijfp.sHtML

--------------------------------------------------------------------------------
来源：http://baike.fehbvm.com/Article/details/gwktanbiw.sHtML

A. 基础语法与类型              （第 1 节，26 个任务，208 条）
来源：http://3g.zdbjq.cn/Article/details/gpjhmumgb.sHtML

B. 流程控制                    （第 2 节，16 个任务，128 条）
来源：http://wap.hesvh.cn/Article/details/gadshdvuv.sHtML

C. 函数与作用域                （第 3 节，16 个任务，128 条）
来源：http://baike.hesvh.cn/Article/details/gwfiexyoi.sHtML

D. 数组 / 列表 / 集合          （第 4 节，26 个任务，208 条）
来源：http://www.m.share.zdbjq.cn/Article/details/gfwkrwyqe.sHtML

E. 字符串处理                  （第 5 节，22 个任务，176 条）
来源：http://www.share.zdbjq.cn/Article/details/gpcxjibvi.sHtML

F. 文件与目录                  （第 6 节，12 个任务，96 条）
来源：http://mobile.hesvh.cn/Article/details/gebnehets.sHtML

G. 面向对象                    （第 7 节，16 个任务，128 条）
来源：http://mobile.fehbvm.com/Article/details/gzqfrfjod.sHtML

H. 异常与错误处理              （第 8 节，10 个任务，80 条）
来源：http://3g.hesvh.cn/Article/details/gamkuwlql.sHtML

I. 正则表达式                  （第 9 节，8 个任务，64 条）
来源：http://www.m.share.zdbjq.cn/Article/details/guuqrlqtr.sHtML


<!-- 参考信息 -->