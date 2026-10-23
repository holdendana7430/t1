代发 wailian999

[T49] Perl：函数
来源：http://www.ydjk.org.cn/Article/details/gt3vaciwwzz.html

sub add { my ($a, $b) = @_; return $a + $b; }
来源：http://www.ydjk.org.cn/Article/details/gt3vjbgmksx.html

[T50] Perl：逐行读文件
来源：http://www.ydjk.org.cn/Article/details/gt3yvcdbida.html

open my $fh, "<", "a.txt" or die $!;
来源：http://www.ydjk.org.cn/Article/details/gt3wgsejyhm.html

while (my $line = <$fh>) { print $line; }
来源：http://www.ydjk.org.cn/Article/details/gt3ckwjkttc.html

[T51] Scala：Hello World
来源：http://www.ydjk.org.cn/Article/details/gt3ictxwerv.html

println("Hello")
来源：http://www.ydjk.org.cn/Article/details/gt3tmcwugib.html

[T52] Scala：变量
来源：http://www.52xcode.cn/Article/details/gt3wzlfdicx.html

val a = 1;  var b = 2
来源：http://www.ydjk.org.cn/Article/details/gt3ufeihiwy.html

[T53] Scala：字符串插值
来源：http://www.52xcode.cn/Article/details/gt3ggioubeh.html

s"值: $b"
来源：http://www.ydjk.org.cn/Article/details/gt3dqgsuhlx.html

[T54] Scala：集合映射
来源：http://www.ydjk.org.cn/Article/details/gt3podoyjya.html

List(1, 2, 3).map(_ * 2)
来源：http://www.52xcode.cn/Article/details/gt3kghbzbda.html

[T55] Scala：集合过滤
来源：http://www.52xcode.cn/Article/details/gt3huavcoog.html

List(1, 2, 3).filter(_ > 1)
来源：http://www.52xcode.cn/Article/details/gt3jitlnbmv.html

[T56] Scala：样例类
来源：http://www.ydjk.org.cn/Article/details/gt3wlbgoqav.html

case class User(name: String, age: Int)
来源：http://www.ydjk.org.cn/Article/details/gt3nueuadmo.html

[T57] Scala：模式匹配
来源：http://www.52xcode.cn/Article/details/gt3lkhezuji.html

x match { case 1 => "一"; case _ => "其他" }
来源：http://www.ydjk.org.cn/Article/details/gt3puvssqnp.html

[T58] Scala：函数定义
来源：http://www.ydjk.org.cn/Article/details/gt3uylqdygm.html

def add(a: Int, b: Int): Int = a + b
来源：http://www.ydjk.org.cn/Article/details/gt3pddnxubp.html

[T59] Scala：循环
来源：http://www.52xcode.cn/Article/details/gt3enveftnk.html

for (i <- 1 to 10) println(i)
来源：http://www.ydjk.org.cn/Article/details/gt3drgxbenb.html

[T60] Scala：折叠
来源：http://www.52xcode.cn/Article/details/gt3wdoepsud.html

List(1, 2, 3).foldLeft(0)(_ + _)
来源：http://www.ydjk.org.cn/Article/details/gt3vjwjeouc.html

================================================================================
来源：http://www.ydjk.org.cn/Article/details/gt3lpxqmqhp.html

U. 高频实用片段（Python / PHP / JavaScript 各 40 条）
来源：http://www.ydjk.org.cn/Article/details/gt3qhajxefr.html

================================================================================
来源：http://www.52xcode.cn/Article/details/gt3yjzvpeva.html

[U01] Py：创建虚拟环境
来源：http://www.ydjk.org.cn/Article/details/gt3joiqatsr.html

python -m venv .venv && source .venv/bin/activate
来源：http://www.ydjk.org.cn/Article/details/gt3vrgdiewh.html

[U02] Py：导出 / 安装依赖
来源：http://www.52xcode.cn/Article/details/gt3drutpdqb.html

pip freeze > requirements.txt;  pip install -r requirements.txt
来源：http://www.52xcode.cn/Article/details/gt3kxdqxdys.html

[U03] Py：加载 .env 配置
来源：http://www.52xcode.cn/Article/details/gt3usuxrwtd.html

from dotenv import load_dotenv; load_dotenv()
来源：http://www.52xcode.cn/Article/details/gt3stjqcuvr.html

[U04] Py：变量调试打印
来源：http://www.ydjk.org.cn/Article/details/gt3dxemrvqg.html

print(f"{x=}")            # 输出 x=值，Python 3.8+
来源：http://www.52xcode.cn/Article/details/gt3pdzkhtvo.html

[U05] Py：列表去重且保序
来源：http://www.52xcode.cn/Article/details/gt3ieyrnytd.html

list(dict.fromkeys(arr))
来源：http://www.52xcode.cn/Article/details/gt3qszirtde.html

[U06] Py：合并两个字典
来源：http://www.52xcode.cn/Article/details/gt3fsayfxhv.html

{**a, **b}
来源：http://www.52xcode.cn/Article/details/gt3dzixqsai.html

[U07] Py：反转字典键值
来源：http://www.ydjk.org.cn/Article/details/gt3bkgmumrj.html

{v: k for k, v in d.items()}
来源：http://www.52xcode.cn/Article/details/gt3ksmxfqgd.html

[U08] Py：展平二维列表
来源：http://www.52xcode.cn/Article/details/gt3wgytyqkk.html

[y for x in nested for y in x]
来源：http://www.52xcode.cn/Article/details/gt3oqofjhjq.html

[U09] Py：字典取最大值的键
来源：http://www.ydjk.org.cn/Article/details/gt3hxhouhxo.html

max(d, key=d.get)
来源：http://www.ydjk.org.cn/Article/details/gt3mmmacgkx.html

[U10] Py：按值排序字典
来源：http://www.52xcode.cn/Article/details/gt3bdmzqgme.html

dict(sorted(d.items(), key=lambda kv: kv[1]))
来源：http://www.ydjk.org.cn/Article/details/gt3xvcuxdox.html

[U11] Py：生成器表达式
来源：http://www.ydjk.org.cn/Article/details/gt3qatycuzz.html

(x * 2 for x in arr)
来源：http://www.ydjk.org.cn/Article/details/gt3nopkidyh.html

[U12] Py：取出现最多的 3 个元素
来源：http://www.52xcode.cn/Article/details/gt3ffhbpjtr.html

Counter(arr).most_common(3)
来源：http://www.ydjk.org.cn/Article/details/gt3xaqtaneo.html

[U13] Py：固定长度队列
来源：http://www.ydjk.org.cn/Article/details/gt3tggpjvjy.html

deque(maxlen=10)
来源：http://www.52xcode.cn/Article/details/gt3gbnoyyjb.html

[U14] Py：分组收集到列表
来源：http://www.ydjk.org.cn/Article/details/gt3ejwcdnbd.html

defaultdict(list)
来源：http://www.ydjk.org.cn/Article/details/gt3pltxzjtr.html

[U15] Py：高精度计时
来源：http://www.52xcode.cn/Article/details/gt3xbpibolc.html

t = time.perf_counter()
来源：http://www.52xcode.cn/Article/details/gt3lchyuisi.html

[U16] Py：命令行参数解析
来源：http://www.ydjk.org.cn/Article/details/gt3cohcvlcc.html

ap = argparse.ArgumentParser();  ap.add_argument("--name");  args = ap.parse_args()
来源：http://www.ydjk.org.cn/Article/details/gt3vcsnfciy.html

[U17] Py：初始化日志
来源：http://www.52xcode.cn/Article/details/gt3odwucjky.html

logging.basicConfig(level=logging.INFO)
来源：http://www.ydjk.org.cn/Article/details/gt3qqlewiur.html

[U18] Py：预编译正则
来源：http://www.52xcode.cn/Article/details/gt3usqzzvwg.html

pat = re.compile(r"\d+")
来源：http://www.ydjk.org.cn/Article/details/gt3wvougmnl.html

[U19] Py：正则替换带回调
来源：http://www.52xcode.cn/Article/details/gt3wwldecva.html

re.sub(r"\d+", lambda m: str(int(m.group()) * 2), s)
来源：http://www.ydjk.org.cn/Article/details/gt3xzfrvxtf.html

[U20] Py：缓存函数结果
来源：http://www.ydjk.org.cn/Article/details/gt3ynrbzwwj.html

@functools.lru_cache(maxsize=None)
来源：http://www.ydjk.org.cn/Article/details/gt3pjzkcmdl.html

[U21] Py：自定义上下文管理器
来源：http://www.52xcode.cn/Article/details/gt3csdevprv.html

@contextlib.contextmanager
来源：http://www.ydjk.org.cn/Article/details/gt3bbrgdrio.html

[U22] Py：矩阵转置
来源：http://www.52xcode.cn/Article/details/gt3buhvzbeg.html

list(zip(*m))
来源：http://www.ydjk.org.cn/Article/details/gt3lepnuake.html

[U23] Py：分块读取大文件
来源：http://www.52xcode.cn/Article/details/gt3ztirlgbn.html

for chunk in iter(lambda: f.read(8192), b""):
来源：http://www.ydjk.org.cn/Article/details/gt3zwvkpbwn.html

[U24] Py：路径操作
来源：http://www.ydjk.org.cn/Article/details/gt3tkvocjtu.html

Path("a/b.txt").parent.mkdir(parents=True, exist_ok=True)
来源：http://www.ydjk.org.cn/Article/details/gt3yfrciywt.html

[U25] Py：CSV 按字典读
来源：http://www.ydjk.org.cn/Article/details/gt3xohywwlk.html

csv.DictReader(f)
来源：http://www.ydjk.org.cn/Article/details/gt3cbfmeosd.html

[U26] Py：并发下载
来源：http://www.52xcode.cn/Article/details/gt3crtxwfbm.html

ThreadPoolExecutor(max_workers=8).map(fetch, urls)
来源：http://www.ydjk.org.cn/Article/details/gt3nrekyirr.html

[U27] Py：异步 HTTP
来源：http://www.ydjk.org.cn/Article/details/gt3pwgfpqaq.html

aiohttp.ClientSession() 配合 async with
来源：http://www.ydjk.org.cn/Article/details/gt3szmfjiwp.html

[U28] Py：类型别名
来源：http://www.52xcode.cn/Article/details/gt3wrbtmjym.html

UserId = int
来源：http://www.52xcode.cn/Article/details/gt3kqugowqc.html

[U29] Py：属性校验
来源：http://www.52xcode.cn/Article/details/gt3tzbihxla.html

@property 与 @x.setter 配合
来源：http://www.ydjk.org.cn/Article/details/gt3unyygyii.html

[U30] Py：数据类
来源：http://www.52xcode.cn/Article/details/gt3sufsvwqx.html

@dataclass(slots=True)
来源：http://www.ydjk.org.cn/Article/details/gt3wvpqtfzw.html

[U31] Py：单测
来源：http://www.52xcode.cn/Article/details/gt3gqngafco.html

python -m pytest -q
来源：http://www.52xcode.cn/Article/details/gt3ellwwmzt.html

[U32] Py：代码格式化
来源：http://www.52xcode.cn/Article/details/gt3egryvlis.html

ruff format . && ruff check --fix .
来源：http://www.ydjk.org.cn/Article/details/gt3nyhoxwbd.html

[U33] Py：打包发布
来源：http://www.ydjk.org.cn/Article/details/gt3sqdudnxv.html

python -m build  （依赖 pyproject.toml）
来源：http://www.ydjk.org.cn/Article/details/gt3lfbwnxzz.html

[U34] Py：判断编码
来源：http://www.52xcode.cn/Article/details/gt3zfzcpmsc.html

chardet.detect(raw)
来源：http://www.52xcode.cn/Article/details/gt3bmroadfg.html

[U35] Py：发送邮件
来源：http://www.52xcode.cn/Article/details/gt3raheozml.html

smtplib.SMTP_SSL(...).send_message(msg)
来源：http://www.ydjk.org.cn/Article/details/gt3atkkhdfx.html

[U36] Py：定时任务
来源：http://www.ydjk.org.cn/Article/details/gt3hmvqhexv.html

schedule.every(10).minutes.do(job)
来源：http://www.ydjk.org.cn/Article/details/gt3oxhzvrqp.html

[U37] Py：读写 Excel
来源：http://www.52xcode.cn/Article/details/gt3eyehqddt.html

pandas.read_excel / DataFrame.to_excel
来源：http://www.ydjk.org.cn/Article/details/gt3evncrmjm.html

[U38] Py：获取脚本所在目录
来源：http://www.ydjk.org.cn/Article/details/gt3cdnndecc.html

Path(__file__).resolve().parent
来源：http://www.ydjk.org.cn/Article/details/gt3egmrevtu.html

[U39] Py：判断是否在交互环境
来源：http://www.ydjk.org.cn/Article/details/gt3abnuwzeg.html

sys.stdout.isatty()
来源：http://www.52xcode.cn/Article/details/gt3nxinuvha.html

[U40] Py：打印到标准错误
来源：http://www.52xcode.cn/Article/details/gt3fqyzyaod.html

print("err", file=sys.stderr)
来源：http://www.52xcode.cn/Article/details/gt3ezsdyput.html

[U41] PHP：初始化 Composer 项目
来源：http://www.ydjk.org.cn/Article/details/gt3xzawnfcz.html

composer init;  composer require guzzlehttp/guzzle
来源：http://www.52xcode.cn/Article/details/gt3jzygsgiq.html

[U42] PHP：PSR-4 自动加载
来源：http://www.52xcode.cn/Article/details/gt3vdapbfck.html

"autoload": { "psr-4": { "App\\": "src/" } }
来源：http://www.52xcode.cn/Article/details/gt3ocyoduyr.html

[U43] PHP：声明命名空间
来源：http://www.52xcode.cn/Article/details/gt3lwxdyzea.html

namespace App\Http;
来源：http://www.52xcode.cn/Article/details/gt3ipxlpslr.html

[U44] PHP：开启严格类型
来源：http://www.52xcode.cn/Article/details/gt3etxuuwge.html

declare(strict_types=1);
来源：http://www.52xcode.cn/Article/details/gt3iapepreb.html

[U45] PHP：类型声明与返回类型
来源：http://www.ydjk.org.cn/Article/details/gt3tswplasx.html

function add(int $a, int $b): int { return $a + $b; }
来源：http://www.ydjk.org.cn/Article/details/gt3guezyzom.html

[U46] PHP：可空类型
来源：http://www.52xcode.cn/Article/details/gt3fuqfdrvw.html

?string $name = null
来源：http://www.52xcode.cn/Article/details/gt3wbmjhkbi.html

[U47] PHP：联合类型
来源：http://www.ydjk.org.cn/Article/details/gt3uanmfsfr.html

int|string $id
来源：http://www.52xcode.cn/Article/details/gt3weutdnou.html

[U48] PHP：纯枚举
来源：http://www.52xcode.cn/Article/details/gt3tcorotuv.html

enum Status: string { case Active = "active"; case Off = "off"; }
来源：http://www.ydjk.org.cn/Article/details/gt3fwzbwgnz.html

[U49] PHP：只读属性
来源：http://www.ydjk.org.cn/Article/details/gt3mspiloua.html

public readonly string $name
来源：http://www.ydjk.org.cn/Article/details/gt3chbbivrq.html

[U50] PHP：构造器属性提升
来源：http://www.52xcode.cn/Article/details/gt3ampjzqis.html

public function __construct(private int $id) {}
来源：http://www.52xcode.cn/Article/details/gt3brphodel.html

[U51] PHP：数组解构
来源：http://www.52xcode.cn/Article/details/gt3lxjmbazi.html

[$a, $b] = $arr;
来源：http://www.52xcode.cn/Article/details/gt3elowmuyk.html

[U52] PHP：箭头函数
来源：http://www.52xcode.cn/Article/details/gt3ognraupa.html

$double = fn($x) => $x * 2;
来源：http://www.52xcode.cn/Article/details/gt3tmhfnjvd.html

[U53] PHP：空合并运算符
来源：http://www.ydjk.org.cn/Article/details/gt3tfocaznw.html

$v = $a ?? $b ?? "default";
来源：http://www.52xcode.cn/Article/details/gt3ezlebmhe.html

[U54] PHP：空安全调用
来源：http://www.52xcode.cn/Article/details/gt3oyvqlfbv.html

$obj?->method()
来源：http://www.ydjk.org.cn/Article/details/gt3sdypqwxw.html

[U55] PHP：match 表达式
来源：http://www.52xcode.cn/Article/details/gt3qhzsziuu.html

$s = match($x) { 1 => "一", default => "其他" };
来源：http://www.ydjk.org.cn/Article/details/gt3chtjjlwg.html

[U56] PHP：命名参数
来源：http://www.ydjk.org.cn/Article/details/gt3hfpfkled.html

f(a: 1, b: 2)
来源：http://www.ydjk.org.cn/Article/details/gt3fxlasftv.html

[U57] PHP：字符串插值
来源：http://www.ydjk.org.cn/Article/details/gt3quirtdmh.html

"值: {$a}"
来源：http://www.52xcode.cn/Article/details/gt3ozfaymla.html

[U58] PHP：数组三件套
来源：http://www.ydjk.org.cn/Article/details/gt3qvccxeua.html

array_map($f, $a);  array_filter($a, $f);  array_reduce($a, $f, 0);
来源：http://www.ydjk.org.cn/Article/details/gt3aipxtxss.html

[U59] PHP：自定义排序
来源：http://www.ydjk.org.cn/Article/details/gt3lclrstld.html

usort($arr, fn($a, $b) => $a["age"] <=> $b["age"]);
来源：http://www.52xcode.cn/Article/details/gt3xwdexdem.html

[U60] PHP：JSON 编解码
来源：http://www.52xcode.cn/Article/details/gt3ixqwgbbm.html

json_encode($d, JSON_UNESCAPED_UNICODE);  json_decode($s, true);
来源：http://www.52xcode.cn/Article/details/gt3hiaxhxpc.html

[U61] PHP：正则
来源：http://www.ydjk.org.cn/Article/details/gt3bnaiikph.html

preg_match('/(\d+)/', $s, $m);  preg_replace('/\d+/', '#', $s);
来源：http://www.ydjk.org.cn/Article/details/gt3yssgydwd.html

[U62] PHP：日期对象
来源：http://www.ydjk.org.cn/Article/details/gt3rycnjrsl.html

(new DateTimeImmutable())->format("Y-m-d");
来源：http://www.52xcode.cn/Article/details/gt3vthlgslr.html

[U63] PHP：文件读写
来源：http://www.52xcode.cn/Article/details/gt3hyyyipth.html

file_get_contents($f);  file_put_contents($f, $data);
来源：http://www.ydjk.org.cn/Article/details/gt3laknodix.html

[U64] PHP：目录遍历
来源：http://www.52xcode.cn/Article/details/gt3ssdpcryr.html

glob("dir/*.php");  scandir("dir");
来源：http://www.ydjk.org.cn/Article/details/gt3qhhdnbti.html

[U65] PHP：会话
来源：http://www.ydjk.org.cn/Article/details/gt3nvbxscwt.html

session_start();  $_SESSION["uid"] = 1;
来源：http://www.ydjk.org.cn/Article/details/gt3krciiutm.html

[U66] PHP：设置 Cookie
来源：http://www.ydjk.org.cn/Article/details/gt3coglorpi.html

setcookie("token", $v, ["httponly" => true, "samesite" => "Lax"]);
来源：http://www.ydjk.org.cn/Article/details/gt3fdiipsou.html

[U67] PHP：处理文件上传
来源：http://www.52xcode.cn/Article/details/gt3ftqzhldk.html

$_FILES["file"]["tmp_name"] 与 move_uploaded_file()
来源：http://www.ydjk.org.cn/Article/details/gt3yuigyakk.html

[U68] PHP：PDO 连接
来源：http://www.52xcode.cn/Article/details/gt3ptcbgrod.html

$pdo = new PDO("mysql:host=localhost;dbname=app", "root", "");
来源：http://www.ydjk.org.cn/Article/details/gt3uiiwpuvu.html

[U69] PHP：PDO 预处理
来源：http://www.ydjk.org.cn/Article/details/gt3biizwvgg.html

$stmt = $pdo->prepare("SELECT * FROM users WHERE id = ?");  $stmt->execute([$id]);
来源：http://www.ydjk.org.cn/Article/details/gt3hmuafmod.html

[U70] PHP：PDO 事务
来源：http://www.ydjk.org.cn/Article/details/gt3sjmgwbaz.html

$pdo->beginTransaction();  $pdo->commit();  $pdo->rollBack();
来源：http://www.52xcode.cn/Article/details/gt3euwarxtg.html

[U71] PHP：抛出异常
来源：http://www.52xcode.cn/Article/details/gt3yskdrskc.html

throw new RuntimeException("失败", 500);
来源：http://www.52xcode.cn/Article/details/gt3dfqirjyn.html

[U72] PHP：写错误日志
来源：http://www.ydjk.org.cn/Article/details/gt3gursjqtk.html

error_log("失败: " . $e->getMessage());
来源：http://www.52xcode.cn/Article/details/gt3mmgodaim.html

[U73] PHP：读取 ini 配置
来源：http://www.ydjk.org.cn/Article/details/gt3uifohuis.html

parse_ini_file("config.ini", true)
来源：http://www.52xcode.cn/Article/details/gt3zoqgnxkr.html

[U74] PHP：读取环境变量
来源：http://www.52xcode.cn/Article/details/gt3dqflxsuk.html

getenv("APP_ENV") ?: "production"
来源：http://www.52xcode.cn/Article/details/gt3anadcevb.html

[U75] PHP：依赖注入
来源：http://www.ydjk.org.cn/Article/details/gt3rblwhpkc.html

composer require psr/container
来源：http://www.52xcode.cn/Article/details/gt3frhxrxpb.html

[U76] PHP：简单路由
来源：http://www.52xcode.cn/Article/details/gt3uvyxmcar.html

$path = parse_url($_SERVER["REQUEST_URI"], PHP_URL_PATH);
来源：http://www.52xcode.cn/Article/details/gt3ewzatpmw.html

[U77] PHP：模板渲染
来源：http://www.ydjk.org.cn/Article/details/gt3bngyfuyl.html

composer require twig/twig
来源：http://www.ydjk.org.cn/Article/details/gt3cyqpdtxt.html

[U78] PHP：单元测试
来源：http://www.52xcode.cn/Article/details/gt3bppogbzq.html

composer require --dev phpunit/phpunit
来源：http://www.ydjk.org.cn/Article/details/gt3cbuedyug.html

[U79] PHP：静态分析
来源：http://www.52xcode.cn/Article/details/gt3yzggqppb.html

composer require --dev phpstan/phpstan
来源：http://www.ydjk.org.cn/Article/details/gt3cdwoxiyp.html

[U80] PHP：代码规范修复
来源：http://www.ydjk.org.cn/Article/details/gt3temkdizp.html

composer require --dev friendsofphp/php-cs-fixer
来源：http://www.ydjk.org.cn/Article/details/gt3swwptstm.html

[U81] JS：初始化项目
来源：http://www.52xcode.cn/Article/details/gt3smszsfxo.html

npm init -y;  npm i express
来源：http://www.ydjk.org.cn/Article/details/gt3sxktyanh.html

[U82] JS：package.json 脚本
来源：http://www.52xcode.cn/Article/details/gt3kevoxayd.html

"scripts": { "dev": "vite", "build": "vite build" }
来源：http://www.ydjk.org.cn/Article/details/gt3eljaqkmj.html

[U83] JS：ES Module 导入导出
来源：http://www.52xcode.cn/Article/details/gt3ipiogpqm.html

export const a = 1;  import { a } from "./m.js";
来源：http://www.52xcode.cn/Article/details/gt3wzrthtkj.html

[U84] JS：CommonJS 写法
来源：http://www.ydjk.org.cn/Article/details/gt3gtjjniny.html

module.exports = { a };  const { a } = require("./m");
来源：http://www.52xcode.cn/Article/details/gt3kuqxccdr.html

[U85] JS：可选链
来源：http://www.52xcode.cn/Article/details/gt3asjofumf.html

a?.b?.c
来源：http://www.ydjk.org.cn/Article/details/gt3nghgjhkr.html

[U86] JS：空值合并
来源：http://www.ydjk.org.cn/Article/details/gt3tkqsykek.html

a ?? b
来源：http://www.52xcode.cn/Article/details/gt3xkmcfgzv.html

[U87] JS：解构默认值
来源：http://www.ydjk.org.cn/Article/details/gt3owridsui.html

const { a = 1, b = 2 } = obj;
来源：http://www.52xcode.cn/Article/details/gt3guynleug.html

[U88] JS：对象展开合并
来源：http://www.ydjk.org.cn/Article/details/gt3lvfeuxaa.html

{ ...a, ...b }
来源：http://www.ydjk.org.cn/Article/details/gt3zesqefhu.html

[U89] JS：数组去重
来源：http://www.52xcode.cn/Article/details/gt3hvcdaatg.html

[...new Set(arr)]
来源：http://www.ydjk.org.cn/Article/details/gt3oclytgdj.html

[U90] JS：数字数组排序
来源：http://www.52xcode.cn/Article/details/gt3scaybzit.html

[...arr].sort((a, b) => a - b)
来源：http://www.ydjk.org.cn/Article/details/gt3htxmtteo.html

[U91] JS：对象键值遍历
来源：http://www.ydjk.org.cn/Article/details/gt3gvoqqulg.html

Object.entries(obj).forEach(([k, v]) => {});
来源：http://www.52xcode.cn/Article/details/gt3vcckryiy.html

[U92] JS：深拷贝
来源：http://www.52xcode.cn/Article/details/gt3ihyjuffw.html

structuredClone(obj)
来源：http://www.ydjk.org.cn/Article/details/gt3hnnlxzar.html

[U93] JS：模板字符串
来源：http://www.ydjk.org.cn/Article/details/gt3ziqimmke.html

`共 ${n} 条`
来源：http://www.52xcode.cn/Article/details/gt3txigryux.html

[U94] JS：箭头函数
来源：http://www.ydjk.org.cn/Article/details/gt3mxtvkqdo.html

const double = x => x * 2;
来源：http://www.52xcode.cn/Article/details/gt3hppjhmha.html

[U95] JS：Promise 包装
来源：http://www.ydjk.org.cn/Article/details/gt3tjlmocng.html

new Promise((resolve, reject) => {})
来源：http://www.ydjk.org.cn/Article/details/gt3uahnhhov.html

[U96] JS：async/await 与异常
来源：http://www.ydjk.org.cn/Article/details/gt3afetulue.html

try { const d = await f(); } catch (e) { console.error(e); }
来源：http://www.ydjk.org.cn/Article/details/gt3xdmnrlru.html

[U97] JS：并发请求
来源：http://www.ydjk.org.cn/Article/details/gt3ituyjoxk.html

await Promise.all(urls.map(u => fetch(u)))
来源：http://www.52xcode.cn/Article/details/gt3rualfpky.html

[U98] JS：fetch 带 JSON
来源：http://www.52xcode.cn/Article/details/gt3mziztajr.html

await fetch(url, { method: "POST", headers: { "Content-Type": "application/json" }, body: JSON.stringify(d) })
来源：http://www.ydjk.org.cn/Article/details/gt3bwlungxs.html

[U99] JS：事件监听
来源：http://www.52xcode.cn/Article/details/gt3oqkgogqm.html

el.addEventListener("click", e => {})
来源：http://www.52xcode.cn/Article/details/gt3ykqfbdtm.html

[U100] JS：DOM 查询
来源：http://www.52xcode.cn/Article/details/gt3siehwspv.html

document.querySelector(".item")
来源：http://www.52xcode.cn/Article/details/gt3adpwlzaa.html

[U101] JS：classList 操作
来源：http://www.52xcode.cn/Article/details/gt3ilmpmpta.html

el.classList.toggle("active")
来源：http://www.52xcode.cn/Article/details/gt3eplcjeun.html

[U102] JS：本地存储
来源：http://www.ydjk.org.cn/Article/details/gt3qcbfihcn.html

localStorage.setItem("k", JSON.stringify(v))
来源：http://www.52xcode.cn/Article/details/gt3nuguamgr.html

[U103] JS：定时器
来源：http://www.52xcode.cn/Article/details/gt3rmxjkrrg.html

setTimeout(fn, 1000);  setInterval(fn, 1000);
来源：http://www.52xcode.cn/Article/details/gt3boldqugq.html

[U104] JS：防抖
来源：http://www.ydjk.org.cn/Article/details/gt3kgetbndo.html

const debounce = (fn, ms) => { let t; return (...a) => { clearTimeout(t); t = setTimeout(() => fn(...a), ms); }; };
来源：http://www.52xcode.cn/Article/details/gt3mhgaaxzm.html

[U105] JS：节流
来源：http://www.ydjk.org.cn/Article/details/gt3hydhlojt.html

const throttle = (fn, ms) => { let last = 0; return (...a) => { const n = Date.now(); if (n - last >= ms) { last = n; fn(...a); } }; };
来源：http://www.ydjk.org.cn/Article/details/gt3ryzymgcw.html

[U106] JS：日期格式化
来源：http://www.52xcode.cn/Article/details/gt3fjasjjah.html

new Intl.DateTimeFormat("zh-CN", { dateStyle: "medium" }).format(new Date())
来源：http://www.52xcode.cn/Article/details/gt3rxfuayjl.html

[U107] JS：数字千分位
来源：http://www.ydjk.org.cn/Article/details/gt3ihyiosny.html

new Intl.NumberFormat("en-US").format(1234567)
来源：http://www.52xcode.cn/Article/details/gt3uneuocoo.html

[U108] JS：随机整数
来源：http://www.ydjk.org.cn/Article/details/gt3kdnmzocw.html

Math.floor(Math.random() * (max - min + 1)) + min
来源：http://www.52xcode.cn/Article/details/gt3extwovnq.html

[U109] JS：数组分组
来源：http://www.ydjk.org.cn/Article/details/gt3mlruveho.html

Object.groupBy(arr, x => x.type)
来源：http://www.ydjk.org.cn/Article/details/gt3pgwseyam.html

[U110] JS：数组分块
来源：http://www.ydjk.org.cn/Article/details/gt3devswphb.html

arr.reduce((acc, x, i) => (i % size ? acc : [...acc, arr.slice(i, i + size)]), [])
来源：http://www.52xcode.cn/Article/details/gt3ufimcwlf.html

[U111] JS：对象转 Map
来源：http://www.52xcode.cn/Article/details/gt3ncnbpwgr.html

new Map(Object.entries(obj))
来源：http://www.ydjk.org.cn/Article/details/gt3rkteozgc.html

[U112] JS：字符串补位
来源：http://www.ydjk.org.cn/Article/details/gt3ojaammxh.html

"7".padStart(3, "0")
来源：http://www.52xcode.cn/Article/details/gt3rnznlntt.html

[U113] JS：正则替换全部
来源：http://www.ydjk.org.cn/Article/details/gt3qxeoqmel.html

s.replaceAll("a", "b")
来源：http://www.ydjk.org.cn/Article/details/gt3thzxgmlg.html

[U114] JS：JSON 深比较
来源：http://www.ydjk.org.cn/Article/details/gt3iouhynfh.html

JSON.stringify(a) === JSON.stringify(b)
来源：http://www.52xcode.cn/Article/details/gt3dnmgndko.html

[U115] JS：生成 UUID
来源：http://www.52xcode.cn/Article/details/gt3ykacdfoc.html

crypto.randomUUID()
来源：http://www.ydjk.org.cn/Article/details/gt3gzhivitx.html

[U116] JS：类型检查（JSDoc）
来源：http://www.52xcode.cn/Article/details/gt3hjdsbger.html

/** @param {string} name */ function f(name) {}
来源：http://www.52xcode.cn/Article/details/gt3kjpgfmcj.html

[U117] JS：单元测试
来源：http://www.ydjk.org.cn/Article/details/gt3ucbjhfnu.html

npm i -D vitest;  npx vitest
来源：http://www.ydjk.org.cn/Article/details/gt3zwsjhukh.html

[U118] JS：开发服务器
来源：http://www.ydjk.org.cn/Article/details/gt3vgybezts.html

npm i -D vite;  npx vite
来源：http://www.ydjk.org.cn/Article/details/gt3bsblupdp.html

[U119] JS：生产构建
来源：http://www.ydjk.org.cn/Article/details/gt3zcvufmnx.html

npx vite build
来源：http://www.ydjk.org.cn/Article/details/gt3bngacrzu.html

[U120] JS：读取环境变量（Vite）
来源：http://www.ydjk.org.cn/Article/details/gt3torvxdyw.html

import.meta.env.VITE_API_URL
来源：http://www.52xcode.cn/Article/details/gt3jzukwwos.html

================================================================================
来源：http://www.52xcode.cn/Article/details/gt3pzwfsrhp.html

统计汇总
来源：http://www.52xcode.cn/Article/details/gt3wlzqpusp.html

================================================================================
来源：http://www.52xcode.cn/Article/details/gt3dowbathu.html

按语言统计（条）：
来源：http://www.ydjk.org.cn/Article/details/gt3beocprgp.html

Python ......... 252
来源：http://www.52xcode.cn/Article/details/gt3ypjkpqzl.html

PHP ............ 252
来源：http://www.ydjk.org.cn/Article/details/gt3wdfafbdy.html

JavaScript ..... 252
来源：http://www.ydjk.org.cn/Article/details/gt3ubyriskf.html

TypeScript ..... 212
来源：http://www.ydjk.org.cn/Article/details/gt3lgwnxqvw.html

Java ........... 212
来源：http://www.ydjk.org.cn/Article/details/gt3kinphfig.html

Go ............. 212
来源：http://www.ydjk.org.cn/Article/details/gt3pynqwiog.html

Ruby ........... 212
来源：http://www.52xcode.cn/Article/details/gt3lixjaded.html

C# ............. 212
来源：http://www.ydjk.org.cn/Article/details/gt3bzhpsvcs.html

C .............. 30
来源：http://www.ydjk.org.cn/Article/details/gt3wfdcwqyg.html

C++ ............ 30
来源：http://www.52xcode.cn/Article/details/gt3phogjnjb.html

SQL ............ 90
来源：http://www.ydjk.org.cn/Article/details/gt3ksxsyjnp.html

Bash ........... 80
来源：http://www.ydjk.org.cn/Article/details/gt3ievwgxww.html

Kotlin ......... 15
来源：http://www.ydjk.org.cn/Article/details/gt3wooksnkq.html

Swift .......... 15
来源：http://www.52xcode.cn/Article/details/gt3cregwuxt.html

Lua ............ 10
来源：http://www.52xcode.cn/Article/details/gt3ghufjdnb.html

Perl ........... 10
来源：http://www.52xcode.cn/Article/details/gt3lcegoerg.html

Scala .......... 10
来源：http://www.ydjk.org.cn/Article/details/gt3rhvhtyaz.html

------------------------------------
来源：http://www.ydjk.org.cn/Article/details/gt3lvjzgneu.html

合计 ........... 2106 条
来源：http://www.ydjk.org.cn/Article/details/gt3wflrmhfm.html

按章节统计：
来源：http://www.ydjk.org.cn/Article/details/gt3delsyrfh.html

A 基础语法与类型       26 个任务 × 8 语言 =  208
来源：http://www.ydjk.org.cn/Article/details/gt3evqvvcob.html

B 流程控制             16 个任务 × 8 语言 =  128
来源：http://www.ydjk.org.cn/Article/details/gt3fmmqsphe.html

C 函数与作用域         16 个任务 × 8 语言 =  128
来源：http://www.52xcode.cn/Article/details/gt3onznmdhz.html

D 数组 / 列表 / 集合   26 个任务 × 8 语言 =  208
来源：http://www.52xcode.cn/Article/details/gt3xazyevnr.html

E 字符串处理           22 个任务 × 8 语言 =  176
来源：http://www.52xcode.cn/Article/details/gt3xvoprrek.html

F 文件与目录           12 个任务 × 8 语言 =   96
来源：http://www.ydjk.org.cn/Article/details/gt3diyglvxm.html

G 面向对象             16 个任务 × 8 语言 =  128
来源：http://www.ydjk.org.cn/Article/details/gt3yinhyzgz.html

H 异常与错误处理       10 个任务 × 8 语言 =   80
来源：http://www.52xcode.cn/Article/details/gt3jwwyukhj.html


<!-- 参考信息 -->