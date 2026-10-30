代发 wailian999

[U13] Py：固定长度队列
来源：http://mobile.fehbvm.com/Article/details/gmahbeyvy.sHtML

deque(maxlen=10)
来源：http://www.blog.fehbvm.com/Article/details/gkkwcgvgv.sHtML

[U14] Py：分组收集到列表
来源：http://blog.fehbvm.com/Article/details/gbvwekslp.sHtML

defaultdict(list)
来源：http://m.share.zdbjq.cn/Article/details/gkvycjvfn.sHtML

[U15] Py：高精度计时
来源：http://www.m.share.fehbvm.com/Article/details/gjfhjckiz.sHtML

t = time.perf_counter()
来源：http://m.share.fehbvm.com/Article/details/gqfskkipn.sHtML

[U16] Py：命令行参数解析
来源：http://baike.fehbvm.com/Article/details/grmqfsole.sHtML

ap = argparse.ArgumentParser();  ap.add_argument("--name");  args = ap.parse_args()
来源：http://baike.fehbvm.com/Article/details/gtcvbmzck.sHtML

[U17] Py：初始化日志
来源：http://baike.fehbvm.com/Article/details/geuetzoga.sHtML

logging.basicConfig(level=logging.INFO)
来源：http://wap.hesvh.cn/Article/details/gxoqjfxat.sHtML

[U18] Py：预编译正则
来源：http://mobile.hesvh.cn/Article/details/gtqxezwww.sHtML

pat = re.compile(r"\d+")
来源：http://mobile.zdbjq.cn/Article/details/gdymenffq.sHtML

[U19] Py：正则替换带回调
来源：http://www.m.share.fehbvm.com/Article/details/gntlqkmmf.sHtML

re.sub(r"\d+", lambda m: str(int(m.group()) * 2), s)
来源：http://3g.hesvh.cn/Article/details/gowenovlf.sHtML

[U20] Py：缓存函数结果
来源：http://baike.hesvh.cn/Article/details/gfjsanshe.sHtML

@functools.lru_cache(maxsize=None)
来源：http://blog.zdbjq.cn/Article/details/gqgafdbfu.sHtML

[U21] Py：自定义上下文管理器
来源：http://www.share.hesvh.cn/Article/details/gijdwfgkl.sHtML

@contextlib.contextmanager
来源：http://blog.zdbjq.cn/Article/details/gdlnksnpp.sHtML

[U22] Py：矩阵转置
来源：http://baike.fehbvm.com/Article/details/gixoyerbn.sHtML

list(zip(*m))
来源：http://wap.zdbjq.cn/Article/details/geirmvflk.sHtML

[U23] Py：分块读取大文件
来源：http://www.blog.zdbjq.cn/Article/details/glknkjzdm.sHtML

for chunk in iter(lambda: f.read(8192), b""):
来源：http://wap.zdbjq.cn/Article/details/gvrvqripd.sHtML

[U24] Py：路径操作
来源：http://wap.hesvh.cn/Article/details/ggrymttts.sHtML

Path("a/b.txt").parent.mkdir(parents=True, exist_ok=True)
来源：http://m.share.hesvh.cn/Article/details/gugqtpjzi.sHtML

[U25] Py：CSV 按字典读
来源：http://www.share.hesvh.cn/Article/details/gshwabaww.sHtML

csv.DictReader(f)
来源：http://www.share.fehbvm.com/Article/details/gamflpmuk.sHtML

[U26] Py：并发下载
来源：http://wap.hesvh.cn/Article/details/gtwfnebae.sHtML

ThreadPoolExecutor(max_workers=8).map(fetch, urls)
来源：http://wap.zdbjq.cn/Article/details/gtftdfyyo.sHtML

[U27] Py：异步 HTTP
来源：http://www.m.share.fehbvm.com/Article/details/gyeoluozf.sHtML

aiohttp.ClientSession() 配合 async with
来源：http://www.m.share.fehbvm.com/Article/details/gtyaiqblw.sHtML

[U28] Py：类型别名
来源：http://www.blog.fehbvm.com/Article/details/gyzfkrabt.sHtML

UserId = int
来源：http://m.share.zdbjq.cn/Article/details/gxdfajsmd.sHtML

[U29] Py：属性校验
来源：http://blog.hesvh.cn/Article/details/gbbfrmclb.sHtML

@property 与 @x.setter 配合
来源：http://baike.hesvh.cn/Article/details/gmvseafsz.sHtML

[U30] Py：数据类
来源：http://3g.fehbvm.com/Article/details/gwtdfvdty.sHtML

@dataclass(slots=True)
来源：http://baike.hesvh.cn/Article/details/gjatavosp.sHtML

[U31] Py：单测
来源：http://www.share.fehbvm.com/Article/details/gpgrdmwhd.sHtML

python -m pytest -q
来源：http://read.share.hesvh.cn/Article/details/gjhlgogae.sHtML

[U32] Py：代码格式化
来源：http://m.share.zdbjq.cn/Article/details/glrxpnusd.sHtML

ruff format . && ruff check --fix .
来源：http://m.share.zdbjq.cn/Article/details/gykkwqgdj.sHtML

[U33] Py：打包发布
来源：http://m.share.hesvh.cn/Article/details/gylqsvwsh.sHtML

python -m build  （依赖 pyproject.toml）
来源：http://baike.fehbvm.com/Article/details/gqtmwitgl.sHtML

[U34] Py：判断编码
来源：http://www.blog.fehbvm.com/Article/details/gukxztnav.sHtML

chardet.detect(raw)
来源：http://3g.fehbvm.com/Article/details/gnismmyxd.sHtML

[U35] Py：发送邮件
来源：http://mobile.zdbjq.cn/Article/details/glphfulgz.sHtML

smtplib.SMTP_SSL(...).send_message(msg)
来源：http://www.share.zdbjq.cn/Article/details/gdxypfoov.sHtML

[U36] Py：定时任务
来源：http://read.share.hesvh.cn/Article/details/gcpvjbtfc.sHtML

schedule.every(10).minutes.do(job)
来源：http://www.share.fehbvm.com/Article/details/gfthqcxdp.sHtML

[U37] Py：读写 Excel
来源：http://www.m.share.zdbjq.cn/Article/details/gxkvuywtr.sHtML

pandas.read_excel / DataFrame.to_excel
来源：http://www.m.share.zdbjq.cn/Article/details/gvxhquirj.sHtML

[U38] Py：获取脚本所在目录
来源：http://m.share.fehbvm.com/Article/details/ggahzoqdv.sHtML

Path(__file__).resolve().parent
来源：http://www.m.share.fehbvm.com/Article/details/gatbjtqsy.sHtML

[U39] Py：判断是否在交互环境
来源：http://www.m.share.hesvh.cn/Article/details/gxteljlil.sHtML

sys.stdout.isatty()
来源：http://3g.fehbvm.com/Article/details/gpbsiudfm.sHtML

[U40] Py：打印到标准错误
来源：http://read.share.fehbvm.com/Article/details/gjuyqeypd.sHtML

print("err", file=sys.stderr)
来源：http://www.blog.zdbjq.cn/Article/details/gzrhpgbsv.sHtML

[U41] PHP：初始化 Composer 项目
来源：http://read.share.zdbjq.cn/Article/details/gigluqxdf.sHtML

composer init;  composer require guzzlehttp/guzzle
来源：http://m.share.fehbvm.com/Article/details/gdcwtwuys.sHtML

[U42] PHP：PSR-4 自动加载
来源：http://baike.fehbvm.com/Article/details/gmfmskcfl.sHtML

"autoload": { "psr-4": { "App\\": "src/" } }
来源：http://read.share.fehbvm.com/Article/details/gwztsgrde.sHtML

[U43] PHP：声明命名空间
来源：http://m.share.fehbvm.com/Article/details/gwyoxzehy.sHtML

namespace App\Http;
来源：http://mobile.zdbjq.cn/Article/details/gokulsoth.sHtML

[U44] PHP：开启严格类型
来源：http://m.share.zdbjq.cn/Article/details/gjebokzfe.sHtML

declare(strict_types=1);
来源：http://read.share.fehbvm.com/Article/details/gpgvaxmtm.sHtML

[U45] PHP：类型声明与返回类型
来源：http://www.blog.hesvh.cn/Article/details/gsumibicx.sHtML

function add(int $a, int $b): int { return $a + $b; }
来源：http://blog.hesvh.cn/Article/details/gqfpbbnvs.sHtML

[U46] PHP：可空类型
来源：http://baike.hesvh.cn/Article/details/gfzywjflv.sHtML

?string $name = null
来源：http://read.share.fehbvm.com/Article/details/gruguqrpe.sHtML

[U47] PHP：联合类型
来源：http://www.share.zdbjq.cn/Article/details/gubtqtkhc.sHtML

int|string $id
来源：http://3g.fehbvm.com/Article/details/gqgwlhzwe.sHtML

[U48] PHP：纯枚举
来源：http://www.share.fehbvm.com/Article/details/gahvbmatb.sHtML

enum Status: string { case Active = "active"; case Off = "off"; }
来源：http://blog.zdbjq.cn/Article/details/gyjuzinqx.sHtML

[U49] PHP：只读属性
来源：http://www.share.zdbjq.cn/Article/details/gfulyewov.sHtML

public readonly string $name
来源：http://baike.fehbvm.com/Article/details/gsoqvhvwi.sHtML

[U50] PHP：构造器属性提升
来源：http://www.blog.zdbjq.cn/Article/details/gwrhojpdl.sHtML

public function __construct(private int $id) {}
来源：http://read.share.zdbjq.cn/Article/details/grfnawviu.sHtML

[U51] PHP：数组解构
来源：http://m.share.hesvh.cn/Article/details/ggcgkpcrh.sHtML

[$a, $b] = $arr;
来源：http://www.m.share.hesvh.cn/Article/details/gpsxbbalh.sHtML

[U52] PHP：箭头函数
来源：http://blog.fehbvm.com/Article/details/gotnmfnwq.sHtML

$double = fn($x) => $x * 2;
来源：http://3g.fehbvm.com/Article/details/gehmnqdrx.sHtML

[U53] PHP：空合并运算符
来源：http://3g.zdbjq.cn/Article/details/gxgwkxovw.sHtML

$v = $a ?? $b ?? "default";
来源：http://read.share.fehbvm.com/Article/details/godawkduv.sHtML

[U54] PHP：空安全调用
来源：http://blog.zdbjq.cn/Article/details/ggpvuvbig.sHtML

$obj?->method()
来源：http://m.share.hesvh.cn/Article/details/gaukaxyqt.sHtML

[U55] PHP：match 表达式
来源：http://mobile.zdbjq.cn/Article/details/gsikxgdxc.sHtML

$s = match($x) { 1 => "一", default => "其他" };
来源：http://www.share.fehbvm.com/Article/details/gsjtuuxkp.sHtML

[U56] PHP：命名参数
来源：http://m.share.zdbjq.cn/Article/details/gkhrnprnb.sHtML

f(a: 1, b: 2)
来源：http://mobile.fehbvm.com/Article/details/gnvbmirli.sHtML

[U57] PHP：字符串插值
来源：http://www.m.share.zdbjq.cn/Article/details/ggoebnzjn.sHtML

"值: {$a}"
来源：http://read.share.hesvh.cn/Article/details/gcaltgjrr.sHtML

[U58] PHP：数组三件套
来源：http://blog.zdbjq.cn/Article/details/goalmnoli.sHtML

array_map($f, $a);  array_filter($a, $f);  array_reduce($a, $f, 0);
来源：http://baike.zdbjq.cn/Article/details/gpyrqhquh.sHtML

[U59] PHP：自定义排序
来源：http://mobile.fehbvm.com/Article/details/ggnzufhea.sHtML

usort($arr, fn($a, $b) => $a["age"] <=> $b["age"]);
来源：http://blog.hesvh.cn/Article/details/gjvlaifah.sHtML

[U60] PHP：JSON 编解码
来源：http://3g.hesvh.cn/Article/details/gbzxrfdxs.sHtML

json_encode($d, JSON_UNESCAPED_UNICODE);  json_decode($s, true);
来源：http://3g.zdbjq.cn/Article/details/gpprijinp.sHtML

[U61] PHP：正则
来源：http://wap.hesvh.cn/Article/details/gcxmsmwdl.sHtML

preg_match('/(\d+)/', $s, $m);  preg_replace('/\d+/', '#', $s);
来源：http://3g.fehbvm.com/Article/details/gnfmtfgws.sHtML

[U62] PHP：日期对象
来源：http://read.share.zdbjq.cn/Article/details/ghmxwrzoz.sHtML

(new DateTimeImmutable())->format("Y-m-d");
来源：http://blog.hesvh.cn/Article/details/gkvxsodkr.sHtML

[U63] PHP：文件读写
来源：http://www.blog.zdbjq.cn/Article/details/gxgfrbhxn.sHtML

file_get_contents($f);  file_put_contents($f, $data);
来源：http://www.share.hesvh.cn/Article/details/giswxmnyy.sHtML

[U64] PHP：目录遍历
来源：http://www.share.zdbjq.cn/Article/details/gbfudsrzf.sHtML

glob("dir/*.php");  scandir("dir");
来源：http://m.share.hesvh.cn/Article/details/gqccppaox.sHtML

[U65] PHP：会话
来源：http://wap.fehbvm.com/Article/details/gqlosukrx.sHtML

session_start();  $_SESSION["uid"] = 1;
来源：http://www.share.fehbvm.com/Article/details/golrwopqo.sHtML

[U66] PHP：设置 Cookie
来源：http://m.share.zdbjq.cn/Article/details/gwmdubqdx.sHtML

setcookie("token", $v, ["httponly" => true, "samesite" => "Lax"]);
来源：http://wap.hesvh.cn/Article/details/gwctrxaqh.sHtML

[U67] PHP：处理文件上传
来源：http://wap.fehbvm.com/Article/details/gljnfbztp.sHtML

$_FILES["file"]["tmp_name"] 与 move_uploaded_file()
来源：http://wap.zdbjq.cn/Article/details/ghgewwasu.sHtML

[U68] PHP：PDO 连接
来源：http://www.m.share.hesvh.cn/Article/details/gbgsipdba.sHtML

$pdo = new PDO("mysql:host=localhost;dbname=app", "root", "");
来源：http://read.share.fehbvm.com/Article/details/gfltvmqob.sHtML

[U69] PHP：PDO 预处理
来源：http://baike.hesvh.cn/Article/details/gbrjbcefg.sHtML

$stmt = $pdo->prepare("SELECT * FROM users WHERE id = ?");  $stmt->execute([$id]);
来源：http://3g.fehbvm.com/Article/details/gnpmazyzp.sHtML

[U70] PHP：PDO 事务
来源：http://blog.fehbvm.com/Article/details/gjeyilojq.sHtML

$pdo->beginTransaction();  $pdo->commit();  $pdo->rollBack();
来源：http://baike.fehbvm.com/Article/details/ggjspcfyg.sHtML

[U71] PHP：抛出异常
来源：http://www.blog.zdbjq.cn/Article/details/grxodrglg.sHtML

throw new RuntimeException("失败", 500);
来源：http://3g.zdbjq.cn/Article/details/gohhvppjo.sHtML

[U72] PHP：写错误日志
来源：http://www.share.fehbvm.com/Article/details/gtveugdsu.sHtML

error_log("失败: " . $e->getMessage());
来源：http://www.m.share.hesvh.cn/Article/details/gixxdwmsl.sHtML

[U73] PHP：读取 ini 配置
来源：http://www.blog.fehbvm.com/Article/details/gfskrkixg.sHtML

parse_ini_file("config.ini", true)
来源：http://www.m.share.hesvh.cn/Article/details/gggjkdqdi.sHtML

[U74] PHP：读取环境变量
来源：http://read.share.hesvh.cn/Article/details/gqkgoqdku.sHtML

getenv("APP_ENV") ?: "production"
来源：http://read.share.hesvh.cn/Article/details/gewcakatb.sHtML

[U75] PHP：依赖注入
来源：http://3g.zdbjq.cn/Article/details/grchjkieu.sHtML

composer require psr/container
来源：http://www.blog.fehbvm.com/Article/details/ghxoiaqut.sHtML

[U76] PHP：简单路由
来源：http://read.share.zdbjq.cn/Article/details/gvjbmnozk.sHtML

$path = parse_url($_SERVER["REQUEST_URI"], PHP_URL_PATH);
来源：http://m.share.fehbvm.com/Article/details/gkwpkiukn.sHtML

[U77] PHP：模板渲染
来源：http://wap.fehbvm.com/Article/details/grycautjj.sHtML

composer require twig/twig
来源：http://m.share.hesvh.cn/Article/details/gtdslqolp.sHtML

[U78] PHP：单元测试
来源：http://www.share.fehbvm.com/Article/details/gfwrzivku.sHtML

composer require --dev phpunit/phpunit
来源：http://m.share.hesvh.cn/Article/details/grmndfqam.sHtML

[U79] PHP：静态分析
来源：http://www.share.hesvh.cn/Article/details/gcuzhbvxg.sHtML

composer require --dev phpstan/phpstan
来源：http://blog.hesvh.cn/Article/details/gukrzcktl.sHtML

[U80] PHP：代码规范修复
来源：http://mobile.hesvh.cn/Article/details/gdtuxpukk.sHtML

composer require --dev friendsofphp/php-cs-fixer
来源：http://m.share.hesvh.cn/Article/details/glxcgnzig.sHtML

[U81] JS：初始化项目
来源：http://read.share.zdbjq.cn/Article/details/gslfokiqq.sHtML

npm init -y;  npm i express
来源：http://read.share.zdbjq.cn/Article/details/gnqmuszqg.sHtML

[U82] JS：package.json 脚本
来源：http://blog.hesvh.cn/Article/details/gtwecthig.sHtML

"scripts": { "dev": "vite", "build": "vite build" }
来源：http://www.share.hesvh.cn/Article/details/gytmjlzuu.sHtML

[U83] JS：ES Module 导入导出
来源：http://m.share.hesvh.cn/Article/details/gviyoeame.sHtML

export const a = 1;  import { a } from "./m.js";
来源：http://www.m.share.fehbvm.com/Article/details/gmrgsgnjd.sHtML

[U84] JS：CommonJS 写法
来源：http://www.blog.hesvh.cn/Article/details/gdlbdczfw.sHtML

module.exports = { a };  const { a } = require("./m");
来源：http://baike.zdbjq.cn/Article/details/gchjyicuh.sHtML

[U85] JS：可选链
来源：http://m.share.hesvh.cn/Article/details/ghajdfgwk.sHtML

a?.b?.c
来源：http://wap.zdbjq.cn/Article/details/gdjbkhuxc.sHtML

[U86] JS：空值合并
来源：http://www.share.fehbvm.com/Article/details/gacsimwcb.sHtML

a ?? b
来源：http://m.share.zdbjq.cn/Article/details/gyuobgcfq.sHtML

[U87] JS：解构默认值
来源：http://m.share.fehbvm.com/Article/details/gunhmmnhi.sHtML

const { a = 1, b = 2 } = obj;
来源：http://www.share.hesvh.cn/Article/details/gnfgothqb.sHtML

[U88] JS：对象展开合并
来源：http://baike.fehbvm.com/Article/details/gcslopxuv.sHtML

{ ...a, ...b }
来源：http://mobile.fehbvm.com/Article/details/ghjadjxay.sHtML

[U89] JS：数组去重
来源：http://blog.zdbjq.cn/Article/details/gjpcvgriy.sHtML

[...new Set(arr)]
来源：http://blog.hesvh.cn/Article/details/gjzszeywf.sHtML

[U90] JS：数字数组排序
来源：http://m.share.fehbvm.com/Article/details/glddgokec.sHtML

[...arr].sort((a, b) => a - b)
来源：http://m.share.hesvh.cn/Article/details/gjiibfxlb.sHtML

[U91] JS：对象键值遍历
来源：http://mobile.fehbvm.com/Article/details/gmfqvdxmw.sHtML

Object.entries(obj).forEach(([k, v]) => {});
来源：http://blog.fehbvm.com/Article/details/grbbhotzw.sHtML

[U92] JS：深拷贝
来源：http://www.blog.zdbjq.cn/Article/details/gcufpiqel.sHtML

structuredClone(obj)
来源：http://www.blog.fehbvm.com/Article/details/gopcpcacp.sHtML

[U93] JS：模板字符串
来源：http://www.m.share.zdbjq.cn/Article/details/gjpajzzdo.sHtML

`共 ${n} 条`
来源：http://www.share.fehbvm.com/Article/details/gtbzwdfha.sHtML

[U94] JS：箭头函数
来源：http://wap.zdbjq.cn/Article/details/gfofiixld.sHtML

const double = x => x * 2;
来源：http://m.share.fehbvm.com/Article/details/gpyvzdhkd.sHtML

[U95] JS：Promise 包装
来源：http://3g.zdbjq.cn/Article/details/gmiwdxeth.sHtML

new Promise((resolve, reject) => {})
来源：http://www.blog.zdbjq.cn/Article/details/gurkesbzk.sHtML

[U96] JS：async/await 与异常
来源：http://blog.hesvh.cn/Article/details/gfcjwbucd.sHtML

try { const d = await f(); } catch (e) { console.error(e); }
来源：http://read.share.fehbvm.com/Article/details/ghbcekczg.sHtML

[U97] JS：并发请求
来源：http://baike.zdbjq.cn/Article/details/gyqfqsfbl.sHtML

await Promise.all(urls.map(u => fetch(u)))
来源：http://m.share.fehbvm.com/Article/details/gjnaahnrl.sHtML

[U98] JS：fetch 带 JSON
来源：http://read.share.fehbvm.com/Article/details/ghkwajsdn.sHtML

await fetch(url, { method: "POST", headers: { "Content-Type": "application/json" }, body: JSON.stringify(d) })
来源：http://3g.fehbvm.com/Article/details/gkgqluvsu.sHtML

[U99] JS：事件监听
来源：http://blog.hesvh.cn/Article/details/gfzistqer.sHtML

el.addEventListener("click", e => {})
来源：http://blog.zdbjq.cn/Article/details/gggwmlrnj.sHtML

[U100] JS：DOM 查询
来源：http://m.share.zdbjq.cn/Article/details/gajqarsum.sHtML

document.querySelector(".item")
来源：http://mobile.hesvh.cn/Article/details/gglhcsngj.sHtML

[U101] JS：classList 操作
来源：http://www.share.fehbvm.com/Article/details/gwhckrtwi.sHtML

el.classList.toggle("active")
来源：http://read.share.fehbvm.com/Article/details/gbzmavwnq.sHtML

[U102] JS：本地存储
来源：http://read.share.hesvh.cn/Article/details/gdxcdjsao.sHtML

localStorage.setItem("k", JSON.stringify(v))
来源：http://www.m.share.fehbvm.com/Article/details/gsqfaqkmm.sHtML

[U103] JS：定时器
来源：http://www.blog.hesvh.cn/Article/details/gpqdejdke.sHtML

setTimeout(fn, 1000);  setInterval(fn, 1000);
来源：http://www.blog.hesvh.cn/Article/details/ggauqouyb.sHtML

[U104] JS：防抖
来源：http://baike.fehbvm.com/Article/details/gdiwmpcpd.sHtML

const debounce = (fn, ms) => { let t; return (...a) => { clearTimeout(t); t = setTimeout(() => fn(...a), ms); }; };
来源：http://baike.zdbjq.cn/Article/details/gnnaskast.sHtML

[U105] JS：节流
来源：http://baike.fehbvm.com/Article/details/gmdkecrxx.sHtML

const throttle = (fn, ms) => { let last = 0; return (...a) => { const n = Date.now(); if (n - last >= ms) { last = n; fn(...a); } }; };
来源：http://www.share.fehbvm.com/Article/details/gmlwkzlqf.sHtML

[U106] JS：日期格式化
来源：http://blog.hesvh.cn/Article/details/gywgxstph.sHtML

new Intl.DateTimeFormat("zh-CN", { dateStyle: "medium" }).format(new Date())
来源：http://3g.hesvh.cn/Article/details/ggdqtwrfn.sHtML

[U107] JS：数字千分位
来源：http://read.share.hesvh.cn/Article/details/gsiztubiz.sHtML

new Intl.NumberFormat("en-US").format(1234567)
来源：http://www.m.share.zdbjq.cn/Article/details/gexsdxmga.sHtML

[U108] JS：随机整数
来源：http://read.share.hesvh.cn/Article/details/gnbzjgawr.sHtML

Math.floor(Math.random() * (max - min + 1)) + min
来源：http://www.share.hesvh.cn/Article/details/gvkzptvse.sHtML

[U109] JS：数组分组
来源：http://m.share.zdbjq.cn/Article/details/gpvtaoucw.sHtML

Object.groupBy(arr, x => x.type)
来源：http://3g.hesvh.cn/Article/details/gbybtapgo.sHtML

[U110] JS：数组分块
来源：http://www.m.share.hesvh.cn/Article/details/ggvhkejia.sHtML

arr.reduce((acc, x, i) => (i % size ? acc : [...acc, arr.slice(i, i + size)]), [])
来源：http://www.blog.hesvh.cn/Article/details/gbxdfuslm.sHtML

[U111] JS：对象转 Map
来源：http://baike.zdbjq.cn/Article/details/ghcqagzyb.sHtML

new Map(Object.entries(obj))
来源：http://www.blog.fehbvm.com/Article/details/gulfuclwj.sHtML

[U112] JS：字符串补位
来源：http://blog.zdbjq.cn/Article/details/ggtigazgc.sHtML

"7".padStart(3, "0")
来源：http://www.share.zdbjq.cn/Article/details/gtdpmwunt.sHtML

[U113] JS：正则替换全部
来源：http://www.share.zdbjq.cn/Article/details/gqaxotupa.sHtML

s.replaceAll("a", "b")
来源：http://3g.zdbjq.cn/Article/details/gnqjnpsed.sHtML

[U114] JS：JSON 深比较
来源：http://m.share.zdbjq.cn/Article/details/grarevuja.sHtML

JSON.stringify(a) === JSON.stringify(b)
来源：http://blog.zdbjq.cn/Article/details/gowlfrexl.sHtML

[U115] JS：生成 UUID
来源：http://read.share.zdbjq.cn/Article/details/gwflqxohc.sHtML

crypto.randomUUID()
来源：http://mobile.zdbjq.cn/Article/details/gogcphgbp.sHtML

[U116] JS：类型检查（JSDoc）
来源：http://mobile.zdbjq.cn/Article/details/gnhbnspcu.sHtML

/** @param {string} name */ function f(name) {}
来源：http://read.share.zdbjq.cn/Article/details/grnwrdfmq.sHtML

[U117] JS：单元测试
来源：http://read.share.zdbjq.cn/Article/details/gkhftwzjp.sHtML

npm i -D vitest;  npx vitest
来源：http://baike.fehbvm.com/Article/details/gkchzylbu.sHtML

[U118] JS：开发服务器
来源：http://www.blog.zdbjq.cn/Article/details/gcmomebep.sHtML

npm i -D vite;  npx vite
来源：http://baike.zdbjq.cn/Article/details/ggorlfffj.sHtML

[U119] JS：生产构建
来源：http://blog.hesvh.cn/Article/details/gynahcvxa.sHtML

npx vite build
来源：http://3g.hesvh.cn/Article/details/gmzwruxge.sHtML

[U120] JS：读取环境变量（Vite）
来源：http://3g.fehbvm.com/Article/details/gvecnnqea.sHtML

import.meta.env.VITE_API_URL
来源：http://www.share.fehbvm.com/Article/details/gxkerbnby.sHtML

================================================================================
来源：http://www.blog.hesvh.cn/Article/details/gzrwxinwm.sHtML

统计汇总
来源：http://www.share.fehbvm.com/Article/details/grafrwjhd.sHtML

================================================================================
来源：http://www.blog.fehbvm.com/Article/details/ghwpbuaxm.sHtML

按语言统计（条）：
来源：http://read.share.hesvh.cn/Article/details/glzpiuqci.sHtML

Python ......... 252
来源：http://blog.fehbvm.com/Article/details/grxhbufdn.sHtML

PHP ............ 252
来源：http://m.share.zdbjq.cn/Article/details/glvejshkp.sHtML

JavaScript ..... 252
来源：http://www.share.hesvh.cn/Article/details/gqcgaznij.sHtML

TypeScript ..... 212
来源：http://www.share.fehbvm.com/Article/details/gihltfpph.sHtML

Java ........... 212
来源：http://3g.hesvh.cn/Article/details/gqcmirins.sHtML

Go ............. 212
来源：http://read.share.hesvh.cn/Article/details/ghqkwnaqv.sHtML

Ruby ........... 212
来源：http://blog.fehbvm.com/Article/details/gwifmutlh.sHtML

C# ............. 212
来源：http://3g.hesvh.cn/Article/details/gybcvxxby.sHtML

C .............. 30
来源：http://3g.fehbvm.com/Article/details/gwbbumgim.sHtML

C++ ............ 30
来源：http://mobile.fehbvm.com/Article/details/gtfvlgmge.sHtML

SQL ............ 90
来源：http://read.share.zdbjq.cn/Article/details/gjfiizsrf.sHtML

Bash ........... 80
来源：http://read.share.fehbvm.com/Article/details/gztbbytyd.sHtML

Kotlin ......... 15
来源：http://read.share.fehbvm.com/Article/details/gseniqkbc.sHtML

Swift .......... 15
来源：http://m.share.zdbjq.cn/Article/details/gynnmctrb.sHtML

Lua ............ 10
来源：http://m.share.fehbvm.com/Article/details/gbrslzbfh.sHtML

Perl ........... 10
来源：http://m.share.zdbjq.cn/Article/details/gzicjrxes.sHtML

Scala .......... 10
来源：http://www.m.share.zdbjq.cn/Article/details/gwuzledou.sHtML

------------------------------------
来源：http://www.m.share.zdbjq.cn/Article/details/gewavpifi.sHtML

合计 ........... 2106 条
来源：http://www.share.hesvh.cn/Article/details/gamahptyw.sHtML

按章节统计：
来源：http://www.blog.fehbvm.com/Article/details/gahjnqbza.sHtML

A 基础语法与类型       26 个任务 × 8 语言 =  208
来源：http://www.share.zdbjq.cn/Article/details/gxshdtnbo.sHtML

B 流程控制             16 个任务 × 8 语言 =  128
来源：http://m.share.hesvh.cn/Article/details/ggdzhthgv.sHtML

C 函数与作用域         16 个任务 × 8 语言 =  128
来源：http://www.blog.zdbjq.cn/Article/details/glfgoawdl.sHtML

D 数组 / 列表 / 集合   26 个任务 × 8 语言 =  208
来源：http://www.blog.zdbjq.cn/Article/details/gxfjobdxj.sHtML

E 字符串处理           22 个任务 × 8 语言 =  176
来源：http://www.m.share.hesvh.cn/Article/details/ghegegrxc.sHtML

F 文件与目录           12 个任务 × 8 语言 =   96
来源：http://baike.fehbvm.com/Article/details/gagckfuks.sHtML

G 面向对象             16 个任务 × 8 语言 =  128
来源：http://mobile.hesvh.cn/Article/details/gspffintp.sHtML

H 异常与错误处理       10 个任务 × 8 语言 =   80
来源：http://read.share.hesvh.cn/Article/details/gbhtmjgez.sHtML

I 正则表达式            8 个任务 × 8 语言 =   64
来源：http://wap.hesvh.cn/Article/details/gzoryudrk.sHtML

J 日期与时间           10 个任务 × 8 语言 =   80
来源：http://read.share.zdbjq.cn/Article/details/gflthmhvu.sHtML

K JSON 与序列化         8 个任务 × 8 语言 =   64
来源：http://3g.hesvh.cn/Article/details/gaufyhqye.sHtML

L 网络请求              8 个任务 × 8 语言 =   64
来源：http://wap.zdbjq.cn/Article/details/gwwkhkiix.sHtML

M 命令行 / 进程         8 个任务 × 8 语言 =   64
来源：http://mobile.fehbvm.com/Article/details/gnjxpvtjk.sHtML

N 数据结构与算法       12 个任务 × 8 语言 =   96
来源：http://mobile.zdbjq.cn/Article/details/gofokzkpg.sHtML

O 并发与异步            6 个任务 × 8 语言 =   48
来源：http://www.share.zdbjq.cn/Article/details/gjmrqrzht.sHtML

P 常用工具函数          8 个任务 × 8 语言 =   64
来源：http://blog.fehbvm.com/Article/details/gdjyihhjy.sHtML

Q SQL 专题                              90
来源：http://www.share.zdbjq.cn/Article/details/gctcyarhl.sHtML

R Bash 专题                             80
来源：http://read.share.fehbvm.com/Article/details/gyrbxjcvg.sHtML

S C / C++ 专题                          60
来源：http://www.m.share.zdbjq.cn/Article/details/gsmkouebj.sHtML

T 其他语言补充                          60
来源：http://read.share.zdbjq.cn/Article/details/gzaxlesps.sHtML

U 高频实用片段                         120
来源：http://blog.hesvh.cn/Article/details/gjshphzqu.sHtML

------------------------------------
来源：http://wap.zdbjq.cn/Article/details/gmertvcrh.sHtML

合计                                  2106 条
来源：http://mobile.zdbjq.cn/Article/details/gpkkeyovo.sHtML

--------------------------------------------------------------------------------
来源：http://baike.hesvh.cn/Article/details/gurvdqcgo.sHtML

使用提醒
来源：http://mobile.zdbjq.cn/Article/details/gjfkpxpps.sHtML

--------------------------------------------------------------------------------
来源：http://www.blog.fehbvm.com/Article/details/gfmxmyjkz.sHtML

1. 示例追求"最小可用"，正式项目中请补齐导入、错误处理与边界判断。
来源：http://mobile.hesvh.cn/Article/details/glidvikad.sHtML

2. 涉及文件、网络、数据库的示例，注意资源释放与异常捕获。
来源：http://blog.hesvh.cn/Article/details/gktynbuys.sHtML

3. 语言版本差异较大（如 Python 3.10 的 match、Java 17 的 record/switch 箭头），
来源：http://mobile.zdbjq.cn/Article/details/gzugatyme.sHtML

在旧版本上使用前请先确认语法支持情况。
来源：http://www.m.share.hesvh.cn/Article/details/gopvutltm.sHtML

4. 标注"手写"的条目是因为该语言缺少对应内置能力，实际项目中可引入成熟库。
来源：http://baike.hesvh.cn/Article/details/gwmfajkwp.sHtML

—— 文件结束 ——
来源：http://www.blog.fehbvm.com/Article/details/gelwgjrbc.sHtML

================================================================================
来源：http://blog.hesvh.cn/Article/details/glurzjxhq.sHtML

程序语言常见例子速查手册（2024 版）
来源：http://mobile.fehbvm.com/Article/details/gnqhdkecp.sHtML

Common Programming Examples Cheat Book
来源：http://3g.hesvh.cn/Article/details/gtyiwncsg.sHtML

================================================================================
来源：http://3g.fehbvm.com/Article/details/gmndvofva.sHtML

【收录内容】
来源：http://m.share.zdbjq.cn/Article/details/gasgvyfxe.sHtML

覆盖 12 种语言 / 语法与常见 API：
来源：http://www.m.share.fehbvm.com/Article/details/gmjnraebt.sHtML

Python · PHP · JavaScript · TypeScript · Java · Go · Ruby · C#
来源：http://www.blog.zdbjq.cn/Article/details/gfxgafwey.sHtML

SQL · Bash · C · C++
来源：http://www.blog.zdbjq.cn/Article/details/gmjxlsvps.sHtML

按「任务」分组：每个任务下按语言各给出一条最小可用示例。
来源：http://blog.hesvh.cn/Article/details/gcafeqwfd.sHtML

【使用说明】
来源：http://read.share.zdbjq.cn/Article/details/gousugjwv.sHtML

1. 每个任务形如 "[编号] 任务名"，下面每行以语言标记开头：
来源：http://www.m.share.fehbvm.com/Article/details/gcsqdzbva.sHtML

Py:    Python        PHP:   PHP           JS:    JavaScript
来源：http://wap.hesvh.cn/Article/details/gkidcdvxr.sHtML

TS:    TypeScript    Java:  Java          Go:    Go
来源：http://wap.hesvh.cn/Article/details/gcdbxtshl.sHtML

Ruby:  Ruby          C#:    C#            SQL:   SQL
来源：http://blog.zdbjq.cn/Article/details/gwjewyuli.sHtML

Bash:  Shell         C:     C             C++:   C++
来源：http://baike.hesvh.cn/Article/details/gxjkuovqh.sHtML

2. 示例只展示核心写法，刻意省略 import / require / include / using 等样板代码。
来源：http://3g.fehbvm.com/Article/details/gthkmltzj.sHtML

需要完整可运行文件时，请自行补齐当前语言的导入语句。
来源：http://m.share.hesvh.cn/Article/details/gdnnivlik.sHtML

3. 语法基准：Python 3.10+ / PHP 8.1+ / ES2020+ / TypeScript 5 / Java 17 /
来源：http://read.share.fehbvm.com/Article/details/giiwsmrrr.sHtML

Go 1.21+ / Ruby 3.x / C# 10+ / C17 / C++17。
来源：http://www.blog.fehbvm.com/Article/details/gfmnolpik.sHtML

4. 检索建议：用编辑器或浏览器 Ctrl+F 搜关键词，如 "排序" "读取文件" "正则"。
来源：http://www.blog.zdbjq.cn/Article/details/gmqjonmzo.sHtML

5. 标记为 "// 无" 表示该语言没有对应的一等语法，需用替代写法（示例给出替代方案）。
来源：http://wap.zdbjq.cn/Article/details/ghmvrhfed.sHtML

6. 符号 "⏎" 表示代码在此处换行（主要用于 Python 等强制缩进、无法压成一行的结构）。
来源：http://wap.hesvh.cn/Article/details/gwkkpoprk.sHtML

【文件统计】
来源：http://www.m.share.zdbjq.cn/Article/details/gbtmnapel.sHtML

语言示例共 2106 条，分布见本文末尾的「统计汇总」。
来源：http://read.share.zdbjq.cn/Article/details/gmbeeadkj.sHtML

--------------------------------------------------------------------------------
来源：http://www.m.share.fehbvm.com/Article/details/gwvxuhwja.sHtML

目  录
来源：http://www.blog.zdbjq.cn/Article/details/ghenczxpw.sHtML

--------------------------------------------------------------------------------
来源：http://baike.fehbvm.com/Article/details/gpgzhpdfn.sHtML

A. 基础语法与类型              （第 1 节，26 个任务，208 条）
来源：http://mobile.zdbjq.cn/Article/details/gxjgtzjrl.sHtML


<!-- 参考信息 -->