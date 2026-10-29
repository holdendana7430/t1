代发 wailian999

[U15] Py：高精度计时
来源：http://m.share.fehbvm.com/Article/details/ghimdjyeg.sHtML

t = time.perf_counter()
来源：http://www.blog.hesvh.cn/Article/details/gscltkbuh.sHtML

[U16] Py：命令行参数解析
来源：http://3g.hesvh.cn/Article/details/gicpzhgym.sHtML

ap = argparse.ArgumentParser();  ap.add_argument("--name");  args = ap.parse_args()
来源：http://mobile.fehbvm.com/Article/details/gqmvobgeu.sHtML

[U17] Py：初始化日志
来源：http://wap.hesvh.cn/Article/details/gclnzqjqo.sHtML

logging.basicConfig(level=logging.INFO)
来源：http://blog.zdbjq.cn/Article/details/gfdxlmctk.sHtML

[U18] Py：预编译正则
来源：http://www.share.zdbjq.cn/Article/details/gafetstys.sHtML

pat = re.compile(r"\d+")
来源：http://m.share.zdbjq.cn/Article/details/gzksoqsbj.sHtML

[U19] Py：正则替换带回调
来源：http://read.share.zdbjq.cn/Article/details/gzzfrvriw.sHtML

re.sub(r"\d+", lambda m: str(int(m.group()) * 2), s)
来源：http://m.share.hesvh.cn/Article/details/gwpuqakjz.sHtML

[U20] Py：缓存函数结果
来源：http://www.m.share.fehbvm.com/Article/details/grrexqcab.sHtML

@functools.lru_cache(maxsize=None)
来源：http://www.blog.hesvh.cn/Article/details/gmsfskrjo.sHtML

[U21] Py：自定义上下文管理器
来源：http://blog.zdbjq.cn/Article/details/gmrykruko.sHtML

@contextlib.contextmanager
来源：http://blog.hesvh.cn/Article/details/gtstnibvs.sHtML

[U22] Py：矩阵转置
来源：http://3g.hesvh.cn/Article/details/ghslgtkvk.sHtML

list(zip(*m))
来源：http://3g.hesvh.cn/Article/details/gmfqiekgp.sHtML

[U23] Py：分块读取大文件
来源：http://3g.fehbvm.com/Article/details/gtrbnrpip.sHtML

for chunk in iter(lambda: f.read(8192), b""):
来源：http://read.share.zdbjq.cn/Article/details/grjsnjakq.sHtML

[U24] Py：路径操作
来源：http://read.share.fehbvm.com/Article/details/gcgtsyovo.sHtML

Path("a/b.txt").parent.mkdir(parents=True, exist_ok=True)
来源：http://read.share.hesvh.cn/Article/details/gdpoglaxh.sHtML

[U25] Py：CSV 按字典读
来源：http://www.m.share.hesvh.cn/Article/details/gvmnmkidq.sHtML

csv.DictReader(f)
来源：http://blog.zdbjq.cn/Article/details/gzaxkcvhh.sHtML

[U26] Py：并发下载
来源：http://www.blog.hesvh.cn/Article/details/gchvwambg.sHtML

ThreadPoolExecutor(max_workers=8).map(fetch, urls)
来源：http://read.share.hesvh.cn/Article/details/ggmonfltb.sHtML

[U27] Py：异步 HTTP
来源：http://m.share.zdbjq.cn/Article/details/gpionmxdq.sHtML

aiohttp.ClientSession() 配合 async with
来源：http://mobile.fehbvm.com/Article/details/gpsirqbgs.sHtML

[U28] Py：类型别名
来源：http://blog.fehbvm.com/Article/details/gifgivbza.sHtML

UserId = int
来源：http://www.share.hesvh.cn/Article/details/gkaulzmpn.sHtML

[U29] Py：属性校验
来源：http://read.share.zdbjq.cn/Article/details/gblaxhkqk.sHtML

@property 与 @x.setter 配合
来源：http://m.share.hesvh.cn/Article/details/guoyywydf.sHtML

[U30] Py：数据类
来源：http://www.m.share.zdbjq.cn/Article/details/gvzlfwtpn.sHtML

@dataclass(slots=True)
来源：http://m.share.zdbjq.cn/Article/details/glokweeqb.sHtML

[U31] Py：单测
来源：http://baike.hesvh.cn/Article/details/ghtdwcedk.sHtML

python -m pytest -q
来源：http://www.m.share.hesvh.cn/Article/details/gerqevyux.sHtML

[U32] Py：代码格式化
来源：http://read.share.fehbvm.com/Article/details/gmivtcrmb.sHtML

ruff format . && ruff check --fix .
来源：http://read.share.hesvh.cn/Article/details/gltgyqjnd.sHtML

[U33] Py：打包发布
来源：http://m.share.fehbvm.com/Article/details/gfmymctxm.sHtML

python -m build  （依赖 pyproject.toml）
来源：http://3g.zdbjq.cn/Article/details/gdgotpqqi.sHtML

[U34] Py：判断编码
来源：http://mobile.zdbjq.cn/Article/details/gihgiljxf.sHtML

chardet.detect(raw)
来源：http://www.m.share.zdbjq.cn/Article/details/grjmwmkfz.sHtML

[U35] Py：发送邮件
来源：http://blog.zdbjq.cn/Article/details/glkpuoysw.sHtML

smtplib.SMTP_SSL(...).send_message(msg)
来源：http://mobile.zdbjq.cn/Article/details/gfdxgrylo.sHtML

[U36] Py：定时任务
来源：http://blog.fehbvm.com/Article/details/gaaitdexw.sHtML

schedule.every(10).minutes.do(job)
来源：http://www.blog.fehbvm.com/Article/details/getpbazdx.sHtML

[U37] Py：读写 Excel
来源：http://www.blog.zdbjq.cn/Article/details/gthjzzxee.sHtML

pandas.read_excel / DataFrame.to_excel
来源：http://www.share.hesvh.cn/Article/details/gnzyxjqtx.sHtML

[U38] Py：获取脚本所在目录
来源：http://www.share.fehbvm.com/Article/details/grnjbbgww.sHtML

Path(__file__).resolve().parent
来源：http://baike.fehbvm.com/Article/details/gofstjpyh.sHtML

[U39] Py：判断是否在交互环境
来源：http://read.share.hesvh.cn/Article/details/gjwqvvbgz.sHtML

sys.stdout.isatty()
来源：http://mobile.fehbvm.com/Article/details/ghknvpdvh.sHtML

[U40] Py：打印到标准错误
来源：http://wap.hesvh.cn/Article/details/gebfjknae.sHtML

print("err", file=sys.stderr)
来源：http://www.blog.hesvh.cn/Article/details/gcziskqks.sHtML

[U41] PHP：初始化 Composer 项目
来源：http://www.blog.zdbjq.cn/Article/details/ganprpisp.sHtML

composer init;  composer require guzzlehttp/guzzle
来源：http://wap.hesvh.cn/Article/details/gaduavmjb.sHtML

[U42] PHP：PSR-4 自动加载
来源：http://www.blog.zdbjq.cn/Article/details/gexvmbxap.sHtML

"autoload": { "psr-4": { "App\\": "src/" } }
来源：http://www.m.share.hesvh.cn/Article/details/ghyfurukl.sHtML

[U43] PHP：声明命名空间
来源：http://mobile.zdbjq.cn/Article/details/gvpffjwki.sHtML

namespace App\Http;
来源：http://read.share.fehbvm.com/Article/details/gvlgmxiee.sHtML

[U44] PHP：开启严格类型
来源：http://www.blog.zdbjq.cn/Article/details/gzcetrnbk.sHtML

declare(strict_types=1);
来源：http://wap.hesvh.cn/Article/details/gzrloahps.sHtML

[U45] PHP：类型声明与返回类型
来源：http://read.share.hesvh.cn/Article/details/gktfyjhgt.sHtML

function add(int $a, int $b): int { return $a + $b; }
来源：http://m.share.fehbvm.com/Article/details/goovmcmat.sHtML

[U46] PHP：可空类型
来源：http://www.blog.hesvh.cn/Article/details/gmgixafuw.sHtML

?string $name = null
来源：http://wap.fehbvm.com/Article/details/gfheraudi.sHtML

[U47] PHP：联合类型
来源：http://baike.zdbjq.cn/Article/details/gkzlpjfnr.sHtML

int|string $id
来源：http://baike.fehbvm.com/Article/details/gpsvjwhfq.sHtML

[U48] PHP：纯枚举
来源：http://blog.zdbjq.cn/Article/details/gyjfsbjog.sHtML

enum Status: string { case Active = "active"; case Off = "off"; }
来源：http://wap.zdbjq.cn/Article/details/gatthmodn.sHtML

[U49] PHP：只读属性
来源：http://baike.hesvh.cn/Article/details/gnaaxatky.sHtML

public readonly string $name
来源：http://read.share.zdbjq.cn/Article/details/gtqlzrzec.sHtML

[U50] PHP：构造器属性提升
来源：http://3g.hesvh.cn/Article/details/gpmjyguoi.sHtML

public function __construct(private int $id) {}
来源：http://wap.fehbvm.com/Article/details/gpugooigi.sHtML

[U51] PHP：数组解构
来源：http://www.share.hesvh.cn/Article/details/gweyzuqbb.sHtML

[$a, $b] = $arr;
来源：http://read.share.fehbvm.com/Article/details/gmnwtyads.sHtML

[U52] PHP：箭头函数
来源：http://baike.hesvh.cn/Article/details/gnhnxstxx.sHtML

$double = fn($x) => $x * 2;
来源：http://baike.hesvh.cn/Article/details/gdpsqoxxy.sHtML

[U53] PHP：空合并运算符
来源：http://wap.fehbvm.com/Article/details/gsndvcxdp.sHtML

$v = $a ?? $b ?? "default";
来源：http://blog.hesvh.cn/Article/details/gnussgjwo.sHtML

[U54] PHP：空安全调用
来源：http://3g.fehbvm.com/Article/details/gvlpafcpy.sHtML

$obj?->method()
来源：http://www.m.share.hesvh.cn/Article/details/ghuttvoja.sHtML

[U55] PHP：match 表达式
来源：http://3g.zdbjq.cn/Article/details/gynrzeved.sHtML

$s = match($x) { 1 => "一", default => "其他" };
来源：http://www.share.zdbjq.cn/Article/details/gjywnrhdu.sHtML

[U56] PHP：命名参数
来源：http://m.share.fehbvm.com/Article/details/gxjzgwcig.sHtML

f(a: 1, b: 2)
来源：http://mobile.fehbvm.com/Article/details/gjnlskdyy.sHtML

[U57] PHP：字符串插值
来源：http://blog.zdbjq.cn/Article/details/gezczlbdt.sHtML

"值: {$a}"
来源：http://wap.zdbjq.cn/Article/details/ghgvffsiv.sHtML

[U58] PHP：数组三件套
来源：http://read.share.hesvh.cn/Article/details/gygoqtucc.sHtML

array_map($f, $a);  array_filter($a, $f);  array_reduce($a, $f, 0);
来源：http://wap.hesvh.cn/Article/details/gycpxstld.sHtML

[U59] PHP：自定义排序
来源：http://read.share.zdbjq.cn/Article/details/ghsmcaxgg.sHtML

usort($arr, fn($a, $b) => $a["age"] <=> $b["age"]);
来源：http://baike.hesvh.cn/Article/details/gddtdqxuj.sHtML

[U60] PHP：JSON 编解码
来源：http://3g.zdbjq.cn/Article/details/gfipjnasp.sHtML

json_encode($d, JSON_UNESCAPED_UNICODE);  json_decode($s, true);
来源：http://baike.fehbvm.com/Article/details/gkinxctrv.sHtML

[U61] PHP：正则
来源：http://m.share.zdbjq.cn/Article/details/gspecouyq.sHtML

preg_match('/(\d+)/', $s, $m);  preg_replace('/\d+/', '#', $s);
来源：http://www.blog.zdbjq.cn/Article/details/gosckychc.sHtML

[U62] PHP：日期对象
来源：http://www.share.hesvh.cn/Article/details/ggdglhorb.sHtML

(new DateTimeImmutable())->format("Y-m-d");
来源：http://www.share.fehbvm.com/Article/details/gumkieaqu.sHtML

[U63] PHP：文件读写
来源：http://mobile.zdbjq.cn/Article/details/ghbxsodow.sHtML

file_get_contents($f);  file_put_contents($f, $data);
来源：http://baike.fehbvm.com/Article/details/grykzdmpx.sHtML

[U64] PHP：目录遍历
来源：http://wap.zdbjq.cn/Article/details/glquncsgc.sHtML

glob("dir/*.php");  scandir("dir");
来源：http://wap.zdbjq.cn/Article/details/genarglyo.sHtML

[U65] PHP：会话
来源：http://m.share.hesvh.cn/Article/details/gfkipaame.sHtML

session_start();  $_SESSION["uid"] = 1;
来源：http://3g.fehbvm.com/Article/details/gjnlzhfkv.sHtML

[U66] PHP：设置 Cookie
来源：http://www.share.zdbjq.cn/Article/details/grpwimknr.sHtML

setcookie("token", $v, ["httponly" => true, "samesite" => "Lax"]);
来源：http://blog.fehbvm.com/Article/details/gslemxzuq.sHtML

[U67] PHP：处理文件上传
来源：http://3g.zdbjq.cn/Article/details/glzhihmgw.sHtML

$_FILES["file"]["tmp_name"] 与 move_uploaded_file()
来源：http://www.m.share.zdbjq.cn/Article/details/gwuhjgkzj.sHtML

[U68] PHP：PDO 连接
来源：http://mobile.hesvh.cn/Article/details/gmuxqdmat.sHtML

$pdo = new PDO("mysql:host=localhost;dbname=app", "root", "");
来源：http://www.blog.zdbjq.cn/Article/details/galaqfcya.sHtML

[U69] PHP：PDO 预处理
来源：http://www.blog.fehbvm.com/Article/details/glilpkbjr.sHtML

$stmt = $pdo->prepare("SELECT * FROM users WHERE id = ?");  $stmt->execute([$id]);
来源：http://3g.fehbvm.com/Article/details/gjzvmblbo.sHtML

[U70] PHP：PDO 事务
来源：http://mobile.hesvh.cn/Article/details/guhmwfwya.sHtML

$pdo->beginTransaction();  $pdo->commit();  $pdo->rollBack();
来源：http://wap.fehbvm.com/Article/details/gxdlpsxwg.sHtML

[U71] PHP：抛出异常
来源：http://mobile.hesvh.cn/Article/details/gqwuujqmz.sHtML

throw new RuntimeException("失败", 500);
来源：http://baike.fehbvm.com/Article/details/gpnwoiojs.sHtML

[U72] PHP：写错误日志
来源：http://blog.fehbvm.com/Article/details/gvemoezfo.sHtML

error_log("失败: " . $e->getMessage());
来源：http://3g.zdbjq.cn/Article/details/gemxmipvn.sHtML

[U73] PHP：读取 ini 配置
来源：http://www.share.fehbvm.com/Article/details/gfkrkzhpr.sHtML

parse_ini_file("config.ini", true)
来源：http://3g.fehbvm.com/Article/details/ggxkzofmj.sHtML

[U74] PHP：读取环境变量
来源：http://read.share.zdbjq.cn/Article/details/gtvtkuwfb.sHtML

getenv("APP_ENV") ?: "production"
来源：http://mobile.hesvh.cn/Article/details/gaiqbqshg.sHtML

[U75] PHP：依赖注入
来源：http://3g.zdbjq.cn/Article/details/gcqrjqipz.sHtML

composer require psr/container
来源：http://mobile.hesvh.cn/Article/details/gqncotqgr.sHtML

[U76] PHP：简单路由
来源：http://www.share.zdbjq.cn/Article/details/gdzfdovqh.sHtML

$path = parse_url($_SERVER["REQUEST_URI"], PHP_URL_PATH);
来源：http://www.m.share.hesvh.cn/Article/details/gjldjrxqr.sHtML

[U77] PHP：模板渲染
来源：http://read.share.zdbjq.cn/Article/details/gvashmpqn.sHtML

composer require twig/twig
来源：http://baike.fehbvm.com/Article/details/gbrslfztj.sHtML

[U78] PHP：单元测试
来源：http://mobile.zdbjq.cn/Article/details/gbzhpdtpi.sHtML

composer require --dev phpunit/phpunit
来源：http://blog.fehbvm.com/Article/details/gtqociddp.sHtML

[U79] PHP：静态分析
来源：http://m.share.zdbjq.cn/Article/details/gxguyvuww.sHtML

composer require --dev phpstan/phpstan
来源：http://wap.fehbvm.com/Article/details/gyvjagmcq.sHtML

[U80] PHP：代码规范修复
来源：http://baike.fehbvm.com/Article/details/gehxqoxez.sHtML

composer require --dev friendsofphp/php-cs-fixer
来源：http://mobile.fehbvm.com/Article/details/gengglpiw.sHtML

[U81] JS：初始化项目
来源：http://read.share.hesvh.cn/Article/details/gndecteey.sHtML

npm init -y;  npm i express
来源：http://www.share.zdbjq.cn/Article/details/gtmkzybgs.sHtML

[U82] JS：package.json 脚本
来源：http://blog.zdbjq.cn/Article/details/gyrhnmdku.sHtML

"scripts": { "dev": "vite", "build": "vite build" }
来源：http://blog.hesvh.cn/Article/details/gacrjcmxu.sHtML

[U83] JS：ES Module 导入导出
来源：http://3g.hesvh.cn/Article/details/gsuykzfek.sHtML

export const a = 1;  import { a } from "./m.js";
来源：http://m.share.hesvh.cn/Article/details/gzlautpkc.sHtML

[U84] JS：CommonJS 写法
来源：http://3g.hesvh.cn/Article/details/glvmshirw.sHtML

module.exports = { a };  const { a } = require("./m");
来源：http://www.share.hesvh.cn/Article/details/gskzrarjj.sHtML

[U85] JS：可选链
来源：http://blog.hesvh.cn/Article/details/gcixmqtel.sHtML

a?.b?.c
来源：http://m.share.fehbvm.com/Article/details/gaelbnewe.sHtML

[U86] JS：空值合并
来源：http://www.blog.hesvh.cn/Article/details/gznvfnarl.sHtML

a ?? b
来源：http://www.share.hesvh.cn/Article/details/gbtjkcfqi.sHtML

[U87] JS：解构默认值
来源：http://baike.hesvh.cn/Article/details/gdqfjvdwh.sHtML

const { a = 1, b = 2 } = obj;
来源：http://read.share.hesvh.cn/Article/details/glhinzyas.sHtML

[U88] JS：对象展开合并
来源：http://www.blog.fehbvm.com/Article/details/gnzlecfnb.sHtML

{ ...a, ...b }
来源：http://wap.fehbvm.com/Article/details/guhurhdbd.sHtML

[U89] JS：数组去重
来源：http://blog.hesvh.cn/Article/details/gozgdphzw.sHtML

[...new Set(arr)]
来源：http://3g.zdbjq.cn/Article/details/ggodhfkil.sHtML

[U90] JS：数字数组排序
来源：http://mobile.fehbvm.com/Article/details/guyztxumm.sHtML

[...arr].sort((a, b) => a - b)
来源：http://mobile.hesvh.cn/Article/details/gflqchzem.sHtML

[U91] JS：对象键值遍历
来源：http://m.share.hesvh.cn/Article/details/gpxodimkw.sHtML

Object.entries(obj).forEach(([k, v]) => {});
来源：http://mobile.fehbvm.com/Article/details/gcprpvpmg.sHtML

[U92] JS：深拷贝
来源：http://read.share.zdbjq.cn/Article/details/gwglisqvf.sHtML

structuredClone(obj)
来源：http://blog.hesvh.cn/Article/details/gbkbsfbzu.sHtML

[U93] JS：模板字符串
来源：http://m.share.hesvh.cn/Article/details/gfzpzjkaq.sHtML

`共 ${n} 条`
来源：http://read.share.hesvh.cn/Article/details/gxzoafmdw.sHtML

[U94] JS：箭头函数
来源：http://m.share.hesvh.cn/Article/details/gbeiftayw.sHtML

const double = x => x * 2;
来源：http://blog.fehbvm.com/Article/details/gimlarncs.sHtML

[U95] JS：Promise 包装
来源：http://www.blog.zdbjq.cn/Article/details/gdgrnkerl.sHtML

new Promise((resolve, reject) => {})
来源：http://mobile.zdbjq.cn/Article/details/gxbngzzyy.sHtML

[U96] JS：async/await 与异常
来源：http://www.m.share.zdbjq.cn/Article/details/gybgnwwyu.sHtML

try { const d = await f(); } catch (e) { console.error(e); }
来源：http://www.share.zdbjq.cn/Article/details/gllfzeczi.sHtML

[U97] JS：并发请求
来源：http://www.m.share.zdbjq.cn/Article/details/guxcxbuom.sHtML

await Promise.all(urls.map(u => fetch(u)))
来源：http://3g.zdbjq.cn/Article/details/gktijeltd.sHtML

[U98] JS：fetch 带 JSON
来源：http://www.blog.fehbvm.com/Article/details/gmizydvyl.sHtML

await fetch(url, { method: "POST", headers: { "Content-Type": "application/json" }, body: JSON.stringify(d) })
来源：http://www.blog.fehbvm.com/Article/details/gnvzokjag.sHtML

[U99] JS：事件监听
来源：http://www.share.zdbjq.cn/Article/details/gafuynqyd.sHtML

el.addEventListener("click", e => {})
来源：http://blog.hesvh.cn/Article/details/gljmftzlw.sHtML

[U100] JS：DOM 查询
来源：http://blog.hesvh.cn/Article/details/gzvulaztl.sHtML

document.querySelector(".item")
来源：http://3g.fehbvm.com/Article/details/gybaphwyw.sHtML

[U101] JS：classList 操作
来源：http://m.share.fehbvm.com/Article/details/gecmhmvpy.sHtML

el.classList.toggle("active")
来源：http://3g.fehbvm.com/Article/details/gtqhudgmt.sHtML

[U102] JS：本地存储
来源：http://www.m.share.fehbvm.com/Article/details/gbbnjrmvb.sHtML

localStorage.setItem("k", JSON.stringify(v))
来源：http://mobile.zdbjq.cn/Article/details/gxwyzndls.sHtML

[U103] JS：定时器
来源：http://www.share.hesvh.cn/Article/details/gfryawxoi.sHtML

setTimeout(fn, 1000);  setInterval(fn, 1000);
来源：http://www.share.fehbvm.com/Article/details/gcfqwdqjf.sHtML

[U104] JS：防抖
来源：http://www.blog.zdbjq.cn/Article/details/gyyktduiq.sHtML

const debounce = (fn, ms) => { let t; return (...a) => { clearTimeout(t); t = setTimeout(() => fn(...a), ms); }; };
来源：http://blog.hesvh.cn/Article/details/gbgzzrgjz.sHtML

[U105] JS：节流
来源：http://www.blog.zdbjq.cn/Article/details/gcdqgiicy.sHtML

const throttle = (fn, ms) => { let last = 0; return (...a) => { const n = Date.now(); if (n - last >= ms) { last = n; fn(...a); } }; };
来源：http://m.share.hesvh.cn/Article/details/gazirkslw.sHtML

[U106] JS：日期格式化
来源：http://baike.fehbvm.com/Article/details/gtjpplkau.sHtML

new Intl.DateTimeFormat("zh-CN", { dateStyle: "medium" }).format(new Date())
来源：http://www.blog.hesvh.cn/Article/details/gkuulcoyb.sHtML

[U107] JS：数字千分位
来源：http://wap.hesvh.cn/Article/details/gaoqxktqu.sHtML

new Intl.NumberFormat("en-US").format(1234567)
来源：http://m.share.hesvh.cn/Article/details/gmscqllkh.sHtML

[U108] JS：随机整数
来源：http://www.share.hesvh.cn/Article/details/ghsuykkzh.sHtML

Math.floor(Math.random() * (max - min + 1)) + min
来源：http://www.share.zdbjq.cn/Article/details/gruykzmgd.sHtML

[U109] JS：数组分组
来源：http://www.blog.fehbvm.com/Article/details/gryleqboe.sHtML

Object.groupBy(arr, x => x.type)
来源：http://read.share.hesvh.cn/Article/details/gspmtbgyp.sHtML

[U110] JS：数组分块
来源：http://www.blog.zdbjq.cn/Article/details/gegiriwmb.sHtML

arr.reduce((acc, x, i) => (i % size ? acc : [...acc, arr.slice(i, i + size)]), [])
来源：http://3g.fehbvm.com/Article/details/gpelbspgi.sHtML

[U111] JS：对象转 Map
来源：http://www.blog.hesvh.cn/Article/details/glnulcwnk.sHtML

new Map(Object.entries(obj))
来源：http://www.m.share.zdbjq.cn/Article/details/giygdbbml.sHtML

[U112] JS：字符串补位
来源：http://baike.hesvh.cn/Article/details/gilfxrrej.sHtML

"7".padStart(3, "0")
来源：http://baike.zdbjq.cn/Article/details/gmbgfjcre.sHtML

[U113] JS：正则替换全部
来源：http://www.blog.hesvh.cn/Article/details/gpnjhqvrt.sHtML

s.replaceAll("a", "b")
来源：http://baike.zdbjq.cn/Article/details/gaiqnfkhz.sHtML

[U114] JS：JSON 深比较
来源：http://wap.fehbvm.com/Article/details/glajxhjse.sHtML

JSON.stringify(a) === JSON.stringify(b)
来源：http://www.blog.zdbjq.cn/Article/details/gitwqercw.sHtML

[U115] JS：生成 UUID
来源：http://baike.zdbjq.cn/Article/details/gecjjbzvq.sHtML

crypto.randomUUID()
来源：http://3g.zdbjq.cn/Article/details/gvsgvwjpf.sHtML

[U116] JS：类型检查（JSDoc）
来源：http://www.m.share.fehbvm.com/Article/details/gjypttvii.sHtML

/** @param {string} name */ function f(name) {}
来源：http://read.share.fehbvm.com/Article/details/golyugrjl.sHtML

[U117] JS：单元测试
来源：http://mobile.hesvh.cn/Article/details/gccrchcmg.sHtML

npm i -D vitest;  npx vitest
来源：http://read.share.zdbjq.cn/Article/details/gczfqakec.sHtML

[U118] JS：开发服务器
来源：http://www.m.share.fehbvm.com/Article/details/gobzawrfy.sHtML

npm i -D vite;  npx vite
来源：http://www.m.share.fehbvm.com/Article/details/gmrdpngbr.sHtML

[U119] JS：生产构建
来源：http://mobile.zdbjq.cn/Article/details/gzrhsntos.sHtML

npx vite build
来源：http://mobile.fehbvm.com/Article/details/guwxqgxfw.sHtML

[U120] JS：读取环境变量（Vite）
来源：http://blog.fehbvm.com/Article/details/gkvdgywxt.sHtML

import.meta.env.VITE_API_URL
来源：http://blog.fehbvm.com/Article/details/gsakhoosk.sHtML

================================================================================
来源：http://3g.zdbjq.cn/Article/details/gdhrfvwte.sHtML

统计汇总
来源：http://blog.zdbjq.cn/Article/details/gzaekgxww.sHtML

================================================================================
来源：http://read.share.hesvh.cn/Article/details/geibihsud.sHtML

按语言统计（条）：
来源：http://blog.hesvh.cn/Article/details/gfoukpcio.sHtML

Python ......... 252
来源：http://mobile.zdbjq.cn/Article/details/gvhrdxfgl.sHtML

PHP ............ 252
来源：http://wap.zdbjq.cn/Article/details/gvplndhsd.sHtML

JavaScript ..... 252
来源：http://www.m.share.hesvh.cn/Article/details/gyiytobts.sHtML

TypeScript ..... 212
来源：http://m.share.hesvh.cn/Article/details/glidejdjl.sHtML

Java ........... 212
来源：http://read.share.zdbjq.cn/Article/details/gjavaxvtd.sHtML

Go ............. 212
来源：http://www.share.fehbvm.com/Article/details/gplfxesqu.sHtML

Ruby ........... 212
来源：http://blog.hesvh.cn/Article/details/gbcfgxsch.sHtML

C# ............. 212
来源：http://read.share.zdbjq.cn/Article/details/gepdavehs.sHtML

C .............. 30
来源：http://www.share.zdbjq.cn/Article/details/glcdednip.sHtML

C++ ............ 30
来源：http://baike.fehbvm.com/Article/details/ggahwyusp.sHtML

SQL ............ 90
来源：http://www.m.share.fehbvm.com/Article/details/gsqdhnoqk.sHtML

Bash ........... 80
来源：http://3g.hesvh.cn/Article/details/gtgfksiqh.sHtML

Kotlin ......... 15
来源：http://blog.hesvh.cn/Article/details/ggoflbwdu.sHtML

Swift .......... 15
来源：http://mobile.fehbvm.com/Article/details/gewzfsive.sHtML

Lua ............ 10
来源：http://wap.fehbvm.com/Article/details/gdsfemxmf.sHtML

Perl ........... 10
来源：http://mobile.hesvh.cn/Article/details/gcxyyzefn.sHtML

Scala .......... 10
来源：http://www.m.share.zdbjq.cn/Article/details/gikbixaek.sHtML

------------------------------------
来源：http://read.share.hesvh.cn/Article/details/ggminlofi.sHtML

合计 ........... 2106 条
来源：http://m.share.zdbjq.cn/Article/details/grgclycry.sHtML

按章节统计：
来源：http://mobile.fehbvm.com/Article/details/grfynqcpq.sHtML

A 基础语法与类型       26 个任务 × 8 语言 =  208
来源：http://mobile.zdbjq.cn/Article/details/gwsrukdjm.sHtML

B 流程控制             16 个任务 × 8 语言 =  128
来源：http://mobile.fehbvm.com/Article/details/gmrzzbwde.sHtML

C 函数与作用域         16 个任务 × 8 语言 =  128
来源：http://mobile.hesvh.cn/Article/details/gjrtayulj.sHtML

D 数组 / 列表 / 集合   26 个任务 × 8 语言 =  208
来源：http://wap.hesvh.cn/Article/details/gmodpouoj.sHtML

E 字符串处理           22 个任务 × 8 语言 =  176
来源：http://wap.hesvh.cn/Article/details/grdnbefsu.sHtML

F 文件与目录           12 个任务 × 8 语言 =   96
来源：http://mobile.fehbvm.com/Article/details/gwdzxkmfw.sHtML

G 面向对象             16 个任务 × 8 语言 =  128
来源：http://www.blog.fehbvm.com/Article/details/gyfhjzdlz.sHtML

H 异常与错误处理       10 个任务 × 8 语言 =   80
来源：http://mobile.zdbjq.cn/Article/details/gitxlokvz.sHtML

I 正则表达式            8 个任务 × 8 语言 =   64
来源：http://3g.hesvh.cn/Article/details/gaxtrhkhr.sHtML

J 日期与时间           10 个任务 × 8 语言 =   80
来源：http://www.blog.fehbvm.com/Article/details/gsxdgenks.sHtML

K JSON 与序列化         8 个任务 × 8 语言 =   64
来源：http://www.blog.fehbvm.com/Article/details/glwbunttg.sHtML

L 网络请求              8 个任务 × 8 语言 =   64
来源：http://m.share.fehbvm.com/Article/details/gpzrtawdf.sHtML

M 命令行 / 进程         8 个任务 × 8 语言 =   64
来源：http://blog.fehbvm.com/Article/details/gvtozbbij.sHtML

N 数据结构与算法       12 个任务 × 8 语言 =   96
来源：http://www.blog.fehbvm.com/Article/details/ghrqpplkd.sHtML

O 并发与异步            6 个任务 × 8 语言 =   48
来源：http://m.share.fehbvm.com/Article/details/gibzrnheg.sHtML

P 常用工具函数          8 个任务 × 8 语言 =   64
来源：http://mobile.hesvh.cn/Article/details/gpswlrswf.sHtML

Q SQL 专题                              90
来源：http://read.share.zdbjq.cn/Article/details/gxisiwrhc.sHtML

R Bash 专题                             80
来源：http://baike.zdbjq.cn/Article/details/gmgmrhbqr.sHtML

S C / C++ 专题                          60
来源：http://m.share.hesvh.cn/Article/details/gjiamkawx.sHtML

T 其他语言补充                          60
来源：http://read.share.fehbvm.com/Article/details/gdsmhjtrd.sHtML

U 高频实用片段                         120
来源：http://mobile.hesvh.cn/Article/details/gojyyngnn.sHtML

------------------------------------
来源：http://wap.fehbvm.com/Article/details/govvrebcc.sHtML

合计                                  2106 条
来源：http://baike.hesvh.cn/Article/details/gyjhugcbg.sHtML

--------------------------------------------------------------------------------
来源：http://m.share.hesvh.cn/Article/details/gxpwnxutb.sHtML

使用提醒
来源：http://www.share.hesvh.cn/Article/details/gbwoqnbja.sHtML

--------------------------------------------------------------------------------
来源：http://mobile.hesvh.cn/Article/details/ggzoqnkrn.sHtML

1. 示例追求"最小可用"，正式项目中请补齐导入、错误处理与边界判断。
来源：http://wap.fehbvm.com/Article/details/giyzltbls.sHtML

2. 涉及文件、网络、数据库的示例，注意资源释放与异常捕获。
来源：http://blog.fehbvm.com/Article/details/goahkuvup.sHtML

3. 语言版本差异较大（如 Python 3.10 的 match、Java 17 的 record/switch 箭头），
来源：http://www.blog.zdbjq.cn/Article/details/gfmswxzke.sHtML

在旧版本上使用前请先确认语法支持情况。
来源：http://baike.zdbjq.cn/Article/details/gtyxjqcds.sHtML

4. 标注"手写"的条目是因为该语言缺少对应内置能力，实际项目中可引入成熟库。
来源：http://read.share.zdbjq.cn/Article/details/gcqldjjtt.sHtML

—— 文件结束 ——
来源：http://3g.fehbvm.com/Article/details/ghcfmidqr.sHtML

================================================================================
来源：http://baike.hesvh.cn/Article/details/gzjxfoxop.sHtML

程序语言常见例子速查手册（2024 版）
来源：http://mobile.hesvh.cn/Article/details/giayvkxkj.sHtML

Common Programming Examples Cheat Book
来源：http://blog.fehbvm.com/Article/details/grbcgmctr.sHtML

================================================================================
来源：http://www.blog.fehbvm.com/Article/details/gdxgqutbw.sHtML

【收录内容】
来源：http://read.share.fehbvm.com/Article/details/getzvfkov.sHtML

覆盖 12 种语言 / 语法与常见 API：
来源：http://baike.fehbvm.com/Article/details/gqrrmtxdn.sHtML

Python · PHP · JavaScript · TypeScript · Java · Go · Ruby · C#
来源：http://baike.zdbjq.cn/Article/details/gymlafanz.sHtML

SQL · Bash · C · C++
来源：http://mobile.fehbvm.com/Article/details/gydkqiixp.sHtML

按「任务」分组：每个任务下按语言各给出一条最小可用示例。
来源：http://wap.zdbjq.cn/Article/details/gchoggjws.sHtML

【使用说明】
来源：http://www.m.share.hesvh.cn/Article/details/gylcxpyqr.sHtML

1. 每个任务形如 "[编号] 任务名"，下面每行以语言标记开头：
来源：http://www.blog.zdbjq.cn/Article/details/gliokqjvb.sHtML

Py:    Python        PHP:   PHP           JS:    JavaScript
来源：http://wap.fehbvm.com/Article/details/gljoevquf.sHtML

TS:    TypeScript    Java:  Java          Go:    Go
来源：http://www.m.share.hesvh.cn/Article/details/gdmvkoabs.sHtML

Ruby:  Ruby          C#:    C#            SQL:   SQL
来源：http://baike.zdbjq.cn/Article/details/gjtenkeyo.sHtML

Bash:  Shell         C:     C             C++:   C++
来源：http://3g.fehbvm.com/Article/details/glqoxmvuz.sHtML

2. 示例只展示核心写法，刻意省略 import / require / include / using 等样板代码。
来源：http://3g.fehbvm.com/Article/details/gclggacqa.sHtML

需要完整可运行文件时，请自行补齐当前语言的导入语句。
来源：http://baike.zdbjq.cn/Article/details/ganvlqfnu.sHtML

3. 语法基准：Python 3.10+ / PHP 8.1+ / ES2020+ / TypeScript 5 / Java 17 /
来源：http://m.share.hesvh.cn/Article/details/gxpzchmjf.sHtML

Go 1.21+ / Ruby 3.x / C# 10+ / C17 / C++17。
来源：http://baike.zdbjq.cn/Article/details/gbhmzrebh.sHtML

4. 检索建议：用编辑器或浏览器 Ctrl+F 搜关键词，如 "排序" "读取文件" "正则"。
来源：http://3g.zdbjq.cn/Article/details/gxznxdbgu.sHtML

5. 标记为 "// 无" 表示该语言没有对应的一等语法，需用替代写法（示例给出替代方案）。
来源：http://blog.fehbvm.com/Article/details/gnhbazkeo.sHtML

6. 符号 "⏎" 表示代码在此处换行（主要用于 Python 等强制缩进、无法压成一行的结构）。
来源：http://3g.hesvh.cn/Article/details/gawsuvvsj.sHtML

【文件统计】
来源：http://www.blog.hesvh.cn/Article/details/ghewrodox.sHtML

语言示例共 2106 条，分布见本文末尾的「统计汇总」。
来源：http://3g.zdbjq.cn/Article/details/gexlxapjy.sHtML

--------------------------------------------------------------------------------
来源：http://blog.fehbvm.com/Article/details/gngroulcc.sHtML

目  录
来源：http://baike.hesvh.cn/Article/details/gvtjouayf.sHtML

--------------------------------------------------------------------------------
来源：http://www.blog.hesvh.cn/Article/details/gikybgpik.sHtML

A. 基础语法与类型              （第 1 节，26 个任务，208 条）
来源：http://baike.zdbjq.cn/Article/details/gvzudjzpp.sHtML

B. 流程控制                    （第 2 节，16 个任务，128 条）
来源：http://www.blog.hesvh.cn/Article/details/grughczwr.sHtML

C. 函数与作用域                （第 3 节，16 个任务，128 条）
来源：http://read.share.zdbjq.cn/Article/details/gsupxsjbl.sHtML

D. 数组 / 列表 / 集合          （第 4 节，26 个任务，208 条）
来源：http://3g.fehbvm.com/Article/details/gwpqxznkw.sHtML

E. 字符串处理                  （第 5 节，22 个任务，176 条）
来源：http://3g.hesvh.cn/Article/details/gnubycgwb.sHtML


<!-- 参考信息 -->