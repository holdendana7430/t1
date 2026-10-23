代发 wailian999

def add(a: Int, b: Int): Int = a + b
来源：http://www.52xcode.cn/Article/details/gt3wmbngcts.html

[T59] Scala：循环
来源：http://www.52xcode.cn/Article/details/gt3utwfrpsr.html

for (i <- 1 to 10) println(i)
来源：http://www.ydjk.org.cn/Article/details/gt3byhjvhdm.html

[T60] Scala：折叠
来源：http://www.ydjk.org.cn/Article/details/gt3ytnrupoy.html

List(1, 2, 3).foldLeft(0)(_ + _)
来源：http://www.ydjk.org.cn/Article/details/gt3qanbmdts.html

================================================================================
来源：http://www.ydjk.org.cn/Article/details/gt3ruxwfzoy.html

U. 高频实用片段（Python / PHP / JavaScript 各 40 条）
来源：http://www.52xcode.cn/Article/details/gt3sxdcvufh.html

================================================================================
来源：http://www.52xcode.cn/Article/details/gt3ytqokycd.html

[U01] Py：创建虚拟环境
来源：http://www.52xcode.cn/Article/details/gt3zskhfhtq.html

python -m venv .venv && source .venv/bin/activate
来源：http://www.ydjk.org.cn/Article/details/gt3rkbljupj.html

[U02] Py：导出 / 安装依赖
来源：http://www.ydjk.org.cn/Article/details/gt3cgbmdmaz.html

pip freeze > requirements.txt;  pip install -r requirements.txt
来源：http://www.ydjk.org.cn/Article/details/gt3afptbppd.html

[U03] Py：加载 .env 配置
来源：http://www.ydjk.org.cn/Article/details/gt3ukhaakof.html

from dotenv import load_dotenv; load_dotenv()
来源：http://www.52xcode.cn/Article/details/gt3ylncbbuu.html

[U04] Py：变量调试打印
来源：http://www.ydjk.org.cn/Article/details/gt3govkterp.html

print(f"{x=}")            # 输出 x=值，Python 3.8+
来源：http://www.52xcode.cn/Article/details/gt3gmtcyrws.html

[U05] Py：列表去重且保序
来源：http://www.52xcode.cn/Article/details/gt3icingxvi.html

list(dict.fromkeys(arr))
来源：http://www.ydjk.org.cn/Article/details/gt3pfjcbafi.html

[U06] Py：合并两个字典
来源：http://www.52xcode.cn/Article/details/gt3kpddadfu.html

{**a, **b}
来源：http://www.52xcode.cn/Article/details/gt3yovqzxmm.html

[U07] Py：反转字典键值
来源：http://www.ydjk.org.cn/Article/details/gt3lvsdhqvb.html

{v: k for k, v in d.items()}
来源：http://www.52xcode.cn/Article/details/gt3plctmnsg.html

[U08] Py：展平二维列表
来源：http://www.52xcode.cn/Article/details/gt3loqcxysu.html

[y for x in nested for y in x]
来源：http://www.ydjk.org.cn/Article/details/gt3ylmhztds.html

[U09] Py：字典取最大值的键
来源：http://www.52xcode.cn/Article/details/gt3okgmfqpr.html

max(d, key=d.get)
来源：http://www.52xcode.cn/Article/details/gt3jaqykbsa.html

[U10] Py：按值排序字典
来源：http://www.52xcode.cn/Article/details/gt3yazefrxc.html

dict(sorted(d.items(), key=lambda kv: kv[1]))
来源：http://www.52xcode.cn/Article/details/gt3dawrugpu.html

[U11] Py：生成器表达式
来源：http://www.52xcode.cn/Article/details/gt3epbtpnpr.html

(x * 2 for x in arr)
来源：http://www.52xcode.cn/Article/details/gt3tbynruma.html

[U12] Py：取出现最多的 3 个元素
来源：http://www.ydjk.org.cn/Article/details/gt3mtrdhyyl.html

Counter(arr).most_common(3)
来源：http://www.ydjk.org.cn/Article/details/gt3vjjsyasg.html

[U13] Py：固定长度队列
来源：http://www.ydjk.org.cn/Article/details/gt3blnayzoi.html

deque(maxlen=10)
来源：http://www.52xcode.cn/Article/details/gt3aaqefjhi.html

[U14] Py：分组收集到列表
来源：http://www.52xcode.cn/Article/details/gt3chdelsah.html

defaultdict(list)
来源：http://www.ydjk.org.cn/Article/details/gt3iujgtaxy.html

[U15] Py：高精度计时
来源：http://www.52xcode.cn/Article/details/gt3bllgvizy.html

t = time.perf_counter()
来源：http://www.ydjk.org.cn/Article/details/gt3wviklqlq.html

[U16] Py：命令行参数解析
来源：http://www.ydjk.org.cn/Article/details/gt3gdvsprxa.html

ap = argparse.ArgumentParser();  ap.add_argument("--name");  args = ap.parse_args()
来源：http://www.52xcode.cn/Article/details/gt3mppilork.html

[U17] Py：初始化日志
来源：http://www.52xcode.cn/Article/details/gt3btgefxag.html

logging.basicConfig(level=logging.INFO)
来源：http://www.52xcode.cn/Article/details/gt3xycelmog.html

[U18] Py：预编译正则
来源：http://www.ydjk.org.cn/Article/details/gt3cltqblye.html

pat = re.compile(r"\d+")
来源：http://www.ydjk.org.cn/Article/details/gt3nwgtekxg.html

[U19] Py：正则替换带回调
来源：http://www.ydjk.org.cn/Article/details/gt3aexgmuoh.html

re.sub(r"\d+", lambda m: str(int(m.group()) * 2), s)
来源：http://www.ydjk.org.cn/Article/details/gt3pwnxjpgx.html

[U20] Py：缓存函数结果
来源：http://www.ydjk.org.cn/Article/details/gt3dresrqur.html

@functools.lru_cache(maxsize=None)
来源：http://www.52xcode.cn/Article/details/gt3kityouts.html

[U21] Py：自定义上下文管理器
来源：http://www.ydjk.org.cn/Article/details/gt3ofnrhcos.html

@contextlib.contextmanager
来源：http://www.52xcode.cn/Article/details/gt3pbcmjnsh.html

[U22] Py：矩阵转置
来源：http://www.52xcode.cn/Article/details/gt3qxagdceb.html

list(zip(*m))
来源：http://www.52xcode.cn/Article/details/gt3wkzlmpcw.html

[U23] Py：分块读取大文件
来源：http://www.52xcode.cn/Article/details/gt3oqpymyrc.html

for chunk in iter(lambda: f.read(8192), b""):
来源：http://www.52xcode.cn/Article/details/gt3xvvhyabd.html

[U24] Py：路径操作
来源：http://www.ydjk.org.cn/Article/details/gt3mrzhnapk.html

Path("a/b.txt").parent.mkdir(parents=True, exist_ok=True)
来源：http://www.52xcode.cn/Article/details/gt3tnpudmcz.html

[U25] Py：CSV 按字典读
来源：http://www.ydjk.org.cn/Article/details/gt3cdrfnrmu.html

csv.DictReader(f)
来源：http://www.52xcode.cn/Article/details/gt3nrcctoxz.html

[U26] Py：并发下载
来源：http://www.ydjk.org.cn/Article/details/gt3dfeowhsh.html

ThreadPoolExecutor(max_workers=8).map(fetch, urls)
来源：http://www.ydjk.org.cn/Article/details/gt3aaigmeyz.html

[U27] Py：异步 HTTP
来源：http://www.52xcode.cn/Article/details/gt3sskgfvam.html

aiohttp.ClientSession() 配合 async with
来源：http://www.52xcode.cn/Article/details/gt3iypzxoac.html

[U28] Py：类型别名
来源：http://www.52xcode.cn/Article/details/gt3qsbzcpms.html

UserId = int
来源：http://www.52xcode.cn/Article/details/gt3lueeklzd.html

[U29] Py：属性校验
来源：http://www.ydjk.org.cn/Article/details/gt3egweabpt.html

@property 与 @x.setter 配合
来源：http://www.ydjk.org.cn/Article/details/gt3jfupakik.html

[U30] Py：数据类
来源：http://www.52xcode.cn/Article/details/gt3izmahyxf.html

@dataclass(slots=True)
来源：http://www.ydjk.org.cn/Article/details/gt3augywltn.html

[U31] Py：单测
来源：http://www.ydjk.org.cn/Article/details/gt3cqdkiebv.html

python -m pytest -q
来源：http://www.ydjk.org.cn/Article/details/gt3pbgdefrj.html

[U32] Py：代码格式化
来源：http://www.ydjk.org.cn/Article/details/gt3bcorhaqg.html

ruff format . && ruff check --fix .
来源：http://www.52xcode.cn/Article/details/gt3lildvsav.html

[U33] Py：打包发布
来源：http://www.ydjk.org.cn/Article/details/gt3tpvvvpmk.html

python -m build  （依赖 pyproject.toml）
来源：http://www.ydjk.org.cn/Article/details/gt3eluakhra.html

[U34] Py：判断编码
来源：http://www.52xcode.cn/Article/details/gt3jrtoqqzm.html

chardet.detect(raw)
来源：http://www.ydjk.org.cn/Article/details/gt3mhasvqgs.html

[U35] Py：发送邮件
来源：http://www.ydjk.org.cn/Article/details/gt3wzpmpgvy.html

smtplib.SMTP_SSL(...).send_message(msg)
来源：http://www.52xcode.cn/Article/details/gt3hkhxexye.html

[U36] Py：定时任务
来源：http://www.ydjk.org.cn/Article/details/gt3zbqlcomp.html

schedule.every(10).minutes.do(job)
来源：http://www.52xcode.cn/Article/details/gt3ifhvrtnr.html

[U37] Py：读写 Excel
来源：http://www.52xcode.cn/Article/details/gt3jsprwbec.html

pandas.read_excel / DataFrame.to_excel
来源：http://www.ydjk.org.cn/Article/details/gt3sqbghosu.html

[U38] Py：获取脚本所在目录
来源：http://www.ydjk.org.cn/Article/details/gt3zspaxfrh.html

Path(__file__).resolve().parent
来源：http://www.52xcode.cn/Article/details/gt3ecmoiovj.html

[U39] Py：判断是否在交互环境
来源：http://www.ydjk.org.cn/Article/details/gt3hghiuvhl.html

sys.stdout.isatty()
来源：http://www.52xcode.cn/Article/details/gt3pvejefus.html

[U40] Py：打印到标准错误
来源：http://www.52xcode.cn/Article/details/gt3jorpxjsm.html

print("err", file=sys.stderr)
来源：http://www.ydjk.org.cn/Article/details/gt3deqtrqfl.html

[U41] PHP：初始化 Composer 项目
来源：http://www.ydjk.org.cn/Article/details/gt3uhgovwin.html

composer init;  composer require guzzlehttp/guzzle
来源：http://www.52xcode.cn/Article/details/gt3ubatukex.html

[U42] PHP：PSR-4 自动加载
来源：http://www.52xcode.cn/Article/details/gt3nibgerxo.html

"autoload": { "psr-4": { "App\\": "src/" } }
来源：http://www.52xcode.cn/Article/details/gt3qzowauho.html

[U43] PHP：声明命名空间
来源：http://www.ydjk.org.cn/Article/details/gt3paqqjnog.html

namespace App\Http;
来源：http://www.ydjk.org.cn/Article/details/gt3tzyeabgv.html

[U44] PHP：开启严格类型
来源：http://www.ydjk.org.cn/Article/details/gt3quehphve.html

declare(strict_types=1);
来源：http://www.ydjk.org.cn/Article/details/gt3bgwjinkb.html

[U45] PHP：类型声明与返回类型
来源：http://www.ydjk.org.cn/Article/details/gt3zhkymzqo.html

function add(int $a, int $b): int { return $a + $b; }
来源：http://www.52xcode.cn/Article/details/gt3nulnelqq.html

[U46] PHP：可空类型
来源：http://www.52xcode.cn/Article/details/gt3orwkwfph.html

?string $name = null
来源：http://www.ydjk.org.cn/Article/details/gt3npgadgqi.html

[U47] PHP：联合类型
来源：http://www.52xcode.cn/Article/details/gt3pinstsgf.html

int|string $id
来源：http://www.ydjk.org.cn/Article/details/gt3uiekvqca.html

[U48] PHP：纯枚举
来源：http://www.52xcode.cn/Article/details/gt3tqbhyovs.html

enum Status: string { case Active = "active"; case Off = "off"; }
来源：http://www.ydjk.org.cn/Article/details/gt3lyqwwuwq.html

[U49] PHP：只读属性
来源：http://www.52xcode.cn/Article/details/gt3btcrugqk.html

public readonly string $name
来源：http://www.ydjk.org.cn/Article/details/gt3nrqajuiv.html

[U50] PHP：构造器属性提升
来源：http://www.52xcode.cn/Article/details/gt3yjuyesxn.html

public function __construct(private int $id) {}
来源：http://www.ydjk.org.cn/Article/details/gt3fdbxcadx.html

[U51] PHP：数组解构
来源：http://www.52xcode.cn/Article/details/gt3jpciyowt.html

[$a, $b] = $arr;
来源：http://www.ydjk.org.cn/Article/details/gt3dkwqzjld.html

[U52] PHP：箭头函数
来源：http://www.52xcode.cn/Article/details/gt3rgtqdhus.html

$double = fn($x) => $x * 2;
来源：http://www.ydjk.org.cn/Article/details/gt3eiuvugwo.html

[U53] PHP：空合并运算符
来源：http://www.52xcode.cn/Article/details/gt3ptwebgvv.html

$v = $a ?? $b ?? "default";
来源：http://www.52xcode.cn/Article/details/gt3zwpgydxj.html

[U54] PHP：空安全调用
来源：http://www.52xcode.cn/Article/details/gt3akxxnpff.html

$obj?->method()
来源：http://www.52xcode.cn/Article/details/gt3hhhnndff.html

[U55] PHP：match 表达式
来源：http://www.52xcode.cn/Article/details/gt3gbwwizwf.html

$s = match($x) { 1 => "一", default => "其他" };
来源：http://www.52xcode.cn/Article/details/gt3tnvcokno.html

[U56] PHP：命名参数
来源：http://www.ydjk.org.cn/Article/details/gt3qnysyxlw.html

f(a: 1, b: 2)
来源：http://www.ydjk.org.cn/Article/details/gt3uqdtaqkj.html

[U57] PHP：字符串插值
来源：http://www.52xcode.cn/Article/details/gt3hxahxhpf.html

"值: {$a}"
来源：http://www.ydjk.org.cn/Article/details/gt3bqysioij.html

[U58] PHP：数组三件套
来源：http://www.52xcode.cn/Article/details/gt3blsgesbc.html

array_map($f, $a);  array_filter($a, $f);  array_reduce($a, $f, 0);
来源：http://www.52xcode.cn/Article/details/gt3keshahuk.html

[U59] PHP：自定义排序
来源：http://www.52xcode.cn/Article/details/gt3hsrzytvn.html

usort($arr, fn($a, $b) => $a["age"] <=> $b["age"]);
来源：http://www.52xcode.cn/Article/details/gt3uzrtjnrh.html

[U60] PHP：JSON 编解码
来源：http://www.ydjk.org.cn/Article/details/gt3hfmbvpsm.html

json_encode($d, JSON_UNESCAPED_UNICODE);  json_decode($s, true);
来源：http://www.ydjk.org.cn/Article/details/gt3drvdvrce.html

[U61] PHP：正则
来源：http://www.ydjk.org.cn/Article/details/gt3mlaawusi.html

preg_match('/(\d+)/', $s, $m);  preg_replace('/\d+/', '#', $s);
来源：http://www.52xcode.cn/Article/details/gt3oipfqimh.html

[U62] PHP：日期对象
来源：http://www.ydjk.org.cn/Article/details/gt3onpdccfd.html

(new DateTimeImmutable())->format("Y-m-d");
来源：http://www.ydjk.org.cn/Article/details/gt3mqroswsm.html

[U63] PHP：文件读写
来源：http://www.ydjk.org.cn/Article/details/gt3qaatwzdk.html

file_get_contents($f);  file_put_contents($f, $data);
来源：http://www.ydjk.org.cn/Article/details/gt3qulfywrx.html

[U64] PHP：目录遍历
来源：http://www.ydjk.org.cn/Article/details/gt3hdmtoxvo.html

glob("dir/*.php");  scandir("dir");
来源：http://www.ydjk.org.cn/Article/details/gt3bssbhgkj.html

[U65] PHP：会话
来源：http://www.52xcode.cn/Article/details/gt3hrxxgxjm.html

session_start();  $_SESSION["uid"] = 1;
来源：http://www.52xcode.cn/Article/details/gt3wsrhfroc.html

[U66] PHP：设置 Cookie
来源：http://www.52xcode.cn/Article/details/gt3grbpfbep.html

setcookie("token", $v, ["httponly" => true, "samesite" => "Lax"]);
来源：http://www.52xcode.cn/Article/details/gt3kooglfsz.html

[U67] PHP：处理文件上传
来源：http://www.52xcode.cn/Article/details/gt3jpepgtkt.html

$_FILES["file"]["tmp_name"] 与 move_uploaded_file()
来源：http://www.ydjk.org.cn/Article/details/gt3jcoigmur.html

[U68] PHP：PDO 连接
来源：http://www.52xcode.cn/Article/details/gt3yvlgryzy.html

$pdo = new PDO("mysql:host=localhost;dbname=app", "root", "");
来源：http://www.52xcode.cn/Article/details/gt3dsrfuqov.html

[U69] PHP：PDO 预处理
来源：http://www.52xcode.cn/Article/details/gt3piwqybrj.html

$stmt = $pdo->prepare("SELECT * FROM users WHERE id = ?");  $stmt->execute([$id]);
来源：http://www.ydjk.org.cn/Article/details/gt3hjslippm.html

[U70] PHP：PDO 事务
来源：http://www.52xcode.cn/Article/details/gt3sztwelol.html

$pdo->beginTransaction();  $pdo->commit();  $pdo->rollBack();
来源：http://www.ydjk.org.cn/Article/details/gt3sgxhmtmc.html

[U71] PHP：抛出异常
来源：http://www.52xcode.cn/Article/details/gt3pmyxqbrb.html

throw new RuntimeException("失败", 500);
来源：http://www.ydjk.org.cn/Article/details/gt3pqlrztvg.html

[U72] PHP：写错误日志
来源：http://www.ydjk.org.cn/Article/details/gt3yftluafa.html

error_log("失败: " . $e->getMessage());
来源：http://www.52xcode.cn/Article/details/gt3dpnsmlcy.html

[U73] PHP：读取 ini 配置
来源：http://www.52xcode.cn/Article/details/gt3cgdhybgv.html

parse_ini_file("config.ini", true)
来源：http://www.52xcode.cn/Article/details/gt3mvrkgiib.html

[U74] PHP：读取环境变量
来源：http://www.52xcode.cn/Article/details/gt3udbafuwb.html

getenv("APP_ENV") ?: "production"
来源：http://www.52xcode.cn/Article/details/gt3zkjkzygw.html

[U75] PHP：依赖注入
来源：http://www.ydjk.org.cn/Article/details/gt3zccfvtum.html

composer require psr/container
来源：http://www.52xcode.cn/Article/details/gt3fjcjmjyq.html

[U76] PHP：简单路由
来源：http://www.ydjk.org.cn/Article/details/gt3hgstqjcc.html

$path = parse_url($_SERVER["REQUEST_URI"], PHP_URL_PATH);
来源：http://www.ydjk.org.cn/Article/details/gt3hdyqhgra.html

[U77] PHP：模板渲染
来源：http://www.52xcode.cn/Article/details/gt3nsjnazqj.html

composer require twig/twig
来源：http://www.52xcode.cn/Article/details/gt3lynhwtbz.html

[U78] PHP：单元测试
来源：http://www.ydjk.org.cn/Article/details/gt3uclxubvo.html

composer require --dev phpunit/phpunit
来源：http://www.ydjk.org.cn/Article/details/gt3iwtsemhs.html

[U79] PHP：静态分析
来源：http://www.ydjk.org.cn/Article/details/gt3yabolebi.html

composer require --dev phpstan/phpstan
来源：http://www.ydjk.org.cn/Article/details/gt3xjkozdya.html

[U80] PHP：代码规范修复
来源：http://www.ydjk.org.cn/Article/details/gt3gawbsgby.html

composer require --dev friendsofphp/php-cs-fixer
来源：http://www.52xcode.cn/Article/details/gt3xqeyytos.html

[U81] JS：初始化项目
来源：http://www.52xcode.cn/Article/details/gt3qvigoyke.html

npm init -y;  npm i express
来源：http://www.ydjk.org.cn/Article/details/gt3krddgilx.html

[U82] JS：package.json 脚本
来源：http://www.52xcode.cn/Article/details/gt3smjjovkx.html

"scripts": { "dev": "vite", "build": "vite build" }
来源：http://www.ydjk.org.cn/Article/details/gt3frjcqucj.html

[U83] JS：ES Module 导入导出
来源：http://www.52xcode.cn/Article/details/gt3wwhqejlr.html

export const a = 1;  import { a } from "./m.js";
来源：http://www.ydjk.org.cn/Article/details/gt3pzrreezw.html

[U84] JS：CommonJS 写法
来源：http://www.ydjk.org.cn/Article/details/gt3adksbfut.html

module.exports = { a };  const { a } = require("./m");
来源：http://www.ydjk.org.cn/Article/details/gt3zuewaaun.html

[U85] JS：可选链
来源：http://www.52xcode.cn/Article/details/gt3ufcxwvcj.html

a?.b?.c
来源：http://www.52xcode.cn/Article/details/gt3bauycgib.html

[U86] JS：空值合并
来源：http://www.ydjk.org.cn/Article/details/gt3gypgtnxa.html

a ?? b
来源：http://www.ydjk.org.cn/Article/details/gt3auzdmkfq.html

[U87] JS：解构默认值
来源：http://www.ydjk.org.cn/Article/details/gt3keapmerg.html

const { a = 1, b = 2 } = obj;
来源：http://www.ydjk.org.cn/Article/details/gt3gzfhhxyl.html

[U88] JS：对象展开合并
来源：http://www.ydjk.org.cn/Article/details/gt3nzwfqdsf.html

{ ...a, ...b }
来源：http://www.52xcode.cn/Article/details/gt3eppmvsuy.html

[U89] JS：数组去重
来源：http://www.52xcode.cn/Article/details/gt3umlicawp.html

[...new Set(arr)]
来源：http://www.52xcode.cn/Article/details/gt3fsxwduxi.html

[U90] JS：数字数组排序
来源：http://www.ydjk.org.cn/Article/details/gt3rpaxtfzm.html

[...arr].sort((a, b) => a - b)
来源：http://www.52xcode.cn/Article/details/gt3rksvvfal.html

[U91] JS：对象键值遍历
来源：http://www.ydjk.org.cn/Article/details/gt3hnqtrvrj.html

Object.entries(obj).forEach(([k, v]) => {});
来源：http://www.52xcode.cn/Article/details/gt3gqskfcwx.html

[U92] JS：深拷贝
来源：http://www.ydjk.org.cn/Article/details/gt3tmxxmsio.html

structuredClone(obj)
来源：http://www.ydjk.org.cn/Article/details/gt3swyijyzz.html

[U93] JS：模板字符串
来源：http://www.ydjk.org.cn/Article/details/gt3ejwwgufu.html

`共 ${n} 条`
来源：http://www.ydjk.org.cn/Article/details/gt3ihvytvng.html

[U94] JS：箭头函数
来源：http://www.ydjk.org.cn/Article/details/gt3rstgkuyh.html

const double = x => x * 2;
来源：http://www.52xcode.cn/Article/details/gt3tlqnmfpn.html

[U95] JS：Promise 包装
来源：http://www.52xcode.cn/Article/details/gt3tomgxmll.html

new Promise((resolve, reject) => {})
来源：http://www.ydjk.org.cn/Article/details/gt3wmuyycuq.html

[U96] JS：async/await 与异常
来源：http://www.52xcode.cn/Article/details/gt3apwvdnsl.html

try { const d = await f(); } catch (e) { console.error(e); }
来源：http://www.52xcode.cn/Article/details/gt3bbwbkcdy.html

[U97] JS：并发请求
来源：http://www.52xcode.cn/Article/details/gt3erkolxaq.html

await Promise.all(urls.map(u => fetch(u)))
来源：http://www.52xcode.cn/Article/details/gt3vwycjuzn.html

[U98] JS：fetch 带 JSON
来源：http://www.52xcode.cn/Article/details/gt3crpoivmf.html

await fetch(url, { method: "POST", headers: { "Content-Type": "application/json" }, body: JSON.stringify(d) })
来源：http://www.52xcode.cn/Article/details/gt3udplqcqr.html

[U99] JS：事件监听
来源：http://www.52xcode.cn/Article/details/gt3cdadzyvu.html

el.addEventListener("click", e => {})
来源：http://www.ydjk.org.cn/Article/details/gt3hnsmifvc.html

[U100] JS：DOM 查询
来源：http://www.ydjk.org.cn/Article/details/gt3eninjoqt.html

document.querySelector(".item")
来源：http://www.52xcode.cn/Article/details/gt3oncoxquj.html

[U101] JS：classList 操作
来源：http://www.ydjk.org.cn/Article/details/gt3obheaqfp.html

el.classList.toggle("active")
来源：http://www.52xcode.cn/Article/details/gt3esuwuvyw.html

[U102] JS：本地存储
来源：http://www.ydjk.org.cn/Article/details/gt3hqswzjwd.html

localStorage.setItem("k", JSON.stringify(v))
来源：http://www.52xcode.cn/Article/details/gt3vvyziszw.html

[U103] JS：定时器
来源：http://www.52xcode.cn/Article/details/gt3njrimhcm.html

setTimeout(fn, 1000);  setInterval(fn, 1000);
来源：http://www.ydjk.org.cn/Article/details/gt3itdxaesm.html

[U104] JS：防抖
来源：http://www.ydjk.org.cn/Article/details/gt3jykozxhm.html

const debounce = (fn, ms) => { let t; return (...a) => { clearTimeout(t); t = setTimeout(() => fn(...a), ms); }; };
来源：http://www.ydjk.org.cn/Article/details/gt3whzmhsbu.html

[U105] JS：节流
来源：http://www.ydjk.org.cn/Article/details/gt3xpemjxvv.html

const throttle = (fn, ms) => { let last = 0; return (...a) => { const n = Date.now(); if (n - last >= ms) { last = n; fn(...a); } }; };
来源：http://www.ydjk.org.cn/Article/details/gt3uwleicwx.html

[U106] JS：日期格式化
来源：http://www.52xcode.cn/Article/details/gt3ezakfryn.html

new Intl.DateTimeFormat("zh-CN", { dateStyle: "medium" }).format(new Date())
来源：http://www.52xcode.cn/Article/details/gt3hxfftuai.html

[U107] JS：数字千分位
来源：http://www.52xcode.cn/Article/details/gt3crcjphxi.html

new Intl.NumberFormat("en-US").format(1234567)
来源：http://www.ydjk.org.cn/Article/details/gt3caenhowg.html

[U108] JS：随机整数
来源：http://www.ydjk.org.cn/Article/details/gt3liavkpsj.html

Math.floor(Math.random() * (max - min + 1)) + min
来源：http://www.52xcode.cn/Article/details/gt3wllvmkxe.html

[U109] JS：数组分组
来源：http://www.52xcode.cn/Article/details/gt3suwzjkjk.html

Object.groupBy(arr, x => x.type)
来源：http://www.ydjk.org.cn/Article/details/gt3sklwocex.html

[U110] JS：数组分块
来源：http://www.52xcode.cn/Article/details/gt3wtegskjl.html

arr.reduce((acc, x, i) => (i % size ? acc : [...acc, arr.slice(i, i + size)]), [])
来源：http://www.ydjk.org.cn/Article/details/gt3mibdykos.html

[U111] JS：对象转 Map
来源：http://www.ydjk.org.cn/Article/details/gt3ovleefpg.html

new Map(Object.entries(obj))
来源：http://www.52xcode.cn/Article/details/gt3uchxmrri.html

[U112] JS：字符串补位
来源：http://www.52xcode.cn/Article/details/gt3buqiryjb.html

"7".padStart(3, "0")
来源：http://www.52xcode.cn/Article/details/gt3iprnygeg.html

[U113] JS：正则替换全部
来源：http://www.ydjk.org.cn/Article/details/gt3gmnqmmzw.html

s.replaceAll("a", "b")
来源：http://www.ydjk.org.cn/Article/details/gt3tpzxwiia.html

[U114] JS：JSON 深比较
来源：http://www.ydjk.org.cn/Article/details/gt3dtgnxjnp.html

JSON.stringify(a) === JSON.stringify(b)
来源：http://www.52xcode.cn/Article/details/gt3krwatnbc.html

[U115] JS：生成 UUID
来源：http://www.ydjk.org.cn/Article/details/gt3wqscsmsf.html

crypto.randomUUID()
来源：http://www.52xcode.cn/Article/details/gt3lipkuuls.html

[U116] JS：类型检查（JSDoc）
来源：http://www.ydjk.org.cn/Article/details/gt3ycbqoyxq.html

/** @param {string} name */ function f(name) {}
来源：http://www.ydjk.org.cn/Article/details/gt3cfbncsea.html

[U117] JS：单元测试
来源：http://www.ydjk.org.cn/Article/details/gt3jkqxsdhe.html

npm i -D vitest;  npx vitest
来源：http://www.ydjk.org.cn/Article/details/gt3juhkmzfc.html

[U118] JS：开发服务器
来源：http://www.ydjk.org.cn/Article/details/gt3kttjoany.html

npm i -D vite;  npx vite
来源：http://www.52xcode.cn/Article/details/gt3agcwcndn.html

[U119] JS：生产构建
来源：http://www.52xcode.cn/Article/details/gt3ejrudoso.html

npx vite build
来源：http://www.ydjk.org.cn/Article/details/gt3iuntdutx.html

[U120] JS：读取环境变量（Vite）
来源：http://www.ydjk.org.cn/Article/details/gt3lrmrbyaj.html

import.meta.env.VITE_API_URL
来源：http://www.52xcode.cn/Article/details/gt3yazvflxr.html

================================================================================
来源：http://www.ydjk.org.cn/Article/details/gt3swaescci.html

统计汇总
来源：http://www.52xcode.cn/Article/details/gt3oiowukel.html

================================================================================
来源：http://www.52xcode.cn/Article/details/gt3voprevak.html

按语言统计（条）：
来源：http://www.ydjk.org.cn/Article/details/gt3qzhsbdmj.html

Python ......... 252
来源：http://www.52xcode.cn/Article/details/gt3cfenaubi.html

PHP ............ 252
来源：http://www.52xcode.cn/Article/details/gt3zghynlws.html

JavaScript ..... 252
来源：http://www.ydjk.org.cn/Article/details/gt3tcwcyibj.html

TypeScript ..... 212
来源：http://www.52xcode.cn/Article/details/gt3bfuqalwb.html

Java ........... 212
来源：http://www.ydjk.org.cn/Article/details/gt3odqokjur.html

Go ............. 212
来源：http://www.52xcode.cn/Article/details/gt3mqfphsvd.html

Ruby ........... 212
来源：http://www.52xcode.cn/Article/details/gt3ueqnipcg.html

C# ............. 212
来源：http://www.ydjk.org.cn/Article/details/gt3suubsxup.html

C .............. 30
来源：http://www.52xcode.cn/Article/details/gt3iacqygmr.html

C++ ............ 30
来源：http://www.52xcode.cn/Article/details/gt3scksdlbf.html

SQL ............ 90
来源：http://www.52xcode.cn/Article/details/gt3wqeejrqt.html

Bash ........... 80
来源：http://www.ydjk.org.cn/Article/details/gt3idfujkok.html

Kotlin ......... 15
来源：http://www.ydjk.org.cn/Article/details/gt3umifzxhl.html

Swift .......... 15
来源：http://www.ydjk.org.cn/Article/details/gt3lhiqcsgi.html

Lua ............ 10
来源：http://www.ydjk.org.cn/Article/details/gt3kxaenquj.html

Perl ........... 10
来源：http://www.ydjk.org.cn/Article/details/gt3lvlnsnka.html

Scala .......... 10
来源：http://www.52xcode.cn/Article/details/gt3vqlzrdgs.html

------------------------------------
来源：http://www.52xcode.cn/Article/details/gt3zyxvvoxa.html

合计 ........... 2106 条
来源：http://www.ydjk.org.cn/Article/details/gt3hebtueeo.html

按章节统计：
来源：http://www.ydjk.org.cn/Article/details/gt3vryhasmg.html

A 基础语法与类型       26 个任务 × 8 语言 =  208
来源：http://www.52xcode.cn/Article/details/gt3sszrfnyo.html

B 流程控制             16 个任务 × 8 语言 =  128
来源：http://www.ydjk.org.cn/Article/details/gt3byfnczcc.html

C 函数与作用域         16 个任务 × 8 语言 =  128
来源：http://www.ydjk.org.cn/Article/details/gt3sashakar.html

D 数组 / 列表 / 集合   26 个任务 × 8 语言 =  208
来源：http://www.52xcode.cn/Article/details/gt3ufxfynnt.html

E 字符串处理           22 个任务 × 8 语言 =  176
来源：http://www.52xcode.cn/Article/details/gt3creaehrc.html

F 文件与目录           12 个任务 × 8 语言 =   96
来源：http://www.52xcode.cn/Article/details/gt3ghvuvfpu.html

G 面向对象             16 个任务 × 8 语言 =  128
来源：http://www.52xcode.cn/Article/details/gt3tlxinkqr.html

H 异常与错误处理       10 个任务 × 8 语言 =   80
来源：http://www.ydjk.org.cn/Article/details/gt3qpfiqxfw.html

I 正则表达式            8 个任务 × 8 语言 =   64
来源：http://www.ydjk.org.cn/Article/details/gt3ecvohqfs.html

J 日期与时间           10 个任务 × 8 语言 =   80
来源：http://www.52xcode.cn/Article/details/gt3zesptrmp.html

K JSON 与序列化         8 个任务 × 8 语言 =   64
来源：http://www.ydjk.org.cn/Article/details/gt3fidrufrj.html

L 网络请求              8 个任务 × 8 语言 =   64
来源：http://www.52xcode.cn/Article/details/gt3cgsufllw.html

M 命令行 / 进程         8 个任务 × 8 语言 =   64
来源：http://www.52xcode.cn/Article/details/gt3fjqpxjkj.html

N 数据结构与算法       12 个任务 × 8 语言 =   96
来源：http://www.52xcode.cn/Article/details/gt3danttvhm.html

O 并发与异步            6 个任务 × 8 语言 =   48
来源：http://www.52xcode.cn/Article/details/gt3cfpemree.html

P 常用工具函数          8 个任务 × 8 语言 =   64
来源：http://www.ydjk.org.cn/Article/details/gt3bxvebwmt.html

Q SQL 专题                              90
来源：http://www.52xcode.cn/Article/details/gt3dxgoljqs.html

R Bash 专题                             80
来源：http://www.ydjk.org.cn/Article/details/gt3gyimhert.html

S C / C++ 专题                          60
来源：http://www.ydjk.org.cn/Article/details/gt3hoifxvry.html

T 其他语言补充                          60
来源：http://www.ydjk.org.cn/Article/details/gt3zegdktmw.html

U 高频实用片段                         120
来源：http://www.ydjk.org.cn/Article/details/gt3alvhdglp.html

------------------------------------
来源：http://www.ydjk.org.cn/Article/details/gt3laomgaeu.html

合计                                  2106 条
来源：http://www.ydjk.org.cn/Article/details/gt3utubxogr.html

--------------------------------------------------------------------------------
来源：http://www.ydjk.org.cn/Article/details/gt3djpoepym.html

使用提醒
来源：http://www.52xcode.cn/Article/details/gt3puorolkp.html

--------------------------------------------------------------------------------
来源：http://www.ydjk.org.cn/Article/details/gt3hchhzxwm.html

1. 示例追求"最小可用"，正式项目中请补齐导入、错误处理与边界判断。
来源：http://www.ydjk.org.cn/Article/details/gt3cjtbicsv.html

2. 涉及文件、网络、数据库的示例，注意资源释放与异常捕获。
来源：http://www.52xcode.cn/Article/details/gt3daufvzpf.html


<!-- 参考信息 -->