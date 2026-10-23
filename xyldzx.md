代发 wailian999

List(1, 2, 3).foldLeft(0)(_ + _)
来源：http://www.52xcode.cn/Article/details/gt3dxlhlxar.html

================================================================================
来源：http://www.52xcode.cn/Article/details/gt3fnlgllrf.html

U. 高频实用片段（Python / PHP / JavaScript 各 40 条）
来源：http://www.52xcode.cn/Article/details/gt3dynskihm.html

================================================================================
来源：http://www.ydjk.org.cn/Article/details/gt3upeprcpj.html

[U01] Py：创建虚拟环境
来源：http://www.52xcode.cn/Article/details/gt3lfuzwjdb.html

python -m venv .venv && source .venv/bin/activate
来源：http://www.ydjk.org.cn/Article/details/gt3lqjpskbv.html

[U02] Py：导出 / 安装依赖
来源：http://www.ydjk.org.cn/Article/details/gt3dervdips.html

pip freeze > requirements.txt;  pip install -r requirements.txt
来源：http://www.52xcode.cn/Article/details/gt3kgxkpjza.html

[U03] Py：加载 .env 配置
来源：http://www.ydjk.org.cn/Article/details/gt3lzeynfkd.html

from dotenv import load_dotenv; load_dotenv()
来源：http://www.52xcode.cn/Article/details/gt3ofrwpiix.html

[U04] Py：变量调试打印
来源：http://www.52xcode.cn/Article/details/gt3sgdkhciw.html

print(f"{x=}")            # 输出 x=值，Python 3.8+
来源：http://www.52xcode.cn/Article/details/gt3iukzimuh.html

[U05] Py：列表去重且保序
来源：http://www.52xcode.cn/Article/details/gt3jzyiszua.html

list(dict.fromkeys(arr))
来源：http://www.ydjk.org.cn/Article/details/gt3bfzshlzu.html

[U06] Py：合并两个字典
来源：http://www.ydjk.org.cn/Article/details/gt3dfglueww.html

{**a, **b}
来源：http://www.ydjk.org.cn/Article/details/gt3epqatyfz.html

[U07] Py：反转字典键值
来源：http://www.52xcode.cn/Article/details/gt3reqkwenp.html

{v: k for k, v in d.items()}
来源：http://www.52xcode.cn/Article/details/gt3ovtisrvd.html

[U08] Py：展平二维列表
来源：http://www.52xcode.cn/Article/details/gt3ypnpkqif.html

[y for x in nested for y in x]
来源：http://www.ydjk.org.cn/Article/details/gt3jhjkqxxh.html

[U09] Py：字典取最大值的键
来源：http://www.ydjk.org.cn/Article/details/gt3cvxnjaao.html

max(d, key=d.get)
来源：http://www.52xcode.cn/Article/details/gt3myrsrrmc.html

[U10] Py：按值排序字典
来源：http://www.52xcode.cn/Article/details/gt3klajcxci.html

dict(sorted(d.items(), key=lambda kv: kv[1]))
来源：http://www.52xcode.cn/Article/details/gt3tscljdag.html

[U11] Py：生成器表达式
来源：http://www.ydjk.org.cn/Article/details/gt3lxzfwrdt.html

(x * 2 for x in arr)
来源：http://www.ydjk.org.cn/Article/details/gt3qpzmmcmb.html

[U12] Py：取出现最多的 3 个元素
来源：http://www.52xcode.cn/Article/details/gt3ebjfbgme.html

Counter(arr).most_common(3)
来源：http://www.52xcode.cn/Article/details/gt3glxexwdt.html

[U13] Py：固定长度队列
来源：http://www.ydjk.org.cn/Article/details/gt3bubwtmro.html

deque(maxlen=10)
来源：http://www.ydjk.org.cn/Article/details/gt3wwvtqous.html

[U14] Py：分组收集到列表
来源：http://www.ydjk.org.cn/Article/details/gt3gcyducwc.html

defaultdict(list)
来源：http://www.52xcode.cn/Article/details/gt3ldvrdckk.html

[U15] Py：高精度计时
来源：http://www.52xcode.cn/Article/details/gt3zoogzefa.html

t = time.perf_counter()
来源：http://www.52xcode.cn/Article/details/gt3vkjjczev.html

[U16] Py：命令行参数解析
来源：http://www.ydjk.org.cn/Article/details/gt3pclddzef.html

ap = argparse.ArgumentParser();  ap.add_argument("--name");  args = ap.parse_args()
来源：http://www.ydjk.org.cn/Article/details/gt3yixyhvju.html

[U17] Py：初始化日志
来源：http://www.ydjk.org.cn/Article/details/gt3sdjpiozp.html

logging.basicConfig(level=logging.INFO)
来源：http://www.ydjk.org.cn/Article/details/gt3jwykwsmf.html

[U18] Py：预编译正则
来源：http://www.ydjk.org.cn/Article/details/gt3tdkoxfui.html

pat = re.compile(r"\d+")
来源：http://www.ydjk.org.cn/Article/details/gt3hmuvgqpg.html

[U19] Py：正则替换带回调
来源：http://www.52xcode.cn/Article/details/gt3zjgmnosl.html

re.sub(r"\d+", lambda m: str(int(m.group()) * 2), s)
来源：http://www.ydjk.org.cn/Article/details/gt3xwfdgvyu.html

[U20] Py：缓存函数结果
来源：http://www.ydjk.org.cn/Article/details/gt3oksqmyih.html

@functools.lru_cache(maxsize=None)
来源：http://www.52xcode.cn/Article/details/gt3ixrgeidy.html

[U21] Py：自定义上下文管理器
来源：http://www.ydjk.org.cn/Article/details/gt3hecvuljr.html

@contextlib.contextmanager
来源：http://www.ydjk.org.cn/Article/details/gt3hsfcgpfx.html

[U22] Py：矩阵转置
来源：http://www.ydjk.org.cn/Article/details/gt3jzogobda.html

list(zip(*m))
来源：http://www.52xcode.cn/Article/details/gt3rlnoxgzh.html

[U23] Py：分块读取大文件
来源：http://www.52xcode.cn/Article/details/gt3dhzoojtx.html

for chunk in iter(lambda: f.read(8192), b""):
来源：http://www.52xcode.cn/Article/details/gt3rasbvhqb.html

[U24] Py：路径操作
来源：http://www.ydjk.org.cn/Article/details/gt3xhbleqrc.html

Path("a/b.txt").parent.mkdir(parents=True, exist_ok=True)
来源：http://www.52xcode.cn/Article/details/gt3vfsnphuf.html

[U25] Py：CSV 按字典读
来源：http://www.ydjk.org.cn/Article/details/gt3zdhwpcfi.html

csv.DictReader(f)
来源：http://www.52xcode.cn/Article/details/gt3wsghraon.html

[U26] Py：并发下载
来源：http://www.ydjk.org.cn/Article/details/gt3prosqpft.html

ThreadPoolExecutor(max_workers=8).map(fetch, urls)
来源：http://www.ydjk.org.cn/Article/details/gt3tnnbwszv.html

[U27] Py：异步 HTTP
来源：http://www.ydjk.org.cn/Article/details/gt3spvciyyt.html

aiohttp.ClientSession() 配合 async with
来源：http://www.ydjk.org.cn/Article/details/gt3qokwmioa.html

[U28] Py：类型别名
来源：http://www.52xcode.cn/Article/details/gt3brjxpmfa.html

UserId = int
来源：http://www.52xcode.cn/Article/details/gt3ceupulpm.html

[U29] Py：属性校验
来源：http://www.52xcode.cn/Article/details/gt3oygwaquf.html

@property 与 @x.setter 配合
来源：http://www.52xcode.cn/Article/details/gt3diugjnhi.html

[U30] Py：数据类
来源：http://www.ydjk.org.cn/Article/details/gt3gwnhgyvc.html

@dataclass(slots=True)
来源：http://www.52xcode.cn/Article/details/gt3vovtxadv.html

[U31] Py：单测
来源：http://www.ydjk.org.cn/Article/details/gt3xevgsxvw.html

python -m pytest -q
来源：http://www.ydjk.org.cn/Article/details/gt3qiztiyxn.html

[U32] Py：代码格式化
来源：http://www.ydjk.org.cn/Article/details/gt3vwxzdmee.html

ruff format . && ruff check --fix .
来源：http://www.52xcode.cn/Article/details/gt3rxijpcse.html

[U33] Py：打包发布
来源：http://www.ydjk.org.cn/Article/details/gt3unzmwxvp.html

python -m build  （依赖 pyproject.toml）
来源：http://www.52xcode.cn/Article/details/gt3iexwbogv.html

[U34] Py：判断编码
来源：http://www.ydjk.org.cn/Article/details/gt3casdffai.html

chardet.detect(raw)
来源：http://www.ydjk.org.cn/Article/details/gt3bnnizcxr.html

[U35] Py：发送邮件
来源：http://www.52xcode.cn/Article/details/gt3yhvziedt.html

smtplib.SMTP_SSL(...).send_message(msg)
来源：http://www.52xcode.cn/Article/details/gt3sksjuqix.html

[U36] Py：定时任务
来源：http://www.52xcode.cn/Article/details/gt3hcfkqwsx.html

schedule.every(10).minutes.do(job)
来源：http://www.52xcode.cn/Article/details/gt3fjnnfpjh.html

[U37] Py：读写 Excel
来源：http://www.52xcode.cn/Article/details/gt3xncxmuxy.html

pandas.read_excel / DataFrame.to_excel
来源：http://www.52xcode.cn/Article/details/gt3zxdrdemd.html

[U38] Py：获取脚本所在目录
来源：http://www.ydjk.org.cn/Article/details/gt3qimupzgi.html

Path(__file__).resolve().parent
来源：http://www.ydjk.org.cn/Article/details/gt3rjqbcjof.html

[U39] Py：判断是否在交互环境
来源：http://www.52xcode.cn/Article/details/gt3tawqccmy.html

sys.stdout.isatty()
来源：http://www.ydjk.org.cn/Article/details/gt3reyvjyue.html

[U40] Py：打印到标准错误
来源：http://www.52xcode.cn/Article/details/gt3uaqvwbgz.html

print("err", file=sys.stderr)
来源：http://www.ydjk.org.cn/Article/details/gt3zhlelhnp.html

[U41] PHP：初始化 Composer 项目
来源：http://www.ydjk.org.cn/Article/details/gt3ftyzxtqw.html

composer init;  composer require guzzlehttp/guzzle
来源：http://www.52xcode.cn/Article/details/gt3jismawcg.html

[U42] PHP：PSR-4 自动加载
来源：http://www.ydjk.org.cn/Article/details/gt3wfmfyvyh.html

"autoload": { "psr-4": { "App\\": "src/" } }
来源：http://www.ydjk.org.cn/Article/details/gt3ywtlxzad.html

[U43] PHP：声明命名空间
来源：http://www.ydjk.org.cn/Article/details/gt3yoynvlxl.html

namespace App\Http;
来源：http://www.52xcode.cn/Article/details/gt3iqibclxi.html

[U44] PHP：开启严格类型
来源：http://www.ydjk.org.cn/Article/details/gt3fdxeucjr.html

declare(strict_types=1);
来源：http://www.52xcode.cn/Article/details/gt3hnjcwell.html

[U45] PHP：类型声明与返回类型
来源：http://www.ydjk.org.cn/Article/details/gt3grmsldpc.html

function add(int $a, int $b): int { return $a + $b; }
来源：http://www.52xcode.cn/Article/details/gt3fxshfwjn.html

[U46] PHP：可空类型
来源：http://www.52xcode.cn/Article/details/gt3dllojtpa.html

?string $name = null
来源：http://www.52xcode.cn/Article/details/gt3qpdmgpha.html

[U47] PHP：联合类型
来源：http://www.ydjk.org.cn/Article/details/gt3gdpqbdmd.html

int|string $id
来源：http://www.52xcode.cn/Article/details/gt3kmquedfp.html

[U48] PHP：纯枚举
来源：http://www.ydjk.org.cn/Article/details/gt3pejmuzhc.html

enum Status: string { case Active = "active"; case Off = "off"; }
来源：http://www.52xcode.cn/Article/details/gt3hgdqzgfk.html

[U49] PHP：只读属性
来源：http://www.52xcode.cn/Article/details/gt3ipcdpkjg.html

public readonly string $name
来源：http://www.52xcode.cn/Article/details/gt3xgbypymu.html

[U50] PHP：构造器属性提升
来源：http://www.52xcode.cn/Article/details/gt3iphoyuer.html

public function __construct(private int $id) {}
来源：http://www.52xcode.cn/Article/details/gt3pokrpath.html

[U51] PHP：数组解构
来源：http://www.ydjk.org.cn/Article/details/gt3ncijhdmu.html

[$a, $b] = $arr;
来源：http://www.52xcode.cn/Article/details/gt3piawcduo.html

[U52] PHP：箭头函数
来源：http://www.ydjk.org.cn/Article/details/gt3mbgxznfq.html

$double = fn($x) => $x * 2;
来源：http://www.ydjk.org.cn/Article/details/gt3godcbvuc.html

[U53] PHP：空合并运算符
来源：http://www.52xcode.cn/Article/details/gt3tvsaexau.html

$v = $a ?? $b ?? "default";
来源：http://www.52xcode.cn/Article/details/gt3bdestorl.html

[U54] PHP：空安全调用
来源：http://www.52xcode.cn/Article/details/gt3hgpeunli.html

$obj?->method()
来源：http://www.ydjk.org.cn/Article/details/gt3lrxsnecl.html

[U55] PHP：match 表达式
来源：http://www.52xcode.cn/Article/details/gt3wkzqrraz.html

$s = match($x) { 1 => "一", default => "其他" };
来源：http://www.52xcode.cn/Article/details/gt3ppbhhixi.html

[U56] PHP：命名参数
来源：http://www.ydjk.org.cn/Article/details/gt3wmvdjizn.html

f(a: 1, b: 2)
来源：http://www.52xcode.cn/Article/details/gt3eqfcawpk.html

[U57] PHP：字符串插值
来源：http://www.ydjk.org.cn/Article/details/gt3whqrwtgc.html

"值: {$a}"
来源：http://www.ydjk.org.cn/Article/details/gt3sevlzkxj.html

[U58] PHP：数组三件套
来源：http://www.52xcode.cn/Article/details/gt3rjdreene.html

array_map($f, $a);  array_filter($a, $f);  array_reduce($a, $f, 0);
来源：http://www.52xcode.cn/Article/details/gt3rehsdhei.html

[U59] PHP：自定义排序
来源：http://www.ydjk.org.cn/Article/details/gt3slsnhaku.html

usort($arr, fn($a, $b) => $a["age"] <=> $b["age"]);
来源：http://www.52xcode.cn/Article/details/gt3xsdqpljx.html

[U60] PHP：JSON 编解码
来源：http://www.52xcode.cn/Article/details/gt3yojkafcy.html

json_encode($d, JSON_UNESCAPED_UNICODE);  json_decode($s, true);
来源：http://www.52xcode.cn/Article/details/gt3kmvsaqyy.html

[U61] PHP：正则
来源：http://www.52xcode.cn/Article/details/gt3puctmbhe.html

preg_match('/(\d+)/', $s, $m);  preg_replace('/\d+/', '#', $s);
来源：http://www.52xcode.cn/Article/details/gt3mjvgpkla.html

[U62] PHP：日期对象
来源：http://www.ydjk.org.cn/Article/details/gt3tchuaqlw.html

(new DateTimeImmutable())->format("Y-m-d");
来源：http://www.ydjk.org.cn/Article/details/gt3yaiiigzw.html

[U63] PHP：文件读写
来源：http://www.52xcode.cn/Article/details/gt3ajbdeila.html

file_get_contents($f);  file_put_contents($f, $data);
来源：http://www.52xcode.cn/Article/details/gt3redizogx.html

[U64] PHP：目录遍历
来源：http://www.52xcode.cn/Article/details/gt3nqbtuihl.html

glob("dir/*.php");  scandir("dir");
来源：http://www.52xcode.cn/Article/details/gt3lgtrhocf.html

[U65] PHP：会话
来源：http://www.52xcode.cn/Article/details/gt3drwduzpo.html

session_start();  $_SESSION["uid"] = 1;
来源：http://www.52xcode.cn/Article/details/gt3dzzieowg.html

[U66] PHP：设置 Cookie
来源：http://www.52xcode.cn/Article/details/gt3zvuzxovh.html

setcookie("token", $v, ["httponly" => true, "samesite" => "Lax"]);
来源：http://www.52xcode.cn/Article/details/gt3xmxrrsld.html

[U67] PHP：处理文件上传
来源：http://www.ydjk.org.cn/Article/details/gt3gwhfvejq.html

$_FILES["file"]["tmp_name"] 与 move_uploaded_file()
来源：http://www.52xcode.cn/Article/details/gt3cthlrptx.html

[U68] PHP：PDO 连接
来源：http://www.ydjk.org.cn/Article/details/gt3ecjgiole.html

$pdo = new PDO("mysql:host=localhost;dbname=app", "root", "");
来源：http://www.ydjk.org.cn/Article/details/gt3ejqgaogj.html

[U69] PHP：PDO 预处理
来源：http://www.52xcode.cn/Article/details/gt3gizmihsf.html

$stmt = $pdo->prepare("SELECT * FROM users WHERE id = ?");  $stmt->execute([$id]);
来源：http://www.ydjk.org.cn/Article/details/gt3vbmuhmvv.html

[U70] PHP：PDO 事务
来源：http://www.ydjk.org.cn/Article/details/gt3eedeikha.html

$pdo->beginTransaction();  $pdo->commit();  $pdo->rollBack();
来源：http://www.ydjk.org.cn/Article/details/gt3sgjmdtpz.html

[U71] PHP：抛出异常
来源：http://www.ydjk.org.cn/Article/details/gt3mubricui.html

throw new RuntimeException("失败", 500);
来源：http://www.52xcode.cn/Article/details/gt3dybanuzi.html

[U72] PHP：写错误日志
来源：http://www.ydjk.org.cn/Article/details/gt3xeqbcosl.html

error_log("失败: " . $e->getMessage());
来源：http://www.52xcode.cn/Article/details/gt3couazeyp.html

[U73] PHP：读取 ini 配置
来源：http://www.52xcode.cn/Article/details/gt3swajerfu.html

parse_ini_file("config.ini", true)
来源：http://www.ydjk.org.cn/Article/details/gt3owdawoyp.html

[U74] PHP：读取环境变量
来源：http://www.52xcode.cn/Article/details/gt3dgrrqtqz.html

getenv("APP_ENV") ?: "production"
来源：http://www.52xcode.cn/Article/details/gt3ndseeveg.html

[U75] PHP：依赖注入
来源：http://www.ydjk.org.cn/Article/details/gt3mmhvylbb.html

composer require psr/container
来源：http://www.ydjk.org.cn/Article/details/gt3yixwnmrn.html

[U76] PHP：简单路由
来源：http://www.ydjk.org.cn/Article/details/gt3mbezbkhk.html

$path = parse_url($_SERVER["REQUEST_URI"], PHP_URL_PATH);
来源：http://www.52xcode.cn/Article/details/gt3wuahgmpp.html

[U77] PHP：模板渲染
来源：http://www.ydjk.org.cn/Article/details/gt3zplacufc.html

composer require twig/twig
来源：http://www.52xcode.cn/Article/details/gt3vpmzqowb.html

[U78] PHP：单元测试
来源：http://www.ydjk.org.cn/Article/details/gt3jggtinnj.html

composer require --dev phpunit/phpunit
来源：http://www.ydjk.org.cn/Article/details/gt3sozlqcwj.html

[U79] PHP：静态分析
来源：http://www.52xcode.cn/Article/details/gt3odphyxdn.html

composer require --dev phpstan/phpstan
来源：http://www.ydjk.org.cn/Article/details/gt3dgemweqa.html

[U80] PHP：代码规范修复
来源：http://www.ydjk.org.cn/Article/details/gt3fbeamrgn.html

composer require --dev friendsofphp/php-cs-fixer
来源：http://www.52xcode.cn/Article/details/gt3gmymueyt.html

[U81] JS：初始化项目
来源：http://www.52xcode.cn/Article/details/gt3ailwmfta.html

npm init -y;  npm i express
来源：http://www.ydjk.org.cn/Article/details/gt3fohoumjr.html

[U82] JS：package.json 脚本
来源：http://www.ydjk.org.cn/Article/details/gt3zymqqfjy.html

"scripts": { "dev": "vite", "build": "vite build" }
来源：http://www.ydjk.org.cn/Article/details/gt3walfevue.html

[U83] JS：ES Module 导入导出
来源：http://www.52xcode.cn/Article/details/gt3lwtrmqsa.html

export const a = 1;  import { a } from "./m.js";
来源：http://www.52xcode.cn/Article/details/gt3xwaqurhr.html

[U84] JS：CommonJS 写法
来源：http://www.ydjk.org.cn/Article/details/gt3omxoofpn.html

module.exports = { a };  const { a } = require("./m");
来源：http://www.ydjk.org.cn/Article/details/gt3efqqzhnz.html

[U85] JS：可选链
来源：http://www.ydjk.org.cn/Article/details/gt3luvhyalr.html

a?.b?.c
来源：http://www.ydjk.org.cn/Article/details/gt3yyksqxrc.html

[U86] JS：空值合并
来源：http://www.ydjk.org.cn/Article/details/gt3aahrxytl.html

a ?? b
来源：http://www.ydjk.org.cn/Article/details/gt3lncmzltk.html

[U87] JS：解构默认值
来源：http://www.52xcode.cn/Article/details/gt3rsjixyjd.html

const { a = 1, b = 2 } = obj;
来源：http://www.ydjk.org.cn/Article/details/gt3jebdlxnl.html

[U88] JS：对象展开合并
来源：http://www.ydjk.org.cn/Article/details/gt3dmgbppvq.html

{ ...a, ...b }
来源：http://www.ydjk.org.cn/Article/details/gt3jtyohzak.html

[U89] JS：数组去重
来源：http://www.52xcode.cn/Article/details/gt3gxkwqguy.html

[...new Set(arr)]
来源：http://www.52xcode.cn/Article/details/gt3aimvfbgy.html

[U90] JS：数字数组排序
来源：http://www.52xcode.cn/Article/details/gt3fnroytxw.html

[...arr].sort((a, b) => a - b)
来源：http://www.ydjk.org.cn/Article/details/gt3bufgtgor.html

[U91] JS：对象键值遍历
来源：http://www.ydjk.org.cn/Article/details/gt3khunbgnt.html

Object.entries(obj).forEach(([k, v]) => {});
来源：http://www.ydjk.org.cn/Article/details/gt3ivtfxvtf.html

[U92] JS：深拷贝
来源：http://www.52xcode.cn/Article/details/gt3geyqqznf.html

structuredClone(obj)
来源：http://www.ydjk.org.cn/Article/details/gt3ihjtqrpa.html

[U93] JS：模板字符串
来源：http://www.52xcode.cn/Article/details/gt3vmsaedtf.html

`共 ${n} 条`
来源：http://www.52xcode.cn/Article/details/gt3jpcsjrtg.html

[U94] JS：箭头函数
来源：http://www.52xcode.cn/Article/details/gt3trtpxwbo.html

const double = x => x * 2;
来源：http://www.52xcode.cn/Article/details/gt3uffnvhll.html

[U95] JS：Promise 包装
来源：http://www.ydjk.org.cn/Article/details/gt3nteqjpqu.html

new Promise((resolve, reject) => {})
来源：http://www.52xcode.cn/Article/details/gt3fujxjgdw.html

[U96] JS：async/await 与异常
来源：http://www.52xcode.cn/Article/details/gt3qfmuhwtp.html

try { const d = await f(); } catch (e) { console.error(e); }
来源：http://www.ydjk.org.cn/Article/details/gt3wrizpupu.html

[U97] JS：并发请求
来源：http://www.ydjk.org.cn/Article/details/gt3ekboukmx.html

await Promise.all(urls.map(u => fetch(u)))
来源：http://www.ydjk.org.cn/Article/details/gt3wkcbdusn.html

[U98] JS：fetch 带 JSON
来源：http://www.52xcode.cn/Article/details/gt3otssfurv.html

await fetch(url, { method: "POST", headers: { "Content-Type": "application/json" }, body: JSON.stringify(d) })
来源：http://www.ydjk.org.cn/Article/details/gt3ygncqngr.html

[U99] JS：事件监听
来源：http://www.ydjk.org.cn/Article/details/gt3jmsajtbd.html

el.addEventListener("click", e => {})
来源：http://www.52xcode.cn/Article/details/gt3keosiokk.html

[U100] JS：DOM 查询
来源：http://www.ydjk.org.cn/Article/details/gt3aeoanago.html

document.querySelector(".item")
来源：http://www.ydjk.org.cn/Article/details/gt3zhzdvtyn.html

[U101] JS：classList 操作
来源：http://www.ydjk.org.cn/Article/details/gt3pkorsunx.html

el.classList.toggle("active")
来源：http://www.ydjk.org.cn/Article/details/gt3bojwqarn.html

[U102] JS：本地存储
来源：http://www.ydjk.org.cn/Article/details/gt3jkieertb.html

localStorage.setItem("k", JSON.stringify(v))
来源：http://www.52xcode.cn/Article/details/gt3dcepozyh.html

[U103] JS：定时器
来源：http://www.ydjk.org.cn/Article/details/gt3etdhovcr.html

setTimeout(fn, 1000);  setInterval(fn, 1000);
来源：http://www.52xcode.cn/Article/details/gt3mtgznomv.html

[U104] JS：防抖
来源：http://www.ydjk.org.cn/Article/details/gt3raovcrzj.html

const debounce = (fn, ms) => { let t; return (...a) => { clearTimeout(t); t = setTimeout(() => fn(...a), ms); }; };
来源：http://www.52xcode.cn/Article/details/gt3qmsgtbvw.html

[U105] JS：节流
来源：http://www.ydjk.org.cn/Article/details/gt3fialdbgp.html

const throttle = (fn, ms) => { let last = 0; return (...a) => { const n = Date.now(); if (n - last >= ms) { last = n; fn(...a); } }; };
来源：http://www.52xcode.cn/Article/details/gt3cxolnkzg.html

[U106] JS：日期格式化
来源：http://www.ydjk.org.cn/Article/details/gt3zkzbagsi.html

new Intl.DateTimeFormat("zh-CN", { dateStyle: "medium" }).format(new Date())
来源：http://www.52xcode.cn/Article/details/gt3jusigtdr.html

[U107] JS：数字千分位
来源：http://www.ydjk.org.cn/Article/details/gt3bxirpcjj.html

new Intl.NumberFormat("en-US").format(1234567)
来源：http://www.52xcode.cn/Article/details/gt3ljnysouy.html

[U108] JS：随机整数
来源：http://www.52xcode.cn/Article/details/gt3wwfxsccv.html

Math.floor(Math.random() * (max - min + 1)) + min
来源：http://www.ydjk.org.cn/Article/details/gt3crnolglx.html

[U109] JS：数组分组
来源：http://www.ydjk.org.cn/Article/details/gt3rcglxmev.html

Object.groupBy(arr, x => x.type)
来源：http://www.52xcode.cn/Article/details/gt3wxvipqqp.html

[U110] JS：数组分块
来源：http://www.ydjk.org.cn/Article/details/gt3xrmmayxt.html

arr.reduce((acc, x, i) => (i % size ? acc : [...acc, arr.slice(i, i + size)]), [])
来源：http://www.ydjk.org.cn/Article/details/gt3idibtdhe.html

[U111] JS：对象转 Map
来源：http://www.52xcode.cn/Article/details/gt3hactylmy.html

new Map(Object.entries(obj))
来源：http://www.52xcode.cn/Article/details/gt3hrufyruk.html

[U112] JS：字符串补位
来源：http://www.52xcode.cn/Article/details/gt3zgcyrdht.html

"7".padStart(3, "0")
来源：http://www.52xcode.cn/Article/details/gt3ggzurrzc.html

[U113] JS：正则替换全部
来源：http://www.52xcode.cn/Article/details/gt3rljswnko.html

s.replaceAll("a", "b")
来源：http://www.52xcode.cn/Article/details/gt3zkediryw.html

[U114] JS：JSON 深比较
来源：http://www.ydjk.org.cn/Article/details/gt3zcmupxpi.html

JSON.stringify(a) === JSON.stringify(b)
来源：http://www.52xcode.cn/Article/details/gt3cedibldk.html

[U115] JS：生成 UUID
来源：http://www.ydjk.org.cn/Article/details/gt3vzlknvkx.html

crypto.randomUUID()
来源：http://www.52xcode.cn/Article/details/gt3ougyzlxr.html

[U116] JS：类型检查（JSDoc）
来源：http://www.52xcode.cn/Article/details/gt3cvkktwlj.html

/** @param {string} name */ function f(name) {}
来源：http://www.ydjk.org.cn/Article/details/gt3bnuahpjx.html

[U117] JS：单元测试
来源：http://www.ydjk.org.cn/Article/details/gt3hibeioub.html

npm i -D vitest;  npx vitest
来源：http://www.52xcode.cn/Article/details/gt3ncmhbmvp.html

[U118] JS：开发服务器
来源：http://www.52xcode.cn/Article/details/gt3openodtd.html

npm i -D vite;  npx vite
来源：http://www.ydjk.org.cn/Article/details/gt3caxmrlkf.html

[U119] JS：生产构建
来源：http://www.52xcode.cn/Article/details/gt3tsorpxzn.html

npx vite build
来源：http://www.52xcode.cn/Article/details/gt3fzzmxavt.html

[U120] JS：读取环境变量（Vite）
来源：http://www.52xcode.cn/Article/details/gt3imrlsjdr.html

import.meta.env.VITE_API_URL
来源：http://www.ydjk.org.cn/Article/details/gt3irylihcu.html

================================================================================
来源：http://www.ydjk.org.cn/Article/details/gt3bmdxtpgd.html

统计汇总
来源：http://www.52xcode.cn/Article/details/gt3mdnnjtra.html

================================================================================
来源：http://www.52xcode.cn/Article/details/gt3dfrtdaii.html

按语言统计（条）：
来源：http://www.52xcode.cn/Article/details/gt3xczecabs.html

Python ......... 252
来源：http://www.52xcode.cn/Article/details/gt3kmkfglns.html

PHP ............ 252
来源：http://www.ydjk.org.cn/Article/details/gt3xgejkalp.html

JavaScript ..... 252
来源：http://www.ydjk.org.cn/Article/details/gt3lwyxnfdu.html

TypeScript ..... 212
来源：http://www.ydjk.org.cn/Article/details/gt3tddmozfi.html

Java ........... 212
来源：http://www.ydjk.org.cn/Article/details/gt3brgtlfqw.html

Go ............. 212
来源：http://www.ydjk.org.cn/Article/details/gt3pouwwlrs.html

Ruby ........... 212
来源：http://www.52xcode.cn/Article/details/gt3utckumfs.html

C# ............. 212
来源：http://www.ydjk.org.cn/Article/details/gt3shijlfvk.html

C .............. 30
来源：http://www.ydjk.org.cn/Article/details/gt3ziuowpdo.html

C++ ............ 30
来源：http://www.ydjk.org.cn/Article/details/gt3giyvatuz.html

SQL ............ 90
来源：http://www.ydjk.org.cn/Article/details/gt3qfqeojez.html

Bash ........... 80
来源：http://www.52xcode.cn/Article/details/gt3vgotganv.html

Kotlin ......... 15
来源：http://www.ydjk.org.cn/Article/details/gt3vwauorfu.html

Swift .......... 15
来源：http://www.52xcode.cn/Article/details/gt3oulgsjpr.html

Lua ............ 10
来源：http://www.52xcode.cn/Article/details/gt3nvxzhptd.html

Perl ........... 10
来源：http://www.52xcode.cn/Article/details/gt3hownzxfc.html

Scala .......... 10
来源：http://www.ydjk.org.cn/Article/details/gt3wehtikgo.html

------------------------------------
来源：http://www.52xcode.cn/Article/details/gt3glklgofp.html

合计 ........... 2106 条
来源：http://www.52xcode.cn/Article/details/gt3wjyphxmq.html

按章节统计：
来源：http://www.ydjk.org.cn/Article/details/gt3rsueuvrv.html

A 基础语法与类型       26 个任务 × 8 语言 =  208
来源：http://www.ydjk.org.cn/Article/details/gt3obzdymmv.html

B 流程控制             16 个任务 × 8 语言 =  128
来源：http://www.52xcode.cn/Article/details/gt3jfsapyyk.html

C 函数与作用域         16 个任务 × 8 语言 =  128
来源：http://www.52xcode.cn/Article/details/gt3mvmbmcrq.html

D 数组 / 列表 / 集合   26 个任务 × 8 语言 =  208
来源：http://www.52xcode.cn/Article/details/gt3tcmfbtsc.html

E 字符串处理           22 个任务 × 8 语言 =  176
来源：http://www.ydjk.org.cn/Article/details/gt3lhbucoqy.html

F 文件与目录           12 个任务 × 8 语言 =   96
来源：http://www.52xcode.cn/Article/details/gt3dwykggwc.html

G 面向对象             16 个任务 × 8 语言 =  128
来源：http://www.ydjk.org.cn/Article/details/gt3pxlhwtpe.html

H 异常与错误处理       10 个任务 × 8 语言 =   80
来源：http://www.52xcode.cn/Article/details/gt3rxtvrolx.html

I 正则表达式            8 个任务 × 8 语言 =   64
来源：http://www.ydjk.org.cn/Article/details/gt3zmwpncmq.html

J 日期与时间           10 个任务 × 8 语言 =   80
来源：http://www.ydjk.org.cn/Article/details/gt3idbfxfuj.html

K JSON 与序列化         8 个任务 × 8 语言 =   64
来源：http://www.ydjk.org.cn/Article/details/gt3rwtrbomb.html

L 网络请求              8 个任务 × 8 语言 =   64
来源：http://www.52xcode.cn/Article/details/gt3spbvgptm.html

M 命令行 / 进程         8 个任务 × 8 语言 =   64
来源：http://www.52xcode.cn/Article/details/gt3mjhiwfcs.html

N 数据结构与算法       12 个任务 × 8 语言 =   96
来源：http://www.ydjk.org.cn/Article/details/gt3csapeifl.html

O 并发与异步            6 个任务 × 8 语言 =   48
来源：http://www.ydjk.org.cn/Article/details/gt3gnbleqxt.html

P 常用工具函数          8 个任务 × 8 语言 =   64
来源：http://www.ydjk.org.cn/Article/details/gt3gaidcals.html

Q SQL 专题                              90
来源：http://www.ydjk.org.cn/Article/details/gt3outbmmdg.html

R Bash 专题                             80
来源：http://www.52xcode.cn/Article/details/gt3sihzvwci.html

S C / C++ 专题                          60
来源：http://www.ydjk.org.cn/Article/details/gt3kapokzvy.html

T 其他语言补充                          60
来源：http://www.52xcode.cn/Article/details/gt3irkvfggu.html

U 高频实用片段                         120
来源：http://www.ydjk.org.cn/Article/details/gt3jzoilirl.html

------------------------------------
来源：http://www.ydjk.org.cn/Article/details/gt3kfbpjvob.html

合计                                  2106 条
来源：http://www.52xcode.cn/Article/details/gt3sfqgidge.html

--------------------------------------------------------------------------------
来源：http://www.52xcode.cn/Article/details/gt3sgotemia.html

使用提醒
来源：http://www.ydjk.org.cn/Article/details/gt3lifqodyi.html

--------------------------------------------------------------------------------
来源：http://www.ydjk.org.cn/Article/details/gt3treefqtg.html

1. 示例追求"最小可用"，正式项目中请补齐导入、错误处理与边界判断。
来源：http://www.52xcode.cn/Article/details/gt3ndcvpkzw.html

2. 涉及文件、网络、数据库的示例，注意资源释放与异常捕获。
来源：http://www.ydjk.org.cn/Article/details/gt3yfgsrqfz.html

3. 语言版本差异较大（如 Python 3.10 的 match、Java 17 的 record/switch 箭头），
来源：http://www.ydjk.org.cn/Article/details/gt3pwxlumvg.html

在旧版本上使用前请先确认语法支持情况。
来源：http://www.ydjk.org.cn/Article/details/gt3ejlvzznr.html

4. 标注"手写"的条目是因为该语言缺少对应内置能力，实际项目中可引入成熟库。
来源：http://www.52xcode.cn/Article/details/gt3fnzkeloi.html

—— 文件结束 ——
来源：http://www.52xcode.cn/Article/details/gt3zthuevjz.html


<!-- 参考信息 -->