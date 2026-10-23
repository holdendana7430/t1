代发 wailian999

[U19] Py：正则替换带回调
来源：http://www.ydjk.org.cn/Article/details/gt3zveqummb.html

re.sub(r"\d+", lambda m: str(int(m.group()) * 2), s)
来源：http://www.52xcode.cn/Article/details/gt3hryozsjc.html

[U20] Py：缓存函数结果
来源：http://www.52xcode.cn/Article/details/gt3lezqpvns.html

@functools.lru_cache(maxsize=None)
来源：http://www.ydjk.org.cn/Article/details/gt3pdsmeabo.html

[U21] Py：自定义上下文管理器
来源：http://www.ydjk.org.cn/Article/details/gt3aymosljn.html

@contextlib.contextmanager
来源：http://www.ydjk.org.cn/Article/details/gt3uorrgezg.html

[U22] Py：矩阵转置
来源：http://www.ydjk.org.cn/Article/details/gt3dxvpiblh.html

list(zip(*m))
来源：http://www.ydjk.org.cn/Article/details/gt3hcwsjemq.html

[U23] Py：分块读取大文件
来源：http://www.ydjk.org.cn/Article/details/gt3zskuoigc.html

for chunk in iter(lambda: f.read(8192), b""):
来源：http://www.ydjk.org.cn/Article/details/gt3lkgddzfl.html

[U24] Py：路径操作
来源：http://www.52xcode.cn/Article/details/gt3ixroraym.html

Path("a/b.txt").parent.mkdir(parents=True, exist_ok=True)
来源：http://www.52xcode.cn/Article/details/gt3zrafdpic.html

[U25] Py：CSV 按字典读
来源：http://www.ydjk.org.cn/Article/details/gt3bqedsnfp.html

csv.DictReader(f)
来源：http://www.52xcode.cn/Article/details/gt3fujcqwwm.html

[U26] Py：并发下载
来源：http://www.52xcode.cn/Article/details/gt3eqhyoftr.html

ThreadPoolExecutor(max_workers=8).map(fetch, urls)
来源：http://www.52xcode.cn/Article/details/gt3rtwytchb.html

[U27] Py：异步 HTTP
来源：http://www.ydjk.org.cn/Article/details/gt3kqngcllz.html

aiohttp.ClientSession() 配合 async with
来源：http://www.52xcode.cn/Article/details/gt3kijshrtr.html

[U28] Py：类型别名
来源：http://www.ydjk.org.cn/Article/details/gt3xcrltihz.html

UserId = int
来源：http://www.52xcode.cn/Article/details/gt3kaoogmtj.html

[U29] Py：属性校验
来源：http://www.52xcode.cn/Article/details/gt3yioundpr.html

@property 与 @x.setter 配合
来源：http://www.ydjk.org.cn/Article/details/gt3pnblraeu.html

[U30] Py：数据类
来源：http://www.ydjk.org.cn/Article/details/gt3darzpmvg.html

@dataclass(slots=True)
来源：http://www.52xcode.cn/Article/details/gt3fplkthpc.html

[U31] Py：单测
来源：http://www.ydjk.org.cn/Article/details/gt3wgmuqndj.html

python -m pytest -q
来源：http://www.52xcode.cn/Article/details/gt3bzfmsyrg.html

[U32] Py：代码格式化
来源：http://www.ydjk.org.cn/Article/details/gt3hnhzywuw.html

ruff format . && ruff check --fix .
来源：http://www.ydjk.org.cn/Article/details/gt3npcnzdoy.html

[U33] Py：打包发布
来源：http://www.52xcode.cn/Article/details/gt3mjqljdsp.html

python -m build  （依赖 pyproject.toml）
来源：http://www.52xcode.cn/Article/details/gt3nrvexioz.html

[U34] Py：判断编码
来源：http://www.52xcode.cn/Article/details/gt3sikfwuml.html

chardet.detect(raw)
来源：http://www.52xcode.cn/Article/details/gt3uyluhbcp.html

[U35] Py：发送邮件
来源：http://www.ydjk.org.cn/Article/details/gt3biesmqsz.html

smtplib.SMTP_SSL(...).send_message(msg)
来源：http://www.ydjk.org.cn/Article/details/gt3xfitjuvk.html

[U36] Py：定时任务
来源：http://www.ydjk.org.cn/Article/details/gt3oikgrpjz.html

schedule.every(10).minutes.do(job)
来源：http://www.ydjk.org.cn/Article/details/gt3fevyaypw.html

[U37] Py：读写 Excel
来源：http://www.ydjk.org.cn/Article/details/gt3emcrpgtt.html

pandas.read_excel / DataFrame.to_excel
来源：http://www.ydjk.org.cn/Article/details/gt3ihwlpyff.html

[U38] Py：获取脚本所在目录
来源：http://www.52xcode.cn/Article/details/gt3limoybnb.html

Path(__file__).resolve().parent
来源：http://www.52xcode.cn/Article/details/gt3rfugzwja.html

[U39] Py：判断是否在交互环境
来源：http://www.ydjk.org.cn/Article/details/gt3ycifcjed.html

sys.stdout.isatty()
来源：http://www.52xcode.cn/Article/details/gt3bisebogy.html

[U40] Py：打印到标准错误
来源：http://www.52xcode.cn/Article/details/gt3xulzmiqi.html

print("err", file=sys.stderr)
来源：http://www.ydjk.org.cn/Article/details/gt3zunzyomt.html

[U41] PHP：初始化 Composer 项目
来源：http://www.ydjk.org.cn/Article/details/gt3roufnzfd.html

composer init;  composer require guzzlehttp/guzzle
来源：http://www.ydjk.org.cn/Article/details/gt3zkrnlmln.html

[U42] PHP：PSR-4 自动加载
来源：http://www.ydjk.org.cn/Article/details/gt3polmyvmi.html

"autoload": { "psr-4": { "App\\": "src/" } }
来源：http://www.52xcode.cn/Article/details/gt3ktueowyi.html

[U43] PHP：声明命名空间
来源：http://www.ydjk.org.cn/Article/details/gt3hsboybze.html

namespace App\Http;
来源：http://www.ydjk.org.cn/Article/details/gt3ehtbrakl.html

[U44] PHP：开启严格类型
来源：http://www.ydjk.org.cn/Article/details/gt3zriytysb.html

declare(strict_types=1);
来源：http://www.52xcode.cn/Article/details/gt3qhtqfetr.html

[U45] PHP：类型声明与返回类型
来源：http://www.52xcode.cn/Article/details/gt3gvgowslk.html

function add(int $a, int $b): int { return $a + $b; }
来源：http://www.ydjk.org.cn/Article/details/gt3dqbhkgeb.html

[U46] PHP：可空类型
来源：http://www.52xcode.cn/Article/details/gt3ttlcocjg.html

?string $name = null
来源：http://www.ydjk.org.cn/Article/details/gt3jjrsbvih.html

[U47] PHP：联合类型
来源：http://www.ydjk.org.cn/Article/details/gt3ljutxxco.html

int|string $id
来源：http://www.ydjk.org.cn/Article/details/gt3zmzozbfy.html

[U48] PHP：纯枚举
来源：http://www.ydjk.org.cn/Article/details/gt3ngmiteyq.html

enum Status: string { case Active = "active"; case Off = "off"; }
来源：http://www.ydjk.org.cn/Article/details/gt3jdixgmma.html

[U49] PHP：只读属性
来源：http://www.52xcode.cn/Article/details/gt3kmssgvzv.html

public readonly string $name
来源：http://www.ydjk.org.cn/Article/details/gt3waabiceq.html

[U50] PHP：构造器属性提升
来源：http://www.ydjk.org.cn/Article/details/gt3tvwhgeac.html

public function __construct(private int $id) {}
来源：http://www.ydjk.org.cn/Article/details/gt3ngcrqjci.html

[U51] PHP：数组解构
来源：http://www.ydjk.org.cn/Article/details/gt3gkqdbsbm.html

[$a, $b] = $arr;
来源：http://www.52xcode.cn/Article/details/gt3ounmibnt.html

[U52] PHP：箭头函数
来源：http://www.52xcode.cn/Article/details/gt3wbciluwd.html

$double = fn($x) => $x * 2;
来源：http://www.52xcode.cn/Article/details/gt3pjrpgawz.html

[U53] PHP：空合并运算符
来源：http://www.ydjk.org.cn/Article/details/gt3monryozm.html

$v = $a ?? $b ?? "default";
来源：http://www.ydjk.org.cn/Article/details/gt3nemnlfnb.html

[U54] PHP：空安全调用
来源：http://www.52xcode.cn/Article/details/gt3dwchnfvj.html

$obj?->method()
来源：http://www.52xcode.cn/Article/details/gt3axntwunn.html

[U55] PHP：match 表达式
来源：http://www.ydjk.org.cn/Article/details/gt3ftyxjshi.html

$s = match($x) { 1 => "一", default => "其他" };
来源：http://www.52xcode.cn/Article/details/gt3beaykmvw.html

[U56] PHP：命名参数
来源：http://www.52xcode.cn/Article/details/gt3oflinwlf.html

f(a: 1, b: 2)
来源：http://www.52xcode.cn/Article/details/gt3xsnihthh.html

[U57] PHP：字符串插值
来源：http://www.52xcode.cn/Article/details/gt3gayaxhkt.html

"值: {$a}"
来源：http://www.ydjk.org.cn/Article/details/gt3ftkdaiht.html

[U58] PHP：数组三件套
来源：http://www.52xcode.cn/Article/details/gt3dbksdllp.html

array_map($f, $a);  array_filter($a, $f);  array_reduce($a, $f, 0);
来源：http://www.52xcode.cn/Article/details/gt3retwcmmz.html

[U59] PHP：自定义排序
来源：http://www.ydjk.org.cn/Article/details/gt3bsxqxcwk.html

usort($arr, fn($a, $b) => $a["age"] <=> $b["age"]);
来源：http://www.ydjk.org.cn/Article/details/gt3jhhxijwp.html

[U60] PHP：JSON 编解码
来源：http://www.52xcode.cn/Article/details/gt3uwlvqyyf.html

json_encode($d, JSON_UNESCAPED_UNICODE);  json_decode($s, true);
来源：http://www.ydjk.org.cn/Article/details/gt3pzfykrkn.html

[U61] PHP：正则
来源：http://www.ydjk.org.cn/Article/details/gt3ylvuqyaa.html

preg_match('/(\d+)/', $s, $m);  preg_replace('/\d+/', '#', $s);
来源：http://www.52xcode.cn/Article/details/gt3golpignq.html

[U62] PHP：日期对象
来源：http://www.ydjk.org.cn/Article/details/gt3hgosaghx.html

(new DateTimeImmutable())->format("Y-m-d");
来源：http://www.ydjk.org.cn/Article/details/gt3easszqmq.html

[U63] PHP：文件读写
来源：http://www.52xcode.cn/Article/details/gt3axowmdob.html

file_get_contents($f);  file_put_contents($f, $data);
来源：http://www.ydjk.org.cn/Article/details/gt3gufqodul.html

[U64] PHP：目录遍历
来源：http://www.ydjk.org.cn/Article/details/gt3kghtfujb.html

glob("dir/*.php");  scandir("dir");
来源：http://www.52xcode.cn/Article/details/gt3fsevqnru.html

[U65] PHP：会话
来源：http://www.ydjk.org.cn/Article/details/gt3pygbllkq.html

session_start();  $_SESSION["uid"] = 1;
来源：http://www.ydjk.org.cn/Article/details/gt3qgsdlixl.html

[U66] PHP：设置 Cookie
来源：http://www.52xcode.cn/Article/details/gt3fwdpbeon.html

setcookie("token", $v, ["httponly" => true, "samesite" => "Lax"]);
来源：http://www.52xcode.cn/Article/details/gt3qrlgznhe.html

[U67] PHP：处理文件上传
来源：http://www.ydjk.org.cn/Article/details/gt3qwrwnppu.html

$_FILES["file"]["tmp_name"] 与 move_uploaded_file()
来源：http://www.ydjk.org.cn/Article/details/gt3feyqxoae.html

[U68] PHP：PDO 连接
来源：http://www.52xcode.cn/Article/details/gt3bdpyhymd.html

$pdo = new PDO("mysql:host=localhost;dbname=app", "root", "");
来源：http://www.ydjk.org.cn/Article/details/gt3gslzwili.html

[U69] PHP：PDO 预处理
来源：http://www.52xcode.cn/Article/details/gt3btwzjgjm.html

$stmt = $pdo->prepare("SELECT * FROM users WHERE id = ?");  $stmt->execute([$id]);
来源：http://www.ydjk.org.cn/Article/details/gt3jtejxlve.html

[U70] PHP：PDO 事务
来源：http://www.52xcode.cn/Article/details/gt3avurzcvk.html

$pdo->beginTransaction();  $pdo->commit();  $pdo->rollBack();
来源：http://www.52xcode.cn/Article/details/gt3nnjwvzmv.html

[U71] PHP：抛出异常
来源：http://www.52xcode.cn/Article/details/gt3mvbepbck.html

throw new RuntimeException("失败", 500);
来源：http://www.ydjk.org.cn/Article/details/gt3fguaxwxo.html

[U72] PHP：写错误日志
来源：http://www.ydjk.org.cn/Article/details/gt3ciwgyczn.html

error_log("失败: " . $e->getMessage());
来源：http://www.ydjk.org.cn/Article/details/gt3dlrigifx.html

[U73] PHP：读取 ini 配置
来源：http://www.ydjk.org.cn/Article/details/gt3hxowlofk.html

parse_ini_file("config.ini", true)
来源：http://www.52xcode.cn/Article/details/gt3vdvcrfsm.html

[U74] PHP：读取环境变量
来源：http://www.52xcode.cn/Article/details/gt3uuwteyxz.html

getenv("APP_ENV") ?: "production"
来源：http://www.52xcode.cn/Article/details/gt3mqsmvrne.html

[U75] PHP：依赖注入
来源：http://www.ydjk.org.cn/Article/details/gt3khhbhkqv.html

composer require psr/container
来源：http://www.52xcode.cn/Article/details/gt3tyrgalpx.html

[U76] PHP：简单路由
来源：http://www.ydjk.org.cn/Article/details/gt3vwdbgioi.html

$path = parse_url($_SERVER["REQUEST_URI"], PHP_URL_PATH);
来源：http://www.ydjk.org.cn/Article/details/gt3oivffkoa.html

[U77] PHP：模板渲染
来源：http://www.ydjk.org.cn/Article/details/gt3egfnuype.html

composer require twig/twig
来源：http://www.52xcode.cn/Article/details/gt3xqttqeaq.html

[U78] PHP：单元测试
来源：http://www.52xcode.cn/Article/details/gt3iaeqoomq.html

composer require --dev phpunit/phpunit
来源：http://www.52xcode.cn/Article/details/gt3axvkxdno.html

[U79] PHP：静态分析
来源：http://www.52xcode.cn/Article/details/gt3lctuimlk.html

composer require --dev phpstan/phpstan
来源：http://www.52xcode.cn/Article/details/gt3keqicfjl.html

[U80] PHP：代码规范修复
来源：http://www.ydjk.org.cn/Article/details/gt3wkyxltjp.html

composer require --dev friendsofphp/php-cs-fixer
来源：http://www.ydjk.org.cn/Article/details/gt3gogdwwkl.html

[U81] JS：初始化项目
来源：http://www.52xcode.cn/Article/details/gt3bcualgkf.html

npm init -y;  npm i express
来源：http://www.ydjk.org.cn/Article/details/gt3uafsrtme.html

[U82] JS：package.json 脚本
来源：http://www.ydjk.org.cn/Article/details/gt3swduuvtm.html

"scripts": { "dev": "vite", "build": "vite build" }
来源：http://www.52xcode.cn/Article/details/gt3rbltumzw.html

[U83] JS：ES Module 导入导出
来源：http://www.52xcode.cn/Article/details/gt3nreqnshi.html

export const a = 1;  import { a } from "./m.js";
来源：http://www.ydjk.org.cn/Article/details/gt3hedakcty.html

[U84] JS：CommonJS 写法
来源：http://www.52xcode.cn/Article/details/gt3cfannydv.html

module.exports = { a };  const { a } = require("./m");
来源：http://www.52xcode.cn/Article/details/gt3ttwhutry.html

[U85] JS：可选链
来源：http://www.52xcode.cn/Article/details/gt3sqmaudjb.html

a?.b?.c
来源：http://www.52xcode.cn/Article/details/gt3laqnaqer.html

[U86] JS：空值合并
来源：http://www.52xcode.cn/Article/details/gt3gomgiyvg.html

a ?? b
来源：http://www.ydjk.org.cn/Article/details/gt3tuzkovgj.html

[U87] JS：解构默认值
来源：http://www.ydjk.org.cn/Article/details/gt3ztvqiuuv.html

const { a = 1, b = 2 } = obj;
来源：http://www.ydjk.org.cn/Article/details/gt3spledicq.html

[U88] JS：对象展开合并
来源：http://www.52xcode.cn/Article/details/gt3xqppnypu.html

{ ...a, ...b }
来源：http://www.ydjk.org.cn/Article/details/gt3hpbmrehq.html

[U89] JS：数组去重
来源：http://www.52xcode.cn/Article/details/gt3psgverqm.html

[...new Set(arr)]
来源：http://www.52xcode.cn/Article/details/gt3ymbxculi.html

[U90] JS：数字数组排序
来源：http://www.52xcode.cn/Article/details/gt3jketowof.html

[...arr].sort((a, b) => a - b)
来源：http://www.52xcode.cn/Article/details/gt3obvjfdkg.html

[U91] JS：对象键值遍历
来源：http://www.52xcode.cn/Article/details/gt3eaqkclil.html

Object.entries(obj).forEach(([k, v]) => {});
来源：http://www.ydjk.org.cn/Article/details/gt3zvbmgxlj.html

[U92] JS：深拷贝
来源：http://www.ydjk.org.cn/Article/details/gt3seqmpiqo.html

structuredClone(obj)
来源：http://www.52xcode.cn/Article/details/gt3fnlsqeir.html

[U93] JS：模板字符串
来源：http://www.52xcode.cn/Article/details/gt3kuwdasob.html

`共 ${n} 条`
来源：http://www.ydjk.org.cn/Article/details/gt3ozccgfuz.html

[U94] JS：箭头函数
来源：http://www.ydjk.org.cn/Article/details/gt3pioeyskf.html

const double = x => x * 2;
来源：http://www.52xcode.cn/Article/details/gt3ybyjwkuc.html

[U95] JS：Promise 包装
来源：http://www.52xcode.cn/Article/details/gt3ficyjzze.html

new Promise((resolve, reject) => {})
来源：http://www.52xcode.cn/Article/details/gt3nrmwxymi.html

[U96] JS：async/await 与异常
来源：http://www.52xcode.cn/Article/details/gt3yhpwtcph.html

try { const d = await f(); } catch (e) { console.error(e); }
来源：http://www.ydjk.org.cn/Article/details/gt3ceamixqo.html

[U97] JS：并发请求
来源：http://www.52xcode.cn/Article/details/gt3ghncyxhg.html

await Promise.all(urls.map(u => fetch(u)))
来源：http://www.ydjk.org.cn/Article/details/gt3wkizjxvj.html

[U98] JS：fetch 带 JSON
来源：http://www.52xcode.cn/Article/details/gt3jkdhjbrs.html

await fetch(url, { method: "POST", headers: { "Content-Type": "application/json" }, body: JSON.stringify(d) })
来源：http://www.ydjk.org.cn/Article/details/gt3vqpgxkxr.html

[U99] JS：事件监听
来源：http://www.ydjk.org.cn/Article/details/gt3coimmlbu.html

el.addEventListener("click", e => {})
来源：http://www.ydjk.org.cn/Article/details/gt3zbbcqyve.html

[U100] JS：DOM 查询
来源：http://www.52xcode.cn/Article/details/gt3tgukupvq.html

document.querySelector(".item")
来源：http://www.52xcode.cn/Article/details/gt3frhhsjcc.html

[U101] JS：classList 操作
来源：http://www.52xcode.cn/Article/details/gt3jcbraskg.html

el.classList.toggle("active")
来源：http://www.ydjk.org.cn/Article/details/gt3hrkwkpcg.html

[U102] JS：本地存储
来源：http://www.52xcode.cn/Article/details/gt3ixgdkdtg.html

localStorage.setItem("k", JSON.stringify(v))
来源：http://www.ydjk.org.cn/Article/details/gt3nffuksix.html

[U103] JS：定时器
来源：http://www.ydjk.org.cn/Article/details/gt3yjnhhyqk.html

setTimeout(fn, 1000);  setInterval(fn, 1000);
来源：http://www.ydjk.org.cn/Article/details/gt3rbyhusbc.html

[U104] JS：防抖
来源：http://www.ydjk.org.cn/Article/details/gt3nbuzwvuo.html

const debounce = (fn, ms) => { let t; return (...a) => { clearTimeout(t); t = setTimeout(() => fn(...a), ms); }; };
来源：http://www.52xcode.cn/Article/details/gt3vumeqdjv.html

[U105] JS：节流
来源：http://www.ydjk.org.cn/Article/details/gt3wvuhhuto.html

const throttle = (fn, ms) => { let last = 0; return (...a) => { const n = Date.now(); if (n - last >= ms) { last = n; fn(...a); } }; };
来源：http://www.52xcode.cn/Article/details/gt3pebtwzvu.html

[U106] JS：日期格式化
来源：http://www.52xcode.cn/Article/details/gt3ibgezngo.html

new Intl.DateTimeFormat("zh-CN", { dateStyle: "medium" }).format(new Date())
来源：http://www.52xcode.cn/Article/details/gt3shjjoqln.html

[U107] JS：数字千分位
来源：http://www.ydjk.org.cn/Article/details/gt3davzckcr.html

new Intl.NumberFormat("en-US").format(1234567)
来源：http://www.ydjk.org.cn/Article/details/gt3ysuamvmd.html

[U108] JS：随机整数
来源：http://www.ydjk.org.cn/Article/details/gt3uduumiyb.html

Math.floor(Math.random() * (max - min + 1)) + min
来源：http://www.ydjk.org.cn/Article/details/gt3jacvbihe.html

[U109] JS：数组分组
来源：http://www.ydjk.org.cn/Article/details/gt3kjmpudyt.html

Object.groupBy(arr, x => x.type)
来源：http://www.ydjk.org.cn/Article/details/gt3obvnqxkw.html

[U110] JS：数组分块
来源：http://www.ydjk.org.cn/Article/details/gt3guhahidv.html

arr.reduce((acc, x, i) => (i % size ? acc : [...acc, arr.slice(i, i + size)]), [])
来源：http://www.ydjk.org.cn/Article/details/gt3ioimpeqx.html

[U111] JS：对象转 Map
来源：http://www.ydjk.org.cn/Article/details/gt3mazapqyt.html

new Map(Object.entries(obj))
来源：http://www.52xcode.cn/Article/details/gt3pumzyeqc.html

[U112] JS：字符串补位
来源：http://www.52xcode.cn/Article/details/gt3iskjeyad.html

"7".padStart(3, "0")
来源：http://www.ydjk.org.cn/Article/details/gt3atvdyymj.html

[U113] JS：正则替换全部
来源：http://www.52xcode.cn/Article/details/gt3zmemmbht.html

s.replaceAll("a", "b")
来源：http://www.52xcode.cn/Article/details/gt3swwxrukm.html

[U114] JS：JSON 深比较
来源：http://www.ydjk.org.cn/Article/details/gt3nknstqao.html

JSON.stringify(a) === JSON.stringify(b)
来源：http://www.52xcode.cn/Article/details/gt3rxtuuzoo.html

[U115] JS：生成 UUID
来源：http://www.52xcode.cn/Article/details/gt3pthvbndk.html

crypto.randomUUID()
来源：http://www.52xcode.cn/Article/details/gt3dulihywg.html

[U116] JS：类型检查（JSDoc）
来源：http://www.ydjk.org.cn/Article/details/gt3kjhluesb.html

/** @param {string} name */ function f(name) {}
来源：http://www.52xcode.cn/Article/details/gt3ayikxjwz.html

[U117] JS：单元测试
来源：http://www.ydjk.org.cn/Article/details/gt3elyorrlb.html

npm i -D vitest;  npx vitest
来源：http://www.ydjk.org.cn/Article/details/gt3vridqijm.html

[U118] JS：开发服务器
来源：http://www.52xcode.cn/Article/details/gt3xwknypoh.html

npm i -D vite;  npx vite
来源：http://www.ydjk.org.cn/Article/details/gt3chjxiujp.html

[U119] JS：生产构建
来源：http://www.52xcode.cn/Article/details/gt3hnzaqdlz.html

npx vite build
来源：http://www.ydjk.org.cn/Article/details/gt3vpenmmmc.html

[U120] JS：读取环境变量（Vite）
来源：http://www.52xcode.cn/Article/details/gt3urdspynw.html

import.meta.env.VITE_API_URL
来源：http://www.52xcode.cn/Article/details/gt3ezhprxvx.html

================================================================================
来源：http://www.ydjk.org.cn/Article/details/gt3dsssrorr.html

统计汇总
来源：http://www.52xcode.cn/Article/details/gt3wxasduta.html

================================================================================
来源：http://www.52xcode.cn/Article/details/gt3qkbbblql.html

按语言统计（条）：
来源：http://www.ydjk.org.cn/Article/details/gt3sehnwfwa.html

Python ......... 252
来源：http://www.ydjk.org.cn/Article/details/gt3nzftedyq.html

PHP ............ 252
来源：http://www.52xcode.cn/Article/details/gt3uvdiwgnh.html

JavaScript ..... 252
来源：http://www.ydjk.org.cn/Article/details/gt3drsjjtgp.html

TypeScript ..... 212
来源：http://www.ydjk.org.cn/Article/details/gt3xcdrpopa.html

Java ........... 212
来源：http://www.ydjk.org.cn/Article/details/gt3nimzmuta.html

Go ............. 212
来源：http://www.ydjk.org.cn/Article/details/gt3zywfkngk.html

Ruby ........... 212
来源：http://www.52xcode.cn/Article/details/gt3pysybxdl.html

C# ............. 212
来源：http://www.ydjk.org.cn/Article/details/gt3paurfbnf.html

C .............. 30
来源：http://www.ydjk.org.cn/Article/details/gt3kkdacswv.html

C++ ............ 30
来源：http://www.52xcode.cn/Article/details/gt3ggbwdkzj.html

SQL ............ 90
来源：http://www.52xcode.cn/Article/details/gt3wexabhrj.html

Bash ........... 80
来源：http://www.ydjk.org.cn/Article/details/gt3kaqpnpyd.html

Kotlin ......... 15
来源：http://www.ydjk.org.cn/Article/details/gt3hidsgjhv.html

Swift .......... 15
来源：http://www.52xcode.cn/Article/details/gt3ikpvmtlm.html

Lua ............ 10
来源：http://www.ydjk.org.cn/Article/details/gt3qndvxfgj.html

Perl ........... 10
来源：http://www.52xcode.cn/Article/details/gt3psxeoull.html

Scala .......... 10
来源：http://www.ydjk.org.cn/Article/details/gt3noclnnms.html

------------------------------------
来源：http://www.ydjk.org.cn/Article/details/gt3lklmmgun.html

合计 ........... 2106 条
来源：http://www.ydjk.org.cn/Article/details/gt3zdlrlugd.html

按章节统计：
来源：http://www.52xcode.cn/Article/details/gt3gfzdraoe.html

A 基础语法与类型       26 个任务 × 8 语言 =  208
来源：http://www.52xcode.cn/Article/details/gt3gzlixfcr.html

B 流程控制             16 个任务 × 8 语言 =  128
来源：http://www.52xcode.cn/Article/details/gt3ilrjzugg.html

C 函数与作用域         16 个任务 × 8 语言 =  128
来源：http://www.ydjk.org.cn/Article/details/gt3xtewdovt.html

D 数组 / 列表 / 集合   26 个任务 × 8 语言 =  208
来源：http://www.ydjk.org.cn/Article/details/gt3hatsbgys.html

E 字符串处理           22 个任务 × 8 语言 =  176
来源：http://www.ydjk.org.cn/Article/details/gt3fgopnnmt.html

F 文件与目录           12 个任务 × 8 语言 =   96
来源：http://www.ydjk.org.cn/Article/details/gt3twsdasgx.html

G 面向对象             16 个任务 × 8 语言 =  128
来源：http://www.52xcode.cn/Article/details/gt3ilbuiutb.html

H 异常与错误处理       10 个任务 × 8 语言 =   80
来源：http://www.52xcode.cn/Article/details/gt3vohqkepa.html

I 正则表达式            8 个任务 × 8 语言 =   64
来源：http://www.ydjk.org.cn/Article/details/gt3zhtdpepl.html

J 日期与时间           10 个任务 × 8 语言 =   80
来源：http://www.ydjk.org.cn/Article/details/gt3ngibhnti.html

K JSON 与序列化         8 个任务 × 8 语言 =   64
来源：http://www.ydjk.org.cn/Article/details/gt3aywggkzq.html

L 网络请求              8 个任务 × 8 语言 =   64
来源：http://www.ydjk.org.cn/Article/details/gt3xckohxes.html

M 命令行 / 进程         8 个任务 × 8 语言 =   64
来源：http://www.ydjk.org.cn/Article/details/gt3qbqxmaka.html

N 数据结构与算法       12 个任务 × 8 语言 =   96
来源：http://www.52xcode.cn/Article/details/gt3amkvfltu.html

O 并发与异步            6 个任务 × 8 语言 =   48
来源：http://www.ydjk.org.cn/Article/details/gt3ycawogjq.html

P 常用工具函数          8 个任务 × 8 语言 =   64
来源：http://www.52xcode.cn/Article/details/gt3vsxexked.html

Q SQL 专题                              90
来源：http://www.52xcode.cn/Article/details/gt3cstsvese.html

R Bash 专题                             80
来源：http://www.52xcode.cn/Article/details/gt3xxqqpxlq.html

S C / C++ 专题                          60
来源：http://www.52xcode.cn/Article/details/gt3criyftra.html

T 其他语言补充                          60
来源：http://www.52xcode.cn/Article/details/gt3snjhmdut.html

U 高频实用片段                         120
来源：http://www.52xcode.cn/Article/details/gt3ngltxquu.html

------------------------------------
来源：http://www.52xcode.cn/Article/details/gt3jtvjdkcf.html

合计                                  2106 条
来源：http://www.52xcode.cn/Article/details/gt3fwcadjrc.html

--------------------------------------------------------------------------------
来源：http://www.52xcode.cn/Article/details/gt3mqqojlkg.html

使用提醒
来源：http://www.ydjk.org.cn/Article/details/gt3vvgixigi.html

--------------------------------------------------------------------------------
来源：http://www.52xcode.cn/Article/details/gt3jobhwthu.html

1. 示例追求"最小可用"，正式项目中请补齐导入、错误处理与边界判断。
来源：http://www.ydjk.org.cn/Article/details/gt3iivxqwsw.html

2. 涉及文件、网络、数据库的示例，注意资源释放与异常捕获。
来源：http://www.ydjk.org.cn/Article/details/gt3tnygoxwg.html

3. 语言版本差异较大（如 Python 3.10 的 match、Java 17 的 record/switch 箭头），
来源：http://www.52xcode.cn/Article/details/gt3gwcuwifk.html

在旧版本上使用前请先确认语法支持情况。
来源：http://www.ydjk.org.cn/Article/details/gt3rnhrlbzl.html

4. 标注"手写"的条目是因为该语言缺少对应内置能力，实际项目中可引入成熟库。
来源：http://www.52xcode.cn/Article/details/gt3uueupjki.html

—— 文件结束 ——
来源：http://www.ydjk.org.cn/Article/details/gt3qkmjacpl.html

================================================================================
来源：http://www.52xcode.cn/Article/details/gt3dpscltvd.html

程序语言常见例子速查手册（2024 版）
来源：http://www.52xcode.cn/Article/details/gt3iltpyzlp.html

Common Programming Examples Cheat Book
来源：http://www.52xcode.cn/Article/details/gt3lhzedvmp.html

================================================================================
来源：http://www.52xcode.cn/Article/details/gt3xtvdewvc.html

【收录内容】
来源：http://www.52xcode.cn/Article/details/gt3rwflkxle.html

覆盖 12 种语言 / 语法与常见 API：
来源：http://www.52xcode.cn/Article/details/gt3jhchjzkx.html

Python · PHP · JavaScript · TypeScript · Java · Go · Ruby · C#
来源：http://www.52xcode.cn/Article/details/gt3otlmojev.html

SQL · Bash · C · C++
来源：http://www.52xcode.cn/Article/details/gt3bvkanemy.html

按「任务」分组：每个任务下按语言各给出一条最小可用示例。
来源：http://www.ydjk.org.cn/Article/details/gt3vactsxyn.html

【使用说明】
来源：http://www.52xcode.cn/Article/details/gt3zywuteum.html

1. 每个任务形如 "[编号] 任务名"，下面每行以语言标记开头：
来源：http://www.52xcode.cn/Article/details/gt3bkmgneeo.html

Py:    Python        PHP:   PHP           JS:    JavaScript
来源：http://www.ydjk.org.cn/Article/details/gt3buhibqzc.html

TS:    TypeScript    Java:  Java          Go:    Go
来源：http://www.ydjk.org.cn/Article/details/gt3xgrdlery.html

Ruby:  Ruby          C#:    C#            SQL:   SQL
来源：http://www.ydjk.org.cn/Article/details/gt3cesuydtj.html

Bash:  Shell         C:     C             C++:   C++
来源：http://www.ydjk.org.cn/Article/details/gt3bquhpbaq.html

2. 示例只展示核心写法，刻意省略 import / require / include / using 等样板代码。
来源：http://www.ydjk.org.cn/Article/details/gt3djjiaqjr.html

需要完整可运行文件时，请自行补齐当前语言的导入语句。
来源：http://www.ydjk.org.cn/Article/details/gt3nrvvbeeh.html

3. 语法基准：Python 3.10+ / PHP 8.1+ / ES2020+ / TypeScript 5 / Java 17 /
来源：http://www.52xcode.cn/Article/details/gt3rzkaskgb.html

Go 1.21+ / Ruby 3.x / C# 10+ / C17 / C++17。
来源：http://www.52xcode.cn/Article/details/gt3jbbqfxfc.html

4. 检索建议：用编辑器或浏览器 Ctrl+F 搜关键词，如 "排序" "读取文件" "正则"。
来源：http://www.52xcode.cn/Article/details/gt3pwcjgecd.html

5. 标记为 "// 无" 表示该语言没有对应的一等语法，需用替代写法（示例给出替代方案）。
来源：http://www.52xcode.cn/Article/details/gt3zqrgnpyo.html

6. 符号 "⏎" 表示代码在此处换行（主要用于 Python 等强制缩进、无法压成一行的结构）。
来源：http://www.52xcode.cn/Article/details/gt3hzeeuzhz.html

【文件统计】
来源：http://www.52xcode.cn/Article/details/gt3qqlpfzbp.html

语言示例共 2106 条，分布见本文末尾的「统计汇总」。
来源：http://www.52xcode.cn/Article/details/gt3slutuosx.html

--------------------------------------------------------------------------------
来源：http://www.52xcode.cn/Article/details/gt3rdhccdjg.html

目  录
来源：http://www.52xcode.cn/Article/details/gt3yuhgcstl.html

--------------------------------------------------------------------------------
来源：http://www.52xcode.cn/Article/details/gt3efuofclh.html

A. 基础语法与类型              （第 1 节，26 个任务，208 条）
来源：http://www.52xcode.cn/Article/details/gt3qfoeubtr.html

B. 流程控制                    （第 2 节，16 个任务，128 条）
来源：http://www.52xcode.cn/Article/details/gt3jeatcfxq.html

C. 函数与作用域                （第 3 节，16 个任务，128 条）
来源：http://www.52xcode.cn/Article/details/gt3yhdpjvpz.html

D. 数组 / 列表 / 集合          （第 4 节，26 个任务，208 条）
来源：http://www.ydjk.org.cn/Article/details/gt3nuirafcl.html

E. 字符串处理                  （第 5 节，22 个任务，176 条）
来源：http://www.52xcode.cn/Article/details/gt3nyxfdesg.html

F. 文件与目录                  （第 6 节，12 个任务，96 条）
来源：http://www.52xcode.cn/Article/details/gt3zcctloqz.html

G. 面向对象                    （第 7 节，16 个任务，128 条）
来源：http://www.52xcode.cn/Article/details/gt3dfleezen.html

H. 异常与错误处理              （第 8 节，10 个任务，80 条）
来源：http://www.52xcode.cn/Article/details/gt3bfddgmqx.html

I. 正则表达式                  （第 9 节，8 个任务，64 条）
来源：http://www.ydjk.org.cn/Article/details/gt3upgsqutj.html

J. 日期与时间                  （第 10 节，10 个任务，80 条）
来源：http://www.ydjk.org.cn/Article/details/gt3wnbjawht.html

K. JSON 与序列化               （第 11 节，8 个任务，64 条）
来源：http://www.52xcode.cn/Article/details/gt3dvoxuuai.html

L. 网络请求                    （第 12 节，8 个任务，64 条）
来源：http://www.ydjk.org.cn/Article/details/gt3rvhwijmb.html

M. 命令行 / 进程 / 环境        （第 13 节，8 个任务，64 条）
来源：http://www.52xcode.cn/Article/details/gt3rauyapfo.html


<!-- 参考信息 -->