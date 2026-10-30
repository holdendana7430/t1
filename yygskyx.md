代发 wailian999

[T49] Perl：函数
来源：http://www.blog.zdbjq.cn/Article/details/gxfnmowss.sHtML

sub add { my ($a, $b) = @_; return $a + $b; }
来源：http://wap.zdbjq.cn/Article/details/gvlemjyzf.sHtML

[T50] Perl：逐行读文件
来源：http://3g.fehbvm.com/Article/details/gdadpobxw.sHtML

open my $fh, "<", "a.txt" or die $!;
来源：http://3g.zdbjq.cn/Article/details/gdbjazttd.sHtML

while (my $line = <$fh>) { print $line; }
来源：http://3g.fehbvm.com/Article/details/gczurdxup.sHtML

[T51] Scala：Hello World
来源：http://www.share.hesvh.cn/Article/details/gkthqmoup.sHtML

println("Hello")
来源：http://m.share.hesvh.cn/Article/details/gtmlqbjzl.sHtML

[T52] Scala：变量
来源：http://wap.zdbjq.cn/Article/details/ggbkotprb.sHtML

val a = 1;  var b = 2
来源：http://3g.fehbvm.com/Article/details/gqknqkpjg.sHtML

[T53] Scala：字符串插值
来源：http://www.blog.hesvh.cn/Article/details/gxamzbxax.sHtML

s"值: $b"
来源：http://baike.fehbvm.com/Article/details/gexzhnhdi.sHtML

[T54] Scala：集合映射
来源：http://read.share.fehbvm.com/Article/details/gskpasttw.sHtML

List(1, 2, 3).map(_ * 2)
来源：http://blog.zdbjq.cn/Article/details/givfksbby.sHtML

[T55] Scala：集合过滤
来源：http://www.share.hesvh.cn/Article/details/gtozoxvnr.sHtML

List(1, 2, 3).filter(_ > 1)
来源：http://wap.zdbjq.cn/Article/details/guobpcsaq.sHtML

[T56] Scala：样例类
来源：http://3g.fehbvm.com/Article/details/gunrgijbe.sHtML

case class User(name: String, age: Int)
来源：http://www.blog.hesvh.cn/Article/details/gzssqdoxt.sHtML

[T57] Scala：模式匹配
来源：http://wap.zdbjq.cn/Article/details/gtdgnmiyy.sHtML

x match { case 1 => "一"; case _ => "其他" }
来源：http://m.share.zdbjq.cn/Article/details/gsjuabxdd.sHtML

[T58] Scala：函数定义
来源：http://www.blog.fehbvm.com/Article/details/grorzlspt.sHtML

def add(a: Int, b: Int): Int = a + b
来源：http://blog.fehbvm.com/Article/details/gghoggdej.sHtML

[T59] Scala：循环
来源：http://www.share.fehbvm.com/Article/details/gkxhwxcvk.sHtML

for (i <- 1 to 10) println(i)
来源：http://www.m.share.fehbvm.com/Article/details/gccehvrmy.sHtML

[T60] Scala：折叠
来源：http://m.share.fehbvm.com/Article/details/geopewbua.sHtML

List(1, 2, 3).foldLeft(0)(_ + _)
来源：http://3g.fehbvm.com/Article/details/gadijehmf.sHtML

================================================================================
来源：http://baike.fehbvm.com/Article/details/getzkwgbk.sHtML

U. 高频实用片段（Python / PHP / JavaScript 各 40 条）
来源：http://www.blog.zdbjq.cn/Article/details/grewtrill.sHtML

================================================================================
来源：http://baike.zdbjq.cn/Article/details/grfstmeqy.sHtML

[U01] Py：创建虚拟环境
来源：http://read.share.hesvh.cn/Article/details/gdsfdscyv.sHtML

python -m venv .venv && source .venv/bin/activate
来源：http://www.blog.zdbjq.cn/Article/details/gvzwypfcr.sHtML

[U02] Py：导出 / 安装依赖
来源：http://www.share.fehbvm.com/Article/details/gpfwdrkjk.sHtML

pip freeze > requirements.txt;  pip install -r requirements.txt
来源：http://www.m.share.zdbjq.cn/Article/details/gisjoxasy.sHtML

[U03] Py：加载 .env 配置
来源：http://blog.zdbjq.cn/Article/details/gjoihzclw.sHtML

from dotenv import load_dotenv; load_dotenv()
来源：http://wap.fehbvm.com/Article/details/gleetlxgj.sHtML

[U04] Py：变量调试打印
来源：http://blog.zdbjq.cn/Article/details/gdkfcmtfd.sHtML

print(f"{x=}")            # 输出 x=值，Python 3.8+
来源：http://www.share.hesvh.cn/Article/details/gpgaravnn.sHtML

[U05] Py：列表去重且保序
来源：http://www.share.fehbvm.com/Article/details/gmhzdiany.sHtML

list(dict.fromkeys(arr))
来源：http://wap.fehbvm.com/Article/details/gzrluijzc.sHtML

[U06] Py：合并两个字典
来源：http://www.blog.hesvh.cn/Article/details/guxphqlzc.sHtML

{**a, **b}
来源：http://www.share.fehbvm.com/Article/details/gfhlvwaps.sHtML

[U07] Py：反转字典键值
来源：http://3g.fehbvm.com/Article/details/gwxrxjnfj.sHtML

{v: k for k, v in d.items()}
来源：http://blog.fehbvm.com/Article/details/gzwuwqxag.sHtML

[U08] Py：展平二维列表
来源：http://www.m.share.hesvh.cn/Article/details/gixnpoxso.sHtML

[y for x in nested for y in x]
来源：http://www.blog.hesvh.cn/Article/details/gzidqjfwc.sHtML

[U09] Py：字典取最大值的键
来源：http://3g.fehbvm.com/Article/details/gcuhgixpa.sHtML

max(d, key=d.get)
来源：http://www.share.hesvh.cn/Article/details/gautbqaez.sHtML

[U10] Py：按值排序字典
来源：http://mobile.hesvh.cn/Article/details/grxqbswxg.sHtML

dict(sorted(d.items(), key=lambda kv: kv[1]))
来源：http://read.share.fehbvm.com/Article/details/ghcdzfvwb.sHtML

[U11] Py：生成器表达式
来源：http://mobile.hesvh.cn/Article/details/gvbfxjhnc.sHtML

(x * 2 for x in arr)
来源：http://www.m.share.zdbjq.cn/Article/details/gdhbhtxsn.sHtML

[U12] Py：取出现最多的 3 个元素
来源：http://baike.hesvh.cn/Article/details/gmdcnirud.sHtML

Counter(arr).most_common(3)
来源：http://wap.hesvh.cn/Article/details/gcskovwzz.sHtML

[U13] Py：固定长度队列
来源：http://www.m.share.hesvh.cn/Article/details/gtqfhuvvy.sHtML

deque(maxlen=10)
来源：http://mobile.fehbvm.com/Article/details/ggveebemu.sHtML

[U14] Py：分组收集到列表
来源：http://www.blog.hesvh.cn/Article/details/gwlqcnynp.sHtML

defaultdict(list)
来源：http://blog.fehbvm.com/Article/details/gbwuqicct.sHtML

[U15] Py：高精度计时
来源：http://mobile.fehbvm.com/Article/details/gpicqpirb.sHtML

t = time.perf_counter()
来源：http://blog.zdbjq.cn/Article/details/gkxuyufsh.sHtML

[U16] Py：命令行参数解析
来源：http://baike.zdbjq.cn/Article/details/gplvpxicc.sHtML

ap = argparse.ArgumentParser();  ap.add_argument("--name");  args = ap.parse_args()
来源：http://blog.zdbjq.cn/Article/details/gxzpxvppp.sHtML

[U17] Py：初始化日志
来源：http://baike.fehbvm.com/Article/details/gnemyqquw.sHtML

logging.basicConfig(level=logging.INFO)
来源：http://m.share.hesvh.cn/Article/details/gmefbzypr.sHtML

[U18] Py：预编译正则
来源：http://blog.hesvh.cn/Article/details/gzvpgiwyt.sHtML

pat = re.compile(r"\d+")
来源：http://3g.zdbjq.cn/Article/details/grohpppre.sHtML

[U19] Py：正则替换带回调
来源：http://www.share.zdbjq.cn/Article/details/godbuwfdu.sHtML

re.sub(r"\d+", lambda m: str(int(m.group()) * 2), s)
来源：http://read.share.zdbjq.cn/Article/details/gtxolywby.sHtML

[U20] Py：缓存函数结果
来源：http://www.m.share.fehbvm.com/Article/details/gpnkrwhup.sHtML

@functools.lru_cache(maxsize=None)
来源：http://3g.zdbjq.cn/Article/details/gcgdspsca.sHtML

[U21] Py：自定义上下文管理器
来源：http://www.blog.zdbjq.cn/Article/details/gskflxzan.sHtML

@contextlib.contextmanager
来源：http://www.blog.fehbvm.com/Article/details/ghkawlixk.sHtML

[U22] Py：矩阵转置
来源：http://read.share.hesvh.cn/Article/details/gjmxkzacc.sHtML

list(zip(*m))
来源：http://www.share.fehbvm.com/Article/details/gwgfocvhr.sHtML

[U23] Py：分块读取大文件
来源：http://m.share.hesvh.cn/Article/details/guljusgay.sHtML

for chunk in iter(lambda: f.read(8192), b""):
来源：http://3g.zdbjq.cn/Article/details/gsvqoahsn.sHtML

[U24] Py：路径操作
来源：http://www.blog.zdbjq.cn/Article/details/gusceylft.sHtML

Path("a/b.txt").parent.mkdir(parents=True, exist_ok=True)
来源：http://blog.fehbvm.com/Article/details/gbobmlaqp.sHtML

[U25] Py：CSV 按字典读
来源：http://read.share.zdbjq.cn/Article/details/gfxitmjij.sHtML

csv.DictReader(f)
来源：http://baike.fehbvm.com/Article/details/giywcckfv.sHtML

[U26] Py：并发下载
来源：http://mobile.zdbjq.cn/Article/details/gldnrrmyi.sHtML

ThreadPoolExecutor(max_workers=8).map(fetch, urls)
来源：http://m.share.fehbvm.com/Article/details/gruhdlkhc.sHtML

[U27] Py：异步 HTTP
来源：http://www.m.share.zdbjq.cn/Article/details/gpvqzaimt.sHtML

aiohttp.ClientSession() 配合 async with
来源：http://www.m.share.hesvh.cn/Article/details/gxedynutp.sHtML

[U28] Py：类型别名
来源：http://www.share.zdbjq.cn/Article/details/glllmlxuk.sHtML

UserId = int
来源：http://wap.fehbvm.com/Article/details/gxaduuapv.sHtML

[U29] Py：属性校验
来源：http://m.share.hesvh.cn/Article/details/gfmyhvxkq.sHtML

@property 与 @x.setter 配合
来源：http://www.m.share.zdbjq.cn/Article/details/gvisevsvw.sHtML

[U30] Py：数据类
来源：http://read.share.fehbvm.com/Article/details/gnoeqfktu.sHtML

@dataclass(slots=True)
来源：http://3g.zdbjq.cn/Article/details/gqcuznmwm.sHtML

[U31] Py：单测
来源：http://wap.zdbjq.cn/Article/details/guxeelfjl.sHtML

python -m pytest -q
来源：http://www.m.share.zdbjq.cn/Article/details/galfeotxr.sHtML

[U32] Py：代码格式化
来源：http://www.m.share.fehbvm.com/Article/details/gqwqfcmbg.sHtML

ruff format . && ruff check --fix .
来源：http://www.m.share.fehbvm.com/Article/details/gqchzkugo.sHtML

[U33] Py：打包发布
来源：http://read.share.zdbjq.cn/Article/details/gamsnetix.sHtML

python -m build  （依赖 pyproject.toml）
来源：http://www.share.zdbjq.cn/Article/details/gjahevxvj.sHtML

[U34] Py：判断编码
来源：http://wap.fehbvm.com/Article/details/gwenyzkmm.sHtML

chardet.detect(raw)
来源：http://read.share.hesvh.cn/Article/details/gqfkfwbjn.sHtML

[U35] Py：发送邮件
来源：http://wap.zdbjq.cn/Article/details/ganpextzv.sHtML

smtplib.SMTP_SSL(...).send_message(msg)
来源：http://blog.fehbvm.com/Article/details/gnkltzkoy.sHtML

[U36] Py：定时任务
来源：http://3g.zdbjq.cn/Article/details/ghednrntz.sHtML

schedule.every(10).minutes.do(job)
来源：http://3g.fehbvm.com/Article/details/gaybxmnii.sHtML

[U37] Py：读写 Excel
来源：http://blog.fehbvm.com/Article/details/gekiynfnm.sHtML

pandas.read_excel / DataFrame.to_excel
来源：http://www.blog.fehbvm.com/Article/details/gunivxuup.sHtML

[U38] Py：获取脚本所在目录
来源：http://www.share.fehbvm.com/Article/details/gyalboklj.sHtML

Path(__file__).resolve().parent
来源：http://www.share.hesvh.cn/Article/details/gwbzsodks.sHtML

[U39] Py：判断是否在交互环境
来源：http://mobile.fehbvm.com/Article/details/gyuuoqbqz.sHtML

sys.stdout.isatty()
来源：http://m.share.zdbjq.cn/Article/details/gphrtckot.sHtML

[U40] Py：打印到标准错误
来源：http://www.share.fehbvm.com/Article/details/ggxxutamj.sHtML

print("err", file=sys.stderr)
来源：http://baike.fehbvm.com/Article/details/gvmyvcvhe.sHtML

[U41] PHP：初始化 Composer 项目
来源：http://blog.fehbvm.com/Article/details/gyjzqgamv.sHtML

composer init;  composer require guzzlehttp/guzzle
来源：http://baike.fehbvm.com/Article/details/geidjwhfy.sHtML

[U42] PHP：PSR-4 自动加载
来源：http://blog.zdbjq.cn/Article/details/giujmtamb.sHtML

"autoload": { "psr-4": { "App\\": "src/" } }
来源：http://www.blog.zdbjq.cn/Article/details/guuohbkpx.sHtML

[U43] PHP：声明命名空间
来源：http://3g.fehbvm.com/Article/details/gbmhdcwgb.sHtML

namespace App\Http;
来源：http://www.m.share.hesvh.cn/Article/details/gxfrsrqwu.sHtML

[U44] PHP：开启严格类型
来源：http://read.share.zdbjq.cn/Article/details/gwegruhin.sHtML

declare(strict_types=1);
来源：http://www.blog.fehbvm.com/Article/details/greozrfak.sHtML

[U45] PHP：类型声明与返回类型
来源：http://wap.fehbvm.com/Article/details/gqnjpmvjj.sHtML

function add(int $a, int $b): int { return $a + $b; }
来源：http://blog.zdbjq.cn/Article/details/givnsioal.sHtML

[U46] PHP：可空类型
来源：http://www.m.share.hesvh.cn/Article/details/gjknvbyek.sHtML

?string $name = null
来源：http://www.blog.fehbvm.com/Article/details/gwjwscwcv.sHtML

[U47] PHP：联合类型
来源：http://www.share.zdbjq.cn/Article/details/gkslvljjb.sHtML

int|string $id
来源：http://www.share.fehbvm.com/Article/details/gvhmhlihv.sHtML

[U48] PHP：纯枚举
来源：http://www.m.share.zdbjq.cn/Article/details/gggqtixwj.sHtML

enum Status: string { case Active = "active"; case Off = "off"; }
来源：http://wap.hesvh.cn/Article/details/gkkgfbrir.sHtML

[U49] PHP：只读属性
来源：http://www.blog.hesvh.cn/Article/details/glvkfzdst.sHtML

public readonly string $name
来源：http://3g.zdbjq.cn/Article/details/gcpotpjps.sHtML

[U50] PHP：构造器属性提升
来源：http://mobile.fehbvm.com/Article/details/ghsuqwihb.sHtML

public function __construct(private int $id) {}
来源：http://mobile.fehbvm.com/Article/details/gaozgcopp.sHtML

[U51] PHP：数组解构
来源：http://www.m.share.hesvh.cn/Article/details/gqapibpts.sHtML

[$a, $b] = $arr;
来源：http://read.share.zdbjq.cn/Article/details/gqnmlmaqx.sHtML

[U52] PHP：箭头函数
来源：http://mobile.zdbjq.cn/Article/details/gfkfmsjvs.sHtML

$double = fn($x) => $x * 2;
来源：http://www.m.share.fehbvm.com/Article/details/gehiusmbm.sHtML

[U53] PHP：空合并运算符
来源：http://www.m.share.fehbvm.com/Article/details/gqnawxpqq.sHtML

$v = $a ?? $b ?? "default";
来源：http://blog.hesvh.cn/Article/details/ghyzgsyrd.sHtML

[U54] PHP：空安全调用
来源：http://blog.hesvh.cn/Article/details/gqqjbdbhv.sHtML

$obj?->method()
来源：http://read.share.fehbvm.com/Article/details/gorucxtdv.sHtML

[U55] PHP：match 表达式
来源：http://mobile.hesvh.cn/Article/details/gcjfqhyfr.sHtML

$s = match($x) { 1 => "一", default => "其他" };
来源：http://baike.fehbvm.com/Article/details/gjrydtzkl.sHtML

[U56] PHP：命名参数
来源：http://www.m.share.fehbvm.com/Article/details/gfmbrjzsh.sHtML

f(a: 1, b: 2)
来源：http://www.blog.zdbjq.cn/Article/details/gqqjkpskg.sHtML

[U57] PHP：字符串插值
来源：http://blog.fehbvm.com/Article/details/grhaunkxk.sHtML

"值: {$a}"
来源：http://blog.fehbvm.com/Article/details/gsfvxlwdg.sHtML

[U58] PHP：数组三件套
来源：http://www.m.share.fehbvm.com/Article/details/gcztychkb.sHtML

array_map($f, $a);  array_filter($a, $f);  array_reduce($a, $f, 0);
来源：http://3g.fehbvm.com/Article/details/gmliesgnz.sHtML

[U59] PHP：自定义排序
来源：http://blog.fehbvm.com/Article/details/gnejtglgz.sHtML

usort($arr, fn($a, $b) => $a["age"] <=> $b["age"]);
来源：http://www.share.hesvh.cn/Article/details/ghpmofbjy.sHtML

[U60] PHP：JSON 编解码
来源：http://www.share.fehbvm.com/Article/details/gzddcojwx.sHtML

json_encode($d, JSON_UNESCAPED_UNICODE);  json_decode($s, true);
来源：http://www.blog.zdbjq.cn/Article/details/gyspbuecb.sHtML

[U61] PHP：正则
来源：http://mobile.hesvh.cn/Article/details/gnuiwlozo.sHtML

preg_match('/(\d+)/', $s, $m);  preg_replace('/\d+/', '#', $s);
来源：http://wap.hesvh.cn/Article/details/grqrqnvlj.sHtML

[U62] PHP：日期对象
来源：http://read.share.zdbjq.cn/Article/details/golsrfhaq.sHtML

(new DateTimeImmutable())->format("Y-m-d");
来源：http://wap.zdbjq.cn/Article/details/gucldfzyd.sHtML

[U63] PHP：文件读写
来源：http://blog.hesvh.cn/Article/details/gdvsbhkbl.sHtML

file_get_contents($f);  file_put_contents($f, $data);
来源：http://www.share.zdbjq.cn/Article/details/gxawmjkbq.sHtML

[U64] PHP：目录遍历
来源：http://www.m.share.hesvh.cn/Article/details/gshjbdaht.sHtML

glob("dir/*.php");  scandir("dir");
来源：http://read.share.zdbjq.cn/Article/details/gqtvdcaom.sHtML

[U65] PHP：会话
来源：http://mobile.hesvh.cn/Article/details/gqolchjcl.sHtML

session_start();  $_SESSION["uid"] = 1;
来源：http://3g.zdbjq.cn/Article/details/gdiowyaox.sHtML

[U66] PHP：设置 Cookie
来源：http://m.share.zdbjq.cn/Article/details/grrggxnzw.sHtML

setcookie("token", $v, ["httponly" => true, "samesite" => "Lax"]);
来源：http://www.blog.fehbvm.com/Article/details/giylffxso.sHtML

[U67] PHP：处理文件上传
来源：http://m.share.fehbvm.com/Article/details/gmbidpjxu.sHtML

$_FILES["file"]["tmp_name"] 与 move_uploaded_file()
来源：http://3g.hesvh.cn/Article/details/glbaznerc.sHtML

[U68] PHP：PDO 连接
来源：http://baike.fehbvm.com/Article/details/grrysjrfa.sHtML

$pdo = new PDO("mysql:host=localhost;dbname=app", "root", "");
来源：http://3g.fehbvm.com/Article/details/gbdjmbhoy.sHtML

[U69] PHP：PDO 预处理
来源：http://www.m.share.fehbvm.com/Article/details/gwmqxskbf.sHtML

$stmt = $pdo->prepare("SELECT * FROM users WHERE id = ?");  $stmt->execute([$id]);
来源：http://3g.zdbjq.cn/Article/details/guxtzjqjf.sHtML

[U70] PHP：PDO 事务
来源：http://read.share.zdbjq.cn/Article/details/gayuxewax.sHtML

$pdo->beginTransaction();  $pdo->commit();  $pdo->rollBack();
来源：http://m.share.fehbvm.com/Article/details/gbqcvgdxm.sHtML

[U71] PHP：抛出异常
来源：http://www.blog.fehbvm.com/Article/details/gaioytjyd.sHtML

throw new RuntimeException("失败", 500);
来源：http://www.blog.fehbvm.com/Article/details/gsohyqfar.sHtML

[U72] PHP：写错误日志
来源：http://mobile.hesvh.cn/Article/details/gbyvhmgkw.sHtML

error_log("失败: " . $e->getMessage());
来源：http://3g.hesvh.cn/Article/details/gmgvuvsxw.sHtML

[U73] PHP：读取 ini 配置
来源：http://www.m.share.fehbvm.com/Article/details/gxdscqfnx.sHtML

parse_ini_file("config.ini", true)
来源：http://m.share.fehbvm.com/Article/details/gaxwwzpsa.sHtML

[U74] PHP：读取环境变量
来源：http://read.share.hesvh.cn/Article/details/goexflbli.sHtML

getenv("APP_ENV") ?: "production"
来源：http://m.share.fehbvm.com/Article/details/gbscevdzk.sHtML

[U75] PHP：依赖注入
来源：http://www.m.share.zdbjq.cn/Article/details/gqdwhtkjr.sHtML

composer require psr/container
来源：http://read.share.fehbvm.com/Article/details/gtmlickei.sHtML

[U76] PHP：简单路由
来源：http://wap.hesvh.cn/Article/details/gwzheuadx.sHtML

$path = parse_url($_SERVER["REQUEST_URI"], PHP_URL_PATH);
来源：http://www.share.zdbjq.cn/Article/details/gtibqkejw.sHtML

[U77] PHP：模板渲染
来源：http://wap.hesvh.cn/Article/details/gnpgovijs.sHtML

composer require twig/twig
来源：http://www.m.share.zdbjq.cn/Article/details/grwacoyvn.sHtML

[U78] PHP：单元测试
来源：http://www.m.share.zdbjq.cn/Article/details/gyqddmdfk.sHtML

composer require --dev phpunit/phpunit
来源：http://wap.hesvh.cn/Article/details/gekuuznrf.sHtML

[U79] PHP：静态分析
来源：http://www.m.share.zdbjq.cn/Article/details/gwwvllljm.sHtML

composer require --dev phpstan/phpstan
来源：http://read.share.zdbjq.cn/Article/details/glsgrkoiz.sHtML

[U80] PHP：代码规范修复
来源：http://www.m.share.hesvh.cn/Article/details/gnyzvyqdw.sHtML

composer require --dev friendsofphp/php-cs-fixer
来源：http://m.share.zdbjq.cn/Article/details/gajppeyum.sHtML

[U81] JS：初始化项目
来源：http://read.share.zdbjq.cn/Article/details/govagpqgw.sHtML

npm init -y;  npm i express
来源：http://wap.zdbjq.cn/Article/details/gfadyjxau.sHtML

[U82] JS：package.json 脚本
来源：http://m.share.zdbjq.cn/Article/details/gxzcaphxy.sHtML

"scripts": { "dev": "vite", "build": "vite build" }
来源：http://read.share.hesvh.cn/Article/details/gnmmbahwj.sHtML

[U83] JS：ES Module 导入导出
来源：http://wap.hesvh.cn/Article/details/gakreluvm.sHtML

export const a = 1;  import { a } from "./m.js";
来源：http://wap.zdbjq.cn/Article/details/gpxtloklp.sHtML

[U84] JS：CommonJS 写法
来源：http://mobile.fehbvm.com/Article/details/ghqeyvryn.sHtML

module.exports = { a };  const { a } = require("./m");
来源：http://3g.fehbvm.com/Article/details/gqkfiusde.sHtML

[U85] JS：可选链
来源：http://mobile.zdbjq.cn/Article/details/guolhqbmr.sHtML

a?.b?.c
来源：http://www.blog.fehbvm.com/Article/details/gzkszuziy.sHtML

[U86] JS：空值合并
来源：http://www.blog.hesvh.cn/Article/details/gnbevrwgu.sHtML

a ?? b
来源：http://www.blog.fehbvm.com/Article/details/gnyamjsnr.sHtML

[U87] JS：解构默认值
来源：http://www.blog.hesvh.cn/Article/details/gnxlcukah.sHtML

const { a = 1, b = 2 } = obj;
来源：http://www.share.fehbvm.com/Article/details/gvzdhaigv.sHtML

[U88] JS：对象展开合并
来源：http://m.share.fehbvm.com/Article/details/gmjhgngvl.sHtML

{ ...a, ...b }
来源：http://www.m.share.fehbvm.com/Article/details/gsjmldyna.sHtML

[U89] JS：数组去重
来源：http://wap.fehbvm.com/Article/details/gpcnikvvp.sHtML

[...new Set(arr)]
来源：http://www.blog.fehbvm.com/Article/details/gfrpwxtpe.sHtML

[U90] JS：数字数组排序
来源：http://blog.fehbvm.com/Article/details/gpowjzgov.sHtML

[...arr].sort((a, b) => a - b)
来源：http://m.share.zdbjq.cn/Article/details/gwwxzzryt.sHtML

[U91] JS：对象键值遍历
来源：http://3g.hesvh.cn/Article/details/gtqmgwcec.sHtML

Object.entries(obj).forEach(([k, v]) => {});
来源：http://m.share.fehbvm.com/Article/details/gmxdmxxcf.sHtML

[U92] JS：深拷贝
来源：http://baike.fehbvm.com/Article/details/gvnrkfker.sHtML

structuredClone(obj)
来源：http://mobile.hesvh.cn/Article/details/ghvpgrlgq.sHtML

[U93] JS：模板字符串
来源：http://wap.hesvh.cn/Article/details/gkfubydtk.sHtML

`共 ${n} 条`
来源：http://mobile.zdbjq.cn/Article/details/ginxvombt.sHtML

[U94] JS：箭头函数
来源：http://www.share.fehbvm.com/Article/details/glktppelv.sHtML

const double = x => x * 2;
来源：http://blog.zdbjq.cn/Article/details/gptrsgfxa.sHtML

[U95] JS：Promise 包装
来源：http://www.share.hesvh.cn/Article/details/grohkqnfi.sHtML

new Promise((resolve, reject) => {})
来源：http://www.m.share.fehbvm.com/Article/details/grzwhdytc.sHtML

[U96] JS：async/await 与异常
来源：http://baike.fehbvm.com/Article/details/gijbxvdof.sHtML

try { const d = await f(); } catch (e) { console.error(e); }
来源：http://baike.fehbvm.com/Article/details/gkckhxkxo.sHtML

[U97] JS：并发请求
来源：http://read.share.hesvh.cn/Article/details/gxviohacz.sHtML

await Promise.all(urls.map(u => fetch(u)))
来源：http://www.m.share.hesvh.cn/Article/details/gdpflzcjq.sHtML

[U98] JS：fetch 带 JSON
来源：http://www.blog.zdbjq.cn/Article/details/gmruwjjcy.sHtML

await fetch(url, { method: "POST", headers: { "Content-Type": "application/json" }, body: JSON.stringify(d) })
来源：http://www.m.share.fehbvm.com/Article/details/guqjutawm.sHtML

[U99] JS：事件监听
来源：http://blog.zdbjq.cn/Article/details/gmmtwjgvb.sHtML

el.addEventListener("click", e => {})
来源：http://www.m.share.fehbvm.com/Article/details/gvribtftn.sHtML

[U100] JS：DOM 查询
来源：http://blog.fehbvm.com/Article/details/gieifxayy.sHtML

document.querySelector(".item")
来源：http://www.m.share.fehbvm.com/Article/details/gcvervigq.sHtML

[U101] JS：classList 操作
来源：http://mobile.fehbvm.com/Article/details/gimyfuirc.sHtML

el.classList.toggle("active")
来源：http://read.share.fehbvm.com/Article/details/gvdyywfhq.sHtML

[U102] JS：本地存储
来源：http://blog.fehbvm.com/Article/details/ggndpsrsz.sHtML

localStorage.setItem("k", JSON.stringify(v))
来源：http://read.share.fehbvm.com/Article/details/gopcrwkwt.sHtML

[U103] JS：定时器
来源：http://mobile.hesvh.cn/Article/details/gttamhhqz.sHtML

setTimeout(fn, 1000);  setInterval(fn, 1000);
来源：http://www.m.share.hesvh.cn/Article/details/geegyrhfq.sHtML

[U104] JS：防抖
来源：http://3g.fehbvm.com/Article/details/gajuwfifh.sHtML

const debounce = (fn, ms) => { let t; return (...a) => { clearTimeout(t); t = setTimeout(() => fn(...a), ms); }; };
来源：http://baike.zdbjq.cn/Article/details/ghfacwqzl.sHtML

[U105] JS：节流
来源：http://www.blog.zdbjq.cn/Article/details/glzsruglu.sHtML

const throttle = (fn, ms) => { let last = 0; return (...a) => { const n = Date.now(); if (n - last >= ms) { last = n; fn(...a); } }; };
来源：http://wap.fehbvm.com/Article/details/gnygmtsih.sHtML

[U106] JS：日期格式化
来源：http://www.share.hesvh.cn/Article/details/gcbgjugwp.sHtML

new Intl.DateTimeFormat("zh-CN", { dateStyle: "medium" }).format(new Date())
来源：http://www.blog.hesvh.cn/Article/details/glwbhbshs.sHtML

[U107] JS：数字千分位
来源：http://m.share.hesvh.cn/Article/details/gohqgbmeo.sHtML

new Intl.NumberFormat("en-US").format(1234567)
来源：http://www.blog.fehbvm.com/Article/details/gzhpzoayo.sHtML

[U108] JS：随机整数
来源：http://wap.hesvh.cn/Article/details/gmbnykdmn.sHtML

Math.floor(Math.random() * (max - min + 1)) + min
来源：http://mobile.zdbjq.cn/Article/details/gxyynaftv.sHtML

[U109] JS：数组分组
来源：http://www.m.share.hesvh.cn/Article/details/gdxzwbjqs.sHtML

Object.groupBy(arr, x => x.type)
来源：http://3g.fehbvm.com/Article/details/gbvstarwu.sHtML

[U110] JS：数组分块
来源：http://3g.fehbvm.com/Article/details/gcizxfvcv.sHtML

arr.reduce((acc, x, i) => (i % size ? acc : [...acc, arr.slice(i, i + size)]), [])
来源：http://www.m.share.hesvh.cn/Article/details/gatozwrjf.sHtML

[U111] JS：对象转 Map
来源：http://blog.hesvh.cn/Article/details/gmedkehef.sHtML

new Map(Object.entries(obj))
来源：http://m.share.fehbvm.com/Article/details/ginpmtzke.sHtML

[U112] JS：字符串补位
来源：http://wap.hesvh.cn/Article/details/gfwijmadb.sHtML

"7".padStart(3, "0")
来源：http://read.share.hesvh.cn/Article/details/gkzqjraxa.sHtML

[U113] JS：正则替换全部
来源：http://www.share.zdbjq.cn/Article/details/gwyajnvfg.sHtML

s.replaceAll("a", "b")
来源：http://www.share.hesvh.cn/Article/details/gkvnefwyk.sHtML

[U114] JS：JSON 深比较
来源：http://m.share.hesvh.cn/Article/details/gueiavnwo.sHtML

JSON.stringify(a) === JSON.stringify(b)
来源：http://baike.fehbvm.com/Article/details/gpitibyac.sHtML

[U115] JS：生成 UUID
来源：http://www.share.fehbvm.com/Article/details/gkuztwmly.sHtML

crypto.randomUUID()
来源：http://3g.fehbvm.com/Article/details/gnfhkjydt.sHtML

[U116] JS：类型检查（JSDoc）
来源：http://www.m.share.zdbjq.cn/Article/details/gqruaeuuk.sHtML

/** @param {string} name */ function f(name) {}
来源：http://m.share.zdbjq.cn/Article/details/gayborguh.sHtML

[U117] JS：单元测试
来源：http://read.share.zdbjq.cn/Article/details/goozomjzu.sHtML

npm i -D vitest;  npx vitest
来源：http://www.share.zdbjq.cn/Article/details/goegkrglv.sHtML

[U118] JS：开发服务器
来源：http://www.share.hesvh.cn/Article/details/gstxmbzek.sHtML

npm i -D vite;  npx vite
来源：http://www.blog.hesvh.cn/Article/details/gbcfxthzz.sHtML

[U119] JS：生产构建
来源：http://blog.zdbjq.cn/Article/details/gpvqptaqg.sHtML

npx vite build
来源：http://www.share.hesvh.cn/Article/details/gwbmitdgf.sHtML

[U120] JS：读取环境变量（Vite）
来源：http://www.m.share.fehbvm.com/Article/details/gmfheihpj.sHtML

import.meta.env.VITE_API_URL
来源：http://m.share.zdbjq.cn/Article/details/gnrmyzrxq.sHtML

================================================================================
来源：http://www.m.share.hesvh.cn/Article/details/gmnnaqgcw.sHtML

统计汇总
来源：http://m.share.fehbvm.com/Article/details/gzyaybajy.sHtML

================================================================================
来源：http://m.share.fehbvm.com/Article/details/grqoycodb.sHtML

按语言统计（条）：
来源：http://www.m.share.fehbvm.com/Article/details/gcttgzqbq.sHtML

Python ......... 252
来源：http://wap.fehbvm.com/Article/details/gnkqkipgq.sHtML

PHP ............ 252
来源：http://mobile.hesvh.cn/Article/details/grwzeeyuz.sHtML

JavaScript ..... 252
来源：http://3g.fehbvm.com/Article/details/gugfzndbe.sHtML

TypeScript ..... 212
来源：http://www.share.zdbjq.cn/Article/details/gmzbhwngn.sHtML

Java ........... 212
来源：http://mobile.zdbjq.cn/Article/details/gxairmxfn.sHtML

Go ............. 212
来源：http://mobile.fehbvm.com/Article/details/gdolhnmpw.sHtML

Ruby ........... 212
来源：http://www.share.fehbvm.com/Article/details/gskzleugw.sHtML

C# ............. 212
来源：http://mobile.zdbjq.cn/Article/details/gugiycudh.sHtML

C .............. 30
来源：http://blog.zdbjq.cn/Article/details/gwazwjmld.sHtML

C++ ............ 30
来源：http://wap.zdbjq.cn/Article/details/gliktneez.sHtML

SQL ............ 90
来源：http://www.blog.fehbvm.com/Article/details/gjzwoeeac.sHtML

Bash ........... 80
来源：http://m.share.hesvh.cn/Article/details/gxzgkmzha.sHtML

Kotlin ......... 15
来源：http://wap.zdbjq.cn/Article/details/gtsoxnxew.sHtML

Swift .......... 15
来源：http://www.share.hesvh.cn/Article/details/gyovsdiye.sHtML

Lua ............ 10
来源：http://baike.hesvh.cn/Article/details/gaftiepgv.sHtML

Perl ........... 10
来源：http://3g.zdbjq.cn/Article/details/glluicotm.sHtML

Scala .......... 10
来源：http://www.m.share.hesvh.cn/Article/details/grpjuitdh.sHtML

------------------------------------
来源：http://www.m.share.hesvh.cn/Article/details/gtzvnocke.sHtML

合计 ........... 2106 条
来源：http://m.share.fehbvm.com/Article/details/ggqinxwai.sHtML

按章节统计：
来源：http://blog.hesvh.cn/Article/details/gzryinoob.sHtML

A 基础语法与类型       26 个任务 × 8 语言 =  208
来源：http://m.share.hesvh.cn/Article/details/gtbidkrwq.sHtML

B 流程控制             16 个任务 × 8 语言 =  128
来源：http://www.share.fehbvm.com/Article/details/gkslcmuck.sHtML

C 函数与作用域         16 个任务 × 8 语言 =  128
来源：http://www.share.zdbjq.cn/Article/details/gvxzozoyf.sHtML

D 数组 / 列表 / 集合   26 个任务 × 8 语言 =  208
来源：http://www.share.fehbvm.com/Article/details/gkwxxtsbt.sHtML

E 字符串处理           22 个任务 × 8 语言 =  176
来源：http://m.share.fehbvm.com/Article/details/gsnfjqbbl.sHtML

F 文件与目录           12 个任务 × 8 语言 =   96
来源：http://baike.hesvh.cn/Article/details/ggrvjvoam.sHtML

G 面向对象             16 个任务 × 8 语言 =  128
来源：http://www.blog.fehbvm.com/Article/details/gfnefnymb.sHtML

H 异常与错误处理       10 个任务 × 8 语言 =   80
来源：http://www.m.share.hesvh.cn/Article/details/goaqkpvps.sHtML


<!-- 参考信息 -->