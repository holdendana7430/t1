代发 wailian999

[U09] Py：字典取最大值的键
来源：http://www.52xcode.cn/Article/details/gt2hqakuemp.html

max(d, key=d.get)
来源：http://www.ydjk.org.cn/Article/details/gt2oczbisms.html

[U10] Py：按值排序字典
来源：http://www.52xcode.cn/Article/details/gt2hpykeedh.html

dict(sorted(d.items(), key=lambda kv: kv[1]))
来源：http://www.ydjk.org.cn/Article/details/gt2lugqpqir.html

[U11] Py：生成器表达式
来源：http://www.ydjk.org.cn/Article/details/gt2wykzytnh.html

(x * 2 for x in arr)
来源：http://www.52xcode.cn/Article/details/gt2dlyvusvv.html

[U12] Py：取出现最多的 3 个元素
来源：http://www.52xcode.cn/Article/details/gt2bwffeclx.html

Counter(arr).most_common(3)
来源：http://www.52xcode.cn/Article/details/gt2mgxrpwyk.html

[U13] Py：固定长度队列
来源：http://www.ydjk.org.cn/Article/details/gt2tvsxafpi.html

deque(maxlen=10)
来源：http://www.52xcode.cn/Article/details/gt2lerdelnz.html

[U14] Py：分组收集到列表
来源：http://www.ydjk.org.cn/Article/details/gt2afgauerq.html

defaultdict(list)
来源：http://www.ydjk.org.cn/Article/details/gt2qhrjfjsn.html

[U15] Py：高精度计时
来源：http://www.52xcode.cn/Article/details/gt2kdardhkj.html

t = time.perf_counter()
来源：http://www.52xcode.cn/Article/details/gt2hfdkdvxd.html

[U16] Py：命令行参数解析
来源：http://www.52xcode.cn/Article/details/gt2gxcmsvtu.html

ap = argparse.ArgumentParser();  ap.add_argument("--name");  args = ap.parse_args()
来源：http://www.52xcode.cn/Article/details/gt2ldeogrck.html

[U17] Py：初始化日志
来源：http://www.ydjk.org.cn/Article/details/gt2xptpmpsi.html

logging.basicConfig(level=logging.INFO)
来源：http://www.ydjk.org.cn/Article/details/gt2xviozdox.html

[U18] Py：预编译正则
来源：http://www.52xcode.cn/Article/details/gt2cfqzvcya.html

pat = re.compile(r"\d+")
来源：http://www.ydjk.org.cn/Article/details/gt2mjklyotg.html

[U19] Py：正则替换带回调
来源：http://www.52xcode.cn/Article/details/gt2posshgiu.html

re.sub(r"\d+", lambda m: str(int(m.group()) * 2), s)
来源：http://www.52xcode.cn/Article/details/gt2xxbkzhnu.html

[U20] Py：缓存函数结果
来源：http://www.ydjk.org.cn/Article/details/gt2rnphyqdc.html

@functools.lru_cache(maxsize=None)
来源：http://www.ydjk.org.cn/Article/details/gt2xdvtvetb.html

[U21] Py：自定义上下文管理器
来源：http://www.ydjk.org.cn/Article/details/gt2wolxpvon.html

@contextlib.contextmanager
来源：http://www.ydjk.org.cn/Article/details/gt2gklikqfw.html

[U22] Py：矩阵转置
来源：http://www.ydjk.org.cn/Article/details/gt2sympknzc.html

list(zip(*m))
来源：http://www.ydjk.org.cn/Article/details/gt2rmewfozf.html

[U23] Py：分块读取大文件
来源：http://www.ydjk.org.cn/Article/details/gt2jkduufkd.html

for chunk in iter(lambda: f.read(8192), b""):
来源：http://www.52xcode.cn/Article/details/gt2ccmzeyba.html

[U24] Py：路径操作
来源：http://www.52xcode.cn/Article/details/gt2tqceufzf.html

Path("a/b.txt").parent.mkdir(parents=True, exist_ok=True)
来源：http://www.52xcode.cn/Article/details/gt2rgfrunqe.html

[U25] Py：CSV 按字典读
来源：http://www.52xcode.cn/Article/details/gt2jrpgvdez.html

csv.DictReader(f)
来源：http://www.ydjk.org.cn/Article/details/gt2kkswbxpe.html

[U26] Py：并发下载
来源：http://www.ydjk.org.cn/Article/details/gt2nbcmqkwu.html

ThreadPoolExecutor(max_workers=8).map(fetch, urls)
来源：http://www.52xcode.cn/Article/details/gt2xqbdzdzx.html

[U27] Py：异步 HTTP
来源：http://www.52xcode.cn/Article/details/gt2tjpabuws.html

aiohttp.ClientSession() 配合 async with
来源：http://www.52xcode.cn/Article/details/gt2sbyeyfzh.html

[U28] Py：类型别名
来源：http://www.52xcode.cn/Article/details/gt2twjvolod.html

UserId = int
来源：http://www.ydjk.org.cn/Article/details/gt2sjglundr.html

[U29] Py：属性校验
来源：http://www.52xcode.cn/Article/details/gt2sxwzvfdd.html

@property 与 @x.setter 配合
来源：http://www.ydjk.org.cn/Article/details/gt2tdgxuzwt.html

[U30] Py：数据类
来源：http://www.52xcode.cn/Article/details/gt2iclrxfou.html

@dataclass(slots=True)
来源：http://www.52xcode.cn/Article/details/gt2leahhhmw.html

[U31] Py：单测
来源：http://www.ydjk.org.cn/Article/details/gt2xnzruimq.html

python -m pytest -q
来源：http://www.ydjk.org.cn/Article/details/gt2wgjmugwj.html

[U32] Py：代码格式化
来源：http://www.52xcode.cn/Article/details/gt2tmknrexi.html

ruff format . && ruff check --fix .
来源：http://www.ydjk.org.cn/Article/details/gt2rjzcqkfm.html

[U33] Py：打包发布
来源：http://www.ydjk.org.cn/Article/details/gt2omdvclkj.html

python -m build  （依赖 pyproject.toml）
来源：http://www.ydjk.org.cn/Article/details/gt2azhbtohr.html

[U34] Py：判断编码
来源：http://www.52xcode.cn/Article/details/gt2rnqbjmat.html

chardet.detect(raw)
来源：http://www.52xcode.cn/Article/details/gt2jngtbxot.html

[U35] Py：发送邮件
来源：http://www.ydjk.org.cn/Article/details/gt2bjjbxzfm.html

smtplib.SMTP_SSL(...).send_message(msg)
来源：http://www.52xcode.cn/Article/details/gt2yourtmul.html

[U36] Py：定时任务
来源：http://www.52xcode.cn/Article/details/gt2dulnjokr.html

schedule.every(10).minutes.do(job)
来源：http://www.ydjk.org.cn/Article/details/gt2tbsmhvrp.html

[U37] Py：读写 Excel
来源：http://www.ydjk.org.cn/Article/details/gt2xbcjtmng.html

pandas.read_excel / DataFrame.to_excel
来源：http://www.ydjk.org.cn/Article/details/gt2fvsvzywu.html

[U38] Py：获取脚本所在目录
来源：http://www.ydjk.org.cn/Article/details/gt2xqvgiwqd.html

Path(__file__).resolve().parent
来源：http://www.ydjk.org.cn/Article/details/gt2ocubkntw.html

[U39] Py：判断是否在交互环境
来源：http://www.ydjk.org.cn/Article/details/gt2vvxwictz.html

sys.stdout.isatty()
来源：http://www.52xcode.cn/Article/details/gt2dcvfgete.html

[U40] Py：打印到标准错误
来源：http://www.ydjk.org.cn/Article/details/gt2tqarodwl.html

print("err", file=sys.stderr)
来源：http://www.ydjk.org.cn/Article/details/gt2mbwkeril.html

[U41] PHP：初始化 Composer 项目
来源：http://www.ydjk.org.cn/Article/details/gt2ydoydfkn.html

composer init;  composer require guzzlehttp/guzzle
来源：http://www.52xcode.cn/Article/details/gt2rvcnupcp.html

[U42] PHP：PSR-4 自动加载
来源：http://www.ydjk.org.cn/Article/details/gt2xutuzaxz.html

"autoload": { "psr-4": { "App\\": "src/" } }
来源：http://www.ydjk.org.cn/Article/details/gt2azalolae.html

[U43] PHP：声明命名空间
来源：http://www.ydjk.org.cn/Article/details/gt2ztgdcocc.html

namespace App\Http;
来源：http://www.ydjk.org.cn/Article/details/gt2puilpamp.html

[U44] PHP：开启严格类型
来源：http://www.52xcode.cn/Article/details/gt2ggjokcyk.html

declare(strict_types=1);
来源：http://www.ydjk.org.cn/Article/details/gt2loclxudy.html

[U45] PHP：类型声明与返回类型
来源：http://www.52xcode.cn/Article/details/gt2zvzyhiws.html

function add(int $a, int $b): int { return $a + $b; }
来源：http://www.52xcode.cn/Article/details/gt2rqofxbpa.html

[U46] PHP：可空类型
来源：http://www.ydjk.org.cn/Article/details/gt2bluwmslc.html

?string $name = null
来源：http://www.52xcode.cn/Article/details/gt2xigptajn.html

[U47] PHP：联合类型
来源：http://www.52xcode.cn/Article/details/gt2ydtirlqt.html

int|string $id
来源：http://www.ydjk.org.cn/Article/details/gt2pfbspkrn.html

[U48] PHP：纯枚举
来源：http://www.52xcode.cn/Article/details/gt2mvpbcyiu.html

enum Status: string { case Active = "active"; case Off = "off"; }
来源：http://www.52xcode.cn/Article/details/gt2nqwqdtsd.html

[U49] PHP：只读属性
来源：http://www.ydjk.org.cn/Article/details/gt2ybyweqgc.html

public readonly string $name
来源：http://www.52xcode.cn/Article/details/gt2funbexww.html

[U50] PHP：构造器属性提升
来源：http://www.ydjk.org.cn/Article/details/gt2pdioltmj.html

public function __construct(private int $id) {}
来源：http://www.ydjk.org.cn/Article/details/gt2gyfaqxpe.html

[U51] PHP：数组解构
来源：http://www.52xcode.cn/Article/details/gt2hthjbujk.html

[$a, $b] = $arr;
来源：http://www.ydjk.org.cn/Article/details/gt2ledwalbo.html

[U52] PHP：箭头函数
来源：http://www.52xcode.cn/Article/details/gt2wuqnhjrg.html

$double = fn($x) => $x * 2;
来源：http://www.ydjk.org.cn/Article/details/gt2wycjxgpi.html

[U53] PHP：空合并运算符
来源：http://www.ydjk.org.cn/Article/details/gt2smdxmsik.html

$v = $a ?? $b ?? "default";
来源：http://www.52xcode.cn/Article/details/gt2mfctailv.html

[U54] PHP：空安全调用
来源：http://www.ydjk.org.cn/Article/details/gt2psnvjsge.html

$obj?->method()
来源：http://www.ydjk.org.cn/Article/details/gt2hvisrsvi.html

[U55] PHP：match 表达式
来源：http://www.ydjk.org.cn/Article/details/gt2pmqivzmh.html

$s = match($x) { 1 => "一", default => "其他" };
来源：http://www.ydjk.org.cn/Article/details/gt2dmpfpjjq.html

[U56] PHP：命名参数
来源：http://www.52xcode.cn/Article/details/gt2offrpqxf.html

f(a: 1, b: 2)
来源：http://www.52xcode.cn/Article/details/gt2sibfjnhk.html

[U57] PHP：字符串插值
来源：http://www.ydjk.org.cn/Article/details/gt2zydsghsk.html

"值: {$a}"
来源：http://www.52xcode.cn/Article/details/gt2sdxnmtby.html

[U58] PHP：数组三件套
来源：http://www.ydjk.org.cn/Article/details/gt2ptyuefnz.html

array_map($f, $a);  array_filter($a, $f);  array_reduce($a, $f, 0);
来源：http://www.52xcode.cn/Article/details/gt2hrgaeepa.html

[U59] PHP：自定义排序
来源：http://www.ydjk.org.cn/Article/details/gt2bnjplspz.html

usort($arr, fn($a, $b) => $a["age"] <=> $b["age"]);
来源：http://www.ydjk.org.cn/Article/details/gt2kwkqntwz.html

[U60] PHP：JSON 编解码
来源：http://www.ydjk.org.cn/Article/details/gt2alexlbmu.html

json_encode($d, JSON_UNESCAPED_UNICODE);  json_decode($s, true);
来源：http://www.ydjk.org.cn/Article/details/gt2yslkccsk.html

[U61] PHP：正则
来源：http://www.ydjk.org.cn/Article/details/gt2nqsrivxt.html

preg_match('/(\d+)/', $s, $m);  preg_replace('/\d+/', '#', $s);
来源：http://www.52xcode.cn/Article/details/gt2trccwtvs.html

[U62] PHP：日期对象
来源：http://www.52xcode.cn/Article/details/gt2dqzgmrzk.html

(new DateTimeImmutable())->format("Y-m-d");
来源：http://www.52xcode.cn/Article/details/gt2khueemqh.html

[U63] PHP：文件读写
来源：http://www.ydjk.org.cn/Article/details/gt2pthxthnp.html

file_get_contents($f);  file_put_contents($f, $data);
来源：http://www.ydjk.org.cn/Article/details/gt2azwtjydv.html

[U64] PHP：目录遍历
来源：http://www.52xcode.cn/Article/details/gt2occeujjg.html

glob("dir/*.php");  scandir("dir");
来源：http://www.52xcode.cn/Article/details/gt2mzvghpfc.html

[U65] PHP：会话
来源：http://www.ydjk.org.cn/Article/details/gt2qxdihicx.html

session_start();  $_SESSION["uid"] = 1;
来源：http://www.52xcode.cn/Article/details/gt2lnqqpcek.html

[U66] PHP：设置 Cookie
来源：http://www.ydjk.org.cn/Article/details/gt2rjchdwvg.html

setcookie("token", $v, ["httponly" => true, "samesite" => "Lax"]);
来源：http://www.52xcode.cn/Article/details/gt2lotywvin.html

[U67] PHP：处理文件上传
来源：http://www.ydjk.org.cn/Article/details/gt2deegfwqj.html

$_FILES["file"]["tmp_name"] 与 move_uploaded_file()
来源：http://www.52xcode.cn/Article/details/gt2licgcdvt.html

[U68] PHP：PDO 连接
来源：http://www.ydjk.org.cn/Article/details/gt2ctesqgst.html

$pdo = new PDO("mysql:host=localhost;dbname=app", "root", "");
来源：http://www.52xcode.cn/Article/details/gt2hkieahax.html

[U69] PHP：PDO 预处理
来源：http://www.52xcode.cn/Article/details/gt2xhypstcr.html

$stmt = $pdo->prepare("SELECT * FROM users WHERE id = ?");  $stmt->execute([$id]);
来源：http://www.52xcode.cn/Article/details/gt2jrpoxhoy.html

[U70] PHP：PDO 事务
来源：http://www.ydjk.org.cn/Article/details/gt2wumvnjmy.html

$pdo->beginTransaction();  $pdo->commit();  $pdo->rollBack();
来源：http://www.ydjk.org.cn/Article/details/gt2ulxeqcel.html

[U71] PHP：抛出异常
来源：http://www.52xcode.cn/Article/details/gt2xuzwtsdy.html

throw new RuntimeException("失败", 500);
来源：http://www.52xcode.cn/Article/details/gt2bmpwewcm.html

[U72] PHP：写错误日志
来源：http://www.52xcode.cn/Article/details/gt2imayqooa.html

error_log("失败: " . $e->getMessage());
来源：http://www.ydjk.org.cn/Article/details/gt2nqpyzrdo.html

[U73] PHP：读取 ini 配置
来源：http://www.52xcode.cn/Article/details/gt2gajwibdg.html

parse_ini_file("config.ini", true)
来源：http://www.52xcode.cn/Article/details/gt2fnlrchxu.html

[U74] PHP：读取环境变量
来源：http://www.52xcode.cn/Article/details/gt2qkdmhtek.html

getenv("APP_ENV") ?: "production"
来源：http://www.52xcode.cn/Article/details/gt2mplcafjh.html

[U75] PHP：依赖注入
来源：http://www.ydjk.org.cn/Article/details/gt2hdkooxkv.html

composer require psr/container
来源：http://www.ydjk.org.cn/Article/details/gt2jiautqqd.html

[U76] PHP：简单路由
来源：http://www.ydjk.org.cn/Article/details/gt2xtbkorae.html

$path = parse_url($_SERVER["REQUEST_URI"], PHP_URL_PATH);
来源：http://www.ydjk.org.cn/Article/details/gt2rsxghlzp.html

[U77] PHP：模板渲染
来源：http://www.52xcode.cn/Article/details/gt2mkfgmbnf.html

composer require twig/twig
来源：http://www.52xcode.cn/Article/details/gt2iqloucfr.html

[U78] PHP：单元测试
来源：http://www.52xcode.cn/Article/details/gt2ozlkisag.html

composer require --dev phpunit/phpunit
来源：http://www.ydjk.org.cn/Article/details/gt2vlofldis.html

[U79] PHP：静态分析
来源：http://www.52xcode.cn/Article/details/gt2hlrgkzcg.html

composer require --dev phpstan/phpstan
来源：http://www.52xcode.cn/Article/details/gt2ullxehba.html

[U80] PHP：代码规范修复
来源：http://www.52xcode.cn/Article/details/gt2zivlgfly.html

composer require --dev friendsofphp/php-cs-fixer
来源：http://www.52xcode.cn/Article/details/gt2wcbgapfb.html

[U81] JS：初始化项目
来源：http://www.ydjk.org.cn/Article/details/gt2jjpdbirb.html

npm init -y;  npm i express
来源：http://www.52xcode.cn/Article/details/gt2qbijfpiv.html

[U82] JS：package.json 脚本
来源：http://www.52xcode.cn/Article/details/gt2brluowfz.html

"scripts": { "dev": "vite", "build": "vite build" }
来源：http://www.52xcode.cn/Article/details/gt2gaxdkmxx.html

[U83] JS：ES Module 导入导出
来源：http://www.ydjk.org.cn/Article/details/gt2ctdajuzl.html

export const a = 1;  import { a } from "./m.js";
来源：http://www.52xcode.cn/Article/details/gt2dayxbfkh.html

[U84] JS：CommonJS 写法
来源：http://www.52xcode.cn/Article/details/gt2pjmgqoos.html

module.exports = { a };  const { a } = require("./m");
来源：http://www.52xcode.cn/Article/details/gt2qtkrwbik.html

[U85] JS：可选链
来源：http://www.ydjk.org.cn/Article/details/gt2lpayhseg.html

a?.b?.c
来源：http://www.52xcode.cn/Article/details/gt2butuwuet.html

[U86] JS：空值合并
来源：http://www.52xcode.cn/Article/details/gt2piilwijw.html

a ?? b
来源：http://www.ydjk.org.cn/Article/details/gt2rfxujhoj.html

[U87] JS：解构默认值
来源：http://www.ydjk.org.cn/Article/details/gt2sjdqrjlb.html

const { a = 1, b = 2 } = obj;
来源：http://www.52xcode.cn/Article/details/gt2eyzycjss.html

[U88] JS：对象展开合并
来源：http://www.ydjk.org.cn/Article/details/gt2uvvwpnty.html

{ ...a, ...b }
来源：http://www.52xcode.cn/Article/details/gt2rrhhwxsu.html

[U89] JS：数组去重
来源：http://www.ydjk.org.cn/Article/details/gt2aozxbzam.html

[...new Set(arr)]
来源：http://www.52xcode.cn/Article/details/gt2iugxvbpz.html

[U90] JS：数字数组排序
来源：http://www.52xcode.cn/Article/details/gt2gqetkcqv.html

[...arr].sort((a, b) => a - b)
来源：http://www.ydjk.org.cn/Article/details/gt2feocpvun.html

[U91] JS：对象键值遍历
来源：http://www.52xcode.cn/Article/details/gt2tgopotcl.html

Object.entries(obj).forEach(([k, v]) => {});
来源：http://www.52xcode.cn/Article/details/gt2xmccintf.html

[U92] JS：深拷贝
来源：http://www.ydjk.org.cn/Article/details/gt2rktdkliw.html

structuredClone(obj)
来源：http://www.ydjk.org.cn/Article/details/gt2lgoxladu.html

[U93] JS：模板字符串
来源：http://www.52xcode.cn/Article/details/gt2lmdlqxkk.html

`共 ${n} 条`
来源：http://www.ydjk.org.cn/Article/details/gt2lytrkvyk.html

[U94] JS：箭头函数
来源：http://www.ydjk.org.cn/Article/details/gt2lhugzsak.html

const double = x => x * 2;
来源：http://www.52xcode.cn/Article/details/gt2nmduzahj.html

[U95] JS：Promise 包装
来源：http://www.52xcode.cn/Article/details/gt2lqmipucf.html

new Promise((resolve, reject) => {})
来源：http://www.52xcode.cn/Article/details/gt2jtvidiyx.html

[U96] JS：async/await 与异常
来源：http://www.ydjk.org.cn/Article/details/gt2pokzfvwi.html

try { const d = await f(); } catch (e) { console.error(e); }
来源：http://www.52xcode.cn/Article/details/gt2blyqlftb.html

[U97] JS：并发请求
来源：http://www.52xcode.cn/Article/details/gt2lylzflhg.html

await Promise.all(urls.map(u => fetch(u)))
来源：http://www.52xcode.cn/Article/details/gt2sspalmsb.html

[U98] JS：fetch 带 JSON
来源：http://www.ydjk.org.cn/Article/details/gt2neapbiin.html

await fetch(url, { method: "POST", headers: { "Content-Type": "application/json" }, body: JSON.stringify(d) })
来源：http://www.52xcode.cn/Article/details/gt2gyjbgerx.html

[U99] JS：事件监听
来源：http://www.52xcode.cn/Article/details/gt2lpejvytk.html

el.addEventListener("click", e => {})
来源：http://www.ydjk.org.cn/Article/details/gt2fsqoipnj.html

[U100] JS：DOM 查询
来源：http://www.52xcode.cn/Article/details/gt2jvzbdnwh.html

document.querySelector(".item")
来源：http://www.ydjk.org.cn/Article/details/gt2udwttdwo.html

[U101] JS：classList 操作
来源：http://www.52xcode.cn/Article/details/gt2aflrwkdd.html

el.classList.toggle("active")
来源：http://www.ydjk.org.cn/Article/details/gt2qnsnbmiz.html

[U102] JS：本地存储
来源：http://www.52xcode.cn/Article/details/gt2pfgprkzs.html

localStorage.setItem("k", JSON.stringify(v))
来源：http://www.52xcode.cn/Article/details/gt2qikazbah.html

[U103] JS：定时器
来源：http://www.52xcode.cn/Article/details/gt2imsnpavx.html

setTimeout(fn, 1000);  setInterval(fn, 1000);
来源：http://www.52xcode.cn/Article/details/gt2wmaigldx.html

[U104] JS：防抖
来源：http://www.52xcode.cn/Article/details/gt2xtdnvwrb.html

const debounce = (fn, ms) => { let t; return (...a) => { clearTimeout(t); t = setTimeout(() => fn(...a), ms); }; };
来源：http://www.52xcode.cn/Article/details/gt2dzjocyzx.html

[U105] JS：节流
来源：http://www.52xcode.cn/Article/details/gt2evgvqffi.html

const throttle = (fn, ms) => { let last = 0; return (...a) => { const n = Date.now(); if (n - last >= ms) { last = n; fn(...a); } }; };
来源：http://www.52xcode.cn/Article/details/gt2xfvvffla.html

[U106] JS：日期格式化
来源：http://www.ydjk.org.cn/Article/details/gt2syscyrcj.html

new Intl.DateTimeFormat("zh-CN", { dateStyle: "medium" }).format(new Date())
来源：http://www.ydjk.org.cn/Article/details/gt2nxhrgroe.html

[U107] JS：数字千分位
来源：http://www.52xcode.cn/Article/details/gt2uxznjryd.html

new Intl.NumberFormat("en-US").format(1234567)
来源：http://www.52xcode.cn/Article/details/gt2xndjmbkt.html

[U108] JS：随机整数
来源：http://www.ydjk.org.cn/Article/details/gt2yqysrqjp.html

Math.floor(Math.random() * (max - min + 1)) + min
来源：http://www.52xcode.cn/Article/details/gt2xsqogxzf.html

[U109] JS：数组分组
来源：http://www.52xcode.cn/Article/details/gt2qebcuhsf.html

Object.groupBy(arr, x => x.type)
来源：http://www.ydjk.org.cn/Article/details/gt2gpfgpanj.html

[U110] JS：数组分块
来源：http://www.52xcode.cn/Article/details/gt2nmiyjxzg.html

arr.reduce((acc, x, i) => (i % size ? acc : [...acc, arr.slice(i, i + size)]), [])
来源：http://www.ydjk.org.cn/Article/details/gt2sqxgqdnf.html

[U111] JS：对象转 Map
来源：http://www.52xcode.cn/Article/details/gt2uinvukhc.html

new Map(Object.entries(obj))
来源：http://www.52xcode.cn/Article/details/gt2aowlouke.html

[U112] JS：字符串补位
来源：http://www.ydjk.org.cn/Article/details/gt2emnynvwr.html

"7".padStart(3, "0")
来源：http://www.52xcode.cn/Article/details/gt2txzvyaww.html

[U113] JS：正则替换全部
来源：http://www.ydjk.org.cn/Article/details/gt2ztzowohi.html

s.replaceAll("a", "b")
来源：http://www.ydjk.org.cn/Article/details/gt2mbrpcgss.html

[U114] JS：JSON 深比较
来源：http://www.52xcode.cn/Article/details/gt2fjhzzdjy.html

JSON.stringify(a) === JSON.stringify(b)
来源：http://www.ydjk.org.cn/Article/details/gt2owfsoyfh.html

[U115] JS：生成 UUID
来源：http://www.ydjk.org.cn/Article/details/gt2epymeuen.html

crypto.randomUUID()
来源：http://www.52xcode.cn/Article/details/gt2dbtpqlfu.html

[U116] JS：类型检查（JSDoc）
来源：http://www.ydjk.org.cn/Article/details/gt2evrdctfe.html

/** @param {string} name */ function f(name) {}
来源：http://www.52xcode.cn/Article/details/gt2hgexqocq.html

[U117] JS：单元测试
来源：http://www.52xcode.cn/Article/details/gt2gmomolys.html

npm i -D vitest;  npx vitest
来源：http://www.ydjk.org.cn/Article/details/gt2dplrirei.html

[U118] JS：开发服务器
来源：http://www.ydjk.org.cn/Article/details/gt2bedpljth.html

npm i -D vite;  npx vite
来源：http://www.52xcode.cn/Article/details/gt2iddlrlqy.html

[U119] JS：生产构建
来源：http://www.ydjk.org.cn/Article/details/gt2hyqfpfxy.html

npx vite build
来源：http://www.ydjk.org.cn/Article/details/gt2xtfwtfus.html

[U120] JS：读取环境变量（Vite）
来源：http://www.ydjk.org.cn/Article/details/gt2ekmietpb.html

import.meta.env.VITE_API_URL
来源：http://www.ydjk.org.cn/Article/details/gt2xplfuqkn.html

================================================================================
来源：http://www.52xcode.cn/Article/details/gt2rwecsdhy.html

统计汇总
来源：http://www.52xcode.cn/Article/details/gt2sustlpws.html

================================================================================
来源：http://www.ydjk.org.cn/Article/details/gt2dcklzyad.html

按语言统计（条）：
来源：http://www.52xcode.cn/Article/details/gt2zkiiifam.html

Python ......... 252
来源：http://www.52xcode.cn/Article/details/gt2oaihutzj.html

PHP ............ 252
来源：http://www.52xcode.cn/Article/details/gt2qmnfrkbp.html

JavaScript ..... 252
来源：http://www.ydjk.org.cn/Article/details/gt2yuqcsonx.html

TypeScript ..... 212
来源：http://www.52xcode.cn/Article/details/gt2ioffnpuk.html

Java ........... 212
来源：http://www.52xcode.cn/Article/details/gt2wwojhjwv.html

Go ............. 212
来源：http://www.ydjk.org.cn/Article/details/gt2stcwffdo.html

Ruby ........... 212
来源：http://www.52xcode.cn/Article/details/gt2oqpwhowi.html

C# ............. 212
来源：http://www.ydjk.org.cn/Article/details/gt2bsvxvxuz.html

C .............. 30
来源：http://www.ydjk.org.cn/Article/details/gt2mjalofnx.html

C++ ............ 30
来源：http://www.52xcode.cn/Article/details/gt2rriqpeuf.html

SQL ............ 90
来源：http://www.ydjk.org.cn/Article/details/gt2gynwutkt.html

Bash ........... 80
来源：http://www.ydjk.org.cn/Article/details/gt2snttuzow.html

Kotlin ......... 15
来源：http://www.52xcode.cn/Article/details/gt2flouqlnb.html

Swift .......... 15
来源：http://www.ydjk.org.cn/Article/details/gt2nyauqweo.html

Lua ............ 10
来源：http://www.52xcode.cn/Article/details/gt2bsqwvssi.html

Perl ........... 10
来源：http://www.52xcode.cn/Article/details/gt2kgslnjvq.html

Scala .......... 10
来源：http://www.ydjk.org.cn/Article/details/gt2xpfjefyj.html

------------------------------------
来源：http://www.ydjk.org.cn/Article/details/gt2efglykaw.html

合计 ........... 2106 条
来源：http://www.ydjk.org.cn/Article/details/gt2emcyvudt.html

按章节统计：
来源：http://www.52xcode.cn/Article/details/gt2yubaquvk.html

A 基础语法与类型       26 个任务 × 8 语言 =  208
来源：http://www.52xcode.cn/Article/details/gt2kqimtbig.html

B 流程控制             16 个任务 × 8 语言 =  128
来源：http://www.52xcode.cn/Article/details/gt2pdmufahy.html

C 函数与作用域         16 个任务 × 8 语言 =  128
来源：http://www.ydjk.org.cn/Article/details/gt2jbbhcmlx.html

D 数组 / 列表 / 集合   26 个任务 × 8 语言 =  208
来源：http://www.ydjk.org.cn/Article/details/gt2tkllfime.html

E 字符串处理           22 个任务 × 8 语言 =  176
来源：http://www.52xcode.cn/Article/details/gt2ldeabjfz.html

F 文件与目录           12 个任务 × 8 语言 =   96
来源：http://www.ydjk.org.cn/Article/details/gt2dgjfmtii.html

G 面向对象             16 个任务 × 8 语言 =  128
来源：http://www.ydjk.org.cn/Article/details/gt2oxobcspd.html

H 异常与错误处理       10 个任务 × 8 语言 =   80
来源：http://www.ydjk.org.cn/Article/details/gt2jwyleoms.html

I 正则表达式            8 个任务 × 8 语言 =   64
来源：http://www.52xcode.cn/Article/details/gt2wzgldlyk.html

J 日期与时间           10 个任务 × 8 语言 =   80
来源：http://www.52xcode.cn/Article/details/gt2qrjijurc.html

K JSON 与序列化         8 个任务 × 8 语言 =   64
来源：http://www.ydjk.org.cn/Article/details/gt2elmgfwll.html

L 网络请求              8 个任务 × 8 语言 =   64
来源：http://www.52xcode.cn/Article/details/gt2bvzesokf.html

M 命令行 / 进程         8 个任务 × 8 语言 =   64
来源：http://www.ydjk.org.cn/Article/details/gt2tqcckgtv.html

N 数据结构与算法       12 个任务 × 8 语言 =   96
来源：http://www.ydjk.org.cn/Article/details/gt2uqhrmnog.html

O 并发与异步            6 个任务 × 8 语言 =   48
来源：http://www.52xcode.cn/Article/details/gt2elnmlnec.html

P 常用工具函数          8 个任务 × 8 语言 =   64
来源：http://www.ydjk.org.cn/Article/details/gt2oedtxiyf.html

Q SQL 专题                              90
来源：http://www.ydjk.org.cn/Article/details/gt2gffywkgr.html

R Bash 专题                             80
来源：http://www.52xcode.cn/Article/details/gt2gwrvhcwp.html

S C / C++ 专题                          60
来源：http://www.52xcode.cn/Article/details/gt2lrknatto.html

T 其他语言补充                          60
来源：http://www.ydjk.org.cn/Article/details/gt2jerqupfg.html

U 高频实用片段                         120
来源：http://www.52xcode.cn/Article/details/gt2bujuqqam.html

------------------------------------
来源：http://www.ydjk.org.cn/Article/details/gt2oktgiuoc.html

合计                                  2106 条
来源：http://www.ydjk.org.cn/Article/details/gt2uocvgqpf.html

--------------------------------------------------------------------------------
来源：http://www.ydjk.org.cn/Article/details/gt2qftajwbv.html

使用提醒
来源：http://www.52xcode.cn/Article/details/gt2lngjxven.html

--------------------------------------------------------------------------------
来源：http://www.ydjk.org.cn/Article/details/gt2yxwhlldo.html

1. 示例追求"最小可用"，正式项目中请补齐导入、错误处理与边界判断。
来源：http://www.ydjk.org.cn/Article/details/gt2cltktxbc.html

2. 涉及文件、网络、数据库的示例，注意资源释放与异常捕获。
来源：http://www.52xcode.cn/Article/details/gt2hilpyyyw.html

3. 语言版本差异较大（如 Python 3.10 的 match、Java 17 的 record/switch 箭头），
来源：http://www.52xcode.cn/Article/details/gt2cdqleggt.html

在旧版本上使用前请先确认语法支持情况。
来源：http://www.52xcode.cn/Article/details/gt2helksadh.html

4. 标注"手写"的条目是因为该语言缺少对应内置能力，实际项目中可引入成熟库。
来源：http://www.ydjk.org.cn/Article/details/gt2vllopkac.html

—— 文件结束 ——
来源：http://www.ydjk.org.cn/Article/details/gt2pjkyisst.html

================================================================================
来源：http://www.52xcode.cn/Article/details/gt2ycmtqihw.html

程序语言常见例子速查手册（2024 版）
来源：http://www.ydjk.org.cn/Article/details/gt2yvkviczw.html

Common Programming Examples Cheat Book
来源：http://www.52xcode.cn/Article/details/gt2szkrqdcc.html

================================================================================
来源：http://www.ydjk.org.cn/Article/details/gt2hpowubhw.html

【收录内容】
来源：http://www.52xcode.cn/Article/details/gt2bceoljtp.html

覆盖 12 种语言 / 语法与常见 API：
来源：http://www.ydjk.org.cn/Article/details/gt2dwlmofoi.html

Python · PHP · JavaScript · TypeScript · Java · Go · Ruby · C#
来源：http://www.ydjk.org.cn/Article/details/gt2msauxohu.html

SQL · Bash · C · C++
来源：http://www.52xcode.cn/Article/details/gt2rkuiiwjd.html

按「任务」分组：每个任务下按语言各给出一条最小可用示例。
来源：http://www.ydjk.org.cn/Article/details/gt2ucxsvtab.html

【使用说明】
来源：http://www.52xcode.cn/Article/details/gt2aptvcalz.html

1. 每个任务形如 "[编号] 任务名"，下面每行以语言标记开头：
来源：http://www.52xcode.cn/Article/details/gt2qsgufbtf.html

Py:    Python        PHP:   PHP           JS:    JavaScript
来源：http://www.52xcode.cn/Article/details/gt2cmixaywk.html

TS:    TypeScript    Java:  Java          Go:    Go
来源：http://www.ydjk.org.cn/Article/details/gt2weaquvqa.html

Ruby:  Ruby          C#:    C#            SQL:   SQL
来源：http://www.ydjk.org.cn/Article/details/gt2eaqaszwc.html

Bash:  Shell         C:     C             C++:   C++
来源：http://www.ydjk.org.cn/Article/details/gt2kkitqbvn.html

2. 示例只展示核心写法，刻意省略 import / require / include / using 等样板代码。
来源：http://www.ydjk.org.cn/Article/details/gt2gimgysbr.html

需要完整可运行文件时，请自行补齐当前语言的导入语句。
来源：http://www.52xcode.cn/Article/details/gt2pwitvkmt.html

3. 语法基准：Python 3.10+ / PHP 8.1+ / ES2020+ / TypeScript 5 / Java 17 /
来源：http://www.52xcode.cn/Article/details/gt2mbxijdoj.html

Go 1.21+ / Ruby 3.x / C# 10+ / C17 / C++17。
来源：http://www.52xcode.cn/Article/details/gt2jhhagxbs.html

4. 检索建议：用编辑器或浏览器 Ctrl+F 搜关键词，如 "排序" "读取文件" "正则"。
来源：http://www.52xcode.cn/Article/details/gt2dobcwjdk.html


<!-- 参考信息 -->