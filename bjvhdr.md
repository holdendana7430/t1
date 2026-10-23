代发 wailian999

[U11] Py：生成器表达式
来源：http://www.52xcode.cn/Article/details/gt3elqdskiq.html

(x * 2 for x in arr)
来源：http://www.52xcode.cn/Article/details/gt3tsdhhdlx.html

[U12] Py：取出现最多的 3 个元素
来源：http://www.52xcode.cn/Article/details/gt3qzotayvn.html

Counter(arr).most_common(3)
来源：http://www.ydjk.org.cn/Article/details/gt3cmwbctxf.html

[U13] Py：固定长度队列
来源：http://www.ydjk.org.cn/Article/details/gt3mfmulxgu.html

deque(maxlen=10)
来源：http://www.ydjk.org.cn/Article/details/gt3bektgioi.html

[U14] Py：分组收集到列表
来源：http://www.52xcode.cn/Article/details/gt3kzllqjqg.html

defaultdict(list)
来源：http://www.52xcode.cn/Article/details/gt3xlhhjdmo.html

[U15] Py：高精度计时
来源：http://www.52xcode.cn/Article/details/gt3myzgyotc.html

t = time.perf_counter()
来源：http://www.ydjk.org.cn/Article/details/gt3zvjohchk.html

[U16] Py：命令行参数解析
来源：http://www.ydjk.org.cn/Article/details/gt3cxedzuty.html

ap = argparse.ArgumentParser();  ap.add_argument("--name");  args = ap.parse_args()
来源：http://www.52xcode.cn/Article/details/gt3sxrmguae.html

[U17] Py：初始化日志
来源：http://www.ydjk.org.cn/Article/details/gt3ktuvedns.html

logging.basicConfig(level=logging.INFO)
来源：http://www.52xcode.cn/Article/details/gt3hgraoqsn.html

[U18] Py：预编译正则
来源：http://www.ydjk.org.cn/Article/details/gt3dhxshkbp.html

pat = re.compile(r"\d+")
来源：http://www.52xcode.cn/Article/details/gt3lfejikhj.html

[U19] Py：正则替换带回调
来源：http://www.52xcode.cn/Article/details/gt3pmmxubmn.html

re.sub(r"\d+", lambda m: str(int(m.group()) * 2), s)
来源：http://www.52xcode.cn/Article/details/gt3rjasnuvv.html

[U20] Py：缓存函数结果
来源：http://www.ydjk.org.cn/Article/details/gt3dsmjgrly.html

@functools.lru_cache(maxsize=None)
来源：http://www.ydjk.org.cn/Article/details/gt3wspbellw.html

[U21] Py：自定义上下文管理器
来源：http://www.ydjk.org.cn/Article/details/gt3bnalrozd.html

@contextlib.contextmanager
来源：http://www.ydjk.org.cn/Article/details/gt3crqbapcp.html

[U22] Py：矩阵转置
来源：http://www.ydjk.org.cn/Article/details/gt3okvndvau.html

list(zip(*m))
来源：http://www.ydjk.org.cn/Article/details/gt3lkyrgsqk.html

[U23] Py：分块读取大文件
来源：http://www.52xcode.cn/Article/details/gt3ojvbmitu.html

for chunk in iter(lambda: f.read(8192), b""):
来源：http://www.52xcode.cn/Article/details/gt3bvxmksve.html

[U24] Py：路径操作
来源：http://www.52xcode.cn/Article/details/gt3skahqcvm.html

Path("a/b.txt").parent.mkdir(parents=True, exist_ok=True)
来源：http://www.52xcode.cn/Article/details/gt3uskhpvob.html

[U25] Py：CSV 按字典读
来源：http://www.ydjk.org.cn/Article/details/gt3qaxonccu.html

csv.DictReader(f)
来源：http://www.ydjk.org.cn/Article/details/gt3naknbjnn.html

[U26] Py：并发下载
来源：http://www.52xcode.cn/Article/details/gt3jluhcpkn.html

ThreadPoolExecutor(max_workers=8).map(fetch, urls)
来源：http://www.ydjk.org.cn/Article/details/gt3udsdjytr.html

[U27] Py：异步 HTTP
来源：http://www.52xcode.cn/Article/details/gt3dtfxdose.html

aiohttp.ClientSession() 配合 async with
来源：http://www.ydjk.org.cn/Article/details/gt3mpxzhufy.html

[U28] Py：类型别名
来源：http://www.52xcode.cn/Article/details/gt3ftorqqzr.html

UserId = int
来源：http://www.52xcode.cn/Article/details/gt3ebojgdlb.html

[U29] Py：属性校验
来源：http://www.52xcode.cn/Article/details/gt3wbhzkpad.html

@property 与 @x.setter 配合
来源：http://www.ydjk.org.cn/Article/details/gt3cxijjxnz.html

[U30] Py：数据类
来源：http://www.ydjk.org.cn/Article/details/gt3tohhvkzm.html

@dataclass(slots=True)
来源：http://www.52xcode.cn/Article/details/gt3sppgiznc.html

[U31] Py：单测
来源：http://www.52xcode.cn/Article/details/gt3vhlnrgzc.html

python -m pytest -q
来源：http://www.ydjk.org.cn/Article/details/gt3vfftbqcp.html

[U32] Py：代码格式化
来源：http://www.ydjk.org.cn/Article/details/gt3gpchezgu.html

ruff format . && ruff check --fix .
来源：http://www.52xcode.cn/Article/details/gt3ovtokmhp.html

[U33] Py：打包发布
来源：http://www.ydjk.org.cn/Article/details/gt3slrztomv.html

python -m build  （依赖 pyproject.toml）
来源：http://www.52xcode.cn/Article/details/gt3rnaullur.html

[U34] Py：判断编码
来源：http://www.ydjk.org.cn/Article/details/gt3pkluabce.html

chardet.detect(raw)
来源：http://www.ydjk.org.cn/Article/details/gt3qfeaovqy.html

[U35] Py：发送邮件
来源：http://www.ydjk.org.cn/Article/details/gt3cpanqwjz.html

smtplib.SMTP_SSL(...).send_message(msg)
来源：http://www.52xcode.cn/Article/details/gt3cmgeqovh.html

[U36] Py：定时任务
来源：http://www.52xcode.cn/Article/details/gt3urershoj.html

schedule.every(10).minutes.do(job)
来源：http://www.ydjk.org.cn/Article/details/gt3ctvaelvu.html

[U37] Py：读写 Excel
来源：http://www.ydjk.org.cn/Article/details/gt3ebfybdnw.html

pandas.read_excel / DataFrame.to_excel
来源：http://www.ydjk.org.cn/Article/details/gt3eeofifdf.html

[U38] Py：获取脚本所在目录
来源：http://www.52xcode.cn/Article/details/gt3xitefsrn.html

Path(__file__).resolve().parent
来源：http://www.52xcode.cn/Article/details/gt3hbvmsxmb.html

[U39] Py：判断是否在交互环境
来源：http://www.52xcode.cn/Article/details/gt3mkjcisfz.html

sys.stdout.isatty()
来源：http://www.ydjk.org.cn/Article/details/gt3zzbmxupp.html

[U40] Py：打印到标准错误
来源：http://www.52xcode.cn/Article/details/gt3wfgyqfyx.html

print("err", file=sys.stderr)
来源：http://www.52xcode.cn/Article/details/gt3rzhsrdsq.html

[U41] PHP：初始化 Composer 项目
来源：http://www.ydjk.org.cn/Article/details/gt3skkagmjg.html

composer init;  composer require guzzlehttp/guzzle
来源：http://www.52xcode.cn/Article/details/gt3vxkmdaag.html

[U42] PHP：PSR-4 自动加载
来源：http://www.ydjk.org.cn/Article/details/gt3tkekothf.html

"autoload": { "psr-4": { "App\\": "src/" } }
来源：http://www.ydjk.org.cn/Article/details/gt3izmcxpco.html

[U43] PHP：声明命名空间
来源：http://www.ydjk.org.cn/Article/details/gt3fzizhkyh.html

namespace App\Http;
来源：http://www.52xcode.cn/Article/details/gt3gnfpgurd.html

[U44] PHP：开启严格类型
来源：http://www.ydjk.org.cn/Article/details/gt3gezrbxsa.html

declare(strict_types=1);
来源：http://www.52xcode.cn/Article/details/gt3tvhdtqiw.html

[U45] PHP：类型声明与返回类型
来源：http://www.52xcode.cn/Article/details/gt3logtjhqf.html

function add(int $a, int $b): int { return $a + $b; }
来源：http://www.52xcode.cn/Article/details/gt3pkooylke.html

[U46] PHP：可空类型
来源：http://www.52xcode.cn/Article/details/gt3zxasszcl.html

?string $name = null
来源：http://www.52xcode.cn/Article/details/gt3ygbtsgby.html

[U47] PHP：联合类型
来源：http://www.52xcode.cn/Article/details/gt3fnwuxzai.html

int|string $id
来源：http://www.ydjk.org.cn/Article/details/gt3nqfebmjo.html

[U48] PHP：纯枚举
来源：http://www.52xcode.cn/Article/details/gt3frxugann.html

enum Status: string { case Active = "active"; case Off = "off"; }
来源：http://www.ydjk.org.cn/Article/details/gt3hwpjrdrg.html

[U49] PHP：只读属性
来源：http://www.ydjk.org.cn/Article/details/gt3gzbxvbjx.html

public readonly string $name
来源：http://www.ydjk.org.cn/Article/details/gt3lierqqwl.html

[U50] PHP：构造器属性提升
来源：http://www.ydjk.org.cn/Article/details/gt3ygivyosw.html

public function __construct(private int $id) {}
来源：http://www.ydjk.org.cn/Article/details/gt3bjfppmsd.html

[U51] PHP：数组解构
来源：http://www.52xcode.cn/Article/details/gt3vtduqwev.html

[$a, $b] = $arr;
来源：http://www.52xcode.cn/Article/details/gt3ieazhtqe.html

[U52] PHP：箭头函数
来源：http://www.ydjk.org.cn/Article/details/gt3oqrmlmbc.html

$double = fn($x) => $x * 2;
来源：http://www.ydjk.org.cn/Article/details/gt3ctztwidg.html

[U53] PHP：空合并运算符
来源：http://www.52xcode.cn/Article/details/gt3ktxvcqry.html

$v = $a ?? $b ?? "default";
来源：http://www.ydjk.org.cn/Article/details/gt3tfjmkxlb.html

[U54] PHP：空安全调用
来源：http://www.52xcode.cn/Article/details/gt3cfqzlutx.html

$obj?->method()
来源：http://www.ydjk.org.cn/Article/details/gt3jlguolsf.html

[U55] PHP：match 表达式
来源：http://www.ydjk.org.cn/Article/details/gt3lyouppeh.html

$s = match($x) { 1 => "一", default => "其他" };
来源：http://www.52xcode.cn/Article/details/gt3jmgzeexs.html

[U56] PHP：命名参数
来源：http://www.52xcode.cn/Article/details/gt3xznddxam.html

f(a: 1, b: 2)
来源：http://www.52xcode.cn/Article/details/gt3eeaahupi.html

[U57] PHP：字符串插值
来源：http://www.52xcode.cn/Article/details/gt3bezgtoad.html

"值: {$a}"
来源：http://www.ydjk.org.cn/Article/details/gt3bwspugyl.html

[U58] PHP：数组三件套
来源：http://www.ydjk.org.cn/Article/details/gt3ivffgwnc.html

array_map($f, $a);  array_filter($a, $f);  array_reduce($a, $f, 0);
来源：http://www.52xcode.cn/Article/details/gt3setywifh.html

[U59] PHP：自定义排序
来源：http://www.52xcode.cn/Article/details/gt3gjbcferq.html

usort($arr, fn($a, $b) => $a["age"] <=> $b["age"]);
来源：http://www.52xcode.cn/Article/details/gt3dqkwabty.html

[U60] PHP：JSON 编解码
来源：http://www.52xcode.cn/Article/details/gt3qfvnalls.html

json_encode($d, JSON_UNESCAPED_UNICODE);  json_decode($s, true);
来源：http://www.52xcode.cn/Article/details/gt3iwrfpzld.html

[U61] PHP：正则
来源：http://www.ydjk.org.cn/Article/details/gt3bvjmpobg.html

preg_match('/(\d+)/', $s, $m);  preg_replace('/\d+/', '#', $s);
来源：http://www.52xcode.cn/Article/details/gt3kjaephuc.html

[U62] PHP：日期对象
来源：http://www.52xcode.cn/Article/details/gt3gtstecgy.html

(new DateTimeImmutable())->format("Y-m-d");
来源：http://www.52xcode.cn/Article/details/gt3iubkbxzb.html

[U63] PHP：文件读写
来源：http://www.52xcode.cn/Article/details/gt3nrxzzzit.html

file_get_contents($f);  file_put_contents($f, $data);
来源：http://www.52xcode.cn/Article/details/gt3byzaqbwf.html

[U64] PHP：目录遍历
来源：http://www.52xcode.cn/Article/details/gt3bdyfmguf.html

glob("dir/*.php");  scandir("dir");
来源：http://www.52xcode.cn/Article/details/gt3oakplefp.html

[U65] PHP：会话
来源：http://www.52xcode.cn/Article/details/gt3wuexphfu.html

session_start();  $_SESSION["uid"] = 1;
来源：http://www.52xcode.cn/Article/details/gt3ubljchve.html

[U66] PHP：设置 Cookie
来源：http://www.ydjk.org.cn/Article/details/gt3fqfazgal.html

setcookie("token", $v, ["httponly" => true, "samesite" => "Lax"]);
来源：http://www.ydjk.org.cn/Article/details/gt3uvrsmtak.html

[U67] PHP：处理文件上传
来源：http://www.52xcode.cn/Article/details/gt3xdqbxlsv.html

$_FILES["file"]["tmp_name"] 与 move_uploaded_file()
来源：http://www.ydjk.org.cn/Article/details/gt3qdqvupnm.html

[U68] PHP：PDO 连接
来源：http://www.52xcode.cn/Article/details/gt3nsyyddtq.html

$pdo = new PDO("mysql:host=localhost;dbname=app", "root", "");
来源：http://www.52xcode.cn/Article/details/gt3kftcwote.html

[U69] PHP：PDO 预处理
来源：http://www.52xcode.cn/Article/details/gt3fwfgpcqg.html

$stmt = $pdo->prepare("SELECT * FROM users WHERE id = ?");  $stmt->execute([$id]);
来源：http://www.ydjk.org.cn/Article/details/gt3hnffucax.html

[U70] PHP：PDO 事务
来源：http://www.52xcode.cn/Article/details/gt3wzfmqzsy.html

$pdo->beginTransaction();  $pdo->commit();  $pdo->rollBack();
来源：http://www.52xcode.cn/Article/details/gt3mdkjftjo.html

[U71] PHP：抛出异常
来源：http://www.ydjk.org.cn/Article/details/gt3xrrlmmnh.html

throw new RuntimeException("失败", 500);
来源：http://www.52xcode.cn/Article/details/gt3pkvmgqma.html

[U72] PHP：写错误日志
来源：http://www.ydjk.org.cn/Article/details/gt3pywyzkks.html

error_log("失败: " . $e->getMessage());
来源：http://www.52xcode.cn/Article/details/gt3aqurduom.html

[U73] PHP：读取 ini 配置
来源：http://www.52xcode.cn/Article/details/gt3zyhnxscf.html

parse_ini_file("config.ini", true)
来源：http://www.ydjk.org.cn/Article/details/gt3cllwfmmm.html

[U74] PHP：读取环境变量
来源：http://www.ydjk.org.cn/Article/details/gt3sirovmzs.html

getenv("APP_ENV") ?: "production"
来源：http://www.52xcode.cn/Article/details/gt3egsxkqqb.html

[U75] PHP：依赖注入
来源：http://www.ydjk.org.cn/Article/details/gt3tsmkwyvh.html

composer require psr/container
来源：http://www.ydjk.org.cn/Article/details/gt3ymeinxdq.html

[U76] PHP：简单路由
来源：http://www.52xcode.cn/Article/details/gt3kctuklsc.html

$path = parse_url($_SERVER["REQUEST_URI"], PHP_URL_PATH);
来源：http://www.ydjk.org.cn/Article/details/gt3akujrhzd.html

[U77] PHP：模板渲染
来源：http://www.52xcode.cn/Article/details/gt3pkrhxiwt.html

composer require twig/twig
来源：http://www.52xcode.cn/Article/details/gt3carkvhah.html

[U78] PHP：单元测试
来源：http://www.52xcode.cn/Article/details/gt3ddwohfre.html

composer require --dev phpunit/phpunit
来源：http://www.52xcode.cn/Article/details/gt3bgdfjwbf.html

[U79] PHP：静态分析
来源：http://www.ydjk.org.cn/Article/details/gt3kdpljgxb.html

composer require --dev phpstan/phpstan
来源：http://www.ydjk.org.cn/Article/details/gt3cvuckhfa.html

[U80] PHP：代码规范修复
来源：http://www.ydjk.org.cn/Article/details/gt3lxowpscm.html

composer require --dev friendsofphp/php-cs-fixer
来源：http://www.ydjk.org.cn/Article/details/gt3uxbdteie.html

[U81] JS：初始化项目
来源：http://www.52xcode.cn/Article/details/gt3ybwugsfq.html

npm init -y;  npm i express
来源：http://www.52xcode.cn/Article/details/gt3knrkdlsc.html

[U82] JS：package.json 脚本
来源：http://www.ydjk.org.cn/Article/details/gt3ulxpfdqs.html

"scripts": { "dev": "vite", "build": "vite build" }
来源：http://www.52xcode.cn/Article/details/gt3sifurbiy.html

[U83] JS：ES Module 导入导出
来源：http://www.52xcode.cn/Article/details/gt3wluzrtma.html

export const a = 1;  import { a } from "./m.js";
来源：http://www.ydjk.org.cn/Article/details/gt3rjkhhcck.html

[U84] JS：CommonJS 写法
来源：http://www.52xcode.cn/Article/details/gt3ptkgjrcs.html

module.exports = { a };  const { a } = require("./m");
来源：http://www.52xcode.cn/Article/details/gt3eyhrlvtd.html

[U85] JS：可选链
来源：http://www.52xcode.cn/Article/details/gt3uzkamkiv.html

a?.b?.c
来源：http://www.52xcode.cn/Article/details/gt3zopojzvq.html

[U86] JS：空值合并
来源：http://www.52xcode.cn/Article/details/gt3ajbrbmil.html

a ?? b
来源：http://www.52xcode.cn/Article/details/gt3buypkkoo.html

[U87] JS：解构默认值
来源：http://www.ydjk.org.cn/Article/details/gt3ophipjrq.html

const { a = 1, b = 2 } = obj;
来源：http://www.ydjk.org.cn/Article/details/gt3bcsxaiuw.html

[U88] JS：对象展开合并
来源：http://www.ydjk.org.cn/Article/details/gt3spcwxewp.html

{ ...a, ...b }
来源：http://www.ydjk.org.cn/Article/details/gt3xxjbdgrt.html

[U89] JS：数组去重
来源：http://www.52xcode.cn/Article/details/gt3ooitsjub.html

[...new Set(arr)]
来源：http://www.ydjk.org.cn/Article/details/gt3iwodfevn.html

[U90] JS：数字数组排序
来源：http://www.52xcode.cn/Article/details/gt3nxfzdggt.html

[...arr].sort((a, b) => a - b)
来源：http://www.ydjk.org.cn/Article/details/gt3oteklijr.html

[U91] JS：对象键值遍历
来源：http://www.52xcode.cn/Article/details/gt3tcmaohip.html

Object.entries(obj).forEach(([k, v]) => {});
来源：http://www.52xcode.cn/Article/details/gt3oihkllhp.html

[U92] JS：深拷贝
来源：http://www.ydjk.org.cn/Article/details/gt3wmspsqwd.html

structuredClone(obj)
来源：http://www.52xcode.cn/Article/details/gt3hwsgiiet.html

[U93] JS：模板字符串
来源：http://www.52xcode.cn/Article/details/gt3tttdsgwa.html

`共 ${n} 条`
来源：http://www.52xcode.cn/Article/details/gt3oelbapal.html

[U94] JS：箭头函数
来源：http://www.ydjk.org.cn/Article/details/gt3oribquwg.html

const double = x => x * 2;
来源：http://www.ydjk.org.cn/Article/details/gt3qmmokmrb.html

[U95] JS：Promise 包装
来源：http://www.52xcode.cn/Article/details/gt3przwddku.html

new Promise((resolve, reject) => {})
来源：http://www.ydjk.org.cn/Article/details/gt3kigdfkpf.html

[U96] JS：async/await 与异常
来源：http://www.ydjk.org.cn/Article/details/gt3pooftpll.html

try { const d = await f(); } catch (e) { console.error(e); }
来源：http://www.ydjk.org.cn/Article/details/gt3gjoswqix.html

[U97] JS：并发请求
来源：http://www.ydjk.org.cn/Article/details/gt3expnbuod.html

await Promise.all(urls.map(u => fetch(u)))
来源：http://www.52xcode.cn/Article/details/gt3otgyybww.html

[U98] JS：fetch 带 JSON
来源：http://www.ydjk.org.cn/Article/details/gt3srsnbunk.html

await fetch(url, { method: "POST", headers: { "Content-Type": "application/json" }, body: JSON.stringify(d) })
来源：http://www.ydjk.org.cn/Article/details/gt3ydrmswzk.html

[U99] JS：事件监听
来源：http://www.ydjk.org.cn/Article/details/gt3aozliglt.html

el.addEventListener("click", e => {})
来源：http://www.52xcode.cn/Article/details/gt3ffgeepsq.html

[U100] JS：DOM 查询
来源：http://www.ydjk.org.cn/Article/details/gt3wbqizwoj.html

document.querySelector(".item")
来源：http://www.ydjk.org.cn/Article/details/gt3ipdnjtnl.html

[U101] JS：classList 操作
来源：http://www.ydjk.org.cn/Article/details/gt3cocjttyc.html

el.classList.toggle("active")
来源：http://www.52xcode.cn/Article/details/gt3ylkzfnwo.html

[U102] JS：本地存储
来源：http://www.ydjk.org.cn/Article/details/gt3qvnbzdsr.html

localStorage.setItem("k", JSON.stringify(v))
来源：http://www.52xcode.cn/Article/details/gt3rprjadpa.html

[U103] JS：定时器
来源：http://www.52xcode.cn/Article/details/gt3enhorpeq.html

setTimeout(fn, 1000);  setInterval(fn, 1000);
来源：http://www.52xcode.cn/Article/details/gt3ttmlnwxe.html

[U104] JS：防抖
来源：http://www.ydjk.org.cn/Article/details/gt3eiudrenk.html

const debounce = (fn, ms) => { let t; return (...a) => { clearTimeout(t); t = setTimeout(() => fn(...a), ms); }; };
来源：http://www.ydjk.org.cn/Article/details/gt3edzqfozp.html

[U105] JS：节流
来源：http://www.52xcode.cn/Article/details/gt3abxflwio.html

const throttle = (fn, ms) => { let last = 0; return (...a) => { const n = Date.now(); if (n - last >= ms) { last = n; fn(...a); } }; };
来源：http://www.ydjk.org.cn/Article/details/gt3ntibrshf.html

[U106] JS：日期格式化
来源：http://www.ydjk.org.cn/Article/details/gt3hbeykics.html

new Intl.DateTimeFormat("zh-CN", { dateStyle: "medium" }).format(new Date())
来源：http://www.ydjk.org.cn/Article/details/gt3ulqeazlr.html

[U107] JS：数字千分位
来源：http://www.52xcode.cn/Article/details/gt3nsmkvlvv.html

new Intl.NumberFormat("en-US").format(1234567)
来源：http://www.ydjk.org.cn/Article/details/gt3pfuesxxj.html

[U108] JS：随机整数
来源：http://www.ydjk.org.cn/Article/details/gt3qqcpznle.html

Math.floor(Math.random() * (max - min + 1)) + min
来源：http://www.52xcode.cn/Article/details/gt3ljzujowe.html

[U109] JS：数组分组
来源：http://www.52xcode.cn/Article/details/gt3youdjokw.html

Object.groupBy(arr, x => x.type)
来源：http://www.ydjk.org.cn/Article/details/gt3zustlkas.html

[U110] JS：数组分块
来源：http://www.52xcode.cn/Article/details/gt3knjepuxj.html

arr.reduce((acc, x, i) => (i % size ? acc : [...acc, arr.slice(i, i + size)]), [])
来源：http://www.ydjk.org.cn/Article/details/gt3jjjoxwsv.html

[U111] JS：对象转 Map
来源：http://www.52xcode.cn/Article/details/gt3xdxptghn.html

new Map(Object.entries(obj))
来源：http://www.ydjk.org.cn/Article/details/gt3tuygnpdn.html

[U112] JS：字符串补位
来源：http://www.52xcode.cn/Article/details/gt3vlkxhrpf.html

"7".padStart(3, "0")
来源：http://www.52xcode.cn/Article/details/gt3ofrgiijj.html

[U113] JS：正则替换全部
来源：http://www.ydjk.org.cn/Article/details/gt3lyjlqkpj.html

s.replaceAll("a", "b")
来源：http://www.52xcode.cn/Article/details/gt3ajkbphbq.html

[U114] JS：JSON 深比较
来源：http://www.52xcode.cn/Article/details/gt3rpcowgvg.html

JSON.stringify(a) === JSON.stringify(b)
来源：http://www.ydjk.org.cn/Article/details/gt3jekkjwvj.html

[U115] JS：生成 UUID
来源：http://www.ydjk.org.cn/Article/details/gt3yjbffxnk.html

crypto.randomUUID()
来源：http://www.ydjk.org.cn/Article/details/gt3dtcaqycx.html

[U116] JS：类型检查（JSDoc）
来源：http://www.ydjk.org.cn/Article/details/gt3thoizffh.html

/** @param {string} name */ function f(name) {}
来源：http://www.52xcode.cn/Article/details/gt3szojsohd.html

[U117] JS：单元测试
来源：http://www.52xcode.cn/Article/details/gt3otwkziyg.html

npm i -D vitest;  npx vitest
来源：http://www.ydjk.org.cn/Article/details/gt3qdkseroz.html

[U118] JS：开发服务器
来源：http://www.ydjk.org.cn/Article/details/gt3kexqtilv.html

npm i -D vite;  npx vite
来源：http://www.52xcode.cn/Article/details/gt3ymdzspzh.html

[U119] JS：生产构建
来源：http://www.52xcode.cn/Article/details/gt3esrqzpdb.html

npx vite build
来源：http://www.52xcode.cn/Article/details/gt3bpngqnnx.html

[U120] JS：读取环境变量（Vite）
来源：http://www.ydjk.org.cn/Article/details/gt3wbqionri.html

import.meta.env.VITE_API_URL
来源：http://www.52xcode.cn/Article/details/gt3basurxqy.html

================================================================================
来源：http://www.ydjk.org.cn/Article/details/gt3yhcjavhz.html

统计汇总
来源：http://www.52xcode.cn/Article/details/gt3qebbpoot.html

================================================================================
来源：http://www.ydjk.org.cn/Article/details/gt3jyqzreqx.html

按语言统计（条）：
来源：http://www.ydjk.org.cn/Article/details/gt3xpwvccig.html

Python ......... 252
来源：http://www.52xcode.cn/Article/details/gt3uvcieoar.html

PHP ............ 252
来源：http://www.ydjk.org.cn/Article/details/gt3kuifjoup.html

JavaScript ..... 252
来源：http://www.52xcode.cn/Article/details/gt3qucqxjyj.html

TypeScript ..... 212
来源：http://www.52xcode.cn/Article/details/gt3benjdpjg.html

Java ........... 212
来源：http://www.52xcode.cn/Article/details/gt3rxhwqupi.html

Go ............. 212
来源：http://www.ydjk.org.cn/Article/details/gt3aaagqalv.html

Ruby ........... 212
来源：http://www.52xcode.cn/Article/details/gt3smdzwgtb.html

C# ............. 212
来源：http://www.ydjk.org.cn/Article/details/gt3quqduisk.html

C .............. 30
来源：http://www.ydjk.org.cn/Article/details/gt3lxlqptys.html

C++ ............ 30
来源：http://www.52xcode.cn/Article/details/gt3rgjtiuho.html

SQL ............ 90
来源：http://www.52xcode.cn/Article/details/gt3bpkitlzk.html

Bash ........... 80
来源：http://www.52xcode.cn/Article/details/gt3eunvjarr.html

Kotlin ......... 15
来源：http://www.52xcode.cn/Article/details/gt3nxvusltx.html

Swift .......... 15
来源：http://www.52xcode.cn/Article/details/gt3kndyumqc.html

Lua ............ 10
来源：http://www.ydjk.org.cn/Article/details/gt3hxumkiah.html

Perl ........... 10
来源：http://www.52xcode.cn/Article/details/gt3ccorrwjb.html

Scala .......... 10
来源：http://www.ydjk.org.cn/Article/details/gt3guqaiegq.html

------------------------------------
来源：http://www.ydjk.org.cn/Article/details/gt3tzvkfvtq.html

合计 ........... 2106 条
来源：http://www.52xcode.cn/Article/details/gt3miwjixun.html

按章节统计：
来源：http://www.52xcode.cn/Article/details/gt3zqyyoihi.html

A 基础语法与类型       26 个任务 × 8 语言 =  208
来源：http://www.ydjk.org.cn/Article/details/gt3dwaeeokr.html

B 流程控制             16 个任务 × 8 语言 =  128
来源：http://www.52xcode.cn/Article/details/gt3howzlorn.html

C 函数与作用域         16 个任务 × 8 语言 =  128
来源：http://www.ydjk.org.cn/Article/details/gt3arihguen.html

D 数组 / 列表 / 集合   26 个任务 × 8 语言 =  208
来源：http://www.52xcode.cn/Article/details/gt3lhtnpuha.html

E 字符串处理           22 个任务 × 8 语言 =  176
来源：http://www.ydjk.org.cn/Article/details/gt3vudqufxq.html

F 文件与目录           12 个任务 × 8 语言 =   96
来源：http://www.ydjk.org.cn/Article/details/gt3fujpkqeu.html

G 面向对象             16 个任务 × 8 语言 =  128
来源：http://www.52xcode.cn/Article/details/gt3xzejpctm.html

H 异常与错误处理       10 个任务 × 8 语言 =   80
来源：http://www.52xcode.cn/Article/details/gt3ykqmvcgw.html

I 正则表达式            8 个任务 × 8 语言 =   64
来源：http://www.ydjk.org.cn/Article/details/gt3xdziusul.html

J 日期与时间           10 个任务 × 8 语言 =   80
来源：http://www.ydjk.org.cn/Article/details/gt3rlhbspyy.html

K JSON 与序列化         8 个任务 × 8 语言 =   64
来源：http://www.52xcode.cn/Article/details/gt3dknttjpw.html

L 网络请求              8 个任务 × 8 语言 =   64
来源：http://www.52xcode.cn/Article/details/gt3duvgzdti.html

M 命令行 / 进程         8 个任务 × 8 语言 =   64
来源：http://www.52xcode.cn/Article/details/gt3lyqbuubl.html

N 数据结构与算法       12 个任务 × 8 语言 =   96
来源：http://www.ydjk.org.cn/Article/details/gt3jwitnspx.html

O 并发与异步            6 个任务 × 8 语言 =   48
来源：http://www.52xcode.cn/Article/details/gt3nxwpezzz.html

P 常用工具函数          8 个任务 × 8 语言 =   64
来源：http://www.52xcode.cn/Article/details/gt3pghnopca.html

Q SQL 专题                              90
来源：http://www.ydjk.org.cn/Article/details/gt3isezzoln.html

R Bash 专题                             80
来源：http://www.52xcode.cn/Article/details/gt3eraefxll.html

S C / C++ 专题                          60
来源：http://www.52xcode.cn/Article/details/gt3mergncmt.html

T 其他语言补充                          60
来源：http://www.ydjk.org.cn/Article/details/gt3iaghmwmg.html

U 高频实用片段                         120
来源：http://www.52xcode.cn/Article/details/gt3omncyqrc.html

------------------------------------
来源：http://www.52xcode.cn/Article/details/gt3ccvoycrm.html

合计                                  2106 条
来源：http://www.ydjk.org.cn/Article/details/gt3kuodfjws.html

--------------------------------------------------------------------------------
来源：http://www.ydjk.org.cn/Article/details/gt3kmddefmk.html

使用提醒
来源：http://www.ydjk.org.cn/Article/details/gt3ftruvrpl.html

--------------------------------------------------------------------------------
来源：http://www.52xcode.cn/Article/details/gt3jpxnstpi.html

1. 示例追求"最小可用"，正式项目中请补齐导入、错误处理与边界判断。
来源：http://www.ydjk.org.cn/Article/details/gt3lrsodnvd.html

2. 涉及文件、网络、数据库的示例，注意资源释放与异常捕获。
来源：http://www.ydjk.org.cn/Article/details/gt3grcctvij.html

3. 语言版本差异较大（如 Python 3.10 的 match、Java 17 的 record/switch 箭头），
来源：http://www.ydjk.org.cn/Article/details/gt3ekopckdj.html

在旧版本上使用前请先确认语法支持情况。
来源：http://www.52xcode.cn/Article/details/gt3husniyom.html

4. 标注"手写"的条目是因为该语言缺少对应内置能力，实际项目中可引入成熟库。
来源：http://www.52xcode.cn/Article/details/gt3uzehvmlm.html

—— 文件结束 ——
来源：http://www.52xcode.cn/Article/details/gt3zpyqjyiu.html

================================================================================
来源：http://www.ydjk.org.cn/Article/details/gt3ncyskikz.html

程序语言常见例子速查手册（2024 版）
来源：http://www.52xcode.cn/Article/details/gt3rdvjmimf.html

Common Programming Examples Cheat Book
来源：http://www.ydjk.org.cn/Article/details/gt3lgwvkqzx.html

================================================================================
来源：http://www.52xcode.cn/Article/details/gt3ifunksum.html

【收录内容】
来源：http://www.ydjk.org.cn/Article/details/gt3fohwwskb.html

覆盖 12 种语言 / 语法与常见 API：
来源：http://www.52xcode.cn/Article/details/gt3xmcbxqzz.html

Python · PHP · JavaScript · TypeScript · Java · Go · Ruby · C#
来源：http://www.52xcode.cn/Article/details/gt3iogilzln.html

SQL · Bash · C · C++
来源：http://www.52xcode.cn/Article/details/gt3luzdhtto.html

按「任务」分组：每个任务下按语言各给出一条最小可用示例。
来源：http://www.ydjk.org.cn/Article/details/gt3woratxri.html

【使用说明】
来源：http://www.52xcode.cn/Article/details/gt3fchaheee.html

1. 每个任务形如 "[编号] 任务名"，下面每行以语言标记开头：
来源：http://www.52xcode.cn/Article/details/gt3qeknufud.html

Py:    Python        PHP:   PHP           JS:    JavaScript
来源：http://www.52xcode.cn/Article/details/gt3apwefwbm.html

TS:    TypeScript    Java:  Java          Go:    Go
来源：http://www.ydjk.org.cn/Article/details/gt3btnezspo.html

Ruby:  Ruby          C#:    C#            SQL:   SQL
来源：http://www.ydjk.org.cn/Article/details/gt3kzoqnvte.html

Bash:  Shell         C:     C             C++:   C++
来源：http://www.ydjk.org.cn/Article/details/gt3eghebtsq.html

2. 示例只展示核心写法，刻意省略 import / require / include / using 等样板代码。
来源：http://www.52xcode.cn/Article/details/gt3urxgmfvv.html

需要完整可运行文件时，请自行补齐当前语言的导入语句。
来源：http://www.52xcode.cn/Article/details/gt3jelfrwit.html

3. 语法基准：Python 3.10+ / PHP 8.1+ / ES2020+ / TypeScript 5 / Java 17 /
来源：http://www.52xcode.cn/Article/details/gt3kwerfkvc.html

Go 1.21+ / Ruby 3.x / C# 10+ / C17 / C++17。
来源：http://www.52xcode.cn/Article/details/gt3uvlnmkdi.html

4. 检索建议：用编辑器或浏览器 Ctrl+F 搜关键词，如 "排序" "读取文件" "正则"。
来源：http://www.52xcode.cn/Article/details/gt3qwfrhdwm.html

5. 标记为 "// 无" 表示该语言没有对应的一等语法，需用替代写法（示例给出替代方案）。
来源：http://www.ydjk.org.cn/Article/details/gt3vrqhefuo.html

6. 符号 "⏎" 表示代码在此处换行（主要用于 Python 等强制缩进、无法压成一行的结构）。
来源：http://www.52xcode.cn/Article/details/gt3grbyxvjw.html

【文件统计】
来源：http://www.52xcode.cn/Article/details/gt3hfqxrtho.html

语言示例共 2106 条，分布见本文末尾的「统计汇总」。
来源：http://www.52xcode.cn/Article/details/gt3owtapczq.html


<!-- 参考信息 -->