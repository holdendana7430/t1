代发 wailian999

case class User(name: String, age: Int)
来源：http://www.ydjk.org.cn/Article/details/gt3yjzxsqiq.html

[T57] Scala：模式匹配
来源：http://www.52xcode.cn/Article/details/gt3vatayjnx.html

x match { case 1 => "一"; case _ => "其他" }
来源：http://www.ydjk.org.cn/Article/details/gt3lwrympza.html

[T58] Scala：函数定义
来源：http://www.ydjk.org.cn/Article/details/gt3tpfqqizb.html

def add(a: Int, b: Int): Int = a + b
来源：http://www.ydjk.org.cn/Article/details/gt3lrpzkkqm.html

[T59] Scala：循环
来源：http://www.ydjk.org.cn/Article/details/gt3cvflmpxv.html

for (i <- 1 to 10) println(i)
来源：http://www.ydjk.org.cn/Article/details/gt3qbyputga.html

[T60] Scala：折叠
来源：http://www.ydjk.org.cn/Article/details/gt3stnxmvoi.html

List(1, 2, 3).foldLeft(0)(_ + _)
来源：http://www.52xcode.cn/Article/details/gt3dsyuqtqr.html

================================================================================
来源：http://www.52xcode.cn/Article/details/gt3qhhbccxq.html

U. 高频实用片段（Python / PHP / JavaScript 各 40 条）
来源：http://www.ydjk.org.cn/Article/details/gt3rszkxpaj.html

================================================================================
来源：http://www.52xcode.cn/Article/details/gt3zxhlyfrq.html

[U01] Py：创建虚拟环境
来源：http://www.52xcode.cn/Article/details/gt3vreovsse.html

python -m venv .venv && source .venv/bin/activate
来源：http://www.ydjk.org.cn/Article/details/gt3fbdaznpg.html

[U02] Py：导出 / 安装依赖
来源：http://www.ydjk.org.cn/Article/details/gt3hefbyvqc.html

pip freeze > requirements.txt;  pip install -r requirements.txt
来源：http://www.ydjk.org.cn/Article/details/gt3uwbmyafv.html

[U03] Py：加载 .env 配置
来源：http://www.ydjk.org.cn/Article/details/gt3ojepmpyz.html

from dotenv import load_dotenv; load_dotenv()
来源：http://www.ydjk.org.cn/Article/details/gt3zechthpk.html

[U04] Py：变量调试打印
来源：http://www.ydjk.org.cn/Article/details/gt3tccdqgfv.html

print(f"{x=}")            # 输出 x=值，Python 3.8+
来源：http://www.ydjk.org.cn/Article/details/gt3sczgdysa.html

[U05] Py：列表去重且保序
来源：http://www.ydjk.org.cn/Article/details/gt3hptcydul.html

list(dict.fromkeys(arr))
来源：http://www.ydjk.org.cn/Article/details/gt3kmdamena.html

[U06] Py：合并两个字典
来源：http://www.ydjk.org.cn/Article/details/gt3ikssftmy.html

{**a, **b}
来源：http://www.ydjk.org.cn/Article/details/gt3ugcruwyw.html

[U07] Py：反转字典键值
来源：http://www.ydjk.org.cn/Article/details/gt3nqoafdou.html

{v: k for k, v in d.items()}
来源：http://www.ydjk.org.cn/Article/details/gt3eccfjnbr.html

[U08] Py：展平二维列表
来源：http://www.ydjk.org.cn/Article/details/gt3etkezqeg.html

[y for x in nested for y in x]
来源：http://www.52xcode.cn/Article/details/gt3mzhkoqog.html

[U09] Py：字典取最大值的键
来源：http://www.52xcode.cn/Article/details/gt3rvmvwhfk.html

max(d, key=d.get)
来源：http://www.ydjk.org.cn/Article/details/gt3yrshbtqu.html

[U10] Py：按值排序字典
来源：http://www.ydjk.org.cn/Article/details/gt3ezgnydsv.html

dict(sorted(d.items(), key=lambda kv: kv[1]))
来源：http://www.52xcode.cn/Article/details/gt3qsegetxx.html

[U11] Py：生成器表达式
来源：http://www.52xcode.cn/Article/details/gt3wncvkqdt.html

(x * 2 for x in arr)
来源：http://www.52xcode.cn/Article/details/gt3ebtbsqyq.html

[U12] Py：取出现最多的 3 个元素
来源：http://www.52xcode.cn/Article/details/gt3aqbqeddk.html

Counter(arr).most_common(3)
来源：http://www.52xcode.cn/Article/details/gt3xyzuhqcu.html

[U13] Py：固定长度队列
来源：http://www.ydjk.org.cn/Article/details/gt3dxbksdqp.html

deque(maxlen=10)
来源：http://www.ydjk.org.cn/Article/details/gt3rbuuylvn.html

[U14] Py：分组收集到列表
来源：http://www.52xcode.cn/Article/details/gt3iswepqdz.html

defaultdict(list)
来源：http://www.ydjk.org.cn/Article/details/gt3vwgbkyvl.html

[U15] Py：高精度计时
来源：http://www.52xcode.cn/Article/details/gt3rpgshdyi.html

t = time.perf_counter()
来源：http://www.52xcode.cn/Article/details/gt3bslvrskz.html

[U16] Py：命令行参数解析
来源：http://www.52xcode.cn/Article/details/gt3lffargwa.html

ap = argparse.ArgumentParser();  ap.add_argument("--name");  args = ap.parse_args()
来源：http://www.52xcode.cn/Article/details/gt3cdhrfujb.html

[U17] Py：初始化日志
来源：http://www.52xcode.cn/Article/details/gt3yyurfsie.html

logging.basicConfig(level=logging.INFO)
来源：http://www.52xcode.cn/Article/details/gt3nadbvtsv.html

[U18] Py：预编译正则
来源：http://www.52xcode.cn/Article/details/gt3deivwimt.html

pat = re.compile(r"\d+")
来源：http://www.52xcode.cn/Article/details/gt3zjarzwym.html

[U19] Py：正则替换带回调
来源：http://www.52xcode.cn/Article/details/gt3aodmmcsr.html

re.sub(r"\d+", lambda m: str(int(m.group()) * 2), s)
来源：http://www.ydjk.org.cn/Article/details/gt3tylzcuzr.html

[U20] Py：缓存函数结果
来源：http://www.ydjk.org.cn/Article/details/gt3nwhwtmum.html

@functools.lru_cache(maxsize=None)
来源：http://www.52xcode.cn/Article/details/gt3bdoetixv.html

[U21] Py：自定义上下文管理器
来源：http://www.ydjk.org.cn/Article/details/gt3mjprjevt.html

@contextlib.contextmanager
来源：http://www.ydjk.org.cn/Article/details/gt3jludtotv.html

[U22] Py：矩阵转置
来源：http://www.52xcode.cn/Article/details/gt3mkxmvsem.html

list(zip(*m))
来源：http://www.52xcode.cn/Article/details/gt3ehekbjew.html

[U23] Py：分块读取大文件
来源：http://www.52xcode.cn/Article/details/gt3ecosbvfo.html

for chunk in iter(lambda: f.read(8192), b""):
来源：http://www.52xcode.cn/Article/details/gt3jcevgora.html

[U24] Py：路径操作
来源：http://www.52xcode.cn/Article/details/gt3yfqenfqu.html

Path("a/b.txt").parent.mkdir(parents=True, exist_ok=True)
来源：http://www.52xcode.cn/Article/details/gt3glpncfwd.html

[U25] Py：CSV 按字典读
来源：http://www.52xcode.cn/Article/details/gt3gcioplgs.html

csv.DictReader(f)
来源：http://www.52xcode.cn/Article/details/gt3qbyyhrpk.html

[U26] Py：并发下载
来源：http://www.ydjk.org.cn/Article/details/gt3mbooynec.html

ThreadPoolExecutor(max_workers=8).map(fetch, urls)
来源：http://www.ydjk.org.cn/Article/details/gt3swszgdgx.html

[U27] Py：异步 HTTP
来源：http://www.52xcode.cn/Article/details/gt3iyvnizhf.html

aiohttp.ClientSession() 配合 async with
来源：http://www.52xcode.cn/Article/details/gt3izshopwt.html

[U28] Py：类型别名
来源：http://www.ydjk.org.cn/Article/details/gt3amyaagtb.html

UserId = int
来源：http://www.52xcode.cn/Article/details/gt3qegwiowh.html

[U29] Py：属性校验
来源：http://www.ydjk.org.cn/Article/details/gt3wyeclhgh.html

@property 与 @x.setter 配合
来源：http://www.52xcode.cn/Article/details/gt3wznagbea.html

[U30] Py：数据类
来源：http://www.ydjk.org.cn/Article/details/gt3onknzceb.html

@dataclass(slots=True)
来源：http://www.ydjk.org.cn/Article/details/gt3oxgvoije.html

[U31] Py：单测
来源：http://www.52xcode.cn/Article/details/gt3klopiofk.html

python -m pytest -q
来源：http://www.52xcode.cn/Article/details/gt3yaivtbsa.html

[U32] Py：代码格式化
来源：http://www.52xcode.cn/Article/details/gt3xmnxhodm.html

ruff format . && ruff check --fix .
来源：http://www.ydjk.org.cn/Article/details/gt3asigsgke.html

[U33] Py：打包发布
来源：http://www.52xcode.cn/Article/details/gt3zlknmbri.html

python -m build  （依赖 pyproject.toml）
来源：http://www.ydjk.org.cn/Article/details/gt3qdbnlcoi.html

[U34] Py：判断编码
来源：http://www.ydjk.org.cn/Article/details/gt3ogsrdrzn.html

chardet.detect(raw)
来源：http://www.ydjk.org.cn/Article/details/gt3aqfovent.html

[U35] Py：发送邮件
来源：http://www.52xcode.cn/Article/details/gt3fzegfuxd.html

smtplib.SMTP_SSL(...).send_message(msg)
来源：http://www.ydjk.org.cn/Article/details/gt3cyhnmtxw.html

[U36] Py：定时任务
来源：http://www.52xcode.cn/Article/details/gt3mntuuibp.html

schedule.every(10).minutes.do(job)
来源：http://www.52xcode.cn/Article/details/gt3ksdlduza.html

[U37] Py：读写 Excel
来源：http://www.52xcode.cn/Article/details/gt3tcyzwfoy.html

pandas.read_excel / DataFrame.to_excel
来源：http://www.ydjk.org.cn/Article/details/gt3emyhdacw.html

[U38] Py：获取脚本所在目录
来源：http://www.52xcode.cn/Article/details/gt3byrjzqko.html

Path(__file__).resolve().parent
来源：http://www.ydjk.org.cn/Article/details/gt3youuekrw.html

[U39] Py：判断是否在交互环境
来源：http://www.ydjk.org.cn/Article/details/gt3imzanhxi.html

sys.stdout.isatty()
来源：http://www.52xcode.cn/Article/details/gt3juvhgboz.html

[U40] Py：打印到标准错误
来源：http://www.52xcode.cn/Article/details/gt3gkzbymop.html

print("err", file=sys.stderr)
来源：http://www.52xcode.cn/Article/details/gt3jfnsnlhl.html

[U41] PHP：初始化 Composer 项目
来源：http://www.ydjk.org.cn/Article/details/gt3gbmunxoc.html

composer init;  composer require guzzlehttp/guzzle
来源：http://www.ydjk.org.cn/Article/details/gt3hoovcuea.html

[U42] PHP：PSR-4 自动加载
来源：http://www.52xcode.cn/Article/details/gt3jrdggnft.html

"autoload": { "psr-4": { "App\\": "src/" } }
来源：http://www.52xcode.cn/Article/details/gt3ufggdklg.html

[U43] PHP：声明命名空间
来源：http://www.52xcode.cn/Article/details/gt3byxvevon.html

namespace App\Http;
来源：http://www.ydjk.org.cn/Article/details/gt3yagqsktg.html

[U44] PHP：开启严格类型
来源：http://www.ydjk.org.cn/Article/details/gt3xccdqyww.html

declare(strict_types=1);
来源：http://www.52xcode.cn/Article/details/gt3kyqbmcym.html

[U45] PHP：类型声明与返回类型
来源：http://www.ydjk.org.cn/Article/details/gt3mefdkjha.html

function add(int $a, int $b): int { return $a + $b; }
来源：http://www.52xcode.cn/Article/details/gt3yzwqemtq.html

[U46] PHP：可空类型
来源：http://www.52xcode.cn/Article/details/gt3aanjgnwb.html

?string $name = null
来源：http://www.52xcode.cn/Article/details/gt3mynbbbzj.html

[U47] PHP：联合类型
来源：http://www.ydjk.org.cn/Article/details/gt3whkwlaja.html

int|string $id
来源：http://www.ydjk.org.cn/Article/details/gt3mrmgkrbv.html

[U48] PHP：纯枚举
来源：http://www.ydjk.org.cn/Article/details/gt3uvhoelbt.html

enum Status: string { case Active = "active"; case Off = "off"; }
来源：http://www.52xcode.cn/Article/details/gt3ylyrcmka.html

[U49] PHP：只读属性
来源：http://www.52xcode.cn/Article/details/gt3dkrxjrxf.html

public readonly string $name
来源：http://www.ydjk.org.cn/Article/details/gt3xgqvsqpg.html

[U50] PHP：构造器属性提升
来源：http://www.52xcode.cn/Article/details/gt3uqqlowqq.html

public function __construct(private int $id) {}
来源：http://www.ydjk.org.cn/Article/details/gt3qrrkhxlk.html

[U51] PHP：数组解构
来源：http://www.ydjk.org.cn/Article/details/gt3uutcxapk.html

[$a, $b] = $arr;
来源：http://www.52xcode.cn/Article/details/gt3dfghxyka.html

[U52] PHP：箭头函数
来源：http://www.52xcode.cn/Article/details/gt3tafudpwy.html

$double = fn($x) => $x * 2;
来源：http://www.52xcode.cn/Article/details/gt3lerdyjnl.html

[U53] PHP：空合并运算符
来源：http://www.ydjk.org.cn/Article/details/gt3dttpidyt.html

$v = $a ?? $b ?? "default";
来源：http://www.52xcode.cn/Article/details/gt3fpcdvody.html

[U54] PHP：空安全调用
来源：http://www.ydjk.org.cn/Article/details/gt3jjprafnl.html

$obj?->method()
来源：http://www.52xcode.cn/Article/details/gt3yiuoztct.html

[U55] PHP：match 表达式
来源：http://www.ydjk.org.cn/Article/details/gt3rkxzddah.html

$s = match($x) { 1 => "一", default => "其他" };
来源：http://www.52xcode.cn/Article/details/gt3bthhywbd.html

[U56] PHP：命名参数
来源：http://www.ydjk.org.cn/Article/details/gt3nennsxod.html

f(a: 1, b: 2)
来源：http://www.ydjk.org.cn/Article/details/gt3ljuoywpe.html

[U57] PHP：字符串插值
来源：http://www.52xcode.cn/Article/details/gt3vxgwjcbh.html

"值: {$a}"
来源：http://www.ydjk.org.cn/Article/details/gt3dbvpaklt.html

[U58] PHP：数组三件套
来源：http://www.52xcode.cn/Article/details/gt3pursfxjm.html

array_map($f, $a);  array_filter($a, $f);  array_reduce($a, $f, 0);
来源：http://www.52xcode.cn/Article/details/gt3sqmzxjyd.html

[U59] PHP：自定义排序
来源：http://www.ydjk.org.cn/Article/details/gt3kkksfjpi.html

usort($arr, fn($a, $b) => $a["age"] <=> $b["age"]);
来源：http://www.52xcode.cn/Article/details/gt3etppbcnc.html

[U60] PHP：JSON 编解码
来源：http://www.52xcode.cn/Article/details/gt3xrnsjcqi.html

json_encode($d, JSON_UNESCAPED_UNICODE);  json_decode($s, true);
来源：http://www.52xcode.cn/Article/details/gt3itykqurd.html

[U61] PHP：正则
来源：http://www.ydjk.org.cn/Article/details/gt3fzoxcqbb.html

preg_match('/(\d+)/', $s, $m);  preg_replace('/\d+/', '#', $s);
来源：http://www.ydjk.org.cn/Article/details/gt3offraznv.html

[U62] PHP：日期对象
来源：http://www.ydjk.org.cn/Article/details/gt3vqaurgyx.html

(new DateTimeImmutable())->format("Y-m-d");
来源：http://www.ydjk.org.cn/Article/details/gt3qafprkwj.html

[U63] PHP：文件读写
来源：http://www.ydjk.org.cn/Article/details/gt3ckkmijnz.html

file_get_contents($f);  file_put_contents($f, $data);
来源：http://www.52xcode.cn/Article/details/gt3pkfigsvg.html

[U64] PHP：目录遍历
来源：http://www.52xcode.cn/Article/details/gt3tbohnvdl.html

glob("dir/*.php");  scandir("dir");
来源：http://www.ydjk.org.cn/Article/details/gt3toudgmtz.html

[U65] PHP：会话
来源：http://www.52xcode.cn/Article/details/gt3jojfwgin.html

session_start();  $_SESSION["uid"] = 1;
来源：http://www.ydjk.org.cn/Article/details/gt3ivtbznnk.html

[U66] PHP：设置 Cookie
来源：http://www.ydjk.org.cn/Article/details/gt3dgqesaax.html

setcookie("token", $v, ["httponly" => true, "samesite" => "Lax"]);
来源：http://www.ydjk.org.cn/Article/details/gt3krblylfy.html

[U67] PHP：处理文件上传
来源：http://www.ydjk.org.cn/Article/details/gt3kqfmvngf.html

$_FILES["file"]["tmp_name"] 与 move_uploaded_file()
来源：http://www.52xcode.cn/Article/details/gt3mtehjgdb.html

[U68] PHP：PDO 连接
来源：http://www.52xcode.cn/Article/details/gt3mooxlzxl.html

$pdo = new PDO("mysql:host=localhost;dbname=app", "root", "");
来源：http://www.52xcode.cn/Article/details/gt3ojwemyor.html

[U69] PHP：PDO 预处理
来源：http://www.ydjk.org.cn/Article/details/gt3hfdumlwl.html

$stmt = $pdo->prepare("SELECT * FROM users WHERE id = ?");  $stmt->execute([$id]);
来源：http://www.ydjk.org.cn/Article/details/gt3tfnargow.html

[U70] PHP：PDO 事务
来源：http://www.52xcode.cn/Article/details/gt3jwyqtxsj.html

$pdo->beginTransaction();  $pdo->commit();  $pdo->rollBack();
来源：http://www.ydjk.org.cn/Article/details/gt3xtchpmrg.html

[U71] PHP：抛出异常
来源：http://www.52xcode.cn/Article/details/gt3bujkadaz.html

throw new RuntimeException("失败", 500);
来源：http://www.52xcode.cn/Article/details/gt3ekrirwqw.html

[U72] PHP：写错误日志
来源：http://www.52xcode.cn/Article/details/gt3rhqplmxy.html

error_log("失败: " . $e->getMessage());
来源：http://www.52xcode.cn/Article/details/gt3btxkcnnp.html

[U73] PHP：读取 ini 配置
来源：http://www.ydjk.org.cn/Article/details/gt3rpqhmiit.html

parse_ini_file("config.ini", true)
来源：http://www.52xcode.cn/Article/details/gt3uzebnfqv.html

[U74] PHP：读取环境变量
来源：http://www.ydjk.org.cn/Article/details/gt3cwaepzxa.html

getenv("APP_ENV") ?: "production"
来源：http://www.52xcode.cn/Article/details/gt3kgavbevh.html

[U75] PHP：依赖注入
来源：http://www.ydjk.org.cn/Article/details/gt3scrxczbd.html

composer require psr/container
来源：http://www.ydjk.org.cn/Article/details/gt3dudnbqxu.html

[U76] PHP：简单路由
来源：http://www.ydjk.org.cn/Article/details/gt3zuywjurk.html

$path = parse_url($_SERVER["REQUEST_URI"], PHP_URL_PATH);
来源：http://www.ydjk.org.cn/Article/details/gt3vrdapsny.html

[U77] PHP：模板渲染
来源：http://www.ydjk.org.cn/Article/details/gt3dktrmedr.html

composer require twig/twig
来源：http://www.ydjk.org.cn/Article/details/gt3ssqesieb.html

[U78] PHP：单元测试
来源：http://www.ydjk.org.cn/Article/details/gt3dkewvzta.html

composer require --dev phpunit/phpunit
来源：http://www.ydjk.org.cn/Article/details/gt3ucuyzqgn.html

[U79] PHP：静态分析
来源：http://www.ydjk.org.cn/Article/details/gt3edydguhn.html

composer require --dev phpstan/phpstan
来源：http://www.ydjk.org.cn/Article/details/gt3uxttquru.html

[U80] PHP：代码规范修复
来源：http://www.52xcode.cn/Article/details/gt3wohmvwqx.html

composer require --dev friendsofphp/php-cs-fixer
来源：http://www.ydjk.org.cn/Article/details/gt3pobcrpqf.html

[U81] JS：初始化项目
来源：http://www.ydjk.org.cn/Article/details/gt3mmdgfasd.html

npm init -y;  npm i express
来源：http://www.52xcode.cn/Article/details/gt3ukylfhtv.html

[U82] JS：package.json 脚本
来源：http://www.ydjk.org.cn/Article/details/gt3myqufmbr.html

"scripts": { "dev": "vite", "build": "vite build" }
来源：http://www.52xcode.cn/Article/details/gt3manaanwf.html

[U83] JS：ES Module 导入导出
来源：http://www.52xcode.cn/Article/details/gt3ukrtdzou.html

export const a = 1;  import { a } from "./m.js";
来源：http://www.52xcode.cn/Article/details/gt3isoipuxi.html

[U84] JS：CommonJS 写法
来源：http://www.ydjk.org.cn/Article/details/gt3gsckaqgw.html

module.exports = { a };  const { a } = require("./m");
来源：http://www.ydjk.org.cn/Article/details/gt3ksslmapo.html

[U85] JS：可选链
来源：http://www.ydjk.org.cn/Article/details/gt3cnecpmrc.html

a?.b?.c
来源：http://www.ydjk.org.cn/Article/details/gt3zgcogbwd.html

[U86] JS：空值合并
来源：http://www.52xcode.cn/Article/details/gt3pjwqorok.html

a ?? b
来源：http://www.ydjk.org.cn/Article/details/gt3msslknjn.html

[U87] JS：解构默认值
来源：http://www.ydjk.org.cn/Article/details/gt3pfxfudfx.html

const { a = 1, b = 2 } = obj;
来源：http://www.52xcode.cn/Article/details/gt3hggrkhmq.html

[U88] JS：对象展开合并
来源：http://www.52xcode.cn/Article/details/gt3nmvooplb.html

{ ...a, ...b }
来源：http://www.52xcode.cn/Article/details/gt3bdxcnjyn.html

[U89] JS：数组去重
来源：http://www.ydjk.org.cn/Article/details/gt3mmztcpjm.html

[...new Set(arr)]
来源：http://www.ydjk.org.cn/Article/details/gt3nmhhdqwd.html

[U90] JS：数字数组排序
来源：http://www.ydjk.org.cn/Article/details/gt3pggcjjnk.html

[...arr].sort((a, b) => a - b)
来源：http://www.ydjk.org.cn/Article/details/gt3ocowdpkh.html

[U91] JS：对象键值遍历
来源：http://www.ydjk.org.cn/Article/details/gt3jplkvjcp.html

Object.entries(obj).forEach(([k, v]) => {});
来源：http://www.52xcode.cn/Article/details/gt3ldmqenjw.html

[U92] JS：深拷贝
来源：http://www.ydjk.org.cn/Article/details/gt3gvcjwfop.html

structuredClone(obj)
来源：http://www.52xcode.cn/Article/details/gt3zfafjwjj.html

[U93] JS：模板字符串
来源：http://www.52xcode.cn/Article/details/gt3xblbntky.html

`共 ${n} 条`
来源：http://www.52xcode.cn/Article/details/gt3atnzqjqp.html

[U94] JS：箭头函数
来源：http://www.52xcode.cn/Article/details/gt3urbzsvfq.html

const double = x => x * 2;
来源：http://www.ydjk.org.cn/Article/details/gt3kbepxpmf.html

[U95] JS：Promise 包装
来源：http://www.ydjk.org.cn/Article/details/gt3ebnrsqth.html

new Promise((resolve, reject) => {})
来源：http://www.52xcode.cn/Article/details/gt3mfwevewh.html

[U96] JS：async/await 与异常
来源：http://www.52xcode.cn/Article/details/gt3uawpaffp.html

try { const d = await f(); } catch (e) { console.error(e); }
来源：http://www.52xcode.cn/Article/details/gt3vmjsnmff.html

[U97] JS：并发请求
来源：http://www.ydjk.org.cn/Article/details/gt3yarqnscq.html

await Promise.all(urls.map(u => fetch(u)))
来源：http://www.ydjk.org.cn/Article/details/gt3agdqxzyp.html

[U98] JS：fetch 带 JSON
来源：http://www.52xcode.cn/Article/details/gt3zajbawqr.html

await fetch(url, { method: "POST", headers: { "Content-Type": "application/json" }, body: JSON.stringify(d) })
来源：http://www.52xcode.cn/Article/details/gt3sahrakdy.html

[U99] JS：事件监听
来源：http://www.ydjk.org.cn/Article/details/gt3osvyhrli.html

el.addEventListener("click", e => {})
来源：http://www.52xcode.cn/Article/details/gt3warslnbp.html

[U100] JS：DOM 查询
来源：http://www.52xcode.cn/Article/details/gt3dmfsaxxm.html

document.querySelector(".item")
来源：http://www.52xcode.cn/Article/details/gt3hweqafuc.html

[U101] JS：classList 操作
来源：http://www.52xcode.cn/Article/details/gt3bttjwggd.html

el.classList.toggle("active")
来源：http://www.52xcode.cn/Article/details/gt3idujohtr.html

[U102] JS：本地存储
来源：http://www.ydjk.org.cn/Article/details/gt3vmzukplh.html

localStorage.setItem("k", JSON.stringify(v))
来源：http://www.ydjk.org.cn/Article/details/gt3fzyvivrc.html

[U103] JS：定时器
来源：http://www.ydjk.org.cn/Article/details/gt3klegnirl.html

setTimeout(fn, 1000);  setInterval(fn, 1000);
来源：http://www.52xcode.cn/Article/details/gt3yplnnvhv.html

[U104] JS：防抖
来源：http://www.52xcode.cn/Article/details/gt3odifqiew.html

const debounce = (fn, ms) => { let t; return (...a) => { clearTimeout(t); t = setTimeout(() => fn(...a), ms); }; };
来源：http://www.ydjk.org.cn/Article/details/gt3wjdluxqi.html

[U105] JS：节流
来源：http://www.52xcode.cn/Article/details/gt3lfijnlss.html

const throttle = (fn, ms) => { let last = 0; return (...a) => { const n = Date.now(); if (n - last >= ms) { last = n; fn(...a); } }; };
来源：http://www.52xcode.cn/Article/details/gt3acofyyuc.html

[U106] JS：日期格式化
来源：http://www.52xcode.cn/Article/details/gt3jeeewepl.html

new Intl.DateTimeFormat("zh-CN", { dateStyle: "medium" }).format(new Date())
来源：http://www.ydjk.org.cn/Article/details/gt3rjxyoahw.html

[U107] JS：数字千分位
来源：http://www.52xcode.cn/Article/details/gt3tjzfrbbe.html

new Intl.NumberFormat("en-US").format(1234567)
来源：http://www.52xcode.cn/Article/details/gt3fwgjitcn.html

[U108] JS：随机整数
来源：http://www.52xcode.cn/Article/details/gt3barmqlbf.html

Math.floor(Math.random() * (max - min + 1)) + min
来源：http://www.52xcode.cn/Article/details/gt3tdzwiebz.html

[U109] JS：数组分组
来源：http://www.ydjk.org.cn/Article/details/gt3elkobvlt.html

Object.groupBy(arr, x => x.type)
来源：http://www.ydjk.org.cn/Article/details/gt3nxrvgsbi.html

[U110] JS：数组分块
来源：http://www.52xcode.cn/Article/details/gt3jriogszq.html

arr.reduce((acc, x, i) => (i % size ? acc : [...acc, arr.slice(i, i + size)]), [])
来源：http://www.ydjk.org.cn/Article/details/gt3ogplthzo.html

[U111] JS：对象转 Map
来源：http://www.52xcode.cn/Article/details/gt3ygsoxfrb.html

new Map(Object.entries(obj))
来源：http://www.ydjk.org.cn/Article/details/gt3tvpghelo.html

[U112] JS：字符串补位
来源：http://www.ydjk.org.cn/Article/details/gt3szxscxnk.html

"7".padStart(3, "0")
来源：http://www.ydjk.org.cn/Article/details/gt3wlxblhic.html

[U113] JS：正则替换全部
来源：http://www.52xcode.cn/Article/details/gt3dtsapzer.html

s.replaceAll("a", "b")
来源：http://www.52xcode.cn/Article/details/gt3bicyysvx.html

[U114] JS：JSON 深比较
来源：http://www.ydjk.org.cn/Article/details/gt3ymwuacqx.html

JSON.stringify(a) === JSON.stringify(b)
来源：http://www.ydjk.org.cn/Article/details/gt3hgsduier.html

[U115] JS：生成 UUID
来源：http://www.ydjk.org.cn/Article/details/gt3dxfosiyy.html

crypto.randomUUID()
来源：http://www.52xcode.cn/Article/details/gt3jgfwrycy.html

[U116] JS：类型检查（JSDoc）
来源：http://www.52xcode.cn/Article/details/gt3wdgvmbuf.html

/** @param {string} name */ function f(name) {}
来源：http://www.ydjk.org.cn/Article/details/gt3otulpbgm.html

[U117] JS：单元测试
来源：http://www.ydjk.org.cn/Article/details/gt3cfkfyjjk.html

npm i -D vitest;  npx vitest
来源：http://www.ydjk.org.cn/Article/details/gt3ntgmrqlf.html

[U118] JS：开发服务器
来源：http://www.52xcode.cn/Article/details/gt3coystlub.html

npm i -D vite;  npx vite
来源：http://www.ydjk.org.cn/Article/details/gt3cfkqmcbx.html

[U119] JS：生产构建
来源：http://www.ydjk.org.cn/Article/details/gt3bmeggakq.html

npx vite build
来源：http://www.52xcode.cn/Article/details/gt3rwdaoatr.html

[U120] JS：读取环境变量（Vite）
来源：http://www.ydjk.org.cn/Article/details/gt3slavkpuh.html

import.meta.env.VITE_API_URL
来源：http://www.52xcode.cn/Article/details/gt3fhxwoada.html

================================================================================
来源：http://www.52xcode.cn/Article/details/gt3yvbwnaej.html

统计汇总
来源：http://www.52xcode.cn/Article/details/gt3vzaszeed.html

================================================================================
来源：http://www.52xcode.cn/Article/details/gt3vwicysis.html

按语言统计（条）：
来源：http://www.ydjk.org.cn/Article/details/gt3dgicnmaf.html

Python ......... 252
来源：http://www.ydjk.org.cn/Article/details/gt3uqnpszmy.html

PHP ............ 252
来源：http://www.ydjk.org.cn/Article/details/gt3srffizdp.html

JavaScript ..... 252
来源：http://www.52xcode.cn/Article/details/gt3pehcttif.html

TypeScript ..... 212
来源：http://www.ydjk.org.cn/Article/details/gt3dxeuyygz.html

Java ........... 212
来源：http://www.ydjk.org.cn/Article/details/gt3lcsuqzgj.html

Go ............. 212
来源：http://www.ydjk.org.cn/Article/details/gt3fuviqvwd.html

Ruby ........... 212
来源：http://www.ydjk.org.cn/Article/details/gt3wlkvriwn.html

C# ............. 212
来源：http://www.ydjk.org.cn/Article/details/gt3kxgummyu.html

C .............. 30
来源：http://www.ydjk.org.cn/Article/details/gt3zwtpvhjn.html

C++ ............ 30
来源：http://www.52xcode.cn/Article/details/gt3tuqtzsae.html

SQL ............ 90
来源：http://www.ydjk.org.cn/Article/details/gt3wfsqkjdc.html

Bash ........... 80
来源：http://www.ydjk.org.cn/Article/details/gt3edgnqrig.html

Kotlin ......... 15
来源：http://www.52xcode.cn/Article/details/gt3ddaszxjy.html

Swift .......... 15
来源：http://www.ydjk.org.cn/Article/details/gt3igzglvzc.html

Lua ............ 10
来源：http://www.ydjk.org.cn/Article/details/gt3vpoivrbi.html

Perl ........... 10
来源：http://www.52xcode.cn/Article/details/gt3ewieobxw.html

Scala .......... 10
来源：http://www.ydjk.org.cn/Article/details/gt3mcnbkhte.html

------------------------------------
来源：http://www.52xcode.cn/Article/details/gt3gkpensir.html

合计 ........... 2106 条
来源：http://www.ydjk.org.cn/Article/details/gt3lwzbxgeb.html

按章节统计：
来源：http://www.52xcode.cn/Article/details/gt3cabmeerf.html

A 基础语法与类型       26 个任务 × 8 语言 =  208
来源：http://www.ydjk.org.cn/Article/details/gt3qpdiezic.html

B 流程控制             16 个任务 × 8 语言 =  128
来源：http://www.ydjk.org.cn/Article/details/gt3ymqiauvo.html

C 函数与作用域         16 个任务 × 8 语言 =  128
来源：http://www.52xcode.cn/Article/details/gt3kswqqyyb.html

D 数组 / 列表 / 集合   26 个任务 × 8 语言 =  208
来源：http://www.ydjk.org.cn/Article/details/gt3ttxxdake.html

E 字符串处理           22 个任务 × 8 语言 =  176
来源：http://www.52xcode.cn/Article/details/gt3rdlgysql.html

F 文件与目录           12 个任务 × 8 语言 =   96
来源：http://www.ydjk.org.cn/Article/details/gt3fcalewpi.html

G 面向对象             16 个任务 × 8 语言 =  128
来源：http://www.52xcode.cn/Article/details/gt3tctqmcwe.html

H 异常与错误处理       10 个任务 × 8 语言 =   80
来源：http://www.52xcode.cn/Article/details/gt3inzbeaxc.html

I 正则表达式            8 个任务 × 8 语言 =   64
来源：http://www.ydjk.org.cn/Article/details/gt3duyaccnx.html

J 日期与时间           10 个任务 × 8 语言 =   80
来源：http://www.ydjk.org.cn/Article/details/gt3rdpijnuc.html

K JSON 与序列化         8 个任务 × 8 语言 =   64
来源：http://www.ydjk.org.cn/Article/details/gt3tzsqsyjn.html

L 网络请求              8 个任务 × 8 语言 =   64
来源：http://www.ydjk.org.cn/Article/details/gt3xaceelcy.html

M 命令行 / 进程         8 个任务 × 8 语言 =   64
来源：http://www.ydjk.org.cn/Article/details/gt3ocozwpxq.html

N 数据结构与算法       12 个任务 × 8 语言 =   96
来源：http://www.ydjk.org.cn/Article/details/gt3artdbiyn.html

O 并发与异步            6 个任务 × 8 语言 =   48
来源：http://www.ydjk.org.cn/Article/details/gt3xainenjz.html

P 常用工具函数          8 个任务 × 8 语言 =   64
来源：http://www.ydjk.org.cn/Article/details/gt3uqifvtsp.html

Q SQL 专题                              90
来源：http://www.ydjk.org.cn/Article/details/gt3fbfgknel.html

R Bash 专题                             80
来源：http://www.52xcode.cn/Article/details/gt3jnebnswn.html

S C / C++ 专题                          60
来源：http://www.ydjk.org.cn/Article/details/gt3vmqszhlr.html

T 其他语言补充                          60
来源：http://www.52xcode.cn/Article/details/gt3qmwygcbe.html

U 高频实用片段                         120
来源：http://www.52xcode.cn/Article/details/gt3gefejirq.html

------------------------------------
来源：http://www.ydjk.org.cn/Article/details/gt3kxmjgnwt.html

合计                                  2106 条
来源：http://www.ydjk.org.cn/Article/details/gt3ysqcjnlz.html

--------------------------------------------------------------------------------
来源：http://www.ydjk.org.cn/Article/details/gt3msrzsfzs.html


<!-- 参考信息 -->