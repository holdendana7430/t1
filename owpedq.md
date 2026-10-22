代发 wailian999

[U13] Py：固定长度队列
来源：http://www.52xcode.cn/Article/details/gt2alnfsnfl.html

deque(maxlen=10)
来源：http://www.ydjk.org.cn/Article/details/gt2sqgaskph.html

[U14] Py：分组收集到列表
来源：http://www.52xcode.cn/Article/details/gt2rtoxgugw.html

defaultdict(list)
来源：http://www.52xcode.cn/Article/details/gt2kwqqaltv.html

[U15] Py：高精度计时
来源：http://www.52xcode.cn/Article/details/gt2oxsvgwcl.html

t = time.perf_counter()
来源：http://www.ydjk.org.cn/Article/details/gt2rralisrk.html

[U16] Py：命令行参数解析
来源：http://www.ydjk.org.cn/Article/details/gt2vgkkdeak.html

ap = argparse.ArgumentParser();  ap.add_argument("--name");  args = ap.parse_args()
来源：http://www.ydjk.org.cn/Article/details/gt2fcfmnfqf.html

[U17] Py：初始化日志
来源：http://www.ydjk.org.cn/Article/details/gt2szoqbumy.html

logging.basicConfig(level=logging.INFO)
来源：http://www.ydjk.org.cn/Article/details/gt2zqwshpyn.html

[U18] Py：预编译正则
来源：http://www.52xcode.cn/Article/details/gt2xwjdmqct.html

pat = re.compile(r"\d+")
来源：http://www.52xcode.cn/Article/details/gt2itztugwk.html

[U19] Py：正则替换带回调
来源：http://www.52xcode.cn/Article/details/gt2nwqamkke.html

re.sub(r"\d+", lambda m: str(int(m.group()) * 2), s)
来源：http://www.ydjk.org.cn/Article/details/gt2cxjdvmpe.html

[U20] Py：缓存函数结果
来源：http://www.ydjk.org.cn/Article/details/gt2mwtqwakk.html

@functools.lru_cache(maxsize=None)
来源：http://www.ydjk.org.cn/Article/details/gt2fmkjufkn.html

[U21] Py：自定义上下文管理器
来源：http://www.52xcode.cn/Article/details/gt2wrevuexn.html

@contextlib.contextmanager
来源：http://www.52xcode.cn/Article/details/gt2drcccpqh.html

[U22] Py：矩阵转置
来源：http://www.52xcode.cn/Article/details/gt2ztfxtvbr.html

list(zip(*m))
来源：http://www.52xcode.cn/Article/details/gt2jrmxokgq.html

[U23] Py：分块读取大文件
来源：http://www.52xcode.cn/Article/details/gt2iszidxgo.html

for chunk in iter(lambda: f.read(8192), b""):
来源：http://www.52xcode.cn/Article/details/gt2hgpvsrsj.html

[U24] Py：路径操作
来源：http://www.ydjk.org.cn/Article/details/gt2uvaxqnje.html

Path("a/b.txt").parent.mkdir(parents=True, exist_ok=True)
来源：http://www.ydjk.org.cn/Article/details/gt2gwfcklws.html

[U25] Py：CSV 按字典读
来源：http://www.52xcode.cn/Article/details/gt2cmngukga.html

csv.DictReader(f)
来源：http://www.ydjk.org.cn/Article/details/gt2vuvkmuek.html

[U26] Py：并发下载
来源：http://www.52xcode.cn/Article/details/gt2qvkcbipd.html

ThreadPoolExecutor(max_workers=8).map(fetch, urls)
来源：http://www.ydjk.org.cn/Article/details/gt2klephggz.html

[U27] Py：异步 HTTP
来源：http://www.ydjk.org.cn/Article/details/gt2wjesqrpg.html

aiohttp.ClientSession() 配合 async with
来源：http://www.ydjk.org.cn/Article/details/gt2bucqtmuz.html

[U28] Py：类型别名
来源：http://www.ydjk.org.cn/Article/details/gt2bfhwenwc.html

UserId = int
来源：http://www.ydjk.org.cn/Article/details/gt2kpbvxuar.html

[U29] Py：属性校验
来源：http://www.ydjk.org.cn/Article/details/gt2ceflejos.html

@property 与 @x.setter 配合
来源：http://www.52xcode.cn/Article/details/gt2duocpjjm.html

[U30] Py：数据类
来源：http://www.52xcode.cn/Article/details/gt2zuqlqhqz.html

@dataclass(slots=True)
来源：http://www.52xcode.cn/Article/details/gt2lfswnyia.html

[U31] Py：单测
来源：http://www.52xcode.cn/Article/details/gt2ummqocuu.html

python -m pytest -q
来源：http://www.ydjk.org.cn/Article/details/gt2orbokrlt.html

[U32] Py：代码格式化
来源：http://www.52xcode.cn/Article/details/gt2xxpqxbif.html

ruff format . && ruff check --fix .
来源：http://www.ydjk.org.cn/Article/details/gt2alwqtbuc.html

[U33] Py：打包发布
来源：http://www.52xcode.cn/Article/details/gt2ytpgaxmt.html

python -m build  （依赖 pyproject.toml）
来源：http://www.52xcode.cn/Article/details/gt2edowbwiv.html

[U34] Py：判断编码
来源：http://www.ydjk.org.cn/Article/details/gt2sengociv.html

chardet.detect(raw)
来源：http://www.52xcode.cn/Article/details/gt2rzvfphdq.html

[U35] Py：发送邮件
来源：http://www.52xcode.cn/Article/details/gt2wrjoixcf.html

smtplib.SMTP_SSL(...).send_message(msg)
来源：http://www.52xcode.cn/Article/details/gt2zglcxfjs.html

[U36] Py：定时任务
来源：http://www.52xcode.cn/Article/details/gt2ldkjnxwi.html

schedule.every(10).minutes.do(job)
来源：http://www.52xcode.cn/Article/details/gt2sxgjyyef.html

[U37] Py：读写 Excel
来源：http://www.52xcode.cn/Article/details/gt2ghvcsfbf.html

pandas.read_excel / DataFrame.to_excel
来源：http://www.ydjk.org.cn/Article/details/gt2vhvhflnh.html

[U38] Py：获取脚本所在目录
来源：http://www.ydjk.org.cn/Article/details/gt2wgxraayr.html

Path(__file__).resolve().parent
来源：http://www.52xcode.cn/Article/details/gt2yexpqypg.html

[U39] Py：判断是否在交互环境
来源：http://www.ydjk.org.cn/Article/details/gt2ltxigvro.html

sys.stdout.isatty()
来源：http://www.ydjk.org.cn/Article/details/gt2xrjhyxxc.html

[U40] Py：打印到标准错误
来源：http://www.ydjk.org.cn/Article/details/gt2ngpmjyhz.html

print("err", file=sys.stderr)
来源：http://www.52xcode.cn/Article/details/gt2lguebjqa.html

[U41] PHP：初始化 Composer 项目
来源：http://www.52xcode.cn/Article/details/gt2dioktkvx.html

composer init;  composer require guzzlehttp/guzzle
来源：http://www.ydjk.org.cn/Article/details/gt2dsvarifb.html

[U42] PHP：PSR-4 自动加载
来源：http://www.ydjk.org.cn/Article/details/gt2pslmzemv.html

"autoload": { "psr-4": { "App\\": "src/" } }
来源：http://www.52xcode.cn/Article/details/gt2gyazlzvp.html

[U43] PHP：声明命名空间
来源：http://www.ydjk.org.cn/Article/details/gt2vuuhnvnh.html

namespace App\Http;
来源：http://www.ydjk.org.cn/Article/details/gt2jcintvhs.html

[U44] PHP：开启严格类型
来源：http://www.ydjk.org.cn/Article/details/gt2zqhfcgln.html

declare(strict_types=1);
来源：http://www.ydjk.org.cn/Article/details/gt2ymchrhfv.html

[U45] PHP：类型声明与返回类型
来源：http://www.ydjk.org.cn/Article/details/gt2avgakeef.html

function add(int $a, int $b): int { return $a + $b; }
来源：http://www.52xcode.cn/Article/details/gt2kvjuzaxu.html

[U46] PHP：可空类型
来源：http://www.52xcode.cn/Article/details/gt2dxkkhsvn.html

?string $name = null
来源：http://www.ydjk.org.cn/Article/details/gt2gyfzarxq.html

[U47] PHP：联合类型
来源：http://www.ydjk.org.cn/Article/details/gt2dcnbtpim.html

int|string $id
来源：http://www.52xcode.cn/Article/details/gt2mxedziir.html

[U48] PHP：纯枚举
来源：http://www.ydjk.org.cn/Article/details/gt2afwpsfdt.html

enum Status: string { case Active = "active"; case Off = "off"; }
来源：http://www.ydjk.org.cn/Article/details/gt2zkamxkbo.html

[U49] PHP：只读属性
来源：http://www.52xcode.cn/Article/details/gt2qegxvpno.html

public readonly string $name
来源：http://www.52xcode.cn/Article/details/gt2kksquwis.html

[U50] PHP：构造器属性提升
来源：http://www.52xcode.cn/Article/details/gt2wmjlgqsl.html

public function __construct(private int $id) {}
来源：http://www.52xcode.cn/Article/details/gt2rvvgdhyl.html

[U51] PHP：数组解构
来源：http://www.ydjk.org.cn/Article/details/gt2nkkaghbx.html

[$a, $b] = $arr;
来源：http://www.ydjk.org.cn/Article/details/gt2livjiytz.html

[U52] PHP：箭头函数
来源：http://www.52xcode.cn/Article/details/gt2szxxfdbr.html

$double = fn($x) => $x * 2;
来源：http://www.52xcode.cn/Article/details/gt2dfqoizzj.html

[U53] PHP：空合并运算符
来源：http://www.52xcode.cn/Article/details/gt2mookgsus.html

$v = $a ?? $b ?? "default";
来源：http://www.ydjk.org.cn/Article/details/gt2dztxwtav.html

[U54] PHP：空安全调用
来源：http://www.52xcode.cn/Article/details/gt2iewlmeky.html

$obj?->method()
来源：http://www.ydjk.org.cn/Article/details/gt2bosadruq.html

[U55] PHP：match 表达式
来源：http://www.ydjk.org.cn/Article/details/gt2yuqofrjm.html

$s = match($x) { 1 => "一", default => "其他" };
来源：http://www.ydjk.org.cn/Article/details/gt2zpmfvmgx.html

[U56] PHP：命名参数
来源：http://www.ydjk.org.cn/Article/details/gt2pgmosyrl.html

f(a: 1, b: 2)
来源：http://www.52xcode.cn/Article/details/gt2qahkotub.html

[U57] PHP：字符串插值
来源：http://www.ydjk.org.cn/Article/details/gt2odpkneom.html

"值: {$a}"
来源：http://www.ydjk.org.cn/Article/details/gt2jdwdenpj.html

[U58] PHP：数组三件套
来源：http://www.ydjk.org.cn/Article/details/gt2xwjgouou.html

array_map($f, $a);  array_filter($a, $f);  array_reduce($a, $f, 0);
来源：http://www.52xcode.cn/Article/details/gt2caxhcuqe.html

[U59] PHP：自定义排序
来源：http://www.ydjk.org.cn/Article/details/gt2ogpcvooe.html

usort($arr, fn($a, $b) => $a["age"] <=> $b["age"]);
来源：http://www.52xcode.cn/Article/details/gt2tpmaactr.html

[U60] PHP：JSON 编解码
来源：http://www.ydjk.org.cn/Article/details/gt2lezvyxew.html

json_encode($d, JSON_UNESCAPED_UNICODE);  json_decode($s, true);
来源：http://www.ydjk.org.cn/Article/details/gt2nvqnmeuw.html

[U61] PHP：正则
来源：http://www.ydjk.org.cn/Article/details/gt2dftwvtzy.html

preg_match('/(\d+)/', $s, $m);  preg_replace('/\d+/', '#', $s);
来源：http://www.52xcode.cn/Article/details/gt2jaekyhej.html

[U62] PHP：日期对象
来源：http://www.52xcode.cn/Article/details/gt2yxbxmwza.html

(new DateTimeImmutable())->format("Y-m-d");
来源：http://www.52xcode.cn/Article/details/gt2wdycqrkp.html

[U63] PHP：文件读写
来源：http://www.52xcode.cn/Article/details/gt2rnoslrgc.html

file_get_contents($f);  file_put_contents($f, $data);
来源：http://www.ydjk.org.cn/Article/details/gt2sdxhruli.html

[U64] PHP：目录遍历
来源：http://www.ydjk.org.cn/Article/details/gt2kktjvvdd.html

glob("dir/*.php");  scandir("dir");
来源：http://www.ydjk.org.cn/Article/details/gt2nnggpbmr.html

[U65] PHP：会话
来源：http://www.ydjk.org.cn/Article/details/gt2tfpzitok.html

session_start();  $_SESSION["uid"] = 1;
来源：http://www.ydjk.org.cn/Article/details/gt2jbnloxdq.html

[U66] PHP：设置 Cookie
来源：http://www.ydjk.org.cn/Article/details/gt2rjhjuafx.html

setcookie("token", $v, ["httponly" => true, "samesite" => "Lax"]);
来源：http://www.52xcode.cn/Article/details/gt2zjkzbvnd.html

[U67] PHP：处理文件上传
来源：http://www.52xcode.cn/Article/details/gt2zzguzams.html

$_FILES["file"]["tmp_name"] 与 move_uploaded_file()
来源：http://www.ydjk.org.cn/Article/details/gt2eudteeit.html

[U68] PHP：PDO 连接
来源：http://www.ydjk.org.cn/Article/details/gt2doasrfqk.html

$pdo = new PDO("mysql:host=localhost;dbname=app", "root", "");
来源：http://www.ydjk.org.cn/Article/details/gt2kfbgzkpb.html

[U69] PHP：PDO 预处理
来源：http://www.52xcode.cn/Article/details/gt2bhwaolbp.html

$stmt = $pdo->prepare("SELECT * FROM users WHERE id = ?");  $stmt->execute([$id]);
来源：http://www.52xcode.cn/Article/details/gt2xuchhuuz.html

[U70] PHP：PDO 事务
来源：http://www.ydjk.org.cn/Article/details/gt2rcedekbs.html

$pdo->beginTransaction();  $pdo->commit();  $pdo->rollBack();
来源：http://www.52xcode.cn/Article/details/gt2coigyolk.html

[U71] PHP：抛出异常
来源：http://www.52xcode.cn/Article/details/gt2kbiyahei.html

throw new RuntimeException("失败", 500);
来源：http://www.52xcode.cn/Article/details/gt2gnwevjao.html

[U72] PHP：写错误日志
来源：http://www.52xcode.cn/Article/details/gt2dkoulqmq.html

error_log("失败: " . $e->getMessage());
来源：http://www.ydjk.org.cn/Article/details/gt2oabjxoaw.html

[U73] PHP：读取 ini 配置
来源：http://www.52xcode.cn/Article/details/gt2iwxumuqy.html

parse_ini_file("config.ini", true)
来源：http://www.ydjk.org.cn/Article/details/gt2awadbate.html

[U74] PHP：读取环境变量
来源：http://www.ydjk.org.cn/Article/details/gt2tcfonwpy.html

getenv("APP_ENV") ?: "production"
来源：http://www.ydjk.org.cn/Article/details/gt2diztbvbt.html

[U75] PHP：依赖注入
来源：http://www.52xcode.cn/Article/details/gt2chwfamnj.html

composer require psr/container
来源：http://www.52xcode.cn/Article/details/gt2tigzmkbv.html

[U76] PHP：简单路由
来源：http://www.52xcode.cn/Article/details/gt2zacckddc.html

$path = parse_url($_SERVER["REQUEST_URI"], PHP_URL_PATH);
来源：http://www.ydjk.org.cn/Article/details/gt2lqtqmcoq.html

[U77] PHP：模板渲染
来源：http://www.ydjk.org.cn/Article/details/gt2rikheqmf.html

composer require twig/twig
来源：http://www.ydjk.org.cn/Article/details/gt2sxjbrosy.html

[U78] PHP：单元测试
来源：http://www.52xcode.cn/Article/details/gt2suqoqzzv.html

composer require --dev phpunit/phpunit
来源：http://www.52xcode.cn/Article/details/gt2zzggoksy.html

[U79] PHP：静态分析
来源：http://www.ydjk.org.cn/Article/details/gt2jtxakhae.html

composer require --dev phpstan/phpstan
来源：http://www.52xcode.cn/Article/details/gt2xzocwgwy.html

[U80] PHP：代码规范修复
来源：http://www.ydjk.org.cn/Article/details/gt2wpsbblvz.html

composer require --dev friendsofphp/php-cs-fixer
来源：http://www.52xcode.cn/Article/details/gt2lwokkocb.html

[U81] JS：初始化项目
来源：http://www.52xcode.cn/Article/details/gt2fdjggyow.html

npm init -y;  npm i express
来源：http://www.52xcode.cn/Article/details/gt2whnkjmdk.html

[U82] JS：package.json 脚本
来源：http://www.ydjk.org.cn/Article/details/gt2ebdfmeva.html

"scripts": { "dev": "vite", "build": "vite build" }
来源：http://www.52xcode.cn/Article/details/gt2unxcdoss.html

[U83] JS：ES Module 导入导出
来源：http://www.52xcode.cn/Article/details/gt2xmyfotvr.html

export const a = 1;  import { a } from "./m.js";
来源：http://www.52xcode.cn/Article/details/gt2gitxrgyo.html

[U84] JS：CommonJS 写法
来源：http://www.ydjk.org.cn/Article/details/gt2wyrhwqev.html

module.exports = { a };  const { a } = require("./m");
来源：http://www.52xcode.cn/Article/details/gt2fefwwyne.html

[U85] JS：可选链
来源：http://www.ydjk.org.cn/Article/details/gt2urwurhzq.html

a?.b?.c
来源：http://www.ydjk.org.cn/Article/details/gt2yibvmgdf.html

[U86] JS：空值合并
来源：http://www.52xcode.cn/Article/details/gt2qkvussjp.html

a ?? b
来源：http://www.ydjk.org.cn/Article/details/gt2nbgkajin.html

[U87] JS：解构默认值
来源：http://www.52xcode.cn/Article/details/gt2tvjvisdt.html

const { a = 1, b = 2 } = obj;
来源：http://www.ydjk.org.cn/Article/details/gt2fnstexxk.html

[U88] JS：对象展开合并
来源：http://www.52xcode.cn/Article/details/gt2lhfigwyd.html

{ ...a, ...b }
来源：http://www.ydjk.org.cn/Article/details/gt2viefxlks.html

[U89] JS：数组去重
来源：http://www.52xcode.cn/Article/details/gt2hytygiez.html

[...new Set(arr)]
来源：http://www.ydjk.org.cn/Article/details/gt2xblolnpu.html

[U90] JS：数字数组排序
来源：http://www.ydjk.org.cn/Article/details/gt2wsjxxfoj.html

[...arr].sort((a, b) => a - b)
来源：http://www.52xcode.cn/Article/details/gt2jxvvwhsl.html

[U91] JS：对象键值遍历
来源：http://www.52xcode.cn/Article/details/gt2joevdfzt.html

Object.entries(obj).forEach(([k, v]) => {});
来源：http://www.52xcode.cn/Article/details/gt2rpjbemzg.html

[U92] JS：深拷贝
来源：http://www.52xcode.cn/Article/details/gt2qsavwonh.html

structuredClone(obj)
来源：http://www.52xcode.cn/Article/details/gt2ycahjhll.html

[U93] JS：模板字符串
来源：http://www.ydjk.org.cn/Article/details/gt2wriclzja.html

`共 ${n} 条`
来源：http://www.52xcode.cn/Article/details/gt2soympwba.html

[U94] JS：箭头函数
来源：http://www.52xcode.cn/Article/details/gt2vbhuaygm.html

const double = x => x * 2;
来源：http://www.ydjk.org.cn/Article/details/gt2zfpsnihz.html

[U95] JS：Promise 包装
来源：http://www.ydjk.org.cn/Article/details/gt2enpqkazd.html

new Promise((resolve, reject) => {})
来源：http://www.ydjk.org.cn/Article/details/gt2kuajiqwf.html

[U96] JS：async/await 与异常
来源：http://www.ydjk.org.cn/Article/details/gt2sdganoec.html

try { const d = await f(); } catch (e) { console.error(e); }
来源：http://www.ydjk.org.cn/Article/details/gt2kslyztdw.html

[U97] JS：并发请求
来源：http://www.52xcode.cn/Article/details/gt2bcsatayf.html

await Promise.all(urls.map(u => fetch(u)))
来源：http://www.52xcode.cn/Article/details/gt2wguhhztz.html

[U98] JS：fetch 带 JSON
来源：http://www.52xcode.cn/Article/details/gt2jyxvvije.html

await fetch(url, { method: "POST", headers: { "Content-Type": "application/json" }, body: JSON.stringify(d) })
来源：http://www.52xcode.cn/Article/details/gt2nmpqoeym.html

[U99] JS：事件监听
来源：http://www.ydjk.org.cn/Article/details/gt2pjcncxdr.html

el.addEventListener("click", e => {})
来源：http://www.52xcode.cn/Article/details/gt2wsstniqd.html

[U100] JS：DOM 查询
来源：http://www.ydjk.org.cn/Article/details/gt2krfxbnbz.html

document.querySelector(".item")
来源：http://www.ydjk.org.cn/Article/details/gt2wltcutoi.html

[U101] JS：classList 操作
来源：http://www.52xcode.cn/Article/details/gt2doxfmolz.html

el.classList.toggle("active")
来源：http://www.ydjk.org.cn/Article/details/gt2gvmejemi.html

[U102] JS：本地存储
来源：http://www.ydjk.org.cn/Article/details/gt2ntybsyug.html

localStorage.setItem("k", JSON.stringify(v))
来源：http://www.52xcode.cn/Article/details/gt2qzjajmma.html

[U103] JS：定时器
来源：http://www.52xcode.cn/Article/details/gt2qsjweaej.html

setTimeout(fn, 1000);  setInterval(fn, 1000);
来源：http://www.52xcode.cn/Article/details/gt2wptjxeka.html

[U104] JS：防抖
来源：http://www.ydjk.org.cn/Article/details/gt2lblsbcil.html

const debounce = (fn, ms) => { let t; return (...a) => { clearTimeout(t); t = setTimeout(() => fn(...a), ms); }; };
来源：http://www.52xcode.cn/Article/details/gt2bdaegeyr.html

[U105] JS：节流
来源：http://www.ydjk.org.cn/Article/details/gt2oatjbhhc.html

const throttle = (fn, ms) => { let last = 0; return (...a) => { const n = Date.now(); if (n - last >= ms) { last = n; fn(...a); } }; };
来源：http://www.ydjk.org.cn/Article/details/gt2uwoxkpcr.html

[U106] JS：日期格式化
来源：http://www.ydjk.org.cn/Article/details/gt2zegcjwuf.html

new Intl.DateTimeFormat("zh-CN", { dateStyle: "medium" }).format(new Date())
来源：http://www.52xcode.cn/Article/details/gt2jgylpdfa.html

[U107] JS：数字千分位
来源：http://www.52xcode.cn/Article/details/gt2wurwoscj.html

new Intl.NumberFormat("en-US").format(1234567)
来源：http://www.52xcode.cn/Article/details/gt2nwlwxnbz.html

[U108] JS：随机整数
来源：http://www.ydjk.org.cn/Article/details/gt2brgkjyfs.html

Math.floor(Math.random() * (max - min + 1)) + min
来源：http://www.52xcode.cn/Article/details/gt2pkjnqkpv.html

[U109] JS：数组分组
来源：http://www.ydjk.org.cn/Article/details/gt2nqhxjqwu.html

Object.groupBy(arr, x => x.type)
来源：http://www.ydjk.org.cn/Article/details/gt2shkbdmec.html

[U110] JS：数组分块
来源：http://www.ydjk.org.cn/Article/details/gt2znizlcmm.html

arr.reduce((acc, x, i) => (i % size ? acc : [...acc, arr.slice(i, i + size)]), [])
来源：http://www.ydjk.org.cn/Article/details/gt2tiktsjgt.html

[U111] JS：对象转 Map
来源：http://www.52xcode.cn/Article/details/gt2chvhoitg.html

new Map(Object.entries(obj))
来源：http://www.ydjk.org.cn/Article/details/gt2pksxrjpp.html

[U112] JS：字符串补位
来源：http://www.ydjk.org.cn/Article/details/gt2hqbmdxsw.html

"7".padStart(3, "0")
来源：http://www.52xcode.cn/Article/details/gt2whquvqxh.html

[U113] JS：正则替换全部
来源：http://www.ydjk.org.cn/Article/details/gt2jrkswskx.html

s.replaceAll("a", "b")
来源：http://www.ydjk.org.cn/Article/details/gt2czubglqn.html

[U114] JS：JSON 深比较
来源：http://www.52xcode.cn/Article/details/gt2wdlqxaii.html

JSON.stringify(a) === JSON.stringify(b)
来源：http://www.ydjk.org.cn/Article/details/gt2jsfvptlt.html

[U115] JS：生成 UUID
来源：http://www.ydjk.org.cn/Article/details/gt2nnfqvexc.html

crypto.randomUUID()
来源：http://www.52xcode.cn/Article/details/gt2wtynfwuy.html

[U116] JS：类型检查（JSDoc）
来源：http://www.ydjk.org.cn/Article/details/gt2pucrwtcd.html

/** @param {string} name */ function f(name) {}
来源：http://www.52xcode.cn/Article/details/gt2filoqswo.html

[U117] JS：单元测试
来源：http://www.52xcode.cn/Article/details/gt2ejqrzjks.html

npm i -D vitest;  npx vitest
来源：http://www.52xcode.cn/Article/details/gt2lzpgbbwo.html

[U118] JS：开发服务器
来源：http://www.52xcode.cn/Article/details/gt2tsqxjtme.html

npm i -D vite;  npx vite
来源：http://www.52xcode.cn/Article/details/gt2isrlzfuz.html

[U119] JS：生产构建
来源：http://www.ydjk.org.cn/Article/details/gt2ncpcxcmi.html

npx vite build
来源：http://www.ydjk.org.cn/Article/details/gt2njbnylhd.html

[U120] JS：读取环境变量（Vite）
来源：http://www.ydjk.org.cn/Article/details/gt2docnbaig.html

import.meta.env.VITE_API_URL
来源：http://www.52xcode.cn/Article/details/gt2vhktffee.html

================================================================================
来源：http://www.ydjk.org.cn/Article/details/gt2bslvvjxg.html

统计汇总
来源：http://www.52xcode.cn/Article/details/gt2zlsuornr.html

================================================================================
来源：http://www.52xcode.cn/Article/details/gt2lggzozaf.html

按语言统计（条）：
来源：http://www.52xcode.cn/Article/details/gt2jspzcfzm.html

Python ......... 252
来源：http://www.52xcode.cn/Article/details/gt2cjhykuiu.html

PHP ............ 252
来源：http://www.ydjk.org.cn/Article/details/gt2ujftciqd.html

JavaScript ..... 252
来源：http://www.ydjk.org.cn/Article/details/gt2vzmwcpsi.html

TypeScript ..... 212
来源：http://www.ydjk.org.cn/Article/details/gt2hrtvxvrs.html

Java ........... 212
来源：http://www.52xcode.cn/Article/details/gt2unvcaaob.html

Go ............. 212
来源：http://www.52xcode.cn/Article/details/gt2yfqfwuxj.html

Ruby ........... 212
来源：http://www.52xcode.cn/Article/details/gt2cfeljqws.html

C# ............. 212
来源：http://www.52xcode.cn/Article/details/gt2vduzhmhh.html

C .............. 30
来源：http://www.ydjk.org.cn/Article/details/gt2nlbcsfub.html

C++ ............ 30
来源：http://www.52xcode.cn/Article/details/gt2rhvjtfec.html

SQL ............ 90
来源：http://www.ydjk.org.cn/Article/details/gt2bgzyplbu.html

Bash ........... 80
来源：http://www.ydjk.org.cn/Article/details/gt2zcjamgpc.html

Kotlin ......... 15
来源：http://www.ydjk.org.cn/Article/details/gt2jktdpjxm.html

Swift .......... 15
来源：http://www.ydjk.org.cn/Article/details/gt2yqxaewue.html

Lua ............ 10
来源：http://www.52xcode.cn/Article/details/gt2zuxteuaf.html

Perl ........... 10
来源：http://www.ydjk.org.cn/Article/details/gt2zatwavus.html

Scala .......... 10
来源：http://www.ydjk.org.cn/Article/details/gt2twyuptkh.html

------------------------------------
来源：http://www.52xcode.cn/Article/details/gt2axubygpo.html

合计 ........... 2106 条
来源：http://www.ydjk.org.cn/Article/details/gt2fapqysez.html

按章节统计：
来源：http://www.52xcode.cn/Article/details/gt2twqowqko.html

A 基础语法与类型       26 个任务 × 8 语言 =  208
来源：http://www.52xcode.cn/Article/details/gt2ofwbolez.html

B 流程控制             16 个任务 × 8 语言 =  128
来源：http://www.ydjk.org.cn/Article/details/gt2aqjmtwdy.html

C 函数与作用域         16 个任务 × 8 语言 =  128
来源：http://www.ydjk.org.cn/Article/details/gt2knwiblws.html

D 数组 / 列表 / 集合   26 个任务 × 8 语言 =  208
来源：http://www.ydjk.org.cn/Article/details/gt2ayfkkvye.html

E 字符串处理           22 个任务 × 8 语言 =  176
来源：http://www.ydjk.org.cn/Article/details/gt2ibpppdia.html

F 文件与目录           12 个任务 × 8 语言 =   96
来源：http://www.ydjk.org.cn/Article/details/gt2vjzhdtao.html

G 面向对象             16 个任务 × 8 语言 =  128
来源：http://www.ydjk.org.cn/Article/details/gt2zhjgriql.html

H 异常与错误处理       10 个任务 × 8 语言 =   80
来源：http://www.ydjk.org.cn/Article/details/gt2myojwmls.html

I 正则表达式            8 个任务 × 8 语言 =   64
来源：http://www.52xcode.cn/Article/details/gt2uxgfhizk.html

J 日期与时间           10 个任务 × 8 语言 =   80
来源：http://www.52xcode.cn/Article/details/gt2zeqkqmwy.html

K JSON 与序列化         8 个任务 × 8 语言 =   64
来源：http://www.ydjk.org.cn/Article/details/gt2fbhjvdyq.html

L 网络请求              8 个任务 × 8 语言 =   64
来源：http://www.52xcode.cn/Article/details/gt2ssflbeze.html

M 命令行 / 进程         8 个任务 × 8 语言 =   64
来源：http://www.ydjk.org.cn/Article/details/gt2nnnumgsh.html

N 数据结构与算法       12 个任务 × 8 语言 =   96
来源：http://www.52xcode.cn/Article/details/gt2eoivfifi.html

O 并发与异步            6 个任务 × 8 语言 =   48
来源：http://www.52xcode.cn/Article/details/gt2bluobleo.html

P 常用工具函数          8 个任务 × 8 语言 =   64
来源：http://www.52xcode.cn/Article/details/gt2vsunhucz.html

Q SQL 专题                              90
来源：http://www.ydjk.org.cn/Article/details/gt2vcnpwdlw.html

R Bash 专题                             80
来源：http://www.52xcode.cn/Article/details/gt2zjftxzfj.html

S C / C++ 专题                          60
来源：http://www.ydjk.org.cn/Article/details/gt2shdapwfi.html

T 其他语言补充                          60
来源：http://www.ydjk.org.cn/Article/details/gt2wamibpnb.html

U 高频实用片段                         120
来源：http://www.52xcode.cn/Article/details/gt2dwqlwxup.html

------------------------------------
来源：http://www.ydjk.org.cn/Article/details/gt2larxmpkx.html

合计                                  2106 条
来源：http://www.52xcode.cn/Article/details/gt2zckjcjrb.html

--------------------------------------------------------------------------------
来源：http://www.52xcode.cn/Article/details/gt2yulrecfs.html

使用提醒
来源：http://www.52xcode.cn/Article/details/gt2hfyyswrg.html

--------------------------------------------------------------------------------
来源：http://www.ydjk.org.cn/Article/details/gt2ylmjqdqt.html

1. 示例追求"最小可用"，正式项目中请补齐导入、错误处理与边界判断。
来源：http://www.ydjk.org.cn/Article/details/gt2uhbumfty.html

2. 涉及文件、网络、数据库的示例，注意资源释放与异常捕获。
来源：http://www.52xcode.cn/Article/details/gt2ajmkbzbg.html

3. 语言版本差异较大（如 Python 3.10 的 match、Java 17 的 record/switch 箭头），
来源：http://www.ydjk.org.cn/Article/details/gt2rkckvrwh.html

在旧版本上使用前请先确认语法支持情况。
来源：http://www.ydjk.org.cn/Article/details/gt2wtqkqawt.html

4. 标注"手写"的条目是因为该语言缺少对应内置能力，实际项目中可引入成熟库。
来源：http://www.ydjk.org.cn/Article/details/gt2kvgbeamg.html

—— 文件结束 ——
来源：http://www.52xcode.cn/Article/details/gt2hrnqhazo.html

================================================================================
来源：http://www.52xcode.cn/Article/details/gt2luswetra.html

程序语言常见例子速查手册（2024 版）
来源：http://www.52xcode.cn/Article/details/gt2gxbqskcq.html

Common Programming Examples Cheat Book
来源：http://www.ydjk.org.cn/Article/details/gt2tigcdatx.html

================================================================================
来源：http://www.ydjk.org.cn/Article/details/gt2dzbojmqw.html

【收录内容】
来源：http://www.ydjk.org.cn/Article/details/gt2hlrqmxac.html

覆盖 12 种语言 / 语法与常见 API：
来源：http://www.ydjk.org.cn/Article/details/gt2jiclvzah.html

Python · PHP · JavaScript · TypeScript · Java · Go · Ruby · C#
来源：http://www.52xcode.cn/Article/details/gt2dvgjqhxl.html

SQL · Bash · C · C++
来源：http://www.ydjk.org.cn/Article/details/gt2gtzwhhbh.html

按「任务」分组：每个任务下按语言各给出一条最小可用示例。
来源：http://www.ydjk.org.cn/Article/details/gt2tfxktzqa.html

【使用说明】
来源：http://www.52xcode.cn/Article/details/gt2vsscsxps.html

1. 每个任务形如 "[编号] 任务名"，下面每行以语言标记开头：
来源：http://www.52xcode.cn/Article/details/gt2iggxryuy.html

Py:    Python        PHP:   PHP           JS:    JavaScript
来源：http://www.52xcode.cn/Article/details/gt2qfdhkykm.html

TS:    TypeScript    Java:  Java          Go:    Go
来源：http://www.ydjk.org.cn/Article/details/gt2dfvazjdn.html

Ruby:  Ruby          C#:    C#            SQL:   SQL
来源：http://www.52xcode.cn/Article/details/gt2cwixencb.html

Bash:  Shell         C:     C             C++:   C++
来源：http://www.52xcode.cn/Article/details/gt2jbqkpaho.html

2. 示例只展示核心写法，刻意省略 import / require / include / using 等样板代码。
来源：http://www.ydjk.org.cn/Article/details/gt2wfqkrnto.html

需要完整可运行文件时，请自行补齐当前语言的导入语句。
来源：http://www.52xcode.cn/Article/details/gt2giijofmf.html

3. 语法基准：Python 3.10+ / PHP 8.1+ / ES2020+ / TypeScript 5 / Java 17 /
来源：http://www.ydjk.org.cn/Article/details/gt2qqxupuza.html

Go 1.21+ / Ruby 3.x / C# 10+ / C17 / C++17。
来源：http://www.52xcode.cn/Article/details/gt2qeauzlpd.html

4. 检索建议：用编辑器或浏览器 Ctrl+F 搜关键词，如 "排序" "读取文件" "正则"。
来源：http://www.ydjk.org.cn/Article/details/gt2yfvjezoz.html

5. 标记为 "// 无" 表示该语言没有对应的一等语法，需用替代写法（示例给出替代方案）。
来源：http://www.52xcode.cn/Article/details/gt2peoriwrq.html

6. 符号 "⏎" 表示代码在此处换行（主要用于 Python 等强制缩进、无法压成一行的结构）。
来源：http://www.ydjk.org.cn/Article/details/gt2adaveiyy.html

【文件统计】
来源：http://www.52xcode.cn/Article/details/gt2alelqhzl.html

语言示例共 2106 条，分布见本文末尾的「统计汇总」。
来源：http://www.ydjk.org.cn/Article/details/gt2anvorfsk.html

--------------------------------------------------------------------------------
来源：http://www.ydjk.org.cn/Article/details/gt2qzowyewv.html

目  录
来源：http://www.52xcode.cn/Article/details/gt2shxcgzuq.html

--------------------------------------------------------------------------------
来源：http://www.52xcode.cn/Article/details/gt2zmdzgems.html

A. 基础语法与类型              （第 1 节，26 个任务，208 条）
来源：http://www.ydjk.org.cn/Article/details/gt2hrtatioo.html


<!-- 参考信息 -->