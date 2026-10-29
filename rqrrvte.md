代发 wailian999

[U15] Py：高精度计时
来源：http://3g.fehbvm.com/Article/details/gfahhyrup.sHtML

t = time.perf_counter()
来源：http://blog.zdbjq.cn/Article/details/gxhbqujfw.sHtML

[U16] Py：命令行参数解析
来源：http://www.blog.fehbvm.com/Article/details/gtxqelrkd.sHtML

ap = argparse.ArgumentParser();  ap.add_argument("--name");  args = ap.parse_args()
来源：http://3g.hesvh.cn/Article/details/gaqzlcrdp.sHtML

[U17] Py：初始化日志
来源：http://3g.zdbjq.cn/Article/details/gejpmyjsm.sHtML

logging.basicConfig(level=logging.INFO)
来源：http://3g.hesvh.cn/Article/details/gnesqsdsa.sHtML

[U18] Py：预编译正则
来源：http://www.share.hesvh.cn/Article/details/gyqdpdxge.sHtML

pat = re.compile(r"\d+")
来源：http://www.blog.fehbvm.com/Article/details/gyboavpni.sHtML

[U19] Py：正则替换带回调
来源：http://blog.fehbvm.com/Article/details/gqksegsib.sHtML

re.sub(r"\d+", lambda m: str(int(m.group()) * 2), s)
来源：http://mobile.fehbvm.com/Article/details/gerhbgdiz.sHtML

[U20] Py：缓存函数结果
来源：http://read.share.zdbjq.cn/Article/details/gmlgymydc.sHtML

@functools.lru_cache(maxsize=None)
来源：http://www.blog.hesvh.cn/Article/details/gonwmccro.sHtML

[U21] Py：自定义上下文管理器
来源：http://www.blog.hesvh.cn/Article/details/gdwxxjmuk.sHtML

@contextlib.contextmanager
来源：http://www.m.share.hesvh.cn/Article/details/gocqaqjtf.sHtML

[U22] Py：矩阵转置
来源：http://m.share.fehbvm.com/Article/details/ggawjrhbl.sHtML

list(zip(*m))
来源：http://wap.hesvh.cn/Article/details/gcztmhbkl.sHtML

[U23] Py：分块读取大文件
来源：http://mobile.zdbjq.cn/Article/details/gkeorafwc.sHtML

for chunk in iter(lambda: f.read(8192), b""):
来源：http://3g.hesvh.cn/Article/details/gxzasciuf.sHtML

[U24] Py：路径操作
来源：http://3g.fehbvm.com/Article/details/gegxdueho.sHtML

Path("a/b.txt").parent.mkdir(parents=True, exist_ok=True)
来源：http://www.share.fehbvm.com/Article/details/giokrbofj.sHtML

[U25] Py：CSV 按字典读
来源：http://www.share.fehbvm.com/Article/details/glodwsqgv.sHtML

csv.DictReader(f)
来源：http://blog.fehbvm.com/Article/details/gjsvprcoc.sHtML

[U26] Py：并发下载
来源：http://m.share.zdbjq.cn/Article/details/griwgscrp.sHtML

ThreadPoolExecutor(max_workers=8).map(fetch, urls)
来源：http://m.share.zdbjq.cn/Article/details/grouetbjy.sHtML

[U27] Py：异步 HTTP
来源：http://wap.zdbjq.cn/Article/details/gsgjlgjqi.sHtML

aiohttp.ClientSession() 配合 async with
来源：http://www.share.fehbvm.com/Article/details/gaicgjgbp.sHtML

[U28] Py：类型别名
来源：http://www.m.share.hesvh.cn/Article/details/gvoopqpxd.sHtML

UserId = int
来源：http://www.blog.fehbvm.com/Article/details/gffkqpphy.sHtML

[U29] Py：属性校验
来源：http://mobile.zdbjq.cn/Article/details/goyipyqnb.sHtML

@property 与 @x.setter 配合
来源：http://blog.hesvh.cn/Article/details/glzqyxlty.sHtML

[U30] Py：数据类
来源：http://baike.hesvh.cn/Article/details/gdwlgyjmf.sHtML

@dataclass(slots=True)
来源：http://3g.hesvh.cn/Article/details/gwhexkdzs.sHtML

[U31] Py：单测
来源：http://www.share.zdbjq.cn/Article/details/guedegtti.sHtML

python -m pytest -q
来源：http://www.m.share.fehbvm.com/Article/details/gqcumowbc.sHtML

[U32] Py：代码格式化
来源：http://baike.hesvh.cn/Article/details/ghgnkmuie.sHtML

ruff format . && ruff check --fix .
来源：http://www.share.fehbvm.com/Article/details/giuoqjrfm.sHtML

[U33] Py：打包发布
来源：http://mobile.zdbjq.cn/Article/details/geccrbnxv.sHtML

python -m build  （依赖 pyproject.toml）
来源：http://www.share.hesvh.cn/Article/details/gozrycfff.sHtML

[U34] Py：判断编码
来源：http://www.blog.hesvh.cn/Article/details/gnerwuajq.sHtML

chardet.detect(raw)
来源：http://blog.fehbvm.com/Article/details/gjmyqgrbn.sHtML

[U35] Py：发送邮件
来源：http://baike.hesvh.cn/Article/details/gbvmgpkiw.sHtML

smtplib.SMTP_SSL(...).send_message(msg)
来源：http://wap.zdbjq.cn/Article/details/gpzbbyzmv.sHtML

[U36] Py：定时任务
来源：http://baike.zdbjq.cn/Article/details/gqajfjzwp.sHtML

schedule.every(10).minutes.do(job)
来源：http://wap.hesvh.cn/Article/details/gbpvksywb.sHtML

[U37] Py：读写 Excel
来源：http://www.share.zdbjq.cn/Article/details/gvyyvegtb.sHtML

pandas.read_excel / DataFrame.to_excel
来源：http://www.share.zdbjq.cn/Article/details/gfdwqtuch.sHtML

[U38] Py：获取脚本所在目录
来源：http://www.m.share.zdbjq.cn/Article/details/gfcrskagk.sHtML

Path(__file__).resolve().parent
来源：http://wap.fehbvm.com/Article/details/glyfosxmr.sHtML

[U39] Py：判断是否在交互环境
来源：http://read.share.hesvh.cn/Article/details/gfursquhi.sHtML

sys.stdout.isatty()
来源：http://m.share.fehbvm.com/Article/details/ghzdcixly.sHtML

[U40] Py：打印到标准错误
来源：http://3g.fehbvm.com/Article/details/guntbfcge.sHtML

print("err", file=sys.stderr)
来源：http://m.share.zdbjq.cn/Article/details/gbpugdubf.sHtML

[U41] PHP：初始化 Composer 项目
来源：http://3g.zdbjq.cn/Article/details/ghcvmkhph.sHtML

composer init;  composer require guzzlehttp/guzzle
来源：http://www.share.zdbjq.cn/Article/details/guuqkaidf.sHtML

[U42] PHP：PSR-4 自动加载
来源：http://blog.hesvh.cn/Article/details/gecauvrak.sHtML

"autoload": { "psr-4": { "App\\": "src/" } }
来源：http://mobile.hesvh.cn/Article/details/guuwhwlde.sHtML

[U43] PHP：声明命名空间
来源：http://wap.fehbvm.com/Article/details/gtzuqcjej.sHtML

namespace App\Http;
来源：http://www.m.share.zdbjq.cn/Article/details/gbeibpano.sHtML

[U44] PHP：开启严格类型
来源：http://3g.fehbvm.com/Article/details/gnicoxjxo.sHtML

declare(strict_types=1);
来源：http://wap.zdbjq.cn/Article/details/gwjruorwq.sHtML

[U45] PHP：类型声明与返回类型
来源：http://wap.fehbvm.com/Article/details/gtmphewfa.sHtML

function add(int $a, int $b): int { return $a + $b; }
来源：http://www.blog.fehbvm.com/Article/details/ggjcbqglt.sHtML

[U46] PHP：可空类型
来源：http://baike.zdbjq.cn/Article/details/gxixwkmri.sHtML

?string $name = null
来源：http://wap.zdbjq.cn/Article/details/grnldxvgt.sHtML

[U47] PHP：联合类型
来源：http://www.blog.zdbjq.cn/Article/details/gczfnuice.sHtML

int|string $id
来源：http://m.share.fehbvm.com/Article/details/gkhmmagzp.sHtML

[U48] PHP：纯枚举
来源：http://www.m.share.hesvh.cn/Article/details/gluqigcwo.sHtML

enum Status: string { case Active = "active"; case Off = "off"; }
来源：http://www.share.hesvh.cn/Article/details/gfboixozm.sHtML

[U49] PHP：只读属性
来源：http://3g.hesvh.cn/Article/details/gaaffzdci.sHtML

public readonly string $name
来源：http://m.share.hesvh.cn/Article/details/gmudvnoui.sHtML

[U50] PHP：构造器属性提升
来源：http://3g.zdbjq.cn/Article/details/gelrlqahp.sHtML

public function __construct(private int $id) {}
来源：http://www.share.zdbjq.cn/Article/details/giyzdrxju.sHtML

[U51] PHP：数组解构
来源：http://www.m.share.hesvh.cn/Article/details/gsjieyypr.sHtML

[$a, $b] = $arr;
来源：http://blog.hesvh.cn/Article/details/gkqiqzvth.sHtML

[U52] PHP：箭头函数
来源：http://www.m.share.fehbvm.com/Article/details/geisxqdhy.sHtML

$double = fn($x) => $x * 2;
来源：http://3g.hesvh.cn/Article/details/gksqsieqo.sHtML

[U53] PHP：空合并运算符
来源：http://www.m.share.hesvh.cn/Article/details/gwypcsfqx.sHtML

$v = $a ?? $b ?? "default";
来源：http://m.share.fehbvm.com/Article/details/guljtrzgl.sHtML

[U54] PHP：空安全调用
来源：http://www.blog.fehbvm.com/Article/details/gtsyxyvwg.sHtML

$obj?->method()
来源：http://m.share.hesvh.cn/Article/details/gevpumctq.sHtML

[U55] PHP：match 表达式
来源：http://www.m.share.zdbjq.cn/Article/details/glghsgnky.sHtML

$s = match($x) { 1 => "一", default => "其他" };
来源：http://blog.hesvh.cn/Article/details/gcookqbym.sHtML

[U56] PHP：命名参数
来源：http://blog.zdbjq.cn/Article/details/gxgndwcgq.sHtML

f(a: 1, b: 2)
来源：http://baike.fehbvm.com/Article/details/gkxutevnh.sHtML

[U57] PHP：字符串插值
来源：http://mobile.fehbvm.com/Article/details/gwhvplisd.sHtML

"值: {$a}"
来源：http://mobile.hesvh.cn/Article/details/gpsltvzhy.sHtML

[U58] PHP：数组三件套
来源：http://m.share.fehbvm.com/Article/details/gerhiofve.sHtML

array_map($f, $a);  array_filter($a, $f);  array_reduce($a, $f, 0);
来源：http://www.share.fehbvm.com/Article/details/gvqzlquyv.sHtML

[U59] PHP：自定义排序
来源：http://read.share.hesvh.cn/Article/details/gyeeekiwy.sHtML

usort($arr, fn($a, $b) => $a["age"] <=> $b["age"]);
来源：http://read.share.zdbjq.cn/Article/details/gdvfidrtf.sHtML

[U60] PHP：JSON 编解码
来源：http://wap.zdbjq.cn/Article/details/gifcehksm.sHtML

json_encode($d, JSON_UNESCAPED_UNICODE);  json_decode($s, true);
来源：http://www.blog.fehbvm.com/Article/details/glwnlaxoi.sHtML

[U61] PHP：正则
来源：http://3g.hesvh.cn/Article/details/gpeddhxli.sHtML

preg_match('/(\d+)/', $s, $m);  preg_replace('/\d+/', '#', $s);
来源：http://www.m.share.hesvh.cn/Article/details/gxkotcicz.sHtML

[U62] PHP：日期对象
来源：http://www.m.share.zdbjq.cn/Article/details/gfwhquhhc.sHtML

(new DateTimeImmutable())->format("Y-m-d");
来源：http://read.share.zdbjq.cn/Article/details/gpkrpoklq.sHtML

[U63] PHP：文件读写
来源：http://3g.hesvh.cn/Article/details/ggpmbjgys.sHtML

file_get_contents($f);  file_put_contents($f, $data);
来源：http://baike.zdbjq.cn/Article/details/gpvxlslja.sHtML

[U64] PHP：目录遍历
来源：http://www.m.share.hesvh.cn/Article/details/gftxqadix.sHtML

glob("dir/*.php");  scandir("dir");
来源：http://www.blog.fehbvm.com/Article/details/gtugbrhhw.sHtML

[U65] PHP：会话
来源：http://www.blog.hesvh.cn/Article/details/gwoaocefh.sHtML

session_start();  $_SESSION["uid"] = 1;
来源：http://m.share.fehbvm.com/Article/details/gkjginwyr.sHtML

[U66] PHP：设置 Cookie
来源：http://mobile.hesvh.cn/Article/details/gmmjqrwnj.sHtML

setcookie("token", $v, ["httponly" => true, "samesite" => "Lax"]);
来源：http://www.blog.hesvh.cn/Article/details/guwbgqqbj.sHtML

[U67] PHP：处理文件上传
来源：http://m.share.zdbjq.cn/Article/details/gxxovdcem.sHtML

$_FILES["file"]["tmp_name"] 与 move_uploaded_file()
来源：http://blog.fehbvm.com/Article/details/gmndzbtgo.sHtML

[U68] PHP：PDO 连接
来源：http://baike.fehbvm.com/Article/details/gwromcqos.sHtML

$pdo = new PDO("mysql:host=localhost;dbname=app", "root", "");
来源：http://www.blog.fehbvm.com/Article/details/gpqvjnhgv.sHtML

[U69] PHP：PDO 预处理
来源：http://www.m.share.zdbjq.cn/Article/details/guyqcvkdj.sHtML

$stmt = $pdo->prepare("SELECT * FROM users WHERE id = ?");  $stmt->execute([$id]);
来源：http://wap.hesvh.cn/Article/details/grqrgifbm.sHtML

[U70] PHP：PDO 事务
来源：http://www.share.zdbjq.cn/Article/details/gprnphvvw.sHtML

$pdo->beginTransaction();  $pdo->commit();  $pdo->rollBack();
来源：http://m.share.hesvh.cn/Article/details/gkaeliknq.sHtML

[U71] PHP：抛出异常
来源：http://www.m.share.hesvh.cn/Article/details/gbvyrzxbx.sHtML

throw new RuntimeException("失败", 500);
来源：http://www.share.zdbjq.cn/Article/details/gwlbaafdu.sHtML

[U72] PHP：写错误日志
来源：http://wap.zdbjq.cn/Article/details/gjsczqcxc.sHtML

error_log("失败: " . $e->getMessage());
来源：http://blog.fehbvm.com/Article/details/gexdduisb.sHtML

[U73] PHP：读取 ini 配置
来源：http://www.blog.zdbjq.cn/Article/details/gudscbakx.sHtML

parse_ini_file("config.ini", true)
来源：http://mobile.hesvh.cn/Article/details/glrrzbviu.sHtML

[U74] PHP：读取环境变量
来源：http://blog.fehbvm.com/Article/details/gwzcsprjz.sHtML

getenv("APP_ENV") ?: "production"
来源：http://3g.zdbjq.cn/Article/details/grilgkfgi.sHtML

[U75] PHP：依赖注入
来源：http://www.blog.fehbvm.com/Article/details/gihhfzjpz.sHtML

composer require psr/container
来源：http://baike.fehbvm.com/Article/details/gvsovouvq.sHtML

[U76] PHP：简单路由
来源：http://mobile.zdbjq.cn/Article/details/gtxotrmgj.sHtML

$path = parse_url($_SERVER["REQUEST_URI"], PHP_URL_PATH);
来源：http://wap.zdbjq.cn/Article/details/gzsbcgjqd.sHtML

[U77] PHP：模板渲染
来源：http://read.share.fehbvm.com/Article/details/gunklafkh.sHtML

composer require twig/twig
来源：http://www.share.fehbvm.com/Article/details/gfqlmgdzs.sHtML

[U78] PHP：单元测试
来源：http://www.share.hesvh.cn/Article/details/gprzhwuls.sHtML

composer require --dev phpunit/phpunit
来源：http://blog.zdbjq.cn/Article/details/gxwsdgsmm.sHtML

[U79] PHP：静态分析
来源：http://read.share.fehbvm.com/Article/details/gbwropptl.sHtML

composer require --dev phpstan/phpstan
来源：http://3g.zdbjq.cn/Article/details/gowjygrhc.sHtML

[U80] PHP：代码规范修复
来源：http://read.share.fehbvm.com/Article/details/gjuvjjlzm.sHtML

composer require --dev friendsofphp/php-cs-fixer
来源：http://baike.hesvh.cn/Article/details/gagrerkvi.sHtML

[U81] JS：初始化项目
来源：http://blog.fehbvm.com/Article/details/gtxtjiebx.sHtML

npm init -y;  npm i express
来源：http://mobile.zdbjq.cn/Article/details/grxyvurcm.sHtML

[U82] JS：package.json 脚本
来源：http://www.m.share.fehbvm.com/Article/details/gtjukjpsx.sHtML

"scripts": { "dev": "vite", "build": "vite build" }
来源：http://www.share.zdbjq.cn/Article/details/gkfoggymf.sHtML

[U83] JS：ES Module 导入导出
来源：http://www.share.fehbvm.com/Article/details/gttbmbzmg.sHtML

export const a = 1;  import { a } from "./m.js";
来源：http://baike.fehbvm.com/Article/details/gaxrypebf.sHtML

[U84] JS：CommonJS 写法
来源：http://mobile.hesvh.cn/Article/details/gnjgnkgvr.sHtML

module.exports = { a };  const { a } = require("./m");
来源：http://blog.hesvh.cn/Article/details/gjgcnnamk.sHtML

[U85] JS：可选链
来源：http://read.share.hesvh.cn/Article/details/gdgjzbeua.sHtML

a?.b?.c
来源：http://3g.fehbvm.com/Article/details/gspefbkpl.sHtML

[U86] JS：空值合并
来源：http://mobile.hesvh.cn/Article/details/gexnwstra.sHtML

a ?? b
来源：http://m.share.fehbvm.com/Article/details/gysffifms.sHtML

[U87] JS：解构默认值
来源：http://mobile.zdbjq.cn/Article/details/gdambjlqe.sHtML

const { a = 1, b = 2 } = obj;
来源：http://baike.hesvh.cn/Article/details/gjghsjzkj.sHtML

[U88] JS：对象展开合并
来源：http://blog.hesvh.cn/Article/details/gffxemrcy.sHtML

{ ...a, ...b }
来源：http://wap.fehbvm.com/Article/details/gjfhhhlcu.sHtML

[U89] JS：数组去重
来源：http://mobile.fehbvm.com/Article/details/gzkdvmzat.sHtML

[...new Set(arr)]
来源：http://m.share.hesvh.cn/Article/details/guvayuayr.sHtML

[U90] JS：数字数组排序
来源：http://read.share.zdbjq.cn/Article/details/gdhdkudqn.sHtML

[...arr].sort((a, b) => a - b)
来源：http://www.blog.hesvh.cn/Article/details/grenkfbnt.sHtML

[U91] JS：对象键值遍历
来源：http://m.share.zdbjq.cn/Article/details/ghmgnwwbe.sHtML

Object.entries(obj).forEach(([k, v]) => {});
来源：http://blog.fehbvm.com/Article/details/ggzgwvfyn.sHtML

[U92] JS：深拷贝
来源：http://www.m.share.hesvh.cn/Article/details/gbuhxdftb.sHtML

structuredClone(obj)
来源：http://www.m.share.hesvh.cn/Article/details/gpyumtfds.sHtML

[U93] JS：模板字符串
来源：http://www.m.share.zdbjq.cn/Article/details/gzrpmadhb.sHtML

`共 ${n} 条`
来源：http://mobile.hesvh.cn/Article/details/gwukvzwcv.sHtML

[U94] JS：箭头函数
来源：http://blog.hesvh.cn/Article/details/gzuyejnwh.sHtML

const double = x => x * 2;
来源：http://read.share.zdbjq.cn/Article/details/gixitvxxi.sHtML

[U95] JS：Promise 包装
来源：http://wap.zdbjq.cn/Article/details/gdklkhteg.sHtML

new Promise((resolve, reject) => {})
来源：http://www.blog.hesvh.cn/Article/details/grhmswqju.sHtML

[U96] JS：async/await 与异常
来源：http://www.blog.fehbvm.com/Article/details/giiidptcr.sHtML

try { const d = await f(); } catch (e) { console.error(e); }
来源：http://www.blog.hesvh.cn/Article/details/gabzjwhfj.sHtML

[U97] JS：并发请求
来源：http://mobile.hesvh.cn/Article/details/gdqajamdu.sHtML

await Promise.all(urls.map(u => fetch(u)))
来源：http://www.m.share.zdbjq.cn/Article/details/gcinfehqs.sHtML

[U98] JS：fetch 带 JSON
来源：http://wap.zdbjq.cn/Article/details/gderhrpbk.sHtML

await fetch(url, { method: "POST", headers: { "Content-Type": "application/json" }, body: JSON.stringify(d) })
来源：http://m.share.zdbjq.cn/Article/details/gtghknram.sHtML

[U99] JS：事件监听
来源：http://mobile.zdbjq.cn/Article/details/gtvcqhrat.sHtML

el.addEventListener("click", e => {})
来源：http://read.share.hesvh.cn/Article/details/gytgezkuv.sHtML

[U100] JS：DOM 查询
来源：http://3g.fehbvm.com/Article/details/gzynlhxbh.sHtML

document.querySelector(".item")
来源：http://read.share.hesvh.cn/Article/details/gmdvbwngf.sHtML

[U101] JS：classList 操作
来源：http://www.share.fehbvm.com/Article/details/gzbbwmfbn.sHtML

el.classList.toggle("active")
来源：http://www.blog.zdbjq.cn/Article/details/gcmikckge.sHtML

[U102] JS：本地存储
来源：http://read.share.hesvh.cn/Article/details/gbyzwtkya.sHtML

localStorage.setItem("k", JSON.stringify(v))
来源：http://3g.zdbjq.cn/Article/details/gxpphznam.sHtML

[U103] JS：定时器
来源：http://www.share.fehbvm.com/Article/details/ganodoegn.sHtML

setTimeout(fn, 1000);  setInterval(fn, 1000);
来源：http://www.m.share.zdbjq.cn/Article/details/gibcggmqd.sHtML

[U104] JS：防抖
来源：http://baike.zdbjq.cn/Article/details/gagdsuxuz.sHtML

const debounce = (fn, ms) => { let t; return (...a) => { clearTimeout(t); t = setTimeout(() => fn(...a), ms); }; };
来源：http://www.m.share.zdbjq.cn/Article/details/gphwbwjjl.sHtML

[U105] JS：节流
来源：http://www.share.fehbvm.com/Article/details/gtboxvurl.sHtML

const throttle = (fn, ms) => { let last = 0; return (...a) => { const n = Date.now(); if (n - last >= ms) { last = n; fn(...a); } }; };
来源：http://m.share.fehbvm.com/Article/details/gvuqnczni.sHtML

[U106] JS：日期格式化
来源：http://m.share.hesvh.cn/Article/details/gtjrddutd.sHtML

new Intl.DateTimeFormat("zh-CN", { dateStyle: "medium" }).format(new Date())
来源：http://www.share.hesvh.cn/Article/details/glgkvdgeq.sHtML

[U107] JS：数字千分位
来源：http://www.blog.fehbvm.com/Article/details/gzadvahpv.sHtML

new Intl.NumberFormat("en-US").format(1234567)
来源：http://www.m.share.hesvh.cn/Article/details/gmskejcdm.sHtML

[U108] JS：随机整数
来源：http://www.blog.hesvh.cn/Article/details/gsnleiawz.sHtML

Math.floor(Math.random() * (max - min + 1)) + min
来源：http://3g.fehbvm.com/Article/details/gyyrqnxdj.sHtML

[U109] JS：数组分组
来源：http://www.m.share.hesvh.cn/Article/details/gbnxeefys.sHtML

Object.groupBy(arr, x => x.type)
来源：http://baike.hesvh.cn/Article/details/gwgegbnvs.sHtML

[U110] JS：数组分块
来源：http://baike.fehbvm.com/Article/details/ggbyfgybt.sHtML

arr.reduce((acc, x, i) => (i % size ? acc : [...acc, arr.slice(i, i + size)]), [])
来源：http://mobile.fehbvm.com/Article/details/gslxichwx.sHtML

[U111] JS：对象转 Map
来源：http://m.share.hesvh.cn/Article/details/gfmuwmtuy.sHtML

new Map(Object.entries(obj))
来源：http://read.share.zdbjq.cn/Article/details/gwcweveat.sHtML

[U112] JS：字符串补位
来源：http://www.blog.fehbvm.com/Article/details/gdrbkwblg.sHtML

"7".padStart(3, "0")
来源：http://baike.fehbvm.com/Article/details/gkmmivxim.sHtML

[U113] JS：正则替换全部
来源：http://read.share.fehbvm.com/Article/details/grdmzesrt.sHtML

s.replaceAll("a", "b")
来源：http://read.share.zdbjq.cn/Article/details/gribzvsow.sHtML

[U114] JS：JSON 深比较
来源：http://wap.fehbvm.com/Article/details/gkigqgnav.sHtML

JSON.stringify(a) === JSON.stringify(b)
来源：http://www.blog.fehbvm.com/Article/details/gmneanhkk.sHtML

[U115] JS：生成 UUID
来源：http://www.share.hesvh.cn/Article/details/gzsajosnq.sHtML

crypto.randomUUID()
来源：http://m.share.hesvh.cn/Article/details/gbkkxszjg.sHtML

[U116] JS：类型检查（JSDoc）
来源：http://wap.zdbjq.cn/Article/details/gfcdshqji.sHtML

/** @param {string} name */ function f(name) {}
来源：http://3g.fehbvm.com/Article/details/gldugfftg.sHtML

[U117] JS：单元测试
来源：http://read.share.fehbvm.com/Article/details/gacpfuujg.sHtML

npm i -D vitest;  npx vitest
来源：http://www.share.fehbvm.com/Article/details/gxtmmmykr.sHtML

[U118] JS：开发服务器
来源：http://blog.hesvh.cn/Article/details/gxeqcacnz.sHtML

npm i -D vite;  npx vite
来源：http://mobile.hesvh.cn/Article/details/gwzngfimc.sHtML

[U119] JS：生产构建
来源：http://www.share.zdbjq.cn/Article/details/givqpgalr.sHtML

npx vite build
来源：http://read.share.zdbjq.cn/Article/details/goilzkldf.sHtML

[U120] JS：读取环境变量（Vite）
来源：http://www.blog.zdbjq.cn/Article/details/gzvwsfjye.sHtML

import.meta.env.VITE_API_URL
来源：http://read.share.hesvh.cn/Article/details/gnbwfyktm.sHtML

================================================================================
来源：http://mobile.hesvh.cn/Article/details/gdarjcjpb.sHtML

统计汇总
来源：http://blog.fehbvm.com/Article/details/gtdvtpbdg.sHtML

================================================================================
来源：http://baike.hesvh.cn/Article/details/gcgwtyxnl.sHtML

按语言统计（条）：
来源：http://mobile.hesvh.cn/Article/details/gxgrnhocg.sHtML

Python ......... 252
来源：http://baike.fehbvm.com/Article/details/gdvipygrk.sHtML

PHP ............ 252
来源：http://www.blog.zdbjq.cn/Article/details/ghfcqrhre.sHtML

JavaScript ..... 252
来源：http://www.blog.hesvh.cn/Article/details/gelkohafe.sHtML

TypeScript ..... 212
来源：http://3g.zdbjq.cn/Article/details/gkiywgxdr.sHtML

Java ........... 212
来源：http://3g.zdbjq.cn/Article/details/gmzrdngnq.sHtML

Go ............. 212
来源：http://read.share.fehbvm.com/Article/details/gtppnvxeu.sHtML

Ruby ........... 212
来源：http://wap.zdbjq.cn/Article/details/gnxzfhqdr.sHtML

C# ............. 212
来源：http://www.share.hesvh.cn/Article/details/gimrqxuxy.sHtML

C .............. 30
来源：http://blog.hesvh.cn/Article/details/gvjnmgqif.sHtML

C++ ............ 30
来源：http://baike.zdbjq.cn/Article/details/geylfhmmq.sHtML

SQL ............ 90
来源：http://mobile.hesvh.cn/Article/details/gugmdlren.sHtML

Bash ........... 80
来源：http://www.share.hesvh.cn/Article/details/girqjggla.sHtML

Kotlin ......... 15
来源：http://www.m.share.fehbvm.com/Article/details/gryrgbuht.sHtML

Swift .......... 15
来源：http://3g.hesvh.cn/Article/details/guwihpcvs.sHtML

Lua ............ 10
来源：http://read.share.zdbjq.cn/Article/details/glanqnwli.sHtML

Perl ........... 10
来源：http://www.share.fehbvm.com/Article/details/gybtpwane.sHtML

Scala .......... 10
来源：http://wap.fehbvm.com/Article/details/gqoltznhu.sHtML

------------------------------------
来源：http://read.share.hesvh.cn/Article/details/ghewpnfuu.sHtML

合计 ........... 2106 条
来源：http://read.share.hesvh.cn/Article/details/ggkcejuei.sHtML

按章节统计：
来源：http://3g.zdbjq.cn/Article/details/gfiwsxtad.sHtML

A 基础语法与类型       26 个任务 × 8 语言 =  208
来源：http://baike.zdbjq.cn/Article/details/grklnyonz.sHtML

B 流程控制             16 个任务 × 8 语言 =  128
来源：http://www.blog.fehbvm.com/Article/details/gputdgguj.sHtML

C 函数与作用域         16 个任务 × 8 语言 =  128
来源：http://blog.hesvh.cn/Article/details/gvkygumre.sHtML

D 数组 / 列表 / 集合   26 个任务 × 8 语言 =  208
来源：http://www.share.zdbjq.cn/Article/details/geiypjmts.sHtML

E 字符串处理           22 个任务 × 8 语言 =  176
来源：http://www.blog.hesvh.cn/Article/details/gnnlyjgyh.sHtML

F 文件与目录           12 个任务 × 8 语言 =   96
来源：http://baike.fehbvm.com/Article/details/gvpxkxjzd.sHtML

G 面向对象             16 个任务 × 8 语言 =  128
来源：http://www.share.hesvh.cn/Article/details/guyueugxz.sHtML

H 异常与错误处理       10 个任务 × 8 语言 =   80
来源：http://baike.zdbjq.cn/Article/details/gmizkrkdk.sHtML

I 正则表达式            8 个任务 × 8 语言 =   64
来源：http://mobile.zdbjq.cn/Article/details/gnbrkaakl.sHtML

J 日期与时间           10 个任务 × 8 语言 =   80
来源：http://www.share.fehbvm.com/Article/details/gswlwbcbl.sHtML

K JSON 与序列化         8 个任务 × 8 语言 =   64
来源：http://www.m.share.fehbvm.com/Article/details/gkyxxtpdw.sHtML

L 网络请求              8 个任务 × 8 语言 =   64
来源：http://blog.zdbjq.cn/Article/details/gmbqilelm.sHtML

M 命令行 / 进程         8 个任务 × 8 语言 =   64
来源：http://baike.fehbvm.com/Article/details/gyrunmxef.sHtML

N 数据结构与算法       12 个任务 × 8 语言 =   96
来源：http://www.share.fehbvm.com/Article/details/gkmwhnqtd.sHtML

O 并发与异步            6 个任务 × 8 语言 =   48
来源：http://wap.hesvh.cn/Article/details/gqiksniqo.sHtML

P 常用工具函数          8 个任务 × 8 语言 =   64
来源：http://www.m.share.fehbvm.com/Article/details/gdqivnbms.sHtML

Q SQL 专题                              90
来源：http://read.share.hesvh.cn/Article/details/gosaoemfn.sHtML

R Bash 专题                             80
来源：http://wap.fehbvm.com/Article/details/ggdjflylp.sHtML

S C / C++ 专题                          60
来源：http://baike.fehbvm.com/Article/details/grotuyobf.sHtML

T 其他语言补充                          60
来源：http://baike.fehbvm.com/Article/details/gckbgcfwr.sHtML

U 高频实用片段                         120
来源：http://mobile.fehbvm.com/Article/details/gurgivtir.sHtML

------------------------------------
来源：http://3g.hesvh.cn/Article/details/gkbvcrefu.sHtML

合计                                  2106 条
来源：http://www.m.share.fehbvm.com/Article/details/gklnatxgy.sHtML

--------------------------------------------------------------------------------
来源：http://m.share.fehbvm.com/Article/details/geicsuasa.sHtML

使用提醒
来源：http://blog.hesvh.cn/Article/details/gqvbsaazd.sHtML

--------------------------------------------------------------------------------
来源：http://mobile.hesvh.cn/Article/details/gquhezuzz.sHtML

1. 示例追求"最小可用"，正式项目中请补齐导入、错误处理与边界判断。
来源：http://baike.fehbvm.com/Article/details/gznznhely.sHtML

2. 涉及文件、网络、数据库的示例，注意资源释放与异常捕获。
来源：http://www.m.share.hesvh.cn/Article/details/gevwrsdcz.sHtML

3. 语言版本差异较大（如 Python 3.10 的 match、Java 17 的 record/switch 箭头），
来源：http://www.share.hesvh.cn/Article/details/gcqywjkqs.sHtML

在旧版本上使用前请先确认语法支持情况。
来源：http://blog.fehbvm.com/Article/details/gieodbhzi.sHtML

4. 标注"手写"的条目是因为该语言缺少对应内置能力，实际项目中可引入成熟库。
来源：http://www.blog.zdbjq.cn/Article/details/gcphazjcc.sHtML

—— 文件结束 ——
来源：http://m.share.hesvh.cn/Article/details/gmksntdre.sHtML

================================================================================
来源：http://wap.zdbjq.cn/Article/details/gzlnwujig.sHtML

程序语言常见例子速查手册（2024 版）
来源：http://read.share.zdbjq.cn/Article/details/gxhzehnkm.sHtML

Common Programming Examples Cheat Book
来源：http://www.blog.fehbvm.com/Article/details/gnhtzyghm.sHtML

================================================================================
来源：http://m.share.fehbvm.com/Article/details/gxvncryxy.sHtML

【收录内容】
来源：http://read.share.hesvh.cn/Article/details/gprzlvoyf.sHtML

覆盖 12 种语言 / 语法与常见 API：
来源：http://mobile.zdbjq.cn/Article/details/grlpceozp.sHtML

Python · PHP · JavaScript · TypeScript · Java · Go · Ruby · C#
来源：http://baike.hesvh.cn/Article/details/gqkhrmdyl.sHtML

SQL · Bash · C · C++
来源：http://read.share.hesvh.cn/Article/details/gvtaqsbuv.sHtML

按「任务」分组：每个任务下按语言各给出一条最小可用示例。
来源：http://baike.zdbjq.cn/Article/details/gruaifdvx.sHtML

【使用说明】
来源：http://www.blog.hesvh.cn/Article/details/givaiobjo.sHtML

1. 每个任务形如 "[编号] 任务名"，下面每行以语言标记开头：
来源：http://www.share.zdbjq.cn/Article/details/gwklyzxds.sHtML

Py:    Python        PHP:   PHP           JS:    JavaScript
来源：http://www.m.share.fehbvm.com/Article/details/gupwqqnfr.sHtML

TS:    TypeScript    Java:  Java          Go:    Go
来源：http://blog.fehbvm.com/Article/details/gbgzelvop.sHtML

Ruby:  Ruby          C#:    C#            SQL:   SQL
来源：http://m.share.hesvh.cn/Article/details/gnzykyubz.sHtML

Bash:  Shell         C:     C             C++:   C++
来源：http://www.share.fehbvm.com/Article/details/gmgowhaug.sHtML

2. 示例只展示核心写法，刻意省略 import / require / include / using 等样板代码。
来源：http://www.m.share.hesvh.cn/Article/details/giianyoom.sHtML

需要完整可运行文件时，请自行补齐当前语言的导入语句。
来源：http://m.share.fehbvm.com/Article/details/gvejipovw.sHtML

3. 语法基准：Python 3.10+ / PHP 8.1+ / ES2020+ / TypeScript 5 / Java 17 /
来源：http://www.blog.zdbjq.cn/Article/details/gpswqojzs.sHtML

Go 1.21+ / Ruby 3.x / C# 10+ / C17 / C++17。
来源：http://read.share.fehbvm.com/Article/details/gcpoufwpc.sHtML

4. 检索建议：用编辑器或浏览器 Ctrl+F 搜关键词，如 "排序" "读取文件" "正则"。
来源：http://3g.fehbvm.com/Article/details/gsmrebnqf.sHtML

5. 标记为 "// 无" 表示该语言没有对应的一等语法，需用替代写法（示例给出替代方案）。
来源：http://wap.zdbjq.cn/Article/details/gcndzqljc.sHtML

6. 符号 "⏎" 表示代码在此处换行（主要用于 Python 等强制缩进、无法压成一行的结构）。
来源：http://m.share.hesvh.cn/Article/details/gqoesoutl.sHtML

【文件统计】
来源：http://3g.fehbvm.com/Article/details/gpfmyhxbp.sHtML

语言示例共 2106 条，分布见本文末尾的「统计汇总」。
来源：http://read.share.fehbvm.com/Article/details/gntehfgnk.sHtML

--------------------------------------------------------------------------------
来源：http://mobile.fehbvm.com/Article/details/gylfpegvq.sHtML

目  录
来源：http://www.share.hesvh.cn/Article/details/glwvkausf.sHtML

--------------------------------------------------------------------------------
来源：http://www.blog.zdbjq.cn/Article/details/guayjbjum.sHtML

A. 基础语法与类型              （第 1 节，26 个任务，208 条）
来源：http://www.m.share.fehbvm.com/Article/details/gsgqbdxfw.sHtML

B. 流程控制                    （第 2 节，16 个任务，128 条）
来源：http://baike.fehbvm.com/Article/details/gorqlaskv.sHtML

C. 函数与作用域                （第 3 节，16 个任务，128 条）
来源：http://read.share.zdbjq.cn/Article/details/grrvupceb.sHtML

D. 数组 / 列表 / 集合          （第 4 节，26 个任务，208 条）
来源：http://www.m.share.hesvh.cn/Article/details/gihdncdmj.sHtML

E. 字符串处理                  （第 5 节，22 个任务，176 条）
来源：http://baike.zdbjq.cn/Article/details/geknbrrfb.sHtML


<!-- 参考信息 -->