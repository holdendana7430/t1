代发 wailian999

[U09] Py：字典取最大值的键
来源：http://www.ydjk.org.cn/Article/details/gt3cbfdtdrj.html

max(d, key=d.get)
来源：http://www.ydjk.org.cn/Article/details/gt3qgndtiwh.html

[U10] Py：按值排序字典
来源：http://www.ydjk.org.cn/Article/details/gt3vmqqsxmv.html

dict(sorted(d.items(), key=lambda kv: kv[1]))
来源：http://www.ydjk.org.cn/Article/details/gt3ofwucbxj.html

[U11] Py：生成器表达式
来源：http://www.ydjk.org.cn/Article/details/gt3cwvnoexd.html

(x * 2 for x in arr)
来源：http://www.52xcode.cn/Article/details/gt3rnhcdrjv.html

[U12] Py：取出现最多的 3 个元素
来源：http://www.52xcode.cn/Article/details/gt3wxaihvnf.html

Counter(arr).most_common(3)
来源：http://www.ydjk.org.cn/Article/details/gt3zogrvrbj.html

[U13] Py：固定长度队列
来源：http://www.ydjk.org.cn/Article/details/gt3fpgvduzc.html

deque(maxlen=10)
来源：http://www.ydjk.org.cn/Article/details/gt3gjcmychk.html

[U14] Py：分组收集到列表
来源：http://www.52xcode.cn/Article/details/gt3wuzknbsy.html

defaultdict(list)
来源：http://www.52xcode.cn/Article/details/gt3svzgclmv.html

[U15] Py：高精度计时
来源：http://www.ydjk.org.cn/Article/details/gt3sqorcjva.html

t = time.perf_counter()
来源：http://www.ydjk.org.cn/Article/details/gt3praxcxrr.html

[U16] Py：命令行参数解析
来源：http://www.ydjk.org.cn/Article/details/gt3htjbqcgu.html

ap = argparse.ArgumentParser();  ap.add_argument("--name");  args = ap.parse_args()
来源：http://www.ydjk.org.cn/Article/details/gt3wggmxesn.html

[U17] Py：初始化日志
来源：http://www.52xcode.cn/Article/details/gt3reupohdq.html

logging.basicConfig(level=logging.INFO)
来源：http://www.52xcode.cn/Article/details/gt3obbubnlv.html

[U18] Py：预编译正则
来源：http://www.52xcode.cn/Article/details/gt3uopgyiti.html

pat = re.compile(r"\d+")
来源：http://www.ydjk.org.cn/Article/details/gt3iqzilraf.html

[U19] Py：正则替换带回调
来源：http://www.ydjk.org.cn/Article/details/gt3grwuqfht.html

re.sub(r"\d+", lambda m: str(int(m.group()) * 2), s)
来源：http://www.ydjk.org.cn/Article/details/gt3aonwjzml.html

[U20] Py：缓存函数结果
来源：http://www.52xcode.cn/Article/details/gt3slupwtoq.html

@functools.lru_cache(maxsize=None)
来源：http://www.ydjk.org.cn/Article/details/gt3pfkrnpve.html

[U21] Py：自定义上下文管理器
来源：http://www.52xcode.cn/Article/details/gt3borwkzci.html

@contextlib.contextmanager
来源：http://www.ydjk.org.cn/Article/details/gt3sdimoepk.html

[U22] Py：矩阵转置
来源：http://www.52xcode.cn/Article/details/gt3krywkrsi.html

list(zip(*m))
来源：http://www.ydjk.org.cn/Article/details/gt3ehcvouna.html

[U23] Py：分块读取大文件
来源：http://www.ydjk.org.cn/Article/details/gt3xwlgvdmc.html

for chunk in iter(lambda: f.read(8192), b""):
来源：http://www.52xcode.cn/Article/details/gt3uuizvxus.html

[U24] Py：路径操作
来源：http://www.ydjk.org.cn/Article/details/gt3ydxohljk.html

Path("a/b.txt").parent.mkdir(parents=True, exist_ok=True)
来源：http://www.52xcode.cn/Article/details/gt3bgqugeeg.html

[U25] Py：CSV 按字典读
来源：http://www.ydjk.org.cn/Article/details/gt3bxbskfxs.html

csv.DictReader(f)
来源：http://www.ydjk.org.cn/Article/details/gt3qwtvyidi.html

[U26] Py：并发下载
来源：http://www.52xcode.cn/Article/details/gt3eshlgccc.html

ThreadPoolExecutor(max_workers=8).map(fetch, urls)
来源：http://www.52xcode.cn/Article/details/gt3utrfyaxe.html

[U27] Py：异步 HTTP
来源：http://www.52xcode.cn/Article/details/gt3ugezvkuf.html

aiohttp.ClientSession() 配合 async with
来源：http://www.ydjk.org.cn/Article/details/gt3xlkncepo.html

[U28] Py：类型别名
来源：http://www.ydjk.org.cn/Article/details/gt3afkvuoee.html

UserId = int
来源：http://www.ydjk.org.cn/Article/details/gt3lzmyqzij.html

[U29] Py：属性校验
来源：http://www.52xcode.cn/Article/details/gt3ydokhdxa.html

@property 与 @x.setter 配合
来源：http://www.ydjk.org.cn/Article/details/gt3kkchkbhc.html

[U30] Py：数据类
来源：http://www.ydjk.org.cn/Article/details/gt3pdlmrhol.html

@dataclass(slots=True)
来源：http://www.ydjk.org.cn/Article/details/gt3fabycogb.html

[U31] Py：单测
来源：http://www.ydjk.org.cn/Article/details/gt3aibkjruv.html

python -m pytest -q
来源：http://www.ydjk.org.cn/Article/details/gt3mgcjsmla.html

[U32] Py：代码格式化
来源：http://www.52xcode.cn/Article/details/gt3vgudgtng.html

ruff format . && ruff check --fix .
来源：http://www.52xcode.cn/Article/details/gt3yomkcjve.html

[U33] Py：打包发布
来源：http://www.52xcode.cn/Article/details/gt3xhvfycxd.html

python -m build  （依赖 pyproject.toml）
来源：http://www.ydjk.org.cn/Article/details/gt3gjinmukr.html

[U34] Py：判断编码
来源：http://www.ydjk.org.cn/Article/details/gt3tlngdquy.html

chardet.detect(raw)
来源：http://www.ydjk.org.cn/Article/details/gt3yvowtdia.html

[U35] Py：发送邮件
来源：http://www.ydjk.org.cn/Article/details/gt3gyiuutmc.html

smtplib.SMTP_SSL(...).send_message(msg)
来源：http://www.ydjk.org.cn/Article/details/gt3kxmyhqrt.html

[U36] Py：定时任务
来源：http://www.ydjk.org.cn/Article/details/gt3glisusos.html

schedule.every(10).minutes.do(job)
来源：http://www.ydjk.org.cn/Article/details/gt3aqkpjkch.html

[U37] Py：读写 Excel
来源：http://www.52xcode.cn/Article/details/gt3ihuqjkrr.html

pandas.read_excel / DataFrame.to_excel
来源：http://www.52xcode.cn/Article/details/gt3ghymirez.html

[U38] Py：获取脚本所在目录
来源：http://www.52xcode.cn/Article/details/gt3sylqtmky.html

Path(__file__).resolve().parent
来源：http://www.52xcode.cn/Article/details/gt3wbmenhps.html

[U39] Py：判断是否在交互环境
来源：http://www.ydjk.org.cn/Article/details/gt3optvgzou.html

sys.stdout.isatty()
来源：http://www.ydjk.org.cn/Article/details/gt3ohimlrow.html

[U40] Py：打印到标准错误
来源：http://www.ydjk.org.cn/Article/details/gt3rdvlkfle.html

print("err", file=sys.stderr)
来源：http://www.ydjk.org.cn/Article/details/gt3xkzdarzd.html

[U41] PHP：初始化 Composer 项目
来源：http://www.ydjk.org.cn/Article/details/gt3njikxglk.html

composer init;  composer require guzzlehttp/guzzle
来源：http://www.52xcode.cn/Article/details/gt3icvwuwce.html

[U42] PHP：PSR-4 自动加载
来源：http://www.ydjk.org.cn/Article/details/gt3ncgoakyf.html

"autoload": { "psr-4": { "App\\": "src/" } }
来源：http://www.52xcode.cn/Article/details/gt3dfjdyyth.html

[U43] PHP：声明命名空间
来源：http://www.ydjk.org.cn/Article/details/gt3ibblsaex.html

namespace App\Http;
来源：http://www.ydjk.org.cn/Article/details/gt3zbtnlkpi.html

[U44] PHP：开启严格类型
来源：http://www.52xcode.cn/Article/details/gt3mjwvnzke.html

declare(strict_types=1);
来源：http://www.ydjk.org.cn/Article/details/gt3cyrenhod.html

[U45] PHP：类型声明与返回类型
来源：http://www.ydjk.org.cn/Article/details/gt3uqbahjsg.html

function add(int $a, int $b): int { return $a + $b; }
来源：http://www.52xcode.cn/Article/details/gt3dhhoofki.html

[U46] PHP：可空类型
来源：http://www.ydjk.org.cn/Article/details/gt3xaoallud.html

?string $name = null
来源：http://www.ydjk.org.cn/Article/details/gt3ehltqlen.html

[U47] PHP：联合类型
来源：http://www.52xcode.cn/Article/details/gt3ytzqthcr.html

int|string $id
来源：http://www.52xcode.cn/Article/details/gt3wgqtcpbi.html

[U48] PHP：纯枚举
来源：http://www.52xcode.cn/Article/details/gt3yuteuryp.html

enum Status: string { case Active = "active"; case Off = "off"; }
来源：http://www.52xcode.cn/Article/details/gt3qkmhzbsr.html

[U49] PHP：只读属性
来源：http://www.52xcode.cn/Article/details/gt3vgtntggq.html

public readonly string $name
来源：http://www.52xcode.cn/Article/details/gt3tmtcwfrn.html

[U50] PHP：构造器属性提升
来源：http://www.ydjk.org.cn/Article/details/gt3qfoylsxn.html

public function __construct(private int $id) {}
来源：http://www.ydjk.org.cn/Article/details/gt3zlnoyorx.html

[U51] PHP：数组解构
来源：http://www.ydjk.org.cn/Article/details/gt3cozmzkmc.html

[$a, $b] = $arr;
来源：http://www.ydjk.org.cn/Article/details/gt3otkfusoc.html

[U52] PHP：箭头函数
来源：http://www.ydjk.org.cn/Article/details/gt3dibhsvii.html

$double = fn($x) => $x * 2;
来源：http://www.52xcode.cn/Article/details/gt3zwjpizdm.html

[U53] PHP：空合并运算符
来源：http://www.ydjk.org.cn/Article/details/gt3zbmbxmqu.html

$v = $a ?? $b ?? "default";
来源：http://www.52xcode.cn/Article/details/gt3ftpojvvs.html

[U54] PHP：空安全调用
来源：http://www.ydjk.org.cn/Article/details/gt3fqgricju.html

$obj?->method()
来源：http://www.52xcode.cn/Article/details/gt3leopxilh.html

[U55] PHP：match 表达式
来源：http://www.ydjk.org.cn/Article/details/gt3exehcwfz.html

$s = match($x) { 1 => "一", default => "其他" };
来源：http://www.ydjk.org.cn/Article/details/gt3yhpudwwk.html

[U56] PHP：命名参数
来源：http://www.ydjk.org.cn/Article/details/gt3jnvipjwj.html

f(a: 1, b: 2)
来源：http://www.52xcode.cn/Article/details/gt3fhdirngo.html

[U57] PHP：字符串插值
来源：http://www.52xcode.cn/Article/details/gt3ycjgldsv.html

"值: {$a}"
来源：http://www.52xcode.cn/Article/details/gt3ivctpuzn.html

[U58] PHP：数组三件套
来源：http://www.ydjk.org.cn/Article/details/gt3kkbikprk.html

array_map($f, $a);  array_filter($a, $f);  array_reduce($a, $f, 0);
来源：http://www.ydjk.org.cn/Article/details/gt3gueehvxt.html

[U59] PHP：自定义排序
来源：http://www.52xcode.cn/Article/details/gt3yxwwlkpi.html

usort($arr, fn($a, $b) => $a["age"] <=> $b["age"]);
来源：http://www.ydjk.org.cn/Article/details/gt3ymzkvzbd.html

[U60] PHP：JSON 编解码
来源：http://www.52xcode.cn/Article/details/gt3xquenjde.html

json_encode($d, JSON_UNESCAPED_UNICODE);  json_decode($s, true);
来源：http://www.52xcode.cn/Article/details/gt3hpmxqmua.html

[U61] PHP：正则
来源：http://www.ydjk.org.cn/Article/details/gt3vouvbeen.html

preg_match('/(\d+)/', $s, $m);  preg_replace('/\d+/', '#', $s);
来源：http://www.ydjk.org.cn/Article/details/gt3avgcyxey.html

[U62] PHP：日期对象
来源：http://www.ydjk.org.cn/Article/details/gt3havuszcw.html

(new DateTimeImmutable())->format("Y-m-d");
来源：http://www.ydjk.org.cn/Article/details/gt3imivhlwy.html

[U63] PHP：文件读写
来源：http://www.52xcode.cn/Article/details/gt3vnuoqknh.html

file_get_contents($f);  file_put_contents($f, $data);
来源：http://www.52xcode.cn/Article/details/gt3mdaqtlxw.html

[U64] PHP：目录遍历
来源：http://www.ydjk.org.cn/Article/details/gt3hworfukm.html

glob("dir/*.php");  scandir("dir");
来源：http://www.52xcode.cn/Article/details/gt3qbsfnzuh.html

[U65] PHP：会话
来源：http://www.52xcode.cn/Article/details/gt3ekkdlyff.html

session_start();  $_SESSION["uid"] = 1;
来源：http://www.ydjk.org.cn/Article/details/gt3onajhddq.html

[U66] PHP：设置 Cookie
来源：http://www.ydjk.org.cn/Article/details/gt3ueaeiwcx.html

setcookie("token", $v, ["httponly" => true, "samesite" => "Lax"]);
来源：http://www.52xcode.cn/Article/details/gt3jzesythl.html

[U67] PHP：处理文件上传
来源：http://www.ydjk.org.cn/Article/details/gt3qvztzahi.html

$_FILES["file"]["tmp_name"] 与 move_uploaded_file()
来源：http://www.ydjk.org.cn/Article/details/gt3yevtkbde.html

[U68] PHP：PDO 连接
来源：http://www.ydjk.org.cn/Article/details/gt3qyjiobtj.html

$pdo = new PDO("mysql:host=localhost;dbname=app", "root", "");
来源：http://www.52xcode.cn/Article/details/gt3xvrlidqg.html

[U69] PHP：PDO 预处理
来源：http://www.52xcode.cn/Article/details/gt3bskwcnel.html

$stmt = $pdo->prepare("SELECT * FROM users WHERE id = ?");  $stmt->execute([$id]);
来源：http://www.52xcode.cn/Article/details/gt3ptqvhnio.html

[U70] PHP：PDO 事务
来源：http://www.ydjk.org.cn/Article/details/gt3ouxeqpwz.html

$pdo->beginTransaction();  $pdo->commit();  $pdo->rollBack();
来源：http://www.ydjk.org.cn/Article/details/gt3zufmlbgt.html

[U71] PHP：抛出异常
来源：http://www.ydjk.org.cn/Article/details/gt3oilpvwns.html

throw new RuntimeException("失败", 500);
来源：http://www.52xcode.cn/Article/details/gt3itygenfw.html

[U72] PHP：写错误日志
来源：http://www.52xcode.cn/Article/details/gt3mlmqxjab.html

error_log("失败: " . $e->getMessage());
来源：http://www.ydjk.org.cn/Article/details/gt3okpmlsev.html

[U73] PHP：读取 ini 配置
来源：http://www.ydjk.org.cn/Article/details/gt3ihxmmaiu.html

parse_ini_file("config.ini", true)
来源：http://www.52xcode.cn/Article/details/gt3cbqeepsl.html

[U74] PHP：读取环境变量
来源：http://www.52xcode.cn/Article/details/gt3iyhjpund.html

getenv("APP_ENV") ?: "production"
来源：http://www.ydjk.org.cn/Article/details/gt3ddajavav.html

[U75] PHP：依赖注入
来源：http://www.52xcode.cn/Article/details/gt3oovspkjg.html

composer require psr/container
来源：http://www.52xcode.cn/Article/details/gt3ltniblmx.html

[U76] PHP：简单路由
来源：http://www.ydjk.org.cn/Article/details/gt3frbbseht.html

$path = parse_url($_SERVER["REQUEST_URI"], PHP_URL_PATH);
来源：http://www.ydjk.org.cn/Article/details/gt3yraqkxzv.html

[U77] PHP：模板渲染
来源：http://www.ydjk.org.cn/Article/details/gt3kifpuvau.html

composer require twig/twig
来源：http://www.ydjk.org.cn/Article/details/gt3sntrizjk.html

[U78] PHP：单元测试
来源：http://www.52xcode.cn/Article/details/gt3ewzsjlab.html

composer require --dev phpunit/phpunit
来源：http://www.52xcode.cn/Article/details/gt3ysdpxxvr.html

[U79] PHP：静态分析
来源：http://www.52xcode.cn/Article/details/gt3onwtyulb.html

composer require --dev phpstan/phpstan
来源：http://www.52xcode.cn/Article/details/gt3wtygubwr.html

[U80] PHP：代码规范修复
来源：http://www.52xcode.cn/Article/details/gt3kvuxdcct.html

composer require --dev friendsofphp/php-cs-fixer
来源：http://www.ydjk.org.cn/Article/details/gt3zzsgjswp.html

[U81] JS：初始化项目
来源：http://www.ydjk.org.cn/Article/details/gt3vwnuzphq.html

npm init -y;  npm i express
来源：http://www.ydjk.org.cn/Article/details/gt3gwlsdxhw.html

[U82] JS：package.json 脚本
来源：http://www.ydjk.org.cn/Article/details/gt3qdjwggho.html

"scripts": { "dev": "vite", "build": "vite build" }
来源：http://www.52xcode.cn/Article/details/gt3pchifmqh.html

[U83] JS：ES Module 导入导出
来源：http://www.ydjk.org.cn/Article/details/gt3fagrqndp.html

export const a = 1;  import { a } from "./m.js";
来源：http://www.ydjk.org.cn/Article/details/gt3uaeiegik.html

[U84] JS：CommonJS 写法
来源：http://www.52xcode.cn/Article/details/gt3cvvwzcer.html

module.exports = { a };  const { a } = require("./m");
来源：http://www.ydjk.org.cn/Article/details/gt3zuafmnbf.html

[U85] JS：可选链
来源：http://www.ydjk.org.cn/Article/details/gt3ebajatgn.html

a?.b?.c
来源：http://www.ydjk.org.cn/Article/details/gt3ntxmvohy.html

[U86] JS：空值合并
来源：http://www.ydjk.org.cn/Article/details/gt3eazknmmx.html

a ?? b
来源：http://www.52xcode.cn/Article/details/gt3iybfaeow.html

[U87] JS：解构默认值
来源：http://www.ydjk.org.cn/Article/details/gt3aopjmuhw.html

const { a = 1, b = 2 } = obj;
来源：http://www.52xcode.cn/Article/details/gt3dzvedtvd.html

[U88] JS：对象展开合并
来源：http://www.52xcode.cn/Article/details/gt3yjmktiek.html

{ ...a, ...b }
来源：http://www.ydjk.org.cn/Article/details/gt3fqmbflad.html

[U89] JS：数组去重
来源：http://www.52xcode.cn/Article/details/gt3gwkplolu.html

[...new Set(arr)]
来源：http://www.52xcode.cn/Article/details/gt3zdbbobwm.html

[U90] JS：数字数组排序
来源：http://www.ydjk.org.cn/Article/details/gt3habsskgu.html

[...arr].sort((a, b) => a - b)
来源：http://www.ydjk.org.cn/Article/details/gt3rxbqqnul.html

[U91] JS：对象键值遍历
来源：http://www.ydjk.org.cn/Article/details/gt3nsjtcldi.html

Object.entries(obj).forEach(([k, v]) => {});
来源：http://www.ydjk.org.cn/Article/details/gt3tmobfjoy.html

[U92] JS：深拷贝
来源：http://www.ydjk.org.cn/Article/details/gt3pdythrac.html

structuredClone(obj)
来源：http://www.ydjk.org.cn/Article/details/gt3vrquhpeh.html

[U93] JS：模板字符串
来源：http://www.ydjk.org.cn/Article/details/gt3yyiodqfd.html

`共 ${n} 条`
来源：http://www.ydjk.org.cn/Article/details/gt3poqgypjz.html

[U94] JS：箭头函数
来源：http://www.ydjk.org.cn/Article/details/gt3benpqwkm.html

const double = x => x * 2;
来源：http://www.ydjk.org.cn/Article/details/gt3dzvkzmhe.html

[U95] JS：Promise 包装
来源：http://www.52xcode.cn/Article/details/gt3rtdzujeh.html

new Promise((resolve, reject) => {})
来源：http://www.52xcode.cn/Article/details/gt3xzpvgxdv.html

[U96] JS：async/await 与异常
来源：http://www.52xcode.cn/Article/details/gt3gqxzfeoy.html

try { const d = await f(); } catch (e) { console.error(e); }
来源：http://www.52xcode.cn/Article/details/gt3goxdltns.html

[U97] JS：并发请求
来源：http://www.52xcode.cn/Article/details/gt3qfnncdso.html

await Promise.all(urls.map(u => fetch(u)))
来源：http://www.ydjk.org.cn/Article/details/gt3qcgyixce.html

[U98] JS：fetch 带 JSON
来源：http://www.52xcode.cn/Article/details/gt3lisrxdnr.html

await fetch(url, { method: "POST", headers: { "Content-Type": "application/json" }, body: JSON.stringify(d) })
来源：http://www.52xcode.cn/Article/details/gt3iuqnmzsp.html

[U99] JS：事件监听
来源：http://www.52xcode.cn/Article/details/gt3ejqivmdt.html

el.addEventListener("click", e => {})
来源：http://www.ydjk.org.cn/Article/details/gt3gpjzpdhe.html

[U100] JS：DOM 查询
来源：http://www.52xcode.cn/Article/details/gt3cdkapmby.html

document.querySelector(".item")
来源：http://www.ydjk.org.cn/Article/details/gt3smblnhye.html

[U101] JS：classList 操作
来源：http://www.52xcode.cn/Article/details/gt3xqskbbrc.html

el.classList.toggle("active")
来源：http://www.52xcode.cn/Article/details/gt3ssslpsfy.html

[U102] JS：本地存储
来源：http://www.52xcode.cn/Article/details/gt3retxrxmx.html

localStorage.setItem("k", JSON.stringify(v))
来源：http://www.52xcode.cn/Article/details/gt3joglrcli.html

[U103] JS：定时器
来源：http://www.ydjk.org.cn/Article/details/gt3gvbxlnxf.html

setTimeout(fn, 1000);  setInterval(fn, 1000);
来源：http://www.ydjk.org.cn/Article/details/gt3qmvnqlky.html

[U104] JS：防抖
来源：http://www.ydjk.org.cn/Article/details/gt3fxzsdlxa.html

const debounce = (fn, ms) => { let t; return (...a) => { clearTimeout(t); t = setTimeout(() => fn(...a), ms); }; };
来源：http://www.ydjk.org.cn/Article/details/gt3xdihncgn.html

[U105] JS：节流
来源：http://www.52xcode.cn/Article/details/gt3tzaykdzr.html

const throttle = (fn, ms) => { let last = 0; return (...a) => { const n = Date.now(); if (n - last >= ms) { last = n; fn(...a); } }; };
来源：http://www.52xcode.cn/Article/details/gt3oamtvntp.html

[U106] JS：日期格式化
来源：http://www.52xcode.cn/Article/details/gt3icpvffhx.html

new Intl.DateTimeFormat("zh-CN", { dateStyle: "medium" }).format(new Date())
来源：http://www.52xcode.cn/Article/details/gt3hfkcwule.html

[U107] JS：数字千分位
来源：http://www.52xcode.cn/Article/details/gt3phdezmxm.html

new Intl.NumberFormat("en-US").format(1234567)
来源：http://www.ydjk.org.cn/Article/details/gt3yxfrsdbn.html

[U108] JS：随机整数
来源：http://www.ydjk.org.cn/Article/details/gt3vhttfihs.html

Math.floor(Math.random() * (max - min + 1)) + min
来源：http://www.52xcode.cn/Article/details/gt3qgldfyes.html

[U109] JS：数组分组
来源：http://www.52xcode.cn/Article/details/gt3wyywvojz.html

Object.groupBy(arr, x => x.type)
来源：http://www.52xcode.cn/Article/details/gt3njmotebu.html

[U110] JS：数组分块
来源：http://www.52xcode.cn/Article/details/gt3gtnefayj.html

arr.reduce((acc, x, i) => (i % size ? acc : [...acc, arr.slice(i, i + size)]), [])
来源：http://www.ydjk.org.cn/Article/details/gt3gchzwoum.html

[U111] JS：对象转 Map
来源：http://www.ydjk.org.cn/Article/details/gt3jkwvtpke.html

new Map(Object.entries(obj))
来源：http://www.ydjk.org.cn/Article/details/gt3cbhilatx.html

[U112] JS：字符串补位
来源：http://www.ydjk.org.cn/Article/details/gt3atvmoooo.html

"7".padStart(3, "0")
来源：http://www.52xcode.cn/Article/details/gt3borrshzv.html

[U113] JS：正则替换全部
来源：http://www.ydjk.org.cn/Article/details/gt3ndjzecfo.html

s.replaceAll("a", "b")
来源：http://www.ydjk.org.cn/Article/details/gt3jgsaognh.html

[U114] JS：JSON 深比较
来源：http://www.52xcode.cn/Article/details/gt3jrfemcln.html

JSON.stringify(a) === JSON.stringify(b)
来源：http://www.ydjk.org.cn/Article/details/gt3ihulgvod.html

[U115] JS：生成 UUID
来源：http://www.ydjk.org.cn/Article/details/gt3lpvfavxt.html

crypto.randomUUID()
来源：http://www.52xcode.cn/Article/details/gt3zsqpcfjp.html

[U116] JS：类型检查（JSDoc）
来源：http://www.52xcode.cn/Article/details/gt3crqufmhq.html

/** @param {string} name */ function f(name) {}
来源：http://www.ydjk.org.cn/Article/details/gt3wqubwgft.html

[U117] JS：单元测试
来源：http://www.52xcode.cn/Article/details/gt3cclvsurg.html

npm i -D vitest;  npx vitest
来源：http://www.52xcode.cn/Article/details/gt3aaggpgxz.html

[U118] JS：开发服务器
来源：http://www.52xcode.cn/Article/details/gt3onlplwtx.html

npm i -D vite;  npx vite
来源：http://www.52xcode.cn/Article/details/gt3ybrgijyh.html

[U119] JS：生产构建
来源：http://www.ydjk.org.cn/Article/details/gt3ejdzodwc.html

npx vite build
来源：http://www.ydjk.org.cn/Article/details/gt3mcepuwih.html

[U120] JS：读取环境变量（Vite）
来源：http://www.ydjk.org.cn/Article/details/gt3haovfgjr.html

import.meta.env.VITE_API_URL
来源：http://www.52xcode.cn/Article/details/gt3iqmcnyqu.html

================================================================================
来源：http://www.ydjk.org.cn/Article/details/gt3kmqzukyt.html

统计汇总
来源：http://www.ydjk.org.cn/Article/details/gt3hfgamwzb.html

================================================================================
来源：http://www.ydjk.org.cn/Article/details/gt3ydyerahv.html

按语言统计（条）：
来源：http://www.52xcode.cn/Article/details/gt3kyoxstrz.html

Python ......... 252
来源：http://www.ydjk.org.cn/Article/details/gt3lmbdvqee.html

PHP ............ 252
来源：http://www.ydjk.org.cn/Article/details/gt3ewyirayd.html

JavaScript ..... 252
来源：http://www.ydjk.org.cn/Article/details/gt3rocbcuzi.html

TypeScript ..... 212
来源：http://www.ydjk.org.cn/Article/details/gt3vabxfjgt.html

Java ........... 212
来源：http://www.52xcode.cn/Article/details/gt3yubnftqs.html

Go ............. 212
来源：http://www.ydjk.org.cn/Article/details/gt3azpasilk.html

Ruby ........... 212
来源：http://www.52xcode.cn/Article/details/gt3pbcddfuf.html

C# ............. 212
来源：http://www.ydjk.org.cn/Article/details/gt3agznoxqp.html

C .............. 30
来源：http://www.52xcode.cn/Article/details/gt3nnbfisfx.html

C++ ............ 30
来源：http://www.ydjk.org.cn/Article/details/gt3uyafkbjy.html

SQL ............ 90
来源：http://www.ydjk.org.cn/Article/details/gt3jriswfvg.html

Bash ........... 80
来源：http://www.52xcode.cn/Article/details/gt3ouvxatuj.html

Kotlin ......... 15
来源：http://www.52xcode.cn/Article/details/gt3zksmflcs.html

Swift .......... 15
来源：http://www.ydjk.org.cn/Article/details/gt3dysptkkj.html

Lua ............ 10
来源：http://www.ydjk.org.cn/Article/details/gt3aokumtax.html

Perl ........... 10
来源：http://www.ydjk.org.cn/Article/details/gt3efoqkcnn.html

Scala .......... 10
来源：http://www.52xcode.cn/Article/details/gt3tdyjebqz.html

------------------------------------
来源：http://www.ydjk.org.cn/Article/details/gt3rvkmtlwq.html

合计 ........... 2106 条
来源：http://www.ydjk.org.cn/Article/details/gt3mtlaxmqn.html

按章节统计：
来源：http://www.52xcode.cn/Article/details/gt3rahvsdzs.html

A 基础语法与类型       26 个任务 × 8 语言 =  208
来源：http://www.ydjk.org.cn/Article/details/gt3tjblejux.html

B 流程控制             16 个任务 × 8 语言 =  128
来源：http://www.52xcode.cn/Article/details/gt3plfjhzem.html

C 函数与作用域         16 个任务 × 8 语言 =  128
来源：http://www.ydjk.org.cn/Article/details/gt3narwuyjv.html

D 数组 / 列表 / 集合   26 个任务 × 8 语言 =  208
来源：http://www.52xcode.cn/Article/details/gt3qvbxtxjw.html

E 字符串处理           22 个任务 × 8 语言 =  176
来源：http://www.ydjk.org.cn/Article/details/gt3gzkoikft.html

F 文件与目录           12 个任务 × 8 语言 =   96
来源：http://www.ydjk.org.cn/Article/details/gt3geosbqlo.html

G 面向对象             16 个任务 × 8 语言 =  128
来源：http://www.ydjk.org.cn/Article/details/gt3bjzuvaiu.html

H 异常与错误处理       10 个任务 × 8 语言 =   80
来源：http://www.ydjk.org.cn/Article/details/gt3ndkshkiz.html

I 正则表达式            8 个任务 × 8 语言 =   64
来源：http://www.ydjk.org.cn/Article/details/gt3chkizjed.html

J 日期与时间           10 个任务 × 8 语言 =   80
来源：http://www.52xcode.cn/Article/details/gt3sdwhoptq.html

K JSON 与序列化         8 个任务 × 8 语言 =   64
来源：http://www.52xcode.cn/Article/details/gt3dwodyalc.html

L 网络请求              8 个任务 × 8 语言 =   64
来源：http://www.ydjk.org.cn/Article/details/gt3oxuzmsfv.html

M 命令行 / 进程         8 个任务 × 8 语言 =   64
来源：http://www.ydjk.org.cn/Article/details/gt3bushmvvn.html

N 数据结构与算法       12 个任务 × 8 语言 =   96
来源：http://www.ydjk.org.cn/Article/details/gt3rskemnxe.html

O 并发与异步            6 个任务 × 8 语言 =   48
来源：http://www.52xcode.cn/Article/details/gt3gioudgeq.html

P 常用工具函数          8 个任务 × 8 语言 =   64
来源：http://www.52xcode.cn/Article/details/gt3azcochce.html

Q SQL 专题                              90
来源：http://www.52xcode.cn/Article/details/gt3olfpnxiv.html

R Bash 专题                             80
来源：http://www.ydjk.org.cn/Article/details/gt3ximtljmj.html

S C / C++ 专题                          60
来源：http://www.52xcode.cn/Article/details/gt3kwjazctr.html

T 其他语言补充                          60
来源：http://www.ydjk.org.cn/Article/details/gt3vuppsytx.html

U 高频实用片段                         120
来源：http://www.52xcode.cn/Article/details/gt3lrzcewjf.html

------------------------------------
来源：http://www.ydjk.org.cn/Article/details/gt3ssxvqspv.html

合计                                  2106 条
来源：http://www.52xcode.cn/Article/details/gt3kdnmfbid.html

--------------------------------------------------------------------------------
来源：http://www.52xcode.cn/Article/details/gt3tuwofmxy.html

使用提醒
来源：http://www.52xcode.cn/Article/details/gt3wlsiovtp.html

--------------------------------------------------------------------------------
来源：http://www.ydjk.org.cn/Article/details/gt3enokjhpo.html

1. 示例追求"最小可用"，正式项目中请补齐导入、错误处理与边界判断。
来源：http://www.ydjk.org.cn/Article/details/gt3ldhmxvcp.html

2. 涉及文件、网络、数据库的示例，注意资源释放与异常捕获。
来源：http://www.52xcode.cn/Article/details/gt3obajvbhw.html

3. 语言版本差异较大（如 Python 3.10 的 match、Java 17 的 record/switch 箭头），
来源：http://www.ydjk.org.cn/Article/details/gt3wgzvbiko.html

在旧版本上使用前请先确认语法支持情况。
来源：http://www.52xcode.cn/Article/details/gt3ubfeeqfc.html

4. 标注"手写"的条目是因为该语言缺少对应内置能力，实际项目中可引入成熟库。
来源：http://www.ydjk.org.cn/Article/details/gt3jvunvyjs.html

—— 文件结束 ——
来源：http://www.ydjk.org.cn/Article/details/gt3kotjfwld.html

================================================================================
来源：http://www.52xcode.cn/Article/details/gt3owfzoudi.html

程序语言常见例子速查手册（2024 版）
来源：http://www.ydjk.org.cn/Article/details/gt3chnmrvxr.html

Common Programming Examples Cheat Book
来源：http://www.52xcode.cn/Article/details/gt3qacrvywv.html

================================================================================
来源：http://www.ydjk.org.cn/Article/details/gt3jswnfdma.html

【收录内容】
来源：http://www.52xcode.cn/Article/details/gt3duvepmio.html

覆盖 12 种语言 / 语法与常见 API：
来源：http://www.52xcode.cn/Article/details/gt3etoumezd.html

Python · PHP · JavaScript · TypeScript · Java · Go · Ruby · C#
来源：http://www.ydjk.org.cn/Article/details/gt3pjopiqil.html

SQL · Bash · C · C++
来源：http://www.ydjk.org.cn/Article/details/gt3gjmwvtow.html

按「任务」分组：每个任务下按语言各给出一条最小可用示例。
来源：http://www.52xcode.cn/Article/details/gt3wlzpqvac.html

【使用说明】
来源：http://www.ydjk.org.cn/Article/details/gt3otzgdzqs.html

1. 每个任务形如 "[编号] 任务名"，下面每行以语言标记开头：
来源：http://www.52xcode.cn/Article/details/gt3swrlitys.html

Py:    Python        PHP:   PHP           JS:    JavaScript
来源：http://www.52xcode.cn/Article/details/gt3bziarjip.html

TS:    TypeScript    Java:  Java          Go:    Go
来源：http://www.52xcode.cn/Article/details/gt3daihyslm.html

Ruby:  Ruby          C#:    C#            SQL:   SQL
来源：http://www.ydjk.org.cn/Article/details/gt3oibcqcwc.html

Bash:  Shell         C:     C             C++:   C++
来源：http://www.52xcode.cn/Article/details/gt3bkjleuxl.html

2. 示例只展示核心写法，刻意省略 import / require / include / using 等样板代码。
来源：http://www.ydjk.org.cn/Article/details/gt3tdvllwsx.html

需要完整可运行文件时，请自行补齐当前语言的导入语句。
来源：http://www.ydjk.org.cn/Article/details/gt3dbikavod.html

3. 语法基准：Python 3.10+ / PHP 8.1+ / ES2020+ / TypeScript 5 / Java 17 /
来源：http://www.ydjk.org.cn/Article/details/gt3kvpytviq.html

Go 1.21+ / Ruby 3.x / C# 10+ / C17 / C++17。
来源：http://www.52xcode.cn/Article/details/gt3rgkmumtm.html

4. 检索建议：用编辑器或浏览器 Ctrl+F 搜关键词，如 "排序" "读取文件" "正则"。
来源：http://www.52xcode.cn/Article/details/gt3vbjgrmcd.html


<!-- 参考信息 -->