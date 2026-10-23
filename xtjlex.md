代发 wailian999

case class User(name: String, age: Int)
来源：http://www.ydjk.org.cn/Article/details/gt3vmsbzjtn.html

[T57] Scala：模式匹配
来源：http://www.ydjk.org.cn/Article/details/gt3tebvfyus.html

x match { case 1 => "一"; case _ => "其他" }
来源：http://www.ydjk.org.cn/Article/details/gt3ssbxcdts.html

[T58] Scala：函数定义
来源：http://www.ydjk.org.cn/Article/details/gt3koxdpdly.html

def add(a: Int, b: Int): Int = a + b
来源：http://www.52xcode.cn/Article/details/gt3fwaknwoc.html

[T59] Scala：循环
来源：http://www.52xcode.cn/Article/details/gt3pnozfioo.html

for (i <- 1 to 10) println(i)
来源：http://www.ydjk.org.cn/Article/details/gt3hkhdgyjv.html

[T60] Scala：折叠
来源：http://www.52xcode.cn/Article/details/gt3dfelpzzg.html

List(1, 2, 3).foldLeft(0)(_ + _)
来源：http://www.52xcode.cn/Article/details/gt3qyluwjzi.html

================================================================================
来源：http://www.52xcode.cn/Article/details/gt3shcndmoi.html

U. 高频实用片段（Python / PHP / JavaScript 各 40 条）
来源：http://www.52xcode.cn/Article/details/gt3ppxozqna.html

================================================================================
来源：http://www.52xcode.cn/Article/details/gt3yidwgyly.html

[U01] Py：创建虚拟环境
来源：http://www.52xcode.cn/Article/details/gt3syeoxzff.html

python -m venv .venv && source .venv/bin/activate
来源：http://www.52xcode.cn/Article/details/gt3rrrlorzd.html

[U02] Py：导出 / 安装依赖
来源：http://www.ydjk.org.cn/Article/details/gt3wpzonyzp.html

pip freeze > requirements.txt;  pip install -r requirements.txt
来源：http://www.ydjk.org.cn/Article/details/gt3pfwgfmho.html

[U03] Py：加载 .env 配置
来源：http://www.52xcode.cn/Article/details/gt3kfqpjnjo.html

from dotenv import load_dotenv; load_dotenv()
来源：http://www.ydjk.org.cn/Article/details/gt3ybtcpkzq.html

[U04] Py：变量调试打印
来源：http://www.ydjk.org.cn/Article/details/gt3llmdezlt.html

print(f"{x=}")            # 输出 x=值，Python 3.8+
来源：http://www.ydjk.org.cn/Article/details/gt3qyyshkkz.html

[U05] Py：列表去重且保序
来源：http://www.ydjk.org.cn/Article/details/gt3wbqcxnvd.html

list(dict.fromkeys(arr))
来源：http://www.ydjk.org.cn/Article/details/gt3ekyfbyec.html

[U06] Py：合并两个字典
来源：http://www.ydjk.org.cn/Article/details/gt3iefavkin.html

{**a, **b}
来源：http://www.ydjk.org.cn/Article/details/gt3lbaqeyda.html

[U07] Py：反转字典键值
来源：http://www.ydjk.org.cn/Article/details/gt3slofkjhi.html

{v: k for k, v in d.items()}
来源：http://www.ydjk.org.cn/Article/details/gt3ycdioxkx.html

[U08] Py：展平二维列表
来源：http://www.ydjk.org.cn/Article/details/gt3uxdpfwuv.html

[y for x in nested for y in x]
来源：http://www.52xcode.cn/Article/details/gt3yxkfoxwl.html

[U09] Py：字典取最大值的键
来源：http://www.52xcode.cn/Article/details/gt3gexsrwcn.html

max(d, key=d.get)
来源：http://www.ydjk.org.cn/Article/details/gt3fryxlaie.html

[U10] Py：按值排序字典
来源：http://www.ydjk.org.cn/Article/details/gt3ntfslpor.html

dict(sorted(d.items(), key=lambda kv: kv[1]))
来源：http://www.ydjk.org.cn/Article/details/gt3gkbfgndk.html

[U11] Py：生成器表达式
来源：http://www.ydjk.org.cn/Article/details/gt3ydtbzzhz.html

(x * 2 for x in arr)
来源：http://www.ydjk.org.cn/Article/details/gt3qksrtcbl.html

[U12] Py：取出现最多的 3 个元素
来源：http://www.52xcode.cn/Article/details/gt3esdvrhqr.html

Counter(arr).most_common(3)
来源：http://www.ydjk.org.cn/Article/details/gt3ictgkyvt.html

[U13] Py：固定长度队列
来源：http://www.ydjk.org.cn/Article/details/gt3pjzemnpl.html

deque(maxlen=10)
来源：http://www.ydjk.org.cn/Article/details/gt3uwtmqiof.html

[U14] Py：分组收集到列表
来源：http://www.ydjk.org.cn/Article/details/gt3auafricu.html

defaultdict(list)
来源：http://www.ydjk.org.cn/Article/details/gt3eqtzjziu.html

[U15] Py：高精度计时
来源：http://www.ydjk.org.cn/Article/details/gt3eoczkgsg.html

t = time.perf_counter()
来源：http://www.ydjk.org.cn/Article/details/gt3wawvnmtt.html

[U16] Py：命令行参数解析
来源：http://www.ydjk.org.cn/Article/details/gt3eauugfxl.html

ap = argparse.ArgumentParser();  ap.add_argument("--name");  args = ap.parse_args()
来源：http://www.52xcode.cn/Article/details/gt3lkptcfms.html

[U17] Py：初始化日志
来源：http://www.52xcode.cn/Article/details/gt3fruyzvhr.html

logging.basicConfig(level=logging.INFO)
来源：http://www.52xcode.cn/Article/details/gt3imdgijbx.html

[U18] Py：预编译正则
来源：http://www.52xcode.cn/Article/details/gt3osdbhhxk.html

pat = re.compile(r"\d+")
来源：http://www.ydjk.org.cn/Article/details/gt3nhwpsfxt.html

[U19] Py：正则替换带回调
来源：http://www.52xcode.cn/Article/details/gt3rzxsfiqh.html

re.sub(r"\d+", lambda m: str(int(m.group()) * 2), s)
来源：http://www.52xcode.cn/Article/details/gt3pyxijbzy.html

[U20] Py：缓存函数结果
来源：http://www.ydjk.org.cn/Article/details/gt3zpgqiipm.html

@functools.lru_cache(maxsize=None)
来源：http://www.ydjk.org.cn/Article/details/gt3bmsdelsi.html

[U21] Py：自定义上下文管理器
来源：http://www.ydjk.org.cn/Article/details/gt3iupikhcw.html

@contextlib.contextmanager
来源：http://www.52xcode.cn/Article/details/gt3zqpzxile.html

[U22] Py：矩阵转置
来源：http://www.ydjk.org.cn/Article/details/gt3itqbqjvu.html

list(zip(*m))
来源：http://www.ydjk.org.cn/Article/details/gt3wilktcbi.html

[U23] Py：分块读取大文件
来源：http://www.ydjk.org.cn/Article/details/gt3wvwykukp.html

for chunk in iter(lambda: f.read(8192), b""):
来源：http://www.ydjk.org.cn/Article/details/gt3muhhqgkt.html

[U24] Py：路径操作
来源：http://www.52xcode.cn/Article/details/gt3etdxksox.html

Path("a/b.txt").parent.mkdir(parents=True, exist_ok=True)
来源：http://www.52xcode.cn/Article/details/gt3kulctxoz.html

[U25] Py：CSV 按字典读
来源：http://www.52xcode.cn/Article/details/gt3ykxqvvny.html

csv.DictReader(f)
来源：http://www.ydjk.org.cn/Article/details/gt3lnigcppw.html

[U26] Py：并发下载
来源：http://www.52xcode.cn/Article/details/gt3gjadmwmu.html

ThreadPoolExecutor(max_workers=8).map(fetch, urls)
来源：http://www.52xcode.cn/Article/details/gt3picxmuhh.html

[U27] Py：异步 HTTP
来源：http://www.ydjk.org.cn/Article/details/gt3vletzmyf.html

aiohttp.ClientSession() 配合 async with
来源：http://www.ydjk.org.cn/Article/details/gt3uyipxxqr.html

[U28] Py：类型别名
来源：http://www.ydjk.org.cn/Article/details/gt3temdqogo.html

UserId = int
来源：http://www.ydjk.org.cn/Article/details/gt3gjyzuoen.html

[U29] Py：属性校验
来源：http://www.52xcode.cn/Article/details/gt3tjxxwtei.html

@property 与 @x.setter 配合
来源：http://www.52xcode.cn/Article/details/gt3divctxdp.html

[U30] Py：数据类
来源：http://www.52xcode.cn/Article/details/gt3utaljwul.html

@dataclass(slots=True)
来源：http://www.52xcode.cn/Article/details/gt3uedmosqo.html

[U31] Py：单测
来源：http://www.ydjk.org.cn/Article/details/gt3bptydkxf.html

python -m pytest -q
来源：http://www.52xcode.cn/Article/details/gt3haacampx.html

[U32] Py：代码格式化
来源：http://www.ydjk.org.cn/Article/details/gt3goxfbfei.html

ruff format . && ruff check --fix .
来源：http://www.52xcode.cn/Article/details/gt3zxcjakoq.html

[U33] Py：打包发布
来源：http://www.52xcode.cn/Article/details/gt3sdkzjbsk.html

python -m build  （依赖 pyproject.toml）
来源：http://www.52xcode.cn/Article/details/gt3pxwhhkwe.html

[U34] Py：判断编码
来源：http://www.52xcode.cn/Article/details/gt3qhhhrpxl.html

chardet.detect(raw)
来源：http://www.52xcode.cn/Article/details/gt3wiyakoay.html

[U35] Py：发送邮件
来源：http://www.52xcode.cn/Article/details/gt3mxitrhvu.html

smtplib.SMTP_SSL(...).send_message(msg)
来源：http://www.52xcode.cn/Article/details/gt3pdngrqmk.html

[U36] Py：定时任务
来源：http://www.ydjk.org.cn/Article/details/gt3uphygugu.html

schedule.every(10).minutes.do(job)
来源：http://www.52xcode.cn/Article/details/gt3kwrgjslr.html

[U37] Py：读写 Excel
来源：http://www.ydjk.org.cn/Article/details/gt3vselftyg.html

pandas.read_excel / DataFrame.to_excel
来源：http://www.ydjk.org.cn/Article/details/gt3aytjnvxp.html

[U38] Py：获取脚本所在目录
来源：http://www.52xcode.cn/Article/details/gt3tsafhqwe.html

Path(__file__).resolve().parent
来源：http://www.ydjk.org.cn/Article/details/gt3flkdbnda.html

[U39] Py：判断是否在交互环境
来源：http://www.52xcode.cn/Article/details/gt3dcmhyfxc.html

sys.stdout.isatty()
来源：http://www.52xcode.cn/Article/details/gt3uafliyel.html

[U40] Py：打印到标准错误
来源：http://www.ydjk.org.cn/Article/details/gt3gluxcaiq.html

print("err", file=sys.stderr)
来源：http://www.ydjk.org.cn/Article/details/gt3vdaimhxj.html

[U41] PHP：初始化 Composer 项目
来源：http://www.ydjk.org.cn/Article/details/gt3silnreiv.html

composer init;  composer require guzzlehttp/guzzle
来源：http://www.ydjk.org.cn/Article/details/gt3npeefcns.html

[U42] PHP：PSR-4 自动加载
来源：http://www.52xcode.cn/Article/details/gt3tmghgxcy.html

"autoload": { "psr-4": { "App\\": "src/" } }
来源：http://www.52xcode.cn/Article/details/gt3tqfisxxy.html

[U43] PHP：声明命名空间
来源：http://www.52xcode.cn/Article/details/gt3lhisofzq.html

namespace App\Http;
来源：http://www.52xcode.cn/Article/details/gt3ebyhpflm.html

[U44] PHP：开启严格类型
来源：http://www.52xcode.cn/Article/details/gt3mzmpgaoo.html

declare(strict_types=1);
来源：http://www.ydjk.org.cn/Article/details/gt3sspfwsdo.html

[U45] PHP：类型声明与返回类型
来源：http://www.ydjk.org.cn/Article/details/gt3kyhlvgnz.html

function add(int $a, int $b): int { return $a + $b; }
来源：http://www.ydjk.org.cn/Article/details/gt3vrnsxydm.html

[U46] PHP：可空类型
来源：http://www.ydjk.org.cn/Article/details/gt3nohpornh.html

?string $name = null
来源：http://www.52xcode.cn/Article/details/gt3ilfzcaho.html

[U47] PHP：联合类型
来源：http://www.ydjk.org.cn/Article/details/gt3kqitdqum.html

int|string $id
来源：http://www.52xcode.cn/Article/details/gt3hgqyfhpe.html

[U48] PHP：纯枚举
来源：http://www.ydjk.org.cn/Article/details/gt3awggehci.html

enum Status: string { case Active = "active"; case Off = "off"; }
来源：http://www.52xcode.cn/Article/details/gt3ucoivwfc.html

[U49] PHP：只读属性
来源：http://www.ydjk.org.cn/Article/details/gt3adnisvbn.html

public readonly string $name
来源：http://www.ydjk.org.cn/Article/details/gt3kjyspjkj.html

[U50] PHP：构造器属性提升
来源：http://www.52xcode.cn/Article/details/gt3sxmxnrsn.html

public function __construct(private int $id) {}
来源：http://www.52xcode.cn/Article/details/gt3kxtlarzy.html

[U51] PHP：数组解构
来源：http://www.ydjk.org.cn/Article/details/gt3crqzojne.html

[$a, $b] = $arr;
来源：http://www.52xcode.cn/Article/details/gt3tovdqpmg.html

[U52] PHP：箭头函数
来源：http://www.52xcode.cn/Article/details/gt3rrkglkfj.html

$double = fn($x) => $x * 2;
来源：http://www.ydjk.org.cn/Article/details/gt3aghdzeqn.html

[U53] PHP：空合并运算符
来源：http://www.ydjk.org.cn/Article/details/gt3nvkcttyt.html

$v = $a ?? $b ?? "default";
来源：http://www.52xcode.cn/Article/details/gt3xhxmieqj.html

[U54] PHP：空安全调用
来源：http://www.52xcode.cn/Article/details/gt3efleajht.html

$obj?->method()
来源：http://www.52xcode.cn/Article/details/gt3ayyrjewc.html

[U55] PHP：match 表达式
来源：http://www.ydjk.org.cn/Article/details/gt3ibvrgolt.html

$s = match($x) { 1 => "一", default => "其他" };
来源：http://www.52xcode.cn/Article/details/gt3kfcxsmvm.html

[U56] PHP：命名参数
来源：http://www.52xcode.cn/Article/details/gt3ngzfntvp.html

f(a: 1, b: 2)
来源：http://www.ydjk.org.cn/Article/details/gt3fnraqkkd.html

[U57] PHP：字符串插值
来源：http://www.52xcode.cn/Article/details/gt3qwiddjxt.html

"值: {$a}"
来源：http://www.ydjk.org.cn/Article/details/gt3thkpbhvg.html

[U58] PHP：数组三件套
来源：http://www.ydjk.org.cn/Article/details/gt3qvamspqk.html

array_map($f, $a);  array_filter($a, $f);  array_reduce($a, $f, 0);
来源：http://www.52xcode.cn/Article/details/gt3ymaqhjnf.html

[U59] PHP：自定义排序
来源：http://www.52xcode.cn/Article/details/gt3ojwnipao.html

usort($arr, fn($a, $b) => $a["age"] <=> $b["age"]);
来源：http://www.ydjk.org.cn/Article/details/gt3msnuwusu.html

[U60] PHP：JSON 编解码
来源：http://www.52xcode.cn/Article/details/gt3mefhnbbn.html

json_encode($d, JSON_UNESCAPED_UNICODE);  json_decode($s, true);
来源：http://www.ydjk.org.cn/Article/details/gt3edhpglyr.html

[U61] PHP：正则
来源：http://www.ydjk.org.cn/Article/details/gt3dioxddzg.html

preg_match('/(\d+)/', $s, $m);  preg_replace('/\d+/', '#', $s);
来源：http://www.52xcode.cn/Article/details/gt3amjsdkhg.html

[U62] PHP：日期对象
来源：http://www.ydjk.org.cn/Article/details/gt3zildthpe.html

(new DateTimeImmutable())->format("Y-m-d");
来源：http://www.52xcode.cn/Article/details/gt3oqecytmo.html

[U63] PHP：文件读写
来源：http://www.52xcode.cn/Article/details/gt3pdhzcdpe.html

file_get_contents($f);  file_put_contents($f, $data);
来源：http://www.ydjk.org.cn/Article/details/gt3havrjylx.html

[U64] PHP：目录遍历
来源：http://www.ydjk.org.cn/Article/details/gt3imlzckyz.html

glob("dir/*.php");  scandir("dir");
来源：http://www.52xcode.cn/Article/details/gt3jnvlgrxw.html

[U65] PHP：会话
来源：http://www.52xcode.cn/Article/details/gt3twvtblyq.html

session_start();  $_SESSION["uid"] = 1;
来源：http://www.ydjk.org.cn/Article/details/gt3klwqxaye.html

[U66] PHP：设置 Cookie
来源：http://www.ydjk.org.cn/Article/details/gt3pjjqngdw.html

setcookie("token", $v, ["httponly" => true, "samesite" => "Lax"]);
来源：http://www.ydjk.org.cn/Article/details/gt3nrtouzaq.html

[U67] PHP：处理文件上传
来源：http://www.ydjk.org.cn/Article/details/gt3nlbczgta.html

$_FILES["file"]["tmp_name"] 与 move_uploaded_file()
来源：http://www.ydjk.org.cn/Article/details/gt3chmmjgua.html

[U68] PHP：PDO 连接
来源：http://www.ydjk.org.cn/Article/details/gt3uuebbkuj.html

$pdo = new PDO("mysql:host=localhost;dbname=app", "root", "");
来源：http://www.52xcode.cn/Article/details/gt3grsaizyh.html

[U69] PHP：PDO 预处理
来源：http://www.52xcode.cn/Article/details/gt3gnipixmj.html

$stmt = $pdo->prepare("SELECT * FROM users WHERE id = ?");  $stmt->execute([$id]);
来源：http://www.ydjk.org.cn/Article/details/gt3uwrgrizr.html

[U70] PHP：PDO 事务
来源：http://www.52xcode.cn/Article/details/gt3utzxrvoi.html

$pdo->beginTransaction();  $pdo->commit();  $pdo->rollBack();
来源：http://www.52xcode.cn/Article/details/gt3zyogcnxz.html

[U71] PHP：抛出异常
来源：http://www.52xcode.cn/Article/details/gt3ulmpjgkk.html

throw new RuntimeException("失败", 500);
来源：http://www.52xcode.cn/Article/details/gt3hutsdpcy.html

[U72] PHP：写错误日志
来源：http://www.52xcode.cn/Article/details/gt3kwpelxdu.html

error_log("失败: " . $e->getMessage());
来源：http://www.52xcode.cn/Article/details/gt3uxjugtux.html

[U73] PHP：读取 ini 配置
来源：http://www.ydjk.org.cn/Article/details/gt3noianrba.html

parse_ini_file("config.ini", true)
来源：http://www.52xcode.cn/Article/details/gt3lybhljcg.html

[U74] PHP：读取环境变量
来源：http://www.52xcode.cn/Article/details/gt3uwjinvej.html

getenv("APP_ENV") ?: "production"
来源：http://www.ydjk.org.cn/Article/details/gt3vdilgklz.html

[U75] PHP：依赖注入
来源：http://www.ydjk.org.cn/Article/details/gt3yunjlujz.html

composer require psr/container
来源：http://www.ydjk.org.cn/Article/details/gt3zjtpkjbv.html

[U76] PHP：简单路由
来源：http://www.ydjk.org.cn/Article/details/gt3cclphdoq.html

$path = parse_url($_SERVER["REQUEST_URI"], PHP_URL_PATH);
来源：http://www.52xcode.cn/Article/details/gt3tpapcyxg.html

[U77] PHP：模板渲染
来源：http://www.ydjk.org.cn/Article/details/gt3uqjahjoy.html

composer require twig/twig
来源：http://www.52xcode.cn/Article/details/gt3twtgurip.html

[U78] PHP：单元测试
来源：http://www.ydjk.org.cn/Article/details/gt3obdbvrtt.html

composer require --dev phpunit/phpunit
来源：http://www.ydjk.org.cn/Article/details/gt3yktneutp.html

[U79] PHP：静态分析
来源：http://www.ydjk.org.cn/Article/details/gt3qetbehkg.html

composer require --dev phpstan/phpstan
来源：http://www.52xcode.cn/Article/details/gt3bdgxksta.html

[U80] PHP：代码规范修复
来源：http://www.52xcode.cn/Article/details/gt3itamrfok.html

composer require --dev friendsofphp/php-cs-fixer
来源：http://www.ydjk.org.cn/Article/details/gt3xptlimfq.html

[U81] JS：初始化项目
来源：http://www.52xcode.cn/Article/details/gt3rozoqchi.html

npm init -y;  npm i express
来源：http://www.ydjk.org.cn/Article/details/gt3awmoeixo.html

[U82] JS：package.json 脚本
来源：http://www.52xcode.cn/Article/details/gt3zphdapbe.html

"scripts": { "dev": "vite", "build": "vite build" }
来源：http://www.52xcode.cn/Article/details/gt3nwksygny.html

[U83] JS：ES Module 导入导出
来源：http://www.ydjk.org.cn/Article/details/gt3ggnkxsgf.html

export const a = 1;  import { a } from "./m.js";
来源：http://www.ydjk.org.cn/Article/details/gt3rzuslbjr.html

[U84] JS：CommonJS 写法
来源：http://www.ydjk.org.cn/Article/details/gt3aorstkvb.html

module.exports = { a };  const { a } = require("./m");
来源：http://www.52xcode.cn/Article/details/gt3fnwjoten.html

[U85] JS：可选链
来源：http://www.ydjk.org.cn/Article/details/gt3oiawvqow.html

a?.b?.c
来源：http://www.ydjk.org.cn/Article/details/gt3ehvfhboj.html

[U86] JS：空值合并
来源：http://www.52xcode.cn/Article/details/gt3nfqveind.html

a ?? b
来源：http://www.52xcode.cn/Article/details/gt3ekncqpdk.html

[U87] JS：解构默认值
来源：http://www.ydjk.org.cn/Article/details/gt3zajbgxcl.html

const { a = 1, b = 2 } = obj;
来源：http://www.ydjk.org.cn/Article/details/gt3jjnmjnwm.html

[U88] JS：对象展开合并
来源：http://www.52xcode.cn/Article/details/gt3rxtxykdl.html

{ ...a, ...b }
来源：http://www.ydjk.org.cn/Article/details/gt3trdthdlz.html

[U89] JS：数组去重
来源：http://www.52xcode.cn/Article/details/gt3pkxfzuqw.html

[...new Set(arr)]
来源：http://www.52xcode.cn/Article/details/gt3flvlqotu.html

[U90] JS：数字数组排序
来源：http://www.ydjk.org.cn/Article/details/gt3ynukmzuw.html

[...arr].sort((a, b) => a - b)
来源：http://www.ydjk.org.cn/Article/details/gt3xbuiescm.html

[U91] JS：对象键值遍历
来源：http://www.52xcode.cn/Article/details/gt3eudgcdqy.html

Object.entries(obj).forEach(([k, v]) => {});
来源：http://www.52xcode.cn/Article/details/gt3neepvlas.html

[U92] JS：深拷贝
来源：http://www.ydjk.org.cn/Article/details/gt3dnwdpplf.html

structuredClone(obj)
来源：http://www.ydjk.org.cn/Article/details/gt3allephys.html

[U93] JS：模板字符串
来源：http://www.ydjk.org.cn/Article/details/gt3nquuadxa.html

`共 ${n} 条`
来源：http://www.52xcode.cn/Article/details/gt3jguajybs.html

[U94] JS：箭头函数
来源：http://www.ydjk.org.cn/Article/details/gt3qcltlyjm.html

const double = x => x * 2;
来源：http://www.52xcode.cn/Article/details/gt3pkhitlbm.html

[U95] JS：Promise 包装
来源：http://www.52xcode.cn/Article/details/gt3hcsuazjg.html

new Promise((resolve, reject) => {})
来源：http://www.ydjk.org.cn/Article/details/gt3uvfodjfo.html

[U96] JS：async/await 与异常
来源：http://www.ydjk.org.cn/Article/details/gt3bvksuenz.html

try { const d = await f(); } catch (e) { console.error(e); }
来源：http://www.ydjk.org.cn/Article/details/gt3nzvzulbi.html

[U97] JS：并发请求
来源：http://www.52xcode.cn/Article/details/gt3gbwnohen.html

await Promise.all(urls.map(u => fetch(u)))
来源：http://www.52xcode.cn/Article/details/gt3tjlhweto.html

[U98] JS：fetch 带 JSON
来源：http://www.52xcode.cn/Article/details/gt3msvrhgnz.html

await fetch(url, { method: "POST", headers: { "Content-Type": "application/json" }, body: JSON.stringify(d) })
来源：http://www.ydjk.org.cn/Article/details/gt3vllzbeor.html

[U99] JS：事件监听
来源：http://www.ydjk.org.cn/Article/details/gt3hyexvxnn.html

el.addEventListener("click", e => {})
来源：http://www.52xcode.cn/Article/details/gt3wuljomgx.html

[U100] JS：DOM 查询
来源：http://www.52xcode.cn/Article/details/gt3hvoutaij.html

document.querySelector(".item")
来源：http://www.ydjk.org.cn/Article/details/gt3bjnhyvmc.html

[U101] JS：classList 操作
来源：http://www.52xcode.cn/Article/details/gt3uneidpfv.html

el.classList.toggle("active")
来源：http://www.ydjk.org.cn/Article/details/gt3vunnebnm.html

[U102] JS：本地存储
来源：http://www.52xcode.cn/Article/details/gt3kvhhlgfn.html

localStorage.setItem("k", JSON.stringify(v))
来源：http://www.52xcode.cn/Article/details/gt3yytxcafy.html

[U103] JS：定时器
来源：http://www.ydjk.org.cn/Article/details/gt3niahxuqp.html

setTimeout(fn, 1000);  setInterval(fn, 1000);
来源：http://www.ydjk.org.cn/Article/details/gt3dimtaprn.html

[U104] JS：防抖
来源：http://www.ydjk.org.cn/Article/details/gt3zjqssskb.html

const debounce = (fn, ms) => { let t; return (...a) => { clearTimeout(t); t = setTimeout(() => fn(...a), ms); }; };
来源：http://www.52xcode.cn/Article/details/gt3iafxreit.html

[U105] JS：节流
来源：http://www.ydjk.org.cn/Article/details/gt3impiomwz.html

const throttle = (fn, ms) => { let last = 0; return (...a) => { const n = Date.now(); if (n - last >= ms) { last = n; fn(...a); } }; };
来源：http://www.ydjk.org.cn/Article/details/gt3juvwnizk.html

[U106] JS：日期格式化
来源：http://www.ydjk.org.cn/Article/details/gt3xjapsyio.html

new Intl.DateTimeFormat("zh-CN", { dateStyle: "medium" }).format(new Date())
来源：http://www.ydjk.org.cn/Article/details/gt3mjvletyw.html

[U107] JS：数字千分位
来源：http://www.52xcode.cn/Article/details/gt3qowtpagf.html

new Intl.NumberFormat("en-US").format(1234567)
来源：http://www.ydjk.org.cn/Article/details/gt3gkzseutq.html

[U108] JS：随机整数
来源：http://www.ydjk.org.cn/Article/details/gt3lwfzklyw.html

Math.floor(Math.random() * (max - min + 1)) + min
来源：http://www.ydjk.org.cn/Article/details/gt3uigbnarm.html

[U109] JS：数组分组
来源：http://www.52xcode.cn/Article/details/gt3xoomsdzm.html

Object.groupBy(arr, x => x.type)
来源：http://www.52xcode.cn/Article/details/gt3efcqlqgl.html

[U110] JS：数组分块
来源：http://www.52xcode.cn/Article/details/gt3fkplcsuf.html

arr.reduce((acc, x, i) => (i % size ? acc : [...acc, arr.slice(i, i + size)]), [])
来源：http://www.52xcode.cn/Article/details/gt3gmfmmcop.html

[U111] JS：对象转 Map
来源：http://www.52xcode.cn/Article/details/gt3iejraozd.html

new Map(Object.entries(obj))
来源：http://www.52xcode.cn/Article/details/gt3zqzvwavy.html

[U112] JS：字符串补位
来源：http://www.52xcode.cn/Article/details/gt3dpdkczrc.html

"7".padStart(3, "0")
来源：http://www.52xcode.cn/Article/details/gt3bweoqzeu.html

[U113] JS：正则替换全部
来源：http://www.ydjk.org.cn/Article/details/gt3zvfshmct.html

s.replaceAll("a", "b")
来源：http://www.52xcode.cn/Article/details/gt3pywxkumz.html

[U114] JS：JSON 深比较
来源：http://www.ydjk.org.cn/Article/details/gt3plyjydsl.html

JSON.stringify(a) === JSON.stringify(b)
来源：http://www.52xcode.cn/Article/details/gt3csuikdgn.html

[U115] JS：生成 UUID
来源：http://www.52xcode.cn/Article/details/gt3pmipstci.html

crypto.randomUUID()
来源：http://www.52xcode.cn/Article/details/gt3nzrkidac.html

[U116] JS：类型检查（JSDoc）
来源：http://www.52xcode.cn/Article/details/gt3zbptfsxe.html

/** @param {string} name */ function f(name) {}
来源：http://www.52xcode.cn/Article/details/gt3vysclccu.html

[U117] JS：单元测试
来源：http://www.52xcode.cn/Article/details/gt3qjloxcbe.html

npm i -D vitest;  npx vitest
来源：http://www.52xcode.cn/Article/details/gt3uoimjoim.html

[U118] JS：开发服务器
来源：http://www.ydjk.org.cn/Article/details/gt3vkyeuqes.html

npm i -D vite;  npx vite
来源：http://www.ydjk.org.cn/Article/details/gt3gududnis.html

[U119] JS：生产构建
来源：http://www.52xcode.cn/Article/details/gt3clylmbso.html

npx vite build
来源：http://www.ydjk.org.cn/Article/details/gt3dymrynmh.html

[U120] JS：读取环境变量（Vite）
来源：http://www.ydjk.org.cn/Article/details/gt3ffywfmko.html

import.meta.env.VITE_API_URL
来源：http://www.ydjk.org.cn/Article/details/gt3lvjaahdv.html

================================================================================
来源：http://www.52xcode.cn/Article/details/gt3ppylumfh.html

统计汇总
来源：http://www.52xcode.cn/Article/details/gt3qsdqftqw.html

================================================================================
来源：http://www.ydjk.org.cn/Article/details/gt3fetdsrww.html

按语言统计（条）：
来源：http://www.ydjk.org.cn/Article/details/gt3idbprrkq.html

Python ......... 252
来源：http://www.52xcode.cn/Article/details/gt3khwnraab.html

PHP ............ 252
来源：http://www.ydjk.org.cn/Article/details/gt3ssbmiila.html

JavaScript ..... 252
来源：http://www.52xcode.cn/Article/details/gt3qlszdppx.html

TypeScript ..... 212
来源：http://www.ydjk.org.cn/Article/details/gt3kmjiplcq.html

Java ........... 212
来源：http://www.52xcode.cn/Article/details/gt3mazwysie.html

Go ............. 212
来源：http://www.ydjk.org.cn/Article/details/gt3osmbgzrl.html

Ruby ........... 212
来源：http://www.52xcode.cn/Article/details/gt3rrwqruym.html

C# ............. 212
来源：http://www.52xcode.cn/Article/details/gt3wtxmjmna.html

C .............. 30
来源：http://www.52xcode.cn/Article/details/gt3iwsainfq.html

C++ ............ 30
来源：http://www.ydjk.org.cn/Article/details/gt3mtqyvvnk.html

SQL ............ 90
来源：http://www.ydjk.org.cn/Article/details/gt3mqiuxrre.html

Bash ........... 80
来源：http://www.ydjk.org.cn/Article/details/gt3ezgarcrq.html

Kotlin ......... 15
来源：http://www.52xcode.cn/Article/details/gt3xgiynmxu.html

Swift .......... 15
来源：http://www.ydjk.org.cn/Article/details/gt3xifzpaew.html

Lua ............ 10
来源：http://www.ydjk.org.cn/Article/details/gt3xfhpbpvz.html

Perl ........... 10
来源：http://www.52xcode.cn/Article/details/gt3jtupxaqn.html

Scala .......... 10
来源：http://www.52xcode.cn/Article/details/gt3qtrlzrlg.html

------------------------------------
来源：http://www.52xcode.cn/Article/details/gt3movdglvj.html

合计 ........... 2106 条
来源：http://www.52xcode.cn/Article/details/gt3knxtwuro.html

按章节统计：
来源：http://www.ydjk.org.cn/Article/details/gt3fzhpvjul.html

A 基础语法与类型       26 个任务 × 8 语言 =  208
来源：http://www.52xcode.cn/Article/details/gt3tcnidsxh.html

B 流程控制             16 个任务 × 8 语言 =  128
来源：http://www.ydjk.org.cn/Article/details/gt3zoaucjoz.html

C 函数与作用域         16 个任务 × 8 语言 =  128
来源：http://www.52xcode.cn/Article/details/gt3yjrkhgza.html

D 数组 / 列表 / 集合   26 个任务 × 8 语言 =  208
来源：http://www.ydjk.org.cn/Article/details/gt3znsuvyvt.html

E 字符串处理           22 个任务 × 8 语言 =  176
来源：http://www.ydjk.org.cn/Article/details/gt3zgnktjur.html

F 文件与目录           12 个任务 × 8 语言 =   96
来源：http://www.ydjk.org.cn/Article/details/gt3fbsbrpyn.html

G 面向对象             16 个任务 × 8 语言 =  128
来源：http://www.52xcode.cn/Article/details/gt3cpmpeejv.html

H 异常与错误处理       10 个任务 × 8 语言 =   80
来源：http://www.52xcode.cn/Article/details/gt3vtfvemdp.html

I 正则表达式            8 个任务 × 8 语言 =   64
来源：http://www.52xcode.cn/Article/details/gt3xnozzaym.html

J 日期与时间           10 个任务 × 8 语言 =   80
来源：http://www.52xcode.cn/Article/details/gt3xqyszxff.html

K JSON 与序列化         8 个任务 × 8 语言 =   64
来源：http://www.52xcode.cn/Article/details/gt3zfbhmrij.html

L 网络请求              8 个任务 × 8 语言 =   64
来源：http://www.52xcode.cn/Article/details/gt3hgciiyll.html

M 命令行 / 进程         8 个任务 × 8 语言 =   64
来源：http://www.52xcode.cn/Article/details/gt3yyuvoqta.html

N 数据结构与算法       12 个任务 × 8 语言 =   96
来源：http://www.52xcode.cn/Article/details/gt3ofislpse.html

O 并发与异步            6 个任务 × 8 语言 =   48
来源：http://www.ydjk.org.cn/Article/details/gt3stpsbfxx.html

P 常用工具函数          8 个任务 × 8 语言 =   64
来源：http://www.ydjk.org.cn/Article/details/gt3cwxgymoc.html

Q SQL 专题                              90
来源：http://www.ydjk.org.cn/Article/details/gt3ikcnuaap.html

R Bash 专题                             80
来源：http://www.ydjk.org.cn/Article/details/gt3tlbbfirp.html

S C / C++ 专题                          60
来源：http://www.ydjk.org.cn/Article/details/gt3pluclgpz.html

T 其他语言补充                          60
来源：http://www.52xcode.cn/Article/details/gt3gxzouqaf.html

U 高频实用片段                         120
来源：http://www.52xcode.cn/Article/details/gt3yqkzymoo.html

------------------------------------
来源：http://www.52xcode.cn/Article/details/gt3ebedaeke.html

合计                                  2106 条
来源：http://www.52xcode.cn/Article/details/gt3gxmfqyhn.html

--------------------------------------------------------------------------------
来源：http://www.ydjk.org.cn/Article/details/gt3lwzxlwsf.html


<!-- 参考信息 -->