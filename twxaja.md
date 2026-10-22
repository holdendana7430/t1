代发 wailian999

[U01] Py：创建虚拟环境
来源：http://www.ydjk.org.cn/Article/details/gt2upcmsczo.html

python -m venv .venv && source .venv/bin/activate
来源：http://www.52xcode.cn/Article/details/gt2wmaxahik.html

[U02] Py：导出 / 安装依赖
来源：http://www.ydjk.org.cn/Article/details/gt2chuslwor.html

pip freeze > requirements.txt;  pip install -r requirements.txt
来源：http://www.ydjk.org.cn/Article/details/gt2ewxnuyav.html

[U03] Py：加载 .env 配置
来源：http://www.52xcode.cn/Article/details/gt2tdemcfgp.html

from dotenv import load_dotenv; load_dotenv()
来源：http://www.ydjk.org.cn/Article/details/gt2whkkpjsu.html

[U04] Py：变量调试打印
来源：http://www.52xcode.cn/Article/details/gt2estoeoae.html

print(f"{x=}")            # 输出 x=值，Python 3.8+
来源：http://www.ydjk.org.cn/Article/details/gt2pnmhclbc.html

[U05] Py：列表去重且保序
来源：http://www.52xcode.cn/Article/details/gt2grhriabi.html

list(dict.fromkeys(arr))
来源：http://www.52xcode.cn/Article/details/gt2yikhgujr.html

[U06] Py：合并两个字典
来源：http://www.52xcode.cn/Article/details/gt2btosnywp.html

{**a, **b}
来源：http://www.52xcode.cn/Article/details/gt2xpnbwufb.html

[U07] Py：反转字典键值
来源：http://www.ydjk.org.cn/Article/details/gt2eulmpbvt.html

{v: k for k, v in d.items()}
来源：http://www.52xcode.cn/Article/details/gt2opyijozt.html

[U08] Py：展平二维列表
来源：http://www.ydjk.org.cn/Article/details/gt2mdjvdjpu.html

[y for x in nested for y in x]
来源：http://www.ydjk.org.cn/Article/details/gt2wbdcugzk.html

[U09] Py：字典取最大值的键
来源：http://www.ydjk.org.cn/Article/details/gt2chqusnry.html

max(d, key=d.get)
来源：http://www.ydjk.org.cn/Article/details/gt2ljacvpcd.html

[U10] Py：按值排序字典
来源：http://www.ydjk.org.cn/Article/details/gt2pblrnglz.html

dict(sorted(d.items(), key=lambda kv: kv[1]))
来源：http://www.52xcode.cn/Article/details/gt2ojdtqmze.html

[U11] Py：生成器表达式
来源：http://www.ydjk.org.cn/Article/details/gt2bkghbkzj.html

(x * 2 for x in arr)
来源：http://www.ydjk.org.cn/Article/details/gt2srarcgyq.html

[U12] Py：取出现最多的 3 个元素
来源：http://www.52xcode.cn/Article/details/gt2tvxphmqh.html

Counter(arr).most_common(3)
来源：http://www.52xcode.cn/Article/details/gt2lochxhrv.html

[U13] Py：固定长度队列
来源：http://www.52xcode.cn/Article/details/gt2bqlvrgli.html

deque(maxlen=10)
来源：http://www.52xcode.cn/Article/details/gt2nthsytks.html

[U14] Py：分组收集到列表
来源：http://www.ydjk.org.cn/Article/details/gt2xqococxl.html

defaultdict(list)
来源：http://www.ydjk.org.cn/Article/details/gt2pkhubkif.html

[U15] Py：高精度计时
来源：http://www.52xcode.cn/Article/details/gt2olecxsuf.html

t = time.perf_counter()
来源：http://www.ydjk.org.cn/Article/details/gt2ysrjzkez.html

[U16] Py：命令行参数解析
来源：http://www.52xcode.cn/Article/details/gt2tqnqyqne.html

ap = argparse.ArgumentParser();  ap.add_argument("--name");  args = ap.parse_args()
来源：http://www.52xcode.cn/Article/details/gt2ogjxyitn.html

[U17] Py：初始化日志
来源：http://www.52xcode.cn/Article/details/gt2hfkneikr.html

logging.basicConfig(level=logging.INFO)
来源：http://www.52xcode.cn/Article/details/gt2wockehgl.html

[U18] Py：预编译正则
来源：http://www.ydjk.org.cn/Article/details/gt2dxycnjul.html

pat = re.compile(r"\d+")
来源：http://www.ydjk.org.cn/Article/details/gt2fljcpsok.html

[U19] Py：正则替换带回调
来源：http://www.52xcode.cn/Article/details/gt2oypasxhi.html

re.sub(r"\d+", lambda m: str(int(m.group()) * 2), s)
来源：http://www.ydjk.org.cn/Article/details/gt2epyfsvfs.html

[U20] Py：缓存函数结果
来源：http://www.52xcode.cn/Article/details/gt2xfawerlt.html

@functools.lru_cache(maxsize=None)
来源：http://www.52xcode.cn/Article/details/gt2nhggmvoq.html

[U21] Py：自定义上下文管理器
来源：http://www.52xcode.cn/Article/details/gt2wiyvagdr.html

@contextlib.contextmanager
来源：http://www.52xcode.cn/Article/details/gt2xsdplffc.html

[U22] Py：矩阵转置
来源：http://www.ydjk.org.cn/Article/details/gt2baqpuavi.html

list(zip(*m))
来源：http://www.ydjk.org.cn/Article/details/gt2awuiuhyf.html

[U23] Py：分块读取大文件
来源：http://www.ydjk.org.cn/Article/details/gt2ppahgjev.html

for chunk in iter(lambda: f.read(8192), b""):
来源：http://www.52xcode.cn/Article/details/gt2skbwkelf.html

[U24] Py：路径操作
来源：http://www.52xcode.cn/Article/details/gt2xnwrartq.html

Path("a/b.txt").parent.mkdir(parents=True, exist_ok=True)
来源：http://www.52xcode.cn/Article/details/gt2dnszsasq.html

[U25] Py：CSV 按字典读
来源：http://www.52xcode.cn/Article/details/gt2qkutjeri.html

csv.DictReader(f)
来源：http://www.ydjk.org.cn/Article/details/gt2gxdjaxdo.html

[U26] Py：并发下载
来源：http://www.52xcode.cn/Article/details/gt2ymadoyiy.html

ThreadPoolExecutor(max_workers=8).map(fetch, urls)
来源：http://www.ydjk.org.cn/Article/details/gt2wwcbvbjl.html

[U27] Py：异步 HTTP
来源：http://www.52xcode.cn/Article/details/gt2qvtaspar.html

aiohttp.ClientSession() 配合 async with
来源：http://www.ydjk.org.cn/Article/details/gt2tgvpfcfq.html

[U28] Py：类型别名
来源：http://www.52xcode.cn/Article/details/gt2csrovnug.html

UserId = int
来源：http://www.ydjk.org.cn/Article/details/gt2djzhtpuj.html

[U29] Py：属性校验
来源：http://www.ydjk.org.cn/Article/details/gt2ryijkapi.html

@property 与 @x.setter 配合
来源：http://www.ydjk.org.cn/Article/details/gt2mkvbsdjj.html

[U30] Py：数据类
来源：http://www.ydjk.org.cn/Article/details/gt2erqflygr.html

@dataclass(slots=True)
来源：http://www.52xcode.cn/Article/details/gt2lyeodygg.html

[U31] Py：单测
来源：http://www.52xcode.cn/Article/details/gt2pfbegkkn.html

python -m pytest -q
来源：http://www.52xcode.cn/Article/details/gt2yiecmcdg.html

[U32] Py：代码格式化
来源：http://www.ydjk.org.cn/Article/details/gt2hiyxxqtu.html

ruff format . && ruff check --fix .
来源：http://www.52xcode.cn/Article/details/gt2dofhmdaa.html

[U33] Py：打包发布
来源：http://www.ydjk.org.cn/Article/details/gt2teukkyhn.html

python -m build  （依赖 pyproject.toml）
来源：http://www.ydjk.org.cn/Article/details/gt2qilhzeqe.html

[U34] Py：判断编码
来源：http://www.ydjk.org.cn/Article/details/gt2mvarrbvn.html

chardet.detect(raw)
来源：http://www.ydjk.org.cn/Article/details/gt2gwawuvmr.html

[U35] Py：发送邮件
来源：http://www.ydjk.org.cn/Article/details/gt2idqfohwp.html

smtplib.SMTP_SSL(...).send_message(msg)
来源：http://www.ydjk.org.cn/Article/details/gt2thimvjip.html

[U36] Py：定时任务
来源：http://www.52xcode.cn/Article/details/gt2qjfdhfjc.html

schedule.every(10).minutes.do(job)
来源：http://www.ydjk.org.cn/Article/details/gt2dvfkatkk.html

[U37] Py：读写 Excel
来源：http://www.ydjk.org.cn/Article/details/gt2gkbusgvi.html

pandas.read_excel / DataFrame.to_excel
来源：http://www.52xcode.cn/Article/details/gt2jxsliylv.html

[U38] Py：获取脚本所在目录
来源：http://www.ydjk.org.cn/Article/details/gt2scrsoscs.html

Path(__file__).resolve().parent
来源：http://www.52xcode.cn/Article/details/gt2wdtkahwd.html

[U39] Py：判断是否在交互环境
来源：http://www.ydjk.org.cn/Article/details/gt2zwctjpvw.html

sys.stdout.isatty()
来源：http://www.52xcode.cn/Article/details/gt2sizzloew.html

[U40] Py：打印到标准错误
来源：http://www.ydjk.org.cn/Article/details/gt2eqtqoiyw.html

print("err", file=sys.stderr)
来源：http://www.52xcode.cn/Article/details/gt2iyjtymvn.html

[U41] PHP：初始化 Composer 项目
来源：http://www.ydjk.org.cn/Article/details/gt2eocqpvzv.html

composer init;  composer require guzzlehttp/guzzle
来源：http://www.ydjk.org.cn/Article/details/gt2zknkdyav.html

[U42] PHP：PSR-4 自动加载
来源：http://www.52xcode.cn/Article/details/gt2hzkqhxat.html

"autoload": { "psr-4": { "App\\": "src/" } }
来源：http://www.52xcode.cn/Article/details/gt2rppxtlnr.html

[U43] PHP：声明命名空间
来源：http://www.52xcode.cn/Article/details/gt2esremuso.html

namespace App\Http;
来源：http://www.52xcode.cn/Article/details/gt2wjgzwbyr.html

[U44] PHP：开启严格类型
来源：http://www.ydjk.org.cn/Article/details/gt2aydgdcmc.html

declare(strict_types=1);
来源：http://www.ydjk.org.cn/Article/details/gt2kfnvbdke.html

[U45] PHP：类型声明与返回类型
来源：http://www.52xcode.cn/Article/details/gt2fdzmaowx.html

function add(int $a, int $b): int { return $a + $b; }
来源：http://www.ydjk.org.cn/Article/details/gt2olvnqrxy.html

[U46] PHP：可空类型
来源：http://www.52xcode.cn/Article/details/gt2qmoilqlc.html

?string $name = null
来源：http://www.ydjk.org.cn/Article/details/gt2aoukuiqs.html

[U47] PHP：联合类型
来源：http://www.ydjk.org.cn/Article/details/gt2xxbdzbic.html

int|string $id
来源：http://www.ydjk.org.cn/Article/details/gt2sfkgjyrs.html

[U48] PHP：纯枚举
来源：http://www.ydjk.org.cn/Article/details/gt2kzdxqykj.html

enum Status: string { case Active = "active"; case Off = "off"; }
来源：http://www.ydjk.org.cn/Article/details/gt2zjnbwdai.html

[U49] PHP：只读属性
来源：http://www.52xcode.cn/Article/details/gt2prkgvvau.html

public readonly string $name
来源：http://www.ydjk.org.cn/Article/details/gt2qreykikc.html

[U50] PHP：构造器属性提升
来源：http://www.52xcode.cn/Article/details/gt2tycaqbku.html

public function __construct(private int $id) {}
来源：http://www.ydjk.org.cn/Article/details/gt2dsgenqrr.html

[U51] PHP：数组解构
来源：http://www.52xcode.cn/Article/details/gt2qichuail.html

[$a, $b] = $arr;
来源：http://www.ydjk.org.cn/Article/details/gt2jibfwyjk.html

[U52] PHP：箭头函数
来源：http://www.52xcode.cn/Article/details/gt2xvwtntrv.html

$double = fn($x) => $x * 2;
来源：http://www.52xcode.cn/Article/details/gt2ftjmxmab.html

[U53] PHP：空合并运算符
来源：http://www.ydjk.org.cn/Article/details/gt2qdiocqed.html

$v = $a ?? $b ?? "default";
来源：http://www.ydjk.org.cn/Article/details/gt2tcqwxuzx.html

[U54] PHP：空安全调用
来源：http://www.ydjk.org.cn/Article/details/gt2ncqdwxio.html

$obj?->method()
来源：http://www.52xcode.cn/Article/details/gt2fptjrwlt.html

[U55] PHP：match 表达式
来源：http://www.52xcode.cn/Article/details/gt2kefzguyi.html

$s = match($x) { 1 => "一", default => "其他" };
来源：http://www.ydjk.org.cn/Article/details/gt2firoxucq.html

[U56] PHP：命名参数
来源：http://www.52xcode.cn/Article/details/gt2ioajoltf.html

f(a: 1, b: 2)
来源：http://www.52xcode.cn/Article/details/gt2kugkdprc.html

[U57] PHP：字符串插值
来源：http://www.ydjk.org.cn/Article/details/gt2nhioyvab.html

"值: {$a}"
来源：http://www.52xcode.cn/Article/details/gt2ugxbarlz.html

[U58] PHP：数组三件套
来源：http://www.ydjk.org.cn/Article/details/gt2umntytdy.html

array_map($f, $a);  array_filter($a, $f);  array_reduce($a, $f, 0);
来源：http://www.52xcode.cn/Article/details/gt2ugyztozy.html

[U59] PHP：自定义排序
来源：http://www.ydjk.org.cn/Article/details/gt2mrxbsbsi.html

usort($arr, fn($a, $b) => $a["age"] <=> $b["age"]);
来源：http://www.52xcode.cn/Article/details/gt2ahjdkbip.html

[U60] PHP：JSON 编解码
来源：http://www.ydjk.org.cn/Article/details/gt2wrfvwnny.html

json_encode($d, JSON_UNESCAPED_UNICODE);  json_decode($s, true);
来源：http://www.ydjk.org.cn/Article/details/gt2gdsllqgd.html

[U61] PHP：正则
来源：http://www.ydjk.org.cn/Article/details/gt2ubdyeraa.html

preg_match('/(\d+)/', $s, $m);  preg_replace('/\d+/', '#', $s);
来源：http://www.52xcode.cn/Article/details/gt2qqqggnxk.html

[U62] PHP：日期对象
来源：http://www.52xcode.cn/Article/details/gt2hkkilciz.html

(new DateTimeImmutable())->format("Y-m-d");
来源：http://www.52xcode.cn/Article/details/gt2lbvhdxyi.html

[U63] PHP：文件读写
来源：http://www.ydjk.org.cn/Article/details/gt2aioojwcu.html

file_get_contents($f);  file_put_contents($f, $data);
来源：http://www.ydjk.org.cn/Article/details/gt2hoiiqtfr.html

[U64] PHP：目录遍历
来源：http://www.ydjk.org.cn/Article/details/gt2ceztmrui.html

glob("dir/*.php");  scandir("dir");
来源：http://www.52xcode.cn/Article/details/gt2rjtzlhri.html

[U65] PHP：会话
来源：http://www.52xcode.cn/Article/details/gt2gswwgtcr.html

session_start();  $_SESSION["uid"] = 1;
来源：http://www.ydjk.org.cn/Article/details/gt2mkbgbfsi.html

[U66] PHP：设置 Cookie
来源：http://www.52xcode.cn/Article/details/gt2jkpzkjxp.html

setcookie("token", $v, ["httponly" => true, "samesite" => "Lax"]);
来源：http://www.52xcode.cn/Article/details/gt2xegpiven.html

[U67] PHP：处理文件上传
来源：http://www.52xcode.cn/Article/details/gt2pxlmxmnc.html

$_FILES["file"]["tmp_name"] 与 move_uploaded_file()
来源：http://www.ydjk.org.cn/Article/details/gt2hnjvolml.html

[U68] PHP：PDO 连接
来源：http://www.52xcode.cn/Article/details/gt2euareiqs.html

$pdo = new PDO("mysql:host=localhost;dbname=app", "root", "");
来源：http://www.ydjk.org.cn/Article/details/gt2yjpjdbgr.html

[U69] PHP：PDO 预处理
来源：http://www.52xcode.cn/Article/details/gt2irhdubte.html

$stmt = $pdo->prepare("SELECT * FROM users WHERE id = ?");  $stmt->execute([$id]);
来源：http://www.52xcode.cn/Article/details/gt2dkqphgri.html

[U70] PHP：PDO 事务
来源：http://www.ydjk.org.cn/Article/details/gt2encuaphz.html

$pdo->beginTransaction();  $pdo->commit();  $pdo->rollBack();
来源：http://www.ydjk.org.cn/Article/details/gt2bwchhhfv.html

[U71] PHP：抛出异常
来源：http://www.52xcode.cn/Article/details/gt2wstadadj.html

throw new RuntimeException("失败", 500);
来源：http://www.52xcode.cn/Article/details/gt2vjjvxpog.html

[U72] PHP：写错误日志
来源：http://www.52xcode.cn/Article/details/gt2gastnmox.html

error_log("失败: " . $e->getMessage());
来源：http://www.ydjk.org.cn/Article/details/gt2omyuqzet.html

[U73] PHP：读取 ini 配置
来源：http://www.52xcode.cn/Article/details/gt2blugwhcz.html

parse_ini_file("config.ini", true)
来源：http://www.52xcode.cn/Article/details/gt2mxtlljql.html

[U74] PHP：读取环境变量
来源：http://www.52xcode.cn/Article/details/gt2jdiafbog.html

getenv("APP_ENV") ?: "production"
来源：http://www.ydjk.org.cn/Article/details/gt2pishxnrc.html

[U75] PHP：依赖注入
来源：http://www.ydjk.org.cn/Article/details/gt2jyovvgxu.html

composer require psr/container
来源：http://www.52xcode.cn/Article/details/gt2cymghnzx.html

[U76] PHP：简单路由
来源：http://www.52xcode.cn/Article/details/gt2fzbjndsk.html

$path = parse_url($_SERVER["REQUEST_URI"], PHP_URL_PATH);
来源：http://www.ydjk.org.cn/Article/details/gt2ykkqlyby.html

[U77] PHP：模板渲染
来源：http://www.ydjk.org.cn/Article/details/gt2faudoexo.html

composer require twig/twig
来源：http://www.52xcode.cn/Article/details/gt2tgeudfib.html

[U78] PHP：单元测试
来源：http://www.52xcode.cn/Article/details/gt2omftnrkq.html

composer require --dev phpunit/phpunit
来源：http://www.ydjk.org.cn/Article/details/gt2oxkqkkbt.html

[U79] PHP：静态分析
来源：http://www.52xcode.cn/Article/details/gt2iglsakut.html

composer require --dev phpstan/phpstan
来源：http://www.52xcode.cn/Article/details/gt2bbntecjz.html

[U80] PHP：代码规范修复
来源：http://www.52xcode.cn/Article/details/gt2awqwseqn.html

composer require --dev friendsofphp/php-cs-fixer
来源：http://www.ydjk.org.cn/Article/details/gt2browztsw.html

[U81] JS：初始化项目
来源：http://www.52xcode.cn/Article/details/gt2clpbiblj.html

npm init -y;  npm i express
来源：http://www.52xcode.cn/Article/details/gt2tvpswkox.html

[U82] JS：package.json 脚本
来源：http://www.ydjk.org.cn/Article/details/gt2bzzxvozw.html

"scripts": { "dev": "vite", "build": "vite build" }
来源：http://www.52xcode.cn/Article/details/gt2sparjegn.html

[U83] JS：ES Module 导入导出
来源：http://www.ydjk.org.cn/Article/details/gt2ezznrlrf.html

export const a = 1;  import { a } from "./m.js";
来源：http://www.52xcode.cn/Article/details/gt2qbwrygne.html

[U84] JS：CommonJS 写法
来源：http://www.52xcode.cn/Article/details/gt2avvbwbxh.html

module.exports = { a };  const { a } = require("./m");
来源：http://www.ydjk.org.cn/Article/details/gt2aznpvmec.html

[U85] JS：可选链
来源：http://www.ydjk.org.cn/Article/details/gt2obpfgwtk.html

a?.b?.c
来源：http://www.ydjk.org.cn/Article/details/gt2qlkxrnur.html

[U86] JS：空值合并
来源：http://www.52xcode.cn/Article/details/gt2ouqeexks.html

a ?? b
来源：http://www.52xcode.cn/Article/details/gt2uysncfiq.html

[U87] JS：解构默认值
来源：http://www.52xcode.cn/Article/details/gt2rfffsrfv.html

const { a = 1, b = 2 } = obj;
来源：http://www.ydjk.org.cn/Article/details/gt2izwkbzhe.html

[U88] JS：对象展开合并
来源：http://www.ydjk.org.cn/Article/details/gt2wmxsxnsf.html

{ ...a, ...b }
来源：http://www.ydjk.org.cn/Article/details/gt2kqnfwbba.html

[U89] JS：数组去重
来源：http://www.ydjk.org.cn/Article/details/gt2dafpepsc.html

[...new Set(arr)]
来源：http://www.52xcode.cn/Article/details/gt2sqhxssfb.html

[U90] JS：数字数组排序
来源：http://www.ydjk.org.cn/Article/details/gt2wlxhkbix.html

[...arr].sort((a, b) => a - b)
来源：http://www.ydjk.org.cn/Article/details/gt2spawabga.html

[U91] JS：对象键值遍历
来源：http://www.ydjk.org.cn/Article/details/gt2gvnicihv.html

Object.entries(obj).forEach(([k, v]) => {});
来源：http://www.ydjk.org.cn/Article/details/gt2mdbzpfhx.html

[U92] JS：深拷贝
来源：http://www.ydjk.org.cn/Article/details/gt2yhdnvvas.html

structuredClone(obj)
来源：http://www.52xcode.cn/Article/details/gt2yonsadkt.html

[U93] JS：模板字符串
来源：http://www.ydjk.org.cn/Article/details/gt2jutzhwqn.html

`共 ${n} 条`
来源：http://www.52xcode.cn/Article/details/gt2ffpfjduu.html

[U94] JS：箭头函数
来源：http://www.52xcode.cn/Article/details/gt2htpfpiih.html

const double = x => x * 2;
来源：http://www.ydjk.org.cn/Article/details/gt2mjmnyywz.html

[U95] JS：Promise 包装
来源：http://www.ydjk.org.cn/Article/details/gt2ksxbrmun.html

new Promise((resolve, reject) => {})
来源：http://www.ydjk.org.cn/Article/details/gt2pppyzsgx.html

[U96] JS：async/await 与异常
来源：http://www.52xcode.cn/Article/details/gt2dnjqwarm.html

try { const d = await f(); } catch (e) { console.error(e); }
来源：http://www.ydjk.org.cn/Article/details/gt2tviohwwh.html

[U97] JS：并发请求
来源：http://www.ydjk.org.cn/Article/details/gt2jjhsabwf.html

await Promise.all(urls.map(u => fetch(u)))
来源：http://www.52xcode.cn/Article/details/gt2mexxkcmh.html

[U98] JS：fetch 带 JSON
来源：http://www.52xcode.cn/Article/details/gt2xkidgyco.html

await fetch(url, { method: "POST", headers: { "Content-Type": "application/json" }, body: JSON.stringify(d) })
来源：http://www.52xcode.cn/Article/details/gt2jxnjodtj.html

[U99] JS：事件监听
来源：http://www.ydjk.org.cn/Article/details/gt2gtoyxjks.html

el.addEventListener("click", e => {})
来源：http://www.ydjk.org.cn/Article/details/gt2aaezaqmp.html

[U100] JS：DOM 查询
来源：http://www.52xcode.cn/Article/details/gt2lzqjpzxv.html

document.querySelector(".item")
来源：http://www.ydjk.org.cn/Article/details/gt2dwwlsoab.html

[U101] JS：classList 操作
来源：http://www.52xcode.cn/Article/details/gt2bvlwzuri.html

el.classList.toggle("active")
来源：http://www.ydjk.org.cn/Article/details/gt2zcbcaowk.html

[U102] JS：本地存储
来源：http://www.52xcode.cn/Article/details/gt2oxrwvfak.html

localStorage.setItem("k", JSON.stringify(v))
来源：http://www.ydjk.org.cn/Article/details/gt2milgsrnh.html

[U103] JS：定时器
来源：http://www.52xcode.cn/Article/details/gt2vwhqkkfi.html

setTimeout(fn, 1000);  setInterval(fn, 1000);
来源：http://www.52xcode.cn/Article/details/gt2ndomhnpb.html

[U104] JS：防抖
来源：http://www.ydjk.org.cn/Article/details/gt2wdsysoix.html

const debounce = (fn, ms) => { let t; return (...a) => { clearTimeout(t); t = setTimeout(() => fn(...a), ms); }; };
来源：http://www.52xcode.cn/Article/details/gt2yxhiyjyn.html

[U105] JS：节流
来源：http://www.ydjk.org.cn/Article/details/gt2fhvnmxys.html

const throttle = (fn, ms) => { let last = 0; return (...a) => { const n = Date.now(); if (n - last >= ms) { last = n; fn(...a); } }; };
来源：http://www.52xcode.cn/Article/details/gt2mqvwztms.html

[U106] JS：日期格式化
来源：http://www.52xcode.cn/Article/details/gt2igwuqdva.html

new Intl.DateTimeFormat("zh-CN", { dateStyle: "medium" }).format(new Date())
来源：http://www.ydjk.org.cn/Article/details/gt2okdryndo.html

[U107] JS：数字千分位
来源：http://www.ydjk.org.cn/Article/details/gt2rxbshclf.html

new Intl.NumberFormat("en-US").format(1234567)
来源：http://www.52xcode.cn/Article/details/gt2wobmrdqe.html

[U108] JS：随机整数
来源：http://www.52xcode.cn/Article/details/gt2zkxzmvfn.html

Math.floor(Math.random() * (max - min + 1)) + min
来源：http://www.52xcode.cn/Article/details/gt2hgcyfgjq.html

[U109] JS：数组分组
来源：http://www.52xcode.cn/Article/details/gt2fbewgvlr.html

Object.groupBy(arr, x => x.type)
来源：http://www.ydjk.org.cn/Article/details/gt2diaggdjo.html

[U110] JS：数组分块
来源：http://www.52xcode.cn/Article/details/gt2rvtnebqb.html

arr.reduce((acc, x, i) => (i % size ? acc : [...acc, arr.slice(i, i + size)]), [])
来源：http://www.ydjk.org.cn/Article/details/gt2xuuqlttf.html

[U111] JS：对象转 Map
来源：http://www.ydjk.org.cn/Article/details/gt2wcvwxcuv.html

new Map(Object.entries(obj))
来源：http://www.ydjk.org.cn/Article/details/gt2ozexznzn.html

[U112] JS：字符串补位
来源：http://www.ydjk.org.cn/Article/details/gt2ampgcsyb.html

"7".padStart(3, "0")
来源：http://www.ydjk.org.cn/Article/details/gt2tgkgzgnk.html

[U113] JS：正则替换全部
来源：http://www.ydjk.org.cn/Article/details/gt2eakvvxek.html

s.replaceAll("a", "b")
来源：http://www.ydjk.org.cn/Article/details/gt2cmmlqebz.html

[U114] JS：JSON 深比较
来源：http://www.52xcode.cn/Article/details/gt2lgbzjpox.html

JSON.stringify(a) === JSON.stringify(b)
来源：http://www.52xcode.cn/Article/details/gt2mfndnvpx.html

[U115] JS：生成 UUID
来源：http://www.52xcode.cn/Article/details/gt2jrpgfelr.html

crypto.randomUUID()
来源：http://www.52xcode.cn/Article/details/gt2hvoybypa.html

[U116] JS：类型检查（JSDoc）
来源：http://www.ydjk.org.cn/Article/details/gt2otetqwij.html

/** @param {string} name */ function f(name) {}
来源：http://www.52xcode.cn/Article/details/gt2cisdbldw.html

[U117] JS：单元测试
来源：http://www.ydjk.org.cn/Article/details/gt2itsumgev.html

npm i -D vitest;  npx vitest
来源：http://www.ydjk.org.cn/Article/details/gt2tvkhiegb.html

[U118] JS：开发服务器
来源：http://www.52xcode.cn/Article/details/gt2fvejbcnl.html

npm i -D vite;  npx vite
来源：http://www.ydjk.org.cn/Article/details/gt2snhvcdtn.html

[U119] JS：生产构建
来源：http://www.ydjk.org.cn/Article/details/gt2nujrgfkg.html

npx vite build
来源：http://www.52xcode.cn/Article/details/gt2awapaojh.html

[U120] JS：读取环境变量（Vite）
来源：http://www.52xcode.cn/Article/details/gt2jcoxlluv.html

import.meta.env.VITE_API_URL
来源：http://www.52xcode.cn/Article/details/gt2psqqltbu.html

================================================================================
来源：http://www.52xcode.cn/Article/details/gt2tgndmcpq.html

统计汇总
来源：http://www.ydjk.org.cn/Article/details/gt2mldoztlv.html

================================================================================
来源：http://www.52xcode.cn/Article/details/gt2bjewgdsw.html

按语言统计（条）：
来源：http://www.52xcode.cn/Article/details/gt2lexxdcsd.html

Python ......... 252
来源：http://www.ydjk.org.cn/Article/details/gt2xjlhtbtw.html

PHP ............ 252
来源：http://www.ydjk.org.cn/Article/details/gt2ocqyutkx.html

JavaScript ..... 252
来源：http://www.ydjk.org.cn/Article/details/gt2duvjmcgd.html

TypeScript ..... 212
来源：http://www.52xcode.cn/Article/details/gt2bpajglkz.html

Java ........... 212
来源：http://www.52xcode.cn/Article/details/gt2xbtolpbl.html

Go ............. 212
来源：http://www.52xcode.cn/Article/details/gt2ndartuak.html

Ruby ........... 212
来源：http://www.ydjk.org.cn/Article/details/gt2zvpmynum.html

C# ............. 212
来源：http://www.ydjk.org.cn/Article/details/gt2chobcwnx.html

C .............. 30
来源：http://www.ydjk.org.cn/Article/details/gt2ocvjybib.html

C++ ............ 30
来源：http://www.52xcode.cn/Article/details/gt2agjvikql.html

SQL ............ 90
来源：http://www.ydjk.org.cn/Article/details/gt2xsruyeun.html

Bash ........... 80
来源：http://www.ydjk.org.cn/Article/details/gt2xuzkvitr.html

Kotlin ......... 15
来源：http://www.ydjk.org.cn/Article/details/gt2wbncoryv.html

Swift .......... 15
来源：http://www.ydjk.org.cn/Article/details/gt2oncdbqlp.html

Lua ............ 10
来源：http://www.ydjk.org.cn/Article/details/gt2pdxgoshb.html

Perl ........... 10
来源：http://www.ydjk.org.cn/Article/details/gt2oqcmitem.html

Scala .......... 10
来源：http://www.52xcode.cn/Article/details/gt2olkyfbnm.html

------------------------------------
来源：http://www.52xcode.cn/Article/details/gt2orlxqpfz.html

合计 ........... 2106 条
来源：http://www.ydjk.org.cn/Article/details/gt2nfynphhh.html

按章节统计：
来源：http://www.52xcode.cn/Article/details/gt2mwnllymm.html

A 基础语法与类型       26 个任务 × 8 语言 =  208
来源：http://www.ydjk.org.cn/Article/details/gt2fabixbyx.html

B 流程控制             16 个任务 × 8 语言 =  128
来源：http://www.ydjk.org.cn/Article/details/gt2yohlmzpn.html

C 函数与作用域         16 个任务 × 8 语言 =  128
来源：http://www.52xcode.cn/Article/details/gt2ptanqnvg.html

D 数组 / 列表 / 集合   26 个任务 × 8 语言 =  208
来源：http://www.52xcode.cn/Article/details/gt2fywgdtmh.html

E 字符串处理           22 个任务 × 8 语言 =  176
来源：http://www.ydjk.org.cn/Article/details/gt2fjprwpgy.html

F 文件与目录           12 个任务 × 8 语言 =   96
来源：http://www.52xcode.cn/Article/details/gt2iwemigfi.html

G 面向对象             16 个任务 × 8 语言 =  128
来源：http://www.52xcode.cn/Article/details/gt2agqeeyaf.html

H 异常与错误处理       10 个任务 × 8 语言 =   80
来源：http://www.52xcode.cn/Article/details/gt2zepcouzw.html

I 正则表达式            8 个任务 × 8 语言 =   64
来源：http://www.ydjk.org.cn/Article/details/gt2ckicufsf.html

J 日期与时间           10 个任务 × 8 语言 =   80
来源：http://www.ydjk.org.cn/Article/details/gt2vixrpgil.html

K JSON 与序列化         8 个任务 × 8 语言 =   64
来源：http://www.52xcode.cn/Article/details/gt2zgknvpmf.html

L 网络请求              8 个任务 × 8 语言 =   64
来源：http://www.ydjk.org.cn/Article/details/gt2hxkiqwrd.html

M 命令行 / 进程         8 个任务 × 8 语言 =   64
来源：http://www.ydjk.org.cn/Article/details/gt2etpjcvhi.html

N 数据结构与算法       12 个任务 × 8 语言 =   96
来源：http://www.ydjk.org.cn/Article/details/gt2lrshyvxb.html

O 并发与异步            6 个任务 × 8 语言 =   48
来源：http://www.ydjk.org.cn/Article/details/gt2gyepxsdf.html

P 常用工具函数          8 个任务 × 8 语言 =   64
来源：http://www.ydjk.org.cn/Article/details/gt2mrnvtaof.html

Q SQL 专题                              90
来源：http://www.ydjk.org.cn/Article/details/gt2jcnydbtl.html

R Bash 专题                             80
来源：http://www.ydjk.org.cn/Article/details/gt2jkzjicof.html

S C / C++ 专题                          60
来源：http://www.52xcode.cn/Article/details/gt2fruhnfrh.html

T 其他语言补充                          60
来源：http://www.52xcode.cn/Article/details/gt2ontjoihl.html

U 高频实用片段                         120
来源：http://www.ydjk.org.cn/Article/details/gt2mjexaugp.html

------------------------------------
来源：http://www.52xcode.cn/Article/details/gt2qmmbypyy.html

合计                                  2106 条
来源：http://www.52xcode.cn/Article/details/gt2oxbwsmjw.html

--------------------------------------------------------------------------------
来源：http://www.52xcode.cn/Article/details/gt2rmroiylg.html

使用提醒
来源：http://www.ydjk.org.cn/Article/details/gt2jsqcuroz.html

--------------------------------------------------------------------------------
来源：http://www.ydjk.org.cn/Article/details/gt2pokiaqyo.html

1. 示例追求"最小可用"，正式项目中请补齐导入、错误处理与边界判断。
来源：http://www.ydjk.org.cn/Article/details/gt2rzmxanql.html

2. 涉及文件、网络、数据库的示例，注意资源释放与异常捕获。
来源：http://www.52xcode.cn/Article/details/gt2aspzdmwh.html

3. 语言版本差异较大（如 Python 3.10 的 match、Java 17 的 record/switch 箭头），
来源：http://www.52xcode.cn/Article/details/gt2kfeiewxg.html

在旧版本上使用前请先确认语法支持情况。
来源：http://www.52xcode.cn/Article/details/gt2wndhhktl.html

4. 标注"手写"的条目是因为该语言缺少对应内置能力，实际项目中可引入成熟库。
来源：http://www.52xcode.cn/Article/details/gt2lhxeigsh.html

—— 文件结束 ——
来源：http://www.52xcode.cn/Article/details/gt2xcycrljq.html

================================================================================
来源：http://www.52xcode.cn/Article/details/gt2vfvwnqst.html

程序语言常见例子速查手册（2024 版）
来源：http://www.ydjk.org.cn/Article/details/gt2nnuweamk.html

Common Programming Examples Cheat Book
来源：http://www.ydjk.org.cn/Article/details/gt2vibtdsyv.html

================================================================================
来源：http://www.ydjk.org.cn/Article/details/gt2jpxzzcrd.html


<!-- 参考信息 -->