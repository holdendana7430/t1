代发 wailian999

[U17] Py：初始化日志
来源：http://www.ydjk.org.cn/Article/details/gt3azaeozns.html

logging.basicConfig(level=logging.INFO)
来源：http://www.52xcode.cn/Article/details/gt3vxonyfca.html

[U18] Py：预编译正则
来源：http://www.ydjk.org.cn/Article/details/gt3bztyvskq.html

pat = re.compile(r"\d+")
来源：http://www.52xcode.cn/Article/details/gt3hmgukwzp.html

[U19] Py：正则替换带回调
来源：http://www.52xcode.cn/Article/details/gt3rsmonnzv.html

re.sub(r"\d+", lambda m: str(int(m.group()) * 2), s)
来源：http://www.52xcode.cn/Article/details/gt3irfmftaq.html

[U20] Py：缓存函数结果
来源：http://www.52xcode.cn/Article/details/gt3unewzfhs.html

@functools.lru_cache(maxsize=None)
来源：http://www.ydjk.org.cn/Article/details/gt3xrxnfitj.html

[U21] Py：自定义上下文管理器
来源：http://www.ydjk.org.cn/Article/details/gt3vnupsric.html

@contextlib.contextmanager
来源：http://www.ydjk.org.cn/Article/details/gt3tbnltugv.html

[U22] Py：矩阵转置
来源：http://www.ydjk.org.cn/Article/details/gt3ymposzkq.html

list(zip(*m))
来源：http://www.ydjk.org.cn/Article/details/gt3tjhpwaaz.html

[U23] Py：分块读取大文件
来源：http://www.52xcode.cn/Article/details/gt3kbmbbxcj.html

for chunk in iter(lambda: f.read(8192), b""):
来源：http://www.52xcode.cn/Article/details/gt3mwwcdwey.html

[U24] Py：路径操作
来源：http://www.ydjk.org.cn/Article/details/gt3xnxgcfce.html

Path("a/b.txt").parent.mkdir(parents=True, exist_ok=True)
来源：http://www.52xcode.cn/Article/details/gt3pxldkwsy.html

[U25] Py：CSV 按字典读
来源：http://www.52xcode.cn/Article/details/gt3admadsgp.html

csv.DictReader(f)
来源：http://www.52xcode.cn/Article/details/gt3fnjzbaur.html

[U26] Py：并发下载
来源：http://www.ydjk.org.cn/Article/details/gt3gduqbmou.html

ThreadPoolExecutor(max_workers=8).map(fetch, urls)
来源：http://www.52xcode.cn/Article/details/gt3bjllfqrs.html

[U27] Py：异步 HTTP
来源：http://www.ydjk.org.cn/Article/details/gt3rlsfhwkn.html

aiohttp.ClientSession() 配合 async with
来源：http://www.52xcode.cn/Article/details/gt3kimzejhg.html

[U28] Py：类型别名
来源：http://www.ydjk.org.cn/Article/details/gt3mdrryzyt.html

UserId = int
来源：http://www.ydjk.org.cn/Article/details/gt3cudfyudn.html

[U29] Py：属性校验
来源：http://www.52xcode.cn/Article/details/gt3loncowvv.html

@property 与 @x.setter 配合
来源：http://www.52xcode.cn/Article/details/gt3hohmylrb.html

[U30] Py：数据类
来源：http://www.ydjk.org.cn/Article/details/gt3vjxfdsyg.html

@dataclass(slots=True)
来源：http://www.52xcode.cn/Article/details/gt3mngwhpif.html

[U31] Py：单测
来源：http://www.52xcode.cn/Article/details/gt3rlajjflq.html

python -m pytest -q
来源：http://www.ydjk.org.cn/Article/details/gt3vjnvnwco.html

[U32] Py：代码格式化
来源：http://www.ydjk.org.cn/Article/details/gt3rdktywpd.html

ruff format . && ruff check --fix .
来源：http://www.ydjk.org.cn/Article/details/gt3zrtqshaw.html

[U33] Py：打包发布
来源：http://www.52xcode.cn/Article/details/gt3hslgvfuu.html

python -m build  （依赖 pyproject.toml）
来源：http://www.52xcode.cn/Article/details/gt3tkwnzedi.html

[U34] Py：判断编码
来源：http://www.52xcode.cn/Article/details/gt3ipzgjfmi.html

chardet.detect(raw)
来源：http://www.52xcode.cn/Article/details/gt3hvhlguny.html

[U35] Py：发送邮件
来源：http://www.52xcode.cn/Article/details/gt3ddwfsvgi.html

smtplib.SMTP_SSL(...).send_message(msg)
来源：http://www.52xcode.cn/Article/details/gt3ilhtydwf.html

[U36] Py：定时任务
来源：http://www.ydjk.org.cn/Article/details/gt3gxfahxzu.html

schedule.every(10).minutes.do(job)
来源：http://www.ydjk.org.cn/Article/details/gt3hususcfz.html

[U37] Py：读写 Excel
来源：http://www.52xcode.cn/Article/details/gt3aptssjoj.html

pandas.read_excel / DataFrame.to_excel
来源：http://www.ydjk.org.cn/Article/details/gt3mikutmvf.html

[U38] Py：获取脚本所在目录
来源：http://www.ydjk.org.cn/Article/details/gt3kifniyrh.html

Path(__file__).resolve().parent
来源：http://www.ydjk.org.cn/Article/details/gt3lotwlqhh.html

[U39] Py：判断是否在交互环境
来源：http://www.52xcode.cn/Article/details/gt3fkcqhzve.html

sys.stdout.isatty()
来源：http://www.ydjk.org.cn/Article/details/gt3jjtbbjow.html

[U40] Py：打印到标准错误
来源：http://www.52xcode.cn/Article/details/gt3aoqbubpt.html

print("err", file=sys.stderr)
来源：http://www.ydjk.org.cn/Article/details/gt3zhsvrfdg.html

[U41] PHP：初始化 Composer 项目
来源：http://www.ydjk.org.cn/Article/details/gt3eujqpdju.html

composer init;  composer require guzzlehttp/guzzle
来源：http://www.52xcode.cn/Article/details/gt3vzovafhr.html

[U42] PHP：PSR-4 自动加载
来源：http://www.52xcode.cn/Article/details/gt3xeajzhps.html

"autoload": { "psr-4": { "App\\": "src/" } }
来源：http://www.ydjk.org.cn/Article/details/gt3mcoeisue.html

[U43] PHP：声明命名空间
来源：http://www.52xcode.cn/Article/details/gt3mmflzmxh.html

namespace App\Http;
来源：http://www.52xcode.cn/Article/details/gt3ayrinvtz.html

[U44] PHP：开启严格类型
来源：http://www.52xcode.cn/Article/details/gt3gpxlhxpc.html

declare(strict_types=1);
来源：http://www.52xcode.cn/Article/details/gt3lawwjrku.html

[U45] PHP：类型声明与返回类型
来源：http://www.52xcode.cn/Article/details/gt3vvauariv.html

function add(int $a, int $b): int { return $a + $b; }
来源：http://www.52xcode.cn/Article/details/gt3wuahfhei.html

[U46] PHP：可空类型
来源：http://www.52xcode.cn/Article/details/gt3ebgpzqqe.html

?string $name = null
来源：http://www.ydjk.org.cn/Article/details/gt3usnacscg.html

[U47] PHP：联合类型
来源：http://www.52xcode.cn/Article/details/gt3sliyfppp.html

int|string $id
来源：http://www.52xcode.cn/Article/details/gt3zcnrgsvc.html

[U48] PHP：纯枚举
来源：http://www.52xcode.cn/Article/details/gt3immwnrah.html

enum Status: string { case Active = "active"; case Off = "off"; }
来源：http://www.52xcode.cn/Article/details/gt3nvjiaajy.html

[U49] PHP：只读属性
来源：http://www.ydjk.org.cn/Article/details/gt3gqctnwqu.html

public readonly string $name
来源：http://www.ydjk.org.cn/Article/details/gt3fdeefrvz.html

[U50] PHP：构造器属性提升
来源：http://www.ydjk.org.cn/Article/details/gt3ecelqpvc.html

public function __construct(private int $id) {}
来源：http://www.ydjk.org.cn/Article/details/gt3saxenvqk.html

[U51] PHP：数组解构
来源：http://www.52xcode.cn/Article/details/gt3jsvxhstu.html

[$a, $b] = $arr;
来源：http://www.ydjk.org.cn/Article/details/gt3owfbicct.html

[U52] PHP：箭头函数
来源：http://www.52xcode.cn/Article/details/gt3cubhyjdj.html

$double = fn($x) => $x * 2;
来源：http://www.ydjk.org.cn/Article/details/gt3ttgmdddm.html

[U53] PHP：空合并运算符
来源：http://www.ydjk.org.cn/Article/details/gt3fgwdmfre.html

$v = $a ?? $b ?? "default";
来源：http://www.ydjk.org.cn/Article/details/gt3kepwjrdq.html

[U54] PHP：空安全调用
来源：http://www.ydjk.org.cn/Article/details/gt3gjdjjpxc.html

$obj?->method()
来源：http://www.ydjk.org.cn/Article/details/gt3aozuevtk.html

[U55] PHP：match 表达式
来源：http://www.52xcode.cn/Article/details/gt3faiaifdz.html

$s = match($x) { 1 => "一", default => "其他" };
来源：http://www.ydjk.org.cn/Article/details/gt3hwmdgguc.html

[U56] PHP：命名参数
来源：http://www.52xcode.cn/Article/details/gt3kxyenqvr.html

f(a: 1, b: 2)
来源：http://www.ydjk.org.cn/Article/details/gt3qzgmdnzh.html

[U57] PHP：字符串插值
来源：http://www.52xcode.cn/Article/details/gt3fimlvwgy.html

"值: {$a}"
来源：http://www.52xcode.cn/Article/details/gt3wklpswrc.html

[U58] PHP：数组三件套
来源：http://www.52xcode.cn/Article/details/gt3kbtauhdi.html

array_map($f, $a);  array_filter($a, $f);  array_reduce($a, $f, 0);
来源：http://www.ydjk.org.cn/Article/details/gt3rawdlssh.html

[U59] PHP：自定义排序
来源：http://www.52xcode.cn/Article/details/gt3xsjbtdxf.html

usort($arr, fn($a, $b) => $a["age"] <=> $b["age"]);
来源：http://www.52xcode.cn/Article/details/gt3wyefxaoa.html

[U60] PHP：JSON 编解码
来源：http://www.ydjk.org.cn/Article/details/gt3dorvfrtt.html

json_encode($d, JSON_UNESCAPED_UNICODE);  json_decode($s, true);
来源：http://www.52xcode.cn/Article/details/gt3opabbrtu.html

[U61] PHP：正则
来源：http://www.ydjk.org.cn/Article/details/gt3cwsmzlcj.html

preg_match('/(\d+)/', $s, $m);  preg_replace('/\d+/', '#', $s);
来源：http://www.ydjk.org.cn/Article/details/gt3xxmtlhwu.html

[U62] PHP：日期对象
来源：http://www.52xcode.cn/Article/details/gt3jguitvtg.html

(new DateTimeImmutable())->format("Y-m-d");
来源：http://www.ydjk.org.cn/Article/details/gt3cpgmssyv.html

[U63] PHP：文件读写
来源：http://www.52xcode.cn/Article/details/gt3vydycvit.html

file_get_contents($f);  file_put_contents($f, $data);
来源：http://www.ydjk.org.cn/Article/details/gt3acybppiq.html

[U64] PHP：目录遍历
来源：http://www.52xcode.cn/Article/details/gt3rzznwgtc.html

glob("dir/*.php");  scandir("dir");
来源：http://www.ydjk.org.cn/Article/details/gt3xnrksrse.html

[U65] PHP：会话
来源：http://www.52xcode.cn/Article/details/gt3bvqqtprm.html

session_start();  $_SESSION["uid"] = 1;
来源：http://www.52xcode.cn/Article/details/gt3nerlkkyu.html

[U66] PHP：设置 Cookie
来源：http://www.ydjk.org.cn/Article/details/gt3yiksuixb.html

setcookie("token", $v, ["httponly" => true, "samesite" => "Lax"]);
来源：http://www.ydjk.org.cn/Article/details/gt3kgkelbti.html

[U67] PHP：处理文件上传
来源：http://www.ydjk.org.cn/Article/details/gt3rvwtojgj.html

$_FILES["file"]["tmp_name"] 与 move_uploaded_file()
来源：http://www.ydjk.org.cn/Article/details/gt3wytrvlof.html

[U68] PHP：PDO 连接
来源：http://www.ydjk.org.cn/Article/details/gt3cxgirdld.html

$pdo = new PDO("mysql:host=localhost;dbname=app", "root", "");
来源：http://www.ydjk.org.cn/Article/details/gt3yqhqofsw.html

[U69] PHP：PDO 预处理
来源：http://www.52xcode.cn/Article/details/gt3wkeeihql.html

$stmt = $pdo->prepare("SELECT * FROM users WHERE id = ?");  $stmt->execute([$id]);
来源：http://www.ydjk.org.cn/Article/details/gt3rcpditlw.html

[U70] PHP：PDO 事务
来源：http://www.ydjk.org.cn/Article/details/gt3xtijxbdr.html

$pdo->beginTransaction();  $pdo->commit();  $pdo->rollBack();
来源：http://www.52xcode.cn/Article/details/gt3bmifbzml.html

[U71] PHP：抛出异常
来源：http://www.ydjk.org.cn/Article/details/gt3qbpxkaps.html

throw new RuntimeException("失败", 500);
来源：http://www.ydjk.org.cn/Article/details/gt3wgihmpli.html

[U72] PHP：写错误日志
来源：http://www.52xcode.cn/Article/details/gt3frnvebhd.html

error_log("失败: " . $e->getMessage());
来源：http://www.52xcode.cn/Article/details/gt3kjiwwqmw.html

[U73] PHP：读取 ini 配置
来源：http://www.52xcode.cn/Article/details/gt3omwfuhhi.html

parse_ini_file("config.ini", true)
来源：http://www.52xcode.cn/Article/details/gt3ufavwknu.html

[U74] PHP：读取环境变量
来源：http://www.52xcode.cn/Article/details/gt3gehapyhl.html

getenv("APP_ENV") ?: "production"
来源：http://www.ydjk.org.cn/Article/details/gt3vaielhlg.html

[U75] PHP：依赖注入
来源：http://www.52xcode.cn/Article/details/gt3taopgyxr.html

composer require psr/container
来源：http://www.ydjk.org.cn/Article/details/gt3cqbrehia.html

[U76] PHP：简单路由
来源：http://www.52xcode.cn/Article/details/gt3fxhvxuqj.html

$path = parse_url($_SERVER["REQUEST_URI"], PHP_URL_PATH);
来源：http://www.52xcode.cn/Article/details/gt3gmjvoqym.html

[U77] PHP：模板渲染
来源：http://www.ydjk.org.cn/Article/details/gt3vzphnies.html

composer require twig/twig
来源：http://www.52xcode.cn/Article/details/gt3qyvqteme.html

[U78] PHP：单元测试
来源：http://www.ydjk.org.cn/Article/details/gt3uwgxeaty.html

composer require --dev phpunit/phpunit
来源：http://www.ydjk.org.cn/Article/details/gt3jdzneujo.html

[U79] PHP：静态分析
来源：http://www.52xcode.cn/Article/details/gt3yrydcrhk.html

composer require --dev phpstan/phpstan
来源：http://www.ydjk.org.cn/Article/details/gt3qvcywhmy.html

[U80] PHP：代码规范修复
来源：http://www.ydjk.org.cn/Article/details/gt3oimhvdrh.html

composer require --dev friendsofphp/php-cs-fixer
来源：http://www.ydjk.org.cn/Article/details/gt3yzbbsbcp.html

[U81] JS：初始化项目
来源：http://www.ydjk.org.cn/Article/details/gt3zhshkews.html

npm init -y;  npm i express
来源：http://www.52xcode.cn/Article/details/gt3msddavdu.html

[U82] JS：package.json 脚本
来源：http://www.52xcode.cn/Article/details/gt3ejdcwlst.html

"scripts": { "dev": "vite", "build": "vite build" }
来源：http://www.52xcode.cn/Article/details/gt3zppjlgan.html

[U83] JS：ES Module 导入导出
来源：http://www.ydjk.org.cn/Article/details/gt3mmtvvwba.html

export const a = 1;  import { a } from "./m.js";
来源：http://www.ydjk.org.cn/Article/details/gt3nrteoync.html

[U84] JS：CommonJS 写法
来源：http://www.52xcode.cn/Article/details/gt3vfdghqek.html

module.exports = { a };  const { a } = require("./m");
来源：http://www.52xcode.cn/Article/details/gt3xihoapdz.html

[U85] JS：可选链
来源：http://www.ydjk.org.cn/Article/details/gt3boeiejwn.html

a?.b?.c
来源：http://www.52xcode.cn/Article/details/gt3arptxnmo.html

[U86] JS：空值合并
来源：http://www.ydjk.org.cn/Article/details/gt3irjapslt.html

a ?? b
来源：http://www.ydjk.org.cn/Article/details/gt3zuiuoezw.html

[U87] JS：解构默认值
来源：http://www.52xcode.cn/Article/details/gt3vjclhrzw.html

const { a = 1, b = 2 } = obj;
来源：http://www.52xcode.cn/Article/details/gt3wablfbwf.html

[U88] JS：对象展开合并
来源：http://www.52xcode.cn/Article/details/gt3lxndowiq.html

{ ...a, ...b }
来源：http://www.ydjk.org.cn/Article/details/gt3olgegfkb.html

[U89] JS：数组去重
来源：http://www.ydjk.org.cn/Article/details/gt3onextmxc.html

[...new Set(arr)]
来源：http://www.52xcode.cn/Article/details/gt3nivqgmey.html

[U90] JS：数字数组排序
来源：http://www.52xcode.cn/Article/details/gt3hgytkfpx.html

[...arr].sort((a, b) => a - b)
来源：http://www.ydjk.org.cn/Article/details/gt3gvtzncgp.html

[U91] JS：对象键值遍历
来源：http://www.ydjk.org.cn/Article/details/gt3tahcqoqs.html

Object.entries(obj).forEach(([k, v]) => {});
来源：http://www.52xcode.cn/Article/details/gt3vfcnhpia.html

[U92] JS：深拷贝
来源：http://www.ydjk.org.cn/Article/details/gt3kgulwzsa.html

structuredClone(obj)
来源：http://www.52xcode.cn/Article/details/gt3nglhlxuu.html

[U93] JS：模板字符串
来源：http://www.ydjk.org.cn/Article/details/gt3edmeqkjr.html

`共 ${n} 条`
来源：http://www.52xcode.cn/Article/details/gt3ztfrygfc.html

[U94] JS：箭头函数
来源：http://www.ydjk.org.cn/Article/details/gt3xbzxkvjw.html

const double = x => x * 2;
来源：http://www.52xcode.cn/Article/details/gt3ftlvxftf.html

[U95] JS：Promise 包装
来源：http://www.ydjk.org.cn/Article/details/gt3znnvizeo.html

new Promise((resolve, reject) => {})
来源：http://www.ydjk.org.cn/Article/details/gt3lxafcwbs.html

[U96] JS：async/await 与异常
来源：http://www.52xcode.cn/Article/details/gt3awouwqsu.html

try { const d = await f(); } catch (e) { console.error(e); }
来源：http://www.52xcode.cn/Article/details/gt3eclwxzid.html

[U97] JS：并发请求
来源：http://www.52xcode.cn/Article/details/gt3voabxept.html

await Promise.all(urls.map(u => fetch(u)))
来源：http://www.ydjk.org.cn/Article/details/gt3iytlbbfj.html

[U98] JS：fetch 带 JSON
来源：http://www.ydjk.org.cn/Article/details/gt3jwhkvhcn.html

await fetch(url, { method: "POST", headers: { "Content-Type": "application/json" }, body: JSON.stringify(d) })
来源：http://www.ydjk.org.cn/Article/details/gt3fvdrqnnw.html

[U99] JS：事件监听
来源：http://www.ydjk.org.cn/Article/details/gt3kvdvlydx.html

el.addEventListener("click", e => {})
来源：http://www.52xcode.cn/Article/details/gt3aegdzrym.html

[U100] JS：DOM 查询
来源：http://www.52xcode.cn/Article/details/gt3jyqsltgu.html

document.querySelector(".item")
来源：http://www.52xcode.cn/Article/details/gt3unnhvolh.html

[U101] JS：classList 操作
来源：http://www.52xcode.cn/Article/details/gt3nrfyagdj.html

el.classList.toggle("active")
来源：http://www.ydjk.org.cn/Article/details/gt3wpysamwb.html

[U102] JS：本地存储
来源：http://www.ydjk.org.cn/Article/details/gt3zqxryqqj.html

localStorage.setItem("k", JSON.stringify(v))
来源：http://www.52xcode.cn/Article/details/gt3jpkfdvsq.html

[U103] JS：定时器
来源：http://www.52xcode.cn/Article/details/gt3gpqcvyav.html

setTimeout(fn, 1000);  setInterval(fn, 1000);
来源：http://www.ydjk.org.cn/Article/details/gt3swzwbjar.html

[U104] JS：防抖
来源：http://www.52xcode.cn/Article/details/gt3fgrljjrn.html

const debounce = (fn, ms) => { let t; return (...a) => { clearTimeout(t); t = setTimeout(() => fn(...a), ms); }; };
来源：http://www.ydjk.org.cn/Article/details/gt3zitssrmm.html

[U105] JS：节流
来源：http://www.ydjk.org.cn/Article/details/gt3bugyhxww.html

const throttle = (fn, ms) => { let last = 0; return (...a) => { const n = Date.now(); if (n - last >= ms) { last = n; fn(...a); } }; };
来源：http://www.ydjk.org.cn/Article/details/gt3lvhraiit.html

[U106] JS：日期格式化
来源：http://www.52xcode.cn/Article/details/gt3lyawlxas.html

new Intl.DateTimeFormat("zh-CN", { dateStyle: "medium" }).format(new Date())
来源：http://www.52xcode.cn/Article/details/gt3hbuptthd.html

[U107] JS：数字千分位
来源：http://www.ydjk.org.cn/Article/details/gt3emkpkuff.html

new Intl.NumberFormat("en-US").format(1234567)
来源：http://www.ydjk.org.cn/Article/details/gt3hhlgonuu.html

[U108] JS：随机整数
来源：http://www.ydjk.org.cn/Article/details/gt3iopdspyy.html

Math.floor(Math.random() * (max - min + 1)) + min
来源：http://www.52xcode.cn/Article/details/gt3zybudgec.html

[U109] JS：数组分组
来源：http://www.ydjk.org.cn/Article/details/gt3hedrgulm.html

Object.groupBy(arr, x => x.type)
来源：http://www.ydjk.org.cn/Article/details/gt3sgkpvlem.html

[U110] JS：数组分块
来源：http://www.52xcode.cn/Article/details/gt3aajxyzka.html

arr.reduce((acc, x, i) => (i % size ? acc : [...acc, arr.slice(i, i + size)]), [])
来源：http://www.52xcode.cn/Article/details/gt3iohqkkyx.html

[U111] JS：对象转 Map
来源：http://www.ydjk.org.cn/Article/details/gt3athoksut.html

new Map(Object.entries(obj))
来源：http://www.52xcode.cn/Article/details/gt3idpvhcrd.html

[U112] JS：字符串补位
来源：http://www.52xcode.cn/Article/details/gt3vwawpptw.html

"7".padStart(3, "0")
来源：http://www.ydjk.org.cn/Article/details/gt3mynjiehc.html

[U113] JS：正则替换全部
来源：http://www.52xcode.cn/Article/details/gt3brhvjsuu.html

s.replaceAll("a", "b")
来源：http://www.ydjk.org.cn/Article/details/gt3oasvxleg.html

[U114] JS：JSON 深比较
来源：http://www.52xcode.cn/Article/details/gt3bfxmvkms.html

JSON.stringify(a) === JSON.stringify(b)
来源：http://www.ydjk.org.cn/Article/details/gt3tnbjwfoc.html

[U115] JS：生成 UUID
来源：http://www.ydjk.org.cn/Article/details/gt3cpyatien.html

crypto.randomUUID()
来源：http://www.52xcode.cn/Article/details/gt3xvrsvjdy.html

[U116] JS：类型检查（JSDoc）
来源：http://www.ydjk.org.cn/Article/details/gt3ccesoqnx.html

/** @param {string} name */ function f(name) {}
来源：http://www.52xcode.cn/Article/details/gt3uarbfkfj.html

[U117] JS：单元测试
来源：http://www.52xcode.cn/Article/details/gt3trzvcxzb.html

npm i -D vitest;  npx vitest
来源：http://www.52xcode.cn/Article/details/gt3sybsqcwy.html

[U118] JS：开发服务器
来源：http://www.52xcode.cn/Article/details/gt3laghibwa.html

npm i -D vite;  npx vite
来源：http://www.52xcode.cn/Article/details/gt3dzmormce.html

[U119] JS：生产构建
来源：http://www.52xcode.cn/Article/details/gt3hmiyoptw.html

npx vite build
来源：http://www.52xcode.cn/Article/details/gt3zzwzpsyp.html

[U120] JS：读取环境变量（Vite）
来源：http://www.ydjk.org.cn/Article/details/gt3lqdmbodb.html

import.meta.env.VITE_API_URL
来源：http://www.ydjk.org.cn/Article/details/gt3oizfzufm.html

================================================================================
来源：http://www.ydjk.org.cn/Article/details/gt3qxuccwdn.html

统计汇总
来源：http://www.52xcode.cn/Article/details/gt3evzmydyk.html

================================================================================
来源：http://www.ydjk.org.cn/Article/details/gt3ptsmsuyb.html

按语言统计（条）：
来源：http://www.52xcode.cn/Article/details/gt3efljxydh.html

Python ......... 252
来源：http://www.52xcode.cn/Article/details/gt3ukrucvmo.html

PHP ............ 252
来源：http://www.52xcode.cn/Article/details/gt3plypjmsl.html

JavaScript ..... 252
来源：http://www.52xcode.cn/Article/details/gt3fgcanmen.html

TypeScript ..... 212
来源：http://www.ydjk.org.cn/Article/details/gt3lurnzsrq.html

Java ........... 212
来源：http://www.52xcode.cn/Article/details/gt3fkiisoxh.html

Go ............. 212
来源：http://www.ydjk.org.cn/Article/details/gt3jbchehgw.html

Ruby ........... 212
来源：http://www.ydjk.org.cn/Article/details/gt3gxguduni.html

C# ............. 212
来源：http://www.52xcode.cn/Article/details/gt3themswsq.html

C .............. 30
来源：http://www.52xcode.cn/Article/details/gt3lnkzcnog.html

C++ ............ 30
来源：http://www.52xcode.cn/Article/details/gt3tjvsdwvi.html

SQL ............ 90
来源：http://www.ydjk.org.cn/Article/details/gt3wxqxlxhy.html

Bash ........... 80
来源：http://www.52xcode.cn/Article/details/gt3rninqvex.html

Kotlin ......... 15
来源：http://www.52xcode.cn/Article/details/gt3zqlfxhdv.html

Swift .......... 15
来源：http://www.ydjk.org.cn/Article/details/gt3wapowrgu.html

Lua ............ 10
来源：http://www.52xcode.cn/Article/details/gt3sehgrgdh.html

Perl ........... 10
来源：http://www.52xcode.cn/Article/details/gt3xttkanic.html

Scala .......... 10
来源：http://www.ydjk.org.cn/Article/details/gt3pjklodcg.html

------------------------------------
来源：http://www.ydjk.org.cn/Article/details/gt3rtcljgay.html

合计 ........... 2106 条
来源：http://www.ydjk.org.cn/Article/details/gt3mecqsleo.html

按章节统计：
来源：http://www.52xcode.cn/Article/details/gt3kooihsff.html

A 基础语法与类型       26 个任务 × 8 语言 =  208
来源：http://www.52xcode.cn/Article/details/gt3vkboassq.html

B 流程控制             16 个任务 × 8 语言 =  128
来源：http://www.52xcode.cn/Article/details/gt3mgzhngbf.html

C 函数与作用域         16 个任务 × 8 语言 =  128
来源：http://www.ydjk.org.cn/Article/details/gt3ksosknev.html

D 数组 / 列表 / 集合   26 个任务 × 8 语言 =  208
来源：http://www.ydjk.org.cn/Article/details/gt3fybgtxds.html

E 字符串处理           22 个任务 × 8 语言 =  176
来源：http://www.ydjk.org.cn/Article/details/gt3nouvyxdp.html

F 文件与目录           12 个任务 × 8 语言 =   96
来源：http://www.ydjk.org.cn/Article/details/gt3wroceuxk.html

G 面向对象             16 个任务 × 8 语言 =  128
来源：http://www.ydjk.org.cn/Article/details/gt3dxrysuix.html

H 异常与错误处理       10 个任务 × 8 语言 =   80
来源：http://www.ydjk.org.cn/Article/details/gt3hefiiveg.html

I 正则表达式            8 个任务 × 8 语言 =   64
来源：http://www.52xcode.cn/Article/details/gt3ornglpxh.html

J 日期与时间           10 个任务 × 8 语言 =   80
来源：http://www.ydjk.org.cn/Article/details/gt3dbeczezo.html

K JSON 与序列化         8 个任务 × 8 语言 =   64
来源：http://www.ydjk.org.cn/Article/details/gt3bkplrirf.html

L 网络请求              8 个任务 × 8 语言 =   64
来源：http://www.52xcode.cn/Article/details/gt3aemqfoql.html

M 命令行 / 进程         8 个任务 × 8 语言 =   64
来源：http://www.52xcode.cn/Article/details/gt3uqqdnzgp.html

N 数据结构与算法       12 个任务 × 8 语言 =   96
来源：http://www.52xcode.cn/Article/details/gt3jrgkidad.html

O 并发与异步            6 个任务 × 8 语言 =   48
来源：http://www.52xcode.cn/Article/details/gt3zvcetmku.html

P 常用工具函数          8 个任务 × 8 语言 =   64
来源：http://www.52xcode.cn/Article/details/gt3ndumczts.html

Q SQL 专题                              90
来源：http://www.ydjk.org.cn/Article/details/gt3uzghowya.html

R Bash 专题                             80
来源：http://www.52xcode.cn/Article/details/gt3evnzshmt.html

S C / C++ 专题                          60
来源：http://www.ydjk.org.cn/Article/details/gt3ixkbjmiq.html

T 其他语言补充                          60
来源：http://www.ydjk.org.cn/Article/details/gt3sumdewtt.html

U 高频实用片段                         120
来源：http://www.52xcode.cn/Article/details/gt3cqobkrds.html

------------------------------------
来源：http://www.52xcode.cn/Article/details/gt3nqgdovxd.html

合计                                  2106 条
来源：http://www.ydjk.org.cn/Article/details/gt3jqorgfzh.html

--------------------------------------------------------------------------------
来源：http://www.52xcode.cn/Article/details/gt3xmuqxgng.html

使用提醒
来源：http://www.ydjk.org.cn/Article/details/gt3eivjdszx.html

--------------------------------------------------------------------------------
来源：http://www.ydjk.org.cn/Article/details/gt3uvoakcxb.html

1. 示例追求"最小可用"，正式项目中请补齐导入、错误处理与边界判断。
来源：http://www.ydjk.org.cn/Article/details/gt3yflzfsel.html

2. 涉及文件、网络、数据库的示例，注意资源释放与异常捕获。
来源：http://www.52xcode.cn/Article/details/gt3bjaxjhre.html

3. 语言版本差异较大（如 Python 3.10 的 match、Java 17 的 record/switch 箭头），
来源：http://www.ydjk.org.cn/Article/details/gt3pvphonah.html

在旧版本上使用前请先确认语法支持情况。
来源：http://www.ydjk.org.cn/Article/details/gt3lnitlzht.html

4. 标注"手写"的条目是因为该语言缺少对应内置能力，实际项目中可引入成熟库。
来源：http://www.ydjk.org.cn/Article/details/gt3rbjgzmji.html

—— 文件结束 ——
来源：http://www.ydjk.org.cn/Article/details/gt3ljqxsupi.html

================================================================================
来源：http://www.ydjk.org.cn/Article/details/gt3hxadagdy.html

程序语言常见例子速查手册（2024 版）
来源：http://www.ydjk.org.cn/Article/details/gt3cnxfpilw.html

Common Programming Examples Cheat Book
来源：http://www.52xcode.cn/Article/details/gt3ypulhbsk.html

================================================================================
来源：http://www.ydjk.org.cn/Article/details/gt3fdfzuful.html

【收录内容】
来源：http://www.ydjk.org.cn/Article/details/gt3kpeolmyn.html

覆盖 12 种语言 / 语法与常见 API：
来源：http://www.52xcode.cn/Article/details/gt3rskpxzvv.html

Python · PHP · JavaScript · TypeScript · Java · Go · Ruby · C#
来源：http://www.52xcode.cn/Article/details/gt3taxwzmzz.html

SQL · Bash · C · C++
来源：http://www.ydjk.org.cn/Article/details/gt3mvjhbjxq.html

按「任务」分组：每个任务下按语言各给出一条最小可用示例。
来源：http://www.52xcode.cn/Article/details/gt3ubfamsuf.html

【使用说明】
来源：http://www.ydjk.org.cn/Article/details/gt3givsfrbf.html

1. 每个任务形如 "[编号] 任务名"，下面每行以语言标记开头：
来源：http://www.52xcode.cn/Article/details/gt3hqytbfvs.html

Py:    Python        PHP:   PHP           JS:    JavaScript
来源：http://www.52xcode.cn/Article/details/gt3brufevjp.html

TS:    TypeScript    Java:  Java          Go:    Go
来源：http://www.ydjk.org.cn/Article/details/gt3boospvfa.html

Ruby:  Ruby          C#:    C#            SQL:   SQL
来源：http://www.ydjk.org.cn/Article/details/gt3cwudympm.html

Bash:  Shell         C:     C             C++:   C++
来源：http://www.ydjk.org.cn/Article/details/gt3sdmttjdr.html

2. 示例只展示核心写法，刻意省略 import / require / include / using 等样板代码。
来源：http://www.ydjk.org.cn/Article/details/gt3nrvmsfqk.html

需要完整可运行文件时，请自行补齐当前语言的导入语句。
来源：http://www.ydjk.org.cn/Article/details/gt3ltcsxrvw.html

3. 语法基准：Python 3.10+ / PHP 8.1+ / ES2020+ / TypeScript 5 / Java 17 /
来源：http://www.52xcode.cn/Article/details/gt3xauxhbmw.html

Go 1.21+ / Ruby 3.x / C# 10+ / C17 / C++17。
来源：http://www.ydjk.org.cn/Article/details/gt3dhxamleg.html

4. 检索建议：用编辑器或浏览器 Ctrl+F 搜关键词，如 "排序" "读取文件" "正则"。
来源：http://www.ydjk.org.cn/Article/details/gt3rmflcgqq.html

5. 标记为 "// 无" 表示该语言没有对应的一等语法，需用替代写法（示例给出替代方案）。
来源：http://www.ydjk.org.cn/Article/details/gt3gcghbhtm.html

6. 符号 "⏎" 表示代码在此处换行（主要用于 Python 等强制缩进、无法压成一行的结构）。
来源：http://www.ydjk.org.cn/Article/details/gt3yfvbuabs.html

【文件统计】
来源：http://www.52xcode.cn/Article/details/gt3bbouqjkh.html

语言示例共 2106 条，分布见本文末尾的「统计汇总」。
来源：http://www.ydjk.org.cn/Article/details/gt3cvtvrxzj.html

--------------------------------------------------------------------------------
来源：http://www.ydjk.org.cn/Article/details/gt3otnvyywh.html

目  录
来源：http://www.52xcode.cn/Article/details/gt3eidryxmj.html

--------------------------------------------------------------------------------
来源：http://www.52xcode.cn/Article/details/gt3aycxunrs.html

A. 基础语法与类型              （第 1 节，26 个任务，208 条）
来源：http://www.ydjk.org.cn/Article/details/gt3mmutgbzo.html

B. 流程控制                    （第 2 节，16 个任务，128 条）
来源：http://www.ydjk.org.cn/Article/details/gt3qvusjygz.html

C. 函数与作用域                （第 3 节，16 个任务，128 条）
来源：http://www.ydjk.org.cn/Article/details/gt3uwpsqvzf.html

D. 数组 / 列表 / 集合          （第 4 节，26 个任务，208 条）
来源：http://www.ydjk.org.cn/Article/details/gt3rrczlnth.html

E. 字符串处理                  （第 5 节，22 个任务，176 条）
来源：http://www.ydjk.org.cn/Article/details/gt3roolhwtc.html

F. 文件与目录                  （第 6 节，12 个任务，96 条）
来源：http://www.52xcode.cn/Article/details/gt3zsbwcbjv.html

G. 面向对象                    （第 7 节，16 个任务，128 条）
来源：http://www.ydjk.org.cn/Article/details/gt3ijenlekr.html

H. 异常与错误处理              （第 8 节，10 个任务，80 条）
来源：http://www.ydjk.org.cn/Article/details/gt3jvdcjsnh.html

I. 正则表达式                  （第 9 节，8 个任务，64 条）
来源：http://www.ydjk.org.cn/Article/details/gt3hmehondt.html


<!-- 参考信息 -->