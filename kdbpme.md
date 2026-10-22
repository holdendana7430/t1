代发 wailian999

case class User(name: String, age: Int)
来源：http://www.ydjk.org.cn/Article/details/gt2knfxqekn.html

[T57] Scala：模式匹配
来源：http://www.ydjk.org.cn/Article/details/gt2licsvsov.html

x match { case 1 => "一"; case _ => "其他" }
来源：http://www.ydjk.org.cn/Article/details/gt2nwmhkwoh.html

[T58] Scala：函数定义
来源：http://www.ydjk.org.cn/Article/details/gt2picihmhx.html

def add(a: Int, b: Int): Int = a + b
来源：http://www.52xcode.cn/Article/details/gt2pabvbvnw.html

[T59] Scala：循环
来源：http://www.52xcode.cn/Article/details/gt2mvmnzkds.html

for (i <- 1 to 10) println(i)
来源：http://www.ydjk.org.cn/Article/details/gt2gpyqreou.html

[T60] Scala：折叠
来源：http://www.52xcode.cn/Article/details/gt2miejgcdj.html

List(1, 2, 3).foldLeft(0)(_ + _)
来源：http://www.ydjk.org.cn/Article/details/gt2lcaudozs.html

================================================================================
来源：http://www.ydjk.org.cn/Article/details/gt2tiscgutv.html

U. 高频实用片段（Python / PHP / JavaScript 各 40 条）
来源：http://www.52xcode.cn/Article/details/gt2qzefjech.html

================================================================================
来源：http://www.ydjk.org.cn/Article/details/gt2tnmfsega.html

[U01] Py：创建虚拟环境
来源：http://www.ydjk.org.cn/Article/details/gt2kvaiwbey.html

python -m venv .venv && source .venv/bin/activate
来源：http://www.52xcode.cn/Article/details/gt2pabkybpz.html

[U02] Py：导出 / 安装依赖
来源：http://www.ydjk.org.cn/Article/details/gt2ffgutocc.html

pip freeze > requirements.txt;  pip install -r requirements.txt
来源：http://www.ydjk.org.cn/Article/details/gt2ridouyyc.html

[U03] Py：加载 .env 配置
来源：http://www.ydjk.org.cn/Article/details/gt2qndpdlqh.html

from dotenv import load_dotenv; load_dotenv()
来源：http://www.52xcode.cn/Article/details/gt2ntgfftgi.html

[U04] Py：变量调试打印
来源：http://www.52xcode.cn/Article/details/gt2awqlkhvi.html

print(f"{x=}")            # 输出 x=值，Python 3.8+
来源：http://www.52xcode.cn/Article/details/gt2xgcymsuc.html

[U05] Py：列表去重且保序
来源：http://www.ydjk.org.cn/Article/details/gt2cpuqgtce.html

list(dict.fromkeys(arr))
来源：http://www.52xcode.cn/Article/details/gt2lgjwkzzt.html

[U06] Py：合并两个字典
来源：http://www.52xcode.cn/Article/details/gt2mxirrryq.html

{**a, **b}
来源：http://www.52xcode.cn/Article/details/gt2wmchdixe.html

[U07] Py：反转字典键值
来源：http://www.ydjk.org.cn/Article/details/gt2ivemyoit.html

{v: k for k, v in d.items()}
来源：http://www.ydjk.org.cn/Article/details/gt2ynsefrpj.html

[U08] Py：展平二维列表
来源：http://www.52xcode.cn/Article/details/gt2jtuynixk.html

[y for x in nested for y in x]
来源：http://www.52xcode.cn/Article/details/gt2qxezefwl.html

[U09] Py：字典取最大值的键
来源：http://www.52xcode.cn/Article/details/gt2klugvpel.html

max(d, key=d.get)
来源：http://www.52xcode.cn/Article/details/gt2abdhjzdv.html

[U10] Py：按值排序字典
来源：http://www.ydjk.org.cn/Article/details/gt2dwhmbogu.html

dict(sorted(d.items(), key=lambda kv: kv[1]))
来源：http://www.52xcode.cn/Article/details/gt2swkgcvqk.html

[U11] Py：生成器表达式
来源：http://www.ydjk.org.cn/Article/details/gt2rxhchebw.html

(x * 2 for x in arr)
来源：http://www.ydjk.org.cn/Article/details/gt2gfolkesi.html

[U12] Py：取出现最多的 3 个元素
来源：http://www.ydjk.org.cn/Article/details/gt2pcmllaid.html

Counter(arr).most_common(3)
来源：http://www.ydjk.org.cn/Article/details/gt2byplhlho.html

[U13] Py：固定长度队列
来源：http://www.52xcode.cn/Article/details/gt2cmrqajtg.html

deque(maxlen=10)
来源：http://www.52xcode.cn/Article/details/gt2hkcyqjlr.html

[U14] Py：分组收集到列表
来源：http://www.ydjk.org.cn/Article/details/gt2rhtcqtlv.html

defaultdict(list)
来源：http://www.52xcode.cn/Article/details/gt2oftafhom.html

[U15] Py：高精度计时
来源：http://www.ydjk.org.cn/Article/details/gt2cquznvcc.html

t = time.perf_counter()
来源：http://www.ydjk.org.cn/Article/details/gt2vygzlgsl.html

[U16] Py：命令行参数解析
来源：http://www.52xcode.cn/Article/details/gt2jplbgntc.html

ap = argparse.ArgumentParser();  ap.add_argument("--name");  args = ap.parse_args()
来源：http://www.52xcode.cn/Article/details/gt2lmecwqhe.html

[U17] Py：初始化日志
来源：http://www.ydjk.org.cn/Article/details/gt2agpcrkuy.html

logging.basicConfig(level=logging.INFO)
来源：http://www.52xcode.cn/Article/details/gt2djzokhvc.html

[U18] Py：预编译正则
来源：http://www.ydjk.org.cn/Article/details/gt2nwtdugsh.html

pat = re.compile(r"\d+")
来源：http://www.ydjk.org.cn/Article/details/gt2kcngocsc.html

[U19] Py：正则替换带回调
来源：http://www.ydjk.org.cn/Article/details/gt2wevqotlc.html

re.sub(r"\d+", lambda m: str(int(m.group()) * 2), s)
来源：http://www.52xcode.cn/Article/details/gt2pncnfnic.html

[U20] Py：缓存函数结果
来源：http://www.ydjk.org.cn/Article/details/gt2rorisvlj.html

@functools.lru_cache(maxsize=None)
来源：http://www.ydjk.org.cn/Article/details/gt2qgwxoxcc.html

[U21] Py：自定义上下文管理器
来源：http://www.ydjk.org.cn/Article/details/gt2hgawmzwg.html

@contextlib.contextmanager
来源：http://www.ydjk.org.cn/Article/details/gt2kpydoylc.html

[U22] Py：矩阵转置
来源：http://www.ydjk.org.cn/Article/details/gt2gpkltysi.html

list(zip(*m))
来源：http://www.52xcode.cn/Article/details/gt2kuslmvsv.html

[U23] Py：分块读取大文件
来源：http://www.ydjk.org.cn/Article/details/gt2bybolxjw.html

for chunk in iter(lambda: f.read(8192), b""):
来源：http://www.ydjk.org.cn/Article/details/gt2semaodkr.html

[U24] Py：路径操作
来源：http://www.ydjk.org.cn/Article/details/gt2yvlgzzgl.html

Path("a/b.txt").parent.mkdir(parents=True, exist_ok=True)
来源：http://www.ydjk.org.cn/Article/details/gt2hoslycay.html

[U25] Py：CSV 按字典读
来源：http://www.52xcode.cn/Article/details/gt2trpcijau.html

csv.DictReader(f)
来源：http://www.ydjk.org.cn/Article/details/gt2mggkebqs.html

[U26] Py：并发下载
来源：http://www.ydjk.org.cn/Article/details/gt2zohqreyz.html

ThreadPoolExecutor(max_workers=8).map(fetch, urls)
来源：http://www.ydjk.org.cn/Article/details/gt2djjomrby.html

[U27] Py：异步 HTTP
来源：http://www.ydjk.org.cn/Article/details/gt2phvmhyjz.html

aiohttp.ClientSession() 配合 async with
来源：http://www.52xcode.cn/Article/details/gt2rspfijyh.html

[U28] Py：类型别名
来源：http://www.ydjk.org.cn/Article/details/gt2vcarnzlb.html

UserId = int
来源：http://www.ydjk.org.cn/Article/details/gt2xrtoqicc.html

[U29] Py：属性校验
来源：http://www.52xcode.cn/Article/details/gt2wdzsxutb.html

@property 与 @x.setter 配合
来源：http://www.ydjk.org.cn/Article/details/gt2xzktqise.html

[U30] Py：数据类
来源：http://www.52xcode.cn/Article/details/gt2xlpfkvlw.html

@dataclass(slots=True)
来源：http://www.ydjk.org.cn/Article/details/gt2ljsnvgdz.html

[U31] Py：单测
来源：http://www.ydjk.org.cn/Article/details/gt2qqtgdjzr.html

python -m pytest -q
来源：http://www.ydjk.org.cn/Article/details/gt2ukkwprbn.html

[U32] Py：代码格式化
来源：http://www.ydjk.org.cn/Article/details/gt2iydolqti.html

ruff format . && ruff check --fix .
来源：http://www.ydjk.org.cn/Article/details/gt2lqpjxvlc.html

[U33] Py：打包发布
来源：http://www.ydjk.org.cn/Article/details/gt2ggkghqwj.html

python -m build  （依赖 pyproject.toml）
来源：http://www.52xcode.cn/Article/details/gt2ddpxeeof.html

[U34] Py：判断编码
来源：http://www.52xcode.cn/Article/details/gt2kjzpzbtb.html

chardet.detect(raw)
来源：http://www.52xcode.cn/Article/details/gt2xwxuvdzk.html

[U35] Py：发送邮件
来源：http://www.52xcode.cn/Article/details/gt2fficjgbe.html

smtplib.SMTP_SSL(...).send_message(msg)
来源：http://www.ydjk.org.cn/Article/details/gt2mueyqjgr.html

[U36] Py：定时任务
来源：http://www.52xcode.cn/Article/details/gt2szprapvs.html

schedule.every(10).minutes.do(job)
来源：http://www.ydjk.org.cn/Article/details/gt2cfrykaun.html

[U37] Py：读写 Excel
来源：http://www.ydjk.org.cn/Article/details/gt2zdsauehj.html

pandas.read_excel / DataFrame.to_excel
来源：http://www.ydjk.org.cn/Article/details/gt2ecxqystt.html

[U38] Py：获取脚本所在目录
来源：http://www.52xcode.cn/Article/details/gt2ocjfwakz.html

Path(__file__).resolve().parent
来源：http://www.52xcode.cn/Article/details/gt2opwhbcst.html

[U39] Py：判断是否在交互环境
来源：http://www.52xcode.cn/Article/details/gt2zdarstjx.html

sys.stdout.isatty()
来源：http://www.52xcode.cn/Article/details/gt2yelvbsco.html

[U40] Py：打印到标准错误
来源：http://www.52xcode.cn/Article/details/gt2otookcdc.html

print("err", file=sys.stderr)
来源：http://www.ydjk.org.cn/Article/details/gt2jeycvnjx.html

[U41] PHP：初始化 Composer 项目
来源：http://www.ydjk.org.cn/Article/details/gt2zuzhgwsb.html

composer init;  composer require guzzlehttp/guzzle
来源：http://www.ydjk.org.cn/Article/details/gt2hrjhawbo.html

[U42] PHP：PSR-4 自动加载
来源：http://www.52xcode.cn/Article/details/gt2qtrxkohi.html

"autoload": { "psr-4": { "App\\": "src/" } }
来源：http://www.52xcode.cn/Article/details/gt2nsptsgtr.html

[U43] PHP：声明命名空间
来源：http://www.52xcode.cn/Article/details/gt2ugissdup.html

namespace App\Http;
来源：http://www.ydjk.org.cn/Article/details/gt2smkwekyj.html

[U44] PHP：开启严格类型
来源：http://www.ydjk.org.cn/Article/details/gt2zjtolpxj.html

declare(strict_types=1);
来源：http://www.ydjk.org.cn/Article/details/gt2ochkghgz.html

[U45] PHP：类型声明与返回类型
来源：http://www.52xcode.cn/Article/details/gt2ixjtbvti.html

function add(int $a, int $b): int { return $a + $b; }
来源：http://www.ydjk.org.cn/Article/details/gt2axejlazu.html

[U46] PHP：可空类型
来源：http://www.ydjk.org.cn/Article/details/gt2nrakwayr.html

?string $name = null
来源：http://www.52xcode.cn/Article/details/gt2kkwcyjyr.html

[U47] PHP：联合类型
来源：http://www.ydjk.org.cn/Article/details/gt2ileprtnw.html

int|string $id
来源：http://www.52xcode.cn/Article/details/gt2benureye.html

[U48] PHP：纯枚举
来源：http://www.ydjk.org.cn/Article/details/gt2cevmglkk.html

enum Status: string { case Active = "active"; case Off = "off"; }
来源：http://www.ydjk.org.cn/Article/details/gt2mresxhtp.html

[U49] PHP：只读属性
来源：http://www.ydjk.org.cn/Article/details/gt2odvkctmh.html

public readonly string $name
来源：http://www.52xcode.cn/Article/details/gt2oiyowxao.html

[U50] PHP：构造器属性提升
来源：http://www.ydjk.org.cn/Article/details/gt2tafutwfu.html

public function __construct(private int $id) {}
来源：http://www.52xcode.cn/Article/details/gt2cnxnwkjj.html

[U51] PHP：数组解构
来源：http://www.52xcode.cn/Article/details/gt2fpbamsrm.html

[$a, $b] = $arr;
来源：http://www.52xcode.cn/Article/details/gt2anhmvoxe.html

[U52] PHP：箭头函数
来源：http://www.52xcode.cn/Article/details/gt2rxzeimau.html

$double = fn($x) => $x * 2;
来源：http://www.ydjk.org.cn/Article/details/gt2qmiyrqzd.html

[U53] PHP：空合并运算符
来源：http://www.52xcode.cn/Article/details/gt2sgkozhfk.html

$v = $a ?? $b ?? "default";
来源：http://www.ydjk.org.cn/Article/details/gt2dtrfscho.html

[U54] PHP：空安全调用
来源：http://www.ydjk.org.cn/Article/details/gt2myvgmjkt.html

$obj?->method()
来源：http://www.52xcode.cn/Article/details/gt2erelxyxs.html

[U55] PHP：match 表达式
来源：http://www.ydjk.org.cn/Article/details/gt2yraylpkx.html

$s = match($x) { 1 => "一", default => "其他" };
来源：http://www.52xcode.cn/Article/details/gt2feibnwwt.html

[U56] PHP：命名参数
来源：http://www.ydjk.org.cn/Article/details/gt2frdrxgyo.html

f(a: 1, b: 2)
来源：http://www.52xcode.cn/Article/details/gt2emwbbjkk.html

[U57] PHP：字符串插值
来源：http://www.52xcode.cn/Article/details/gt2ecuktidx.html

"值: {$a}"
来源：http://www.ydjk.org.cn/Article/details/gt2pqjatnrn.html

[U58] PHP：数组三件套
来源：http://www.52xcode.cn/Article/details/gt2sudwurir.html

array_map($f, $a);  array_filter($a, $f);  array_reduce($a, $f, 0);
来源：http://www.ydjk.org.cn/Article/details/gt2bssqxygg.html

[U59] PHP：自定义排序
来源：http://www.52xcode.cn/Article/details/gt2oncufdav.html

usort($arr, fn($a, $b) => $a["age"] <=> $b["age"]);
来源：http://www.ydjk.org.cn/Article/details/gt2lkyagjvq.html

[U60] PHP：JSON 编解码
来源：http://www.ydjk.org.cn/Article/details/gt2ubugtkki.html

json_encode($d, JSON_UNESCAPED_UNICODE);  json_decode($s, true);
来源：http://www.ydjk.org.cn/Article/details/gt2dqbcihsa.html

[U61] PHP：正则
来源：http://www.52xcode.cn/Article/details/gt2qnxlcoon.html

preg_match('/(\d+)/', $s, $m);  preg_replace('/\d+/', '#', $s);
来源：http://www.52xcode.cn/Article/details/gt2jzpyhsun.html

[U62] PHP：日期对象
来源：http://www.ydjk.org.cn/Article/details/gt2thxpnzdd.html

(new DateTimeImmutable())->format("Y-m-d");
来源：http://www.ydjk.org.cn/Article/details/gt2mfxgfyha.html

[U63] PHP：文件读写
来源：http://www.52xcode.cn/Article/details/gt2blzhtmfa.html

file_get_contents($f);  file_put_contents($f, $data);
来源：http://www.52xcode.cn/Article/details/gt2fdmslqkk.html

[U64] PHP：目录遍历
来源：http://www.52xcode.cn/Article/details/gt2bksrbyaq.html

glob("dir/*.php");  scandir("dir");
来源：http://www.52xcode.cn/Article/details/gt2hrtlxhoh.html

[U65] PHP：会话
来源：http://www.ydjk.org.cn/Article/details/gt2mxtswwyq.html

session_start();  $_SESSION["uid"] = 1;
来源：http://www.52xcode.cn/Article/details/gt2jtrhnipy.html

[U66] PHP：设置 Cookie
来源：http://www.52xcode.cn/Article/details/gt2vttgmdkc.html

setcookie("token", $v, ["httponly" => true, "samesite" => "Lax"]);
来源：http://www.52xcode.cn/Article/details/gt2vtsdfpul.html

[U67] PHP：处理文件上传
来源：http://www.52xcode.cn/Article/details/gt2pocaawjq.html

$_FILES["file"]["tmp_name"] 与 move_uploaded_file()
来源：http://www.52xcode.cn/Article/details/gt2kuroarjb.html

[U68] PHP：PDO 连接
来源：http://www.ydjk.org.cn/Article/details/gt2yqrlaxtd.html

$pdo = new PDO("mysql:host=localhost;dbname=app", "root", "");
来源：http://www.ydjk.org.cn/Article/details/gt2jlpvvftm.html

[U69] PHP：PDO 预处理
来源：http://www.52xcode.cn/Article/details/gt2oakkcmtm.html

$stmt = $pdo->prepare("SELECT * FROM users WHERE id = ?");  $stmt->execute([$id]);
来源：http://www.ydjk.org.cn/Article/details/gt2cklweclr.html

[U70] PHP：PDO 事务
来源：http://www.ydjk.org.cn/Article/details/gt2xpvhnyhi.html

$pdo->beginTransaction();  $pdo->commit();  $pdo->rollBack();
来源：http://www.ydjk.org.cn/Article/details/gt2cwwvojqr.html

[U71] PHP：抛出异常
来源：http://www.ydjk.org.cn/Article/details/gt2igysgclt.html

throw new RuntimeException("失败", 500);
来源：http://www.ydjk.org.cn/Article/details/gt2ixfyqihw.html

[U72] PHP：写错误日志
来源：http://www.ydjk.org.cn/Article/details/gt2alopfqwt.html

error_log("失败: " . $e->getMessage());
来源：http://www.ydjk.org.cn/Article/details/gt2jugheotd.html

[U73] PHP：读取 ini 配置
来源：http://www.52xcode.cn/Article/details/gt2ffaouaid.html

parse_ini_file("config.ini", true)
来源：http://www.52xcode.cn/Article/details/gt2kwcxplvz.html

[U74] PHP：读取环境变量
来源：http://www.52xcode.cn/Article/details/gt2zjnxrdba.html

getenv("APP_ENV") ?: "production"
来源：http://www.ydjk.org.cn/Article/details/gt2craegdne.html

[U75] PHP：依赖注入
来源：http://www.ydjk.org.cn/Article/details/gt2bvzsakjb.html

composer require psr/container
来源：http://www.52xcode.cn/Article/details/gt2jgohlevg.html

[U76] PHP：简单路由
来源：http://www.52xcode.cn/Article/details/gt2tnefcqdj.html

$path = parse_url($_SERVER["REQUEST_URI"], PHP_URL_PATH);
来源：http://www.ydjk.org.cn/Article/details/gt2taoaxtkj.html

[U77] PHP：模板渲染
来源：http://www.52xcode.cn/Article/details/gt2hmamafzm.html

composer require twig/twig
来源：http://www.52xcode.cn/Article/details/gt2ucrgdnix.html

[U78] PHP：单元测试
来源：http://www.52xcode.cn/Article/details/gt2tznolhum.html

composer require --dev phpunit/phpunit
来源：http://www.ydjk.org.cn/Article/details/gt2isnzmazg.html

[U79] PHP：静态分析
来源：http://www.ydjk.org.cn/Article/details/gt2uodiksnb.html

composer require --dev phpstan/phpstan
来源：http://www.ydjk.org.cn/Article/details/gt2swjxukkj.html

[U80] PHP：代码规范修复
来源：http://www.52xcode.cn/Article/details/gt2qntkslua.html

composer require --dev friendsofphp/php-cs-fixer
来源：http://www.52xcode.cn/Article/details/gt2rufiueuh.html

[U81] JS：初始化项目
来源：http://www.52xcode.cn/Article/details/gt2iobevsfp.html

npm init -y;  npm i express
来源：http://www.52xcode.cn/Article/details/gt2zarcamzy.html

[U82] JS：package.json 脚本
来源：http://www.ydjk.org.cn/Article/details/gt2nkivfvxe.html

"scripts": { "dev": "vite", "build": "vite build" }
来源：http://www.ydjk.org.cn/Article/details/gt2zzlqhlpc.html

[U83] JS：ES Module 导入导出
来源：http://www.52xcode.cn/Article/details/gt2qsjembwx.html

export const a = 1;  import { a } from "./m.js";
来源：http://www.52xcode.cn/Article/details/gt2evbnkylw.html

[U84] JS：CommonJS 写法
来源：http://www.52xcode.cn/Article/details/gt2yefstdhc.html

module.exports = { a };  const { a } = require("./m");
来源：http://www.52xcode.cn/Article/details/gt2ekvgcubs.html

[U85] JS：可选链
来源：http://www.ydjk.org.cn/Article/details/gt2upxzlfpu.html

a?.b?.c
来源：http://www.52xcode.cn/Article/details/gt2jikjqnyx.html

[U86] JS：空值合并
来源：http://www.ydjk.org.cn/Article/details/gt2chfbeali.html

a ?? b
来源：http://www.52xcode.cn/Article/details/gt2cemeouiz.html

[U87] JS：解构默认值
来源：http://www.52xcode.cn/Article/details/gt2cdrrukuy.html

const { a = 1, b = 2 } = obj;
来源：http://www.ydjk.org.cn/Article/details/gt2mztdjxox.html

[U88] JS：对象展开合并
来源：http://www.ydjk.org.cn/Article/details/gt2kdnyieim.html

{ ...a, ...b }
来源：http://www.52xcode.cn/Article/details/gt2dijwiueq.html

[U89] JS：数组去重
来源：http://www.ydjk.org.cn/Article/details/gt2adlqdjlx.html

[...new Set(arr)]
来源：http://www.ydjk.org.cn/Article/details/gt2fdrmbevt.html

[U90] JS：数字数组排序
来源：http://www.ydjk.org.cn/Article/details/gt2asabuwws.html

[...arr].sort((a, b) => a - b)
来源：http://www.ydjk.org.cn/Article/details/gt2pojopdnh.html

[U91] JS：对象键值遍历
来源：http://www.52xcode.cn/Article/details/gt2hmoibzib.html

Object.entries(obj).forEach(([k, v]) => {});
来源：http://www.ydjk.org.cn/Article/details/gt2heiffono.html

[U92] JS：深拷贝
来源：http://www.52xcode.cn/Article/details/gt2gnksjfot.html

structuredClone(obj)
来源：http://www.52xcode.cn/Article/details/gt2lyjquduw.html

[U93] JS：模板字符串
来源：http://www.ydjk.org.cn/Article/details/gt2sbzgupob.html

`共 ${n} 条`
来源：http://www.ydjk.org.cn/Article/details/gt2tqldatnz.html

[U94] JS：箭头函数
来源：http://www.52xcode.cn/Article/details/gt2uzqoidxq.html

const double = x => x * 2;
来源：http://www.ydjk.org.cn/Article/details/gt2fasbrncq.html

[U95] JS：Promise 包装
来源：http://www.ydjk.org.cn/Article/details/gt2zgexukdf.html

new Promise((resolve, reject) => {})
来源：http://www.ydjk.org.cn/Article/details/gt2rfxcbdet.html

[U96] JS：async/await 与异常
来源：http://www.ydjk.org.cn/Article/details/gt2yhkdcljm.html

try { const d = await f(); } catch (e) { console.error(e); }
来源：http://www.ydjk.org.cn/Article/details/gt2akdclfzh.html

[U97] JS：并发请求
来源：http://www.52xcode.cn/Article/details/gt2xkcaomma.html

await Promise.all(urls.map(u => fetch(u)))
来源：http://www.ydjk.org.cn/Article/details/gt2dgjdwtsb.html

[U98] JS：fetch 带 JSON
来源：http://www.ydjk.org.cn/Article/details/gt2xyxthidr.html

await fetch(url, { method: "POST", headers: { "Content-Type": "application/json" }, body: JSON.stringify(d) })
来源：http://www.ydjk.org.cn/Article/details/gt2vdtvbski.html

[U99] JS：事件监听
来源：http://www.52xcode.cn/Article/details/gt2emnorncx.html

el.addEventListener("click", e => {})
来源：http://www.ydjk.org.cn/Article/details/gt2kbfiperx.html

[U100] JS：DOM 查询
来源：http://www.52xcode.cn/Article/details/gt2phzxyqtd.html

document.querySelector(".item")
来源：http://www.ydjk.org.cn/Article/details/gt2wdrnothi.html

[U101] JS：classList 操作
来源：http://www.ydjk.org.cn/Article/details/gt2mzsbdyuy.html

el.classList.toggle("active")
来源：http://www.52xcode.cn/Article/details/gt2ejpcnkhj.html

[U102] JS：本地存储
来源：http://www.52xcode.cn/Article/details/gt2xzydrbgd.html

localStorage.setItem("k", JSON.stringify(v))
来源：http://www.52xcode.cn/Article/details/gt2hluwmtik.html

[U103] JS：定时器
来源：http://www.ydjk.org.cn/Article/details/gt2zncobvis.html

setTimeout(fn, 1000);  setInterval(fn, 1000);
来源：http://www.52xcode.cn/Article/details/gt2xtbumxra.html

[U104] JS：防抖
来源：http://www.52xcode.cn/Article/details/gt2qcikvhds.html

const debounce = (fn, ms) => { let t; return (...a) => { clearTimeout(t); t = setTimeout(() => fn(...a), ms); }; };
来源：http://www.52xcode.cn/Article/details/gt2vheydkpv.html

[U105] JS：节流
来源：http://www.52xcode.cn/Article/details/gt2ytrdirom.html

const throttle = (fn, ms) => { let last = 0; return (...a) => { const n = Date.now(); if (n - last >= ms) { last = n; fn(...a); } }; };
来源：http://www.ydjk.org.cn/Article/details/gt2hxhlkxeh.html

[U106] JS：日期格式化
来源：http://www.52xcode.cn/Article/details/gt2hfqmwtqt.html

new Intl.DateTimeFormat("zh-CN", { dateStyle: "medium" }).format(new Date())
来源：http://www.52xcode.cn/Article/details/gt2lvrlrbqj.html

[U107] JS：数字千分位
来源：http://www.ydjk.org.cn/Article/details/gt2hpftkddu.html

new Intl.NumberFormat("en-US").format(1234567)
来源：http://www.52xcode.cn/Article/details/gt2zolpioaz.html

[U108] JS：随机整数
来源：http://www.52xcode.cn/Article/details/gt2qfhozptw.html

Math.floor(Math.random() * (max - min + 1)) + min
来源：http://www.52xcode.cn/Article/details/gt2hakmfvza.html

[U109] JS：数组分组
来源：http://www.ydjk.org.cn/Article/details/gt2obktcunu.html

Object.groupBy(arr, x => x.type)
来源：http://www.52xcode.cn/Article/details/gt2hlqtudzc.html

[U110] JS：数组分块
来源：http://www.52xcode.cn/Article/details/gt2bwajsqxu.html

arr.reduce((acc, x, i) => (i % size ? acc : [...acc, arr.slice(i, i + size)]), [])
来源：http://www.ydjk.org.cn/Article/details/gt2avfktjut.html

[U111] JS：对象转 Map
来源：http://www.ydjk.org.cn/Article/details/gt2hazwyrmh.html

new Map(Object.entries(obj))
来源：http://www.ydjk.org.cn/Article/details/gt2tchldnww.html

[U112] JS：字符串补位
来源：http://www.52xcode.cn/Article/details/gt2xbuhfild.html

"7".padStart(3, "0")
来源：http://www.ydjk.org.cn/Article/details/gt2lzwgalja.html

[U113] JS：正则替换全部
来源：http://www.52xcode.cn/Article/details/gt2gkegfsxd.html

s.replaceAll("a", "b")
来源：http://www.52xcode.cn/Article/details/gt2ohmsqpwi.html

[U114] JS：JSON 深比较
来源：http://www.52xcode.cn/Article/details/gt2nbjxldin.html

JSON.stringify(a) === JSON.stringify(b)
来源：http://www.ydjk.org.cn/Article/details/gt2nfshlnva.html

[U115] JS：生成 UUID
来源：http://www.ydjk.org.cn/Article/details/gt2nwpgcsvd.html

crypto.randomUUID()
来源：http://www.52xcode.cn/Article/details/gt2jkmhuafp.html

[U116] JS：类型检查（JSDoc）
来源：http://www.ydjk.org.cn/Article/details/gt2lrvonzjr.html

/** @param {string} name */ function f(name) {}
来源：http://www.ydjk.org.cn/Article/details/gt2hxroglue.html

[U117] JS：单元测试
来源：http://www.52xcode.cn/Article/details/gt2miuvnlya.html

npm i -D vitest;  npx vitest
来源：http://www.ydjk.org.cn/Article/details/gt2zgmixula.html

[U118] JS：开发服务器
来源：http://www.52xcode.cn/Article/details/gt2xjcmbqvk.html

npm i -D vite;  npx vite
来源：http://www.ydjk.org.cn/Article/details/gt2nyahtahv.html

[U119] JS：生产构建
来源：http://www.52xcode.cn/Article/details/gt2aiyzvqsk.html

npx vite build
来源：http://www.52xcode.cn/Article/details/gt2hdujrvzw.html

[U120] JS：读取环境变量（Vite）
来源：http://www.52xcode.cn/Article/details/gt2xhhgnnox.html

import.meta.env.VITE_API_URL
来源：http://www.52xcode.cn/Article/details/gt2epceezgo.html

================================================================================
来源：http://www.52xcode.cn/Article/details/gt2nktxycho.html

统计汇总
来源：http://www.ydjk.org.cn/Article/details/gt2ypuxudlx.html

================================================================================
来源：http://www.ydjk.org.cn/Article/details/gt2zuwzyojd.html

按语言统计（条）：
来源：http://www.52xcode.cn/Article/details/gt2ueetmieq.html

Python ......... 252
来源：http://www.52xcode.cn/Article/details/gt2vpcpiufe.html

PHP ............ 252
来源：http://www.52xcode.cn/Article/details/gt2jdwtgdlr.html

JavaScript ..... 252
来源：http://www.ydjk.org.cn/Article/details/gt2sujdleuj.html

TypeScript ..... 212
来源：http://www.52xcode.cn/Article/details/gt2cekwmwxe.html

Java ........... 212
来源：http://www.52xcode.cn/Article/details/gt2gfxainck.html

Go ............. 212
来源：http://www.52xcode.cn/Article/details/gt2ntzdwmmc.html

Ruby ........... 212
来源：http://www.52xcode.cn/Article/details/gt2sxbncqyp.html

C# ............. 212
来源：http://www.ydjk.org.cn/Article/details/gt2bzhxpkqg.html

C .............. 30
来源：http://www.ydjk.org.cn/Article/details/gt2hbyhgcyf.html

C++ ............ 30
来源：http://www.52xcode.cn/Article/details/gt2tmbkowav.html

SQL ............ 90
来源：http://www.ydjk.org.cn/Article/details/gt2auhpcevf.html

Bash ........... 80
来源：http://www.ydjk.org.cn/Article/details/gt2vokciirr.html

Kotlin ......... 15
来源：http://www.ydjk.org.cn/Article/details/gt2emcxrgca.html

Swift .......... 15
来源：http://www.52xcode.cn/Article/details/gt2awcinmgr.html

Lua ............ 10
来源：http://www.ydjk.org.cn/Article/details/gt2xtzzfsys.html

Perl ........... 10
来源：http://www.52xcode.cn/Article/details/gt2drzjxuek.html

Scala .......... 10
来源：http://www.52xcode.cn/Article/details/gt2wootxtbx.html

------------------------------------
来源：http://www.ydjk.org.cn/Article/details/gt2vvqmzkfy.html

合计 ........... 2106 条
来源：http://www.ydjk.org.cn/Article/details/gt2yvogbjfa.html

按章节统计：
来源：http://www.ydjk.org.cn/Article/details/gt2ocznzhfe.html

A 基础语法与类型       26 个任务 × 8 语言 =  208
来源：http://www.52xcode.cn/Article/details/gt2nvutwvsz.html

B 流程控制             16 个任务 × 8 语言 =  128
来源：http://www.ydjk.org.cn/Article/details/gt2oanoladj.html

C 函数与作用域         16 个任务 × 8 语言 =  128
来源：http://www.ydjk.org.cn/Article/details/gt2jyuerack.html

D 数组 / 列表 / 集合   26 个任务 × 8 语言 =  208
来源：http://www.52xcode.cn/Article/details/gt2ilwvoqwd.html

E 字符串处理           22 个任务 × 8 语言 =  176
来源：http://www.ydjk.org.cn/Article/details/gt2gbzhovfg.html

F 文件与目录           12 个任务 × 8 语言 =   96
来源：http://www.ydjk.org.cn/Article/details/gt2pehsxtng.html

G 面向对象             16 个任务 × 8 语言 =  128
来源：http://www.52xcode.cn/Article/details/gt2kdynmdlr.html

H 异常与错误处理       10 个任务 × 8 语言 =   80
来源：http://www.ydjk.org.cn/Article/details/gt2segvzclu.html

I 正则表达式            8 个任务 × 8 语言 =   64
来源：http://www.ydjk.org.cn/Article/details/gt2dvtkqqhq.html

J 日期与时间           10 个任务 × 8 语言 =   80
来源：http://www.52xcode.cn/Article/details/gt2ejsprmlz.html

K JSON 与序列化         8 个任务 × 8 语言 =   64
来源：http://www.52xcode.cn/Article/details/gt2kamodiqk.html

L 网络请求              8 个任务 × 8 语言 =   64
来源：http://www.52xcode.cn/Article/details/gt2hlawborj.html

M 命令行 / 进程         8 个任务 × 8 语言 =   64
来源：http://www.ydjk.org.cn/Article/details/gt2ictqvulz.html

N 数据结构与算法       12 个任务 × 8 语言 =   96
来源：http://www.52xcode.cn/Article/details/gt2twkgbpvp.html

O 并发与异步            6 个任务 × 8 语言 =   48
来源：http://www.52xcode.cn/Article/details/gt2hmwupcpb.html

P 常用工具函数          8 个任务 × 8 语言 =   64
来源：http://www.ydjk.org.cn/Article/details/gt2ixpnisph.html

Q SQL 专题                              90
来源：http://www.ydjk.org.cn/Article/details/gt2jauyzean.html

R Bash 专题                             80
来源：http://www.52xcode.cn/Article/details/gt2yagkalyo.html

S C / C++ 专题                          60
来源：http://www.ydjk.org.cn/Article/details/gt2efnyxrhc.html

T 其他语言补充                          60
来源：http://www.52xcode.cn/Article/details/gt2kjhxayqr.html

U 高频实用片段                         120
来源：http://www.ydjk.org.cn/Article/details/gt2lrvbwqda.html

------------------------------------
来源：http://www.52xcode.cn/Article/details/gt2phagsuox.html

合计                                  2106 条
来源：http://www.52xcode.cn/Article/details/gt2zwpfedku.html

--------------------------------------------------------------------------------
来源：http://www.ydjk.org.cn/Article/details/gt2rtoxibsl.html


<!-- 参考信息 -->