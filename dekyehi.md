代发 wailian999

[U25] Py：CSV 按字典读
来源：http://m.share.fanxiaobao.xyz/Article/details/gveaaxwrm.sHtML

csv.DictReader(f)
来源：http://baike.fanxiaobao.xyz/Article/details/gdphcothw.sHtML

[U26] Py：并发下载
来源：http://mobile.fanxiaobao.xyz/Article/details/gxzsdjzzj.sHtML

ThreadPoolExecutor(max_workers=8).map(fetch, urls)
来源：http://www.blog.fanxiaobao.xyz/Article/details/gpqtzezro.sHtML

[U27] Py：异步 HTTP
来源：http://blog.fanxiaobao.xyz/Article/details/gmaiildfr.sHtML

aiohttp.ClientSession() 配合 async with
来源：http://www.share.fanxiaobao.xyz/Article/details/gkrwiiewx.sHtML

[U28] Py：类型别名
来源：http://wap.fanxiaobao.xyz/Article/details/gxmdyiyxf.sHtML

UserId = int
来源：http://www.blog.fanxiaobao.xyz/Article/details/gtvnghhug.sHtML

[U29] Py：属性校验
来源：http://read.share.fanxiaobao.xyz/Article/details/githugxfa.sHtML

@property 与 @x.setter 配合
来源：http://read.share.fanxiaobao.xyz/Article/details/gvsrxfgdn.sHtML

[U30] Py：数据类
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gaflfjxhf.sHtML

@dataclass(slots=True)
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gcvjcjxzk.sHtML

[U31] Py：单测
来源：http://wap.fanxiaobao.xyz/Article/details/gyuxugtax.sHtML

python -m pytest -q
来源：http://blog.fanxiaobao.xyz/Article/details/gkdkeaaif.sHtML

[U32] Py：代码格式化
来源：http://3g.fanxiaobao.xyz/Article/details/gdqmnwgmr.sHtML

ruff format . && ruff check --fix .
来源：http://baike.fanxiaobao.xyz/Article/details/grmskcorj.sHtML

[U33] Py：打包发布
来源：http://read.share.fanxiaobao.xyz/Article/details/ggwgnqfks.sHtML

python -m build  （依赖 pyproject.toml）
来源：http://www.blog.fanxiaobao.xyz/Article/details/gjscfmaph.sHtML

[U34] Py：判断编码
来源：http://blog.fanxiaobao.xyz/Article/details/gyfvaouvc.sHtML

chardet.detect(raw)
来源：http://baike.fanxiaobao.xyz/Article/details/gxfjzciar.sHtML

[U35] Py：发送邮件
来源：http://blog.fanxiaobao.xyz/Article/details/gorrezbfa.sHtML

smtplib.SMTP_SSL(...).send_message(msg)
来源：http://baike.fanxiaobao.xyz/Article/details/gcaahqxdc.sHtML

[U36] Py：定时任务
来源：http://mobile.fanxiaobao.xyz/Article/details/gskybqtue.sHtML

schedule.every(10).minutes.do(job)
来源：http://www.blog.fanxiaobao.xyz/Article/details/gomyfjnzl.sHtML

[U37] Py：读写 Excel
来源：http://wap.fanxiaobao.xyz/Article/details/gblfebprb.sHtML

pandas.read_excel / DataFrame.to_excel
来源：http://baike.fanxiaobao.xyz/Article/details/glerkbeks.sHtML

[U38] Py：获取脚本所在目录
来源：http://3g.fanxiaobao.xyz/Article/details/gqjhzysfn.sHtML

Path(__file__).resolve().parent
来源：http://read.share.fanxiaobao.xyz/Article/details/genzigbwz.sHtML

[U39] Py：判断是否在交互环境
来源：http://m.share.fanxiaobao.xyz/Article/details/gqsgdouve.sHtML

sys.stdout.isatty()
来源：http://read.share.fanxiaobao.xyz/Article/details/gpxtdwdga.sHtML

[U40] Py：打印到标准错误
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gwunonmzj.sHtML

print("err", file=sys.stderr)
来源：http://baike.fanxiaobao.xyz/Article/details/gowtpyuyu.sHtML

[U41] PHP：初始化 Composer 项目
来源：http://3g.fanxiaobao.xyz/Article/details/gxyvrmess.sHtML

composer init;  composer require guzzlehttp/guzzle
来源：http://wap.fanxiaobao.xyz/Article/details/gljorjctm.sHtML

[U42] PHP：PSR-4 自动加载
来源：http://www.share.fanxiaobao.xyz/Article/details/gkgnycngs.sHtML

"autoload": { "psr-4": { "App\\": "src/" } }
来源：http://www.share.fanxiaobao.xyz/Article/details/glvhzwvvd.sHtML

[U43] PHP：声明命名空间
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gterrsjrr.sHtML

namespace App\Http;
来源：http://3g.fanxiaobao.xyz/Article/details/gbyknhkuh.sHtML

[U44] PHP：开启严格类型
来源：http://read.share.fanxiaobao.xyz/Article/details/gymhhvhxn.sHtML

declare(strict_types=1);
来源：http://baike.fanxiaobao.xyz/Article/details/gfofuhohg.sHtML

[U45] PHP：类型声明与返回类型
来源：http://3g.fanxiaobao.xyz/Article/details/gjlpvewcr.sHtML

function add(int $a, int $b): int { return $a + $b; }
来源：http://mobile.fanxiaobao.xyz/Article/details/gxsdqjwmx.sHtML

[U46] PHP：可空类型
来源：http://www.blog.fanxiaobao.xyz/Article/details/gthlwikcz.sHtML

?string $name = null
来源：http://m.share.fanxiaobao.xyz/Article/details/gtdvjhaij.sHtML

[U47] PHP：联合类型
来源：http://mobile.fanxiaobao.xyz/Article/details/gmklthdzl.sHtML

int|string $id
来源：http://www.share.fanxiaobao.xyz/Article/details/gswioweka.sHtML

[U48] PHP：纯枚举
来源：http://mobile.fanxiaobao.xyz/Article/details/guforkiqc.sHtML

enum Status: string { case Active = "active"; case Off = "off"; }
来源：http://baike.fanxiaobao.xyz/Article/details/gjntnomro.sHtML

[U49] PHP：只读属性
来源：http://3g.fanxiaobao.xyz/Article/details/ghdyjxvpd.sHtML

public readonly string $name
来源：http://blog.fanxiaobao.xyz/Article/details/gvxtuekkm.sHtML

[U50] PHP：构造器属性提升
来源：http://read.share.fanxiaobao.xyz/Article/details/gkcjvndkm.sHtML

public function __construct(private int $id) {}
来源：http://blog.fanxiaobao.xyz/Article/details/gxtlxkzud.sHtML

[U51] PHP：数组解构
来源：http://baike.fanxiaobao.xyz/Article/details/gwvilmwxk.sHtML

[$a, $b] = $arr;
来源：http://www.share.fanxiaobao.xyz/Article/details/glrtbcpdm.sHtML

[U52] PHP：箭头函数
来源：http://baike.fanxiaobao.xyz/Article/details/gvgnslxzd.sHtML

$double = fn($x) => $x * 2;
来源：http://blog.fanxiaobao.xyz/Article/details/geydoukzr.sHtML

[U53] PHP：空合并运算符
来源：http://blog.fanxiaobao.xyz/Article/details/gmhfrtcmf.sHtML

$v = $a ?? $b ?? "default";
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gnzhjcood.sHtML

[U54] PHP：空安全调用
来源：http://blog.fanxiaobao.xyz/Article/details/gdosnjlul.sHtML

$obj?->method()
来源：http://blog.fanxiaobao.xyz/Article/details/ggwaepbvd.sHtML

[U55] PHP：match 表达式
来源：http://www.blog.fanxiaobao.xyz/Article/details/gwkksgknz.sHtML

$s = match($x) { 1 => "一", default => "其他" };
来源：http://www.m.share.fanxiaobao.xyz/Article/details/geapecaxq.sHtML

[U56] PHP：命名参数
来源：http://read.share.fanxiaobao.xyz/Article/details/grpewakxr.sHtML

f(a: 1, b: 2)
来源：http://read.share.fanxiaobao.xyz/Article/details/gpqvemfgw.sHtML

[U57] PHP：字符串插值
来源：http://m.share.fanxiaobao.xyz/Article/details/gdjhthlgy.sHtML

"值: {$a}"
来源：http://www.share.fanxiaobao.xyz/Article/details/gfedqftuh.sHtML

[U58] PHP：数组三件套
来源：http://baike.fanxiaobao.xyz/Article/details/gxtnwmlvf.sHtML

array_map($f, $a);  array_filter($a, $f);  array_reduce($a, $f, 0);
来源：http://baike.fanxiaobao.xyz/Article/details/geaosngik.sHtML

[U59] PHP：自定义排序
来源：http://baike.fanxiaobao.xyz/Article/details/gmybgcirz.sHtML

usort($arr, fn($a, $b) => $a["age"] <=> $b["age"]);
来源：http://wap.fanxiaobao.xyz/Article/details/gnqfovhsm.sHtML

[U60] PHP：JSON 编解码
来源：http://mobile.fanxiaobao.xyz/Article/details/gdbytthwi.sHtML

json_encode($d, JSON_UNESCAPED_UNICODE);  json_decode($s, true);
来源：http://3g.fanxiaobao.xyz/Article/details/gseoomtti.sHtML

[U61] PHP：正则
来源：http://read.share.fanxiaobao.xyz/Article/details/ghqakprot.sHtML

preg_match('/(\d+)/', $s, $m);  preg_replace('/\d+/', '#', $s);
来源：http://www.share.fanxiaobao.xyz/Article/details/gnbtgnudn.sHtML

[U62] PHP：日期对象
来源：http://blog.fanxiaobao.xyz/Article/details/gqqdevagk.sHtML

(new DateTimeImmutable())->format("Y-m-d");
来源：http://3g.fanxiaobao.xyz/Article/details/gigcabvdv.sHtML

[U63] PHP：文件读写
来源：http://www.share.fanxiaobao.xyz/Article/details/gmlonceyp.sHtML

file_get_contents($f);  file_put_contents($f, $data);
来源：http://baike.fanxiaobao.xyz/Article/details/ghiyqclgr.sHtML

[U64] PHP：目录遍历
来源：http://www.blog.fanxiaobao.xyz/Article/details/gcytrdqkh.sHtML

glob("dir/*.php");  scandir("dir");
来源：http://wap.fanxiaobao.xyz/Article/details/gwwefsjzp.sHtML

[U65] PHP：会话
来源：http://baike.fanxiaobao.xyz/Article/details/ggrggfwpp.sHtML

session_start();  $_SESSION["uid"] = 1;
来源：http://mobile.fanxiaobao.xyz/Article/details/gjehvzhkm.sHtML

[U66] PHP：设置 Cookie
来源：http://wap.fanxiaobao.xyz/Article/details/gmumewuyg.sHtML

setcookie("token", $v, ["httponly" => true, "samesite" => "Lax"]);
来源：http://m.share.fanxiaobao.xyz/Article/details/giovpczhg.sHtML

[U67] PHP：处理文件上传
来源：http://read.share.fanxiaobao.xyz/Article/details/gtzmuytww.sHtML

$_FILES["file"]["tmp_name"] 与 move_uploaded_file()
来源：http://3g.fanxiaobao.xyz/Article/details/gsgmhbnfm.sHtML

[U68] PHP：PDO 连接
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gxmtxuivo.sHtML

$pdo = new PDO("mysql:host=localhost;dbname=app", "root", "");
来源：http://www.share.fanxiaobao.xyz/Article/details/gbrkfbdvv.sHtML

[U69] PHP：PDO 预处理
来源：http://www.share.fanxiaobao.xyz/Article/details/gdbyuailm.sHtML

$stmt = $pdo->prepare("SELECT * FROM users WHERE id = ?");  $stmt->execute([$id]);
来源：http://www.share.fanxiaobao.xyz/Article/details/grungkglz.sHtML

[U70] PHP：PDO 事务
来源：http://mobile.fanxiaobao.xyz/Article/details/gncnbebwb.sHtML

$pdo->beginTransaction();  $pdo->commit();  $pdo->rollBack();
来源：http://read.share.fanxiaobao.xyz/Article/details/gtzxpnbla.sHtML

[U71] PHP：抛出异常
来源：http://3g.fanxiaobao.xyz/Article/details/gfbazthiu.sHtML

throw new RuntimeException("失败", 500);
来源：http://www.blog.fanxiaobao.xyz/Article/details/gkddewurf.sHtML

[U72] PHP：写错误日志
来源：http://baike.fanxiaobao.xyz/Article/details/gvsqrdcil.sHtML

error_log("失败: " . $e->getMessage());
来源：http://baike.fanxiaobao.xyz/Article/details/gxxsazbgo.sHtML

[U73] PHP：读取 ini 配置
来源：http://read.share.fanxiaobao.xyz/Article/details/gbwcfujjv.sHtML

parse_ini_file("config.ini", true)
来源：http://3g.fanxiaobao.xyz/Article/details/ggjmncjgh.sHtML

[U74] PHP：读取环境变量
来源：http://www.blog.fanxiaobao.xyz/Article/details/ghvfwjkfs.sHtML

getenv("APP_ENV") ?: "production"
来源：http://m.share.fanxiaobao.xyz/Article/details/ggfmtkgho.sHtML

[U75] PHP：依赖注入
来源：http://read.share.fanxiaobao.xyz/Article/details/gkgoozqjx.sHtML

composer require psr/container
来源：http://www.m.share.fanxiaobao.xyz/Article/details/ghzzlbxkg.sHtML

[U76] PHP：简单路由
来源：http://mobile.fanxiaobao.xyz/Article/details/guetlncuu.sHtML

$path = parse_url($_SERVER["REQUEST_URI"], PHP_URL_PATH);
来源：http://www.share.fanxiaobao.xyz/Article/details/goihqszwc.sHtML

[U77] PHP：模板渲染
来源：http://www.blog.fanxiaobao.xyz/Article/details/gjmdnseuv.sHtML

composer require twig/twig
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gxczmtqhi.sHtML

[U78] PHP：单元测试
来源：http://mobile.fanxiaobao.xyz/Article/details/gmwcjhkhb.sHtML

composer require --dev phpunit/phpunit
来源：http://www.share.fanxiaobao.xyz/Article/details/gsxawjzxr.sHtML

[U79] PHP：静态分析
来源：http://read.share.fanxiaobao.xyz/Article/details/grrsxmfib.sHtML

composer require --dev phpstan/phpstan
来源：http://m.share.fanxiaobao.xyz/Article/details/gzrrybgcf.sHtML

[U80] PHP：代码规范修复
来源：http://blog.fanxiaobao.xyz/Article/details/gxhtgyins.sHtML

composer require --dev friendsofphp/php-cs-fixer
来源：http://wap.fanxiaobao.xyz/Article/details/gendwwlid.sHtML

[U81] JS：初始化项目
来源：http://mobile.fanxiaobao.xyz/Article/details/gdmahadyj.sHtML

npm init -y;  npm i express
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gbwvxzmet.sHtML

[U82] JS：package.json 脚本
来源：http://m.share.fanxiaobao.xyz/Article/details/gibnkeutc.sHtML

"scripts": { "dev": "vite", "build": "vite build" }
来源：http://m.share.fanxiaobao.xyz/Article/details/gimprvmvn.sHtML

[U83] JS：ES Module 导入导出
来源：http://3g.fanxiaobao.xyz/Article/details/ggdlnqidp.sHtML

export const a = 1;  import { a } from "./m.js";
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gzyrfukjv.sHtML

[U84] JS：CommonJS 写法
来源：http://www.blog.fanxiaobao.xyz/Article/details/gmzvwczze.sHtML

module.exports = { a };  const { a } = require("./m");
来源：http://mobile.fanxiaobao.xyz/Article/details/gpiynfeja.sHtML

[U85] JS：可选链
来源：http://blog.fanxiaobao.xyz/Article/details/gsncacpbo.sHtML

a?.b?.c
来源：http://read.share.fanxiaobao.xyz/Article/details/gjwauhfnp.sHtML

[U86] JS：空值合并
来源：http://www.blog.fanxiaobao.xyz/Article/details/gnwracslo.sHtML

a ?? b
来源：http://www.blog.fanxiaobao.xyz/Article/details/gzuzvgwad.sHtML

[U87] JS：解构默认值
来源：http://blog.fanxiaobao.xyz/Article/details/gluypyimo.sHtML

const { a = 1, b = 2 } = obj;
来源：http://3g.fanxiaobao.xyz/Article/details/gzrpfvdpg.sHtML

[U88] JS：对象展开合并
来源：http://wap.fanxiaobao.xyz/Article/details/gnxddfstz.sHtML

{ ...a, ...b }
来源：http://baike.fanxiaobao.xyz/Article/details/gtmybeseh.sHtML

[U89] JS：数组去重
来源：http://mobile.fanxiaobao.xyz/Article/details/guulleupc.sHtML

[...new Set(arr)]
来源：http://m.share.fanxiaobao.xyz/Article/details/geldriysf.sHtML

[U90] JS：数字数组排序
来源：http://baike.fanxiaobao.xyz/Article/details/gncdwofel.sHtML

[...arr].sort((a, b) => a - b)
来源：http://3g.fanxiaobao.xyz/Article/details/gqsohurpu.sHtML

[U91] JS：对象键值遍历
来源：http://www.share.fanxiaobao.xyz/Article/details/gjkxmyare.sHtML

Object.entries(obj).forEach(([k, v]) => {});
来源：http://3g.fanxiaobao.xyz/Article/details/grauudgah.sHtML

[U92] JS：深拷贝
来源：http://www.blog.fanxiaobao.xyz/Article/details/gyuungdks.sHtML

structuredClone(obj)
来源：http://mobile.fanxiaobao.xyz/Article/details/gjgytclns.sHtML

[U93] JS：模板字符串
来源：http://m.share.fanxiaobao.xyz/Article/details/gtwxytoem.sHtML

`共 ${n} 条`
来源：http://www.share.fanxiaobao.xyz/Article/details/gjqxsqrwn.sHtML

[U94] JS：箭头函数
来源：http://m.share.fanxiaobao.xyz/Article/details/gbytpeicq.sHtML

const double = x => x * 2;
来源：http://baike.fanxiaobao.xyz/Article/details/gmsiugqgd.sHtML

[U95] JS：Promise 包装
来源：http://www.blog.fanxiaobao.xyz/Article/details/gssemaybf.sHtML

new Promise((resolve, reject) => {})
来源：http://www.blog.fanxiaobao.xyz/Article/details/glucmwbsr.sHtML

[U96] JS：async/await 与异常
来源：http://www.blog.fanxiaobao.xyz/Article/details/gantmfeit.sHtML

try { const d = await f(); } catch (e) { console.error(e); }
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gvpntrgqa.sHtML

[U97] JS：并发请求
来源：http://baike.fanxiaobao.xyz/Article/details/gtfliedzp.sHtML

await Promise.all(urls.map(u => fetch(u)))
来源：http://read.share.fanxiaobao.xyz/Article/details/gvairzhpj.sHtML

[U98] JS：fetch 带 JSON
来源：http://read.share.fanxiaobao.xyz/Article/details/gybfxioll.sHtML

await fetch(url, { method: "POST", headers: { "Content-Type": "application/json" }, body: JSON.stringify(d) })
来源：http://mobile.fanxiaobao.xyz/Article/details/gpovnxdfu.sHtML

[U99] JS：事件监听
来源：http://blog.fanxiaobao.xyz/Article/details/gdlhiyiqi.sHtML

el.addEventListener("click", e => {})
来源：http://wap.fanxiaobao.xyz/Article/details/gldtnmttw.sHtML

[U100] JS：DOM 查询
来源：http://m.share.fanxiaobao.xyz/Article/details/gdgmiayqg.sHtML

document.querySelector(".item")
来源：http://www.share.fanxiaobao.xyz/Article/details/gdvcsbzrd.sHtML

[U101] JS：classList 操作
来源：http://blog.fanxiaobao.xyz/Article/details/gwbmygufu.sHtML

el.classList.toggle("active")
来源：http://blog.fanxiaobao.xyz/Article/details/gedimeagl.sHtML

[U102] JS：本地存储
来源：http://wap.fanxiaobao.xyz/Article/details/geminzkyq.sHtML

localStorage.setItem("k", JSON.stringify(v))
来源：http://3g.fanxiaobao.xyz/Article/details/grhexgrpz.sHtML

[U103] JS：定时器
来源：http://wap.fanxiaobao.xyz/Article/details/gawqjnahi.sHtML

setTimeout(fn, 1000);  setInterval(fn, 1000);
来源：http://www.share.fanxiaobao.xyz/Article/details/glqneayxz.sHtML

[U104] JS：防抖
来源：http://3g.fanxiaobao.xyz/Article/details/gkxmoolvj.sHtML

const debounce = (fn, ms) => { let t; return (...a) => { clearTimeout(t); t = setTimeout(() => fn(...a), ms); }; };
来源：http://mobile.fanxiaobao.xyz/Article/details/gnsnmwkhx.sHtML

[U105] JS：节流
来源：http://www.share.fanxiaobao.xyz/Article/details/gfvaiujdu.sHtML

const throttle = (fn, ms) => { let last = 0; return (...a) => { const n = Date.now(); if (n - last >= ms) { last = n; fn(...a); } }; };
来源：http://m.share.fanxiaobao.xyz/Article/details/ggvesfhdl.sHtML

[U106] JS：日期格式化
来源：http://baike.fanxiaobao.xyz/Article/details/gmfuowxmo.sHtML

new Intl.DateTimeFormat("zh-CN", { dateStyle: "medium" }).format(new Date())
来源：http://www.share.fanxiaobao.xyz/Article/details/gsfswdvsy.sHtML

[U107] JS：数字千分位
来源：http://read.share.fanxiaobao.xyz/Article/details/gsoepxwof.sHtML

new Intl.NumberFormat("en-US").format(1234567)
来源：http://blog.fanxiaobao.xyz/Article/details/gnkdnphho.sHtML

[U108] JS：随机整数
来源：http://www.blog.fanxiaobao.xyz/Article/details/gbualdysd.sHtML

Math.floor(Math.random() * (max - min + 1)) + min
来源：http://3g.fanxiaobao.xyz/Article/details/gwcdbfpcc.sHtML

[U109] JS：数组分组
来源：http://wap.fanxiaobao.xyz/Article/details/gaysizbfu.sHtML

Object.groupBy(arr, x => x.type)
来源：http://blog.fanxiaobao.xyz/Article/details/gqmlxxeoz.sHtML

[U110] JS：数组分块
来源：http://read.share.fanxiaobao.xyz/Article/details/gzoucuwxl.sHtML

arr.reduce((acc, x, i) => (i % size ? acc : [...acc, arr.slice(i, i + size)]), [])
来源：http://wap.fanxiaobao.xyz/Article/details/grvhvtfwg.sHtML

[U111] JS：对象转 Map
来源：http://m.share.fanxiaobao.xyz/Article/details/gdbeuemgj.sHtML

new Map(Object.entries(obj))
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gdvnnnpss.sHtML

[U112] JS：字符串补位
来源：http://read.share.fanxiaobao.xyz/Article/details/gfyvmxncp.sHtML

"7".padStart(3, "0")
来源：http://read.share.fanxiaobao.xyz/Article/details/gowombsud.sHtML

[U113] JS：正则替换全部
来源：http://m.share.fanxiaobao.xyz/Article/details/giopxmljj.sHtML

s.replaceAll("a", "b")
来源：http://read.share.fanxiaobao.xyz/Article/details/gmdqpsgpd.sHtML

[U114] JS：JSON 深比较
来源：http://wap.fanxiaobao.xyz/Article/details/gclkcugoo.sHtML

JSON.stringify(a) === JSON.stringify(b)
来源：http://www.blog.fanxiaobao.xyz/Article/details/gvolxnqyf.sHtML

[U115] JS：生成 UUID
来源：http://m.share.fanxiaobao.xyz/Article/details/gebdxfsls.sHtML

crypto.randomUUID()
来源：http://www.share.fanxiaobao.xyz/Article/details/gpfrkvhks.sHtML

[U116] JS：类型检查（JSDoc）
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gohpnzabl.sHtML

/** @param {string} name */ function f(name) {}
来源：http://wap.fanxiaobao.xyz/Article/details/ghrkscfvv.sHtML

[U117] JS：单元测试
来源：http://3g.fanxiaobao.xyz/Article/details/geefithab.sHtML

npm i -D vitest;  npx vitest
来源：http://www.share.fanxiaobao.xyz/Article/details/gywosrzhh.sHtML

[U118] JS：开发服务器
来源：http://www.share.fanxiaobao.xyz/Article/details/gcvqsutvi.sHtML

npm i -D vite;  npx vite
来源：http://3g.fanxiaobao.xyz/Article/details/gaqwzrwkp.sHtML

[U119] JS：生产构建
来源：http://m.share.fanxiaobao.xyz/Article/details/ghlcbmblw.sHtML

npx vite build
来源：http://3g.fanxiaobao.xyz/Article/details/gophvixls.sHtML

[U120] JS：读取环境变量（Vite）
来源：http://www.share.fanxiaobao.xyz/Article/details/gopczsoeg.sHtML

import.meta.env.VITE_API_URL
来源：http://m.share.fanxiaobao.xyz/Article/details/gvbdukhjw.sHtML

================================================================================
来源：http://mobile.fanxiaobao.xyz/Article/details/gbmhtnsjk.sHtML

统计汇总
来源：http://baike.fanxiaobao.xyz/Article/details/gmjysflta.sHtML

================================================================================
来源：http://www.share.fanxiaobao.xyz/Article/details/gvyhlkipo.sHtML

按语言统计（条）：
来源：http://blog.fanxiaobao.xyz/Article/details/gvxldzkvu.sHtML

Python ......... 252
来源：http://read.share.fanxiaobao.xyz/Article/details/gotuudsnw.sHtML

PHP ............ 252
来源：http://3g.fanxiaobao.xyz/Article/details/gqqqukuci.sHtML

JavaScript ..... 252
来源：http://blog.fanxiaobao.xyz/Article/details/gqyjsbknd.sHtML

TypeScript ..... 212
来源：http://wap.fanxiaobao.xyz/Article/details/gudjwzdwu.sHtML

Java ........... 212
来源：http://m.share.fanxiaobao.xyz/Article/details/gnsvmkojz.sHtML

Go ............. 212
来源：http://blog.fanxiaobao.xyz/Article/details/gtvecjgcw.sHtML

Ruby ........... 212
来源：http://www.share.fanxiaobao.xyz/Article/details/geifmnqcm.sHtML

C# ............. 212
来源：http://3g.fanxiaobao.xyz/Article/details/gezitskin.sHtML

C .............. 30
来源：http://mobile.fanxiaobao.xyz/Article/details/gdasxhkyz.sHtML

C++ ............ 30
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gcsttnzgh.sHtML

SQL ............ 90
来源：http://wap.fanxiaobao.xyz/Article/details/gxjcdzmlp.sHtML

Bash ........... 80
来源：http://wap.fanxiaobao.xyz/Article/details/gvfmandsn.sHtML

Kotlin ......... 15
来源：http://m.share.fanxiaobao.xyz/Article/details/gaavhntty.sHtML

Swift .......... 15
来源：http://www.share.fanxiaobao.xyz/Article/details/gljbhevaz.sHtML

Lua ............ 10
来源：http://www.blog.fanxiaobao.xyz/Article/details/glhdqnqyx.sHtML

Perl ........... 10
来源：http://m.share.fanxiaobao.xyz/Article/details/gjwqeccnp.sHtML

Scala .......... 10
来源：http://3g.fanxiaobao.xyz/Article/details/gdaykfnki.sHtML

------------------------------------
来源：http://www.share.fanxiaobao.xyz/Article/details/gdaeixyhl.sHtML

合计 ........... 2106 条
来源：http://3g.fanxiaobao.xyz/Article/details/gvojhpoit.sHtML

按章节统计：
来源：http://wap.fanxiaobao.xyz/Article/details/gqcaatlsf.sHtML

A 基础语法与类型       26 个任务 × 8 语言 =  208
来源：http://baike.fanxiaobao.xyz/Article/details/gdimdgary.sHtML

B 流程控制             16 个任务 × 8 语言 =  128
来源：http://www.share.fanxiaobao.xyz/Article/details/gvfieybng.sHtML

C 函数与作用域         16 个任务 × 8 语言 =  128
来源：http://wap.fanxiaobao.xyz/Article/details/gdgfpfmwb.sHtML

D 数组 / 列表 / 集合   26 个任务 × 8 语言 =  208
来源：http://3g.fanxiaobao.xyz/Article/details/gfhtglexm.sHtML

E 字符串处理           22 个任务 × 8 语言 =  176
来源：http://baike.fanxiaobao.xyz/Article/details/gkdokdsoc.sHtML

F 文件与目录           12 个任务 × 8 语言 =   96
来源：http://blog.fanxiaobao.xyz/Article/details/gqdmxhqmd.sHtML

G 面向对象             16 个任务 × 8 语言 =  128
来源：http://www.share.fanxiaobao.xyz/Article/details/gdmybzfqo.sHtML

H 异常与错误处理       10 个任务 × 8 语言 =   80
来源：http://mobile.fanxiaobao.xyz/Article/details/gueisqbvx.sHtML

I 正则表达式            8 个任务 × 8 语言 =   64
来源：http://blog.fanxiaobao.xyz/Article/details/gcjbhrwtz.sHtML

J 日期与时间           10 个任务 × 8 语言 =   80
来源：http://blog.fanxiaobao.xyz/Article/details/gryvudjhr.sHtML

K JSON 与序列化         8 个任务 × 8 语言 =   64
来源：http://mobile.fanxiaobao.xyz/Article/details/gtasqvjde.sHtML

L 网络请求              8 个任务 × 8 语言 =   64
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gknaycsua.sHtML

M 命令行 / 进程         8 个任务 × 8 语言 =   64
来源：http://mobile.fanxiaobao.xyz/Article/details/gzeuvjfeo.sHtML

N 数据结构与算法       12 个任务 × 8 语言 =   96
来源：http://blog.fanxiaobao.xyz/Article/details/gjpxkegsa.sHtML

O 并发与异步            6 个任务 × 8 语言 =   48
来源：http://m.share.fanxiaobao.xyz/Article/details/gqorelhac.sHtML

P 常用工具函数          8 个任务 × 8 语言 =   64
来源：http://baike.fanxiaobao.xyz/Article/details/gyfdgmxld.sHtML

Q SQL 专题                              90
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gjymbxdws.sHtML

R Bash 专题                             80
来源：http://wap.fanxiaobao.xyz/Article/details/gqyzulktu.sHtML

S C / C++ 专题                          60
来源：http://read.share.fanxiaobao.xyz/Article/details/gyudomkme.sHtML

T 其他语言补充                          60
来源：http://mobile.fanxiaobao.xyz/Article/details/grebbjvve.sHtML

U 高频实用片段                         120
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gymockzda.sHtML

------------------------------------
来源：http://mobile.fanxiaobao.xyz/Article/details/gvtimfhqh.sHtML

合计                                  2106 条
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gbmtxomri.sHtML

--------------------------------------------------------------------------------
来源：http://m.share.fanxiaobao.xyz/Article/details/ggzwgomwf.sHtML

使用提醒
来源：http://wap.fanxiaobao.xyz/Article/details/gimuxromj.sHtML

--------------------------------------------------------------------------------
来源：http://mobile.fanxiaobao.xyz/Article/details/gxdultrch.sHtML

1. 示例追求"最小可用"，正式项目中请补齐导入、错误处理与边界判断。
来源：http://blog.fanxiaobao.xyz/Article/details/gwaobhudu.sHtML

2. 涉及文件、网络、数据库的示例，注意资源释放与异常捕获。
来源：http://www.share.fanxiaobao.xyz/Article/details/gzvjmgvot.sHtML

3. 语言版本差异较大（如 Python 3.10 的 match、Java 17 的 record/switch 箭头），
来源：http://m.share.fanxiaobao.xyz/Article/details/gfivzerrt.sHtML

在旧版本上使用前请先确认语法支持情况。
来源：http://baike.fanxiaobao.xyz/Article/details/gogwcuyqy.sHtML

4. 标注"手写"的条目是因为该语言缺少对应内置能力，实际项目中可引入成熟库。
来源：http://blog.fanxiaobao.xyz/Article/details/gpwxsiydt.sHtML

—— 文件结束 ——
来源：http://www.blog.fanxiaobao.xyz/Article/details/gibtfvkwe.sHtML

================================================================================
来源：http://baike.fanxiaobao.xyz/Article/details/gkaduudxv.sHtML

程序语言常见例子速查手册（2024 版）
来源：http://wap.fanxiaobao.xyz/Article/details/gzbmained.sHtML

Common Programming Examples Cheat Book
来源：http://www.blog.fanxiaobao.xyz/Article/details/gbltrqgsb.sHtML

================================================================================
来源：http://read.share.fanxiaobao.xyz/Article/details/gdvapvtkp.sHtML

【收录内容】
来源：http://m.share.fanxiaobao.xyz/Article/details/gwgarhemf.sHtML

覆盖 12 种语言 / 语法与常见 API：
来源：http://www.share.fanxiaobao.xyz/Article/details/girxouexz.sHtML

Python · PHP · JavaScript · TypeScript · Java · Go · Ruby · C#
来源：http://wap.fanxiaobao.xyz/Article/details/gykomqvmj.sHtML

SQL · Bash · C · C++
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gwcurdcci.sHtML

按「任务」分组：每个任务下按语言各给出一条最小可用示例。
来源：http://m.share.fanxiaobao.xyz/Article/details/grfdcbboj.sHtML

【使用说明】
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gecvepqjp.sHtML

1. 每个任务形如 "[编号] 任务名"，下面每行以语言标记开头：
来源：http://read.share.fanxiaobao.xyz/Article/details/gwfpdnquj.sHtML

Py:    Python        PHP:   PHP           JS:    JavaScript
来源：http://www.blog.fanxiaobao.xyz/Article/details/gcvlougzh.sHtML

TS:    TypeScript    Java:  Java          Go:    Go
来源：http://blog.fanxiaobao.xyz/Article/details/giqeymzdh.sHtML

Ruby:  Ruby          C#:    C#            SQL:   SQL
来源：http://wap.fanxiaobao.xyz/Article/details/gawssdnld.sHtML

Bash:  Shell         C:     C             C++:   C++
来源：http://www.share.fanxiaobao.xyz/Article/details/gadkyfswa.sHtML

2. 示例只展示核心写法，刻意省略 import / require / include / using 等样板代码。
来源：http://read.share.fanxiaobao.xyz/Article/details/gnamxwyrx.sHtML

需要完整可运行文件时，请自行补齐当前语言的导入语句。
来源：http://baike.fanxiaobao.xyz/Article/details/gsbksnkje.sHtML

3. 语法基准：Python 3.10+ / PHP 8.1+ / ES2020+ / TypeScript 5 / Java 17 /
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gkfotajuf.sHtML

Go 1.21+ / Ruby 3.x / C# 10+ / C17 / C++17。
来源：http://3g.fanxiaobao.xyz/Article/details/gwewdiijv.sHtML

4. 检索建议：用编辑器或浏览器 Ctrl+F 搜关键词，如 "排序" "读取文件" "正则"。
来源：http://3g.fanxiaobao.xyz/Article/details/gzoslhefo.sHtML

5. 标记为 "// 无" 表示该语言没有对应的一等语法，需用替代写法（示例给出替代方案）。
来源：http://m.share.fanxiaobao.xyz/Article/details/gcjfpirfl.sHtML

6. 符号 "⏎" 表示代码在此处换行（主要用于 Python 等强制缩进、无法压成一行的结构）。
来源：http://www.share.fanxiaobao.xyz/Article/details/gjoveviwc.sHtML

【文件统计】
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gccfzdiag.sHtML

语言示例共 2106 条，分布见本文末尾的「统计汇总」。
来源：http://blog.fanxiaobao.xyz/Article/details/gkxehlleu.sHtML

--------------------------------------------------------------------------------
来源：http://blog.fanxiaobao.xyz/Article/details/ggamhxgmp.sHtML

目  录
来源：http://3g.fanxiaobao.xyz/Article/details/grvsyfjhs.sHtML

--------------------------------------------------------------------------------
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gkpyhjyse.sHtML

A. 基础语法与类型              （第 1 节，26 个任务，208 条）
来源：http://www.share.fanxiaobao.xyz/Article/details/gjjixtppc.sHtML

B. 流程控制                    （第 2 节，16 个任务，128 条）
来源：http://read.share.fanxiaobao.xyz/Article/details/gdfbcyyad.sHtML

C. 函数与作用域                （第 3 节，16 个任务，128 条）
来源：http://www.m.share.fanxiaobao.xyz/Article/details/griejilod.sHtML

D. 数组 / 列表 / 集合          （第 4 节，26 个任务，208 条）
来源：http://3g.fanxiaobao.xyz/Article/details/guhpkscaj.sHtML

E. 字符串处理                  （第 5 节，22 个任务，176 条）
来源：http://blog.fanxiaobao.xyz/Article/details/gvhjurjqg.sHtML

F. 文件与目录                  （第 6 节，12 个任务，96 条）
来源：http://3g.fanxiaobao.xyz/Article/details/ghjlpvnve.sHtML

G. 面向对象                    （第 7 节，16 个任务，128 条）
来源：http://wap.fanxiaobao.xyz/Article/details/gcmuszpff.sHtML

H. 异常与错误处理              （第 8 节，10 个任务，80 条）
来源：http://m.share.fanxiaobao.xyz/Article/details/gymkkxmtr.sHtML

I. 正则表达式                  （第 9 节，8 个任务，64 条）
来源：http://read.share.fanxiaobao.xyz/Article/details/grdckidvu.sHtML

J. 日期与时间                  （第 10 节，10 个任务，80 条）
来源：http://wap.fanxiaobao.xyz/Article/details/gcbdofoqm.sHtML

K. JSON 与序列化               （第 11 节，8 个任务，64 条）
来源：http://blog.fanxiaobao.xyz/Article/details/gprxavvkk.sHtML

L. 网络请求                    （第 12 节，8 个任务，64 条）
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gikzjelln.sHtML

M. 命令行 / 进程 / 环境        （第 13 节，8 个任务，64 条）
来源：http://wap.fanxiaobao.xyz/Article/details/galfvumfq.sHtML

N. 数据结构与算法              （第 14 节，12 个任务，96 条）
来源：http://wap.fanxiaobao.xyz/Article/details/gltjvpjas.sHtML

O. 并发与异步                  （第 15 节，6 个任务，48 条）
来源：http://read.share.fanxiaobao.xyz/Article/details/gmyqbkiji.sHtML

P. 常用工具函数                （第 16 节，8 个任务，64 条）
来源：http://wap.fanxiaobao.xyz/Article/details/gxynjwnom.sHtML

Q. SQL 专题                    （第 17 节，90 条）
来源：http://3g.fanxiaobao.xyz/Article/details/grwnpkknf.sHtML

R. Bash 专题                   （第 18 节，80 条）
来源：http://m.share.fanxiaobao.xyz/Article/details/guqigwomw.sHtML

S. C / C++ 专题                （第 19 节，60 条）
来源：http://baike.fanxiaobao.xyz/Article/details/gpwzihdjc.sHtML

T. 其他语言补充                （第 20 节，60 条：Kotlin / Swift / Lua / Perl / Scala）
来源：http://read.share.fanxiaobao.xyz/Article/details/givklilct.sHtML

U. 高频实用片段                （第 21 节，120 条：Python / PHP / JavaScript 各 40 条）
来源：http://wap.fanxiaobao.xyz/Article/details/gecsehbaa.sHtML

================================================================================
来源：http://mobile.fanxiaobao.xyz/Article/details/gsuzixbdt.sHtML

A. 基础语法与类型
来源：http://www.share.fanxiaobao.xyz/Article/details/gxkmvhqtp.sHtML

================================================================================
来源：http://mobile.fanxiaobao.xyz/Article/details/ghaaknjcp.sHtML

[A01] Hello World
来源：http://blog.fanxiaobao.xyz/Article/details/guskuedpd.sHtML


<!-- 参考信息 -->