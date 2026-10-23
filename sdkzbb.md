代发 wailian999

[T49] Perl：函数
来源：http://www.52xcode.cn/Article/details/gt3tveszstb.html

sub add { my ($a, $b) = @_; return $a + $b; }
来源：http://www.52xcode.cn/Article/details/gt3flmkijib.html

[T50] Perl：逐行读文件
来源：http://www.52xcode.cn/Article/details/gt3dysnkpcf.html

open my $fh, "<", "a.txt" or die $!;
来源：http://www.ydjk.org.cn/Article/details/gt3aztljyic.html

while (my $line = <$fh>) { print $line; }
来源：http://www.ydjk.org.cn/Article/details/gt3bryvciqp.html

[T51] Scala：Hello World
来源：http://www.ydjk.org.cn/Article/details/gt3aiadhhmx.html

println("Hello")
来源：http://www.52xcode.cn/Article/details/gt3wzisfszn.html

[T52] Scala：变量
来源：http://www.52xcode.cn/Article/details/gt3hdutgkni.html

val a = 1;  var b = 2
来源：http://www.52xcode.cn/Article/details/gt3rkpbpnxl.html

[T53] Scala：字符串插值
来源：http://www.ydjk.org.cn/Article/details/gt3lwarhbwx.html

s"值: $b"
来源：http://www.ydjk.org.cn/Article/details/gt3hasxtgke.html

[T54] Scala：集合映射
来源：http://www.52xcode.cn/Article/details/gt3myqnvjno.html

List(1, 2, 3).map(_ * 2)
来源：http://www.52xcode.cn/Article/details/gt3sxzfwarv.html

[T55] Scala：集合过滤
来源：http://www.52xcode.cn/Article/details/gt3nqjmnmqn.html

List(1, 2, 3).filter(_ > 1)
来源：http://www.52xcode.cn/Article/details/gt3rccswugd.html

[T56] Scala：样例类
来源：http://www.52xcode.cn/Article/details/gt3latuzqmd.html

case class User(name: String, age: Int)
来源：http://www.52xcode.cn/Article/details/gt3wuvqyisy.html

[T57] Scala：模式匹配
来源：http://www.52xcode.cn/Article/details/gt3pwvityxc.html

x match { case 1 => "一"; case _ => "其他" }
来源：http://www.52xcode.cn/Article/details/gt3veuhbsev.html

[T58] Scala：函数定义
来源：http://www.52xcode.cn/Article/details/gt3cquzemaa.html

def add(a: Int, b: Int): Int = a + b
来源：http://www.ydjk.org.cn/Article/details/gt3ankvzclb.html

[T59] Scala：循环
来源：http://www.ydjk.org.cn/Article/details/gt3fdizsrle.html

for (i <- 1 to 10) println(i)
来源：http://www.ydjk.org.cn/Article/details/gt3meblexty.html

[T60] Scala：折叠
来源：http://www.52xcode.cn/Article/details/gt3bxnwmhxz.html

List(1, 2, 3).foldLeft(0)(_ + _)
来源：http://www.ydjk.org.cn/Article/details/gt3qpegvodh.html

================================================================================
来源：http://www.52xcode.cn/Article/details/gt3vvaabcfx.html

U. 高频实用片段（Python / PHP / JavaScript 各 40 条）
来源：http://www.ydjk.org.cn/Article/details/gt3hvrclsoa.html

================================================================================
来源：http://www.52xcode.cn/Article/details/gt3ospaxqcp.html

[U01] Py：创建虚拟环境
来源：http://www.ydjk.org.cn/Article/details/gt3wrlghhzr.html

python -m venv .venv && source .venv/bin/activate
来源：http://www.52xcode.cn/Article/details/gt3hrfpzqrq.html

[U02] Py：导出 / 安装依赖
来源：http://www.ydjk.org.cn/Article/details/gt3xrzyxzrt.html

pip freeze > requirements.txt;  pip install -r requirements.txt
来源：http://www.52xcode.cn/Article/details/gt3qvtnrkui.html

[U03] Py：加载 .env 配置
来源：http://www.52xcode.cn/Article/details/gt3klrsyiwn.html

from dotenv import load_dotenv; load_dotenv()
来源：http://www.52xcode.cn/Article/details/gt3aritcmwn.html

[U04] Py：变量调试打印
来源：http://www.52xcode.cn/Article/details/gt3wyogcrmo.html

print(f"{x=}")            # 输出 x=值，Python 3.8+
来源：http://www.ydjk.org.cn/Article/details/gt3mhdsmcyk.html

[U05] Py：列表去重且保序
来源：http://www.52xcode.cn/Article/details/gt3dqigwsuu.html

list(dict.fromkeys(arr))
来源：http://www.52xcode.cn/Article/details/gt3moefmlao.html

[U06] Py：合并两个字典
来源：http://www.52xcode.cn/Article/details/gt3ckqwmuod.html

{**a, **b}
来源：http://www.ydjk.org.cn/Article/details/gt3pimherql.html

[U07] Py：反转字典键值
来源：http://www.ydjk.org.cn/Article/details/gt3eiyfnxdb.html

{v: k for k, v in d.items()}
来源：http://www.52xcode.cn/Article/details/gt3eztmympp.html

[U08] Py：展平二维列表
来源：http://www.ydjk.org.cn/Article/details/gt3vbflofsx.html

[y for x in nested for y in x]
来源：http://www.ydjk.org.cn/Article/details/gt3snuhghtf.html

[U09] Py：字典取最大值的键
来源：http://www.ydjk.org.cn/Article/details/gt3lqbgndfj.html

max(d, key=d.get)
来源：http://www.ydjk.org.cn/Article/details/gt3wpecofco.html

[U10] Py：按值排序字典
来源：http://www.52xcode.cn/Article/details/gt3efzhiyyu.html

dict(sorted(d.items(), key=lambda kv: kv[1]))
来源：http://www.52xcode.cn/Article/details/gt3gqzcvygx.html

[U11] Py：生成器表达式
来源：http://www.52xcode.cn/Article/details/gt3elsxqhrw.html

(x * 2 for x in arr)
来源：http://www.52xcode.cn/Article/details/gt3frecrrrb.html

[U12] Py：取出现最多的 3 个元素
来源：http://www.52xcode.cn/Article/details/gt3uxdcgrtk.html

Counter(arr).most_common(3)
来源：http://www.ydjk.org.cn/Article/details/gt3wwiqxhtr.html

[U13] Py：固定长度队列
来源：http://www.ydjk.org.cn/Article/details/gt3ntpugxlb.html

deque(maxlen=10)
来源：http://www.ydjk.org.cn/Article/details/gt3uesxzavd.html

[U14] Py：分组收集到列表
来源：http://www.ydjk.org.cn/Article/details/gt3bjfwnocd.html

defaultdict(list)
来源：http://www.ydjk.org.cn/Article/details/gt3ephuhism.html

[U15] Py：高精度计时
来源：http://www.52xcode.cn/Article/details/gt3pjswngmb.html

t = time.perf_counter()
来源：http://www.52xcode.cn/Article/details/gt3woxqlkvo.html

[U16] Py：命令行参数解析
来源：http://www.ydjk.org.cn/Article/details/gt3tbedwjfs.html

ap = argparse.ArgumentParser();  ap.add_argument("--name");  args = ap.parse_args()
来源：http://www.ydjk.org.cn/Article/details/gt3oyzntorr.html

[U17] Py：初始化日志
来源：http://www.52xcode.cn/Article/details/gt3mkatojiz.html

logging.basicConfig(level=logging.INFO)
来源：http://www.52xcode.cn/Article/details/gt3vlqmbcql.html

[U18] Py：预编译正则
来源：http://www.ydjk.org.cn/Article/details/gt3ggchcttm.html

pat = re.compile(r"\d+")
来源：http://www.52xcode.cn/Article/details/gt3tdqhtwrq.html

[U19] Py：正则替换带回调
来源：http://www.ydjk.org.cn/Article/details/gt3allkzboq.html

re.sub(r"\d+", lambda m: str(int(m.group()) * 2), s)
来源：http://www.ydjk.org.cn/Article/details/gt3qezicmso.html

[U20] Py：缓存函数结果
来源：http://www.52xcode.cn/Article/details/gt3pcukauej.html

@functools.lru_cache(maxsize=None)
来源：http://www.52xcode.cn/Article/details/gt3dsanqkgp.html

[U21] Py：自定义上下文管理器
来源：http://www.ydjk.org.cn/Article/details/gt3sywacyyd.html

@contextlib.contextmanager
来源：http://www.ydjk.org.cn/Article/details/gt3ogcocjmn.html

[U22] Py：矩阵转置
来源：http://www.52xcode.cn/Article/details/gt3lklbpbbl.html

list(zip(*m))
来源：http://www.52xcode.cn/Article/details/gt3gpbuopje.html

[U23] Py：分块读取大文件
来源：http://www.ydjk.org.cn/Article/details/gt3xnpjfbno.html

for chunk in iter(lambda: f.read(8192), b""):
来源：http://www.52xcode.cn/Article/details/gt3aentvxhn.html

[U24] Py：路径操作
来源：http://www.52xcode.cn/Article/details/gt3cpljxleb.html

Path("a/b.txt").parent.mkdir(parents=True, exist_ok=True)
来源：http://www.ydjk.org.cn/Article/details/gt3qkmnnpqd.html

[U25] Py：CSV 按字典读
来源：http://www.52xcode.cn/Article/details/gt3jttvndzf.html

csv.DictReader(f)
来源：http://www.52xcode.cn/Article/details/gt3ccurzooh.html

[U26] Py：并发下载
来源：http://www.ydjk.org.cn/Article/details/gt3ofmnthcq.html

ThreadPoolExecutor(max_workers=8).map(fetch, urls)
来源：http://www.ydjk.org.cn/Article/details/gt3iajffpyf.html

[U27] Py：异步 HTTP
来源：http://www.ydjk.org.cn/Article/details/gt3cvkcvfzz.html

aiohttp.ClientSession() 配合 async with
来源：http://www.52xcode.cn/Article/details/gt3pcfnznct.html

[U28] Py：类型别名
来源：http://www.ydjk.org.cn/Article/details/gt3ddonwgqd.html

UserId = int
来源：http://www.52xcode.cn/Article/details/gt3bpydgtmt.html

[U29] Py：属性校验
来源：http://www.52xcode.cn/Article/details/gt3qrxynlzr.html

@property 与 @x.setter 配合
来源：http://www.52xcode.cn/Article/details/gt3tujhczhe.html

[U30] Py：数据类
来源：http://www.ydjk.org.cn/Article/details/gt3eijmgbwk.html

@dataclass(slots=True)
来源：http://www.ydjk.org.cn/Article/details/gt3vsvqkoog.html

[U31] Py：单测
来源：http://www.52xcode.cn/Article/details/gt3ukzcibhz.html

python -m pytest -q
来源：http://www.52xcode.cn/Article/details/gt3pafbgckj.html

[U32] Py：代码格式化
来源：http://www.52xcode.cn/Article/details/gt3lwjnnrwm.html

ruff format . && ruff check --fix .
来源：http://www.52xcode.cn/Article/details/gt3ufluwkhs.html

[U33] Py：打包发布
来源：http://www.52xcode.cn/Article/details/gt3lnsutroe.html

python -m build  （依赖 pyproject.toml）
来源：http://www.52xcode.cn/Article/details/gt3apzkhufb.html

[U34] Py：判断编码
来源：http://www.52xcode.cn/Article/details/gt3vnocpdca.html

chardet.detect(raw)
来源：http://www.52xcode.cn/Article/details/gt3nbiedjqh.html

[U35] Py：发送邮件
来源：http://www.52xcode.cn/Article/details/gt3nnpnjjpm.html

smtplib.SMTP_SSL(...).send_message(msg)
来源：http://www.52xcode.cn/Article/details/gt3spfrlumw.html

[U36] Py：定时任务
来源：http://www.52xcode.cn/Article/details/gt3psazxjsx.html

schedule.every(10).minutes.do(job)
来源：http://www.52xcode.cn/Article/details/gt3pgnfmgcm.html

[U37] Py：读写 Excel
来源：http://www.52xcode.cn/Article/details/gt3roduvwzj.html

pandas.read_excel / DataFrame.to_excel
来源：http://www.ydjk.org.cn/Article/details/gt3xjnybkrl.html

[U38] Py：获取脚本所在目录
来源：http://www.52xcode.cn/Article/details/gt3mecqpxrv.html

Path(__file__).resolve().parent
来源：http://www.52xcode.cn/Article/details/gt3zqphcoqj.html

[U39] Py：判断是否在交互环境
来源：http://www.52xcode.cn/Article/details/gt3llixapst.html

sys.stdout.isatty()
来源：http://www.52xcode.cn/Article/details/gt3voevvjau.html

[U40] Py：打印到标准错误
来源：http://www.ydjk.org.cn/Article/details/gt3xsfpvsqs.html

print("err", file=sys.stderr)
来源：http://www.ydjk.org.cn/Article/details/gt3szbhjbcf.html

[U41] PHP：初始化 Composer 项目
来源：http://www.ydjk.org.cn/Article/details/gt3xwaknpkj.html

composer init;  composer require guzzlehttp/guzzle
来源：http://www.ydjk.org.cn/Article/details/gt3tiebqcws.html

[U42] PHP：PSR-4 自动加载
来源：http://www.ydjk.org.cn/Article/details/gt3qmupwjnc.html

"autoload": { "psr-4": { "App\\": "src/" } }
来源：http://www.52xcode.cn/Article/details/gt3hbxylsoz.html

[U43] PHP：声明命名空间
来源：http://www.ydjk.org.cn/Article/details/gt3feplvajh.html

namespace App\Http;
来源：http://www.52xcode.cn/Article/details/gt3pquthlky.html

[U44] PHP：开启严格类型
来源：http://www.ydjk.org.cn/Article/details/gt3smvcfwqi.html

declare(strict_types=1);
来源：http://www.52xcode.cn/Article/details/gt3jsewrhwe.html

[U45] PHP：类型声明与返回类型
来源：http://www.ydjk.org.cn/Article/details/gt3sutrhexa.html

function add(int $a, int $b): int { return $a + $b; }
来源：http://www.ydjk.org.cn/Article/details/gt3sfydonbg.html

[U46] PHP：可空类型
来源：http://www.52xcode.cn/Article/details/gt3blxloshw.html

?string $name = null
来源：http://www.ydjk.org.cn/Article/details/gt3blinlguc.html

[U47] PHP：联合类型
来源：http://www.52xcode.cn/Article/details/gt3qrbxdxmx.html

int|string $id
来源：http://www.52xcode.cn/Article/details/gt3kbtqxzrc.html

[U48] PHP：纯枚举
来源：http://www.52xcode.cn/Article/details/gt3nbifuvmi.html

enum Status: string { case Active = "active"; case Off = "off"; }
来源：http://www.ydjk.org.cn/Article/details/gt3ylajruac.html

[U49] PHP：只读属性
来源：http://www.52xcode.cn/Article/details/gt3excaxose.html

public readonly string $name
来源：http://www.52xcode.cn/Article/details/gt3shkjmivk.html

[U50] PHP：构造器属性提升
来源：http://www.ydjk.org.cn/Article/details/gt3ixhhupiy.html

public function __construct(private int $id) {}
来源：http://www.ydjk.org.cn/Article/details/gt3aevpxojb.html

[U51] PHP：数组解构
来源：http://www.ydjk.org.cn/Article/details/gt3hcnkupew.html

[$a, $b] = $arr;
来源：http://www.ydjk.org.cn/Article/details/gt3frtqdjvz.html

[U52] PHP：箭头函数
来源：http://www.52xcode.cn/Article/details/gt3gondsrje.html

$double = fn($x) => $x * 2;
来源：http://www.52xcode.cn/Article/details/gt3mkofwcdb.html

[U53] PHP：空合并运算符
来源：http://www.52xcode.cn/Article/details/gt3fumyxyvx.html

$v = $a ?? $b ?? "default";
来源：http://www.52xcode.cn/Article/details/gt3xxupfhse.html

[U54] PHP：空安全调用
来源：http://www.ydjk.org.cn/Article/details/gt3mkmgyozq.html

$obj?->method()
来源：http://www.ydjk.org.cn/Article/details/gt3xtjraqln.html

[U55] PHP：match 表达式
来源：http://www.ydjk.org.cn/Article/details/gt3vwwslsno.html

$s = match($x) { 1 => "一", default => "其他" };
来源：http://www.52xcode.cn/Article/details/gt3cdgutekq.html

[U56] PHP：命名参数
来源：http://www.ydjk.org.cn/Article/details/gt3eybxlufm.html

f(a: 1, b: 2)
来源：http://www.52xcode.cn/Article/details/gt3unpfdsht.html

[U57] PHP：字符串插值
来源：http://www.ydjk.org.cn/Article/details/gt3ehveoxvn.html

"值: {$a}"
来源：http://www.52xcode.cn/Article/details/gt3ssrjzzvx.html

[U58] PHP：数组三件套
来源：http://www.52xcode.cn/Article/details/gt3ovabpgqa.html

array_map($f, $a);  array_filter($a, $f);  array_reduce($a, $f, 0);
来源：http://www.ydjk.org.cn/Article/details/gt3pxvdlfkc.html

[U59] PHP：自定义排序
来源：http://www.ydjk.org.cn/Article/details/gt3zyytovxk.html

usort($arr, fn($a, $b) => $a["age"] <=> $b["age"]);
来源：http://www.52xcode.cn/Article/details/gt3rghnyjsn.html

[U60] PHP：JSON 编解码
来源：http://www.52xcode.cn/Article/details/gt3vfzvpkkx.html

json_encode($d, JSON_UNESCAPED_UNICODE);  json_decode($s, true);
来源：http://www.52xcode.cn/Article/details/gt3ccgcgafa.html

[U61] PHP：正则
来源：http://www.52xcode.cn/Article/details/gt3aezlgqsu.html

preg_match('/(\d+)/', $s, $m);  preg_replace('/\d+/', '#', $s);
来源：http://www.ydjk.org.cn/Article/details/gt3uvghgqba.html

[U62] PHP：日期对象
来源：http://www.ydjk.org.cn/Article/details/gt3qtubfwsn.html

(new DateTimeImmutable())->format("Y-m-d");
来源：http://www.52xcode.cn/Article/details/gt3abpouvwj.html

[U63] PHP：文件读写
来源：http://www.ydjk.org.cn/Article/details/gt3zejntvne.html

file_get_contents($f);  file_put_contents($f, $data);
来源：http://www.52xcode.cn/Article/details/gt3viqqaxxf.html

[U64] PHP：目录遍历
来源：http://www.52xcode.cn/Article/details/gt3egrootli.html

glob("dir/*.php");  scandir("dir");
来源：http://www.ydjk.org.cn/Article/details/gt3moihvyvo.html

[U65] PHP：会话
来源：http://www.ydjk.org.cn/Article/details/gt3skzdlqaq.html

session_start();  $_SESSION["uid"] = 1;
来源：http://www.52xcode.cn/Article/details/gt3oywjypes.html

[U66] PHP：设置 Cookie
来源：http://www.ydjk.org.cn/Article/details/gt3yswvbzxd.html

setcookie("token", $v, ["httponly" => true, "samesite" => "Lax"]);
来源：http://www.ydjk.org.cn/Article/details/gt3pqyvminp.html

[U67] PHP：处理文件上传
来源：http://www.ydjk.org.cn/Article/details/gt3ipqtvibq.html

$_FILES["file"]["tmp_name"] 与 move_uploaded_file()
来源：http://www.52xcode.cn/Article/details/gt3lqpxpvhb.html

[U68] PHP：PDO 连接
来源：http://www.ydjk.org.cn/Article/details/gt3ncignumr.html

$pdo = new PDO("mysql:host=localhost;dbname=app", "root", "");
来源：http://www.52xcode.cn/Article/details/gt3qzjbuvvh.html

[U69] PHP：PDO 预处理
来源：http://www.ydjk.org.cn/Article/details/gt3seosaziv.html

$stmt = $pdo->prepare("SELECT * FROM users WHERE id = ?");  $stmt->execute([$id]);
来源：http://www.ydjk.org.cn/Article/details/gt3swerpnhz.html

[U70] PHP：PDO 事务
来源：http://www.52xcode.cn/Article/details/gt3aulahqvy.html

$pdo->beginTransaction();  $pdo->commit();  $pdo->rollBack();
来源：http://www.52xcode.cn/Article/details/gt3hliyndzx.html

[U71] PHP：抛出异常
来源：http://www.52xcode.cn/Article/details/gt3mgbymjws.html

throw new RuntimeException("失败", 500);
来源：http://www.52xcode.cn/Article/details/gt3hsgpzxtd.html

[U72] PHP：写错误日志
来源：http://www.ydjk.org.cn/Article/details/gt3zfjqqekm.html

error_log("失败: " . $e->getMessage());
来源：http://www.52xcode.cn/Article/details/gt3ihxasypb.html

[U73] PHP：读取 ini 配置
来源：http://www.ydjk.org.cn/Article/details/gt3hgiwcfwu.html

parse_ini_file("config.ini", true)
来源：http://www.ydjk.org.cn/Article/details/gt3mowemjlv.html

[U74] PHP：读取环境变量
来源：http://www.52xcode.cn/Article/details/gt3atpkwiye.html

getenv("APP_ENV") ?: "production"
来源：http://www.ydjk.org.cn/Article/details/gt3hrofxdbx.html

[U75] PHP：依赖注入
来源：http://www.ydjk.org.cn/Article/details/gt3qopcjwce.html

composer require psr/container
来源：http://www.ydjk.org.cn/Article/details/gt3qxgswdkv.html

[U76] PHP：简单路由
来源：http://www.52xcode.cn/Article/details/gt3klidhdud.html

$path = parse_url($_SERVER["REQUEST_URI"], PHP_URL_PATH);
来源：http://www.52xcode.cn/Article/details/gt3mqhhrbya.html

[U77] PHP：模板渲染
来源：http://www.ydjk.org.cn/Article/details/gt3qhumorfs.html

composer require twig/twig
来源：http://www.52xcode.cn/Article/details/gt3mvisnfbx.html

[U78] PHP：单元测试
来源：http://www.ydjk.org.cn/Article/details/gt3ayfzulfh.html

composer require --dev phpunit/phpunit
来源：http://www.52xcode.cn/Article/details/gt3wkbaeemz.html

[U79] PHP：静态分析
来源：http://www.ydjk.org.cn/Article/details/gt3zudixdsi.html

composer require --dev phpstan/phpstan
来源：http://www.ydjk.org.cn/Article/details/gt3akaptxhq.html

[U80] PHP：代码规范修复
来源：http://www.52xcode.cn/Article/details/gt3qbwkdjku.html

composer require --dev friendsofphp/php-cs-fixer
来源：http://www.ydjk.org.cn/Article/details/gt3btvpjssv.html

[U81] JS：初始化项目
来源：http://www.52xcode.cn/Article/details/gt3qufcmuan.html

npm init -y;  npm i express
来源：http://www.ydjk.org.cn/Article/details/gt3bogtfkny.html

[U82] JS：package.json 脚本
来源：http://www.52xcode.cn/Article/details/gt3qbyubpmc.html

"scripts": { "dev": "vite", "build": "vite build" }
来源：http://www.52xcode.cn/Article/details/gt3mjgmflqc.html

[U83] JS：ES Module 导入导出
来源：http://www.52xcode.cn/Article/details/gt3sjolkwam.html

export const a = 1;  import { a } from "./m.js";
来源：http://www.52xcode.cn/Article/details/gt3qjiqtlht.html

[U84] JS：CommonJS 写法
来源：http://www.52xcode.cn/Article/details/gt3vdkohopp.html

module.exports = { a };  const { a } = require("./m");
来源：http://www.52xcode.cn/Article/details/gt3ghzbhbis.html

[U85] JS：可选链
来源：http://www.ydjk.org.cn/Article/details/gt3gvzwzfxq.html

a?.b?.c
来源：http://www.52xcode.cn/Article/details/gt3fzirtstw.html

[U86] JS：空值合并
来源：http://www.52xcode.cn/Article/details/gt3olrsjgfp.html

a ?? b
来源：http://www.ydjk.org.cn/Article/details/gt3sewqggah.html

[U87] JS：解构默认值
来源：http://www.ydjk.org.cn/Article/details/gt3uqomtuja.html

const { a = 1, b = 2 } = obj;
来源：http://www.52xcode.cn/Article/details/gt3owjjkfgg.html

[U88] JS：对象展开合并
来源：http://www.ydjk.org.cn/Article/details/gt3kkkiwrjd.html

{ ...a, ...b }
来源：http://www.ydjk.org.cn/Article/details/gt3cppdjbgz.html

[U89] JS：数组去重
来源：http://www.ydjk.org.cn/Article/details/gt3hvqilewv.html

[...new Set(arr)]
来源：http://www.ydjk.org.cn/Article/details/gt3ftadldvv.html

[U90] JS：数字数组排序
来源：http://www.52xcode.cn/Article/details/gt3socqndun.html

[...arr].sort((a, b) => a - b)
来源：http://www.52xcode.cn/Article/details/gt3thtglqqf.html

[U91] JS：对象键值遍历
来源：http://www.52xcode.cn/Article/details/gt3dbepyyqd.html

Object.entries(obj).forEach(([k, v]) => {});
来源：http://www.ydjk.org.cn/Article/details/gt3nrscsbxe.html

[U92] JS：深拷贝
来源：http://www.52xcode.cn/Article/details/gt3hdxteoyj.html

structuredClone(obj)
来源：http://www.52xcode.cn/Article/details/gt3cpnmmitt.html

[U93] JS：模板字符串
来源：http://www.ydjk.org.cn/Article/details/gt3gtinzwlx.html

`共 ${n} 条`
来源：http://www.52xcode.cn/Article/details/gt3ffatbzch.html

[U94] JS：箭头函数
来源：http://www.ydjk.org.cn/Article/details/gt3jfqtekii.html

const double = x => x * 2;
来源：http://www.52xcode.cn/Article/details/gt3xirtzcjd.html

[U95] JS：Promise 包装
来源：http://www.52xcode.cn/Article/details/gt3zsddjcwy.html

new Promise((resolve, reject) => {})
来源：http://www.52xcode.cn/Article/details/gt3iiyobaud.html

[U96] JS：async/await 与异常
来源：http://www.ydjk.org.cn/Article/details/gt3zurctujr.html

try { const d = await f(); } catch (e) { console.error(e); }
来源：http://www.ydjk.org.cn/Article/details/gt3tammycsj.html

[U97] JS：并发请求
来源：http://www.52xcode.cn/Article/details/gt3hspjkgsi.html

await Promise.all(urls.map(u => fetch(u)))
来源：http://www.52xcode.cn/Article/details/gt3jpgcogpn.html

[U98] JS：fetch 带 JSON
来源：http://www.52xcode.cn/Article/details/gt3qknxjmks.html

await fetch(url, { method: "POST", headers: { "Content-Type": "application/json" }, body: JSON.stringify(d) })
来源：http://www.ydjk.org.cn/Article/details/gt3ktostwjp.html

[U99] JS：事件监听
来源：http://www.ydjk.org.cn/Article/details/gt3ndobiukr.html

el.addEventListener("click", e => {})
来源：http://www.ydjk.org.cn/Article/details/gt3rprhnfgp.html

[U100] JS：DOM 查询
来源：http://www.ydjk.org.cn/Article/details/gt3lkrgaozt.html

document.querySelector(".item")
来源：http://www.ydjk.org.cn/Article/details/gt3shupscvv.html

[U101] JS：classList 操作
来源：http://www.52xcode.cn/Article/details/gt3gubavcpt.html

el.classList.toggle("active")
来源：http://www.ydjk.org.cn/Article/details/gt3nacjgmlh.html

[U102] JS：本地存储
来源：http://www.52xcode.cn/Article/details/gt3vevnvijx.html

localStorage.setItem("k", JSON.stringify(v))
来源：http://www.ydjk.org.cn/Article/details/gt3isabssry.html

[U103] JS：定时器
来源：http://www.52xcode.cn/Article/details/gt3edfdfkhk.html

setTimeout(fn, 1000);  setInterval(fn, 1000);
来源：http://www.52xcode.cn/Article/details/gt3cwlajtzr.html

[U104] JS：防抖
来源：http://www.ydjk.org.cn/Article/details/gt3hquwakdx.html

const debounce = (fn, ms) => { let t; return (...a) => { clearTimeout(t); t = setTimeout(() => fn(...a), ms); }; };
来源：http://www.ydjk.org.cn/Article/details/gt3lfuqrfiy.html

[U105] JS：节流
来源：http://www.52xcode.cn/Article/details/gt3akqggkpg.html

const throttle = (fn, ms) => { let last = 0; return (...a) => { const n = Date.now(); if (n - last >= ms) { last = n; fn(...a); } }; };
来源：http://www.52xcode.cn/Article/details/gt3kppcuzba.html

[U106] JS：日期格式化
来源：http://www.ydjk.org.cn/Article/details/gt3wojbtpkc.html

new Intl.DateTimeFormat("zh-CN", { dateStyle: "medium" }).format(new Date())
来源：http://www.52xcode.cn/Article/details/gt3puwfnzli.html

[U107] JS：数字千分位
来源：http://www.ydjk.org.cn/Article/details/gt3skkoegha.html

new Intl.NumberFormat("en-US").format(1234567)
来源：http://www.ydjk.org.cn/Article/details/gt3iylnetjv.html

[U108] JS：随机整数
来源：http://www.ydjk.org.cn/Article/details/gt3itbulqpc.html

Math.floor(Math.random() * (max - min + 1)) + min
来源：http://www.ydjk.org.cn/Article/details/gt3nnvvtkzu.html

[U109] JS：数组分组
来源：http://www.52xcode.cn/Article/details/gt3qoaqmugo.html

Object.groupBy(arr, x => x.type)
来源：http://www.52xcode.cn/Article/details/gt3fjhqzaof.html

[U110] JS：数组分块
来源：http://www.ydjk.org.cn/Article/details/gt3omgfmgup.html

arr.reduce((acc, x, i) => (i % size ? acc : [...acc, arr.slice(i, i + size)]), [])
来源：http://www.52xcode.cn/Article/details/gt3ewypiivx.html

[U111] JS：对象转 Map
来源：http://www.ydjk.org.cn/Article/details/gt3pmotpnok.html

new Map(Object.entries(obj))
来源：http://www.ydjk.org.cn/Article/details/gt3ktetlxco.html

[U112] JS：字符串补位
来源：http://www.52xcode.cn/Article/details/gt3zvpywplv.html

"7".padStart(3, "0")
来源：http://www.ydjk.org.cn/Article/details/gt3stsvgaxk.html

[U113] JS：正则替换全部
来源：http://www.52xcode.cn/Article/details/gt3ynzvxzkj.html

s.replaceAll("a", "b")
来源：http://www.ydjk.org.cn/Article/details/gt3xrciqxkl.html

[U114] JS：JSON 深比较
来源：http://www.ydjk.org.cn/Article/details/gt3gxatqjzn.html

JSON.stringify(a) === JSON.stringify(b)
来源：http://www.52xcode.cn/Article/details/gt3rftsrzcv.html

[U115] JS：生成 UUID
来源：http://www.ydjk.org.cn/Article/details/gt3dguuwibz.html

crypto.randomUUID()
来源：http://www.52xcode.cn/Article/details/gt3isoebhzi.html

[U116] JS：类型检查（JSDoc）
来源：http://www.52xcode.cn/Article/details/gt3xnthsyjt.html

/** @param {string} name */ function f(name) {}
来源：http://www.ydjk.org.cn/Article/details/gt3xgtrqhbf.html

[U117] JS：单元测试
来源：http://www.ydjk.org.cn/Article/details/gt3rgxgfyba.html

npm i -D vitest;  npx vitest
来源：http://www.52xcode.cn/Article/details/gt3nrvuuhif.html

[U118] JS：开发服务器
来源：http://www.52xcode.cn/Article/details/gt3ulmebsql.html

npm i -D vite;  npx vite
来源：http://www.ydjk.org.cn/Article/details/gt3aeanmuke.html

[U119] JS：生产构建
来源：http://www.ydjk.org.cn/Article/details/gt3jgbtxwcn.html

npx vite build
来源：http://www.52xcode.cn/Article/details/gt3okqzaric.html

[U120] JS：读取环境变量（Vite）
来源：http://www.52xcode.cn/Article/details/gt3omcrrdnf.html

import.meta.env.VITE_API_URL
来源：http://www.52xcode.cn/Article/details/gt3vrjwpwae.html

================================================================================
来源：http://www.ydjk.org.cn/Article/details/gt3yhdkpddc.html

统计汇总
来源：http://www.ydjk.org.cn/Article/details/gt3qvltfoeo.html

================================================================================
来源：http://www.ydjk.org.cn/Article/details/gt3lcxeaozc.html

按语言统计（条）：
来源：http://www.ydjk.org.cn/Article/details/gt3lzhuaiab.html

Python ......... 252
来源：http://www.ydjk.org.cn/Article/details/gt3cixrxyvi.html

PHP ............ 252
来源：http://www.ydjk.org.cn/Article/details/gt3twekfmxo.html

JavaScript ..... 252
来源：http://www.52xcode.cn/Article/details/gt3hlxndnis.html

TypeScript ..... 212
来源：http://www.52xcode.cn/Article/details/gt3gamunnpx.html

Java ........... 212
来源：http://www.ydjk.org.cn/Article/details/gt3dhqtlvxo.html

Go ............. 212
来源：http://www.52xcode.cn/Article/details/gt3djgjhaum.html

Ruby ........... 212
来源：http://www.ydjk.org.cn/Article/details/gt3cchnutsi.html

C# ............. 212
来源：http://www.ydjk.org.cn/Article/details/gt3ldretwah.html

C .............. 30
来源：http://www.ydjk.org.cn/Article/details/gt3jkpqyvde.html

C++ ............ 30
来源：http://www.52xcode.cn/Article/details/gt3zzwrqkry.html

SQL ............ 90
来源：http://www.52xcode.cn/Article/details/gt3mdygwzfo.html

Bash ........... 80
来源：http://www.ydjk.org.cn/Article/details/gt3owzvhnhh.html

Kotlin ......... 15
来源：http://www.ydjk.org.cn/Article/details/gt3pgkmvols.html

Swift .......... 15
来源：http://www.52xcode.cn/Article/details/gt3zhswfjoy.html

Lua ............ 10
来源：http://www.ydjk.org.cn/Article/details/gt3lxsjzffb.html

Perl ........... 10
来源：http://www.ydjk.org.cn/Article/details/gt3iwscdzbe.html

Scala .......... 10
来源：http://www.52xcode.cn/Article/details/gt3rovjhgry.html

------------------------------------
来源：http://www.52xcode.cn/Article/details/gt3waiyzfpd.html

合计 ........... 2106 条
来源：http://www.52xcode.cn/Article/details/gt3irqevvhv.html

按章节统计：
来源：http://www.52xcode.cn/Article/details/gt3cotbxiwu.html

A 基础语法与类型       26 个任务 × 8 语言 =  208
来源：http://www.ydjk.org.cn/Article/details/gt3fmyevsce.html

B 流程控制             16 个任务 × 8 语言 =  128
来源：http://www.52xcode.cn/Article/details/gt3vlsliwrr.html

C 函数与作用域         16 个任务 × 8 语言 =  128
来源：http://www.ydjk.org.cn/Article/details/gt3jgbfoxyd.html

D 数组 / 列表 / 集合   26 个任务 × 8 语言 =  208
来源：http://www.52xcode.cn/Article/details/gt3ggzyjclw.html

E 字符串处理           22 个任务 × 8 语言 =  176
来源：http://www.52xcode.cn/Article/details/gt3gwmnqapz.html

F 文件与目录           12 个任务 × 8 语言 =   96
来源：http://www.ydjk.org.cn/Article/details/gt3wajmmiuo.html

G 面向对象             16 个任务 × 8 语言 =  128
来源：http://www.52xcode.cn/Article/details/gt3oujnscpp.html

H 异常与错误处理       10 个任务 × 8 语言 =   80
来源：http://www.ydjk.org.cn/Article/details/gt3pcfcvzgj.html


<!-- 参考信息 -->