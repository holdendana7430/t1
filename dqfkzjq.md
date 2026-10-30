代发 wailian999

[U17] Py：初始化日志
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gocecrqxg.sHtML

logging.basicConfig(level=logging.INFO)
来源：http://mobile.fanxiaobao.xyz/Article/details/gtxzdesfk.sHtML

[U18] Py：预编译正则
来源：http://baike.fanxiaobao.xyz/Article/details/gpccslger.sHtML

pat = re.compile(r"\d+")
来源：http://m.share.fanxiaobao.xyz/Article/details/gpqghfsfj.sHtML

[U19] Py：正则替换带回调
来源：http://3g.fanxiaobao.xyz/Article/details/gosdfplhn.sHtML

re.sub(r"\d+", lambda m: str(int(m.group()) * 2), s)
来源：http://www.blog.fanxiaobao.xyz/Article/details/gxtfezwuj.sHtML

[U20] Py：缓存函数结果
来源：http://www.blog.fanxiaobao.xyz/Article/details/gglcuwsbw.sHtML

@functools.lru_cache(maxsize=None)
来源：http://3g.fanxiaobao.xyz/Article/details/gdarzwcrj.sHtML

[U21] Py：自定义上下文管理器
来源：http://www.share.fanxiaobao.xyz/Article/details/gjoeovmbf.sHtML

@contextlib.contextmanager
来源：http://wap.fanxiaobao.xyz/Article/details/gdfrlsuff.sHtML

[U22] Py：矩阵转置
来源：http://blog.fanxiaobao.xyz/Article/details/gopmqjgxb.sHtML

list(zip(*m))
来源：http://m.share.fanxiaobao.xyz/Article/details/gsyusnnvr.sHtML

[U23] Py：分块读取大文件
来源：http://3g.fanxiaobao.xyz/Article/details/gfspetxhh.sHtML

for chunk in iter(lambda: f.read(8192), b""):
来源：http://www.blog.fanxiaobao.xyz/Article/details/gafrcsiyw.sHtML

[U24] Py：路径操作
来源：http://m.share.fanxiaobao.xyz/Article/details/gwhlyicsq.sHtML

Path("a/b.txt").parent.mkdir(parents=True, exist_ok=True)
来源：http://m.share.fanxiaobao.xyz/Article/details/gkxjftwgy.sHtML

[U25] Py：CSV 按字典读
来源：http://3g.fanxiaobao.xyz/Article/details/gjkbvvtwj.sHtML

csv.DictReader(f)
来源：http://baike.fanxiaobao.xyz/Article/details/gkhutjgbg.sHtML

[U26] Py：并发下载
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gmudpslxe.sHtML

ThreadPoolExecutor(max_workers=8).map(fetch, urls)
来源：http://www.share.fanxiaobao.xyz/Article/details/glcnuftpg.sHtML

[U27] Py：异步 HTTP
来源：http://3g.fanxiaobao.xyz/Article/details/ggvhmhytw.sHtML

aiohttp.ClientSession() 配合 async with
来源：http://3g.fanxiaobao.xyz/Article/details/gqvisoyot.sHtML

[U28] Py：类型别名
来源：http://baike.fanxiaobao.xyz/Article/details/gdolnbafh.sHtML

UserId = int
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gvkgcbgbq.sHtML

[U29] Py：属性校验
来源：http://read.share.fanxiaobao.xyz/Article/details/glxuwzoaa.sHtML

@property 与 @x.setter 配合
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gaonpowrf.sHtML

[U30] Py：数据类
来源：http://wap.fanxiaobao.xyz/Article/details/gpzseeotk.sHtML

@dataclass(slots=True)
来源：http://blog.fanxiaobao.xyz/Article/details/gphbvdvel.sHtML

[U31] Py：单测
来源：http://www.share.fanxiaobao.xyz/Article/details/gojzprouj.sHtML

python -m pytest -q
来源：http://3g.fanxiaobao.xyz/Article/details/gwnnbovew.sHtML

[U32] Py：代码格式化
来源：http://baike.fanxiaobao.xyz/Article/details/ghdcuydcb.sHtML

ruff format . && ruff check --fix .
来源：http://www.share.fanxiaobao.xyz/Article/details/gkqdygwbg.sHtML

[U33] Py：打包发布
来源：http://mobile.fanxiaobao.xyz/Article/details/gynlyodql.sHtML

python -m build  （依赖 pyproject.toml）
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gpudaxblo.sHtML

[U34] Py：判断编码
来源：http://www.share.fanxiaobao.xyz/Article/details/gmwbuntey.sHtML

chardet.detect(raw)
来源：http://www.blog.fanxiaobao.xyz/Article/details/gndrauqdu.sHtML

[U35] Py：发送邮件
来源：http://baike.fanxiaobao.xyz/Article/details/gederqxox.sHtML

smtplib.SMTP_SSL(...).send_message(msg)
来源：http://read.share.fanxiaobao.xyz/Article/details/gvdavfxpb.sHtML

[U36] Py：定时任务
来源：http://baike.fanxiaobao.xyz/Article/details/gvivndwan.sHtML

schedule.every(10).minutes.do(job)
来源：http://wap.fanxiaobao.xyz/Article/details/gzegczknd.sHtML

[U37] Py：读写 Excel
来源：http://blog.fanxiaobao.xyz/Article/details/gykzicrak.sHtML

pandas.read_excel / DataFrame.to_excel
来源：http://www.share.fanxiaobao.xyz/Article/details/guilrzqqe.sHtML

[U38] Py：获取脚本所在目录
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gvsxycarl.sHtML

Path(__file__).resolve().parent
来源：http://read.share.fanxiaobao.xyz/Article/details/gvshwmbqe.sHtML

[U39] Py：判断是否在交互环境
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gwfwdnqaj.sHtML

sys.stdout.isatty()
来源：http://www.share.fanxiaobao.xyz/Article/details/gzekqzhrx.sHtML

[U40] Py：打印到标准错误
来源：http://blog.fanxiaobao.xyz/Article/details/gjruznfgz.sHtML

print("err", file=sys.stderr)
来源：http://m.share.fanxiaobao.xyz/Article/details/gqhfzmzie.sHtML

[U41] PHP：初始化 Composer 项目
来源：http://blog.fanxiaobao.xyz/Article/details/gygfhqgqb.sHtML

composer init;  composer require guzzlehttp/guzzle
来源：http://m.share.fanxiaobao.xyz/Article/details/gnxyimsib.sHtML

[U42] PHP：PSR-4 自动加载
来源：http://www.blog.fanxiaobao.xyz/Article/details/gvbvcpkrq.sHtML

"autoload": { "psr-4": { "App\\": "src/" } }
来源：http://m.share.fanxiaobao.xyz/Article/details/glnnvemhp.sHtML

[U43] PHP：声明命名空间
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gbyibfepv.sHtML

namespace App\Http;
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gqwljwzll.sHtML

[U44] PHP：开启严格类型
来源：http://mobile.fanxiaobao.xyz/Article/details/gpyqfatlw.sHtML

declare(strict_types=1);
来源：http://www.blog.fanxiaobao.xyz/Article/details/gdrtyaaie.sHtML

[U45] PHP：类型声明与返回类型
来源：http://wap.fanxiaobao.xyz/Article/details/giuytpbwp.sHtML

function add(int $a, int $b): int { return $a + $b; }
来源：http://mobile.fanxiaobao.xyz/Article/details/gvdfyrrqj.sHtML

[U46] PHP：可空类型
来源：http://mobile.fanxiaobao.xyz/Article/details/gdbsltrqx.sHtML

?string $name = null
来源：http://mobile.fanxiaobao.xyz/Article/details/gnzumymut.sHtML

[U47] PHP：联合类型
来源：http://blog.fanxiaobao.xyz/Article/details/gmcgbphik.sHtML

int|string $id
来源：http://www.share.fanxiaobao.xyz/Article/details/gddcbowjf.sHtML

[U48] PHP：纯枚举
来源：http://www.blog.fanxiaobao.xyz/Article/details/gzywiwbfj.sHtML

enum Status: string { case Active = "active"; case Off = "off"; }
来源：http://3g.fanxiaobao.xyz/Article/details/gugyxfngh.sHtML

[U49] PHP：只读属性
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gcskyhhbt.sHtML

public readonly string $name
来源：http://wap.fanxiaobao.xyz/Article/details/gtjexhfvf.sHtML

[U50] PHP：构造器属性提升
来源：http://3g.fanxiaobao.xyz/Article/details/gwwvwsxua.sHtML

public function __construct(private int $id) {}
来源：http://3g.fanxiaobao.xyz/Article/details/gqobvbgnz.sHtML

[U51] PHP：数组解构
来源：http://3g.fanxiaobao.xyz/Article/details/gomfwwucc.sHtML

[$a, $b] = $arr;
来源：http://www.blog.fanxiaobao.xyz/Article/details/gfcykspvn.sHtML

[U52] PHP：箭头函数
来源：http://blog.fanxiaobao.xyz/Article/details/gfnosfbbn.sHtML

$double = fn($x) => $x * 2;
来源：http://read.share.fanxiaobao.xyz/Article/details/gsytakkec.sHtML

[U53] PHP：空合并运算符
来源：http://www.share.fanxiaobao.xyz/Article/details/gamybtspk.sHtML

$v = $a ?? $b ?? "default";
来源：http://read.share.fanxiaobao.xyz/Article/details/gcptyqomo.sHtML

[U54] PHP：空安全调用
来源：http://3g.fanxiaobao.xyz/Article/details/gtlxxsfwo.sHtML

$obj?->method()
来源：http://wap.fanxiaobao.xyz/Article/details/gvopqupgx.sHtML

[U55] PHP：match 表达式
来源：http://mobile.fanxiaobao.xyz/Article/details/grjluetxx.sHtML

$s = match($x) { 1 => "一", default => "其他" };
来源：http://www.blog.fanxiaobao.xyz/Article/details/gittlebgj.sHtML

[U56] PHP：命名参数
来源：http://read.share.fanxiaobao.xyz/Article/details/gtvalepzm.sHtML

f(a: 1, b: 2)
来源：http://mobile.fanxiaobao.xyz/Article/details/gwtpiqane.sHtML

[U57] PHP：字符串插值
来源：http://3g.fanxiaobao.xyz/Article/details/gpnumxjsn.sHtML

"值: {$a}"
来源：http://wap.fanxiaobao.xyz/Article/details/gpjucsghs.sHtML

[U58] PHP：数组三件套
来源：http://www.blog.fanxiaobao.xyz/Article/details/gaixxfsly.sHtML

array_map($f, $a);  array_filter($a, $f);  array_reduce($a, $f, 0);
来源：http://baike.fanxiaobao.xyz/Article/details/gsaalvcri.sHtML

[U59] PHP：自定义排序
来源：http://www.share.fanxiaobao.xyz/Article/details/gjyfmzkmb.sHtML

usort($arr, fn($a, $b) => $a["age"] <=> $b["age"]);
来源：http://3g.fanxiaobao.xyz/Article/details/gnhqnvaxr.sHtML

[U60] PHP：JSON 编解码
来源：http://www.blog.fanxiaobao.xyz/Article/details/gryniaruv.sHtML

json_encode($d, JSON_UNESCAPED_UNICODE);  json_decode($s, true);
来源：http://baike.fanxiaobao.xyz/Article/details/ghtnyszng.sHtML

[U61] PHP：正则
来源：http://m.share.fanxiaobao.xyz/Article/details/gmgmgalcz.sHtML

preg_match('/(\d+)/', $s, $m);  preg_replace('/\d+/', '#', $s);
来源：http://wap.fanxiaobao.xyz/Article/details/gjkbgdefc.sHtML

[U62] PHP：日期对象
来源：http://blog.fanxiaobao.xyz/Article/details/grqjhegwk.sHtML

(new DateTimeImmutable())->format("Y-m-d");
来源：http://baike.fanxiaobao.xyz/Article/details/gcmtyvtiv.sHtML

[U63] PHP：文件读写
来源：http://www.blog.fanxiaobao.xyz/Article/details/gjxkgjniq.sHtML

file_get_contents($f);  file_put_contents($f, $data);
来源：http://baike.fanxiaobao.xyz/Article/details/gwtzzoleb.sHtML

[U64] PHP：目录遍历
来源：http://www.m.share.fanxiaobao.xyz/Article/details/giskpfufg.sHtML

glob("dir/*.php");  scandir("dir");
来源：http://wap.fanxiaobao.xyz/Article/details/gwvqjdnju.sHtML

[U65] PHP：会话
来源：http://baike.fanxiaobao.xyz/Article/details/gtezrchxx.sHtML

session_start();  $_SESSION["uid"] = 1;
来源：http://wap.fanxiaobao.xyz/Article/details/gfxfyfjsx.sHtML

[U66] PHP：设置 Cookie
来源：http://www.blog.fanxiaobao.xyz/Article/details/ghqpglhxc.sHtML

setcookie("token", $v, ["httponly" => true, "samesite" => "Lax"]);
来源：http://www.share.fanxiaobao.xyz/Article/details/gfeibwtqw.sHtML

[U67] PHP：处理文件上传
来源：http://read.share.fanxiaobao.xyz/Article/details/gqrslitrn.sHtML

$_FILES["file"]["tmp_name"] 与 move_uploaded_file()
来源：http://www.share.fanxiaobao.xyz/Article/details/gqbrotshk.sHtML

[U68] PHP：PDO 连接
来源：http://mobile.fanxiaobao.xyz/Article/details/glkvccnub.sHtML

$pdo = new PDO("mysql:host=localhost;dbname=app", "root", "");
来源：http://mobile.fanxiaobao.xyz/Article/details/gewpdhrin.sHtML

[U69] PHP：PDO 预处理
来源：http://www.share.fanxiaobao.xyz/Article/details/gjbuunlre.sHtML

$stmt = $pdo->prepare("SELECT * FROM users WHERE id = ?");  $stmt->execute([$id]);
来源：http://wap.fanxiaobao.xyz/Article/details/grymbkswv.sHtML

[U70] PHP：PDO 事务
来源：http://read.share.fanxiaobao.xyz/Article/details/gcnkpvwur.sHtML

$pdo->beginTransaction();  $pdo->commit();  $pdo->rollBack();
来源：http://www.share.fanxiaobao.xyz/Article/details/glolmrktr.sHtML

[U71] PHP：抛出异常
来源：http://read.share.fanxiaobao.xyz/Article/details/gsulslslq.sHtML

throw new RuntimeException("失败", 500);
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gaxwrpgga.sHtML

[U72] PHP：写错误日志
来源：http://www.share.fanxiaobao.xyz/Article/details/gbgnflyxb.sHtML

error_log("失败: " . $e->getMessage());
来源：http://3g.fanxiaobao.xyz/Article/details/gnncqsmmd.sHtML

[U73] PHP：读取 ini 配置
来源：http://read.share.fanxiaobao.xyz/Article/details/gjfjyyhhc.sHtML

parse_ini_file("config.ini", true)
来源：http://www.blog.fanxiaobao.xyz/Article/details/gjsbeqvwf.sHtML

[U74] PHP：读取环境变量
来源：http://www.blog.fanxiaobao.xyz/Article/details/gctrztors.sHtML

getenv("APP_ENV") ?: "production"
来源：http://wap.fanxiaobao.xyz/Article/details/ghiegsacg.sHtML

[U75] PHP：依赖注入
来源：http://m.share.fanxiaobao.xyz/Article/details/gzqjjxkhn.sHtML

composer require psr/container
来源：http://m.share.fanxiaobao.xyz/Article/details/geqwhjpui.sHtML

[U76] PHP：简单路由
来源：http://baike.fanxiaobao.xyz/Article/details/gzzgmgzdc.sHtML

$path = parse_url($_SERVER["REQUEST_URI"], PHP_URL_PATH);
来源：http://3g.fanxiaobao.xyz/Article/details/gmljlsmxf.sHtML

[U77] PHP：模板渲染
来源：http://baike.fanxiaobao.xyz/Article/details/gswmevimq.sHtML

composer require twig/twig
来源：http://www.blog.fanxiaobao.xyz/Article/details/gqiikhtlq.sHtML

[U78] PHP：单元测试
来源：http://read.share.fanxiaobao.xyz/Article/details/gmedkbnwj.sHtML

composer require --dev phpunit/phpunit
来源：http://read.share.fanxiaobao.xyz/Article/details/gnyqryfwb.sHtML

[U79] PHP：静态分析
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gzddtfqyc.sHtML

composer require --dev phpstan/phpstan
来源：http://mobile.fanxiaobao.xyz/Article/details/gjlttqhcb.sHtML

[U80] PHP：代码规范修复
来源：http://m.share.fanxiaobao.xyz/Article/details/gddwzjkhj.sHtML

composer require --dev friendsofphp/php-cs-fixer
来源：http://www.m.share.fanxiaobao.xyz/Article/details/grwfuwjqc.sHtML

[U81] JS：初始化项目
来源：http://mobile.fanxiaobao.xyz/Article/details/gruapuflr.sHtML

npm init -y;  npm i express
来源：http://www.share.fanxiaobao.xyz/Article/details/gczmwdodr.sHtML

[U82] JS：package.json 脚本
来源：http://wap.fanxiaobao.xyz/Article/details/ghepgihbg.sHtML

"scripts": { "dev": "vite", "build": "vite build" }
来源：http://blog.fanxiaobao.xyz/Article/details/gsullmbzq.sHtML

[U83] JS：ES Module 导入导出
来源：http://www.share.fanxiaobao.xyz/Article/details/gmsadnfxx.sHtML

export const a = 1;  import { a } from "./m.js";
来源：http://blog.fanxiaobao.xyz/Article/details/gbelznsdd.sHtML

[U84] JS：CommonJS 写法
来源：http://www.blog.fanxiaobao.xyz/Article/details/gsmylkedk.sHtML

module.exports = { a };  const { a } = require("./m");
来源：http://m.share.fanxiaobao.xyz/Article/details/gyayxydjs.sHtML

[U85] JS：可选链
来源：http://baike.fanxiaobao.xyz/Article/details/gvvolbhgd.sHtML

a?.b?.c
来源：http://blog.fanxiaobao.xyz/Article/details/gchvxmwqh.sHtML

[U86] JS：空值合并
来源：http://3g.fanxiaobao.xyz/Article/details/gxamqdssw.sHtML

a ?? b
来源：http://mobile.fanxiaobao.xyz/Article/details/glicwdkyn.sHtML

[U87] JS：解构默认值
来源：http://mobile.fanxiaobao.xyz/Article/details/ghpoqqkil.sHtML

const { a = 1, b = 2 } = obj;
来源：http://3g.fanxiaobao.xyz/Article/details/ggsijdmva.sHtML

[U88] JS：对象展开合并
来源：http://baike.fanxiaobao.xyz/Article/details/gwnrdgjig.sHtML

{ ...a, ...b }
来源：http://www.m.share.fanxiaobao.xyz/Article/details/glyzykccq.sHtML

[U89] JS：数组去重
来源：http://m.share.fanxiaobao.xyz/Article/details/gpbxdgcip.sHtML

[...new Set(arr)]
来源：http://www.blog.fanxiaobao.xyz/Article/details/gsrcexjbk.sHtML

[U90] JS：数字数组排序
来源：http://baike.fanxiaobao.xyz/Article/details/gxunybdls.sHtML

[...arr].sort((a, b) => a - b)
来源：http://3g.fanxiaobao.xyz/Article/details/gjcfsdgdy.sHtML

[U91] JS：对象键值遍历
来源：http://baike.fanxiaobao.xyz/Article/details/grtaqbewy.sHtML

Object.entries(obj).forEach(([k, v]) => {});
来源：http://read.share.fanxiaobao.xyz/Article/details/ghjlndvmq.sHtML

[U92] JS：深拷贝
来源：http://www.share.fanxiaobao.xyz/Article/details/gbcngwfnj.sHtML

structuredClone(obj)
来源：http://baike.fanxiaobao.xyz/Article/details/gokqzgfuc.sHtML

[U93] JS：模板字符串
来源：http://www.share.fanxiaobao.xyz/Article/details/gckipbtvy.sHtML

`共 ${n} 条`
来源：http://wap.fanxiaobao.xyz/Article/details/gblwpssjf.sHtML

[U94] JS：箭头函数
来源：http://www.blog.fanxiaobao.xyz/Article/details/gfpeculpv.sHtML

const double = x => x * 2;
来源：http://mobile.fanxiaobao.xyz/Article/details/gbniwucoa.sHtML

[U95] JS：Promise 包装
来源：http://blog.fanxiaobao.xyz/Article/details/gbubqsqlq.sHtML

new Promise((resolve, reject) => {})
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gpcxvljyz.sHtML

[U96] JS：async/await 与异常
来源：http://baike.fanxiaobao.xyz/Article/details/gpdgazzaz.sHtML

try { const d = await f(); } catch (e) { console.error(e); }
来源：http://www.blog.fanxiaobao.xyz/Article/details/glvhmstwz.sHtML

[U97] JS：并发请求
来源：http://www.share.fanxiaobao.xyz/Article/details/ggcdssnrd.sHtML

await Promise.all(urls.map(u => fetch(u)))
来源：http://www.share.fanxiaobao.xyz/Article/details/gitpbeorg.sHtML

[U98] JS：fetch 带 JSON
来源：http://wap.fanxiaobao.xyz/Article/details/gnmvfyilo.sHtML

await fetch(url, { method: "POST", headers: { "Content-Type": "application/json" }, body: JSON.stringify(d) })
来源：http://www.blog.fanxiaobao.xyz/Article/details/geleiccpu.sHtML

[U99] JS：事件监听
来源：http://m.share.fanxiaobao.xyz/Article/details/gbzeiscfs.sHtML

el.addEventListener("click", e => {})
来源：http://baike.fanxiaobao.xyz/Article/details/gevxdzgcp.sHtML

[U100] JS：DOM 查询
来源：http://wap.fanxiaobao.xyz/Article/details/grswjawpu.sHtML

document.querySelector(".item")
来源：http://www.blog.fanxiaobao.xyz/Article/details/gsmfddyku.sHtML

[U101] JS：classList 操作
来源：http://3g.fanxiaobao.xyz/Article/details/glhulzlbo.sHtML

el.classList.toggle("active")
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gzwldkevb.sHtML

[U102] JS：本地存储
来源：http://read.share.fanxiaobao.xyz/Article/details/gazqmxjei.sHtML

localStorage.setItem("k", JSON.stringify(v))
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gsozknvnn.sHtML

[U103] JS：定时器
来源：http://wap.fanxiaobao.xyz/Article/details/gxmwwxoue.sHtML

setTimeout(fn, 1000);  setInterval(fn, 1000);
来源：http://mobile.fanxiaobao.xyz/Article/details/ghnlardnr.sHtML

[U104] JS：防抖
来源：http://mobile.fanxiaobao.xyz/Article/details/gyzqydazq.sHtML

const debounce = (fn, ms) => { let t; return (...a) => { clearTimeout(t); t = setTimeout(() => fn(...a), ms); }; };
来源：http://3g.fanxiaobao.xyz/Article/details/gngwhhsur.sHtML

[U105] JS：节流
来源：http://wap.fanxiaobao.xyz/Article/details/gjdbwmlkv.sHtML

const throttle = (fn, ms) => { let last = 0; return (...a) => { const n = Date.now(); if (n - last >= ms) { last = n; fn(...a); } }; };
来源：http://wap.fanxiaobao.xyz/Article/details/gwijsfdlo.sHtML

[U106] JS：日期格式化
来源：http://www.share.fanxiaobao.xyz/Article/details/ghnvfeplh.sHtML

new Intl.DateTimeFormat("zh-CN", { dateStyle: "medium" }).format(new Date())
来源：http://read.share.fanxiaobao.xyz/Article/details/gcjezjnob.sHtML

[U107] JS：数字千分位
来源：http://wap.fanxiaobao.xyz/Article/details/gtdemiqqp.sHtML

new Intl.NumberFormat("en-US").format(1234567)
来源：http://blog.fanxiaobao.xyz/Article/details/giwyyolen.sHtML

[U108] JS：随机整数
来源：http://3g.fanxiaobao.xyz/Article/details/guvxiasdk.sHtML

Math.floor(Math.random() * (max - min + 1)) + min
来源：http://www.share.fanxiaobao.xyz/Article/details/gdpmpvaxd.sHtML

[U109] JS：数组分组
来源：http://baike.fanxiaobao.xyz/Article/details/gmvdmzqim.sHtML

Object.groupBy(arr, x => x.type)
来源：http://www.blog.fanxiaobao.xyz/Article/details/gkitkgxwd.sHtML

[U110] JS：数组分块
来源：http://wap.fanxiaobao.xyz/Article/details/gkyhksqqs.sHtML

arr.reduce((acc, x, i) => (i % size ? acc : [...acc, arr.slice(i, i + size)]), [])
来源：http://blog.fanxiaobao.xyz/Article/details/gojyqojur.sHtML

[U111] JS：对象转 Map
来源：http://m.share.fanxiaobao.xyz/Article/details/guhppjwsm.sHtML

new Map(Object.entries(obj))
来源：http://baike.fanxiaobao.xyz/Article/details/gmyavjjcy.sHtML

[U112] JS：字符串补位
来源：http://3g.fanxiaobao.xyz/Article/details/glaibggwv.sHtML

"7".padStart(3, "0")
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gyifcanrh.sHtML

[U113] JS：正则替换全部
来源：http://m.share.fanxiaobao.xyz/Article/details/glftphrnu.sHtML

s.replaceAll("a", "b")
来源：http://read.share.fanxiaobao.xyz/Article/details/gagiwhjff.sHtML

[U114] JS：JSON 深比较
来源：http://blog.fanxiaobao.xyz/Article/details/gfrrgqzuv.sHtML

JSON.stringify(a) === JSON.stringify(b)
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gvyuovjhm.sHtML

[U115] JS：生成 UUID
来源：http://blog.fanxiaobao.xyz/Article/details/gaqqrqeot.sHtML

crypto.randomUUID()
来源：http://read.share.fanxiaobao.xyz/Article/details/gzhceopkz.sHtML

[U116] JS：类型检查（JSDoc）
来源：http://read.share.fanxiaobao.xyz/Article/details/gwxrqukci.sHtML

/** @param {string} name */ function f(name) {}
来源：http://3g.fanxiaobao.xyz/Article/details/gljgkdmpr.sHtML

[U117] JS：单元测试
来源：http://m.share.fanxiaobao.xyz/Article/details/gtfsebxbh.sHtML

npm i -D vitest;  npx vitest
来源：http://baike.fanxiaobao.xyz/Article/details/gxeyjhmnv.sHtML

[U118] JS：开发服务器
来源：http://baike.fanxiaobao.xyz/Article/details/gtjtvtcxx.sHtML

npm i -D vite;  npx vite
来源：http://www.blog.fanxiaobao.xyz/Article/details/gecollubt.sHtML

[U119] JS：生产构建
来源：http://www.blog.fanxiaobao.xyz/Article/details/gfxqobnro.sHtML

npx vite build
来源：http://www.blog.fanxiaobao.xyz/Article/details/gbmnygezj.sHtML

[U120] JS：读取环境变量（Vite）
来源：http://www.blog.fanxiaobao.xyz/Article/details/gxnhiojpo.sHtML

import.meta.env.VITE_API_URL
来源：http://baike.fanxiaobao.xyz/Article/details/ggaifzvcm.sHtML

================================================================================
来源：http://3g.fanxiaobao.xyz/Article/details/giqpmxzrt.sHtML

统计汇总
来源：http://www.blog.fanxiaobao.xyz/Article/details/gvqbmjlhs.sHtML

================================================================================
来源：http://read.share.fanxiaobao.xyz/Article/details/gtfyzkxts.sHtML

按语言统计（条）：
来源：http://wap.fanxiaobao.xyz/Article/details/glcoayxgy.sHtML

Python ......... 252
来源：http://blog.fanxiaobao.xyz/Article/details/gigycvyzl.sHtML

PHP ............ 252
来源：http://m.share.fanxiaobao.xyz/Article/details/gomskenkq.sHtML

JavaScript ..... 252
来源：http://3g.fanxiaobao.xyz/Article/details/godiscnyt.sHtML

TypeScript ..... 212
来源：http://m.share.fanxiaobao.xyz/Article/details/gjczufsgp.sHtML

Java ........... 212
来源：http://read.share.fanxiaobao.xyz/Article/details/gkszyvuln.sHtML

Go ............. 212
来源：http://blog.fanxiaobao.xyz/Article/details/gaghmwtim.sHtML

Ruby ........... 212
来源：http://www.share.fanxiaobao.xyz/Article/details/gjycshuod.sHtML

C# ............. 212
来源：http://blog.fanxiaobao.xyz/Article/details/gwuqzctwd.sHtML

C .............. 30
来源：http://wap.fanxiaobao.xyz/Article/details/gcpffstyf.sHtML

C++ ............ 30
来源：http://mobile.fanxiaobao.xyz/Article/details/gxizqfoqh.sHtML

SQL ............ 90
来源：http://www.blog.fanxiaobao.xyz/Article/details/gzqjdproo.sHtML

Bash ........... 80
来源：http://3g.fanxiaobao.xyz/Article/details/gurrkshqd.sHtML

Kotlin ......... 15
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gdpooyuxn.sHtML

Swift .......... 15
来源：http://3g.fanxiaobao.xyz/Article/details/gkjtlhrri.sHtML

Lua ............ 10
来源：http://m.share.fanxiaobao.xyz/Article/details/glgzjfyiz.sHtML

Perl ........... 10
来源：http://mobile.fanxiaobao.xyz/Article/details/grhtjuqzh.sHtML

Scala .......... 10
来源：http://www.blog.fanxiaobao.xyz/Article/details/goognieny.sHtML

------------------------------------
来源：http://m.share.fanxiaobao.xyz/Article/details/gyhpqdpoi.sHtML

合计 ........... 2106 条
来源：http://read.share.fanxiaobao.xyz/Article/details/gaehwalyf.sHtML

按章节统计：
来源：http://baike.fanxiaobao.xyz/Article/details/gzpqqkblq.sHtML

A 基础语法与类型       26 个任务 × 8 语言 =  208
来源：http://mobile.fanxiaobao.xyz/Article/details/ghciyamzr.sHtML

B 流程控制             16 个任务 × 8 语言 =  128
来源：http://m.share.fanxiaobao.xyz/Article/details/gqkalvmom.sHtML

C 函数与作用域         16 个任务 × 8 语言 =  128
来源：http://www.share.fanxiaobao.xyz/Article/details/gifvuenon.sHtML

D 数组 / 列表 / 集合   26 个任务 × 8 语言 =  208
来源：http://www.m.share.fanxiaobao.xyz/Article/details/glfgrhqel.sHtML

E 字符串处理           22 个任务 × 8 语言 =  176
来源：http://read.share.fanxiaobao.xyz/Article/details/gmwxpqncf.sHtML

F 文件与目录           12 个任务 × 8 语言 =   96
来源：http://baike.fanxiaobao.xyz/Article/details/geygtinsd.sHtML

G 面向对象             16 个任务 × 8 语言 =  128
来源：http://read.share.fanxiaobao.xyz/Article/details/gafdfpaih.sHtML

H 异常与错误处理       10 个任务 × 8 语言 =   80
来源：http://m.share.fanxiaobao.xyz/Article/details/grkzsmogn.sHtML

I 正则表达式            8 个任务 × 8 语言 =   64
来源：http://www.blog.fanxiaobao.xyz/Article/details/gckoxsvwk.sHtML

J 日期与时间           10 个任务 × 8 语言 =   80
来源：http://read.share.fanxiaobao.xyz/Article/details/gtptemhbf.sHtML

K JSON 与序列化         8 个任务 × 8 语言 =   64
来源：http://www.blog.fanxiaobao.xyz/Article/details/gleatoldu.sHtML

L 网络请求              8 个任务 × 8 语言 =   64
来源：http://baike.fanxiaobao.xyz/Article/details/gskanajtf.sHtML

M 命令行 / 进程         8 个任务 × 8 语言 =   64
来源：http://www.blog.fanxiaobao.xyz/Article/details/gyenvdbsa.sHtML

N 数据结构与算法       12 个任务 × 8 语言 =   96
来源：http://m.share.fanxiaobao.xyz/Article/details/gtohrfovx.sHtML

O 并发与异步            6 个任务 × 8 语言 =   48
来源：http://baike.fanxiaobao.xyz/Article/details/gzokyvncx.sHtML

P 常用工具函数          8 个任务 × 8 语言 =   64
来源：http://m.share.fanxiaobao.xyz/Article/details/gzcxxcyqa.sHtML

Q SQL 专题                              90
来源：http://blog.fanxiaobao.xyz/Article/details/gixwacpje.sHtML

R Bash 专题                             80
来源：http://wap.fanxiaobao.xyz/Article/details/gzcpyjyuy.sHtML

S C / C++ 专题                          60
来源：http://www.share.fanxiaobao.xyz/Article/details/gjmdpzjxt.sHtML

T 其他语言补充                          60
来源：http://wap.fanxiaobao.xyz/Article/details/gcvintxtc.sHtML

U 高频实用片段                         120
来源：http://wap.fanxiaobao.xyz/Article/details/glahpkwke.sHtML

------------------------------------
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gnmegzxzx.sHtML

合计                                  2106 条
来源：http://wap.fanxiaobao.xyz/Article/details/gabmynvpf.sHtML

--------------------------------------------------------------------------------
来源：http://blog.fanxiaobao.xyz/Article/details/gczlfuxnx.sHtML

使用提醒
来源：http://mobile.fanxiaobao.xyz/Article/details/gnizydkzz.sHtML

--------------------------------------------------------------------------------
来源：http://wap.fanxiaobao.xyz/Article/details/gdtqgcwrn.sHtML

1. 示例追求"最小可用"，正式项目中请补齐导入、错误处理与边界判断。
来源：http://wap.fanxiaobao.xyz/Article/details/ghlceyfyq.sHtML

2. 涉及文件、网络、数据库的示例，注意资源释放与异常捕获。
来源：http://baike.fanxiaobao.xyz/Article/details/gqdmtvkhx.sHtML

3. 语言版本差异较大（如 Python 3.10 的 match、Java 17 的 record/switch 箭头），
来源：http://3g.fanxiaobao.xyz/Article/details/gmxqcddhk.sHtML

在旧版本上使用前请先确认语法支持情况。
来源：http://www.share.fanxiaobao.xyz/Article/details/gqaytqgnl.sHtML

4. 标注"手写"的条目是因为该语言缺少对应内置能力，实际项目中可引入成熟库。
来源：http://blog.fanxiaobao.xyz/Article/details/gsalhhjlq.sHtML

—— 文件结束 ——
来源：http://www.blog.fanxiaobao.xyz/Article/details/gvclshlhq.sHtML

================================================================================
来源：http://m.share.fanxiaobao.xyz/Article/details/gbwaykust.sHtML

程序语言常见例子速查手册（2024 版）
来源：http://mobile.fanxiaobao.xyz/Article/details/gdthksden.sHtML

Common Programming Examples Cheat Book
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gbzunyouj.sHtML

================================================================================
来源：http://blog.fanxiaobao.xyz/Article/details/gymzodbqc.sHtML

【收录内容】
来源：http://www.share.fanxiaobao.xyz/Article/details/giiywplju.sHtML

覆盖 12 种语言 / 语法与常见 API：
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gttpxmuox.sHtML

Python · PHP · JavaScript · TypeScript · Java · Go · Ruby · C#
来源：http://www.share.fanxiaobao.xyz/Article/details/gmdhnyvzx.sHtML

SQL · Bash · C · C++
来源：http://www.share.fanxiaobao.xyz/Article/details/gzahqzcrj.sHtML

按「任务」分组：每个任务下按语言各给出一条最小可用示例。
来源：http://blog.fanxiaobao.xyz/Article/details/gxolqqvpp.sHtML

【使用说明】
来源：http://www.share.fanxiaobao.xyz/Article/details/gmozrspsi.sHtML

1. 每个任务形如 "[编号] 任务名"，下面每行以语言标记开头：
来源：http://www.share.fanxiaobao.xyz/Article/details/gggndberb.sHtML

Py:    Python        PHP:   PHP           JS:    JavaScript
来源：http://baike.fanxiaobao.xyz/Article/details/gqaqyyqkt.sHtML

TS:    TypeScript    Java:  Java          Go:    Go
来源：http://m.share.fanxiaobao.xyz/Article/details/gjkxgpykw.sHtML

Ruby:  Ruby          C#:    C#            SQL:   SQL
来源：http://m.share.fanxiaobao.xyz/Article/details/gapxxxdsv.sHtML

Bash:  Shell         C:     C             C++:   C++
来源：http://www.share.fanxiaobao.xyz/Article/details/ghiopthfo.sHtML

2. 示例只展示核心写法，刻意省略 import / require / include / using 等样板代码。
来源：http://3g.fanxiaobao.xyz/Article/details/gvczjknbu.sHtML

需要完整可运行文件时，请自行补齐当前语言的导入语句。
来源：http://blog.fanxiaobao.xyz/Article/details/gvhkwiycf.sHtML

3. 语法基准：Python 3.10+ / PHP 8.1+ / ES2020+ / TypeScript 5 / Java 17 /
来源：http://www.share.fanxiaobao.xyz/Article/details/glshhyfol.sHtML

Go 1.21+ / Ruby 3.x / C# 10+ / C17 / C++17。
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gnvabtkwg.sHtML

4. 检索建议：用编辑器或浏览器 Ctrl+F 搜关键词，如 "排序" "读取文件" "正则"。
来源：http://www.blog.fanxiaobao.xyz/Article/details/gmdcwpxfe.sHtML

5. 标记为 "// 无" 表示该语言没有对应的一等语法，需用替代写法（示例给出替代方案）。
来源：http://www.share.fanxiaobao.xyz/Article/details/gtrkzakwt.sHtML

6. 符号 "⏎" 表示代码在此处换行（主要用于 Python 等强制缩进、无法压成一行的结构）。
来源：http://baike.fanxiaobao.xyz/Article/details/godlftqpc.sHtML

【文件统计】
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gofbjirku.sHtML

语言示例共 2106 条，分布见本文末尾的「统计汇总」。
来源：http://www.share.fanxiaobao.xyz/Article/details/gwsqgiugi.sHtML

--------------------------------------------------------------------------------
来源：http://www.share.fanxiaobao.xyz/Article/details/grwjwpswc.sHtML

目  录
来源：http://3g.fanxiaobao.xyz/Article/details/gjiqajoll.sHtML

--------------------------------------------------------------------------------
来源：http://www.m.share.fanxiaobao.xyz/Article/details/ggcclarln.sHtML

A. 基础语法与类型              （第 1 节，26 个任务，208 条）
来源：http://mobile.fanxiaobao.xyz/Article/details/ghjomrqqm.sHtML

B. 流程控制                    （第 2 节，16 个任务，128 条）
来源：http://www.blog.fanxiaobao.xyz/Article/details/gbsvozwkt.sHtML

C. 函数与作用域                （第 3 节，16 个任务，128 条）
来源：http://baike.fanxiaobao.xyz/Article/details/grfmfhjkl.sHtML

D. 数组 / 列表 / 集合          （第 4 节，26 个任务，208 条）
来源：http://blog.fanxiaobao.xyz/Article/details/glnfggncv.sHtML

E. 字符串处理                  （第 5 节，22 个任务，176 条）
来源：http://mobile.fanxiaobao.xyz/Article/details/gfqoigzwl.sHtML

F. 文件与目录                  （第 6 节，12 个任务，96 条）
来源：http://m.share.fanxiaobao.xyz/Article/details/gbgyvcnpg.sHtML

G. 面向对象                    （第 7 节，16 个任务，128 条）
来源：http://www.share.fanxiaobao.xyz/Article/details/geuhqquqs.sHtML

H. 异常与错误处理              （第 8 节，10 个任务，80 条）
来源：http://mobile.fanxiaobao.xyz/Article/details/gpymynlnc.sHtML

I. 正则表达式                  （第 9 节，8 个任务，64 条）
来源：http://3g.fanxiaobao.xyz/Article/details/gphnlclqp.sHtML


<!-- 参考信息 -->