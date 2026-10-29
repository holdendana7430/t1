代发 wailian999

while (my $line = <$fh>) { print $line; }
来源：http://www.blog.fehbvm.com/Article/details/gmfoyacja.sHtML

[T51] Scala：Hello World
来源：http://www.share.zdbjq.cn/Article/details/gwnlvfheq.sHtML

println("Hello")
来源：http://mobile.fehbvm.com/Article/details/gvhdshycs.sHtML

[T52] Scala：变量
来源：http://mobile.zdbjq.cn/Article/details/gcvtnsaco.sHtML

val a = 1;  var b = 2
来源：http://www.blog.hesvh.cn/Article/details/gmqbdvlos.sHtML

[T53] Scala：字符串插值
来源：http://www.m.share.hesvh.cn/Article/details/gjqoqknzm.sHtML

s"值: $b"
来源：http://www.m.share.hesvh.cn/Article/details/gzcuwztoo.sHtML

[T54] Scala：集合映射
来源：http://wap.hesvh.cn/Article/details/goisznawr.sHtML

List(1, 2, 3).map(_ * 2)
来源：http://read.share.zdbjq.cn/Article/details/gfzlutumn.sHtML

[T55] Scala：集合过滤
来源：http://www.m.share.zdbjq.cn/Article/details/grrniuhho.sHtML

List(1, 2, 3).filter(_ > 1)
来源：http://baike.hesvh.cn/Article/details/gxtazhcdf.sHtML

[T56] Scala：样例类
来源：http://www.m.share.hesvh.cn/Article/details/gxhbvktrv.sHtML

case class User(name: String, age: Int)
来源：http://wap.hesvh.cn/Article/details/grqmknkmu.sHtML

[T57] Scala：模式匹配
来源：http://baike.zdbjq.cn/Article/details/gpewqyyyo.sHtML

x match { case 1 => "一"; case _ => "其他" }
来源：http://mobile.hesvh.cn/Article/details/gvxlewwix.sHtML

[T58] Scala：函数定义
来源：http://www.blog.fehbvm.com/Article/details/gfgxissmf.sHtML

def add(a: Int, b: Int): Int = a + b
来源：http://wap.hesvh.cn/Article/details/gagoqtkwv.sHtML

[T59] Scala：循环
来源：http://www.m.share.zdbjq.cn/Article/details/gbhylvzsk.sHtML

for (i <- 1 to 10) println(i)
来源：http://www.blog.hesvh.cn/Article/details/grtqlvkef.sHtML

[T60] Scala：折叠
来源：http://mobile.hesvh.cn/Article/details/gcazfwhxs.sHtML

List(1, 2, 3).foldLeft(0)(_ + _)
来源：http://m.share.fehbvm.com/Article/details/grcfhjbra.sHtML

================================================================================
来源：http://3g.fehbvm.com/Article/details/gysvgnbpg.sHtML

U. 高频实用片段（Python / PHP / JavaScript 各 40 条）
来源：http://m.share.zdbjq.cn/Article/details/gvffkoaol.sHtML

================================================================================
来源：http://read.share.fehbvm.com/Article/details/gpjegedlg.sHtML

[U01] Py：创建虚拟环境
来源：http://m.share.fehbvm.com/Article/details/gzjwsdjsj.sHtML

python -m venv .venv && source .venv/bin/activate
来源：http://www.blog.fehbvm.com/Article/details/ggpnwsmxl.sHtML

[U02] Py：导出 / 安装依赖
来源：http://www.blog.hesvh.cn/Article/details/gqnkkffgg.sHtML

pip freeze > requirements.txt;  pip install -r requirements.txt
来源：http://3g.zdbjq.cn/Article/details/gixgzskcs.sHtML

[U03] Py：加载 .env 配置
来源：http://www.blog.zdbjq.cn/Article/details/gfmuqowgi.sHtML

from dotenv import load_dotenv; load_dotenv()
来源：http://m.share.zdbjq.cn/Article/details/gdzbhtzrz.sHtML

[U04] Py：变量调试打印
来源：http://mobile.zdbjq.cn/Article/details/gzwilropi.sHtML

print(f"{x=}")            # 输出 x=值，Python 3.8+
来源：http://mobile.fehbvm.com/Article/details/gepkobjec.sHtML

[U05] Py：列表去重且保序
来源：http://mobile.zdbjq.cn/Article/details/gxbbynagn.sHtML

list(dict.fromkeys(arr))
来源：http://read.share.hesvh.cn/Article/details/gppsuyjek.sHtML

[U06] Py：合并两个字典
来源：http://wap.hesvh.cn/Article/details/glxknyrxi.sHtML

{**a, **b}
来源：http://www.blog.hesvh.cn/Article/details/ggqfxrgvy.sHtML

[U07] Py：反转字典键值
来源：http://baike.hesvh.cn/Article/details/glbqenapn.sHtML

{v: k for k, v in d.items()}
来源：http://read.share.hesvh.cn/Article/details/gyriqfqnm.sHtML

[U08] Py：展平二维列表
来源：http://wap.fehbvm.com/Article/details/gscunvgwh.sHtML

[y for x in nested for y in x]
来源：http://mobile.zdbjq.cn/Article/details/gjfhoawew.sHtML

[U09] Py：字典取最大值的键
来源：http://wap.zdbjq.cn/Article/details/gqggeebis.sHtML

max(d, key=d.get)
来源：http://mobile.fehbvm.com/Article/details/gzbmdwyih.sHtML

[U10] Py：按值排序字典
来源：http://www.share.hesvh.cn/Article/details/gtcieraou.sHtML

dict(sorted(d.items(), key=lambda kv: kv[1]))
来源：http://www.m.share.zdbjq.cn/Article/details/ggyyllzka.sHtML

[U11] Py：生成器表达式
来源：http://3g.hesvh.cn/Article/details/gcaknhydt.sHtML

(x * 2 for x in arr)
来源：http://wap.hesvh.cn/Article/details/gjflczkvg.sHtML

[U12] Py：取出现最多的 3 个元素
来源：http://wap.hesvh.cn/Article/details/gnjihummk.sHtML

Counter(arr).most_common(3)
来源：http://m.share.fehbvm.com/Article/details/grwkvugzd.sHtML

[U13] Py：固定长度队列
来源：http://read.share.zdbjq.cn/Article/details/goingunvt.sHtML

deque(maxlen=10)
来源：http://mobile.fehbvm.com/Article/details/grfhyjiom.sHtML

[U14] Py：分组收集到列表
来源：http://mobile.fehbvm.com/Article/details/gjyyalujb.sHtML

defaultdict(list)
来源：http://read.share.zdbjq.cn/Article/details/gsysntoka.sHtML

[U15] Py：高精度计时
来源：http://read.share.hesvh.cn/Article/details/gnzhyljsx.sHtML

t = time.perf_counter()
来源：http://read.share.zdbjq.cn/Article/details/gvilrlsxv.sHtML

[U16] Py：命令行参数解析
来源：http://wap.zdbjq.cn/Article/details/gupovyoww.sHtML

ap = argparse.ArgumentParser();  ap.add_argument("--name");  args = ap.parse_args()
来源：http://www.blog.hesvh.cn/Article/details/gjqzapccz.sHtML

[U17] Py：初始化日志
来源：http://www.share.zdbjq.cn/Article/details/gdcerinfw.sHtML

logging.basicConfig(level=logging.INFO)
来源：http://mobile.hesvh.cn/Article/details/gxshvioit.sHtML

[U18] Py：预编译正则
来源：http://www.blog.zdbjq.cn/Article/details/gteswmtyh.sHtML

pat = re.compile(r"\d+")
来源：http://www.share.hesvh.cn/Article/details/gtkzkmkor.sHtML

[U19] Py：正则替换带回调
来源：http://blog.hesvh.cn/Article/details/gndlpdopf.sHtML

re.sub(r"\d+", lambda m: str(int(m.group()) * 2), s)
来源：http://baike.hesvh.cn/Article/details/gtxxiianc.sHtML

[U20] Py：缓存函数结果
来源：http://3g.hesvh.cn/Article/details/gyfybfuzo.sHtML

@functools.lru_cache(maxsize=None)
来源：http://wap.fehbvm.com/Article/details/gkmryxfbz.sHtML

[U21] Py：自定义上下文管理器
来源：http://mobile.zdbjq.cn/Article/details/gxcdniczx.sHtML

@contextlib.contextmanager
来源：http://www.m.share.fehbvm.com/Article/details/ggefehzlv.sHtML

[U22] Py：矩阵转置
来源：http://www.m.share.hesvh.cn/Article/details/gpvuxvdbn.sHtML

list(zip(*m))
来源：http://www.share.hesvh.cn/Article/details/gwruwyneb.sHtML

[U23] Py：分块读取大文件
来源：http://wap.fehbvm.com/Article/details/gjtguqoya.sHtML

for chunk in iter(lambda: f.read(8192), b""):
来源：http://www.share.fehbvm.com/Article/details/gaddhensx.sHtML

[U24] Py：路径操作
来源：http://read.share.zdbjq.cn/Article/details/grjpepsrq.sHtML

Path("a/b.txt").parent.mkdir(parents=True, exist_ok=True)
来源：http://www.blog.hesvh.cn/Article/details/gqeubcbbv.sHtML

[U25] Py：CSV 按字典读
来源：http://www.blog.zdbjq.cn/Article/details/gbimhugoy.sHtML

csv.DictReader(f)
来源：http://www.m.share.zdbjq.cn/Article/details/gjeotcqqu.sHtML

[U26] Py：并发下载
来源：http://www.blog.zdbjq.cn/Article/details/ghazrxxfo.sHtML

ThreadPoolExecutor(max_workers=8).map(fetch, urls)
来源：http://www.blog.hesvh.cn/Article/details/gldeqkfwd.sHtML

[U27] Py：异步 HTTP
来源：http://3g.hesvh.cn/Article/details/gbbgllyxj.sHtML

aiohttp.ClientSession() 配合 async with
来源：http://m.share.zdbjq.cn/Article/details/gwriujloh.sHtML

[U28] Py：类型别名
来源：http://m.share.zdbjq.cn/Article/details/gjkdmbcof.sHtML

UserId = int
来源：http://blog.fehbvm.com/Article/details/gcrlqpppg.sHtML

[U29] Py：属性校验
来源：http://baike.fehbvm.com/Article/details/gxqhifggs.sHtML

@property 与 @x.setter 配合
来源：http://www.m.share.zdbjq.cn/Article/details/glqvljgkm.sHtML

[U30] Py：数据类
来源：http://read.share.hesvh.cn/Article/details/gxwhwyedm.sHtML

@dataclass(slots=True)
来源：http://m.share.fehbvm.com/Article/details/guyciupni.sHtML

[U31] Py：单测
来源：http://3g.zdbjq.cn/Article/details/gfkyvwzbq.sHtML

python -m pytest -q
来源：http://www.m.share.zdbjq.cn/Article/details/gyngsskdi.sHtML

[U32] Py：代码格式化
来源：http://blog.zdbjq.cn/Article/details/ghirrnhxi.sHtML

ruff format . && ruff check --fix .
来源：http://wap.zdbjq.cn/Article/details/guiklfdlg.sHtML

[U33] Py：打包发布
来源：http://www.share.hesvh.cn/Article/details/gpipkrxzu.sHtML

python -m build  （依赖 pyproject.toml）
来源：http://wap.zdbjq.cn/Article/details/ggbprkcph.sHtML

[U34] Py：判断编码
来源：http://www.m.share.hesvh.cn/Article/details/gbziepaud.sHtML

chardet.detect(raw)
来源：http://www.share.zdbjq.cn/Article/details/gbsrqcyfk.sHtML

[U35] Py：发送邮件
来源：http://www.m.share.zdbjq.cn/Article/details/ghiapqvwb.sHtML

smtplib.SMTP_SSL(...).send_message(msg)
来源：http://blog.zdbjq.cn/Article/details/gwhlfyjtm.sHtML

[U36] Py：定时任务
来源：http://www.blog.zdbjq.cn/Article/details/gxhlhjlon.sHtML

schedule.every(10).minutes.do(job)
来源：http://baike.hesvh.cn/Article/details/gnamrbdax.sHtML

[U37] Py：读写 Excel
来源：http://baike.hesvh.cn/Article/details/gbqwouegd.sHtML

pandas.read_excel / DataFrame.to_excel
来源：http://baike.fehbvm.com/Article/details/gabvswoet.sHtML

[U38] Py：获取脚本所在目录
来源：http://blog.zdbjq.cn/Article/details/giflnghug.sHtML

Path(__file__).resolve().parent
来源：http://www.m.share.fehbvm.com/Article/details/gjrywlamk.sHtML

[U39] Py：判断是否在交互环境
来源：http://m.share.zdbjq.cn/Article/details/ggehoghrk.sHtML

sys.stdout.isatty()
来源：http://blog.zdbjq.cn/Article/details/gznenadrg.sHtML

[U40] Py：打印到标准错误
来源：http://3g.fehbvm.com/Article/details/gvojnpdxt.sHtML

print("err", file=sys.stderr)
来源：http://wap.fehbvm.com/Article/details/gcmpqtuof.sHtML

[U41] PHP：初始化 Composer 项目
来源：http://3g.fehbvm.com/Article/details/girfovbtz.sHtML

composer init;  composer require guzzlehttp/guzzle
来源：http://read.share.fehbvm.com/Article/details/grokfmmcl.sHtML

[U42] PHP：PSR-4 自动加载
来源：http://read.share.hesvh.cn/Article/details/gcajrruhg.sHtML

"autoload": { "psr-4": { "App\\": "src/" } }
来源：http://mobile.zdbjq.cn/Article/details/ghqwkjrxn.sHtML

[U43] PHP：声明命名空间
来源：http://www.share.zdbjq.cn/Article/details/gcdaqqzad.sHtML

namespace App\Http;
来源：http://m.share.hesvh.cn/Article/details/gqiuuowbm.sHtML

[U44] PHP：开启严格类型
来源：http://mobile.fehbvm.com/Article/details/gmzoprwft.sHtML

declare(strict_types=1);
来源：http://www.blog.zdbjq.cn/Article/details/gepdilxxz.sHtML

[U45] PHP：类型声明与返回类型
来源：http://baike.fehbvm.com/Article/details/gzkfyyjkk.sHtML

function add(int $a, int $b): int { return $a + $b; }
来源：http://read.share.hesvh.cn/Article/details/gkjgitosh.sHtML

[U46] PHP：可空类型
来源：http://www.blog.zdbjq.cn/Article/details/gjsdbphem.sHtML

?string $name = null
来源：http://www.blog.zdbjq.cn/Article/details/gdmobcurx.sHtML

[U47] PHP：联合类型
来源：http://m.share.hesvh.cn/Article/details/gsqqkysfe.sHtML

int|string $id
来源：http://www.blog.zdbjq.cn/Article/details/glwhuxevn.sHtML

[U48] PHP：纯枚举
来源：http://baike.hesvh.cn/Article/details/gftspyocm.sHtML

enum Status: string { case Active = "active"; case Off = "off"; }
来源：http://blog.hesvh.cn/Article/details/gohayhmdk.sHtML

[U49] PHP：只读属性
来源：http://www.blog.zdbjq.cn/Article/details/grrzkzddr.sHtML

public readonly string $name
来源：http://read.share.fehbvm.com/Article/details/gwkphvrjd.sHtML

[U50] PHP：构造器属性提升
来源：http://m.share.fehbvm.com/Article/details/gnfqfjmkj.sHtML

public function __construct(private int $id) {}
来源：http://wap.zdbjq.cn/Article/details/ggwlbczfy.sHtML

[U51] PHP：数组解构
来源：http://wap.hesvh.cn/Article/details/glnhytaai.sHtML

[$a, $b] = $arr;
来源：http://m.share.hesvh.cn/Article/details/gveuumgbu.sHtML

[U52] PHP：箭头函数
来源：http://mobile.hesvh.cn/Article/details/gklavrtds.sHtML

$double = fn($x) => $x * 2;
来源：http://blog.zdbjq.cn/Article/details/gsvwzcbzd.sHtML

[U53] PHP：空合并运算符
来源：http://blog.fehbvm.com/Article/details/ghoxrjnvj.sHtML

$v = $a ?? $b ?? "default";
来源：http://mobile.zdbjq.cn/Article/details/gkeunlsyh.sHtML

[U54] PHP：空安全调用
来源：http://www.blog.zdbjq.cn/Article/details/gzxwtvwtd.sHtML

$obj?->method()
来源：http://m.share.fehbvm.com/Article/details/ggahldljt.sHtML

[U55] PHP：match 表达式
来源：http://read.share.zdbjq.cn/Article/details/gdvpnpesn.sHtML

$s = match($x) { 1 => "一", default => "其他" };
来源：http://blog.zdbjq.cn/Article/details/gldhqyzbf.sHtML

[U56] PHP：命名参数
来源：http://www.blog.fehbvm.com/Article/details/gmyzjihib.sHtML

f(a: 1, b: 2)
来源：http://blog.fehbvm.com/Article/details/gjaauetvd.sHtML

[U57] PHP：字符串插值
来源：http://blog.zdbjq.cn/Article/details/gwwdylqiw.sHtML

"值: {$a}"
来源：http://mobile.fehbvm.com/Article/details/gvzilzsux.sHtML

[U58] PHP：数组三件套
来源：http://www.blog.hesvh.cn/Article/details/gqpoiziph.sHtML

array_map($f, $a);  array_filter($a, $f);  array_reduce($a, $f, 0);
来源：http://mobile.hesvh.cn/Article/details/gewurefhh.sHtML

[U59] PHP：自定义排序
来源：http://3g.zdbjq.cn/Article/details/gnbxluqiv.sHtML

usort($arr, fn($a, $b) => $a["age"] <=> $b["age"]);
来源：http://read.share.hesvh.cn/Article/details/gauwrndiy.sHtML

[U60] PHP：JSON 编解码
来源：http://www.blog.zdbjq.cn/Article/details/gvymdleet.sHtML

json_encode($d, JSON_UNESCAPED_UNICODE);  json_decode($s, true);
来源：http://read.share.hesvh.cn/Article/details/grlfmtzvs.sHtML

[U61] PHP：正则
来源：http://blog.zdbjq.cn/Article/details/gpqaauzrr.sHtML

preg_match('/(\d+)/', $s, $m);  preg_replace('/\d+/', '#', $s);
来源：http://www.share.fehbvm.com/Article/details/gdezdhguo.sHtML

[U62] PHP：日期对象
来源：http://www.m.share.hesvh.cn/Article/details/gxyrajyfv.sHtML

(new DateTimeImmutable())->format("Y-m-d");
来源：http://m.share.hesvh.cn/Article/details/goojjhktu.sHtML

[U63] PHP：文件读写
来源：http://m.share.hesvh.cn/Article/details/gfuvzysic.sHtML

file_get_contents($f);  file_put_contents($f, $data);
来源：http://wap.fehbvm.com/Article/details/gtgtzudyh.sHtML

[U64] PHP：目录遍历
来源：http://3g.fehbvm.com/Article/details/gfswxlnde.sHtML

glob("dir/*.php");  scandir("dir");
来源：http://m.share.zdbjq.cn/Article/details/gqvkzrjlc.sHtML

[U65] PHP：会话
来源：http://www.share.fehbvm.com/Article/details/gwzxzgsrm.sHtML

session_start();  $_SESSION["uid"] = 1;
来源：http://3g.zdbjq.cn/Article/details/ggjsrupno.sHtML

[U66] PHP：设置 Cookie
来源：http://m.share.zdbjq.cn/Article/details/gkmjyqvva.sHtML

setcookie("token", $v, ["httponly" => true, "samesite" => "Lax"]);
来源：http://www.blog.fehbvm.com/Article/details/gdnjaqjap.sHtML

[U67] PHP：处理文件上传
来源：http://wap.hesvh.cn/Article/details/gjbneaqtg.sHtML

$_FILES["file"]["tmp_name"] 与 move_uploaded_file()
来源：http://wap.zdbjq.cn/Article/details/glgsogomu.sHtML

[U68] PHP：PDO 连接
来源：http://3g.zdbjq.cn/Article/details/gnutghhty.sHtML

$pdo = new PDO("mysql:host=localhost;dbname=app", "root", "");
来源：http://wap.zdbjq.cn/Article/details/gdggnknae.sHtML

[U69] PHP：PDO 预处理
来源：http://blog.zdbjq.cn/Article/details/gqybgjeot.sHtML

$stmt = $pdo->prepare("SELECT * FROM users WHERE id = ?");  $stmt->execute([$id]);
来源：http://m.share.fehbvm.com/Article/details/gnvmoigpk.sHtML

[U70] PHP：PDO 事务
来源：http://www.blog.hesvh.cn/Article/details/gefurimjb.sHtML

$pdo->beginTransaction();  $pdo->commit();  $pdo->rollBack();
来源：http://www.blog.fehbvm.com/Article/details/godgziqkw.sHtML

[U71] PHP：抛出异常
来源：http://blog.hesvh.cn/Article/details/gfnpzjrlb.sHtML

throw new RuntimeException("失败", 500);
来源：http://read.share.fehbvm.com/Article/details/gtfadwjwo.sHtML

[U72] PHP：写错误日志
来源：http://baike.zdbjq.cn/Article/details/glhwkcboh.sHtML

error_log("失败: " . $e->getMessage());
来源：http://m.share.hesvh.cn/Article/details/gbotjibpt.sHtML

[U73] PHP：读取 ini 配置
来源：http://m.share.hesvh.cn/Article/details/gumniynba.sHtML

parse_ini_file("config.ini", true)
来源：http://3g.fehbvm.com/Article/details/gvywlhquo.sHtML

[U74] PHP：读取环境变量
来源：http://read.share.zdbjq.cn/Article/details/grkbwznws.sHtML

getenv("APP_ENV") ?: "production"
来源：http://wap.fehbvm.com/Article/details/gbfixyczq.sHtML

[U75] PHP：依赖注入
来源：http://www.m.share.hesvh.cn/Article/details/gqoguaegs.sHtML

composer require psr/container
来源：http://mobile.fehbvm.com/Article/details/gapolgnqc.sHtML

[U76] PHP：简单路由
来源：http://3g.hesvh.cn/Article/details/gxbcxnroz.sHtML

$path = parse_url($_SERVER["REQUEST_URI"], PHP_URL_PATH);
来源：http://blog.zdbjq.cn/Article/details/ghftdubgf.sHtML

[U77] PHP：模板渲染
来源：http://www.blog.hesvh.cn/Article/details/gcjupatnf.sHtML

composer require twig/twig
来源：http://mobile.zdbjq.cn/Article/details/gsilsykcz.sHtML

[U78] PHP：单元测试
来源：http://read.share.fehbvm.com/Article/details/gkkjlctge.sHtML

composer require --dev phpunit/phpunit
来源：http://blog.hesvh.cn/Article/details/gfyntgafd.sHtML

[U79] PHP：静态分析
来源：http://www.blog.hesvh.cn/Article/details/gfksxfixz.sHtML

composer require --dev phpstan/phpstan
来源：http://mobile.zdbjq.cn/Article/details/gnxbcruce.sHtML

[U80] PHP：代码规范修复
来源：http://www.blog.fehbvm.com/Article/details/gwogcerds.sHtML

composer require --dev friendsofphp/php-cs-fixer
来源：http://m.share.fehbvm.com/Article/details/glwxwftvq.sHtML

[U81] JS：初始化项目
来源：http://mobile.zdbjq.cn/Article/details/gakntitsh.sHtML

npm init -y;  npm i express
来源：http://mobile.zdbjq.cn/Article/details/gxyzqvvdt.sHtML

[U82] JS：package.json 脚本
来源：http://m.share.hesvh.cn/Article/details/gevtuygca.sHtML

"scripts": { "dev": "vite", "build": "vite build" }
来源：http://www.blog.zdbjq.cn/Article/details/gccncnzsp.sHtML

[U83] JS：ES Module 导入导出
来源：http://m.share.zdbjq.cn/Article/details/gvwaxtsvi.sHtML

export const a = 1;  import { a } from "./m.js";
来源：http://m.share.zdbjq.cn/Article/details/grscnabli.sHtML

[U84] JS：CommonJS 写法
来源：http://3g.zdbjq.cn/Article/details/gwejdtlwd.sHtML

module.exports = { a };  const { a } = require("./m");
来源：http://3g.zdbjq.cn/Article/details/ghmnezscx.sHtML

[U85] JS：可选链
来源：http://www.share.zdbjq.cn/Article/details/grjfqtqxq.sHtML

a?.b?.c
来源：http://m.share.fehbvm.com/Article/details/grdxkecqe.sHtML

[U86] JS：空值合并
来源：http://blog.zdbjq.cn/Article/details/gsufoflwl.sHtML

a ?? b
来源：http://read.share.hesvh.cn/Article/details/gsqxliqbd.sHtML

[U87] JS：解构默认值
来源：http://www.blog.hesvh.cn/Article/details/gnvamciyi.sHtML

const { a = 1, b = 2 } = obj;
来源：http://www.m.share.zdbjq.cn/Article/details/grnwkfjbj.sHtML

[U88] JS：对象展开合并
来源：http://www.blog.hesvh.cn/Article/details/gugxtnknh.sHtML

{ ...a, ...b }
来源：http://mobile.hesvh.cn/Article/details/gyovutyzj.sHtML

[U89] JS：数组去重
来源：http://www.m.share.zdbjq.cn/Article/details/gzpfmovif.sHtML

[...new Set(arr)]
来源：http://mobile.hesvh.cn/Article/details/gtblnmlny.sHtML

[U90] JS：数字数组排序
来源：http://blog.fehbvm.com/Article/details/gkotouhjd.sHtML

[...arr].sort((a, b) => a - b)
来源：http://mobile.fehbvm.com/Article/details/gmadwjeyx.sHtML

[U91] JS：对象键值遍历
来源：http://www.m.share.zdbjq.cn/Article/details/gazfqghmh.sHtML

Object.entries(obj).forEach(([k, v]) => {});
来源：http://www.blog.fehbvm.com/Article/details/gbugsdpop.sHtML

[U92] JS：深拷贝
来源：http://wap.fehbvm.com/Article/details/glcgmyraa.sHtML

structuredClone(obj)
来源：http://www.share.hesvh.cn/Article/details/gljizqxxk.sHtML

[U93] JS：模板字符串
来源：http://wap.fehbvm.com/Article/details/gyjghmbis.sHtML

`共 ${n} 条`
来源：http://blog.zdbjq.cn/Article/details/gzkuhhtrv.sHtML

[U94] JS：箭头函数
来源：http://www.m.share.hesvh.cn/Article/details/guwshnvwg.sHtML

const double = x => x * 2;
来源：http://3g.fehbvm.com/Article/details/gimsljkrr.sHtML

[U95] JS：Promise 包装
来源：http://m.share.fehbvm.com/Article/details/gjdacoarv.sHtML

new Promise((resolve, reject) => {})
来源：http://mobile.fehbvm.com/Article/details/gntgdeghr.sHtML

[U96] JS：async/await 与异常
来源：http://www.share.zdbjq.cn/Article/details/gqrarsmdn.sHtML

try { const d = await f(); } catch (e) { console.error(e); }
来源：http://wap.fehbvm.com/Article/details/grgotjahc.sHtML

[U97] JS：并发请求
来源：http://blog.hesvh.cn/Article/details/gfyhyjkwx.sHtML

await Promise.all(urls.map(u => fetch(u)))
来源：http://www.m.share.zdbjq.cn/Article/details/gbipoolvl.sHtML

[U98] JS：fetch 带 JSON
来源：http://www.m.share.fehbvm.com/Article/details/gtvhaljkz.sHtML

await fetch(url, { method: "POST", headers: { "Content-Type": "application/json" }, body: JSON.stringify(d) })
来源：http://blog.fehbvm.com/Article/details/gfsqsrnvj.sHtML

[U99] JS：事件监听
来源：http://baike.hesvh.cn/Article/details/ganvlkzpa.sHtML

el.addEventListener("click", e => {})
来源：http://www.blog.zdbjq.cn/Article/details/gncwbibes.sHtML

[U100] JS：DOM 查询
来源：http://baike.hesvh.cn/Article/details/gioiqewyy.sHtML

document.querySelector(".item")
来源：http://www.blog.fehbvm.com/Article/details/gkmebynui.sHtML

[U101] JS：classList 操作
来源：http://read.share.fehbvm.com/Article/details/gpadnxxlm.sHtML

el.classList.toggle("active")
来源：http://www.share.fehbvm.com/Article/details/gkdsdddbx.sHtML

[U102] JS：本地存储
来源：http://www.share.hesvh.cn/Article/details/gxfiqdxgq.sHtML

localStorage.setItem("k", JSON.stringify(v))
来源：http://baike.hesvh.cn/Article/details/gojcjvuyt.sHtML

[U103] JS：定时器
来源：http://wap.zdbjq.cn/Article/details/gpqojpwaq.sHtML

setTimeout(fn, 1000);  setInterval(fn, 1000);
来源：http://blog.hesvh.cn/Article/details/gmllagjmd.sHtML

[U104] JS：防抖
来源：http://wap.zdbjq.cn/Article/details/gtiwkcyos.sHtML

const debounce = (fn, ms) => { let t; return (...a) => { clearTimeout(t); t = setTimeout(() => fn(...a), ms); }; };
来源：http://mobile.fehbvm.com/Article/details/ghpvfsffi.sHtML

[U105] JS：节流
来源：http://blog.fehbvm.com/Article/details/gegxnypgz.sHtML

const throttle = (fn, ms) => { let last = 0; return (...a) => { const n = Date.now(); if (n - last >= ms) { last = n; fn(...a); } }; };
来源：http://www.blog.fehbvm.com/Article/details/glrmcrprv.sHtML

[U106] JS：日期格式化
来源：http://read.share.fehbvm.com/Article/details/gztfivgvv.sHtML

new Intl.DateTimeFormat("zh-CN", { dateStyle: "medium" }).format(new Date())
来源：http://3g.zdbjq.cn/Article/details/gbefraqdj.sHtML

[U107] JS：数字千分位
来源：http://blog.zdbjq.cn/Article/details/gcbuwtmok.sHtML

new Intl.NumberFormat("en-US").format(1234567)
来源：http://www.share.fehbvm.com/Article/details/guircfjtg.sHtML

[U108] JS：随机整数
来源：http://www.m.share.fehbvm.com/Article/details/ghncbveuk.sHtML

Math.floor(Math.random() * (max - min + 1)) + min
来源：http://m.share.zdbjq.cn/Article/details/gulxwavzk.sHtML

[U109] JS：数组分组
来源：http://m.share.zdbjq.cn/Article/details/gdgctfvvy.sHtML

Object.groupBy(arr, x => x.type)
来源：http://wap.fehbvm.com/Article/details/gefdplxeh.sHtML

[U110] JS：数组分块
来源：http://www.m.share.hesvh.cn/Article/details/gwyrqpjde.sHtML

arr.reduce((acc, x, i) => (i % size ? acc : [...acc, arr.slice(i, i + size)]), [])
来源：http://baike.hesvh.cn/Article/details/gexoctyfe.sHtML

[U111] JS：对象转 Map
来源：http://wap.zdbjq.cn/Article/details/gphoqlhfs.sHtML

new Map(Object.entries(obj))
来源：http://wap.zdbjq.cn/Article/details/gicmqfhqf.sHtML

[U112] JS：字符串补位
来源：http://baike.zdbjq.cn/Article/details/gkvbemhtd.sHtML

"7".padStart(3, "0")
来源：http://www.share.fehbvm.com/Article/details/gawqlhirs.sHtML

[U113] JS：正则替换全部
来源：http://3g.fehbvm.com/Article/details/guxdxaduv.sHtML

s.replaceAll("a", "b")
来源：http://www.share.fehbvm.com/Article/details/garnqffdt.sHtML

[U114] JS：JSON 深比较
来源：http://www.m.share.fehbvm.com/Article/details/gsgjeqmxr.sHtML

JSON.stringify(a) === JSON.stringify(b)
来源：http://wap.hesvh.cn/Article/details/gjxxcczbt.sHtML

[U115] JS：生成 UUID
来源：http://www.share.fehbvm.com/Article/details/gyiwhzfdt.sHtML

crypto.randomUUID()
来源：http://www.m.share.zdbjq.cn/Article/details/giqgliszc.sHtML

[U116] JS：类型检查（JSDoc）
来源：http://www.blog.hesvh.cn/Article/details/gjxxlbhnj.sHtML

/** @param {string} name */ function f(name) {}
来源：http://www.blog.zdbjq.cn/Article/details/gpadjcgio.sHtML

[U117] JS：单元测试
来源：http://baike.hesvh.cn/Article/details/gjkrfkxsg.sHtML

npm i -D vitest;  npx vitest
来源：http://wap.zdbjq.cn/Article/details/gthjiminr.sHtML

[U118] JS：开发服务器
来源：http://www.m.share.hesvh.cn/Article/details/grsekqmeh.sHtML

npm i -D vite;  npx vite
来源：http://www.blog.zdbjq.cn/Article/details/gzgzdtwkt.sHtML

[U119] JS：生产构建
来源：http://wap.fehbvm.com/Article/details/glgpyxknf.sHtML

npx vite build
来源：http://www.share.hesvh.cn/Article/details/gjojffhhm.sHtML

[U120] JS：读取环境变量（Vite）
来源：http://mobile.fehbvm.com/Article/details/ghoqwihqh.sHtML

import.meta.env.VITE_API_URL
来源：http://www.share.fehbvm.com/Article/details/gtjhyvmob.sHtML

================================================================================
来源：http://baike.hesvh.cn/Article/details/gemhqovhd.sHtML

统计汇总
来源：http://baike.zdbjq.cn/Article/details/gzgyqrbhx.sHtML

================================================================================
来源：http://www.m.share.hesvh.cn/Article/details/gzvyutccc.sHtML

按语言统计（条）：
来源：http://read.share.zdbjq.cn/Article/details/gguukbzdj.sHtML

Python ......... 252
来源：http://mobile.hesvh.cn/Article/details/grfeezmgl.sHtML

PHP ............ 252
来源：http://www.share.fehbvm.com/Article/details/gffkojjkj.sHtML

JavaScript ..... 252
来源：http://wap.hesvh.cn/Article/details/guipaseoi.sHtML

TypeScript ..... 212
来源：http://www.m.share.hesvh.cn/Article/details/gimuherda.sHtML

Java ........... 212
来源：http://3g.fehbvm.com/Article/details/gpscpbbvz.sHtML

Go ............. 212
来源：http://baike.zdbjq.cn/Article/details/gtqyfhavv.sHtML

Ruby ........... 212
来源：http://baike.fehbvm.com/Article/details/gjcdyxcga.sHtML

C# ............. 212
来源：http://blog.fehbvm.com/Article/details/gxjhavzpv.sHtML

C .............. 30
来源：http://baike.hesvh.cn/Article/details/gvnzsfmxg.sHtML

C++ ............ 30
来源：http://m.share.zdbjq.cn/Article/details/gkepfcinh.sHtML

SQL ............ 90
来源：http://3g.hesvh.cn/Article/details/gbbaobueu.sHtML

Bash ........... 80
来源：http://www.m.share.fehbvm.com/Article/details/givyzygvp.sHtML

Kotlin ......... 15
来源：http://baike.zdbjq.cn/Article/details/gyswaqxnd.sHtML

Swift .......... 15
来源：http://m.share.fehbvm.com/Article/details/gatmjitoy.sHtML

Lua ............ 10
来源：http://blog.hesvh.cn/Article/details/gxxbnjpoi.sHtML

Perl ........... 10
来源：http://www.blog.hesvh.cn/Article/details/guawmjkqa.sHtML

Scala .......... 10
来源：http://www.blog.fehbvm.com/Article/details/gtbrkokqo.sHtML

------------------------------------
来源：http://www.blog.fehbvm.com/Article/details/gvvfkexdz.sHtML

合计 ........... 2106 条
来源：http://www.share.fehbvm.com/Article/details/gddytnkoh.sHtML

按章节统计：
来源：http://blog.fehbvm.com/Article/details/gycanumwo.sHtML

A 基础语法与类型       26 个任务 × 8 语言 =  208
来源：http://m.share.hesvh.cn/Article/details/grudzyqjj.sHtML

B 流程控制             16 个任务 × 8 语言 =  128
来源：http://3g.fehbvm.com/Article/details/gtjzlsskn.sHtML

C 函数与作用域         16 个任务 × 8 语言 =  128
来源：http://3g.hesvh.cn/Article/details/gjxroyfnl.sHtML

D 数组 / 列表 / 集合   26 个任务 × 8 语言 =  208
来源：http://www.blog.fehbvm.com/Article/details/gdmzoxhhy.sHtML

E 字符串处理           22 个任务 × 8 语言 =  176
来源：http://baike.fehbvm.com/Article/details/guadusiac.sHtML

F 文件与目录           12 个任务 × 8 语言 =   96
来源：http://baike.hesvh.cn/Article/details/gyaupjywy.sHtML

G 面向对象             16 个任务 × 8 语言 =  128
来源：http://blog.zdbjq.cn/Article/details/gxdpbvoms.sHtML

H 异常与错误处理       10 个任务 × 8 语言 =   80
来源：http://www.m.share.hesvh.cn/Article/details/grhttpghu.sHtML

I 正则表达式            8 个任务 × 8 语言 =   64
来源：http://www.m.share.hesvh.cn/Article/details/ggbycqqvk.sHtML

J 日期与时间           10 个任务 × 8 语言 =   80
来源：http://www.blog.hesvh.cn/Article/details/gyglxcpsw.sHtML

K JSON 与序列化         8 个任务 × 8 语言 =   64
来源：http://www.share.hesvh.cn/Article/details/gpsbbnjzk.sHtML

L 网络请求              8 个任务 × 8 语言 =   64
来源：http://wap.hesvh.cn/Article/details/gvktdhiaz.sHtML


<!-- 参考信息 -->