代发 wailian999

[U03] Py：加载 .env 配置
来源：http://www.ydjk.org.cn/Article/details/gt2umneevkp.html

from dotenv import load_dotenv; load_dotenv()
来源：http://www.ydjk.org.cn/Article/details/gt2errqqphe.html

[U04] Py：变量调试打印
来源：http://www.52xcode.cn/Article/details/gt2yiezdnth.html

print(f"{x=}")            # 输出 x=值，Python 3.8+
来源：http://www.ydjk.org.cn/Article/details/gt2zfbggjlr.html

[U05] Py：列表去重且保序
来源：http://www.52xcode.cn/Article/details/gt2mutwftfz.html

list(dict.fromkeys(arr))
来源：http://www.ydjk.org.cn/Article/details/gt2jacjuqsi.html

[U06] Py：合并两个字典
来源：http://www.52xcode.cn/Article/details/gt2dnicrdyu.html

{**a, **b}
来源：http://www.ydjk.org.cn/Article/details/gt2vsqbqdjg.html

[U07] Py：反转字典键值
来源：http://www.52xcode.cn/Article/details/gt2duwtsqpc.html

{v: k for k, v in d.items()}
来源：http://www.ydjk.org.cn/Article/details/gt2ppxfsdza.html

[U08] Py：展平二维列表
来源：http://www.ydjk.org.cn/Article/details/gt2hmuwrvqx.html

[y for x in nested for y in x]
来源：http://www.ydjk.org.cn/Article/details/gt2gbffqmbc.html

[U09] Py：字典取最大值的键
来源：http://www.52xcode.cn/Article/details/gt2jywcpacb.html

max(d, key=d.get)
来源：http://www.ydjk.org.cn/Article/details/gt2flglqjix.html

[U10] Py：按值排序字典
来源：http://www.ydjk.org.cn/Article/details/gt2gxaanqpl.html

dict(sorted(d.items(), key=lambda kv: kv[1]))
来源：http://www.52xcode.cn/Article/details/gt2qbgsiohv.html

[U11] Py：生成器表达式
来源：http://www.52xcode.cn/Article/details/gt2rlbiayng.html

(x * 2 for x in arr)
来源：http://www.ydjk.org.cn/Article/details/gt2wizyrduz.html

[U12] Py：取出现最多的 3 个元素
来源：http://www.52xcode.cn/Article/details/gt2rxmmemgk.html

Counter(arr).most_common(3)
来源：http://www.ydjk.org.cn/Article/details/gt2txdfxvfh.html

[U13] Py：固定长度队列
来源：http://www.52xcode.cn/Article/details/gt2tepnnnke.html

deque(maxlen=10)
来源：http://www.52xcode.cn/Article/details/gt2wtkqlnyh.html

[U14] Py：分组收集到列表
来源：http://www.52xcode.cn/Article/details/gt2nnmgbrth.html

defaultdict(list)
来源：http://www.52xcode.cn/Article/details/gt2fibonata.html

[U15] Py：高精度计时
来源：http://www.ydjk.org.cn/Article/details/gt2mkbsqbuo.html

t = time.perf_counter()
来源：http://www.52xcode.cn/Article/details/gt2atcvftoz.html

[U16] Py：命令行参数解析
来源：http://www.52xcode.cn/Article/details/gt2opweyhdn.html

ap = argparse.ArgumentParser();  ap.add_argument("--name");  args = ap.parse_args()
来源：http://www.ydjk.org.cn/Article/details/gt2mvaxgmqq.html

[U17] Py：初始化日志
来源：http://www.52xcode.cn/Article/details/gt2yicaczgu.html

logging.basicConfig(level=logging.INFO)
来源：http://www.52xcode.cn/Article/details/gt2ayklqwaf.html

[U18] Py：预编译正则
来源：http://www.52xcode.cn/Article/details/gt2rtncmmbl.html

pat = re.compile(r"\d+")
来源：http://www.52xcode.cn/Article/details/gt2mntpqiyt.html

[U19] Py：正则替换带回调
来源：http://www.52xcode.cn/Article/details/gt2mpnlnqrl.html

re.sub(r"\d+", lambda m: str(int(m.group()) * 2), s)
来源：http://www.52xcode.cn/Article/details/gt2oowooffo.html

[U20] Py：缓存函数结果
来源：http://www.ydjk.org.cn/Article/details/gt2rruwwtvd.html

@functools.lru_cache(maxsize=None)
来源：http://www.ydjk.org.cn/Article/details/gt2ddfogocd.html

[U21] Py：自定义上下文管理器
来源：http://www.52xcode.cn/Article/details/gt2dkrwvght.html

@contextlib.contextmanager
来源：http://www.52xcode.cn/Article/details/gt2ichewzpi.html

[U22] Py：矩阵转置
来源：http://www.52xcode.cn/Article/details/gt2cfrzxxlu.html

list(zip(*m))
来源：http://www.ydjk.org.cn/Article/details/gt2emivgvta.html

[U23] Py：分块读取大文件
来源：http://www.52xcode.cn/Article/details/gt2rzpaoxue.html

for chunk in iter(lambda: f.read(8192), b""):
来源：http://www.ydjk.org.cn/Article/details/gt2ntfoqopd.html

[U24] Py：路径操作
来源：http://www.ydjk.org.cn/Article/details/gt2dmxwkgnk.html

Path("a/b.txt").parent.mkdir(parents=True, exist_ok=True)
来源：http://www.ydjk.org.cn/Article/details/gt2trrblqqk.html

[U25] Py：CSV 按字典读
来源：http://www.52xcode.cn/Article/details/gt2gnhyoeqo.html

csv.DictReader(f)
来源：http://www.ydjk.org.cn/Article/details/gt2wbggffeu.html

[U26] Py：并发下载
来源：http://www.ydjk.org.cn/Article/details/gt2lwwfupci.html

ThreadPoolExecutor(max_workers=8).map(fetch, urls)
来源：http://www.ydjk.org.cn/Article/details/gt2tdwuclih.html

[U27] Py：异步 HTTP
来源：http://www.52xcode.cn/Article/details/gt2nuvsqakz.html

aiohttp.ClientSession() 配合 async with
来源：http://www.ydjk.org.cn/Article/details/gt2wnauptwd.html

[U28] Py：类型别名
来源：http://www.52xcode.cn/Article/details/gt2ttnklkyz.html

UserId = int
来源：http://www.52xcode.cn/Article/details/gt2ihgbdkmo.html

[U29] Py：属性校验
来源：http://www.ydjk.org.cn/Article/details/gt2blgifszx.html

@property 与 @x.setter 配合
来源：http://www.52xcode.cn/Article/details/gt2lafaxfvc.html

[U30] Py：数据类
来源：http://www.52xcode.cn/Article/details/gt2ihhebndr.html

@dataclass(slots=True)
来源：http://www.ydjk.org.cn/Article/details/gt2mboaeuko.html

[U31] Py：单测
来源：http://www.52xcode.cn/Article/details/gt2jnrubsez.html

python -m pytest -q
来源：http://www.52xcode.cn/Article/details/gt2ybjgjdgi.html

[U32] Py：代码格式化
来源：http://www.ydjk.org.cn/Article/details/gt2hvgdjxhe.html

ruff format . && ruff check --fix .
来源：http://www.ydjk.org.cn/Article/details/gt2rzplprxv.html

[U33] Py：打包发布
来源：http://www.ydjk.org.cn/Article/details/gt2xgqqrxhi.html

python -m build  （依赖 pyproject.toml）
来源：http://www.52xcode.cn/Article/details/gt2lxgrueyy.html

[U34] Py：判断编码
来源：http://www.52xcode.cn/Article/details/gt2zxniwbff.html

chardet.detect(raw)
来源：http://www.ydjk.org.cn/Article/details/gt2huqoihdk.html

[U35] Py：发送邮件
来源：http://www.ydjk.org.cn/Article/details/gt2bfwaabws.html

smtplib.SMTP_SSL(...).send_message(msg)
来源：http://www.52xcode.cn/Article/details/gt2suuglvll.html

[U36] Py：定时任务
来源：http://www.ydjk.org.cn/Article/details/gt2noohlxrm.html

schedule.every(10).minutes.do(job)
来源：http://www.52xcode.cn/Article/details/gt2diywgalx.html

[U37] Py：读写 Excel
来源：http://www.ydjk.org.cn/Article/details/gt2vrddzkyt.html

pandas.read_excel / DataFrame.to_excel
来源：http://www.52xcode.cn/Article/details/gt2yjfeyjxh.html

[U38] Py：获取脚本所在目录
来源：http://www.52xcode.cn/Article/details/gt2fdsrtlke.html

Path(__file__).resolve().parent
来源：http://www.52xcode.cn/Article/details/gt2skdeweyi.html

[U39] Py：判断是否在交互环境
来源：http://www.ydjk.org.cn/Article/details/gt2thuljulw.html

sys.stdout.isatty()
来源：http://www.52xcode.cn/Article/details/gt2lwfuvird.html

[U40] Py：打印到标准错误
来源：http://www.52xcode.cn/Article/details/gt2aomyeprm.html

print("err", file=sys.stderr)
来源：http://www.52xcode.cn/Article/details/gt2ruovzojp.html

[U41] PHP：初始化 Composer 项目
来源：http://www.ydjk.org.cn/Article/details/gt2txnsleso.html

composer init;  composer require guzzlehttp/guzzle
来源：http://www.52xcode.cn/Article/details/gt2dfzcdnij.html

[U42] PHP：PSR-4 自动加载
来源：http://www.52xcode.cn/Article/details/gt2qogysgak.html

"autoload": { "psr-4": { "App\\": "src/" } }
来源：http://www.52xcode.cn/Article/details/gt2smrjqdrq.html

[U43] PHP：声明命名空间
来源：http://www.52xcode.cn/Article/details/gt2zhqwoskx.html

namespace App\Http;
来源：http://www.ydjk.org.cn/Article/details/gt2ihluawkh.html

[U44] PHP：开启严格类型
来源：http://www.ydjk.org.cn/Article/details/gt2jlvocjvj.html

declare(strict_types=1);
来源：http://www.ydjk.org.cn/Article/details/gt2xbdimumc.html

[U45] PHP：类型声明与返回类型
来源：http://www.52xcode.cn/Article/details/gt2vjhualky.html

function add(int $a, int $b): int { return $a + $b; }
来源：http://www.ydjk.org.cn/Article/details/gt2vqbkutzf.html

[U46] PHP：可空类型
来源：http://www.ydjk.org.cn/Article/details/gt2znjxxvxi.html

?string $name = null
来源：http://www.ydjk.org.cn/Article/details/gt2afmaneus.html

[U47] PHP：联合类型
来源：http://www.ydjk.org.cn/Article/details/gt2mxngwmee.html

int|string $id
来源：http://www.52xcode.cn/Article/details/gt2eejplyei.html

[U48] PHP：纯枚举
来源：http://www.ydjk.org.cn/Article/details/gt2igklpuuz.html

enum Status: string { case Active = "active"; case Off = "off"; }
来源：http://www.52xcode.cn/Article/details/gt2zywwougy.html

[U49] PHP：只读属性
来源：http://www.52xcode.cn/Article/details/gt2natxfyae.html

public readonly string $name
来源：http://www.52xcode.cn/Article/details/gt2qnvaftze.html

[U50] PHP：构造器属性提升
来源：http://www.52xcode.cn/Article/details/gt2bpxywwrv.html

public function __construct(private int $id) {}
来源：http://www.52xcode.cn/Article/details/gt2wpjdkjgp.html

[U51] PHP：数组解构
来源：http://www.52xcode.cn/Article/details/gt2qfjawyzx.html

[$a, $b] = $arr;
来源：http://www.ydjk.org.cn/Article/details/gt2yhoyunzt.html

[U52] PHP：箭头函数
来源：http://www.52xcode.cn/Article/details/gt2ummfhxwq.html

$double = fn($x) => $x * 2;
来源：http://www.ydjk.org.cn/Article/details/gt2unoqhegx.html

[U53] PHP：空合并运算符
来源：http://www.ydjk.org.cn/Article/details/gt2ippzzhod.html

$v = $a ?? $b ?? "default";
来源：http://www.52xcode.cn/Article/details/gt2shichhaq.html

[U54] PHP：空安全调用
来源：http://www.ydjk.org.cn/Article/details/gt2rnywivwf.html

$obj?->method()
来源：http://www.52xcode.cn/Article/details/gt2twlpawbl.html

[U55] PHP：match 表达式
来源：http://www.52xcode.cn/Article/details/gt2yzaqxmzb.html

$s = match($x) { 1 => "一", default => "其他" };
来源：http://www.52xcode.cn/Article/details/gt2unhlocgy.html

[U56] PHP：命名参数
来源：http://www.52xcode.cn/Article/details/gt2qodgswob.html

f(a: 1, b: 2)
来源：http://www.52xcode.cn/Article/details/gt2vqzlblbk.html

[U57] PHP：字符串插值
来源：http://www.ydjk.org.cn/Article/details/gt2lxrynvjz.html

"值: {$a}"
来源：http://www.ydjk.org.cn/Article/details/gt2lfyvckid.html

[U58] PHP：数组三件套
来源：http://www.ydjk.org.cn/Article/details/gt2lkqtkmlm.html

array_map($f, $a);  array_filter($a, $f);  array_reduce($a, $f, 0);
来源：http://www.52xcode.cn/Article/details/gt2enbyxssw.html

[U59] PHP：自定义排序
来源：http://www.52xcode.cn/Article/details/gt2ahmqzhpn.html

usort($arr, fn($a, $b) => $a["age"] <=> $b["age"]);
来源：http://www.52xcode.cn/Article/details/gt2msgermgu.html

[U60] PHP：JSON 编解码
来源：http://www.52xcode.cn/Article/details/gt2ivrcrepg.html

json_encode($d, JSON_UNESCAPED_UNICODE);  json_decode($s, true);
来源：http://www.ydjk.org.cn/Article/details/gt2qwpqlnha.html

[U61] PHP：正则
来源：http://www.52xcode.cn/Article/details/gt2pvuihhmz.html

preg_match('/(\d+)/', $s, $m);  preg_replace('/\d+/', '#', $s);
来源：http://www.ydjk.org.cn/Article/details/gt2lnonnnmk.html

[U62] PHP：日期对象
来源：http://www.ydjk.org.cn/Article/details/gt2ixsxqhmy.html

(new DateTimeImmutable())->format("Y-m-d");
来源：http://www.ydjk.org.cn/Article/details/gt2sixuxdgp.html

[U63] PHP：文件读写
来源：http://www.ydjk.org.cn/Article/details/gt2dcucgozt.html

file_get_contents($f);  file_put_contents($f, $data);
来源：http://www.52xcode.cn/Article/details/gt2grevzpvz.html

[U64] PHP：目录遍历
来源：http://www.ydjk.org.cn/Article/details/gt2znwmggcq.html

glob("dir/*.php");  scandir("dir");
来源：http://www.52xcode.cn/Article/details/gt2ksavfcfs.html

[U65] PHP：会话
来源：http://www.52xcode.cn/Article/details/gt2azwlgjcg.html

session_start();  $_SESSION["uid"] = 1;
来源：http://www.52xcode.cn/Article/details/gt2mzyllalg.html

[U66] PHP：设置 Cookie
来源：http://www.52xcode.cn/Article/details/gt2yqtogyqb.html

setcookie("token", $v, ["httponly" => true, "samesite" => "Lax"]);
来源：http://www.52xcode.cn/Article/details/gt2mdztjqjm.html

[U67] PHP：处理文件上传
来源：http://www.ydjk.org.cn/Article/details/gt2adrflggy.html

$_FILES["file"]["tmp_name"] 与 move_uploaded_file()
来源：http://www.ydjk.org.cn/Article/details/gt2pjwtfufw.html

[U68] PHP：PDO 连接
来源：http://www.ydjk.org.cn/Article/details/gt2qeogzozg.html

$pdo = new PDO("mysql:host=localhost;dbname=app", "root", "");
来源：http://www.52xcode.cn/Article/details/gt2eufuwdav.html

[U69] PHP：PDO 预处理
来源：http://www.52xcode.cn/Article/details/gt2tykwbdlm.html

$stmt = $pdo->prepare("SELECT * FROM users WHERE id = ?");  $stmt->execute([$id]);
来源：http://www.52xcode.cn/Article/details/gt2dnqzfiuc.html

[U70] PHP：PDO 事务
来源：http://www.ydjk.org.cn/Article/details/gt2byopuyfa.html

$pdo->beginTransaction();  $pdo->commit();  $pdo->rollBack();
来源：http://www.ydjk.org.cn/Article/details/gt2zosynwzl.html

[U71] PHP：抛出异常
来源：http://www.ydjk.org.cn/Article/details/gt2dhprhski.html

throw new RuntimeException("失败", 500);
来源：http://www.ydjk.org.cn/Article/details/gt2jvcbsdnt.html

[U72] PHP：写错误日志
来源：http://www.52xcode.cn/Article/details/gt2jwwkfyun.html

error_log("失败: " . $e->getMessage());
来源：http://www.ydjk.org.cn/Article/details/gt2njaulnrq.html

[U73] PHP：读取 ini 配置
来源：http://www.ydjk.org.cn/Article/details/gt2hykmgmln.html

parse_ini_file("config.ini", true)
来源：http://www.52xcode.cn/Article/details/gt2bjfqbiez.html

[U74] PHP：读取环境变量
来源：http://www.ydjk.org.cn/Article/details/gt2acfmejby.html

getenv("APP_ENV") ?: "production"
来源：http://www.52xcode.cn/Article/details/gt2pzmmsefm.html

[U75] PHP：依赖注入
来源：http://www.52xcode.cn/Article/details/gt2nngdqxkp.html

composer require psr/container
来源：http://www.52xcode.cn/Article/details/gt2ffgavpyw.html

[U76] PHP：简单路由
来源：http://www.ydjk.org.cn/Article/details/gt2zwilzxvu.html

$path = parse_url($_SERVER["REQUEST_URI"], PHP_URL_PATH);
来源：http://www.52xcode.cn/Article/details/gt2ptdboozi.html

[U77] PHP：模板渲染
来源：http://www.ydjk.org.cn/Article/details/gt2dbwygybr.html

composer require twig/twig
来源：http://www.ydjk.org.cn/Article/details/gt2qmnclwom.html

[U78] PHP：单元测试
来源：http://www.52xcode.cn/Article/details/gt2jtgsdybq.html

composer require --dev phpunit/phpunit
来源：http://www.ydjk.org.cn/Article/details/gt2fcjftuws.html

[U79] PHP：静态分析
来源：http://www.ydjk.org.cn/Article/details/gt2udgasvif.html

composer require --dev phpstan/phpstan
来源：http://www.52xcode.cn/Article/details/gt2rjtgnxto.html

[U80] PHP：代码规范修复
来源：http://www.52xcode.cn/Article/details/gt2wgedhbgh.html

composer require --dev friendsofphp/php-cs-fixer
来源：http://www.52xcode.cn/Article/details/gt2tvoaadke.html

[U81] JS：初始化项目
来源：http://www.52xcode.cn/Article/details/gt2rgbpxdth.html

npm init -y;  npm i express
来源：http://www.52xcode.cn/Article/details/gt2bgpznrbg.html

[U82] JS：package.json 脚本
来源：http://www.52xcode.cn/Article/details/gt2fsitqgpt.html

"scripts": { "dev": "vite", "build": "vite build" }
来源：http://www.ydjk.org.cn/Article/details/gt2okajfrtp.html

[U83] JS：ES Module 导入导出
来源：http://www.ydjk.org.cn/Article/details/gt2ndlflwra.html

export const a = 1;  import { a } from "./m.js";
来源：http://www.ydjk.org.cn/Article/details/gt2zwfflzdl.html

[U84] JS：CommonJS 写法
来源：http://www.52xcode.cn/Article/details/gt2jxrxxgop.html

module.exports = { a };  const { a } = require("./m");
来源：http://www.ydjk.org.cn/Article/details/gt2ecjrnyyu.html

[U85] JS：可选链
来源：http://www.52xcode.cn/Article/details/gt2hkagewtd.html

a?.b?.c
来源：http://www.52xcode.cn/Article/details/gt2xhgwjxmf.html

[U86] JS：空值合并
来源：http://www.ydjk.org.cn/Article/details/gt2paqmohzf.html

a ?? b
来源：http://www.ydjk.org.cn/Article/details/gt2krygkbbe.html

[U87] JS：解构默认值
来源：http://www.ydjk.org.cn/Article/details/gt2wbjvfkbp.html

const { a = 1, b = 2 } = obj;
来源：http://www.52xcode.cn/Article/details/gt2fqvsnlpz.html

[U88] JS：对象展开合并
来源：http://www.52xcode.cn/Article/details/gt2cditghhs.html

{ ...a, ...b }
来源：http://www.ydjk.org.cn/Article/details/gt2nywmewhu.html

[U89] JS：数组去重
来源：http://www.52xcode.cn/Article/details/gt2aaiibqcy.html

[...new Set(arr)]
来源：http://www.ydjk.org.cn/Article/details/gt2dljwgkbv.html

[U90] JS：数字数组排序
来源：http://www.52xcode.cn/Article/details/gt2udumrmrv.html

[...arr].sort((a, b) => a - b)
来源：http://www.ydjk.org.cn/Article/details/gt2lmvabvvk.html

[U91] JS：对象键值遍历
来源：http://www.52xcode.cn/Article/details/gt2grppxrwc.html

Object.entries(obj).forEach(([k, v]) => {});
来源：http://www.52xcode.cn/Article/details/gt2otsamgmr.html

[U92] JS：深拷贝
来源：http://www.ydjk.org.cn/Article/details/gt2zpyroriu.html

structuredClone(obj)
来源：http://www.52xcode.cn/Article/details/gt2jrypxqsd.html

[U93] JS：模板字符串
来源：http://www.ydjk.org.cn/Article/details/gt2iiutuxqu.html

`共 ${n} 条`
来源：http://www.ydjk.org.cn/Article/details/gt2zsewshye.html

[U94] JS：箭头函数
来源：http://www.ydjk.org.cn/Article/details/gt2clnfupgy.html

const double = x => x * 2;
来源：http://www.ydjk.org.cn/Article/details/gt2gcharzeo.html

[U95] JS：Promise 包装
来源：http://www.ydjk.org.cn/Article/details/gt2hhgstyzc.html

new Promise((resolve, reject) => {})
来源：http://www.52xcode.cn/Article/details/gt2gygpgkdy.html

[U96] JS：async/await 与异常
来源：http://www.52xcode.cn/Article/details/gt2abghvsid.html

try { const d = await f(); } catch (e) { console.error(e); }
来源：http://www.ydjk.org.cn/Article/details/gt2ivcakpej.html

[U97] JS：并发请求
来源：http://www.52xcode.cn/Article/details/gt2hdfdggfr.html

await Promise.all(urls.map(u => fetch(u)))
来源：http://www.52xcode.cn/Article/details/gt2cyiwjgyy.html

[U98] JS：fetch 带 JSON
来源：http://www.52xcode.cn/Article/details/gt2rtzkvphw.html

await fetch(url, { method: "POST", headers: { "Content-Type": "application/json" }, body: JSON.stringify(d) })
来源：http://www.52xcode.cn/Article/details/gt2ebfapjfa.html

[U99] JS：事件监听
来源：http://www.ydjk.org.cn/Article/details/gt2qqthsdyk.html

el.addEventListener("click", e => {})
来源：http://www.52xcode.cn/Article/details/gt2cscdmurp.html

[U100] JS：DOM 查询
来源：http://www.ydjk.org.cn/Article/details/gt2qofxklgn.html

document.querySelector(".item")
来源：http://www.ydjk.org.cn/Article/details/gt2stlawnok.html

[U101] JS：classList 操作
来源：http://www.52xcode.cn/Article/details/gt2uzxjjjhi.html

el.classList.toggle("active")
来源：http://www.52xcode.cn/Article/details/gt2nedapqaz.html

[U102] JS：本地存储
来源：http://www.ydjk.org.cn/Article/details/gt2fwtgddqw.html

localStorage.setItem("k", JSON.stringify(v))
来源：http://www.ydjk.org.cn/Article/details/gt2svjhsahs.html

[U103] JS：定时器
来源：http://www.ydjk.org.cn/Article/details/gt2cmnwisda.html

setTimeout(fn, 1000);  setInterval(fn, 1000);
来源：http://www.ydjk.org.cn/Article/details/gt2wgmnwtdp.html

[U104] JS：防抖
来源：http://www.ydjk.org.cn/Article/details/gt2azahcmfv.html

const debounce = (fn, ms) => { let t; return (...a) => { clearTimeout(t); t = setTimeout(() => fn(...a), ms); }; };
来源：http://www.52xcode.cn/Article/details/gt2siukzlwg.html

[U105] JS：节流
来源：http://www.ydjk.org.cn/Article/details/gt2vfwxnsmz.html

const throttle = (fn, ms) => { let last = 0; return (...a) => { const n = Date.now(); if (n - last >= ms) { last = n; fn(...a); } }; };
来源：http://www.52xcode.cn/Article/details/gt2talzjmel.html

[U106] JS：日期格式化
来源：http://www.ydjk.org.cn/Article/details/gt2cgaohacv.html

new Intl.DateTimeFormat("zh-CN", { dateStyle: "medium" }).format(new Date())
来源：http://www.52xcode.cn/Article/details/gt2lgxpuumb.html

[U107] JS：数字千分位
来源：http://www.ydjk.org.cn/Article/details/gt2tzvueaze.html

new Intl.NumberFormat("en-US").format(1234567)
来源：http://www.ydjk.org.cn/Article/details/gt2wgmwdkli.html

[U108] JS：随机整数
来源：http://www.52xcode.cn/Article/details/gt2tbxhkhfh.html

Math.floor(Math.random() * (max - min + 1)) + min
来源：http://www.52xcode.cn/Article/details/gt2jfsaevnq.html

[U109] JS：数组分组
来源：http://www.ydjk.org.cn/Article/details/gt2owdgxsaz.html

Object.groupBy(arr, x => x.type)
来源：http://www.ydjk.org.cn/Article/details/gt2spibijix.html

[U110] JS：数组分块
来源：http://www.ydjk.org.cn/Article/details/gt2esdkyenw.html

arr.reduce((acc, x, i) => (i % size ? acc : [...acc, arr.slice(i, i + size)]), [])
来源：http://www.ydjk.org.cn/Article/details/gt2yqmguggk.html

[U111] JS：对象转 Map
来源：http://www.52xcode.cn/Article/details/gt2gewhllga.html

new Map(Object.entries(obj))
来源：http://www.ydjk.org.cn/Article/details/gt2fqulmfmn.html

[U112] JS：字符串补位
来源：http://www.ydjk.org.cn/Article/details/gt2pkdfbgsk.html

"7".padStart(3, "0")
来源：http://www.52xcode.cn/Article/details/gt2mkpfwdrb.html

[U113] JS：正则替换全部
来源：http://www.ydjk.org.cn/Article/details/gt2rtsgjnjb.html

s.replaceAll("a", "b")
来源：http://www.ydjk.org.cn/Article/details/gt2sermeivg.html

[U114] JS：JSON 深比较
来源：http://www.52xcode.cn/Article/details/gt2qhbaidui.html

JSON.stringify(a) === JSON.stringify(b)
来源：http://www.52xcode.cn/Article/details/gt2vuckmbgf.html

[U115] JS：生成 UUID
来源：http://www.52xcode.cn/Article/details/gt2cclowqyb.html

crypto.randomUUID()
来源：http://www.ydjk.org.cn/Article/details/gt2dgpzefgs.html

[U116] JS：类型检查（JSDoc）
来源：http://www.ydjk.org.cn/Article/details/gt2pujyrxqn.html

/** @param {string} name */ function f(name) {}
来源：http://www.52xcode.cn/Article/details/gt2dwhzzwot.html

[U117] JS：单元测试
来源：http://www.ydjk.org.cn/Article/details/gt2gnsyfrmx.html

npm i -D vitest;  npx vitest
来源：http://www.52xcode.cn/Article/details/gt2swblylcj.html

[U118] JS：开发服务器
来源：http://www.52xcode.cn/Article/details/gt2hwmlojhs.html

npm i -D vite;  npx vite
来源：http://www.52xcode.cn/Article/details/gt2nnstpaju.html

[U119] JS：生产构建
来源：http://www.52xcode.cn/Article/details/gt2ryadovlo.html

npx vite build
来源：http://www.52xcode.cn/Article/details/gt2ogmiemxb.html

[U120] JS：读取环境变量（Vite）
来源：http://www.ydjk.org.cn/Article/details/gt2fhpioovw.html

import.meta.env.VITE_API_URL
来源：http://www.ydjk.org.cn/Article/details/gt2dclnvdpm.html

================================================================================
来源：http://www.ydjk.org.cn/Article/details/gt2efsoseet.html

统计汇总
来源：http://www.52xcode.cn/Article/details/gt2qiaagdxl.html

================================================================================
来源：http://www.52xcode.cn/Article/details/gt2ilodkpjp.html

按语言统计（条）：
来源：http://www.52xcode.cn/Article/details/gt2qepoeiqg.html

Python ......... 252
来源：http://www.ydjk.org.cn/Article/details/gt2iiasdmmt.html

PHP ............ 252
来源：http://www.52xcode.cn/Article/details/gt2kzwietpo.html

JavaScript ..... 252
来源：http://www.ydjk.org.cn/Article/details/gt2bvtkmiyz.html

TypeScript ..... 212
来源：http://www.52xcode.cn/Article/details/gt2sbnfnopz.html

Java ........... 212
来源：http://www.52xcode.cn/Article/details/gt2kkyzwbed.html

Go ............. 212
来源：http://www.52xcode.cn/Article/details/gt2ollonemz.html

Ruby ........... 212
来源：http://www.ydjk.org.cn/Article/details/gt2xakfsmrw.html

C# ............. 212
来源：http://www.52xcode.cn/Article/details/gt2vpxlbldk.html

C .............. 30
来源：http://www.52xcode.cn/Article/details/gt2cbwomfkc.html

C++ ............ 30
来源：http://www.52xcode.cn/Article/details/gt2axexydnd.html

SQL ............ 90
来源：http://www.ydjk.org.cn/Article/details/gt2ixdgpvyu.html

Bash ........... 80
来源：http://www.ydjk.org.cn/Article/details/gt2onhpqrbf.html

Kotlin ......... 15
来源：http://www.ydjk.org.cn/Article/details/gt2toziizrp.html

Swift .......... 15
来源：http://www.ydjk.org.cn/Article/details/gt2yqxpezmo.html

Lua ............ 10
来源：http://www.ydjk.org.cn/Article/details/gt2vbttejyv.html

Perl ........... 10
来源：http://www.52xcode.cn/Article/details/gt2pyrsjanc.html

Scala .......... 10
来源：http://www.52xcode.cn/Article/details/gt2ykmathov.html

------------------------------------
来源：http://www.ydjk.org.cn/Article/details/gt2piscnpmf.html

合计 ........... 2106 条
来源：http://www.52xcode.cn/Article/details/gt2vjvworau.html

按章节统计：
来源：http://www.52xcode.cn/Article/details/gt2toaabxlq.html

A 基础语法与类型       26 个任务 × 8 语言 =  208
来源：http://www.ydjk.org.cn/Article/details/gt2aotnodff.html

B 流程控制             16 个任务 × 8 语言 =  128
来源：http://www.52xcode.cn/Article/details/gt2meqbwwrs.html

C 函数与作用域         16 个任务 × 8 语言 =  128
来源：http://www.52xcode.cn/Article/details/gt2meahligg.html

D 数组 / 列表 / 集合   26 个任务 × 8 语言 =  208
来源：http://www.52xcode.cn/Article/details/gt2iozqghon.html

E 字符串处理           22 个任务 × 8 语言 =  176
来源：http://www.52xcode.cn/Article/details/gt2rjgkkifg.html

F 文件与目录           12 个任务 × 8 语言 =   96
来源：http://www.52xcode.cn/Article/details/gt2wmvkuugy.html

G 面向对象             16 个任务 × 8 语言 =  128
来源：http://www.ydjk.org.cn/Article/details/gt2axzybuek.html

H 异常与错误处理       10 个任务 × 8 语言 =   80
来源：http://www.ydjk.org.cn/Article/details/gt2vkupndtm.html

I 正则表达式            8 个任务 × 8 语言 =   64
来源：http://www.ydjk.org.cn/Article/details/gt2mdrrlxoh.html

J 日期与时间           10 个任务 × 8 语言 =   80
来源：http://www.ydjk.org.cn/Article/details/gt2unobskak.html

K JSON 与序列化         8 个任务 × 8 语言 =   64
来源：http://www.52xcode.cn/Article/details/gt2hosaoiwh.html

L 网络请求              8 个任务 × 8 语言 =   64
来源：http://www.ydjk.org.cn/Article/details/gt2rniadoef.html

M 命令行 / 进程         8 个任务 × 8 语言 =   64
来源：http://www.52xcode.cn/Article/details/gt2ugzvwrmm.html

N 数据结构与算法       12 个任务 × 8 语言 =   96
来源：http://www.ydjk.org.cn/Article/details/gt2fwthcopu.html

O 并发与异步            6 个任务 × 8 语言 =   48
来源：http://www.52xcode.cn/Article/details/gt2wxhlvrms.html

P 常用工具函数          8 个任务 × 8 语言 =   64
来源：http://www.52xcode.cn/Article/details/gt2dkslpmzo.html

Q SQL 专题                              90
来源：http://www.52xcode.cn/Article/details/gt2zuwndhcd.html

R Bash 专题                             80
来源：http://www.52xcode.cn/Article/details/gt2dkhvcapc.html

S C / C++ 专题                          60
来源：http://www.52xcode.cn/Article/details/gt2mzfuhwqm.html

T 其他语言补充                          60
来源：http://www.52xcode.cn/Article/details/gt2jfodqxut.html

U 高频实用片段                         120
来源：http://www.52xcode.cn/Article/details/gt2oddxxmlr.html

------------------------------------
来源：http://www.52xcode.cn/Article/details/gt2lwyihzgb.html

合计                                  2106 条
来源：http://www.ydjk.org.cn/Article/details/gt2ihttffzx.html

--------------------------------------------------------------------------------
来源：http://www.ydjk.org.cn/Article/details/gt2gujkwkjo.html

使用提醒
来源：http://www.52xcode.cn/Article/details/gt2jeupjxad.html

--------------------------------------------------------------------------------
来源：http://www.ydjk.org.cn/Article/details/gt2udyxsldp.html

1. 示例追求"最小可用"，正式项目中请补齐导入、错误处理与边界判断。
来源：http://www.ydjk.org.cn/Article/details/gt2qhetbiex.html

2. 涉及文件、网络、数据库的示例，注意资源释放与异常捕获。
来源：http://www.ydjk.org.cn/Article/details/gt2traceewb.html

3. 语言版本差异较大（如 Python 3.10 的 match、Java 17 的 record/switch 箭头），
来源：http://www.52xcode.cn/Article/details/gt2nuuggffq.html

在旧版本上使用前请先确认语法支持情况。
来源：http://www.52xcode.cn/Article/details/gt2wfioweyy.html

4. 标注"手写"的条目是因为该语言缺少对应内置能力，实际项目中可引入成熟库。
来源：http://www.52xcode.cn/Article/details/gt2aiiwhtgf.html

—— 文件结束 ——
来源：http://www.ydjk.org.cn/Article/details/gt2wdpjbuxh.html

================================================================================
来源：http://www.ydjk.org.cn/Article/details/gt2ofkhlwtj.html

程序语言常见例子速查手册（2024 版）
来源：http://www.ydjk.org.cn/Article/details/gt2hobcfnlw.html

Common Programming Examples Cheat Book
来源：http://www.52xcode.cn/Article/details/gt2eokaoqcp.html

================================================================================
来源：http://www.ydjk.org.cn/Article/details/gt2lmvzjmkd.html

【收录内容】
来源：http://www.ydjk.org.cn/Article/details/gt2kzqcbxhb.html

覆盖 12 种语言 / 语法与常见 API：
来源：http://www.52xcode.cn/Article/details/gt2kymkhalk.html

Python · PHP · JavaScript · TypeScript · Java · Go · Ruby · C#
来源：http://www.ydjk.org.cn/Article/details/gt2fqtcrcjg.html

SQL · Bash · C · C++
来源：http://www.52xcode.cn/Article/details/gt2jxevfxrz.html


<!-- 参考信息 -->