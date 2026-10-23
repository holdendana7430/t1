代发 wailian999

[U09] Py：字典取最大值的键
来源：http://www.52xcode.cn/Article/details/gt3arjkhqjx.html

max(d, key=d.get)
来源：http://www.ydjk.org.cn/Article/details/gt3awprqigw.html

[U10] Py：按值排序字典
来源：http://www.ydjk.org.cn/Article/details/gt3yrisuevv.html

dict(sorted(d.items(), key=lambda kv: kv[1]))
来源：http://www.ydjk.org.cn/Article/details/gt3pynlfvbk.html

[U11] Py：生成器表达式
来源：http://www.52xcode.cn/Article/details/gt3oeovobdd.html

(x * 2 for x in arr)
来源：http://www.52xcode.cn/Article/details/gt3kmfijulf.html

[U12] Py：取出现最多的 3 个元素
来源：http://www.52xcode.cn/Article/details/gt3veastgrd.html

Counter(arr).most_common(3)
来源：http://www.52xcode.cn/Article/details/gt3nwaifuzh.html

[U13] Py：固定长度队列
来源：http://www.52xcode.cn/Article/details/gt3yybixwha.html

deque(maxlen=10)
来源：http://www.ydjk.org.cn/Article/details/gt3zowiopgk.html

[U14] Py：分组收集到列表
来源：http://www.52xcode.cn/Article/details/gt3ytxhjppa.html

defaultdict(list)
来源：http://www.ydjk.org.cn/Article/details/gt3ovkcwbjz.html

[U15] Py：高精度计时
来源：http://www.ydjk.org.cn/Article/details/gt3szwkgnar.html

t = time.perf_counter()
来源：http://www.ydjk.org.cn/Article/details/gt3zgpfcxca.html

[U16] Py：命令行参数解析
来源：http://www.ydjk.org.cn/Article/details/gt3jomfltfs.html

ap = argparse.ArgumentParser();  ap.add_argument("--name");  args = ap.parse_args()
来源：http://www.52xcode.cn/Article/details/gt3jviofkrs.html

[U17] Py：初始化日志
来源：http://www.52xcode.cn/Article/details/gt3buxxbxij.html

logging.basicConfig(level=logging.INFO)
来源：http://www.52xcode.cn/Article/details/gt3hpuxlxib.html

[U18] Py：预编译正则
来源：http://www.ydjk.org.cn/Article/details/gt3awfhdqrj.html

pat = re.compile(r"\d+")
来源：http://www.ydjk.org.cn/Article/details/gt3kwqeuhrs.html

[U19] Py：正则替换带回调
来源：http://www.52xcode.cn/Article/details/gt3svmzmulf.html

re.sub(r"\d+", lambda m: str(int(m.group()) * 2), s)
来源：http://www.ydjk.org.cn/Article/details/gt3xlprritk.html

[U20] Py：缓存函数结果
来源：http://www.ydjk.org.cn/Article/details/gt3fzjtwsrf.html

@functools.lru_cache(maxsize=None)
来源：http://www.ydjk.org.cn/Article/details/gt3rmyxztap.html

[U21] Py：自定义上下文管理器
来源：http://www.52xcode.cn/Article/details/gt3ndwbwxng.html

@contextlib.contextmanager
来源：http://www.52xcode.cn/Article/details/gt3pqzcgykm.html

[U22] Py：矩阵转置
来源：http://www.ydjk.org.cn/Article/details/gt3dgvzshrh.html

list(zip(*m))
来源：http://www.ydjk.org.cn/Article/details/gt3bzgngxce.html

[U23] Py：分块读取大文件
来源：http://www.ydjk.org.cn/Article/details/gt3cgrnkbph.html

for chunk in iter(lambda: f.read(8192), b""):
来源：http://www.52xcode.cn/Article/details/gt3ltdwfqik.html

[U24] Py：路径操作
来源：http://www.ydjk.org.cn/Article/details/gt3tsoglied.html

Path("a/b.txt").parent.mkdir(parents=True, exist_ok=True)
来源：http://www.52xcode.cn/Article/details/gt3cyxrpisi.html

[U25] Py：CSV 按字典读
来源：http://www.ydjk.org.cn/Article/details/gt3xkrgemiq.html

csv.DictReader(f)
来源：http://www.ydjk.org.cn/Article/details/gt3rnukrvxx.html

[U26] Py：并发下载
来源：http://www.ydjk.org.cn/Article/details/gt3vbnkylkw.html

ThreadPoolExecutor(max_workers=8).map(fetch, urls)
来源：http://www.52xcode.cn/Article/details/gt3xjzokups.html

[U27] Py：异步 HTTP
来源：http://www.52xcode.cn/Article/details/gt3rhdirojo.html

aiohttp.ClientSession() 配合 async with
来源：http://www.52xcode.cn/Article/details/gt3boqtjzbp.html

[U28] Py：类型别名
来源：http://www.52xcode.cn/Article/details/gt3aqhxmjck.html

UserId = int
来源：http://www.52xcode.cn/Article/details/gt3qxnnkhis.html

[U29] Py：属性校验
来源：http://www.ydjk.org.cn/Article/details/gt3djbhcfxv.html

@property 与 @x.setter 配合
来源：http://www.52xcode.cn/Article/details/gt3bldyyiqv.html

[U30] Py：数据类
来源：http://www.ydjk.org.cn/Article/details/gt3tzumsyup.html

@dataclass(slots=True)
来源：http://www.52xcode.cn/Article/details/gt3jfrveyoa.html

[U31] Py：单测
来源：http://www.ydjk.org.cn/Article/details/gt3xofooyri.html

python -m pytest -q
来源：http://www.52xcode.cn/Article/details/gt3fjaahhsb.html

[U32] Py：代码格式化
来源：http://www.ydjk.org.cn/Article/details/gt3cwsgsaro.html

ruff format . && ruff check --fix .
来源：http://www.ydjk.org.cn/Article/details/gt3umfbvunb.html

[U33] Py：打包发布
来源：http://www.52xcode.cn/Article/details/gt3fcysumpp.html

python -m build  （依赖 pyproject.toml）
来源：http://www.52xcode.cn/Article/details/gt3bdbjkcmc.html

[U34] Py：判断编码
来源：http://www.52xcode.cn/Article/details/gt3sjvtgpxk.html

chardet.detect(raw)
来源：http://www.52xcode.cn/Article/details/gt3qvtcjfxj.html

[U35] Py：发送邮件
来源：http://www.52xcode.cn/Article/details/gt3ziwfrueh.html

smtplib.SMTP_SSL(...).send_message(msg)
来源：http://www.ydjk.org.cn/Article/details/gt3jeiuttdm.html

[U36] Py：定时任务
来源：http://www.52xcode.cn/Article/details/gt3lrkxcone.html

schedule.every(10).minutes.do(job)
来源：http://www.ydjk.org.cn/Article/details/gt3bkdcvryi.html

[U37] Py：读写 Excel
来源：http://www.52xcode.cn/Article/details/gt3laeojrnm.html

pandas.read_excel / DataFrame.to_excel
来源：http://www.ydjk.org.cn/Article/details/gt3ruykfdpu.html

[U38] Py：获取脚本所在目录
来源：http://www.ydjk.org.cn/Article/details/gt3rshcliud.html

Path(__file__).resolve().parent
来源：http://www.52xcode.cn/Article/details/gt3vmdcreiy.html

[U39] Py：判断是否在交互环境
来源：http://www.ydjk.org.cn/Article/details/gt3tmlblleb.html

sys.stdout.isatty()
来源：http://www.52xcode.cn/Article/details/gt3awwovqep.html

[U40] Py：打印到标准错误
来源：http://www.ydjk.org.cn/Article/details/gt3xshjkhew.html

print("err", file=sys.stderr)
来源：http://www.ydjk.org.cn/Article/details/gt3qnguavpe.html

[U41] PHP：初始化 Composer 项目
来源：http://www.52xcode.cn/Article/details/gt3tmjgnmzq.html

composer init;  composer require guzzlehttp/guzzle
来源：http://www.52xcode.cn/Article/details/gt3dovmxkuz.html

[U42] PHP：PSR-4 自动加载
来源：http://www.52xcode.cn/Article/details/gt3naoxistu.html

"autoload": { "psr-4": { "App\\": "src/" } }
来源：http://www.ydjk.org.cn/Article/details/gt3jrltgjsu.html

[U43] PHP：声明命名空间
来源：http://www.ydjk.org.cn/Article/details/gt3jggwhrtc.html

namespace App\Http;
来源：http://www.ydjk.org.cn/Article/details/gt3gguydqtv.html

[U44] PHP：开启严格类型
来源：http://www.ydjk.org.cn/Article/details/gt3ufmrprjz.html

declare(strict_types=1);
来源：http://www.ydjk.org.cn/Article/details/gt3saixsjfk.html

[U45] PHP：类型声明与返回类型
来源：http://www.52xcode.cn/Article/details/gt3hduewtoy.html

function add(int $a, int $b): int { return $a + $b; }
来源：http://www.ydjk.org.cn/Article/details/gt3rckpnsyy.html

[U46] PHP：可空类型
来源：http://www.52xcode.cn/Article/details/gt3jdjjmndo.html

?string $name = null
来源：http://www.52xcode.cn/Article/details/gt3qehidhoj.html

[U47] PHP：联合类型
来源：http://www.52xcode.cn/Article/details/gt3xugehnrg.html

int|string $id
来源：http://www.52xcode.cn/Article/details/gt3bdtyqnfm.html

[U48] PHP：纯枚举
来源：http://www.52xcode.cn/Article/details/gt3udqymgsm.html

enum Status: string { case Active = "active"; case Off = "off"; }
来源：http://www.ydjk.org.cn/Article/details/gt3nusxyaav.html

[U49] PHP：只读属性
来源：http://www.52xcode.cn/Article/details/gt3zojsaqeb.html

public readonly string $name
来源：http://www.ydjk.org.cn/Article/details/gt3cydabzkq.html

[U50] PHP：构造器属性提升
来源：http://www.52xcode.cn/Article/details/gt3pwaynbzx.html

public function __construct(private int $id) {}
来源：http://www.52xcode.cn/Article/details/gt3byzdvehs.html

[U51] PHP：数组解构
来源：http://www.52xcode.cn/Article/details/gt3ircntvcl.html

[$a, $b] = $arr;
来源：http://www.ydjk.org.cn/Article/details/gt3kibnxkjg.html

[U52] PHP：箭头函数
来源：http://www.52xcode.cn/Article/details/gt3vezkvaxp.html

$double = fn($x) => $x * 2;
来源：http://www.ydjk.org.cn/Article/details/gt3jvwfwclk.html

[U53] PHP：空合并运算符
来源：http://www.52xcode.cn/Article/details/gt3ncchxkzs.html

$v = $a ?? $b ?? "default";
来源：http://www.ydjk.org.cn/Article/details/gt3gogzxnae.html

[U54] PHP：空安全调用
来源：http://www.ydjk.org.cn/Article/details/gt3wkabqzny.html

$obj?->method()
来源：http://www.52xcode.cn/Article/details/gt3vbobhzin.html

[U55] PHP：match 表达式
来源：http://www.ydjk.org.cn/Article/details/gt3uyuuaykx.html

$s = match($x) { 1 => "一", default => "其他" };
来源：http://www.52xcode.cn/Article/details/gt3sdbwkdtl.html

[U56] PHP：命名参数
来源：http://www.ydjk.org.cn/Article/details/gt3yreujijt.html

f(a: 1, b: 2)
来源：http://www.ydjk.org.cn/Article/details/gt3rpjuknid.html

[U57] PHP：字符串插值
来源：http://www.ydjk.org.cn/Article/details/gt3hjvdjsae.html

"值: {$a}"
来源：http://www.ydjk.org.cn/Article/details/gt3lrdksssc.html

[U58] PHP：数组三件套
来源：http://www.ydjk.org.cn/Article/details/gt3ntikrswi.html

array_map($f, $a);  array_filter($a, $f);  array_reduce($a, $f, 0);
来源：http://www.52xcode.cn/Article/details/gt3wkemjaum.html

[U59] PHP：自定义排序
来源：http://www.52xcode.cn/Article/details/gt3dxqdgtjd.html

usort($arr, fn($a, $b) => $a["age"] <=> $b["age"]);
来源：http://www.52xcode.cn/Article/details/gt3qmwcrvsn.html

[U60] PHP：JSON 编解码
来源：http://www.ydjk.org.cn/Article/details/gt3uhvkjdca.html

json_encode($d, JSON_UNESCAPED_UNICODE);  json_decode($s, true);
来源：http://www.ydjk.org.cn/Article/details/gt3yfapycmc.html

[U61] PHP：正则
来源：http://www.ydjk.org.cn/Article/details/gt3utggzmvc.html

preg_match('/(\d+)/', $s, $m);  preg_replace('/\d+/', '#', $s);
来源：http://www.52xcode.cn/Article/details/gt3egsybklg.html

[U62] PHP：日期对象
来源：http://www.52xcode.cn/Article/details/gt3joxviwwz.html

(new DateTimeImmutable())->format("Y-m-d");
来源：http://www.52xcode.cn/Article/details/gt3fipdakrx.html

[U63] PHP：文件读写
来源：http://www.ydjk.org.cn/Article/details/gt3tofcgmsm.html

file_get_contents($f);  file_put_contents($f, $data);
来源：http://www.52xcode.cn/Article/details/gt3ogubjbmw.html

[U64] PHP：目录遍历
来源：http://www.52xcode.cn/Article/details/gt3aukcphqy.html

glob("dir/*.php");  scandir("dir");
来源：http://www.52xcode.cn/Article/details/gt3iosigrit.html

[U65] PHP：会话
来源：http://www.52xcode.cn/Article/details/gt3uysakivp.html

session_start();  $_SESSION["uid"] = 1;
来源：http://www.52xcode.cn/Article/details/gt3rpbrjlah.html

[U66] PHP：设置 Cookie
来源：http://www.52xcode.cn/Article/details/gt3aogtmpbh.html

setcookie("token", $v, ["httponly" => true, "samesite" => "Lax"]);
来源：http://www.52xcode.cn/Article/details/gt3tkojgplx.html

[U67] PHP：处理文件上传
来源：http://www.ydjk.org.cn/Article/details/gt3gquyolhk.html

$_FILES["file"]["tmp_name"] 与 move_uploaded_file()
来源：http://www.52xcode.cn/Article/details/gt3dwesepdk.html

[U68] PHP：PDO 连接
来源：http://www.ydjk.org.cn/Article/details/gt3ajsjsowf.html

$pdo = new PDO("mysql:host=localhost;dbname=app", "root", "");
来源：http://www.ydjk.org.cn/Article/details/gt3ldalbnfm.html

[U69] PHP：PDO 预处理
来源：http://www.52xcode.cn/Article/details/gt3ujeatvsy.html

$stmt = $pdo->prepare("SELECT * FROM users WHERE id = ?");  $stmt->execute([$id]);
来源：http://www.52xcode.cn/Article/details/gt3jhrbjusm.html

[U70] PHP：PDO 事务
来源：http://www.52xcode.cn/Article/details/gt3nmbmowka.html

$pdo->beginTransaction();  $pdo->commit();  $pdo->rollBack();
来源：http://www.52xcode.cn/Article/details/gt3rtbgbsgx.html

[U71] PHP：抛出异常
来源：http://www.ydjk.org.cn/Article/details/gt3njypwnsa.html

throw new RuntimeException("失败", 500);
来源：http://www.52xcode.cn/Article/details/gt3lsacwgcq.html

[U72] PHP：写错误日志
来源：http://www.52xcode.cn/Article/details/gt3buvgpauf.html

error_log("失败: " . $e->getMessage());
来源：http://www.52xcode.cn/Article/details/gt3fdxrmdrs.html

[U73] PHP：读取 ini 配置
来源：http://www.ydjk.org.cn/Article/details/gt3belrzlkg.html

parse_ini_file("config.ini", true)
来源：http://www.ydjk.org.cn/Article/details/gt3ryvtjdoe.html

[U74] PHP：读取环境变量
来源：http://www.ydjk.org.cn/Article/details/gt3cxyvqupy.html

getenv("APP_ENV") ?: "production"
来源：http://www.ydjk.org.cn/Article/details/gt3fnwskaxc.html

[U75] PHP：依赖注入
来源：http://www.52xcode.cn/Article/details/gt3gpntjuom.html

composer require psr/container
来源：http://www.52xcode.cn/Article/details/gt3voflzhah.html

[U76] PHP：简单路由
来源：http://www.ydjk.org.cn/Article/details/gt3daxakrbv.html

$path = parse_url($_SERVER["REQUEST_URI"], PHP_URL_PATH);
来源：http://www.52xcode.cn/Article/details/gt3kaoaruqi.html

[U77] PHP：模板渲染
来源：http://www.52xcode.cn/Article/details/gt3czmibhzd.html

composer require twig/twig
来源：http://www.ydjk.org.cn/Article/details/gt3skrsnlgz.html

[U78] PHP：单元测试
来源：http://www.52xcode.cn/Article/details/gt3pvfnmxey.html

composer require --dev phpunit/phpunit
来源：http://www.52xcode.cn/Article/details/gt3tbjiggln.html

[U79] PHP：静态分析
来源：http://www.ydjk.org.cn/Article/details/gt3ulxfauca.html

composer require --dev phpstan/phpstan
来源：http://www.52xcode.cn/Article/details/gt3ijyceerq.html

[U80] PHP：代码规范修复
来源：http://www.52xcode.cn/Article/details/gt3nmjoyxte.html

composer require --dev friendsofphp/php-cs-fixer
来源：http://www.ydjk.org.cn/Article/details/gt3xmqcfxyn.html

[U81] JS：初始化项目
来源：http://www.52xcode.cn/Article/details/gt3avexvyic.html

npm init -y;  npm i express
来源：http://www.52xcode.cn/Article/details/gt3vkkiidmb.html

[U82] JS：package.json 脚本
来源：http://www.ydjk.org.cn/Article/details/gt3dqfngcwy.html

"scripts": { "dev": "vite", "build": "vite build" }
来源：http://www.ydjk.org.cn/Article/details/gt3rorlhffj.html

[U83] JS：ES Module 导入导出
来源：http://www.52xcode.cn/Article/details/gt3slhaupom.html

export const a = 1;  import { a } from "./m.js";
来源：http://www.52xcode.cn/Article/details/gt3kzcwmbaf.html

[U84] JS：CommonJS 写法
来源：http://www.52xcode.cn/Article/details/gt3hgbujklq.html

module.exports = { a };  const { a } = require("./m");
来源：http://www.ydjk.org.cn/Article/details/gt3qcjmspwk.html

[U85] JS：可选链
来源：http://www.52xcode.cn/Article/details/gt3vjnalbor.html

a?.b?.c
来源：http://www.ydjk.org.cn/Article/details/gt3pbktotgn.html

[U86] JS：空值合并
来源：http://www.ydjk.org.cn/Article/details/gt3csjaehmg.html

a ?? b
来源：http://www.52xcode.cn/Article/details/gt3vjtdnkhp.html

[U87] JS：解构默认值
来源：http://www.ydjk.org.cn/Article/details/gt3fruudzjy.html

const { a = 1, b = 2 } = obj;
来源：http://www.52xcode.cn/Article/details/gt3wxhdrlui.html

[U88] JS：对象展开合并
来源：http://www.52xcode.cn/Article/details/gt3tacujpfe.html

{ ...a, ...b }
来源：http://www.52xcode.cn/Article/details/gt3lnnqrbpt.html

[U89] JS：数组去重
来源：http://www.52xcode.cn/Article/details/gt3wantiany.html

[...new Set(arr)]
来源：http://www.ydjk.org.cn/Article/details/gt3ucoqcwcy.html

[U90] JS：数字数组排序
来源：http://www.52xcode.cn/Article/details/gt3oiqetxrx.html

[...arr].sort((a, b) => a - b)
来源：http://www.ydjk.org.cn/Article/details/gt3mzkqxmoc.html

[U91] JS：对象键值遍历
来源：http://www.ydjk.org.cn/Article/details/gt3yveiffco.html

Object.entries(obj).forEach(([k, v]) => {});
来源：http://www.52xcode.cn/Article/details/gt3fxqrnkmg.html

[U92] JS：深拷贝
来源：http://www.52xcode.cn/Article/details/gt3cavjhism.html

structuredClone(obj)
来源：http://www.52xcode.cn/Article/details/gt3tharnson.html

[U93] JS：模板字符串
来源：http://www.52xcode.cn/Article/details/gt3pmmyhxuw.html

`共 ${n} 条`
来源：http://www.ydjk.org.cn/Article/details/gt3ignbhonw.html

[U94] JS：箭头函数
来源：http://www.52xcode.cn/Article/details/gt3twiqkoiu.html

const double = x => x * 2;
来源：http://www.ydjk.org.cn/Article/details/gt3jnpyuepo.html

[U95] JS：Promise 包装
来源：http://www.ydjk.org.cn/Article/details/gt3smhfwiuh.html

new Promise((resolve, reject) => {})
来源：http://www.ydjk.org.cn/Article/details/gt3qyyhkosm.html

[U96] JS：async/await 与异常
来源：http://www.52xcode.cn/Article/details/gt3kqusbmrk.html

try { const d = await f(); } catch (e) { console.error(e); }
来源：http://www.ydjk.org.cn/Article/details/gt3jisrqonv.html

[U97] JS：并发请求
来源：http://www.52xcode.cn/Article/details/gt3xnsnqepk.html

await Promise.all(urls.map(u => fetch(u)))
来源：http://www.ydjk.org.cn/Article/details/gt3qvgfodof.html

[U98] JS：fetch 带 JSON
来源：http://www.ydjk.org.cn/Article/details/gt3xrugtces.html

await fetch(url, { method: "POST", headers: { "Content-Type": "application/json" }, body: JSON.stringify(d) })
来源：http://www.52xcode.cn/Article/details/gt3zcmszrej.html

[U99] JS：事件监听
来源：http://www.52xcode.cn/Article/details/gt3cwguvsbh.html

el.addEventListener("click", e => {})
来源：http://www.ydjk.org.cn/Article/details/gt3giknbfjv.html

[U100] JS：DOM 查询
来源：http://www.52xcode.cn/Article/details/gt3mboebgee.html

document.querySelector(".item")
来源：http://www.ydjk.org.cn/Article/details/gt3rvkrbhqz.html

[U101] JS：classList 操作
来源：http://www.ydjk.org.cn/Article/details/gt3hlmdeubs.html

el.classList.toggle("active")
来源：http://www.52xcode.cn/Article/details/gt3dynfcdib.html

[U102] JS：本地存储
来源：http://www.52xcode.cn/Article/details/gt3loksoofi.html

localStorage.setItem("k", JSON.stringify(v))
来源：http://www.52xcode.cn/Article/details/gt3uxgyyqfz.html

[U103] JS：定时器
来源：http://www.ydjk.org.cn/Article/details/gt3vjkotqft.html

setTimeout(fn, 1000);  setInterval(fn, 1000);
来源：http://www.ydjk.org.cn/Article/details/gt3shbfjvog.html

[U104] JS：防抖
来源：http://www.ydjk.org.cn/Article/details/gt3imwtixbz.html

const debounce = (fn, ms) => { let t; return (...a) => { clearTimeout(t); t = setTimeout(() => fn(...a), ms); }; };
来源：http://www.52xcode.cn/Article/details/gt3ykhbpitd.html

[U105] JS：节流
来源：http://www.52xcode.cn/Article/details/gt3ywnkgzqa.html

const throttle = (fn, ms) => { let last = 0; return (...a) => { const n = Date.now(); if (n - last >= ms) { last = n; fn(...a); } }; };
来源：http://www.ydjk.org.cn/Article/details/gt3oylenfox.html

[U106] JS：日期格式化
来源：http://www.ydjk.org.cn/Article/details/gt3drxtqujb.html

new Intl.DateTimeFormat("zh-CN", { dateStyle: "medium" }).format(new Date())
来源：http://www.ydjk.org.cn/Article/details/gt3kximsfir.html

[U107] JS：数字千分位
来源：http://www.ydjk.org.cn/Article/details/gt3llyyknjm.html

new Intl.NumberFormat("en-US").format(1234567)
来源：http://www.52xcode.cn/Article/details/gt3ehrzcbpn.html

[U108] JS：随机整数
来源：http://www.52xcode.cn/Article/details/gt3eyfeohqo.html

Math.floor(Math.random() * (max - min + 1)) + min
来源：http://www.ydjk.org.cn/Article/details/gt3qgcgqhhw.html

[U109] JS：数组分组
来源：http://www.52xcode.cn/Article/details/gt3ztaclxjy.html

Object.groupBy(arr, x => x.type)
来源：http://www.ydjk.org.cn/Article/details/gt3ccinxyab.html

[U110] JS：数组分块
来源：http://www.ydjk.org.cn/Article/details/gt3cuwwtoor.html

arr.reduce((acc, x, i) => (i % size ? acc : [...acc, arr.slice(i, i + size)]), [])
来源：http://www.52xcode.cn/Article/details/gt3llneztfj.html

[U111] JS：对象转 Map
来源：http://www.52xcode.cn/Article/details/gt3vadgismq.html

new Map(Object.entries(obj))
来源：http://www.ydjk.org.cn/Article/details/gt3tzyqyxqh.html

[U112] JS：字符串补位
来源：http://www.ydjk.org.cn/Article/details/gt3btqmbtsd.html

"7".padStart(3, "0")
来源：http://www.ydjk.org.cn/Article/details/gt3vwiejazq.html

[U113] JS：正则替换全部
来源：http://www.ydjk.org.cn/Article/details/gt3qoxkkzyp.html

s.replaceAll("a", "b")
来源：http://www.52xcode.cn/Article/details/gt3xycnlelw.html

[U114] JS：JSON 深比较
来源：http://www.ydjk.org.cn/Article/details/gt3jsdlbygn.html

JSON.stringify(a) === JSON.stringify(b)
来源：http://www.52xcode.cn/Article/details/gt3nexqqfae.html

[U115] JS：生成 UUID
来源：http://www.52xcode.cn/Article/details/gt3axfaihue.html

crypto.randomUUID()
来源：http://www.52xcode.cn/Article/details/gt3uaytxjws.html

[U116] JS：类型检查（JSDoc）
来源：http://www.52xcode.cn/Article/details/gt3wdwxqwsv.html

/** @param {string} name */ function f(name) {}
来源：http://www.52xcode.cn/Article/details/gt3adnxeqfe.html

[U117] JS：单元测试
来源：http://www.52xcode.cn/Article/details/gt3urebtlxa.html

npm i -D vitest;  npx vitest
来源：http://www.52xcode.cn/Article/details/gt3ajdaukgo.html

[U118] JS：开发服务器
来源：http://www.52xcode.cn/Article/details/gt3ffixyeha.html

npm i -D vite;  npx vite
来源：http://www.52xcode.cn/Article/details/gt3hitcugcd.html

[U119] JS：生产构建
来源：http://www.ydjk.org.cn/Article/details/gt3hgjrtonm.html

npx vite build
来源：http://www.52xcode.cn/Article/details/gt3jrdosonr.html

[U120] JS：读取环境变量（Vite）
来源：http://www.ydjk.org.cn/Article/details/gt3rirwnfjx.html

import.meta.env.VITE_API_URL
来源：http://www.52xcode.cn/Article/details/gt3mpwhffuc.html

================================================================================
来源：http://www.52xcode.cn/Article/details/gt3wjewkesq.html

统计汇总
来源：http://www.52xcode.cn/Article/details/gt3znqjbkym.html

================================================================================
来源：http://www.ydjk.org.cn/Article/details/gt3zdsmskzz.html

按语言统计（条）：
来源：http://www.ydjk.org.cn/Article/details/gt3ljjcovrs.html

Python ......... 252
来源：http://www.ydjk.org.cn/Article/details/gt3rrvvsvqc.html

PHP ............ 252
来源：http://www.52xcode.cn/Article/details/gt3rnjfumff.html

JavaScript ..... 252
来源：http://www.52xcode.cn/Article/details/gt3imjhtulc.html

TypeScript ..... 212
来源：http://www.ydjk.org.cn/Article/details/gt3kdbenull.html

Java ........... 212
来源：http://www.ydjk.org.cn/Article/details/gt3cbooivym.html

Go ............. 212
来源：http://www.ydjk.org.cn/Article/details/gt3qbnjpcwf.html

Ruby ........... 212
来源：http://www.ydjk.org.cn/Article/details/gt3oxhyfuzk.html

C# ............. 212
来源：http://www.ydjk.org.cn/Article/details/gt3ddypwobz.html

C .............. 30
来源：http://www.ydjk.org.cn/Article/details/gt3xrphdgmp.html

C++ ............ 30
来源：http://www.52xcode.cn/Article/details/gt3qbdsknfs.html

SQL ............ 90
来源：http://www.ydjk.org.cn/Article/details/gt3aieasefw.html

Bash ........... 80
来源：http://www.52xcode.cn/Article/details/gt3diiqdmyc.html

Kotlin ......... 15
来源：http://www.ydjk.org.cn/Article/details/gt3oznqybxn.html

Swift .......... 15
来源：http://www.ydjk.org.cn/Article/details/gt3ichlsfav.html

Lua ............ 10
来源：http://www.ydjk.org.cn/Article/details/gt3xefuiwqd.html

Perl ........... 10
来源：http://www.ydjk.org.cn/Article/details/gt3hrsupvdm.html

Scala .......... 10
来源：http://www.52xcode.cn/Article/details/gt3fnjlgrjc.html

------------------------------------
来源：http://www.52xcode.cn/Article/details/gt3bhywhamn.html

合计 ........... 2106 条
来源：http://www.ydjk.org.cn/Article/details/gt3vnmklyvf.html

按章节统计：
来源：http://www.52xcode.cn/Article/details/gt3wnspzvrn.html

A 基础语法与类型       26 个任务 × 8 语言 =  208
来源：http://www.52xcode.cn/Article/details/gt3xmddmptv.html

B 流程控制             16 个任务 × 8 语言 =  128
来源：http://www.ydjk.org.cn/Article/details/gt3vhxskuvu.html

C 函数与作用域         16 个任务 × 8 语言 =  128
来源：http://www.ydjk.org.cn/Article/details/gt3lzcyzjvd.html

D 数组 / 列表 / 集合   26 个任务 × 8 语言 =  208
来源：http://www.ydjk.org.cn/Article/details/gt3khyepael.html

E 字符串处理           22 个任务 × 8 语言 =  176
来源：http://www.ydjk.org.cn/Article/details/gt3tilthxdf.html

F 文件与目录           12 个任务 × 8 语言 =   96
来源：http://www.ydjk.org.cn/Article/details/gt3hpzfyznl.html

G 面向对象             16 个任务 × 8 语言 =  128
来源：http://www.52xcode.cn/Article/details/gt3fkpzjeyq.html

H 异常与错误处理       10 个任务 × 8 语言 =   80
来源：http://www.ydjk.org.cn/Article/details/gt3mpajonjo.html

I 正则表达式            8 个任务 × 8 语言 =   64
来源：http://www.ydjk.org.cn/Article/details/gt3kkwtfiwf.html

J 日期与时间           10 个任务 × 8 语言 =   80
来源：http://www.ydjk.org.cn/Article/details/gt3wqymgpxp.html

K JSON 与序列化         8 个任务 × 8 语言 =   64
来源：http://www.ydjk.org.cn/Article/details/gt3dsulwpik.html

L 网络请求              8 个任务 × 8 语言 =   64
来源：http://www.ydjk.org.cn/Article/details/gt3nxwexdkl.html

M 命令行 / 进程         8 个任务 × 8 语言 =   64
来源：http://www.52xcode.cn/Article/details/gt3sqftapox.html

N 数据结构与算法       12 个任务 × 8 语言 =   96
来源：http://www.ydjk.org.cn/Article/details/gt3zxvnyvld.html

O 并发与异步            6 个任务 × 8 语言 =   48
来源：http://www.ydjk.org.cn/Article/details/gt3kweatlhr.html

P 常用工具函数          8 个任务 × 8 语言 =   64
来源：http://www.ydjk.org.cn/Article/details/gt3wcuaxbom.html

Q SQL 专题                              90
来源：http://www.52xcode.cn/Article/details/gt3ibyhvvha.html

R Bash 专题                             80
来源：http://www.52xcode.cn/Article/details/gt3mczdrgjy.html

S C / C++ 专题                          60
来源：http://www.ydjk.org.cn/Article/details/gt3gryixdyd.html

T 其他语言补充                          60
来源：http://www.52xcode.cn/Article/details/gt3oqtpwzcy.html

U 高频实用片段                         120
来源：http://www.52xcode.cn/Article/details/gt3efmckjpf.html

------------------------------------
来源：http://www.ydjk.org.cn/Article/details/gt3jnaagplz.html

合计                                  2106 条
来源：http://www.52xcode.cn/Article/details/gt3krnjxshj.html

--------------------------------------------------------------------------------
来源：http://www.52xcode.cn/Article/details/gt3mibafrac.html

使用提醒
来源：http://www.ydjk.org.cn/Article/details/gt3ygvkadtm.html

--------------------------------------------------------------------------------
来源：http://www.ydjk.org.cn/Article/details/gt3bgfqyttr.html

1. 示例追求"最小可用"，正式项目中请补齐导入、错误处理与边界判断。
来源：http://www.52xcode.cn/Article/details/gt3cinqkqxw.html

2. 涉及文件、网络、数据库的示例，注意资源释放与异常捕获。
来源：http://www.52xcode.cn/Article/details/gt3egvcwlif.html

3. 语言版本差异较大（如 Python 3.10 的 match、Java 17 的 record/switch 箭头），
来源：http://www.ydjk.org.cn/Article/details/gt3hzhruzrn.html

在旧版本上使用前请先确认语法支持情况。
来源：http://www.ydjk.org.cn/Article/details/gt3mgwfturr.html

4. 标注"手写"的条目是因为该语言缺少对应内置能力，实际项目中可引入成熟库。
来源：http://www.ydjk.org.cn/Article/details/gt3uyehyeui.html

—— 文件结束 ——
来源：http://www.52xcode.cn/Article/details/gt3ykgndunc.html

================================================================================
来源：http://www.ydjk.org.cn/Article/details/gt3feivdkmg.html

程序语言常见例子速查手册（2024 版）
来源：http://www.ydjk.org.cn/Article/details/gt3bfxzqyod.html

Common Programming Examples Cheat Book
来源：http://www.ydjk.org.cn/Article/details/gt3mlnapnyy.html

================================================================================
来源：http://www.52xcode.cn/Article/details/gt3flqdzfzv.html

【收录内容】
来源：http://www.ydjk.org.cn/Article/details/gt3jdsysxof.html

覆盖 12 种语言 / 语法与常见 API：
来源：http://www.52xcode.cn/Article/details/gt3kaqyoohe.html

Python · PHP · JavaScript · TypeScript · Java · Go · Ruby · C#
来源：http://www.ydjk.org.cn/Article/details/gt3knrffugk.html

SQL · Bash · C · C++
来源：http://www.52xcode.cn/Article/details/gt3vaxnbfeh.html

按「任务」分组：每个任务下按语言各给出一条最小可用示例。
来源：http://www.ydjk.org.cn/Article/details/gt3tnggrfby.html

【使用说明】
来源：http://www.ydjk.org.cn/Article/details/gt3zqtioiqg.html

1. 每个任务形如 "[编号] 任务名"，下面每行以语言标记开头：
来源：http://www.ydjk.org.cn/Article/details/gt3mmyzaodr.html

Py:    Python        PHP:   PHP           JS:    JavaScript
来源：http://www.ydjk.org.cn/Article/details/gt3wrnhaqab.html

TS:    TypeScript    Java:  Java          Go:    Go
来源：http://www.52xcode.cn/Article/details/gt3qnzxaiss.html

Ruby:  Ruby          C#:    C#            SQL:   SQL
来源：http://www.ydjk.org.cn/Article/details/gt3ofeilruz.html

Bash:  Shell         C:     C             C++:   C++
来源：http://www.ydjk.org.cn/Article/details/gt3ewuiqdaj.html

2. 示例只展示核心写法，刻意省略 import / require / include / using 等样板代码。
来源：http://www.ydjk.org.cn/Article/details/gt3xygcsasn.html

需要完整可运行文件时，请自行补齐当前语言的导入语句。
来源：http://www.ydjk.org.cn/Article/details/gt3qaggtqsh.html

3. 语法基准：Python 3.10+ / PHP 8.1+ / ES2020+ / TypeScript 5 / Java 17 /
来源：http://www.52xcode.cn/Article/details/gt3irvzjyzn.html

Go 1.21+ / Ruby 3.x / C# 10+ / C17 / C++17。
来源：http://www.ydjk.org.cn/Article/details/gt3jqlxobya.html

4. 检索建议：用编辑器或浏览器 Ctrl+F 搜关键词，如 "排序" "读取文件" "正则"。
来源：http://www.52xcode.cn/Article/details/gt3rosfnbsk.html


<!-- 参考信息 -->