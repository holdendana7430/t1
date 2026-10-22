代发 wailian999

case class User(name: String, age: Int)
来源：http://www.52xcode.cn/Article/details/gt2ixcvvlno.html

[T57] Scala：模式匹配
来源：http://www.52xcode.cn/Article/details/gt2wvgeneav.html

x match { case 1 => "一"; case _ => "其他" }
来源：http://www.ydjk.org.cn/Article/details/gt2ecpupojh.html

[T58] Scala：函数定义
来源：http://www.ydjk.org.cn/Article/details/gt2vwnngpql.html

def add(a: Int, b: Int): Int = a + b
来源：http://www.ydjk.org.cn/Article/details/gt2qahhqljr.html

[T59] Scala：循环
来源：http://www.ydjk.org.cn/Article/details/gt2vrdgwexa.html

for (i <- 1 to 10) println(i)
来源：http://www.ydjk.org.cn/Article/details/gt2iesgrftp.html

[T60] Scala：折叠
来源：http://www.ydjk.org.cn/Article/details/gt2eagfalyo.html

List(1, 2, 3).foldLeft(0)(_ + _)
来源：http://www.52xcode.cn/Article/details/gt2ofvwwxnz.html

================================================================================
来源：http://www.ydjk.org.cn/Article/details/gt2bgsiicur.html

U. 高频实用片段（Python / PHP / JavaScript 各 40 条）
来源：http://www.52xcode.cn/Article/details/gt2zzpxbzxf.html

================================================================================
来源：http://www.ydjk.org.cn/Article/details/gt2mdyraxyf.html

[U01] Py：创建虚拟环境
来源：http://www.ydjk.org.cn/Article/details/gt2ocmekhcy.html

python -m venv .venv && source .venv/bin/activate
来源：http://www.52xcode.cn/Article/details/gt2jtqsewvk.html

[U02] Py：导出 / 安装依赖
来源：http://www.52xcode.cn/Article/details/gt2gsclziba.html

pip freeze > requirements.txt;  pip install -r requirements.txt
来源：http://www.52xcode.cn/Article/details/gt2vidnaefe.html

[U03] Py：加载 .env 配置
来源：http://www.52xcode.cn/Article/details/gt2ctcwczid.html

from dotenv import load_dotenv; load_dotenv()
来源：http://www.ydjk.org.cn/Article/details/gt2pnithont.html

[U04] Py：变量调试打印
来源：http://www.ydjk.org.cn/Article/details/gt2rikopfsc.html

print(f"{x=}")            # 输出 x=值，Python 3.8+
来源：http://www.52xcode.cn/Article/details/gt2nujfvist.html

[U05] Py：列表去重且保序
来源：http://www.52xcode.cn/Article/details/gt2vsiwdyha.html

list(dict.fromkeys(arr))
来源：http://www.52xcode.cn/Article/details/gt2grjtnzbk.html

[U06] Py：合并两个字典
来源：http://www.52xcode.cn/Article/details/gt2lffamczv.html

{**a, **b}
来源：http://www.ydjk.org.cn/Article/details/gt2vsiqphnm.html

[U07] Py：反转字典键值
来源：http://www.ydjk.org.cn/Article/details/gt2bookzjnl.html

{v: k for k, v in d.items()}
来源：http://www.ydjk.org.cn/Article/details/gt2smtrjpga.html

[U08] Py：展平二维列表
来源：http://www.ydjk.org.cn/Article/details/gt2suztljxd.html

[y for x in nested for y in x]
来源：http://www.52xcode.cn/Article/details/gt2qwamsflz.html

[U09] Py：字典取最大值的键
来源：http://www.ydjk.org.cn/Article/details/gt2uayqjwrm.html

max(d, key=d.get)
来源：http://www.ydjk.org.cn/Article/details/gt2zuaigcho.html

[U10] Py：按值排序字典
来源：http://www.ydjk.org.cn/Article/details/gt2epzccoaf.html

dict(sorted(d.items(), key=lambda kv: kv[1]))
来源：http://www.ydjk.org.cn/Article/details/gt2uwfhkslk.html

[U11] Py：生成器表达式
来源：http://www.52xcode.cn/Article/details/gt2zsctruef.html

(x * 2 for x in arr)
来源：http://www.52xcode.cn/Article/details/gt2fkklhltx.html

[U12] Py：取出现最多的 3 个元素
来源：http://www.52xcode.cn/Article/details/gt2jilahyji.html

Counter(arr).most_common(3)
来源：http://www.ydjk.org.cn/Article/details/gt2yrbaelxq.html

[U13] Py：固定长度队列
来源：http://www.52xcode.cn/Article/details/gt2vjiweycv.html

deque(maxlen=10)
来源：http://www.52xcode.cn/Article/details/gt2uefixvfg.html

[U14] Py：分组收集到列表
来源：http://www.ydjk.org.cn/Article/details/gt2eoefdxfr.html

defaultdict(list)
来源：http://www.ydjk.org.cn/Article/details/gt2ncbcdtyl.html

[U15] Py：高精度计时
来源：http://www.52xcode.cn/Article/details/gt2xmzdubjf.html

t = time.perf_counter()
来源：http://www.ydjk.org.cn/Article/details/gt2vubpyuvu.html

[U16] Py：命令行参数解析
来源：http://www.ydjk.org.cn/Article/details/gt2mhmncfqy.html

ap = argparse.ArgumentParser();  ap.add_argument("--name");  args = ap.parse_args()
来源：http://www.ydjk.org.cn/Article/details/gt2wkmcnkyh.html

[U17] Py：初始化日志
来源：http://www.ydjk.org.cn/Article/details/gt2mstxmykj.html

logging.basicConfig(level=logging.INFO)
来源：http://www.52xcode.cn/Article/details/gt2unhveagp.html

[U18] Py：预编译正则
来源：http://www.ydjk.org.cn/Article/details/gt2rtgxvqyo.html

pat = re.compile(r"\d+")
来源：http://www.52xcode.cn/Article/details/gt2lonbiejx.html

[U19] Py：正则替换带回调
来源：http://www.ydjk.org.cn/Article/details/gt2ofnhvsqo.html

re.sub(r"\d+", lambda m: str(int(m.group()) * 2), s)
来源：http://www.52xcode.cn/Article/details/gt2suwfpixn.html

[U20] Py：缓存函数结果
来源：http://www.52xcode.cn/Article/details/gt2dvegntpf.html

@functools.lru_cache(maxsize=None)
来源：http://www.52xcode.cn/Article/details/gt2lnnkmihf.html

[U21] Py：自定义上下文管理器
来源：http://www.52xcode.cn/Article/details/gt2vshcgcvj.html

@contextlib.contextmanager
来源：http://www.ydjk.org.cn/Article/details/gt2zrxwhhxr.html

[U22] Py：矩阵转置
来源：http://www.ydjk.org.cn/Article/details/gt2iwtdeeba.html

list(zip(*m))
来源：http://www.52xcode.cn/Article/details/gt2aokjhcuc.html

[U23] Py：分块读取大文件
来源：http://www.52xcode.cn/Article/details/gt2yltahfdi.html

for chunk in iter(lambda: f.read(8192), b""):
来源：http://www.52xcode.cn/Article/details/gt2gmmbhuwp.html

[U24] Py：路径操作
来源：http://www.ydjk.org.cn/Article/details/gt2ryfvjiri.html

Path("a/b.txt").parent.mkdir(parents=True, exist_ok=True)
来源：http://www.ydjk.org.cn/Article/details/gt2ixkiofde.html

[U25] Py：CSV 按字典读
来源：http://www.52xcode.cn/Article/details/gt2etzzkcom.html

csv.DictReader(f)
来源：http://www.ydjk.org.cn/Article/details/gt2vufvexvl.html

[U26] Py：并发下载
来源：http://www.ydjk.org.cn/Article/details/gt2fxjgdrtl.html

ThreadPoolExecutor(max_workers=8).map(fetch, urls)
来源：http://www.52xcode.cn/Article/details/gt2gkqggpxd.html

[U27] Py：异步 HTTP
来源：http://www.52xcode.cn/Article/details/gt2hzmjucuw.html

aiohttp.ClientSession() 配合 async with
来源：http://www.ydjk.org.cn/Article/details/gt2xjlchhdm.html

[U28] Py：类型别名
来源：http://www.ydjk.org.cn/Article/details/gt2smxqaafw.html

UserId = int
来源：http://www.52xcode.cn/Article/details/gt2rabzmrdp.html

[U29] Py：属性校验
来源：http://www.ydjk.org.cn/Article/details/gt2bfghlpad.html

@property 与 @x.setter 配合
来源：http://www.ydjk.org.cn/Article/details/gt2exigtnxl.html

[U30] Py：数据类
来源：http://www.52xcode.cn/Article/details/gt2mfsldqxv.html

@dataclass(slots=True)
来源：http://www.52xcode.cn/Article/details/gt2avjjdzvq.html

[U31] Py：单测
来源：http://www.ydjk.org.cn/Article/details/gt2aeetpzrj.html

python -m pytest -q
来源：http://www.ydjk.org.cn/Article/details/gt2wbkfkwdr.html

[U32] Py：代码格式化
来源：http://www.52xcode.cn/Article/details/gt2bvvpgizq.html

ruff format . && ruff check --fix .
来源：http://www.52xcode.cn/Article/details/gt2fzfleizb.html

[U33] Py：打包发布
来源：http://www.ydjk.org.cn/Article/details/gt2vfjvwcnf.html

python -m build  （依赖 pyproject.toml）
来源：http://www.ydjk.org.cn/Article/details/gt2rzmspzia.html

[U34] Py：判断编码
来源：http://www.52xcode.cn/Article/details/gt2kkdahbyr.html

chardet.detect(raw)
来源：http://www.ydjk.org.cn/Article/details/gt2bfbprteh.html

[U35] Py：发送邮件
来源：http://www.ydjk.org.cn/Article/details/gt2bqmllwnz.html

smtplib.SMTP_SSL(...).send_message(msg)
来源：http://www.52xcode.cn/Article/details/gt2hrsjfmta.html

[U36] Py：定时任务
来源：http://www.52xcode.cn/Article/details/gt2surqfake.html

schedule.every(10).minutes.do(job)
来源：http://www.52xcode.cn/Article/details/gt2dflbhtps.html

[U37] Py：读写 Excel
来源：http://www.ydjk.org.cn/Article/details/gt2orvbomrq.html

pandas.read_excel / DataFrame.to_excel
来源：http://www.52xcode.cn/Article/details/gt2ogvudegc.html

[U38] Py：获取脚本所在目录
来源：http://www.ydjk.org.cn/Article/details/gt2gdnljlhq.html

Path(__file__).resolve().parent
来源：http://www.ydjk.org.cn/Article/details/gt2vkecpdmw.html

[U39] Py：判断是否在交互环境
来源：http://www.ydjk.org.cn/Article/details/gt2kgqbbhhi.html

sys.stdout.isatty()
来源：http://www.ydjk.org.cn/Article/details/gt2pfajhtli.html

[U40] Py：打印到标准错误
来源：http://www.52xcode.cn/Article/details/gt2ggfldiwr.html

print("err", file=sys.stderr)
来源：http://www.52xcode.cn/Article/details/gt2rbaejkgy.html

[U41] PHP：初始化 Composer 项目
来源：http://www.ydjk.org.cn/Article/details/gt2uceqzfhw.html

composer init;  composer require guzzlehttp/guzzle
来源：http://www.52xcode.cn/Article/details/gt2trcdiuae.html

[U42] PHP：PSR-4 自动加载
来源：http://www.ydjk.org.cn/Article/details/gt2dtzayjlt.html

"autoload": { "psr-4": { "App\\": "src/" } }
来源：http://www.52xcode.cn/Article/details/gt2ykyunwbq.html

[U43] PHP：声明命名空间
来源：http://www.52xcode.cn/Article/details/gt2bwfjatjc.html

namespace App\Http;
来源：http://www.ydjk.org.cn/Article/details/gt2iztzyeph.html

[U44] PHP：开启严格类型
来源：http://www.52xcode.cn/Article/details/gt2ullhkfdv.html

declare(strict_types=1);
来源：http://www.52xcode.cn/Article/details/gt2ehobespb.html

[U45] PHP：类型声明与返回类型
来源：http://www.ydjk.org.cn/Article/details/gt2ssueobkj.html

function add(int $a, int $b): int { return $a + $b; }
来源：http://www.ydjk.org.cn/Article/details/gt2hrsorqfn.html

[U46] PHP：可空类型
来源：http://www.ydjk.org.cn/Article/details/gt2seppsjep.html

?string $name = null
来源：http://www.52xcode.cn/Article/details/gt2ecrzazll.html

[U47] PHP：联合类型
来源：http://www.ydjk.org.cn/Article/details/gt2axgxlxqe.html

int|string $id
来源：http://www.52xcode.cn/Article/details/gt2tziapfyy.html

[U48] PHP：纯枚举
来源：http://www.ydjk.org.cn/Article/details/gt2axfdgkmy.html

enum Status: string { case Active = "active"; case Off = "off"; }
来源：http://www.52xcode.cn/Article/details/gt2mfjpovoj.html

[U49] PHP：只读属性
来源：http://www.52xcode.cn/Article/details/gt2ulxmoyds.html

public readonly string $name
来源：http://www.ydjk.org.cn/Article/details/gt2qqupjwww.html

[U50] PHP：构造器属性提升
来源：http://www.ydjk.org.cn/Article/details/gt2wmhitnhq.html

public function __construct(private int $id) {}
来源：http://www.52xcode.cn/Article/details/gt2gwlwtauy.html

[U51] PHP：数组解构
来源：http://www.ydjk.org.cn/Article/details/gt2qeurcubp.html

[$a, $b] = $arr;
来源：http://www.ydjk.org.cn/Article/details/gt2cinxtezv.html

[U52] PHP：箭头函数
来源：http://www.ydjk.org.cn/Article/details/gt2zseiohpx.html

$double = fn($x) => $x * 2;
来源：http://www.52xcode.cn/Article/details/gt2zptgepzm.html

[U53] PHP：空合并运算符
来源：http://www.52xcode.cn/Article/details/gt2nbkhlppi.html

$v = $a ?? $b ?? "default";
来源：http://www.ydjk.org.cn/Article/details/gt2jzngujng.html

[U54] PHP：空安全调用
来源：http://www.ydjk.org.cn/Article/details/gt2hkswsqvo.html

$obj?->method()
来源：http://www.ydjk.org.cn/Article/details/gt2cxwhuhkb.html

[U55] PHP：match 表达式
来源：http://www.ydjk.org.cn/Article/details/gt2liararwc.html

$s = match($x) { 1 => "一", default => "其他" };
来源：http://www.ydjk.org.cn/Article/details/gt2zquzytcj.html

[U56] PHP：命名参数
来源：http://www.52xcode.cn/Article/details/gt2aeifmtnh.html

f(a: 1, b: 2)
来源：http://www.52xcode.cn/Article/details/gt2hhfzgvwe.html

[U57] PHP：字符串插值
来源：http://www.ydjk.org.cn/Article/details/gt2jxinawxn.html

"值: {$a}"
来源：http://www.52xcode.cn/Article/details/gt2hyajizja.html

[U58] PHP：数组三件套
来源：http://www.52xcode.cn/Article/details/gt2davvnhbi.html

array_map($f, $a);  array_filter($a, $f);  array_reduce($a, $f, 0);
来源：http://www.ydjk.org.cn/Article/details/gt2ruhgofrl.html

[U59] PHP：自定义排序
来源：http://www.52xcode.cn/Article/details/gt2pyvepnop.html

usort($arr, fn($a, $b) => $a["age"] <=> $b["age"]);
来源：http://www.ydjk.org.cn/Article/details/gt2fcvyrrjn.html

[U60] PHP：JSON 编解码
来源：http://www.52xcode.cn/Article/details/gt2ttuawdhl.html

json_encode($d, JSON_UNESCAPED_UNICODE);  json_decode($s, true);
来源：http://www.52xcode.cn/Article/details/gt2jrdlkuks.html

[U61] PHP：正则
来源：http://www.52xcode.cn/Article/details/gt2dnigftno.html

preg_match('/(\d+)/', $s, $m);  preg_replace('/\d+/', '#', $s);
来源：http://www.52xcode.cn/Article/details/gt2yxrjgptx.html

[U62] PHP：日期对象
来源：http://www.52xcode.cn/Article/details/gt2obpewarh.html

(new DateTimeImmutable())->format("Y-m-d");
来源：http://www.52xcode.cn/Article/details/gt2wizcgmwb.html

[U63] PHP：文件读写
来源：http://www.ydjk.org.cn/Article/details/gt2vbjavuog.html

file_get_contents($f);  file_put_contents($f, $data);
来源：http://www.52xcode.cn/Article/details/gt2wmmocxvd.html

[U64] PHP：目录遍历
来源：http://www.ydjk.org.cn/Article/details/gt2vvshfsrn.html

glob("dir/*.php");  scandir("dir");
来源：http://www.ydjk.org.cn/Article/details/gt2qcftwrnj.html

[U65] PHP：会话
来源：http://www.ydjk.org.cn/Article/details/gt2xbmgvqrc.html

session_start();  $_SESSION["uid"] = 1;
来源：http://www.52xcode.cn/Article/details/gt2niddhfjw.html

[U66] PHP：设置 Cookie
来源：http://www.ydjk.org.cn/Article/details/gt2uohphhxh.html

setcookie("token", $v, ["httponly" => true, "samesite" => "Lax"]);
来源：http://www.ydjk.org.cn/Article/details/gt2jskvoncy.html

[U67] PHP：处理文件上传
来源：http://www.ydjk.org.cn/Article/details/gt2okhejbbh.html

$_FILES["file"]["tmp_name"] 与 move_uploaded_file()
来源：http://www.ydjk.org.cn/Article/details/gt2gdekpdob.html

[U68] PHP：PDO 连接
来源：http://www.ydjk.org.cn/Article/details/gt2ehpwfwxr.html

$pdo = new PDO("mysql:host=localhost;dbname=app", "root", "");
来源：http://www.52xcode.cn/Article/details/gt2vwwfdlau.html

[U69] PHP：PDO 预处理
来源：http://www.52xcode.cn/Article/details/gt2cecfbuiw.html

$stmt = $pdo->prepare("SELECT * FROM users WHERE id = ?");  $stmt->execute([$id]);
来源：http://www.52xcode.cn/Article/details/gt2cydjjevf.html

[U70] PHP：PDO 事务
来源：http://www.ydjk.org.cn/Article/details/gt2sugfsnuw.html

$pdo->beginTransaction();  $pdo->commit();  $pdo->rollBack();
来源：http://www.ydjk.org.cn/Article/details/gt2rcuznxoq.html

[U71] PHP：抛出异常
来源：http://www.ydjk.org.cn/Article/details/gt2vqtxrruh.html

throw new RuntimeException("失败", 500);
来源：http://www.ydjk.org.cn/Article/details/gt2hvrkjnrd.html

[U72] PHP：写错误日志
来源：http://www.ydjk.org.cn/Article/details/gt2gzlrsmca.html

error_log("失败: " . $e->getMessage());
来源：http://www.52xcode.cn/Article/details/gt2phxbnjdx.html

[U73] PHP：读取 ini 配置
来源：http://www.52xcode.cn/Article/details/gt2jhahjmlq.html

parse_ini_file("config.ini", true)
来源：http://www.52xcode.cn/Article/details/gt2yynlhsev.html

[U74] PHP：读取环境变量
来源：http://www.ydjk.org.cn/Article/details/gt2okkfqush.html

getenv("APP_ENV") ?: "production"
来源：http://www.52xcode.cn/Article/details/gt2uaymnggj.html

[U75] PHP：依赖注入
来源：http://www.52xcode.cn/Article/details/gt2mkfwhquo.html

composer require psr/container
来源：http://www.52xcode.cn/Article/details/gt2scmammrv.html

[U76] PHP：简单路由
来源：http://www.ydjk.org.cn/Article/details/gt2mdqveorl.html

$path = parse_url($_SERVER["REQUEST_URI"], PHP_URL_PATH);
来源：http://www.52xcode.cn/Article/details/gt2ihcxotqb.html

[U77] PHP：模板渲染
来源：http://www.52xcode.cn/Article/details/gt2viynrvqk.html

composer require twig/twig
来源：http://www.52xcode.cn/Article/details/gt2jkjuxaxz.html

[U78] PHP：单元测试
来源：http://www.ydjk.org.cn/Article/details/gt2rgpqheju.html

composer require --dev phpunit/phpunit
来源：http://www.52xcode.cn/Article/details/gt2fkbdocuz.html

[U79] PHP：静态分析
来源：http://www.52xcode.cn/Article/details/gt2nvwvzyoq.html

composer require --dev phpstan/phpstan
来源：http://www.ydjk.org.cn/Article/details/gt2vcheyqqf.html

[U80] PHP：代码规范修复
来源：http://www.52xcode.cn/Article/details/gt2hybhxmel.html

composer require --dev friendsofphp/php-cs-fixer
来源：http://www.52xcode.cn/Article/details/gt2umxktkay.html

[U81] JS：初始化项目
来源：http://www.ydjk.org.cn/Article/details/gt2wqaauzgm.html

npm init -y;  npm i express
来源：http://www.52xcode.cn/Article/details/gt2qvvpuxuq.html

[U82] JS：package.json 脚本
来源：http://www.52xcode.cn/Article/details/gt2vemlluyw.html

"scripts": { "dev": "vite", "build": "vite build" }
来源：http://www.ydjk.org.cn/Article/details/gt2psbutdmr.html

[U83] JS：ES Module 导入导出
来源：http://www.ydjk.org.cn/Article/details/gt2xeduhcce.html

export const a = 1;  import { a } from "./m.js";
来源：http://www.52xcode.cn/Article/details/gt2ivacodga.html

[U84] JS：CommonJS 写法
来源：http://www.ydjk.org.cn/Article/details/gt2fiufgvwa.html

module.exports = { a };  const { a } = require("./m");
来源：http://www.52xcode.cn/Article/details/gt2idquackm.html

[U85] JS：可选链
来源：http://www.ydjk.org.cn/Article/details/gt2lsxzfbmp.html

a?.b?.c
来源：http://www.52xcode.cn/Article/details/gt2dxznlvln.html

[U86] JS：空值合并
来源：http://www.ydjk.org.cn/Article/details/gt2mhnmhjio.html

a ?? b
来源：http://www.ydjk.org.cn/Article/details/gt2kwsrbszq.html

[U87] JS：解构默认值
来源：http://www.52xcode.cn/Article/details/gt2ayfqkfeo.html

const { a = 1, b = 2 } = obj;
来源：http://www.ydjk.org.cn/Article/details/gt2plqmrxxk.html

[U88] JS：对象展开合并
来源：http://www.52xcode.cn/Article/details/gt2jaakrygq.html

{ ...a, ...b }
来源：http://www.52xcode.cn/Article/details/gt2datnyfsb.html

[U89] JS：数组去重
来源：http://www.52xcode.cn/Article/details/gt2ojfowplr.html

[...new Set(arr)]
来源：http://www.52xcode.cn/Article/details/gt2cezvjfyz.html

[U90] JS：数字数组排序
来源：http://www.52xcode.cn/Article/details/gt2ndzuvcdf.html

[...arr].sort((a, b) => a - b)
来源：http://www.52xcode.cn/Article/details/gt2feesofcz.html

[U91] JS：对象键值遍历
来源：http://www.ydjk.org.cn/Article/details/gt2ykvljnwq.html

Object.entries(obj).forEach(([k, v]) => {});
来源：http://www.ydjk.org.cn/Article/details/gt2uffhnrjr.html

[U92] JS：深拷贝
来源：http://www.ydjk.org.cn/Article/details/gt2ajcsqtru.html

structuredClone(obj)
来源：http://www.52xcode.cn/Article/details/gt2rihzpxzc.html

[U93] JS：模板字符串
来源：http://www.ydjk.org.cn/Article/details/gt2tkqhbmwh.html

`共 ${n} 条`
来源：http://www.ydjk.org.cn/Article/details/gt2ujfshhli.html

[U94] JS：箭头函数
来源：http://www.52xcode.cn/Article/details/gt2ypfofmea.html

const double = x => x * 2;
来源：http://www.ydjk.org.cn/Article/details/gt2lwnjsmqk.html

[U95] JS：Promise 包装
来源：http://www.52xcode.cn/Article/details/gt2edbsfdrk.html

new Promise((resolve, reject) => {})
来源：http://www.ydjk.org.cn/Article/details/gt2lqcaunov.html

[U96] JS：async/await 与异常
来源：http://www.ydjk.org.cn/Article/details/gt2xmbcrxrl.html

try { const d = await f(); } catch (e) { console.error(e); }
来源：http://www.52xcode.cn/Article/details/gt2zztvxokl.html

[U97] JS：并发请求
来源：http://www.ydjk.org.cn/Article/details/gt2lzioxgik.html

await Promise.all(urls.map(u => fetch(u)))
来源：http://www.52xcode.cn/Article/details/gt2etomddhd.html

[U98] JS：fetch 带 JSON
来源：http://www.ydjk.org.cn/Article/details/gt2asbxiosr.html

await fetch(url, { method: "POST", headers: { "Content-Type": "application/json" }, body: JSON.stringify(d) })
来源：http://www.52xcode.cn/Article/details/gt2xhikzgvx.html

[U99] JS：事件监听
来源：http://www.ydjk.org.cn/Article/details/gt2qwarolun.html

el.addEventListener("click", e => {})
来源：http://www.ydjk.org.cn/Article/details/gt2eovzddbj.html

[U100] JS：DOM 查询
来源：http://www.52xcode.cn/Article/details/gt2lylxyciu.html

document.querySelector(".item")
来源：http://www.52xcode.cn/Article/details/gt2zwhnelzj.html

[U101] JS：classList 操作
来源：http://www.ydjk.org.cn/Article/details/gt2kgtnoxhg.html

el.classList.toggle("active")
来源：http://www.ydjk.org.cn/Article/details/gt2bvwuatvh.html

[U102] JS：本地存储
来源：http://www.52xcode.cn/Article/details/gt2mbelbtzc.html

localStorage.setItem("k", JSON.stringify(v))
来源：http://www.ydjk.org.cn/Article/details/gt2lwppfjjp.html

[U103] JS：定时器
来源：http://www.52xcode.cn/Article/details/gt2uqmhnbya.html

setTimeout(fn, 1000);  setInterval(fn, 1000);
来源：http://www.52xcode.cn/Article/details/gt2xwhjfcto.html

[U104] JS：防抖
来源：http://www.52xcode.cn/Article/details/gt2kcmdzufn.html

const debounce = (fn, ms) => { let t; return (...a) => { clearTimeout(t); t = setTimeout(() => fn(...a), ms); }; };
来源：http://www.ydjk.org.cn/Article/details/gt2lkeajawr.html

[U105] JS：节流
来源：http://www.52xcode.cn/Article/details/gt2tjwmmypo.html

const throttle = (fn, ms) => { let last = 0; return (...a) => { const n = Date.now(); if (n - last >= ms) { last = n; fn(...a); } }; };
来源：http://www.ydjk.org.cn/Article/details/gt2dsfmmtky.html

[U106] JS：日期格式化
来源：http://www.ydjk.org.cn/Article/details/gt2yttqbjjo.html

new Intl.DateTimeFormat("zh-CN", { dateStyle: "medium" }).format(new Date())
来源：http://www.ydjk.org.cn/Article/details/gt2zptgkgqi.html

[U107] JS：数字千分位
来源：http://www.ydjk.org.cn/Article/details/gt2kklpgzal.html

new Intl.NumberFormat("en-US").format(1234567)
来源：http://www.ydjk.org.cn/Article/details/gt2kivyqift.html

[U108] JS：随机整数
来源：http://www.52xcode.cn/Article/details/gt2etgrshzc.html

Math.floor(Math.random() * (max - min + 1)) + min
来源：http://www.52xcode.cn/Article/details/gt2wzdvwxkc.html

[U109] JS：数组分组
来源：http://www.52xcode.cn/Article/details/gt2mcqdsdde.html

Object.groupBy(arr, x => x.type)
来源：http://www.52xcode.cn/Article/details/gt2afqdngsb.html

[U110] JS：数组分块
来源：http://www.52xcode.cn/Article/details/gt2alefbara.html

arr.reduce((acc, x, i) => (i % size ? acc : [...acc, arr.slice(i, i + size)]), [])
来源：http://www.ydjk.org.cn/Article/details/gt2bfdtvzqb.html

[U111] JS：对象转 Map
来源：http://www.52xcode.cn/Article/details/gt2yhaosqyg.html

new Map(Object.entries(obj))
来源：http://www.ydjk.org.cn/Article/details/gt2reovrrti.html

[U112] JS：字符串补位
来源：http://www.52xcode.cn/Article/details/gt2vkgluexh.html

"7".padStart(3, "0")
来源：http://www.ydjk.org.cn/Article/details/gt2hdvqsnmk.html

[U113] JS：正则替换全部
来源：http://www.52xcode.cn/Article/details/gt2utwonmyv.html

s.replaceAll("a", "b")
来源：http://www.52xcode.cn/Article/details/gt2ogvuquju.html

[U114] JS：JSON 深比较
来源：http://www.ydjk.org.cn/Article/details/gt2uwgtmciq.html

JSON.stringify(a) === JSON.stringify(b)
来源：http://www.ydjk.org.cn/Article/details/gt2aciwnosu.html

[U115] JS：生成 UUID
来源：http://www.52xcode.cn/Article/details/gt2nkwavnfe.html

crypto.randomUUID()
来源：http://www.52xcode.cn/Article/details/gt2scckfwzi.html

[U116] JS：类型检查（JSDoc）
来源：http://www.52xcode.cn/Article/details/gt2pmuayamw.html

/** @param {string} name */ function f(name) {}
来源：http://www.ydjk.org.cn/Article/details/gt2hgsrkhug.html

[U117] JS：单元测试
来源：http://www.ydjk.org.cn/Article/details/gt2mbnitbgw.html

npm i -D vitest;  npx vitest
来源：http://www.ydjk.org.cn/Article/details/gt2qigoyndb.html

[U118] JS：开发服务器
来源：http://www.ydjk.org.cn/Article/details/gt2wmlgnwee.html

npm i -D vite;  npx vite
来源：http://www.52xcode.cn/Article/details/gt2nzvqosxq.html

[U119] JS：生产构建
来源：http://www.52xcode.cn/Article/details/gt2tehyigjj.html

npx vite build
来源：http://www.52xcode.cn/Article/details/gt2daziubko.html

[U120] JS：读取环境变量（Vite）
来源：http://www.52xcode.cn/Article/details/gt2fixyyqra.html

import.meta.env.VITE_API_URL
来源：http://www.ydjk.org.cn/Article/details/gt2pyceoisn.html

================================================================================
来源：http://www.ydjk.org.cn/Article/details/gt2xrjmvqdv.html

统计汇总
来源：http://www.ydjk.org.cn/Article/details/gt2kswcqgaz.html

================================================================================
来源：http://www.ydjk.org.cn/Article/details/gt2jywaviui.html

按语言统计（条）：
来源：http://www.52xcode.cn/Article/details/gt2fzbdghdh.html

Python ......... 252
来源：http://www.ydjk.org.cn/Article/details/gt2duvazdwq.html

PHP ............ 252
来源：http://www.52xcode.cn/Article/details/gt2jcwkdjue.html

JavaScript ..... 252
来源：http://www.52xcode.cn/Article/details/gt2ppconnnq.html

TypeScript ..... 212
来源：http://www.52xcode.cn/Article/details/gt2hbhwypzw.html

Java ........... 212
来源：http://www.52xcode.cn/Article/details/gt2wxdihmkh.html

Go ............. 212
来源：http://www.ydjk.org.cn/Article/details/gt2gaqmejqr.html

Ruby ........... 212
来源：http://www.52xcode.cn/Article/details/gt2dszsgtgz.html

C# ............. 212
来源：http://www.ydjk.org.cn/Article/details/gt2qyzzozpz.html

C .............. 30
来源：http://www.52xcode.cn/Article/details/gt2kuhstrcw.html

C++ ............ 30
来源：http://www.ydjk.org.cn/Article/details/gt2stqwmrhk.html

SQL ............ 90
来源：http://www.ydjk.org.cn/Article/details/gt2fsbvajpe.html

Bash ........... 80
来源：http://www.52xcode.cn/Article/details/gt2bskxnomn.html

Kotlin ......... 15
来源：http://www.ydjk.org.cn/Article/details/gt2irebvhai.html

Swift .......... 15
来源：http://www.52xcode.cn/Article/details/gt2aryolyts.html

Lua ............ 10
来源：http://www.52xcode.cn/Article/details/gt2ctqdakek.html

Perl ........... 10
来源：http://www.52xcode.cn/Article/details/gt2vkmuwmrr.html

Scala .......... 10
来源：http://www.ydjk.org.cn/Article/details/gt2ewtwskxp.html

------------------------------------
来源：http://www.ydjk.org.cn/Article/details/gt2avicfarl.html

合计 ........... 2106 条
来源：http://www.52xcode.cn/Article/details/gt2jhfovcrx.html

按章节统计：
来源：http://www.52xcode.cn/Article/details/gt2ukhakyhh.html

A 基础语法与类型       26 个任务 × 8 语言 =  208
来源：http://www.ydjk.org.cn/Article/details/gt2fcpalpij.html

B 流程控制             16 个任务 × 8 语言 =  128
来源：http://www.ydjk.org.cn/Article/details/gt2tcryhtng.html

C 函数与作用域         16 个任务 × 8 语言 =  128
来源：http://www.ydjk.org.cn/Article/details/gt2qextpxnk.html

D 数组 / 列表 / 集合   26 个任务 × 8 语言 =  208
来源：http://www.ydjk.org.cn/Article/details/gt2fpampiuj.html

E 字符串处理           22 个任务 × 8 语言 =  176
来源：http://www.52xcode.cn/Article/details/gt2natrghfp.html

F 文件与目录           12 个任务 × 8 语言 =   96
来源：http://www.ydjk.org.cn/Article/details/gt2wevvcena.html

G 面向对象             16 个任务 × 8 语言 =  128
来源：http://www.ydjk.org.cn/Article/details/gt2xelnasot.html

H 异常与错误处理       10 个任务 × 8 语言 =   80
来源：http://www.52xcode.cn/Article/details/gt2hckmgiyv.html

I 正则表达式            8 个任务 × 8 语言 =   64
来源：http://www.52xcode.cn/Article/details/gt2wtldixic.html

J 日期与时间           10 个任务 × 8 语言 =   80
来源：http://www.ydjk.org.cn/Article/details/gt2lybxakta.html

K JSON 与序列化         8 个任务 × 8 语言 =   64
来源：http://www.52xcode.cn/Article/details/gt2rsgzadgw.html

L 网络请求              8 个任务 × 8 语言 =   64
来源：http://www.52xcode.cn/Article/details/gt2bglkbwfz.html

M 命令行 / 进程         8 个任务 × 8 语言 =   64
来源：http://www.52xcode.cn/Article/details/gt2fzaklsgo.html

N 数据结构与算法       12 个任务 × 8 语言 =   96
来源：http://www.ydjk.org.cn/Article/details/gt2lmpkilph.html

O 并发与异步            6 个任务 × 8 语言 =   48
来源：http://www.52xcode.cn/Article/details/gt2jifltnuh.html

P 常用工具函数          8 个任务 × 8 语言 =   64
来源：http://www.ydjk.org.cn/Article/details/gt2rjpgxlun.html

Q SQL 专题                              90
来源：http://www.52xcode.cn/Article/details/gt2zqifcelx.html

R Bash 专题                             80
来源：http://www.52xcode.cn/Article/details/gt2vbzljdhy.html

S C / C++ 专题                          60
来源：http://www.52xcode.cn/Article/details/gt2qpignbzx.html

T 其他语言补充                          60
来源：http://www.ydjk.org.cn/Article/details/gt2sjjtxwye.html

U 高频实用片段                         120
来源：http://www.52xcode.cn/Article/details/gt2zqpawkgu.html

------------------------------------
来源：http://www.52xcode.cn/Article/details/gt2pmejxuet.html

合计                                  2106 条
来源：http://www.52xcode.cn/Article/details/gt2kvcglnuh.html

--------------------------------------------------------------------------------
来源：http://www.52xcode.cn/Article/details/gt2acgskhvu.html


<!-- 参考信息 -->