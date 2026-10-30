代发 wailian999

[U17] Py：初始化日志
来源：http://www.m.share.zdbjq.cn/Article/details/ggpqapaya.sHtML

logging.basicConfig(level=logging.INFO)
来源：http://www.share.zdbjq.cn/Article/details/glxoyzgil.sHtML

[U18] Py：预编译正则
来源：http://www.share.hesvh.cn/Article/details/gxvjbehaz.sHtML

pat = re.compile(r"\d+")
来源：http://mobile.hesvh.cn/Article/details/guzqijskk.sHtML

[U19] Py：正则替换带回调
来源：http://read.share.hesvh.cn/Article/details/gvfadxihc.sHtML

re.sub(r"\d+", lambda m: str(int(m.group()) * 2), s)
来源：http://baike.fehbvm.com/Article/details/gxfkqmlgx.sHtML

[U20] Py：缓存函数结果
来源：http://m.share.fehbvm.com/Article/details/gabjephtq.sHtML

@functools.lru_cache(maxsize=None)
来源：http://mobile.zdbjq.cn/Article/details/gegjrtzye.sHtML

[U21] Py：自定义上下文管理器
来源：http://www.share.fehbvm.com/Article/details/guekywyue.sHtML

@contextlib.contextmanager
来源：http://mobile.fehbvm.com/Article/details/gdmglvdzp.sHtML

[U22] Py：矩阵转置
来源：http://mobile.hesvh.cn/Article/details/girhfnfwv.sHtML

list(zip(*m))
来源：http://blog.zdbjq.cn/Article/details/gqbqssnmr.sHtML

[U23] Py：分块读取大文件
来源：http://wap.fehbvm.com/Article/details/gwoscetdb.sHtML

for chunk in iter(lambda: f.read(8192), b""):
来源：http://www.share.fehbvm.com/Article/details/gwvrghsiy.sHtML

[U24] Py：路径操作
来源：http://www.blog.hesvh.cn/Article/details/gujhwdheh.sHtML

Path("a/b.txt").parent.mkdir(parents=True, exist_ok=True)
来源：http://www.share.zdbjq.cn/Article/details/gxujaqrqg.sHtML

[U25] Py：CSV 按字典读
来源：http://m.share.zdbjq.cn/Article/details/gpkfyozyg.sHtML

csv.DictReader(f)
来源：http://3g.hesvh.cn/Article/details/gwnallzak.sHtML

[U26] Py：并发下载
来源：http://www.blog.zdbjq.cn/Article/details/gmfijanmf.sHtML

ThreadPoolExecutor(max_workers=8).map(fetch, urls)
来源：http://baike.fehbvm.com/Article/details/gzvdanmhs.sHtML

[U27] Py：异步 HTTP
来源：http://mobile.fehbvm.com/Article/details/gckxnwurd.sHtML

aiohttp.ClientSession() 配合 async with
来源：http://m.share.hesvh.cn/Article/details/gitvamkxz.sHtML

[U28] Py：类型别名
来源：http://mobile.zdbjq.cn/Article/details/gjucdtkcc.sHtML

UserId = int
来源：http://www.share.hesvh.cn/Article/details/ggrrbtzxf.sHtML

[U29] Py：属性校验
来源：http://read.share.fehbvm.com/Article/details/glaaaqxpd.sHtML

@property 与 @x.setter 配合
来源：http://www.m.share.hesvh.cn/Article/details/geyvfqdcd.sHtML

[U30] Py：数据类
来源：http://wap.zdbjq.cn/Article/details/gurecsplh.sHtML

@dataclass(slots=True)
来源：http://mobile.fehbvm.com/Article/details/gnaitxnru.sHtML

[U31] Py：单测
来源：http://read.share.zdbjq.cn/Article/details/gklmhvuvw.sHtML

python -m pytest -q
来源：http://3g.fehbvm.com/Article/details/gcprfvwgl.sHtML

[U32] Py：代码格式化
来源：http://m.share.fehbvm.com/Article/details/gusxkthca.sHtML

ruff format . && ruff check --fix .
来源：http://wap.zdbjq.cn/Article/details/gimvsslxi.sHtML

[U33] Py：打包发布
来源：http://www.m.share.hesvh.cn/Article/details/gvjigqksn.sHtML

python -m build  （依赖 pyproject.toml）
来源：http://blog.hesvh.cn/Article/details/gvlkrwvsk.sHtML

[U34] Py：判断编码
来源：http://blog.hesvh.cn/Article/details/gnhsnojwx.sHtML

chardet.detect(raw)
来源：http://www.share.hesvh.cn/Article/details/gehmxrawg.sHtML

[U35] Py：发送邮件
来源：http://mobile.hesvh.cn/Article/details/gsunggigw.sHtML

smtplib.SMTP_SSL(...).send_message(msg)
来源：http://read.share.hesvh.cn/Article/details/gthingcmc.sHtML

[U36] Py：定时任务
来源：http://wap.hesvh.cn/Article/details/gpdmssbmj.sHtML

schedule.every(10).minutes.do(job)
来源：http://3g.hesvh.cn/Article/details/gaxgxydfu.sHtML

[U37] Py：读写 Excel
来源：http://read.share.hesvh.cn/Article/details/gektabjaa.sHtML

pandas.read_excel / DataFrame.to_excel
来源：http://www.blog.zdbjq.cn/Article/details/gkvcrkizt.sHtML

[U38] Py：获取脚本所在目录
来源：http://read.share.fehbvm.com/Article/details/guzrsgdzb.sHtML

Path(__file__).resolve().parent
来源：http://blog.zdbjq.cn/Article/details/gbrcqciul.sHtML

[U39] Py：判断是否在交互环境
来源：http://wap.hesvh.cn/Article/details/gjygtbsmo.sHtML

sys.stdout.isatty()
来源：http://blog.hesvh.cn/Article/details/gsgfnskgm.sHtML

[U40] Py：打印到标准错误
来源：http://www.blog.zdbjq.cn/Article/details/ghgggsbva.sHtML

print("err", file=sys.stderr)
来源：http://wap.zdbjq.cn/Article/details/gufcidpuk.sHtML

[U41] PHP：初始化 Composer 项目
来源：http://baike.zdbjq.cn/Article/details/gkunyufqg.sHtML

composer init;  composer require guzzlehttp/guzzle
来源：http://www.blog.hesvh.cn/Article/details/grjgeevkp.sHtML

[U42] PHP：PSR-4 自动加载
来源：http://blog.fehbvm.com/Article/details/gjxhstowx.sHtML

"autoload": { "psr-4": { "App\\": "src/" } }
来源：http://www.m.share.fehbvm.com/Article/details/giursywdz.sHtML

[U43] PHP：声明命名空间
来源：http://www.m.share.fehbvm.com/Article/details/gllcxjxer.sHtML

namespace App\Http;
来源：http://www.m.share.hesvh.cn/Article/details/gkjytajxc.sHtML

[U44] PHP：开启严格类型
来源：http://www.share.hesvh.cn/Article/details/gbvbftgep.sHtML

declare(strict_types=1);
来源：http://www.m.share.zdbjq.cn/Article/details/gdekhndlw.sHtML

[U45] PHP：类型声明与返回类型
来源：http://baike.zdbjq.cn/Article/details/gflzzdcdy.sHtML

function add(int $a, int $b): int { return $a + $b; }
来源：http://www.m.share.zdbjq.cn/Article/details/gdlvzvhek.sHtML

[U46] PHP：可空类型
来源：http://blog.fehbvm.com/Article/details/gfuihbdcq.sHtML

?string $name = null
来源：http://read.share.fehbvm.com/Article/details/gorlytugv.sHtML

[U47] PHP：联合类型
来源：http://www.share.zdbjq.cn/Article/details/gqineklpg.sHtML

int|string $id
来源：http://m.share.fehbvm.com/Article/details/ghyxqhdwt.sHtML

[U48] PHP：纯枚举
来源：http://read.share.hesvh.cn/Article/details/guflutyoe.sHtML

enum Status: string { case Active = "active"; case Off = "off"; }
来源：http://baike.fehbvm.com/Article/details/gruwycxoq.sHtML

[U49] PHP：只读属性
来源：http://www.m.share.fehbvm.com/Article/details/gwkrqyirm.sHtML

public readonly string $name
来源：http://m.share.zdbjq.cn/Article/details/gjheralej.sHtML

[U50] PHP：构造器属性提升
来源：http://www.share.hesvh.cn/Article/details/gwdvftkjh.sHtML

public function __construct(private int $id) {}
来源：http://3g.hesvh.cn/Article/details/gmdqibgtk.sHtML

[U51] PHP：数组解构
来源：http://blog.zdbjq.cn/Article/details/guddtgrbc.sHtML

[$a, $b] = $arr;
来源：http://read.share.hesvh.cn/Article/details/gntvwvsrx.sHtML

[U52] PHP：箭头函数
来源：http://mobile.zdbjq.cn/Article/details/gevzztlue.sHtML

$double = fn($x) => $x * 2;
来源：http://mobile.fehbvm.com/Article/details/gczyqient.sHtML

[U53] PHP：空合并运算符
来源：http://www.share.zdbjq.cn/Article/details/glxnhwjoz.sHtML

$v = $a ?? $b ?? "default";
来源：http://www.m.share.hesvh.cn/Article/details/gtubbpeka.sHtML

[U54] PHP：空安全调用
来源：http://mobile.fehbvm.com/Article/details/gxcbfoyal.sHtML

$obj?->method()
来源：http://www.share.zdbjq.cn/Article/details/gnfdpgqga.sHtML

[U55] PHP：match 表达式
来源：http://read.share.zdbjq.cn/Article/details/gdqqcqqev.sHtML

$s = match($x) { 1 => "一", default => "其他" };
来源：http://blog.fehbvm.com/Article/details/gionenebr.sHtML

[U56] PHP：命名参数
来源：http://read.share.fehbvm.com/Article/details/gwesxjzne.sHtML

f(a: 1, b: 2)
来源：http://3g.fehbvm.com/Article/details/glkwugewb.sHtML

[U57] PHP：字符串插值
来源：http://m.share.hesvh.cn/Article/details/giusrotpy.sHtML

"值: {$a}"
来源：http://m.share.zdbjq.cn/Article/details/gpqbxaquj.sHtML

[U58] PHP：数组三件套
来源：http://baike.zdbjq.cn/Article/details/gbakqlidg.sHtML

array_map($f, $a);  array_filter($a, $f);  array_reduce($a, $f, 0);
来源：http://www.blog.zdbjq.cn/Article/details/grmmpjpse.sHtML

[U59] PHP：自定义排序
来源：http://wap.hesvh.cn/Article/details/glwnhkcqq.sHtML

usort($arr, fn($a, $b) => $a["age"] <=> $b["age"]);
来源：http://www.m.share.hesvh.cn/Article/details/gzigwztoc.sHtML

[U60] PHP：JSON 编解码
来源：http://wap.hesvh.cn/Article/details/gpchtyoml.sHtML

json_encode($d, JSON_UNESCAPED_UNICODE);  json_decode($s, true);
来源：http://baike.fehbvm.com/Article/details/geavzxjhs.sHtML

[U61] PHP：正则
来源：http://read.share.fehbvm.com/Article/details/gfxteqdaa.sHtML

preg_match('/(\d+)/', $s, $m);  preg_replace('/\d+/', '#', $s);
来源：http://www.share.fehbvm.com/Article/details/gbcekyheh.sHtML

[U62] PHP：日期对象
来源：http://www.m.share.fehbvm.com/Article/details/gbosuekgn.sHtML

(new DateTimeImmutable())->format("Y-m-d");
来源：http://3g.fehbvm.com/Article/details/gunivosgs.sHtML

[U63] PHP：文件读写
来源：http://www.m.share.fehbvm.com/Article/details/gjahqexeb.sHtML

file_get_contents($f);  file_put_contents($f, $data);
来源：http://wap.zdbjq.cn/Article/details/gjbdljlkx.sHtML

[U64] PHP：目录遍历
来源：http://3g.zdbjq.cn/Article/details/gfpbfzzvs.sHtML

glob("dir/*.php");  scandir("dir");
来源：http://baike.fehbvm.com/Article/details/gqivyzjpb.sHtML

[U65] PHP：会话
来源：http://3g.fehbvm.com/Article/details/gdowpblnp.sHtML

session_start();  $_SESSION["uid"] = 1;
来源：http://wap.zdbjq.cn/Article/details/ghpubhmoe.sHtML

[U66] PHP：设置 Cookie
来源：http://www.m.share.fehbvm.com/Article/details/gufbvzitj.sHtML

setcookie("token", $v, ["httponly" => true, "samesite" => "Lax"]);
来源：http://read.share.zdbjq.cn/Article/details/ggpzhbjsc.sHtML

[U67] PHP：处理文件上传
来源：http://wap.hesvh.cn/Article/details/gsstlcxmd.sHtML

$_FILES["file"]["tmp_name"] 与 move_uploaded_file()
来源：http://read.share.zdbjq.cn/Article/details/gfmvrbywe.sHtML

[U68] PHP：PDO 连接
来源：http://read.share.zdbjq.cn/Article/details/gizqzhohh.sHtML

$pdo = new PDO("mysql:host=localhost;dbname=app", "root", "");
来源：http://3g.fehbvm.com/Article/details/gtoltynwg.sHtML

[U69] PHP：PDO 预处理
来源：http://mobile.zdbjq.cn/Article/details/grgantijl.sHtML

$stmt = $pdo->prepare("SELECT * FROM users WHERE id = ?");  $stmt->execute([$id]);
来源：http://m.share.zdbjq.cn/Article/details/gzlaohvob.sHtML

[U70] PHP：PDO 事务
来源：http://mobile.zdbjq.cn/Article/details/gxcinezvz.sHtML

$pdo->beginTransaction();  $pdo->commit();  $pdo->rollBack();
来源：http://wap.hesvh.cn/Article/details/gdtpteadh.sHtML

[U71] PHP：抛出异常
来源：http://m.share.hesvh.cn/Article/details/gkushuifl.sHtML

throw new RuntimeException("失败", 500);
来源：http://3g.hesvh.cn/Article/details/gqkmcxvfl.sHtML

[U72] PHP：写错误日志
来源：http://wap.zdbjq.cn/Article/details/gmmedjjmi.sHtML

error_log("失败: " . $e->getMessage());
来源：http://www.share.fehbvm.com/Article/details/gvvstmfmx.sHtML

[U73] PHP：读取 ini 配置
来源：http://www.share.hesvh.cn/Article/details/gozsbaqxx.sHtML

parse_ini_file("config.ini", true)
来源：http://www.m.share.hesvh.cn/Article/details/gjkpqbeyl.sHtML

[U74] PHP：读取环境变量
来源：http://3g.fehbvm.com/Article/details/gjgsmfdyi.sHtML

getenv("APP_ENV") ?: "production"
来源：http://read.share.fehbvm.com/Article/details/gkzdkzflk.sHtML

[U75] PHP：依赖注入
来源：http://3g.hesvh.cn/Article/details/gnplkwpui.sHtML

composer require psr/container
来源：http://www.blog.hesvh.cn/Article/details/gajdcplrg.sHtML

[U76] PHP：简单路由
来源：http://read.share.zdbjq.cn/Article/details/gazvrmvkj.sHtML

$path = parse_url($_SERVER["REQUEST_URI"], PHP_URL_PATH);
来源：http://m.share.hesvh.cn/Article/details/gvffcsyji.sHtML

[U77] PHP：模板渲染
来源：http://www.m.share.hesvh.cn/Article/details/glzpicsmg.sHtML

composer require twig/twig
来源：http://www.blog.zdbjq.cn/Article/details/gthozbacp.sHtML

[U78] PHP：单元测试
来源：http://baike.fehbvm.com/Article/details/govqukzgz.sHtML

composer require --dev phpunit/phpunit
来源：http://www.m.share.hesvh.cn/Article/details/geaidcwpy.sHtML

[U79] PHP：静态分析
来源：http://www.share.zdbjq.cn/Article/details/gjefdocqb.sHtML

composer require --dev phpstan/phpstan
来源：http://www.blog.hesvh.cn/Article/details/gedgdigjz.sHtML

[U80] PHP：代码规范修复
来源：http://read.share.hesvh.cn/Article/details/gctzyfazb.sHtML

composer require --dev friendsofphp/php-cs-fixer
来源：http://wap.hesvh.cn/Article/details/gjabbljkn.sHtML

[U81] JS：初始化项目
来源：http://m.share.hesvh.cn/Article/details/gzpzvzmsy.sHtML

npm init -y;  npm i express
来源：http://m.share.fehbvm.com/Article/details/gdxeyljfy.sHtML

[U82] JS：package.json 脚本
来源：http://baike.zdbjq.cn/Article/details/gsvtsbucz.sHtML

"scripts": { "dev": "vite", "build": "vite build" }
来源：http://www.m.share.fehbvm.com/Article/details/gxpjvsoen.sHtML

[U83] JS：ES Module 导入导出
来源：http://www.share.hesvh.cn/Article/details/gflxwpdiw.sHtML

export const a = 1;  import { a } from "./m.js";
来源：http://baike.zdbjq.cn/Article/details/gtjztktyy.sHtML

[U84] JS：CommonJS 写法
来源：http://m.share.zdbjq.cn/Article/details/gnznpxhvj.sHtML

module.exports = { a };  const { a } = require("./m");
来源：http://www.blog.fehbvm.com/Article/details/gdpjvznpu.sHtML

[U85] JS：可选链
来源：http://blog.zdbjq.cn/Article/details/gxedquvvx.sHtML

a?.b?.c
来源：http://wap.fehbvm.com/Article/details/ggrinwada.sHtML

[U86] JS：空值合并
来源：http://baike.hesvh.cn/Article/details/gkodiyvmx.sHtML

a ?? b
来源：http://3g.zdbjq.cn/Article/details/glhabgsaw.sHtML

[U87] JS：解构默认值
来源：http://baike.hesvh.cn/Article/details/geenygkpx.sHtML

const { a = 1, b = 2 } = obj;
来源：http://www.blog.hesvh.cn/Article/details/gzqocjown.sHtML

[U88] JS：对象展开合并
来源：http://www.blog.zdbjq.cn/Article/details/gepmrtqry.sHtML

{ ...a, ...b }
来源：http://3g.fehbvm.com/Article/details/gqgsjjrmx.sHtML

[U89] JS：数组去重
来源：http://read.share.hesvh.cn/Article/details/gplfshxyw.sHtML

[...new Set(arr)]
来源：http://www.blog.fehbvm.com/Article/details/gyiigwurf.sHtML

[U90] JS：数字数组排序
来源：http://baike.hesvh.cn/Article/details/gbfyvetns.sHtML

[...arr].sort((a, b) => a - b)
来源：http://www.m.share.zdbjq.cn/Article/details/ggtmqygjf.sHtML

[U91] JS：对象键值遍历
来源：http://read.share.fehbvm.com/Article/details/gfvxoinmx.sHtML

Object.entries(obj).forEach(([k, v]) => {});
来源：http://m.share.hesvh.cn/Article/details/gxfdeaqop.sHtML

[U92] JS：深拷贝
来源：http://mobile.hesvh.cn/Article/details/geoxapeif.sHtML

structuredClone(obj)
来源：http://3g.hesvh.cn/Article/details/gmtubveai.sHtML

[U93] JS：模板字符串
来源：http://read.share.hesvh.cn/Article/details/ggjcnbplg.sHtML

`共 ${n} 条`
来源：http://blog.fehbvm.com/Article/details/gpgvorepc.sHtML

[U94] JS：箭头函数
来源：http://www.m.share.hesvh.cn/Article/details/glnxzopbr.sHtML

const double = x => x * 2;
来源：http://www.blog.hesvh.cn/Article/details/gljrwmkng.sHtML

[U95] JS：Promise 包装
来源：http://www.blog.hesvh.cn/Article/details/gebdsymrs.sHtML

new Promise((resolve, reject) => {})
来源：http://3g.fehbvm.com/Article/details/gowzqxdyy.sHtML

[U96] JS：async/await 与异常
来源：http://3g.fehbvm.com/Article/details/gaqkwetkt.sHtML

try { const d = await f(); } catch (e) { console.error(e); }
来源：http://mobile.zdbjq.cn/Article/details/gqstqgyjg.sHtML

[U97] JS：并发请求
来源：http://3g.hesvh.cn/Article/details/gzajobbpw.sHtML

await Promise.all(urls.map(u => fetch(u)))
来源：http://3g.hesvh.cn/Article/details/grjemzmrs.sHtML

[U98] JS：fetch 带 JSON
来源：http://www.m.share.fehbvm.com/Article/details/gyljplcfm.sHtML

await fetch(url, { method: "POST", headers: { "Content-Type": "application/json" }, body: JSON.stringify(d) })
来源：http://3g.zdbjq.cn/Article/details/gyejjamsx.sHtML

[U99] JS：事件监听
来源：http://3g.zdbjq.cn/Article/details/grzvwtfao.sHtML

el.addEventListener("click", e => {})
来源：http://www.blog.hesvh.cn/Article/details/gvpmotqsi.sHtML

[U100] JS：DOM 查询
来源：http://www.blog.fehbvm.com/Article/details/gtfiklzta.sHtML

document.querySelector(".item")
来源：http://3g.zdbjq.cn/Article/details/gxsalgbhd.sHtML

[U101] JS：classList 操作
来源：http://read.share.zdbjq.cn/Article/details/glipnhedq.sHtML

el.classList.toggle("active")
来源：http://baike.hesvh.cn/Article/details/gvzupdipd.sHtML

[U102] JS：本地存储
来源：http://m.share.fehbvm.com/Article/details/grxdoyhfi.sHtML

localStorage.setItem("k", JSON.stringify(v))
来源：http://www.m.share.hesvh.cn/Article/details/gmnwzowgm.sHtML

[U103] JS：定时器
来源：http://m.share.zdbjq.cn/Article/details/gachhxnow.sHtML

setTimeout(fn, 1000);  setInterval(fn, 1000);
来源：http://read.share.hesvh.cn/Article/details/gdqunjocg.sHtML

[U104] JS：防抖
来源：http://www.share.fehbvm.com/Article/details/gbnecwglt.sHtML

const debounce = (fn, ms) => { let t; return (...a) => { clearTimeout(t); t = setTimeout(() => fn(...a), ms); }; };
来源：http://baike.hesvh.cn/Article/details/gvogkwral.sHtML

[U105] JS：节流
来源：http://www.share.hesvh.cn/Article/details/gpbeumjfm.sHtML

const throttle = (fn, ms) => { let last = 0; return (...a) => { const n = Date.now(); if (n - last >= ms) { last = n; fn(...a); } }; };
来源：http://m.share.zdbjq.cn/Article/details/gneodypnw.sHtML

[U106] JS：日期格式化
来源：http://mobile.hesvh.cn/Article/details/ggjeqtbna.sHtML

new Intl.DateTimeFormat("zh-CN", { dateStyle: "medium" }).format(new Date())
来源：http://m.share.fehbvm.com/Article/details/gijwvntdx.sHtML

[U107] JS：数字千分位
来源：http://m.share.zdbjq.cn/Article/details/gzhcdrgti.sHtML

new Intl.NumberFormat("en-US").format(1234567)
来源：http://mobile.hesvh.cn/Article/details/gronckbxq.sHtML

[U108] JS：随机整数
来源：http://3g.fehbvm.com/Article/details/gzeftugnt.sHtML

Math.floor(Math.random() * (max - min + 1)) + min
来源：http://m.share.zdbjq.cn/Article/details/gbtyyaveq.sHtML

[U109] JS：数组分组
来源：http://mobile.hesvh.cn/Article/details/gnauvtlrh.sHtML

Object.groupBy(arr, x => x.type)
来源：http://wap.hesvh.cn/Article/details/grdcqcqjv.sHtML

[U110] JS：数组分块
来源：http://mobile.fehbvm.com/Article/details/gfqqdsmql.sHtML

arr.reduce((acc, x, i) => (i % size ? acc : [...acc, arr.slice(i, i + size)]), [])
来源：http://mobile.hesvh.cn/Article/details/gqwdplbxe.sHtML

[U111] JS：对象转 Map
来源：http://3g.zdbjq.cn/Article/details/gwbmeexgy.sHtML

new Map(Object.entries(obj))
来源：http://m.share.zdbjq.cn/Article/details/gkeeipbdx.sHtML

[U112] JS：字符串补位
来源：http://wap.zdbjq.cn/Article/details/gzqzlplzr.sHtML

"7".padStart(3, "0")
来源：http://www.blog.hesvh.cn/Article/details/gfrufqrny.sHtML

[U113] JS：正则替换全部
来源：http://mobile.hesvh.cn/Article/details/gimmmmfol.sHtML

s.replaceAll("a", "b")
来源：http://blog.fehbvm.com/Article/details/gusiwgeho.sHtML

[U114] JS：JSON 深比较
来源：http://m.share.zdbjq.cn/Article/details/gmxngwspq.sHtML

JSON.stringify(a) === JSON.stringify(b)
来源：http://mobile.fehbvm.com/Article/details/gqhaxrfai.sHtML

[U115] JS：生成 UUID
来源：http://www.blog.fehbvm.com/Article/details/gjziscpys.sHtML

crypto.randomUUID()
来源：http://www.blog.hesvh.cn/Article/details/gvjobcdjr.sHtML

[U116] JS：类型检查（JSDoc）
来源：http://www.blog.hesvh.cn/Article/details/gpxmzbofl.sHtML

/** @param {string} name */ function f(name) {}
来源：http://read.share.hesvh.cn/Article/details/gelthmasb.sHtML

[U117] JS：单元测试
来源：http://3g.hesvh.cn/Article/details/gylmckeuw.sHtML

npm i -D vitest;  npx vitest
来源：http://wap.fehbvm.com/Article/details/gnlinnrsh.sHtML

[U118] JS：开发服务器
来源：http://www.blog.hesvh.cn/Article/details/geifhnbgq.sHtML

npm i -D vite;  npx vite
来源：http://m.share.hesvh.cn/Article/details/garibcszl.sHtML

[U119] JS：生产构建
来源：http://www.share.hesvh.cn/Article/details/gkgfbdtou.sHtML

npx vite build
来源：http://mobile.zdbjq.cn/Article/details/gokbeledf.sHtML

[U120] JS：读取环境变量（Vite）
来源：http://wap.hesvh.cn/Article/details/gxtsjvbwj.sHtML

import.meta.env.VITE_API_URL
来源：http://mobile.hesvh.cn/Article/details/ggahaeskt.sHtML

================================================================================
来源：http://read.share.zdbjq.cn/Article/details/gnldnaxqf.sHtML

统计汇总
来源：http://baike.hesvh.cn/Article/details/giufecwlr.sHtML

================================================================================
来源：http://m.share.zdbjq.cn/Article/details/gptidmoeb.sHtML

按语言统计（条）：
来源：http://baike.zdbjq.cn/Article/details/gmkaaocho.sHtML

Python ......... 252
来源：http://www.blog.hesvh.cn/Article/details/grmiejyoi.sHtML

PHP ............ 252
来源：http://www.blog.hesvh.cn/Article/details/gkbxmcina.sHtML

JavaScript ..... 252
来源：http://baike.zdbjq.cn/Article/details/giahhizpb.sHtML

TypeScript ..... 212
来源：http://www.m.share.hesvh.cn/Article/details/gcxkduuej.sHtML

Java ........... 212
来源：http://www.blog.hesvh.cn/Article/details/ggqsfctny.sHtML

Go ............. 212
来源：http://m.share.hesvh.cn/Article/details/glqvgcpvo.sHtML

Ruby ........... 212
来源：http://read.share.hesvh.cn/Article/details/gmqdiizba.sHtML

C# ............. 212
来源：http://baike.hesvh.cn/Article/details/gzaognnll.sHtML

C .............. 30
来源：http://www.share.zdbjq.cn/Article/details/gtmrngwso.sHtML

C++ ............ 30
来源：http://read.share.hesvh.cn/Article/details/gwtogwkky.sHtML

SQL ............ 90
来源：http://3g.fehbvm.com/Article/details/gybvssbct.sHtML

Bash ........... 80
来源：http://www.m.share.zdbjq.cn/Article/details/gdvhxwzwq.sHtML

Kotlin ......... 15
来源：http://www.m.share.zdbjq.cn/Article/details/gfgpzmvcp.sHtML

Swift .......... 15
来源：http://wap.zdbjq.cn/Article/details/genyufzfh.sHtML

Lua ............ 10
来源：http://blog.hesvh.cn/Article/details/gblyjdcym.sHtML

Perl ........... 10
来源：http://blog.hesvh.cn/Article/details/gdhaslytd.sHtML

Scala .......... 10
来源：http://www.share.hesvh.cn/Article/details/gtjjypydv.sHtML

------------------------------------
来源：http://blog.hesvh.cn/Article/details/gumiywoqx.sHtML

合计 ........... 2106 条
来源：http://www.blog.zdbjq.cn/Article/details/gsphscjqf.sHtML

按章节统计：
来源：http://3g.fehbvm.com/Article/details/gngzbniin.sHtML

A 基础语法与类型       26 个任务 × 8 语言 =  208
来源：http://www.blog.fehbvm.com/Article/details/gleplkczp.sHtML

B 流程控制             16 个任务 × 8 语言 =  128
来源：http://read.share.zdbjq.cn/Article/details/gktylzjxc.sHtML

C 函数与作用域         16 个任务 × 8 语言 =  128
来源：http://m.share.zdbjq.cn/Article/details/ggzycxalv.sHtML

D 数组 / 列表 / 集合   26 个任务 × 8 语言 =  208
来源：http://www.m.share.fehbvm.com/Article/details/gnqrpcbwq.sHtML

E 字符串处理           22 个任务 × 8 语言 =  176
来源：http://www.m.share.hesvh.cn/Article/details/goxyyrlmw.sHtML

F 文件与目录           12 个任务 × 8 语言 =   96
来源：http://3g.hesvh.cn/Article/details/gtwkkmgzu.sHtML

G 面向对象             16 个任务 × 8 语言 =  128
来源：http://www.share.hesvh.cn/Article/details/ghebqpngx.sHtML

H 异常与错误处理       10 个任务 × 8 语言 =   80
来源：http://mobile.hesvh.cn/Article/details/geopyciyy.sHtML

I 正则表达式            8 个任务 × 8 语言 =   64
来源：http://blog.fehbvm.com/Article/details/goffomczc.sHtML

J 日期与时间           10 个任务 × 8 语言 =   80
来源：http://3g.fehbvm.com/Article/details/gehtkbnjg.sHtML

K JSON 与序列化         8 个任务 × 8 语言 =   64
来源：http://blog.zdbjq.cn/Article/details/gvlrsuaow.sHtML

L 网络请求              8 个任务 × 8 语言 =   64
来源：http://read.share.zdbjq.cn/Article/details/gimdxkxhg.sHtML

M 命令行 / 进程         8 个任务 × 8 语言 =   64
来源：http://www.share.fehbvm.com/Article/details/gixvnowhe.sHtML

N 数据结构与算法       12 个任务 × 8 语言 =   96
来源：http://wap.zdbjq.cn/Article/details/glipzfgnn.sHtML

O 并发与异步            6 个任务 × 8 语言 =   48
来源：http://read.share.zdbjq.cn/Article/details/gjozmrtvd.sHtML

P 常用工具函数          8 个任务 × 8 语言 =   64
来源：http://www.share.zdbjq.cn/Article/details/gzvylpmkd.sHtML

Q SQL 专题                              90
来源：http://baike.fehbvm.com/Article/details/gsgeyhknw.sHtML

R Bash 专题                             80
来源：http://read.share.fehbvm.com/Article/details/grgdeimoz.sHtML

S C / C++ 专题                          60
来源：http://www.m.share.zdbjq.cn/Article/details/ghjyyjtfj.sHtML

T 其他语言补充                          60
来源：http://blog.fehbvm.com/Article/details/gfjclccuy.sHtML

U 高频实用片段                         120
来源：http://m.share.zdbjq.cn/Article/details/ggmmulqyf.sHtML

------------------------------------
来源：http://www.blog.fehbvm.com/Article/details/gzutxauuq.sHtML

合计                                  2106 条
来源：http://read.share.zdbjq.cn/Article/details/gajmeawug.sHtML

--------------------------------------------------------------------------------
来源：http://3g.hesvh.cn/Article/details/gfhgzgvti.sHtML

使用提醒
来源：http://read.share.hesvh.cn/Article/details/gcpxplyss.sHtML

--------------------------------------------------------------------------------
来源：http://mobile.zdbjq.cn/Article/details/gumjiymfp.sHtML

1. 示例追求"最小可用"，正式项目中请补齐导入、错误处理与边界判断。
来源：http://wap.hesvh.cn/Article/details/ggzrmfxsa.sHtML

2. 涉及文件、网络、数据库的示例，注意资源释放与异常捕获。
来源：http://www.blog.zdbjq.cn/Article/details/gmvqutxea.sHtML

3. 语言版本差异较大（如 Python 3.10 的 match、Java 17 的 record/switch 箭头），
来源：http://m.share.fehbvm.com/Article/details/gcgvkwkar.sHtML

在旧版本上使用前请先确认语法支持情况。
来源：http://www.share.fehbvm.com/Article/details/gwndgxqrh.sHtML

4. 标注"手写"的条目是因为该语言缺少对应内置能力，实际项目中可引入成熟库。
来源：http://www.blog.fehbvm.com/Article/details/golnkrnpz.sHtML

—— 文件结束 ——
来源：http://mobile.zdbjq.cn/Article/details/gdfqhcdjw.sHtML

================================================================================
来源：http://baike.fehbvm.com/Article/details/gyigkugxr.sHtML

程序语言常见例子速查手册（2024 版）
来源：http://blog.zdbjq.cn/Article/details/gxwvscnxe.sHtML

Common Programming Examples Cheat Book
来源：http://www.m.share.hesvh.cn/Article/details/gebmfgyfg.sHtML

================================================================================
来源：http://m.share.zdbjq.cn/Article/details/gtzvtwivu.sHtML

【收录内容】
来源：http://blog.fehbvm.com/Article/details/gajgpxhki.sHtML

覆盖 12 种语言 / 语法与常见 API：
来源：http://www.m.share.hesvh.cn/Article/details/gpkgqxfro.sHtML

Python · PHP · JavaScript · TypeScript · Java · Go · Ruby · C#
来源：http://www.share.zdbjq.cn/Article/details/gohlxsezb.sHtML

SQL · Bash · C · C++
来源：http://www.blog.zdbjq.cn/Article/details/gevypiuxy.sHtML

按「任务」分组：每个任务下按语言各给出一条最小可用示例。
来源：http://read.share.fehbvm.com/Article/details/glqgyuwxq.sHtML

【使用说明】
来源：http://wap.zdbjq.cn/Article/details/glfbgnfat.sHtML

1. 每个任务形如 "[编号] 任务名"，下面每行以语言标记开头：
来源：http://www.m.share.fehbvm.com/Article/details/gsqazviar.sHtML

Py:    Python        PHP:   PHP           JS:    JavaScript
来源：http://www.share.fehbvm.com/Article/details/glyozholg.sHtML

TS:    TypeScript    Java:  Java          Go:    Go
来源：http://www.share.fehbvm.com/Article/details/gvnqxxygk.sHtML

Ruby:  Ruby          C#:    C#            SQL:   SQL
来源：http://www.m.share.hesvh.cn/Article/details/ggekkrwzt.sHtML

Bash:  Shell         C:     C             C++:   C++
来源：http://3g.hesvh.cn/Article/details/gliufuwyk.sHtML

2. 示例只展示核心写法，刻意省略 import / require / include / using 等样板代码。
来源：http://blog.zdbjq.cn/Article/details/gwcgwsyvo.sHtML

需要完整可运行文件时，请自行补齐当前语言的导入语句。
来源：http://blog.fehbvm.com/Article/details/gzheeckoj.sHtML

3. 语法基准：Python 3.10+ / PHP 8.1+ / ES2020+ / TypeScript 5 / Java 17 /
来源：http://www.blog.hesvh.cn/Article/details/gjemlifvi.sHtML

Go 1.21+ / Ruby 3.x / C# 10+ / C17 / C++17。
来源：http://baike.zdbjq.cn/Article/details/ggbmldhhr.sHtML

4. 检索建议：用编辑器或浏览器 Ctrl+F 搜关键词，如 "排序" "读取文件" "正则"。
来源：http://www.m.share.hesvh.cn/Article/details/gbebulola.sHtML

5. 标记为 "// 无" 表示该语言没有对应的一等语法，需用替代写法（示例给出替代方案）。
来源：http://read.share.zdbjq.cn/Article/details/gcuuznghv.sHtML

6. 符号 "⏎" 表示代码在此处换行（主要用于 Python 等强制缩进、无法压成一行的结构）。
来源：http://wap.hesvh.cn/Article/details/gnuifxacy.sHtML

【文件统计】
来源：http://wap.hesvh.cn/Article/details/gdsjviikt.sHtML

语言示例共 2106 条，分布见本文末尾的「统计汇总」。
来源：http://mobile.zdbjq.cn/Article/details/gvlzscwlx.sHtML

--------------------------------------------------------------------------------
来源：http://mobile.zdbjq.cn/Article/details/gzmvfgskt.sHtML

目  录
来源：http://3g.hesvh.cn/Article/details/gfmmrepou.sHtML

--------------------------------------------------------------------------------
来源：http://mobile.zdbjq.cn/Article/details/gkylzjtpi.sHtML

A. 基础语法与类型              （第 1 节，26 个任务，208 条）
来源：http://www.m.share.zdbjq.cn/Article/details/gxmekrrhq.sHtML

B. 流程控制                    （第 2 节，16 个任务，128 条）
来源：http://www.m.share.zdbjq.cn/Article/details/gioklsloh.sHtML

C. 函数与作用域                （第 3 节，16 个任务，128 条）
来源：http://read.share.fehbvm.com/Article/details/ggycjowot.sHtML

D. 数组 / 列表 / 集合          （第 4 节，26 个任务，208 条）
来源：http://mobile.zdbjq.cn/Article/details/gcispdqwk.sHtML

E. 字符串处理                  （第 5 节，22 个任务，176 条）
来源：http://wap.hesvh.cn/Article/details/gteprqtte.sHtML

F. 文件与目录                  （第 6 节，12 个任务，96 条）
来源：http://baike.fehbvm.com/Article/details/ggcfssszk.sHtML

G. 面向对象                    （第 7 节，16 个任务，128 条）
来源：http://www.blog.zdbjq.cn/Article/details/gnmjothdi.sHtML

H. 异常与错误处理              （第 8 节，10 个任务，80 条）
来源：http://www.share.fehbvm.com/Article/details/gauotfztp.sHtML

I. 正则表达式                  （第 9 节，8 个任务，64 条）
来源：http://mobile.hesvh.cn/Article/details/gqcdebuxk.sHtML


<!-- 参考信息 -->