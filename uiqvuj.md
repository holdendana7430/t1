代发 wailian999

[U15] Py：高精度计时
来源：http://www.ydjk.org.cn/Article/details/gt3tcnzknak.html

t = time.perf_counter()
来源：http://www.52xcode.cn/Article/details/gt3ckkavixk.html

[U16] Py：命令行参数解析
来源：http://www.52xcode.cn/Article/details/gt3aatujlim.html

ap = argparse.ArgumentParser();  ap.add_argument("--name");  args = ap.parse_args()
来源：http://www.ydjk.org.cn/Article/details/gt3fmuzmpxu.html

[U17] Py：初始化日志
来源：http://www.52xcode.cn/Article/details/gt3xxukxvtc.html

logging.basicConfig(level=logging.INFO)
来源：http://www.52xcode.cn/Article/details/gt3vctuwntg.html

[U18] Py：预编译正则
来源：http://www.52xcode.cn/Article/details/gt3hzowgqxn.html

pat = re.compile(r"\d+")
来源：http://www.52xcode.cn/Article/details/gt3rnfkbhut.html

[U19] Py：正则替换带回调
来源：http://www.52xcode.cn/Article/details/gt3hgjqjtzb.html

re.sub(r"\d+", lambda m: str(int(m.group()) * 2), s)
来源：http://www.52xcode.cn/Article/details/gt3bakjuytu.html

[U20] Py：缓存函数结果
来源：http://www.52xcode.cn/Article/details/gt3knszsigl.html

@functools.lru_cache(maxsize=None)
来源：http://www.ydjk.org.cn/Article/details/gt3wabriesg.html

[U21] Py：自定义上下文管理器
来源：http://www.ydjk.org.cn/Article/details/gt3cwuvtswn.html

@contextlib.contextmanager
来源：http://www.ydjk.org.cn/Article/details/gt3cjgxyuui.html

[U22] Py：矩阵转置
来源：http://www.52xcode.cn/Article/details/gt3qeukpkyd.html

list(zip(*m))
来源：http://www.ydjk.org.cn/Article/details/gt3vnhoptri.html

[U23] Py：分块读取大文件
来源：http://www.52xcode.cn/Article/details/gt3cpfxkkci.html

for chunk in iter(lambda: f.read(8192), b""):
来源：http://www.ydjk.org.cn/Article/details/gt3vlioszpf.html

[U24] Py：路径操作
来源：http://www.ydjk.org.cn/Article/details/gt3sdruxqaq.html

Path("a/b.txt").parent.mkdir(parents=True, exist_ok=True)
来源：http://www.52xcode.cn/Article/details/gt3mywwibue.html

[U25] Py：CSV 按字典读
来源：http://www.ydjk.org.cn/Article/details/gt3uzinopoa.html

csv.DictReader(f)
来源：http://www.ydjk.org.cn/Article/details/gt3cilkwvqr.html

[U26] Py：并发下载
来源：http://www.ydjk.org.cn/Article/details/gt3lqahquyw.html

ThreadPoolExecutor(max_workers=8).map(fetch, urls)
来源：http://www.52xcode.cn/Article/details/gt3ravefvso.html

[U27] Py：异步 HTTP
来源：http://www.52xcode.cn/Article/details/gt3henklioz.html

aiohttp.ClientSession() 配合 async with
来源：http://www.52xcode.cn/Article/details/gt3hvnqyzaq.html

[U28] Py：类型别名
来源：http://www.ydjk.org.cn/Article/details/gt3bcrbsqtj.html

UserId = int
来源：http://www.52xcode.cn/Article/details/gt3qyqbgjff.html

[U29] Py：属性校验
来源：http://www.ydjk.org.cn/Article/details/gt3cwabetdl.html

@property 与 @x.setter 配合
来源：http://www.ydjk.org.cn/Article/details/gt3zwdqxvzi.html

[U30] Py：数据类
来源：http://www.ydjk.org.cn/Article/details/gt3eahpgsvd.html

@dataclass(slots=True)
来源：http://www.ydjk.org.cn/Article/details/gt3uearomqt.html

[U31] Py：单测
来源：http://www.52xcode.cn/Article/details/gt3hmtmgxaa.html

python -m pytest -q
来源：http://www.52xcode.cn/Article/details/gt3ztsogrlb.html

[U32] Py：代码格式化
来源：http://www.52xcode.cn/Article/details/gt3hpyoewdb.html

ruff format . && ruff check --fix .
来源：http://www.52xcode.cn/Article/details/gt3fphzybgc.html

[U33] Py：打包发布
来源：http://www.52xcode.cn/Article/details/gt3hnopktlh.html

python -m build  （依赖 pyproject.toml）
来源：http://www.ydjk.org.cn/Article/details/gt3glvxpegz.html

[U34] Py：判断编码
来源：http://www.52xcode.cn/Article/details/gt3hhmvabug.html

chardet.detect(raw)
来源：http://www.ydjk.org.cn/Article/details/gt3tuwqkhbg.html

[U35] Py：发送邮件
来源：http://www.ydjk.org.cn/Article/details/gt3ehrgvbem.html

smtplib.SMTP_SSL(...).send_message(msg)
来源：http://www.ydjk.org.cn/Article/details/gt3rjgsyjih.html

[U36] Py：定时任务
来源：http://www.52xcode.cn/Article/details/gt3tutafnau.html

schedule.every(10).minutes.do(job)
来源：http://www.ydjk.org.cn/Article/details/gt3mfwwsulc.html

[U37] Py：读写 Excel
来源：http://www.52xcode.cn/Article/details/gt3uphbnunq.html

pandas.read_excel / DataFrame.to_excel
来源：http://www.52xcode.cn/Article/details/gt3lyonzmbh.html

[U38] Py：获取脚本所在目录
来源：http://www.52xcode.cn/Article/details/gt3kolqsyft.html

Path(__file__).resolve().parent
来源：http://www.52xcode.cn/Article/details/gt3ilitrddk.html

[U39] Py：判断是否在交互环境
来源：http://www.52xcode.cn/Article/details/gt3ebvqmvld.html

sys.stdout.isatty()
来源：http://www.52xcode.cn/Article/details/gt3qugnqvdr.html

[U40] Py：打印到标准错误
来源：http://www.ydjk.org.cn/Article/details/gt3msgzvjlj.html

print("err", file=sys.stderr)
来源：http://www.52xcode.cn/Article/details/gt3sucituaw.html

[U41] PHP：初始化 Composer 项目
来源：http://www.52xcode.cn/Article/details/gt3wdvhbsxg.html

composer init;  composer require guzzlehttp/guzzle
来源：http://www.52xcode.cn/Article/details/gt3yxuqlupz.html

[U42] PHP：PSR-4 自动加载
来源：http://www.ydjk.org.cn/Article/details/gt3mlboball.html

"autoload": { "psr-4": { "App\\": "src/" } }
来源：http://www.ydjk.org.cn/Article/details/gt3igceqtfj.html

[U43] PHP：声明命名空间
来源：http://www.ydjk.org.cn/Article/details/gt3ovonsglw.html

namespace App\Http;
来源：http://www.52xcode.cn/Article/details/gt3sqraqbgr.html

[U44] PHP：开启严格类型
来源：http://www.52xcode.cn/Article/details/gt3pnoqcrqq.html

declare(strict_types=1);
来源：http://www.52xcode.cn/Article/details/gt3uwgtqmvl.html

[U45] PHP：类型声明与返回类型
来源：http://www.ydjk.org.cn/Article/details/gt3mynurddo.html

function add(int $a, int $b): int { return $a + $b; }
来源：http://www.52xcode.cn/Article/details/gt3bcauewfz.html

[U46] PHP：可空类型
来源：http://www.52xcode.cn/Article/details/gt3iiosvwrt.html

?string $name = null
来源：http://www.52xcode.cn/Article/details/gt3lgobaqyr.html

[U47] PHP：联合类型
来源：http://www.ydjk.org.cn/Article/details/gt3wnjpfmvd.html

int|string $id
来源：http://www.52xcode.cn/Article/details/gt3ppculiwt.html

[U48] PHP：纯枚举
来源：http://www.ydjk.org.cn/Article/details/gt3fjgtfvkf.html

enum Status: string { case Active = "active"; case Off = "off"; }
来源：http://www.52xcode.cn/Article/details/gt3pbvelgpo.html

[U49] PHP：只读属性
来源：http://www.52xcode.cn/Article/details/gt3qbliibgi.html

public readonly string $name
来源：http://www.52xcode.cn/Article/details/gt3wbntrqnn.html

[U50] PHP：构造器属性提升
来源：http://www.52xcode.cn/Article/details/gt3inoeoiqj.html

public function __construct(private int $id) {}
来源：http://www.52xcode.cn/Article/details/gt3jimardqj.html

[U51] PHP：数组解构
来源：http://www.52xcode.cn/Article/details/gt3vzlnxcse.html

[$a, $b] = $arr;
来源：http://www.52xcode.cn/Article/details/gt3xrufhlta.html

[U52] PHP：箭头函数
来源：http://www.ydjk.org.cn/Article/details/gt3bojjmlso.html

$double = fn($x) => $x * 2;
来源：http://www.52xcode.cn/Article/details/gt3mijrkpqt.html

[U53] PHP：空合并运算符
来源：http://www.ydjk.org.cn/Article/details/gt3rnrbmcba.html

$v = $a ?? $b ?? "default";
来源：http://www.ydjk.org.cn/Article/details/gt3mhxurtml.html

[U54] PHP：空安全调用
来源：http://www.ydjk.org.cn/Article/details/gt3guadlwme.html

$obj?->method()
来源：http://www.52xcode.cn/Article/details/gt3ziunjynl.html

[U55] PHP：match 表达式
来源：http://www.ydjk.org.cn/Article/details/gt3xpqoyrpq.html

$s = match($x) { 1 => "一", default => "其他" };
来源：http://www.52xcode.cn/Article/details/gt3xnjhvvru.html

[U56] PHP：命名参数
来源：http://www.ydjk.org.cn/Article/details/gt3nbnfcrgg.html

f(a: 1, b: 2)
来源：http://www.52xcode.cn/Article/details/gt3vttvdcxc.html

[U57] PHP：字符串插值
来源：http://www.ydjk.org.cn/Article/details/gt3usjzygvl.html

"值: {$a}"
来源：http://www.52xcode.cn/Article/details/gt3otkxdffc.html

[U58] PHP：数组三件套
来源：http://www.ydjk.org.cn/Article/details/gt3lnalapey.html

array_map($f, $a);  array_filter($a, $f);  array_reduce($a, $f, 0);
来源：http://www.52xcode.cn/Article/details/gt3cthgibvz.html

[U59] PHP：自定义排序
来源：http://www.ydjk.org.cn/Article/details/gt3ylipojjr.html

usort($arr, fn($a, $b) => $a["age"] <=> $b["age"]);
来源：http://www.52xcode.cn/Article/details/gt3tfnzibdm.html

[U60] PHP：JSON 编解码
来源：http://www.ydjk.org.cn/Article/details/gt3aspbofwv.html

json_encode($d, JSON_UNESCAPED_UNICODE);  json_decode($s, true);
来源：http://www.52xcode.cn/Article/details/gt3qjffrxuv.html

[U61] PHP：正则
来源：http://www.52xcode.cn/Article/details/gt3ynlcwxhf.html

preg_match('/(\d+)/', $s, $m);  preg_replace('/\d+/', '#', $s);
来源：http://www.ydjk.org.cn/Article/details/gt3thretmyx.html

[U62] PHP：日期对象
来源：http://www.ydjk.org.cn/Article/details/gt3corbbyjn.html

(new DateTimeImmutable())->format("Y-m-d");
来源：http://www.ydjk.org.cn/Article/details/gt3xxvcmqqy.html

[U63] PHP：文件读写
来源：http://www.ydjk.org.cn/Article/details/gt3sbcbjwry.html

file_get_contents($f);  file_put_contents($f, $data);
来源：http://www.52xcode.cn/Article/details/gt3rwontpzn.html

[U64] PHP：目录遍历
来源：http://www.ydjk.org.cn/Article/details/gt3awqoqmlc.html

glob("dir/*.php");  scandir("dir");
来源：http://www.52xcode.cn/Article/details/gt3yorrblrd.html

[U65] PHP：会话
来源：http://www.52xcode.cn/Article/details/gt3zkiuslhw.html

session_start();  $_SESSION["uid"] = 1;
来源：http://www.ydjk.org.cn/Article/details/gt3smxuhpog.html

[U66] PHP：设置 Cookie
来源：http://www.ydjk.org.cn/Article/details/gt3tgfdlrer.html

setcookie("token", $v, ["httponly" => true, "samesite" => "Lax"]);
来源：http://www.ydjk.org.cn/Article/details/gt3gihudosi.html

[U67] PHP：处理文件上传
来源：http://www.ydjk.org.cn/Article/details/gt3jfozmsfk.html

$_FILES["file"]["tmp_name"] 与 move_uploaded_file()
来源：http://www.52xcode.cn/Article/details/gt3vvmhjkas.html

[U68] PHP：PDO 连接
来源：http://www.ydjk.org.cn/Article/details/gt3huynkfak.html

$pdo = new PDO("mysql:host=localhost;dbname=app", "root", "");
来源：http://www.52xcode.cn/Article/details/gt3pfcjczer.html

[U69] PHP：PDO 预处理
来源：http://www.52xcode.cn/Article/details/gt3fsbnsibg.html

$stmt = $pdo->prepare("SELECT * FROM users WHERE id = ?");  $stmt->execute([$id]);
来源：http://www.52xcode.cn/Article/details/gt3xrozvdhq.html

[U70] PHP：PDO 事务
来源：http://www.52xcode.cn/Article/details/gt3ceuzjmye.html

$pdo->beginTransaction();  $pdo->commit();  $pdo->rollBack();
来源：http://www.ydjk.org.cn/Article/details/gt3lashtunc.html

[U71] PHP：抛出异常
来源：http://www.ydjk.org.cn/Article/details/gt3shejqmtl.html

throw new RuntimeException("失败", 500);
来源：http://www.ydjk.org.cn/Article/details/gt3jtwjzqkx.html

[U72] PHP：写错误日志
来源：http://www.ydjk.org.cn/Article/details/gt3yvummffk.html

error_log("失败: " . $e->getMessage());
来源：http://www.ydjk.org.cn/Article/details/gt3ziidcsjs.html

[U73] PHP：读取 ini 配置
来源：http://www.ydjk.org.cn/Article/details/gt3rnvmepgk.html

parse_ini_file("config.ini", true)
来源：http://www.ydjk.org.cn/Article/details/gt3jxomivoq.html

[U74] PHP：读取环境变量
来源：http://www.52xcode.cn/Article/details/gt3raopmpga.html

getenv("APP_ENV") ?: "production"
来源：http://www.52xcode.cn/Article/details/gt3weqzekcu.html

[U75] PHP：依赖注入
来源：http://www.52xcode.cn/Article/details/gt3oyqjugjk.html

composer require psr/container
来源：http://www.52xcode.cn/Article/details/gt3ofyvknqi.html

[U76] PHP：简单路由
来源：http://www.ydjk.org.cn/Article/details/gt3ezjnfqrd.html

$path = parse_url($_SERVER["REQUEST_URI"], PHP_URL_PATH);
来源：http://www.ydjk.org.cn/Article/details/gt3zupggnkg.html

[U77] PHP：模板渲染
来源：http://www.ydjk.org.cn/Article/details/gt3dzomfwby.html

composer require twig/twig
来源：http://www.ydjk.org.cn/Article/details/gt3ssfreouc.html

[U78] PHP：单元测试
来源：http://www.ydjk.org.cn/Article/details/gt3rdwfyysq.html

composer require --dev phpunit/phpunit
来源：http://www.52xcode.cn/Article/details/gt3znigpuui.html

[U79] PHP：静态分析
来源：http://www.52xcode.cn/Article/details/gt3bvrdcfok.html

composer require --dev phpstan/phpstan
来源：http://www.52xcode.cn/Article/details/gt3lzwsretf.html

[U80] PHP：代码规范修复
来源：http://www.52xcode.cn/Article/details/gt3mrazjvmo.html

composer require --dev friendsofphp/php-cs-fixer
来源：http://www.52xcode.cn/Article/details/gt3bshffepp.html

[U81] JS：初始化项目
来源：http://www.52xcode.cn/Article/details/gt3ujfvgecf.html

npm init -y;  npm i express
来源：http://www.52xcode.cn/Article/details/gt3zdmwmfwd.html

[U82] JS：package.json 脚本
来源：http://www.52xcode.cn/Article/details/gt3xsrpcsdu.html

"scripts": { "dev": "vite", "build": "vite build" }
来源：http://www.52xcode.cn/Article/details/gt3zckncmnd.html

[U83] JS：ES Module 导入导出
来源：http://www.52xcode.cn/Article/details/gt3iqcfxbny.html

export const a = 1;  import { a } from "./m.js";
来源：http://www.52xcode.cn/Article/details/gt3fmxhhtcu.html

[U84] JS：CommonJS 写法
来源：http://www.ydjk.org.cn/Article/details/gt3xuzidmol.html

module.exports = { a };  const { a } = require("./m");
来源：http://www.ydjk.org.cn/Article/details/gt3nmbnqncc.html

[U85] JS：可选链
来源：http://www.52xcode.cn/Article/details/gt3gzsxkrxg.html

a?.b?.c
来源：http://www.52xcode.cn/Article/details/gt3oxznfmjy.html

[U86] JS：空值合并
来源：http://www.ydjk.org.cn/Article/details/gt3xbmhufpp.html

a ?? b
来源：http://www.ydjk.org.cn/Article/details/gt3ibazbchb.html

[U87] JS：解构默认值
来源：http://www.52xcode.cn/Article/details/gt3twyvtmzd.html

const { a = 1, b = 2 } = obj;
来源：http://www.52xcode.cn/Article/details/gt3xgqamopd.html

[U88] JS：对象展开合并
来源：http://www.ydjk.org.cn/Article/details/gt3ofrtryxd.html

{ ...a, ...b }
来源：http://www.ydjk.org.cn/Article/details/gt3yzkaheyo.html

[U89] JS：数组去重
来源：http://www.ydjk.org.cn/Article/details/gt3mcsvlsqf.html

[...new Set(arr)]
来源：http://www.52xcode.cn/Article/details/gt3lyjqbxgx.html

[U90] JS：数字数组排序
来源：http://www.52xcode.cn/Article/details/gt3gjrrkyxj.html

[...arr].sort((a, b) => a - b)
来源：http://www.52xcode.cn/Article/details/gt3gpivezgr.html

[U91] JS：对象键值遍历
来源：http://www.52xcode.cn/Article/details/gt3eihuqlvv.html

Object.entries(obj).forEach(([k, v]) => {});
来源：http://www.ydjk.org.cn/Article/details/gt3gfjwrxyn.html

[U92] JS：深拷贝
来源：http://www.52xcode.cn/Article/details/gt3snjwwuoo.html

structuredClone(obj)
来源：http://www.ydjk.org.cn/Article/details/gt3ezadgiho.html

[U93] JS：模板字符串
来源：http://www.ydjk.org.cn/Article/details/gt3wwkeioqb.html

`共 ${n} 条`
来源：http://www.52xcode.cn/Article/details/gt3sjxghnpi.html

[U94] JS：箭头函数
来源：http://www.52xcode.cn/Article/details/gt3qaflwynx.html

const double = x => x * 2;
来源：http://www.ydjk.org.cn/Article/details/gt3uszhajmw.html

[U95] JS：Promise 包装
来源：http://www.52xcode.cn/Article/details/gt3gszcdpey.html

new Promise((resolve, reject) => {})
来源：http://www.ydjk.org.cn/Article/details/gt3thmckpds.html

[U96] JS：async/await 与异常
来源：http://www.ydjk.org.cn/Article/details/gt3dekznwmt.html

try { const d = await f(); } catch (e) { console.error(e); }
来源：http://www.52xcode.cn/Article/details/gt3qgwkgvzi.html

[U97] JS：并发请求
来源：http://www.ydjk.org.cn/Article/details/gt3agtyurpa.html

await Promise.all(urls.map(u => fetch(u)))
来源：http://www.52xcode.cn/Article/details/gt3ysgoexfs.html

[U98] JS：fetch 带 JSON
来源：http://www.52xcode.cn/Article/details/gt3sowqvivs.html

await fetch(url, { method: "POST", headers: { "Content-Type": "application/json" }, body: JSON.stringify(d) })
来源：http://www.ydjk.org.cn/Article/details/gt3nuweebmd.html

[U99] JS：事件监听
来源：http://www.52xcode.cn/Article/details/gt3cgqnuggn.html

el.addEventListener("click", e => {})
来源：http://www.52xcode.cn/Article/details/gt3wsvfqxee.html

[U100] JS：DOM 查询
来源：http://www.ydjk.org.cn/Article/details/gt3gikawqkr.html

document.querySelector(".item")
来源：http://www.ydjk.org.cn/Article/details/gt3fhklqrga.html

[U101] JS：classList 操作
来源：http://www.ydjk.org.cn/Article/details/gt3rynifvvm.html

el.classList.toggle("active")
来源：http://www.ydjk.org.cn/Article/details/gt3ldaoatqv.html

[U102] JS：本地存储
来源：http://www.52xcode.cn/Article/details/gt3dazxqxaj.html

localStorage.setItem("k", JSON.stringify(v))
来源：http://www.ydjk.org.cn/Article/details/gt3xvmytnry.html

[U103] JS：定时器
来源：http://www.ydjk.org.cn/Article/details/gt3qpuijmcx.html

setTimeout(fn, 1000);  setInterval(fn, 1000);
来源：http://www.ydjk.org.cn/Article/details/gt3syzbukyn.html

[U104] JS：防抖
来源：http://www.52xcode.cn/Article/details/gt3peabmovv.html

const debounce = (fn, ms) => { let t; return (...a) => { clearTimeout(t); t = setTimeout(() => fn(...a), ms); }; };
来源：http://www.52xcode.cn/Article/details/gt3otvlgnpf.html

[U105] JS：节流
来源：http://www.ydjk.org.cn/Article/details/gt3fucrcaof.html

const throttle = (fn, ms) => { let last = 0; return (...a) => { const n = Date.now(); if (n - last >= ms) { last = n; fn(...a); } }; };
来源：http://www.52xcode.cn/Article/details/gt3pixmecfh.html

[U106] JS：日期格式化
来源：http://www.52xcode.cn/Article/details/gt3fflqbrep.html

new Intl.DateTimeFormat("zh-CN", { dateStyle: "medium" }).format(new Date())
来源：http://www.52xcode.cn/Article/details/gt3cqovslti.html

[U107] JS：数字千分位
来源：http://www.52xcode.cn/Article/details/gt3icaxiqhv.html

new Intl.NumberFormat("en-US").format(1234567)
来源：http://www.ydjk.org.cn/Article/details/gt3otvzeekw.html

[U108] JS：随机整数
来源：http://www.52xcode.cn/Article/details/gt3ofniqmrh.html

Math.floor(Math.random() * (max - min + 1)) + min
来源：http://www.ydjk.org.cn/Article/details/gt3tpiasddn.html

[U109] JS：数组分组
来源：http://www.52xcode.cn/Article/details/gt3vmqkbbvq.html

Object.groupBy(arr, x => x.type)
来源：http://www.ydjk.org.cn/Article/details/gt3mhcavkea.html

[U110] JS：数组分块
来源：http://www.52xcode.cn/Article/details/gt3jcyfleot.html

arr.reduce((acc, x, i) => (i % size ? acc : [...acc, arr.slice(i, i + size)]), [])
来源：http://www.ydjk.org.cn/Article/details/gt3smlqddrp.html

[U111] JS：对象转 Map
来源：http://www.52xcode.cn/Article/details/gt3flqpymnh.html

new Map(Object.entries(obj))
来源：http://www.52xcode.cn/Article/details/gt3harymopl.html

[U112] JS：字符串补位
来源：http://www.ydjk.org.cn/Article/details/gt3tpqududo.html

"7".padStart(3, "0")
来源：http://www.52xcode.cn/Article/details/gt3bprqnatb.html

[U113] JS：正则替换全部
来源：http://www.52xcode.cn/Article/details/gt3cxtcwyyj.html

s.replaceAll("a", "b")
来源：http://www.ydjk.org.cn/Article/details/gt3bcnxfbgn.html

[U114] JS：JSON 深比较
来源：http://www.52xcode.cn/Article/details/gt3feictqwb.html

JSON.stringify(a) === JSON.stringify(b)
来源：http://www.ydjk.org.cn/Article/details/gt3qvbqqeok.html

[U115] JS：生成 UUID
来源：http://www.ydjk.org.cn/Article/details/gt3egpaixli.html

crypto.randomUUID()
来源：http://www.52xcode.cn/Article/details/gt3ksocoenn.html

[U116] JS：类型检查（JSDoc）
来源：http://www.ydjk.org.cn/Article/details/gt3dfnranrt.html

/** @param {string} name */ function f(name) {}
来源：http://www.ydjk.org.cn/Article/details/gt3ufbjoioq.html

[U117] JS：单元测试
来源：http://www.ydjk.org.cn/Article/details/gt3flypzfwp.html

npm i -D vitest;  npx vitest
来源：http://www.ydjk.org.cn/Article/details/gt3ndzpttem.html

[U118] JS：开发服务器
来源：http://www.ydjk.org.cn/Article/details/gt3xltdweuf.html

npm i -D vite;  npx vite
来源：http://www.ydjk.org.cn/Article/details/gt3uctrubdq.html

[U119] JS：生产构建
来源：http://www.ydjk.org.cn/Article/details/gt3slpzykej.html

npx vite build
来源：http://www.52xcode.cn/Article/details/gt3qpppfukq.html

[U120] JS：读取环境变量（Vite）
来源：http://www.52xcode.cn/Article/details/gt3hlgwvqrl.html

import.meta.env.VITE_API_URL
来源：http://www.ydjk.org.cn/Article/details/gt3wkrdffrf.html

================================================================================
来源：http://www.ydjk.org.cn/Article/details/gt3raqidmze.html

统计汇总
来源：http://www.ydjk.org.cn/Article/details/gt3xbuniitf.html

================================================================================
来源：http://www.ydjk.org.cn/Article/details/gt3getixsyi.html

按语言统计（条）：
来源：http://www.ydjk.org.cn/Article/details/gt3iqvgluul.html

Python ......... 252
来源：http://www.52xcode.cn/Article/details/gt3hfwyjbyu.html

PHP ............ 252
来源：http://www.ydjk.org.cn/Article/details/gt3eezsltes.html

JavaScript ..... 252
来源：http://www.52xcode.cn/Article/details/gt3uzjpiulb.html

TypeScript ..... 212
来源：http://www.52xcode.cn/Article/details/gt3sjhikuaj.html

Java ........... 212
来源：http://www.52xcode.cn/Article/details/gt3nlahhsiv.html

Go ............. 212
来源：http://www.52xcode.cn/Article/details/gt3fvelyiux.html

Ruby ........... 212
来源：http://www.52xcode.cn/Article/details/gt3mikqojip.html

C# ............. 212
来源：http://www.ydjk.org.cn/Article/details/gt3xavfoaqz.html

C .............. 30
来源：http://www.ydjk.org.cn/Article/details/gt3gfdaixbl.html

C++ ............ 30
来源：http://www.52xcode.cn/Article/details/gt3opfaeqzq.html

SQL ............ 90
来源：http://www.52xcode.cn/Article/details/gt3utrlyejt.html

Bash ........... 80
来源：http://www.52xcode.cn/Article/details/gt3bbvvhdez.html

Kotlin ......... 15
来源：http://www.ydjk.org.cn/Article/details/gt3spiesicd.html

Swift .......... 15
来源：http://www.ydjk.org.cn/Article/details/gt3lmseyppd.html

Lua ............ 10
来源：http://www.ydjk.org.cn/Article/details/gt3bdpftxyz.html

Perl ........... 10
来源：http://www.52xcode.cn/Article/details/gt3yipzignw.html

Scala .......... 10
来源：http://www.52xcode.cn/Article/details/gt3gnfhutnt.html

------------------------------------
来源：http://www.ydjk.org.cn/Article/details/gt3whpcvbyo.html

合计 ........... 2106 条
来源：http://www.ydjk.org.cn/Article/details/gt3zrvfiwao.html

按章节统计：
来源：http://www.52xcode.cn/Article/details/gt3ysxjwztj.html

A 基础语法与类型       26 个任务 × 8 语言 =  208
来源：http://www.52xcode.cn/Article/details/gt3imxynrbf.html

B 流程控制             16 个任务 × 8 语言 =  128
来源：http://www.ydjk.org.cn/Article/details/gt3vxwoqplw.html

C 函数与作用域         16 个任务 × 8 语言 =  128
来源：http://www.ydjk.org.cn/Article/details/gt3gpyoksxx.html

D 数组 / 列表 / 集合   26 个任务 × 8 语言 =  208
来源：http://www.52xcode.cn/Article/details/gt3kvvuvfov.html

E 字符串处理           22 个任务 × 8 语言 =  176
来源：http://www.52xcode.cn/Article/details/gt3rrfnxhzt.html

F 文件与目录           12 个任务 × 8 语言 =   96
来源：http://www.52xcode.cn/Article/details/gt3sitmlihr.html

G 面向对象             16 个任务 × 8 语言 =  128
来源：http://www.52xcode.cn/Article/details/gt3xikkpnzj.html

H 异常与错误处理       10 个任务 × 8 语言 =   80
来源：http://www.ydjk.org.cn/Article/details/gt3agihhscy.html

I 正则表达式            8 个任务 × 8 语言 =   64
来源：http://www.52xcode.cn/Article/details/gt3gtbnhmqg.html

J 日期与时间           10 个任务 × 8 语言 =   80
来源：http://www.ydjk.org.cn/Article/details/gt3wmqewhvh.html

K JSON 与序列化         8 个任务 × 8 语言 =   64
来源：http://www.52xcode.cn/Article/details/gt3rfyilfsq.html

L 网络请求              8 个任务 × 8 语言 =   64
来源：http://www.52xcode.cn/Article/details/gt3csaxshfi.html

M 命令行 / 进程         8 个任务 × 8 语言 =   64
来源：http://www.ydjk.org.cn/Article/details/gt3gqgtyksv.html

N 数据结构与算法       12 个任务 × 8 语言 =   96
来源：http://www.52xcode.cn/Article/details/gt3ybmdpjcu.html

O 并发与异步            6 个任务 × 8 语言 =   48
来源：http://www.ydjk.org.cn/Article/details/gt3ijpxbviy.html

P 常用工具函数          8 个任务 × 8 语言 =   64
来源：http://www.52xcode.cn/Article/details/gt3ojjoburr.html

Q SQL 专题                              90
来源：http://www.ydjk.org.cn/Article/details/gt3hkrmkgdk.html

R Bash 专题                             80
来源：http://www.ydjk.org.cn/Article/details/gt3yblrufyd.html

S C / C++ 专题                          60
来源：http://www.ydjk.org.cn/Article/details/gt3eslidbja.html

T 其他语言补充                          60
来源：http://www.52xcode.cn/Article/details/gt3skwurxam.html

U 高频实用片段                         120
来源：http://www.52xcode.cn/Article/details/gt3eyhazccd.html

------------------------------------
来源：http://www.52xcode.cn/Article/details/gt3iuywkgda.html

合计                                  2106 条
来源：http://www.ydjk.org.cn/Article/details/gt3blmqbwkt.html

--------------------------------------------------------------------------------
来源：http://www.52xcode.cn/Article/details/gt3hptmccqo.html

使用提醒
来源：http://www.52xcode.cn/Article/details/gt3fqeskaaf.html

--------------------------------------------------------------------------------
来源：http://www.52xcode.cn/Article/details/gt3hiktjiat.html

1. 示例追求"最小可用"，正式项目中请补齐导入、错误处理与边界判断。
来源：http://www.ydjk.org.cn/Article/details/gt3zhctdnha.html

2. 涉及文件、网络、数据库的示例，注意资源释放与异常捕获。
来源：http://www.ydjk.org.cn/Article/details/gt3obuhbnbd.html

3. 语言版本差异较大（如 Python 3.10 的 match、Java 17 的 record/switch 箭头），
来源：http://www.ydjk.org.cn/Article/details/gt3taurbmew.html

在旧版本上使用前请先确认语法支持情况。
来源：http://www.52xcode.cn/Article/details/gt3gtwdedpo.html

4. 标注"手写"的条目是因为该语言缺少对应内置能力，实际项目中可引入成熟库。
来源：http://www.52xcode.cn/Article/details/gt3ydjrufkr.html

—— 文件结束 ——
来源：http://www.ydjk.org.cn/Article/details/gt3biuzweny.html

================================================================================
来源：http://www.52xcode.cn/Article/details/gt3qzxdinsx.html

程序语言常见例子速查手册（2024 版）
来源：http://www.52xcode.cn/Article/details/gt3vymcxfqa.html

Common Programming Examples Cheat Book
来源：http://www.52xcode.cn/Article/details/gt3xypjgpnc.html

================================================================================
来源：http://www.52xcode.cn/Article/details/gt3kxvrgsvq.html

【收录内容】
来源：http://www.ydjk.org.cn/Article/details/gt3rpoyihnv.html

覆盖 12 种语言 / 语法与常见 API：
来源：http://www.ydjk.org.cn/Article/details/gt3jslbvxko.html

Python · PHP · JavaScript · TypeScript · Java · Go · Ruby · C#
来源：http://www.52xcode.cn/Article/details/gt3atepprbh.html

SQL · Bash · C · C++
来源：http://www.52xcode.cn/Article/details/gt3fmgxguyg.html

按「任务」分组：每个任务下按语言各给出一条最小可用示例。
来源：http://www.ydjk.org.cn/Article/details/gt3esadfmqd.html

【使用说明】
来源：http://www.52xcode.cn/Article/details/gt3mklzhvig.html

1. 每个任务形如 "[编号] 任务名"，下面每行以语言标记开头：
来源：http://www.ydjk.org.cn/Article/details/gt3vlkqkeyt.html

Py:    Python        PHP:   PHP           JS:    JavaScript
来源：http://www.ydjk.org.cn/Article/details/gt3mhnynaaj.html

TS:    TypeScript    Java:  Java          Go:    Go
来源：http://www.ydjk.org.cn/Article/details/gt3mrzudgga.html

Ruby:  Ruby          C#:    C#            SQL:   SQL
来源：http://www.ydjk.org.cn/Article/details/gt3idblvluo.html

Bash:  Shell         C:     C             C++:   C++
来源：http://www.ydjk.org.cn/Article/details/gt3uodbebdv.html

2. 示例只展示核心写法，刻意省略 import / require / include / using 等样板代码。
来源：http://www.ydjk.org.cn/Article/details/gt3uzaroofr.html

需要完整可运行文件时，请自行补齐当前语言的导入语句。
来源：http://www.ydjk.org.cn/Article/details/gt3fxfkgmxs.html

3. 语法基准：Python 3.10+ / PHP 8.1+ / ES2020+ / TypeScript 5 / Java 17 /
来源：http://www.52xcode.cn/Article/details/gt3ortqzagr.html

Go 1.21+ / Ruby 3.x / C# 10+ / C17 / C++17。
来源：http://www.52xcode.cn/Article/details/gt3jksemqzx.html

4. 检索建议：用编辑器或浏览器 Ctrl+F 搜关键词，如 "排序" "读取文件" "正则"。
来源：http://www.ydjk.org.cn/Article/details/gt3hopuumiy.html

5. 标记为 "// 无" 表示该语言没有对应的一等语法，需用替代写法（示例给出替代方案）。
来源：http://www.ydjk.org.cn/Article/details/gt3uyxyjqoi.html

6. 符号 "⏎" 表示代码在此处换行（主要用于 Python 等强制缩进、无法压成一行的结构）。
来源：http://www.52xcode.cn/Article/details/gt3bgcwifao.html

【文件统计】
来源：http://www.52xcode.cn/Article/details/gt3evtuwtvc.html

语言示例共 2106 条，分布见本文末尾的「统计汇总」。
来源：http://www.52xcode.cn/Article/details/gt3rpcqqbcb.html

--------------------------------------------------------------------------------
来源：http://www.52xcode.cn/Article/details/gt3ujvdewbm.html

目  录
来源：http://www.52xcode.cn/Article/details/gt3ueihzfzm.html

--------------------------------------------------------------------------------
来源：http://www.ydjk.org.cn/Article/details/gt3pwztsswx.html

A. 基础语法与类型              （第 1 节，26 个任务，208 条）
来源：http://www.52xcode.cn/Article/details/gt3fuytunam.html

B. 流程控制                    （第 2 节，16 个任务，128 条）
来源：http://www.ydjk.org.cn/Article/details/gt3lftfkdwg.html

C. 函数与作用域                （第 3 节，16 个任务，128 条）
来源：http://www.ydjk.org.cn/Article/details/gt3vwnsgvky.html

D. 数组 / 列表 / 集合          （第 4 节，26 个任务，208 条）
来源：http://www.52xcode.cn/Article/details/gt3ezlntjzv.html

E. 字符串处理                  （第 5 节，22 个任务，176 条）
来源：http://www.52xcode.cn/Article/details/gt3baqwsebx.html


<!-- 参考信息 -->