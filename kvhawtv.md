代发 wailian999

[T47] Perl：正则捕获
来源：http://baike.zdbjq.cn/Article/details/gilzywhib.sHtML

if ($s =~ /(\d+)/) { print $1; }
来源：http://blog.hesvh.cn/Article/details/gdurfrugl.sHtML

[T48] Perl：正则替换
来源：http://www.blog.fehbvm.com/Article/details/gwribgqxq.sHtML

$s =~ s/old/new/g;
来源：http://read.share.fehbvm.com/Article/details/goaeqwosk.sHtML

[T49] Perl：函数
来源：http://mobile.fehbvm.com/Article/details/ggnqmffkt.sHtML

sub add { my ($a, $b) = @_; return $a + $b; }
来源：http://wap.fehbvm.com/Article/details/gbdsbmqfl.sHtML

[T50] Perl：逐行读文件
来源：http://www.share.hesvh.cn/Article/details/grsvrgdlc.sHtML

open my $fh, "<", "a.txt" or die $!;
来源：http://baike.hesvh.cn/Article/details/ggexudmts.sHtML

while (my $line = <$fh>) { print $line; }
来源：http://www.m.share.fehbvm.com/Article/details/gnqfpjaco.sHtML

[T51] Scala：Hello World
来源：http://www.share.hesvh.cn/Article/details/ghmieqvgo.sHtML

println("Hello")
来源：http://read.share.hesvh.cn/Article/details/gzatflzzp.sHtML

[T52] Scala：变量
来源：http://blog.zdbjq.cn/Article/details/gpgnxblsm.sHtML

val a = 1;  var b = 2
来源：http://3g.hesvh.cn/Article/details/gyvxqlulx.sHtML

[T53] Scala：字符串插值
来源：http://mobile.zdbjq.cn/Article/details/gwijnekjw.sHtML

s"值: $b"
来源：http://wap.fehbvm.com/Article/details/glkulpdvg.sHtML

[T54] Scala：集合映射
来源：http://wap.zdbjq.cn/Article/details/gqmhmptce.sHtML

List(1, 2, 3).map(_ * 2)
来源：http://m.share.fehbvm.com/Article/details/gbnvluspd.sHtML

[T55] Scala：集合过滤
来源：http://www.m.share.zdbjq.cn/Article/details/gexaprtbo.sHtML

List(1, 2, 3).filter(_ > 1)
来源：http://baike.hesvh.cn/Article/details/gecwjxuyh.sHtML

[T56] Scala：样例类
来源：http://www.blog.fehbvm.com/Article/details/gveerkozw.sHtML

case class User(name: String, age: Int)
来源：http://3g.zdbjq.cn/Article/details/glnseasqm.sHtML

[T57] Scala：模式匹配
来源：http://mobile.hesvh.cn/Article/details/gebzhqfco.sHtML

x match { case 1 => "一"; case _ => "其他" }
来源：http://mobile.hesvh.cn/Article/details/gcuempaad.sHtML

[T58] Scala：函数定义
来源：http://wap.hesvh.cn/Article/details/gobwzepoo.sHtML

def add(a: Int, b: Int): Int = a + b
来源：http://www.blog.zdbjq.cn/Article/details/gudvfundv.sHtML

[T59] Scala：循环
来源：http://www.blog.fehbvm.com/Article/details/gfclhsakk.sHtML

for (i <- 1 to 10) println(i)
来源：http://baike.fehbvm.com/Article/details/gfptofppb.sHtML

[T60] Scala：折叠
来源：http://baike.zdbjq.cn/Article/details/gphjjzkss.sHtML

List(1, 2, 3).foldLeft(0)(_ + _)
来源：http://read.share.zdbjq.cn/Article/details/gcxgqhmet.sHtML

================================================================================
来源：http://3g.hesvh.cn/Article/details/gqmcmmtmv.sHtML

U. 高频实用片段（Python / PHP / JavaScript 各 40 条）
来源：http://blog.fehbvm.com/Article/details/gkgndazne.sHtML

================================================================================
来源：http://3g.fehbvm.com/Article/details/gzyecvwln.sHtML

[U01] Py：创建虚拟环境
来源：http://www.m.share.fehbvm.com/Article/details/gnbbxkfmp.sHtML

python -m venv .venv && source .venv/bin/activate
来源：http://www.blog.hesvh.cn/Article/details/gkesaffgp.sHtML

[U02] Py：导出 / 安装依赖
来源：http://www.m.share.fehbvm.com/Article/details/gtewvypyt.sHtML

pip freeze > requirements.txt;  pip install -r requirements.txt
来源：http://www.blog.zdbjq.cn/Article/details/gwinevvbb.sHtML

[U03] Py：加载 .env 配置
来源：http://mobile.hesvh.cn/Article/details/gyoslcxhb.sHtML

from dotenv import load_dotenv; load_dotenv()
来源：http://m.share.zdbjq.cn/Article/details/glbskhhjb.sHtML

[U04] Py：变量调试打印
来源：http://m.share.hesvh.cn/Article/details/gpmdclrbf.sHtML

print(f"{x=}")            # 输出 x=值，Python 3.8+
来源：http://blog.hesvh.cn/Article/details/grnuokcwf.sHtML

[U05] Py：列表去重且保序
来源：http://3g.fehbvm.com/Article/details/gueqvizmt.sHtML

list(dict.fromkeys(arr))
来源：http://3g.fehbvm.com/Article/details/gwafekfyb.sHtML

[U06] Py：合并两个字典
来源：http://wap.fehbvm.com/Article/details/gvbjwnirp.sHtML

{**a, **b}
来源：http://baike.hesvh.cn/Article/details/ggozksstr.sHtML

[U07] Py：反转字典键值
来源：http://m.share.fehbvm.com/Article/details/gcveawlmu.sHtML

{v: k for k, v in d.items()}
来源：http://baike.fehbvm.com/Article/details/giggzmrmg.sHtML

[U08] Py：展平二维列表
来源：http://www.m.share.fehbvm.com/Article/details/gybsjbczx.sHtML

[y for x in nested for y in x]
来源：http://www.blog.hesvh.cn/Article/details/gpshjmrel.sHtML

[U09] Py：字典取最大值的键
来源：http://mobile.hesvh.cn/Article/details/gotjqqnch.sHtML

max(d, key=d.get)
来源：http://www.share.zdbjq.cn/Article/details/gzqwyeooy.sHtML

[U10] Py：按值排序字典
来源：http://baike.fehbvm.com/Article/details/gukqitefn.sHtML

dict(sorted(d.items(), key=lambda kv: kv[1]))
来源：http://m.share.zdbjq.cn/Article/details/glmzvciag.sHtML

[U11] Py：生成器表达式
来源：http://3g.hesvh.cn/Article/details/gmtcrsrgi.sHtML

(x * 2 for x in arr)
来源：http://www.blog.hesvh.cn/Article/details/gqmvoukle.sHtML

[U12] Py：取出现最多的 3 个元素
来源：http://www.share.hesvh.cn/Article/details/glfijvlew.sHtML

Counter(arr).most_common(3)
来源：http://3g.zdbjq.cn/Article/details/gerlomvta.sHtML

[U13] Py：固定长度队列
来源：http://blog.fehbvm.com/Article/details/gmucynall.sHtML

deque(maxlen=10)
来源：http://3g.fehbvm.com/Article/details/gsmllvpsn.sHtML

[U14] Py：分组收集到列表
来源：http://mobile.zdbjq.cn/Article/details/gwsdfsdxu.sHtML

defaultdict(list)
来源：http://www.share.zdbjq.cn/Article/details/gxzzffzso.sHtML

[U15] Py：高精度计时
来源：http://read.share.fehbvm.com/Article/details/gtbcetffe.sHtML

t = time.perf_counter()
来源：http://m.share.fehbvm.com/Article/details/gnxiybanw.sHtML

[U16] Py：命令行参数解析
来源：http://baike.hesvh.cn/Article/details/gqaqmraqx.sHtML

ap = argparse.ArgumentParser();  ap.add_argument("--name");  args = ap.parse_args()
来源：http://wap.zdbjq.cn/Article/details/gjdtsafbz.sHtML

[U17] Py：初始化日志
来源：http://www.blog.hesvh.cn/Article/details/gbpbxmdsk.sHtML

logging.basicConfig(level=logging.INFO)
来源：http://3g.zdbjq.cn/Article/details/gjzuyymal.sHtML

[U18] Py：预编译正则
来源：http://blog.hesvh.cn/Article/details/gthrybyla.sHtML

pat = re.compile(r"\d+")
来源：http://www.blog.fehbvm.com/Article/details/gogbgcqze.sHtML

[U19] Py：正则替换带回调
来源：http://m.share.fehbvm.com/Article/details/gkfxlurgx.sHtML

re.sub(r"\d+", lambda m: str(int(m.group()) * 2), s)
来源：http://blog.hesvh.cn/Article/details/gopsndwtl.sHtML

[U20] Py：缓存函数结果
来源：http://m.share.hesvh.cn/Article/details/guwjipoqs.sHtML

@functools.lru_cache(maxsize=None)
来源：http://m.share.hesvh.cn/Article/details/gaxrpihyk.sHtML

[U21] Py：自定义上下文管理器
来源：http://wap.hesvh.cn/Article/details/guezlunoa.sHtML

@contextlib.contextmanager
来源：http://read.share.hesvh.cn/Article/details/grboyjsdf.sHtML

[U22] Py：矩阵转置
来源：http://m.share.hesvh.cn/Article/details/gsajftads.sHtML

list(zip(*m))
来源：http://mobile.hesvh.cn/Article/details/gfavopknx.sHtML

[U23] Py：分块读取大文件
来源：http://www.share.zdbjq.cn/Article/details/gwgqinbiy.sHtML

for chunk in iter(lambda: f.read(8192), b""):
来源：http://baike.zdbjq.cn/Article/details/gtizkdqsr.sHtML

[U24] Py：路径操作
来源：http://www.m.share.zdbjq.cn/Article/details/gbcxrjqop.sHtML

Path("a/b.txt").parent.mkdir(parents=True, exist_ok=True)
来源：http://www.m.share.zdbjq.cn/Article/details/gcdqznwpa.sHtML

[U25] Py：CSV 按字典读
来源：http://wap.zdbjq.cn/Article/details/ggqiumsfk.sHtML

csv.DictReader(f)
来源：http://wap.zdbjq.cn/Article/details/gnjjxzgoz.sHtML

[U26] Py：并发下载
来源：http://3g.zdbjq.cn/Article/details/glotzsxrq.sHtML

ThreadPoolExecutor(max_workers=8).map(fetch, urls)
来源：http://m.share.hesvh.cn/Article/details/guktqwdzl.sHtML

[U27] Py：异步 HTTP
来源：http://mobile.hesvh.cn/Article/details/gfcsvizng.sHtML

aiohttp.ClientSession() 配合 async with
来源：http://3g.hesvh.cn/Article/details/gbxaquukv.sHtML

[U28] Py：类型别名
来源：http://wap.zdbjq.cn/Article/details/gbctcnftl.sHtML

UserId = int
来源：http://m.share.zdbjq.cn/Article/details/gktmaxrlf.sHtML

[U29] Py：属性校验
来源：http://3g.zdbjq.cn/Article/details/gfutueyfj.sHtML

@property 与 @x.setter 配合
来源：http://mobile.hesvh.cn/Article/details/gcdeninyd.sHtML

[U30] Py：数据类
来源：http://m.share.fehbvm.com/Article/details/gpypcvtoa.sHtML

@dataclass(slots=True)
来源：http://baike.zdbjq.cn/Article/details/gehkockki.sHtML

[U31] Py：单测
来源：http://3g.zdbjq.cn/Article/details/gskobjswu.sHtML

python -m pytest -q
来源：http://m.share.fehbvm.com/Article/details/glemrrwkm.sHtML

[U32] Py：代码格式化
来源：http://www.share.fehbvm.com/Article/details/gmeuqxznr.sHtML

ruff format . && ruff check --fix .
来源：http://read.share.hesvh.cn/Article/details/gssryqqrp.sHtML

[U33] Py：打包发布
来源：http://baike.zdbjq.cn/Article/details/gyrcsmwhq.sHtML

python -m build  （依赖 pyproject.toml）
来源：http://wap.hesvh.cn/Article/details/gqhutkllw.sHtML

[U34] Py：判断编码
来源：http://www.share.zdbjq.cn/Article/details/gmivhsbeq.sHtML

chardet.detect(raw)
来源：http://baike.zdbjq.cn/Article/details/glwdnirfc.sHtML

[U35] Py：发送邮件
来源：http://www.m.share.fehbvm.com/Article/details/ggafhfvec.sHtML

smtplib.SMTP_SSL(...).send_message(msg)
来源：http://blog.zdbjq.cn/Article/details/gcumxksjo.sHtML

[U36] Py：定时任务
来源：http://baike.hesvh.cn/Article/details/gcpjbownt.sHtML

schedule.every(10).minutes.do(job)
来源：http://mobile.fehbvm.com/Article/details/gbtmksyrf.sHtML

[U37] Py：读写 Excel
来源：http://mobile.hesvh.cn/Article/details/gtpruphxb.sHtML

pandas.read_excel / DataFrame.to_excel
来源：http://mobile.zdbjq.cn/Article/details/geeglfpsu.sHtML

[U38] Py：获取脚本所在目录
来源：http://www.share.hesvh.cn/Article/details/goeexicex.sHtML

Path(__file__).resolve().parent
来源：http://www.m.share.fehbvm.com/Article/details/gqwihezgh.sHtML

[U39] Py：判断是否在交互环境
来源：http://mobile.fehbvm.com/Article/details/gamxyquzb.sHtML

sys.stdout.isatty()
来源：http://wap.zdbjq.cn/Article/details/gxggbmvwi.sHtML

[U40] Py：打印到标准错误
来源：http://m.share.fehbvm.com/Article/details/gkzjytqdf.sHtML

print("err", file=sys.stderr)
来源：http://read.share.hesvh.cn/Article/details/gbeyjdplr.sHtML

[U41] PHP：初始化 Composer 项目
来源：http://mobile.fehbvm.com/Article/details/gqhbcprqv.sHtML

composer init;  composer require guzzlehttp/guzzle
来源：http://www.blog.fehbvm.com/Article/details/gbhvubfcj.sHtML

[U42] PHP：PSR-4 自动加载
来源：http://wap.fehbvm.com/Article/details/gdxzerbus.sHtML

"autoload": { "psr-4": { "App\\": "src/" } }
来源：http://mobile.hesvh.cn/Article/details/ggjyswhva.sHtML

[U43] PHP：声明命名空间
来源：http://m.share.zdbjq.cn/Article/details/gxevfdyhq.sHtML

namespace App\Http;
来源：http://wap.hesvh.cn/Article/details/gemvvopla.sHtML

[U44] PHP：开启严格类型
来源：http://mobile.hesvh.cn/Article/details/gnezkkcgp.sHtML

declare(strict_types=1);
来源：http://mobile.fehbvm.com/Article/details/gqfqvvftu.sHtML

[U45] PHP：类型声明与返回类型
来源：http://read.share.hesvh.cn/Article/details/gfdpfxvwo.sHtML

function add(int $a, int $b): int { return $a + $b; }
来源：http://www.m.share.hesvh.cn/Article/details/gscsiogsa.sHtML

[U46] PHP：可空类型
来源：http://read.share.zdbjq.cn/Article/details/gexwrfiip.sHtML

?string $name = null
来源：http://blog.hesvh.cn/Article/details/gdqujmyru.sHtML

[U47] PHP：联合类型
来源：http://wap.zdbjq.cn/Article/details/gwwefsmnc.sHtML

int|string $id
来源：http://mobile.zdbjq.cn/Article/details/gcoacishe.sHtML

[U48] PHP：纯枚举
来源：http://blog.hesvh.cn/Article/details/gudczmpyk.sHtML

enum Status: string { case Active = "active"; case Off = "off"; }
来源：http://m.share.fehbvm.com/Article/details/gcfhjnjoe.sHtML

[U49] PHP：只读属性
来源：http://www.share.zdbjq.cn/Article/details/gzpiizsbp.sHtML

public readonly string $name
来源：http://m.share.hesvh.cn/Article/details/gwbmpbwji.sHtML

[U50] PHP：构造器属性提升
来源：http://m.share.zdbjq.cn/Article/details/guixcjuqm.sHtML

public function __construct(private int $id) {}
来源：http://mobile.hesvh.cn/Article/details/gydinpsxr.sHtML

[U51] PHP：数组解构
来源：http://mobile.hesvh.cn/Article/details/gewghlzaf.sHtML

[$a, $b] = $arr;
来源：http://m.share.zdbjq.cn/Article/details/gmpfxmsae.sHtML

[U52] PHP：箭头函数
来源：http://www.blog.fehbvm.com/Article/details/gnkoyzphr.sHtML

$double = fn($x) => $x * 2;
来源：http://blog.hesvh.cn/Article/details/gmqqgojwu.sHtML

[U53] PHP：空合并运算符
来源：http://www.share.hesvh.cn/Article/details/gkmfyinsm.sHtML

$v = $a ?? $b ?? "default";
来源：http://wap.zdbjq.cn/Article/details/gcylufket.sHtML

[U54] PHP：空安全调用
来源：http://m.share.fehbvm.com/Article/details/gklwenlgi.sHtML

$obj?->method()
来源：http://mobile.hesvh.cn/Article/details/gozyloese.sHtML

[U55] PHP：match 表达式
来源：http://www.m.share.fehbvm.com/Article/details/gicifybau.sHtML

$s = match($x) { 1 => "一", default => "其他" };
来源：http://blog.zdbjq.cn/Article/details/gebhzqbyp.sHtML

[U56] PHP：命名参数
来源：http://www.blog.fehbvm.com/Article/details/ghnpjfkcc.sHtML

f(a: 1, b: 2)
来源：http://read.share.hesvh.cn/Article/details/gjddxiwpu.sHtML

[U57] PHP：字符串插值
来源：http://read.share.fehbvm.com/Article/details/guqfkeurp.sHtML

"值: {$a}"
来源：http://www.m.share.zdbjq.cn/Article/details/gviocrmyh.sHtML

[U58] PHP：数组三件套
来源：http://wap.zdbjq.cn/Article/details/gctcckuvi.sHtML

array_map($f, $a);  array_filter($a, $f);  array_reduce($a, $f, 0);
来源：http://baike.zdbjq.cn/Article/details/gfiemaapy.sHtML

[U59] PHP：自定义排序
来源：http://wap.fehbvm.com/Article/details/gvhrzfmli.sHtML

usort($arr, fn($a, $b) => $a["age"] <=> $b["age"]);
来源：http://mobile.hesvh.cn/Article/details/gbzrnmtbc.sHtML

[U60] PHP：JSON 编解码
来源：http://www.m.share.zdbjq.cn/Article/details/gxxcjrwiz.sHtML

json_encode($d, JSON_UNESCAPED_UNICODE);  json_decode($s, true);
来源：http://blog.zdbjq.cn/Article/details/gnmrkqhjn.sHtML

[U61] PHP：正则
来源：http://3g.fehbvm.com/Article/details/gvzzcyevt.sHtML

preg_match('/(\d+)/', $s, $m);  preg_replace('/\d+/', '#', $s);
来源：http://mobile.hesvh.cn/Article/details/gyhmknibn.sHtML

[U62] PHP：日期对象
来源：http://www.blog.zdbjq.cn/Article/details/gyvpouulv.sHtML

(new DateTimeImmutable())->format("Y-m-d");
来源：http://www.blog.fehbvm.com/Article/details/gtjfiiqcs.sHtML

[U63] PHP：文件读写
来源：http://www.m.share.fehbvm.com/Article/details/gkdpfszeb.sHtML

file_get_contents($f);  file_put_contents($f, $data);
来源：http://www.blog.hesvh.cn/Article/details/gxmafonnn.sHtML

[U64] PHP：目录遍历
来源：http://wap.zdbjq.cn/Article/details/gdenjhttv.sHtML

glob("dir/*.php");  scandir("dir");
来源：http://3g.fehbvm.com/Article/details/gabhsrogv.sHtML

[U65] PHP：会话
来源：http://read.share.hesvh.cn/Article/details/gyzsuphni.sHtML

session_start();  $_SESSION["uid"] = 1;
来源：http://3g.fehbvm.com/Article/details/gdrewecyj.sHtML

[U66] PHP：设置 Cookie
来源：http://read.share.fehbvm.com/Article/details/guremwhun.sHtML

setcookie("token", $v, ["httponly" => true, "samesite" => "Lax"]);
来源：http://mobile.hesvh.cn/Article/details/gfofdzwcd.sHtML

[U67] PHP：处理文件上传
来源：http://mobile.fehbvm.com/Article/details/ggxpoqykj.sHtML

$_FILES["file"]["tmp_name"] 与 move_uploaded_file()
来源：http://mobile.fehbvm.com/Article/details/gytoapqnk.sHtML

[U68] PHP：PDO 连接
来源：http://3g.hesvh.cn/Article/details/glmkvxltt.sHtML

$pdo = new PDO("mysql:host=localhost;dbname=app", "root", "");
来源：http://www.blog.zdbjq.cn/Article/details/grcihhdxu.sHtML

[U69] PHP：PDO 预处理
来源：http://www.blog.zdbjq.cn/Article/details/gdackqmbj.sHtML

$stmt = $pdo->prepare("SELECT * FROM users WHERE id = ?");  $stmt->execute([$id]);
来源：http://www.m.share.zdbjq.cn/Article/details/gqfwymuqe.sHtML

[U70] PHP：PDO 事务
来源：http://3g.fehbvm.com/Article/details/gyaciyice.sHtML

$pdo->beginTransaction();  $pdo->commit();  $pdo->rollBack();
来源：http://m.share.zdbjq.cn/Article/details/gaowcegvp.sHtML

[U71] PHP：抛出异常
来源：http://blog.zdbjq.cn/Article/details/gpvyupscj.sHtML

throw new RuntimeException("失败", 500);
来源：http://www.m.share.fehbvm.com/Article/details/gqtkkpztr.sHtML

[U72] PHP：写错误日志
来源：http://m.share.hesvh.cn/Article/details/gqwrgiuss.sHtML

error_log("失败: " . $e->getMessage());
来源：http://mobile.zdbjq.cn/Article/details/gqwpkaopp.sHtML

[U73] PHP：读取 ini 配置
来源：http://mobile.zdbjq.cn/Article/details/gfrfmcpos.sHtML

parse_ini_file("config.ini", true)
来源：http://wap.fehbvm.com/Article/details/gamltehfi.sHtML

[U74] PHP：读取环境变量
来源：http://read.share.hesvh.cn/Article/details/grmlddxti.sHtML

getenv("APP_ENV") ?: "production"
来源：http://mobile.fehbvm.com/Article/details/glcnphtfb.sHtML

[U75] PHP：依赖注入
来源：http://blog.zdbjq.cn/Article/details/gzxwtjyuv.sHtML

composer require psr/container
来源：http://www.blog.hesvh.cn/Article/details/gulnsuvab.sHtML

[U76] PHP：简单路由
来源：http://www.share.zdbjq.cn/Article/details/gwcijhwfh.sHtML

$path = parse_url($_SERVER["REQUEST_URI"], PHP_URL_PATH);
来源：http://read.share.hesvh.cn/Article/details/ggoxopdlw.sHtML

[U77] PHP：模板渲染
来源：http://wap.fehbvm.com/Article/details/gzqxuxtwr.sHtML

composer require twig/twig
来源：http://wap.fehbvm.com/Article/details/grmawppvm.sHtML

[U78] PHP：单元测试
来源：http://mobile.zdbjq.cn/Article/details/grnypkgga.sHtML

composer require --dev phpunit/phpunit
来源：http://www.blog.hesvh.cn/Article/details/gkqwnjalg.sHtML

[U79] PHP：静态分析
来源：http://www.m.share.fehbvm.com/Article/details/gytiplrkf.sHtML

composer require --dev phpstan/phpstan
来源：http://www.blog.fehbvm.com/Article/details/gygenaing.sHtML

[U80] PHP：代码规范修复
来源：http://3g.zdbjq.cn/Article/details/girrrjhct.sHtML

composer require --dev friendsofphp/php-cs-fixer
来源：http://wap.hesvh.cn/Article/details/gdepefobr.sHtML

[U81] JS：初始化项目
来源：http://www.m.share.zdbjq.cn/Article/details/gglpamncc.sHtML

npm init -y;  npm i express
来源：http://www.share.fehbvm.com/Article/details/gvojprwxi.sHtML

[U82] JS：package.json 脚本
来源：http://baike.fehbvm.com/Article/details/godhenkyo.sHtML

"scripts": { "dev": "vite", "build": "vite build" }
来源：http://baike.zdbjq.cn/Article/details/gkbdjkjxk.sHtML

[U83] JS：ES Module 导入导出
来源：http://blog.fehbvm.com/Article/details/gttscedbz.sHtML

export const a = 1;  import { a } from "./m.js";
来源：http://m.share.zdbjq.cn/Article/details/gxtfepwbd.sHtML

[U84] JS：CommonJS 写法
来源：http://mobile.hesvh.cn/Article/details/gpylwaxcu.sHtML

module.exports = { a };  const { a } = require("./m");
来源：http://www.m.share.hesvh.cn/Article/details/ggjvskqhi.sHtML

[U85] JS：可选链
来源：http://blog.fehbvm.com/Article/details/gqydhljgf.sHtML

a?.b?.c
来源：http://wap.hesvh.cn/Article/details/gafkiaahv.sHtML

[U86] JS：空值合并
来源：http://www.share.zdbjq.cn/Article/details/gwwuwxcqp.sHtML

a ?? b
来源：http://mobile.hesvh.cn/Article/details/gxurimewf.sHtML

[U87] JS：解构默认值
来源：http://read.share.hesvh.cn/Article/details/gneyijxct.sHtML

const { a = 1, b = 2 } = obj;
来源：http://www.share.fehbvm.com/Article/details/gzerulusz.sHtML

[U88] JS：对象展开合并
来源：http://www.share.zdbjq.cn/Article/details/gzarjtmxl.sHtML

{ ...a, ...b }
来源：http://www.m.share.hesvh.cn/Article/details/gykscyzyy.sHtML

[U89] JS：数组去重
来源：http://www.blog.hesvh.cn/Article/details/gpqfxfgtp.sHtML

[...new Set(arr)]
来源：http://mobile.hesvh.cn/Article/details/gcyhkkbgv.sHtML

[U90] JS：数字数组排序
来源：http://www.m.share.fehbvm.com/Article/details/gxcoliusf.sHtML

[...arr].sort((a, b) => a - b)
来源：http://www.blog.hesvh.cn/Article/details/gmeoiwkqs.sHtML

[U91] JS：对象键值遍历
来源：http://www.m.share.hesvh.cn/Article/details/gyzprbmua.sHtML

Object.entries(obj).forEach(([k, v]) => {});
来源：http://www.blog.zdbjq.cn/Article/details/gebpizwmg.sHtML

[U92] JS：深拷贝
来源：http://blog.fehbvm.com/Article/details/gjacigafl.sHtML

structuredClone(obj)
来源：http://wap.zdbjq.cn/Article/details/gooaxenkj.sHtML

[U93] JS：模板字符串
来源：http://read.share.zdbjq.cn/Article/details/gpyoykany.sHtML

`共 ${n} 条`
来源：http://baike.fehbvm.com/Article/details/gmdycyrka.sHtML

[U94] JS：箭头函数
来源：http://baike.zdbjq.cn/Article/details/ggrwjfcdm.sHtML

const double = x => x * 2;
来源：http://www.blog.hesvh.cn/Article/details/gacvthhrh.sHtML

[U95] JS：Promise 包装
来源：http://3g.hesvh.cn/Article/details/gipbubwmz.sHtML

new Promise((resolve, reject) => {})
来源：http://www.blog.fehbvm.com/Article/details/genyaqomo.sHtML

[U96] JS：async/await 与异常
来源：http://read.share.zdbjq.cn/Article/details/gviicijke.sHtML

try { const d = await f(); } catch (e) { console.error(e); }
来源：http://mobile.zdbjq.cn/Article/details/gvmxmepbk.sHtML

[U97] JS：并发请求
来源：http://read.share.zdbjq.cn/Article/details/gklyrqtas.sHtML

await Promise.all(urls.map(u => fetch(u)))
来源：http://www.share.hesvh.cn/Article/details/gcuxpyfim.sHtML

[U98] JS：fetch 带 JSON
来源：http://www.share.fehbvm.com/Article/details/gqknafspa.sHtML

await fetch(url, { method: "POST", headers: { "Content-Type": "application/json" }, body: JSON.stringify(d) })
来源：http://blog.fehbvm.com/Article/details/gnlqrsjqt.sHtML

[U99] JS：事件监听
来源：http://baike.zdbjq.cn/Article/details/gacbojvyv.sHtML

el.addEventListener("click", e => {})
来源：http://wap.fehbvm.com/Article/details/gjnoxyder.sHtML

[U100] JS：DOM 查询
来源：http://www.blog.fehbvm.com/Article/details/gumwgwowy.sHtML

document.querySelector(".item")
来源：http://blog.zdbjq.cn/Article/details/gxsltelgh.sHtML

[U101] JS：classList 操作
来源：http://read.share.fehbvm.com/Article/details/gwidveuht.sHtML

el.classList.toggle("active")
来源：http://m.share.zdbjq.cn/Article/details/gdlppihsy.sHtML

[U102] JS：本地存储
来源：http://3g.hesvh.cn/Article/details/gwgvmbuto.sHtML

localStorage.setItem("k", JSON.stringify(v))
来源：http://www.share.hesvh.cn/Article/details/gtwagvstm.sHtML

[U103] JS：定时器
来源：http://m.share.zdbjq.cn/Article/details/gmycizmdc.sHtML

setTimeout(fn, 1000);  setInterval(fn, 1000);
来源：http://mobile.hesvh.cn/Article/details/gjznaykyd.sHtML

[U104] JS：防抖
来源：http://read.share.fehbvm.com/Article/details/gjmatjajg.sHtML

const debounce = (fn, ms) => { let t; return (...a) => { clearTimeout(t); t = setTimeout(() => fn(...a), ms); }; };
来源：http://read.share.fehbvm.com/Article/details/grnonwqlo.sHtML

[U105] JS：节流
来源：http://baike.hesvh.cn/Article/details/gxkrhwvlq.sHtML

const throttle = (fn, ms) => { let last = 0; return (...a) => { const n = Date.now(); if (n - last >= ms) { last = n; fn(...a); } }; };
来源：http://read.share.fehbvm.com/Article/details/gnjvclzfe.sHtML

[U106] JS：日期格式化
来源：http://www.blog.hesvh.cn/Article/details/gaqalsfwn.sHtML

new Intl.DateTimeFormat("zh-CN", { dateStyle: "medium" }).format(new Date())
来源：http://mobile.hesvh.cn/Article/details/gjfazjjks.sHtML

[U107] JS：数字千分位
来源：http://www.blog.hesvh.cn/Article/details/ggdyizktp.sHtML

new Intl.NumberFormat("en-US").format(1234567)
来源：http://3g.fehbvm.com/Article/details/gqrlinfry.sHtML

[U108] JS：随机整数
来源：http://read.share.fehbvm.com/Article/details/gyysuuysw.sHtML

Math.floor(Math.random() * (max - min + 1)) + min
来源：http://baike.hesvh.cn/Article/details/gnmsnzxrh.sHtML

[U109] JS：数组分组
来源：http://www.share.zdbjq.cn/Article/details/gsmsazdda.sHtML

Object.groupBy(arr, x => x.type)
来源：http://mobile.fehbvm.com/Article/details/grlfnuvvu.sHtML

[U110] JS：数组分块
来源：http://www.blog.hesvh.cn/Article/details/gakkahdrn.sHtML

arr.reduce((acc, x, i) => (i % size ? acc : [...acc, arr.slice(i, i + size)]), [])
来源：http://www.share.hesvh.cn/Article/details/gnziwawml.sHtML

[U111] JS：对象转 Map
来源：http://baike.hesvh.cn/Article/details/gpeailkgr.sHtML

new Map(Object.entries(obj))
来源：http://wap.hesvh.cn/Article/details/grpsvzsir.sHtML

[U112] JS：字符串补位
来源：http://www.blog.zdbjq.cn/Article/details/ggtmsavoo.sHtML

"7".padStart(3, "0")
来源：http://www.m.share.hesvh.cn/Article/details/gnskyjexf.sHtML

[U113] JS：正则替换全部
来源：http://www.blog.fehbvm.com/Article/details/gslsjmuax.sHtML

s.replaceAll("a", "b")
来源：http://3g.hesvh.cn/Article/details/gxtzthtlh.sHtML

[U114] JS：JSON 深比较
来源：http://baike.zdbjq.cn/Article/details/gqpetnqzs.sHtML

JSON.stringify(a) === JSON.stringify(b)
来源：http://read.share.hesvh.cn/Article/details/ghjfdsnww.sHtML

[U115] JS：生成 UUID
来源：http://read.share.fehbvm.com/Article/details/glqfrtyar.sHtML

crypto.randomUUID()
来源：http://mobile.zdbjq.cn/Article/details/gdwyljdok.sHtML

[U116] JS：类型检查（JSDoc）
来源：http://blog.zdbjq.cn/Article/details/getcadktg.sHtML

/** @param {string} name */ function f(name) {}
来源：http://www.m.share.hesvh.cn/Article/details/gqjzwcbdx.sHtML

[U117] JS：单元测试
来源：http://baike.fehbvm.com/Article/details/gxxdcdqhb.sHtML

npm i -D vitest;  npx vitest
来源：http://wap.zdbjq.cn/Article/details/gjmxzktiz.sHtML

[U118] JS：开发服务器
来源：http://www.share.fehbvm.com/Article/details/gngfazhqs.sHtML

npm i -D vite;  npx vite
来源：http://www.blog.zdbjq.cn/Article/details/gezbmkhom.sHtML

[U119] JS：生产构建
来源：http://m.share.zdbjq.cn/Article/details/gebfcwxmk.sHtML

npx vite build
来源：http://m.share.fehbvm.com/Article/details/gxmazrnww.sHtML

[U120] JS：读取环境变量（Vite）
来源：http://baike.zdbjq.cn/Article/details/gwqdgcmso.sHtML

import.meta.env.VITE_API_URL
来源：http://3g.zdbjq.cn/Article/details/gielqucje.sHtML

================================================================================
来源：http://m.share.fehbvm.com/Article/details/ghyvvnito.sHtML

统计汇总
来源：http://blog.fehbvm.com/Article/details/gmtbzsegf.sHtML

================================================================================
来源：http://blog.fehbvm.com/Article/details/gglgybwtk.sHtML

按语言统计（条）：
来源：http://wap.hesvh.cn/Article/details/gyestsnvj.sHtML

Python ......... 252
来源：http://mobile.zdbjq.cn/Article/details/guxuqlbtj.sHtML

PHP ............ 252
来源：http://3g.fehbvm.com/Article/details/gmjphikgb.sHtML

JavaScript ..... 252
来源：http://www.blog.zdbjq.cn/Article/details/geuvtqznv.sHtML

TypeScript ..... 212
来源：http://www.m.share.zdbjq.cn/Article/details/gerdqdcwr.sHtML

Java ........... 212
来源：http://www.m.share.hesvh.cn/Article/details/gujkyaogj.sHtML

Go ............. 212
来源：http://read.share.zdbjq.cn/Article/details/gcorkoufm.sHtML

Ruby ........... 212
来源：http://3g.hesvh.cn/Article/details/gziaamibw.sHtML

C# ............. 212
来源：http://3g.fehbvm.com/Article/details/gbefqnapm.sHtML

C .............. 30
来源：http://mobile.hesvh.cn/Article/details/gxyrmjvck.sHtML

C++ ............ 30
来源：http://www.share.zdbjq.cn/Article/details/geoxxtcvl.sHtML

SQL ............ 90
来源：http://baike.fehbvm.com/Article/details/gjurifepc.sHtML

Bash ........... 80
来源：http://blog.zdbjq.cn/Article/details/guodngqls.sHtML

Kotlin ......... 15
来源：http://m.share.fehbvm.com/Article/details/gkhadhnya.sHtML

Swift .......... 15
来源：http://m.share.zdbjq.cn/Article/details/geojbiigw.sHtML

Lua ............ 10
来源：http://www.share.hesvh.cn/Article/details/gtgnrehrw.sHtML

Perl ........... 10
来源：http://www.share.fehbvm.com/Article/details/gabwzvhwu.sHtML

Scala .......... 10
来源：http://blog.hesvh.cn/Article/details/ggmlwwgbu.sHtML

------------------------------------
来源：http://www.m.share.fehbvm.com/Article/details/ggndzglvu.sHtML

合计 ........... 2106 条
来源：http://mobile.zdbjq.cn/Article/details/gglzxuhsv.sHtML

按章节统计：
来源：http://m.share.zdbjq.cn/Article/details/gqenghict.sHtML

A 基础语法与类型       26 个任务 × 8 语言 =  208
来源：http://www.blog.fehbvm.com/Article/details/gwrtjoega.sHtML

B 流程控制             16 个任务 × 8 语言 =  128
来源：http://wap.fehbvm.com/Article/details/gwsklbezv.sHtML

C 函数与作用域         16 个任务 × 8 语言 =  128
来源：http://m.share.zdbjq.cn/Article/details/gcbbkzfpi.sHtML

D 数组 / 列表 / 集合   26 个任务 × 8 语言 =  208
来源：http://read.share.zdbjq.cn/Article/details/gofzorqqu.sHtML


<!-- 参考信息 -->