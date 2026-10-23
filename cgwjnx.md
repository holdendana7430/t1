代发 wailian999

[U11] Py：生成器表达式
来源：http://www.52xcode.cn/Article/details/gt3mysxixzx.html

(x * 2 for x in arr)
来源：http://www.52xcode.cn/Article/details/gt3xlpjxhng.html

[U12] Py：取出现最多的 3 个元素
来源：http://www.52xcode.cn/Article/details/gt3tjewdekv.html

Counter(arr).most_common(3)
来源：http://www.ydjk.org.cn/Article/details/gt3nhyazsol.html

[U13] Py：固定长度队列
来源：http://www.52xcode.cn/Article/details/gt3fwmrstma.html

deque(maxlen=10)
来源：http://www.52xcode.cn/Article/details/gt3qqgvorbg.html

[U14] Py：分组收集到列表
来源：http://www.ydjk.org.cn/Article/details/gt3pagrkglt.html

defaultdict(list)
来源：http://www.52xcode.cn/Article/details/gt3btvgwkvc.html

[U15] Py：高精度计时
来源：http://www.52xcode.cn/Article/details/gt3tjwigscv.html

t = time.perf_counter()
来源：http://www.52xcode.cn/Article/details/gt3dnsvnsxp.html

[U16] Py：命令行参数解析
来源：http://www.52xcode.cn/Article/details/gt3oiudmgai.html

ap = argparse.ArgumentParser();  ap.add_argument("--name");  args = ap.parse_args()
来源：http://www.ydjk.org.cn/Article/details/gt3ahobegmm.html

[U17] Py：初始化日志
来源：http://www.52xcode.cn/Article/details/gt3zeepewla.html

logging.basicConfig(level=logging.INFO)
来源：http://www.52xcode.cn/Article/details/gt3svgcczxd.html

[U18] Py：预编译正则
来源：http://www.52xcode.cn/Article/details/gt3cwzzpzij.html

pat = re.compile(r"\d+")
来源：http://www.ydjk.org.cn/Article/details/gt3uaagtwnm.html

[U19] Py：正则替换带回调
来源：http://www.ydjk.org.cn/Article/details/gt3bcgulabj.html

re.sub(r"\d+", lambda m: str(int(m.group()) * 2), s)
来源：http://www.52xcode.cn/Article/details/gt3ojgaznde.html

[U20] Py：缓存函数结果
来源：http://www.ydjk.org.cn/Article/details/gt3gyuktfad.html

@functools.lru_cache(maxsize=None)
来源：http://www.52xcode.cn/Article/details/gt3ovsvuzmh.html

[U21] Py：自定义上下文管理器
来源：http://www.ydjk.org.cn/Article/details/gt3wnpxuguo.html

@contextlib.contextmanager
来源：http://www.ydjk.org.cn/Article/details/gt3bjhczasd.html

[U22] Py：矩阵转置
来源：http://www.ydjk.org.cn/Article/details/gt3ibpyeica.html

list(zip(*m))
来源：http://www.ydjk.org.cn/Article/details/gt3bkbcehcb.html

[U23] Py：分块读取大文件
来源：http://www.52xcode.cn/Article/details/gt3ndhdtekd.html

for chunk in iter(lambda: f.read(8192), b""):
来源：http://www.ydjk.org.cn/Article/details/gt3sjxfytgf.html

[U24] Py：路径操作
来源：http://www.ydjk.org.cn/Article/details/gt3shkusdum.html

Path("a/b.txt").parent.mkdir(parents=True, exist_ok=True)
来源：http://www.52xcode.cn/Article/details/gt3qqxbcfzu.html

[U25] Py：CSV 按字典读
来源：http://www.52xcode.cn/Article/details/gt3tdsbcldq.html

csv.DictReader(f)
来源：http://www.ydjk.org.cn/Article/details/gt3ehwrojce.html

[U26] Py：并发下载
来源：http://www.52xcode.cn/Article/details/gt3qewxtkvh.html

ThreadPoolExecutor(max_workers=8).map(fetch, urls)
来源：http://www.52xcode.cn/Article/details/gt3bwcucjzb.html

[U27] Py：异步 HTTP
来源：http://www.52xcode.cn/Article/details/gt3lcwyebrb.html

aiohttp.ClientSession() 配合 async with
来源：http://www.ydjk.org.cn/Article/details/gt3becmutfi.html

[U28] Py：类型别名
来源：http://www.52xcode.cn/Article/details/gt3aesxqpxx.html

UserId = int
来源：http://www.52xcode.cn/Article/details/gt3imbeakli.html

[U29] Py：属性校验
来源：http://www.ydjk.org.cn/Article/details/gt3skigwlqm.html

@property 与 @x.setter 配合
来源：http://www.52xcode.cn/Article/details/gt3dxbrhlyr.html

[U30] Py：数据类
来源：http://www.ydjk.org.cn/Article/details/gt3xbwxhboc.html

@dataclass(slots=True)
来源：http://www.ydjk.org.cn/Article/details/gt3xjmxdsgx.html

[U31] Py：单测
来源：http://www.52xcode.cn/Article/details/gt3wpyxufod.html

python -m pytest -q
来源：http://www.ydjk.org.cn/Article/details/gt3olrsikuu.html

[U32] Py：代码格式化
来源：http://www.ydjk.org.cn/Article/details/gt3mnvhqurw.html

ruff format . && ruff check --fix .
来源：http://www.ydjk.org.cn/Article/details/gt3rgrswdyq.html

[U33] Py：打包发布
来源：http://www.52xcode.cn/Article/details/gt3cyjgmrmq.html

python -m build  （依赖 pyproject.toml）
来源：http://www.52xcode.cn/Article/details/gt3ujgauadd.html

[U34] Py：判断编码
来源：http://www.ydjk.org.cn/Article/details/gt3ykwtzpjq.html

chardet.detect(raw)
来源：http://www.52xcode.cn/Article/details/gt3lgoadduv.html

[U35] Py：发送邮件
来源：http://www.ydjk.org.cn/Article/details/gt3pwtecbni.html

smtplib.SMTP_SSL(...).send_message(msg)
来源：http://www.52xcode.cn/Article/details/gt3mctwxvxv.html

[U36] Py：定时任务
来源：http://www.52xcode.cn/Article/details/gt3nnvlgdsz.html

schedule.every(10).minutes.do(job)
来源：http://www.52xcode.cn/Article/details/gt3oretihxg.html

[U37] Py：读写 Excel
来源：http://www.52xcode.cn/Article/details/gt3nbxdqyeo.html

pandas.read_excel / DataFrame.to_excel
来源：http://www.52xcode.cn/Article/details/gt3zwiwgtkq.html

[U38] Py：获取脚本所在目录
来源：http://www.ydjk.org.cn/Article/details/gt3ptxtxpux.html

Path(__file__).resolve().parent
来源：http://www.52xcode.cn/Article/details/gt3qtxusutp.html

[U39] Py：判断是否在交互环境
来源：http://www.52xcode.cn/Article/details/gt3juhggyhb.html

sys.stdout.isatty()
来源：http://www.52xcode.cn/Article/details/gt3oyizjftv.html

[U40] Py：打印到标准错误
来源：http://www.ydjk.org.cn/Article/details/gt3uextyazs.html

print("err", file=sys.stderr)
来源：http://www.52xcode.cn/Article/details/gt3ezbvexqu.html

[U41] PHP：初始化 Composer 项目
来源：http://www.ydjk.org.cn/Article/details/gt3utpnlgig.html

composer init;  composer require guzzlehttp/guzzle
来源：http://www.ydjk.org.cn/Article/details/gt3znwgmrii.html

[U42] PHP：PSR-4 自动加载
来源：http://www.ydjk.org.cn/Article/details/gt3tyvaotae.html

"autoload": { "psr-4": { "App\\": "src/" } }
来源：http://www.ydjk.org.cn/Article/details/gt3notzzzyh.html

[U43] PHP：声明命名空间
来源：http://www.52xcode.cn/Article/details/gt3nkrkpbft.html

namespace App\Http;
来源：http://www.ydjk.org.cn/Article/details/gt3yhikhnwg.html

[U44] PHP：开启严格类型
来源：http://www.ydjk.org.cn/Article/details/gt3yqbdxidt.html

declare(strict_types=1);
来源：http://www.ydjk.org.cn/Article/details/gt3ntoffzvs.html

[U45] PHP：类型声明与返回类型
来源：http://www.ydjk.org.cn/Article/details/gt3moyoloao.html

function add(int $a, int $b): int { return $a + $b; }
来源：http://www.ydjk.org.cn/Article/details/gt3zdnrftzo.html

[U46] PHP：可空类型
来源：http://www.ydjk.org.cn/Article/details/gt3kpspfdcy.html

?string $name = null
来源：http://www.ydjk.org.cn/Article/details/gt3txurkdhi.html

[U47] PHP：联合类型
来源：http://www.ydjk.org.cn/Article/details/gt3uucvmhsf.html

int|string $id
来源：http://www.ydjk.org.cn/Article/details/gt3oghztayu.html

[U48] PHP：纯枚举
来源：http://www.ydjk.org.cn/Article/details/gt3swqiofzj.html

enum Status: string { case Active = "active"; case Off = "off"; }
来源：http://www.ydjk.org.cn/Article/details/gt3akstclsq.html

[U49] PHP：只读属性
来源：http://www.ydjk.org.cn/Article/details/gt3xvmiboqd.html

public readonly string $name
来源：http://www.ydjk.org.cn/Article/details/gt3ozeocoqp.html

[U50] PHP：构造器属性提升
来源：http://www.52xcode.cn/Article/details/gt3nafmhilt.html

public function __construct(private int $id) {}
来源：http://www.ydjk.org.cn/Article/details/gt3ebmmdctp.html

[U51] PHP：数组解构
来源：http://www.52xcode.cn/Article/details/gt3vpkncslg.html

[$a, $b] = $arr;
来源：http://www.52xcode.cn/Article/details/gt3dzpabmhc.html

[U52] PHP：箭头函数
来源：http://www.52xcode.cn/Article/details/gt3cdbgmrkq.html

$double = fn($x) => $x * 2;
来源：http://www.ydjk.org.cn/Article/details/gt3bpszxatm.html

[U53] PHP：空合并运算符
来源：http://www.52xcode.cn/Article/details/gt3fkxwrcig.html

$v = $a ?? $b ?? "default";
来源：http://www.52xcode.cn/Article/details/gt3wjnvlqir.html

[U54] PHP：空安全调用
来源：http://www.ydjk.org.cn/Article/details/gt3rozmhtdd.html

$obj?->method()
来源：http://www.52xcode.cn/Article/details/gt3vzioclrv.html

[U55] PHP：match 表达式
来源：http://www.52xcode.cn/Article/details/gt3lfjuqhkq.html

$s = match($x) { 1 => "一", default => "其他" };
来源：http://www.52xcode.cn/Article/details/gt3rqrqwlvh.html

[U56] PHP：命名参数
来源：http://www.ydjk.org.cn/Article/details/gt3biqsksln.html

f(a: 1, b: 2)
来源：http://www.52xcode.cn/Article/details/gt3csusvbot.html

[U57] PHP：字符串插值
来源：http://www.ydjk.org.cn/Article/details/gt3ipswlxcj.html

"值: {$a}"
来源：http://www.52xcode.cn/Article/details/gt3bwowekao.html

[U58] PHP：数组三件套
来源：http://www.52xcode.cn/Article/details/gt3ditrrplf.html

array_map($f, $a);  array_filter($a, $f);  array_reduce($a, $f, 0);
来源：http://www.ydjk.org.cn/Article/details/gt3xsuvmrno.html

[U59] PHP：自定义排序
来源：http://www.ydjk.org.cn/Article/details/gt3bmhwwunq.html

usort($arr, fn($a, $b) => $a["age"] <=> $b["age"]);
来源：http://www.52xcode.cn/Article/details/gt3mkncgskp.html

[U60] PHP：JSON 编解码
来源：http://www.ydjk.org.cn/Article/details/gt3rhpmqqsh.html

json_encode($d, JSON_UNESCAPED_UNICODE);  json_decode($s, true);
来源：http://www.52xcode.cn/Article/details/gt3prcizieo.html

[U61] PHP：正则
来源：http://www.52xcode.cn/Article/details/gt3iwyvnbib.html

preg_match('/(\d+)/', $s, $m);  preg_replace('/\d+/', '#', $s);
来源：http://www.52xcode.cn/Article/details/gt3ihhxbifx.html

[U62] PHP：日期对象
来源：http://www.52xcode.cn/Article/details/gt3clpxksxq.html

(new DateTimeImmutable())->format("Y-m-d");
来源：http://www.ydjk.org.cn/Article/details/gt3vqimzady.html

[U63] PHP：文件读写
来源：http://www.52xcode.cn/Article/details/gt3frgoqbsv.html

file_get_contents($f);  file_put_contents($f, $data);
来源：http://www.52xcode.cn/Article/details/gt3wsxcmjru.html

[U64] PHP：目录遍历
来源：http://www.52xcode.cn/Article/details/gt3pkmouatt.html

glob("dir/*.php");  scandir("dir");
来源：http://www.52xcode.cn/Article/details/gt3stdcgsax.html

[U65] PHP：会话
来源：http://www.ydjk.org.cn/Article/details/gt3qitzlxje.html

session_start();  $_SESSION["uid"] = 1;
来源：http://www.ydjk.org.cn/Article/details/gt3gpxzplwb.html

[U66] PHP：设置 Cookie
来源：http://www.ydjk.org.cn/Article/details/gt3iujsnado.html

setcookie("token", $v, ["httponly" => true, "samesite" => "Lax"]);
来源：http://www.ydjk.org.cn/Article/details/gt3jdffzmzh.html

[U67] PHP：处理文件上传
来源：http://www.52xcode.cn/Article/details/gt3fijpnsrg.html

$_FILES["file"]["tmp_name"] 与 move_uploaded_file()
来源：http://www.52xcode.cn/Article/details/gt3qtnjlowe.html

[U68] PHP：PDO 连接
来源：http://www.ydjk.org.cn/Article/details/gt3lwnxtkls.html

$pdo = new PDO("mysql:host=localhost;dbname=app", "root", "");
来源：http://www.52xcode.cn/Article/details/gt3opzsqvvw.html

[U69] PHP：PDO 预处理
来源：http://www.ydjk.org.cn/Article/details/gt3swdyvfoc.html

$stmt = $pdo->prepare("SELECT * FROM users WHERE id = ?");  $stmt->execute([$id]);
来源：http://www.52xcode.cn/Article/details/gt3sybisxmb.html

[U70] PHP：PDO 事务
来源：http://www.52xcode.cn/Article/details/gt3pynsjzjc.html

$pdo->beginTransaction();  $pdo->commit();  $pdo->rollBack();
来源：http://www.ydjk.org.cn/Article/details/gt3lybsizmt.html

[U71] PHP：抛出异常
来源：http://www.ydjk.org.cn/Article/details/gt3vxjrwkcg.html

throw new RuntimeException("失败", 500);
来源：http://www.52xcode.cn/Article/details/gt3icrrmqbg.html

[U72] PHP：写错误日志
来源：http://www.52xcode.cn/Article/details/gt3gdwyzesd.html

error_log("失败: " . $e->getMessage());
来源：http://www.ydjk.org.cn/Article/details/gt3ruwfawup.html

[U73] PHP：读取 ini 配置
来源：http://www.52xcode.cn/Article/details/gt3rsfapzct.html

parse_ini_file("config.ini", true)
来源：http://www.52xcode.cn/Article/details/gt3anorivld.html

[U74] PHP：读取环境变量
来源：http://www.52xcode.cn/Article/details/gt3zzeemwxf.html

getenv("APP_ENV") ?: "production"
来源：http://www.52xcode.cn/Article/details/gt3cubgcqyw.html

[U75] PHP：依赖注入
来源：http://www.ydjk.org.cn/Article/details/gt3wiywndro.html

composer require psr/container
来源：http://www.ydjk.org.cn/Article/details/gt3rxyqcxzp.html

[U76] PHP：简单路由
来源：http://www.52xcode.cn/Article/details/gt3ezruwpwx.html

$path = parse_url($_SERVER["REQUEST_URI"], PHP_URL_PATH);
来源：http://www.ydjk.org.cn/Article/details/gt3xrmumxtb.html

[U77] PHP：模板渲染
来源：http://www.ydjk.org.cn/Article/details/gt3mokukzpg.html

composer require twig/twig
来源：http://www.52xcode.cn/Article/details/gt3gdngrghd.html

[U78] PHP：单元测试
来源：http://www.ydjk.org.cn/Article/details/gt3ogkgcfvi.html

composer require --dev phpunit/phpunit
来源：http://www.ydjk.org.cn/Article/details/gt3xnfcpugr.html

[U79] PHP：静态分析
来源：http://www.ydjk.org.cn/Article/details/gt3dzzeebtq.html

composer require --dev phpstan/phpstan
来源：http://www.52xcode.cn/Article/details/gt3tweqixbo.html

[U80] PHP：代码规范修复
来源：http://www.52xcode.cn/Article/details/gt3wtbtpnke.html

composer require --dev friendsofphp/php-cs-fixer
来源：http://www.52xcode.cn/Article/details/gt3potnofim.html

[U81] JS：初始化项目
来源：http://www.ydjk.org.cn/Article/details/gt3jdufqbml.html

npm init -y;  npm i express
来源：http://www.52xcode.cn/Article/details/gt3auokmldv.html

[U82] JS：package.json 脚本
来源：http://www.52xcode.cn/Article/details/gt3iuxrujou.html

"scripts": { "dev": "vite", "build": "vite build" }
来源：http://www.52xcode.cn/Article/details/gt3qpxmfqfs.html

[U83] JS：ES Module 导入导出
来源：http://www.52xcode.cn/Article/details/gt3rhsablgk.html

export const a = 1;  import { a } from "./m.js";
来源：http://www.ydjk.org.cn/Article/details/gt3rqzreenk.html

[U84] JS：CommonJS 写法
来源：http://www.ydjk.org.cn/Article/details/gt3fodzagkp.html

module.exports = { a };  const { a } = require("./m");
来源：http://www.ydjk.org.cn/Article/details/gt3yjgtcqfa.html

[U85] JS：可选链
来源：http://www.52xcode.cn/Article/details/gt3tumtwmep.html

a?.b?.c
来源：http://www.ydjk.org.cn/Article/details/gt3hjzmqczm.html

[U86] JS：空值合并
来源：http://www.52xcode.cn/Article/details/gt3dejicoyv.html

a ?? b
来源：http://www.52xcode.cn/Article/details/gt3czzcuarw.html

[U87] JS：解构默认值
来源：http://www.52xcode.cn/Article/details/gt3fiykmiug.html

const { a = 1, b = 2 } = obj;
来源：http://www.52xcode.cn/Article/details/gt3cvsrqecj.html

[U88] JS：对象展开合并
来源：http://www.52xcode.cn/Article/details/gt3qmcgbyld.html

{ ...a, ...b }
来源：http://www.ydjk.org.cn/Article/details/gt3wvyleaka.html

[U89] JS：数组去重
来源：http://www.ydjk.org.cn/Article/details/gt3hgezgfri.html

[...new Set(arr)]
来源：http://www.52xcode.cn/Article/details/gt3zasyatqz.html

[U90] JS：数字数组排序
来源：http://www.ydjk.org.cn/Article/details/gt3spxqhgld.html

[...arr].sort((a, b) => a - b)
来源：http://www.ydjk.org.cn/Article/details/gt3ryqiowcn.html

[U91] JS：对象键值遍历
来源：http://www.ydjk.org.cn/Article/details/gt3gtcqapyt.html

Object.entries(obj).forEach(([k, v]) => {});
来源：http://www.52xcode.cn/Article/details/gt3rhebbhxg.html

[U92] JS：深拷贝
来源：http://www.ydjk.org.cn/Article/details/gt3etiavcgs.html

structuredClone(obj)
来源：http://www.ydjk.org.cn/Article/details/gt3oshsvcyz.html

[U93] JS：模板字符串
来源：http://www.52xcode.cn/Article/details/gt3xvvjgesu.html

`共 ${n} 条`
来源：http://www.52xcode.cn/Article/details/gt3oyjqdgpa.html

[U94] JS：箭头函数
来源：http://www.ydjk.org.cn/Article/details/gt3fupioown.html

const double = x => x * 2;
来源：http://www.52xcode.cn/Article/details/gt3vwwsrrld.html

[U95] JS：Promise 包装
来源：http://www.ydjk.org.cn/Article/details/gt3leqxmwdr.html

new Promise((resolve, reject) => {})
来源：http://www.52xcode.cn/Article/details/gt3ozkmnzfy.html

[U96] JS：async/await 与异常
来源：http://www.ydjk.org.cn/Article/details/gt3wdrihqvo.html

try { const d = await f(); } catch (e) { console.error(e); }
来源：http://www.ydjk.org.cn/Article/details/gt3jontawqi.html

[U97] JS：并发请求
来源：http://www.ydjk.org.cn/Article/details/gt3mvfrtfug.html

await Promise.all(urls.map(u => fetch(u)))
来源：http://www.52xcode.cn/Article/details/gt3nzlzxuia.html

[U98] JS：fetch 带 JSON
来源：http://www.ydjk.org.cn/Article/details/gt3ximcpgfo.html

await fetch(url, { method: "POST", headers: { "Content-Type": "application/json" }, body: JSON.stringify(d) })
来源：http://www.ydjk.org.cn/Article/details/gt3acozbpbh.html

[U99] JS：事件监听
来源：http://www.ydjk.org.cn/Article/details/gt3tzhbgqws.html

el.addEventListener("click", e => {})
来源：http://www.ydjk.org.cn/Article/details/gt3cgenjokl.html

[U100] JS：DOM 查询
来源：http://www.52xcode.cn/Article/details/gt3svmyilso.html

document.querySelector(".item")
来源：http://www.52xcode.cn/Article/details/gt3mzzpojge.html

[U101] JS：classList 操作
来源：http://www.ydjk.org.cn/Article/details/gt3tikrqjns.html

el.classList.toggle("active")
来源：http://www.52xcode.cn/Article/details/gt3mbxardoj.html

[U102] JS：本地存储
来源：http://www.52xcode.cn/Article/details/gt3xnxyclwq.html

localStorage.setItem("k", JSON.stringify(v))
来源：http://www.52xcode.cn/Article/details/gt3yvwzvbyn.html

[U103] JS：定时器
来源：http://www.52xcode.cn/Article/details/gt3gqagqvfs.html

setTimeout(fn, 1000);  setInterval(fn, 1000);
来源：http://www.ydjk.org.cn/Article/details/gt3xxrzuqyb.html

[U104] JS：防抖
来源：http://www.52xcode.cn/Article/details/gt3kpmzpntv.html

const debounce = (fn, ms) => { let t; return (...a) => { clearTimeout(t); t = setTimeout(() => fn(...a), ms); }; };
来源：http://www.52xcode.cn/Article/details/gt3foygaeli.html

[U105] JS：节流
来源：http://www.ydjk.org.cn/Article/details/gt3mgvfujwy.html

const throttle = (fn, ms) => { let last = 0; return (...a) => { const n = Date.now(); if (n - last >= ms) { last = n; fn(...a); } }; };
来源：http://www.ydjk.org.cn/Article/details/gt3xbbgpmqn.html

[U106] JS：日期格式化
来源：http://www.52xcode.cn/Article/details/gt3pnhcysmd.html

new Intl.DateTimeFormat("zh-CN", { dateStyle: "medium" }).format(new Date())
来源：http://www.52xcode.cn/Article/details/gt3hfsymdqk.html

[U107] JS：数字千分位
来源：http://www.ydjk.org.cn/Article/details/gt3qkadruhq.html

new Intl.NumberFormat("en-US").format(1234567)
来源：http://www.52xcode.cn/Article/details/gt3bksrpwzc.html

[U108] JS：随机整数
来源：http://www.ydjk.org.cn/Article/details/gt3hxjoufsr.html

Math.floor(Math.random() * (max - min + 1)) + min
来源：http://www.ydjk.org.cn/Article/details/gt3fzxkmkfc.html

[U109] JS：数组分组
来源：http://www.52xcode.cn/Article/details/gt3jgcvrcdc.html

Object.groupBy(arr, x => x.type)
来源：http://www.52xcode.cn/Article/details/gt3szkzoofy.html

[U110] JS：数组分块
来源：http://www.52xcode.cn/Article/details/gt3gnkrrupy.html

arr.reduce((acc, x, i) => (i % size ? acc : [...acc, arr.slice(i, i + size)]), [])
来源：http://www.ydjk.org.cn/Article/details/gt3xfcioxnm.html

[U111] JS：对象转 Map
来源：http://www.ydjk.org.cn/Article/details/gt3zyzidwiy.html

new Map(Object.entries(obj))
来源：http://www.52xcode.cn/Article/details/gt3seupxztb.html

[U112] JS：字符串补位
来源：http://www.52xcode.cn/Article/details/gt3muifkjyg.html

"7".padStart(3, "0")
来源：http://www.52xcode.cn/Article/details/gt3tavgesut.html

[U113] JS：正则替换全部
来源：http://www.52xcode.cn/Article/details/gt3srulvkpe.html

s.replaceAll("a", "b")
来源：http://www.ydjk.org.cn/Article/details/gt3ldgwlugk.html

[U114] JS：JSON 深比较
来源：http://www.ydjk.org.cn/Article/details/gt3xmtojoux.html

JSON.stringify(a) === JSON.stringify(b)
来源：http://www.52xcode.cn/Article/details/gt3qmhgesjw.html

[U115] JS：生成 UUID
来源：http://www.ydjk.org.cn/Article/details/gt3qpjttcel.html

crypto.randomUUID()
来源：http://www.ydjk.org.cn/Article/details/gt3uiyyeano.html

[U116] JS：类型检查（JSDoc）
来源：http://www.52xcode.cn/Article/details/gt3lbxxxsku.html

/** @param {string} name */ function f(name) {}
来源：http://www.52xcode.cn/Article/details/gt3fbbtmvir.html

[U117] JS：单元测试
来源：http://www.52xcode.cn/Article/details/gt3etsapftd.html

npm i -D vitest;  npx vitest
来源：http://www.ydjk.org.cn/Article/details/gt3aywiuiff.html

[U118] JS：开发服务器
来源：http://www.ydjk.org.cn/Article/details/gt3lnvpwfth.html

npm i -D vite;  npx vite
来源：http://www.ydjk.org.cn/Article/details/gt3xocpqmpe.html

[U119] JS：生产构建
来源：http://www.52xcode.cn/Article/details/gt3oxjhbxiu.html

npx vite build
来源：http://www.52xcode.cn/Article/details/gt3rdfnkfry.html

[U120] JS：读取环境变量（Vite）
来源：http://www.ydjk.org.cn/Article/details/gt3cogujpfp.html

import.meta.env.VITE_API_URL
来源：http://www.52xcode.cn/Article/details/gt3nnltqlaq.html

================================================================================
来源：http://www.ydjk.org.cn/Article/details/gt3katsmkfh.html

统计汇总
来源：http://www.ydjk.org.cn/Article/details/gt3dtkvhcpx.html

================================================================================
来源：http://www.52xcode.cn/Article/details/gt3qbvvcvxe.html

按语言统计（条）：
来源：http://www.52xcode.cn/Article/details/gt3yuohkeoe.html

Python ......... 252
来源：http://www.52xcode.cn/Article/details/gt3iokpmalj.html

PHP ............ 252
来源：http://www.ydjk.org.cn/Article/details/gt3nblbbghj.html

JavaScript ..... 252
来源：http://www.ydjk.org.cn/Article/details/gt3optzrwhz.html

TypeScript ..... 212
来源：http://www.ydjk.org.cn/Article/details/gt3sdrrmcep.html

Java ........... 212
来源：http://www.ydjk.org.cn/Article/details/gt3clatdxuo.html

Go ............. 212
来源：http://www.ydjk.org.cn/Article/details/gt3zzqghhew.html

Ruby ........... 212
来源：http://www.52xcode.cn/Article/details/gt3nrukkelx.html

C# ............. 212
来源：http://www.ydjk.org.cn/Article/details/gt3azndixzn.html

C .............. 30
来源：http://www.52xcode.cn/Article/details/gt3mdqdkwhn.html

C++ ............ 30
来源：http://www.ydjk.org.cn/Article/details/gt3gslhelxi.html

SQL ............ 90
来源：http://www.ydjk.org.cn/Article/details/gt3cjjokbcx.html

Bash ........... 80
来源：http://www.ydjk.org.cn/Article/details/gt3wjfxkxdp.html

Kotlin ......... 15
来源：http://www.52xcode.cn/Article/details/gt3gqjymywx.html

Swift .......... 15
来源：http://www.ydjk.org.cn/Article/details/gt3fcsnlffl.html

Lua ............ 10
来源：http://www.52xcode.cn/Article/details/gt3zewltdku.html

Perl ........... 10
来源：http://www.ydjk.org.cn/Article/details/gt3yhpxcheu.html

Scala .......... 10
来源：http://www.ydjk.org.cn/Article/details/gt3bouobzsu.html

------------------------------------
来源：http://www.ydjk.org.cn/Article/details/gt3pnobbwup.html

合计 ........... 2106 条
来源：http://www.ydjk.org.cn/Article/details/gt3jiblvkvd.html

按章节统计：
来源：http://www.52xcode.cn/Article/details/gt3tszuscpb.html

A 基础语法与类型       26 个任务 × 8 语言 =  208
来源：http://www.52xcode.cn/Article/details/gt3ikhrzflh.html

B 流程控制             16 个任务 × 8 语言 =  128
来源：http://www.52xcode.cn/Article/details/gt3qombuetb.html

C 函数与作用域         16 个任务 × 8 语言 =  128
来源：http://www.ydjk.org.cn/Article/details/gt3xfhzaqdy.html

D 数组 / 列表 / 集合   26 个任务 × 8 语言 =  208
来源：http://www.ydjk.org.cn/Article/details/gt3klkfkang.html

E 字符串处理           22 个任务 × 8 语言 =  176
来源：http://www.52xcode.cn/Article/details/gt3sydldndv.html

F 文件与目录           12 个任务 × 8 语言 =   96
来源：http://www.ydjk.org.cn/Article/details/gt3bmzevmwl.html

G 面向对象             16 个任务 × 8 语言 =  128
来源：http://www.52xcode.cn/Article/details/gt3btlevpec.html

H 异常与错误处理       10 个任务 × 8 语言 =   80
来源：http://www.52xcode.cn/Article/details/gt3liqcnytw.html

I 正则表达式            8 个任务 × 8 语言 =   64
来源：http://www.52xcode.cn/Article/details/gt3admdfufq.html

J 日期与时间           10 个任务 × 8 语言 =   80
来源：http://www.52xcode.cn/Article/details/gt3uvgfamya.html

K JSON 与序列化         8 个任务 × 8 语言 =   64
来源：http://www.ydjk.org.cn/Article/details/gt3xayfbykb.html

L 网络请求              8 个任务 × 8 语言 =   64
来源：http://www.52xcode.cn/Article/details/gt3yqsdwhns.html

M 命令行 / 进程         8 个任务 × 8 语言 =   64
来源：http://www.ydjk.org.cn/Article/details/gt3ohnnedtl.html

N 数据结构与算法       12 个任务 × 8 语言 =   96
来源：http://www.52xcode.cn/Article/details/gt3mfwfdkts.html

O 并发与异步            6 个任务 × 8 语言 =   48
来源：http://www.ydjk.org.cn/Article/details/gt3lypxdfmw.html

P 常用工具函数          8 个任务 × 8 语言 =   64
来源：http://www.52xcode.cn/Article/details/gt3ixjcmuka.html

Q SQL 专题                              90
来源：http://www.52xcode.cn/Article/details/gt3bnhwtzec.html

R Bash 专题                             80
来源：http://www.ydjk.org.cn/Article/details/gt3ebqyhtlk.html

S C / C++ 专题                          60
来源：http://www.52xcode.cn/Article/details/gt3swpnyvjh.html

T 其他语言补充                          60
来源：http://www.ydjk.org.cn/Article/details/gt3ienhxyxw.html

U 高频实用片段                         120
来源：http://www.52xcode.cn/Article/details/gt3xhuktuyf.html

------------------------------------
来源：http://www.52xcode.cn/Article/details/gt3kiznetpn.html

合计                                  2106 条
来源：http://www.ydjk.org.cn/Article/details/gt3wbbvvjnc.html

--------------------------------------------------------------------------------
来源：http://www.ydjk.org.cn/Article/details/gt3tnkfewih.html

使用提醒
来源：http://www.ydjk.org.cn/Article/details/gt3vufjhvwc.html

--------------------------------------------------------------------------------
来源：http://www.ydjk.org.cn/Article/details/gt3ybiqhivn.html

1. 示例追求"最小可用"，正式项目中请补齐导入、错误处理与边界判断。
来源：http://www.52xcode.cn/Article/details/gt3dcexohmi.html

2. 涉及文件、网络、数据库的示例，注意资源释放与异常捕获。
来源：http://www.52xcode.cn/Article/details/gt3wjjbelha.html

3. 语言版本差异较大（如 Python 3.10 的 match、Java 17 的 record/switch 箭头），
来源：http://www.ydjk.org.cn/Article/details/gt3tnjnwuzj.html

在旧版本上使用前请先确认语法支持情况。
来源：http://www.52xcode.cn/Article/details/gt3ophnbsuz.html

4. 标注"手写"的条目是因为该语言缺少对应内置能力，实际项目中可引入成熟库。
来源：http://www.52xcode.cn/Article/details/gt3gwmnwmen.html

—— 文件结束 ——
来源：http://www.52xcode.cn/Article/details/gt3scymkfus.html

================================================================================
来源：http://www.52xcode.cn/Article/details/gt3znprtxtg.html

程序语言常见例子速查手册（2024 版）
来源：http://www.ydjk.org.cn/Article/details/gt3owqbcaeq.html

Common Programming Examples Cheat Book
来源：http://www.52xcode.cn/Article/details/gt3fwytpnxk.html

================================================================================
来源：http://www.52xcode.cn/Article/details/gt3ztghabuv.html

【收录内容】
来源：http://www.ydjk.org.cn/Article/details/gt3nwqnmbai.html

覆盖 12 种语言 / 语法与常见 API：
来源：http://www.52xcode.cn/Article/details/gt3lynpelsn.html

Python · PHP · JavaScript · TypeScript · Java · Go · Ruby · C#
来源：http://www.52xcode.cn/Article/details/gt3notpzyaq.html

SQL · Bash · C · C++
来源：http://www.ydjk.org.cn/Article/details/gt3igoxvrgs.html

按「任务」分组：每个任务下按语言各给出一条最小可用示例。
来源：http://www.52xcode.cn/Article/details/gt3peaudnse.html

【使用说明】
来源：http://www.ydjk.org.cn/Article/details/gt3jyugzzdm.html

1. 每个任务形如 "[编号] 任务名"，下面每行以语言标记开头：
来源：http://www.52xcode.cn/Article/details/gt3hjkhgiej.html

Py:    Python        PHP:   PHP           JS:    JavaScript
来源：http://www.52xcode.cn/Article/details/gt3cnkurpsm.html

TS:    TypeScript    Java:  Java          Go:    Go
来源：http://www.52xcode.cn/Article/details/gt3dahsbhps.html

Ruby:  Ruby          C#:    C#            SQL:   SQL
来源：http://www.ydjk.org.cn/Article/details/gt3bpocyigp.html

Bash:  Shell         C:     C             C++:   C++
来源：http://www.52xcode.cn/Article/details/gt3jvkqdncx.html

2. 示例只展示核心写法，刻意省略 import / require / include / using 等样板代码。
来源：http://www.52xcode.cn/Article/details/gt3peeoocou.html

需要完整可运行文件时，请自行补齐当前语言的导入语句。
来源：http://www.ydjk.org.cn/Article/details/gt3uodsvcax.html

3. 语法基准：Python 3.10+ / PHP 8.1+ / ES2020+ / TypeScript 5 / Java 17 /
来源：http://www.52xcode.cn/Article/details/gt3bnfbpmuw.html

Go 1.21+ / Ruby 3.x / C# 10+ / C17 / C++17。
来源：http://www.ydjk.org.cn/Article/details/gt3bggejssw.html

4. 检索建议：用编辑器或浏览器 Ctrl+F 搜关键词，如 "排序" "读取文件" "正则"。
来源：http://www.52xcode.cn/Article/details/gt3rmnguwtx.html

5. 标记为 "// 无" 表示该语言没有对应的一等语法，需用替代写法（示例给出替代方案）。
来源：http://www.ydjk.org.cn/Article/details/gt3lnnkhgbj.html

6. 符号 "⏎" 表示代码在此处换行（主要用于 Python 等强制缩进、无法压成一行的结构）。
来源：http://www.52xcode.cn/Article/details/gt3tnwbibxp.html

【文件统计】
来源：http://www.52xcode.cn/Article/details/gt3urowcctu.html

语言示例共 2106 条，分布见本文末尾的「统计汇总」。
来源：http://www.52xcode.cn/Article/details/gt3scpxcgne.html


<!-- 参考信息 -->