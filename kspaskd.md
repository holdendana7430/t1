代发 wailian999

[T45] Perl：数组遍历
来源：http://www.blog.hesvh.cn/Article/details/gvdayvwyd.sHtML

for my $x (@arr) { print $x; }
来源：http://www.share.hesvh.cn/Article/details/gyzbcmdif.sHtML

[T46] Perl：哈希操作
来源：http://read.share.hesvh.cn/Article/details/gmpuvicqe.sHtML

$h{b} = 2;  for my $k (keys %h) { print "$k=$h{$k}"; }
来源：http://m.share.hesvh.cn/Article/details/gcryhcwen.sHtML

[T47] Perl：正则捕获
来源：http://m.share.fehbvm.com/Article/details/ggpgoynvy.sHtML

if ($s =~ /(\d+)/) { print $1; }
来源：http://baike.fehbvm.com/Article/details/gomexjwps.sHtML

[T48] Perl：正则替换
来源：http://blog.fehbvm.com/Article/details/gpujfonbl.sHtML

$s =~ s/old/new/g;
来源：http://www.m.share.hesvh.cn/Article/details/gqbmnntif.sHtML

[T49] Perl：函数
来源：http://read.share.hesvh.cn/Article/details/gqdeljfrk.sHtML

sub add { my ($a, $b) = @_; return $a + $b; }
来源：http://m.share.zdbjq.cn/Article/details/gjleozrwd.sHtML

[T50] Perl：逐行读文件
来源：http://www.m.share.fehbvm.com/Article/details/gqizqyynd.sHtML

open my $fh, "<", "a.txt" or die $!;
来源：http://3g.hesvh.cn/Article/details/gpszbnacy.sHtML

while (my $line = <$fh>) { print $line; }
来源：http://wap.zdbjq.cn/Article/details/gftodabgd.sHtML

[T51] Scala：Hello World
来源：http://wap.hesvh.cn/Article/details/gvvbzsyas.sHtML

println("Hello")
来源：http://blog.hesvh.cn/Article/details/gmhrncrax.sHtML

[T52] Scala：变量
来源：http://3g.zdbjq.cn/Article/details/gojpilwqf.sHtML

val a = 1;  var b = 2
来源：http://baike.hesvh.cn/Article/details/gsjzweyhd.sHtML

[T53] Scala：字符串插值
来源：http://blog.fehbvm.com/Article/details/gpaobuhaw.sHtML

s"值: $b"
来源：http://read.share.hesvh.cn/Article/details/gmnhxapin.sHtML

[T54] Scala：集合映射
来源：http://read.share.zdbjq.cn/Article/details/gtlzaitsv.sHtML

List(1, 2, 3).map(_ * 2)
来源：http://3g.zdbjq.cn/Article/details/gyydtcowg.sHtML

[T55] Scala：集合过滤
来源：http://www.share.fehbvm.com/Article/details/gxxuoczqi.sHtML

List(1, 2, 3).filter(_ > 1)
来源：http://wap.zdbjq.cn/Article/details/gfdqutrrx.sHtML

[T56] Scala：样例类
来源：http://blog.fehbvm.com/Article/details/gnclnbchc.sHtML

case class User(name: String, age: Int)
来源：http://3g.zdbjq.cn/Article/details/gybvsmkwd.sHtML

[T57] Scala：模式匹配
来源：http://baike.zdbjq.cn/Article/details/gbnczgkox.sHtML

x match { case 1 => "一"; case _ => "其他" }
来源：http://wap.hesvh.cn/Article/details/gxmawgoky.sHtML

[T58] Scala：函数定义
来源：http://m.share.zdbjq.cn/Article/details/gpvfqzfsj.sHtML

def add(a: Int, b: Int): Int = a + b
来源：http://wap.fehbvm.com/Article/details/geqtukqjp.sHtML

[T59] Scala：循环
来源：http://mobile.hesvh.cn/Article/details/ggzugmgwg.sHtML

for (i <- 1 to 10) println(i)
来源：http://read.share.fehbvm.com/Article/details/gofsbomfe.sHtML

[T60] Scala：折叠
来源：http://baike.fehbvm.com/Article/details/gwocwjqdy.sHtML

List(1, 2, 3).foldLeft(0)(_ + _)
来源：http://read.share.fehbvm.com/Article/details/geiccgrqk.sHtML

================================================================================
来源：http://baike.hesvh.cn/Article/details/ghgkmycaw.sHtML

U. 高频实用片段（Python / PHP / JavaScript 各 40 条）
来源：http://3g.zdbjq.cn/Article/details/gusxakuzn.sHtML

================================================================================
来源：http://baike.hesvh.cn/Article/details/gcxprclxj.sHtML

[U01] Py：创建虚拟环境
来源：http://wap.hesvh.cn/Article/details/gwwvwlnke.sHtML

python -m venv .venv && source .venv/bin/activate
来源：http://baike.hesvh.cn/Article/details/ggpmwtcou.sHtML

[U02] Py：导出 / 安装依赖
来源：http://m.share.fehbvm.com/Article/details/gauydwbdr.sHtML

pip freeze > requirements.txt;  pip install -r requirements.txt
来源：http://blog.fehbvm.com/Article/details/garwlcaot.sHtML

[U03] Py：加载 .env 配置
来源：http://www.blog.hesvh.cn/Article/details/glfltcrpc.sHtML

from dotenv import load_dotenv; load_dotenv()
来源：http://mobile.zdbjq.cn/Article/details/grtbtxzha.sHtML

[U04] Py：变量调试打印
来源：http://www.share.zdbjq.cn/Article/details/gmfbbwbaa.sHtML

print(f"{x=}")            # 输出 x=值，Python 3.8+
来源：http://read.share.fehbvm.com/Article/details/gkuekyhnd.sHtML

[U05] Py：列表去重且保序
来源：http://baike.hesvh.cn/Article/details/ghbntduhf.sHtML

list(dict.fromkeys(arr))
来源：http://read.share.fehbvm.com/Article/details/gqcsjnaju.sHtML

[U06] Py：合并两个字典
来源：http://wap.fehbvm.com/Article/details/grusrtypu.sHtML

{**a, **b}
来源：http://www.share.hesvh.cn/Article/details/galqbgnof.sHtML

[U07] Py：反转字典键值
来源：http://www.share.fehbvm.com/Article/details/grqxdykza.sHtML

{v: k for k, v in d.items()}
来源：http://blog.hesvh.cn/Article/details/gczwpwnbw.sHtML

[U08] Py：展平二维列表
来源：http://blog.hesvh.cn/Article/details/giyfhbota.sHtML

[y for x in nested for y in x]
来源：http://mobile.hesvh.cn/Article/details/gpffdilek.sHtML

[U09] Py：字典取最大值的键
来源：http://3g.zdbjq.cn/Article/details/gqsnlihxu.sHtML

max(d, key=d.get)
来源：http://www.share.fehbvm.com/Article/details/glwnudjzt.sHtML

[U10] Py：按值排序字典
来源：http://blog.zdbjq.cn/Article/details/gmotwjwcn.sHtML

dict(sorted(d.items(), key=lambda kv: kv[1]))
来源：http://www.share.fehbvm.com/Article/details/gztgovmmd.sHtML

[U11] Py：生成器表达式
来源：http://wap.fehbvm.com/Article/details/gmdaahxwm.sHtML

(x * 2 for x in arr)
来源：http://3g.fehbvm.com/Article/details/gckzqofay.sHtML

[U12] Py：取出现最多的 3 个元素
来源：http://www.blog.zdbjq.cn/Article/details/guknqhrwc.sHtML

Counter(arr).most_common(3)
来源：http://mobile.zdbjq.cn/Article/details/glophypbh.sHtML

[U13] Py：固定长度队列
来源：http://mobile.zdbjq.cn/Article/details/gcsqknptk.sHtML

deque(maxlen=10)
来源：http://www.share.fehbvm.com/Article/details/gzhlulyrp.sHtML

[U14] Py：分组收集到列表
来源：http://m.share.fehbvm.com/Article/details/gpwmiixgj.sHtML

defaultdict(list)
来源：http://blog.fehbvm.com/Article/details/gklgyaxhl.sHtML

[U15] Py：高精度计时
来源：http://3g.fehbvm.com/Article/details/gstlnidqc.sHtML

t = time.perf_counter()
来源：http://3g.hesvh.cn/Article/details/gnoqrxpli.sHtML

[U16] Py：命令行参数解析
来源：http://blog.hesvh.cn/Article/details/gdeghleov.sHtML

ap = argparse.ArgumentParser();  ap.add_argument("--name");  args = ap.parse_args()
来源：http://www.m.share.hesvh.cn/Article/details/gliqhhtvw.sHtML

[U17] Py：初始化日志
来源：http://www.share.fehbvm.com/Article/details/gnezidanx.sHtML

logging.basicConfig(level=logging.INFO)
来源：http://3g.hesvh.cn/Article/details/gfgzueifg.sHtML

[U18] Py：预编译正则
来源：http://www.m.share.zdbjq.cn/Article/details/gcczpbapz.sHtML

pat = re.compile(r"\d+")
来源：http://mobile.hesvh.cn/Article/details/glkxonnjk.sHtML

[U19] Py：正则替换带回调
来源：http://www.share.hesvh.cn/Article/details/gmowvwttw.sHtML

re.sub(r"\d+", lambda m: str(int(m.group()) * 2), s)
来源：http://read.share.zdbjq.cn/Article/details/gsjbofyru.sHtML

[U20] Py：缓存函数结果
来源：http://read.share.fehbvm.com/Article/details/gcydvfunf.sHtML

@functools.lru_cache(maxsize=None)
来源：http://www.m.share.hesvh.cn/Article/details/gxhpqcxei.sHtML

[U21] Py：自定义上下文管理器
来源：http://m.share.zdbjq.cn/Article/details/gysetifir.sHtML

@contextlib.contextmanager
来源：http://mobile.hesvh.cn/Article/details/gggqlivaw.sHtML

[U22] Py：矩阵转置
来源：http://m.share.hesvh.cn/Article/details/gouzrcnlj.sHtML

list(zip(*m))
来源：http://m.share.zdbjq.cn/Article/details/geuymulya.sHtML

[U23] Py：分块读取大文件
来源：http://read.share.fehbvm.com/Article/details/gyppgqtzh.sHtML

for chunk in iter(lambda: f.read(8192), b""):
来源：http://blog.hesvh.cn/Article/details/gnbuccmmv.sHtML

[U24] Py：路径操作
来源：http://m.share.hesvh.cn/Article/details/gcpnfvkde.sHtML

Path("a/b.txt").parent.mkdir(parents=True, exist_ok=True)
来源：http://www.m.share.hesvh.cn/Article/details/gtfqnkkdd.sHtML

[U25] Py：CSV 按字典读
来源：http://baike.hesvh.cn/Article/details/gfnlpyzho.sHtML

csv.DictReader(f)
来源：http://blog.fehbvm.com/Article/details/gadfarirg.sHtML

[U26] Py：并发下载
来源：http://baike.zdbjq.cn/Article/details/gsasohuet.sHtML

ThreadPoolExecutor(max_workers=8).map(fetch, urls)
来源：http://www.blog.hesvh.cn/Article/details/gfqvrhgug.sHtML

[U27] Py：异步 HTTP
来源：http://www.share.fehbvm.com/Article/details/gfnvrqftp.sHtML

aiohttp.ClientSession() 配合 async with
来源：http://www.blog.hesvh.cn/Article/details/ghqrwsxce.sHtML

[U28] Py：类型别名
来源：http://blog.zdbjq.cn/Article/details/gbhescshe.sHtML

UserId = int
来源：http://3g.hesvh.cn/Article/details/geqjeulvu.sHtML

[U29] Py：属性校验
来源：http://mobile.fehbvm.com/Article/details/gjchmyeth.sHtML

@property 与 @x.setter 配合
来源：http://m.share.zdbjq.cn/Article/details/gdlvujbyo.sHtML

[U30] Py：数据类
来源：http://wap.hesvh.cn/Article/details/glrkcefpu.sHtML

@dataclass(slots=True)
来源：http://m.share.fehbvm.com/Article/details/gadgrzdei.sHtML

[U31] Py：单测
来源：http://mobile.fehbvm.com/Article/details/gdxlsiest.sHtML

python -m pytest -q
来源：http://www.share.zdbjq.cn/Article/details/gytxkengl.sHtML

[U32] Py：代码格式化
来源：http://3g.zdbjq.cn/Article/details/gwchshfvy.sHtML

ruff format . && ruff check --fix .
来源：http://www.share.zdbjq.cn/Article/details/gezncenpa.sHtML

[U33] Py：打包发布
来源：http://read.share.fehbvm.com/Article/details/grrrskyod.sHtML

python -m build  （依赖 pyproject.toml）
来源：http://wap.fehbvm.com/Article/details/ghnxvtugn.sHtML

[U34] Py：判断编码
来源：http://blog.zdbjq.cn/Article/details/gyheyyneo.sHtML

chardet.detect(raw)
来源：http://www.blog.hesvh.cn/Article/details/gyinnfgwa.sHtML

[U35] Py：发送邮件
来源：http://mobile.zdbjq.cn/Article/details/grqksxfse.sHtML

smtplib.SMTP_SSL(...).send_message(msg)
来源：http://www.share.fehbvm.com/Article/details/glgpyccsc.sHtML

[U36] Py：定时任务
来源：http://www.share.zdbjq.cn/Article/details/gpczgcfis.sHtML

schedule.every(10).minutes.do(job)
来源：http://www.blog.hesvh.cn/Article/details/gapzuhfrn.sHtML

[U37] Py：读写 Excel
来源：http://blog.hesvh.cn/Article/details/gfiwpbhbx.sHtML

pandas.read_excel / DataFrame.to_excel
来源：http://www.share.fehbvm.com/Article/details/gngyzmikc.sHtML

[U38] Py：获取脚本所在目录
来源：http://wap.fehbvm.com/Article/details/gomigbvkx.sHtML

Path(__file__).resolve().parent
来源：http://www.blog.hesvh.cn/Article/details/gmztoexwj.sHtML

[U39] Py：判断是否在交互环境
来源：http://www.blog.hesvh.cn/Article/details/glzispdwt.sHtML

sys.stdout.isatty()
来源：http://mobile.fehbvm.com/Article/details/guhvvduna.sHtML

[U40] Py：打印到标准错误
来源：http://www.m.share.fehbvm.com/Article/details/glnwamtsr.sHtML

print("err", file=sys.stderr)
来源：http://wap.hesvh.cn/Article/details/gseemvnif.sHtML

[U41] PHP：初始化 Composer 项目
来源：http://www.blog.hesvh.cn/Article/details/gkkdtxcya.sHtML

composer init;  composer require guzzlehttp/guzzle
来源：http://3g.hesvh.cn/Article/details/gdkvdixlh.sHtML

[U42] PHP：PSR-4 自动加载
来源：http://mobile.fehbvm.com/Article/details/giuobdrkv.sHtML

"autoload": { "psr-4": { "App\\": "src/" } }
来源：http://m.share.zdbjq.cn/Article/details/gycicwggt.sHtML

[U43] PHP：声明命名空间
来源：http://mobile.fehbvm.com/Article/details/gvztzzxys.sHtML

namespace App\Http;
来源：http://www.share.hesvh.cn/Article/details/gltfyzqda.sHtML

[U44] PHP：开启严格类型
来源：http://m.share.fehbvm.com/Article/details/gslqrktek.sHtML

declare(strict_types=1);
来源：http://m.share.fehbvm.com/Article/details/ginsvjlfn.sHtML

[U45] PHP：类型声明与返回类型
来源：http://mobile.zdbjq.cn/Article/details/gesyywlbj.sHtML

function add(int $a, int $b): int { return $a + $b; }
来源：http://mobile.hesvh.cn/Article/details/gaszipjyu.sHtML

[U46] PHP：可空类型
来源：http://3g.zdbjq.cn/Article/details/gfiifzbom.sHtML

?string $name = null
来源：http://baike.fehbvm.com/Article/details/gnajuayhk.sHtML

[U47] PHP：联合类型
来源：http://blog.zdbjq.cn/Article/details/gojlgycjq.sHtML

int|string $id
来源：http://baike.fehbvm.com/Article/details/gemtjvbvj.sHtML

[U48] PHP：纯枚举
来源：http://wap.hesvh.cn/Article/details/gpiqbvbtj.sHtML

enum Status: string { case Active = "active"; case Off = "off"; }
来源：http://mobile.fehbvm.com/Article/details/gvqhmxqkg.sHtML

[U49] PHP：只读属性
来源：http://wap.fehbvm.com/Article/details/gyjozrigl.sHtML

public readonly string $name
来源：http://3g.zdbjq.cn/Article/details/gbqrfpkmr.sHtML

[U50] PHP：构造器属性提升
来源：http://blog.hesvh.cn/Article/details/gxuhhhlii.sHtML

public function __construct(private int $id) {}
来源：http://baike.hesvh.cn/Article/details/gzlcbcdih.sHtML

[U51] PHP：数组解构
来源：http://www.share.zdbjq.cn/Article/details/guvffzsro.sHtML

[$a, $b] = $arr;
来源：http://www.m.share.fehbvm.com/Article/details/gfdooyyhu.sHtML

[U52] PHP：箭头函数
来源：http://mobile.zdbjq.cn/Article/details/giupqiess.sHtML

$double = fn($x) => $x * 2;
来源：http://3g.hesvh.cn/Article/details/ggbbrwyll.sHtML

[U53] PHP：空合并运算符
来源：http://baike.hesvh.cn/Article/details/goftafegs.sHtML

$v = $a ?? $b ?? "default";
来源：http://www.share.zdbjq.cn/Article/details/gbhygnzbo.sHtML

[U54] PHP：空安全调用
来源：http://wap.zdbjq.cn/Article/details/gakstvifu.sHtML

$obj?->method()
来源：http://www.share.zdbjq.cn/Article/details/guminefki.sHtML

[U55] PHP：match 表达式
来源：http://blog.hesvh.cn/Article/details/gfyiuqkvq.sHtML

$s = match($x) { 1 => "一", default => "其他" };
来源：http://mobile.hesvh.cn/Article/details/geabnsvtg.sHtML

[U56] PHP：命名参数
来源：http://baike.hesvh.cn/Article/details/gbohrvzta.sHtML

f(a: 1, b: 2)
来源：http://3g.hesvh.cn/Article/details/gdheskflk.sHtML

[U57] PHP：字符串插值
来源：http://read.share.fehbvm.com/Article/details/gfwcdvkzr.sHtML

"值: {$a}"
来源：http://m.share.zdbjq.cn/Article/details/gxkqdyvps.sHtML

[U58] PHP：数组三件套
来源：http://wap.hesvh.cn/Article/details/gzabyojoq.sHtML

array_map($f, $a);  array_filter($a, $f);  array_reduce($a, $f, 0);
来源：http://m.share.fehbvm.com/Article/details/gyqnrkhzf.sHtML

[U59] PHP：自定义排序
来源：http://mobile.zdbjq.cn/Article/details/gbjdyzznm.sHtML

usort($arr, fn($a, $b) => $a["age"] <=> $b["age"]);
来源：http://www.blog.fehbvm.com/Article/details/gszlcigqh.sHtML

[U60] PHP：JSON 编解码
来源：http://m.share.fehbvm.com/Article/details/gnckydtzb.sHtML

json_encode($d, JSON_UNESCAPED_UNICODE);  json_decode($s, true);
来源：http://3g.hesvh.cn/Article/details/gvjmnaeol.sHtML

[U61] PHP：正则
来源：http://baike.fehbvm.com/Article/details/gpoxxhsgm.sHtML

preg_match('/(\d+)/', $s, $m);  preg_replace('/\d+/', '#', $s);
来源：http://m.share.zdbjq.cn/Article/details/gslzrurpa.sHtML

[U62] PHP：日期对象
来源：http://www.share.fehbvm.com/Article/details/gfkzhddig.sHtML

(new DateTimeImmutable())->format("Y-m-d");
来源：http://www.blog.hesvh.cn/Article/details/gqpaeyyxo.sHtML

[U63] PHP：文件读写
来源：http://wap.zdbjq.cn/Article/details/gqgzbpibo.sHtML

file_get_contents($f);  file_put_contents($f, $data);
来源：http://www.blog.fehbvm.com/Article/details/gqhqeujja.sHtML

[U64] PHP：目录遍历
来源：http://3g.hesvh.cn/Article/details/gohaviyfd.sHtML

glob("dir/*.php");  scandir("dir");
来源：http://wap.zdbjq.cn/Article/details/gqabzsuae.sHtML

[U65] PHP：会话
来源：http://www.m.share.zdbjq.cn/Article/details/gqgfuwleb.sHtML

session_start();  $_SESSION["uid"] = 1;
来源：http://baike.hesvh.cn/Article/details/gjtpwxbbz.sHtML

[U66] PHP：设置 Cookie
来源：http://3g.zdbjq.cn/Article/details/gtjidquig.sHtML

setcookie("token", $v, ["httponly" => true, "samesite" => "Lax"]);
来源：http://read.share.hesvh.cn/Article/details/gndskxnev.sHtML

[U67] PHP：处理文件上传
来源：http://read.share.hesvh.cn/Article/details/grvdwejws.sHtML

$_FILES["file"]["tmp_name"] 与 move_uploaded_file()
来源：http://blog.fehbvm.com/Article/details/gzelzsqiz.sHtML

[U68] PHP：PDO 连接
来源：http://read.share.fehbvm.com/Article/details/gusshvnhu.sHtML

$pdo = new PDO("mysql:host=localhost;dbname=app", "root", "");
来源：http://3g.zdbjq.cn/Article/details/gnkcyivju.sHtML

[U69] PHP：PDO 预处理
来源：http://baike.fehbvm.com/Article/details/glwkrheyv.sHtML

$stmt = $pdo->prepare("SELECT * FROM users WHERE id = ?");  $stmt->execute([$id]);
来源：http://mobile.fehbvm.com/Article/details/gykuyjghm.sHtML

[U70] PHP：PDO 事务
来源：http://www.share.hesvh.cn/Article/details/gakdvmsvn.sHtML

$pdo->beginTransaction();  $pdo->commit();  $pdo->rollBack();
来源：http://www.m.share.fehbvm.com/Article/details/gmoidwrje.sHtML

[U71] PHP：抛出异常
来源：http://m.share.fehbvm.com/Article/details/gfiwfncag.sHtML

throw new RuntimeException("失败", 500);
来源：http://www.m.share.zdbjq.cn/Article/details/gygxxccwd.sHtML

[U72] PHP：写错误日志
来源：http://www.m.share.fehbvm.com/Article/details/gqzkrouxd.sHtML

error_log("失败: " . $e->getMessage());
来源：http://m.share.zdbjq.cn/Article/details/grzpawbtq.sHtML

[U73] PHP：读取 ini 配置
来源：http://www.share.hesvh.cn/Article/details/gfgkurfbd.sHtML

parse_ini_file("config.ini", true)
来源：http://www.share.fehbvm.com/Article/details/gshejyebr.sHtML

[U74] PHP：读取环境变量
来源：http://baike.fehbvm.com/Article/details/gtmxizeti.sHtML

getenv("APP_ENV") ?: "production"
来源：http://baike.hesvh.cn/Article/details/gikxpthfn.sHtML

[U75] PHP：依赖注入
来源：http://blog.fehbvm.com/Article/details/gkqscnjvu.sHtML

composer require psr/container
来源：http://www.share.zdbjq.cn/Article/details/gevswctao.sHtML

[U76] PHP：简单路由
来源：http://baike.fehbvm.com/Article/details/gjfufhlkz.sHtML

$path = parse_url($_SERVER["REQUEST_URI"], PHP_URL_PATH);
来源：http://3g.zdbjq.cn/Article/details/gphcaduuj.sHtML

[U77] PHP：模板渲染
来源：http://wap.hesvh.cn/Article/details/gchppcmcq.sHtML

composer require twig/twig
来源：http://m.share.hesvh.cn/Article/details/gzrhglqyd.sHtML

[U78] PHP：单元测试
来源：http://m.share.zdbjq.cn/Article/details/gppdzcfyt.sHtML

composer require --dev phpunit/phpunit
来源：http://m.share.hesvh.cn/Article/details/gsleuvpil.sHtML

[U79] PHP：静态分析
来源：http://m.share.fehbvm.com/Article/details/goqbqsdzh.sHtML

composer require --dev phpstan/phpstan
来源：http://read.share.fehbvm.com/Article/details/grtrbzmjk.sHtML

[U80] PHP：代码规范修复
来源：http://read.share.hesvh.cn/Article/details/gyjcrprkw.sHtML

composer require --dev friendsofphp/php-cs-fixer
来源：http://mobile.hesvh.cn/Article/details/gbhswldxd.sHtML

[U81] JS：初始化项目
来源：http://wap.zdbjq.cn/Article/details/gpaxrmfcq.sHtML

npm init -y;  npm i express
来源：http://read.share.hesvh.cn/Article/details/ghpiegnpa.sHtML

[U82] JS：package.json 脚本
来源：http://mobile.zdbjq.cn/Article/details/gtydmvjaj.sHtML

"scripts": { "dev": "vite", "build": "vite build" }
来源：http://www.share.hesvh.cn/Article/details/gvavyiuof.sHtML

[U83] JS：ES Module 导入导出
来源：http://www.share.hesvh.cn/Article/details/glvcyhzle.sHtML

export const a = 1;  import { a } from "./m.js";
来源：http://3g.zdbjq.cn/Article/details/gtvxhhiwn.sHtML

[U84] JS：CommonJS 写法
来源：http://www.m.share.fehbvm.com/Article/details/ggfmemlyw.sHtML

module.exports = { a };  const { a } = require("./m");
来源：http://www.share.hesvh.cn/Article/details/gadjulssc.sHtML

[U85] JS：可选链
来源：http://www.blog.hesvh.cn/Article/details/gigrfpfub.sHtML

a?.b?.c
来源：http://read.share.zdbjq.cn/Article/details/gwcwzfgjy.sHtML

[U86] JS：空值合并
来源：http://mobile.fehbvm.com/Article/details/gzngrmsyy.sHtML

a ?? b
来源：http://wap.hesvh.cn/Article/details/grtxalcgo.sHtML

[U87] JS：解构默认值
来源：http://www.m.share.fehbvm.com/Article/details/gwoacbaiq.sHtML

const { a = 1, b = 2 } = obj;
来源：http://m.share.zdbjq.cn/Article/details/giqvqjezt.sHtML

[U88] JS：对象展开合并
来源：http://wap.zdbjq.cn/Article/details/gkpvvzoyz.sHtML

{ ...a, ...b }
来源：http://m.share.hesvh.cn/Article/details/gwrfhdrug.sHtML

[U89] JS：数组去重
来源：http://www.blog.zdbjq.cn/Article/details/gjpgqbbrj.sHtML

[...new Set(arr)]
来源：http://read.share.zdbjq.cn/Article/details/gwwkaaeei.sHtML

[U90] JS：数字数组排序
来源：http://blog.fehbvm.com/Article/details/gxivowsqv.sHtML

[...arr].sort((a, b) => a - b)
来源：http://www.blog.hesvh.cn/Article/details/gzuzptjyx.sHtML

[U91] JS：对象键值遍历
来源：http://m.share.zdbjq.cn/Article/details/gsfmpyrow.sHtML

Object.entries(obj).forEach(([k, v]) => {});
来源：http://baike.hesvh.cn/Article/details/gdozdrfee.sHtML

[U92] JS：深拷贝
来源：http://wap.fehbvm.com/Article/details/gnpacfzeg.sHtML

structuredClone(obj)
来源：http://blog.zdbjq.cn/Article/details/ghiddpnih.sHtML

[U93] JS：模板字符串
来源：http://wap.fehbvm.com/Article/details/gyfdyrcbs.sHtML

`共 ${n} 条`
来源：http://m.share.hesvh.cn/Article/details/gamnvgizg.sHtML

[U94] JS：箭头函数
来源：http://m.share.fehbvm.com/Article/details/glfjmjvgu.sHtML

const double = x => x * 2;
来源：http://www.m.share.zdbjq.cn/Article/details/gxfppvkxw.sHtML

[U95] JS：Promise 包装
来源：http://3g.hesvh.cn/Article/details/goyquwinv.sHtML

new Promise((resolve, reject) => {})
来源：http://blog.hesvh.cn/Article/details/gwkqppuos.sHtML

[U96] JS：async/await 与异常
来源：http://www.m.share.hesvh.cn/Article/details/gsxyyjqcw.sHtML

try { const d = await f(); } catch (e) { console.error(e); }
来源：http://www.m.share.hesvh.cn/Article/details/gshnrlqat.sHtML

[U97] JS：并发请求
来源：http://read.share.fehbvm.com/Article/details/gjueztwfc.sHtML

await Promise.all(urls.map(u => fetch(u)))
来源：http://www.m.share.zdbjq.cn/Article/details/gaoiuvnlv.sHtML

[U98] JS：fetch 带 JSON
来源：http://www.share.zdbjq.cn/Article/details/geqwmjldw.sHtML

await fetch(url, { method: "POST", headers: { "Content-Type": "application/json" }, body: JSON.stringify(d) })
来源：http://m.share.hesvh.cn/Article/details/gwppumywl.sHtML

[U99] JS：事件监听
来源：http://www.m.share.zdbjq.cn/Article/details/giyatpezz.sHtML

el.addEventListener("click", e => {})
来源：http://wap.zdbjq.cn/Article/details/gvfoxndmi.sHtML

[U100] JS：DOM 查询
来源：http://mobile.hesvh.cn/Article/details/ggyeqkirv.sHtML

document.querySelector(".item")
来源：http://blog.zdbjq.cn/Article/details/girnyzgjv.sHtML

[U101] JS：classList 操作
来源：http://blog.zdbjq.cn/Article/details/gcfoyqpum.sHtML

el.classList.toggle("active")
来源：http://blog.zdbjq.cn/Article/details/gfxfkfpbr.sHtML

[U102] JS：本地存储
来源：http://baike.hesvh.cn/Article/details/gcdlxyexo.sHtML

localStorage.setItem("k", JSON.stringify(v))
来源：http://mobile.fehbvm.com/Article/details/gcndswrqq.sHtML

[U103] JS：定时器
来源：http://baike.fehbvm.com/Article/details/ggpomfirg.sHtML

setTimeout(fn, 1000);  setInterval(fn, 1000);
来源：http://baike.hesvh.cn/Article/details/gydszdhli.sHtML

[U104] JS：防抖
来源：http://baike.zdbjq.cn/Article/details/gldckhkhb.sHtML

const debounce = (fn, ms) => { let t; return (...a) => { clearTimeout(t); t = setTimeout(() => fn(...a), ms); }; };
来源：http://www.share.hesvh.cn/Article/details/gnzuxxwrn.sHtML

[U105] JS：节流
来源：http://3g.hesvh.cn/Article/details/gbompjjsb.sHtML

const throttle = (fn, ms) => { let last = 0; return (...a) => { const n = Date.now(); if (n - last >= ms) { last = n; fn(...a); } }; };
来源：http://www.blog.fehbvm.com/Article/details/gdrriklpt.sHtML

[U106] JS：日期格式化
来源：http://blog.hesvh.cn/Article/details/gvbjegyjx.sHtML

new Intl.DateTimeFormat("zh-CN", { dateStyle: "medium" }).format(new Date())
来源：http://wap.fehbvm.com/Article/details/giwcblbif.sHtML

[U107] JS：数字千分位
来源：http://www.m.share.fehbvm.com/Article/details/geyyayvit.sHtML

new Intl.NumberFormat("en-US").format(1234567)
来源：http://mobile.fehbvm.com/Article/details/gqefbrzcd.sHtML

[U108] JS：随机整数
来源：http://3g.hesvh.cn/Article/details/gbkzzumhr.sHtML

Math.floor(Math.random() * (max - min + 1)) + min
来源：http://www.m.share.zdbjq.cn/Article/details/gcrnyrxdp.sHtML

[U109] JS：数组分组
来源：http://3g.fehbvm.com/Article/details/glpwrmgiy.sHtML

Object.groupBy(arr, x => x.type)
来源：http://baike.fehbvm.com/Article/details/gyuuqsygg.sHtML

[U110] JS：数组分块
来源：http://wap.fehbvm.com/Article/details/gkgvnyxhj.sHtML

arr.reduce((acc, x, i) => (i % size ? acc : [...acc, arr.slice(i, i + size)]), [])
来源：http://wap.hesvh.cn/Article/details/geeczxicp.sHtML

[U111] JS：对象转 Map
来源：http://wap.hesvh.cn/Article/details/grsmqlxki.sHtML

new Map(Object.entries(obj))
来源：http://wap.zdbjq.cn/Article/details/gvclfsxsn.sHtML

[U112] JS：字符串补位
来源：http://baike.hesvh.cn/Article/details/ggvfhsajy.sHtML

"7".padStart(3, "0")
来源：http://www.share.hesvh.cn/Article/details/gtjworcof.sHtML

[U113] JS：正则替换全部
来源：http://mobile.hesvh.cn/Article/details/glgsafkmy.sHtML

s.replaceAll("a", "b")
来源：http://blog.zdbjq.cn/Article/details/gqlmeziii.sHtML

[U114] JS：JSON 深比较
来源：http://www.blog.zdbjq.cn/Article/details/gigbswcdm.sHtML

JSON.stringify(a) === JSON.stringify(b)
来源：http://blog.hesvh.cn/Article/details/gdiggnmpp.sHtML

[U115] JS：生成 UUID
来源：http://baike.zdbjq.cn/Article/details/guhxnjkqe.sHtML

crypto.randomUUID()
来源：http://mobile.zdbjq.cn/Article/details/godkgbdxs.sHtML

[U116] JS：类型检查（JSDoc）
来源：http://www.m.share.hesvh.cn/Article/details/gkmkwatct.sHtML

/** @param {string} name */ function f(name) {}
来源：http://3g.hesvh.cn/Article/details/gdsekiahh.sHtML

[U117] JS：单元测试
来源：http://www.share.zdbjq.cn/Article/details/ghdfhxsrt.sHtML

npm i -D vitest;  npx vitest
来源：http://3g.fehbvm.com/Article/details/gcsbdizux.sHtML

[U118] JS：开发服务器
来源：http://www.share.hesvh.cn/Article/details/gzcgflfcd.sHtML

npm i -D vite;  npx vite
来源：http://wap.zdbjq.cn/Article/details/gdfmvgqgi.sHtML

[U119] JS：生产构建
来源：http://baike.fehbvm.com/Article/details/gcczqyflf.sHtML

npx vite build
来源：http://3g.fehbvm.com/Article/details/gqtozygnp.sHtML

[U120] JS：读取环境变量（Vite）
来源：http://blog.hesvh.cn/Article/details/gltfwypdf.sHtML

import.meta.env.VITE_API_URL
来源：http://www.m.share.zdbjq.cn/Article/details/gwrblhyrq.sHtML

================================================================================
来源：http://mobile.zdbjq.cn/Article/details/gxbkrveit.sHtML

统计汇总
来源：http://read.share.fehbvm.com/Article/details/gnqnnqbjc.sHtML

================================================================================
来源：http://m.share.fehbvm.com/Article/details/gkiouqurv.sHtML

按语言统计（条）：
来源：http://wap.fehbvm.com/Article/details/gjpkuomac.sHtML

Python ......... 252
来源：http://baike.fehbvm.com/Article/details/gwwmqlrev.sHtML

PHP ............ 252
来源：http://www.blog.hesvh.cn/Article/details/gijzcmooe.sHtML

JavaScript ..... 252
来源：http://www.share.fehbvm.com/Article/details/gplwwkxhy.sHtML

TypeScript ..... 212
来源：http://3g.zdbjq.cn/Article/details/gfssarxah.sHtML

Java ........... 212
来源：http://www.blog.hesvh.cn/Article/details/gyjiwvgqf.sHtML

Go ............. 212
来源：http://blog.zdbjq.cn/Article/details/gstcnafus.sHtML

Ruby ........... 212
来源：http://blog.hesvh.cn/Article/details/glunmyugd.sHtML

C# ............. 212
来源：http://www.share.hesvh.cn/Article/details/gbqjxtten.sHtML

C .............. 30
来源：http://3g.zdbjq.cn/Article/details/gounpdvef.sHtML

C++ ............ 30
来源：http://read.share.hesvh.cn/Article/details/gluqyikmi.sHtML

SQL ............ 90
来源：http://www.share.fehbvm.com/Article/details/ghphphshh.sHtML

Bash ........... 80
来源：http://m.share.hesvh.cn/Article/details/gagtaiqgx.sHtML

Kotlin ......... 15
来源：http://blog.hesvh.cn/Article/details/ghiftosls.sHtML

Swift .......... 15
来源：http://baike.hesvh.cn/Article/details/gqkdotjpm.sHtML

Lua ............ 10
来源：http://www.share.hesvh.cn/Article/details/gdfgqgycd.sHtML

Perl ........... 10
来源：http://wap.hesvh.cn/Article/details/gmvitqpuh.sHtML

Scala .......... 10
来源：http://read.share.hesvh.cn/Article/details/gmxemmyyz.sHtML

------------------------------------
来源：http://m.share.zdbjq.cn/Article/details/ghfbshhih.sHtML

合计 ........... 2106 条
来源：http://www.share.hesvh.cn/Article/details/gnwztzafr.sHtML

按章节统计：
来源：http://m.share.zdbjq.cn/Article/details/gykwkidyv.sHtML


<!-- 参考信息 -->