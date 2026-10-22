代发 wailian999

def add(a: Int, b: Int): Int = a + b
来源：http://www.52xcode.cn/Article/details/gt2xlwlayvc.html

[T59] Scala：循环
来源：http://www.52xcode.cn/Article/details/gt2dyhseubd.html

for (i <- 1 to 10) println(i)
来源：http://www.52xcode.cn/Article/details/gt2zllzyxdy.html

[T60] Scala：折叠
来源：http://www.52xcode.cn/Article/details/gt2lcqplari.html

List(1, 2, 3).foldLeft(0)(_ + _)
来源：http://www.ydjk.org.cn/Article/details/gt2hkspefzw.html

================================================================================
来源：http://www.ydjk.org.cn/Article/details/gt2uvszsaeh.html

U. 高频实用片段（Python / PHP / JavaScript 各 40 条）
来源：http://www.52xcode.cn/Article/details/gt2fjsuzsqc.html

================================================================================
来源：http://www.52xcode.cn/Article/details/gt2fbthslbs.html

[U01] Py：创建虚拟环境
来源：http://www.52xcode.cn/Article/details/gt2hrsaolnl.html

python -m venv .venv && source .venv/bin/activate
来源：http://www.52xcode.cn/Article/details/gt2brmfskfa.html

[U02] Py：导出 / 安装依赖
来源：http://www.52xcode.cn/Article/details/gt2mhnfjbjy.html

pip freeze > requirements.txt;  pip install -r requirements.txt
来源：http://www.ydjk.org.cn/Article/details/gt2zzdyivjn.html

[U03] Py：加载 .env 配置
来源：http://www.ydjk.org.cn/Article/details/gt2lgcixcak.html

from dotenv import load_dotenv; load_dotenv()
来源：http://www.52xcode.cn/Article/details/gt2yaanvuec.html

[U04] Py：变量调试打印
来源：http://www.ydjk.org.cn/Article/details/gt2loozfqxg.html

print(f"{x=}")            # 输出 x=值，Python 3.8+
来源：http://www.ydjk.org.cn/Article/details/gt2lqqgkdtq.html

[U05] Py：列表去重且保序
来源：http://www.52xcode.cn/Article/details/gt2qmlyivjr.html

list(dict.fromkeys(arr))
来源：http://www.ydjk.org.cn/Article/details/gt2imxujhzw.html

[U06] Py：合并两个字典
来源：http://www.52xcode.cn/Article/details/gt2kxdmztqc.html

{**a, **b}
来源：http://www.ydjk.org.cn/Article/details/gt2kzqfkprv.html

[U07] Py：反转字典键值
来源：http://www.ydjk.org.cn/Article/details/gt2zkwhnxfa.html

{v: k for k, v in d.items()}
来源：http://www.52xcode.cn/Article/details/gt2exnqrfnh.html

[U08] Py：展平二维列表
来源：http://www.52xcode.cn/Article/details/gt2yorjmkos.html

[y for x in nested for y in x]
来源：http://www.52xcode.cn/Article/details/gt2tgqxkfcr.html

[U09] Py：字典取最大值的键
来源：http://www.52xcode.cn/Article/details/gt2ubrgkhvd.html

max(d, key=d.get)
来源：http://www.52xcode.cn/Article/details/gt2czvlxvoa.html

[U10] Py：按值排序字典
来源：http://www.52xcode.cn/Article/details/gt2epgzjekf.html

dict(sorted(d.items(), key=lambda kv: kv[1]))
来源：http://www.ydjk.org.cn/Article/details/gt2ybuteyln.html

[U11] Py：生成器表达式
来源：http://www.52xcode.cn/Article/details/gt2vvuqjyeb.html

(x * 2 for x in arr)
来源：http://www.ydjk.org.cn/Article/details/gt2xmqjpiby.html

[U12] Py：取出现最多的 3 个元素
来源：http://www.ydjk.org.cn/Article/details/gt2prmwxqqd.html

Counter(arr).most_common(3)
来源：http://www.ydjk.org.cn/Article/details/gt2kkxirqjb.html

[U13] Py：固定长度队列
来源：http://www.52xcode.cn/Article/details/gt2cktxcqvx.html

deque(maxlen=10)
来源：http://www.52xcode.cn/Article/details/gt2qhepmzal.html

[U14] Py：分组收集到列表
来源：http://www.ydjk.org.cn/Article/details/gt2owdvjbpn.html

defaultdict(list)
来源：http://www.ydjk.org.cn/Article/details/gt2szlfngpa.html

[U15] Py：高精度计时
来源：http://www.52xcode.cn/Article/details/gt2tqgfmuiy.html

t = time.perf_counter()
来源：http://www.52xcode.cn/Article/details/gt2koophvgg.html

[U16] Py：命令行参数解析
来源：http://www.52xcode.cn/Article/details/gt2lkxrxegf.html

ap = argparse.ArgumentParser();  ap.add_argument("--name");  args = ap.parse_args()
来源：http://www.52xcode.cn/Article/details/gt2zdxlcqsr.html

[U17] Py：初始化日志
来源：http://www.ydjk.org.cn/Article/details/gt2sdwqknlj.html

logging.basicConfig(level=logging.INFO)
来源：http://www.ydjk.org.cn/Article/details/gt2kmiwgerp.html

[U18] Py：预编译正则
来源：http://www.ydjk.org.cn/Article/details/gt2zdohofvc.html

pat = re.compile(r"\d+")
来源：http://www.ydjk.org.cn/Article/details/gt2tnsajdrn.html

[U19] Py：正则替换带回调
来源：http://www.52xcode.cn/Article/details/gt2sxtadosp.html

re.sub(r"\d+", lambda m: str(int(m.group()) * 2), s)
来源：http://www.52xcode.cn/Article/details/gt2upahhzvk.html

[U20] Py：缓存函数结果
来源：http://www.ydjk.org.cn/Article/details/gt2eqlxvzvl.html

@functools.lru_cache(maxsize=None)
来源：http://www.52xcode.cn/Article/details/gt2gdimfaci.html

[U21] Py：自定义上下文管理器
来源：http://www.52xcode.cn/Article/details/gt2boehxdtc.html

@contextlib.contextmanager
来源：http://www.ydjk.org.cn/Article/details/gt2ytpzeill.html

[U22] Py：矩阵转置
来源：http://www.52xcode.cn/Article/details/gt2fxivnvcy.html

list(zip(*m))
来源：http://www.ydjk.org.cn/Article/details/gt2sovwtkuh.html

[U23] Py：分块读取大文件
来源：http://www.52xcode.cn/Article/details/gt2gbxudjno.html

for chunk in iter(lambda: f.read(8192), b""):
来源：http://www.ydjk.org.cn/Article/details/gt2oxabzzge.html

[U24] Py：路径操作
来源：http://www.52xcode.cn/Article/details/gt2bcsyjmlj.html

Path("a/b.txt").parent.mkdir(parents=True, exist_ok=True)
来源：http://www.ydjk.org.cn/Article/details/gt2yoztulad.html

[U25] Py：CSV 按字典读
来源：http://www.52xcode.cn/Article/details/gt2ubpuxqzn.html

csv.DictReader(f)
来源：http://www.ydjk.org.cn/Article/details/gt2mvtqrcby.html

[U26] Py：并发下载
来源：http://www.ydjk.org.cn/Article/details/gt2mdbqtloi.html

ThreadPoolExecutor(max_workers=8).map(fetch, urls)
来源：http://www.ydjk.org.cn/Article/details/gt2ptuakahc.html

[U27] Py：异步 HTTP
来源：http://www.ydjk.org.cn/Article/details/gt2jhdafvej.html

aiohttp.ClientSession() 配合 async with
来源：http://www.ydjk.org.cn/Article/details/gt2omwnovrw.html

[U28] Py：类型别名
来源：http://www.ydjk.org.cn/Article/details/gt2ksqbxpui.html

UserId = int
来源：http://www.ydjk.org.cn/Article/details/gt2jxdyndli.html

[U29] Py：属性校验
来源：http://www.52xcode.cn/Article/details/gt2ttkieuaz.html

@property 与 @x.setter 配合
来源：http://www.52xcode.cn/Article/details/gt2nusvcnfc.html

[U30] Py：数据类
来源：http://www.ydjk.org.cn/Article/details/gt2vhjcejaa.html

@dataclass(slots=True)
来源：http://www.52xcode.cn/Article/details/gt2cgsfchol.html

[U31] Py：单测
来源：http://www.ydjk.org.cn/Article/details/gt2xpuhlqri.html

python -m pytest -q
来源：http://www.ydjk.org.cn/Article/details/gt2juilfxps.html

[U32] Py：代码格式化
来源：http://www.52xcode.cn/Article/details/gt2fsvvelub.html

ruff format . && ruff check --fix .
来源：http://www.52xcode.cn/Article/details/gt2iadwxkmt.html

[U33] Py：打包发布
来源：http://www.ydjk.org.cn/Article/details/gt2mmpzwnjk.html

python -m build  （依赖 pyproject.toml）
来源：http://www.ydjk.org.cn/Article/details/gt2djgqkuvm.html

[U34] Py：判断编码
来源：http://www.52xcode.cn/Article/details/gt2fwemxbkc.html

chardet.detect(raw)
来源：http://www.52xcode.cn/Article/details/gt2vtbxcfva.html

[U35] Py：发送邮件
来源：http://www.ydjk.org.cn/Article/details/gt2ljufkbhr.html

smtplib.SMTP_SSL(...).send_message(msg)
来源：http://www.ydjk.org.cn/Article/details/gt2objvhrpk.html

[U36] Py：定时任务
来源：http://www.ydjk.org.cn/Article/details/gt2pjsqldvg.html

schedule.every(10).minutes.do(job)
来源：http://www.52xcode.cn/Article/details/gt2tupsbuvq.html

[U37] Py：读写 Excel
来源：http://www.52xcode.cn/Article/details/gt2ynpfwcjh.html

pandas.read_excel / DataFrame.to_excel
来源：http://www.52xcode.cn/Article/details/gt2cflkorfg.html

[U38] Py：获取脚本所在目录
来源：http://www.ydjk.org.cn/Article/details/gt2curaejty.html

Path(__file__).resolve().parent
来源：http://www.52xcode.cn/Article/details/gt2qjxfyyoe.html

[U39] Py：判断是否在交互环境
来源：http://www.52xcode.cn/Article/details/gt2rsnfmmfs.html

sys.stdout.isatty()
来源：http://www.ydjk.org.cn/Article/details/gt2pjgsjvbf.html

[U40] Py：打印到标准错误
来源：http://www.ydjk.org.cn/Article/details/gt2utqotqsx.html

print("err", file=sys.stderr)
来源：http://www.52xcode.cn/Article/details/gt2ltalcfvt.html

[U41] PHP：初始化 Composer 项目
来源：http://www.ydjk.org.cn/Article/details/gt2jddtxejn.html

composer init;  composer require guzzlehttp/guzzle
来源：http://www.ydjk.org.cn/Article/details/gt2lihdayio.html

[U42] PHP：PSR-4 自动加载
来源：http://www.52xcode.cn/Article/details/gt2gxtnlmeo.html

"autoload": { "psr-4": { "App\\": "src/" } }
来源：http://www.ydjk.org.cn/Article/details/gt2kewnonzt.html

[U43] PHP：声明命名空间
来源：http://www.52xcode.cn/Article/details/gt2negydrcd.html

namespace App\Http;
来源：http://www.ydjk.org.cn/Article/details/gt2cjbuwhsq.html

[U44] PHP：开启严格类型
来源：http://www.52xcode.cn/Article/details/gt2orvsbznx.html

declare(strict_types=1);
来源：http://www.52xcode.cn/Article/details/gt2jygeiqlk.html

[U45] PHP：类型声明与返回类型
来源：http://www.52xcode.cn/Article/details/gt2deaggbry.html

function add(int $a, int $b): int { return $a + $b; }
来源：http://www.ydjk.org.cn/Article/details/gt2flyctocc.html

[U46] PHP：可空类型
来源：http://www.52xcode.cn/Article/details/gt2jfkshtiu.html

?string $name = null
来源：http://www.52xcode.cn/Article/details/gt2hxtqlpyt.html

[U47] PHP：联合类型
来源：http://www.ydjk.org.cn/Article/details/gt2jegrwods.html

int|string $id
来源：http://www.ydjk.org.cn/Article/details/gt2itiixnte.html

[U48] PHP：纯枚举
来源：http://www.ydjk.org.cn/Article/details/gt2vioertdo.html

enum Status: string { case Active = "active"; case Off = "off"; }
来源：http://www.52xcode.cn/Article/details/gt2wjyhuvdb.html

[U49] PHP：只读属性
来源：http://www.52xcode.cn/Article/details/gt2vurejlsu.html

public readonly string $name
来源：http://www.ydjk.org.cn/Article/details/gt2lzoxcdbx.html

[U50] PHP：构造器属性提升
来源：http://www.52xcode.cn/Article/details/gt2yjbgqcxu.html

public function __construct(private int $id) {}
来源：http://www.ydjk.org.cn/Article/details/gt2mvzhqrle.html

[U51] PHP：数组解构
来源：http://www.52xcode.cn/Article/details/gt2nbujgybp.html

[$a, $b] = $arr;
来源：http://www.52xcode.cn/Article/details/gt2tcpumzkn.html

[U52] PHP：箭头函数
来源：http://www.ydjk.org.cn/Article/details/gt2uyhvaepj.html

$double = fn($x) => $x * 2;
来源：http://www.ydjk.org.cn/Article/details/gt2ynzdwkdg.html

[U53] PHP：空合并运算符
来源：http://www.52xcode.cn/Article/details/gt2jrksdvjc.html

$v = $a ?? $b ?? "default";
来源：http://www.52xcode.cn/Article/details/gt2ccagizqb.html

[U54] PHP：空安全调用
来源：http://www.ydjk.org.cn/Article/details/gt2ldusqgel.html

$obj?->method()
来源：http://www.ydjk.org.cn/Article/details/gt2bzvvvixk.html

[U55] PHP：match 表达式
来源：http://www.ydjk.org.cn/Article/details/gt2ytefwweu.html

$s = match($x) { 1 => "一", default => "其他" };
来源：http://www.ydjk.org.cn/Article/details/gt2mqufhuzf.html

[U56] PHP：命名参数
来源：http://www.52xcode.cn/Article/details/gt2yaznyvmx.html

f(a: 1, b: 2)
来源：http://www.52xcode.cn/Article/details/gt2lurokmtb.html

[U57] PHP：字符串插值
来源：http://www.52xcode.cn/Article/details/gt2oownwkyb.html

"值: {$a}"
来源：http://www.ydjk.org.cn/Article/details/gt2bikrbfet.html

[U58] PHP：数组三件套
来源：http://www.ydjk.org.cn/Article/details/gt2dmirmmvu.html

array_map($f, $a);  array_filter($a, $f);  array_reduce($a, $f, 0);
来源：http://www.ydjk.org.cn/Article/details/gt2rxvhalcp.html

[U59] PHP：自定义排序
来源：http://www.52xcode.cn/Article/details/gt2jwubzbmc.html

usort($arr, fn($a, $b) => $a["age"] <=> $b["age"]);
来源：http://www.52xcode.cn/Article/details/gt2vtfuguge.html

[U60] PHP：JSON 编解码
来源：http://www.ydjk.org.cn/Article/details/gt2gmtcpemg.html

json_encode($d, JSON_UNESCAPED_UNICODE);  json_decode($s, true);
来源：http://www.ydjk.org.cn/Article/details/gt2sgshopin.html

[U61] PHP：正则
来源：http://www.ydjk.org.cn/Article/details/gt2qquelhfd.html

preg_match('/(\d+)/', $s, $m);  preg_replace('/\d+/', '#', $s);
来源：http://www.ydjk.org.cn/Article/details/gt2ajnjhbum.html

[U62] PHP：日期对象
来源：http://www.52xcode.cn/Article/details/gt2xvtbxcub.html

(new DateTimeImmutable())->format("Y-m-d");
来源：http://www.ydjk.org.cn/Article/details/gt2mqinrjck.html

[U63] PHP：文件读写
来源：http://www.ydjk.org.cn/Article/details/gt2lyrapxbo.html

file_get_contents($f);  file_put_contents($f, $data);
来源：http://www.ydjk.org.cn/Article/details/gt2vufwtils.html

[U64] PHP：目录遍历
来源：http://www.ydjk.org.cn/Article/details/gt2inoratuw.html

glob("dir/*.php");  scandir("dir");
来源：http://www.52xcode.cn/Article/details/gt2stdzzcwa.html

[U65] PHP：会话
来源：http://www.52xcode.cn/Article/details/gt2kjbptsac.html

session_start();  $_SESSION["uid"] = 1;
来源：http://www.52xcode.cn/Article/details/gt2huikodcz.html

[U66] PHP：设置 Cookie
来源：http://www.ydjk.org.cn/Article/details/gt2arxvnquu.html

setcookie("token", $v, ["httponly" => true, "samesite" => "Lax"]);
来源：http://www.ydjk.org.cn/Article/details/gt2mtkcodec.html

[U67] PHP：处理文件上传
来源：http://www.ydjk.org.cn/Article/details/gt2ospngebq.html

$_FILES["file"]["tmp_name"] 与 move_uploaded_file()
来源：http://www.ydjk.org.cn/Article/details/gt2fybjgifp.html

[U68] PHP：PDO 连接
来源：http://www.ydjk.org.cn/Article/details/gt2rpzfufkr.html

$pdo = new PDO("mysql:host=localhost;dbname=app", "root", "");
来源：http://www.52xcode.cn/Article/details/gt2jdqxoddf.html

[U69] PHP：PDO 预处理
来源：http://www.ydjk.org.cn/Article/details/gt2bnrylrow.html

$stmt = $pdo->prepare("SELECT * FROM users WHERE id = ?");  $stmt->execute([$id]);
来源：http://www.52xcode.cn/Article/details/gt2tkfrbmoz.html

[U70] PHP：PDO 事务
来源：http://www.52xcode.cn/Article/details/gt2bbukfadz.html

$pdo->beginTransaction();  $pdo->commit();  $pdo->rollBack();
来源：http://www.ydjk.org.cn/Article/details/gt2bohwrzdl.html

[U71] PHP：抛出异常
来源：http://www.ydjk.org.cn/Article/details/gt2pfleaboq.html

throw new RuntimeException("失败", 500);
来源：http://www.52xcode.cn/Article/details/gt2uebhhjru.html

[U72] PHP：写错误日志
来源：http://www.52xcode.cn/Article/details/gt2mnzchbiy.html

error_log("失败: " . $e->getMessage());
来源：http://www.52xcode.cn/Article/details/gt2dejjaowx.html

[U73] PHP：读取 ini 配置
来源：http://www.ydjk.org.cn/Article/details/gt2mlsikqvx.html

parse_ini_file("config.ini", true)
来源：http://www.ydjk.org.cn/Article/details/gt2dxdpalbs.html

[U74] PHP：读取环境变量
来源：http://www.52xcode.cn/Article/details/gt2qvnvnqbs.html

getenv("APP_ENV") ?: "production"
来源：http://www.52xcode.cn/Article/details/gt2thdafzfx.html

[U75] PHP：依赖注入
来源：http://www.52xcode.cn/Article/details/gt2zdaqtncl.html

composer require psr/container
来源：http://www.ydjk.org.cn/Article/details/gt2gjtgpeqq.html

[U76] PHP：简单路由
来源：http://www.ydjk.org.cn/Article/details/gt2ulmbskns.html

$path = parse_url($_SERVER["REQUEST_URI"], PHP_URL_PATH);
来源：http://www.52xcode.cn/Article/details/gt2aqxermyc.html

[U77] PHP：模板渲染
来源：http://www.52xcode.cn/Article/details/gt2xnrwkslt.html

composer require twig/twig
来源：http://www.ydjk.org.cn/Article/details/gt2xtjtdqpo.html

[U78] PHP：单元测试
来源：http://www.ydjk.org.cn/Article/details/gt2nmasoczu.html

composer require --dev phpunit/phpunit
来源：http://www.52xcode.cn/Article/details/gt2uibflbjz.html

[U79] PHP：静态分析
来源：http://www.52xcode.cn/Article/details/gt2zcpkrlcj.html

composer require --dev phpstan/phpstan
来源：http://www.52xcode.cn/Article/details/gt2wdsigira.html

[U80] PHP：代码规范修复
来源：http://www.ydjk.org.cn/Article/details/gt2flcobcii.html

composer require --dev friendsofphp/php-cs-fixer
来源：http://www.ydjk.org.cn/Article/details/gt2abagqvxm.html

[U81] JS：初始化项目
来源：http://www.52xcode.cn/Article/details/gt2lnvrvxwu.html

npm init -y;  npm i express
来源：http://www.ydjk.org.cn/Article/details/gt2prphszte.html

[U82] JS：package.json 脚本
来源：http://www.ydjk.org.cn/Article/details/gt2dypprcpl.html

"scripts": { "dev": "vite", "build": "vite build" }
来源：http://www.ydjk.org.cn/Article/details/gt2xuvbcuvu.html

[U83] JS：ES Module 导入导出
来源：http://www.52xcode.cn/Article/details/gt2wefzhqds.html

export const a = 1;  import { a } from "./m.js";
来源：http://www.52xcode.cn/Article/details/gt2lbitoqcm.html

[U84] JS：CommonJS 写法
来源：http://www.52xcode.cn/Article/details/gt2gwlqwxha.html

module.exports = { a };  const { a } = require("./m");
来源：http://www.52xcode.cn/Article/details/gt2apikhcci.html

[U85] JS：可选链
来源：http://www.ydjk.org.cn/Article/details/gt2kyubacfp.html

a?.b?.c
来源：http://www.ydjk.org.cn/Article/details/gt2uboqgtxc.html

[U86] JS：空值合并
来源：http://www.52xcode.cn/Article/details/gt2pvsoyret.html

a ?? b
来源：http://www.ydjk.org.cn/Article/details/gt2uyfgzbst.html

[U87] JS：解构默认值
来源：http://www.ydjk.org.cn/Article/details/gt2ywicdhdg.html

const { a = 1, b = 2 } = obj;
来源：http://www.ydjk.org.cn/Article/details/gt2gftlyrof.html

[U88] JS：对象展开合并
来源：http://www.ydjk.org.cn/Article/details/gt2eatolgbi.html

{ ...a, ...b }
来源：http://www.52xcode.cn/Article/details/gt2efrouboj.html

[U89] JS：数组去重
来源：http://www.52xcode.cn/Article/details/gt2wpihciom.html

[...new Set(arr)]
来源：http://www.ydjk.org.cn/Article/details/gt2ijeauvsw.html

[U90] JS：数字数组排序
来源：http://www.ydjk.org.cn/Article/details/gt2xeaxhkkw.html

[...arr].sort((a, b) => a - b)
来源：http://www.52xcode.cn/Article/details/gt2podvdyig.html

[U91] JS：对象键值遍历
来源：http://www.ydjk.org.cn/Article/details/gt2hkkxgexd.html

Object.entries(obj).forEach(([k, v]) => {});
来源：http://www.ydjk.org.cn/Article/details/gt2ojwqumrk.html

[U92] JS：深拷贝
来源：http://www.ydjk.org.cn/Article/details/gt2zipoosqh.html

structuredClone(obj)
来源：http://www.ydjk.org.cn/Article/details/gt2bnngdmyi.html

[U93] JS：模板字符串
来源：http://www.ydjk.org.cn/Article/details/gt2mulxzxwa.html

`共 ${n} 条`
来源：http://www.ydjk.org.cn/Article/details/gt2ycbxqdzw.html

[U94] JS：箭头函数
来源：http://www.ydjk.org.cn/Article/details/gt2zhefeiii.html

const double = x => x * 2;
来源：http://www.ydjk.org.cn/Article/details/gt2pdbkcemy.html

[U95] JS：Promise 包装
来源：http://www.52xcode.cn/Article/details/gt2xiwopoqu.html

new Promise((resolve, reject) => {})
来源：http://www.ydjk.org.cn/Article/details/gt2brgbcztp.html

[U96] JS：async/await 与异常
来源：http://www.ydjk.org.cn/Article/details/gt2eocdfzhq.html

try { const d = await f(); } catch (e) { console.error(e); }
来源：http://www.ydjk.org.cn/Article/details/gt2ubpbzyxz.html

[U97] JS：并发请求
来源：http://www.ydjk.org.cn/Article/details/gt2jvcjxpit.html

await Promise.all(urls.map(u => fetch(u)))
来源：http://www.ydjk.org.cn/Article/details/gt2gfmoikqg.html

[U98] JS：fetch 带 JSON
来源：http://www.ydjk.org.cn/Article/details/gt2fekypvnl.html

await fetch(url, { method: "POST", headers: { "Content-Type": "application/json" }, body: JSON.stringify(d) })
来源：http://www.52xcode.cn/Article/details/gt2jbwnwhav.html

[U99] JS：事件监听
来源：http://www.52xcode.cn/Article/details/gt2htomuhuh.html

el.addEventListener("click", e => {})
来源：http://www.ydjk.org.cn/Article/details/gt2mcdezwws.html

[U100] JS：DOM 查询
来源：http://www.ydjk.org.cn/Article/details/gt2cqxqygwp.html

document.querySelector(".item")
来源：http://www.ydjk.org.cn/Article/details/gt2oogtyjhg.html

[U101] JS：classList 操作
来源：http://www.ydjk.org.cn/Article/details/gt2szotxiyb.html

el.classList.toggle("active")
来源：http://www.52xcode.cn/Article/details/gt2rjtmazex.html

[U102] JS：本地存储
来源：http://www.52xcode.cn/Article/details/gt2apddrnhc.html

localStorage.setItem("k", JSON.stringify(v))
来源：http://www.52xcode.cn/Article/details/gt2eglhdysp.html

[U103] JS：定时器
来源：http://www.52xcode.cn/Article/details/gt2qmvvjtya.html

setTimeout(fn, 1000);  setInterval(fn, 1000);
来源：http://www.ydjk.org.cn/Article/details/gt2hwkjxqku.html

[U104] JS：防抖
来源：http://www.52xcode.cn/Article/details/gt2lkjsxwpy.html

const debounce = (fn, ms) => { let t; return (...a) => { clearTimeout(t); t = setTimeout(() => fn(...a), ms); }; };
来源：http://www.ydjk.org.cn/Article/details/gt2fprmasxc.html

[U105] JS：节流
来源：http://www.ydjk.org.cn/Article/details/gt2pcblenip.html

const throttle = (fn, ms) => { let last = 0; return (...a) => { const n = Date.now(); if (n - last >= ms) { last = n; fn(...a); } }; };
来源：http://www.ydjk.org.cn/Article/details/gt2rhnvcuoy.html

[U106] JS：日期格式化
来源：http://www.ydjk.org.cn/Article/details/gt2byfarofs.html

new Intl.DateTimeFormat("zh-CN", { dateStyle: "medium" }).format(new Date())
来源：http://www.52xcode.cn/Article/details/gt2yzymaajg.html

[U107] JS：数字千分位
来源：http://www.ydjk.org.cn/Article/details/gt2mfkjpvwk.html

new Intl.NumberFormat("en-US").format(1234567)
来源：http://www.52xcode.cn/Article/details/gt2osdsaqeu.html

[U108] JS：随机整数
来源：http://www.ydjk.org.cn/Article/details/gt2fttfgdce.html

Math.floor(Math.random() * (max - min + 1)) + min
来源：http://www.52xcode.cn/Article/details/gt2uxanblix.html

[U109] JS：数组分组
来源：http://www.52xcode.cn/Article/details/gt2bztkdmxl.html

Object.groupBy(arr, x => x.type)
来源：http://www.52xcode.cn/Article/details/gt2xyycitqr.html

[U110] JS：数组分块
来源：http://www.ydjk.org.cn/Article/details/gt2wwbocwkf.html

arr.reduce((acc, x, i) => (i % size ? acc : [...acc, arr.slice(i, i + size)]), [])
来源：http://www.52xcode.cn/Article/details/gt2zdjbqcph.html

[U111] JS：对象转 Map
来源：http://www.52xcode.cn/Article/details/gt2pursnywo.html

new Map(Object.entries(obj))
来源：http://www.ydjk.org.cn/Article/details/gt2jmvetpnv.html

[U112] JS：字符串补位
来源：http://www.ydjk.org.cn/Article/details/gt2xmegqryj.html

"7".padStart(3, "0")
来源：http://www.ydjk.org.cn/Article/details/gt2fuztinba.html

[U113] JS：正则替换全部
来源：http://www.ydjk.org.cn/Article/details/gt2ehjahdxm.html

s.replaceAll("a", "b")
来源：http://www.52xcode.cn/Article/details/gt2baxskzmw.html

[U114] JS：JSON 深比较
来源：http://www.ydjk.org.cn/Article/details/gt2sdmlmujq.html

JSON.stringify(a) === JSON.stringify(b)
来源：http://www.52xcode.cn/Article/details/gt2ayzuupfc.html

[U115] JS：生成 UUID
来源：http://www.ydjk.org.cn/Article/details/gt2nxfomohb.html

crypto.randomUUID()
来源：http://www.52xcode.cn/Article/details/gt2lilumnpz.html

[U116] JS：类型检查（JSDoc）
来源：http://www.ydjk.org.cn/Article/details/gt2tawgjuds.html

/** @param {string} name */ function f(name) {}
来源：http://www.52xcode.cn/Article/details/gt2okariwqa.html

[U117] JS：单元测试
来源：http://www.ydjk.org.cn/Article/details/gt2bwchllvl.html

npm i -D vitest;  npx vitest
来源：http://www.ydjk.org.cn/Article/details/gt2thrqytzs.html

[U118] JS：开发服务器
来源：http://www.ydjk.org.cn/Article/details/gt2mqdggkdu.html

npm i -D vite;  npx vite
来源：http://www.52xcode.cn/Article/details/gt2quryzyui.html

[U119] JS：生产构建
来源：http://www.ydjk.org.cn/Article/details/gt2xfefmrqb.html

npx vite build
来源：http://www.52xcode.cn/Article/details/gt2hoogmnxh.html

[U120] JS：读取环境变量（Vite）
来源：http://www.52xcode.cn/Article/details/gt2gzjufqjd.html

import.meta.env.VITE_API_URL
来源：http://www.ydjk.org.cn/Article/details/gt2kszpvfck.html

================================================================================
来源：http://www.ydjk.org.cn/Article/details/gt2defnqlto.html

统计汇总
来源：http://www.52xcode.cn/Article/details/gt2stdxqnpi.html

================================================================================
来源：http://www.ydjk.org.cn/Article/details/gt2klkxjqcc.html

按语言统计（条）：
来源：http://www.ydjk.org.cn/Article/details/gt2yvyosmgx.html

Python ......... 252
来源：http://www.52xcode.cn/Article/details/gt2vvrwksnf.html

PHP ............ 252
来源：http://www.52xcode.cn/Article/details/gt2hqsjwrmz.html

JavaScript ..... 252
来源：http://www.52xcode.cn/Article/details/gt2awleznkg.html

TypeScript ..... 212
来源：http://www.52xcode.cn/Article/details/gt2gxgazvlw.html

Java ........... 212
来源：http://www.52xcode.cn/Article/details/gt2huvpudgo.html

Go ............. 212
来源：http://www.52xcode.cn/Article/details/gt2udbgzhtg.html

Ruby ........... 212
来源：http://www.52xcode.cn/Article/details/gt2aarlghce.html

C# ............. 212
来源：http://www.52xcode.cn/Article/details/gt2gochyvpg.html

C .............. 30
来源：http://www.52xcode.cn/Article/details/gt2uuopftla.html

C++ ............ 30
来源：http://www.52xcode.cn/Article/details/gt2rkagghrs.html

SQL ............ 90
来源：http://www.52xcode.cn/Article/details/gt2fxwrmogc.html

Bash ........... 80
来源：http://www.ydjk.org.cn/Article/details/gt2rguaoekv.html

Kotlin ......... 15
来源：http://www.ydjk.org.cn/Article/details/gt2fonjqpzj.html

Swift .......... 15
来源：http://www.ydjk.org.cn/Article/details/gt2jdayrfvf.html

Lua ............ 10
来源：http://www.ydjk.org.cn/Article/details/gt2bdkzhdvh.html

Perl ........... 10
来源：http://www.52xcode.cn/Article/details/gt2qnkiykni.html

Scala .......... 10
来源：http://www.ydjk.org.cn/Article/details/gt2fpvdezco.html

------------------------------------
来源：http://www.52xcode.cn/Article/details/gt2hbhvfcbj.html

合计 ........... 2106 条
来源：http://www.52xcode.cn/Article/details/gt2udaytzhc.html

按章节统计：
来源：http://www.52xcode.cn/Article/details/gt2vywnedwh.html

A 基础语法与类型       26 个任务 × 8 语言 =  208
来源：http://www.ydjk.org.cn/Article/details/gt2njvfvbek.html

B 流程控制             16 个任务 × 8 语言 =  128
来源：http://www.ydjk.org.cn/Article/details/gt2htzxxkkx.html

C 函数与作用域         16 个任务 × 8 语言 =  128
来源：http://www.ydjk.org.cn/Article/details/gt2ympsmzbt.html

D 数组 / 列表 / 集合   26 个任务 × 8 语言 =  208
来源：http://www.52xcode.cn/Article/details/gt2kyatpnja.html

E 字符串处理           22 个任务 × 8 语言 =  176
来源：http://www.52xcode.cn/Article/details/gt2wyjsvyqe.html

F 文件与目录           12 个任务 × 8 语言 =   96
来源：http://www.ydjk.org.cn/Article/details/gt2alztaczd.html

G 面向对象             16 个任务 × 8 语言 =  128
来源：http://www.52xcode.cn/Article/details/gt2jhccgitd.html

H 异常与错误处理       10 个任务 × 8 语言 =   80
来源：http://www.ydjk.org.cn/Article/details/gt2efbgbdbq.html

I 正则表达式            8 个任务 × 8 语言 =   64
来源：http://www.52xcode.cn/Article/details/gt2ynomeace.html

J 日期与时间           10 个任务 × 8 语言 =   80
来源：http://www.52xcode.cn/Article/details/gt2xnvtyacq.html

K JSON 与序列化         8 个任务 × 8 语言 =   64
来源：http://www.ydjk.org.cn/Article/details/gt2gdnfhykk.html

L 网络请求              8 个任务 × 8 语言 =   64
来源：http://www.52xcode.cn/Article/details/gt2qdpflvtn.html

M 命令行 / 进程         8 个任务 × 8 语言 =   64
来源：http://www.52xcode.cn/Article/details/gt2hcstixtq.html

N 数据结构与算法       12 个任务 × 8 语言 =   96
来源：http://www.52xcode.cn/Article/details/gt2jltzqgvd.html

O 并发与异步            6 个任务 × 8 语言 =   48
来源：http://www.52xcode.cn/Article/details/gt2jbxwgllb.html

P 常用工具函数          8 个任务 × 8 语言 =   64
来源：http://www.ydjk.org.cn/Article/details/gt2tahvkdmf.html

Q SQL 专题                              90
来源：http://www.ydjk.org.cn/Article/details/gt2qtyfneyb.html

R Bash 专题                             80
来源：http://www.52xcode.cn/Article/details/gt2qwgelakm.html

S C / C++ 专题                          60
来源：http://www.ydjk.org.cn/Article/details/gt2aqhyjhri.html

T 其他语言补充                          60
来源：http://www.ydjk.org.cn/Article/details/gt2zlcajdmj.html

U 高频实用片段                         120
来源：http://www.52xcode.cn/Article/details/gt2myvnclwi.html

------------------------------------
来源：http://www.52xcode.cn/Article/details/gt2rulrrtep.html

合计                                  2106 条
来源：http://www.ydjk.org.cn/Article/details/gt2fxtdjyba.html

--------------------------------------------------------------------------------
来源：http://www.ydjk.org.cn/Article/details/gt2rdtwkgab.html

使用提醒
来源：http://www.ydjk.org.cn/Article/details/gt2ejvbnyqj.html

--------------------------------------------------------------------------------
来源：http://www.ydjk.org.cn/Article/details/gt2lnnfsjvp.html

1. 示例追求"最小可用"，正式项目中请补齐导入、错误处理与边界判断。
来源：http://www.ydjk.org.cn/Article/details/gt2qxxvtesw.html

2. 涉及文件、网络、数据库的示例，注意资源释放与异常捕获。
来源：http://www.52xcode.cn/Article/details/gt2kpdzjgnd.html


<!-- 参考信息 -->