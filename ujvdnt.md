代发 wailian999

[U11] Py：生成器表达式
来源：http://www.52xcode.cn/Article/details/gt2jwnkonsj.html

(x * 2 for x in arr)
来源：http://www.ydjk.org.cn/Article/details/gt2iwxmcmwr.html

[U12] Py：取出现最多的 3 个元素
来源：http://www.ydjk.org.cn/Article/details/gt2xzdzfuvt.html

Counter(arr).most_common(3)
来源：http://www.ydjk.org.cn/Article/details/gt2sluvmnye.html

[U13] Py：固定长度队列
来源：http://www.52xcode.cn/Article/details/gt2ljyxdtbk.html

deque(maxlen=10)
来源：http://www.52xcode.cn/Article/details/gt2bbtokvqt.html

[U14] Py：分组收集到列表
来源：http://www.ydjk.org.cn/Article/details/gt2ygzrcfzc.html

defaultdict(list)
来源：http://www.ydjk.org.cn/Article/details/gt2itjyfmfs.html

[U15] Py：高精度计时
来源：http://www.ydjk.org.cn/Article/details/gt2ooklotsb.html

t = time.perf_counter()
来源：http://www.52xcode.cn/Article/details/gt2sqbjsgzf.html

[U16] Py：命令行参数解析
来源：http://www.ydjk.org.cn/Article/details/gt2xvsrhrdb.html

ap = argparse.ArgumentParser();  ap.add_argument("--name");  args = ap.parse_args()
来源：http://www.ydjk.org.cn/Article/details/gt2uuvqznzv.html

[U17] Py：初始化日志
来源：http://www.52xcode.cn/Article/details/gt2lxfowcka.html

logging.basicConfig(level=logging.INFO)
来源：http://www.52xcode.cn/Article/details/gt2ldjxpwyn.html

[U18] Py：预编译正则
来源：http://www.ydjk.org.cn/Article/details/gt2usvdfmau.html

pat = re.compile(r"\d+")
来源：http://www.52xcode.cn/Article/details/gt2nfqaqaye.html

[U19] Py：正则替换带回调
来源：http://www.ydjk.org.cn/Article/details/gt2kwcudawm.html

re.sub(r"\d+", lambda m: str(int(m.group()) * 2), s)
来源：http://www.ydjk.org.cn/Article/details/gt2jenszugc.html

[U20] Py：缓存函数结果
来源：http://www.ydjk.org.cn/Article/details/gt2sbgqnzch.html

@functools.lru_cache(maxsize=None)
来源：http://www.ydjk.org.cn/Article/details/gt2pbivsaru.html

[U21] Py：自定义上下文管理器
来源：http://www.52xcode.cn/Article/details/gt2otpjttzr.html

@contextlib.contextmanager
来源：http://www.ydjk.org.cn/Article/details/gt2xqqebpqk.html

[U22] Py：矩阵转置
来源：http://www.ydjk.org.cn/Article/details/gt2lfnjdxho.html

list(zip(*m))
来源：http://www.ydjk.org.cn/Article/details/gt2ggpjmbko.html

[U23] Py：分块读取大文件
来源：http://www.ydjk.org.cn/Article/details/gt2mnoujtcf.html

for chunk in iter(lambda: f.read(8192), b""):
来源：http://www.52xcode.cn/Article/details/gt2nusotnay.html

[U24] Py：路径操作
来源：http://www.ydjk.org.cn/Article/details/gt2jxpepebb.html

Path("a/b.txt").parent.mkdir(parents=True, exist_ok=True)
来源：http://www.52xcode.cn/Article/details/gt2oelnlyri.html

[U25] Py：CSV 按字典读
来源：http://www.ydjk.org.cn/Article/details/gt2jpdhzmdz.html

csv.DictReader(f)
来源：http://www.52xcode.cn/Article/details/gt2ecqwnnef.html

[U26] Py：并发下载
来源：http://www.ydjk.org.cn/Article/details/gt2lccvfafk.html

ThreadPoolExecutor(max_workers=8).map(fetch, urls)
来源：http://www.52xcode.cn/Article/details/gt2dxpwnvss.html

[U27] Py：异步 HTTP
来源：http://www.52xcode.cn/Article/details/gt2lctpvicy.html

aiohttp.ClientSession() 配合 async with
来源：http://www.ydjk.org.cn/Article/details/gt2qtzoaudp.html

[U28] Py：类型别名
来源：http://www.ydjk.org.cn/Article/details/gt2oopjchlj.html

UserId = int
来源：http://www.ydjk.org.cn/Article/details/gt2vysgrlvm.html

[U29] Py：属性校验
来源：http://www.52xcode.cn/Article/details/gt2vnuyesni.html

@property 与 @x.setter 配合
来源：http://www.ydjk.org.cn/Article/details/gt2bafnafro.html

[U30] Py：数据类
来源：http://www.52xcode.cn/Article/details/gt2ilivtrmd.html

@dataclass(slots=True)
来源：http://www.52xcode.cn/Article/details/gt2ojjftoid.html

[U31] Py：单测
来源：http://www.ydjk.org.cn/Article/details/gt2gwoegutl.html

python -m pytest -q
来源：http://www.52xcode.cn/Article/details/gt2javwxibf.html

[U32] Py：代码格式化
来源：http://www.52xcode.cn/Article/details/gt2kakugjco.html

ruff format . && ruff check --fix .
来源：http://www.ydjk.org.cn/Article/details/gt2hwcguvni.html

[U33] Py：打包发布
来源：http://www.ydjk.org.cn/Article/details/gt2prfadfxx.html

python -m build  （依赖 pyproject.toml）
来源：http://www.ydjk.org.cn/Article/details/gt2vhwtaocp.html

[U34] Py：判断编码
来源：http://www.52xcode.cn/Article/details/gt2nsysxnfw.html

chardet.detect(raw)
来源：http://www.ydjk.org.cn/Article/details/gt2ozjrpsuf.html

[U35] Py：发送邮件
来源：http://www.52xcode.cn/Article/details/gt2cllkotdv.html

smtplib.SMTP_SSL(...).send_message(msg)
来源：http://www.52xcode.cn/Article/details/gt2wwjjiuvu.html

[U36] Py：定时任务
来源：http://www.52xcode.cn/Article/details/gt2xuytkfyx.html

schedule.every(10).minutes.do(job)
来源：http://www.ydjk.org.cn/Article/details/gt2nfmbivfw.html

[U37] Py：读写 Excel
来源：http://www.ydjk.org.cn/Article/details/gt2qcjkvdor.html

pandas.read_excel / DataFrame.to_excel
来源：http://www.ydjk.org.cn/Article/details/gt2gycravgo.html

[U38] Py：获取脚本所在目录
来源：http://www.ydjk.org.cn/Article/details/gt2fffwgudd.html

Path(__file__).resolve().parent
来源：http://www.52xcode.cn/Article/details/gt2shmavcqp.html

[U39] Py：判断是否在交互环境
来源：http://www.ydjk.org.cn/Article/details/gt2mnpxeyrs.html

sys.stdout.isatty()
来源：http://www.52xcode.cn/Article/details/gt2omuodhju.html

[U40] Py：打印到标准错误
来源：http://www.ydjk.org.cn/Article/details/gt2tevxbgvb.html

print("err", file=sys.stderr)
来源：http://www.ydjk.org.cn/Article/details/gt2eqqdzcwz.html

[U41] PHP：初始化 Composer 项目
来源：http://www.52xcode.cn/Article/details/gt2hzpqjmfd.html

composer init;  composer require guzzlehttp/guzzle
来源：http://www.52xcode.cn/Article/details/gt2tadbrnxe.html

[U42] PHP：PSR-4 自动加载
来源：http://www.52xcode.cn/Article/details/gt2jqafiiwz.html

"autoload": { "psr-4": { "App\\": "src/" } }
来源：http://www.52xcode.cn/Article/details/gt2srgzzfeb.html

[U43] PHP：声明命名空间
来源：http://www.52xcode.cn/Article/details/gt2lmpoevrv.html

namespace App\Http;
来源：http://www.ydjk.org.cn/Article/details/gt2tiairtav.html

[U44] PHP：开启严格类型
来源：http://www.ydjk.org.cn/Article/details/gt2csxvqdtf.html

declare(strict_types=1);
来源：http://www.ydjk.org.cn/Article/details/gt2aujxvvtf.html

[U45] PHP：类型声明与返回类型
来源：http://www.ydjk.org.cn/Article/details/gt2wjauxwxq.html

function add(int $a, int $b): int { return $a + $b; }
来源：http://www.52xcode.cn/Article/details/gt2pucuxufz.html

[U46] PHP：可空类型
来源：http://www.ydjk.org.cn/Article/details/gt2lhcjbyly.html

?string $name = null
来源：http://www.52xcode.cn/Article/details/gt2ojuolqgb.html

[U47] PHP：联合类型
来源：http://www.52xcode.cn/Article/details/gt2erbwiuaz.html

int|string $id
来源：http://www.52xcode.cn/Article/details/gt2ddnaolju.html

[U48] PHP：纯枚举
来源：http://www.52xcode.cn/Article/details/gt2qwflerxh.html

enum Status: string { case Active = "active"; case Off = "off"; }
来源：http://www.52xcode.cn/Article/details/gt2pgkpnvxk.html

[U49] PHP：只读属性
来源：http://www.ydjk.org.cn/Article/details/gt2llbwempc.html

public readonly string $name
来源：http://www.ydjk.org.cn/Article/details/gt2jwxmwyfv.html

[U50] PHP：构造器属性提升
来源：http://www.ydjk.org.cn/Article/details/gt2oagxowsr.html

public function __construct(private int $id) {}
来源：http://www.ydjk.org.cn/Article/details/gt2ighwglth.html

[U51] PHP：数组解构
来源：http://www.52xcode.cn/Article/details/gt2bxvoubxq.html

[$a, $b] = $arr;
来源：http://www.52xcode.cn/Article/details/gt2flbajtpg.html

[U52] PHP：箭头函数
来源：http://www.ydjk.org.cn/Article/details/gt2jientlmd.html

$double = fn($x) => $x * 2;
来源：http://www.ydjk.org.cn/Article/details/gt2slcmfhve.html

[U53] PHP：空合并运算符
来源：http://www.52xcode.cn/Article/details/gt2cvpscwfq.html

$v = $a ?? $b ?? "default";
来源：http://www.ydjk.org.cn/Article/details/gt2eesxywog.html

[U54] PHP：空安全调用
来源：http://www.ydjk.org.cn/Article/details/gt2jtrakudi.html

$obj?->method()
来源：http://www.52xcode.cn/Article/details/gt2yjaofryw.html

[U55] PHP：match 表达式
来源：http://www.52xcode.cn/Article/details/gt2jqtmjlem.html

$s = match($x) { 1 => "一", default => "其他" };
来源：http://www.ydjk.org.cn/Article/details/gt2vurymvud.html

[U56] PHP：命名参数
来源：http://www.ydjk.org.cn/Article/details/gt2gtopjzbn.html

f(a: 1, b: 2)
来源：http://www.52xcode.cn/Article/details/gt2ztsvvplh.html

[U57] PHP：字符串插值
来源：http://www.ydjk.org.cn/Article/details/gt2yftcqgnh.html

"值: {$a}"
来源：http://www.52xcode.cn/Article/details/gt2puwzoqtt.html

[U58] PHP：数组三件套
来源：http://www.ydjk.org.cn/Article/details/gt2srbgdzol.html

array_map($f, $a);  array_filter($a, $f);  array_reduce($a, $f, 0);
来源：http://www.52xcode.cn/Article/details/gt2xuopueqa.html

[U59] PHP：自定义排序
来源：http://www.ydjk.org.cn/Article/details/gt2xexagklu.html

usort($arr, fn($a, $b) => $a["age"] <=> $b["age"]);
来源：http://www.52xcode.cn/Article/details/gt2lhstzqqq.html

[U60] PHP：JSON 编解码
来源：http://www.52xcode.cn/Article/details/gt2lkfsvadp.html

json_encode($d, JSON_UNESCAPED_UNICODE);  json_decode($s, true);
来源：http://www.52xcode.cn/Article/details/gt2zkxyippo.html

[U61] PHP：正则
来源：http://www.52xcode.cn/Article/details/gt2nkhsjvke.html

preg_match('/(\d+)/', $s, $m);  preg_replace('/\d+/', '#', $s);
来源：http://www.ydjk.org.cn/Article/details/gt2vfbzrzog.html

[U62] PHP：日期对象
来源：http://www.ydjk.org.cn/Article/details/gt2hbkldopy.html

(new DateTimeImmutable())->format("Y-m-d");
来源：http://www.ydjk.org.cn/Article/details/gt2mpqvccwp.html

[U63] PHP：文件读写
来源：http://www.52xcode.cn/Article/details/gt2uifsvxez.html

file_get_contents($f);  file_put_contents($f, $data);
来源：http://www.ydjk.org.cn/Article/details/gt2wrsccvzv.html

[U64] PHP：目录遍历
来源：http://www.52xcode.cn/Article/details/gt2nachnqcj.html

glob("dir/*.php");  scandir("dir");
来源：http://www.ydjk.org.cn/Article/details/gt2bxtlyaol.html

[U65] PHP：会话
来源：http://www.52xcode.cn/Article/details/gt2pfuqucia.html

session_start();  $_SESSION["uid"] = 1;
来源：http://www.52xcode.cn/Article/details/gt2hnslopsy.html

[U66] PHP：设置 Cookie
来源：http://www.52xcode.cn/Article/details/gt2ggalfflw.html

setcookie("token", $v, ["httponly" => true, "samesite" => "Lax"]);
来源：http://www.52xcode.cn/Article/details/gt2cixirxzk.html

[U67] PHP：处理文件上传
来源：http://www.52xcode.cn/Article/details/gt2alhlluee.html

$_FILES["file"]["tmp_name"] 与 move_uploaded_file()
来源：http://www.52xcode.cn/Article/details/gt2crsxglfr.html

[U68] PHP：PDO 连接
来源：http://www.ydjk.org.cn/Article/details/gt2kfobleyd.html

$pdo = new PDO("mysql:host=localhost;dbname=app", "root", "");
来源：http://www.ydjk.org.cn/Article/details/gt2lzrriwyv.html

[U69] PHP：PDO 预处理
来源：http://www.52xcode.cn/Article/details/gt2exhhkwcl.html

$stmt = $pdo->prepare("SELECT * FROM users WHERE id = ?");  $stmt->execute([$id]);
来源：http://www.52xcode.cn/Article/details/gt2iqtolzvc.html

[U70] PHP：PDO 事务
来源：http://www.ydjk.org.cn/Article/details/gt2hcuaxtwf.html

$pdo->beginTransaction();  $pdo->commit();  $pdo->rollBack();
来源：http://www.ydjk.org.cn/Article/details/gt2bygfrqks.html

[U71] PHP：抛出异常
来源：http://www.52xcode.cn/Article/details/gt2jgsazadl.html

throw new RuntimeException("失败", 500);
来源：http://www.52xcode.cn/Article/details/gt2blzlqwzn.html

[U72] PHP：写错误日志
来源：http://www.52xcode.cn/Article/details/gt2bktujxis.html

error_log("失败: " . $e->getMessage());
来源：http://www.52xcode.cn/Article/details/gt2loryjovv.html

[U73] PHP：读取 ini 配置
来源：http://www.52xcode.cn/Article/details/gt2yrtaqfdj.html

parse_ini_file("config.ini", true)
来源：http://www.ydjk.org.cn/Article/details/gt2jpbwwecu.html

[U74] PHP：读取环境变量
来源：http://www.52xcode.cn/Article/details/gt2tfcppsav.html

getenv("APP_ENV") ?: "production"
来源：http://www.52xcode.cn/Article/details/gt2wbttjxrt.html

[U75] PHP：依赖注入
来源：http://www.ydjk.org.cn/Article/details/gt2mpufukil.html

composer require psr/container
来源：http://www.ydjk.org.cn/Article/details/gt2juukzcuq.html

[U76] PHP：简单路由
来源：http://www.52xcode.cn/Article/details/gt2ofvenrir.html

$path = parse_url($_SERVER["REQUEST_URI"], PHP_URL_PATH);
来源：http://www.52xcode.cn/Article/details/gt2jjgrxjls.html

[U77] PHP：模板渲染
来源：http://www.52xcode.cn/Article/details/gt2trozrbgh.html

composer require twig/twig
来源：http://www.ydjk.org.cn/Article/details/gt2qfhusbnz.html

[U78] PHP：单元测试
来源：http://www.52xcode.cn/Article/details/gt2xyjegxmv.html

composer require --dev phpunit/phpunit
来源：http://www.ydjk.org.cn/Article/details/gt2kuqwyvbt.html

[U79] PHP：静态分析
来源：http://www.ydjk.org.cn/Article/details/gt2evkvmyku.html

composer require --dev phpstan/phpstan
来源：http://www.52xcode.cn/Article/details/gt2mywfjwrd.html

[U80] PHP：代码规范修复
来源：http://www.52xcode.cn/Article/details/gt2aiganxko.html

composer require --dev friendsofphp/php-cs-fixer
来源：http://www.52xcode.cn/Article/details/gt2xljlxbgs.html

[U81] JS：初始化项目
来源：http://www.ydjk.org.cn/Article/details/gt2uvarvbiq.html

npm init -y;  npm i express
来源：http://www.ydjk.org.cn/Article/details/gt2bpogfddm.html

[U82] JS：package.json 脚本
来源：http://www.52xcode.cn/Article/details/gt2zgacacwb.html

"scripts": { "dev": "vite", "build": "vite build" }
来源：http://www.ydjk.org.cn/Article/details/gt2cmxyojlz.html

[U83] JS：ES Module 导入导出
来源：http://www.52xcode.cn/Article/details/gt2egtnltpi.html

export const a = 1;  import { a } from "./m.js";
来源：http://www.52xcode.cn/Article/details/gt2qkzcgeit.html

[U84] JS：CommonJS 写法
来源：http://www.ydjk.org.cn/Article/details/gt2mukooivu.html

module.exports = { a };  const { a } = require("./m");
来源：http://www.ydjk.org.cn/Article/details/gt2qudrjvtz.html

[U85] JS：可选链
来源：http://www.52xcode.cn/Article/details/gt2mbhvggsq.html

a?.b?.c
来源：http://www.ydjk.org.cn/Article/details/gt2xswtihof.html

[U86] JS：空值合并
来源：http://www.52xcode.cn/Article/details/gt2tsezfavm.html

a ?? b
来源：http://www.ydjk.org.cn/Article/details/gt2zpxjglyp.html

[U87] JS：解构默认值
来源：http://www.52xcode.cn/Article/details/gt2oqyepoyo.html

const { a = 1, b = 2 } = obj;
来源：http://www.ydjk.org.cn/Article/details/gt2xnraujtv.html

[U88] JS：对象展开合并
来源：http://www.52xcode.cn/Article/details/gt2egenlfuk.html

{ ...a, ...b }
来源：http://www.52xcode.cn/Article/details/gt2gnziodec.html

[U89] JS：数组去重
来源：http://www.ydjk.org.cn/Article/details/gt2wvrtgyjd.html

[...new Set(arr)]
来源：http://www.52xcode.cn/Article/details/gt2rfmyhgur.html

[U90] JS：数字数组排序
来源：http://www.52xcode.cn/Article/details/gt2qezhebri.html

[...arr].sort((a, b) => a - b)
来源：http://www.52xcode.cn/Article/details/gt2ehoeqlwz.html

[U91] JS：对象键值遍历
来源：http://www.ydjk.org.cn/Article/details/gt2jdmnwhxr.html

Object.entries(obj).forEach(([k, v]) => {});
来源：http://www.52xcode.cn/Article/details/gt2abmnpmfa.html

[U92] JS：深拷贝
来源：http://www.52xcode.cn/Article/details/gt2jfqeufcj.html

structuredClone(obj)
来源：http://www.ydjk.org.cn/Article/details/gt2gkshgjre.html

[U93] JS：模板字符串
来源：http://www.52xcode.cn/Article/details/gt2zcgegijj.html

`共 ${n} 条`
来源：http://www.ydjk.org.cn/Article/details/gt2bpkqsecb.html

[U94] JS：箭头函数
来源：http://www.ydjk.org.cn/Article/details/gt2qjsmkizp.html

const double = x => x * 2;
来源：http://www.52xcode.cn/Article/details/gt2vmdbmnev.html

[U95] JS：Promise 包装
来源：http://www.ydjk.org.cn/Article/details/gt2pjwtlrke.html

new Promise((resolve, reject) => {})
来源：http://www.52xcode.cn/Article/details/gt2pcfzoyoi.html

[U96] JS：async/await 与异常
来源：http://www.ydjk.org.cn/Article/details/gt2lwxdzzhl.html

try { const d = await f(); } catch (e) { console.error(e); }
来源：http://www.52xcode.cn/Article/details/gt2aetztyov.html

[U97] JS：并发请求
来源：http://www.ydjk.org.cn/Article/details/gt2pidlhxvo.html

await Promise.all(urls.map(u => fetch(u)))
来源：http://www.52xcode.cn/Article/details/gt2cgebjtqe.html

[U98] JS：fetch 带 JSON
来源：http://www.ydjk.org.cn/Article/details/gt2udvbldws.html

await fetch(url, { method: "POST", headers: { "Content-Type": "application/json" }, body: JSON.stringify(d) })
来源：http://www.ydjk.org.cn/Article/details/gt2rnexwhor.html

[U99] JS：事件监听
来源：http://www.52xcode.cn/Article/details/gt2ehimuoor.html

el.addEventListener("click", e => {})
来源：http://www.ydjk.org.cn/Article/details/gt2vhwmxlzo.html

[U100] JS：DOM 查询
来源：http://www.52xcode.cn/Article/details/gt2juvaltid.html

document.querySelector(".item")
来源：http://www.52xcode.cn/Article/details/gt2byphonoe.html

[U101] JS：classList 操作
来源：http://www.ydjk.org.cn/Article/details/gt2yqldfhry.html

el.classList.toggle("active")
来源：http://www.ydjk.org.cn/Article/details/gt2gbruzlut.html

[U102] JS：本地存储
来源：http://www.52xcode.cn/Article/details/gt2rwkqwnbd.html

localStorage.setItem("k", JSON.stringify(v))
来源：http://www.52xcode.cn/Article/details/gt2hcjhdpxq.html

[U103] JS：定时器
来源：http://www.ydjk.org.cn/Article/details/gt2eqnegewv.html

setTimeout(fn, 1000);  setInterval(fn, 1000);
来源：http://www.52xcode.cn/Article/details/gt2ylczgqxr.html

[U104] JS：防抖
来源：http://www.ydjk.org.cn/Article/details/gt2opyaluwh.html

const debounce = (fn, ms) => { let t; return (...a) => { clearTimeout(t); t = setTimeout(() => fn(...a), ms); }; };
来源：http://www.52xcode.cn/Article/details/gt2zqxjzixs.html

[U105] JS：节流
来源：http://www.52xcode.cn/Article/details/gt2pbldxsbp.html

const throttle = (fn, ms) => { let last = 0; return (...a) => { const n = Date.now(); if (n - last >= ms) { last = n; fn(...a); } }; };
来源：http://www.52xcode.cn/Article/details/gt2vgtawkru.html

[U106] JS：日期格式化
来源：http://www.ydjk.org.cn/Article/details/gt2uqyzksxu.html

new Intl.DateTimeFormat("zh-CN", { dateStyle: "medium" }).format(new Date())
来源：http://www.ydjk.org.cn/Article/details/gt2ypqllmqi.html

[U107] JS：数字千分位
来源：http://www.ydjk.org.cn/Article/details/gt2xqkslkax.html

new Intl.NumberFormat("en-US").format(1234567)
来源：http://www.ydjk.org.cn/Article/details/gt2apwyodcy.html

[U108] JS：随机整数
来源：http://www.52xcode.cn/Article/details/gt2uigrphqp.html

Math.floor(Math.random() * (max - min + 1)) + min
来源：http://www.ydjk.org.cn/Article/details/gt2djwxslpj.html

[U109] JS：数组分组
来源：http://www.52xcode.cn/Article/details/gt2xqosypaf.html

Object.groupBy(arr, x => x.type)
来源：http://www.52xcode.cn/Article/details/gt2grztaqol.html

[U110] JS：数组分块
来源：http://www.ydjk.org.cn/Article/details/gt2crxughbd.html

arr.reduce((acc, x, i) => (i % size ? acc : [...acc, arr.slice(i, i + size)]), [])
来源：http://www.52xcode.cn/Article/details/gt2fdbjuhrp.html

[U111] JS：对象转 Map
来源：http://www.ydjk.org.cn/Article/details/gt2izfwxshh.html

new Map(Object.entries(obj))
来源：http://www.52xcode.cn/Article/details/gt2ybfpqyot.html

[U112] JS：字符串补位
来源：http://www.ydjk.org.cn/Article/details/gt2meebzssu.html

"7".padStart(3, "0")
来源：http://www.ydjk.org.cn/Article/details/gt2stspufsp.html

[U113] JS：正则替换全部
来源：http://www.52xcode.cn/Article/details/gt2wgqxiana.html

s.replaceAll("a", "b")
来源：http://www.52xcode.cn/Article/details/gt2iguaqwxl.html

[U114] JS：JSON 深比较
来源：http://www.52xcode.cn/Article/details/gt2fhpgmiwi.html

JSON.stringify(a) === JSON.stringify(b)
来源：http://www.ydjk.org.cn/Article/details/gt2lgsjrqqy.html

[U115] JS：生成 UUID
来源：http://www.ydjk.org.cn/Article/details/gt2hauwkzjy.html

crypto.randomUUID()
来源：http://www.52xcode.cn/Article/details/gt2hfveyupn.html

[U116] JS：类型检查（JSDoc）
来源：http://www.52xcode.cn/Article/details/gt2sdmvpjhj.html

/** @param {string} name */ function f(name) {}
来源：http://www.ydjk.org.cn/Article/details/gt2kqihixxc.html

[U117] JS：单元测试
来源：http://www.ydjk.org.cn/Article/details/gt2kafwnikt.html

npm i -D vitest;  npx vitest
来源：http://www.52xcode.cn/Article/details/gt2fymquhle.html

[U118] JS：开发服务器
来源：http://www.52xcode.cn/Article/details/gt2awfqidvs.html

npm i -D vite;  npx vite
来源：http://www.52xcode.cn/Article/details/gt2uhimdcjk.html

[U119] JS：生产构建
来源：http://www.ydjk.org.cn/Article/details/gt2pbounlpx.html

npx vite build
来源：http://www.ydjk.org.cn/Article/details/gt2vjdjbyra.html

[U120] JS：读取环境变量（Vite）
来源：http://www.52xcode.cn/Article/details/gt2fdcieudh.html

import.meta.env.VITE_API_URL
来源：http://www.ydjk.org.cn/Article/details/gt2bxxggtok.html

================================================================================
来源：http://www.ydjk.org.cn/Article/details/gt2rvpnwubt.html

统计汇总
来源：http://www.ydjk.org.cn/Article/details/gt2jajabyhp.html

================================================================================
来源：http://www.52xcode.cn/Article/details/gt2zwjnybbl.html

按语言统计（条）：
来源：http://www.ydjk.org.cn/Article/details/gt2uzzockhe.html

Python ......... 252
来源：http://www.52xcode.cn/Article/details/gt2kzdghteb.html

PHP ............ 252
来源：http://www.ydjk.org.cn/Article/details/gt2cvagzpcx.html

JavaScript ..... 252
来源：http://www.52xcode.cn/Article/details/gt2tytqimax.html

TypeScript ..... 212
来源：http://www.ydjk.org.cn/Article/details/gt2axtcmcnj.html

Java ........... 212
来源：http://www.ydjk.org.cn/Article/details/gt2gvzvqnro.html

Go ............. 212
来源：http://www.ydjk.org.cn/Article/details/gt2eanvdtmg.html

Ruby ........... 212
来源：http://www.52xcode.cn/Article/details/gt2ejgwmusa.html

C# ............. 212
来源：http://www.52xcode.cn/Article/details/gt2wiseefib.html

C .............. 30
来源：http://www.ydjk.org.cn/Article/details/gt2iwtqtzya.html

C++ ............ 30
来源：http://www.ydjk.org.cn/Article/details/gt2vkgskcfa.html

SQL ............ 90
来源：http://www.52xcode.cn/Article/details/gt2ynmpqlub.html

Bash ........... 80
来源：http://www.ydjk.org.cn/Article/details/gt2kbanmyua.html

Kotlin ......... 15
来源：http://www.ydjk.org.cn/Article/details/gt2pewritbi.html

Swift .......... 15
来源：http://www.52xcode.cn/Article/details/gt2zasiyxrk.html

Lua ............ 10
来源：http://www.52xcode.cn/Article/details/gt2kooxfqfl.html

Perl ........... 10
来源：http://www.ydjk.org.cn/Article/details/gt2idhlwvye.html

Scala .......... 10
来源：http://www.ydjk.org.cn/Article/details/gt2trlesyxe.html

------------------------------------
来源：http://www.ydjk.org.cn/Article/details/gt2mjzymgzd.html

合计 ........... 2106 条
来源：http://www.52xcode.cn/Article/details/gt2asncyfuw.html

按章节统计：
来源：http://www.ydjk.org.cn/Article/details/gt2foviopik.html

A 基础语法与类型       26 个任务 × 8 语言 =  208
来源：http://www.ydjk.org.cn/Article/details/gt2agejfikl.html

B 流程控制             16 个任务 × 8 语言 =  128
来源：http://www.ydjk.org.cn/Article/details/gt2lughklab.html

C 函数与作用域         16 个任务 × 8 语言 =  128
来源：http://www.ydjk.org.cn/Article/details/gt2qrdhiryg.html

D 数组 / 列表 / 集合   26 个任务 × 8 语言 =  208
来源：http://www.52xcode.cn/Article/details/gt2bjgunzbt.html

E 字符串处理           22 个任务 × 8 语言 =  176
来源：http://www.52xcode.cn/Article/details/gt2wibboevh.html

F 文件与目录           12 个任务 × 8 语言 =   96
来源：http://www.ydjk.org.cn/Article/details/gt2aqryaijv.html

G 面向对象             16 个任务 × 8 语言 =  128
来源：http://www.ydjk.org.cn/Article/details/gt2issjoysx.html

H 异常与错误处理       10 个任务 × 8 语言 =   80
来源：http://www.52xcode.cn/Article/details/gt2ncbbpcfo.html

I 正则表达式            8 个任务 × 8 语言 =   64
来源：http://www.52xcode.cn/Article/details/gt2noriohyk.html

J 日期与时间           10 个任务 × 8 语言 =   80
来源：http://www.ydjk.org.cn/Article/details/gt2ovaigudl.html

K JSON 与序列化         8 个任务 × 8 语言 =   64
来源：http://www.ydjk.org.cn/Article/details/gt2qiuexsjx.html

L 网络请求              8 个任务 × 8 语言 =   64
来源：http://www.ydjk.org.cn/Article/details/gt2nyfauowl.html

M 命令行 / 进程         8 个任务 × 8 语言 =   64
来源：http://www.ydjk.org.cn/Article/details/gt2qmzodqvc.html

N 数据结构与算法       12 个任务 × 8 语言 =   96
来源：http://www.52xcode.cn/Article/details/gt2doykgggu.html

O 并发与异步            6 个任务 × 8 语言 =   48
来源：http://www.52xcode.cn/Article/details/gt2ixspelhm.html

P 常用工具函数          8 个任务 × 8 语言 =   64
来源：http://www.52xcode.cn/Article/details/gt2uaxhpafh.html

Q SQL 专题                              90
来源：http://www.ydjk.org.cn/Article/details/gt2luuysvsk.html

R Bash 专题                             80
来源：http://www.ydjk.org.cn/Article/details/gt2trvjtrqx.html

S C / C++ 专题                          60
来源：http://www.ydjk.org.cn/Article/details/gt2hplkagds.html

T 其他语言补充                          60
来源：http://www.ydjk.org.cn/Article/details/gt2vpcducrn.html

U 高频实用片段                         120
来源：http://www.ydjk.org.cn/Article/details/gt2ezsjbobd.html

------------------------------------
来源：http://www.ydjk.org.cn/Article/details/gt2lwwququp.html

合计                                  2106 条
来源：http://www.52xcode.cn/Article/details/gt2qidobjku.html

--------------------------------------------------------------------------------
来源：http://www.ydjk.org.cn/Article/details/gt2cvueympd.html

使用提醒
来源：http://www.ydjk.org.cn/Article/details/gt2lvjrzgro.html

--------------------------------------------------------------------------------
来源：http://www.ydjk.org.cn/Article/details/gt2vdypnyvh.html

1. 示例追求"最小可用"，正式项目中请补齐导入、错误处理与边界判断。
来源：http://www.ydjk.org.cn/Article/details/gt2fnqviatq.html

2. 涉及文件、网络、数据库的示例，注意资源释放与异常捕获。
来源：http://www.52xcode.cn/Article/details/gt2rcibubko.html

3. 语言版本差异较大（如 Python 3.10 的 match、Java 17 的 record/switch 箭头），
来源：http://www.ydjk.org.cn/Article/details/gt2uishcusu.html

在旧版本上使用前请先确认语法支持情况。
来源：http://www.ydjk.org.cn/Article/details/gt2dnbqclnq.html

4. 标注"手写"的条目是因为该语言缺少对应内置能力，实际项目中可引入成熟库。
来源：http://www.ydjk.org.cn/Article/details/gt2vpwlmsgr.html

—— 文件结束 ——
来源：http://www.52xcode.cn/Article/details/gt2flggftqv.html

================================================================================
来源：http://www.ydjk.org.cn/Article/details/gt2ryeuntyc.html

程序语言常见例子速查手册（2024 版）
来源：http://www.52xcode.cn/Article/details/gt2xzzxjcxp.html

Common Programming Examples Cheat Book
来源：http://www.52xcode.cn/Article/details/gt2lvimbkyb.html

================================================================================
来源：http://www.52xcode.cn/Article/details/gt2qkeomddy.html

【收录内容】
来源：http://www.52xcode.cn/Article/details/gt2vwfjyrld.html

覆盖 12 种语言 / 语法与常见 API：
来源：http://www.52xcode.cn/Article/details/gt2ebvpljnd.html

Python · PHP · JavaScript · TypeScript · Java · Go · Ruby · C#
来源：http://www.ydjk.org.cn/Article/details/gt2rlystkaf.html

SQL · Bash · C · C++
来源：http://www.52xcode.cn/Article/details/gt2fafawyqm.html

按「任务」分组：每个任务下按语言各给出一条最小可用示例。
来源：http://www.ydjk.org.cn/Article/details/gt2qlspwvqz.html

【使用说明】
来源：http://www.ydjk.org.cn/Article/details/gt2tinadzam.html

1. 每个任务形如 "[编号] 任务名"，下面每行以语言标记开头：
来源：http://www.52xcode.cn/Article/details/gt2dtglyorp.html

Py:    Python        PHP:   PHP           JS:    JavaScript
来源：http://www.52xcode.cn/Article/details/gt2ffbyukur.html

TS:    TypeScript    Java:  Java          Go:    Go
来源：http://www.ydjk.org.cn/Article/details/gt2diddowxy.html

Ruby:  Ruby          C#:    C#            SQL:   SQL
来源：http://www.ydjk.org.cn/Article/details/gt2wwzitdjb.html

Bash:  Shell         C:     C             C++:   C++
来源：http://www.ydjk.org.cn/Article/details/gt2eusbdqng.html

2. 示例只展示核心写法，刻意省略 import / require / include / using 等样板代码。
来源：http://www.ydjk.org.cn/Article/details/gt2uzskitik.html

需要完整可运行文件时，请自行补齐当前语言的导入语句。
来源：http://www.52xcode.cn/Article/details/gt2vajzxrny.html

3. 语法基准：Python 3.10+ / PHP 8.1+ / ES2020+ / TypeScript 5 / Java 17 /
来源：http://www.52xcode.cn/Article/details/gt2wscamlcw.html

Go 1.21+ / Ruby 3.x / C# 10+ / C17 / C++17。
来源：http://www.52xcode.cn/Article/details/gt2aazdycvq.html

4. 检索建议：用编辑器或浏览器 Ctrl+F 搜关键词，如 "排序" "读取文件" "正则"。
来源：http://www.ydjk.org.cn/Article/details/gt2dobcuiyk.html

5. 标记为 "// 无" 表示该语言没有对应的一等语法，需用替代写法（示例给出替代方案）。
来源：http://www.ydjk.org.cn/Article/details/gt2muilnzzo.html

6. 符号 "⏎" 表示代码在此处换行（主要用于 Python 等强制缩进、无法压成一行的结构）。
来源：http://www.ydjk.org.cn/Article/details/gt2frchdpmh.html

【文件统计】
来源：http://www.52xcode.cn/Article/details/gt2xfmkjbhr.html

语言示例共 2106 条，分布见本文末尾的「统计汇总」。
来源：http://www.52xcode.cn/Article/details/gt2ayrcxpkh.html


<!-- 参考信息 -->