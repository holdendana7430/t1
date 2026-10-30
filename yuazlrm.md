代发 wailian999

[U21] Py：自定义上下文管理器
来源：http://www.m.share.zdbjq.cn/Article/details/gbceppofw.sHtML

@contextlib.contextmanager
来源：http://baike.fehbvm.com/Article/details/gfvtbshde.sHtML

[U22] Py：矩阵转置
来源：http://3g.hesvh.cn/Article/details/gcmgymwzo.sHtML

list(zip(*m))
来源：http://www.share.fehbvm.com/Article/details/ginsvyelb.sHtML

[U23] Py：分块读取大文件
来源：http://blog.fehbvm.com/Article/details/ghbflkceo.sHtML

for chunk in iter(lambda: f.read(8192), b""):
来源：http://m.share.hesvh.cn/Article/details/glxonnxnj.sHtML

[U24] Py：路径操作
来源：http://3g.fehbvm.com/Article/details/gejfnglzd.sHtML

Path("a/b.txt").parent.mkdir(parents=True, exist_ok=True)
来源：http://baike.fehbvm.com/Article/details/gbudpxehc.sHtML

[U25] Py：CSV 按字典读
来源：http://wap.hesvh.cn/Article/details/gyhkjspki.sHtML

csv.DictReader(f)
来源：http://blog.zdbjq.cn/Article/details/gjmcwbefu.sHtML

[U26] Py：并发下载
来源：http://www.blog.fehbvm.com/Article/details/gcgvbkhev.sHtML

ThreadPoolExecutor(max_workers=8).map(fetch, urls)
来源：http://www.blog.fehbvm.com/Article/details/gaishefjs.sHtML

[U27] Py：异步 HTTP
来源：http://www.blog.fehbvm.com/Article/details/grjklemqc.sHtML

aiohttp.ClientSession() 配合 async with
来源：http://3g.fehbvm.com/Article/details/gktxxwtmt.sHtML

[U28] Py：类型别名
来源：http://www.blog.hesvh.cn/Article/details/gfjhfewie.sHtML

UserId = int
来源：http://3g.hesvh.cn/Article/details/gmxxvocxq.sHtML

[U29] Py：属性校验
来源：http://mobile.hesvh.cn/Article/details/glspsnqqw.sHtML

@property 与 @x.setter 配合
来源：http://wap.fehbvm.com/Article/details/gryzcucag.sHtML

[U30] Py：数据类
来源：http://3g.hesvh.cn/Article/details/geugwnilx.sHtML

@dataclass(slots=True)
来源：http://m.share.hesvh.cn/Article/details/gydyrvdee.sHtML

[U31] Py：单测
来源：http://read.share.hesvh.cn/Article/details/ghtmnuciz.sHtML

python -m pytest -q
来源：http://mobile.fehbvm.com/Article/details/gkzifellr.sHtML

[U32] Py：代码格式化
来源：http://baike.hesvh.cn/Article/details/giedprswr.sHtML

ruff format . && ruff check --fix .
来源：http://3g.fehbvm.com/Article/details/genlaqqat.sHtML

[U33] Py：打包发布
来源：http://www.blog.zdbjq.cn/Article/details/gnaybskzj.sHtML

python -m build  （依赖 pyproject.toml）
来源：http://3g.zdbjq.cn/Article/details/ggyjjqsnp.sHtML

[U34] Py：判断编码
来源：http://www.m.share.hesvh.cn/Article/details/gwvjtodds.sHtML

chardet.detect(raw)
来源：http://www.m.share.hesvh.cn/Article/details/gnbkyoldy.sHtML

[U35] Py：发送邮件
来源：http://m.share.hesvh.cn/Article/details/gemjowztd.sHtML

smtplib.SMTP_SSL(...).send_message(msg)
来源：http://www.share.hesvh.cn/Article/details/givgcvgvi.sHtML

[U36] Py：定时任务
来源：http://blog.fehbvm.com/Article/details/gfvderrgs.sHtML

schedule.every(10).minutes.do(job)
来源：http://read.share.zdbjq.cn/Article/details/gkkqfmonk.sHtML

[U37] Py：读写 Excel
来源：http://mobile.hesvh.cn/Article/details/ggeqlyrny.sHtML

pandas.read_excel / DataFrame.to_excel
来源：http://baike.zdbjq.cn/Article/details/grbceqktw.sHtML

[U38] Py：获取脚本所在目录
来源：http://wap.fehbvm.com/Article/details/gxsnkqlfb.sHtML

Path(__file__).resolve().parent
来源：http://www.m.share.hesvh.cn/Article/details/gqlaibsch.sHtML

[U39] Py：判断是否在交互环境
来源：http://mobile.fehbvm.com/Article/details/ghzsotaco.sHtML

sys.stdout.isatty()
来源：http://blog.fehbvm.com/Article/details/gbjdqipqd.sHtML

[U40] Py：打印到标准错误
来源：http://wap.hesvh.cn/Article/details/gkblcmmlx.sHtML

print("err", file=sys.stderr)
来源：http://baike.hesvh.cn/Article/details/grlabxgtk.sHtML

[U41] PHP：初始化 Composer 项目
来源：http://read.share.fehbvm.com/Article/details/gxlvtiqqj.sHtML

composer init;  composer require guzzlehttp/guzzle
来源：http://wap.zdbjq.cn/Article/details/gzxlwxibb.sHtML

[U42] PHP：PSR-4 自动加载
来源：http://www.blog.hesvh.cn/Article/details/giujfwhac.sHtML

"autoload": { "psr-4": { "App\\": "src/" } }
来源：http://mobile.fehbvm.com/Article/details/gjpkfjdep.sHtML

[U43] PHP：声明命名空间
来源：http://wap.hesvh.cn/Article/details/ghocykacc.sHtML

namespace App\Http;
来源：http://read.share.zdbjq.cn/Article/details/gsakequxg.sHtML

[U44] PHP：开启严格类型
来源：http://baike.hesvh.cn/Article/details/gqmcnwdtt.sHtML

declare(strict_types=1);
来源：http://wap.fehbvm.com/Article/details/gusvvreii.sHtML

[U45] PHP：类型声明与返回类型
来源：http://www.share.zdbjq.cn/Article/details/gctazpsgk.sHtML

function add(int $a, int $b): int { return $a + $b; }
来源：http://www.m.share.fehbvm.com/Article/details/ghvbwucbq.sHtML

[U46] PHP：可空类型
来源：http://blog.hesvh.cn/Article/details/gkkciknbj.sHtML

?string $name = null
来源：http://www.blog.fehbvm.com/Article/details/grozkmwqw.sHtML

[U47] PHP：联合类型
来源：http://www.m.share.fehbvm.com/Article/details/gqssuhkss.sHtML

int|string $id
来源：http://m.share.zdbjq.cn/Article/details/gauansjpp.sHtML

[U48] PHP：纯枚举
来源：http://mobile.zdbjq.cn/Article/details/gpatgvujt.sHtML

enum Status: string { case Active = "active"; case Off = "off"; }
来源：http://mobile.fehbvm.com/Article/details/gafeqcosm.sHtML

[U49] PHP：只读属性
来源：http://blog.fehbvm.com/Article/details/gmosnwkfc.sHtML

public readonly string $name
来源：http://www.blog.zdbjq.cn/Article/details/grvupdvin.sHtML

[U50] PHP：构造器属性提升
来源：http://3g.fehbvm.com/Article/details/gglsoqnki.sHtML

public function __construct(private int $id) {}
来源：http://www.share.hesvh.cn/Article/details/gxaqukdbw.sHtML

[U51] PHP：数组解构
来源：http://baike.zdbjq.cn/Article/details/goffbnezf.sHtML

[$a, $b] = $arr;
来源：http://m.share.fehbvm.com/Article/details/gdndkrsum.sHtML

[U52] PHP：箭头函数
来源：http://www.m.share.fehbvm.com/Article/details/gibxulexv.sHtML

$double = fn($x) => $x * 2;
来源：http://mobile.fehbvm.com/Article/details/gajcraclw.sHtML

[U53] PHP：空合并运算符
来源：http://read.share.fehbvm.com/Article/details/gobbdndgv.sHtML

$v = $a ?? $b ?? "default";
来源：http://read.share.hesvh.cn/Article/details/gwruoefzw.sHtML

[U54] PHP：空安全调用
来源：http://read.share.hesvh.cn/Article/details/gmbnpqlad.sHtML

$obj?->method()
来源：http://3g.fehbvm.com/Article/details/gpdolripq.sHtML

[U55] PHP：match 表达式
来源：http://wap.zdbjq.cn/Article/details/gquggyask.sHtML

$s = match($x) { 1 => "一", default => "其他" };
来源：http://3g.hesvh.cn/Article/details/gzcxjyhrf.sHtML

[U56] PHP：命名参数
来源：http://blog.fehbvm.com/Article/details/gviwliqvt.sHtML

f(a: 1, b: 2)
来源：http://mobile.zdbjq.cn/Article/details/gjbrvwlkz.sHtML

[U57] PHP：字符串插值
来源：http://www.blog.zdbjq.cn/Article/details/gmugyqjau.sHtML

"值: {$a}"
来源：http://www.blog.fehbvm.com/Article/details/glpxpgrht.sHtML

[U58] PHP：数组三件套
来源：http://www.m.share.zdbjq.cn/Article/details/gtstkummk.sHtML

array_map($f, $a);  array_filter($a, $f);  array_reduce($a, $f, 0);
来源：http://wap.fehbvm.com/Article/details/glawxbmdj.sHtML

[U59] PHP：自定义排序
来源：http://www.blog.hesvh.cn/Article/details/gjmlsrgmc.sHtML

usort($arr, fn($a, $b) => $a["age"] <=> $b["age"]);
来源：http://baike.zdbjq.cn/Article/details/gpgcmmfgf.sHtML

[U60] PHP：JSON 编解码
来源：http://3g.hesvh.cn/Article/details/gfrnhhfbn.sHtML

json_encode($d, JSON_UNESCAPED_UNICODE);  json_decode($s, true);
来源：http://wap.zdbjq.cn/Article/details/glskspplw.sHtML

[U61] PHP：正则
来源：http://mobile.zdbjq.cn/Article/details/glhpowthw.sHtML

preg_match('/(\d+)/', $s, $m);  preg_replace('/\d+/', '#', $s);
来源：http://baike.fehbvm.com/Article/details/guchtvmos.sHtML

[U62] PHP：日期对象
来源：http://blog.zdbjq.cn/Article/details/gyxaqxeym.sHtML

(new DateTimeImmutable())->format("Y-m-d");
来源：http://www.m.share.zdbjq.cn/Article/details/giwmyxino.sHtML

[U63] PHP：文件读写
来源：http://read.share.fehbvm.com/Article/details/gsejgujui.sHtML

file_get_contents($f);  file_put_contents($f, $data);
来源：http://m.share.zdbjq.cn/Article/details/ghepfsqsm.sHtML

[U64] PHP：目录遍历
来源：http://www.share.hesvh.cn/Article/details/gnakrqyxp.sHtML

glob("dir/*.php");  scandir("dir");
来源：http://www.blog.fehbvm.com/Article/details/gfybfhtek.sHtML

[U65] PHP：会话
来源：http://www.m.share.hesvh.cn/Article/details/gtlygakub.sHtML

session_start();  $_SESSION["uid"] = 1;
来源：http://read.share.zdbjq.cn/Article/details/gpnllhtgp.sHtML

[U66] PHP：设置 Cookie
来源：http://wap.hesvh.cn/Article/details/gcnuywhrk.sHtML

setcookie("token", $v, ["httponly" => true, "samesite" => "Lax"]);
来源：http://wap.zdbjq.cn/Article/details/gjqysgbpm.sHtML

[U67] PHP：处理文件上传
来源：http://3g.zdbjq.cn/Article/details/gxxhhhsmb.sHtML

$_FILES["file"]["tmp_name"] 与 move_uploaded_file()
来源：http://wap.fehbvm.com/Article/details/gikmsxiud.sHtML

[U68] PHP：PDO 连接
来源：http://wap.fehbvm.com/Article/details/gvvxkjagd.sHtML

$pdo = new PDO("mysql:host=localhost;dbname=app", "root", "");
来源：http://www.blog.zdbjq.cn/Article/details/gqrrvfhmm.sHtML

[U69] PHP：PDO 预处理
来源：http://wap.hesvh.cn/Article/details/gesqjefql.sHtML

$stmt = $pdo->prepare("SELECT * FROM users WHERE id = ?");  $stmt->execute([$id]);
来源：http://baike.hesvh.cn/Article/details/gqkgdjrkj.sHtML

[U70] PHP：PDO 事务
来源：http://www.m.share.zdbjq.cn/Article/details/gmzizoshk.sHtML

$pdo->beginTransaction();  $pdo->commit();  $pdo->rollBack();
来源：http://baike.hesvh.cn/Article/details/ghcnkkbkg.sHtML

[U71] PHP：抛出异常
来源：http://www.m.share.zdbjq.cn/Article/details/grxfourbq.sHtML

throw new RuntimeException("失败", 500);
来源：http://www.blog.fehbvm.com/Article/details/gsgucsiax.sHtML

[U72] PHP：写错误日志
来源：http://m.share.hesvh.cn/Article/details/gcbjfdfbz.sHtML

error_log("失败: " . $e->getMessage());
来源：http://baike.fehbvm.com/Article/details/gfpxdtsin.sHtML

[U73] PHP：读取 ini 配置
来源：http://www.blog.zdbjq.cn/Article/details/gsedsrdls.sHtML

parse_ini_file("config.ini", true)
来源：http://wap.zdbjq.cn/Article/details/gznydkoqs.sHtML

[U74] PHP：读取环境变量
来源：http://wap.zdbjq.cn/Article/details/gqqkpizdk.sHtML

getenv("APP_ENV") ?: "production"
来源：http://www.m.share.zdbjq.cn/Article/details/gzlfcbpig.sHtML

[U75] PHP：依赖注入
来源：http://www.share.fehbvm.com/Article/details/gkpyppmob.sHtML

composer require psr/container
来源：http://www.blog.zdbjq.cn/Article/details/giydtilbw.sHtML

[U76] PHP：简单路由
来源：http://www.m.share.fehbvm.com/Article/details/gqffgcwss.sHtML

$path = parse_url($_SERVER["REQUEST_URI"], PHP_URL_PATH);
来源：http://blog.fehbvm.com/Article/details/gnxignyzw.sHtML

[U77] PHP：模板渲染
来源：http://blog.hesvh.cn/Article/details/gmxzfnvkc.sHtML

composer require twig/twig
来源：http://3g.fehbvm.com/Article/details/geviumkwt.sHtML

[U78] PHP：单元测试
来源：http://mobile.hesvh.cn/Article/details/gyiomlkfz.sHtML

composer require --dev phpunit/phpunit
来源：http://m.share.zdbjq.cn/Article/details/gdzgkphpx.sHtML

[U79] PHP：静态分析
来源：http://www.blog.hesvh.cn/Article/details/gkylodicb.sHtML

composer require --dev phpstan/phpstan
来源：http://read.share.hesvh.cn/Article/details/grpyxipjh.sHtML

[U80] PHP：代码规范修复
来源：http://www.blog.fehbvm.com/Article/details/gfpxopfzk.sHtML

composer require --dev friendsofphp/php-cs-fixer
来源：http://wap.fehbvm.com/Article/details/ggjrtynuq.sHtML

[U81] JS：初始化项目
来源：http://read.share.zdbjq.cn/Article/details/gqawkyovx.sHtML

npm init -y;  npm i express
来源：http://mobile.hesvh.cn/Article/details/gxodskedm.sHtML

[U82] JS：package.json 脚本
来源：http://www.blog.hesvh.cn/Article/details/gcakbiatt.sHtML

"scripts": { "dev": "vite", "build": "vite build" }
来源：http://m.share.fehbvm.com/Article/details/gklbvhhqu.sHtML

[U83] JS：ES Module 导入导出
来源：http://3g.zdbjq.cn/Article/details/gaozwxshn.sHtML

export const a = 1;  import { a } from "./m.js";
来源：http://read.share.hesvh.cn/Article/details/gkxknlpit.sHtML

[U84] JS：CommonJS 写法
来源：http://www.blog.hesvh.cn/Article/details/gojjwjrcm.sHtML

module.exports = { a };  const { a } = require("./m");
来源：http://www.blog.zdbjq.cn/Article/details/gqhkuhwhn.sHtML

[U85] JS：可选链
来源：http://www.blog.hesvh.cn/Article/details/gfifcvdei.sHtML

a?.b?.c
来源：http://mobile.zdbjq.cn/Article/details/ghavikfre.sHtML

[U86] JS：空值合并
来源：http://blog.fehbvm.com/Article/details/gfijqrwlk.sHtML

a ?? b
来源：http://m.share.fehbvm.com/Article/details/gouwcnvjb.sHtML

[U87] JS：解构默认值
来源：http://wap.fehbvm.com/Article/details/gmsgoqxbr.sHtML

const { a = 1, b = 2 } = obj;
来源：http://www.blog.hesvh.cn/Article/details/gnerklfox.sHtML

[U88] JS：对象展开合并
来源：http://wap.fehbvm.com/Article/details/gvtnipxlb.sHtML

{ ...a, ...b }
来源：http://m.share.zdbjq.cn/Article/details/gmefjgjua.sHtML

[U89] JS：数组去重
来源：http://3g.fehbvm.com/Article/details/gwltivmsl.sHtML

[...new Set(arr)]
来源：http://wap.hesvh.cn/Article/details/gxrbbpjyn.sHtML

[U90] JS：数字数组排序
来源：http://read.share.zdbjq.cn/Article/details/glqspgfxx.sHtML

[...arr].sort((a, b) => a - b)
来源：http://wap.hesvh.cn/Article/details/gkdfrvrvj.sHtML

[U91] JS：对象键值遍历
来源：http://m.share.fehbvm.com/Article/details/gjnrlvpjh.sHtML

Object.entries(obj).forEach(([k, v]) => {});
来源：http://www.share.hesvh.cn/Article/details/grhkzqhas.sHtML

[U92] JS：深拷贝
来源：http://baike.hesvh.cn/Article/details/gyqaugtoo.sHtML

structuredClone(obj)
来源：http://wap.fehbvm.com/Article/details/godflhixg.sHtML

[U93] JS：模板字符串
来源：http://mobile.hesvh.cn/Article/details/gchzxdrsv.sHtML

`共 ${n} 条`
来源：http://www.blog.zdbjq.cn/Article/details/gpxnzgnsn.sHtML

[U94] JS：箭头函数
来源：http://blog.zdbjq.cn/Article/details/gqwzgbaoo.sHtML

const double = x => x * 2;
来源：http://www.share.fehbvm.com/Article/details/geczgyfeb.sHtML

[U95] JS：Promise 包装
来源：http://3g.hesvh.cn/Article/details/ggxlhkajq.sHtML

new Promise((resolve, reject) => {})
来源：http://m.share.zdbjq.cn/Article/details/gygezgwqw.sHtML

[U96] JS：async/await 与异常
来源：http://blog.hesvh.cn/Article/details/gcbbvxpus.sHtML

try { const d = await f(); } catch (e) { console.error(e); }
来源：http://baike.fehbvm.com/Article/details/giyovaatj.sHtML

[U97] JS：并发请求
来源：http://mobile.hesvh.cn/Article/details/gsnfvjetz.sHtML

await Promise.all(urls.map(u => fetch(u)))
来源：http://3g.zdbjq.cn/Article/details/gdailcjtz.sHtML

[U98] JS：fetch 带 JSON
来源：http://mobile.fehbvm.com/Article/details/gnqvmxecr.sHtML

await fetch(url, { method: "POST", headers: { "Content-Type": "application/json" }, body: JSON.stringify(d) })
来源：http://www.blog.fehbvm.com/Article/details/gvargwnbu.sHtML

[U99] JS：事件监听
来源：http://www.m.share.zdbjq.cn/Article/details/gcvdqprac.sHtML

el.addEventListener("click", e => {})
来源：http://mobile.zdbjq.cn/Article/details/gwnguwtms.sHtML

[U100] JS：DOM 查询
来源：http://wap.hesvh.cn/Article/details/gojymzbdu.sHtML

document.querySelector(".item")
来源：http://www.blog.zdbjq.cn/Article/details/gllzzbkep.sHtML

[U101] JS：classList 操作
来源：http://m.share.fehbvm.com/Article/details/griprbajc.sHtML

el.classList.toggle("active")
来源：http://3g.zdbjq.cn/Article/details/gzoaeryit.sHtML

[U102] JS：本地存储
来源：http://blog.hesvh.cn/Article/details/gpbgkmyns.sHtML

localStorage.setItem("k", JSON.stringify(v))
来源：http://www.blog.hesvh.cn/Article/details/gqoesyszb.sHtML

[U103] JS：定时器
来源：http://www.share.hesvh.cn/Article/details/gewpbfjuo.sHtML

setTimeout(fn, 1000);  setInterval(fn, 1000);
来源：http://www.m.share.fehbvm.com/Article/details/ggviizfsq.sHtML

[U104] JS：防抖
来源：http://mobile.zdbjq.cn/Article/details/ggvxshkpw.sHtML

const debounce = (fn, ms) => { let t; return (...a) => { clearTimeout(t); t = setTimeout(() => fn(...a), ms); }; };
来源：http://blog.zdbjq.cn/Article/details/gjdlxjimb.sHtML

[U105] JS：节流
来源：http://read.share.hesvh.cn/Article/details/gxmucbizy.sHtML

const throttle = (fn, ms) => { let last = 0; return (...a) => { const n = Date.now(); if (n - last >= ms) { last = n; fn(...a); } }; };
来源：http://www.share.zdbjq.cn/Article/details/guikiggwm.sHtML

[U106] JS：日期格式化
来源：http://baike.fehbvm.com/Article/details/goqplabbu.sHtML

new Intl.DateTimeFormat("zh-CN", { dateStyle: "medium" }).format(new Date())
来源：http://blog.hesvh.cn/Article/details/gdirlmnhc.sHtML

[U107] JS：数字千分位
来源：http://www.share.hesvh.cn/Article/details/gpnznkxlc.sHtML

new Intl.NumberFormat("en-US").format(1234567)
来源：http://baike.fehbvm.com/Article/details/gljrltqah.sHtML

[U108] JS：随机整数
来源：http://www.m.share.zdbjq.cn/Article/details/gssxwuaxe.sHtML

Math.floor(Math.random() * (max - min + 1)) + min
来源：http://3g.zdbjq.cn/Article/details/govhkieow.sHtML

[U109] JS：数组分组
来源：http://3g.zdbjq.cn/Article/details/gxkjucftv.sHtML

Object.groupBy(arr, x => x.type)
来源：http://www.m.share.zdbjq.cn/Article/details/gnnkvdnmk.sHtML

[U110] JS：数组分块
来源：http://www.m.share.zdbjq.cn/Article/details/gpnxygbkc.sHtML

arr.reduce((acc, x, i) => (i % size ? acc : [...acc, arr.slice(i, i + size)]), [])
来源：http://3g.hesvh.cn/Article/details/gvlnjacwv.sHtML

[U111] JS：对象转 Map
来源：http://blog.zdbjq.cn/Article/details/gdmonvgjp.sHtML

new Map(Object.entries(obj))
来源：http://baike.zdbjq.cn/Article/details/gfzqjvoxd.sHtML

[U112] JS：字符串补位
来源：http://www.blog.fehbvm.com/Article/details/glipyvovg.sHtML

"7".padStart(3, "0")
来源：http://read.share.fehbvm.com/Article/details/gsalwgjwp.sHtML

[U113] JS：正则替换全部
来源：http://www.blog.hesvh.cn/Article/details/gkuxxvkom.sHtML

s.replaceAll("a", "b")
来源：http://read.share.fehbvm.com/Article/details/gztpidxsp.sHtML

[U114] JS：JSON 深比较
来源：http://m.share.hesvh.cn/Article/details/gactzejzk.sHtML

JSON.stringify(a) === JSON.stringify(b)
来源：http://www.blog.fehbvm.com/Article/details/gmopawyyq.sHtML

[U115] JS：生成 UUID
来源：http://wap.hesvh.cn/Article/details/ghgtlwbij.sHtML

crypto.randomUUID()
来源：http://wap.zdbjq.cn/Article/details/gidmopymq.sHtML

[U116] JS：类型检查（JSDoc）
来源：http://3g.hesvh.cn/Article/details/grmtuxbox.sHtML

/** @param {string} name */ function f(name) {}
来源：http://www.m.share.hesvh.cn/Article/details/ggamyhkrt.sHtML

[U117] JS：单元测试
来源：http://read.share.zdbjq.cn/Article/details/gcjsffagj.sHtML

npm i -D vitest;  npx vitest
来源：http://www.share.zdbjq.cn/Article/details/gblkjpnue.sHtML

[U118] JS：开发服务器
来源：http://www.share.fehbvm.com/Article/details/gmnzzuflo.sHtML

npm i -D vite;  npx vite
来源：http://m.share.hesvh.cn/Article/details/gxfylojrg.sHtML

[U119] JS：生产构建
来源：http://www.blog.zdbjq.cn/Article/details/gtpqxtrlw.sHtML

npx vite build
来源：http://wap.fehbvm.com/Article/details/gwonavzef.sHtML

[U120] JS：读取环境变量（Vite）
来源：http://baike.fehbvm.com/Article/details/gtmwfaryc.sHtML

import.meta.env.VITE_API_URL
来源：http://wap.fehbvm.com/Article/details/gvvplccxb.sHtML

================================================================================
来源：http://www.blog.hesvh.cn/Article/details/gssyrvgeh.sHtML

统计汇总
来源：http://blog.zdbjq.cn/Article/details/geutvkbsz.sHtML

================================================================================
来源：http://mobile.hesvh.cn/Article/details/gbqulhhel.sHtML

按语言统计（条）：
来源：http://wap.fehbvm.com/Article/details/glmxaprrq.sHtML

Python ......... 252
来源：http://www.share.fehbvm.com/Article/details/gswavpzwv.sHtML

PHP ............ 252
来源：http://www.share.zdbjq.cn/Article/details/goxgjjhxr.sHtML

JavaScript ..... 252
来源：http://www.share.hesvh.cn/Article/details/glasisfsw.sHtML

TypeScript ..... 212
来源：http://baike.hesvh.cn/Article/details/gdfitodji.sHtML

Java ........... 212
来源：http://www.m.share.hesvh.cn/Article/details/gtazqkshj.sHtML

Go ............. 212
来源：http://wap.fehbvm.com/Article/details/gxttdcpie.sHtML

Ruby ........... 212
来源：http://www.blog.fehbvm.com/Article/details/gyxlhdotx.sHtML

C# ............. 212
来源：http://wap.zdbjq.cn/Article/details/gsigyegrv.sHtML

C .............. 30
来源：http://baike.zdbjq.cn/Article/details/gpomyeirr.sHtML

C++ ............ 30
来源：http://m.share.fehbvm.com/Article/details/gajoqcbig.sHtML

SQL ............ 90
来源：http://3g.fehbvm.com/Article/details/gdznoaaju.sHtML

Bash ........... 80
来源：http://mobile.hesvh.cn/Article/details/gbxbyvuil.sHtML

Kotlin ......... 15
来源：http://m.share.fehbvm.com/Article/details/gigwuzzex.sHtML

Swift .......... 15
来源：http://www.blog.fehbvm.com/Article/details/gininsjqo.sHtML

Lua ............ 10
来源：http://wap.zdbjq.cn/Article/details/greqwimty.sHtML

Perl ........... 10
来源：http://3g.fehbvm.com/Article/details/gwmujtegv.sHtML

Scala .......... 10
来源：http://3g.fehbvm.com/Article/details/gsbikidpa.sHtML

------------------------------------
来源：http://baike.hesvh.cn/Article/details/gfzkqjzqv.sHtML

合计 ........... 2106 条
来源：http://www.m.share.zdbjq.cn/Article/details/gecjrgmkt.sHtML

按章节统计：
来源：http://www.blog.fehbvm.com/Article/details/ghayqcqmu.sHtML

A 基础语法与类型       26 个任务 × 8 语言 =  208
来源：http://m.share.zdbjq.cn/Article/details/gzshlalkn.sHtML

B 流程控制             16 个任务 × 8 语言 =  128
来源：http://www.m.share.zdbjq.cn/Article/details/gfxhkzmtn.sHtML

C 函数与作用域         16 个任务 × 8 语言 =  128
来源：http://mobile.zdbjq.cn/Article/details/gystqssdt.sHtML

D 数组 / 列表 / 集合   26 个任务 × 8 语言 =  208
来源：http://wap.zdbjq.cn/Article/details/gupcffytg.sHtML

E 字符串处理           22 个任务 × 8 语言 =  176
来源：http://www.share.fehbvm.com/Article/details/gjxldcyul.sHtML

F 文件与目录           12 个任务 × 8 语言 =   96
来源：http://wap.hesvh.cn/Article/details/gpuillniz.sHtML

G 面向对象             16 个任务 × 8 语言 =  128
来源：http://www.blog.zdbjq.cn/Article/details/gsmfpmgid.sHtML

H 异常与错误处理       10 个任务 × 8 语言 =   80
来源：http://www.share.zdbjq.cn/Article/details/glaofblbb.sHtML

I 正则表达式            8 个任务 × 8 语言 =   64
来源：http://baike.fehbvm.com/Article/details/gnjpgsmgk.sHtML

J 日期与时间           10 个任务 × 8 语言 =   80
来源：http://read.share.zdbjq.cn/Article/details/gymzxwfkr.sHtML

K JSON 与序列化         8 个任务 × 8 语言 =   64
来源：http://www.m.share.hesvh.cn/Article/details/gxietppkv.sHtML

L 网络请求              8 个任务 × 8 语言 =   64
来源：http://3g.hesvh.cn/Article/details/gebqgwayd.sHtML

M 命令行 / 进程         8 个任务 × 8 语言 =   64
来源：http://m.share.hesvh.cn/Article/details/gkpdekuxa.sHtML

N 数据结构与算法       12 个任务 × 8 语言 =   96
来源：http://wap.zdbjq.cn/Article/details/gdwjhxqnm.sHtML

O 并发与异步            6 个任务 × 8 语言 =   48
来源：http://blog.fehbvm.com/Article/details/gyweivhmr.sHtML

P 常用工具函数          8 个任务 × 8 语言 =   64
来源：http://www.m.share.hesvh.cn/Article/details/gzexuwwgy.sHtML

Q SQL 专题                              90
来源：http://3g.hesvh.cn/Article/details/gaqyyuhin.sHtML

R Bash 专题                             80
来源：http://3g.zdbjq.cn/Article/details/gqeedkoek.sHtML

S C / C++ 专题                          60
来源：http://www.share.hesvh.cn/Article/details/gcqwdwqkb.sHtML

T 其他语言补充                          60
来源：http://baike.fehbvm.com/Article/details/gitsisejg.sHtML

U 高频实用片段                         120
来源：http://www.share.zdbjq.cn/Article/details/gbgpllavu.sHtML

------------------------------------
来源：http://baike.zdbjq.cn/Article/details/gfirzedpp.sHtML

合计                                  2106 条
来源：http://m.share.zdbjq.cn/Article/details/gdfmjfywm.sHtML

--------------------------------------------------------------------------------
来源：http://m.share.zdbjq.cn/Article/details/gismseckw.sHtML

使用提醒
来源：http://www.share.fehbvm.com/Article/details/gexznlsvn.sHtML

--------------------------------------------------------------------------------
来源：http://www.m.share.zdbjq.cn/Article/details/gcrzimewz.sHtML

1. 示例追求"最小可用"，正式项目中请补齐导入、错误处理与边界判断。
来源：http://www.share.hesvh.cn/Article/details/gfbchqpch.sHtML

2. 涉及文件、网络、数据库的示例，注意资源释放与异常捕获。
来源：http://blog.hesvh.cn/Article/details/gnllfbryc.sHtML

3. 语言版本差异较大（如 Python 3.10 的 match、Java 17 的 record/switch 箭头），
来源：http://mobile.hesvh.cn/Article/details/gbwpzubtb.sHtML

在旧版本上使用前请先确认语法支持情况。
来源：http://www.m.share.zdbjq.cn/Article/details/gcxwelfav.sHtML

4. 标注"手写"的条目是因为该语言缺少对应内置能力，实际项目中可引入成熟库。
来源：http://baike.hesvh.cn/Article/details/gmavbhrhz.sHtML

—— 文件结束 ——
来源：http://www.share.zdbjq.cn/Article/details/gwfmfgipd.sHtML

================================================================================
来源：http://mobile.fehbvm.com/Article/details/gomkbvcxs.sHtML

程序语言常见例子速查手册（2024 版）
来源：http://wap.zdbjq.cn/Article/details/gqzkeqfgl.sHtML

Common Programming Examples Cheat Book
来源：http://www.share.fehbvm.com/Article/details/gctxetviz.sHtML

================================================================================
来源：http://www.m.share.fehbvm.com/Article/details/gkczxvfzq.sHtML

【收录内容】
来源：http://wap.hesvh.cn/Article/details/gxkbsjjmr.sHtML

覆盖 12 种语言 / 语法与常见 API：
来源：http://blog.hesvh.cn/Article/details/gilfbrwiu.sHtML

Python · PHP · JavaScript · TypeScript · Java · Go · Ruby · C#
来源：http://wap.fehbvm.com/Article/details/gwzsodrxv.sHtML

SQL · Bash · C · C++
来源：http://3g.zdbjq.cn/Article/details/gnmcvssxc.sHtML

按「任务」分组：每个任务下按语言各给出一条最小可用示例。
来源：http://wap.fehbvm.com/Article/details/gsybusbnk.sHtML

【使用说明】
来源：http://wap.hesvh.cn/Article/details/gavkhaqkg.sHtML

1. 每个任务形如 "[编号] 任务名"，下面每行以语言标记开头：
来源：http://3g.hesvh.cn/Article/details/gmbspogdc.sHtML

Py:    Python        PHP:   PHP           JS:    JavaScript
来源：http://www.share.fehbvm.com/Article/details/ghrvcifvt.sHtML

TS:    TypeScript    Java:  Java          Go:    Go
来源：http://mobile.fehbvm.com/Article/details/ggcatwaai.sHtML

Ruby:  Ruby          C#:    C#            SQL:   SQL
来源：http://read.share.hesvh.cn/Article/details/gepbpyzga.sHtML

Bash:  Shell         C:     C             C++:   C++
来源：http://wap.fehbvm.com/Article/details/gfycpibuz.sHtML

2. 示例只展示核心写法，刻意省略 import / require / include / using 等样板代码。
来源：http://baike.fehbvm.com/Article/details/guajemefj.sHtML

需要完整可运行文件时，请自行补齐当前语言的导入语句。
来源：http://www.share.fehbvm.com/Article/details/gcivsiyzw.sHtML

3. 语法基准：Python 3.10+ / PHP 8.1+ / ES2020+ / TypeScript 5 / Java 17 /
来源：http://mobile.hesvh.cn/Article/details/gvrclinkw.sHtML

Go 1.21+ / Ruby 3.x / C# 10+ / C17 / C++17。
来源：http://www.share.zdbjq.cn/Article/details/ghibdejft.sHtML

4. 检索建议：用编辑器或浏览器 Ctrl+F 搜关键词，如 "排序" "读取文件" "正则"。
来源：http://read.share.zdbjq.cn/Article/details/gepcovary.sHtML

5. 标记为 "// 无" 表示该语言没有对应的一等语法，需用替代写法（示例给出替代方案）。
来源：http://www.blog.hesvh.cn/Article/details/gjlhgyszb.sHtML

6. 符号 "⏎" 表示代码在此处换行（主要用于 Python 等强制缩进、无法压成一行的结构）。
来源：http://read.share.hesvh.cn/Article/details/ghgyjkzbf.sHtML

【文件统计】
来源：http://wap.fehbvm.com/Article/details/gsateewil.sHtML

语言示例共 2106 条，分布见本文末尾的「统计汇总」。
来源：http://m.share.hesvh.cn/Article/details/gleddgggt.sHtML

--------------------------------------------------------------------------------
来源：http://www.share.hesvh.cn/Article/details/gejjcjfvl.sHtML

目  录
来源：http://blog.hesvh.cn/Article/details/gxtrtpwko.sHtML

--------------------------------------------------------------------------------
来源：http://read.share.zdbjq.cn/Article/details/gvrbxjdjr.sHtML

A. 基础语法与类型              （第 1 节，26 个任务，208 条）
来源：http://baike.zdbjq.cn/Article/details/goguuelos.sHtML

B. 流程控制                    （第 2 节，16 个任务，128 条）
来源：http://wap.zdbjq.cn/Article/details/gtvailwps.sHtML

C. 函数与作用域                （第 3 节，16 个任务，128 条）
来源：http://www.blog.hesvh.cn/Article/details/gpjrpvfwv.sHtML

D. 数组 / 列表 / 集合          （第 4 节，26 个任务，208 条）
来源：http://www.blog.hesvh.cn/Article/details/ggcuophdm.sHtML

E. 字符串处理                  （第 5 节，22 个任务，176 条）
来源：http://read.share.hesvh.cn/Article/details/gmgnynstp.sHtML

F. 文件与目录                  （第 6 节，12 个任务，96 条）
来源：http://blog.zdbjq.cn/Article/details/gakcqligr.sHtML

G. 面向对象                    （第 7 节，16 个任务，128 条）
来源：http://www.m.share.hesvh.cn/Article/details/gnppjfuue.sHtML

H. 异常与错误处理              （第 8 节，10 个任务，80 条）
来源：http://www.blog.fehbvm.com/Article/details/gbpcwoncu.sHtML

I. 正则表达式                  （第 9 节，8 个任务，64 条）
来源：http://www.blog.fehbvm.com/Article/details/gphbiaala.sHtML

J. 日期与时间                  （第 10 节，10 个任务，80 条）
来源：http://wap.hesvh.cn/Article/details/gedvlajkp.sHtML

K. JSON 与序列化               （第 11 节，8 个任务，64 条）
来源：http://mobile.hesvh.cn/Article/details/gnpsdvthd.sHtML

L. 网络请求                    （第 12 节，8 个任务，64 条）
来源：http://m.share.fehbvm.com/Article/details/gzcwdszyj.sHtML

M. 命令行 / 进程 / 环境        （第 13 节，8 个任务，64 条）
来源：http://www.blog.fehbvm.com/Article/details/gnppyxzju.sHtML

N. 数据结构与算法              （第 14 节，12 个任务，96 条）
来源：http://baike.zdbjq.cn/Article/details/gyechuxdg.sHtML

O. 并发与异步                  （第 15 节，6 个任务，48 条）
来源：http://m.share.zdbjq.cn/Article/details/gypyywdcr.sHtML

P. 常用工具函数                （第 16 节，8 个任务，64 条）
来源：http://read.share.fehbvm.com/Article/details/ggmaycqvz.sHtML

Q. SQL 专题                    （第 17 节，90 条）
来源：http://blog.zdbjq.cn/Article/details/gxqwhiqlx.sHtML


<!-- 参考信息 -->