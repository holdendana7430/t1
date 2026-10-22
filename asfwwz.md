代发 wailian999

[U11] Py：生成器表达式
来源：http://www.52xcode.cn/Article/details/gt2awbzfdmz.html

(x * 2 for x in arr)
来源：http://www.ydjk.org.cn/Article/details/gt2yvlnrzus.html

[U12] Py：取出现最多的 3 个元素
来源：http://www.52xcode.cn/Article/details/gt2bnzvsjoy.html

Counter(arr).most_common(3)
来源：http://www.ydjk.org.cn/Article/details/gt2qallxesm.html

[U13] Py：固定长度队列
来源：http://www.ydjk.org.cn/Article/details/gt2flpirfmp.html

deque(maxlen=10)
来源：http://www.ydjk.org.cn/Article/details/gt2sqhqagjr.html

[U14] Py：分组收集到列表
来源：http://www.ydjk.org.cn/Article/details/gt2neptyafp.html

defaultdict(list)
来源：http://www.52xcode.cn/Article/details/gt2rictioda.html

[U15] Py：高精度计时
来源：http://www.52xcode.cn/Article/details/gt2oyfociog.html

t = time.perf_counter()
来源：http://www.52xcode.cn/Article/details/gt2dtnrqqnj.html

[U16] Py：命令行参数解析
来源：http://www.ydjk.org.cn/Article/details/gt2fpkxvrpx.html

ap = argparse.ArgumentParser();  ap.add_argument("--name");  args = ap.parse_args()
来源：http://www.ydjk.org.cn/Article/details/gt2qrjrbcoo.html

[U17] Py：初始化日志
来源：http://www.ydjk.org.cn/Article/details/gt2tkyimons.html

logging.basicConfig(level=logging.INFO)
来源：http://www.52xcode.cn/Article/details/gt2fcalpvis.html

[U18] Py：预编译正则
来源：http://www.ydjk.org.cn/Article/details/gt2gtanpncj.html

pat = re.compile(r"\d+")
来源：http://www.52xcode.cn/Article/details/gt2rxmygtxm.html

[U19] Py：正则替换带回调
来源：http://www.ydjk.org.cn/Article/details/gt2mtoriqqp.html

re.sub(r"\d+", lambda m: str(int(m.group()) * 2), s)
来源：http://www.ydjk.org.cn/Article/details/gt2tfcbqgyz.html

[U20] Py：缓存函数结果
来源：http://www.ydjk.org.cn/Article/details/gt2ztijtlao.html

@functools.lru_cache(maxsize=None)
来源：http://www.ydjk.org.cn/Article/details/gt2hlwxqtau.html

[U21] Py：自定义上下文管理器
来源：http://www.ydjk.org.cn/Article/details/gt2zulpzszh.html

@contextlib.contextmanager
来源：http://www.ydjk.org.cn/Article/details/gt2vapzlcda.html

[U22] Py：矩阵转置
来源：http://www.ydjk.org.cn/Article/details/gt2nrqswowx.html

list(zip(*m))
来源：http://www.ydjk.org.cn/Article/details/gt2zewncroq.html

[U23] Py：分块读取大文件
来源：http://www.ydjk.org.cn/Article/details/gt2hfqibimd.html

for chunk in iter(lambda: f.read(8192), b""):
来源：http://www.52xcode.cn/Article/details/gt2ijkhjnyl.html

[U24] Py：路径操作
来源：http://www.ydjk.org.cn/Article/details/gt2nvlqtwwu.html

Path("a/b.txt").parent.mkdir(parents=True, exist_ok=True)
来源：http://www.ydjk.org.cn/Article/details/gt2urarttgu.html

[U25] Py：CSV 按字典读
来源：http://www.52xcode.cn/Article/details/gt2gtbehnfh.html

csv.DictReader(f)
来源：http://www.ydjk.org.cn/Article/details/gt2vwgxamwk.html

[U26] Py：并发下载
来源：http://www.ydjk.org.cn/Article/details/gt2bzexvwjh.html

ThreadPoolExecutor(max_workers=8).map(fetch, urls)
来源：http://www.52xcode.cn/Article/details/gt2xllbcebw.html

[U27] Py：异步 HTTP
来源：http://www.52xcode.cn/Article/details/gt2xqncefzg.html

aiohttp.ClientSession() 配合 async with
来源：http://www.ydjk.org.cn/Article/details/gt2xcpkcoeg.html

[U28] Py：类型别名
来源：http://www.ydjk.org.cn/Article/details/gt2hwraujsw.html

UserId = int
来源：http://www.52xcode.cn/Article/details/gt2pkpjczxp.html

[U29] Py：属性校验
来源：http://www.ydjk.org.cn/Article/details/gt2fmttlzkd.html

@property 与 @x.setter 配合
来源：http://www.ydjk.org.cn/Article/details/gt2eorqswzx.html

[U30] Py：数据类
来源：http://www.52xcode.cn/Article/details/gt2rdukxcsa.html

@dataclass(slots=True)
来源：http://www.52xcode.cn/Article/details/gt2ezycynoo.html

[U31] Py：单测
来源：http://www.52xcode.cn/Article/details/gt2uvbelwza.html

python -m pytest -q
来源：http://www.ydjk.org.cn/Article/details/gt2lkvyzcwq.html

[U32] Py：代码格式化
来源：http://www.52xcode.cn/Article/details/gt2cxylbcft.html

ruff format . && ruff check --fix .
来源：http://www.52xcode.cn/Article/details/gt2zwukpbsx.html

[U33] Py：打包发布
来源：http://www.52xcode.cn/Article/details/gt2rvbrrubu.html

python -m build  （依赖 pyproject.toml）
来源：http://www.ydjk.org.cn/Article/details/gt2azznvode.html

[U34] Py：判断编码
来源：http://www.52xcode.cn/Article/details/gt2anvpuscj.html

chardet.detect(raw)
来源：http://www.ydjk.org.cn/Article/details/gt2vmnxkark.html

[U35] Py：发送邮件
来源：http://www.52xcode.cn/Article/details/gt2anmewbip.html

smtplib.SMTP_SSL(...).send_message(msg)
来源：http://www.52xcode.cn/Article/details/gt2sfrcvtqr.html

[U36] Py：定时任务
来源：http://www.52xcode.cn/Article/details/gt2bbikyydu.html

schedule.every(10).minutes.do(job)
来源：http://www.52xcode.cn/Article/details/gt2cytpscep.html

[U37] Py：读写 Excel
来源：http://www.ydjk.org.cn/Article/details/gt2xqwozzin.html

pandas.read_excel / DataFrame.to_excel
来源：http://www.52xcode.cn/Article/details/gt2fxtbtsaw.html

[U38] Py：获取脚本所在目录
来源：http://www.ydjk.org.cn/Article/details/gt2qqaymxye.html

Path(__file__).resolve().parent
来源：http://www.52xcode.cn/Article/details/gt2nbhbxshz.html

[U39] Py：判断是否在交互环境
来源：http://www.52xcode.cn/Article/details/gt2vqtdpmsr.html

sys.stdout.isatty()
来源：http://www.ydjk.org.cn/Article/details/gt2uemdudco.html

[U40] Py：打印到标准错误
来源：http://www.ydjk.org.cn/Article/details/gt2oxeyvnsk.html

print("err", file=sys.stderr)
来源：http://www.ydjk.org.cn/Article/details/gt2hcvdriee.html

[U41] PHP：初始化 Composer 项目
来源：http://www.52xcode.cn/Article/details/gt2vwdimjdp.html

composer init;  composer require guzzlehttp/guzzle
来源：http://www.52xcode.cn/Article/details/gt2caeclnoy.html

[U42] PHP：PSR-4 自动加载
来源：http://www.52xcode.cn/Article/details/gt2cnvhmexo.html

"autoload": { "psr-4": { "App\\": "src/" } }
来源：http://www.52xcode.cn/Article/details/gt2qmnvvptm.html

[U43] PHP：声明命名空间
来源：http://www.52xcode.cn/Article/details/gt2eegayaxt.html

namespace App\Http;
来源：http://www.52xcode.cn/Article/details/gt2vcsemcij.html

[U44] PHP：开启严格类型
来源：http://www.ydjk.org.cn/Article/details/gt2zzuhvtnj.html

declare(strict_types=1);
来源：http://www.52xcode.cn/Article/details/gt2igclfral.html

[U45] PHP：类型声明与返回类型
来源：http://www.52xcode.cn/Article/details/gt2efbfzpkg.html

function add(int $a, int $b): int { return $a + $b; }
来源：http://www.52xcode.cn/Article/details/gt2tolegmvq.html

[U46] PHP：可空类型
来源：http://www.ydjk.org.cn/Article/details/gt2yiqilcpz.html

?string $name = null
来源：http://www.ydjk.org.cn/Article/details/gt2xbicforl.html

[U47] PHP：联合类型
来源：http://www.ydjk.org.cn/Article/details/gt2mnvcprcm.html

int|string $id
来源：http://www.ydjk.org.cn/Article/details/gt2lsmjaegb.html

[U48] PHP：纯枚举
来源：http://www.52xcode.cn/Article/details/gt2cciskynb.html

enum Status: string { case Active = "active"; case Off = "off"; }
来源：http://www.52xcode.cn/Article/details/gt2mrcugtwf.html

[U49] PHP：只读属性
来源：http://www.52xcode.cn/Article/details/gt2eezvrbfq.html

public readonly string $name
来源：http://www.ydjk.org.cn/Article/details/gt2getkmctb.html

[U50] PHP：构造器属性提升
来源：http://www.ydjk.org.cn/Article/details/gt2nsjsxyou.html

public function __construct(private int $id) {}
来源：http://www.52xcode.cn/Article/details/gt2ulburqjl.html

[U51] PHP：数组解构
来源：http://www.ydjk.org.cn/Article/details/gt2baaymbth.html

[$a, $b] = $arr;
来源：http://www.52xcode.cn/Article/details/gt2cupdsqsy.html

[U52] PHP：箭头函数
来源：http://www.ydjk.org.cn/Article/details/gt2avsxyvgq.html

$double = fn($x) => $x * 2;
来源：http://www.52xcode.cn/Article/details/gt2cadkcoha.html

[U53] PHP：空合并运算符
来源：http://www.ydjk.org.cn/Article/details/gt2ifnjqvxg.html

$v = $a ?? $b ?? "default";
来源：http://www.52xcode.cn/Article/details/gt2uyhzqtxa.html

[U54] PHP：空安全调用
来源：http://www.ydjk.org.cn/Article/details/gt2cwqzfcgs.html

$obj?->method()
来源：http://www.52xcode.cn/Article/details/gt2iprocbgr.html

[U55] PHP：match 表达式
来源：http://www.52xcode.cn/Article/details/gt2pkzfefai.html

$s = match($x) { 1 => "一", default => "其他" };
来源：http://www.ydjk.org.cn/Article/details/gt2yglvrztr.html

[U56] PHP：命名参数
来源：http://www.ydjk.org.cn/Article/details/gt2axvnayip.html

f(a: 1, b: 2)
来源：http://www.52xcode.cn/Article/details/gt2funvgctg.html

[U57] PHP：字符串插值
来源：http://www.ydjk.org.cn/Article/details/gt2ibascrga.html

"值: {$a}"
来源：http://www.ydjk.org.cn/Article/details/gt2zoomntro.html

[U58] PHP：数组三件套
来源：http://www.ydjk.org.cn/Article/details/gt2jqhfsyod.html

array_map($f, $a);  array_filter($a, $f);  array_reduce($a, $f, 0);
来源：http://www.ydjk.org.cn/Article/details/gt2ajylrlqi.html

[U59] PHP：自定义排序
来源：http://www.ydjk.org.cn/Article/details/gt2pgarnvkw.html

usort($arr, fn($a, $b) => $a["age"] <=> $b["age"]);
来源：http://www.52xcode.cn/Article/details/gt2bdsydfgk.html

[U60] PHP：JSON 编解码
来源：http://www.ydjk.org.cn/Article/details/gt2mhxrkhgt.html

json_encode($d, JSON_UNESCAPED_UNICODE);  json_decode($s, true);
来源：http://www.ydjk.org.cn/Article/details/gt2fcxvfqdx.html

[U61] PHP：正则
来源：http://www.52xcode.cn/Article/details/gt2ipnkyzre.html

preg_match('/(\d+)/', $s, $m);  preg_replace('/\d+/', '#', $s);
来源：http://www.ydjk.org.cn/Article/details/gt2jnnvfdxo.html

[U62] PHP：日期对象
来源：http://www.ydjk.org.cn/Article/details/gt2htjrlrgf.html

(new DateTimeImmutable())->format("Y-m-d");
来源：http://www.ydjk.org.cn/Article/details/gt2dytwpewo.html

[U63] PHP：文件读写
来源：http://www.52xcode.cn/Article/details/gt2wsghgtrf.html

file_get_contents($f);  file_put_contents($f, $data);
来源：http://www.52xcode.cn/Article/details/gt2nffbyamx.html

[U64] PHP：目录遍历
来源：http://www.ydjk.org.cn/Article/details/gt2gsoktvax.html

glob("dir/*.php");  scandir("dir");
来源：http://www.52xcode.cn/Article/details/gt2ukhyqvyn.html

[U65] PHP：会话
来源：http://www.52xcode.cn/Article/details/gt2sipfzgna.html

session_start();  $_SESSION["uid"] = 1;
来源：http://www.52xcode.cn/Article/details/gt2dvhjsyhg.html

[U66] PHP：设置 Cookie
来源：http://www.52xcode.cn/Article/details/gt2ugydscuc.html

setcookie("token", $v, ["httponly" => true, "samesite" => "Lax"]);
来源：http://www.52xcode.cn/Article/details/gt2vhzokwfx.html

[U67] PHP：处理文件上传
来源：http://www.ydjk.org.cn/Article/details/gt2zsduqelz.html

$_FILES["file"]["tmp_name"] 与 move_uploaded_file()
来源：http://www.ydjk.org.cn/Article/details/gt2xwajmmjl.html

[U68] PHP：PDO 连接
来源：http://www.ydjk.org.cn/Article/details/gt2xknvnzlk.html

$pdo = new PDO("mysql:host=localhost;dbname=app", "root", "");
来源：http://www.52xcode.cn/Article/details/gt2luccgrjb.html

[U69] PHP：PDO 预处理
来源：http://www.52xcode.cn/Article/details/gt2wjddqkqm.html

$stmt = $pdo->prepare("SELECT * FROM users WHERE id = ?");  $stmt->execute([$id]);
来源：http://www.ydjk.org.cn/Article/details/gt2nesmjhvb.html

[U70] PHP：PDO 事务
来源：http://www.ydjk.org.cn/Article/details/gt2chvhbzdv.html

$pdo->beginTransaction();  $pdo->commit();  $pdo->rollBack();
来源：http://www.ydjk.org.cn/Article/details/gt2vchmtjki.html

[U71] PHP：抛出异常
来源：http://www.ydjk.org.cn/Article/details/gt2hkokruqi.html

throw new RuntimeException("失败", 500);
来源：http://www.ydjk.org.cn/Article/details/gt2wnrxgrgt.html

[U72] PHP：写错误日志
来源：http://www.52xcode.cn/Article/details/gt2qgcqkdpz.html

error_log("失败: " . $e->getMessage());
来源：http://www.52xcode.cn/Article/details/gt2rgrfkypk.html

[U73] PHP：读取 ini 配置
来源：http://www.ydjk.org.cn/Article/details/gt2oemwmyju.html

parse_ini_file("config.ini", true)
来源：http://www.ydjk.org.cn/Article/details/gt2rbltftqx.html

[U74] PHP：读取环境变量
来源：http://www.52xcode.cn/Article/details/gt2pfseibwd.html

getenv("APP_ENV") ?: "production"
来源：http://www.ydjk.org.cn/Article/details/gt2vbtzbhop.html

[U75] PHP：依赖注入
来源：http://www.52xcode.cn/Article/details/gt2eqjdwzgv.html

composer require psr/container
来源：http://www.52xcode.cn/Article/details/gt2kwbogdov.html

[U76] PHP：简单路由
来源：http://www.52xcode.cn/Article/details/gt2rilxhaht.html

$path = parse_url($_SERVER["REQUEST_URI"], PHP_URL_PATH);
来源：http://www.52xcode.cn/Article/details/gt2gjwwjpxa.html

[U77] PHP：模板渲染
来源：http://www.52xcode.cn/Article/details/gt2nwgxzuwe.html

composer require twig/twig
来源：http://www.52xcode.cn/Article/details/gt2uhvudjle.html

[U78] PHP：单元测试
来源：http://www.52xcode.cn/Article/details/gt2ydvrwcla.html

composer require --dev phpunit/phpunit
来源：http://www.ydjk.org.cn/Article/details/gt2itiowbha.html

[U79] PHP：静态分析
来源：http://www.52xcode.cn/Article/details/gt2klikynws.html

composer require --dev phpstan/phpstan
来源：http://www.52xcode.cn/Article/details/gt2vtqsjbyl.html

[U80] PHP：代码规范修复
来源：http://www.ydjk.org.cn/Article/details/gt2bemoufgm.html

composer require --dev friendsofphp/php-cs-fixer
来源：http://www.ydjk.org.cn/Article/details/gt2sxgcxbya.html

[U81] JS：初始化项目
来源：http://www.ydjk.org.cn/Article/details/gt2xgoqqoqi.html

npm init -y;  npm i express
来源：http://www.ydjk.org.cn/Article/details/gt2qpwwvcpq.html

[U82] JS：package.json 脚本
来源：http://www.ydjk.org.cn/Article/details/gt2yndmcguy.html

"scripts": { "dev": "vite", "build": "vite build" }
来源：http://www.52xcode.cn/Article/details/gt2fttyjztf.html

[U83] JS：ES Module 导入导出
来源：http://www.52xcode.cn/Article/details/gt2tmqszsgd.html

export const a = 1;  import { a } from "./m.js";
来源：http://www.ydjk.org.cn/Article/details/gt2lcjtdbjc.html

[U84] JS：CommonJS 写法
来源：http://www.ydjk.org.cn/Article/details/gt2eolujcyg.html

module.exports = { a };  const { a } = require("./m");
来源：http://www.ydjk.org.cn/Article/details/gt2mdfekmfg.html

[U85] JS：可选链
来源：http://www.ydjk.org.cn/Article/details/gt2pnipdolu.html

a?.b?.c
来源：http://www.52xcode.cn/Article/details/gt2lieevqkt.html

[U86] JS：空值合并
来源：http://www.ydjk.org.cn/Article/details/gt2rglfrbim.html

a ?? b
来源：http://www.ydjk.org.cn/Article/details/gt2sybxaqeb.html

[U87] JS：解构默认值
来源：http://www.52xcode.cn/Article/details/gt2qgrlukgx.html

const { a = 1, b = 2 } = obj;
来源：http://www.52xcode.cn/Article/details/gt2enslpnil.html

[U88] JS：对象展开合并
来源：http://www.52xcode.cn/Article/details/gt2gvdxumvu.html

{ ...a, ...b }
来源：http://www.ydjk.org.cn/Article/details/gt2cuxnxezn.html

[U89] JS：数组去重
来源：http://www.52xcode.cn/Article/details/gt2dgwiedta.html

[...new Set(arr)]
来源：http://www.52xcode.cn/Article/details/gt2sfokvsdd.html

[U90] JS：数字数组排序
来源：http://www.ydjk.org.cn/Article/details/gt2wbnresbs.html

[...arr].sort((a, b) => a - b)
来源：http://www.ydjk.org.cn/Article/details/gt2uzbeohow.html

[U91] JS：对象键值遍历
来源：http://www.52xcode.cn/Article/details/gt2wgqhuxxt.html

Object.entries(obj).forEach(([k, v]) => {});
来源：http://www.52xcode.cn/Article/details/gt2wlawcsjc.html

[U92] JS：深拷贝
来源：http://www.ydjk.org.cn/Article/details/gt2gvptajtd.html

structuredClone(obj)
来源：http://www.ydjk.org.cn/Article/details/gt2ignpiqgb.html

[U93] JS：模板字符串
来源：http://www.ydjk.org.cn/Article/details/gt2ywgfpasf.html

`共 ${n} 条`
来源：http://www.ydjk.org.cn/Article/details/gt2tukquuer.html

[U94] JS：箭头函数
来源：http://www.52xcode.cn/Article/details/gt2czkpisch.html

const double = x => x * 2;
来源：http://www.52xcode.cn/Article/details/gt2pogyqksl.html

[U95] JS：Promise 包装
来源：http://www.52xcode.cn/Article/details/gt2gtxrgeyo.html

new Promise((resolve, reject) => {})
来源：http://www.52xcode.cn/Article/details/gt2jmlltebe.html

[U96] JS：async/await 与异常
来源：http://www.ydjk.org.cn/Article/details/gt2vkhchulz.html

try { const d = await f(); } catch (e) { console.error(e); }
来源：http://www.ydjk.org.cn/Article/details/gt2sinbxndm.html

[U97] JS：并发请求
来源：http://www.52xcode.cn/Article/details/gt2zfaacjjc.html

await Promise.all(urls.map(u => fetch(u)))
来源：http://www.52xcode.cn/Article/details/gt2toqiiklo.html

[U98] JS：fetch 带 JSON
来源：http://www.52xcode.cn/Article/details/gt2utouibcr.html

await fetch(url, { method: "POST", headers: { "Content-Type": "application/json" }, body: JSON.stringify(d) })
来源：http://www.ydjk.org.cn/Article/details/gt2mepnvveg.html

[U99] JS：事件监听
来源：http://www.ydjk.org.cn/Article/details/gt2vvcqygyv.html

el.addEventListener("click", e => {})
来源：http://www.ydjk.org.cn/Article/details/gt2gqqjqwne.html

[U100] JS：DOM 查询
来源：http://www.52xcode.cn/Article/details/gt2cvaqahkb.html

document.querySelector(".item")
来源：http://www.ydjk.org.cn/Article/details/gt2ooowpbpi.html

[U101] JS：classList 操作
来源：http://www.52xcode.cn/Article/details/gt2smoyrfby.html

el.classList.toggle("active")
来源：http://www.ydjk.org.cn/Article/details/gt2ppnwqcag.html

[U102] JS：本地存储
来源：http://www.52xcode.cn/Article/details/gt2gizrncif.html

localStorage.setItem("k", JSON.stringify(v))
来源：http://www.52xcode.cn/Article/details/gt2gdapbwez.html

[U103] JS：定时器
来源：http://www.52xcode.cn/Article/details/gt2sbqrlgpn.html

setTimeout(fn, 1000);  setInterval(fn, 1000);
来源：http://www.52xcode.cn/Article/details/gt2klgnonzx.html

[U104] JS：防抖
来源：http://www.ydjk.org.cn/Article/details/gt2kdogydjs.html

const debounce = (fn, ms) => { let t; return (...a) => { clearTimeout(t); t = setTimeout(() => fn(...a), ms); }; };
来源：http://www.ydjk.org.cn/Article/details/gt2vssdtsmj.html

[U105] JS：节流
来源：http://www.ydjk.org.cn/Article/details/gt2dbptukuk.html

const throttle = (fn, ms) => { let last = 0; return (...a) => { const n = Date.now(); if (n - last >= ms) { last = n; fn(...a); } }; };
来源：http://www.ydjk.org.cn/Article/details/gt2orcfasjz.html

[U106] JS：日期格式化
来源：http://www.52xcode.cn/Article/details/gt2guiwbjtp.html

new Intl.DateTimeFormat("zh-CN", { dateStyle: "medium" }).format(new Date())
来源：http://www.ydjk.org.cn/Article/details/gt2dlrxescy.html

[U107] JS：数字千分位
来源：http://www.52xcode.cn/Article/details/gt2lkkxlewu.html

new Intl.NumberFormat("en-US").format(1234567)
来源：http://www.52xcode.cn/Article/details/gt2clvsnljn.html

[U108] JS：随机整数
来源：http://www.52xcode.cn/Article/details/gt2ikbxcvrv.html

Math.floor(Math.random() * (max - min + 1)) + min
来源：http://www.52xcode.cn/Article/details/gt2jcjpiosv.html

[U109] JS：数组分组
来源：http://www.52xcode.cn/Article/details/gt2tmvtgxzg.html

Object.groupBy(arr, x => x.type)
来源：http://www.52xcode.cn/Article/details/gt2jluqedft.html

[U110] JS：数组分块
来源：http://www.52xcode.cn/Article/details/gt2haqxarlh.html

arr.reduce((acc, x, i) => (i % size ? acc : [...acc, arr.slice(i, i + size)]), [])
来源：http://www.ydjk.org.cn/Article/details/gt2ziahdtcn.html

[U111] JS：对象转 Map
来源：http://www.ydjk.org.cn/Article/details/gt2rpmwddlx.html

new Map(Object.entries(obj))
来源：http://www.ydjk.org.cn/Article/details/gt2tiwsmasm.html

[U112] JS：字符串补位
来源：http://www.52xcode.cn/Article/details/gt2uvgiqhkn.html

"7".padStart(3, "0")
来源：http://www.52xcode.cn/Article/details/gt2oeosowvx.html

[U113] JS：正则替换全部
来源：http://www.ydjk.org.cn/Article/details/gt2oqakrdhw.html

s.replaceAll("a", "b")
来源：http://www.52xcode.cn/Article/details/gt2vvzjdmmv.html

[U114] JS：JSON 深比较
来源：http://www.ydjk.org.cn/Article/details/gt2qdzbptfy.html

JSON.stringify(a) === JSON.stringify(b)
来源：http://www.ydjk.org.cn/Article/details/gt2oopkmist.html

[U115] JS：生成 UUID
来源：http://www.ydjk.org.cn/Article/details/gt2vpcuukzr.html

crypto.randomUUID()
来源：http://www.52xcode.cn/Article/details/gt2ecyykfdv.html

[U116] JS：类型检查（JSDoc）
来源：http://www.ydjk.org.cn/Article/details/gt2rrkdocbw.html

/** @param {string} name */ function f(name) {}
来源：http://www.52xcode.cn/Article/details/gt2sgygqgeo.html

[U117] JS：单元测试
来源：http://www.52xcode.cn/Article/details/gt2npqywubb.html

npm i -D vitest;  npx vitest
来源：http://www.52xcode.cn/Article/details/gt2onhtstbk.html

[U118] JS：开发服务器
来源：http://www.52xcode.cn/Article/details/gt2wqzdbwpr.html

npm i -D vite;  npx vite
来源：http://www.52xcode.cn/Article/details/gt2qavmiyzy.html

[U119] JS：生产构建
来源：http://www.52xcode.cn/Article/details/gt2inwgbxdy.html

npx vite build
来源：http://www.ydjk.org.cn/Article/details/gt2pqvqnchu.html

[U120] JS：读取环境变量（Vite）
来源：http://www.ydjk.org.cn/Article/details/gt2xpyjwlsq.html

import.meta.env.VITE_API_URL
来源：http://www.ydjk.org.cn/Article/details/gt2zhsruhsi.html

================================================================================
来源：http://www.ydjk.org.cn/Article/details/gt2xktizora.html

统计汇总
来源：http://www.52xcode.cn/Article/details/gt2paxrtahu.html

================================================================================
来源：http://www.52xcode.cn/Article/details/gt2zjuzufuv.html

按语言统计（条）：
来源：http://www.ydjk.org.cn/Article/details/gt2wbbrubwf.html

Python ......... 252
来源：http://www.52xcode.cn/Article/details/gt2xrggmgdz.html

PHP ............ 252
来源：http://www.ydjk.org.cn/Article/details/gt2jfasgihl.html

JavaScript ..... 252
来源：http://www.ydjk.org.cn/Article/details/gt2rxlqqhsi.html

TypeScript ..... 212
来源：http://www.ydjk.org.cn/Article/details/gt2ttwzkpzv.html

Java ........... 212
来源：http://www.ydjk.org.cn/Article/details/gt2wwoulcba.html

Go ............. 212
来源：http://www.ydjk.org.cn/Article/details/gt2yzrvaabg.html

Ruby ........... 212
来源：http://www.ydjk.org.cn/Article/details/gt2ttxmaywf.html

C# ............. 212
来源：http://www.52xcode.cn/Article/details/gt2jaddjaub.html

C .............. 30
来源：http://www.52xcode.cn/Article/details/gt2gkvdfcii.html

C++ ............ 30
来源：http://www.52xcode.cn/Article/details/gt2gnskatjp.html

SQL ............ 90
来源：http://www.ydjk.org.cn/Article/details/gt2vsdtlmnc.html

Bash ........... 80
来源：http://www.ydjk.org.cn/Article/details/gt2qwlffjng.html

Kotlin ......... 15
来源：http://www.ydjk.org.cn/Article/details/gt2yobihpbu.html

Swift .......... 15
来源：http://www.ydjk.org.cn/Article/details/gt2duzexvlw.html

Lua ............ 10
来源：http://www.ydjk.org.cn/Article/details/gt2ynaxtezd.html

Perl ........... 10
来源：http://www.ydjk.org.cn/Article/details/gt2ixcotqhp.html

Scala .......... 10
来源：http://www.52xcode.cn/Article/details/gt2bzfmozws.html

------------------------------------
来源：http://www.ydjk.org.cn/Article/details/gt2mjjingoo.html

合计 ........... 2106 条
来源：http://www.52xcode.cn/Article/details/gt2rawvgxpa.html

按章节统计：
来源：http://www.52xcode.cn/Article/details/gt2zrrsazfc.html

A 基础语法与类型       26 个任务 × 8 语言 =  208
来源：http://www.52xcode.cn/Article/details/gt2wqpxrzrl.html

B 流程控制             16 个任务 × 8 语言 =  128
来源：http://www.ydjk.org.cn/Article/details/gt2ydylpldn.html

C 函数与作用域         16 个任务 × 8 语言 =  128
来源：http://www.52xcode.cn/Article/details/gt2spkbcmgv.html

D 数组 / 列表 / 集合   26 个任务 × 8 语言 =  208
来源：http://www.ydjk.org.cn/Article/details/gt2vzyrplsx.html

E 字符串处理           22 个任务 × 8 语言 =  176
来源：http://www.52xcode.cn/Article/details/gt2ccjvzhre.html

F 文件与目录           12 个任务 × 8 语言 =   96
来源：http://www.52xcode.cn/Article/details/gt2bcqvthrt.html

G 面向对象             16 个任务 × 8 语言 =  128
来源：http://www.52xcode.cn/Article/details/gt2fdzglqfa.html

H 异常与错误处理       10 个任务 × 8 语言 =   80
来源：http://www.ydjk.org.cn/Article/details/gt2mqyxelge.html

I 正则表达式            8 个任务 × 8 语言 =   64
来源：http://www.52xcode.cn/Article/details/gt2egkogrrx.html

J 日期与时间           10 个任务 × 8 语言 =   80
来源：http://www.52xcode.cn/Article/details/gt2qslmtkof.html

K JSON 与序列化         8 个任务 × 8 语言 =   64
来源：http://www.ydjk.org.cn/Article/details/gt2cxtxzphn.html

L 网络请求              8 个任务 × 8 语言 =   64
来源：http://www.ydjk.org.cn/Article/details/gt2lglfansl.html

M 命令行 / 进程         8 个任务 × 8 语言 =   64
来源：http://www.52xcode.cn/Article/details/gt2uhcwfoyq.html

N 数据结构与算法       12 个任务 × 8 语言 =   96
来源：http://www.52xcode.cn/Article/details/gt2xkowbtux.html

O 并发与异步            6 个任务 × 8 语言 =   48
来源：http://www.ydjk.org.cn/Article/details/gt2vglscmuw.html

P 常用工具函数          8 个任务 × 8 语言 =   64
来源：http://www.52xcode.cn/Article/details/gt2ruozymng.html

Q SQL 专题                              90
来源：http://www.ydjk.org.cn/Article/details/gt2pxvnjgee.html

R Bash 专题                             80
来源：http://www.ydjk.org.cn/Article/details/gt2hozcjvil.html

S C / C++ 专题                          60
来源：http://www.ydjk.org.cn/Article/details/gt2kezzthfj.html

T 其他语言补充                          60
来源：http://www.ydjk.org.cn/Article/details/gt2flaojbqz.html

U 高频实用片段                         120
来源：http://www.ydjk.org.cn/Article/details/gt2xtcfaygt.html

------------------------------------
来源：http://www.ydjk.org.cn/Article/details/gt2qevbwgkp.html

合计                                  2106 条
来源：http://www.52xcode.cn/Article/details/gt2odhpgtbm.html

--------------------------------------------------------------------------------
来源：http://www.ydjk.org.cn/Article/details/gt2mpbbxgda.html

使用提醒
来源：http://www.52xcode.cn/Article/details/gt2izainlpf.html

--------------------------------------------------------------------------------
来源：http://www.ydjk.org.cn/Article/details/gt2kznynkun.html

1. 示例追求"最小可用"，正式项目中请补齐导入、错误处理与边界判断。
来源：http://www.52xcode.cn/Article/details/gt2tjzbbuvt.html

2. 涉及文件、网络、数据库的示例，注意资源释放与异常捕获。
来源：http://www.ydjk.org.cn/Article/details/gt2ultjajcg.html

3. 语言版本差异较大（如 Python 3.10 的 match、Java 17 的 record/switch 箭头），
来源：http://www.ydjk.org.cn/Article/details/gt2shbadlxr.html

在旧版本上使用前请先确认语法支持情况。
来源：http://www.52xcode.cn/Article/details/gt2yexeqafx.html

4. 标注"手写"的条目是因为该语言缺少对应内置能力，实际项目中可引入成熟库。
来源：http://www.ydjk.org.cn/Article/details/gt2hdqfwloy.html

—— 文件结束 ——
来源：http://www.52xcode.cn/Article/details/gt2vmroamsl.html

================================================================================
来源：http://www.52xcode.cn/Article/details/gt2yodijnjv.html

程序语言常见例子速查手册（2024 版）
来源：http://www.52xcode.cn/Article/details/gt2dmtjczwv.html

Common Programming Examples Cheat Book
来源：http://www.52xcode.cn/Article/details/gt2lwrnmfaz.html

================================================================================
来源：http://www.ydjk.org.cn/Article/details/gt2yuvawedl.html

【收录内容】
来源：http://www.52xcode.cn/Article/details/gt2fbqwepuo.html

覆盖 12 种语言 / 语法与常见 API：
来源：http://www.ydjk.org.cn/Article/details/gt2oamovelr.html

Python · PHP · JavaScript · TypeScript · Java · Go · Ruby · C#
来源：http://www.52xcode.cn/Article/details/gt2tszyspxr.html

SQL · Bash · C · C++
来源：http://www.52xcode.cn/Article/details/gt2uhgiacba.html

按「任务」分组：每个任务下按语言各给出一条最小可用示例。
来源：http://www.52xcode.cn/Article/details/gt2ormazhur.html

【使用说明】
来源：http://www.52xcode.cn/Article/details/gt2ilcvoykc.html

1. 每个任务形如 "[编号] 任务名"，下面每行以语言标记开头：
来源：http://www.ydjk.org.cn/Article/details/gt2sfbuphnw.html

Py:    Python        PHP:   PHP           JS:    JavaScript
来源：http://www.52xcode.cn/Article/details/gt2rfnwrlcr.html

TS:    TypeScript    Java:  Java          Go:    Go
来源：http://www.ydjk.org.cn/Article/details/gt2qyrcfmio.html

Ruby:  Ruby          C#:    C#            SQL:   SQL
来源：http://www.52xcode.cn/Article/details/gt2lhwporpr.html

Bash:  Shell         C:     C             C++:   C++
来源：http://www.52xcode.cn/Article/details/gt2zthabwqc.html

2. 示例只展示核心写法，刻意省略 import / require / include / using 等样板代码。
来源：http://www.52xcode.cn/Article/details/gt2dlknyieo.html

需要完整可运行文件时，请自行补齐当前语言的导入语句。
来源：http://www.ydjk.org.cn/Article/details/gt2ljihnetq.html

3. 语法基准：Python 3.10+ / PHP 8.1+ / ES2020+ / TypeScript 5 / Java 17 /
来源：http://www.ydjk.org.cn/Article/details/gt2bzhultor.html

Go 1.21+ / Ruby 3.x / C# 10+ / C17 / C++17。
来源：http://www.52xcode.cn/Article/details/gt2balwoypm.html

4. 检索建议：用编辑器或浏览器 Ctrl+F 搜关键词，如 "排序" "读取文件" "正则"。
来源：http://www.ydjk.org.cn/Article/details/gt2ocubjufm.html

5. 标记为 "// 无" 表示该语言没有对应的一等语法，需用替代写法（示例给出替代方案）。
来源：http://www.ydjk.org.cn/Article/details/gt2edlphowo.html

6. 符号 "⏎" 表示代码在此处换行（主要用于 Python 等强制缩进、无法压成一行的结构）。
来源：http://www.ydjk.org.cn/Article/details/gt2xtgfqxrw.html

【文件统计】
来源：http://www.52xcode.cn/Article/details/gt2rqggqogw.html

语言示例共 2106 条，分布见本文末尾的「统计汇总」。
来源：http://www.ydjk.org.cn/Article/details/gt2hbqeilmw.html


<!-- 参考信息 -->