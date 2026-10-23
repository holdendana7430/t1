代发 wailian999

[T49] Perl：函数
来源：http://www.52xcode.cn/Article/details/gt3lsticrel.html

sub add { my ($a, $b) = @_; return $a + $b; }
来源：http://www.52xcode.cn/Article/details/gt3pyrrobmv.html

[T50] Perl：逐行读文件
来源：http://www.52xcode.cn/Article/details/gt3xtragooy.html

open my $fh, "<", "a.txt" or die $!;
来源：http://www.ydjk.org.cn/Article/details/gt3vqffzweb.html

while (my $line = <$fh>) { print $line; }
来源：http://www.ydjk.org.cn/Article/details/gt3lzeveqds.html

[T51] Scala：Hello World
来源：http://www.52xcode.cn/Article/details/gt3turxjxov.html

println("Hello")
来源：http://www.ydjk.org.cn/Article/details/gt3aabcrsqt.html

[T52] Scala：变量
来源：http://www.52xcode.cn/Article/details/gt3aekugxqp.html

val a = 1;  var b = 2
来源：http://www.ydjk.org.cn/Article/details/gt3gdwpgpge.html

[T53] Scala：字符串插值
来源：http://www.ydjk.org.cn/Article/details/gt3uudbusiq.html

s"值: $b"
来源：http://www.52xcode.cn/Article/details/gt3mwtmpysn.html

[T54] Scala：集合映射
来源：http://www.52xcode.cn/Article/details/gt3elblzkno.html

List(1, 2, 3).map(_ * 2)
来源：http://www.52xcode.cn/Article/details/gt3xorayfou.html

[T55] Scala：集合过滤
来源：http://www.52xcode.cn/Article/details/gt3vdieonat.html

List(1, 2, 3).filter(_ > 1)
来源：http://www.52xcode.cn/Article/details/gt3sjlxwasf.html

[T56] Scala：样例类
来源：http://www.52xcode.cn/Article/details/gt3pvccatyb.html

case class User(name: String, age: Int)
来源：http://www.52xcode.cn/Article/details/gt3wgtstpmx.html

[T57] Scala：模式匹配
来源：http://www.ydjk.org.cn/Article/details/gt3nmwiuwjn.html

x match { case 1 => "一"; case _ => "其他" }
来源：http://www.ydjk.org.cn/Article/details/gt3axtzxeiy.html

[T58] Scala：函数定义
来源：http://www.ydjk.org.cn/Article/details/gt3phegrmyd.html

def add(a: Int, b: Int): Int = a + b
来源：http://www.52xcode.cn/Article/details/gt3toqkbgfp.html

[T59] Scala：循环
来源：http://www.52xcode.cn/Article/details/gt3okpukrbk.html

for (i <- 1 to 10) println(i)
来源：http://www.ydjk.org.cn/Article/details/gt3kxuloflr.html

[T60] Scala：折叠
来源：http://www.52xcode.cn/Article/details/gt3lilyvurh.html

List(1, 2, 3).foldLeft(0)(_ + _)
来源：http://www.52xcode.cn/Article/details/gt3aegxayij.html

================================================================================
来源：http://www.52xcode.cn/Article/details/gt3xmmwjcbp.html

U. 高频实用片段（Python / PHP / JavaScript 各 40 条）
来源：http://www.ydjk.org.cn/Article/details/gt3fncvkwsx.html

================================================================================
来源：http://www.52xcode.cn/Article/details/gt3atomyhvs.html

[U01] Py：创建虚拟环境
来源：http://www.ydjk.org.cn/Article/details/gt3lhuiqynt.html

python -m venv .venv && source .venv/bin/activate
来源：http://www.52xcode.cn/Article/details/gt3hhqebqww.html

[U02] Py：导出 / 安装依赖
来源：http://www.ydjk.org.cn/Article/details/gt3tdqlcskp.html

pip freeze > requirements.txt;  pip install -r requirements.txt
来源：http://www.52xcode.cn/Article/details/gt3gzrgfzkc.html

[U03] Py：加载 .env 配置
来源：http://www.ydjk.org.cn/Article/details/gt3vwdsohbv.html

from dotenv import load_dotenv; load_dotenv()
来源：http://www.ydjk.org.cn/Article/details/gt3hhgoqkxc.html

[U04] Py：变量调试打印
来源：http://www.ydjk.org.cn/Article/details/gt3xsnikzmy.html

print(f"{x=}")            # 输出 x=值，Python 3.8+
来源：http://www.ydjk.org.cn/Article/details/gt3smafvcob.html

[U05] Py：列表去重且保序
来源：http://www.ydjk.org.cn/Article/details/gt3vubnzgre.html

list(dict.fromkeys(arr))
来源：http://www.52xcode.cn/Article/details/gt3eohszmrs.html

[U06] Py：合并两个字典
来源：http://www.ydjk.org.cn/Article/details/gt3sntfetel.html

{**a, **b}
来源：http://www.52xcode.cn/Article/details/gt3jgkribxj.html

[U07] Py：反转字典键值
来源：http://www.52xcode.cn/Article/details/gt3lqirtcon.html

{v: k for k, v in d.items()}
来源：http://www.52xcode.cn/Article/details/gt3tetvbjga.html

[U08] Py：展平二维列表
来源：http://www.52xcode.cn/Article/details/gt3mmyypwpg.html

[y for x in nested for y in x]
来源：http://www.ydjk.org.cn/Article/details/gt3qnwcxjoe.html

[U09] Py：字典取最大值的键
来源：http://www.ydjk.org.cn/Article/details/gt3hppaooso.html

max(d, key=d.get)
来源：http://www.ydjk.org.cn/Article/details/gt3khecqqim.html

[U10] Py：按值排序字典
来源：http://www.ydjk.org.cn/Article/details/gt3csmurjvh.html

dict(sorted(d.items(), key=lambda kv: kv[1]))
来源：http://www.52xcode.cn/Article/details/gt3ppimwtvd.html

[U11] Py：生成器表达式
来源：http://www.ydjk.org.cn/Article/details/gt3bvypujcc.html

(x * 2 for x in arr)
来源：http://www.52xcode.cn/Article/details/gt3mzybhkdv.html

[U12] Py：取出现最多的 3 个元素
来源：http://www.52xcode.cn/Article/details/gt3dcnofyhw.html

Counter(arr).most_common(3)
来源：http://www.ydjk.org.cn/Article/details/gt3logswlhs.html

[U13] Py：固定长度队列
来源：http://www.52xcode.cn/Article/details/gt3dulldjvq.html

deque(maxlen=10)
来源：http://www.ydjk.org.cn/Article/details/gt3pjxqugol.html

[U14] Py：分组收集到列表
来源：http://www.ydjk.org.cn/Article/details/gt3acpzzxvv.html

defaultdict(list)
来源：http://www.52xcode.cn/Article/details/gt3zkhyjsbm.html

[U15] Py：高精度计时
来源：http://www.ydjk.org.cn/Article/details/gt3zjvuvbdf.html

t = time.perf_counter()
来源：http://www.ydjk.org.cn/Article/details/gt3eoxuvckn.html

[U16] Py：命令行参数解析
来源：http://www.ydjk.org.cn/Article/details/gt3jagbspqe.html

ap = argparse.ArgumentParser();  ap.add_argument("--name");  args = ap.parse_args()
来源：http://www.ydjk.org.cn/Article/details/gt3dmcfcnvs.html

[U17] Py：初始化日志
来源：http://www.ydjk.org.cn/Article/details/gt3mzrhprur.html

logging.basicConfig(level=logging.INFO)
来源：http://www.ydjk.org.cn/Article/details/gt3czbvxutp.html

[U18] Py：预编译正则
来源：http://www.ydjk.org.cn/Article/details/gt3sqzhzlkn.html

pat = re.compile(r"\d+")
来源：http://www.52xcode.cn/Article/details/gt3gfsptjth.html

[U19] Py：正则替换带回调
来源：http://www.52xcode.cn/Article/details/gt3aooxhvea.html

re.sub(r"\d+", lambda m: str(int(m.group()) * 2), s)
来源：http://www.52xcode.cn/Article/details/gt3oxgmzvyx.html

[U20] Py：缓存函数结果
来源：http://www.52xcode.cn/Article/details/gt3jbblkdhn.html

@functools.lru_cache(maxsize=None)
来源：http://www.52xcode.cn/Article/details/gt3jvvxfilx.html

[U21] Py：自定义上下文管理器
来源：http://www.52xcode.cn/Article/details/gt3zpolkvtg.html

@contextlib.contextmanager
来源：http://www.52xcode.cn/Article/details/gt3naozferz.html

[U22] Py：矩阵转置
来源：http://www.52xcode.cn/Article/details/gt3wxacqolc.html

list(zip(*m))
来源：http://www.52xcode.cn/Article/details/gt3densexxj.html

[U23] Py：分块读取大文件
来源：http://www.ydjk.org.cn/Article/details/gt3jyomkwrr.html

for chunk in iter(lambda: f.read(8192), b""):
来源：http://www.52xcode.cn/Article/details/gt3ellxbbeu.html

[U24] Py：路径操作
来源：http://www.52xcode.cn/Article/details/gt3lgkoifdw.html

Path("a/b.txt").parent.mkdir(parents=True, exist_ok=True)
来源：http://www.52xcode.cn/Article/details/gt3ipgwqayl.html

[U25] Py：CSV 按字典读
来源：http://www.ydjk.org.cn/Article/details/gt3badxysso.html

csv.DictReader(f)
来源：http://www.52xcode.cn/Article/details/gt3qynqhtjl.html

[U26] Py：并发下载
来源：http://www.52xcode.cn/Article/details/gt3xxlxibkr.html

ThreadPoolExecutor(max_workers=8).map(fetch, urls)
来源：http://www.ydjk.org.cn/Article/details/gt3hjllursz.html

[U27] Py：异步 HTTP
来源：http://www.52xcode.cn/Article/details/gt3mkqxtsmo.html

aiohttp.ClientSession() 配合 async with
来源：http://www.52xcode.cn/Article/details/gt3bbytkean.html

[U28] Py：类型别名
来源：http://www.ydjk.org.cn/Article/details/gt3agxawaik.html

UserId = int
来源：http://www.52xcode.cn/Article/details/gt3vjioqnzr.html

[U29] Py：属性校验
来源：http://www.52xcode.cn/Article/details/gt3cyqihegp.html

@property 与 @x.setter 配合
来源：http://www.ydjk.org.cn/Article/details/gt3gpvxrkfx.html

[U30] Py：数据类
来源：http://www.52xcode.cn/Article/details/gt3rkopvnrl.html

@dataclass(slots=True)
来源：http://www.ydjk.org.cn/Article/details/gt3tnwgugrh.html

[U31] Py：单测
来源：http://www.52xcode.cn/Article/details/gt3wrzntwxo.html

python -m pytest -q
来源：http://www.52xcode.cn/Article/details/gt3fqailjwj.html

[U32] Py：代码格式化
来源：http://www.ydjk.org.cn/Article/details/gt3baaphnwl.html

ruff format . && ruff check --fix .
来源：http://www.52xcode.cn/Article/details/gt3qulhqmkr.html

[U33] Py：打包发布
来源：http://www.ydjk.org.cn/Article/details/gt3rkscatwx.html

python -m build  （依赖 pyproject.toml）
来源：http://www.52xcode.cn/Article/details/gt3zfiogsho.html

[U34] Py：判断编码
来源：http://www.52xcode.cn/Article/details/gt3uvhgrbfb.html

chardet.detect(raw)
来源：http://www.ydjk.org.cn/Article/details/gt3fozikbsj.html

[U35] Py：发送邮件
来源：http://www.ydjk.org.cn/Article/details/gt3josxzpvf.html

smtplib.SMTP_SSL(...).send_message(msg)
来源：http://www.52xcode.cn/Article/details/gt3rgrbhjan.html

[U36] Py：定时任务
来源：http://www.ydjk.org.cn/Article/details/gt3odjxbqxd.html

schedule.every(10).minutes.do(job)
来源：http://www.ydjk.org.cn/Article/details/gt3tdxdcmof.html

[U37] Py：读写 Excel
来源：http://www.ydjk.org.cn/Article/details/gt3wwvuzbio.html

pandas.read_excel / DataFrame.to_excel
来源：http://www.ydjk.org.cn/Article/details/gt3alracrlx.html

[U38] Py：获取脚本所在目录
来源：http://www.ydjk.org.cn/Article/details/gt3rnirezpk.html

Path(__file__).resolve().parent
来源：http://www.52xcode.cn/Article/details/gt3zcvdhurl.html

[U39] Py：判断是否在交互环境
来源：http://www.ydjk.org.cn/Article/details/gt3bgvhakxw.html

sys.stdout.isatty()
来源：http://www.52xcode.cn/Article/details/gt3navmgbqj.html

[U40] Py：打印到标准错误
来源：http://www.52xcode.cn/Article/details/gt3dabybqph.html

print("err", file=sys.stderr)
来源：http://www.ydjk.org.cn/Article/details/gt3ughfbvsz.html

[U41] PHP：初始化 Composer 项目
来源：http://www.52xcode.cn/Article/details/gt3ykiuhmjd.html

composer init;  composer require guzzlehttp/guzzle
来源：http://www.ydjk.org.cn/Article/details/gt3voavgnmk.html

[U42] PHP：PSR-4 自动加载
来源：http://www.ydjk.org.cn/Article/details/gt3nxdqcmme.html

"autoload": { "psr-4": { "App\\": "src/" } }
来源：http://www.ydjk.org.cn/Article/details/gt3yfvmgdsx.html

[U43] PHP：声明命名空间
来源：http://www.ydjk.org.cn/Article/details/gt3exjzzipi.html

namespace App\Http;
来源：http://www.52xcode.cn/Article/details/gt3kwkzwmkh.html

[U44] PHP：开启严格类型
来源：http://www.52xcode.cn/Article/details/gt3thdmuqnx.html

declare(strict_types=1);
来源：http://www.52xcode.cn/Article/details/gt3afjdzqub.html

[U45] PHP：类型声明与返回类型
来源：http://www.ydjk.org.cn/Article/details/gt3wjqluqjw.html

function add(int $a, int $b): int { return $a + $b; }
来源：http://www.ydjk.org.cn/Article/details/gt3wkrvrurm.html

[U46] PHP：可空类型
来源：http://www.52xcode.cn/Article/details/gt3nwzbdebg.html

?string $name = null
来源：http://www.ydjk.org.cn/Article/details/gt3tdtbfzju.html

[U47] PHP：联合类型
来源：http://www.52xcode.cn/Article/details/gt3kdscdfbw.html

int|string $id
来源：http://www.52xcode.cn/Article/details/gt3tugcylfr.html

[U48] PHP：纯枚举
来源：http://www.ydjk.org.cn/Article/details/gt3lsznerek.html

enum Status: string { case Active = "active"; case Off = "off"; }
来源：http://www.52xcode.cn/Article/details/gt3zssjcuiu.html

[U49] PHP：只读属性
来源：http://www.ydjk.org.cn/Article/details/gt3wgcrzkuh.html

public readonly string $name
来源：http://www.ydjk.org.cn/Article/details/gt3ueohqeun.html

[U50] PHP：构造器属性提升
来源：http://www.52xcode.cn/Article/details/gt3fmnkmpzd.html

public function __construct(private int $id) {}
来源：http://www.ydjk.org.cn/Article/details/gt3ipaxfewi.html

[U51] PHP：数组解构
来源：http://www.52xcode.cn/Article/details/gt3kmoovwsr.html

[$a, $b] = $arr;
来源：http://www.52xcode.cn/Article/details/gt3cbeklqzp.html

[U52] PHP：箭头函数
来源：http://www.52xcode.cn/Article/details/gt3graornfs.html

$double = fn($x) => $x * 2;
来源：http://www.ydjk.org.cn/Article/details/gt3cfqenmfa.html

[U53] PHP：空合并运算符
来源：http://www.52xcode.cn/Article/details/gt3wjzggccw.html

$v = $a ?? $b ?? "default";
来源：http://www.ydjk.org.cn/Article/details/gt3cahjmquq.html

[U54] PHP：空安全调用
来源：http://www.52xcode.cn/Article/details/gt3uowlgtlx.html

$obj?->method()
来源：http://www.ydjk.org.cn/Article/details/gt3sdgbiikb.html

[U55] PHP：match 表达式
来源：http://www.52xcode.cn/Article/details/gt3blezoamw.html

$s = match($x) { 1 => "一", default => "其他" };
来源：http://www.ydjk.org.cn/Article/details/gt3irwbnees.html

[U56] PHP：命名参数
来源：http://www.52xcode.cn/Article/details/gt3dobnpsez.html

f(a: 1, b: 2)
来源：http://www.52xcode.cn/Article/details/gt3rswdrntu.html

[U57] PHP：字符串插值
来源：http://www.ydjk.org.cn/Article/details/gt3hljlenzo.html

"值: {$a}"
来源：http://www.52xcode.cn/Article/details/gt3mjbfivyu.html

[U58] PHP：数组三件套
来源：http://www.ydjk.org.cn/Article/details/gt3jrxtvbin.html

array_map($f, $a);  array_filter($a, $f);  array_reduce($a, $f, 0);
来源：http://www.52xcode.cn/Article/details/gt3viszilwm.html

[U59] PHP：自定义排序
来源：http://www.ydjk.org.cn/Article/details/gt3tuuixlkk.html

usort($arr, fn($a, $b) => $a["age"] <=> $b["age"]);
来源：http://www.52xcode.cn/Article/details/gt3znjmtvhh.html

[U60] PHP：JSON 编解码
来源：http://www.ydjk.org.cn/Article/details/gt3xcxvpnha.html

json_encode($d, JSON_UNESCAPED_UNICODE);  json_decode($s, true);
来源：http://www.ydjk.org.cn/Article/details/gt3mhxzxfxj.html

[U61] PHP：正则
来源：http://www.ydjk.org.cn/Article/details/gt3xdydzoov.html

preg_match('/(\d+)/', $s, $m);  preg_replace('/\d+/', '#', $s);
来源：http://www.52xcode.cn/Article/details/gt3nistljar.html

[U62] PHP：日期对象
来源：http://www.52xcode.cn/Article/details/gt3gtdxqely.html

(new DateTimeImmutable())->format("Y-m-d");
来源：http://www.52xcode.cn/Article/details/gt3udvujyol.html

[U63] PHP：文件读写
来源：http://www.52xcode.cn/Article/details/gt3aishspml.html

file_get_contents($f);  file_put_contents($f, $data);
来源：http://www.ydjk.org.cn/Article/details/gt3lljmafpr.html

[U64] PHP：目录遍历
来源：http://www.ydjk.org.cn/Article/details/gt3taetehgo.html

glob("dir/*.php");  scandir("dir");
来源：http://www.52xcode.cn/Article/details/gt3kzlqiezk.html

[U65] PHP：会话
来源：http://www.ydjk.org.cn/Article/details/gt3zjjtgksx.html

session_start();  $_SESSION["uid"] = 1;
来源：http://www.ydjk.org.cn/Article/details/gt3hykgvsyl.html

[U66] PHP：设置 Cookie
来源：http://www.52xcode.cn/Article/details/gt3zdvfoxjo.html

setcookie("token", $v, ["httponly" => true, "samesite" => "Lax"]);
来源：http://www.ydjk.org.cn/Article/details/gt3zhxzgzte.html

[U67] PHP：处理文件上传
来源：http://www.ydjk.org.cn/Article/details/gt3pxxpnefi.html

$_FILES["file"]["tmp_name"] 与 move_uploaded_file()
来源：http://www.ydjk.org.cn/Article/details/gt3wlskjjih.html

[U68] PHP：PDO 连接
来源：http://www.ydjk.org.cn/Article/details/gt3vtjcwuzu.html

$pdo = new PDO("mysql:host=localhost;dbname=app", "root", "");
来源：http://www.52xcode.cn/Article/details/gt3thtzkljv.html

[U69] PHP：PDO 预处理
来源：http://www.52xcode.cn/Article/details/gt3dxhfrlar.html

$stmt = $pdo->prepare("SELECT * FROM users WHERE id = ?");  $stmt->execute([$id]);
来源：http://www.52xcode.cn/Article/details/gt3hynfrovy.html

[U70] PHP：PDO 事务
来源：http://www.ydjk.org.cn/Article/details/gt3ubnisbsa.html

$pdo->beginTransaction();  $pdo->commit();  $pdo->rollBack();
来源：http://www.ydjk.org.cn/Article/details/gt3umxiodpd.html

[U71] PHP：抛出异常
来源：http://www.52xcode.cn/Article/details/gt3oiyjdnih.html

throw new RuntimeException("失败", 500);
来源：http://www.ydjk.org.cn/Article/details/gt3wwbnetbc.html

[U72] PHP：写错误日志
来源：http://www.ydjk.org.cn/Article/details/gt3yvkhiurf.html

error_log("失败: " . $e->getMessage());
来源：http://www.ydjk.org.cn/Article/details/gt3vvcouzsy.html

[U73] PHP：读取 ini 配置
来源：http://www.52xcode.cn/Article/details/gt3qdzerwsa.html

parse_ini_file("config.ini", true)
来源：http://www.52xcode.cn/Article/details/gt3blqlfazq.html

[U74] PHP：读取环境变量
来源：http://www.ydjk.org.cn/Article/details/gt3ivdstbei.html

getenv("APP_ENV") ?: "production"
来源：http://www.ydjk.org.cn/Article/details/gt3wuqldfjw.html

[U75] PHP：依赖注入
来源：http://www.ydjk.org.cn/Article/details/gt3qbmqfifz.html

composer require psr/container
来源：http://www.52xcode.cn/Article/details/gt3wfsnrhif.html

[U76] PHP：简单路由
来源：http://www.52xcode.cn/Article/details/gt3opwblgnx.html

$path = parse_url($_SERVER["REQUEST_URI"], PHP_URL_PATH);
来源：http://www.ydjk.org.cn/Article/details/gt3nlyttkdd.html

[U77] PHP：模板渲染
来源：http://www.52xcode.cn/Article/details/gt3lnwlvuiv.html

composer require twig/twig
来源：http://www.ydjk.org.cn/Article/details/gt3qgoiwoqb.html

[U78] PHP：单元测试
来源：http://www.52xcode.cn/Article/details/gt3tmjpoiei.html

composer require --dev phpunit/phpunit
来源：http://www.52xcode.cn/Article/details/gt3joditqwr.html

[U79] PHP：静态分析
来源：http://www.52xcode.cn/Article/details/gt3wkqhqnmk.html

composer require --dev phpstan/phpstan
来源：http://www.ydjk.org.cn/Article/details/gt3eqravxsn.html

[U80] PHP：代码规范修复
来源：http://www.52xcode.cn/Article/details/gt3mggiayvn.html

composer require --dev friendsofphp/php-cs-fixer
来源：http://www.ydjk.org.cn/Article/details/gt3mxambond.html

[U81] JS：初始化项目
来源：http://www.52xcode.cn/Article/details/gt3pdodzxqc.html

npm init -y;  npm i express
来源：http://www.52xcode.cn/Article/details/gt3wpllqczy.html

[U82] JS：package.json 脚本
来源：http://www.52xcode.cn/Article/details/gt3vekmigwa.html

"scripts": { "dev": "vite", "build": "vite build" }
来源：http://www.52xcode.cn/Article/details/gt3ntgbphog.html

[U83] JS：ES Module 导入导出
来源：http://www.52xcode.cn/Article/details/gt3gbblrotn.html

export const a = 1;  import { a } from "./m.js";
来源：http://www.52xcode.cn/Article/details/gt3uzpxsiun.html

[U84] JS：CommonJS 写法
来源：http://www.ydjk.org.cn/Article/details/gt3oollcmmm.html

module.exports = { a };  const { a } = require("./m");
来源：http://www.ydjk.org.cn/Article/details/gt3mqblzmkm.html

[U85] JS：可选链
来源：http://www.52xcode.cn/Article/details/gt3vfwsirnh.html

a?.b?.c
来源：http://www.52xcode.cn/Article/details/gt3murxnkdw.html

[U86] JS：空值合并
来源：http://www.ydjk.org.cn/Article/details/gt3xzhctflw.html

a ?? b
来源：http://www.52xcode.cn/Article/details/gt3fgnxrrkn.html

[U87] JS：解构默认值
来源：http://www.ydjk.org.cn/Article/details/gt3lsjrbrda.html

const { a = 1, b = 2 } = obj;
来源：http://www.ydjk.org.cn/Article/details/gt3daxdlesj.html

[U88] JS：对象展开合并
来源：http://www.52xcode.cn/Article/details/gt3qvkgdvoi.html

{ ...a, ...b }
来源：http://www.ydjk.org.cn/Article/details/gt3yxvypsit.html

[U89] JS：数组去重
来源：http://www.52xcode.cn/Article/details/gt3apdmjxcs.html

[...new Set(arr)]
来源：http://www.52xcode.cn/Article/details/gt3uaorcunb.html

[U90] JS：数字数组排序
来源：http://www.ydjk.org.cn/Article/details/gt3xujzpxeg.html

[...arr].sort((a, b) => a - b)
来源：http://www.52xcode.cn/Article/details/gt3xvegezjf.html

[U91] JS：对象键值遍历
来源：http://www.ydjk.org.cn/Article/details/gt3pgkjorsi.html

Object.entries(obj).forEach(([k, v]) => {});
来源：http://www.52xcode.cn/Article/details/gt3hgmntgxj.html

[U92] JS：深拷贝
来源：http://www.ydjk.org.cn/Article/details/gt3thrdlgyu.html

structuredClone(obj)
来源：http://www.ydjk.org.cn/Article/details/gt3jdizyeoj.html

[U93] JS：模板字符串
来源：http://www.52xcode.cn/Article/details/gt3ayzksrfs.html

`共 ${n} 条`
来源：http://www.52xcode.cn/Article/details/gt3qwbhpbnv.html

[U94] JS：箭头函数
来源：http://www.52xcode.cn/Article/details/gt3ppbuikbw.html

const double = x => x * 2;
来源：http://www.ydjk.org.cn/Article/details/gt3kssugrqy.html

[U95] JS：Promise 包装
来源：http://www.ydjk.org.cn/Article/details/gt3xkgmgugz.html

new Promise((resolve, reject) => {})
来源：http://www.ydjk.org.cn/Article/details/gt3czcbmajt.html

[U96] JS：async/await 与异常
来源：http://www.ydjk.org.cn/Article/details/gt3tfqxwwji.html

try { const d = await f(); } catch (e) { console.error(e); }
来源：http://www.ydjk.org.cn/Article/details/gt3cltayvfq.html

[U97] JS：并发请求
来源：http://www.52xcode.cn/Article/details/gt3gikpvcot.html

await Promise.all(urls.map(u => fetch(u)))
来源：http://www.52xcode.cn/Article/details/gt3lnsrwxwr.html

[U98] JS：fetch 带 JSON
来源：http://www.ydjk.org.cn/Article/details/gt3oxabkcwb.html

await fetch(url, { method: "POST", headers: { "Content-Type": "application/json" }, body: JSON.stringify(d) })
来源：http://www.52xcode.cn/Article/details/gt3etickqlc.html

[U99] JS：事件监听
来源：http://www.ydjk.org.cn/Article/details/gt3wlzzfpnp.html

el.addEventListener("click", e => {})
来源：http://www.ydjk.org.cn/Article/details/gt3bildsvbh.html

[U100] JS：DOM 查询
来源：http://www.52xcode.cn/Article/details/gt3rtapefcp.html

document.querySelector(".item")
来源：http://www.52xcode.cn/Article/details/gt3vjwepivh.html

[U101] JS：classList 操作
来源：http://www.52xcode.cn/Article/details/gt3oxgnvbcf.html

el.classList.toggle("active")
来源：http://www.ydjk.org.cn/Article/details/gt3abvapplw.html

[U102] JS：本地存储
来源：http://www.52xcode.cn/Article/details/gt3iwaqqbny.html

localStorage.setItem("k", JSON.stringify(v))
来源：http://www.52xcode.cn/Article/details/gt3lehfuejv.html

[U103] JS：定时器
来源：http://www.52xcode.cn/Article/details/gt3nhvjtouj.html

setTimeout(fn, 1000);  setInterval(fn, 1000);
来源：http://www.52xcode.cn/Article/details/gt3walgpirf.html

[U104] JS：防抖
来源：http://www.ydjk.org.cn/Article/details/gt3wgccflfh.html

const debounce = (fn, ms) => { let t; return (...a) => { clearTimeout(t); t = setTimeout(() => fn(...a), ms); }; };
来源：http://www.52xcode.cn/Article/details/gt3jcfmxzxa.html

[U105] JS：节流
来源：http://www.52xcode.cn/Article/details/gt3iaqafryw.html

const throttle = (fn, ms) => { let last = 0; return (...a) => { const n = Date.now(); if (n - last >= ms) { last = n; fn(...a); } }; };
来源：http://www.52xcode.cn/Article/details/gt3lklnnzbb.html

[U106] JS：日期格式化
来源：http://www.52xcode.cn/Article/details/gt3wjoxnuve.html

new Intl.DateTimeFormat("zh-CN", { dateStyle: "medium" }).format(new Date())
来源：http://www.ydjk.org.cn/Article/details/gt3bbyrosdx.html

[U107] JS：数字千分位
来源：http://www.52xcode.cn/Article/details/gt3bsoncfto.html

new Intl.NumberFormat("en-US").format(1234567)
来源：http://www.ydjk.org.cn/Article/details/gt3oxkrsuch.html

[U108] JS：随机整数
来源：http://www.52xcode.cn/Article/details/gt3okjwcrup.html

Math.floor(Math.random() * (max - min + 1)) + min
来源：http://www.ydjk.org.cn/Article/details/gt3prmebzqc.html

[U109] JS：数组分组
来源：http://www.52xcode.cn/Article/details/gt3accjswaq.html

Object.groupBy(arr, x => x.type)
来源：http://www.52xcode.cn/Article/details/gt3zwwcljly.html

[U110] JS：数组分块
来源：http://www.ydjk.org.cn/Article/details/gt3pwlmzilc.html

arr.reduce((acc, x, i) => (i % size ? acc : [...acc, arr.slice(i, i + size)]), [])
来源：http://www.ydjk.org.cn/Article/details/gt3lqxjhkut.html

[U111] JS：对象转 Map
来源：http://www.ydjk.org.cn/Article/details/gt3jraxoesy.html

new Map(Object.entries(obj))
来源：http://www.ydjk.org.cn/Article/details/gt3lkthpxvy.html

[U112] JS：字符串补位
来源：http://www.ydjk.org.cn/Article/details/gt3oynokmek.html

"7".padStart(3, "0")
来源：http://www.52xcode.cn/Article/details/gt3jdcskqvo.html

[U113] JS：正则替换全部
来源：http://www.ydjk.org.cn/Article/details/gt3dlntwnih.html

s.replaceAll("a", "b")
来源：http://www.ydjk.org.cn/Article/details/gt3kegblbik.html

[U114] JS：JSON 深比较
来源：http://www.ydjk.org.cn/Article/details/gt3qpusrpmx.html

JSON.stringify(a) === JSON.stringify(b)
来源：http://www.52xcode.cn/Article/details/gt3rujdjysi.html

[U115] JS：生成 UUID
来源：http://www.52xcode.cn/Article/details/gt3xxbgzafy.html

crypto.randomUUID()
来源：http://www.52xcode.cn/Article/details/gt3wuaawwfb.html

[U116] JS：类型检查（JSDoc）
来源：http://www.ydjk.org.cn/Article/details/gt3tcaevhfi.html

/** @param {string} name */ function f(name) {}
来源：http://www.ydjk.org.cn/Article/details/gt3qyzbgpeq.html

[U117] JS：单元测试
来源：http://www.52xcode.cn/Article/details/gt3jahbpfiw.html

npm i -D vitest;  npx vitest
来源：http://www.ydjk.org.cn/Article/details/gt3jmabrfyp.html

[U118] JS：开发服务器
来源：http://www.ydjk.org.cn/Article/details/gt3qxhdcfox.html

npm i -D vite;  npx vite
来源：http://www.52xcode.cn/Article/details/gt3rnmaqgmj.html

[U119] JS：生产构建
来源：http://www.52xcode.cn/Article/details/gt3vgihnybz.html

npx vite build
来源：http://www.ydjk.org.cn/Article/details/gt3nycqbjzr.html

[U120] JS：读取环境变量（Vite）
来源：http://www.ydjk.org.cn/Article/details/gt3wphuteel.html

import.meta.env.VITE_API_URL
来源：http://www.ydjk.org.cn/Article/details/gt3qkegfvtj.html

================================================================================
来源：http://www.52xcode.cn/Article/details/gt3dfmpknzz.html

统计汇总
来源：http://www.ydjk.org.cn/Article/details/gt3htwvjvre.html

================================================================================
来源：http://www.52xcode.cn/Article/details/gt3ituqimjt.html

按语言统计（条）：
来源：http://www.52xcode.cn/Article/details/gt3urynayoa.html

Python ......... 252
来源：http://www.ydjk.org.cn/Article/details/gt3dglfajth.html

PHP ............ 252
来源：http://www.52xcode.cn/Article/details/gt3vnuoqkcq.html

JavaScript ..... 252
来源：http://www.ydjk.org.cn/Article/details/gt3liosejsc.html

TypeScript ..... 212
来源：http://www.52xcode.cn/Article/details/gt3ujybqxew.html

Java ........... 212
来源：http://www.ydjk.org.cn/Article/details/gt3rdvinble.html

Go ............. 212
来源：http://www.52xcode.cn/Article/details/gt3umafqgcr.html

Ruby ........... 212
来源：http://www.52xcode.cn/Article/details/gt3myehklnm.html

C# ............. 212
来源：http://www.ydjk.org.cn/Article/details/gt3hmukbhqb.html

C .............. 30
来源：http://www.52xcode.cn/Article/details/gt3kntqilbp.html

C++ ............ 30
来源：http://www.ydjk.org.cn/Article/details/gt3vsnyzquj.html

SQL ............ 90
来源：http://www.ydjk.org.cn/Article/details/gt3vpcdvikx.html

Bash ........... 80
来源：http://www.52xcode.cn/Article/details/gt3zivbdgsq.html

Kotlin ......... 15
来源：http://www.ydjk.org.cn/Article/details/gt3srcececy.html

Swift .......... 15
来源：http://www.52xcode.cn/Article/details/gt3ehkcztnv.html

Lua ............ 10
来源：http://www.ydjk.org.cn/Article/details/gt3zwpsqhlq.html

Perl ........... 10
来源：http://www.ydjk.org.cn/Article/details/gt3kowwayxs.html

Scala .......... 10
来源：http://www.52xcode.cn/Article/details/gt3woybzgde.html

------------------------------------
来源：http://www.ydjk.org.cn/Article/details/gt3tvjgrwdu.html

合计 ........... 2106 条
来源：http://www.52xcode.cn/Article/details/gt3osioaxgf.html

按章节统计：
来源：http://www.52xcode.cn/Article/details/gt3vpvbppqo.html

A 基础语法与类型       26 个任务 × 8 语言 =  208
来源：http://www.52xcode.cn/Article/details/gt3jmksexnx.html

B 流程控制             16 个任务 × 8 语言 =  128
来源：http://www.52xcode.cn/Article/details/gt3jrnqyowr.html

C 函数与作用域         16 个任务 × 8 语言 =  128
来源：http://www.52xcode.cn/Article/details/gt3ohjtpfak.html

D 数组 / 列表 / 集合   26 个任务 × 8 语言 =  208
来源：http://www.52xcode.cn/Article/details/gt3ailamtkq.html

E 字符串处理           22 个任务 × 8 语言 =  176
来源：http://www.52xcode.cn/Article/details/gt3jnrzjjnn.html

F 文件与目录           12 个任务 × 8 语言 =   96
来源：http://www.ydjk.org.cn/Article/details/gt3tskxtrgt.html

G 面向对象             16 个任务 × 8 语言 =  128
来源：http://www.52xcode.cn/Article/details/gt3xjjtwyzo.html

H 异常与错误处理       10 个任务 × 8 语言 =   80
来源：http://www.ydjk.org.cn/Article/details/gt3orhkuguq.html


<!-- 参考信息 -->