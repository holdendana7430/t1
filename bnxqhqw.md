代发 wailian999

[U19] Py：正则替换带回调
来源：http://mobile.zdbjq.cn/Article/details/gccgjdogn.sHtML

re.sub(r"\d+", lambda m: str(int(m.group()) * 2), s)
来源：http://wap.fehbvm.com/Article/details/gjrhksprq.sHtML

[U20] Py：缓存函数结果
来源：http://m.share.zdbjq.cn/Article/details/gfhzgprma.sHtML

@functools.lru_cache(maxsize=None)
来源：http://www.blog.fehbvm.com/Article/details/gmsmzfltb.sHtML

[U21] Py：自定义上下文管理器
来源：http://blog.hesvh.cn/Article/details/gfkjgqtaf.sHtML

@contextlib.contextmanager
来源：http://www.share.zdbjq.cn/Article/details/gyfirjyxr.sHtML

[U22] Py：矩阵转置
来源：http://www.m.share.fehbvm.com/Article/details/gpfkbenar.sHtML

list(zip(*m))
来源：http://www.blog.hesvh.cn/Article/details/gdqvzppma.sHtML

[U23] Py：分块读取大文件
来源：http://mobile.zdbjq.cn/Article/details/geeoqmtla.sHtML

for chunk in iter(lambda: f.read(8192), b""):
来源：http://m.share.hesvh.cn/Article/details/gjfzbpugw.sHtML

[U24] Py：路径操作
来源：http://www.share.hesvh.cn/Article/details/gmmzjsawh.sHtML

Path("a/b.txt").parent.mkdir(parents=True, exist_ok=True)
来源：http://baike.zdbjq.cn/Article/details/ggwyjhpgx.sHtML

[U25] Py：CSV 按字典读
来源：http://www.blog.zdbjq.cn/Article/details/gjfnwmocc.sHtML

csv.DictReader(f)
来源：http://read.share.fehbvm.com/Article/details/gkkfaswya.sHtML

[U26] Py：并发下载
来源：http://www.m.share.zdbjq.cn/Article/details/gacfxfmrh.sHtML

ThreadPoolExecutor(max_workers=8).map(fetch, urls)
来源：http://mobile.zdbjq.cn/Article/details/gdcvrsyjr.sHtML

[U27] Py：异步 HTTP
来源：http://read.share.hesvh.cn/Article/details/glxwttlsm.sHtML

aiohttp.ClientSession() 配合 async with
来源：http://www.m.share.fehbvm.com/Article/details/gzwhdkvlu.sHtML

[U28] Py：类型别名
来源：http://www.blog.zdbjq.cn/Article/details/gsvauwqlf.sHtML

UserId = int
来源：http://read.share.fehbvm.com/Article/details/genvmxkpb.sHtML

[U29] Py：属性校验
来源：http://www.m.share.fehbvm.com/Article/details/gvvebiolf.sHtML

@property 与 @x.setter 配合
来源：http://www.m.share.fehbvm.com/Article/details/gezdzwugb.sHtML

[U30] Py：数据类
来源：http://3g.zdbjq.cn/Article/details/gwrkrfaii.sHtML

@dataclass(slots=True)
来源：http://mobile.hesvh.cn/Article/details/gqhtpwurx.sHtML

[U31] Py：单测
来源：http://wap.hesvh.cn/Article/details/gyrqvcvkk.sHtML

python -m pytest -q
来源：http://m.share.hesvh.cn/Article/details/gpbezncny.sHtML

[U32] Py：代码格式化
来源：http://read.share.hesvh.cn/Article/details/glaliwbka.sHtML

ruff format . && ruff check --fix .
来源：http://3g.hesvh.cn/Article/details/goucpiluf.sHtML

[U33] Py：打包发布
来源：http://blog.zdbjq.cn/Article/details/gjgmozksh.sHtML

python -m build  （依赖 pyproject.toml）
来源：http://m.share.hesvh.cn/Article/details/glswwwdgi.sHtML

[U34] Py：判断编码
来源：http://3g.hesvh.cn/Article/details/gexbptzuw.sHtML

chardet.detect(raw)
来源：http://blog.zdbjq.cn/Article/details/grgpbmoln.sHtML

[U35] Py：发送邮件
来源：http://www.share.hesvh.cn/Article/details/gdmsvontu.sHtML

smtplib.SMTP_SSL(...).send_message(msg)
来源：http://mobile.hesvh.cn/Article/details/gqladuxcb.sHtML

[U36] Py：定时任务
来源：http://read.share.fehbvm.com/Article/details/grtgbcqgw.sHtML

schedule.every(10).minutes.do(job)
来源：http://wap.fehbvm.com/Article/details/ggovtwqjx.sHtML

[U37] Py：读写 Excel
来源：http://www.share.zdbjq.cn/Article/details/gbpzhstsh.sHtML

pandas.read_excel / DataFrame.to_excel
来源：http://www.share.hesvh.cn/Article/details/gyowpegsd.sHtML

[U38] Py：获取脚本所在目录
来源：http://mobile.fehbvm.com/Article/details/gpletqsou.sHtML

Path(__file__).resolve().parent
来源：http://read.share.zdbjq.cn/Article/details/gzfhmtncw.sHtML

[U39] Py：判断是否在交互环境
来源：http://www.share.hesvh.cn/Article/details/gncdkxwfy.sHtML

sys.stdout.isatty()
来源：http://www.m.share.fehbvm.com/Article/details/gwcxfygvj.sHtML

[U40] Py：打印到标准错误
来源：http://www.m.share.hesvh.cn/Article/details/geloiwooa.sHtML

print("err", file=sys.stderr)
来源：http://m.share.zdbjq.cn/Article/details/ghfxqonpt.sHtML

[U41] PHP：初始化 Composer 项目
来源：http://mobile.hesvh.cn/Article/details/glvtfammh.sHtML

composer init;  composer require guzzlehttp/guzzle
来源：http://wap.zdbjq.cn/Article/details/glnnyqhpa.sHtML

[U42] PHP：PSR-4 自动加载
来源：http://www.m.share.zdbjq.cn/Article/details/gkehuqmam.sHtML

"autoload": { "psr-4": { "App\\": "src/" } }
来源：http://blog.hesvh.cn/Article/details/gtmehxoee.sHtML

[U43] PHP：声明命名空间
来源：http://read.share.hesvh.cn/Article/details/gqnonhxnm.sHtML

namespace App\Http;
来源：http://mobile.zdbjq.cn/Article/details/giomftovu.sHtML

[U44] PHP：开启严格类型
来源：http://www.blog.fehbvm.com/Article/details/gpdljcfoc.sHtML

declare(strict_types=1);
来源：http://blog.hesvh.cn/Article/details/gohvjjqjd.sHtML

[U45] PHP：类型声明与返回类型
来源：http://wap.fehbvm.com/Article/details/gymcntcuq.sHtML

function add(int $a, int $b): int { return $a + $b; }
来源：http://3g.fehbvm.com/Article/details/glcrsscoi.sHtML

[U46] PHP：可空类型
来源：http://baike.fehbvm.com/Article/details/gklvuxilk.sHtML

?string $name = null
来源：http://www.m.share.zdbjq.cn/Article/details/gswwfmnop.sHtML

[U47] PHP：联合类型
来源：http://baike.fehbvm.com/Article/details/gcxjpsgzs.sHtML

int|string $id
来源：http://m.share.hesvh.cn/Article/details/ghnfefbgf.sHtML

[U48] PHP：纯枚举
来源：http://www.m.share.fehbvm.com/Article/details/gnocpglbq.sHtML

enum Status: string { case Active = "active"; case Off = "off"; }
来源：http://www.m.share.hesvh.cn/Article/details/gxmitjbvi.sHtML

[U49] PHP：只读属性
来源：http://3g.fehbvm.com/Article/details/gmzkxnzjh.sHtML

public readonly string $name
来源：http://m.share.fehbvm.com/Article/details/gdoybreir.sHtML

[U50] PHP：构造器属性提升
来源：http://3g.fehbvm.com/Article/details/gwvvzyabj.sHtML

public function __construct(private int $id) {}
来源：http://mobile.hesvh.cn/Article/details/gfieqwkjk.sHtML

[U51] PHP：数组解构
来源：http://www.blog.hesvh.cn/Article/details/ggkfvnxkx.sHtML

[$a, $b] = $arr;
来源：http://www.m.share.fehbvm.com/Article/details/gwzngvamd.sHtML

[U52] PHP：箭头函数
来源：http://baike.zdbjq.cn/Article/details/gvipbiycy.sHtML

$double = fn($x) => $x * 2;
来源：http://m.share.zdbjq.cn/Article/details/gbzsctgtp.sHtML

[U53] PHP：空合并运算符
来源：http://wap.fehbvm.com/Article/details/gtzxjdimb.sHtML

$v = $a ?? $b ?? "default";
来源：http://www.share.fehbvm.com/Article/details/grdoegend.sHtML

[U54] PHP：空安全调用
来源：http://www.blog.hesvh.cn/Article/details/gjhkeaxmn.sHtML

$obj?->method()
来源：http://m.share.hesvh.cn/Article/details/glustljnn.sHtML

[U55] PHP：match 表达式
来源：http://baike.hesvh.cn/Article/details/gwhqatsmx.sHtML

$s = match($x) { 1 => "一", default => "其他" };
来源：http://read.share.fehbvm.com/Article/details/gjulecrbh.sHtML

[U56] PHP：命名参数
来源：http://mobile.hesvh.cn/Article/details/grkrypbic.sHtML

f(a: 1, b: 2)
来源：http://www.share.fehbvm.com/Article/details/gdmvdteqc.sHtML

[U57] PHP：字符串插值
来源：http://baike.hesvh.cn/Article/details/gipknzpol.sHtML

"值: {$a}"
来源：http://www.m.share.zdbjq.cn/Article/details/gqbdcuara.sHtML

[U58] PHP：数组三件套
来源：http://www.m.share.zdbjq.cn/Article/details/gydxbffba.sHtML

array_map($f, $a);  array_filter($a, $f);  array_reduce($a, $f, 0);
来源：http://www.m.share.hesvh.cn/Article/details/gnyypmivd.sHtML

[U59] PHP：自定义排序
来源：http://mobile.hesvh.cn/Article/details/gqfbkrzga.sHtML

usort($arr, fn($a, $b) => $a["age"] <=> $b["age"]);
来源：http://baike.zdbjq.cn/Article/details/gstgswolf.sHtML

[U60] PHP：JSON 编解码
来源：http://wap.hesvh.cn/Article/details/gpteagigq.sHtML

json_encode($d, JSON_UNESCAPED_UNICODE);  json_decode($s, true);
来源：http://m.share.fehbvm.com/Article/details/gaoabccih.sHtML

[U61] PHP：正则
来源：http://blog.hesvh.cn/Article/details/gxeiolayy.sHtML

preg_match('/(\d+)/', $s, $m);  preg_replace('/\d+/', '#', $s);
来源：http://www.m.share.hesvh.cn/Article/details/gibpimqar.sHtML

[U62] PHP：日期对象
来源：http://www.blog.zdbjq.cn/Article/details/gxfijcrmz.sHtML

(new DateTimeImmutable())->format("Y-m-d");
来源：http://www.share.fehbvm.com/Article/details/gkmbwxuvh.sHtML

[U63] PHP：文件读写
来源：http://www.share.fehbvm.com/Article/details/gkspxdsyo.sHtML

file_get_contents($f);  file_put_contents($f, $data);
来源：http://m.share.zdbjq.cn/Article/details/gnvptttzz.sHtML

[U64] PHP：目录遍历
来源：http://blog.zdbjq.cn/Article/details/ggbxjpoyh.sHtML

glob("dir/*.php");  scandir("dir");
来源：http://www.share.fehbvm.com/Article/details/ggxtjyqmu.sHtML

[U65] PHP：会话
来源：http://baike.hesvh.cn/Article/details/gpugrgbif.sHtML

session_start();  $_SESSION["uid"] = 1;
来源：http://www.blog.fehbvm.com/Article/details/gcmenylve.sHtML

[U66] PHP：设置 Cookie
来源：http://blog.fehbvm.com/Article/details/gjcqkhhaw.sHtML

setcookie("token", $v, ["httponly" => true, "samesite" => "Lax"]);
来源：http://read.share.fehbvm.com/Article/details/ghbyimyrr.sHtML

[U67] PHP：处理文件上传
来源：http://mobile.fehbvm.com/Article/details/gdtankjil.sHtML

$_FILES["file"]["tmp_name"] 与 move_uploaded_file()
来源：http://read.share.fehbvm.com/Article/details/gxapyimwb.sHtML

[U68] PHP：PDO 连接
来源：http://baike.fehbvm.com/Article/details/gttkkspiw.sHtML

$pdo = new PDO("mysql:host=localhost;dbname=app", "root", "");
来源：http://baike.zdbjq.cn/Article/details/glztlvfqd.sHtML

[U69] PHP：PDO 预处理
来源：http://www.share.zdbjq.cn/Article/details/gvwddhorr.sHtML

$stmt = $pdo->prepare("SELECT * FROM users WHERE id = ?");  $stmt->execute([$id]);
来源：http://3g.hesvh.cn/Article/details/grirgbpfd.sHtML

[U70] PHP：PDO 事务
来源：http://m.share.fehbvm.com/Article/details/ggnoskusx.sHtML

$pdo->beginTransaction();  $pdo->commit();  $pdo->rollBack();
来源：http://m.share.hesvh.cn/Article/details/gefbcwhei.sHtML

[U71] PHP：抛出异常
来源：http://blog.hesvh.cn/Article/details/gipvchkpb.sHtML

throw new RuntimeException("失败", 500);
来源：http://www.share.hesvh.cn/Article/details/gnsdizfha.sHtML

[U72] PHP：写错误日志
来源：http://www.m.share.zdbjq.cn/Article/details/grnrrstdw.sHtML

error_log("失败: " . $e->getMessage());
来源：http://baike.zdbjq.cn/Article/details/guhqnvkkp.sHtML

[U73] PHP：读取 ini 配置
来源：http://3g.zdbjq.cn/Article/details/gjturwbsm.sHtML

parse_ini_file("config.ini", true)
来源：http://3g.hesvh.cn/Article/details/ggvgjpviz.sHtML

[U74] PHP：读取环境变量
来源：http://blog.zdbjq.cn/Article/details/gdgydvpnl.sHtML

getenv("APP_ENV") ?: "production"
来源：http://wap.hesvh.cn/Article/details/gexeoqfgk.sHtML

[U75] PHP：依赖注入
来源：http://www.blog.hesvh.cn/Article/details/gtyzyhhpm.sHtML

composer require psr/container
来源：http://www.share.fehbvm.com/Article/details/gkwsldody.sHtML

[U76] PHP：简单路由
来源：http://www.blog.fehbvm.com/Article/details/gtcavwfpc.sHtML

$path = parse_url($_SERVER["REQUEST_URI"], PHP_URL_PATH);
来源：http://m.share.hesvh.cn/Article/details/gardzbshn.sHtML

[U77] PHP：模板渲染
来源：http://read.share.fehbvm.com/Article/details/gzastjjwq.sHtML

composer require twig/twig
来源：http://www.blog.zdbjq.cn/Article/details/gdqghxyfj.sHtML

[U78] PHP：单元测试
来源：http://3g.fehbvm.com/Article/details/gemrmdhir.sHtML

composer require --dev phpunit/phpunit
来源：http://3g.zdbjq.cn/Article/details/gkhlldhxv.sHtML

[U79] PHP：静态分析
来源：http://baike.fehbvm.com/Article/details/gmshgirlv.sHtML

composer require --dev phpstan/phpstan
来源：http://wap.fehbvm.com/Article/details/gkjlmkjxf.sHtML

[U80] PHP：代码规范修复
来源：http://baike.fehbvm.com/Article/details/gvuypohzg.sHtML

composer require --dev friendsofphp/php-cs-fixer
来源：http://3g.fehbvm.com/Article/details/gazhrwsgx.sHtML

[U81] JS：初始化项目
来源：http://m.share.fehbvm.com/Article/details/gsgkphonn.sHtML

npm init -y;  npm i express
来源：http://www.m.share.fehbvm.com/Article/details/gvzhjauml.sHtML

[U82] JS：package.json 脚本
来源：http://www.blog.zdbjq.cn/Article/details/gfbhknxso.sHtML

"scripts": { "dev": "vite", "build": "vite build" }
来源：http://wap.zdbjq.cn/Article/details/gltqlrfxo.sHtML

[U83] JS：ES Module 导入导出
来源：http://baike.zdbjq.cn/Article/details/gbqqfiwzz.sHtML

export const a = 1;  import { a } from "./m.js";
来源：http://wap.zdbjq.cn/Article/details/gpcmazjft.sHtML

[U84] JS：CommonJS 写法
来源：http://wap.hesvh.cn/Article/details/goqynruga.sHtML

module.exports = { a };  const { a } = require("./m");
来源：http://blog.hesvh.cn/Article/details/gshjokxov.sHtML

[U85] JS：可选链
来源：http://blog.fehbvm.com/Article/details/gpwwqdogj.sHtML

a?.b?.c
来源：http://wap.fehbvm.com/Article/details/gqajjpugy.sHtML

[U86] JS：空值合并
来源：http://mobile.fehbvm.com/Article/details/glmaoidxq.sHtML

a ?? b
来源：http://read.share.hesvh.cn/Article/details/gqwmxbikv.sHtML

[U87] JS：解构默认值
来源：http://wap.zdbjq.cn/Article/details/gqchufpel.sHtML

const { a = 1, b = 2 } = obj;
来源：http://blog.zdbjq.cn/Article/details/gtjoohtff.sHtML

[U88] JS：对象展开合并
来源：http://www.share.zdbjq.cn/Article/details/gawfztesr.sHtML

{ ...a, ...b }
来源：http://mobile.hesvh.cn/Article/details/gjfuurvpo.sHtML

[U89] JS：数组去重
来源：http://wap.hesvh.cn/Article/details/gqrmznces.sHtML

[...new Set(arr)]
来源：http://3g.hesvh.cn/Article/details/gntfoevmo.sHtML

[U90] JS：数字数组排序
来源：http://www.m.share.fehbvm.com/Article/details/ggdsdilxp.sHtML

[...arr].sort((a, b) => a - b)
来源：http://blog.fehbvm.com/Article/details/gckxpogpq.sHtML

[U91] JS：对象键值遍历
来源：http://blog.hesvh.cn/Article/details/ghmldqsqv.sHtML

Object.entries(obj).forEach(([k, v]) => {});
来源：http://wap.zdbjq.cn/Article/details/gqwbasybe.sHtML

[U92] JS：深拷贝
来源：http://mobile.zdbjq.cn/Article/details/gesjlzhjj.sHtML

structuredClone(obj)
来源：http://read.share.hesvh.cn/Article/details/gfvxasuqd.sHtML

[U93] JS：模板字符串
来源：http://read.share.zdbjq.cn/Article/details/gavmmyqqm.sHtML

`共 ${n} 条`
来源：http://blog.hesvh.cn/Article/details/gcinbgpvg.sHtML

[U94] JS：箭头函数
来源：http://blog.hesvh.cn/Article/details/geqgenisb.sHtML

const double = x => x * 2;
来源：http://www.blog.hesvh.cn/Article/details/gyovsoyiv.sHtML

[U95] JS：Promise 包装
来源：http://m.share.fehbvm.com/Article/details/glaxwhlcl.sHtML

new Promise((resolve, reject) => {})
来源：http://www.share.zdbjq.cn/Article/details/ghbgloigq.sHtML

[U96] JS：async/await 与异常
来源：http://wap.hesvh.cn/Article/details/gltblgeju.sHtML

try { const d = await f(); } catch (e) { console.error(e); }
来源：http://www.share.hesvh.cn/Article/details/ggojreakh.sHtML

[U97] JS：并发请求
来源：http://baike.hesvh.cn/Article/details/gylozgrlv.sHtML

await Promise.all(urls.map(u => fetch(u)))
来源：http://baike.hesvh.cn/Article/details/gwhlhqsbs.sHtML

[U98] JS：fetch 带 JSON
来源：http://www.blog.zdbjq.cn/Article/details/gjlnayvky.sHtML

await fetch(url, { method: "POST", headers: { "Content-Type": "application/json" }, body: JSON.stringify(d) })
来源：http://baike.zdbjq.cn/Article/details/grddrrtxd.sHtML

[U99] JS：事件监听
来源：http://read.share.hesvh.cn/Article/details/grqwlmhup.sHtML

el.addEventListener("click", e => {})
来源：http://mobile.zdbjq.cn/Article/details/gkimsgbwc.sHtML

[U100] JS：DOM 查询
来源：http://baike.fehbvm.com/Article/details/gvcuwbmtv.sHtML

document.querySelector(".item")
来源：http://www.share.fehbvm.com/Article/details/gfqhahovm.sHtML

[U101] JS：classList 操作
来源：http://baike.fehbvm.com/Article/details/glnsleefh.sHtML

el.classList.toggle("active")
来源：http://baike.zdbjq.cn/Article/details/gazrihhyz.sHtML

[U102] JS：本地存储
来源：http://baike.zdbjq.cn/Article/details/gbushhfer.sHtML

localStorage.setItem("k", JSON.stringify(v))
来源：http://www.share.hesvh.cn/Article/details/glhwborfh.sHtML

[U103] JS：定时器
来源：http://blog.fehbvm.com/Article/details/gdwiweyzj.sHtML

setTimeout(fn, 1000);  setInterval(fn, 1000);
来源：http://www.share.fehbvm.com/Article/details/gnyeytdhd.sHtML

[U104] JS：防抖
来源：http://m.share.fehbvm.com/Article/details/gyswxnuik.sHtML

const debounce = (fn, ms) => { let t; return (...a) => { clearTimeout(t); t = setTimeout(() => fn(...a), ms); }; };
来源：http://baike.fehbvm.com/Article/details/gohwtujzu.sHtML

[U105] JS：节流
来源：http://www.blog.zdbjq.cn/Article/details/grndioujm.sHtML

const throttle = (fn, ms) => { let last = 0; return (...a) => { const n = Date.now(); if (n - last >= ms) { last = n; fn(...a); } }; };
来源：http://www.m.share.hesvh.cn/Article/details/gjymxiqmw.sHtML

[U106] JS：日期格式化
来源：http://3g.fehbvm.com/Article/details/gbzlptykq.sHtML

new Intl.DateTimeFormat("zh-CN", { dateStyle: "medium" }).format(new Date())
来源：http://blog.hesvh.cn/Article/details/gtlyehdnr.sHtML

[U107] JS：数字千分位
来源：http://read.share.fehbvm.com/Article/details/gjfbyhxqz.sHtML

new Intl.NumberFormat("en-US").format(1234567)
来源：http://blog.fehbvm.com/Article/details/gtqpheumi.sHtML

[U108] JS：随机整数
来源：http://www.share.hesvh.cn/Article/details/gcxxgglkd.sHtML

Math.floor(Math.random() * (max - min + 1)) + min
来源：http://www.blog.hesvh.cn/Article/details/gmwebqwaw.sHtML

[U109] JS：数组分组
来源：http://www.m.share.fehbvm.com/Article/details/gypzmvhdp.sHtML

Object.groupBy(arr, x => x.type)
来源：http://blog.hesvh.cn/Article/details/guxdlyobq.sHtML

[U110] JS：数组分块
来源：http://read.share.hesvh.cn/Article/details/gieuonfjt.sHtML

arr.reduce((acc, x, i) => (i % size ? acc : [...acc, arr.slice(i, i + size)]), [])
来源：http://read.share.fehbvm.com/Article/details/grgbqvkxo.sHtML

[U111] JS：对象转 Map
来源：http://www.share.fehbvm.com/Article/details/gvzodxttu.sHtML

new Map(Object.entries(obj))
来源：http://www.blog.fehbvm.com/Article/details/gjmdlxmjk.sHtML

[U112] JS：字符串补位
来源：http://wap.zdbjq.cn/Article/details/gdcogntuw.sHtML

"7".padStart(3, "0")
来源：http://www.blog.zdbjq.cn/Article/details/gilveehyj.sHtML

[U113] JS：正则替换全部
来源：http://blog.zdbjq.cn/Article/details/gpwmsolev.sHtML

s.replaceAll("a", "b")
来源：http://m.share.hesvh.cn/Article/details/gcsvecxlw.sHtML

[U114] JS：JSON 深比较
来源：http://www.share.zdbjq.cn/Article/details/gvqacwufo.sHtML

JSON.stringify(a) === JSON.stringify(b)
来源：http://www.blog.hesvh.cn/Article/details/gqyyyryra.sHtML

[U115] JS：生成 UUID
来源：http://www.blog.zdbjq.cn/Article/details/gvjftitpu.sHtML

crypto.randomUUID()
来源：http://read.share.fehbvm.com/Article/details/gpowfgcyc.sHtML

[U116] JS：类型检查（JSDoc）
来源：http://www.m.share.zdbjq.cn/Article/details/grhtzhsjm.sHtML

/** @param {string} name */ function f(name) {}
来源：http://3g.fehbvm.com/Article/details/gdqegqmer.sHtML

[U117] JS：单元测试
来源：http://blog.zdbjq.cn/Article/details/gdoqobcdk.sHtML

npm i -D vitest;  npx vitest
来源：http://m.share.fehbvm.com/Article/details/gzubrwihv.sHtML

[U118] JS：开发服务器
来源：http://baike.zdbjq.cn/Article/details/girmavbgs.sHtML

npm i -D vite;  npx vite
来源：http://wap.hesvh.cn/Article/details/gamudxdzb.sHtML

[U119] JS：生产构建
来源：http://m.share.zdbjq.cn/Article/details/gudgnxjce.sHtML

npx vite build
来源：http://read.share.hesvh.cn/Article/details/gpwglwogt.sHtML

[U120] JS：读取环境变量（Vite）
来源：http://mobile.hesvh.cn/Article/details/gnwtlfein.sHtML

import.meta.env.VITE_API_URL
来源：http://baike.zdbjq.cn/Article/details/gtnuckuww.sHtML

================================================================================
来源：http://www.share.zdbjq.cn/Article/details/gownrcuae.sHtML

统计汇总
来源：http://www.blog.hesvh.cn/Article/details/gufqqarpu.sHtML

================================================================================
来源：http://wap.fehbvm.com/Article/details/gfgdvpkag.sHtML

按语言统计（条）：
来源：http://www.share.zdbjq.cn/Article/details/grjliuimw.sHtML

Python ......... 252
来源：http://wap.zdbjq.cn/Article/details/giusasjxk.sHtML

PHP ............ 252
来源：http://blog.zdbjq.cn/Article/details/gfrlxrjiq.sHtML

JavaScript ..... 252
来源：http://m.share.zdbjq.cn/Article/details/gafnsroyq.sHtML

TypeScript ..... 212
来源：http://wap.fehbvm.com/Article/details/gusigzawh.sHtML

Java ........... 212
来源：http://3g.zdbjq.cn/Article/details/ghxrerscq.sHtML

Go ............. 212
来源：http://m.share.fehbvm.com/Article/details/ghaljpiya.sHtML

Ruby ........... 212
来源：http://www.m.share.fehbvm.com/Article/details/gmzuzjurh.sHtML

C# ............. 212
来源：http://www.blog.hesvh.cn/Article/details/gvwcynsve.sHtML

C .............. 30
来源：http://3g.zdbjq.cn/Article/details/glkieqisn.sHtML

C++ ............ 30
来源：http://3g.zdbjq.cn/Article/details/gzyapitwp.sHtML

SQL ............ 90
来源：http://www.blog.zdbjq.cn/Article/details/guvwkrluq.sHtML

Bash ........... 80
来源：http://baike.fehbvm.com/Article/details/glhpxfzhs.sHtML

Kotlin ......... 15
来源：http://blog.fehbvm.com/Article/details/giwrfuqkc.sHtML

Swift .......... 15
来源：http://blog.hesvh.cn/Article/details/gqqhzrtlf.sHtML

Lua ............ 10
来源：http://read.share.zdbjq.cn/Article/details/glkmxfucu.sHtML

Perl ........... 10
来源：http://mobile.fehbvm.com/Article/details/gmjtkiagd.sHtML

Scala .......... 10
来源：http://3g.zdbjq.cn/Article/details/glmsvdunp.sHtML

------------------------------------
来源：http://read.share.hesvh.cn/Article/details/gxxbcmzon.sHtML

合计 ........... 2106 条
来源：http://www.share.fehbvm.com/Article/details/gjhynzhxf.sHtML

按章节统计：
来源：http://blog.zdbjq.cn/Article/details/gcrrbrlox.sHtML

A 基础语法与类型       26 个任务 × 8 语言 =  208
来源：http://www.m.share.fehbvm.com/Article/details/gojomtgvt.sHtML

B 流程控制             16 个任务 × 8 语言 =  128
来源：http://www.blog.zdbjq.cn/Article/details/gmiuiyvih.sHtML

C 函数与作用域         16 个任务 × 8 语言 =  128
来源：http://www.blog.hesvh.cn/Article/details/gudwqwzbs.sHtML

D 数组 / 列表 / 集合   26 个任务 × 8 语言 =  208
来源：http://mobile.hesvh.cn/Article/details/gettziiba.sHtML

E 字符串处理           22 个任务 × 8 语言 =  176
来源：http://www.share.hesvh.cn/Article/details/gvbqztzoj.sHtML

F 文件与目录           12 个任务 × 8 语言 =   96
来源：http://3g.zdbjq.cn/Article/details/geuorrofc.sHtML

G 面向对象             16 个任务 × 8 语言 =  128
来源：http://baike.zdbjq.cn/Article/details/gawywimnu.sHtML

H 异常与错误处理       10 个任务 × 8 语言 =   80
来源：http://read.share.fehbvm.com/Article/details/gqrufbqke.sHtML

I 正则表达式            8 个任务 × 8 语言 =   64
来源：http://blog.hesvh.cn/Article/details/gjyappfsl.sHtML

J 日期与时间           10 个任务 × 8 语言 =   80
来源：http://read.share.hesvh.cn/Article/details/gyxsunopr.sHtML

K JSON 与序列化         8 个任务 × 8 语言 =   64
来源：http://www.blog.hesvh.cn/Article/details/gjlgyfswn.sHtML

L 网络请求              8 个任务 × 8 语言 =   64
来源：http://read.share.fehbvm.com/Article/details/gjzuuxuxo.sHtML

M 命令行 / 进程         8 个任务 × 8 语言 =   64
来源：http://www.share.zdbjq.cn/Article/details/gspjjgbry.sHtML

N 数据结构与算法       12 个任务 × 8 语言 =   96
来源：http://baike.hesvh.cn/Article/details/gswlmmlav.sHtML

O 并发与异步            6 个任务 × 8 语言 =   48
来源：http://www.m.share.hesvh.cn/Article/details/gywhcjmgd.sHtML

P 常用工具函数          8 个任务 × 8 语言 =   64
来源：http://blog.hesvh.cn/Article/details/grurbgjqv.sHtML

Q SQL 专题                              90
来源：http://read.share.fehbvm.com/Article/details/gnvthqxuz.sHtML

R Bash 专题                             80
来源：http://m.share.hesvh.cn/Article/details/gkqdklors.sHtML

S C / C++ 专题                          60
来源：http://wap.zdbjq.cn/Article/details/gespjbxzn.sHtML

T 其他语言补充                          60
来源：http://www.m.share.zdbjq.cn/Article/details/guqmtptjw.sHtML

U 高频实用片段                         120
来源：http://blog.hesvh.cn/Article/details/gyohqbbax.sHtML

------------------------------------
来源：http://mobile.zdbjq.cn/Article/details/geipoiipc.sHtML

合计                                  2106 条
来源：http://3g.zdbjq.cn/Article/details/gaqpnvpln.sHtML

--------------------------------------------------------------------------------
来源：http://wap.zdbjq.cn/Article/details/ggtswmdbp.sHtML

使用提醒
来源：http://www.blog.fehbvm.com/Article/details/gysbgnjnr.sHtML

--------------------------------------------------------------------------------
来源：http://m.share.hesvh.cn/Article/details/gifhceymq.sHtML

1. 示例追求"最小可用"，正式项目中请补齐导入、错误处理与边界判断。
来源：http://www.m.share.fehbvm.com/Article/details/gjnkvynke.sHtML

2. 涉及文件、网络、数据库的示例，注意资源释放与异常捕获。
来源：http://read.share.hesvh.cn/Article/details/gfuktqosj.sHtML

3. 语言版本差异较大（如 Python 3.10 的 match、Java 17 的 record/switch 箭头），
来源：http://baike.fehbvm.com/Article/details/ghyuxewnm.sHtML

在旧版本上使用前请先确认语法支持情况。
来源：http://www.share.zdbjq.cn/Article/details/gvwcwlqjy.sHtML

4. 标注"手写"的条目是因为该语言缺少对应内置能力，实际项目中可引入成熟库。
来源：http://blog.zdbjq.cn/Article/details/gjezprmpa.sHtML

—— 文件结束 ——
来源：http://www.m.share.fehbvm.com/Article/details/guixygsuf.sHtML

================================================================================
来源：http://mobile.fehbvm.com/Article/details/gzmgltgsa.sHtML

程序语言常见例子速查手册（2024 版）
来源：http://blog.zdbjq.cn/Article/details/gndpbvcjv.sHtML

Common Programming Examples Cheat Book
来源：http://3g.zdbjq.cn/Article/details/gacotovsi.sHtML

================================================================================
来源：http://baike.zdbjq.cn/Article/details/gyogfeaed.sHtML

【收录内容】
来源：http://baike.zdbjq.cn/Article/details/gyiqrlvhx.sHtML

覆盖 12 种语言 / 语法与常见 API：
来源：http://m.share.hesvh.cn/Article/details/gvryvlqpt.sHtML

Python · PHP · JavaScript · TypeScript · Java · Go · Ruby · C#
来源：http://www.share.hesvh.cn/Article/details/gfmcidiae.sHtML

SQL · Bash · C · C++
来源：http://www.m.share.fehbvm.com/Article/details/gveklznuu.sHtML

按「任务」分组：每个任务下按语言各给出一条最小可用示例。
来源：http://wap.hesvh.cn/Article/details/glmpjsljj.sHtML

【使用说明】
来源：http://wap.hesvh.cn/Article/details/gvgfhoxgk.sHtML

1. 每个任务形如 "[编号] 任务名"，下面每行以语言标记开头：
来源：http://read.share.fehbvm.com/Article/details/gupmjlhfo.sHtML

Py:    Python        PHP:   PHP           JS:    JavaScript
来源：http://baike.zdbjq.cn/Article/details/gwkoogzkl.sHtML

TS:    TypeScript    Java:  Java          Go:    Go
来源：http://www.share.hesvh.cn/Article/details/guihpmyuh.sHtML

Ruby:  Ruby          C#:    C#            SQL:   SQL
来源：http://m.share.zdbjq.cn/Article/details/genpolnmi.sHtML

Bash:  Shell         C:     C             C++:   C++
来源：http://baike.zdbjq.cn/Article/details/gtkbdrhvp.sHtML

2. 示例只展示核心写法，刻意省略 import / require / include / using 等样板代码。
来源：http://wap.zdbjq.cn/Article/details/giaeazetl.sHtML

需要完整可运行文件时，请自行补齐当前语言的导入语句。
来源：http://mobile.zdbjq.cn/Article/details/gsslwgxug.sHtML

3. 语法基准：Python 3.10+ / PHP 8.1+ / ES2020+ / TypeScript 5 / Java 17 /
来源：http://www.m.share.zdbjq.cn/Article/details/gudqapkdj.sHtML

Go 1.21+ / Ruby 3.x / C# 10+ / C17 / C++17。
来源：http://baike.fehbvm.com/Article/details/gdobytujv.sHtML

4. 检索建议：用编辑器或浏览器 Ctrl+F 搜关键词，如 "排序" "读取文件" "正则"。
来源：http://www.share.zdbjq.cn/Article/details/gmoyhewzl.sHtML

5. 标记为 "// 无" 表示该语言没有对应的一等语法，需用替代写法（示例给出替代方案）。
来源：http://baike.zdbjq.cn/Article/details/gtupjecbl.sHtML

6. 符号 "⏎" 表示代码在此处换行（主要用于 Python 等强制缩进、无法压成一行的结构）。
来源：http://wap.fehbvm.com/Article/details/gpdtqkwnn.sHtML

【文件统计】
来源：http://www.m.share.hesvh.cn/Article/details/gfyyjfqtv.sHtML

语言示例共 2106 条，分布见本文末尾的「统计汇总」。
来源：http://m.share.hesvh.cn/Article/details/glzctjugm.sHtML

--------------------------------------------------------------------------------
来源：http://read.share.hesvh.cn/Article/details/gdxqucexi.sHtML

目  录
来源：http://www.blog.zdbjq.cn/Article/details/gudcnaspe.sHtML

--------------------------------------------------------------------------------
来源：http://m.share.zdbjq.cn/Article/details/ghctxxael.sHtML

A. 基础语法与类型              （第 1 节，26 个任务，208 条）
来源：http://blog.hesvh.cn/Article/details/gyeykpcti.sHtML

B. 流程控制                    （第 2 节，16 个任务，128 条）
来源：http://mobile.hesvh.cn/Article/details/guywmfxqp.sHtML

C. 函数与作用域                （第 3 节，16 个任务，128 条）
来源：http://m.share.fehbvm.com/Article/details/gfsiabsdh.sHtML

D. 数组 / 列表 / 集合          （第 4 节，26 个任务，208 条）
来源：http://wap.zdbjq.cn/Article/details/gvhkiyvgr.sHtML

E. 字符串处理                  （第 5 节，22 个任务，176 条）
来源：http://m.share.fehbvm.com/Article/details/gqmlzkiak.sHtML

F. 文件与目录                  （第 6 节，12 个任务，96 条）
来源：http://blog.fehbvm.com/Article/details/ghvsrvrpz.sHtML

G. 面向对象                    （第 7 节，16 个任务，128 条）
来源：http://blog.hesvh.cn/Article/details/gpubwqify.sHtML

H. 异常与错误处理              （第 8 节，10 个任务，80 条）
来源：http://www.m.share.hesvh.cn/Article/details/gjaysoosz.sHtML

I. 正则表达式                  （第 9 节，8 个任务，64 条）
来源：http://read.share.hesvh.cn/Article/details/gvxutoqcd.sHtML

J. 日期与时间                  （第 10 节，10 个任务，80 条）
来源：http://mobile.hesvh.cn/Article/details/grffhcdhs.sHtML

K. JSON 与序列化               （第 11 节，8 个任务，64 条）
来源：http://www.share.zdbjq.cn/Article/details/gjzzvduez.sHtML

L. 网络请求                    （第 12 节，8 个任务，64 条）
来源：http://3g.zdbjq.cn/Article/details/ghtdgowaf.sHtML

M. 命令行 / 进程 / 环境        （第 13 节，8 个任务，64 条）
来源：http://read.share.fehbvm.com/Article/details/gomllzcgd.sHtML


<!-- 参考信息 -->