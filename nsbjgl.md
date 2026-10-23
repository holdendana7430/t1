代发 wailian999

[U23] Py：分块读取大文件
来源：http://www.ydjk.org.cn/Article/details/gt3ydwoqazg.html

for chunk in iter(lambda: f.read(8192), b""):
来源：http://www.ydjk.org.cn/Article/details/gt3jtteovcg.html

[U24] Py：路径操作
来源：http://www.ydjk.org.cn/Article/details/gt3jjhqjgny.html

Path("a/b.txt").parent.mkdir(parents=True, exist_ok=True)
来源：http://www.52xcode.cn/Article/details/gt3dzkstjpd.html

[U25] Py：CSV 按字典读
来源：http://www.52xcode.cn/Article/details/gt3crtmuows.html

csv.DictReader(f)
来源：http://www.52xcode.cn/Article/details/gt3hyvqasdn.html

[U26] Py：并发下载
来源：http://www.52xcode.cn/Article/details/gt3nayhxivq.html

ThreadPoolExecutor(max_workers=8).map(fetch, urls)
来源：http://www.ydjk.org.cn/Article/details/gt3eifgxbhq.html

[U27] Py：异步 HTTP
来源：http://www.ydjk.org.cn/Article/details/gt3gyrwomiq.html

aiohttp.ClientSession() 配合 async with
来源：http://www.ydjk.org.cn/Article/details/gt3rllmuxvn.html

[U28] Py：类型别名
来源：http://www.52xcode.cn/Article/details/gt3pzyarehn.html

UserId = int
来源：http://www.ydjk.org.cn/Article/details/gt3uutqezxs.html

[U29] Py：属性校验
来源：http://www.ydjk.org.cn/Article/details/gt3wjqffset.html

@property 与 @x.setter 配合
来源：http://www.52xcode.cn/Article/details/gt3mksgkutl.html

[U30] Py：数据类
来源：http://www.ydjk.org.cn/Article/details/gt3vvlvfgjb.html

@dataclass(slots=True)
来源：http://www.52xcode.cn/Article/details/gt3msorokxw.html

[U31] Py：单测
来源：http://www.52xcode.cn/Article/details/gt3claeggut.html

python -m pytest -q
来源：http://www.ydjk.org.cn/Article/details/gt3gvxnsiqa.html

[U32] Py：代码格式化
来源：http://www.52xcode.cn/Article/details/gt3xbdijigs.html

ruff format . && ruff check --fix .
来源：http://www.ydjk.org.cn/Article/details/gt3iizdropa.html

[U33] Py：打包发布
来源：http://www.52xcode.cn/Article/details/gt3hlmseibq.html

python -m build  （依赖 pyproject.toml）
来源：http://www.ydjk.org.cn/Article/details/gt3eblnaqzz.html

[U34] Py：判断编码
来源：http://www.52xcode.cn/Article/details/gt3kvvujnop.html

chardet.detect(raw)
来源：http://www.ydjk.org.cn/Article/details/gt3jssznlmg.html

[U35] Py：发送邮件
来源：http://www.ydjk.org.cn/Article/details/gt3yrfivctc.html

smtplib.SMTP_SSL(...).send_message(msg)
来源：http://www.52xcode.cn/Article/details/gt3estqsnua.html

[U36] Py：定时任务
来源：http://www.52xcode.cn/Article/details/gt3jajoordi.html

schedule.every(10).minutes.do(job)
来源：http://www.ydjk.org.cn/Article/details/gt3rpukgqes.html

[U37] Py：读写 Excel
来源：http://www.ydjk.org.cn/Article/details/gt3rnpipwkx.html

pandas.read_excel / DataFrame.to_excel
来源：http://www.52xcode.cn/Article/details/gt3rkggtvbv.html

[U38] Py：获取脚本所在目录
来源：http://www.ydjk.org.cn/Article/details/gt3gecazfyv.html

Path(__file__).resolve().parent
来源：http://www.ydjk.org.cn/Article/details/gt3elrqyiox.html

[U39] Py：判断是否在交互环境
来源：http://www.52xcode.cn/Article/details/gt3dyaaqlms.html

sys.stdout.isatty()
来源：http://www.52xcode.cn/Article/details/gt3atorhydj.html

[U40] Py：打印到标准错误
来源：http://www.52xcode.cn/Article/details/gt3yjtnwnef.html

print("err", file=sys.stderr)
来源：http://www.52xcode.cn/Article/details/gt3ceoywkws.html

[U41] PHP：初始化 Composer 项目
来源：http://www.ydjk.org.cn/Article/details/gt3hrlfbfbu.html

composer init;  composer require guzzlehttp/guzzle
来源：http://www.ydjk.org.cn/Article/details/gt3boatbcru.html

[U42] PHP：PSR-4 自动加载
来源：http://www.ydjk.org.cn/Article/details/gt3fcjwnrni.html

"autoload": { "psr-4": { "App\\": "src/" } }
来源：http://www.ydjk.org.cn/Article/details/gt3zrsgorkc.html

[U43] PHP：声明命名空间
来源：http://www.ydjk.org.cn/Article/details/gt3vpfvpadd.html

namespace App\Http;
来源：http://www.ydjk.org.cn/Article/details/gt3crejyitp.html

[U44] PHP：开启严格类型
来源：http://www.ydjk.org.cn/Article/details/gt3lokjjgpg.html

declare(strict_types=1);
来源：http://www.ydjk.org.cn/Article/details/gt3enrfmjyw.html

[U45] PHP：类型声明与返回类型
来源：http://www.52xcode.cn/Article/details/gt3pycboqao.html

function add(int $a, int $b): int { return $a + $b; }
来源：http://www.52xcode.cn/Article/details/gt3umjukxqi.html

[U46] PHP：可空类型
来源：http://www.ydjk.org.cn/Article/details/gt3azhihnnn.html

?string $name = null
来源：http://www.52xcode.cn/Article/details/gt3gtgrfcml.html

[U47] PHP：联合类型
来源：http://www.52xcode.cn/Article/details/gt3ftgjeeaa.html

int|string $id
来源：http://www.52xcode.cn/Article/details/gt3qktmvsuz.html

[U48] PHP：纯枚举
来源：http://www.ydjk.org.cn/Article/details/gt3nubagorl.html

enum Status: string { case Active = "active"; case Off = "off"; }
来源：http://www.ydjk.org.cn/Article/details/gt3rnpwnwjo.html

[U49] PHP：只读属性
来源：http://www.52xcode.cn/Article/details/gt3vlfneyud.html

public readonly string $name
来源：http://www.52xcode.cn/Article/details/gt3wtawxhfz.html

[U50] PHP：构造器属性提升
来源：http://www.ydjk.org.cn/Article/details/gt3njjxlvzk.html

public function __construct(private int $id) {}
来源：http://www.52xcode.cn/Article/details/gt3rsxatjlj.html

[U51] PHP：数组解构
来源：http://www.ydjk.org.cn/Article/details/gt3irhlbuus.html

[$a, $b] = $arr;
来源：http://www.52xcode.cn/Article/details/gt3amxfomzc.html

[U52] PHP：箭头函数
来源：http://www.52xcode.cn/Article/details/gt3vpstyxck.html

$double = fn($x) => $x * 2;
来源：http://www.52xcode.cn/Article/details/gt3cocmsgah.html

[U53] PHP：空合并运算符
来源：http://www.ydjk.org.cn/Article/details/gt3flhmwbrh.html

$v = $a ?? $b ?? "default";
来源：http://www.ydjk.org.cn/Article/details/gt3ktwqyldb.html

[U54] PHP：空安全调用
来源：http://www.52xcode.cn/Article/details/gt3cdxpbqxk.html

$obj?->method()
来源：http://www.ydjk.org.cn/Article/details/gt3agrdqjhk.html

[U55] PHP：match 表达式
来源：http://www.ydjk.org.cn/Article/details/gt3gkpkalgx.html

$s = match($x) { 1 => "一", default => "其他" };
来源：http://www.ydjk.org.cn/Article/details/gt3qfpcgopr.html

[U56] PHP：命名参数
来源：http://www.ydjk.org.cn/Article/details/gt3hcecntyv.html

f(a: 1, b: 2)
来源：http://www.52xcode.cn/Article/details/gt3dboyyjya.html

[U57] PHP：字符串插值
来源：http://www.52xcode.cn/Article/details/gt3gdklcnfj.html

"值: {$a}"
来源：http://www.ydjk.org.cn/Article/details/gt3xawdfctt.html

[U58] PHP：数组三件套
来源：http://www.52xcode.cn/Article/details/gt3ykueppoa.html

array_map($f, $a);  array_filter($a, $f);  array_reduce($a, $f, 0);
来源：http://www.52xcode.cn/Article/details/gt3exivkgdo.html

[U59] PHP：自定义排序
来源：http://www.52xcode.cn/Article/details/gt3dzsnuhxx.html

usort($arr, fn($a, $b) => $a["age"] <=> $b["age"]);
来源：http://www.ydjk.org.cn/Article/details/gt3gehrmjmi.html

[U60] PHP：JSON 编解码
来源：http://www.ydjk.org.cn/Article/details/gt3xsalhptb.html

json_encode($d, JSON_UNESCAPED_UNICODE);  json_decode($s, true);
来源：http://www.ydjk.org.cn/Article/details/gt3ltemphcj.html

[U61] PHP：正则
来源：http://www.ydjk.org.cn/Article/details/gt3fkqoerfw.html

preg_match('/(\d+)/', $s, $m);  preg_replace('/\d+/', '#', $s);
来源：http://www.52xcode.cn/Article/details/gt3rfglrrve.html

[U62] PHP：日期对象
来源：http://www.ydjk.org.cn/Article/details/gt3ycyhvnjb.html

(new DateTimeImmutable())->format("Y-m-d");
来源：http://www.52xcode.cn/Article/details/gt3phdkqbqg.html

[U63] PHP：文件读写
来源：http://www.52xcode.cn/Article/details/gt3pusaxrkw.html

file_get_contents($f);  file_put_contents($f, $data);
来源：http://www.52xcode.cn/Article/details/gt3zgcafqfg.html

[U64] PHP：目录遍历
来源：http://www.ydjk.org.cn/Article/details/gt3umwanefu.html

glob("dir/*.php");  scandir("dir");
来源：http://www.ydjk.org.cn/Article/details/gt3kchojcck.html

[U65] PHP：会话
来源：http://www.ydjk.org.cn/Article/details/gt3qfwcatkq.html

session_start();  $_SESSION["uid"] = 1;
来源：http://www.ydjk.org.cn/Article/details/gt3qwcwvdct.html

[U66] PHP：设置 Cookie
来源：http://www.52xcode.cn/Article/details/gt3plfqbqou.html

setcookie("token", $v, ["httponly" => true, "samesite" => "Lax"]);
来源：http://www.ydjk.org.cn/Article/details/gt3xphaufbm.html

[U67] PHP：处理文件上传
来源：http://www.52xcode.cn/Article/details/gt3brrvqjdt.html

$_FILES["file"]["tmp_name"] 与 move_uploaded_file()
来源：http://www.ydjk.org.cn/Article/details/gt3veopcyju.html

[U68] PHP：PDO 连接
来源：http://www.52xcode.cn/Article/details/gt3mshdqqgb.html

$pdo = new PDO("mysql:host=localhost;dbname=app", "root", "");
来源：http://www.ydjk.org.cn/Article/details/gt3gavqbjfw.html

[U69] PHP：PDO 预处理
来源：http://www.ydjk.org.cn/Article/details/gt3kgepbtst.html

$stmt = $pdo->prepare("SELECT * FROM users WHERE id = ?");  $stmt->execute([$id]);
来源：http://www.ydjk.org.cn/Article/details/gt3adcjhnjn.html

[U70] PHP：PDO 事务
来源：http://www.ydjk.org.cn/Article/details/gt3ehlwbzsh.html

$pdo->beginTransaction();  $pdo->commit();  $pdo->rollBack();
来源：http://www.ydjk.org.cn/Article/details/gt3qfcvdgzy.html

[U71] PHP：抛出异常
来源：http://www.ydjk.org.cn/Article/details/gt3vyrwihui.html

throw new RuntimeException("失败", 500);
来源：http://www.52xcode.cn/Article/details/gt3xhuhactc.html

[U72] PHP：写错误日志
来源：http://www.52xcode.cn/Article/details/gt3wkazytnz.html

error_log("失败: " . $e->getMessage());
来源：http://www.ydjk.org.cn/Article/details/gt3tofoezxb.html

[U73] PHP：读取 ini 配置
来源：http://www.52xcode.cn/Article/details/gt3rbiqjdhf.html

parse_ini_file("config.ini", true)
来源：http://www.ydjk.org.cn/Article/details/gt3hztyyyqx.html

[U74] PHP：读取环境变量
来源：http://www.52xcode.cn/Article/details/gt3qabybbdq.html

getenv("APP_ENV") ?: "production"
来源：http://www.52xcode.cn/Article/details/gt3qhvqurue.html

[U75] PHP：依赖注入
来源：http://www.52xcode.cn/Article/details/gt3dfthtsbm.html

composer require psr/container
来源：http://www.ydjk.org.cn/Article/details/gt3tyubissy.html

[U76] PHP：简单路由
来源：http://www.52xcode.cn/Article/details/gt3gfjktkvg.html

$path = parse_url($_SERVER["REQUEST_URI"], PHP_URL_PATH);
来源：http://www.52xcode.cn/Article/details/gt3wsnrafjb.html

[U77] PHP：模板渲染
来源：http://www.52xcode.cn/Article/details/gt3vtklkmsm.html

composer require twig/twig
来源：http://www.52xcode.cn/Article/details/gt3xnpohkzv.html

[U78] PHP：单元测试
来源：http://www.52xcode.cn/Article/details/gt3utiqaagi.html

composer require --dev phpunit/phpunit
来源：http://www.52xcode.cn/Article/details/gt3pvwewcse.html

[U79] PHP：静态分析
来源：http://www.52xcode.cn/Article/details/gt3ntturila.html

composer require --dev phpstan/phpstan
来源：http://www.ydjk.org.cn/Article/details/gt3mipniwzl.html

[U80] PHP：代码规范修复
来源：http://www.52xcode.cn/Article/details/gt3maxdamzw.html

composer require --dev friendsofphp/php-cs-fixer
来源：http://www.ydjk.org.cn/Article/details/gt3svslyrxg.html

[U81] JS：初始化项目
来源：http://www.52xcode.cn/Article/details/gt3vafwpssy.html

npm init -y;  npm i express
来源：http://www.ydjk.org.cn/Article/details/gt3mqnstiwh.html

[U82] JS：package.json 脚本
来源：http://www.52xcode.cn/Article/details/gt3qizujybn.html

"scripts": { "dev": "vite", "build": "vite build" }
来源：http://www.52xcode.cn/Article/details/gt3qefmbkev.html

[U83] JS：ES Module 导入导出
来源：http://www.52xcode.cn/Article/details/gt3zhemoqrh.html

export const a = 1;  import { a } from "./m.js";
来源：http://www.ydjk.org.cn/Article/details/gt3vjpgmgow.html

[U84] JS：CommonJS 写法
来源：http://www.52xcode.cn/Article/details/gt3gnghzqhl.html

module.exports = { a };  const { a } = require("./m");
来源：http://www.ydjk.org.cn/Article/details/gt3banbdhrm.html

[U85] JS：可选链
来源：http://www.52xcode.cn/Article/details/gt3nelbrgom.html

a?.b?.c
来源：http://www.ydjk.org.cn/Article/details/gt3fznbsfwb.html

[U86] JS：空值合并
来源：http://www.52xcode.cn/Article/details/gt3ssaxstdn.html

a ?? b
来源：http://www.ydjk.org.cn/Article/details/gt3xyflvkrv.html

[U87] JS：解构默认值
来源：http://www.52xcode.cn/Article/details/gt3cqjlwzgj.html

const { a = 1, b = 2 } = obj;
来源：http://www.52xcode.cn/Article/details/gt3lstkhltz.html

[U88] JS：对象展开合并
来源：http://www.ydjk.org.cn/Article/details/gt3fpnhuayb.html

{ ...a, ...b }
来源：http://www.ydjk.org.cn/Article/details/gt3mwslspic.html

[U89] JS：数组去重
来源：http://www.52xcode.cn/Article/details/gt3qewlxges.html

[...new Set(arr)]
来源：http://www.52xcode.cn/Article/details/gt3xxpoooxq.html

[U90] JS：数字数组排序
来源：http://www.52xcode.cn/Article/details/gt3yjuoljmn.html

[...arr].sort((a, b) => a - b)
来源：http://www.ydjk.org.cn/Article/details/gt3nvnfrwsn.html

[U91] JS：对象键值遍历
来源：http://www.ydjk.org.cn/Article/details/gt3kcxejkzg.html

Object.entries(obj).forEach(([k, v]) => {});
来源：http://www.ydjk.org.cn/Article/details/gt3klopnudq.html

[U92] JS：深拷贝
来源：http://www.ydjk.org.cn/Article/details/gt3ubfihywo.html

structuredClone(obj)
来源：http://www.52xcode.cn/Article/details/gt3xvvchwys.html

[U93] JS：模板字符串
来源：http://www.ydjk.org.cn/Article/details/gt3vzvdoreb.html

`共 ${n} 条`
来源：http://www.ydjk.org.cn/Article/details/gt3eqpggxdb.html

[U94] JS：箭头函数
来源：http://www.ydjk.org.cn/Article/details/gt3vsgkbxrl.html

const double = x => x * 2;
来源：http://www.ydjk.org.cn/Article/details/gt3vgggsyec.html

[U95] JS：Promise 包装
来源：http://www.ydjk.org.cn/Article/details/gt3qexigmwa.html

new Promise((resolve, reject) => {})
来源：http://www.52xcode.cn/Article/details/gt3znixltzw.html

[U96] JS：async/await 与异常
来源：http://www.ydjk.org.cn/Article/details/gt3kbspjpmv.html

try { const d = await f(); } catch (e) { console.error(e); }
来源：http://www.ydjk.org.cn/Article/details/gt3ybykiugd.html

[U97] JS：并发请求
来源：http://www.52xcode.cn/Article/details/gt3atjewqct.html

await Promise.all(urls.map(u => fetch(u)))
来源：http://www.52xcode.cn/Article/details/gt3cipvhdlw.html

[U98] JS：fetch 带 JSON
来源：http://www.ydjk.org.cn/Article/details/gt3mrkipyex.html

await fetch(url, { method: "POST", headers: { "Content-Type": "application/json" }, body: JSON.stringify(d) })
来源：http://www.52xcode.cn/Article/details/gt3kizbfxth.html

[U99] JS：事件监听
来源：http://www.ydjk.org.cn/Article/details/gt3isjtbort.html

el.addEventListener("click", e => {})
来源：http://www.ydjk.org.cn/Article/details/gt3cxrspcft.html

[U100] JS：DOM 查询
来源：http://www.ydjk.org.cn/Article/details/gt3sacgbysd.html

document.querySelector(".item")
来源：http://www.ydjk.org.cn/Article/details/gt3hvebeffq.html

[U101] JS：classList 操作
来源：http://www.52xcode.cn/Article/details/gt3bhibquya.html

el.classList.toggle("active")
来源：http://www.52xcode.cn/Article/details/gt3kodycwuq.html

[U102] JS：本地存储
来源：http://www.ydjk.org.cn/Article/details/gt3zsvilofu.html

localStorage.setItem("k", JSON.stringify(v))
来源：http://www.ydjk.org.cn/Article/details/gt3zdaxcsxp.html

[U103] JS：定时器
来源：http://www.ydjk.org.cn/Article/details/gt3ladmmrwu.html

setTimeout(fn, 1000);  setInterval(fn, 1000);
来源：http://www.52xcode.cn/Article/details/gt3brkheamw.html

[U104] JS：防抖
来源：http://www.52xcode.cn/Article/details/gt3gwditoht.html

const debounce = (fn, ms) => { let t; return (...a) => { clearTimeout(t); t = setTimeout(() => fn(...a), ms); }; };
来源：http://www.ydjk.org.cn/Article/details/gt3mmavhckt.html

[U105] JS：节流
来源：http://www.ydjk.org.cn/Article/details/gt3ylpuptof.html

const throttle = (fn, ms) => { let last = 0; return (...a) => { const n = Date.now(); if (n - last >= ms) { last = n; fn(...a); } }; };
来源：http://www.52xcode.cn/Article/details/gt3ogxecvhz.html

[U106] JS：日期格式化
来源：http://www.ydjk.org.cn/Article/details/gt3gajdujde.html

new Intl.DateTimeFormat("zh-CN", { dateStyle: "medium" }).format(new Date())
来源：http://www.ydjk.org.cn/Article/details/gt3ycaetcny.html

[U107] JS：数字千分位
来源：http://www.ydjk.org.cn/Article/details/gt3gfouimnh.html

new Intl.NumberFormat("en-US").format(1234567)
来源：http://www.ydjk.org.cn/Article/details/gt3jzpodpsh.html

[U108] JS：随机整数
来源：http://www.ydjk.org.cn/Article/details/gt3wicfetfx.html

Math.floor(Math.random() * (max - min + 1)) + min
来源：http://www.ydjk.org.cn/Article/details/gt3znajwhjb.html

[U109] JS：数组分组
来源：http://www.ydjk.org.cn/Article/details/gt3eudsmutr.html

Object.groupBy(arr, x => x.type)
来源：http://www.52xcode.cn/Article/details/gt3aaidqpxs.html

[U110] JS：数组分块
来源：http://www.ydjk.org.cn/Article/details/gt3zmiksuhh.html

arr.reduce((acc, x, i) => (i % size ? acc : [...acc, arr.slice(i, i + size)]), [])
来源：http://www.52xcode.cn/Article/details/gt3wdvrgtir.html

[U111] JS：对象转 Map
来源：http://www.ydjk.org.cn/Article/details/gt3apehqwdb.html

new Map(Object.entries(obj))
来源：http://www.ydjk.org.cn/Article/details/gt3nprdgmnj.html

[U112] JS：字符串补位
来源：http://www.ydjk.org.cn/Article/details/gt3drqgagtw.html

"7".padStart(3, "0")
来源：http://www.52xcode.cn/Article/details/gt3pqawmoiu.html

[U113] JS：正则替换全部
来源：http://www.ydjk.org.cn/Article/details/gt3pmhljdev.html

s.replaceAll("a", "b")
来源：http://www.52xcode.cn/Article/details/gt3cdfwojse.html

[U114] JS：JSON 深比较
来源：http://www.52xcode.cn/Article/details/gt3kulgqgoq.html

JSON.stringify(a) === JSON.stringify(b)
来源：http://www.52xcode.cn/Article/details/gt3rltimisi.html

[U115] JS：生成 UUID
来源：http://www.ydjk.org.cn/Article/details/gt3wobwsjyf.html

crypto.randomUUID()
来源：http://www.52xcode.cn/Article/details/gt3fzaqznuc.html

[U116] JS：类型检查（JSDoc）
来源：http://www.52xcode.cn/Article/details/gt3hbmvirqy.html

/** @param {string} name */ function f(name) {}
来源：http://www.52xcode.cn/Article/details/gt3iobyxsoh.html

[U117] JS：单元测试
来源：http://www.ydjk.org.cn/Article/details/gt3rktpofck.html

npm i -D vitest;  npx vitest
来源：http://www.52xcode.cn/Article/details/gt3mnjeihhz.html

[U118] JS：开发服务器
来源：http://www.ydjk.org.cn/Article/details/gt3slrgydyh.html

npm i -D vite;  npx vite
来源：http://www.52xcode.cn/Article/details/gt3tzyjzkyq.html

[U119] JS：生产构建
来源：http://www.52xcode.cn/Article/details/gt3mzilxnne.html

npx vite build
来源：http://www.52xcode.cn/Article/details/gt3kczsanbo.html

[U120] JS：读取环境变量（Vite）
来源：http://www.ydjk.org.cn/Article/details/gt3hbkpsdru.html

import.meta.env.VITE_API_URL
来源：http://www.52xcode.cn/Article/details/gt3zydmnkbo.html

================================================================================
来源：http://www.52xcode.cn/Article/details/gt3rekpfyfe.html

统计汇总
来源：http://www.ydjk.org.cn/Article/details/gt3xcebhnbq.html

================================================================================
来源：http://www.52xcode.cn/Article/details/gt3zfqykpmp.html

按语言统计（条）：
来源：http://www.52xcode.cn/Article/details/gt3whsijazz.html

Python ......... 252
来源：http://www.ydjk.org.cn/Article/details/gt3mghnmepe.html

PHP ............ 252
来源：http://www.52xcode.cn/Article/details/gt3bzdqhqun.html

JavaScript ..... 252
来源：http://www.ydjk.org.cn/Article/details/gt3eesycbwd.html

TypeScript ..... 212
来源：http://www.52xcode.cn/Article/details/gt3aetiflog.html

Java ........... 212
来源：http://www.ydjk.org.cn/Article/details/gt3mdqfgfqu.html

Go ............. 212
来源：http://www.52xcode.cn/Article/details/gt3rlrijtqv.html

Ruby ........... 212
来源：http://www.ydjk.org.cn/Article/details/gt3jvgkjyja.html

C# ............. 212
来源：http://www.ydjk.org.cn/Article/details/gt3wgfbwtcs.html

C .............. 30
来源：http://www.ydjk.org.cn/Article/details/gt3zzithihx.html

C++ ............ 30
来源：http://www.52xcode.cn/Article/details/gt3ydaqdhxj.html

SQL ............ 90
来源：http://www.52xcode.cn/Article/details/gt3ntwaccio.html

Bash ........... 80
来源：http://www.ydjk.org.cn/Article/details/gt3lnqbbqbg.html

Kotlin ......... 15
来源：http://www.52xcode.cn/Article/details/gt3hklugusf.html

Swift .......... 15
来源：http://www.ydjk.org.cn/Article/details/gt3yrssfrxf.html

Lua ............ 10
来源：http://www.52xcode.cn/Article/details/gt3extyqnlc.html

Perl ........... 10
来源：http://www.52xcode.cn/Article/details/gt3yjzqfkec.html

Scala .......... 10
来源：http://www.52xcode.cn/Article/details/gt3hlfgerxx.html

------------------------------------
来源：http://www.ydjk.org.cn/Article/details/gt3gxcjwikl.html

合计 ........... 2106 条
来源：http://www.ydjk.org.cn/Article/details/gt3zqzygfqq.html

按章节统计：
来源：http://www.ydjk.org.cn/Article/details/gt3skodpaix.html

A 基础语法与类型       26 个任务 × 8 语言 =  208
来源：http://www.52xcode.cn/Article/details/gt3faadsjvr.html

B 流程控制             16 个任务 × 8 语言 =  128
来源：http://www.ydjk.org.cn/Article/details/gt3vjmswoef.html

C 函数与作用域         16 个任务 × 8 语言 =  128
来源：http://www.ydjk.org.cn/Article/details/gt3pxbwkcnn.html

D 数组 / 列表 / 集合   26 个任务 × 8 语言 =  208
来源：http://www.ydjk.org.cn/Article/details/gt3drgxxhvv.html

E 字符串处理           22 个任务 × 8 语言 =  176
来源：http://www.52xcode.cn/Article/details/gt3qqjumnup.html

F 文件与目录           12 个任务 × 8 语言 =   96
来源：http://www.52xcode.cn/Article/details/gt3nfzbegkw.html

G 面向对象             16 个任务 × 8 语言 =  128
来源：http://www.52xcode.cn/Article/details/gt3xxswlcvl.html

H 异常与错误处理       10 个任务 × 8 语言 =   80
来源：http://www.52xcode.cn/Article/details/gt3wqsruxqu.html

I 正则表达式            8 个任务 × 8 语言 =   64
来源：http://www.52xcode.cn/Article/details/gt3olzsoxro.html

J 日期与时间           10 个任务 × 8 语言 =   80
来源：http://www.ydjk.org.cn/Article/details/gt3nnkpoayw.html

K JSON 与序列化         8 个任务 × 8 语言 =   64
来源：http://www.ydjk.org.cn/Article/details/gt3kexpwnsb.html

L 网络请求              8 个任务 × 8 语言 =   64
来源：http://www.52xcode.cn/Article/details/gt3qxrroxne.html

M 命令行 / 进程         8 个任务 × 8 语言 =   64
来源：http://www.ydjk.org.cn/Article/details/gt3ovioafsc.html

N 数据结构与算法       12 个任务 × 8 语言 =   96
来源：http://www.52xcode.cn/Article/details/gt3deksjtie.html

O 并发与异步            6 个任务 × 8 语言 =   48
来源：http://www.ydjk.org.cn/Article/details/gt3afogssxh.html

P 常用工具函数          8 个任务 × 8 语言 =   64
来源：http://www.ydjk.org.cn/Article/details/gt3bqqhngso.html

Q SQL 专题                              90
来源：http://www.ydjk.org.cn/Article/details/gt3bnmqadoj.html

R Bash 专题                             80
来源：http://www.ydjk.org.cn/Article/details/gt3ebfaekqn.html

S C / C++ 专题                          60
来源：http://www.52xcode.cn/Article/details/gt3ommlyzwq.html

T 其他语言补充                          60
来源：http://www.52xcode.cn/Article/details/gt3oqhxcevp.html

U 高频实用片段                         120
来源：http://www.52xcode.cn/Article/details/gt3umsjtjgq.html

------------------------------------
来源：http://www.ydjk.org.cn/Article/details/gt3enorinjr.html

合计                                  2106 条
来源：http://www.52xcode.cn/Article/details/gt3rvnngbvq.html

--------------------------------------------------------------------------------
来源：http://www.52xcode.cn/Article/details/gt3unbzypuc.html

使用提醒
来源：http://www.ydjk.org.cn/Article/details/gt3isgfohju.html

--------------------------------------------------------------------------------
来源：http://www.52xcode.cn/Article/details/gt3jwkydnlb.html

1. 示例追求"最小可用"，正式项目中请补齐导入、错误处理与边界判断。
来源：http://www.ydjk.org.cn/Article/details/gt3snmkmivt.html

2. 涉及文件、网络、数据库的示例，注意资源释放与异常捕获。
来源：http://www.52xcode.cn/Article/details/gt3ubzrtayf.html

3. 语言版本差异较大（如 Python 3.10 的 match、Java 17 的 record/switch 箭头），
来源：http://www.52xcode.cn/Article/details/gt3mexvjdhy.html

在旧版本上使用前请先确认语法支持情况。
来源：http://www.ydjk.org.cn/Article/details/gt3jchtoily.html

4. 标注"手写"的条目是因为该语言缺少对应内置能力，实际项目中可引入成熟库。
来源：http://www.ydjk.org.cn/Article/details/gt3nlryrnrh.html

—— 文件结束 ——
来源：http://www.52xcode.cn/Article/details/gt3bmigmphb.html

================================================================================
来源：http://www.ydjk.org.cn/Article/details/gt3enpfqrca.html

程序语言常见例子速查手册（2024 版）
来源：http://www.ydjk.org.cn/Article/details/gt3czqigcux.html

Common Programming Examples Cheat Book
来源：http://www.52xcode.cn/Article/details/gt3bcjkxeub.html

================================================================================
来源：http://www.52xcode.cn/Article/details/gt3xvtzjdlm.html

【收录内容】
来源：http://www.52xcode.cn/Article/details/gt3hxgwydds.html

覆盖 12 种语言 / 语法与常见 API：
来源：http://www.52xcode.cn/Article/details/gt3sjviyzku.html

Python · PHP · JavaScript · TypeScript · Java · Go · Ruby · C#
来源：http://www.52xcode.cn/Article/details/gt3lmsgoack.html

SQL · Bash · C · C++
来源：http://www.ydjk.org.cn/Article/details/gt3woaijgpk.html

按「任务」分组：每个任务下按语言各给出一条最小可用示例。
来源：http://www.52xcode.cn/Article/details/gt3tusmnpso.html

【使用说明】
来源：http://www.ydjk.org.cn/Article/details/gt3cuedgpal.html

1. 每个任务形如 "[编号] 任务名"，下面每行以语言标记开头：
来源：http://www.ydjk.org.cn/Article/details/gt3tmmpiruu.html

Py:    Python        PHP:   PHP           JS:    JavaScript
来源：http://www.52xcode.cn/Article/details/gt3nmfnivrw.html

TS:    TypeScript    Java:  Java          Go:    Go
来源：http://www.52xcode.cn/Article/details/gt3yqaduadw.html

Ruby:  Ruby          C#:    C#            SQL:   SQL
来源：http://www.52xcode.cn/Article/details/gt3fuwhudqx.html

Bash:  Shell         C:     C             C++:   C++
来源：http://www.ydjk.org.cn/Article/details/gt3hgnjyakf.html

2. 示例只展示核心写法，刻意省略 import / require / include / using 等样板代码。
来源：http://www.52xcode.cn/Article/details/gt3pqcabshc.html

需要完整可运行文件时，请自行补齐当前语言的导入语句。
来源：http://www.ydjk.org.cn/Article/details/gt3ykqcwymw.html

3. 语法基准：Python 3.10+ / PHP 8.1+ / ES2020+ / TypeScript 5 / Java 17 /
来源：http://www.52xcode.cn/Article/details/gt3eiyosyvt.html

Go 1.21+ / Ruby 3.x / C# 10+ / C17 / C++17。
来源：http://www.52xcode.cn/Article/details/gt3aliegcyw.html

4. 检索建议：用编辑器或浏览器 Ctrl+F 搜关键词，如 "排序" "读取文件" "正则"。
来源：http://www.ydjk.org.cn/Article/details/gt3ytxoaewu.html

5. 标记为 "// 无" 表示该语言没有对应的一等语法，需用替代写法（示例给出替代方案）。
来源：http://www.ydjk.org.cn/Article/details/gt3ijferhwe.html

6. 符号 "⏎" 表示代码在此处换行（主要用于 Python 等强制缩进、无法压成一行的结构）。
来源：http://www.ydjk.org.cn/Article/details/gt3muumszhj.html

【文件统计】
来源：http://www.ydjk.org.cn/Article/details/gt3oeycwrxd.html

语言示例共 2106 条，分布见本文末尾的「统计汇总」。
来源：http://www.52xcode.cn/Article/details/gt3nahpaqba.html

--------------------------------------------------------------------------------
来源：http://www.52xcode.cn/Article/details/gt3sbbyqpno.html

目  录
来源：http://www.ydjk.org.cn/Article/details/gt3hhxffbgu.html

--------------------------------------------------------------------------------
来源：http://www.52xcode.cn/Article/details/gt3uqrfldjz.html

A. 基础语法与类型              （第 1 节，26 个任务，208 条）
来源：http://www.ydjk.org.cn/Article/details/gt3ltqfxqdp.html

B. 流程控制                    （第 2 节，16 个任务，128 条）
来源：http://www.52xcode.cn/Article/details/gt3cgbwlmho.html

C. 函数与作用域                （第 3 节，16 个任务，128 条）
来源：http://www.ydjk.org.cn/Article/details/gt3ogatbaup.html

D. 数组 / 列表 / 集合          （第 4 节，26 个任务，208 条）
来源：http://www.ydjk.org.cn/Article/details/gt3xvtzkybf.html

E. 字符串处理                  （第 5 节，22 个任务，176 条）
来源：http://www.ydjk.org.cn/Article/details/gt3mxpjutoi.html

F. 文件与目录                  （第 6 节，12 个任务，96 条）
来源：http://www.ydjk.org.cn/Article/details/gt3xemdhegi.html

G. 面向对象                    （第 7 节，16 个任务，128 条）
来源：http://www.ydjk.org.cn/Article/details/gt3aehztbab.html

H. 异常与错误处理              （第 8 节，10 个任务，80 条）
来源：http://www.52xcode.cn/Article/details/gt3kvbszfkg.html

I. 正则表达式                  （第 9 节，8 个任务，64 条）
来源：http://www.ydjk.org.cn/Article/details/gt3haybquet.html

J. 日期与时间                  （第 10 节，10 个任务，80 条）
来源：http://www.52xcode.cn/Article/details/gt3cazmblvm.html

K. JSON 与序列化               （第 11 节，8 个任务，64 条）
来源：http://www.52xcode.cn/Article/details/gt3cnyggtaa.html

L. 网络请求                    （第 12 节，8 个任务，64 条）
来源：http://www.ydjk.org.cn/Article/details/gt3rxiftdng.html

M. 命令行 / 进程 / 环境        （第 13 节，8 个任务，64 条）
来源：http://www.ydjk.org.cn/Article/details/gt3beyvbwls.html

N. 数据结构与算法              （第 14 节，12 个任务，96 条）
来源：http://www.ydjk.org.cn/Article/details/gt3zljsdewj.html

O. 并发与异步                  （第 15 节，6 个任务，48 条）
来源：http://www.ydjk.org.cn/Article/details/gt3qhrkljio.html

P. 常用工具函数                （第 16 节，8 个任务，64 条）
来源：http://www.52xcode.cn/Article/details/gt3hwbnfmhc.html

Q. SQL 专题                    （第 17 节，90 条）
来源：http://www.ydjk.org.cn/Article/details/gt3efyzoipn.html

R. Bash 专题                   （第 18 节，80 条）
来源：http://www.52xcode.cn/Article/details/gt3xmidcinj.html

S. C / C++ 专题                （第 19 节，60 条）
来源：http://www.ydjk.org.cn/Article/details/gt3qejucokw.html

T. 其他语言补充                （第 20 节，60 条：Kotlin / Swift / Lua / Perl / Scala）
来源：http://www.52xcode.cn/Article/details/gt3jirnwxtw.html

U. 高频实用片段                （第 21 节，120 条：Python / PHP / JavaScript 各 40 条）
来源：http://www.52xcode.cn/Article/details/gt3fcreemhx.html


<!-- 参考信息 -->