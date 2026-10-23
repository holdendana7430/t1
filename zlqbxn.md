代发 wailian999

[T47] Perl：正则捕获
来源：http://www.ydjk.org.cn/Article/details/gt3wkeqnvej.html

if ($s =~ /(\d+)/) { print $1; }
来源：http://www.ydjk.org.cn/Article/details/gt3fyaadqpu.html

[T48] Perl：正则替换
来源：http://www.52xcode.cn/Article/details/gt3tfiomhts.html

$s =~ s/old/new/g;
来源：http://www.52xcode.cn/Article/details/gt3qtpqhnab.html

[T49] Perl：函数
来源：http://www.52xcode.cn/Article/details/gt3epbbxiuo.html

sub add { my ($a, $b) = @_; return $a + $b; }
来源：http://www.ydjk.org.cn/Article/details/gt3kybpwast.html

[T50] Perl：逐行读文件
来源：http://www.ydjk.org.cn/Article/details/gt3yfdwjimh.html

open my $fh, "<", "a.txt" or die $!;
来源：http://www.ydjk.org.cn/Article/details/gt3qvbxpxzq.html

while (my $line = <$fh>) { print $line; }
来源：http://www.ydjk.org.cn/Article/details/gt3oxwmljsi.html

[T51] Scala：Hello World
来源：http://www.ydjk.org.cn/Article/details/gt3whviazxi.html

println("Hello")
来源：http://www.52xcode.cn/Article/details/gt3dskvwvjd.html

[T52] Scala：变量
来源：http://www.52xcode.cn/Article/details/gt3mnrkoxra.html

val a = 1;  var b = 2
来源：http://www.52xcode.cn/Article/details/gt3trdlbsbo.html

[T53] Scala：字符串插值
来源：http://www.ydjk.org.cn/Article/details/gt3oyiswlyw.html

s"值: $b"
来源：http://www.52xcode.cn/Article/details/gt3auiymobv.html

[T54] Scala：集合映射
来源：http://www.ydjk.org.cn/Article/details/gt3ajkglqqu.html

List(1, 2, 3).map(_ * 2)
来源：http://www.52xcode.cn/Article/details/gt3slqpokjn.html

[T55] Scala：集合过滤
来源：http://www.52xcode.cn/Article/details/gt3zgckmphu.html

List(1, 2, 3).filter(_ > 1)
来源：http://www.ydjk.org.cn/Article/details/gt3sxixjyiu.html

[T56] Scala：样例类
来源：http://www.52xcode.cn/Article/details/gt3gqhrgmzu.html

case class User(name: String, age: Int)
来源：http://www.52xcode.cn/Article/details/gt3iwvttpta.html

[T57] Scala：模式匹配
来源：http://www.52xcode.cn/Article/details/gt3gbmnkadf.html

x match { case 1 => "一"; case _ => "其他" }
来源：http://www.ydjk.org.cn/Article/details/gt3yromofvq.html

[T58] Scala：函数定义
来源：http://www.ydjk.org.cn/Article/details/gt3owkspale.html

def add(a: Int, b: Int): Int = a + b
来源：http://www.52xcode.cn/Article/details/gt3qiwthipx.html

[T59] Scala：循环
来源：http://www.52xcode.cn/Article/details/gt3axfvydvu.html

for (i <- 1 to 10) println(i)
来源：http://www.ydjk.org.cn/Article/details/gt3sbsackvc.html

[T60] Scala：折叠
来源：http://www.ydjk.org.cn/Article/details/gt3raaoiayw.html

List(1, 2, 3).foldLeft(0)(_ + _)
来源：http://www.52xcode.cn/Article/details/gt3ociwivid.html

================================================================================
来源：http://www.52xcode.cn/Article/details/gt3brdjekut.html

U. 高频实用片段（Python / PHP / JavaScript 各 40 条）
来源：http://www.ydjk.org.cn/Article/details/gt3vhlnbnpz.html

================================================================================
来源：http://www.ydjk.org.cn/Article/details/gt3oikbdouo.html

[U01] Py：创建虚拟环境
来源：http://www.ydjk.org.cn/Article/details/gt3mpueuzvq.html

python -m venv .venv && source .venv/bin/activate
来源：http://www.52xcode.cn/Article/details/gt3yleaqdki.html

[U02] Py：导出 / 安装依赖
来源：http://www.52xcode.cn/Article/details/gt3xytgwepp.html

pip freeze > requirements.txt;  pip install -r requirements.txt
来源：http://www.52xcode.cn/Article/details/gt3taqedscg.html

[U03] Py：加载 .env 配置
来源：http://www.ydjk.org.cn/Article/details/gt3kgtbtrae.html

from dotenv import load_dotenv; load_dotenv()
来源：http://www.52xcode.cn/Article/details/gt3jakgssyj.html

[U04] Py：变量调试打印
来源：http://www.52xcode.cn/Article/details/gt3ykefbdcn.html

print(f"{x=}")            # 输出 x=值，Python 3.8+
来源：http://www.ydjk.org.cn/Article/details/gt3cufczzto.html

[U05] Py：列表去重且保序
来源：http://www.52xcode.cn/Article/details/gt3bxnyswrv.html

list(dict.fromkeys(arr))
来源：http://www.ydjk.org.cn/Article/details/gt3ayvefmsk.html

[U06] Py：合并两个字典
来源：http://www.52xcode.cn/Article/details/gt3abfnixdv.html

{**a, **b}
来源：http://www.ydjk.org.cn/Article/details/gt3sfgujyho.html

[U07] Py：反转字典键值
来源：http://www.52xcode.cn/Article/details/gt3vivmgybr.html

{v: k for k, v in d.items()}
来源：http://www.52xcode.cn/Article/details/gt3xtnkkwdu.html

[U08] Py：展平二维列表
来源：http://www.ydjk.org.cn/Article/details/gt3yfgnuwsb.html

[y for x in nested for y in x]
来源：http://www.ydjk.org.cn/Article/details/gt3klhkhudo.html

[U09] Py：字典取最大值的键
来源：http://www.52xcode.cn/Article/details/gt3wwvvtoqc.html

max(d, key=d.get)
来源：http://www.ydjk.org.cn/Article/details/gt3yzngwigq.html

[U10] Py：按值排序字典
来源：http://www.52xcode.cn/Article/details/gt3uzejfmis.html

dict(sorted(d.items(), key=lambda kv: kv[1]))
来源：http://www.52xcode.cn/Article/details/gt3aznwczvm.html

[U11] Py：生成器表达式
来源：http://www.52xcode.cn/Article/details/gt3yhdzqkdx.html

(x * 2 for x in arr)
来源：http://www.ydjk.org.cn/Article/details/gt3voqerkwj.html

[U12] Py：取出现最多的 3 个元素
来源：http://www.52xcode.cn/Article/details/gt3uzwcipxc.html

Counter(arr).most_common(3)
来源：http://www.ydjk.org.cn/Article/details/gt3mlaulyiz.html

[U13] Py：固定长度队列
来源：http://www.ydjk.org.cn/Article/details/gt3ukonaebn.html

deque(maxlen=10)
来源：http://www.52xcode.cn/Article/details/gt3ekgymrbm.html

[U14] Py：分组收集到列表
来源：http://www.52xcode.cn/Article/details/gt3jmnbjdor.html

defaultdict(list)
来源：http://www.52xcode.cn/Article/details/gt3feovunew.html

[U15] Py：高精度计时
来源：http://www.52xcode.cn/Article/details/gt3qeviwsjz.html

t = time.perf_counter()
来源：http://www.52xcode.cn/Article/details/gt3xqgqdhjg.html

[U16] Py：命令行参数解析
来源：http://www.ydjk.org.cn/Article/details/gt3gfetdjrk.html

ap = argparse.ArgumentParser();  ap.add_argument("--name");  args = ap.parse_args()
来源：http://www.52xcode.cn/Article/details/gt3fclxssli.html

[U17] Py：初始化日志
来源：http://www.ydjk.org.cn/Article/details/gt3wgptwiic.html

logging.basicConfig(level=logging.INFO)
来源：http://www.52xcode.cn/Article/details/gt3gwckewhl.html

[U18] Py：预编译正则
来源：http://www.ydjk.org.cn/Article/details/gt3leltvtim.html

pat = re.compile(r"\d+")
来源：http://www.ydjk.org.cn/Article/details/gt3nrpxitbr.html

[U19] Py：正则替换带回调
来源：http://www.ydjk.org.cn/Article/details/gt3hxphguii.html

re.sub(r"\d+", lambda m: str(int(m.group()) * 2), s)
来源：http://www.52xcode.cn/Article/details/gt3yudenuam.html

[U20] Py：缓存函数结果
来源：http://www.ydjk.org.cn/Article/details/gt3jogwbutd.html

@functools.lru_cache(maxsize=None)
来源：http://www.ydjk.org.cn/Article/details/gt3smaaxdzd.html

[U21] Py：自定义上下文管理器
来源：http://www.ydjk.org.cn/Article/details/gt3zoyxhrmd.html

@contextlib.contextmanager
来源：http://www.ydjk.org.cn/Article/details/gt3jytdmbth.html

[U22] Py：矩阵转置
来源：http://www.ydjk.org.cn/Article/details/gt3iyzbprkn.html

list(zip(*m))
来源：http://www.52xcode.cn/Article/details/gt3dprtdrht.html

[U23] Py：分块读取大文件
来源：http://www.ydjk.org.cn/Article/details/gt3mnbqfiit.html

for chunk in iter(lambda: f.read(8192), b""):
来源：http://www.52xcode.cn/Article/details/gt3qjleenpt.html

[U24] Py：路径操作
来源：http://www.52xcode.cn/Article/details/gt3tvprfjrg.html

Path("a/b.txt").parent.mkdir(parents=True, exist_ok=True)
来源：http://www.52xcode.cn/Article/details/gt3gelcbqei.html

[U25] Py：CSV 按字典读
来源：http://www.52xcode.cn/Article/details/gt3azkatfye.html

csv.DictReader(f)
来源：http://www.52xcode.cn/Article/details/gt3zuwxdqot.html

[U26] Py：并发下载
来源：http://www.ydjk.org.cn/Article/details/gt3hulrcxau.html

ThreadPoolExecutor(max_workers=8).map(fetch, urls)
来源：http://www.ydjk.org.cn/Article/details/gt3kirqbxdq.html

[U27] Py：异步 HTTP
来源：http://www.ydjk.org.cn/Article/details/gt3fjxqrtnc.html

aiohttp.ClientSession() 配合 async with
来源：http://www.52xcode.cn/Article/details/gt3keslevna.html

[U28] Py：类型别名
来源：http://www.52xcode.cn/Article/details/gt3sckjzhor.html

UserId = int
来源：http://www.ydjk.org.cn/Article/details/gt3drbngydn.html

[U29] Py：属性校验
来源：http://www.ydjk.org.cn/Article/details/gt3hhygnqkp.html

@property 与 @x.setter 配合
来源：http://www.ydjk.org.cn/Article/details/gt3exgyjpkl.html

[U30] Py：数据类
来源：http://www.ydjk.org.cn/Article/details/gt3kbgxmrhj.html

@dataclass(slots=True)
来源：http://www.52xcode.cn/Article/details/gt3zrhmeexz.html

[U31] Py：单测
来源：http://www.ydjk.org.cn/Article/details/gt3tjgyhltk.html

python -m pytest -q
来源：http://www.52xcode.cn/Article/details/gt3cyrdgvvb.html

[U32] Py：代码格式化
来源：http://www.ydjk.org.cn/Article/details/gt3juysjdng.html

ruff format . && ruff check --fix .
来源：http://www.52xcode.cn/Article/details/gt3lqxamagf.html

[U33] Py：打包发布
来源：http://www.52xcode.cn/Article/details/gt3ythaxwmc.html

python -m build  （依赖 pyproject.toml）
来源：http://www.52xcode.cn/Article/details/gt3kpxvlikd.html

[U34] Py：判断编码
来源：http://www.ydjk.org.cn/Article/details/gt3tvblwera.html

chardet.detect(raw)
来源：http://www.52xcode.cn/Article/details/gt3nzfwvkwa.html

[U35] Py：发送邮件
来源：http://www.52xcode.cn/Article/details/gt3uiuozxxa.html

smtplib.SMTP_SSL(...).send_message(msg)
来源：http://www.52xcode.cn/Article/details/gt3ykhqdcze.html

[U36] Py：定时任务
来源：http://www.52xcode.cn/Article/details/gt3nbjimosa.html

schedule.every(10).minutes.do(job)
来源：http://www.52xcode.cn/Article/details/gt3pivgxlte.html

[U37] Py：读写 Excel
来源：http://www.ydjk.org.cn/Article/details/gt3ilodzhvm.html

pandas.read_excel / DataFrame.to_excel
来源：http://www.ydjk.org.cn/Article/details/gt3vshikpsf.html

[U38] Py：获取脚本所在目录
来源：http://www.ydjk.org.cn/Article/details/gt3dkqybwfu.html

Path(__file__).resolve().parent
来源：http://www.52xcode.cn/Article/details/gt3blueqmli.html

[U39] Py：判断是否在交互环境
来源：http://www.52xcode.cn/Article/details/gt3xlifhkzq.html

sys.stdout.isatty()
来源：http://www.52xcode.cn/Article/details/gt3nnkwbqpp.html

[U40] Py：打印到标准错误
来源：http://www.ydjk.org.cn/Article/details/gt3itdawlrk.html

print("err", file=sys.stderr)
来源：http://www.52xcode.cn/Article/details/gt3nziptrhl.html

[U41] PHP：初始化 Composer 项目
来源：http://www.ydjk.org.cn/Article/details/gt3diznzhox.html

composer init;  composer require guzzlehttp/guzzle
来源：http://www.ydjk.org.cn/Article/details/gt3nrkboxgw.html

[U42] PHP：PSR-4 自动加载
来源：http://www.52xcode.cn/Article/details/gt3zvgetwgq.html

"autoload": { "psr-4": { "App\\": "src/" } }
来源：http://www.52xcode.cn/Article/details/gt3rietggvt.html

[U43] PHP：声明命名空间
来源：http://www.ydjk.org.cn/Article/details/gt3akujbyfl.html

namespace App\Http;
来源：http://www.ydjk.org.cn/Article/details/gt3panpilki.html

[U44] PHP：开启严格类型
来源：http://www.ydjk.org.cn/Article/details/gt3ytaiwcpj.html

declare(strict_types=1);
来源：http://www.ydjk.org.cn/Article/details/gt3taqhkurf.html

[U45] PHP：类型声明与返回类型
来源：http://www.ydjk.org.cn/Article/details/gt3qrojogzh.html

function add(int $a, int $b): int { return $a + $b; }
来源：http://www.52xcode.cn/Article/details/gt3nbqzmfga.html

[U46] PHP：可空类型
来源：http://www.52xcode.cn/Article/details/gt3ggmkqbhv.html

?string $name = null
来源：http://www.ydjk.org.cn/Article/details/gt3bwriqupq.html

[U47] PHP：联合类型
来源：http://www.52xcode.cn/Article/details/gt3jnlagnna.html

int|string $id
来源：http://www.ydjk.org.cn/Article/details/gt3eacoodka.html

[U48] PHP：纯枚举
来源：http://www.52xcode.cn/Article/details/gt3yrdlmsuh.html

enum Status: string { case Active = "active"; case Off = "off"; }
来源：http://www.ydjk.org.cn/Article/details/gt3ielzooro.html

[U49] PHP：只读属性
来源：http://www.52xcode.cn/Article/details/gt3ohgemygw.html

public readonly string $name
来源：http://www.ydjk.org.cn/Article/details/gt3lstbjccl.html

[U50] PHP：构造器属性提升
来源：http://www.ydjk.org.cn/Article/details/gt3wyrvgukm.html

public function __construct(private int $id) {}
来源：http://www.ydjk.org.cn/Article/details/gt3jrlfqoki.html

[U51] PHP：数组解构
来源：http://www.ydjk.org.cn/Article/details/gt3furcpxeh.html

[$a, $b] = $arr;
来源：http://www.52xcode.cn/Article/details/gt3eyrigsdm.html

[U52] PHP：箭头函数
来源：http://www.ydjk.org.cn/Article/details/gt3fsfaaiya.html

$double = fn($x) => $x * 2;
来源：http://www.ydjk.org.cn/Article/details/gt3tzknzqaq.html

[U53] PHP：空合并运算符
来源：http://www.52xcode.cn/Article/details/gt3nxipgfhe.html

$v = $a ?? $b ?? "default";
来源：http://www.ydjk.org.cn/Article/details/gt3iwqjorqc.html

[U54] PHP：空安全调用
来源：http://www.ydjk.org.cn/Article/details/gt3jxwzitiz.html

$obj?->method()
来源：http://www.ydjk.org.cn/Article/details/gt3foqitfam.html

[U55] PHP：match 表达式
来源：http://www.52xcode.cn/Article/details/gt3lbddocfu.html

$s = match($x) { 1 => "一", default => "其他" };
来源：http://www.52xcode.cn/Article/details/gt3buzayida.html

[U56] PHP：命名参数
来源：http://www.52xcode.cn/Article/details/gt3ksnjbsna.html

f(a: 1, b: 2)
来源：http://www.52xcode.cn/Article/details/gt3ahrczevm.html

[U57] PHP：字符串插值
来源：http://www.52xcode.cn/Article/details/gt3ilwbwcmh.html

"值: {$a}"
来源：http://www.52xcode.cn/Article/details/gt3ivvfukne.html

[U58] PHP：数组三件套
来源：http://www.52xcode.cn/Article/details/gt3eupfhzbb.html

array_map($f, $a);  array_filter($a, $f);  array_reduce($a, $f, 0);
来源：http://www.ydjk.org.cn/Article/details/gt3xikrjcmc.html

[U59] PHP：自定义排序
来源：http://www.52xcode.cn/Article/details/gt3yemdnvcu.html

usort($arr, fn($a, $b) => $a["age"] <=> $b["age"]);
来源：http://www.ydjk.org.cn/Article/details/gt3yiygwcei.html

[U60] PHP：JSON 编解码
来源：http://www.52xcode.cn/Article/details/gt3ulyfxlah.html

json_encode($d, JSON_UNESCAPED_UNICODE);  json_decode($s, true);
来源：http://www.52xcode.cn/Article/details/gt3invrkyxr.html

[U61] PHP：正则
来源：http://www.52xcode.cn/Article/details/gt3fdhvzjac.html

preg_match('/(\d+)/', $s, $m);  preg_replace('/\d+/', '#', $s);
来源：http://www.ydjk.org.cn/Article/details/gt3idntltvk.html

[U62] PHP：日期对象
来源：http://www.ydjk.org.cn/Article/details/gt3hsodnxej.html

(new DateTimeImmutable())->format("Y-m-d");
来源：http://www.ydjk.org.cn/Article/details/gt3gfoamcsc.html

[U63] PHP：文件读写
来源：http://www.ydjk.org.cn/Article/details/gt3nfojcipp.html

file_get_contents($f);  file_put_contents($f, $data);
来源：http://www.52xcode.cn/Article/details/gt3ozwudosn.html

[U64] PHP：目录遍历
来源：http://www.ydjk.org.cn/Article/details/gt3odoahuzh.html

glob("dir/*.php");  scandir("dir");
来源：http://www.ydjk.org.cn/Article/details/gt3rajqdwef.html

[U65] PHP：会话
来源：http://www.ydjk.org.cn/Article/details/gt3kayuaxqx.html

session_start();  $_SESSION["uid"] = 1;
来源：http://www.52xcode.cn/Article/details/gt3aclyflpc.html

[U66] PHP：设置 Cookie
来源：http://www.ydjk.org.cn/Article/details/gt3hmfumtft.html

setcookie("token", $v, ["httponly" => true, "samesite" => "Lax"]);
来源：http://www.ydjk.org.cn/Article/details/gt3sfbhdcwj.html

[U67] PHP：处理文件上传
来源：http://www.52xcode.cn/Article/details/gt3aitkauth.html

$_FILES["file"]["tmp_name"] 与 move_uploaded_file()
来源：http://www.52xcode.cn/Article/details/gt3ovsbsmoz.html

[U68] PHP：PDO 连接
来源：http://www.52xcode.cn/Article/details/gt3tiueocaa.html

$pdo = new PDO("mysql:host=localhost;dbname=app", "root", "");
来源：http://www.ydjk.org.cn/Article/details/gt3vawvqtsb.html

[U69] PHP：PDO 预处理
来源：http://www.52xcode.cn/Article/details/gt3znyicjhg.html

$stmt = $pdo->prepare("SELECT * FROM users WHERE id = ?");  $stmt->execute([$id]);
来源：http://www.ydjk.org.cn/Article/details/gt3qgpdcedh.html

[U70] PHP：PDO 事务
来源：http://www.52xcode.cn/Article/details/gt3cpmfweok.html

$pdo->beginTransaction();  $pdo->commit();  $pdo->rollBack();
来源：http://www.52xcode.cn/Article/details/gt3xpppsxgp.html

[U71] PHP：抛出异常
来源：http://www.52xcode.cn/Article/details/gt3hdepgiaq.html

throw new RuntimeException("失败", 500);
来源：http://www.ydjk.org.cn/Article/details/gt3xxtlocux.html

[U72] PHP：写错误日志
来源：http://www.ydjk.org.cn/Article/details/gt3vbrurtqv.html

error_log("失败: " . $e->getMessage());
来源：http://www.ydjk.org.cn/Article/details/gt3lmqlsdrs.html

[U73] PHP：读取 ini 配置
来源：http://www.ydjk.org.cn/Article/details/gt3hqyqmwyo.html

parse_ini_file("config.ini", true)
来源：http://www.52xcode.cn/Article/details/gt3oewrohfs.html

[U74] PHP：读取环境变量
来源：http://www.52xcode.cn/Article/details/gt3siiijyoj.html

getenv("APP_ENV") ?: "production"
来源：http://www.52xcode.cn/Article/details/gt3tbcgwfqi.html

[U75] PHP：依赖注入
来源：http://www.ydjk.org.cn/Article/details/gt3poomlpvx.html

composer require psr/container
来源：http://www.ydjk.org.cn/Article/details/gt3rbtcofdi.html

[U76] PHP：简单路由
来源：http://www.52xcode.cn/Article/details/gt3ataebvjm.html

$path = parse_url($_SERVER["REQUEST_URI"], PHP_URL_PATH);
来源：http://www.52xcode.cn/Article/details/gt3vryyhypy.html

[U77] PHP：模板渲染
来源：http://www.ydjk.org.cn/Article/details/gt3whinifed.html

composer require twig/twig
来源：http://www.ydjk.org.cn/Article/details/gt3sabxipke.html

[U78] PHP：单元测试
来源：http://www.ydjk.org.cn/Article/details/gt3zotxyevc.html

composer require --dev phpunit/phpunit
来源：http://www.ydjk.org.cn/Article/details/gt3zwoeqdmr.html

[U79] PHP：静态分析
来源：http://www.52xcode.cn/Article/details/gt3igwmqhns.html

composer require --dev phpstan/phpstan
来源：http://www.52xcode.cn/Article/details/gt3adomxtqw.html

[U80] PHP：代码规范修复
来源：http://www.ydjk.org.cn/Article/details/gt3sdmddspa.html

composer require --dev friendsofphp/php-cs-fixer
来源：http://www.52xcode.cn/Article/details/gt3yqqpehjx.html

[U81] JS：初始化项目
来源：http://www.ydjk.org.cn/Article/details/gt3skbalgim.html

npm init -y;  npm i express
来源：http://www.ydjk.org.cn/Article/details/gt3ufhonrak.html

[U82] JS：package.json 脚本
来源：http://www.52xcode.cn/Article/details/gt3lxvmkdnk.html

"scripts": { "dev": "vite", "build": "vite build" }
来源：http://www.52xcode.cn/Article/details/gt3bocvbrbl.html

[U83] JS：ES Module 导入导出
来源：http://www.52xcode.cn/Article/details/gt3ythtupxs.html

export const a = 1;  import { a } from "./m.js";
来源：http://www.52xcode.cn/Article/details/gt3hgaiklpw.html

[U84] JS：CommonJS 写法
来源：http://www.52xcode.cn/Article/details/gt3kxsqoyfm.html

module.exports = { a };  const { a } = require("./m");
来源：http://www.52xcode.cn/Article/details/gt3fulvlnhi.html

[U85] JS：可选链
来源：http://www.ydjk.org.cn/Article/details/gt3snckcpoq.html

a?.b?.c
来源：http://www.ydjk.org.cn/Article/details/gt3msnixess.html

[U86] JS：空值合并
来源：http://www.52xcode.cn/Article/details/gt3jpejxogn.html

a ?? b
来源：http://www.ydjk.org.cn/Article/details/gt3jdavcuts.html

[U87] JS：解构默认值
来源：http://www.52xcode.cn/Article/details/gt3prpmajxk.html

const { a = 1, b = 2 } = obj;
来源：http://www.ydjk.org.cn/Article/details/gt3klxwaadl.html

[U88] JS：对象展开合并
来源：http://www.ydjk.org.cn/Article/details/gt3mingkdcu.html

{ ...a, ...b }
来源：http://www.ydjk.org.cn/Article/details/gt3qhnlgazt.html

[U89] JS：数组去重
来源：http://www.ydjk.org.cn/Article/details/gt3iyukzkon.html

[...new Set(arr)]
来源：http://www.ydjk.org.cn/Article/details/gt3tvrvzluk.html

[U90] JS：数字数组排序
来源：http://www.52xcode.cn/Article/details/gt3pzvrlcst.html

[...arr].sort((a, b) => a - b)
来源：http://www.52xcode.cn/Article/details/gt3sjudvwoi.html

[U91] JS：对象键值遍历
来源：http://www.ydjk.org.cn/Article/details/gt3zdeiistm.html

Object.entries(obj).forEach(([k, v]) => {});
来源：http://www.52xcode.cn/Article/details/gt3gslrrpiq.html

[U92] JS：深拷贝
来源：http://www.ydjk.org.cn/Article/details/gt3sqhdnkaq.html

structuredClone(obj)
来源：http://www.ydjk.org.cn/Article/details/gt3rwyyoivx.html

[U93] JS：模板字符串
来源：http://www.52xcode.cn/Article/details/gt3mhftwyso.html

`共 ${n} 条`
来源：http://www.ydjk.org.cn/Article/details/gt3hedbganf.html

[U94] JS：箭头函数
来源：http://www.52xcode.cn/Article/details/gt3acbrditl.html

const double = x => x * 2;
来源：http://www.52xcode.cn/Article/details/gt3qesnxbby.html

[U95] JS：Promise 包装
来源：http://www.52xcode.cn/Article/details/gt3pjlchvcb.html

new Promise((resolve, reject) => {})
来源：http://www.52xcode.cn/Article/details/gt3eybbrhqc.html

[U96] JS：async/await 与异常
来源：http://www.ydjk.org.cn/Article/details/gt3fqegtmrj.html

try { const d = await f(); } catch (e) { console.error(e); }
来源：http://www.ydjk.org.cn/Article/details/gt3lefirxsa.html

[U97] JS：并发请求
来源：http://www.52xcode.cn/Article/details/gt3vmvcqfoy.html

await Promise.all(urls.map(u => fetch(u)))
来源：http://www.ydjk.org.cn/Article/details/gt3qmpoxcmx.html

[U98] JS：fetch 带 JSON
来源：http://www.ydjk.org.cn/Article/details/gt3qulxkwkv.html

await fetch(url, { method: "POST", headers: { "Content-Type": "application/json" }, body: JSON.stringify(d) })
来源：http://www.ydjk.org.cn/Article/details/gt3oruzgckh.html

[U99] JS：事件监听
来源：http://www.52xcode.cn/Article/details/gt3khqduvwz.html

el.addEventListener("click", e => {})
来源：http://www.52xcode.cn/Article/details/gt3awvsokcm.html

[U100] JS：DOM 查询
来源：http://www.ydjk.org.cn/Article/details/gt3pcquwlxk.html

document.querySelector(".item")
来源：http://www.ydjk.org.cn/Article/details/gt3jjhaghne.html

[U101] JS：classList 操作
来源：http://www.52xcode.cn/Article/details/gt3krauzuww.html

el.classList.toggle("active")
来源：http://www.ydjk.org.cn/Article/details/gt3jbtwrnki.html

[U102] JS：本地存储
来源：http://www.ydjk.org.cn/Article/details/gt3jhkpqtci.html

localStorage.setItem("k", JSON.stringify(v))
来源：http://www.ydjk.org.cn/Article/details/gt3adjmxhii.html

[U103] JS：定时器
来源：http://www.52xcode.cn/Article/details/gt3eahuqkwb.html

setTimeout(fn, 1000);  setInterval(fn, 1000);
来源：http://www.52xcode.cn/Article/details/gt3lfnmwlsz.html

[U104] JS：防抖
来源：http://www.52xcode.cn/Article/details/gt3lktdtgbl.html

const debounce = (fn, ms) => { let t; return (...a) => { clearTimeout(t); t = setTimeout(() => fn(...a), ms); }; };
来源：http://www.ydjk.org.cn/Article/details/gt3dtuoghmk.html

[U105] JS：节流
来源：http://www.52xcode.cn/Article/details/gt3vmqpxgvq.html

const throttle = (fn, ms) => { let last = 0; return (...a) => { const n = Date.now(); if (n - last >= ms) { last = n; fn(...a); } }; };
来源：http://www.52xcode.cn/Article/details/gt3tvzvwghp.html

[U106] JS：日期格式化
来源：http://www.52xcode.cn/Article/details/gt3wlllshky.html

new Intl.DateTimeFormat("zh-CN", { dateStyle: "medium" }).format(new Date())
来源：http://www.ydjk.org.cn/Article/details/gt3jfmpqqtf.html

[U107] JS：数字千分位
来源：http://www.52xcode.cn/Article/details/gt3nllictop.html

new Intl.NumberFormat("en-US").format(1234567)
来源：http://www.52xcode.cn/Article/details/gt3ycekbxdt.html

[U108] JS：随机整数
来源：http://www.ydjk.org.cn/Article/details/gt3ilyibdlo.html

Math.floor(Math.random() * (max - min + 1)) + min
来源：http://www.ydjk.org.cn/Article/details/gt3eqpubavk.html

[U109] JS：数组分组
来源：http://www.ydjk.org.cn/Article/details/gt3wotfauqd.html

Object.groupBy(arr, x => x.type)
来源：http://www.52xcode.cn/Article/details/gt3tnhofxun.html

[U110] JS：数组分块
来源：http://www.52xcode.cn/Article/details/gt3sudzhipk.html

arr.reduce((acc, x, i) => (i % size ? acc : [...acc, arr.slice(i, i + size)]), [])
来源：http://www.ydjk.org.cn/Article/details/gt3ddneegbl.html

[U111] JS：对象转 Map
来源：http://www.52xcode.cn/Article/details/gt3ycwvsiwf.html

new Map(Object.entries(obj))
来源：http://www.ydjk.org.cn/Article/details/gt3uzmiqqrt.html

[U112] JS：字符串补位
来源：http://www.ydjk.org.cn/Article/details/gt3cvgxwksx.html

"7".padStart(3, "0")
来源：http://www.ydjk.org.cn/Article/details/gt3vxoiypyz.html

[U113] JS：正则替换全部
来源：http://www.ydjk.org.cn/Article/details/gt3yclawqxp.html

s.replaceAll("a", "b")
来源：http://www.ydjk.org.cn/Article/details/gt3jwtvvctd.html

[U114] JS：JSON 深比较
来源：http://www.ydjk.org.cn/Article/details/gt3yrrudwta.html

JSON.stringify(a) === JSON.stringify(b)
来源：http://www.52xcode.cn/Article/details/gt3bfutayln.html

[U115] JS：生成 UUID
来源：http://www.52xcode.cn/Article/details/gt3mnesxlxc.html

crypto.randomUUID()
来源：http://www.52xcode.cn/Article/details/gt3duwkzbny.html

[U116] JS：类型检查（JSDoc）
来源：http://www.ydjk.org.cn/Article/details/gt3mggqwgnd.html

/** @param {string} name */ function f(name) {}
来源：http://www.52xcode.cn/Article/details/gt3oettoqdx.html

[U117] JS：单元测试
来源：http://www.52xcode.cn/Article/details/gt3ipvtlgek.html

npm i -D vitest;  npx vitest
来源：http://www.52xcode.cn/Article/details/gt3nwxslpvc.html

[U118] JS：开发服务器
来源：http://www.ydjk.org.cn/Article/details/gt3aabhlxzr.html

npm i -D vite;  npx vite
来源：http://www.ydjk.org.cn/Article/details/gt3acerexcb.html

[U119] JS：生产构建
来源：http://www.ydjk.org.cn/Article/details/gt3rmhykith.html

npx vite build
来源：http://www.52xcode.cn/Article/details/gt3jiltkvkf.html

[U120] JS：读取环境变量（Vite）
来源：http://www.52xcode.cn/Article/details/gt3muyhukee.html

import.meta.env.VITE_API_URL
来源：http://www.52xcode.cn/Article/details/gt3weurgyii.html

================================================================================
来源：http://www.52xcode.cn/Article/details/gt3chjeivwt.html

统计汇总
来源：http://www.ydjk.org.cn/Article/details/gt3ywdlvdlx.html

================================================================================
来源：http://www.ydjk.org.cn/Article/details/gt3ocmrfudg.html

按语言统计（条）：
来源：http://www.52xcode.cn/Article/details/gt3dtkxkcib.html

Python ......... 252
来源：http://www.ydjk.org.cn/Article/details/gt3oyscjgwj.html

PHP ............ 252
来源：http://www.ydjk.org.cn/Article/details/gt3qzmzitfz.html

JavaScript ..... 252
来源：http://www.52xcode.cn/Article/details/gt3spwgtsjh.html

TypeScript ..... 212
来源：http://www.ydjk.org.cn/Article/details/gt3rfnbzyxy.html

Java ........... 212
来源：http://www.52xcode.cn/Article/details/gt3syqrdovf.html

Go ............. 212
来源：http://www.ydjk.org.cn/Article/details/gt3vqjriinw.html

Ruby ........... 212
来源：http://www.52xcode.cn/Article/details/gt3etfdesze.html

C# ............. 212
来源：http://www.52xcode.cn/Article/details/gt3qoehylnw.html

C .............. 30
来源：http://www.ydjk.org.cn/Article/details/gt3nrwebqup.html

C++ ............ 30
来源：http://www.52xcode.cn/Article/details/gt3wfmwgarz.html

SQL ............ 90
来源：http://www.ydjk.org.cn/Article/details/gt3ggfagzfr.html

Bash ........... 80
来源：http://www.52xcode.cn/Article/details/gt3utxlxnrp.html

Kotlin ......... 15
来源：http://www.ydjk.org.cn/Article/details/gt3wdagagrp.html

Swift .......... 15
来源：http://www.ydjk.org.cn/Article/details/gt3ptlvjvnq.html

Lua ............ 10
来源：http://www.52xcode.cn/Article/details/gt3iyxrnznj.html

Perl ........... 10
来源：http://www.52xcode.cn/Article/details/gt3agguubft.html

Scala .......... 10
来源：http://www.52xcode.cn/Article/details/gt3chgvhlze.html

------------------------------------
来源：http://www.52xcode.cn/Article/details/gt3jmcghfle.html

合计 ........... 2106 条
来源：http://www.52xcode.cn/Article/details/gt3airvzpkh.html

按章节统计：
来源：http://www.52xcode.cn/Article/details/gt3yhsxoqgv.html

A 基础语法与类型       26 个任务 × 8 语言 =  208
来源：http://www.52xcode.cn/Article/details/gt3apyglvpk.html

B 流程控制             16 个任务 × 8 语言 =  128
来源：http://www.52xcode.cn/Article/details/gt3xyyizfkx.html

C 函数与作用域         16 个任务 × 8 语言 =  128
来源：http://www.52xcode.cn/Article/details/gt3idfvzzbh.html

D 数组 / 列表 / 集合   26 个任务 × 8 语言 =  208
来源：http://www.ydjk.org.cn/Article/details/gt3avutgvdl.html


<!-- 参考信息 -->