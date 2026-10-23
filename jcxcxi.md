代发 wailian999

while (my $line = <$fh>) { print $line; }
来源：http://www.52xcode.cn/Article/details/gt3vijtogmy.html

[T51] Scala：Hello World
来源：http://www.52xcode.cn/Article/details/gt3jplahujb.html

println("Hello")
来源：http://www.ydjk.org.cn/Article/details/gt3buylccxk.html

[T52] Scala：变量
来源：http://www.ydjk.org.cn/Article/details/gt3yopadyjb.html

val a = 1;  var b = 2
来源：http://www.52xcode.cn/Article/details/gt3zlyvaxnb.html

[T53] Scala：字符串插值
来源：http://www.ydjk.org.cn/Article/details/gt3ldoqkvkj.html

s"值: $b"
来源：http://www.ydjk.org.cn/Article/details/gt3femsqtch.html

[T54] Scala：集合映射
来源：http://www.ydjk.org.cn/Article/details/gt3yftuyrff.html

List(1, 2, 3).map(_ * 2)
来源：http://www.52xcode.cn/Article/details/gt3yulklfid.html

[T55] Scala：集合过滤
来源：http://www.52xcode.cn/Article/details/gt3gabmdlhl.html

List(1, 2, 3).filter(_ > 1)
来源：http://www.ydjk.org.cn/Article/details/gt3scdzhjdl.html

[T56] Scala：样例类
来源：http://www.ydjk.org.cn/Article/details/gt3lsxsudgk.html

case class User(name: String, age: Int)
来源：http://www.52xcode.cn/Article/details/gt3yusisbvm.html

[T57] Scala：模式匹配
来源：http://www.ydjk.org.cn/Article/details/gt3vqiutcru.html

x match { case 1 => "一"; case _ => "其他" }
来源：http://www.ydjk.org.cn/Article/details/gt3bljzdojy.html

[T58] Scala：函数定义
来源：http://www.52xcode.cn/Article/details/gt3aalepkdc.html

def add(a: Int, b: Int): Int = a + b
来源：http://www.ydjk.org.cn/Article/details/gt3qeqnvvaa.html

[T59] Scala：循环
来源：http://www.52xcode.cn/Article/details/gt3xzzaaeek.html

for (i <- 1 to 10) println(i)
来源：http://www.ydjk.org.cn/Article/details/gt3qtyupjme.html

[T60] Scala：折叠
来源：http://www.52xcode.cn/Article/details/gt3mdojhkyu.html

List(1, 2, 3).foldLeft(0)(_ + _)
来源：http://www.52xcode.cn/Article/details/gt3igslkhkd.html

================================================================================
来源：http://www.ydjk.org.cn/Article/details/gt3xilfsqty.html

U. 高频实用片段（Python / PHP / JavaScript 各 40 条）
来源：http://www.ydjk.org.cn/Article/details/gt3evxayxry.html

================================================================================
来源：http://www.ydjk.org.cn/Article/details/gt3jhojvfcr.html

[U01] Py：创建虚拟环境
来源：http://www.ydjk.org.cn/Article/details/gt3xjqfmvrc.html

python -m venv .venv && source .venv/bin/activate
来源：http://www.52xcode.cn/Article/details/gt3wisrscxe.html

[U02] Py：导出 / 安装依赖
来源：http://www.52xcode.cn/Article/details/gt3liboefkh.html

pip freeze > requirements.txt;  pip install -r requirements.txt
来源：http://www.ydjk.org.cn/Article/details/gt3mquybvzh.html

[U03] Py：加载 .env 配置
来源：http://www.ydjk.org.cn/Article/details/gt3awghcilf.html

from dotenv import load_dotenv; load_dotenv()
来源：http://www.ydjk.org.cn/Article/details/gt3lmtoiacv.html

[U04] Py：变量调试打印
来源：http://www.ydjk.org.cn/Article/details/gt3xesyjqnv.html

print(f"{x=}")            # 输出 x=值，Python 3.8+
来源：http://www.52xcode.cn/Article/details/gt3ryfjuwys.html

[U05] Py：列表去重且保序
来源：http://www.52xcode.cn/Article/details/gt3xkfzotct.html

list(dict.fromkeys(arr))
来源：http://www.ydjk.org.cn/Article/details/gt3cxrojfiq.html

[U06] Py：合并两个字典
来源：http://www.ydjk.org.cn/Article/details/gt3enpfitpd.html

{**a, **b}
来源：http://www.ydjk.org.cn/Article/details/gt3ehfbxokx.html

[U07] Py：反转字典键值
来源：http://www.ydjk.org.cn/Article/details/gt3xkenmary.html

{v: k for k, v in d.items()}
来源：http://www.ydjk.org.cn/Article/details/gt3ohzxzglk.html

[U08] Py：展平二维列表
来源：http://www.52xcode.cn/Article/details/gt3shyohocw.html

[y for x in nested for y in x]
来源：http://www.52xcode.cn/Article/details/gt3zqgiedsm.html

[U09] Py：字典取最大值的键
来源：http://www.52xcode.cn/Article/details/gt3ptpqkqna.html

max(d, key=d.get)
来源：http://www.52xcode.cn/Article/details/gt3yntmiuzn.html

[U10] Py：按值排序字典
来源：http://www.ydjk.org.cn/Article/details/gt3qtopgbew.html

dict(sorted(d.items(), key=lambda kv: kv[1]))
来源：http://www.ydjk.org.cn/Article/details/gt3midrkyvy.html

[U11] Py：生成器表达式
来源：http://www.52xcode.cn/Article/details/gt3wgctcujg.html

(x * 2 for x in arr)
来源：http://www.52xcode.cn/Article/details/gt3tiyqujzx.html

[U12] Py：取出现最多的 3 个元素
来源：http://www.52xcode.cn/Article/details/gt3xkgskute.html

Counter(arr).most_common(3)
来源：http://www.52xcode.cn/Article/details/gt3zjwuioaw.html

[U13] Py：固定长度队列
来源：http://www.52xcode.cn/Article/details/gt3pweyhlki.html

deque(maxlen=10)
来源：http://www.ydjk.org.cn/Article/details/gt3uvvteype.html

[U14] Py：分组收集到列表
来源：http://www.ydjk.org.cn/Article/details/gt3lorqqrxd.html

defaultdict(list)
来源：http://www.52xcode.cn/Article/details/gt3kguruflv.html

[U15] Py：高精度计时
来源：http://www.52xcode.cn/Article/details/gt3szbfzfgf.html

t = time.perf_counter()
来源：http://www.52xcode.cn/Article/details/gt3tmfifnmm.html

[U16] Py：命令行参数解析
来源：http://www.52xcode.cn/Article/details/gt3dhhbjbgn.html

ap = argparse.ArgumentParser();  ap.add_argument("--name");  args = ap.parse_args()
来源：http://www.52xcode.cn/Article/details/gt3jhyrnppr.html

[U17] Py：初始化日志
来源：http://www.52xcode.cn/Article/details/gt3lnwriasp.html

logging.basicConfig(level=logging.INFO)
来源：http://www.52xcode.cn/Article/details/gt3nsglkjbp.html

[U18] Py：预编译正则
来源：http://www.52xcode.cn/Article/details/gt3sxoxilzf.html

pat = re.compile(r"\d+")
来源：http://www.ydjk.org.cn/Article/details/gt3evosgyak.html

[U19] Py：正则替换带回调
来源：http://www.ydjk.org.cn/Article/details/gt3mxxxjeoy.html

re.sub(r"\d+", lambda m: str(int(m.group()) * 2), s)
来源：http://www.ydjk.org.cn/Article/details/gt3fotukwjz.html

[U20] Py：缓存函数结果
来源：http://www.ydjk.org.cn/Article/details/gt3fjeskqwm.html

@functools.lru_cache(maxsize=None)
来源：http://www.52xcode.cn/Article/details/gt3wolnsovd.html

[U21] Py：自定义上下文管理器
来源：http://www.ydjk.org.cn/Article/details/gt3sfkxmqta.html

@contextlib.contextmanager
来源：http://www.52xcode.cn/Article/details/gt3hhmbfgaz.html

[U22] Py：矩阵转置
来源：http://www.52xcode.cn/Article/details/gt3zmzauvtm.html

list(zip(*m))
来源：http://www.52xcode.cn/Article/details/gt3muoivomw.html

[U23] Py：分块读取大文件
来源：http://www.ydjk.org.cn/Article/details/gt3qwvxhyns.html

for chunk in iter(lambda: f.read(8192), b""):
来源：http://www.52xcode.cn/Article/details/gt3xiyvtiod.html

[U24] Py：路径操作
来源：http://www.52xcode.cn/Article/details/gt3ukjswdtw.html

Path("a/b.txt").parent.mkdir(parents=True, exist_ok=True)
来源：http://www.52xcode.cn/Article/details/gt3osvbzxbb.html

[U25] Py：CSV 按字典读
来源：http://www.52xcode.cn/Article/details/gt3ktvciwpt.html

csv.DictReader(f)
来源：http://www.52xcode.cn/Article/details/gt3yymgmmyq.html

[U26] Py：并发下载
来源：http://www.52xcode.cn/Article/details/gt3bzgnlvza.html

ThreadPoolExecutor(max_workers=8).map(fetch, urls)
来源：http://www.52xcode.cn/Article/details/gt3hzhrkize.html

[U27] Py：异步 HTTP
来源：http://www.52xcode.cn/Article/details/gt3otkzkxwz.html

aiohttp.ClientSession() 配合 async with
来源：http://www.ydjk.org.cn/Article/details/gt3ofrktihd.html

[U28] Py：类型别名
来源：http://www.52xcode.cn/Article/details/gt3gqloidkq.html

UserId = int
来源：http://www.ydjk.org.cn/Article/details/gt3cmemjqam.html

[U29] Py：属性校验
来源：http://www.ydjk.org.cn/Article/details/gt3utrhfbfy.html

@property 与 @x.setter 配合
来源：http://www.ydjk.org.cn/Article/details/gt3pxgpqbay.html

[U30] Py：数据类
来源：http://www.ydjk.org.cn/Article/details/gt3ahgzncoz.html

@dataclass(slots=True)
来源：http://www.ydjk.org.cn/Article/details/gt3vuqanqgd.html

[U31] Py：单测
来源：http://www.52xcode.cn/Article/details/gt3bfseuxzd.html

python -m pytest -q
来源：http://www.ydjk.org.cn/Article/details/gt3nmaysamt.html

[U32] Py：代码格式化
来源：http://www.ydjk.org.cn/Article/details/gt3ueceidzi.html

ruff format . && ruff check --fix .
来源：http://www.ydjk.org.cn/Article/details/gt3sclmvpqm.html

[U33] Py：打包发布
来源：http://www.ydjk.org.cn/Article/details/gt3wjujrkst.html

python -m build  （依赖 pyproject.toml）
来源：http://www.52xcode.cn/Article/details/gt3mnuzwpdy.html

[U34] Py：判断编码
来源：http://www.52xcode.cn/Article/details/gt3wdvwlqle.html

chardet.detect(raw)
来源：http://www.52xcode.cn/Article/details/gt3qapskkil.html

[U35] Py：发送邮件
来源：http://www.52xcode.cn/Article/details/gt3bmaazcqw.html

smtplib.SMTP_SSL(...).send_message(msg)
来源：http://www.52xcode.cn/Article/details/gt3ohsknslm.html

[U36] Py：定时任务
来源：http://www.52xcode.cn/Article/details/gt3pedicewt.html

schedule.every(10).minutes.do(job)
来源：http://www.ydjk.org.cn/Article/details/gt3wfleddsa.html

[U37] Py：读写 Excel
来源：http://www.52xcode.cn/Article/details/gt3xqrjjwhj.html

pandas.read_excel / DataFrame.to_excel
来源：http://www.ydjk.org.cn/Article/details/gt3zfqfucxm.html

[U38] Py：获取脚本所在目录
来源：http://www.ydjk.org.cn/Article/details/gt3mrevewiq.html

Path(__file__).resolve().parent
来源：http://www.ydjk.org.cn/Article/details/gt3bsarsvkn.html

[U39] Py：判断是否在交互环境
来源：http://www.ydjk.org.cn/Article/details/gt3iiolzwij.html

sys.stdout.isatty()
来源：http://www.52xcode.cn/Article/details/gt3pjwowxfd.html

[U40] Py：打印到标准错误
来源：http://www.52xcode.cn/Article/details/gt3gezjzyld.html

print("err", file=sys.stderr)
来源：http://www.52xcode.cn/Article/details/gt3xzaaplge.html

[U41] PHP：初始化 Composer 项目
来源：http://www.ydjk.org.cn/Article/details/gt3nctvoknb.html

composer init;  composer require guzzlehttp/guzzle
来源：http://www.52xcode.cn/Article/details/gt3xxhxrlfs.html

[U42] PHP：PSR-4 自动加载
来源：http://www.ydjk.org.cn/Article/details/gt3qqznkuvp.html

"autoload": { "psr-4": { "App\\": "src/" } }
来源：http://www.ydjk.org.cn/Article/details/gt3xsgmyxah.html

[U43] PHP：声明命名空间
来源：http://www.52xcode.cn/Article/details/gt3iwuduxjb.html

namespace App\Http;
来源：http://www.ydjk.org.cn/Article/details/gt3sqdjfyuc.html

[U44] PHP：开启严格类型
来源：http://www.52xcode.cn/Article/details/gt3vljuycfm.html

declare(strict_types=1);
来源：http://www.ydjk.org.cn/Article/details/gt3mlafenij.html

[U45] PHP：类型声明与返回类型
来源：http://www.52xcode.cn/Article/details/gt3iqczurem.html

function add(int $a, int $b): int { return $a + $b; }
来源：http://www.ydjk.org.cn/Article/details/gt3nxkvbtxq.html

[U46] PHP：可空类型
来源：http://www.52xcode.cn/Article/details/gt3xzdeimao.html

?string $name = null
来源：http://www.52xcode.cn/Article/details/gt3zdiyjlap.html

[U47] PHP：联合类型
来源：http://www.ydjk.org.cn/Article/details/gt3qqqfvxjb.html

int|string $id
来源：http://www.52xcode.cn/Article/details/gt3ugkwqyju.html

[U48] PHP：纯枚举
来源：http://www.ydjk.org.cn/Article/details/gt3heihrvcp.html

enum Status: string { case Active = "active"; case Off = "off"; }
来源：http://www.52xcode.cn/Article/details/gt3ttwcdgch.html

[U49] PHP：只读属性
来源：http://www.ydjk.org.cn/Article/details/gt3cspeqkfd.html

public readonly string $name
来源：http://www.52xcode.cn/Article/details/gt3aljgathi.html

[U50] PHP：构造器属性提升
来源：http://www.ydjk.org.cn/Article/details/gt3ssdluklx.html

public function __construct(private int $id) {}
来源：http://www.52xcode.cn/Article/details/gt3ouixigyl.html

[U51] PHP：数组解构
来源：http://www.52xcode.cn/Article/details/gt3njvibslh.html

[$a, $b] = $arr;
来源：http://www.52xcode.cn/Article/details/gt3ujlvsjwq.html

[U52] PHP：箭头函数
来源：http://www.52xcode.cn/Article/details/gt3zqawigej.html

$double = fn($x) => $x * 2;
来源：http://www.52xcode.cn/Article/details/gt3kdyxxkyz.html

[U53] PHP：空合并运算符
来源：http://www.ydjk.org.cn/Article/details/gt3hgkzvkin.html

$v = $a ?? $b ?? "default";
来源：http://www.ydjk.org.cn/Article/details/gt3hmxnmedn.html

[U54] PHP：空安全调用
来源：http://www.52xcode.cn/Article/details/gt3jomsujwl.html

$obj?->method()
来源：http://www.ydjk.org.cn/Article/details/gt3dtpkbulu.html

[U55] PHP：match 表达式
来源：http://www.ydjk.org.cn/Article/details/gt3blnblffx.html

$s = match($x) { 1 => "一", default => "其他" };
来源：http://www.ydjk.org.cn/Article/details/gt3vgthvzyv.html

[U56] PHP：命名参数
来源：http://www.52xcode.cn/Article/details/gt3ttnwrtuc.html

f(a: 1, b: 2)
来源：http://www.52xcode.cn/Article/details/gt3cxfyczgi.html

[U57] PHP：字符串插值
来源：http://www.ydjk.org.cn/Article/details/gt3bocilktb.html

"值: {$a}"
来源：http://www.52xcode.cn/Article/details/gt3sbnmirgz.html

[U58] PHP：数组三件套
来源：http://www.ydjk.org.cn/Article/details/gt3udigameo.html

array_map($f, $a);  array_filter($a, $f);  array_reduce($a, $f, 0);
来源：http://www.ydjk.org.cn/Article/details/gt3bnrktqtw.html

[U59] PHP：自定义排序
来源：http://www.52xcode.cn/Article/details/gt3ngtnbzed.html

usort($arr, fn($a, $b) => $a["age"] <=> $b["age"]);
来源：http://www.52xcode.cn/Article/details/gt3hkqxkylo.html

[U60] PHP：JSON 编解码
来源：http://www.52xcode.cn/Article/details/gt3wotupfyq.html

json_encode($d, JSON_UNESCAPED_UNICODE);  json_decode($s, true);
来源：http://www.52xcode.cn/Article/details/gt3lukvbaci.html

[U61] PHP：正则
来源：http://www.ydjk.org.cn/Article/details/gt3ahdipvjh.html

preg_match('/(\d+)/', $s, $m);  preg_replace('/\d+/', '#', $s);
来源：http://www.52xcode.cn/Article/details/gt3ntpkevkc.html

[U62] PHP：日期对象
来源：http://www.52xcode.cn/Article/details/gt3xmrzjxxm.html

(new DateTimeImmutable())->format("Y-m-d");
来源：http://www.ydjk.org.cn/Article/details/gt3ipmhushg.html

[U63] PHP：文件读写
来源：http://www.ydjk.org.cn/Article/details/gt3jwepdogt.html

file_get_contents($f);  file_put_contents($f, $data);
来源：http://www.ydjk.org.cn/Article/details/gt3fxigxfed.html

[U64] PHP：目录遍历
来源：http://www.52xcode.cn/Article/details/gt3lcykmygz.html

glob("dir/*.php");  scandir("dir");
来源：http://www.ydjk.org.cn/Article/details/gt3jkyxeorf.html

[U65] PHP：会话
来源：http://www.ydjk.org.cn/Article/details/gt3keymthqh.html

session_start();  $_SESSION["uid"] = 1;
来源：http://www.ydjk.org.cn/Article/details/gt3rgpgencw.html

[U66] PHP：设置 Cookie
来源：http://www.ydjk.org.cn/Article/details/gt3niiheebd.html

setcookie("token", $v, ["httponly" => true, "samesite" => "Lax"]);
来源：http://www.ydjk.org.cn/Article/details/gt3mznkujoq.html

[U67] PHP：处理文件上传
来源：http://www.ydjk.org.cn/Article/details/gt3bmcxshzs.html

$_FILES["file"]["tmp_name"] 与 move_uploaded_file()
来源：http://www.ydjk.org.cn/Article/details/gt3msvyndgp.html

[U68] PHP：PDO 连接
来源：http://www.ydjk.org.cn/Article/details/gt3mmdoirfe.html

$pdo = new PDO("mysql:host=localhost;dbname=app", "root", "");
来源：http://www.ydjk.org.cn/Article/details/gt3ccqgjtbm.html

[U69] PHP：PDO 预处理
来源：http://www.ydjk.org.cn/Article/details/gt3yihrdfts.html

$stmt = $pdo->prepare("SELECT * FROM users WHERE id = ?");  $stmt->execute([$id]);
来源：http://www.52xcode.cn/Article/details/gt3wtfphggr.html

[U70] PHP：PDO 事务
来源：http://www.ydjk.org.cn/Article/details/gt3ztlvvoby.html

$pdo->beginTransaction();  $pdo->commit();  $pdo->rollBack();
来源：http://www.ydjk.org.cn/Article/details/gt3odqpkbel.html

[U71] PHP：抛出异常
来源：http://www.52xcode.cn/Article/details/gt3fxgmyeba.html

throw new RuntimeException("失败", 500);
来源：http://www.52xcode.cn/Article/details/gt3oeoonkid.html

[U72] PHP：写错误日志
来源：http://www.ydjk.org.cn/Article/details/gt3jiskhtpj.html

error_log("失败: " . $e->getMessage());
来源：http://www.ydjk.org.cn/Article/details/gt3lbgzvlgx.html

[U73] PHP：读取 ini 配置
来源：http://www.52xcode.cn/Article/details/gt3bdifcpqy.html

parse_ini_file("config.ini", true)
来源：http://www.ydjk.org.cn/Article/details/gt3oadgbnfk.html

[U74] PHP：读取环境变量
来源：http://www.ydjk.org.cn/Article/details/gt3btwumabj.html

getenv("APP_ENV") ?: "production"
来源：http://www.52xcode.cn/Article/details/gt3doadmcxp.html

[U75] PHP：依赖注入
来源：http://www.ydjk.org.cn/Article/details/gt3jpnltrlt.html

composer require psr/container
来源：http://www.52xcode.cn/Article/details/gt3uimgbfdn.html

[U76] PHP：简单路由
来源：http://www.ydjk.org.cn/Article/details/gt3naysolie.html

$path = parse_url($_SERVER["REQUEST_URI"], PHP_URL_PATH);
来源：http://www.ydjk.org.cn/Article/details/gt3vuxyjodw.html

[U77] PHP：模板渲染
来源：http://www.52xcode.cn/Article/details/gt3plhyskng.html

composer require twig/twig
来源：http://www.ydjk.org.cn/Article/details/gt3vjpxtzhr.html

[U78] PHP：单元测试
来源：http://www.52xcode.cn/Article/details/gt3pnmhvmym.html

composer require --dev phpunit/phpunit
来源：http://www.52xcode.cn/Article/details/gt3zakdycwo.html

[U79] PHP：静态分析
来源：http://www.52xcode.cn/Article/details/gt3pguwbmlr.html

composer require --dev phpstan/phpstan
来源：http://www.52xcode.cn/Article/details/gt3rlpppbiu.html

[U80] PHP：代码规范修复
来源：http://www.ydjk.org.cn/Article/details/gt3sifbdpbw.html

composer require --dev friendsofphp/php-cs-fixer
来源：http://www.52xcode.cn/Article/details/gt3bnzggvqr.html

[U81] JS：初始化项目
来源：http://www.ydjk.org.cn/Article/details/gt3ffamtfvn.html

npm init -y;  npm i express
来源：http://www.ydjk.org.cn/Article/details/gt3gjhmnoue.html

[U82] JS：package.json 脚本
来源：http://www.52xcode.cn/Article/details/gt3nsqgkhxj.html

"scripts": { "dev": "vite", "build": "vite build" }
来源：http://www.ydjk.org.cn/Article/details/gt3tgzqgfiu.html

[U83] JS：ES Module 导入导出
来源：http://www.52xcode.cn/Article/details/gt3zffijggp.html

export const a = 1;  import { a } from "./m.js";
来源：http://www.ydjk.org.cn/Article/details/gt3ndgxhfgd.html

[U84] JS：CommonJS 写法
来源：http://www.ydjk.org.cn/Article/details/gt3vjehcfsl.html

module.exports = { a };  const { a } = require("./m");
来源：http://www.52xcode.cn/Article/details/gt3jnvajdzi.html

[U85] JS：可选链
来源：http://www.52xcode.cn/Article/details/gt3kqghxczz.html

a?.b?.c
来源：http://www.ydjk.org.cn/Article/details/gt3mtkwkios.html

[U86] JS：空值合并
来源：http://www.ydjk.org.cn/Article/details/gt3aavutzpn.html

a ?? b
来源：http://www.ydjk.org.cn/Article/details/gt3hmetnpzv.html

[U87] JS：解构默认值
来源：http://www.52xcode.cn/Article/details/gt3alijgsvj.html

const { a = 1, b = 2 } = obj;
来源：http://www.52xcode.cn/Article/details/gt3reuvqthp.html

[U88] JS：对象展开合并
来源：http://www.ydjk.org.cn/Article/details/gt3whzgsfqw.html

{ ...a, ...b }
来源：http://www.52xcode.cn/Article/details/gt3ezbralkh.html

[U89] JS：数组去重
来源：http://www.ydjk.org.cn/Article/details/gt3wafdtnpz.html

[...new Set(arr)]
来源：http://www.52xcode.cn/Article/details/gt3wqvwvjhu.html

[U90] JS：数字数组排序
来源：http://www.52xcode.cn/Article/details/gt3ilqizxob.html

[...arr].sort((a, b) => a - b)
来源：http://www.52xcode.cn/Article/details/gt3xsuzbtvl.html

[U91] JS：对象键值遍历
来源：http://www.ydjk.org.cn/Article/details/gt3prdtixeh.html

Object.entries(obj).forEach(([k, v]) => {});
来源：http://www.ydjk.org.cn/Article/details/gt3mwhgrjga.html

[U92] JS：深拷贝
来源：http://www.52xcode.cn/Article/details/gt3htnuidkc.html

structuredClone(obj)
来源：http://www.ydjk.org.cn/Article/details/gt3vqwptlan.html

[U93] JS：模板字符串
来源：http://www.ydjk.org.cn/Article/details/gt3psxreyuf.html

`共 ${n} 条`
来源：http://www.ydjk.org.cn/Article/details/gt3rlljckyf.html

[U94] JS：箭头函数
来源：http://www.ydjk.org.cn/Article/details/gt3ecbjqpqv.html

const double = x => x * 2;
来源：http://www.52xcode.cn/Article/details/gt3vpvejtmu.html

[U95] JS：Promise 包装
来源：http://www.52xcode.cn/Article/details/gt3itwtretb.html

new Promise((resolve, reject) => {})
来源：http://www.52xcode.cn/Article/details/gt3bhpguhyt.html

[U96] JS：async/await 与异常
来源：http://www.52xcode.cn/Article/details/gt3cmkkjqya.html

try { const d = await f(); } catch (e) { console.error(e); }
来源：http://www.ydjk.org.cn/Article/details/gt3unsvkxre.html

[U97] JS：并发请求
来源：http://www.ydjk.org.cn/Article/details/gt3ezpkxxiv.html

await Promise.all(urls.map(u => fetch(u)))
来源：http://www.ydjk.org.cn/Article/details/gt3mepdfrba.html

[U98] JS：fetch 带 JSON
来源：http://www.ydjk.org.cn/Article/details/gt3nhywumjs.html

await fetch(url, { method: "POST", headers: { "Content-Type": "application/json" }, body: JSON.stringify(d) })
来源：http://www.ydjk.org.cn/Article/details/gt3wwwtzkxf.html

[U99] JS：事件监听
来源：http://www.ydjk.org.cn/Article/details/gt3mqhbugcw.html

el.addEventListener("click", e => {})
来源：http://www.ydjk.org.cn/Article/details/gt3csqplowk.html

[U100] JS：DOM 查询
来源：http://www.ydjk.org.cn/Article/details/gt3wnpcmqow.html

document.querySelector(".item")
来源：http://www.52xcode.cn/Article/details/gt3mozflrtx.html

[U101] JS：classList 操作
来源：http://www.52xcode.cn/Article/details/gt3ccgurfev.html

el.classList.toggle("active")
来源：http://www.ydjk.org.cn/Article/details/gt3muwooojk.html

[U102] JS：本地存储
来源：http://www.52xcode.cn/Article/details/gt3wormvysj.html

localStorage.setItem("k", JSON.stringify(v))
来源：http://www.ydjk.org.cn/Article/details/gt3pyiuqrck.html

[U103] JS：定时器
来源：http://www.52xcode.cn/Article/details/gt3lqvqqunz.html

setTimeout(fn, 1000);  setInterval(fn, 1000);
来源：http://www.ydjk.org.cn/Article/details/gt3pdwwvtre.html

[U104] JS：防抖
来源：http://www.ydjk.org.cn/Article/details/gt3zydnrllc.html

const debounce = (fn, ms) => { let t; return (...a) => { clearTimeout(t); t = setTimeout(() => fn(...a), ms); }; };
来源：http://www.52xcode.cn/Article/details/gt3djppbegw.html

[U105] JS：节流
来源：http://www.52xcode.cn/Article/details/gt3ogkqizal.html

const throttle = (fn, ms) => { let last = 0; return (...a) => { const n = Date.now(); if (n - last >= ms) { last = n; fn(...a); } }; };
来源：http://www.ydjk.org.cn/Article/details/gt3csoimeoi.html

[U106] JS：日期格式化
来源：http://www.52xcode.cn/Article/details/gt3ckunqqxr.html

new Intl.DateTimeFormat("zh-CN", { dateStyle: "medium" }).format(new Date())
来源：http://www.ydjk.org.cn/Article/details/gt3wttepugb.html

[U107] JS：数字千分位
来源：http://www.ydjk.org.cn/Article/details/gt3bsmivgjk.html

new Intl.NumberFormat("en-US").format(1234567)
来源：http://www.52xcode.cn/Article/details/gt3nifyfvar.html

[U108] JS：随机整数
来源：http://www.52xcode.cn/Article/details/gt3ckoikecw.html

Math.floor(Math.random() * (max - min + 1)) + min
来源：http://www.ydjk.org.cn/Article/details/gt3orpgjeuk.html

[U109] JS：数组分组
来源：http://www.52xcode.cn/Article/details/gt3fokwjpdw.html

Object.groupBy(arr, x => x.type)
来源：http://www.52xcode.cn/Article/details/gt3nyljhvhe.html

[U110] JS：数组分块
来源：http://www.52xcode.cn/Article/details/gt3vmaiejbm.html

arr.reduce((acc, x, i) => (i % size ? acc : [...acc, arr.slice(i, i + size)]), [])
来源：http://www.ydjk.org.cn/Article/details/gt3clsakzga.html

[U111] JS：对象转 Map
来源：http://www.52xcode.cn/Article/details/gt3kuezmvys.html

new Map(Object.entries(obj))
来源：http://www.ydjk.org.cn/Article/details/gt3fsisarxg.html

[U112] JS：字符串补位
来源：http://www.52xcode.cn/Article/details/gt3sacwllyk.html

"7".padStart(3, "0")
来源：http://www.ydjk.org.cn/Article/details/gt3qsddvpti.html

[U113] JS：正则替换全部
来源：http://www.ydjk.org.cn/Article/details/gt3vorgbtkn.html

s.replaceAll("a", "b")
来源：http://www.52xcode.cn/Article/details/gt3imguasvi.html

[U114] JS：JSON 深比较
来源：http://www.52xcode.cn/Article/details/gt3bjdmgvoa.html

JSON.stringify(a) === JSON.stringify(b)
来源：http://www.52xcode.cn/Article/details/gt3zhjuvhbu.html

[U115] JS：生成 UUID
来源：http://www.ydjk.org.cn/Article/details/gt3rwvyawoi.html

crypto.randomUUID()
来源：http://www.ydjk.org.cn/Article/details/gt3hbbjlytl.html

[U116] JS：类型检查（JSDoc）
来源：http://www.52xcode.cn/Article/details/gt3fnzzoxzk.html

/** @param {string} name */ function f(name) {}
来源：http://www.52xcode.cn/Article/details/gt3rrixzlmf.html

[U117] JS：单元测试
来源：http://www.52xcode.cn/Article/details/gt3nunokjvj.html

npm i -D vitest;  npx vitest
来源：http://www.ydjk.org.cn/Article/details/gt3ckskqqom.html

[U118] JS：开发服务器
来源：http://www.ydjk.org.cn/Article/details/gt3supdkuyn.html

npm i -D vite;  npx vite
来源：http://www.52xcode.cn/Article/details/gt3linddsbd.html

[U119] JS：生产构建
来源：http://www.ydjk.org.cn/Article/details/gt3vfnoydud.html

npx vite build
来源：http://www.ydjk.org.cn/Article/details/gt3ueqjdbzx.html

[U120] JS：读取环境变量（Vite）
来源：http://www.ydjk.org.cn/Article/details/gt3wxdihzwj.html

import.meta.env.VITE_API_URL
来源：http://www.ydjk.org.cn/Article/details/gt3ipixzpxo.html

================================================================================
来源：http://www.ydjk.org.cn/Article/details/gt3sihnavbt.html

统计汇总
来源：http://www.ydjk.org.cn/Article/details/gt3vwdbtoaj.html

================================================================================
来源：http://www.52xcode.cn/Article/details/gt3viuskjux.html

按语言统计（条）：
来源：http://www.ydjk.org.cn/Article/details/gt3ttqmpwws.html

Python ......... 252
来源：http://www.ydjk.org.cn/Article/details/gt3lgfojoet.html

PHP ............ 252
来源：http://www.52xcode.cn/Article/details/gt3xrxpwfef.html

JavaScript ..... 252
来源：http://www.ydjk.org.cn/Article/details/gt3omssxsdf.html

TypeScript ..... 212
来源：http://www.52xcode.cn/Article/details/gt3ywmlcgao.html

Java ........... 212
来源：http://www.52xcode.cn/Article/details/gt3ktodrgkh.html

Go ............. 212
来源：http://www.52xcode.cn/Article/details/gt3hlxamuwr.html

Ruby ........... 212
来源：http://www.ydjk.org.cn/Article/details/gt3ywrrqvlu.html

C# ............. 212
来源：http://www.52xcode.cn/Article/details/gt3ypnedmyl.html

C .............. 30
来源：http://www.ydjk.org.cn/Article/details/gt3oploguni.html

C++ ............ 30
来源：http://www.52xcode.cn/Article/details/gt3yoeejxtt.html

SQL ............ 90
来源：http://www.ydjk.org.cn/Article/details/gt3bwcrfrai.html

Bash ........... 80
来源：http://www.52xcode.cn/Article/details/gt3egtftzdk.html

Kotlin ......... 15
来源：http://www.52xcode.cn/Article/details/gt3nhwjobva.html

Swift .......... 15
来源：http://www.52xcode.cn/Article/details/gt3mmlrvyuz.html

Lua ............ 10
来源：http://www.ydjk.org.cn/Article/details/gt3exocssqi.html

Perl ........... 10
来源：http://www.ydjk.org.cn/Article/details/gt3ezdqqcjo.html

Scala .......... 10
来源：http://www.ydjk.org.cn/Article/details/gt3dtkfiwst.html

------------------------------------
来源：http://www.ydjk.org.cn/Article/details/gt3rzzvpeea.html

合计 ........... 2106 条
来源：http://www.ydjk.org.cn/Article/details/gt3jrgqvepd.html

按章节统计：
来源：http://www.52xcode.cn/Article/details/gt3ymljxyzy.html

A 基础语法与类型       26 个任务 × 8 语言 =  208
来源：http://www.ydjk.org.cn/Article/details/gt3whyovdhi.html

B 流程控制             16 个任务 × 8 语言 =  128
来源：http://www.ydjk.org.cn/Article/details/gt3pbajdsrr.html

C 函数与作用域         16 个任务 × 8 语言 =  128
来源：http://www.ydjk.org.cn/Article/details/gt3dkadlotz.html

D 数组 / 列表 / 集合   26 个任务 × 8 语言 =  208
来源：http://www.ydjk.org.cn/Article/details/gt3ysbybpnn.html

E 字符串处理           22 个任务 × 8 语言 =  176
来源：http://www.52xcode.cn/Article/details/gt3jzzgaeuz.html

F 文件与目录           12 个任务 × 8 语言 =   96
来源：http://www.ydjk.org.cn/Article/details/gt3ozznsjam.html

G 面向对象             16 个任务 × 8 语言 =  128
来源：http://www.52xcode.cn/Article/details/gt3cuebneyo.html

H 异常与错误处理       10 个任务 × 8 语言 =   80
来源：http://www.52xcode.cn/Article/details/gt3wowdlbkh.html

I 正则表达式            8 个任务 × 8 语言 =   64
来源：http://www.ydjk.org.cn/Article/details/gt3kimgyqcj.html

J 日期与时间           10 个任务 × 8 语言 =   80
来源：http://www.52xcode.cn/Article/details/gt3xxaqfuwc.html

K JSON 与序列化         8 个任务 × 8 语言 =   64
来源：http://www.52xcode.cn/Article/details/gt3xwjuyrxe.html

L 网络请求              8 个任务 × 8 语言 =   64
来源：http://www.ydjk.org.cn/Article/details/gt3udqnhbug.html


<!-- 参考信息 -->