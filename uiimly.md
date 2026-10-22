代发 wailian999

List(1, 2, 3).foldLeft(0)(_ + _)
来源：http://www.ydjk.org.cn/Article/details/gt2jwhmwdkk.html

================================================================================
来源：http://www.52xcode.cn/Article/details/gt2rdufolih.html

U. 高频实用片段（Python / PHP / JavaScript 各 40 条）
来源：http://www.52xcode.cn/Article/details/gt2ozijuxph.html

================================================================================
来源：http://www.52xcode.cn/Article/details/gt2gbwuhdww.html

[U01] Py：创建虚拟环境
来源：http://www.ydjk.org.cn/Article/details/gt2tbnurlnk.html

python -m venv .venv && source .venv/bin/activate
来源：http://www.52xcode.cn/Article/details/gt2mknudiry.html

[U02] Py：导出 / 安装依赖
来源：http://www.ydjk.org.cn/Article/details/gt2urgybwij.html

pip freeze > requirements.txt;  pip install -r requirements.txt
来源：http://www.52xcode.cn/Article/details/gt2dudpfybx.html

[U03] Py：加载 .env 配置
来源：http://www.52xcode.cn/Article/details/gt2redgfwew.html

from dotenv import load_dotenv; load_dotenv()
来源：http://www.52xcode.cn/Article/details/gt2ykwsdtbl.html

[U04] Py：变量调试打印
来源：http://www.ydjk.org.cn/Article/details/gt2xlbqtlhv.html

print(f"{x=}")            # 输出 x=值，Python 3.8+
来源：http://www.52xcode.cn/Article/details/gt2jeuttwpp.html

[U05] Py：列表去重且保序
来源：http://www.52xcode.cn/Article/details/gt2zwyywizh.html

list(dict.fromkeys(arr))
来源：http://www.ydjk.org.cn/Article/details/gt2urukhszh.html

[U06] Py：合并两个字典
来源：http://www.ydjk.org.cn/Article/details/gt2vhdihohn.html

{**a, **b}
来源：http://www.ydjk.org.cn/Article/details/gt2aueahsvv.html

[U07] Py：反转字典键值
来源：http://www.ydjk.org.cn/Article/details/gt2evlvnkos.html

{v: k for k, v in d.items()}
来源：http://www.52xcode.cn/Article/details/gt2dfywzqpe.html

[U08] Py：展平二维列表
来源：http://www.ydjk.org.cn/Article/details/gt2fabjxvlb.html

[y for x in nested for y in x]
来源：http://www.ydjk.org.cn/Article/details/gt2jalcxhbj.html

[U09] Py：字典取最大值的键
来源：http://www.52xcode.cn/Article/details/gt2bsbrtwjm.html

max(d, key=d.get)
来源：http://www.52xcode.cn/Article/details/gt2izmmtlju.html

[U10] Py：按值排序字典
来源：http://www.ydjk.org.cn/Article/details/gt2swynmtmr.html

dict(sorted(d.items(), key=lambda kv: kv[1]))
来源：http://www.ydjk.org.cn/Article/details/gt2qdddfopc.html

[U11] Py：生成器表达式
来源：http://www.ydjk.org.cn/Article/details/gt2rgjklqth.html

(x * 2 for x in arr)
来源：http://www.ydjk.org.cn/Article/details/gt2yqhvyphw.html

[U12] Py：取出现最多的 3 个元素
来源：http://www.ydjk.org.cn/Article/details/gt2rjuwelyy.html

Counter(arr).most_common(3)
来源：http://www.52xcode.cn/Article/details/gt2cjbvqncp.html

[U13] Py：固定长度队列
来源：http://www.ydjk.org.cn/Article/details/gt2guwpuwvd.html

deque(maxlen=10)
来源：http://www.ydjk.org.cn/Article/details/gt2qroitfeb.html

[U14] Py：分组收集到列表
来源：http://www.52xcode.cn/Article/details/gt2kojnazhu.html

defaultdict(list)
来源：http://www.52xcode.cn/Article/details/gt2pwpftqyk.html

[U15] Py：高精度计时
来源：http://www.ydjk.org.cn/Article/details/gt2bomztsrv.html

t = time.perf_counter()
来源：http://www.ydjk.org.cn/Article/details/gt2petvsrev.html

[U16] Py：命令行参数解析
来源：http://www.ydjk.org.cn/Article/details/gt2cxjgbpla.html

ap = argparse.ArgumentParser();  ap.add_argument("--name");  args = ap.parse_args()
来源：http://www.52xcode.cn/Article/details/gt2mfghrcqa.html

[U17] Py：初始化日志
来源：http://www.ydjk.org.cn/Article/details/gt2aaoyppnv.html

logging.basicConfig(level=logging.INFO)
来源：http://www.ydjk.org.cn/Article/details/gt2wfghrkzi.html

[U18] Py：预编译正则
来源：http://www.ydjk.org.cn/Article/details/gt2rofwmfgy.html

pat = re.compile(r"\d+")
来源：http://www.52xcode.cn/Article/details/gt2zavvadev.html

[U19] Py：正则替换带回调
来源：http://www.ydjk.org.cn/Article/details/gt2rwgvhdbz.html

re.sub(r"\d+", lambda m: str(int(m.group()) * 2), s)
来源：http://www.ydjk.org.cn/Article/details/gt2tuhzxhuk.html

[U20] Py：缓存函数结果
来源：http://www.52xcode.cn/Article/details/gt2dldrdlkn.html

@functools.lru_cache(maxsize=None)
来源：http://www.ydjk.org.cn/Article/details/gt2welnlpzv.html

[U21] Py：自定义上下文管理器
来源：http://www.ydjk.org.cn/Article/details/gt2jaadqnwu.html

@contextlib.contextmanager
来源：http://www.ydjk.org.cn/Article/details/gt2lncykduv.html

[U22] Py：矩阵转置
来源：http://www.52xcode.cn/Article/details/gt2qkiunqbu.html

list(zip(*m))
来源：http://www.52xcode.cn/Article/details/gt2atomcezf.html

[U23] Py：分块读取大文件
来源：http://www.52xcode.cn/Article/details/gt2qepgxxil.html

for chunk in iter(lambda: f.read(8192), b""):
来源：http://www.ydjk.org.cn/Article/details/gt2ysbqdfic.html

[U24] Py：路径操作
来源：http://www.52xcode.cn/Article/details/gt2lfgiiiev.html

Path("a/b.txt").parent.mkdir(parents=True, exist_ok=True)
来源：http://www.ydjk.org.cn/Article/details/gt2bjgauprp.html

[U25] Py：CSV 按字典读
来源：http://www.ydjk.org.cn/Article/details/gt2jlmjfzhm.html

csv.DictReader(f)
来源：http://www.ydjk.org.cn/Article/details/gt2kjprfslw.html

[U26] Py：并发下载
来源：http://www.52xcode.cn/Article/details/gt2jokornbv.html

ThreadPoolExecutor(max_workers=8).map(fetch, urls)
来源：http://www.52xcode.cn/Article/details/gt2vzwltscj.html

[U27] Py：异步 HTTP
来源：http://www.52xcode.cn/Article/details/gt2jlcwpnoq.html

aiohttp.ClientSession() 配合 async with
来源：http://www.52xcode.cn/Article/details/gt2ljzfplqi.html

[U28] Py：类型别名
来源：http://www.ydjk.org.cn/Article/details/gt2oodtjlbq.html

UserId = int
来源：http://www.ydjk.org.cn/Article/details/gt2gdzxwqzr.html

[U29] Py：属性校验
来源：http://www.52xcode.cn/Article/details/gt2cjloswke.html

@property 与 @x.setter 配合
来源：http://www.52xcode.cn/Article/details/gt2vdhkhknt.html

[U30] Py：数据类
来源：http://www.52xcode.cn/Article/details/gt2mdbdkkav.html

@dataclass(slots=True)
来源：http://www.52xcode.cn/Article/details/gt2qytrxzjv.html

[U31] Py：单测
来源：http://www.52xcode.cn/Article/details/gt2qusakkgj.html

python -m pytest -q
来源：http://www.ydjk.org.cn/Article/details/gt2hfeqlmie.html

[U32] Py：代码格式化
来源：http://www.ydjk.org.cn/Article/details/gt2yygdvlxn.html

ruff format . && ruff check --fix .
来源：http://www.52xcode.cn/Article/details/gt2alcznqsq.html

[U33] Py：打包发布
来源：http://www.52xcode.cn/Article/details/gt2cdbcbldm.html

python -m build  （依赖 pyproject.toml）
来源：http://www.ydjk.org.cn/Article/details/gt2kwnbkmnh.html

[U34] Py：判断编码
来源：http://www.ydjk.org.cn/Article/details/gt2hazyyigu.html

chardet.detect(raw)
来源：http://www.ydjk.org.cn/Article/details/gt2tnmglsvu.html

[U35] Py：发送邮件
来源：http://www.52xcode.cn/Article/details/gt2erstjlqv.html

smtplib.SMTP_SSL(...).send_message(msg)
来源：http://www.52xcode.cn/Article/details/gt2dowpzelv.html

[U36] Py：定时任务
来源：http://www.52xcode.cn/Article/details/gt2jbelmpbv.html

schedule.every(10).minutes.do(job)
来源：http://www.ydjk.org.cn/Article/details/gt2xjvxbyof.html

[U37] Py：读写 Excel
来源：http://www.ydjk.org.cn/Article/details/gt2fpuybqjp.html

pandas.read_excel / DataFrame.to_excel
来源：http://www.ydjk.org.cn/Article/details/gt2ijsydvvt.html

[U38] Py：获取脚本所在目录
来源：http://www.52xcode.cn/Article/details/gt2daewvikn.html

Path(__file__).resolve().parent
来源：http://www.52xcode.cn/Article/details/gt2iyqxmjyl.html

[U39] Py：判断是否在交互环境
来源：http://www.ydjk.org.cn/Article/details/gt2knqgtrte.html

sys.stdout.isatty()
来源：http://www.52xcode.cn/Article/details/gt2gvpgpibw.html

[U40] Py：打印到标准错误
来源：http://www.52xcode.cn/Article/details/gt2pxshdqag.html

print("err", file=sys.stderr)
来源：http://www.ydjk.org.cn/Article/details/gt2snxqsqmk.html

[U41] PHP：初始化 Composer 项目
来源：http://www.52xcode.cn/Article/details/gt2pbrewjtf.html

composer init;  composer require guzzlehttp/guzzle
来源：http://www.ydjk.org.cn/Article/details/gt2ssnaesfy.html

[U42] PHP：PSR-4 自动加载
来源：http://www.ydjk.org.cn/Article/details/gt2sdjobshl.html

"autoload": { "psr-4": { "App\\": "src/" } }
来源：http://www.ydjk.org.cn/Article/details/gt2dqvoeido.html

[U43] PHP：声明命名空间
来源：http://www.52xcode.cn/Article/details/gt2xkvzdrvp.html

namespace App\Http;
来源：http://www.52xcode.cn/Article/details/gt2lfxnuddg.html

[U44] PHP：开启严格类型
来源：http://www.ydjk.org.cn/Article/details/gt2spkwylan.html

declare(strict_types=1);
来源：http://www.ydjk.org.cn/Article/details/gt2kihlhgcn.html

[U45] PHP：类型声明与返回类型
来源：http://www.ydjk.org.cn/Article/details/gt2gvdrwxnx.html

function add(int $a, int $b): int { return $a + $b; }
来源：http://www.52xcode.cn/Article/details/gt2jjysnjpy.html

[U46] PHP：可空类型
来源：http://www.52xcode.cn/Article/details/gt2ditzmouf.html

?string $name = null
来源：http://www.52xcode.cn/Article/details/gt2furfzujf.html

[U47] PHP：联合类型
来源：http://www.52xcode.cn/Article/details/gt2xkulzdkj.html

int|string $id
来源：http://www.ydjk.org.cn/Article/details/gt2dmtxjckl.html

[U48] PHP：纯枚举
来源：http://www.ydjk.org.cn/Article/details/gt2uameuprp.html

enum Status: string { case Active = "active"; case Off = "off"; }
来源：http://www.52xcode.cn/Article/details/gt2xrdrmbvd.html

[U49] PHP：只读属性
来源：http://www.ydjk.org.cn/Article/details/gt2tyhdkbwg.html

public readonly string $name
来源：http://www.52xcode.cn/Article/details/gt2ujyzcyyf.html

[U50] PHP：构造器属性提升
来源：http://www.ydjk.org.cn/Article/details/gt2nzbktkna.html

public function __construct(private int $id) {}
来源：http://www.52xcode.cn/Article/details/gt2vvlcfwgd.html

[U51] PHP：数组解构
来源：http://www.ydjk.org.cn/Article/details/gt2iwftssew.html

[$a, $b] = $arr;
来源：http://www.ydjk.org.cn/Article/details/gt2ynofoubh.html

[U52] PHP：箭头函数
来源：http://www.52xcode.cn/Article/details/gt2pvijijly.html

$double = fn($x) => $x * 2;
来源：http://www.ydjk.org.cn/Article/details/gt2qorslqey.html

[U53] PHP：空合并运算符
来源：http://www.ydjk.org.cn/Article/details/gt2dtwgevuf.html

$v = $a ?? $b ?? "default";
来源：http://www.ydjk.org.cn/Article/details/gt2buagywoi.html

[U54] PHP：空安全调用
来源：http://www.52xcode.cn/Article/details/gt2tbhkoazd.html

$obj?->method()
来源：http://www.ydjk.org.cn/Article/details/gt2abgsadeo.html

[U55] PHP：match 表达式
来源：http://www.ydjk.org.cn/Article/details/gt2dtycbzxn.html

$s = match($x) { 1 => "一", default => "其他" };
来源：http://www.52xcode.cn/Article/details/gt2fhpbknjf.html

[U56] PHP：命名参数
来源：http://www.ydjk.org.cn/Article/details/gt2pihwwhlz.html

f(a: 1, b: 2)
来源：http://www.ydjk.org.cn/Article/details/gt2zslsdkgr.html

[U57] PHP：字符串插值
来源：http://www.52xcode.cn/Article/details/gt2aejorceu.html

"值: {$a}"
来源：http://www.ydjk.org.cn/Article/details/gt2imtmbfga.html

[U58] PHP：数组三件套
来源：http://www.ydjk.org.cn/Article/details/gt2mmqbqoel.html

array_map($f, $a);  array_filter($a, $f);  array_reduce($a, $f, 0);
来源：http://www.ydjk.org.cn/Article/details/gt2zetqpxoq.html

[U59] PHP：自定义排序
来源：http://www.52xcode.cn/Article/details/gt2zfuelxra.html

usort($arr, fn($a, $b) => $a["age"] <=> $b["age"]);
来源：http://www.ydjk.org.cn/Article/details/gt2xgukvuvt.html

[U60] PHP：JSON 编解码
来源：http://www.52xcode.cn/Article/details/gt2leuldfnu.html

json_encode($d, JSON_UNESCAPED_UNICODE);  json_decode($s, true);
来源：http://www.52xcode.cn/Article/details/gt2rujztsnt.html

[U61] PHP：正则
来源：http://www.ydjk.org.cn/Article/details/gt2ivwcskcg.html

preg_match('/(\d+)/', $s, $m);  preg_replace('/\d+/', '#', $s);
来源：http://www.52xcode.cn/Article/details/gt2foxgdnfy.html

[U62] PHP：日期对象
来源：http://www.ydjk.org.cn/Article/details/gt2fyjwrqaj.html

(new DateTimeImmutable())->format("Y-m-d");
来源：http://www.52xcode.cn/Article/details/gt2xykfincf.html

[U63] PHP：文件读写
来源：http://www.52xcode.cn/Article/details/gt2jaqphhts.html

file_get_contents($f);  file_put_contents($f, $data);
来源：http://www.ydjk.org.cn/Article/details/gt2lgyolvwx.html

[U64] PHP：目录遍历
来源：http://www.52xcode.cn/Article/details/gt2paasqlqv.html

glob("dir/*.php");  scandir("dir");
来源：http://www.52xcode.cn/Article/details/gt2gzmglvnq.html

[U65] PHP：会话
来源：http://www.52xcode.cn/Article/details/gt2cntmjtgx.html

session_start();  $_SESSION["uid"] = 1;
来源：http://www.ydjk.org.cn/Article/details/gt2jqcknjvh.html

[U66] PHP：设置 Cookie
来源：http://www.ydjk.org.cn/Article/details/gt2msisugfq.html

setcookie("token", $v, ["httponly" => true, "samesite" => "Lax"]);
来源：http://www.52xcode.cn/Article/details/gt2uitondyh.html

[U67] PHP：处理文件上传
来源：http://www.ydjk.org.cn/Article/details/gt2jvculfjh.html

$_FILES["file"]["tmp_name"] 与 move_uploaded_file()
来源：http://www.52xcode.cn/Article/details/gt2bmiccpkf.html

[U68] PHP：PDO 连接
来源：http://www.ydjk.org.cn/Article/details/gt2wyvxnopi.html

$pdo = new PDO("mysql:host=localhost;dbname=app", "root", "");
来源：http://www.52xcode.cn/Article/details/gt2sjmdllaw.html

[U69] PHP：PDO 预处理
来源：http://www.ydjk.org.cn/Article/details/gt2dzapxpfn.html

$stmt = $pdo->prepare("SELECT * FROM users WHERE id = ?");  $stmt->execute([$id]);
来源：http://www.52xcode.cn/Article/details/gt2vpfdsmce.html

[U70] PHP：PDO 事务
来源：http://www.52xcode.cn/Article/details/gt2dstngpct.html

$pdo->beginTransaction();  $pdo->commit();  $pdo->rollBack();
来源：http://www.ydjk.org.cn/Article/details/gt2pzmmwrlr.html

[U71] PHP：抛出异常
来源：http://www.52xcode.cn/Article/details/gt2zmxuhlax.html

throw new RuntimeException("失败", 500);
来源：http://www.ydjk.org.cn/Article/details/gt2xxtfkfho.html

[U72] PHP：写错误日志
来源：http://www.52xcode.cn/Article/details/gt2yfabnihx.html

error_log("失败: " . $e->getMessage());
来源：http://www.52xcode.cn/Article/details/gt2uonfnkqf.html

[U73] PHP：读取 ini 配置
来源：http://www.ydjk.org.cn/Article/details/gt2ppephvhv.html

parse_ini_file("config.ini", true)
来源：http://www.52xcode.cn/Article/details/gt2rtpwjntt.html

[U74] PHP：读取环境变量
来源：http://www.52xcode.cn/Article/details/gt2arrcokax.html

getenv("APP_ENV") ?: "production"
来源：http://www.ydjk.org.cn/Article/details/gt2vexkgvrt.html

[U75] PHP：依赖注入
来源：http://www.ydjk.org.cn/Article/details/gt2soegqbcv.html

composer require psr/container
来源：http://www.52xcode.cn/Article/details/gt2qxnxsyhu.html

[U76] PHP：简单路由
来源：http://www.52xcode.cn/Article/details/gt2ccypcbom.html

$path = parse_url($_SERVER["REQUEST_URI"], PHP_URL_PATH);
来源：http://www.52xcode.cn/Article/details/gt2vsjcnoca.html

[U77] PHP：模板渲染
来源：http://www.ydjk.org.cn/Article/details/gt2qqxiafxv.html

composer require twig/twig
来源：http://www.52xcode.cn/Article/details/gt2falrcjxu.html

[U78] PHP：单元测试
来源：http://www.52xcode.cn/Article/details/gt2phpeulwk.html

composer require --dev phpunit/phpunit
来源：http://www.52xcode.cn/Article/details/gt2ccwmdcun.html

[U79] PHP：静态分析
来源：http://www.52xcode.cn/Article/details/gt2mypudgqi.html

composer require --dev phpstan/phpstan
来源：http://www.52xcode.cn/Article/details/gt2olgnuimk.html

[U80] PHP：代码规范修复
来源：http://www.ydjk.org.cn/Article/details/gt2ojsikijc.html

composer require --dev friendsofphp/php-cs-fixer
来源：http://www.ydjk.org.cn/Article/details/gt2ijwqdgid.html

[U81] JS：初始化项目
来源：http://www.ydjk.org.cn/Article/details/gt2vuqotsma.html

npm init -y;  npm i express
来源：http://www.ydjk.org.cn/Article/details/gt2xgqtdfni.html

[U82] JS：package.json 脚本
来源：http://www.ydjk.org.cn/Article/details/gt2ekkjuaix.html

"scripts": { "dev": "vite", "build": "vite build" }
来源：http://www.52xcode.cn/Article/details/gt2natmozkz.html

[U83] JS：ES Module 导入导出
来源：http://www.ydjk.org.cn/Article/details/gt2oaqkaqqj.html

export const a = 1;  import { a } from "./m.js";
来源：http://www.ydjk.org.cn/Article/details/gt2cipbaopr.html

[U84] JS：CommonJS 写法
来源：http://www.52xcode.cn/Article/details/gt2fgipqwqq.html

module.exports = { a };  const { a } = require("./m");
来源：http://www.52xcode.cn/Article/details/gt2ujfjorvs.html

[U85] JS：可选链
来源：http://www.ydjk.org.cn/Article/details/gt2npksfcmc.html

a?.b?.c
来源：http://www.ydjk.org.cn/Article/details/gt2bisihdms.html

[U86] JS：空值合并
来源：http://www.ydjk.org.cn/Article/details/gt2fuxwynsg.html

a ?? b
来源：http://www.52xcode.cn/Article/details/gt2xrmlpdum.html

[U87] JS：解构默认值
来源：http://www.ydjk.org.cn/Article/details/gt2qrblkqxs.html

const { a = 1, b = 2 } = obj;
来源：http://www.52xcode.cn/Article/details/gt2hjvhxmdv.html

[U88] JS：对象展开合并
来源：http://www.52xcode.cn/Article/details/gt2jatdmofi.html

{ ...a, ...b }
来源：http://www.52xcode.cn/Article/details/gt2keahnqki.html

[U89] JS：数组去重
来源：http://www.52xcode.cn/Article/details/gt2jqbczgvg.html

[...new Set(arr)]
来源：http://www.52xcode.cn/Article/details/gt2gtevfdxe.html

[U90] JS：数字数组排序
来源：http://www.ydjk.org.cn/Article/details/gt2abgawbji.html

[...arr].sort((a, b) => a - b)
来源：http://www.52xcode.cn/Article/details/gt2cnuegfnl.html

[U91] JS：对象键值遍历
来源：http://www.52xcode.cn/Article/details/gt2hqkwmkqr.html

Object.entries(obj).forEach(([k, v]) => {});
来源：http://www.ydjk.org.cn/Article/details/gt2xwusruhr.html

[U92] JS：深拷贝
来源：http://www.ydjk.org.cn/Article/details/gt2bscvskyv.html

structuredClone(obj)
来源：http://www.ydjk.org.cn/Article/details/gt2kkhznutm.html

[U93] JS：模板字符串
来源：http://www.52xcode.cn/Article/details/gt2qyiuzwat.html

`共 ${n} 条`
来源：http://www.ydjk.org.cn/Article/details/gt2iwrmfwnp.html

[U94] JS：箭头函数
来源：http://www.ydjk.org.cn/Article/details/gt2koejgaet.html

const double = x => x * 2;
来源：http://www.52xcode.cn/Article/details/gt2xqrxldkb.html

[U95] JS：Promise 包装
来源：http://www.ydjk.org.cn/Article/details/gt2kqppeuwd.html

new Promise((resolve, reject) => {})
来源：http://www.52xcode.cn/Article/details/gt2qplntvav.html

[U96] JS：async/await 与异常
来源：http://www.ydjk.org.cn/Article/details/gt2ujhqzmwt.html

try { const d = await f(); } catch (e) { console.error(e); }
来源：http://www.52xcode.cn/Article/details/gt2bhsovmyh.html

[U97] JS：并发请求
来源：http://www.ydjk.org.cn/Article/details/gt2wfsjyytb.html

await Promise.all(urls.map(u => fetch(u)))
来源：http://www.ydjk.org.cn/Article/details/gt2ubvmlfcg.html

[U98] JS：fetch 带 JSON
来源：http://www.ydjk.org.cn/Article/details/gt2oefmmesz.html

await fetch(url, { method: "POST", headers: { "Content-Type": "application/json" }, body: JSON.stringify(d) })
来源：http://www.52xcode.cn/Article/details/gt2jjfnxlqa.html

[U99] JS：事件监听
来源：http://www.52xcode.cn/Article/details/gt2dxfhbinc.html

el.addEventListener("click", e => {})
来源：http://www.52xcode.cn/Article/details/gt2fcabrorw.html

[U100] JS：DOM 查询
来源：http://www.ydjk.org.cn/Article/details/gt2aqrnoozr.html

document.querySelector(".item")
来源：http://www.52xcode.cn/Article/details/gt2gjzpupfa.html

[U101] JS：classList 操作
来源：http://www.ydjk.org.cn/Article/details/gt2qikogqog.html

el.classList.toggle("active")
来源：http://www.ydjk.org.cn/Article/details/gt2ppmgiluz.html

[U102] JS：本地存储
来源：http://www.52xcode.cn/Article/details/gt2yoovxzws.html

localStorage.setItem("k", JSON.stringify(v))
来源：http://www.52xcode.cn/Article/details/gt2dslbwgym.html

[U103] JS：定时器
来源：http://www.52xcode.cn/Article/details/gt2mnmrlgzi.html

setTimeout(fn, 1000);  setInterval(fn, 1000);
来源：http://www.52xcode.cn/Article/details/gt2bbdiqtxc.html

[U104] JS：防抖
来源：http://www.ydjk.org.cn/Article/details/gt2jesttmnp.html

const debounce = (fn, ms) => { let t; return (...a) => { clearTimeout(t); t = setTimeout(() => fn(...a), ms); }; };
来源：http://www.52xcode.cn/Article/details/gt2plwolkrm.html

[U105] JS：节流
来源：http://www.ydjk.org.cn/Article/details/gt2hupwptoo.html

const throttle = (fn, ms) => { let last = 0; return (...a) => { const n = Date.now(); if (n - last >= ms) { last = n; fn(...a); } }; };
来源：http://www.52xcode.cn/Article/details/gt2fhrmjzka.html

[U106] JS：日期格式化
来源：http://www.ydjk.org.cn/Article/details/gt2oycvunjc.html

new Intl.DateTimeFormat("zh-CN", { dateStyle: "medium" }).format(new Date())
来源：http://www.ydjk.org.cn/Article/details/gt2cxenkpui.html

[U107] JS：数字千分位
来源：http://www.52xcode.cn/Article/details/gt2qjkioixa.html

new Intl.NumberFormat("en-US").format(1234567)
来源：http://www.ydjk.org.cn/Article/details/gt2xtwhvvpx.html

[U108] JS：随机整数
来源：http://www.ydjk.org.cn/Article/details/gt2bnaltvvg.html

Math.floor(Math.random() * (max - min + 1)) + min
来源：http://www.ydjk.org.cn/Article/details/gt2rjwcsqlc.html

[U109] JS：数组分组
来源：http://www.ydjk.org.cn/Article/details/gt2uuzjltnk.html

Object.groupBy(arr, x => x.type)
来源：http://www.ydjk.org.cn/Article/details/gt2ytjqqaih.html

[U110] JS：数组分块
来源：http://www.52xcode.cn/Article/details/gt2kzxkwwae.html

arr.reduce((acc, x, i) => (i % size ? acc : [...acc, arr.slice(i, i + size)]), [])
来源：http://www.ydjk.org.cn/Article/details/gt2wibnpmpz.html

[U111] JS：对象转 Map
来源：http://www.ydjk.org.cn/Article/details/gt2mhtjewbk.html

new Map(Object.entries(obj))
来源：http://www.ydjk.org.cn/Article/details/gt2bomxoigu.html

[U112] JS：字符串补位
来源：http://www.ydjk.org.cn/Article/details/gt2mzlamiwj.html

"7".padStart(3, "0")
来源：http://www.ydjk.org.cn/Article/details/gt2vqsvpshf.html

[U113] JS：正则替换全部
来源：http://www.52xcode.cn/Article/details/gt2yxrlofdm.html

s.replaceAll("a", "b")
来源：http://www.52xcode.cn/Article/details/gt2jbelcsrp.html

[U114] JS：JSON 深比较
来源：http://www.52xcode.cn/Article/details/gt2jfwkqlyq.html

JSON.stringify(a) === JSON.stringify(b)
来源：http://www.52xcode.cn/Article/details/gt2qcaddcgx.html

[U115] JS：生成 UUID
来源：http://www.52xcode.cn/Article/details/gt2paoyprla.html

crypto.randomUUID()
来源：http://www.ydjk.org.cn/Article/details/gt2vdqqoipd.html

[U116] JS：类型检查（JSDoc）
来源：http://www.ydjk.org.cn/Article/details/gt2tjeyvnyv.html

/** @param {string} name */ function f(name) {}
来源：http://www.ydjk.org.cn/Article/details/gt2ghrniwub.html

[U117] JS：单元测试
来源：http://www.ydjk.org.cn/Article/details/gt2fhkhwugh.html

npm i -D vitest;  npx vitest
来源：http://www.52xcode.cn/Article/details/gt2yvdvxspk.html

[U118] JS：开发服务器
来源：http://www.52xcode.cn/Article/details/gt2tmdfprqz.html

npm i -D vite;  npx vite
来源：http://www.ydjk.org.cn/Article/details/gt2zjomaawp.html

[U119] JS：生产构建
来源：http://www.52xcode.cn/Article/details/gt2nsquaiff.html

npx vite build
来源：http://www.52xcode.cn/Article/details/gt2zdrggyhd.html

[U120] JS：读取环境变量（Vite）
来源：http://www.ydjk.org.cn/Article/details/gt2ylgylhmt.html

import.meta.env.VITE_API_URL
来源：http://www.52xcode.cn/Article/details/gt2ktfbockz.html

================================================================================
来源：http://www.52xcode.cn/Article/details/gt2hkctdlzn.html

统计汇总
来源：http://www.ydjk.org.cn/Article/details/gt2sqkztypu.html

================================================================================
来源：http://www.ydjk.org.cn/Article/details/gt2iipxwdsd.html

按语言统计（条）：
来源：http://www.ydjk.org.cn/Article/details/gt2vwdtuxwe.html

Python ......... 252
来源：http://www.ydjk.org.cn/Article/details/gt2wzrzcnrf.html

PHP ............ 252
来源：http://www.52xcode.cn/Article/details/gt2pslhgnrh.html

JavaScript ..... 252
来源：http://www.ydjk.org.cn/Article/details/gt2tubkcwsy.html

TypeScript ..... 212
来源：http://www.52xcode.cn/Article/details/gt2pjqbybta.html

Java ........... 212
来源：http://www.52xcode.cn/Article/details/gt2pwdbrpxp.html

Go ............. 212
来源：http://www.52xcode.cn/Article/details/gt2karregrh.html

Ruby ........... 212
来源：http://www.ydjk.org.cn/Article/details/gt2ruyqtmoq.html

C# ............. 212
来源：http://www.ydjk.org.cn/Article/details/gt2ohwccuya.html

C .............. 30
来源：http://www.ydjk.org.cn/Article/details/gt2qxoyvghn.html

C++ ............ 30
来源：http://www.ydjk.org.cn/Article/details/gt2woupiavt.html

SQL ............ 90
来源：http://www.52xcode.cn/Article/details/gt2qkvwimlt.html

Bash ........... 80
来源：http://www.ydjk.org.cn/Article/details/gt2dttydkfn.html

Kotlin ......... 15
来源：http://www.52xcode.cn/Article/details/gt2chtnajae.html

Swift .......... 15
来源：http://www.52xcode.cn/Article/details/gt2zehvcdfc.html

Lua ............ 10
来源：http://www.ydjk.org.cn/Article/details/gt2idzbvifc.html

Perl ........... 10
来源：http://www.ydjk.org.cn/Article/details/gt2gizulynw.html

Scala .......... 10
来源：http://www.ydjk.org.cn/Article/details/gt2tqflucxq.html

------------------------------------
来源：http://www.ydjk.org.cn/Article/details/gt2ilgvhwde.html

合计 ........... 2106 条
来源：http://www.ydjk.org.cn/Article/details/gt2popnwffe.html

按章节统计：
来源：http://www.52xcode.cn/Article/details/gt2nlapjmhy.html

A 基础语法与类型       26 个任务 × 8 语言 =  208
来源：http://www.52xcode.cn/Article/details/gt2znxyozci.html

B 流程控制             16 个任务 × 8 语言 =  128
来源：http://www.52xcode.cn/Article/details/gt2mxgoeaow.html

C 函数与作用域         16 个任务 × 8 语言 =  128
来源：http://www.ydjk.org.cn/Article/details/gt2cxorwkrl.html

D 数组 / 列表 / 集合   26 个任务 × 8 语言 =  208
来源：http://www.52xcode.cn/Article/details/gt2utlrpeni.html

E 字符串处理           22 个任务 × 8 语言 =  176
来源：http://www.52xcode.cn/Article/details/gt2vgzsbimc.html

F 文件与目录           12 个任务 × 8 语言 =   96
来源：http://www.52xcode.cn/Article/details/gt2vgsadvug.html

G 面向对象             16 个任务 × 8 语言 =  128
来源：http://www.52xcode.cn/Article/details/gt2gsdnwqae.html

H 异常与错误处理       10 个任务 × 8 语言 =   80
来源：http://www.ydjk.org.cn/Article/details/gt2riupvdau.html

I 正则表达式            8 个任务 × 8 语言 =   64
来源：http://www.ydjk.org.cn/Article/details/gt2ncxkaage.html

J 日期与时间           10 个任务 × 8 语言 =   80
来源：http://www.52xcode.cn/Article/details/gt2jxnseoov.html

K JSON 与序列化         8 个任务 × 8 语言 =   64
来源：http://www.52xcode.cn/Article/details/gt2ttstbgvb.html

L 网络请求              8 个任务 × 8 语言 =   64
来源：http://www.ydjk.org.cn/Article/details/gt2imaahptp.html

M 命令行 / 进程         8 个任务 × 8 语言 =   64
来源：http://www.52xcode.cn/Article/details/gt2srlgickd.html

N 数据结构与算法       12 个任务 × 8 语言 =   96
来源：http://www.52xcode.cn/Article/details/gt2ajswoavw.html

O 并发与异步            6 个任务 × 8 语言 =   48
来源：http://www.ydjk.org.cn/Article/details/gt2bqslbqks.html

P 常用工具函数          8 个任务 × 8 语言 =   64
来源：http://www.ydjk.org.cn/Article/details/gt2dxsvoksn.html

Q SQL 专题                              90
来源：http://www.ydjk.org.cn/Article/details/gt2eughdxlo.html

R Bash 专题                             80
来源：http://www.ydjk.org.cn/Article/details/gt2rvbyhkac.html

S C / C++ 专题                          60
来源：http://www.52xcode.cn/Article/details/gt2wrpwnxgs.html

T 其他语言补充                          60
来源：http://www.52xcode.cn/Article/details/gt2nfigjlfd.html

U 高频实用片段                         120
来源：http://www.52xcode.cn/Article/details/gt2ohczqqei.html

------------------------------------
来源：http://www.52xcode.cn/Article/details/gt2nwdomtoy.html

合计                                  2106 条
来源：http://www.52xcode.cn/Article/details/gt2uenyromb.html

--------------------------------------------------------------------------------
来源：http://www.52xcode.cn/Article/details/gt2pgxpqkea.html

使用提醒
来源：http://www.52xcode.cn/Article/details/gt2bneowbho.html

--------------------------------------------------------------------------------
来源：http://www.ydjk.org.cn/Article/details/gt2nbpiaqqc.html

1. 示例追求"最小可用"，正式项目中请补齐导入、错误处理与边界判断。
来源：http://www.52xcode.cn/Article/details/gt2hozsqati.html

2. 涉及文件、网络、数据库的示例，注意资源释放与异常捕获。
来源：http://www.52xcode.cn/Article/details/gt2yhxbqpac.html

3. 语言版本差异较大（如 Python 3.10 的 match、Java 17 的 record/switch 箭头），
来源：http://www.ydjk.org.cn/Article/details/gt2sioldjnu.html

在旧版本上使用前请先确认语法支持情况。
来源：http://www.ydjk.org.cn/Article/details/gt2ngsypfzc.html

4. 标注"手写"的条目是因为该语言缺少对应内置能力，实际项目中可引入成熟库。
来源：http://www.52xcode.cn/Article/details/gt2ujceedjn.html

—— 文件结束 ——
来源：http://www.ydjk.org.cn/Article/details/gt2laymrlga.html


<!-- 参考信息 -->