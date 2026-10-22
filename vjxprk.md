代发 wailian999

while (my $line = <$fh>) { print $line; }
来源：http://www.ydjk.org.cn/Article/details/gt2nwyrypye.html

[T51] Scala：Hello World
来源：http://www.ydjk.org.cn/Article/details/gt2yozwqvrn.html

println("Hello")
来源：http://www.52xcode.cn/Article/details/gt2qbdqckqc.html

[T52] Scala：变量
来源：http://www.52xcode.cn/Article/details/gt2hixygzpn.html

val a = 1;  var b = 2
来源：http://www.ydjk.org.cn/Article/details/gt2acrivxpl.html

[T53] Scala：字符串插值
来源：http://www.52xcode.cn/Article/details/gt2kpzpelkf.html

s"值: $b"
来源：http://www.52xcode.cn/Article/details/gt2fnlfrqon.html

[T54] Scala：集合映射
来源：http://www.52xcode.cn/Article/details/gt2idwiaorf.html

List(1, 2, 3).map(_ * 2)
来源：http://www.ydjk.org.cn/Article/details/gt2gelonvdg.html

[T55] Scala：集合过滤
来源：http://www.52xcode.cn/Article/details/gt2htsukvgj.html

List(1, 2, 3).filter(_ > 1)
来源：http://www.ydjk.org.cn/Article/details/gt2gzfpbrdv.html

[T56] Scala：样例类
来源：http://www.ydjk.org.cn/Article/details/gt2wulevheg.html

case class User(name: String, age: Int)
来源：http://www.52xcode.cn/Article/details/gt2flgammvd.html

[T57] Scala：模式匹配
来源：http://www.ydjk.org.cn/Article/details/gt2fkalzmcz.html

x match { case 1 => "一"; case _ => "其他" }
来源：http://www.52xcode.cn/Article/details/gt2usjvsftw.html

[T58] Scala：函数定义
来源：http://www.52xcode.cn/Article/details/gt2ybxmespk.html

def add(a: Int, b: Int): Int = a + b
来源：http://www.ydjk.org.cn/Article/details/gt2ptamzjsb.html

[T59] Scala：循环
来源：http://www.ydjk.org.cn/Article/details/gt2hjbqicmi.html

for (i <- 1 to 10) println(i)
来源：http://www.ydjk.org.cn/Article/details/gt2pkkpbvan.html

[T60] Scala：折叠
来源：http://www.52xcode.cn/Article/details/gt2ttppylri.html

List(1, 2, 3).foldLeft(0)(_ + _)
来源：http://www.52xcode.cn/Article/details/gt2emvswmzr.html

================================================================================
来源：http://www.52xcode.cn/Article/details/gt2oznvnupl.html

U. 高频实用片段（Python / PHP / JavaScript 各 40 条）
来源：http://www.ydjk.org.cn/Article/details/gt2cswggkeo.html

================================================================================
来源：http://www.ydjk.org.cn/Article/details/gt2uydtlfnj.html

[U01] Py：创建虚拟环境
来源：http://www.52xcode.cn/Article/details/gt2kjcmvdvl.html

python -m venv .venv && source .venv/bin/activate
来源：http://www.ydjk.org.cn/Article/details/gt2xjkxpgyk.html

[U02] Py：导出 / 安装依赖
来源：http://www.52xcode.cn/Article/details/gt2ucbwrnmd.html

pip freeze > requirements.txt;  pip install -r requirements.txt
来源：http://www.52xcode.cn/Article/details/gt2uuqxyvma.html

[U03] Py：加载 .env 配置
来源：http://www.52xcode.cn/Article/details/gt2mjekdqct.html

from dotenv import load_dotenv; load_dotenv()
来源：http://www.52xcode.cn/Article/details/gt2fraondws.html

[U04] Py：变量调试打印
来源：http://www.ydjk.org.cn/Article/details/gt2eolmvkkc.html

print(f"{x=}")            # 输出 x=值，Python 3.8+
来源：http://www.52xcode.cn/Article/details/gt2ieebtaou.html

[U05] Py：列表去重且保序
来源：http://www.ydjk.org.cn/Article/details/gt2rpjpasal.html

list(dict.fromkeys(arr))
来源：http://www.52xcode.cn/Article/details/gt2iwmwmqfq.html

[U06] Py：合并两个字典
来源：http://www.ydjk.org.cn/Article/details/gt2knbrydyt.html

{**a, **b}
来源：http://www.52xcode.cn/Article/details/gt2bbhdyjte.html

[U07] Py：反转字典键值
来源：http://www.52xcode.cn/Article/details/gt2rrxpahhb.html

{v: k for k, v in d.items()}
来源：http://www.52xcode.cn/Article/details/gt2spggxuwi.html

[U08] Py：展平二维列表
来源：http://www.ydjk.org.cn/Article/details/gt2xlbcberi.html

[y for x in nested for y in x]
来源：http://www.52xcode.cn/Article/details/gt2bnrnaxiv.html

[U09] Py：字典取最大值的键
来源：http://www.52xcode.cn/Article/details/gt2rchnigwt.html

max(d, key=d.get)
来源：http://www.52xcode.cn/Article/details/gt2gdtcvkhh.html

[U10] Py：按值排序字典
来源：http://www.52xcode.cn/Article/details/gt2ubxyxezq.html

dict(sorted(d.items(), key=lambda kv: kv[1]))
来源：http://www.52xcode.cn/Article/details/gt2gbnvmfwz.html

[U11] Py：生成器表达式
来源：http://www.ydjk.org.cn/Article/details/gt2nreenwod.html

(x * 2 for x in arr)
来源：http://www.52xcode.cn/Article/details/gt2mcqjekbi.html

[U12] Py：取出现最多的 3 个元素
来源：http://www.52xcode.cn/Article/details/gt2vomcenii.html

Counter(arr).most_common(3)
来源：http://www.52xcode.cn/Article/details/gt2ueqzkjww.html

[U13] Py：固定长度队列
来源：http://www.ydjk.org.cn/Article/details/gt2gomsdeey.html

deque(maxlen=10)
来源：http://www.ydjk.org.cn/Article/details/gt2icubunrx.html

[U14] Py：分组收集到列表
来源：http://www.52xcode.cn/Article/details/gt2ynxujhfw.html

defaultdict(list)
来源：http://www.ydjk.org.cn/Article/details/gt2oaxlyiag.html

[U15] Py：高精度计时
来源：http://www.52xcode.cn/Article/details/gt2nculkikn.html

t = time.perf_counter()
来源：http://www.52xcode.cn/Article/details/gt2uydqmfck.html

[U16] Py：命令行参数解析
来源：http://www.52xcode.cn/Article/details/gt2vzftotwv.html

ap = argparse.ArgumentParser();  ap.add_argument("--name");  args = ap.parse_args()
来源：http://www.ydjk.org.cn/Article/details/gt2mrxmdmmc.html

[U17] Py：初始化日志
来源：http://www.52xcode.cn/Article/details/gt2gtuytlli.html

logging.basicConfig(level=logging.INFO)
来源：http://www.52xcode.cn/Article/details/gt2ccbwcpzz.html

[U18] Py：预编译正则
来源：http://www.ydjk.org.cn/Article/details/gt2ekrvcxnq.html

pat = re.compile(r"\d+")
来源：http://www.52xcode.cn/Article/details/gt2qqvgdiua.html

[U19] Py：正则替换带回调
来源：http://www.ydjk.org.cn/Article/details/gt2ivgcydkx.html

re.sub(r"\d+", lambda m: str(int(m.group()) * 2), s)
来源：http://www.52xcode.cn/Article/details/gt2sakhguae.html

[U20] Py：缓存函数结果
来源：http://www.52xcode.cn/Article/details/gt2evuknitw.html

@functools.lru_cache(maxsize=None)
来源：http://www.ydjk.org.cn/Article/details/gt2zbgnudcm.html

[U21] Py：自定义上下文管理器
来源：http://www.52xcode.cn/Article/details/gt2ubgpnsci.html

@contextlib.contextmanager
来源：http://www.ydjk.org.cn/Article/details/gt2noujvrfj.html

[U22] Py：矩阵转置
来源：http://www.ydjk.org.cn/Article/details/gt2yybaigdd.html

list(zip(*m))
来源：http://www.52xcode.cn/Article/details/gt2hmcwxbeu.html

[U23] Py：分块读取大文件
来源：http://www.52xcode.cn/Article/details/gt2rbydzdmj.html

for chunk in iter(lambda: f.read(8192), b""):
来源：http://www.ydjk.org.cn/Article/details/gt2nkywtyhz.html

[U24] Py：路径操作
来源：http://www.ydjk.org.cn/Article/details/gt2ccivsxxu.html

Path("a/b.txt").parent.mkdir(parents=True, exist_ok=True)
来源：http://www.52xcode.cn/Article/details/gt2bynyxnnl.html

[U25] Py：CSV 按字典读
来源：http://www.ydjk.org.cn/Article/details/gt2keqpseyd.html

csv.DictReader(f)
来源：http://www.ydjk.org.cn/Article/details/gt2uhlcwpgt.html

[U26] Py：并发下载
来源：http://www.ydjk.org.cn/Article/details/gt2hhptydjw.html

ThreadPoolExecutor(max_workers=8).map(fetch, urls)
来源：http://www.52xcode.cn/Article/details/gt2lvpbnerw.html

[U27] Py：异步 HTTP
来源：http://www.ydjk.org.cn/Article/details/gt2zwisyjli.html

aiohttp.ClientSession() 配合 async with
来源：http://www.52xcode.cn/Article/details/gt2kzmbfogq.html

[U28] Py：类型别名
来源：http://www.ydjk.org.cn/Article/details/gt2frlnlkbp.html

UserId = int
来源：http://www.52xcode.cn/Article/details/gt2sixeyihz.html

[U29] Py：属性校验
来源：http://www.52xcode.cn/Article/details/gt2urrfrqfk.html

@property 与 @x.setter 配合
来源：http://www.ydjk.org.cn/Article/details/gt2jloxqrgh.html

[U30] Py：数据类
来源：http://www.52xcode.cn/Article/details/gt2wyeahaog.html

@dataclass(slots=True)
来源：http://www.52xcode.cn/Article/details/gt2butohxib.html

[U31] Py：单测
来源：http://www.ydjk.org.cn/Article/details/gt2zpjxcktv.html

python -m pytest -q
来源：http://www.ydjk.org.cn/Article/details/gt2upufcqmy.html

[U32] Py：代码格式化
来源：http://www.52xcode.cn/Article/details/gt2yspledgz.html

ruff format . && ruff check --fix .
来源：http://www.52xcode.cn/Article/details/gt2iqxwefqh.html

[U33] Py：打包发布
来源：http://www.ydjk.org.cn/Article/details/gt2npootsqz.html

python -m build  （依赖 pyproject.toml）
来源：http://www.52xcode.cn/Article/details/gt2otqbqgww.html

[U34] Py：判断编码
来源：http://www.ydjk.org.cn/Article/details/gt2unyumxte.html

chardet.detect(raw)
来源：http://www.ydjk.org.cn/Article/details/gt2qcumljrm.html

[U35] Py：发送邮件
来源：http://www.52xcode.cn/Article/details/gt2ubovpyny.html

smtplib.SMTP_SSL(...).send_message(msg)
来源：http://www.ydjk.org.cn/Article/details/gt2ylfymnuy.html

[U36] Py：定时任务
来源：http://www.ydjk.org.cn/Article/details/gt2pplcvhee.html

schedule.every(10).minutes.do(job)
来源：http://www.ydjk.org.cn/Article/details/gt2mlfbdoox.html

[U37] Py：读写 Excel
来源：http://www.ydjk.org.cn/Article/details/gt2raxhivtb.html

pandas.read_excel / DataFrame.to_excel
来源：http://www.ydjk.org.cn/Article/details/gt2fojcpnvs.html

[U38] Py：获取脚本所在目录
来源：http://www.52xcode.cn/Article/details/gt2swxvwkns.html

Path(__file__).resolve().parent
来源：http://www.ydjk.org.cn/Article/details/gt2tsakvsaf.html

[U39] Py：判断是否在交互环境
来源：http://www.ydjk.org.cn/Article/details/gt2rvpsmnql.html

sys.stdout.isatty()
来源：http://www.52xcode.cn/Article/details/gt2rgwttzut.html

[U40] Py：打印到标准错误
来源：http://www.52xcode.cn/Article/details/gt2ihiwexhj.html

print("err", file=sys.stderr)
来源：http://www.ydjk.org.cn/Article/details/gt2mmyucxhd.html

[U41] PHP：初始化 Composer 项目
来源：http://www.ydjk.org.cn/Article/details/gt2prrqhung.html

composer init;  composer require guzzlehttp/guzzle
来源：http://www.52xcode.cn/Article/details/gt2mahtfwzp.html

[U42] PHP：PSR-4 自动加载
来源：http://www.ydjk.org.cn/Article/details/gt2vdmwvhtl.html

"autoload": { "psr-4": { "App\\": "src/" } }
来源：http://www.52xcode.cn/Article/details/gt2vxptjmof.html

[U43] PHP：声明命名空间
来源：http://www.ydjk.org.cn/Article/details/gt2ihiijuon.html

namespace App\Http;
来源：http://www.ydjk.org.cn/Article/details/gt2ijkamjla.html

[U44] PHP：开启严格类型
来源：http://www.ydjk.org.cn/Article/details/gt2clybwoac.html

declare(strict_types=1);
来源：http://www.52xcode.cn/Article/details/gt2cqdvstlc.html

[U45] PHP：类型声明与返回类型
来源：http://www.52xcode.cn/Article/details/gt2bqsgetxu.html

function add(int $a, int $b): int { return $a + $b; }
来源：http://www.ydjk.org.cn/Article/details/gt2tomcqjrn.html

[U46] PHP：可空类型
来源：http://www.ydjk.org.cn/Article/details/gt2mvflcrem.html

?string $name = null
来源：http://www.ydjk.org.cn/Article/details/gt2kfgetxmc.html

[U47] PHP：联合类型
来源：http://www.ydjk.org.cn/Article/details/gt2iqeytfhm.html

int|string $id
来源：http://www.ydjk.org.cn/Article/details/gt2fwbajqnz.html

[U48] PHP：纯枚举
来源：http://www.ydjk.org.cn/Article/details/gt2nbksjpad.html

enum Status: string { case Active = "active"; case Off = "off"; }
来源：http://www.52xcode.cn/Article/details/gt2xxpirmtm.html

[U49] PHP：只读属性
来源：http://www.52xcode.cn/Article/details/gt2hgwncbxd.html

public readonly string $name
来源：http://www.52xcode.cn/Article/details/gt2qyvosbrc.html

[U50] PHP：构造器属性提升
来源：http://www.ydjk.org.cn/Article/details/gt2liowzzrw.html

public function __construct(private int $id) {}
来源：http://www.ydjk.org.cn/Article/details/gt2pfwaivmn.html

[U51] PHP：数组解构
来源：http://www.52xcode.cn/Article/details/gt2uxnjgaxb.html

[$a, $b] = $arr;
来源：http://www.ydjk.org.cn/Article/details/gt2gwhvqvrv.html

[U52] PHP：箭头函数
来源：http://www.52xcode.cn/Article/details/gt2qhfopunh.html

$double = fn($x) => $x * 2;
来源：http://www.ydjk.org.cn/Article/details/gt2pbztuwwd.html

[U53] PHP：空合并运算符
来源：http://www.ydjk.org.cn/Article/details/gt2esygkzyq.html

$v = $a ?? $b ?? "default";
来源：http://www.ydjk.org.cn/Article/details/gt2duotpvys.html

[U54] PHP：空安全调用
来源：http://www.ydjk.org.cn/Article/details/gt2bkcfeert.html

$obj?->method()
来源：http://www.52xcode.cn/Article/details/gt2hbnlheup.html

[U55] PHP：match 表达式
来源：http://www.52xcode.cn/Article/details/gt2pftdkska.html

$s = match($x) { 1 => "一", default => "其他" };
来源：http://www.ydjk.org.cn/Article/details/gt2irmgekfj.html

[U56] PHP：命名参数
来源：http://www.52xcode.cn/Article/details/gt2hodicnch.html

f(a: 1, b: 2)
来源：http://www.52xcode.cn/Article/details/gt2vcgewvpi.html

[U57] PHP：字符串插值
来源：http://www.ydjk.org.cn/Article/details/gt2tapzxejd.html

"值: {$a}"
来源：http://www.52xcode.cn/Article/details/gt2wrkkdcht.html

[U58] PHP：数组三件套
来源：http://www.52xcode.cn/Article/details/gt2dqfqdzze.html

array_map($f, $a);  array_filter($a, $f);  array_reduce($a, $f, 0);
来源：http://www.52xcode.cn/Article/details/gt2fltzwqxc.html

[U59] PHP：自定义排序
来源：http://www.ydjk.org.cn/Article/details/gt2usdntzlw.html

usort($arr, fn($a, $b) => $a["age"] <=> $b["age"]);
来源：http://www.52xcode.cn/Article/details/gt2uldhxlzz.html

[U60] PHP：JSON 编解码
来源：http://www.52xcode.cn/Article/details/gt2pesylshq.html

json_encode($d, JSON_UNESCAPED_UNICODE);  json_decode($s, true);
来源：http://www.ydjk.org.cn/Article/details/gt2xwerckiv.html

[U61] PHP：正则
来源：http://www.ydjk.org.cn/Article/details/gt2bedftvyq.html

preg_match('/(\d+)/', $s, $m);  preg_replace('/\d+/', '#', $s);
来源：http://www.52xcode.cn/Article/details/gt2oabbllqb.html

[U62] PHP：日期对象
来源：http://www.ydjk.org.cn/Article/details/gt2ksqtxjfq.html

(new DateTimeImmutable())->format("Y-m-d");
来源：http://www.ydjk.org.cn/Article/details/gt2oqltfwpl.html

[U63] PHP：文件读写
来源：http://www.ydjk.org.cn/Article/details/gt2mydzryqb.html

file_get_contents($f);  file_put_contents($f, $data);
来源：http://www.52xcode.cn/Article/details/gt2psavqfxo.html

[U64] PHP：目录遍历
来源：http://www.52xcode.cn/Article/details/gt2pfxuwelr.html

glob("dir/*.php");  scandir("dir");
来源：http://www.52xcode.cn/Article/details/gt2vjdbjgce.html

[U65] PHP：会话
来源：http://www.52xcode.cn/Article/details/gt2ijzufasm.html

session_start();  $_SESSION["uid"] = 1;
来源：http://www.ydjk.org.cn/Article/details/gt2odaosqsw.html

[U66] PHP：设置 Cookie
来源：http://www.52xcode.cn/Article/details/gt2kdbhmitb.html

setcookie("token", $v, ["httponly" => true, "samesite" => "Lax"]);
来源：http://www.ydjk.org.cn/Article/details/gt2jjtaouaj.html

[U67] PHP：处理文件上传
来源：http://www.ydjk.org.cn/Article/details/gt2nydxrscz.html

$_FILES["file"]["tmp_name"] 与 move_uploaded_file()
来源：http://www.52xcode.cn/Article/details/gt2otbpuuei.html

[U68] PHP：PDO 连接
来源：http://www.ydjk.org.cn/Article/details/gt2adaskxjs.html

$pdo = new PDO("mysql:host=localhost;dbname=app", "root", "");
来源：http://www.52xcode.cn/Article/details/gt2nqwhjame.html

[U69] PHP：PDO 预处理
来源：http://www.52xcode.cn/Article/details/gt2yqkdlkax.html

$stmt = $pdo->prepare("SELECT * FROM users WHERE id = ?");  $stmt->execute([$id]);
来源：http://www.ydjk.org.cn/Article/details/gt2qmpylkhb.html

[U70] PHP：PDO 事务
来源：http://www.52xcode.cn/Article/details/gt2wibetklr.html

$pdo->beginTransaction();  $pdo->commit();  $pdo->rollBack();
来源：http://www.52xcode.cn/Article/details/gt2uprhyefj.html

[U71] PHP：抛出异常
来源：http://www.ydjk.org.cn/Article/details/gt2sxfixleh.html

throw new RuntimeException("失败", 500);
来源：http://www.ydjk.org.cn/Article/details/gt2ngtjugde.html

[U72] PHP：写错误日志
来源：http://www.ydjk.org.cn/Article/details/gt2xvdstlle.html

error_log("失败: " . $e->getMessage());
来源：http://www.52xcode.cn/Article/details/gt2mbhyijfl.html

[U73] PHP：读取 ini 配置
来源：http://www.ydjk.org.cn/Article/details/gt2nkwrjskn.html

parse_ini_file("config.ini", true)
来源：http://www.ydjk.org.cn/Article/details/gt2dwngkpsc.html

[U74] PHP：读取环境变量
来源：http://www.ydjk.org.cn/Article/details/gt2xgahynwa.html

getenv("APP_ENV") ?: "production"
来源：http://www.ydjk.org.cn/Article/details/gt2aicngeoo.html

[U75] PHP：依赖注入
来源：http://www.52xcode.cn/Article/details/gt2audikuks.html

composer require psr/container
来源：http://www.52xcode.cn/Article/details/gt2jfurawhm.html

[U76] PHP：简单路由
来源：http://www.ydjk.org.cn/Article/details/gt2ywzkwuzn.html

$path = parse_url($_SERVER["REQUEST_URI"], PHP_URL_PATH);
来源：http://www.52xcode.cn/Article/details/gt2gekstkyj.html

[U77] PHP：模板渲染
来源：http://www.52xcode.cn/Article/details/gt2csihkfaa.html

composer require twig/twig
来源：http://www.ydjk.org.cn/Article/details/gt2yorurbqs.html

[U78] PHP：单元测试
来源：http://www.ydjk.org.cn/Article/details/gt2zlmnvjkt.html

composer require --dev phpunit/phpunit
来源：http://www.52xcode.cn/Article/details/gt2natzdgyy.html

[U79] PHP：静态分析
来源：http://www.52xcode.cn/Article/details/gt2dxxhcrhq.html

composer require --dev phpstan/phpstan
来源：http://www.ydjk.org.cn/Article/details/gt2ftxdjvfd.html

[U80] PHP：代码规范修复
来源：http://www.52xcode.cn/Article/details/gt2zychnmvi.html

composer require --dev friendsofphp/php-cs-fixer
来源：http://www.ydjk.org.cn/Article/details/gt2pqaadzdk.html

[U81] JS：初始化项目
来源：http://www.52xcode.cn/Article/details/gt2mmiwjesq.html

npm init -y;  npm i express
来源：http://www.52xcode.cn/Article/details/gt2zuhdmfqo.html

[U82] JS：package.json 脚本
来源：http://www.ydjk.org.cn/Article/details/gt2wobtrvhx.html

"scripts": { "dev": "vite", "build": "vite build" }
来源：http://www.ydjk.org.cn/Article/details/gt2pszmlbvu.html

[U83] JS：ES Module 导入导出
来源：http://www.ydjk.org.cn/Article/details/gt2scquysha.html

export const a = 1;  import { a } from "./m.js";
来源：http://www.ydjk.org.cn/Article/details/gt2pzmmuqsh.html

[U84] JS：CommonJS 写法
来源：http://www.ydjk.org.cn/Article/details/gt2nnueiihb.html

module.exports = { a };  const { a } = require("./m");
来源：http://www.ydjk.org.cn/Article/details/gt2dameymgp.html

[U85] JS：可选链
来源：http://www.ydjk.org.cn/Article/details/gt2orsfvcoj.html

a?.b?.c
来源：http://www.52xcode.cn/Article/details/gt2dwcpvqwq.html

[U86] JS：空值合并
来源：http://www.52xcode.cn/Article/details/gt2hqelkkqb.html

a ?? b
来源：http://www.52xcode.cn/Article/details/gt2iazncner.html

[U87] JS：解构默认值
来源：http://www.ydjk.org.cn/Article/details/gt2znnagosp.html

const { a = 1, b = 2 } = obj;
来源：http://www.ydjk.org.cn/Article/details/gt2tyhkjqbz.html

[U88] JS：对象展开合并
来源：http://www.ydjk.org.cn/Article/details/gt2fsaofezt.html

{ ...a, ...b }
来源：http://www.52xcode.cn/Article/details/gt2zttymvom.html

[U89] JS：数组去重
来源：http://www.52xcode.cn/Article/details/gt2jvxkjhvn.html

[...new Set(arr)]
来源：http://www.ydjk.org.cn/Article/details/gt2jgsvbosq.html

[U90] JS：数字数组排序
来源：http://www.52xcode.cn/Article/details/gt2pkqlbdpw.html

[...arr].sort((a, b) => a - b)
来源：http://www.ydjk.org.cn/Article/details/gt2vbfmetpk.html

[U91] JS：对象键值遍历
来源：http://www.52xcode.cn/Article/details/gt2kyxlczgt.html

Object.entries(obj).forEach(([k, v]) => {});
来源：http://www.52xcode.cn/Article/details/gt2vrqrxulc.html

[U92] JS：深拷贝
来源：http://www.ydjk.org.cn/Article/details/gt2xzinfqad.html

structuredClone(obj)
来源：http://www.52xcode.cn/Article/details/gt2lcnajlkv.html

[U93] JS：模板字符串
来源：http://www.52xcode.cn/Article/details/gt2rtitwkqa.html

`共 ${n} 条`
来源：http://www.52xcode.cn/Article/details/gt2ztinmlkm.html

[U94] JS：箭头函数
来源：http://www.ydjk.org.cn/Article/details/gt2pxhkwarh.html

const double = x => x * 2;
来源：http://www.52xcode.cn/Article/details/gt2kgfybxak.html

[U95] JS：Promise 包装
来源：http://www.52xcode.cn/Article/details/gt2vlwrqjhh.html

new Promise((resolve, reject) => {})
来源：http://www.52xcode.cn/Article/details/gt2cqseqinc.html

[U96] JS：async/await 与异常
来源：http://www.52xcode.cn/Article/details/gt2ikbqyejj.html

try { const d = await f(); } catch (e) { console.error(e); }
来源：http://www.ydjk.org.cn/Article/details/gt2dbxrwrea.html

[U97] JS：并发请求
来源：http://www.ydjk.org.cn/Article/details/gt2syydmeim.html

await Promise.all(urls.map(u => fetch(u)))
来源：http://www.ydjk.org.cn/Article/details/gt2cqpdpgwy.html

[U98] JS：fetch 带 JSON
来源：http://www.ydjk.org.cn/Article/details/gt2zpctlefd.html

await fetch(url, { method: "POST", headers: { "Content-Type": "application/json" }, body: JSON.stringify(d) })
来源：http://www.52xcode.cn/Article/details/gt2oxgwtwhn.html

[U99] JS：事件监听
来源：http://www.52xcode.cn/Article/details/gt2kdxekjdq.html

el.addEventListener("click", e => {})
来源：http://www.52xcode.cn/Article/details/gt2dxddxzka.html

[U100] JS：DOM 查询
来源：http://www.52xcode.cn/Article/details/gt2dskuicgt.html

document.querySelector(".item")
来源：http://www.ydjk.org.cn/Article/details/gt2viwjxaqm.html

[U101] JS：classList 操作
来源：http://www.52xcode.cn/Article/details/gt2hdvjodwh.html

el.classList.toggle("active")
来源：http://www.ydjk.org.cn/Article/details/gt2tqpfzfvr.html

[U102] JS：本地存储
来源：http://www.ydjk.org.cn/Article/details/gt2qdjhnqyi.html

localStorage.setItem("k", JSON.stringify(v))
来源：http://www.52xcode.cn/Article/details/gt2ftbrjmlz.html

[U103] JS：定时器
来源：http://www.52xcode.cn/Article/details/gt2dkvegolz.html

setTimeout(fn, 1000);  setInterval(fn, 1000);
来源：http://www.52xcode.cn/Article/details/gt2hdcdkqfc.html

[U104] JS：防抖
来源：http://www.ydjk.org.cn/Article/details/gt2ccsaftwd.html

const debounce = (fn, ms) => { let t; return (...a) => { clearTimeout(t); t = setTimeout(() => fn(...a), ms); }; };
来源：http://www.52xcode.cn/Article/details/gt2gtrbnijk.html

[U105] JS：节流
来源：http://www.52xcode.cn/Article/details/gt2zrlornlh.html

const throttle = (fn, ms) => { let last = 0; return (...a) => { const n = Date.now(); if (n - last >= ms) { last = n; fn(...a); } }; };
来源：http://www.ydjk.org.cn/Article/details/gt2nsslyrey.html

[U106] JS：日期格式化
来源：http://www.ydjk.org.cn/Article/details/gt2nzdutcop.html

new Intl.DateTimeFormat("zh-CN", { dateStyle: "medium" }).format(new Date())
来源：http://www.ydjk.org.cn/Article/details/gt2fuhkflkc.html

[U107] JS：数字千分位
来源：http://www.52xcode.cn/Article/details/gt2gwaesefz.html

new Intl.NumberFormat("en-US").format(1234567)
来源：http://www.ydjk.org.cn/Article/details/gt2jrxfheoo.html

[U108] JS：随机整数
来源：http://www.52xcode.cn/Article/details/gt2stmnmnsj.html

Math.floor(Math.random() * (max - min + 1)) + min
来源：http://www.ydjk.org.cn/Article/details/gt2nswkdntq.html

[U109] JS：数组分组
来源：http://www.52xcode.cn/Article/details/gt2ftvbmpcz.html

Object.groupBy(arr, x => x.type)
来源：http://www.52xcode.cn/Article/details/gt2hckimmyu.html

[U110] JS：数组分块
来源：http://www.ydjk.org.cn/Article/details/gt2nllmpqai.html

arr.reduce((acc, x, i) => (i % size ? acc : [...acc, arr.slice(i, i + size)]), [])
来源：http://www.ydjk.org.cn/Article/details/gt2qognxfcy.html

[U111] JS：对象转 Map
来源：http://www.52xcode.cn/Article/details/gt2voryyzfd.html

new Map(Object.entries(obj))
来源：http://www.52xcode.cn/Article/details/gt2czdoxnrw.html

[U112] JS：字符串补位
来源：http://www.ydjk.org.cn/Article/details/gt2dwexugsf.html

"7".padStart(3, "0")
来源：http://www.ydjk.org.cn/Article/details/gt2rupeympj.html

[U113] JS：正则替换全部
来源：http://www.ydjk.org.cn/Article/details/gt2wwseenrr.html

s.replaceAll("a", "b")
来源：http://www.ydjk.org.cn/Article/details/gt2mitbegav.html

[U114] JS：JSON 深比较
来源：http://www.52xcode.cn/Article/details/gt2mnithmzv.html

JSON.stringify(a) === JSON.stringify(b)
来源：http://www.52xcode.cn/Article/details/gt2pcubbfan.html

[U115] JS：生成 UUID
来源：http://www.52xcode.cn/Article/details/gt2vsjudwyk.html

crypto.randomUUID()
来源：http://www.52xcode.cn/Article/details/gt2ryseriuq.html

[U116] JS：类型检查（JSDoc）
来源：http://www.52xcode.cn/Article/details/gt2syngcywe.html

/** @param {string} name */ function f(name) {}
来源：http://www.ydjk.org.cn/Article/details/gt2ejviqgcl.html

[U117] JS：单元测试
来源：http://www.52xcode.cn/Article/details/gt2gnivdfwr.html

npm i -D vitest;  npx vitest
来源：http://www.52xcode.cn/Article/details/gt2zmookgto.html

[U118] JS：开发服务器
来源：http://www.52xcode.cn/Article/details/gt2zixydftk.html

npm i -D vite;  npx vite
来源：http://www.52xcode.cn/Article/details/gt2mdrerdht.html

[U119] JS：生产构建
来源：http://www.52xcode.cn/Article/details/gt2cpptxcgp.html

npx vite build
来源：http://www.ydjk.org.cn/Article/details/gt2vbfsqdrw.html

[U120] JS：读取环境变量（Vite）
来源：http://www.52xcode.cn/Article/details/gt2joyijgce.html

import.meta.env.VITE_API_URL
来源：http://www.52xcode.cn/Article/details/gt2zvfcatho.html

================================================================================
来源：http://www.52xcode.cn/Article/details/gt2giikdqar.html

统计汇总
来源：http://www.52xcode.cn/Article/details/gt2yhcwokhj.html

================================================================================
来源：http://www.ydjk.org.cn/Article/details/gt2ybqcmiuy.html

按语言统计（条）：
来源：http://www.52xcode.cn/Article/details/gt2livarcnf.html

Python ......... 252
来源：http://www.ydjk.org.cn/Article/details/gt2pedvztzt.html

PHP ............ 252
来源：http://www.ydjk.org.cn/Article/details/gt2omqrytaz.html

JavaScript ..... 252
来源：http://www.ydjk.org.cn/Article/details/gt2xjowtfqk.html

TypeScript ..... 212
来源：http://www.ydjk.org.cn/Article/details/gt2sqbsjcbs.html

Java ........... 212
来源：http://www.ydjk.org.cn/Article/details/gt2ttvilnxk.html

Go ............. 212
来源：http://www.52xcode.cn/Article/details/gt2fifnvcyr.html

Ruby ........... 212
来源：http://www.52xcode.cn/Article/details/gt2ussprzdn.html

C# ............. 212
来源：http://www.52xcode.cn/Article/details/gt2hctxystl.html

C .............. 30
来源：http://www.52xcode.cn/Article/details/gt2neqmpagc.html

C++ ............ 30
来源：http://www.52xcode.cn/Article/details/gt2saeaetou.html

SQL ............ 90
来源：http://www.ydjk.org.cn/Article/details/gt2lwmbvzss.html

Bash ........... 80
来源：http://www.52xcode.cn/Article/details/gt2czstckbl.html

Kotlin ......... 15
来源：http://www.ydjk.org.cn/Article/details/gt2ztixidtm.html

Swift .......... 15
来源：http://www.ydjk.org.cn/Article/details/gt2lxhfldke.html

Lua ............ 10
来源：http://www.ydjk.org.cn/Article/details/gt2einmcxkh.html

Perl ........... 10
来源：http://www.52xcode.cn/Article/details/gt2lcddjuyx.html

Scala .......... 10
来源：http://www.ydjk.org.cn/Article/details/gt2frocvmhj.html

------------------------------------
来源：http://www.52xcode.cn/Article/details/gt2lttdprix.html

合计 ........... 2106 条
来源：http://www.52xcode.cn/Article/details/gt2kuxaymnw.html

按章节统计：
来源：http://www.52xcode.cn/Article/details/gt2suyttvwn.html

A 基础语法与类型       26 个任务 × 8 语言 =  208
来源：http://www.ydjk.org.cn/Article/details/gt2awahinso.html

B 流程控制             16 个任务 × 8 语言 =  128
来源：http://www.ydjk.org.cn/Article/details/gt2ojaftuhm.html

C 函数与作用域         16 个任务 × 8 语言 =  128
来源：http://www.52xcode.cn/Article/details/gt2otlyhtiz.html

D 数组 / 列表 / 集合   26 个任务 × 8 语言 =  208
来源：http://www.ydjk.org.cn/Article/details/gt2zmxhqpmp.html

E 字符串处理           22 个任务 × 8 语言 =  176
来源：http://www.52xcode.cn/Article/details/gt2focjvgxf.html

F 文件与目录           12 个任务 × 8 语言 =   96
来源：http://www.52xcode.cn/Article/details/gt2mjryephr.html

G 面向对象             16 个任务 × 8 语言 =  128
来源：http://www.ydjk.org.cn/Article/details/gt2yyfgdxpm.html

H 异常与错误处理       10 个任务 × 8 语言 =   80
来源：http://www.ydjk.org.cn/Article/details/gt2ogrxboel.html

I 正则表达式            8 个任务 × 8 语言 =   64
来源：http://www.52xcode.cn/Article/details/gt2aaiiqnzd.html

J 日期与时间           10 个任务 × 8 语言 =   80
来源：http://www.ydjk.org.cn/Article/details/gt2mgtcrpma.html

K JSON 与序列化         8 个任务 × 8 语言 =   64
来源：http://www.52xcode.cn/Article/details/gt2iwhrivfl.html

L 网络请求              8 个任务 × 8 语言 =   64
来源：http://www.ydjk.org.cn/Article/details/gt2vsogqprt.html


<!-- 参考信息 -->