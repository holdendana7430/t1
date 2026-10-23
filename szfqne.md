代发 wailian999

[T49] Perl：函数
来源：http://www.ydjk.org.cn/Article/details/gt3eloidttw.html

sub add { my ($a, $b) = @_; return $a + $b; }
来源：http://www.52xcode.cn/Article/details/gt3jsjkejxp.html

[T50] Perl：逐行读文件
来源：http://www.52xcode.cn/Article/details/gt3hofrschh.html

open my $fh, "<", "a.txt" or die $!;
来源：http://www.52xcode.cn/Article/details/gt3vsonoecs.html

while (my $line = <$fh>) { print $line; }
来源：http://www.ydjk.org.cn/Article/details/gt3msxjcviz.html

[T51] Scala：Hello World
来源：http://www.ydjk.org.cn/Article/details/gt3jscwjgtv.html

println("Hello")
来源：http://www.52xcode.cn/Article/details/gt3sfultgvh.html

[T52] Scala：变量
来源：http://www.52xcode.cn/Article/details/gt3kdopgqao.html

val a = 1;  var b = 2
来源：http://www.52xcode.cn/Article/details/gt3ogsjcyot.html

[T53] Scala：字符串插值
来源：http://www.52xcode.cn/Article/details/gt3jpluthvp.html

s"值: $b"
来源：http://www.52xcode.cn/Article/details/gt3smjbqujj.html

[T54] Scala：集合映射
来源：http://www.ydjk.org.cn/Article/details/gt3hbexsegz.html

List(1, 2, 3).map(_ * 2)
来源：http://www.ydjk.org.cn/Article/details/gt3jcnrghba.html

[T55] Scala：集合过滤
来源：http://www.ydjk.org.cn/Article/details/gt3kfewwyvt.html

List(1, 2, 3).filter(_ > 1)
来源：http://www.ydjk.org.cn/Article/details/gt3ymkbtjlk.html

[T56] Scala：样例类
来源：http://www.52xcode.cn/Article/details/gt3wurkvxdf.html

case class User(name: String, age: Int)
来源：http://www.ydjk.org.cn/Article/details/gt3ylbgwcmg.html

[T57] Scala：模式匹配
来源：http://www.52xcode.cn/Article/details/gt3dwbrzbdy.html

x match { case 1 => "一"; case _ => "其他" }
来源：http://www.52xcode.cn/Article/details/gt3xbcuexfs.html

[T58] Scala：函数定义
来源：http://www.52xcode.cn/Article/details/gt3kpyxxrlf.html

def add(a: Int, b: Int): Int = a + b
来源：http://www.52xcode.cn/Article/details/gt3zjwtwzih.html

[T59] Scala：循环
来源：http://www.ydjk.org.cn/Article/details/gt3jenlrxcd.html

for (i <- 1 to 10) println(i)
来源：http://www.ydjk.org.cn/Article/details/gt3icvrcesa.html

[T60] Scala：折叠
来源：http://www.ydjk.org.cn/Article/details/gt3xeyuggwq.html

List(1, 2, 3).foldLeft(0)(_ + _)
来源：http://www.ydjk.org.cn/Article/details/gt3czumhevy.html

================================================================================
来源：http://www.52xcode.cn/Article/details/gt3fbnlrkzw.html

U. 高频实用片段（Python / PHP / JavaScript 各 40 条）
来源：http://www.ydjk.org.cn/Article/details/gt3dpkviikc.html

================================================================================
来源：http://www.ydjk.org.cn/Article/details/gt3eygacqds.html

[U01] Py：创建虚拟环境
来源：http://www.52xcode.cn/Article/details/gt3mjrqress.html

python -m venv .venv && source .venv/bin/activate
来源：http://www.ydjk.org.cn/Article/details/gt3hphgubfn.html

[U02] Py：导出 / 安装依赖
来源：http://www.52xcode.cn/Article/details/gt3qpdlyvqx.html

pip freeze > requirements.txt;  pip install -r requirements.txt
来源：http://www.ydjk.org.cn/Article/details/gt3rfoudkrw.html

[U03] Py：加载 .env 配置
来源：http://www.ydjk.org.cn/Article/details/gt3afitfvtx.html

from dotenv import load_dotenv; load_dotenv()
来源：http://www.ydjk.org.cn/Article/details/gt3hsjlipbx.html

[U04] Py：变量调试打印
来源：http://www.52xcode.cn/Article/details/gt3kgkpklkb.html

print(f"{x=}")            # 输出 x=值，Python 3.8+
来源：http://www.ydjk.org.cn/Article/details/gt3psgmtzhk.html

[U05] Py：列表去重且保序
来源：http://www.ydjk.org.cn/Article/details/gt3jjevevyd.html

list(dict.fromkeys(arr))
来源：http://www.52xcode.cn/Article/details/gt3tmgmhmes.html

[U06] Py：合并两个字典
来源：http://www.52xcode.cn/Article/details/gt3wsvuzhwi.html

{**a, **b}
来源：http://www.52xcode.cn/Article/details/gt3kjfjofyu.html

[U07] Py：反转字典键值
来源：http://www.52xcode.cn/Article/details/gt3zpgwpvpm.html

{v: k for k, v in d.items()}
来源：http://www.52xcode.cn/Article/details/gt3dfqvxpeb.html

[U08] Py：展平二维列表
来源：http://www.52xcode.cn/Article/details/gt3fxhabtcq.html

[y for x in nested for y in x]
来源：http://www.ydjk.org.cn/Article/details/gt3wskyqycb.html

[U09] Py：字典取最大值的键
来源：http://www.ydjk.org.cn/Article/details/gt3xwspovfo.html

max(d, key=d.get)
来源：http://www.ydjk.org.cn/Article/details/gt3bodenikn.html

[U10] Py：按值排序字典
来源：http://www.ydjk.org.cn/Article/details/gt3apedukrp.html

dict(sorted(d.items(), key=lambda kv: kv[1]))
来源：http://www.52xcode.cn/Article/details/gt3ifaynzei.html

[U11] Py：生成器表达式
来源：http://www.52xcode.cn/Article/details/gt3jsinozdw.html

(x * 2 for x in arr)
来源：http://www.ydjk.org.cn/Article/details/gt3shflbeck.html

[U12] Py：取出现最多的 3 个元素
来源：http://www.52xcode.cn/Article/details/gt3krflywbs.html

Counter(arr).most_common(3)
来源：http://www.ydjk.org.cn/Article/details/gt3payephgp.html

[U13] Py：固定长度队列
来源：http://www.52xcode.cn/Article/details/gt3fcfowgvc.html

deque(maxlen=10)
来源：http://www.ydjk.org.cn/Article/details/gt3uxmfbvte.html

[U14] Py：分组收集到列表
来源：http://www.52xcode.cn/Article/details/gt3oynvexpp.html

defaultdict(list)
来源：http://www.ydjk.org.cn/Article/details/gt3ybmmppoh.html

[U15] Py：高精度计时
来源：http://www.52xcode.cn/Article/details/gt3arvpnmig.html

t = time.perf_counter()
来源：http://www.ydjk.org.cn/Article/details/gt3yxqanfkt.html

[U16] Py：命令行参数解析
来源：http://www.ydjk.org.cn/Article/details/gt3licwzhnh.html

ap = argparse.ArgumentParser();  ap.add_argument("--name");  args = ap.parse_args()
来源：http://www.ydjk.org.cn/Article/details/gt3fvnsikqb.html

[U17] Py：初始化日志
来源：http://www.ydjk.org.cn/Article/details/gt3ppamsyog.html

logging.basicConfig(level=logging.INFO)
来源：http://www.52xcode.cn/Article/details/gt3puapdzqh.html

[U18] Py：预编译正则
来源：http://www.52xcode.cn/Article/details/gt3rxzzyuat.html

pat = re.compile(r"\d+")
来源：http://www.ydjk.org.cn/Article/details/gt3feynpyqy.html

[U19] Py：正则替换带回调
来源：http://www.ydjk.org.cn/Article/details/gt3bclijstm.html

re.sub(r"\d+", lambda m: str(int(m.group()) * 2), s)
来源：http://www.52xcode.cn/Article/details/gt3ixszkdgz.html

[U20] Py：缓存函数结果
来源：http://www.52xcode.cn/Article/details/gt3faafuhpm.html

@functools.lru_cache(maxsize=None)
来源：http://www.52xcode.cn/Article/details/gt3akpgzyne.html

[U21] Py：自定义上下文管理器
来源：http://www.ydjk.org.cn/Article/details/gt3evmnnkui.html

@contextlib.contextmanager
来源：http://www.52xcode.cn/Article/details/gt3qeqkgvzj.html

[U22] Py：矩阵转置
来源：http://www.ydjk.org.cn/Article/details/gt3xgbzaiel.html

list(zip(*m))
来源：http://www.ydjk.org.cn/Article/details/gt3beaiorcl.html

[U23] Py：分块读取大文件
来源：http://www.52xcode.cn/Article/details/gt3lrnlavse.html

for chunk in iter(lambda: f.read(8192), b""):
来源：http://www.ydjk.org.cn/Article/details/gt3nmrstutn.html

[U24] Py：路径操作
来源：http://www.52xcode.cn/Article/details/gt3evxidodw.html

Path("a/b.txt").parent.mkdir(parents=True, exist_ok=True)
来源：http://www.52xcode.cn/Article/details/gt3pkczirbm.html

[U25] Py：CSV 按字典读
来源：http://www.52xcode.cn/Article/details/gt3kmcpydyw.html

csv.DictReader(f)
来源：http://www.ydjk.org.cn/Article/details/gt3lsnzmwyk.html

[U26] Py：并发下载
来源：http://www.52xcode.cn/Article/details/gt3vzjmtdyc.html

ThreadPoolExecutor(max_workers=8).map(fetch, urls)
来源：http://www.52xcode.cn/Article/details/gt3uqengqwe.html

[U27] Py：异步 HTTP
来源：http://www.ydjk.org.cn/Article/details/gt3dcrazylm.html

aiohttp.ClientSession() 配合 async with
来源：http://www.52xcode.cn/Article/details/gt3jtmihifi.html

[U28] Py：类型别名
来源：http://www.52xcode.cn/Article/details/gt3zwzdbnig.html

UserId = int
来源：http://www.52xcode.cn/Article/details/gt3aqjrilum.html

[U29] Py：属性校验
来源：http://www.ydjk.org.cn/Article/details/gt3nkujgwuq.html

@property 与 @x.setter 配合
来源：http://www.52xcode.cn/Article/details/gt3jdrgcsqo.html

[U30] Py：数据类
来源：http://www.52xcode.cn/Article/details/gt3faspulvi.html

@dataclass(slots=True)
来源：http://www.ydjk.org.cn/Article/details/gt3gjwjvini.html

[U31] Py：单测
来源：http://www.ydjk.org.cn/Article/details/gt3aepkcwrp.html

python -m pytest -q
来源：http://www.ydjk.org.cn/Article/details/gt3uxcvrfyr.html

[U32] Py：代码格式化
来源：http://www.ydjk.org.cn/Article/details/gt3btnhtpfc.html

ruff format . && ruff check --fix .
来源：http://www.ydjk.org.cn/Article/details/gt3oujdnola.html

[U33] Py：打包发布
来源：http://www.52xcode.cn/Article/details/gt3ykywfcpg.html

python -m build  （依赖 pyproject.toml）
来源：http://www.52xcode.cn/Article/details/gt3indcourg.html

[U34] Py：判断编码
来源：http://www.52xcode.cn/Article/details/gt3fncebnhg.html

chardet.detect(raw)
来源：http://www.52xcode.cn/Article/details/gt3jzwbgwzp.html

[U35] Py：发送邮件
来源：http://www.ydjk.org.cn/Article/details/gt3isbrzfvj.html

smtplib.SMTP_SSL(...).send_message(msg)
来源：http://www.ydjk.org.cn/Article/details/gt3dpdaorbw.html

[U36] Py：定时任务
来源：http://www.ydjk.org.cn/Article/details/gt3awrewxiy.html

schedule.every(10).minutes.do(job)
来源：http://www.ydjk.org.cn/Article/details/gt3mtezskhy.html

[U37] Py：读写 Excel
来源：http://www.ydjk.org.cn/Article/details/gt3mdybgvjk.html

pandas.read_excel / DataFrame.to_excel
来源：http://www.52xcode.cn/Article/details/gt3pwqqqjlr.html

[U38] Py：获取脚本所在目录
来源：http://www.ydjk.org.cn/Article/details/gt3kjytenqu.html

Path(__file__).resolve().parent
来源：http://www.52xcode.cn/Article/details/gt3npacvhtm.html

[U39] Py：判断是否在交互环境
来源：http://www.ydjk.org.cn/Article/details/gt3kdhetwmq.html

sys.stdout.isatty()
来源：http://www.52xcode.cn/Article/details/gt3reosuqkl.html

[U40] Py：打印到标准错误
来源：http://www.52xcode.cn/Article/details/gt3czoschem.html

print("err", file=sys.stderr)
来源：http://www.ydjk.org.cn/Article/details/gt3ogbeehkx.html

[U41] PHP：初始化 Composer 项目
来源：http://www.ydjk.org.cn/Article/details/gt3ulcbbvgz.html

composer init;  composer require guzzlehttp/guzzle
来源：http://www.52xcode.cn/Article/details/gt3orshntom.html

[U42] PHP：PSR-4 自动加载
来源：http://www.52xcode.cn/Article/details/gt3gvlqzvvz.html

"autoload": { "psr-4": { "App\\": "src/" } }
来源：http://www.ydjk.org.cn/Article/details/gt3wmzwiqoh.html

[U43] PHP：声明命名空间
来源：http://www.ydjk.org.cn/Article/details/gt3utjzzwfu.html

namespace App\Http;
来源：http://www.ydjk.org.cn/Article/details/gt3ijdnskqi.html

[U44] PHP：开启严格类型
来源：http://www.52xcode.cn/Article/details/gt3apjuyoyk.html

declare(strict_types=1);
来源：http://www.ydjk.org.cn/Article/details/gt3fotywdji.html

[U45] PHP：类型声明与返回类型
来源：http://www.52xcode.cn/Article/details/gt3jkclpegv.html

function add(int $a, int $b): int { return $a + $b; }
来源：http://www.52xcode.cn/Article/details/gt3rhlxebld.html

[U46] PHP：可空类型
来源：http://www.ydjk.org.cn/Article/details/gt3ihjzikmv.html

?string $name = null
来源：http://www.ydjk.org.cn/Article/details/gt3ddfjwqlj.html

[U47] PHP：联合类型
来源：http://www.ydjk.org.cn/Article/details/gt3bozqbotx.html

int|string $id
来源：http://www.52xcode.cn/Article/details/gt3ghkrddlq.html

[U48] PHP：纯枚举
来源：http://www.ydjk.org.cn/Article/details/gt3axaorhoc.html

enum Status: string { case Active = "active"; case Off = "off"; }
来源：http://www.52xcode.cn/Article/details/gt3gfvuhrst.html

[U49] PHP：只读属性
来源：http://www.ydjk.org.cn/Article/details/gt3yakmxayd.html

public readonly string $name
来源：http://www.52xcode.cn/Article/details/gt3xilwhtfy.html

[U50] PHP：构造器属性提升
来源：http://www.52xcode.cn/Article/details/gt3trzoywws.html

public function __construct(private int $id) {}
来源：http://www.52xcode.cn/Article/details/gt3bzjkfsol.html

[U51] PHP：数组解构
来源：http://www.ydjk.org.cn/Article/details/gt3jjqfctka.html

[$a, $b] = $arr;
来源：http://www.52xcode.cn/Article/details/gt3msskvate.html

[U52] PHP：箭头函数
来源：http://www.ydjk.org.cn/Article/details/gt3imagaedx.html

$double = fn($x) => $x * 2;
来源：http://www.52xcode.cn/Article/details/gt3vqjlypmj.html

[U53] PHP：空合并运算符
来源：http://www.52xcode.cn/Article/details/gt3vgnfrdws.html

$v = $a ?? $b ?? "default";
来源：http://www.ydjk.org.cn/Article/details/gt3ekwwbzzw.html

[U54] PHP：空安全调用
来源：http://www.52xcode.cn/Article/details/gt3qxbadriw.html

$obj?->method()
来源：http://www.ydjk.org.cn/Article/details/gt3gvrxlwyu.html

[U55] PHP：match 表达式
来源：http://www.52xcode.cn/Article/details/gt3ptchvdft.html

$s = match($x) { 1 => "一", default => "其他" };
来源：http://www.ydjk.org.cn/Article/details/gt3wgipkpqi.html

[U56] PHP：命名参数
来源：http://www.52xcode.cn/Article/details/gt3ytagctmw.html

f(a: 1, b: 2)
来源：http://www.52xcode.cn/Article/details/gt3fwktgbmj.html

[U57] PHP：字符串插值
来源：http://www.ydjk.org.cn/Article/details/gt3acyzghrm.html

"值: {$a}"
来源：http://www.ydjk.org.cn/Article/details/gt3jvplneny.html

[U58] PHP：数组三件套
来源：http://www.ydjk.org.cn/Article/details/gt3lgbtfjdr.html

array_map($f, $a);  array_filter($a, $f);  array_reduce($a, $f, 0);
来源：http://www.52xcode.cn/Article/details/gt3vuzreqil.html

[U59] PHP：自定义排序
来源：http://www.52xcode.cn/Article/details/gt3udgvsxtj.html

usort($arr, fn($a, $b) => $a["age"] <=> $b["age"]);
来源：http://www.ydjk.org.cn/Article/details/gt3dxxtqirl.html

[U60] PHP：JSON 编解码
来源：http://www.52xcode.cn/Article/details/gt3jtakdjzr.html

json_encode($d, JSON_UNESCAPED_UNICODE);  json_decode($s, true);
来源：http://www.ydjk.org.cn/Article/details/gt3qogzoneo.html

[U61] PHP：正则
来源：http://www.52xcode.cn/Article/details/gt3nzppwhvp.html

preg_match('/(\d+)/', $s, $m);  preg_replace('/\d+/', '#', $s);
来源：http://www.ydjk.org.cn/Article/details/gt3qevffrla.html

[U62] PHP：日期对象
来源：http://www.52xcode.cn/Article/details/gt3fzfqiugx.html

(new DateTimeImmutable())->format("Y-m-d");
来源：http://www.ydjk.org.cn/Article/details/gt3ccxiovvy.html

[U63] PHP：文件读写
来源：http://www.ydjk.org.cn/Article/details/gt3bfvcseck.html

file_get_contents($f);  file_put_contents($f, $data);
来源：http://www.52xcode.cn/Article/details/gt3ddxgujgt.html

[U64] PHP：目录遍历
来源：http://www.ydjk.org.cn/Article/details/gt3tfhhpwhq.html

glob("dir/*.php");  scandir("dir");
来源：http://www.ydjk.org.cn/Article/details/gt3fkmfgdql.html

[U65] PHP：会话
来源：http://www.ydjk.org.cn/Article/details/gt3zlrehezk.html

session_start();  $_SESSION["uid"] = 1;
来源：http://www.52xcode.cn/Article/details/gt3dfvxvort.html

[U66] PHP：设置 Cookie
来源：http://www.52xcode.cn/Article/details/gt3dwemhfvk.html

setcookie("token", $v, ["httponly" => true, "samesite" => "Lax"]);
来源：http://www.52xcode.cn/Article/details/gt3rrmxlszv.html

[U67] PHP：处理文件上传
来源：http://www.ydjk.org.cn/Article/details/gt3xkecswvx.html

$_FILES["file"]["tmp_name"] 与 move_uploaded_file()
来源：http://www.ydjk.org.cn/Article/details/gt3zzpmspek.html

[U68] PHP：PDO 连接
来源：http://www.52xcode.cn/Article/details/gt3btsybgjm.html

$pdo = new PDO("mysql:host=localhost;dbname=app", "root", "");
来源：http://www.52xcode.cn/Article/details/gt3wajmkvrf.html

[U69] PHP：PDO 预处理
来源：http://www.52xcode.cn/Article/details/gt3cddnglni.html

$stmt = $pdo->prepare("SELECT * FROM users WHERE id = ?");  $stmt->execute([$id]);
来源：http://www.52xcode.cn/Article/details/gt3djbyjvmp.html

[U70] PHP：PDO 事务
来源：http://www.52xcode.cn/Article/details/gt3adodelta.html

$pdo->beginTransaction();  $pdo->commit();  $pdo->rollBack();
来源：http://www.52xcode.cn/Article/details/gt3bvhzwskh.html

[U71] PHP：抛出异常
来源：http://www.52xcode.cn/Article/details/gt3nteofwud.html

throw new RuntimeException("失败", 500);
来源：http://www.ydjk.org.cn/Article/details/gt3kwqaxcto.html

[U72] PHP：写错误日志
来源：http://www.52xcode.cn/Article/details/gt3eonbhuls.html

error_log("失败: " . $e->getMessage());
来源：http://www.52xcode.cn/Article/details/gt3lkxpakyp.html

[U73] PHP：读取 ini 配置
来源：http://www.ydjk.org.cn/Article/details/gt3wimgaqnp.html

parse_ini_file("config.ini", true)
来源：http://www.52xcode.cn/Article/details/gt3nqulfeoh.html

[U74] PHP：读取环境变量
来源：http://www.ydjk.org.cn/Article/details/gt3zwbqiogp.html

getenv("APP_ENV") ?: "production"
来源：http://www.ydjk.org.cn/Article/details/gt3gvlyxrka.html

[U75] PHP：依赖注入
来源：http://www.ydjk.org.cn/Article/details/gt3qzyfyrko.html

composer require psr/container
来源：http://www.52xcode.cn/Article/details/gt3vydvnteg.html

[U76] PHP：简单路由
来源：http://www.ydjk.org.cn/Article/details/gt3iujeidvm.html

$path = parse_url($_SERVER["REQUEST_URI"], PHP_URL_PATH);
来源：http://www.52xcode.cn/Article/details/gt3wypuohnh.html

[U77] PHP：模板渲染
来源：http://www.ydjk.org.cn/Article/details/gt3raahogen.html

composer require twig/twig
来源：http://www.52xcode.cn/Article/details/gt3tmnknkcu.html

[U78] PHP：单元测试
来源：http://www.52xcode.cn/Article/details/gt3fikmjojs.html

composer require --dev phpunit/phpunit
来源：http://www.ydjk.org.cn/Article/details/gt3xcapqcyl.html

[U79] PHP：静态分析
来源：http://www.ydjk.org.cn/Article/details/gt3ajogogmi.html

composer require --dev phpstan/phpstan
来源：http://www.ydjk.org.cn/Article/details/gt3yexuccdb.html

[U80] PHP：代码规范修复
来源：http://www.52xcode.cn/Article/details/gt3zuijkewl.html

composer require --dev friendsofphp/php-cs-fixer
来源：http://www.ydjk.org.cn/Article/details/gt3pkwucnld.html

[U81] JS：初始化项目
来源：http://www.52xcode.cn/Article/details/gt3rgtunzmx.html

npm init -y;  npm i express
来源：http://www.52xcode.cn/Article/details/gt3kgzquqyj.html

[U82] JS：package.json 脚本
来源：http://www.52xcode.cn/Article/details/gt3gfodgmps.html

"scripts": { "dev": "vite", "build": "vite build" }
来源：http://www.52xcode.cn/Article/details/gt3cknsiazq.html

[U83] JS：ES Module 导入导出
来源：http://www.ydjk.org.cn/Article/details/gt3cugsubhr.html

export const a = 1;  import { a } from "./m.js";
来源：http://www.52xcode.cn/Article/details/gt3vfuqqlxt.html

[U84] JS：CommonJS 写法
来源：http://www.52xcode.cn/Article/details/gt3mugequgb.html

module.exports = { a };  const { a } = require("./m");
来源：http://www.ydjk.org.cn/Article/details/gt3yvfwjflv.html

[U85] JS：可选链
来源：http://www.52xcode.cn/Article/details/gt3yjpbxbko.html

a?.b?.c
来源：http://www.52xcode.cn/Article/details/gt3exjrpaeg.html

[U86] JS：空值合并
来源：http://www.52xcode.cn/Article/details/gt3uglvuntt.html

a ?? b
来源：http://www.52xcode.cn/Article/details/gt3ikyeyfip.html

[U87] JS：解构默认值
来源：http://www.ydjk.org.cn/Article/details/gt3epvmhofa.html

const { a = 1, b = 2 } = obj;
来源：http://www.52xcode.cn/Article/details/gt3lrorcrkq.html

[U88] JS：对象展开合并
来源：http://www.52xcode.cn/Article/details/gt3nmjiiwar.html

{ ...a, ...b }
来源：http://www.ydjk.org.cn/Article/details/gt3pgzqfwmr.html

[U89] JS：数组去重
来源：http://www.52xcode.cn/Article/details/gt3yoyyelfm.html

[...new Set(arr)]
来源：http://www.ydjk.org.cn/Article/details/gt3uxmjmebb.html

[U90] JS：数字数组排序
来源：http://www.ydjk.org.cn/Article/details/gt3bfhrittn.html

[...arr].sort((a, b) => a - b)
来源：http://www.52xcode.cn/Article/details/gt3wxpaulcg.html

[U91] JS：对象键值遍历
来源：http://www.ydjk.org.cn/Article/details/gt3rwxccene.html

Object.entries(obj).forEach(([k, v]) => {});
来源：http://www.52xcode.cn/Article/details/gt3jbzujvsj.html

[U92] JS：深拷贝
来源：http://www.52xcode.cn/Article/details/gt3ozkrhokt.html

structuredClone(obj)
来源：http://www.ydjk.org.cn/Article/details/gt3iuhwunbd.html

[U93] JS：模板字符串
来源：http://www.ydjk.org.cn/Article/details/gt3fghehseh.html

`共 ${n} 条`
来源：http://www.52xcode.cn/Article/details/gt3vpenmyls.html

[U94] JS：箭头函数
来源：http://www.52xcode.cn/Article/details/gt3vciqlhjv.html

const double = x => x * 2;
来源：http://www.ydjk.org.cn/Article/details/gt3ftvbbbix.html

[U95] JS：Promise 包装
来源：http://www.52xcode.cn/Article/details/gt3vdxelata.html

new Promise((resolve, reject) => {})
来源：http://www.52xcode.cn/Article/details/gt3fgcytkok.html

[U96] JS：async/await 与异常
来源：http://www.52xcode.cn/Article/details/gt3tvifxljo.html

try { const d = await f(); } catch (e) { console.error(e); }
来源：http://www.ydjk.org.cn/Article/details/gt3ateddivf.html

[U97] JS：并发请求
来源：http://www.ydjk.org.cn/Article/details/gt3qnuktkwv.html

await Promise.all(urls.map(u => fetch(u)))
来源：http://www.52xcode.cn/Article/details/gt3hvedmlvi.html

[U98] JS：fetch 带 JSON
来源：http://www.ydjk.org.cn/Article/details/gt3uayhgpte.html

await fetch(url, { method: "POST", headers: { "Content-Type": "application/json" }, body: JSON.stringify(d) })
来源：http://www.52xcode.cn/Article/details/gt3vxarpcpo.html

[U99] JS：事件监听
来源：http://www.52xcode.cn/Article/details/gt3yeziyewm.html

el.addEventListener("click", e => {})
来源：http://www.ydjk.org.cn/Article/details/gt3xfhuueqy.html

[U100] JS：DOM 查询
来源：http://www.52xcode.cn/Article/details/gt3czwrohhl.html

document.querySelector(".item")
来源：http://www.52xcode.cn/Article/details/gt3ldcwpawb.html

[U101] JS：classList 操作
来源：http://www.ydjk.org.cn/Article/details/gt3pnpyxljc.html

el.classList.toggle("active")
来源：http://www.ydjk.org.cn/Article/details/gt3wiymlvfb.html

[U102] JS：本地存储
来源：http://www.ydjk.org.cn/Article/details/gt3jboledaa.html

localStorage.setItem("k", JSON.stringify(v))
来源：http://www.ydjk.org.cn/Article/details/gt3xiwxtitt.html

[U103] JS：定时器
来源：http://www.52xcode.cn/Article/details/gt3gsnqenvs.html

setTimeout(fn, 1000);  setInterval(fn, 1000);
来源：http://www.52xcode.cn/Article/details/gt3ggnfknbj.html

[U104] JS：防抖
来源：http://www.52xcode.cn/Article/details/gt3ftzmnljb.html

const debounce = (fn, ms) => { let t; return (...a) => { clearTimeout(t); t = setTimeout(() => fn(...a), ms); }; };
来源：http://www.ydjk.org.cn/Article/details/gt3bqbbkvsx.html

[U105] JS：节流
来源：http://www.ydjk.org.cn/Article/details/gt3sraskxka.html

const throttle = (fn, ms) => { let last = 0; return (...a) => { const n = Date.now(); if (n - last >= ms) { last = n; fn(...a); } }; };
来源：http://www.ydjk.org.cn/Article/details/gt3ihxnuviv.html

[U106] JS：日期格式化
来源：http://www.52xcode.cn/Article/details/gt3vicesfgz.html

new Intl.DateTimeFormat("zh-CN", { dateStyle: "medium" }).format(new Date())
来源：http://www.ydjk.org.cn/Article/details/gt3niegqgzm.html

[U107] JS：数字千分位
来源：http://www.52xcode.cn/Article/details/gt3yttigjwe.html

new Intl.NumberFormat("en-US").format(1234567)
来源：http://www.52xcode.cn/Article/details/gt3ltqgiqvx.html

[U108] JS：随机整数
来源：http://www.ydjk.org.cn/Article/details/gt3mwdutviz.html

Math.floor(Math.random() * (max - min + 1)) + min
来源：http://www.ydjk.org.cn/Article/details/gt3cdcfuyzk.html

[U109] JS：数组分组
来源：http://www.52xcode.cn/Article/details/gt3xezvoglz.html

Object.groupBy(arr, x => x.type)
来源：http://www.52xcode.cn/Article/details/gt3aujvytox.html

[U110] JS：数组分块
来源：http://www.ydjk.org.cn/Article/details/gt3bzatmznl.html

arr.reduce((acc, x, i) => (i % size ? acc : [...acc, arr.slice(i, i + size)]), [])
来源：http://www.52xcode.cn/Article/details/gt3dizwywoj.html

[U111] JS：对象转 Map
来源：http://www.ydjk.org.cn/Article/details/gt3nvcserqj.html

new Map(Object.entries(obj))
来源：http://www.ydjk.org.cn/Article/details/gt3vikfixsg.html

[U112] JS：字符串补位
来源：http://www.52xcode.cn/Article/details/gt3ehxayghw.html

"7".padStart(3, "0")
来源：http://www.52xcode.cn/Article/details/gt3uxnwqpqm.html

[U113] JS：正则替换全部
来源：http://www.52xcode.cn/Article/details/gt3locfijkl.html

s.replaceAll("a", "b")
来源：http://www.ydjk.org.cn/Article/details/gt3gtamcjhf.html

[U114] JS：JSON 深比较
来源：http://www.52xcode.cn/Article/details/gt3jdiqjizq.html

JSON.stringify(a) === JSON.stringify(b)
来源：http://www.ydjk.org.cn/Article/details/gt3xjltisup.html

[U115] JS：生成 UUID
来源：http://www.ydjk.org.cn/Article/details/gt3fvjejkgi.html

crypto.randomUUID()
来源：http://www.52xcode.cn/Article/details/gt3agsyuouj.html

[U116] JS：类型检查（JSDoc）
来源：http://www.52xcode.cn/Article/details/gt3wpsrcjqd.html

/** @param {string} name */ function f(name) {}
来源：http://www.52xcode.cn/Article/details/gt3tvrhnqda.html

[U117] JS：单元测试
来源：http://www.ydjk.org.cn/Article/details/gt3dmtdcbza.html

npm i -D vitest;  npx vitest
来源：http://www.52xcode.cn/Article/details/gt3peusnzzy.html

[U118] JS：开发服务器
来源：http://www.52xcode.cn/Article/details/gt3pgzlhbuh.html

npm i -D vite;  npx vite
来源：http://www.52xcode.cn/Article/details/gt3cysgzekc.html

[U119] JS：生产构建
来源：http://www.ydjk.org.cn/Article/details/gt3lrxnvaef.html

npx vite build
来源：http://www.ydjk.org.cn/Article/details/gt3yksytvyy.html

[U120] JS：读取环境变量（Vite）
来源：http://www.52xcode.cn/Article/details/gt3nyhxukfq.html

import.meta.env.VITE_API_URL
来源：http://www.52xcode.cn/Article/details/gt3bbhdtfst.html

================================================================================
来源：http://www.52xcode.cn/Article/details/gt3hzuuqhmt.html

统计汇总
来源：http://www.52xcode.cn/Article/details/gt3khxfubga.html

================================================================================
来源：http://www.ydjk.org.cn/Article/details/gt3ixritbyl.html

按语言统计（条）：
来源：http://www.ydjk.org.cn/Article/details/gt3gpmgobyq.html

Python ......... 252
来源：http://www.52xcode.cn/Article/details/gt3cuwbzbfk.html

PHP ............ 252
来源：http://www.ydjk.org.cn/Article/details/gt3wqipccpk.html

JavaScript ..... 252
来源：http://www.ydjk.org.cn/Article/details/gt3vjkkgjyw.html

TypeScript ..... 212
来源：http://www.52xcode.cn/Article/details/gt3zeajymwn.html

Java ........... 212
来源：http://www.ydjk.org.cn/Article/details/gt3vnqigeag.html

Go ............. 212
来源：http://www.52xcode.cn/Article/details/gt3gpacqrdi.html

Ruby ........... 212
来源：http://www.ydjk.org.cn/Article/details/gt3mmgjeqps.html

C# ............. 212
来源：http://www.ydjk.org.cn/Article/details/gt3xsmvdwwy.html

C .............. 30
来源：http://www.52xcode.cn/Article/details/gt3rycbayyo.html

C++ ............ 30
来源：http://www.ydjk.org.cn/Article/details/gt3rxdpfdsi.html

SQL ............ 90
来源：http://www.52xcode.cn/Article/details/gt3mzdxaulh.html

Bash ........... 80
来源：http://www.52xcode.cn/Article/details/gt3uaeqbwpt.html

Kotlin ......... 15
来源：http://www.52xcode.cn/Article/details/gt3asqzuvkf.html

Swift .......... 15
来源：http://www.ydjk.org.cn/Article/details/gt3reokoigr.html

Lua ............ 10
来源：http://www.ydjk.org.cn/Article/details/gt3btsoaprz.html

Perl ........... 10
来源：http://www.52xcode.cn/Article/details/gt3cnriozzh.html

Scala .......... 10
来源：http://www.ydjk.org.cn/Article/details/gt3tfpkzgbc.html

------------------------------------
来源：http://www.ydjk.org.cn/Article/details/gt3ubbncddp.html

合计 ........... 2106 条
来源：http://www.ydjk.org.cn/Article/details/gt3wsbuwajw.html

按章节统计：
来源：http://www.52xcode.cn/Article/details/gt3lrbaperp.html

A 基础语法与类型       26 个任务 × 8 语言 =  208
来源：http://www.52xcode.cn/Article/details/gt3tsnyxekr.html

B 流程控制             16 个任务 × 8 语言 =  128
来源：http://www.52xcode.cn/Article/details/gt3itwduiwq.html

C 函数与作用域         16 个任务 × 8 语言 =  128
来源：http://www.ydjk.org.cn/Article/details/gt3ghultqdu.html

D 数组 / 列表 / 集合   26 个任务 × 8 语言 =  208
来源：http://www.ydjk.org.cn/Article/details/gt3hxfvwczu.html

E 字符串处理           22 个任务 × 8 语言 =  176
来源：http://www.52xcode.cn/Article/details/gt3xbqdufok.html

F 文件与目录           12 个任务 × 8 语言 =   96
来源：http://www.52xcode.cn/Article/details/gt3luiwzzti.html

G 面向对象             16 个任务 × 8 语言 =  128
来源：http://www.52xcode.cn/Article/details/gt3osjvjvqd.html

H 异常与错误处理       10 个任务 × 8 语言 =   80
来源：http://www.ydjk.org.cn/Article/details/gt3eokizrtx.html


<!-- 参考信息 -->