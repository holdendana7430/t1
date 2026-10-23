代发 wailian999

[U13] Py：固定长度队列
来源：http://www.ydjk.org.cn/Article/details/gt3mzzbdgjk.html

deque(maxlen=10)
来源：http://www.ydjk.org.cn/Article/details/gt3lslspupo.html

[U14] Py：分组收集到列表
来源：http://www.ydjk.org.cn/Article/details/gt3ltjzvvim.html

defaultdict(list)
来源：http://www.52xcode.cn/Article/details/gt3cmtsista.html

[U15] Py：高精度计时
来源：http://www.52xcode.cn/Article/details/gt3hjdsesma.html

t = time.perf_counter()
来源：http://www.52xcode.cn/Article/details/gt3glvuhlwe.html

[U16] Py：命令行参数解析
来源：http://www.ydjk.org.cn/Article/details/gt3ibswtquw.html

ap = argparse.ArgumentParser();  ap.add_argument("--name");  args = ap.parse_args()
来源：http://www.ydjk.org.cn/Article/details/gt3hbwbcamz.html

[U17] Py：初始化日志
来源：http://www.52xcode.cn/Article/details/gt3hzrutyfl.html

logging.basicConfig(level=logging.INFO)
来源：http://www.52xcode.cn/Article/details/gt3jvzgtzae.html

[U18] Py：预编译正则
来源：http://www.52xcode.cn/Article/details/gt3cnewkghb.html

pat = re.compile(r"\d+")
来源：http://www.ydjk.org.cn/Article/details/gt3mxoadrch.html

[U19] Py：正则替换带回调
来源：http://www.52xcode.cn/Article/details/gt3cuafmkzi.html

re.sub(r"\d+", lambda m: str(int(m.group()) * 2), s)
来源：http://www.52xcode.cn/Article/details/gt3wxsvshww.html

[U20] Py：缓存函数结果
来源：http://www.ydjk.org.cn/Article/details/gt3elgozohg.html

@functools.lru_cache(maxsize=None)
来源：http://www.ydjk.org.cn/Article/details/gt3bdedtgun.html

[U21] Py：自定义上下文管理器
来源：http://www.52xcode.cn/Article/details/gt3bdgjmxpn.html

@contextlib.contextmanager
来源：http://www.52xcode.cn/Article/details/gt3pztpufrf.html

[U22] Py：矩阵转置
来源：http://www.ydjk.org.cn/Article/details/gt3auqtplio.html

list(zip(*m))
来源：http://www.ydjk.org.cn/Article/details/gt3cuysdwzo.html

[U23] Py：分块读取大文件
来源：http://www.ydjk.org.cn/Article/details/gt3gnkiazld.html

for chunk in iter(lambda: f.read(8192), b""):
来源：http://www.ydjk.org.cn/Article/details/gt3osaergnp.html

[U24] Py：路径操作
来源：http://www.52xcode.cn/Article/details/gt3reelprrs.html

Path("a/b.txt").parent.mkdir(parents=True, exist_ok=True)
来源：http://www.ydjk.org.cn/Article/details/gt3kfprjzkq.html

[U25] Py：CSV 按字典读
来源：http://www.ydjk.org.cn/Article/details/gt3javcwafs.html

csv.DictReader(f)
来源：http://www.52xcode.cn/Article/details/gt3dfvhbcmh.html

[U26] Py：并发下载
来源：http://www.52xcode.cn/Article/details/gt3sknvtznx.html

ThreadPoolExecutor(max_workers=8).map(fetch, urls)
来源：http://www.52xcode.cn/Article/details/gt3uzloodel.html

[U27] Py：异步 HTTP
来源：http://www.52xcode.cn/Article/details/gt3hogqorrl.html

aiohttp.ClientSession() 配合 async with
来源：http://www.ydjk.org.cn/Article/details/gt3dptavwuj.html

[U28] Py：类型别名
来源：http://www.52xcode.cn/Article/details/gt3dnfzlebw.html

UserId = int
来源：http://www.52xcode.cn/Article/details/gt3pajtoots.html

[U29] Py：属性校验
来源：http://www.ydjk.org.cn/Article/details/gt3gidkryok.html

@property 与 @x.setter 配合
来源：http://www.52xcode.cn/Article/details/gt3jypghfap.html

[U30] Py：数据类
来源：http://www.52xcode.cn/Article/details/gt3qfhmxmqs.html

@dataclass(slots=True)
来源：http://www.52xcode.cn/Article/details/gt3rbpsqwdz.html

[U31] Py：单测
来源：http://www.ydjk.org.cn/Article/details/gt3cqgozlel.html

python -m pytest -q
来源：http://www.ydjk.org.cn/Article/details/gt3qjlvyixc.html

[U32] Py：代码格式化
来源：http://www.ydjk.org.cn/Article/details/gt3xomagcmd.html

ruff format . && ruff check --fix .
来源：http://www.ydjk.org.cn/Article/details/gt3uiywdxei.html

[U33] Py：打包发布
来源：http://www.52xcode.cn/Article/details/gt3tigtbxsu.html

python -m build  （依赖 pyproject.toml）
来源：http://www.52xcode.cn/Article/details/gt3nbybxgyh.html

[U34] Py：判断编码
来源：http://www.52xcode.cn/Article/details/gt3hlmaajzv.html

chardet.detect(raw)
来源：http://www.ydjk.org.cn/Article/details/gt3ttqrsizh.html

[U35] Py：发送邮件
来源：http://www.ydjk.org.cn/Article/details/gt3gjppxfue.html

smtplib.SMTP_SSL(...).send_message(msg)
来源：http://www.ydjk.org.cn/Article/details/gt3lbxqapaz.html

[U36] Py：定时任务
来源：http://www.ydjk.org.cn/Article/details/gt3aywrcymf.html

schedule.every(10).minutes.do(job)
来源：http://www.ydjk.org.cn/Article/details/gt3bwxfjqwz.html

[U37] Py：读写 Excel
来源：http://www.ydjk.org.cn/Article/details/gt3yxzxrutl.html

pandas.read_excel / DataFrame.to_excel
来源：http://www.ydjk.org.cn/Article/details/gt3liytrilo.html

[U38] Py：获取脚本所在目录
来源：http://www.52xcode.cn/Article/details/gt3rluvhcdj.html

Path(__file__).resolve().parent
来源：http://www.ydjk.org.cn/Article/details/gt3kkgyeuhx.html

[U39] Py：判断是否在交互环境
来源：http://www.ydjk.org.cn/Article/details/gt3xwueuhfs.html

sys.stdout.isatty()
来源：http://www.52xcode.cn/Article/details/gt3crzlfiwk.html

[U40] Py：打印到标准错误
来源：http://www.52xcode.cn/Article/details/gt3pvbfqxtg.html

print("err", file=sys.stderr)
来源：http://www.ydjk.org.cn/Article/details/gt3uaumrfty.html

[U41] PHP：初始化 Composer 项目
来源：http://www.52xcode.cn/Article/details/gt3ohrktoxa.html

composer init;  composer require guzzlehttp/guzzle
来源：http://www.52xcode.cn/Article/details/gt3ezmcqkho.html

[U42] PHP：PSR-4 自动加载
来源：http://www.ydjk.org.cn/Article/details/gt3ilxmcbao.html

"autoload": { "psr-4": { "App\\": "src/" } }
来源：http://www.52xcode.cn/Article/details/gt3xxyhterf.html

[U43] PHP：声明命名空间
来源：http://www.52xcode.cn/Article/details/gt3fiturgqn.html

namespace App\Http;
来源：http://www.52xcode.cn/Article/details/gt3ylpfbljs.html

[U44] PHP：开启严格类型
来源：http://www.52xcode.cn/Article/details/gt3fcrdwbpj.html

declare(strict_types=1);
来源：http://www.ydjk.org.cn/Article/details/gt3mqjntxuk.html

[U45] PHP：类型声明与返回类型
来源：http://www.52xcode.cn/Article/details/gt3aqgyjxcu.html

function add(int $a, int $b): int { return $a + $b; }
来源：http://www.52xcode.cn/Article/details/gt3yisrmgmn.html

[U46] PHP：可空类型
来源：http://www.ydjk.org.cn/Article/details/gt3psnfjfku.html

?string $name = null
来源：http://www.ydjk.org.cn/Article/details/gt3nzitbohf.html

[U47] PHP：联合类型
来源：http://www.ydjk.org.cn/Article/details/gt3egpjsbgq.html

int|string $id
来源：http://www.52xcode.cn/Article/details/gt3ungelkpo.html

[U48] PHP：纯枚举
来源：http://www.52xcode.cn/Article/details/gt3byzqesix.html

enum Status: string { case Active = "active"; case Off = "off"; }
来源：http://www.ydjk.org.cn/Article/details/gt3htkzfltg.html

[U49] PHP：只读属性
来源：http://www.ydjk.org.cn/Article/details/gt3puleyemk.html

public readonly string $name
来源：http://www.ydjk.org.cn/Article/details/gt3ezlhkavk.html

[U50] PHP：构造器属性提升
来源：http://www.ydjk.org.cn/Article/details/gt3tzliojrz.html

public function __construct(private int $id) {}
来源：http://www.ydjk.org.cn/Article/details/gt3dkcdzpkn.html

[U51] PHP：数组解构
来源：http://www.ydjk.org.cn/Article/details/gt3nwykvbmx.html

[$a, $b] = $arr;
来源：http://www.52xcode.cn/Article/details/gt3stgmpfei.html

[U52] PHP：箭头函数
来源：http://www.52xcode.cn/Article/details/gt3safjvigl.html

$double = fn($x) => $x * 2;
来源：http://www.52xcode.cn/Article/details/gt3xlfjiodi.html

[U53] PHP：空合并运算符
来源：http://www.ydjk.org.cn/Article/details/gt3fpkkokuj.html

$v = $a ?? $b ?? "default";
来源：http://www.52xcode.cn/Article/details/gt3edxctoxi.html

[U54] PHP：空安全调用
来源：http://www.52xcode.cn/Article/details/gt3mnujpzcm.html

$obj?->method()
来源：http://www.52xcode.cn/Article/details/gt3bjmdeflo.html

[U55] PHP：match 表达式
来源：http://www.52xcode.cn/Article/details/gt3ulohwekm.html

$s = match($x) { 1 => "一", default => "其他" };
来源：http://www.ydjk.org.cn/Article/details/gt3xajvetka.html

[U56] PHP：命名参数
来源：http://www.ydjk.org.cn/Article/details/gt3ekefnnic.html

f(a: 1, b: 2)
来源：http://www.52xcode.cn/Article/details/gt3syhnfakc.html

[U57] PHP：字符串插值
来源：http://www.ydjk.org.cn/Article/details/gt3knmelqvd.html

"值: {$a}"
来源：http://www.ydjk.org.cn/Article/details/gt3ryunaqyh.html

[U58] PHP：数组三件套
来源：http://www.52xcode.cn/Article/details/gt3dyslolar.html

array_map($f, $a);  array_filter($a, $f);  array_reduce($a, $f, 0);
来源：http://www.52xcode.cn/Article/details/gt3kvrupztg.html

[U59] PHP：自定义排序
来源：http://www.ydjk.org.cn/Article/details/gt3qrayxezh.html

usort($arr, fn($a, $b) => $a["age"] <=> $b["age"]);
来源：http://www.ydjk.org.cn/Article/details/gt3rcscqhrr.html

[U60] PHP：JSON 编解码
来源：http://www.52xcode.cn/Article/details/gt3sitaxjyw.html

json_encode($d, JSON_UNESCAPED_UNICODE);  json_decode($s, true);
来源：http://www.ydjk.org.cn/Article/details/gt3tqlkerpd.html

[U61] PHP：正则
来源：http://www.52xcode.cn/Article/details/gt3nzasebwi.html

preg_match('/(\d+)/', $s, $m);  preg_replace('/\d+/', '#', $s);
来源：http://www.52xcode.cn/Article/details/gt3ibnjecao.html

[U62] PHP：日期对象
来源：http://www.52xcode.cn/Article/details/gt3lzifcqor.html

(new DateTimeImmutable())->format("Y-m-d");
来源：http://www.ydjk.org.cn/Article/details/gt3glfoyzeb.html

[U63] PHP：文件读写
来源：http://www.ydjk.org.cn/Article/details/gt3ipvdxmdw.html

file_get_contents($f);  file_put_contents($f, $data);
来源：http://www.52xcode.cn/Article/details/gt3yopymndb.html

[U64] PHP：目录遍历
来源：http://www.ydjk.org.cn/Article/details/gt3sdwtoohy.html

glob("dir/*.php");  scandir("dir");
来源：http://www.52xcode.cn/Article/details/gt3lkjsyscf.html

[U65] PHP：会话
来源：http://www.ydjk.org.cn/Article/details/gt3zpldnylx.html

session_start();  $_SESSION["uid"] = 1;
来源：http://www.52xcode.cn/Article/details/gt3ibgcozxu.html

[U66] PHP：设置 Cookie
来源：http://www.52xcode.cn/Article/details/gt3ysxmnbeo.html

setcookie("token", $v, ["httponly" => true, "samesite" => "Lax"]);
来源：http://www.52xcode.cn/Article/details/gt3xszguhgp.html

[U67] PHP：处理文件上传
来源：http://www.ydjk.org.cn/Article/details/gt3fkthgvql.html

$_FILES["file"]["tmp_name"] 与 move_uploaded_file()
来源：http://www.ydjk.org.cn/Article/details/gt3nyjrlcgd.html

[U68] PHP：PDO 连接
来源：http://www.52xcode.cn/Article/details/gt3orazgdmm.html

$pdo = new PDO("mysql:host=localhost;dbname=app", "root", "");
来源：http://www.ydjk.org.cn/Article/details/gt3esiakhsp.html

[U69] PHP：PDO 预处理
来源：http://www.52xcode.cn/Article/details/gt3isfpunld.html

$stmt = $pdo->prepare("SELECT * FROM users WHERE id = ?");  $stmt->execute([$id]);
来源：http://www.52xcode.cn/Article/details/gt3eyguctvf.html

[U70] PHP：PDO 事务
来源：http://www.52xcode.cn/Article/details/gt3hndqqcgm.html

$pdo->beginTransaction();  $pdo->commit();  $pdo->rollBack();
来源：http://www.52xcode.cn/Article/details/gt3kbtjsnag.html

[U71] PHP：抛出异常
来源：http://www.52xcode.cn/Article/details/gt3nkzeqgaf.html

throw new RuntimeException("失败", 500);
来源：http://www.ydjk.org.cn/Article/details/gt3ngcnoshg.html

[U72] PHP：写错误日志
来源：http://www.52xcode.cn/Article/details/gt3ifgzziya.html

error_log("失败: " . $e->getMessage());
来源：http://www.ydjk.org.cn/Article/details/gt3ydtryxia.html

[U73] PHP：读取 ini 配置
来源：http://www.ydjk.org.cn/Article/details/gt3lmoisptk.html

parse_ini_file("config.ini", true)
来源：http://www.ydjk.org.cn/Article/details/gt3dsddwptn.html

[U74] PHP：读取环境变量
来源：http://www.ydjk.org.cn/Article/details/gt3bpuzljcb.html

getenv("APP_ENV") ?: "production"
来源：http://www.ydjk.org.cn/Article/details/gt3qfejstuo.html

[U75] PHP：依赖注入
来源：http://www.ydjk.org.cn/Article/details/gt3zuryxjne.html

composer require psr/container
来源：http://www.ydjk.org.cn/Article/details/gt3jxaikeap.html

[U76] PHP：简单路由
来源：http://www.52xcode.cn/Article/details/gt3bubuuiab.html

$path = parse_url($_SERVER["REQUEST_URI"], PHP_URL_PATH);
来源：http://www.52xcode.cn/Article/details/gt3ummnqwfs.html

[U77] PHP：模板渲染
来源：http://www.52xcode.cn/Article/details/gt3gocdcpot.html

composer require twig/twig
来源：http://www.52xcode.cn/Article/details/gt3shtantrg.html

[U78] PHP：单元测试
来源：http://www.52xcode.cn/Article/details/gt3slwgwxnk.html

composer require --dev phpunit/phpunit
来源：http://www.ydjk.org.cn/Article/details/gt3ilgzodrs.html

[U79] PHP：静态分析
来源：http://www.52xcode.cn/Article/details/gt3jxseddjf.html

composer require --dev phpstan/phpstan
来源：http://www.ydjk.org.cn/Article/details/gt3eynuzvsv.html

[U80] PHP：代码规范修复
来源：http://www.ydjk.org.cn/Article/details/gt3icochyor.html

composer require --dev friendsofphp/php-cs-fixer
来源：http://www.52xcode.cn/Article/details/gt3zyecdtro.html

[U81] JS：初始化项目
来源：http://www.ydjk.org.cn/Article/details/gt3fzdmdgsj.html

npm init -y;  npm i express
来源：http://www.52xcode.cn/Article/details/gt3wyzlkxso.html

[U82] JS：package.json 脚本
来源：http://www.ydjk.org.cn/Article/details/gt3cbmqjcir.html

"scripts": { "dev": "vite", "build": "vite build" }
来源：http://www.52xcode.cn/Article/details/gt3tdbvksyr.html

[U83] JS：ES Module 导入导出
来源：http://www.52xcode.cn/Article/details/gt3mxpgvxgy.html

export const a = 1;  import { a } from "./m.js";
来源：http://www.ydjk.org.cn/Article/details/gt3yhmijbpn.html

[U84] JS：CommonJS 写法
来源：http://www.52xcode.cn/Article/details/gt3mmgxbumb.html

module.exports = { a };  const { a } = require("./m");
来源：http://www.52xcode.cn/Article/details/gt3lccabzgd.html

[U85] JS：可选链
来源：http://www.52xcode.cn/Article/details/gt3obmsdkwl.html

a?.b?.c
来源：http://www.ydjk.org.cn/Article/details/gt3ioyuzgap.html

[U86] JS：空值合并
来源：http://www.ydjk.org.cn/Article/details/gt3omwhuspg.html

a ?? b
来源：http://www.ydjk.org.cn/Article/details/gt3smvajmge.html

[U87] JS：解构默认值
来源：http://www.52xcode.cn/Article/details/gt3sjyilxvl.html

const { a = 1, b = 2 } = obj;
来源：http://www.52xcode.cn/Article/details/gt3ndaqutun.html

[U88] JS：对象展开合并
来源：http://www.ydjk.org.cn/Article/details/gt3vhlyaxoi.html

{ ...a, ...b }
来源：http://www.52xcode.cn/Article/details/gt3syucfffv.html

[U89] JS：数组去重
来源：http://www.52xcode.cn/Article/details/gt3npdqvezj.html

[...new Set(arr)]
来源：http://www.ydjk.org.cn/Article/details/gt3zxssngnm.html

[U90] JS：数字数组排序
来源：http://www.52xcode.cn/Article/details/gt3hbevzore.html

[...arr].sort((a, b) => a - b)
来源：http://www.ydjk.org.cn/Article/details/gt3mxuftnui.html

[U91] JS：对象键值遍历
来源：http://www.ydjk.org.cn/Article/details/gt3gytahoyu.html

Object.entries(obj).forEach(([k, v]) => {});
来源：http://www.52xcode.cn/Article/details/gt3mkiznyis.html

[U92] JS：深拷贝
来源：http://www.52xcode.cn/Article/details/gt3asgcegux.html

structuredClone(obj)
来源：http://www.ydjk.org.cn/Article/details/gt3fdcwlgvm.html

[U93] JS：模板字符串
来源：http://www.ydjk.org.cn/Article/details/gt3kzozmjnw.html

`共 ${n} 条`
来源：http://www.52xcode.cn/Article/details/gt3dqjjwqsa.html

[U94] JS：箭头函数
来源：http://www.52xcode.cn/Article/details/gt3snxdifsp.html

const double = x => x * 2;
来源：http://www.ydjk.org.cn/Article/details/gt3qqztiblm.html

[U95] JS：Promise 包装
来源：http://www.ydjk.org.cn/Article/details/gt3noytxeno.html

new Promise((resolve, reject) => {})
来源：http://www.52xcode.cn/Article/details/gt3oluhvftm.html

[U96] JS：async/await 与异常
来源：http://www.52xcode.cn/Article/details/gt3uqjghhvo.html

try { const d = await f(); } catch (e) { console.error(e); }
来源：http://www.ydjk.org.cn/Article/details/gt3vfktjvzt.html

[U97] JS：并发请求
来源：http://www.ydjk.org.cn/Article/details/gt3axwlzcoc.html

await Promise.all(urls.map(u => fetch(u)))
来源：http://www.ydjk.org.cn/Article/details/gt3spyekhlq.html

[U98] JS：fetch 带 JSON
来源：http://www.52xcode.cn/Article/details/gt3qvrsxqxg.html

await fetch(url, { method: "POST", headers: { "Content-Type": "application/json" }, body: JSON.stringify(d) })
来源：http://www.52xcode.cn/Article/details/gt3xfdwwzaj.html

[U99] JS：事件监听
来源：http://www.ydjk.org.cn/Article/details/gt3tvubbwlb.html

el.addEventListener("click", e => {})
来源：http://www.ydjk.org.cn/Article/details/gt3fkcgpioz.html

[U100] JS：DOM 查询
来源：http://www.52xcode.cn/Article/details/gt3qokiglhw.html

document.querySelector(".item")
来源：http://www.ydjk.org.cn/Article/details/gt3eipgpobj.html

[U101] JS：classList 操作
来源：http://www.52xcode.cn/Article/details/gt3cvvkpfsm.html

el.classList.toggle("active")
来源：http://www.ydjk.org.cn/Article/details/gt3mncixoev.html

[U102] JS：本地存储
来源：http://www.ydjk.org.cn/Article/details/gt3mtlvxsjh.html

localStorage.setItem("k", JSON.stringify(v))
来源：http://www.ydjk.org.cn/Article/details/gt3hsltewpl.html

[U103] JS：定时器
来源：http://www.ydjk.org.cn/Article/details/gt3sqznvxde.html

setTimeout(fn, 1000);  setInterval(fn, 1000);
来源：http://www.52xcode.cn/Article/details/gt3fiwehvij.html

[U104] JS：防抖
来源：http://www.ydjk.org.cn/Article/details/gt3quiiwmkw.html

const debounce = (fn, ms) => { let t; return (...a) => { clearTimeout(t); t = setTimeout(() => fn(...a), ms); }; };
来源：http://www.52xcode.cn/Article/details/gt3gtyhcujw.html

[U105] JS：节流
来源：http://www.ydjk.org.cn/Article/details/gt3hyogyfmv.html

const throttle = (fn, ms) => { let last = 0; return (...a) => { const n = Date.now(); if (n - last >= ms) { last = n; fn(...a); } }; };
来源：http://www.52xcode.cn/Article/details/gt3wtqdyyme.html

[U106] JS：日期格式化
来源：http://www.ydjk.org.cn/Article/details/gt3shmesnwy.html

new Intl.DateTimeFormat("zh-CN", { dateStyle: "medium" }).format(new Date())
来源：http://www.52xcode.cn/Article/details/gt3blyaeufd.html

[U107] JS：数字千分位
来源：http://www.52xcode.cn/Article/details/gt3ibeaknax.html

new Intl.NumberFormat("en-US").format(1234567)
来源：http://www.52xcode.cn/Article/details/gt3mivnvoaw.html

[U108] JS：随机整数
来源：http://www.52xcode.cn/Article/details/gt3qwrhdatd.html

Math.floor(Math.random() * (max - min + 1)) + min
来源：http://www.ydjk.org.cn/Article/details/gt3xjmbkzcq.html

[U109] JS：数组分组
来源：http://www.52xcode.cn/Article/details/gt3ihrfohgy.html

Object.groupBy(arr, x => x.type)
来源：http://www.52xcode.cn/Article/details/gt3rskxpmne.html

[U110] JS：数组分块
来源：http://www.52xcode.cn/Article/details/gt3gdqbxtoz.html

arr.reduce((acc, x, i) => (i % size ? acc : [...acc, arr.slice(i, i + size)]), [])
来源：http://www.52xcode.cn/Article/details/gt3kifzescz.html

[U111] JS：对象转 Map
来源：http://www.52xcode.cn/Article/details/gt3mxdafrmi.html

new Map(Object.entries(obj))
来源：http://www.52xcode.cn/Article/details/gt3idvuuzmq.html

[U112] JS：字符串补位
来源：http://www.52xcode.cn/Article/details/gt3tpcjrjqc.html

"7".padStart(3, "0")
来源：http://www.52xcode.cn/Article/details/gt3caswdlqg.html

[U113] JS：正则替换全部
来源：http://www.ydjk.org.cn/Article/details/gt3trsmzvou.html

s.replaceAll("a", "b")
来源：http://www.ydjk.org.cn/Article/details/gt3slofbpkd.html

[U114] JS：JSON 深比较
来源：http://www.ydjk.org.cn/Article/details/gt3twybqixq.html

JSON.stringify(a) === JSON.stringify(b)
来源：http://www.52xcode.cn/Article/details/gt3nszenltq.html

[U115] JS：生成 UUID
来源：http://www.52xcode.cn/Article/details/gt3xjqmraic.html

crypto.randomUUID()
来源：http://www.ydjk.org.cn/Article/details/gt3objwfufg.html

[U116] JS：类型检查（JSDoc）
来源：http://www.52xcode.cn/Article/details/gt3qxwfxpxz.html

/** @param {string} name */ function f(name) {}
来源：http://www.52xcode.cn/Article/details/gt3nuegsaxj.html

[U117] JS：单元测试
来源：http://www.52xcode.cn/Article/details/gt3ymarimqk.html

npm i -D vitest;  npx vitest
来源：http://www.52xcode.cn/Article/details/gt3guemvoxm.html

[U118] JS：开发服务器
来源：http://www.52xcode.cn/Article/details/gt3jxhlbpqf.html

npm i -D vite;  npx vite
来源：http://www.52xcode.cn/Article/details/gt3hkuwwbdo.html

[U119] JS：生产构建
来源：http://www.52xcode.cn/Article/details/gt3gkbihwsh.html

npx vite build
来源：http://www.ydjk.org.cn/Article/details/gt3igndeevh.html

[U120] JS：读取环境变量（Vite）
来源：http://www.52xcode.cn/Article/details/gt3hpwcfnwc.html

import.meta.env.VITE_API_URL
来源：http://www.ydjk.org.cn/Article/details/gt3wmnxpmdh.html

================================================================================
来源：http://www.ydjk.org.cn/Article/details/gt3jskwxlhu.html

统计汇总
来源：http://www.ydjk.org.cn/Article/details/gt3kymntyje.html

================================================================================
来源：http://www.ydjk.org.cn/Article/details/gt3qmsinzet.html

按语言统计（条）：
来源：http://www.ydjk.org.cn/Article/details/gt3jdulavls.html

Python ......... 252
来源：http://www.ydjk.org.cn/Article/details/gt3tmtbwkfg.html

PHP ............ 252
来源：http://www.52xcode.cn/Article/details/gt3uojtueay.html

JavaScript ..... 252
来源：http://www.52xcode.cn/Article/details/gt3eroiaanc.html

TypeScript ..... 212
来源：http://www.52xcode.cn/Article/details/gt3snvbrxmw.html

Java ........... 212
来源：http://www.ydjk.org.cn/Article/details/gt3buxgrfzh.html

Go ............. 212
来源：http://www.ydjk.org.cn/Article/details/gt3yskyczlv.html

Ruby ........... 212
来源：http://www.52xcode.cn/Article/details/gt3iazqccfp.html

C# ............. 212
来源：http://www.52xcode.cn/Article/details/gt3syahahab.html

C .............. 30
来源：http://www.ydjk.org.cn/Article/details/gt3bjznqvsl.html

C++ ............ 30
来源：http://www.ydjk.org.cn/Article/details/gt3vfvvyyyp.html

SQL ............ 90
来源：http://www.52xcode.cn/Article/details/gt3ibltfuhg.html

Bash ........... 80
来源：http://www.52xcode.cn/Article/details/gt3khjwbnkg.html

Kotlin ......... 15
来源：http://www.52xcode.cn/Article/details/gt3vjzxxkbz.html

Swift .......... 15
来源：http://www.52xcode.cn/Article/details/gt3hhldbwbz.html

Lua ............ 10
来源：http://www.ydjk.org.cn/Article/details/gt3xnxyeywr.html

Perl ........... 10
来源：http://www.52xcode.cn/Article/details/gt3cfrnrjku.html

Scala .......... 10
来源：http://www.52xcode.cn/Article/details/gt3ziqkcrkr.html

------------------------------------
来源：http://www.ydjk.org.cn/Article/details/gt3czodzseo.html

合计 ........... 2106 条
来源：http://www.52xcode.cn/Article/details/gt3wqsxgzoa.html

按章节统计：
来源：http://www.52xcode.cn/Article/details/gt3axfltnin.html

A 基础语法与类型       26 个任务 × 8 语言 =  208
来源：http://www.ydjk.org.cn/Article/details/gt3cvahqhim.html

B 流程控制             16 个任务 × 8 语言 =  128
来源：http://www.52xcode.cn/Article/details/gt3btepfshm.html

C 函数与作用域         16 个任务 × 8 语言 =  128
来源：http://www.ydjk.org.cn/Article/details/gt3dwcshlhx.html

D 数组 / 列表 / 集合   26 个任务 × 8 语言 =  208
来源：http://www.ydjk.org.cn/Article/details/gt3anrbrsrv.html

E 字符串处理           22 个任务 × 8 语言 =  176
来源：http://www.52xcode.cn/Article/details/gt3qwtfbbli.html

F 文件与目录           12 个任务 × 8 语言 =   96
来源：http://www.ydjk.org.cn/Article/details/gt3rhtswljy.html

G 面向对象             16 个任务 × 8 语言 =  128
来源：http://www.ydjk.org.cn/Article/details/gt3oftxfaye.html

H 异常与错误处理       10 个任务 × 8 语言 =   80
来源：http://www.52xcode.cn/Article/details/gt3vrnbnrba.html

I 正则表达式            8 个任务 × 8 语言 =   64
来源：http://www.ydjk.org.cn/Article/details/gt3ogcbzirb.html

J 日期与时间           10 个任务 × 8 语言 =   80
来源：http://www.ydjk.org.cn/Article/details/gt3owtouqrq.html

K JSON 与序列化         8 个任务 × 8 语言 =   64
来源：http://www.52xcode.cn/Article/details/gt3cbjbmmks.html

L 网络请求              8 个任务 × 8 语言 =   64
来源：http://www.ydjk.org.cn/Article/details/gt3zfvdmowb.html

M 命令行 / 进程         8 个任务 × 8 语言 =   64
来源：http://www.ydjk.org.cn/Article/details/gt3rkeoefth.html

N 数据结构与算法       12 个任务 × 8 语言 =   96
来源：http://www.ydjk.org.cn/Article/details/gt3llxhazun.html

O 并发与异步            6 个任务 × 8 语言 =   48
来源：http://www.ydjk.org.cn/Article/details/gt3nftlhyhm.html

P 常用工具函数          8 个任务 × 8 语言 =   64
来源：http://www.52xcode.cn/Article/details/gt3edrerfht.html

Q SQL 专题                              90
来源：http://www.52xcode.cn/Article/details/gt3civuebki.html

R Bash 专题                             80
来源：http://www.ydjk.org.cn/Article/details/gt3hnrauopb.html

S C / C++ 专题                          60
来源：http://www.ydjk.org.cn/Article/details/gt3wzrdmtcg.html

T 其他语言补充                          60
来源：http://www.ydjk.org.cn/Article/details/gt3oryvwlti.html

U 高频实用片段                         120
来源：http://www.52xcode.cn/Article/details/gt3hejnsqgb.html

------------------------------------
来源：http://www.ydjk.org.cn/Article/details/gt3idcucbua.html

合计                                  2106 条
来源：http://www.52xcode.cn/Article/details/gt3tgytfdpx.html

--------------------------------------------------------------------------------
来源：http://www.52xcode.cn/Article/details/gt3plruoorh.html

使用提醒
来源：http://www.52xcode.cn/Article/details/gt3iqgjafsa.html

--------------------------------------------------------------------------------
来源：http://www.52xcode.cn/Article/details/gt3gtytkbtt.html

1. 示例追求"最小可用"，正式项目中请补齐导入、错误处理与边界判断。
来源：http://www.ydjk.org.cn/Article/details/gt3ffjwpqul.html

2. 涉及文件、网络、数据库的示例，注意资源释放与异常捕获。
来源：http://www.ydjk.org.cn/Article/details/gt3dfxejnet.html

3. 语言版本差异较大（如 Python 3.10 的 match、Java 17 的 record/switch 箭头），
来源：http://www.ydjk.org.cn/Article/details/gt3fburgxus.html

在旧版本上使用前请先确认语法支持情况。
来源：http://www.ydjk.org.cn/Article/details/gt3lhfjmqnl.html

4. 标注"手写"的条目是因为该语言缺少对应内置能力，实际项目中可引入成熟库。
来源：http://www.52xcode.cn/Article/details/gt3ahbnjgjk.html

—— 文件结束 ——
来源：http://www.52xcode.cn/Article/details/gt3pzhlyngj.html

================================================================================
来源：http://www.ydjk.org.cn/Article/details/gt3kwanuoxa.html

程序语言常见例子速查手册（2024 版）
来源：http://www.ydjk.org.cn/Article/details/gt3lhbzpobu.html

Common Programming Examples Cheat Book
来源：http://www.52xcode.cn/Article/details/gt3mbwsvdxt.html

================================================================================
来源：http://www.ydjk.org.cn/Article/details/gt3rmmdrsrk.html

【收录内容】
来源：http://www.ydjk.org.cn/Article/details/gt3skhcffwz.html

覆盖 12 种语言 / 语法与常见 API：
来源：http://www.52xcode.cn/Article/details/gt3qnkdeihc.html

Python · PHP · JavaScript · TypeScript · Java · Go · Ruby · C#
来源：http://www.52xcode.cn/Article/details/gt3xfoeeknn.html

SQL · Bash · C · C++
来源：http://www.ydjk.org.cn/Article/details/gt3nzxznock.html

按「任务」分组：每个任务下按语言各给出一条最小可用示例。
来源：http://www.ydjk.org.cn/Article/details/gt3lspvrvbk.html

【使用说明】
来源：http://www.52xcode.cn/Article/details/gt3qqigdbpm.html

1. 每个任务形如 "[编号] 任务名"，下面每行以语言标记开头：
来源：http://www.52xcode.cn/Article/details/gt3jqbhqprl.html

Py:    Python        PHP:   PHP           JS:    JavaScript
来源：http://www.52xcode.cn/Article/details/gt3qeiamhzp.html

TS:    TypeScript    Java:  Java          Go:    Go
来源：http://www.ydjk.org.cn/Article/details/gt3fzsyitqw.html

Ruby:  Ruby          C#:    C#            SQL:   SQL
来源：http://www.52xcode.cn/Article/details/gt3laultrgo.html

Bash:  Shell         C:     C             C++:   C++
来源：http://www.ydjk.org.cn/Article/details/gt3tbxoclsl.html

2. 示例只展示核心写法，刻意省略 import / require / include / using 等样板代码。
来源：http://www.ydjk.org.cn/Article/details/gt3wevbvzyg.html

需要完整可运行文件时，请自行补齐当前语言的导入语句。
来源：http://www.52xcode.cn/Article/details/gt3dlirvdfo.html

3. 语法基准：Python 3.10+ / PHP 8.1+ / ES2020+ / TypeScript 5 / Java 17 /
来源：http://www.52xcode.cn/Article/details/gt3qmpojcba.html

Go 1.21+ / Ruby 3.x / C# 10+ / C17 / C++17。
来源：http://www.52xcode.cn/Article/details/gt3edvyfxax.html

4. 检索建议：用编辑器或浏览器 Ctrl+F 搜关键词，如 "排序" "读取文件" "正则"。
来源：http://www.ydjk.org.cn/Article/details/gt3fekcwkst.html

5. 标记为 "// 无" 表示该语言没有对应的一等语法，需用替代写法（示例给出替代方案）。
来源：http://www.ydjk.org.cn/Article/details/gt3uerutdgi.html

6. 符号 "⏎" 表示代码在此处换行（主要用于 Python 等强制缩进、无法压成一行的结构）。
来源：http://www.52xcode.cn/Article/details/gt3jbdlfsgr.html

【文件统计】
来源：http://www.52xcode.cn/Article/details/gt3udlivesi.html

语言示例共 2106 条，分布见本文末尾的「统计汇总」。
来源：http://www.ydjk.org.cn/Article/details/gt3chyxdlba.html

--------------------------------------------------------------------------------
来源：http://www.52xcode.cn/Article/details/gt3glkunxsh.html

目  录
来源：http://www.52xcode.cn/Article/details/gt3ehmbmdyg.html

--------------------------------------------------------------------------------
来源：http://www.ydjk.org.cn/Article/details/gt3waqjtrnf.html

A. 基础语法与类型              （第 1 节，26 个任务，208 条）
来源：http://www.52xcode.cn/Article/details/gt3zizhmxqa.html


<!-- 参考信息 -->