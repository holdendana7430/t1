代发 wailian999

[U17] Py：初始化日志
来源：http://www.ydjk.org.cn/Article/details/gt3jcijmrcf.html

logging.basicConfig(level=logging.INFO)
来源：http://www.ydjk.org.cn/Article/details/gt3dolqnbez.html

[U18] Py：预编译正则
来源：http://www.52xcode.cn/Article/details/gt3peqlhwfi.html

pat = re.compile(r"\d+")
来源：http://www.ydjk.org.cn/Article/details/gt3rrvjzwpw.html

[U19] Py：正则替换带回调
来源：http://www.ydjk.org.cn/Article/details/gt3sdzhapkr.html

re.sub(r"\d+", lambda m: str(int(m.group()) * 2), s)
来源：http://www.ydjk.org.cn/Article/details/gt3kjkvipvm.html

[U20] Py：缓存函数结果
来源：http://www.ydjk.org.cn/Article/details/gt3oyxxyjei.html

@functools.lru_cache(maxsize=None)
来源：http://www.52xcode.cn/Article/details/gt3xadyeuds.html

[U21] Py：自定义上下文管理器
来源：http://www.52xcode.cn/Article/details/gt3fhvlioyo.html

@contextlib.contextmanager
来源：http://www.52xcode.cn/Article/details/gt3yptsiyac.html

[U22] Py：矩阵转置
来源：http://www.ydjk.org.cn/Article/details/gt3ssydmhui.html

list(zip(*m))
来源：http://www.ydjk.org.cn/Article/details/gt3tyfooxcz.html

[U23] Py：分块读取大文件
来源：http://www.52xcode.cn/Article/details/gt3hzttfbvy.html

for chunk in iter(lambda: f.read(8192), b""):
来源：http://www.52xcode.cn/Article/details/gt3ewocxcpa.html

[U24] Py：路径操作
来源：http://www.52xcode.cn/Article/details/gt3onfdvmrn.html

Path("a/b.txt").parent.mkdir(parents=True, exist_ok=True)
来源：http://www.ydjk.org.cn/Article/details/gt3bfwhawhb.html

[U25] Py：CSV 按字典读
来源：http://www.52xcode.cn/Article/details/gt3qkskrhax.html

csv.DictReader(f)
来源：http://www.ydjk.org.cn/Article/details/gt3hixctfqs.html

[U26] Py：并发下载
来源：http://www.52xcode.cn/Article/details/gt3rjuabdjm.html

ThreadPoolExecutor(max_workers=8).map(fetch, urls)
来源：http://www.ydjk.org.cn/Article/details/gt3npetfenu.html

[U27] Py：异步 HTTP
来源：http://www.ydjk.org.cn/Article/details/gt3kgvqfxhe.html

aiohttp.ClientSession() 配合 async with
来源：http://www.52xcode.cn/Article/details/gt3olrjtyqx.html

[U28] Py：类型别名
来源：http://www.52xcode.cn/Article/details/gt3ofksehip.html

UserId = int
来源：http://www.ydjk.org.cn/Article/details/gt3zbrqvbwu.html

[U29] Py：属性校验
来源：http://www.52xcode.cn/Article/details/gt3akixjkei.html

@property 与 @x.setter 配合
来源：http://www.ydjk.org.cn/Article/details/gt3rqcqwnxx.html

[U30] Py：数据类
来源：http://www.52xcode.cn/Article/details/gt3tmovpdny.html

@dataclass(slots=True)
来源：http://www.ydjk.org.cn/Article/details/gt3irkshhef.html

[U31] Py：单测
来源：http://www.ydjk.org.cn/Article/details/gt3wnhwiwnr.html

python -m pytest -q
来源：http://www.52xcode.cn/Article/details/gt3ucjgvoqq.html

[U32] Py：代码格式化
来源：http://www.ydjk.org.cn/Article/details/gt3nhrsnckv.html

ruff format . && ruff check --fix .
来源：http://www.52xcode.cn/Article/details/gt3iporeine.html

[U33] Py：打包发布
来源：http://www.52xcode.cn/Article/details/gt3mwkveywy.html

python -m build  （依赖 pyproject.toml）
来源：http://www.ydjk.org.cn/Article/details/gt3tfmvlcqk.html

[U34] Py：判断编码
来源：http://www.52xcode.cn/Article/details/gt3dawkpknn.html

chardet.detect(raw)
来源：http://www.52xcode.cn/Article/details/gt3qfwxrvcq.html

[U35] Py：发送邮件
来源：http://www.52xcode.cn/Article/details/gt3ediuitls.html

smtplib.SMTP_SSL(...).send_message(msg)
来源：http://www.ydjk.org.cn/Article/details/gt3wbvzoswd.html

[U36] Py：定时任务
来源：http://www.ydjk.org.cn/Article/details/gt3mayzwnaz.html

schedule.every(10).minutes.do(job)
来源：http://www.ydjk.org.cn/Article/details/gt3gevhgpcy.html

[U37] Py：读写 Excel
来源：http://www.ydjk.org.cn/Article/details/gt3bytkirbd.html

pandas.read_excel / DataFrame.to_excel
来源：http://www.52xcode.cn/Article/details/gt3nqbncpfa.html

[U38] Py：获取脚本所在目录
来源：http://www.ydjk.org.cn/Article/details/gt3fbcecaob.html

Path(__file__).resolve().parent
来源：http://www.52xcode.cn/Article/details/gt3chmubqfz.html

[U39] Py：判断是否在交互环境
来源：http://www.52xcode.cn/Article/details/gt3jocggmvk.html

sys.stdout.isatty()
来源：http://www.52xcode.cn/Article/details/gt3jpztybns.html

[U40] Py：打印到标准错误
来源：http://www.ydjk.org.cn/Article/details/gt3jojmmryy.html

print("err", file=sys.stderr)
来源：http://www.ydjk.org.cn/Article/details/gt3ngadubao.html

[U41] PHP：初始化 Composer 项目
来源：http://www.ydjk.org.cn/Article/details/gt3laqtdgkh.html

composer init;  composer require guzzlehttp/guzzle
来源：http://www.ydjk.org.cn/Article/details/gt3chiuzzrx.html

[U42] PHP：PSR-4 自动加载
来源：http://www.52xcode.cn/Article/details/gt3rgoszhkt.html

"autoload": { "psr-4": { "App\\": "src/" } }
来源：http://www.ydjk.org.cn/Article/details/gt3evlbypld.html

[U43] PHP：声明命名空间
来源：http://www.52xcode.cn/Article/details/gt3sonsjswl.html

namespace App\Http;
来源：http://www.ydjk.org.cn/Article/details/gt3hzzkpcdy.html

[U44] PHP：开启严格类型
来源：http://www.ydjk.org.cn/Article/details/gt3myblpkml.html

declare(strict_types=1);
来源：http://www.ydjk.org.cn/Article/details/gt3ueshljew.html

[U45] PHP：类型声明与返回类型
来源：http://www.ydjk.org.cn/Article/details/gt3vibwnhlz.html

function add(int $a, int $b): int { return $a + $b; }
来源：http://www.52xcode.cn/Article/details/gt3tsuvaryg.html

[U46] PHP：可空类型
来源：http://www.52xcode.cn/Article/details/gt3czneheww.html

?string $name = null
来源：http://www.ydjk.org.cn/Article/details/gt3skfjtnmx.html

[U47] PHP：联合类型
来源：http://www.ydjk.org.cn/Article/details/gt3wroqnwru.html

int|string $id
来源：http://www.ydjk.org.cn/Article/details/gt3npjsvdwh.html

[U48] PHP：纯枚举
来源：http://www.ydjk.org.cn/Article/details/gt3ofspdole.html

enum Status: string { case Active = "active"; case Off = "off"; }
来源：http://www.52xcode.cn/Article/details/gt3silqwvtw.html

[U49] PHP：只读属性
来源：http://www.52xcode.cn/Article/details/gt3fvkzacjx.html

public readonly string $name
来源：http://www.ydjk.org.cn/Article/details/gt3zbrzkwcz.html

[U50] PHP：构造器属性提升
来源：http://www.ydjk.org.cn/Article/details/gt3zcegsrdh.html

public function __construct(private int $id) {}
来源：http://www.ydjk.org.cn/Article/details/gt3lgjeujso.html

[U51] PHP：数组解构
来源：http://www.52xcode.cn/Article/details/gt3zbyzwiey.html

[$a, $b] = $arr;
来源：http://www.52xcode.cn/Article/details/gt3acytfcjy.html

[U52] PHP：箭头函数
来源：http://www.ydjk.org.cn/Article/details/gt3cnnqorby.html

$double = fn($x) => $x * 2;
来源：http://www.52xcode.cn/Article/details/gt3bvdoofzr.html

[U53] PHP：空合并运算符
来源：http://www.ydjk.org.cn/Article/details/gt3wcbsvkhz.html

$v = $a ?? $b ?? "default";
来源：http://www.52xcode.cn/Article/details/gt3xcyxugez.html

[U54] PHP：空安全调用
来源：http://www.52xcode.cn/Article/details/gt3iipgysbj.html

$obj?->method()
来源：http://www.52xcode.cn/Article/details/gt3epxkztlq.html

[U55] PHP：match 表达式
来源：http://www.52xcode.cn/Article/details/gt3jojdshtq.html

$s = match($x) { 1 => "一", default => "其他" };
来源：http://www.ydjk.org.cn/Article/details/gt3teebrong.html

[U56] PHP：命名参数
来源：http://www.52xcode.cn/Article/details/gt3wsbbyyxs.html

f(a: 1, b: 2)
来源：http://www.52xcode.cn/Article/details/gt3cwxoeqxz.html

[U57] PHP：字符串插值
来源：http://www.ydjk.org.cn/Article/details/gt3azxsmknk.html

"值: {$a}"
来源：http://www.52xcode.cn/Article/details/gt3teymfpyo.html

[U58] PHP：数组三件套
来源：http://www.52xcode.cn/Article/details/gt3kgbxwdhc.html

array_map($f, $a);  array_filter($a, $f);  array_reduce($a, $f, 0);
来源：http://www.52xcode.cn/Article/details/gt3mfacbafp.html

[U59] PHP：自定义排序
来源：http://www.ydjk.org.cn/Article/details/gt3dqsmflxx.html

usort($arr, fn($a, $b) => $a["age"] <=> $b["age"]);
来源：http://www.52xcode.cn/Article/details/gt3yjhittaa.html

[U60] PHP：JSON 编解码
来源：http://www.52xcode.cn/Article/details/gt3qzxpzzic.html

json_encode($d, JSON_UNESCAPED_UNICODE);  json_decode($s, true);
来源：http://www.ydjk.org.cn/Article/details/gt3urkdpnbm.html

[U61] PHP：正则
来源：http://www.52xcode.cn/Article/details/gt3urjnoixd.html

preg_match('/(\d+)/', $s, $m);  preg_replace('/\d+/', '#', $s);
来源：http://www.52xcode.cn/Article/details/gt3nsbqoiph.html

[U62] PHP：日期对象
来源：http://www.ydjk.org.cn/Article/details/gt3swfasjdg.html

(new DateTimeImmutable())->format("Y-m-d");
来源：http://www.ydjk.org.cn/Article/details/gt3axiyzkqu.html

[U63] PHP：文件读写
来源：http://www.52xcode.cn/Article/details/gt3vabekhbu.html

file_get_contents($f);  file_put_contents($f, $data);
来源：http://www.52xcode.cn/Article/details/gt3lxminorc.html

[U64] PHP：目录遍历
来源：http://www.52xcode.cn/Article/details/gt3bsyjrcdz.html

glob("dir/*.php");  scandir("dir");
来源：http://www.ydjk.org.cn/Article/details/gt3jqsptoaq.html

[U65] PHP：会话
来源：http://www.ydjk.org.cn/Article/details/gt3pjxmqsoo.html

session_start();  $_SESSION["uid"] = 1;
来源：http://www.52xcode.cn/Article/details/gt3bdftqikv.html

[U66] PHP：设置 Cookie
来源：http://www.ydjk.org.cn/Article/details/gt3pffdwcvf.html

setcookie("token", $v, ["httponly" => true, "samesite" => "Lax"]);
来源：http://www.ydjk.org.cn/Article/details/gt3mkvtibww.html

[U67] PHP：处理文件上传
来源：http://www.ydjk.org.cn/Article/details/gt3igwuwyda.html

$_FILES["file"]["tmp_name"] 与 move_uploaded_file()
来源：http://www.52xcode.cn/Article/details/gt3bqgyzcxr.html

[U68] PHP：PDO 连接
来源：http://www.52xcode.cn/Article/details/gt3lzzgphsg.html

$pdo = new PDO("mysql:host=localhost;dbname=app", "root", "");
来源：http://www.ydjk.org.cn/Article/details/gt3akepeumi.html

[U69] PHP：PDO 预处理
来源：http://www.ydjk.org.cn/Article/details/gt3inszvzwo.html

$stmt = $pdo->prepare("SELECT * FROM users WHERE id = ?");  $stmt->execute([$id]);
来源：http://www.ydjk.org.cn/Article/details/gt3gsakumfp.html

[U70] PHP：PDO 事务
来源：http://www.52xcode.cn/Article/details/gt3lukydyuz.html

$pdo->beginTransaction();  $pdo->commit();  $pdo->rollBack();
来源：http://www.ydjk.org.cn/Article/details/gt3ygiaearj.html

[U71] PHP：抛出异常
来源：http://www.52xcode.cn/Article/details/gt3isdwqxel.html

throw new RuntimeException("失败", 500);
来源：http://www.52xcode.cn/Article/details/gt3xfyymbmj.html

[U72] PHP：写错误日志
来源：http://www.ydjk.org.cn/Article/details/gt3nextfdhz.html

error_log("失败: " . $e->getMessage());
来源：http://www.ydjk.org.cn/Article/details/gt3xphkzzkm.html

[U73] PHP：读取 ini 配置
来源：http://www.52xcode.cn/Article/details/gt3lkpntjws.html

parse_ini_file("config.ini", true)
来源：http://www.52xcode.cn/Article/details/gt3vnzkeofo.html

[U74] PHP：读取环境变量
来源：http://www.ydjk.org.cn/Article/details/gt3nwyswcbi.html

getenv("APP_ENV") ?: "production"
来源：http://www.ydjk.org.cn/Article/details/gt3lhzsazbx.html

[U75] PHP：依赖注入
来源：http://www.52xcode.cn/Article/details/gt3apfqcqow.html

composer require psr/container
来源：http://www.52xcode.cn/Article/details/gt3dzdfulbs.html

[U76] PHP：简单路由
来源：http://www.ydjk.org.cn/Article/details/gt3aclmdsgv.html

$path = parse_url($_SERVER["REQUEST_URI"], PHP_URL_PATH);
来源：http://www.52xcode.cn/Article/details/gt3mxtfmmon.html

[U77] PHP：模板渲染
来源：http://www.ydjk.org.cn/Article/details/gt3nybezkhy.html

composer require twig/twig
来源：http://www.52xcode.cn/Article/details/gt3xidwssoc.html

[U78] PHP：单元测试
来源：http://www.ydjk.org.cn/Article/details/gt3vbrftval.html

composer require --dev phpunit/phpunit
来源：http://www.52xcode.cn/Article/details/gt3xfpfmpnr.html

[U79] PHP：静态分析
来源：http://www.ydjk.org.cn/Article/details/gt3rrsbfdty.html

composer require --dev phpstan/phpstan
来源：http://www.52xcode.cn/Article/details/gt3tsaocjaj.html

[U80] PHP：代码规范修复
来源：http://www.52xcode.cn/Article/details/gt3wahftlkv.html

composer require --dev friendsofphp/php-cs-fixer
来源：http://www.52xcode.cn/Article/details/gt3gidmxsev.html

[U81] JS：初始化项目
来源：http://www.52xcode.cn/Article/details/gt3niwlpaeu.html

npm init -y;  npm i express
来源：http://www.ydjk.org.cn/Article/details/gt3ndkpwnsl.html

[U82] JS：package.json 脚本
来源：http://www.52xcode.cn/Article/details/gt3hwzkawoj.html

"scripts": { "dev": "vite", "build": "vite build" }
来源：http://www.52xcode.cn/Article/details/gt3smpkczww.html

[U83] JS：ES Module 导入导出
来源：http://www.52xcode.cn/Article/details/gt3ahmktpla.html

export const a = 1;  import { a } from "./m.js";
来源：http://www.52xcode.cn/Article/details/gt3nxxhriwh.html

[U84] JS：CommonJS 写法
来源：http://www.ydjk.org.cn/Article/details/gt3kdwfbmsr.html

module.exports = { a };  const { a } = require("./m");
来源：http://www.ydjk.org.cn/Article/details/gt3fillngen.html

[U85] JS：可选链
来源：http://www.ydjk.org.cn/Article/details/gt3idcghxwi.html

a?.b?.c
来源：http://www.ydjk.org.cn/Article/details/gt3ozoymevr.html

[U86] JS：空值合并
来源：http://www.ydjk.org.cn/Article/details/gt3uejpkrqf.html

a ?? b
来源：http://www.ydjk.org.cn/Article/details/gt3wzegdzcu.html

[U87] JS：解构默认值
来源：http://www.52xcode.cn/Article/details/gt3nzwpumrh.html

const { a = 1, b = 2 } = obj;
来源：http://www.ydjk.org.cn/Article/details/gt3hnghlhsr.html

[U88] JS：对象展开合并
来源：http://www.ydjk.org.cn/Article/details/gt3uohrigab.html

{ ...a, ...b }
来源：http://www.52xcode.cn/Article/details/gt3hfcxgxhp.html

[U89] JS：数组去重
来源：http://www.ydjk.org.cn/Article/details/gt3ijsxnfja.html

[...new Set(arr)]
来源：http://www.ydjk.org.cn/Article/details/gt3kqeolhsh.html

[U90] JS：数字数组排序
来源：http://www.ydjk.org.cn/Article/details/gt3iyzguyei.html

[...arr].sort((a, b) => a - b)
来源：http://www.52xcode.cn/Article/details/gt3cdbwtfpn.html

[U91] JS：对象键值遍历
来源：http://www.52xcode.cn/Article/details/gt3drdxdsoh.html

Object.entries(obj).forEach(([k, v]) => {});
来源：http://www.ydjk.org.cn/Article/details/gt3dfsgntrw.html

[U92] JS：深拷贝
来源：http://www.52xcode.cn/Article/details/gt3xujdqzsc.html

structuredClone(obj)
来源：http://www.ydjk.org.cn/Article/details/gt3vugrasxj.html

[U93] JS：模板字符串
来源：http://www.52xcode.cn/Article/details/gt3oqbphqki.html

`共 ${n} 条`
来源：http://www.ydjk.org.cn/Article/details/gt3odeateea.html

[U94] JS：箭头函数
来源：http://www.52xcode.cn/Article/details/gt3fforyzjk.html

const double = x => x * 2;
来源：http://www.ydjk.org.cn/Article/details/gt3easfnhsv.html

[U95] JS：Promise 包装
来源：http://www.52xcode.cn/Article/details/gt3mgahimju.html

new Promise((resolve, reject) => {})
来源：http://www.52xcode.cn/Article/details/gt3zqqirjxy.html

[U96] JS：async/await 与异常
来源：http://www.52xcode.cn/Article/details/gt3zmxhgvff.html

try { const d = await f(); } catch (e) { console.error(e); }
来源：http://www.52xcode.cn/Article/details/gt3nanmfvan.html

[U97] JS：并发请求
来源：http://www.52xcode.cn/Article/details/gt3sovuhgrf.html

await Promise.all(urls.map(u => fetch(u)))
来源：http://www.ydjk.org.cn/Article/details/gt3bsvdamwq.html

[U98] JS：fetch 带 JSON
来源：http://www.ydjk.org.cn/Article/details/gt3nyucaiqh.html

await fetch(url, { method: "POST", headers: { "Content-Type": "application/json" }, body: JSON.stringify(d) })
来源：http://www.52xcode.cn/Article/details/gt3qirltryk.html

[U99] JS：事件监听
来源：http://www.52xcode.cn/Article/details/gt3tgfgdyev.html

el.addEventListener("click", e => {})
来源：http://www.52xcode.cn/Article/details/gt3ofzhbhwu.html

[U100] JS：DOM 查询
来源：http://www.ydjk.org.cn/Article/details/gt3qeaufkau.html

document.querySelector(".item")
来源：http://www.52xcode.cn/Article/details/gt3kdtlxluv.html

[U101] JS：classList 操作
来源：http://www.52xcode.cn/Article/details/gt3vbprhjxb.html

el.classList.toggle("active")
来源：http://www.52xcode.cn/Article/details/gt3zfsyweli.html

[U102] JS：本地存储
来源：http://www.52xcode.cn/Article/details/gt3paijvbnf.html

localStorage.setItem("k", JSON.stringify(v))
来源：http://www.52xcode.cn/Article/details/gt3uzkhgjfl.html

[U103] JS：定时器
来源：http://www.ydjk.org.cn/Article/details/gt3ecfahwjf.html

setTimeout(fn, 1000);  setInterval(fn, 1000);
来源：http://www.ydjk.org.cn/Article/details/gt3skpracig.html

[U104] JS：防抖
来源：http://www.52xcode.cn/Article/details/gt3yftavlwd.html

const debounce = (fn, ms) => { let t; return (...a) => { clearTimeout(t); t = setTimeout(() => fn(...a), ms); }; };
来源：http://www.ydjk.org.cn/Article/details/gt3mlzvadsj.html

[U105] JS：节流
来源：http://www.ydjk.org.cn/Article/details/gt3dvlywtej.html

const throttle = (fn, ms) => { let last = 0; return (...a) => { const n = Date.now(); if (n - last >= ms) { last = n; fn(...a); } }; };
来源：http://www.ydjk.org.cn/Article/details/gt3jmvcelzs.html

[U106] JS：日期格式化
来源：http://www.52xcode.cn/Article/details/gt3jdnqykiw.html

new Intl.DateTimeFormat("zh-CN", { dateStyle: "medium" }).format(new Date())
来源：http://www.ydjk.org.cn/Article/details/gt3smunnhxh.html

[U107] JS：数字千分位
来源：http://www.ydjk.org.cn/Article/details/gt3nyxbyeue.html

new Intl.NumberFormat("en-US").format(1234567)
来源：http://www.52xcode.cn/Article/details/gt3enniastc.html

[U108] JS：随机整数
来源：http://www.ydjk.org.cn/Article/details/gt3jvulfviz.html

Math.floor(Math.random() * (max - min + 1)) + min
来源：http://www.52xcode.cn/Article/details/gt3mljeozpg.html

[U109] JS：数组分组
来源：http://www.ydjk.org.cn/Article/details/gt3tdtbiciw.html

Object.groupBy(arr, x => x.type)
来源：http://www.52xcode.cn/Article/details/gt3faexhcfb.html

[U110] JS：数组分块
来源：http://www.ydjk.org.cn/Article/details/gt3rwzorsxn.html

arr.reduce((acc, x, i) => (i % size ? acc : [...acc, arr.slice(i, i + size)]), [])
来源：http://www.ydjk.org.cn/Article/details/gt3zixkkqpu.html

[U111] JS：对象转 Map
来源：http://www.52xcode.cn/Article/details/gt3jhmkvdsc.html

new Map(Object.entries(obj))
来源：http://www.52xcode.cn/Article/details/gt3ycmpclxt.html

[U112] JS：字符串补位
来源：http://www.ydjk.org.cn/Article/details/gt3divrfudq.html

"7".padStart(3, "0")
来源：http://www.ydjk.org.cn/Article/details/gt3ammoajtk.html

[U113] JS：正则替换全部
来源：http://www.ydjk.org.cn/Article/details/gt3zpmwubxp.html

s.replaceAll("a", "b")
来源：http://www.52xcode.cn/Article/details/gt3mxdvezcw.html

[U114] JS：JSON 深比较
来源：http://www.52xcode.cn/Article/details/gt3puutldki.html

JSON.stringify(a) === JSON.stringify(b)
来源：http://www.52xcode.cn/Article/details/gt3wnqwrhtz.html

[U115] JS：生成 UUID
来源：http://www.ydjk.org.cn/Article/details/gt3bcswovnh.html

crypto.randomUUID()
来源：http://www.52xcode.cn/Article/details/gt3nnmvkenr.html

[U116] JS：类型检查（JSDoc）
来源：http://www.ydjk.org.cn/Article/details/gt3hkrhdzma.html

/** @param {string} name */ function f(name) {}
来源：http://www.52xcode.cn/Article/details/gt3uyteqcru.html

[U117] JS：单元测试
来源：http://www.52xcode.cn/Article/details/gt3ahnmkero.html

npm i -D vitest;  npx vitest
来源：http://www.ydjk.org.cn/Article/details/gt3lplchufb.html

[U118] JS：开发服务器
来源：http://www.ydjk.org.cn/Article/details/gt3vqfuozju.html

npm i -D vite;  npx vite
来源：http://www.ydjk.org.cn/Article/details/gt3jxlwghqp.html

[U119] JS：生产构建
来源：http://www.ydjk.org.cn/Article/details/gt3dzdypbss.html

npx vite build
来源：http://www.52xcode.cn/Article/details/gt3rcwcebsk.html

[U120] JS：读取环境变量（Vite）
来源：http://www.ydjk.org.cn/Article/details/gt3rbrlkigq.html

import.meta.env.VITE_API_URL
来源：http://www.ydjk.org.cn/Article/details/gt3pnsxkldf.html

================================================================================
来源：http://www.52xcode.cn/Article/details/gt3qqgtqyos.html

统计汇总
来源：http://www.ydjk.org.cn/Article/details/gt3qzkzkmae.html

================================================================================
来源：http://www.ydjk.org.cn/Article/details/gt3grqbbbhx.html

按语言统计（条）：
来源：http://www.ydjk.org.cn/Article/details/gt3yteznyfg.html

Python ......... 252
来源：http://www.ydjk.org.cn/Article/details/gt3iwhjoxxk.html

PHP ............ 252
来源：http://www.52xcode.cn/Article/details/gt3xduntjev.html

JavaScript ..... 252
来源：http://www.52xcode.cn/Article/details/gt3dpgxzych.html

TypeScript ..... 212
来源：http://www.52xcode.cn/Article/details/gt3ntcgwart.html

Java ........... 212
来源：http://www.52xcode.cn/Article/details/gt3ikuqcquv.html

Go ............. 212
来源：http://www.52xcode.cn/Article/details/gt3dakvwggl.html

Ruby ........... 212
来源：http://www.52xcode.cn/Article/details/gt3lyyntdon.html

C# ............. 212
来源：http://www.ydjk.org.cn/Article/details/gt3qhpxsnxe.html

C .............. 30
来源：http://www.52xcode.cn/Article/details/gt3pjzmhmwm.html

C++ ............ 30
来源：http://www.52xcode.cn/Article/details/gt3omwknfyq.html

SQL ............ 90
来源：http://www.ydjk.org.cn/Article/details/gt3dtmmdojg.html

Bash ........... 80
来源：http://www.ydjk.org.cn/Article/details/gt3lacvgglx.html

Kotlin ......... 15
来源：http://www.52xcode.cn/Article/details/gt3pmrjhnln.html

Swift .......... 15
来源：http://www.52xcode.cn/Article/details/gt3phafelen.html

Lua ............ 10
来源：http://www.52xcode.cn/Article/details/gt3bwavvsvx.html

Perl ........... 10
来源：http://www.ydjk.org.cn/Article/details/gt3vqhonrww.html

Scala .......... 10
来源：http://www.ydjk.org.cn/Article/details/gt3uwxmprxr.html

------------------------------------
来源：http://www.52xcode.cn/Article/details/gt3lkrvmyxl.html

合计 ........... 2106 条
来源：http://www.52xcode.cn/Article/details/gt3ffexmiyq.html

按章节统计：
来源：http://www.ydjk.org.cn/Article/details/gt3cwsgwuzt.html

A 基础语法与类型       26 个任务 × 8 语言 =  208
来源：http://www.ydjk.org.cn/Article/details/gt3wjuyfygt.html

B 流程控制             16 个任务 × 8 语言 =  128
来源：http://www.52xcode.cn/Article/details/gt3fpjzgvta.html

C 函数与作用域         16 个任务 × 8 语言 =  128
来源：http://www.ydjk.org.cn/Article/details/gt3elgpkbvd.html

D 数组 / 列表 / 集合   26 个任务 × 8 语言 =  208
来源：http://www.52xcode.cn/Article/details/gt3narmrevl.html

E 字符串处理           22 个任务 × 8 语言 =  176
来源：http://www.52xcode.cn/Article/details/gt3rgjcaowq.html

F 文件与目录           12 个任务 × 8 语言 =   96
来源：http://www.52xcode.cn/Article/details/gt3ueplbexs.html

G 面向对象             16 个任务 × 8 语言 =  128
来源：http://www.ydjk.org.cn/Article/details/gt3hzkqlymf.html

H 异常与错误处理       10 个任务 × 8 语言 =   80
来源：http://www.52xcode.cn/Article/details/gt3hbmzaejq.html

I 正则表达式            8 个任务 × 8 语言 =   64
来源：http://www.52xcode.cn/Article/details/gt3agpjbsts.html

J 日期与时间           10 个任务 × 8 语言 =   80
来源：http://www.52xcode.cn/Article/details/gt3rdajhyzk.html

K JSON 与序列化         8 个任务 × 8 语言 =   64
来源：http://www.52xcode.cn/Article/details/gt3buzdgail.html

L 网络请求              8 个任务 × 8 语言 =   64
来源：http://www.ydjk.org.cn/Article/details/gt3ougrrihf.html

M 命令行 / 进程         8 个任务 × 8 语言 =   64
来源：http://www.52xcode.cn/Article/details/gt3dewcdqgt.html

N 数据结构与算法       12 个任务 × 8 语言 =   96
来源：http://www.52xcode.cn/Article/details/gt3dlfacvkk.html

O 并发与异步            6 个任务 × 8 语言 =   48
来源：http://www.52xcode.cn/Article/details/gt3cpwpgtpf.html

P 常用工具函数          8 个任务 × 8 语言 =   64
来源：http://www.ydjk.org.cn/Article/details/gt3xqneaqbw.html

Q SQL 专题                              90
来源：http://www.ydjk.org.cn/Article/details/gt3wtajoccu.html

R Bash 专题                             80
来源：http://www.ydjk.org.cn/Article/details/gt3qbdmdqtu.html

S C / C++ 专题                          60
来源：http://www.ydjk.org.cn/Article/details/gt3fvvvgumf.html

T 其他语言补充                          60
来源：http://www.52xcode.cn/Article/details/gt3lcmrjgdu.html

U 高频实用片段                         120
来源：http://www.52xcode.cn/Article/details/gt3bmiwkprs.html

------------------------------------
来源：http://www.52xcode.cn/Article/details/gt3mdrpizky.html

合计                                  2106 条
来源：http://www.ydjk.org.cn/Article/details/gt3fgofvjsw.html

--------------------------------------------------------------------------------
来源：http://www.ydjk.org.cn/Article/details/gt3ozixkolq.html

使用提醒
来源：http://www.ydjk.org.cn/Article/details/gt3ndvpooxu.html

--------------------------------------------------------------------------------
来源：http://www.ydjk.org.cn/Article/details/gt3bmmqjbhk.html

1. 示例追求"最小可用"，正式项目中请补齐导入、错误处理与边界判断。
来源：http://www.ydjk.org.cn/Article/details/gt3xpkvhsrf.html

2. 涉及文件、网络、数据库的示例，注意资源释放与异常捕获。
来源：http://www.52xcode.cn/Article/details/gt3rzsbsiva.html

3. 语言版本差异较大（如 Python 3.10 的 match、Java 17 的 record/switch 箭头），
来源：http://www.ydjk.org.cn/Article/details/gt3cqozguif.html

在旧版本上使用前请先确认语法支持情况。
来源：http://www.52xcode.cn/Article/details/gt3dcubxobw.html

4. 标注"手写"的条目是因为该语言缺少对应内置能力，实际项目中可引入成熟库。
来源：http://www.ydjk.org.cn/Article/details/gt3jsobaqgh.html

—— 文件结束 ——
来源：http://www.52xcode.cn/Article/details/gt3jeeszmzt.html

================================================================================
来源：http://www.ydjk.org.cn/Article/details/gt3nasmwfek.html

程序语言常见例子速查手册（2024 版）
来源：http://www.52xcode.cn/Article/details/gt3tonipmvt.html

Common Programming Examples Cheat Book
来源：http://www.ydjk.org.cn/Article/details/gt3rpdazvus.html

================================================================================
来源：http://www.52xcode.cn/Article/details/gt3fqxpknbv.html

【收录内容】
来源：http://www.52xcode.cn/Article/details/gt3tpdjzelv.html

覆盖 12 种语言 / 语法与常见 API：
来源：http://www.52xcode.cn/Article/details/gt3rklzpsxz.html

Python · PHP · JavaScript · TypeScript · Java · Go · Ruby · C#
来源：http://www.ydjk.org.cn/Article/details/gt3zkfzvhvk.html

SQL · Bash · C · C++
来源：http://www.ydjk.org.cn/Article/details/gt3azucdtmx.html

按「任务」分组：每个任务下按语言各给出一条最小可用示例。
来源：http://www.ydjk.org.cn/Article/details/gt3vjicmslu.html

【使用说明】
来源：http://www.52xcode.cn/Article/details/gt3fivgphws.html

1. 每个任务形如 "[编号] 任务名"，下面每行以语言标记开头：
来源：http://www.ydjk.org.cn/Article/details/gt3ysglbixf.html

Py:    Python        PHP:   PHP           JS:    JavaScript
来源：http://www.ydjk.org.cn/Article/details/gt3dpvfhpea.html

TS:    TypeScript    Java:  Java          Go:    Go
来源：http://www.ydjk.org.cn/Article/details/gt3nahvuztm.html

Ruby:  Ruby          C#:    C#            SQL:   SQL
来源：http://www.ydjk.org.cn/Article/details/gt3wxdzjnde.html

Bash:  Shell         C:     C             C++:   C++
来源：http://www.ydjk.org.cn/Article/details/gt3kqhtzevi.html

2. 示例只展示核心写法，刻意省略 import / require / include / using 等样板代码。
来源：http://www.ydjk.org.cn/Article/details/gt3ytgiiqjr.html

需要完整可运行文件时，请自行补齐当前语言的导入语句。
来源：http://www.ydjk.org.cn/Article/details/gt3wgzlxrez.html

3. 语法基准：Python 3.10+ / PHP 8.1+ / ES2020+ / TypeScript 5 / Java 17 /
来源：http://www.ydjk.org.cn/Article/details/gt3knvpwyoc.html

Go 1.21+ / Ruby 3.x / C# 10+ / C17 / C++17。
来源：http://www.52xcode.cn/Article/details/gt3grjsteit.html

4. 检索建议：用编辑器或浏览器 Ctrl+F 搜关键词，如 "排序" "读取文件" "正则"。
来源：http://www.52xcode.cn/Article/details/gt3nevmghwz.html

5. 标记为 "// 无" 表示该语言没有对应的一等语法，需用替代写法（示例给出替代方案）。
来源：http://www.ydjk.org.cn/Article/details/gt3xppbacxk.html

6. 符号 "⏎" 表示代码在此处换行（主要用于 Python 等强制缩进、无法压成一行的结构）。
来源：http://www.52xcode.cn/Article/details/gt3uixyvgdm.html

【文件统计】
来源：http://www.ydjk.org.cn/Article/details/gt3vnwkxjqv.html

语言示例共 2106 条，分布见本文末尾的「统计汇总」。
来源：http://www.52xcode.cn/Article/details/gt3mhtrlqas.html

--------------------------------------------------------------------------------
来源：http://www.52xcode.cn/Article/details/gt3btbrvxjm.html

目  录
来源：http://www.ydjk.org.cn/Article/details/gt3qdnoyprp.html

--------------------------------------------------------------------------------
来源：http://www.52xcode.cn/Article/details/gt3vpswxtzv.html

A. 基础语法与类型              （第 1 节，26 个任务，208 条）
来源：http://www.ydjk.org.cn/Article/details/gt3dcddmilb.html

B. 流程控制                    （第 2 节，16 个任务，128 条）
来源：http://www.ydjk.org.cn/Article/details/gt3umfvudow.html

C. 函数与作用域                （第 3 节，16 个任务，128 条）
来源：http://www.52xcode.cn/Article/details/gt3qtbarndl.html

D. 数组 / 列表 / 集合          （第 4 节，26 个任务，208 条）
来源：http://www.52xcode.cn/Article/details/gt3plyhlqop.html

E. 字符串处理                  （第 5 节，22 个任务，176 条）
来源：http://www.52xcode.cn/Article/details/gt3cwpnqxyh.html

F. 文件与目录                  （第 6 节，12 个任务，96 条）
来源：http://www.ydjk.org.cn/Article/details/gt3avhpbjgk.html

G. 面向对象                    （第 7 节，16 个任务，128 条）
来源：http://www.52xcode.cn/Article/details/gt3khbqofbl.html

H. 异常与错误处理              （第 8 节，10 个任务，80 条）
来源：http://www.52xcode.cn/Article/details/gt3tcmttirj.html

I. 正则表达式                  （第 9 节，8 个任务，64 条）
来源：http://www.52xcode.cn/Article/details/gt3bwsciwwk.html


<!-- 参考信息 -->