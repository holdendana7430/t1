代发 wailian999

def add(a: Int, b: Int): Int = a + b
来源：http://www.ydjk.org.cn/Article/details/gt3hrqelnku.html

[T59] Scala：循环
来源：http://www.ydjk.org.cn/Article/details/gt3rfmpkymd.html

for (i <- 1 to 10) println(i)
来源：http://www.ydjk.org.cn/Article/details/gt3ummwuobb.html

[T60] Scala：折叠
来源：http://www.ydjk.org.cn/Article/details/gt3yocufdsd.html

List(1, 2, 3).foldLeft(0)(_ + _)
来源：http://www.52xcode.cn/Article/details/gt3ocmueqjt.html

================================================================================
来源：http://www.ydjk.org.cn/Article/details/gt3guyekogu.html

U. 高频实用片段（Python / PHP / JavaScript 各 40 条）
来源：http://www.ydjk.org.cn/Article/details/gt3hrnqvovp.html

================================================================================
来源：http://www.ydjk.org.cn/Article/details/gt3gbtwtmfl.html

[U01] Py：创建虚拟环境
来源：http://www.ydjk.org.cn/Article/details/gt3cgphyhsj.html

python -m venv .venv && source .venv/bin/activate
来源：http://www.52xcode.cn/Article/details/gt3qpkfifav.html

[U02] Py：导出 / 安装依赖
来源：http://www.52xcode.cn/Article/details/gt3tnpbtuxl.html

pip freeze > requirements.txt;  pip install -r requirements.txt
来源：http://www.52xcode.cn/Article/details/gt3cbimiysc.html

[U03] Py：加载 .env 配置
来源：http://www.52xcode.cn/Article/details/gt3dqwzdfms.html

from dotenv import load_dotenv; load_dotenv()
来源：http://www.52xcode.cn/Article/details/gt3zjaxmtlj.html

[U04] Py：变量调试打印
来源：http://www.ydjk.org.cn/Article/details/gt3sjwrovbc.html

print(f"{x=}")            # 输出 x=值，Python 3.8+
来源：http://www.ydjk.org.cn/Article/details/gt3iphaaxot.html

[U05] Py：列表去重且保序
来源：http://www.52xcode.cn/Article/details/gt3ikgijvzt.html

list(dict.fromkeys(arr))
来源：http://www.52xcode.cn/Article/details/gt3vuwbgueh.html

[U06] Py：合并两个字典
来源：http://www.52xcode.cn/Article/details/gt3emqgqile.html

{**a, **b}
来源：http://www.ydjk.org.cn/Article/details/gt3mvpystoa.html

[U07] Py：反转字典键值
来源：http://www.52xcode.cn/Article/details/gt3wmkmdlqk.html

{v: k for k, v in d.items()}
来源：http://www.ydjk.org.cn/Article/details/gt3iwxamkwp.html

[U08] Py：展平二维列表
来源：http://www.ydjk.org.cn/Article/details/gt3hohnhept.html

[y for x in nested for y in x]
来源：http://www.52xcode.cn/Article/details/gt3lhmfwkhv.html

[U09] Py：字典取最大值的键
来源：http://www.ydjk.org.cn/Article/details/gt3luvxfiky.html

max(d, key=d.get)
来源：http://www.ydjk.org.cn/Article/details/gt3yotepnlq.html

[U10] Py：按值排序字典
来源：http://www.52xcode.cn/Article/details/gt3ufcohpzj.html

dict(sorted(d.items(), key=lambda kv: kv[1]))
来源：http://www.52xcode.cn/Article/details/gt3anggqenw.html

[U11] Py：生成器表达式
来源：http://www.52xcode.cn/Article/details/gt3dliyuuyw.html

(x * 2 for x in arr)
来源：http://www.ydjk.org.cn/Article/details/gt3lnpihppo.html

[U12] Py：取出现最多的 3 个元素
来源：http://www.ydjk.org.cn/Article/details/gt3agwufjiu.html

Counter(arr).most_common(3)
来源：http://www.52xcode.cn/Article/details/gt3yhbvnidc.html

[U13] Py：固定长度队列
来源：http://www.52xcode.cn/Article/details/gt3nagiharo.html

deque(maxlen=10)
来源：http://www.52xcode.cn/Article/details/gt3phkllpkm.html

[U14] Py：分组收集到列表
来源：http://www.52xcode.cn/Article/details/gt3boiscocj.html

defaultdict(list)
来源：http://www.ydjk.org.cn/Article/details/gt3irjxierd.html

[U15] Py：高精度计时
来源：http://www.52xcode.cn/Article/details/gt3ubrfidnr.html

t = time.perf_counter()
来源：http://www.ydjk.org.cn/Article/details/gt3ghtuawlb.html

[U16] Py：命令行参数解析
来源：http://www.52xcode.cn/Article/details/gt3qjjbuqfl.html

ap = argparse.ArgumentParser();  ap.add_argument("--name");  args = ap.parse_args()
来源：http://www.52xcode.cn/Article/details/gt3eqwmjkwg.html

[U17] Py：初始化日志
来源：http://www.52xcode.cn/Article/details/gt3yvgavdkc.html

logging.basicConfig(level=logging.INFO)
来源：http://www.ydjk.org.cn/Article/details/gt3kddqtxxd.html

[U18] Py：预编译正则
来源：http://www.52xcode.cn/Article/details/gt3kwwsaqkh.html

pat = re.compile(r"\d+")
来源：http://www.ydjk.org.cn/Article/details/gt3lbswdwgw.html

[U19] Py：正则替换带回调
来源：http://www.ydjk.org.cn/Article/details/gt3mxgpjqgn.html

re.sub(r"\d+", lambda m: str(int(m.group()) * 2), s)
来源：http://www.52xcode.cn/Article/details/gt3zmwmocmm.html

[U20] Py：缓存函数结果
来源：http://www.52xcode.cn/Article/details/gt3rpomosno.html

@functools.lru_cache(maxsize=None)
来源：http://www.52xcode.cn/Article/details/gt3gcrjcrhq.html

[U21] Py：自定义上下文管理器
来源：http://www.ydjk.org.cn/Article/details/gt3xxfowllm.html

@contextlib.contextmanager
来源：http://www.52xcode.cn/Article/details/gt3qcxhrnav.html

[U22] Py：矩阵转置
来源：http://www.ydjk.org.cn/Article/details/gt3meemjwwj.html

list(zip(*m))
来源：http://www.ydjk.org.cn/Article/details/gt3kgrnoxfd.html

[U23] Py：分块读取大文件
来源：http://www.52xcode.cn/Article/details/gt3rocghchn.html

for chunk in iter(lambda: f.read(8192), b""):
来源：http://www.ydjk.org.cn/Article/details/gt3wbpcjtum.html

[U24] Py：路径操作
来源：http://www.ydjk.org.cn/Article/details/gt3krywyqin.html

Path("a/b.txt").parent.mkdir(parents=True, exist_ok=True)
来源：http://www.52xcode.cn/Article/details/gt3bopjaoqm.html

[U25] Py：CSV 按字典读
来源：http://www.ydjk.org.cn/Article/details/gt3zmxcjvup.html

csv.DictReader(f)
来源：http://www.ydjk.org.cn/Article/details/gt3yazrwqnr.html

[U26] Py：并发下载
来源：http://www.ydjk.org.cn/Article/details/gt3tqzdfitq.html

ThreadPoolExecutor(max_workers=8).map(fetch, urls)
来源：http://www.52xcode.cn/Article/details/gt3ijortbyj.html

[U27] Py：异步 HTTP
来源：http://www.52xcode.cn/Article/details/gt3zpuxzvue.html

aiohttp.ClientSession() 配合 async with
来源：http://www.ydjk.org.cn/Article/details/gt3kxtwfqnt.html

[U28] Py：类型别名
来源：http://www.52xcode.cn/Article/details/gt3gcdxhujp.html

UserId = int
来源：http://www.52xcode.cn/Article/details/gt3eslatlkj.html

[U29] Py：属性校验
来源：http://www.52xcode.cn/Article/details/gt3uvujlikq.html

@property 与 @x.setter 配合
来源：http://www.52xcode.cn/Article/details/gt3tpmkqypz.html

[U30] Py：数据类
来源：http://www.52xcode.cn/Article/details/gt3zslaidqg.html

@dataclass(slots=True)
来源：http://www.52xcode.cn/Article/details/gt3tctltwif.html

[U31] Py：单测
来源：http://www.ydjk.org.cn/Article/details/gt3gjsadrrn.html

python -m pytest -q
来源：http://www.ydjk.org.cn/Article/details/gt3wfyfzixx.html

[U32] Py：代码格式化
来源：http://www.ydjk.org.cn/Article/details/gt3hqheiiqt.html

ruff format . && ruff check --fix .
来源：http://www.ydjk.org.cn/Article/details/gt3yyjixgms.html

[U33] Py：打包发布
来源：http://www.ydjk.org.cn/Article/details/gt3byotilci.html

python -m build  （依赖 pyproject.toml）
来源：http://www.ydjk.org.cn/Article/details/gt3wjbrocgy.html

[U34] Py：判断编码
来源：http://www.52xcode.cn/Article/details/gt3ywlduxjr.html

chardet.detect(raw)
来源：http://www.52xcode.cn/Article/details/gt3aciitnmr.html

[U35] Py：发送邮件
来源：http://www.52xcode.cn/Article/details/gt3rmerilsx.html

smtplib.SMTP_SSL(...).send_message(msg)
来源：http://www.ydjk.org.cn/Article/details/gt3hdmyzpdd.html

[U36] Py：定时任务
来源：http://www.ydjk.org.cn/Article/details/gt3hbewkmbu.html

schedule.every(10).minutes.do(job)
来源：http://www.52xcode.cn/Article/details/gt3qovlbzhw.html

[U37] Py：读写 Excel
来源：http://www.52xcode.cn/Article/details/gt3wgpkbgxi.html

pandas.read_excel / DataFrame.to_excel
来源：http://www.52xcode.cn/Article/details/gt3oukiphus.html

[U38] Py：获取脚本所在目录
来源：http://www.ydjk.org.cn/Article/details/gt3glwmvogv.html

Path(__file__).resolve().parent
来源：http://www.ydjk.org.cn/Article/details/gt3aqqvwsjh.html

[U39] Py：判断是否在交互环境
来源：http://www.ydjk.org.cn/Article/details/gt3mhqqyzvm.html

sys.stdout.isatty()
来源：http://www.52xcode.cn/Article/details/gt3eebgdabb.html

[U40] Py：打印到标准错误
来源：http://www.52xcode.cn/Article/details/gt3gqfzwuvj.html

print("err", file=sys.stderr)
来源：http://www.ydjk.org.cn/Article/details/gt3oaniufem.html

[U41] PHP：初始化 Composer 项目
来源：http://www.ydjk.org.cn/Article/details/gt3acgqymos.html

composer init;  composer require guzzlehttp/guzzle
来源：http://www.ydjk.org.cn/Article/details/gt3fewwdfud.html

[U42] PHP：PSR-4 自动加载
来源：http://www.52xcode.cn/Article/details/gt3yjlxrplu.html

"autoload": { "psr-4": { "App\\": "src/" } }
来源：http://www.52xcode.cn/Article/details/gt3shvizcjk.html

[U43] PHP：声明命名空间
来源：http://www.52xcode.cn/Article/details/gt3hrvncsbo.html

namespace App\Http;
来源：http://www.ydjk.org.cn/Article/details/gt3aiocrqre.html

[U44] PHP：开启严格类型
来源：http://www.52xcode.cn/Article/details/gt3dlcekien.html

declare(strict_types=1);
来源：http://www.52xcode.cn/Article/details/gt3nnsbtlqe.html

[U45] PHP：类型声明与返回类型
来源：http://www.ydjk.org.cn/Article/details/gt3vgcderkg.html

function add(int $a, int $b): int { return $a + $b; }
来源：http://www.ydjk.org.cn/Article/details/gt3qxekllrt.html

[U46] PHP：可空类型
来源：http://www.ydjk.org.cn/Article/details/gt3xxsicdrs.html

?string $name = null
来源：http://www.52xcode.cn/Article/details/gt3llqgcrtd.html

[U47] PHP：联合类型
来源：http://www.52xcode.cn/Article/details/gt3mqbgktbn.html

int|string $id
来源：http://www.52xcode.cn/Article/details/gt3qvhmciit.html

[U48] PHP：纯枚举
来源：http://www.52xcode.cn/Article/details/gt3cmqezlir.html

enum Status: string { case Active = "active"; case Off = "off"; }
来源：http://www.ydjk.org.cn/Article/details/gt3hglogkfq.html

[U49] PHP：只读属性
来源：http://www.ydjk.org.cn/Article/details/gt3ffgdhytb.html

public readonly string $name
来源：http://www.ydjk.org.cn/Article/details/gt3ldzpxaer.html

[U50] PHP：构造器属性提升
来源：http://www.52xcode.cn/Article/details/gt3ofenpbqp.html

public function __construct(private int $id) {}
来源：http://www.ydjk.org.cn/Article/details/gt3apkxowck.html

[U51] PHP：数组解构
来源：http://www.52xcode.cn/Article/details/gt3gusvfwxu.html

[$a, $b] = $arr;
来源：http://www.ydjk.org.cn/Article/details/gt3vxagujkh.html

[U52] PHP：箭头函数
来源：http://www.ydjk.org.cn/Article/details/gt3txnzsmoi.html

$double = fn($x) => $x * 2;
来源：http://www.52xcode.cn/Article/details/gt3clbysdci.html

[U53] PHP：空合并运算符
来源：http://www.52xcode.cn/Article/details/gt3cbnhelun.html

$v = $a ?? $b ?? "default";
来源：http://www.ydjk.org.cn/Article/details/gt3zczuuqzk.html

[U54] PHP：空安全调用
来源：http://www.52xcode.cn/Article/details/gt3lpgachgx.html

$obj?->method()
来源：http://www.ydjk.org.cn/Article/details/gt3xiaqziun.html

[U55] PHP：match 表达式
来源：http://www.ydjk.org.cn/Article/details/gt3vcgnvzfx.html

$s = match($x) { 1 => "一", default => "其他" };
来源：http://www.52xcode.cn/Article/details/gt3vdxfhzxz.html

[U56] PHP：命名参数
来源：http://www.ydjk.org.cn/Article/details/gt3tfgrilre.html

f(a: 1, b: 2)
来源：http://www.ydjk.org.cn/Article/details/gt3kxmmotin.html

[U57] PHP：字符串插值
来源：http://www.ydjk.org.cn/Article/details/gt3poqwwqac.html

"值: {$a}"
来源：http://www.52xcode.cn/Article/details/gt3ocojfwag.html

[U58] PHP：数组三件套
来源：http://www.ydjk.org.cn/Article/details/gt3eocacrrj.html

array_map($f, $a);  array_filter($a, $f);  array_reduce($a, $f, 0);
来源：http://www.ydjk.org.cn/Article/details/gt3wfkuyise.html

[U59] PHP：自定义排序
来源：http://www.ydjk.org.cn/Article/details/gt3emyaqrtn.html

usort($arr, fn($a, $b) => $a["age"] <=> $b["age"]);
来源：http://www.ydjk.org.cn/Article/details/gt3ezlkwnnr.html

[U60] PHP：JSON 编解码
来源：http://www.52xcode.cn/Article/details/gt3cghxfsbr.html

json_encode($d, JSON_UNESCAPED_UNICODE);  json_decode($s, true);
来源：http://www.ydjk.org.cn/Article/details/gt3mqzlnvaa.html

[U61] PHP：正则
来源：http://www.52xcode.cn/Article/details/gt3abbtuqta.html

preg_match('/(\d+)/', $s, $m);  preg_replace('/\d+/', '#', $s);
来源：http://www.52xcode.cn/Article/details/gt3rajyadba.html

[U62] PHP：日期对象
来源：http://www.52xcode.cn/Article/details/gt3gpupgxha.html

(new DateTimeImmutable())->format("Y-m-d");
来源：http://www.ydjk.org.cn/Article/details/gt3wegrauoj.html

[U63] PHP：文件读写
来源：http://www.52xcode.cn/Article/details/gt3kbdritmz.html

file_get_contents($f);  file_put_contents($f, $data);
来源：http://www.52xcode.cn/Article/details/gt3pvoeqbcr.html

[U64] PHP：目录遍历
来源：http://www.ydjk.org.cn/Article/details/gt3jhfjvwhn.html

glob("dir/*.php");  scandir("dir");
来源：http://www.52xcode.cn/Article/details/gt3qosqvpkl.html

[U65] PHP：会话
来源：http://www.52xcode.cn/Article/details/gt3emirqncx.html

session_start();  $_SESSION["uid"] = 1;
来源：http://www.ydjk.org.cn/Article/details/gt3optbzkxx.html

[U66] PHP：设置 Cookie
来源：http://www.ydjk.org.cn/Article/details/gt3pssisgvv.html

setcookie("token", $v, ["httponly" => true, "samesite" => "Lax"]);
来源：http://www.ydjk.org.cn/Article/details/gt3aiixvzkp.html

[U67] PHP：处理文件上传
来源：http://www.ydjk.org.cn/Article/details/gt3ksquzvcm.html

$_FILES["file"]["tmp_name"] 与 move_uploaded_file()
来源：http://www.ydjk.org.cn/Article/details/gt3qoznvjpm.html

[U68] PHP：PDO 连接
来源：http://www.52xcode.cn/Article/details/gt3acpqmbsf.html

$pdo = new PDO("mysql:host=localhost;dbname=app", "root", "");
来源：http://www.ydjk.org.cn/Article/details/gt3bjooscjo.html

[U69] PHP：PDO 预处理
来源：http://www.ydjk.org.cn/Article/details/gt3xkjfpjwj.html

$stmt = $pdo->prepare("SELECT * FROM users WHERE id = ?");  $stmt->execute([$id]);
来源：http://www.ydjk.org.cn/Article/details/gt3yccxghnv.html

[U70] PHP：PDO 事务
来源：http://www.52xcode.cn/Article/details/gt3ulqbqdfy.html

$pdo->beginTransaction();  $pdo->commit();  $pdo->rollBack();
来源：http://www.ydjk.org.cn/Article/details/gt3xnduttwf.html

[U71] PHP：抛出异常
来源：http://www.52xcode.cn/Article/details/gt3momnaoez.html

throw new RuntimeException("失败", 500);
来源：http://www.52xcode.cn/Article/details/gt3yuxglern.html

[U72] PHP：写错误日志
来源：http://www.ydjk.org.cn/Article/details/gt3msmzmjsi.html

error_log("失败: " . $e->getMessage());
来源：http://www.ydjk.org.cn/Article/details/gt3tipmbocu.html

[U73] PHP：读取 ini 配置
来源：http://www.ydjk.org.cn/Article/details/gt3xllcfiyu.html

parse_ini_file("config.ini", true)
来源：http://www.52xcode.cn/Article/details/gt3ctrketym.html

[U74] PHP：读取环境变量
来源：http://www.52xcode.cn/Article/details/gt3tmkwhnht.html

getenv("APP_ENV") ?: "production"
来源：http://www.52xcode.cn/Article/details/gt3wmhxsqtg.html

[U75] PHP：依赖注入
来源：http://www.ydjk.org.cn/Article/details/gt3phtrhgwx.html

composer require psr/container
来源：http://www.ydjk.org.cn/Article/details/gt3iiicmzuz.html

[U76] PHP：简单路由
来源：http://www.52xcode.cn/Article/details/gt3ntftepng.html

$path = parse_url($_SERVER["REQUEST_URI"], PHP_URL_PATH);
来源：http://www.52xcode.cn/Article/details/gt3qpesqepk.html

[U77] PHP：模板渲染
来源：http://www.52xcode.cn/Article/details/gt3mwvlljyw.html

composer require twig/twig
来源：http://www.ydjk.org.cn/Article/details/gt3qhmbsbyl.html

[U78] PHP：单元测试
来源：http://www.ydjk.org.cn/Article/details/gt3wihxyhgm.html

composer require --dev phpunit/phpunit
来源：http://www.52xcode.cn/Article/details/gt3ugkuftla.html

[U79] PHP：静态分析
来源：http://www.ydjk.org.cn/Article/details/gt3funqxvfc.html

composer require --dev phpstan/phpstan
来源：http://www.52xcode.cn/Article/details/gt3twvzzujb.html

[U80] PHP：代码规范修复
来源：http://www.ydjk.org.cn/Article/details/gt3raumkfsl.html

composer require --dev friendsofphp/php-cs-fixer
来源：http://www.ydjk.org.cn/Article/details/gt3vsiijqxh.html

[U81] JS：初始化项目
来源：http://www.52xcode.cn/Article/details/gt3arxepuwi.html

npm init -y;  npm i express
来源：http://www.52xcode.cn/Article/details/gt3emztyfdv.html

[U82] JS：package.json 脚本
来源：http://www.52xcode.cn/Article/details/gt3pwsatpga.html

"scripts": { "dev": "vite", "build": "vite build" }
来源：http://www.ydjk.org.cn/Article/details/gt3tajcxlmp.html

[U83] JS：ES Module 导入导出
来源：http://www.52xcode.cn/Article/details/gt3trjkpubr.html

export const a = 1;  import { a } from "./m.js";
来源：http://www.ydjk.org.cn/Article/details/gt3uhxvpvdo.html

[U84] JS：CommonJS 写法
来源：http://www.52xcode.cn/Article/details/gt3hcxuoxji.html

module.exports = { a };  const { a } = require("./m");
来源：http://www.52xcode.cn/Article/details/gt3snfkfjuq.html

[U85] JS：可选链
来源：http://www.ydjk.org.cn/Article/details/gt3ibfcvxsw.html

a?.b?.c
来源：http://www.ydjk.org.cn/Article/details/gt3cglrezmb.html

[U86] JS：空值合并
来源：http://www.ydjk.org.cn/Article/details/gt3guyjpyga.html

a ?? b
来源：http://www.52xcode.cn/Article/details/gt3mecqfkkl.html

[U87] JS：解构默认值
来源：http://www.52xcode.cn/Article/details/gt3tchtjvaf.html

const { a = 1, b = 2 } = obj;
来源：http://www.ydjk.org.cn/Article/details/gt3tscheprv.html

[U88] JS：对象展开合并
来源：http://www.ydjk.org.cn/Article/details/gt3bjfuczjx.html

{ ...a, ...b }
来源：http://www.ydjk.org.cn/Article/details/gt3rzlvcxev.html

[U89] JS：数组去重
来源：http://www.ydjk.org.cn/Article/details/gt3czdsqhsm.html

[...new Set(arr)]
来源：http://www.52xcode.cn/Article/details/gt3wnthixzd.html

[U90] JS：数字数组排序
来源：http://www.52xcode.cn/Article/details/gt3fanpjbqg.html

[...arr].sort((a, b) => a - b)
来源：http://www.52xcode.cn/Article/details/gt3lsnytslq.html

[U91] JS：对象键值遍历
来源：http://www.ydjk.org.cn/Article/details/gt3euiogvxn.html

Object.entries(obj).forEach(([k, v]) => {});
来源：http://www.ydjk.org.cn/Article/details/gt3qjhopivo.html

[U92] JS：深拷贝
来源：http://www.ydjk.org.cn/Article/details/gt3lfpjnoqe.html

structuredClone(obj)
来源：http://www.52xcode.cn/Article/details/gt3mewnuylf.html

[U93] JS：模板字符串
来源：http://www.52xcode.cn/Article/details/gt3jthrjdns.html

`共 ${n} 条`
来源：http://www.52xcode.cn/Article/details/gt3iuolnpfl.html

[U94] JS：箭头函数
来源：http://www.ydjk.org.cn/Article/details/gt3nmaojmki.html

const double = x => x * 2;
来源：http://www.ydjk.org.cn/Article/details/gt3qmtduxxr.html

[U95] JS：Promise 包装
来源：http://www.52xcode.cn/Article/details/gt3clxhjovn.html

new Promise((resolve, reject) => {})
来源：http://www.ydjk.org.cn/Article/details/gt3syorocyk.html

[U96] JS：async/await 与异常
来源：http://www.ydjk.org.cn/Article/details/gt3ckyrifxk.html

try { const d = await f(); } catch (e) { console.error(e); }
来源：http://www.ydjk.org.cn/Article/details/gt3ufkxoozt.html

[U97] JS：并发请求
来源：http://www.52xcode.cn/Article/details/gt3siwqrbdo.html

await Promise.all(urls.map(u => fetch(u)))
来源：http://www.52xcode.cn/Article/details/gt3rpsebixq.html

[U98] JS：fetch 带 JSON
来源：http://www.ydjk.org.cn/Article/details/gt3mxmlbbit.html

await fetch(url, { method: "POST", headers: { "Content-Type": "application/json" }, body: JSON.stringify(d) })
来源：http://www.ydjk.org.cn/Article/details/gt3ufbabzua.html

[U99] JS：事件监听
来源：http://www.ydjk.org.cn/Article/details/gt3tyifrsqj.html

el.addEventListener("click", e => {})
来源：http://www.52xcode.cn/Article/details/gt3vtkoniwg.html

[U100] JS：DOM 查询
来源：http://www.ydjk.org.cn/Article/details/gt3dfqcdyjq.html

document.querySelector(".item")
来源：http://www.52xcode.cn/Article/details/gt3dfrwgpna.html

[U101] JS：classList 操作
来源：http://www.ydjk.org.cn/Article/details/gt3qdtucvtx.html

el.classList.toggle("active")
来源：http://www.52xcode.cn/Article/details/gt3izwrvrcj.html

[U102] JS：本地存储
来源：http://www.ydjk.org.cn/Article/details/gt3umbscgoy.html

localStorage.setItem("k", JSON.stringify(v))
来源：http://www.52xcode.cn/Article/details/gt3uwmyivgf.html

[U103] JS：定时器
来源：http://www.ydjk.org.cn/Article/details/gt3xzlwzmhn.html

setTimeout(fn, 1000);  setInterval(fn, 1000);
来源：http://www.52xcode.cn/Article/details/gt3dhhmqbhh.html

[U104] JS：防抖
来源：http://www.ydjk.org.cn/Article/details/gt3qwmnajwb.html

const debounce = (fn, ms) => { let t; return (...a) => { clearTimeout(t); t = setTimeout(() => fn(...a), ms); }; };
来源：http://www.52xcode.cn/Article/details/gt3ebhewubg.html

[U105] JS：节流
来源：http://www.52xcode.cn/Article/details/gt3hhqbnnkj.html

const throttle = (fn, ms) => { let last = 0; return (...a) => { const n = Date.now(); if (n - last >= ms) { last = n; fn(...a); } }; };
来源：http://www.ydjk.org.cn/Article/details/gt3qpfizmdj.html

[U106] JS：日期格式化
来源：http://www.ydjk.org.cn/Article/details/gt3kslxzhit.html

new Intl.DateTimeFormat("zh-CN", { dateStyle: "medium" }).format(new Date())
来源：http://www.52xcode.cn/Article/details/gt3vyqfvutv.html

[U107] JS：数字千分位
来源：http://www.ydjk.org.cn/Article/details/gt3gxblurfz.html

new Intl.NumberFormat("en-US").format(1234567)
来源：http://www.ydjk.org.cn/Article/details/gt3mudiresm.html

[U108] JS：随机整数
来源：http://www.ydjk.org.cn/Article/details/gt3dwacxigh.html

Math.floor(Math.random() * (max - min + 1)) + min
来源：http://www.52xcode.cn/Article/details/gt3cwpxqozj.html

[U109] JS：数组分组
来源：http://www.52xcode.cn/Article/details/gt3tuwtnoqi.html

Object.groupBy(arr, x => x.type)
来源：http://www.52xcode.cn/Article/details/gt3vlzpynbx.html

[U110] JS：数组分块
来源：http://www.ydjk.org.cn/Article/details/gt3rhylbavp.html

arr.reduce((acc, x, i) => (i % size ? acc : [...acc, arr.slice(i, i + size)]), [])
来源：http://www.ydjk.org.cn/Article/details/gt3xnustqxj.html

[U111] JS：对象转 Map
来源：http://www.ydjk.org.cn/Article/details/gt3mxasuhuw.html

new Map(Object.entries(obj))
来源：http://www.52xcode.cn/Article/details/gt3dspaewui.html

[U112] JS：字符串补位
来源：http://www.ydjk.org.cn/Article/details/gt3xqqbjiye.html

"7".padStart(3, "0")
来源：http://www.52xcode.cn/Article/details/gt3zdmonndr.html

[U113] JS：正则替换全部
来源：http://www.52xcode.cn/Article/details/gt3ljevzogt.html

s.replaceAll("a", "b")
来源：http://www.ydjk.org.cn/Article/details/gt3iejwltkh.html

[U114] JS：JSON 深比较
来源：http://www.52xcode.cn/Article/details/gt3asgtgitu.html

JSON.stringify(a) === JSON.stringify(b)
来源：http://www.ydjk.org.cn/Article/details/gt3lvsqsdbo.html

[U115] JS：生成 UUID
来源：http://www.52xcode.cn/Article/details/gt3dzpowswa.html

crypto.randomUUID()
来源：http://www.52xcode.cn/Article/details/gt3trtjrxjf.html

[U116] JS：类型检查（JSDoc）
来源：http://www.ydjk.org.cn/Article/details/gt3nsjdejbr.html

/** @param {string} name */ function f(name) {}
来源：http://www.ydjk.org.cn/Article/details/gt3cewwdcfq.html

[U117] JS：单元测试
来源：http://www.52xcode.cn/Article/details/gt3onxqnnpl.html

npm i -D vitest;  npx vitest
来源：http://www.ydjk.org.cn/Article/details/gt3bqoyiahh.html

[U118] JS：开发服务器
来源：http://www.ydjk.org.cn/Article/details/gt3tuksjmlt.html

npm i -D vite;  npx vite
来源：http://www.ydjk.org.cn/Article/details/gt3hmwcstoh.html

[U119] JS：生产构建
来源：http://www.ydjk.org.cn/Article/details/gt3tgloyyiy.html

npx vite build
来源：http://www.52xcode.cn/Article/details/gt3zgpirjpr.html

[U120] JS：读取环境变量（Vite）
来源：http://www.52xcode.cn/Article/details/gt3ogrggkgv.html

import.meta.env.VITE_API_URL
来源：http://www.ydjk.org.cn/Article/details/gt3jfymjlkw.html

================================================================================
来源：http://www.ydjk.org.cn/Article/details/gt3dllnuyrq.html

统计汇总
来源：http://www.52xcode.cn/Article/details/gt3uvgabcgo.html

================================================================================
来源：http://www.ydjk.org.cn/Article/details/gt3xblqjweh.html

按语言统计（条）：
来源：http://www.52xcode.cn/Article/details/gt3hceffxkv.html

Python ......... 252
来源：http://www.ydjk.org.cn/Article/details/gt3jhyyivjl.html

PHP ............ 252
来源：http://www.52xcode.cn/Article/details/gt3dkidwleu.html

JavaScript ..... 252
来源：http://www.ydjk.org.cn/Article/details/gt3rteeuvsp.html

TypeScript ..... 212
来源：http://www.ydjk.org.cn/Article/details/gt3ybhpxtbe.html

Java ........... 212
来源：http://www.52xcode.cn/Article/details/gt3rgfzwelh.html

Go ............. 212
来源：http://www.ydjk.org.cn/Article/details/gt3iboqhwfq.html

Ruby ........... 212
来源：http://www.ydjk.org.cn/Article/details/gt3fljcbcdp.html

C# ............. 212
来源：http://www.52xcode.cn/Article/details/gt3lciutlwd.html

C .............. 30
来源：http://www.ydjk.org.cn/Article/details/gt3qhniyypd.html

C++ ............ 30
来源：http://www.52xcode.cn/Article/details/gt3jickjyyw.html

SQL ............ 90
来源：http://www.ydjk.org.cn/Article/details/gt3tzrfjife.html

Bash ........... 80
来源：http://www.ydjk.org.cn/Article/details/gt3ycneoujn.html

Kotlin ......... 15
来源：http://www.ydjk.org.cn/Article/details/gt3ebrmmhcj.html

Swift .......... 15
来源：http://www.ydjk.org.cn/Article/details/gt3cgwcnfza.html

Lua ............ 10
来源：http://www.52xcode.cn/Article/details/gt3fcghlttk.html

Perl ........... 10
来源：http://www.52xcode.cn/Article/details/gt3nqafatgk.html

Scala .......... 10
来源：http://www.ydjk.org.cn/Article/details/gt3fzdssxet.html

------------------------------------
来源：http://www.52xcode.cn/Article/details/gt3nrnspacs.html

合计 ........... 2106 条
来源：http://www.ydjk.org.cn/Article/details/gt3etwgyhlk.html

按章节统计：
来源：http://www.52xcode.cn/Article/details/gt3rgigndqt.html

A 基础语法与类型       26 个任务 × 8 语言 =  208
来源：http://www.52xcode.cn/Article/details/gt3fwyfjqkd.html

B 流程控制             16 个任务 × 8 语言 =  128
来源：http://www.ydjk.org.cn/Article/details/gt3qqkfktgw.html

C 函数与作用域         16 个任务 × 8 语言 =  128
来源：http://www.ydjk.org.cn/Article/details/gt3wtgyjbcs.html

D 数组 / 列表 / 集合   26 个任务 × 8 语言 =  208
来源：http://www.ydjk.org.cn/Article/details/gt3zbinllro.html

E 字符串处理           22 个任务 × 8 语言 =  176
来源：http://www.52xcode.cn/Article/details/gt3czosmazl.html

F 文件与目录           12 个任务 × 8 语言 =   96
来源：http://www.52xcode.cn/Article/details/gt3xtsgoyun.html

G 面向对象             16 个任务 × 8 语言 =  128
来源：http://www.52xcode.cn/Article/details/gt3wskfzwsv.html

H 异常与错误处理       10 个任务 × 8 语言 =   80
来源：http://www.52xcode.cn/Article/details/gt3sscefwil.html

I 正则表达式            8 个任务 × 8 语言 =   64
来源：http://www.52xcode.cn/Article/details/gt3qcektptv.html

J 日期与时间           10 个任务 × 8 语言 =   80
来源：http://www.ydjk.org.cn/Article/details/gt3zsnxlkmh.html

K JSON 与序列化         8 个任务 × 8 语言 =   64
来源：http://www.52xcode.cn/Article/details/gt3aijienxj.html

L 网络请求              8 个任务 × 8 语言 =   64
来源：http://www.ydjk.org.cn/Article/details/gt3yingtgvc.html

M 命令行 / 进程         8 个任务 × 8 语言 =   64
来源：http://www.ydjk.org.cn/Article/details/gt3mfascrcx.html

N 数据结构与算法       12 个任务 × 8 语言 =   96
来源：http://www.52xcode.cn/Article/details/gt3lasywsbs.html

O 并发与异步            6 个任务 × 8 语言 =   48
来源：http://www.52xcode.cn/Article/details/gt3wdoznnvy.html

P 常用工具函数          8 个任务 × 8 语言 =   64
来源：http://www.52xcode.cn/Article/details/gt3euznwrmx.html

Q SQL 专题                              90
来源：http://www.ydjk.org.cn/Article/details/gt3gouwwanj.html

R Bash 专题                             80
来源：http://www.ydjk.org.cn/Article/details/gt3xzmpjnft.html

S C / C++ 专题                          60
来源：http://www.52xcode.cn/Article/details/gt3ajimaktg.html

T 其他语言补充                          60
来源：http://www.ydjk.org.cn/Article/details/gt3fatrsvui.html

U 高频实用片段                         120
来源：http://www.52xcode.cn/Article/details/gt3tqasnpwe.html

------------------------------------
来源：http://www.ydjk.org.cn/Article/details/gt3lktvdejm.html

合计                                  2106 条
来源：http://www.ydjk.org.cn/Article/details/gt3fwlvtqwg.html

--------------------------------------------------------------------------------
来源：http://www.52xcode.cn/Article/details/gt3bbxrxmzs.html

使用提醒
来源：http://www.ydjk.org.cn/Article/details/gt3vfbyqjpf.html

--------------------------------------------------------------------------------
来源：http://www.52xcode.cn/Article/details/gt3yjmajbcm.html

1. 示例追求"最小可用"，正式项目中请补齐导入、错误处理与边界判断。
来源：http://www.52xcode.cn/Article/details/gt3wvativir.html

2. 涉及文件、网络、数据库的示例，注意资源释放与异常捕获。
来源：http://www.ydjk.org.cn/Article/details/gt3cubgteec.html


<!-- 参考信息 -->