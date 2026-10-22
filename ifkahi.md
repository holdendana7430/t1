代发 wailian999

while (my $line = <$fh>) { print $line; }
来源：http://www.ydjk.org.cn/Article/details/gt2zddvyyks.html

[T51] Scala：Hello World
来源：http://www.52xcode.cn/Article/details/gt2fxzthfmk.html

println("Hello")
来源：http://www.ydjk.org.cn/Article/details/gt2acflhsoq.html

[T52] Scala：变量
来源：http://www.52xcode.cn/Article/details/gt2hwfgodjq.html

val a = 1;  var b = 2
来源：http://www.52xcode.cn/Article/details/gt2ajkpcldt.html

[T53] Scala：字符串插值
来源：http://www.ydjk.org.cn/Article/details/gt2nphzkfkv.html

s"值: $b"
来源：http://www.52xcode.cn/Article/details/gt2jwdeqacz.html

[T54] Scala：集合映射
来源：http://www.52xcode.cn/Article/details/gt2kohrhszh.html

List(1, 2, 3).map(_ * 2)
来源：http://www.52xcode.cn/Article/details/gt2kawmvhpu.html

[T55] Scala：集合过滤
来源：http://www.52xcode.cn/Article/details/gt2eynesbdv.html

List(1, 2, 3).filter(_ > 1)
来源：http://www.52xcode.cn/Article/details/gt2jgrilxko.html

[T56] Scala：样例类
来源：http://www.52xcode.cn/Article/details/gt2rjsxgfcs.html

case class User(name: String, age: Int)
来源：http://www.ydjk.org.cn/Article/details/gt2bvbfndof.html

[T57] Scala：模式匹配
来源：http://www.52xcode.cn/Article/details/gt2dgmmhmau.html

x match { case 1 => "一"; case _ => "其他" }
来源：http://www.52xcode.cn/Article/details/gt2zcketudn.html

[T58] Scala：函数定义
来源：http://www.52xcode.cn/Article/details/gt2rsfhwycu.html

def add(a: Int, b: Int): Int = a + b
来源：http://www.52xcode.cn/Article/details/gt2avutlglh.html

[T59] Scala：循环
来源：http://www.52xcode.cn/Article/details/gt2tpcumkma.html

for (i <- 1 to 10) println(i)
来源：http://www.52xcode.cn/Article/details/gt2dxtarboj.html

[T60] Scala：折叠
来源：http://www.ydjk.org.cn/Article/details/gt2ocmsgkbi.html

List(1, 2, 3).foldLeft(0)(_ + _)
来源：http://www.52xcode.cn/Article/details/gt2jpjjfgxz.html

================================================================================
来源：http://www.52xcode.cn/Article/details/gt2iwjlabmi.html

U. 高频实用片段（Python / PHP / JavaScript 各 40 条）
来源：http://www.ydjk.org.cn/Article/details/gt2jhgzdftk.html

================================================================================
来源：http://www.52xcode.cn/Article/details/gt2eddkdimo.html

[U01] Py：创建虚拟环境
来源：http://www.ydjk.org.cn/Article/details/gt2jlnxcxza.html

python -m venv .venv && source .venv/bin/activate
来源：http://www.52xcode.cn/Article/details/gt2xbhdafsd.html

[U02] Py：导出 / 安装依赖
来源：http://www.ydjk.org.cn/Article/details/gt2tghuteta.html

pip freeze > requirements.txt;  pip install -r requirements.txt
来源：http://www.ydjk.org.cn/Article/details/gt2gfjwzoii.html

[U03] Py：加载 .env 配置
来源：http://www.ydjk.org.cn/Article/details/gt2zbizqywk.html

from dotenv import load_dotenv; load_dotenv()
来源：http://www.ydjk.org.cn/Article/details/gt2lxlqbmqb.html

[U04] Py：变量调试打印
来源：http://www.52xcode.cn/Article/details/gt2terdbpib.html

print(f"{x=}")            # 输出 x=值，Python 3.8+
来源：http://www.ydjk.org.cn/Article/details/gt2wklrwhkx.html

[U05] Py：列表去重且保序
来源：http://www.52xcode.cn/Article/details/gt2fqhlcykj.html

list(dict.fromkeys(arr))
来源：http://www.52xcode.cn/Article/details/gt2asmgeqhv.html

[U06] Py：合并两个字典
来源：http://www.52xcode.cn/Article/details/gt2ulhilllr.html

{**a, **b}
来源：http://www.ydjk.org.cn/Article/details/gt2gloxcqnm.html

[U07] Py：反转字典键值
来源：http://www.52xcode.cn/Article/details/gt2mmokfzkt.html

{v: k for k, v in d.items()}
来源：http://www.52xcode.cn/Article/details/gt2tqrnbhuq.html

[U08] Py：展平二维列表
来源：http://www.52xcode.cn/Article/details/gt2vabgweey.html

[y for x in nested for y in x]
来源：http://www.52xcode.cn/Article/details/gt2axkqgqan.html

[U09] Py：字典取最大值的键
来源：http://www.52xcode.cn/Article/details/gt2qnmqgecu.html

max(d, key=d.get)
来源：http://www.52xcode.cn/Article/details/gt2kfprjrey.html

[U10] Py：按值排序字典
来源：http://www.ydjk.org.cn/Article/details/gt2tzwfxqfu.html

dict(sorted(d.items(), key=lambda kv: kv[1]))
来源：http://www.52xcode.cn/Article/details/gt2uslpihjo.html

[U11] Py：生成器表达式
来源：http://www.ydjk.org.cn/Article/details/gt2tttcrxrx.html

(x * 2 for x in arr)
来源：http://www.ydjk.org.cn/Article/details/gt2dddluzfp.html

[U12] Py：取出现最多的 3 个元素
来源：http://www.ydjk.org.cn/Article/details/gt2tigkwjya.html

Counter(arr).most_common(3)
来源：http://www.52xcode.cn/Article/details/gt2mdpbsyra.html

[U13] Py：固定长度队列
来源：http://www.ydjk.org.cn/Article/details/gt2wsqcodzu.html

deque(maxlen=10)
来源：http://www.ydjk.org.cn/Article/details/gt2biyazaxd.html

[U14] Py：分组收集到列表
来源：http://www.ydjk.org.cn/Article/details/gt2ortfmmsl.html

defaultdict(list)
来源：http://www.ydjk.org.cn/Article/details/gt2lxrivvkc.html

[U15] Py：高精度计时
来源：http://www.ydjk.org.cn/Article/details/gt2juefnmdj.html

t = time.perf_counter()
来源：http://www.ydjk.org.cn/Article/details/gt2jjvkdudi.html

[U16] Py：命令行参数解析
来源：http://www.52xcode.cn/Article/details/gt2lbxexeiv.html

ap = argparse.ArgumentParser();  ap.add_argument("--name");  args = ap.parse_args()
来源：http://www.52xcode.cn/Article/details/gt2sqtfsfao.html

[U17] Py：初始化日志
来源：http://www.ydjk.org.cn/Article/details/gt2wcoexoaf.html

logging.basicConfig(level=logging.INFO)
来源：http://www.52xcode.cn/Article/details/gt2rqextpei.html

[U18] Py：预编译正则
来源：http://www.52xcode.cn/Article/details/gt2hntaiiep.html

pat = re.compile(r"\d+")
来源：http://www.52xcode.cn/Article/details/gt2mfwwrnok.html

[U19] Py：正则替换带回调
来源：http://www.52xcode.cn/Article/details/gt2okzuraww.html

re.sub(r"\d+", lambda m: str(int(m.group()) * 2), s)
来源：http://www.52xcode.cn/Article/details/gt2yvqjwaiw.html

[U20] Py：缓存函数结果
来源：http://www.52xcode.cn/Article/details/gt2tlhvrhrp.html

@functools.lru_cache(maxsize=None)
来源：http://www.ydjk.org.cn/Article/details/gt2vdmawxrz.html

[U21] Py：自定义上下文管理器
来源：http://www.ydjk.org.cn/Article/details/gt2umxpaoki.html

@contextlib.contextmanager
来源：http://www.52xcode.cn/Article/details/gt2fcrvzubl.html

[U22] Py：矩阵转置
来源：http://www.ydjk.org.cn/Article/details/gt2qfghxrvi.html

list(zip(*m))
来源：http://www.52xcode.cn/Article/details/gt2ifjrfstt.html

[U23] Py：分块读取大文件
来源：http://www.52xcode.cn/Article/details/gt2gyzvphdo.html

for chunk in iter(lambda: f.read(8192), b""):
来源：http://www.52xcode.cn/Article/details/gt2epsogigf.html

[U24] Py：路径操作
来源：http://www.52xcode.cn/Article/details/gt2ntjieksc.html

Path("a/b.txt").parent.mkdir(parents=True, exist_ok=True)
来源：http://www.ydjk.org.cn/Article/details/gt2vezgyaoj.html

[U25] Py：CSV 按字典读
来源：http://www.ydjk.org.cn/Article/details/gt2ftdcmait.html

csv.DictReader(f)
来源：http://www.52xcode.cn/Article/details/gt2oowtrqtg.html

[U26] Py：并发下载
来源：http://www.ydjk.org.cn/Article/details/gt2zqlmtnst.html

ThreadPoolExecutor(max_workers=8).map(fetch, urls)
来源：http://www.52xcode.cn/Article/details/gt2uqveidrg.html

[U27] Py：异步 HTTP
来源：http://www.ydjk.org.cn/Article/details/gt2eljtnsii.html

aiohttp.ClientSession() 配合 async with
来源：http://www.52xcode.cn/Article/details/gt2neduhgsr.html

[U28] Py：类型别名
来源：http://www.ydjk.org.cn/Article/details/gt2quzpnfmi.html

UserId = int
来源：http://www.ydjk.org.cn/Article/details/gt2zmdhfkrh.html

[U29] Py：属性校验
来源：http://www.ydjk.org.cn/Article/details/gt2xzvzqeny.html

@property 与 @x.setter 配合
来源：http://www.52xcode.cn/Article/details/gt2mqpkcxic.html

[U30] Py：数据类
来源：http://www.52xcode.cn/Article/details/gt2zspnodtn.html

@dataclass(slots=True)
来源：http://www.52xcode.cn/Article/details/gt2qtbkmgwl.html

[U31] Py：单测
来源：http://www.52xcode.cn/Article/details/gt2ehskwkgm.html

python -m pytest -q
来源：http://www.52xcode.cn/Article/details/gt2gfqebzcb.html

[U32] Py：代码格式化
来源：http://www.ydjk.org.cn/Article/details/gt2gaxrmwux.html

ruff format . && ruff check --fix .
来源：http://www.52xcode.cn/Article/details/gt2khpxmpmn.html

[U33] Py：打包发布
来源：http://www.52xcode.cn/Article/details/gt2vszxswor.html

python -m build  （依赖 pyproject.toml）
来源：http://www.ydjk.org.cn/Article/details/gt2skywpuer.html

[U34] Py：判断编码
来源：http://www.52xcode.cn/Article/details/gt2vtcrjfhm.html

chardet.detect(raw)
来源：http://www.52xcode.cn/Article/details/gt2ppnbkvwm.html

[U35] Py：发送邮件
来源：http://www.ydjk.org.cn/Article/details/gt2yugtalhs.html

smtplib.SMTP_SSL(...).send_message(msg)
来源：http://www.52xcode.cn/Article/details/gt2sgirjxjb.html

[U36] Py：定时任务
来源：http://www.52xcode.cn/Article/details/gt2lzinukce.html

schedule.every(10).minutes.do(job)
来源：http://www.52xcode.cn/Article/details/gt2tditwglb.html

[U37] Py：读写 Excel
来源：http://www.ydjk.org.cn/Article/details/gt2jyqvqmov.html

pandas.read_excel / DataFrame.to_excel
来源：http://www.ydjk.org.cn/Article/details/gt2bkyjxtgs.html

[U38] Py：获取脚本所在目录
来源：http://www.52xcode.cn/Article/details/gt2phlsjoko.html

Path(__file__).resolve().parent
来源：http://www.ydjk.org.cn/Article/details/gt2sqyrcgcu.html

[U39] Py：判断是否在交互环境
来源：http://www.52xcode.cn/Article/details/gt2psyeicmt.html

sys.stdout.isatty()
来源：http://www.52xcode.cn/Article/details/gt2hrsdexny.html

[U40] Py：打印到标准错误
来源：http://www.ydjk.org.cn/Article/details/gt2vodaltua.html

print("err", file=sys.stderr)
来源：http://www.ydjk.org.cn/Article/details/gt2sycppfsl.html

[U41] PHP：初始化 Composer 项目
来源：http://www.52xcode.cn/Article/details/gt2xvszdtdn.html

composer init;  composer require guzzlehttp/guzzle
来源：http://www.ydjk.org.cn/Article/details/gt2ejhnfmih.html

[U42] PHP：PSR-4 自动加载
来源：http://www.52xcode.cn/Article/details/gt2ictfdhmo.html

"autoload": { "psr-4": { "App\\": "src/" } }
来源：http://www.ydjk.org.cn/Article/details/gt2aupxzdai.html

[U43] PHP：声明命名空间
来源：http://www.ydjk.org.cn/Article/details/gt2exbwvzio.html

namespace App\Http;
来源：http://www.52xcode.cn/Article/details/gt2fcjdiatq.html

[U44] PHP：开启严格类型
来源：http://www.ydjk.org.cn/Article/details/gt2goqlssux.html

declare(strict_types=1);
来源：http://www.ydjk.org.cn/Article/details/gt2ewqdkstw.html

[U45] PHP：类型声明与返回类型
来源：http://www.ydjk.org.cn/Article/details/gt2giyelihh.html

function add(int $a, int $b): int { return $a + $b; }
来源：http://www.ydjk.org.cn/Article/details/gt2gzekajyu.html

[U46] PHP：可空类型
来源：http://www.ydjk.org.cn/Article/details/gt2reujwwlx.html

?string $name = null
来源：http://www.ydjk.org.cn/Article/details/gt2guwzwyff.html

[U47] PHP：联合类型
来源：http://www.52xcode.cn/Article/details/gt2fpdbnand.html

int|string $id
来源：http://www.ydjk.org.cn/Article/details/gt2pyjvuytp.html

[U48] PHP：纯枚举
来源：http://www.ydjk.org.cn/Article/details/gt2pxqjnejz.html

enum Status: string { case Active = "active"; case Off = "off"; }
来源：http://www.ydjk.org.cn/Article/details/gt2jebzuigm.html

[U49] PHP：只读属性
来源：http://www.ydjk.org.cn/Article/details/gt2dwwfdhcd.html

public readonly string $name
来源：http://www.ydjk.org.cn/Article/details/gt2yjtizinz.html

[U50] PHP：构造器属性提升
来源：http://www.52xcode.cn/Article/details/gt2gxpdzace.html

public function __construct(private int $id) {}
来源：http://www.ydjk.org.cn/Article/details/gt2lzdwwbje.html

[U51] PHP：数组解构
来源：http://www.52xcode.cn/Article/details/gt2werkaenb.html

[$a, $b] = $arr;
来源：http://www.52xcode.cn/Article/details/gt2ieoohrzw.html

[U52] PHP：箭头函数
来源：http://www.52xcode.cn/Article/details/gt2oatmxpwx.html

$double = fn($x) => $x * 2;
来源：http://www.ydjk.org.cn/Article/details/gt2bbmoxmjy.html

[U53] PHP：空合并运算符
来源：http://www.ydjk.org.cn/Article/details/gt2voelbhox.html

$v = $a ?? $b ?? "default";
来源：http://www.ydjk.org.cn/Article/details/gt2lehbnysk.html

[U54] PHP：空安全调用
来源：http://www.52xcode.cn/Article/details/gt2qdbxdsva.html

$obj?->method()
来源：http://www.ydjk.org.cn/Article/details/gt2tzjdqyqv.html

[U55] PHP：match 表达式
来源：http://www.52xcode.cn/Article/details/gt2dypaajse.html

$s = match($x) { 1 => "一", default => "其他" };
来源：http://www.ydjk.org.cn/Article/details/gt2sgisvaml.html

[U56] PHP：命名参数
来源：http://www.52xcode.cn/Article/details/gt2bgxobrpr.html

f(a: 1, b: 2)
来源：http://www.ydjk.org.cn/Article/details/gt2dquixzvy.html

[U57] PHP：字符串插值
来源：http://www.ydjk.org.cn/Article/details/gt2whuekixh.html

"值: {$a}"
来源：http://www.ydjk.org.cn/Article/details/gt2eynkhbba.html

[U58] PHP：数组三件套
来源：http://www.52xcode.cn/Article/details/gt2ewbpwsmj.html

array_map($f, $a);  array_filter($a, $f);  array_reduce($a, $f, 0);
来源：http://www.ydjk.org.cn/Article/details/gt2ihoiithu.html

[U59] PHP：自定义排序
来源：http://www.ydjk.org.cn/Article/details/gt2bdxokjqx.html

usort($arr, fn($a, $b) => $a["age"] <=> $b["age"]);
来源：http://www.52xcode.cn/Article/details/gt2nhehfeex.html

[U60] PHP：JSON 编解码
来源：http://www.52xcode.cn/Article/details/gt2gspmhcko.html

json_encode($d, JSON_UNESCAPED_UNICODE);  json_decode($s, true);
来源：http://www.52xcode.cn/Article/details/gt2kussetnq.html

[U61] PHP：正则
来源：http://www.52xcode.cn/Article/details/gt2cbwntoee.html

preg_match('/(\d+)/', $s, $m);  preg_replace('/\d+/', '#', $s);
来源：http://www.52xcode.cn/Article/details/gt2flhqvmdh.html

[U62] PHP：日期对象
来源：http://www.52xcode.cn/Article/details/gt2cibvblpr.html

(new DateTimeImmutable())->format("Y-m-d");
来源：http://www.52xcode.cn/Article/details/gt2ixfqfqbe.html

[U63] PHP：文件读写
来源：http://www.ydjk.org.cn/Article/details/gt2ibxcunxj.html

file_get_contents($f);  file_put_contents($f, $data);
来源：http://www.52xcode.cn/Article/details/gt2sjjfymvt.html

[U64] PHP：目录遍历
来源：http://www.ydjk.org.cn/Article/details/gt2xnseuuoa.html

glob("dir/*.php");  scandir("dir");
来源：http://www.ydjk.org.cn/Article/details/gt2olfcnbif.html

[U65] PHP：会话
来源：http://www.52xcode.cn/Article/details/gt2bdntjfga.html

session_start();  $_SESSION["uid"] = 1;
来源：http://www.52xcode.cn/Article/details/gt2jsydlhco.html

[U66] PHP：设置 Cookie
来源：http://www.52xcode.cn/Article/details/gt2ljjbrovh.html

setcookie("token", $v, ["httponly" => true, "samesite" => "Lax"]);
来源：http://www.52xcode.cn/Article/details/gt2fjwrahnw.html

[U67] PHP：处理文件上传
来源：http://www.52xcode.cn/Article/details/gt2sfauhxsu.html

$_FILES["file"]["tmp_name"] 与 move_uploaded_file()
来源：http://www.52xcode.cn/Article/details/gt2nvrvfhlb.html

[U68] PHP：PDO 连接
来源：http://www.52xcode.cn/Article/details/gt2upakpbdd.html

$pdo = new PDO("mysql:host=localhost;dbname=app", "root", "");
来源：http://www.ydjk.org.cn/Article/details/gt2sonakcvh.html

[U69] PHP：PDO 预处理
来源：http://www.52xcode.cn/Article/details/gt2hinilxvv.html

$stmt = $pdo->prepare("SELECT * FROM users WHERE id = ?");  $stmt->execute([$id]);
来源：http://www.52xcode.cn/Article/details/gt2ftvrwxsw.html

[U70] PHP：PDO 事务
来源：http://www.52xcode.cn/Article/details/gt2csxqwieg.html

$pdo->beginTransaction();  $pdo->commit();  $pdo->rollBack();
来源：http://www.52xcode.cn/Article/details/gt2ljsvuegr.html

[U71] PHP：抛出异常
来源：http://www.ydjk.org.cn/Article/details/gt2pszapeej.html

throw new RuntimeException("失败", 500);
来源：http://www.ydjk.org.cn/Article/details/gt2gzmyvqli.html

[U72] PHP：写错误日志
来源：http://www.52xcode.cn/Article/details/gt2zzlfwdcr.html

error_log("失败: " . $e->getMessage());
来源：http://www.ydjk.org.cn/Article/details/gt2jzceyzck.html

[U73] PHP：读取 ini 配置
来源：http://www.52xcode.cn/Article/details/gt2przdrbwv.html

parse_ini_file("config.ini", true)
来源：http://www.52xcode.cn/Article/details/gt2zkssxbir.html

[U74] PHP：读取环境变量
来源：http://www.ydjk.org.cn/Article/details/gt2aisqfgut.html

getenv("APP_ENV") ?: "production"
来源：http://www.52xcode.cn/Article/details/gt2fkugctoa.html

[U75] PHP：依赖注入
来源：http://www.ydjk.org.cn/Article/details/gt2gjlxyfqu.html

composer require psr/container
来源：http://www.ydjk.org.cn/Article/details/gt2afsskgss.html

[U76] PHP：简单路由
来源：http://www.ydjk.org.cn/Article/details/gt2qyvrsxic.html

$path = parse_url($_SERVER["REQUEST_URI"], PHP_URL_PATH);
来源：http://www.52xcode.cn/Article/details/gt2ikfyxvtv.html

[U77] PHP：模板渲染
来源：http://www.ydjk.org.cn/Article/details/gt2mflurfsq.html

composer require twig/twig
来源：http://www.52xcode.cn/Article/details/gt2kghskqwj.html

[U78] PHP：单元测试
来源：http://www.ydjk.org.cn/Article/details/gt2zgmwgdrd.html

composer require --dev phpunit/phpunit
来源：http://www.ydjk.org.cn/Article/details/gt2ddajglkp.html

[U79] PHP：静态分析
来源：http://www.52xcode.cn/Article/details/gt2breqcppb.html

composer require --dev phpstan/phpstan
来源：http://www.52xcode.cn/Article/details/gt2mctgkcid.html

[U80] PHP：代码规范修复
来源：http://www.52xcode.cn/Article/details/gt2insgaiyc.html

composer require --dev friendsofphp/php-cs-fixer
来源：http://www.ydjk.org.cn/Article/details/gt2rgskfzis.html

[U81] JS：初始化项目
来源：http://www.ydjk.org.cn/Article/details/gt2egjcipev.html

npm init -y;  npm i express
来源：http://www.52xcode.cn/Article/details/gt2xcpzsrok.html

[U82] JS：package.json 脚本
来源：http://www.ydjk.org.cn/Article/details/gt2tqwzbnkj.html

"scripts": { "dev": "vite", "build": "vite build" }
来源：http://www.ydjk.org.cn/Article/details/gt2ctwcgwse.html

[U83] JS：ES Module 导入导出
来源：http://www.ydjk.org.cn/Article/details/gt2tjokhqre.html

export const a = 1;  import { a } from "./m.js";
来源：http://www.52xcode.cn/Article/details/gt2wjjhrygw.html

[U84] JS：CommonJS 写法
来源：http://www.ydjk.org.cn/Article/details/gt2gpekiyba.html

module.exports = { a };  const { a } = require("./m");
来源：http://www.52xcode.cn/Article/details/gt2lvzgxigk.html

[U85] JS：可选链
来源：http://www.52xcode.cn/Article/details/gt2nqyxmfra.html

a?.b?.c
来源：http://www.52xcode.cn/Article/details/gt2qjwavvul.html

[U86] JS：空值合并
来源：http://www.ydjk.org.cn/Article/details/gt2lnvbbhqa.html

a ?? b
来源：http://www.ydjk.org.cn/Article/details/gt2pfuoketp.html

[U87] JS：解构默认值
来源：http://www.ydjk.org.cn/Article/details/gt2wtauxwox.html

const { a = 1, b = 2 } = obj;
来源：http://www.52xcode.cn/Article/details/gt2qndaekss.html

[U88] JS：对象展开合并
来源：http://www.52xcode.cn/Article/details/gt2qwmmludx.html

{ ...a, ...b }
来源：http://www.52xcode.cn/Article/details/gt2wbxbdfpq.html

[U89] JS：数组去重
来源：http://www.ydjk.org.cn/Article/details/gt2otmgkaov.html

[...new Set(arr)]
来源：http://www.52xcode.cn/Article/details/gt2qgggapxk.html

[U90] JS：数字数组排序
来源：http://www.ydjk.org.cn/Article/details/gt2nuyhksvz.html

[...arr].sort((a, b) => a - b)
来源：http://www.ydjk.org.cn/Article/details/gt2wroudmnh.html

[U91] JS：对象键值遍历
来源：http://www.ydjk.org.cn/Article/details/gt2ltkwnbgy.html

Object.entries(obj).forEach(([k, v]) => {});
来源：http://www.ydjk.org.cn/Article/details/gt2lznjpzsn.html

[U92] JS：深拷贝
来源：http://www.ydjk.org.cn/Article/details/gt2rwzrxove.html

structuredClone(obj)
来源：http://www.52xcode.cn/Article/details/gt2hdlmpctm.html

[U93] JS：模板字符串
来源：http://www.52xcode.cn/Article/details/gt2tiywxvjg.html

`共 ${n} 条`
来源：http://www.ydjk.org.cn/Article/details/gt2lbontkky.html

[U94] JS：箭头函数
来源：http://www.52xcode.cn/Article/details/gt2fwhgqirx.html

const double = x => x * 2;
来源：http://www.ydjk.org.cn/Article/details/gt2fjghggoo.html

[U95] JS：Promise 包装
来源：http://www.52xcode.cn/Article/details/gt2qosxvofy.html

new Promise((resolve, reject) => {})
来源：http://www.52xcode.cn/Article/details/gt2kzyknqzc.html

[U96] JS：async/await 与异常
来源：http://www.52xcode.cn/Article/details/gt2epqsuwbq.html

try { const d = await f(); } catch (e) { console.error(e); }
来源：http://www.ydjk.org.cn/Article/details/gt2powyvhxw.html

[U97] JS：并发请求
来源：http://www.ydjk.org.cn/Article/details/gt2vlspwxpp.html

await Promise.all(urls.map(u => fetch(u)))
来源：http://www.ydjk.org.cn/Article/details/gt2dbpibllh.html

[U98] JS：fetch 带 JSON
来源：http://www.ydjk.org.cn/Article/details/gt2uhkgsnqi.html

await fetch(url, { method: "POST", headers: { "Content-Type": "application/json" }, body: JSON.stringify(d) })
来源：http://www.ydjk.org.cn/Article/details/gt2oyifbtht.html

[U99] JS：事件监听
来源：http://www.52xcode.cn/Article/details/gt2dxvayija.html

el.addEventListener("click", e => {})
来源：http://www.52xcode.cn/Article/details/gt2tdxpxbnl.html

[U100] JS：DOM 查询
来源：http://www.ydjk.org.cn/Article/details/gt2wjthayiw.html

document.querySelector(".item")
来源：http://www.ydjk.org.cn/Article/details/gt2jnwtkdtj.html

[U101] JS：classList 操作
来源：http://www.ydjk.org.cn/Article/details/gt2nslltxtx.html

el.classList.toggle("active")
来源：http://www.52xcode.cn/Article/details/gt2pinfbxok.html

[U102] JS：本地存储
来源：http://www.ydjk.org.cn/Article/details/gt2aelewzwp.html

localStorage.setItem("k", JSON.stringify(v))
来源：http://www.ydjk.org.cn/Article/details/gt2wafepgsy.html

[U103] JS：定时器
来源：http://www.ydjk.org.cn/Article/details/gt2nvtaapyi.html

setTimeout(fn, 1000);  setInterval(fn, 1000);
来源：http://www.52xcode.cn/Article/details/gt2upvaijly.html

[U104] JS：防抖
来源：http://www.52xcode.cn/Article/details/gt2pdzgmiqs.html

const debounce = (fn, ms) => { let t; return (...a) => { clearTimeout(t); t = setTimeout(() => fn(...a), ms); }; };
来源：http://www.52xcode.cn/Article/details/gt2cwdyperk.html

[U105] JS：节流
来源：http://www.ydjk.org.cn/Article/details/gt2pdkhmptq.html

const throttle = (fn, ms) => { let last = 0; return (...a) => { const n = Date.now(); if (n - last >= ms) { last = n; fn(...a); } }; };
来源：http://www.52xcode.cn/Article/details/gt2cponkbla.html

[U106] JS：日期格式化
来源：http://www.52xcode.cn/Article/details/gt2brwnbufb.html

new Intl.DateTimeFormat("zh-CN", { dateStyle: "medium" }).format(new Date())
来源：http://www.ydjk.org.cn/Article/details/gt2vwzitidn.html

[U107] JS：数字千分位
来源：http://www.52xcode.cn/Article/details/gt2isfgwtxs.html

new Intl.NumberFormat("en-US").format(1234567)
来源：http://www.52xcode.cn/Article/details/gt2xwjpernk.html

[U108] JS：随机整数
来源：http://www.52xcode.cn/Article/details/gt2atufjpfh.html

Math.floor(Math.random() * (max - min + 1)) + min
来源：http://www.52xcode.cn/Article/details/gt2bjzgixhk.html

[U109] JS：数组分组
来源：http://www.52xcode.cn/Article/details/gt2stjpdyer.html

Object.groupBy(arr, x => x.type)
来源：http://www.ydjk.org.cn/Article/details/gt2jdlnzbdi.html

[U110] JS：数组分块
来源：http://www.ydjk.org.cn/Article/details/gt2bzotrfqi.html

arr.reduce((acc, x, i) => (i % size ? acc : [...acc, arr.slice(i, i + size)]), [])
来源：http://www.ydjk.org.cn/Article/details/gt2olscgyre.html

[U111] JS：对象转 Map
来源：http://www.ydjk.org.cn/Article/details/gt2qqlenzag.html

new Map(Object.entries(obj))
来源：http://www.52xcode.cn/Article/details/gt2lnigqeat.html

[U112] JS：字符串补位
来源：http://www.52xcode.cn/Article/details/gt2vuuysxoj.html

"7".padStart(3, "0")
来源：http://www.ydjk.org.cn/Article/details/gt2giwpqlzm.html

[U113] JS：正则替换全部
来源：http://www.ydjk.org.cn/Article/details/gt2yiomufos.html

s.replaceAll("a", "b")
来源：http://www.ydjk.org.cn/Article/details/gt2mhfmswyu.html

[U114] JS：JSON 深比较
来源：http://www.ydjk.org.cn/Article/details/gt2nhlajkkh.html

JSON.stringify(a) === JSON.stringify(b)
来源：http://www.52xcode.cn/Article/details/gt2zofigkbg.html

[U115] JS：生成 UUID
来源：http://www.ydjk.org.cn/Article/details/gt2dlzucaxf.html

crypto.randomUUID()
来源：http://www.52xcode.cn/Article/details/gt2uucnepsh.html

[U116] JS：类型检查（JSDoc）
来源：http://www.ydjk.org.cn/Article/details/gt2kuruymun.html

/** @param {string} name */ function f(name) {}
来源：http://www.52xcode.cn/Article/details/gt2mxymrqfl.html

[U117] JS：单元测试
来源：http://www.52xcode.cn/Article/details/gt2zbtzftes.html

npm i -D vitest;  npx vitest
来源：http://www.ydjk.org.cn/Article/details/gt2crczeytd.html

[U118] JS：开发服务器
来源：http://www.52xcode.cn/Article/details/gt2aisveytd.html

npm i -D vite;  npx vite
来源：http://www.52xcode.cn/Article/details/gt2mtvfopsv.html

[U119] JS：生产构建
来源：http://www.ydjk.org.cn/Article/details/gt2ezptqyvn.html

npx vite build
来源：http://www.52xcode.cn/Article/details/gt2rnreisqf.html

[U120] JS：读取环境变量（Vite）
来源：http://www.ydjk.org.cn/Article/details/gt2itdtorrv.html

import.meta.env.VITE_API_URL
来源：http://www.ydjk.org.cn/Article/details/gt2cdjnyymj.html

================================================================================
来源：http://www.ydjk.org.cn/Article/details/gt2csazaqmj.html

统计汇总
来源：http://www.ydjk.org.cn/Article/details/gt2zncorkev.html

================================================================================
来源：http://www.52xcode.cn/Article/details/gt2broqkbfs.html

按语言统计（条）：
来源：http://www.ydjk.org.cn/Article/details/gt2lhzinkxs.html

Python ......... 252
来源：http://www.ydjk.org.cn/Article/details/gt2fjaphbfx.html

PHP ............ 252
来源：http://www.52xcode.cn/Article/details/gt2fpdqkvfs.html

JavaScript ..... 252
来源：http://www.52xcode.cn/Article/details/gt2cikixnuq.html

TypeScript ..... 212
来源：http://www.ydjk.org.cn/Article/details/gt2ceazgabb.html

Java ........... 212
来源：http://www.52xcode.cn/Article/details/gt2yjclkovm.html

Go ............. 212
来源：http://www.ydjk.org.cn/Article/details/gt2fetlpwgq.html

Ruby ........... 212
来源：http://www.ydjk.org.cn/Article/details/gt2fnrstglv.html

C# ............. 212
来源：http://www.52xcode.cn/Article/details/gt2ggtwtmfo.html

C .............. 30
来源：http://www.ydjk.org.cn/Article/details/gt2uktrztmy.html

C++ ............ 30
来源：http://www.ydjk.org.cn/Article/details/gt2rvxjvftl.html

SQL ............ 90
来源：http://www.52xcode.cn/Article/details/gt2qsztsxoa.html

Bash ........... 80
来源：http://www.ydjk.org.cn/Article/details/gt2fullmvce.html

Kotlin ......... 15
来源：http://www.52xcode.cn/Article/details/gt2ukrxgxnz.html

Swift .......... 15
来源：http://www.ydjk.org.cn/Article/details/gt2ikfnnwmo.html

Lua ............ 10
来源：http://www.ydjk.org.cn/Article/details/gt2svonllth.html

Perl ........... 10
来源：http://www.52xcode.cn/Article/details/gt2xemmigll.html

Scala .......... 10
来源：http://www.ydjk.org.cn/Article/details/gt2kymcvapu.html

------------------------------------
来源：http://www.ydjk.org.cn/Article/details/gt2tludufum.html

合计 ........... 2106 条
来源：http://www.52xcode.cn/Article/details/gt2rcmtbwbk.html

按章节统计：
来源：http://www.ydjk.org.cn/Article/details/gt2dolurdrv.html

A 基础语法与类型       26 个任务 × 8 语言 =  208
来源：http://www.ydjk.org.cn/Article/details/gt2mwdpnzfv.html

B 流程控制             16 个任务 × 8 语言 =  128
来源：http://www.ydjk.org.cn/Article/details/gt2rrwzhjkp.html

C 函数与作用域         16 个任务 × 8 语言 =  128
来源：http://www.ydjk.org.cn/Article/details/gt2rpwkonzt.html

D 数组 / 列表 / 集合   26 个任务 × 8 语言 =  208
来源：http://www.ydjk.org.cn/Article/details/gt2qkgdmqdx.html

E 字符串处理           22 个任务 × 8 语言 =  176
来源：http://www.ydjk.org.cn/Article/details/gt2lejmmdvd.html

F 文件与目录           12 个任务 × 8 语言 =   96
来源：http://www.ydjk.org.cn/Article/details/gt2uptrucek.html

G 面向对象             16 个任务 × 8 语言 =  128
来源：http://www.52xcode.cn/Article/details/gt2eazmpnnm.html

H 异常与错误处理       10 个任务 × 8 语言 =   80
来源：http://www.52xcode.cn/Article/details/gt2panpqtxq.html

I 正则表达式            8 个任务 × 8 语言 =   64
来源：http://www.52xcode.cn/Article/details/gt2tytiabwb.html

J 日期与时间           10 个任务 × 8 语言 =   80
来源：http://www.52xcode.cn/Article/details/gt2arlcglvu.html

K JSON 与序列化         8 个任务 × 8 语言 =   64
来源：http://www.ydjk.org.cn/Article/details/gt2npgtwtic.html

L 网络请求              8 个任务 × 8 语言 =   64
来源：http://www.ydjk.org.cn/Article/details/gt2blitllea.html


<!-- 参考信息 -->