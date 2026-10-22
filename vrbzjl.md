代发 wailian999

[U07] Py：反转字典键值
来源：http://www.52xcode.cn/Article/details/gt2gvsbcgtx.html

{v: k for k, v in d.items()}
来源：http://www.52xcode.cn/Article/details/gt2qydbvcwg.html

[U08] Py：展平二维列表
来源：http://www.52xcode.cn/Article/details/gt2thpsmcoi.html

[y for x in nested for y in x]
来源：http://www.ydjk.org.cn/Article/details/gt2vurvdqzx.html

[U09] Py：字典取最大值的键
来源：http://www.ydjk.org.cn/Article/details/gt2umkkwgvs.html

max(d, key=d.get)
来源：http://www.ydjk.org.cn/Article/details/gt2dpujfcsn.html

[U10] Py：按值排序字典
来源：http://www.52xcode.cn/Article/details/gt2yhpupgbg.html

dict(sorted(d.items(), key=lambda kv: kv[1]))
来源：http://www.52xcode.cn/Article/details/gt2oaccmfxk.html

[U11] Py：生成器表达式
来源：http://www.52xcode.cn/Article/details/gt2otmkgobb.html

(x * 2 for x in arr)
来源：http://www.52xcode.cn/Article/details/gt2wxdlfqse.html

[U12] Py：取出现最多的 3 个元素
来源：http://www.52xcode.cn/Article/details/gt2zbjbsliv.html

Counter(arr).most_common(3)
来源：http://www.52xcode.cn/Article/details/gt2fdkaffok.html

[U13] Py：固定长度队列
来源：http://www.ydjk.org.cn/Article/details/gt2kzoduytl.html

deque(maxlen=10)
来源：http://www.ydjk.org.cn/Article/details/gt2ayhhrvke.html

[U14] Py：分组收集到列表
来源：http://www.ydjk.org.cn/Article/details/gt2llhggzfq.html

defaultdict(list)
来源：http://www.52xcode.cn/Article/details/gt2qrxcaayw.html

[U15] Py：高精度计时
来源：http://www.ydjk.org.cn/Article/details/gt2ivqfxcxe.html

t = time.perf_counter()
来源：http://www.52xcode.cn/Article/details/gt2wlunsweu.html

[U16] Py：命令行参数解析
来源：http://www.ydjk.org.cn/Article/details/gt2dzvvfgbw.html

ap = argparse.ArgumentParser();  ap.add_argument("--name");  args = ap.parse_args()
来源：http://www.52xcode.cn/Article/details/gt2yoyldgpg.html

[U17] Py：初始化日志
来源：http://www.ydjk.org.cn/Article/details/gt2okhaqteo.html

logging.basicConfig(level=logging.INFO)
来源：http://www.52xcode.cn/Article/details/gt2tvfpwdsf.html

[U18] Py：预编译正则
来源：http://www.ydjk.org.cn/Article/details/gt2hcrputkv.html

pat = re.compile(r"\d+")
来源：http://www.52xcode.cn/Article/details/gt2fowjhfjc.html

[U19] Py：正则替换带回调
来源：http://www.52xcode.cn/Article/details/gt2ptjidyzc.html

re.sub(r"\d+", lambda m: str(int(m.group()) * 2), s)
来源：http://www.52xcode.cn/Article/details/gt2udhucyvm.html

[U20] Py：缓存函数结果
来源：http://www.52xcode.cn/Article/details/gt2htthdjos.html

@functools.lru_cache(maxsize=None)
来源：http://www.52xcode.cn/Article/details/gt2bpulvatf.html

[U21] Py：自定义上下文管理器
来源：http://www.52xcode.cn/Article/details/gt2mnufvwoh.html

@contextlib.contextmanager
来源：http://www.ydjk.org.cn/Article/details/gt2qwnpzdjx.html

[U22] Py：矩阵转置
来源：http://www.52xcode.cn/Article/details/gt2ytzpmatj.html

list(zip(*m))
来源：http://www.52xcode.cn/Article/details/gt2ihupaxnu.html

[U23] Py：分块读取大文件
来源：http://www.ydjk.org.cn/Article/details/gt2jbjtnfnd.html

for chunk in iter(lambda: f.read(8192), b""):
来源：http://www.52xcode.cn/Article/details/gt2uxmgyyve.html

[U24] Py：路径操作
来源：http://www.52xcode.cn/Article/details/gt2swuutemf.html

Path("a/b.txt").parent.mkdir(parents=True, exist_ok=True)
来源：http://www.ydjk.org.cn/Article/details/gt2zsppczvt.html

[U25] Py：CSV 按字典读
来源：http://www.52xcode.cn/Article/details/gt2batbdqlg.html

csv.DictReader(f)
来源：http://www.52xcode.cn/Article/details/gt2esubuoln.html

[U26] Py：并发下载
来源：http://www.ydjk.org.cn/Article/details/gt2vbogwuoa.html

ThreadPoolExecutor(max_workers=8).map(fetch, urls)
来源：http://www.ydjk.org.cn/Article/details/gt2sgkruvoz.html

[U27] Py：异步 HTTP
来源：http://www.ydjk.org.cn/Article/details/gt2zveqopta.html

aiohttp.ClientSession() 配合 async with
来源：http://www.52xcode.cn/Article/details/gt2bnxwikad.html

[U28] Py：类型别名
来源：http://www.ydjk.org.cn/Article/details/gt2hcmwygkt.html

UserId = int
来源：http://www.52xcode.cn/Article/details/gt2vfxcbaia.html

[U29] Py：属性校验
来源：http://www.ydjk.org.cn/Article/details/gt2myoendeu.html

@property 与 @x.setter 配合
来源：http://www.52xcode.cn/Article/details/gt2xujlhvmb.html

[U30] Py：数据类
来源：http://www.52xcode.cn/Article/details/gt2dwucjsxj.html

@dataclass(slots=True)
来源：http://www.52xcode.cn/Article/details/gt2vneyoolv.html

[U31] Py：单测
来源：http://www.ydjk.org.cn/Article/details/gt2buokxinb.html

python -m pytest -q
来源：http://www.52xcode.cn/Article/details/gt2wyoyrifd.html

[U32] Py：代码格式化
来源：http://www.ydjk.org.cn/Article/details/gt2axrgoukw.html

ruff format . && ruff check --fix .
来源：http://www.ydjk.org.cn/Article/details/gt2okegutpy.html

[U33] Py：打包发布
来源：http://www.ydjk.org.cn/Article/details/gt2ybizfbty.html

python -m build  （依赖 pyproject.toml）
来源：http://www.ydjk.org.cn/Article/details/gt2gafofkhx.html

[U34] Py：判断编码
来源：http://www.52xcode.cn/Article/details/gt2gjdvfbbr.html

chardet.detect(raw)
来源：http://www.52xcode.cn/Article/details/gt2gpcualqt.html

[U35] Py：发送邮件
来源：http://www.ydjk.org.cn/Article/details/gt2fbhvgcxa.html

smtplib.SMTP_SSL(...).send_message(msg)
来源：http://www.52xcode.cn/Article/details/gt2zuzkrrzx.html

[U36] Py：定时任务
来源：http://www.ydjk.org.cn/Article/details/gt2trpfcilb.html

schedule.every(10).minutes.do(job)
来源：http://www.ydjk.org.cn/Article/details/gt2gjyukctc.html

[U37] Py：读写 Excel
来源：http://www.52xcode.cn/Article/details/gt2fmsxpzix.html

pandas.read_excel / DataFrame.to_excel
来源：http://www.ydjk.org.cn/Article/details/gt2nwqftlvz.html

[U38] Py：获取脚本所在目录
来源：http://www.52xcode.cn/Article/details/gt2gsqafqqv.html

Path(__file__).resolve().parent
来源：http://www.ydjk.org.cn/Article/details/gt2qbddyubu.html

[U39] Py：判断是否在交互环境
来源：http://www.52xcode.cn/Article/details/gt2sncohsnm.html

sys.stdout.isatty()
来源：http://www.52xcode.cn/Article/details/gt2ndfwgheo.html

[U40] Py：打印到标准错误
来源：http://www.ydjk.org.cn/Article/details/gt2ugthlhku.html

print("err", file=sys.stderr)
来源：http://www.52xcode.cn/Article/details/gt2iuuhdnsf.html

[U41] PHP：初始化 Composer 项目
来源：http://www.52xcode.cn/Article/details/gt2minxdztu.html

composer init;  composer require guzzlehttp/guzzle
来源：http://www.52xcode.cn/Article/details/gt2aslqnsum.html

[U42] PHP：PSR-4 自动加载
来源：http://www.ydjk.org.cn/Article/details/gt2tkqzxwxe.html

"autoload": { "psr-4": { "App\\": "src/" } }
来源：http://www.ydjk.org.cn/Article/details/gt2dchoamjo.html

[U43] PHP：声明命名空间
来源：http://www.ydjk.org.cn/Article/details/gt2hnnwpeos.html

namespace App\Http;
来源：http://www.52xcode.cn/Article/details/gt2xdhksrnj.html

[U44] PHP：开启严格类型
来源：http://www.ydjk.org.cn/Article/details/gt2kuavgcri.html

declare(strict_types=1);
来源：http://www.52xcode.cn/Article/details/gt2vmeyglvv.html

[U45] PHP：类型声明与返回类型
来源：http://www.52xcode.cn/Article/details/gt2cufplvmv.html

function add(int $a, int $b): int { return $a + $b; }
来源：http://www.ydjk.org.cn/Article/details/gt2uccfkrjz.html

[U46] PHP：可空类型
来源：http://www.ydjk.org.cn/Article/details/gt2qcheedgv.html

?string $name = null
来源：http://www.ydjk.org.cn/Article/details/gt2wejocvto.html

[U47] PHP：联合类型
来源：http://www.52xcode.cn/Article/details/gt2kfsrhjuu.html

int|string $id
来源：http://www.ydjk.org.cn/Article/details/gt2cmewrpun.html

[U48] PHP：纯枚举
来源：http://www.ydjk.org.cn/Article/details/gt2fkpxxdrv.html

enum Status: string { case Active = "active"; case Off = "off"; }
来源：http://www.ydjk.org.cn/Article/details/gt2gooftdxf.html

[U49] PHP：只读属性
来源：http://www.ydjk.org.cn/Article/details/gt2ldfzwzji.html

public readonly string $name
来源：http://www.52xcode.cn/Article/details/gt2szrvxctg.html

[U50] PHP：构造器属性提升
来源：http://www.52xcode.cn/Article/details/gt2gyczvrok.html

public function __construct(private int $id) {}
来源：http://www.52xcode.cn/Article/details/gt2jhnyfrhx.html

[U51] PHP：数组解构
来源：http://www.52xcode.cn/Article/details/gt2npzvlgoc.html

[$a, $b] = $arr;
来源：http://www.52xcode.cn/Article/details/gt2qlllqkeb.html

[U52] PHP：箭头函数
来源：http://www.52xcode.cn/Article/details/gt2erarmsqp.html

$double = fn($x) => $x * 2;
来源：http://www.ydjk.org.cn/Article/details/gt2dzttovpw.html

[U53] PHP：空合并运算符
来源：http://www.52xcode.cn/Article/details/gt2jyglwmdj.html

$v = $a ?? $b ?? "default";
来源：http://www.ydjk.org.cn/Article/details/gt2gtmjtoul.html

[U54] PHP：空安全调用
来源：http://www.ydjk.org.cn/Article/details/gt2kbrcwsjp.html

$obj?->method()
来源：http://www.52xcode.cn/Article/details/gt2hgxffxfi.html

[U55] PHP：match 表达式
来源：http://www.ydjk.org.cn/Article/details/gt2wylrhgkr.html

$s = match($x) { 1 => "一", default => "其他" };
来源：http://www.52xcode.cn/Article/details/gt2ggtslsom.html

[U56] PHP：命名参数
来源：http://www.52xcode.cn/Article/details/gt2ynxtpjtm.html

f(a: 1, b: 2)
来源：http://www.ydjk.org.cn/Article/details/gt2scmhqbjt.html

[U57] PHP：字符串插值
来源：http://www.ydjk.org.cn/Article/details/gt2ijhlyzgh.html

"值: {$a}"
来源：http://www.ydjk.org.cn/Article/details/gt2mvvpznqf.html

[U58] PHP：数组三件套
来源：http://www.52xcode.cn/Article/details/gt2vwmmneye.html

array_map($f, $a);  array_filter($a, $f);  array_reduce($a, $f, 0);
来源：http://www.ydjk.org.cn/Article/details/gt2ydanwxao.html

[U59] PHP：自定义排序
来源：http://www.ydjk.org.cn/Article/details/gt2swaplbev.html

usort($arr, fn($a, $b) => $a["age"] <=> $b["age"]);
来源：http://www.52xcode.cn/Article/details/gt2nbbqkjom.html

[U60] PHP：JSON 编解码
来源：http://www.ydjk.org.cn/Article/details/gt2rnbfbscf.html

json_encode($d, JSON_UNESCAPED_UNICODE);  json_decode($s, true);
来源：http://www.ydjk.org.cn/Article/details/gt2kbfslhzs.html

[U61] PHP：正则
来源：http://www.52xcode.cn/Article/details/gt2xgkdthsg.html

preg_match('/(\d+)/', $s, $m);  preg_replace('/\d+/', '#', $s);
来源：http://www.ydjk.org.cn/Article/details/gt2jbvinrmu.html

[U62] PHP：日期对象
来源：http://www.52xcode.cn/Article/details/gt2lxykrfwn.html

(new DateTimeImmutable())->format("Y-m-d");
来源：http://www.ydjk.org.cn/Article/details/gt2degxmqeu.html

[U63] PHP：文件读写
来源：http://www.52xcode.cn/Article/details/gt2ebuekjlk.html

file_get_contents($f);  file_put_contents($f, $data);
来源：http://www.52xcode.cn/Article/details/gt2ecfbncup.html

[U64] PHP：目录遍历
来源：http://www.ydjk.org.cn/Article/details/gt2rfzuaman.html

glob("dir/*.php");  scandir("dir");
来源：http://www.52xcode.cn/Article/details/gt2zuocowhq.html

[U65] PHP：会话
来源：http://www.ydjk.org.cn/Article/details/gt2eltdhmlu.html

session_start();  $_SESSION["uid"] = 1;
来源：http://www.ydjk.org.cn/Article/details/gt2nodtndjr.html

[U66] PHP：设置 Cookie
来源：http://www.ydjk.org.cn/Article/details/gt2myarukku.html

setcookie("token", $v, ["httponly" => true, "samesite" => "Lax"]);
来源：http://www.ydjk.org.cn/Article/details/gt2deseugwb.html

[U67] PHP：处理文件上传
来源：http://www.52xcode.cn/Article/details/gt2yuamzwsz.html

$_FILES["file"]["tmp_name"] 与 move_uploaded_file()
来源：http://www.52xcode.cn/Article/details/gt2wwoiigpk.html

[U68] PHP：PDO 连接
来源：http://www.ydjk.org.cn/Article/details/gt2kwrcuygu.html

$pdo = new PDO("mysql:host=localhost;dbname=app", "root", "");
来源：http://www.ydjk.org.cn/Article/details/gt2tnmrkcru.html

[U69] PHP：PDO 预处理
来源：http://www.ydjk.org.cn/Article/details/gt2dsomkyuk.html

$stmt = $pdo->prepare("SELECT * FROM users WHERE id = ?");  $stmt->execute([$id]);
来源：http://www.52xcode.cn/Article/details/gt2bivrctph.html

[U70] PHP：PDO 事务
来源：http://www.52xcode.cn/Article/details/gt2ihkjxcqz.html

$pdo->beginTransaction();  $pdo->commit();  $pdo->rollBack();
来源：http://www.52xcode.cn/Article/details/gt2fyqizfef.html

[U71] PHP：抛出异常
来源：http://www.52xcode.cn/Article/details/gt2alihkaem.html

throw new RuntimeException("失败", 500);
来源：http://www.ydjk.org.cn/Article/details/gt2nyzacnjv.html

[U72] PHP：写错误日志
来源：http://www.ydjk.org.cn/Article/details/gt2ceowuiuq.html

error_log("失败: " . $e->getMessage());
来源：http://www.ydjk.org.cn/Article/details/gt2yhqtjsbx.html

[U73] PHP：读取 ini 配置
来源：http://www.ydjk.org.cn/Article/details/gt2ruwskkxm.html

parse_ini_file("config.ini", true)
来源：http://www.ydjk.org.cn/Article/details/gt2oerqaxpp.html

[U74] PHP：读取环境变量
来源：http://www.52xcode.cn/Article/details/gt2qjiwvnfq.html

getenv("APP_ENV") ?: "production"
来源：http://www.52xcode.cn/Article/details/gt2ceswjmvi.html

[U75] PHP：依赖注入
来源：http://www.ydjk.org.cn/Article/details/gt2vdyhqhxy.html

composer require psr/container
来源：http://www.ydjk.org.cn/Article/details/gt2dtionnpm.html

[U76] PHP：简单路由
来源：http://www.52xcode.cn/Article/details/gt2nobjboze.html

$path = parse_url($_SERVER["REQUEST_URI"], PHP_URL_PATH);
来源：http://www.52xcode.cn/Article/details/gt2anwscpew.html

[U77] PHP：模板渲染
来源：http://www.ydjk.org.cn/Article/details/gt2ybidvhmy.html

composer require twig/twig
来源：http://www.ydjk.org.cn/Article/details/gt2zxllmquu.html

[U78] PHP：单元测试
来源：http://www.52xcode.cn/Article/details/gt2ukmsgqwg.html

composer require --dev phpunit/phpunit
来源：http://www.52xcode.cn/Article/details/gt2xbowbohv.html

[U79] PHP：静态分析
来源：http://www.ydjk.org.cn/Article/details/gt2gputtnhn.html

composer require --dev phpstan/phpstan
来源：http://www.52xcode.cn/Article/details/gt2zswggywe.html

[U80] PHP：代码规范修复
来源：http://www.ydjk.org.cn/Article/details/gt2wtfzjckb.html

composer require --dev friendsofphp/php-cs-fixer
来源：http://www.52xcode.cn/Article/details/gt2geqsmedg.html

[U81] JS：初始化项目
来源：http://www.ydjk.org.cn/Article/details/gt2kmoxyuhp.html

npm init -y;  npm i express
来源：http://www.52xcode.cn/Article/details/gt2tkeitnpo.html

[U82] JS：package.json 脚本
来源：http://www.ydjk.org.cn/Article/details/gt2uutuuakx.html

"scripts": { "dev": "vite", "build": "vite build" }
来源：http://www.ydjk.org.cn/Article/details/gt2lqkigqfs.html

[U83] JS：ES Module 导入导出
来源：http://www.ydjk.org.cn/Article/details/gt2ifwsvzly.html

export const a = 1;  import { a } from "./m.js";
来源：http://www.52xcode.cn/Article/details/gt2dxtraamz.html

[U84] JS：CommonJS 写法
来源：http://www.52xcode.cn/Article/details/gt2wnyqteqg.html

module.exports = { a };  const { a } = require("./m");
来源：http://www.ydjk.org.cn/Article/details/gt2urlmjfxy.html

[U85] JS：可选链
来源：http://www.ydjk.org.cn/Article/details/gt2cbrtefqv.html

a?.b?.c
来源：http://www.52xcode.cn/Article/details/gt2goshmafn.html

[U86] JS：空值合并
来源：http://www.52xcode.cn/Article/details/gt2itwsgjsl.html

a ?? b
来源：http://www.ydjk.org.cn/Article/details/gt2alkhhlma.html

[U87] JS：解构默认值
来源：http://www.ydjk.org.cn/Article/details/gt2kdlfibph.html

const { a = 1, b = 2 } = obj;
来源：http://www.ydjk.org.cn/Article/details/gt2zohvgpcv.html

[U88] JS：对象展开合并
来源：http://www.ydjk.org.cn/Article/details/gt2xwmzizaa.html

{ ...a, ...b }
来源：http://www.ydjk.org.cn/Article/details/gt2vlfdccvh.html

[U89] JS：数组去重
来源：http://www.ydjk.org.cn/Article/details/gt2tudevcyg.html

[...new Set(arr)]
来源：http://www.52xcode.cn/Article/details/gt2sglfweqr.html

[U90] JS：数字数组排序
来源：http://www.52xcode.cn/Article/details/gt2peurkjhd.html

[...arr].sort((a, b) => a - b)
来源：http://www.52xcode.cn/Article/details/gt2hbsoldcp.html

[U91] JS：对象键值遍历
来源：http://www.52xcode.cn/Article/details/gt2mcmqxtcn.html

Object.entries(obj).forEach(([k, v]) => {});
来源：http://www.ydjk.org.cn/Article/details/gt2pisvjjds.html

[U92] JS：深拷贝
来源：http://www.52xcode.cn/Article/details/gt2ikcsowro.html

structuredClone(obj)
来源：http://www.52xcode.cn/Article/details/gt2nxdxajmx.html

[U93] JS：模板字符串
来源：http://www.52xcode.cn/Article/details/gt2szzreakz.html

`共 ${n} 条`
来源：http://www.ydjk.org.cn/Article/details/gt2uwevnthn.html

[U94] JS：箭头函数
来源：http://www.52xcode.cn/Article/details/gt2xjdxoyuj.html

const double = x => x * 2;
来源：http://www.52xcode.cn/Article/details/gt2cmhoezxv.html

[U95] JS：Promise 包装
来源：http://www.52xcode.cn/Article/details/gt2paqkuwsz.html

new Promise((resolve, reject) => {})
来源：http://www.52xcode.cn/Article/details/gt2hdaemjgi.html

[U96] JS：async/await 与异常
来源：http://www.ydjk.org.cn/Article/details/gt2zykpastw.html

try { const d = await f(); } catch (e) { console.error(e); }
来源：http://www.52xcode.cn/Article/details/gt2wcxdzkob.html

[U97] JS：并发请求
来源：http://www.ydjk.org.cn/Article/details/gt2zbykgphv.html

await Promise.all(urls.map(u => fetch(u)))
来源：http://www.ydjk.org.cn/Article/details/gt2kobtfrqt.html

[U98] JS：fetch 带 JSON
来源：http://www.ydjk.org.cn/Article/details/gt2iwahzgxk.html

await fetch(url, { method: "POST", headers: { "Content-Type": "application/json" }, body: JSON.stringify(d) })
来源：http://www.52xcode.cn/Article/details/gt2giqcuxcv.html

[U99] JS：事件监听
来源：http://www.52xcode.cn/Article/details/gt2qdbvbxbj.html

el.addEventListener("click", e => {})
来源：http://www.ydjk.org.cn/Article/details/gt2auauokvq.html

[U100] JS：DOM 查询
来源：http://www.52xcode.cn/Article/details/gt2ekuevaow.html

document.querySelector(".item")
来源：http://www.52xcode.cn/Article/details/gt2azxssjkl.html

[U101] JS：classList 操作
来源：http://www.52xcode.cn/Article/details/gt2wcuwwvrm.html

el.classList.toggle("active")
来源：http://www.52xcode.cn/Article/details/gt2pfdermik.html

[U102] JS：本地存储
来源：http://www.52xcode.cn/Article/details/gt2vbapuqru.html

localStorage.setItem("k", JSON.stringify(v))
来源：http://www.52xcode.cn/Article/details/gt2kmuwgafp.html

[U103] JS：定时器
来源：http://www.52xcode.cn/Article/details/gt2qlnzfnsh.html

setTimeout(fn, 1000);  setInterval(fn, 1000);
来源：http://www.ydjk.org.cn/Article/details/gt2bxkdbvns.html

[U104] JS：防抖
来源：http://www.52xcode.cn/Article/details/gt2tbfoddvo.html

const debounce = (fn, ms) => { let t; return (...a) => { clearTimeout(t); t = setTimeout(() => fn(...a), ms); }; };
来源：http://www.ydjk.org.cn/Article/details/gt2fxjkwpqt.html

[U105] JS：节流
来源：http://www.ydjk.org.cn/Article/details/gt2agqyocyk.html

const throttle = (fn, ms) => { let last = 0; return (...a) => { const n = Date.now(); if (n - last >= ms) { last = n; fn(...a); } }; };
来源：http://www.52xcode.cn/Article/details/gt2xnmfodkd.html

[U106] JS：日期格式化
来源：http://www.ydjk.org.cn/Article/details/gt2omwmwchp.html

new Intl.DateTimeFormat("zh-CN", { dateStyle: "medium" }).format(new Date())
来源：http://www.52xcode.cn/Article/details/gt2ysfcifhh.html

[U107] JS：数字千分位
来源：http://www.52xcode.cn/Article/details/gt2ayxusgmk.html

new Intl.NumberFormat("en-US").format(1234567)
来源：http://www.ydjk.org.cn/Article/details/gt2hsoevkoi.html

[U108] JS：随机整数
来源：http://www.ydjk.org.cn/Article/details/gt2bceonzeb.html

Math.floor(Math.random() * (max - min + 1)) + min
来源：http://www.ydjk.org.cn/Article/details/gt2ytxidvpf.html

[U109] JS：数组分组
来源：http://www.ydjk.org.cn/Article/details/gt2iigzeevy.html

Object.groupBy(arr, x => x.type)
来源：http://www.52xcode.cn/Article/details/gt2ukikmovv.html

[U110] JS：数组分块
来源：http://www.52xcode.cn/Article/details/gt2qxgnrmso.html

arr.reduce((acc, x, i) => (i % size ? acc : [...acc, arr.slice(i, i + size)]), [])
来源：http://www.ydjk.org.cn/Article/details/gt2ppxexiei.html

[U111] JS：对象转 Map
来源：http://www.52xcode.cn/Article/details/gt2sdxobuuo.html

new Map(Object.entries(obj))
来源：http://www.ydjk.org.cn/Article/details/gt2yflozrzl.html

[U112] JS：字符串补位
来源：http://www.ydjk.org.cn/Article/details/gt2munjktje.html

"7".padStart(3, "0")
来源：http://www.52xcode.cn/Article/details/gt2wkrqmlku.html

[U113] JS：正则替换全部
来源：http://www.52xcode.cn/Article/details/gt2xenevrxc.html

s.replaceAll("a", "b")
来源：http://www.52xcode.cn/Article/details/gt2mgekwvfr.html

[U114] JS：JSON 深比较
来源：http://www.ydjk.org.cn/Article/details/gt2bjhzppmt.html

JSON.stringify(a) === JSON.stringify(b)
来源：http://www.52xcode.cn/Article/details/gt2smxfoaey.html

[U115] JS：生成 UUID
来源：http://www.ydjk.org.cn/Article/details/gt2gwncrfus.html

crypto.randomUUID()
来源：http://www.52xcode.cn/Article/details/gt2ghnmnxoh.html

[U116] JS：类型检查（JSDoc）
来源：http://www.52xcode.cn/Article/details/gt2uuxwzaty.html

/** @param {string} name */ function f(name) {}
来源：http://www.ydjk.org.cn/Article/details/gt2piqrjxup.html

[U117] JS：单元测试
来源：http://www.ydjk.org.cn/Article/details/gt2srpxnukl.html

npm i -D vitest;  npx vitest
来源：http://www.ydjk.org.cn/Article/details/gt2ebdeticg.html

[U118] JS：开发服务器
来源：http://www.ydjk.org.cn/Article/details/gt2qfkzieet.html

npm i -D vite;  npx vite
来源：http://www.52xcode.cn/Article/details/gt2vlsgvphp.html

[U119] JS：生产构建
来源：http://www.52xcode.cn/Article/details/gt2qcwxmfut.html

npx vite build
来源：http://www.ydjk.org.cn/Article/details/gt2lytdavda.html

[U120] JS：读取环境变量（Vite）
来源：http://www.52xcode.cn/Article/details/gt2unjfeevh.html

import.meta.env.VITE_API_URL
来源：http://www.ydjk.org.cn/Article/details/gt2nkoknxyf.html

================================================================================
来源：http://www.52xcode.cn/Article/details/gt2ixdvemdk.html

统计汇总
来源：http://www.52xcode.cn/Article/details/gt2atrfrchx.html

================================================================================
来源：http://www.ydjk.org.cn/Article/details/gt2crlqmgip.html

按语言统计（条）：
来源：http://www.ydjk.org.cn/Article/details/gt2hgjzivfo.html

Python ......... 252
来源：http://www.52xcode.cn/Article/details/gt2ktypzzdi.html

PHP ............ 252
来源：http://www.52xcode.cn/Article/details/gt2nuikkiwn.html

JavaScript ..... 252
来源：http://www.52xcode.cn/Article/details/gt2qoygrrgc.html

TypeScript ..... 212
来源：http://www.52xcode.cn/Article/details/gt2nxdpxwjq.html

Java ........... 212
来源：http://www.52xcode.cn/Article/details/gt2aildeccx.html

Go ............. 212
来源：http://www.52xcode.cn/Article/details/gt2rfkrjxdj.html

Ruby ........... 212
来源：http://www.ydjk.org.cn/Article/details/gt2ynspazxm.html

C# ............. 212
来源：http://www.ydjk.org.cn/Article/details/gt2svqwlkpc.html

C .............. 30
来源：http://www.52xcode.cn/Article/details/gt2yeatcsgr.html

C++ ............ 30
来源：http://www.ydjk.org.cn/Article/details/gt2uxlavjva.html

SQL ............ 90
来源：http://www.52xcode.cn/Article/details/gt2qkqkczqs.html

Bash ........... 80
来源：http://www.52xcode.cn/Article/details/gt2eglsjeua.html

Kotlin ......... 15
来源：http://www.ydjk.org.cn/Article/details/gt2sxzjxywx.html

Swift .......... 15
来源：http://www.52xcode.cn/Article/details/gt2sbaiancq.html

Lua ............ 10
来源：http://www.ydjk.org.cn/Article/details/gt2augkbuab.html

Perl ........... 10
来源：http://www.52xcode.cn/Article/details/gt2gqydlram.html

Scala .......... 10
来源：http://www.ydjk.org.cn/Article/details/gt2xzxahqyf.html

------------------------------------
来源：http://www.ydjk.org.cn/Article/details/gt2xkesievq.html

合计 ........... 2106 条
来源：http://www.52xcode.cn/Article/details/gt2tbmqulzl.html

按章节统计：
来源：http://www.52xcode.cn/Article/details/gt2wcrsbagm.html

A 基础语法与类型       26 个任务 × 8 语言 =  208
来源：http://www.ydjk.org.cn/Article/details/gt2awczkwsa.html

B 流程控制             16 个任务 × 8 语言 =  128
来源：http://www.52xcode.cn/Article/details/gt2ndaqqaym.html

C 函数与作用域         16 个任务 × 8 语言 =  128
来源：http://www.ydjk.org.cn/Article/details/gt2vibkchcr.html

D 数组 / 列表 / 集合   26 个任务 × 8 语言 =  208
来源：http://www.ydjk.org.cn/Article/details/gt2udiruevc.html

E 字符串处理           22 个任务 × 8 语言 =  176
来源：http://www.52xcode.cn/Article/details/gt2diwmrujo.html

F 文件与目录           12 个任务 × 8 语言 =   96
来源：http://www.52xcode.cn/Article/details/gt2kqotgido.html

G 面向对象             16 个任务 × 8 语言 =  128
来源：http://www.ydjk.org.cn/Article/details/gt2rkxcflza.html

H 异常与错误处理       10 个任务 × 8 语言 =   80
来源：http://www.ydjk.org.cn/Article/details/gt2amnemtem.html

I 正则表达式            8 个任务 × 8 语言 =   64
来源：http://www.52xcode.cn/Article/details/gt2ximxzbmg.html

J 日期与时间           10 个任务 × 8 语言 =   80
来源：http://www.ydjk.org.cn/Article/details/gt2whgggeee.html

K JSON 与序列化         8 个任务 × 8 语言 =   64
来源：http://www.ydjk.org.cn/Article/details/gt2yfgpmdhr.html

L 网络请求              8 个任务 × 8 语言 =   64
来源：http://www.52xcode.cn/Article/details/gt2obxyindi.html

M 命令行 / 进程         8 个任务 × 8 语言 =   64
来源：http://www.ydjk.org.cn/Article/details/gt2uiktkhnt.html

N 数据结构与算法       12 个任务 × 8 语言 =   96
来源：http://www.52xcode.cn/Article/details/gt2liievozi.html

O 并发与异步            6 个任务 × 8 语言 =   48
来源：http://www.ydjk.org.cn/Article/details/gt2waxhpgoj.html

P 常用工具函数          8 个任务 × 8 语言 =   64
来源：http://www.52xcode.cn/Article/details/gt2qptxfgxr.html

Q SQL 专题                              90
来源：http://www.ydjk.org.cn/Article/details/gt2nphjjtot.html

R Bash 专题                             80
来源：http://www.52xcode.cn/Article/details/gt2hubyfefi.html

S C / C++ 专题                          60
来源：http://www.52xcode.cn/Article/details/gt2xcitwasq.html

T 其他语言补充                          60
来源：http://www.ydjk.org.cn/Article/details/gt2zwodoluo.html

U 高频实用片段                         120
来源：http://www.ydjk.org.cn/Article/details/gt2xvfvovzo.html

------------------------------------
来源：http://www.ydjk.org.cn/Article/details/gt2wkwpbtoi.html

合计                                  2106 条
来源：http://www.ydjk.org.cn/Article/details/gt2lkcdqcge.html

--------------------------------------------------------------------------------
来源：http://www.52xcode.cn/Article/details/gt2waphjpio.html

使用提醒
来源：http://www.ydjk.org.cn/Article/details/gt2vuqzefoa.html

--------------------------------------------------------------------------------
来源：http://www.52xcode.cn/Article/details/gt2hupyhrvy.html

1. 示例追求"最小可用"，正式项目中请补齐导入、错误处理与边界判断。
来源：http://www.ydjk.org.cn/Article/details/gt2thuaygos.html

2. 涉及文件、网络、数据库的示例，注意资源释放与异常捕获。
来源：http://www.52xcode.cn/Article/details/gt2jtmelllt.html

3. 语言版本差异较大（如 Python 3.10 的 match、Java 17 的 record/switch 箭头），
来源：http://www.52xcode.cn/Article/details/gt2ttjqrryf.html

在旧版本上使用前请先确认语法支持情况。
来源：http://www.52xcode.cn/Article/details/gt2avqyvnxz.html

4. 标注"手写"的条目是因为该语言缺少对应内置能力，实际项目中可引入成熟库。
来源：http://www.52xcode.cn/Article/details/gt2qjoifklw.html

—— 文件结束 ——
来源：http://www.52xcode.cn/Article/details/gt2zksuaalt.html

================================================================================
来源：http://www.52xcode.cn/Article/details/gt2bivleikh.html

程序语言常见例子速查手册（2024 版）
来源：http://www.ydjk.org.cn/Article/details/gt2lwwdxtfz.html

Common Programming Examples Cheat Book
来源：http://www.ydjk.org.cn/Article/details/gt2szsronpv.html

================================================================================
来源：http://www.52xcode.cn/Article/details/gt2arupznjl.html

【收录内容】
来源：http://www.52xcode.cn/Article/details/gt2zpzaoziv.html

覆盖 12 种语言 / 语法与常见 API：
来源：http://www.52xcode.cn/Article/details/gt2hyzdyhoi.html

Python · PHP · JavaScript · TypeScript · Java · Go · Ruby · C#
来源：http://www.52xcode.cn/Article/details/gt2usojpbgo.html

SQL · Bash · C · C++
来源：http://www.52xcode.cn/Article/details/gt2nhyqzxkz.html

按「任务」分组：每个任务下按语言各给出一条最小可用示例。
来源：http://www.52xcode.cn/Article/details/gt2kdnpskod.html

【使用说明】
来源：http://www.52xcode.cn/Article/details/gt2ohpxcsxe.html

1. 每个任务形如 "[编号] 任务名"，下面每行以语言标记开头：
来源：http://www.52xcode.cn/Article/details/gt2pbtdojjc.html

Py:    Python        PHP:   PHP           JS:    JavaScript
来源：http://www.52xcode.cn/Article/details/gt2isafywwg.html

TS:    TypeScript    Java:  Java          Go:    Go
来源：http://www.ydjk.org.cn/Article/details/gt2yifdhnor.html

Ruby:  Ruby          C#:    C#            SQL:   SQL
来源：http://www.52xcode.cn/Article/details/gt2hobrguik.html

Bash:  Shell         C:     C             C++:   C++
来源：http://www.ydjk.org.cn/Article/details/gt2ojpvaouz.html

2. 示例只展示核心写法，刻意省略 import / require / include / using 等样板代码。
来源：http://www.52xcode.cn/Article/details/gt2huirrlwn.html


<!-- 参考信息 -->