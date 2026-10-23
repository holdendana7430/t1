代发 wailian999

[U11] Py：生成器表达式
来源：http://www.52xcode.cn/Article/details/gt3jyxjsxkp.html

(x * 2 for x in arr)
来源：http://www.52xcode.cn/Article/details/gt3rivqajsq.html

[U12] Py：取出现最多的 3 个元素
来源：http://www.ydjk.org.cn/Article/details/gt3rgtesjgj.html

Counter(arr).most_common(3)
来源：http://www.52xcode.cn/Article/details/gt3lusdntfo.html

[U13] Py：固定长度队列
来源：http://www.ydjk.org.cn/Article/details/gt3wrenvact.html

deque(maxlen=10)
来源：http://www.ydjk.org.cn/Article/details/gt3bdbbyntv.html

[U14] Py：分组收集到列表
来源：http://www.52xcode.cn/Article/details/gt3oemzohfa.html

defaultdict(list)
来源：http://www.ydjk.org.cn/Article/details/gt3ohhspykl.html

[U15] Py：高精度计时
来源：http://www.ydjk.org.cn/Article/details/gt3pilcfmbe.html

t = time.perf_counter()
来源：http://www.ydjk.org.cn/Article/details/gt3jmfiziry.html

[U16] Py：命令行参数解析
来源：http://www.52xcode.cn/Article/details/gt3wxdrvhqy.html

ap = argparse.ArgumentParser();  ap.add_argument("--name");  args = ap.parse_args()
来源：http://www.52xcode.cn/Article/details/gt3itnbsqfg.html

[U17] Py：初始化日志
来源：http://www.ydjk.org.cn/Article/details/gt3icmgmrte.html

logging.basicConfig(level=logging.INFO)
来源：http://www.52xcode.cn/Article/details/gt3cjflnvaj.html

[U18] Py：预编译正则
来源：http://www.52xcode.cn/Article/details/gt3deahhuho.html

pat = re.compile(r"\d+")
来源：http://www.ydjk.org.cn/Article/details/gt3xpeweoxj.html

[U19] Py：正则替换带回调
来源：http://www.ydjk.org.cn/Article/details/gt3trwrcmrs.html

re.sub(r"\d+", lambda m: str(int(m.group()) * 2), s)
来源：http://www.52xcode.cn/Article/details/gt3hxmlvozu.html

[U20] Py：缓存函数结果
来源：http://www.ydjk.org.cn/Article/details/gt3gjcmavxk.html

@functools.lru_cache(maxsize=None)
来源：http://www.ydjk.org.cn/Article/details/gt3cjgxplmw.html

[U21] Py：自定义上下文管理器
来源：http://www.52xcode.cn/Article/details/gt3soscntbl.html

@contextlib.contextmanager
来源：http://www.52xcode.cn/Article/details/gt3aewdcfen.html

[U22] Py：矩阵转置
来源：http://www.52xcode.cn/Article/details/gt3lihgmool.html

list(zip(*m))
来源：http://www.ydjk.org.cn/Article/details/gt3udnojvsv.html

[U23] Py：分块读取大文件
来源：http://www.ydjk.org.cn/Article/details/gt3pbvcjobe.html

for chunk in iter(lambda: f.read(8192), b""):
来源：http://www.52xcode.cn/Article/details/gt3igrhnney.html

[U24] Py：路径操作
来源：http://www.ydjk.org.cn/Article/details/gt3auspkdlt.html

Path("a/b.txt").parent.mkdir(parents=True, exist_ok=True)
来源：http://www.ydjk.org.cn/Article/details/gt3zwxfpzfs.html

[U25] Py：CSV 按字典读
来源：http://www.ydjk.org.cn/Article/details/gt3xjjvmyjo.html

csv.DictReader(f)
来源：http://www.52xcode.cn/Article/details/gt3lpctrndp.html

[U26] Py：并发下载
来源：http://www.ydjk.org.cn/Article/details/gt3cllloqba.html

ThreadPoolExecutor(max_workers=8).map(fetch, urls)
来源：http://www.52xcode.cn/Article/details/gt3alleobir.html

[U27] Py：异步 HTTP
来源：http://www.52xcode.cn/Article/details/gt3qdedtpuw.html

aiohttp.ClientSession() 配合 async with
来源：http://www.52xcode.cn/Article/details/gt3kylbyifb.html

[U28] Py：类型别名
来源：http://www.52xcode.cn/Article/details/gt3bzcefyjf.html

UserId = int
来源：http://www.52xcode.cn/Article/details/gt3ooohorvo.html

[U29] Py：属性校验
来源：http://www.ydjk.org.cn/Article/details/gt3pedgnwwq.html

@property 与 @x.setter 配合
来源：http://www.52xcode.cn/Article/details/gt3rmrikfhe.html

[U30] Py：数据类
来源：http://www.ydjk.org.cn/Article/details/gt3wkcaejni.html

@dataclass(slots=True)
来源：http://www.52xcode.cn/Article/details/gt3rjtsrrax.html

[U31] Py：单测
来源：http://www.52xcode.cn/Article/details/gt3kwczodvq.html

python -m pytest -q
来源：http://www.ydjk.org.cn/Article/details/gt3qyylllaj.html

[U32] Py：代码格式化
来源：http://www.ydjk.org.cn/Article/details/gt3vysjnrpa.html

ruff format . && ruff check --fix .
来源：http://www.ydjk.org.cn/Article/details/gt3vyfawjxy.html

[U33] Py：打包发布
来源：http://www.ydjk.org.cn/Article/details/gt3zamcpdqe.html

python -m build  （依赖 pyproject.toml）
来源：http://www.52xcode.cn/Article/details/gt3pkbqgawj.html

[U34] Py：判断编码
来源：http://www.ydjk.org.cn/Article/details/gt3ehjxrycz.html

chardet.detect(raw)
来源：http://www.ydjk.org.cn/Article/details/gt3ondxgtcw.html

[U35] Py：发送邮件
来源：http://www.52xcode.cn/Article/details/gt3qwnpamgf.html

smtplib.SMTP_SSL(...).send_message(msg)
来源：http://www.52xcode.cn/Article/details/gt3kzpirqtg.html

[U36] Py：定时任务
来源：http://www.ydjk.org.cn/Article/details/gt3xsoizkbp.html

schedule.every(10).minutes.do(job)
来源：http://www.52xcode.cn/Article/details/gt3xravroaz.html

[U37] Py：读写 Excel
来源：http://www.ydjk.org.cn/Article/details/gt3nuucuelq.html

pandas.read_excel / DataFrame.to_excel
来源：http://www.ydjk.org.cn/Article/details/gt3llwoovcr.html

[U38] Py：获取脚本所在目录
来源：http://www.ydjk.org.cn/Article/details/gt3wcbjydvq.html

Path(__file__).resolve().parent
来源：http://www.52xcode.cn/Article/details/gt3xqbpzkih.html

[U39] Py：判断是否在交互环境
来源：http://www.52xcode.cn/Article/details/gt3slgexxzn.html

sys.stdout.isatty()
来源：http://www.ydjk.org.cn/Article/details/gt3xwzniixy.html

[U40] Py：打印到标准错误
来源：http://www.ydjk.org.cn/Article/details/gt3cnuptgni.html

print("err", file=sys.stderr)
来源：http://www.52xcode.cn/Article/details/gt3jkzdpeot.html

[U41] PHP：初始化 Composer 项目
来源：http://www.52xcode.cn/Article/details/gt3wbuvrvvl.html

composer init;  composer require guzzlehttp/guzzle
来源：http://www.ydjk.org.cn/Article/details/gt3ntftvnfa.html

[U42] PHP：PSR-4 自动加载
来源：http://www.ydjk.org.cn/Article/details/gt3ivxqpsgt.html

"autoload": { "psr-4": { "App\\": "src/" } }
来源：http://www.52xcode.cn/Article/details/gt3ivnggyga.html

[U43] PHP：声明命名空间
来源：http://www.52xcode.cn/Article/details/gt3lvdpxdxe.html

namespace App\Http;
来源：http://www.ydjk.org.cn/Article/details/gt3vsjniqrj.html

[U44] PHP：开启严格类型
来源：http://www.ydjk.org.cn/Article/details/gt3bimpqxwy.html

declare(strict_types=1);
来源：http://www.ydjk.org.cn/Article/details/gt3odyljcfz.html

[U45] PHP：类型声明与返回类型
来源：http://www.ydjk.org.cn/Article/details/gt3ecuvaxfw.html

function add(int $a, int $b): int { return $a + $b; }
来源：http://www.ydjk.org.cn/Article/details/gt3tvdpidhf.html

[U46] PHP：可空类型
来源：http://www.ydjk.org.cn/Article/details/gt3awvwbdln.html

?string $name = null
来源：http://www.52xcode.cn/Article/details/gt3gdwyvjlp.html

[U47] PHP：联合类型
来源：http://www.ydjk.org.cn/Article/details/gt3peuqcnxp.html

int|string $id
来源：http://www.52xcode.cn/Article/details/gt3erhaiejx.html

[U48] PHP：纯枚举
来源：http://www.ydjk.org.cn/Article/details/gt3fptgqhqj.html

enum Status: string { case Active = "active"; case Off = "off"; }
来源：http://www.ydjk.org.cn/Article/details/gt3ulmhaoin.html

[U49] PHP：只读属性
来源：http://www.ydjk.org.cn/Article/details/gt3elifeyob.html

public readonly string $name
来源：http://www.ydjk.org.cn/Article/details/gt3dixlesae.html

[U50] PHP：构造器属性提升
来源：http://www.52xcode.cn/Article/details/gt3qygpesqj.html

public function __construct(private int $id) {}
来源：http://www.ydjk.org.cn/Article/details/gt3ygwxiisa.html

[U51] PHP：数组解构
来源：http://www.52xcode.cn/Article/details/gt3vmmmrjbe.html

[$a, $b] = $arr;
来源：http://www.ydjk.org.cn/Article/details/gt3oikfmtpz.html

[U52] PHP：箭头函数
来源：http://www.52xcode.cn/Article/details/gt3qbxydjep.html

$double = fn($x) => $x * 2;
来源：http://www.ydjk.org.cn/Article/details/gt3lbtxzfur.html

[U53] PHP：空合并运算符
来源：http://www.ydjk.org.cn/Article/details/gt3brkgxenz.html

$v = $a ?? $b ?? "default";
来源：http://www.ydjk.org.cn/Article/details/gt3llszlkoa.html

[U54] PHP：空安全调用
来源：http://www.ydjk.org.cn/Article/details/gt3xedyaono.html

$obj?->method()
来源：http://www.52xcode.cn/Article/details/gt3slzrxdxp.html

[U55] PHP：match 表达式
来源：http://www.52xcode.cn/Article/details/gt3sylcamrw.html

$s = match($x) { 1 => "一", default => "其他" };
来源：http://www.ydjk.org.cn/Article/details/gt3gdagrvll.html

[U56] PHP：命名参数
来源：http://www.52xcode.cn/Article/details/gt3kantadsc.html

f(a: 1, b: 2)
来源：http://www.52xcode.cn/Article/details/gt3dbwtdpue.html

[U57] PHP：字符串插值
来源：http://www.52xcode.cn/Article/details/gt3lygmlfby.html

"值: {$a}"
来源：http://www.ydjk.org.cn/Article/details/gt3ooohothj.html

[U58] PHP：数组三件套
来源：http://www.52xcode.cn/Article/details/gt3hmpjazry.html

array_map($f, $a);  array_filter($a, $f);  array_reduce($a, $f, 0);
来源：http://www.52xcode.cn/Article/details/gt3adwrerzx.html

[U59] PHP：自定义排序
来源：http://www.ydjk.org.cn/Article/details/gt3nplcbdmb.html

usort($arr, fn($a, $b) => $a["age"] <=> $b["age"]);
来源：http://www.ydjk.org.cn/Article/details/gt3euuzkwna.html

[U60] PHP：JSON 编解码
来源：http://www.ydjk.org.cn/Article/details/gt3oonkcwkw.html

json_encode($d, JSON_UNESCAPED_UNICODE);  json_decode($s, true);
来源：http://www.ydjk.org.cn/Article/details/gt3lkytzdxu.html

[U61] PHP：正则
来源：http://www.52xcode.cn/Article/details/gt3ljghyvpn.html

preg_match('/(\d+)/', $s, $m);  preg_replace('/\d+/', '#', $s);
来源：http://www.52xcode.cn/Article/details/gt3zpetscqi.html

[U62] PHP：日期对象
来源：http://www.52xcode.cn/Article/details/gt3gbpcfdfl.html

(new DateTimeImmutable())->format("Y-m-d");
来源：http://www.52xcode.cn/Article/details/gt3gryssgvu.html

[U63] PHP：文件读写
来源：http://www.ydjk.org.cn/Article/details/gt3lfufpfbw.html

file_get_contents($f);  file_put_contents($f, $data);
来源：http://www.ydjk.org.cn/Article/details/gt3uyvuwapv.html

[U64] PHP：目录遍历
来源：http://www.ydjk.org.cn/Article/details/gt3xumoblgs.html

glob("dir/*.php");  scandir("dir");
来源：http://www.ydjk.org.cn/Article/details/gt3oqfcpinj.html

[U65] PHP：会话
来源：http://www.ydjk.org.cn/Article/details/gt3mhimgmsc.html

session_start();  $_SESSION["uid"] = 1;
来源：http://www.ydjk.org.cn/Article/details/gt3jvncboaa.html

[U66] PHP：设置 Cookie
来源：http://www.52xcode.cn/Article/details/gt3jbfcxogu.html

setcookie("token", $v, ["httponly" => true, "samesite" => "Lax"]);
来源：http://www.52xcode.cn/Article/details/gt3nrudzbyf.html

[U67] PHP：处理文件上传
来源：http://www.ydjk.org.cn/Article/details/gt3kwcqjxvp.html

$_FILES["file"]["tmp_name"] 与 move_uploaded_file()
来源：http://www.ydjk.org.cn/Article/details/gt3aligqcul.html

[U68] PHP：PDO 连接
来源：http://www.52xcode.cn/Article/details/gt3knqzklcd.html

$pdo = new PDO("mysql:host=localhost;dbname=app", "root", "");
来源：http://www.ydjk.org.cn/Article/details/gt3nrnoonqw.html

[U69] PHP：PDO 预处理
来源：http://www.ydjk.org.cn/Article/details/gt3sdotgfgv.html

$stmt = $pdo->prepare("SELECT * FROM users WHERE id = ?");  $stmt->execute([$id]);
来源：http://www.52xcode.cn/Article/details/gt3ufjabrov.html

[U70] PHP：PDO 事务
来源：http://www.ydjk.org.cn/Article/details/gt3vehmdsxd.html

$pdo->beginTransaction();  $pdo->commit();  $pdo->rollBack();
来源：http://www.52xcode.cn/Article/details/gt3wiqkvovo.html

[U71] PHP：抛出异常
来源：http://www.52xcode.cn/Article/details/gt3xiopjmzp.html

throw new RuntimeException("失败", 500);
来源：http://www.ydjk.org.cn/Article/details/gt3swielruh.html

[U72] PHP：写错误日志
来源：http://www.ydjk.org.cn/Article/details/gt3gqdxpyom.html

error_log("失败: " . $e->getMessage());
来源：http://www.ydjk.org.cn/Article/details/gt3yefyiwtj.html

[U73] PHP：读取 ini 配置
来源：http://www.ydjk.org.cn/Article/details/gt3zjrcqtzb.html

parse_ini_file("config.ini", true)
来源：http://www.52xcode.cn/Article/details/gt3jbgeyalg.html

[U74] PHP：读取环境变量
来源：http://www.52xcode.cn/Article/details/gt3blhmikmi.html

getenv("APP_ENV") ?: "production"
来源：http://www.ydjk.org.cn/Article/details/gt3rldthevc.html

[U75] PHP：依赖注入
来源：http://www.52xcode.cn/Article/details/gt3shslxixl.html

composer require psr/container
来源：http://www.ydjk.org.cn/Article/details/gt3ltxfbirb.html

[U76] PHP：简单路由
来源：http://www.ydjk.org.cn/Article/details/gt3wntwiani.html

$path = parse_url($_SERVER["REQUEST_URI"], PHP_URL_PATH);
来源：http://www.ydjk.org.cn/Article/details/gt3frpfvkvc.html

[U77] PHP：模板渲染
来源：http://www.ydjk.org.cn/Article/details/gt3hvdkddyg.html

composer require twig/twig
来源：http://www.52xcode.cn/Article/details/gt3aazyrwih.html

[U78] PHP：单元测试
来源：http://www.52xcode.cn/Article/details/gt3iajjxpgg.html

composer require --dev phpunit/phpunit
来源：http://www.52xcode.cn/Article/details/gt3qkmtodtz.html

[U79] PHP：静态分析
来源：http://www.52xcode.cn/Article/details/gt3tfrrpimt.html

composer require --dev phpstan/phpstan
来源：http://www.ydjk.org.cn/Article/details/gt3xqhwaokd.html

[U80] PHP：代码规范修复
来源：http://www.52xcode.cn/Article/details/gt3smtqjymp.html

composer require --dev friendsofphp/php-cs-fixer
来源：http://www.52xcode.cn/Article/details/gt3djifzvwq.html

[U81] JS：初始化项目
来源：http://www.52xcode.cn/Article/details/gt3oidvvqfx.html

npm init -y;  npm i express
来源：http://www.52xcode.cn/Article/details/gt3ymvydejr.html

[U82] JS：package.json 脚本
来源：http://www.52xcode.cn/Article/details/gt3tpwxawjo.html

"scripts": { "dev": "vite", "build": "vite build" }
来源：http://www.ydjk.org.cn/Article/details/gt3xitefqui.html

[U83] JS：ES Module 导入导出
来源：http://www.ydjk.org.cn/Article/details/gt3fzwhdcxr.html

export const a = 1;  import { a } from "./m.js";
来源：http://www.ydjk.org.cn/Article/details/gt3kpldmdiz.html

[U84] JS：CommonJS 写法
来源：http://www.ydjk.org.cn/Article/details/gt3rrudbhcu.html

module.exports = { a };  const { a } = require("./m");
来源：http://www.ydjk.org.cn/Article/details/gt3ovrtxwyw.html

[U85] JS：可选链
来源：http://www.52xcode.cn/Article/details/gt3swyforln.html

a?.b?.c
来源：http://www.ydjk.org.cn/Article/details/gt3fgnawlfp.html

[U86] JS：空值合并
来源：http://www.ydjk.org.cn/Article/details/gt3tvolvjpo.html

a ?? b
来源：http://www.ydjk.org.cn/Article/details/gt3wmjqypfa.html

[U87] JS：解构默认值
来源：http://www.ydjk.org.cn/Article/details/gt3wjcbgift.html

const { a = 1, b = 2 } = obj;
来源：http://www.ydjk.org.cn/Article/details/gt3knlbsrid.html

[U88] JS：对象展开合并
来源：http://www.52xcode.cn/Article/details/gt3buftwouc.html

{ ...a, ...b }
来源：http://www.ydjk.org.cn/Article/details/gt3ytovbkww.html

[U89] JS：数组去重
来源：http://www.ydjk.org.cn/Article/details/gt3aykrvpkn.html

[...new Set(arr)]
来源：http://www.ydjk.org.cn/Article/details/gt3bxkcdgkz.html

[U90] JS：数字数组排序
来源：http://www.ydjk.org.cn/Article/details/gt3kbwhmtdk.html

[...arr].sort((a, b) => a - b)
来源：http://www.ydjk.org.cn/Article/details/gt3nsuqnxty.html

[U91] JS：对象键值遍历
来源：http://www.52xcode.cn/Article/details/gt3sbdvciwx.html

Object.entries(obj).forEach(([k, v]) => {});
来源：http://www.52xcode.cn/Article/details/gt3ftynuexu.html

[U92] JS：深拷贝
来源：http://www.ydjk.org.cn/Article/details/gt3jgqmqscv.html

structuredClone(obj)
来源：http://www.ydjk.org.cn/Article/details/gt3mjhdqeoc.html

[U93] JS：模板字符串
来源：http://www.ydjk.org.cn/Article/details/gt3uhbrhoiz.html

`共 ${n} 条`
来源：http://www.52xcode.cn/Article/details/gt3hdwshbio.html

[U94] JS：箭头函数
来源：http://www.52xcode.cn/Article/details/gt3lsfclqeu.html

const double = x => x * 2;
来源：http://www.ydjk.org.cn/Article/details/gt3fftvlloa.html

[U95] JS：Promise 包装
来源：http://www.52xcode.cn/Article/details/gt3nbfmmlqz.html

new Promise((resolve, reject) => {})
来源：http://www.52xcode.cn/Article/details/gt3wbyamgac.html

[U96] JS：async/await 与异常
来源：http://www.ydjk.org.cn/Article/details/gt3norqhsxh.html

try { const d = await f(); } catch (e) { console.error(e); }
来源：http://www.ydjk.org.cn/Article/details/gt3dfzydayu.html

[U97] JS：并发请求
来源：http://www.ydjk.org.cn/Article/details/gt3clbjoewg.html

await Promise.all(urls.map(u => fetch(u)))
来源：http://www.52xcode.cn/Article/details/gt3ldlhppsz.html

[U98] JS：fetch 带 JSON
来源：http://www.52xcode.cn/Article/details/gt3wyhevzpt.html

await fetch(url, { method: "POST", headers: { "Content-Type": "application/json" }, body: JSON.stringify(d) })
来源：http://www.ydjk.org.cn/Article/details/gt3goqiyoxr.html

[U99] JS：事件监听
来源：http://www.ydjk.org.cn/Article/details/gt3kilspovf.html

el.addEventListener("click", e => {})
来源：http://www.52xcode.cn/Article/details/gt3uykknnpe.html

[U100] JS：DOM 查询
来源：http://www.52xcode.cn/Article/details/gt3grjviaks.html

document.querySelector(".item")
来源：http://www.52xcode.cn/Article/details/gt3zkkndluk.html

[U101] JS：classList 操作
来源：http://www.52xcode.cn/Article/details/gt3rmgufqjg.html

el.classList.toggle("active")
来源：http://www.52xcode.cn/Article/details/gt3haspkzpw.html

[U102] JS：本地存储
来源：http://www.52xcode.cn/Article/details/gt3vpwouotc.html

localStorage.setItem("k", JSON.stringify(v))
来源：http://www.ydjk.org.cn/Article/details/gt3omtmjwer.html

[U103] JS：定时器
来源：http://www.ydjk.org.cn/Article/details/gt3evgweohx.html

setTimeout(fn, 1000);  setInterval(fn, 1000);
来源：http://www.52xcode.cn/Article/details/gt3swfbftna.html

[U104] JS：防抖
来源：http://www.52xcode.cn/Article/details/gt3phrezbos.html

const debounce = (fn, ms) => { let t; return (...a) => { clearTimeout(t); t = setTimeout(() => fn(...a), ms); }; };
来源：http://www.52xcode.cn/Article/details/gt3jigvkbyx.html

[U105] JS：节流
来源：http://www.52xcode.cn/Article/details/gt3nyrfmamx.html

const throttle = (fn, ms) => { let last = 0; return (...a) => { const n = Date.now(); if (n - last >= ms) { last = n; fn(...a); } }; };
来源：http://www.52xcode.cn/Article/details/gt3ukjolqex.html

[U106] JS：日期格式化
来源：http://www.52xcode.cn/Article/details/gt3ursekjhl.html

new Intl.DateTimeFormat("zh-CN", { dateStyle: "medium" }).format(new Date())
来源：http://www.ydjk.org.cn/Article/details/gt3qhwzhium.html

[U107] JS：数字千分位
来源：http://www.52xcode.cn/Article/details/gt3ecqnnwfr.html

new Intl.NumberFormat("en-US").format(1234567)
来源：http://www.52xcode.cn/Article/details/gt3rpgfcuhc.html

[U108] JS：随机整数
来源：http://www.52xcode.cn/Article/details/gt3qaylpvtk.html

Math.floor(Math.random() * (max - min + 1)) + min
来源：http://www.52xcode.cn/Article/details/gt3bhoenxtw.html

[U109] JS：数组分组
来源：http://www.ydjk.org.cn/Article/details/gt3ksxingxe.html

Object.groupBy(arr, x => x.type)
来源：http://www.ydjk.org.cn/Article/details/gt3qywyrjio.html

[U110] JS：数组分块
来源：http://www.ydjk.org.cn/Article/details/gt3xjzastjk.html

arr.reduce((acc, x, i) => (i % size ? acc : [...acc, arr.slice(i, i + size)]), [])
来源：http://www.ydjk.org.cn/Article/details/gt3xpxxuvlw.html

[U111] JS：对象转 Map
来源：http://www.ydjk.org.cn/Article/details/gt3gzvxgert.html

new Map(Object.entries(obj))
来源：http://www.ydjk.org.cn/Article/details/gt3ooabcbhp.html

[U112] JS：字符串补位
来源：http://www.52xcode.cn/Article/details/gt3givizbvy.html

"7".padStart(3, "0")
来源：http://www.ydjk.org.cn/Article/details/gt3rvowvgfb.html

[U113] JS：正则替换全部
来源：http://www.ydjk.org.cn/Article/details/gt3dlzkzktg.html

s.replaceAll("a", "b")
来源：http://www.52xcode.cn/Article/details/gt3msagqfvy.html

[U114] JS：JSON 深比较
来源：http://www.52xcode.cn/Article/details/gt3xxrlyxzd.html

JSON.stringify(a) === JSON.stringify(b)
来源：http://www.52xcode.cn/Article/details/gt3olgmqrrd.html

[U115] JS：生成 UUID
来源：http://www.52xcode.cn/Article/details/gt3qimencsm.html

crypto.randomUUID()
来源：http://www.52xcode.cn/Article/details/gt3asmcwqix.html

[U116] JS：类型检查（JSDoc）
来源：http://www.52xcode.cn/Article/details/gt3rhwwtdtv.html

/** @param {string} name */ function f(name) {}
来源：http://www.ydjk.org.cn/Article/details/gt3kblvaxor.html

[U117] JS：单元测试
来源：http://www.52xcode.cn/Article/details/gt3wdomozij.html

npm i -D vitest;  npx vitest
来源：http://www.52xcode.cn/Article/details/gt3siocmgyb.html

[U118] JS：开发服务器
来源：http://www.ydjk.org.cn/Article/details/gt3ymbdelcq.html

npm i -D vite;  npx vite
来源：http://www.ydjk.org.cn/Article/details/gt3nlibmlar.html

[U119] JS：生产构建
来源：http://www.52xcode.cn/Article/details/gt3ykycwnvs.html

npx vite build
来源：http://www.52xcode.cn/Article/details/gt3fljrxqpe.html

[U120] JS：读取环境变量（Vite）
来源：http://www.52xcode.cn/Article/details/gt3hnjwdmbh.html

import.meta.env.VITE_API_URL
来源：http://www.ydjk.org.cn/Article/details/gt3vwefbytz.html

================================================================================
来源：http://www.52xcode.cn/Article/details/gt3bmmrvtev.html

统计汇总
来源：http://www.ydjk.org.cn/Article/details/gt3yjmqqvyr.html

================================================================================
来源：http://www.ydjk.org.cn/Article/details/gt3usolymal.html

按语言统计（条）：
来源：http://www.52xcode.cn/Article/details/gt3bwzxnnqu.html

Python ......... 252
来源：http://www.52xcode.cn/Article/details/gt3bjohtuek.html

PHP ............ 252
来源：http://www.52xcode.cn/Article/details/gt3vveimzje.html

JavaScript ..... 252
来源：http://www.52xcode.cn/Article/details/gt3ngzckyzt.html

TypeScript ..... 212
来源：http://www.52xcode.cn/Article/details/gt3clyavqmc.html

Java ........... 212
来源：http://www.52xcode.cn/Article/details/gt3hukpyuwt.html

Go ............. 212
来源：http://www.52xcode.cn/Article/details/gt3vcngbjrh.html

Ruby ........... 212
来源：http://www.ydjk.org.cn/Article/details/gt3vvtgcjmt.html

C# ............. 212
来源：http://www.ydjk.org.cn/Article/details/gt3ydeyslwq.html

C .............. 30
来源：http://www.ydjk.org.cn/Article/details/gt3mmwutnov.html

C++ ............ 30
来源：http://www.52xcode.cn/Article/details/gt3osxrooqy.html

SQL ............ 90
来源：http://www.52xcode.cn/Article/details/gt3rdmbqegs.html

Bash ........... 80
来源：http://www.ydjk.org.cn/Article/details/gt3ywsqfthz.html

Kotlin ......... 15
来源：http://www.52xcode.cn/Article/details/gt3wlfaacfv.html

Swift .......... 15
来源：http://www.ydjk.org.cn/Article/details/gt3klkihlsp.html

Lua ............ 10
来源：http://www.52xcode.cn/Article/details/gt3ffpmppnp.html

Perl ........... 10
来源：http://www.52xcode.cn/Article/details/gt3heoquxzf.html

Scala .......... 10
来源：http://www.ydjk.org.cn/Article/details/gt3zqtunuqe.html

------------------------------------
来源：http://www.ydjk.org.cn/Article/details/gt3wxctznps.html

合计 ........... 2106 条
来源：http://www.52xcode.cn/Article/details/gt3hizfdetb.html

按章节统计：
来源：http://www.52xcode.cn/Article/details/gt3mwtqztdf.html

A 基础语法与类型       26 个任务 × 8 语言 =  208
来源：http://www.52xcode.cn/Article/details/gt3bwhwidte.html

B 流程控制             16 个任务 × 8 语言 =  128
来源：http://www.ydjk.org.cn/Article/details/gt3vxnqqkun.html

C 函数与作用域         16 个任务 × 8 语言 =  128
来源：http://www.52xcode.cn/Article/details/gt3sxgleatr.html

D 数组 / 列表 / 集合   26 个任务 × 8 语言 =  208
来源：http://www.52xcode.cn/Article/details/gt3kqgqchai.html

E 字符串处理           22 个任务 × 8 语言 =  176
来源：http://www.ydjk.org.cn/Article/details/gt3ocbiemsz.html

F 文件与目录           12 个任务 × 8 语言 =   96
来源：http://www.ydjk.org.cn/Article/details/gt3bprpiqnl.html

G 面向对象             16 个任务 × 8 语言 =  128
来源：http://www.52xcode.cn/Article/details/gt3yijwxqhd.html

H 异常与错误处理       10 个任务 × 8 语言 =   80
来源：http://www.ydjk.org.cn/Article/details/gt3nqdfkzuc.html

I 正则表达式            8 个任务 × 8 语言 =   64
来源：http://www.ydjk.org.cn/Article/details/gt3tthuulkd.html

J 日期与时间           10 个任务 × 8 语言 =   80
来源：http://www.52xcode.cn/Article/details/gt3tvotckpf.html

K JSON 与序列化         8 个任务 × 8 语言 =   64
来源：http://www.ydjk.org.cn/Article/details/gt3xoznyfij.html

L 网络请求              8 个任务 × 8 语言 =   64
来源：http://www.ydjk.org.cn/Article/details/gt3hxhoshqq.html

M 命令行 / 进程         8 个任务 × 8 语言 =   64
来源：http://www.52xcode.cn/Article/details/gt3fkxghefi.html

N 数据结构与算法       12 个任务 × 8 语言 =   96
来源：http://www.52xcode.cn/Article/details/gt3gsknmcwo.html

O 并发与异步            6 个任务 × 8 语言 =   48
来源：http://www.ydjk.org.cn/Article/details/gt3xwibyxcg.html

P 常用工具函数          8 个任务 × 8 语言 =   64
来源：http://www.ydjk.org.cn/Article/details/gt3tsqqcaqw.html

Q SQL 专题                              90
来源：http://www.52xcode.cn/Article/details/gt3slcpcbka.html

R Bash 专题                             80
来源：http://www.ydjk.org.cn/Article/details/gt3thefsiqy.html

S C / C++ 专题                          60
来源：http://www.52xcode.cn/Article/details/gt3nbvvwxlc.html

T 其他语言补充                          60
来源：http://www.ydjk.org.cn/Article/details/gt3tuxkovuc.html

U 高频实用片段                         120
来源：http://www.52xcode.cn/Article/details/gt3rmgwdtqq.html

------------------------------------
来源：http://www.52xcode.cn/Article/details/gt3isfpmdlz.html

合计                                  2106 条
来源：http://www.ydjk.org.cn/Article/details/gt3tbfxdlgh.html

--------------------------------------------------------------------------------
来源：http://www.ydjk.org.cn/Article/details/gt3pwhvmido.html

使用提醒
来源：http://www.52xcode.cn/Article/details/gt3dwqkzoco.html

--------------------------------------------------------------------------------
来源：http://www.52xcode.cn/Article/details/gt3krnymktg.html

1. 示例追求"最小可用"，正式项目中请补齐导入、错误处理与边界判断。
来源：http://www.ydjk.org.cn/Article/details/gt3xhaquseh.html

2. 涉及文件、网络、数据库的示例，注意资源释放与异常捕获。
来源：http://www.ydjk.org.cn/Article/details/gt3sluvbmux.html

3. 语言版本差异较大（如 Python 3.10 的 match、Java 17 的 record/switch 箭头），
来源：http://www.ydjk.org.cn/Article/details/gt3nksmdmfj.html

在旧版本上使用前请先确认语法支持情况。
来源：http://www.52xcode.cn/Article/details/gt3pxzipfez.html

4. 标注"手写"的条目是因为该语言缺少对应内置能力，实际项目中可引入成熟库。
来源：http://www.52xcode.cn/Article/details/gt3ooqloxpy.html

—— 文件结束 ——
来源：http://www.52xcode.cn/Article/details/gt3lixwlsjg.html

================================================================================
来源：http://www.ydjk.org.cn/Article/details/gt3cjdrwtdc.html

程序语言常见例子速查手册（2024 版）
来源：http://www.52xcode.cn/Article/details/gt3lglrzdlq.html

Common Programming Examples Cheat Book
来源：http://www.52xcode.cn/Article/details/gt3lbqgpemv.html

================================================================================
来源：http://www.52xcode.cn/Article/details/gt3qkocylpj.html

【收录内容】
来源：http://www.52xcode.cn/Article/details/gt3kitswlff.html

覆盖 12 种语言 / 语法与常见 API：
来源：http://www.ydjk.org.cn/Article/details/gt3stqnxvlj.html

Python · PHP · JavaScript · TypeScript · Java · Go · Ruby · C#
来源：http://www.ydjk.org.cn/Article/details/gt3gngwvpgx.html

SQL · Bash · C · C++
来源：http://www.52xcode.cn/Article/details/gt3rwebmnef.html

按「任务」分组：每个任务下按语言各给出一条最小可用示例。
来源：http://www.ydjk.org.cn/Article/details/gt3ppondkfo.html

【使用说明】
来源：http://www.ydjk.org.cn/Article/details/gt3bipdwowk.html

1. 每个任务形如 "[编号] 任务名"，下面每行以语言标记开头：
来源：http://www.ydjk.org.cn/Article/details/gt3mtgncmvt.html

Py:    Python        PHP:   PHP           JS:    JavaScript
来源：http://www.ydjk.org.cn/Article/details/gt3yakepqrw.html

TS:    TypeScript    Java:  Java          Go:    Go
来源：http://www.52xcode.cn/Article/details/gt3ovbnsjme.html

Ruby:  Ruby          C#:    C#            SQL:   SQL
来源：http://www.ydjk.org.cn/Article/details/gt3cfayeoze.html

Bash:  Shell         C:     C             C++:   C++
来源：http://www.ydjk.org.cn/Article/details/gt3dqqvpzfs.html

2. 示例只展示核心写法，刻意省略 import / require / include / using 等样板代码。
来源：http://www.52xcode.cn/Article/details/gt3jwrkeclv.html

需要完整可运行文件时，请自行补齐当前语言的导入语句。
来源：http://www.ydjk.org.cn/Article/details/gt3viiydkwl.html

3. 语法基准：Python 3.10+ / PHP 8.1+ / ES2020+ / TypeScript 5 / Java 17 /
来源：http://www.52xcode.cn/Article/details/gt3kscxiprj.html

Go 1.21+ / Ruby 3.x / C# 10+ / C17 / C++17。
来源：http://www.ydjk.org.cn/Article/details/gt3cwdoehne.html

4. 检索建议：用编辑器或浏览器 Ctrl+F 搜关键词，如 "排序" "读取文件" "正则"。
来源：http://www.ydjk.org.cn/Article/details/gt3vbmyvptt.html

5. 标记为 "// 无" 表示该语言没有对应的一等语法，需用替代写法（示例给出替代方案）。
来源：http://www.52xcode.cn/Article/details/gt3yrjrfjso.html

6. 符号 "⏎" 表示代码在此处换行（主要用于 Python 等强制缩进、无法压成一行的结构）。
来源：http://www.ydjk.org.cn/Article/details/gt3xayflmfo.html

【文件统计】
来源：http://www.ydjk.org.cn/Article/details/gt3nuaegmgf.html

语言示例共 2106 条，分布见本文末尾的「统计汇总」。
来源：http://www.ydjk.org.cn/Article/details/gt3rixbfuhh.html


<!-- 参考信息 -->