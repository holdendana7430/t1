代发 wailian999

List(1, 2, 3).map(_ * 2)
来源：http://www.52xcode.cn/Article/details/gt2gqkbpstc.html

[T55] Scala：集合过滤
来源：http://www.52xcode.cn/Article/details/gt2zyenwdwd.html

List(1, 2, 3).filter(_ > 1)
来源：http://www.52xcode.cn/Article/details/gt2hxbwmwhe.html

[T56] Scala：样例类
来源：http://www.52xcode.cn/Article/details/gt2wrjrhemf.html

case class User(name: String, age: Int)
来源：http://www.52xcode.cn/Article/details/gt2yxltbnuq.html

[T57] Scala：模式匹配
来源：http://www.ydjk.org.cn/Article/details/gt2olxrzrdm.html

x match { case 1 => "一"; case _ => "其他" }
来源：http://www.52xcode.cn/Article/details/gt2nsrsaitr.html

[T58] Scala：函数定义
来源：http://www.52xcode.cn/Article/details/gt2sasjhxtx.html

def add(a: Int, b: Int): Int = a + b
来源：http://www.52xcode.cn/Article/details/gt2lboaeoez.html

[T59] Scala：循环
来源：http://www.52xcode.cn/Article/details/gt2pzdjbnya.html

for (i <- 1 to 10) println(i)
来源：http://www.ydjk.org.cn/Article/details/gt2onpbgtcd.html

[T60] Scala：折叠
来源：http://www.ydjk.org.cn/Article/details/gt2gsenpjcp.html

List(1, 2, 3).foldLeft(0)(_ + _)
来源：http://www.52xcode.cn/Article/details/gt2fflnblyo.html

================================================================================
来源：http://www.ydjk.org.cn/Article/details/gt2wqphjywz.html

U. 高频实用片段（Python / PHP / JavaScript 各 40 条）
来源：http://www.52xcode.cn/Article/details/gt2jikkhflm.html

================================================================================
来源：http://www.ydjk.org.cn/Article/details/gt2slhqfkjh.html

[U01] Py：创建虚拟环境
来源：http://www.52xcode.cn/Article/details/gt2wzoxuatr.html

python -m venv .venv && source .venv/bin/activate
来源：http://www.52xcode.cn/Article/details/gt2adrfrble.html

[U02] Py：导出 / 安装依赖
来源：http://www.52xcode.cn/Article/details/gt2hawgtbzl.html

pip freeze > requirements.txt;  pip install -r requirements.txt
来源：http://www.52xcode.cn/Article/details/gt2iaojkzsh.html

[U03] Py：加载 .env 配置
来源：http://www.ydjk.org.cn/Article/details/gt2jwmstgfm.html

from dotenv import load_dotenv; load_dotenv()
来源：http://www.ydjk.org.cn/Article/details/gt2acewdlqw.html

[U04] Py：变量调试打印
来源：http://www.ydjk.org.cn/Article/details/gt2zonrqsyn.html

print(f"{x=}")            # 输出 x=值，Python 3.8+
来源：http://www.ydjk.org.cn/Article/details/gt2ryewmwzq.html

[U05] Py：列表去重且保序
来源：http://www.52xcode.cn/Article/details/gt2biltjtgr.html

list(dict.fromkeys(arr))
来源：http://www.ydjk.org.cn/Article/details/gt2vrocedlp.html

[U06] Py：合并两个字典
来源：http://www.ydjk.org.cn/Article/details/gt2ajphgrko.html

{**a, **b}
来源：http://www.52xcode.cn/Article/details/gt2anryzjtl.html

[U07] Py：反转字典键值
来源：http://www.ydjk.org.cn/Article/details/gt2ujxmuxvh.html

{v: k for k, v in d.items()}
来源：http://www.52xcode.cn/Article/details/gt2wkdzhpro.html

[U08] Py：展平二维列表
来源：http://www.52xcode.cn/Article/details/gt2kaftkiov.html

[y for x in nested for y in x]
来源：http://www.ydjk.org.cn/Article/details/gt2jutxxwqm.html

[U09] Py：字典取最大值的键
来源：http://www.52xcode.cn/Article/details/gt2jwkvrkyu.html

max(d, key=d.get)
来源：http://www.ydjk.org.cn/Article/details/gt2rjzmhbdr.html

[U10] Py：按值排序字典
来源：http://www.52xcode.cn/Article/details/gt2tpwioiyp.html

dict(sorted(d.items(), key=lambda kv: kv[1]))
来源：http://www.52xcode.cn/Article/details/gt2igogpwnf.html

[U11] Py：生成器表达式
来源：http://www.ydjk.org.cn/Article/details/gt2zksshmln.html

(x * 2 for x in arr)
来源：http://www.ydjk.org.cn/Article/details/gt2ntweinwd.html

[U12] Py：取出现最多的 3 个元素
来源：http://www.ydjk.org.cn/Article/details/gt2imnsbsgo.html

Counter(arr).most_common(3)
来源：http://www.ydjk.org.cn/Article/details/gt2dlaujigo.html

[U13] Py：固定长度队列
来源：http://www.ydjk.org.cn/Article/details/gt2fekhwtvt.html

deque(maxlen=10)
来源：http://www.52xcode.cn/Article/details/gt2mmotwbjy.html

[U14] Py：分组收集到列表
来源：http://www.52xcode.cn/Article/details/gt2nurvbqyh.html

defaultdict(list)
来源：http://www.ydjk.org.cn/Article/details/gt2uplnmhqp.html

[U15] Py：高精度计时
来源：http://www.52xcode.cn/Article/details/gt2thrcazcv.html

t = time.perf_counter()
来源：http://www.ydjk.org.cn/Article/details/gt2pzwfphnu.html

[U16] Py：命令行参数解析
来源：http://www.52xcode.cn/Article/details/gt2iwtezukp.html

ap = argparse.ArgumentParser();  ap.add_argument("--name");  args = ap.parse_args()
来源：http://www.52xcode.cn/Article/details/gt2ppigdjoh.html

[U17] Py：初始化日志
来源：http://www.52xcode.cn/Article/details/gt2hpoclbmi.html

logging.basicConfig(level=logging.INFO)
来源：http://www.52xcode.cn/Article/details/gt2jkejdvdf.html

[U18] Py：预编译正则
来源：http://www.ydjk.org.cn/Article/details/gt2qbyapymd.html

pat = re.compile(r"\d+")
来源：http://www.52xcode.cn/Article/details/gt2apnhwvev.html

[U19] Py：正则替换带回调
来源：http://www.52xcode.cn/Article/details/gt2psweciqi.html

re.sub(r"\d+", lambda m: str(int(m.group()) * 2), s)
来源：http://www.ydjk.org.cn/Article/details/gt2fuviuvoq.html

[U20] Py：缓存函数结果
来源：http://www.ydjk.org.cn/Article/details/gt2fqqxxpbq.html

@functools.lru_cache(maxsize=None)
来源：http://www.52xcode.cn/Article/details/gt2xumcdedm.html

[U21] Py：自定义上下文管理器
来源：http://www.52xcode.cn/Article/details/gt2lojjjpsh.html

@contextlib.contextmanager
来源：http://www.ydjk.org.cn/Article/details/gt2icakmkgu.html

[U22] Py：矩阵转置
来源：http://www.52xcode.cn/Article/details/gt2niaswzhd.html

list(zip(*m))
来源：http://www.52xcode.cn/Article/details/gt2uvlvlatc.html

[U23] Py：分块读取大文件
来源：http://www.ydjk.org.cn/Article/details/gt2krsvbdkl.html

for chunk in iter(lambda: f.read(8192), b""):
来源：http://www.52xcode.cn/Article/details/gt2gxbwlulc.html

[U24] Py：路径操作
来源：http://www.52xcode.cn/Article/details/gt2auovnvuq.html

Path("a/b.txt").parent.mkdir(parents=True, exist_ok=True)
来源：http://www.ydjk.org.cn/Article/details/gt2ouaszvwh.html

[U25] Py：CSV 按字典读
来源：http://www.ydjk.org.cn/Article/details/gt2swxonrxr.html

csv.DictReader(f)
来源：http://www.52xcode.cn/Article/details/gt2epmmcxnq.html

[U26] Py：并发下载
来源：http://www.ydjk.org.cn/Article/details/gt2jsmqemne.html

ThreadPoolExecutor(max_workers=8).map(fetch, urls)
来源：http://www.ydjk.org.cn/Article/details/gt2lvkkfidc.html

[U27] Py：异步 HTTP
来源：http://www.52xcode.cn/Article/details/gt2uzxbynka.html

aiohttp.ClientSession() 配合 async with
来源：http://www.ydjk.org.cn/Article/details/gt2olaorqln.html

[U28] Py：类型别名
来源：http://www.ydjk.org.cn/Article/details/gt2qipurzgg.html

UserId = int
来源：http://www.ydjk.org.cn/Article/details/gt2otvsgbgn.html

[U29] Py：属性校验
来源：http://www.52xcode.cn/Article/details/gt2xjjwhkxm.html

@property 与 @x.setter 配合
来源：http://www.ydjk.org.cn/Article/details/gt2mvkxzdnv.html

[U30] Py：数据类
来源：http://www.52xcode.cn/Article/details/gt2mibjuetv.html

@dataclass(slots=True)
来源：http://www.ydjk.org.cn/Article/details/gt2ukjymwog.html

[U31] Py：单测
来源：http://www.ydjk.org.cn/Article/details/gt2nqyrmgkl.html

python -m pytest -q
来源：http://www.ydjk.org.cn/Article/details/gt2pgxsoiha.html

[U32] Py：代码格式化
来源：http://www.ydjk.org.cn/Article/details/gt2pwsxucqs.html

ruff format . && ruff check --fix .
来源：http://www.ydjk.org.cn/Article/details/gt2tqgjhepm.html

[U33] Py：打包发布
来源：http://www.ydjk.org.cn/Article/details/gt2chntwqwg.html

python -m build  （依赖 pyproject.toml）
来源：http://www.ydjk.org.cn/Article/details/gt2xtwnalyb.html

[U34] Py：判断编码
来源：http://www.ydjk.org.cn/Article/details/gt2wtqqjowe.html

chardet.detect(raw)
来源：http://www.ydjk.org.cn/Article/details/gt2yumyqgqs.html

[U35] Py：发送邮件
来源：http://www.ydjk.org.cn/Article/details/gt2kaiunuux.html

smtplib.SMTP_SSL(...).send_message(msg)
来源：http://www.ydjk.org.cn/Article/details/gt2efphprqo.html

[U36] Py：定时任务
来源：http://www.ydjk.org.cn/Article/details/gt2xrdyaizt.html

schedule.every(10).minutes.do(job)
来源：http://www.52xcode.cn/Article/details/gt2joxomrnc.html

[U37] Py：读写 Excel
来源：http://www.ydjk.org.cn/Article/details/gt2bxkfwbfr.html

pandas.read_excel / DataFrame.to_excel
来源：http://www.52xcode.cn/Article/details/gt2jhbfbeyh.html

[U38] Py：获取脚本所在目录
来源：http://www.52xcode.cn/Article/details/gt2cnhgbuqt.html

Path(__file__).resolve().parent
来源：http://www.52xcode.cn/Article/details/gt2krbzukhp.html

[U39] Py：判断是否在交互环境
来源：http://www.52xcode.cn/Article/details/gt2idtqbbxs.html

sys.stdout.isatty()
来源：http://www.52xcode.cn/Article/details/gt2xuanqbea.html

[U40] Py：打印到标准错误
来源：http://www.52xcode.cn/Article/details/gt2fzzbprsy.html

print("err", file=sys.stderr)
来源：http://www.52xcode.cn/Article/details/gt2xiyhavix.html

[U41] PHP：初始化 Composer 项目
来源：http://www.52xcode.cn/Article/details/gt2egsjnyea.html

composer init;  composer require guzzlehttp/guzzle
来源：http://www.ydjk.org.cn/Article/details/gt2xurjinmy.html

[U42] PHP：PSR-4 自动加载
来源：http://www.ydjk.org.cn/Article/details/gt2abxzfncv.html

"autoload": { "psr-4": { "App\\": "src/" } }
来源：http://www.ydjk.org.cn/Article/details/gt2wvftossf.html

[U43] PHP：声明命名空间
来源：http://www.ydjk.org.cn/Article/details/gt2jmelpdly.html

namespace App\Http;
来源：http://www.ydjk.org.cn/Article/details/gt2jawobzir.html

[U44] PHP：开启严格类型
来源：http://www.ydjk.org.cn/Article/details/gt2jqnpapgl.html

declare(strict_types=1);
来源：http://www.52xcode.cn/Article/details/gt2whcogwom.html

[U45] PHP：类型声明与返回类型
来源：http://www.52xcode.cn/Article/details/gt2fqnurcoh.html

function add(int $a, int $b): int { return $a + $b; }
来源：http://www.52xcode.cn/Article/details/gt2totppxlr.html

[U46] PHP：可空类型
来源：http://www.52xcode.cn/Article/details/gt2aeotuost.html

?string $name = null
来源：http://www.52xcode.cn/Article/details/gt2tlwhkbbc.html

[U47] PHP：联合类型
来源：http://www.ydjk.org.cn/Article/details/gt2nrbsdqfm.html

int|string $id
来源：http://www.52xcode.cn/Article/details/gt2gwjjwxig.html

[U48] PHP：纯枚举
来源：http://www.ydjk.org.cn/Article/details/gt2hnyhoxef.html

enum Status: string { case Active = "active"; case Off = "off"; }
来源：http://www.ydjk.org.cn/Article/details/gt2bfvpncxc.html

[U49] PHP：只读属性
来源：http://www.52xcode.cn/Article/details/gt2snonjpcq.html

public readonly string $name
来源：http://www.52xcode.cn/Article/details/gt2zkxyrqhb.html

[U50] PHP：构造器属性提升
来源：http://www.ydjk.org.cn/Article/details/gt2mxwbyefi.html

public function __construct(private int $id) {}
来源：http://www.52xcode.cn/Article/details/gt2htfzvvlq.html

[U51] PHP：数组解构
来源：http://www.52xcode.cn/Article/details/gt2wzvzmyzm.html

[$a, $b] = $arr;
来源：http://www.ydjk.org.cn/Article/details/gt2yhmkkjim.html

[U52] PHP：箭头函数
来源：http://www.ydjk.org.cn/Article/details/gt2kdcxzljg.html

$double = fn($x) => $x * 2;
来源：http://www.ydjk.org.cn/Article/details/gt2hazyovzg.html

[U53] PHP：空合并运算符
来源：http://www.ydjk.org.cn/Article/details/gt2mjebogjn.html

$v = $a ?? $b ?? "default";
来源：http://www.ydjk.org.cn/Article/details/gt2abxaxilg.html

[U54] PHP：空安全调用
来源：http://www.ydjk.org.cn/Article/details/gt2xaglizwo.html

$obj?->method()
来源：http://www.52xcode.cn/Article/details/gt2ojmjptpl.html

[U55] PHP：match 表达式
来源：http://www.52xcode.cn/Article/details/gt2lmphpovw.html

$s = match($x) { 1 => "一", default => "其他" };
来源：http://www.ydjk.org.cn/Article/details/gt2kdwmbjfe.html

[U56] PHP：命名参数
来源：http://www.52xcode.cn/Article/details/gt2zbtmnrmr.html

f(a: 1, b: 2)
来源：http://www.52xcode.cn/Article/details/gt2cisphvxe.html

[U57] PHP：字符串插值
来源：http://www.ydjk.org.cn/Article/details/gt2medpdstk.html

"值: {$a}"
来源：http://www.ydjk.org.cn/Article/details/gt2zqqcshmm.html

[U58] PHP：数组三件套
来源：http://www.52xcode.cn/Article/details/gt2zjwhkwtp.html

array_map($f, $a);  array_filter($a, $f);  array_reduce($a, $f, 0);
来源：http://www.52xcode.cn/Article/details/gt2litiwayv.html

[U59] PHP：自定义排序
来源：http://www.52xcode.cn/Article/details/gt2qqgqznwj.html

usort($arr, fn($a, $b) => $a["age"] <=> $b["age"]);
来源：http://www.52xcode.cn/Article/details/gt2ksokklup.html

[U60] PHP：JSON 编解码
来源：http://www.52xcode.cn/Article/details/gt2zkugrusg.html

json_encode($d, JSON_UNESCAPED_UNICODE);  json_decode($s, true);
来源：http://www.ydjk.org.cn/Article/details/gt2hjznbouc.html

[U61] PHP：正则
来源：http://www.ydjk.org.cn/Article/details/gt2nimeacld.html

preg_match('/(\d+)/', $s, $m);  preg_replace('/\d+/', '#', $s);
来源：http://www.52xcode.cn/Article/details/gt2ybcjfdjl.html

[U62] PHP：日期对象
来源：http://www.ydjk.org.cn/Article/details/gt2uxyrlnmv.html

(new DateTimeImmutable())->format("Y-m-d");
来源：http://www.52xcode.cn/Article/details/gt2jbrpnssa.html

[U63] PHP：文件读写
来源：http://www.52xcode.cn/Article/details/gt2alpjansl.html

file_get_contents($f);  file_put_contents($f, $data);
来源：http://www.ydjk.org.cn/Article/details/gt2dewbymcu.html

[U64] PHP：目录遍历
来源：http://www.52xcode.cn/Article/details/gt2gsbkdkkl.html

glob("dir/*.php");  scandir("dir");
来源：http://www.52xcode.cn/Article/details/gt2hkumyuba.html

[U65] PHP：会话
来源：http://www.ydjk.org.cn/Article/details/gt2pxabphue.html

session_start();  $_SESSION["uid"] = 1;
来源：http://www.52xcode.cn/Article/details/gt2eyeeztsm.html

[U66] PHP：设置 Cookie
来源：http://www.52xcode.cn/Article/details/gt2napmsqgl.html

setcookie("token", $v, ["httponly" => true, "samesite" => "Lax"]);
来源：http://www.52xcode.cn/Article/details/gt2miipzpwn.html

[U67] PHP：处理文件上传
来源：http://www.ydjk.org.cn/Article/details/gt2ibvtvcvd.html

$_FILES["file"]["tmp_name"] 与 move_uploaded_file()
来源：http://www.52xcode.cn/Article/details/gt2cwjuocyl.html

[U68] PHP：PDO 连接
来源：http://www.52xcode.cn/Article/details/gt2chtzswal.html

$pdo = new PDO("mysql:host=localhost;dbname=app", "root", "");
来源：http://www.ydjk.org.cn/Article/details/gt2rvxhsuco.html

[U69] PHP：PDO 预处理
来源：http://www.ydjk.org.cn/Article/details/gt2ioinxttl.html

$stmt = $pdo->prepare("SELECT * FROM users WHERE id = ?");  $stmt->execute([$id]);
来源：http://www.52xcode.cn/Article/details/gt2kgkfzljq.html

[U70] PHP：PDO 事务
来源：http://www.52xcode.cn/Article/details/gt2grnkxoro.html

$pdo->beginTransaction();  $pdo->commit();  $pdo->rollBack();
来源：http://www.ydjk.org.cn/Article/details/gt2sbsusxvz.html

[U71] PHP：抛出异常
来源：http://www.52xcode.cn/Article/details/gt2agdymxgu.html

throw new RuntimeException("失败", 500);
来源：http://www.52xcode.cn/Article/details/gt2imvdashv.html

[U72] PHP：写错误日志
来源：http://www.52xcode.cn/Article/details/gt2obcmqyhe.html

error_log("失败: " . $e->getMessage());
来源：http://www.ydjk.org.cn/Article/details/gt2nnevyfui.html

[U73] PHP：读取 ini 配置
来源：http://www.52xcode.cn/Article/details/gt2dlklvcut.html

parse_ini_file("config.ini", true)
来源：http://www.52xcode.cn/Article/details/gt2djplyzlc.html

[U74] PHP：读取环境变量
来源：http://www.52xcode.cn/Article/details/gt2rjywsqnv.html

getenv("APP_ENV") ?: "production"
来源：http://www.52xcode.cn/Article/details/gt2zbovcntf.html

[U75] PHP：依赖注入
来源：http://www.ydjk.org.cn/Article/details/gt2rsohctne.html

composer require psr/container
来源：http://www.52xcode.cn/Article/details/gt2ombfaqcl.html

[U76] PHP：简单路由
来源：http://www.ydjk.org.cn/Article/details/gt2ysfwycyd.html

$path = parse_url($_SERVER["REQUEST_URI"], PHP_URL_PATH);
来源：http://www.ydjk.org.cn/Article/details/gt2smvpiway.html

[U77] PHP：模板渲染
来源：http://www.52xcode.cn/Article/details/gt2dnwqqqzy.html

composer require twig/twig
来源：http://www.ydjk.org.cn/Article/details/gt2ociqnuct.html

[U78] PHP：单元测试
来源：http://www.52xcode.cn/Article/details/gt2bslgdaxv.html

composer require --dev phpunit/phpunit
来源：http://www.ydjk.org.cn/Article/details/gt2clnlytuj.html

[U79] PHP：静态分析
来源：http://www.ydjk.org.cn/Article/details/gt2bbhknxht.html

composer require --dev phpstan/phpstan
来源：http://www.ydjk.org.cn/Article/details/gt2mutnvkqd.html

[U80] PHP：代码规范修复
来源：http://www.52xcode.cn/Article/details/gt2hlxrbten.html

composer require --dev friendsofphp/php-cs-fixer
来源：http://www.52xcode.cn/Article/details/gt2akjhtmuy.html

[U81] JS：初始化项目
来源：http://www.ydjk.org.cn/Article/details/gt2huqwwpao.html

npm init -y;  npm i express
来源：http://www.ydjk.org.cn/Article/details/gt2awyrzpee.html

[U82] JS：package.json 脚本
来源：http://www.ydjk.org.cn/Article/details/gt2bplyzhcr.html

"scripts": { "dev": "vite", "build": "vite build" }
来源：http://www.52xcode.cn/Article/details/gt2jdycdntk.html

[U83] JS：ES Module 导入导出
来源：http://www.ydjk.org.cn/Article/details/gt2aundamwu.html

export const a = 1;  import { a } from "./m.js";
来源：http://www.52xcode.cn/Article/details/gt2ifwvthts.html

[U84] JS：CommonJS 写法
来源：http://www.ydjk.org.cn/Article/details/gt2begdfrld.html

module.exports = { a };  const { a } = require("./m");
来源：http://www.ydjk.org.cn/Article/details/gt2bbkhvjgf.html

[U85] JS：可选链
来源：http://www.ydjk.org.cn/Article/details/gt2vcakkobe.html

a?.b?.c
来源：http://www.52xcode.cn/Article/details/gt2fxmfhznq.html

[U86] JS：空值合并
来源：http://www.52xcode.cn/Article/details/gt2bvshmobq.html

a ?? b
来源：http://www.52xcode.cn/Article/details/gt2fvmzarrn.html

[U87] JS：解构默认值
来源：http://www.52xcode.cn/Article/details/gt2yejctdkb.html

const { a = 1, b = 2 } = obj;
来源：http://www.52xcode.cn/Article/details/gt2jvittucq.html

[U88] JS：对象展开合并
来源：http://www.ydjk.org.cn/Article/details/gt2fuvsfkkq.html

{ ...a, ...b }
来源：http://www.ydjk.org.cn/Article/details/gt2qdpfwcig.html

[U89] JS：数组去重
来源：http://www.ydjk.org.cn/Article/details/gt2eqykzlng.html

[...new Set(arr)]
来源：http://www.ydjk.org.cn/Article/details/gt2qznanfzm.html

[U90] JS：数字数组排序
来源：http://www.52xcode.cn/Article/details/gt2zpebunsg.html

[...arr].sort((a, b) => a - b)
来源：http://www.ydjk.org.cn/Article/details/gt2jottjjsh.html

[U91] JS：对象键值遍历
来源：http://www.ydjk.org.cn/Article/details/gt2olkmbkmp.html

Object.entries(obj).forEach(([k, v]) => {});
来源：http://www.52xcode.cn/Article/details/gt2mprdzena.html

[U92] JS：深拷贝
来源：http://www.ydjk.org.cn/Article/details/gt2imiwizbm.html

structuredClone(obj)
来源：http://www.52xcode.cn/Article/details/gt2tsqqqkpl.html

[U93] JS：模板字符串
来源：http://www.52xcode.cn/Article/details/gt2zeaxhjub.html

`共 ${n} 条`
来源：http://www.ydjk.org.cn/Article/details/gt2jwghtddf.html

[U94] JS：箭头函数
来源：http://www.52xcode.cn/Article/details/gt2aithffqe.html

const double = x => x * 2;
来源：http://www.ydjk.org.cn/Article/details/gt2nitikcpd.html

[U95] JS：Promise 包装
来源：http://www.52xcode.cn/Article/details/gt2iixkdfse.html

new Promise((resolve, reject) => {})
来源：http://www.ydjk.org.cn/Article/details/gt2alkhrxja.html

[U96] JS：async/await 与异常
来源：http://www.52xcode.cn/Article/details/gt2nejicnnv.html

try { const d = await f(); } catch (e) { console.error(e); }
来源：http://www.52xcode.cn/Article/details/gt2lwkjmoql.html

[U97] JS：并发请求
来源：http://www.ydjk.org.cn/Article/details/gt2qbfngemm.html

await Promise.all(urls.map(u => fetch(u)))
来源：http://www.ydjk.org.cn/Article/details/gt2ygoimvde.html

[U98] JS：fetch 带 JSON
来源：http://www.ydjk.org.cn/Article/details/gt2uigrfnfj.html

await fetch(url, { method: "POST", headers: { "Content-Type": "application/json" }, body: JSON.stringify(d) })
来源：http://www.ydjk.org.cn/Article/details/gt2wfyvtnri.html

[U99] JS：事件监听
来源：http://www.ydjk.org.cn/Article/details/gt2fpodedbh.html

el.addEventListener("click", e => {})
来源：http://www.ydjk.org.cn/Article/details/gt2nbfpsakf.html

[U100] JS：DOM 查询
来源：http://www.ydjk.org.cn/Article/details/gt2bpmchxzq.html

document.querySelector(".item")
来源：http://www.ydjk.org.cn/Article/details/gt2giulxijz.html

[U101] JS：classList 操作
来源：http://www.52xcode.cn/Article/details/gt2uxgzhawu.html

el.classList.toggle("active")
来源：http://www.52xcode.cn/Article/details/gt2ccjjpzdy.html

[U102] JS：本地存储
来源：http://www.52xcode.cn/Article/details/gt2ovswmpge.html

localStorage.setItem("k", JSON.stringify(v))
来源：http://www.ydjk.org.cn/Article/details/gt2shnnhcdq.html

[U103] JS：定时器
来源：http://www.ydjk.org.cn/Article/details/gt2gchxlusp.html

setTimeout(fn, 1000);  setInterval(fn, 1000);
来源：http://www.52xcode.cn/Article/details/gt2cypjeasl.html

[U104] JS：防抖
来源：http://www.52xcode.cn/Article/details/gt2kntcuuxs.html

const debounce = (fn, ms) => { let t; return (...a) => { clearTimeout(t); t = setTimeout(() => fn(...a), ms); }; };
来源：http://www.52xcode.cn/Article/details/gt2luxmgwdb.html

[U105] JS：节流
来源：http://www.ydjk.org.cn/Article/details/gt2mozilwop.html

const throttle = (fn, ms) => { let last = 0; return (...a) => { const n = Date.now(); if (n - last >= ms) { last = n; fn(...a); } }; };
来源：http://www.ydjk.org.cn/Article/details/gt2sqnyqeib.html

[U106] JS：日期格式化
来源：http://www.52xcode.cn/Article/details/gt2uafrzsnu.html

new Intl.DateTimeFormat("zh-CN", { dateStyle: "medium" }).format(new Date())
来源：http://www.52xcode.cn/Article/details/gt2wreglasp.html

[U107] JS：数字千分位
来源：http://www.52xcode.cn/Article/details/gt2xupnguhb.html

new Intl.NumberFormat("en-US").format(1234567)
来源：http://www.52xcode.cn/Article/details/gt2leoiskis.html

[U108] JS：随机整数
来源：http://www.52xcode.cn/Article/details/gt2nsrgqkfl.html

Math.floor(Math.random() * (max - min + 1)) + min
来源：http://www.ydjk.org.cn/Article/details/gt2fmuzrcsh.html

[U109] JS：数组分组
来源：http://www.52xcode.cn/Article/details/gt2sfszqqsj.html

Object.groupBy(arr, x => x.type)
来源：http://www.52xcode.cn/Article/details/gt2wrnxeyot.html

[U110] JS：数组分块
来源：http://www.52xcode.cn/Article/details/gt2bhlngsfy.html

arr.reduce((acc, x, i) => (i % size ? acc : [...acc, arr.slice(i, i + size)]), [])
来源：http://www.ydjk.org.cn/Article/details/gt2jaoeueme.html

[U111] JS：对象转 Map
来源：http://www.ydjk.org.cn/Article/details/gt2kemynbig.html

new Map(Object.entries(obj))
来源：http://www.ydjk.org.cn/Article/details/gt2tocjkxeu.html

[U112] JS：字符串补位
来源：http://www.52xcode.cn/Article/details/gt2vdqsjgoi.html

"7".padStart(3, "0")
来源：http://www.ydjk.org.cn/Article/details/gt2kvqypzua.html

[U113] JS：正则替换全部
来源：http://www.ydjk.org.cn/Article/details/gt2corujdny.html

s.replaceAll("a", "b")
来源：http://www.52xcode.cn/Article/details/gt2doxnahcq.html

[U114] JS：JSON 深比较
来源：http://www.52xcode.cn/Article/details/gt2jnkfekfb.html

JSON.stringify(a) === JSON.stringify(b)
来源：http://www.52xcode.cn/Article/details/gt2amnggcih.html

[U115] JS：生成 UUID
来源：http://www.ydjk.org.cn/Article/details/gt2skhqftxi.html

crypto.randomUUID()
来源：http://www.52xcode.cn/Article/details/gt2hulwxopd.html

[U116] JS：类型检查（JSDoc）
来源：http://www.ydjk.org.cn/Article/details/gt2znbjogog.html

/** @param {string} name */ function f(name) {}
来源：http://www.52xcode.cn/Article/details/gt2fzikfurf.html

[U117] JS：单元测试
来源：http://www.52xcode.cn/Article/details/gt2orowitbr.html

npm i -D vitest;  npx vitest
来源：http://www.52xcode.cn/Article/details/gt2uhiovklc.html

[U118] JS：开发服务器
来源：http://www.ydjk.org.cn/Article/details/gt2prusflxh.html

npm i -D vite;  npx vite
来源：http://www.ydjk.org.cn/Article/details/gt2tyysowzz.html

[U119] JS：生产构建
来源：http://www.52xcode.cn/Article/details/gt2rewtksxx.html

npx vite build
来源：http://www.ydjk.org.cn/Article/details/gt2lqgnszlz.html

[U120] JS：读取环境变量（Vite）
来源：http://www.52xcode.cn/Article/details/gt2jjvpxiqj.html

import.meta.env.VITE_API_URL
来源：http://www.52xcode.cn/Article/details/gt2gkbavpwz.html

================================================================================
来源：http://www.ydjk.org.cn/Article/details/gt2edybyert.html

统计汇总
来源：http://www.52xcode.cn/Article/details/gt2squfeycb.html

================================================================================
来源：http://www.52xcode.cn/Article/details/gt2muxivpiq.html

按语言统计（条）：
来源：http://www.52xcode.cn/Article/details/gt2nexudyxe.html

Python ......... 252
来源：http://www.52xcode.cn/Article/details/gt2bhioaluc.html

PHP ............ 252
来源：http://www.ydjk.org.cn/Article/details/gt2fhkllugq.html

JavaScript ..... 252
来源：http://www.52xcode.cn/Article/details/gt2liziccna.html

TypeScript ..... 212
来源：http://www.52xcode.cn/Article/details/gt2ogzinjwd.html

Java ........... 212
来源：http://www.52xcode.cn/Article/details/gt2epfciphv.html

Go ............. 212
来源：http://www.52xcode.cn/Article/details/gt2imkbyohs.html

Ruby ........... 212
来源：http://www.ydjk.org.cn/Article/details/gt2kzdohqhg.html

C# ............. 212
来源：http://www.52xcode.cn/Article/details/gt2rvbzjfws.html

C .............. 30
来源：http://www.52xcode.cn/Article/details/gt2vbxpsukc.html

C++ ............ 30
来源：http://www.52xcode.cn/Article/details/gt2ixcnruwc.html

SQL ............ 90
来源：http://www.ydjk.org.cn/Article/details/gt2oyounxeu.html

Bash ........... 80
来源：http://www.ydjk.org.cn/Article/details/gt2iwkogghj.html

Kotlin ......... 15
来源：http://www.52xcode.cn/Article/details/gt2ylsiwpjn.html

Swift .......... 15
来源：http://www.ydjk.org.cn/Article/details/gt2dfldbikh.html

Lua ............ 10
来源：http://www.ydjk.org.cn/Article/details/gt2rodnwpkm.html

Perl ........... 10
来源：http://www.52xcode.cn/Article/details/gt2kqmulqwc.html

Scala .......... 10
来源：http://www.ydjk.org.cn/Article/details/gt2pfphzmgc.html

------------------------------------
来源：http://www.ydjk.org.cn/Article/details/gt2yswcgarf.html

合计 ........... 2106 条
来源：http://www.ydjk.org.cn/Article/details/gt2ctoolyed.html

按章节统计：
来源：http://www.ydjk.org.cn/Article/details/gt2lmqpoxcv.html

A 基础语法与类型       26 个任务 × 8 语言 =  208
来源：http://www.ydjk.org.cn/Article/details/gt2ujseoegt.html

B 流程控制             16 个任务 × 8 语言 =  128
来源：http://www.ydjk.org.cn/Article/details/gt2eboschuo.html

C 函数与作用域         16 个任务 × 8 语言 =  128
来源：http://www.52xcode.cn/Article/details/gt2aokhuyjf.html

D 数组 / 列表 / 集合   26 个任务 × 8 语言 =  208
来源：http://www.ydjk.org.cn/Article/details/gt2rwrnnitc.html

E 字符串处理           22 个任务 × 8 语言 =  176
来源：http://www.ydjk.org.cn/Article/details/gt2vcztiude.html

F 文件与目录           12 个任务 × 8 语言 =   96
来源：http://www.52xcode.cn/Article/details/gt2exoowcql.html

G 面向对象             16 个任务 × 8 语言 =  128
来源：http://www.ydjk.org.cn/Article/details/gt2uhlvoicr.html

H 异常与错误处理       10 个任务 × 8 语言 =   80
来源：http://www.52xcode.cn/Article/details/gt2imocukiv.html

I 正则表达式            8 个任务 × 8 语言 =   64
来源：http://www.ydjk.org.cn/Article/details/gt2pgzmqliw.html

J 日期与时间           10 个任务 × 8 语言 =   80
来源：http://www.ydjk.org.cn/Article/details/gt2dmofpzcd.html

K JSON 与序列化         8 个任务 × 8 语言 =   64
来源：http://www.52xcode.cn/Article/details/gt2mignnyyk.html

L 网络请求              8 个任务 × 8 语言 =   64
来源：http://www.52xcode.cn/Article/details/gt2xgmckdfw.html

M 命令行 / 进程         8 个任务 × 8 语言 =   64
来源：http://www.52xcode.cn/Article/details/gt2zvsjgejn.html

N 数据结构与算法       12 个任务 × 8 语言 =   96
来源：http://www.52xcode.cn/Article/details/gt2kaciwgvj.html

O 并发与异步            6 个任务 × 8 语言 =   48
来源：http://www.ydjk.org.cn/Article/details/gt2gdrpstbf.html

P 常用工具函数          8 个任务 × 8 语言 =   64
来源：http://www.ydjk.org.cn/Article/details/gt2svqvklso.html

Q SQL 专题                              90
来源：http://www.52xcode.cn/Article/details/gt2ylaqpxdr.html

R Bash 专题                             80
来源：http://www.52xcode.cn/Article/details/gt2nzfjxabq.html

S C / C++ 专题                          60
来源：http://www.52xcode.cn/Article/details/gt2ekxaakob.html

T 其他语言补充                          60
来源：http://www.ydjk.org.cn/Article/details/gt2kihgyava.html


<!-- 参考信息 -->