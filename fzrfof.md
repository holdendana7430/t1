代发 wailian999

def add(a: Int, b: Int): Int = a + b
来源：http://www.52xcode.cn/Article/details/gt2kxlmmbxb.html

[T59] Scala：循环
来源：http://www.52xcode.cn/Article/details/gt2ioejwwxr.html

for (i <- 1 to 10) println(i)
来源：http://www.52xcode.cn/Article/details/gt2nslkpqbo.html

[T60] Scala：折叠
来源：http://www.52xcode.cn/Article/details/gt2pgvtepsi.html

List(1, 2, 3).foldLeft(0)(_ + _)
来源：http://www.52xcode.cn/Article/details/gt2uvduvftx.html

================================================================================
来源：http://www.52xcode.cn/Article/details/gt2creljbwz.html

U. 高频实用片段（Python / PHP / JavaScript 各 40 条）
来源：http://www.52xcode.cn/Article/details/gt2xtnzxpvz.html

================================================================================
来源：http://www.52xcode.cn/Article/details/gt2mhspcprs.html

[U01] Py：创建虚拟环境
来源：http://www.52xcode.cn/Article/details/gt2ukuejepw.html

python -m venv .venv && source .venv/bin/activate
来源：http://www.ydjk.org.cn/Article/details/gt2wgonilgs.html

[U02] Py：导出 / 安装依赖
来源：http://www.ydjk.org.cn/Article/details/gt2mjlwbpru.html

pip freeze > requirements.txt;  pip install -r requirements.txt
来源：http://www.ydjk.org.cn/Article/details/gt2gdgipwsd.html

[U03] Py：加载 .env 配置
来源：http://www.ydjk.org.cn/Article/details/gt2mmeusdjf.html

from dotenv import load_dotenv; load_dotenv()
来源：http://www.52xcode.cn/Article/details/gt2jpduqiot.html

[U04] Py：变量调试打印
来源：http://www.52xcode.cn/Article/details/gt2dpwuuval.html

print(f"{x=}")            # 输出 x=值，Python 3.8+
来源：http://www.ydjk.org.cn/Article/details/gt2xyxhmpnx.html

[U05] Py：列表去重且保序
来源：http://www.ydjk.org.cn/Article/details/gt2edbkgnfl.html

list(dict.fromkeys(arr))
来源：http://www.ydjk.org.cn/Article/details/gt2txvslrof.html

[U06] Py：合并两个字典
来源：http://www.52xcode.cn/Article/details/gt2vewqzyyj.html

{**a, **b}
来源：http://www.52xcode.cn/Article/details/gt2dwpcfksg.html

[U07] Py：反转字典键值
来源：http://www.52xcode.cn/Article/details/gt2tiholgdv.html

{v: k for k, v in d.items()}
来源：http://www.52xcode.cn/Article/details/gt2ywqtgwtx.html

[U08] Py：展平二维列表
来源：http://www.52xcode.cn/Article/details/gt2jjrkfsmj.html

[y for x in nested for y in x]
来源：http://www.52xcode.cn/Article/details/gt2pmtvrtnq.html

[U09] Py：字典取最大值的键
来源：http://www.52xcode.cn/Article/details/gt2ixqnyhxo.html

max(d, key=d.get)
来源：http://www.52xcode.cn/Article/details/gt2vawtvbmn.html

[U10] Py：按值排序字典
来源：http://www.52xcode.cn/Article/details/gt2ljtghemr.html

dict(sorted(d.items(), key=lambda kv: kv[1]))
来源：http://www.52xcode.cn/Article/details/gt2apwhsifi.html

[U11] Py：生成器表达式
来源：http://www.ydjk.org.cn/Article/details/gt2fymqktrx.html

(x * 2 for x in arr)
来源：http://www.52xcode.cn/Article/details/gt2dqaiefmi.html

[U12] Py：取出现最多的 3 个元素
来源：http://www.52xcode.cn/Article/details/gt2zbbdrjpo.html

Counter(arr).most_common(3)
来源：http://www.ydjk.org.cn/Article/details/gt2rjknoddz.html

[U13] Py：固定长度队列
来源：http://www.52xcode.cn/Article/details/gt2lxlpwvhv.html

deque(maxlen=10)
来源：http://www.ydjk.org.cn/Article/details/gt2meibclnj.html

[U14] Py：分组收集到列表
来源：http://www.52xcode.cn/Article/details/gt2elhxzdpu.html

defaultdict(list)
来源：http://www.ydjk.org.cn/Article/details/gt2qqmvgooc.html

[U15] Py：高精度计时
来源：http://www.52xcode.cn/Article/details/gt2cwmbmmsy.html

t = time.perf_counter()
来源：http://www.ydjk.org.cn/Article/details/gt2iqyrmjpb.html

[U16] Py：命令行参数解析
来源：http://www.52xcode.cn/Article/details/gt2sebuztbk.html

ap = argparse.ArgumentParser();  ap.add_argument("--name");  args = ap.parse_args()
来源：http://www.ydjk.org.cn/Article/details/gt2fuudugma.html

[U17] Py：初始化日志
来源：http://www.52xcode.cn/Article/details/gt2yjzykifb.html

logging.basicConfig(level=logging.INFO)
来源：http://www.52xcode.cn/Article/details/gt2fptogizj.html

[U18] Py：预编译正则
来源：http://www.ydjk.org.cn/Article/details/gt2wbhulzfr.html

pat = re.compile(r"\d+")
来源：http://www.52xcode.cn/Article/details/gt2putghifp.html

[U19] Py：正则替换带回调
来源：http://www.ydjk.org.cn/Article/details/gt2ybtaajhi.html

re.sub(r"\d+", lambda m: str(int(m.group()) * 2), s)
来源：http://www.ydjk.org.cn/Article/details/gt2gxdzwims.html

[U20] Py：缓存函数结果
来源：http://www.52xcode.cn/Article/details/gt2vvfmkxds.html

@functools.lru_cache(maxsize=None)
来源：http://www.ydjk.org.cn/Article/details/gt2cfewbicq.html

[U21] Py：自定义上下文管理器
来源：http://www.ydjk.org.cn/Article/details/gt2hywkhmsq.html

@contextlib.contextmanager
来源：http://www.ydjk.org.cn/Article/details/gt2gibfzefm.html

[U22] Py：矩阵转置
来源：http://www.ydjk.org.cn/Article/details/gt2ajlmclmw.html

list(zip(*m))
来源：http://www.52xcode.cn/Article/details/gt2yzlxynvt.html

[U23] Py：分块读取大文件
来源：http://www.52xcode.cn/Article/details/gt2ccghtabl.html

for chunk in iter(lambda: f.read(8192), b""):
来源：http://www.52xcode.cn/Article/details/gt2rzpsczhu.html

[U24] Py：路径操作
来源：http://www.ydjk.org.cn/Article/details/gt2agnzehil.html

Path("a/b.txt").parent.mkdir(parents=True, exist_ok=True)
来源：http://www.ydjk.org.cn/Article/details/gt2rjxctwgy.html

[U25] Py：CSV 按字典读
来源：http://www.52xcode.cn/Article/details/gt2domjxstr.html

csv.DictReader(f)
来源：http://www.ydjk.org.cn/Article/details/gt2bkplvunb.html

[U26] Py：并发下载
来源：http://www.52xcode.cn/Article/details/gt2nxapjlsd.html

ThreadPoolExecutor(max_workers=8).map(fetch, urls)
来源：http://www.52xcode.cn/Article/details/gt2iwzsizaz.html

[U27] Py：异步 HTTP
来源：http://www.52xcode.cn/Article/details/gt2filolzqq.html

aiohttp.ClientSession() 配合 async with
来源：http://www.52xcode.cn/Article/details/gt2ppcrsgiy.html

[U28] Py：类型别名
来源：http://www.ydjk.org.cn/Article/details/gt2vmvwnfjk.html

UserId = int
来源：http://www.ydjk.org.cn/Article/details/gt2ygasqwiz.html

[U29] Py：属性校验
来源：http://www.ydjk.org.cn/Article/details/gt2rmenszjj.html

@property 与 @x.setter 配合
来源：http://www.ydjk.org.cn/Article/details/gt2eybjbgev.html

[U30] Py：数据类
来源：http://www.52xcode.cn/Article/details/gt2enybmpuw.html

@dataclass(slots=True)
来源：http://www.52xcode.cn/Article/details/gt2qsjtbqli.html

[U31] Py：单测
来源：http://www.52xcode.cn/Article/details/gt2mlbkudqi.html

python -m pytest -q
来源：http://www.52xcode.cn/Article/details/gt2rzqjxkqv.html

[U32] Py：代码格式化
来源：http://www.ydjk.org.cn/Article/details/gt2oeurexuz.html

ruff format . && ruff check --fix .
来源：http://www.ydjk.org.cn/Article/details/gt2jldojbkm.html

[U33] Py：打包发布
来源：http://www.52xcode.cn/Article/details/gt2dyraiydw.html

python -m build  （依赖 pyproject.toml）
来源：http://www.52xcode.cn/Article/details/gt2avvvctkk.html

[U34] Py：判断编码
来源：http://www.ydjk.org.cn/Article/details/gt2oikwtzaw.html

chardet.detect(raw)
来源：http://www.52xcode.cn/Article/details/gt2bgaaszwa.html

[U35] Py：发送邮件
来源：http://www.ydjk.org.cn/Article/details/gt2hvxdbojm.html

smtplib.SMTP_SSL(...).send_message(msg)
来源：http://www.ydjk.org.cn/Article/details/gt2orenozmq.html

[U36] Py：定时任务
来源：http://www.52xcode.cn/Article/details/gt2qndykuwg.html

schedule.every(10).minutes.do(job)
来源：http://www.ydjk.org.cn/Article/details/gt2ctzavqok.html

[U37] Py：读写 Excel
来源：http://www.ydjk.org.cn/Article/details/gt2vlmbgkpi.html

pandas.read_excel / DataFrame.to_excel
来源：http://www.ydjk.org.cn/Article/details/gt2qfnpvqla.html

[U38] Py：获取脚本所在目录
来源：http://www.ydjk.org.cn/Article/details/gt2thffsdfu.html

Path(__file__).resolve().parent
来源：http://www.52xcode.cn/Article/details/gt2nqbpracl.html

[U39] Py：判断是否在交互环境
来源：http://www.52xcode.cn/Article/details/gt2hlgxunyy.html

sys.stdout.isatty()
来源：http://www.52xcode.cn/Article/details/gt2ubpoawdp.html

[U40] Py：打印到标准错误
来源：http://www.52xcode.cn/Article/details/gt2yboepfkk.html

print("err", file=sys.stderr)
来源：http://www.52xcode.cn/Article/details/gt2byqaglhd.html

[U41] PHP：初始化 Composer 项目
来源：http://www.ydjk.org.cn/Article/details/gt2aypyaqqd.html

composer init;  composer require guzzlehttp/guzzle
来源：http://www.52xcode.cn/Article/details/gt2dvzzyons.html

[U42] PHP：PSR-4 自动加载
来源：http://www.52xcode.cn/Article/details/gt2mtrznvgn.html

"autoload": { "psr-4": { "App\\": "src/" } }
来源：http://www.52xcode.cn/Article/details/gt2ucoeffgg.html

[U43] PHP：声明命名空间
来源：http://www.52xcode.cn/Article/details/gt2jwzboynt.html

namespace App\Http;
来源：http://www.52xcode.cn/Article/details/gt2lkpvsyax.html

[U44] PHP：开启严格类型
来源：http://www.ydjk.org.cn/Article/details/gt2kxvnyeen.html

declare(strict_types=1);
来源：http://www.52xcode.cn/Article/details/gt2bggqolkv.html

[U45] PHP：类型声明与返回类型
来源：http://www.ydjk.org.cn/Article/details/gt2zyqyxdvh.html

function add(int $a, int $b): int { return $a + $b; }
来源：http://www.52xcode.cn/Article/details/gt2pyzjiqkl.html

[U46] PHP：可空类型
来源：http://www.52xcode.cn/Article/details/gt2vfxqjomk.html

?string $name = null
来源：http://www.ydjk.org.cn/Article/details/gt2rvmjgnds.html

[U47] PHP：联合类型
来源：http://www.ydjk.org.cn/Article/details/gt2grtwthuc.html

int|string $id
来源：http://www.52xcode.cn/Article/details/gt2wsmnjzbk.html

[U48] PHP：纯枚举
来源：http://www.52xcode.cn/Article/details/gt2wrtcnjka.html

enum Status: string { case Active = "active"; case Off = "off"; }
来源：http://www.52xcode.cn/Article/details/gt2zhifwzdz.html

[U49] PHP：只读属性
来源：http://www.52xcode.cn/Article/details/gt2jrxaadgz.html

public readonly string $name
来源：http://www.52xcode.cn/Article/details/gt2mrivnfrr.html

[U50] PHP：构造器属性提升
来源：http://www.52xcode.cn/Article/details/gt2mrseibyr.html

public function __construct(private int $id) {}
来源：http://www.52xcode.cn/Article/details/gt2ouncirhr.html

[U51] PHP：数组解构
来源：http://www.52xcode.cn/Article/details/gt2pskhmvlv.html

[$a, $b] = $arr;
来源：http://www.52xcode.cn/Article/details/gt2mmepftdf.html

[U52] PHP：箭头函数
来源：http://www.52xcode.cn/Article/details/gt2utxzllrh.html

$double = fn($x) => $x * 2;
来源：http://www.ydjk.org.cn/Article/details/gt2yndldtpq.html

[U53] PHP：空合并运算符
来源：http://www.52xcode.cn/Article/details/gt2vrkxnqkv.html

$v = $a ?? $b ?? "default";
来源：http://www.ydjk.org.cn/Article/details/gt2nfgjjrli.html

[U54] PHP：空安全调用
来源：http://www.52xcode.cn/Article/details/gt2nppfmjcv.html

$obj?->method()
来源：http://www.52xcode.cn/Article/details/gt2hwjkfzyh.html

[U55] PHP：match 表达式
来源：http://www.52xcode.cn/Article/details/gt2mfawzpru.html

$s = match($x) { 1 => "一", default => "其他" };
来源：http://www.ydjk.org.cn/Article/details/gt2oxexzbxh.html

[U56] PHP：命名参数
来源：http://www.52xcode.cn/Article/details/gt2kqwuhvpt.html

f(a: 1, b: 2)
来源：http://www.ydjk.org.cn/Article/details/gt2aoyjvmol.html

[U57] PHP：字符串插值
来源：http://www.52xcode.cn/Article/details/gt2efuzhnwn.html

"值: {$a}"
来源：http://www.ydjk.org.cn/Article/details/gt2mjdskjun.html

[U58] PHP：数组三件套
来源：http://www.ydjk.org.cn/Article/details/gt2tbtjwwdp.html

array_map($f, $a);  array_filter($a, $f);  array_reduce($a, $f, 0);
来源：http://www.52xcode.cn/Article/details/gt2yhahncsn.html

[U59] PHP：自定义排序
来源：http://www.ydjk.org.cn/Article/details/gt2slddffvi.html

usort($arr, fn($a, $b) => $a["age"] <=> $b["age"]);
来源：http://www.52xcode.cn/Article/details/gt2mclpebwe.html

[U60] PHP：JSON 编解码
来源：http://www.ydjk.org.cn/Article/details/gt2kuztezmo.html

json_encode($d, JSON_UNESCAPED_UNICODE);  json_decode($s, true);
来源：http://www.ydjk.org.cn/Article/details/gt2ouprwbbc.html

[U61] PHP：正则
来源：http://www.ydjk.org.cn/Article/details/gt2nscfeitk.html

preg_match('/(\d+)/', $s, $m);  preg_replace('/\d+/', '#', $s);
来源：http://www.52xcode.cn/Article/details/gt2pqbxmdlk.html

[U62] PHP：日期对象
来源：http://www.ydjk.org.cn/Article/details/gt2estlerqi.html

(new DateTimeImmutable())->format("Y-m-d");
来源：http://www.ydjk.org.cn/Article/details/gt2sotamojc.html

[U63] PHP：文件读写
来源：http://www.52xcode.cn/Article/details/gt2cxjvdcac.html

file_get_contents($f);  file_put_contents($f, $data);
来源：http://www.ydjk.org.cn/Article/details/gt2wjahbozn.html

[U64] PHP：目录遍历
来源：http://www.52xcode.cn/Article/details/gt2undwapox.html

glob("dir/*.php");  scandir("dir");
来源：http://www.ydjk.org.cn/Article/details/gt2llypxidi.html

[U65] PHP：会话
来源：http://www.52xcode.cn/Article/details/gt2xvxwxdvb.html

session_start();  $_SESSION["uid"] = 1;
来源：http://www.52xcode.cn/Article/details/gt2mrdhgqhc.html

[U66] PHP：设置 Cookie
来源：http://www.ydjk.org.cn/Article/details/gt2kanurzzc.html

setcookie("token", $v, ["httponly" => true, "samesite" => "Lax"]);
来源：http://www.ydjk.org.cn/Article/details/gt2quvevocn.html

[U67] PHP：处理文件上传
来源：http://www.ydjk.org.cn/Article/details/gt2rvmciaoa.html

$_FILES["file"]["tmp_name"] 与 move_uploaded_file()
来源：http://www.ydjk.org.cn/Article/details/gt2bppqabxd.html

[U68] PHP：PDO 连接
来源：http://www.ydjk.org.cn/Article/details/gt2dauhdiqv.html

$pdo = new PDO("mysql:host=localhost;dbname=app", "root", "");
来源：http://www.52xcode.cn/Article/details/gt2uzfdtdpp.html

[U69] PHP：PDO 预处理
来源：http://www.52xcode.cn/Article/details/gt2dnyybdws.html

$stmt = $pdo->prepare("SELECT * FROM users WHERE id = ?");  $stmt->execute([$id]);
来源：http://www.52xcode.cn/Article/details/gt2aprxrlwy.html

[U70] PHP：PDO 事务
来源：http://www.ydjk.org.cn/Article/details/gt2xohfeamz.html

$pdo->beginTransaction();  $pdo->commit();  $pdo->rollBack();
来源：http://www.ydjk.org.cn/Article/details/gt2gslvhqqn.html

[U71] PHP：抛出异常
来源：http://www.52xcode.cn/Article/details/gt2wabrcscj.html

throw new RuntimeException("失败", 500);
来源：http://www.52xcode.cn/Article/details/gt2isjcfqfw.html

[U72] PHP：写错误日志
来源：http://www.ydjk.org.cn/Article/details/gt2mhycftaa.html

error_log("失败: " . $e->getMessage());
来源：http://www.52xcode.cn/Article/details/gt2dnxqntrf.html

[U73] PHP：读取 ini 配置
来源：http://www.ydjk.org.cn/Article/details/gt2kifvmqbx.html

parse_ini_file("config.ini", true)
来源：http://www.52xcode.cn/Article/details/gt2kganrmkz.html

[U74] PHP：读取环境变量
来源：http://www.52xcode.cn/Article/details/gt2fnniqqie.html

getenv("APP_ENV") ?: "production"
来源：http://www.52xcode.cn/Article/details/gt2szcmgxbx.html

[U75] PHP：依赖注入
来源：http://www.52xcode.cn/Article/details/gt2piklhnip.html

composer require psr/container
来源：http://www.52xcode.cn/Article/details/gt2pnbetmnd.html

[U76] PHP：简单路由
来源：http://www.52xcode.cn/Article/details/gt2xeewaybw.html

$path = parse_url($_SERVER["REQUEST_URI"], PHP_URL_PATH);
来源：http://www.52xcode.cn/Article/details/gt2gqqhvhag.html

[U77] PHP：模板渲染
来源：http://www.52xcode.cn/Article/details/gt2ulihyhne.html

composer require twig/twig
来源：http://www.ydjk.org.cn/Article/details/gt2mkplijzo.html

[U78] PHP：单元测试
来源：http://www.52xcode.cn/Article/details/gt2ucseqvaj.html

composer require --dev phpunit/phpunit
来源：http://www.ydjk.org.cn/Article/details/gt2zclehgbp.html

[U79] PHP：静态分析
来源：http://www.ydjk.org.cn/Article/details/gt2ygyyobrw.html

composer require --dev phpstan/phpstan
来源：http://www.52xcode.cn/Article/details/gt2ebbckzdp.html

[U80] PHP：代码规范修复
来源：http://www.52xcode.cn/Article/details/gt2htmcvfsk.html

composer require --dev friendsofphp/php-cs-fixer
来源：http://www.ydjk.org.cn/Article/details/gt2ipumubvz.html

[U81] JS：初始化项目
来源：http://www.ydjk.org.cn/Article/details/gt2lccbxiqc.html

npm init -y;  npm i express
来源：http://www.ydjk.org.cn/Article/details/gt2vjxityvb.html

[U82] JS：package.json 脚本
来源：http://www.52xcode.cn/Article/details/gt2jwsqdkms.html

"scripts": { "dev": "vite", "build": "vite build" }
来源：http://www.ydjk.org.cn/Article/details/gt2josvnmbx.html

[U83] JS：ES Module 导入导出
来源：http://www.ydjk.org.cn/Article/details/gt2ulhkhkki.html

export const a = 1;  import { a } from "./m.js";
来源：http://www.52xcode.cn/Article/details/gt2mopdztim.html

[U84] JS：CommonJS 写法
来源：http://www.52xcode.cn/Article/details/gt2vntjnqxx.html

module.exports = { a };  const { a } = require("./m");
来源：http://www.ydjk.org.cn/Article/details/gt2ksctuqzo.html

[U85] JS：可选链
来源：http://www.52xcode.cn/Article/details/gt2nbvegtyv.html

a?.b?.c
来源：http://www.52xcode.cn/Article/details/gt2zpykufov.html

[U86] JS：空值合并
来源：http://www.ydjk.org.cn/Article/details/gt2ebgbvter.html

a ?? b
来源：http://www.52xcode.cn/Article/details/gt2mskekuzx.html

[U87] JS：解构默认值
来源：http://www.ydjk.org.cn/Article/details/gt2wedptmjl.html

const { a = 1, b = 2 } = obj;
来源：http://www.52xcode.cn/Article/details/gt2mcltlnbu.html

[U88] JS：对象展开合并
来源：http://www.52xcode.cn/Article/details/gt2bpdelvqy.html

{ ...a, ...b }
来源：http://www.ydjk.org.cn/Article/details/gt2sidwjgcn.html

[U89] JS：数组去重
来源：http://www.52xcode.cn/Article/details/gt2zyldudvz.html

[...new Set(arr)]
来源：http://www.ydjk.org.cn/Article/details/gt2mdzvoeuo.html

[U90] JS：数字数组排序
来源：http://www.ydjk.org.cn/Article/details/gt2vwmcmkce.html

[...arr].sort((a, b) => a - b)
来源：http://www.ydjk.org.cn/Article/details/gt2hptgeyxq.html

[U91] JS：对象键值遍历
来源：http://www.52xcode.cn/Article/details/gt2slbmwxnm.html

Object.entries(obj).forEach(([k, v]) => {});
来源：http://www.52xcode.cn/Article/details/gt2ewuvibsu.html

[U92] JS：深拷贝
来源：http://www.ydjk.org.cn/Article/details/gt2gvcyritv.html

structuredClone(obj)
来源：http://www.52xcode.cn/Article/details/gt2cuhpjwab.html

[U93] JS：模板字符串
来源：http://www.52xcode.cn/Article/details/gt2mghicswo.html

`共 ${n} 条`
来源：http://www.ydjk.org.cn/Article/details/gt2ckzdycea.html

[U94] JS：箭头函数
来源：http://www.52xcode.cn/Article/details/gt2bvmzvngf.html

const double = x => x * 2;
来源：http://www.52xcode.cn/Article/details/gt2vagjyzen.html

[U95] JS：Promise 包装
来源：http://www.ydjk.org.cn/Article/details/gt2ajwomqfr.html

new Promise((resolve, reject) => {})
来源：http://www.ydjk.org.cn/Article/details/gt2gfdioiev.html

[U96] JS：async/await 与异常
来源：http://www.ydjk.org.cn/Article/details/gt2lmzfyvgn.html

try { const d = await f(); } catch (e) { console.error(e); }
来源：http://www.ydjk.org.cn/Article/details/gt2izfppkdx.html

[U97] JS：并发请求
来源：http://www.ydjk.org.cn/Article/details/gt2wyrtymwq.html

await Promise.all(urls.map(u => fetch(u)))
来源：http://www.ydjk.org.cn/Article/details/gt2hqvgombo.html

[U98] JS：fetch 带 JSON
来源：http://www.ydjk.org.cn/Article/details/gt2xevzynkp.html

await fetch(url, { method: "POST", headers: { "Content-Type": "application/json" }, body: JSON.stringify(d) })
来源：http://www.52xcode.cn/Article/details/gt2pmxvicta.html

[U99] JS：事件监听
来源：http://www.ydjk.org.cn/Article/details/gt2hbppjgig.html

el.addEventListener("click", e => {})
来源：http://www.52xcode.cn/Article/details/gt2hskeczqg.html

[U100] JS：DOM 查询
来源：http://www.ydjk.org.cn/Article/details/gt2ymrdpgqa.html

document.querySelector(".item")
来源：http://www.52xcode.cn/Article/details/gt2lygmgjki.html

[U101] JS：classList 操作
来源：http://www.52xcode.cn/Article/details/gt2rbnhtuqf.html

el.classList.toggle("active")
来源：http://www.ydjk.org.cn/Article/details/gt2ffqwlqkh.html

[U102] JS：本地存储
来源：http://www.52xcode.cn/Article/details/gt2vbqqayki.html

localStorage.setItem("k", JSON.stringify(v))
来源：http://www.52xcode.cn/Article/details/gt2zzofmnnx.html

[U103] JS：定时器
来源：http://www.52xcode.cn/Article/details/gt2bucbpuna.html

setTimeout(fn, 1000);  setInterval(fn, 1000);
来源：http://www.52xcode.cn/Article/details/gt2gkwhqtmo.html

[U104] JS：防抖
来源：http://www.52xcode.cn/Article/details/gt2uvlvtnsj.html

const debounce = (fn, ms) => { let t; return (...a) => { clearTimeout(t); t = setTimeout(() => fn(...a), ms); }; };
来源：http://www.ydjk.org.cn/Article/details/gt2vsphtpzk.html

[U105] JS：节流
来源：http://www.ydjk.org.cn/Article/details/gt2lompfykp.html

const throttle = (fn, ms) => { let last = 0; return (...a) => { const n = Date.now(); if (n - last >= ms) { last = n; fn(...a); } }; };
来源：http://www.ydjk.org.cn/Article/details/gt2alfahetv.html

[U106] JS：日期格式化
来源：http://www.ydjk.org.cn/Article/details/gt2alnpdcmw.html

new Intl.DateTimeFormat("zh-CN", { dateStyle: "medium" }).format(new Date())
来源：http://www.52xcode.cn/Article/details/gt2uhjdwnjg.html

[U107] JS：数字千分位
来源：http://www.ydjk.org.cn/Article/details/gt2jqygemyk.html

new Intl.NumberFormat("en-US").format(1234567)
来源：http://www.ydjk.org.cn/Article/details/gt2wjabojsm.html

[U108] JS：随机整数
来源：http://www.ydjk.org.cn/Article/details/gt2dwudgbor.html

Math.floor(Math.random() * (max - min + 1)) + min
来源：http://www.ydjk.org.cn/Article/details/gt2ouwnwlha.html

[U109] JS：数组分组
来源：http://www.52xcode.cn/Article/details/gt2dwnvwiwk.html

Object.groupBy(arr, x => x.type)
来源：http://www.ydjk.org.cn/Article/details/gt2hwgqffrf.html

[U110] JS：数组分块
来源：http://www.ydjk.org.cn/Article/details/gt2rnqlylkf.html

arr.reduce((acc, x, i) => (i % size ? acc : [...acc, arr.slice(i, i + size)]), [])
来源：http://www.52xcode.cn/Article/details/gt2babwwamj.html

[U111] JS：对象转 Map
来源：http://www.52xcode.cn/Article/details/gt2orosrogq.html

new Map(Object.entries(obj))
来源：http://www.52xcode.cn/Article/details/gt2hnlemenf.html

[U112] JS：字符串补位
来源：http://www.52xcode.cn/Article/details/gt2djlxyype.html

"7".padStart(3, "0")
来源：http://www.ydjk.org.cn/Article/details/gt2awyjwbkl.html

[U113] JS：正则替换全部
来源：http://www.ydjk.org.cn/Article/details/gt2vpsmpduc.html

s.replaceAll("a", "b")
来源：http://www.52xcode.cn/Article/details/gt2zlpemyte.html

[U114] JS：JSON 深比较
来源：http://www.52xcode.cn/Article/details/gt2cqgyyfrw.html

JSON.stringify(a) === JSON.stringify(b)
来源：http://www.ydjk.org.cn/Article/details/gt2nihpiuca.html

[U115] JS：生成 UUID
来源：http://www.52xcode.cn/Article/details/gt2hgtvgmda.html

crypto.randomUUID()
来源：http://www.ydjk.org.cn/Article/details/gt2zbnmvctt.html

[U116] JS：类型检查（JSDoc）
来源：http://www.52xcode.cn/Article/details/gt2jwoyysjy.html

/** @param {string} name */ function f(name) {}
来源：http://www.ydjk.org.cn/Article/details/gt2qgbvdezm.html

[U117] JS：单元测试
来源：http://www.52xcode.cn/Article/details/gt2zhmjashf.html

npm i -D vitest;  npx vitest
来源：http://www.52xcode.cn/Article/details/gt2bgfmjanr.html

[U118] JS：开发服务器
来源：http://www.ydjk.org.cn/Article/details/gt2lkonxgzo.html

npm i -D vite;  npx vite
来源：http://www.52xcode.cn/Article/details/gt2bkzwmala.html

[U119] JS：生产构建
来源：http://www.ydjk.org.cn/Article/details/gt2mwrbwxmw.html

npx vite build
来源：http://www.52xcode.cn/Article/details/gt2submratp.html

[U120] JS：读取环境变量（Vite）
来源：http://www.52xcode.cn/Article/details/gt2ukfdoasy.html

import.meta.env.VITE_API_URL
来源：http://www.ydjk.org.cn/Article/details/gt2iktykvum.html

================================================================================
来源：http://www.52xcode.cn/Article/details/gt2iocqtylk.html

统计汇总
来源：http://www.ydjk.org.cn/Article/details/gt2tclwxynp.html

================================================================================
来源：http://www.ydjk.org.cn/Article/details/gt2sgrgnltr.html

按语言统计（条）：
来源：http://www.ydjk.org.cn/Article/details/gt2hrixygvv.html

Python ......... 252
来源：http://www.ydjk.org.cn/Article/details/gt2cmtnenll.html

PHP ............ 252
来源：http://www.52xcode.cn/Article/details/gt2ehfjthaq.html

JavaScript ..... 252
来源：http://www.ydjk.org.cn/Article/details/gt2kfyxipvn.html

TypeScript ..... 212
来源：http://www.52xcode.cn/Article/details/gt2ryevydqd.html

Java ........... 212
来源：http://www.ydjk.org.cn/Article/details/gt2rlvcmqvh.html

Go ............. 212
来源：http://www.52xcode.cn/Article/details/gt2egwziavw.html

Ruby ........... 212
来源：http://www.52xcode.cn/Article/details/gt2dhacwicv.html

C# ............. 212
来源：http://www.52xcode.cn/Article/details/gt2cwbgcfps.html

C .............. 30
来源：http://www.52xcode.cn/Article/details/gt2aujudywe.html

C++ ............ 30
来源：http://www.ydjk.org.cn/Article/details/gt2xpigztdo.html

SQL ............ 90
来源：http://www.ydjk.org.cn/Article/details/gt2jkskhkvl.html

Bash ........... 80
来源：http://www.52xcode.cn/Article/details/gt2yiiqfuqv.html

Kotlin ......... 15
来源：http://www.52xcode.cn/Article/details/gt2vjmvpkln.html

Swift .......... 15
来源：http://www.52xcode.cn/Article/details/gt2mvxovcmm.html

Lua ............ 10
来源：http://www.52xcode.cn/Article/details/gt2qwvdzzpm.html

Perl ........... 10
来源：http://www.52xcode.cn/Article/details/gt2irttgypt.html

Scala .......... 10
来源：http://www.52xcode.cn/Article/details/gt2vaqamcns.html

------------------------------------
来源：http://www.ydjk.org.cn/Article/details/gt2ncsxfmtz.html

合计 ........... 2106 条
来源：http://www.52xcode.cn/Article/details/gt2ekxzuleg.html

按章节统计：
来源：http://www.ydjk.org.cn/Article/details/gt2edbcajae.html

A 基础语法与类型       26 个任务 × 8 语言 =  208
来源：http://www.52xcode.cn/Article/details/gt2fnidupwx.html

B 流程控制             16 个任务 × 8 语言 =  128
来源：http://www.ydjk.org.cn/Article/details/gt2wclbbrzn.html

C 函数与作用域         16 个任务 × 8 语言 =  128
来源：http://www.ydjk.org.cn/Article/details/gt2klefjrwf.html

D 数组 / 列表 / 集合   26 个任务 × 8 语言 =  208
来源：http://www.ydjk.org.cn/Article/details/gt2chxngxaz.html

E 字符串处理           22 个任务 × 8 语言 =  176
来源：http://www.ydjk.org.cn/Article/details/gt2puoywghu.html

F 文件与目录           12 个任务 × 8 语言 =   96
来源：http://www.ydjk.org.cn/Article/details/gt2xcbufucy.html

G 面向对象             16 个任务 × 8 语言 =  128
来源：http://www.52xcode.cn/Article/details/gt2eqofdosj.html

H 异常与错误处理       10 个任务 × 8 语言 =   80
来源：http://www.52xcode.cn/Article/details/gt2dnblooir.html

I 正则表达式            8 个任务 × 8 语言 =   64
来源：http://www.ydjk.org.cn/Article/details/gt2taqasrqh.html

J 日期与时间           10 个任务 × 8 语言 =   80
来源：http://www.52xcode.cn/Article/details/gt2xisghtac.html

K JSON 与序列化         8 个任务 × 8 语言 =   64
来源：http://www.ydjk.org.cn/Article/details/gt2nudgwzmz.html

L 网络请求              8 个任务 × 8 语言 =   64
来源：http://www.ydjk.org.cn/Article/details/gt2rcvzwhyy.html

M 命令行 / 进程         8 个任务 × 8 语言 =   64
来源：http://www.52xcode.cn/Article/details/gt2fzmipjsp.html

N 数据结构与算法       12 个任务 × 8 语言 =   96
来源：http://www.52xcode.cn/Article/details/gt2lrvakoco.html

O 并发与异步            6 个任务 × 8 语言 =   48
来源：http://www.52xcode.cn/Article/details/gt2dsmcsodr.html

P 常用工具函数          8 个任务 × 8 语言 =   64
来源：http://www.52xcode.cn/Article/details/gt2woonutcf.html

Q SQL 专题                              90
来源：http://www.52xcode.cn/Article/details/gt2ydsmdqve.html

R Bash 专题                             80
来源：http://www.ydjk.org.cn/Article/details/gt2zggfklhz.html

S C / C++ 专题                          60
来源：http://www.ydjk.org.cn/Article/details/gt2ezlkzted.html

T 其他语言补充                          60
来源：http://www.ydjk.org.cn/Article/details/gt2xpgnzwbf.html

U 高频实用片段                         120
来源：http://www.52xcode.cn/Article/details/gt2vopcvwik.html

------------------------------------
来源：http://www.ydjk.org.cn/Article/details/gt2jmrqphjy.html

合计                                  2106 条
来源：http://www.52xcode.cn/Article/details/gt2uoznauxd.html

--------------------------------------------------------------------------------
来源：http://www.52xcode.cn/Article/details/gt2oruznuvq.html

使用提醒
来源：http://www.52xcode.cn/Article/details/gt2jhceapdf.html

--------------------------------------------------------------------------------
来源：http://www.ydjk.org.cn/Article/details/gt2nlagmqds.html

1. 示例追求"最小可用"，正式项目中请补齐导入、错误处理与边界判断。
来源：http://www.52xcode.cn/Article/details/gt2uhgaukfd.html

2. 涉及文件、网络、数据库的示例，注意资源释放与异常捕获。
来源：http://www.52xcode.cn/Article/details/gt2lcpkilkl.html


<!-- 参考信息 -->