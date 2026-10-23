代发 wailian999

[U07] Py：反转字典键值
来源：http://www.52xcode.cn/Article/details/gt3zzujktpz.html

{v: k for k, v in d.items()}
来源：http://www.52xcode.cn/Article/details/gt3qnphdwqk.html

[U08] Py：展平二维列表
来源：http://www.ydjk.org.cn/Article/details/gt3rpmxiige.html

[y for x in nested for y in x]
来源：http://www.52xcode.cn/Article/details/gt3bbkxpjem.html

[U09] Py：字典取最大值的键
来源：http://www.ydjk.org.cn/Article/details/gt3gkcjocfd.html

max(d, key=d.get)
来源：http://www.ydjk.org.cn/Article/details/gt3iorqtovu.html

[U10] Py：按值排序字典
来源：http://www.52xcode.cn/Article/details/gt3dbqdrepc.html

dict(sorted(d.items(), key=lambda kv: kv[1]))
来源：http://www.52xcode.cn/Article/details/gt3zejgsedn.html

[U11] Py：生成器表达式
来源：http://www.52xcode.cn/Article/details/gt3rvdhvjdt.html

(x * 2 for x in arr)
来源：http://www.52xcode.cn/Article/details/gt3tkjbjqsb.html

[U12] Py：取出现最多的 3 个元素
来源：http://www.ydjk.org.cn/Article/details/gt3scbohizz.html

Counter(arr).most_common(3)
来源：http://www.ydjk.org.cn/Article/details/gt3xltxomjw.html

[U13] Py：固定长度队列
来源：http://www.52xcode.cn/Article/details/gt3nqtkfkoy.html

deque(maxlen=10)
来源：http://www.ydjk.org.cn/Article/details/gt3fynflcng.html

[U14] Py：分组收集到列表
来源：http://www.52xcode.cn/Article/details/gt3yztbnpnb.html

defaultdict(list)
来源：http://www.ydjk.org.cn/Article/details/gt3mopobsyq.html

[U15] Py：高精度计时
来源：http://www.52xcode.cn/Article/details/gt3tbtymlpe.html

t = time.perf_counter()
来源：http://www.ydjk.org.cn/Article/details/gt3jlympfls.html

[U16] Py：命令行参数解析
来源：http://www.52xcode.cn/Article/details/gt3vmhvsrgt.html

ap = argparse.ArgumentParser();  ap.add_argument("--name");  args = ap.parse_args()
来源：http://www.ydjk.org.cn/Article/details/gt3ubsnqgos.html

[U17] Py：初始化日志
来源：http://www.ydjk.org.cn/Article/details/gt3aoozfrib.html

logging.basicConfig(level=logging.INFO)
来源：http://www.52xcode.cn/Article/details/gt3tklcfjxi.html

[U18] Py：预编译正则
来源：http://www.ydjk.org.cn/Article/details/gt3bxtfailf.html

pat = re.compile(r"\d+")
来源：http://www.52xcode.cn/Article/details/gt3zibdcurf.html

[U19] Py：正则替换带回调
来源：http://www.ydjk.org.cn/Article/details/gt3skicajiw.html

re.sub(r"\d+", lambda m: str(int(m.group()) * 2), s)
来源：http://www.52xcode.cn/Article/details/gt3asnnzksl.html

[U20] Py：缓存函数结果
来源：http://www.52xcode.cn/Article/details/gt3ruueccdy.html

@functools.lru_cache(maxsize=None)
来源：http://www.ydjk.org.cn/Article/details/gt3bfokzyne.html

[U21] Py：自定义上下文管理器
来源：http://www.52xcode.cn/Article/details/gt3phbbrnpv.html

@contextlib.contextmanager
来源：http://www.52xcode.cn/Article/details/gt3djozmyfm.html

[U22] Py：矩阵转置
来源：http://www.52xcode.cn/Article/details/gt3gahhmfev.html

list(zip(*m))
来源：http://www.ydjk.org.cn/Article/details/gt3noxmsfod.html

[U23] Py：分块读取大文件
来源：http://www.52xcode.cn/Article/details/gt3duzpgfnw.html

for chunk in iter(lambda: f.read(8192), b""):
来源：http://www.52xcode.cn/Article/details/gt3rgqwvego.html

[U24] Py：路径操作
来源：http://www.52xcode.cn/Article/details/gt3vykmaitc.html

Path("a/b.txt").parent.mkdir(parents=True, exist_ok=True)
来源：http://www.ydjk.org.cn/Article/details/gt3wbgwmvwx.html

[U25] Py：CSV 按字典读
来源：http://www.ydjk.org.cn/Article/details/gt3mwrswxlv.html

csv.DictReader(f)
来源：http://www.ydjk.org.cn/Article/details/gt3oqgaaqbd.html

[U26] Py：并发下载
来源：http://www.ydjk.org.cn/Article/details/gt3ijyneovj.html

ThreadPoolExecutor(max_workers=8).map(fetch, urls)
来源：http://www.52xcode.cn/Article/details/gt3nwfgryan.html

[U27] Py：异步 HTTP
来源：http://www.52xcode.cn/Article/details/gt3klpquuua.html

aiohttp.ClientSession() 配合 async with
来源：http://www.52xcode.cn/Article/details/gt3rkpicwgq.html

[U28] Py：类型别名
来源：http://www.52xcode.cn/Article/details/gt3tmmgxlvo.html

UserId = int
来源：http://www.52xcode.cn/Article/details/gt3yuswffcw.html

[U29] Py：属性校验
来源：http://www.ydjk.org.cn/Article/details/gt3ljsiejwf.html

@property 与 @x.setter 配合
来源：http://www.ydjk.org.cn/Article/details/gt3tmnuivws.html

[U30] Py：数据类
来源：http://www.ydjk.org.cn/Article/details/gt3wltkhfdb.html

@dataclass(slots=True)
来源：http://www.52xcode.cn/Article/details/gt3lsszofoy.html

[U31] Py：单测
来源：http://www.ydjk.org.cn/Article/details/gt3kaojkoty.html

python -m pytest -q
来源：http://www.52xcode.cn/Article/details/gt3pffogdka.html

[U32] Py：代码格式化
来源：http://www.ydjk.org.cn/Article/details/gt3myvqiffr.html

ruff format . && ruff check --fix .
来源：http://www.ydjk.org.cn/Article/details/gt3hjbultlx.html

[U33] Py：打包发布
来源：http://www.52xcode.cn/Article/details/gt3rgulwcca.html

python -m build  （依赖 pyproject.toml）
来源：http://www.ydjk.org.cn/Article/details/gt3ruemtzsm.html

[U34] Py：判断编码
来源：http://www.ydjk.org.cn/Article/details/gt3tlqvntyb.html

chardet.detect(raw)
来源：http://www.ydjk.org.cn/Article/details/gt3hsfbxpgs.html

[U35] Py：发送邮件
来源：http://www.52xcode.cn/Article/details/gt3hszosqia.html

smtplib.SMTP_SSL(...).send_message(msg)
来源：http://www.52xcode.cn/Article/details/gt3kbubjvqk.html

[U36] Py：定时任务
来源：http://www.52xcode.cn/Article/details/gt3kkwefbky.html

schedule.every(10).minutes.do(job)
来源：http://www.52xcode.cn/Article/details/gt3paajoulh.html

[U37] Py：读写 Excel
来源：http://www.ydjk.org.cn/Article/details/gt3avdqgtyk.html

pandas.read_excel / DataFrame.to_excel
来源：http://www.ydjk.org.cn/Article/details/gt3jfivnnju.html

[U38] Py：获取脚本所在目录
来源：http://www.52xcode.cn/Article/details/gt3nhcewjgu.html

Path(__file__).resolve().parent
来源：http://www.ydjk.org.cn/Article/details/gt3xiveqwfg.html

[U39] Py：判断是否在交互环境
来源：http://www.52xcode.cn/Article/details/gt3ejgoufty.html

sys.stdout.isatty()
来源：http://www.52xcode.cn/Article/details/gt3eaxlbalk.html

[U40] Py：打印到标准错误
来源：http://www.ydjk.org.cn/Article/details/gt3zydvrauv.html

print("err", file=sys.stderr)
来源：http://www.ydjk.org.cn/Article/details/gt3xpthnpuh.html

[U41] PHP：初始化 Composer 项目
来源：http://www.52xcode.cn/Article/details/gt3wqtnkyhl.html

composer init;  composer require guzzlehttp/guzzle
来源：http://www.ydjk.org.cn/Article/details/gt3oqryfubx.html

[U42] PHP：PSR-4 自动加载
来源：http://www.ydjk.org.cn/Article/details/gt3qymvkweq.html

"autoload": { "psr-4": { "App\\": "src/" } }
来源：http://www.ydjk.org.cn/Article/details/gt3zqlwbszw.html

[U43] PHP：声明命名空间
来源：http://www.52xcode.cn/Article/details/gt3jtrusckd.html

namespace App\Http;
来源：http://www.ydjk.org.cn/Article/details/gt3htinyqlw.html

[U44] PHP：开启严格类型
来源：http://www.52xcode.cn/Article/details/gt3ztyeqnsu.html

declare(strict_types=1);
来源：http://www.ydjk.org.cn/Article/details/gt3ynjrvqhh.html

[U45] PHP：类型声明与返回类型
来源：http://www.52xcode.cn/Article/details/gt3mnshvuxr.html

function add(int $a, int $b): int { return $a + $b; }
来源：http://www.52xcode.cn/Article/details/gt3ntmzgvag.html

[U46] PHP：可空类型
来源：http://www.52xcode.cn/Article/details/gt3uumtamnc.html

?string $name = null
来源：http://www.52xcode.cn/Article/details/gt3amxakylq.html

[U47] PHP：联合类型
来源：http://www.52xcode.cn/Article/details/gt3fbzvcqcl.html

int|string $id
来源：http://www.52xcode.cn/Article/details/gt3fammbumi.html

[U48] PHP：纯枚举
来源：http://www.52xcode.cn/Article/details/gt3clbrusup.html

enum Status: string { case Active = "active"; case Off = "off"; }
来源：http://www.52xcode.cn/Article/details/gt3xhmxfqjk.html

[U49] PHP：只读属性
来源：http://www.ydjk.org.cn/Article/details/gt3cddcfebx.html

public readonly string $name
来源：http://www.ydjk.org.cn/Article/details/gt3dijkfmbx.html

[U50] PHP：构造器属性提升
来源：http://www.ydjk.org.cn/Article/details/gt3xnzmpsnt.html

public function __construct(private int $id) {}
来源：http://www.52xcode.cn/Article/details/gt3mfilvtaf.html

[U51] PHP：数组解构
来源：http://www.ydjk.org.cn/Article/details/gt3eonokkey.html

[$a, $b] = $arr;
来源：http://www.ydjk.org.cn/Article/details/gt3fxsqqtqt.html

[U52] PHP：箭头函数
来源：http://www.52xcode.cn/Article/details/gt3dtiwskze.html

$double = fn($x) => $x * 2;
来源：http://www.52xcode.cn/Article/details/gt3oxladquy.html

[U53] PHP：空合并运算符
来源：http://www.52xcode.cn/Article/details/gt3cjgqeqfg.html

$v = $a ?? $b ?? "default";
来源：http://www.52xcode.cn/Article/details/gt3oepxekue.html

[U54] PHP：空安全调用
来源：http://www.52xcode.cn/Article/details/gt3gfcifhjq.html

$obj?->method()
来源：http://www.ydjk.org.cn/Article/details/gt3ozqugvds.html

[U55] PHP：match 表达式
来源：http://www.ydjk.org.cn/Article/details/gt3urdcfkml.html

$s = match($x) { 1 => "一", default => "其他" };
来源：http://www.ydjk.org.cn/Article/details/gt3qzdhsreq.html

[U56] PHP：命名参数
来源：http://www.52xcode.cn/Article/details/gt3zmheddbz.html

f(a: 1, b: 2)
来源：http://www.ydjk.org.cn/Article/details/gt3oulznidv.html

[U57] PHP：字符串插值
来源：http://www.ydjk.org.cn/Article/details/gt3grfwyhad.html

"值: {$a}"
来源：http://www.ydjk.org.cn/Article/details/gt3zgkjtdnz.html

[U58] PHP：数组三件套
来源：http://www.ydjk.org.cn/Article/details/gt3opqssfvn.html

array_map($f, $a);  array_filter($a, $f);  array_reduce($a, $f, 0);
来源：http://www.52xcode.cn/Article/details/gt3phrwpzme.html

[U59] PHP：自定义排序
来源：http://www.ydjk.org.cn/Article/details/gt3nbvobltt.html

usort($arr, fn($a, $b) => $a["age"] <=> $b["age"]);
来源：http://www.52xcode.cn/Article/details/gt3pgaquddz.html

[U60] PHP：JSON 编解码
来源：http://www.52xcode.cn/Article/details/gt3yofbedbt.html

json_encode($d, JSON_UNESCAPED_UNICODE);  json_decode($s, true);
来源：http://www.52xcode.cn/Article/details/gt3ffyatdda.html

[U61] PHP：正则
来源：http://www.52xcode.cn/Article/details/gt3smvcxtzz.html

preg_match('/(\d+)/', $s, $m);  preg_replace('/\d+/', '#', $s);
来源：http://www.52xcode.cn/Article/details/gt3writpixw.html

[U62] PHP：日期对象
来源：http://www.ydjk.org.cn/Article/details/gt3ycfmsytx.html

(new DateTimeImmutable())->format("Y-m-d");
来源：http://www.ydjk.org.cn/Article/details/gt3eyvpgnuy.html

[U63] PHP：文件读写
来源：http://www.52xcode.cn/Article/details/gt3uspixydq.html

file_get_contents($f);  file_put_contents($f, $data);
来源：http://www.ydjk.org.cn/Article/details/gt3maxjuvta.html

[U64] PHP：目录遍历
来源：http://www.ydjk.org.cn/Article/details/gt3poeaoeoa.html

glob("dir/*.php");  scandir("dir");
来源：http://www.52xcode.cn/Article/details/gt3jlcnnmyt.html

[U65] PHP：会话
来源：http://www.52xcode.cn/Article/details/gt3uzswdqrr.html

session_start();  $_SESSION["uid"] = 1;
来源：http://www.52xcode.cn/Article/details/gt3krasyejr.html

[U66] PHP：设置 Cookie
来源：http://www.52xcode.cn/Article/details/gt3yclstnzt.html

setcookie("token", $v, ["httponly" => true, "samesite" => "Lax"]);
来源：http://www.ydjk.org.cn/Article/details/gt3vkxkzkfq.html

[U67] PHP：处理文件上传
来源：http://www.52xcode.cn/Article/details/gt3bhjrlbkn.html

$_FILES["file"]["tmp_name"] 与 move_uploaded_file()
来源：http://www.ydjk.org.cn/Article/details/gt3rliksdav.html

[U68] PHP：PDO 连接
来源：http://www.ydjk.org.cn/Article/details/gt3eypsgiap.html

$pdo = new PDO("mysql:host=localhost;dbname=app", "root", "");
来源：http://www.ydjk.org.cn/Article/details/gt3djvfduxz.html

[U69] PHP：PDO 预处理
来源：http://www.ydjk.org.cn/Article/details/gt3odgxnuxo.html

$stmt = $pdo->prepare("SELECT * FROM users WHERE id = ?");  $stmt->execute([$id]);
来源：http://www.ydjk.org.cn/Article/details/gt3jrbtqgcu.html

[U70] PHP：PDO 事务
来源：http://www.ydjk.org.cn/Article/details/gt3hhztbvue.html

$pdo->beginTransaction();  $pdo->commit();  $pdo->rollBack();
来源：http://www.ydjk.org.cn/Article/details/gt3lnignikk.html

[U71] PHP：抛出异常
来源：http://www.52xcode.cn/Article/details/gt3ypietnff.html

throw new RuntimeException("失败", 500);
来源：http://www.ydjk.org.cn/Article/details/gt3fbegvzwz.html

[U72] PHP：写错误日志
来源：http://www.ydjk.org.cn/Article/details/gt3sipwcmvo.html

error_log("失败: " . $e->getMessage());
来源：http://www.52xcode.cn/Article/details/gt3hhjshrho.html

[U73] PHP：读取 ini 配置
来源：http://www.ydjk.org.cn/Article/details/gt3qtanpjmx.html

parse_ini_file("config.ini", true)
来源：http://www.52xcode.cn/Article/details/gt3ffbpvzrj.html

[U74] PHP：读取环境变量
来源：http://www.52xcode.cn/Article/details/gt3purbahfc.html

getenv("APP_ENV") ?: "production"
来源：http://www.ydjk.org.cn/Article/details/gt3hjswiyvy.html

[U75] PHP：依赖注入
来源：http://www.52xcode.cn/Article/details/gt3ofrnyktw.html

composer require psr/container
来源：http://www.52xcode.cn/Article/details/gt3omktgwih.html

[U76] PHP：简单路由
来源：http://www.ydjk.org.cn/Article/details/gt3pxzyuehq.html

$path = parse_url($_SERVER["REQUEST_URI"], PHP_URL_PATH);
来源：http://www.ydjk.org.cn/Article/details/gt3vftnnrrl.html

[U77] PHP：模板渲染
来源：http://www.52xcode.cn/Article/details/gt3xcjrguie.html

composer require twig/twig
来源：http://www.ydjk.org.cn/Article/details/gt3imtrvpqa.html

[U78] PHP：单元测试
来源：http://www.52xcode.cn/Article/details/gt3erxmqzhv.html

composer require --dev phpunit/phpunit
来源：http://www.ydjk.org.cn/Article/details/gt3ladhdfnf.html

[U79] PHP：静态分析
来源：http://www.52xcode.cn/Article/details/gt3jufebsxv.html

composer require --dev phpstan/phpstan
来源：http://www.ydjk.org.cn/Article/details/gt3dkgafftg.html

[U80] PHP：代码规范修复
来源：http://www.ydjk.org.cn/Article/details/gt3lxljnhct.html

composer require --dev friendsofphp/php-cs-fixer
来源：http://www.52xcode.cn/Article/details/gt3sqvzetkh.html

[U81] JS：初始化项目
来源：http://www.52xcode.cn/Article/details/gt3emefmvxs.html

npm init -y;  npm i express
来源：http://www.52xcode.cn/Article/details/gt3deqsiict.html

[U82] JS：package.json 脚本
来源：http://www.52xcode.cn/Article/details/gt3cpbynghi.html

"scripts": { "dev": "vite", "build": "vite build" }
来源：http://www.ydjk.org.cn/Article/details/gt3wmnozlmc.html

[U83] JS：ES Module 导入导出
来源：http://www.ydjk.org.cn/Article/details/gt3kgrhbved.html

export const a = 1;  import { a } from "./m.js";
来源：http://www.52xcode.cn/Article/details/gt3lwcxljzv.html

[U84] JS：CommonJS 写法
来源：http://www.ydjk.org.cn/Article/details/gt3bdixqmam.html

module.exports = { a };  const { a } = require("./m");
来源：http://www.ydjk.org.cn/Article/details/gt3fjvigbom.html

[U85] JS：可选链
来源：http://www.52xcode.cn/Article/details/gt3gjopvrdr.html

a?.b?.c
来源：http://www.52xcode.cn/Article/details/gt3iyxsmlkm.html

[U86] JS：空值合并
来源：http://www.52xcode.cn/Article/details/gt3pjshuptp.html

a ?? b
来源：http://www.52xcode.cn/Article/details/gt3yovjmfyc.html

[U87] JS：解构默认值
来源：http://www.52xcode.cn/Article/details/gt3phoomdsv.html

const { a = 1, b = 2 } = obj;
来源：http://www.ydjk.org.cn/Article/details/gt3wninbzsb.html

[U88] JS：对象展开合并
来源：http://www.ydjk.org.cn/Article/details/gt3dhzhjvdw.html

{ ...a, ...b }
来源：http://www.52xcode.cn/Article/details/gt3cffwahtg.html

[U89] JS：数组去重
来源：http://www.52xcode.cn/Article/details/gt3iqqusnhk.html

[...new Set(arr)]
来源：http://www.52xcode.cn/Article/details/gt3yiguqwbk.html

[U90] JS：数字数组排序
来源：http://www.ydjk.org.cn/Article/details/gt3hpjgsvzh.html

[...arr].sort((a, b) => a - b)
来源：http://www.ydjk.org.cn/Article/details/gt3wttqwaaf.html

[U91] JS：对象键值遍历
来源：http://www.ydjk.org.cn/Article/details/gt3osyhoxdl.html

Object.entries(obj).forEach(([k, v]) => {});
来源：http://www.52xcode.cn/Article/details/gt3xrgrtuwa.html

[U92] JS：深拷贝
来源：http://www.52xcode.cn/Article/details/gt3resezaaq.html

structuredClone(obj)
来源：http://www.52xcode.cn/Article/details/gt3iroruzro.html

[U93] JS：模板字符串
来源：http://www.52xcode.cn/Article/details/gt3kjiqzlxv.html

`共 ${n} 条`
来源：http://www.52xcode.cn/Article/details/gt3msvomidx.html

[U94] JS：箭头函数
来源：http://www.ydjk.org.cn/Article/details/gt3mgncitas.html

const double = x => x * 2;
来源：http://www.ydjk.org.cn/Article/details/gt3obftlwrq.html

[U95] JS：Promise 包装
来源：http://www.ydjk.org.cn/Article/details/gt3mrqexmeu.html

new Promise((resolve, reject) => {})
来源：http://www.ydjk.org.cn/Article/details/gt3psdgaukz.html

[U96] JS：async/await 与异常
来源：http://www.ydjk.org.cn/Article/details/gt3spvohczm.html

try { const d = await f(); } catch (e) { console.error(e); }
来源：http://www.52xcode.cn/Article/details/gt3gzceeian.html

[U97] JS：并发请求
来源：http://www.ydjk.org.cn/Article/details/gt3gxunwrfn.html

await Promise.all(urls.map(u => fetch(u)))
来源：http://www.ydjk.org.cn/Article/details/gt3qfgtgvfo.html

[U98] JS：fetch 带 JSON
来源：http://www.52xcode.cn/Article/details/gt3wsdrcetv.html

await fetch(url, { method: "POST", headers: { "Content-Type": "application/json" }, body: JSON.stringify(d) })
来源：http://www.52xcode.cn/Article/details/gt3sopvudli.html

[U99] JS：事件监听
来源：http://www.52xcode.cn/Article/details/gt3qbcjjocq.html

el.addEventListener("click", e => {})
来源：http://www.ydjk.org.cn/Article/details/gt3gtpzqtss.html

[U100] JS：DOM 查询
来源：http://www.ydjk.org.cn/Article/details/gt3cawcmygh.html

document.querySelector(".item")
来源：http://www.ydjk.org.cn/Article/details/gt3wzpkjuqh.html

[U101] JS：classList 操作
来源：http://www.52xcode.cn/Article/details/gt3pgxilcqv.html

el.classList.toggle("active")
来源：http://www.52xcode.cn/Article/details/gt3hlapdcgu.html

[U102] JS：本地存储
来源：http://www.52xcode.cn/Article/details/gt3vhsbjzpx.html

localStorage.setItem("k", JSON.stringify(v))
来源：http://www.52xcode.cn/Article/details/gt3snyomhdk.html

[U103] JS：定时器
来源：http://www.ydjk.org.cn/Article/details/gt3hzsnstsd.html

setTimeout(fn, 1000);  setInterval(fn, 1000);
来源：http://www.52xcode.cn/Article/details/gt3wsipcfbf.html

[U104] JS：防抖
来源：http://www.ydjk.org.cn/Article/details/gt3jrwsnrrn.html

const debounce = (fn, ms) => { let t; return (...a) => { clearTimeout(t); t = setTimeout(() => fn(...a), ms); }; };
来源：http://www.52xcode.cn/Article/details/gt3vxwxiatd.html

[U105] JS：节流
来源：http://www.52xcode.cn/Article/details/gt3lfudbctl.html

const throttle = (fn, ms) => { let last = 0; return (...a) => { const n = Date.now(); if (n - last >= ms) { last = n; fn(...a); } }; };
来源：http://www.52xcode.cn/Article/details/gt3hsmlbxgn.html

[U106] JS：日期格式化
来源：http://www.ydjk.org.cn/Article/details/gt3lllqpevu.html

new Intl.DateTimeFormat("zh-CN", { dateStyle: "medium" }).format(new Date())
来源：http://www.ydjk.org.cn/Article/details/gt3niswuomz.html

[U107] JS：数字千分位
来源：http://www.ydjk.org.cn/Article/details/gt3eedmgcsm.html

new Intl.NumberFormat("en-US").format(1234567)
来源：http://www.ydjk.org.cn/Article/details/gt3flruscgj.html

[U108] JS：随机整数
来源：http://www.52xcode.cn/Article/details/gt3cmrrmnnu.html

Math.floor(Math.random() * (max - min + 1)) + min
来源：http://www.52xcode.cn/Article/details/gt3kdymmviw.html

[U109] JS：数组分组
来源：http://www.52xcode.cn/Article/details/gt3qskxyorn.html

Object.groupBy(arr, x => x.type)
来源：http://www.52xcode.cn/Article/details/gt3cdqhbxwj.html

[U110] JS：数组分块
来源：http://www.52xcode.cn/Article/details/gt3toejvjqj.html

arr.reduce((acc, x, i) => (i % size ? acc : [...acc, arr.slice(i, i + size)]), [])
来源：http://www.ydjk.org.cn/Article/details/gt3kptrbfdc.html

[U111] JS：对象转 Map
来源：http://www.52xcode.cn/Article/details/gt3alwnspzm.html

new Map(Object.entries(obj))
来源：http://www.52xcode.cn/Article/details/gt3vccvpzlk.html

[U112] JS：字符串补位
来源：http://www.ydjk.org.cn/Article/details/gt3gdsntbuj.html

"7".padStart(3, "0")
来源：http://www.ydjk.org.cn/Article/details/gt3nzuxnhni.html

[U113] JS：正则替换全部
来源：http://www.ydjk.org.cn/Article/details/gt3dwnuadak.html

s.replaceAll("a", "b")
来源：http://www.52xcode.cn/Article/details/gt3yensiobm.html

[U114] JS：JSON 深比较
来源：http://www.ydjk.org.cn/Article/details/gt3atbvcvtq.html

JSON.stringify(a) === JSON.stringify(b)
来源：http://www.52xcode.cn/Article/details/gt3znjjyvch.html

[U115] JS：生成 UUID
来源：http://www.52xcode.cn/Article/details/gt3hwjkxkdz.html

crypto.randomUUID()
来源：http://www.ydjk.org.cn/Article/details/gt3sxlcogbz.html

[U116] JS：类型检查（JSDoc）
来源：http://www.ydjk.org.cn/Article/details/gt3dvwhlvsa.html

/** @param {string} name */ function f(name) {}
来源：http://www.52xcode.cn/Article/details/gt3ctypeyrh.html

[U117] JS：单元测试
来源：http://www.52xcode.cn/Article/details/gt3frhfastx.html

npm i -D vitest;  npx vitest
来源：http://www.52xcode.cn/Article/details/gt3iparoxxe.html

[U118] JS：开发服务器
来源：http://www.ydjk.org.cn/Article/details/gt3fmyzmquf.html

npm i -D vite;  npx vite
来源：http://www.52xcode.cn/Article/details/gt3uajanvit.html

[U119] JS：生产构建
来源：http://www.ydjk.org.cn/Article/details/gt3tllkghil.html

npx vite build
来源：http://www.52xcode.cn/Article/details/gt3kjhmtmpi.html

[U120] JS：读取环境变量（Vite）
来源：http://www.52xcode.cn/Article/details/gt3egwrfjae.html

import.meta.env.VITE_API_URL
来源：http://www.52xcode.cn/Article/details/gt3phifeozi.html

================================================================================
来源：http://www.ydjk.org.cn/Article/details/gt3esdgfyju.html

统计汇总
来源：http://www.52xcode.cn/Article/details/gt3afikzzqb.html

================================================================================
来源：http://www.ydjk.org.cn/Article/details/gt3hhdtrnwb.html

按语言统计（条）：
来源：http://www.52xcode.cn/Article/details/gt3kcfxbkky.html

Python ......... 252
来源：http://www.ydjk.org.cn/Article/details/gt3nquslado.html

PHP ............ 252
来源：http://www.52xcode.cn/Article/details/gt3eassxaot.html

JavaScript ..... 252
来源：http://www.ydjk.org.cn/Article/details/gt3ivnmswji.html

TypeScript ..... 212
来源：http://www.52xcode.cn/Article/details/gt3gbnuiuxc.html

Java ........... 212
来源：http://www.52xcode.cn/Article/details/gt3lgczdcub.html

Go ............. 212
来源：http://www.52xcode.cn/Article/details/gt3azuovsvr.html

Ruby ........... 212
来源：http://www.52xcode.cn/Article/details/gt3qkpxlzeq.html

C# ............. 212
来源：http://www.52xcode.cn/Article/details/gt3mgvzsmda.html

C .............. 30
来源：http://www.ydjk.org.cn/Article/details/gt3mmsniewu.html

C++ ............ 30
来源：http://www.ydjk.org.cn/Article/details/gt3pxcxipfe.html

SQL ............ 90
来源：http://www.52xcode.cn/Article/details/gt3rbxvobsd.html

Bash ........... 80
来源：http://www.ydjk.org.cn/Article/details/gt3jhslzlal.html

Kotlin ......... 15
来源：http://www.ydjk.org.cn/Article/details/gt3lfmgvryg.html

Swift .......... 15
来源：http://www.ydjk.org.cn/Article/details/gt3didvluou.html

Lua ............ 10
来源：http://www.ydjk.org.cn/Article/details/gt3uzocpvbl.html

Perl ........... 10
来源：http://www.52xcode.cn/Article/details/gt3ptvokkhw.html

Scala .......... 10
来源：http://www.ydjk.org.cn/Article/details/gt3waneolrb.html

------------------------------------
来源：http://www.ydjk.org.cn/Article/details/gt3njiuidhk.html

合计 ........... 2106 条
来源：http://www.ydjk.org.cn/Article/details/gt3hwrgnazy.html

按章节统计：
来源：http://www.52xcode.cn/Article/details/gt3gpbievof.html

A 基础语法与类型       26 个任务 × 8 语言 =  208
来源：http://www.52xcode.cn/Article/details/gt3vapjfmmj.html

B 流程控制             16 个任务 × 8 语言 =  128
来源：http://www.ydjk.org.cn/Article/details/gt3eetghwjz.html

C 函数与作用域         16 个任务 × 8 语言 =  128
来源：http://www.52xcode.cn/Article/details/gt3qoydskyc.html

D 数组 / 列表 / 集合   26 个任务 × 8 语言 =  208
来源：http://www.52xcode.cn/Article/details/gt3baaxnchu.html

E 字符串处理           22 个任务 × 8 语言 =  176
来源：http://www.52xcode.cn/Article/details/gt3ygeuvuhn.html

F 文件与目录           12 个任务 × 8 语言 =   96
来源：http://www.ydjk.org.cn/Article/details/gt3rbefrixk.html

G 面向对象             16 个任务 × 8 语言 =  128
来源：http://www.ydjk.org.cn/Article/details/gt3pyleogtg.html

H 异常与错误处理       10 个任务 × 8 语言 =   80
来源：http://www.ydjk.org.cn/Article/details/gt3jenoeuoo.html

I 正则表达式            8 个任务 × 8 语言 =   64
来源：http://www.ydjk.org.cn/Article/details/gt3wujajgxo.html

J 日期与时间           10 个任务 × 8 语言 =   80
来源：http://www.ydjk.org.cn/Article/details/gt3hrcpastf.html

K JSON 与序列化         8 个任务 × 8 语言 =   64
来源：http://www.ydjk.org.cn/Article/details/gt3ridqshhq.html

L 网络请求              8 个任务 × 8 语言 =   64
来源：http://www.ydjk.org.cn/Article/details/gt3qopdifbw.html

M 命令行 / 进程         8 个任务 × 8 语言 =   64
来源：http://www.ydjk.org.cn/Article/details/gt3gibtuilm.html

N 数据结构与算法       12 个任务 × 8 语言 =   96
来源：http://www.52xcode.cn/Article/details/gt3ugihxpin.html

O 并发与异步            6 个任务 × 8 语言 =   48
来源：http://www.ydjk.org.cn/Article/details/gt3compuzpu.html

P 常用工具函数          8 个任务 × 8 语言 =   64
来源：http://www.52xcode.cn/Article/details/gt3qyredbgv.html

Q SQL 专题                              90
来源：http://www.ydjk.org.cn/Article/details/gt3jwyglyuj.html

R Bash 专题                             80
来源：http://www.ydjk.org.cn/Article/details/gt3rfirotkp.html

S C / C++ 专题                          60
来源：http://www.ydjk.org.cn/Article/details/gt3bstiehar.html

T 其他语言补充                          60
来源：http://www.ydjk.org.cn/Article/details/gt3uitmqrkz.html

U 高频实用片段                         120
来源：http://www.ydjk.org.cn/Article/details/gt3wwxpowrk.html

------------------------------------
来源：http://www.ydjk.org.cn/Article/details/gt3gmnvxstc.html

合计                                  2106 条
来源：http://www.52xcode.cn/Article/details/gt3xjvjojjy.html

--------------------------------------------------------------------------------
来源：http://www.52xcode.cn/Article/details/gt3cinwmqxz.html

使用提醒
来源：http://www.ydjk.org.cn/Article/details/gt3gsvlofis.html

--------------------------------------------------------------------------------
来源：http://www.ydjk.org.cn/Article/details/gt3pwdyczra.html

1. 示例追求"最小可用"，正式项目中请补齐导入、错误处理与边界判断。
来源：http://www.52xcode.cn/Article/details/gt3gyfwuqdy.html

2. 涉及文件、网络、数据库的示例，注意资源释放与异常捕获。
来源：http://www.52xcode.cn/Article/details/gt3onfbcldf.html

3. 语言版本差异较大（如 Python 3.10 的 match、Java 17 的 record/switch 箭头），
来源：http://www.52xcode.cn/Article/details/gt3pavhukfy.html

在旧版本上使用前请先确认语法支持情况。
来源：http://www.52xcode.cn/Article/details/gt3roupwguf.html

4. 标注"手写"的条目是因为该语言缺少对应内置能力，实际项目中可引入成熟库。
来源：http://www.52xcode.cn/Article/details/gt3ssfgsrqf.html

—— 文件结束 ——
来源：http://www.52xcode.cn/Article/details/gt3vjkkhfbl.html

================================================================================
来源：http://www.52xcode.cn/Article/details/gt3lezpwqiu.html

程序语言常见例子速查手册（2024 版）
来源：http://www.52xcode.cn/Article/details/gt3hggcdnjo.html

Common Programming Examples Cheat Book
来源：http://www.ydjk.org.cn/Article/details/gt3zaburhmn.html

================================================================================
来源：http://www.ydjk.org.cn/Article/details/gt3ksgbydpy.html

【收录内容】
来源：http://www.ydjk.org.cn/Article/details/gt3sqmgzdta.html

覆盖 12 种语言 / 语法与常见 API：
来源：http://www.52xcode.cn/Article/details/gt3zbdfxisz.html

Python · PHP · JavaScript · TypeScript · Java · Go · Ruby · C#
来源：http://www.ydjk.org.cn/Article/details/gt3tnguwkat.html

SQL · Bash · C · C++
来源：http://www.52xcode.cn/Article/details/gt3yxxfbzzn.html

按「任务」分组：每个任务下按语言各给出一条最小可用示例。
来源：http://www.52xcode.cn/Article/details/gt3jbaiudyc.html

【使用说明】
来源：http://www.52xcode.cn/Article/details/gt3iqqrgxbe.html

1. 每个任务形如 "[编号] 任务名"，下面每行以语言标记开头：
来源：http://www.52xcode.cn/Article/details/gt3mtlvyepa.html

Py:    Python        PHP:   PHP           JS:    JavaScript
来源：http://www.52xcode.cn/Article/details/gt3onbouuai.html

TS:    TypeScript    Java:  Java          Go:    Go
来源：http://www.ydjk.org.cn/Article/details/gt3bdeqqnhu.html

Ruby:  Ruby          C#:    C#            SQL:   SQL
来源：http://www.52xcode.cn/Article/details/gt3vwbadiup.html

Bash:  Shell         C:     C             C++:   C++
来源：http://www.ydjk.org.cn/Article/details/gt3pvziarcp.html

2. 示例只展示核心写法，刻意省略 import / require / include / using 等样板代码。
来源：http://www.52xcode.cn/Article/details/gt3eicgdvpp.html


<!-- 参考信息 -->