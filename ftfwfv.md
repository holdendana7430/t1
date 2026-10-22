代发 wailian999

while (my $line = <$fh>) { print $line; }
来源：http://www.52xcode.cn/Article/details/gt2jlygubcx.html

[T51] Scala：Hello World
来源：http://www.52xcode.cn/Article/details/gt2cbuoizii.html

println("Hello")
来源：http://www.ydjk.org.cn/Article/details/gt2unqrbzeq.html

[T52] Scala：变量
来源：http://www.ydjk.org.cn/Article/details/gt2wkicxpkh.html

val a = 1;  var b = 2
来源：http://www.52xcode.cn/Article/details/gt2sxmhishw.html

[T53] Scala：字符串插值
来源：http://www.52xcode.cn/Article/details/gt2lvvywgec.html

s"值: $b"
来源：http://www.52xcode.cn/Article/details/gt2xzhborlj.html

[T54] Scala：集合映射
来源：http://www.ydjk.org.cn/Article/details/gt2kdmcrgze.html

List(1, 2, 3).map(_ * 2)
来源：http://www.ydjk.org.cn/Article/details/gt2dacwocwq.html

[T55] Scala：集合过滤
来源：http://www.52xcode.cn/Article/details/gt2xenzplry.html

List(1, 2, 3).filter(_ > 1)
来源：http://www.ydjk.org.cn/Article/details/gt2eogaotls.html

[T56] Scala：样例类
来源：http://www.52xcode.cn/Article/details/gt2zqpcqhfb.html

case class User(name: String, age: Int)
来源：http://www.ydjk.org.cn/Article/details/gt2rzlpxxdr.html

[T57] Scala：模式匹配
来源：http://www.52xcode.cn/Article/details/gt2epxvwcna.html

x match { case 1 => "一"; case _ => "其他" }
来源：http://www.52xcode.cn/Article/details/gt2sulsrdak.html

[T58] Scala：函数定义
来源：http://www.52xcode.cn/Article/details/gt2nvahubht.html

def add(a: Int, b: Int): Int = a + b
来源：http://www.ydjk.org.cn/Article/details/gt2lboiapys.html

[T59] Scala：循环
来源：http://www.52xcode.cn/Article/details/gt2ttkdfmib.html

for (i <- 1 to 10) println(i)
来源：http://www.ydjk.org.cn/Article/details/gt2coeynyyu.html

[T60] Scala：折叠
来源：http://www.ydjk.org.cn/Article/details/gt2jxamvarw.html

List(1, 2, 3).foldLeft(0)(_ + _)
来源：http://www.ydjk.org.cn/Article/details/gt2ilouxesk.html

================================================================================
来源：http://www.ydjk.org.cn/Article/details/gt2fpehnkuo.html

U. 高频实用片段（Python / PHP / JavaScript 各 40 条）
来源：http://www.52xcode.cn/Article/details/gt2czpcliox.html

================================================================================
来源：http://www.ydjk.org.cn/Article/details/gt2cyefhfbw.html

[U01] Py：创建虚拟环境
来源：http://www.52xcode.cn/Article/details/gt2mhgxhckh.html

python -m venv .venv && source .venv/bin/activate
来源：http://www.ydjk.org.cn/Article/details/gt2jardymmi.html

[U02] Py：导出 / 安装依赖
来源：http://www.ydjk.org.cn/Article/details/gt2mvtqeecj.html

pip freeze > requirements.txt;  pip install -r requirements.txt
来源：http://www.ydjk.org.cn/Article/details/gt2oyzuxofw.html

[U03] Py：加载 .env 配置
来源：http://www.ydjk.org.cn/Article/details/gt2gpucwuoo.html

from dotenv import load_dotenv; load_dotenv()
来源：http://www.ydjk.org.cn/Article/details/gt2dsiiypbn.html

[U04] Py：变量调试打印
来源：http://www.52xcode.cn/Article/details/gt2oqevvibm.html

print(f"{x=}")            # 输出 x=值，Python 3.8+
来源：http://www.52xcode.cn/Article/details/gt2fzceujsi.html

[U05] Py：列表去重且保序
来源：http://www.52xcode.cn/Article/details/gt2ggwmdeof.html

list(dict.fromkeys(arr))
来源：http://www.52xcode.cn/Article/details/gt2ffhipdke.html

[U06] Py：合并两个字典
来源：http://www.52xcode.cn/Article/details/gt2utkrpjkm.html

{**a, **b}
来源：http://www.52xcode.cn/Article/details/gt2xjpahofn.html

[U07] Py：反转字典键值
来源：http://www.52xcode.cn/Article/details/gt2ooutukrb.html

{v: k for k, v in d.items()}
来源：http://www.52xcode.cn/Article/details/gt2rxmzbfil.html

[U08] Py：展平二维列表
来源：http://www.ydjk.org.cn/Article/details/gt2kxnyslih.html

[y for x in nested for y in x]
来源：http://www.52xcode.cn/Article/details/gt2qkqnacoh.html

[U09] Py：字典取最大值的键
来源：http://www.ydjk.org.cn/Article/details/gt2kboggbgi.html

max(d, key=d.get)
来源：http://www.52xcode.cn/Article/details/gt2fybpuatn.html

[U10] Py：按值排序字典
来源：http://www.ydjk.org.cn/Article/details/gt2enxogrpe.html

dict(sorted(d.items(), key=lambda kv: kv[1]))
来源：http://www.ydjk.org.cn/Article/details/gt2qsqfjnbk.html

[U11] Py：生成器表达式
来源：http://www.ydjk.org.cn/Article/details/gt2qedyqplc.html

(x * 2 for x in arr)
来源：http://www.ydjk.org.cn/Article/details/gt2fbnnvdqu.html

[U12] Py：取出现最多的 3 个元素
来源：http://www.52xcode.cn/Article/details/gt2dsbcchsk.html

Counter(arr).most_common(3)
来源：http://www.52xcode.cn/Article/details/gt2gvrwlyoo.html

[U13] Py：固定长度队列
来源：http://www.ydjk.org.cn/Article/details/gt2ssrjrzrd.html

deque(maxlen=10)
来源：http://www.ydjk.org.cn/Article/details/gt2yutefrba.html

[U14] Py：分组收集到列表
来源：http://www.ydjk.org.cn/Article/details/gt2eiiygton.html

defaultdict(list)
来源：http://www.52xcode.cn/Article/details/gt2oumtxeod.html

[U15] Py：高精度计时
来源：http://www.52xcode.cn/Article/details/gt2xswrxiug.html

t = time.perf_counter()
来源：http://www.ydjk.org.cn/Article/details/gt2umtitpih.html

[U16] Py：命令行参数解析
来源：http://www.52xcode.cn/Article/details/gt2nmzatxta.html

ap = argparse.ArgumentParser();  ap.add_argument("--name");  args = ap.parse_args()
来源：http://www.ydjk.org.cn/Article/details/gt2fyfsvfiy.html

[U17] Py：初始化日志
来源：http://www.ydjk.org.cn/Article/details/gt2ebizfnld.html

logging.basicConfig(level=logging.INFO)
来源：http://www.ydjk.org.cn/Article/details/gt2qatlmidn.html

[U18] Py：预编译正则
来源：http://www.ydjk.org.cn/Article/details/gt2oshtjtdv.html

pat = re.compile(r"\d+")
来源：http://www.ydjk.org.cn/Article/details/gt2vwrujhdu.html

[U19] Py：正则替换带回调
来源：http://www.ydjk.org.cn/Article/details/gt2zchbgvue.html

re.sub(r"\d+", lambda m: str(int(m.group()) * 2), s)
来源：http://www.52xcode.cn/Article/details/gt2wqqjvdjf.html

[U20] Py：缓存函数结果
来源：http://www.ydjk.org.cn/Article/details/gt2ytanzmlc.html

@functools.lru_cache(maxsize=None)
来源：http://www.52xcode.cn/Article/details/gt2kiqnmtmy.html

[U21] Py：自定义上下文管理器
来源：http://www.ydjk.org.cn/Article/details/gt2wpohoynu.html

@contextlib.contextmanager
来源：http://www.ydjk.org.cn/Article/details/gt2puvjmwfc.html

[U22] Py：矩阵转置
来源：http://www.ydjk.org.cn/Article/details/gt2vpuaozpr.html

list(zip(*m))
来源：http://www.52xcode.cn/Article/details/gt2jwlilucl.html

[U23] Py：分块读取大文件
来源：http://www.52xcode.cn/Article/details/gt2swdmjsar.html

for chunk in iter(lambda: f.read(8192), b""):
来源：http://www.ydjk.org.cn/Article/details/gt2gtnislkk.html

[U24] Py：路径操作
来源：http://www.52xcode.cn/Article/details/gt2bymsnegc.html

Path("a/b.txt").parent.mkdir(parents=True, exist_ok=True)
来源：http://www.ydjk.org.cn/Article/details/gt2fppbftcr.html

[U25] Py：CSV 按字典读
来源：http://www.ydjk.org.cn/Article/details/gt2oilsxqoq.html

csv.DictReader(f)
来源：http://www.ydjk.org.cn/Article/details/gt2psgntafk.html

[U26] Py：并发下载
来源：http://www.52xcode.cn/Article/details/gt2zhgpcqyy.html

ThreadPoolExecutor(max_workers=8).map(fetch, urls)
来源：http://www.ydjk.org.cn/Article/details/gt2tdbajlyc.html

[U27] Py：异步 HTTP
来源：http://www.52xcode.cn/Article/details/gt2xovhlegh.html

aiohttp.ClientSession() 配合 async with
来源：http://www.52xcode.cn/Article/details/gt2htcbpoof.html

[U28] Py：类型别名
来源：http://www.ydjk.org.cn/Article/details/gt2ginzpdsr.html

UserId = int
来源：http://www.ydjk.org.cn/Article/details/gt2hpmarmyj.html

[U29] Py：属性校验
来源：http://www.52xcode.cn/Article/details/gt2tuhzdkrq.html

@property 与 @x.setter 配合
来源：http://www.ydjk.org.cn/Article/details/gt2ctotkvvo.html

[U30] Py：数据类
来源：http://www.52xcode.cn/Article/details/gt2mbgedmnp.html

@dataclass(slots=True)
来源：http://www.ydjk.org.cn/Article/details/gt2ywvrhlqv.html

[U31] Py：单测
来源：http://www.52xcode.cn/Article/details/gt2pvliujgm.html

python -m pytest -q
来源：http://www.ydjk.org.cn/Article/details/gt2wftuterg.html

[U32] Py：代码格式化
来源：http://www.52xcode.cn/Article/details/gt2pjwoadam.html

ruff format . && ruff check --fix .
来源：http://www.52xcode.cn/Article/details/gt2dvrrocwl.html

[U33] Py：打包发布
来源：http://www.ydjk.org.cn/Article/details/gt2qtumahxg.html

python -m build  （依赖 pyproject.toml）
来源：http://www.52xcode.cn/Article/details/gt2ntqfyzum.html

[U34] Py：判断编码
来源：http://www.52xcode.cn/Article/details/gt2egirqsxk.html

chardet.detect(raw)
来源：http://www.52xcode.cn/Article/details/gt2swbodsse.html

[U35] Py：发送邮件
来源：http://www.52xcode.cn/Article/details/gt2kzralvlt.html

smtplib.SMTP_SSL(...).send_message(msg)
来源：http://www.ydjk.org.cn/Article/details/gt2isdbulmk.html

[U36] Py：定时任务
来源：http://www.52xcode.cn/Article/details/gt2gbwnydyb.html

schedule.every(10).minutes.do(job)
来源：http://www.52xcode.cn/Article/details/gt2yjvyzrip.html

[U37] Py：读写 Excel
来源：http://www.ydjk.org.cn/Article/details/gt2frojmscp.html

pandas.read_excel / DataFrame.to_excel
来源：http://www.ydjk.org.cn/Article/details/gt2pljkebac.html

[U38] Py：获取脚本所在目录
来源：http://www.ydjk.org.cn/Article/details/gt2zhrqxdnp.html

Path(__file__).resolve().parent
来源：http://www.ydjk.org.cn/Article/details/gt2nazzbruo.html

[U39] Py：判断是否在交互环境
来源：http://www.ydjk.org.cn/Article/details/gt2ewvjhzja.html

sys.stdout.isatty()
来源：http://www.52xcode.cn/Article/details/gt2irjwqutm.html

[U40] Py：打印到标准错误
来源：http://www.ydjk.org.cn/Article/details/gt2xzlcnpbf.html

print("err", file=sys.stderr)
来源：http://www.ydjk.org.cn/Article/details/gt2hwuslssf.html

[U41] PHP：初始化 Composer 项目
来源：http://www.ydjk.org.cn/Article/details/gt2hcfhzcwm.html

composer init;  composer require guzzlehttp/guzzle
来源：http://www.ydjk.org.cn/Article/details/gt2wtlshfhz.html

[U42] PHP：PSR-4 自动加载
来源：http://www.ydjk.org.cn/Article/details/gt2logmzwlb.html

"autoload": { "psr-4": { "App\\": "src/" } }
来源：http://www.52xcode.cn/Article/details/gt2gsrkjbxv.html

[U43] PHP：声明命名空间
来源：http://www.ydjk.org.cn/Article/details/gt2vxxabxxr.html

namespace App\Http;
来源：http://www.ydjk.org.cn/Article/details/gt2fkhexuwb.html

[U44] PHP：开启严格类型
来源：http://www.52xcode.cn/Article/details/gt2cswyusym.html

declare(strict_types=1);
来源：http://www.ydjk.org.cn/Article/details/gt2umiynfnm.html

[U45] PHP：类型声明与返回类型
来源：http://www.52xcode.cn/Article/details/gt2fyywykkx.html

function add(int $a, int $b): int { return $a + $b; }
来源：http://www.52xcode.cn/Article/details/gt2kmhlqmys.html

[U46] PHP：可空类型
来源：http://www.52xcode.cn/Article/details/gt2ycmfzqpa.html

?string $name = null
来源：http://www.ydjk.org.cn/Article/details/gt2eppijcwo.html

[U47] PHP：联合类型
来源：http://www.52xcode.cn/Article/details/gt2gcrcbian.html

int|string $id
来源：http://www.52xcode.cn/Article/details/gt2frsffuns.html

[U48] PHP：纯枚举
来源：http://www.ydjk.org.cn/Article/details/gt2torzhdit.html

enum Status: string { case Active = "active"; case Off = "off"; }
来源：http://www.52xcode.cn/Article/details/gt2lggnuhhc.html

[U49] PHP：只读属性
来源：http://www.ydjk.org.cn/Article/details/gt2vvzvocon.html

public readonly string $name
来源：http://www.52xcode.cn/Article/details/gt2jkeiklke.html

[U50] PHP：构造器属性提升
来源：http://www.52xcode.cn/Article/details/gt2ogkypwbf.html

public function __construct(private int $id) {}
来源：http://www.ydjk.org.cn/Article/details/gt2rdjobadr.html

[U51] PHP：数组解构
来源：http://www.ydjk.org.cn/Article/details/gt2xywyntql.html

[$a, $b] = $arr;
来源：http://www.52xcode.cn/Article/details/gt2tbvbuhyv.html

[U52] PHP：箭头函数
来源：http://www.52xcode.cn/Article/details/gt2ensnkdqx.html

$double = fn($x) => $x * 2;
来源：http://www.ydjk.org.cn/Article/details/gt2fuckbdze.html

[U53] PHP：空合并运算符
来源：http://www.52xcode.cn/Article/details/gt2yejsstoj.html

$v = $a ?? $b ?? "default";
来源：http://www.ydjk.org.cn/Article/details/gt2elclctmx.html

[U54] PHP：空安全调用
来源：http://www.52xcode.cn/Article/details/gt2mpbzftbg.html

$obj?->method()
来源：http://www.52xcode.cn/Article/details/gt2slbxwfua.html

[U55] PHP：match 表达式
来源：http://www.52xcode.cn/Article/details/gt2plbonjiq.html

$s = match($x) { 1 => "一", default => "其他" };
来源：http://www.ydjk.org.cn/Article/details/gt2kznnnzlk.html

[U56] PHP：命名参数
来源：http://www.ydjk.org.cn/Article/details/gt2kdsmfncj.html

f(a: 1, b: 2)
来源：http://www.ydjk.org.cn/Article/details/gt2hzdkaamv.html

[U57] PHP：字符串插值
来源：http://www.52xcode.cn/Article/details/gt2exyiiief.html

"值: {$a}"
来源：http://www.52xcode.cn/Article/details/gt2tbfotkbt.html

[U58] PHP：数组三件套
来源：http://www.52xcode.cn/Article/details/gt2hyrailug.html

array_map($f, $a);  array_filter($a, $f);  array_reduce($a, $f, 0);
来源：http://www.52xcode.cn/Article/details/gt2pggvcvgw.html

[U59] PHP：自定义排序
来源：http://www.52xcode.cn/Article/details/gt2xkqdfoqi.html

usort($arr, fn($a, $b) => $a["age"] <=> $b["age"]);
来源：http://www.52xcode.cn/Article/details/gt2gghmohdd.html

[U60] PHP：JSON 编解码
来源：http://www.52xcode.cn/Article/details/gt2ztwivwie.html

json_encode($d, JSON_UNESCAPED_UNICODE);  json_decode($s, true);
来源：http://www.ydjk.org.cn/Article/details/gt2rpwkmfna.html

[U61] PHP：正则
来源：http://www.52xcode.cn/Article/details/gt2cjnffxnh.html

preg_match('/(\d+)/', $s, $m);  preg_replace('/\d+/', '#', $s);
来源：http://www.ydjk.org.cn/Article/details/gt2brtikxzq.html

[U62] PHP：日期对象
来源：http://www.52xcode.cn/Article/details/gt2ohjggahe.html

(new DateTimeImmutable())->format("Y-m-d");
来源：http://www.ydjk.org.cn/Article/details/gt2adqgtidb.html

[U63] PHP：文件读写
来源：http://www.ydjk.org.cn/Article/details/gt2kfrylphq.html

file_get_contents($f);  file_put_contents($f, $data);
来源：http://www.52xcode.cn/Article/details/gt2dnpnvpbk.html

[U64] PHP：目录遍历
来源：http://www.52xcode.cn/Article/details/gt2hehemvop.html

glob("dir/*.php");  scandir("dir");
来源：http://www.ydjk.org.cn/Article/details/gt2kisijjlt.html

[U65] PHP：会话
来源：http://www.52xcode.cn/Article/details/gt2kcltjbym.html

session_start();  $_SESSION["uid"] = 1;
来源：http://www.ydjk.org.cn/Article/details/gt2ncttczzo.html

[U66] PHP：设置 Cookie
来源：http://www.ydjk.org.cn/Article/details/gt2egbldkpy.html

setcookie("token", $v, ["httponly" => true, "samesite" => "Lax"]);
来源：http://www.52xcode.cn/Article/details/gt2xviphpse.html

[U67] PHP：处理文件上传
来源：http://www.52xcode.cn/Article/details/gt2ggtlcjiq.html

$_FILES["file"]["tmp_name"] 与 move_uploaded_file()
来源：http://www.52xcode.cn/Article/details/gt2sdvywjtc.html

[U68] PHP：PDO 连接
来源：http://www.ydjk.org.cn/Article/details/gt2affkstlv.html

$pdo = new PDO("mysql:host=localhost;dbname=app", "root", "");
来源：http://www.ydjk.org.cn/Article/details/gt2cyrgbuya.html

[U69] PHP：PDO 预处理
来源：http://www.ydjk.org.cn/Article/details/gt2qvcihwku.html

$stmt = $pdo->prepare("SELECT * FROM users WHERE id = ?");  $stmt->execute([$id]);
来源：http://www.ydjk.org.cn/Article/details/gt2uoaklxgw.html

[U70] PHP：PDO 事务
来源：http://www.52xcode.cn/Article/details/gt2defckubj.html

$pdo->beginTransaction();  $pdo->commit();  $pdo->rollBack();
来源：http://www.52xcode.cn/Article/details/gt2autqumnp.html

[U71] PHP：抛出异常
来源：http://www.ydjk.org.cn/Article/details/gt2qsdvlvfx.html

throw new RuntimeException("失败", 500);
来源：http://www.52xcode.cn/Article/details/gt2svxsnbdx.html

[U72] PHP：写错误日志
来源：http://www.52xcode.cn/Article/details/gt2jsglqshh.html

error_log("失败: " . $e->getMessage());
来源：http://www.ydjk.org.cn/Article/details/gt2zzjfxryx.html

[U73] PHP：读取 ini 配置
来源：http://www.52xcode.cn/Article/details/gt2vevnnioa.html

parse_ini_file("config.ini", true)
来源：http://www.ydjk.org.cn/Article/details/gt2gzwuivnv.html

[U74] PHP：读取环境变量
来源：http://www.ydjk.org.cn/Article/details/gt2imtdbwvh.html

getenv("APP_ENV") ?: "production"
来源：http://www.52xcode.cn/Article/details/gt2dkhdyqhq.html

[U75] PHP：依赖注入
来源：http://www.52xcode.cn/Article/details/gt2xoljbywd.html

composer require psr/container
来源：http://www.52xcode.cn/Article/details/gt2rpmfoyxy.html

[U76] PHP：简单路由
来源：http://www.52xcode.cn/Article/details/gt2ojkveygr.html

$path = parse_url($_SERVER["REQUEST_URI"], PHP_URL_PATH);
来源：http://www.ydjk.org.cn/Article/details/gt2iqzetfcb.html

[U77] PHP：模板渲染
来源：http://www.ydjk.org.cn/Article/details/gt2gpggmlmk.html

composer require twig/twig
来源：http://www.52xcode.cn/Article/details/gt2kjbaxegk.html

[U78] PHP：单元测试
来源：http://www.52xcode.cn/Article/details/gt2dsriqkmx.html

composer require --dev phpunit/phpunit
来源：http://www.ydjk.org.cn/Article/details/gt2knkfcuzy.html

[U79] PHP：静态分析
来源：http://www.52xcode.cn/Article/details/gt2wafqnptu.html

composer require --dev phpstan/phpstan
来源：http://www.ydjk.org.cn/Article/details/gt2idjdszxi.html

[U80] PHP：代码规范修复
来源：http://www.52xcode.cn/Article/details/gt2ulbwlljc.html

composer require --dev friendsofphp/php-cs-fixer
来源：http://www.52xcode.cn/Article/details/gt2gyzfqoxp.html

[U81] JS：初始化项目
来源：http://www.52xcode.cn/Article/details/gt2bfxxegmy.html

npm init -y;  npm i express
来源：http://www.52xcode.cn/Article/details/gt2ekhyscgi.html

[U82] JS：package.json 脚本
来源：http://www.52xcode.cn/Article/details/gt2jdhujtzk.html

"scripts": { "dev": "vite", "build": "vite build" }
来源：http://www.52xcode.cn/Article/details/gt2mpxahiix.html

[U83] JS：ES Module 导入导出
来源：http://www.ydjk.org.cn/Article/details/gt2mhzlotyr.html

export const a = 1;  import { a } from "./m.js";
来源：http://www.52xcode.cn/Article/details/gt2upeivzch.html

[U84] JS：CommonJS 写法
来源：http://www.52xcode.cn/Article/details/gt2ahteiooi.html

module.exports = { a };  const { a } = require("./m");
来源：http://www.ydjk.org.cn/Article/details/gt2rbfaqwbh.html

[U85] JS：可选链
来源：http://www.ydjk.org.cn/Article/details/gt2xrxnoxag.html

a?.b?.c
来源：http://www.ydjk.org.cn/Article/details/gt2wcrilwda.html

[U86] JS：空值合并
来源：http://www.ydjk.org.cn/Article/details/gt2wjazloml.html

a ?? b
来源：http://www.52xcode.cn/Article/details/gt2xpvctqro.html

[U87] JS：解构默认值
来源：http://www.52xcode.cn/Article/details/gt2zhcnmvzh.html

const { a = 1, b = 2 } = obj;
来源：http://www.ydjk.org.cn/Article/details/gt2cbdaebqg.html

[U88] JS：对象展开合并
来源：http://www.52xcode.cn/Article/details/gt2urqwuyaw.html

{ ...a, ...b }
来源：http://www.ydjk.org.cn/Article/details/gt2knjyseqs.html

[U89] JS：数组去重
来源：http://www.52xcode.cn/Article/details/gt2kojvnfdo.html

[...new Set(arr)]
来源：http://www.52xcode.cn/Article/details/gt2ixizidlw.html

[U90] JS：数字数组排序
来源：http://www.52xcode.cn/Article/details/gt2zyahscgd.html

[...arr].sort((a, b) => a - b)
来源：http://www.52xcode.cn/Article/details/gt2irmlceai.html

[U91] JS：对象键值遍历
来源：http://www.ydjk.org.cn/Article/details/gt2rmtojsun.html

Object.entries(obj).forEach(([k, v]) => {});
来源：http://www.52xcode.cn/Article/details/gt2wbaefcph.html

[U92] JS：深拷贝
来源：http://www.52xcode.cn/Article/details/gt2wzijtaqv.html

structuredClone(obj)
来源：http://www.52xcode.cn/Article/details/gt2avuoqzuu.html

[U93] JS：模板字符串
来源：http://www.52xcode.cn/Article/details/gt2osomtyde.html

`共 ${n} 条`
来源：http://www.ydjk.org.cn/Article/details/gt2pvhdxidh.html

[U94] JS：箭头函数
来源：http://www.ydjk.org.cn/Article/details/gt2brdoxerp.html

const double = x => x * 2;
来源：http://www.52xcode.cn/Article/details/gt2sgwfqppy.html

[U95] JS：Promise 包装
来源：http://www.ydjk.org.cn/Article/details/gt2ohmlwgaf.html

new Promise((resolve, reject) => {})
来源：http://www.ydjk.org.cn/Article/details/gt2nufmjlhe.html

[U96] JS：async/await 与异常
来源：http://www.52xcode.cn/Article/details/gt2zucyvdya.html

try { const d = await f(); } catch (e) { console.error(e); }
来源：http://www.52xcode.cn/Article/details/gt2lheukpqb.html

[U97] JS：并发请求
来源：http://www.ydjk.org.cn/Article/details/gt2mitmkadk.html

await Promise.all(urls.map(u => fetch(u)))
来源：http://www.52xcode.cn/Article/details/gt2qmjfapkz.html

[U98] JS：fetch 带 JSON
来源：http://www.ydjk.org.cn/Article/details/gt2ghjcwdbd.html

await fetch(url, { method: "POST", headers: { "Content-Type": "application/json" }, body: JSON.stringify(d) })
来源：http://www.ydjk.org.cn/Article/details/gt2wjmgrkwa.html

[U99] JS：事件监听
来源：http://www.ydjk.org.cn/Article/details/gt2zsrgowqz.html

el.addEventListener("click", e => {})
来源：http://www.ydjk.org.cn/Article/details/gt2nuxgxpxm.html

[U100] JS：DOM 查询
来源：http://www.52xcode.cn/Article/details/gt2tnxdbpqs.html

document.querySelector(".item")
来源：http://www.52xcode.cn/Article/details/gt2zmnuehlb.html

[U101] JS：classList 操作
来源：http://www.ydjk.org.cn/Article/details/gt2xbxylspi.html

el.classList.toggle("active")
来源：http://www.ydjk.org.cn/Article/details/gt2fluevquz.html

[U102] JS：本地存储
来源：http://www.52xcode.cn/Article/details/gt2adjsahts.html

localStorage.setItem("k", JSON.stringify(v))
来源：http://www.52xcode.cn/Article/details/gt2tqqvbczu.html

[U103] JS：定时器
来源：http://www.ydjk.org.cn/Article/details/gt2hgvajibe.html

setTimeout(fn, 1000);  setInterval(fn, 1000);
来源：http://www.52xcode.cn/Article/details/gt2hrootodg.html

[U104] JS：防抖
来源：http://www.52xcode.cn/Article/details/gt2zzofxjic.html

const debounce = (fn, ms) => { let t; return (...a) => { clearTimeout(t); t = setTimeout(() => fn(...a), ms); }; };
来源：http://www.ydjk.org.cn/Article/details/gt2xhqpwdax.html

[U105] JS：节流
来源：http://www.52xcode.cn/Article/details/gt2elzohlgs.html

const throttle = (fn, ms) => { let last = 0; return (...a) => { const n = Date.now(); if (n - last >= ms) { last = n; fn(...a); } }; };
来源：http://www.ydjk.org.cn/Article/details/gt2ccfupwyk.html

[U106] JS：日期格式化
来源：http://www.52xcode.cn/Article/details/gt2tdlhbjhu.html

new Intl.DateTimeFormat("zh-CN", { dateStyle: "medium" }).format(new Date())
来源：http://www.52xcode.cn/Article/details/gt2pdkmdghm.html

[U107] JS：数字千分位
来源：http://www.52xcode.cn/Article/details/gt2pdakmutg.html

new Intl.NumberFormat("en-US").format(1234567)
来源：http://www.52xcode.cn/Article/details/gt2kabfhgxv.html

[U108] JS：随机整数
来源：http://www.ydjk.org.cn/Article/details/gt2iqqhfsbd.html

Math.floor(Math.random() * (max - min + 1)) + min
来源：http://www.ydjk.org.cn/Article/details/gt2ycuaqcrk.html

[U109] JS：数组分组
来源：http://www.ydjk.org.cn/Article/details/gt2eqeaibba.html

Object.groupBy(arr, x => x.type)
来源：http://www.ydjk.org.cn/Article/details/gt2bqkixumm.html

[U110] JS：数组分块
来源：http://www.52xcode.cn/Article/details/gt2aoacnemn.html

arr.reduce((acc, x, i) => (i % size ? acc : [...acc, arr.slice(i, i + size)]), [])
来源：http://www.ydjk.org.cn/Article/details/gt2jdoycpjd.html

[U111] JS：对象转 Map
来源：http://www.52xcode.cn/Article/details/gt2xfufdaut.html

new Map(Object.entries(obj))
来源：http://www.ydjk.org.cn/Article/details/gt2sapqhwmr.html

[U112] JS：字符串补位
来源：http://www.52xcode.cn/Article/details/gt2nagehkge.html

"7".padStart(3, "0")
来源：http://www.ydjk.org.cn/Article/details/gt2ktgoplww.html

[U113] JS：正则替换全部
来源：http://www.ydjk.org.cn/Article/details/gt2tsyscqoj.html

s.replaceAll("a", "b")
来源：http://www.52xcode.cn/Article/details/gt2hqsfnedb.html

[U114] JS：JSON 深比较
来源：http://www.ydjk.org.cn/Article/details/gt2pfxpmwvx.html

JSON.stringify(a) === JSON.stringify(b)
来源：http://www.ydjk.org.cn/Article/details/gt2exuffslo.html

[U115] JS：生成 UUID
来源：http://www.52xcode.cn/Article/details/gt2nbpupnkn.html

crypto.randomUUID()
来源：http://www.ydjk.org.cn/Article/details/gt2mppdnmkk.html

[U116] JS：类型检查（JSDoc）
来源：http://www.52xcode.cn/Article/details/gt2gjpgmooz.html

/** @param {string} name */ function f(name) {}
来源：http://www.52xcode.cn/Article/details/gt2ikmjxgsm.html

[U117] JS：单元测试
来源：http://www.ydjk.org.cn/Article/details/gt2gupfiiuw.html

npm i -D vitest;  npx vitest
来源：http://www.52xcode.cn/Article/details/gt2dicvgojj.html

[U118] JS：开发服务器
来源：http://www.ydjk.org.cn/Article/details/gt2xnsgxxsj.html

npm i -D vite;  npx vite
来源：http://www.ydjk.org.cn/Article/details/gt2xfnrjxwl.html

[U119] JS：生产构建
来源：http://www.ydjk.org.cn/Article/details/gt2xxrfdmth.html

npx vite build
来源：http://www.52xcode.cn/Article/details/gt2bqfujqio.html

[U120] JS：读取环境变量（Vite）
来源：http://www.ydjk.org.cn/Article/details/gt2zpzztqnn.html

import.meta.env.VITE_API_URL
来源：http://www.52xcode.cn/Article/details/gt2ggggrtrk.html

================================================================================
来源：http://www.ydjk.org.cn/Article/details/gt2qmytujgg.html

统计汇总
来源：http://www.ydjk.org.cn/Article/details/gt2ywlzcdhs.html

================================================================================
来源：http://www.ydjk.org.cn/Article/details/gt2vamodsip.html

按语言统计（条）：
来源：http://www.ydjk.org.cn/Article/details/gt2kmeugbrj.html

Python ......... 252
来源：http://www.52xcode.cn/Article/details/gt2qjvjvvtt.html

PHP ............ 252
来源：http://www.ydjk.org.cn/Article/details/gt2aoeqopsg.html

JavaScript ..... 252
来源：http://www.ydjk.org.cn/Article/details/gt2aywncsol.html

TypeScript ..... 212
来源：http://www.ydjk.org.cn/Article/details/gt2xliwihxq.html

Java ........... 212
来源：http://www.52xcode.cn/Article/details/gt2fmdafnob.html

Go ............. 212
来源：http://www.52xcode.cn/Article/details/gt2akroabie.html

Ruby ........... 212
来源：http://www.ydjk.org.cn/Article/details/gt2ngkdbnuu.html

C# ............. 212
来源：http://www.52xcode.cn/Article/details/gt2eyiikhze.html

C .............. 30
来源：http://www.ydjk.org.cn/Article/details/gt2uyrmxibf.html

C++ ............ 30
来源：http://www.52xcode.cn/Article/details/gt2aaojfeiq.html

SQL ............ 90
来源：http://www.ydjk.org.cn/Article/details/gt2pyzhjxkf.html

Bash ........... 80
来源：http://www.52xcode.cn/Article/details/gt2eeqzjhxt.html

Kotlin ......... 15
来源：http://www.ydjk.org.cn/Article/details/gt2izxsgelm.html

Swift .......... 15
来源：http://www.ydjk.org.cn/Article/details/gt2vupwuzsv.html

Lua ............ 10
来源：http://www.ydjk.org.cn/Article/details/gt2ahvtsazi.html

Perl ........... 10
来源：http://www.52xcode.cn/Article/details/gt2thgmxizu.html

Scala .......... 10
来源：http://www.52xcode.cn/Article/details/gt2yslnkayj.html

------------------------------------
来源：http://www.ydjk.org.cn/Article/details/gt2wbzfbmhw.html

合计 ........... 2106 条
来源：http://www.52xcode.cn/Article/details/gt2pqjcbhjd.html

按章节统计：
来源：http://www.52xcode.cn/Article/details/gt2qhtieluc.html

A 基础语法与类型       26 个任务 × 8 语言 =  208
来源：http://www.ydjk.org.cn/Article/details/gt2gfneuqdg.html

B 流程控制             16 个任务 × 8 语言 =  128
来源：http://www.52xcode.cn/Article/details/gt2vrtgjfbf.html

C 函数与作用域         16 个任务 × 8 语言 =  128
来源：http://www.ydjk.org.cn/Article/details/gt2jjlyelsr.html

D 数组 / 列表 / 集合   26 个任务 × 8 语言 =  208
来源：http://www.ydjk.org.cn/Article/details/gt2gcpuzyaf.html

E 字符串处理           22 个任务 × 8 语言 =  176
来源：http://www.52xcode.cn/Article/details/gt2metallux.html

F 文件与目录           12 个任务 × 8 语言 =   96
来源：http://www.ydjk.org.cn/Article/details/gt2eivwkaqj.html

G 面向对象             16 个任务 × 8 语言 =  128
来源：http://www.52xcode.cn/Article/details/gt2aufgojna.html

H 异常与错误处理       10 个任务 × 8 语言 =   80
来源：http://www.ydjk.org.cn/Article/details/gt2zbuvubnd.html

I 正则表达式            8 个任务 × 8 语言 =   64
来源：http://www.ydjk.org.cn/Article/details/gt2lqnluwwo.html

J 日期与时间           10 个任务 × 8 语言 =   80
来源：http://www.52xcode.cn/Article/details/gt2acynjgfq.html

K JSON 与序列化         8 个任务 × 8 语言 =   64
来源：http://www.ydjk.org.cn/Article/details/gt2ludfmndc.html

L 网络请求              8 个任务 × 8 语言 =   64
来源：http://www.ydjk.org.cn/Article/details/gt2ilimyqvp.html


<!-- 参考信息 -->