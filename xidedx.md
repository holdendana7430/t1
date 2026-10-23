代发 wailian999

[T49] Perl：函数
来源：http://www.52xcode.cn/Article/details/gt3mnqpoxgo.html

sub add { my ($a, $b) = @_; return $a + $b; }
来源：http://www.52xcode.cn/Article/details/gt3zntnmljq.html

[T50] Perl：逐行读文件
来源：http://www.52xcode.cn/Article/details/gt3ultzfkbf.html

open my $fh, "<", "a.txt" or die $!;
来源：http://www.52xcode.cn/Article/details/gt3jcaxbeux.html

while (my $line = <$fh>) { print $line; }
来源：http://www.52xcode.cn/Article/details/gt3tgduqifk.html

[T51] Scala：Hello World
来源：http://www.52xcode.cn/Article/details/gt3whhvgltn.html

println("Hello")
来源：http://www.ydjk.org.cn/Article/details/gt3jkrmgxij.html

[T52] Scala：变量
来源：http://www.52xcode.cn/Article/details/gt3tabvijvi.html

val a = 1;  var b = 2
来源：http://www.ydjk.org.cn/Article/details/gt3lpixhqvn.html

[T53] Scala：字符串插值
来源：http://www.52xcode.cn/Article/details/gt3rrpsxtrv.html

s"值: $b"
来源：http://www.ydjk.org.cn/Article/details/gt3fxmsrhhj.html

[T54] Scala：集合映射
来源：http://www.ydjk.org.cn/Article/details/gt3wrhxekek.html

List(1, 2, 3).map(_ * 2)
来源：http://www.52xcode.cn/Article/details/gt3fuuvrhkr.html

[T55] Scala：集合过滤
来源：http://www.ydjk.org.cn/Article/details/gt3pzrtpevh.html

List(1, 2, 3).filter(_ > 1)
来源：http://www.52xcode.cn/Article/details/gt3ushgzkgw.html

[T56] Scala：样例类
来源：http://www.ydjk.org.cn/Article/details/gt3fpbuyzzv.html

case class User(name: String, age: Int)
来源：http://www.52xcode.cn/Article/details/gt3oltxrrgt.html

[T57] Scala：模式匹配
来源：http://www.52xcode.cn/Article/details/gt3rulzraja.html

x match { case 1 => "一"; case _ => "其他" }
来源：http://www.52xcode.cn/Article/details/gt3snctjpyx.html

[T58] Scala：函数定义
来源：http://www.52xcode.cn/Article/details/gt3qfelaktv.html

def add(a: Int, b: Int): Int = a + b
来源：http://www.ydjk.org.cn/Article/details/gt3lsocnltk.html

[T59] Scala：循环
来源：http://www.ydjk.org.cn/Article/details/gt3bossadks.html

for (i <- 1 to 10) println(i)
来源：http://www.52xcode.cn/Article/details/gt3pmvxbvhk.html

[T60] Scala：折叠
来源：http://www.52xcode.cn/Article/details/gt3ambswgvx.html

List(1, 2, 3).foldLeft(0)(_ + _)
来源：http://www.52xcode.cn/Article/details/gt3owbgcppx.html

================================================================================
来源：http://www.ydjk.org.cn/Article/details/gt3uoulnsqq.html

U. 高频实用片段（Python / PHP / JavaScript 各 40 条）
来源：http://www.ydjk.org.cn/Article/details/gt3irrvrpva.html

================================================================================
来源：http://www.52xcode.cn/Article/details/gt3uiwbuiza.html

[U01] Py：创建虚拟环境
来源：http://www.52xcode.cn/Article/details/gt3vtpmiirc.html

python -m venv .venv && source .venv/bin/activate
来源：http://www.ydjk.org.cn/Article/details/gt3wbyhxbhu.html

[U02] Py：导出 / 安装依赖
来源：http://www.ydjk.org.cn/Article/details/gt3ykzgvmla.html

pip freeze > requirements.txt;  pip install -r requirements.txt
来源：http://www.52xcode.cn/Article/details/gt3upjfmpwp.html

[U03] Py：加载 .env 配置
来源：http://www.ydjk.org.cn/Article/details/gt3qdkcwuxm.html

from dotenv import load_dotenv; load_dotenv()
来源：http://www.ydjk.org.cn/Article/details/gt3budmlbqb.html

[U04] Py：变量调试打印
来源：http://www.ydjk.org.cn/Article/details/gt3rxieqmdi.html

print(f"{x=}")            # 输出 x=值，Python 3.8+
来源：http://www.ydjk.org.cn/Article/details/gt3cxvzbxxk.html

[U05] Py：列表去重且保序
来源：http://www.ydjk.org.cn/Article/details/gt3payzfcnz.html

list(dict.fromkeys(arr))
来源：http://www.52xcode.cn/Article/details/gt3gckwvhvq.html

[U06] Py：合并两个字典
来源：http://www.ydjk.org.cn/Article/details/gt3lravzdcf.html

{**a, **b}
来源：http://www.52xcode.cn/Article/details/gt3yelkjizw.html

[U07] Py：反转字典键值
来源：http://www.52xcode.cn/Article/details/gt3gztfnyky.html

{v: k for k, v in d.items()}
来源：http://www.ydjk.org.cn/Article/details/gt3rrbhmhjp.html

[U08] Py：展平二维列表
来源：http://www.52xcode.cn/Article/details/gt3oielftfo.html

[y for x in nested for y in x]
来源：http://www.ydjk.org.cn/Article/details/gt3ylmvunoy.html

[U09] Py：字典取最大值的键
来源：http://www.52xcode.cn/Article/details/gt3nojqptro.html

max(d, key=d.get)
来源：http://www.52xcode.cn/Article/details/gt3tmhgkjin.html

[U10] Py：按值排序字典
来源：http://www.52xcode.cn/Article/details/gt3cemyiywq.html

dict(sorted(d.items(), key=lambda kv: kv[1]))
来源：http://www.52xcode.cn/Article/details/gt3lrivrcjl.html

[U11] Py：生成器表达式
来源：http://www.ydjk.org.cn/Article/details/gt3rsmnjmqy.html

(x * 2 for x in arr)
来源：http://www.52xcode.cn/Article/details/gt3ilqgcaii.html

[U12] Py：取出现最多的 3 个元素
来源：http://www.52xcode.cn/Article/details/gt3hkhaywxi.html

Counter(arr).most_common(3)
来源：http://www.52xcode.cn/Article/details/gt3lfrmjrfq.html

[U13] Py：固定长度队列
来源：http://www.52xcode.cn/Article/details/gt3hrmncdhn.html

deque(maxlen=10)
来源：http://www.52xcode.cn/Article/details/gt3obemojbs.html

[U14] Py：分组收集到列表
来源：http://www.ydjk.org.cn/Article/details/gt3ocfesuol.html

defaultdict(list)
来源：http://www.52xcode.cn/Article/details/gt3vpdtlxgo.html

[U15] Py：高精度计时
来源：http://www.ydjk.org.cn/Article/details/gt3qpuurwta.html

t = time.perf_counter()
来源：http://www.ydjk.org.cn/Article/details/gt3dgtyojhc.html

[U16] Py：命令行参数解析
来源：http://www.52xcode.cn/Article/details/gt3kdmnlcxg.html

ap = argparse.ArgumentParser();  ap.add_argument("--name");  args = ap.parse_args()
来源：http://www.ydjk.org.cn/Article/details/gt3zurgwqbe.html

[U17] Py：初始化日志
来源：http://www.ydjk.org.cn/Article/details/gt3bfzegogl.html

logging.basicConfig(level=logging.INFO)
来源：http://www.ydjk.org.cn/Article/details/gt3crjtbelu.html

[U18] Py：预编译正则
来源：http://www.52xcode.cn/Article/details/gt3tkeasseh.html

pat = re.compile(r"\d+")
来源：http://www.52xcode.cn/Article/details/gt3hmyvetva.html

[U19] Py：正则替换带回调
来源：http://www.52xcode.cn/Article/details/gt3nyufmffd.html

re.sub(r"\d+", lambda m: str(int(m.group()) * 2), s)
来源：http://www.ydjk.org.cn/Article/details/gt3dpziobif.html

[U20] Py：缓存函数结果
来源：http://www.ydjk.org.cn/Article/details/gt3qkntddgg.html

@functools.lru_cache(maxsize=None)
来源：http://www.52xcode.cn/Article/details/gt3bcuqdbbu.html

[U21] Py：自定义上下文管理器
来源：http://www.52xcode.cn/Article/details/gt3istpfujs.html

@contextlib.contextmanager
来源：http://www.ydjk.org.cn/Article/details/gt3efsmgosi.html

[U22] Py：矩阵转置
来源：http://www.ydjk.org.cn/Article/details/gt3kdxsprxh.html

list(zip(*m))
来源：http://www.ydjk.org.cn/Article/details/gt3hvgccidl.html

[U23] Py：分块读取大文件
来源：http://www.52xcode.cn/Article/details/gt3loidtwbs.html

for chunk in iter(lambda: f.read(8192), b""):
来源：http://www.52xcode.cn/Article/details/gt3zlypvwtj.html

[U24] Py：路径操作
来源：http://www.52xcode.cn/Article/details/gt3wyzukexb.html

Path("a/b.txt").parent.mkdir(parents=True, exist_ok=True)
来源：http://www.52xcode.cn/Article/details/gt3hxbvxdfw.html

[U25] Py：CSV 按字典读
来源：http://www.ydjk.org.cn/Article/details/gt3mkzmkimu.html

csv.DictReader(f)
来源：http://www.ydjk.org.cn/Article/details/gt3clqsxpwj.html

[U26] Py：并发下载
来源：http://www.ydjk.org.cn/Article/details/gt3ydesynev.html

ThreadPoolExecutor(max_workers=8).map(fetch, urls)
来源：http://www.52xcode.cn/Article/details/gt3tgbmkknr.html

[U27] Py：异步 HTTP
来源：http://www.ydjk.org.cn/Article/details/gt3dqnitqgr.html

aiohttp.ClientSession() 配合 async with
来源：http://www.ydjk.org.cn/Article/details/gt3luowiuuf.html

[U28] Py：类型别名
来源：http://www.52xcode.cn/Article/details/gt3wgisgbnj.html

UserId = int
来源：http://www.52xcode.cn/Article/details/gt3pntfwmzj.html

[U29] Py：属性校验
来源：http://www.ydjk.org.cn/Article/details/gt3hcsjcsqw.html

@property 与 @x.setter 配合
来源：http://www.ydjk.org.cn/Article/details/gt3bdldvqmd.html

[U30] Py：数据类
来源：http://www.52xcode.cn/Article/details/gt3ytjmgpyf.html

@dataclass(slots=True)
来源：http://www.ydjk.org.cn/Article/details/gt3lgmbxzly.html

[U31] Py：单测
来源：http://www.52xcode.cn/Article/details/gt3vxvrqfok.html

python -m pytest -q
来源：http://www.ydjk.org.cn/Article/details/gt3gmtwunah.html

[U32] Py：代码格式化
来源：http://www.52xcode.cn/Article/details/gt3stsqvfad.html

ruff format . && ruff check --fix .
来源：http://www.ydjk.org.cn/Article/details/gt3ztnurbad.html

[U33] Py：打包发布
来源：http://www.52xcode.cn/Article/details/gt3brqdxhri.html

python -m build  （依赖 pyproject.toml）
来源：http://www.52xcode.cn/Article/details/gt3zveyekmn.html

[U34] Py：判断编码
来源：http://www.52xcode.cn/Article/details/gt3xvwffmxw.html

chardet.detect(raw)
来源：http://www.ydjk.org.cn/Article/details/gt3ycrymfum.html

[U35] Py：发送邮件
来源：http://www.ydjk.org.cn/Article/details/gt3memhmxyo.html

smtplib.SMTP_SSL(...).send_message(msg)
来源：http://www.ydjk.org.cn/Article/details/gt3evrglldd.html

[U36] Py：定时任务
来源：http://www.ydjk.org.cn/Article/details/gt3nlmwoifs.html

schedule.every(10).minutes.do(job)
来源：http://www.52xcode.cn/Article/details/gt3pkjmzrbs.html

[U37] Py：读写 Excel
来源：http://www.ydjk.org.cn/Article/details/gt3ndapahpr.html

pandas.read_excel / DataFrame.to_excel
来源：http://www.52xcode.cn/Article/details/gt3ulacdpvi.html

[U38] Py：获取脚本所在目录
来源：http://www.52xcode.cn/Article/details/gt3vyucquhd.html

Path(__file__).resolve().parent
来源：http://www.ydjk.org.cn/Article/details/gt3ylryftfe.html

[U39] Py：判断是否在交互环境
来源：http://www.ydjk.org.cn/Article/details/gt3irtqjgwq.html

sys.stdout.isatty()
来源：http://www.52xcode.cn/Article/details/gt3lvamycmd.html

[U40] Py：打印到标准错误
来源：http://www.ydjk.org.cn/Article/details/gt3frwkobvy.html

print("err", file=sys.stderr)
来源：http://www.52xcode.cn/Article/details/gt3bzvnbqdx.html

[U41] PHP：初始化 Composer 项目
来源：http://www.52xcode.cn/Article/details/gt3amupkjkd.html

composer init;  composer require guzzlehttp/guzzle
来源：http://www.ydjk.org.cn/Article/details/gt3asmrjwlp.html

[U42] PHP：PSR-4 自动加载
来源：http://www.52xcode.cn/Article/details/gt3kofvrvfg.html

"autoload": { "psr-4": { "App\\": "src/" } }
来源：http://www.ydjk.org.cn/Article/details/gt3joudkqak.html

[U43] PHP：声明命名空间
来源：http://www.52xcode.cn/Article/details/gt3apabbipo.html

namespace App\Http;
来源：http://www.52xcode.cn/Article/details/gt3iueooyso.html

[U44] PHP：开启严格类型
来源：http://www.52xcode.cn/Article/details/gt3eazslhrr.html

declare(strict_types=1);
来源：http://www.ydjk.org.cn/Article/details/gt3kkrmdvfu.html

[U45] PHP：类型声明与返回类型
来源：http://www.52xcode.cn/Article/details/gt3vdcpkcpg.html

function add(int $a, int $b): int { return $a + $b; }
来源：http://www.52xcode.cn/Article/details/gt3lgpijcbu.html

[U46] PHP：可空类型
来源：http://www.ydjk.org.cn/Article/details/gt3jnaqxauu.html

?string $name = null
来源：http://www.ydjk.org.cn/Article/details/gt3yturajxl.html

[U47] PHP：联合类型
来源：http://www.52xcode.cn/Article/details/gt3bpdmovsw.html

int|string $id
来源：http://www.52xcode.cn/Article/details/gt3slysbnya.html

[U48] PHP：纯枚举
来源：http://www.ydjk.org.cn/Article/details/gt3cjnqczaf.html

enum Status: string { case Active = "active"; case Off = "off"; }
来源：http://www.ydjk.org.cn/Article/details/gt3slfbltph.html

[U49] PHP：只读属性
来源：http://www.ydjk.org.cn/Article/details/gt3cbtlqwdb.html

public readonly string $name
来源：http://www.ydjk.org.cn/Article/details/gt3fzwtbzqd.html

[U50] PHP：构造器属性提升
来源：http://www.52xcode.cn/Article/details/gt3icnmcpwl.html

public function __construct(private int $id) {}
来源：http://www.52xcode.cn/Article/details/gt3iufrsaqi.html

[U51] PHP：数组解构
来源：http://www.52xcode.cn/Article/details/gt3jmfmwlnb.html

[$a, $b] = $arr;
来源：http://www.52xcode.cn/Article/details/gt3hcltrzbf.html

[U52] PHP：箭头函数
来源：http://www.52xcode.cn/Article/details/gt3terfzgbn.html

$double = fn($x) => $x * 2;
来源：http://www.52xcode.cn/Article/details/gt3bjnnsqpm.html

[U53] PHP：空合并运算符
来源：http://www.52xcode.cn/Article/details/gt3gfpasmun.html

$v = $a ?? $b ?? "default";
来源：http://www.ydjk.org.cn/Article/details/gt3toriserl.html

[U54] PHP：空安全调用
来源：http://www.52xcode.cn/Article/details/gt3lupbncam.html

$obj?->method()
来源：http://www.52xcode.cn/Article/details/gt3qdtofdup.html

[U55] PHP：match 表达式
来源：http://www.52xcode.cn/Article/details/gt3xdxnztcx.html

$s = match($x) { 1 => "一", default => "其他" };
来源：http://www.ydjk.org.cn/Article/details/gt3bwucqweb.html

[U56] PHP：命名参数
来源：http://www.52xcode.cn/Article/details/gt3hhdflvyz.html

f(a: 1, b: 2)
来源：http://www.52xcode.cn/Article/details/gt3memlmjnh.html

[U57] PHP：字符串插值
来源：http://www.ydjk.org.cn/Article/details/gt3fveztwwq.html

"值: {$a}"
来源：http://www.ydjk.org.cn/Article/details/gt3pzfbwiup.html

[U58] PHP：数组三件套
来源：http://www.52xcode.cn/Article/details/gt3cjundupa.html

array_map($f, $a);  array_filter($a, $f);  array_reduce($a, $f, 0);
来源：http://www.ydjk.org.cn/Article/details/gt3daldztdu.html

[U59] PHP：自定义排序
来源：http://www.52xcode.cn/Article/details/gt3xirgtftz.html

usort($arr, fn($a, $b) => $a["age"] <=> $b["age"]);
来源：http://www.ydjk.org.cn/Article/details/gt3pkbcexnx.html

[U60] PHP：JSON 编解码
来源：http://www.52xcode.cn/Article/details/gt3yyzwxlce.html

json_encode($d, JSON_UNESCAPED_UNICODE);  json_decode($s, true);
来源：http://www.ydjk.org.cn/Article/details/gt3pijakonn.html

[U61] PHP：正则
来源：http://www.ydjk.org.cn/Article/details/gt3kqudpeil.html

preg_match('/(\d+)/', $s, $m);  preg_replace('/\d+/', '#', $s);
来源：http://www.ydjk.org.cn/Article/details/gt3yudctunw.html

[U62] PHP：日期对象
来源：http://www.52xcode.cn/Article/details/gt3pslijerq.html

(new DateTimeImmutable())->format("Y-m-d");
来源：http://www.52xcode.cn/Article/details/gt3vxxeerco.html

[U63] PHP：文件读写
来源：http://www.52xcode.cn/Article/details/gt3fyctfxwn.html

file_get_contents($f);  file_put_contents($f, $data);
来源：http://www.ydjk.org.cn/Article/details/gt3wzzugwdd.html

[U64] PHP：目录遍历
来源：http://www.ydjk.org.cn/Article/details/gt3fpyzyhyj.html

glob("dir/*.php");  scandir("dir");
来源：http://www.52xcode.cn/Article/details/gt3wpxenvrt.html

[U65] PHP：会话
来源：http://www.ydjk.org.cn/Article/details/gt3votyivhw.html

session_start();  $_SESSION["uid"] = 1;
来源：http://www.ydjk.org.cn/Article/details/gt3unufqybu.html

[U66] PHP：设置 Cookie
来源：http://www.52xcode.cn/Article/details/gt3piyalvao.html

setcookie("token", $v, ["httponly" => true, "samesite" => "Lax"]);
来源：http://www.ydjk.org.cn/Article/details/gt3wtwfcwlm.html

[U67] PHP：处理文件上传
来源：http://www.ydjk.org.cn/Article/details/gt3nspowiuc.html

$_FILES["file"]["tmp_name"] 与 move_uploaded_file()
来源：http://www.52xcode.cn/Article/details/gt3ljwzvxoq.html

[U68] PHP：PDO 连接
来源：http://www.ydjk.org.cn/Article/details/gt3ekwqqrtw.html

$pdo = new PDO("mysql:host=localhost;dbname=app", "root", "");
来源：http://www.ydjk.org.cn/Article/details/gt3qpmsvren.html

[U69] PHP：PDO 预处理
来源：http://www.52xcode.cn/Article/details/gt3rxmzoves.html

$stmt = $pdo->prepare("SELECT * FROM users WHERE id = ?");  $stmt->execute([$id]);
来源：http://www.52xcode.cn/Article/details/gt3nbxpgsxn.html

[U70] PHP：PDO 事务
来源：http://www.ydjk.org.cn/Article/details/gt3jnftxdwb.html

$pdo->beginTransaction();  $pdo->commit();  $pdo->rollBack();
来源：http://www.ydjk.org.cn/Article/details/gt3laejoizl.html

[U71] PHP：抛出异常
来源：http://www.52xcode.cn/Article/details/gt3jwudaylq.html

throw new RuntimeException("失败", 500);
来源：http://www.ydjk.org.cn/Article/details/gt3rlekgmue.html

[U72] PHP：写错误日志
来源：http://www.ydjk.org.cn/Article/details/gt3wrcqzjam.html

error_log("失败: " . $e->getMessage());
来源：http://www.52xcode.cn/Article/details/gt3jfykvzkh.html

[U73] PHP：读取 ini 配置
来源：http://www.ydjk.org.cn/Article/details/gt3odtjlwhs.html

parse_ini_file("config.ini", true)
来源：http://www.ydjk.org.cn/Article/details/gt3cgjtvpxs.html

[U74] PHP：读取环境变量
来源：http://www.52xcode.cn/Article/details/gt3fqqpkxpm.html

getenv("APP_ENV") ?: "production"
来源：http://www.52xcode.cn/Article/details/gt3zeplrfln.html

[U75] PHP：依赖注入
来源：http://www.52xcode.cn/Article/details/gt3gabuayww.html

composer require psr/container
来源：http://www.ydjk.org.cn/Article/details/gt3adsmrloe.html

[U76] PHP：简单路由
来源：http://www.ydjk.org.cn/Article/details/gt3bodhiklj.html

$path = parse_url($_SERVER["REQUEST_URI"], PHP_URL_PATH);
来源：http://www.ydjk.org.cn/Article/details/gt3ilrdbuvz.html

[U77] PHP：模板渲染
来源：http://www.ydjk.org.cn/Article/details/gt3rtzpsurn.html

composer require twig/twig
来源：http://www.ydjk.org.cn/Article/details/gt3olgldaob.html

[U78] PHP：单元测试
来源：http://www.52xcode.cn/Article/details/gt3ycjwnphj.html

composer require --dev phpunit/phpunit
来源：http://www.ydjk.org.cn/Article/details/gt3rkndbnfi.html

[U79] PHP：静态分析
来源：http://www.52xcode.cn/Article/details/gt3rhwukrcb.html

composer require --dev phpstan/phpstan
来源：http://www.52xcode.cn/Article/details/gt3reandbqp.html

[U80] PHP：代码规范修复
来源：http://www.52xcode.cn/Article/details/gt3okhbdmud.html

composer require --dev friendsofphp/php-cs-fixer
来源：http://www.52xcode.cn/Article/details/gt3oxxkbvrp.html

[U81] JS：初始化项目
来源：http://www.ydjk.org.cn/Article/details/gt3fakflryy.html

npm init -y;  npm i express
来源：http://www.ydjk.org.cn/Article/details/gt3lasnsewe.html

[U82] JS：package.json 脚本
来源：http://www.52xcode.cn/Article/details/gt3hivpjrid.html

"scripts": { "dev": "vite", "build": "vite build" }
来源：http://www.ydjk.org.cn/Article/details/gt3apwaffsq.html

[U83] JS：ES Module 导入导出
来源：http://www.52xcode.cn/Article/details/gt3hnzrklkj.html

export const a = 1;  import { a } from "./m.js";
来源：http://www.52xcode.cn/Article/details/gt3xgutoveg.html

[U84] JS：CommonJS 写法
来源：http://www.52xcode.cn/Article/details/gt3ugopmzbi.html

module.exports = { a };  const { a } = require("./m");
来源：http://www.52xcode.cn/Article/details/gt3ncmidyhz.html

[U85] JS：可选链
来源：http://www.ydjk.org.cn/Article/details/gt3xucswyvj.html

a?.b?.c
来源：http://www.52xcode.cn/Article/details/gt3zrmvzgro.html

[U86] JS：空值合并
来源：http://www.ydjk.org.cn/Article/details/gt3bhpkchff.html

a ?? b
来源：http://www.52xcode.cn/Article/details/gt3akwgfmlb.html

[U87] JS：解构默认值
来源：http://www.52xcode.cn/Article/details/gt3hzcijmkk.html

const { a = 1, b = 2 } = obj;
来源：http://www.ydjk.org.cn/Article/details/gt3fcnwwutk.html

[U88] JS：对象展开合并
来源：http://www.52xcode.cn/Article/details/gt3pdwhruev.html

{ ...a, ...b }
来源：http://www.ydjk.org.cn/Article/details/gt3zpkpozqr.html

[U89] JS：数组去重
来源：http://www.ydjk.org.cn/Article/details/gt3cpbnkvis.html

[...new Set(arr)]
来源：http://www.52xcode.cn/Article/details/gt3lftmdygp.html

[U90] JS：数字数组排序
来源：http://www.52xcode.cn/Article/details/gt3kpjjesme.html

[...arr].sort((a, b) => a - b)
来源：http://www.ydjk.org.cn/Article/details/gt3ydrduroe.html

[U91] JS：对象键值遍历
来源：http://www.52xcode.cn/Article/details/gt3fuvyletp.html

Object.entries(obj).forEach(([k, v]) => {});
来源：http://www.ydjk.org.cn/Article/details/gt3ytjycncb.html

[U92] JS：深拷贝
来源：http://www.ydjk.org.cn/Article/details/gt3uzlidogh.html

structuredClone(obj)
来源：http://www.ydjk.org.cn/Article/details/gt3ljhmxwfg.html

[U93] JS：模板字符串
来源：http://www.52xcode.cn/Article/details/gt3dfszcpoa.html

`共 ${n} 条`
来源：http://www.52xcode.cn/Article/details/gt3uodxlcyi.html

[U94] JS：箭头函数
来源：http://www.52xcode.cn/Article/details/gt3prrqyyvp.html

const double = x => x * 2;
来源：http://www.52xcode.cn/Article/details/gt3laadcktf.html

[U95] JS：Promise 包装
来源：http://www.52xcode.cn/Article/details/gt3skrzdtwn.html

new Promise((resolve, reject) => {})
来源：http://www.52xcode.cn/Article/details/gt3fegcvisc.html

[U96] JS：async/await 与异常
来源：http://www.ydjk.org.cn/Article/details/gt3bvkoqdfn.html

try { const d = await f(); } catch (e) { console.error(e); }
来源：http://www.52xcode.cn/Article/details/gt3ftftdkpu.html

[U97] JS：并发请求
来源：http://www.52xcode.cn/Article/details/gt3bkymgrdd.html

await Promise.all(urls.map(u => fetch(u)))
来源：http://www.52xcode.cn/Article/details/gt3dqbxvlqg.html

[U98] JS：fetch 带 JSON
来源：http://www.52xcode.cn/Article/details/gt3neiskxdm.html

await fetch(url, { method: "POST", headers: { "Content-Type": "application/json" }, body: JSON.stringify(d) })
来源：http://www.52xcode.cn/Article/details/gt3bpnkvawk.html

[U99] JS：事件监听
来源：http://www.52xcode.cn/Article/details/gt3ywemsvni.html

el.addEventListener("click", e => {})
来源：http://www.52xcode.cn/Article/details/gt3kpuhwcpr.html

[U100] JS：DOM 查询
来源：http://www.ydjk.org.cn/Article/details/gt3csqaayyl.html

document.querySelector(".item")
来源：http://www.52xcode.cn/Article/details/gt3dkkgwhyw.html

[U101] JS：classList 操作
来源：http://www.52xcode.cn/Article/details/gt3javqttgt.html

el.classList.toggle("active")
来源：http://www.52xcode.cn/Article/details/gt3sltpgciu.html

[U102] JS：本地存储
来源：http://www.52xcode.cn/Article/details/gt3uhbraxhj.html

localStorage.setItem("k", JSON.stringify(v))
来源：http://www.52xcode.cn/Article/details/gt3xjfzmtce.html

[U103] JS：定时器
来源：http://www.ydjk.org.cn/Article/details/gt3shrjydzt.html

setTimeout(fn, 1000);  setInterval(fn, 1000);
来源：http://www.52xcode.cn/Article/details/gt3yjwetgqi.html

[U104] JS：防抖
来源：http://www.52xcode.cn/Article/details/gt3xnkpsdtq.html

const debounce = (fn, ms) => { let t; return (...a) => { clearTimeout(t); t = setTimeout(() => fn(...a), ms); }; };
来源：http://www.52xcode.cn/Article/details/gt3rcelybel.html

[U105] JS：节流
来源：http://www.ydjk.org.cn/Article/details/gt3wztorpcd.html

const throttle = (fn, ms) => { let last = 0; return (...a) => { const n = Date.now(); if (n - last >= ms) { last = n; fn(...a); } }; };
来源：http://www.52xcode.cn/Article/details/gt3xglubaoe.html

[U106] JS：日期格式化
来源：http://www.52xcode.cn/Article/details/gt3stlwrfnq.html

new Intl.DateTimeFormat("zh-CN", { dateStyle: "medium" }).format(new Date())
来源：http://www.ydjk.org.cn/Article/details/gt3ldtqogmr.html

[U107] JS：数字千分位
来源：http://www.52xcode.cn/Article/details/gt3xjbvnlia.html

new Intl.NumberFormat("en-US").format(1234567)
来源：http://www.52xcode.cn/Article/details/gt3azvyzivp.html

[U108] JS：随机整数
来源：http://www.52xcode.cn/Article/details/gt3kkjahhjn.html

Math.floor(Math.random() * (max - min + 1)) + min
来源：http://www.52xcode.cn/Article/details/gt3oqpwkzhg.html

[U109] JS：数组分组
来源：http://www.52xcode.cn/Article/details/gt3ilzvxnqx.html

Object.groupBy(arr, x => x.type)
来源：http://www.ydjk.org.cn/Article/details/gt3ukvguftk.html

[U110] JS：数组分块
来源：http://www.52xcode.cn/Article/details/gt3etiirvqq.html

arr.reduce((acc, x, i) => (i % size ? acc : [...acc, arr.slice(i, i + size)]), [])
来源：http://www.52xcode.cn/Article/details/gt3gzrmrsnt.html

[U111] JS：对象转 Map
来源：http://www.52xcode.cn/Article/details/gt3vyrwward.html

new Map(Object.entries(obj))
来源：http://www.ydjk.org.cn/Article/details/gt3rgrvjdul.html

[U112] JS：字符串补位
来源：http://www.52xcode.cn/Article/details/gt3tkzhmkxh.html

"7".padStart(3, "0")
来源：http://www.52xcode.cn/Article/details/gt3qdufabis.html

[U113] JS：正则替换全部
来源：http://www.52xcode.cn/Article/details/gt3nmhsncwv.html

s.replaceAll("a", "b")
来源：http://www.ydjk.org.cn/Article/details/gt3wcxdekro.html

[U114] JS：JSON 深比较
来源：http://www.ydjk.org.cn/Article/details/gt3ljatxkhb.html

JSON.stringify(a) === JSON.stringify(b)
来源：http://www.ydjk.org.cn/Article/details/gt3qnaegobq.html

[U115] JS：生成 UUID
来源：http://www.52xcode.cn/Article/details/gt3dvcwijqq.html

crypto.randomUUID()
来源：http://www.52xcode.cn/Article/details/gt3aoldhjcb.html

[U116] JS：类型检查（JSDoc）
来源：http://www.52xcode.cn/Article/details/gt3koyxjokp.html

/** @param {string} name */ function f(name) {}
来源：http://www.52xcode.cn/Article/details/gt3hbqmsbql.html

[U117] JS：单元测试
来源：http://www.ydjk.org.cn/Article/details/gt3vufcjuor.html

npm i -D vitest;  npx vitest
来源：http://www.ydjk.org.cn/Article/details/gt3yzfgowzn.html

[U118] JS：开发服务器
来源：http://www.52xcode.cn/Article/details/gt3dknotvrm.html

npm i -D vite;  npx vite
来源：http://www.ydjk.org.cn/Article/details/gt3zwwydvra.html

[U119] JS：生产构建
来源：http://www.ydjk.org.cn/Article/details/gt3fzztizvj.html

npx vite build
来源：http://www.ydjk.org.cn/Article/details/gt3epqqrhpr.html

[U120] JS：读取环境变量（Vite）
来源：http://www.ydjk.org.cn/Article/details/gt3razghqhd.html

import.meta.env.VITE_API_URL
来源：http://www.ydjk.org.cn/Article/details/gt3ysertxph.html

================================================================================
来源：http://www.ydjk.org.cn/Article/details/gt3togdmyfj.html

统计汇总
来源：http://www.ydjk.org.cn/Article/details/gt3zgrmgvbk.html

================================================================================
来源：http://www.52xcode.cn/Article/details/gt3ruauyuqr.html

按语言统计（条）：
来源：http://www.ydjk.org.cn/Article/details/gt3pkewfnkw.html

Python ......... 252
来源：http://www.52xcode.cn/Article/details/gt3icbrkgyb.html

PHP ............ 252
来源：http://www.ydjk.org.cn/Article/details/gt3xsgccktk.html

JavaScript ..... 252
来源：http://www.ydjk.org.cn/Article/details/gt3mhdqhdaz.html

TypeScript ..... 212
来源：http://www.ydjk.org.cn/Article/details/gt3rtzpamvl.html

Java ........... 212
来源：http://www.52xcode.cn/Article/details/gt3yrlfisuk.html

Go ............. 212
来源：http://www.52xcode.cn/Article/details/gt3swziyiul.html

Ruby ........... 212
来源：http://www.ydjk.org.cn/Article/details/gt3ceegmbiv.html

C# ............. 212
来源：http://www.ydjk.org.cn/Article/details/gt3zhqayale.html

C .............. 30
来源：http://www.52xcode.cn/Article/details/gt3myrfxnph.html

C++ ............ 30
来源：http://www.ydjk.org.cn/Article/details/gt3scvfsyxo.html

SQL ............ 90
来源：http://www.52xcode.cn/Article/details/gt3iuocausj.html

Bash ........... 80
来源：http://www.52xcode.cn/Article/details/gt3bwqfvqvt.html

Kotlin ......... 15
来源：http://www.ydjk.org.cn/Article/details/gt3qiizakag.html

Swift .......... 15
来源：http://www.52xcode.cn/Article/details/gt3cbdgaqct.html

Lua ............ 10
来源：http://www.52xcode.cn/Article/details/gt3pljsvkdm.html

Perl ........... 10
来源：http://www.52xcode.cn/Article/details/gt3pjltutqi.html

Scala .......... 10
来源：http://www.ydjk.org.cn/Article/details/gt3megubxpr.html

------------------------------------
来源：http://www.ydjk.org.cn/Article/details/gt3dufdwwfa.html

合计 ........... 2106 条
来源：http://www.52xcode.cn/Article/details/gt3ssbjpisq.html

按章节统计：
来源：http://www.ydjk.org.cn/Article/details/gt3ukwyyoqb.html

A 基础语法与类型       26 个任务 × 8 语言 =  208
来源：http://www.52xcode.cn/Article/details/gt3dhxplffw.html

B 流程控制             16 个任务 × 8 语言 =  128
来源：http://www.ydjk.org.cn/Article/details/gt3mxdrrysd.html

C 函数与作用域         16 个任务 × 8 语言 =  128
来源：http://www.ydjk.org.cn/Article/details/gt3ioyedmcx.html

D 数组 / 列表 / 集合   26 个任务 × 8 语言 =  208
来源：http://www.ydjk.org.cn/Article/details/gt3fsznpvjm.html

E 字符串处理           22 个任务 × 8 语言 =  176
来源：http://www.ydjk.org.cn/Article/details/gt3uhppsqsb.html

F 文件与目录           12 个任务 × 8 语言 =   96
来源：http://www.ydjk.org.cn/Article/details/gt3kjtwhleq.html

G 面向对象             16 个任务 × 8 语言 =  128
来源：http://www.52xcode.cn/Article/details/gt3zrcjurdu.html

H 异常与错误处理       10 个任务 × 8 语言 =   80
来源：http://www.52xcode.cn/Article/details/gt3xxjjgqdz.html


<!-- 参考信息 -->