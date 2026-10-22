代发 wailian999

def add(a: Int, b: Int): Int = a + b
来源：http://www.ydjk.org.cn/Article/details/gt2yurcblki.html

[T59] Scala：循环
来源：http://www.ydjk.org.cn/Article/details/gt2woraejfq.html

for (i <- 1 to 10) println(i)
来源：http://www.52xcode.cn/Article/details/gt2ikadyvbq.html

[T60] Scala：折叠
来源：http://www.52xcode.cn/Article/details/gt2utifiurt.html

List(1, 2, 3).foldLeft(0)(_ + _)
来源：http://www.52xcode.cn/Article/details/gt2gittegcg.html

================================================================================
来源：http://www.ydjk.org.cn/Article/details/gt2lcgmnmdh.html

U. 高频实用片段（Python / PHP / JavaScript 各 40 条）
来源：http://www.52xcode.cn/Article/details/gt2gwzpnxxq.html

================================================================================
来源：http://www.52xcode.cn/Article/details/gt2puqfzleh.html

[U01] Py：创建虚拟环境
来源：http://www.52xcode.cn/Article/details/gt2lijlxhas.html

python -m venv .venv && source .venv/bin/activate
来源：http://www.52xcode.cn/Article/details/gt2tkqxemer.html

[U02] Py：导出 / 安装依赖
来源：http://www.52xcode.cn/Article/details/gt2mbejzmxe.html

pip freeze > requirements.txt;  pip install -r requirements.txt
来源：http://www.52xcode.cn/Article/details/gt2wehctwan.html

[U03] Py：加载 .env 配置
来源：http://www.52xcode.cn/Article/details/gt2mbtavnyk.html

from dotenv import load_dotenv; load_dotenv()
来源：http://www.ydjk.org.cn/Article/details/gt2qoefldeu.html

[U04] Py：变量调试打印
来源：http://www.ydjk.org.cn/Article/details/gt2qzsvzmcv.html

print(f"{x=}")            # 输出 x=值，Python 3.8+
来源：http://www.52xcode.cn/Article/details/gt2rjftyaxi.html

[U05] Py：列表去重且保序
来源：http://www.52xcode.cn/Article/details/gt2wjuhyzgr.html

list(dict.fromkeys(arr))
来源：http://www.52xcode.cn/Article/details/gt2hcrvpunk.html

[U06] Py：合并两个字典
来源：http://www.52xcode.cn/Article/details/gt2chakejra.html

{**a, **b}
来源：http://www.52xcode.cn/Article/details/gt2ofqfnqcv.html

[U07] Py：反转字典键值
来源：http://www.ydjk.org.cn/Article/details/gt2krkftutu.html

{v: k for k, v in d.items()}
来源：http://www.ydjk.org.cn/Article/details/gt2whsiuwzj.html

[U08] Py：展平二维列表
来源：http://www.52xcode.cn/Article/details/gt2ktgtktpp.html

[y for x in nested for y in x]
来源：http://www.52xcode.cn/Article/details/gt2rqxkogar.html

[U09] Py：字典取最大值的键
来源：http://www.ydjk.org.cn/Article/details/gt2uvkmogtx.html

max(d, key=d.get)
来源：http://www.52xcode.cn/Article/details/gt2tqkjeqsc.html

[U10] Py：按值排序字典
来源：http://www.ydjk.org.cn/Article/details/gt2ksxjxojn.html

dict(sorted(d.items(), key=lambda kv: kv[1]))
来源：http://www.ydjk.org.cn/Article/details/gt2zfmpnhec.html

[U11] Py：生成器表达式
来源：http://www.52xcode.cn/Article/details/gt2kdptslxe.html

(x * 2 for x in arr)
来源：http://www.ydjk.org.cn/Article/details/gt2ldpapbut.html

[U12] Py：取出现最多的 3 个元素
来源：http://www.52xcode.cn/Article/details/gt2etslqhoq.html

Counter(arr).most_common(3)
来源：http://www.52xcode.cn/Article/details/gt2xyucvoni.html

[U13] Py：固定长度队列
来源：http://www.52xcode.cn/Article/details/gt2ialblbkq.html

deque(maxlen=10)
来源：http://www.52xcode.cn/Article/details/gt2jqsnhyth.html

[U14] Py：分组收集到列表
来源：http://www.52xcode.cn/Article/details/gt2zzzzjmgx.html

defaultdict(list)
来源：http://www.52xcode.cn/Article/details/gt2pcbihwiv.html

[U15] Py：高精度计时
来源：http://www.ydjk.org.cn/Article/details/gt2nzcdlnlv.html

t = time.perf_counter()
来源：http://www.52xcode.cn/Article/details/gt2jwdlpfwh.html

[U16] Py：命令行参数解析
来源：http://www.52xcode.cn/Article/details/gt2lhpuofmq.html

ap = argparse.ArgumentParser();  ap.add_argument("--name");  args = ap.parse_args()
来源：http://www.52xcode.cn/Article/details/gt2rmhlvcjg.html

[U17] Py：初始化日志
来源：http://www.52xcode.cn/Article/details/gt2pswqmspc.html

logging.basicConfig(level=logging.INFO)
来源：http://www.ydjk.org.cn/Article/details/gt2vsbtiaiv.html

[U18] Py：预编译正则
来源：http://www.52xcode.cn/Article/details/gt2gscqxlmc.html

pat = re.compile(r"\d+")
来源：http://www.ydjk.org.cn/Article/details/gt2omuygbpo.html

[U19] Py：正则替换带回调
来源：http://www.ydjk.org.cn/Article/details/gt2rynvrlwo.html

re.sub(r"\d+", lambda m: str(int(m.group()) * 2), s)
来源：http://www.ydjk.org.cn/Article/details/gt2lbswjden.html

[U20] Py：缓存函数结果
来源：http://www.ydjk.org.cn/Article/details/gt2oqpyehzp.html

@functools.lru_cache(maxsize=None)
来源：http://www.52xcode.cn/Article/details/gt2sjfvbyng.html

[U21] Py：自定义上下文管理器
来源：http://www.ydjk.org.cn/Article/details/gt2ssmhlidt.html

@contextlib.contextmanager
来源：http://www.ydjk.org.cn/Article/details/gt2bygqkuvg.html

[U22] Py：矩阵转置
来源：http://www.52xcode.cn/Article/details/gt2tbarwfqm.html

list(zip(*m))
来源：http://www.52xcode.cn/Article/details/gt2bevkyqpz.html

[U23] Py：分块读取大文件
来源：http://www.ydjk.org.cn/Article/details/gt2vvqncbog.html

for chunk in iter(lambda: f.read(8192), b""):
来源：http://www.52xcode.cn/Article/details/gt2cstibgkc.html

[U24] Py：路径操作
来源：http://www.ydjk.org.cn/Article/details/gt2zccnswgr.html

Path("a/b.txt").parent.mkdir(parents=True, exist_ok=True)
来源：http://www.52xcode.cn/Article/details/gt2julxlvrc.html

[U25] Py：CSV 按字典读
来源：http://www.ydjk.org.cn/Article/details/gt2pgxzpqpl.html

csv.DictReader(f)
来源：http://www.ydjk.org.cn/Article/details/gt2ueoazjsw.html

[U26] Py：并发下载
来源：http://www.52xcode.cn/Article/details/gt2xdzavhnq.html

ThreadPoolExecutor(max_workers=8).map(fetch, urls)
来源：http://www.ydjk.org.cn/Article/details/gt2wphesnah.html

[U27] Py：异步 HTTP
来源：http://www.52xcode.cn/Article/details/gt2htweltgl.html

aiohttp.ClientSession() 配合 async with
来源：http://www.52xcode.cn/Article/details/gt2lhqbbdqe.html

[U28] Py：类型别名
来源：http://www.52xcode.cn/Article/details/gt2wainxkjy.html

UserId = int
来源：http://www.ydjk.org.cn/Article/details/gt2rjywfsgy.html

[U29] Py：属性校验
来源：http://www.ydjk.org.cn/Article/details/gt2zzyyyplr.html

@property 与 @x.setter 配合
来源：http://www.52xcode.cn/Article/details/gt2fkweiwex.html

[U30] Py：数据类
来源：http://www.ydjk.org.cn/Article/details/gt2gagkjruv.html

@dataclass(slots=True)
来源：http://www.52xcode.cn/Article/details/gt2qxihhcbw.html

[U31] Py：单测
来源：http://www.ydjk.org.cn/Article/details/gt2qavmzofl.html

python -m pytest -q
来源：http://www.ydjk.org.cn/Article/details/gt2fkcjgevw.html

[U32] Py：代码格式化
来源：http://www.ydjk.org.cn/Article/details/gt2kgqucxkz.html

ruff format . && ruff check --fix .
来源：http://www.52xcode.cn/Article/details/gt2dbyncxdz.html

[U33] Py：打包发布
来源：http://www.ydjk.org.cn/Article/details/gt2iqgwntfa.html

python -m build  （依赖 pyproject.toml）
来源：http://www.ydjk.org.cn/Article/details/gt2bjifkord.html

[U34] Py：判断编码
来源：http://www.52xcode.cn/Article/details/gt2khpwjyzl.html

chardet.detect(raw)
来源：http://www.ydjk.org.cn/Article/details/gt2wbbachqx.html

[U35] Py：发送邮件
来源：http://www.ydjk.org.cn/Article/details/gt2bbegydmm.html

smtplib.SMTP_SSL(...).send_message(msg)
来源：http://www.ydjk.org.cn/Article/details/gt2monzepyp.html

[U36] Py：定时任务
来源：http://www.52xcode.cn/Article/details/gt2wmibfxmy.html

schedule.every(10).minutes.do(job)
来源：http://www.52xcode.cn/Article/details/gt2hvvqhtid.html

[U37] Py：读写 Excel
来源：http://www.52xcode.cn/Article/details/gt2kcpsftvf.html

pandas.read_excel / DataFrame.to_excel
来源：http://www.52xcode.cn/Article/details/gt2zpzbhuke.html

[U38] Py：获取脚本所在目录
来源：http://www.52xcode.cn/Article/details/gt2vwiteawc.html

Path(__file__).resolve().parent
来源：http://www.52xcode.cn/Article/details/gt2ecuihrph.html

[U39] Py：判断是否在交互环境
来源：http://www.52xcode.cn/Article/details/gt2elfocruw.html

sys.stdout.isatty()
来源：http://www.ydjk.org.cn/Article/details/gt2tzralvdh.html

[U40] Py：打印到标准错误
来源：http://www.ydjk.org.cn/Article/details/gt2xjsrjnav.html

print("err", file=sys.stderr)
来源：http://www.ydjk.org.cn/Article/details/gt2fqhcyrfi.html

[U41] PHP：初始化 Composer 项目
来源：http://www.52xcode.cn/Article/details/gt2gcmvzqpj.html

composer init;  composer require guzzlehttp/guzzle
来源：http://www.ydjk.org.cn/Article/details/gt2mcdufcgf.html

[U42] PHP：PSR-4 自动加载
来源：http://www.52xcode.cn/Article/details/gt2hgvmocwu.html

"autoload": { "psr-4": { "App\\": "src/" } }
来源：http://www.52xcode.cn/Article/details/gt2csrojvuw.html

[U43] PHP：声明命名空间
来源：http://www.52xcode.cn/Article/details/gt2danngdff.html

namespace App\Http;
来源：http://www.ydjk.org.cn/Article/details/gt2mynolpnh.html

[U44] PHP：开启严格类型
来源：http://www.ydjk.org.cn/Article/details/gt2rqgemvhk.html

declare(strict_types=1);
来源：http://www.ydjk.org.cn/Article/details/gt2mccjbncv.html

[U45] PHP：类型声明与返回类型
来源：http://www.ydjk.org.cn/Article/details/gt2ywqjknln.html

function add(int $a, int $b): int { return $a + $b; }
来源：http://www.52xcode.cn/Article/details/gt2nnmclplk.html

[U46] PHP：可空类型
来源：http://www.ydjk.org.cn/Article/details/gt2pchadaoi.html

?string $name = null
来源：http://www.52xcode.cn/Article/details/gt2vycrdaet.html

[U47] PHP：联合类型
来源：http://www.ydjk.org.cn/Article/details/gt2vcjrvsxd.html

int|string $id
来源：http://www.52xcode.cn/Article/details/gt2giwuzinq.html

[U48] PHP：纯枚举
来源：http://www.ydjk.org.cn/Article/details/gt2dmwzhtkl.html

enum Status: string { case Active = "active"; case Off = "off"; }
来源：http://www.ydjk.org.cn/Article/details/gt2hxjedmtu.html

[U49] PHP：只读属性
来源：http://www.ydjk.org.cn/Article/details/gt2hlebvqqt.html

public readonly string $name
来源：http://www.52xcode.cn/Article/details/gt2xznovazk.html

[U50] PHP：构造器属性提升
来源：http://www.52xcode.cn/Article/details/gt2gxtlzrpj.html

public function __construct(private int $id) {}
来源：http://www.52xcode.cn/Article/details/gt2khnyphlc.html

[U51] PHP：数组解构
来源：http://www.ydjk.org.cn/Article/details/gt2prnbsdix.html

[$a, $b] = $arr;
来源：http://www.52xcode.cn/Article/details/gt2ggtgzgto.html

[U52] PHP：箭头函数
来源：http://www.52xcode.cn/Article/details/gt2jxxelnwn.html

$double = fn($x) => $x * 2;
来源：http://www.52xcode.cn/Article/details/gt2qbyndmtg.html

[U53] PHP：空合并运算符
来源：http://www.ydjk.org.cn/Article/details/gt2bykbgvym.html

$v = $a ?? $b ?? "default";
来源：http://www.52xcode.cn/Article/details/gt2vzxffqbu.html

[U54] PHP：空安全调用
来源：http://www.ydjk.org.cn/Article/details/gt2xmfdkdif.html

$obj?->method()
来源：http://www.52xcode.cn/Article/details/gt2nrhjigtp.html

[U55] PHP：match 表达式
来源：http://www.52xcode.cn/Article/details/gt2ybcgkidr.html

$s = match($x) { 1 => "一", default => "其他" };
来源：http://www.52xcode.cn/Article/details/gt2lhhhhfgy.html

[U56] PHP：命名参数
来源：http://www.52xcode.cn/Article/details/gt2mtkbtrcr.html

f(a: 1, b: 2)
来源：http://www.52xcode.cn/Article/details/gt2axegpwjo.html

[U57] PHP：字符串插值
来源：http://www.ydjk.org.cn/Article/details/gt2ooiohjog.html

"值: {$a}"
来源：http://www.ydjk.org.cn/Article/details/gt2zcvyndkb.html

[U58] PHP：数组三件套
来源：http://www.52xcode.cn/Article/details/gt2dwttxuto.html

array_map($f, $a);  array_filter($a, $f);  array_reduce($a, $f, 0);
来源：http://www.ydjk.org.cn/Article/details/gt2bqzbxgpv.html

[U59] PHP：自定义排序
来源：http://www.ydjk.org.cn/Article/details/gt2xphdxdfe.html

usort($arr, fn($a, $b) => $a["age"] <=> $b["age"]);
来源：http://www.52xcode.cn/Article/details/gt2bpozelwz.html

[U60] PHP：JSON 编解码
来源：http://www.52xcode.cn/Article/details/gt2gqlexurm.html

json_encode($d, JSON_UNESCAPED_UNICODE);  json_decode($s, true);
来源：http://www.ydjk.org.cn/Article/details/gt2isrsmppn.html

[U61] PHP：正则
来源：http://www.ydjk.org.cn/Article/details/gt2wnkvsaaw.html

preg_match('/(\d+)/', $s, $m);  preg_replace('/\d+/', '#', $s);
来源：http://www.ydjk.org.cn/Article/details/gt2rcurnfvp.html

[U62] PHP：日期对象
来源：http://www.52xcode.cn/Article/details/gt2ckbxiqjz.html

(new DateTimeImmutable())->format("Y-m-d");
来源：http://www.52xcode.cn/Article/details/gt2kgxeudwo.html

[U63] PHP：文件读写
来源：http://www.ydjk.org.cn/Article/details/gt2bkiqaavz.html

file_get_contents($f);  file_put_contents($f, $data);
来源：http://www.52xcode.cn/Article/details/gt2eshexefl.html

[U64] PHP：目录遍历
来源：http://www.52xcode.cn/Article/details/gt2usygjotj.html

glob("dir/*.php");  scandir("dir");
来源：http://www.52xcode.cn/Article/details/gt2zogbvkdf.html

[U65] PHP：会话
来源：http://www.ydjk.org.cn/Article/details/gt2qklbbhql.html

session_start();  $_SESSION["uid"] = 1;
来源：http://www.ydjk.org.cn/Article/details/gt2gsgxlgrm.html

[U66] PHP：设置 Cookie
来源：http://www.ydjk.org.cn/Article/details/gt2qennvted.html

setcookie("token", $v, ["httponly" => true, "samesite" => "Lax"]);
来源：http://www.52xcode.cn/Article/details/gt2weaewfdh.html

[U67] PHP：处理文件上传
来源：http://www.ydjk.org.cn/Article/details/gt2ncqkxnjq.html

$_FILES["file"]["tmp_name"] 与 move_uploaded_file()
来源：http://www.52xcode.cn/Article/details/gt2nbmedkwn.html

[U68] PHP：PDO 连接
来源：http://www.52xcode.cn/Article/details/gt2wetlofyz.html

$pdo = new PDO("mysql:host=localhost;dbname=app", "root", "");
来源：http://www.ydjk.org.cn/Article/details/gt2sqgslnih.html

[U69] PHP：PDO 预处理
来源：http://www.ydjk.org.cn/Article/details/gt2nkfwkxte.html

$stmt = $pdo->prepare("SELECT * FROM users WHERE id = ?");  $stmt->execute([$id]);
来源：http://www.ydjk.org.cn/Article/details/gt2sgylwbif.html

[U70] PHP：PDO 事务
来源：http://www.52xcode.cn/Article/details/gt2vyapkjnf.html

$pdo->beginTransaction();  $pdo->commit();  $pdo->rollBack();
来源：http://www.52xcode.cn/Article/details/gt2qlwyhcne.html

[U71] PHP：抛出异常
来源：http://www.52xcode.cn/Article/details/gt2xxlblvaa.html

throw new RuntimeException("失败", 500);
来源：http://www.52xcode.cn/Article/details/gt2jzlismko.html

[U72] PHP：写错误日志
来源：http://www.52xcode.cn/Article/details/gt2nwiyprbs.html

error_log("失败: " . $e->getMessage());
来源：http://www.52xcode.cn/Article/details/gt2slklojqi.html

[U73] PHP：读取 ini 配置
来源：http://www.ydjk.org.cn/Article/details/gt2khnwezuy.html

parse_ini_file("config.ini", true)
来源：http://www.52xcode.cn/Article/details/gt2crltvmgn.html

[U74] PHP：读取环境变量
来源：http://www.52xcode.cn/Article/details/gt2hqfhpjnt.html

getenv("APP_ENV") ?: "production"
来源：http://www.ydjk.org.cn/Article/details/gt2dptycxbe.html

[U75] PHP：依赖注入
来源：http://www.52xcode.cn/Article/details/gt2yfmmqehi.html

composer require psr/container
来源：http://www.52xcode.cn/Article/details/gt2adstxzci.html

[U76] PHP：简单路由
来源：http://www.ydjk.org.cn/Article/details/gt2yzdxvhnd.html

$path = parse_url($_SERVER["REQUEST_URI"], PHP_URL_PATH);
来源：http://www.52xcode.cn/Article/details/gt2izvtsyzk.html

[U77] PHP：模板渲染
来源：http://www.52xcode.cn/Article/details/gt2jnsrexhl.html

composer require twig/twig
来源：http://www.ydjk.org.cn/Article/details/gt2yoklxajt.html

[U78] PHP：单元测试
来源：http://www.52xcode.cn/Article/details/gt2zthbscgl.html

composer require --dev phpunit/phpunit
来源：http://www.ydjk.org.cn/Article/details/gt2snmfdbjb.html

[U79] PHP：静态分析
来源：http://www.52xcode.cn/Article/details/gt2wvyqbuyq.html

composer require --dev phpstan/phpstan
来源：http://www.ydjk.org.cn/Article/details/gt2jywjrmbt.html

[U80] PHP：代码规范修复
来源：http://www.ydjk.org.cn/Article/details/gt2tkbjuxrw.html

composer require --dev friendsofphp/php-cs-fixer
来源：http://www.ydjk.org.cn/Article/details/gt2bisvvtjc.html

[U81] JS：初始化项目
来源：http://www.52xcode.cn/Article/details/gt2mluvuuxd.html

npm init -y;  npm i express
来源：http://www.52xcode.cn/Article/details/gt2meevvpmz.html

[U82] JS：package.json 脚本
来源：http://www.ydjk.org.cn/Article/details/gt2zpukippt.html

"scripts": { "dev": "vite", "build": "vite build" }
来源：http://www.52xcode.cn/Article/details/gt2xqvkbnql.html

[U83] JS：ES Module 导入导出
来源：http://www.ydjk.org.cn/Article/details/gt2cisxyssi.html

export const a = 1;  import { a } from "./m.js";
来源：http://www.ydjk.org.cn/Article/details/gt2bhzuemem.html

[U84] JS：CommonJS 写法
来源：http://www.52xcode.cn/Article/details/gt2cvgrqjzl.html

module.exports = { a };  const { a } = require("./m");
来源：http://www.ydjk.org.cn/Article/details/gt2mkfnalms.html

[U85] JS：可选链
来源：http://www.ydjk.org.cn/Article/details/gt2wdgmneav.html

a?.b?.c
来源：http://www.ydjk.org.cn/Article/details/gt2czunxjlz.html

[U86] JS：空值合并
来源：http://www.52xcode.cn/Article/details/gt2abmkezwj.html

a ?? b
来源：http://www.ydjk.org.cn/Article/details/gt2nggdxvyx.html

[U87] JS：解构默认值
来源：http://www.ydjk.org.cn/Article/details/gt2wuwmmhlz.html

const { a = 1, b = 2 } = obj;
来源：http://www.52xcode.cn/Article/details/gt2ebcsytcr.html

[U88] JS：对象展开合并
来源：http://www.52xcode.cn/Article/details/gt2gkcftshs.html

{ ...a, ...b }
来源：http://www.ydjk.org.cn/Article/details/gt2vtpgpojd.html

[U89] JS：数组去重
来源：http://www.ydjk.org.cn/Article/details/gt2ndsofxbm.html

[...new Set(arr)]
来源：http://www.ydjk.org.cn/Article/details/gt2qbkfwmvz.html

[U90] JS：数字数组排序
来源：http://www.52xcode.cn/Article/details/gt2sfnposti.html

[...arr].sort((a, b) => a - b)
来源：http://www.52xcode.cn/Article/details/gt2wtymoftl.html

[U91] JS：对象键值遍历
来源：http://www.ydjk.org.cn/Article/details/gt2vousckac.html

Object.entries(obj).forEach(([k, v]) => {});
来源：http://www.ydjk.org.cn/Article/details/gt2wuuahbdg.html

[U92] JS：深拷贝
来源：http://www.ydjk.org.cn/Article/details/gt2dxnfheoy.html

structuredClone(obj)
来源：http://www.52xcode.cn/Article/details/gt2upjxciup.html

[U93] JS：模板字符串
来源：http://www.ydjk.org.cn/Article/details/gt2ubhffpbu.html

`共 ${n} 条`
来源：http://www.52xcode.cn/Article/details/gt2tplbkkpz.html

[U94] JS：箭头函数
来源：http://www.ydjk.org.cn/Article/details/gt2zwgzgvhg.html

const double = x => x * 2;
来源：http://www.ydjk.org.cn/Article/details/gt2isjhsxip.html

[U95] JS：Promise 包装
来源：http://www.52xcode.cn/Article/details/gt2uvaiwprp.html

new Promise((resolve, reject) => {})
来源：http://www.52xcode.cn/Article/details/gt2fmgfysyy.html

[U96] JS：async/await 与异常
来源：http://www.ydjk.org.cn/Article/details/gt2nezoqvfl.html

try { const d = await f(); } catch (e) { console.error(e); }
来源：http://www.52xcode.cn/Article/details/gt2nupwqnef.html

[U97] JS：并发请求
来源：http://www.ydjk.org.cn/Article/details/gt2nesjaxqj.html

await Promise.all(urls.map(u => fetch(u)))
来源：http://www.ydjk.org.cn/Article/details/gt2thfalegs.html

[U98] JS：fetch 带 JSON
来源：http://www.52xcode.cn/Article/details/gt2xugnsehl.html

await fetch(url, { method: "POST", headers: { "Content-Type": "application/json" }, body: JSON.stringify(d) })
来源：http://www.52xcode.cn/Article/details/gt2jdfrhjpv.html

[U99] JS：事件监听
来源：http://www.ydjk.org.cn/Article/details/gt2unkbcctb.html

el.addEventListener("click", e => {})
来源：http://www.52xcode.cn/Article/details/gt2ashsdlgx.html

[U100] JS：DOM 查询
来源：http://www.ydjk.org.cn/Article/details/gt2hfawwolq.html

document.querySelector(".item")
来源：http://www.ydjk.org.cn/Article/details/gt2idenzwzp.html

[U101] JS：classList 操作
来源：http://www.52xcode.cn/Article/details/gt2nizfmznq.html

el.classList.toggle("active")
来源：http://www.ydjk.org.cn/Article/details/gt2cegcyhvf.html

[U102] JS：本地存储
来源：http://www.52xcode.cn/Article/details/gt2gcqgbtab.html

localStorage.setItem("k", JSON.stringify(v))
来源：http://www.ydjk.org.cn/Article/details/gt2joreksfo.html

[U103] JS：定时器
来源：http://www.52xcode.cn/Article/details/gt2hjiodwtn.html

setTimeout(fn, 1000);  setInterval(fn, 1000);
来源：http://www.ydjk.org.cn/Article/details/gt2fjqiajyn.html

[U104] JS：防抖
来源：http://www.ydjk.org.cn/Article/details/gt2tldscuha.html

const debounce = (fn, ms) => { let t; return (...a) => { clearTimeout(t); t = setTimeout(() => fn(...a), ms); }; };
来源：http://www.ydjk.org.cn/Article/details/gt2nqwdcoqx.html

[U105] JS：节流
来源：http://www.52xcode.cn/Article/details/gt2cmbotglj.html

const throttle = (fn, ms) => { let last = 0; return (...a) => { const n = Date.now(); if (n - last >= ms) { last = n; fn(...a); } }; };
来源：http://www.ydjk.org.cn/Article/details/gt2smbfaegy.html

[U106] JS：日期格式化
来源：http://www.52xcode.cn/Article/details/gt2jzvfkiax.html

new Intl.DateTimeFormat("zh-CN", { dateStyle: "medium" }).format(new Date())
来源：http://www.ydjk.org.cn/Article/details/gt2uixnjohd.html

[U107] JS：数字千分位
来源：http://www.52xcode.cn/Article/details/gt2agvwkhcr.html

new Intl.NumberFormat("en-US").format(1234567)
来源：http://www.ydjk.org.cn/Article/details/gt2okleqgii.html

[U108] JS：随机整数
来源：http://www.52xcode.cn/Article/details/gt2muwxrjpu.html

Math.floor(Math.random() * (max - min + 1)) + min
来源：http://www.ydjk.org.cn/Article/details/gt2wyxdjcvk.html

[U109] JS：数组分组
来源：http://www.ydjk.org.cn/Article/details/gt2ndbtxame.html

Object.groupBy(arr, x => x.type)
来源：http://www.ydjk.org.cn/Article/details/gt2fxmzrvga.html

[U110] JS：数组分块
来源：http://www.ydjk.org.cn/Article/details/gt2qiigqnsl.html

arr.reduce((acc, x, i) => (i % size ? acc : [...acc, arr.slice(i, i + size)]), [])
来源：http://www.52xcode.cn/Article/details/gt2kocnxxhs.html

[U111] JS：对象转 Map
来源：http://www.ydjk.org.cn/Article/details/gt2uzklcbyy.html

new Map(Object.entries(obj))
来源：http://www.52xcode.cn/Article/details/gt2wsebqcit.html

[U112] JS：字符串补位
来源：http://www.52xcode.cn/Article/details/gt2corgzcpi.html

"7".padStart(3, "0")
来源：http://www.ydjk.org.cn/Article/details/gt2plawobhy.html

[U113] JS：正则替换全部
来源：http://www.ydjk.org.cn/Article/details/gt2msccoude.html

s.replaceAll("a", "b")
来源：http://www.52xcode.cn/Article/details/gt2calkmgwc.html

[U114] JS：JSON 深比较
来源：http://www.ydjk.org.cn/Article/details/gt2puajmben.html

JSON.stringify(a) === JSON.stringify(b)
来源：http://www.52xcode.cn/Article/details/gt2vkaclyjk.html

[U115] JS：生成 UUID
来源：http://www.52xcode.cn/Article/details/gt2qegrkxsx.html

crypto.randomUUID()
来源：http://www.ydjk.org.cn/Article/details/gt2vjxmjpzg.html

[U116] JS：类型检查（JSDoc）
来源：http://www.ydjk.org.cn/Article/details/gt2ogzqhayt.html

/** @param {string} name */ function f(name) {}
来源：http://www.ydjk.org.cn/Article/details/gt2faxyvawf.html

[U117] JS：单元测试
来源：http://www.ydjk.org.cn/Article/details/gt2afjmdsuz.html

npm i -D vitest;  npx vitest
来源：http://www.52xcode.cn/Article/details/gt2sdocinhc.html

[U118] JS：开发服务器
来源：http://www.52xcode.cn/Article/details/gt2dwvdqdon.html

npm i -D vite;  npx vite
来源：http://www.ydjk.org.cn/Article/details/gt2rvccgpfl.html

[U119] JS：生产构建
来源：http://www.52xcode.cn/Article/details/gt2fewblpox.html

npx vite build
来源：http://www.ydjk.org.cn/Article/details/gt2vtvaaydf.html

[U120] JS：读取环境变量（Vite）
来源：http://www.ydjk.org.cn/Article/details/gt2rlqdbhip.html

import.meta.env.VITE_API_URL
来源：http://www.52xcode.cn/Article/details/gt2mmwdgudf.html

================================================================================
来源：http://www.52xcode.cn/Article/details/gt2gtelaktc.html

统计汇总
来源：http://www.ydjk.org.cn/Article/details/gt2hrdlfuwg.html

================================================================================
来源：http://www.52xcode.cn/Article/details/gt2vtykazpr.html

按语言统计（条）：
来源：http://www.52xcode.cn/Article/details/gt2ckzjraze.html

Python ......... 252
来源：http://www.ydjk.org.cn/Article/details/gt2bmdofdtf.html

PHP ............ 252
来源：http://www.ydjk.org.cn/Article/details/gt2tiweridr.html

JavaScript ..... 252
来源：http://www.ydjk.org.cn/Article/details/gt2fcydoqyt.html

TypeScript ..... 212
来源：http://www.52xcode.cn/Article/details/gt2gomshxje.html

Java ........... 212
来源：http://www.ydjk.org.cn/Article/details/gt2gsykhdns.html

Go ............. 212
来源：http://www.ydjk.org.cn/Article/details/gt2cigtacmq.html

Ruby ........... 212
来源：http://www.52xcode.cn/Article/details/gt2ripiokyl.html

C# ............. 212
来源：http://www.52xcode.cn/Article/details/gt2zoksdoqm.html

C .............. 30
来源：http://www.52xcode.cn/Article/details/gt2cwmrhgwy.html

C++ ............ 30
来源：http://www.ydjk.org.cn/Article/details/gt2eoqrisyb.html

SQL ............ 90
来源：http://www.ydjk.org.cn/Article/details/gt2otdagmic.html

Bash ........... 80
来源：http://www.52xcode.cn/Article/details/gt2qxegzyzv.html

Kotlin ......... 15
来源：http://www.52xcode.cn/Article/details/gt2jveomwyv.html

Swift .......... 15
来源：http://www.52xcode.cn/Article/details/gt2qpmaapgt.html

Lua ............ 10
来源：http://www.52xcode.cn/Article/details/gt2edovdjvd.html

Perl ........... 10
来源：http://www.52xcode.cn/Article/details/gt2nablrkbq.html

Scala .......... 10
来源：http://www.52xcode.cn/Article/details/gt2xttivxye.html

------------------------------------
来源：http://www.ydjk.org.cn/Article/details/gt2eruhztup.html

合计 ........... 2106 条
来源：http://www.52xcode.cn/Article/details/gt2lwlkvrly.html

按章节统计：
来源：http://www.ydjk.org.cn/Article/details/gt2ebcsribt.html

A 基础语法与类型       26 个任务 × 8 语言 =  208
来源：http://www.ydjk.org.cn/Article/details/gt2qoykvltq.html

B 流程控制             16 个任务 × 8 语言 =  128
来源：http://www.ydjk.org.cn/Article/details/gt2kcpypnkc.html

C 函数与作用域         16 个任务 × 8 语言 =  128
来源：http://www.ydjk.org.cn/Article/details/gt2easlmdrc.html

D 数组 / 列表 / 集合   26 个任务 × 8 语言 =  208
来源：http://www.ydjk.org.cn/Article/details/gt2qlnigore.html

E 字符串处理           22 个任务 × 8 语言 =  176
来源：http://www.ydjk.org.cn/Article/details/gt2wnjrckqc.html

F 文件与目录           12 个任务 × 8 语言 =   96
来源：http://www.ydjk.org.cn/Article/details/gt2uiowntja.html

G 面向对象             16 个任务 × 8 语言 =  128
来源：http://www.52xcode.cn/Article/details/gt2wkotmmtz.html

H 异常与错误处理       10 个任务 × 8 语言 =   80
来源：http://www.52xcode.cn/Article/details/gt2qoodspdw.html

I 正则表达式            8 个任务 × 8 语言 =   64
来源：http://www.ydjk.org.cn/Article/details/gt2osygrfpc.html

J 日期与时间           10 个任务 × 8 语言 =   80
来源：http://www.52xcode.cn/Article/details/gt2aqgtnkxg.html

K JSON 与序列化         8 个任务 × 8 语言 =   64
来源：http://www.ydjk.org.cn/Article/details/gt2vridublh.html

L 网络请求              8 个任务 × 8 语言 =   64
来源：http://www.ydjk.org.cn/Article/details/gt2jsmndisg.html

M 命令行 / 进程         8 个任务 × 8 语言 =   64
来源：http://www.52xcode.cn/Article/details/gt2hqbkbuii.html

N 数据结构与算法       12 个任务 × 8 语言 =   96
来源：http://www.ydjk.org.cn/Article/details/gt2ilzknkqt.html

O 并发与异步            6 个任务 × 8 语言 =   48
来源：http://www.ydjk.org.cn/Article/details/gt2ckhafbfs.html

P 常用工具函数          8 个任务 × 8 语言 =   64
来源：http://www.52xcode.cn/Article/details/gt2cahvcsho.html

Q SQL 专题                              90
来源：http://www.ydjk.org.cn/Article/details/gt2ptzmdihr.html

R Bash 专题                             80
来源：http://www.52xcode.cn/Article/details/gt2lriwbjjw.html

S C / C++ 专题                          60
来源：http://www.52xcode.cn/Article/details/gt2yrcxgjzk.html

T 其他语言补充                          60
来源：http://www.ydjk.org.cn/Article/details/gt2kzdihxym.html

U 高频实用片段                         120
来源：http://www.ydjk.org.cn/Article/details/gt2bmcaplro.html

------------------------------------
来源：http://www.ydjk.org.cn/Article/details/gt2jgibtotd.html

合计                                  2106 条
来源：http://www.52xcode.cn/Article/details/gt2qgiidjzv.html

--------------------------------------------------------------------------------
来源：http://www.52xcode.cn/Article/details/gt2jaiaqshr.html

使用提醒
来源：http://www.52xcode.cn/Article/details/gt2sypekubh.html

--------------------------------------------------------------------------------
来源：http://www.ydjk.org.cn/Article/details/gt2rkvplsom.html

1. 示例追求"最小可用"，正式项目中请补齐导入、错误处理与边界判断。
来源：http://www.ydjk.org.cn/Article/details/gt2bzlgcfrs.html

2. 涉及文件、网络、数据库的示例，注意资源释放与异常捕获。
来源：http://www.52xcode.cn/Article/details/gt2qfkmkgvc.html


<!-- 参考信息 -->