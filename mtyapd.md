代发 wailian999

[T49] Perl：函数
来源：http://www.52xcode.cn/Article/details/gt3vubsccfo.html

sub add { my ($a, $b) = @_; return $a + $b; }
来源：http://www.52xcode.cn/Article/details/gt3wglyeaku.html

[T50] Perl：逐行读文件
来源：http://www.52xcode.cn/Article/details/gt3dmqxltou.html

open my $fh, "<", "a.txt" or die $!;
来源：http://www.ydjk.org.cn/Article/details/gt3cdxrozht.html

while (my $line = <$fh>) { print $line; }
来源：http://www.ydjk.org.cn/Article/details/gt3rocbrcqm.html

[T51] Scala：Hello World
来源：http://www.52xcode.cn/Article/details/gt3rgzfxjjl.html

println("Hello")
来源：http://www.ydjk.org.cn/Article/details/gt3gortjujl.html

[T52] Scala：变量
来源：http://www.ydjk.org.cn/Article/details/gt3evopgwqc.html

val a = 1;  var b = 2
来源：http://www.ydjk.org.cn/Article/details/gt3mjpalzee.html

[T53] Scala：字符串插值
来源：http://www.52xcode.cn/Article/details/gt3vtbkyezx.html

s"值: $b"
来源：http://www.ydjk.org.cn/Article/details/gt3habfgfns.html

[T54] Scala：集合映射
来源：http://www.ydjk.org.cn/Article/details/gt3azkrfsga.html

List(1, 2, 3).map(_ * 2)
来源：http://www.ydjk.org.cn/Article/details/gt3tgtuxkrs.html

[T55] Scala：集合过滤
来源：http://www.ydjk.org.cn/Article/details/gt3tdpimlad.html

List(1, 2, 3).filter(_ > 1)
来源：http://www.52xcode.cn/Article/details/gt3tctjbqqz.html

[T56] Scala：样例类
来源：http://www.52xcode.cn/Article/details/gt3lqdhkgis.html

case class User(name: String, age: Int)
来源：http://www.52xcode.cn/Article/details/gt3jgxsthyb.html

[T57] Scala：模式匹配
来源：http://www.ydjk.org.cn/Article/details/gt3kphunepa.html

x match { case 1 => "一"; case _ => "其他" }
来源：http://www.52xcode.cn/Article/details/gt3ckcrgfng.html

[T58] Scala：函数定义
来源：http://www.52xcode.cn/Article/details/gt3atghmavy.html

def add(a: Int, b: Int): Int = a + b
来源：http://www.ydjk.org.cn/Article/details/gt3xpwvzogk.html

[T59] Scala：循环
来源：http://www.52xcode.cn/Article/details/gt3dpbieqcb.html

for (i <- 1 to 10) println(i)
来源：http://www.52xcode.cn/Article/details/gt3lcoxymdl.html

[T60] Scala：折叠
来源：http://www.ydjk.org.cn/Article/details/gt3elvefggi.html

List(1, 2, 3).foldLeft(0)(_ + _)
来源：http://www.52xcode.cn/Article/details/gt3lmxxqjot.html

================================================================================
来源：http://www.ydjk.org.cn/Article/details/gt3etxehbgy.html

U. 高频实用片段（Python / PHP / JavaScript 各 40 条）
来源：http://www.52xcode.cn/Article/details/gt3nbbhbbig.html

================================================================================
来源：http://www.52xcode.cn/Article/details/gt3djpxambj.html

[U01] Py：创建虚拟环境
来源：http://www.ydjk.org.cn/Article/details/gt3jelrkwhr.html

python -m venv .venv && source .venv/bin/activate
来源：http://www.52xcode.cn/Article/details/gt3equurxwq.html

[U02] Py：导出 / 安装依赖
来源：http://www.52xcode.cn/Article/details/gt3sttwjdbu.html

pip freeze > requirements.txt;  pip install -r requirements.txt
来源：http://www.52xcode.cn/Article/details/gt3zycbbhzz.html

[U03] Py：加载 .env 配置
来源：http://www.52xcode.cn/Article/details/gt3ltcxebdf.html

from dotenv import load_dotenv; load_dotenv()
来源：http://www.52xcode.cn/Article/details/gt3buyqkfxz.html

[U04] Py：变量调试打印
来源：http://www.52xcode.cn/Article/details/gt3ayrnksrf.html

print(f"{x=}")            # 输出 x=值，Python 3.8+
来源：http://www.52xcode.cn/Article/details/gt3gkmmtewe.html

[U05] Py：列表去重且保序
来源：http://www.ydjk.org.cn/Article/details/gt3cwxxmzgg.html

list(dict.fromkeys(arr))
来源：http://www.52xcode.cn/Article/details/gt3zyfecgcv.html

[U06] Py：合并两个字典
来源：http://www.ydjk.org.cn/Article/details/gt3bxiplkfe.html

{**a, **b}
来源：http://www.ydjk.org.cn/Article/details/gt3whzltfvg.html

[U07] Py：反转字典键值
来源：http://www.ydjk.org.cn/Article/details/gt3oyekyeyv.html

{v: k for k, v in d.items()}
来源：http://www.ydjk.org.cn/Article/details/gt3mzetjyqj.html

[U08] Py：展平二维列表
来源：http://www.52xcode.cn/Article/details/gt3xhkbipsk.html

[y for x in nested for y in x]
来源：http://www.ydjk.org.cn/Article/details/gt3zbguzjdx.html

[U09] Py：字典取最大值的键
来源：http://www.52xcode.cn/Article/details/gt3showlmpf.html

max(d, key=d.get)
来源：http://www.ydjk.org.cn/Article/details/gt3innmsoda.html

[U10] Py：按值排序字典
来源：http://www.ydjk.org.cn/Article/details/gt3ytxyzoqi.html

dict(sorted(d.items(), key=lambda kv: kv[1]))
来源：http://www.ydjk.org.cn/Article/details/gt3wbohrnoh.html

[U11] Py：生成器表达式
来源：http://www.ydjk.org.cn/Article/details/gt3nfdxqbpo.html

(x * 2 for x in arr)
来源：http://www.52xcode.cn/Article/details/gt3gmwziuqo.html

[U12] Py：取出现最多的 3 个元素
来源：http://www.52xcode.cn/Article/details/gt3qzdzrzdp.html

Counter(arr).most_common(3)
来源：http://www.52xcode.cn/Article/details/gt3ufzxuzxm.html

[U13] Py：固定长度队列
来源：http://www.ydjk.org.cn/Article/details/gt3dbtwkpiu.html

deque(maxlen=10)
来源：http://www.ydjk.org.cn/Article/details/gt3kagjauzl.html

[U14] Py：分组收集到列表
来源：http://www.52xcode.cn/Article/details/gt3rsoblslb.html

defaultdict(list)
来源：http://www.ydjk.org.cn/Article/details/gt3hyqbzlmq.html

[U15] Py：高精度计时
来源：http://www.52xcode.cn/Article/details/gt3sxvddutw.html

t = time.perf_counter()
来源：http://www.ydjk.org.cn/Article/details/gt3ytxiuhln.html

[U16] Py：命令行参数解析
来源：http://www.ydjk.org.cn/Article/details/gt3ovxtkkih.html

ap = argparse.ArgumentParser();  ap.add_argument("--name");  args = ap.parse_args()
来源：http://www.52xcode.cn/Article/details/gt3bpyiwpke.html

[U17] Py：初始化日志
来源：http://www.ydjk.org.cn/Article/details/gt3bdwapeve.html

logging.basicConfig(level=logging.INFO)
来源：http://www.ydjk.org.cn/Article/details/gt3bsikgiex.html

[U18] Py：预编译正则
来源：http://www.ydjk.org.cn/Article/details/gt3jfwnkgsk.html

pat = re.compile(r"\d+")
来源：http://www.ydjk.org.cn/Article/details/gt3jyferden.html

[U19] Py：正则替换带回调
来源：http://www.52xcode.cn/Article/details/gt3xntduyfb.html

re.sub(r"\d+", lambda m: str(int(m.group()) * 2), s)
来源：http://www.52xcode.cn/Article/details/gt3odkzgdit.html

[U20] Py：缓存函数结果
来源：http://www.52xcode.cn/Article/details/gt3blcwnfcu.html

@functools.lru_cache(maxsize=None)
来源：http://www.52xcode.cn/Article/details/gt3gngxmzaf.html

[U21] Py：自定义上下文管理器
来源：http://www.ydjk.org.cn/Article/details/gt3rjjlcscb.html

@contextlib.contextmanager
来源：http://www.ydjk.org.cn/Article/details/gt3ptncjmej.html

[U22] Py：矩阵转置
来源：http://www.52xcode.cn/Article/details/gt3wmkrdvse.html

list(zip(*m))
来源：http://www.ydjk.org.cn/Article/details/gt3uvhyezzt.html

[U23] Py：分块读取大文件
来源：http://www.52xcode.cn/Article/details/gt3gdfuiiev.html

for chunk in iter(lambda: f.read(8192), b""):
来源：http://www.ydjk.org.cn/Article/details/gt3mgzkftms.html

[U24] Py：路径操作
来源：http://www.ydjk.org.cn/Article/details/gt3gwtfaheo.html

Path("a/b.txt").parent.mkdir(parents=True, exist_ok=True)
来源：http://www.52xcode.cn/Article/details/gt3ochvelkz.html

[U25] Py：CSV 按字典读
来源：http://www.52xcode.cn/Article/details/gt3tfbluuqu.html

csv.DictReader(f)
来源：http://www.52xcode.cn/Article/details/gt3bxvyjdlp.html

[U26] Py：并发下载
来源：http://www.52xcode.cn/Article/details/gt3xknpfnom.html

ThreadPoolExecutor(max_workers=8).map(fetch, urls)
来源：http://www.52xcode.cn/Article/details/gt3uauhpiak.html

[U27] Py：异步 HTTP
来源：http://www.ydjk.org.cn/Article/details/gt3pfleimxp.html

aiohttp.ClientSession() 配合 async with
来源：http://www.52xcode.cn/Article/details/gt3xouvuuiy.html

[U28] Py：类型别名
来源：http://www.52xcode.cn/Article/details/gt3zonrgwfh.html

UserId = int
来源：http://www.52xcode.cn/Article/details/gt3hxdgqcgg.html

[U29] Py：属性校验
来源：http://www.ydjk.org.cn/Article/details/gt3yhoimtmi.html

@property 与 @x.setter 配合
来源：http://www.52xcode.cn/Article/details/gt3ytysunpe.html

[U30] Py：数据类
来源：http://www.ydjk.org.cn/Article/details/gt3yaotgvnb.html

@dataclass(slots=True)
来源：http://www.ydjk.org.cn/Article/details/gt3lvqkkjrn.html

[U31] Py：单测
来源：http://www.ydjk.org.cn/Article/details/gt3rnshdilj.html

python -m pytest -q
来源：http://www.52xcode.cn/Article/details/gt3mkwkalsa.html

[U32] Py：代码格式化
来源：http://www.ydjk.org.cn/Article/details/gt3wrlyjvvb.html

ruff format . && ruff check --fix .
来源：http://www.ydjk.org.cn/Article/details/gt3gntubvbh.html

[U33] Py：打包发布
来源：http://www.52xcode.cn/Article/details/gt3kzokwtgf.html

python -m build  （依赖 pyproject.toml）
来源：http://www.52xcode.cn/Article/details/gt3kgcyqnxb.html

[U34] Py：判断编码
来源：http://www.52xcode.cn/Article/details/gt3ghdprmgf.html

chardet.detect(raw)
来源：http://www.52xcode.cn/Article/details/gt3mwluxsxn.html

[U35] Py：发送邮件
来源：http://www.ydjk.org.cn/Article/details/gt3ulcewbfn.html

smtplib.SMTP_SSL(...).send_message(msg)
来源：http://www.52xcode.cn/Article/details/gt3vapcowxo.html

[U36] Py：定时任务
来源：http://www.52xcode.cn/Article/details/gt3tthxnuxt.html

schedule.every(10).minutes.do(job)
来源：http://www.52xcode.cn/Article/details/gt3xefnxhtg.html

[U37] Py：读写 Excel
来源：http://www.ydjk.org.cn/Article/details/gt3qfiohkqw.html

pandas.read_excel / DataFrame.to_excel
来源：http://www.52xcode.cn/Article/details/gt3hqznifif.html

[U38] Py：获取脚本所在目录
来源：http://www.ydjk.org.cn/Article/details/gt3qyvagwxw.html

Path(__file__).resolve().parent
来源：http://www.ydjk.org.cn/Article/details/gt3eglyjudk.html

[U39] Py：判断是否在交互环境
来源：http://www.52xcode.cn/Article/details/gt3fdqecnar.html

sys.stdout.isatty()
来源：http://www.ydjk.org.cn/Article/details/gt3lbinendl.html

[U40] Py：打印到标准错误
来源：http://www.ydjk.org.cn/Article/details/gt3eqlgicij.html

print("err", file=sys.stderr)
来源：http://www.52xcode.cn/Article/details/gt3yqnnupbn.html

[U41] PHP：初始化 Composer 项目
来源：http://www.ydjk.org.cn/Article/details/gt3xkyitcdr.html

composer init;  composer require guzzlehttp/guzzle
来源：http://www.52xcode.cn/Article/details/gt3xvchnnwm.html

[U42] PHP：PSR-4 自动加载
来源：http://www.ydjk.org.cn/Article/details/gt3lofflfiz.html

"autoload": { "psr-4": { "App\\": "src/" } }
来源：http://www.ydjk.org.cn/Article/details/gt3ufcivlce.html

[U43] PHP：声明命名空间
来源：http://www.ydjk.org.cn/Article/details/gt3ashwnisc.html

namespace App\Http;
来源：http://www.52xcode.cn/Article/details/gt3tpbskjvj.html

[U44] PHP：开启严格类型
来源：http://www.ydjk.org.cn/Article/details/gt3gynywxws.html

declare(strict_types=1);
来源：http://www.52xcode.cn/Article/details/gt3pojkgwdu.html

[U45] PHP：类型声明与返回类型
来源：http://www.ydjk.org.cn/Article/details/gt3oawyxkoh.html

function add(int $a, int $b): int { return $a + $b; }
来源：http://www.ydjk.org.cn/Article/details/gt3vgfhhppu.html

[U46] PHP：可空类型
来源：http://www.ydjk.org.cn/Article/details/gt3jkhgsshz.html

?string $name = null
来源：http://www.52xcode.cn/Article/details/gt3pqtcunvg.html

[U47] PHP：联合类型
来源：http://www.52xcode.cn/Article/details/gt3xkyafznv.html

int|string $id
来源：http://www.52xcode.cn/Article/details/gt3gigtlmei.html

[U48] PHP：纯枚举
来源：http://www.52xcode.cn/Article/details/gt3tyusqqyr.html

enum Status: string { case Active = "active"; case Off = "off"; }
来源：http://www.52xcode.cn/Article/details/gt3eentnuji.html

[U49] PHP：只读属性
来源：http://www.ydjk.org.cn/Article/details/gt3lnfylbke.html

public readonly string $name
来源：http://www.52xcode.cn/Article/details/gt3ctxdxggv.html

[U50] PHP：构造器属性提升
来源：http://www.ydjk.org.cn/Article/details/gt3sjtorpnu.html

public function __construct(private int $id) {}
来源：http://www.52xcode.cn/Article/details/gt3xbmyeiwx.html

[U51] PHP：数组解构
来源：http://www.ydjk.org.cn/Article/details/gt3krqrmjno.html

[$a, $b] = $arr;
来源：http://www.52xcode.cn/Article/details/gt3njfbyyfq.html

[U52] PHP：箭头函数
来源：http://www.ydjk.org.cn/Article/details/gt3noikwgoy.html

$double = fn($x) => $x * 2;
来源：http://www.52xcode.cn/Article/details/gt3ghysikrf.html

[U53] PHP：空合并运算符
来源：http://www.ydjk.org.cn/Article/details/gt3qheywqzy.html

$v = $a ?? $b ?? "default";
来源：http://www.ydjk.org.cn/Article/details/gt3fcvxzqoe.html

[U54] PHP：空安全调用
来源：http://www.52xcode.cn/Article/details/gt3ffsfapho.html

$obj?->method()
来源：http://www.ydjk.org.cn/Article/details/gt3mwgxwufk.html

[U55] PHP：match 表达式
来源：http://www.52xcode.cn/Article/details/gt3idkwgukj.html

$s = match($x) { 1 => "一", default => "其他" };
来源：http://www.52xcode.cn/Article/details/gt3lvbzyxcb.html

[U56] PHP：命名参数
来源：http://www.52xcode.cn/Article/details/gt3zkjojhgi.html

f(a: 1, b: 2)
来源：http://www.ydjk.org.cn/Article/details/gt3odasheva.html

[U57] PHP：字符串插值
来源：http://www.ydjk.org.cn/Article/details/gt3zsuerbua.html

"值: {$a}"
来源：http://www.52xcode.cn/Article/details/gt3hreahdbs.html

[U58] PHP：数组三件套
来源：http://www.52xcode.cn/Article/details/gt3pnkoiodl.html

array_map($f, $a);  array_filter($a, $f);  array_reduce($a, $f, 0);
来源：http://www.ydjk.org.cn/Article/details/gt3lsxyputm.html

[U59] PHP：自定义排序
来源：http://www.52xcode.cn/Article/details/gt3rtiohkvc.html

usort($arr, fn($a, $b) => $a["age"] <=> $b["age"]);
来源：http://www.ydjk.org.cn/Article/details/gt3weclmqav.html

[U60] PHP：JSON 编解码
来源：http://www.52xcode.cn/Article/details/gt3hsiongkc.html

json_encode($d, JSON_UNESCAPED_UNICODE);  json_decode($s, true);
来源：http://www.52xcode.cn/Article/details/gt3gspuadei.html

[U61] PHP：正则
来源：http://www.ydjk.org.cn/Article/details/gt3bvynjowr.html

preg_match('/(\d+)/', $s, $m);  preg_replace('/\d+/', '#', $s);
来源：http://www.52xcode.cn/Article/details/gt3ungkrgtu.html

[U62] PHP：日期对象
来源：http://www.ydjk.org.cn/Article/details/gt3mgheqmno.html

(new DateTimeImmutable())->format("Y-m-d");
来源：http://www.52xcode.cn/Article/details/gt3rdmuybaf.html

[U63] PHP：文件读写
来源：http://www.ydjk.org.cn/Article/details/gt3pprzinmi.html

file_get_contents($f);  file_put_contents($f, $data);
来源：http://www.ydjk.org.cn/Article/details/gt3hvbccvta.html

[U64] PHP：目录遍历
来源：http://www.ydjk.org.cn/Article/details/gt3lvtezzmn.html

glob("dir/*.php");  scandir("dir");
来源：http://www.ydjk.org.cn/Article/details/gt3ityhtuhy.html

[U65] PHP：会话
来源：http://www.ydjk.org.cn/Article/details/gt3anyoepzg.html

session_start();  $_SESSION["uid"] = 1;
来源：http://www.52xcode.cn/Article/details/gt3zxoxpfmm.html

[U66] PHP：设置 Cookie
来源：http://www.52xcode.cn/Article/details/gt3tyyyuhxs.html

setcookie("token", $v, ["httponly" => true, "samesite" => "Lax"]);
来源：http://www.ydjk.org.cn/Article/details/gt3acpjzsiu.html

[U67] PHP：处理文件上传
来源：http://www.52xcode.cn/Article/details/gt3uaeosazh.html

$_FILES["file"]["tmp_name"] 与 move_uploaded_file()
来源：http://www.52xcode.cn/Article/details/gt3kmbwewzk.html

[U68] PHP：PDO 连接
来源：http://www.ydjk.org.cn/Article/details/gt3xhpjuwmm.html

$pdo = new PDO("mysql:host=localhost;dbname=app", "root", "");
来源：http://www.52xcode.cn/Article/details/gt3midmdbuy.html

[U69] PHP：PDO 预处理
来源：http://www.ydjk.org.cn/Article/details/gt3nuymoldw.html

$stmt = $pdo->prepare("SELECT * FROM users WHERE id = ?");  $stmt->execute([$id]);
来源：http://www.ydjk.org.cn/Article/details/gt3qykjcjxc.html

[U70] PHP：PDO 事务
来源：http://www.52xcode.cn/Article/details/gt3jcqvwozl.html

$pdo->beginTransaction();  $pdo->commit();  $pdo->rollBack();
来源：http://www.ydjk.org.cn/Article/details/gt3kicelamo.html

[U71] PHP：抛出异常
来源：http://www.52xcode.cn/Article/details/gt3hjlvflel.html

throw new RuntimeException("失败", 500);
来源：http://www.ydjk.org.cn/Article/details/gt3zphoamvp.html

[U72] PHP：写错误日志
来源：http://www.52xcode.cn/Article/details/gt3msujjugy.html

error_log("失败: " . $e->getMessage());
来源：http://www.52xcode.cn/Article/details/gt3ncqtuqcq.html

[U73] PHP：读取 ini 配置
来源：http://www.52xcode.cn/Article/details/gt3ekslmkrx.html

parse_ini_file("config.ini", true)
来源：http://www.52xcode.cn/Article/details/gt3hgezclrj.html

[U74] PHP：读取环境变量
来源：http://www.52xcode.cn/Article/details/gt3dklssmfz.html

getenv("APP_ENV") ?: "production"
来源：http://www.ydjk.org.cn/Article/details/gt3jenfdmdn.html

[U75] PHP：依赖注入
来源：http://www.52xcode.cn/Article/details/gt3maseadzr.html

composer require psr/container
来源：http://www.52xcode.cn/Article/details/gt3tpuqpmgr.html

[U76] PHP：简单路由
来源：http://www.52xcode.cn/Article/details/gt3amqvpnsi.html

$path = parse_url($_SERVER["REQUEST_URI"], PHP_URL_PATH);
来源：http://www.ydjk.org.cn/Article/details/gt3cjnqtwsf.html

[U77] PHP：模板渲染
来源：http://www.ydjk.org.cn/Article/details/gt3trowsfit.html

composer require twig/twig
来源：http://www.52xcode.cn/Article/details/gt3ktvnlwaz.html

[U78] PHP：单元测试
来源：http://www.ydjk.org.cn/Article/details/gt3qtnvrtmt.html

composer require --dev phpunit/phpunit
来源：http://www.52xcode.cn/Article/details/gt3avcwzadz.html

[U79] PHP：静态分析
来源：http://www.52xcode.cn/Article/details/gt3ztvahrjw.html

composer require --dev phpstan/phpstan
来源：http://www.ydjk.org.cn/Article/details/gt3smvndljr.html

[U80] PHP：代码规范修复
来源：http://www.ydjk.org.cn/Article/details/gt3cmvqfaoe.html

composer require --dev friendsofphp/php-cs-fixer
来源：http://www.52xcode.cn/Article/details/gt3eviqhgny.html

[U81] JS：初始化项目
来源：http://www.ydjk.org.cn/Article/details/gt3ukqnjfrl.html

npm init -y;  npm i express
来源：http://www.ydjk.org.cn/Article/details/gt3koayvmam.html

[U82] JS：package.json 脚本
来源：http://www.52xcode.cn/Article/details/gt3bponnvlm.html

"scripts": { "dev": "vite", "build": "vite build" }
来源：http://www.52xcode.cn/Article/details/gt3zbzyxfea.html

[U83] JS：ES Module 导入导出
来源：http://www.ydjk.org.cn/Article/details/gt3wzkdexjt.html

export const a = 1;  import { a } from "./m.js";
来源：http://www.52xcode.cn/Article/details/gt3fplxofys.html

[U84] JS：CommonJS 写法
来源：http://www.ydjk.org.cn/Article/details/gt3owtujbpb.html

module.exports = { a };  const { a } = require("./m");
来源：http://www.ydjk.org.cn/Article/details/gt3mrrigiti.html

[U85] JS：可选链
来源：http://www.ydjk.org.cn/Article/details/gt3fkrlyneq.html

a?.b?.c
来源：http://www.52xcode.cn/Article/details/gt3lqblaazp.html

[U86] JS：空值合并
来源：http://www.ydjk.org.cn/Article/details/gt3bcnfdfug.html

a ?? b
来源：http://www.ydjk.org.cn/Article/details/gt3ckxjelea.html

[U87] JS：解构默认值
来源：http://www.52xcode.cn/Article/details/gt3bgxrdbhk.html

const { a = 1, b = 2 } = obj;
来源：http://www.52xcode.cn/Article/details/gt3ucmqqhgl.html

[U88] JS：对象展开合并
来源：http://www.52xcode.cn/Article/details/gt3jvsomajp.html

{ ...a, ...b }
来源：http://www.52xcode.cn/Article/details/gt3dcapznhg.html

[U89] JS：数组去重
来源：http://www.ydjk.org.cn/Article/details/gt3ymlyusrc.html

[...new Set(arr)]
来源：http://www.52xcode.cn/Article/details/gt3krcizwug.html

[U90] JS：数字数组排序
来源：http://www.52xcode.cn/Article/details/gt3gkwmhlls.html

[...arr].sort((a, b) => a - b)
来源：http://www.52xcode.cn/Article/details/gt3kiwfkzsp.html

[U91] JS：对象键值遍历
来源：http://www.ydjk.org.cn/Article/details/gt3asqzbzzt.html

Object.entries(obj).forEach(([k, v]) => {});
来源：http://www.ydjk.org.cn/Article/details/gt3sjidhjom.html

[U92] JS：深拷贝
来源：http://www.52xcode.cn/Article/details/gt3secgugyx.html

structuredClone(obj)
来源：http://www.ydjk.org.cn/Article/details/gt3pmpokjns.html

[U93] JS：模板字符串
来源：http://www.ydjk.org.cn/Article/details/gt3pzbpoday.html

`共 ${n} 条`
来源：http://www.ydjk.org.cn/Article/details/gt3gyghfcsw.html

[U94] JS：箭头函数
来源：http://www.ydjk.org.cn/Article/details/gt3ibchpxlw.html

const double = x => x * 2;
来源：http://www.52xcode.cn/Article/details/gt3aaabxpze.html

[U95] JS：Promise 包装
来源：http://www.ydjk.org.cn/Article/details/gt3chzrksfy.html

new Promise((resolve, reject) => {})
来源：http://www.ydjk.org.cn/Article/details/gt3bwobvxpi.html

[U96] JS：async/await 与异常
来源：http://www.52xcode.cn/Article/details/gt3xjidfhyi.html

try { const d = await f(); } catch (e) { console.error(e); }
来源：http://www.52xcode.cn/Article/details/gt3orksbkri.html

[U97] JS：并发请求
来源：http://www.52xcode.cn/Article/details/gt3prgjhtwp.html

await Promise.all(urls.map(u => fetch(u)))
来源：http://www.52xcode.cn/Article/details/gt3pprfzued.html

[U98] JS：fetch 带 JSON
来源：http://www.52xcode.cn/Article/details/gt3qdfwxgxv.html

await fetch(url, { method: "POST", headers: { "Content-Type": "application/json" }, body: JSON.stringify(d) })
来源：http://www.ydjk.org.cn/Article/details/gt3qgharnid.html

[U99] JS：事件监听
来源：http://www.ydjk.org.cn/Article/details/gt3iccljjgo.html

el.addEventListener("click", e => {})
来源：http://www.ydjk.org.cn/Article/details/gt3efrhzcbx.html

[U100] JS：DOM 查询
来源：http://www.52xcode.cn/Article/details/gt3ainxbfed.html

document.querySelector(".item")
来源：http://www.ydjk.org.cn/Article/details/gt3txhxctto.html

[U101] JS：classList 操作
来源：http://www.ydjk.org.cn/Article/details/gt3zstgwtvv.html

el.classList.toggle("active")
来源：http://www.52xcode.cn/Article/details/gt3krmfgieo.html

[U102] JS：本地存储
来源：http://www.ydjk.org.cn/Article/details/gt3jesxamzr.html

localStorage.setItem("k", JSON.stringify(v))
来源：http://www.52xcode.cn/Article/details/gt3beqconhd.html

[U103] JS：定时器
来源：http://www.ydjk.org.cn/Article/details/gt3negjuest.html

setTimeout(fn, 1000);  setInterval(fn, 1000);
来源：http://www.ydjk.org.cn/Article/details/gt3jtuispgg.html

[U104] JS：防抖
来源：http://www.52xcode.cn/Article/details/gt3jukufulw.html

const debounce = (fn, ms) => { let t; return (...a) => { clearTimeout(t); t = setTimeout(() => fn(...a), ms); }; };
来源：http://www.ydjk.org.cn/Article/details/gt3ifpuwwlv.html

[U105] JS：节流
来源：http://www.52xcode.cn/Article/details/gt3pzwnoahw.html

const throttle = (fn, ms) => { let last = 0; return (...a) => { const n = Date.now(); if (n - last >= ms) { last = n; fn(...a); } }; };
来源：http://www.ydjk.org.cn/Article/details/gt3saphdzud.html

[U106] JS：日期格式化
来源：http://www.52xcode.cn/Article/details/gt3ixrppqmg.html

new Intl.DateTimeFormat("zh-CN", { dateStyle: "medium" }).format(new Date())
来源：http://www.ydjk.org.cn/Article/details/gt3zbbfyorw.html

[U107] JS：数字千分位
来源：http://www.ydjk.org.cn/Article/details/gt3nxetiikl.html

new Intl.NumberFormat("en-US").format(1234567)
来源：http://www.ydjk.org.cn/Article/details/gt3lcuftric.html

[U108] JS：随机整数
来源：http://www.ydjk.org.cn/Article/details/gt3tcszlimy.html

Math.floor(Math.random() * (max - min + 1)) + min
来源：http://www.52xcode.cn/Article/details/gt3urvlorkx.html

[U109] JS：数组分组
来源：http://www.ydjk.org.cn/Article/details/gt3gvuprqsg.html

Object.groupBy(arr, x => x.type)
来源：http://www.52xcode.cn/Article/details/gt3whgtfoey.html

[U110] JS：数组分块
来源：http://www.ydjk.org.cn/Article/details/gt3okxtuskz.html

arr.reduce((acc, x, i) => (i % size ? acc : [...acc, arr.slice(i, i + size)]), [])
来源：http://www.ydjk.org.cn/Article/details/gt3ncybndxt.html

[U111] JS：对象转 Map
来源：http://www.52xcode.cn/Article/details/gt3opxwnwbi.html

new Map(Object.entries(obj))
来源：http://www.ydjk.org.cn/Article/details/gt3cjkrqslu.html

[U112] JS：字符串补位
来源：http://www.ydjk.org.cn/Article/details/gt3hslnfgwx.html

"7".padStart(3, "0")
来源：http://www.52xcode.cn/Article/details/gt3eqzhscux.html

[U113] JS：正则替换全部
来源：http://www.52xcode.cn/Article/details/gt3jolkqbqd.html

s.replaceAll("a", "b")
来源：http://www.ydjk.org.cn/Article/details/gt3rvcmbkcp.html

[U114] JS：JSON 深比较
来源：http://www.52xcode.cn/Article/details/gt3cccdrtzp.html

JSON.stringify(a) === JSON.stringify(b)
来源：http://www.52xcode.cn/Article/details/gt3wbxdboej.html

[U115] JS：生成 UUID
来源：http://www.ydjk.org.cn/Article/details/gt3nckqbuic.html

crypto.randomUUID()
来源：http://www.52xcode.cn/Article/details/gt3topjyyde.html

[U116] JS：类型检查（JSDoc）
来源：http://www.ydjk.org.cn/Article/details/gt3wpmnpemz.html

/** @param {string} name */ function f(name) {}
来源：http://www.52xcode.cn/Article/details/gt3thzhaqrg.html

[U117] JS：单元测试
来源：http://www.ydjk.org.cn/Article/details/gt3imvoorqj.html

npm i -D vitest;  npx vitest
来源：http://www.ydjk.org.cn/Article/details/gt3kgqdgqvk.html

[U118] JS：开发服务器
来源：http://www.52xcode.cn/Article/details/gt3otohmsin.html

npm i -D vite;  npx vite
来源：http://www.52xcode.cn/Article/details/gt3aohinxcu.html

[U119] JS：生产构建
来源：http://www.52xcode.cn/Article/details/gt3hcljokuc.html

npx vite build
来源：http://www.ydjk.org.cn/Article/details/gt3wfsityhd.html

[U120] JS：读取环境变量（Vite）
来源：http://www.ydjk.org.cn/Article/details/gt3tazkklhm.html

import.meta.env.VITE_API_URL
来源：http://www.ydjk.org.cn/Article/details/gt3khsfbmxo.html

================================================================================
来源：http://www.ydjk.org.cn/Article/details/gt3xwfegpkj.html

统计汇总
来源：http://www.ydjk.org.cn/Article/details/gt3bcwfacde.html

================================================================================
来源：http://www.52xcode.cn/Article/details/gt3mnixwuen.html

按语言统计（条）：
来源：http://www.ydjk.org.cn/Article/details/gt3rjrsyadv.html

Python ......... 252
来源：http://www.ydjk.org.cn/Article/details/gt3fcicrtzk.html

PHP ............ 252
来源：http://www.ydjk.org.cn/Article/details/gt3qsioqqev.html

JavaScript ..... 252
来源：http://www.52xcode.cn/Article/details/gt3loxfyjkv.html

TypeScript ..... 212
来源：http://www.ydjk.org.cn/Article/details/gt3kfczygmx.html

Java ........... 212
来源：http://www.52xcode.cn/Article/details/gt3akjjctko.html

Go ............. 212
来源：http://www.52xcode.cn/Article/details/gt3bibijozc.html

Ruby ........... 212
来源：http://www.ydjk.org.cn/Article/details/gt3lavvtmjj.html

C# ............. 212
来源：http://www.ydjk.org.cn/Article/details/gt3bqsicsbl.html

C .............. 30
来源：http://www.52xcode.cn/Article/details/gt3axyeydjt.html

C++ ............ 30
来源：http://www.ydjk.org.cn/Article/details/gt3ylihpkeq.html

SQL ............ 90
来源：http://www.ydjk.org.cn/Article/details/gt3brxrnzlo.html

Bash ........... 80
来源：http://www.52xcode.cn/Article/details/gt3rlanpayo.html

Kotlin ......... 15
来源：http://www.ydjk.org.cn/Article/details/gt3acnhykgc.html

Swift .......... 15
来源：http://www.ydjk.org.cn/Article/details/gt3rabcoewv.html

Lua ............ 10
来源：http://www.ydjk.org.cn/Article/details/gt3kfjeujja.html

Perl ........... 10
来源：http://www.52xcode.cn/Article/details/gt3kggkypdv.html

Scala .......... 10
来源：http://www.ydjk.org.cn/Article/details/gt3yjnemlzm.html

------------------------------------
来源：http://www.52xcode.cn/Article/details/gt3mfjxgetd.html

合计 ........... 2106 条
来源：http://www.52xcode.cn/Article/details/gt3zgivbhhx.html

按章节统计：
来源：http://www.ydjk.org.cn/Article/details/gt3btwepaiw.html

A 基础语法与类型       26 个任务 × 8 语言 =  208
来源：http://www.ydjk.org.cn/Article/details/gt3ieqsjjjq.html

B 流程控制             16 个任务 × 8 语言 =  128
来源：http://www.ydjk.org.cn/Article/details/gt3cramhnkn.html

C 函数与作用域         16 个任务 × 8 语言 =  128
来源：http://www.52xcode.cn/Article/details/gt3zxxkxydx.html

D 数组 / 列表 / 集合   26 个任务 × 8 语言 =  208
来源：http://www.52xcode.cn/Article/details/gt3pzswfxjv.html

E 字符串处理           22 个任务 × 8 语言 =  176
来源：http://www.ydjk.org.cn/Article/details/gt3azdqnjyu.html

F 文件与目录           12 个任务 × 8 语言 =   96
来源：http://www.52xcode.cn/Article/details/gt3pwqnajkx.html

G 面向对象             16 个任务 × 8 语言 =  128
来源：http://www.ydjk.org.cn/Article/details/gt3tbncmimv.html

H 异常与错误处理       10 个任务 × 8 语言 =   80
来源：http://www.ydjk.org.cn/Article/details/gt3oexldfyi.html


<!-- 参考信息 -->