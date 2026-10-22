代发 wailian999

val a = 1;  var b = 2
来源：http://www.52xcode.cn/Article/details/gt2asosweeb.html

[T53] Scala：字符串插值
来源：http://www.ydjk.org.cn/Article/details/gt2stjzkxii.html

s"值: $b"
来源：http://www.52xcode.cn/Article/details/gt2bequlcrj.html

[T54] Scala：集合映射
来源：http://www.52xcode.cn/Article/details/gt2qbluqsnf.html

List(1, 2, 3).map(_ * 2)
来源：http://www.ydjk.org.cn/Article/details/gt2dduinctq.html

[T55] Scala：集合过滤
来源：http://www.52xcode.cn/Article/details/gt2ebnuceom.html

List(1, 2, 3).filter(_ > 1)
来源：http://www.ydjk.org.cn/Article/details/gt2mbvxoazy.html

[T56] Scala：样例类
来源：http://www.ydjk.org.cn/Article/details/gt2lnopgpai.html

case class User(name: String, age: Int)
来源：http://www.52xcode.cn/Article/details/gt2fhwlburx.html

[T57] Scala：模式匹配
来源：http://www.ydjk.org.cn/Article/details/gt2yofsagln.html

x match { case 1 => "一"; case _ => "其他" }
来源：http://www.52xcode.cn/Article/details/gt2dpehwwdv.html

[T58] Scala：函数定义
来源：http://www.ydjk.org.cn/Article/details/gt2qglxvwpz.html

def add(a: Int, b: Int): Int = a + b
来源：http://www.ydjk.org.cn/Article/details/gt2aayzsmow.html

[T59] Scala：循环
来源：http://www.ydjk.org.cn/Article/details/gt2luhsnsad.html

for (i <- 1 to 10) println(i)
来源：http://www.ydjk.org.cn/Article/details/gt2wvmhxrrb.html

[T60] Scala：折叠
来源：http://www.52xcode.cn/Article/details/gt2qcbbqtgh.html

List(1, 2, 3).foldLeft(0)(_ + _)
来源：http://www.ydjk.org.cn/Article/details/gt2vzqttyeb.html

================================================================================
来源：http://www.52xcode.cn/Article/details/gt2kqafzhpf.html

U. 高频实用片段（Python / PHP / JavaScript 各 40 条）
来源：http://www.ydjk.org.cn/Article/details/gt2bpiretud.html

================================================================================
来源：http://www.52xcode.cn/Article/details/gt2qnxenqiw.html

[U01] Py：创建虚拟环境
来源：http://www.52xcode.cn/Article/details/gt2gflmbfgi.html

python -m venv .venv && source .venv/bin/activate
来源：http://www.52xcode.cn/Article/details/gt2lqdifmad.html

[U02] Py：导出 / 安装依赖
来源：http://www.ydjk.org.cn/Article/details/gt2yvntufrm.html

pip freeze > requirements.txt;  pip install -r requirements.txt
来源：http://www.ydjk.org.cn/Article/details/gt2kbhlffza.html

[U03] Py：加载 .env 配置
来源：http://www.ydjk.org.cn/Article/details/gt2udihnzea.html

from dotenv import load_dotenv; load_dotenv()
来源：http://www.52xcode.cn/Article/details/gt2uwugsmvc.html

[U04] Py：变量调试打印
来源：http://www.52xcode.cn/Article/details/gt2keqrcvxe.html

print(f"{x=}")            # 输出 x=值，Python 3.8+
来源：http://www.52xcode.cn/Article/details/gt2jxityncf.html

[U05] Py：列表去重且保序
来源：http://www.ydjk.org.cn/Article/details/gt2fbtzwsse.html

list(dict.fromkeys(arr))
来源：http://www.ydjk.org.cn/Article/details/gt2krzulmhw.html

[U06] Py：合并两个字典
来源：http://www.52xcode.cn/Article/details/gt2pkzgoisx.html

{**a, **b}
来源：http://www.ydjk.org.cn/Article/details/gt2ejxxdhik.html

[U07] Py：反转字典键值
来源：http://www.ydjk.org.cn/Article/details/gt2uptqonsb.html

{v: k for k, v in d.items()}
来源：http://www.ydjk.org.cn/Article/details/gt2ylzpmgnj.html

[U08] Py：展平二维列表
来源：http://www.ydjk.org.cn/Article/details/gt2xvdeycgw.html

[y for x in nested for y in x]
来源：http://www.52xcode.cn/Article/details/gt2xryjhucl.html

[U09] Py：字典取最大值的键
来源：http://www.52xcode.cn/Article/details/gt2uolrflki.html

max(d, key=d.get)
来源：http://www.52xcode.cn/Article/details/gt2srlxssrm.html

[U10] Py：按值排序字典
来源：http://www.ydjk.org.cn/Article/details/gt2divxflqn.html

dict(sorted(d.items(), key=lambda kv: kv[1]))
来源：http://www.ydjk.org.cn/Article/details/gt2tmtrispq.html

[U11] Py：生成器表达式
来源：http://www.ydjk.org.cn/Article/details/gt2drkfeuxr.html

(x * 2 for x in arr)
来源：http://www.52xcode.cn/Article/details/gt2bveaqvox.html

[U12] Py：取出现最多的 3 个元素
来源：http://www.ydjk.org.cn/Article/details/gt2dbvijzxk.html

Counter(arr).most_common(3)
来源：http://www.52xcode.cn/Article/details/gt2luwdmioi.html

[U13] Py：固定长度队列
来源：http://www.52xcode.cn/Article/details/gt2zbbbtnds.html

deque(maxlen=10)
来源：http://www.ydjk.org.cn/Article/details/gt2stuhkkrx.html

[U14] Py：分组收集到列表
来源：http://www.52xcode.cn/Article/details/gt2eoexsqpq.html

defaultdict(list)
来源：http://www.ydjk.org.cn/Article/details/gt2iivxvnrk.html

[U15] Py：高精度计时
来源：http://www.ydjk.org.cn/Article/details/gt2unyyhfqo.html

t = time.perf_counter()
来源：http://www.ydjk.org.cn/Article/details/gt2qwysiihy.html

[U16] Py：命令行参数解析
来源：http://www.52xcode.cn/Article/details/gt2csovvlcb.html

ap = argparse.ArgumentParser();  ap.add_argument("--name");  args = ap.parse_args()
来源：http://www.ydjk.org.cn/Article/details/gt2aksxigzh.html

[U17] Py：初始化日志
来源：http://www.52xcode.cn/Article/details/gt2ycuyygat.html

logging.basicConfig(level=logging.INFO)
来源：http://www.ydjk.org.cn/Article/details/gt2fhktowto.html

[U18] Py：预编译正则
来源：http://www.52xcode.cn/Article/details/gt2dlvqulaq.html

pat = re.compile(r"\d+")
来源：http://www.52xcode.cn/Article/details/gt2kydzfdvk.html

[U19] Py：正则替换带回调
来源：http://www.52xcode.cn/Article/details/gt2gcehipro.html

re.sub(r"\d+", lambda m: str(int(m.group()) * 2), s)
来源：http://www.52xcode.cn/Article/details/gt2gxyibzrh.html

[U20] Py：缓存函数结果
来源：http://www.52xcode.cn/Article/details/gt2vmvpguan.html

@functools.lru_cache(maxsize=None)
来源：http://www.ydjk.org.cn/Article/details/gt2kcetftxu.html

[U21] Py：自定义上下文管理器
来源：http://www.52xcode.cn/Article/details/gt2bpsgqijk.html

@contextlib.contextmanager
来源：http://www.ydjk.org.cn/Article/details/gt2mwiedtem.html

[U22] Py：矩阵转置
来源：http://www.ydjk.org.cn/Article/details/gt2uthtpwjw.html

list(zip(*m))
来源：http://www.52xcode.cn/Article/details/gt2dunzwrma.html

[U23] Py：分块读取大文件
来源：http://www.ydjk.org.cn/Article/details/gt2hklwocdr.html

for chunk in iter(lambda: f.read(8192), b""):
来源：http://www.52xcode.cn/Article/details/gt2yalcctik.html

[U24] Py：路径操作
来源：http://www.ydjk.org.cn/Article/details/gt2hygboupy.html

Path("a/b.txt").parent.mkdir(parents=True, exist_ok=True)
来源：http://www.52xcode.cn/Article/details/gt2ktcdkxdv.html

[U25] Py：CSV 按字典读
来源：http://www.52xcode.cn/Article/details/gt2uewdsylh.html

csv.DictReader(f)
来源：http://www.ydjk.org.cn/Article/details/gt2fssmmbrc.html

[U26] Py：并发下载
来源：http://www.52xcode.cn/Article/details/gt2jczyrcwc.html

ThreadPoolExecutor(max_workers=8).map(fetch, urls)
来源：http://www.ydjk.org.cn/Article/details/gt2uuacooge.html

[U27] Py：异步 HTTP
来源：http://www.ydjk.org.cn/Article/details/gt2upuvhcxo.html

aiohttp.ClientSession() 配合 async with
来源：http://www.ydjk.org.cn/Article/details/gt2lzmdmaso.html

[U28] Py：类型别名
来源：http://www.52xcode.cn/Article/details/gt2anacyajg.html

UserId = int
来源：http://www.ydjk.org.cn/Article/details/gt2wubionms.html

[U29] Py：属性校验
来源：http://www.52xcode.cn/Article/details/gt2hmeenwzz.html

@property 与 @x.setter 配合
来源：http://www.52xcode.cn/Article/details/gt2zvlkvjaw.html

[U30] Py：数据类
来源：http://www.52xcode.cn/Article/details/gt2diftamgm.html

@dataclass(slots=True)
来源：http://www.52xcode.cn/Article/details/gt2bctcecga.html

[U31] Py：单测
来源：http://www.ydjk.org.cn/Article/details/gt2lsunfeyj.html

python -m pytest -q
来源：http://www.52xcode.cn/Article/details/gt2rijybelq.html

[U32] Py：代码格式化
来源：http://www.ydjk.org.cn/Article/details/gt2htrkmkgm.html

ruff format . && ruff check --fix .
来源：http://www.52xcode.cn/Article/details/gt2cjfmyjfm.html

[U33] Py：打包发布
来源：http://www.ydjk.org.cn/Article/details/gt2xchjpcyz.html

python -m build  （依赖 pyproject.toml）
来源：http://www.ydjk.org.cn/Article/details/gt2ultgpcfg.html

[U34] Py：判断编码
来源：http://www.52xcode.cn/Article/details/gt2iijngcbg.html

chardet.detect(raw)
来源：http://www.52xcode.cn/Article/details/gt2xykdroab.html

[U35] Py：发送邮件
来源：http://www.52xcode.cn/Article/details/gt2crcwsygu.html

smtplib.SMTP_SSL(...).send_message(msg)
来源：http://www.ydjk.org.cn/Article/details/gt2sgahohzj.html

[U36] Py：定时任务
来源：http://www.ydjk.org.cn/Article/details/gt2iquwfebt.html

schedule.every(10).minutes.do(job)
来源：http://www.52xcode.cn/Article/details/gt2zwzfhkml.html

[U37] Py：读写 Excel
来源：http://www.ydjk.org.cn/Article/details/gt2ckxennvt.html

pandas.read_excel / DataFrame.to_excel
来源：http://www.ydjk.org.cn/Article/details/gt2nywuyvfv.html

[U38] Py：获取脚本所在目录
来源：http://www.ydjk.org.cn/Article/details/gt2yukdxytd.html

Path(__file__).resolve().parent
来源：http://www.ydjk.org.cn/Article/details/gt2sihmylnl.html

[U39] Py：判断是否在交互环境
来源：http://www.52xcode.cn/Article/details/gt2ujpubgcl.html

sys.stdout.isatty()
来源：http://www.ydjk.org.cn/Article/details/gt2pwtmfdrj.html

[U40] Py：打印到标准错误
来源：http://www.52xcode.cn/Article/details/gt2ubuoyoav.html

print("err", file=sys.stderr)
来源：http://www.52xcode.cn/Article/details/gt2huqgwphq.html

[U41] PHP：初始化 Composer 项目
来源：http://www.ydjk.org.cn/Article/details/gt2wpedatna.html

composer init;  composer require guzzlehttp/guzzle
来源：http://www.52xcode.cn/Article/details/gt2hpoptypo.html

[U42] PHP：PSR-4 自动加载
来源：http://www.52xcode.cn/Article/details/gt2bzlsqexg.html

"autoload": { "psr-4": { "App\\": "src/" } }
来源：http://www.ydjk.org.cn/Article/details/gt2piyucnby.html

[U43] PHP：声明命名空间
来源：http://www.52xcode.cn/Article/details/gt2unzzuaea.html

namespace App\Http;
来源：http://www.52xcode.cn/Article/details/gt2amfoqqjc.html

[U44] PHP：开启严格类型
来源：http://www.52xcode.cn/Article/details/gt2txcqaopu.html

declare(strict_types=1);
来源：http://www.52xcode.cn/Article/details/gt2ztwnlgca.html

[U45] PHP：类型声明与返回类型
来源：http://www.52xcode.cn/Article/details/gt2wsvtobtl.html

function add(int $a, int $b): int { return $a + $b; }
来源：http://www.52xcode.cn/Article/details/gt2ttycgjuv.html

[U46] PHP：可空类型
来源：http://www.52xcode.cn/Article/details/gt2xlgpxtio.html

?string $name = null
来源：http://www.ydjk.org.cn/Article/details/gt2tknjtvin.html

[U47] PHP：联合类型
来源：http://www.52xcode.cn/Article/details/gt2uetlihzf.html

int|string $id
来源：http://www.52xcode.cn/Article/details/gt2reheasxx.html

[U48] PHP：纯枚举
来源：http://www.ydjk.org.cn/Article/details/gt2lkxvolma.html

enum Status: string { case Active = "active"; case Off = "off"; }
来源：http://www.52xcode.cn/Article/details/gt2bjnmwaow.html

[U49] PHP：只读属性
来源：http://www.52xcode.cn/Article/details/gt2gnytidby.html

public readonly string $name
来源：http://www.ydjk.org.cn/Article/details/gt2edbsxuag.html

[U50] PHP：构造器属性提升
来源：http://www.ydjk.org.cn/Article/details/gt2iwlpudjt.html

public function __construct(private int $id) {}
来源：http://www.52xcode.cn/Article/details/gt2zwbmrhdx.html

[U51] PHP：数组解构
来源：http://www.ydjk.org.cn/Article/details/gt2qmlyhhvx.html

[$a, $b] = $arr;
来源：http://www.ydjk.org.cn/Article/details/gt2zahjfdkc.html

[U52] PHP：箭头函数
来源：http://www.52xcode.cn/Article/details/gt2bwqegtym.html

$double = fn($x) => $x * 2;
来源：http://www.52xcode.cn/Article/details/gt2jfidyxpd.html

[U53] PHP：空合并运算符
来源：http://www.52xcode.cn/Article/details/gt2esijolwr.html

$v = $a ?? $b ?? "default";
来源：http://www.52xcode.cn/Article/details/gt2fypuayrl.html

[U54] PHP：空安全调用
来源：http://www.52xcode.cn/Article/details/gt2elrxnbiq.html

$obj?->method()
来源：http://www.ydjk.org.cn/Article/details/gt2wiaelkdj.html

[U55] PHP：match 表达式
来源：http://www.ydjk.org.cn/Article/details/gt2eoebnwqr.html

$s = match($x) { 1 => "一", default => "其他" };
来源：http://www.ydjk.org.cn/Article/details/gt2hddbijxb.html

[U56] PHP：命名参数
来源：http://www.52xcode.cn/Article/details/gt2qbqymsqq.html

f(a: 1, b: 2)
来源：http://www.52xcode.cn/Article/details/gt2swatlvxf.html

[U57] PHP：字符串插值
来源：http://www.ydjk.org.cn/Article/details/gt2lljacije.html

"值: {$a}"
来源：http://www.ydjk.org.cn/Article/details/gt2gncsgbcu.html

[U58] PHP：数组三件套
来源：http://www.ydjk.org.cn/Article/details/gt2jdenhnag.html

array_map($f, $a);  array_filter($a, $f);  array_reduce($a, $f, 0);
来源：http://www.52xcode.cn/Article/details/gt2igkuocbh.html

[U59] PHP：自定义排序
来源：http://www.52xcode.cn/Article/details/gt2cbhbdvpy.html

usort($arr, fn($a, $b) => $a["age"] <=> $b["age"]);
来源：http://www.52xcode.cn/Article/details/gt2huimyfea.html

[U60] PHP：JSON 编解码
来源：http://www.52xcode.cn/Article/details/gt2sfakjayv.html

json_encode($d, JSON_UNESCAPED_UNICODE);  json_decode($s, true);
来源：http://www.ydjk.org.cn/Article/details/gt2srkzptbn.html

[U61] PHP：正则
来源：http://www.ydjk.org.cn/Article/details/gt2iykkwape.html

preg_match('/(\d+)/', $s, $m);  preg_replace('/\d+/', '#', $s);
来源：http://www.52xcode.cn/Article/details/gt2wrkdcfbh.html

[U62] PHP：日期对象
来源：http://www.ydjk.org.cn/Article/details/gt2igzrntgf.html

(new DateTimeImmutable())->format("Y-m-d");
来源：http://www.52xcode.cn/Article/details/gt2heznxylj.html

[U63] PHP：文件读写
来源：http://www.52xcode.cn/Article/details/gt2ztkobqnx.html

file_get_contents($f);  file_put_contents($f, $data);
来源：http://www.ydjk.org.cn/Article/details/gt2elhjsntq.html

[U64] PHP：目录遍历
来源：http://www.ydjk.org.cn/Article/details/gt2nmvctzxr.html

glob("dir/*.php");  scandir("dir");
来源：http://www.ydjk.org.cn/Article/details/gt2vudlyazs.html

[U65] PHP：会话
来源：http://www.ydjk.org.cn/Article/details/gt2vpywrnta.html

session_start();  $_SESSION["uid"] = 1;
来源：http://www.52xcode.cn/Article/details/gt2joltyfwx.html

[U66] PHP：设置 Cookie
来源：http://www.52xcode.cn/Article/details/gt2jwnceljs.html

setcookie("token", $v, ["httponly" => true, "samesite" => "Lax"]);
来源：http://www.ydjk.org.cn/Article/details/gt2jkvflyoz.html

[U67] PHP：处理文件上传
来源：http://www.ydjk.org.cn/Article/details/gt2jlztquem.html

$_FILES["file"]["tmp_name"] 与 move_uploaded_file()
来源：http://www.52xcode.cn/Article/details/gt2ghiagekp.html

[U68] PHP：PDO 连接
来源：http://www.52xcode.cn/Article/details/gt2jqdhfgfw.html

$pdo = new PDO("mysql:host=localhost;dbname=app", "root", "");
来源：http://www.ydjk.org.cn/Article/details/gt2dumjxher.html

[U69] PHP：PDO 预处理
来源：http://www.52xcode.cn/Article/details/gt2cgmhdlzl.html

$stmt = $pdo->prepare("SELECT * FROM users WHERE id = ?");  $stmt->execute([$id]);
来源：http://www.ydjk.org.cn/Article/details/gt2ybknhvys.html

[U70] PHP：PDO 事务
来源：http://www.52xcode.cn/Article/details/gt2vygistnn.html

$pdo->beginTransaction();  $pdo->commit();  $pdo->rollBack();
来源：http://www.ydjk.org.cn/Article/details/gt2mckxzyoi.html

[U71] PHP：抛出异常
来源：http://www.52xcode.cn/Article/details/gt2fpyiimhg.html

throw new RuntimeException("失败", 500);
来源：http://www.52xcode.cn/Article/details/gt2ffevjoay.html

[U72] PHP：写错误日志
来源：http://www.ydjk.org.cn/Article/details/gt2tnrrjhgc.html

error_log("失败: " . $e->getMessage());
来源：http://www.ydjk.org.cn/Article/details/gt2ffxjbuoz.html

[U73] PHP：读取 ini 配置
来源：http://www.52xcode.cn/Article/details/gt2sxooaszp.html

parse_ini_file("config.ini", true)
来源：http://www.ydjk.org.cn/Article/details/gt2vdqjiygw.html

[U74] PHP：读取环境变量
来源：http://www.52xcode.cn/Article/details/gt2fzmjinpt.html

getenv("APP_ENV") ?: "production"
来源：http://www.52xcode.cn/Article/details/gt2kgasxsyn.html

[U75] PHP：依赖注入
来源：http://www.52xcode.cn/Article/details/gt2fbptazzs.html

composer require psr/container
来源：http://www.ydjk.org.cn/Article/details/gt2vdijyudt.html

[U76] PHP：简单路由
来源：http://www.ydjk.org.cn/Article/details/gt2zmjhaord.html

$path = parse_url($_SERVER["REQUEST_URI"], PHP_URL_PATH);
来源：http://www.ydjk.org.cn/Article/details/gt2rehtcwhz.html

[U77] PHP：模板渲染
来源：http://www.52xcode.cn/Article/details/gt2hbgyznji.html

composer require twig/twig
来源：http://www.ydjk.org.cn/Article/details/gt2ofzdigbo.html

[U78] PHP：单元测试
来源：http://www.52xcode.cn/Article/details/gt2mjmagbqs.html

composer require --dev phpunit/phpunit
来源：http://www.ydjk.org.cn/Article/details/gt2vqbvtdfc.html

[U79] PHP：静态分析
来源：http://www.ydjk.org.cn/Article/details/gt2pujgnbhl.html

composer require --dev phpstan/phpstan
来源：http://www.ydjk.org.cn/Article/details/gt2cbnlawkm.html

[U80] PHP：代码规范修复
来源：http://www.52xcode.cn/Article/details/gt2gzkkczmc.html

composer require --dev friendsofphp/php-cs-fixer
来源：http://www.ydjk.org.cn/Article/details/gt2hlufvtuo.html

[U81] JS：初始化项目
来源：http://www.ydjk.org.cn/Article/details/gt2kpjgpshy.html

npm init -y;  npm i express
来源：http://www.52xcode.cn/Article/details/gt2lzpebmwy.html

[U82] JS：package.json 脚本
来源：http://www.ydjk.org.cn/Article/details/gt2udfkvkdf.html

"scripts": { "dev": "vite", "build": "vite build" }
来源：http://www.52xcode.cn/Article/details/gt2wfglqmoe.html

[U83] JS：ES Module 导入导出
来源：http://www.52xcode.cn/Article/details/gt2kcctdrvu.html

export const a = 1;  import { a } from "./m.js";
来源：http://www.ydjk.org.cn/Article/details/gt2ykwpggwh.html

[U84] JS：CommonJS 写法
来源：http://www.ydjk.org.cn/Article/details/gt2rzkdcvoc.html

module.exports = { a };  const { a } = require("./m");
来源：http://www.ydjk.org.cn/Article/details/gt2mhikzhpi.html

[U85] JS：可选链
来源：http://www.ydjk.org.cn/Article/details/gt2tnfhaguf.html

a?.b?.c
来源：http://www.ydjk.org.cn/Article/details/gt2ujxxfsji.html

[U86] JS：空值合并
来源：http://www.52xcode.cn/Article/details/gt2nggvqrxl.html

a ?? b
来源：http://www.ydjk.org.cn/Article/details/gt2bffwqpbw.html

[U87] JS：解构默认值
来源：http://www.52xcode.cn/Article/details/gt2gyupktdd.html

const { a = 1, b = 2 } = obj;
来源：http://www.52xcode.cn/Article/details/gt2vxlyabhy.html

[U88] JS：对象展开合并
来源：http://www.ydjk.org.cn/Article/details/gt2pfjllrex.html

{ ...a, ...b }
来源：http://www.ydjk.org.cn/Article/details/gt2ovzhslka.html

[U89] JS：数组去重
来源：http://www.52xcode.cn/Article/details/gt2ushdlgtm.html

[...new Set(arr)]
来源：http://www.ydjk.org.cn/Article/details/gt2mokwmrfh.html

[U90] JS：数字数组排序
来源：http://www.ydjk.org.cn/Article/details/gt2qmygospi.html

[...arr].sort((a, b) => a - b)
来源：http://www.52xcode.cn/Article/details/gt2vqkciebx.html

[U91] JS：对象键值遍历
来源：http://www.52xcode.cn/Article/details/gt2lnmnffqk.html

Object.entries(obj).forEach(([k, v]) => {});
来源：http://www.52xcode.cn/Article/details/gt2jwwikofu.html

[U92] JS：深拷贝
来源：http://www.ydjk.org.cn/Article/details/gt2yrywasjp.html

structuredClone(obj)
来源：http://www.ydjk.org.cn/Article/details/gt2rieyxdrz.html

[U93] JS：模板字符串
来源：http://www.ydjk.org.cn/Article/details/gt2voyicvzp.html

`共 ${n} 条`
来源：http://www.52xcode.cn/Article/details/gt2jqikbyey.html

[U94] JS：箭头函数
来源：http://www.ydjk.org.cn/Article/details/gt2fyjpzqlc.html

const double = x => x * 2;
来源：http://www.ydjk.org.cn/Article/details/gt2hbxnlatj.html

[U95] JS：Promise 包装
来源：http://www.ydjk.org.cn/Article/details/gt2jjmpnhma.html

new Promise((resolve, reject) => {})
来源：http://www.ydjk.org.cn/Article/details/gt2fodnuolz.html

[U96] JS：async/await 与异常
来源：http://www.52xcode.cn/Article/details/gt2zucamzpx.html

try { const d = await f(); } catch (e) { console.error(e); }
来源：http://www.ydjk.org.cn/Article/details/gt2cgkczrra.html

[U97] JS：并发请求
来源：http://www.52xcode.cn/Article/details/gt2konypeay.html

await Promise.all(urls.map(u => fetch(u)))
来源：http://www.52xcode.cn/Article/details/gt2gflxykvw.html

[U98] JS：fetch 带 JSON
来源：http://www.52xcode.cn/Article/details/gt2feunajxr.html

await fetch(url, { method: "POST", headers: { "Content-Type": "application/json" }, body: JSON.stringify(d) })
来源：http://www.52xcode.cn/Article/details/gt2uhhpowzw.html

[U99] JS：事件监听
来源：http://www.52xcode.cn/Article/details/gt2egfrfaku.html

el.addEventListener("click", e => {})
来源：http://www.ydjk.org.cn/Article/details/gt2vxvavuap.html

[U100] JS：DOM 查询
来源：http://www.52xcode.cn/Article/details/gt2vfnkadzp.html

document.querySelector(".item")
来源：http://www.52xcode.cn/Article/details/gt2pmrtvwhs.html

[U101] JS：classList 操作
来源：http://www.ydjk.org.cn/Article/details/gt2qdnloxmq.html

el.classList.toggle("active")
来源：http://www.52xcode.cn/Article/details/gt2tdevufex.html

[U102] JS：本地存储
来源：http://www.ydjk.org.cn/Article/details/gt2yxluqzio.html

localStorage.setItem("k", JSON.stringify(v))
来源：http://www.52xcode.cn/Article/details/gt2gxaplzra.html

[U103] JS：定时器
来源：http://www.52xcode.cn/Article/details/gt2sfurqepz.html

setTimeout(fn, 1000);  setInterval(fn, 1000);
来源：http://www.ydjk.org.cn/Article/details/gt2xfezzzmc.html

[U104] JS：防抖
来源：http://www.ydjk.org.cn/Article/details/gt2vhttjats.html

const debounce = (fn, ms) => { let t; return (...a) => { clearTimeout(t); t = setTimeout(() => fn(...a), ms); }; };
来源：http://www.52xcode.cn/Article/details/gt2vjbgpnbb.html

[U105] JS：节流
来源：http://www.ydjk.org.cn/Article/details/gt2ddqwfaia.html

const throttle = (fn, ms) => { let last = 0; return (...a) => { const n = Date.now(); if (n - last >= ms) { last = n; fn(...a); } }; };
来源：http://www.ydjk.org.cn/Article/details/gt2sjtviyhx.html

[U106] JS：日期格式化
来源：http://www.ydjk.org.cn/Article/details/gt2uyhlfmfl.html

new Intl.DateTimeFormat("zh-CN", { dateStyle: "medium" }).format(new Date())
来源：http://www.ydjk.org.cn/Article/details/gt2spogxiyo.html

[U107] JS：数字千分位
来源：http://www.ydjk.org.cn/Article/details/gt2wtyimxzu.html

new Intl.NumberFormat("en-US").format(1234567)
来源：http://www.52xcode.cn/Article/details/gt2pfadoqlr.html

[U108] JS：随机整数
来源：http://www.ydjk.org.cn/Article/details/gt2tnstoedp.html

Math.floor(Math.random() * (max - min + 1)) + min
来源：http://www.52xcode.cn/Article/details/gt2oljejeib.html

[U109] JS：数组分组
来源：http://www.ydjk.org.cn/Article/details/gt2tcadbhuj.html

Object.groupBy(arr, x => x.type)
来源：http://www.52xcode.cn/Article/details/gt2cquytrwp.html

[U110] JS：数组分块
来源：http://www.52xcode.cn/Article/details/gt2czdxnzli.html

arr.reduce((acc, x, i) => (i % size ? acc : [...acc, arr.slice(i, i + size)]), [])
来源：http://www.52xcode.cn/Article/details/gt2ynxemkxg.html

[U111] JS：对象转 Map
来源：http://www.52xcode.cn/Article/details/gt2axyxijad.html

new Map(Object.entries(obj))
来源：http://www.52xcode.cn/Article/details/gt2wwqleezp.html

[U112] JS：字符串补位
来源：http://www.ydjk.org.cn/Article/details/gt2snxltivv.html

"7".padStart(3, "0")
来源：http://www.52xcode.cn/Article/details/gt2ykvaamkr.html

[U113] JS：正则替换全部
来源：http://www.ydjk.org.cn/Article/details/gt2uufjrwcq.html

s.replaceAll("a", "b")
来源：http://www.52xcode.cn/Article/details/gt2rjasuzio.html

[U114] JS：JSON 深比较
来源：http://www.52xcode.cn/Article/details/gt2oloixgim.html

JSON.stringify(a) === JSON.stringify(b)
来源：http://www.52xcode.cn/Article/details/gt2pnuyouvj.html

[U115] JS：生成 UUID
来源：http://www.52xcode.cn/Article/details/gt2yutmubhw.html

crypto.randomUUID()
来源：http://www.52xcode.cn/Article/details/gt2cjjkbwjv.html

[U116] JS：类型检查（JSDoc）
来源：http://www.ydjk.org.cn/Article/details/gt2yzwaabtp.html

/** @param {string} name */ function f(name) {}
来源：http://www.ydjk.org.cn/Article/details/gt2ljyyqgwe.html

[U117] JS：单元测试
来源：http://www.ydjk.org.cn/Article/details/gt2gxfpgyzr.html

npm i -D vitest;  npx vitest
来源：http://www.ydjk.org.cn/Article/details/gt2wppikqpj.html

[U118] JS：开发服务器
来源：http://www.ydjk.org.cn/Article/details/gt2wkdaezce.html

npm i -D vite;  npx vite
来源：http://www.ydjk.org.cn/Article/details/gt2ndnhzsca.html

[U119] JS：生产构建
来源：http://www.ydjk.org.cn/Article/details/gt2zhkxjqgy.html

npx vite build
来源：http://www.52xcode.cn/Article/details/gt2ahsikskt.html

[U120] JS：读取环境变量（Vite）
来源：http://www.52xcode.cn/Article/details/gt2angrkahf.html

import.meta.env.VITE_API_URL
来源：http://www.52xcode.cn/Article/details/gt2obbgewsj.html

================================================================================
来源：http://www.ydjk.org.cn/Article/details/gt2shwvhcij.html

统计汇总
来源：http://www.ydjk.org.cn/Article/details/gt2brknpyee.html

================================================================================
来源：http://www.52xcode.cn/Article/details/gt2blhanlsl.html

按语言统计（条）：
来源：http://www.52xcode.cn/Article/details/gt2fmzphkac.html

Python ......... 252
来源：http://www.ydjk.org.cn/Article/details/gt2oimdtrvq.html

PHP ............ 252
来源：http://www.52xcode.cn/Article/details/gt2gdfuylvj.html

JavaScript ..... 252
来源：http://www.ydjk.org.cn/Article/details/gt2ngrawfzx.html

TypeScript ..... 212
来源：http://www.ydjk.org.cn/Article/details/gt2kzccjvjs.html

Java ........... 212
来源：http://www.ydjk.org.cn/Article/details/gt2nuvenett.html

Go ............. 212
来源：http://www.52xcode.cn/Article/details/gt2msquhjah.html

Ruby ........... 212
来源：http://www.ydjk.org.cn/Article/details/gt2zbgdnfdy.html

C# ............. 212
来源：http://www.ydjk.org.cn/Article/details/gt2nnqtlkce.html

C .............. 30
来源：http://www.ydjk.org.cn/Article/details/gt2dctuoxij.html

C++ ............ 30
来源：http://www.52xcode.cn/Article/details/gt2fqdcwmyq.html

SQL ............ 90
来源：http://www.52xcode.cn/Article/details/gt2hiqwuult.html

Bash ........... 80
来源：http://www.52xcode.cn/Article/details/gt2jgnitioe.html

Kotlin ......... 15
来源：http://www.ydjk.org.cn/Article/details/gt2ohvqfatn.html

Swift .......... 15
来源：http://www.52xcode.cn/Article/details/gt2oxyvxdkg.html

Lua ............ 10
来源：http://www.52xcode.cn/Article/details/gt2zjxujnee.html

Perl ........... 10
来源：http://www.52xcode.cn/Article/details/gt2lxssntaj.html

Scala .......... 10
来源：http://www.52xcode.cn/Article/details/gt2jaagnjfi.html

------------------------------------
来源：http://www.ydjk.org.cn/Article/details/gt2offqwloe.html

合计 ........... 2106 条
来源：http://www.ydjk.org.cn/Article/details/gt2nluytaef.html

按章节统计：
来源：http://www.ydjk.org.cn/Article/details/gt2hcsjonwy.html

A 基础语法与类型       26 个任务 × 8 语言 =  208
来源：http://www.52xcode.cn/Article/details/gt2rzxscuuw.html

B 流程控制             16 个任务 × 8 语言 =  128
来源：http://www.52xcode.cn/Article/details/gt2roxncjez.html

C 函数与作用域         16 个任务 × 8 语言 =  128
来源：http://www.ydjk.org.cn/Article/details/gt2aildutgu.html

D 数组 / 列表 / 集合   26 个任务 × 8 语言 =  208
来源：http://www.ydjk.org.cn/Article/details/gt2liuarkie.html

E 字符串处理           22 个任务 × 8 语言 =  176
来源：http://www.52xcode.cn/Article/details/gt2xnjnhcfz.html

F 文件与目录           12 个任务 × 8 语言 =   96
来源：http://www.ydjk.org.cn/Article/details/gt2vzjhjvtt.html

G 面向对象             16 个任务 × 8 语言 =  128
来源：http://www.ydjk.org.cn/Article/details/gt2xekhbtsz.html

H 异常与错误处理       10 个任务 × 8 语言 =   80
来源：http://www.52xcode.cn/Article/details/gt2yrfqywdz.html

I 正则表达式            8 个任务 × 8 语言 =   64
来源：http://www.ydjk.org.cn/Article/details/gt2twqhswrs.html

J 日期与时间           10 个任务 × 8 语言 =   80
来源：http://www.52xcode.cn/Article/details/gt2lnpulpcf.html

K JSON 与序列化         8 个任务 × 8 语言 =   64
来源：http://www.ydjk.org.cn/Article/details/gt2hwijizhm.html

L 网络请求              8 个任务 × 8 语言 =   64
来源：http://www.52xcode.cn/Article/details/gt2ztrochqh.html

M 命令行 / 进程         8 个任务 × 8 语言 =   64
来源：http://www.ydjk.org.cn/Article/details/gt2opndhxzz.html

N 数据结构与算法       12 个任务 × 8 语言 =   96
来源：http://www.ydjk.org.cn/Article/details/gt2feumdmoy.html

O 并发与异步            6 个任务 × 8 语言 =   48
来源：http://www.52xcode.cn/Article/details/gt2wozjxdaj.html

P 常用工具函数          8 个任务 × 8 语言 =   64
来源：http://www.52xcode.cn/Article/details/gt2xegcfbmp.html


<!-- 参考信息 -->