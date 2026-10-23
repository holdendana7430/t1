代发 wailian999

[U13] Py：固定长度队列
来源：http://www.ydjk.org.cn/Article/details/gt3qtgstpiy.html

deque(maxlen=10)
来源：http://www.ydjk.org.cn/Article/details/gt3obczonio.html

[U14] Py：分组收集到列表
来源：http://www.52xcode.cn/Article/details/gt3ltiskgpa.html

defaultdict(list)
来源：http://www.52xcode.cn/Article/details/gt3hkjwrkjc.html

[U15] Py：高精度计时
来源：http://www.52xcode.cn/Article/details/gt3lwycftua.html

t = time.perf_counter()
来源：http://www.52xcode.cn/Article/details/gt3earmhmuk.html

[U16] Py：命令行参数解析
来源：http://www.ydjk.org.cn/Article/details/gt3ynzziazh.html

ap = argparse.ArgumentParser();  ap.add_argument("--name");  args = ap.parse_args()
来源：http://www.52xcode.cn/Article/details/gt3hkdgntbo.html

[U17] Py：初始化日志
来源：http://www.ydjk.org.cn/Article/details/gt3rffqprvs.html

logging.basicConfig(level=logging.INFO)
来源：http://www.52xcode.cn/Article/details/gt3gzzngkxz.html

[U18] Py：预编译正则
来源：http://www.ydjk.org.cn/Article/details/gt3skypigpq.html

pat = re.compile(r"\d+")
来源：http://www.ydjk.org.cn/Article/details/gt3fqwdifqg.html

[U19] Py：正则替换带回调
来源：http://www.ydjk.org.cn/Article/details/gt3phifverl.html

re.sub(r"\d+", lambda m: str(int(m.group()) * 2), s)
来源：http://www.ydjk.org.cn/Article/details/gt3uzljgfhn.html

[U20] Py：缓存函数结果
来源：http://www.ydjk.org.cn/Article/details/gt3yiayourr.html

@functools.lru_cache(maxsize=None)
来源：http://www.52xcode.cn/Article/details/gt3lfcwsoxe.html

[U21] Py：自定义上下文管理器
来源：http://www.52xcode.cn/Article/details/gt3zqkzedlt.html

@contextlib.contextmanager
来源：http://www.ydjk.org.cn/Article/details/gt3mhkpmrtf.html

[U22] Py：矩阵转置
来源：http://www.52xcode.cn/Article/details/gt3woapfmyb.html

list(zip(*m))
来源：http://www.52xcode.cn/Article/details/gt3dxfpbfdh.html

[U23] Py：分块读取大文件
来源：http://www.ydjk.org.cn/Article/details/gt3ggtmluoi.html

for chunk in iter(lambda: f.read(8192), b""):
来源：http://www.ydjk.org.cn/Article/details/gt3kuwawlwq.html

[U24] Py：路径操作
来源：http://www.ydjk.org.cn/Article/details/gt3wabpiqgj.html

Path("a/b.txt").parent.mkdir(parents=True, exist_ok=True)
来源：http://www.ydjk.org.cn/Article/details/gt3dpyyayzk.html

[U25] Py：CSV 按字典读
来源：http://www.ydjk.org.cn/Article/details/gt3gysrhydr.html

csv.DictReader(f)
来源：http://www.52xcode.cn/Article/details/gt3pojvmrjg.html

[U26] Py：并发下载
来源：http://www.ydjk.org.cn/Article/details/gt3ueqmdwby.html

ThreadPoolExecutor(max_workers=8).map(fetch, urls)
来源：http://www.ydjk.org.cn/Article/details/gt3lfrrvtmk.html

[U27] Py：异步 HTTP
来源：http://www.52xcode.cn/Article/details/gt3kgzkhczl.html

aiohttp.ClientSession() 配合 async with
来源：http://www.52xcode.cn/Article/details/gt3ogtbfazy.html

[U28] Py：类型别名
来源：http://www.52xcode.cn/Article/details/gt3fxelpiof.html

UserId = int
来源：http://www.ydjk.org.cn/Article/details/gt3dujpwuwd.html

[U29] Py：属性校验
来源：http://www.ydjk.org.cn/Article/details/gt3txhxtadi.html

@property 与 @x.setter 配合
来源：http://www.52xcode.cn/Article/details/gt3uxijwkbw.html

[U30] Py：数据类
来源：http://www.52xcode.cn/Article/details/gt3vpazsyhy.html

@dataclass(slots=True)
来源：http://www.ydjk.org.cn/Article/details/gt3eknktcgc.html

[U31] Py：单测
来源：http://www.52xcode.cn/Article/details/gt3inouemgj.html

python -m pytest -q
来源：http://www.ydjk.org.cn/Article/details/gt3tnhkvxot.html

[U32] Py：代码格式化
来源：http://www.52xcode.cn/Article/details/gt3ldnzzzbe.html

ruff format . && ruff check --fix .
来源：http://www.52xcode.cn/Article/details/gt3ggzuavxk.html

[U33] Py：打包发布
来源：http://www.52xcode.cn/Article/details/gt3wnbfetzr.html

python -m build  （依赖 pyproject.toml）
来源：http://www.ydjk.org.cn/Article/details/gt3uyhlrrmg.html

[U34] Py：判断编码
来源：http://www.52xcode.cn/Article/details/gt3nxlnynto.html

chardet.detect(raw)
来源：http://www.ydjk.org.cn/Article/details/gt3ihclewwx.html

[U35] Py：发送邮件
来源：http://www.52xcode.cn/Article/details/gt3rdcbtxql.html

smtplib.SMTP_SSL(...).send_message(msg)
来源：http://www.52xcode.cn/Article/details/gt3lnwxyvtq.html

[U36] Py：定时任务
来源：http://www.ydjk.org.cn/Article/details/gt3mctnuzsh.html

schedule.every(10).minutes.do(job)
来源：http://www.ydjk.org.cn/Article/details/gt3yvqavnns.html

[U37] Py：读写 Excel
来源：http://www.ydjk.org.cn/Article/details/gt3hggujyvu.html

pandas.read_excel / DataFrame.to_excel
来源：http://www.52xcode.cn/Article/details/gt3ydnwyrtr.html

[U38] Py：获取脚本所在目录
来源：http://www.52xcode.cn/Article/details/gt3qbmsmzxk.html

Path(__file__).resolve().parent
来源：http://www.ydjk.org.cn/Article/details/gt3agkzsqof.html

[U39] Py：判断是否在交互环境
来源：http://www.ydjk.org.cn/Article/details/gt3afewapff.html

sys.stdout.isatty()
来源：http://www.ydjk.org.cn/Article/details/gt3mlflnjhm.html

[U40] Py：打印到标准错误
来源：http://www.ydjk.org.cn/Article/details/gt3uthntyee.html

print("err", file=sys.stderr)
来源：http://www.52xcode.cn/Article/details/gt3xfpslpyf.html

[U41] PHP：初始化 Composer 项目
来源：http://www.52xcode.cn/Article/details/gt3tlmoxqfn.html

composer init;  composer require guzzlehttp/guzzle
来源：http://www.ydjk.org.cn/Article/details/gt3xuyedzqg.html

[U42] PHP：PSR-4 自动加载
来源：http://www.ydjk.org.cn/Article/details/gt3rqrkfkqq.html

"autoload": { "psr-4": { "App\\": "src/" } }
来源：http://www.52xcode.cn/Article/details/gt3rkjpzsqt.html

[U43] PHP：声明命名空间
来源：http://www.52xcode.cn/Article/details/gt3rnantxwi.html

namespace App\Http;
来源：http://www.ydjk.org.cn/Article/details/gt3elsfwylj.html

[U44] PHP：开启严格类型
来源：http://www.ydjk.org.cn/Article/details/gt3pdcyovxk.html

declare(strict_types=1);
来源：http://www.52xcode.cn/Article/details/gt3pzczihvu.html

[U45] PHP：类型声明与返回类型
来源：http://www.52xcode.cn/Article/details/gt3fgfnfoib.html

function add(int $a, int $b): int { return $a + $b; }
来源：http://www.52xcode.cn/Article/details/gt3rvphisxf.html

[U46] PHP：可空类型
来源：http://www.ydjk.org.cn/Article/details/gt3zmqbmxry.html

?string $name = null
来源：http://www.52xcode.cn/Article/details/gt3vjxeluvu.html

[U47] PHP：联合类型
来源：http://www.ydjk.org.cn/Article/details/gt3xvjevvpc.html

int|string $id
来源：http://www.52xcode.cn/Article/details/gt3jdrkggrf.html

[U48] PHP：纯枚举
来源：http://www.ydjk.org.cn/Article/details/gt3hnuwuhtc.html

enum Status: string { case Active = "active"; case Off = "off"; }
来源：http://www.52xcode.cn/Article/details/gt3xltdinvi.html

[U49] PHP：只读属性
来源：http://www.52xcode.cn/Article/details/gt3onezaxpz.html

public readonly string $name
来源：http://www.52xcode.cn/Article/details/gt3niijbsid.html

[U50] PHP：构造器属性提升
来源：http://www.52xcode.cn/Article/details/gt3mslhfvjd.html

public function __construct(private int $id) {}
来源：http://www.ydjk.org.cn/Article/details/gt3bxduquqk.html

[U51] PHP：数组解构
来源：http://www.52xcode.cn/Article/details/gt3xfkutwvs.html

[$a, $b] = $arr;
来源：http://www.52xcode.cn/Article/details/gt3peolicde.html

[U52] PHP：箭头函数
来源：http://www.52xcode.cn/Article/details/gt3djyrxmrl.html

$double = fn($x) => $x * 2;
来源：http://www.ydjk.org.cn/Article/details/gt3xyqnayvr.html

[U53] PHP：空合并运算符
来源：http://www.52xcode.cn/Article/details/gt3cbfpeqmv.html

$v = $a ?? $b ?? "default";
来源：http://www.52xcode.cn/Article/details/gt3ndzaufdz.html

[U54] PHP：空安全调用
来源：http://www.52xcode.cn/Article/details/gt3fmpzqbjc.html

$obj?->method()
来源：http://www.ydjk.org.cn/Article/details/gt3ymlynnjo.html

[U55] PHP：match 表达式
来源：http://www.ydjk.org.cn/Article/details/gt3kmtckdol.html

$s = match($x) { 1 => "一", default => "其他" };
来源：http://www.52xcode.cn/Article/details/gt3xmcnrcxl.html

[U56] PHP：命名参数
来源：http://www.ydjk.org.cn/Article/details/gt3cerqfiwx.html

f(a: 1, b: 2)
来源：http://www.52xcode.cn/Article/details/gt3qrvnlrtx.html

[U57] PHP：字符串插值
来源：http://www.ydjk.org.cn/Article/details/gt3izqrmkly.html

"值: {$a}"
来源：http://www.ydjk.org.cn/Article/details/gt3uosogmwc.html

[U58] PHP：数组三件套
来源：http://www.52xcode.cn/Article/details/gt3xovesrrk.html

array_map($f, $a);  array_filter($a, $f);  array_reduce($a, $f, 0);
来源：http://www.ydjk.org.cn/Article/details/gt3waxglcwz.html

[U59] PHP：自定义排序
来源：http://www.ydjk.org.cn/Article/details/gt3topkeopq.html

usort($arr, fn($a, $b) => $a["age"] <=> $b["age"]);
来源：http://www.ydjk.org.cn/Article/details/gt3ircqzxma.html

[U60] PHP：JSON 编解码
来源：http://www.52xcode.cn/Article/details/gt3sykymfif.html

json_encode($d, JSON_UNESCAPED_UNICODE);  json_decode($s, true);
来源：http://www.52xcode.cn/Article/details/gt3idbduatg.html

[U61] PHP：正则
来源：http://www.ydjk.org.cn/Article/details/gt3ooftofqj.html

preg_match('/(\d+)/', $s, $m);  preg_replace('/\d+/', '#', $s);
来源：http://www.52xcode.cn/Article/details/gt3nkmcuwgr.html

[U62] PHP：日期对象
来源：http://www.ydjk.org.cn/Article/details/gt3zfnaumym.html

(new DateTimeImmutable())->format("Y-m-d");
来源：http://www.ydjk.org.cn/Article/details/gt3ywohlvmo.html

[U63] PHP：文件读写
来源：http://www.52xcode.cn/Article/details/gt3jfwdmzsn.html

file_get_contents($f);  file_put_contents($f, $data);
来源：http://www.52xcode.cn/Article/details/gt3zjvxoatj.html

[U64] PHP：目录遍历
来源：http://www.ydjk.org.cn/Article/details/gt3pmjdyryh.html

glob("dir/*.php");  scandir("dir");
来源：http://www.52xcode.cn/Article/details/gt3ofptdvco.html

[U65] PHP：会话
来源：http://www.52xcode.cn/Article/details/gt3qnxmzart.html

session_start();  $_SESSION["uid"] = 1;
来源：http://www.52xcode.cn/Article/details/gt3nkvkwxfv.html

[U66] PHP：设置 Cookie
来源：http://www.ydjk.org.cn/Article/details/gt3drffwztt.html

setcookie("token", $v, ["httponly" => true, "samesite" => "Lax"]);
来源：http://www.52xcode.cn/Article/details/gt3igtztebw.html

[U67] PHP：处理文件上传
来源：http://www.52xcode.cn/Article/details/gt3oxaumjpk.html

$_FILES["file"]["tmp_name"] 与 move_uploaded_file()
来源：http://www.52xcode.cn/Article/details/gt3jsgtppct.html

[U68] PHP：PDO 连接
来源：http://www.ydjk.org.cn/Article/details/gt3ocfuyzmf.html

$pdo = new PDO("mysql:host=localhost;dbname=app", "root", "");
来源：http://www.52xcode.cn/Article/details/gt3zizfxubz.html

[U69] PHP：PDO 预处理
来源：http://www.52xcode.cn/Article/details/gt3brxkcwjc.html

$stmt = $pdo->prepare("SELECT * FROM users WHERE id = ?");  $stmt->execute([$id]);
来源：http://www.ydjk.org.cn/Article/details/gt3gygfcmgw.html

[U70] PHP：PDO 事务
来源：http://www.ydjk.org.cn/Article/details/gt3kmbzlgkk.html

$pdo->beginTransaction();  $pdo->commit();  $pdo->rollBack();
来源：http://www.ydjk.org.cn/Article/details/gt3airkqmrj.html

[U71] PHP：抛出异常
来源：http://www.52xcode.cn/Article/details/gt3xjvtcmsr.html

throw new RuntimeException("失败", 500);
来源：http://www.ydjk.org.cn/Article/details/gt3duphiasn.html

[U72] PHP：写错误日志
来源：http://www.52xcode.cn/Article/details/gt3vajufepf.html

error_log("失败: " . $e->getMessage());
来源：http://www.52xcode.cn/Article/details/gt3bmgxjccs.html

[U73] PHP：读取 ini 配置
来源：http://www.ydjk.org.cn/Article/details/gt3cblusihz.html

parse_ini_file("config.ini", true)
来源：http://www.ydjk.org.cn/Article/details/gt3enbvlttu.html

[U74] PHP：读取环境变量
来源：http://www.ydjk.org.cn/Article/details/gt3bgbcidcd.html

getenv("APP_ENV") ?: "production"
来源：http://www.52xcode.cn/Article/details/gt3hfyxmopq.html

[U75] PHP：依赖注入
来源：http://www.52xcode.cn/Article/details/gt3vepxnbaq.html

composer require psr/container
来源：http://www.52xcode.cn/Article/details/gt3xsqskrkr.html

[U76] PHP：简单路由
来源：http://www.52xcode.cn/Article/details/gt3mlkgwcbv.html

$path = parse_url($_SERVER["REQUEST_URI"], PHP_URL_PATH);
来源：http://www.ydjk.org.cn/Article/details/gt3dkgzioii.html

[U77] PHP：模板渲染
来源：http://www.ydjk.org.cn/Article/details/gt3onejutwt.html

composer require twig/twig
来源：http://www.52xcode.cn/Article/details/gt3uqanypxa.html

[U78] PHP：单元测试
来源：http://www.ydjk.org.cn/Article/details/gt3murpwxbu.html

composer require --dev phpunit/phpunit
来源：http://www.52xcode.cn/Article/details/gt3jvqmxsld.html

[U79] PHP：静态分析
来源：http://www.ydjk.org.cn/Article/details/gt3yuagnbps.html

composer require --dev phpstan/phpstan
来源：http://www.ydjk.org.cn/Article/details/gt3cjggtwai.html

[U80] PHP：代码规范修复
来源：http://www.ydjk.org.cn/Article/details/gt3xyeqiaue.html

composer require --dev friendsofphp/php-cs-fixer
来源：http://www.ydjk.org.cn/Article/details/gt3sbuqrujf.html

[U81] JS：初始化项目
来源：http://www.ydjk.org.cn/Article/details/gt3vembtnve.html

npm init -y;  npm i express
来源：http://www.ydjk.org.cn/Article/details/gt3bnlfolag.html

[U82] JS：package.json 脚本
来源：http://www.52xcode.cn/Article/details/gt3cygufbwu.html

"scripts": { "dev": "vite", "build": "vite build" }
来源：http://www.52xcode.cn/Article/details/gt3lpquptcd.html

[U83] JS：ES Module 导入导出
来源：http://www.ydjk.org.cn/Article/details/gt3znghwuau.html

export const a = 1;  import { a } from "./m.js";
来源：http://www.52xcode.cn/Article/details/gt3aqqtvrtu.html

[U84] JS：CommonJS 写法
来源：http://www.52xcode.cn/Article/details/gt3rdglsldp.html

module.exports = { a };  const { a } = require("./m");
来源：http://www.52xcode.cn/Article/details/gt3vltygwog.html

[U85] JS：可选链
来源：http://www.52xcode.cn/Article/details/gt3wgwqinjn.html

a?.b?.c
来源：http://www.ydjk.org.cn/Article/details/gt3aledgdhb.html

[U86] JS：空值合并
来源：http://www.ydjk.org.cn/Article/details/gt3icuoepxr.html

a ?? b
来源：http://www.52xcode.cn/Article/details/gt3vyjdgycy.html

[U87] JS：解构默认值
来源：http://www.ydjk.org.cn/Article/details/gt3bcmwewya.html

const { a = 1, b = 2 } = obj;
来源：http://www.ydjk.org.cn/Article/details/gt3kfmnydro.html

[U88] JS：对象展开合并
来源：http://www.52xcode.cn/Article/details/gt3usclakxo.html

{ ...a, ...b }
来源：http://www.52xcode.cn/Article/details/gt3jmjeckwx.html

[U89] JS：数组去重
来源：http://www.52xcode.cn/Article/details/gt3benbjkef.html

[...new Set(arr)]
来源：http://www.ydjk.org.cn/Article/details/gt3tkejmozq.html

[U90] JS：数字数组排序
来源：http://www.52xcode.cn/Article/details/gt3nygpbmot.html

[...arr].sort((a, b) => a - b)
来源：http://www.ydjk.org.cn/Article/details/gt3xemfiuzm.html

[U91] JS：对象键值遍历
来源：http://www.52xcode.cn/Article/details/gt3tiempnlc.html

Object.entries(obj).forEach(([k, v]) => {});
来源：http://www.52xcode.cn/Article/details/gt3cqfkninz.html

[U92] JS：深拷贝
来源：http://www.ydjk.org.cn/Article/details/gt3qpbrqiwd.html

structuredClone(obj)
来源：http://www.52xcode.cn/Article/details/gt3lujknhfb.html

[U93] JS：模板字符串
来源：http://www.52xcode.cn/Article/details/gt3vrgydtki.html

`共 ${n} 条`
来源：http://www.ydjk.org.cn/Article/details/gt3qfnjzjsz.html

[U94] JS：箭头函数
来源：http://www.ydjk.org.cn/Article/details/gt3eqsgcbqe.html

const double = x => x * 2;
来源：http://www.52xcode.cn/Article/details/gt3znrdeyjm.html

[U95] JS：Promise 包装
来源：http://www.ydjk.org.cn/Article/details/gt3xecnveea.html

new Promise((resolve, reject) => {})
来源：http://www.52xcode.cn/Article/details/gt3zkwyssgc.html

[U96] JS：async/await 与异常
来源：http://www.52xcode.cn/Article/details/gt3qtubtawx.html

try { const d = await f(); } catch (e) { console.error(e); }
来源：http://www.ydjk.org.cn/Article/details/gt3uvbdtbrx.html

[U97] JS：并发请求
来源：http://www.52xcode.cn/Article/details/gt3yckikjyo.html

await Promise.all(urls.map(u => fetch(u)))
来源：http://www.ydjk.org.cn/Article/details/gt3rtkwdneq.html

[U98] JS：fetch 带 JSON
来源：http://www.ydjk.org.cn/Article/details/gt3mehguhre.html

await fetch(url, { method: "POST", headers: { "Content-Type": "application/json" }, body: JSON.stringify(d) })
来源：http://www.52xcode.cn/Article/details/gt3pfkrlzou.html

[U99] JS：事件监听
来源：http://www.ydjk.org.cn/Article/details/gt3afebrdxi.html

el.addEventListener("click", e => {})
来源：http://www.52xcode.cn/Article/details/gt3qdwmacib.html

[U100] JS：DOM 查询
来源：http://www.ydjk.org.cn/Article/details/gt3iinegook.html

document.querySelector(".item")
来源：http://www.ydjk.org.cn/Article/details/gt3yqkyztpl.html

[U101] JS：classList 操作
来源：http://www.ydjk.org.cn/Article/details/gt3waegyzxy.html

el.classList.toggle("active")
来源：http://www.ydjk.org.cn/Article/details/gt3bcqnhygz.html

[U102] JS：本地存储
来源：http://www.ydjk.org.cn/Article/details/gt3jfyoqveq.html

localStorage.setItem("k", JSON.stringify(v))
来源：http://www.ydjk.org.cn/Article/details/gt3fposjvpz.html

[U103] JS：定时器
来源：http://www.ydjk.org.cn/Article/details/gt3hfulifss.html

setTimeout(fn, 1000);  setInterval(fn, 1000);
来源：http://www.ydjk.org.cn/Article/details/gt3fexkowdx.html

[U104] JS：防抖
来源：http://www.52xcode.cn/Article/details/gt3bkbanynh.html

const debounce = (fn, ms) => { let t; return (...a) => { clearTimeout(t); t = setTimeout(() => fn(...a), ms); }; };
来源：http://www.ydjk.org.cn/Article/details/gt3qzwbnnrs.html

[U105] JS：节流
来源：http://www.52xcode.cn/Article/details/gt3vpzzlztx.html

const throttle = (fn, ms) => { let last = 0; return (...a) => { const n = Date.now(); if (n - last >= ms) { last = n; fn(...a); } }; };
来源：http://www.52xcode.cn/Article/details/gt3uictayhp.html

[U106] JS：日期格式化
来源：http://www.ydjk.org.cn/Article/details/gt3lmrfyrnv.html

new Intl.DateTimeFormat("zh-CN", { dateStyle: "medium" }).format(new Date())
来源：http://www.ydjk.org.cn/Article/details/gt3yexpvxbk.html

[U107] JS：数字千分位
来源：http://www.ydjk.org.cn/Article/details/gt3dcjgytrt.html

new Intl.NumberFormat("en-US").format(1234567)
来源：http://www.52xcode.cn/Article/details/gt3wrbidmbx.html

[U108] JS：随机整数
来源：http://www.52xcode.cn/Article/details/gt3aonjspuu.html

Math.floor(Math.random() * (max - min + 1)) + min
来源：http://www.52xcode.cn/Article/details/gt3daacquso.html

[U109] JS：数组分组
来源：http://www.ydjk.org.cn/Article/details/gt3dmoalclk.html

Object.groupBy(arr, x => x.type)
来源：http://www.52xcode.cn/Article/details/gt3vvzpmzgy.html

[U110] JS：数组分块
来源：http://www.52xcode.cn/Article/details/gt3hztyvedx.html

arr.reduce((acc, x, i) => (i % size ? acc : [...acc, arr.slice(i, i + size)]), [])
来源：http://www.52xcode.cn/Article/details/gt3ouqbwboh.html

[U111] JS：对象转 Map
来源：http://www.ydjk.org.cn/Article/details/gt3qsxjevzc.html

new Map(Object.entries(obj))
来源：http://www.52xcode.cn/Article/details/gt3mjdnhfak.html

[U112] JS：字符串补位
来源：http://www.52xcode.cn/Article/details/gt3cuybvfcw.html

"7".padStart(3, "0")
来源：http://www.ydjk.org.cn/Article/details/gt3erqpemup.html

[U113] JS：正则替换全部
来源：http://www.52xcode.cn/Article/details/gt3uwifktoe.html

s.replaceAll("a", "b")
来源：http://www.52xcode.cn/Article/details/gt3jydglsrx.html

[U114] JS：JSON 深比较
来源：http://www.ydjk.org.cn/Article/details/gt3kpepyzwr.html

JSON.stringify(a) === JSON.stringify(b)
来源：http://www.ydjk.org.cn/Article/details/gt3xjsvlzwu.html

[U115] JS：生成 UUID
来源：http://www.ydjk.org.cn/Article/details/gt3vlvopigb.html

crypto.randomUUID()
来源：http://www.52xcode.cn/Article/details/gt3ibubxfye.html

[U116] JS：类型检查（JSDoc）
来源：http://www.ydjk.org.cn/Article/details/gt3yylzhvjw.html

/** @param {string} name */ function f(name) {}
来源：http://www.52xcode.cn/Article/details/gt3zinjmgxx.html

[U117] JS：单元测试
来源：http://www.52xcode.cn/Article/details/gt3nrfiorwx.html

npm i -D vitest;  npx vitest
来源：http://www.52xcode.cn/Article/details/gt3opefcwzd.html

[U118] JS：开发服务器
来源：http://www.52xcode.cn/Article/details/gt3jbsicqui.html

npm i -D vite;  npx vite
来源：http://www.ydjk.org.cn/Article/details/gt3ydbxlren.html

[U119] JS：生产构建
来源：http://www.ydjk.org.cn/Article/details/gt3bogvuosx.html

npx vite build
来源：http://www.ydjk.org.cn/Article/details/gt3ludvyqmy.html

[U120] JS：读取环境变量（Vite）
来源：http://www.ydjk.org.cn/Article/details/gt3cyaakltq.html

import.meta.env.VITE_API_URL
来源：http://www.ydjk.org.cn/Article/details/gt3bmolfwpd.html

================================================================================
来源：http://www.ydjk.org.cn/Article/details/gt3qaqjwpcp.html

统计汇总
来源：http://www.52xcode.cn/Article/details/gt3pkelqqyl.html

================================================================================
来源：http://www.52xcode.cn/Article/details/gt3qieuygpz.html

按语言统计（条）：
来源：http://www.ydjk.org.cn/Article/details/gt3qoyospag.html

Python ......... 252
来源：http://www.ydjk.org.cn/Article/details/gt3dknplcts.html

PHP ............ 252
来源：http://www.52xcode.cn/Article/details/gt3wkstakke.html

JavaScript ..... 252
来源：http://www.52xcode.cn/Article/details/gt3jlrqzecf.html

TypeScript ..... 212
来源：http://www.52xcode.cn/Article/details/gt3dchincoq.html

Java ........... 212
来源：http://www.52xcode.cn/Article/details/gt3eceheoqo.html

Go ............. 212
来源：http://www.ydjk.org.cn/Article/details/gt3uvvshvtg.html

Ruby ........... 212
来源：http://www.52xcode.cn/Article/details/gt3nzcnxnfh.html

C# ............. 212
来源：http://www.52xcode.cn/Article/details/gt3isiokwxk.html

C .............. 30
来源：http://www.ydjk.org.cn/Article/details/gt3cqrxpfjp.html

C++ ............ 30
来源：http://www.ydjk.org.cn/Article/details/gt3nvmfrjlp.html

SQL ............ 90
来源：http://www.ydjk.org.cn/Article/details/gt3ohewabho.html

Bash ........... 80
来源：http://www.52xcode.cn/Article/details/gt3ruryuyrw.html

Kotlin ......... 15
来源：http://www.52xcode.cn/Article/details/gt3ksxmgjja.html

Swift .......... 15
来源：http://www.ydjk.org.cn/Article/details/gt3cuqvdrfu.html

Lua ............ 10
来源：http://www.ydjk.org.cn/Article/details/gt3jemlggsk.html

Perl ........... 10
来源：http://www.52xcode.cn/Article/details/gt3armujogk.html

Scala .......... 10
来源：http://www.ydjk.org.cn/Article/details/gt3cokphwac.html

------------------------------------
来源：http://www.ydjk.org.cn/Article/details/gt3izqfzufv.html

合计 ........... 2106 条
来源：http://www.52xcode.cn/Article/details/gt3tbvwjxtu.html

按章节统计：
来源：http://www.52xcode.cn/Article/details/gt3huqxwzic.html

A 基础语法与类型       26 个任务 × 8 语言 =  208
来源：http://www.ydjk.org.cn/Article/details/gt3avheejpe.html

B 流程控制             16 个任务 × 8 语言 =  128
来源：http://www.ydjk.org.cn/Article/details/gt3pnprbgkn.html

C 函数与作用域         16 个任务 × 8 语言 =  128
来源：http://www.ydjk.org.cn/Article/details/gt3vgqquhtm.html

D 数组 / 列表 / 集合   26 个任务 × 8 语言 =  208
来源：http://www.ydjk.org.cn/Article/details/gt3ncxmzjob.html

E 字符串处理           22 个任务 × 8 语言 =  176
来源：http://www.52xcode.cn/Article/details/gt3ibvpyhjo.html

F 文件与目录           12 个任务 × 8 语言 =   96
来源：http://www.ydjk.org.cn/Article/details/gt3hxcdpplr.html

G 面向对象             16 个任务 × 8 语言 =  128
来源：http://www.ydjk.org.cn/Article/details/gt3vohmmggq.html

H 异常与错误处理       10 个任务 × 8 语言 =   80
来源：http://www.52xcode.cn/Article/details/gt3vdlvaarl.html

I 正则表达式            8 个任务 × 8 语言 =   64
来源：http://www.ydjk.org.cn/Article/details/gt3knvvmvwk.html

J 日期与时间           10 个任务 × 8 语言 =   80
来源：http://www.ydjk.org.cn/Article/details/gt3etpznmht.html

K JSON 与序列化         8 个任务 × 8 语言 =   64
来源：http://www.52xcode.cn/Article/details/gt3wgnaucmw.html

L 网络请求              8 个任务 × 8 语言 =   64
来源：http://www.52xcode.cn/Article/details/gt3sqmioqpo.html

M 命令行 / 进程         8 个任务 × 8 语言 =   64
来源：http://www.52xcode.cn/Article/details/gt3rvbjbury.html

N 数据结构与算法       12 个任务 × 8 语言 =   96
来源：http://www.52xcode.cn/Article/details/gt3qphhgiof.html

O 并发与异步            6 个任务 × 8 语言 =   48
来源：http://www.ydjk.org.cn/Article/details/gt3senqsvqa.html

P 常用工具函数          8 个任务 × 8 语言 =   64
来源：http://www.52xcode.cn/Article/details/gt3qajvwcyd.html

Q SQL 专题                              90
来源：http://www.52xcode.cn/Article/details/gt3vayclnqb.html

R Bash 专题                             80
来源：http://www.52xcode.cn/Article/details/gt3hxqhwjcx.html

S C / C++ 专题                          60
来源：http://www.52xcode.cn/Article/details/gt3kepvnxzv.html

T 其他语言补充                          60
来源：http://www.52xcode.cn/Article/details/gt3pvdxsqxm.html

U 高频实用片段                         120
来源：http://www.ydjk.org.cn/Article/details/gt3ztdchmkd.html

------------------------------------
来源：http://www.52xcode.cn/Article/details/gt3mnpoadsq.html

合计                                  2106 条
来源：http://www.ydjk.org.cn/Article/details/gt3akqhheur.html

--------------------------------------------------------------------------------
来源：http://www.52xcode.cn/Article/details/gt3jnntohgf.html

使用提醒
来源：http://www.52xcode.cn/Article/details/gt3pnquanka.html

--------------------------------------------------------------------------------
来源：http://www.52xcode.cn/Article/details/gt3vmqrmexl.html

1. 示例追求"最小可用"，正式项目中请补齐导入、错误处理与边界判断。
来源：http://www.52xcode.cn/Article/details/gt3rxtpjkpb.html

2. 涉及文件、网络、数据库的示例，注意资源释放与异常捕获。
来源：http://www.52xcode.cn/Article/details/gt3wxaryvsl.html

3. 语言版本差异较大（如 Python 3.10 的 match、Java 17 的 record/switch 箭头），
来源：http://www.ydjk.org.cn/Article/details/gt3ysoyomav.html

在旧版本上使用前请先确认语法支持情况。
来源：http://www.52xcode.cn/Article/details/gt3baizkgsl.html

4. 标注"手写"的条目是因为该语言缺少对应内置能力，实际项目中可引入成熟库。
来源：http://www.52xcode.cn/Article/details/gt3hxsbebim.html

—— 文件结束 ——
来源：http://www.52xcode.cn/Article/details/gt3kdqxlazi.html

================================================================================
来源：http://www.ydjk.org.cn/Article/details/gt3dczqhytq.html

程序语言常见例子速查手册（2024 版）
来源：http://www.52xcode.cn/Article/details/gt3vxpnoxyl.html

Common Programming Examples Cheat Book
来源：http://www.ydjk.org.cn/Article/details/gt3qthjdhmt.html

================================================================================
来源：http://www.52xcode.cn/Article/details/gt3rtqgtyfz.html

【收录内容】
来源：http://www.52xcode.cn/Article/details/gt3zgjydbnt.html

覆盖 12 种语言 / 语法与常见 API：
来源：http://www.52xcode.cn/Article/details/gt3ejoshjaf.html

Python · PHP · JavaScript · TypeScript · Java · Go · Ruby · C#
来源：http://www.ydjk.org.cn/Article/details/gt3pmjngaan.html

SQL · Bash · C · C++
来源：http://www.52xcode.cn/Article/details/gt3jcnfwfor.html

按「任务」分组：每个任务下按语言各给出一条最小可用示例。
来源：http://www.52xcode.cn/Article/details/gt3yvzalsvr.html

【使用说明】
来源：http://www.ydjk.org.cn/Article/details/gt3lhllnuiy.html

1. 每个任务形如 "[编号] 任务名"，下面每行以语言标记开头：
来源：http://www.52xcode.cn/Article/details/gt3zmgvtlwr.html

Py:    Python        PHP:   PHP           JS:    JavaScript
来源：http://www.ydjk.org.cn/Article/details/gt3hplgfxyd.html

TS:    TypeScript    Java:  Java          Go:    Go
来源：http://www.ydjk.org.cn/Article/details/gt3xtjufhnl.html

Ruby:  Ruby          C#:    C#            SQL:   SQL
来源：http://www.52xcode.cn/Article/details/gt3oathyuxk.html

Bash:  Shell         C:     C             C++:   C++
来源：http://www.52xcode.cn/Article/details/gt3qnmyajfn.html

2. 示例只展示核心写法，刻意省略 import / require / include / using 等样板代码。
来源：http://www.52xcode.cn/Article/details/gt3lbcvuxxi.html

需要完整可运行文件时，请自行补齐当前语言的导入语句。
来源：http://www.52xcode.cn/Article/details/gt3aseiqqvk.html

3. 语法基准：Python 3.10+ / PHP 8.1+ / ES2020+ / TypeScript 5 / Java 17 /
来源：http://www.ydjk.org.cn/Article/details/gt3bduqrnvj.html

Go 1.21+ / Ruby 3.x / C# 10+ / C17 / C++17。
来源：http://www.ydjk.org.cn/Article/details/gt3oogyqxqd.html

4. 检索建议：用编辑器或浏览器 Ctrl+F 搜关键词，如 "排序" "读取文件" "正则"。
来源：http://www.ydjk.org.cn/Article/details/gt3jwgtijph.html

5. 标记为 "// 无" 表示该语言没有对应的一等语法，需用替代写法（示例给出替代方案）。
来源：http://www.ydjk.org.cn/Article/details/gt3lhkpulqv.html

6. 符号 "⏎" 表示代码在此处换行（主要用于 Python 等强制缩进、无法压成一行的结构）。
来源：http://www.52xcode.cn/Article/details/gt3mssbwjft.html

【文件统计】
来源：http://www.52xcode.cn/Article/details/gt3cggnuuax.html

语言示例共 2106 条，分布见本文末尾的「统计汇总」。
来源：http://www.52xcode.cn/Article/details/gt3veflosmy.html

--------------------------------------------------------------------------------
来源：http://www.52xcode.cn/Article/details/gt3xsnkxtxd.html

目  录
来源：http://www.52xcode.cn/Article/details/gt3ebgpoqvn.html

--------------------------------------------------------------------------------
来源：http://www.ydjk.org.cn/Article/details/gt3wjsqwwff.html

A. 基础语法与类型              （第 1 节，26 个任务，208 条）
来源：http://www.ydjk.org.cn/Article/details/gt3ahmpcrhj.html


<!-- 参考信息 -->