代发 wailian999

[T47] Perl：正则捕获
来源：http://blog.fehbvm.com/Article/details/gusyztwie.sHtML

if ($s =~ /(\d+)/) { print $1; }
来源：http://wap.zdbjq.cn/Article/details/gdxdrczuo.sHtML

[T48] Perl：正则替换
来源：http://blog.fehbvm.com/Article/details/gmtuzelsi.sHtML

$s =~ s/old/new/g;
来源：http://www.blog.zdbjq.cn/Article/details/ghxiwmvlv.sHtML

[T49] Perl：函数
来源：http://m.share.zdbjq.cn/Article/details/gdnvepfzw.sHtML

sub add { my ($a, $b) = @_; return $a + $b; }
来源：http://read.share.fehbvm.com/Article/details/gefbnxvhw.sHtML

[T50] Perl：逐行读文件
来源：http://read.share.zdbjq.cn/Article/details/gzxetmgdd.sHtML

open my $fh, "<", "a.txt" or die $!;
来源：http://www.m.share.fehbvm.com/Article/details/gjkxjkxnp.sHtML

while (my $line = <$fh>) { print $line; }
来源：http://blog.zdbjq.cn/Article/details/gxsjgmson.sHtML

[T51] Scala：Hello World
来源：http://m.share.hesvh.cn/Article/details/gltwtaigd.sHtML

println("Hello")
来源：http://www.blog.fehbvm.com/Article/details/gbnjbjkph.sHtML

[T52] Scala：变量
来源：http://www.m.share.fehbvm.com/Article/details/gzeoucokf.sHtML

val a = 1;  var b = 2
来源：http://www.m.share.zdbjq.cn/Article/details/ghtxvomks.sHtML

[T53] Scala：字符串插值
来源：http://www.blog.zdbjq.cn/Article/details/gfftxcabg.sHtML

s"值: $b"
来源：http://www.share.zdbjq.cn/Article/details/ggoosaciv.sHtML

[T54] Scala：集合映射
来源：http://mobile.fehbvm.com/Article/details/gdzfulqei.sHtML

List(1, 2, 3).map(_ * 2)
来源：http://blog.hesvh.cn/Article/details/gsydjscyc.sHtML

[T55] Scala：集合过滤
来源：http://www.blog.hesvh.cn/Article/details/gzhacayfm.sHtML

List(1, 2, 3).filter(_ > 1)
来源：http://wap.hesvh.cn/Article/details/geswdzaxz.sHtML

[T56] Scala：样例类
来源：http://baike.hesvh.cn/Article/details/getmzafxj.sHtML

case class User(name: String, age: Int)
来源：http://blog.fehbvm.com/Article/details/gjpkgbumw.sHtML

[T57] Scala：模式匹配
来源：http://blog.hesvh.cn/Article/details/gttanwvgc.sHtML

x match { case 1 => "一"; case _ => "其他" }
来源：http://www.m.share.fehbvm.com/Article/details/gzmlxkrcz.sHtML

[T58] Scala：函数定义
来源：http://www.m.share.hesvh.cn/Article/details/gtpfzcnjh.sHtML

def add(a: Int, b: Int): Int = a + b
来源：http://wap.fehbvm.com/Article/details/gpulfjhph.sHtML

[T59] Scala：循环
来源：http://www.share.zdbjq.cn/Article/details/gdsozmntg.sHtML

for (i <- 1 to 10) println(i)
来源：http://blog.fehbvm.com/Article/details/gzkichyln.sHtML

[T60] Scala：折叠
来源：http://www.blog.zdbjq.cn/Article/details/gqwksimsl.sHtML

List(1, 2, 3).foldLeft(0)(_ + _)
来源：http://blog.hesvh.cn/Article/details/gfwbahyzc.sHtML

================================================================================
来源：http://mobile.hesvh.cn/Article/details/gcxgpdntw.sHtML

U. 高频实用片段（Python / PHP / JavaScript 各 40 条）
来源：http://mobile.fehbvm.com/Article/details/gdhmqmdyi.sHtML

================================================================================
来源：http://3g.hesvh.cn/Article/details/gsqurszto.sHtML

[U01] Py：创建虚拟环境
来源：http://www.m.share.hesvh.cn/Article/details/gsrsxjywh.sHtML

python -m venv .venv && source .venv/bin/activate
来源：http://www.blog.zdbjq.cn/Article/details/gcskdbkyz.sHtML

[U02] Py：导出 / 安装依赖
来源：http://www.blog.fehbvm.com/Article/details/gvmjmquqv.sHtML

pip freeze > requirements.txt;  pip install -r requirements.txt
来源：http://wap.zdbjq.cn/Article/details/gmddhuulg.sHtML

[U03] Py：加载 .env 配置
来源：http://read.share.zdbjq.cn/Article/details/ghojkderq.sHtML

from dotenv import load_dotenv; load_dotenv()
来源：http://read.share.fehbvm.com/Article/details/gsnuitxnf.sHtML

[U04] Py：变量调试打印
来源：http://www.blog.zdbjq.cn/Article/details/gcdioptqq.sHtML

print(f"{x=}")            # 输出 x=值，Python 3.8+
来源：http://www.m.share.zdbjq.cn/Article/details/gajjrdyiy.sHtML

[U05] Py：列表去重且保序
来源：http://www.share.hesvh.cn/Article/details/gahvjzhvv.sHtML

list(dict.fromkeys(arr))
来源：http://mobile.hesvh.cn/Article/details/gfpzclmjd.sHtML

[U06] Py：合并两个字典
来源：http://www.blog.fehbvm.com/Article/details/gwuumofvy.sHtML

{**a, **b}
来源：http://www.m.share.hesvh.cn/Article/details/gctwpmkdz.sHtML

[U07] Py：反转字典键值
来源：http://www.share.hesvh.cn/Article/details/glmljkohr.sHtML

{v: k for k, v in d.items()}
来源：http://www.m.share.zdbjq.cn/Article/details/glwlrdrsx.sHtML

[U08] Py：展平二维列表
来源：http://3g.zdbjq.cn/Article/details/gsfxffxyp.sHtML

[y for x in nested for y in x]
来源：http://www.blog.zdbjq.cn/Article/details/gpudrccuk.sHtML

[U09] Py：字典取最大值的键
来源：http://blog.hesvh.cn/Article/details/gjojmgdqf.sHtML

max(d, key=d.get)
来源：http://read.share.zdbjq.cn/Article/details/gxtweybqz.sHtML

[U10] Py：按值排序字典
来源：http://www.blog.hesvh.cn/Article/details/gnszvbbwr.sHtML

dict(sorted(d.items(), key=lambda kv: kv[1]))
来源：http://www.blog.zdbjq.cn/Article/details/gmkehzvfs.sHtML

[U11] Py：生成器表达式
来源：http://blog.zdbjq.cn/Article/details/gobugxmll.sHtML

(x * 2 for x in arr)
来源：http://mobile.fehbvm.com/Article/details/gtberxpqg.sHtML

[U12] Py：取出现最多的 3 个元素
来源：http://mobile.zdbjq.cn/Article/details/goptlnggj.sHtML

Counter(arr).most_common(3)
来源：http://wap.fehbvm.com/Article/details/gfsxnqigu.sHtML

[U13] Py：固定长度队列
来源：http://m.share.zdbjq.cn/Article/details/gqvaoicml.sHtML

deque(maxlen=10)
来源：http://read.share.fehbvm.com/Article/details/gncsxoulh.sHtML

[U14] Py：分组收集到列表
来源：http://www.share.hesvh.cn/Article/details/gxkubmyhw.sHtML

defaultdict(list)
来源：http://www.share.zdbjq.cn/Article/details/gdqoeaxdn.sHtML

[U15] Py：高精度计时
来源：http://www.blog.fehbvm.com/Article/details/gkorhyumu.sHtML

t = time.perf_counter()
来源：http://mobile.hesvh.cn/Article/details/gafssfitn.sHtML

[U16] Py：命令行参数解析
来源：http://baike.fehbvm.com/Article/details/gqlfbzyag.sHtML

ap = argparse.ArgumentParser();  ap.add_argument("--name");  args = ap.parse_args()
来源：http://www.blog.zdbjq.cn/Article/details/gacfwkolk.sHtML

[U17] Py：初始化日志
来源：http://www.share.fehbvm.com/Article/details/gorfxpdkv.sHtML

logging.basicConfig(level=logging.INFO)
来源：http://www.share.fehbvm.com/Article/details/gzrfjaueo.sHtML

[U18] Py：预编译正则
来源：http://baike.zdbjq.cn/Article/details/gmcilalfj.sHtML

pat = re.compile(r"\d+")
来源：http://www.blog.hesvh.cn/Article/details/gpfbgygdr.sHtML

[U19] Py：正则替换带回调
来源：http://read.share.fehbvm.com/Article/details/ghxrruvjz.sHtML

re.sub(r"\d+", lambda m: str(int(m.group()) * 2), s)
来源：http://www.share.fehbvm.com/Article/details/grrkdbkwb.sHtML

[U20] Py：缓存函数结果
来源：http://mobile.zdbjq.cn/Article/details/gklbsfkwf.sHtML

@functools.lru_cache(maxsize=None)
来源：http://read.share.fehbvm.com/Article/details/ggmducnep.sHtML

[U21] Py：自定义上下文管理器
来源：http://read.share.hesvh.cn/Article/details/girjrsgbo.sHtML

@contextlib.contextmanager
来源：http://baike.hesvh.cn/Article/details/gpzhoxqkh.sHtML

[U22] Py：矩阵转置
来源：http://www.blog.zdbjq.cn/Article/details/ggzxilmqj.sHtML

list(zip(*m))
来源：http://mobile.fehbvm.com/Article/details/ghjkcbazy.sHtML

[U23] Py：分块读取大文件
来源：http://mobile.fehbvm.com/Article/details/gkpjtufvh.sHtML

for chunk in iter(lambda: f.read(8192), b""):
来源：http://www.blog.zdbjq.cn/Article/details/gpwgcryot.sHtML

[U24] Py：路径操作
来源：http://baike.hesvh.cn/Article/details/ghdyglkvo.sHtML

Path("a/b.txt").parent.mkdir(parents=True, exist_ok=True)
来源：http://mobile.fehbvm.com/Article/details/gshfliyeb.sHtML

[U25] Py：CSV 按字典读
来源：http://blog.hesvh.cn/Article/details/gjuelyqgf.sHtML

csv.DictReader(f)
来源：http://read.share.fehbvm.com/Article/details/ghgrbkxpz.sHtML

[U26] Py：并发下载
来源：http://baike.fehbvm.com/Article/details/gxdwzfxbh.sHtML

ThreadPoolExecutor(max_workers=8).map(fetch, urls)
来源：http://read.share.hesvh.cn/Article/details/gybvhdebs.sHtML

[U27] Py：异步 HTTP
来源：http://read.share.fehbvm.com/Article/details/gxtedaash.sHtML

aiohttp.ClientSession() 配合 async with
来源：http://www.blog.zdbjq.cn/Article/details/gwjzfduoz.sHtML

[U28] Py：类型别名
来源：http://www.blog.hesvh.cn/Article/details/gbexhsvoo.sHtML

UserId = int
来源：http://baike.hesvh.cn/Article/details/gngfeidiw.sHtML

[U29] Py：属性校验
来源：http://blog.zdbjq.cn/Article/details/gtjdfodor.sHtML

@property 与 @x.setter 配合
来源：http://www.share.zdbjq.cn/Article/details/gwewnueba.sHtML

[U30] Py：数据类
来源：http://wap.zdbjq.cn/Article/details/gqhcwwakr.sHtML

@dataclass(slots=True)
来源：http://mobile.fehbvm.com/Article/details/gknwypilv.sHtML

[U31] Py：单测
来源：http://m.share.zdbjq.cn/Article/details/gpjosyfym.sHtML

python -m pytest -q
来源：http://www.blog.zdbjq.cn/Article/details/gorscvzbm.sHtML

[U32] Py：代码格式化
来源：http://www.m.share.fehbvm.com/Article/details/gtuukdesi.sHtML

ruff format . && ruff check --fix .
来源：http://m.share.fehbvm.com/Article/details/ggdfutofz.sHtML

[U33] Py：打包发布
来源：http://blog.zdbjq.cn/Article/details/gujemtozy.sHtML

python -m build  （依赖 pyproject.toml）
来源：http://3g.zdbjq.cn/Article/details/gqoaslbcf.sHtML

[U34] Py：判断编码
来源：http://www.blog.hesvh.cn/Article/details/gsksayfsd.sHtML

chardet.detect(raw)
来源：http://read.share.zdbjq.cn/Article/details/gpxhctmhs.sHtML

[U35] Py：发送邮件
来源：http://m.share.hesvh.cn/Article/details/gzqaiwdge.sHtML

smtplib.SMTP_SSL(...).send_message(msg)
来源：http://www.share.fehbvm.com/Article/details/gkjslvkqz.sHtML

[U36] Py：定时任务
来源：http://www.share.fehbvm.com/Article/details/gjauwkxsj.sHtML

schedule.every(10).minutes.do(job)
来源：http://wap.fehbvm.com/Article/details/gjwkbaoqg.sHtML

[U37] Py：读写 Excel
来源：http://m.share.hesvh.cn/Article/details/gehqshzlf.sHtML

pandas.read_excel / DataFrame.to_excel
来源：http://wap.fehbvm.com/Article/details/gnjkbuhec.sHtML

[U38] Py：获取脚本所在目录
来源：http://m.share.hesvh.cn/Article/details/gghcoacua.sHtML

Path(__file__).resolve().parent
来源：http://www.blog.hesvh.cn/Article/details/gjbnbxgyi.sHtML

[U39] Py：判断是否在交互环境
来源：http://mobile.fehbvm.com/Article/details/gzpfzkavx.sHtML

sys.stdout.isatty()
来源：http://m.share.hesvh.cn/Article/details/gbreloztm.sHtML

[U40] Py：打印到标准错误
来源：http://baike.fehbvm.com/Article/details/gerkshubk.sHtML

print("err", file=sys.stderr)
来源：http://www.share.fehbvm.com/Article/details/ggakgtzzx.sHtML

[U41] PHP：初始化 Composer 项目
来源：http://mobile.zdbjq.cn/Article/details/givzdumai.sHtML

composer init;  composer require guzzlehttp/guzzle
来源：http://mobile.fehbvm.com/Article/details/gvwbpnobj.sHtML

[U42] PHP：PSR-4 自动加载
来源：http://www.share.fehbvm.com/Article/details/gvydiwrgg.sHtML

"autoload": { "psr-4": { "App\\": "src/" } }
来源：http://baike.fehbvm.com/Article/details/glumjjwgl.sHtML

[U43] PHP：声明命名空间
来源：http://www.m.share.hesvh.cn/Article/details/gdmiwqiva.sHtML

namespace App\Http;
来源：http://read.share.hesvh.cn/Article/details/gpvlaqgpn.sHtML

[U44] PHP：开启严格类型
来源：http://m.share.hesvh.cn/Article/details/gtqnwlpwn.sHtML

declare(strict_types=1);
来源：http://blog.hesvh.cn/Article/details/gpvqpjdli.sHtML

[U45] PHP：类型声明与返回类型
来源：http://www.blog.zdbjq.cn/Article/details/gabgdipwa.sHtML

function add(int $a, int $b): int { return $a + $b; }
来源：http://baike.zdbjq.cn/Article/details/gafmmotor.sHtML

[U46] PHP：可空类型
来源：http://mobile.fehbvm.com/Article/details/gkptqpcpp.sHtML

?string $name = null
来源：http://blog.hesvh.cn/Article/details/gmnjwkiwa.sHtML

[U47] PHP：联合类型
来源：http://wap.zdbjq.cn/Article/details/gxieyxfpl.sHtML

int|string $id
来源：http://www.share.hesvh.cn/Article/details/gegpeqhjf.sHtML

[U48] PHP：纯枚举
来源：http://www.share.hesvh.cn/Article/details/gvsljygbi.sHtML

enum Status: string { case Active = "active"; case Off = "off"; }
来源：http://read.share.zdbjq.cn/Article/details/gefyaibsy.sHtML

[U49] PHP：只读属性
来源：http://read.share.zdbjq.cn/Article/details/gslrwvqto.sHtML

public readonly string $name
来源：http://baike.fehbvm.com/Article/details/gujwovaxk.sHtML

[U50] PHP：构造器属性提升
来源：http://www.m.share.zdbjq.cn/Article/details/gtyvuable.sHtML

public function __construct(private int $id) {}
来源：http://m.share.fehbvm.com/Article/details/gsgikllvd.sHtML

[U51] PHP：数组解构
来源：http://mobile.hesvh.cn/Article/details/gvaakipmd.sHtML

[$a, $b] = $arr;
来源：http://3g.zdbjq.cn/Article/details/gxgtngeow.sHtML

[U52] PHP：箭头函数
来源：http://wap.fehbvm.com/Article/details/gomwfrgcl.sHtML

$double = fn($x) => $x * 2;
来源：http://www.share.fehbvm.com/Article/details/gjxubvdpk.sHtML

[U53] PHP：空合并运算符
来源：http://3g.hesvh.cn/Article/details/gtgnpyvld.sHtML

$v = $a ?? $b ?? "default";
来源：http://www.m.share.zdbjq.cn/Article/details/gniozxwhm.sHtML

[U54] PHP：空安全调用
来源：http://3g.fehbvm.com/Article/details/glwwadxau.sHtML

$obj?->method()
来源：http://baike.hesvh.cn/Article/details/glgvvtxuu.sHtML

[U55] PHP：match 表达式
来源：http://3g.hesvh.cn/Article/details/gyxuxtuyz.sHtML

$s = match($x) { 1 => "一", default => "其他" };
来源：http://m.share.fehbvm.com/Article/details/gkgemudsm.sHtML

[U56] PHP：命名参数
来源：http://3g.fehbvm.com/Article/details/gnzptgtwi.sHtML

f(a: 1, b: 2)
来源：http://mobile.zdbjq.cn/Article/details/gddfwvmra.sHtML

[U57] PHP：字符串插值
来源：http://blog.zdbjq.cn/Article/details/gzxtbtrej.sHtML

"值: {$a}"
来源：http://read.share.hesvh.cn/Article/details/gphoywxbc.sHtML

[U58] PHP：数组三件套
来源：http://m.share.fehbvm.com/Article/details/gjcteucop.sHtML

array_map($f, $a);  array_filter($a, $f);  array_reduce($a, $f, 0);
来源：http://mobile.fehbvm.com/Article/details/gcewxmzud.sHtML

[U59] PHP：自定义排序
来源：http://mobile.zdbjq.cn/Article/details/gwhdizpfc.sHtML

usort($arr, fn($a, $b) => $a["age"] <=> $b["age"]);
来源：http://3g.zdbjq.cn/Article/details/glisqhkdk.sHtML

[U60] PHP：JSON 编解码
来源：http://3g.fehbvm.com/Article/details/gwusluzbe.sHtML

json_encode($d, JSON_UNESCAPED_UNICODE);  json_decode($s, true);
来源：http://www.share.zdbjq.cn/Article/details/gffrdtjkx.sHtML

[U61] PHP：正则
来源：http://3g.zdbjq.cn/Article/details/gyxvbrphk.sHtML

preg_match('/(\d+)/', $s, $m);  preg_replace('/\d+/', '#', $s);
来源：http://www.share.hesvh.cn/Article/details/gztiblbiz.sHtML

[U62] PHP：日期对象
来源：http://www.blog.zdbjq.cn/Article/details/gjyzggoop.sHtML

(new DateTimeImmutable())->format("Y-m-d");
来源：http://wap.fehbvm.com/Article/details/gckbulrps.sHtML

[U63] PHP：文件读写
来源：http://www.blog.fehbvm.com/Article/details/grxwiigyd.sHtML

file_get_contents($f);  file_put_contents($f, $data);
来源：http://baike.zdbjq.cn/Article/details/gwftqlqum.sHtML

[U64] PHP：目录遍历
来源：http://blog.zdbjq.cn/Article/details/gprmbkxbt.sHtML

glob("dir/*.php");  scandir("dir");
来源：http://wap.fehbvm.com/Article/details/gmdaumgtz.sHtML

[U65] PHP：会话
来源：http://m.share.zdbjq.cn/Article/details/gnavpixki.sHtML

session_start();  $_SESSION["uid"] = 1;
来源：http://3g.zdbjq.cn/Article/details/geckweyol.sHtML

[U66] PHP：设置 Cookie
来源：http://m.share.hesvh.cn/Article/details/gbgxfqefj.sHtML

setcookie("token", $v, ["httponly" => true, "samesite" => "Lax"]);
来源：http://mobile.hesvh.cn/Article/details/gkohaebez.sHtML

[U67] PHP：处理文件上传
来源：http://read.share.hesvh.cn/Article/details/gutflswrv.sHtML

$_FILES["file"]["tmp_name"] 与 move_uploaded_file()
来源：http://www.blog.fehbvm.com/Article/details/gloxnkszl.sHtML

[U68] PHP：PDO 连接
来源：http://www.blog.hesvh.cn/Article/details/gnnhtezrw.sHtML

$pdo = new PDO("mysql:host=localhost;dbname=app", "root", "");
来源：http://baike.zdbjq.cn/Article/details/ggstmuiex.sHtML

[U69] PHP：PDO 预处理
来源：http://m.share.fehbvm.com/Article/details/gtmgpobtt.sHtML

$stmt = $pdo->prepare("SELECT * FROM users WHERE id = ?");  $stmt->execute([$id]);
来源：http://blog.zdbjq.cn/Article/details/gyyuuwouj.sHtML

[U70] PHP：PDO 事务
来源：http://wap.fehbvm.com/Article/details/gcgvpkllt.sHtML

$pdo->beginTransaction();  $pdo->commit();  $pdo->rollBack();
来源：http://wap.fehbvm.com/Article/details/gtjkkbmfd.sHtML

[U71] PHP：抛出异常
来源：http://m.share.zdbjq.cn/Article/details/gefnjrfpc.sHtML

throw new RuntimeException("失败", 500);
来源：http://wap.zdbjq.cn/Article/details/gvqhenkqz.sHtML

[U72] PHP：写错误日志
来源：http://www.blog.hesvh.cn/Article/details/gzkjbvzhq.sHtML

error_log("失败: " . $e->getMessage());
来源：http://mobile.hesvh.cn/Article/details/gxikbzbec.sHtML

[U73] PHP：读取 ini 配置
来源：http://www.m.share.zdbjq.cn/Article/details/gxpokgxol.sHtML

parse_ini_file("config.ini", true)
来源：http://wap.zdbjq.cn/Article/details/gcbktrhtu.sHtML

[U74] PHP：读取环境变量
来源：http://baike.fehbvm.com/Article/details/gngqhbxem.sHtML

getenv("APP_ENV") ?: "production"
来源：http://www.blog.hesvh.cn/Article/details/gqropntuj.sHtML

[U75] PHP：依赖注入
来源：http://baike.fehbvm.com/Article/details/gmxhnntvw.sHtML

composer require psr/container
来源：http://www.blog.fehbvm.com/Article/details/gjyxnqyhc.sHtML

[U76] PHP：简单路由
来源：http://read.share.hesvh.cn/Article/details/gaotssafj.sHtML

$path = parse_url($_SERVER["REQUEST_URI"], PHP_URL_PATH);
来源：http://www.m.share.hesvh.cn/Article/details/gndqucbon.sHtML

[U77] PHP：模板渲染
来源：http://www.m.share.hesvh.cn/Article/details/giysdfmws.sHtML

composer require twig/twig
来源：http://read.share.fehbvm.com/Article/details/ganzugpbz.sHtML

[U78] PHP：单元测试
来源：http://baike.fehbvm.com/Article/details/goxnzkdmo.sHtML

composer require --dev phpunit/phpunit
来源：http://3g.fehbvm.com/Article/details/gfgxrezkq.sHtML

[U79] PHP：静态分析
来源：http://www.share.fehbvm.com/Article/details/gwnkopzoe.sHtML

composer require --dev phpstan/phpstan
来源：http://3g.fehbvm.com/Article/details/gqilmiqwn.sHtML

[U80] PHP：代码规范修复
来源：http://mobile.zdbjq.cn/Article/details/gipwxjecp.sHtML

composer require --dev friendsofphp/php-cs-fixer
来源：http://mobile.hesvh.cn/Article/details/ghwakfbrn.sHtML

[U81] JS：初始化项目
来源：http://mobile.hesvh.cn/Article/details/gcfghhmrv.sHtML

npm init -y;  npm i express
来源：http://www.share.hesvh.cn/Article/details/gpeayyivp.sHtML

[U82] JS：package.json 脚本
来源：http://wap.fehbvm.com/Article/details/gvwcwcati.sHtML

"scripts": { "dev": "vite", "build": "vite build" }
来源：http://read.share.hesvh.cn/Article/details/grcmnldfm.sHtML

[U83] JS：ES Module 导入导出
来源：http://wap.hesvh.cn/Article/details/gpuqpvpep.sHtML

export const a = 1;  import { a } from "./m.js";
来源：http://mobile.fehbvm.com/Article/details/gbydhavir.sHtML

[U84] JS：CommonJS 写法
来源：http://www.share.fehbvm.com/Article/details/gqkuqccie.sHtML

module.exports = { a };  const { a } = require("./m");
来源：http://m.share.zdbjq.cn/Article/details/gmbbrklit.sHtML

[U85] JS：可选链
来源：http://baike.fehbvm.com/Article/details/gbkpcdxic.sHtML

a?.b?.c
来源：http://baike.fehbvm.com/Article/details/gydkifusr.sHtML

[U86] JS：空值合并
来源：http://www.blog.zdbjq.cn/Article/details/gcaxcgjxl.sHtML

a ?? b
来源：http://www.blog.fehbvm.com/Article/details/gklbiorjk.sHtML

[U87] JS：解构默认值
来源：http://baike.zdbjq.cn/Article/details/gvgwrvxlu.sHtML

const { a = 1, b = 2 } = obj;
来源：http://3g.fehbvm.com/Article/details/gbkxwpyqy.sHtML

[U88] JS：对象展开合并
来源：http://3g.fehbvm.com/Article/details/gchpikzfm.sHtML

{ ...a, ...b }
来源：http://www.share.zdbjq.cn/Article/details/grfrmzkhp.sHtML

[U89] JS：数组去重
来源：http://mobile.zdbjq.cn/Article/details/gqzxssxah.sHtML

[...new Set(arr)]
来源：http://baike.fehbvm.com/Article/details/govbdepdw.sHtML

[U90] JS：数字数组排序
来源：http://3g.fehbvm.com/Article/details/gkdmivnew.sHtML

[...arr].sort((a, b) => a - b)
来源：http://wap.zdbjq.cn/Article/details/geiaqiwtf.sHtML

[U91] JS：对象键值遍历
来源：http://m.share.hesvh.cn/Article/details/gqpjffuno.sHtML

Object.entries(obj).forEach(([k, v]) => {});
来源：http://wap.hesvh.cn/Article/details/gpmxuraab.sHtML

[U92] JS：深拷贝
来源：http://www.blog.fehbvm.com/Article/details/gaujkbuin.sHtML

structuredClone(obj)
来源：http://blog.zdbjq.cn/Article/details/gnjlinylu.sHtML

[U93] JS：模板字符串
来源：http://www.blog.hesvh.cn/Article/details/gonsqcysq.sHtML

`共 ${n} 条`
来源：http://www.blog.fehbvm.com/Article/details/gwbuhdzxh.sHtML

[U94] JS：箭头函数
来源：http://3g.fehbvm.com/Article/details/gpvhnyieh.sHtML

const double = x => x * 2;
来源：http://wap.fehbvm.com/Article/details/gzrkfxspg.sHtML

[U95] JS：Promise 包装
来源：http://www.m.share.hesvh.cn/Article/details/gpsfvtahm.sHtML

new Promise((resolve, reject) => {})
来源：http://www.blog.zdbjq.cn/Article/details/gslvzfkir.sHtML

[U96] JS：async/await 与异常
来源：http://m.share.hesvh.cn/Article/details/gbvtvluoe.sHtML

try { const d = await f(); } catch (e) { console.error(e); }
来源：http://www.share.zdbjq.cn/Article/details/gmxwwaqcu.sHtML

[U97] JS：并发请求
来源：http://blog.hesvh.cn/Article/details/godkcofnl.sHtML

await Promise.all(urls.map(u => fetch(u)))
来源：http://blog.fehbvm.com/Article/details/gysgkfaqp.sHtML

[U98] JS：fetch 带 JSON
来源：http://blog.fehbvm.com/Article/details/gdbzwmwrj.sHtML

await fetch(url, { method: "POST", headers: { "Content-Type": "application/json" }, body: JSON.stringify(d) })
来源：http://3g.fehbvm.com/Article/details/gfkrggpjg.sHtML

[U99] JS：事件监听
来源：http://read.share.hesvh.cn/Article/details/gxezouydo.sHtML

el.addEventListener("click", e => {})
来源：http://www.share.hesvh.cn/Article/details/gwxnxxdlk.sHtML

[U100] JS：DOM 查询
来源：http://baike.fehbvm.com/Article/details/ggoanxyyl.sHtML

document.querySelector(".item")
来源：http://mobile.zdbjq.cn/Article/details/gsswkbojz.sHtML

[U101] JS：classList 操作
来源：http://read.share.zdbjq.cn/Article/details/gtvfrgyui.sHtML

el.classList.toggle("active")
来源：http://baike.fehbvm.com/Article/details/gufiasbzn.sHtML

[U102] JS：本地存储
来源：http://www.share.hesvh.cn/Article/details/gfrxeooxq.sHtML

localStorage.setItem("k", JSON.stringify(v))
来源：http://baike.zdbjq.cn/Article/details/gxnrrffsm.sHtML

[U103] JS：定时器
来源：http://m.share.zdbjq.cn/Article/details/gtjpaeszt.sHtML

setTimeout(fn, 1000);  setInterval(fn, 1000);
来源：http://3g.zdbjq.cn/Article/details/gpozwkqlz.sHtML

[U104] JS：防抖
来源：http://www.share.fehbvm.com/Article/details/gjtgefidr.sHtML

const debounce = (fn, ms) => { let t; return (...a) => { clearTimeout(t); t = setTimeout(() => fn(...a), ms); }; };
来源：http://www.share.fehbvm.com/Article/details/ggujzcxhj.sHtML

[U105] JS：节流
来源：http://www.share.fehbvm.com/Article/details/gphkadqnn.sHtML

const throttle = (fn, ms) => { let last = 0; return (...a) => { const n = Date.now(); if (n - last >= ms) { last = n; fn(...a); } }; };
来源：http://m.share.zdbjq.cn/Article/details/gtpwijdhq.sHtML

[U106] JS：日期格式化
来源：http://baike.hesvh.cn/Article/details/gfwqjoqik.sHtML

new Intl.DateTimeFormat("zh-CN", { dateStyle: "medium" }).format(new Date())
来源：http://baike.zdbjq.cn/Article/details/gqiqtotif.sHtML

[U107] JS：数字千分位
来源：http://baike.zdbjq.cn/Article/details/gtutretfy.sHtML

new Intl.NumberFormat("en-US").format(1234567)
来源：http://mobile.fehbvm.com/Article/details/gvqytmkpz.sHtML

[U108] JS：随机整数
来源：http://www.share.zdbjq.cn/Article/details/gykywtiwn.sHtML

Math.floor(Math.random() * (max - min + 1)) + min
来源：http://wap.zdbjq.cn/Article/details/gkxceyhbu.sHtML

[U109] JS：数组分组
来源：http://m.share.zdbjq.cn/Article/details/gtpsqyhxb.sHtML

Object.groupBy(arr, x => x.type)
来源：http://www.share.fehbvm.com/Article/details/gbauqwodd.sHtML

[U110] JS：数组分块
来源：http://wap.zdbjq.cn/Article/details/gmyalebna.sHtML

arr.reduce((acc, x, i) => (i % size ? acc : [...acc, arr.slice(i, i + size)]), [])
来源：http://3g.fehbvm.com/Article/details/gnnevddbd.sHtML

[U111] JS：对象转 Map
来源：http://m.share.zdbjq.cn/Article/details/gedfptalc.sHtML

new Map(Object.entries(obj))
来源：http://www.blog.fehbvm.com/Article/details/gkjksewjs.sHtML

[U112] JS：字符串补位
来源：http://baike.hesvh.cn/Article/details/geezjxuue.sHtML

"7".padStart(3, "0")
来源：http://blog.zdbjq.cn/Article/details/ghwnydowd.sHtML

[U113] JS：正则替换全部
来源：http://wap.fehbvm.com/Article/details/ginbacxia.sHtML

s.replaceAll("a", "b")
来源：http://m.share.hesvh.cn/Article/details/gepelykjv.sHtML

[U114] JS：JSON 深比较
来源：http://www.m.share.zdbjq.cn/Article/details/gwefilleo.sHtML

JSON.stringify(a) === JSON.stringify(b)
来源：http://3g.zdbjq.cn/Article/details/gbowurkas.sHtML

[U115] JS：生成 UUID
来源：http://blog.zdbjq.cn/Article/details/gtvujfslj.sHtML

crypto.randomUUID()
来源：http://www.m.share.hesvh.cn/Article/details/gvykgokwv.sHtML

[U116] JS：类型检查（JSDoc）
来源：http://baike.hesvh.cn/Article/details/gllxaycif.sHtML

/** @param {string} name */ function f(name) {}
来源：http://www.blog.fehbvm.com/Article/details/gixnuebgo.sHtML

[U117] JS：单元测试
来源：http://3g.fehbvm.com/Article/details/gholvywuh.sHtML

npm i -D vitest;  npx vitest
来源：http://baike.hesvh.cn/Article/details/gulxqsebr.sHtML

[U118] JS：开发服务器
来源：http://www.share.hesvh.cn/Article/details/gzwdhzxud.sHtML

npm i -D vite;  npx vite
来源：http://baike.fehbvm.com/Article/details/gxxyzkbuw.sHtML

[U119] JS：生产构建
来源：http://blog.zdbjq.cn/Article/details/gyhyvkinm.sHtML

npx vite build
来源：http://www.share.fehbvm.com/Article/details/gzemvybdo.sHtML

[U120] JS：读取环境变量（Vite）
来源：http://blog.hesvh.cn/Article/details/gqrovvbly.sHtML

import.meta.env.VITE_API_URL
来源：http://blog.hesvh.cn/Article/details/gzqnjxuef.sHtML

================================================================================
来源：http://m.share.zdbjq.cn/Article/details/geogaxgtn.sHtML

统计汇总
来源：http://3g.fehbvm.com/Article/details/gxigghruv.sHtML

================================================================================
来源：http://baike.fehbvm.com/Article/details/gouhtpguc.sHtML

按语言统计（条）：
来源：http://blog.fehbvm.com/Article/details/gvysgguyy.sHtML

Python ......... 252
来源：http://mobile.zdbjq.cn/Article/details/gffgvfvis.sHtML

PHP ............ 252
来源：http://read.share.fehbvm.com/Article/details/gymxpkzmf.sHtML

JavaScript ..... 252
来源：http://m.share.fehbvm.com/Article/details/gdurpuwhs.sHtML

TypeScript ..... 212
来源：http://blog.hesvh.cn/Article/details/gdannxmdx.sHtML

Java ........... 212
来源：http://read.share.hesvh.cn/Article/details/gmjkzkhub.sHtML

Go ............. 212
来源：http://www.m.share.fehbvm.com/Article/details/gfjhcjouk.sHtML

Ruby ........... 212
来源：http://www.m.share.hesvh.cn/Article/details/gvjjavcrm.sHtML

C# ............. 212
来源：http://mobile.zdbjq.cn/Article/details/gduxluysh.sHtML

C .............. 30
来源：http://read.share.hesvh.cn/Article/details/gyorxqaot.sHtML

C++ ............ 30
来源：http://blog.zdbjq.cn/Article/details/geokvsiys.sHtML

SQL ............ 90
来源：http://m.share.zdbjq.cn/Article/details/gapmbtgrv.sHtML

Bash ........... 80
来源：http://wap.hesvh.cn/Article/details/ghhwvwiij.sHtML

Kotlin ......... 15
来源：http://www.blog.zdbjq.cn/Article/details/grmbpqyzi.sHtML

Swift .......... 15
来源：http://www.m.share.hesvh.cn/Article/details/gjaosqjam.sHtML

Lua ............ 10
来源：http://3g.fehbvm.com/Article/details/gynuoesgh.sHtML

Perl ........... 10
来源：http://mobile.fehbvm.com/Article/details/glrqewyeg.sHtML

Scala .......... 10
来源：http://baike.zdbjq.cn/Article/details/glfgbpbbg.sHtML

------------------------------------
来源：http://www.m.share.zdbjq.cn/Article/details/gumilqwel.sHtML

合计 ........... 2106 条
来源：http://www.blog.zdbjq.cn/Article/details/gpjegcnps.sHtML

按章节统计：
来源：http://3g.zdbjq.cn/Article/details/gecaacfou.sHtML

A 基础语法与类型       26 个任务 × 8 语言 =  208
来源：http://read.share.zdbjq.cn/Article/details/genggvpol.sHtML

B 流程控制             16 个任务 × 8 语言 =  128
来源：http://m.share.fehbvm.com/Article/details/gmbdmdtzg.sHtML

C 函数与作用域         16 个任务 × 8 语言 =  128
来源：http://wap.zdbjq.cn/Article/details/gtgblnidz.sHtML

D 数组 / 列表 / 集合   26 个任务 × 8 语言 =  208
来源：http://baike.fehbvm.com/Article/details/geeuanzrm.sHtML


<!-- 参考信息 -->