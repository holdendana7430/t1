代发 wailian999

[U19] Py：正则替换带回调
来源：http://www.share.fehbvm.com/Article/details/guyhdiszs.sHtML

re.sub(r"\d+", lambda m: str(int(m.group()) * 2), s)
来源：http://wap.hesvh.cn/Article/details/gxkvdrxxu.sHtML

[U20] Py：缓存函数结果
来源：http://www.share.zdbjq.cn/Article/details/gnonsdihk.sHtML

@functools.lru_cache(maxsize=None)
来源：http://m.share.zdbjq.cn/Article/details/gpbzgpjdt.sHtML

[U21] Py：自定义上下文管理器
来源：http://mobile.hesvh.cn/Article/details/gthtvrhli.sHtML

@contextlib.contextmanager
来源：http://www.blog.zdbjq.cn/Article/details/gbffgtmrp.sHtML

[U22] Py：矩阵转置
来源：http://m.share.hesvh.cn/Article/details/gtxrkmndb.sHtML

list(zip(*m))
来源：http://mobile.hesvh.cn/Article/details/grotsvvyk.sHtML

[U23] Py：分块读取大文件
来源：http://read.share.zdbjq.cn/Article/details/gwrhxsgfp.sHtML

for chunk in iter(lambda: f.read(8192), b""):
来源：http://www.m.share.fehbvm.com/Article/details/gubjsolpb.sHtML

[U24] Py：路径操作
来源：http://mobile.hesvh.cn/Article/details/gknsdfqcj.sHtML

Path("a/b.txt").parent.mkdir(parents=True, exist_ok=True)
来源：http://wap.zdbjq.cn/Article/details/gueibjshe.sHtML

[U25] Py：CSV 按字典读
来源：http://mobile.fehbvm.com/Article/details/grngeqhyi.sHtML

csv.DictReader(f)
来源：http://mobile.fehbvm.com/Article/details/gsdxfdyjo.sHtML

[U26] Py：并发下载
来源：http://baike.fehbvm.com/Article/details/gmsbgbtxo.sHtML

ThreadPoolExecutor(max_workers=8).map(fetch, urls)
来源：http://3g.hesvh.cn/Article/details/gopycznki.sHtML

[U27] Py：异步 HTTP
来源：http://baike.zdbjq.cn/Article/details/gixvaswpq.sHtML

aiohttp.ClientSession() 配合 async with
来源：http://mobile.fehbvm.com/Article/details/gdorrdcbp.sHtML

[U28] Py：类型别名
来源：http://3g.hesvh.cn/Article/details/ghqnbglsy.sHtML

UserId = int
来源：http://blog.hesvh.cn/Article/details/gyqhvswrn.sHtML

[U29] Py：属性校验
来源：http://www.blog.zdbjq.cn/Article/details/giqcfkplk.sHtML

@property 与 @x.setter 配合
来源：http://mobile.fehbvm.com/Article/details/gfoxcvkhr.sHtML

[U30] Py：数据类
来源：http://3g.zdbjq.cn/Article/details/giwppytts.sHtML

@dataclass(slots=True)
来源：http://read.share.fehbvm.com/Article/details/gqmcsbtmv.sHtML

[U31] Py：单测
来源：http://www.blog.fehbvm.com/Article/details/gyosphrtd.sHtML

python -m pytest -q
来源：http://wap.zdbjq.cn/Article/details/ghutppahu.sHtML

[U32] Py：代码格式化
来源：http://mobile.fehbvm.com/Article/details/gopzykifi.sHtML

ruff format . && ruff check --fix .
来源：http://www.share.fehbvm.com/Article/details/gaansdaki.sHtML

[U33] Py：打包发布
来源：http://www.share.hesvh.cn/Article/details/gygdrikps.sHtML

python -m build  （依赖 pyproject.toml）
来源：http://m.share.fehbvm.com/Article/details/ggtgwqeai.sHtML

[U34] Py：判断编码
来源：http://www.m.share.zdbjq.cn/Article/details/glsdetgsd.sHtML

chardet.detect(raw)
来源：http://blog.hesvh.cn/Article/details/ghylljwyb.sHtML

[U35] Py：发送邮件
来源：http://www.blog.fehbvm.com/Article/details/gqyednaol.sHtML

smtplib.SMTP_SSL(...).send_message(msg)
来源：http://mobile.hesvh.cn/Article/details/gevfznupy.sHtML

[U36] Py：定时任务
来源：http://read.share.hesvh.cn/Article/details/ggxyucxaf.sHtML

schedule.every(10).minutes.do(job)
来源：http://blog.hesvh.cn/Article/details/ghtjeuiwd.sHtML

[U37] Py：读写 Excel
来源：http://baike.hesvh.cn/Article/details/gmvwkandb.sHtML

pandas.read_excel / DataFrame.to_excel
来源：http://3g.hesvh.cn/Article/details/gjpqfxhxx.sHtML

[U38] Py：获取脚本所在目录
来源：http://www.m.share.hesvh.cn/Article/details/gqicciaxv.sHtML

Path(__file__).resolve().parent
来源：http://www.blog.hesvh.cn/Article/details/gycztozgo.sHtML

[U39] Py：判断是否在交互环境
来源：http://wap.hesvh.cn/Article/details/gcfwblftj.sHtML

sys.stdout.isatty()
来源：http://baike.zdbjq.cn/Article/details/gvmenamvf.sHtML

[U40] Py：打印到标准错误
来源：http://mobile.zdbjq.cn/Article/details/glqpeqisy.sHtML

print("err", file=sys.stderr)
来源：http://mobile.zdbjq.cn/Article/details/gvupsauyb.sHtML

[U41] PHP：初始化 Composer 项目
来源：http://baike.zdbjq.cn/Article/details/gaqjbtfqn.sHtML

composer init;  composer require guzzlehttp/guzzle
来源：http://www.share.hesvh.cn/Article/details/gxrjfgnlf.sHtML

[U42] PHP：PSR-4 自动加载
来源：http://m.share.fehbvm.com/Article/details/gnyskkruc.sHtML

"autoload": { "psr-4": { "App\\": "src/" } }
来源：http://mobile.zdbjq.cn/Article/details/gfdzqqkql.sHtML

[U43] PHP：声明命名空间
来源：http://www.share.hesvh.cn/Article/details/gmxowonkc.sHtML

namespace App\Http;
来源：http://www.m.share.fehbvm.com/Article/details/ggwhdofoq.sHtML

[U44] PHP：开启严格类型
来源：http://blog.hesvh.cn/Article/details/gsouwsvxj.sHtML

declare(strict_types=1);
来源：http://www.m.share.fehbvm.com/Article/details/ghkqzqdxj.sHtML

[U45] PHP：类型声明与返回类型
来源：http://www.m.share.fehbvm.com/Article/details/gvpepsbmi.sHtML

function add(int $a, int $b): int { return $a + $b; }
来源：http://baike.zdbjq.cn/Article/details/gmkktszvb.sHtML

[U46] PHP：可空类型
来源：http://blog.hesvh.cn/Article/details/gdvsdnxgd.sHtML

?string $name = null
来源：http://m.share.fehbvm.com/Article/details/gropwjbah.sHtML

[U47] PHP：联合类型
来源：http://www.share.hesvh.cn/Article/details/grhsyxqbr.sHtML

int|string $id
来源：http://www.share.hesvh.cn/Article/details/gvopdrvha.sHtML

[U48] PHP：纯枚举
来源：http://baike.zdbjq.cn/Article/details/gqutdxnzp.sHtML

enum Status: string { case Active = "active"; case Off = "off"; }
来源：http://www.share.fehbvm.com/Article/details/gairvuapo.sHtML

[U49] PHP：只读属性
来源：http://3g.fehbvm.com/Article/details/guvspquxl.sHtML

public readonly string $name
来源：http://wap.fehbvm.com/Article/details/gxmtvnrve.sHtML

[U50] PHP：构造器属性提升
来源：http://read.share.zdbjq.cn/Article/details/glimfoqqu.sHtML

public function __construct(private int $id) {}
来源：http://3g.hesvh.cn/Article/details/glgaojbji.sHtML

[U51] PHP：数组解构
来源：http://m.share.hesvh.cn/Article/details/ghxqpehzq.sHtML

[$a, $b] = $arr;
来源：http://read.share.hesvh.cn/Article/details/gjwycoqrn.sHtML

[U52] PHP：箭头函数
来源：http://mobile.zdbjq.cn/Article/details/gzmabolko.sHtML

$double = fn($x) => $x * 2;
来源：http://www.share.zdbjq.cn/Article/details/giwtkkair.sHtML

[U53] PHP：空合并运算符
来源：http://www.blog.zdbjq.cn/Article/details/ggxwowsfn.sHtML

$v = $a ?? $b ?? "default";
来源：http://www.share.fehbvm.com/Article/details/gumzxkxdi.sHtML

[U54] PHP：空安全调用
来源：http://www.share.zdbjq.cn/Article/details/glmgfkrrc.sHtML

$obj?->method()
来源：http://www.blog.hesvh.cn/Article/details/gsxygsatn.sHtML

[U55] PHP：match 表达式
来源：http://3g.fehbvm.com/Article/details/ghcuhxsug.sHtML

$s = match($x) { 1 => "一", default => "其他" };
来源：http://blog.hesvh.cn/Article/details/gafsrtwuu.sHtML

[U56] PHP：命名参数
来源：http://blog.hesvh.cn/Article/details/galnnlbil.sHtML

f(a: 1, b: 2)
来源：http://www.m.share.zdbjq.cn/Article/details/gdxcwcfwb.sHtML

[U57] PHP：字符串插值
来源：http://www.share.fehbvm.com/Article/details/gkesovirw.sHtML

"值: {$a}"
来源：http://3g.zdbjq.cn/Article/details/gnszhadtg.sHtML

[U58] PHP：数组三件套
来源：http://3g.fehbvm.com/Article/details/gqztfbbrf.sHtML

array_map($f, $a);  array_filter($a, $f);  array_reduce($a, $f, 0);
来源：http://blog.hesvh.cn/Article/details/gxiaoabhz.sHtML

[U59] PHP：自定义排序
来源：http://mobile.fehbvm.com/Article/details/gjrdhecmu.sHtML

usort($arr, fn($a, $b) => $a["age"] <=> $b["age"]);
来源：http://mobile.hesvh.cn/Article/details/gqcjkyiqn.sHtML

[U60] PHP：JSON 编解码
来源：http://m.share.hesvh.cn/Article/details/glpiazagw.sHtML

json_encode($d, JSON_UNESCAPED_UNICODE);  json_decode($s, true);
来源：http://blog.zdbjq.cn/Article/details/ggbqhhtza.sHtML

[U61] PHP：正则
来源：http://read.share.zdbjq.cn/Article/details/gyllbfgqe.sHtML

preg_match('/(\d+)/', $s, $m);  preg_replace('/\d+/', '#', $s);
来源：http://www.share.fehbvm.com/Article/details/gjpqstqto.sHtML

[U62] PHP：日期对象
来源：http://wap.hesvh.cn/Article/details/ggqhxzfkx.sHtML

(new DateTimeImmutable())->format("Y-m-d");
来源：http://read.share.fehbvm.com/Article/details/gdypxwowu.sHtML

[U63] PHP：文件读写
来源：http://www.share.hesvh.cn/Article/details/gljvvswdf.sHtML

file_get_contents($f);  file_put_contents($f, $data);
来源：http://mobile.fehbvm.com/Article/details/gpclthbmu.sHtML

[U64] PHP：目录遍历
来源：http://www.blog.fehbvm.com/Article/details/gcaaqzgox.sHtML

glob("dir/*.php");  scandir("dir");
来源：http://baike.zdbjq.cn/Article/details/gcwfkqayv.sHtML

[U65] PHP：会话
来源：http://read.share.zdbjq.cn/Article/details/giensbdxc.sHtML

session_start();  $_SESSION["uid"] = 1;
来源：http://www.m.share.fehbvm.com/Article/details/gminommlj.sHtML

[U66] PHP：设置 Cookie
来源：http://www.m.share.zdbjq.cn/Article/details/gosjwvapz.sHtML

setcookie("token", $v, ["httponly" => true, "samesite" => "Lax"]);
来源：http://wap.hesvh.cn/Article/details/gxnxzumql.sHtML

[U67] PHP：处理文件上传
来源：http://wap.zdbjq.cn/Article/details/gzvnmwhdr.sHtML

$_FILES["file"]["tmp_name"] 与 move_uploaded_file()
来源：http://3g.fehbvm.com/Article/details/gjvkeqhfq.sHtML

[U68] PHP：PDO 连接
来源：http://3g.fehbvm.com/Article/details/gebnuhrft.sHtML

$pdo = new PDO("mysql:host=localhost;dbname=app", "root", "");
来源：http://3g.hesvh.cn/Article/details/gsbddwkhe.sHtML

[U69] PHP：PDO 预处理
来源：http://blog.hesvh.cn/Article/details/gligpryts.sHtML

$stmt = $pdo->prepare("SELECT * FROM users WHERE id = ?");  $stmt->execute([$id]);
来源：http://3g.zdbjq.cn/Article/details/gpcaynitb.sHtML

[U70] PHP：PDO 事务
来源：http://www.share.fehbvm.com/Article/details/gxuxpidib.sHtML

$pdo->beginTransaction();  $pdo->commit();  $pdo->rollBack();
来源：http://www.blog.zdbjq.cn/Article/details/gmtiiipie.sHtML

[U71] PHP：抛出异常
来源：http://m.share.fehbvm.com/Article/details/glmwmzvrc.sHtML

throw new RuntimeException("失败", 500);
来源：http://m.share.zdbjq.cn/Article/details/gmsauyrnn.sHtML

[U72] PHP：写错误日志
来源：http://wap.hesvh.cn/Article/details/giiyyjgtp.sHtML

error_log("失败: " . $e->getMessage());
来源：http://wap.fehbvm.com/Article/details/gmosflpuo.sHtML

[U73] PHP：读取 ini 配置
来源：http://mobile.zdbjq.cn/Article/details/gwpigfxyt.sHtML

parse_ini_file("config.ini", true)
来源：http://www.share.fehbvm.com/Article/details/gntpxaejy.sHtML

[U74] PHP：读取环境变量
来源：http://baike.zdbjq.cn/Article/details/gvhyctyge.sHtML

getenv("APP_ENV") ?: "production"
来源：http://wap.zdbjq.cn/Article/details/gysjkkjho.sHtML

[U75] PHP：依赖注入
来源：http://baike.hesvh.cn/Article/details/ggdpzalfk.sHtML

composer require psr/container
来源：http://blog.fehbvm.com/Article/details/ghtzxtswr.sHtML

[U76] PHP：简单路由
来源：http://read.share.hesvh.cn/Article/details/gnbtazvpl.sHtML

$path = parse_url($_SERVER["REQUEST_URI"], PHP_URL_PATH);
来源：http://3g.zdbjq.cn/Article/details/gqvvtkrsi.sHtML

[U77] PHP：模板渲染
来源：http://read.share.zdbjq.cn/Article/details/glcofwgkb.sHtML

composer require twig/twig
来源：http://3g.fehbvm.com/Article/details/gkbbowisv.sHtML

[U78] PHP：单元测试
来源：http://www.m.share.zdbjq.cn/Article/details/gaxufykzh.sHtML

composer require --dev phpunit/phpunit
来源：http://wap.zdbjq.cn/Article/details/grqilrsfa.sHtML

[U79] PHP：静态分析
来源：http://blog.hesvh.cn/Article/details/gqpnhmzwb.sHtML

composer require --dev phpstan/phpstan
来源：http://www.share.zdbjq.cn/Article/details/gfssnlccv.sHtML

[U80] PHP：代码规范修复
来源：http://wap.hesvh.cn/Article/details/gemzzjops.sHtML

composer require --dev friendsofphp/php-cs-fixer
来源：http://m.share.hesvh.cn/Article/details/gmrivkidk.sHtML

[U81] JS：初始化项目
来源：http://blog.fehbvm.com/Article/details/gtrweuwny.sHtML

npm init -y;  npm i express
来源：http://3g.hesvh.cn/Article/details/guqtikdeu.sHtML

[U82] JS：package.json 脚本
来源：http://m.share.zdbjq.cn/Article/details/guamchlkf.sHtML

"scripts": { "dev": "vite", "build": "vite build" }
来源：http://www.blog.zdbjq.cn/Article/details/gisdwbihl.sHtML

[U83] JS：ES Module 导入导出
来源：http://wap.zdbjq.cn/Article/details/ghinjyaao.sHtML

export const a = 1;  import { a } from "./m.js";
来源：http://www.blog.zdbjq.cn/Article/details/groddrveb.sHtML

[U84] JS：CommonJS 写法
来源：http://m.share.zdbjq.cn/Article/details/gryhckucj.sHtML

module.exports = { a };  const { a } = require("./m");
来源：http://baike.hesvh.cn/Article/details/glwgwxhwp.sHtML

[U85] JS：可选链
来源：http://m.share.hesvh.cn/Article/details/gfzixlsgq.sHtML

a?.b?.c
来源：http://www.share.fehbvm.com/Article/details/gdjclsscs.sHtML

[U86] JS：空值合并
来源：http://blog.hesvh.cn/Article/details/glneswnsv.sHtML

a ?? b
来源：http://www.share.zdbjq.cn/Article/details/goikwvqbs.sHtML

[U87] JS：解构默认值
来源：http://www.share.hesvh.cn/Article/details/gojjhfjzl.sHtML

const { a = 1, b = 2 } = obj;
来源：http://www.blog.hesvh.cn/Article/details/gptiwirsb.sHtML

[U88] JS：对象展开合并
来源：http://www.blog.zdbjq.cn/Article/details/gienzzgcm.sHtML

{ ...a, ...b }
来源：http://3g.zdbjq.cn/Article/details/gjxcncyad.sHtML

[U89] JS：数组去重
来源：http://mobile.hesvh.cn/Article/details/gxfckwcbr.sHtML

[...new Set(arr)]
来源：http://www.m.share.fehbvm.com/Article/details/gxypoweue.sHtML

[U90] JS：数字数组排序
来源：http://m.share.zdbjq.cn/Article/details/gslgbzloz.sHtML

[...arr].sort((a, b) => a - b)
来源：http://m.share.fehbvm.com/Article/details/gwnpbzwfd.sHtML

[U91] JS：对象键值遍历
来源：http://www.share.fehbvm.com/Article/details/gfavaxmhg.sHtML

Object.entries(obj).forEach(([k, v]) => {});
来源：http://www.m.share.zdbjq.cn/Article/details/gobsivzta.sHtML

[U92] JS：深拷贝
来源：http://www.blog.fehbvm.com/Article/details/gmulhyshj.sHtML

structuredClone(obj)
来源：http://www.share.zdbjq.cn/Article/details/gulbsnhgl.sHtML

[U93] JS：模板字符串
来源：http://www.blog.hesvh.cn/Article/details/gwcqmdweu.sHtML

`共 ${n} 条`
来源：http://mobile.hesvh.cn/Article/details/gowqtnnjp.sHtML

[U94] JS：箭头函数
来源：http://www.m.share.hesvh.cn/Article/details/gybdbwacl.sHtML

const double = x => x * 2;
来源：http://wap.fehbvm.com/Article/details/gzmmufqbe.sHtML

[U95] JS：Promise 包装
来源：http://www.blog.zdbjq.cn/Article/details/gmqmiltcg.sHtML

new Promise((resolve, reject) => {})
来源：http://m.share.hesvh.cn/Article/details/gotffazgw.sHtML

[U96] JS：async/await 与异常
来源：http://www.blog.zdbjq.cn/Article/details/gxqvkapet.sHtML

try { const d = await f(); } catch (e) { console.error(e); }
来源：http://blog.zdbjq.cn/Article/details/goesnohzq.sHtML

[U97] JS：并发请求
来源：http://wap.hesvh.cn/Article/details/gpsschnzm.sHtML

await Promise.all(urls.map(u => fetch(u)))
来源：http://www.share.zdbjq.cn/Article/details/gkgprzglr.sHtML

[U98] JS：fetch 带 JSON
来源：http://www.m.share.hesvh.cn/Article/details/gpsvvzhgv.sHtML

await fetch(url, { method: "POST", headers: { "Content-Type": "application/json" }, body: JSON.stringify(d) })
来源：http://m.share.zdbjq.cn/Article/details/grzegmcgv.sHtML

[U99] JS：事件监听
来源：http://read.share.zdbjq.cn/Article/details/gcpryptgg.sHtML

el.addEventListener("click", e => {})
来源：http://3g.fehbvm.com/Article/details/gtxhmexjf.sHtML

[U100] JS：DOM 查询
来源：http://read.share.zdbjq.cn/Article/details/glidullme.sHtML

document.querySelector(".item")
来源：http://read.share.fehbvm.com/Article/details/gnpvdamta.sHtML

[U101] JS：classList 操作
来源：http://mobile.zdbjq.cn/Article/details/gldxzhlpi.sHtML

el.classList.toggle("active")
来源：http://blog.hesvh.cn/Article/details/gyvbgienl.sHtML

[U102] JS：本地存储
来源：http://blog.zdbjq.cn/Article/details/gxvldluvw.sHtML

localStorage.setItem("k", JSON.stringify(v))
来源：http://3g.zdbjq.cn/Article/details/gmngbtxey.sHtML

[U103] JS：定时器
来源：http://baike.hesvh.cn/Article/details/gvzclvdli.sHtML

setTimeout(fn, 1000);  setInterval(fn, 1000);
来源：http://m.share.hesvh.cn/Article/details/gnebieuyf.sHtML

[U104] JS：防抖
来源：http://www.m.share.hesvh.cn/Article/details/geujegnar.sHtML

const debounce = (fn, ms) => { let t; return (...a) => { clearTimeout(t); t = setTimeout(() => fn(...a), ms); }; };
来源：http://www.blog.hesvh.cn/Article/details/gkdhxoens.sHtML

[U105] JS：节流
来源：http://www.share.hesvh.cn/Article/details/gcwrjslcj.sHtML

const throttle = (fn, ms) => { let last = 0; return (...a) => { const n = Date.now(); if (n - last >= ms) { last = n; fn(...a); } }; };
来源：http://wap.fehbvm.com/Article/details/gmdrvpklu.sHtML

[U106] JS：日期格式化
来源：http://baike.hesvh.cn/Article/details/gwasmldvk.sHtML

new Intl.DateTimeFormat("zh-CN", { dateStyle: "medium" }).format(new Date())
来源：http://wap.hesvh.cn/Article/details/gpkordjiz.sHtML

[U107] JS：数字千分位
来源：http://mobile.hesvh.cn/Article/details/glewmxvqi.sHtML

new Intl.NumberFormat("en-US").format(1234567)
来源：http://3g.fehbvm.com/Article/details/gqkjluttp.sHtML

[U108] JS：随机整数
来源：http://www.share.zdbjq.cn/Article/details/glkclrgen.sHtML

Math.floor(Math.random() * (max - min + 1)) + min
来源：http://blog.fehbvm.com/Article/details/ggskfeuux.sHtML

[U109] JS：数组分组
来源：http://3g.hesvh.cn/Article/details/giiodmwxr.sHtML

Object.groupBy(arr, x => x.type)
来源：http://www.share.zdbjq.cn/Article/details/gnojvadwg.sHtML

[U110] JS：数组分块
来源：http://m.share.hesvh.cn/Article/details/gcnrmldtf.sHtML

arr.reduce((acc, x, i) => (i % size ? acc : [...acc, arr.slice(i, i + size)]), [])
来源：http://m.share.zdbjq.cn/Article/details/gerqpoofp.sHtML

[U111] JS：对象转 Map
来源：http://www.m.share.hesvh.cn/Article/details/gxpjemore.sHtML

new Map(Object.entries(obj))
来源：http://m.share.zdbjq.cn/Article/details/gfnsdlwcy.sHtML

[U112] JS：字符串补位
来源：http://www.blog.hesvh.cn/Article/details/gfidhresa.sHtML

"7".padStart(3, "0")
来源：http://3g.zdbjq.cn/Article/details/gbzzoxciw.sHtML

[U113] JS：正则替换全部
来源：http://baike.fehbvm.com/Article/details/grxbobamz.sHtML

s.replaceAll("a", "b")
来源：http://3g.fehbvm.com/Article/details/gxumrvcpl.sHtML

[U114] JS：JSON 深比较
来源：http://www.share.zdbjq.cn/Article/details/glogblobg.sHtML

JSON.stringify(a) === JSON.stringify(b)
来源：http://3g.fehbvm.com/Article/details/geijmtwoe.sHtML

[U115] JS：生成 UUID
来源：http://read.share.fehbvm.com/Article/details/glyoxupzn.sHtML

crypto.randomUUID()
来源：http://m.share.hesvh.cn/Article/details/gtcslxtcq.sHtML

[U116] JS：类型检查（JSDoc）
来源：http://m.share.hesvh.cn/Article/details/gmsekiacu.sHtML

/** @param {string} name */ function f(name) {}
来源：http://3g.zdbjq.cn/Article/details/gwxpnqvbs.sHtML

[U117] JS：单元测试
来源：http://www.m.share.zdbjq.cn/Article/details/ghdrogcnx.sHtML

npm i -D vitest;  npx vitest
来源：http://www.share.zdbjq.cn/Article/details/gcaqbqehc.sHtML

[U118] JS：开发服务器
来源：http://blog.hesvh.cn/Article/details/gpbxmnffu.sHtML

npm i -D vite;  npx vite
来源：http://wap.fehbvm.com/Article/details/grwxlkfyw.sHtML

[U119] JS：生产构建
来源：http://www.blog.hesvh.cn/Article/details/gpmkzcvfi.sHtML

npx vite build
来源：http://wap.zdbjq.cn/Article/details/gxhbdfouq.sHtML

[U120] JS：读取环境变量（Vite）
来源：http://www.share.fehbvm.com/Article/details/gcilcmonv.sHtML

import.meta.env.VITE_API_URL
来源：http://blog.hesvh.cn/Article/details/gxxnawkyh.sHtML

================================================================================
来源：http://www.blog.zdbjq.cn/Article/details/gigsunboc.sHtML

统计汇总
来源：http://www.share.fehbvm.com/Article/details/galozskka.sHtML

================================================================================
来源：http://www.share.fehbvm.com/Article/details/gkiahzyos.sHtML

按语言统计（条）：
来源：http://baike.zdbjq.cn/Article/details/gfatyqpcw.sHtML

Python ......... 252
来源：http://baike.zdbjq.cn/Article/details/gcfaishxi.sHtML

PHP ............ 252
来源：http://baike.hesvh.cn/Article/details/gqakyfxzx.sHtML

JavaScript ..... 252
来源：http://www.blog.zdbjq.cn/Article/details/genwllfoi.sHtML

TypeScript ..... 212
来源：http://wap.zdbjq.cn/Article/details/gpyugdfmr.sHtML

Java ........... 212
来源：http://www.m.share.fehbvm.com/Article/details/gdzkertad.sHtML

Go ............. 212
来源：http://www.m.share.fehbvm.com/Article/details/gwmtenzlr.sHtML

Ruby ........... 212
来源：http://3g.fehbvm.com/Article/details/glchmenuo.sHtML

C# ............. 212
来源：http://blog.zdbjq.cn/Article/details/glbyfnudg.sHtML

C .............. 30
来源：http://read.share.zdbjq.cn/Article/details/guvoshuyu.sHtML

C++ ............ 30
来源：http://blog.zdbjq.cn/Article/details/gxazcndct.sHtML

SQL ............ 90
来源：http://mobile.fehbvm.com/Article/details/ggetbxsdj.sHtML

Bash ........... 80
来源：http://3g.hesvh.cn/Article/details/gclyaszno.sHtML

Kotlin ......... 15
来源：http://read.share.zdbjq.cn/Article/details/gnxmdblzj.sHtML

Swift .......... 15
来源：http://wap.zdbjq.cn/Article/details/gtrczrvxx.sHtML

Lua ............ 10
来源：http://wap.fehbvm.com/Article/details/gjhyfrlxi.sHtML

Perl ........... 10
来源：http://www.m.share.hesvh.cn/Article/details/gqbnljulx.sHtML

Scala .......... 10
来源：http://www.blog.zdbjq.cn/Article/details/gvnodrkuj.sHtML

------------------------------------
来源：http://blog.fehbvm.com/Article/details/gexyoougu.sHtML

合计 ........... 2106 条
来源：http://3g.hesvh.cn/Article/details/gddofnyfc.sHtML

按章节统计：
来源：http://www.m.share.hesvh.cn/Article/details/gyfxruwdj.sHtML

A 基础语法与类型       26 个任务 × 8 语言 =  208
来源：http://mobile.zdbjq.cn/Article/details/garniwyhy.sHtML

B 流程控制             16 个任务 × 8 语言 =  128
来源：http://read.share.fehbvm.com/Article/details/grqghpqtd.sHtML

C 函数与作用域         16 个任务 × 8 语言 =  128
来源：http://wap.hesvh.cn/Article/details/giykhkkuj.sHtML

D 数组 / 列表 / 集合   26 个任务 × 8 语言 =  208
来源：http://read.share.hesvh.cn/Article/details/gmcrfbuxu.sHtML

E 字符串处理           22 个任务 × 8 语言 =  176
来源：http://m.share.hesvh.cn/Article/details/gnoxivhvp.sHtML

F 文件与目录           12 个任务 × 8 语言 =   96
来源：http://www.m.share.zdbjq.cn/Article/details/gstmadqii.sHtML

G 面向对象             16 个任务 × 8 语言 =  128
来源：http://www.m.share.zdbjq.cn/Article/details/gyafnxcnz.sHtML

H 异常与错误处理       10 个任务 × 8 语言 =   80
来源：http://baike.zdbjq.cn/Article/details/gnigfloin.sHtML

I 正则表达式            8 个任务 × 8 语言 =   64
来源：http://wap.fehbvm.com/Article/details/gffcngipm.sHtML

J 日期与时间           10 个任务 × 8 语言 =   80
来源：http://wap.hesvh.cn/Article/details/gvmkxmwed.sHtML

K JSON 与序列化         8 个任务 × 8 语言 =   64
来源：http://read.share.hesvh.cn/Article/details/gcmqwsocy.sHtML

L 网络请求              8 个任务 × 8 语言 =   64
来源：http://www.share.hesvh.cn/Article/details/gcslnofxq.sHtML

M 命令行 / 进程         8 个任务 × 8 语言 =   64
来源：http://www.share.fehbvm.com/Article/details/gwtjmemsi.sHtML

N 数据结构与算法       12 个任务 × 8 语言 =   96
来源：http://3g.zdbjq.cn/Article/details/glizieqgq.sHtML

O 并发与异步            6 个任务 × 8 语言 =   48
来源：http://mobile.fehbvm.com/Article/details/gxgyfxmpt.sHtML

P 常用工具函数          8 个任务 × 8 语言 =   64
来源：http://www.m.share.hesvh.cn/Article/details/grpymdrmz.sHtML

Q SQL 专题                              90
来源：http://www.blog.zdbjq.cn/Article/details/gwlhpjrra.sHtML

R Bash 专题                             80
来源：http://www.blog.hesvh.cn/Article/details/gxrmckuje.sHtML

S C / C++ 专题                          60
来源：http://3g.zdbjq.cn/Article/details/gogqowekx.sHtML

T 其他语言补充                          60
来源：http://m.share.fehbvm.com/Article/details/gfivveibf.sHtML

U 高频实用片段                         120
来源：http://www.share.zdbjq.cn/Article/details/gloeewlpi.sHtML

------------------------------------
来源：http://m.share.hesvh.cn/Article/details/goumfbncf.sHtML

合计                                  2106 条
来源：http://www.m.share.fehbvm.com/Article/details/gijkhzkyk.sHtML

--------------------------------------------------------------------------------
来源：http://www.share.zdbjq.cn/Article/details/gnksapvki.sHtML

使用提醒
来源：http://mobile.fehbvm.com/Article/details/grsldossa.sHtML

--------------------------------------------------------------------------------
来源：http://wap.zdbjq.cn/Article/details/gcuoefvsy.sHtML

1. 示例追求"最小可用"，正式项目中请补齐导入、错误处理与边界判断。
来源：http://www.m.share.zdbjq.cn/Article/details/gkkfbiztj.sHtML

2. 涉及文件、网络、数据库的示例，注意资源释放与异常捕获。
来源：http://read.share.hesvh.cn/Article/details/gooaqhfqk.sHtML

3. 语言版本差异较大（如 Python 3.10 的 match、Java 17 的 record/switch 箭头），
来源：http://3g.fehbvm.com/Article/details/gublgljpf.sHtML

在旧版本上使用前请先确认语法支持情况。
来源：http://3g.zdbjq.cn/Article/details/gqtklxpcf.sHtML

4. 标注"手写"的条目是因为该语言缺少对应内置能力，实际项目中可引入成熟库。
来源：http://m.share.fehbvm.com/Article/details/gnhuxjmik.sHtML

—— 文件结束 ——
来源：http://mobile.hesvh.cn/Article/details/gjyqsknhm.sHtML

================================================================================
来源：http://www.m.share.fehbvm.com/Article/details/geohjjaak.sHtML

程序语言常见例子速查手册（2024 版）
来源：http://m.share.zdbjq.cn/Article/details/gonqhgwtu.sHtML

Common Programming Examples Cheat Book
来源：http://www.share.fehbvm.com/Article/details/gnlyxayyn.sHtML

================================================================================
来源：http://www.m.share.fehbvm.com/Article/details/gborpmftd.sHtML

【收录内容】
来源：http://read.share.hesvh.cn/Article/details/gvtnakews.sHtML

覆盖 12 种语言 / 语法与常见 API：
来源：http://www.share.fehbvm.com/Article/details/gvvlxlmhl.sHtML

Python · PHP · JavaScript · TypeScript · Java · Go · Ruby · C#
来源：http://www.m.share.fehbvm.com/Article/details/gnvziukat.sHtML

SQL · Bash · C · C++
来源：http://m.share.zdbjq.cn/Article/details/gwjgqsnxc.sHtML

按「任务」分组：每个任务下按语言各给出一条最小可用示例。
来源：http://read.share.zdbjq.cn/Article/details/gpjzrtede.sHtML

【使用说明】
来源：http://m.share.hesvh.cn/Article/details/gsopkmrvw.sHtML

1. 每个任务形如 "[编号] 任务名"，下面每行以语言标记开头：
来源：http://www.blog.hesvh.cn/Article/details/gdlffxbew.sHtML

Py:    Python        PHP:   PHP           JS:    JavaScript
来源：http://m.share.fehbvm.com/Article/details/govlalbkm.sHtML

TS:    TypeScript    Java:  Java          Go:    Go
来源：http://read.share.zdbjq.cn/Article/details/ghngmqizo.sHtML

Ruby:  Ruby          C#:    C#            SQL:   SQL
来源：http://www.share.zdbjq.cn/Article/details/gomgjkzzp.sHtML

Bash:  Shell         C:     C             C++:   C++
来源：http://www.m.share.fehbvm.com/Article/details/ghcnizfoo.sHtML

2. 示例只展示核心写法，刻意省略 import / require / include / using 等样板代码。
来源：http://baike.zdbjq.cn/Article/details/gtrawunct.sHtML

需要完整可运行文件时，请自行补齐当前语言的导入语句。
来源：http://www.blog.fehbvm.com/Article/details/gtemgvdka.sHtML

3. 语法基准：Python 3.10+ / PHP 8.1+ / ES2020+ / TypeScript 5 / Java 17 /
来源：http://blog.fehbvm.com/Article/details/gmayqsvdx.sHtML

Go 1.21+ / Ruby 3.x / C# 10+ / C17 / C++17。
来源：http://mobile.fehbvm.com/Article/details/garwxeqsg.sHtML

4. 检索建议：用编辑器或浏览器 Ctrl+F 搜关键词，如 "排序" "读取文件" "正则"。
来源：http://m.share.hesvh.cn/Article/details/gkfkxdbtp.sHtML

5. 标记为 "// 无" 表示该语言没有对应的一等语法，需用替代写法（示例给出替代方案）。
来源：http://read.share.zdbjq.cn/Article/details/gpgykfmwc.sHtML

6. 符号 "⏎" 表示代码在此处换行（主要用于 Python 等强制缩进、无法压成一行的结构）。
来源：http://blog.zdbjq.cn/Article/details/gktqntgoa.sHtML

【文件统计】
来源：http://www.m.share.hesvh.cn/Article/details/gifnuqnjg.sHtML

语言示例共 2106 条，分布见本文末尾的「统计汇总」。
来源：http://www.m.share.hesvh.cn/Article/details/gdvpubjgd.sHtML

--------------------------------------------------------------------------------
来源：http://3g.hesvh.cn/Article/details/gcxorhbce.sHtML

目  录
来源：http://www.share.hesvh.cn/Article/details/gyzyswvux.sHtML

--------------------------------------------------------------------------------
来源：http://www.m.share.hesvh.cn/Article/details/ghxmngwyz.sHtML

A. 基础语法与类型              （第 1 节，26 个任务，208 条）
来源：http://mobile.zdbjq.cn/Article/details/gwskomokd.sHtML

B. 流程控制                    （第 2 节，16 个任务，128 条）
来源：http://www.m.share.hesvh.cn/Article/details/gteapupqp.sHtML

C. 函数与作用域                （第 3 节，16 个任务，128 条）
来源：http://wap.hesvh.cn/Article/details/gmfkuwwaj.sHtML

D. 数组 / 列表 / 集合          （第 4 节，26 个任务，208 条）
来源：http://baike.hesvh.cn/Article/details/gdyyvkaff.sHtML

E. 字符串处理                  （第 5 节，22 个任务，176 条）
来源：http://3g.fehbvm.com/Article/details/gscrrcpin.sHtML

F. 文件与目录                  （第 6 节，12 个任务，96 条）
来源：http://mobile.hesvh.cn/Article/details/gdywcjbat.sHtML

G. 面向对象                    （第 7 节，16 个任务，128 条）
来源：http://blog.fehbvm.com/Article/details/grmrifuzo.sHtML

H. 异常与错误处理              （第 8 节，10 个任务，80 条）
来源：http://wap.fehbvm.com/Article/details/ghkhtllde.sHtML

I. 正则表达式                  （第 9 节，8 个任务，64 条）
来源：http://3g.fehbvm.com/Article/details/gimntmktq.sHtML

J. 日期与时间                  （第 10 节，10 个任务，80 条）
来源：http://www.share.zdbjq.cn/Article/details/gnfonsvge.sHtML

K. JSON 与序列化               （第 11 节，8 个任务，64 条）
来源：http://www.share.fehbvm.com/Article/details/gbgkdjymj.sHtML

L. 网络请求                    （第 12 节，8 个任务，64 条）
来源：http://www.share.fehbvm.com/Article/details/gpcecechi.sHtML

M. 命令行 / 进程 / 环境        （第 13 节，8 个任务，64 条）
来源：http://3g.hesvh.cn/Article/details/gojveszyc.sHtML


<!-- 参考信息 -->