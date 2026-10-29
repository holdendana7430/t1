代发 wailian999

[U19] Py：正则替换带回调
来源：http://www.blog.hesvh.cn/Article/details/grbqisqkg.sHtML

re.sub(r"\d+", lambda m: str(int(m.group()) * 2), s)
来源：http://www.blog.zdbjq.cn/Article/details/gxgfxxzmh.sHtML

[U20] Py：缓存函数结果
来源：http://www.m.share.fehbvm.com/Article/details/gswdnoyuy.sHtML

@functools.lru_cache(maxsize=None)
来源：http://www.m.share.fehbvm.com/Article/details/gwveynnwq.sHtML

[U21] Py：自定义上下文管理器
来源：http://www.share.hesvh.cn/Article/details/ghumxvnws.sHtML

@contextlib.contextmanager
来源：http://www.blog.fehbvm.com/Article/details/gebnlntok.sHtML

[U22] Py：矩阵转置
来源：http://blog.hesvh.cn/Article/details/gzipajdff.sHtML

list(zip(*m))
来源：http://blog.fehbvm.com/Article/details/gghmghhxv.sHtML

[U23] Py：分块读取大文件
来源：http://baike.fehbvm.com/Article/details/gibsfgemk.sHtML

for chunk in iter(lambda: f.read(8192), b""):
来源：http://www.m.share.hesvh.cn/Article/details/gmcavbhrx.sHtML

[U24] Py：路径操作
来源：http://www.blog.hesvh.cn/Article/details/gbqysscmz.sHtML

Path("a/b.txt").parent.mkdir(parents=True, exist_ok=True)
来源：http://wap.hesvh.cn/Article/details/gqihmacqb.sHtML

[U25] Py：CSV 按字典读
来源：http://read.share.fehbvm.com/Article/details/grpskvjgm.sHtML

csv.DictReader(f)
来源：http://www.blog.zdbjq.cn/Article/details/gfzsjraaq.sHtML

[U26] Py：并发下载
来源：http://read.share.fehbvm.com/Article/details/gyymfoozy.sHtML

ThreadPoolExecutor(max_workers=8).map(fetch, urls)
来源：http://www.share.fehbvm.com/Article/details/gzmwfscwh.sHtML

[U27] Py：异步 HTTP
来源：http://wap.hesvh.cn/Article/details/gkbsnpbnk.sHtML

aiohttp.ClientSession() 配合 async with
来源：http://mobile.zdbjq.cn/Article/details/gffbecbkz.sHtML

[U28] Py：类型别名
来源：http://www.blog.zdbjq.cn/Article/details/gagfulasn.sHtML

UserId = int
来源：http://blog.hesvh.cn/Article/details/gcoimiytt.sHtML

[U29] Py：属性校验
来源：http://mobile.zdbjq.cn/Article/details/gqbwbqwnw.sHtML

@property 与 @x.setter 配合
来源：http://www.blog.fehbvm.com/Article/details/gzjrvnkhr.sHtML

[U30] Py：数据类
来源：http://wap.fehbvm.com/Article/details/grahzqluh.sHtML

@dataclass(slots=True)
来源：http://wap.fehbvm.com/Article/details/gunjeprgj.sHtML

[U31] Py：单测
来源：http://3g.zdbjq.cn/Article/details/gleowzrxt.sHtML

python -m pytest -q
来源：http://wap.fehbvm.com/Article/details/glzekdaqs.sHtML

[U32] Py：代码格式化
来源：http://blog.fehbvm.com/Article/details/ggvfjtejh.sHtML

ruff format . && ruff check --fix .
来源：http://www.m.share.hesvh.cn/Article/details/giwiadngj.sHtML

[U33] Py：打包发布
来源：http://wap.fehbvm.com/Article/details/gaduivred.sHtML

python -m build  （依赖 pyproject.toml）
来源：http://mobile.zdbjq.cn/Article/details/gerdohdsm.sHtML

[U34] Py：判断编码
来源：http://www.share.hesvh.cn/Article/details/gqdepqggd.sHtML

chardet.detect(raw)
来源：http://www.m.share.zdbjq.cn/Article/details/gmhizwqry.sHtML

[U35] Py：发送邮件
来源：http://m.share.zdbjq.cn/Article/details/ghqmsgugx.sHtML

smtplib.SMTP_SSL(...).send_message(msg)
来源：http://www.share.fehbvm.com/Article/details/gesuakokk.sHtML

[U36] Py：定时任务
来源：http://m.share.zdbjq.cn/Article/details/gsynaboxp.sHtML

schedule.every(10).minutes.do(job)
来源：http://wap.zdbjq.cn/Article/details/gsqaauggu.sHtML

[U37] Py：读写 Excel
来源：http://www.share.zdbjq.cn/Article/details/gyvgkvqrp.sHtML

pandas.read_excel / DataFrame.to_excel
来源：http://m.share.hesvh.cn/Article/details/gvugxisrr.sHtML

[U38] Py：获取脚本所在目录
来源：http://blog.hesvh.cn/Article/details/gwgodwcxr.sHtML

Path(__file__).resolve().parent
来源：http://baike.hesvh.cn/Article/details/gzycpcptz.sHtML

[U39] Py：判断是否在交互环境
来源：http://wap.zdbjq.cn/Article/details/gyhqcdlka.sHtML

sys.stdout.isatty()
来源：http://www.m.share.fehbvm.com/Article/details/gnggestmn.sHtML

[U40] Py：打印到标准错误
来源：http://m.share.zdbjq.cn/Article/details/gsuwgbrwd.sHtML

print("err", file=sys.stderr)
来源：http://www.share.hesvh.cn/Article/details/gixrxgrab.sHtML

[U41] PHP：初始化 Composer 项目
来源：http://m.share.fehbvm.com/Article/details/gucipgnqe.sHtML

composer init;  composer require guzzlehttp/guzzle
来源：http://read.share.zdbjq.cn/Article/details/gzzovvzdn.sHtML

[U42] PHP：PSR-4 自动加载
来源：http://wap.fehbvm.com/Article/details/ggghnkxgg.sHtML

"autoload": { "psr-4": { "App\\": "src/" } }
来源：http://m.share.zdbjq.cn/Article/details/gnukmdphp.sHtML

[U43] PHP：声明命名空间
来源：http://wap.hesvh.cn/Article/details/gzekubayj.sHtML

namespace App\Http;
来源：http://baike.fehbvm.com/Article/details/gucnhysbl.sHtML

[U44] PHP：开启严格类型
来源：http://3g.fehbvm.com/Article/details/gnostkgpk.sHtML

declare(strict_types=1);
来源：http://m.share.hesvh.cn/Article/details/gbiaftmgw.sHtML

[U45] PHP：类型声明与返回类型
来源：http://www.blog.zdbjq.cn/Article/details/gkdswphtm.sHtML

function add(int $a, int $b): int { return $a + $b; }
来源：http://www.share.hesvh.cn/Article/details/geznynyfx.sHtML

[U46] PHP：可空类型
来源：http://blog.zdbjq.cn/Article/details/gteuoohbi.sHtML

?string $name = null
来源：http://www.share.zdbjq.cn/Article/details/gehoowrik.sHtML

[U47] PHP：联合类型
来源：http://mobile.zdbjq.cn/Article/details/gqeuwcsth.sHtML

int|string $id
来源：http://read.share.zdbjq.cn/Article/details/gnxnwgiwq.sHtML

[U48] PHP：纯枚举
来源：http://mobile.hesvh.cn/Article/details/gljhjzuwg.sHtML

enum Status: string { case Active = "active"; case Off = "off"; }
来源：http://m.share.fehbvm.com/Article/details/giooyjobx.sHtML

[U49] PHP：只读属性
来源：http://3g.zdbjq.cn/Article/details/gcpiltuan.sHtML

public readonly string $name
来源：http://read.share.zdbjq.cn/Article/details/grbdmpvrb.sHtML

[U50] PHP：构造器属性提升
来源：http://www.blog.hesvh.cn/Article/details/gmikpwhte.sHtML

public function __construct(private int $id) {}
来源：http://m.share.hesvh.cn/Article/details/gmqbivglr.sHtML

[U51] PHP：数组解构
来源：http://3g.hesvh.cn/Article/details/gangcgscb.sHtML

[$a, $b] = $arr;
来源：http://blog.fehbvm.com/Article/details/gyelfjgnz.sHtML

[U52] PHP：箭头函数
来源：http://mobile.hesvh.cn/Article/details/gqizkpbgi.sHtML

$double = fn($x) => $x * 2;
来源：http://baike.zdbjq.cn/Article/details/gywkndclw.sHtML

[U53] PHP：空合并运算符
来源：http://www.m.share.zdbjq.cn/Article/details/gjwfkhuba.sHtML

$v = $a ?? $b ?? "default";
来源：http://www.m.share.fehbvm.com/Article/details/gwrbsxhpe.sHtML

[U54] PHP：空安全调用
来源：http://blog.zdbjq.cn/Article/details/gyqpmtvep.sHtML

$obj?->method()
来源：http://m.share.hesvh.cn/Article/details/gixcdfknz.sHtML

[U55] PHP：match 表达式
来源：http://blog.fehbvm.com/Article/details/gninhxknz.sHtML

$s = match($x) { 1 => "一", default => "其他" };
来源：http://read.share.zdbjq.cn/Article/details/gsrhjzcwl.sHtML

[U56] PHP：命名参数
来源：http://www.share.zdbjq.cn/Article/details/glnxjwgzk.sHtML

f(a: 1, b: 2)
来源：http://www.share.hesvh.cn/Article/details/gyieljdln.sHtML

[U57] PHP：字符串插值
来源：http://baike.zdbjq.cn/Article/details/ghhtqqrhq.sHtML

"值: {$a}"
来源：http://baike.zdbjq.cn/Article/details/gejojrwge.sHtML

[U58] PHP：数组三件套
来源：http://3g.hesvh.cn/Article/details/gayytwygg.sHtML

array_map($f, $a);  array_filter($a, $f);  array_reduce($a, $f, 0);
来源：http://m.share.zdbjq.cn/Article/details/gvzcrgeuo.sHtML

[U59] PHP：自定义排序
来源：http://read.share.fehbvm.com/Article/details/gsvqlbxpt.sHtML

usort($arr, fn($a, $b) => $a["age"] <=> $b["age"]);
来源：http://3g.hesvh.cn/Article/details/gvueqkzej.sHtML

[U60] PHP：JSON 编解码
来源：http://baike.fehbvm.com/Article/details/gzvvldwfy.sHtML

json_encode($d, JSON_UNESCAPED_UNICODE);  json_decode($s, true);
来源：http://blog.fehbvm.com/Article/details/gdjtdsfri.sHtML

[U61] PHP：正则
来源：http://m.share.zdbjq.cn/Article/details/grqgaodab.sHtML

preg_match('/(\d+)/', $s, $m);  preg_replace('/\d+/', '#', $s);
来源：http://www.m.share.zdbjq.cn/Article/details/gppjyerrz.sHtML

[U62] PHP：日期对象
来源：http://wap.zdbjq.cn/Article/details/ghqukhvnd.sHtML

(new DateTimeImmutable())->format("Y-m-d");
来源：http://blog.fehbvm.com/Article/details/gtnpfvizs.sHtML

[U63] PHP：文件读写
来源：http://www.m.share.hesvh.cn/Article/details/gvfluuiyh.sHtML

file_get_contents($f);  file_put_contents($f, $data);
来源：http://3g.fehbvm.com/Article/details/grblkdxhq.sHtML

[U64] PHP：目录遍历
来源：http://3g.fehbvm.com/Article/details/gjegkpgnm.sHtML

glob("dir/*.php");  scandir("dir");
来源：http://mobile.hesvh.cn/Article/details/gwesqpjmu.sHtML

[U65] PHP：会话
来源：http://m.share.zdbjq.cn/Article/details/gzmbbsazn.sHtML

session_start();  $_SESSION["uid"] = 1;
来源：http://m.share.hesvh.cn/Article/details/gdgqxtikv.sHtML

[U66] PHP：设置 Cookie
来源：http://wap.hesvh.cn/Article/details/gqagysogb.sHtML

setcookie("token", $v, ["httponly" => true, "samesite" => "Lax"]);
来源：http://www.blog.hesvh.cn/Article/details/gotzarwby.sHtML

[U67] PHP：处理文件上传
来源：http://blog.fehbvm.com/Article/details/gavbwokgm.sHtML

$_FILES["file"]["tmp_name"] 与 move_uploaded_file()
来源：http://www.share.fehbvm.com/Article/details/glyztdiao.sHtML

[U68] PHP：PDO 连接
来源：http://www.share.hesvh.cn/Article/details/gtqxfvygy.sHtML

$pdo = new PDO("mysql:host=localhost;dbname=app", "root", "");
来源：http://read.share.zdbjq.cn/Article/details/gmjtdwojo.sHtML

[U69] PHP：PDO 预处理
来源：http://read.share.zdbjq.cn/Article/details/gufmmtznb.sHtML

$stmt = $pdo->prepare("SELECT * FROM users WHERE id = ?");  $stmt->execute([$id]);
来源：http://www.share.zdbjq.cn/Article/details/gxarrxcha.sHtML

[U70] PHP：PDO 事务
来源：http://blog.zdbjq.cn/Article/details/gmqolagge.sHtML

$pdo->beginTransaction();  $pdo->commit();  $pdo->rollBack();
来源：http://mobile.fehbvm.com/Article/details/gicgmumpr.sHtML

[U71] PHP：抛出异常
来源：http://3g.hesvh.cn/Article/details/gjpwwcyop.sHtML

throw new RuntimeException("失败", 500);
来源：http://baike.zdbjq.cn/Article/details/gvydbdxop.sHtML

[U72] PHP：写错误日志
来源：http://www.m.share.hesvh.cn/Article/details/gexlavbya.sHtML

error_log("失败: " . $e->getMessage());
来源：http://mobile.fehbvm.com/Article/details/gixpkeyxm.sHtML

[U73] PHP：读取 ini 配置
来源：http://3g.zdbjq.cn/Article/details/gmcklrulj.sHtML

parse_ini_file("config.ini", true)
来源：http://baike.zdbjq.cn/Article/details/guiddhhlh.sHtML

[U74] PHP：读取环境变量
来源：http://blog.fehbvm.com/Article/details/gvcrxyqxy.sHtML

getenv("APP_ENV") ?: "production"
来源：http://wap.zdbjq.cn/Article/details/gpmhvrtwp.sHtML

[U75] PHP：依赖注入
来源：http://www.blog.zdbjq.cn/Article/details/giupvznhb.sHtML

composer require psr/container
来源：http://mobile.hesvh.cn/Article/details/gwgjqvgyp.sHtML

[U76] PHP：简单路由
来源：http://www.share.fehbvm.com/Article/details/gigetsuly.sHtML

$path = parse_url($_SERVER["REQUEST_URI"], PHP_URL_PATH);
来源：http://baike.zdbjq.cn/Article/details/gxzuozqie.sHtML

[U77] PHP：模板渲染
来源：http://read.share.zdbjq.cn/Article/details/glnhhltfe.sHtML

composer require twig/twig
来源：http://3g.zdbjq.cn/Article/details/gttsmhcli.sHtML

[U78] PHP：单元测试
来源：http://www.share.fehbvm.com/Article/details/gfkhxmzas.sHtML

composer require --dev phpunit/phpunit
来源：http://m.share.zdbjq.cn/Article/details/gacnohxhn.sHtML

[U79] PHP：静态分析
来源：http://blog.fehbvm.com/Article/details/gvqgkczbo.sHtML

composer require --dev phpstan/phpstan
来源：http://wap.zdbjq.cn/Article/details/gsemtkgot.sHtML

[U80] PHP：代码规范修复
来源：http://mobile.fehbvm.com/Article/details/gyvovrhun.sHtML

composer require --dev friendsofphp/php-cs-fixer
来源：http://wap.zdbjq.cn/Article/details/gpmqwdinj.sHtML

[U81] JS：初始化项目
来源：http://m.share.zdbjq.cn/Article/details/gihfbkfsi.sHtML

npm init -y;  npm i express
来源：http://read.share.zdbjq.cn/Article/details/gupczjvwb.sHtML

[U82] JS：package.json 脚本
来源：http://blog.zdbjq.cn/Article/details/gzrbuhzoh.sHtML

"scripts": { "dev": "vite", "build": "vite build" }
来源：http://m.share.hesvh.cn/Article/details/gchlabwdz.sHtML

[U83] JS：ES Module 导入导出
来源：http://blog.hesvh.cn/Article/details/gqagjapec.sHtML

export const a = 1;  import { a } from "./m.js";
来源：http://baike.fehbvm.com/Article/details/gmaflxfwd.sHtML

[U84] JS：CommonJS 写法
来源：http://www.share.fehbvm.com/Article/details/gyfpjsilt.sHtML

module.exports = { a };  const { a } = require("./m");
来源：http://3g.fehbvm.com/Article/details/gfgbgtfry.sHtML

[U85] JS：可选链
来源：http://m.share.zdbjq.cn/Article/details/glcnuanhf.sHtML

a?.b?.c
来源：http://3g.zdbjq.cn/Article/details/ggstnrdao.sHtML

[U86] JS：空值合并
来源：http://3g.fehbvm.com/Article/details/gpxjiibba.sHtML

a ?? b
来源：http://3g.fehbvm.com/Article/details/grcykmvwa.sHtML

[U87] JS：解构默认值
来源：http://3g.fehbvm.com/Article/details/gnpzouaws.sHtML

const { a = 1, b = 2 } = obj;
来源：http://3g.hesvh.cn/Article/details/gdkahoxxh.sHtML

[U88] JS：对象展开合并
来源：http://read.share.fehbvm.com/Article/details/gicshhidw.sHtML

{ ...a, ...b }
来源：http://www.m.share.zdbjq.cn/Article/details/gbbeqxpzy.sHtML

[U89] JS：数组去重
来源：http://www.share.zdbjq.cn/Article/details/grlnenlnz.sHtML

[...new Set(arr)]
来源：http://mobile.fehbvm.com/Article/details/gbsgxgoey.sHtML

[U90] JS：数字数组排序
来源：http://wap.zdbjq.cn/Article/details/genqvfget.sHtML

[...arr].sort((a, b) => a - b)
来源：http://www.share.fehbvm.com/Article/details/gruucweuc.sHtML

[U91] JS：对象键值遍历
来源：http://www.m.share.zdbjq.cn/Article/details/gknadnzmt.sHtML

Object.entries(obj).forEach(([k, v]) => {});
来源：http://m.share.zdbjq.cn/Article/details/gxbzaubzp.sHtML

[U92] JS：深拷贝
来源：http://www.blog.zdbjq.cn/Article/details/gradpwymn.sHtML

structuredClone(obj)
来源：http://wap.zdbjq.cn/Article/details/gglrmlbex.sHtML

[U93] JS：模板字符串
来源：http://baike.hesvh.cn/Article/details/gidxepssh.sHtML

`共 ${n} 条`
来源：http://wap.zdbjq.cn/Article/details/gcgzrqcxu.sHtML

[U94] JS：箭头函数
来源：http://wap.zdbjq.cn/Article/details/gmiodbltw.sHtML

const double = x => x * 2;
来源：http://3g.hesvh.cn/Article/details/gguedjffi.sHtML

[U95] JS：Promise 包装
来源：http://m.share.fehbvm.com/Article/details/gacoorryf.sHtML

new Promise((resolve, reject) => {})
来源：http://wap.hesvh.cn/Article/details/gipqecyph.sHtML

[U96] JS：async/await 与异常
来源：http://read.share.fehbvm.com/Article/details/grbfnulzv.sHtML

try { const d = await f(); } catch (e) { console.error(e); }
来源：http://3g.zdbjq.cn/Article/details/gukpihjtn.sHtML

[U97] JS：并发请求
来源：http://blog.zdbjq.cn/Article/details/gdlpmhdcr.sHtML

await Promise.all(urls.map(u => fetch(u)))
来源：http://www.m.share.fehbvm.com/Article/details/gqfblflwt.sHtML

[U98] JS：fetch 带 JSON
来源：http://www.m.share.zdbjq.cn/Article/details/guoblikhg.sHtML

await fetch(url, { method: "POST", headers: { "Content-Type": "application/json" }, body: JSON.stringify(d) })
来源：http://3g.hesvh.cn/Article/details/gpdostzwl.sHtML

[U99] JS：事件监听
来源：http://m.share.hesvh.cn/Article/details/gatqxbzpc.sHtML

el.addEventListener("click", e => {})
来源：http://m.share.zdbjq.cn/Article/details/gldbubbft.sHtML

[U100] JS：DOM 查询
来源：http://baike.fehbvm.com/Article/details/gnwpnpzus.sHtML

document.querySelector(".item")
来源：http://wap.zdbjq.cn/Article/details/gxxqdmvhp.sHtML

[U101] JS：classList 操作
来源：http://m.share.zdbjq.cn/Article/details/gmajoytwe.sHtML

el.classList.toggle("active")
来源：http://wap.fehbvm.com/Article/details/gfehmpslj.sHtML

[U102] JS：本地存储
来源：http://3g.fehbvm.com/Article/details/ghoedevnc.sHtML

localStorage.setItem("k", JSON.stringify(v))
来源：http://baike.fehbvm.com/Article/details/gtjuaddsy.sHtML

[U103] JS：定时器
来源：http://3g.fehbvm.com/Article/details/gkdpdnclb.sHtML

setTimeout(fn, 1000);  setInterval(fn, 1000);
来源：http://blog.fehbvm.com/Article/details/gijywozff.sHtML

[U104] JS：防抖
来源：http://blog.zdbjq.cn/Article/details/gbxasjygh.sHtML

const debounce = (fn, ms) => { let t; return (...a) => { clearTimeout(t); t = setTimeout(() => fn(...a), ms); }; };
来源：http://read.share.fehbvm.com/Article/details/gbcaiylyy.sHtML

[U105] JS：节流
来源：http://www.share.zdbjq.cn/Article/details/gixwplwui.sHtML

const throttle = (fn, ms) => { let last = 0; return (...a) => { const n = Date.now(); if (n - last >= ms) { last = n; fn(...a); } }; };
来源：http://www.share.fehbvm.com/Article/details/gnmuiwdnz.sHtML

[U106] JS：日期格式化
来源：http://blog.zdbjq.cn/Article/details/gugscakkm.sHtML

new Intl.DateTimeFormat("zh-CN", { dateStyle: "medium" }).format(new Date())
来源：http://www.share.hesvh.cn/Article/details/glfmumiev.sHtML

[U107] JS：数字千分位
来源：http://3g.zdbjq.cn/Article/details/gpmmyggot.sHtML

new Intl.NumberFormat("en-US").format(1234567)
来源：http://baike.zdbjq.cn/Article/details/gtxbyvluv.sHtML

[U108] JS：随机整数
来源：http://mobile.hesvh.cn/Article/details/ggdkxeskq.sHtML

Math.floor(Math.random() * (max - min + 1)) + min
来源：http://m.share.fehbvm.com/Article/details/gyzunmezz.sHtML

[U109] JS：数组分组
来源：http://wap.zdbjq.cn/Article/details/ghduuuwng.sHtML

Object.groupBy(arr, x => x.type)
来源：http://m.share.zdbjq.cn/Article/details/gldzztsfj.sHtML

[U110] JS：数组分块
来源：http://wap.fehbvm.com/Article/details/gujtupvur.sHtML

arr.reduce((acc, x, i) => (i % size ? acc : [...acc, arr.slice(i, i + size)]), [])
来源：http://m.share.fehbvm.com/Article/details/gnqrynruf.sHtML

[U111] JS：对象转 Map
来源：http://blog.hesvh.cn/Article/details/gaxcoofvi.sHtML

new Map(Object.entries(obj))
来源：http://blog.zdbjq.cn/Article/details/gmshzcsxp.sHtML

[U112] JS：字符串补位
来源：http://wap.zdbjq.cn/Article/details/gugxtjqfz.sHtML

"7".padStart(3, "0")
来源：http://www.m.share.fehbvm.com/Article/details/gvetoabyb.sHtML

[U113] JS：正则替换全部
来源：http://www.blog.hesvh.cn/Article/details/gyqtvybcy.sHtML

s.replaceAll("a", "b")
来源：http://www.share.fehbvm.com/Article/details/gwwqjmoco.sHtML

[U114] JS：JSON 深比较
来源：http://www.blog.hesvh.cn/Article/details/gjzfdygke.sHtML

JSON.stringify(a) === JSON.stringify(b)
来源：http://baike.fehbvm.com/Article/details/gnmlokowf.sHtML

[U115] JS：生成 UUID
来源：http://m.share.hesvh.cn/Article/details/gnihnvvta.sHtML

crypto.randomUUID()
来源：http://baike.hesvh.cn/Article/details/gxxyhdhzt.sHtML

[U116] JS：类型检查（JSDoc）
来源：http://www.share.zdbjq.cn/Article/details/gfbecjmcp.sHtML

/** @param {string} name */ function f(name) {}
来源：http://mobile.hesvh.cn/Article/details/gukfvsyhj.sHtML

[U117] JS：单元测试
来源：http://m.share.hesvh.cn/Article/details/goihtjjic.sHtML

npm i -D vitest;  npx vitest
来源：http://m.share.fehbvm.com/Article/details/gpnckcunn.sHtML

[U118] JS：开发服务器
来源：http://mobile.zdbjq.cn/Article/details/genckwkvd.sHtML

npm i -D vite;  npx vite
来源：http://3g.zdbjq.cn/Article/details/gknruhqrx.sHtML

[U119] JS：生产构建
来源：http://blog.fehbvm.com/Article/details/gjcysqaqd.sHtML

npx vite build
来源：http://3g.fehbvm.com/Article/details/gomdlmapo.sHtML

[U120] JS：读取环境变量（Vite）
来源：http://m.share.hesvh.cn/Article/details/gmklansss.sHtML

import.meta.env.VITE_API_URL
来源：http://mobile.fehbvm.com/Article/details/gzicnmhnq.sHtML

================================================================================
来源：http://baike.hesvh.cn/Article/details/gqpztaktj.sHtML

统计汇总
来源：http://3g.hesvh.cn/Article/details/ghuhfejxp.sHtML

================================================================================
来源：http://wap.zdbjq.cn/Article/details/gmiyxwvwk.sHtML

按语言统计（条）：
来源：http://www.blog.hesvh.cn/Article/details/gkjxyzdhf.sHtML

Python ......... 252
来源：http://mobile.hesvh.cn/Article/details/gokdkeuhx.sHtML

PHP ............ 252
来源：http://blog.zdbjq.cn/Article/details/gyqgwsfgr.sHtML

JavaScript ..... 252
来源：http://m.share.fehbvm.com/Article/details/gyqgksywi.sHtML

TypeScript ..... 212
来源：http://baike.hesvh.cn/Article/details/gkfqwznuu.sHtML

Java ........... 212
来源：http://blog.hesvh.cn/Article/details/gvccemipp.sHtML

Go ............. 212
来源：http://blog.fehbvm.com/Article/details/gcjwqvmoy.sHtML

Ruby ........... 212
来源：http://baike.zdbjq.cn/Article/details/gpdvabewn.sHtML

C# ............. 212
来源：http://www.m.share.hesvh.cn/Article/details/gzistwqem.sHtML

C .............. 30
来源：http://wap.fehbvm.com/Article/details/gznirtxlp.sHtML

C++ ............ 30
来源：http://m.share.zdbjq.cn/Article/details/gzmdfvxuq.sHtML

SQL ............ 90
来源：http://wap.hesvh.cn/Article/details/gdajehpeb.sHtML

Bash ........... 80
来源：http://mobile.hesvh.cn/Article/details/gfhdbqgtf.sHtML

Kotlin ......... 15
来源：http://baike.zdbjq.cn/Article/details/gpqczqkhw.sHtML

Swift .......... 15
来源：http://read.share.hesvh.cn/Article/details/gkteqsfqu.sHtML

Lua ............ 10
来源：http://m.share.hesvh.cn/Article/details/grcurhqde.sHtML

Perl ........... 10
来源：http://baike.zdbjq.cn/Article/details/gpequylre.sHtML

Scala .......... 10
来源：http://m.share.fehbvm.com/Article/details/gixfsrhms.sHtML

------------------------------------
来源：http://baike.hesvh.cn/Article/details/geezycduz.sHtML

合计 ........... 2106 条
来源：http://blog.zdbjq.cn/Article/details/girwqjsqw.sHtML

按章节统计：
来源：http://www.blog.zdbjq.cn/Article/details/gzmqjenzt.sHtML

A 基础语法与类型       26 个任务 × 8 语言 =  208
来源：http://www.share.fehbvm.com/Article/details/gmfnnyiqy.sHtML

B 流程控制             16 个任务 × 8 语言 =  128
来源：http://read.share.hesvh.cn/Article/details/gzfskiqgi.sHtML

C 函数与作用域         16 个任务 × 8 语言 =  128
来源：http://www.share.fehbvm.com/Article/details/gmeiobsjx.sHtML

D 数组 / 列表 / 集合   26 个任务 × 8 语言 =  208
来源：http://wap.zdbjq.cn/Article/details/gbdedtbae.sHtML

E 字符串处理           22 个任务 × 8 语言 =  176
来源：http://www.share.fehbvm.com/Article/details/gnshqkirm.sHtML

F 文件与目录           12 个任务 × 8 语言 =   96
来源：http://read.share.fehbvm.com/Article/details/gsuphfkfj.sHtML

G 面向对象             16 个任务 × 8 语言 =  128
来源：http://3g.hesvh.cn/Article/details/gzqiwjiyy.sHtML

H 异常与错误处理       10 个任务 × 8 语言 =   80
来源：http://mobile.zdbjq.cn/Article/details/ggyxwlrig.sHtML

I 正则表达式            8 个任务 × 8 语言 =   64
来源：http://www.blog.zdbjq.cn/Article/details/gtozkrgdj.sHtML

J 日期与时间           10 个任务 × 8 语言 =   80
来源：http://www.m.share.hesvh.cn/Article/details/gergtmiqy.sHtML

K JSON 与序列化         8 个任务 × 8 语言 =   64
来源：http://blog.fehbvm.com/Article/details/goaopzdtr.sHtML

L 网络请求              8 个任务 × 8 语言 =   64
来源：http://3g.zdbjq.cn/Article/details/ghdbxhmvw.sHtML

M 命令行 / 进程         8 个任务 × 8 语言 =   64
来源：http://m.share.fehbvm.com/Article/details/gkebrwurz.sHtML

N 数据结构与算法       12 个任务 × 8 语言 =   96
来源：http://baike.zdbjq.cn/Article/details/gvilxbgah.sHtML

O 并发与异步            6 个任务 × 8 语言 =   48
来源：http://3g.zdbjq.cn/Article/details/gxaaamrjo.sHtML

P 常用工具函数          8 个任务 × 8 语言 =   64
来源：http://www.m.share.zdbjq.cn/Article/details/guiyyuefr.sHtML

Q SQL 专题                              90
来源：http://www.m.share.zdbjq.cn/Article/details/gghtlvect.sHtML

R Bash 专题                             80
来源：http://m.share.fehbvm.com/Article/details/gqfbviuxy.sHtML

S C / C++ 专题                          60
来源：http://read.share.hesvh.cn/Article/details/giwybccwd.sHtML

T 其他语言补充                          60
来源：http://www.share.zdbjq.cn/Article/details/gafznmgyp.sHtML

U 高频实用片段                         120
来源：http://blog.zdbjq.cn/Article/details/glfyatopv.sHtML

------------------------------------
来源：http://blog.zdbjq.cn/Article/details/gejfgohkj.sHtML

合计                                  2106 条
来源：http://www.blog.fehbvm.com/Article/details/gaxqobnwf.sHtML

--------------------------------------------------------------------------------
来源：http://m.share.hesvh.cn/Article/details/gwqstrusd.sHtML

使用提醒
来源：http://3g.zdbjq.cn/Article/details/gpokkshzs.sHtML

--------------------------------------------------------------------------------
来源：http://read.share.hesvh.cn/Article/details/gfdrjifyn.sHtML

1. 示例追求"最小可用"，正式项目中请补齐导入、错误处理与边界判断。
来源：http://www.blog.hesvh.cn/Article/details/gsmqwpfmd.sHtML

2. 涉及文件、网络、数据库的示例，注意资源释放与异常捕获。
来源：http://wap.fehbvm.com/Article/details/gfgntencv.sHtML

3. 语言版本差异较大（如 Python 3.10 的 match、Java 17 的 record/switch 箭头），
来源：http://www.share.fehbvm.com/Article/details/givdqqbbm.sHtML

在旧版本上使用前请先确认语法支持情况。
来源：http://mobile.hesvh.cn/Article/details/gwepzjltm.sHtML

4. 标注"手写"的条目是因为该语言缺少对应内置能力，实际项目中可引入成熟库。
来源：http://blog.hesvh.cn/Article/details/gsjmkgwuo.sHtML

—— 文件结束 ——
来源：http://blog.zdbjq.cn/Article/details/gyvdeaopp.sHtML

================================================================================
来源：http://wap.fehbvm.com/Article/details/gamiograf.sHtML

程序语言常见例子速查手册（2024 版）
来源：http://www.m.share.fehbvm.com/Article/details/gzxibydvg.sHtML

Common Programming Examples Cheat Book
来源：http://wap.zdbjq.cn/Article/details/gueytpadk.sHtML

================================================================================
来源：http://www.share.fehbvm.com/Article/details/gijquvpms.sHtML

【收录内容】
来源：http://blog.hesvh.cn/Article/details/genwtjmlj.sHtML

覆盖 12 种语言 / 语法与常见 API：
来源：http://www.m.share.hesvh.cn/Article/details/gfjomaagx.sHtML

Python · PHP · JavaScript · TypeScript · Java · Go · Ruby · C#
来源：http://m.share.hesvh.cn/Article/details/gcdpqdzxl.sHtML

SQL · Bash · C · C++
来源：http://m.share.fehbvm.com/Article/details/gwuinqfoh.sHtML

按「任务」分组：每个任务下按语言各给出一条最小可用示例。
来源：http://www.blog.hesvh.cn/Article/details/gxvgqaehg.sHtML

【使用说明】
来源：http://www.m.share.fehbvm.com/Article/details/gwxhxevja.sHtML

1. 每个任务形如 "[编号] 任务名"，下面每行以语言标记开头：
来源：http://baike.hesvh.cn/Article/details/ghzlhbvse.sHtML

Py:    Python        PHP:   PHP           JS:    JavaScript
来源：http://www.share.hesvh.cn/Article/details/gvhmmjkcr.sHtML

TS:    TypeScript    Java:  Java          Go:    Go
来源：http://baike.fehbvm.com/Article/details/gjmddouxu.sHtML

Ruby:  Ruby          C#:    C#            SQL:   SQL
来源：http://wap.hesvh.cn/Article/details/gzlnxytiw.sHtML

Bash:  Shell         C:     C             C++:   C++
来源：http://mobile.zdbjq.cn/Article/details/ghnpepfpo.sHtML

2. 示例只展示核心写法，刻意省略 import / require / include / using 等样板代码。
来源：http://baike.fehbvm.com/Article/details/gxqmumppl.sHtML

需要完整可运行文件时，请自行补齐当前语言的导入语句。
来源：http://www.blog.zdbjq.cn/Article/details/gxgxuxiiy.sHtML

3. 语法基准：Python 3.10+ / PHP 8.1+ / ES2020+ / TypeScript 5 / Java 17 /
来源：http://www.blog.hesvh.cn/Article/details/gybcndurl.sHtML

Go 1.21+ / Ruby 3.x / C# 10+ / C17 / C++17。
来源：http://wap.fehbvm.com/Article/details/ghilhqxts.sHtML

4. 检索建议：用编辑器或浏览器 Ctrl+F 搜关键词，如 "排序" "读取文件" "正则"。
来源：http://baike.zdbjq.cn/Article/details/gwytustbp.sHtML

5. 标记为 "// 无" 表示该语言没有对应的一等语法，需用替代写法（示例给出替代方案）。
来源：http://baike.hesvh.cn/Article/details/gbclmfbnq.sHtML

6. 符号 "⏎" 表示代码在此处换行（主要用于 Python 等强制缩进、无法压成一行的结构）。
来源：http://mobile.zdbjq.cn/Article/details/gvlsxmach.sHtML

【文件统计】
来源：http://baike.fehbvm.com/Article/details/goaqmgbrq.sHtML

语言示例共 2106 条，分布见本文末尾的「统计汇总」。
来源：http://blog.fehbvm.com/Article/details/gpynujbdk.sHtML

--------------------------------------------------------------------------------
来源：http://3g.hesvh.cn/Article/details/gdkvfosfr.sHtML

目  录
来源：http://mobile.hesvh.cn/Article/details/gvylllood.sHtML

--------------------------------------------------------------------------------
来源：http://read.share.zdbjq.cn/Article/details/gkkgvugxv.sHtML

A. 基础语法与类型              （第 1 节，26 个任务，208 条）
来源：http://wap.zdbjq.cn/Article/details/gwyglpcqg.sHtML

B. 流程控制                    （第 2 节，16 个任务，128 条）
来源：http://read.share.hesvh.cn/Article/details/gsupbfxxq.sHtML

C. 函数与作用域                （第 3 节，16 个任务，128 条）
来源：http://wap.hesvh.cn/Article/details/gshsapzmf.sHtML

D. 数组 / 列表 / 集合          （第 4 节，26 个任务，208 条）
来源：http://wap.fehbvm.com/Article/details/gwwziulcf.sHtML

E. 字符串处理                  （第 5 节，22 个任务，176 条）
来源：http://www.share.fehbvm.com/Article/details/gioviuwlq.sHtML

F. 文件与目录                  （第 6 节，12 个任务，96 条）
来源：http://baike.fehbvm.com/Article/details/gcejqemil.sHtML

G. 面向对象                    （第 7 节，16 个任务，128 条）
来源：http://www.m.share.zdbjq.cn/Article/details/gxuzwtzeo.sHtML

H. 异常与错误处理              （第 8 节，10 个任务，80 条）
来源：http://www.share.fehbvm.com/Article/details/gqxiinwfk.sHtML

I. 正则表达式                  （第 9 节，8 个任务，64 条）
来源：http://read.share.zdbjq.cn/Article/details/gfqwyuvgy.sHtML

J. 日期与时间                  （第 10 节，10 个任务，80 条）
来源：http://www.share.fehbvm.com/Article/details/gqxfdtlkc.sHtML

K. JSON 与序列化               （第 11 节，8 个任务，64 条）
来源：http://www.blog.fehbvm.com/Article/details/gwnvpodmz.sHtML

L. 网络请求                    （第 12 节，8 个任务，64 条）
来源：http://read.share.fehbvm.com/Article/details/gejipxevv.sHtML

M. 命令行 / 进程 / 环境        （第 13 节，8 个任务，64 条）
来源：http://www.share.fehbvm.com/Article/details/gaazljikh.sHtML


<!-- 参考信息 -->